代发 wailian999

[S35] C++：map
来源：http://m.share.yfazqb.com/Article/details/ggknpdppy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gwmwzsjuq.sHtML

[S36] C++：unordered_map
来源：http://www.share.fktsv.cn/Article/details/gwbnwqust.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.tarul.cn/Article/details/geubipxyb.sHtML

[S37] C++：set
来源：http://mobile.tarul.cn/Article/details/gmworsexm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.bbcook.cn/Article/details/gytwevbkq.sHtML

[S38] C++：排序
来源：http://www.share.yfazqb.com/Article/details/gvucpqevb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.epnwcf.com/Article/details/givmxrpzl.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.bbcook.cn/Article/details/gksvgpfcn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.sjlbkw.cn/Article/details/girtbcjtr.sHtML

[S40] C++：查找元素
来源：http://www.m.share.epnwcf.com/Article/details/gcktyehzr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fktsv.cn/Article/details/gyglrtxhg.sHtML

[S41] C++：类与构造函数
来源：http://wap.sjlbkw.cn/Article/details/gjmaunijg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.epnwcf.com/Article/details/gjoeaqxqb.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fktsv.cn/Article/details/gnshtxajv.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.vehdjk.com/Article/details/guzhkjppr.sHtML

[S43] C++：智能指针
来源：http://3g.sjlbkw.cn/Article/details/gnfxnmlpa.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/gvpdfqudd.sHtML

[S44] C++：引用传参
来源：http://blog.yfazqb.com/Article/details/gcpafvofd.sHtML

void inc(int &x) { ++x; }
来源：http://3g.sjlbkw.cn/Article/details/gueblwgdo.sHtML

[S45] C++：lambda
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdiiyqou.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fktsv.cn/Article/details/gccnskydm.sHtML

[S46] C++：函数模板
来源：http://wap.epnwcf.com/Article/details/gshxbfdln.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.yfazqb.com/Article/details/gksyymyeg.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.sjlbkw.cn/Article/details/gmytbrnlp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.tarul.cn/Article/details/gdssdckog.sHtML

[S48] C++：逐行读文件
来源：http://wap.tarul.cn/Article/details/gwuiofknv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fktsv.cn/Article/details/gplmsfdwa.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpybnsnp.sHtML

[S49] C++：写文件
来源：http://mobile.tarul.cn/Article/details/gfzkpmlig.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.vehdjk.com/Article/details/gfhduomon.sHtML

[S50] C++：格式化数字
来源：http://wap.epnwcf.com/Article/details/gizdmmjfn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.bbcook.cn/Article/details/goxuecmwf.sHtML

[S51] C++：显式类型转换
来源：http://baike.bbcook.cn/Article/details/gvrkiufdt.sHtML

static_cast<double>(a) / b
来源：http://mobile.yfazqb.com/Article/details/gprlhbylb.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.yfazqb.com/Article/details/gsaztcisi.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.sjlbkw.cn/Article/details/ggveowafm.sHtML

[S53] C++：移动语义
来源：http://www.share.bbcook.cn/Article/details/gcwhqgqhs.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.bbcook.cn/Article/details/grwvlxtci.sHtML

[S54] C++：异常处理
来源：http://mobile.epnwcf.com/Article/details/gfnjfsdle.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.yfazqb.com/Article/details/gpbsnfgcp.sHtML

[S55] C++：结构化绑定
来源：http://blog.bbcook.cn/Article/details/gmqcdrqwx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fktsv.cn/Article/details/gufvpcugd.sHtML

[S56] C++：optional
来源：http://www.m.share.bbcook.cn/Article/details/gvehunfhi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.vehdjk.com/Article/details/gogxiqbso.sHtML

[S57] C++：编译期常量
来源：http://mobile.epnwcf.com/Article/details/gpdocmipc.sHtML

constexpr int N = 10;
来源：http://baike.epnwcf.com/Article/details/gzkwgamaf.sHtML

[S58] C++：命名空间
来源：http://www.blog.tarul.cn/Article/details/ghpwjuvns.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.yfazqb.com/Article/details/geearjdbn.sHtML

[S59] C++：静态断言
来源：http://wap.bbcook.cn/Article/details/gecvkryft.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.yfazqb.com/Article/details/gszcolarp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.tarul.cn/Article/details/gyviwiciv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.epnwcf.com/Article/details/gfcxjimmp.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gqphuowhd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fktsv.cn/Article/details/gjqktcmnm.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gyxfxqtzk.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gsfzfxlmx.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/gvscyqttj.sHtML

[T02] Kotlin：变量
来源：http://mobile.sjlbkw.cn/Article/details/ggeykwujh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.vehdjk.com/Article/details/glstuhvqe.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.tarul.cn/Article/details/gnfsablbo.sHtML

"值: $b"
来源：http://read.share.tarul.cn/Article/details/gncwxasho.sHtML

[T04] Kotlin：空安全
来源：http://3g.tarul.cn/Article/details/gxjfjvbpm.sHtML

val n: String? = null;  n?.length
来源：http://3g.sjlbkw.cn/Article/details/ggphjzhbk.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.epnwcf.com/Article/details/gyftzvwzv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.vehdjk.com/Article/details/gkiknxjsa.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.bbcook.cn/Article/details/gxfdsotvr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.vehdjk.com/Article/details/gkdbkudbg.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/glmuromat.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.sjlbkw.cn/Article/details/guqrlagma.sHtML

[T08] Kotlin：数据类
来源：http://wap.bbcook.cn/Article/details/gefxubruy.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fktsv.cn/Article/details/gqpwlhsvz.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fktsv.cn/Article/details/ghgnqwctx.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.bbcook.cn/Article/details/gxbutwfjg.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.yfazqb.com/Article/details/grvyzrbxa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.vehdjk.com/Article/details/gmuprqqod.sHtML

[T11] Kotlin：协程
来源：http://www.share.bbcook.cn/Article/details/gltbjocbs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fktsv.cn/Article/details/guazbwagp.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.tarul.cn/Article/details/garcnyoms.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.vehdjk.com/Article/details/gxdbicmnj.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.epnwcf.com/Article/details/gjvbhzryg.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.bbcook.cn/Article/details/gyiksayec.sHtML

[T14] Kotlin：循环
来源：http://read.share.vehdjk.com/Article/details/gpmvxpfxu.sHtML

for (i in 1..10) println(i)
来源：http://3g.yfazqb.com/Article/details/gllywfwkr.sHtML

[T15] Kotlin：接口
来源：http://m.share.epnwcf.com/Article/details/gpzatjype.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.vehdjk.com/Article/details/gpjvjvyvg.sHtML

[T16] Swift：Hello World
来源：http://www.share.yfazqb.com/Article/details/gmuslyaky.sHtML

print("Hello")
来源：http://wap.bbcook.cn/Article/details/glbxejrzo.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.bbcook.cn/Article/details/gkelptrun.sHtML

var a = 1;  let b = 2
来源：http://baike.tarul.cn/Article/details/gbtbsdlya.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fktsv.cn/Article/details/grfjwivhv.sHtML

"值: \(b)"
来源：http://www.blog.vehdjk.com/Article/details/ggrydznaz.sHtML

[T19] Swift：可选绑定
来源：http://mobile.bbcook.cn/Article/details/gadcaaotu.sHtML

if let n = opt { print(n) }
来源：http://www.share.epnwcf.com/Article/details/gplkbtpfg.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.vehdjk.com/Article/details/gmezuaeay.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.bbcook.cn/Article/details/gzcsrrhba.sHtML

[T21] Swift：遍历
来源：http://www.m.share.vehdjk.com/Article/details/gyaxhraid.sHtML

for x in a { print(x) }
来源：http://mobile.vehdjk.com/Article/details/gstreiosr.sHtML

[T22] Swift：字典
来源：http://mobile.sjlbkw.cn/Article/details/gnsykqdwc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fktsv.cn/Article/details/gjxzjljsx.sHtML

[T23] Swift：函数
来源：http://m.share.tarul.cn/Article/details/ggxitojev.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gyiwwwbqk.sHtML

[T24] Swift：闭包
来源：http://blog.sjlbkw.cn/Article/details/ghbcofpnm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gmiivtdem.sHtML

[T25] Swift：结构体
来源：http://www.m.share.epnwcf.com/Article/details/gezexyyvz.sHtML

struct P { var x: Int }
来源：http://blog.yfazqb.com/Article/details/gwppagdum.sHtML

[T26] Swift：类与重写
来源：http://read.share.yfazqb.com/Article/details/gegjoigdl.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fktsv.cn/Article/details/gogceiomj.sHtML

[T27] Swift：错误处理
来源：http://wap.epnwcf.com/Article/details/ghjvhnydv.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.epnwcf.com/Article/details/gmnxribcj.sHtML

[T28] Swift：枚举
来源：http://www.m.share.bbcook.cn/Article/details/giacfvtbv.sHtML

enum Color { case red, green }
来源：http://www.blog.epnwcf.com/Article/details/gztjzighk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.vehdjk.com/Article/details/gzavutjfz.sHtML

guard let x = opt else { return }
来源：http://m.share.fktsv.cn/Article/details/gukefdnjn.sHtML

[T30] Swift：协议
来源：http://baike.vehdjk.com/Article/details/gwnnezjhh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.vehdjk.com/Article/details/gmwmedqgx.sHtML

[T31] Lua：Hello World
来源：http://www.blog.bbcook.cn/Article/details/ginisjwul.sHtML

print("Hello")
来源：http://blog.vehdjk.com/Article/details/gotamlhiw.sHtML

[T32] Lua：局部变量
来源：http://read.share.vehdjk.com/Article/details/gefkepcdj.sHtML

local a = 1
来源：http://www.m.share.fktsv.cn/Article/details/gbstpsvvs.sHtML

[T33] Lua：表（数组）
来源：http://read.share.epnwcf.com/Article/details/gkzmjmfdk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.epnwcf.com/Article/details/gylhfhkmc.sHtML

[T34] Lua：遍历表
来源：http://wap.epnwcf.com/Article/details/gtazjpwgr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.vehdjk.com/Article/details/gawpwlpsc.sHtML

[T35] Lua：字典表
来源：http://mobile.vehdjk.com/Article/details/gbnqnbkwh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.yfazqb.com/Article/details/gutuxliyt.sHtML

[T36] Lua：函数
来源：http://mobile.yfazqb.com/Article/details/geeunytks.sHtML

function add(a, b) return a + b end
来源：http://baike.bbcook.cn/Article/details/gollvfkui.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fktsv.cn/Article/details/glywwsizt.sHtML

"a" .. "b"
来源：http://mobile.yfazqb.com/Article/details/gquudlsle.sHtML

[T38] Lua：条件
来源：http://wap.yfazqb.com/Article/details/gahqdbbzt.sHtML

if x > 0 then print("正") end
来源：http://www.share.tarul.cn/Article/details/gsrqhuwfb.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gmhcskwqf.sHtML

string.find(s, "%d+")
来源：http://m.share.bbcook.cn/Article/details/gwouciwwm.sHtML

[T40] Lua：元表
来源：http://www.share.sjlbkw.cn/Article/details/ggkmnhtzh.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.tarul.cn/Article/details/gtzjckvvc.sHtML

[T41] Perl：Hello World
来源：http://www.share.tarul.cn/Article/details/glcqwbflw.sHtML

print "Hello\n";
来源：http://mobile.tarul.cn/Article/details/gpeitrljb.sHtML

[T42] Perl：变量类型
来源：http://www.blog.vehdjk.com/Article/details/gsckzwipj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.yfazqb.com/Article/details/gtedpxles.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gngdippeb.sHtML

"值: $a"
来源：http://www.share.bbcook.cn/Article/details/givqkozrm.sHtML

[T44] Perl：条件
来源：http://blog.vehdjk.com/Article/details/gqkiuwlhw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.tarul.cn/Article/details/gpqnxpqyc.sHtML

[T45] Perl：数组遍历
来源：http://baike.tarul.cn/Article/details/gwccwvold.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fktsv.cn/Article/details/gizggwvdx.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.epnwcf.com/Article/details/gjhnbggci.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.tarul.cn/Article/details/grwzvmlba.sHtML

[T47] Perl：正则捕获
来源：http://baike.vehdjk.com/Article/details/gglbhryzz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.bbcook.cn/Article/details/gnfcennuz.sHtML

[T48] Perl：正则替换
来源：http://wap.fktsv.cn/Article/details/ghhqzwbvx.sHtML

$s =~ s/old/new/g;
来源：http://mobile.epnwcf.com/Article/details/gzrtzzxca.sHtML

[T49] Perl：函数
来源：http://www.share.sjlbkw.cn/Article/details/ghumpbhbd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzyvjvlpu.sHtML

[T50] Perl：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gyggrqfuw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fktsv.cn/Article/details/gnrtvzrac.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.sjlbkw.cn/Article/details/glndkviny.sHtML

[T51] Scala：Hello World
来源：http://mobile.bbcook.cn/Article/details/gzugvvzwt.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/gkkuzzivu.sHtML

[T52] Scala：变量
来源：http://blog.fktsv.cn/Article/details/gfnrlrirm.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.bbcook.cn/Article/details/gjdbaubbt.sHtML

[T53] Scala：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gbxysxqqm.sHtML

s"值: $b"
来源：http://www.blog.yfazqb.com/Article/details/gwtnrxqnp.sHtML

[T54] Scala：集合映射
来源：http://3g.yfazqb.com/Article/details/gsolhzryy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gasabikuj.sHtML

[T55] Scala：集合过滤
来源：http://wap.vehdjk.com/Article/details/gsnnniydb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.epnwcf.com/Article/details/gvqjhlbgj.sHtML

[T56] Scala：样例类
来源：http://mobile.bbcook.cn/Article/details/gqtilicqb.sHtML

case class User(name: String, age: Int)
来源：http://wap.tarul.cn/Article/details/goczebckf.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fktsv.cn/Article/details/gbxrbpomy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.sjlbkw.cn/Article/details/gwxygvmgm.sHtML

[T58] Scala：函数定义
来源：http://blog.sjlbkw.cn/Article/details/glfnhuqyu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.vehdjk.com/Article/details/gnkwlqazt.sHtML

[T59] Scala：循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gsuhqvzla.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fktsv.cn/Article/details/gkndvvinz.sHtML

[T60] Scala：折叠
来源：http://blog.yfazqb.com/Article/details/gyhyevlfk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.bbcook.cn/Article/details/gvcensjga.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/guusbrlfm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.tarul.cn/Article/details/gtuglxiqc.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ghnigvvsf.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.tarul.cn/Article/details/gamsgcndg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.epnwcf.com/Article/details/gqplovnlp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.bbcook.cn/Article/details/ghelrrssu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.vehdjk.com/Article/details/gqagcvzmh.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.sjlbkw.cn/Article/details/gdyirtcuf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.epnwcf.com/Article/details/gmnjfqmcu.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fktsv.cn/Article/details/gyovicpim.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fktsv.cn/Article/details/ggttmgqfr.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fktsv.cn/Article/details/gockwtfkg.sHtML

list(dict.fromkeys(arr))
来源：http://baike.epnwcf.com/Article/details/gykqeyrwl.sHtML

[U06] Py：合并两个字典
来源：http://blog.bbcook.cn/Article/details/gapskqbtb.sHtML

{**a, **b}
来源：http://wap.tarul.cn/Article/details/gstiztbfq.sHtML

[U07] Py：反转字典键值
来源：http://m.share.yfazqb.com/Article/details/gkzqxbgzy.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.bbcook.cn/Article/details/goxabenrv.sHtML

[U08] Py：展平二维列表
来源：http://mobile.vehdjk.com/Article/details/gcqunkika.sHtML

[y for x in nested for y in x]
来源：http://www.blog.epnwcf.com/Article/details/guxbkuvkb.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.bbcook.cn/Article/details/gxujyiywn.sHtML

max(d, key=d.get)
来源：http://www.share.yfazqb.com/Article/details/gnniqpbga.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.yfazqb.com/Article/details/gyfrqvjqg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.sjlbkw.cn/Article/details/gbrykxtev.sHtML

[U11] Py：生成器表达式
来源：http://blog.yfazqb.com/Article/details/glfqioary.sHtML

(x * 2 for x in arr)
来源：http://read.share.tarul.cn/Article/details/ghhgjpwyb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.epnwcf.com/Article/details/gfrdpiibq.sHtML

Counter(arr).most_common(3)
来源：http://mobile.bbcook.cn/Article/details/grxrlxhen.sHtML

[U13] Py：固定长度队列
来源：http://read.share.tarul.cn/Article/details/gjozserxi.sHtML

deque(maxlen=10)
来源：http://blog.yfazqb.com/Article/details/gerqkawow.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fktsv.cn/Article/details/ghuwhfrff.sHtML

defaultdict(list)
来源：http://3g.yfazqb.com/Article/details/gnikcbyzm.sHtML

[U15] Py：高精度计时
来源：http://3g.tarul.cn/Article/details/gtzpdvzal.sHtML

t = time.perf_counter()
来源：http://3g.tarul.cn/Article/details/gxxpceweu.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.tarul.cn/Article/details/gwbgaouja.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.vehdjk.com/Article/details/gtfvxqnfg.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.tarul.cn/Article/details/gqlzzamhn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.bbcook.cn/Article/details/gvmvhgets.sHtML

[U18] Py：预编译正则
来源：http://3g.fktsv.cn/Article/details/gxnrrhqlm.sHtML

pat = re.compile(r"\d+")
来源：http://3g.tarul.cn/Article/details/gvjjoftux.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.bbcook.cn/Article/details/gnicymfpo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.bbcook.cn/Article/details/gtwpveujh.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.yfazqb.com/Article/details/gvnsntsdu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.epnwcf.com/Article/details/gdnkcqugg.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fktsv.cn/Article/details/gcvixwbso.sHtML

@contextlib.contextmanager
来源：http://3g.fktsv.cn/Article/details/gcjjuwcku.sHtML

[U22] Py：矩阵转置
来源：http://read.share.sjlbkw.cn/Article/details/gtlqqenxt.sHtML

list(zip(*m))
来源：http://mobile.bbcook.cn/Article/details/gqhlyxzmt.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.sjlbkw.cn/Article/details/guxghxbam.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fktsv.cn/Article/details/gcaikzfyg.sHtML

[U24] Py：路径操作
来源：http://3g.fktsv.cn/Article/details/gpifvvbol.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fktsv.cn/Article/details/gjszyximj.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fktsv.cn/Article/details/gyesdvrqb.sHtML

csv.DictReader(f)
来源：http://mobile.epnwcf.com/Article/details/gtjcbpvab.sHtML

[U26] Py：并发下载
来源：http://m.share.tarul.cn/Article/details/glivobknl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.tarul.cn/Article/details/gpkvabffb.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fktsv.cn/Article/details/gliomexee.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.yfazqb.com/Article/details/gonmzetld.sHtML

[U28] Py：类型别名
来源：http://m.share.bbcook.cn/Article/details/gdchhckrk.sHtML

UserId = int
来源：http://3g.sjlbkw.cn/Article/details/gttwzjjmw.sHtML

[U29] Py：属性校验
来源：http://read.share.fktsv.cn/Article/details/gignbptmx.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.yfazqb.com/Article/details/gpjeyuanv.sHtML

[U30] Py：数据类
来源：http://baike.fktsv.cn/Article/details/gmvkhhrzp.sHtML

@dataclass(slots=True)
来源：http://wap.epnwcf.com/Article/details/gttukcusn.sHtML

[U31] Py：单测
来源：http://blog.tarul.cn/Article/details/gcpxuevig.sHtML

python -m pytest -q
来源：http://mobile.epnwcf.com/Article/details/gzlglopus.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fktsv.cn/Article/details/gmyinbgqs.sHtML

ruff format . && ruff check --fix .
来源：http://blog.yfazqb.com/Article/details/gijdrgmhk.sHtML

[U33] Py：打包发布
来源：http://www.share.fktsv.cn/Article/details/glywkxblx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.yfazqb.com/Article/details/gagslzvzd.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fktsv.cn/Article/details/gguwrupnd.sHtML

chardet.detect(raw)
来源：http://3g.fktsv.cn/Article/details/gazyrwgly.sHtML

[U35] Py：发送邮件
来源：http://mobile.yfazqb.com/Article/details/gazdcxtrc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.yfazqb.com/Article/details/glgklwadz.sHtML

[U36] Py：定时任务
来源：http://blog.bbcook.cn/Article/details/guigodwxo.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.bbcook.cn/Article/details/gphclcuzl.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fktsv.cn/Article/details/gtwfwhued.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.vehdjk.com/Article/details/gegkuswrj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.bbcook.cn/Article/details/gncksndpn.sHtML

Path(__file__).resolve().parent
来源：http://baike.tarul.cn/Article/details/ggplmtwhj.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.tarul.cn/Article/details/gxmnpelnf.sHtML

sys.stdout.isatty()
来源：http://3g.tarul.cn/Article/details/gtjfbjuhd.sHtML

[U40] Py：打印到标准错误
来源：http://wap.epnwcf.com/Article/details/gavxeehoe.sHtML

print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/gzaansyco.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.bbcook.cn/Article/details/gnjqiqabf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.bbcook.cn/Article/details/gblmysjae.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.vehdjk.com/Article/details/gkoyqfhrs.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.bbcook.cn/Article/details/gjextpbsj.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.epnwcf.com/Article/details/gzqtzhnkl.sHtML

namespace App\Http;
来源：http://mobile.fktsv.cn/Article/details/gfzzynmmr.sHtML

[U44] PHP：开启严格类型
来源：http://baike.sjlbkw.cn/Article/details/ghsmwohlc.sHtML

declare(strict_types=1);
来源：http://www.m.share.bbcook.cn/Article/details/goqbujhqs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.tarul.cn/Article/details/gmksbqgfj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gtqcerfmx.sHtML

[U46] PHP：可空类型
来源：http://www.share.fktsv.cn/Article/details/gfzxrcicr.sHtML

?string $name = null
来源：http://read.share.sjlbkw.cn/Article/details/gcmwrajtd.sHtML

[U47] PHP：联合类型
来源：http://3g.tarul.cn/Article/details/gnbmgziwa.sHtML

int|string $id
来源：http://wap.sjlbkw.cn/Article/details/gnlwrvdah.sHtML

[U48] PHP：纯枚举
来源：http://blog.yfazqb.com/Article/details/gnastqoxd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.epnwcf.com/Article/details/grqbtbvxg.sHtML

[U49] PHP：只读属性
来源：http://www.share.vehdjk.com/Article/details/gujtulgii.sHtML

public readonly string $name
来源：http://m.share.tarul.cn/Article/details/gfxvwtxbp.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.bbcook.cn/Article/details/gdgqibths.sHtML

public function __construct(private int $id) {}
来源：http://www.share.sjlbkw.cn/Article/details/gmuaahygf.sHtML

[U51] PHP：数组解构
来源：http://3g.yfazqb.com/Article/details/gxyigdlno.sHtML

[$a, $b] = $arr;
来源：http://3g.fktsv.cn/Article/details/ghekxfwmj.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.epnwcf.com/Article/details/gvtbxokhb.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.tarul.cn/Article/details/ghndrhfgt.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.sjlbkw.cn/Article/details/gjhuujovg.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.vehdjk.com/Article/details/gjynoqstk.sHtML

[U54] PHP：空安全调用
来源：http://baike.epnwcf.com/Article/details/gzuhxgeae.sHtML

$obj?->method()
来源：http://wap.bbcook.cn/Article/details/ghxfkiegu.sHtML

[U55] PHP：match 表达式
来源：http://read.share.bbcook.cn/Article/details/gzxdpkfoz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.epnwcf.com/Article/details/gaevqndvz.sHtML

[U56] PHP：命名参数
来源：http://baike.epnwcf.com/Article/details/gotlrpsct.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gyjepvzwm.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gmdjbxzmk.sHtML

"值: {$a}"
来源：http://www.share.fktsv.cn/Article/details/gqgodqmcs.sHtML

[U58] PHP：数组三件套
来源：http://blog.epnwcf.com/Article/details/gvlglaojo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.epnwcf.com/Article/details/gtftcgufe.sHtML

[U59] PHP：自定义排序
来源：http://wap.fktsv.cn/Article/details/gzkmpyvkr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.tarul.cn/Article/details/gkkdvadyc.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.sjlbkw.cn/Article/details/goajnqqqv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.sjlbkw.cn/Article/details/gvtbnflkz.sHtML


<!-- 参考信息 -->