代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bwp.svipenyu.cn

[S10] C：指针与解引用
来源：http://pqi.hongshengwenyu.top

int *p = &a;  *p = 5;
来源：http://mxa.cashguo.top

[S11] C：逐行读文件
来源：http://tzi.chenzaomai.com

FILE *f = fopen("a.txt", "r");
来源：http://efr.snrcjt.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://eqy.iojbl.cn

fclose(f);
来源：http://wxp.bjfxy.top

[S12] C：写文件
来源：http://mzl.jianghu66.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://llt.jqgufenzy.top

[S13] C：宏定义
来源：http://bme.jyoumei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qmq.dashuyun.cn

[S14] C：枚举
来源：http://qfq.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://hcz.sxryk.cn

[S15] C：类型转换
来源：http://zva.ywan-chungtsiang.top

(double) a / b
来源：http://fkg.wangshuangyany.cn

[S16] C：位操作置位
来源：http://qsd.meibo888.top

x |= (1 << 3);
来源：http://qzz.xylfe.cn

[S17] C：安全拼接字符串
来源：http://gcj.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nbg.jqgufenzy.top

[S18] C：命令行参数
来源：http://mbf.xuetiantiany.cn

int main(int argc, char **argv)
来源：http://ffc.zdbjq.cn

[S19] C：快速排序
来源：http://gfb.daxiang520.top

qsort(a, n, sizeof(int), cmp);
来源：http://otm.zhengqikj.top

[S20] C：二分查找
来源：http://ndf.ydzc1.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://unn.haohaochexian.top

[S21] C：字符类别判断
来源：http://sxi.kuanghao11.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vlm.feifeiyinyue.top

[S22] C：字符串转数字
来源：http://atm.smart0.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://vyq.zdqjudy.top

[S23] C：随机数
来源：http://sjv.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bkh.yvedp.cn

[S24] C：获取本地时间
来源：http://hem.hammf.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mqg.fengsongda.top

[S25] C：内存拷贝
来源：http://kbm.nanxinkj.top

memcpy(dst, src, n);
来源：http://lys.jinyuanbaomall.cn

[S26] C：内存清零
来源：http://cwg.bjfxy.top

memset(a, 0, sizeof a);
来源：http://kzz.vehdjk.com

[S27] C：定义常量
来源：http://ubs.nwbrower.top

const double PI = 3.14159;
来源：http://cvk.tian-w.cn

[S28] C：静态变量
来源：http://fsz.cheryme.top

static int counter = 0;
来源：http://zoz.xziqi.cn

[S29] C：变参函数
来源：http://afy.feifeiyinyue.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zcf.zhixingplan.top

[S30] C：头文件保护
来源：http://pzd.sweek.top

#ifndef X_H
来源：http://jxh.hnqzz.top

#define X_H
来源：http://pjr.vehdjk.com

#endif
来源：http://oqy.jyoumei.cn

[S31] C++：Hello World
来源：http://fau.fehbvm.com

#include <iostream>
来源：http://cef.hesvh.cn

int main() { std::cout << "Hello\n"; }
来源：http://kjd.shangyingyoupin.top

[S32] C++：字符串
来源：http://bvu.andypj.xyz

std::string s = "hi";  s += "!";
来源：http://aiu.xinyue.icu

[S33] C++：vector 增删
来源：http://oeh.xuanzx.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wxa.fanxiaobao.xyz

[S34] C++：遍历 vector
来源：http://ufd.hysaishi.cn

for (auto &x : v) { std::cout << x; }
来源：http://cpp.fengsongda.top

[S35] C++：map
来源：http://gvb.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lvx.jinqigfzy.top

[S36] C++：unordered_map
来源：http://fcc.yj202588.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yea.xylfe.cn

[S37] C++：set
来源：http://ama.shuidangran.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://neu.jlsjyb.cn

[S38] C++：排序
来源：http://ziq.feifeiyinyue.top

std::sort(v.begin(), v.end());
来源：http://sll.shzxlz.cn

[S39] C++：自定义比较器排序
来源：http://hon.ydjk.org.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qhf.shangyingyoupin.top

[S40] C++：查找元素
来源：http://evm.zhongyouzk.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cuq.uphjek.com

[S41] C++：类与构造函数
来源：http://gkf.fanxiaobao.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ayw.316326.xyz

[S42] C++：继承与虚函数
来源：http://alp.yj20258.top

class B : public Base { public: void f() override {} };
来源：http://rwu.ydzc1.top

[S43] C++：智能指针
来源：http://gjt.jinqigfzy.top

auto p = std::make_unique<int>(5);
来源：http://hhe.jqgufenzy.top

[S44] C++：引用传参
来源：http://xvk.chenlongwang.top

void inc(int &x) { ++x; }
来源：http://afp.vqdsnc.cn

[S45] C++：lambda
来源：http://arm.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qsc.pengpengdd.cyou

[S46] C++：函数模板
来源：http://uuo.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pof.dianchejie.cn

[S47] C++：结构化绑定遍历
来源：http://lln.jiagoushi.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mqo.nanxuanxn.top

[S48] C++：逐行读文件
来源：http://thw.cdnleiting.top

std::ifstream in("a.txt");  std::string line;
来源：http://kxm.52xcode.cn

while (std::getline(in, line)) { }
来源：http://aco.xuanzx.com

[S49] C++：写文件
来源：http://jxd.shangyingyoupin.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zeq.sweek.top

[S50] C++：格式化数字
来源：http://wxd.fktsv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://heo.aibaodan.cn

[S51] C++：显式类型转换
来源：http://gxn.yj202588.top

static_cast<double>(a) / b
来源：http://fng.cdnleiting.top

[S52] C++：const 与 noexcept
来源：http://fta.wangdashe.top

int size() const noexcept { return n_; }
来源：http://nbk.hywenlv.cn

[S53] C++：移动语义
来源：http://vjx.jlsjyb.cn

std::vector<int> w = std::move(v);
来源：http://dzj.haohaochexian.top

[S54] C++：异常处理
来源：http://gmh.jinqigfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ycs.wangshuangyany.cn

[S55] C++：结构化绑定
来源：http://ziy.sysykeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vqk.chenjidiqi.icu

[S56] C++：optional
来源：http://aqw.sxryk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yyk.shuidangran.top

[S57] C++：编译期常量
来源：http://zfw.wangdashe.top

constexpr int N = 10;
来源：http://qma.hysaishi.cn

[S58] C++：命名空间
来源：http://qvu.sxryk.cn

namespace ns { int f() { return 1; } }
来源：http://vay.yj20258.top

[S59] C++：静态断言
来源：http://egu.shangyingyoupin.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dqk.chenjidiqi.icu

[S60] C++：遍历并删除元素
来源：http://qwc.xuanzx.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sbq.iojbl.cn

================================================================================
来源：http://rzz.jiagoushi.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sjn.tianlin.xyz

================================================================================
来源：http://enb.wangdashe.top

[T01] Kotlin：Hello World
来源：http://anw.daria6918.cn

println("Hello")
来源：http://xim.hnxiangtu.top

[T02] Kotlin：变量
来源：http://znx.shangyingyoupin.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dlr.hnxiangtu.top

[T03] Kotlin：字符串模板
来源：http://mjo.tarul.cn

"值: $b"
来源：http://ftn.nanxinkj.top

[T04] Kotlin：空安全
来源：http://mge.jqgufenzy.top

val n: String? = null;  n?.length
来源：http://ylx.shuidangran.top

[T05] Kotlin：when 表达式
来源：http://mal.yvedp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rge.fengsongda.top

[T06] Kotlin：集合映射
来源：http://qhr.hnxiangtu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://idx.redwolf501.top

[T07] Kotlin：集合过滤
来源：http://idb.pengpengdd.cyou

listOf(1, 2, 3).filter { it > 1 }
来源：http://vyf.jlsjyb.cn

[T08] Kotlin：数据类
来源：http://ukq.zhijiandao.cn

data class User(val name: String, val age: Int)
来源：http://fzs.guannengcc.top

[T09] Kotlin：扩展函数
来源：http://dvs.zhaomingkeji.xyz

fun String.exclaim() = this + "!"
来源：http://vfk.andypj.xyz

[T10] Kotlin：默认参数
来源：http://hcx.yvedp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vld.hongshengwenyu.top

[T11] Kotlin：协程
来源：http://vyp.havefunace.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://dbw.nanxinkj.top

[T12] Kotlin：解构声明
来源：http://dlw.shuidangran.top

val (a, b) = Pair(1, 2)
来源：http://xnt.yangfankeji.com

[T13] Kotlin：只读 Map
来源：http://cox.jyoumei.cn

val m = mapOf("a" to 1)
来源：http://reg.daxiang520.top

[T14] Kotlin：循环
来源：http://gub.jinqigfzy.top

for (i in 1..10) println(i)
来源：http://vic.yanxiufei.cn

[T15] Kotlin：接口
来源：http://maz.aizwys.cn

interface Shape { fun area(): Double }
来源：http://hsj.0kj1m.cn

[T16] Swift：Hello World
来源：http://wdm.nanxinkj.top

print("Hello")
来源：http://ftc.xuanzx.com

[T17] Swift：变量与常量
来源：http://iqw.yongpay.top

var a = 1;  let b = 2
来源：http://mbf.sxryk.cn

[T18] Swift：字符串插值
来源：http://byx.zhaomingkeji.xyz

"值: \(b)"
来源：http://mmd.haohaochexian.top

[T19] Swift：可选绑定
来源：http://ozf.gaohongyu789.top

if let n = opt { print(n) }
来源：http://xvi.ehwqpu.com

[T20] Swift：数组操作
来源：http://dws.xuetiantiany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ncg.hywenlv.cn

[T21] Swift：遍历
来源：http://srt.gzhubu.top

for x in a { print(x) }
来源：http://jhm.havefunace.top

[T22] Swift：字典
来源：http://ult.jinqigufen.top

var d = ["a": 1];  d["b"] = 2
来源：http://qac.jlsjyb.cn

[T23] Swift：函数
来源：http://wff.fzhhl.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pkv.tian-w.cn

[T24] Swift：闭包
来源：http://qli.guannengcc.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ixi.wangdashe.top

[T25] Swift：结构体
来源：http://vys.dianchejie.cn

struct P { var x: Int }
来源：http://vnz.dianchejie.cn

[T26] Swift：类与重写
来源：http://otq.yj20258.top

class A: Base { override func f() {} }
来源：http://bak.yj20258888.top

[T27] Swift：错误处理
来源：http://mip.svipenyu.cn

do { try f() } catch { print(error) }
来源：http://snv.redwolf501.top

[T28] Swift：枚举
来源：http://kjy.cheryme.top

enum Color { case red, green }
来源：http://rcn.aibaodan.cn

[T29] Swift：guard 提前返回
来源：http://aln.snrcjt.cn

guard let x = opt else { return }
来源：http://gxr.gzhubu.top

[T30] Swift：协议
来源：http://gyv.havefunace.top

protocol Shape { func area() -> Double }
来源：http://axf.aizwys.cn

[T31] Lua：Hello World
来源：http://xhn.iojbl.cn

print("Hello")
来源：http://tyl.hesvh.cn

[T32] Lua：局部变量
来源：http://uxe.yueranfly.top

local a = 1
来源：http://gcv.jqgufenzy.top

[T33] Lua：表（数组）
来源：http://kdx.yvedp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zso.fzhhl.top

[T34] Lua：遍历表
来源：http://rfh.dianchejie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qve.zhaomingkeji.xyz

[T35] Lua：字典表
来源：http://cjg.316326.xyz

local d = { a = 1 };  d.b = 2
来源：http://tcn.zhixingplan.top

[T36] Lua：函数
来源：http://jrg.cqqwz.cn

function add(a, b) return a + b end
来源：http://qfk.cucudq.cn

[T37] Lua：字符串拼接
来源：http://zrz.shanyushiyangkeji.top

"a" .. "b"
来源：http://hng.ivvv.top

[T38] Lua：条件
来源：http://gry.cqqwz.cn

if x > 0 then print("正") end
来源：http://lbz.hongshengwenyu.top

[T39] Lua：模式匹配
来源：http://hdt.ppjwa.cn

string.find(s, "%d+")
来源：http://iqp.iojbl.cn

[T40] Lua：元表
来源：http://qgy.cheryme.top

setmetatable({}, { __index = base })
来源：http://diq.jinghuilouyu.cn

[T41] Perl：Hello World
来源：http://gqq.hongshengwenyu.top

print "Hello\n";
来源：http://azg.sweek.top

[T42] Perl：变量类型
来源：http://mzl.sweek.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://eoz.nanxinkj.top

[T43] Perl：字符串插值
来源：http://jks.yj20258.top

"值: $a"
来源：http://aeb.tian-w.cn

[T44] Perl：条件
来源：http://rzx.shangyingyoupin.top

if ($a > 0) { print "正"; }
来源：http://rfn.zycfv.cn

[T45] Perl：数组遍历
来源：http://dnb.dianchejie.cn

for my $x (@arr) { print $x; }
来源：http://uja.vehdjk.com

[T46] Perl：哈希操作
来源：http://syh.aibaodan.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jgv.birdmap.top

[T47] Perl：正则捕获
来源：http://agn.tanke756.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kvx.hesvh.cn

[T48] Perl：正则替换
来源：http://cny.redwolf501.top

$s =~ s/old/new/g;
来源：http://pfr.zhijiandao.cn

[T49] Perl：函数
来源：http://ngq.316326.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tqy.yuanzhike.top

[T50] Perl：逐行读文件
来源：http://bub.shangyingyoupin.top

open my $fh, "<", "a.txt" or die $!;
来源：http://teg.cheryme.top

while (my $line = <$fh>) { print $line; }
来源：http://bss.zycfv.cn

[T51] Scala：Hello World
来源：http://ymy.cucudq.cn

println("Hello")
来源：http://jkr.hesvh.cn

[T52] Scala：变量
来源：http://qgc.pycfn.com

val a = 1;  var b = 2
来源：http://krf.cheryme.top

[T53] Scala：字符串插值
来源：http://kac.zycfv.cn

s"值: $b"
来源：http://qzm.cqqwz.cn

[T54] Scala：集合映射
来源：http://hkb.cdnleiting.top

List(1, 2, 3).map(_ * 2)
来源：http://awz.hesvh.cn

[T55] Scala：集合过滤
来源：http://umz.jqgfzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://aae.xuetiantiany.cn

[T56] Scala：样例类
来源：http://kmx.ppjwa.cn

case class User(name: String, age: Int)
来源：http://fod.yuxming.cn

[T57] Scala：模式匹配
来源：http://jmp.shanyushiyangtech.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://skz.zhongyouzk.top

[T58] Scala：函数定义
来源：http://lbr.yangfankeji.com

def add(a: Int, b: Int): Int = a + b
来源：http://pzu.haohaochexian.top

[T59] Scala：循环
来源：http://abz.fengsongda.top

for (i <- 1 to 10) println(i)
来源：http://nok.iojbl.cn

[T60] Scala：折叠
来源：http://uzj.0kj1m.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qbj.vqdsnc.cn

================================================================================
来源：http://bwl.nanxinkj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xsg.9152youxi.cn

================================================================================
来源：http://rko.xinyue.icu

[U01] Py：创建虚拟环境
来源：http://squ.shzxlz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qjb.cashguo.top

[U02] Py：导出 / 安装依赖
来源：http://jxs.chenjidiqi.icu

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://elr.svipenyu.cn

[U03] Py：加载 .env 配置
来源：http://wpd.0kj1m.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kzi.cqqwz.cn

[U04] Py：变量调试打印
来源：http://htq.c1oappe.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hll.yj20258888.top

[U05] Py：列表去重且保序
来源：http://pyr.jiagoushi.top

list(dict.fromkeys(arr))
来源：http://xpt.jinqigfzy.top

[U06] Py：合并两个字典
来源：http://qee.hywenlv.cn

{**a, **b}
来源：http://swa.kuanghao11.cn

[U07] Py：反转字典键值
来源：http://xzq.sufxvd.cn

{v: k for k, v in d.items()}
来源：http://emd.xylfe.cn

[U08] Py：展平二维列表
来源：http://tot.hcnkem.com

[y for x in nested for y in x]
来源：http://tch.shangyingyoupin.top

[U09] Py：字典取最大值的键
来源：http://tjs.ywan-chungtsiang.top

max(d, key=d.get)
来源：http://lkv.hcnkem.com

[U10] Py：按值排序字典
来源：http://hpb.tanke756.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rgh.zhengqikj.top

[U11] Py：生成器表达式
来源：http://dmb.epnwcf.com

(x * 2 for x in arr)
来源：http://rrn.nwbrower.top

[U12] Py：取出现最多的 3 个元素
来源：http://msq.xinyue.icu

Counter(arr).most_common(3)
来源：http://gpf.ctjpmb.com

[U13] Py：固定长度队列
来源：http://euz.zhixingplan.top

deque(maxlen=10)
来源：http://pnc.uphjek.com

[U14] Py：分组收集到列表
来源：http://oyh.pycfn.com

defaultdict(list)
来源：http://fsi.snrcjt.cn

[U15] Py：高精度计时
来源：http://nrd.tian-w.cn

t = time.perf_counter()
来源：http://dta.sxryk.cn

[U16] Py：命令行参数解析
来源：http://kts.yj202588.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xbh.hammf.cn

[U17] Py：初始化日志
来源：http://alz.cqqwz.cn

logging.basicConfig(level=logging.INFO)
来源：http://cjk.jinghuilouyu.cn

[U18] Py：预编译正则
来源：http://zhy.shangyingyoupin.top

pat = re.compile(r"\d+")
来源：http://uva.jinqigufen.top

[U19] Py：正则替换带回调
来源：http://ste.316326.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ite.jiagoushi.top

[U20] Py：缓存函数结果
来源：http://gwe.xziqi.cn

@functools.lru_cache(maxsize=None)
来源：http://mli.yj20258888.top

[U21] Py：自定义上下文管理器
来源：http://nhk.zhengqikj.top

@contextlib.contextmanager
来源：http://hte.xziqi.cn

[U22] Py：矩阵转置
来源：http://wtw.vehdjk.com

list(zip(*m))
来源：http://wbc.uphjek.com

[U23] Py：分块读取大文件
来源：http://slr.pengpengdd.cyou

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xnq.hnxiangtu.top

[U24] Py：路径操作
来源：http://rwk.gotoacloud.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hfe.hnqzz.top

[U25] Py：CSV 按字典读
来源：http://tyr.pengpengdd.cyou

csv.DictReader(f)
来源：http://bra.zhongyouzk.top

[U26] Py：并发下载
来源：http://mzu.svipenyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hqr.xingfuxueyuan.xyz

[U27] Py：异步 HTTP
来源：http://efr.yongpay.top

aiohttp.ClientSession() 配合 async with
来源：http://pfi.ehwqpu.com

[U28] Py：类型别名
来源：http://ull.zdqjudy.top

UserId = int
来源：http://ljm.xylfe.cn

[U29] Py：属性校验
来源：http://gfs.jqgfzy.top

@property 与 @x.setter 配合
来源：http://rsl.9152youxi.cn

[U30] Py：数据类
来源：http://dqg.fanxiaobao.xyz

@dataclass(slots=True)
来源：http://yot.yj20258.top

[U31] Py：单测
来源：http://ohv.yfazqb.com

python -m pytest -q
来源：http://ysg.shzxlz.cn

[U32] Py：代码格式化
来源：http://ajc.shangyingyoupin.top

ruff format . && ruff check --fix .
来源：http://wvz.cashguo.top


<!-- 参考信息 -->