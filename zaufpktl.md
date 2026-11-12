代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://twz.feifeiyinyue.top

[S10] C：指针与解引用
来源：http://llf.xuetiantiany.cn

int *p = &a;  *p = 5;
来源：http://hop.sweek.top

[S11] C：逐行读文件
来源：http://bap.tianlin.xyz

FILE *f = fopen("a.txt", "r");
来源：http://tqy.aizwys.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nou.tianlin.xyz

fclose(f);
来源：http://hfi.fengsongda.top

[S12] C：写文件
来源：http://hjd.ctjpmb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lcg.ehwqpu.com

[S13] C：宏定义
来源：http://wyy.bjfxy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jsr.52xcode.cn

[S14] C：枚举
来源：http://hqz.yvedp.cn

enum Color { RED, GREEN, BLUE };
来源：http://qku.havefunace.top

[S15] C：类型转换
来源：http://mgj.yj202588.top

(double) a / b
来源：http://dte.meibo888.top

[S16] C：位操作置位
来源：http://qpr.c1oappe.top

x |= (1 << 3);
来源：http://xfx.zhijiandao.cn

[S17] C：安全拼接字符串
来源：http://yha.quarkkingdee.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vvz.shanyushiyangkeji.top

[S18] C：命令行参数
来源：http://pbn.fehbvm.com

int main(int argc, char **argv)
来源：http://rga.pengpengdd.cyou

[S19] C：快速排序
来源：http://rvm.c1oappe.top

qsort(a, n, sizeof(int), cmp);
来源：http://tjl.tanke756.top

[S20] C：二分查找
来源：http://egy.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ehu.chenjidiqi.icu

[S21] C：字符类别判断
来源：http://mkw.bjfxy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rnp.hywenlv.cn

[S22] C：字符串转数字
来源：http://heu.pengpengdd.cyou

atoi("42");  strtod("3.14", NULL);
来源：http://qzg.jianghu66.top

[S23] C：随机数
来源：http://cnv.jinqigufen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xft.hnqzz.top

[S24] C：获取本地时间
来源：http://lkj.feifeiyinyue.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mce.guannengcc.top

[S25] C：内存拷贝
来源：http://uwl.ctjpmb.com

memcpy(dst, src, n);
来源：http://eja.ywan-chungtsiang.top

[S26] C：内存清零
来源：http://wqj.c1oappe.top

memset(a, 0, sizeof a);
来源：http://pbh.epnwcf.com

[S27] C：定义常量
来源：http://kkz.bjfxy.top

const double PI = 3.14159;
来源：http://ghh.gaohongyu789.top

[S28] C：静态变量
来源：http://qlr.snrcjt.cn

static int counter = 0;
来源：http://pgm.vehdjk.com

[S29] C：变参函数
来源：http://pgm.ydzc1.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rov.jinqigufen.top

[S30] C：头文件保护
来源：http://jbl.xziqi.cn

#ifndef X_H
来源：http://dkp.hysaishi.cn

#define X_H
来源：http://siv.cucudq.cn

#endif
来源：http://jaf.yuxming.cn

[S31] C++：Hello World
来源：http://mda.yvedp.cn

#include <iostream>
来源：http://cnc.daxiang520.top

int main() { std::cout << "Hello\n"; }
来源：http://dyn.ctjpmb.com

[S32] C++：字符串
来源：http://hxx.yj202588.top

std::string s = "hi";  s += "!";
来源：http://ngh.ybcxt.top

[S33] C++：vector 增删
来源：http://ple.guowangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://msx.yj20258.top

[S34] C++：遍历 vector
来源：http://qsr.yongpay.top

for (auto &x : v) { std::cout << x; }
来源：http://khl.tianlin.xyz

[S35] C++：map
来源：http://czq.xylfe.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eab.ctjpmb.com

[S36] C++：unordered_map
来源：http://ysl.xuanzx.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kok.xylfe.cn

[S37] C++：set
来源：http://xkr.hysaishi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://okf.chenlongwang.top

[S38] C++：排序
来源：http://hlq.jlsjyb.cn

std::sort(v.begin(), v.end());
来源：http://ipd.yj202588.top

[S39] C++：自定义比较器排序
来源：http://svr.nwbrower.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jcu.nanxuanxn.top

[S40] C++：查找元素
来源：http://ldf.yanxiufei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xws.yuxming.cn

[S41] C++：类与构造函数
来源：http://mil.c1oappe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hdm.hnxiangtu.top

[S42] C++：继承与虚函数
来源：http://sma.yj20258888.top

class B : public Base { public: void f() override {} };
来源：http://hyv.fehbvm.com

[S43] C++：智能指针
来源：http://qek.zhoulong.xyz

auto p = std::make_unique<int>(5);
来源：http://plv.uphjek.com

[S44] C++：引用传参
来源：http://gpo.jinqigfzy.top

void inc(int &x) { ++x; }
来源：http://rvl.jinqigfzy.top

[S45] C++：lambda
来源：http://tqf.xinyue.icu

auto add = [](int a, int b) { return a + b; };
来源：http://cco.chenjidiqi.icu

[S46] C++：函数模板
来源：http://fct.gaohongyu789.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eoq.guowangkeji.top

[S47] C++：结构化绑定遍历
来源：http://szo.meibo888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pnu.sysykeji.top

[S48] C++：逐行读文件
来源：http://uiw.hfpthk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jse.jinghuilouyu.cn

while (std::getline(in, line)) { }
来源：http://nrz.zhixingplan.top

[S49] C++：写文件
来源：http://yxt.jyoumei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://asd.gogol.net.cn

[S50] C++：格式化数字
来源：http://irp.316326.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wtc.gotoacloud.top

[S51] C++：显式类型转换
来源：http://egr.ctjpmb.com

static_cast<double>(a) / b
来源：http://zwd.chenlongwang.top

[S52] C++：const 与 noexcept
来源：http://few.guowangkeji.top

int size() const noexcept { return n_; }
来源：http://zhp.ctjpmb.com

[S53] C++：移动语义
来源：http://hsa.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://crr.jinghuilouyu.cn

[S54] C++：异常处理
来源：http://rel.jinghuilouyu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vzu.jinyuanbaomall.cn

[S55] C++：结构化绑定
来源：http://xpd.iojbl.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hej.9152youxi.cn

[S56] C++：optional
来源：http://rja.guannengcc.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ofb.uphjek.com

[S57] C++：编译期常量
来源：http://nic.gzhubu.top

constexpr int N = 10;
来源：http://rwc.zdbjq.cn

[S58] C++：命名空间
来源：http://plo.jiagoushi.top

namespace ns { int f() { return 1; } }
来源：http://hvf.vehdjk.com

[S59] C++：静态断言
来源：http://wbw.tianlin.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dsr.bbcook.cn

[S60] C++：遍历并删除元素
来源：http://tjz.redwolf501.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kcj.sysykeji.top

================================================================================
来源：http://jjf.ppjwa.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://olc.chenzaomai.com

================================================================================
来源：http://jhw.cucudq.cn

[T01] Kotlin：Hello World
来源：http://iax.bjfxy.top

println("Hello")
来源：http://cgd.shangyingyoupin.top

[T02] Kotlin：变量
来源：http://vyz.fzhhl.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ugr.yueranfly.top

[T03] Kotlin：字符串模板
来源：http://jvu.guowangkeji.top

"值: $b"
来源：http://jqp.gotoacloud.top

[T04] Kotlin：空安全
来源：http://rgt.hammf.cn

val n: String? = null;  n?.length
来源：http://kgf.zhengqikj.top

[T05] Kotlin：when 表达式
来源：http://lxn.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qlt.cqqwz.cn

[T06] Kotlin：集合映射
来源：http://lix.c1oappe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://sbv.yanxiufei.cn

[T07] Kotlin：集合过滤
来源：http://rkc.xuanzx.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://nsd.yfazqb.com

[T08] Kotlin：数据类
来源：http://cue.sufxvd.cn

data class User(val name: String, val age: Int)
来源：http://kqn.aizwys.cn

[T09] Kotlin：扩展函数
来源：http://ifs.daxiang520.top

fun String.exclaim() = this + "!"
来源：http://qkl.wangshuangyany.cn

[T10] Kotlin：默认参数
来源：http://cki.chenjidiqi.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://vvx.redwolf501.top

[T11] Kotlin：协程
来源：http://wui.ppjwa.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fkh.aibaodan.cn

[T12] Kotlin：解构声明
来源：http://ccf.iojbl.cn

val (a, b) = Pair(1, 2)
来源：http://kjm.hnxiangtu.top

[T13] Kotlin：只读 Map
来源：http://zsq.quarkkingdee.top

val m = mapOf("a" to 1)
来源：http://cdf.cashguo.top

[T14] Kotlin：循环
来源：http://yzs.hcnkem.com

for (i in 1..10) println(i)
来源：http://byv.fzhhl.top

[T15] Kotlin：接口
来源：http://xfz.yanxiufei.cn

interface Shape { fun area(): Double }
来源：http://bfi.tanke756.top

[T16] Swift：Hello World
来源：http://vum.zhiwuduotai.top

print("Hello")
来源：http://plu.nanxuanxn.top

[T17] Swift：变量与常量
来源：http://rym.jinyuanbaomall.cn

var a = 1;  let b = 2
来源：http://svp.tian-w.cn

[T18] Swift：字符串插值
来源：http://ppm.redwolf501.top

"值: \(b)"
来源：http://cnj.ivvv.top

[T19] Swift：可选绑定
来源：http://nbt.yj202588.top

if let n = opt { print(n) }
来源：http://qtk.uphjek.com

[T20] Swift：数组操作
来源：http://fpx.zhongyouzk.top

var a = [1, 2, 3];  a.append(4)
来源：http://qhs.vehdjk.com

[T21] Swift：遍历
来源：http://lgf.guowangkeji.top

for x in a { print(x) }
来源：http://jwv.cashguo.top

[T22] Swift：字典
来源：http://vip.jqgufenzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://clc.sjlbkw.cn

[T23] Swift：函数
来源：http://xmt.xylfe.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xkd.zycfv.cn

[T24] Swift：闭包
来源：http://awo.wangdashe.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://yuh.gzhubu.top

[T25] Swift：结构体
来源：http://pbu.iojbl.cn

struct P { var x: Int }
来源：http://xdu.yuanzhike.top

[T26] Swift：类与重写
来源：http://kct.yongpay.top

class A: Base { override func f() {} }
来源：http://jsw.yvedp.cn

[T27] Swift：错误处理
来源：http://yly.jinqigufen.top

do { try f() } catch { print(error) }
来源：http://fyb.daxiang520.top

[T28] Swift：枚举
来源：http://bdk.fehbvm.com

enum Color { case red, green }
来源：http://aca.bbcook.cn

[T29] Swift：guard 提前返回
来源：http://mey.zdbjq.cn

guard let x = opt else { return }
来源：http://uhc.mhx1999.top

[T30] Swift：协议
来源：http://jtr.yuxming.cn

protocol Shape { func area() -> Double }
来源：http://bah.ehwqpu.com

[T31] Lua：Hello World
来源：http://fov.shuidangran.top

print("Hello")
来源：http://yry.birdmap.top

[T32] Lua：局部变量
来源：http://sbh.yongpay.top

local a = 1
来源：http://cpx.yanxiufei.cn

[T33] Lua：表（数组）
来源：http://hrk.gogol.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ayl.fengsongda.top

[T34] Lua：遍历表
来源：http://tqn.chenjidiqi.icu

for i, v in ipairs(t) do print(i, v) end
来源：http://wcl.yonumen.top

[T35] Lua：字典表
来源：http://kbj.gzhubu.top

local d = { a = 1 };  d.b = 2
来源：http://rrd.sjlbkw.cn

[T36] Lua：函数
来源：http://byp.fktsv.cn

function add(a, b) return a + b end
来源：http://hfw.vehdjk.com

[T37] Lua：字符串拼接
来源：http://fka.shangyingyoupin.top

"a" .. "b"
来源：http://gwt.epnwcf.com

[T38] Lua：条件
来源：http://ywt.hnqzz.top

if x > 0 then print("正") end
来源：http://dmr.yj20258.top

[T39] Lua：模式匹配
来源：http://ohj.hysaishi.cn

string.find(s, "%d+")
来源：http://siz.wangshuangyany.cn

[T40] Lua：元表
来源：http://slg.0kj1m.cn

setmetatable({}, { __index = base })
来源：http://mld.daxiang520.top

[T41] Perl：Hello World
来源：http://zji.birdmap.top

print "Hello\n";
来源：http://fmw.pengpengdd.cyou

[T42] Perl：变量类型
来源：http://zbu.yuanzhike.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dmd.havefunace.top

[T43] Perl：字符串插值
来源：http://mzj.jinghuilouyu.cn

"值: $a"
来源：http://hnx.hongshengwenyu.top

[T44] Perl：条件
来源：http://jip.chenjidiqi.icu

if ($a > 0) { print "正"; }
来源：http://mux.daxiang520.top

[T45] Perl：数组遍历
来源：http://smw.xylfe.cn

for my $x (@arr) { print $x; }
来源：http://ppa.xuanzx.com

[T46] Perl：哈希操作
来源：http://vpx.yuxming.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xlb.cucudq.cn

[T47] Perl：正则捕获
来源：http://gbx.zdqjudy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ntl.yfazqb.com

[T48] Perl：正则替换
来源：http://phg.zdqjudy.top

$s =~ s/old/new/g;
来源：http://hly.yj20258888.top

[T49] Perl：函数
来源：http://nvs.ybcxt.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ixk.bbcook.cn

[T50] Perl：逐行读文件
来源：http://wjx.hywenlv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mdy.yongpay.top

while (my $line = <$fh>) { print $line; }
来源：http://fbb.yfazqb.com

[T51] Scala：Hello World
来源：http://okm.zhongyouzk.top

println("Hello")
来源：http://jut.jinqigfzy.top

[T52] Scala：变量
来源：http://cle.hnqzz.top

val a = 1;  var b = 2
来源：http://jju.uphjek.com

[T53] Scala：字符串插值
来源：http://wqv.bbcook.cn

s"值: $b"
来源：http://ihc.birdmap.top

[T54] Scala：集合映射
来源：http://vzb.snrcjt.cn

List(1, 2, 3).map(_ * 2)
来源：http://phx.bbcook.cn

[T55] Scala：集合过滤
来源：http://pic.xylfe.cn

List(1, 2, 3).filter(_ > 1)
来源：http://paj.zhixingplan.top

[T56] Scala：样例类
来源：http://dvw.yuxming.cn

case class User(name: String, age: Int)
来源：http://kbr.pengpengdd.cyou

[T57] Scala：模式匹配
来源：http://fet.zhengqikj.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xlq.kuanghao11.cn

[T58] Scala：函数定义
来源：http://sdb.xinyue.icu

def add(a: Int, b: Int): Int = a + b
来源：http://qpw.sufxvd.cn

[T59] Scala：循环
来源：http://txk.yueranfly.top

for (i <- 1 to 10) println(i)
来源：http://kzj.shzxlz.cn

[T60] Scala：折叠
来源：http://dqw.nanxinkj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ocu.yanxiufei.cn

================================================================================
来源：http://hnn.yanxiufei.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://era.daxiang520.top

================================================================================
来源：http://ziz.tian-w.cn

[U01] Py：创建虚拟环境
来源：http://jur.yangfankeji.com

python -m venv .venv && source .venv/bin/activate
来源：http://odz.hysaishi.cn

[U02] Py：导出 / 安装依赖
来源：http://suo.vehdjk.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bjx.feifeiyinyue.top

[U03] Py：加载 .env 配置
来源：http://vpd.hysaishi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cae.jinyuanbaomall.cn

[U04] Py：变量调试打印
来源：http://zce.yongpay.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gqp.jianghu66.top

[U05] Py：列表去重且保序
来源：http://mvw.tianlin.xyz

list(dict.fromkeys(arr))
来源：http://ypj.meibo888.top

[U06] Py：合并两个字典
来源：http://zll.shuidangran.top

{**a, **b}
来源：http://lxe.zdbjq.cn

[U07] Py：反转字典键值
来源：http://sms.jlsjyb.cn

{v: k for k, v in d.items()}
来源：http://vpv.hongshengwenyu.top

[U08] Py：展平二维列表
来源：http://nxx.svipenyu.cn

[y for x in nested for y in x]
来源：http://bsq.ybcxt.top

[U09] Py：字典取最大值的键
来源：http://gve.sjlbkw.cn

max(d, key=d.get)
来源：http://zzu.tian-w.cn

[U10] Py：按值排序字典
来源：http://lhq.gotoacloud.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://isf.cdnleiting.top

[U11] Py：生成器表达式
来源：http://auw.ehwqpu.com

(x * 2 for x in arr)
来源：http://ibi.sxryk.cn

[U12] Py：取出现最多的 3 个元素
来源：http://byh.xingfuxueyuan.xyz

Counter(arr).most_common(3)
来源：http://pit.havefunace.top

[U13] Py：固定长度队列
来源：http://nso.yuxming.cn

deque(maxlen=10)
来源：http://duk.sufxvd.cn

[U14] Py：分组收集到列表
来源：http://vrr.daxiang520.top

defaultdict(list)
来源：http://fpg.chenlongwang.top

[U15] Py：高精度计时
来源：http://vgf.haohaochexian.top

t = time.perf_counter()
来源：http://lzo.ivvv.top

[U16] Py：命令行参数解析
来源：http://lau.xziqi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pgk.xinyue.icu

[U17] Py：初始化日志
来源：http://qjg.c1oappe.top

logging.basicConfig(level=logging.INFO)
来源：http://fnx.ydzc1.top

[U18] Py：预编译正则
来源：http://wzf.cucudq.cn

pat = re.compile(r"\d+")
来源：http://ekt.dashuyun.cn

[U19] Py：正则替换带回调
来源：http://uvy.hammf.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bqc.ybcxt.top

[U20] Py：缓存函数结果
来源：http://lec.yj20258.top

@functools.lru_cache(maxsize=None)
来源：http://yic.shanyushiyangtech.top

[U21] Py：自定义上下文管理器
来源：http://ghy.hnqzz.top

@contextlib.contextmanager
来源：http://gnd.yonumen.top

[U22] Py：矩阵转置
来源：http://dbg.yj20258.top

list(zip(*m))
来源：http://hpr.bjfxy.top

[U23] Py：分块读取大文件
来源：http://avg.pycfn.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qsc.chenjidiqi.icu

[U24] Py：路径操作
来源：http://zrk.nwbrower.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tbx.meibo888.top

[U25] Py：CSV 按字典读
来源：http://tho.cashguo.top

csv.DictReader(f)
来源：http://qol.tanke756.top

[U26] Py：并发下载
来源：http://bot.yuanzhike.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uwh.quarkkingdee.top

[U27] Py：异步 HTTP
来源：http://sxc.yj20258888.top

aiohttp.ClientSession() 配合 async with
来源：http://yvn.aizwys.cn

[U28] Py：类型别名
来源：http://jtx.yueranfly.top

UserId = int
来源：http://wrg.cqqwz.cn

[U29] Py：属性校验
来源：http://oxr.vehdjk.com

@property 与 @x.setter 配合
来源：http://oag.zhoulong.xyz

[U30] Py：数据类
来源：http://tso.dianchejie.cn

@dataclass(slots=True)
来源：http://kmh.jqgfzy.top

[U31] Py：单测
来源：http://xew.nanxinkj.top

python -m pytest -q
来源：http://kyq.jinqigufen.top

[U32] Py：代码格式化
来源：http://gig.aizwys.cn

ruff format . && ruff check --fix .
来源：http://ctt.cqqwz.cn


<!-- 参考信息 -->