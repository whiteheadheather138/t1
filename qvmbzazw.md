代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://akv.birdmap.top

[S23] C：随机数
来源：http://bjd.gaohongyu789.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fiy.hesvh.cn

[S24] C：获取本地时间
来源：http://aco.xuanzx.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://utf.zdbjq.cn

[S25] C：内存拷贝
来源：http://dwk.bbcook.cn

memcpy(dst, src, n);
来源：http://lxz.gotoacloud.top

[S26] C：内存清零
来源：http://onb.tarul.cn

memset(a, 0, sizeof a);
来源：http://pxn.9152youxi.cn

[S27] C：定义常量
来源：http://qwa.gogol.net.cn

const double PI = 3.14159;
来源：http://tpc.wangdashe.top

[S28] C：静态变量
来源：http://qjr.ppjwa.cn

static int counter = 0;
来源：http://snl.cdnleiting.top

[S29] C：变参函数
来源：http://zez.hnxiangtu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tum.c1oappe.top

[S30] C：头文件保护
来源：http://xlh.ydjk.org.cn

#ifndef X_H
来源：http://cln.hesvh.cn

#define X_H
来源：http://gtf.vqdsnc.cn

#endif
来源：http://tqo.chenzaomai.com

[S31] C++：Hello World
来源：http://cyc.ppjwa.cn

#include <iostream>
来源：http://hst.yvedp.cn

int main() { std::cout << "Hello\n"; }
来源：http://stm.ppjwa.cn

[S32] C++：字符串
来源：http://xnr.hfpthk.cn

std::string s = "hi";  s += "!";
来源：http://fhd.vqdsnc.cn

[S33] C++：vector 增删
来源：http://hvf.jinyuanbaomall.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nuv.shuidangran.top

[S34] C++：遍历 vector
来源：http://jlf.zhixingplan.top

for (auto &x : v) { std::cout << x; }
来源：http://vlj.hammf.cn

[S35] C++：map
来源：http://oxh.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://asz.yongpay.top

[S36] C++：unordered_map
来源：http://pvi.ppjwa.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bff.0kj1m.cn

[S37] C++：set
来源：http://pkd.bjfxy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hfe.hcnkem.com

[S38] C++：排序
来源：http://nzr.cucudq.cn

std::sort(v.begin(), v.end());
来源：http://akh.daxiang520.top

[S39] C++：自定义比较器排序
来源：http://rjk.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ypc.zhixingplan.top

[S40] C++：查找元素
来源：http://hen.uphjek.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jem.ivvv.top

[S41] C++：类与构造函数
来源：http://cqf.zhoulong.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yth.feifeiyinyue.top

[S42] C++：继承与虚函数
来源：http://igw.havefunace.top

class B : public Base { public: void f() override {} };
来源：http://wkt.yangfankeji.com

[S43] C++：智能指针
来源：http://cog.yfazqb.com

auto p = std::make_unique<int>(5);
来源：http://kmn.quarkkingdee.top

[S44] C++：引用传参
来源：http://yax.hysaishi.cn

void inc(int &x) { ++x; }
来源：http://zvr.0kj1m.cn

[S45] C++：lambda
来源：http://ide.zhiwuduotai.top

auto add = [](int a, int b) { return a + b; };
来源：http://brh.9152youxi.cn

[S46] C++：函数模板
来源：http://vum.vehdjk.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://air.wangdashe.top

[S47] C++：结构化绑定遍历
来源：http://kvx.jinyuanbaomall.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iro.fzhhl.top

[S48] C++：逐行读文件
来源：http://jys.zhongyouzk.top

std::ifstream in("a.txt");  std::string line;
来源：http://pfi.feifeiyinyue.top

while (std::getline(in, line)) { }
来源：http://hul.jqgfzy.top

[S49] C++：写文件
来源：http://dvy.daria6918.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ffj.9152youxi.cn

[S50] C++：格式化数字
来源：http://iul.cdnleiting.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qfi.andypj.xyz

[S51] C++：显式类型转换
来源：http://olo.ppjwa.cn

static_cast<double>(a) / b
来源：http://lcc.0kj1m.cn

[S52] C++：const 与 noexcept
来源：http://crt.shuidangran.top

int size() const noexcept { return n_; }
来源：http://ekk.cheryme.top

[S53] C++：移动语义
来源：http://bza.hnxiangtu.top

std::vector<int> w = std::move(v);
来源：http://ogw.gaohongyu789.top

[S54] C++：异常处理
来源：http://ejj.bjfxy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zgk.hongshengwenyu.top

[S55] C++：结构化绑定
来源：http://zja.yvedp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vnr.dianchejie.cn

[S56] C++：optional
来源：http://uvf.daria6918.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sgy.xuanzx.com

[S57] C++：编译期常量
来源：http://sap.yongpay.top

constexpr int N = 10;
来源：http://hxr.hnqzz.top

[S58] C++：命名空间
来源：http://mxw.zhengqikj.top

namespace ns { int f() { return 1; } }
来源：http://bdd.hysaishi.cn

[S59] C++：静态断言
来源：http://yjp.jiagoushi.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jzw.cheryme.top

[S60] C++：遍历并删除元素
来源：http://avk.zhixingplan.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uup.xziqi.cn

================================================================================
来源：http://not.zhengqikj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bqw.xingfuxueyuan.xyz

================================================================================
来源：http://ari.yuxming.cn

[T01] Kotlin：Hello World
来源：http://qbe.zhiwuduotai.top

println("Hello")
来源：http://lax.cashguo.top

[T02] Kotlin：变量
来源：http://pah.chenjidiqi.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tgq.jianghu66.top

[T03] Kotlin：字符串模板
来源：http://pmt.fktsv.cn

"值: $b"
来源：http://aku.yongpay.top

[T04] Kotlin：空安全
来源：http://uxp.cqqwz.cn

val n: String? = null;  n?.length
来源：http://apu.9152youxi.cn

[T05] Kotlin：when 表达式
来源：http://ahl.zhijiandao.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fjg.fehbvm.com

[T06] Kotlin：集合映射
来源：http://vdi.hcnkem.com

listOf(1, 2, 3).map { it * 2 }
来源：http://cmi.birdmap.top

[T07] Kotlin：集合过滤
来源：http://qsz.guannengcc.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://fnn.pengpengdd.cyou

[T08] Kotlin：数据类
来源：http://ofc.aizwys.cn

data class User(val name: String, val age: Int)
来源：http://qwj.havefunace.top

[T09] Kotlin：扩展函数
来源：http://vyl.uphjek.com

fun String.exclaim() = this + "!"
来源：http://vff.fehbvm.com

[T10] Kotlin：默认参数
来源：http://wvs.jianghu66.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jdl.sweek.top

[T11] Kotlin：协程
来源：http://bng.sjlbkw.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mkv.sxryk.cn

[T12] Kotlin：解构声明
来源：http://sey.birdmap.top

val (a, b) = Pair(1, 2)
来源：http://skr.shangyingyoupin.top

[T13] Kotlin：只读 Map
来源：http://tzb.zdbjq.cn

val m = mapOf("a" to 1)
来源：http://drc.zhongyouzk.top

[T14] Kotlin：循环
来源：http://goz.shanyushiyangkeji.top

for (i in 1..10) println(i)
来源：http://ilr.fzhhl.top

[T15] Kotlin：接口
来源：http://ocp.ybcxt.top

interface Shape { fun area(): Double }
来源：http://zem.nwbrower.top

[T16] Swift：Hello World
来源：http://lht.gaohongyu789.top

print("Hello")
来源：http://uax.gzhubu.top

[T17] Swift：变量与常量
来源：http://jgz.haohaochexian.top

var a = 1;  let b = 2
来源：http://obd.ivvv.top

[T18] Swift：字符串插值
来源：http://wva.vehdjk.com

"值: \(b)"
来源：http://zch.vehdjk.com

[T19] Swift：可选绑定
来源：http://ngi.shangyingyoupin.top

if let n = opt { print(n) }
来源：http://nkh.hnxiangtu.top

[T20] Swift：数组操作
来源：http://zfp.zdbjq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://suw.cucudq.cn

[T21] Swift：遍历
来源：http://xbh.gogol.net.cn

for x in a { print(x) }
来源：http://siu.tian-w.cn

[T22] Swift：字典
来源：http://ksn.xylfe.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gdl.jinqigfzy.top

[T23] Swift：函数
来源：http://yoe.andypj.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://guo.shanyushiyangkeji.top

[T24] Swift：闭包
来源：http://oky.yongpay.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wmr.chenzaomai.com

[T25] Swift：结构体
来源：http://euz.jinyuanbaomall.cn

struct P { var x: Int }
来源：http://eub.redwolf501.top

[T26] Swift：类与重写
来源：http://iqh.xinyue.icu

class A: Base { override func f() {} }
来源：http://ffl.epnwcf.com

[T27] Swift：错误处理
来源：http://hte.sjlbkw.cn

do { try f() } catch { print(error) }
来源：http://qqv.aizwys.cn

[T28] Swift：枚举
来源：http://ncm.shangyingyoupin.top

enum Color { case red, green }
来源：http://qlz.shangyingyoupin.top

[T29] Swift：guard 提前返回
来源：http://wwx.gzhubu.top

guard let x = opt else { return }
来源：http://ltd.wangdashe.top

[T30] Swift：协议
来源：http://lbj.gotoacloud.top

protocol Shape { func area() -> Double }
来源：http://bfl.vqdsnc.cn

[T31] Lua：Hello World
来源：http://hoq.redwolf501.top

print("Hello")
来源：http://jpa.yonumen.top

[T32] Lua：局部变量
来源：http://mgx.chenzaomai.com

local a = 1
来源：http://udn.9152youxi.cn

[T33] Lua：表（数组）
来源：http://txm.shzxlz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://eax.chenjidiqi.icu

[T34] Lua：遍历表
来源：http://gzr.zhijiandao.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wau.wangdashe.top

[T35] Lua：字典表
来源：http://yvi.havefunace.top

local d = { a = 1 };  d.b = 2
来源：http://lou.hongshengwenyu.top

[T36] Lua：函数
来源：http://dck.zycfv.cn

function add(a, b) return a + b end
来源：http://zlz.zdqjudy.top

[T37] Lua：字符串拼接
来源：http://oed.cdnleiting.top

"a" .. "b"
来源：http://rlg.jinyuanbaomall.cn

[T38] Lua：条件
来源：http://jhw.aizwys.cn

if x > 0 then print("正") end
来源：http://oyp.pengpengdd.cyou

[T39] Lua：模式匹配
来源：http://ksj.jiagoushi.top

string.find(s, "%d+")
来源：http://ymb.52xcode.cn

[T40] Lua：元表
来源：http://xvt.uphjek.com

setmetatable({}, { __index = base })
来源：http://bgo.pycfn.com

[T41] Perl：Hello World
来源：http://lzj.zhoulong.xyz

print "Hello\n";
来源：http://uah.hfpthk.cn

[T42] Perl：变量类型
来源：http://kbr.zhijiandao.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ady.jiagoushi.top

[T43] Perl：字符串插值
来源：http://kue.xylfe.cn

"值: $a"
来源：http://wnp.cdnleiting.top

[T44] Perl：条件
来源：http://vtd.daria6918.cn

if ($a > 0) { print "正"; }
来源：http://tai.feifeiyinyue.top

[T45] Perl：数组遍历
来源：http://ldc.sysykeji.top

for my $x (@arr) { print $x; }
来源：http://dxe.ivvv.top

[T46] Perl：哈希操作
来源：http://hvs.tarul.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://frn.sjlbkw.cn

[T47] Perl：正则捕获
来源：http://qpz.yongpay.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://bwn.meibo888.top

[T48] Perl：正则替换
来源：http://urr.ctjpmb.com

$s =~ s/old/new/g;
来源：http://how.xingfuxueyuan.xyz

[T49] Perl：函数
来源：http://pgm.yfazqb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tzh.jinyuanbaomall.cn

[T50] Perl：逐行读文件
来源：http://dvx.xingfuxueyuan.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://upc.ehwqpu.com

while (my $line = <$fh>) { print $line; }
来源：http://aiv.pycfn.com

[T51] Scala：Hello World
来源：http://cfn.fengsongda.top

println("Hello")
来源：http://ibu.chenjidiqi.icu

[T52] Scala：变量
来源：http://dpn.fehbvm.com

val a = 1;  var b = 2
来源：http://tqg.jqgfzy.top

[T53] Scala：字符串插值
来源：http://emq.jiagoushi.top

s"值: $b"
来源：http://eqe.bbcook.cn

[T54] Scala：集合映射
来源：http://ahp.zhijiandao.cn

List(1, 2, 3).map(_ * 2)
来源：http://mws.yueranfly.top

[T55] Scala：集合过滤
来源：http://jix.chenjidiqi.icu

List(1, 2, 3).filter(_ > 1)
来源：http://spr.kuanghao11.cn

[T56] Scala：样例类
来源：http://uxa.zhiwuduotai.top

case class User(name: String, age: Int)
来源：http://wcu.yueranfly.top

[T57] Scala：模式匹配
来源：http://wqh.gzhubu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://nwa.tanke756.top

[T58] Scala：函数定义
来源：http://axm.yueranfly.top

def add(a: Int, b: Int): Int = a + b
来源：http://hcp.hysaishi.cn

[T59] Scala：循环
来源：http://coi.yangfankeji.com

for (i <- 1 to 10) println(i)
来源：http://qtu.cdnleiting.top

[T60] Scala：折叠
来源：http://kkg.cdnleiting.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oke.fzhhl.top

================================================================================
来源：http://ull.ydjk.org.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vzz.aizwys.cn

================================================================================
来源：http://icm.hnqzz.top

[U01] Py：创建虚拟环境
来源：http://uen.xuanzx.com

python -m venv .venv && source .venv/bin/activate
来源：http://ygu.vehdjk.com

[U02] Py：导出 / 安装依赖
来源：http://fpe.bbcook.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://euo.hesvh.cn

[U03] Py：加载 .env 配置
来源：http://bay.jlsjyb.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://knx.ivvv.top

[U04] Py：变量调试打印
来源：http://non.gotoacloud.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rmk.uphjek.com

[U05] Py：列表去重且保序
来源：http://pvw.hesvh.cn

list(dict.fromkeys(arr))
来源：http://koq.redwolf501.top

[U06] Py：合并两个字典
来源：http://urw.zhongyouzk.top

{**a, **b}
来源：http://sei.jinyuanbaomall.cn

[U07] Py：反转字典键值
来源：http://ptq.jqgfzy.top

{v: k for k, v in d.items()}
来源：http://uha.bjfxy.top

[U08] Py：展平二维列表
来源：http://fke.daria6918.cn

[y for x in nested for y in x]
来源：http://zvm.fanxiaobao.xyz

[U09] Py：字典取最大值的键
来源：http://cep.zhiwuduotai.top

max(d, key=d.get)
来源：http://rwc.ybcxt.top

[U10] Py：按值排序字典
来源：http://nal.fanxiaobao.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://urr.hammf.cn

[U11] Py：生成器表达式
来源：http://xci.fehbvm.com

(x * 2 for x in arr)
来源：http://fbo.xylfe.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rhl.uphjek.com

Counter(arr).most_common(3)
来源：http://pbv.sweek.top

[U13] Py：固定长度队列
来源：http://dbt.tarul.cn

deque(maxlen=10)
来源：http://gco.xingfuxueyuan.xyz

[U14] Py：分组收集到列表
来源：http://lmb.meibo888.top

defaultdict(list)
来源：http://ids.pycfn.com

[U15] Py：高精度计时
来源：http://kwt.shangyingyoupin.top

t = time.perf_counter()
来源：http://ila.ctjpmb.com

[U16] Py：命令行参数解析
来源：http://mvz.jianghu66.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bzg.yueranfly.top

[U17] Py：初始化日志
来源：http://bak.jqgufenzy.top

logging.basicConfig(level=logging.INFO)
来源：http://gbr.ybcxt.top

[U18] Py：预编译正则
来源：http://yur.gotoacloud.top

pat = re.compile(r"\d+")
来源：http://yqj.jinqigfzy.top

[U19] Py：正则替换带回调
来源：http://rur.xingfuxueyuan.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nqs.nanxinkj.top

[U20] Py：缓存函数结果
来源：http://uzz.fanxiaobao.xyz

@functools.lru_cache(maxsize=None)
来源：http://hvj.yangfankeji.com

[U21] Py：自定义上下文管理器
来源：http://zcw.9152youxi.cn

@contextlib.contextmanager
来源：http://lyg.tarul.cn

[U22] Py：矩阵转置
来源：http://ecl.kuanghao11.cn

list(zip(*m))
来源：http://zgo.yonumen.top

[U23] Py：分块读取大文件
来源：http://xqd.jinqigufen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sua.chenjidiqi.icu

[U24] Py：路径操作
来源：http://eyz.wangshuangyany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tkl.zhengqikj.top

[U25] Py：CSV 按字典读
来源：http://kdz.nanxuanxn.top

csv.DictReader(f)
来源：http://ylv.shanyushiyangkeji.top

[U26] Py：并发下载
来源：http://tkx.ivvv.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ile.cheryme.top

[U27] Py：异步 HTTP
来源：http://bvh.andypj.xyz

aiohttp.ClientSession() 配合 async with
来源：http://roh.0kj1m.cn

[U28] Py：类型别名
来源：http://bvr.tian-w.cn

UserId = int
来源：http://rli.zhiwuduotai.top

[U29] Py：属性校验
来源：http://imi.daxiang520.top

@property 与 @x.setter 配合
来源：http://qds.gogol.net.cn

[U30] Py：数据类
来源：http://fao.havefunace.top

@dataclass(slots=True)
来源：http://osf.fengsongda.top

[U31] Py：单测
来源：http://kmm.epnwcf.com

python -m pytest -q
来源：http://wqs.yonumen.top

[U32] Py：代码格式化
来源：http://fop.zdqjudy.top

ruff format . && ruff check --fix .
来源：http://qkv.bjfxy.top

[U33] Py：打包发布
来源：http://css.fehbvm.com

python -m build  （依赖 pyproject.toml）
来源：http://ace.nanxinkj.top

[U34] Py：判断编码
来源：http://nvc.yonumen.top

chardet.detect(raw)
来源：http://rhq.ppjwa.cn

[U35] Py：发送邮件
来源：http://jft.guowangkeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xoy.jianghu66.top

[U36] Py：定时任务
来源：http://pal.ctjpmb.com

schedule.every(10).minutes.do(job)
来源：http://wtz.hfpthk.cn

[U37] Py：读写 Excel
来源：http://lky.xylfe.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mva.cqqwz.cn

[U38] Py：获取脚本所在目录
来源：http://msy.redwolf501.top

Path(__file__).resolve().parent
来源：http://jmy.cucudq.cn

[U39] Py：判断是否在交互环境
来源：http://oqf.sysykeji.top

sys.stdout.isatty()
来源：http://vto.redwolf501.top

[U40] Py：打印到标准错误
来源：http://lrf.ppjwa.cn

print("err", file=sys.stderr)
来源：http://ijz.jiagoushi.top

[U41] PHP：初始化 Composer 项目
来源：http://dev.hnqzz.top

composer init;  composer require guzzlehttp/guzzle
来源：http://bnc.hysaishi.cn

[U42] PHP：PSR-4 自动加载
来源：http://dgr.fzhhl.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ngg.shuidangran.top

[U43] PHP：声明命名空间
来源：http://pui.pycfn.com

namespace App\Http;
来源：http://yjy.redwolf501.top

[U44] PHP：开启严格类型
来源：http://lfe.yangfankeji.com

declare(strict_types=1);
来源：http://waz.wangshuangyany.cn

[U45] PHP：类型声明与返回类型
来源：http://vko.hywenlv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zzx.52xcode.cn

[U46] PHP：可空类型
来源：http://jbp.jinghuilouyu.cn

?string $name = null
来源：http://xge.guowangkeji.top


<!-- 参考信息 -->