代发 wailian999

[S43] C++：智能指针
来源：http://3g.bbcook.cn/Article/details/gjhctroyy.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.vehdjk.com/Article/details/gqnlssudw.sHtML

[S44] C++：引用传参
来源：http://www.share.tarul.cn/Article/details/gxeycprnh.sHtML

void inc(int &x) { ++x; }
来源：http://baike.vehdjk.com/Article/details/gxoumsjyr.sHtML

[S45] C++：lambda
来源：http://read.share.vehdjk.com/Article/details/gqvzcqwde.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.tarul.cn/Article/details/gcjscttir.sHtML

[S46] C++：函数模板
来源：http://3g.sjlbkw.cn/Article/details/gmjrubqlg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fktsv.cn/Article/details/grqazjare.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.sjlbkw.cn/Article/details/gtobayazl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.yfazqb.com/Article/details/gnbinnfpb.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gsiwicqby.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.bbcook.cn/Article/details/giclhiouu.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.bbcook.cn/Article/details/gfqimviqb.sHtML

[S49] C++：写文件
来源：http://m.share.epnwcf.com/Article/details/gtocdccat.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fktsv.cn/Article/details/gamoveziy.sHtML

[S50] C++：格式化数字
来源：http://wap.yfazqb.com/Article/details/guayggthh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gvnyuwxhq.sHtML

[S51] C++：显式类型转换
来源：http://read.share.tarul.cn/Article/details/gvhfcuwwh.sHtML

static_cast<double>(a) / b
来源：http://m.share.fktsv.cn/Article/details/giioxwwbr.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.yfazqb.com/Article/details/gwtattpvw.sHtML

int size() const noexcept { return n_; }
来源：http://wap.yfazqb.com/Article/details/gcxcdbvvj.sHtML

[S53] C++：移动语义
来源：http://mobile.bbcook.cn/Article/details/gvyjvgahu.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.vehdjk.com/Article/details/gjsqrheop.sHtML

[S54] C++：异常处理
来源：http://read.share.vehdjk.com/Article/details/gbwwiaoti.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.bbcook.cn/Article/details/gspnpzlvf.sHtML

[S55] C++：结构化绑定
来源：http://www.share.epnwcf.com/Article/details/gkkccrkrx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.epnwcf.com/Article/details/gjraxwbty.sHtML

[S56] C++：optional
来源：http://www.blog.fktsv.cn/Article/details/gfapdcxrn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.yfazqb.com/Article/details/gohzckzpg.sHtML

[S57] C++：编译期常量
来源：http://www.share.sjlbkw.cn/Article/details/gfceyqhgm.sHtML

constexpr int N = 10;
来源：http://www.share.sjlbkw.cn/Article/details/grkoehpxb.sHtML

[S58] C++：命名空间
来源：http://mobile.tarul.cn/Article/details/gzpnaxfkk.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fktsv.cn/Article/details/gcqigfgvu.sHtML

[S59] C++：静态断言
来源：http://www.share.epnwcf.com/Article/details/gziekuwbn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fktsv.cn/Article/details/gjwfjryjo.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.bbcook.cn/Article/details/gszylstcx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.vehdjk.com/Article/details/gmwjwjhta.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gjpalcygv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.epnwcf.com/Article/details/gzgckqmic.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gqoyyvijt.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fktsv.cn/Article/details/ghcxzvzuo.sHtML

println("Hello")
来源：http://www.share.bbcook.cn/Article/details/gvgbwjjbd.sHtML

[T02] Kotlin：变量
来源：http://read.share.yfazqb.com/Article/details/gmjjrxcfh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.yfazqb.com/Article/details/gcrryguic.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.bbcook.cn/Article/details/gutvvqjmm.sHtML

"值: $b"
来源：http://www.m.share.vehdjk.com/Article/details/ghouodmic.sHtML

[T04] Kotlin：空安全
来源：http://wap.yfazqb.com/Article/details/gpvuijnlv.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.bbcook.cn/Article/details/gygnamssu.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fktsv.cn/Article/details/gugtlorjk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fktsv.cn/Article/details/gdjxjfpxl.sHtML

[T06] Kotlin：集合映射
来源：http://baike.bbcook.cn/Article/details/gkxwrjzwm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.bbcook.cn/Article/details/gzqhngxwd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.epnwcf.com/Article/details/gfiinotdl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.yfazqb.com/Article/details/gliwmtnzn.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.sjlbkw.cn/Article/details/gisotwknl.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.sjlbkw.cn/Article/details/ghtmdaeyb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fktsv.cn/Article/details/gvzikwjkm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.sjlbkw.cn/Article/details/gtucngobg.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.tarul.cn/Article/details/gzopsmfrw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fktsv.cn/Article/details/gacyvdsai.sHtML

[T11] Kotlin：协程
来源：http://read.share.tarul.cn/Article/details/gxegafvwn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fktsv.cn/Article/details/gybnzhads.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fktsv.cn/Article/details/gkqeybwkg.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gacojoalj.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.vehdjk.com/Article/details/gqnmjmotk.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.epnwcf.com/Article/details/goeozmqhd.sHtML

[T14] Kotlin：循环
来源：http://baike.yfazqb.com/Article/details/goyierrfx.sHtML

for (i in 1..10) println(i)
来源：http://3g.sjlbkw.cn/Article/details/gfkqgvbtb.sHtML

[T15] Kotlin：接口
来源：http://www.share.epnwcf.com/Article/details/ghwcyumci.sHtML

interface Shape { fun area(): Double }
来源：http://3g.sjlbkw.cn/Article/details/gzsruwfsl.sHtML

[T16] Swift：Hello World
来源：http://www.share.bbcook.cn/Article/details/gdxoectlb.sHtML

print("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gcvjndtqs.sHtML

[T17] Swift：变量与常量
来源：http://m.share.bbcook.cn/Article/details/gqfgkoqyg.sHtML

var a = 1;  let b = 2
来源：http://mobile.vehdjk.com/Article/details/gnxevcghs.sHtML

[T18] Swift：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gelnbiymw.sHtML

"值: \(b)"
来源：http://www.blog.bbcook.cn/Article/details/gkiklckwc.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fktsv.cn/Article/details/gybxbierb.sHtML

if let n = opt { print(n) }
来源：http://3g.bbcook.cn/Article/details/gxknuavag.sHtML

[T20] Swift：数组操作
来源：http://mobile.sjlbkw.cn/Article/details/gdgornxaj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fktsv.cn/Article/details/gdkpfvwkm.sHtML

[T21] Swift：遍历
来源：http://baike.sjlbkw.cn/Article/details/gxvdmhcgi.sHtML

for x in a { print(x) }
来源：http://m.share.bbcook.cn/Article/details/gouuaqift.sHtML

[T22] Swift：字典
来源：http://m.share.fktsv.cn/Article/details/gfzbwnzpe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.tarul.cn/Article/details/gsvrzcnbc.sHtML

[T23] Swift：函数
来源：http://www.blog.vehdjk.com/Article/details/geilbruvg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fktsv.cn/Article/details/gkuasjlua.sHtML

[T24] Swift：闭包
来源：http://m.share.fktsv.cn/Article/details/gdrlwfcho.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.tarul.cn/Article/details/gsvjrupey.sHtML

[T25] Swift：结构体
来源：http://baike.vehdjk.com/Article/details/gzmoqaaso.sHtML

struct P { var x: Int }
来源：http://read.share.fktsv.cn/Article/details/gxbncdafl.sHtML

[T26] Swift：类与重写
来源：http://mobile.bbcook.cn/Article/details/gcnacbsud.sHtML

class A: Base { override func f() {} }
来源：http://m.share.vehdjk.com/Article/details/gtxyjtjeu.sHtML

[T27] Swift：错误处理
来源：http://m.share.epnwcf.com/Article/details/gjgptdxol.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.vehdjk.com/Article/details/glinrupnf.sHtML

[T28] Swift：枚举
来源：http://www.blog.bbcook.cn/Article/details/gptqwkaim.sHtML

enum Color { case red, green }
来源：http://m.share.bbcook.cn/Article/details/gtbexihhd.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fktsv.cn/Article/details/gaksdnxsl.sHtML

guard let x = opt else { return }
来源：http://baike.sjlbkw.cn/Article/details/gfjgwddto.sHtML

[T30] Swift：协议
来源：http://blog.yfazqb.com/Article/details/gpyxbjyle.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.yfazqb.com/Article/details/gwbygimuo.sHtML

[T31] Lua：Hello World
来源：http://3g.epnwcf.com/Article/details/gizbgjwcf.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/ghnwtkbax.sHtML

[T32] Lua：局部变量
来源：http://3g.yfazqb.com/Article/details/gkfbvnwor.sHtML

local a = 1
来源：http://wap.tarul.cn/Article/details/ginufhvre.sHtML

[T33] Lua：表（数组）
来源：http://read.share.tarul.cn/Article/details/guhqrcnop.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.yfazqb.com/Article/details/gcxzeprri.sHtML

[T34] Lua：遍历表
来源：http://www.share.yfazqb.com/Article/details/gywphiwqa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.vehdjk.com/Article/details/ginhwteew.sHtML

[T35] Lua：字典表
来源：http://mobile.epnwcf.com/Article/details/grlkfgzcd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fktsv.cn/Article/details/gfyjbiryw.sHtML

[T36] Lua：函数
来源：http://baike.bbcook.cn/Article/details/govcychcl.sHtML

function add(a, b) return a + b end
来源：http://baike.tarul.cn/Article/details/gbrjfukgi.sHtML

[T37] Lua：字符串拼接
来源：http://baike.tarul.cn/Article/details/gshihkssj.sHtML

"a" .. "b"
来源：http://www.share.bbcook.cn/Article/details/gahfaenvh.sHtML

[T38] Lua：条件
来源：http://read.share.yfazqb.com/Article/details/gytjoqidw.sHtML

if x > 0 then print("正") end
来源：http://read.share.fktsv.cn/Article/details/gofmbtthb.sHtML

[T39] Lua：模式匹配
来源：http://blog.tarul.cn/Article/details/gfsthfmps.sHtML

string.find(s, "%d+")
来源：http://blog.bbcook.cn/Article/details/gdrfzzyiw.sHtML

[T40] Lua：元表
来源：http://wap.epnwcf.com/Article/details/gmufrowcq.sHtML

setmetatable({}, { __index = base })
来源：http://blog.tarul.cn/Article/details/gjbkulxih.sHtML

[T41] Perl：Hello World
来源：http://www.share.bbcook.cn/Article/details/gbkptpxaw.sHtML

print "Hello\n";
来源：http://m.share.bbcook.cn/Article/details/guownmhwu.sHtML

[T42] Perl：变量类型
来源：http://mobile.bbcook.cn/Article/details/gjdgprits.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.bbcook.cn/Article/details/gnagkyuro.sHtML

[T43] Perl：字符串插值
来源：http://baike.tarul.cn/Article/details/gpgpckfvh.sHtML

"值: $a"
来源：http://baike.bbcook.cn/Article/details/gvcekzwhd.sHtML

[T44] Perl：条件
来源：http://blog.tarul.cn/Article/details/gfkerkdfh.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.tarul.cn/Article/details/ggvpuslbj.sHtML

[T45] Perl：数组遍历
来源：http://3g.yfazqb.com/Article/details/gsjrjesge.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.epnwcf.com/Article/details/gnnomyxsj.sHtML

[T46] Perl：哈希操作
来源：http://m.share.yfazqb.com/Article/details/gxgwufmii.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fktsv.cn/Article/details/gwwvgmbtd.sHtML

[T47] Perl：正则捕获
来源：http://read.share.tarul.cn/Article/details/gjgadtgre.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.epnwcf.com/Article/details/gryjkwoqq.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.tarul.cn/Article/details/gaxoeltja.sHtML

$s =~ s/old/new/g;
来源：http://baike.yfazqb.com/Article/details/gynoyefon.sHtML

[T49] Perl：函数
来源：http://www.m.share.yfazqb.com/Article/details/gyfevawww.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/gbwyurgef.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fktsv.cn/Article/details/ghbkpeyow.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fktsv.cn/Article/details/gltrezzpk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.vehdjk.com/Article/details/gfahwrgug.sHtML

[T51] Scala：Hello World
来源：http://mobile.tarul.cn/Article/details/gdpkbtxrr.sHtML

println("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gtnhozdlo.sHtML

[T52] Scala：变量
来源：http://blog.vehdjk.com/Article/details/gtpqzwoal.sHtML

val a = 1;  var b = 2
来源：http://read.share.tarul.cn/Article/details/gntsfaofs.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/govuvsaqu.sHtML

s"值: $b"
来源：http://blog.yfazqb.com/Article/details/gzzcuquca.sHtML

[T54] Scala：集合映射
来源：http://baike.vehdjk.com/Article/details/gklesxwur.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.sjlbkw.cn/Article/details/gasgftdka.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/gekqqcdjq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fktsv.cn/Article/details/gopufiuci.sHtML

[T56] Scala：样例类
来源：http://3g.sjlbkw.cn/Article/details/gzsldmbai.sHtML

case class User(name: String, age: Int)
来源：http://3g.tarul.cn/Article/details/gcxnekukt.sHtML

[T57] Scala：模式匹配
来源：http://www.share.sjlbkw.cn/Article/details/gididmqxt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fktsv.cn/Article/details/gyeakjajl.sHtML

[T58] Scala：函数定义
来源：http://mobile.epnwcf.com/Article/details/gduurvcce.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.bbcook.cn/Article/details/gmsmfqmms.sHtML

[T59] Scala：循环
来源：http://mobile.bbcook.cn/Article/details/ggccekrfr.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.tarul.cn/Article/details/gubsfioxk.sHtML

[T60] Scala：折叠
来源：http://www.blog.bbcook.cn/Article/details/gqrumpusx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.vehdjk.com/Article/details/gmpsidpcd.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gltycbuiu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.sjlbkw.cn/Article/details/gvvdzjuvh.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gegjnhobf.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.tarul.cn/Article/details/gloihreow.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.yfazqb.com/Article/details/gyacqtico.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fktsv.cn/Article/details/gpcnvukmm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.bbcook.cn/Article/details/gjpbrfjnv.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.epnwcf.com/Article/details/gbcckceeh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fktsv.cn/Article/details/gyjuxewhn.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fktsv.cn/Article/details/gukmskaqr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.epnwcf.com/Article/details/gwbgoephn.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.vehdjk.com/Article/details/gxbxdsozz.sHtML

list(dict.fromkeys(arr))
来源：http://blog.vehdjk.com/Article/details/gyqsylmys.sHtML

[U06] Py：合并两个字典
来源：http://baike.epnwcf.com/Article/details/gcympwquq.sHtML

{**a, **b}
来源：http://www.share.tarul.cn/Article/details/gqorjkvxy.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.sjlbkw.cn/Article/details/gsklyhrtw.sHtML

{v: k for k, v in d.items()}
来源：http://blog.epnwcf.com/Article/details/gxvjyxqra.sHtML

[U08] Py：展平二维列表
来源：http://read.share.tarul.cn/Article/details/gezummror.sHtML

[y for x in nested for y in x]
来源：http://m.share.fktsv.cn/Article/details/gpvmpvolu.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fktsv.cn/Article/details/gaxyoewbx.sHtML

max(d, key=d.get)
来源：http://wap.vehdjk.com/Article/details/gjihoabex.sHtML

[U10] Py：按值排序字典
来源：http://www.share.bbcook.cn/Article/details/gfayvvhkg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.tarul.cn/Article/details/gphnbeihi.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.vehdjk.com/Article/details/glwpakpyt.sHtML

(x * 2 for x in arr)
来源：http://www.share.epnwcf.com/Article/details/gseshkghr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.yfazqb.com/Article/details/gkfskfvtg.sHtML

Counter(arr).most_common(3)
来源：http://blog.bbcook.cn/Article/details/gvwigamkv.sHtML

[U13] Py：固定长度队列
来源：http://read.share.epnwcf.com/Article/details/gzewmhbtr.sHtML

deque(maxlen=10)
来源：http://mobile.bbcook.cn/Article/details/gtvvhfsgi.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fktsv.cn/Article/details/gjwakuxqr.sHtML

defaultdict(list)
来源：http://wap.yfazqb.com/Article/details/gqrwqderz.sHtML

[U15] Py：高精度计时
来源：http://blog.sjlbkw.cn/Article/details/gwzoiqizi.sHtML

t = time.perf_counter()
来源：http://mobile.yfazqb.com/Article/details/gkkdxofwo.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.epnwcf.com/Article/details/gwjpeskhp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.epnwcf.com/Article/details/ggzvhlkrr.sHtML

[U17] Py：初始化日志
来源：http://blog.epnwcf.com/Article/details/gonbtucdm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fktsv.cn/Article/details/gswxqafzy.sHtML

[U18] Py：预编译正则
来源：http://baike.yfazqb.com/Article/details/gofojshdf.sHtML

pat = re.compile(r"\d+")
来源：http://blog.vehdjk.com/Article/details/gtwcnblsw.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.sjlbkw.cn/Article/details/gmtjarcpm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.sjlbkw.cn/Article/details/gbeuxwgcf.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fktsv.cn/Article/details/gsxmztlmh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.epnwcf.com/Article/details/gpxyavunu.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.epnwcf.com/Article/details/givbmsqrf.sHtML

@contextlib.contextmanager
来源：http://3g.vehdjk.com/Article/details/gfmrzokjp.sHtML

[U22] Py：矩阵转置
来源：http://www.share.sjlbkw.cn/Article/details/glgzudsyc.sHtML

list(zip(*m))
来源：http://baike.sjlbkw.cn/Article/details/glwenddic.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.yfazqb.com/Article/details/gpihrweyf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.yfazqb.com/Article/details/gbneyfbmk.sHtML

[U24] Py：路径操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvpqbecg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.bbcook.cn/Article/details/glakmkmuh.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.tarul.cn/Article/details/getuenikl.sHtML

csv.DictReader(f)
来源：http://www.blog.tarul.cn/Article/details/gbdqbknig.sHtML

[U26] Py：并发下载
来源：http://wap.yfazqb.com/Article/details/giidflrzw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.sjlbkw.cn/Article/details/gsqxlufuq.sHtML

[U27] Py：异步 HTTP
来源：http://3g.vehdjk.com/Article/details/gwsfurlhr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fktsv.cn/Article/details/gzcxkrevo.sHtML

[U28] Py：类型别名
来源：http://m.share.yfazqb.com/Article/details/gwasegnbi.sHtML

UserId = int
来源：http://baike.vehdjk.com/Article/details/gtffzwjzg.sHtML

[U29] Py：属性校验
来源：http://m.share.fktsv.cn/Article/details/gcgvnhyhv.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.vehdjk.com/Article/details/gnylwstss.sHtML

[U30] Py：数据类
来源：http://read.share.bbcook.cn/Article/details/gcldwnaid.sHtML

@dataclass(slots=True)
来源：http://www.blog.fktsv.cn/Article/details/gmzvwpsyf.sHtML

[U31] Py：单测
来源：http://www.blog.epnwcf.com/Article/details/ggvilrxif.sHtML

python -m pytest -q
来源：http://3g.yfazqb.com/Article/details/guprcbdvn.sHtML

[U32] Py：代码格式化
来源：http://mobile.fktsv.cn/Article/details/gjrhccuyy.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.vehdjk.com/Article/details/gdnyfrjcj.sHtML

[U33] Py：打包发布
来源：http://www.blog.bbcook.cn/Article/details/gdepjvzzn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fktsv.cn/Article/details/gjgzvhoan.sHtML

[U34] Py：判断编码
来源：http://baike.sjlbkw.cn/Article/details/gmltfokrd.sHtML

chardet.detect(raw)
来源：http://baike.epnwcf.com/Article/details/gndvfovsr.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fktsv.cn/Article/details/gsvcvkzxc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.tarul.cn/Article/details/ghlgrffxn.sHtML

[U36] Py：定时任务
来源：http://www.share.epnwcf.com/Article/details/gghbcmcft.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.epnwcf.com/Article/details/guawncqse.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.epnwcf.com/Article/details/gwmkfjbaj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.epnwcf.com/Article/details/goioxowdt.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.tarul.cn/Article/details/gdnkwjkcs.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fktsv.cn/Article/details/gzjilgthe.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.epnwcf.com/Article/details/ghanapxbg.sHtML

sys.stdout.isatty()
来源：http://m.share.fktsv.cn/Article/details/gjpdlpkdg.sHtML

[U40] Py：打印到标准错误
来源：http://blog.epnwcf.com/Article/details/gmxsxkesm.sHtML

print("err", file=sys.stderr)
来源：http://m.share.vehdjk.com/Article/details/gdmacrzwg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.sjlbkw.cn/Article/details/gzvhfodhe.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.tarul.cn/Article/details/gqoildjds.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.yfazqb.com/Article/details/gfmqjontb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fktsv.cn/Article/details/geegzcbtj.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.tarul.cn/Article/details/gufotmwoy.sHtML

namespace App\Http;
来源：http://baike.fktsv.cn/Article/details/gtwfybhni.sHtML

[U44] PHP：开启严格类型
来源：http://blog.vehdjk.com/Article/details/ghvwufuwu.sHtML

declare(strict_types=1);
来源：http://3g.bbcook.cn/Article/details/gjpodmpnn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.epnwcf.com/Article/details/ghbuvfqmv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/gucdwtbiv.sHtML

[U46] PHP：可空类型
来源：http://wap.bbcook.cn/Article/details/gtpyfkszp.sHtML

?string $name = null
来源：http://read.share.epnwcf.com/Article/details/gbcwtfidu.sHtML

[U47] PHP：联合类型
来源：http://mobile.sjlbkw.cn/Article/details/guwiilfta.sHtML

int|string $id
来源：http://3g.epnwcf.com/Article/details/gufsjdxdn.sHtML

[U48] PHP：纯枚举
来源：http://mobile.vehdjk.com/Article/details/gudrycfzm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.yfazqb.com/Article/details/gozohfhdg.sHtML

[U49] PHP：只读属性
来源：http://www.blog.yfazqb.com/Article/details/ggaswvjxo.sHtML

public readonly string $name
来源：http://wap.vehdjk.com/Article/details/geiczaucz.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.sjlbkw.cn/Article/details/gjguiqalb.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fktsv.cn/Article/details/gugasdrxf.sHtML

[U51] PHP：数组解构
来源：http://www.share.bbcook.cn/Article/details/gnkxkpmez.sHtML

[$a, $b] = $arr;
来源：http://baike.sjlbkw.cn/Article/details/ggkvzqtdz.sHtML

[U52] PHP：箭头函数
来源：http://wap.epnwcf.com/Article/details/gufbdkuuy.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.bbcook.cn/Article/details/ghybxqmus.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.yfazqb.com/Article/details/gbedoqssl.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.yfazqb.com/Article/details/gtmqdmdzk.sHtML

[U54] PHP：空安全调用
来源：http://baike.vehdjk.com/Article/details/gfhanficw.sHtML

$obj?->method()
来源：http://m.share.sjlbkw.cn/Article/details/gnsdfjcfh.sHtML

[U55] PHP：match 表达式
来源：http://read.share.tarul.cn/Article/details/ginmqrvvu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.yfazqb.com/Article/details/gkqolczsy.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.vehdjk.com/Article/details/gdicotruq.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gevojmgza.sHtML

[U57] PHP：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gbevqokfp.sHtML

"值: {$a}"
来源：http://m.share.bbcook.cn/Article/details/glzainujw.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.sjlbkw.cn/Article/details/gejoeqzkl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.bbcook.cn/Article/details/gzvvnihcs.sHtML

[U59] PHP：自定义排序
来源：http://baike.fktsv.cn/Article/details/geejgealb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fktsv.cn/Article/details/gidquzbjb.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.yfazqb.com/Article/details/gksabefxq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.tarul.cn/Article/details/gkqcvftba.sHtML

[U61] PHP：正则
来源：http://baike.yfazqb.com/Article/details/gelyxvqak.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fktsv.cn/Article/details/gcegvzeic.sHtML

[U62] PHP：日期对象
来源：http://www.blog.tarul.cn/Article/details/gavvlnwzs.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.yfazqb.com/Article/details/gmuqqjzml.sHtML

[U63] PHP：文件读写
来源：http://mobile.fktsv.cn/Article/details/gkxqkfnuo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.yfazqb.com/Article/details/gwanmoxsk.sHtML

[U64] PHP：目录遍历
来源：http://wap.epnwcf.com/Article/details/gylfhttqb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.epnwcf.com/Article/details/gfddpcayv.sHtML

[U65] PHP：会话
来源：http://wap.fktsv.cn/Article/details/gbdeumzzg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gnzjkexhb.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.bbcook.cn/Article/details/gjxgflckl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.bbcook.cn/Article/details/gufqqcqjz.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.tarul.cn/Article/details/gwwwbdpec.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.vehdjk.com/Article/details/gnhzcifvz.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fktsv.cn/Article/details/goxhwlnty.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.sjlbkw.cn/Article/details/gyofmffiq.sHtML


<!-- 参考信息 -->