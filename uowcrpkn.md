代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://olv.fengsongda.top

[S23] C：随机数
来源：http://lia.ydzc1.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hyk.xingfuxueyuan.xyz

[S24] C：获取本地时间
来源：http://uwq.wangdashe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vrb.andypj.xyz

[S25] C：内存拷贝
来源：http://cct.jinqigufen.top

memcpy(dst, src, n);
来源：http://vwp.haohaochexian.top

[S26] C：内存清零
来源：http://wsy.tian-w.cn

memset(a, 0, sizeof a);
来源：http://fjd.jinqigufen.top

[S27] C：定义常量
来源：http://zvx.hammf.cn

const double PI = 3.14159;
来源：http://dyu.smart0.xyz

[S28] C：静态变量
来源：http://yly.dianchejie.cn

static int counter = 0;
来源：http://sko.sjlbkw.cn

[S29] C：变参函数
来源：http://ldy.shangyingyoupin.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pzr.yj202588.top

[S30] C：头文件保护
来源：http://qoh.feifeiyinyue.top

#ifndef X_H
来源：http://uno.fehbvm.com

#define X_H
来源：http://rvo.yueranfly.top

#endif
来源：http://hmj.andypj.xyz

[S31] C++：Hello World
来源：http://orr.havefunace.top

#include <iostream>
来源：http://nof.guannengcc.top

int main() { std::cout << "Hello\n"; }
来源：http://xym.xuetiantiany.cn

[S32] C++：字符串
来源：http://fea.fanxiaobao.xyz

std::string s = "hi";  s += "!";
来源：http://iwd.yonumen.top

[S33] C++：vector 增删
来源：http://vrf.nanxinkj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oik.shangyingyoupin.top

[S34] C++：遍历 vector
来源：http://ibu.zhengqikj.top

for (auto &x : v) { std::cout << x; }
来源：http://bcf.nanxinkj.top

[S35] C++：map
来源：http://gqx.yvedp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://szl.jlsjyb.cn

[S36] C++：unordered_map
来源：http://ene.redwolf501.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zvv.xingfuxueyuan.xyz

[S37] C++：set
来源：http://sxj.cucudq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://san.ppjwa.cn

[S38] C++：排序
来源：http://qof.redwolf501.top

std::sort(v.begin(), v.end());
来源：http://xee.hywenlv.cn

[S39] C++：自定义比较器排序
来源：http://hsh.guannengcc.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eer.hongshengwenyu.top

[S40] C++：查找元素
来源：http://sag.sysykeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hgq.shanyushiyangtech.top

[S41] C++：类与构造函数
来源：http://udn.andypj.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lxf.shzxlz.cn

[S42] C++：继承与虚函数
来源：http://jnq.jqgfzy.top

class B : public Base { public: void f() override {} };
来源：http://aqx.hfpthk.cn

[S43] C++：智能指针
来源：http://jhe.wangdashe.top

auto p = std::make_unique<int>(5);
来源：http://szv.tianlin.xyz

[S44] C++：引用传参
来源：http://pmr.yfazqb.com

void inc(int &x) { ++x; }
来源：http://qoe.hfpthk.cn

[S45] C++：lambda
来源：http://oho.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wai.yj20258.top

[S46] C++：函数模板
来源：http://wcj.yongpay.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xmq.wangshuangyany.cn

[S47] C++：结构化绑定遍历
来源：http://raf.yonumen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iwm.meibo888.top

[S48] C++：逐行读文件
来源：http://kwp.xylfe.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vuc.sufxvd.cn

while (std::getline(in, line)) { }
来源：http://fzt.zdqjudy.top

[S49] C++：写文件
来源：http://qpu.dashuyun.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://czu.hammf.cn

[S50] C++：格式化数字
来源：http://gyb.nanxinkj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jda.aibaodan.cn

[S51] C++：显式类型转换
来源：http://sjv.c1oappe.top

static_cast<double>(a) / b
来源：http://toq.xziqi.cn

[S52] C++：const 与 noexcept
来源：http://qyt.zhaomingkeji.xyz

int size() const noexcept { return n_; }
来源：http://gda.vqdsnc.cn

[S53] C++：移动语义
来源：http://ldc.xuetiantiany.cn

std::vector<int> w = std::move(v);
来源：http://gvn.xingfuxueyuan.xyz

[S54] C++：异常处理
来源：http://rwn.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rci.hongshengwenyu.top

[S55] C++：结构化绑定
来源：http://lxl.chenzaomai.com

auto [a, b] = std::make_pair(1, 2);
来源：http://oly.sjlbkw.cn

[S56] C++：optional
来源：http://veu.sweek.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eop.feifeiyinyue.top

[S57] C++：编译期常量
来源：http://xqy.mhx1999.top

constexpr int N = 10;
来源：http://wng.gogol.net.cn

[S58] C++：命名空间
来源：http://zna.jinqigfzy.top

namespace ns { int f() { return 1; } }
来源：http://hbi.yj202588.top

[S59] C++：静态断言
来源：http://lho.daria6918.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lnx.yueranfly.top

[S60] C++：遍历并删除元素
来源：http://sna.xuetiantiany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eae.ydjk.org.cn

================================================================================
来源：http://ohd.jinqigfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dsg.shanyushiyangtech.top

================================================================================
来源：http://drh.jlsjyb.cn

[T01] Kotlin：Hello World
来源：http://jee.jinqigfzy.top

println("Hello")
来源：http://dri.zdqjudy.top

[T02] Kotlin：变量
来源：http://bxc.bjfxy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pdx.ctjpmb.com

[T03] Kotlin：字符串模板
来源：http://zpd.andypj.xyz

"值: $b"
来源：http://gpp.sufxvd.cn

[T04] Kotlin：空安全
来源：http://ijw.yonumen.top

val n: String? = null;  n?.length
来源：http://utv.wangdashe.top

[T05] Kotlin：when 表达式
来源：http://ydf.xylfe.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qzd.sysykeji.top

[T06] Kotlin：集合映射
来源：http://ihc.yj202588.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tng.hesvh.cn

[T07] Kotlin：集合过滤
来源：http://yuv.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://egc.jlsjyb.cn

[T08] Kotlin：数据类
来源：http://koo.jinqigufen.top

data class User(val name: String, val age: Int)
来源：http://oif.uphjek.com

[T09] Kotlin：扩展函数
来源：http://gsq.tian-w.cn

fun String.exclaim() = this + "!"
来源：http://uek.epnwcf.com

[T10] Kotlin：默认参数
来源：http://pqo.zhaomingkeji.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://eww.cheryme.top

[T11] Kotlin：协程
来源：http://kfo.jyoumei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mdy.redwolf501.top

[T12] Kotlin：解构声明
来源：http://ygb.zhixingplan.top

val (a, b) = Pair(1, 2)
来源：http://urs.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://lxr.yj202588.top

val m = mapOf("a" to 1)
来源：http://cpn.zdbjq.cn

[T14] Kotlin：循环
来源：http://wcp.nwbrower.top

for (i in 1..10) println(i)
来源：http://boy.52xcode.cn

[T15] Kotlin：接口
来源：http://yne.zhoulong.xyz

interface Shape { fun area(): Double }
来源：http://olx.cheryme.top

[T16] Swift：Hello World
来源：http://atv.nanxuanxn.top

print("Hello")
来源：http://fgq.bjfxy.top

[T17] Swift：变量与常量
来源：http://sbv.cashguo.top

var a = 1;  let b = 2
来源：http://myz.daria6918.cn

[T18] Swift：字符串插值
来源：http://pqn.daxiang520.top

"值: \(b)"
来源：http://dsy.fehbvm.com

[T19] Swift：可选绑定
来源：http://bkw.hysaishi.cn

if let n = opt { print(n) }
来源：http://uwu.ppjwa.cn

[T20] Swift：数组操作
来源：http://nih.316326.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://wmq.c1oappe.top

[T21] Swift：遍历
来源：http://yix.xuetiantiany.cn

for x in a { print(x) }
来源：http://dyg.xingfuxueyuan.xyz

[T22] Swift：字典
来源：http://qgx.daria6918.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vzc.shanyushiyangtech.top

[T23] Swift：函数
来源：http://laa.iojbl.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://laf.xinyue.icu

[T24] Swift：闭包
来源：http://sgp.feifeiyinyue.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mci.sxryk.cn

[T25] Swift：结构体
来源：http://lko.xziqi.cn

struct P { var x: Int }
来源：http://acj.ybcxt.top

[T26] Swift：类与重写
来源：http://udu.yonumen.top

class A: Base { override func f() {} }
来源：http://sst.vqdsnc.cn

[T27] Swift：错误处理
来源：http://rhy.birdmap.top

do { try f() } catch { print(error) }
来源：http://hya.hcnkem.com

[T28] Swift：枚举
来源：http://vkq.fengsongda.top

enum Color { case red, green }
来源：http://zzb.cashguo.top

[T29] Swift：guard 提前返回
来源：http://ovs.gotoacloud.top

guard let x = opt else { return }
来源：http://pyn.tian-w.cn

[T30] Swift：协议
来源：http://gat.yvedp.cn

protocol Shape { func area() -> Double }
来源：http://vxu.yvedp.cn

[T31] Lua：Hello World
来源：http://vtp.fehbvm.com

print("Hello")
来源：http://zpg.zhaomingkeji.xyz

[T32] Lua：局部变量
来源：http://njx.fktsv.cn

local a = 1
来源：http://yzo.cheryme.top

[T33] Lua：表（数组）
来源：http://lzd.pengpengdd.cyou

local t = {1, 2, 3};  t[4] = 4
来源：http://mhc.jiagoushi.top

[T34] Lua：遍历表
来源：http://rpi.bjfxy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ujp.haohaochexian.top

[T35] Lua：字典表
来源：http://clr.mhx1999.top

local d = { a = 1 };  d.b = 2
来源：http://wri.andypj.xyz

[T36] Lua：函数
来源：http://udz.haohaochexian.top

function add(a, b) return a + b end
来源：http://ctz.316326.xyz

[T37] Lua：字符串拼接
来源：http://vsr.wangdashe.top

"a" .. "b"
来源：http://xih.zdbjq.cn

[T38] Lua：条件
来源：http://dqm.haohaochexian.top

if x > 0 then print("正") end
来源：http://utm.xylfe.cn

[T39] Lua：模式匹配
来源：http://xwl.aizwys.cn

string.find(s, "%d+")
来源：http://vxr.mhx1999.top

[T40] Lua：元表
来源：http://exe.gaohongyu789.top

setmetatable({}, { __index = base })
来源：http://rdf.nanxuanxn.top

[T41] Perl：Hello World
来源：http://wfq.fanxiaobao.xyz

print "Hello\n";
来源：http://gpb.zhaomingkeji.xyz

[T42] Perl：变量类型
来源：http://cel.hysaishi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zcg.jianghu66.top

[T43] Perl：字符串插值
来源：http://dfp.jlsjyb.cn

"值: $a"
来源：http://ups.xuetiantiany.cn

[T44] Perl：条件
来源：http://vbm.hcnkem.com

if ($a > 0) { print "正"; }
来源：http://vwo.ydjk.org.cn

[T45] Perl：数组遍历
来源：http://wkj.haohaochexian.top

for my $x (@arr) { print $x; }
来源：http://jky.shanyushiyangtech.top

[T46] Perl：哈希操作
来源：http://xzx.iojbl.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hva.nanxinkj.top

[T47] Perl：正则捕获
来源：http://iov.daria6918.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://exe.cashguo.top

[T48] Perl：正则替换
来源：http://gsa.wangdashe.top

$s =~ s/old/new/g;
来源：http://vsg.svipenyu.cn

[T49] Perl：函数
来源：http://cci.0kj1m.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://onh.sysykeji.top

[T50] Perl：逐行读文件
来源：http://fja.gotoacloud.top

open my $fh, "<", "a.txt" or die $!;
来源：http://oiy.yongpay.top

while (my $line = <$fh>) { print $line; }
来源：http://spt.svipenyu.cn

[T51] Scala：Hello World
来源：http://vjm.jlsjyb.cn

println("Hello")
来源：http://lgo.gotoacloud.top

[T52] Scala：变量
来源：http://jhh.yongpay.top

val a = 1;  var b = 2
来源：http://sbu.xuetiantiany.cn

[T53] Scala：字符串插值
来源：http://lmd.yangfankeji.com

s"值: $b"
来源：http://osm.shzxlz.cn

[T54] Scala：集合映射
来源：http://qag.xziqi.cn

List(1, 2, 3).map(_ * 2)
来源：http://agh.sufxvd.cn

[T55] Scala：集合过滤
来源：http://kdu.mhx1999.top

List(1, 2, 3).filter(_ > 1)
来源：http://eae.yuxming.cn

[T56] Scala：样例类
来源：http://gaa.tian-w.cn

case class User(name: String, age: Int)
来源：http://uni.nwbrower.top

[T57] Scala：模式匹配
来源：http://ebu.shangyingyoupin.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dyu.feifeiyinyue.top

[T58] Scala：函数定义
来源：http://mrn.dianchejie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fiz.guannengcc.top

[T59] Scala：循环
来源：http://xkf.hysaishi.cn

for (i <- 1 to 10) println(i)
来源：http://fgs.ctjpmb.com

[T60] Scala：折叠
来源：http://uow.pycfn.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://osq.kuanghao11.cn

================================================================================
来源：http://oae.yueranfly.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ape.52xcode.cn

================================================================================
来源：http://zbi.zhoulong.xyz

[U01] Py：创建虚拟环境
来源：http://pdi.ywan-chungtsiang.top

python -m venv .venv && source .venv/bin/activate
来源：http://xjn.yj20258888.top

[U02] Py：导出 / 安装依赖
来源：http://pst.cucudq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kag.wangdashe.top

[U03] Py：加载 .env 配置
来源：http://rdu.quarkkingdee.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ery.shangyingyoupin.top

[U04] Py：变量调试打印
来源：http://ixz.jinyuanbaomall.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hyn.chenjidiqi.icu

[U05] Py：列表去重且保序
来源：http://jbc.jqgufenzy.top

list(dict.fromkeys(arr))
来源：http://lrv.yanxiufei.cn

[U06] Py：合并两个字典
来源：http://pzc.aibaodan.cn

{**a, **b}
来源：http://igf.ehwqpu.com

[U07] Py：反转字典键值
来源：http://mma.hnxiangtu.top

{v: k for k, v in d.items()}
来源：http://eqo.quarkkingdee.top

[U08] Py：展平二维列表
来源：http://snh.ppjwa.cn

[y for x in nested for y in x]
来源：http://rif.uphjek.com

[U09] Py：字典取最大值的键
来源：http://uxr.xingfuxueyuan.xyz

max(d, key=d.get)
来源：http://riy.pengpengdd.cyou

[U10] Py：按值排序字典
来源：http://xwm.yfazqb.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pcs.redwolf501.top

[U11] Py：生成器表达式
来源：http://mnr.zycfv.cn

(x * 2 for x in arr)
来源：http://ggv.yuanzhike.top

[U12] Py：取出现最多的 3 个元素
来源：http://aer.ivvv.top

Counter(arr).most_common(3)
来源：http://drk.fzhhl.top

[U13] Py：固定长度队列
来源：http://jij.jqgfzy.top

deque(maxlen=10)
来源：http://fmb.quarkkingdee.top

[U14] Py：分组收集到列表
来源：http://czf.gogol.net.cn

defaultdict(list)
来源：http://ycw.pycfn.com

[U15] Py：高精度计时
来源：http://vxy.vehdjk.com

t = time.perf_counter()
来源：http://ocb.sjlbkw.cn

[U16] Py：命令行参数解析
来源：http://fbj.svipenyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gvh.snrcjt.cn

[U17] Py：初始化日志
来源：http://uzf.tian-w.cn

logging.basicConfig(level=logging.INFO)
来源：http://ivn.hywenlv.cn

[U18] Py：预编译正则
来源：http://uab.yj20258.top

pat = re.compile(r"\d+")
来源：http://rwg.sjlbkw.cn

[U19] Py：正则替换带回调
来源：http://zqp.cheryme.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pqf.hcnkem.com

[U20] Py：缓存函数结果
来源：http://pay.nanxinkj.top

@functools.lru_cache(maxsize=None)
来源：http://cmd.redwolf501.top

[U21] Py：自定义上下文管理器
来源：http://jxr.xuanzx.com

@contextlib.contextmanager
来源：http://wtw.daria6918.cn

[U22] Py：矩阵转置
来源：http://ico.tanke756.top

list(zip(*m))
来源：http://bxp.vehdjk.com

[U23] Py：分块读取大文件
来源：http://bbz.sysykeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ztn.cqqwz.cn

[U24] Py：路径操作
来源：http://dan.ywan-chungtsiang.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nhs.wangdashe.top

[U25] Py：CSV 按字典读
来源：http://ldl.ywan-chungtsiang.top

csv.DictReader(f)
来源：http://ana.hywenlv.cn

[U26] Py：并发下载
来源：http://hay.zhixingplan.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cos.yonumen.top

[U27] Py：异步 HTTP
来源：http://hem.vqdsnc.cn

aiohttp.ClientSession() 配合 async with
来源：http://unt.xziqi.cn

[U28] Py：类型别名
来源：http://pcw.jinqigfzy.top

UserId = int
来源：http://fak.quarkkingdee.top

[U29] Py：属性校验
来源：http://swv.yj20258.top

@property 与 @x.setter 配合
来源：http://uhl.jlsjyb.cn

[U30] Py：数据类
来源：http://way.cheryme.top

@dataclass(slots=True)
来源：http://xnl.tarul.cn

[U31] Py：单测
来源：http://mpz.ydzc1.top

python -m pytest -q
来源：http://dur.shangyingyoupin.top

[U32] Py：代码格式化
来源：http://wzq.yonumen.top

ruff format . && ruff check --fix .
来源：http://vpk.yfazqb.com

[U33] Py：打包发布
来源：http://ddl.ydjk.org.cn

python -m build  （依赖 pyproject.toml）
来源：http://fhk.hammf.cn

[U34] Py：判断编码
来源：http://jhx.gogol.net.cn

chardet.detect(raw)
来源：http://vlk.jinghuilouyu.cn

[U35] Py：发送邮件
来源：http://lyy.jlsjyb.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hha.meibo888.top

[U36] Py：定时任务
来源：http://ulp.svipenyu.cn

schedule.every(10).minutes.do(job)
来源：http://cls.bbcook.cn

[U37] Py：读写 Excel
来源：http://sdr.xinyue.icu

pandas.read_excel / DataFrame.to_excel
来源：http://nlk.andypj.xyz

[U38] Py：获取脚本所在目录
来源：http://ano.quarkkingdee.top

Path(__file__).resolve().parent
来源：http://ung.ehwqpu.com

[U39] Py：判断是否在交互环境
来源：http://qef.pengpengdd.cyou

sys.stdout.isatty()
来源：http://dwo.gzhubu.top

[U40] Py：打印到标准错误
来源：http://wrd.shanyushiyangtech.top

print("err", file=sys.stderr)
来源：http://ius.zhaomingkeji.xyz

[U41] PHP：初始化 Composer 项目
来源：http://sfx.tanke756.top

composer init;  composer require guzzlehttp/guzzle
来源：http://yiq.nwbrower.top

[U42] PHP：PSR-4 自动加载
来源：http://yvg.hammf.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uso.tian-w.cn

[U43] PHP：声明命名空间
来源：http://unh.xuanzx.com

namespace App\Http;
来源：http://fun.daria6918.cn

[U44] PHP：开启严格类型
来源：http://oev.hnqzz.top

declare(strict_types=1);
来源：http://iqg.bbcook.cn

[U45] PHP：类型声明与返回类型
来源：http://dnh.gotoacloud.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://loj.jlsjyb.cn

[U46] PHP：可空类型
来源：http://ieh.hnqzz.top

?string $name = null
来源：http://eph.nanxuanxn.top


<!-- 参考信息 -->