代发 wailian999

[S33] C++：vector 增删
来源：http://mobile.vehdjk.com/Article/details/gkbnktcso.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.tarul.cn/Article/details/gxtazxbzo.sHtML

[S34] C++：遍历 vector
来源：http://m.share.yfazqb.com/Article/details/gxfefyuqf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.tarul.cn/Article/details/gflamuqif.sHtML

[S35] C++：map
来源：http://blog.fktsv.cn/Article/details/ghbfepsfh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gntkgkugp.sHtML

[S36] C++：unordered_map
来源：http://3g.vehdjk.com/Article/details/gnuvcnbpd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/glhginjzg.sHtML

[S37] C++：set
来源：http://www.share.vehdjk.com/Article/details/gxpbigqts.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.epnwcf.com/Article/details/gqmqpqhvw.sHtML

[S38] C++：排序
来源：http://wap.sjlbkw.cn/Article/details/gjxnyvsnw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.sjlbkw.cn/Article/details/genxtlkyu.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.epnwcf.com/Article/details/gkafrxphk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.yfazqb.com/Article/details/ggwsxsqgj.sHtML

[S40] C++：查找元素
来源：http://m.share.sjlbkw.cn/Article/details/gdpboemni.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.bbcook.cn/Article/details/gsvwcgipn.sHtML

[S41] C++：类与构造函数
来源：http://baike.epnwcf.com/Article/details/ghqrjxoxu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.tarul.cn/Article/details/gqojfmbfs.sHtML

[S42] C++：继承与虚函数
来源：http://baike.yfazqb.com/Article/details/giqsdistk.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.bbcook.cn/Article/details/ggluhvoqt.sHtML

[S43] C++：智能指针
来源：http://www.share.sjlbkw.cn/Article/details/gzpqnykpg.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.bbcook.cn/Article/details/gxyplnnxc.sHtML

[S44] C++：引用传参
来源：http://baike.sjlbkw.cn/Article/details/gpdbbwxtn.sHtML

void inc(int &x) { ++x; }
来源：http://wap.tarul.cn/Article/details/gpndgdsjo.sHtML

[S45] C++：lambda
来源：http://baike.fktsv.cn/Article/details/gquewivnl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.sjlbkw.cn/Article/details/gceaypumh.sHtML

[S46] C++：函数模板
来源：http://read.share.sjlbkw.cn/Article/details/gubrgvjdd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.yfazqb.com/Article/details/gpsvigejg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.yfazqb.com/Article/details/gslegmaiw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fktsv.cn/Article/details/grslzknkt.sHtML

[S48] C++：逐行读文件
来源：http://blog.epnwcf.com/Article/details/ggixxhoxa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.yfazqb.com/Article/details/gvxanrphb.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.epnwcf.com/Article/details/gufyvxqoi.sHtML

[S49] C++：写文件
来源：http://blog.sjlbkw.cn/Article/details/gaeddwdpt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.vehdjk.com/Article/details/gnfgwxbrg.sHtML

[S50] C++：格式化数字
来源：http://baike.yfazqb.com/Article/details/gznxhocbl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.bbcook.cn/Article/details/ggduaqpep.sHtML

[S51] C++：显式类型转换
来源：http://baike.yfazqb.com/Article/details/gpdjbncqk.sHtML

static_cast<double>(a) / b
来源：http://read.share.sjlbkw.cn/Article/details/gfjbxhwde.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.vehdjk.com/Article/details/gwlkyotxz.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.yfazqb.com/Article/details/ggisqimya.sHtML

[S53] C++：移动语义
来源：http://m.share.sjlbkw.cn/Article/details/guffxqavg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fktsv.cn/Article/details/gyagkpiqj.sHtML

[S54] C++：异常处理
来源：http://read.share.tarul.cn/Article/details/gcungrxhf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.vehdjk.com/Article/details/gfkwbrkbj.sHtML

[S55] C++：结构化绑定
来源：http://m.share.tarul.cn/Article/details/gtaepdnrd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.vehdjk.com/Article/details/gyeklssdg.sHtML

[S56] C++：optional
来源：http://wap.fktsv.cn/Article/details/gtiowljjy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.tarul.cn/Article/details/gqwufetkg.sHtML

[S57] C++：编译期常量
来源：http://wap.yfazqb.com/Article/details/gnylblsjy.sHtML

constexpr int N = 10;
来源：http://baike.sjlbkw.cn/Article/details/geuinvich.sHtML

[S58] C++：命名空间
来源：http://m.share.tarul.cn/Article/details/gohqwsbeu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.vehdjk.com/Article/details/gtyfaqrdl.sHtML

[S59] C++：静态断言
来源：http://blog.vehdjk.com/Article/details/gnebyhlwz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.vehdjk.com/Article/details/giaxybviq.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.tarul.cn/Article/details/gydljgxtv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.yfazqb.com/Article/details/gziblnchq.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gqzelabmw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.sjlbkw.cn/Article/details/gcomdjtvz.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gqlxnxoug.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fktsv.cn/Article/details/grxnhduzl.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/gbkzexduz.sHtML

[T02] Kotlin：变量
来源：http://m.share.sjlbkw.cn/Article/details/gwxxkeazq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.tarul.cn/Article/details/girjgarrq.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.bbcook.cn/Article/details/geuhwrwko.sHtML

"值: $b"
来源：http://blog.bbcook.cn/Article/details/gyebwetpt.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.tarul.cn/Article/details/gyelagjpj.sHtML

val n: String? = null;  n?.length
来源：http://mobile.tarul.cn/Article/details/gbnxtrdyr.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.sjlbkw.cn/Article/details/glwfsybji.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.bbcook.cn/Article/details/glbsccobw.sHtML

[T06] Kotlin：集合映射
来源：http://3g.tarul.cn/Article/details/gifnbpnhx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gqanqwvbu.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fktsv.cn/Article/details/gmxjqfahr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.vehdjk.com/Article/details/gsfxhrqta.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fktsv.cn/Article/details/goephldgs.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gawttyteg.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.vehdjk.com/Article/details/gkhvxgcwk.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.epnwcf.com/Article/details/gyhqayfjn.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.bbcook.cn/Article/details/gqdjulzmp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.epnwcf.com/Article/details/gxjmpuuqx.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.vehdjk.com/Article/details/gvecezpch.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.epnwcf.com/Article/details/gwfhherwv.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fktsv.cn/Article/details/glkxmdwmn.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.epnwcf.com/Article/details/ghyywjpri.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.bbcook.cn/Article/details/gkazwkmmv.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.vehdjk.com/Article/details/gabpurmen.sHtML

[T14] Kotlin：循环
来源：http://mobile.sjlbkw.cn/Article/details/gqfhfitju.sHtML

for (i in 1..10) println(i)
来源：http://baike.bbcook.cn/Article/details/gbkuvmrar.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.bbcook.cn/Article/details/gqddmzepe.sHtML

interface Shape { fun area(): Double }
来源：http://baike.bbcook.cn/Article/details/gdkpoditc.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/ggyxalpuf.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/genrdzalq.sHtML

[T17] Swift：变量与常量
来源：http://wap.epnwcf.com/Article/details/gbfrlhzgz.sHtML

var a = 1;  let b = 2
来源：http://wap.fktsv.cn/Article/details/gfqwzvugm.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gejbxilmm.sHtML

"值: \(b)"
来源：http://www.blog.tarul.cn/Article/details/ghydpspbg.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fktsv.cn/Article/details/gjxfcqhdk.sHtML

if let n = opt { print(n) }
来源：http://www.share.epnwcf.com/Article/details/gdqblwauc.sHtML

[T20] Swift：数组操作
来源：http://3g.epnwcf.com/Article/details/gucchkxgm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.tarul.cn/Article/details/ggfghmfqn.sHtML

[T21] Swift：遍历
来源：http://3g.yfazqb.com/Article/details/gectvdacq.sHtML

for x in a { print(x) }
来源：http://www.blog.vehdjk.com/Article/details/gporthmil.sHtML

[T22] Swift：字典
来源：http://baike.bbcook.cn/Article/details/gyixztftq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.vehdjk.com/Article/details/gllvadebf.sHtML

[T23] Swift：函数
来源：http://mobile.fktsv.cn/Article/details/gcsbgmvxv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.yfazqb.com/Article/details/gdeoibekq.sHtML

[T24] Swift：闭包
来源：http://www.share.sjlbkw.cn/Article/details/galrvomod.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gnsombgul.sHtML

[T25] Swift：结构体
来源：http://3g.bbcook.cn/Article/details/gxzjeuznw.sHtML

struct P { var x: Int }
来源：http://www.share.bbcook.cn/Article/details/gxihuxpwr.sHtML

[T26] Swift：类与重写
来源：http://www.blog.tarul.cn/Article/details/gqstpznzf.sHtML

class A: Base { override func f() {} }
来源：http://m.share.yfazqb.com/Article/details/gkucpvhnm.sHtML

[T27] Swift：错误处理
来源：http://3g.epnwcf.com/Article/details/guhxrwyta.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.vehdjk.com/Article/details/gljafejee.sHtML

[T28] Swift：枚举
来源：http://wap.yfazqb.com/Article/details/gwwupftqt.sHtML

enum Color { case red, green }
来源：http://blog.fktsv.cn/Article/details/ggmsirxnj.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.tarul.cn/Article/details/gfjforiup.sHtML

guard let x = opt else { return }
来源：http://wap.bbcook.cn/Article/details/gmvsqxrtt.sHtML

[T30] Swift：协议
来源：http://www.share.yfazqb.com/Article/details/grjfucubx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.sjlbkw.cn/Article/details/gdssoyarl.sHtML

[T31] Lua：Hello World
来源：http://blog.tarul.cn/Article/details/ghtongbqd.sHtML

print("Hello")
来源：http://3g.tarul.cn/Article/details/gshsomagz.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.tarul.cn/Article/details/glzvkalel.sHtML

local a = 1
来源：http://baike.tarul.cn/Article/details/gpfnldwko.sHtML

[T33] Lua：表（数组）
来源：http://baike.yfazqb.com/Article/details/gattgmpsp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.vehdjk.com/Article/details/gxqejjxxl.sHtML

[T34] Lua：遍历表
来源：http://www.blog.vehdjk.com/Article/details/galhbwoji.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.tarul.cn/Article/details/gifpbnhsi.sHtML

[T35] Lua：字典表
来源：http://3g.yfazqb.com/Article/details/gujddkurv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.bbcook.cn/Article/details/gwhrfiqqz.sHtML

[T36] Lua：函数
来源：http://m.share.fktsv.cn/Article/details/gkahvgvvs.sHtML

function add(a, b) return a + b end
来源：http://wap.yfazqb.com/Article/details/gahwpkvai.sHtML

[T37] Lua：字符串拼接
来源：http://baike.sjlbkw.cn/Article/details/gyreizkxa.sHtML

"a" .. "b"
来源：http://m.share.tarul.cn/Article/details/gkndqtobi.sHtML

[T38] Lua：条件
来源：http://www.blog.vehdjk.com/Article/details/grydcnggs.sHtML

if x > 0 then print("正") end
来源：http://m.share.fktsv.cn/Article/details/giapweawc.sHtML

[T39] Lua：模式匹配
来源：http://baike.fktsv.cn/Article/details/gzhfvxlms.sHtML

string.find(s, "%d+")
来源：http://wap.fktsv.cn/Article/details/gvyhjgozb.sHtML

[T40] Lua：元表
来源：http://wap.epnwcf.com/Article/details/gnpsqtgss.sHtML

setmetatable({}, { __index = base })
来源：http://baike.tarul.cn/Article/details/gyrteogfl.sHtML

[T41] Perl：Hello World
来源：http://3g.fktsv.cn/Article/details/gqvzvncuc.sHtML

print "Hello\n";
来源：http://blog.epnwcf.com/Article/details/gvxfysdtn.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fktsv.cn/Article/details/gxdwqmmqx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.sjlbkw.cn/Article/details/gzhbgdwra.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gyukiwokl.sHtML

"值: $a"
来源：http://www.blog.fktsv.cn/Article/details/gtesfdbzz.sHtML

[T44] Perl：条件
来源：http://www.share.sjlbkw.cn/Article/details/goiqrsukz.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.sjlbkw.cn/Article/details/gqrjegahp.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gsyhitqcn.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.vehdjk.com/Article/details/grmnerryt.sHtML

[T46] Perl：哈希操作
来源：http://read.share.epnwcf.com/Article/details/gynzqfwsf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.tarul.cn/Article/details/gopsgfesa.sHtML

[T47] Perl：正则捕获
来源：http://read.share.sjlbkw.cn/Article/details/gljglqtbo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.vehdjk.com/Article/details/gqriduzjd.sHtML

[T48] Perl：正则替换
来源：http://baike.tarul.cn/Article/details/gdnmnober.sHtML

$s =~ s/old/new/g;
来源：http://mobile.sjlbkw.cn/Article/details/gikfhshun.sHtML

[T49] Perl：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gxbeoxweh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gkqfwrkzd.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fktsv.cn/Article/details/gfqhikrpk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.sjlbkw.cn/Article/details/girmgpxdb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.epnwcf.com/Article/details/gkagxding.sHtML

[T51] Scala：Hello World
来源：http://wap.fktsv.cn/Article/details/guzqodjzt.sHtML

println("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gdotgtvne.sHtML

[T52] Scala：变量
来源：http://blog.vehdjk.com/Article/details/gcuphfbvp.sHtML

val a = 1;  var b = 2
来源：http://m.share.fktsv.cn/Article/details/gnlvfgswq.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fktsv.cn/Article/details/geansvbsl.sHtML

s"值: $b"
来源：http://3g.bbcook.cn/Article/details/gfpkhzxid.sHtML

[T54] Scala：集合映射
来源：http://3g.sjlbkw.cn/Article/details/gnzesvnhe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.vehdjk.com/Article/details/gdxvekgbe.sHtML

[T55] Scala：集合过滤
来源：http://blog.epnwcf.com/Article/details/gydoxmhad.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.epnwcf.com/Article/details/gvpfxdmnw.sHtML

[T56] Scala：样例类
来源：http://www.blog.epnwcf.com/Article/details/gfnhixkfb.sHtML

case class User(name: String, age: Int)
来源：http://baike.tarul.cn/Article/details/gqidhrgtq.sHtML

[T57] Scala：模式匹配
来源：http://wap.fktsv.cn/Article/details/gegfwafap.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.yfazqb.com/Article/details/gnnrxicef.sHtML

[T58] Scala：函数定义
来源：http://m.share.sjlbkw.cn/Article/details/gnrhihhqq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.vehdjk.com/Article/details/gamunriuk.sHtML

[T59] Scala：循环
来源：http://read.share.vehdjk.com/Article/details/gihugdich.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fktsv.cn/Article/details/ggqlzelzg.sHtML

[T60] Scala：折叠
来源：http://read.share.sjlbkw.cn/Article/details/gixrglofj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.sjlbkw.cn/Article/details/gezkxkcpz.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gqxgoqziz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.epnwcf.com/Article/details/gxnwttguo.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gajoaszwf.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.bbcook.cn/Article/details/gxvfofcqj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.vehdjk.com/Article/details/grmjdgzvg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.sjlbkw.cn/Article/details/gfrjoyjop.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.vehdjk.com/Article/details/ggsmaoajw.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fktsv.cn/Article/details/gnpraynod.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.bbcook.cn/Article/details/grsiedsdr.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fktsv.cn/Article/details/gsvmsmanf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.bbcook.cn/Article/details/goalznfbb.sHtML

[U05] Py：列表去重且保序
来源：http://3g.tarul.cn/Article/details/guodqqttl.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/gvlinokmc.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gbixiahql.sHtML

{**a, **b}
来源：http://read.share.tarul.cn/Article/details/gjxrwhcsu.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.sjlbkw.cn/Article/details/gioxkuybv.sHtML

{v: k for k, v in d.items()}
来源：http://3g.epnwcf.com/Article/details/gtczxepmm.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.yfazqb.com/Article/details/gfrkwrfew.sHtML

[y for x in nested for y in x]
来源：http://www.share.tarul.cn/Article/details/gbpihcsoo.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.tarul.cn/Article/details/gtuwnrpey.sHtML

max(d, key=d.get)
来源：http://3g.tarul.cn/Article/details/gdapylccc.sHtML

[U10] Py：按值排序字典
来源：http://m.share.bbcook.cn/Article/details/gjmdvhhfm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.epnwcf.com/Article/details/guvytkitu.sHtML

[U11] Py：生成器表达式
来源：http://www.share.bbcook.cn/Article/details/gwuhrlcrk.sHtML

(x * 2 for x in arr)
来源：http://www.blog.yfazqb.com/Article/details/glwnucgtv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.tarul.cn/Article/details/gtcqdiisx.sHtML

Counter(arr).most_common(3)
来源：http://m.share.tarul.cn/Article/details/ggdhzziwj.sHtML

[U13] Py：固定长度队列
来源：http://3g.fktsv.cn/Article/details/gzmdeggaf.sHtML

deque(maxlen=10)
来源：http://3g.epnwcf.com/Article/details/gznzvxzux.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.bbcook.cn/Article/details/gtsoxddrp.sHtML

defaultdict(list)
来源：http://wap.tarul.cn/Article/details/gwpneejaf.sHtML

[U15] Py：高精度计时
来源：http://3g.tarul.cn/Article/details/giqbrjjkm.sHtML

t = time.perf_counter()
来源：http://www.share.vehdjk.com/Article/details/gzjxgkcym.sHtML

[U16] Py：命令行参数解析
来源：http://wap.yfazqb.com/Article/details/gxugszjgy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.bbcook.cn/Article/details/gazlkukdy.sHtML

[U17] Py：初始化日志
来源：http://www.share.fktsv.cn/Article/details/gdbzusclb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.yfazqb.com/Article/details/gcheisjpm.sHtML

[U18] Py：预编译正则
来源：http://baike.sjlbkw.cn/Article/details/gwbvponra.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.sjlbkw.cn/Article/details/gzxwcmxsz.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.vehdjk.com/Article/details/goiqzyukq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.bbcook.cn/Article/details/grtrlhjtb.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.vehdjk.com/Article/details/glbbxnjwc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.vehdjk.com/Article/details/gxwlwrtxg.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.sjlbkw.cn/Article/details/gjvuiegtk.sHtML

@contextlib.contextmanager
来源：http://wap.fktsv.cn/Article/details/gxwpubwda.sHtML

[U22] Py：矩阵转置
来源：http://baike.sjlbkw.cn/Article/details/gsdnkwwks.sHtML

list(zip(*m))
来源：http://m.share.tarul.cn/Article/details/gryjllngg.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.bbcook.cn/Article/details/gncfsxwqr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.tarul.cn/Article/details/gggupaxyy.sHtML

[U24] Py：路径操作
来源：http://3g.fktsv.cn/Article/details/gjolqhyzw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.vehdjk.com/Article/details/gmrkvqeey.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fktsv.cn/Article/details/gdojoglgp.sHtML

csv.DictReader(f)
来源：http://wap.sjlbkw.cn/Article/details/gvmsrwinc.sHtML

[U26] Py：并发下载
来源：http://blog.epnwcf.com/Article/details/glhwrolkn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.epnwcf.com/Article/details/genakyaqu.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.sjlbkw.cn/Article/details/gkxhcafdc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.sjlbkw.cn/Article/details/gxwtyhvlc.sHtML

[U28] Py：类型别名
来源：http://read.share.fktsv.cn/Article/details/gzfuxevsc.sHtML

UserId = int
来源：http://m.share.epnwcf.com/Article/details/gdrqwlzlp.sHtML

[U29] Py：属性校验
来源：http://3g.vehdjk.com/Article/details/gtdtnctue.sHtML

@property 与 @x.setter 配合
来源：http://www.share.tarul.cn/Article/details/gfyqwlpst.sHtML

[U30] Py：数据类
来源：http://wap.yfazqb.com/Article/details/ghisnimdv.sHtML

@dataclass(slots=True)
来源：http://mobile.epnwcf.com/Article/details/ggjoeanor.sHtML

[U31] Py：单测
来源：http://read.share.sjlbkw.cn/Article/details/glhfucvtc.sHtML

python -m pytest -q
来源：http://www.share.tarul.cn/Article/details/gnejniogp.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gixcprfbx.sHtML

ruff format . && ruff check --fix .
来源：http://3g.yfazqb.com/Article/details/gvztdvfac.sHtML

[U33] Py：打包发布
来源：http://3g.tarul.cn/Article/details/gfokmmcgb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.vehdjk.com/Article/details/gygggphjf.sHtML

[U34] Py：判断编码
来源：http://3g.sjlbkw.cn/Article/details/gfnanfafv.sHtML

chardet.detect(raw)
来源：http://www.blog.bbcook.cn/Article/details/glgmvnzvm.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.tarul.cn/Article/details/godknvrpn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.epnwcf.com/Article/details/gikibhfjb.sHtML

[U36] Py：定时任务
来源：http://blog.tarul.cn/Article/details/gsjbkdcie.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.bbcook.cn/Article/details/gtrfmzloq.sHtML

[U37] Py：读写 Excel
来源：http://blog.fktsv.cn/Article/details/gpwmwuiva.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.vehdjk.com/Article/details/gvkhoowid.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fktsv.cn/Article/details/gudemmykp.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.tarul.cn/Article/details/gepyvurrk.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.bbcook.cn/Article/details/gghuqvmiy.sHtML

sys.stdout.isatty()
来源：http://read.share.fktsv.cn/Article/details/gngpdnivd.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.tarul.cn/Article/details/gfhgjkixt.sHtML

print("err", file=sys.stderr)
来源：http://baike.epnwcf.com/Article/details/gptgsrgti.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.bbcook.cn/Article/details/gqarkjynd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.sjlbkw.cn/Article/details/gjklmmbmn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.sjlbkw.cn/Article/details/gjchwgeay.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.epnwcf.com/Article/details/gnysdiosr.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fktsv.cn/Article/details/gqhygmlag.sHtML

namespace App\Http;
来源：http://3g.bbcook.cn/Article/details/gvixmsmla.sHtML

[U44] PHP：开启严格类型
来源：http://3g.epnwcf.com/Article/details/gkkvgcpcq.sHtML

declare(strict_types=1);
来源：http://mobile.fktsv.cn/Article/details/gsxnngmuv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.tarul.cn/Article/details/giukovuio.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gznrxemne.sHtML

[U46] PHP：可空类型
来源：http://www.share.sjlbkw.cn/Article/details/gxqatnbzw.sHtML

?string $name = null
来源：http://www.blog.fktsv.cn/Article/details/gomdcoufz.sHtML

[U47] PHP：联合类型
来源：http://www.blog.yfazqb.com/Article/details/ghxeiolgo.sHtML

int|string $id
来源：http://baike.vehdjk.com/Article/details/gwdjcuhmq.sHtML

[U48] PHP：纯枚举
来源：http://3g.vehdjk.com/Article/details/gcnqzeogk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcwueoqfr.sHtML

[U49] PHP：只读属性
来源：http://www.share.tarul.cn/Article/details/gxlxpflau.sHtML

public readonly string $name
来源：http://wap.yfazqb.com/Article/details/gkwnvwbnp.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.tarul.cn/Article/details/grtpvfgrv.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.bbcook.cn/Article/details/gyljcfzhy.sHtML

[U51] PHP：数组解构
来源：http://blog.fktsv.cn/Article/details/gbhronymg.sHtML

[$a, $b] = $arr;
来源：http://www.blog.vehdjk.com/Article/details/gygndoitx.sHtML

[U52] PHP：箭头函数
来源：http://wap.fktsv.cn/Article/details/gooivsnii.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fktsv.cn/Article/details/gfmxyunea.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.sjlbkw.cn/Article/details/gzqbvrcsb.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fktsv.cn/Article/details/gpyymvhaq.sHtML

[U54] PHP：空安全调用
来源：http://m.share.sjlbkw.cn/Article/details/gnkeqfvzl.sHtML

$obj?->method()
来源：http://read.share.vehdjk.com/Article/details/gdcrqivli.sHtML

[U55] PHP：match 表达式
来源：http://read.share.tarul.cn/Article/details/gkdlkbaah.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.sjlbkw.cn/Article/details/gfgjsxfot.sHtML

[U56] PHP：命名参数
来源：http://www.blog.sjlbkw.cn/Article/details/gvqbvwptz.sHtML

f(a: 1, b: 2)
来源：http://baike.epnwcf.com/Article/details/gltutpgyb.sHtML

[U57] PHP：字符串插值
来源：http://3g.yfazqb.com/Article/details/goeuvbsvs.sHtML

"值: {$a}"
来源：http://read.share.sjlbkw.cn/Article/details/gcgtjwkfu.sHtML

[U58] PHP：数组三件套
来源：http://wap.fktsv.cn/Article/details/gujjbiitw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fktsv.cn/Article/details/gqryqaaoz.sHtML


<!-- 参考信息 -->