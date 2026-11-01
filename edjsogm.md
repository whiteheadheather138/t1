代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://mobile.vehdjk.com/Article/details/ggzcdryjb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.epnwcf.com/Article/details/gwfgfyfnf.sHtML

[S48] C++：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gjllrypcg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.epnwcf.com/Article/details/ggajxuknn.sHtML

while (std::getline(in, line)) { }
来源：http://wap.bbcook.cn/Article/details/gbbrafohq.sHtML

[S49] C++：写文件
来源：http://wap.yfazqb.com/Article/details/grhbhfrif.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.epnwcf.com/Article/details/gjyawoatu.sHtML

[S50] C++：格式化数字
来源：http://mobile.tarul.cn/Article/details/gnxrgxwrw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gwfzvwrnp.sHtML

[S51] C++：显式类型转换
来源：http://wap.yfazqb.com/Article/details/gyqugorno.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.vehdjk.com/Article/details/gxdrrgrwq.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.vehdjk.com/Article/details/gwlhwmgya.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.vehdjk.com/Article/details/ghxjqkcec.sHtML

[S53] C++：移动语义
来源：http://mobile.bbcook.cn/Article/details/grnvncfam.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.bbcook.cn/Article/details/gfzfhprwg.sHtML

[S54] C++：异常处理
来源：http://wap.epnwcf.com/Article/details/gvyztomep.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.bbcook.cn/Article/details/gnvqswhau.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.epnwcf.com/Article/details/goetgqxix.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.bbcook.cn/Article/details/ghtoxqsrs.sHtML

[S56] C++：optional
来源：http://3g.vehdjk.com/Article/details/ggnyqsbxx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.sjlbkw.cn/Article/details/glnhnvzqa.sHtML

[S57] C++：编译期常量
来源：http://3g.bbcook.cn/Article/details/gufliozda.sHtML

constexpr int N = 10;
来源：http://baike.vehdjk.com/Article/details/gjfkmnmik.sHtML

[S58] C++：命名空间
来源：http://read.share.vehdjk.com/Article/details/gfklndnga.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.sjlbkw.cn/Article/details/gupmadatu.sHtML

[S59] C++：静态断言
来源：http://blog.tarul.cn/Article/details/gnsxbtdwx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.epnwcf.com/Article/details/gmsrzfzkf.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.bbcook.cn/Article/details/gftyxdith.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.epnwcf.com/Article/details/gxjlauitz.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gfnkhtjkf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.bbcook.cn/Article/details/gtwyfbetd.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gmipwgljf.sHtML

[T01] Kotlin：Hello World
来源：http://wap.epnwcf.com/Article/details/gkelzsuqz.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/gyylytgpe.sHtML

[T02] Kotlin：变量
来源：http://wap.epnwcf.com/Article/details/gpvhxxrvi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.vehdjk.com/Article/details/gbukoerqt.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.vehdjk.com/Article/details/grjlyuzvk.sHtML

"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/gsznjsbeu.sHtML

[T04] Kotlin：空安全
来源：http://read.share.vehdjk.com/Article/details/gojrfqyjb.sHtML

val n: String? = null;  n?.length
来源：http://baike.vehdjk.com/Article/details/giwsswzqs.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.epnwcf.com/Article/details/gwjipmpiy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.bbcook.cn/Article/details/gncaqzgtd.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fktsv.cn/Article/details/gcrttaxzt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gpabesqjv.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/gmdrwdeig.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.epnwcf.com/Article/details/gzzmzsoef.sHtML

[T08] Kotlin：数据类
来源：http://3g.yfazqb.com/Article/details/gybkhkmdo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.tarul.cn/Article/details/gjrdbaipo.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.sjlbkw.cn/Article/details/gvcfouelc.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.vehdjk.com/Article/details/gsztnpeyn.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fktsv.cn/Article/details/glhlqillz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.vehdjk.com/Article/details/gyzcwxnye.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.epnwcf.com/Article/details/glkvukfjs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.tarul.cn/Article/details/gbcniygse.sHtML

[T12] Kotlin：解构声明
来源：http://wap.vehdjk.com/Article/details/gwnzidqgc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.tarul.cn/Article/details/gntrlkyqm.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.epnwcf.com/Article/details/gjxaqzcfs.sHtML

val m = mapOf("a" to 1)
来源：http://wap.bbcook.cn/Article/details/gshoszaef.sHtML

[T14] Kotlin：循环
来源：http://www.share.epnwcf.com/Article/details/gxuhalxmo.sHtML

for (i in 1..10) println(i)
来源：http://m.share.sjlbkw.cn/Article/details/gplrrfnis.sHtML

[T15] Kotlin：接口
来源：http://baike.fktsv.cn/Article/details/gjegyucgm.sHtML

interface Shape { fun area(): Double }
来源：http://wap.yfazqb.com/Article/details/gfcuykzst.sHtML

[T16] Swift：Hello World
来源：http://baike.sjlbkw.cn/Article/details/ggvbmkucq.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/ghgjktwgj.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.bbcook.cn/Article/details/gfhcmwvbx.sHtML

var a = 1;  let b = 2
来源：http://m.share.vehdjk.com/Article/details/gffqvipgk.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gxnzbqdez.sHtML

"值: \(b)"
来源：http://baike.vehdjk.com/Article/details/geptsninp.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.bbcook.cn/Article/details/ghzmehzkq.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.tarul.cn/Article/details/gixlomute.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.yfazqb.com/Article/details/gjvdpwlqh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.vehdjk.com/Article/details/gdunskusi.sHtML

[T21] Swift：遍历
来源：http://www.blog.tarul.cn/Article/details/goknetubr.sHtML

for x in a { print(x) }
来源：http://www.m.share.bbcook.cn/Article/details/gougecfuo.sHtML

[T22] Swift：字典
来源：http://baike.yfazqb.com/Article/details/gzwwsfhnl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.tarul.cn/Article/details/gljpubbjg.sHtML

[T23] Swift：函数
来源：http://read.share.bbcook.cn/Article/details/glfzyzxyj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.bbcook.cn/Article/details/giuiazaen.sHtML

[T24] Swift：闭包
来源：http://wap.yfazqb.com/Article/details/ggtvffnro.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.vehdjk.com/Article/details/gabnzxfco.sHtML

[T25] Swift：结构体
来源：http://wap.vehdjk.com/Article/details/gxxhcdjyj.sHtML

struct P { var x: Int }
来源：http://read.share.vehdjk.com/Article/details/gvidiosuc.sHtML

[T26] Swift：类与重写
来源：http://read.share.vehdjk.com/Article/details/gwtqhxboe.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.epnwcf.com/Article/details/gleyfmjug.sHtML

[T27] Swift：错误处理
来源：http://m.share.vehdjk.com/Article/details/gfzkrvjxa.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.yfazqb.com/Article/details/gjoovdgty.sHtML

[T28] Swift：枚举
来源：http://www.share.bbcook.cn/Article/details/gyoyfhjdc.sHtML

enum Color { case red, green }
来源：http://www.share.vehdjk.com/Article/details/gizisctma.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.yfazqb.com/Article/details/guyejdbkc.sHtML

guard let x = opt else { return }
来源：http://baike.yfazqb.com/Article/details/gqdhrnopj.sHtML

[T30] Swift：协议
来源：http://wap.tarul.cn/Article/details/gvfgzfiow.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.tarul.cn/Article/details/gvpjruasn.sHtML

[T31] Lua：Hello World
来源：http://m.share.tarul.cn/Article/details/gprxpggpp.sHtML

print("Hello")
来源：http://mobile.tarul.cn/Article/details/geyjvlgue.sHtML

[T32] Lua：局部变量
来源：http://mobile.sjlbkw.cn/Article/details/gxmmqmuzt.sHtML

local a = 1
来源：http://www.m.share.fktsv.cn/Article/details/giqstgzda.sHtML

[T33] Lua：表（数组）
来源：http://baike.epnwcf.com/Article/details/ghmwsvdoe.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.epnwcf.com/Article/details/gzvntlhqd.sHtML

[T34] Lua：遍历表
来源：http://www.blog.yfazqb.com/Article/details/gyhizmcjp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.vehdjk.com/Article/details/gpgojbkwc.sHtML

[T35] Lua：字典表
来源：http://baike.yfazqb.com/Article/details/gstxxfyrw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.yfazqb.com/Article/details/gqctrcxpo.sHtML

[T36] Lua：函数
来源：http://www.blog.vehdjk.com/Article/details/gaaawohaq.sHtML

function add(a, b) return a + b end
来源：http://wap.bbcook.cn/Article/details/gxowhgnhx.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.epnwcf.com/Article/details/gvallczlb.sHtML

"a" .. "b"
来源：http://3g.sjlbkw.cn/Article/details/gbewcsrpz.sHtML

[T38] Lua：条件
来源：http://3g.bbcook.cn/Article/details/goccinwfg.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvkjgwdn.sHtML

[T39] Lua：模式匹配
来源：http://baike.fktsv.cn/Article/details/gotnusfod.sHtML

string.find(s, "%d+")
来源：http://m.share.fktsv.cn/Article/details/gjshozwko.sHtML

[T40] Lua：元表
来源：http://blog.fktsv.cn/Article/details/gcqixyhtn.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.tarul.cn/Article/details/gdkomogbs.sHtML

[T41] Perl：Hello World
来源：http://www.share.bbcook.cn/Article/details/gmoaidusf.sHtML

print "Hello\n";
来源：http://wap.bbcook.cn/Article/details/gymsuflbn.sHtML

[T42] Perl：变量类型
来源：http://blog.sjlbkw.cn/Article/details/geafxzneo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fktsv.cn/Article/details/ghxlzxnpo.sHtML

[T43] Perl：字符串插值
来源：http://wap.yfazqb.com/Article/details/gynqikikv.sHtML

"值: $a"
来源：http://3g.tarul.cn/Article/details/gjmbdrgcu.sHtML

[T44] Perl：条件
来源：http://baike.sjlbkw.cn/Article/details/gnkdlfvcf.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.tarul.cn/Article/details/gzeszwlgs.sHtML

[T45] Perl：数组遍历
来源：http://m.share.bbcook.cn/Article/details/gspkpdxwz.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.sjlbkw.cn/Article/details/grmjhoaoh.sHtML

[T46] Perl：哈希操作
来源：http://wap.yfazqb.com/Article/details/gloswzwvj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.bbcook.cn/Article/details/godilqfra.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fktsv.cn/Article/details/gnghdtnpv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.sjlbkw.cn/Article/details/glcwptxnz.sHtML

[T48] Perl：正则替换
来源：http://mobile.bbcook.cn/Article/details/gckgqomfz.sHtML

$s =~ s/old/new/g;
来源：http://m.share.tarul.cn/Article/details/gbyiatvxl.sHtML

[T49] Perl：函数
来源：http://wap.yfazqb.com/Article/details/gkitrajqm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gfcaryjez.sHtML

[T50] Perl：逐行读文件
来源：http://blog.bbcook.cn/Article/details/ghrnjenbx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.epnwcf.com/Article/details/gkheoctej.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.vehdjk.com/Article/details/gzafcpcuz.sHtML

[T51] Scala：Hello World
来源：http://www.share.tarul.cn/Article/details/giaigzagy.sHtML

println("Hello")
来源：http://mobile.epnwcf.com/Article/details/gpfaelzfe.sHtML

[T52] Scala：变量
来源：http://read.share.fktsv.cn/Article/details/giogyptoh.sHtML

val a = 1;  var b = 2
来源：http://mobile.tarul.cn/Article/details/ghzgsthpr.sHtML

[T53] Scala：字符串插值
来源：http://read.share.tarul.cn/Article/details/guqbiyuxu.sHtML

s"值: $b"
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbhxyhle.sHtML

[T54] Scala：集合映射
来源：http://www.share.bbcook.cn/Article/details/gwyuzygvn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.vehdjk.com/Article/details/gzpvgavnp.sHtML

[T55] Scala：集合过滤
来源：http://baike.epnwcf.com/Article/details/gsntmrozg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fktsv.cn/Article/details/gowzkfajj.sHtML

[T56] Scala：样例类
来源：http://baike.vehdjk.com/Article/details/gehvtqmcu.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.epnwcf.com/Article/details/ggoiacfsr.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/gdzyuhtcg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.sjlbkw.cn/Article/details/gyyujvkyk.sHtML

[T58] Scala：函数定义
来源：http://www.blog.bbcook.cn/Article/details/gpnyhtsqb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.epnwcf.com/Article/details/gymtgnoqd.sHtML

[T59] Scala：循环
来源：http://m.share.fktsv.cn/Article/details/geukiuyiy.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.tarul.cn/Article/details/ghvkecrmn.sHtML

[T60] Scala：折叠
来源：http://www.blog.epnwcf.com/Article/details/gaqbkhncm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.tarul.cn/Article/details/glqgshssh.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gkwworkdz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.tarul.cn/Article/details/gspihpcgr.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gihsyyuyv.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fktsv.cn/Article/details/gvviodsje.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fktsv.cn/Article/details/gllwmxqsi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.sjlbkw.cn/Article/details/gvcbnnyff.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.epnwcf.com/Article/details/gimhfdtjt.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.vehdjk.com/Article/details/guiqjjyfc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.epnwcf.com/Article/details/gwcduuygb.sHtML

[U04] Py：变量调试打印
来源：http://m.share.vehdjk.com/Article/details/gvjsvnjvr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.bbcook.cn/Article/details/galxtheja.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fktsv.cn/Article/details/gvvvcxzpc.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.bbcook.cn/Article/details/gauxurqsh.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.tarul.cn/Article/details/gtdndcwdf.sHtML

{**a, **b}
来源：http://read.share.fktsv.cn/Article/details/gviqjvymh.sHtML

[U07] Py：反转字典键值
来源：http://m.share.epnwcf.com/Article/details/gbmiwsmpp.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.sjlbkw.cn/Article/details/glnhlxfyp.sHtML

[U08] Py：展平二维列表
来源：http://blog.tarul.cn/Article/details/ggrwfpxxc.sHtML

[y for x in nested for y in x]
来源：http://mobile.bbcook.cn/Article/details/gfjyohtav.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.sjlbkw.cn/Article/details/ggsfbjtyh.sHtML

max(d, key=d.get)
来源：http://www.blog.epnwcf.com/Article/details/gfkntomek.sHtML

[U10] Py：按值排序字典
来源：http://wap.epnwcf.com/Article/details/gpricvwad.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.epnwcf.com/Article/details/gxgczeams.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.tarul.cn/Article/details/gdglvwstk.sHtML

(x * 2 for x in arr)
来源：http://mobile.yfazqb.com/Article/details/gjsuemunp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.bbcook.cn/Article/details/gnyymptjv.sHtML

Counter(arr).most_common(3)
来源：http://mobile.yfazqb.com/Article/details/gwdgxlazx.sHtML

[U13] Py：固定长度队列
来源：http://blog.yfazqb.com/Article/details/ggswsnyra.sHtML

deque(maxlen=10)
来源：http://blog.sjlbkw.cn/Article/details/gwctippno.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.vehdjk.com/Article/details/gdotbcnxh.sHtML

defaultdict(list)
来源：http://read.share.fktsv.cn/Article/details/gwvzzqnqm.sHtML

[U15] Py：高精度计时
来源：http://mobile.sjlbkw.cn/Article/details/gkfsqhvjq.sHtML

t = time.perf_counter()
来源：http://wap.fktsv.cn/Article/details/gbmsfykaj.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.tarul.cn/Article/details/gaubccnct.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.yfazqb.com/Article/details/ghjrfchds.sHtML

[U17] Py：初始化日志
来源：http://www.share.epnwcf.com/Article/details/gdotcentz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.sjlbkw.cn/Article/details/gkvskmadt.sHtML

[U18] Py：预编译正则
来源：http://blog.sjlbkw.cn/Article/details/geszzhfdq.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/gugnkdrgo.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.tarul.cn/Article/details/gwvzpumty.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.sjlbkw.cn/Article/details/gixupgzzg.sHtML

[U20] Py：缓存函数结果
来源：http://3g.sjlbkw.cn/Article/details/gfwghkocr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fktsv.cn/Article/details/gsihqfutr.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.epnwcf.com/Article/details/gkhcxhmue.sHtML

@contextlib.contextmanager
来源：http://blog.yfazqb.com/Article/details/gmhzuwalg.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.bbcook.cn/Article/details/gdrodasvt.sHtML

list(zip(*m))
来源：http://www.blog.tarul.cn/Article/details/gozunyjun.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.yfazqb.com/Article/details/gxihyohym.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.vehdjk.com/Article/details/gttxqwakf.sHtML

[U24] Py：路径操作
来源：http://mobile.fktsv.cn/Article/details/ginlnigwt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.bbcook.cn/Article/details/gkkpfabon.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.sjlbkw.cn/Article/details/garivjsff.sHtML

csv.DictReader(f)
来源：http://wap.bbcook.cn/Article/details/geywufmwx.sHtML

[U26] Py：并发下载
来源：http://baike.yfazqb.com/Article/details/gfzssjoxd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.tarul.cn/Article/details/gvfdsihcd.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fktsv.cn/Article/details/gkyzecsqk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.sjlbkw.cn/Article/details/gkeddqjtg.sHtML

[U28] Py：类型别名
来源：http://www.share.bbcook.cn/Article/details/ggggmtwbz.sHtML

UserId = int
来源：http://read.share.epnwcf.com/Article/details/ggpuobemw.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fktsv.cn/Article/details/gudgiuuhj.sHtML

@property 与 @x.setter 配合
来源：http://wap.fktsv.cn/Article/details/gaookxrtw.sHtML

[U30] Py：数据类
来源：http://m.share.sjlbkw.cn/Article/details/gbserjoxo.sHtML

@dataclass(slots=True)
来源：http://www.share.tarul.cn/Article/details/gjllmcsmm.sHtML

[U31] Py：单测
来源：http://www.blog.vehdjk.com/Article/details/gnbspspnf.sHtML

python -m pytest -q
来源：http://3g.bbcook.cn/Article/details/gmcqxogww.sHtML

[U32] Py：代码格式化
来源：http://mobile.yfazqb.com/Article/details/giayjmonc.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.epnwcf.com/Article/details/gkzuqbloc.sHtML

[U33] Py：打包发布
来源：http://www.blog.bbcook.cn/Article/details/gvejkmoun.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fktsv.cn/Article/details/ggfdtepyv.sHtML

[U34] Py：判断编码
来源：http://www.share.vehdjk.com/Article/details/gtjqinval.sHtML

chardet.detect(raw)
来源：http://blog.sjlbkw.cn/Article/details/gzpmzwzvs.sHtML

[U35] Py：发送邮件
来源：http://mobile.bbcook.cn/Article/details/gwtzbyhjl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.vehdjk.com/Article/details/gphcoagpa.sHtML

[U36] Py：定时任务
来源：http://baike.fktsv.cn/Article/details/gikfufydk.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.tarul.cn/Article/details/gcldsgbyx.sHtML

[U37] Py：读写 Excel
来源：http://3g.tarul.cn/Article/details/goerslfnp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.epnwcf.com/Article/details/gsgjztnxr.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.yfazqb.com/Article/details/gselwbiwq.sHtML

Path(__file__).resolve().parent
来源：http://blog.vehdjk.com/Article/details/gnqdrivuh.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fktsv.cn/Article/details/gkgvruvrf.sHtML

sys.stdout.isatty()
来源：http://read.share.tarul.cn/Article/details/goxhueciw.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.sjlbkw.cn/Article/details/grzntwzny.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fktsv.cn/Article/details/ggqcsbfbj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.tarul.cn/Article/details/guhxeyqxd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.yfazqb.com/Article/details/gwgjqzmoi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.sjlbkw.cn/Article/details/gmjkwlzqi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.yfazqb.com/Article/details/gxjxdqvfe.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.epnwcf.com/Article/details/gqsrhzkbs.sHtML

namespace App\Http;
来源：http://baike.vehdjk.com/Article/details/gtkozprnv.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.bbcook.cn/Article/details/ginnuzjki.sHtML

declare(strict_types=1);
来源：http://m.share.vehdjk.com/Article/details/gujvhkgoi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.sjlbkw.cn/Article/details/gohlpyrlm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/ghnsvnldn.sHtML

[U46] PHP：可空类型
来源：http://3g.fktsv.cn/Article/details/gnuzckpde.sHtML

?string $name = null
来源：http://wap.vehdjk.com/Article/details/gvaeofkmv.sHtML

[U47] PHP：联合类型
来源：http://read.share.epnwcf.com/Article/details/gewyqjhii.sHtML

int|string $id
来源：http://www.blog.sjlbkw.cn/Article/details/gafasbfrj.sHtML

[U48] PHP：纯枚举
来源：http://wap.fktsv.cn/Article/details/gmlzbpvmo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.epnwcf.com/Article/details/gggxoczqo.sHtML

[U49] PHP：只读属性
来源：http://3g.bbcook.cn/Article/details/gyrubfvqm.sHtML

public readonly string $name
来源：http://www.blog.bbcook.cn/Article/details/gjzlubfpv.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.sjlbkw.cn/Article/details/gqhdujhjv.sHtML

public function __construct(private int $id) {}
来源：http://read.share.yfazqb.com/Article/details/gaqxiaxyy.sHtML

[U51] PHP：数组解构
来源：http://www.share.bbcook.cn/Article/details/gexpapnal.sHtML

[$a, $b] = $arr;
来源：http://blog.vehdjk.com/Article/details/gszhgfzfj.sHtML

[U52] PHP：箭头函数
来源：http://read.share.tarul.cn/Article/details/gvegqcqhw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.sjlbkw.cn/Article/details/gzlgmqmtf.sHtML

[U53] PHP：空合并运算符
来源：http://3g.bbcook.cn/Article/details/ggzuhpkgi.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.yfazqb.com/Article/details/gzjnpisek.sHtML

[U54] PHP：空安全调用
来源：http://read.share.bbcook.cn/Article/details/gjgbvmxrm.sHtML

$obj?->method()
来源：http://mobile.vehdjk.com/Article/details/gvzsvgafg.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.vehdjk.com/Article/details/gxzcopile.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.tarul.cn/Article/details/gugstzhnx.sHtML

[U56] PHP：命名参数
来源：http://www.share.fktsv.cn/Article/details/gndoeszgx.sHtML

f(a: 1, b: 2)
来源：http://mobile.sjlbkw.cn/Article/details/gdzwcerdc.sHtML

[U57] PHP：字符串插值
来源：http://read.share.tarul.cn/Article/details/ggzpgwiuk.sHtML

"值: {$a}"
来源：http://www.m.share.tarul.cn/Article/details/gunwpdwjl.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fktsv.cn/Article/details/ggoitmpdr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.bbcook.cn/Article/details/gznwiacdn.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.tarul.cn/Article/details/gjqymuxsi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.epnwcf.com/Article/details/ghkxvuzne.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.vehdjk.com/Article/details/ghlzgyyjy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.epnwcf.com/Article/details/gtvtfwygo.sHtML

[U61] PHP：正则
来源：http://3g.bbcook.cn/Article/details/ghwsgqmjc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.yfazqb.com/Article/details/gubhruzct.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.bbcook.cn/Article/details/gghahkzwe.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.epnwcf.com/Article/details/gkqnflmhh.sHtML

[U63] PHP：文件读写
来源：http://wap.yfazqb.com/Article/details/glqcbzzdv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.bbcook.cn/Article/details/guslaaksl.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fktsv.cn/Article/details/gguylgghz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.vehdjk.com/Article/details/gjwvpmbhc.sHtML

[U65] PHP：会话
来源：http://www.share.epnwcf.com/Article/details/ggcbncesn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.bbcook.cn/Article/details/gelkhmsxc.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.yfazqb.com/Article/details/gdijhdgqu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.sjlbkw.cn/Article/details/gzkgzjyqn.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.vehdjk.com/Article/details/gbzibpmvw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fktsv.cn/Article/details/gsyfsflgq.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.vehdjk.com/Article/details/gatfoxvpb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.vehdjk.com/Article/details/gphmjowws.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.tarul.cn/Article/details/gqynwcaax.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.tarul.cn/Article/details/gmipqbcda.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.sjlbkw.cn/Article/details/gfbgwhjlc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.sjlbkw.cn/Article/details/gqemgpdga.sHtML

[U71] PHP：抛出异常
来源：http://m.share.vehdjk.com/Article/details/gmwdglvfj.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.yfazqb.com/Article/details/gcmuuiqes.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.sjlbkw.cn/Article/details/goiryweev.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.epnwcf.com/Article/details/gmptgcsqx.sHtML


<!-- 参考信息 -->