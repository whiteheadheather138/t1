代发 wailian999

[S45] C++：lambda
来源：http://3g.fktsv.cn/Article/details/gdifqnzxp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.bbcook.cn/Article/details/ghqgzwcud.sHtML

[S46] C++：函数模板
来源：http://wap.tarul.cn/Article/details/gltphuile.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.yfazqb.com/Article/details/ggsxwnndt.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.bbcook.cn/Article/details/gpvqrfnko.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fktsv.cn/Article/details/gzncksoii.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gkhehvspl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.yfazqb.com/Article/details/gjdbrgxpd.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.yfazqb.com/Article/details/gdlzxruuz.sHtML

[S49] C++：写文件
来源：http://blog.yfazqb.com/Article/details/gopkryjns.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.yfazqb.com/Article/details/gxlefdleg.sHtML

[S50] C++：格式化数字
来源：http://www.share.yfazqb.com/Article/details/gpwleqxuh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gefzzplxl.sHtML

[S51] C++：显式类型转换
来源：http://m.share.vehdjk.com/Article/details/gdhcugblg.sHtML

static_cast<double>(a) / b
来源：http://m.share.sjlbkw.cn/Article/details/gktgzkvtb.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.sjlbkw.cn/Article/details/gradwfwlo.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.yfazqb.com/Article/details/gndfclbgp.sHtML

[S53] C++：移动语义
来源：http://mobile.vehdjk.com/Article/details/gunbqeggh.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fktsv.cn/Article/details/gzpadvldi.sHtML

[S54] C++：异常处理
来源：http://mobile.vehdjk.com/Article/details/gzpyhnuuq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.yfazqb.com/Article/details/grefipbqt.sHtML

[S55] C++：结构化绑定
来源：http://www.share.epnwcf.com/Article/details/gtjmxisca.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.vehdjk.com/Article/details/gzwxyxjgp.sHtML

[S56] C++：optional
来源：http://m.share.sjlbkw.cn/Article/details/gddcfrebu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.bbcook.cn/Article/details/gjdjudvko.sHtML

[S57] C++：编译期常量
来源：http://m.share.yfazqb.com/Article/details/ggjoimvfi.sHtML

constexpr int N = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gitddtiog.sHtML

[S58] C++：命名空间
来源：http://www.blog.tarul.cn/Article/details/gxzvvlzjf.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.vehdjk.com/Article/details/gpdmlwzie.sHtML

[S59] C++：静态断言
来源：http://wap.tarul.cn/Article/details/gwidufxco.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.vehdjk.com/Article/details/gygcgiudo.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.sjlbkw.cn/Article/details/gkizuzdab.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.yfazqb.com/Article/details/gkiquugst.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gnndxliam.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.tarul.cn/Article/details/gfngpgzwq.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlsmrmqa.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.epnwcf.com/Article/details/ghvfefdxb.sHtML

println("Hello")
来源：http://baike.fktsv.cn/Article/details/gjxzoipat.sHtML

[T02] Kotlin：变量
来源：http://blog.fktsv.cn/Article/details/gydurbkgw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.yfazqb.com/Article/details/gewcwqmqr.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.tarul.cn/Article/details/gggvhypyb.sHtML

"值: $b"
来源：http://m.share.sjlbkw.cn/Article/details/gjegetutp.sHtML

[T04] Kotlin：空安全
来源：http://read.share.vehdjk.com/Article/details/guvvdfeff.sHtML

val n: String? = null;  n?.length
来源：http://blog.tarul.cn/Article/details/gxtwerfhm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gktuxrqre.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fktsv.cn/Article/details/gihlexpnm.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.sjlbkw.cn/Article/details/gbgcxzknc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.bbcook.cn/Article/details/ggploaecu.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.bbcook.cn/Article/details/gngxrlgsk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.yfazqb.com/Article/details/gbxnfjvhs.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fktsv.cn/Article/details/gbsbcdpqu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.sjlbkw.cn/Article/details/gynqvldrj.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.yfazqb.com/Article/details/gjxtuoxpq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.yfazqb.com/Article/details/goleinizl.sHtML

[T10] Kotlin：默认参数
来源：http://blog.epnwcf.com/Article/details/genmtpfiz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.sjlbkw.cn/Article/details/gklnzliwp.sHtML

[T11] Kotlin：协程
来源：http://mobile.epnwcf.com/Article/details/gtfzrxgfv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fktsv.cn/Article/details/grbsromud.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fktsv.cn/Article/details/gghbwimro.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gofjpnpvy.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.epnwcf.com/Article/details/glpuzwaer.sHtML

val m = mapOf("a" to 1)
来源：http://blog.tarul.cn/Article/details/gsuhwmuqp.sHtML

[T14] Kotlin：循环
来源：http://m.share.bbcook.cn/Article/details/geuqyjzqd.sHtML

for (i in 1..10) println(i)
来源：http://3g.fktsv.cn/Article/details/gabmvvmbf.sHtML

[T15] Kotlin：接口
来源：http://read.share.vehdjk.com/Article/details/gwesbpdbx.sHtML

interface Shape { fun area(): Double }
来源：http://blog.epnwcf.com/Article/details/gpodmsdpf.sHtML

[T16] Swift：Hello World
来源：http://m.share.vehdjk.com/Article/details/gqhuhuccf.sHtML

print("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/gxqnqghzp.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.epnwcf.com/Article/details/gzienbhzj.sHtML

var a = 1;  let b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gkbwcuvns.sHtML

[T18] Swift：字符串插值
来源：http://blog.vehdjk.com/Article/details/goodljmlm.sHtML

"值: \(b)"
来源：http://www.blog.bbcook.cn/Article/details/gxtwwvbbs.sHtML

[T19] Swift：可选绑定
来源：http://3g.epnwcf.com/Article/details/gxalykjxg.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.vehdjk.com/Article/details/gneaxllye.sHtML

[T20] Swift：数组操作
来源：http://mobile.sjlbkw.cn/Article/details/gdxsaqxui.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.tarul.cn/Article/details/glsiznvzc.sHtML

[T21] Swift：遍历
来源：http://m.share.bbcook.cn/Article/details/gymzyerdl.sHtML

for x in a { print(x) }
来源：http://www.m.share.yfazqb.com/Article/details/gwnjkrtsv.sHtML

[T22] Swift：字典
来源：http://mobile.fktsv.cn/Article/details/gqcvpgtmk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.sjlbkw.cn/Article/details/gvsqqaxrw.sHtML

[T23] Swift：函数
来源：http://read.share.tarul.cn/Article/details/glvoognif.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.tarul.cn/Article/details/gjhmytems.sHtML

[T24] Swift：闭包
来源：http://blog.bbcook.cn/Article/details/gwohallfl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.bbcook.cn/Article/details/gpkbrrwqh.sHtML

[T25] Swift：结构体
来源：http://baike.yfazqb.com/Article/details/ggmgxhgfn.sHtML

struct P { var x: Int }
来源：http://baike.sjlbkw.cn/Article/details/ghjuoxjab.sHtML

[T26] Swift：类与重写
来源：http://3g.tarul.cn/Article/details/gbkskwxxe.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.vehdjk.com/Article/details/gxigvakuu.sHtML

[T27] Swift：错误处理
来源：http://wap.bbcook.cn/Article/details/gefjgpzhw.sHtML

do { try f() } catch { print(error) }
来源：http://wap.tarul.cn/Article/details/gkqkzjxam.sHtML

[T28] Swift：枚举
来源：http://mobile.yfazqb.com/Article/details/gxjaktrmk.sHtML

enum Color { case red, green }
来源：http://read.share.epnwcf.com/Article/details/gwqmpurul.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.bbcook.cn/Article/details/gytpahpyt.sHtML

guard let x = opt else { return }
来源：http://www.blog.vehdjk.com/Article/details/gpcudvcfa.sHtML

[T30] Swift：协议
来源：http://www.blog.tarul.cn/Article/details/gkoegrcqs.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fktsv.cn/Article/details/gzrygmego.sHtML

[T31] Lua：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gttxovhkf.sHtML

print("Hello")
来源：http://blog.tarul.cn/Article/details/gcwoifiec.sHtML

[T32] Lua：局部变量
来源：http://baike.vehdjk.com/Article/details/gaumusxpf.sHtML

local a = 1
来源：http://wap.yfazqb.com/Article/details/gpunfpxyk.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.yfazqb.com/Article/details/gjpmijphz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.epnwcf.com/Article/details/gjnhkiklg.sHtML

[T34] Lua：遍历表
来源：http://read.share.fktsv.cn/Article/details/gtiooskgv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.sjlbkw.cn/Article/details/gltoveszy.sHtML

[T35] Lua：字典表
来源：http://wap.sjlbkw.cn/Article/details/gtsigylne.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.vehdjk.com/Article/details/gxsbsxauq.sHtML

[T36] Lua：函数
来源：http://read.share.yfazqb.com/Article/details/gwuzwjnam.sHtML

function add(a, b) return a + b end
来源：http://www.share.sjlbkw.cn/Article/details/guzegjinb.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fktsv.cn/Article/details/gxxchsixo.sHtML

"a" .. "b"
来源：http://blog.epnwcf.com/Article/details/gjzxcaywq.sHtML

[T38] Lua：条件
来源：http://3g.tarul.cn/Article/details/gywswateu.sHtML

if x > 0 then print("正") end
来源：http://blog.vehdjk.com/Article/details/gqpqqyoxf.sHtML

[T39] Lua：模式匹配
来源：http://www.share.tarul.cn/Article/details/gkkfmokul.sHtML

string.find(s, "%d+")
来源：http://www.share.vehdjk.com/Article/details/gthwwtoix.sHtML

[T40] Lua：元表
来源：http://3g.yfazqb.com/Article/details/gcdanhudt.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fktsv.cn/Article/details/gledepyty.sHtML

[T41] Perl：Hello World
来源：http://wap.epnwcf.com/Article/details/ghgrmgzzz.sHtML

print "Hello\n";
来源：http://www.share.vehdjk.com/Article/details/gjxrtmohu.sHtML

[T42] Perl：变量类型
来源：http://www.share.tarul.cn/Article/details/gydlrvkut.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.tarul.cn/Article/details/gmknlomto.sHtML

[T43] Perl：字符串插值
来源：http://baike.yfazqb.com/Article/details/ggtmbkidf.sHtML

"值: $a"
来源：http://blog.tarul.cn/Article/details/gzfltyuwf.sHtML

[T44] Perl：条件
来源：http://wap.sjlbkw.cn/Article/details/gbankbjdu.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.tarul.cn/Article/details/gyvwvbukf.sHtML

[T45] Perl：数组遍历
来源：http://blog.bbcook.cn/Article/details/geszuuwuf.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.vehdjk.com/Article/details/ganyvzxev.sHtML

[T46] Perl：哈希操作
来源：http://mobile.yfazqb.com/Article/details/gsdnxirip.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.epnwcf.com/Article/details/gdxtmrkeu.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.bbcook.cn/Article/details/gpauiuuax.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fktsv.cn/Article/details/gofgnhspq.sHtML

[T48] Perl：正则替换
来源：http://www.share.sjlbkw.cn/Article/details/gmhdhnrbh.sHtML

$s =~ s/old/new/g;
来源：http://blog.fktsv.cn/Article/details/gsetefvfb.sHtML

[T49] Perl：函数
来源：http://www.blog.bbcook.cn/Article/details/ggjfxntcd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gdugkvzlx.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gbfxzkspb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.vehdjk.com/Article/details/gwxotwzmo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.vehdjk.com/Article/details/gmitobanc.sHtML

[T51] Scala：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gfiughtqa.sHtML

println("Hello")
来源：http://read.share.vehdjk.com/Article/details/gxcxwzoei.sHtML

[T52] Scala：变量
来源：http://baike.tarul.cn/Article/details/gbzomxerb.sHtML

val a = 1;  var b = 2
来源：http://mobile.bbcook.cn/Article/details/glrboidak.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gaieqowkh.sHtML

s"值: $b"
来源：http://blog.vehdjk.com/Article/details/gexbjsasu.sHtML

[T54] Scala：集合映射
来源：http://baike.bbcook.cn/Article/details/gbwxqoqwp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.tarul.cn/Article/details/gkhdomdrp.sHtML

[T55] Scala：集合过滤
来源：http://read.share.vehdjk.com/Article/details/gyxzbxtll.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.tarul.cn/Article/details/ggcaiabjn.sHtML

[T56] Scala：样例类
来源：http://mobile.tarul.cn/Article/details/ghtbctayd.sHtML

case class User(name: String, age: Int)
来源：http://read.share.yfazqb.com/Article/details/gyrvhgwbl.sHtML

[T57] Scala：模式匹配
来源：http://mobile.sjlbkw.cn/Article/details/gowwoieyh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.sjlbkw.cn/Article/details/gdpltwhhn.sHtML

[T58] Scala：函数定义
来源：http://blog.sjlbkw.cn/Article/details/grjmdficx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fktsv.cn/Article/details/gmeajcxgy.sHtML

[T59] Scala：循环
来源：http://wap.epnwcf.com/Article/details/gvdkjaojm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gszvwjuah.sHtML

[T60] Scala：折叠
来源：http://baike.fktsv.cn/Article/details/gykbbznfs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.vehdjk.com/Article/details/ghbzixtrj.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gkzbfkulu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.epnwcf.com/Article/details/giwxrkpnm.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gdjymgpxc.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.epnwcf.com/Article/details/glrdizxll.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fktsv.cn/Article/details/gtrjocxsw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.vehdjk.com/Article/details/gkidwpcxi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.bbcook.cn/Article/details/gqhnwzowm.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.vehdjk.com/Article/details/gbzljagkr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.sjlbkw.cn/Article/details/gnzatrosi.sHtML

[U04] Py：变量调试打印
来源：http://baike.sjlbkw.cn/Article/details/gdsnheogq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.bbcook.cn/Article/details/gkrmysnzq.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.epnwcf.com/Article/details/gjiwgnnik.sHtML

list(dict.fromkeys(arr))
来源：http://blog.epnwcf.com/Article/details/gyuumkeot.sHtML

[U06] Py：合并两个字典
来源：http://baike.vehdjk.com/Article/details/gvntcnxho.sHtML

{**a, **b}
来源：http://blog.yfazqb.com/Article/details/grqoepsed.sHtML

[U07] Py：反转字典键值
来源：http://read.share.sjlbkw.cn/Article/details/gpjkvsvrk.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.yfazqb.com/Article/details/ggtbpinpj.sHtML

[U08] Py：展平二维列表
来源：http://read.share.sjlbkw.cn/Article/details/gngeqgqvc.sHtML

[y for x in nested for y in x]
来源：http://wap.yfazqb.com/Article/details/gogsukpfu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.sjlbkw.cn/Article/details/glkkdcqss.sHtML

max(d, key=d.get)
来源：http://mobile.sjlbkw.cn/Article/details/gbysgqmri.sHtML

[U10] Py：按值排序字典
来源：http://mobile.sjlbkw.cn/Article/details/grfibxtqw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fktsv.cn/Article/details/gxxjfmkwg.sHtML

[U11] Py：生成器表达式
来源：http://wap.epnwcf.com/Article/details/gizangdkf.sHtML

(x * 2 for x in arr)
来源：http://read.share.sjlbkw.cn/Article/details/gmxcnmbzc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.sjlbkw.cn/Article/details/gjhyghhva.sHtML

Counter(arr).most_common(3)
来源：http://mobile.sjlbkw.cn/Article/details/gsdvjmqxk.sHtML

[U13] Py：固定长度队列
来源：http://blog.sjlbkw.cn/Article/details/gfzmquvgg.sHtML

deque(maxlen=10)
来源：http://mobile.vehdjk.com/Article/details/gkmqlvukr.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.yfazqb.com/Article/details/gorxebxgx.sHtML

defaultdict(list)
来源：http://read.share.epnwcf.com/Article/details/gtvscjxdh.sHtML

[U15] Py：高精度计时
来源：http://3g.yfazqb.com/Article/details/gjoyiktxz.sHtML

t = time.perf_counter()
来源：http://www.m.share.bbcook.cn/Article/details/gkkrepnzf.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.epnwcf.com/Article/details/gaxptnxgy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.sjlbkw.cn/Article/details/gmuyhrqbq.sHtML

[U17] Py：初始化日志
来源：http://read.share.tarul.cn/Article/details/gvgioodyj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.bbcook.cn/Article/details/glspiffhy.sHtML

[U18] Py：预编译正则
来源：http://m.share.tarul.cn/Article/details/gqrvaxxrw.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.sjlbkw.cn/Article/details/gjdmxruyp.sHtML

[U19] Py：正则替换带回调
来源：http://blog.bbcook.cn/Article/details/gjmoxdpgp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.epnwcf.com/Article/details/gvmrawvdg.sHtML

[U20] Py：缓存函数结果
来源：http://wap.epnwcf.com/Article/details/grinsmgkf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.epnwcf.com/Article/details/gdylzdxil.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.yfazqb.com/Article/details/gxgywnitm.sHtML

@contextlib.contextmanager
来源：http://3g.tarul.cn/Article/details/gtigzyuxf.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.yfazqb.com/Article/details/gmgesszjh.sHtML

list(zip(*m))
来源：http://read.share.fktsv.cn/Article/details/gvjaoqfbq.sHtML

[U23] Py：分块读取大文件
来源：http://baike.yfazqb.com/Article/details/goiqynbrr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.bbcook.cn/Article/details/grpinffto.sHtML

[U24] Py：路径操作
来源：http://www.blog.vehdjk.com/Article/details/gazajwnwv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.epnwcf.com/Article/details/gtezjkwqr.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.bbcook.cn/Article/details/gyeemwssn.sHtML

csv.DictReader(f)
来源：http://read.share.fktsv.cn/Article/details/gnnjproxf.sHtML

[U26] Py：并发下载
来源：http://baike.fktsv.cn/Article/details/ggytkcbzl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.vehdjk.com/Article/details/ghwyvrynp.sHtML

[U27] Py：异步 HTTP
来源：http://wap.sjlbkw.cn/Article/details/grwwsdipa.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.bbcook.cn/Article/details/gvxfnipch.sHtML

[U28] Py：类型别名
来源：http://www.share.vehdjk.com/Article/details/ggzuxyxld.sHtML

UserId = int
来源：http://www.share.vehdjk.com/Article/details/gdaalxmzo.sHtML

[U29] Py：属性校验
来源：http://www.m.share.bbcook.cn/Article/details/gihbdqacv.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.epnwcf.com/Article/details/gagyqstzm.sHtML

[U30] Py：数据类
来源：http://baike.bbcook.cn/Article/details/ginpzqmyo.sHtML

@dataclass(slots=True)
来源：http://mobile.vehdjk.com/Article/details/gbyhtcmsp.sHtML

[U31] Py：单测
来源：http://www.blog.vehdjk.com/Article/details/gvpniokbe.sHtML

python -m pytest -q
来源：http://m.share.sjlbkw.cn/Article/details/goduhtsia.sHtML

[U32] Py：代码格式化
来源：http://www.blog.tarul.cn/Article/details/gwjvkqvqv.sHtML

ruff format . && ruff check --fix .
来源：http://baike.epnwcf.com/Article/details/grmkxplgg.sHtML

[U33] Py：打包发布
来源：http://www.m.share.vehdjk.com/Article/details/gcnttlyab.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.bbcook.cn/Article/details/gyzuicnru.sHtML

[U34] Py：判断编码
来源：http://wap.vehdjk.com/Article/details/gpryrgowl.sHtML

chardet.detect(raw)
来源：http://wap.epnwcf.com/Article/details/gvexyrpgn.sHtML

[U35] Py：发送邮件
来源：http://3g.epnwcf.com/Article/details/glzaxelyx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.vehdjk.com/Article/details/gcecxnpma.sHtML

[U36] Py：定时任务
来源：http://blog.yfazqb.com/Article/details/gsuhjjpwi.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.sjlbkw.cn/Article/details/gfynsxlqi.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.epnwcf.com/Article/details/gacmmcmsf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.bbcook.cn/Article/details/glsyvjaah.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.bbcook.cn/Article/details/gceofgfsr.sHtML

Path(__file__).resolve().parent
来源：http://blog.tarul.cn/Article/details/gsvnfhruy.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.yfazqb.com/Article/details/gjgbpynia.sHtML

sys.stdout.isatty()
来源：http://baike.sjlbkw.cn/Article/details/gbmdgxyei.sHtML

[U40] Py：打印到标准错误
来源：http://wap.sjlbkw.cn/Article/details/gwjfsuucu.sHtML

print("err", file=sys.stderr)
来源：http://wap.fktsv.cn/Article/details/ghrddgsxr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.sjlbkw.cn/Article/details/guvubomml.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.vehdjk.com/Article/details/golgbqylj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.epnwcf.com/Article/details/gkdbxqnpn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.epnwcf.com/Article/details/gyswaauhj.sHtML

[U43] PHP：声明命名空间
来源：http://wap.tarul.cn/Article/details/gncubuvxn.sHtML

namespace App\Http;
来源：http://read.share.tarul.cn/Article/details/gaypydxzg.sHtML

[U44] PHP：开启严格类型
来源：http://baike.yfazqb.com/Article/details/gbmpdeibm.sHtML

declare(strict_types=1);
来源：http://baike.sjlbkw.cn/Article/details/gznrfodzw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.epnwcf.com/Article/details/gsajdycgb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gpxoncreo.sHtML

[U46] PHP：可空类型
来源：http://www.blog.bbcook.cn/Article/details/gmfexexqr.sHtML

?string $name = null
来源：http://blog.tarul.cn/Article/details/gqyvdlwjz.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fktsv.cn/Article/details/geogisqaw.sHtML

int|string $id
来源：http://www.blog.sjlbkw.cn/Article/details/gnpmxxdek.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fktsv.cn/Article/details/gxbdweyvd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.sjlbkw.cn/Article/details/gzlvlzhyr.sHtML

[U49] PHP：只读属性
来源：http://read.share.vehdjk.com/Article/details/gjsggkwfy.sHtML

public readonly string $name
来源：http://www.m.share.fktsv.cn/Article/details/gigolorhs.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.vehdjk.com/Article/details/gfsiqpyps.sHtML

public function __construct(private int $id) {}
来源：http://read.share.sjlbkw.cn/Article/details/gprpriuqm.sHtML

[U51] PHP：数组解构
来源：http://www.share.epnwcf.com/Article/details/gvsvjozfl.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.tarul.cn/Article/details/gubyecvap.sHtML

[U52] PHP：箭头函数
来源：http://3g.fktsv.cn/Article/details/gdikzeokr.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.yfazqb.com/Article/details/gbskdnkaa.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.bbcook.cn/Article/details/gsznkzzvm.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.vehdjk.com/Article/details/gaaporuuk.sHtML

[U54] PHP：空安全调用
来源：http://www.share.tarul.cn/Article/details/gngtahdsv.sHtML

$obj?->method()
来源：http://m.share.epnwcf.com/Article/details/gdjqiidtt.sHtML

[U55] PHP：match 表达式
来源：http://baike.fktsv.cn/Article/details/gmlfmqjmi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.tarul.cn/Article/details/gpjcjtjyk.sHtML

[U56] PHP：命名参数
来源：http://wap.yfazqb.com/Article/details/gwciwbpvt.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gqyguqhhq.sHtML

[U57] PHP：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gvmvmuexv.sHtML

"值: {$a}"
来源：http://www.m.share.yfazqb.com/Article/details/gkpkztwyi.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.epnwcf.com/Article/details/gybutjzjy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fktsv.cn/Article/details/gqrmvnkds.sHtML

[U59] PHP：自定义排序
来源：http://blog.vehdjk.com/Article/details/gmqyazuqv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.vehdjk.com/Article/details/ghzlaucpi.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.tarul.cn/Article/details/gfqmpdzwf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fktsv.cn/Article/details/gshzosliz.sHtML

[U61] PHP：正则
来源：http://wap.tarul.cn/Article/details/ggxqdqzbr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.vehdjk.com/Article/details/gxdmyopdu.sHtML

[U62] PHP：日期对象
来源：http://m.share.tarul.cn/Article/details/glucivdta.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.vehdjk.com/Article/details/gfgjawdkf.sHtML

[U63] PHP：文件读写
来源：http://baike.bbcook.cn/Article/details/gkrkqndyu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.epnwcf.com/Article/details/gmxemhlsh.sHtML

[U64] PHP：目录遍历
来源：http://blog.epnwcf.com/Article/details/gtqitrphm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.yfazqb.com/Article/details/ggtvttsdy.sHtML

[U65] PHP：会话
来源：http://baike.tarul.cn/Article/details/gkywrfyhv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gmcqvyroj.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.vehdjk.com/Article/details/ggzutvdrm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.bbcook.cn/Article/details/ggmbkflei.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.epnwcf.com/Article/details/gfauewdvf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fktsv.cn/Article/details/gaiedjgnm.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.bbcook.cn/Article/details/ggotcrdwm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.tarul.cn/Article/details/gdqpxsnzd.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.vehdjk.com/Article/details/gimddkhcc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fktsv.cn/Article/details/guumcvuos.sHtML

[U70] PHP：PDO 事务
来源：http://baike.sjlbkw.cn/Article/details/gdbnujeaj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.sjlbkw.cn/Article/details/gkwrxlkjk.sHtML


<!-- 参考信息 -->