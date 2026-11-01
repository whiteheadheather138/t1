代发 wailian999

[S33] C++：vector 增删
来源：http://baike.sjlbkw.cn/Article/details/gpeodnkdd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.sjlbkw.cn/Article/details/gefdxblau.sHtML

[S34] C++：遍历 vector
来源：http://read.share.epnwcf.com/Article/details/gcogqocji.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.bbcook.cn/Article/details/gjndmxisl.sHtML

[S35] C++：map
来源：http://3g.epnwcf.com/Article/details/gxjxzixwm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gkrjrbhdz.sHtML

[S36] C++：unordered_map
来源：http://blog.vehdjk.com/Article/details/gnxyggtdg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gtsbmddtr.sHtML

[S37] C++：set
来源：http://3g.bbcook.cn/Article/details/gitgfeyvh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.tarul.cn/Article/details/gacgvpehr.sHtML

[S38] C++：排序
来源：http://www.m.share.fktsv.cn/Article/details/gnwmdzqxd.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.yfazqb.com/Article/details/gdbddzdtw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.sjlbkw.cn/Article/details/gqighzysq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fktsv.cn/Article/details/getvrdgnm.sHtML

[S40] C++：查找元素
来源：http://wap.bbcook.cn/Article/details/gvpltxhdt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.bbcook.cn/Article/details/gizvwnvlj.sHtML

[S41] C++：类与构造函数
来源：http://baike.vehdjk.com/Article/details/gyvtbgzyc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.yfazqb.com/Article/details/gqyoxakjy.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fktsv.cn/Article/details/gulrbkdkm.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.bbcook.cn/Article/details/gqnppazbc.sHtML

[S43] C++：智能指针
来源：http://wap.bbcook.cn/Article/details/gwmxptlcf.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.epnwcf.com/Article/details/gtbwoidzb.sHtML

[S44] C++：引用传参
来源：http://mobile.yfazqb.com/Article/details/gjlicwqbm.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.epnwcf.com/Article/details/glacjjfyk.sHtML

[S45] C++：lambda
来源：http://wap.vehdjk.com/Article/details/gmexjadzp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.epnwcf.com/Article/details/gmzrjtixh.sHtML

[S46] C++：函数模板
来源：http://mobile.vehdjk.com/Article/details/gpezkeddk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.vehdjk.com/Article/details/gebatsvtd.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.epnwcf.com/Article/details/gfftoavxu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.bbcook.cn/Article/details/gspwxrvtj.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gigdwfylq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.tarul.cn/Article/details/gakwgcjei.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fktsv.cn/Article/details/gylqniuwo.sHtML

[S49] C++：写文件
来源：http://read.share.yfazqb.com/Article/details/guunhimib.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.tarul.cn/Article/details/gjgztdscg.sHtML

[S50] C++：格式化数字
来源：http://www.share.tarul.cn/Article/details/gvlwbnjsz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gkabjnxst.sHtML

[S51] C++：显式类型转换
来源：http://wap.tarul.cn/Article/details/ghyqivrtz.sHtML

static_cast<double>(a) / b
来源：http://m.share.fktsv.cn/Article/details/gpnsegvho.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.vehdjk.com/Article/details/gdstuarre.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.sjlbkw.cn/Article/details/gooyuvvlj.sHtML

[S53] C++：移动语义
来源：http://read.share.bbcook.cn/Article/details/gaoyloqsj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.bbcook.cn/Article/details/ghkjkxusl.sHtML

[S54] C++：异常处理
来源：http://mobile.bbcook.cn/Article/details/gfdvqkrln.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.yfazqb.com/Article/details/grmahgghh.sHtML

[S55] C++：结构化绑定
来源：http://wap.tarul.cn/Article/details/ggmwjsmjx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.tarul.cn/Article/details/gsdndcoeb.sHtML

[S56] C++：optional
来源：http://www.m.share.tarul.cn/Article/details/gdyfuciam.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.bbcook.cn/Article/details/gpfwheveo.sHtML

[S57] C++：编译期常量
来源：http://read.share.vehdjk.com/Article/details/gaoqxpukw.sHtML

constexpr int N = 10;
来源：http://3g.epnwcf.com/Article/details/grlizyujz.sHtML

[S58] C++：命名空间
来源：http://www.blog.sjlbkw.cn/Article/details/gmxznvbyv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.epnwcf.com/Article/details/gaeajliuq.sHtML

[S59] C++：静态断言
来源：http://mobile.yfazqb.com/Article/details/gqmiurhqw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.epnwcf.com/Article/details/guqfnuuyg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fktsv.cn/Article/details/glefkfpug.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fktsv.cn/Article/details/gncflirjn.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gcwrejdic.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.tarul.cn/Article/details/gljyogewe.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gduqgwxlb.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gybkxagba.sHtML

println("Hello")
来源：http://baike.bbcook.cn/Article/details/gqiirsirl.sHtML

[T02] Kotlin：变量
来源：http://www.share.yfazqb.com/Article/details/ganhbkehu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.vehdjk.com/Article/details/ghtvwztez.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.yfazqb.com/Article/details/gshckxgyh.sHtML

"值: $b"
来源：http://www.m.share.tarul.cn/Article/details/gfratcbnv.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fktsv.cn/Article/details/gmbzhgpie.sHtML

val n: String? = null;  n?.length
来源：http://baike.vehdjk.com/Article/details/ghqkzmgke.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.yfazqb.com/Article/details/gkxriobpp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.epnwcf.com/Article/details/gmiefclrs.sHtML

[T06] Kotlin：集合映射
来源：http://3g.epnwcf.com/Article/details/gomkxsutk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gfgwqxlbz.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.tarul.cn/Article/details/gfhdovgkp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fktsv.cn/Article/details/gxhcxkqhs.sHtML

[T08] Kotlin：数据类
来源：http://blog.sjlbkw.cn/Article/details/gswsesmtg.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.sjlbkw.cn/Article/details/gbiwoobar.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.sjlbkw.cn/Article/details/gpvlfzawv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fktsv.cn/Article/details/gocjququu.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fktsv.cn/Article/details/gnpisnruw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.tarul.cn/Article/details/glmivplha.sHtML

[T11] Kotlin：协程
来源：http://wap.fktsv.cn/Article/details/gqyjyoppb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.yfazqb.com/Article/details/gwicpevsr.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.epnwcf.com/Article/details/guekvkysi.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.vehdjk.com/Article/details/grulydukm.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fktsv.cn/Article/details/gmmbeguvp.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fktsv.cn/Article/details/gpbkpzxmf.sHtML

[T14] Kotlin：循环
来源：http://wap.vehdjk.com/Article/details/gwqaqarjn.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/gofgoismr.sHtML

[T15] Kotlin：接口
来源：http://read.share.epnwcf.com/Article/details/gcblpwxzy.sHtML

interface Shape { fun area(): Double }
来源：http://blog.vehdjk.com/Article/details/gjdohmfnm.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gtwmdbmrv.sHtML

print("Hello")
来源：http://baike.tarul.cn/Article/details/gfkhfcwly.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.bbcook.cn/Article/details/gfoktaiwr.sHtML

var a = 1;  let b = 2
来源：http://m.share.epnwcf.com/Article/details/grvzcjiuf.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gyumpivvc.sHtML

"值: \(b)"
来源：http://m.share.sjlbkw.cn/Article/details/gaugxvual.sHtML

[T19] Swift：可选绑定
来源：http://blog.tarul.cn/Article/details/girhxfuqi.sHtML

if let n = opt { print(n) }
来源：http://3g.tarul.cn/Article/details/gvfidkdeu.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgnzcgsp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.vehdjk.com/Article/details/ghvvmcbkb.sHtML

[T21] Swift：遍历
来源：http://www.m.share.yfazqb.com/Article/details/glrxevaou.sHtML

for x in a { print(x) }
来源：http://3g.tarul.cn/Article/details/gukfhgbjn.sHtML

[T22] Swift：字典
来源：http://www.blog.fktsv.cn/Article/details/gjcqbuewn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.tarul.cn/Article/details/gouruvjcp.sHtML

[T23] Swift：函数
来源：http://m.share.yfazqb.com/Article/details/gvyqmirvx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.vehdjk.com/Article/details/gssxfqyqi.sHtML

[T24] Swift：闭包
来源：http://www.blog.bbcook.cn/Article/details/gcburuecr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gueavvmpt.sHtML

[T25] Swift：结构体
来源：http://m.share.vehdjk.com/Article/details/gxrazflie.sHtML

struct P { var x: Int }
来源：http://wap.epnwcf.com/Article/details/gwzweojep.sHtML

[T26] Swift：类与重写
来源：http://mobile.epnwcf.com/Article/details/gfblmvlgn.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghihizcwj.sHtML

[T27] Swift：错误处理
来源：http://baike.fktsv.cn/Article/details/gevauglap.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.epnwcf.com/Article/details/gkxadjuhp.sHtML

[T28] Swift：枚举
来源：http://www.share.yfazqb.com/Article/details/guttuuoht.sHtML

enum Color { case red, green }
来源：http://m.share.vehdjk.com/Article/details/gfsbfyxwe.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fktsv.cn/Article/details/gkgzatxsk.sHtML

guard let x = opt else { return }
来源：http://wap.fktsv.cn/Article/details/gmorrzweu.sHtML

[T30] Swift：协议
来源：http://mobile.sjlbkw.cn/Article/details/gipjbduxs.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.tarul.cn/Article/details/gkjumqqhi.sHtML

[T31] Lua：Hello World
来源：http://blog.bbcook.cn/Article/details/giuzwtfpb.sHtML

print("Hello")
来源：http://www.blog.tarul.cn/Article/details/gwgnonkgr.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.yfazqb.com/Article/details/gorhmhkpo.sHtML

local a = 1
来源：http://m.share.fktsv.cn/Article/details/gnddbjecq.sHtML

[T33] Lua：表（数组）
来源：http://mobile.sjlbkw.cn/Article/details/gtijrnfms.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.bbcook.cn/Article/details/gmzqswvxk.sHtML

[T34] Lua：遍历表
来源：http://baike.fktsv.cn/Article/details/gkaufazll.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.bbcook.cn/Article/details/goykguojk.sHtML

[T35] Lua：字典表
来源：http://read.share.sjlbkw.cn/Article/details/gpspdwegn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.vehdjk.com/Article/details/gvcakqtrj.sHtML

[T36] Lua：函数
来源：http://www.share.yfazqb.com/Article/details/grifbbhvb.sHtML

function add(a, b) return a + b end
来源：http://www.share.epnwcf.com/Article/details/ggjexddgo.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.vehdjk.com/Article/details/gvbamiymh.sHtML

"a" .. "b"
来源：http://www.blog.yfazqb.com/Article/details/gnhwfwfdw.sHtML

[T38] Lua：条件
来源：http://read.share.vehdjk.com/Article/details/glkcifmte.sHtML

if x > 0 then print("正") end
来源：http://baike.fktsv.cn/Article/details/gxqgqnjjf.sHtML

[T39] Lua：模式匹配
来源：http://wap.tarul.cn/Article/details/gjjypqxsn.sHtML

string.find(s, "%d+")
来源：http://3g.epnwcf.com/Article/details/ggownvugy.sHtML

[T40] Lua：元表
来源：http://blog.sjlbkw.cn/Article/details/gxmpdetil.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.vehdjk.com/Article/details/grqtedphs.sHtML

[T41] Perl：Hello World
来源：http://wap.tarul.cn/Article/details/goqmrtdwd.sHtML

print "Hello\n";
来源：http://mobile.yfazqb.com/Article/details/gnuggahvl.sHtML

[T42] Perl：变量类型
来源：http://m.share.yfazqb.com/Article/details/grraabgtp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.tarul.cn/Article/details/gephkqisd.sHtML

[T43] Perl：字符串插值
来源：http://baike.yfazqb.com/Article/details/gtxsevidm.sHtML

"值: $a"
来源：http://www.m.share.bbcook.cn/Article/details/grcucfshy.sHtML

[T44] Perl：条件
来源：http://read.share.yfazqb.com/Article/details/gvdrkhrhw.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.vehdjk.com/Article/details/gxgukkfwv.sHtML

[T45] Perl：数组遍历
来源：http://blog.sjlbkw.cn/Article/details/gagqxomaf.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.bbcook.cn/Article/details/gkesnwhpv.sHtML

[T46] Perl：哈希操作
来源：http://mobile.epnwcf.com/Article/details/gayteeddl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.bbcook.cn/Article/details/ggumwcien.sHtML

[T47] Perl：正则捕获
来源：http://baike.bbcook.cn/Article/details/gznbzvbta.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.yfazqb.com/Article/details/gnagzlaiz.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.yfazqb.com/Article/details/gnqwfdmpz.sHtML

$s =~ s/old/new/g;
来源：http://read.share.bbcook.cn/Article/details/ghaltrdmq.sHtML

[T49] Perl：函数
来源：http://3g.bbcook.cn/Article/details/gapixngry.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbnffnwr.sHtML

[T50] Perl：逐行读文件
来源：http://wap.epnwcf.com/Article/details/ghupucqlu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.epnwcf.com/Article/details/gwjriocnn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.tarul.cn/Article/details/ggsxvqogj.sHtML

[T51] Scala：Hello World
来源：http://3g.vehdjk.com/Article/details/gzmfxtshf.sHtML

println("Hello")
来源：http://www.blog.tarul.cn/Article/details/gekhtakvv.sHtML

[T52] Scala：变量
来源：http://3g.yfazqb.com/Article/details/gmiuishhx.sHtML

val a = 1;  var b = 2
来源：http://baike.epnwcf.com/Article/details/gjvnzdsnu.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gmytmbwhl.sHtML

s"值: $b"
来源：http://3g.epnwcf.com/Article/details/gywbydywx.sHtML

[T54] Scala：集合映射
来源：http://m.share.vehdjk.com/Article/details/gdzqlhefx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.sjlbkw.cn/Article/details/giedbindz.sHtML

[T55] Scala：集合过滤
来源：http://m.share.epnwcf.com/Article/details/gjarlivvf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fktsv.cn/Article/details/gyqwoazxs.sHtML

[T56] Scala：样例类
来源：http://3g.epnwcf.com/Article/details/gotkolcxj.sHtML

case class User(name: String, age: Int)
来源：http://wap.fktsv.cn/Article/details/gzhwxhwfq.sHtML

[T57] Scala：模式匹配
来源：http://blog.sjlbkw.cn/Article/details/ghwtioyce.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.yfazqb.com/Article/details/gvhxlonda.sHtML

[T58] Scala：函数定义
来源：http://blog.yfazqb.com/Article/details/ggoqacepv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.vehdjk.com/Article/details/gmcukrngf.sHtML

[T59] Scala：循环
来源：http://www.m.share.bbcook.cn/Article/details/gvbhwuvmd.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.vehdjk.com/Article/details/gnnnzwdig.sHtML

[T60] Scala：折叠
来源：http://read.share.tarul.cn/Article/details/gtcgefxew.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.yfazqb.com/Article/details/gfcsjooan.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gfwjzafwy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.bbcook.cn/Article/details/gkhrdcief.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gbihlrfmq.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.epnwcf.com/Article/details/giiskhybp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.tarul.cn/Article/details/gjgcnhlky.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fktsv.cn/Article/details/gqpnqlnpf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.epnwcf.com/Article/details/gfolyezpm.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.tarul.cn/Article/details/gdplczzau.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.sjlbkw.cn/Article/details/gzdxwcxja.sHtML

[U04] Py：变量调试打印
来源：http://read.share.vehdjk.com/Article/details/ghdrundfo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.epnwcf.com/Article/details/gpvjjblat.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.bbcook.cn/Article/details/gerfcdlop.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/gosjbfjoa.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gndibfted.sHtML

{**a, **b}
来源：http://read.share.sjlbkw.cn/Article/details/gqnvbqtax.sHtML

[U07] Py：反转字典键值
来源：http://m.share.bbcook.cn/Article/details/gumtsfqos.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.yfazqb.com/Article/details/gjoaewvvj.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gbppvidhj.sHtML

[y for x in nested for y in x]
来源：http://mobile.tarul.cn/Article/details/gulagjtvq.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.bbcook.cn/Article/details/gfcbgfzpo.sHtML

max(d, key=d.get)
来源：http://wap.vehdjk.com/Article/details/ghwncvzca.sHtML

[U10] Py：按值排序字典
来源：http://read.share.vehdjk.com/Article/details/goledytzl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fktsv.cn/Article/details/gzgfvwiqh.sHtML

[U11] Py：生成器表达式
来源：http://baike.sjlbkw.cn/Article/details/gqivdukjv.sHtML

(x * 2 for x in arr)
来源：http://www.blog.yfazqb.com/Article/details/gcfjaxtgo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.epnwcf.com/Article/details/gnyhtoppq.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.tarul.cn/Article/details/gyncwjini.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fktsv.cn/Article/details/gvwsxdzuq.sHtML

deque(maxlen=10)
来源：http://www.blog.sjlbkw.cn/Article/details/gvhglmmzh.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.epnwcf.com/Article/details/grrlhjvyi.sHtML

defaultdict(list)
来源：http://baike.vehdjk.com/Article/details/gyrgiuavn.sHtML

[U15] Py：高精度计时
来源：http://read.share.fktsv.cn/Article/details/gsxhtwbns.sHtML

t = time.perf_counter()
来源：http://www.blog.bbcook.cn/Article/details/gahwuovyz.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.sjlbkw.cn/Article/details/gefimzwun.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.bbcook.cn/Article/details/gelqosjhe.sHtML

[U17] Py：初始化日志
来源：http://mobile.bbcook.cn/Article/details/goyddvmco.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.sjlbkw.cn/Article/details/gzskndwrf.sHtML

[U18] Py：预编译正则
来源：http://wap.yfazqb.com/Article/details/gdqrdlehi.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/gcshixnyy.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.yfazqb.com/Article/details/gsonauszi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.yfazqb.com/Article/details/gseleyrmw.sHtML

[U20] Py：缓存函数结果
来源：http://blog.yfazqb.com/Article/details/gkiygguak.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.bbcook.cn/Article/details/givdpkyhh.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.sjlbkw.cn/Article/details/gtggkajwv.sHtML

@contextlib.contextmanager
来源：http://mobile.tarul.cn/Article/details/gtmqyyhft.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fktsv.cn/Article/details/gagtbcjvr.sHtML

list(zip(*m))
来源：http://blog.tarul.cn/Article/details/gewghfqxt.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.tarul.cn/Article/details/gwvbypyqx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.bbcook.cn/Article/details/gergxofuc.sHtML

[U24] Py：路径操作
来源：http://m.share.fktsv.cn/Article/details/gcjikjlxo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.vehdjk.com/Article/details/gtyomvscz.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.yfazqb.com/Article/details/gsuwdqdjt.sHtML

csv.DictReader(f)
来源：http://www.share.fktsv.cn/Article/details/gumlnmniz.sHtML

[U26] Py：并发下载
来源：http://wap.vehdjk.com/Article/details/glrzhmigw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.bbcook.cn/Article/details/gbpwaojzr.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.yfazqb.com/Article/details/gepepgwsg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.vehdjk.com/Article/details/gmlrkjxtu.sHtML

[U28] Py：类型别名
来源：http://baike.sjlbkw.cn/Article/details/gafodfpse.sHtML

UserId = int
来源：http://www.share.yfazqb.com/Article/details/giywhvdgl.sHtML

[U29] Py：属性校验
来源：http://www.m.share.vehdjk.com/Article/details/gmrvxmzam.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.bbcook.cn/Article/details/gjiukmlri.sHtML

[U30] Py：数据类
来源：http://m.share.tarul.cn/Article/details/gtljiqexn.sHtML

@dataclass(slots=True)
来源：http://www.m.share.tarul.cn/Article/details/gvesokbjc.sHtML

[U31] Py：单测
来源：http://www.share.epnwcf.com/Article/details/grlhntmgb.sHtML

python -m pytest -q
来源：http://baike.sjlbkw.cn/Article/details/gglydgtwk.sHtML

[U32] Py：代码格式化
来源：http://mobile.fktsv.cn/Article/details/gcherlitj.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fktsv.cn/Article/details/gzohcmczb.sHtML

[U33] Py：打包发布
来源：http://mobile.bbcook.cn/Article/details/gwusravha.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.tarul.cn/Article/details/gbliybgrz.sHtML

[U34] Py：判断编码
来源：http://read.share.yfazqb.com/Article/details/gxoonrczy.sHtML

chardet.detect(raw)
来源：http://mobile.vehdjk.com/Article/details/ggqepdmva.sHtML

[U35] Py：发送邮件
来源：http://wap.vehdjk.com/Article/details/gmsuwuenj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.epnwcf.com/Article/details/gmrveslnm.sHtML

[U36] Py：定时任务
来源：http://blog.bbcook.cn/Article/details/gxunsyvbv.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.yfazqb.com/Article/details/gwqbrgmoh.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fktsv.cn/Article/details/gimnqbtcb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.epnwcf.com/Article/details/gkicahruj.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.epnwcf.com/Article/details/gvhyxjjxf.sHtML

Path(__file__).resolve().parent
来源：http://www.share.tarul.cn/Article/details/gudpqgakz.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.yfazqb.com/Article/details/ggyuhtxfz.sHtML

sys.stdout.isatty()
来源：http://read.share.fktsv.cn/Article/details/ghmxrznig.sHtML

[U40] Py：打印到标准错误
来源：http://wap.sjlbkw.cn/Article/details/gzbxcrmxa.sHtML

print("err", file=sys.stderr)
来源：http://mobile.yfazqb.com/Article/details/grxszpuxx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.vehdjk.com/Article/details/gwnaxoypl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.yfazqb.com/Article/details/gfpswoudw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.vehdjk.com/Article/details/gmytzvzah.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fktsv.cn/Article/details/gukixlxzj.sHtML

[U43] PHP：声明命名空间
来源：http://baike.epnwcf.com/Article/details/ghejwmozi.sHtML

namespace App\Http;
来源：http://read.share.sjlbkw.cn/Article/details/gejgxeqtf.sHtML

[U44] PHP：开启严格类型
来源：http://wap.tarul.cn/Article/details/ghbygupva.sHtML

declare(strict_types=1);
来源：http://m.share.fktsv.cn/Article/details/gxpbzcvab.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.epnwcf.com/Article/details/gkccridbq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gzzxpdhyu.sHtML

[U46] PHP：可空类型
来源：http://blog.vehdjk.com/Article/details/gnzqrtxoy.sHtML

?string $name = null
来源：http://blog.sjlbkw.cn/Article/details/giqjzcazz.sHtML

[U47] PHP：联合类型
来源：http://m.share.bbcook.cn/Article/details/gnxvlsezz.sHtML

int|string $id
来源：http://m.share.sjlbkw.cn/Article/details/guubcdwyy.sHtML

[U48] PHP：纯枚举
来源：http://www.share.tarul.cn/Article/details/gvglwzcpb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fktsv.cn/Article/details/gnxuydclc.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.epnwcf.com/Article/details/gsaomnxka.sHtML

public readonly string $name
来源：http://blog.sjlbkw.cn/Article/details/gttjsifaq.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.bbcook.cn/Article/details/ggyubgfqs.sHtML

public function __construct(private int $id) {}
来源：http://3g.yfazqb.com/Article/details/gseezgwau.sHtML

[U51] PHP：数组解构
来源：http://www.blog.bbcook.cn/Article/details/gdicgickk.sHtML

[$a, $b] = $arr;
来源：http://read.share.yfazqb.com/Article/details/glwylxlzs.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fktsv.cn/Article/details/gshipuqsw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fktsv.cn/Article/details/gtgdgsgbx.sHtML

[U53] PHP：空合并运算符
来源：http://wap.sjlbkw.cn/Article/details/gbbereywc.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.bbcook.cn/Article/details/gfethwfxw.sHtML

[U54] PHP：空安全调用
来源：http://blog.fktsv.cn/Article/details/gkbgnvpun.sHtML

$obj?->method()
来源：http://baike.epnwcf.com/Article/details/gzjvoosth.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcvdxsem.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.tarul.cn/Article/details/gmmtrgqmq.sHtML

[U56] PHP：命名参数
来源：http://wap.fktsv.cn/Article/details/gnyfermpf.sHtML

f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gpvkrcexp.sHtML

[U57] PHP：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gtpklnoxa.sHtML

"值: {$a}"
来源：http://read.share.tarul.cn/Article/details/ggapwraxu.sHtML

[U58] PHP：数组三件套
来源：http://blog.tarul.cn/Article/details/gsrdwpuav.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.tarul.cn/Article/details/grhponcbj.sHtML


<!-- 参考信息 -->