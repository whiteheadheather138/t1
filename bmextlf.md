代发 wailian999

[S39] C++：自定义比较器排序
来源：http://m.share.epnwcf.com/Article/details/gtcbmcrvz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.bbcook.cn/Article/details/gxahhaeki.sHtML

[S40] C++：查找元素
来源：http://www.share.bbcook.cn/Article/details/gjpwnliif.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.yfazqb.com/Article/details/gwoxzluiv.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.epnwcf.com/Article/details/guuhkyhiy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.yfazqb.com/Article/details/gvlohbwxy.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fktsv.cn/Article/details/gfvtpsccr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.sjlbkw.cn/Article/details/gvbrnsbcb.sHtML

[S43] C++：智能指针
来源：http://3g.tarul.cn/Article/details/gixkwmqkz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/gounftukf.sHtML

[S44] C++：引用传参
来源：http://blog.bbcook.cn/Article/details/gizljnqft.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.epnwcf.com/Article/details/guipmcdpi.sHtML

[S45] C++：lambda
来源：http://read.share.fktsv.cn/Article/details/guuvpwgav.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.vehdjk.com/Article/details/ghfgvoqol.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/gfcbatwxv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.bbcook.cn/Article/details/ghfcdolkk.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.epnwcf.com/Article/details/glejgpuqh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.yfazqb.com/Article/details/gzeloqxzc.sHtML

[S48] C++：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gyxglrkfj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fktsv.cn/Article/details/gbcmhdbat.sHtML

while (std::getline(in, line)) { }
来源：http://wap.sjlbkw.cn/Article/details/gmujirbbi.sHtML

[S49] C++：写文件
来源：http://wap.tarul.cn/Article/details/glbjphljb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.epnwcf.com/Article/details/gzbdhafkv.sHtML

[S50] C++：格式化数字
来源：http://wap.bbcook.cn/Article/details/gigenrxcu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.vehdjk.com/Article/details/gkevqqfsp.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.tarul.cn/Article/details/ggkrajevd.sHtML

static_cast<double>(a) / b
来源：http://baike.epnwcf.com/Article/details/gybolmlay.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.epnwcf.com/Article/details/gdyuxsofv.sHtML

int size() const noexcept { return n_; }
来源：http://3g.sjlbkw.cn/Article/details/ggdefdnzq.sHtML

[S53] C++：移动语义
来源：http://m.share.fktsv.cn/Article/details/gqblavgvf.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.bbcook.cn/Article/details/gkjtyoofr.sHtML

[S54] C++：异常处理
来源：http://wap.fktsv.cn/Article/details/gaepqiemn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.sjlbkw.cn/Article/details/gvrlrgyiz.sHtML

[S55] C++：结构化绑定
来源：http://read.share.bbcook.cn/Article/details/gtmujdbkk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.sjlbkw.cn/Article/details/gdulybztf.sHtML

[S56] C++：optional
来源：http://wap.fktsv.cn/Article/details/gacfukygt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.tarul.cn/Article/details/gruovnwbo.sHtML

[S57] C++：编译期常量
来源：http://www.share.tarul.cn/Article/details/gwpveyqso.sHtML

constexpr int N = 10;
来源：http://www.share.bbcook.cn/Article/details/gxfadjlwv.sHtML

[S58] C++：命名空间
来源：http://wap.yfazqb.com/Article/details/govrwdlsh.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fktsv.cn/Article/details/gspffnlig.sHtML

[S59] C++：静态断言
来源：http://www.blog.yfazqb.com/Article/details/gtourgzpw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.epnwcf.com/Article/details/gjprlgiqs.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.tarul.cn/Article/details/glheayyqk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.yfazqb.com/Article/details/gvxcsuffa.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gupuhhilk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fktsv.cn/Article/details/gxthaupcq.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gkeiyhujw.sHtML

[T01] Kotlin：Hello World
来源：http://blog.bbcook.cn/Article/details/glketpzvq.sHtML

println("Hello")
来源：http://m.share.tarul.cn/Article/details/gqusgdmhx.sHtML

[T02] Kotlin：变量
来源：http://wap.bbcook.cn/Article/details/gxzocgjtz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.tarul.cn/Article/details/gojohwadz.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.vehdjk.com/Article/details/gxjojtvan.sHtML

"值: $b"
来源：http://www.blog.epnwcf.com/Article/details/gnzbrkszz.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.tarul.cn/Article/details/gmcdgynjr.sHtML

val n: String? = null;  n?.length
来源：http://blog.sjlbkw.cn/Article/details/gwlezmqcg.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.epnwcf.com/Article/details/gpiryvtyj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fktsv.cn/Article/details/grrujrzgn.sHtML

[T06] Kotlin：集合映射
来源：http://blog.yfazqb.com/Article/details/gpzkzjkmj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.yfazqb.com/Article/details/gecfcvzlg.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.yfazqb.com/Article/details/garmnxwkl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.yfazqb.com/Article/details/gywthkpms.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.sjlbkw.cn/Article/details/glxihukpo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.vehdjk.com/Article/details/gmewqjbbb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.tarul.cn/Article/details/gelomdjcr.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.yfazqb.com/Article/details/gxlwkznli.sHtML

[T10] Kotlin：默认参数
来源：http://blog.bbcook.cn/Article/details/gvztinneb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.vehdjk.com/Article/details/gsuzycddn.sHtML

[T11] Kotlin：协程
来源：http://read.share.tarul.cn/Article/details/graxyxctv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.yfazqb.com/Article/details/ggfgacchs.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.bbcook.cn/Article/details/gjbbafxlg.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.bbcook.cn/Article/details/geuvawwrx.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.tarul.cn/Article/details/gpwnxonhv.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.yfazqb.com/Article/details/giihyphdk.sHtML

[T14] Kotlin：循环
来源：http://read.share.tarul.cn/Article/details/gbmfkximy.sHtML

for (i in 1..10) println(i)
来源：http://read.share.yfazqb.com/Article/details/gtolynrcq.sHtML

[T15] Kotlin：接口
来源：http://www.share.vehdjk.com/Article/details/gktqzbwor.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.vehdjk.com/Article/details/gutydxnwl.sHtML

[T16] Swift：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/ghguncncn.sHtML

print("Hello")
来源：http://read.share.fktsv.cn/Article/details/gewmkcvcm.sHtML

[T17] Swift：变量与常量
来源：http://blog.epnwcf.com/Article/details/gtjhlsxrp.sHtML

var a = 1;  let b = 2
来源：http://3g.bbcook.cn/Article/details/gahtvnknu.sHtML

[T18] Swift：字符串插值
来源：http://wap.yfazqb.com/Article/details/gfpbffvvp.sHtML

"值: \(b)"
来源：http://blog.vehdjk.com/Article/details/gsuilbxvx.sHtML

[T19] Swift：可选绑定
来源：http://baike.fktsv.cn/Article/details/gqklfffsx.sHtML

if let n = opt { print(n) }
来源：http://read.share.tarul.cn/Article/details/gkdajizlf.sHtML

[T20] Swift：数组操作
来源：http://read.share.epnwcf.com/Article/details/gcktlvuwj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.tarul.cn/Article/details/gvnduxgoo.sHtML

[T21] Swift：遍历
来源：http://baike.fktsv.cn/Article/details/gnftdxvlx.sHtML

for x in a { print(x) }
来源：http://www.blog.sjlbkw.cn/Article/details/gzbheisdv.sHtML

[T22] Swift：字典
来源：http://wap.sjlbkw.cn/Article/details/gmtjvfxud.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.tarul.cn/Article/details/guqlcczzb.sHtML

[T23] Swift：函数
来源：http://baike.sjlbkw.cn/Article/details/glanvnftd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fktsv.cn/Article/details/gzomjrhjs.sHtML

[T24] Swift：闭包
来源：http://3g.fktsv.cn/Article/details/gmggmzxff.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.vehdjk.com/Article/details/gsojfaubv.sHtML

[T25] Swift：结构体
来源：http://www.share.sjlbkw.cn/Article/details/gvcyfqqpk.sHtML

struct P { var x: Int }
来源：http://read.share.fktsv.cn/Article/details/gglubvmrt.sHtML

[T26] Swift：类与重写
来源：http://www.blog.tarul.cn/Article/details/gwfimbncj.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.yfazqb.com/Article/details/gnhpcgezw.sHtML

[T27] Swift：错误处理
来源：http://baike.fktsv.cn/Article/details/gragftsbf.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.bbcook.cn/Article/details/gqytlcgzw.sHtML

[T28] Swift：枚举
来源：http://read.share.sjlbkw.cn/Article/details/gyoxkxiso.sHtML

enum Color { case red, green }
来源：http://www.share.vehdjk.com/Article/details/gncaqytwa.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.vehdjk.com/Article/details/gljoeobkd.sHtML

guard let x = opt else { return }
来源：http://www.share.fktsv.cn/Article/details/glytqinxx.sHtML

[T30] Swift：协议
来源：http://www.share.epnwcf.com/Article/details/gpkvnipsp.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fktsv.cn/Article/details/glzizatep.sHtML

[T31] Lua：Hello World
来源：http://blog.tarul.cn/Article/details/gjunkqakq.sHtML

print("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gzbizvwcc.sHtML

[T32] Lua：局部变量
来源：http://www.share.yfazqb.com/Article/details/gpuffydxa.sHtML

local a = 1
来源：http://blog.fktsv.cn/Article/details/gbwaomgxq.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.sjlbkw.cn/Article/details/guewkxcyq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.vehdjk.com/Article/details/gdyhqkerb.sHtML

[T34] Lua：遍历表
来源：http://3g.tarul.cn/Article/details/ghqmrtnmz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.vehdjk.com/Article/details/gdtmhrzkp.sHtML

[T35] Lua：字典表
来源：http://3g.sjlbkw.cn/Article/details/gfzvhcyjd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.bbcook.cn/Article/details/gqdbjynai.sHtML

[T36] Lua：函数
来源：http://baike.vehdjk.com/Article/details/gakqyuhgc.sHtML

function add(a, b) return a + b end
来源：http://wap.epnwcf.com/Article/details/gmnlxkplk.sHtML

[T37] Lua：字符串拼接
来源：http://3g.yfazqb.com/Article/details/gwpvmliho.sHtML

"a" .. "b"
来源：http://m.share.tarul.cn/Article/details/gvulaymjx.sHtML

[T38] Lua：条件
来源：http://read.share.fktsv.cn/Article/details/gxtqaokxq.sHtML

if x > 0 then print("正") end
来源：http://wap.tarul.cn/Article/details/gthwhzevd.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.epnwcf.com/Article/details/gtdjrvhez.sHtML

string.find(s, "%d+")
来源：http://baike.epnwcf.com/Article/details/gqbzklapn.sHtML

[T40] Lua：元表
来源：http://www.blog.fktsv.cn/Article/details/gxekqiedt.sHtML

setmetatable({}, { __index = base })
来源：http://baike.sjlbkw.cn/Article/details/gzkibfxfx.sHtML

[T41] Perl：Hello World
来源：http://3g.yfazqb.com/Article/details/ggjusuodu.sHtML

print "Hello\n";
来源：http://baike.yfazqb.com/Article/details/gmybzwxji.sHtML

[T42] Perl：变量类型
来源：http://m.share.vehdjk.com/Article/details/gffxnluzp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.yfazqb.com/Article/details/gdacwsbfu.sHtML

[T43] Perl：字符串插值
来源：http://www.share.tarul.cn/Article/details/gbgatrrfg.sHtML

"值: $a"
来源：http://blog.yfazqb.com/Article/details/gfznyatio.sHtML

[T44] Perl：条件
来源：http://www.blog.bbcook.cn/Article/details/glwxpotmh.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.tarul.cn/Article/details/gkkcmcnrg.sHtML

[T45] Perl：数组遍历
来源：http://m.share.tarul.cn/Article/details/gvvchhxsq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.yfazqb.com/Article/details/gqmmizjxh.sHtML

[T46] Perl：哈希操作
来源：http://read.share.vehdjk.com/Article/details/gsgolsiax.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.tarul.cn/Article/details/gshrplwop.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.yfazqb.com/Article/details/gwnkeiito.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.vehdjk.com/Article/details/gftfasmga.sHtML

[T48] Perl：正则替换
来源：http://baike.vehdjk.com/Article/details/glacldgej.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.yfazqb.com/Article/details/gccqgcjjo.sHtML

[T49] Perl：函数
来源：http://3g.sjlbkw.cn/Article/details/gzmpjueud.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/goovlcktq.sHtML

[T50] Perl：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gdjxecrac.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fktsv.cn/Article/details/gxxrpesqx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.sjlbkw.cn/Article/details/gjvykgsqs.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gtutbefiu.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/gvqxdkaeg.sHtML

[T52] Scala：变量
来源：http://read.share.fktsv.cn/Article/details/grrprxxna.sHtML

val a = 1;  var b = 2
来源：http://wap.fktsv.cn/Article/details/gxzzdazpn.sHtML

[T53] Scala：字符串插值
来源：http://3g.yfazqb.com/Article/details/gwyhkifal.sHtML

s"值: $b"
来源：http://www.share.tarul.cn/Article/details/gjsuutoph.sHtML

[T54] Scala：集合映射
来源：http://baike.sjlbkw.cn/Article/details/gazbhtzbq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.epnwcf.com/Article/details/gnrmzpcmd.sHtML

[T55] Scala：集合过滤
来源：http://blog.tarul.cn/Article/details/ghyocnugg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.yfazqb.com/Article/details/gaoposjng.sHtML

[T56] Scala：样例类
来源：http://mobile.bbcook.cn/Article/details/gblvlxtgd.sHtML

case class User(name: String, age: Int)
来源：http://baike.vehdjk.com/Article/details/gubndipti.sHtML

[T57] Scala：模式匹配
来源：http://m.share.yfazqb.com/Article/details/gkwpfjcxs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.bbcook.cn/Article/details/glloybwjv.sHtML

[T58] Scala：函数定义
来源：http://3g.epnwcf.com/Article/details/gvfsphwue.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.yfazqb.com/Article/details/gqzudoeac.sHtML

[T59] Scala：循环
来源：http://www.blog.bbcook.cn/Article/details/gtsmnyweh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.bbcook.cn/Article/details/gwhwhnorn.sHtML

[T60] Scala：折叠
来源：http://wap.epnwcf.com/Article/details/goabdneyb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.tarul.cn/Article/details/gunhjtekx.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gkcldqxyi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.bbcook.cn/Article/details/gbwnxuiwh.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/guevuwghv.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.yfazqb.com/Article/details/gfcoovotv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.epnwcf.com/Article/details/gxrgaojuu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.yfazqb.com/Article/details/gcgvektle.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.vehdjk.com/Article/details/gqatjszbg.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.sjlbkw.cn/Article/details/gqixdrctf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.bbcook.cn/Article/details/gzfkyhbyh.sHtML

[U04] Py：变量调试打印
来源：http://baike.yfazqb.com/Article/details/gfjuvwryd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fktsv.cn/Article/details/gomyqohjl.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.yfazqb.com/Article/details/gnkwmzwji.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.yfazqb.com/Article/details/gkdqhbkno.sHtML

[U06] Py：合并两个字典
来源：http://m.share.sjlbkw.cn/Article/details/gqbtwxgou.sHtML

{**a, **b}
来源：http://3g.sjlbkw.cn/Article/details/glqopuuht.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fktsv.cn/Article/details/gxfjivbnu.sHtML

{v: k for k, v in d.items()}
来源：http://baike.sjlbkw.cn/Article/details/gerukuxot.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.sjlbkw.cn/Article/details/ghkjhqhib.sHtML

[y for x in nested for y in x]
来源：http://www.share.vehdjk.com/Article/details/ggflloucz.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.yfazqb.com/Article/details/gfigmhanv.sHtML

max(d, key=d.get)
来源：http://wap.sjlbkw.cn/Article/details/gqtjwqsyq.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.yfazqb.com/Article/details/gajnjncjr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.vehdjk.com/Article/details/gupabqsxk.sHtML

[U11] Py：生成器表达式
来源：http://read.share.bbcook.cn/Article/details/gxrkdchcc.sHtML

(x * 2 for x in arr)
来源：http://blog.tarul.cn/Article/details/gvytginlv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.vehdjk.com/Article/details/glqrdtmej.sHtML

Counter(arr).most_common(3)
来源：http://baike.sjlbkw.cn/Article/details/gjzqtjxfs.sHtML

[U13] Py：固定长度队列
来源：http://baike.bbcook.cn/Article/details/gewzkrmre.sHtML

deque(maxlen=10)
来源：http://baike.epnwcf.com/Article/details/gvdrlkdpv.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.yfazqb.com/Article/details/gazzeimyq.sHtML

defaultdict(list)
来源：http://wap.vehdjk.com/Article/details/gwzecskic.sHtML

[U15] Py：高精度计时
来源：http://read.share.epnwcf.com/Article/details/gfifxtlex.sHtML

t = time.perf_counter()
来源：http://blog.tarul.cn/Article/details/gmmridjtt.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.sjlbkw.cn/Article/details/gfzkyrmhz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.vehdjk.com/Article/details/gypxwjvxl.sHtML

[U17] Py：初始化日志
来源：http://www.share.bbcook.cn/Article/details/gddazpxxh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.vehdjk.com/Article/details/ganpsason.sHtML

[U18] Py：预编译正则
来源：http://mobile.tarul.cn/Article/details/gapllbmyg.sHtML

pat = re.compile(r"\d+")
来源：http://wap.vehdjk.com/Article/details/ggtgybhjo.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fktsv.cn/Article/details/gmpdsbbhs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.vehdjk.com/Article/details/gbcyhmxpk.sHtML

[U20] Py：缓存函数结果
来源：http://blog.epnwcf.com/Article/details/gtkqceobf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.bbcook.cn/Article/details/glsgbydmk.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fktsv.cn/Article/details/gtvvxjiam.sHtML

@contextlib.contextmanager
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfiqnvet.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.tarul.cn/Article/details/girpsvlcu.sHtML

list(zip(*m))
来源：http://wap.epnwcf.com/Article/details/gcytuhczs.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.vehdjk.com/Article/details/gsgiptdxj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.tarul.cn/Article/details/gviysigtd.sHtML

[U24] Py：路径操作
来源：http://www.share.epnwcf.com/Article/details/ghexwesqq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.tarul.cn/Article/details/gqusnzgdj.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.yfazqb.com/Article/details/gvuhwlasd.sHtML

csv.DictReader(f)
来源：http://wap.epnwcf.com/Article/details/gexjavcgp.sHtML

[U26] Py：并发下载
来源：http://m.share.tarul.cn/Article/details/gteozmnql.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.sjlbkw.cn/Article/details/gjqrabafb.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.tarul.cn/Article/details/gyffqcfbr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.bbcook.cn/Article/details/gpvoqqaob.sHtML

[U28] Py：类型别名
来源：http://3g.vehdjk.com/Article/details/gqbngpsbu.sHtML

UserId = int
来源：http://www.m.share.epnwcf.com/Article/details/gtveoaigp.sHtML

[U29] Py：属性校验
来源：http://m.share.sjlbkw.cn/Article/details/gupibowlz.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.vehdjk.com/Article/details/gujookwix.sHtML

[U30] Py：数据类
来源：http://wap.sjlbkw.cn/Article/details/gpbdtqouk.sHtML

@dataclass(slots=True)
来源：http://wap.sjlbkw.cn/Article/details/gjvecwccd.sHtML

[U31] Py：单测
来源：http://blog.vehdjk.com/Article/details/grmcvwkgx.sHtML

python -m pytest -q
来源：http://www.blog.sjlbkw.cn/Article/details/gkfdhonza.sHtML

[U32] Py：代码格式化
来源：http://m.share.bbcook.cn/Article/details/gfexmfesm.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.vehdjk.com/Article/details/gpjkgbhxp.sHtML

[U33] Py：打包发布
来源：http://m.share.yfazqb.com/Article/details/gywpdeafw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.tarul.cn/Article/details/gwkdjcukv.sHtML

[U34] Py：判断编码
来源：http://3g.bbcook.cn/Article/details/gsxfneglh.sHtML

chardet.detect(raw)
来源：http://read.share.vehdjk.com/Article/details/gpsllbsqt.sHtML

[U35] Py：发送邮件
来源：http://www.share.vehdjk.com/Article/details/gsrgkceqt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.yfazqb.com/Article/details/gtcnnceyt.sHtML

[U36] Py：定时任务
来源：http://www.share.bbcook.cn/Article/details/gywxoejon.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.vehdjk.com/Article/details/gvzckmoai.sHtML

[U37] Py：读写 Excel
来源：http://wap.epnwcf.com/Article/details/gxwazthdw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.sjlbkw.cn/Article/details/gkuernbwv.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.yfazqb.com/Article/details/grssxjyda.sHtML

Path(__file__).resolve().parent
来源：http://blog.sjlbkw.cn/Article/details/gkzcsqnyv.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.yfazqb.com/Article/details/gwqpquaae.sHtML

sys.stdout.isatty()
来源：http://wap.sjlbkw.cn/Article/details/gkapzbqeh.sHtML

[U40] Py：打印到标准错误
来源：http://3g.sjlbkw.cn/Article/details/gswmeulfa.sHtML

print("err", file=sys.stderr)
来源：http://blog.yfazqb.com/Article/details/gaztpojpl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.vehdjk.com/Article/details/gtfvkpsro.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.epnwcf.com/Article/details/gsrfrcjqf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.vehdjk.com/Article/details/grzuavwyq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.bbcook.cn/Article/details/gnryhuzhw.sHtML

[U43] PHP：声明命名空间
来源：http://3g.sjlbkw.cn/Article/details/gmyouemqh.sHtML

namespace App\Http;
来源：http://www.m.share.epnwcf.com/Article/details/ganlhlhai.sHtML

[U44] PHP：开启严格类型
来源：http://3g.bbcook.cn/Article/details/gfydkwgqg.sHtML

declare(strict_types=1);
来源：http://www.share.vehdjk.com/Article/details/gfifkhupr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.bbcook.cn/Article/details/gdbwmfbst.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gmrrjlitb.sHtML

[U46] PHP：可空类型
来源：http://3g.bbcook.cn/Article/details/gdaskdizy.sHtML

?string $name = null
来源：http://www.share.fktsv.cn/Article/details/gkflddurp.sHtML

[U47] PHP：联合类型
来源：http://mobile.fktsv.cn/Article/details/gnbovdknu.sHtML

int|string $id
来源：http://blog.vehdjk.com/Article/details/ghntphbtb.sHtML

[U48] PHP：纯枚举
来源：http://3g.tarul.cn/Article/details/grxuepyca.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.yfazqb.com/Article/details/gvojovopy.sHtML

[U49] PHP：只读属性
来源：http://m.share.yfazqb.com/Article/details/goavjhwsv.sHtML

public readonly string $name
来源：http://www.m.share.epnwcf.com/Article/details/gqrshpyfh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.bbcook.cn/Article/details/ghgrrwhxz.sHtML

public function __construct(private int $id) {}
来源：http://m.share.bbcook.cn/Article/details/gvoyzsybe.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.yfazqb.com/Article/details/gqcbkiqvz.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.vehdjk.com/Article/details/gpydcnxqs.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.vehdjk.com/Article/details/gneovrtsy.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.sjlbkw.cn/Article/details/gnxfefelt.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.epnwcf.com/Article/details/gvvzzjvgr.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.sjlbkw.cn/Article/details/gavhwjzvd.sHtML

[U54] PHP：空安全调用
来源：http://www.share.bbcook.cn/Article/details/grqeujbdm.sHtML

$obj?->method()
来源：http://read.share.tarul.cn/Article/details/gdwksnero.sHtML

[U55] PHP：match 表达式
来源：http://read.share.tarul.cn/Article/details/gvhxkhjar.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.epnwcf.com/Article/details/gquxdlrop.sHtML

[U56] PHP：命名参数
来源：http://www.share.tarul.cn/Article/details/goifflfup.sHtML

f(a: 1, b: 2)
来源：http://m.share.sjlbkw.cn/Article/details/gifeioghu.sHtML

[U57] PHP：字符串插值
来源：http://3g.tarul.cn/Article/details/gmbbnyfwd.sHtML

"值: {$a}"
来源：http://www.blog.epnwcf.com/Article/details/gzbgguaoz.sHtML

[U58] PHP：数组三件套
来源：http://wap.tarul.cn/Article/details/gvuptddze.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.epnwcf.com/Article/details/ggyripiua.sHtML

[U59] PHP：自定义排序
来源：http://www.share.vehdjk.com/Article/details/ghpetthen.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.tarul.cn/Article/details/gcdhbfckc.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.bbcook.cn/Article/details/gvomqfpze.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fktsv.cn/Article/details/gvteaschl.sHtML

[U61] PHP：正则
来源：http://3g.tarul.cn/Article/details/guniiuncp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gvhtqfnsj.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.epnwcf.com/Article/details/gjhabypmf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.yfazqb.com/Article/details/gjmfmojvd.sHtML

[U63] PHP：文件读写
来源：http://read.share.bbcook.cn/Article/details/ghayzvexf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.sjlbkw.cn/Article/details/ghkidjqvq.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gldczlnzo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.sjlbkw.cn/Article/details/gmjfranfp.sHtML


<!-- 参考信息 -->