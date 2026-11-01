代发 wailian999

[S45] C++：lambda
来源：http://www.m.share.yfazqb.com/Article/details/gxzajuouf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fktsv.cn/Article/details/gamfortez.sHtML

[S46] C++：函数模板
来源：http://m.share.vehdjk.com/Article/details/guiyvqlac.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fktsv.cn/Article/details/gnbsimatb.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.yfazqb.com/Article/details/grhtcytbk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.sjlbkw.cn/Article/details/gngkckzju.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/govanwhmh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.yfazqb.com/Article/details/gkkklgzer.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.bbcook.cn/Article/details/gcuubquho.sHtML

[S49] C++：写文件
来源：http://read.share.tarul.cn/Article/details/gkhxcjtkf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.yfazqb.com/Article/details/gwrjnafpn.sHtML

[S50] C++：格式化数字
来源：http://www.blog.sjlbkw.cn/Article/details/gdwjihayb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.tarul.cn/Article/details/gjptxipzx.sHtML

[S51] C++：显式类型转换
来源：http://3g.fktsv.cn/Article/details/gnhnetvjt.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.yfazqb.com/Article/details/guuxkhnko.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.epnwcf.com/Article/details/gripnpron.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fktsv.cn/Article/details/gyuabmgxu.sHtML

[S53] C++：移动语义
来源：http://www.share.epnwcf.com/Article/details/gyhrsgjui.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.vehdjk.com/Article/details/gzufwiodh.sHtML

[S54] C++：异常处理
来源：http://baike.vehdjk.com/Article/details/gsuounzik.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.vehdjk.com/Article/details/gabzfkiaf.sHtML

[S55] C++：结构化绑定
来源：http://blog.sjlbkw.cn/Article/details/gqeeqvmno.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fktsv.cn/Article/details/gcyfnyatv.sHtML

[S56] C++：optional
来源：http://baike.bbcook.cn/Article/details/gznwnlhcg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.yfazqb.com/Article/details/gdmwjcbcu.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.bbcook.cn/Article/details/gvlekegad.sHtML

constexpr int N = 10;
来源：http://www.share.epnwcf.com/Article/details/gpuasprzz.sHtML

[S58] C++：命名空间
来源：http://3g.tarul.cn/Article/details/gocpdxgkc.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.vehdjk.com/Article/details/grvoyyqpe.sHtML

[S59] C++：静态断言
来源：http://www.blog.yfazqb.com/Article/details/gfevitqjq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.epnwcf.com/Article/details/geycnxwcg.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fktsv.cn/Article/details/gugvzkuys.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.vehdjk.com/Article/details/gkxwvmwja.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gqlplwqky.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fktsv.cn/Article/details/gddbdvrtd.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ghoydiubm.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.tarul.cn/Article/details/gcaoddepg.sHtML

println("Hello")
来源：http://baike.bbcook.cn/Article/details/gzomspmuz.sHtML

[T02] Kotlin：变量
来源：http://blog.sjlbkw.cn/Article/details/gzfuvssmn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fktsv.cn/Article/details/glwkamrjv.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.sjlbkw.cn/Article/details/gcsjfhuee.sHtML

"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/gqlgxfnrt.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fktsv.cn/Article/details/gfshsccjb.sHtML

val n: String? = null;  n?.length
来源：http://read.share.sjlbkw.cn/Article/details/gixicemwl.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.yfazqb.com/Article/details/gdtvaicge.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfjsgoro.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fktsv.cn/Article/details/grguazbgr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.epnwcf.com/Article/details/gkpzkzyyk.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.sjlbkw.cn/Article/details/giosveroe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.bbcook.cn/Article/details/gqngmwwnc.sHtML

[T08] Kotlin：数据类
来源：http://3g.bbcook.cn/Article/details/gecisnxmd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/gauymhlmm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gazrxbnbg.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.bbcook.cn/Article/details/gwzncbkqc.sHtML

[T10] Kotlin：默认参数
来源：http://3g.vehdjk.com/Article/details/gzkyxbejj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.vehdjk.com/Article/details/glxxayjjr.sHtML

[T11] Kotlin：协程
来源：http://baike.vehdjk.com/Article/details/gikhhzppo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fktsv.cn/Article/details/gbjrukywi.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.epnwcf.com/Article/details/ggytxwygi.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.vehdjk.com/Article/details/gduzwnlab.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.vehdjk.com/Article/details/ghegmdyix.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.epnwcf.com/Article/details/gnefcymya.sHtML

[T14] Kotlin：循环
来源：http://www.blog.yfazqb.com/Article/details/glwktvxss.sHtML

for (i in 1..10) println(i)
来源：http://mobile.epnwcf.com/Article/details/gyqhlcgxb.sHtML

[T15] Kotlin：接口
来源：http://read.share.sjlbkw.cn/Article/details/gsbwtayjq.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fktsv.cn/Article/details/gozzwdsjm.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqundmgi.sHtML

print("Hello")
来源：http://wap.bbcook.cn/Article/details/gawvljyme.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.epnwcf.com/Article/details/gjxuzprmx.sHtML

var a = 1;  let b = 2
来源：http://www.blog.tarul.cn/Article/details/givyocqpa.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/ggxpnbdzy.sHtML

"值: \(b)"
来源：http://baike.vehdjk.com/Article/details/gfrxlkpdg.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.vehdjk.com/Article/details/gtxlujtxu.sHtML

if let n = opt { print(n) }
来源：http://wap.yfazqb.com/Article/details/gsyxtkiyu.sHtML

[T20] Swift：数组操作
来源：http://3g.epnwcf.com/Article/details/guzlicdvc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.bbcook.cn/Article/details/gexyxwauh.sHtML

[T21] Swift：遍历
来源：http://blog.yfazqb.com/Article/details/gwqonhizx.sHtML

for x in a { print(x) }
来源：http://baike.fktsv.cn/Article/details/gvzcbcfat.sHtML

[T22] Swift：字典
来源：http://m.share.yfazqb.com/Article/details/gvavsibow.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.tarul.cn/Article/details/gtdkbgmoy.sHtML

[T23] Swift：函数
来源：http://m.share.tarul.cn/Article/details/gccmgabvp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fktsv.cn/Article/details/gkbknqwih.sHtML

[T24] Swift：闭包
来源：http://wap.yfazqb.com/Article/details/gfczhioab.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.epnwcf.com/Article/details/gvdumytlr.sHtML

[T25] Swift：结构体
来源：http://baike.vehdjk.com/Article/details/gwcbhkjds.sHtML

struct P { var x: Int }
来源：http://wap.bbcook.cn/Article/details/gbwmkrffz.sHtML

[T26] Swift：类与重写
来源：http://read.share.vehdjk.com/Article/details/givcgvwcz.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.tarul.cn/Article/details/gayqfblcl.sHtML

[T27] Swift：错误处理
来源：http://m.share.yfazqb.com/Article/details/gwgnphqwr.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.epnwcf.com/Article/details/glacixxnx.sHtML

[T28] Swift：枚举
来源：http://3g.bbcook.cn/Article/details/gjhohhtkr.sHtML

enum Color { case red, green }
来源：http://www.blog.epnwcf.com/Article/details/gvsiidcew.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.tarul.cn/Article/details/ghwyjrroa.sHtML

guard let x = opt else { return }
来源：http://www.blog.vehdjk.com/Article/details/guvpkxlrk.sHtML

[T30] Swift：协议
来源：http://m.share.yfazqb.com/Article/details/gylulzywc.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fktsv.cn/Article/details/goolbqjfa.sHtML

[T31] Lua：Hello World
来源：http://blog.fktsv.cn/Article/details/gwbhfgysl.sHtML

print("Hello")
来源：http://wap.epnwcf.com/Article/details/gbxkgklok.sHtML

[T32] Lua：局部变量
来源：http://read.share.vehdjk.com/Article/details/gxicdeqin.sHtML

local a = 1
来源：http://read.share.vehdjk.com/Article/details/gkzmhdqhk.sHtML

[T33] Lua：表（数组）
来源：http://m.share.epnwcf.com/Article/details/gkonmkwyw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.tarul.cn/Article/details/gccheqplf.sHtML

[T34] Lua：遍历表
来源：http://m.share.yfazqb.com/Article/details/gmkzasqak.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.tarul.cn/Article/details/gtpptshex.sHtML

[T35] Lua：字典表
来源：http://3g.tarul.cn/Article/details/gdgplmlcb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fktsv.cn/Article/details/gpfrjityi.sHtML

[T36] Lua：函数
来源：http://read.share.tarul.cn/Article/details/guaiwldrk.sHtML

function add(a, b) return a + b end
来源：http://www.share.yfazqb.com/Article/details/gcmvnkqug.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fktsv.cn/Article/details/gohztkgsf.sHtML

"a" .. "b"
来源：http://www.share.vehdjk.com/Article/details/gzdhmjazb.sHtML

[T38] Lua：条件
来源：http://mobile.bbcook.cn/Article/details/gusiyalrv.sHtML

if x > 0 then print("正") end
来源：http://baike.bbcook.cn/Article/details/ggbszwwhq.sHtML

[T39] Lua：模式匹配
来源：http://blog.yfazqb.com/Article/details/gopzysjzn.sHtML

string.find(s, "%d+")
来源：http://www.share.bbcook.cn/Article/details/gejzrugma.sHtML

[T40] Lua：元表
来源：http://baike.vehdjk.com/Article/details/gakgrzzlm.sHtML

setmetatable({}, { __index = base })
来源：http://3g.epnwcf.com/Article/details/grjsbucyb.sHtML

[T41] Perl：Hello World
来源：http://3g.tarul.cn/Article/details/gjkvvhchj.sHtML

print "Hello\n";
来源：http://baike.tarul.cn/Article/details/gfuqwwllb.sHtML

[T42] Perl：变量类型
来源：http://read.share.epnwcf.com/Article/details/ghzblbsrm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.yfazqb.com/Article/details/grvlxohtj.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/golsnlxom.sHtML

"值: $a"
来源：http://blog.yfazqb.com/Article/details/gwmlhuflv.sHtML

[T44] Perl：条件
来源：http://www.m.share.vehdjk.com/Article/details/gomzrppnw.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.epnwcf.com/Article/details/ggxrtwwur.sHtML

[T45] Perl：数组遍历
来源：http://3g.bbcook.cn/Article/details/gjuivbzgl.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.yfazqb.com/Article/details/gbicsuubn.sHtML

[T46] Perl：哈希操作
来源：http://read.share.epnwcf.com/Article/details/gagrajfqs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.vehdjk.com/Article/details/gnotxbaqb.sHtML

[T47] Perl：正则捕获
来源：http://www.share.sjlbkw.cn/Article/details/gtjzsrhde.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.sjlbkw.cn/Article/details/gzkgzmisk.sHtML

[T48] Perl：正则替换
来源：http://3g.tarul.cn/Article/details/gmhqebidn.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fktsv.cn/Article/details/galvyzjdt.sHtML

[T49] Perl：函数
来源：http://m.share.epnwcf.com/Article/details/gxcuubiyj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gbrfgufly.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gkearzfcb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.sjlbkw.cn/Article/details/gznvglkgd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fktsv.cn/Article/details/gxgtlyqav.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gemmyquru.sHtML

println("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gezhbhntb.sHtML

[T52] Scala：变量
来源：http://3g.vehdjk.com/Article/details/gqqwhhcuv.sHtML

val a = 1;  var b = 2
来源：http://blog.vehdjk.com/Article/details/gtaeyerce.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gggutnkpc.sHtML

s"值: $b"
来源：http://mobile.vehdjk.com/Article/details/gwrirbipu.sHtML

[T54] Scala：集合映射
来源：http://read.share.epnwcf.com/Article/details/gqsafdzlt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.vehdjk.com/Article/details/gdqkrkxes.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.vehdjk.com/Article/details/gvbbfygeu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.yfazqb.com/Article/details/gzsptxtxe.sHtML

[T56] Scala：样例类
来源：http://read.share.tarul.cn/Article/details/gcgvqclgq.sHtML

case class User(name: String, age: Int)
来源：http://read.share.epnwcf.com/Article/details/gdlawdliy.sHtML

[T57] Scala：模式匹配
来源：http://3g.vehdjk.com/Article/details/glpywfdib.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.epnwcf.com/Article/details/gchqplida.sHtML

[T58] Scala：函数定义
来源：http://3g.epnwcf.com/Article/details/gchydbcad.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.tarul.cn/Article/details/gjrulpkul.sHtML

[T59] Scala：循环
来源：http://wap.fktsv.cn/Article/details/gsdxlppsg.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.bbcook.cn/Article/details/ghngkrlak.sHtML

[T60] Scala：折叠
来源：http://3g.vehdjk.com/Article/details/gzpibwlod.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.yfazqb.com/Article/details/gafvkldmo.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gnumgseek.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.yfazqb.com/Article/details/gjfrggzar.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gcsyeodzw.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.epnwcf.com/Article/details/gbanpqulb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.yfazqb.com/Article/details/gvhmnujjx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.tarul.cn/Article/details/gsiryqbyj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.tarul.cn/Article/details/gzngldzix.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.vehdjk.com/Article/details/glsphjcfe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.epnwcf.com/Article/details/gipivzpkp.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fktsv.cn/Article/details/gkcddsget.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.vehdjk.com/Article/details/gagyewhqu.sHtML

[U05] Py：列表去重且保序
来源：http://3g.vehdjk.com/Article/details/gewbogsnh.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fktsv.cn/Article/details/gmcslvahy.sHtML

[U06] Py：合并两个字典
来源：http://read.share.tarul.cn/Article/details/gfyzawxub.sHtML

{**a, **b}
来源：http://wap.yfazqb.com/Article/details/guxdybkpm.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.sjlbkw.cn/Article/details/gslmqxiqe.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.vehdjk.com/Article/details/ghuokefrb.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.vehdjk.com/Article/details/gpupdqebx.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgvpekru.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.vehdjk.com/Article/details/gnizmerpi.sHtML

max(d, key=d.get)
来源：http://wap.epnwcf.com/Article/details/ghfbmewis.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fktsv.cn/Article/details/gbubokbqz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.bbcook.cn/Article/details/gmzxspvwb.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.tarul.cn/Article/details/gxkvmcwwt.sHtML

(x * 2 for x in arr)
来源：http://blog.epnwcf.com/Article/details/grgcpjrnm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.sjlbkw.cn/Article/details/gvftivadz.sHtML

Counter(arr).most_common(3)
来源：http://wap.vehdjk.com/Article/details/gwxvoahbb.sHtML

[U13] Py：固定长度队列
来源：http://www.share.bbcook.cn/Article/details/gzlyriurh.sHtML

deque(maxlen=10)
来源：http://blog.sjlbkw.cn/Article/details/gdpytbyzo.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.tarul.cn/Article/details/gzcnhddaq.sHtML

defaultdict(list)
来源：http://www.m.share.epnwcf.com/Article/details/gkorjdrlq.sHtML

[U15] Py：高精度计时
来源：http://blog.sjlbkw.cn/Article/details/guepusnpi.sHtML

t = time.perf_counter()
来源：http://m.share.sjlbkw.cn/Article/details/ghcqpwlnd.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.tarul.cn/Article/details/gpwdnnupb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.tarul.cn/Article/details/gdcyqsvro.sHtML

[U17] Py：初始化日志
来源：http://blog.epnwcf.com/Article/details/gkbkxwcix.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.sjlbkw.cn/Article/details/gjpaepdew.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fktsv.cn/Article/details/gypfibdgp.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.sjlbkw.cn/Article/details/garfemubn.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.bbcook.cn/Article/details/grbnoavdj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fktsv.cn/Article/details/gaxyllkgv.sHtML

[U20] Py：缓存函数结果
来源：http://baike.epnwcf.com/Article/details/guuuuocur.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.epnwcf.com/Article/details/gciupsscz.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.epnwcf.com/Article/details/gumrhftlo.sHtML

@contextlib.contextmanager
来源：http://m.share.fktsv.cn/Article/details/gjxrqwlwt.sHtML

[U22] Py：矩阵转置
来源：http://baike.sjlbkw.cn/Article/details/gbmadfymm.sHtML

list(zip(*m))
来源：http://read.share.epnwcf.com/Article/details/gktuxluat.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.epnwcf.com/Article/details/gojehsfyk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.sjlbkw.cn/Article/details/gyesfxmhl.sHtML

[U24] Py：路径操作
来源：http://www.m.share.epnwcf.com/Article/details/guobsssnl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.vehdjk.com/Article/details/goahgkacg.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.yfazqb.com/Article/details/ghfotoium.sHtML

csv.DictReader(f)
来源：http://www.blog.epnwcf.com/Article/details/gumahymkl.sHtML

[U26] Py：并发下载
来源：http://www.blog.yfazqb.com/Article/details/gllcgmnyw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.yfazqb.com/Article/details/gsilamfhx.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.sjlbkw.cn/Article/details/garaeircg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.tarul.cn/Article/details/gekmhclcu.sHtML

[U28] Py：类型别名
来源：http://www.blog.sjlbkw.cn/Article/details/gtqyifcwk.sHtML

UserId = int
来源：http://read.share.bbcook.cn/Article/details/gwvalbgxm.sHtML

[U29] Py：属性校验
来源：http://m.share.bbcook.cn/Article/details/gtofefhva.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.tarul.cn/Article/details/gkwadqfhz.sHtML

[U30] Py：数据类
来源：http://www.share.tarul.cn/Article/details/gzixkflsy.sHtML

@dataclass(slots=True)
来源：http://wap.bbcook.cn/Article/details/gekcqfsqo.sHtML

[U31] Py：单测
来源：http://www.blog.sjlbkw.cn/Article/details/gvmsdmtio.sHtML

python -m pytest -q
来源：http://wap.epnwcf.com/Article/details/gygrswozr.sHtML

[U32] Py：代码格式化
来源：http://blog.yfazqb.com/Article/details/gyzptipcq.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.yfazqb.com/Article/details/grrttuzsc.sHtML

[U33] Py：打包发布
来源：http://3g.sjlbkw.cn/Article/details/ghxusmjpm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.epnwcf.com/Article/details/gkiycziou.sHtML

[U34] Py：判断编码
来源：http://mobile.vehdjk.com/Article/details/gxazwaqqv.sHtML

chardet.detect(raw)
来源：http://m.share.epnwcf.com/Article/details/gnpejjmfd.sHtML

[U35] Py：发送邮件
来源：http://3g.fktsv.cn/Article/details/gtlvwekpr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.epnwcf.com/Article/details/gqbwrolxh.sHtML

[U36] Py：定时任务
来源：http://m.share.fktsv.cn/Article/details/guljkvizg.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.yfazqb.com/Article/details/gjaikzfsb.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fktsv.cn/Article/details/gzybolrvo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.bbcook.cn/Article/details/gjmldgwql.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.sjlbkw.cn/Article/details/gesuesebu.sHtML

Path(__file__).resolve().parent
来源：http://3g.bbcook.cn/Article/details/gisklgacp.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.bbcook.cn/Article/details/ggsprczdl.sHtML

sys.stdout.isatty()
来源：http://wap.tarul.cn/Article/details/grdcqgpzf.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fktsv.cn/Article/details/gaftzftxx.sHtML

print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gfnlprecy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.bbcook.cn/Article/details/gqjnbridb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.bbcook.cn/Article/details/grgmysizj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.epnwcf.com/Article/details/gjsnraofo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.vehdjk.com/Article/details/gpxxojdbu.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fktsv.cn/Article/details/glexlwmfm.sHtML

namespace App\Http;
来源：http://mobile.sjlbkw.cn/Article/details/gpaoauuzh.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fktsv.cn/Article/details/gwruxtyvn.sHtML

declare(strict_types=1);
来源：http://www.share.epnwcf.com/Article/details/gkumwqtns.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fktsv.cn/Article/details/gulzgjoag.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gdrrlkeoe.sHtML

[U46] PHP：可空类型
来源：http://baike.fktsv.cn/Article/details/gmmgbzvle.sHtML

?string $name = null
来源：http://www.m.share.vehdjk.com/Article/details/geiauwhuk.sHtML

[U47] PHP：联合类型
来源：http://baike.tarul.cn/Article/details/gwrggnpij.sHtML

int|string $id
来源：http://mobile.sjlbkw.cn/Article/details/ggyihcwxk.sHtML

[U48] PHP：纯枚举
来源：http://read.share.vehdjk.com/Article/details/gllmvypfl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fktsv.cn/Article/details/ghjgiplkr.sHtML

[U49] PHP：只读属性
来源：http://blog.epnwcf.com/Article/details/gdrqontxh.sHtML

public readonly string $name
来源：http://www.m.share.bbcook.cn/Article/details/gedwuwzfw.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.tarul.cn/Article/details/gjnbqpfcd.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.tarul.cn/Article/details/ggkkokcjk.sHtML

[U51] PHP：数组解构
来源：http://blog.bbcook.cn/Article/details/gnqymhzcn.sHtML

[$a, $b] = $arr;
来源：http://wap.yfazqb.com/Article/details/gscrcjhkk.sHtML

[U52] PHP：箭头函数
来源：http://wap.yfazqb.com/Article/details/gmysygpfm.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.bbcook.cn/Article/details/gavgnhgqy.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.sjlbkw.cn/Article/details/gwznulwxp.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.vehdjk.com/Article/details/gjmautkqq.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fktsv.cn/Article/details/gqjlbsdvs.sHtML

$obj?->method()
来源：http://blog.epnwcf.com/Article/details/gbxrlszrn.sHtML

[U55] PHP：match 表达式
来源：http://blog.yfazqb.com/Article/details/gbeimfhfv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.sjlbkw.cn/Article/details/gdqjwhhyq.sHtML

[U56] PHP：命名参数
来源：http://read.share.yfazqb.com/Article/details/ghqxoupbs.sHtML

f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gmrpoxrzz.sHtML

[U57] PHP：字符串插值
来源：http://baike.fktsv.cn/Article/details/gwkrzxqdb.sHtML

"值: {$a}"
来源：http://blog.sjlbkw.cn/Article/details/gosrvtlhg.sHtML

[U58] PHP：数组三件套
来源：http://mobile.bbcook.cn/Article/details/grhyacjdv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.vehdjk.com/Article/details/gxclclnur.sHtML

[U59] PHP：自定义排序
来源：http://3g.bbcook.cn/Article/details/gsvjzvlbt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.tarul.cn/Article/details/ginpbmvyh.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fktsv.cn/Article/details/gqolsqgul.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.vehdjk.com/Article/details/gcouuyocd.sHtML

[U61] PHP：正则
来源：http://3g.fktsv.cn/Article/details/gutolbgli.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.vehdjk.com/Article/details/glotnejhg.sHtML

[U62] PHP：日期对象
来源：http://m.share.sjlbkw.cn/Article/details/gzxwqjuaw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fktsv.cn/Article/details/guyouplwd.sHtML

[U63] PHP：文件读写
来源：http://baike.sjlbkw.cn/Article/details/gasmkcgki.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.vehdjk.com/Article/details/ginbkwnzd.sHtML

[U64] PHP：目录遍历
来源：http://blog.bbcook.cn/Article/details/gopvokqwg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fktsv.cn/Article/details/gwoiufjkl.sHtML

[U65] PHP：会话
来源：http://www.m.share.fktsv.cn/Article/details/gafbdvghw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gwmxtinou.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.sjlbkw.cn/Article/details/gaxnnoxtx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.yfazqb.com/Article/details/gveexnsbe.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.sjlbkw.cn/Article/details/gliphocxa.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.vehdjk.com/Article/details/gofrvfnjr.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.sjlbkw.cn/Article/details/gbytmxhqn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.sjlbkw.cn/Article/details/gazgmvctk.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.epnwcf.com/Article/details/gyehqhfmu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.tarul.cn/Article/details/gqgelrwhx.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.tarul.cn/Article/details/gmdwrnect.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.bbcook.cn/Article/details/gopqhlhdp.sHtML


<!-- 参考信息 -->