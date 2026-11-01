代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://read.share.fktsv.cn/Article/details/gphtupdjk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fktsv.cn/Article/details/ggwzugilu.sHtML

[S48] C++：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gunocfylb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.sjlbkw.cn/Article/details/gkbqbewpx.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.tarul.cn/Article/details/gqdyeaxix.sHtML

[S49] C++：写文件
来源：http://www.m.share.vehdjk.com/Article/details/gpanmtdtl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.tarul.cn/Article/details/ggofehrcf.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.yfazqb.com/Article/details/gzomazola.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/ggpdnvzju.sHtML

[S51] C++：显式类型转换
来源：http://wap.yfazqb.com/Article/details/gvsabmccr.sHtML

static_cast<double>(a) / b
来源：http://mobile.vehdjk.com/Article/details/giumytobu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.tarul.cn/Article/details/gfzhqsccf.sHtML

int size() const noexcept { return n_; }
来源：http://blog.epnwcf.com/Article/details/gofvdjkqq.sHtML

[S53] C++：移动语义
来源：http://baike.epnwcf.com/Article/details/gxiulodxs.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.vehdjk.com/Article/details/gypftekkt.sHtML

[S54] C++：异常处理
来源：http://read.share.yfazqb.com/Article/details/gttprujbx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.tarul.cn/Article/details/gvinswygq.sHtML

[S55] C++：结构化绑定
来源：http://mobile.bbcook.cn/Article/details/gdnqjtvmf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gvdgffrxw.sHtML

[S56] C++：optional
来源：http://read.share.fktsv.cn/Article/details/gnxkijfhp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.epnwcf.com/Article/details/gulgjhuip.sHtML

[S57] C++：编译期常量
来源：http://www.blog.epnwcf.com/Article/details/gmpwbtylj.sHtML

constexpr int N = 10;
来源：http://3g.sjlbkw.cn/Article/details/gbpurriru.sHtML

[S58] C++：命名空间
来源：http://baike.vehdjk.com/Article/details/gumoeznmi.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.yfazqb.com/Article/details/gzpgdsywc.sHtML

[S59] C++：静态断言
来源：http://mobile.vehdjk.com/Article/details/gdzjzjusa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.sjlbkw.cn/Article/details/gvrdjgwgl.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.epnwcf.com/Article/details/gnfuzazki.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.yfazqb.com/Article/details/gpbtufxcr.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gjtcyyaub.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fktsv.cn/Article/details/gutizunjd.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gerjfoxae.sHtML

[T01] Kotlin：Hello World
来源：http://wap.yfazqb.com/Article/details/gqjswqsgy.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/gnzdrjgwt.sHtML

[T02] Kotlin：变量
来源：http://3g.epnwcf.com/Article/details/gccioxhgi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.bbcook.cn/Article/details/ghzueplvb.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.tarul.cn/Article/details/gszvlofok.sHtML

"值: $b"
来源：http://www.blog.tarul.cn/Article/details/gfqbnfhov.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.yfazqb.com/Article/details/gjbddiqfq.sHtML

val n: String? = null;  n?.length
来源：http://www.share.vehdjk.com/Article/details/gzyjypmtv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.epnwcf.com/Article/details/grenjnfxe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.epnwcf.com/Article/details/guhokusnt.sHtML

[T06] Kotlin：集合映射
来源：http://wap.sjlbkw.cn/Article/details/gnlxpvgvk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.tarul.cn/Article/details/gwuybchsa.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.yfazqb.com/Article/details/gfmjszstk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.epnwcf.com/Article/details/gocpjawfl.sHtML

[T08] Kotlin：数据类
来源：http://3g.epnwcf.com/Article/details/gyrcptuln.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.epnwcf.com/Article/details/gsextppnv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.yfazqb.com/Article/details/gaivedhaj.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fktsv.cn/Article/details/gqkhndxwf.sHtML

[T10] Kotlin：默认参数
来源：http://3g.vehdjk.com/Article/details/guzcqndoq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.tarul.cn/Article/details/grhtsyirt.sHtML

[T11] Kotlin：协程
来源：http://3g.sjlbkw.cn/Article/details/gcwmdtvvj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.bbcook.cn/Article/details/ggdowvemb.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.sjlbkw.cn/Article/details/gerheailv.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.vehdjk.com/Article/details/gjkiofute.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.bbcook.cn/Article/details/gyjmuabku.sHtML

val m = mapOf("a" to 1)
来源：http://blog.vehdjk.com/Article/details/gkwgwvrdt.sHtML

[T14] Kotlin：循环
来源：http://mobile.tarul.cn/Article/details/gfwawvpzn.sHtML

for (i in 1..10) println(i)
来源：http://3g.yfazqb.com/Article/details/gcmscbzpb.sHtML

[T15] Kotlin：接口
来源：http://mobile.fktsv.cn/Article/details/gqkfdioxr.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.vehdjk.com/Article/details/grhywxptt.sHtML

[T16] Swift：Hello World
来源：http://m.share.vehdjk.com/Article/details/gbuxnknvl.sHtML

print("Hello")
来源：http://www.blog.epnwcf.com/Article/details/guwwvcrrw.sHtML

[T17] Swift：变量与常量
来源：http://read.share.bbcook.cn/Article/details/gkadgeqdv.sHtML

var a = 1;  let b = 2
来源：http://read.share.sjlbkw.cn/Article/details/gmkmauawi.sHtML

[T18] Swift：字符串插值
来源：http://wap.vehdjk.com/Article/details/gpmbmfcut.sHtML

"值: \(b)"
来源：http://www.m.share.epnwcf.com/Article/details/glgwuqkfl.sHtML

[T19] Swift：可选绑定
来源：http://3g.vehdjk.com/Article/details/gpeysnqos.sHtML

if let n = opt { print(n) }
来源：http://mobile.bbcook.cn/Article/details/ghzklngrz.sHtML

[T20] Swift：数组操作
来源：http://baike.tarul.cn/Article/details/gistvzuzw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fktsv.cn/Article/details/gbtvigkhf.sHtML

[T21] Swift：遍历
来源：http://read.share.fktsv.cn/Article/details/gvbpeqrlu.sHtML

for x in a { print(x) }
来源：http://3g.bbcook.cn/Article/details/gavvreptb.sHtML

[T22] Swift：字典
来源：http://blog.fktsv.cn/Article/details/ggyvdzgte.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.tarul.cn/Article/details/gztneetda.sHtML

[T23] Swift：函数
来源：http://m.share.vehdjk.com/Article/details/gcrvkdume.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fktsv.cn/Article/details/gnxtirpeu.sHtML

[T24] Swift：闭包
来源：http://www.m.share.yfazqb.com/Article/details/gkgdwdpxd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.epnwcf.com/Article/details/gzouirmqk.sHtML

[T25] Swift：结构体
来源：http://wap.epnwcf.com/Article/details/gmsewbbqa.sHtML

struct P { var x: Int }
来源：http://m.share.yfazqb.com/Article/details/gszsktrrz.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fktsv.cn/Article/details/gxcjozpfk.sHtML

class A: Base { override func f() {} }
来源：http://3g.fktsv.cn/Article/details/gwfbjkpnh.sHtML

[T27] Swift：错误处理
来源：http://blog.sjlbkw.cn/Article/details/ghoadhyyi.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fktsv.cn/Article/details/gwdmxgnjk.sHtML

[T28] Swift：枚举
来源：http://read.share.fktsv.cn/Article/details/gqoxewcoe.sHtML

enum Color { case red, green }
来源：http://read.share.sjlbkw.cn/Article/details/geoulnrci.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.epnwcf.com/Article/details/goqvcsuwh.sHtML

guard let x = opt else { return }
来源：http://wap.yfazqb.com/Article/details/gewqdcqdl.sHtML

[T30] Swift：协议
来源：http://m.share.fktsv.cn/Article/details/gqjxkrorh.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.tarul.cn/Article/details/gfqnqrkkz.sHtML

[T31] Lua：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gsfzwjoue.sHtML

print("Hello")
来源：http://mobile.fktsv.cn/Article/details/gsojoflwt.sHtML

[T32] Lua：局部变量
来源：http://3g.epnwcf.com/Article/details/gharraxbd.sHtML

local a = 1
来源：http://3g.vehdjk.com/Article/details/gquowioak.sHtML

[T33] Lua：表（数组）
来源：http://baike.tarul.cn/Article/details/gtbgbofwq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.tarul.cn/Article/details/glrjtarjp.sHtML

[T34] Lua：遍历表
来源：http://baike.sjlbkw.cn/Article/details/gizqngerw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.vehdjk.com/Article/details/ggdxtlbzt.sHtML

[T35] Lua：字典表
来源：http://read.share.yfazqb.com/Article/details/gtwplkgmi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.tarul.cn/Article/details/gkozosntq.sHtML

[T36] Lua：函数
来源：http://3g.bbcook.cn/Article/details/gmtesokyi.sHtML

function add(a, b) return a + b end
来源：http://m.share.bbcook.cn/Article/details/gnnajpvhv.sHtML

[T37] Lua：字符串拼接
来源：http://blog.vehdjk.com/Article/details/gofrackym.sHtML

"a" .. "b"
来源：http://mobile.tarul.cn/Article/details/gmfomcsif.sHtML

[T38] Lua：条件
来源：http://blog.yfazqb.com/Article/details/ghlucobsv.sHtML

if x > 0 then print("正") end
来源：http://mobile.vehdjk.com/Article/details/gwyewlhfe.sHtML

[T39] Lua：模式匹配
来源：http://3g.bbcook.cn/Article/details/gghvbruiu.sHtML

string.find(s, "%d+")
来源：http://wap.sjlbkw.cn/Article/details/gduyietxb.sHtML

[T40] Lua：元表
来源：http://3g.sjlbkw.cn/Article/details/gpqxotgut.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.yfazqb.com/Article/details/gjyflfoja.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/ggfyxfemh.sHtML

print "Hello\n";
来源：http://3g.yfazqb.com/Article/details/gudodhpie.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.tarul.cn/Article/details/glbkmuesm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fktsv.cn/Article/details/gbqikjlay.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/guemaarvh.sHtML

"值: $a"
来源：http://baike.tarul.cn/Article/details/gigpxtbwa.sHtML

[T44] Perl：条件
来源：http://www.m.share.epnwcf.com/Article/details/giohvorhb.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.tarul.cn/Article/details/gpnxfllbk.sHtML

[T45] Perl：数组遍历
来源：http://m.share.epnwcf.com/Article/details/gbrhilfma.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.yfazqb.com/Article/details/gamnvynuz.sHtML

[T46] Perl：哈希操作
来源：http://read.share.tarul.cn/Article/details/gvaedbyca.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fktsv.cn/Article/details/gpidghwjf.sHtML

[T47] Perl：正则捕获
来源：http://blog.epnwcf.com/Article/details/gkaeszkjk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.sjlbkw.cn/Article/details/grynpzckz.sHtML

[T48] Perl：正则替换
来源：http://mobile.yfazqb.com/Article/details/golndigft.sHtML

$s =~ s/old/new/g;
来源：http://m.share.tarul.cn/Article/details/gruvnzajh.sHtML

[T49] Perl：函数
来源：http://mobile.bbcook.cn/Article/details/gxotzwmaq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/giulrpupn.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gpypypudf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fktsv.cn/Article/details/gwswlcpic.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.bbcook.cn/Article/details/gnnwlsuod.sHtML

[T51] Scala：Hello World
来源：http://read.share.vehdjk.com/Article/details/glvqjrtos.sHtML

println("Hello")
来源：http://wap.vehdjk.com/Article/details/gssysnrjy.sHtML

[T52] Scala：变量
来源：http://www.blog.sjlbkw.cn/Article/details/gguvaiveo.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.yfazqb.com/Article/details/gsfpscdzo.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/geziupwas.sHtML

s"值: $b"
来源：http://baike.epnwcf.com/Article/details/glgghpecw.sHtML

[T54] Scala：集合映射
来源：http://m.share.fktsv.cn/Article/details/gxnmhagyp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gyfotqsnx.sHtML

[T55] Scala：集合过滤
来源：http://read.share.epnwcf.com/Article/details/glpumwkeh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.epnwcf.com/Article/details/gdxeylzzf.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fktsv.cn/Article/details/grsxtxbsd.sHtML

case class User(name: String, age: Int)
来源：http://read.share.vehdjk.com/Article/details/ggcpvxmoc.sHtML

[T57] Scala：模式匹配
来源：http://www.share.sjlbkw.cn/Article/details/gluskxikm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fktsv.cn/Article/details/gqtphhyjj.sHtML

[T58] Scala：函数定义
来源：http://baike.sjlbkw.cn/Article/details/gnjzhccgq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fktsv.cn/Article/details/gbvrqrbzy.sHtML

[T59] Scala：循环
来源：http://baike.tarul.cn/Article/details/giwrijjss.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fktsv.cn/Article/details/gbdbyokau.sHtML

[T60] Scala：折叠
来源：http://www.m.share.vehdjk.com/Article/details/gdwsqipsg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.sjlbkw.cn/Article/details/gpjtpzgwd.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gzaqxycmq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.sjlbkw.cn/Article/details/gxcsawpvf.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gtkdbrhzu.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.epnwcf.com/Article/details/gghswcuzi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.epnwcf.com/Article/details/gwrihvzft.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fktsv.cn/Article/details/gekwvarve.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.epnwcf.com/Article/details/gevjnqsar.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.bbcook.cn/Article/details/ghesfjima.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.vehdjk.com/Article/details/goquageix.sHtML

[U04] Py：变量调试打印
来源：http://baike.sjlbkw.cn/Article/details/gqdrdopxf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.yfazqb.com/Article/details/ghptoqqcn.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.epnwcf.com/Article/details/gblpnbvkg.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fktsv.cn/Article/details/gdgcekjwv.sHtML

[U06] Py：合并两个字典
来源：http://3g.bbcook.cn/Article/details/gkfkzjqle.sHtML

{**a, **b}
来源：http://www.blog.tarul.cn/Article/details/gewcmwyej.sHtML

[U07] Py：反转字典键值
来源：http://www.share.vehdjk.com/Article/details/grvtzupge.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.yfazqb.com/Article/details/gdgrinsgz.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.sjlbkw.cn/Article/details/gthqjsvtq.sHtML

[y for x in nested for y in x]
来源：http://blog.vehdjk.com/Article/details/ggnnehuan.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.yfazqb.com/Article/details/gusvofqpn.sHtML

max(d, key=d.get)
来源：http://m.share.sjlbkw.cn/Article/details/gzktynmyu.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.sjlbkw.cn/Article/details/grbbblqga.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fktsv.cn/Article/details/gtowfabkq.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fktsv.cn/Article/details/gkxadzocw.sHtML

(x * 2 for x in arr)
来源：http://mobile.sjlbkw.cn/Article/details/gishmrffg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.bbcook.cn/Article/details/gqcubnrut.sHtML

Counter(arr).most_common(3)
来源：http://m.share.vehdjk.com/Article/details/gkenebzei.sHtML

[U13] Py：固定长度队列
来源：http://read.share.yfazqb.com/Article/details/gqudomodi.sHtML

deque(maxlen=10)
来源：http://www.m.share.vehdjk.com/Article/details/gtkaihces.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.yfazqb.com/Article/details/grpslqtih.sHtML

defaultdict(list)
来源：http://www.blog.epnwcf.com/Article/details/gdqojqmlm.sHtML

[U15] Py：高精度计时
来源：http://baike.vehdjk.com/Article/details/gnoieywsp.sHtML

t = time.perf_counter()
来源：http://baike.yfazqb.com/Article/details/gkgejweiy.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.bbcook.cn/Article/details/goxtlxqqk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.yfazqb.com/Article/details/grzqyejtn.sHtML

[U17] Py：初始化日志
来源：http://3g.epnwcf.com/Article/details/gyfaijppy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.tarul.cn/Article/details/gbakbszjz.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.yfazqb.com/Article/details/gdpbmoglz.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fktsv.cn/Article/details/ggvmpeflc.sHtML

[U19] Py：正则替换带回调
来源：http://3g.yfazqb.com/Article/details/goyjfggil.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.yfazqb.com/Article/details/gojsvkxuj.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fktsv.cn/Article/details/gjkgaozdg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.sjlbkw.cn/Article/details/ggkdlidzz.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.tarul.cn/Article/details/gdoonzqii.sHtML

@contextlib.contextmanager
来源：http://baike.yfazqb.com/Article/details/guplrsywu.sHtML

[U22] Py：矩阵转置
来源：http://mobile.yfazqb.com/Article/details/ghjujkrhq.sHtML

list(zip(*m))
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbetgusi.sHtML

[U23] Py：分块读取大文件
来源：http://blog.yfazqb.com/Article/details/gxpguglop.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.tarul.cn/Article/details/gjyrzkrfx.sHtML

[U24] Py：路径操作
来源：http://www.m.share.sjlbkw.cn/Article/details/giamfhhru.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gavyhhong.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fktsv.cn/Article/details/gkdudixiy.sHtML

csv.DictReader(f)
来源：http://www.share.sjlbkw.cn/Article/details/gllmjwgpi.sHtML

[U26] Py：并发下载
来源：http://mobile.epnwcf.com/Article/details/gmuxvtnqi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.epnwcf.com/Article/details/gnynvrhpr.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.epnwcf.com/Article/details/ghtejlhor.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgddpigg.sHtML

[U28] Py：类型别名
来源：http://wap.epnwcf.com/Article/details/gkdocxytb.sHtML

UserId = int
来源：http://wap.fktsv.cn/Article/details/glgnrsmyl.sHtML

[U29] Py：属性校验
来源：http://blog.yfazqb.com/Article/details/glhtudgyg.sHtML

@property 与 @x.setter 配合
来源：http://baike.sjlbkw.cn/Article/details/gsgxpcqmk.sHtML

[U30] Py：数据类
来源：http://wap.sjlbkw.cn/Article/details/gubabqacr.sHtML

@dataclass(slots=True)
来源：http://mobile.sjlbkw.cn/Article/details/ghrqilnbs.sHtML

[U31] Py：单测
来源：http://baike.sjlbkw.cn/Article/details/garbncpaz.sHtML

python -m pytest -q
来源：http://www.m.share.fktsv.cn/Article/details/gxhykerae.sHtML

[U32] Py：代码格式化
来源：http://3g.epnwcf.com/Article/details/gahziaycs.sHtML

ruff format . && ruff check --fix .
来源：http://baike.epnwcf.com/Article/details/gyfmwkdir.sHtML

[U33] Py：打包发布
来源：http://3g.epnwcf.com/Article/details/gvchjonnt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.sjlbkw.cn/Article/details/gktnotkik.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fktsv.cn/Article/details/gjtgvhtba.sHtML

chardet.detect(raw)
来源：http://www.share.tarul.cn/Article/details/gytspfspk.sHtML

[U35] Py：发送邮件
来源：http://baike.bbcook.cn/Article/details/gtxczqiax.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.epnwcf.com/Article/details/gzxpyrxrf.sHtML

[U36] Py：定时任务
来源：http://wap.yfazqb.com/Article/details/gzdsfygsb.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.sjlbkw.cn/Article/details/gmvibbcxw.sHtML

[U37] Py：读写 Excel
来源：http://mobile.yfazqb.com/Article/details/gclltawzg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.epnwcf.com/Article/details/ggghqjmpr.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.bbcook.cn/Article/details/grqdtpqui.sHtML

Path(__file__).resolve().parent
来源：http://3g.epnwcf.com/Article/details/gocgppbjv.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.vehdjk.com/Article/details/gbnmvlhun.sHtML

sys.stdout.isatty()
来源：http://m.share.bbcook.cn/Article/details/gbxcsgcrj.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.bbcook.cn/Article/details/gqvfrtjqx.sHtML

print("err", file=sys.stderr)
来源：http://baike.yfazqb.com/Article/details/goqisynra.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fktsv.cn/Article/details/glmlcigmv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.tarul.cn/Article/details/gtcrgqmfz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.bbcook.cn/Article/details/gsklyynrn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.bbcook.cn/Article/details/gbefedime.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.vehdjk.com/Article/details/gwiwwujmv.sHtML

namespace App\Http;
来源：http://www.share.fktsv.cn/Article/details/ggdnebfci.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.bbcook.cn/Article/details/ggbbbewhl.sHtML

declare(strict_types=1);
来源：http://read.share.yfazqb.com/Article/details/gewbzoglo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.yfazqb.com/Article/details/gjxzpqrha.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gzhvpfzpu.sHtML

[U46] PHP：可空类型
来源：http://read.share.tarul.cn/Article/details/ggmyqtjrt.sHtML

?string $name = null
来源：http://blog.epnwcf.com/Article/details/gymfgqutz.sHtML

[U47] PHP：联合类型
来源：http://mobile.bbcook.cn/Article/details/gammdekuc.sHtML

int|string $id
来源：http://read.share.bbcook.cn/Article/details/gqhuhzejf.sHtML

[U48] PHP：纯枚举
来源：http://m.share.vehdjk.com/Article/details/gmmkrmbrl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.tarul.cn/Article/details/gqnrhngkl.sHtML

[U49] PHP：只读属性
来源：http://blog.yfazqb.com/Article/details/gwyaiwidj.sHtML

public readonly string $name
来源：http://mobile.tarul.cn/Article/details/gybxgtwfo.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.vehdjk.com/Article/details/gvkellkaa.sHtML

public function __construct(private int $id) {}
来源：http://blog.bbcook.cn/Article/details/ghppauyuy.sHtML

[U51] PHP：数组解构
来源：http://m.share.yfazqb.com/Article/details/gvwtpujwg.sHtML

[$a, $b] = $arr;
来源：http://wap.vehdjk.com/Article/details/gozqxeoig.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fktsv.cn/Article/details/godujcrhd.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fktsv.cn/Article/details/gtxilzpzb.sHtML

[U53] PHP：空合并运算符
来源：http://3g.yfazqb.com/Article/details/glmasezos.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.bbcook.cn/Article/details/gydfxbokm.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.sjlbkw.cn/Article/details/goegdfovz.sHtML

$obj?->method()
来源：http://wap.bbcook.cn/Article/details/gxokmowsy.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.vehdjk.com/Article/details/gjoukjzmg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fktsv.cn/Article/details/gfdrzfvsl.sHtML

[U56] PHP：命名参数
来源：http://m.share.yfazqb.com/Article/details/gxjfpnxva.sHtML

f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/gvjvkfgpc.sHtML

[U57] PHP：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gilwgyjqn.sHtML

"值: {$a}"
来源：http://read.share.vehdjk.com/Article/details/ghmcgkwuu.sHtML

[U58] PHP：数组三件套
来源：http://mobile.sjlbkw.cn/Article/details/gnrpapkzn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.epnwcf.com/Article/details/golkdaoxt.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.yfazqb.com/Article/details/gbgqpolnp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.vehdjk.com/Article/details/gstjeeodi.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.bbcook.cn/Article/details/geajhutaz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.vehdjk.com/Article/details/gajgicoeq.sHtML

[U61] PHP：正则
来源：http://blog.tarul.cn/Article/details/giruuhmkq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.tarul.cn/Article/details/gnojwuwuf.sHtML

[U62] PHP：日期对象
来源：http://baike.sjlbkw.cn/Article/details/gqqyzihdi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.yfazqb.com/Article/details/ggamiwabu.sHtML

[U63] PHP：文件读写
来源：http://baike.vehdjk.com/Article/details/gsbnycpnj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.vehdjk.com/Article/details/gqpctaosz.sHtML

[U64] PHP：目录遍历
来源：http://www.share.epnwcf.com/Article/details/gofxcedqb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.vehdjk.com/Article/details/gwbccikld.sHtML

[U65] PHP：会话
来源：http://read.share.bbcook.cn/Article/details/gvlkbwqpd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.epnwcf.com/Article/details/ghnwbiazb.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.epnwcf.com/Article/details/gglltqmlm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.vehdjk.com/Article/details/gshqdwrjm.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.sjlbkw.cn/Article/details/gicbxmtgv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.sjlbkw.cn/Article/details/gvxdurhaj.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.vehdjk.com/Article/details/glqemzsrq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.bbcook.cn/Article/details/gucqugcsj.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.yfazqb.com/Article/details/gmroagzly.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.tarul.cn/Article/details/gvzoxucnx.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.bbcook.cn/Article/details/grjfobvqv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.vehdjk.com/Article/details/gwvvennyz.sHtML

[U71] PHP：抛出异常
来源：http://baike.sjlbkw.cn/Article/details/gxkbxzuku.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.bbcook.cn/Article/details/gkdumaexo.sHtML

[U72] PHP：写错误日志
来源：http://m.share.bbcook.cn/Article/details/gtwmffxeo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.yfazqb.com/Article/details/gfzitdmqi.sHtML


<!-- 参考信息 -->