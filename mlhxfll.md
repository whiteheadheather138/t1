代发 wailian999

[S43] C++：智能指针
来源：http://m.share.vehdjk.com/Article/details/gxqpkfrvz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fktsv.cn/Article/details/gvhzyvfgh.sHtML

[S44] C++：引用传参
来源：http://wap.fktsv.cn/Article/details/gyaphuapw.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.vehdjk.com/Article/details/gbitygxxp.sHtML

[S45] C++：lambda
来源：http://wap.fktsv.cn/Article/details/gpsgwycot.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fktsv.cn/Article/details/gpshzzskt.sHtML

[S46] C++：函数模板
来源：http://www.share.epnwcf.com/Article/details/gdiwultxg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.tarul.cn/Article/details/geastlllp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.tarul.cn/Article/details/gvlisyffe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.yfazqb.com/Article/details/gekgoyakl.sHtML

[S48] C++：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gknknmbdn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.yfazqb.com/Article/details/gbxiovvfw.sHtML

while (std::getline(in, line)) { }
来源：http://blog.epnwcf.com/Article/details/greycivxr.sHtML

[S49] C++：写文件
来源：http://m.share.sjlbkw.cn/Article/details/gvqctldyc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.yfazqb.com/Article/details/gclnsmnxw.sHtML

[S50] C++：格式化数字
来源：http://read.share.sjlbkw.cn/Article/details/glphwefbo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gcnpdckiq.sHtML

[S51] C++：显式类型转换
来源：http://mobile.bbcook.cn/Article/details/gwhyjnsfp.sHtML

static_cast<double>(a) / b
来源：http://m.share.tarul.cn/Article/details/gzguzoxkz.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.vehdjk.com/Article/details/ggvmzzerv.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.sjlbkw.cn/Article/details/gxgdhcmsl.sHtML

[S53] C++：移动语义
来源：http://www.share.sjlbkw.cn/Article/details/gcnoaewhu.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.epnwcf.com/Article/details/gcpymvaog.sHtML

[S54] C++：异常处理
来源：http://3g.bbcook.cn/Article/details/ggindlgkf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.tarul.cn/Article/details/gutdvfvzl.sHtML

[S55] C++：结构化绑定
来源：http://baike.tarul.cn/Article/details/glbuhwgzj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.sjlbkw.cn/Article/details/gpyjjpqfm.sHtML

[S56] C++：optional
来源：http://www.blog.tarul.cn/Article/details/gfveirirv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.epnwcf.com/Article/details/ghsvinwal.sHtML

[S57] C++：编译期常量
来源：http://www.share.tarul.cn/Article/details/gowghtyml.sHtML

constexpr int N = 10;
来源：http://3g.vehdjk.com/Article/details/gvtcrhvsg.sHtML

[S58] C++：命名空间
来源：http://www.share.sjlbkw.cn/Article/details/gpbxqbbgv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.epnwcf.com/Article/details/gyqzbgpnh.sHtML

[S59] C++：静态断言
来源：http://wap.epnwcf.com/Article/details/gvklshwlr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fktsv.cn/Article/details/givcbjjcd.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.epnwcf.com/Article/details/gwsobazot.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fktsv.cn/Article/details/gvrnsdlml.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ghrmbdivj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.tarul.cn/Article/details/ghrezwfae.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gpazceovm.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fktsv.cn/Article/details/gdsrzzobg.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/grexturog.sHtML

[T02] Kotlin：变量
来源：http://read.share.yfazqb.com/Article/details/gvvqycblq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.sjlbkw.cn/Article/details/gfzqiwsjt.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.sjlbkw.cn/Article/details/gwjmtdtsc.sHtML

"值: $b"
来源：http://www.share.yfazqb.com/Article/details/gnbrwtwlw.sHtML

[T04] Kotlin：空安全
来源：http://baike.sjlbkw.cn/Article/details/gyqjregfh.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.bbcook.cn/Article/details/gifcwuwwn.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.sjlbkw.cn/Article/details/gdkivvfne.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fktsv.cn/Article/details/gonchxejs.sHtML

[T06] Kotlin：集合映射
来源：http://3g.sjlbkw.cn/Article/details/gxsuyohmr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gdzspskrj.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fktsv.cn/Article/details/gzrkioeqf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.yfazqb.com/Article/details/gzcnxflzf.sHtML

[T08] Kotlin：数据类
来源：http://wap.sjlbkw.cn/Article/details/gtulykmxd.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.sjlbkw.cn/Article/details/gbbhxqbzc.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.sjlbkw.cn/Article/details/gvapxbptj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.tarul.cn/Article/details/gybfhvjgb.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.epnwcf.com/Article/details/gbbyjwgec.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.bbcook.cn/Article/details/gwzqqexbm.sHtML

[T11] Kotlin：协程
来源：http://read.share.yfazqb.com/Article/details/gwezauwcl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.tarul.cn/Article/details/gcsehfdrf.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmoxckfu.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.yfazqb.com/Article/details/gdmpueqbi.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.epnwcf.com/Article/details/gskztbbdt.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.yfazqb.com/Article/details/geikumcfi.sHtML

[T14] Kotlin：循环
来源：http://read.share.fktsv.cn/Article/details/gcpovhnyr.sHtML

for (i in 1..10) println(i)
来源：http://wap.sjlbkw.cn/Article/details/gkiacxpcj.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fktsv.cn/Article/details/gvmbydapd.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.sjlbkw.cn/Article/details/gdtpqarxj.sHtML

[T16] Swift：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gxcpvpskk.sHtML

print("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gauasfnii.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.tarul.cn/Article/details/gfjonfejf.sHtML

var a = 1;  let b = 2
来源：http://m.share.bbcook.cn/Article/details/gnwzanhyi.sHtML

[T18] Swift：字符串插值
来源：http://m.share.vehdjk.com/Article/details/gmtkvleed.sHtML

"值: \(b)"
来源：http://wap.fktsv.cn/Article/details/gumqktmsa.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fktsv.cn/Article/details/gcqdzohzf.sHtML

if let n = opt { print(n) }
来源：http://3g.bbcook.cn/Article/details/gukapayhw.sHtML

[T20] Swift：数组操作
来源：http://wap.epnwcf.com/Article/details/gdykdktyl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.yfazqb.com/Article/details/gaoorfomy.sHtML

[T21] Swift：遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhykisks.sHtML

for x in a { print(x) }
来源：http://wap.epnwcf.com/Article/details/gmvjhzwzf.sHtML

[T22] Swift：字典
来源：http://3g.epnwcf.com/Article/details/grubutoqj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.bbcook.cn/Article/details/gstvtwlou.sHtML

[T23] Swift：函数
来源：http://blog.yfazqb.com/Article/details/gcqamyqom.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gyumnykyn.sHtML

[T24] Swift：闭包
来源：http://www.share.tarul.cn/Article/details/gfhubxhdz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.tarul.cn/Article/details/gksmwyzou.sHtML

[T25] Swift：结构体
来源：http://read.share.tarul.cn/Article/details/gbljapphf.sHtML

struct P { var x: Int }
来源：http://blog.tarul.cn/Article/details/gwujexrjv.sHtML

[T26] Swift：类与重写
来源：http://mobile.fktsv.cn/Article/details/gtzqohsoq.sHtML

class A: Base { override func f() {} }
来源：http://baike.tarul.cn/Article/details/gqluwdbdr.sHtML

[T27] Swift：错误处理
来源：http://blog.epnwcf.com/Article/details/ghervnlqg.sHtML

do { try f() } catch { print(error) }
来源：http://blog.yfazqb.com/Article/details/ghipgnhhw.sHtML

[T28] Swift：枚举
来源：http://wap.vehdjk.com/Article/details/gfskuwzci.sHtML

enum Color { case red, green }
来源：http://blog.sjlbkw.cn/Article/details/gyeznfxch.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.epnwcf.com/Article/details/gdnzhacjq.sHtML

guard let x = opt else { return }
来源：http://baike.fktsv.cn/Article/details/grtshjgih.sHtML

[T30] Swift：协议
来源：http://read.share.epnwcf.com/Article/details/gsuzwgtdo.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.bbcook.cn/Article/details/gqeyntfrd.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gcnbnilcn.sHtML

print("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/guaogngua.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.tarul.cn/Article/details/gbkduxfkq.sHtML

local a = 1
来源：http://baike.epnwcf.com/Article/details/gydwxzsmq.sHtML

[T33] Lua：表（数组）
来源：http://wap.yfazqb.com/Article/details/gnzsijoxh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.yfazqb.com/Article/details/guyhopffe.sHtML

[T34] Lua：遍历表
来源：http://m.share.sjlbkw.cn/Article/details/gqauzykvz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.tarul.cn/Article/details/gonkddopy.sHtML

[T35] Lua：字典表
来源：http://m.share.vehdjk.com/Article/details/gmwkpjsaz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.sjlbkw.cn/Article/details/ggvgqrkqb.sHtML

[T36] Lua：函数
来源：http://www.share.fktsv.cn/Article/details/goljttngd.sHtML

function add(a, b) return a + b end
来源：http://mobile.bbcook.cn/Article/details/gugresefv.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.sjlbkw.cn/Article/details/gecuceuno.sHtML

"a" .. "b"
来源：http://baike.tarul.cn/Article/details/gpbeeiyhy.sHtML

[T38] Lua：条件
来源：http://mobile.fktsv.cn/Article/details/giiuxjsjb.sHtML

if x > 0 then print("正") end
来源：http://read.share.yfazqb.com/Article/details/gphdxvlgg.sHtML

[T39] Lua：模式匹配
来源：http://m.share.bbcook.cn/Article/details/geytflwka.sHtML

string.find(s, "%d+")
来源：http://baike.yfazqb.com/Article/details/giqjjnufv.sHtML

[T40] Lua：元表
来源：http://www.m.share.sjlbkw.cn/Article/details/gpswyzcqm.sHtML

setmetatable({}, { __index = base })
来源：http://blog.tarul.cn/Article/details/gugboerry.sHtML

[T41] Perl：Hello World
来源：http://wap.fktsv.cn/Article/details/gnvacspbm.sHtML

print "Hello\n";
来源：http://www.blog.tarul.cn/Article/details/gkseoojcl.sHtML

[T42] Perl：变量类型
来源：http://www.share.vehdjk.com/Article/details/ggquorfka.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.sjlbkw.cn/Article/details/gkfhkklzi.sHtML

[T43] Perl：字符串插值
来源：http://baike.tarul.cn/Article/details/gmbwnpshf.sHtML

"值: $a"
来源：http://read.share.fktsv.cn/Article/details/grrnsyqie.sHtML

[T44] Perl：条件
来源：http://baike.fktsv.cn/Article/details/gvevvsmyw.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.tarul.cn/Article/details/gsvfwyczv.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fktsv.cn/Article/details/gvbgavofa.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.sjlbkw.cn/Article/details/gsfzmcucf.sHtML

[T46] Perl：哈希操作
来源：http://mobile.vehdjk.com/Article/details/gjixrmjxn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.tarul.cn/Article/details/gozxbqmqz.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fktsv.cn/Article/details/gtmdhcday.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.epnwcf.com/Article/details/ghjzbghkj.sHtML

[T48] Perl：正则替换
来源：http://blog.tarul.cn/Article/details/gnvftoyco.sHtML

$s =~ s/old/new/g;
来源：http://blog.tarul.cn/Article/details/glirlbtuy.sHtML

[T49] Perl：函数
来源：http://www.share.fktsv.cn/Article/details/gvfsiajdf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gbetcnjql.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/guzuoquvi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.epnwcf.com/Article/details/griemxcvs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.yfazqb.com/Article/details/gsnfvpmrd.sHtML

[T51] Scala：Hello World
来源：http://m.share.epnwcf.com/Article/details/gkngyatwp.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/ghtevpmow.sHtML

[T52] Scala：变量
来源：http://www.blog.vehdjk.com/Article/details/gdtepzuha.sHtML

val a = 1;  var b = 2
来源：http://mobile.epnwcf.com/Article/details/gstchcelt.sHtML

[T53] Scala：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gonphuupd.sHtML

s"值: $b"
来源：http://mobile.sjlbkw.cn/Article/details/gajcctlnr.sHtML

[T54] Scala：集合映射
来源：http://baike.vehdjk.com/Article/details/gvihgronh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.epnwcf.com/Article/details/gkyefoiga.sHtML

[T55] Scala：集合过滤
来源：http://3g.yfazqb.com/Article/details/gdmqxkcpg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.yfazqb.com/Article/details/gdrmatwob.sHtML

[T56] Scala：样例类
来源：http://3g.sjlbkw.cn/Article/details/geaoxujco.sHtML

case class User(name: String, age: Int)
来源：http://blog.vehdjk.com/Article/details/gietrbfrr.sHtML

[T57] Scala：模式匹配
来源：http://mobile.tarul.cn/Article/details/gtijzfphh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fktsv.cn/Article/details/ghdoomkee.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.yfazqb.com/Article/details/gswffdfrq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.tarul.cn/Article/details/gjozabpfa.sHtML

[T59] Scala：循环
来源：http://read.share.vehdjk.com/Article/details/grobwepyr.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.yfazqb.com/Article/details/gmafvcirj.sHtML

[T60] Scala：折叠
来源：http://baike.bbcook.cn/Article/details/gwggdjxfr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.sjlbkw.cn/Article/details/gtmtiwzdw.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gjtvbeful.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.epnwcf.com/Article/details/gmsgoekkg.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gfmgmmsue.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.vehdjk.com/Article/details/gdbavkzbk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.tarul.cn/Article/details/gdvfvnogc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.vehdjk.com/Article/details/gpdelnrkd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.bbcook.cn/Article/details/ghyjaxzso.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.bbcook.cn/Article/details/gdzmyjvdm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fktsv.cn/Article/details/gzroqclzq.sHtML

[U04] Py：变量调试打印
来源：http://read.share.sjlbkw.cn/Article/details/gscmdfktr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.bbcook.cn/Article/details/gtjcujkwv.sHtML

[U05] Py：列表去重且保序
来源：http://baike.yfazqb.com/Article/details/gijtfmcsc.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.epnwcf.com/Article/details/guxfzfmdd.sHtML

[U06] Py：合并两个字典
来源：http://wap.fktsv.cn/Article/details/gofxtsbfc.sHtML

{**a, **b}
来源：http://www.share.bbcook.cn/Article/details/gaufwapag.sHtML

[U07] Py：反转字典键值
来源：http://wap.vehdjk.com/Article/details/gviysgfat.sHtML

{v: k for k, v in d.items()}
来源：http://wap.epnwcf.com/Article/details/ggwkgktvk.sHtML

[U08] Py：展平二维列表
来源：http://wap.tarul.cn/Article/details/gjvdtvlxq.sHtML

[y for x in nested for y in x]
来源：http://baike.fktsv.cn/Article/details/grwroqqpi.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.sjlbkw.cn/Article/details/ginzmgicw.sHtML

max(d, key=d.get)
来源：http://baike.yfazqb.com/Article/details/gjaurkkyc.sHtML

[U10] Py：按值排序字典
来源：http://www.share.bbcook.cn/Article/details/gwfijuozp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.vehdjk.com/Article/details/gucqzadjb.sHtML

[U11] Py：生成器表达式
来源：http://3g.bbcook.cn/Article/details/gunhidnwx.sHtML

(x * 2 for x in arr)
来源：http://www.share.fktsv.cn/Article/details/gmkykjbuh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.tarul.cn/Article/details/gtkoruazj.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.bbcook.cn/Article/details/glohfxivh.sHtML

[U13] Py：固定长度队列
来源：http://3g.yfazqb.com/Article/details/gkwdicgrz.sHtML

deque(maxlen=10)
来源：http://blog.yfazqb.com/Article/details/gtlnqbswp.sHtML

[U14] Py：分组收集到列表
来源：http://3g.epnwcf.com/Article/details/gahytkxlk.sHtML

defaultdict(list)
来源：http://m.share.fktsv.cn/Article/details/giwcfjlta.sHtML

[U15] Py：高精度计时
来源：http://www.share.bbcook.cn/Article/details/glgpafckf.sHtML

t = time.perf_counter()
来源：http://read.share.bbcook.cn/Article/details/gedgjissr.sHtML

[U16] Py：命令行参数解析
来源：http://baike.bbcook.cn/Article/details/gxqktroyo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fktsv.cn/Article/details/gaadagfjq.sHtML

[U17] Py：初始化日志
来源：http://baike.sjlbkw.cn/Article/details/grlfvrvlh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.yfazqb.com/Article/details/gsszdkpgl.sHtML

[U18] Py：预编译正则
来源：http://www.blog.vehdjk.com/Article/details/glniecpxm.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fktsv.cn/Article/details/gcvietfgb.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.epnwcf.com/Article/details/gqtutinpk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fktsv.cn/Article/details/gxqywfzeh.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fktsv.cn/Article/details/geayhdflo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.yfazqb.com/Article/details/gtszisfsm.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.tarul.cn/Article/details/gixsifezs.sHtML

@contextlib.contextmanager
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpyivcfh.sHtML

[U22] Py：矩阵转置
来源：http://mobile.bbcook.cn/Article/details/gbuzcdehp.sHtML

list(zip(*m))
来源：http://3g.vehdjk.com/Article/details/gxqtqsfce.sHtML

[U23] Py：分块读取大文件
来源：http://blog.sjlbkw.cn/Article/details/gqgokttqk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtnrldck.sHtML

[U24] Py：路径操作
来源：http://mobile.tarul.cn/Article/details/gtcgwfgyj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.tarul.cn/Article/details/gzqatizji.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.vehdjk.com/Article/details/ghdfrmebt.sHtML

csv.DictReader(f)
来源：http://www.m.share.yfazqb.com/Article/details/gljmmxsls.sHtML

[U26] Py：并发下载
来源：http://read.share.fktsv.cn/Article/details/gfhvkzkqf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.bbcook.cn/Article/details/gbracigpj.sHtML

[U27] Py：异步 HTTP
来源：http://3g.bbcook.cn/Article/details/gftizrhoy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.tarul.cn/Article/details/gramcuqwt.sHtML

[U28] Py：类型别名
来源：http://3g.yfazqb.com/Article/details/gtskxwbll.sHtML

UserId = int
来源：http://3g.fktsv.cn/Article/details/gvdnvupcz.sHtML

[U29] Py：属性校验
来源：http://blog.sjlbkw.cn/Article/details/gtvvsynff.sHtML

@property 与 @x.setter 配合
来源：http://wap.sjlbkw.cn/Article/details/glqqvryry.sHtML

[U30] Py：数据类
来源：http://read.share.tarul.cn/Article/details/gfqeqepmn.sHtML

@dataclass(slots=True)
来源：http://read.share.tarul.cn/Article/details/grmlvmpdw.sHtML

[U31] Py：单测
来源：http://3g.bbcook.cn/Article/details/gymdktjnr.sHtML

python -m pytest -q
来源：http://read.share.tarul.cn/Article/details/gxntruhvm.sHtML

[U32] Py：代码格式化
来源：http://wap.epnwcf.com/Article/details/gxnjkfalk.sHtML

ruff format . && ruff check --fix .
来源：http://wap.vehdjk.com/Article/details/gfslhsvpd.sHtML

[U33] Py：打包发布
来源：http://blog.bbcook.cn/Article/details/gicllyqka.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.tarul.cn/Article/details/gitaeczzx.sHtML

[U34] Py：判断编码
来源：http://www.share.fktsv.cn/Article/details/gupyllimj.sHtML

chardet.detect(raw)
来源：http://wap.fktsv.cn/Article/details/gmwqgjnyr.sHtML

[U35] Py：发送邮件
来源：http://wap.bbcook.cn/Article/details/giuclnpnr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.sjlbkw.cn/Article/details/gveubiddd.sHtML

[U36] Py：定时任务
来源：http://www.share.sjlbkw.cn/Article/details/gwpitluab.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.bbcook.cn/Article/details/gazrjgilt.sHtML

[U37] Py：读写 Excel
来源：http://m.share.bbcook.cn/Article/details/gbvlmswds.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.epnwcf.com/Article/details/gpjslaezl.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.epnwcf.com/Article/details/gvvfhsqav.sHtML

Path(__file__).resolve().parent
来源：http://blog.yfazqb.com/Article/details/gzorhmxzi.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.sjlbkw.cn/Article/details/gmmlanxkk.sHtML

sys.stdout.isatty()
来源：http://3g.tarul.cn/Article/details/gizfyetnd.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.tarul.cn/Article/details/gpisaaoom.sHtML

print("err", file=sys.stderr)
来源：http://baike.sjlbkw.cn/Article/details/glhvfqngb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.sjlbkw.cn/Article/details/gkeedoeog.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.tarul.cn/Article/details/gpfqzwwos.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.epnwcf.com/Article/details/grilyybse.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.bbcook.cn/Article/details/guvfbhxul.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.tarul.cn/Article/details/gsbgqcuik.sHtML

namespace App\Http;
来源：http://www.blog.yfazqb.com/Article/details/gscdzduni.sHtML

[U44] PHP：开启严格类型
来源：http://baike.tarul.cn/Article/details/givxqvvap.sHtML

declare(strict_types=1);
来源：http://www.share.sjlbkw.cn/Article/details/gujxqnqqu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.sjlbkw.cn/Article/details/ghuwbvifi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/gopbozwfz.sHtML

[U46] PHP：可空类型
来源：http://3g.epnwcf.com/Article/details/gvocebtdk.sHtML

?string $name = null
来源：http://mobile.bbcook.cn/Article/details/ghtijlgiz.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fktsv.cn/Article/details/gdacvmngy.sHtML

int|string $id
来源：http://www.m.share.fktsv.cn/Article/details/gvjmmdpdv.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fktsv.cn/Article/details/gcslxhxcm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.epnwcf.com/Article/details/gxvuybbwu.sHtML

[U49] PHP：只读属性
来源：http://mobile.yfazqb.com/Article/details/gjaqvxqae.sHtML

public readonly string $name
来源：http://mobile.fktsv.cn/Article/details/gtdhjbisu.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.bbcook.cn/Article/details/gfxmtkztt.sHtML

public function __construct(private int $id) {}
来源：http://mobile.epnwcf.com/Article/details/gdyrzicws.sHtML

[U51] PHP：数组解构
来源：http://www.share.fktsv.cn/Article/details/gvaxlypjv.sHtML

[$a, $b] = $arr;
来源：http://3g.epnwcf.com/Article/details/gyfrjjdxo.sHtML

[U52] PHP：箭头函数
来源：http://mobile.sjlbkw.cn/Article/details/gogdywfky.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.vehdjk.com/Article/details/gywgberdm.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fktsv.cn/Article/details/gqhudxsxm.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.yfazqb.com/Article/details/gjhsycqpx.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.tarul.cn/Article/details/gcybajtcc.sHtML

$obj?->method()
来源：http://blog.tarul.cn/Article/details/goxjyeukb.sHtML

[U55] PHP：match 表达式
来源：http://www.share.bbcook.cn/Article/details/gebgtbyrw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.yfazqb.com/Article/details/gvgvkwyow.sHtML

[U56] PHP：命名参数
来源：http://mobile.yfazqb.com/Article/details/ghhxoyhtf.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.yfazqb.com/Article/details/gsfrwyzam.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gxapzdfmu.sHtML

"值: {$a}"
来源：http://blog.bbcook.cn/Article/details/gockkuyjb.sHtML

[U58] PHP：数组三件套
来源：http://baike.yfazqb.com/Article/details/gtkkpllxn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.sjlbkw.cn/Article/details/gwhmjtpwx.sHtML

[U59] PHP：自定义排序
来源：http://baike.fktsv.cn/Article/details/graumcdjt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.epnwcf.com/Article/details/geshzfkyw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fktsv.cn/Article/details/gceqszcoz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.yfazqb.com/Article/details/gyopzeggp.sHtML

[U61] PHP：正则
来源：http://www.blog.epnwcf.com/Article/details/gfhifxbal.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.vehdjk.com/Article/details/gcgblphmm.sHtML

[U62] PHP：日期对象
来源：http://baike.tarul.cn/Article/details/ghmbshqmf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.vehdjk.com/Article/details/gasfsxjje.sHtML

[U63] PHP：文件读写
来源：http://read.share.sjlbkw.cn/Article/details/gltinaejl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.yfazqb.com/Article/details/grzmgqbvw.sHtML

[U64] PHP：目录遍历
来源：http://baike.epnwcf.com/Article/details/gzxwytoxo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.yfazqb.com/Article/details/gbdwihofa.sHtML

[U65] PHP：会话
来源：http://m.share.yfazqb.com/Article/details/ggucxfgvv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gmdkmzdto.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.epnwcf.com/Article/details/gsldunrda.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.sjlbkw.cn/Article/details/gerbsxktu.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.epnwcf.com/Article/details/gracsatqo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.vehdjk.com/Article/details/gcsldljav.sHtML

[U68] PHP：PDO 连接
来源：http://blog.yfazqb.com/Article/details/ggetpiwhv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.epnwcf.com/Article/details/gkizjrhiz.sHtML


<!-- 参考信息 -->