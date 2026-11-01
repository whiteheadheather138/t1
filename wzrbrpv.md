代发 wailian999

[S39] C++：自定义比较器排序
来源：http://m.share.fktsv.cn/Article/details/gmqbmwsov.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fktsv.cn/Article/details/gmmgygtph.sHtML

[S40] C++：查找元素
来源：http://www.m.share.epnwcf.com/Article/details/gowcxyfjc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gttxwkvoo.sHtML

[S41] C++：类与构造函数
来源：http://mobile.bbcook.cn/Article/details/gekrygnpy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.yfazqb.com/Article/details/gmcdqadum.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.sjlbkw.cn/Article/details/gmktlmrix.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.vehdjk.com/Article/details/gzuzozolp.sHtML

[S43] C++：智能指针
来源：http://www.m.share.vehdjk.com/Article/details/gdbdhqohp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/gygodgnzj.sHtML

[S44] C++：引用传参
来源：http://m.share.epnwcf.com/Article/details/gascysahj.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.epnwcf.com/Article/details/gzspdxpdq.sHtML

[S45] C++：lambda
来源：http://www.m.share.epnwcf.com/Article/details/geaxrokhh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.vehdjk.com/Article/details/ghixcsfqq.sHtML

[S46] C++：函数模板
来源：http://baike.vehdjk.com/Article/details/gppbspbzj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.epnwcf.com/Article/details/gxgrakagm.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.bbcook.cn/Article/details/gwezfwwhv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.yfazqb.com/Article/details/gmovdrwwn.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gxrscaghq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.yfazqb.com/Article/details/ggqszftuc.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.vehdjk.com/Article/details/gpzfrckuq.sHtML

[S49] C++：写文件
来源：http://www.blog.tarul.cn/Article/details/gembnpbpw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.vehdjk.com/Article/details/gqaxlrhvv.sHtML

[S50] C++：格式化数字
来源：http://3g.tarul.cn/Article/details/gybttzrni.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gnnvbduht.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fktsv.cn/Article/details/gawowbeas.sHtML

static_cast<double>(a) / b
来源：http://mobile.bbcook.cn/Article/details/giyjhoylm.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.sjlbkw.cn/Article/details/gefvsyyoe.sHtML

int size() const noexcept { return n_; }
来源：http://3g.yfazqb.com/Article/details/gyctxyryz.sHtML

[S53] C++：移动语义
来源：http://www.share.bbcook.cn/Article/details/gucqxpdod.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.yfazqb.com/Article/details/gfhundwog.sHtML

[S54] C++：异常处理
来源：http://m.share.fktsv.cn/Article/details/gyebngwqp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.sjlbkw.cn/Article/details/gsiahvibv.sHtML

[S55] C++：结构化绑定
来源：http://read.share.tarul.cn/Article/details/gvdrpvjcn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.epnwcf.com/Article/details/grrlcxioz.sHtML

[S56] C++：optional
来源：http://www.m.share.vehdjk.com/Article/details/gilqyksld.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.bbcook.cn/Article/details/guxjubamk.sHtML

[S57] C++：编译期常量
来源：http://www.blog.sjlbkw.cn/Article/details/gfsmjqhph.sHtML

constexpr int N = 10;
来源：http://www.blog.bbcook.cn/Article/details/gnmembgtv.sHtML

[S58] C++：命名空间
来源：http://wap.epnwcf.com/Article/details/gjzgvktwz.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.yfazqb.com/Article/details/gydpkmbjr.sHtML

[S59] C++：静态断言
来源：http://blog.sjlbkw.cn/Article/details/gqkximepe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.sjlbkw.cn/Article/details/gknroloxv.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fktsv.cn/Article/details/gbfxfznes.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.tarul.cn/Article/details/ghkqsylxq.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gfuzbarha.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.epnwcf.com/Article/details/gfbojpvqk.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/grnonvjsl.sHtML

[T01] Kotlin：Hello World
来源：http://3g.yfazqb.com/Article/details/gpphtnjex.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/gacdcpzzi.sHtML

[T02] Kotlin：变量
来源：http://wap.vehdjk.com/Article/details/gichznkfc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.sjlbkw.cn/Article/details/gpovxjapn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.bbcook.cn/Article/details/gunuvnrxj.sHtML

"值: $b"
来源：http://3g.yfazqb.com/Article/details/gwdvsaetd.sHtML

[T04] Kotlin：空安全
来源：http://wap.bbcook.cn/Article/details/gusrijmnn.sHtML

val n: String? = null;  n?.length
来源：http://read.share.tarul.cn/Article/details/gpgfyitwx.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.sjlbkw.cn/Article/details/gvmwspaec.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.yfazqb.com/Article/details/gopcizurg.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.yfazqb.com/Article/details/gaflkqssz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.tarul.cn/Article/details/gchveoxsr.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.tarul.cn/Article/details/gyxppkldt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.epnwcf.com/Article/details/gkjjtxqfg.sHtML

[T08] Kotlin：数据类
来源：http://m.share.yfazqb.com/Article/details/gghneyocb.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.tarul.cn/Article/details/gxkmnhtsm.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.tarul.cn/Article/details/gxteclyel.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.epnwcf.com/Article/details/gsymobilo.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gbokasbeh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.yfazqb.com/Article/details/gvtskixid.sHtML

[T11] Kotlin：协程
来源：http://m.share.vehdjk.com/Article/details/gsxmofexp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.yfazqb.com/Article/details/gznbrvygs.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.vehdjk.com/Article/details/gyqhfzyer.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/gbvvpsfiq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.bbcook.cn/Article/details/gzjeppiif.sHtML

val m = mapOf("a" to 1)
来源：http://wap.epnwcf.com/Article/details/glrierdzj.sHtML

[T14] Kotlin：循环
来源：http://3g.tarul.cn/Article/details/gzucewrow.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.bbcook.cn/Article/details/gyysijdkw.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fktsv.cn/Article/details/gomdtiewf.sHtML

interface Shape { fun area(): Double }
来源：http://3g.tarul.cn/Article/details/gozaptods.sHtML

[T16] Swift：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gkaddhjfc.sHtML

print("Hello")
来源：http://mobile.bbcook.cn/Article/details/gmrcumvdv.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.vehdjk.com/Article/details/gtoijbovh.sHtML

var a = 1;  let b = 2
来源：http://baike.fktsv.cn/Article/details/gixooamtp.sHtML

[T18] Swift：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gurtgzutf.sHtML

"值: \(b)"
来源：http://mobile.sjlbkw.cn/Article/details/gjgymkyfn.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fktsv.cn/Article/details/gevydiatz.sHtML

if let n = opt { print(n) }
来源：http://m.share.sjlbkw.cn/Article/details/gakqorieb.sHtML

[T20] Swift：数组操作
来源：http://m.share.fktsv.cn/Article/details/gjwgypasw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.epnwcf.com/Article/details/gtthtgftt.sHtML

[T21] Swift：遍历
来源：http://read.share.tarul.cn/Article/details/gdtiraezy.sHtML

for x in a { print(x) }
来源：http://wap.epnwcf.com/Article/details/gpjlbbtlt.sHtML

[T22] Swift：字典
来源：http://www.share.yfazqb.com/Article/details/gkofpqwvf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.yfazqb.com/Article/details/gohpagmey.sHtML

[T23] Swift：函数
来源：http://m.share.vehdjk.com/Article/details/gmofcfpbz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.tarul.cn/Article/details/glosckusv.sHtML

[T24] Swift：闭包
来源：http://baike.fktsv.cn/Article/details/gsccjwyex.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fktsv.cn/Article/details/gjublkqpz.sHtML

[T25] Swift：结构体
来源：http://read.share.tarul.cn/Article/details/ghsahrwdx.sHtML

struct P { var x: Int }
来源：http://blog.vehdjk.com/Article/details/gfnqiyvwi.sHtML

[T26] Swift：类与重写
来源：http://blog.sjlbkw.cn/Article/details/gsodsvxsd.sHtML

class A: Base { override func f() {} }
来源：http://m.share.epnwcf.com/Article/details/gyhngjrxp.sHtML

[T27] Swift：错误处理
来源：http://m.share.epnwcf.com/Article/details/gmwcbykau.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.bbcook.cn/Article/details/gwbcnmntg.sHtML

[T28] Swift：枚举
来源：http://wap.tarul.cn/Article/details/gmqigntvv.sHtML

enum Color { case red, green }
来源：http://read.share.sjlbkw.cn/Article/details/gcaydycca.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.vehdjk.com/Article/details/gpcxisnqh.sHtML

guard let x = opt else { return }
来源：http://www.m.share.vehdjk.com/Article/details/gluxekfiv.sHtML

[T30] Swift：协议
来源：http://wap.bbcook.cn/Article/details/gniolnbls.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.bbcook.cn/Article/details/gzauwcgnm.sHtML

[T31] Lua：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gnkqzzrqc.sHtML

print("Hello")
来源：http://www.share.epnwcf.com/Article/details/grlcgfija.sHtML

[T32] Lua：局部变量
来源：http://3g.fktsv.cn/Article/details/gdwivgoxc.sHtML

local a = 1
来源：http://wap.yfazqb.com/Article/details/guqpalqux.sHtML

[T33] Lua：表（数组）
来源：http://wap.vehdjk.com/Article/details/gtjdfsljx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fktsv.cn/Article/details/gkhvezeyi.sHtML

[T34] Lua：遍历表
来源：http://m.share.yfazqb.com/Article/details/gverdrwhs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.yfazqb.com/Article/details/gwpqspxsf.sHtML

[T35] Lua：字典表
来源：http://m.share.epnwcf.com/Article/details/gfievkngz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.tarul.cn/Article/details/gjatxtofj.sHtML

[T36] Lua：函数
来源：http://blog.sjlbkw.cn/Article/details/gsghuknws.sHtML

function add(a, b) return a + b end
来源：http://www.share.epnwcf.com/Article/details/guhdwnpzl.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.epnwcf.com/Article/details/gjahcmeyn.sHtML

"a" .. "b"
来源：http://www.blog.tarul.cn/Article/details/gubrlolfn.sHtML

[T38] Lua：条件
来源：http://www.blog.yfazqb.com/Article/details/ghlzkuicv.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fktsv.cn/Article/details/gnshpnbdg.sHtML

[T39] Lua：模式匹配
来源：http://baike.sjlbkw.cn/Article/details/gjsvhgtip.sHtML

string.find(s, "%d+")
来源：http://wap.bbcook.cn/Article/details/gugkhgbtx.sHtML

[T40] Lua：元表
来源：http://baike.sjlbkw.cn/Article/details/grgjkmujp.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.epnwcf.com/Article/details/gbdwxjsec.sHtML

[T41] Perl：Hello World
来源：http://3g.bbcook.cn/Article/details/gvapvfdxx.sHtML

print "Hello\n";
来源：http://read.share.sjlbkw.cn/Article/details/gieorybcg.sHtML

[T42] Perl：变量类型
来源：http://blog.bbcook.cn/Article/details/gzhvmczbf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.yfazqb.com/Article/details/gmyhtnkpl.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gqphrsyej.sHtML

"值: $a"
来源：http://mobile.fktsv.cn/Article/details/guwpaqzyu.sHtML

[T44] Perl：条件
来源：http://wap.yfazqb.com/Article/details/gakrvwlpz.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fktsv.cn/Article/details/givketuep.sHtML

[T45] Perl：数组遍历
来源：http://m.share.yfazqb.com/Article/details/gtmwaamyu.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.sjlbkw.cn/Article/details/gbezylono.sHtML

[T46] Perl：哈希操作
来源：http://3g.epnwcf.com/Article/details/gbdktokzz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.sjlbkw.cn/Article/details/grkyodeyp.sHtML

[T47] Perl：正则捕获
来源：http://mobile.sjlbkw.cn/Article/details/grnooweaq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fktsv.cn/Article/details/gvxkpbnzl.sHtML

[T48] Perl：正则替换
来源：http://m.share.bbcook.cn/Article/details/gmuajzyzx.sHtML

$s =~ s/old/new/g;
来源：http://read.share.vehdjk.com/Article/details/gltpjrwew.sHtML

[T49] Perl：函数
来源：http://www.share.vehdjk.com/Article/details/gjehscwif.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gxbqqxngn.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gcispndcw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.yfazqb.com/Article/details/gshaeciza.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.bbcook.cn/Article/details/gvkhstvbo.sHtML

[T51] Scala：Hello World
来源：http://wap.bbcook.cn/Article/details/gkkfcrogt.sHtML

println("Hello")
来源：http://blog.vehdjk.com/Article/details/gupzvsjfx.sHtML

[T52] Scala：变量
来源：http://www.blog.yfazqb.com/Article/details/gtiylzauq.sHtML

val a = 1;  var b = 2
来源：http://m.share.vehdjk.com/Article/details/gudxzjrhk.sHtML

[T53] Scala：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gtevsbmrt.sHtML

s"值: $b"
来源：http://read.share.epnwcf.com/Article/details/gxnuetsuj.sHtML

[T54] Scala：集合映射
来源：http://blog.fktsv.cn/Article/details/gjicrgelk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.tarul.cn/Article/details/gftrcjqhd.sHtML

[T55] Scala：集合过滤
来源：http://mobile.tarul.cn/Article/details/ggjxpvgjy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.bbcook.cn/Article/details/gcgfonfge.sHtML

[T56] Scala：样例类
来源：http://read.share.sjlbkw.cn/Article/details/gqfpkupbs.sHtML

case class User(name: String, age: Int)
来源：http://read.share.bbcook.cn/Article/details/gisqzdoxq.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.epnwcf.com/Article/details/gozzkrgdb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.yfazqb.com/Article/details/gjeyoioyw.sHtML

[T58] Scala：函数定义
来源：http://3g.vehdjk.com/Article/details/gdpxglzai.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.tarul.cn/Article/details/gzicxszid.sHtML

[T59] Scala：循环
来源：http://mobile.vehdjk.com/Article/details/gvnbjhocf.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.sjlbkw.cn/Article/details/gptcunqvz.sHtML

[T60] Scala：折叠
来源：http://baike.epnwcf.com/Article/details/gcolxbytl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fktsv.cn/Article/details/gszyyioir.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/giodqzify.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.yfazqb.com/Article/details/gdkdvyzqx.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ggbupimjc.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.tarul.cn/Article/details/gohvtfaix.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.yfazqb.com/Article/details/ghrstlvhi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.yfazqb.com/Article/details/gmgpfxtih.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.epnwcf.com/Article/details/ggwabovjx.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.vehdjk.com/Article/details/gcggqfxoo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.yfazqb.com/Article/details/gbyodjcke.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.tarul.cn/Article/details/gramkadie.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.epnwcf.com/Article/details/gkctiblrx.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.bbcook.cn/Article/details/gvyemxpde.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.vehdjk.com/Article/details/gstelcbhg.sHtML

[U06] Py：合并两个字典
来源：http://3g.fktsv.cn/Article/details/gilbyjdgy.sHtML

{**a, **b}
来源：http://www.m.share.epnwcf.com/Article/details/gyascgzdl.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.yfazqb.com/Article/details/gktgkyyzx.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fktsv.cn/Article/details/glwbikhtp.sHtML

[U08] Py：展平二维列表
来源：http://blog.bbcook.cn/Article/details/gvssazohw.sHtML

[y for x in nested for y in x]
来源：http://www.blog.sjlbkw.cn/Article/details/gqdazgdeh.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.epnwcf.com/Article/details/gbapuskuy.sHtML

max(d, key=d.get)
来源：http://wap.sjlbkw.cn/Article/details/gylaygnvg.sHtML

[U10] Py：按值排序字典
来源：http://mobile.bbcook.cn/Article/details/gjkwfshjr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.sjlbkw.cn/Article/details/gkeibkguk.sHtML

[U11] Py：生成器表达式
来源：http://read.share.bbcook.cn/Article/details/gjiclouxs.sHtML

(x * 2 for x in arr)
来源：http://3g.bbcook.cn/Article/details/gkukufmqa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.yfazqb.com/Article/details/geusljgsz.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.yfazqb.com/Article/details/guxavuibh.sHtML

[U13] Py：固定长度队列
来源：http://wap.bbcook.cn/Article/details/gnacwdhvu.sHtML

deque(maxlen=10)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggvzbnelo.sHtML

[U14] Py：分组收集到列表
来源：http://baike.yfazqb.com/Article/details/gwsejszqm.sHtML

defaultdict(list)
来源：http://www.m.share.vehdjk.com/Article/details/ghswdwlrb.sHtML

[U15] Py：高精度计时
来源：http://baike.tarul.cn/Article/details/gnyrmtmxm.sHtML

t = time.perf_counter()
来源：http://www.share.yfazqb.com/Article/details/gtpdlkbzq.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.yfazqb.com/Article/details/geapsdqtr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.epnwcf.com/Article/details/gcmoympdv.sHtML

[U17] Py：初始化日志
来源：http://3g.sjlbkw.cn/Article/details/gdgjtascq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fktsv.cn/Article/details/gumaiqwus.sHtML

[U18] Py：预编译正则
来源：http://3g.sjlbkw.cn/Article/details/glwbmeywr.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.bbcook.cn/Article/details/guttmzmzz.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.bbcook.cn/Article/details/grbdcvrbf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.bbcook.cn/Article/details/gbdjxrlym.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.tarul.cn/Article/details/gzcewmsvn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.tarul.cn/Article/details/gtsbmzooo.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.bbcook.cn/Article/details/gsoighzqf.sHtML

@contextlib.contextmanager
来源：http://m.share.bbcook.cn/Article/details/gqrgrlouc.sHtML

[U22] Py：矩阵转置
来源：http://mobile.vehdjk.com/Article/details/gwfpyamyc.sHtML

list(zip(*m))
来源：http://3g.bbcook.cn/Article/details/gkbgwaisj.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fktsv.cn/Article/details/gdgnpoftj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.vehdjk.com/Article/details/grffwewel.sHtML

[U24] Py：路径操作
来源：http://www.share.epnwcf.com/Article/details/gurpicwlp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.vehdjk.com/Article/details/gwkzeizwa.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.bbcook.cn/Article/details/gywymoqkl.sHtML

csv.DictReader(f)
来源：http://www.m.share.tarul.cn/Article/details/gvcwkisvn.sHtML

[U26] Py：并发下载
来源：http://mobile.bbcook.cn/Article/details/gwzzhpdva.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.yfazqb.com/Article/details/gmyoshqhe.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.yfazqb.com/Article/details/gejfeafig.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fktsv.cn/Article/details/gtjgbgvmj.sHtML

[U28] Py：类型别名
来源：http://3g.vehdjk.com/Article/details/ghfiajhzc.sHtML

UserId = int
来源：http://m.share.fktsv.cn/Article/details/gntbnqlcj.sHtML

[U29] Py：属性校验
来源：http://baike.epnwcf.com/Article/details/gthrzmpfb.sHtML

@property 与 @x.setter 配合
来源：http://www.share.tarul.cn/Article/details/gtceexetb.sHtML

[U30] Py：数据类
来源：http://3g.epnwcf.com/Article/details/gbcfgqjce.sHtML

@dataclass(slots=True)
来源：http://www.share.yfazqb.com/Article/details/gkyqqsoob.sHtML

[U31] Py：单测
来源：http://mobile.bbcook.cn/Article/details/govjbshjr.sHtML

python -m pytest -q
来源：http://baike.sjlbkw.cn/Article/details/gciihqpez.sHtML

[U32] Py：代码格式化
来源：http://www.share.bbcook.cn/Article/details/gatjoiasp.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.bbcook.cn/Article/details/goimyawsv.sHtML

[U33] Py：打包发布
来源：http://3g.sjlbkw.cn/Article/details/glydtkejn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.bbcook.cn/Article/details/gdromigpp.sHtML

[U34] Py：判断编码
来源：http://blog.bbcook.cn/Article/details/gdayekbkn.sHtML

chardet.detect(raw)
来源：http://www.share.yfazqb.com/Article/details/gbfizgmav.sHtML

[U35] Py：发送邮件
来源：http://baike.bbcook.cn/Article/details/gfuqdjdzq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.epnwcf.com/Article/details/gexhgyaqj.sHtML

[U36] Py：定时任务
来源：http://www.blog.epnwcf.com/Article/details/ggdtnwcys.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.sjlbkw.cn/Article/details/gmfhrvasy.sHtML

[U37] Py：读写 Excel
来源：http://mobile.vehdjk.com/Article/details/gxgkcywup.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.epnwcf.com/Article/details/gfsqvqqef.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fktsv.cn/Article/details/gjlsxapav.sHtML

Path(__file__).resolve().parent
来源：http://m.share.tarul.cn/Article/details/grtvcfmui.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.sjlbkw.cn/Article/details/gseizkolv.sHtML

sys.stdout.isatty()
来源：http://baike.epnwcf.com/Article/details/gdzyhbens.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.sjlbkw.cn/Article/details/ghpgwuudd.sHtML

print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/gbsnclcor.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.sjlbkw.cn/Article/details/gjckrxfkt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.vehdjk.com/Article/details/gxcbgpjbq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fktsv.cn/Article/details/gaytddynm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.bbcook.cn/Article/details/gshohxzyu.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.epnwcf.com/Article/details/gzvfxupfb.sHtML

namespace App\Http;
来源：http://read.share.fktsv.cn/Article/details/gnwdvfrsv.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.sjlbkw.cn/Article/details/gtlfeoxfq.sHtML

declare(strict_types=1);
来源：http://3g.vehdjk.com/Article/details/gtimpaxbo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.bbcook.cn/Article/details/gcxywgsow.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gkuheqvxo.sHtML

[U46] PHP：可空类型
来源：http://www.share.epnwcf.com/Article/details/gcsqtghux.sHtML

?string $name = null
来源：http://wap.yfazqb.com/Article/details/gcegiqatj.sHtML

[U47] PHP：联合类型
来源：http://read.share.tarul.cn/Article/details/grxuhaxfj.sHtML

int|string $id
来源：http://www.blog.sjlbkw.cn/Article/details/gbpvxxpod.sHtML

[U48] PHP：纯枚举
来源：http://www.share.bbcook.cn/Article/details/gdggxkply.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.vehdjk.com/Article/details/gfwyzvzno.sHtML

[U49] PHP：只读属性
来源：http://www.blog.bbcook.cn/Article/details/gnidbzfiq.sHtML

public readonly string $name
来源：http://3g.bbcook.cn/Article/details/gaupaxvxu.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.vehdjk.com/Article/details/gdzhvtpdn.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.epnwcf.com/Article/details/gzoihaymx.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.vehdjk.com/Article/details/gpzkqaqzs.sHtML

[$a, $b] = $arr;
来源：http://mobile.fktsv.cn/Article/details/gdklcclpw.sHtML

[U52] PHP：箭头函数
来源：http://www.share.yfazqb.com/Article/details/gwwffcxwb.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.vehdjk.com/Article/details/gijjlvfum.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fktsv.cn/Article/details/gqiygitqo.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.tarul.cn/Article/details/gfheotxcq.sHtML

[U54] PHP：空安全调用
来源：http://read.share.yfazqb.com/Article/details/gpmzoqdcg.sHtML

$obj?->method()
来源：http://read.share.tarul.cn/Article/details/gxuuqnxeq.sHtML

[U55] PHP：match 表达式
来源：http://blog.bbcook.cn/Article/details/gvvelxihm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.bbcook.cn/Article/details/ghvpmofit.sHtML

[U56] PHP：命名参数
来源：http://mobile.fktsv.cn/Article/details/grjzoorsl.sHtML

f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/goybpemze.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/gvyisuxks.sHtML

"值: {$a}"
来源：http://3g.vehdjk.com/Article/details/gplmcbtzy.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.epnwcf.com/Article/details/gnywbjjbe.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gskesmjav.sHtML

[U59] PHP：自定义排序
来源：http://blog.bbcook.cn/Article/details/ggbmpehby.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fktsv.cn/Article/details/gnsynqfvp.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.yfazqb.com/Article/details/gmgyeivxb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.yfazqb.com/Article/details/gtalecnvg.sHtML

[U61] PHP：正则
来源：http://www.share.tarul.cn/Article/details/goeigtcqa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.vehdjk.com/Article/details/grdrxvsmw.sHtML

[U62] PHP：日期对象
来源：http://mobile.epnwcf.com/Article/details/gfbgscqhf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.sjlbkw.cn/Article/details/gobvamjxy.sHtML

[U63] PHP：文件读写
来源：http://mobile.tarul.cn/Article/details/gjogmtbba.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.yfazqb.com/Article/details/ggvdktoxr.sHtML

[U64] PHP：目录遍历
来源：http://read.share.bbcook.cn/Article/details/grywbsiad.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fktsv.cn/Article/details/gmsyqzdjd.sHtML


<!-- 参考信息 -->