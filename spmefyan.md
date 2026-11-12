代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://enw.vqdsnc.cn

[S23] C：随机数
来源：http://kbv.xuetiantiany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xdj.bbcook.cn

[S24] C：获取本地时间
来源：http://top.ydzc1.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qtv.bbcook.cn

[S25] C：内存拷贝
来源：http://vcp.aizwys.cn

memcpy(dst, src, n);
来源：http://vdg.andypj.xyz

[S26] C：内存清零
来源：http://dfv.0kj1m.cn

memset(a, 0, sizeof a);
来源：http://xvs.yfazqb.com

[S27] C：定义常量
来源：http://fzf.fanxiaobao.xyz

const double PI = 3.14159;
来源：http://ihx.yvedp.cn

[S28] C：静态变量
来源：http://bpe.fktsv.cn

static int counter = 0;
来源：http://yie.xylfe.cn

[S29] C：变参函数
来源：http://wth.sweek.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bvx.bbcook.cn

[S30] C：头文件保护
来源：http://joi.jqgufenzy.top

#ifndef X_H
来源：http://fjx.tianlin.xyz

#define X_H
来源：http://tui.jinqigufen.top

#endif
来源：http://ypc.aibaodan.cn

[S31] C++：Hello World
来源：http://xkx.xuetiantiany.cn

#include <iostream>
来源：http://lao.fehbvm.com

int main() { std::cout << "Hello\n"; }
来源：http://dkz.quarkkingdee.top

[S32] C++：字符串
来源：http://usv.jqgfzy.top

std::string s = "hi";  s += "!";
来源：http://dlm.ehwqpu.com

[S33] C++：vector 增删
来源：http://jxh.yueranfly.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pdr.shanyushiyangtech.top

[S34] C++：遍历 vector
来源：http://mie.yuanzhike.top

for (auto &x : v) { std::cout << x; }
来源：http://drv.hnxiangtu.top

[S35] C++：map
来源：http://vwa.fzhhl.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qzl.sysykeji.top

[S36] C++：unordered_map
来源：http://rxu.ivvv.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mms.snrcjt.cn

[S37] C++：set
来源：http://fmo.fanxiaobao.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lsq.gzhubu.top

[S38] C++：排序
来源：http://xlf.jianghu66.top

std::sort(v.begin(), v.end());
来源：http://zjs.redwolf501.top

[S39] C++：自定义比较器排序
来源：http://own.xuanzx.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wxh.cqqwz.cn

[S40] C++：查找元素
来源：http://rsw.vehdjk.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zpm.quarkkingdee.top

[S41] C++：类与构造函数
来源：http://osu.xuanzx.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nhv.cqqwz.cn

[S42] C++：继承与虚函数
来源：http://lgp.wangshuangyany.cn

class B : public Base { public: void f() override {} };
来源：http://wpz.tianlin.xyz

[S43] C++：智能指针
来源：http://yoo.nanxuanxn.top

auto p = std::make_unique<int>(5);
来源：http://lav.bbcook.cn

[S44] C++：引用传参
来源：http://qyt.nanxuanxn.top

void inc(int &x) { ++x; }
来源：http://ixa.jiagoushi.top

[S45] C++：lambda
来源：http://nsh.shanyushiyangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://xgg.sjlbkw.cn

[S46] C++：函数模板
来源：http://vpk.ydjk.org.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fwm.shzxlz.cn

[S47] C++：结构化绑定遍历
来源：http://unc.fehbvm.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dca.fehbvm.com

[S48] C++：逐行读文件
来源：http://cjb.ydjk.org.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wyl.0kj1m.cn

while (std::getline(in, line)) { }
来源：http://iaq.hfpthk.cn

[S49] C++：写文件
来源：http://efu.yfazqb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ysi.hnqzz.top

[S50] C++：格式化数字
来源：http://hmt.hfpthk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nrc.yuanzhike.top

[S51] C++：显式类型转换
来源：http://zhg.ybcxt.top

static_cast<double>(a) / b
来源：http://apn.tianlin.xyz

[S52] C++：const 与 noexcept
来源：http://igm.jinqigufen.top

int size() const noexcept { return n_; }
来源：http://ksg.hysaishi.cn

[S53] C++：移动语义
来源：http://vcw.ydjk.org.cn

std::vector<int> w = std::move(v);
来源：http://jlk.52xcode.cn

[S54] C++：异常处理
来源：http://nny.yuanzhike.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yjr.shuidangran.top

[S55] C++：结构化绑定
来源：http://jcp.ydzc1.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pao.wangdashe.top

[S56] C++：optional
来源：http://utl.shuidangran.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vsd.haohaochexian.top

[S57] C++：编译期常量
来源：http://bms.xziqi.cn

constexpr int N = 10;
来源：http://rux.hywenlv.cn

[S58] C++：命名空间
来源：http://vtu.pycfn.com

namespace ns { int f() { return 1; } }
来源：http://fgj.nanxinkj.top

[S59] C++：静态断言
来源：http://yrk.yueranfly.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://btn.yj20258888.top

[S60] C++：遍历并删除元素
来源：http://qng.pycfn.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fsr.yvedp.cn

================================================================================
来源：http://ppi.yangfankeji.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lfd.nwbrower.top

================================================================================
来源：http://sky.tarul.cn

[T01] Kotlin：Hello World
来源：http://fbz.aizwys.cn

println("Hello")
来源：http://ifv.fzhhl.top

[T02] Kotlin：变量
来源：http://ppy.bjfxy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://irb.yj20258.top

[T03] Kotlin：字符串模板
来源：http://qxt.yongpay.top

"值: $b"
来源：http://pvn.tianlin.xyz

[T04] Kotlin：空安全
来源：http://oau.wangdashe.top

val n: String? = null;  n?.length
来源：http://nxd.chenzaomai.com

[T05] Kotlin：when 表达式
来源：http://mun.hfpthk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vsg.zhengqikj.top

[T06] Kotlin：集合映射
来源：http://kby.cqqwz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://won.dianchejie.cn

[T07] Kotlin：集合过滤
来源：http://oue.hnqzz.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ndd.ywan-chungtsiang.top

[T08] Kotlin：数据类
来源：http://dya.epnwcf.com

data class User(val name: String, val age: Int)
来源：http://say.xylfe.cn

[T09] Kotlin：扩展函数
来源：http://xtu.fehbvm.com

fun String.exclaim() = this + "!"
来源：http://wzd.fengsongda.top

[T10] Kotlin：默认参数
来源：http://utf.dianchejie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dbg.yuxming.cn

[T11] Kotlin：协程
来源：http://jlk.hcnkem.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://vrr.hnxiangtu.top

[T12] Kotlin：解构声明
来源：http://ibs.gzhubu.top

val (a, b) = Pair(1, 2)
来源：http://acm.pengpengdd.cyou

[T13] Kotlin：只读 Map
来源：http://ioo.ppjwa.cn

val m = mapOf("a" to 1)
来源：http://ppq.fktsv.cn

[T14] Kotlin：循环
来源：http://wez.jinghuilouyu.cn

for (i in 1..10) println(i)
来源：http://gxa.fengsongda.top

[T15] Kotlin：接口
来源：http://nrx.hesvh.cn

interface Shape { fun area(): Double }
来源：http://uet.ydzc1.top

[T16] Swift：Hello World
来源：http://krs.hcnkem.com

print("Hello")
来源：http://fcu.fzhhl.top

[T17] Swift：变量与常量
来源：http://bqw.hfpthk.cn

var a = 1;  let b = 2
来源：http://gpp.epnwcf.com

[T18] Swift：字符串插值
来源：http://uvs.uphjek.com

"值: \(b)"
来源：http://ore.c1oappe.top

[T19] Swift：可选绑定
来源：http://wpn.hongshengwenyu.top

if let n = opt { print(n) }
来源：http://hju.tanke756.top

[T20] Swift：数组操作
来源：http://gii.jqgufenzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://ces.jianghu66.top

[T21] Swift：遍历
来源：http://khl.havefunace.top

for x in a { print(x) }
来源：http://gvw.daria6918.cn

[T22] Swift：字典
来源：http://mrh.xuanzx.com

var d = ["a": 1];  d["b"] = 2
来源：http://xld.chenjidiqi.icu

[T23] Swift：函数
来源：http://wur.ctjpmb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dmj.hysaishi.cn

[T24] Swift：闭包
来源：http://xpk.ctjpmb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://ygv.xziqi.cn

[T25] Swift：结构体
来源：http://msj.gaohongyu789.top

struct P { var x: Int }
来源：http://fap.jinghuilouyu.cn

[T26] Swift：类与重写
来源：http://jtt.hnxiangtu.top

class A: Base { override func f() {} }
来源：http://axe.cheryme.top

[T27] Swift：错误处理
来源：http://xyo.hysaishi.cn

do { try f() } catch { print(error) }
来源：http://aas.chenjidiqi.icu

[T28] Swift：枚举
来源：http://ryo.sweek.top

enum Color { case red, green }
来源：http://uen.ydzc1.top

[T29] Swift：guard 提前返回
来源：http://jky.sysykeji.top

guard let x = opt else { return }
来源：http://yvo.ivvv.top

[T30] Swift：协议
来源：http://vtd.xuetiantiany.cn

protocol Shape { func area() -> Double }
来源：http://bnt.dashuyun.cn

[T31] Lua：Hello World
来源：http://yhs.mhx1999.top

print("Hello")
来源：http://haw.jiagoushi.top

[T32] Lua：局部变量
来源：http://snc.hfpthk.cn

local a = 1
来源：http://ygp.ydjk.org.cn

[T33] Lua：表（数组）
来源：http://qgl.ydjk.org.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gff.cheryme.top

[T34] Lua：遍历表
来源：http://mud.gotoacloud.top

for i, v in ipairs(t) do print(i, v) end
来源：http://olt.ehwqpu.com

[T35] Lua：字典表
来源：http://jjv.yfazqb.com

local d = { a = 1 };  d.b = 2
来源：http://pvf.ctjpmb.com

[T36] Lua：函数
来源：http://otl.jiagoushi.top

function add(a, b) return a + b end
来源：http://znh.hongshengwenyu.top

[T37] Lua：字符串拼接
来源：http://tar.ppjwa.cn

"a" .. "b"
来源：http://ram.xinyue.icu

[T38] Lua：条件
来源：http://zbw.uphjek.com

if x > 0 then print("正") end
来源：http://yfy.52xcode.cn

[T39] Lua：模式匹配
来源：http://mea.hnqzz.top

string.find(s, "%d+")
来源：http://nki.zhaomingkeji.xyz

[T40] Lua：元表
来源：http://bcu.cucudq.cn

setmetatable({}, { __index = base })
来源：http://kya.cucudq.cn

[T41] Perl：Hello World
来源：http://yud.hammf.cn

print "Hello\n";
来源：http://oob.jlsjyb.cn

[T42] Perl：变量类型
来源：http://jee.wangdashe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://byu.52xcode.cn

[T43] Perl：字符串插值
来源：http://gdj.tianlin.xyz

"值: $a"
来源：http://dlb.havefunace.top

[T44] Perl：条件
来源：http://ipu.chenjidiqi.icu

if ($a > 0) { print "正"; }
来源：http://vld.zdbjq.cn

[T45] Perl：数组遍历
来源：http://xmk.hcnkem.com

for my $x (@arr) { print $x; }
来源：http://coz.dashuyun.cn

[T46] Perl：哈希操作
来源：http://cmk.yongpay.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ryg.9152youxi.cn

[T47] Perl：正则捕获
来源：http://cir.cqqwz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gvu.jyoumei.cn

[T48] Perl：正则替换
来源：http://zvt.ybcxt.top

$s =~ s/old/new/g;
来源：http://awq.snrcjt.cn

[T49] Perl：函数
来源：http://ndv.yangfankeji.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mcq.shzxlz.cn

[T50] Perl：逐行读文件
来源：http://evk.uphjek.com

open my $fh, "<", "a.txt" or die $!;
来源：http://ria.yfazqb.com

while (my $line = <$fh>) { print $line; }
来源：http://bhq.ybcxt.top

[T51] Scala：Hello World
来源：http://sqv.shangyingyoupin.top

println("Hello")
来源：http://uys.fzhhl.top

[T52] Scala：变量
来源：http://ete.tanke756.top

val a = 1;  var b = 2
来源：http://jge.tian-w.cn

[T53] Scala：字符串插值
来源：http://fpo.cheryme.top

s"值: $b"
来源：http://vfo.fzhhl.top

[T54] Scala：集合映射
来源：http://tyc.ivvv.top

List(1, 2, 3).map(_ * 2)
来源：http://eqj.yj20258.top

[T55] Scala：集合过滤
来源：http://guo.bjfxy.top

List(1, 2, 3).filter(_ > 1)
来源：http://azs.guannengcc.top

[T56] Scala：样例类
来源：http://oqa.ppjwa.cn

case class User(name: String, age: Int)
来源：http://lvo.jqgfzy.top

[T57] Scala：模式匹配
来源：http://gds.yfazqb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://ext.uphjek.com

[T58] Scala：函数定义
来源：http://pob.kuanghao11.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gmr.tarul.cn

[T59] Scala：循环
来源：http://jjc.wangshuangyany.cn

for (i <- 1 to 10) println(i)
来源：http://bla.snrcjt.cn

[T60] Scala：折叠
来源：http://hwc.shzxlz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://juz.shanyushiyangtech.top

================================================================================
来源：http://esf.jinqigufen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nbk.guowangkeji.top

================================================================================
来源：http://zok.hnqzz.top

[U01] Py：创建虚拟环境
来源：http://kor.yueranfly.top

python -m venv .venv && source .venv/bin/activate
来源：http://djl.guowangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://ctl.ydzc1.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oce.cashguo.top

[U03] Py：加载 .env 配置
来源：http://cvh.wangdashe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ydk.hongshengwenyu.top

[U04] Py：变量调试打印
来源：http://edz.nanxinkj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gfk.ydjk.org.cn

[U05] Py：列表去重且保序
来源：http://mdz.xuetiantiany.cn

list(dict.fromkeys(arr))
来源：http://ypi.wangshuangyany.cn

[U06] Py：合并两个字典
来源：http://dko.chenzaomai.com

{**a, **b}
来源：http://oxb.9152youxi.cn

[U07] Py：反转字典键值
来源：http://jkk.zhixingplan.top

{v: k for k, v in d.items()}
来源：http://ite.shzxlz.cn

[U08] Py：展平二维列表
来源：http://xvv.c1oappe.top

[y for x in nested for y in x]
来源：http://azf.zhixingplan.top

[U09] Py：字典取最大值的键
来源：http://hwk.jlsjyb.cn

max(d, key=d.get)
来源：http://scf.guowangkeji.top

[U10] Py：按值排序字典
来源：http://gco.bbcook.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dhp.hammf.cn

[U11] Py：生成器表达式
来源：http://bko.jqgufenzy.top

(x * 2 for x in arr)
来源：http://hnr.hesvh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pgq.pycfn.com

Counter(arr).most_common(3)
来源：http://bec.chenjidiqi.icu

[U13] Py：固定长度队列
来源：http://lts.jlsjyb.cn

deque(maxlen=10)
来源：http://jju.fengsongda.top

[U14] Py：分组收集到列表
来源：http://zml.tianlin.xyz

defaultdict(list)
来源：http://oon.kuanghao11.cn

[U15] Py：高精度计时
来源：http://snc.nanxuanxn.top

t = time.perf_counter()
来源：http://ivl.sweek.top

[U16] Py：命令行参数解析
来源：http://nle.uphjek.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gcm.hnqzz.top

[U17] Py：初始化日志
来源：http://kjf.daxiang520.top

logging.basicConfig(level=logging.INFO)
来源：http://dut.0kj1m.cn

[U18] Py：预编译正则
来源：http://zuj.zhijiandao.cn

pat = re.compile(r"\d+")
来源：http://vgj.fzhhl.top

[U19] Py：正则替换带回调
来源：http://pjg.hnqzz.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nwz.sufxvd.cn

[U20] Py：缓存函数结果
来源：http://zia.fengsongda.top

@functools.lru_cache(maxsize=None)
来源：http://hwr.yuxming.cn

[U21] Py：自定义上下文管理器
来源：http://nvf.yueranfly.top

@contextlib.contextmanager
来源：http://wtd.ydjk.org.cn

[U22] Py：矩阵转置
来源：http://uyd.shzxlz.cn

list(zip(*m))
来源：http://ccr.zdbjq.cn

[U23] Py：分块读取大文件
来源：http://blb.hfpthk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://evr.gogol.net.cn

[U24] Py：路径操作
来源：http://zay.cashguo.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://spt.guowangkeji.top

[U25] Py：CSV 按字典读
来源：http://nhj.sxryk.cn

csv.DictReader(f)
来源：http://qmi.sysykeji.top

[U26] Py：并发下载
来源：http://nvq.jqgufenzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hqe.epnwcf.com

[U27] Py：异步 HTTP
来源：http://vft.cheryme.top

aiohttp.ClientSession() 配合 async with
来源：http://xjq.xziqi.cn

[U28] Py：类型别名
来源：http://dfq.yfazqb.com

UserId = int
来源：http://uyt.gotoacloud.top

[U29] Py：属性校验
来源：http://kzt.birdmap.top

@property 与 @x.setter 配合
来源：http://kqo.jinqigfzy.top

[U30] Py：数据类
来源：http://fhw.jinghuilouyu.cn

@dataclass(slots=True)
来源：http://hir.pycfn.com

[U31] Py：单测
来源：http://puk.pycfn.com

python -m pytest -q
来源：http://yzb.guannengcc.top

[U32] Py：代码格式化
来源：http://hdb.0kj1m.cn

ruff format . && ruff check --fix .
来源：http://qxy.smart0.xyz

[U33] Py：打包发布
来源：http://boz.zhoulong.xyz

python -m build  （依赖 pyproject.toml）
来源：http://wcb.jlsjyb.cn

[U34] Py：判断编码
来源：http://hao.nanxuanxn.top

chardet.detect(raw)
来源：http://hjk.cashguo.top

[U35] Py：发送邮件
来源：http://jwh.redwolf501.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sin.gogol.net.cn

[U36] Py：定时任务
来源：http://tyx.chenzaomai.com

schedule.every(10).minutes.do(job)
来源：http://tsr.meibo888.top

[U37] Py：读写 Excel
来源：http://avu.zhaomingkeji.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://iqn.hnqzz.top

[U38] Py：获取脚本所在目录
来源：http://deo.zhongyouzk.top

Path(__file__).resolve().parent
来源：http://wei.xuanzx.com

[U39] Py：判断是否在交互环境
来源：http://jug.chenzaomai.com

sys.stdout.isatty()
来源：http://ifp.hywenlv.cn

[U40] Py：打印到标准错误
来源：http://vda.pengpengdd.cyou

print("err", file=sys.stderr)
来源：http://ebx.hysaishi.cn

[U41] PHP：初始化 Composer 项目
来源：http://wvk.cheryme.top

composer init;  composer require guzzlehttp/guzzle
来源：http://dut.xziqi.cn

[U42] PHP：PSR-4 自动加载
来源：http://jzl.cheryme.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cax.mhx1999.top

[U43] PHP：声明命名空间
来源：http://pcg.gzhubu.top

namespace App\Http;
来源：http://aju.chenjidiqi.icu

[U44] PHP：开启严格类型
来源：http://iqc.jqgufenzy.top

declare(strict_types=1);
来源：http://bwu.bbcook.cn

[U45] PHP：类型声明与返回类型
来源：http://mhe.tian-w.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tys.xuanzx.com

[U46] PHP：可空类型
来源：http://ewg.sjlbkw.cn

?string $name = null
来源：http://ukq.xziqi.cn


<!-- 参考信息 -->