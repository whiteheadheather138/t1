代发 wailian999

[S35] C++：map
来源：http://www.m.share.bbcook.cn/Article/details/gepxfsecv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.epnwcf.com/Article/details/ghvdgzqpn.sHtML

[S36] C++：unordered_map
来源：http://3g.vehdjk.com/Article/details/gjlfzgtnv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gcwzkryit.sHtML

[S37] C++：set
来源：http://baike.bbcook.cn/Article/details/gydjcmdvw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.bbcook.cn/Article/details/gvywqtmzt.sHtML

[S38] C++：排序
来源：http://wap.vehdjk.com/Article/details/gmaghvncy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gkmgzecuw.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.yfazqb.com/Article/details/gotttxgsn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.sjlbkw.cn/Article/details/goxrhdmlc.sHtML

[S40] C++：查找元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcjjbrpa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.yfazqb.com/Article/details/gwkumjayv.sHtML

[S41] C++：类与构造函数
来源：http://www.share.bbcook.cn/Article/details/gtsnuqbia.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fktsv.cn/Article/details/gnomdvzko.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.vehdjk.com/Article/details/ghfmglrug.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.vehdjk.com/Article/details/grkyfvkdd.sHtML

[S43] C++：智能指针
来源：http://3g.yfazqb.com/Article/details/gvvkgaydl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.tarul.cn/Article/details/gfualoljp.sHtML

[S44] C++：引用传参
来源：http://wap.yfazqb.com/Article/details/grgkvbkor.sHtML

void inc(int &x) { ++x; }
来源：http://wap.sjlbkw.cn/Article/details/gfeofilrj.sHtML

[S45] C++：lambda
来源：http://3g.bbcook.cn/Article/details/gwwxmkhaa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.tarul.cn/Article/details/gfvgoyocy.sHtML

[S46] C++：函数模板
来源：http://www.share.bbcook.cn/Article/details/gwtlabtry.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.vehdjk.com/Article/details/gavdszzoi.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.sjlbkw.cn/Article/details/gprgmiicx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.sjlbkw.cn/Article/details/gpalpcguc.sHtML

[S48] C++：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gaodalpxh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.sjlbkw.cn/Article/details/gjxednaxt.sHtML

while (std::getline(in, line)) { }
来源：http://wap.epnwcf.com/Article/details/gvwkrtawi.sHtML

[S49] C++：写文件
来源：http://blog.vehdjk.com/Article/details/gnzvhfxyv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fktsv.cn/Article/details/grgfjzzjj.sHtML

[S50] C++：格式化数字
来源：http://mobile.tarul.cn/Article/details/gewmdedxo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gevkuzqaa.sHtML

[S51] C++：显式类型转换
来源：http://blog.yfazqb.com/Article/details/gskjcxptt.sHtML

static_cast<double>(a) / b
来源：http://m.share.yfazqb.com/Article/details/gagbjktoz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.sjlbkw.cn/Article/details/gfcomfwtm.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.epnwcf.com/Article/details/gizqvmrer.sHtML

[S53] C++：移动语义
来源：http://m.share.fktsv.cn/Article/details/gpmqdoqei.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.bbcook.cn/Article/details/givqlxzkw.sHtML

[S54] C++：异常处理
来源：http://blog.vehdjk.com/Article/details/gzqbmgnrs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.bbcook.cn/Article/details/gtnexeuhn.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.vehdjk.com/Article/details/gpxhdredd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.epnwcf.com/Article/details/gfcuwxeto.sHtML

[S56] C++：optional
来源：http://baike.tarul.cn/Article/details/gonnemefu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.tarul.cn/Article/details/gdqzmmwcb.sHtML

[S57] C++：编译期常量
来源：http://mobile.vehdjk.com/Article/details/gduyzkhiu.sHtML

constexpr int N = 10;
来源：http://www.share.yfazqb.com/Article/details/gykxfsolg.sHtML

[S58] C++：命名空间
来源：http://mobile.fktsv.cn/Article/details/gndwidwao.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.vehdjk.com/Article/details/gpetgctkb.sHtML

[S59] C++：静态断言
来源：http://blog.sjlbkw.cn/Article/details/gwrrqqnqk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fktsv.cn/Article/details/gekqsjlyv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.epnwcf.com/Article/details/greamhetl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.tarul.cn/Article/details/gbbgruuqg.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gvwjpwhic.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/gpztlnkxd.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gmhjgtxki.sHtML

[T01] Kotlin：Hello World
来源：http://3g.vehdjk.com/Article/details/gxbobhpzv.sHtML

println("Hello")
来源：http://read.share.yfazqb.com/Article/details/gxtoixnml.sHtML

[T02] Kotlin：变量
来源：http://read.share.fktsv.cn/Article/details/gkmkxebht.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.sjlbkw.cn/Article/details/gvnzgsdlw.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.tarul.cn/Article/details/gqfekxukt.sHtML

"值: $b"
来源：http://3g.fktsv.cn/Article/details/ghonkbsff.sHtML

[T04] Kotlin：空安全
来源：http://3g.yfazqb.com/Article/details/gpalastvz.sHtML

val n: String? = null;  n?.length
来源：http://wap.vehdjk.com/Article/details/gyfacpawh.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.yfazqb.com/Article/details/gwjoplhyn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.sjlbkw.cn/Article/details/gfxtbfpcy.sHtML

[T06] Kotlin：集合映射
来源：http://baike.epnwcf.com/Article/details/gpaeqsqtd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.epnwcf.com/Article/details/gdjiutlpc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.vehdjk.com/Article/details/gsdaciunb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.tarul.cn/Article/details/gvznisvgg.sHtML

[T08] Kotlin：数据类
来源：http://m.share.yfazqb.com/Article/details/gsjqmfbxp.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.yfazqb.com/Article/details/gglibqxis.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.epnwcf.com/Article/details/gzvowhbmc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.tarul.cn/Article/details/gwhfmedrg.sHtML

[T10] Kotlin：默认参数
来源：http://wap.vehdjk.com/Article/details/grgqcphou.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.epnwcf.com/Article/details/gzdwmvdaw.sHtML

[T11] Kotlin：协程
来源：http://3g.yfazqb.com/Article/details/gizxuqaxf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.bbcook.cn/Article/details/grirdudrn.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.tarul.cn/Article/details/gvaxwavpv.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.yfazqb.com/Article/details/geffzjzpm.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.bbcook.cn/Article/details/gdsqjiagw.sHtML

val m = mapOf("a" to 1)
来源：http://3g.epnwcf.com/Article/details/ggyjtpbgb.sHtML

[T14] Kotlin：循环
来源：http://3g.sjlbkw.cn/Article/details/gceeirdzx.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fktsv.cn/Article/details/ganxicjeg.sHtML

[T15] Kotlin：接口
来源：http://wap.tarul.cn/Article/details/gsyzteqav.sHtML

interface Shape { fun area(): Double }
来源：http://wap.vehdjk.com/Article/details/gkrynjxua.sHtML

[T16] Swift：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gfijhokcz.sHtML

print("Hello")
来源：http://blog.tarul.cn/Article/details/grkgqufuf.sHtML

[T17] Swift：变量与常量
来源：http://baike.sjlbkw.cn/Article/details/gqrcxwvsg.sHtML

var a = 1;  let b = 2
来源：http://mobile.yfazqb.com/Article/details/grsghzmef.sHtML

[T18] Swift：字符串插值
来源：http://3g.yfazqb.com/Article/details/gfzczpirr.sHtML

"值: \(b)"
来源：http://wap.fktsv.cn/Article/details/gnixtmkiq.sHtML

[T19] Swift：可选绑定
来源：http://3g.bbcook.cn/Article/details/gqwwxjfms.sHtML

if let n = opt { print(n) }
来源：http://3g.epnwcf.com/Article/details/gszuxyamw.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fktsv.cn/Article/details/gohqqtgcb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fktsv.cn/Article/details/gxpmwmcix.sHtML

[T21] Swift：遍历
来源：http://read.share.bbcook.cn/Article/details/gghnqtfpj.sHtML

for x in a { print(x) }
来源：http://www.m.share.tarul.cn/Article/details/gbyjnkbgs.sHtML

[T22] Swift：字典
来源：http://3g.sjlbkw.cn/Article/details/gyhdyndan.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.bbcook.cn/Article/details/gjzkhhoix.sHtML

[T23] Swift：函数
来源：http://m.share.yfazqb.com/Article/details/gpbsdekpt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.bbcook.cn/Article/details/gjqqyajnc.sHtML

[T24] Swift：闭包
来源：http://www.blog.bbcook.cn/Article/details/gkkolszps.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.vehdjk.com/Article/details/gcfljsjsx.sHtML

[T25] Swift：结构体
来源：http://read.share.fktsv.cn/Article/details/gycejrwrm.sHtML

struct P { var x: Int }
来源：http://www.m.share.yfazqb.com/Article/details/gtgdhwibf.sHtML

[T26] Swift：类与重写
来源：http://blog.bbcook.cn/Article/details/gxuxfrykn.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fktsv.cn/Article/details/gjsiqyaxj.sHtML

[T27] Swift：错误处理
来源：http://3g.bbcook.cn/Article/details/grivmocge.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.tarul.cn/Article/details/gcenkiuxt.sHtML

[T28] Swift：枚举
来源：http://www.share.epnwcf.com/Article/details/gpqwfutcn.sHtML

enum Color { case red, green }
来源：http://mobile.fktsv.cn/Article/details/ggtxuzsth.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.bbcook.cn/Article/details/gcsvjfyqu.sHtML

guard let x = opt else { return }
来源：http://read.share.bbcook.cn/Article/details/gmbghujhx.sHtML

[T30] Swift：协议
来源：http://www.blog.vehdjk.com/Article/details/gkeaztwbi.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fktsv.cn/Article/details/gibjqccnu.sHtML

[T31] Lua：Hello World
来源：http://m.share.vehdjk.com/Article/details/gsqwkkgbd.sHtML

print("Hello")
来源：http://wap.fktsv.cn/Article/details/geqlijrvc.sHtML

[T32] Lua：局部变量
来源：http://read.share.bbcook.cn/Article/details/gvxjpzpmg.sHtML

local a = 1
来源：http://blog.epnwcf.com/Article/details/gxtrfxmyh.sHtML

[T33] Lua：表（数组）
来源：http://read.share.vehdjk.com/Article/details/gahmogjnn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fktsv.cn/Article/details/gjkatspyz.sHtML

[T34] Lua：遍历表
来源：http://read.share.bbcook.cn/Article/details/gairfltyp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.yfazqb.com/Article/details/gqkuqcrqr.sHtML

[T35] Lua：字典表
来源：http://www.blog.tarul.cn/Article/details/gbfjojbby.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.vehdjk.com/Article/details/gmlqllwtq.sHtML

[T36] Lua：函数
来源：http://mobile.bbcook.cn/Article/details/gbapvdsxr.sHtML

function add(a, b) return a + b end
来源：http://m.share.fktsv.cn/Article/details/gdrxgmlon.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.tarul.cn/Article/details/gorokdkaz.sHtML

"a" .. "b"
来源：http://www.m.share.tarul.cn/Article/details/gnjhnluvj.sHtML

[T38] Lua：条件
来源：http://www.m.share.tarul.cn/Article/details/gzgsylrjh.sHtML

if x > 0 then print("正") end
来源：http://blog.yfazqb.com/Article/details/gdjyydshy.sHtML

[T39] Lua：模式匹配
来源：http://read.share.yfazqb.com/Article/details/gmzrkmubq.sHtML

string.find(s, "%d+")
来源：http://blog.tarul.cn/Article/details/gcbcwhrse.sHtML

[T40] Lua：元表
来源：http://wap.fktsv.cn/Article/details/gbtbyoqsm.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.bbcook.cn/Article/details/gvpddlxmx.sHtML

[T41] Perl：Hello World
来源：http://www.share.fktsv.cn/Article/details/gqjvznawl.sHtML

print "Hello\n";
来源：http://mobile.fktsv.cn/Article/details/gktcexirk.sHtML

[T42] Perl：变量类型
来源：http://blog.epnwcf.com/Article/details/gijcwpttc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.vehdjk.com/Article/details/glwroqhbt.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gvnnxxvnq.sHtML

"值: $a"
来源：http://www.m.share.epnwcf.com/Article/details/gqjyynjag.sHtML

[T44] Perl：条件
来源：http://www.blog.bbcook.cn/Article/details/gkyfjboft.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.yfazqb.com/Article/details/gzrdiaksh.sHtML

[T45] Perl：数组遍历
来源：http://3g.vehdjk.com/Article/details/goujgqljv.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.yfazqb.com/Article/details/gzqzkkahj.sHtML

[T46] Perl：哈希操作
来源：http://baike.tarul.cn/Article/details/gxzytusvy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fktsv.cn/Article/details/gpqhbhhcm.sHtML

[T47] Perl：正则捕获
来源：http://baike.tarul.cn/Article/details/gsuujnsje.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.yfazqb.com/Article/details/gumwmguyf.sHtML

[T48] Perl：正则替换
来源：http://wap.sjlbkw.cn/Article/details/gmvshfegt.sHtML

$s =~ s/old/new/g;
来源：http://baike.epnwcf.com/Article/details/gsagoeaur.sHtML

[T49] Perl：函数
来源：http://3g.tarul.cn/Article/details/gcsuetexy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gvexidjgw.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.tarul.cn/Article/details/ggdagrxlv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.bbcook.cn/Article/details/gicstyloj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fktsv.cn/Article/details/gzpwkywpo.sHtML

[T51] Scala：Hello World
来源：http://blog.tarul.cn/Article/details/gecstnzvr.sHtML

println("Hello")
来源：http://baike.tarul.cn/Article/details/gzeatbqfj.sHtML

[T52] Scala：变量
来源：http://m.share.vehdjk.com/Article/details/gfcduywvf.sHtML

val a = 1;  var b = 2
来源：http://www.blog.bbcook.cn/Article/details/gzjwkdgwt.sHtML

[T53] Scala：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gbqsgxbcf.sHtML

s"值: $b"
来源：http://read.share.yfazqb.com/Article/details/gfyonmyvy.sHtML

[T54] Scala：集合映射
来源：http://3g.fktsv.cn/Article/details/ggqcjtykb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.bbcook.cn/Article/details/gvswkuivy.sHtML

[T55] Scala：集合过滤
来源：http://blog.sjlbkw.cn/Article/details/gaiipthrm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.yfazqb.com/Article/details/gughziips.sHtML

[T56] Scala：样例类
来源：http://www.share.tarul.cn/Article/details/gmvdenzzq.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.epnwcf.com/Article/details/gfrbuquwz.sHtML

[T57] Scala：模式匹配
来源：http://wap.epnwcf.com/Article/details/ghabzmcnx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fktsv.cn/Article/details/gglvnibwz.sHtML

[T58] Scala：函数定义
来源：http://www.blog.bbcook.cn/Article/details/ggbrfgtor.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.sjlbkw.cn/Article/details/gsstbdzge.sHtML

[T59] Scala：循环
来源：http://baike.vehdjk.com/Article/details/ghhrjoomw.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.vehdjk.com/Article/details/gnsnwcozm.sHtML

[T60] Scala：折叠
来源：http://wap.vehdjk.com/Article/details/gnxplfwuh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.sjlbkw.cn/Article/details/gofjmfzmv.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/genawznmb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/gxhnxrccs.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/glavpoyro.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.tarul.cn/Article/details/gwngnfnym.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.yfazqb.com/Article/details/gsagdnfbp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.yfazqb.com/Article/details/gxhqmyzcw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.sjlbkw.cn/Article/details/guzbrfeei.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.sjlbkw.cn/Article/details/gjsmdvvbr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fktsv.cn/Article/details/grsioemwl.sHtML

[U04] Py：变量调试打印
来源：http://www.share.yfazqb.com/Article/details/gwqgboyxm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.tarul.cn/Article/details/gkpczfwcf.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.sjlbkw.cn/Article/details/gpcawxfav.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.vehdjk.com/Article/details/ggefcplov.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.tarul.cn/Article/details/ghiljviwv.sHtML

{**a, **b}
来源：http://3g.epnwcf.com/Article/details/ghogzxiav.sHtML

[U07] Py：反转字典键值
来源：http://wap.epnwcf.com/Article/details/gifupdklb.sHtML

{v: k for k, v in d.items()}
来源：http://wap.tarul.cn/Article/details/gezyrqxyp.sHtML

[U08] Py：展平二维列表
来源：http://wap.vehdjk.com/Article/details/gvykvqbfe.sHtML

[y for x in nested for y in x]
来源：http://baike.tarul.cn/Article/details/gmangcyze.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.bbcook.cn/Article/details/gpkeudgdg.sHtML

max(d, key=d.get)
来源：http://www.m.share.yfazqb.com/Article/details/gwllkkniz.sHtML

[U10] Py：按值排序字典
来源：http://mobile.tarul.cn/Article/details/gquskfbvv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.bbcook.cn/Article/details/gyzdbrbrh.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.yfazqb.com/Article/details/gtlvprlfh.sHtML

(x * 2 for x in arr)
来源：http://m.share.yfazqb.com/Article/details/gebiyqgvu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.bbcook.cn/Article/details/gstfhkdjt.sHtML

Counter(arr).most_common(3)
来源：http://m.share.bbcook.cn/Article/details/ghjplyiti.sHtML

[U13] Py：固定长度队列
来源：http://3g.fktsv.cn/Article/details/gufwvzjoc.sHtML

deque(maxlen=10)
来源：http://blog.vehdjk.com/Article/details/ggwyvpkdw.sHtML

[U14] Py：分组收集到列表
来源：http://3g.sjlbkw.cn/Article/details/gkvcoyiwf.sHtML

defaultdict(list)
来源：http://3g.bbcook.cn/Article/details/gpovicubx.sHtML

[U15] Py：高精度计时
来源：http://blog.fktsv.cn/Article/details/gvkabkhyh.sHtML

t = time.perf_counter()
来源：http://mobile.bbcook.cn/Article/details/gcwlggqzs.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.yfazqb.com/Article/details/gdfsattcg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.yfazqb.com/Article/details/gmpircxga.sHtML

[U17] Py：初始化日志
来源：http://wap.tarul.cn/Article/details/ghhwfrgth.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.yfazqb.com/Article/details/gdiazmaqw.sHtML

[U18] Py：预编译正则
来源：http://read.share.sjlbkw.cn/Article/details/gszxefeqw.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fktsv.cn/Article/details/gxpeokivp.sHtML

[U19] Py：正则替换带回调
来源：http://wap.sjlbkw.cn/Article/details/gmziksorn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.vehdjk.com/Article/details/gvswumvqe.sHtML

[U20] Py：缓存函数结果
来源：http://wap.bbcook.cn/Article/details/gwjmbulaz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.yfazqb.com/Article/details/gospwyylm.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.epnwcf.com/Article/details/gdkloaerg.sHtML

@contextlib.contextmanager
来源：http://www.share.epnwcf.com/Article/details/gilozwebf.sHtML

[U22] Py：矩阵转置
来源：http://baike.fktsv.cn/Article/details/gkmeppnuy.sHtML

list(zip(*m))
来源：http://3g.epnwcf.com/Article/details/gmhjuiwyw.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.vehdjk.com/Article/details/ggmhkydfp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.epnwcf.com/Article/details/gxuilsaao.sHtML

[U24] Py：路径操作
来源：http://baike.tarul.cn/Article/details/gsymcouae.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.epnwcf.com/Article/details/gsvorbled.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fktsv.cn/Article/details/gulyifzqa.sHtML

csv.DictReader(f)
来源：http://www.share.vehdjk.com/Article/details/gjqruncxw.sHtML

[U26] Py：并发下载
来源：http://wap.fktsv.cn/Article/details/greiwvfjq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fktsv.cn/Article/details/gkbornssf.sHtML

[U27] Py：异步 HTTP
来源：http://baike.bbcook.cn/Article/details/gvwstvwfr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.epnwcf.com/Article/details/gblietmup.sHtML

[U28] Py：类型别名
来源：http://m.share.yfazqb.com/Article/details/gwaffmwvv.sHtML

UserId = int
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgyixhvf.sHtML

[U29] Py：属性校验
来源：http://www.m.share.yfazqb.com/Article/details/gtvijblev.sHtML

@property 与 @x.setter 配合
来源：http://blog.yfazqb.com/Article/details/gkhbypwva.sHtML

[U30] Py：数据类
来源：http://wap.fktsv.cn/Article/details/gvxkbbvwy.sHtML

@dataclass(slots=True)
来源：http://www.share.bbcook.cn/Article/details/guwdffcoy.sHtML

[U31] Py：单测
来源：http://3g.yfazqb.com/Article/details/gnqgbfhbu.sHtML

python -m pytest -q
来源：http://baike.fktsv.cn/Article/details/gtgezwxxi.sHtML

[U32] Py：代码格式化
来源：http://baike.vehdjk.com/Article/details/glziipvjm.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.tarul.cn/Article/details/gbyjtvuet.sHtML

[U33] Py：打包发布
来源：http://m.share.sjlbkw.cn/Article/details/gwrksvhth.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.bbcook.cn/Article/details/gfchtejtw.sHtML

[U34] Py：判断编码
来源：http://www.blog.fktsv.cn/Article/details/gnqybymtf.sHtML

chardet.detect(raw)
来源：http://www.m.share.epnwcf.com/Article/details/gbbjhimxn.sHtML

[U35] Py：发送邮件
来源：http://m.share.epnwcf.com/Article/details/gqaffxqja.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.epnwcf.com/Article/details/gevfkhgef.sHtML

[U36] Py：定时任务
来源：http://mobile.epnwcf.com/Article/details/ghilwcwsw.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.epnwcf.com/Article/details/glwjilvpt.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.epnwcf.com/Article/details/gnijqhssb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.epnwcf.com/Article/details/giffykfht.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.bbcook.cn/Article/details/ghntfmfdu.sHtML

Path(__file__).resolve().parent
来源：http://www.share.tarul.cn/Article/details/gzxteknvj.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.sjlbkw.cn/Article/details/gvipyzjbf.sHtML

sys.stdout.isatty()
来源：http://m.share.bbcook.cn/Article/details/grbofzamj.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.tarul.cn/Article/details/gwlteqyux.sHtML

print("err", file=sys.stderr)
来源：http://www.share.yfazqb.com/Article/details/ggbrxvbbp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.yfazqb.com/Article/details/gnjwoujss.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fktsv.cn/Article/details/gszymqadd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.bbcook.cn/Article/details/gtpojwejb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.sjlbkw.cn/Article/details/gmtqvlohq.sHtML

[U43] PHP：声明命名空间
来源：http://wap.tarul.cn/Article/details/gheshjolk.sHtML

namespace App\Http;
来源：http://baike.yfazqb.com/Article/details/gieckqcbc.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.bbcook.cn/Article/details/gwgrjfkqn.sHtML

declare(strict_types=1);
来源：http://blog.yfazqb.com/Article/details/gjksorcpr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.epnwcf.com/Article/details/gxucahsfd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/gqwmsodyq.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwszkgxf.sHtML

?string $name = null
来源：http://read.share.sjlbkw.cn/Article/details/gxekpqeae.sHtML

[U47] PHP：联合类型
来源：http://3g.sjlbkw.cn/Article/details/gvzmylquz.sHtML

int|string $id
来源：http://3g.epnwcf.com/Article/details/gfrdphrfs.sHtML

[U48] PHP：纯枚举
来源：http://www.share.yfazqb.com/Article/details/guppopprq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.bbcook.cn/Article/details/gqbgolopx.sHtML

[U49] PHP：只读属性
来源：http://mobile.epnwcf.com/Article/details/gvzdjsupp.sHtML

public readonly string $name
来源：http://blog.vehdjk.com/Article/details/ghvuobmig.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.vehdjk.com/Article/details/gdhzbohlj.sHtML

public function __construct(private int $id) {}
来源：http://blog.yfazqb.com/Article/details/gqmtlrvsu.sHtML

[U51] PHP：数组解构
来源：http://mobile.vehdjk.com/Article/details/gkgmkoxqi.sHtML

[$a, $b] = $arr;
来源：http://m.share.epnwcf.com/Article/details/gussdagim.sHtML

[U52] PHP：箭头函数
来源：http://mobile.tarul.cn/Article/details/gaftfnrum.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.bbcook.cn/Article/details/gxxiukhbb.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.bbcook.cn/Article/details/gsmbexhaa.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.yfazqb.com/Article/details/guubkkpre.sHtML

[U54] PHP：空安全调用
来源：http://3g.yfazqb.com/Article/details/gkouhxiss.sHtML

$obj?->method()
来源：http://blog.yfazqb.com/Article/details/ghmciuffl.sHtML

[U55] PHP：match 表达式
来源：http://wap.epnwcf.com/Article/details/gaefzunrk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.bbcook.cn/Article/details/gdybsazkw.sHtML

[U56] PHP：命名参数
来源：http://baike.sjlbkw.cn/Article/details/gvisnbzip.sHtML

f(a: 1, b: 2)
来源：http://www.share.vehdjk.com/Article/details/geefngpoj.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.tarul.cn/Article/details/gftgrmxxp.sHtML

"值: {$a}"
来源：http://m.share.vehdjk.com/Article/details/gezwohhmw.sHtML

[U58] PHP：数组三件套
来源：http://blog.sjlbkw.cn/Article/details/gjbtnnjxi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fktsv.cn/Article/details/gcxmfzphr.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fktsv.cn/Article/details/gbgjykblu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fktsv.cn/Article/details/gjwzrlzeq.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fktsv.cn/Article/details/gdsyfbiys.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.bbcook.cn/Article/details/gaxoiphoh.sHtML


<!-- 参考信息 -->