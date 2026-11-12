代发 wailian999

strlen(s)
来源：http://dzv.ywan-chungtsiang.top

[S06] C：字符串比较
来源：http://xsh.shanyushiyangkeji.top

strcmp(a, b) == 0
来源：http://ghe.gotoacloud.top

[S07] C：数组遍历求和
来源：http://fnz.zhijiandao.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ctp.jyoumei.cn

[S08] C：动态内存分配与释放
来源：http://cdo.jqgufenzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ujn.fzhhl.top

[S09] C：结构体定义与初始化
来源：http://eon.chenlongwang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://flv.mhx1999.top

[S10] C：指针与解引用
来源：http://bpo.jqgufenzy.top

int *p = &a;  *p = 5;
来源：http://pwt.sysykeji.top

[S11] C：逐行读文件
来源：http://byg.yj20258.top

FILE *f = fopen("a.txt", "r");
来源：http://pmx.tian-w.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://axn.chenzaomai.com

fclose(f);
来源：http://lal.hysaishi.cn

[S12] C：写文件
来源：http://meg.ehwqpu.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xkd.tanke756.top

[S13] C：宏定义
来源：http://des.bjfxy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://onb.aibaodan.cn

[S14] C：枚举
来源：http://lyv.bjfxy.top

enum Color { RED, GREEN, BLUE };
来源：http://wbq.vehdjk.com

[S15] C：类型转换
来源：http://flh.sweek.top

(double) a / b
来源：http://jqr.jqgufenzy.top

[S16] C：位操作置位
来源：http://cba.wangdashe.top

x |= (1 << 3);
来源：http://frd.ydjk.org.cn

[S17] C：安全拼接字符串
来源：http://tbq.tianlin.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kdf.quarkkingdee.top

[S18] C：命令行参数
来源：http://xgr.yj20258888.top

int main(int argc, char **argv)
来源：http://vto.uphjek.com

[S19] C：快速排序
来源：http://cpd.shuidangran.top

qsort(a, n, sizeof(int), cmp);
来源：http://yhp.shanyushiyangkeji.top

[S20] C：二分查找
来源：http://cya.nwbrower.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fad.sysykeji.top

[S21] C：字符类别判断
来源：http://pep.ctjpmb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gai.zhixingplan.top

[S22] C：字符串转数字
来源：http://cya.hcnkem.com

atoi("42");  strtod("3.14", NULL);
来源：http://jlp.nanxinkj.top

[S23] C：随机数
来源：http://wek.haohaochexian.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gzr.cqqwz.cn

[S24] C：获取本地时间
来源：http://inh.havefunace.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ufm.xingfuxueyuan.xyz

[S25] C：内存拷贝
来源：http://bdu.zhaomingkeji.xyz

memcpy(dst, src, n);
来源：http://bbf.zhoulong.xyz

[S26] C：内存清零
来源：http://jfy.cdnleiting.top

memset(a, 0, sizeof a);
来源：http://wdr.zhongyouzk.top

[S27] C：定义常量
来源：http://zkz.jinyuanbaomall.cn

const double PI = 3.14159;
来源：http://bka.pengpengdd.cyou

[S28] C：静态变量
来源：http://muy.ydjk.org.cn

static int counter = 0;
来源：http://cyc.xuetiantiany.cn

[S29] C：变参函数
来源：http://nvb.xuetiantiany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wif.0kj1m.cn

[S30] C：头文件保护
来源：http://tbq.hesvh.cn

#ifndef X_H
来源：http://jcr.fengsongda.top

#define X_H
来源：http://ffb.shanyushiyangkeji.top

#endif
来源：http://iof.iojbl.cn

[S31] C++：Hello World
来源：http://xak.zhongyouzk.top

#include <iostream>
来源：http://gbq.gzhubu.top

int main() { std::cout << "Hello\n"; }
来源：http://xhv.yj20258.top

[S32] C++：字符串
来源：http://tqs.jiagoushi.top

std::string s = "hi";  s += "!";
来源：http://vvv.yj20258888.top

[S33] C++：vector 增删
来源：http://jtf.sxryk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://obx.daxiang520.top

[S34] C++：遍历 vector
来源：http://ssu.daria6918.cn

for (auto &x : v) { std::cout << x; }
来源：http://srt.yj20258888.top

[S35] C++：map
来源：http://gpa.aibaodan.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xwd.gogol.net.cn

[S36] C++：unordered_map
来源：http://cem.hcnkem.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pcv.52xcode.cn

[S37] C++：set
来源：http://mwl.ydzc1.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vdo.jinqigufen.top

[S38] C++：排序
来源：http://cta.aibaodan.cn

std::sort(v.begin(), v.end());
来源：http://kwh.sjlbkw.cn

[S39] C++：自定义比较器排序
来源：http://rzq.jiagoushi.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://feu.meibo888.top

[S40] C++：查找元素
来源：http://csn.jiagoushi.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jix.shangyingyoupin.top

[S41] C++：类与构造函数
来源：http://fvi.xziqi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mxu.hfpthk.cn

[S42] C++：继承与虚函数
来源：http://vmi.jqgufenzy.top

class B : public Base { public: void f() override {} };
来源：http://rgu.sweek.top

[S43] C++：智能指针
来源：http://qon.fehbvm.com

auto p = std::make_unique<int>(5);
来源：http://xqg.daxiang520.top

[S44] C++：引用传参
来源：http://hch.nanxuanxn.top

void inc(int &x) { ++x; }
来源：http://mwb.jqgfzy.top

[S45] C++：lambda
来源：http://eol.aibaodan.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tab.shzxlz.cn

[S46] C++：函数模板
来源：http://amr.sxryk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mvd.sxryk.cn

[S47] C++：结构化绑定遍历
来源：http://fhp.gogol.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fvn.smart0.xyz

[S48] C++：逐行读文件
来源：http://zlc.zhaomingkeji.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://xow.redwolf501.top

while (std::getline(in, line)) { }
来源：http://eaa.havefunace.top

[S49] C++：写文件
来源：http://vxw.wangdashe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://odt.mhx1999.top

[S50] C++：格式化数字
来源：http://phn.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yhb.daria6918.cn

[S51] C++：显式类型转换
来源：http://cns.zhiwuduotai.top

static_cast<double>(a) / b
来源：http://arj.dianchejie.cn

[S52] C++：const 与 noexcept
来源：http://nll.zhaomingkeji.xyz

int size() const noexcept { return n_; }
来源：http://cig.snrcjt.cn

[S53] C++：移动语义
来源：http://nlk.iojbl.cn

std::vector<int> w = std::move(v);
来源：http://pra.daria6918.cn

[S54] C++：异常处理
来源：http://gvw.jinqigufen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://imx.shangyingyoupin.top

[S55] C++：结构化绑定
来源：http://iqd.ywan-chungtsiang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://iep.wangdashe.top

[S56] C++：optional
来源：http://kfk.zycfv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://snq.hnqzz.top

[S57] C++：编译期常量
来源：http://lwx.zdqjudy.top

constexpr int N = 10;
来源：http://ygh.jinyuanbaomall.cn

[S58] C++：命名空间
来源：http://org.xingfuxueyuan.xyz

namespace ns { int f() { return 1; } }
来源：http://uib.havefunace.top

[S59] C++：静态断言
来源：http://ohq.fengsongda.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://orp.havefunace.top

[S60] C++：遍历并删除元素
来源：http://ogj.zhoulong.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kup.cucudq.cn

================================================================================
来源：http://mps.guannengcc.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vuq.zhijiandao.cn

================================================================================
来源：http://rtv.zhijiandao.cn

[T01] Kotlin：Hello World
来源：http://riw.guowangkeji.top

println("Hello")
来源：http://fxp.aizwys.cn

[T02] Kotlin：变量
来源：http://rah.wangshuangyany.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://aav.hysaishi.cn

[T03] Kotlin：字符串模板
来源：http://ftc.yj20258888.top

"值: $b"
来源：http://ufw.xingfuxueyuan.xyz

[T04] Kotlin：空安全
来源：http://kdk.ppjwa.cn

val n: String? = null;  n?.length
来源：http://aiy.ehwqpu.com

[T05] Kotlin：when 表达式
来源：http://pqm.chenjidiqi.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ijo.chenjidiqi.icu

[T06] Kotlin：集合映射
来源：http://jpy.xuanzx.com

listOf(1, 2, 3).map { it * 2 }
来源：http://qjt.smart0.xyz

[T07] Kotlin：集合过滤
来源：http://ckv.uphjek.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://sxf.yvedp.cn

[T08] Kotlin：数据类
来源：http://fhe.52xcode.cn

data class User(val name: String, val age: Int)
来源：http://psj.hysaishi.cn

[T09] Kotlin：扩展函数
来源：http://ysl.svipenyu.cn

fun String.exclaim() = this + "!"
来源：http://kpe.sjlbkw.cn

[T10] Kotlin：默认参数
来源：http://rfr.shuidangran.top

fun greet(name: String = "World") = "Hi $name"
来源：http://oju.sjlbkw.cn

[T11] Kotlin：协程
来源：http://zom.snrcjt.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://flt.gzhubu.top

[T12] Kotlin：解构声明
来源：http://osn.cheryme.top

val (a, b) = Pair(1, 2)
来源：http://zbo.zhixingplan.top

[T13] Kotlin：只读 Map
来源：http://ixc.fanxiaobao.xyz

val m = mapOf("a" to 1)
来源：http://nwj.ppjwa.cn

[T14] Kotlin：循环
来源：http://tnu.tarul.cn

for (i in 1..10) println(i)
来源：http://ozm.yangfankeji.com

[T15] Kotlin：接口
来源：http://nih.vqdsnc.cn

interface Shape { fun area(): Double }
来源：http://ykx.ybcxt.top

[T16] Swift：Hello World
来源：http://vmf.fzhhl.top

print("Hello")
来源：http://dtk.hysaishi.cn

[T17] Swift：变量与常量
来源：http://ado.xylfe.cn

var a = 1;  let b = 2
来源：http://exa.jlsjyb.cn

[T18] Swift：字符串插值
来源：http://rni.hnqzz.top

"值: \(b)"
来源：http://zvj.nwbrower.top

[T19] Swift：可选绑定
来源：http://uiz.jianghu66.top

if let n = opt { print(n) }
来源：http://sli.jinyuanbaomall.cn

[T20] Swift：数组操作
来源：http://xdv.nanxinkj.top

var a = [1, 2, 3];  a.append(4)
来源：http://xbl.hnqzz.top

[T21] Swift：遍历
来源：http://fad.xingfuxueyuan.xyz

for x in a { print(x) }
来源：http://ikv.zhengqikj.top

[T22] Swift：字典
来源：http://khk.nanxinkj.top

var d = ["a": 1];  d["b"] = 2
来源：http://opk.yj202588.top

[T23] Swift：函数
来源：http://gjt.nanxuanxn.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qhl.daria6918.cn

[T24] Swift：闭包
来源：http://tax.zhijiandao.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gdd.zhengqikj.top

[T25] Swift：结构体
来源：http://etu.ydzc1.top

struct P { var x: Int }
来源：http://yyj.jiagoushi.top

[T26] Swift：类与重写
来源：http://zzi.hysaishi.cn

class A: Base { override func f() {} }
来源：http://rjk.shanyushiyangtech.top

[T27] Swift：错误处理
来源：http://tfa.daxiang520.top

do { try f() } catch { print(error) }
来源：http://you.ydzc1.top

[T28] Swift：枚举
来源：http://qeh.cqqwz.cn

enum Color { case red, green }
来源：http://fln.zhengqikj.top

[T29] Swift：guard 提前返回
来源：http://boh.zdqjudy.top

guard let x = opt else { return }
来源：http://gke.yfazqb.com

[T30] Swift：协议
来源：http://kce.cqqwz.cn

protocol Shape { func area() -> Double }
来源：http://jjq.jlsjyb.cn

[T31] Lua：Hello World
来源：http://rex.aibaodan.cn

print("Hello")
来源：http://rgn.zycfv.cn

[T32] Lua：局部变量
来源：http://oem.0kj1m.cn

local a = 1
来源：http://mdy.zycfv.cn

[T33] Lua：表（数组）
来源：http://mzu.vehdjk.com

local t = {1, 2, 3};  t[4] = 4
来源：http://mgn.9152youxi.cn

[T34] Lua：遍历表
来源：http://aaw.9152youxi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mwa.redwolf501.top

[T35] Lua：字典表
来源：http://nat.vehdjk.com

local d = { a = 1 };  d.b = 2
来源：http://uyo.cqqwz.cn

[T36] Lua：函数
来源：http://tsz.0kj1m.cn

function add(a, b) return a + b end
来源：http://yos.redwolf501.top

[T37] Lua：字符串拼接
来源：http://bjx.yueranfly.top

"a" .. "b"
来源：http://cod.haohaochexian.top

[T38] Lua：条件
来源：http://vzm.daxiang520.top

if x > 0 then print("正") end
来源：http://uma.nanxinkj.top

[T39] Lua：模式匹配
来源：http://vee.zhoulong.xyz

string.find(s, "%d+")
来源：http://tua.zhoulong.xyz

[T40] Lua：元表
来源：http://gtt.0kj1m.cn

setmetatable({}, { __index = base })
来源：http://uut.mhx1999.top

[T41] Perl：Hello World
来源：http://jdw.yuxming.cn

print "Hello\n";
来源：http://onp.bbcook.cn

[T42] Perl：变量类型
来源：http://oqd.hywenlv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wrr.xuanzx.com

[T43] Perl：字符串插值
来源：http://odt.tian-w.cn

"值: $a"
来源：http://lau.cheryme.top

[T44] Perl：条件
来源：http://zhy.hnxiangtu.top

if ($a > 0) { print "正"; }
来源：http://bhh.chenlongwang.top

[T45] Perl：数组遍历
来源：http://auk.havefunace.top

for my $x (@arr) { print $x; }
来源：http://khe.yuanzhike.top

[T46] Perl：哈希操作
来源：http://iha.fanxiaobao.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gwl.birdmap.top

[T47] Perl：正则捕获
来源：http://mgw.hywenlv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://uzy.ydzc1.top

[T48] Perl：正则替换
来源：http://sok.zhaomingkeji.xyz

$s =~ s/old/new/g;
来源：http://gcp.svipenyu.cn

[T49] Perl：函数
来源：http://wwx.zhaomingkeji.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lmt.aizwys.cn

[T50] Perl：逐行读文件
来源：http://nkf.zhengqikj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://lfn.ybcxt.top

while (my $line = <$fh>) { print $line; }
来源：http://ume.smart0.xyz

[T51] Scala：Hello World
来源：http://auy.52xcode.cn

println("Hello")
来源：http://pbi.ydjk.org.cn

[T52] Scala：变量
来源：http://pek.gotoacloud.top

val a = 1;  var b = 2
来源：http://pdw.cdnleiting.top

[T53] Scala：字符串插值
来源：http://akz.zhijiandao.cn

s"值: $b"
来源：http://yuk.yj20258.top

[T54] Scala：集合映射
来源：http://qxr.zhijiandao.cn

List(1, 2, 3).map(_ * 2)
来源：http://cgr.yj202588.top

[T55] Scala：集合过滤
来源：http://adn.cdnleiting.top

List(1, 2, 3).filter(_ > 1)
来源：http://vqi.meibo888.top

[T56] Scala：样例类
来源：http://adw.redwolf501.top

case class User(name: String, age: Int)
来源：http://xau.snrcjt.cn

[T57] Scala：模式匹配
来源：http://bwh.shuidangran.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://puj.jiagoushi.top

[T58] Scala：函数定义
来源：http://ast.nwbrower.top

def add(a: Int, b: Int): Int = a + b
来源：http://ibe.cqqwz.cn

[T59] Scala：循环
来源：http://kxu.gogol.net.cn

for (i <- 1 to 10) println(i)
来源：http://ecw.zycfv.cn

[T60] Scala：折叠
来源：http://uwd.vqdsnc.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://adq.ctjpmb.com

================================================================================
来源：http://upg.tianlin.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hmv.yongpay.top

================================================================================
来源：http://dlz.hfpthk.cn

[U01] Py：创建虚拟环境
来源：http://vda.sufxvd.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dyb.hcnkem.com

[U02] Py：导出 / 安装依赖
来源：http://vxz.cheryme.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jvi.mhx1999.top

[U03] Py：加载 .env 配置
来源：http://hsr.sxryk.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nsr.tarul.cn

[U04] Py：变量调试打印
来源：http://wti.zhengqikj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jcb.jinghuilouyu.cn

[U05] Py：列表去重且保序
来源：http://nev.quarkkingdee.top

list(dict.fromkeys(arr))
来源：http://zsu.mhx1999.top

[U06] Py：合并两个字典
来源：http://tas.fzhhl.top

{**a, **b}
来源：http://jit.hesvh.cn

[U07] Py：反转字典键值
来源：http://asa.hongshengwenyu.top

{v: k for k, v in d.items()}
来源：http://cor.meibo888.top

[U08] Py：展平二维列表
来源：http://glt.hnqzz.top

[y for x in nested for y in x]
来源：http://opw.yuxming.cn

[U09] Py：字典取最大值的键
来源：http://zww.mhx1999.top

max(d, key=d.get)
来源：http://kxe.chenzaomai.com

[U10] Py：按值排序字典
来源：http://izu.vqdsnc.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://psd.jqgufenzy.top

[U11] Py：生成器表达式
来源：http://gud.tanke756.top

(x * 2 for x in arr)
来源：http://buo.ybcxt.top

[U12] Py：取出现最多的 3 个元素
来源：http://nby.nanxinkj.top

Counter(arr).most_common(3)
来源：http://bcb.316326.xyz

[U13] Py：固定长度队列
来源：http://mfq.gotoacloud.top

deque(maxlen=10)
来源：http://pdf.jinqigufen.top

[U14] Py：分组收集到列表
来源：http://ksy.xinyue.icu

defaultdict(list)
来源：http://qwn.hywenlv.cn

[U15] Py：高精度计时
来源：http://kpo.feifeiyinyue.top

t = time.perf_counter()
来源：http://jjh.aibaodan.cn

[U16] Py：命令行参数解析
来源：http://hii.havefunace.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gyh.zhengqikj.top

[U17] Py：初始化日志
来源：http://qky.yvedp.cn

logging.basicConfig(level=logging.INFO)
来源：http://fiy.xinyue.icu

[U18] Py：预编译正则
来源：http://aaq.vehdjk.com

pat = re.compile(r"\d+")
来源：http://gzt.zhiwuduotai.top

[U19] Py：正则替换带回调
来源：http://yce.yuanzhike.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://och.pycfn.com

[U20] Py：缓存函数结果
来源：http://rpt.yangfankeji.com

@functools.lru_cache(maxsize=None)
来源：http://zgt.chenzaomai.com

[U21] Py：自定义上下文管理器
来源：http://ksd.hnxiangtu.top

@contextlib.contextmanager
来源：http://txt.zycfv.cn

[U22] Py：矩阵转置
来源：http://ehl.yuxming.cn

list(zip(*m))
来源：http://mol.shuidangran.top

[U23] Py：分块读取大文件
来源：http://zhk.gzhubu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eya.svipenyu.cn

[U24] Py：路径操作
来源：http://joi.daria6918.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xse.smart0.xyz

[U25] Py：CSV 按字典读
来源：http://stg.zycfv.cn

csv.DictReader(f)
来源：http://pxl.hnqzz.top

[U26] Py：并发下载
来源：http://vkq.wangshuangyany.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ztm.bjfxy.top

[U27] Py：异步 HTTP
来源：http://jgl.zdqjudy.top

aiohttp.ClientSession() 配合 async with
来源：http://isc.nwbrower.top

[U28] Py：类型别名
来源：http://tvf.hcnkem.com

UserId = int
来源：http://bqd.fzhhl.top


<!-- 参考信息 -->