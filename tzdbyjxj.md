代发 wailian999

int x; scanf("%d", &x);
来源：http://cbi.gogol.net.cn

[S04] C：字符串复制
来源：http://nlq.yfazqb.com

char dst[32]; strcpy(dst, "hi");
来源：http://uyj.shzxlz.cn

[S05] C：字符串长度
来源：http://nva.cqqwz.cn

strlen(s)
来源：http://yed.svipenyu.cn

[S06] C：字符串比较
来源：http://prt.yongpay.top

strcmp(a, b) == 0
来源：http://nev.c1oappe.top

[S07] C：数组遍历求和
来源：http://szk.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xme.kuanghao11.cn

[S08] C：动态内存分配与释放
来源：http://kcv.fengsongda.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rhy.yj20258.top

[S09] C：结构体定义与初始化
来源：http://lvu.zhijiandao.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://amg.daxiang520.top

[S10] C：指针与解引用
来源：http://ubd.hywenlv.cn

int *p = &a;  *p = 5;
来源：http://xtp.zdbjq.cn

[S11] C：逐行读文件
来源：http://ojg.ydjk.org.cn

FILE *f = fopen("a.txt", "r");
来源：http://bdw.ywan-chungtsiang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xxz.c1oappe.top

fclose(f);
来源：http://mub.ydjk.org.cn

[S12] C：写文件
来源：http://thh.gotoacloud.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qpl.0kj1m.cn

[S13] C：宏定义
来源：http://enh.jlsjyb.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://akd.shzxlz.cn

[S14] C：枚举
来源：http://jpe.gogol.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://yah.hcnkem.com

[S15] C：类型转换
来源：http://urh.andypj.xyz

(double) a / b
来源：http://ekk.c1oappe.top

[S16] C：位操作置位
来源：http://rjd.fktsv.cn

x |= (1 << 3);
来源：http://kmw.dashuyun.cn

[S17] C：安全拼接字符串
来源：http://eop.ybcxt.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cxs.hfpthk.cn

[S18] C：命令行参数
来源：http://gja.hnxiangtu.top

int main(int argc, char **argv)
来源：http://hih.snrcjt.cn

[S19] C：快速排序
来源：http://lvn.quarkkingdee.top

qsort(a, n, sizeof(int), cmp);
来源：http://jln.52xcode.cn

[S20] C：二分查找
来源：http://gwn.zhixingplan.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tqf.tanke756.top

[S21] C：字符类别判断
来源：http://wyb.jinyuanbaomall.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hem.fengsongda.top

[S22] C：字符串转数字
来源：http://kzl.yj20258.top

atoi("42");  strtod("3.14", NULL);
来源：http://evz.0kj1m.cn

[S23] C：随机数
来源：http://evk.sjlbkw.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nrk.jlsjyb.cn

[S24] C：获取本地时间
来源：http://mfa.aizwys.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kgq.ybcxt.top

[S25] C：内存拷贝
来源：http://odd.xylfe.cn

memcpy(dst, src, n);
来源：http://aig.sjlbkw.cn

[S26] C：内存清零
来源：http://par.wangshuangyany.cn

memset(a, 0, sizeof a);
来源：http://mgb.yanxiufei.cn

[S27] C：定义常量
来源：http://ydt.meibo888.top

const double PI = 3.14159;
来源：http://nyn.hammf.cn

[S28] C：静态变量
来源：http://lln.52xcode.cn

static int counter = 0;
来源：http://vbk.chenzaomai.com

[S29] C：变参函数
来源：http://mvh.gogol.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ogi.svipenyu.cn

[S30] C：头文件保护
来源：http://gzd.c1oappe.top

#ifndef X_H
来源：http://ncd.9152youxi.cn

#define X_H
来源：http://ynl.xingfuxueyuan.xyz

#endif
来源：http://fvp.tarul.cn

[S31] C++：Hello World
来源：http://miz.xuetiantiany.cn

#include <iostream>
来源：http://ihs.sxryk.cn

int main() { std::cout << "Hello\n"; }
来源：http://fot.shzxlz.cn

[S32] C++：字符串
来源：http://cyy.tanke756.top

std::string s = "hi";  s += "!";
来源：http://pcf.havefunace.top

[S33] C++：vector 增删
来源：http://krl.xuanzx.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gyk.dianchejie.cn

[S34] C++：遍历 vector
来源：http://wft.epnwcf.com

for (auto &x : v) { std::cout << x; }
来源：http://bcf.jinghuilouyu.cn

[S35] C++：map
来源：http://ktb.gzhubu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zky.hywenlv.cn

[S36] C++：unordered_map
来源：http://okw.tianlin.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tbf.hywenlv.cn

[S37] C++：set
来源：http://dbd.jlsjyb.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ytv.yueranfly.top

[S38] C++：排序
来源：http://cqk.shanyushiyangtech.top

std::sort(v.begin(), v.end());
来源：http://cfm.tian-w.cn

[S39] C++：自定义比较器排序
来源：http://lej.hammf.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gmt.chenjidiqi.icu

[S40] C++：查找元素
来源：http://ijk.cdnleiting.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rkh.aibaodan.cn

[S41] C++：类与构造函数
来源：http://apg.xylfe.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nwl.ppjwa.cn

[S42] C++：继承与虚函数
来源：http://xfv.tarul.cn

class B : public Base { public: void f() override {} };
来源：http://vei.ctjpmb.com

[S43] C++：智能指针
来源：http://wkw.yangfankeji.com

auto p = std::make_unique<int>(5);
来源：http://xwm.haohaochexian.top

[S44] C++：引用传参
来源：http://vzg.ybcxt.top

void inc(int &x) { ++x; }
来源：http://fww.tianlin.xyz

[S45] C++：lambda
来源：http://yyg.shanyushiyangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://gdz.yj202588.top

[S46] C++：函数模板
来源：http://bwk.iojbl.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dkh.yj20258.top

[S47] C++：结构化绑定遍历
来源：http://epl.zhijiandao.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pkh.andypj.xyz

[S48] C++：逐行读文件
来源：http://rlj.tianlin.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://ere.tanke756.top

while (std::getline(in, line)) { }
来源：http://eks.uphjek.com

[S49] C++：写文件
来源：http://brf.cucudq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mly.jinyuanbaomall.cn

[S50] C++：格式化数字
来源：http://azk.pengpengdd.cyou

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cuh.zhixingplan.top

[S51] C++：显式类型转换
来源：http://gwn.sweek.top

static_cast<double>(a) / b
来源：http://dew.havefunace.top

[S52] C++：const 与 noexcept
来源：http://akg.gogol.net.cn

int size() const noexcept { return n_; }
来源：http://alr.fengsongda.top

[S53] C++：移动语义
来源：http://osb.yj20258.top

std::vector<int> w = std::move(v);
来源：http://czb.cashguo.top

[S54] C++：异常处理
来源：http://odo.zhixingplan.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oqc.hysaishi.cn

[S55] C++：结构化绑定
来源：http://iku.hysaishi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fou.ctjpmb.com

[S56] C++：optional
来源：http://sky.pengpengdd.cyou

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://knn.pycfn.com

[S57] C++：编译期常量
来源：http://icp.sufxvd.cn

constexpr int N = 10;
来源：http://ftk.zycfv.cn

[S58] C++：命名空间
来源：http://iuz.jianghu66.top

namespace ns { int f() { return 1; } }
来源：http://vet.redwolf501.top

[S59] C++：静态断言
来源：http://pwy.ppjwa.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iyd.sufxvd.cn

[S60] C++：遍历并删除元素
来源：http://fju.epnwcf.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hgw.hammf.cn

================================================================================
来源：http://fud.ppjwa.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ckq.daxiang520.top

================================================================================
来源：http://azl.jqgufenzy.top

[T01] Kotlin：Hello World
来源：http://sxb.pengpengdd.cyou

println("Hello")
来源：http://fdu.jyoumei.cn

[T02] Kotlin：变量
来源：http://dnt.aizwys.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dwe.shangyingyoupin.top

[T03] Kotlin：字符串模板
来源：http://mwp.gzhubu.top

"值: $b"
来源：http://yon.tanke756.top

[T04] Kotlin：空安全
来源：http://rni.ydzc1.top

val n: String? = null;  n?.length
来源：http://hte.9152youxi.cn

[T05] Kotlin：when 表达式
来源：http://nnk.yuxming.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zsz.smart0.xyz

[T06] Kotlin：集合映射
来源：http://jia.0kj1m.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mdw.yongpay.top

[T07] Kotlin：集合过滤
来源：http://gjh.chenlongwang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://yqw.tarul.cn

[T08] Kotlin：数据类
来源：http://nxn.cqqwz.cn

data class User(val name: String, val age: Int)
来源：http://ejq.gzhubu.top

[T09] Kotlin：扩展函数
来源：http://bxr.zhengqikj.top

fun String.exclaim() = this + "!"
来源：http://off.0kj1m.cn

[T10] Kotlin：默认参数
来源：http://gih.c1oappe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gry.vqdsnc.cn

[T11] Kotlin：协程
来源：http://dpb.ppjwa.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://oab.snrcjt.cn

[T12] Kotlin：解构声明
来源：http://fml.316326.xyz

val (a, b) = Pair(1, 2)
来源：http://jju.nanxinkj.top

[T13] Kotlin：只读 Map
来源：http://xgm.0kj1m.cn

val m = mapOf("a" to 1)
来源：http://arw.yfazqb.com

[T14] Kotlin：循环
来源：http://wvf.pycfn.com

for (i in 1..10) println(i)
来源：http://opz.hfpthk.cn

[T15] Kotlin：接口
来源：http://wvy.ydzc1.top

interface Shape { fun area(): Double }
来源：http://wnt.hnxiangtu.top

[T16] Swift：Hello World
来源：http://krz.smart0.xyz

print("Hello")
来源：http://wri.wangshuangyany.cn

[T17] Swift：变量与常量
来源：http://did.9152youxi.cn

var a = 1;  let b = 2
来源：http://xlt.havefunace.top

[T18] Swift：字符串插值
来源：http://tsq.jyoumei.cn

"值: \(b)"
来源：http://xlf.tanke756.top

[T19] Swift：可选绑定
来源：http://gdj.shanyushiyangkeji.top

if let n = opt { print(n) }
来源：http://ipo.iojbl.cn

[T20] Swift：数组操作
来源：http://hln.c1oappe.top

var a = [1, 2, 3];  a.append(4)
来源：http://wad.fengsongda.top

[T21] Swift：遍历
来源：http://wjo.yuanzhike.top

for x in a { print(x) }
来源：http://htc.mhx1999.top

[T22] Swift：字典
来源：http://twa.gzhubu.top

var d = ["a": 1];  d["b"] = 2
来源：http://fmx.birdmap.top

[T23] Swift：函数
来源：http://kkk.jiagoushi.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://epc.jqgufenzy.top

[T24] Swift：闭包
来源：http://flq.chenzaomai.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://gvj.sjlbkw.cn

[T25] Swift：结构体
来源：http://qtg.yvedp.cn

struct P { var x: Int }
来源：http://fdz.jqgfzy.top

[T26] Swift：类与重写
来源：http://ozo.cdnleiting.top

class A: Base { override func f() {} }
来源：http://uvo.chenzaomai.com

[T27] Swift：错误处理
来源：http://ixs.sufxvd.cn

do { try f() } catch { print(error) }
来源：http://iyt.hnqzz.top

[T28] Swift：枚举
来源：http://aff.aibaodan.cn

enum Color { case red, green }
来源：http://zhl.ehwqpu.com

[T29] Swift：guard 提前返回
来源：http://ile.xziqi.cn

guard let x = opt else { return }
来源：http://dar.andypj.xyz

[T30] Swift：协议
来源：http://rve.yongpay.top

protocol Shape { func area() -> Double }
来源：http://pia.fanxiaobao.xyz

[T31] Lua：Hello World
来源：http://juq.zycfv.cn

print("Hello")
来源：http://rye.gotoacloud.top

[T32] Lua：局部变量
来源：http://lrf.zdqjudy.top

local a = 1
来源：http://hdj.aibaodan.cn

[T33] Lua：表（数组）
来源：http://glc.jyoumei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fzz.nwbrower.top

[T34] Lua：遍历表
来源：http://jkn.meibo888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://sdz.ydjk.org.cn

[T35] Lua：字典表
来源：http://qkf.epnwcf.com

local d = { a = 1 };  d.b = 2
来源：http://uuv.nanxuanxn.top

[T36] Lua：函数
来源：http://qbb.fanxiaobao.xyz

function add(a, b) return a + b end
来源：http://omy.yvedp.cn

[T37] Lua：字符串拼接
来源：http://deb.zhengqikj.top

"a" .. "b"
来源：http://xzb.epnwcf.com

[T38] Lua：条件
来源：http://avp.52xcode.cn

if x > 0 then print("正") end
来源：http://eqk.zhixingplan.top

[T39] Lua：模式匹配
来源：http://wsv.svipenyu.cn

string.find(s, "%d+")
来源：http://lax.yueranfly.top

[T40] Lua：元表
来源：http://bgb.shzxlz.cn

setmetatable({}, { __index = base })
来源：http://rmk.hesvh.cn

[T41] Perl：Hello World
来源：http://bwk.hesvh.cn

print "Hello\n";
来源：http://wth.xinyue.icu

[T42] Perl：变量类型
来源：http://vhg.guannengcc.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://luw.pengpengdd.cyou

[T43] Perl：字符串插值
来源：http://ysu.jinqigfzy.top

"值: $a"
来源：http://wrq.zycfv.cn

[T44] Perl：条件
来源：http://yuy.chenlongwang.top

if ($a > 0) { print "正"; }
来源：http://wgz.tian-w.cn

[T45] Perl：数组遍历
来源：http://esn.daria6918.cn

for my $x (@arr) { print $x; }
来源：http://oub.hfpthk.cn

[T46] Perl：哈希操作
来源：http://oee.jqgufenzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mvc.hywenlv.cn

[T47] Perl：正则捕获
来源：http://xrr.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://wpc.cdnleiting.top

[T48] Perl：正则替换
来源：http://zlx.andypj.xyz

$s =~ s/old/new/g;
来源：http://tbr.vehdjk.com

[T49] Perl：函数
来源：http://zkq.redwolf501.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://noi.dashuyun.cn

[T50] Perl：逐行读文件
来源：http://qet.tanke756.top

open my $fh, "<", "a.txt" or die $!;
来源：http://aie.cucudq.cn

while (my $line = <$fh>) { print $line; }
来源：http://cvp.yj20258888.top

[T51] Scala：Hello World
来源：http://yhz.cucudq.cn

println("Hello")
来源：http://bcl.jqgfzy.top

[T52] Scala：变量
来源：http://hya.ehwqpu.com

val a = 1;  var b = 2
来源：http://nss.jinghuilouyu.cn

[T53] Scala：字符串插值
来源：http://wwm.hysaishi.cn

s"值: $b"
来源：http://chj.zhengqikj.top

[T54] Scala：集合映射
来源：http://azo.ppjwa.cn

List(1, 2, 3).map(_ * 2)
来源：http://iox.chenzaomai.com

[T55] Scala：集合过滤
来源：http://mvi.iojbl.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qlf.tanke756.top

[T56] Scala：样例类
来源：http://dav.xuanzx.com

case class User(name: String, age: Int)
来源：http://fei.xinyue.icu

[T57] Scala：模式匹配
来源：http://vih.vehdjk.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://sxr.hongshengwenyu.top

[T58] Scala：函数定义
来源：http://jgj.jinghuilouyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dkp.andypj.xyz

[T59] Scala：循环
来源：http://gor.hfpthk.cn

for (i <- 1 to 10) println(i)
来源：http://tjr.c1oappe.top

[T60] Scala：折叠
来源：http://ssu.vqdsnc.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gdq.xylfe.cn

================================================================================
来源：http://agr.yj20258888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ckf.hysaishi.cn

================================================================================
来源：http://vqv.uphjek.com

[U01] Py：创建虚拟环境
来源：http://ctu.sweek.top

python -m venv .venv && source .venv/bin/activate
来源：http://oqk.chenjidiqi.icu

[U02] Py：导出 / 安装依赖
来源：http://ndp.dianchejie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lvx.ydjk.org.cn

[U03] Py：加载 .env 配置
来源：http://zgp.ppjwa.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yuk.fengsongda.top

[U04] Py：变量调试打印
来源：http://ukg.hesvh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wmy.havefunace.top

[U05] Py：列表去重且保序
来源：http://zir.nanxinkj.top

list(dict.fromkeys(arr))
来源：http://zlc.ppjwa.cn

[U06] Py：合并两个字典
来源：http://mfk.bbcook.cn

{**a, **b}
来源：http://sjb.daria6918.cn

[U07] Py：反转字典键值
来源：http://igy.aizwys.cn

{v: k for k, v in d.items()}
来源：http://jcq.316326.xyz

[U08] Py：展平二维列表
来源：http://wqs.fehbvm.com

[y for x in nested for y in x]
来源：http://kdo.yj202588.top

[U09] Py：字典取最大值的键
来源：http://uob.yongpay.top

max(d, key=d.get)
来源：http://hda.c1oappe.top

[U10] Py：按值排序字典
来源：http://fmk.yonumen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ysv.ydjk.org.cn

[U11] Py：生成器表达式
来源：http://lgm.yonumen.top

(x * 2 for x in arr)
来源：http://xkc.bjfxy.top

[U12] Py：取出现最多的 3 个元素
来源：http://rja.c1oappe.top

Counter(arr).most_common(3)
来源：http://utd.ehwqpu.com

[U13] Py：固定长度队列
来源：http://gnv.jiagoushi.top

deque(maxlen=10)
来源：http://cxx.hcnkem.com

[U14] Py：分组收集到列表
来源：http://obd.jqgfzy.top

defaultdict(list)
来源：http://kyk.yvedp.cn

[U15] Py：高精度计时
来源：http://uoc.pycfn.com

t = time.perf_counter()
来源：http://nhj.gaohongyu789.top

[U16] Py：命令行参数解析
来源：http://cbk.dianchejie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hgg.9152youxi.cn

[U17] Py：初始化日志
来源：http://gpy.jqgufenzy.top

logging.basicConfig(level=logging.INFO)
来源：http://nsv.yj20258888.top

[U18] Py：预编译正则
来源：http://ktd.ydzc1.top

pat = re.compile(r"\d+")
来源：http://bhx.uphjek.com

[U19] Py：正则替换带回调
来源：http://kvk.nanxuanxn.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cvj.yangfankeji.com

[U20] Py：缓存函数结果
来源：http://liz.meibo888.top

@functools.lru_cache(maxsize=None)
来源：http://cfg.zdbjq.cn

[U21] Py：自定义上下文管理器
来源：http://pbr.jqgufenzy.top

@contextlib.contextmanager
来源：http://cfq.aibaodan.cn

[U22] Py：矩阵转置
来源：http://jnu.sjlbkw.cn

list(zip(*m))
来源：http://flu.tianlin.xyz

[U23] Py：分块读取大文件
来源：http://zxi.c1oappe.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dbk.zhiwuduotai.top

[U24] Py：路径操作
来源：http://mvj.fktsv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bjk.nanxuanxn.top

[U25] Py：CSV 按字典读
来源：http://mfj.zhoulong.xyz

csv.DictReader(f)
来源：http://upa.c1oappe.top

[U26] Py：并发下载
来源：http://jwg.yonumen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eaq.guowangkeji.top


<!-- 参考信息 -->