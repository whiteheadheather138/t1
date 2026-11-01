代发 wailian999

[S37] C++：set
来源：http://read.share.bbcook.cn/Article/details/gjtsttdzl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.bbcook.cn/Article/details/grhsqtoxh.sHtML

[S38] C++：排序
来源：http://read.share.bbcook.cn/Article/details/gioupsuzz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fktsv.cn/Article/details/ggbcmsuzl.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.bbcook.cn/Article/details/goghprecm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.epnwcf.com/Article/details/gkrzdjsnm.sHtML

[S40] C++：查找元素
来源：http://www.share.vehdjk.com/Article/details/gghapmmrm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.epnwcf.com/Article/details/gghtcqlhd.sHtML

[S41] C++：类与构造函数
来源：http://www.share.yfazqb.com/Article/details/gwhrotbwf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.yfazqb.com/Article/details/gtksagndf.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.sjlbkw.cn/Article/details/gokjmljfu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.yfazqb.com/Article/details/gmkzydduu.sHtML

[S43] C++：智能指针
来源：http://3g.bbcook.cn/Article/details/gerarnebu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.yfazqb.com/Article/details/gcpeopxxg.sHtML

[S44] C++：引用传参
来源：http://read.share.bbcook.cn/Article/details/gjktyzpno.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.bbcook.cn/Article/details/gycnztvbp.sHtML

[S45] C++：lambda
来源：http://baike.vehdjk.com/Article/details/gncslddez.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.bbcook.cn/Article/details/gkpywgnxl.sHtML

[S46] C++：函数模板
来源：http://m.share.sjlbkw.cn/Article/details/ghzmwefbt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fktsv.cn/Article/details/gahfqjgpy.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.bbcook.cn/Article/details/gkikymadu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.sjlbkw.cn/Article/details/gffumnkzp.sHtML

[S48] C++：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gsvfnuzik.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.bbcook.cn/Article/details/gkmxhixip.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.yfazqb.com/Article/details/gregpvvku.sHtML

[S49] C++：写文件
来源：http://m.share.fktsv.cn/Article/details/gjtafokyd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.vehdjk.com/Article/details/gjkmpokla.sHtML

[S50] C++：格式化数字
来源：http://blog.tarul.cn/Article/details/ggzqlubss.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.tarul.cn/Article/details/gbrjihsoz.sHtML

[S51] C++：显式类型转换
来源：http://3g.epnwcf.com/Article/details/gowkaaelo.sHtML

static_cast<double>(a) / b
来源：http://3g.fktsv.cn/Article/details/gintnykqi.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.bbcook.cn/Article/details/gabufxrjf.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.sjlbkw.cn/Article/details/gmzjqxybq.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fktsv.cn/Article/details/gjkytdxvq.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.yfazqb.com/Article/details/gizopwcad.sHtML

[S54] C++：异常处理
来源：http://www.share.epnwcf.com/Article/details/gmpxensws.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.bbcook.cn/Article/details/gslvdcnzt.sHtML

[S55] C++：结构化绑定
来源：http://mobile.vehdjk.com/Article/details/gdyvvpakb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.vehdjk.com/Article/details/gbmfbhpug.sHtML

[S56] C++：optional
来源：http://m.share.vehdjk.com/Article/details/gmiacncdd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.yfazqb.com/Article/details/gfqzuctsk.sHtML

[S57] C++：编译期常量
来源：http://www.share.bbcook.cn/Article/details/gsevfiwtd.sHtML

constexpr int N = 10;
来源：http://www.blog.fktsv.cn/Article/details/ggondwlsb.sHtML

[S58] C++：命名空间
来源：http://read.share.tarul.cn/Article/details/gwwsltrma.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.tarul.cn/Article/details/gnbrhkkjy.sHtML

[S59] C++：静态断言
来源：http://mobile.vehdjk.com/Article/details/glkoxvgqj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.vehdjk.com/Article/details/gbagjszrc.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.vehdjk.com/Article/details/gnwksswqu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.tarul.cn/Article/details/gbupctupw.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gclxblvhf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.vehdjk.com/Article/details/gizanhdgq.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/guixtpeie.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.epnwcf.com/Article/details/glsvlbugn.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/glkshialn.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.vehdjk.com/Article/details/gipcveowh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.tarul.cn/Article/details/gnmwjeeed.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.yfazqb.com/Article/details/gpxnzyadu.sHtML

"值: $b"
来源：http://www.m.share.fktsv.cn/Article/details/gbxikuepx.sHtML

[T04] Kotlin：空安全
来源：http://baike.sjlbkw.cn/Article/details/gvoltabna.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fktsv.cn/Article/details/gjmekdzws.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.bbcook.cn/Article/details/gtoedkryp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.vehdjk.com/Article/details/gkbkdodul.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.epnwcf.com/Article/details/gmerfcdql.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.yfazqb.com/Article/details/gpedpvaqx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.tarul.cn/Article/details/gpskcznqv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fktsv.cn/Article/details/ggmebypdm.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.vehdjk.com/Article/details/gaetqlxxx.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.vehdjk.com/Article/details/gdosatlrp.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.vehdjk.com/Article/details/gioawkwif.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.epnwcf.com/Article/details/gmsxbovmz.sHtML

[T10] Kotlin：默认参数
来源：http://wap.yfazqb.com/Article/details/gjzdbmmft.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.tarul.cn/Article/details/gfvneesgs.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlsnpukp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.vehdjk.com/Article/details/gleedgnav.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.vehdjk.com/Article/details/gcfjkdlnr.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.yfazqb.com/Article/details/gdimswhek.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.tarul.cn/Article/details/geudrethz.sHtML

val m = mapOf("a" to 1)
来源：http://blog.yfazqb.com/Article/details/gndxrbpet.sHtML

[T14] Kotlin：循环
来源：http://3g.fktsv.cn/Article/details/gsmosfiqw.sHtML

for (i in 1..10) println(i)
来源：http://3g.fktsv.cn/Article/details/gbwmfsyeo.sHtML

[T15] Kotlin：接口
来源：http://read.share.yfazqb.com/Article/details/gdiplzdwn.sHtML

interface Shape { fun area(): Double }
来源：http://blog.yfazqb.com/Article/details/gyqwllqjf.sHtML

[T16] Swift：Hello World
来源：http://wap.tarul.cn/Article/details/gwxlqdjjr.sHtML

print("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/galxlfpaa.sHtML

[T17] Swift：变量与常量
来源：http://wap.tarul.cn/Article/details/gdletkmgu.sHtML

var a = 1;  let b = 2
来源：http://www.blog.tarul.cn/Article/details/ghxvtdcdb.sHtML

[T18] Swift：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gymxqwkey.sHtML

"值: \(b)"
来源：http://m.share.bbcook.cn/Article/details/gohnqzwhr.sHtML

[T19] Swift：可选绑定
来源：http://www.share.vehdjk.com/Article/details/gkckhhnnh.sHtML

if let n = opt { print(n) }
来源：http://mobile.tarul.cn/Article/details/gzkhepord.sHtML

[T20] Swift：数组操作
来源：http://read.share.fktsv.cn/Article/details/gqnwjftjm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.tarul.cn/Article/details/gflfgpmiu.sHtML

[T21] Swift：遍历
来源：http://blog.epnwcf.com/Article/details/geollyuis.sHtML

for x in a { print(x) }
来源：http://mobile.yfazqb.com/Article/details/gcignrigr.sHtML

[T22] Swift：字典
来源：http://www.share.sjlbkw.cn/Article/details/golmcycvc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.tarul.cn/Article/details/gisuikroj.sHtML

[T23] Swift：函数
来源：http://www.share.sjlbkw.cn/Article/details/gbiayanfw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.bbcook.cn/Article/details/gdokucfgl.sHtML

[T24] Swift：闭包
来源：http://wap.bbcook.cn/Article/details/grxqrsism.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gtciafaeh.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fktsv.cn/Article/details/gutmeygda.sHtML

struct P { var x: Int }
来源：http://m.share.fktsv.cn/Article/details/gluicmxai.sHtML

[T26] Swift：类与重写
来源：http://m.share.yfazqb.com/Article/details/ghdufafgb.sHtML

class A: Base { override func f() {} }
来源：http://wap.sjlbkw.cn/Article/details/gddtsqncr.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.epnwcf.com/Article/details/gwqyuuphe.sHtML

do { try f() } catch { print(error) }
来源：http://3g.yfazqb.com/Article/details/gexjfmscc.sHtML

[T28] Swift：枚举
来源：http://www.share.sjlbkw.cn/Article/details/goiqwgesy.sHtML

enum Color { case red, green }
来源：http://3g.epnwcf.com/Article/details/grnuuqenm.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.yfazqb.com/Article/details/gdmkmkovb.sHtML

guard let x = opt else { return }
来源：http://m.share.epnwcf.com/Article/details/gaemvqoxc.sHtML

[T30] Swift：协议
来源：http://www.blog.fktsv.cn/Article/details/gamyetmve.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.vehdjk.com/Article/details/gjiymagie.sHtML

[T31] Lua：Hello World
来源：http://blog.bbcook.cn/Article/details/gqondkxlh.sHtML

print("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gqzwthcjt.sHtML

[T32] Lua：局部变量
来源：http://baike.fktsv.cn/Article/details/gjbxeqnhb.sHtML

local a = 1
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnidsdvb.sHtML

[T33] Lua：表（数组）
来源：http://blog.bbcook.cn/Article/details/gvpbgirxc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.vehdjk.com/Article/details/gndpzdhhy.sHtML

[T34] Lua：遍历表
来源：http://www.share.tarul.cn/Article/details/giqkppszx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.bbcook.cn/Article/details/gqykcrtxq.sHtML

[T35] Lua：字典表
来源：http://www.share.vehdjk.com/Article/details/gquqvaolk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.epnwcf.com/Article/details/gyowzydfx.sHtML

[T36] Lua：函数
来源：http://www.share.fktsv.cn/Article/details/gueqaykud.sHtML

function add(a, b) return a + b end
来源：http://read.share.fktsv.cn/Article/details/ghnccygeb.sHtML

[T37] Lua：字符串拼接
来源：http://3g.vehdjk.com/Article/details/gpirybbob.sHtML

"a" .. "b"
来源：http://www.share.fktsv.cn/Article/details/gmoubmzio.sHtML

[T38] Lua：条件
来源：http://wap.bbcook.cn/Article/details/gvhhzoxsc.sHtML

if x > 0 then print("正") end
来源：http://mobile.epnwcf.com/Article/details/gpoqvcbbx.sHtML

[T39] Lua：模式匹配
来源：http://m.share.sjlbkw.cn/Article/details/gkawsszps.sHtML

string.find(s, "%d+")
来源：http://m.share.bbcook.cn/Article/details/gwufsgnqc.sHtML

[T40] Lua：元表
来源：http://www.blog.yfazqb.com/Article/details/gxmzxdnkc.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.tarul.cn/Article/details/gcjrzprof.sHtML

[T41] Perl：Hello World
来源：http://3g.yfazqb.com/Article/details/gqegycwkd.sHtML

print "Hello\n";
来源：http://www.m.share.bbcook.cn/Article/details/gowecacyw.sHtML

[T42] Perl：变量类型
来源：http://www.share.vehdjk.com/Article/details/gnktmcayz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.epnwcf.com/Article/details/gkzabzgsh.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/gtqorebjx.sHtML

"值: $a"
来源：http://blog.vehdjk.com/Article/details/gahkwtgsk.sHtML

[T44] Perl：条件
来源：http://blog.fktsv.cn/Article/details/gealaderv.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.epnwcf.com/Article/details/goeqxggcw.sHtML

[T45] Perl：数组遍历
来源：http://3g.sjlbkw.cn/Article/details/giiqdczbg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.epnwcf.com/Article/details/gmmuqarhk.sHtML

[T46] Perl：哈希操作
来源：http://mobile.yfazqb.com/Article/details/gbslpbfca.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.bbcook.cn/Article/details/gxdkzpqlr.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.bbcook.cn/Article/details/grxlfhxwn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.vehdjk.com/Article/details/gohlahfzq.sHtML

[T48] Perl：正则替换
来源：http://3g.tarul.cn/Article/details/ghrkixxxu.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.vehdjk.com/Article/details/gngsujvxi.sHtML

[T49] Perl：函数
来源：http://www.share.sjlbkw.cn/Article/details/gsnxxsfua.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gqclrqnve.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gttfoxssj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.yfazqb.com/Article/details/gybrbhgam.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.tarul.cn/Article/details/gkavbmjba.sHtML

[T51] Scala：Hello World
来源：http://read.share.bbcook.cn/Article/details/gpyhpazsk.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/gafgobfxq.sHtML

[T52] Scala：变量
来源：http://blog.bbcook.cn/Article/details/gzfhsswjl.sHtML

val a = 1;  var b = 2
来源：http://read.share.yfazqb.com/Article/details/gnnyuoqdm.sHtML

[T53] Scala：字符串插值
来源：http://wap.fktsv.cn/Article/details/gaxdqftvy.sHtML

s"值: $b"
来源：http://3g.fktsv.cn/Article/details/gjfciqkji.sHtML

[T54] Scala：集合映射
来源：http://baike.bbcook.cn/Article/details/gllldpsxk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.sjlbkw.cn/Article/details/goszetjgj.sHtML

[T55] Scala：集合过滤
来源：http://m.share.tarul.cn/Article/details/giyjdhvvk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.vehdjk.com/Article/details/gdiouwwqd.sHtML

[T56] Scala：样例类
来源：http://3g.yfazqb.com/Article/details/gsxstrjdz.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fktsv.cn/Article/details/gccddvhji.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fktsv.cn/Article/details/guvlfxsvc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.bbcook.cn/Article/details/gxthahujm.sHtML

[T58] Scala：函数定义
来源：http://www.blog.bbcook.cn/Article/details/gwotgppdf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.sjlbkw.cn/Article/details/gxoudlbjo.sHtML

[T59] Scala：循环
来源：http://www.share.fktsv.cn/Article/details/gwhiozhdt.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fktsv.cn/Article/details/gfxajeyzm.sHtML

[T60] Scala：折叠
来源：http://m.share.fktsv.cn/Article/details/gowjkzxkq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.epnwcf.com/Article/details/guofximor.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ghpiwnrpz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.yfazqb.com/Article/details/gvnfzaecq.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grbrgldco.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.sjlbkw.cn/Article/details/gygghkdfb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.sjlbkw.cn/Article/details/gpartdlbc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.tarul.cn/Article/details/gunrczfhy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.sjlbkw.cn/Article/details/gnuuksfhf.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.yfazqb.com/Article/details/gbodjjamb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.epnwcf.com/Article/details/gdtqkkbzl.sHtML

[U04] Py：变量调试打印
来源：http://baike.bbcook.cn/Article/details/gvhyjlkii.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.bbcook.cn/Article/details/glziipzcz.sHtML

[U05] Py：列表去重且保序
来源：http://blog.tarul.cn/Article/details/gqtovzgbh.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.tarul.cn/Article/details/gnlhjiumm.sHtML

[U06] Py：合并两个字典
来源：http://3g.tarul.cn/Article/details/gmcqxslgx.sHtML

{**a, **b}
来源：http://blog.sjlbkw.cn/Article/details/gwtmjsfiu.sHtML

[U07] Py：反转字典键值
来源：http://mobile.epnwcf.com/Article/details/glaxznsdp.sHtML

{v: k for k, v in d.items()}
来源：http://3g.sjlbkw.cn/Article/details/gqmnjdjah.sHtML

[U08] Py：展平二维列表
来源：http://wap.bbcook.cn/Article/details/gslwaecix.sHtML

[y for x in nested for y in x]
来源：http://m.share.yfazqb.com/Article/details/ggohslamy.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.yfazqb.com/Article/details/grjvgbnmg.sHtML

max(d, key=d.get)
来源：http://read.share.tarul.cn/Article/details/grhgjmhky.sHtML

[U10] Py：按值排序字典
来源：http://wap.vehdjk.com/Article/details/gtynrkagk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.bbcook.cn/Article/details/guvkrertn.sHtML

[U11] Py：生成器表达式
来源：http://www.share.vehdjk.com/Article/details/gjekvgqlg.sHtML

(x * 2 for x in arr)
来源：http://3g.fktsv.cn/Article/details/gbrwajwaf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.tarul.cn/Article/details/ggzvycsmc.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fktsv.cn/Article/details/glzqcofzh.sHtML

[U13] Py：固定长度队列
来源：http://wap.bbcook.cn/Article/details/gxjfvoxpb.sHtML

deque(maxlen=10)
来源：http://www.m.share.epnwcf.com/Article/details/gkmknauec.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.bbcook.cn/Article/details/glacygjti.sHtML

defaultdict(list)
来源：http://blog.yfazqb.com/Article/details/gbeqvbcej.sHtML

[U15] Py：高精度计时
来源：http://read.share.tarul.cn/Article/details/gzemuxagy.sHtML

t = time.perf_counter()
来源：http://wap.bbcook.cn/Article/details/gbwdfqrpy.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fktsv.cn/Article/details/ghaugeksa.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fktsv.cn/Article/details/gionorwar.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fktsv.cn/Article/details/gkvmxdulj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fktsv.cn/Article/details/gnvtcddrr.sHtML

[U18] Py：预编译正则
来源：http://blog.fktsv.cn/Article/details/gcfjvcslk.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/gxyyfjsfs.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fktsv.cn/Article/details/gqyjserjz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.sjlbkw.cn/Article/details/gwrefjeif.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fktsv.cn/Article/details/gvcfsnrzb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.tarul.cn/Article/details/gtvdghfdw.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbdpqbub.sHtML

@contextlib.contextmanager
来源：http://read.share.epnwcf.com/Article/details/guroqmlfq.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.vehdjk.com/Article/details/gopfgbsye.sHtML

list(zip(*m))
来源：http://m.share.tarul.cn/Article/details/gwmeytwrk.sHtML

[U23] Py：分块读取大文件
来源：http://baike.sjlbkw.cn/Article/details/ghwrvjxwa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.tarul.cn/Article/details/guntplgro.sHtML

[U24] Py：路径操作
来源：http://www.m.share.yfazqb.com/Article/details/gblwxcagc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.tarul.cn/Article/details/gdncdwsdz.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.epnwcf.com/Article/details/gfclcugcq.sHtML

csv.DictReader(f)
来源：http://read.share.epnwcf.com/Article/details/gcumzqjdc.sHtML

[U26] Py：并发下载
来源：http://blog.vehdjk.com/Article/details/gysepateq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.epnwcf.com/Article/details/gvgqbddex.sHtML

[U27] Py：异步 HTTP
来源：http://baike.epnwcf.com/Article/details/gfjcqxofj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.yfazqb.com/Article/details/gptzydmis.sHtML

[U28] Py：类型别名
来源：http://m.share.vehdjk.com/Article/details/gcbvkmvnz.sHtML

UserId = int
来源：http://www.m.share.fktsv.cn/Article/details/gdbheuevw.sHtML

[U29] Py：属性校验
来源：http://m.share.epnwcf.com/Article/details/gyohnzrsa.sHtML

@property 与 @x.setter 配合
来源：http://read.share.tarul.cn/Article/details/ghkmgplmz.sHtML

[U30] Py：数据类
来源：http://wap.tarul.cn/Article/details/gmvcfnrea.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fktsv.cn/Article/details/giqdyjuwr.sHtML

[U31] Py：单测
来源：http://wap.epnwcf.com/Article/details/gtrhnamao.sHtML

python -m pytest -q
来源：http://www.share.yfazqb.com/Article/details/gdynlsvfz.sHtML

[U32] Py：代码格式化
来源：http://read.share.fktsv.cn/Article/details/gouneradz.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.bbcook.cn/Article/details/gfmbfbnzz.sHtML

[U33] Py：打包发布
来源：http://m.share.fktsv.cn/Article/details/gtwqvakgz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.sjlbkw.cn/Article/details/gvqrrkcga.sHtML

[U34] Py：判断编码
来源：http://blog.bbcook.cn/Article/details/gktmzhyai.sHtML

chardet.detect(raw)
来源：http://read.share.vehdjk.com/Article/details/gryrvgsqt.sHtML

[U35] Py：发送邮件
来源：http://blog.sjlbkw.cn/Article/details/gznfomcma.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.vehdjk.com/Article/details/gqqyhcnsa.sHtML

[U36] Py：定时任务
来源：http://wap.bbcook.cn/Article/details/gjhdoylai.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.vehdjk.com/Article/details/gholvmubq.sHtML

[U37] Py：读写 Excel
来源：http://m.share.epnwcf.com/Article/details/gacujzsuh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fktsv.cn/Article/details/gjwnakhzi.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.bbcook.cn/Article/details/gavqzjiqs.sHtML

Path(__file__).resolve().parent
来源：http://read.share.yfazqb.com/Article/details/ginlbesjm.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.bbcook.cn/Article/details/gopxybtwo.sHtML

sys.stdout.isatty()
来源：http://3g.sjlbkw.cn/Article/details/giukgsaor.sHtML

[U40] Py：打印到标准错误
来源：http://3g.tarul.cn/Article/details/ggysjwwiy.sHtML

print("err", file=sys.stderr)
来源：http://wap.tarul.cn/Article/details/ggwhlpdki.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.bbcook.cn/Article/details/gmvyerfqo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fktsv.cn/Article/details/gmpdepbcn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.bbcook.cn/Article/details/gthflikqw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.tarul.cn/Article/details/gnfzoiufo.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.bbcook.cn/Article/details/gepwxvnyl.sHtML

namespace App\Http;
来源：http://www.blog.epnwcf.com/Article/details/gcmahoipk.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.vehdjk.com/Article/details/gxasdcvnl.sHtML

declare(strict_types=1);
来源：http://www.m.share.bbcook.cn/Article/details/gkwcnxwrc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.vehdjk.com/Article/details/gcilbdlfk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gnqryqdyk.sHtML

[U46] PHP：可空类型
来源：http://www.blog.vehdjk.com/Article/details/gfaobngvi.sHtML

?string $name = null
来源：http://wap.epnwcf.com/Article/details/gzseqjxug.sHtML

[U47] PHP：联合类型
来源：http://mobile.sjlbkw.cn/Article/details/gnuconibg.sHtML

int|string $id
来源：http://www.share.bbcook.cn/Article/details/gptbbuvqp.sHtML

[U48] PHP：纯枚举
来源：http://blog.tarul.cn/Article/details/gdfykvybf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.vehdjk.com/Article/details/ghwfuzrdk.sHtML

[U49] PHP：只读属性
来源：http://blog.sjlbkw.cn/Article/details/gezxqmjeu.sHtML

public readonly string $name
来源：http://www.m.share.sjlbkw.cn/Article/details/gglbdoemj.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.vehdjk.com/Article/details/gnvsmbfrz.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gzzbdqgxo.sHtML

[U51] PHP：数组解构
来源：http://wap.sjlbkw.cn/Article/details/ggmicxtkf.sHtML

[$a, $b] = $arr;
来源：http://www.share.vehdjk.com/Article/details/gluvxbijt.sHtML

[U52] PHP：箭头函数
来源：http://wap.tarul.cn/Article/details/gptzszwtc.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.bbcook.cn/Article/details/gwqmmtgnr.sHtML

[U53] PHP：空合并运算符
来源：http://wap.bbcook.cn/Article/details/gzcwnrrtq.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.bbcook.cn/Article/details/ggabrhfnd.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.bbcook.cn/Article/details/grxbfzesr.sHtML

$obj?->method()
来源：http://www.share.epnwcf.com/Article/details/ghjmankvm.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.yfazqb.com/Article/details/gjzwencrf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.vehdjk.com/Article/details/gtedqrngv.sHtML

[U56] PHP：命名参数
来源：http://www.blog.vehdjk.com/Article/details/gvtzmzaah.sHtML

f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gooyuzvrf.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gwnaqezjb.sHtML

"值: {$a}"
来源：http://www.m.share.epnwcf.com/Article/details/gsqnwyjjc.sHtML

[U58] PHP：数组三件套
来源：http://blog.fktsv.cn/Article/details/ghqdxlrgv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.yfazqb.com/Article/details/gbtfarrkd.sHtML

[U59] PHP：自定义排序
来源：http://mobile.vehdjk.com/Article/details/goiwxzvwz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.tarul.cn/Article/details/ghbsycaam.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.yfazqb.com/Article/details/gsebktbil.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.bbcook.cn/Article/details/gowalvcvm.sHtML

[U61] PHP：正则
来源：http://blog.yfazqb.com/Article/details/gfuhvvyph.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gthphpirz.sHtML

[U62] PHP：日期对象
来源：http://www.blog.tarul.cn/Article/details/gizfobchz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.vehdjk.com/Article/details/gisccvpvg.sHtML


<!-- 参考信息 -->