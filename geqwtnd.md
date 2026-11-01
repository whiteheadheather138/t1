代发 wailian999

[S37] C++：set
来源：http://baike.fktsv.cn/Article/details/gxzikxpwh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.vehdjk.com/Article/details/gxahusbnq.sHtML

[S38] C++：排序
来源：http://blog.epnwcf.com/Article/details/gwucieowv.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.epnwcf.com/Article/details/gtbwuaoiy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.epnwcf.com/Article/details/grkncgtan.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.vehdjk.com/Article/details/ghgzqwilk.sHtML

[S40] C++：查找元素
来源：http://read.share.epnwcf.com/Article/details/gcfxgvpyg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fktsv.cn/Article/details/gfspxzalm.sHtML

[S41] C++：类与构造函数
来源：http://baike.tarul.cn/Article/details/gytkcfxyh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.bbcook.cn/Article/details/gjxxxavoc.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.vehdjk.com/Article/details/gsbgnistp.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fktsv.cn/Article/details/gbvmtmgok.sHtML

[S43] C++：智能指针
来源：http://3g.epnwcf.com/Article/details/ghesbhaig.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.bbcook.cn/Article/details/gzelrplgk.sHtML

[S44] C++：引用传参
来源：http://baike.yfazqb.com/Article/details/gtmatgurq.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fktsv.cn/Article/details/grzjyrwjr.sHtML

[S45] C++：lambda
来源：http://mobile.tarul.cn/Article/details/ghyhfhkuz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.sjlbkw.cn/Article/details/gdlhhrmkc.sHtML

[S46] C++：函数模板
来源：http://wap.tarul.cn/Article/details/gjuwuzrpg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.epnwcf.com/Article/details/gcyamgkbb.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.vehdjk.com/Article/details/gahypjexe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.yfazqb.com/Article/details/gkrjyjveq.sHtML

[S48] C++：逐行读文件
来源：http://blog.fktsv.cn/Article/details/glbxtzbgp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.tarul.cn/Article/details/gspqvczyj.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.epnwcf.com/Article/details/gnvwfaspy.sHtML

[S49] C++：写文件
来源：http://m.share.yfazqb.com/Article/details/gxjrultgd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.sjlbkw.cn/Article/details/gqmogcrei.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fktsv.cn/Article/details/gagvuisub.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.epnwcf.com/Article/details/gyfhjioqp.sHtML

[S51] C++：显式类型转换
来源：http://m.share.sjlbkw.cn/Article/details/gejowotoz.sHtML

static_cast<double>(a) / b
来源：http://m.share.yfazqb.com/Article/details/gqvuhcohx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fktsv.cn/Article/details/gaomoqydn.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fktsv.cn/Article/details/gpempxbyj.sHtML

[S53] C++：移动语义
来源：http://www.m.share.yfazqb.com/Article/details/gxepkaltf.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.tarul.cn/Article/details/geujsabbp.sHtML

[S54] C++：异常处理
来源：http://blog.vehdjk.com/Article/details/goxjberya.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.sjlbkw.cn/Article/details/gxbhyfrzz.sHtML

[S55] C++：结构化绑定
来源：http://baike.tarul.cn/Article/details/gsswpkpwu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.tarul.cn/Article/details/grnvqnsqc.sHtML

[S56] C++：optional
来源：http://read.share.yfazqb.com/Article/details/grfhslfcj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.sjlbkw.cn/Article/details/ggkumujmo.sHtML

[S57] C++：编译期常量
来源：http://3g.sjlbkw.cn/Article/details/gyocvhdlx.sHtML

constexpr int N = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsdyzkbj.sHtML

[S58] C++：命名空间
来源：http://www.share.yfazqb.com/Article/details/gndopxlrg.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fktsv.cn/Article/details/gfmlpjxtq.sHtML

[S59] C++：静态断言
来源：http://www.blog.epnwcf.com/Article/details/gydeqvbyq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.bbcook.cn/Article/details/gaxndgwmj.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.vehdjk.com/Article/details/gkcpfqvca.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.vehdjk.com/Article/details/gxluteygx.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gqyfbosdh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.tarul.cn/Article/details/gjzcripdu.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/guwleldcy.sHtML

[T01] Kotlin：Hello World
来源：http://3g.vehdjk.com/Article/details/gqmfkcuux.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/giqgtkqnm.sHtML

[T02] Kotlin：变量
来源：http://baike.sjlbkw.cn/Article/details/gevrztpzh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.bbcook.cn/Article/details/gifacxwcv.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.epnwcf.com/Article/details/gdoaciebr.sHtML

"值: $b"
来源：http://www.share.epnwcf.com/Article/details/gzmnrkcwp.sHtML

[T04] Kotlin：空安全
来源：http://www.share.bbcook.cn/Article/details/gujrckfrm.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fktsv.cn/Article/details/guplkwpjx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.epnwcf.com/Article/details/gfazkqloe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.yfazqb.com/Article/details/giqntnlal.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.bbcook.cn/Article/details/gomnrcric.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fktsv.cn/Article/details/ghiplxzfd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.tarul.cn/Article/details/ghisakemh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.epnwcf.com/Article/details/gscfvmhqg.sHtML

[T08] Kotlin：数据类
来源：http://wap.sjlbkw.cn/Article/details/gnkglrqsc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.yfazqb.com/Article/details/gbiknoikv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.yfazqb.com/Article/details/gqrhwrqkl.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.sjlbkw.cn/Article/details/gosdxvmvd.sHtML

[T10] Kotlin：默认参数
来源：http://blog.yfazqb.com/Article/details/gaghqiqyl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fktsv.cn/Article/details/gvupgynmc.sHtML

[T11] Kotlin：协程
来源：http://www.blog.tarul.cn/Article/details/gjfhcdaci.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.sjlbkw.cn/Article/details/guhfethvn.sHtML

[T12] Kotlin：解构声明
来源：http://wap.epnwcf.com/Article/details/gfkkszvgh.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gapkoascm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fktsv.cn/Article/details/gmhdqkxue.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.tarul.cn/Article/details/glnxqimdy.sHtML

[T14] Kotlin：循环
来源：http://m.share.bbcook.cn/Article/details/gfjzjeqnk.sHtML

for (i in 1..10) println(i)
来源：http://mobile.epnwcf.com/Article/details/gociascpa.sHtML

[T15] Kotlin：接口
来源：http://baike.epnwcf.com/Article/details/gtrjyxptr.sHtML

interface Shape { fun area(): Double }
来源：http://blog.vehdjk.com/Article/details/grtypxbuf.sHtML

[T16] Swift：Hello World
来源：http://read.share.vehdjk.com/Article/details/gskyilxjf.sHtML

print("Hello")
来源：http://m.share.yfazqb.com/Article/details/ggzpngmdj.sHtML

[T17] Swift：变量与常量
来源：http://read.share.vehdjk.com/Article/details/grnmolojb.sHtML

var a = 1;  let b = 2
来源：http://www.blog.yfazqb.com/Article/details/gklbsckvc.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gzspnakja.sHtML

"值: \(b)"
来源：http://wap.fktsv.cn/Article/details/gwdlzniai.sHtML

[T19] Swift：可选绑定
来源：http://baike.yfazqb.com/Article/details/gacpvmkuc.sHtML

if let n = opt { print(n) }
来源：http://baike.sjlbkw.cn/Article/details/gunenvhyr.sHtML

[T20] Swift：数组操作
来源：http://read.share.epnwcf.com/Article/details/gepthbksx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.tarul.cn/Article/details/gvkvovcfr.sHtML

[T21] Swift：遍历
来源：http://wap.yfazqb.com/Article/details/gadcfnwac.sHtML

for x in a { print(x) }
来源：http://3g.bbcook.cn/Article/details/gxviesfwm.sHtML

[T22] Swift：字典
来源：http://www.blog.yfazqb.com/Article/details/gooqazgpc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.yfazqb.com/Article/details/gdjwjfnkk.sHtML

[T23] Swift：函数
来源：http://3g.epnwcf.com/Article/details/gvndufmex.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.yfazqb.com/Article/details/gvinkiyfe.sHtML

[T24] Swift：闭包
来源：http://www.share.tarul.cn/Article/details/ggfssvzxk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.tarul.cn/Article/details/gbgyjxgmr.sHtML

[T25] Swift：结构体
来源：http://wap.yfazqb.com/Article/details/gqdvhojof.sHtML

struct P { var x: Int }
来源：http://m.share.yfazqb.com/Article/details/glfbuiluw.sHtML

[T26] Swift：类与重写
来源：http://wap.fktsv.cn/Article/details/girxhecrt.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.vehdjk.com/Article/details/gxsqmkccf.sHtML

[T27] Swift：错误处理
来源：http://www.share.epnwcf.com/Article/details/gdjcvibum.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fktsv.cn/Article/details/gmpmwtejq.sHtML

[T28] Swift：枚举
来源：http://mobile.sjlbkw.cn/Article/details/gdwdozfuw.sHtML

enum Color { case red, green }
来源：http://m.share.yfazqb.com/Article/details/goxbrkctx.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.tarul.cn/Article/details/gmxvmtagv.sHtML

guard let x = opt else { return }
来源：http://read.share.bbcook.cn/Article/details/gtiegnwxl.sHtML

[T30] Swift：协议
来源：http://m.share.epnwcf.com/Article/details/glkvbtiqk.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.bbcook.cn/Article/details/gkmurhmnz.sHtML

[T31] Lua：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gvyxdftkh.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/gknqxpxwt.sHtML

[T32] Lua：局部变量
来源：http://read.share.fktsv.cn/Article/details/ghcnbpgjn.sHtML

local a = 1
来源：http://read.share.yfazqb.com/Article/details/gjqhtntpt.sHtML

[T33] Lua：表（数组）
来源：http://wap.tarul.cn/Article/details/goqzwsrdh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.tarul.cn/Article/details/gdqjfjhgq.sHtML

[T34] Lua：遍历表
来源：http://read.share.bbcook.cn/Article/details/gevnxfmhp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.epnwcf.com/Article/details/gzgimuowq.sHtML

[T35] Lua：字典表
来源：http://read.share.epnwcf.com/Article/details/gxeldsvmo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.yfazqb.com/Article/details/gymvepuqr.sHtML

[T36] Lua：函数
来源：http://m.share.sjlbkw.cn/Article/details/glxsbyito.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fktsv.cn/Article/details/glrujttkw.sHtML

[T37] Lua：字符串拼接
来源：http://baike.yfazqb.com/Article/details/gsiomqowq.sHtML

"a" .. "b"
来源：http://read.share.fktsv.cn/Article/details/gmzbdwjpi.sHtML

[T38] Lua：条件
来源：http://read.share.fktsv.cn/Article/details/gmnldatis.sHtML

if x > 0 then print("正") end
来源：http://read.share.yfazqb.com/Article/details/gkqvbmqgh.sHtML

[T39] Lua：模式匹配
来源：http://mobile.bbcook.cn/Article/details/gxdekkomg.sHtML

string.find(s, "%d+")
来源：http://m.share.vehdjk.com/Article/details/gkotemtnj.sHtML

[T40] Lua：元表
来源：http://m.share.sjlbkw.cn/Article/details/ghmawjtkg.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.bbcook.cn/Article/details/gdmmcvyho.sHtML

[T41] Perl：Hello World
来源：http://read.share.tarul.cn/Article/details/gbrvjqtqe.sHtML

print "Hello\n";
来源：http://baike.yfazqb.com/Article/details/gwtkazdhf.sHtML

[T42] Perl：变量类型
来源：http://wap.tarul.cn/Article/details/gmkhyuzjb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.epnwcf.com/Article/details/gdphkwvhl.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gebiqhmgk.sHtML

"值: $a"
来源：http://blog.bbcook.cn/Article/details/glheksffk.sHtML

[T44] Perl：条件
来源：http://www.m.share.epnwcf.com/Article/details/gxwejmfvr.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.sjlbkw.cn/Article/details/gfskzpoid.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.tarul.cn/Article/details/gypydjmgh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.epnwcf.com/Article/details/gawlnerti.sHtML

[T46] Perl：哈希操作
来源：http://blog.fktsv.cn/Article/details/ggukeopwn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.epnwcf.com/Article/details/gehsoslof.sHtML

[T47] Perl：正则捕获
来源：http://baike.vehdjk.com/Article/details/ghqhrgloo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.vehdjk.com/Article/details/gnvicnnwo.sHtML

[T48] Perl：正则替换
来源：http://m.share.sjlbkw.cn/Article/details/gncvcnhna.sHtML

$s =~ s/old/new/g;
来源：http://m.share.yfazqb.com/Article/details/gzagravjx.sHtML

[T49] Perl：函数
来源：http://wap.yfazqb.com/Article/details/gjpwsxvzo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gugvogdih.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.epnwcf.com/Article/details/gluevibzd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.yfazqb.com/Article/details/gibxnxywi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.sjlbkw.cn/Article/details/gcszwrgpy.sHtML

[T51] Scala：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/guqiktmeu.sHtML

println("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzjpqotu.sHtML

[T52] Scala：变量
来源：http://blog.bbcook.cn/Article/details/gjmmtaesd.sHtML

val a = 1;  var b = 2
来源：http://m.share.yfazqb.com/Article/details/gmprgpjho.sHtML

[T53] Scala：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gfwzolasa.sHtML

s"值: $b"
来源：http://3g.fktsv.cn/Article/details/gagfasrtf.sHtML

[T54] Scala：集合映射
来源：http://www.blog.epnwcf.com/Article/details/ghstnatxt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.sjlbkw.cn/Article/details/gvlvicosi.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fktsv.cn/Article/details/gexepnvzn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.vehdjk.com/Article/details/gauikxbqz.sHtML

[T56] Scala：样例类
来源：http://www.share.epnwcf.com/Article/details/gxnghsbpf.sHtML

case class User(name: String, age: Int)
来源：http://m.share.bbcook.cn/Article/details/gorfjnzav.sHtML

[T57] Scala：模式匹配
来源：http://3g.bbcook.cn/Article/details/gywhvzdqe.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.epnwcf.com/Article/details/gqmgxyome.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gccurpuqx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fktsv.cn/Article/details/geebpkbeu.sHtML

[T59] Scala：循环
来源：http://baike.fktsv.cn/Article/details/gylldgghc.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.vehdjk.com/Article/details/gvcnqdqdt.sHtML

[T60] Scala：折叠
来源：http://m.share.vehdjk.com/Article/details/gcsckguod.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.yfazqb.com/Article/details/gxpvaobpw.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/glonfwril.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.tarul.cn/Article/details/gpvjrzmse.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gflcvahgj.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.yfazqb.com/Article/details/gqhpcznjm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fktsv.cn/Article/details/grxqqpfwy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fktsv.cn/Article/details/gcphlzmqb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.yfazqb.com/Article/details/gcsmfmvra.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.tarul.cn/Article/details/gcqqjoqpx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.bbcook.cn/Article/details/gwwadxydx.sHtML

[U04] Py：变量调试打印
来源：http://www.share.yfazqb.com/Article/details/gjgjzhlyx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.tarul.cn/Article/details/ggqcvpycl.sHtML

[U05] Py：列表去重且保序
来源：http://baike.epnwcf.com/Article/details/gdjtohbdh.sHtML

list(dict.fromkeys(arr))
来源：http://blog.yfazqb.com/Article/details/gjnjluhyc.sHtML

[U06] Py：合并两个字典
来源：http://mobile.yfazqb.com/Article/details/gkfoepyuq.sHtML

{**a, **b}
来源：http://mobile.bbcook.cn/Article/details/gypcggzop.sHtML

[U07] Py：反转字典键值
来源：http://mobile.epnwcf.com/Article/details/gsrvqyzxy.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.vehdjk.com/Article/details/gnwpuxtzp.sHtML

[U08] Py：展平二维列表
来源：http://3g.sjlbkw.cn/Article/details/gwmlktgwb.sHtML

[y for x in nested for y in x]
来源：http://read.share.bbcook.cn/Article/details/ggkhbbdvs.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.sjlbkw.cn/Article/details/gpmvaaefc.sHtML

max(d, key=d.get)
来源：http://www.blog.yfazqb.com/Article/details/gcjeyyvyf.sHtML

[U10] Py：按值排序字典
来源：http://baike.sjlbkw.cn/Article/details/guzaxupiw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.sjlbkw.cn/Article/details/gcuxahnva.sHtML

[U11] Py：生成器表达式
来源：http://read.share.vehdjk.com/Article/details/ghiwsbtzi.sHtML

(x * 2 for x in arr)
来源：http://baike.bbcook.cn/Article/details/grruhrxcy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.epnwcf.com/Article/details/gifkakkef.sHtML

Counter(arr).most_common(3)
来源：http://m.share.vehdjk.com/Article/details/gguggjgru.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fktsv.cn/Article/details/gijujusvb.sHtML

deque(maxlen=10)
来源：http://baike.fktsv.cn/Article/details/gpmpziglp.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.epnwcf.com/Article/details/gyzrhjqgi.sHtML

defaultdict(list)
来源：http://blog.bbcook.cn/Article/details/grvpjjkzt.sHtML

[U15] Py：高精度计时
来源：http://www.share.bbcook.cn/Article/details/gpskmkezc.sHtML

t = time.perf_counter()
来源：http://www.blog.tarul.cn/Article/details/gdtfkxhlg.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fktsv.cn/Article/details/gajrzcjne.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fktsv.cn/Article/details/gxyepelze.sHtML

[U17] Py：初始化日志
来源：http://baike.vehdjk.com/Article/details/gwizmmcld.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.sjlbkw.cn/Article/details/gtdekohpi.sHtML

[U18] Py：预编译正则
来源：http://wap.yfazqb.com/Article/details/ggddsvdke.sHtML

pat = re.compile(r"\d+")
来源：http://wap.vehdjk.com/Article/details/gfdyvqaxb.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.tarul.cn/Article/details/gqwfhdpdc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.sjlbkw.cn/Article/details/gbaugueha.sHtML

[U20] Py：缓存函数结果
来源：http://wap.epnwcf.com/Article/details/gpmmtrffh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fktsv.cn/Article/details/gfrrreasx.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.epnwcf.com/Article/details/ghhseucun.sHtML

@contextlib.contextmanager
来源：http://www.blog.vehdjk.com/Article/details/gnlkitahh.sHtML

[U22] Py：矩阵转置
来源：http://3g.bbcook.cn/Article/details/gofqtagbp.sHtML

list(zip(*m))
来源：http://baike.bbcook.cn/Article/details/gkrmafvdt.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqioegcb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.sjlbkw.cn/Article/details/grwbkizwb.sHtML

[U24] Py：路径操作
来源：http://read.share.yfazqb.com/Article/details/gqvgsznop.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/gzjirhavj.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.bbcook.cn/Article/details/gnawsuyrz.sHtML

csv.DictReader(f)
来源：http://mobile.epnwcf.com/Article/details/gjfjxmssk.sHtML

[U26] Py：并发下载
来源：http://baike.fktsv.cn/Article/details/gsthwpnet.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.bbcook.cn/Article/details/gtaoongwy.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.bbcook.cn/Article/details/gvhnanezn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.bbcook.cn/Article/details/gmralmagp.sHtML

[U28] Py：类型别名
来源：http://blog.vehdjk.com/Article/details/gglmakcwn.sHtML

UserId = int
来源：http://3g.epnwcf.com/Article/details/gphcqzsbr.sHtML

[U29] Py：属性校验
来源：http://www.share.bbcook.cn/Article/details/gjwptpvuj.sHtML

@property 与 @x.setter 配合
来源：http://blog.vehdjk.com/Article/details/gstofpqnh.sHtML

[U30] Py：数据类
来源：http://blog.fktsv.cn/Article/details/gjuruvpjb.sHtML

@dataclass(slots=True)
来源：http://www.m.share.yfazqb.com/Article/details/gutbnukat.sHtML

[U31] Py：单测
来源：http://m.share.yfazqb.com/Article/details/gcqvpojox.sHtML

python -m pytest -q
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtqowibc.sHtML

[U32] Py：代码格式化
来源：http://www.share.fktsv.cn/Article/details/gzwonuuuj.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.tarul.cn/Article/details/gthhnwfni.sHtML

[U33] Py：打包发布
来源：http://www.blog.epnwcf.com/Article/details/gxhucbvgs.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.yfazqb.com/Article/details/gwavgtkml.sHtML

[U34] Py：判断编码
来源：http://blog.vehdjk.com/Article/details/guysbropd.sHtML

chardet.detect(raw)
来源：http://www.share.vehdjk.com/Article/details/gwzswreco.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.epnwcf.com/Article/details/gcafnbfqf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.epnwcf.com/Article/details/gjwfoldvv.sHtML

[U36] Py：定时任务
来源：http://baike.sjlbkw.cn/Article/details/gqteopsnx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fktsv.cn/Article/details/gxdfggeft.sHtML

[U37] Py：读写 Excel
来源：http://www.share.yfazqb.com/Article/details/gderparmy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.tarul.cn/Article/details/gkdwybvhu.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.tarul.cn/Article/details/gpcyqkbdc.sHtML

Path(__file__).resolve().parent
来源：http://baike.vehdjk.com/Article/details/gtyqcbqsp.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.vehdjk.com/Article/details/guuxfasbh.sHtML

sys.stdout.isatty()
来源：http://www.share.yfazqb.com/Article/details/ghhcuzdtm.sHtML

[U40] Py：打印到标准错误
来源：http://wap.yfazqb.com/Article/details/grtnbustb.sHtML

print("err", file=sys.stderr)
来源：http://m.share.tarul.cn/Article/details/gfhggyewy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.bbcook.cn/Article/details/gjqymvchl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.bbcook.cn/Article/details/gcwoyztdo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.sjlbkw.cn/Article/details/gwvuvjtoj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.sjlbkw.cn/Article/details/gxqojdbqv.sHtML

[U43] PHP：声明命名空间
来源：http://blog.vehdjk.com/Article/details/goecqzlfp.sHtML

namespace App\Http;
来源：http://blog.epnwcf.com/Article/details/ghvthynhm.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.yfazqb.com/Article/details/ggwdmknyq.sHtML

declare(strict_types=1);
来源：http://www.blog.yfazqb.com/Article/details/gaifmzlcd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.bbcook.cn/Article/details/gwwrajvhl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gkbdfaewx.sHtML

[U46] PHP：可空类型
来源：http://wap.yfazqb.com/Article/details/gvvbnrntu.sHtML

?string $name = null
来源：http://wap.yfazqb.com/Article/details/gatpqzdfs.sHtML

[U47] PHP：联合类型
来源：http://wap.vehdjk.com/Article/details/gjubnrivc.sHtML

int|string $id
来源：http://m.share.fktsv.cn/Article/details/geywgkbzl.sHtML

[U48] PHP：纯枚举
来源：http://read.share.tarul.cn/Article/details/gythjfzhr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.vehdjk.com/Article/details/gvxoiwmcp.sHtML

[U49] PHP：只读属性
来源：http://blog.yfazqb.com/Article/details/gopwsznzg.sHtML

public readonly string $name
来源：http://baike.fktsv.cn/Article/details/gnfgczith.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.bbcook.cn/Article/details/gzqedkxaq.sHtML

public function __construct(private int $id) {}
来源：http://wap.bbcook.cn/Article/details/gjvjzavoe.sHtML

[U51] PHP：数组解构
来源：http://www.blog.sjlbkw.cn/Article/details/gktkszegx.sHtML

[$a, $b] = $arr;
来源：http://wap.bbcook.cn/Article/details/gojhwpfgl.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.tarul.cn/Article/details/gpbuqmkqm.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fktsv.cn/Article/details/gmpakotqx.sHtML

[U53] PHP：空合并运算符
来源：http://wap.bbcook.cn/Article/details/gaopsmgqw.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.sjlbkw.cn/Article/details/gporgqtyu.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.vehdjk.com/Article/details/gryexohyj.sHtML

$obj?->method()
来源：http://www.blog.epnwcf.com/Article/details/ghqpurwvp.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gzycnwrwp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.sjlbkw.cn/Article/details/gwmgvkuxd.sHtML

[U56] PHP：命名参数
来源：http://read.share.yfazqb.com/Article/details/gmwhfikuq.sHtML

f(a: 1, b: 2)
来源：http://3g.fktsv.cn/Article/details/ginosolsk.sHtML

[U57] PHP：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gunfnxbvt.sHtML

"值: {$a}"
来源：http://wap.sjlbkw.cn/Article/details/gzkmjvzyx.sHtML

[U58] PHP：数组三件套
来源：http://www.share.epnwcf.com/Article/details/ghcsgmloi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fktsv.cn/Article/details/gqfffcxus.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmwpkdkf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.epnwcf.com/Article/details/gggzzsbih.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.yfazqb.com/Article/details/gbzywwvua.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.sjlbkw.cn/Article/details/gvrghoadi.sHtML

[U61] PHP：正则
来源：http://3g.bbcook.cn/Article/details/gsgaaabqd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.vehdjk.com/Article/details/gskplnnib.sHtML

[U62] PHP：日期对象
来源：http://mobile.bbcook.cn/Article/details/gwqyshlat.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.yfazqb.com/Article/details/gebscxyro.sHtML


<!-- 参考信息 -->