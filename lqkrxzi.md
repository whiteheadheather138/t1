代发 wailian999

[S37] C++：set
来源：http://www.share.sjlbkw.cn/Article/details/gzdnhnxba.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.yfazqb.com/Article/details/gdjtlcadw.sHtML

[S38] C++：排序
来源：http://read.share.fktsv.cn/Article/details/grcdhlfii.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.sjlbkw.cn/Article/details/guvamismp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.sjlbkw.cn/Article/details/gwvvopvas.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.tarul.cn/Article/details/gagcblkpq.sHtML

[S40] C++：查找元素
来源：http://read.share.epnwcf.com/Article/details/glhdxdsde.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fktsv.cn/Article/details/gppwmxnbx.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.vehdjk.com/Article/details/grtnmpgoi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.tarul.cn/Article/details/gqxgdjgga.sHtML

[S42] C++：继承与虚函数
来源：http://baike.epnwcf.com/Article/details/gqrgrzrjn.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.yfazqb.com/Article/details/gdmltsizf.sHtML

[S43] C++：智能指针
来源：http://blog.vehdjk.com/Article/details/gfprlgtqy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.epnwcf.com/Article/details/gxyqqwybd.sHtML

[S44] C++：引用传参
来源：http://baike.yfazqb.com/Article/details/gdtqrnxye.sHtML

void inc(int &x) { ++x; }
来源：http://wap.epnwcf.com/Article/details/gcifohtfi.sHtML

[S45] C++：lambda
来源：http://m.share.fktsv.cn/Article/details/gbpxugdte.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.yfazqb.com/Article/details/gokvaliik.sHtML

[S46] C++：函数模板
来源：http://wap.fktsv.cn/Article/details/gopuonyiy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.tarul.cn/Article/details/gkngkuvqh.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.epnwcf.com/Article/details/gqwxhrsmy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fktsv.cn/Article/details/gkvbznwhn.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gqgajoaaj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fktsv.cn/Article/details/gtxjfusjs.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.epnwcf.com/Article/details/gqxkhqqpd.sHtML

[S49] C++：写文件
来源：http://m.share.tarul.cn/Article/details/gxofnlzmt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.epnwcf.com/Article/details/gcyzuqdiv.sHtML

[S50] C++：格式化数字
来源：http://read.share.epnwcf.com/Article/details/gafewjbfp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/ghycshkhb.sHtML

[S51] C++：显式类型转换
来源：http://blog.epnwcf.com/Article/details/gojejpjuw.sHtML

static_cast<double>(a) / b
来源：http://3g.yfazqb.com/Article/details/gwnthtwry.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.epnwcf.com/Article/details/gfhmheshq.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.vehdjk.com/Article/details/ggqufapuu.sHtML

[S53] C++：移动语义
来源：http://www.share.epnwcf.com/Article/details/gmmccvbnx.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.sjlbkw.cn/Article/details/gdwblldzy.sHtML

[S54] C++：异常处理
来源：http://www.blog.epnwcf.com/Article/details/gzzyyrops.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.yfazqb.com/Article/details/gspixtmae.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.yfazqb.com/Article/details/gepmycnms.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.bbcook.cn/Article/details/goehndpoq.sHtML

[S56] C++：optional
来源：http://www.m.share.tarul.cn/Article/details/gxzkwcllj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.sjlbkw.cn/Article/details/gnlmvkdzq.sHtML

[S57] C++：编译期常量
来源：http://blog.vehdjk.com/Article/details/guwnzwzad.sHtML

constexpr int N = 10;
来源：http://baike.vehdjk.com/Article/details/gdptbssbw.sHtML

[S58] C++：命名空间
来源：http://read.share.epnwcf.com/Article/details/gxixjbhmb.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fktsv.cn/Article/details/gftynqkka.sHtML

[S59] C++：静态断言
来源：http://www.blog.epnwcf.com/Article/details/gedkviifl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.sjlbkw.cn/Article/details/gvxhvezyp.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.epnwcf.com/Article/details/gyydrabyg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.sjlbkw.cn/Article/details/glamfdoko.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxqetzqcc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.sjlbkw.cn/Article/details/gfhhetlph.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gvaoyrjti.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.yfazqb.com/Article/details/gqhbiyhca.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/geajzgtiu.sHtML

[T02] Kotlin：变量
来源：http://m.share.fktsv.cn/Article/details/gegaehkhc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.epnwcf.com/Article/details/gqniewprh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.tarul.cn/Article/details/gyqtcbghq.sHtML

"值: $b"
来源：http://wap.yfazqb.com/Article/details/ghryfvmrq.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fktsv.cn/Article/details/gcnfzblrl.sHtML

val n: String? = null;  n?.length
来源：http://m.share.sjlbkw.cn/Article/details/gbwiblxdg.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fktsv.cn/Article/details/gqkbelnoy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.sjlbkw.cn/Article/details/gcszskcqu.sHtML

[T06] Kotlin：集合映射
来源：http://wap.tarul.cn/Article/details/gdenyhmcn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.bbcook.cn/Article/details/gyeaiamuv.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.tarul.cn/Article/details/gqragblxf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.yfazqb.com/Article/details/gzrxpbbdv.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fktsv.cn/Article/details/ghtmahrxa.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.tarul.cn/Article/details/gubpmumyi.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.vehdjk.com/Article/details/gwpgwzlql.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.tarul.cn/Article/details/glxpqeoeo.sHtML

[T10] Kotlin：默认参数
来源：http://blog.bbcook.cn/Article/details/gjouaeiwo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.epnwcf.com/Article/details/ginohwbro.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fktsv.cn/Article/details/gjpippxho.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fktsv.cn/Article/details/gonjznnjj.sHtML

[T12] Kotlin：解构声明
来源：http://3g.yfazqb.com/Article/details/guaxayxcs.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gztlxdksp.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.sjlbkw.cn/Article/details/gkuksrvwl.sHtML

val m = mapOf("a" to 1)
来源：http://blog.yfazqb.com/Article/details/gweqcxvit.sHtML

[T14] Kotlin：循环
来源：http://baike.sjlbkw.cn/Article/details/gwwfmpedv.sHtML

for (i in 1..10) println(i)
来源：http://mobile.epnwcf.com/Article/details/gugsqocsy.sHtML

[T15] Kotlin：接口
来源：http://mobile.yfazqb.com/Article/details/gocgaegyc.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fktsv.cn/Article/details/gltfuzcak.sHtML

[T16] Swift：Hello World
来源：http://baike.yfazqb.com/Article/details/gypeelbdh.sHtML

print("Hello")
来源：http://wap.fktsv.cn/Article/details/goypczkvu.sHtML

[T17] Swift：变量与常量
来源：http://read.share.yfazqb.com/Article/details/ggsyzylez.sHtML

var a = 1;  let b = 2
来源：http://read.share.fktsv.cn/Article/details/gzoagmzvo.sHtML

[T18] Swift：字符串插值
来源：http://3g.yfazqb.com/Article/details/gifsssnnt.sHtML

"值: \(b)"
来源：http://baike.epnwcf.com/Article/details/gljwrbbni.sHtML

[T19] Swift：可选绑定
来源：http://blog.bbcook.cn/Article/details/gcpeujfim.sHtML

if let n = opt { print(n) }
来源：http://mobile.yfazqb.com/Article/details/gvtxocgqo.sHtML

[T20] Swift：数组操作
来源：http://www.share.yfazqb.com/Article/details/gsxglqefa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.epnwcf.com/Article/details/gryssecqy.sHtML

[T21] Swift：遍历
来源：http://wap.yfazqb.com/Article/details/grkigvonw.sHtML

for x in a { print(x) }
来源：http://mobile.yfazqb.com/Article/details/gfrfihsdn.sHtML

[T22] Swift：字典
来源：http://baike.epnwcf.com/Article/details/gzwvbgakk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fktsv.cn/Article/details/grkwnwbrj.sHtML

[T23] Swift：函数
来源：http://blog.tarul.cn/Article/details/gsfynxrzp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.tarul.cn/Article/details/grnmmmncz.sHtML

[T24] Swift：闭包
来源：http://mobile.fktsv.cn/Article/details/gfaeqrtyo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.bbcook.cn/Article/details/genogtwkv.sHtML

[T25] Swift：结构体
来源：http://mobile.fktsv.cn/Article/details/gdrapagfi.sHtML

struct P { var x: Int }
来源：http://baike.tarul.cn/Article/details/gijtjbssb.sHtML

[T26] Swift：类与重写
来源：http://wap.vehdjk.com/Article/details/gierofrqp.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.bbcook.cn/Article/details/gkrvdtrkh.sHtML

[T27] Swift：错误处理
来源：http://read.share.epnwcf.com/Article/details/gsguuvviw.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.epnwcf.com/Article/details/grkhpdpuq.sHtML

[T28] Swift：枚举
来源：http://blog.vehdjk.com/Article/details/gvvdmynzo.sHtML

enum Color { case red, green }
来源：http://baike.yfazqb.com/Article/details/ghbrokwxu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fktsv.cn/Article/details/gercpyvkg.sHtML

guard let x = opt else { return }
来源：http://mobile.fktsv.cn/Article/details/gtqisurhg.sHtML

[T30] Swift：协议
来源：http://wap.fktsv.cn/Article/details/gjtjilagf.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.vehdjk.com/Article/details/gmmapyzol.sHtML

[T31] Lua：Hello World
来源：http://www.share.tarul.cn/Article/details/grgzmtmoo.sHtML

print("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gnqmxrmpp.sHtML

[T32] Lua：局部变量
来源：http://mobile.sjlbkw.cn/Article/details/ggjovjssk.sHtML

local a = 1
来源：http://baike.sjlbkw.cn/Article/details/ggrsqfbyu.sHtML

[T33] Lua：表（数组）
来源：http://blog.tarul.cn/Article/details/grrmxkbye.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.tarul.cn/Article/details/gmzennrro.sHtML

[T34] Lua：遍历表
来源：http://mobile.tarul.cn/Article/details/gtwsdyhsu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.yfazqb.com/Article/details/gmuhpkmhn.sHtML

[T35] Lua：字典表
来源：http://wap.epnwcf.com/Article/details/gpuyhsrri.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fktsv.cn/Article/details/gmilgddih.sHtML

[T36] Lua：函数
来源：http://www.m.share.fktsv.cn/Article/details/ghjdfdqrb.sHtML

function add(a, b) return a + b end
来源：http://www.blog.bbcook.cn/Article/details/gqatwounc.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.sjlbkw.cn/Article/details/gvecmfhmc.sHtML

"a" .. "b"
来源：http://baike.bbcook.cn/Article/details/gxyuyraln.sHtML

[T38] Lua：条件
来源：http://blog.yfazqb.com/Article/details/gmgknhuff.sHtML

if x > 0 then print("正") end
来源：http://m.share.sjlbkw.cn/Article/details/gugohjpdz.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fktsv.cn/Article/details/gmrzvcawj.sHtML

string.find(s, "%d+")
来源：http://baike.bbcook.cn/Article/details/gmnhgaakf.sHtML

[T40] Lua：元表
来源：http://blog.tarul.cn/Article/details/ggmhjmuay.sHtML

setmetatable({}, { __index = base })
来源：http://baike.yfazqb.com/Article/details/gyjayspgx.sHtML

[T41] Perl：Hello World
来源：http://m.share.yfazqb.com/Article/details/gsrdgfvap.sHtML

print "Hello\n";
来源：http://www.m.share.bbcook.cn/Article/details/gnbhsezet.sHtML

[T42] Perl：变量类型
来源：http://3g.bbcook.cn/Article/details/gjmfdwxfn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.epnwcf.com/Article/details/gbfbfnumn.sHtML

[T43] Perl：字符串插值
来源：http://3g.yfazqb.com/Article/details/ghgsozsun.sHtML

"值: $a"
来源：http://www.m.share.sjlbkw.cn/Article/details/grposdghs.sHtML

[T44] Perl：条件
来源：http://www.m.share.tarul.cn/Article/details/gmbxeyxcj.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.epnwcf.com/Article/details/gdtberecv.sHtML

[T45] Perl：数组遍历
来源：http://m.share.sjlbkw.cn/Article/details/gqkauacco.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fktsv.cn/Article/details/ggcdiddly.sHtML

[T46] Perl：哈希操作
来源：http://wap.epnwcf.com/Article/details/gtzfyievs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.sjlbkw.cn/Article/details/gzsddqgmr.sHtML

[T47] Perl：正则捕获
来源：http://read.share.sjlbkw.cn/Article/details/gvoqgdexi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.sjlbkw.cn/Article/details/gngswocjx.sHtML

[T48] Perl：正则替换
来源：http://3g.vehdjk.com/Article/details/gkmynfpny.sHtML

$s =~ s/old/new/g;
来源：http://mobile.yfazqb.com/Article/details/gdiendktb.sHtML

[T49] Perl：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzarqljz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gfzjlbhnm.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gvckfrptt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.sjlbkw.cn/Article/details/gsbthyncx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsdhsroz.sHtML

[T51] Scala：Hello World
来源：http://wap.yfazqb.com/Article/details/gicvpqkav.sHtML

println("Hello")
来源：http://wap.tarul.cn/Article/details/ggjzhgiyq.sHtML

[T52] Scala：变量
来源：http://read.share.epnwcf.com/Article/details/gqhtqaedh.sHtML

val a = 1;  var b = 2
来源：http://wap.epnwcf.com/Article/details/gyahzltdd.sHtML

[T53] Scala：字符串插值
来源：http://blog.fktsv.cn/Article/details/gxhiziqja.sHtML

s"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/ghkilgpaq.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fktsv.cn/Article/details/grcoizyfs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.vehdjk.com/Article/details/gvnkfacml.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fktsv.cn/Article/details/glccgunci.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.yfazqb.com/Article/details/gourlnpoj.sHtML

[T56] Scala：样例类
来源：http://wap.epnwcf.com/Article/details/gwhbvqmjm.sHtML

case class User(name: String, age: Int)
来源：http://baike.epnwcf.com/Article/details/gcjtmmqnd.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.epnwcf.com/Article/details/gkcyrztvz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.tarul.cn/Article/details/gpepdmmzg.sHtML

[T58] Scala：函数定义
来源：http://read.share.epnwcf.com/Article/details/gznrvjomi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.bbcook.cn/Article/details/gbxgdzfdi.sHtML

[T59] Scala：循环
来源：http://www.blog.tarul.cn/Article/details/gairjpzce.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/gymeozsbx.sHtML

[T60] Scala：折叠
来源：http://3g.sjlbkw.cn/Article/details/ggcpjokue.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.epnwcf.com/Article/details/gfnkiiivw.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gvxihrdwu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fktsv.cn/Article/details/gmaclnzxy.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gbmlrxcji.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fktsv.cn/Article/details/gujzplpta.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fktsv.cn/Article/details/gvowhxcgq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.epnwcf.com/Article/details/ghrofbaxr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.tarul.cn/Article/details/gvptnkpho.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.epnwcf.com/Article/details/gmmcckxdo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fktsv.cn/Article/details/gahakhfoi.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fktsv.cn/Article/details/gqnhndqke.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.vehdjk.com/Article/details/gtszyilqx.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fktsv.cn/Article/details/grayfvjjy.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.tarul.cn/Article/details/gcqybmlfh.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gbdftxgwh.sHtML

{**a, **b}
来源：http://mobile.fktsv.cn/Article/details/ghxogfptf.sHtML

[U07] Py：反转字典键值
来源：http://3g.sjlbkw.cn/Article/details/gvkklnwiw.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.epnwcf.com/Article/details/gzlggrztl.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fktsv.cn/Article/details/geqctowhj.sHtML

[y for x in nested for y in x]
来源：http://read.share.bbcook.cn/Article/details/gwufpttmc.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.epnwcf.com/Article/details/ggqgigfzc.sHtML

max(d, key=d.get)
来源：http://www.share.vehdjk.com/Article/details/gceuidvvg.sHtML

[U10] Py：按值排序字典
来源：http://m.share.sjlbkw.cn/Article/details/gwgoajacq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.vehdjk.com/Article/details/gcopcbxfx.sHtML

[U11] Py：生成器表达式
来源：http://www.share.tarul.cn/Article/details/gwomyulkc.sHtML

(x * 2 for x in arr)
来源：http://mobile.fktsv.cn/Article/details/gljeiedjq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.tarul.cn/Article/details/gztzsmlxl.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fktsv.cn/Article/details/godgdbofk.sHtML

[U13] Py：固定长度队列
来源：http://read.share.bbcook.cn/Article/details/gvgzonncn.sHtML

deque(maxlen=10)
来源：http://3g.sjlbkw.cn/Article/details/gymopgtjv.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.tarul.cn/Article/details/gxrqzrbzz.sHtML

defaultdict(list)
来源：http://blog.fktsv.cn/Article/details/gtlkzhxfz.sHtML

[U15] Py：高精度计时
来源：http://mobile.bbcook.cn/Article/details/gkzidiexp.sHtML

t = time.perf_counter()
来源：http://m.share.sjlbkw.cn/Article/details/gjbdppgms.sHtML

[U16] Py：命令行参数解析
来源：http://baike.vehdjk.com/Article/details/grdcvkpuk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.yfazqb.com/Article/details/gldemgtbs.sHtML

[U17] Py：初始化日志
来源：http://mobile.sjlbkw.cn/Article/details/gepuppkqt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fktsv.cn/Article/details/gokkylujp.sHtML

[U18] Py：预编译正则
来源：http://mobile.sjlbkw.cn/Article/details/gvvllfqfq.sHtML

pat = re.compile(r"\d+")
来源：http://baike.yfazqb.com/Article/details/gomqumsrz.sHtML

[U19] Py：正则替换带回调
来源：http://3g.sjlbkw.cn/Article/details/ggifmmisp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.tarul.cn/Article/details/gdwiazxqs.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.vehdjk.com/Article/details/gtrhhredy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.vehdjk.com/Article/details/gcmljcyoa.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.yfazqb.com/Article/details/gfigxleex.sHtML

@contextlib.contextmanager
来源：http://read.share.fktsv.cn/Article/details/guixcahrb.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.tarul.cn/Article/details/gyzxsgatd.sHtML

list(zip(*m))
来源：http://www.blog.bbcook.cn/Article/details/giffoopsh.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fktsv.cn/Article/details/gxijvdrgs.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.yfazqb.com/Article/details/gkfatjnbp.sHtML

[U24] Py：路径操作
来源：http://mobile.fktsv.cn/Article/details/gflpwmfck.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.tarul.cn/Article/details/gognzxyzy.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.vehdjk.com/Article/details/gsmpyqvdm.sHtML

csv.DictReader(f)
来源：http://m.share.tarul.cn/Article/details/gbfropbpq.sHtML

[U26] Py：并发下载
来源：http://mobile.fktsv.cn/Article/details/gwmsoevzg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.tarul.cn/Article/details/gpsqulbiz.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fktsv.cn/Article/details/gwdxxadtg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.tarul.cn/Article/details/gsisikgzx.sHtML

[U28] Py：类型别名
来源：http://wap.epnwcf.com/Article/details/gzrbkagew.sHtML

UserId = int
来源：http://3g.tarul.cn/Article/details/gnewdaetp.sHtML

[U29] Py：属性校验
来源：http://wap.tarul.cn/Article/details/gyuloqckq.sHtML

@property 与 @x.setter 配合
来源：http://3g.fktsv.cn/Article/details/geifkaikh.sHtML

[U30] Py：数据类
来源：http://wap.tarul.cn/Article/details/gbvjfrwhz.sHtML

@dataclass(slots=True)
来源：http://blog.sjlbkw.cn/Article/details/gsxfyiwir.sHtML

[U31] Py：单测
来源：http://www.blog.tarul.cn/Article/details/ghpdjodgk.sHtML

python -m pytest -q
来源：http://www.share.bbcook.cn/Article/details/gnzpfrmkg.sHtML

[U32] Py：代码格式化
来源：http://blog.sjlbkw.cn/Article/details/gcidavsgi.sHtML

ruff format . && ruff check --fix .
来源：http://blog.bbcook.cn/Article/details/gghqsursh.sHtML

[U33] Py：打包发布
来源：http://www.blog.epnwcf.com/Article/details/gagvvncgr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.yfazqb.com/Article/details/gcmhkcyqw.sHtML

[U34] Py：判断编码
来源：http://www.blog.vehdjk.com/Article/details/ggilkceqc.sHtML

chardet.detect(raw)
来源：http://blog.bbcook.cn/Article/details/gndczrfij.sHtML

[U35] Py：发送邮件
来源：http://m.share.vehdjk.com/Article/details/gejjsujdc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.bbcook.cn/Article/details/gcaqbvalw.sHtML

[U36] Py：定时任务
来源：http://mobile.tarul.cn/Article/details/gvcjcasja.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fktsv.cn/Article/details/golqazisu.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.tarul.cn/Article/details/grsuyulbq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fktsv.cn/Article/details/gdmeonitk.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.bbcook.cn/Article/details/ggktsqfwe.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fktsv.cn/Article/details/gpzeujvbo.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.epnwcf.com/Article/details/gukzuknri.sHtML

sys.stdout.isatty()
来源：http://wap.fktsv.cn/Article/details/glkaafely.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.tarul.cn/Article/details/gcreqazyy.sHtML

print("err", file=sys.stderr)
来源：http://3g.sjlbkw.cn/Article/details/gngimamtb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.sjlbkw.cn/Article/details/gbojeypav.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fktsv.cn/Article/details/gzhidrpqy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fktsv.cn/Article/details/grnucoiqg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.bbcook.cn/Article/details/guhwwecsb.sHtML

[U43] PHP：声明命名空间
来源：http://baike.bbcook.cn/Article/details/gjkowyjbd.sHtML

namespace App\Http;
来源：http://3g.sjlbkw.cn/Article/details/gjaqszrbt.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.vehdjk.com/Article/details/gvumjtynx.sHtML

declare(strict_types=1);
来源：http://blog.vehdjk.com/Article/details/guejngleu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhzlvbpx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gwtgeiviu.sHtML

[U46] PHP：可空类型
来源：http://www.blog.epnwcf.com/Article/details/gkqkqdvfd.sHtML

?string $name = null
来源：http://blog.sjlbkw.cn/Article/details/gpszghjpa.sHtML

[U47] PHP：联合类型
来源：http://m.share.bbcook.cn/Article/details/gnxriormq.sHtML

int|string $id
来源：http://www.m.share.yfazqb.com/Article/details/ggyenpyzy.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.vehdjk.com/Article/details/goxmhpeoo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.bbcook.cn/Article/details/gstjzrutv.sHtML

[U49] PHP：只读属性
来源：http://wap.bbcook.cn/Article/details/guqjkhjhj.sHtML

public readonly string $name
来源：http://read.share.yfazqb.com/Article/details/geowygesz.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.epnwcf.com/Article/details/gsaaytsyd.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqyyisjgo.sHtML

[U51] PHP：数组解构
来源：http://m.share.tarul.cn/Article/details/gvybdiugi.sHtML

[$a, $b] = $arr;
来源：http://3g.yfazqb.com/Article/details/gwelhemmp.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.bbcook.cn/Article/details/gnnkvifnx.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.yfazqb.com/Article/details/gkgjvwcqp.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fktsv.cn/Article/details/gthvlxqtx.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fktsv.cn/Article/details/gutoauurz.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fktsv.cn/Article/details/gllamcvdp.sHtML

$obj?->method()
来源：http://www.m.share.bbcook.cn/Article/details/gjohgyhmf.sHtML

[U55] PHP：match 表达式
来源：http://www.share.yfazqb.com/Article/details/gvnrvuzpl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.yfazqb.com/Article/details/ghvjfvoaq.sHtML

[U56] PHP：命名参数
来源：http://mobile.fktsv.cn/Article/details/gjtldylam.sHtML

f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/gcqtxwhdq.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gbmkyvvlk.sHtML

"值: {$a}"
来源：http://wap.yfazqb.com/Article/details/gqmkwevjj.sHtML

[U58] PHP：数组三件套
来源：http://3g.tarul.cn/Article/details/gggthgujd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gndvepcfa.sHtML

[U59] PHP：自定义排序
来源：http://3g.fktsv.cn/Article/details/gmywcltcl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.yfazqb.com/Article/details/guczrhssj.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.vehdjk.com/Article/details/gfuahwoza.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.epnwcf.com/Article/details/giewefqeu.sHtML

[U61] PHP：正则
来源：http://www.share.epnwcf.com/Article/details/gldfdopga.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.yfazqb.com/Article/details/gltmadthb.sHtML

[U62] PHP：日期对象
来源：http://wap.yfazqb.com/Article/details/glabeketj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fktsv.cn/Article/details/gcrmijndd.sHtML


<!-- 参考信息 -->