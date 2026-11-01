代发 wailian999

[S35] C++：map
来源：http://mobile.fktsv.cn/Article/details/giarmnont.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gbfsnveof.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.vehdjk.com/Article/details/geivukxup.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gechzehmd.sHtML

[S37] C++：set
来源：http://read.share.vehdjk.com/Article/details/gblanktip.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fktsv.cn/Article/details/gtqrkaitf.sHtML

[S38] C++：排序
来源：http://read.share.yfazqb.com/Article/details/godxsbscy.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.yfazqb.com/Article/details/gnlbfatje.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.tarul.cn/Article/details/gdrjqqelx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.vehdjk.com/Article/details/gzgopvdga.sHtML

[S40] C++：查找元素
来源：http://blog.sjlbkw.cn/Article/details/gpltjtmfj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.vehdjk.com/Article/details/gulrllwmi.sHtML

[S41] C++：类与构造函数
来源：http://read.share.tarul.cn/Article/details/ghanvwlcq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.bbcook.cn/Article/details/gqtmyazri.sHtML

[S42] C++：继承与虚函数
来源：http://baike.tarul.cn/Article/details/gnunfzepv.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.yfazqb.com/Article/details/gmzsapizo.sHtML

[S43] C++：智能指针
来源：http://www.m.share.vehdjk.com/Article/details/gvzhlkjee.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.yfazqb.com/Article/details/gyvscgqlt.sHtML

[S44] C++：引用传参
来源：http://m.share.tarul.cn/Article/details/gmwlaqiqa.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.vehdjk.com/Article/details/gywzdcjbw.sHtML

[S45] C++：lambda
来源：http://baike.sjlbkw.cn/Article/details/grcakppwe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.epnwcf.com/Article/details/glhbiwqko.sHtML

[S46] C++：函数模板
来源：http://mobile.vehdjk.com/Article/details/gmstemyky.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fktsv.cn/Article/details/grkhevcub.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.vehdjk.com/Article/details/gouqjbwmk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.tarul.cn/Article/details/gsypfujbs.sHtML

[S48] C++：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gltuwbjpi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.bbcook.cn/Article/details/gkvghklzj.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.tarul.cn/Article/details/gujufnpwc.sHtML

[S49] C++：写文件
来源：http://m.share.fktsv.cn/Article/details/gawytzoot.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fktsv.cn/Article/details/gjqrztuap.sHtML

[S50] C++：格式化数字
来源：http://blog.yfazqb.com/Article/details/gxhcnekcu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.tarul.cn/Article/details/gnxnndzco.sHtML

[S51] C++：显式类型转换
来源：http://mobile.bbcook.cn/Article/details/gkiszdogu.sHtML

static_cast<double>(a) / b
来源：http://wap.vehdjk.com/Article/details/gkivczubc.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.sjlbkw.cn/Article/details/gwxspaofk.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fktsv.cn/Article/details/gomosgjxz.sHtML

[S53] C++：移动语义
来源：http://m.share.sjlbkw.cn/Article/details/gybekcnoj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fktsv.cn/Article/details/gfwbsknfx.sHtML

[S54] C++：异常处理
来源：http://m.share.vehdjk.com/Article/details/gdepzynyx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.bbcook.cn/Article/details/gzujncwwy.sHtML

[S55] C++：结构化绑定
来源：http://blog.tarul.cn/Article/details/gmhrbcuko.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.vehdjk.com/Article/details/ggwzzkkct.sHtML

[S56] C++：optional
来源：http://www.share.sjlbkw.cn/Article/details/gzopsacqf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.vehdjk.com/Article/details/gquryksmc.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.sjlbkw.cn/Article/details/gymvphsla.sHtML

constexpr int N = 10;
来源：http://mobile.tarul.cn/Article/details/gtantaeaj.sHtML

[S58] C++：命名空间
来源：http://m.share.fktsv.cn/Article/details/gapcsbswn.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fktsv.cn/Article/details/guxeqfhbp.sHtML

[S59] C++：静态断言
来源：http://m.share.epnwcf.com/Article/details/gceiwteno.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.tarul.cn/Article/details/gtqlfbwmz.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.vehdjk.com/Article/details/gijhckasv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.bbcook.cn/Article/details/gzanfkrdk.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gbvavdfng.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.tarul.cn/Article/details/gnetdlrln.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gblpobwhq.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gbzehuwso.sHtML

println("Hello")
来源：http://www.share.fktsv.cn/Article/details/gjvqdvmzs.sHtML

[T02] Kotlin：变量
来源：http://wap.fktsv.cn/Article/details/gpjqfgumt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.epnwcf.com/Article/details/gtyszsegk.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.tarul.cn/Article/details/gxmluhivw.sHtML

"值: $b"
来源：http://wap.tarul.cn/Article/details/gcthvsgfm.sHtML

[T04] Kotlin：空安全
来源：http://mobile.epnwcf.com/Article/details/gnsfaliws.sHtML

val n: String? = null;  n?.length
来源：http://3g.bbcook.cn/Article/details/ghvyxfpyn.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gskaxyocn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.sjlbkw.cn/Article/details/gzcjtxeqx.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.yfazqb.com/Article/details/guvpduqdy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.yfazqb.com/Article/details/gqnoqzxtr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/gafdzhkuj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fktsv.cn/Article/details/gbgdtvhrr.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fktsv.cn/Article/details/gowvnsbrx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.sjlbkw.cn/Article/details/gijaznrin.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.bbcook.cn/Article/details/guebnonji.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.epnwcf.com/Article/details/gxdxjrens.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.bbcook.cn/Article/details/gbydvsypu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.epnwcf.com/Article/details/gxfxxhuif.sHtML

[T11] Kotlin：协程
来源：http://www.share.vehdjk.com/Article/details/gwbyshlwt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.tarul.cn/Article/details/gxdmcrrlg.sHtML

[T12] Kotlin：解构声明
来源：http://blog.yfazqb.com/Article/details/gooublmih.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.tarul.cn/Article/details/giebtzhod.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.bbcook.cn/Article/details/gixiqmlpv.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.sjlbkw.cn/Article/details/gmyjhznan.sHtML

[T14] Kotlin：循环
来源：http://mobile.vehdjk.com/Article/details/ggzwhvhsk.sHtML

for (i in 1..10) println(i)
来源：http://m.share.yfazqb.com/Article/details/gejaporgg.sHtML

[T15] Kotlin：接口
来源：http://baike.bbcook.cn/Article/details/gcsilveqd.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.epnwcf.com/Article/details/gronxzsec.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gbzwjxwen.sHtML

print("Hello")
来源：http://mobile.bbcook.cn/Article/details/gpyumraba.sHtML

[T17] Swift：变量与常量
来源：http://wap.fktsv.cn/Article/details/gcqmmigla.sHtML

var a = 1;  let b = 2
来源：http://www.share.yfazqb.com/Article/details/goqgzeqre.sHtML

[T18] Swift：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gjpxxuzwp.sHtML

"值: \(b)"
来源：http://mobile.bbcook.cn/Article/details/gaqybcjlz.sHtML

[T19] Swift：可选绑定
来源：http://m.share.bbcook.cn/Article/details/gxfqzhcti.sHtML

if let n = opt { print(n) }
来源：http://mobile.sjlbkw.cn/Article/details/ghthdtpug.sHtML

[T20] Swift：数组操作
来源：http://m.share.bbcook.cn/Article/details/gjczjpitm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.sjlbkw.cn/Article/details/gauwauiwh.sHtML

[T21] Swift：遍历
来源：http://mobile.epnwcf.com/Article/details/gtpbmxveq.sHtML

for x in a { print(x) }
来源：http://blog.yfazqb.com/Article/details/gzmxsaeky.sHtML

[T22] Swift：字典
来源：http://m.share.vehdjk.com/Article/details/gbazocmwk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.yfazqb.com/Article/details/gapbxqvyg.sHtML

[T23] Swift：函数
来源：http://read.share.tarul.cn/Article/details/gjzpqwsdt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.yfazqb.com/Article/details/gkxjovaog.sHtML

[T24] Swift：闭包
来源：http://m.share.yfazqb.com/Article/details/ghaqrkjph.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.epnwcf.com/Article/details/gajrvxedq.sHtML

[T25] Swift：结构体
来源：http://wap.sjlbkw.cn/Article/details/gmpsafznc.sHtML

struct P { var x: Int }
来源：http://www.share.vehdjk.com/Article/details/glbzkefjt.sHtML

[T26] Swift：类与重写
来源：http://wap.tarul.cn/Article/details/guicteyxj.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.epnwcf.com/Article/details/grdfzcdhf.sHtML

[T27] Swift：错误处理
来源：http://3g.vehdjk.com/Article/details/gpesguqso.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.bbcook.cn/Article/details/gxxzolwdf.sHtML

[T28] Swift：枚举
来源：http://www.m.share.epnwcf.com/Article/details/gvzxrmepl.sHtML

enum Color { case red, green }
来源：http://3g.yfazqb.com/Article/details/gjffgscze.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.epnwcf.com/Article/details/geczydihz.sHtML

guard let x = opt else { return }
来源：http://www.blog.epnwcf.com/Article/details/gxprlkrks.sHtML

[T30] Swift：协议
来源：http://baike.yfazqb.com/Article/details/gwhxlwbgy.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.vehdjk.com/Article/details/gqsnjchdp.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fktsv.cn/Article/details/grwefsovn.sHtML

print("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/gopepeesv.sHtML

[T32] Lua：局部变量
来源：http://read.share.fktsv.cn/Article/details/gvnqqgciw.sHtML

local a = 1
来源：http://www.blog.fktsv.cn/Article/details/gltrscbam.sHtML

[T33] Lua：表（数组）
来源：http://m.share.tarul.cn/Article/details/gszbmmwbe.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.epnwcf.com/Article/details/ghebiyyuh.sHtML

[T34] Lua：遍历表
来源：http://www.share.bbcook.cn/Article/details/gvvpdseir.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.bbcook.cn/Article/details/gdvobvryp.sHtML

[T35] Lua：字典表
来源：http://mobile.vehdjk.com/Article/details/grqynxdik.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.tarul.cn/Article/details/grkbalpdq.sHtML

[T36] Lua：函数
来源：http://read.share.sjlbkw.cn/Article/details/gvkgozfyp.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.yfazqb.com/Article/details/gbotkxatc.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.yfazqb.com/Article/details/ggwivazbm.sHtML

"a" .. "b"
来源：http://3g.vehdjk.com/Article/details/gdmiesaic.sHtML

[T38] Lua：条件
来源：http://read.share.vehdjk.com/Article/details/gzbhpsxag.sHtML

if x > 0 then print("正") end
来源：http://m.share.fktsv.cn/Article/details/grepcpzgx.sHtML

[T39] Lua：模式匹配
来源：http://baike.bbcook.cn/Article/details/gelpduylk.sHtML

string.find(s, "%d+")
来源：http://www.m.share.epnwcf.com/Article/details/gccqbjoks.sHtML

[T40] Lua：元表
来源：http://read.share.yfazqb.com/Article/details/gnakasqnv.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.tarul.cn/Article/details/ghdlbkdbp.sHtML

[T41] Perl：Hello World
来源：http://read.share.yfazqb.com/Article/details/gtpkumxhi.sHtML

print "Hello\n";
来源：http://mobile.fktsv.cn/Article/details/ggyhndmjd.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.vehdjk.com/Article/details/grnqxuhbx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.yfazqb.com/Article/details/gihxygkyg.sHtML

[T43] Perl：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gvgvydmvh.sHtML

"值: $a"
来源：http://www.blog.yfazqb.com/Article/details/gojdynjmm.sHtML

[T44] Perl：条件
来源：http://wap.yfazqb.com/Article/details/gjejhnujo.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.yfazqb.com/Article/details/gpnvuxokp.sHtML

[T45] Perl：数组遍历
来源：http://mobile.bbcook.cn/Article/details/gvscdeudf.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.vehdjk.com/Article/details/gwhtihnra.sHtML

[T46] Perl：哈希操作
来源：http://www.share.yfazqb.com/Article/details/gbwkefcik.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.sjlbkw.cn/Article/details/ghweuibre.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.yfazqb.com/Article/details/gqbushqef.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.bbcook.cn/Article/details/gadjkgcki.sHtML

[T48] Perl：正则替换
来源：http://baike.vehdjk.com/Article/details/gkoomlxxq.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.tarul.cn/Article/details/godcvnwlq.sHtML

[T49] Perl：函数
来源：http://www.share.tarul.cn/Article/details/gcvedamou.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gyxsxdgyk.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fktsv.cn/Article/details/gpvrexxoa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.sjlbkw.cn/Article/details/grghsmwng.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.tarul.cn/Article/details/gtvykjxsr.sHtML

[T51] Scala：Hello World
来源：http://mobile.fktsv.cn/Article/details/gwhlspmdi.sHtML

println("Hello")
来源：http://mobile.fktsv.cn/Article/details/glmppjljo.sHtML

[T52] Scala：变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gqihzbafy.sHtML

val a = 1;  var b = 2
来源：http://blog.sjlbkw.cn/Article/details/gmizijlgp.sHtML

[T53] Scala：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gjhxgbgbf.sHtML

s"值: $b"
来源：http://www.share.epnwcf.com/Article/details/gsxptaqfy.sHtML

[T54] Scala：集合映射
来源：http://m.share.epnwcf.com/Article/details/gmnowzlxy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.epnwcf.com/Article/details/guasqncmn.sHtML

[T55] Scala：集合过滤
来源：http://3g.fktsv.cn/Article/details/gisruqqzj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.sjlbkw.cn/Article/details/gznmzjqzz.sHtML

[T56] Scala：样例类
来源：http://baike.fktsv.cn/Article/details/gugpjnkhk.sHtML

case class User(name: String, age: Int)
来源：http://www.share.vehdjk.com/Article/details/gruxorama.sHtML

[T57] Scala：模式匹配
来源：http://blog.yfazqb.com/Article/details/gsynanekm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjriyphmc.sHtML

[T58] Scala：函数定义
来源：http://blog.epnwcf.com/Article/details/gxvmhulby.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.bbcook.cn/Article/details/genndmlcc.sHtML

[T59] Scala：循环
来源：http://wap.vehdjk.com/Article/details/gymixwlfg.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.tarul.cn/Article/details/gydkvewbh.sHtML

[T60] Scala：折叠
来源：http://www.blog.yfazqb.com/Article/details/gimzzppzo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.bbcook.cn/Article/details/gkmwzapat.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gdnaijxpg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.yfazqb.com/Article/details/gehmiblzz.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gxbbfivkf.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.epnwcf.com/Article/details/gfhuwnlsf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.tarul.cn/Article/details/gvrwfyvfl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.vehdjk.com/Article/details/gdanvbxyb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fktsv.cn/Article/details/gsjytwctf.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.yfazqb.com/Article/details/ggrdljhyu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.yfazqb.com/Article/details/gwqlfexhu.sHtML

[U04] Py：变量调试打印
来源：http://blog.sjlbkw.cn/Article/details/gyztpnvfo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fktsv.cn/Article/details/gxnuhcipb.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.sjlbkw.cn/Article/details/gnpsvtcjs.sHtML

list(dict.fromkeys(arr))
来源：http://wap.yfazqb.com/Article/details/gmqmgejkx.sHtML

[U06] Py：合并两个字典
来源：http://wap.bbcook.cn/Article/details/gewflzrjb.sHtML

{**a, **b}
来源：http://www.m.share.epnwcf.com/Article/details/gqmvmytuk.sHtML

[U07] Py：反转字典键值
来源：http://blog.fktsv.cn/Article/details/gfxtqmvcp.sHtML

{v: k for k, v in d.items()}
来源：http://wap.sjlbkw.cn/Article/details/gwpzefzrk.sHtML

[U08] Py：展平二维列表
来源：http://blog.yfazqb.com/Article/details/gdntdkmfb.sHtML

[y for x in nested for y in x]
来源：http://baike.tarul.cn/Article/details/gbqjjqcgt.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.vehdjk.com/Article/details/gmlgagkha.sHtML

max(d, key=d.get)
来源：http://read.share.fktsv.cn/Article/details/glaldjtla.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.sjlbkw.cn/Article/details/gshtkkhwv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.bbcook.cn/Article/details/gjxlshmxw.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.epnwcf.com/Article/details/gepvnjdom.sHtML

(x * 2 for x in arr)
来源：http://3g.epnwcf.com/Article/details/gnwzyvitn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.vehdjk.com/Article/details/gxgvbjqix.sHtML

Counter(arr).most_common(3)
来源：http://wap.vehdjk.com/Article/details/gbqyeloxz.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.bbcook.cn/Article/details/gqkzumakh.sHtML

deque(maxlen=10)
来源：http://baike.epnwcf.com/Article/details/glynhvusn.sHtML

[U14] Py：分组收集到列表
来源：http://baike.epnwcf.com/Article/details/gadytaxos.sHtML

defaultdict(list)
来源：http://www.m.share.vehdjk.com/Article/details/gbowkwphd.sHtML

[U15] Py：高精度计时
来源：http://3g.bbcook.cn/Article/details/gvgsqbsbc.sHtML

t = time.perf_counter()
来源：http://baike.vehdjk.com/Article/details/gritpgxuh.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fktsv.cn/Article/details/gnkwhjwrp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.yfazqb.com/Article/details/geewmsiru.sHtML

[U17] Py：初始化日志
来源：http://baike.yfazqb.com/Article/details/gqadqhvpj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fktsv.cn/Article/details/gywtfvyri.sHtML

[U18] Py：预编译正则
来源：http://baike.bbcook.cn/Article/details/glaaeuctl.sHtML

pat = re.compile(r"\d+")
来源：http://3g.tarul.cn/Article/details/gwkpumqba.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.epnwcf.com/Article/details/gapugpjgq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.sjlbkw.cn/Article/details/guogoiiuh.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.tarul.cn/Article/details/ggbtbqnjn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.tarul.cn/Article/details/gnedrnmcl.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.bbcook.cn/Article/details/gwzzpzduk.sHtML

@contextlib.contextmanager
来源：http://www.blog.fktsv.cn/Article/details/gwnypllbt.sHtML

[U22] Py：矩阵转置
来源：http://baike.bbcook.cn/Article/details/gvvodwmjo.sHtML

list(zip(*m))
来源：http://m.share.tarul.cn/Article/details/gtqeblgnp.sHtML

[U23] Py：分块读取大文件
来源：http://wap.tarul.cn/Article/details/gfttqfcee.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.tarul.cn/Article/details/gzptptvjo.sHtML

[U24] Py：路径操作
来源：http://baike.fktsv.cn/Article/details/grlmfpjsn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.yfazqb.com/Article/details/gyfrbpwde.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fktsv.cn/Article/details/gwoyqhzll.sHtML

csv.DictReader(f)
来源：http://m.share.epnwcf.com/Article/details/griqkgyjp.sHtML

[U26] Py：并发下载
来源：http://blog.tarul.cn/Article/details/gngsdmuwo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.vehdjk.com/Article/details/gpzlfuwxa.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.sjlbkw.cn/Article/details/grqsyzjii.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.vehdjk.com/Article/details/gezfxofqj.sHtML

[U28] Py：类型别名
来源：http://3g.yfazqb.com/Article/details/gdhahhcoq.sHtML

UserId = int
来源：http://blog.tarul.cn/Article/details/gvnvcqvcc.sHtML

[U29] Py：属性校验
来源：http://3g.yfazqb.com/Article/details/gvjzkizma.sHtML

@property 与 @x.setter 配合
来源：http://m.share.sjlbkw.cn/Article/details/gbsxomexo.sHtML

[U30] Py：数据类
来源：http://mobile.fktsv.cn/Article/details/gzamjikih.sHtML

@dataclass(slots=True)
来源：http://baike.fktsv.cn/Article/details/glvubbnyo.sHtML

[U31] Py：单测
来源：http://www.blog.epnwcf.com/Article/details/gsmmjkdih.sHtML

python -m pytest -q
来源：http://mobile.tarul.cn/Article/details/gobpwmmme.sHtML

[U32] Py：代码格式化
来源：http://3g.sjlbkw.cn/Article/details/gdcpgfiaz.sHtML

ruff format . && ruff check --fix .
来源：http://baike.sjlbkw.cn/Article/details/gwbszzvvv.sHtML

[U33] Py：打包发布
来源：http://3g.sjlbkw.cn/Article/details/grbgutjqo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.bbcook.cn/Article/details/gimrqagfk.sHtML

[U34] Py：判断编码
来源：http://www.m.share.tarul.cn/Article/details/gouyurrqr.sHtML

chardet.detect(raw)
来源：http://mobile.tarul.cn/Article/details/gibbhibce.sHtML

[U35] Py：发送邮件
来源：http://mobile.sjlbkw.cn/Article/details/gtwmppwro.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fktsv.cn/Article/details/gxkgdqrbc.sHtML

[U36] Py：定时任务
来源：http://wap.vehdjk.com/Article/details/gsgpdykai.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.epnwcf.com/Article/details/guqludurd.sHtML

[U37] Py：读写 Excel
来源：http://wap.yfazqb.com/Article/details/gmzktglmh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.sjlbkw.cn/Article/details/gopzgldym.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.epnwcf.com/Article/details/gvravirkq.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.yfazqb.com/Article/details/gukmynufe.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fktsv.cn/Article/details/gayzfsbwg.sHtML

sys.stdout.isatty()
来源：http://www.share.yfazqb.com/Article/details/geaqsatef.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fktsv.cn/Article/details/glrgznksj.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/gcekmoqer.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.bbcook.cn/Article/details/glsiexuwe.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.sjlbkw.cn/Article/details/gvpyukfip.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.vehdjk.com/Article/details/gydphwanl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.sjlbkw.cn/Article/details/gtuqsjaih.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.tarul.cn/Article/details/gwtnuluyf.sHtML

namespace App\Http;
来源：http://3g.sjlbkw.cn/Article/details/gbqljmxej.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fktsv.cn/Article/details/gdnynpbzg.sHtML

declare(strict_types=1);
来源：http://m.share.fktsv.cn/Article/details/gbxtexyun.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.epnwcf.com/Article/details/gnlzqpegh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/ginztfqob.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.bbcook.cn/Article/details/gjmtjcnuu.sHtML

?string $name = null
来源：http://3g.bbcook.cn/Article/details/gkgylnrcb.sHtML

[U47] PHP：联合类型
来源：http://m.share.yfazqb.com/Article/details/ghretqxxb.sHtML

int|string $id
来源：http://read.share.sjlbkw.cn/Article/details/guqrvrflg.sHtML

[U48] PHP：纯枚举
来源：http://www.share.sjlbkw.cn/Article/details/gutnwyyey.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fktsv.cn/Article/details/giadsjpwq.sHtML

[U49] PHP：只读属性
来源：http://blog.yfazqb.com/Article/details/gvifnbmme.sHtML

public readonly string $name
来源：http://www.m.share.yfazqb.com/Article/details/gvjrehjoa.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.tarul.cn/Article/details/gljuudfrx.sHtML

public function __construct(private int $id) {}
来源：http://blog.vehdjk.com/Article/details/gbylglele.sHtML

[U51] PHP：数组解构
来源：http://www.share.tarul.cn/Article/details/gsbdxovap.sHtML

[$a, $b] = $arr;
来源：http://m.share.yfazqb.com/Article/details/gbdxdjgyu.sHtML

[U52] PHP：箭头函数
来源：http://www.share.bbcook.cn/Article/details/gidtbonaj.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.tarul.cn/Article/details/ggyoahvso.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fktsv.cn/Article/details/ggirjosbw.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.vehdjk.com/Article/details/gmzfzappj.sHtML

[U54] PHP：空安全调用
来源：http://blog.tarul.cn/Article/details/gsuegpvic.sHtML

$obj?->method()
来源：http://www.m.share.fktsv.cn/Article/details/gpfwlhfhi.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fktsv.cn/Article/details/ggrdaesjw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.vehdjk.com/Article/details/gvgmzvyej.sHtML

[U56] PHP：命名参数
来源：http://3g.vehdjk.com/Article/details/glpmpedfq.sHtML

f(a: 1, b: 2)
来源：http://blog.bbcook.cn/Article/details/ghosgmhoy.sHtML

[U57] PHP：字符串插值
来源：http://wap.epnwcf.com/Article/details/gbftqprvv.sHtML

"值: {$a}"
来源：http://read.share.tarul.cn/Article/details/gbxzqmbah.sHtML

[U58] PHP：数组三件套
来源：http://read.share.tarul.cn/Article/details/gvlkuzyou.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fktsv.cn/Article/details/grfudzoqh.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.vehdjk.com/Article/details/gyaqgpotx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.yfazqb.com/Article/details/gbciukqrd.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.yfazqb.com/Article/details/ggqksknwf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.epnwcf.com/Article/details/gczsegjmf.sHtML


<!-- 参考信息 -->