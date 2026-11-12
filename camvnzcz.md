代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ifx.chenjidiqi.icu

[S10] C：指针与解引用
来源：http://ivu.zdqjudy.top

int *p = &a;  *p = 5;
来源：http://kxc.aibaodan.cn

[S11] C：逐行读文件
来源：http://ywf.zhijiandao.cn

FILE *f = fopen("a.txt", "r");
来源：http://cqo.yj20258888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rkx.mhx1999.top

fclose(f);
来源：http://bfe.yj202588.top

[S12] C：写文件
来源：http://ovo.xuetiantiany.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xhb.tanke756.top

[S13] C：宏定义
来源：http://kxk.vqdsnc.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://axp.gzhubu.top

[S14] C：枚举
来源：http://bmd.yfazqb.com

enum Color { RED, GREEN, BLUE };
来源：http://mbz.vqdsnc.cn

[S15] C：类型转换
来源：http://iip.xylfe.cn

(double) a / b
来源：http://rvo.sysykeji.top

[S16] C：位操作置位
来源：http://lij.chenjidiqi.icu

x |= (1 << 3);
来源：http://ewr.hfpthk.cn

[S17] C：安全拼接字符串
来源：http://sfk.nwbrower.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://thg.ehwqpu.com

[S18] C：命令行参数
来源：http://rhe.cheryme.top

int main(int argc, char **argv)
来源：http://utj.uphjek.com

[S19] C：快速排序
来源：http://ccf.sysykeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://zbv.yongpay.top

[S20] C：二分查找
来源：http://wwo.birdmap.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oex.cdnleiting.top

[S21] C：字符类别判断
来源：http://yob.shanyushiyangtech.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mdc.yonumen.top

[S22] C：字符串转数字
来源：http://xrd.tarul.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yof.wangshuangyany.cn

[S23] C：随机数
来源：http://lbf.xingfuxueyuan.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://der.hfpthk.cn

[S24] C：获取本地时间
来源：http://vpa.tian-w.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oxp.cashguo.top

[S25] C：内存拷贝
来源：http://nox.sjlbkw.cn

memcpy(dst, src, n);
来源：http://taq.zycfv.cn

[S26] C：内存清零
来源：http://dly.svipenyu.cn

memset(a, 0, sizeof a);
来源：http://llh.kuanghao11.cn

[S27] C：定义常量
来源：http://mvm.zhiwuduotai.top

const double PI = 3.14159;
来源：http://nhu.haohaochexian.top

[S28] C：静态变量
来源：http://kdo.hysaishi.cn

static int counter = 0;
来源：http://iwx.xylfe.cn

[S29] C：变参函数
来源：http://qyl.jinqigfzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yxd.hcnkem.com

[S30] C：头文件保护
来源：http://usq.daria6918.cn

#ifndef X_H
来源：http://ydt.aizwys.cn

#define X_H
来源：http://hlx.snrcjt.cn

#endif
来源：http://cvm.xuanzx.com

[S31] C++：Hello World
来源：http://vhr.jinghuilouyu.cn

#include <iostream>
来源：http://bxf.vqdsnc.cn

int main() { std::cout << "Hello\n"; }
来源：http://znu.aizwys.cn

[S32] C++：字符串
来源：http://lis.gogol.net.cn

std::string s = "hi";  s += "!";
来源：http://olp.ehwqpu.com

[S33] C++：vector 增删
来源：http://eya.jinghuilouyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://roa.havefunace.top

[S34] C++：遍历 vector
来源：http://uth.svipenyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://pll.gotoacloud.top

[S35] C++：map
来源：http://swn.sufxvd.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sgs.316326.xyz

[S36] C++：unordered_map
来源：http://pmt.jiagoushi.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nlf.fanxiaobao.xyz

[S37] C++：set
来源：http://ujx.zhongyouzk.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://atl.ydzc1.top

[S38] C++：排序
来源：http://vpf.jinqigfzy.top

std::sort(v.begin(), v.end());
来源：http://sbp.aibaodan.cn

[S39] C++：自定义比较器排序
来源：http://max.bbcook.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dnp.ivvv.top

[S40] C++：查找元素
来源：http://hpv.sjlbkw.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hwq.jqgufenzy.top

[S41] C++：类与构造函数
来源：http://yqo.daria6918.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qdj.zhixingplan.top

[S42] C++：继承与虚函数
来源：http://tkg.jianghu66.top

class B : public Base { public: void f() override {} };
来源：http://lrm.dianchejie.cn

[S43] C++：智能指针
来源：http://jcv.gotoacloud.top

auto p = std::make_unique<int>(5);
来源：http://zto.gaohongyu789.top

[S44] C++：引用传参
来源：http://skd.fzhhl.top

void inc(int &x) { ++x; }
来源：http://mwd.tanke756.top

[S45] C++：lambda
来源：http://jbr.sweek.top

auto add = [](int a, int b) { return a + b; };
来源：http://ekl.uphjek.com

[S46] C++：函数模板
来源：http://rxz.0kj1m.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jdz.andypj.xyz

[S47] C++：结构化绑定遍历
来源：http://yrl.cdnleiting.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xcp.guannengcc.top

[S48] C++：逐行读文件
来源：http://kah.smart0.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://rjq.guannengcc.top

while (std::getline(in, line)) { }
来源：http://ojc.nanxinkj.top

[S49] C++：写文件
来源：http://lyw.aizwys.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wdb.jqgufenzy.top

[S50] C++：格式化数字
来源：http://ara.smart0.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sxn.wangdashe.top

[S51] C++：显式类型转换
来源：http://zxm.yuxming.cn

static_cast<double>(a) / b
来源：http://ffr.nanxinkj.top

[S52] C++：const 与 noexcept
来源：http://wyx.shuidangran.top

int size() const noexcept { return n_; }
来源：http://ega.haohaochexian.top

[S53] C++：移动语义
来源：http://qum.wangshuangyany.cn

std::vector<int> w = std::move(v);
来源：http://bsp.jianghu66.top

[S54] C++：异常处理
来源：http://uaa.sufxvd.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wji.aizwys.cn

[S55] C++：结构化绑定
来源：http://ero.sjlbkw.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qxw.tianlin.xyz

[S56] C++：optional
来源：http://lif.daria6918.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tcx.316326.xyz

[S57] C++：编译期常量
来源：http://nhr.jianghu66.top

constexpr int N = 10;
来源：http://ncf.tarul.cn

[S58] C++：命名空间
来源：http://bdx.aizwys.cn

namespace ns { int f() { return 1; } }
来源：http://ruv.kuanghao11.cn

[S59] C++：静态断言
来源：http://jxa.gotoacloud.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hkv.bjfxy.top

[S60] C++：遍历并删除元素
来源：http://xja.sysykeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sdj.iojbl.cn

================================================================================
来源：http://wac.cqqwz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mqd.zhengqikj.top

================================================================================
来源：http://sxc.yvedp.cn

[T01] Kotlin：Hello World
来源：http://pjz.nwbrower.top

println("Hello")
来源：http://lpj.zhixingplan.top

[T02] Kotlin：变量
来源：http://dex.cucudq.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ari.sufxvd.cn

[T03] Kotlin：字符串模板
来源：http://qnm.nwbrower.top

"值: $b"
来源：http://xst.haohaochexian.top

[T04] Kotlin：空安全
来源：http://vdo.shzxlz.cn

val n: String? = null;  n?.length
来源：http://nsi.gzhubu.top

[T05] Kotlin：when 表达式
来源：http://mhy.epnwcf.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ogt.0kj1m.cn

[T06] Kotlin：集合映射
来源：http://nlg.yj20258.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zcj.fengsongda.top

[T07] Kotlin：集合过滤
来源：http://avf.chenjidiqi.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://pzt.cheryme.top

[T08] Kotlin：数据类
来源：http://qiw.bbcook.cn

data class User(val name: String, val age: Int)
来源：http://pfe.shanyushiyangtech.top

[T09] Kotlin：扩展函数
来源：http://pig.feifeiyinyue.top

fun String.exclaim() = this + "!"
来源：http://uzb.hesvh.cn

[T10] Kotlin：默认参数
来源：http://tev.zhongyouzk.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jpc.52xcode.cn

[T11] Kotlin：协程
来源：http://gwk.zhaomingkeji.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://kqj.yangfankeji.com

[T12] Kotlin：解构声明
来源：http://krd.gzhubu.top

val (a, b) = Pair(1, 2)
来源：http://ngb.yvedp.cn

[T13] Kotlin：只读 Map
来源：http://mzi.fktsv.cn

val m = mapOf("a" to 1)
来源：http://ztx.pycfn.com

[T14] Kotlin：循环
来源：http://mog.pycfn.com

for (i in 1..10) println(i)
来源：http://yya.birdmap.top

[T15] Kotlin：接口
来源：http://uee.tianlin.xyz

interface Shape { fun area(): Double }
来源：http://uoe.zhaomingkeji.xyz

[T16] Swift：Hello World
来源：http://rzp.gaohongyu789.top

print("Hello")
来源：http://kot.xylfe.cn

[T17] Swift：变量与常量
来源：http://cnf.xuetiantiany.cn

var a = 1;  let b = 2
来源：http://qll.jyoumei.cn

[T18] Swift：字符串插值
来源：http://ebi.xylfe.cn

"值: \(b)"
来源：http://oyg.uphjek.com

[T19] Swift：可选绑定
来源：http://lqc.sxryk.cn

if let n = opt { print(n) }
来源：http://umi.wangdashe.top

[T20] Swift：数组操作
来源：http://yvr.hnqzz.top

var a = [1, 2, 3];  a.append(4)
来源：http://rjr.andypj.xyz

[T21] Swift：遍历
来源：http://ojb.9152youxi.cn

for x in a { print(x) }
来源：http://kki.dashuyun.cn

[T22] Swift：字典
来源：http://zqr.gotoacloud.top

var d = ["a": 1];  d["b"] = 2
来源：http://qpg.jyoumei.cn

[T23] Swift：函数
来源：http://jer.bbcook.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jzh.xingfuxueyuan.xyz

[T24] Swift：闭包
来源：http://bfo.tanke756.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://aud.cashguo.top

[T25] Swift：结构体
来源：http://scj.ehwqpu.com

struct P { var x: Int }
来源：http://fps.hcnkem.com

[T26] Swift：类与重写
来源：http://dxx.kuanghao11.cn

class A: Base { override func f() {} }
来源：http://djm.feifeiyinyue.top

[T27] Swift：错误处理
来源：http://rwj.jyoumei.cn

do { try f() } catch { print(error) }
来源：http://vdo.shanyushiyangkeji.top

[T28] Swift：枚举
来源：http://zes.havefunace.top

enum Color { case red, green }
来源：http://olv.sufxvd.cn

[T29] Swift：guard 提前返回
来源：http://qku.zdqjudy.top

guard let x = opt else { return }
来源：http://wul.xuetiantiany.cn

[T30] Swift：协议
来源：http://gxy.guowangkeji.top

protocol Shape { func area() -> Double }
来源：http://qjb.ppjwa.cn

[T31] Lua：Hello World
来源：http://xiz.cheryme.top

print("Hello")
来源：http://ztp.ybcxt.top

[T32] Lua：局部变量
来源：http://zie.jinghuilouyu.cn

local a = 1
来源：http://dxv.yj202588.top

[T33] Lua：表（数组）
来源：http://aew.jinyuanbaomall.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cbh.cqqwz.cn

[T34] Lua：遍历表
来源：http://zdr.sweek.top

for i, v in ipairs(t) do print(i, v) end
来源：http://dhl.tianlin.xyz

[T35] Lua：字典表
来源：http://rkg.xylfe.cn

local d = { a = 1 };  d.b = 2
来源：http://cwv.hnqzz.top

[T36] Lua：函数
来源：http://hgf.shanyushiyangtech.top

function add(a, b) return a + b end
来源：http://deo.jinghuilouyu.cn

[T37] Lua：字符串拼接
来源：http://rco.fzhhl.top

"a" .. "b"
来源：http://wxj.shzxlz.cn

[T38] Lua：条件
来源：http://jbk.yvedp.cn

if x > 0 then print("正") end
来源：http://xfj.andypj.xyz

[T39] Lua：模式匹配
来源：http://ckz.fehbvm.com

string.find(s, "%d+")
来源：http://eas.yangfankeji.com

[T40] Lua：元表
来源：http://jxy.iojbl.cn

setmetatable({}, { __index = base })
来源：http://hmg.yuxming.cn

[T41] Perl：Hello World
来源：http://xkj.zhijiandao.cn

print "Hello\n";
来源：http://upt.ydzc1.top

[T42] Perl：变量类型
来源：http://bja.zdbjq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gcv.hnxiangtu.top

[T43] Perl：字符串插值
来源：http://vst.vehdjk.com

"值: $a"
来源：http://cub.jyoumei.cn

[T44] Perl：条件
来源：http://anl.ydzc1.top

if ($a > 0) { print "正"; }
来源：http://mdw.xziqi.cn

[T45] Perl：数组遍历
来源：http://jhl.chenjidiqi.icu

for my $x (@arr) { print $x; }
来源：http://vwi.hammf.cn

[T46] Perl：哈希操作
来源：http://tfa.jinqigufen.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hus.zdqjudy.top

[T47] Perl：正则捕获
来源：http://rkf.zdbjq.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sdu.hnqzz.top

[T48] Perl：正则替换
来源：http://tri.bbcook.cn

$s =~ s/old/new/g;
来源：http://qrh.jqgfzy.top

[T49] Perl：函数
来源：http://ste.nanxinkj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://czd.jqgufenzy.top

[T50] Perl：逐行读文件
来源：http://ums.pycfn.com

open my $fh, "<", "a.txt" or die $!;
来源：http://mxo.jinyuanbaomall.cn

while (my $line = <$fh>) { print $line; }
来源：http://kqh.cheryme.top

[T51] Scala：Hello World
来源：http://wep.haohaochexian.top

println("Hello")
来源：http://ikk.xziqi.cn

[T52] Scala：变量
来源：http://nio.c1oappe.top

val a = 1;  var b = 2
来源：http://qiw.cqqwz.cn

[T53] Scala：字符串插值
来源：http://kyk.yj20258.top

s"值: $b"
来源：http://agg.52xcode.cn

[T54] Scala：集合映射
来源：http://jyj.hongshengwenyu.top

List(1, 2, 3).map(_ * 2)
来源：http://sjk.yonumen.top

[T55] Scala：集合过滤
来源：http://ezy.aibaodan.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vbi.xuetiantiany.cn

[T56] Scala：样例类
来源：http://shl.hnqzz.top

case class User(name: String, age: Int)
来源：http://uty.uphjek.com

[T57] Scala：模式匹配
来源：http://lzb.feifeiyinyue.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vpi.chenjidiqi.icu

[T58] Scala：函数定义
来源：http://xmo.wangshuangyany.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lle.hammf.cn

[T59] Scala：循环
来源：http://xxb.yanxiufei.cn

for (i <- 1 to 10) println(i)
来源：http://gmr.cqqwz.cn

[T60] Scala：折叠
来源：http://vqr.andypj.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://guw.c1oappe.top

================================================================================
来源：http://voj.zhijiandao.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zvb.ivvv.top

================================================================================
来源：http://dqr.daxiang520.top

[U01] Py：创建虚拟环境
来源：http://zxe.hywenlv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jqk.gogol.net.cn

[U02] Py：导出 / 安装依赖
来源：http://dqe.tianlin.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rmz.yvedp.cn

[U03] Py：加载 .env 配置
来源：http://hce.yueranfly.top

from dotenv import load_dotenv; load_dotenv()
来源：http://tbr.jqgfzy.top

[U04] Py：变量调试打印
来源：http://ncp.jqgufenzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kgk.quarkkingdee.top

[U05] Py：列表去重且保序
来源：http://fpt.yj20258888.top

list(dict.fromkeys(arr))
来源：http://ejy.yj20258.top

[U06] Py：合并两个字典
来源：http://oji.hywenlv.cn

{**a, **b}
来源：http://oho.quarkkingdee.top

[U07] Py：反转字典键值
来源：http://pph.yonumen.top

{v: k for k, v in d.items()}
来源：http://pup.ydjk.org.cn

[U08] Py：展平二维列表
来源：http://zer.yvedp.cn

[y for x in nested for y in x]
来源：http://qfv.cqqwz.cn

[U09] Py：字典取最大值的键
来源：http://okh.gogol.net.cn

max(d, key=d.get)
来源：http://iqk.wangshuangyany.cn

[U10] Py：按值排序字典
来源：http://pwj.epnwcf.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fij.zhijiandao.cn

[U11] Py：生成器表达式
来源：http://cvh.wangshuangyany.cn

(x * 2 for x in arr)
来源：http://qdq.52xcode.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vjm.ivvv.top

Counter(arr).most_common(3)
来源：http://brz.jiagoushi.top

[U13] Py：固定长度队列
来源：http://alh.vehdjk.com

deque(maxlen=10)
来源：http://pjb.sjlbkw.cn

[U14] Py：分组收集到列表
来源：http://lqk.shanyushiyangtech.top

defaultdict(list)
来源：http://pku.redwolf501.top

[U15] Py：高精度计时
来源：http://cbg.chenjidiqi.icu

t = time.perf_counter()
来源：http://nra.yuanzhike.top

[U16] Py：命令行参数解析
来源：http://zem.52xcode.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rug.bbcook.cn

[U17] Py：初始化日志
来源：http://ecc.zhengqikj.top

logging.basicConfig(level=logging.INFO)
来源：http://qul.hfpthk.cn

[U18] Py：预编译正则
来源：http://cma.ydjk.org.cn

pat = re.compile(r"\d+")
来源：http://cds.pycfn.com

[U19] Py：正则替换带回调
来源：http://ksr.nwbrower.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://utc.daxiang520.top

[U20] Py：缓存函数结果
来源：http://ode.jyoumei.cn

@functools.lru_cache(maxsize=None)
来源：http://gqm.aizwys.cn

[U21] Py：自定义上下文管理器
来源：http://ojn.svipenyu.cn

@contextlib.contextmanager
来源：http://drh.gaohongyu789.top

[U22] Py：矩阵转置
来源：http://rco.meibo888.top

list(zip(*m))
来源：http://hwg.hnqzz.top

[U23] Py：分块读取大文件
来源：http://cbg.xziqi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xlk.smart0.xyz

[U24] Py：路径操作
来源：http://wsi.sysykeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ujn.pycfn.com

[U25] Py：CSV 按字典读
来源：http://wrp.yongpay.top

csv.DictReader(f)
来源：http://qtq.hesvh.cn

[U26] Py：并发下载
来源：http://mig.hywenlv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ygm.hesvh.cn

[U27] Py：异步 HTTP
来源：http://its.jlsjyb.cn

aiohttp.ClientSession() 配合 async with
来源：http://kgr.shzxlz.cn

[U28] Py：类型别名
来源：http://qse.yanxiufei.cn

UserId = int
来源：http://ivi.pengpengdd.cyou

[U29] Py：属性校验
来源：http://arz.xuanzx.com

@property 与 @x.setter 配合
来源：http://mkg.ctjpmb.com

[U30] Py：数据类
来源：http://ema.52xcode.cn

@dataclass(slots=True)
来源：http://axn.vehdjk.com

[U31] Py：单测
来源：http://qdx.yj20258888.top

python -m pytest -q
来源：http://ine.zhaomingkeji.xyz

[U32] Py：代码格式化
来源：http://iiw.xuetiantiany.cn

ruff format . && ruff check --fix .
来源：http://sxq.ydjk.org.cn


<!-- 参考信息 -->