代发 wailian999

[S33] C++：vector 增删
来源：http://www.m.share.bbcook.cn/Article/details/gwwqhpgpu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.yfazqb.com/Article/details/gvdlfvlwf.sHtML

[S34] C++：遍历 vector
来源：http://baike.epnwcf.com/Article/details/gxepxqmho.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.tarul.cn/Article/details/ghhtlrzyq.sHtML

[S35] C++：map
来源：http://wap.bbcook.cn/Article/details/gvxgplbbk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.tarul.cn/Article/details/gebuosvsv.sHtML

[S36] C++：unordered_map
来源：http://blog.vehdjk.com/Article/details/gvzybsiep.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gasmsxdyw.sHtML

[S37] C++：set
来源：http://mobile.bbcook.cn/Article/details/glpwjtyaj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fktsv.cn/Article/details/gnoqozvye.sHtML

[S38] C++：排序
来源：http://3g.bbcook.cn/Article/details/gqblanait.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.yfazqb.com/Article/details/gpjutlqqj.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.vehdjk.com/Article/details/ghttqaigt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.sjlbkw.cn/Article/details/galdberox.sHtML

[S40] C++：查找元素
来源：http://m.share.tarul.cn/Article/details/ghfopjlko.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.vehdjk.com/Article/details/gdfexmwcc.sHtML

[S41] C++：类与构造函数
来源：http://3g.bbcook.cn/Article/details/ginxwxmlv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.tarul.cn/Article/details/gowoncsdd.sHtML

[S42] C++：继承与虚函数
来源：http://baike.bbcook.cn/Article/details/ggikccpwk.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.tarul.cn/Article/details/gouetvzsq.sHtML

[S43] C++：智能指针
来源：http://www.share.sjlbkw.cn/Article/details/gsksiawyo.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.yfazqb.com/Article/details/gmigqirjl.sHtML

[S44] C++：引用传参
来源：http://3g.vehdjk.com/Article/details/gtidkormp.sHtML

void inc(int &x) { ++x; }
来源：http://3g.yfazqb.com/Article/details/gpaskxlzd.sHtML

[S45] C++：lambda
来源：http://read.share.sjlbkw.cn/Article/details/ghzgcagvl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.epnwcf.com/Article/details/gtfhpalxs.sHtML

[S46] C++：函数模板
来源：http://www.m.share.vehdjk.com/Article/details/gqjsbhfdq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fktsv.cn/Article/details/ghnrogwrs.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fktsv.cn/Article/details/gavnpqcrc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.epnwcf.com/Article/details/gnoboiflc.sHtML

[S48] C++：逐行读文件
来源：http://baike.fktsv.cn/Article/details/gmrqekuqi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.sjlbkw.cn/Article/details/gktzestue.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.bbcook.cn/Article/details/grsttcpiw.sHtML

[S49] C++：写文件
来源：http://wap.epnwcf.com/Article/details/guaqqpyqj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.epnwcf.com/Article/details/gfhmqlgjh.sHtML

[S50] C++：格式化数字
来源：http://blog.fktsv.cn/Article/details/gbtgxjhjb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gkzanaxud.sHtML

[S51] C++：显式类型转换
来源：http://read.share.sjlbkw.cn/Article/details/gdmuqybjb.sHtML

static_cast<double>(a) / b
来源：http://m.share.fktsv.cn/Article/details/glmaifezw.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.yfazqb.com/Article/details/gtrmcdinj.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.yfazqb.com/Article/details/gaaxkxktu.sHtML

[S53] C++：移动语义
来源：http://www.blog.yfazqb.com/Article/details/gxudkyuyd.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.vehdjk.com/Article/details/gxrlxxxha.sHtML

[S54] C++：异常处理
来源：http://baike.epnwcf.com/Article/details/gtzqrvjdh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.vehdjk.com/Article/details/ghlixsvfq.sHtML

[S55] C++：结构化绑定
来源：http://read.share.sjlbkw.cn/Article/details/gwprxbvkv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.sjlbkw.cn/Article/details/ggxxdyuka.sHtML

[S56] C++：optional
来源：http://blog.vehdjk.com/Article/details/gsmbuvqkh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.yfazqb.com/Article/details/gfoikhbjn.sHtML

[S57] C++：编译期常量
来源：http://wap.vehdjk.com/Article/details/gimbumwcf.sHtML

constexpr int N = 10;
来源：http://read.share.vehdjk.com/Article/details/guuycbfka.sHtML

[S58] C++：命名空间
来源：http://mobile.vehdjk.com/Article/details/grxpwxias.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.vehdjk.com/Article/details/gdlssmfwe.sHtML

[S59] C++：静态断言
来源：http://baike.bbcook.cn/Article/details/gkierrzfc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.tarul.cn/Article/details/gvxmdvgtb.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.epnwcf.com/Article/details/glmajakoa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.epnwcf.com/Article/details/gdwzfzcsz.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gjjsjxsnm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.bbcook.cn/Article/details/gbzhtiuag.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gxzbqiitx.sHtML

[T01] Kotlin：Hello World
来源：http://3g.vehdjk.com/Article/details/gbzqxgoub.sHtML

println("Hello")
来源：http://mobile.vehdjk.com/Article/details/gxkholnal.sHtML

[T02] Kotlin：变量
来源：http://www.share.tarul.cn/Article/details/gydwfngbz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.epnwcf.com/Article/details/gtzniysvj.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.vehdjk.com/Article/details/gqwuexoap.sHtML

"值: $b"
来源：http://www.m.share.vehdjk.com/Article/details/gtiaadlud.sHtML

[T04] Kotlin：空安全
来源：http://wap.tarul.cn/Article/details/gtvwpipxl.sHtML

val n: String? = null;  n?.length
来源：http://blog.bbcook.cn/Article/details/gkerjjujk.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.vehdjk.com/Article/details/gmllkzdjx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.tarul.cn/Article/details/gmsqwnnpv.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.epnwcf.com/Article/details/gdcygnunb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.sjlbkw.cn/Article/details/giqnxdgcm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.epnwcf.com/Article/details/glkmxmadj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.tarul.cn/Article/details/gyfgufwvp.sHtML

[T08] Kotlin：数据类
来源：http://mobile.bbcook.cn/Article/details/grbdvjwep.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.vehdjk.com/Article/details/gscctssqs.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.bbcook.cn/Article/details/gdlxrledz.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.tarul.cn/Article/details/gjcmbngtq.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.epnwcf.com/Article/details/gtgdvqiug.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.vehdjk.com/Article/details/giyujyzre.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.sjlbkw.cn/Article/details/gytslvtvc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fktsv.cn/Article/details/gpftjsimm.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.yfazqb.com/Article/details/gnhjgytii.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gkgiuihcs.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.tarul.cn/Article/details/guorhjylb.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.yfazqb.com/Article/details/gygnkmncv.sHtML

[T14] Kotlin：循环
来源：http://read.share.bbcook.cn/Article/details/gdhmuvycd.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/gyshnuvme.sHtML

[T15] Kotlin：接口
来源：http://m.share.yfazqb.com/Article/details/gfrkyvzgd.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fktsv.cn/Article/details/gnzibkpuj.sHtML

[T16] Swift：Hello World
来源：http://baike.bbcook.cn/Article/details/gkbjxwtls.sHtML

print("Hello")
来源：http://read.share.tarul.cn/Article/details/gzcycbrum.sHtML

[T17] Swift：变量与常量
来源：http://baike.bbcook.cn/Article/details/gdiwcykrg.sHtML

var a = 1;  let b = 2
来源：http://baike.fktsv.cn/Article/details/gbidfkbxy.sHtML

[T18] Swift：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gqszqwqix.sHtML

"值: \(b)"
来源：http://www.share.sjlbkw.cn/Article/details/grcvncbpy.sHtML

[T19] Swift：可选绑定
来源：http://3g.fktsv.cn/Article/details/gfcbmsaee.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdszilew.sHtML

[T20] Swift：数组操作
来源：http://3g.bbcook.cn/Article/details/glzxlvtak.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.epnwcf.com/Article/details/gztklabev.sHtML

[T21] Swift：遍历
来源：http://3g.bbcook.cn/Article/details/gcmzeacis.sHtML

for x in a { print(x) }
来源：http://www.blog.fktsv.cn/Article/details/gthrzqdfm.sHtML

[T22] Swift：字典
来源：http://mobile.fktsv.cn/Article/details/gjniinopl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.tarul.cn/Article/details/gchsksijp.sHtML

[T23] Swift：函数
来源：http://mobile.yfazqb.com/Article/details/gknnanedt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gpdenjywy.sHtML

[T24] Swift：闭包
来源：http://3g.bbcook.cn/Article/details/gkkliniub.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.epnwcf.com/Article/details/gofihjesw.sHtML

[T25] Swift：结构体
来源：http://3g.epnwcf.com/Article/details/gofqumsjo.sHtML

struct P { var x: Int }
来源：http://m.share.epnwcf.com/Article/details/gazmznyei.sHtML

[T26] Swift：类与重写
来源：http://3g.epnwcf.com/Article/details/gjthblrnu.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fktsv.cn/Article/details/gjewzfcwz.sHtML

[T27] Swift：错误处理
来源：http://m.share.tarul.cn/Article/details/gpjtelnjg.sHtML

do { try f() } catch { print(error) }
来源：http://wap.tarul.cn/Article/details/gpkkymohv.sHtML

[T28] Swift：枚举
来源：http://www.m.share.tarul.cn/Article/details/gnteykqqg.sHtML

enum Color { case red, green }
来源：http://baike.epnwcf.com/Article/details/glhuifalb.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.yfazqb.com/Article/details/gfxvyenvq.sHtML

guard let x = opt else { return }
来源：http://baike.yfazqb.com/Article/details/gpwlijqry.sHtML

[T30] Swift：协议
来源：http://www.blog.bbcook.cn/Article/details/gkbdnbusm.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.bbcook.cn/Article/details/gvhaioett.sHtML

[T31] Lua：Hello World
来源：http://www.share.vehdjk.com/Article/details/gwrgdmszu.sHtML

print("Hello")
来源：http://www.blog.vehdjk.com/Article/details/gjxonenhy.sHtML

[T32] Lua：局部变量
来源：http://read.share.fktsv.cn/Article/details/ggewmrbyo.sHtML

local a = 1
来源：http://www.blog.vehdjk.com/Article/details/gzzzztkdm.sHtML

[T33] Lua：表（数组）
来源：http://baike.yfazqb.com/Article/details/gbzomwkae.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.yfazqb.com/Article/details/gdyqzlxeg.sHtML

[T34] Lua：遍历表
来源：http://www.blog.sjlbkw.cn/Article/details/gqqqefwdn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.epnwcf.com/Article/details/giqllpimr.sHtML

[T35] Lua：字典表
来源：http://read.share.yfazqb.com/Article/details/grzdhbdoy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.epnwcf.com/Article/details/guzqabkey.sHtML

[T36] Lua：函数
来源：http://www.share.fktsv.cn/Article/details/gbalsiuvp.sHtML

function add(a, b) return a + b end
来源：http://www.blog.vehdjk.com/Article/details/gkcaonpvp.sHtML

[T37] Lua：字符串拼接
来源：http://baike.tarul.cn/Article/details/gpgogzvgi.sHtML

"a" .. "b"
来源：http://www.m.share.vehdjk.com/Article/details/gnqreyeuz.sHtML

[T38] Lua：条件
来源：http://read.share.epnwcf.com/Article/details/gmgzersfw.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.bbcook.cn/Article/details/gckpcyrsh.sHtML

[T39] Lua：模式匹配
来源：http://m.share.yfazqb.com/Article/details/gmudtgnoo.sHtML

string.find(s, "%d+")
来源：http://m.share.epnwcf.com/Article/details/gpsbdqzva.sHtML

[T40] Lua：元表
来源：http://wap.yfazqb.com/Article/details/gachxvxjl.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.sjlbkw.cn/Article/details/gocrlnegu.sHtML

[T41] Perl：Hello World
来源：http://read.share.tarul.cn/Article/details/gbgszgbos.sHtML

print "Hello\n";
来源：http://www.share.vehdjk.com/Article/details/gkdpnzlsc.sHtML

[T42] Perl：变量类型
来源：http://read.share.tarul.cn/Article/details/gywarmqod.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.yfazqb.com/Article/details/gicpjktqo.sHtML

[T43] Perl：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gvvlbefcs.sHtML

"值: $a"
来源：http://3g.epnwcf.com/Article/details/gdfawccwj.sHtML

[T44] Perl：条件
来源：http://wap.vehdjk.com/Article/details/gtermxyet.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.bbcook.cn/Article/details/gniflzwzi.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.yfazqb.com/Article/details/gubofedje.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.sjlbkw.cn/Article/details/gjrxzxhmm.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fktsv.cn/Article/details/gecgqtojn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.tarul.cn/Article/details/gnosugfwx.sHtML

[T47] Perl：正则捕获
来源：http://wap.epnwcf.com/Article/details/gddwgritu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.bbcook.cn/Article/details/gylpwyumh.sHtML

[T48] Perl：正则替换
来源：http://wap.fktsv.cn/Article/details/gppchgwme.sHtML

$s =~ s/old/new/g;
来源：http://m.share.bbcook.cn/Article/details/giwngwpgo.sHtML

[T49] Perl：函数
来源：http://m.share.tarul.cn/Article/details/gmzhyqyow.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/grhqgqpey.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gnfwfcsqq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.bbcook.cn/Article/details/gibmrflrg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fktsv.cn/Article/details/gjoccqgvz.sHtML

[T51] Scala：Hello World
来源：http://read.share.bbcook.cn/Article/details/gneupnygt.sHtML

println("Hello")
来源：http://mobile.bbcook.cn/Article/details/gsylqbyxn.sHtML

[T52] Scala：变量
来源：http://baike.sjlbkw.cn/Article/details/gtcwhwhif.sHtML

val a = 1;  var b = 2
来源：http://www.share.bbcook.cn/Article/details/guexbuisk.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gbuwjtvqx.sHtML

s"值: $b"
来源：http://m.share.epnwcf.com/Article/details/gliwgonpo.sHtML

[T54] Scala：集合映射
来源：http://mobile.vehdjk.com/Article/details/ggrjctrdg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.bbcook.cn/Article/details/guqsmpseq.sHtML

[T55] Scala：集合过滤
来源：http://read.share.sjlbkw.cn/Article/details/gckwzagmy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.tarul.cn/Article/details/gimznyddr.sHtML

[T56] Scala：样例类
来源：http://www.share.vehdjk.com/Article/details/giarswxui.sHtML

case class User(name: String, age: Int)
来源：http://read.share.epnwcf.com/Article/details/gtmahxrlo.sHtML

[T57] Scala：模式匹配
来源：http://mobile.yfazqb.com/Article/details/gezyojhyh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.bbcook.cn/Article/details/gwqjsbldb.sHtML

[T58] Scala：函数定义
来源：http://read.share.epnwcf.com/Article/details/gqpmtqpnn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.vehdjk.com/Article/details/gkxddnrgx.sHtML

[T59] Scala：循环
来源：http://www.m.share.epnwcf.com/Article/details/gyqspceys.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.bbcook.cn/Article/details/gthergqyt.sHtML

[T60] Scala：折叠
来源：http://m.share.yfazqb.com/Article/details/gtnrtnbdj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fktsv.cn/Article/details/goyqyrvkr.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/glcwmlgud.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.tarul.cn/Article/details/glaatvano.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/grsgtbjzw.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.vehdjk.com/Article/details/glakxgaev.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.vehdjk.com/Article/details/ggifhwdov.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.epnwcf.com/Article/details/gxcmngcxa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.tarul.cn/Article/details/gjgszcxxt.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.bbcook.cn/Article/details/gtiknnvqk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.bbcook.cn/Article/details/gxhyabxno.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.bbcook.cn/Article/details/gellkpsjh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fktsv.cn/Article/details/gjhuhkxir.sHtML

[U05] Py：列表去重且保序
来源：http://baike.epnwcf.com/Article/details/gywsmpzkp.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.yfazqb.com/Article/details/gvpmmdrqm.sHtML

[U06] Py：合并两个字典
来源：http://read.share.epnwcf.com/Article/details/ggamummwn.sHtML

{**a, **b}
来源：http://mobile.epnwcf.com/Article/details/ghmizhrqe.sHtML

[U07] Py：反转字典键值
来源：http://wap.fktsv.cn/Article/details/gqcjevokk.sHtML

{v: k for k, v in d.items()}
来源：http://wap.sjlbkw.cn/Article/details/gmxdehrvt.sHtML

[U08] Py：展平二维列表
来源：http://blog.fktsv.cn/Article/details/gtbbtpywb.sHtML

[y for x in nested for y in x]
来源：http://3g.vehdjk.com/Article/details/gsgkvnyyv.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.bbcook.cn/Article/details/gtkithlth.sHtML

max(d, key=d.get)
来源：http://www.blog.vehdjk.com/Article/details/guzozbhfn.sHtML

[U10] Py：按值排序字典
来源：http://www.share.vehdjk.com/Article/details/gvzjqpblt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.bbcook.cn/Article/details/gyrojxfdw.sHtML

[U11] Py：生成器表达式
来源：http://blog.tarul.cn/Article/details/gzuvnjtlh.sHtML

(x * 2 for x in arr)
来源：http://blog.epnwcf.com/Article/details/gousbfhoy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.epnwcf.com/Article/details/glaqwfqyh.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.vehdjk.com/Article/details/gjxycarnj.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.sjlbkw.cn/Article/details/gpxbyfmbl.sHtML

deque(maxlen=10)
来源：http://wap.yfazqb.com/Article/details/goevraqor.sHtML

[U14] Py：分组收集到列表
来源：http://baike.tarul.cn/Article/details/gqgoqdnxf.sHtML

defaultdict(list)
来源：http://blog.vehdjk.com/Article/details/gjzxzmiiy.sHtML

[U15] Py：高精度计时
来源：http://read.share.yfazqb.com/Article/details/gmvigkdyf.sHtML

t = time.perf_counter()
来源：http://3g.bbcook.cn/Article/details/gwpqifxtm.sHtML

[U16] Py：命令行参数解析
来源：http://wap.yfazqb.com/Article/details/gnrbzbimu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.vehdjk.com/Article/details/gxcrpmbdh.sHtML

[U17] Py：初始化日志
来源：http://read.share.sjlbkw.cn/Article/details/gsvocnobj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.vehdjk.com/Article/details/gzqobgynv.sHtML

[U18] Py：预编译正则
来源：http://baike.yfazqb.com/Article/details/gwmlatwzo.sHtML

pat = re.compile(r"\d+")
来源：http://blog.yfazqb.com/Article/details/gmfmmczgq.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fktsv.cn/Article/details/gojymgeyl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.vehdjk.com/Article/details/gzuofooww.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.sjlbkw.cn/Article/details/gftfowvsl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.tarul.cn/Article/details/gemurssbc.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.yfazqb.com/Article/details/gaqcxpouv.sHtML

@contextlib.contextmanager
来源：http://mobile.sjlbkw.cn/Article/details/gobprcwog.sHtML

[U22] Py：矩阵转置
来源：http://wap.sjlbkw.cn/Article/details/gbkyrkqiy.sHtML

list(zip(*m))
来源：http://mobile.epnwcf.com/Article/details/gepttnmfa.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.tarul.cn/Article/details/gucykvmkx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fktsv.cn/Article/details/gtfubalnf.sHtML

[U24] Py：路径操作
来源：http://baike.bbcook.cn/Article/details/gfgqopwsl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/giocvthfn.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.tarul.cn/Article/details/gdxsftjdg.sHtML

csv.DictReader(f)
来源：http://www.m.share.epnwcf.com/Article/details/gshtnysyv.sHtML

[U26] Py：并发下载
来源：http://www.share.vehdjk.com/Article/details/gwssukbgx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.sjlbkw.cn/Article/details/gglqiofyr.sHtML

[U27] Py：异步 HTTP
来源：http://wap.sjlbkw.cn/Article/details/gslzsgnxf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.epnwcf.com/Article/details/glphjafyj.sHtML

[U28] Py：类型别名
来源：http://www.blog.bbcook.cn/Article/details/gpvcqaoqz.sHtML

UserId = int
来源：http://read.share.fktsv.cn/Article/details/gqthcdapz.sHtML

[U29] Py：属性校验
来源：http://www.share.epnwcf.com/Article/details/gnpmjomek.sHtML

@property 与 @x.setter 配合
来源：http://baike.fktsv.cn/Article/details/giycynhhd.sHtML

[U30] Py：数据类
来源：http://www.m.share.tarul.cn/Article/details/gklwumnqw.sHtML

@dataclass(slots=True)
来源：http://wap.yfazqb.com/Article/details/goimkbjjs.sHtML

[U31] Py：单测
来源：http://baike.epnwcf.com/Article/details/gbtknedam.sHtML

python -m pytest -q
来源：http://blog.sjlbkw.cn/Article/details/gkxxdjhqc.sHtML

[U32] Py：代码格式化
来源：http://www.blog.bbcook.cn/Article/details/gkmmhvslo.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.bbcook.cn/Article/details/gmesruvqk.sHtML

[U33] Py：打包发布
来源：http://www.m.share.tarul.cn/Article/details/gzgnuaoob.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.vehdjk.com/Article/details/gpzzjiwvw.sHtML

[U34] Py：判断编码
来源：http://wap.tarul.cn/Article/details/gulmotrkl.sHtML

chardet.detect(raw)
来源：http://read.share.yfazqb.com/Article/details/glwqtuthq.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.epnwcf.com/Article/details/gdzzjseef.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fktsv.cn/Article/details/gygamkevr.sHtML

[U36] Py：定时任务
来源：http://wap.vehdjk.com/Article/details/gesznedrw.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.epnwcf.com/Article/details/ggzoijkjb.sHtML

[U37] Py：读写 Excel
来源：http://baike.vehdjk.com/Article/details/gsqaozwao.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.vehdjk.com/Article/details/gbhhdwwas.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.sjlbkw.cn/Article/details/gohhdlcgq.sHtML

Path(__file__).resolve().parent
来源：http://www.share.epnwcf.com/Article/details/gubvqqpxs.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.bbcook.cn/Article/details/gunxpefwu.sHtML

sys.stdout.isatty()
来源：http://wap.fktsv.cn/Article/details/grpmhskbo.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.vehdjk.com/Article/details/gnonltcpo.sHtML

print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/gdyacudpk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.tarul.cn/Article/details/gydtdzjra.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.tarul.cn/Article/details/gjtpkihes.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.sjlbkw.cn/Article/details/gaenuuynk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.bbcook.cn/Article/details/gxquzgiob.sHtML

[U43] PHP：声明命名空间
来源：http://blog.epnwcf.com/Article/details/ghldaljzx.sHtML

namespace App\Http;
来源：http://blog.epnwcf.com/Article/details/gebnawdnk.sHtML

[U44] PHP：开启严格类型
来源：http://baike.yfazqb.com/Article/details/gceiqplmz.sHtML

declare(strict_types=1);
来源：http://www.blog.vehdjk.com/Article/details/gfsezpdxo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.vehdjk.com/Article/details/gywqtublq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gvyeymxex.sHtML

[U46] PHP：可空类型
来源：http://baike.vehdjk.com/Article/details/gykildkur.sHtML

?string $name = null
来源：http://3g.sjlbkw.cn/Article/details/gcatmzcxr.sHtML

[U47] PHP：联合类型
来源：http://3g.epnwcf.com/Article/details/gtanjxxkd.sHtML

int|string $id
来源：http://blog.yfazqb.com/Article/details/gdyflpgay.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.vehdjk.com/Article/details/gmsbitjsn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.tarul.cn/Article/details/gxqdqeyzm.sHtML

[U49] PHP：只读属性
来源：http://wap.tarul.cn/Article/details/gjsflhxwo.sHtML

public readonly string $name
来源：http://blog.vehdjk.com/Article/details/grftubxip.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fktsv.cn/Article/details/gkevfakwi.sHtML

public function __construct(private int $id) {}
来源：http://read.share.yfazqb.com/Article/details/gpwkwkocz.sHtML

[U51] PHP：数组解构
来源：http://3g.vehdjk.com/Article/details/gpnybnfve.sHtML

[$a, $b] = $arr;
来源：http://3g.bbcook.cn/Article/details/gshwompdv.sHtML

[U52] PHP：箭头函数
来源：http://baike.epnwcf.com/Article/details/gmdgmjqrc.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fktsv.cn/Article/details/gaznfobmy.sHtML

[U53] PHP：空合并运算符
来源：http://wap.tarul.cn/Article/details/gdkofolyw.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fktsv.cn/Article/details/grorkvysx.sHtML

[U54] PHP：空安全调用
来源：http://blog.tarul.cn/Article/details/gifwdwmxt.sHtML

$obj?->method()
来源：http://3g.epnwcf.com/Article/details/gyqvmqiur.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gfmxclifr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.bbcook.cn/Article/details/gbytqjpra.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fktsv.cn/Article/details/ghovbhpmm.sHtML

f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/ggnzozuxx.sHtML

[U57] PHP：字符串插值
来源：http://baike.yfazqb.com/Article/details/gvnayttwn.sHtML

"值: {$a}"
来源：http://read.share.vehdjk.com/Article/details/gizqorlog.sHtML

[U58] PHP：数组三件套
来源：http://mobile.vehdjk.com/Article/details/gkigtwygf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.bbcook.cn/Article/details/gvgsidflp.sHtML


<!-- 参考信息 -->