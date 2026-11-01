代发 wailian999

[S39] C++：自定义比较器排序
来源：http://wap.yfazqb.com/Article/details/gmzlhblfs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.bbcook.cn/Article/details/gsjhiyozg.sHtML

[S40] C++：查找元素
来源：http://m.share.bbcook.cn/Article/details/gzfqvtbyn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.yfazqb.com/Article/details/gyeprryzi.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gpnnxnjjk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fktsv.cn/Article/details/gczouscub.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fktsv.cn/Article/details/gkgdzpdht.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.vehdjk.com/Article/details/gonuzjjms.sHtML

[S43] C++：智能指针
来源：http://wap.yfazqb.com/Article/details/gpjtuvyuv.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.epnwcf.com/Article/details/gryhbuqee.sHtML

[S44] C++：引用传参
来源：http://baike.fktsv.cn/Article/details/grihshcit.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.bbcook.cn/Article/details/ganjinhdj.sHtML

[S45] C++：lambda
来源：http://read.share.vehdjk.com/Article/details/gigazdhlx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.tarul.cn/Article/details/gkyawunai.sHtML

[S46] C++：函数模板
来源：http://m.share.sjlbkw.cn/Article/details/gdmjjweme.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.yfazqb.com/Article/details/gfgzzlrqj.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.yfazqb.com/Article/details/ghgmujcph.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.vehdjk.com/Article/details/gejewxrqx.sHtML

[S48] C++：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gktxintnf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.epnwcf.com/Article/details/gksxclcrr.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fktsv.cn/Article/details/grrmyqcvg.sHtML

[S49] C++：写文件
来源：http://www.share.sjlbkw.cn/Article/details/gaobewcyi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhpsfztj.sHtML

[S50] C++：格式化数字
来源：http://baike.vehdjk.com/Article/details/gzaxoaheq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.vehdjk.com/Article/details/gbruflvfz.sHtML

[S51] C++：显式类型转换
来源：http://mobile.vehdjk.com/Article/details/ggkomzstk.sHtML

static_cast<double>(a) / b
来源：http://read.share.tarul.cn/Article/details/grgzigazl.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.yfazqb.com/Article/details/gwvyzzmcb.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.yfazqb.com/Article/details/gzweusvua.sHtML

[S53] C++：移动语义
来源：http://www.share.bbcook.cn/Article/details/gpqfykyro.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.sjlbkw.cn/Article/details/gsxvclchk.sHtML

[S54] C++：异常处理
来源：http://www.share.sjlbkw.cn/Article/details/gmczbebjf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.yfazqb.com/Article/details/gogbfqcep.sHtML

[S55] C++：结构化绑定
来源：http://baike.yfazqb.com/Article/details/gtighcibv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.epnwcf.com/Article/details/gauwnqjbg.sHtML

[S56] C++：optional
来源：http://www.blog.fktsv.cn/Article/details/gkgfbxuep.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.yfazqb.com/Article/details/gwatukwka.sHtML

[S57] C++：编译期常量
来源：http://blog.fktsv.cn/Article/details/gnawsgprv.sHtML

constexpr int N = 10;
来源：http://www.blog.vehdjk.com/Article/details/gvsvgielg.sHtML

[S58] C++：命名空间
来源：http://www.blog.vehdjk.com/Article/details/ghlyppzbn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.tarul.cn/Article/details/gxzfwpcsg.sHtML

[S59] C++：静态断言
来源：http://wap.epnwcf.com/Article/details/goifanavq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.bbcook.cn/Article/details/glhbvwihr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.sjlbkw.cn/Article/details/giwqqzaxf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.tarul.cn/Article/details/glmbqrsyv.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gurvnxvqk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.vehdjk.com/Article/details/gywykcbkb.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gigqdravj.sHtML

[T01] Kotlin：Hello World
来源：http://3g.bbcook.cn/Article/details/ghvjggykz.sHtML

println("Hello")
来源：http://mobile.fktsv.cn/Article/details/gmfumxfhc.sHtML

[T02] Kotlin：变量
来源：http://blog.tarul.cn/Article/details/gypymxqbn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.yfazqb.com/Article/details/gwscrrpyw.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.yfazqb.com/Article/details/gswznwctw.sHtML

"值: $b"
来源：http://read.share.sjlbkw.cn/Article/details/gtugexmyf.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.sjlbkw.cn/Article/details/gkagwejmq.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fktsv.cn/Article/details/gpxruolal.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.epnwcf.com/Article/details/gckpqkbfx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.epnwcf.com/Article/details/ghvckefgc.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.epnwcf.com/Article/details/gadehebao.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.yfazqb.com/Article/details/guwcdhspm.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.sjlbkw.cn/Article/details/gcgpmrqsz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.epnwcf.com/Article/details/gsohfgpuj.sHtML

[T08] Kotlin：数据类
来源：http://mobile.epnwcf.com/Article/details/ghtkosysv.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.sjlbkw.cn/Article/details/guvsuwqdf.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fktsv.cn/Article/details/gogcobpbt.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.yfazqb.com/Article/details/gieftzzcb.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gvknpfutm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.tarul.cn/Article/details/gfdckhcbf.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fktsv.cn/Article/details/gltwtjvbo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.tarul.cn/Article/details/gojssswab.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.yfazqb.com/Article/details/gdwdkkzzs.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gdbutjuvm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fktsv.cn/Article/details/giuuoyyjp.sHtML

val m = mapOf("a" to 1)
来源：http://wap.tarul.cn/Article/details/gjsfhwxuu.sHtML

[T14] Kotlin：循环
来源：http://m.share.vehdjk.com/Article/details/ggejjzsjs.sHtML

for (i in 1..10) println(i)
来源：http://mobile.yfazqb.com/Article/details/ghtqpfiay.sHtML

[T15] Kotlin：接口
来源：http://blog.sjlbkw.cn/Article/details/gojebgcqz.sHtML

interface Shape { fun area(): Double }
来源：http://3g.tarul.cn/Article/details/gbyhnmboi.sHtML

[T16] Swift：Hello World
来源：http://www.share.tarul.cn/Article/details/genymendz.sHtML

print("Hello")
来源：http://m.share.tarul.cn/Article/details/gnsudtrxh.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.vehdjk.com/Article/details/gdnfutvfj.sHtML

var a = 1;  let b = 2
来源：http://blog.epnwcf.com/Article/details/gsxdkyvna.sHtML

[T18] Swift：字符串插值
来源：http://wap.epnwcf.com/Article/details/gbqljfewm.sHtML

"值: \(b)"
来源：http://www.blog.yfazqb.com/Article/details/gavkzavmv.sHtML

[T19] Swift：可选绑定
来源：http://baike.bbcook.cn/Article/details/gyezuudku.sHtML

if let n = opt { print(n) }
来源：http://mobile.tarul.cn/Article/details/grvbqptdl.sHtML

[T20] Swift：数组操作
来源：http://3g.yfazqb.com/Article/details/gnksorxoo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.vehdjk.com/Article/details/gzbfynczn.sHtML

[T21] Swift：遍历
来源：http://blog.yfazqb.com/Article/details/gadxqjbfh.sHtML

for x in a { print(x) }
来源：http://3g.yfazqb.com/Article/details/gvsekqdpn.sHtML

[T22] Swift：字典
来源：http://wap.vehdjk.com/Article/details/gtfilphqn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.tarul.cn/Article/details/gkzzapwhm.sHtML

[T23] Swift：函数
来源：http://www.m.share.epnwcf.com/Article/details/gdhtazmcn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.tarul.cn/Article/details/gcitpybtj.sHtML

[T24] Swift：闭包
来源：http://mobile.tarul.cn/Article/details/gscoadjkx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.bbcook.cn/Article/details/gyanzparq.sHtML

[T25] Swift：结构体
来源：http://wap.fktsv.cn/Article/details/gcdenealy.sHtML

struct P { var x: Int }
来源：http://3g.vehdjk.com/Article/details/gbxitdjwg.sHtML

[T26] Swift：类与重写
来源：http://mobile.bbcook.cn/Article/details/gaqgwxnnr.sHtML

class A: Base { override func f() {} }
来源：http://baike.sjlbkw.cn/Article/details/gsbvbdwrh.sHtML

[T27] Swift：错误处理
来源：http://3g.bbcook.cn/Article/details/gzujpwbrb.sHtML

do { try f() } catch { print(error) }
来源：http://baike.vehdjk.com/Article/details/gisjkupse.sHtML

[T28] Swift：枚举
来源：http://blog.sjlbkw.cn/Article/details/grsxlbwcw.sHtML

enum Color { case red, green }
来源：http://mobile.tarul.cn/Article/details/gftmclavo.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.tarul.cn/Article/details/gomktafke.sHtML

guard let x = opt else { return }
来源：http://www.m.share.bbcook.cn/Article/details/gkbafgjeq.sHtML

[T30] Swift：协议
来源：http://wap.epnwcf.com/Article/details/gfdbjxmgm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fktsv.cn/Article/details/gjbdopsrk.sHtML

[T31] Lua：Hello World
来源：http://wap.sjlbkw.cn/Article/details/ghvbxhxzf.sHtML

print("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gqhmhfjzx.sHtML

[T32] Lua：局部变量
来源：http://3g.yfazqb.com/Article/details/gcdgozfzn.sHtML

local a = 1
来源：http://3g.tarul.cn/Article/details/grbdgpsfx.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.vehdjk.com/Article/details/gklxvlntn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.tarul.cn/Article/details/gomwydjnq.sHtML

[T34] Lua：遍历表
来源：http://m.share.epnwcf.com/Article/details/gplyiuttc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.yfazqb.com/Article/details/gbwzyuaos.sHtML

[T35] Lua：字典表
来源：http://blog.tarul.cn/Article/details/gdrrkhyew.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fktsv.cn/Article/details/gdzadlesp.sHtML

[T36] Lua：函数
来源：http://wap.sjlbkw.cn/Article/details/googczqxt.sHtML

function add(a, b) return a + b end
来源：http://baike.tarul.cn/Article/details/gkydcjdkm.sHtML

[T37] Lua：字符串拼接
来源：http://wap.tarul.cn/Article/details/gsuhqazlh.sHtML

"a" .. "b"
来源：http://read.share.tarul.cn/Article/details/gbqqrisol.sHtML

[T38] Lua：条件
来源：http://www.share.tarul.cn/Article/details/gtgydnnyq.sHtML

if x > 0 then print("正") end
来源：http://blog.tarul.cn/Article/details/gtzgvkugm.sHtML

[T39] Lua：模式匹配
来源：http://mobile.vehdjk.com/Article/details/gpknyyevg.sHtML

string.find(s, "%d+")
来源：http://www.blog.fktsv.cn/Article/details/gylphkolx.sHtML

[T40] Lua：元表
来源：http://wap.vehdjk.com/Article/details/gvqdqqkvh.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.sjlbkw.cn/Article/details/gxhrqweff.sHtML

[T41] Perl：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gcvsggbuk.sHtML

print "Hello\n";
来源：http://www.m.share.sjlbkw.cn/Article/details/gaacojumk.sHtML

[T42] Perl：变量类型
来源：http://read.share.vehdjk.com/Article/details/gkqquqapg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.bbcook.cn/Article/details/giiuxiufr.sHtML

[T43] Perl：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gubzbimbt.sHtML

"值: $a"
来源：http://www.m.share.tarul.cn/Article/details/gunefyhkf.sHtML

[T44] Perl：条件
来源：http://m.share.vehdjk.com/Article/details/gclupwpsd.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.epnwcf.com/Article/details/gmwduysxd.sHtML

[T45] Perl：数组遍历
来源：http://blog.yfazqb.com/Article/details/guqlgskto.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.tarul.cn/Article/details/gqcyemdxl.sHtML

[T46] Perl：哈希操作
来源：http://3g.yfazqb.com/Article/details/gkaqqhwxb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.tarul.cn/Article/details/gghzspshh.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fktsv.cn/Article/details/gusaxdmmt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fktsv.cn/Article/details/gbfiivsir.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.yfazqb.com/Article/details/gycfggdcj.sHtML

$s =~ s/old/new/g;
来源：http://3g.vehdjk.com/Article/details/givomjyov.sHtML

[T49] Perl：函数
来源：http://wap.vehdjk.com/Article/details/gtwcvlxde.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gggamyncn.sHtML

[T50] Perl：逐行读文件
来源：http://wap.yfazqb.com/Article/details/glfqermcc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.epnwcf.com/Article/details/gfocthdqk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.vehdjk.com/Article/details/gpgdrjxxm.sHtML

[T51] Scala：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gahypayhc.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gaamzwpdk.sHtML

[T52] Scala：变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gdolmrcqb.sHtML

val a = 1;  var b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gxhjjiids.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gzagjlujt.sHtML

s"值: $b"
来源：http://mobile.sjlbkw.cn/Article/details/gnbsjqfyv.sHtML

[T54] Scala：集合映射
来源：http://www.blog.yfazqb.com/Article/details/gcmvekwup.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.yfazqb.com/Article/details/guncxparm.sHtML

[T55] Scala：集合过滤
来源：http://wap.fktsv.cn/Article/details/gbiutvxwm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.sjlbkw.cn/Article/details/gpkrtymvn.sHtML

[T56] Scala：样例类
来源：http://3g.epnwcf.com/Article/details/gnhwfcrzb.sHtML

case class User(name: String, age: Int)
来源：http://m.share.vehdjk.com/Article/details/guwmsogfb.sHtML

[T57] Scala：模式匹配
来源：http://www.share.epnwcf.com/Article/details/gimeeayyv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fktsv.cn/Article/details/gdhmxbayh.sHtML

[T58] Scala：函数定义
来源：http://m.share.fktsv.cn/Article/details/gstzltssb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fktsv.cn/Article/details/gnwdacuqu.sHtML

[T59] Scala：循环
来源：http://m.share.fktsv.cn/Article/details/gfgnztbic.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gqztbeyee.sHtML

[T60] Scala：折叠
来源：http://blog.yfazqb.com/Article/details/gbnwaoeqz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fktsv.cn/Article/details/giwvwwusx.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/grgaqkvlr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.tarul.cn/Article/details/gfmdecaae.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gjqxrqmkn.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.sjlbkw.cn/Article/details/ggbjgqpyb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fktsv.cn/Article/details/godatefrc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.sjlbkw.cn/Article/details/gvysbakhy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.yfazqb.com/Article/details/gbjkipqah.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.tarul.cn/Article/details/gqmxcgkno.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.sjlbkw.cn/Article/details/gpohqnwbm.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.tarul.cn/Article/details/gteiqgxvt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.vehdjk.com/Article/details/gjubvsljr.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.epnwcf.com/Article/details/greosyfjg.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.vehdjk.com/Article/details/gqkgsnlrq.sHtML

[U06] Py：合并两个字典
来源：http://mobile.tarul.cn/Article/details/gyocslnsp.sHtML

{**a, **b}
来源：http://www.blog.epnwcf.com/Article/details/gdkmxjobe.sHtML

[U07] Py：反转字典键值
来源：http://blog.bbcook.cn/Article/details/gbjbbcsdn.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.bbcook.cn/Article/details/gijrtzaqf.sHtML

[U08] Py：展平二维列表
来源：http://3g.bbcook.cn/Article/details/gqzpewmzb.sHtML

[y for x in nested for y in x]
来源：http://blog.tarul.cn/Article/details/gweeeieak.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.vehdjk.com/Article/details/gshqnvgxc.sHtML

max(d, key=d.get)
来源：http://3g.vehdjk.com/Article/details/gzwngpioi.sHtML

[U10] Py：按值排序字典
来源：http://baike.vehdjk.com/Article/details/gypatmcmw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.yfazqb.com/Article/details/gngjrhhvp.sHtML

[U11] Py：生成器表达式
来源：http://www.share.tarul.cn/Article/details/gnmkbotqp.sHtML

(x * 2 for x in arr)
来源：http://read.share.fktsv.cn/Article/details/gxcfdnimc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.vehdjk.com/Article/details/gzompitbo.sHtML

Counter(arr).most_common(3)
来源：http://m.share.bbcook.cn/Article/details/gxybohftc.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fktsv.cn/Article/details/gsnmrkysg.sHtML

deque(maxlen=10)
来源：http://baike.tarul.cn/Article/details/giglgnrtm.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.tarul.cn/Article/details/gfbzgrrgv.sHtML

defaultdict(list)
来源：http://wap.bbcook.cn/Article/details/ggfbeolpa.sHtML

[U15] Py：高精度计时
来源：http://blog.vehdjk.com/Article/details/gbmuuythp.sHtML

t = time.perf_counter()
来源：http://www.share.bbcook.cn/Article/details/gkisutbgp.sHtML

[U16] Py：命令行参数解析
来源：http://baike.tarul.cn/Article/details/ghsoseijw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.bbcook.cn/Article/details/gxcshhpim.sHtML

[U17] Py：初始化日志
来源：http://www.share.vehdjk.com/Article/details/gpsrbvifb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fktsv.cn/Article/details/gmppzlilu.sHtML

[U18] Py：预编译正则
来源：http://m.share.epnwcf.com/Article/details/gabugttrr.sHtML

pat = re.compile(r"\d+")
来源：http://blog.bbcook.cn/Article/details/gkhvewmns.sHtML

[U19] Py：正则替换带回调
来源：http://blog.tarul.cn/Article/details/gpivkwsyk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fktsv.cn/Article/details/gjfkoatuv.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.vehdjk.com/Article/details/gmsecsbzk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fktsv.cn/Article/details/gqgyhvueh.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.sjlbkw.cn/Article/details/gzfimpten.sHtML

@contextlib.contextmanager
来源：http://wap.vehdjk.com/Article/details/gzzfpoazp.sHtML

[U22] Py：矩阵转置
来源：http://www.share.tarul.cn/Article/details/gwgyganwm.sHtML

list(zip(*m))
来源：http://3g.bbcook.cn/Article/details/gkdbhdcql.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.epnwcf.com/Article/details/ggoriulaq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.epnwcf.com/Article/details/gwklogwsf.sHtML

[U24] Py：路径操作
来源：http://www.share.epnwcf.com/Article/details/gnizrzmrr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.vehdjk.com/Article/details/gibwbwpvj.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.vehdjk.com/Article/details/gebmuyabw.sHtML

csv.DictReader(f)
来源：http://3g.bbcook.cn/Article/details/gdqwtcevl.sHtML

[U26] Py：并发下载
来源：http://mobile.tarul.cn/Article/details/gegukxcmn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.yfazqb.com/Article/details/glzptsllk.sHtML

[U27] Py：异步 HTTP
来源：http://blog.bbcook.cn/Article/details/gzfysszby.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.bbcook.cn/Article/details/gyxgnipgz.sHtML

[U28] Py：类型别名
来源：http://read.share.fktsv.cn/Article/details/grzahkvob.sHtML

UserId = int
来源：http://read.share.fktsv.cn/Article/details/gsysilzdn.sHtML

[U29] Py：属性校验
来源：http://www.blog.bbcook.cn/Article/details/gcwqsxxmj.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.bbcook.cn/Article/details/gubtocpjn.sHtML

[U30] Py：数据类
来源：http://blog.fktsv.cn/Article/details/gceulmszm.sHtML

@dataclass(slots=True)
来源：http://wap.bbcook.cn/Article/details/ggvoeowqq.sHtML

[U31] Py：单测
来源：http://www.m.share.vehdjk.com/Article/details/goowfmpff.sHtML

python -m pytest -q
来源：http://mobile.epnwcf.com/Article/details/gaemrqpsu.sHtML

[U32] Py：代码格式化
来源：http://www.share.sjlbkw.cn/Article/details/guirfdupp.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.yfazqb.com/Article/details/gpsckrmgv.sHtML

[U33] Py：打包发布
来源：http://wap.sjlbkw.cn/Article/details/ghvykueyf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.vehdjk.com/Article/details/gdphnyixu.sHtML

[U34] Py：判断编码
来源：http://wap.tarul.cn/Article/details/gsdtssaus.sHtML

chardet.detect(raw)
来源：http://3g.fktsv.cn/Article/details/gstgrrzjf.sHtML

[U35] Py：发送邮件
来源：http://3g.yfazqb.com/Article/details/gwcqdrvec.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.sjlbkw.cn/Article/details/ghnzcajxc.sHtML

[U36] Py：定时任务
来源：http://read.share.bbcook.cn/Article/details/gsvsthbzq.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.vehdjk.com/Article/details/gblslrvxc.sHtML

[U37] Py：读写 Excel
来源：http://blog.vehdjk.com/Article/details/gwcbrzaqo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fktsv.cn/Article/details/ghvvomrst.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.epnwcf.com/Article/details/gcizblrpy.sHtML

Path(__file__).resolve().parent
来源：http://read.share.sjlbkw.cn/Article/details/gswpfcoqa.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fktsv.cn/Article/details/goisngfcm.sHtML

sys.stdout.isatty()
来源：http://www.m.share.tarul.cn/Article/details/gfknuhsst.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.yfazqb.com/Article/details/ghnsbdodl.sHtML

print("err", file=sys.stderr)
来源：http://www.share.bbcook.cn/Article/details/gifgvqozc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.epnwcf.com/Article/details/giabsaoef.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfukckyg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.bbcook.cn/Article/details/gstufrypw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.bbcook.cn/Article/details/gukbvkdib.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.bbcook.cn/Article/details/gejemldvb.sHtML

namespace App\Http;
来源：http://3g.sjlbkw.cn/Article/details/grjaekdhn.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.yfazqb.com/Article/details/ggzqcpevd.sHtML

declare(strict_types=1);
来源：http://wap.fktsv.cn/Article/details/gnpnupdec.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fktsv.cn/Article/details/gqgkxacvx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gizsrphvf.sHtML

[U46] PHP：可空类型
来源：http://baike.bbcook.cn/Article/details/gmjacnlbw.sHtML

?string $name = null
来源：http://m.share.bbcook.cn/Article/details/groadsfid.sHtML

[U47] PHP：联合类型
来源：http://blog.fktsv.cn/Article/details/gzhbwikbu.sHtML

int|string $id
来源：http://www.m.share.tarul.cn/Article/details/gxnpctzun.sHtML

[U48] PHP：纯枚举
来源：http://blog.tarul.cn/Article/details/gllfamdey.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.yfazqb.com/Article/details/gztwaaamg.sHtML

[U49] PHP：只读属性
来源：http://www.share.bbcook.cn/Article/details/gdhxqpgfe.sHtML

public readonly string $name
来源：http://wap.yfazqb.com/Article/details/geyivuazx.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.vehdjk.com/Article/details/gchsfrsbi.sHtML

public function __construct(private int $id) {}
来源：http://3g.yfazqb.com/Article/details/geubjjvmg.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.bbcook.cn/Article/details/gwtplgrqs.sHtML

[$a, $b] = $arr;
来源：http://www.blog.yfazqb.com/Article/details/gbtoiqrlz.sHtML

[U52] PHP：箭头函数
来源：http://read.share.tarul.cn/Article/details/gkrjlibay.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.vehdjk.com/Article/details/grinrahpz.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.yfazqb.com/Article/details/gfxpvyjah.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.tarul.cn/Article/details/gvsrbsmvj.sHtML

[U54] PHP：空安全调用
来源：http://www.share.bbcook.cn/Article/details/gvaltogku.sHtML

$obj?->method()
来源：http://baike.fktsv.cn/Article/details/ggoowtpws.sHtML

[U55] PHP：match 表达式
来源：http://3g.epnwcf.com/Article/details/gpudcbqfb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.vehdjk.com/Article/details/gzqdwjinr.sHtML

[U56] PHP：命名参数
来源：http://read.share.vehdjk.com/Article/details/gkkhtuctp.sHtML

f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gcizvrsss.sHtML

[U57] PHP：字符串插值
来源：http://3g.epnwcf.com/Article/details/gqzaenatq.sHtML

"值: {$a}"
来源：http://m.share.fktsv.cn/Article/details/gypedwedy.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fktsv.cn/Article/details/gtralwndc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.yfazqb.com/Article/details/ghhcavslt.sHtML

[U59] PHP：自定义排序
来源：http://read.share.bbcook.cn/Article/details/ggroihzcb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.tarul.cn/Article/details/ghlyoosjr.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.sjlbkw.cn/Article/details/govnhhzvw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.yfazqb.com/Article/details/gxghnovri.sHtML

[U61] PHP：正则
来源：http://baike.epnwcf.com/Article/details/gqryqnjrm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.yfazqb.com/Article/details/gkyaedvkd.sHtML

[U62] PHP：日期对象
来源：http://mobile.yfazqb.com/Article/details/gdmjqhvck.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.tarul.cn/Article/details/gqcekppxz.sHtML

[U63] PHP：文件读写
来源：http://mobile.tarul.cn/Article/details/gkwnnqiqg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.sjlbkw.cn/Article/details/gruyfdcce.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.epnwcf.com/Article/details/gdacghalh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.sjlbkw.cn/Article/details/gulsaqyda.sHtML


<!-- 参考信息 -->