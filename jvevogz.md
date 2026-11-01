代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://read.share.yfazqb.com/Article/details/gfxfnhues.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fktsv.cn/Article/details/gdriptuqy.sHtML

[S48] C++：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gcemcusws.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.epnwcf.com/Article/details/gaakszsem.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.tarul.cn/Article/details/gpqamplcx.sHtML

[S49] C++：写文件
来源：http://3g.yfazqb.com/Article/details/gfqervmfl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.vehdjk.com/Article/details/gfvsipuwk.sHtML

[S50] C++：格式化数字
来源：http://mobile.bbcook.cn/Article/details/gtmgjvjul.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gykttmsmf.sHtML

[S51] C++：显式类型转换
来源：http://read.share.bbcook.cn/Article/details/gihphjlwj.sHtML

static_cast<double>(a) / b
来源：http://m.share.epnwcf.com/Article/details/gjpeqomvh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.tarul.cn/Article/details/gzwyoqbkz.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.tarul.cn/Article/details/grlnwbyyi.sHtML

[S53] C++：移动语义
来源：http://m.share.tarul.cn/Article/details/gfepnyzav.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.epnwcf.com/Article/details/gxbjvooor.sHtML

[S54] C++：异常处理
来源：http://3g.fktsv.cn/Article/details/gkutagxdv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.sjlbkw.cn/Article/details/gnjlxwgig.sHtML

[S55] C++：结构化绑定
来源：http://read.share.tarul.cn/Article/details/gfzkcvghd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.sjlbkw.cn/Article/details/gvpzntsdh.sHtML

[S56] C++：optional
来源：http://www.m.share.bbcook.cn/Article/details/gmejcqenv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.vehdjk.com/Article/details/gsdrwubcj.sHtML

[S57] C++：编译期常量
来源：http://blog.vehdjk.com/Article/details/gcplothai.sHtML

constexpr int N = 10;
来源：http://www.share.fktsv.cn/Article/details/gbsubzpuv.sHtML

[S58] C++：命名空间
来源：http://mobile.bbcook.cn/Article/details/ggxeftxlk.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.epnwcf.com/Article/details/gvkuphzrq.sHtML

[S59] C++：静态断言
来源：http://www.share.tarul.cn/Article/details/gbyqbxdbr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.bbcook.cn/Article/details/grrtadppq.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fktsv.cn/Article/details/gbcbfopdj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.sjlbkw.cn/Article/details/gtncokxhd.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gyfxaffsi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.yfazqb.com/Article/details/gpfongqki.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gggalassp.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.vehdjk.com/Article/details/gjukheeuv.sHtML

println("Hello")
来源：http://wap.fktsv.cn/Article/details/guspsqvtw.sHtML

[T02] Kotlin：变量
来源：http://www.share.fktsv.cn/Article/details/gpqpjbhbq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fktsv.cn/Article/details/gkwzahssk.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.yfazqb.com/Article/details/gtqjpkxzq.sHtML

"值: $b"
来源：http://blog.sjlbkw.cn/Article/details/gxlbzcexg.sHtML

[T04] Kotlin：空安全
来源：http://wap.tarul.cn/Article/details/gvtfifktn.sHtML

val n: String? = null;  n?.length
来源：http://blog.vehdjk.com/Article/details/gfokrlzbd.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gzarnovyz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.vehdjk.com/Article/details/gtvamvdro.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.yfazqb.com/Article/details/gzjknexws.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.bbcook.cn/Article/details/gbhktqsis.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.sjlbkw.cn/Article/details/getcxynch.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fktsv.cn/Article/details/gotyzayej.sHtML

[T08] Kotlin：数据类
来源：http://read.share.sjlbkw.cn/Article/details/gnnitmsbc.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.epnwcf.com/Article/details/gelcpemou.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.yfazqb.com/Article/details/ggmwgawdj.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.sjlbkw.cn/Article/details/geklazrbp.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fktsv.cn/Article/details/gitlkacxg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.vehdjk.com/Article/details/gcdzcwkag.sHtML

[T11] Kotlin：协程
来源：http://www.blog.yfazqb.com/Article/details/gmpugiiwv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.bbcook.cn/Article/details/gvkkisiwi.sHtML

[T12] Kotlin：解构声明
来源：http://wap.sjlbkw.cn/Article/details/gzphmsxqk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gnvgseqaq.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fktsv.cn/Article/details/gokfmwkih.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.epnwcf.com/Article/details/gtovidojo.sHtML

[T14] Kotlin：循环
来源：http://mobile.yfazqb.com/Article/details/gcntdxyas.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.tarul.cn/Article/details/ghystorwd.sHtML

[T15] Kotlin：接口
来源：http://www.share.epnwcf.com/Article/details/gsfllmhuc.sHtML

interface Shape { fun area(): Double }
来源：http://blog.epnwcf.com/Article/details/gmjqyjhhg.sHtML

[T16] Swift：Hello World
来源：http://wap.tarul.cn/Article/details/gaytdvsmv.sHtML

print("Hello")
来源：http://wap.yfazqb.com/Article/details/gpjpcssix.sHtML

[T17] Swift：变量与常量
来源：http://read.share.vehdjk.com/Article/details/gjtieciog.sHtML

var a = 1;  let b = 2
来源：http://wap.bbcook.cn/Article/details/galjlheuz.sHtML

[T18] Swift：字符串插值
来源：http://read.share.bbcook.cn/Article/details/glbhiftdj.sHtML

"值: \(b)"
来源：http://www.share.bbcook.cn/Article/details/gwluqbnfn.sHtML

[T19] Swift：可选绑定
来源：http://blog.sjlbkw.cn/Article/details/gggrjfghr.sHtML

if let n = opt { print(n) }
来源：http://read.share.fktsv.cn/Article/details/glqrftpen.sHtML

[T20] Swift：数组操作
来源：http://baike.epnwcf.com/Article/details/guastsmpt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfmotijc.sHtML

[T21] Swift：遍历
来源：http://m.share.vehdjk.com/Article/details/gkuzoeamy.sHtML

for x in a { print(x) }
来源：http://read.share.tarul.cn/Article/details/gqeduibxq.sHtML

[T22] Swift：字典
来源：http://mobile.fktsv.cn/Article/details/gbmxrhemp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.sjlbkw.cn/Article/details/gzwycntgb.sHtML

[T23] Swift：函数
来源：http://3g.vehdjk.com/Article/details/geryzvzfq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gsxwdvlol.sHtML

[T24] Swift：闭包
来源：http://wap.epnwcf.com/Article/details/guszilxrg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.yfazqb.com/Article/details/gvqzwxdjb.sHtML

[T25] Swift：结构体
来源：http://www.blog.yfazqb.com/Article/details/grpbjxvbr.sHtML

struct P { var x: Int }
来源：http://3g.sjlbkw.cn/Article/details/gmvpjwhlm.sHtML

[T26] Swift：类与重写
来源：http://blog.sjlbkw.cn/Article/details/gtdisianv.sHtML

class A: Base { override func f() {} }
来源：http://m.share.yfazqb.com/Article/details/gjgduuhcj.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fktsv.cn/Article/details/gpkuqpujc.sHtML

do { try f() } catch { print(error) }
来源：http://3g.yfazqb.com/Article/details/gysqomzia.sHtML

[T28] Swift：枚举
来源：http://read.share.tarul.cn/Article/details/gbiovwbmo.sHtML

enum Color { case red, green }
来源：http://www.share.epnwcf.com/Article/details/gelmrxyye.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.epnwcf.com/Article/details/gxozwqolf.sHtML

guard let x = opt else { return }
来源：http://read.share.epnwcf.com/Article/details/gxmyqfdqu.sHtML

[T30] Swift：协议
来源：http://mobile.epnwcf.com/Article/details/getxmzynu.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fktsv.cn/Article/details/gzsmkhdea.sHtML

[T31] Lua：Hello World
来源：http://read.share.epnwcf.com/Article/details/glhdfwssl.sHtML

print("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gbrlsaszo.sHtML

[T32] Lua：局部变量
来源：http://read.share.fktsv.cn/Article/details/gjuskjgil.sHtML

local a = 1
来源：http://www.share.fktsv.cn/Article/details/gtrxvnhab.sHtML

[T33] Lua：表（数组）
来源：http://www.share.bbcook.cn/Article/details/gxebkelgc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.yfazqb.com/Article/details/gqonspmtg.sHtML

[T34] Lua：遍历表
来源：http://read.share.sjlbkw.cn/Article/details/gotzxrubm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.tarul.cn/Article/details/gtqgeuxqa.sHtML

[T35] Lua：字典表
来源：http://www.m.share.tarul.cn/Article/details/gzghnkhbx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.epnwcf.com/Article/details/gjdofpgen.sHtML

[T36] Lua：函数
来源：http://read.share.tarul.cn/Article/details/gkcyjfoun.sHtML

function add(a, b) return a + b end
来源：http://mobile.vehdjk.com/Article/details/gykyuyenk.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/gesuxoxwr.sHtML

"a" .. "b"
来源：http://www.blog.tarul.cn/Article/details/glweeywvc.sHtML

[T38] Lua：条件
来源：http://www.share.epnwcf.com/Article/details/gucpykjqy.sHtML

if x > 0 then print("正") end
来源：http://3g.tarul.cn/Article/details/gcboybdfa.sHtML

[T39] Lua：模式匹配
来源：http://3g.fktsv.cn/Article/details/gzwzkfnwd.sHtML

string.find(s, "%d+")
来源：http://read.share.vehdjk.com/Article/details/ghzuncgew.sHtML

[T40] Lua：元表
来源：http://mobile.epnwcf.com/Article/details/ghbbrwwil.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.vehdjk.com/Article/details/groyeqkxs.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gokagxclk.sHtML

print "Hello\n";
来源：http://blog.vehdjk.com/Article/details/gctavqfek.sHtML

[T42] Perl：变量类型
来源：http://www.blog.epnwcf.com/Article/details/gjwlzyfra.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.yfazqb.com/Article/details/gncbylrur.sHtML

[T43] Perl：字符串插值
来源：http://wap.epnwcf.com/Article/details/gbvnkvcxl.sHtML

"值: $a"
来源：http://www.m.share.tarul.cn/Article/details/gpddoiahe.sHtML

[T44] Perl：条件
来源：http://m.share.epnwcf.com/Article/details/gfmutdulm.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.vehdjk.com/Article/details/gkauwrpdx.sHtML

[T45] Perl：数组遍历
来源：http://baike.epnwcf.com/Article/details/gbhwetfvs.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fktsv.cn/Article/details/gwgiyijzs.sHtML

[T46] Perl：哈希操作
来源：http://baike.vehdjk.com/Article/details/gtphrktly.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.tarul.cn/Article/details/gktuypcap.sHtML

[T47] Perl：正则捕获
来源：http://read.share.vehdjk.com/Article/details/geywnvxto.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.epnwcf.com/Article/details/gisdcdrhc.sHtML

[T48] Perl：正则替换
来源：http://m.share.fktsv.cn/Article/details/guncylyav.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.epnwcf.com/Article/details/gnyinbhrv.sHtML

[T49] Perl：函数
来源：http://mobile.sjlbkw.cn/Article/details/gknrfodgx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gfvpcbcab.sHtML

[T50] Perl：逐行读文件
来源：http://blog.tarul.cn/Article/details/gakztujlt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.tarul.cn/Article/details/ggpqoipmj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fktsv.cn/Article/details/gabxqeqsr.sHtML

[T51] Scala：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/guvpyxxos.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/gnurxmudk.sHtML

[T52] Scala：变量
来源：http://mobile.yfazqb.com/Article/details/grkigswco.sHtML

val a = 1;  var b = 2
来源：http://mobile.epnwcf.com/Article/details/gvkvjiidx.sHtML

[T53] Scala：字符串插值
来源：http://blog.tarul.cn/Article/details/gfvqgwhbi.sHtML

s"值: $b"
来源：http://blog.fktsv.cn/Article/details/glfxxktby.sHtML

[T54] Scala：集合映射
来源：http://read.share.yfazqb.com/Article/details/glctisgxv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.bbcook.cn/Article/details/gfpyzxwvn.sHtML

[T55] Scala：集合过滤
来源：http://blog.fktsv.cn/Article/details/glftacqro.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fktsv.cn/Article/details/gjuadsbum.sHtML

[T56] Scala：样例类
来源：http://3g.tarul.cn/Article/details/gamfvodhi.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fktsv.cn/Article/details/gaakjsiir.sHtML

[T57] Scala：模式匹配
来源：http://3g.fktsv.cn/Article/details/grpvfnbob.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.bbcook.cn/Article/details/gkpiekkdb.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gckvhaaql.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.yfazqb.com/Article/details/gnwlghcnf.sHtML

[T59] Scala：循环
来源：http://www.m.share.vehdjk.com/Article/details/ggchhlyck.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.epnwcf.com/Article/details/gcreebuza.sHtML

[T60] Scala：折叠
来源：http://blog.epnwcf.com/Article/details/glwkztitx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.sjlbkw.cn/Article/details/gbyyktroj.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gqsvnncea.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.sjlbkw.cn/Article/details/gulrnhejw.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gywssloqz.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.vehdjk.com/Article/details/gfpralakv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fktsv.cn/Article/details/gmdfwyuyd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fktsv.cn/Article/details/gjrekndsj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.yfazqb.com/Article/details/ggnvugonl.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.vehdjk.com/Article/details/ghdqydiwd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.tarul.cn/Article/details/ghegvlqxy.sHtML

[U04] Py：变量调试打印
来源：http://m.share.bbcook.cn/Article/details/grywaqyvw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.yfazqb.com/Article/details/gckmwgtyx.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.epnwcf.com/Article/details/gkoczgfqo.sHtML

list(dict.fromkeys(arr))
来源：http://wap.vehdjk.com/Article/details/gusoliqcz.sHtML

[U06] Py：合并两个字典
来源：http://wap.epnwcf.com/Article/details/gnbzrhiel.sHtML

{**a, **b}
来源：http://www.share.yfazqb.com/Article/details/giuzjhbty.sHtML

[U07] Py：反转字典键值
来源：http://www.share.bbcook.cn/Article/details/gsuncjerc.sHtML

{v: k for k, v in d.items()}
来源：http://3g.epnwcf.com/Article/details/grnrrxlma.sHtML

[U08] Py：展平二维列表
来源：http://3g.sjlbkw.cn/Article/details/gphccwpua.sHtML

[y for x in nested for y in x]
来源：http://3g.fktsv.cn/Article/details/gnwelbipg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.vehdjk.com/Article/details/gxomvyaen.sHtML

max(d, key=d.get)
来源：http://read.share.bbcook.cn/Article/details/gszrlehux.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvpfivwm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.vehdjk.com/Article/details/guhezbcpr.sHtML

[U11] Py：生成器表达式
来源：http://baike.bbcook.cn/Article/details/gcavvgiqh.sHtML

(x * 2 for x in arr)
来源：http://wap.sjlbkw.cn/Article/details/grnghgfco.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.epnwcf.com/Article/details/gkgubainx.sHtML

Counter(arr).most_common(3)
来源：http://www.share.vehdjk.com/Article/details/guyhlhxkt.sHtML

[U13] Py：固定长度队列
来源：http://mobile.tarul.cn/Article/details/gsqxokptv.sHtML

deque(maxlen=10)
来源：http://www.m.share.sjlbkw.cn/Article/details/glqzugggy.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fktsv.cn/Article/details/gvzozdoaw.sHtML

defaultdict(list)
来源：http://3g.vehdjk.com/Article/details/ggvbiyylt.sHtML

[U15] Py：高精度计时
来源：http://wap.yfazqb.com/Article/details/gpqsjiqip.sHtML

t = time.perf_counter()
来源：http://m.share.vehdjk.com/Article/details/gnoeyhumv.sHtML

[U16] Py：命令行参数解析
来源：http://blog.yfazqb.com/Article/details/giujkwkhs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.bbcook.cn/Article/details/ghtmtqsqp.sHtML

[U17] Py：初始化日志
来源：http://www.share.tarul.cn/Article/details/gmldpcmzi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fktsv.cn/Article/details/gbzdszghh.sHtML

[U18] Py：预编译正则
来源：http://mobile.yfazqb.com/Article/details/gvvijbgib.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.bbcook.cn/Article/details/gdoetgujm.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.epnwcf.com/Article/details/gafvthjkm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.yfazqb.com/Article/details/gmevrphrp.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.sjlbkw.cn/Article/details/gwkybfqpc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fktsv.cn/Article/details/gjubipwje.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.tarul.cn/Article/details/gznbtblty.sHtML

@contextlib.contextmanager
来源：http://www.m.share.sjlbkw.cn/Article/details/gapxmzyaf.sHtML

[U22] Py：矩阵转置
来源：http://www.share.bbcook.cn/Article/details/grykjtelh.sHtML

list(zip(*m))
来源：http://3g.bbcook.cn/Article/details/gwirtzcgv.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.tarul.cn/Article/details/gulmojmlz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.sjlbkw.cn/Article/details/gocueokgo.sHtML

[U24] Py：路径操作
来源：http://www.m.share.yfazqb.com/Article/details/gckngshou.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.tarul.cn/Article/details/geltvyzad.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.tarul.cn/Article/details/grqaowbpv.sHtML

csv.DictReader(f)
来源：http://www.blog.bbcook.cn/Article/details/gkmycufiy.sHtML

[U26] Py：并发下载
来源：http://mobile.vehdjk.com/Article/details/grwkbzhzc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.yfazqb.com/Article/details/gktqagyhx.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.epnwcf.com/Article/details/gednmfykh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.yfazqb.com/Article/details/ghhnxxfev.sHtML

[U28] Py：类型别名
来源：http://3g.sjlbkw.cn/Article/details/gbtylmvhm.sHtML

UserId = int
来源：http://www.blog.sjlbkw.cn/Article/details/geilnodbs.sHtML

[U29] Py：属性校验
来源：http://read.share.bbcook.cn/Article/details/gwdnpaamv.sHtML

@property 与 @x.setter 配合
来源：http://wap.fktsv.cn/Article/details/givqcveat.sHtML

[U30] Py：数据类
来源：http://www.share.vehdjk.com/Article/details/gxisladbt.sHtML

@dataclass(slots=True)
来源：http://read.share.epnwcf.com/Article/details/gthvhkxvz.sHtML

[U31] Py：单测
来源：http://www.share.yfazqb.com/Article/details/gjxufwnxt.sHtML

python -m pytest -q
来源：http://www.share.sjlbkw.cn/Article/details/gipqcadtn.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gjseofrie.sHtML

ruff format . && ruff check --fix .
来源：http://3g.epnwcf.com/Article/details/gzsxlgyzh.sHtML

[U33] Py：打包发布
来源：http://baike.yfazqb.com/Article/details/gtibxkrin.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.yfazqb.com/Article/details/gtbcnsfux.sHtML

[U34] Py：判断编码
来源：http://read.share.sjlbkw.cn/Article/details/giqncrxhb.sHtML

chardet.detect(raw)
来源：http://blog.tarul.cn/Article/details/gmigwvrvb.sHtML

[U35] Py：发送邮件
来源：http://www.share.tarul.cn/Article/details/gxvdtxfrx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.vehdjk.com/Article/details/gljnijuha.sHtML

[U36] Py：定时任务
来源：http://3g.epnwcf.com/Article/details/gnarrqvhw.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.epnwcf.com/Article/details/gxeeiscsi.sHtML

[U37] Py：读写 Excel
来源：http://www.share.yfazqb.com/Article/details/gjjedcsnq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fktsv.cn/Article/details/gbkwivaru.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.vehdjk.com/Article/details/glngrrjfw.sHtML

Path(__file__).resolve().parent
来源：http://www.share.vehdjk.com/Article/details/gxbaabnyo.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.epnwcf.com/Article/details/gohnmymro.sHtML

sys.stdout.isatty()
来源：http://m.share.sjlbkw.cn/Article/details/gzvvjpdyk.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.yfazqb.com/Article/details/gdvseqdan.sHtML

print("err", file=sys.stderr)
来源：http://baike.vehdjk.com/Article/details/gmeemrkjx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.epnwcf.com/Article/details/gwjdpidwg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.vehdjk.com/Article/details/gjazwnhqf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fktsv.cn/Article/details/guhrlwogm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.sjlbkw.cn/Article/details/gxpadvhht.sHtML

[U43] PHP：声明命名空间
来源：http://baike.tarul.cn/Article/details/gbdkdvgio.sHtML

namespace App\Http;
来源：http://m.share.epnwcf.com/Article/details/gappqlepy.sHtML

[U44] PHP：开启严格类型
来源：http://baike.bbcook.cn/Article/details/gbaudjxry.sHtML

declare(strict_types=1);
来源：http://www.m.share.yfazqb.com/Article/details/glggqezxn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.tarul.cn/Article/details/grdguhmyx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gozrqeoxg.sHtML

[U46] PHP：可空类型
来源：http://baike.sjlbkw.cn/Article/details/gharwtjct.sHtML

?string $name = null
来源：http://www.blog.sjlbkw.cn/Article/details/goqvbxufb.sHtML

[U47] PHP：联合类型
来源：http://wap.epnwcf.com/Article/details/gyhiukgnk.sHtML

int|string $id
来源：http://mobile.tarul.cn/Article/details/geefgmxbh.sHtML

[U48] PHP：纯枚举
来源：http://m.share.tarul.cn/Article/details/gmrdxpzrg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.bbcook.cn/Article/details/gytwlvuuy.sHtML

[U49] PHP：只读属性
来源：http://www.share.bbcook.cn/Article/details/gtzmvtcfa.sHtML

public readonly string $name
来源：http://www.m.share.tarul.cn/Article/details/geerwinmg.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.sjlbkw.cn/Article/details/ghsqrxhwa.sHtML

public function __construct(private int $id) {}
来源：http://baike.yfazqb.com/Article/details/glnebmuam.sHtML

[U51] PHP：数组解构
来源：http://baike.epnwcf.com/Article/details/gbuxsrhlp.sHtML

[$a, $b] = $arr;
来源：http://baike.epnwcf.com/Article/details/gimyviakf.sHtML

[U52] PHP：箭头函数
来源：http://blog.vehdjk.com/Article/details/gchyzpplq.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.bbcook.cn/Article/details/gbzfopdrw.sHtML

[U53] PHP：空合并运算符
来源：http://3g.vehdjk.com/Article/details/ghzqhgeba.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.sjlbkw.cn/Article/details/gfthlvirv.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fktsv.cn/Article/details/gczzbefwd.sHtML

$obj?->method()
来源：http://read.share.bbcook.cn/Article/details/gtffjkkvh.sHtML

[U55] PHP：match 表达式
来源：http://3g.tarul.cn/Article/details/gklbkiaxi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.bbcook.cn/Article/details/gfrzpxkmw.sHtML

[U56] PHP：命名参数
来源：http://www.blog.epnwcf.com/Article/details/gfmitdcio.sHtML

f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gtaxbstzr.sHtML

[U57] PHP：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gtthdmdlu.sHtML

"值: {$a}"
来源：http://www.m.share.vehdjk.com/Article/details/gfdqckcoz.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.bbcook.cn/Article/details/grzplzabq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.epnwcf.com/Article/details/gekqyenvf.sHtML

[U59] PHP：自定义排序
来源：http://3g.vehdjk.com/Article/details/guacaltwt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.bbcook.cn/Article/details/ganhplwcn.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.yfazqb.com/Article/details/gadvakclh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.vehdjk.com/Article/details/gdyxniqnn.sHtML

[U61] PHP：正则
来源：http://3g.yfazqb.com/Article/details/gnbbbzhud.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.sjlbkw.cn/Article/details/gwypiwtqx.sHtML

[U62] PHP：日期对象
来源：http://blog.epnwcf.com/Article/details/gjphlqhwc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.tarul.cn/Article/details/gvibqmpma.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fktsv.cn/Article/details/gwnofgijj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.bbcook.cn/Article/details/gqknxgdqs.sHtML

[U64] PHP：目录遍历
来源：http://wap.vehdjk.com/Article/details/gzvbqrdvi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.vehdjk.com/Article/details/gezvrtowt.sHtML

[U65] PHP：会话
来源：http://read.share.bbcook.cn/Article/details/gecfwaifk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fktsv.cn/Article/details/gkonlbcff.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fktsv.cn/Article/details/gysqgzezq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.tarul.cn/Article/details/glazelnwe.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.vehdjk.com/Article/details/gccijmjde.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.epnwcf.com/Article/details/glkiwxzms.sHtML

[U68] PHP：PDO 连接
来源：http://baike.yfazqb.com/Article/details/guvcozxyw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.yfazqb.com/Article/details/gauvdujhl.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fktsv.cn/Article/details/gnhtwfexe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.epnwcf.com/Article/details/grsvsyslx.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsaompog.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.epnwcf.com/Article/details/glcyrpdeb.sHtML

[U71] PHP：抛出异常
来源：http://mobile.vehdjk.com/Article/details/gkrlscjbz.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.yfazqb.com/Article/details/gxwackros.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.bbcook.cn/Article/details/ggwvchdoh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.bbcook.cn/Article/details/ghhsxandx.sHtML


<!-- 参考信息 -->