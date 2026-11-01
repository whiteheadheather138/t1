代发 wailian999

[S33] C++：vector 增删
来源：http://blog.epnwcf.com/Article/details/ghqecrexg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fktsv.cn/Article/details/gxmoqqopa.sHtML

[S34] C++：遍历 vector
来源：http://read.share.yfazqb.com/Article/details/grjjqbggm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.tarul.cn/Article/details/gwzopnndm.sHtML

[S35] C++：map
来源：http://blog.yfazqb.com/Article/details/gqzdjqdma.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.vehdjk.com/Article/details/gvncgblsk.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.yfazqb.com/Article/details/guqnkcbxg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gtgligrkh.sHtML

[S37] C++：set
来源：http://m.share.epnwcf.com/Article/details/gfqwmquke.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.bbcook.cn/Article/details/gobuqgtzl.sHtML

[S38] C++：排序
来源：http://baike.epnwcf.com/Article/details/gdirbjpjc.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.sjlbkw.cn/Article/details/geqoccode.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.sjlbkw.cn/Article/details/gifetleue.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.vehdjk.com/Article/details/gluyxacsy.sHtML

[S40] C++：查找元素
来源：http://baike.epnwcf.com/Article/details/gutkfsubs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.vehdjk.com/Article/details/godinesgi.sHtML

[S41] C++：类与构造函数
来源：http://www.share.tarul.cn/Article/details/giafoppnd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.epnwcf.com/Article/details/gkkazkird.sHtML

[S42] C++：继承与虚函数
来源：http://wap.yfazqb.com/Article/details/gmxankqdz.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.sjlbkw.cn/Article/details/gpmrmxbnn.sHtML

[S43] C++：智能指针
来源：http://baike.fktsv.cn/Article/details/gowoqymbb.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.yfazqb.com/Article/details/gtdpmnouh.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fktsv.cn/Article/details/geoghiqbb.sHtML

void inc(int &x) { ++x; }
来源：http://blog.yfazqb.com/Article/details/gycwsrurg.sHtML

[S45] C++：lambda
来源：http://wap.vehdjk.com/Article/details/gvpmoazig.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.epnwcf.com/Article/details/ggvquyzzn.sHtML

[S46] C++：函数模板
来源：http://www.m.share.vehdjk.com/Article/details/gvthdvfvp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.epnwcf.com/Article/details/gacbpnzzo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.tarul.cn/Article/details/gkrlxeggg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.bbcook.cn/Article/details/gpixdbtzr.sHtML

[S48] C++：逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gtwnapyvq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fktsv.cn/Article/details/gukjtiyqq.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fktsv.cn/Article/details/gomxzhqis.sHtML

[S49] C++：写文件
来源：http://3g.epnwcf.com/Article/details/garxidayp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.yfazqb.com/Article/details/gvdsvzjhi.sHtML

[S50] C++：格式化数字
来源：http://baike.fktsv.cn/Article/details/gutfiyfko.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gygckdger.sHtML

[S51] C++：显式类型转换
来源：http://mobile.tarul.cn/Article/details/gglnucpui.sHtML

static_cast<double>(a) / b
来源：http://www.blog.tarul.cn/Article/details/gokrnvfmy.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.vehdjk.com/Article/details/gjxaqepui.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fktsv.cn/Article/details/gkgpmkijg.sHtML

[S53] C++：移动语义
来源：http://wap.epnwcf.com/Article/details/gsarqljey.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.bbcook.cn/Article/details/gpgokbokk.sHtML

[S54] C++：异常处理
来源：http://mobile.sjlbkw.cn/Article/details/gztdyadrb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.tarul.cn/Article/details/grgjzfdok.sHtML

[S55] C++：结构化绑定
来源：http://baike.bbcook.cn/Article/details/gmpwlfugr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.yfazqb.com/Article/details/gmmxjwgcg.sHtML

[S56] C++：optional
来源：http://mobile.vehdjk.com/Article/details/gjtuyczhz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fktsv.cn/Article/details/gpzeiohnw.sHtML

[S57] C++：编译期常量
来源：http://baike.yfazqb.com/Article/details/glnioxdrw.sHtML

constexpr int N = 10;
来源：http://wap.epnwcf.com/Article/details/gcqeteswi.sHtML

[S58] C++：命名空间
来源：http://blog.sjlbkw.cn/Article/details/gtwnlvcsl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.epnwcf.com/Article/details/gmxkrbkco.sHtML

[S59] C++：静态断言
来源：http://wap.fktsv.cn/Article/details/geofstebe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.yfazqb.com/Article/details/gtvncnyjg.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.sjlbkw.cn/Article/details/goijveeuk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.tarul.cn/Article/details/gzmhqtlls.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gqsqpukqd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.bbcook.cn/Article/details/gipqjgpnx.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/giycmrkei.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gzxhldldi.sHtML

println("Hello")
来源：http://m.share.yfazqb.com/Article/details/gontsyjoj.sHtML

[T02] Kotlin：变量
来源：http://m.share.fktsv.cn/Article/details/gheipcxmk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.tarul.cn/Article/details/glrunysuj.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.bbcook.cn/Article/details/ghwryibop.sHtML

"值: $b"
来源：http://read.share.epnwcf.com/Article/details/ghwjnmfit.sHtML

[T04] Kotlin：空安全
来源：http://m.share.sjlbkw.cn/Article/details/ghrnbngpz.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.bbcook.cn/Article/details/gpysegtcw.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fktsv.cn/Article/details/gcaxvofiv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.sjlbkw.cn/Article/details/gizmbueop.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.sjlbkw.cn/Article/details/gzppfglgk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fktsv.cn/Article/details/gjzqvxoav.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.tarul.cn/Article/details/ggwuhxniy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.vehdjk.com/Article/details/gqsxdlyla.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.tarul.cn/Article/details/gjcczaplk.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.bbcook.cn/Article/details/grosqcswl.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.sjlbkw.cn/Article/details/gfmdgietw.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.tarul.cn/Article/details/gxdaydkgs.sHtML

[T10] Kotlin：默认参数
来源：http://wap.epnwcf.com/Article/details/gxzhircpn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.epnwcf.com/Article/details/gsibgxlal.sHtML

[T11] Kotlin：协程
来源：http://blog.epnwcf.com/Article/details/grtlqbcfv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.yfazqb.com/Article/details/gifhlzzkp.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.vehdjk.com/Article/details/gylyqfmkn.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.epnwcf.com/Article/details/gaiulqwel.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.bbcook.cn/Article/details/ggfphaory.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fktsv.cn/Article/details/gcndniolw.sHtML

[T14] Kotlin：循环
来源：http://www.blog.yfazqb.com/Article/details/gpjzmlnyd.sHtML

for (i in 1..10) println(i)
来源：http://m.share.sjlbkw.cn/Article/details/gqbfncunv.sHtML

[T15] Kotlin：接口
来源：http://wap.tarul.cn/Article/details/gstajxgct.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.bbcook.cn/Article/details/gzakfihhl.sHtML

[T16] Swift：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gogdirxro.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/gwygevqom.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.bbcook.cn/Article/details/gwtcgoocp.sHtML

var a = 1;  let b = 2
来源：http://mobile.bbcook.cn/Article/details/gzkmvmzcz.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fktsv.cn/Article/details/ginwhfsqs.sHtML

"值: \(b)"
来源：http://read.share.sjlbkw.cn/Article/details/gxaijhpzi.sHtML

[T19] Swift：可选绑定
来源：http://baike.vehdjk.com/Article/details/gblfgbive.sHtML

if let n = opt { print(n) }
来源：http://blog.bbcook.cn/Article/details/gqqfvtgkh.sHtML

[T20] Swift：数组操作
来源：http://mobile.bbcook.cn/Article/details/gptnwrzlk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.sjlbkw.cn/Article/details/gzibirmro.sHtML

[T21] Swift：遍历
来源：http://3g.tarul.cn/Article/details/gwlarobim.sHtML

for x in a { print(x) }
来源：http://wap.tarul.cn/Article/details/gdqihimog.sHtML

[T22] Swift：字典
来源：http://m.share.epnwcf.com/Article/details/gvhaetzxa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.yfazqb.com/Article/details/gmpjldblj.sHtML

[T23] Swift：函数
来源：http://blog.fktsv.cn/Article/details/grkxezhbe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.tarul.cn/Article/details/gseingggw.sHtML

[T24] Swift：闭包
来源：http://read.share.yfazqb.com/Article/details/gefoqqpox.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.vehdjk.com/Article/details/gyiryywcu.sHtML

[T25] Swift：结构体
来源：http://blog.tarul.cn/Article/details/ggsbsmjbt.sHtML

struct P { var x: Int }
来源：http://wap.tarul.cn/Article/details/gfuiggbzp.sHtML

[T26] Swift：类与重写
来源：http://read.share.bbcook.cn/Article/details/gyewgncjm.sHtML

class A: Base { override func f() {} }
来源：http://read.share.tarul.cn/Article/details/glykjkfsn.sHtML

[T27] Swift：错误处理
来源：http://read.share.epnwcf.com/Article/details/gnxckcnsd.sHtML

do { try f() } catch { print(error) }
来源：http://baike.epnwcf.com/Article/details/gnsctlnmx.sHtML

[T28] Swift：枚举
来源：http://blog.tarul.cn/Article/details/gadojkdjr.sHtML

enum Color { case red, green }
来源：http://wap.yfazqb.com/Article/details/gykjvkahe.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.epnwcf.com/Article/details/glqyyxrnv.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fktsv.cn/Article/details/geixtddnq.sHtML

[T30] Swift：协议
来源：http://baike.bbcook.cn/Article/details/gkxjaoyqb.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.vehdjk.com/Article/details/gxjbapsil.sHtML

[T31] Lua：Hello World
来源：http://www.blog.tarul.cn/Article/details/gizmcqirr.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/gvrgkqokd.sHtML

[T32] Lua：局部变量
来源：http://mobile.sjlbkw.cn/Article/details/guwqifdvr.sHtML

local a = 1
来源：http://wap.yfazqb.com/Article/details/gvxzgwjeh.sHtML

[T33] Lua：表（数组）
来源：http://mobile.vehdjk.com/Article/details/gaqgpiuim.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.tarul.cn/Article/details/gfovepkqt.sHtML

[T34] Lua：遍历表
来源：http://3g.vehdjk.com/Article/details/ggoaeqzui.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.sjlbkw.cn/Article/details/gusjxtizr.sHtML

[T35] Lua：字典表
来源：http://wap.tarul.cn/Article/details/gaxsyukyn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.tarul.cn/Article/details/gpxkqgkjh.sHtML

[T36] Lua：函数
来源：http://www.blog.vehdjk.com/Article/details/gixdyxidb.sHtML

function add(a, b) return a + b end
来源：http://blog.tarul.cn/Article/details/gczphhexe.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.vehdjk.com/Article/details/gmdkqaraj.sHtML

"a" .. "b"
来源：http://read.share.fktsv.cn/Article/details/gghscdksh.sHtML

[T38] Lua：条件
来源：http://read.share.fktsv.cn/Article/details/gyedorwrg.sHtML

if x > 0 then print("正") end
来源：http://www.share.sjlbkw.cn/Article/details/gdwcdcjwv.sHtML

[T39] Lua：模式匹配
来源：http://baike.yfazqb.com/Article/details/gebmwyxsq.sHtML

string.find(s, "%d+")
来源：http://m.share.sjlbkw.cn/Article/details/guowiskko.sHtML

[T40] Lua：元表
来源：http://3g.tarul.cn/Article/details/gcmaaseno.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.epnwcf.com/Article/details/gfgtqinzb.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gkesdvlbm.sHtML

print "Hello\n";
来源：http://wap.epnwcf.com/Article/details/gorxijnsn.sHtML

[T42] Perl：变量类型
来源：http://m.share.fktsv.cn/Article/details/gszubhdis.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.vehdjk.com/Article/details/gbqxcpdlb.sHtML

[T43] Perl：字符串插值
来源：http://read.share.tarul.cn/Article/details/gvnreescn.sHtML

"值: $a"
来源：http://www.blog.vehdjk.com/Article/details/gjtbiwkxt.sHtML

[T44] Perl：条件
来源：http://read.share.yfazqb.com/Article/details/goslpninr.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fktsv.cn/Article/details/gpbmnxcqk.sHtML

[T45] Perl：数组遍历
来源：http://wap.epnwcf.com/Article/details/grultrdih.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.tarul.cn/Article/details/ghrrgnzpq.sHtML

[T46] Perl：哈希操作
来源：http://read.share.tarul.cn/Article/details/gubdsvtoa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.epnwcf.com/Article/details/ghccdegea.sHtML

[T47] Perl：正则捕获
来源：http://blog.sjlbkw.cn/Article/details/gtznhnnfz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.epnwcf.com/Article/details/glvhdalnu.sHtML

[T48] Perl：正则替换
来源：http://www.share.yfazqb.com/Article/details/gdomwufau.sHtML

$s =~ s/old/new/g;
来源：http://wap.fktsv.cn/Article/details/giceeirvw.sHtML

[T49] Perl：函数
来源：http://www.blog.tarul.cn/Article/details/grvnkrtvt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gafdcaiof.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqthrotx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.yfazqb.com/Article/details/gmitzmxtl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.sjlbkw.cn/Article/details/geputrvub.sHtML

[T51] Scala：Hello World
来源：http://blog.tarul.cn/Article/details/gxattjtdy.sHtML

println("Hello")
来源：http://3g.tarul.cn/Article/details/gmumctozw.sHtML

[T52] Scala：变量
来源：http://mobile.vehdjk.com/Article/details/gktidgzsj.sHtML

val a = 1;  var b = 2
来源：http://3g.epnwcf.com/Article/details/gwhqdqgio.sHtML

[T53] Scala：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gatgfqolt.sHtML

s"值: $b"
来源：http://read.share.fktsv.cn/Article/details/gxrduketq.sHtML

[T54] Scala：集合映射
来源：http://blog.yfazqb.com/Article/details/gxkusbjrz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fktsv.cn/Article/details/guywepycx.sHtML

[T55] Scala：集合过滤
来源：http://wap.yfazqb.com/Article/details/gruiuqwkd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.bbcook.cn/Article/details/gxzlslmtg.sHtML

[T56] Scala：样例类
来源：http://wap.vehdjk.com/Article/details/gzaeemjmv.sHtML

case class User(name: String, age: Int)
来源：http://blog.bbcook.cn/Article/details/ghumavuka.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fktsv.cn/Article/details/gcnbdxvdh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.yfazqb.com/Article/details/gipolwtxw.sHtML

[T58] Scala：函数定义
来源：http://www.blog.bbcook.cn/Article/details/gqubwjpjx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.bbcook.cn/Article/details/ghhwwrnlv.sHtML

[T59] Scala：循环
来源：http://www.blog.fktsv.cn/Article/details/gbmrobygc.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fktsv.cn/Article/details/gbnbriybj.sHtML

[T60] Scala：折叠
来源：http://blog.fktsv.cn/Article/details/gbaxhnqfo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.sjlbkw.cn/Article/details/gzoturjhd.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/garadjari.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.tarul.cn/Article/details/gdjczirgg.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gazkdiilo.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fktsv.cn/Article/details/gmjhqnkni.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.vehdjk.com/Article/details/gejzpvmrf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.bbcook.cn/Article/details/gdwcmguhe.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fktsv.cn/Article/details/gwhowkzur.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.tarul.cn/Article/details/gloopzxgi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.sjlbkw.cn/Article/details/gqhrvjbst.sHtML

[U04] Py：变量调试打印
来源：http://m.share.tarul.cn/Article/details/gvrcsiflu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.epnwcf.com/Article/details/ghvqlfimo.sHtML

[U05] Py：列表去重且保序
来源：http://baike.sjlbkw.cn/Article/details/gjjzwnxid.sHtML

list(dict.fromkeys(arr))
来源：http://blog.vehdjk.com/Article/details/gtpkeufqc.sHtML

[U06] Py：合并两个字典
来源：http://read.share.vehdjk.com/Article/details/ggjsgatwk.sHtML

{**a, **b}
来源：http://mobile.bbcook.cn/Article/details/gotpsehwy.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fktsv.cn/Article/details/geauayxsl.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.yfazqb.com/Article/details/ggqcmopkj.sHtML

[U08] Py：展平二维列表
来源：http://3g.epnwcf.com/Article/details/gejtcrjfb.sHtML

[y for x in nested for y in x]
来源：http://wap.vehdjk.com/Article/details/gdhwwvwyz.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.vehdjk.com/Article/details/gypovbqkt.sHtML

max(d, key=d.get)
来源：http://www.m.share.fktsv.cn/Article/details/glornxvib.sHtML

[U10] Py：按值排序字典
来源：http://read.share.tarul.cn/Article/details/gifvmomds.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.epnwcf.com/Article/details/glwshnqii.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.bbcook.cn/Article/details/gznrhpnti.sHtML

(x * 2 for x in arr)
来源：http://3g.bbcook.cn/Article/details/ggnzcgvcg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.yfazqb.com/Article/details/gaxqanuzk.sHtML

Counter(arr).most_common(3)
来源：http://baike.yfazqb.com/Article/details/gftjdfahd.sHtML

[U13] Py：固定长度队列
来源：http://wap.epnwcf.com/Article/details/gdcptizrj.sHtML

deque(maxlen=10)
来源：http://m.share.yfazqb.com/Article/details/gbwkrwese.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.bbcook.cn/Article/details/gjnblqiqj.sHtML

defaultdict(list)
来源：http://www.m.share.vehdjk.com/Article/details/gckdudnul.sHtML

[U15] Py：高精度计时
来源：http://wap.tarul.cn/Article/details/glgzbnnfl.sHtML

t = time.perf_counter()
来源：http://www.share.fktsv.cn/Article/details/ggzxglpll.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fktsv.cn/Article/details/ggfkkepux.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.sjlbkw.cn/Article/details/gbukrywhq.sHtML

[U17] Py：初始化日志
来源：http://read.share.yfazqb.com/Article/details/grpxvxyud.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.tarul.cn/Article/details/gebkypuyy.sHtML

[U18] Py：预编译正则
来源：http://m.share.tarul.cn/Article/details/gqhpawzrn.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fktsv.cn/Article/details/gyhlngngo.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.epnwcf.com/Article/details/gzvmfnpup.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.bbcook.cn/Article/details/ghomtgwqb.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fktsv.cn/Article/details/gryonmgxo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.vehdjk.com/Article/details/gkapvfecw.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.yfazqb.com/Article/details/gcvnwgles.sHtML

@contextlib.contextmanager
来源：http://3g.epnwcf.com/Article/details/gbxdijmif.sHtML

[U22] Py：矩阵转置
来源：http://baike.yfazqb.com/Article/details/grgyrwgny.sHtML

list(zip(*m))
来源：http://3g.epnwcf.com/Article/details/gfyboyvlx.sHtML

[U23] Py：分块读取大文件
来源：http://baike.tarul.cn/Article/details/gpnpdqnwi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.epnwcf.com/Article/details/gqdogwjnx.sHtML

[U24] Py：路径操作
来源：http://baike.bbcook.cn/Article/details/gbxphucqj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fktsv.cn/Article/details/gusxcotvk.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvyndwvz.sHtML

csv.DictReader(f)
来源：http://baike.yfazqb.com/Article/details/gcfgzkrrz.sHtML

[U26] Py：并发下载
来源：http://wap.vehdjk.com/Article/details/guhqnulkh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.yfazqb.com/Article/details/gdhbxazvh.sHtML

[U27] Py：异步 HTTP
来源：http://3g.yfazqb.com/Article/details/gnffrpmsu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.tarul.cn/Article/details/gtjxztchj.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fktsv.cn/Article/details/gkpjxgxbs.sHtML

UserId = int
来源：http://www.blog.fktsv.cn/Article/details/gbycizgru.sHtML

[U29] Py：属性校验
来源：http://3g.vehdjk.com/Article/details/gcuhdfqok.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.vehdjk.com/Article/details/gmyxndmsd.sHtML

[U30] Py：数据类
来源：http://www.share.bbcook.cn/Article/details/gaoqlgivd.sHtML

@dataclass(slots=True)
来源：http://mobile.vehdjk.com/Article/details/gzalhcoch.sHtML

[U31] Py：单测
来源：http://blog.fktsv.cn/Article/details/gbosocluz.sHtML

python -m pytest -q
来源：http://www.blog.vehdjk.com/Article/details/gefciudka.sHtML

[U32] Py：代码格式化
来源：http://3g.vehdjk.com/Article/details/gioqduogt.sHtML

ruff format . && ruff check --fix .
来源：http://3g.sjlbkw.cn/Article/details/gdhotulpa.sHtML

[U33] Py：打包发布
来源：http://blog.vehdjk.com/Article/details/gjqlifwyc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.sjlbkw.cn/Article/details/gmmlilafm.sHtML

[U34] Py：判断编码
来源：http://baike.bbcook.cn/Article/details/gxauecvps.sHtML

chardet.detect(raw)
来源：http://www.blog.tarul.cn/Article/details/gxvoigsoi.sHtML

[U35] Py：发送邮件
来源：http://m.share.epnwcf.com/Article/details/gqmqxwalg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.vehdjk.com/Article/details/gwvfgzswd.sHtML

[U36] Py：定时任务
来源：http://www.blog.epnwcf.com/Article/details/ggjmvqjzn.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.tarul.cn/Article/details/gabhzrroc.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.vehdjk.com/Article/details/gutuevjeo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fktsv.cn/Article/details/gmtemmetm.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.bbcook.cn/Article/details/gikdlepio.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.yfazqb.com/Article/details/gsbmpxrth.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.yfazqb.com/Article/details/gtomolopr.sHtML

sys.stdout.isatty()
来源：http://wap.sjlbkw.cn/Article/details/guppyxjzc.sHtML

[U40] Py：打印到标准错误
来源：http://baike.sjlbkw.cn/Article/details/gojfgnrrr.sHtML

print("err", file=sys.stderr)
来源：http://read.share.epnwcf.com/Article/details/gqberqsdv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.tarul.cn/Article/details/gnzysknhx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.sjlbkw.cn/Article/details/goddjasnl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.epnwcf.com/Article/details/gjynepltw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.epnwcf.com/Article/details/gldfcdfme.sHtML

[U43] PHP：声明命名空间
来源：http://wap.vehdjk.com/Article/details/gugrftvbr.sHtML

namespace App\Http;
来源：http://wap.epnwcf.com/Article/details/ghrwktcth.sHtML

[U44] PHP：开启严格类型
来源：http://blog.vehdjk.com/Article/details/gkfnxliyr.sHtML

declare(strict_types=1);
来源：http://3g.tarul.cn/Article/details/gadjyvyal.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.epnwcf.com/Article/details/gbblnplgz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/ghtwzxzdq.sHtML

[U46] PHP：可空类型
来源：http://baike.tarul.cn/Article/details/gejqutzrl.sHtML

?string $name = null
来源：http://read.share.tarul.cn/Article/details/glicuvmpw.sHtML

[U47] PHP：联合类型
来源：http://3g.vehdjk.com/Article/details/gkgzuyavo.sHtML

int|string $id
来源：http://mobile.yfazqb.com/Article/details/gnrmdviyc.sHtML

[U48] PHP：纯枚举
来源：http://read.share.vehdjk.com/Article/details/grdstohwi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.sjlbkw.cn/Article/details/gsszepndr.sHtML

[U49] PHP：只读属性
来源：http://baike.bbcook.cn/Article/details/geqvafbwq.sHtML

public readonly string $name
来源：http://wap.tarul.cn/Article/details/guzyamkvw.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.bbcook.cn/Article/details/gorthnfab.sHtML

public function __construct(private int $id) {}
来源：http://baike.bbcook.cn/Article/details/glmdutqfm.sHtML

[U51] PHP：数组解构
来源：http://mobile.epnwcf.com/Article/details/gllynqudr.sHtML

[$a, $b] = $arr;
来源：http://3g.yfazqb.com/Article/details/geopkirjy.sHtML

[U52] PHP：箭头函数
来源：http://www.share.tarul.cn/Article/details/gwhzztzdb.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fktsv.cn/Article/details/gbmtfdnnf.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.sjlbkw.cn/Article/details/ghysmlsjs.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.epnwcf.com/Article/details/gnwwffyyg.sHtML

[U54] PHP：空安全调用
来源：http://3g.fktsv.cn/Article/details/gezobscuc.sHtML

$obj?->method()
来源：http://read.share.tarul.cn/Article/details/globwpmfo.sHtML

[U55] PHP：match 表达式
来源：http://baike.bbcook.cn/Article/details/grpzppsyj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.tarul.cn/Article/details/gqljhaajz.sHtML

[U56] PHP：命名参数
来源：http://read.share.vehdjk.com/Article/details/gvfizthud.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/gazomkkxv.sHtML

[U57] PHP：字符串插值
来源：http://blog.vehdjk.com/Article/details/ghuzbbiit.sHtML

"值: {$a}"
来源：http://mobile.vehdjk.com/Article/details/gxwvcmqod.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.sjlbkw.cn/Article/details/gqglnvtbg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.bbcook.cn/Article/details/gxfsjlmcs.sHtML


<!-- 参考信息 -->