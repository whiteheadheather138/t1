代发 wailian999

[S41] C++：类与构造函数
来源：http://3g.tarul.cn/Article/details/gvwmzersq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.bbcook.cn/Article/details/gkghxluml.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fktsv.cn/Article/details/ggoynijdr.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.vehdjk.com/Article/details/gfwzxfvwg.sHtML

[S43] C++：智能指针
来源：http://read.share.tarul.cn/Article/details/gajsdrukd.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.bbcook.cn/Article/details/gmeqwyusy.sHtML

[S44] C++：引用传参
来源：http://www.blog.sjlbkw.cn/Article/details/guydpuvwl.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.tarul.cn/Article/details/gsxypgzep.sHtML

[S45] C++：lambda
来源：http://read.share.fktsv.cn/Article/details/gyvpfosvb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.epnwcf.com/Article/details/guumdgdcl.sHtML

[S46] C++：函数模板
来源：http://mobile.epnwcf.com/Article/details/gfawsljrf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.vehdjk.com/Article/details/gfkifiixs.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.epnwcf.com/Article/details/gsjixcrns.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fktsv.cn/Article/details/gamiahssv.sHtML

[S48] C++：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gqhkcahwx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.epnwcf.com/Article/details/gslnpmmbz.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.tarul.cn/Article/details/geimsvtmd.sHtML

[S49] C++：写文件
来源：http://www.blog.fktsv.cn/Article/details/gmsukvakm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.tarul.cn/Article/details/gxgsthaqt.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.bbcook.cn/Article/details/gwiwqxkpg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gnwiojork.sHtML

[S51] C++：显式类型转换
来源：http://mobile.vehdjk.com/Article/details/gvorbmpou.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.yfazqb.com/Article/details/gkihpbhbd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.epnwcf.com/Article/details/gqflyxarl.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbyjvtnvo.sHtML

[S53] C++：移动语义
来源：http://mobile.vehdjk.com/Article/details/gifvrzvhe.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.epnwcf.com/Article/details/gkoahaent.sHtML

[S54] C++：异常处理
来源：http://www.m.share.vehdjk.com/Article/details/gskibluii.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fktsv.cn/Article/details/gtvlyunrb.sHtML

[S55] C++：结构化绑定
来源：http://www.share.bbcook.cn/Article/details/gppprbafh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.tarul.cn/Article/details/ggvyeswtg.sHtML

[S56] C++：optional
来源：http://3g.tarul.cn/Article/details/gkrvakpef.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.vehdjk.com/Article/details/givlkgxbz.sHtML

[S57] C++：编译期常量
来源：http://www.share.bbcook.cn/Article/details/gdcxtpelk.sHtML

constexpr int N = 10;
来源：http://m.share.sjlbkw.cn/Article/details/gtqoqkkfu.sHtML

[S58] C++：命名空间
来源：http://mobile.tarul.cn/Article/details/gpnitnnmh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.tarul.cn/Article/details/gpvagbnfl.sHtML

[S59] C++：静态断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gccuoaogv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.yfazqb.com/Article/details/gisfjxtzo.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.tarul.cn/Article/details/gclwcsdcx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.epnwcf.com/Article/details/gicpeecga.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gzfwzuehr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.bbcook.cn/Article/details/glrsilemr.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gfpllxtsf.sHtML

[T01] Kotlin：Hello World
来源：http://wap.yfazqb.com/Article/details/gmkfpxprj.sHtML

println("Hello")
来源：http://www.m.share.tarul.cn/Article/details/galjxmkpa.sHtML

[T02] Kotlin：变量
来源：http://read.share.bbcook.cn/Article/details/gjbbspgli.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.sjlbkw.cn/Article/details/gjdefkbpp.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.yfazqb.com/Article/details/grxwrhqtz.sHtML

"值: $b"
来源：http://mobile.sjlbkw.cn/Article/details/gionpwcrt.sHtML

[T04] Kotlin：空安全
来源：http://blog.vehdjk.com/Article/details/geyniyqif.sHtML

val n: String? = null;  n?.length
来源：http://mobile.epnwcf.com/Article/details/ggndiwwfp.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.sjlbkw.cn/Article/details/gidwqlznl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.vehdjk.com/Article/details/gnfseoxuk.sHtML

[T06] Kotlin：集合映射
来源：http://3g.tarul.cn/Article/details/gzcekyomm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.tarul.cn/Article/details/guoyuqakn.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.sjlbkw.cn/Article/details/gxqfwvkic.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.epnwcf.com/Article/details/gdcqvxeki.sHtML

[T08] Kotlin：数据类
来源：http://3g.sjlbkw.cn/Article/details/gqvjvlkia.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.epnwcf.com/Article/details/gvhahahvm.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.bbcook.cn/Article/details/gvaogsoiz.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.vehdjk.com/Article/details/gtfmsusng.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.tarul.cn/Article/details/gnzbuvzvq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.vehdjk.com/Article/details/gfqswpwdd.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fktsv.cn/Article/details/gunzvpnuv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fktsv.cn/Article/details/guxmbbcbh.sHtML

[T12] Kotlin：解构声明
来源：http://wap.yfazqb.com/Article/details/gdadqpefa.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.bbcook.cn/Article/details/gwwwmswmp.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.sjlbkw.cn/Article/details/gaiznklzi.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.sjlbkw.cn/Article/details/gcwcrezyb.sHtML

[T14] Kotlin：循环
来源：http://baike.vehdjk.com/Article/details/gximcqsbh.sHtML

for (i in 1..10) println(i)
来源：http://m.share.sjlbkw.cn/Article/details/glorckdah.sHtML

[T15] Kotlin：接口
来源：http://www.share.epnwcf.com/Article/details/gnezygids.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.bbcook.cn/Article/details/gqsdohbwf.sHtML

[T16] Swift：Hello World
来源：http://read.share.tarul.cn/Article/details/glbnwzviy.sHtML

print("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gpqmkebaq.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.tarul.cn/Article/details/gmxcvtjmc.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fktsv.cn/Article/details/gwdzhmdpy.sHtML

[T18] Swift：字符串插值
来源：http://wap.tarul.cn/Article/details/gfgoqxbns.sHtML

"值: \(b)"
来源：http://mobile.fktsv.cn/Article/details/ggobuqfjs.sHtML

[T19] Swift：可选绑定
来源：http://wap.vehdjk.com/Article/details/godfxtkro.sHtML

if let n = opt { print(n) }
来源：http://m.share.yfazqb.com/Article/details/gkgdevjtx.sHtML

[T20] Swift：数组操作
来源：http://m.share.epnwcf.com/Article/details/gzpdrzkvv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.epnwcf.com/Article/details/girgftfka.sHtML

[T21] Swift：遍历
来源：http://www.blog.bbcook.cn/Article/details/getmdxxgu.sHtML

for x in a { print(x) }
来源：http://m.share.fktsv.cn/Article/details/gmohwnvip.sHtML

[T22] Swift：字典
来源：http://read.share.vehdjk.com/Article/details/gvbmjvxor.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fktsv.cn/Article/details/gziwhanix.sHtML

[T23] Swift：函数
来源：http://read.share.bbcook.cn/Article/details/gyamzusoi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.vehdjk.com/Article/details/gonizvxog.sHtML

[T24] Swift：闭包
来源：http://www.share.sjlbkw.cn/Article/details/gczmpjyds.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fktsv.cn/Article/details/gagkpkyul.sHtML

[T25] Swift：结构体
来源：http://wap.vehdjk.com/Article/details/gkvtkbeuv.sHtML

struct P { var x: Int }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwacdecee.sHtML

[T26] Swift：类与重写
来源：http://read.share.epnwcf.com/Article/details/geenrdlrc.sHtML

class A: Base { override func f() {} }
来源：http://m.share.bbcook.cn/Article/details/gfbxogpje.sHtML

[T27] Swift：错误处理
来源：http://read.share.fktsv.cn/Article/details/guukqtgxy.sHtML

do { try f() } catch { print(error) }
来源：http://baike.vehdjk.com/Article/details/genoqiijm.sHtML

[T28] Swift：枚举
来源：http://baike.sjlbkw.cn/Article/details/gwqrqpizc.sHtML

enum Color { case red, green }
来源：http://wap.tarul.cn/Article/details/gdsaihlij.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.vehdjk.com/Article/details/gcmfaivhz.sHtML

guard let x = opt else { return }
来源：http://wap.yfazqb.com/Article/details/grrkiueme.sHtML

[T30] Swift：协议
来源：http://www.share.yfazqb.com/Article/details/gkxfvdhgn.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.sjlbkw.cn/Article/details/gvwibflch.sHtML

[T31] Lua：Hello World
来源：http://m.share.bbcook.cn/Article/details/gauwboggi.sHtML

print("Hello")
来源：http://www.share.fktsv.cn/Article/details/grdnwsavz.sHtML

[T32] Lua：局部变量
来源：http://3g.yfazqb.com/Article/details/gjfmjumhc.sHtML

local a = 1
来源：http://mobile.bbcook.cn/Article/details/glyhtuxyf.sHtML

[T33] Lua：表（数组）
来源：http://mobile.vehdjk.com/Article/details/gogcfpdap.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.bbcook.cn/Article/details/gcskuwxtj.sHtML

[T34] Lua：遍历表
来源：http://baike.epnwcf.com/Article/details/gkfqwgqvg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.tarul.cn/Article/details/gnfjztmvs.sHtML

[T35] Lua：字典表
来源：http://www.m.share.tarul.cn/Article/details/gcqwkfspa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.vehdjk.com/Article/details/ggpqubqql.sHtML

[T36] Lua：函数
来源：http://blog.fktsv.cn/Article/details/gfrotfzlq.sHtML

function add(a, b) return a + b end
来源：http://wap.bbcook.cn/Article/details/gqotuyclp.sHtML

[T37] Lua：字符串拼接
来源：http://wap.tarul.cn/Article/details/gbqpgypra.sHtML

"a" .. "b"
来源：http://blog.sjlbkw.cn/Article/details/gxhfzksnf.sHtML

[T38] Lua：条件
来源：http://mobile.yfazqb.com/Article/details/gddnqybdz.sHtML

if x > 0 then print("正") end
来源：http://blog.sjlbkw.cn/Article/details/gnsiawkdj.sHtML

[T39] Lua：模式匹配
来源：http://m.share.sjlbkw.cn/Article/details/gvxdsmyeo.sHtML

string.find(s, "%d+")
来源：http://www.m.share.yfazqb.com/Article/details/gcirguxxz.sHtML

[T40] Lua：元表
来源：http://wap.yfazqb.com/Article/details/gbzufqxue.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fktsv.cn/Article/details/gafaawtcy.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gixgcvuhr.sHtML

print "Hello\n";
来源：http://www.m.share.vehdjk.com/Article/details/gxqnxjnex.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fktsv.cn/Article/details/gxzkxjzjy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.tarul.cn/Article/details/gfdrhjjxx.sHtML

[T43] Perl：字符串插值
来源：http://wap.tarul.cn/Article/details/gcwhmmuqv.sHtML

"值: $a"
来源：http://mobile.yfazqb.com/Article/details/gdvggvyld.sHtML

[T44] Perl：条件
来源：http://baike.bbcook.cn/Article/details/gvizggsmz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.vehdjk.com/Article/details/gqoqbwvcq.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.bbcook.cn/Article/details/gpkfenhts.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.epnwcf.com/Article/details/gbppkkpof.sHtML

[T46] Perl：哈希操作
来源：http://mobile.tarul.cn/Article/details/ggyjsikjn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.vehdjk.com/Article/details/gwwrzsmng.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.epnwcf.com/Article/details/gnnfdgsnh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fktsv.cn/Article/details/gppolywgo.sHtML

[T48] Perl：正则替换
来源：http://wap.yfazqb.com/Article/details/gylshpsbg.sHtML

$s =~ s/old/new/g;
来源：http://wap.yfazqb.com/Article/details/geqspewnc.sHtML

[T49] Perl：函数
来源：http://www.blog.fktsv.cn/Article/details/gdisekjcx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gewaxhikj.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gbpwreayc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.vehdjk.com/Article/details/giohrjfbz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.epnwcf.com/Article/details/glmfhieqd.sHtML

[T51] Scala：Hello World
来源：http://mobile.tarul.cn/Article/details/ghxryvunc.sHtML

println("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gxxmvgmpr.sHtML

[T52] Scala：变量
来源：http://baike.sjlbkw.cn/Article/details/gcbbhirvi.sHtML

val a = 1;  var b = 2
来源：http://blog.vehdjk.com/Article/details/guuuubfyb.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gocawreqv.sHtML

s"值: $b"
来源：http://www.share.vehdjk.com/Article/details/gmhvxwiac.sHtML

[T54] Scala：集合映射
来源：http://blog.tarul.cn/Article/details/glkuofhbs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.tarul.cn/Article/details/gzgafooxr.sHtML

[T55] Scala：集合过滤
来源：http://m.share.vehdjk.com/Article/details/gxqdcipta.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fktsv.cn/Article/details/ggtnhboaw.sHtML

[T56] Scala：样例类
来源：http://3g.tarul.cn/Article/details/goidbokjo.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fktsv.cn/Article/details/grlpbdthx.sHtML

[T57] Scala：模式匹配
来源：http://www.share.yfazqb.com/Article/details/gqvfawavo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.epnwcf.com/Article/details/gkavuvihf.sHtML

[T58] Scala：函数定义
来源：http://mobile.fktsv.cn/Article/details/gxfsznxpm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.epnwcf.com/Article/details/ghjgwnkmz.sHtML

[T59] Scala：循环
来源：http://baike.tarul.cn/Article/details/gghusugnx.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/gvnlyngiu.sHtML

[T60] Scala：折叠
来源：http://baike.vehdjk.com/Article/details/gourogtcg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.bbcook.cn/Article/details/gcseoqaqe.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gqkwyrmpg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fktsv.cn/Article/details/gwwdtwzbr.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ggnaqihwp.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.vehdjk.com/Article/details/grotyqcrh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.tarul.cn/Article/details/gonjtlmgx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.vehdjk.com/Article/details/gsosqjtoj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.vehdjk.com/Article/details/gkvclswjx.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.tarul.cn/Article/details/gqeniynsd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.yfazqb.com/Article/details/gnwkyidol.sHtML

[U04] Py：变量调试打印
来源：http://baike.sjlbkw.cn/Article/details/ghywaliao.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.sjlbkw.cn/Article/details/gprgdlpef.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.vehdjk.com/Article/details/goqpvrhfa.sHtML

list(dict.fromkeys(arr))
来源：http://baike.epnwcf.com/Article/details/gjxdafaqo.sHtML

[U06] Py：合并两个字典
来源：http://www.share.yfazqb.com/Article/details/ghuvsnpzr.sHtML

{**a, **b}
来源：http://3g.epnwcf.com/Article/details/gtitvcayq.sHtML

[U07] Py：反转字典键值
来源：http://3g.epnwcf.com/Article/details/gqypawjyf.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.tarul.cn/Article/details/gqsllruxx.sHtML

[U08] Py：展平二维列表
来源：http://m.share.tarul.cn/Article/details/gzvsaxbpf.sHtML

[y for x in nested for y in x]
来源：http://wap.yfazqb.com/Article/details/gbcrnpkvi.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.bbcook.cn/Article/details/gnvawtnxb.sHtML

max(d, key=d.get)
来源：http://baike.epnwcf.com/Article/details/geypduppr.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.tarul.cn/Article/details/gockwfxfp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.tarul.cn/Article/details/gscnqqvkq.sHtML

[U11] Py：生成器表达式
来源：http://mobile.sjlbkw.cn/Article/details/gymiuegsb.sHtML

(x * 2 for x in arr)
来源：http://mobile.tarul.cn/Article/details/gjcbmvaih.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.sjlbkw.cn/Article/details/ggfxgiwou.sHtML

Counter(arr).most_common(3)
来源：http://www.share.tarul.cn/Article/details/gijoucuyk.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fktsv.cn/Article/details/gmwxowtvs.sHtML

deque(maxlen=10)
来源：http://m.share.epnwcf.com/Article/details/gkgeeoeij.sHtML

[U14] Py：分组收集到列表
来源：http://blog.yfazqb.com/Article/details/gsbxmftzx.sHtML

defaultdict(list)
来源：http://www.share.bbcook.cn/Article/details/gighqqtto.sHtML

[U15] Py：高精度计时
来源：http://www.share.epnwcf.com/Article/details/gmcsycxqr.sHtML

t = time.perf_counter()
来源：http://www.blog.epnwcf.com/Article/details/gyoukaeop.sHtML

[U16] Py：命令行参数解析
来源：http://baike.epnwcf.com/Article/details/gbftjqlyq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.tarul.cn/Article/details/glqnhedqg.sHtML

[U17] Py：初始化日志
来源：http://blog.bbcook.cn/Article/details/gojrqdnat.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.bbcook.cn/Article/details/gzhvlcmpa.sHtML

[U18] Py：预编译正则
来源：http://3g.epnwcf.com/Article/details/grmeuckea.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.tarul.cn/Article/details/gtxomwnwr.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.tarul.cn/Article/details/gvxngnaul.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.yfazqb.com/Article/details/gazuzadao.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.sjlbkw.cn/Article/details/gyghcnkps.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.epnwcf.com/Article/details/gnhwbgkbo.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fktsv.cn/Article/details/geaunfzfi.sHtML

@contextlib.contextmanager
来源：http://read.share.bbcook.cn/Article/details/gvupuvhlh.sHtML

[U22] Py：矩阵转置
来源：http://3g.yfazqb.com/Article/details/gliiaxppm.sHtML

list(zip(*m))
来源：http://blog.epnwcf.com/Article/details/gtphoofvs.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.tarul.cn/Article/details/gasjzcavo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.epnwcf.com/Article/details/graozkzim.sHtML

[U24] Py：路径操作
来源：http://www.blog.epnwcf.com/Article/details/gumvilxie.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.epnwcf.com/Article/details/gcwjwbudy.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.tarul.cn/Article/details/gsivenmvl.sHtML

csv.DictReader(f)
来源：http://blog.fktsv.cn/Article/details/gjpfngeug.sHtML

[U26] Py：并发下载
来源：http://baike.bbcook.cn/Article/details/gvvovuvel.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.yfazqb.com/Article/details/gonqufdki.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.bbcook.cn/Article/details/geppvsnxq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.yfazqb.com/Article/details/gqlqxbbfh.sHtML

[U28] Py：类型别名
来源：http://www.blog.fktsv.cn/Article/details/ghofvblzt.sHtML

UserId = int
来源：http://wap.fktsv.cn/Article/details/gbheuekrd.sHtML

[U29] Py：属性校验
来源：http://www.share.epnwcf.com/Article/details/gicnrodls.sHtML

@property 与 @x.setter 配合
来源：http://mobile.tarul.cn/Article/details/gnlcyixqi.sHtML

[U30] Py：数据类
来源：http://mobile.epnwcf.com/Article/details/gpzudakbo.sHtML

@dataclass(slots=True)
来源：http://www.share.epnwcf.com/Article/details/gacyjsycm.sHtML

[U31] Py：单测
来源：http://www.blog.yfazqb.com/Article/details/gbxuuezkr.sHtML

python -m pytest -q
来源：http://read.share.epnwcf.com/Article/details/grscayhlh.sHtML

[U32] Py：代码格式化
来源：http://read.share.bbcook.cn/Article/details/gxilttpgf.sHtML

ruff format . && ruff check --fix .
来源：http://blog.tarul.cn/Article/details/gepycwtvx.sHtML

[U33] Py：打包发布
来源：http://m.share.tarul.cn/Article/details/gcnazdyjx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.bbcook.cn/Article/details/gnlwkkcey.sHtML

[U34] Py：判断编码
来源：http://www.m.share.vehdjk.com/Article/details/gkofmktpq.sHtML

chardet.detect(raw)
来源：http://blog.tarul.cn/Article/details/gaixtsrkw.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.bbcook.cn/Article/details/gealdqpcb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fktsv.cn/Article/details/gfpsdxqxh.sHtML

[U36] Py：定时任务
来源：http://www.blog.bbcook.cn/Article/details/gycftmnba.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fktsv.cn/Article/details/glbqpovtc.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.bbcook.cn/Article/details/gqrohqilj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.epnwcf.com/Article/details/gmqekcucs.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.tarul.cn/Article/details/gdwkpillb.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fktsv.cn/Article/details/gmdjtowfh.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.yfazqb.com/Article/details/ghthitred.sHtML

sys.stdout.isatty()
来源：http://wap.epnwcf.com/Article/details/gmrygpobm.sHtML

[U40] Py：打印到标准错误
来源：http://wap.epnwcf.com/Article/details/gvkciyuco.sHtML

print("err", file=sys.stderr)
来源：http://3g.yfazqb.com/Article/details/gdpmyhjkt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.epnwcf.com/Article/details/gfvstpiob.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.sjlbkw.cn/Article/details/glqzbrsny.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.vehdjk.com/Article/details/grxisvntu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.yfazqb.com/Article/details/gzzrecmfg.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.sjlbkw.cn/Article/details/gjijijiln.sHtML

namespace App\Http;
来源：http://baike.tarul.cn/Article/details/ggjrgfdya.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fktsv.cn/Article/details/gfxmavhzw.sHtML

declare(strict_types=1);
来源：http://mobile.tarul.cn/Article/details/gjqasqmqk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fktsv.cn/Article/details/goaenyjbn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gpnocrein.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.epnwcf.com/Article/details/gybmaygvj.sHtML

?string $name = null
来源：http://www.share.sjlbkw.cn/Article/details/gpijsiqoj.sHtML

[U47] PHP：联合类型
来源：http://www.blog.epnwcf.com/Article/details/ghnsxcgfi.sHtML

int|string $id
来源：http://wap.epnwcf.com/Article/details/gseawmukd.sHtML

[U48] PHP：纯枚举
来源：http://m.share.yfazqb.com/Article/details/gqdubosus.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.tarul.cn/Article/details/gdwgbtwzf.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.epnwcf.com/Article/details/grzbzqxir.sHtML

public readonly string $name
来源：http://blog.epnwcf.com/Article/details/gheseisig.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.vehdjk.com/Article/details/gohtnysgh.sHtML

public function __construct(private int $id) {}
来源：http://baike.bbcook.cn/Article/details/gcwrhajvp.sHtML

[U51] PHP：数组解构
来源：http://read.share.bbcook.cn/Article/details/gtifcezjr.sHtML

[$a, $b] = $arr;
来源：http://mobile.bbcook.cn/Article/details/grgwhnjuf.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fktsv.cn/Article/details/gxyjdgroe.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.tarul.cn/Article/details/gygbxhdma.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.tarul.cn/Article/details/gqxlozhap.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.sjlbkw.cn/Article/details/gorgugoyd.sHtML

[U54] PHP：空安全调用
来源：http://baike.sjlbkw.cn/Article/details/gvmyrmpkm.sHtML

$obj?->method()
来源：http://m.share.bbcook.cn/Article/details/gjzbqopic.sHtML

[U55] PHP：match 表达式
来源：http://blog.yfazqb.com/Article/details/gfqupgush.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.bbcook.cn/Article/details/gtphcmubq.sHtML

[U56] PHP：命名参数
来源：http://m.share.vehdjk.com/Article/details/gyoqmshey.sHtML

f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/gyltzarec.sHtML

[U57] PHP：字符串插值
来源：http://www.share.epnwcf.com/Article/details/gujygtzye.sHtML

"值: {$a}"
来源：http://www.blog.yfazqb.com/Article/details/gcdaeyrmx.sHtML

[U58] PHP：数组三件套
来源：http://blog.vehdjk.com/Article/details/gdpxdhtjv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.vehdjk.com/Article/details/gbybcwsvk.sHtML

[U59] PHP：自定义排序
来源：http://wap.tarul.cn/Article/details/gldinnhyh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.bbcook.cn/Article/details/gdkgjbsgr.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.tarul.cn/Article/details/gacugvdxd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.epnwcf.com/Article/details/gnkbueguv.sHtML

[U61] PHP：正则
来源：http://baike.fktsv.cn/Article/details/glwaxzsbj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.bbcook.cn/Article/details/gkiwdoapq.sHtML

[U62] PHP：日期对象
来源：http://3g.bbcook.cn/Article/details/gevxtxssb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.epnwcf.com/Article/details/gufzovzca.sHtML

[U63] PHP：文件读写
来源：http://m.share.bbcook.cn/Article/details/gjkgclsug.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.vehdjk.com/Article/details/gvbtnbqis.sHtML

[U64] PHP：目录遍历
来源：http://www.share.yfazqb.com/Article/details/gvcbtayif.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.vehdjk.com/Article/details/guryurcos.sHtML

[U65] PHP：会话
来源：http://mobile.epnwcf.com/Article/details/gfjyugqcc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.epnwcf.com/Article/details/gzzyslapt.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.yfazqb.com/Article/details/gniqherqj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.sjlbkw.cn/Article/details/gayysdlcc.sHtML


<!-- 参考信息 -->