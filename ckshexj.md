代发 wailian999

[S43] C++：智能指针
来源：http://mobile.sjlbkw.cn/Article/details/gjngcrrcl.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.bbcook.cn/Article/details/gangdhfsb.sHtML

[S44] C++：引用传参
来源：http://3g.yfazqb.com/Article/details/gpqshloft.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.bbcook.cn/Article/details/gjwpjaehg.sHtML

[S45] C++：lambda
来源：http://read.share.bbcook.cn/Article/details/gqblbkqlo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fktsv.cn/Article/details/gvnzkyicv.sHtML

[S46] C++：函数模板
来源：http://www.share.yfazqb.com/Article/details/gtwvpyfyp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.tarul.cn/Article/details/gxnxfbosa.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.bbcook.cn/Article/details/gqzmzfbvk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.epnwcf.com/Article/details/gxrbqvvra.sHtML

[S48] C++：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gjjcqxgnx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fktsv.cn/Article/details/gkwjitvjt.sHtML

while (std::getline(in, line)) { }
来源：http://3g.tarul.cn/Article/details/gurtywsot.sHtML

[S49] C++：写文件
来源：http://mobile.epnwcf.com/Article/details/gstoziqrm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.bbcook.cn/Article/details/gqluiigrc.sHtML

[S50] C++：格式化数字
来源：http://3g.epnwcf.com/Article/details/giqsusrsw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.epnwcf.com/Article/details/ghpgwrynq.sHtML

[S51] C++：显式类型转换
来源：http://wap.yfazqb.com/Article/details/gznnnnzjf.sHtML

static_cast<double>(a) / b
来源：http://baike.vehdjk.com/Article/details/gpnmddwne.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.sjlbkw.cn/Article/details/gzpmljzwp.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fktsv.cn/Article/details/gtqtsodjb.sHtML

[S53] C++：移动语义
来源：http://blog.sjlbkw.cn/Article/details/gktbnikxh.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fktsv.cn/Article/details/gdshosceo.sHtML

[S54] C++：异常处理
来源：http://mobile.tarul.cn/Article/details/gyxfrxkay.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.epnwcf.com/Article/details/gmpchffmq.sHtML

[S55] C++：结构化绑定
来源：http://blog.vehdjk.com/Article/details/gwkcwvjlk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.yfazqb.com/Article/details/ggqlrjbsd.sHtML

[S56] C++：optional
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtciyoak.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.yfazqb.com/Article/details/gcovyfhed.sHtML

[S57] C++：编译期常量
来源：http://www.share.yfazqb.com/Article/details/gkeeduybm.sHtML

constexpr int N = 10;
来源：http://wap.bbcook.cn/Article/details/ghlziapbk.sHtML

[S58] C++：命名空间
来源：http://blog.vehdjk.com/Article/details/gsugoomcg.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.sjlbkw.cn/Article/details/grnynpaht.sHtML

[S59] C++：静态断言
来源：http://m.share.sjlbkw.cn/Article/details/grnnlalhj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.yfazqb.com/Article/details/gquqnreev.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.tarul.cn/Article/details/ghfgujzqi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fktsv.cn/Article/details/gjjwoaovl.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gbkuilcqp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.tarul.cn/Article/details/gcnkwzldk.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/guspcbiwh.sHtML

[T01] Kotlin：Hello World
来源：http://baike.vehdjk.com/Article/details/gqdchkoef.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/ggucgotpe.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwyvmwbs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.tarul.cn/Article/details/gltflbxeo.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fktsv.cn/Article/details/gsjmtopcy.sHtML

"值: $b"
来源：http://blog.tarul.cn/Article/details/gbaaiuags.sHtML

[T04] Kotlin：空安全
来源：http://wap.yfazqb.com/Article/details/gjlvbrbwv.sHtML

val n: String? = null;  n?.length
来源：http://wap.sjlbkw.cn/Article/details/ghqjmgzqa.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.epnwcf.com/Article/details/gjhthcztv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.sjlbkw.cn/Article/details/ghxwciaze.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fktsv.cn/Article/details/gatztwfee.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.tarul.cn/Article/details/gdcniaiwc.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.vehdjk.com/Article/details/glbjdjgoi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.epnwcf.com/Article/details/gpmwbchnd.sHtML

[T08] Kotlin：数据类
来源：http://wap.epnwcf.com/Article/details/gjonnjqlc.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.bbcook.cn/Article/details/gdnwgahwv.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.yfazqb.com/Article/details/geglnqfbz.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.tarul.cn/Article/details/gxslcgjvt.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.yfazqb.com/Article/details/gemakrqgx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.vehdjk.com/Article/details/gxhfiymyn.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fktsv.cn/Article/details/ghsaruwca.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.bbcook.cn/Article/details/grwueovmq.sHtML

[T12] Kotlin：解构声明
来源：http://wap.sjlbkw.cn/Article/details/ghirpqlpl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gbfmsbzlw.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.vehdjk.com/Article/details/gecuogttp.sHtML

val m = mapOf("a" to 1)
来源：http://wap.yfazqb.com/Article/details/glrnuzeec.sHtML

[T14] Kotlin：循环
来源：http://www.share.fktsv.cn/Article/details/gfnincbom.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.vehdjk.com/Article/details/gvdvgavcc.sHtML

[T15] Kotlin：接口
来源：http://www.share.tarul.cn/Article/details/gncqydssb.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.vehdjk.com/Article/details/gicohkwoi.sHtML

[T16] Swift：Hello World
来源：http://www.share.fktsv.cn/Article/details/gyncmdseo.sHtML

print("Hello")
来源：http://baike.bbcook.cn/Article/details/gjfvhkeic.sHtML

[T17] Swift：变量与常量
来源：http://m.share.bbcook.cn/Article/details/gkuxzezuy.sHtML

var a = 1;  let b = 2
来源：http://blog.tarul.cn/Article/details/gobfvqxhp.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.epnwcf.com/Article/details/gplidnkea.sHtML

"值: \(b)"
来源：http://read.share.sjlbkw.cn/Article/details/gsksdyccu.sHtML

[T19] Swift：可选绑定
来源：http://wap.fktsv.cn/Article/details/gbryymggq.sHtML

if let n = opt { print(n) }
来源：http://3g.epnwcf.com/Article/details/gmaigffrk.sHtML

[T20] Swift：数组操作
来源：http://www.blog.bbcook.cn/Article/details/ghfllnpsj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fktsv.cn/Article/details/gmdsqlvof.sHtML

[T21] Swift：遍历
来源：http://m.share.sjlbkw.cn/Article/details/gbduaeuie.sHtML

for x in a { print(x) }
来源：http://wap.sjlbkw.cn/Article/details/gwsqhfpqw.sHtML

[T22] Swift：字典
来源：http://baike.fktsv.cn/Article/details/gwloobesz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gosjgmqqw.sHtML

[T23] Swift：函数
来源：http://www.blog.vehdjk.com/Article/details/gvklgnsjf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.tarul.cn/Article/details/gghgrxgqj.sHtML

[T24] Swift：闭包
来源：http://www.m.share.epnwcf.com/Article/details/gkwgiiizu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.yfazqb.com/Article/details/gvwwzmjry.sHtML

[T25] Swift：结构体
来源：http://read.share.bbcook.cn/Article/details/glsqsxlxq.sHtML

struct P { var x: Int }
来源：http://blog.tarul.cn/Article/details/goobpnqmv.sHtML

[T26] Swift：类与重写
来源：http://3g.sjlbkw.cn/Article/details/gnzwsgtqw.sHtML

class A: Base { override func f() {} }
来源：http://blog.sjlbkw.cn/Article/details/ginicjkao.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.vehdjk.com/Article/details/gplhjnupg.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.epnwcf.com/Article/details/ghihqdyzq.sHtML

[T28] Swift：枚举
来源：http://read.share.fktsv.cn/Article/details/gcrfijtuv.sHtML

enum Color { case red, green }
来源：http://3g.bbcook.cn/Article/details/gdyhotlqu.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.epnwcf.com/Article/details/gchibubfa.sHtML

guard let x = opt else { return }
来源：http://read.share.tarul.cn/Article/details/gnxhmxehu.sHtML

[T30] Swift：协议
来源：http://www.blog.epnwcf.com/Article/details/gykuhybku.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.tarul.cn/Article/details/gfbocmdeq.sHtML

[T31] Lua：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gartthdra.sHtML

print("Hello")
来源：http://mobile.bbcook.cn/Article/details/gsngxcjxz.sHtML

[T32] Lua：局部变量
来源：http://m.share.fktsv.cn/Article/details/gtyieywwp.sHtML

local a = 1
来源：http://baike.bbcook.cn/Article/details/giltsbvio.sHtML

[T33] Lua：表（数组）
来源：http://blog.epnwcf.com/Article/details/gsaytvojw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.epnwcf.com/Article/details/gpyodwupo.sHtML

[T34] Lua：遍历表
来源：http://3g.fktsv.cn/Article/details/gfjbpuonx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.sjlbkw.cn/Article/details/gsqjcvdhh.sHtML

[T35] Lua：字典表
来源：http://www.share.fktsv.cn/Article/details/glnxmkwlq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.epnwcf.com/Article/details/gaqwhobfh.sHtML

[T36] Lua：函数
来源：http://blog.tarul.cn/Article/details/gwyqybkhp.sHtML

function add(a, b) return a + b end
来源：http://3g.bbcook.cn/Article/details/gglwvxgtj.sHtML

[T37] Lua：字符串拼接
来源：http://3g.sjlbkw.cn/Article/details/gzjxefarx.sHtML

"a" .. "b"
来源：http://wap.fktsv.cn/Article/details/gzfmfuhxp.sHtML

[T38] Lua：条件
来源：http://read.share.yfazqb.com/Article/details/gyczzkhya.sHtML

if x > 0 then print("正") end
来源：http://www.share.sjlbkw.cn/Article/details/gczgngsam.sHtML

[T39] Lua：模式匹配
来源：http://blog.epnwcf.com/Article/details/ghidvxvdw.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fktsv.cn/Article/details/gknbglqmf.sHtML

[T40] Lua：元表
来源：http://www.blog.sjlbkw.cn/Article/details/gbjbbuzaz.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.tarul.cn/Article/details/gknfoofze.sHtML

[T41] Perl：Hello World
来源：http://blog.bbcook.cn/Article/details/gsrpxutrh.sHtML

print "Hello\n";
来源：http://www.blog.sjlbkw.cn/Article/details/grdciwart.sHtML

[T42] Perl：变量类型
来源：http://blog.yfazqb.com/Article/details/gzajskuml.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.sjlbkw.cn/Article/details/gbqdwrrkx.sHtML

[T43] Perl：字符串插值
来源：http://wap.epnwcf.com/Article/details/ggrrztvym.sHtML

"值: $a"
来源：http://m.share.fktsv.cn/Article/details/gyulntdaq.sHtML

[T44] Perl：条件
来源：http://www.m.share.epnwcf.com/Article/details/guxdjknuf.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.vehdjk.com/Article/details/gpufqdppj.sHtML

[T45] Perl：数组遍历
来源：http://www.share.bbcook.cn/Article/details/gzfuyhsxl.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.yfazqb.com/Article/details/ggopwhdcy.sHtML

[T46] Perl：哈希操作
来源：http://www.share.epnwcf.com/Article/details/gqrhyudlf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.tarul.cn/Article/details/goohkdvxj.sHtML

[T47] Perl：正则捕获
来源：http://m.share.vehdjk.com/Article/details/gqzrairxf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.bbcook.cn/Article/details/gkudmowfr.sHtML

[T48] Perl：正则替换
来源：http://mobile.yfazqb.com/Article/details/gcdljmkvv.sHtML

$s =~ s/old/new/g;
来源：http://read.share.vehdjk.com/Article/details/gglzbnymp.sHtML

[T49] Perl：函数
来源：http://read.share.bbcook.cn/Article/details/gzkuqnxzh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gvrdgqxvy.sHtML

[T50] Perl：逐行读文件
来源：http://wap.tarul.cn/Article/details/gpzluorra.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.bbcook.cn/Article/details/gpvewxeoo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.yfazqb.com/Article/details/guwnkyjuk.sHtML

[T51] Scala：Hello World
来源：http://3g.epnwcf.com/Article/details/gzjwrtglz.sHtML

println("Hello")
来源：http://m.share.yfazqb.com/Article/details/gykanvozd.sHtML

[T52] Scala：变量
来源：http://wap.bbcook.cn/Article/details/gqltrcrqo.sHtML

val a = 1;  var b = 2
来源：http://blog.vehdjk.com/Article/details/gsnzdikml.sHtML

[T53] Scala：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gevaqtpxe.sHtML

s"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/gndxnpxdv.sHtML

[T54] Scala：集合映射
来源：http://m.share.yfazqb.com/Article/details/gvzymdbxl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.yfazqb.com/Article/details/gogngzmlf.sHtML

[T55] Scala：集合过滤
来源：http://wap.bbcook.cn/Article/details/ghtebazak.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.bbcook.cn/Article/details/gadqtfnla.sHtML

[T56] Scala：样例类
来源：http://blog.epnwcf.com/Article/details/geasexhwh.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.epnwcf.com/Article/details/gshfdiicw.sHtML

[T57] Scala：模式匹配
来源：http://3g.epnwcf.com/Article/details/grfleipfb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.epnwcf.com/Article/details/glhawkopa.sHtML

[T58] Scala：函数定义
来源：http://m.share.vehdjk.com/Article/details/grbkrfwdc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.yfazqb.com/Article/details/gkqcyoxid.sHtML

[T59] Scala：循环
来源：http://www.m.share.vehdjk.com/Article/details/ghfxwkcdi.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.vehdjk.com/Article/details/giqczupty.sHtML

[T60] Scala：折叠
来源：http://baike.epnwcf.com/Article/details/ghgmhtrdr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.bbcook.cn/Article/details/gixelpopx.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gbayrgoyx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.vehdjk.com/Article/details/ggtjgnsih.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gdlkeaprv.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.yfazqb.com/Article/details/gsdeesalp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fktsv.cn/Article/details/gzizscsxw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.tarul.cn/Article/details/geousejnq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.epnwcf.com/Article/details/gfgqmkkcr.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.bbcook.cn/Article/details/gccgbgyty.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.tarul.cn/Article/details/gasqzkpmk.sHtML

[U04] Py：变量调试打印
来源：http://wap.epnwcf.com/Article/details/gqdzgwhxs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.vehdjk.com/Article/details/gvaypddhe.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.sjlbkw.cn/Article/details/gtqlouuep.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/gsqsigxhu.sHtML

[U06] Py：合并两个字典
来源：http://baike.sjlbkw.cn/Article/details/gevcluxmy.sHtML

{**a, **b}
来源：http://baike.tarul.cn/Article/details/gaitdfolr.sHtML

[U07] Py：反转字典键值
来源：http://mobile.bbcook.cn/Article/details/gyozwybgh.sHtML

{v: k for k, v in d.items()}
来源：http://3g.sjlbkw.cn/Article/details/gottcddsr.sHtML

[U08] Py：展平二维列表
来源：http://blog.vehdjk.com/Article/details/gmckkmqyl.sHtML

[y for x in nested for y in x]
来源：http://3g.epnwcf.com/Article/details/gprfrowya.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.vehdjk.com/Article/details/govsbgojn.sHtML

max(d, key=d.get)
来源：http://m.share.epnwcf.com/Article/details/gjzqwifgs.sHtML

[U10] Py：按值排序字典
来源：http://blog.vehdjk.com/Article/details/gwfjmjdqt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.tarul.cn/Article/details/gbmnjvbxg.sHtML

[U11] Py：生成器表达式
来源：http://baike.bbcook.cn/Article/details/gsqriddiy.sHtML

(x * 2 for x in arr)
来源：http://www.share.sjlbkw.cn/Article/details/gwakydyde.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.epnwcf.com/Article/details/gvsmbcvyu.sHtML

Counter(arr).most_common(3)
来源：http://read.share.yfazqb.com/Article/details/gtbjcczaa.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fktsv.cn/Article/details/ghplgdmmn.sHtML

deque(maxlen=10)
来源：http://www.blog.fktsv.cn/Article/details/gedlwgyhl.sHtML

[U14] Py：分组收集到列表
来源：http://blog.tarul.cn/Article/details/goygnywul.sHtML

defaultdict(list)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcucknzwn.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.yfazqb.com/Article/details/ggtxfequf.sHtML

t = time.perf_counter()
来源：http://blog.vehdjk.com/Article/details/gbboqtlao.sHtML

[U16] Py：命令行参数解析
来源：http://wap.epnwcf.com/Article/details/ggdeargoo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.epnwcf.com/Article/details/grjylkmat.sHtML

[U17] Py：初始化日志
来源：http://read.share.fktsv.cn/Article/details/gzsgfvqif.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.vehdjk.com/Article/details/gguvyerjq.sHtML

[U18] Py：预编译正则
来源：http://baike.tarul.cn/Article/details/gppoatqfm.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fktsv.cn/Article/details/gepuujkqb.sHtML

[U19] Py：正则替换带回调
来源：http://baike.tarul.cn/Article/details/gvqwgrdvc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.yfazqb.com/Article/details/gpqhnnbhj.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.vehdjk.com/Article/details/grkgeueaa.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.vehdjk.com/Article/details/grxizaqzo.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.sjlbkw.cn/Article/details/gpdrejscr.sHtML

@contextlib.contextmanager
来源：http://m.share.vehdjk.com/Article/details/gwbzoechk.sHtML

[U22] Py：矩阵转置
来源：http://www.share.yfazqb.com/Article/details/glqmltkfw.sHtML

list(zip(*m))
来源：http://mobile.sjlbkw.cn/Article/details/ggrjaexgu.sHtML

[U23] Py：分块读取大文件
来源：http://baike.bbcook.cn/Article/details/gksdwsxua.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.vehdjk.com/Article/details/grrqlqmpe.sHtML

[U24] Py：路径操作
来源：http://mobile.epnwcf.com/Article/details/gbwcerrjg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.vehdjk.com/Article/details/gwhwsispy.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.yfazqb.com/Article/details/goqfzluyr.sHtML

csv.DictReader(f)
来源：http://mobile.yfazqb.com/Article/details/gwzjorqcr.sHtML

[U26] Py：并发下载
来源：http://wap.vehdjk.com/Article/details/gzeaplwpi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.sjlbkw.cn/Article/details/gyvjhscyr.sHtML

[U27] Py：异步 HTTP
来源：http://baike.tarul.cn/Article/details/gmllmhrxf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.vehdjk.com/Article/details/gwqxfvwhc.sHtML

[U28] Py：类型别名
来源：http://mobile.bbcook.cn/Article/details/gsiollxby.sHtML

UserId = int
来源：http://www.share.fktsv.cn/Article/details/grnrretwk.sHtML

[U29] Py：属性校验
来源：http://read.share.tarul.cn/Article/details/gtrnqdbpx.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.vehdjk.com/Article/details/gwjhfezid.sHtML

[U30] Py：数据类
来源：http://wap.fktsv.cn/Article/details/gtfxyrjyr.sHtML

@dataclass(slots=True)
来源：http://www.blog.yfazqb.com/Article/details/gkfyngbcp.sHtML

[U31] Py：单测
来源：http://wap.fktsv.cn/Article/details/gapcxjkls.sHtML

python -m pytest -q
来源：http://www.m.share.fktsv.cn/Article/details/gdmmmwuyk.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fktsv.cn/Article/details/gmfzrwxvj.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.sjlbkw.cn/Article/details/grftmjwvn.sHtML

[U33] Py：打包发布
来源：http://baike.sjlbkw.cn/Article/details/gtladtqyl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fktsv.cn/Article/details/gjipbssvq.sHtML

[U34] Py：判断编码
来源：http://www.blog.vehdjk.com/Article/details/gcopqaqgt.sHtML

chardet.detect(raw)
来源：http://wap.fktsv.cn/Article/details/gdhrpaagf.sHtML

[U35] Py：发送邮件
来源：http://www.share.fktsv.cn/Article/details/gnwrpqecd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.epnwcf.com/Article/details/ghqnakatx.sHtML

[U36] Py：定时任务
来源：http://www.share.sjlbkw.cn/Article/details/ganxynzew.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fktsv.cn/Article/details/guaetnmjj.sHtML

[U37] Py：读写 Excel
来源：http://mobile.vehdjk.com/Article/details/gihpahnqf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fktsv.cn/Article/details/gdkxxrrgu.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.bbcook.cn/Article/details/gumfabajb.sHtML

Path(__file__).resolve().parent
来源：http://3g.yfazqb.com/Article/details/gfzpmcjfl.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.yfazqb.com/Article/details/gvvzohaww.sHtML

sys.stdout.isatty()
来源：http://blog.bbcook.cn/Article/details/gcpetkprx.sHtML

[U40] Py：打印到标准错误
来源：http://wap.epnwcf.com/Article/details/gdyinvrzv.sHtML

print("err", file=sys.stderr)
来源：http://mobile.vehdjk.com/Article/details/gulsthxzk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.epnwcf.com/Article/details/gkbvndymg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.tarul.cn/Article/details/gtclfffky.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.tarul.cn/Article/details/gfapunogv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.epnwcf.com/Article/details/ghlyrahgy.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gaknqnlwq.sHtML

namespace App\Http;
来源：http://wap.tarul.cn/Article/details/gtenttdki.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.tarul.cn/Article/details/ghovnwxbk.sHtML

declare(strict_types=1);
来源：http://3g.yfazqb.com/Article/details/gyentzqjd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.epnwcf.com/Article/details/givrufrzw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gcodukiis.sHtML

[U46] PHP：可空类型
来源：http://mobile.vehdjk.com/Article/details/gbrpapkkt.sHtML

?string $name = null
来源：http://blog.fktsv.cn/Article/details/gdmrbrhwy.sHtML

[U47] PHP：联合类型
来源：http://baike.epnwcf.com/Article/details/gbzmxbzqi.sHtML

int|string $id
来源：http://m.share.epnwcf.com/Article/details/gquicxcym.sHtML

[U48] PHP：纯枚举
来源：http://3g.yfazqb.com/Article/details/goxkagvjt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.tarul.cn/Article/details/ghqgzsjja.sHtML

[U49] PHP：只读属性
来源：http://m.share.fktsv.cn/Article/details/gflfelcvc.sHtML

public readonly string $name
来源：http://3g.yfazqb.com/Article/details/gcygsllfq.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.epnwcf.com/Article/details/grcayhuzc.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.yfazqb.com/Article/details/gnixipwzm.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fktsv.cn/Article/details/gomsyoysi.sHtML

[$a, $b] = $arr;
来源：http://m.share.yfazqb.com/Article/details/gkawxlagd.sHtML

[U52] PHP：箭头函数
来源：http://blog.epnwcf.com/Article/details/guuzjboae.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.epnwcf.com/Article/details/gtcehpash.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.vehdjk.com/Article/details/ggrltjpyf.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.bbcook.cn/Article/details/gcxyqcdkd.sHtML

[U54] PHP：空安全调用
来源：http://www.share.vehdjk.com/Article/details/grcoxrwgq.sHtML

$obj?->method()
来源：http://www.blog.sjlbkw.cn/Article/details/gybyaybuj.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fktsv.cn/Article/details/gzohksbxn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.bbcook.cn/Article/details/gmfmifoft.sHtML

[U56] PHP：命名参数
来源：http://read.share.bbcook.cn/Article/details/gggpwvfka.sHtML

f(a: 1, b: 2)
来源：http://mobile.epnwcf.com/Article/details/gtnpszrag.sHtML

[U57] PHP：字符串插值
来源：http://m.share.vehdjk.com/Article/details/gwgmetbab.sHtML

"值: {$a}"
来源：http://baike.yfazqb.com/Article/details/goqukuwva.sHtML

[U58] PHP：数组三件套
来源：http://blog.tarul.cn/Article/details/gfvuwffln.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.tarul.cn/Article/details/gkwpirkpu.sHtML

[U59] PHP：自定义排序
来源：http://baike.fktsv.cn/Article/details/gkvcqznzp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.sjlbkw.cn/Article/details/gwxuobmdb.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.sjlbkw.cn/Article/details/gbrltzcvu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.epnwcf.com/Article/details/givtsnoic.sHtML

[U61] PHP：正则
来源：http://3g.sjlbkw.cn/Article/details/gedgcclow.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/gpcwjarsh.sHtML

[U62] PHP：日期对象
来源：http://wap.vehdjk.com/Article/details/gxwfjzvcm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.vehdjk.com/Article/details/gogmtourt.sHtML

[U63] PHP：文件读写
来源：http://m.share.yfazqb.com/Article/details/gtosghwat.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.epnwcf.com/Article/details/gcaoykako.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.epnwcf.com/Article/details/gszuijihm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.bbcook.cn/Article/details/grdejztvi.sHtML

[U65] PHP：会话
来源：http://www.m.share.epnwcf.com/Article/details/gxjbbeytm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gvgpuhixt.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.vehdjk.com/Article/details/gpgkaflik.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.sjlbkw.cn/Article/details/gcxyrvbmy.sHtML

[U67] PHP：处理文件上传
来源：http://baike.vehdjk.com/Article/details/gpgqelrky.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.vehdjk.com/Article/details/gezvmebhm.sHtML

[U68] PHP：PDO 连接
来源：http://blog.epnwcf.com/Article/details/grffqmpkm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.yfazqb.com/Article/details/gasftcqzq.sHtML


<!-- 参考信息 -->