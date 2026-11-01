代发 wailian999

[S37] C++：set
来源：http://read.share.epnwcf.com/Article/details/gthldrafq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.bbcook.cn/Article/details/gpvvcdwtx.sHtML

[S38] C++：排序
来源：http://read.share.bbcook.cn/Article/details/gwtoepbkz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gzqiceenx.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fktsv.cn/Article/details/gqozsihcd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.sjlbkw.cn/Article/details/gkgeekgla.sHtML

[S40] C++：查找元素
来源：http://mobile.sjlbkw.cn/Article/details/goqasfopt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.vehdjk.com/Article/details/gpmvlzamz.sHtML

[S41] C++：类与构造函数
来源：http://baike.tarul.cn/Article/details/gblpslbxn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.sjlbkw.cn/Article/details/gyhznuqrl.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.sjlbkw.cn/Article/details/gaoxkgwle.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.epnwcf.com/Article/details/gzpydhjrz.sHtML

[S43] C++：智能指针
来源：http://read.share.tarul.cn/Article/details/gtqshnpdy.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.sjlbkw.cn/Article/details/gxyhcjogs.sHtML

[S44] C++：引用传参
来源：http://blog.vehdjk.com/Article/details/gzexuxfhr.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.vehdjk.com/Article/details/gdpjpywju.sHtML

[S45] C++：lambda
来源：http://3g.tarul.cn/Article/details/gzientqqi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.sjlbkw.cn/Article/details/grypjbckb.sHtML

[S46] C++：函数模板
来源：http://www.share.tarul.cn/Article/details/gklvrejhp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fktsv.cn/Article/details/gwivzkmur.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmedzveg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.tarul.cn/Article/details/ghhdbsxwf.sHtML

[S48] C++：逐行读文件
来源：http://mobile.epnwcf.com/Article/details/gkzseyrdg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fktsv.cn/Article/details/gsnbbhktz.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.bbcook.cn/Article/details/geksaishm.sHtML

[S49] C++：写文件
来源：http://www.share.yfazqb.com/Article/details/gxnlwagbd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.epnwcf.com/Article/details/gaxaylila.sHtML

[S50] C++：格式化数字
来源：http://wap.bbcook.cn/Article/details/gsnmtvwpp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gkaupnhar.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/gkwxshdzp.sHtML

static_cast<double>(a) / b
来源：http://blog.vehdjk.com/Article/details/gansmwjlz.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fktsv.cn/Article/details/gfriscszn.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.tarul.cn/Article/details/grhoukild.sHtML

[S53] C++：移动语义
来源：http://m.share.bbcook.cn/Article/details/ghaizlnau.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.vehdjk.com/Article/details/gbbpbyray.sHtML

[S54] C++：异常处理
来源：http://3g.sjlbkw.cn/Article/details/gowmfepjc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.yfazqb.com/Article/details/gopzzwnhc.sHtML

[S55] C++：结构化绑定
来源：http://blog.fktsv.cn/Article/details/ggnalpwwj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.tarul.cn/Article/details/gytzwzvwb.sHtML

[S56] C++：optional
来源：http://wap.yfazqb.com/Article/details/giddedlvr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.bbcook.cn/Article/details/gjefasmmu.sHtML

[S57] C++：编译期常量
来源：http://www.share.sjlbkw.cn/Article/details/gimqooxpx.sHtML

constexpr int N = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gstbwhfan.sHtML

[S58] C++：命名空间
来源：http://3g.tarul.cn/Article/details/gnghkjknv.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.sjlbkw.cn/Article/details/guepilyex.sHtML

[S59] C++：静态断言
来源：http://blog.bbcook.cn/Article/details/gnwpagajf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.vehdjk.com/Article/details/gldtzcnyw.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fktsv.cn/Article/details/gufcxvcry.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.sjlbkw.cn/Article/details/ghvnqsagn.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gkilmeoem.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.sjlbkw.cn/Article/details/gnpgbpepa.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gxuznkztu.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.epnwcf.com/Article/details/giwffhpss.sHtML

println("Hello")
来源：http://mobile.fktsv.cn/Article/details/gdccjsuek.sHtML

[T02] Kotlin：变量
来源：http://read.share.bbcook.cn/Article/details/gnrsmzpoa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.epnwcf.com/Article/details/gzavnqchp.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.epnwcf.com/Article/details/gssdgloah.sHtML

"值: $b"
来源：http://blog.vehdjk.com/Article/details/gpyfpknzg.sHtML

[T04] Kotlin：空安全
来源：http://www.share.epnwcf.com/Article/details/gyplmfbjh.sHtML

val n: String? = null;  n?.length
来源：http://read.share.vehdjk.com/Article/details/gncjuhqcw.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.sjlbkw.cn/Article/details/gjrvnksxa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.epnwcf.com/Article/details/gukwozkhr.sHtML

[T06] Kotlin：集合映射
来源：http://blog.epnwcf.com/Article/details/gldbtrcgf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.vehdjk.com/Article/details/gckjhnzcq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fktsv.cn/Article/details/gznirzvrk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.yfazqb.com/Article/details/guuvbgsky.sHtML

[T08] Kotlin：数据类
来源：http://m.share.tarul.cn/Article/details/gcatctmrl.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fktsv.cn/Article/details/gmieacfsk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.vehdjk.com/Article/details/gncogzqcz.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fktsv.cn/Article/details/gjqokavcr.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.bbcook.cn/Article/details/guklqetgc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.bbcook.cn/Article/details/ghebvtind.sHtML

[T11] Kotlin：协程
来源：http://blog.vehdjk.com/Article/details/gtaljbara.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.epnwcf.com/Article/details/gmppubanu.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.vehdjk.com/Article/details/gfumgkmqq.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gtuyynofv.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fktsv.cn/Article/details/grxsfnlfs.sHtML

val m = mapOf("a" to 1)
来源：http://baike.vehdjk.com/Article/details/gvxvhxvmz.sHtML

[T14] Kotlin：循环
来源：http://www.share.fktsv.cn/Article/details/goamwazif.sHtML

for (i in 1..10) println(i)
来源：http://m.share.tarul.cn/Article/details/gmnfvzsbh.sHtML

[T15] Kotlin：接口
来源：http://read.share.fktsv.cn/Article/details/gbtiuybiy.sHtML

interface Shape { fun area(): Double }
来源：http://blog.yfazqb.com/Article/details/gmiqasruq.sHtML

[T16] Swift：Hello World
来源：http://read.share.yfazqb.com/Article/details/ggalrejyp.sHtML

print("Hello")
来源：http://blog.tarul.cn/Article/details/gorqdcteh.sHtML

[T17] Swift：变量与常量
来源：http://mobile.tarul.cn/Article/details/gixmhkgdi.sHtML

var a = 1;  let b = 2
来源：http://www.share.tarul.cn/Article/details/gxunwatlv.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/gzzgmwrhx.sHtML

"值: \(b)"
来源：http://m.share.sjlbkw.cn/Article/details/ghmmiawrx.sHtML

[T19] Swift：可选绑定
来源：http://blog.vehdjk.com/Article/details/gjpjektdw.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.vehdjk.com/Article/details/gbxqddwsz.sHtML

[T20] Swift：数组操作
来源：http://www.share.bbcook.cn/Article/details/ghdkbmpav.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.yfazqb.com/Article/details/gsbsmjkev.sHtML

[T21] Swift：遍历
来源：http://mobile.sjlbkw.cn/Article/details/gznallnsr.sHtML

for x in a { print(x) }
来源：http://www.share.tarul.cn/Article/details/gkmebbzud.sHtML

[T22] Swift：字典
来源：http://www.m.share.epnwcf.com/Article/details/gluibnfmu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.yfazqb.com/Article/details/grrbqopse.sHtML

[T23] Swift：函数
来源：http://www.share.sjlbkw.cn/Article/details/gihwpcllq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.tarul.cn/Article/details/gixgmikgf.sHtML

[T24] Swift：闭包
来源：http://3g.tarul.cn/Article/details/gtlnnclpp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.yfazqb.com/Article/details/geuhkrctf.sHtML

[T25] Swift：结构体
来源：http://m.share.yfazqb.com/Article/details/gryttkzjk.sHtML

struct P { var x: Int }
来源：http://www.blog.vehdjk.com/Article/details/gbrhqcydj.sHtML

[T26] Swift：类与重写
来源：http://www.blog.epnwcf.com/Article/details/goezjrhvb.sHtML

class A: Base { override func f() {} }
来源：http://baike.sjlbkw.cn/Article/details/guahppghc.sHtML

[T27] Swift：错误处理
来源：http://blog.sjlbkw.cn/Article/details/gpvohiabb.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.bbcook.cn/Article/details/grcxweohz.sHtML

[T28] Swift：枚举
来源：http://wap.sjlbkw.cn/Article/details/gtlqlrrfq.sHtML

enum Color { case red, green }
来源：http://mobile.sjlbkw.cn/Article/details/glbolerhv.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.yfazqb.com/Article/details/gzfihypvf.sHtML

guard let x = opt else { return }
来源：http://wap.fktsv.cn/Article/details/gkacimrox.sHtML

[T30] Swift：协议
来源：http://m.share.vehdjk.com/Article/details/gbacibzum.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.tarul.cn/Article/details/gwyztpilo.sHtML

[T31] Lua：Hello World
来源：http://www.blog.bbcook.cn/Article/details/guxlwrafr.sHtML

print("Hello")
来源：http://mobile.yfazqb.com/Article/details/gttukxrth.sHtML

[T32] Lua：局部变量
来源：http://mobile.vehdjk.com/Article/details/gvenszbxo.sHtML

local a = 1
来源：http://mobile.epnwcf.com/Article/details/gzayfwgso.sHtML

[T33] Lua：表（数组）
来源：http://read.share.yfazqb.com/Article/details/gomkejpjn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.epnwcf.com/Article/details/gnfviaxbp.sHtML

[T34] Lua：遍历表
来源：http://www.blog.yfazqb.com/Article/details/gjctibbjt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.tarul.cn/Article/details/gqmpkkass.sHtML

[T35] Lua：字典表
来源：http://read.share.sjlbkw.cn/Article/details/gtshpwula.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.epnwcf.com/Article/details/gdpmzukpo.sHtML

[T36] Lua：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gkfjvkxik.sHtML

function add(a, b) return a + b end
来源：http://www.blog.sjlbkw.cn/Article/details/gehuiviyf.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.epnwcf.com/Article/details/gfmcvgaqu.sHtML

"a" .. "b"
来源：http://m.share.yfazqb.com/Article/details/gqdjfgylt.sHtML

[T38] Lua：条件
来源：http://www.share.yfazqb.com/Article/details/gfprxkoxy.sHtML

if x > 0 then print("正") end
来源：http://www.share.fktsv.cn/Article/details/gfeallhef.sHtML

[T39] Lua：模式匹配
来源：http://baike.epnwcf.com/Article/details/gfjkpzmrx.sHtML

string.find(s, "%d+")
来源：http://read.share.epnwcf.com/Article/details/gdhwppmbg.sHtML

[T40] Lua：元表
来源：http://3g.tarul.cn/Article/details/gvoqkkyfo.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.epnwcf.com/Article/details/gzsyuloij.sHtML

[T41] Perl：Hello World
来源：http://read.share.fktsv.cn/Article/details/gdmeongrd.sHtML

print "Hello\n";
来源：http://mobile.yfazqb.com/Article/details/gggfktfcs.sHtML

[T42] Perl：变量类型
来源：http://www.share.fktsv.cn/Article/details/gvdawixux.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.tarul.cn/Article/details/gtjwznxni.sHtML

[T43] Perl：字符串插值
来源：http://3g.fktsv.cn/Article/details/gmvlnbihu.sHtML

"值: $a"
来源：http://www.m.share.epnwcf.com/Article/details/gavznbsmb.sHtML

[T44] Perl：条件
来源：http://www.share.fktsv.cn/Article/details/gpayvtonx.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.bbcook.cn/Article/details/gkjxrwgxu.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fktsv.cn/Article/details/gluzwrogf.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.tarul.cn/Article/details/gjtlfidzl.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fktsv.cn/Article/details/gwwkaryha.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.sjlbkw.cn/Article/details/gwuwnxecm.sHtML

[T47] Perl：正则捕获
来源：http://blog.sjlbkw.cn/Article/details/gknztfgnz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.vehdjk.com/Article/details/gvidzimey.sHtML

[T48] Perl：正则替换
来源：http://www.share.yfazqb.com/Article/details/gxhdmxera.sHtML

$s =~ s/old/new/g;
来源：http://3g.bbcook.cn/Article/details/gdfxovfhz.sHtML

[T49] Perl：函数
来源：http://3g.sjlbkw.cn/Article/details/gttggaqju.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.tarul.cn/Article/details/gqelgioes.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gziuusopz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.sjlbkw.cn/Article/details/gsyuhqknd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.epnwcf.com/Article/details/gmmnwshsr.sHtML

[T51] Scala：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gfieugwxj.sHtML

println("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gysiykkzg.sHtML

[T52] Scala：变量
来源：http://www.m.share.vehdjk.com/Article/details/gllblbhgu.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.yfazqb.com/Article/details/gddcrfupk.sHtML

[T53] Scala：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gxtbtlshh.sHtML

s"值: $b"
来源：http://www.share.bbcook.cn/Article/details/gfejxpxzb.sHtML

[T54] Scala：集合映射
来源：http://m.share.epnwcf.com/Article/details/glxqmhoha.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fktsv.cn/Article/details/gbfestjvs.sHtML

[T55] Scala：集合过滤
来源：http://baike.tarul.cn/Article/details/grzhugoty.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fktsv.cn/Article/details/glrpyqgom.sHtML

[T56] Scala：样例类
来源：http://www.share.yfazqb.com/Article/details/gvbsukjfz.sHtML

case class User(name: String, age: Int)
来源：http://baike.bbcook.cn/Article/details/gravowjcs.sHtML

[T57] Scala：模式匹配
来源：http://wap.sjlbkw.cn/Article/details/ghfqfxieu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.yfazqb.com/Article/details/giliqwnds.sHtML

[T58] Scala：函数定义
来源：http://www.share.vehdjk.com/Article/details/gfsuimdfl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.epnwcf.com/Article/details/gtibdkjln.sHtML

[T59] Scala：循环
来源：http://3g.bbcook.cn/Article/details/gpnmmyrjv.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.tarul.cn/Article/details/glzxitozz.sHtML

[T60] Scala：折叠
来源：http://www.m.share.bbcook.cn/Article/details/gdkfpppui.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fktsv.cn/Article/details/grkcmtyql.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gitweskrf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.vehdjk.com/Article/details/gyofvavpn.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gltzipglh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.tarul.cn/Article/details/gzffytzzg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.tarul.cn/Article/details/gteswldny.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.yfazqb.com/Article/details/gkxyfmtgn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.sjlbkw.cn/Article/details/grjpnfriz.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.bbcook.cn/Article/details/gezxhxdzw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fktsv.cn/Article/details/gwmrpqyyw.sHtML

[U04] Py：变量调试打印
来源：http://3g.yfazqb.com/Article/details/gfgwmvtqr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.yfazqb.com/Article/details/grpozsrmc.sHtML

[U05] Py：列表去重且保序
来源：http://wap.bbcook.cn/Article/details/gdbzhjfge.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.yfazqb.com/Article/details/gopxigvqf.sHtML

[U06] Py：合并两个字典
来源：http://read.share.sjlbkw.cn/Article/details/gicbaqujy.sHtML

{**a, **b}
来源：http://baike.vehdjk.com/Article/details/gzfpjmhcu.sHtML

[U07] Py：反转字典键值
来源：http://baike.fktsv.cn/Article/details/gmmtwtssa.sHtML

{v: k for k, v in d.items()}
来源：http://blog.tarul.cn/Article/details/gvvdzbrje.sHtML

[U08] Py：展平二维列表
来源：http://m.share.tarul.cn/Article/details/gwqlxciqg.sHtML

[y for x in nested for y in x]
来源：http://blog.vehdjk.com/Article/details/gwrzzqbrm.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fktsv.cn/Article/details/gpvrujhow.sHtML

max(d, key=d.get)
来源：http://3g.yfazqb.com/Article/details/ggevjbcpk.sHtML

[U10] Py：按值排序字典
来源：http://baike.yfazqb.com/Article/details/ghyjxxjnw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.bbcook.cn/Article/details/gxsxtgijy.sHtML

[U11] Py：生成器表达式
来源：http://blog.sjlbkw.cn/Article/details/gppuawikh.sHtML

(x * 2 for x in arr)
来源：http://3g.fktsv.cn/Article/details/ggkjevjoy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fktsv.cn/Article/details/gpagyziue.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gogibwlct.sHtML

[U13] Py：固定长度队列
来源：http://blog.tarul.cn/Article/details/ggseoapum.sHtML

deque(maxlen=10)
来源：http://read.share.vehdjk.com/Article/details/gqkrkswkc.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.tarul.cn/Article/details/gkjlclgcy.sHtML

defaultdict(list)
来源：http://mobile.sjlbkw.cn/Article/details/gmtttcpaq.sHtML

[U15] Py：高精度计时
来源：http://mobile.bbcook.cn/Article/details/gbggperxt.sHtML

t = time.perf_counter()
来源：http://read.share.sjlbkw.cn/Article/details/gqmjrqxku.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.sjlbkw.cn/Article/details/grfmpqbkv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.bbcook.cn/Article/details/gcacjrunz.sHtML

[U17] Py：初始化日志
来源：http://mobile.sjlbkw.cn/Article/details/gfggmmycs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.tarul.cn/Article/details/ggboticgo.sHtML

[U18] Py：预编译正则
来源：http://read.share.bbcook.cn/Article/details/gmpswtejm.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.tarul.cn/Article/details/gehagxuiz.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.tarul.cn/Article/details/gstjdlkns.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fktsv.cn/Article/details/gzkuifmkm.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.tarul.cn/Article/details/gvodladlq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.epnwcf.com/Article/details/gecwiirct.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.yfazqb.com/Article/details/gqzlxsayy.sHtML

@contextlib.contextmanager
来源：http://www.m.share.tarul.cn/Article/details/gvnwtppnn.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.vehdjk.com/Article/details/gvfeiwgpe.sHtML

list(zip(*m))
来源：http://mobile.vehdjk.com/Article/details/gpndykzif.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.vehdjk.com/Article/details/gkgvggakg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.yfazqb.com/Article/details/gbogmitlz.sHtML

[U24] Py：路径操作
来源：http://wap.epnwcf.com/Article/details/golwxmalt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.epnwcf.com/Article/details/gsuylafzy.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.bbcook.cn/Article/details/gwaytdojv.sHtML

csv.DictReader(f)
来源：http://read.share.epnwcf.com/Article/details/ggfzcxylq.sHtML

[U26] Py：并发下载
来源：http://3g.fktsv.cn/Article/details/gbgosmoxg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fktsv.cn/Article/details/gnsbfhrcg.sHtML

[U27] Py：异步 HTTP
来源：http://baike.sjlbkw.cn/Article/details/gnthbtrxg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.yfazqb.com/Article/details/gxscrsblo.sHtML

[U28] Py：类型别名
来源：http://www.share.bbcook.cn/Article/details/geundahuj.sHtML

UserId = int
来源：http://www.blog.fktsv.cn/Article/details/gmzngtwfd.sHtML

[U29] Py：属性校验
来源：http://3g.yfazqb.com/Article/details/gbhqdclsq.sHtML

@property 与 @x.setter 配合
来源：http://3g.bbcook.cn/Article/details/gcyjxnbwf.sHtML

[U30] Py：数据类
来源：http://m.share.fktsv.cn/Article/details/gmfmfovxc.sHtML

@dataclass(slots=True)
来源：http://m.share.yfazqb.com/Article/details/gbywolrpx.sHtML

[U31] Py：单测
来源：http://www.blog.sjlbkw.cn/Article/details/gxxhsabpx.sHtML

python -m pytest -q
来源：http://www.m.share.tarul.cn/Article/details/gtngfnheq.sHtML

[U32] Py：代码格式化
来源：http://blog.epnwcf.com/Article/details/gmnpjjuxt.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhdlckqe.sHtML

[U33] Py：打包发布
来源：http://blog.sjlbkw.cn/Article/details/gfpeokzcf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.epnwcf.com/Article/details/gjuuokwxp.sHtML

[U34] Py：判断编码
来源：http://baike.yfazqb.com/Article/details/geyzzipom.sHtML

chardet.detect(raw)
来源：http://www.m.share.fktsv.cn/Article/details/gpemriyko.sHtML

[U35] Py：发送邮件
来源：http://m.share.fktsv.cn/Article/details/gsqifhbll.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.bbcook.cn/Article/details/gbzeceaxg.sHtML

[U36] Py：定时任务
来源：http://read.share.sjlbkw.cn/Article/details/gppujwdpl.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.yfazqb.com/Article/details/guddvhwnk.sHtML

[U37] Py：读写 Excel
来源：http://m.share.yfazqb.com/Article/details/gjqbavctu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.yfazqb.com/Article/details/gvtixsbgg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.tarul.cn/Article/details/gpnwgihun.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.tarul.cn/Article/details/gmtrqnnjc.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.tarul.cn/Article/details/gddiqtcbr.sHtML

sys.stdout.isatty()
来源：http://baike.sjlbkw.cn/Article/details/gqnymehlx.sHtML

[U40] Py：打印到标准错误
来源：http://wap.epnwcf.com/Article/details/gxptgaqnd.sHtML

print("err", file=sys.stderr)
来源：http://baike.vehdjk.com/Article/details/gcebdnoum.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.yfazqb.com/Article/details/gfnjlsbhe.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fktsv.cn/Article/details/gazasnvtm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.epnwcf.com/Article/details/gjflboekl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.vehdjk.com/Article/details/gvfsgxhjx.sHtML

[U43] PHP：声明命名空间
来源：http://blog.vehdjk.com/Article/details/gtfwckoja.sHtML

namespace App\Http;
来源：http://mobile.vehdjk.com/Article/details/gqpeowyuy.sHtML

[U44] PHP：开启严格类型
来源：http://3g.vehdjk.com/Article/details/gzqdzycjo.sHtML

declare(strict_types=1);
来源：http://3g.vehdjk.com/Article/details/goafkmbgl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fktsv.cn/Article/details/glreubknj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gcngrhslj.sHtML

[U46] PHP：可空类型
来源：http://mobile.epnwcf.com/Article/details/gtqkfeham.sHtML

?string $name = null
来源：http://m.share.bbcook.cn/Article/details/ghvxxnfen.sHtML

[U47] PHP：联合类型
来源：http://www.share.vehdjk.com/Article/details/gnehheiot.sHtML

int|string $id
来源：http://read.share.epnwcf.com/Article/details/gnhhwovzz.sHtML

[U48] PHP：纯枚举
来源：http://mobile.sjlbkw.cn/Article/details/ghfktaozq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fktsv.cn/Article/details/gamoytsiz.sHtML

[U49] PHP：只读属性
来源：http://baike.yfazqb.com/Article/details/goinmgwzl.sHtML

public readonly string $name
来源：http://blog.epnwcf.com/Article/details/gamlurvto.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.epnwcf.com/Article/details/gqvwxxogh.sHtML

public function __construct(private int $id) {}
来源：http://wap.tarul.cn/Article/details/gdrpdsazw.sHtML

[U51] PHP：数组解构
来源：http://3g.tarul.cn/Article/details/gzzasoosq.sHtML

[$a, $b] = $arr;
来源：http://www.share.bbcook.cn/Article/details/gpqzhccdg.sHtML

[U52] PHP：箭头函数
来源：http://baike.fktsv.cn/Article/details/gzzkpwuuo.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.tarul.cn/Article/details/ghuttsvia.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.tarul.cn/Article/details/gfjzzznoi.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.yfazqb.com/Article/details/gygxzufnj.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.bbcook.cn/Article/details/grtgwgsvg.sHtML

$obj?->method()
来源：http://m.share.fktsv.cn/Article/details/gvrfqspbx.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fktsv.cn/Article/details/ghgbzjaac.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.yfazqb.com/Article/details/gxowpojas.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.tarul.cn/Article/details/gbdlnqbhu.sHtML

f(a: 1, b: 2)
来源：http://m.share.fktsv.cn/Article/details/gdwcplyes.sHtML

[U57] PHP：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gcrakluoy.sHtML

"值: {$a}"
来源：http://read.share.epnwcf.com/Article/details/gdpfcdpks.sHtML

[U58] PHP：数组三件套
来源：http://wap.yfazqb.com/Article/details/gykuyqbpr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.epnwcf.com/Article/details/gotbymvir.sHtML

[U59] PHP：自定义排序
来源：http://wap.fktsv.cn/Article/details/gryhnlkna.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.sjlbkw.cn/Article/details/ghfhaqviv.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.epnwcf.com/Article/details/gbufydkrw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.bbcook.cn/Article/details/gqofznqtk.sHtML

[U61] PHP：正则
来源：http://blog.epnwcf.com/Article/details/gfqwqlvnh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.epnwcf.com/Article/details/gthjnqvxv.sHtML

[U62] PHP：日期对象
来源：http://blog.tarul.cn/Article/details/gxihmwtkz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.yfazqb.com/Article/details/gfrkuaayr.sHtML


<!-- 参考信息 -->