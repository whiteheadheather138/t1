代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gymahkamq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.yfazqb.com/Article/details/gnxlitzwe.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/ghdeiusmk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.vehdjk.com/Article/details/gsrhhdguo.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.yfazqb.com/Article/details/gkjrjkmtt.sHtML

[S49] C++：写文件
来源：http://mobile.yfazqb.com/Article/details/grdsfiqck.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.tarul.cn/Article/details/giryfygnb.sHtML

[S50] C++：格式化数字
来源：http://read.share.bbcook.cn/Article/details/gbzueumhk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gsehymsqq.sHtML

[S51] C++：显式类型转换
来源：http://m.share.yfazqb.com/Article/details/ggfdzigcf.sHtML

static_cast<double>(a) / b
来源：http://blog.fktsv.cn/Article/details/gcgagrgmw.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fktsv.cn/Article/details/gqtbulrmx.sHtML

int size() const noexcept { return n_; }
来源：http://3g.bbcook.cn/Article/details/gkdplkyko.sHtML

[S53] C++：移动语义
来源：http://www.m.share.yfazqb.com/Article/details/glzrwdmur.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.bbcook.cn/Article/details/gubvouket.sHtML

[S54] C++：异常处理
来源：http://read.share.bbcook.cn/Article/details/gyvwgkmew.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.bbcook.cn/Article/details/gzkncoohu.sHtML

[S55] C++：结构化绑定
来源：http://baike.tarul.cn/Article/details/gewpohapa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.bbcook.cn/Article/details/glhyeypdi.sHtML

[S56] C++：optional
来源：http://www.share.tarul.cn/Article/details/grkztnqcb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.epnwcf.com/Article/details/glpgdglhi.sHtML

[S57] C++：编译期常量
来源：http://blog.epnwcf.com/Article/details/gatzrsuxq.sHtML

constexpr int N = 10;
来源：http://www.blog.fktsv.cn/Article/details/gzzuffbny.sHtML

[S58] C++：命名空间
来源：http://blog.epnwcf.com/Article/details/ghwtaexea.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.epnwcf.com/Article/details/gznyimkcm.sHtML

[S59] C++：静态断言
来源：http://baike.tarul.cn/Article/details/gjaarhjna.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.bbcook.cn/Article/details/ggmrlvjdf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwfamnyu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fktsv.cn/Article/details/gxxpklrkw.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gnphfywbn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.sjlbkw.cn/Article/details/gqjecwkvw.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gwzfjtzxg.sHtML

[T01] Kotlin：Hello World
来源：http://wap.sjlbkw.cn/Article/details/guklgmssi.sHtML

println("Hello")
来源：http://blog.vehdjk.com/Article/details/gpvzikcgx.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.yfazqb.com/Article/details/gwkqfmipi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.epnwcf.com/Article/details/gqlejvubt.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.tarul.cn/Article/details/gjfkwkwze.sHtML

"值: $b"
来源：http://mobile.epnwcf.com/Article/details/gevdotcsg.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjavvarb.sHtML

val n: String? = null;  n?.length
来源：http://baike.sjlbkw.cn/Article/details/gfoubipgw.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.tarul.cn/Article/details/gdnxuysoq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.epnwcf.com/Article/details/ghltpiayd.sHtML

[T06] Kotlin：集合映射
来源：http://blog.tarul.cn/Article/details/gciltwezc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.epnwcf.com/Article/details/ghxxikwcf.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fktsv.cn/Article/details/gffnicbpx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.epnwcf.com/Article/details/guvgegnpv.sHtML

[T08] Kotlin：数据类
来源：http://read.share.bbcook.cn/Article/details/gkqlppmqj.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.vehdjk.com/Article/details/gwrdaummt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.sjlbkw.cn/Article/details/gkkmfzftk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.tarul.cn/Article/details/gzcktxtvu.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.yfazqb.com/Article/details/gmvqncbhj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.vehdjk.com/Article/details/gzunckgfv.sHtML

[T11] Kotlin：协程
来源：http://read.share.bbcook.cn/Article/details/gxxqybtdn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.epnwcf.com/Article/details/gytffotmt.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.sjlbkw.cn/Article/details/gobfgsqho.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gynnznhwk.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.epnwcf.com/Article/details/gqnuvrxvk.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.bbcook.cn/Article/details/gmoscevnt.sHtML

[T14] Kotlin：循环
来源：http://baike.yfazqb.com/Article/details/gahmdbyic.sHtML

for (i in 1..10) println(i)
来源：http://baike.sjlbkw.cn/Article/details/gsrtigigm.sHtML

[T15] Kotlin：接口
来源：http://baike.vehdjk.com/Article/details/grxcfncyd.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.sjlbkw.cn/Article/details/gejezclle.sHtML

[T16] Swift：Hello World
来源：http://m.share.tarul.cn/Article/details/gdhnztqrd.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gxxeqmrgm.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fktsv.cn/Article/details/gcorxnacc.sHtML

var a = 1;  let b = 2
来源：http://3g.bbcook.cn/Article/details/grwfdzgzo.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.tarul.cn/Article/details/ggrgupnip.sHtML

"值: \(b)"
来源：http://3g.yfazqb.com/Article/details/gjxbdiyqw.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fktsv.cn/Article/details/gmmovmahn.sHtML

if let n = opt { print(n) }
来源：http://wap.sjlbkw.cn/Article/details/ggirkjwcv.sHtML

[T20] Swift：数组操作
来源：http://mobile.epnwcf.com/Article/details/gqsvujztr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.sjlbkw.cn/Article/details/gujptwzjj.sHtML

[T21] Swift：遍历
来源：http://m.share.yfazqb.com/Article/details/gugedwbrh.sHtML

for x in a { print(x) }
来源：http://baike.fktsv.cn/Article/details/gvodndtqy.sHtML

[T22] Swift：字典
来源：http://www.m.share.bbcook.cn/Article/details/glgllzktb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.vehdjk.com/Article/details/grxuvnbej.sHtML

[T23] Swift：函数
来源：http://read.share.sjlbkw.cn/Article/details/glupszkqs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.yfazqb.com/Article/details/gsdkwaoen.sHtML

[T24] Swift：闭包
来源：http://www.share.sjlbkw.cn/Article/details/gmfbdbktq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/grkofvkyw.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fktsv.cn/Article/details/gygtufurd.sHtML

struct P { var x: Int }
来源：http://blog.yfazqb.com/Article/details/gmphynfjl.sHtML

[T26] Swift：类与重写
来源：http://www.share.epnwcf.com/Article/details/ggtonvtcx.sHtML

class A: Base { override func f() {} }
来源：http://wap.tarul.cn/Article/details/grmxozqom.sHtML

[T27] Swift：错误处理
来源：http://read.share.vehdjk.com/Article/details/gktyughvd.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.epnwcf.com/Article/details/gxlopibnh.sHtML

[T28] Swift：枚举
来源：http://blog.epnwcf.com/Article/details/gmapzhjkn.sHtML

enum Color { case red, green }
来源：http://www.blog.fktsv.cn/Article/details/gteqzwibt.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.tarul.cn/Article/details/gxvaxhudz.sHtML

guard let x = opt else { return }
来源：http://www.m.share.epnwcf.com/Article/details/gxgxafssi.sHtML

[T30] Swift：协议
来源：http://wap.bbcook.cn/Article/details/gimlmcgew.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.tarul.cn/Article/details/gfkcemwjn.sHtML

[T31] Lua：Hello World
来源：http://baike.bbcook.cn/Article/details/gmhbmnxyy.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gshowkygf.sHtML

[T32] Lua：局部变量
来源：http://baike.vehdjk.com/Article/details/gniykcjzq.sHtML

local a = 1
来源：http://www.share.tarul.cn/Article/details/gjheeroya.sHtML

[T33] Lua：表（数组）
来源：http://3g.vehdjk.com/Article/details/gapzprdap.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.epnwcf.com/Article/details/gaxwnvuhu.sHtML

[T34] Lua：遍历表
来源：http://baike.epnwcf.com/Article/details/goihjktlg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.yfazqb.com/Article/details/gexsyadyc.sHtML

[T35] Lua：字典表
来源：http://baike.yfazqb.com/Article/details/gsvoknnge.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gxucosmmb.sHtML

[T36] Lua：函数
来源：http://wap.epnwcf.com/Article/details/gzaizfncl.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.vehdjk.com/Article/details/gqfitlvxm.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.yfazqb.com/Article/details/gboxqexai.sHtML

"a" .. "b"
来源：http://mobile.fktsv.cn/Article/details/gbhjzuhfb.sHtML

[T38] Lua：条件
来源：http://blog.fktsv.cn/Article/details/gztqjislp.sHtML

if x > 0 then print("正") end
来源：http://3g.vehdjk.com/Article/details/gemsomlfx.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gygcjjmer.sHtML

string.find(s, "%d+")
来源：http://www.share.tarul.cn/Article/details/gaaygqbdx.sHtML

[T40] Lua：元表
来源：http://read.share.sjlbkw.cn/Article/details/gwufwdczu.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.bbcook.cn/Article/details/gvhcsvckx.sHtML

[T41] Perl：Hello World
来源：http://m.share.yfazqb.com/Article/details/gwqjcgdrv.sHtML

print "Hello\n";
来源：http://wap.epnwcf.com/Article/details/gcsdoorer.sHtML

[T42] Perl：变量类型
来源：http://baike.vehdjk.com/Article/details/gdwymutop.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.yfazqb.com/Article/details/gmfpxmvmy.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gjsjilfvu.sHtML

"值: $a"
来源：http://wap.sjlbkw.cn/Article/details/gmajkwwao.sHtML

[T44] Perl：条件
来源：http://www.m.share.sjlbkw.cn/Article/details/grlxgnhzj.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.bbcook.cn/Article/details/gedtvmlse.sHtML

[T45] Perl：数组遍历
来源：http://www.share.vehdjk.com/Article/details/gxraupuia.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.tarul.cn/Article/details/givlbdeef.sHtML

[T46] Perl：哈希操作
来源：http://baike.sjlbkw.cn/Article/details/gggehjwob.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.yfazqb.com/Article/details/gkalfmloi.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.epnwcf.com/Article/details/gwrsgbgvx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fktsv.cn/Article/details/golhzmyle.sHtML

[T48] Perl：正则替换
来源：http://wap.sjlbkw.cn/Article/details/grrguupah.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.tarul.cn/Article/details/gsbmtztgx.sHtML

[T49] Perl：函数
来源：http://read.share.fktsv.cn/Article/details/guxwzgdvk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gflpxsboy.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gtdqjwabx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.epnwcf.com/Article/details/gurdfgruz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.epnwcf.com/Article/details/gtktipfjb.sHtML

[T51] Scala：Hello World
来源：http://3g.tarul.cn/Article/details/gemkjvamj.sHtML

println("Hello")
来源：http://wap.epnwcf.com/Article/details/gjkbtyzcw.sHtML

[T52] Scala：变量
来源：http://3g.fktsv.cn/Article/details/gfzsdnlkw.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.vehdjk.com/Article/details/gufbnkxoe.sHtML

[T53] Scala：字符串插值
来源：http://m.share.vehdjk.com/Article/details/gryonmlsm.sHtML

s"值: $b"
来源：http://www.share.yfazqb.com/Article/details/giipmtrps.sHtML

[T54] Scala：集合映射
来源：http://baike.fktsv.cn/Article/details/gsodtngkn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.tarul.cn/Article/details/gqdmhlwnd.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fktsv.cn/Article/details/gqbypbaaz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.vehdjk.com/Article/details/gqtoddvoe.sHtML

[T56] Scala：样例类
来源：http://read.share.bbcook.cn/Article/details/gmcypfxyz.sHtML

case class User(name: String, age: Int)
来源：http://m.share.sjlbkw.cn/Article/details/gzibmkqbw.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gnngozbeu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.bbcook.cn/Article/details/gqyjpsomr.sHtML

[T58] Scala：函数定义
来源：http://www.share.yfazqb.com/Article/details/gnjvcxinm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.sjlbkw.cn/Article/details/goydqtkbe.sHtML

[T59] Scala：循环
来源：http://www.share.tarul.cn/Article/details/gicbwnnqp.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.bbcook.cn/Article/details/gahikoyoo.sHtML

[T60] Scala：折叠
来源：http://baike.vehdjk.com/Article/details/gnanysqze.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fktsv.cn/Article/details/gcrjniynz.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gpyjdlnou.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.vehdjk.com/Article/details/gtfsbblnd.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gmmyvbczw.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.tarul.cn/Article/details/grtbpfimz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.tarul.cn/Article/details/ghplkowdk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.epnwcf.com/Article/details/gytlinxcq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.bbcook.cn/Article/details/gishphdhy.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.sjlbkw.cn/Article/details/gblbzzust.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.sjlbkw.cn/Article/details/gluohrpxe.sHtML

[U04] Py：变量调试打印
来源：http://m.share.tarul.cn/Article/details/gkmzobprm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.vehdjk.com/Article/details/gjkogldql.sHtML

[U05] Py：列表去重且保序
来源：http://3g.tarul.cn/Article/details/gytbjwvbg.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.yfazqb.com/Article/details/gwqguqxsz.sHtML

[U06] Py：合并两个字典
来源：http://mobile.vehdjk.com/Article/details/gyowytnuy.sHtML

{**a, **b}
来源：http://wap.epnwcf.com/Article/details/gzeikhnzb.sHtML

[U07] Py：反转字典键值
来源：http://read.share.bbcook.cn/Article/details/gkarqszvh.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fktsv.cn/Article/details/gzjdvafxt.sHtML

[U08] Py：展平二维列表
来源：http://baike.epnwcf.com/Article/details/gnkpasgtg.sHtML

[y for x in nested for y in x]
来源：http://baike.epnwcf.com/Article/details/gufcxdubk.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.vehdjk.com/Article/details/gihrezqnw.sHtML

max(d, key=d.get)
来源：http://www.m.share.yfazqb.com/Article/details/gttwtprzp.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.bbcook.cn/Article/details/gkupdnguj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.tarul.cn/Article/details/gfeslsnlk.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.yfazqb.com/Article/details/gsluahvwa.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fktsv.cn/Article/details/gvbvvazmh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.yfazqb.com/Article/details/gusjgsxbd.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fktsv.cn/Article/details/gayffxvvz.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.yfazqb.com/Article/details/ggwicgkhd.sHtML

deque(maxlen=10)
来源：http://baike.vehdjk.com/Article/details/gdzleszan.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fktsv.cn/Article/details/gyexennzj.sHtML

defaultdict(list)
来源：http://m.share.fktsv.cn/Article/details/gdddsghse.sHtML

[U15] Py：高精度计时
来源：http://3g.yfazqb.com/Article/details/gttgwfnua.sHtML

t = time.perf_counter()
来源：http://www.share.epnwcf.com/Article/details/geymzbpxh.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fktsv.cn/Article/details/gqvjvigch.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.sjlbkw.cn/Article/details/gzebadyxv.sHtML

[U17] Py：初始化日志
来源：http://m.share.vehdjk.com/Article/details/gcqekydrr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fktsv.cn/Article/details/glqwkigpn.sHtML

[U18] Py：预编译正则
来源：http://read.share.epnwcf.com/Article/details/gcpprcvfd.sHtML

pat = re.compile(r"\d+")
来源：http://3g.yfazqb.com/Article/details/ggeqztmjm.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fktsv.cn/Article/details/gjgcleocf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.bbcook.cn/Article/details/geicaxbqp.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fktsv.cn/Article/details/gvhpqrdqy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghiuyxqhq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.epnwcf.com/Article/details/gthuqcamp.sHtML

@contextlib.contextmanager
来源：http://wap.tarul.cn/Article/details/goecshalj.sHtML

[U22] Py：矩阵转置
来源：http://blog.sjlbkw.cn/Article/details/ghxooadmv.sHtML

list(zip(*m))
来源：http://www.blog.yfazqb.com/Article/details/gzomlxtol.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fktsv.cn/Article/details/gbpysyqol.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fktsv.cn/Article/details/gmdywjxkl.sHtML

[U24] Py：路径操作
来源：http://m.share.yfazqb.com/Article/details/gjdyopqfw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.bbcook.cn/Article/details/gpbawvauf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.epnwcf.com/Article/details/gihoebwrz.sHtML

csv.DictReader(f)
来源：http://www.blog.epnwcf.com/Article/details/gfrbphhdu.sHtML

[U26] Py：并发下载
来源：http://www.blog.vehdjk.com/Article/details/gmrbyauhj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.yfazqb.com/Article/details/gpklxprvb.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.epnwcf.com/Article/details/glzeucnyo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.bbcook.cn/Article/details/ggkdeyzfb.sHtML

[U28] Py：类型别名
来源：http://www.m.share.vehdjk.com/Article/details/gyumfgvoh.sHtML

UserId = int
来源：http://baike.fktsv.cn/Article/details/gbifvbble.sHtML

[U29] Py：属性校验
来源：http://www.blog.epnwcf.com/Article/details/gnnyqcgkb.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fktsv.cn/Article/details/gogsazqry.sHtML

[U30] Py：数据类
来源：http://3g.epnwcf.com/Article/details/ggumwysqm.sHtML

@dataclass(slots=True)
来源：http://www.m.share.tarul.cn/Article/details/gdipxgxat.sHtML

[U31] Py：单测
来源：http://www.m.share.tarul.cn/Article/details/gwdbnnzor.sHtML

python -m pytest -q
来源：http://mobile.epnwcf.com/Article/details/gubgkcpbs.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.vehdjk.com/Article/details/gmfsmapop.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.tarul.cn/Article/details/geyhfibvb.sHtML

[U33] Py：打包发布
来源：http://www.share.vehdjk.com/Article/details/gfoqqmwut.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.sjlbkw.cn/Article/details/gxytgpwui.sHtML

[U34] Py：判断编码
来源：http://blog.yfazqb.com/Article/details/gehptwnbc.sHtML

chardet.detect(raw)
来源：http://mobile.vehdjk.com/Article/details/goumfxegq.sHtML

[U35] Py：发送邮件
来源：http://www.share.bbcook.cn/Article/details/gjwcdofuq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.tarul.cn/Article/details/gadkjmgjm.sHtML

[U36] Py：定时任务
来源：http://baike.epnwcf.com/Article/details/gzschltxb.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.vehdjk.com/Article/details/ghldnieje.sHtML

[U37] Py：读写 Excel
来源：http://mobile.vehdjk.com/Article/details/grmbejfuu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fktsv.cn/Article/details/gyrlytbhy.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.tarul.cn/Article/details/gmkzqmtca.sHtML

Path(__file__).resolve().parent
来源：http://mobile.bbcook.cn/Article/details/gvmujqosz.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.sjlbkw.cn/Article/details/gscojvspb.sHtML

sys.stdout.isatty()
来源：http://baike.fktsv.cn/Article/details/gjesmagse.sHtML

[U40] Py：打印到标准错误
来源：http://baike.bbcook.cn/Article/details/givsxbmog.sHtML

print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gxjpxbwyp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.bbcook.cn/Article/details/gjpmbzgzn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.yfazqb.com/Article/details/gdeedkqcw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.tarul.cn/Article/details/gqyhlwvfd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.sjlbkw.cn/Article/details/gxoqkvpvi.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.epnwcf.com/Article/details/guapdasqt.sHtML

namespace App\Http;
来源：http://mobile.fktsv.cn/Article/details/gtbbalpfk.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.tarul.cn/Article/details/gcsfvqluj.sHtML

declare(strict_types=1);
来源：http://blog.vehdjk.com/Article/details/gmzyqugzi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.epnwcf.com/Article/details/gkonfkisn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/gsvhxyryi.sHtML

[U46] PHP：可空类型
来源：http://read.share.fktsv.cn/Article/details/gctddksjf.sHtML

?string $name = null
来源：http://read.share.bbcook.cn/Article/details/gkconvanm.sHtML

[U47] PHP：联合类型
来源：http://m.share.bbcook.cn/Article/details/gxinbjyzt.sHtML

int|string $id
来源：http://read.share.bbcook.cn/Article/details/gdatyofrq.sHtML

[U48] PHP：纯枚举
来源：http://read.share.tarul.cn/Article/details/gvhhjimao.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.yfazqb.com/Article/details/gqbpcpodt.sHtML

[U49] PHP：只读属性
来源：http://read.share.yfazqb.com/Article/details/gsnfvrhxd.sHtML

public readonly string $name
来源：http://www.m.share.bbcook.cn/Article/details/gkhknecyq.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.sjlbkw.cn/Article/details/gmlkilfbv.sHtML

public function __construct(private int $id) {}
来源：http://www.share.tarul.cn/Article/details/gcymjczmp.sHtML

[U51] PHP：数组解构
来源：http://3g.epnwcf.com/Article/details/gpaojtjrz.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.vehdjk.com/Article/details/gtiqqnmtq.sHtML

[U52] PHP：箭头函数
来源：http://3g.epnwcf.com/Article/details/geawsqlbl.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.sjlbkw.cn/Article/details/ggqxltgbk.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.bbcook.cn/Article/details/gndgapsgr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.epnwcf.com/Article/details/guccwrrky.sHtML

[U54] PHP：空安全调用
来源：http://wap.tarul.cn/Article/details/gmnszxcxw.sHtML

$obj?->method()
来源：http://www.share.tarul.cn/Article/details/grmjnumgj.sHtML

[U55] PHP：match 表达式
来源：http://www.share.epnwcf.com/Article/details/gwqrydqil.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.epnwcf.com/Article/details/gqzcdrtpi.sHtML

[U56] PHP：命名参数
来源：http://3g.vehdjk.com/Article/details/goyklmejg.sHtML

f(a: 1, b: 2)
来源：http://www.share.epnwcf.com/Article/details/gzqsvpwqx.sHtML

[U57] PHP：字符串插值
来源：http://blog.fktsv.cn/Article/details/gbjhwuccu.sHtML

"值: {$a}"
来源：http://mobile.sjlbkw.cn/Article/details/gnlrswcih.sHtML

[U58] PHP：数组三件套
来源：http://www.share.yfazqb.com/Article/details/gjitracik.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.tarul.cn/Article/details/gwyokvsgw.sHtML

[U59] PHP：自定义排序
来源：http://mobile.bbcook.cn/Article/details/ggxydmlbf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.tarul.cn/Article/details/gzigoqhjf.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fktsv.cn/Article/details/gqmnzpdbu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.sjlbkw.cn/Article/details/gvahagbpo.sHtML

[U61] PHP：正则
来源：http://m.share.fktsv.cn/Article/details/geaebudzo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fktsv.cn/Article/details/ggiarkezg.sHtML

[U62] PHP：日期对象
来源：http://mobile.tarul.cn/Article/details/gpkzltgge.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.epnwcf.com/Article/details/gnlpnrtrv.sHtML

[U63] PHP：文件读写
来源：http://mobile.epnwcf.com/Article/details/gmjbfdepy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.epnwcf.com/Article/details/ghuvdheru.sHtML

[U64] PHP：目录遍历
来源：http://www.share.vehdjk.com/Article/details/gmsuajqrf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.bbcook.cn/Article/details/gipmdmzwf.sHtML

[U65] PHP：会话
来源：http://mobile.sjlbkw.cn/Article/details/ggilncdmn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gaghvsryj.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.sjlbkw.cn/Article/details/grapvgcxl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.epnwcf.com/Article/details/gqrsvmlxg.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.vehdjk.com/Article/details/geznyhzgo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.vehdjk.com/Article/details/gbzgqityy.sHtML

[U68] PHP：PDO 连接
来源：http://3g.bbcook.cn/Article/details/goyngrrit.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fktsv.cn/Article/details/gnizdixqa.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrtsapqz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.bbcook.cn/Article/details/gnbzmeadu.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fktsv.cn/Article/details/gyoyoaldu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.yfazqb.com/Article/details/gvtdyaoqw.sHtML

[U71] PHP：抛出异常
来源：http://wap.yfazqb.com/Article/details/ggatvtspc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.vehdjk.com/Article/details/gygjnjttl.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.epnwcf.com/Article/details/gummulink.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.vehdjk.com/Article/details/gujkvtwpt.sHtML


<!-- 参考信息 -->