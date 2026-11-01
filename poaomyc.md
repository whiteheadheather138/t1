代发 wailian999

while (std::getline(in, line)) { }
来源：http://3g.sjlbkw.cn/Article/details/gczdpldod.sHtML

[S49] C++：写文件
来源：http://www.share.vehdjk.com/Article/details/gpgmuxqiz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.sjlbkw.cn/Article/details/giuykqcuw.sHtML

[S50] C++：格式化数字
来源：http://blog.vehdjk.com/Article/details/gkxxkspks.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.vehdjk.com/Article/details/gdopscqxf.sHtML

[S51] C++：显式类型转换
来源：http://mobile.yfazqb.com/Article/details/gwbzjzxok.sHtML

static_cast<double>(a) / b
来源：http://read.share.tarul.cn/Article/details/gbpevtwls.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.tarul.cn/Article/details/gkwvgguhz.sHtML

int size() const noexcept { return n_; }
来源：http://wap.yfazqb.com/Article/details/gxjxmeqnv.sHtML

[S53] C++：移动语义
来源：http://blog.sjlbkw.cn/Article/details/gwtmnqgvy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.epnwcf.com/Article/details/gypectetk.sHtML

[S54] C++：异常处理
来源：http://wap.vehdjk.com/Article/details/ggywvupoi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.epnwcf.com/Article/details/gwdnqjkow.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.bbcook.cn/Article/details/glnlkoxjo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fktsv.cn/Article/details/gnqdfgoug.sHtML

[S56] C++：optional
来源：http://m.share.bbcook.cn/Article/details/gnsbfhwyv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.sjlbkw.cn/Article/details/gneqjndth.sHtML

[S57] C++：编译期常量
来源：http://3g.vehdjk.com/Article/details/gwpccalsk.sHtML

constexpr int N = 10;
来源：http://www.share.yfazqb.com/Article/details/gpkncxtff.sHtML

[S58] C++：命名空间
来源：http://www.blog.vehdjk.com/Article/details/gmzivnqpr.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.yfazqb.com/Article/details/glovcslpn.sHtML

[S59] C++：静态断言
来源：http://www.share.epnwcf.com/Article/details/gxqgidqpj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbmqhsas.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.yfazqb.com/Article/details/glmmawkoa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.vehdjk.com/Article/details/gkwzeqjdh.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gvxtqwduh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.epnwcf.com/Article/details/gpicxoveo.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gnhbdziqo.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/geqdthddu.sHtML

println("Hello")
来源：http://mobile.epnwcf.com/Article/details/gfszjzcbj.sHtML

[T02] Kotlin：变量
来源：http://baike.sjlbkw.cn/Article/details/gxduyucoq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.epnwcf.com/Article/details/gcbgvxexr.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.bbcook.cn/Article/details/ggkhvwlni.sHtML

"值: $b"
来源：http://mobile.tarul.cn/Article/details/ghxmfwpdb.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fktsv.cn/Article/details/gewujciil.sHtML

val n: String? = null;  n?.length
来源：http://wap.bbcook.cn/Article/details/gygpzqdxg.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.yfazqb.com/Article/details/gbblxqydy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fktsv.cn/Article/details/gzauetrfi.sHtML

[T06] Kotlin：集合映射
来源：http://blog.vehdjk.com/Article/details/guryqwozb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/ggxrsdqjj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.vehdjk.com/Article/details/gdbllbgmj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.bbcook.cn/Article/details/gchfxxnzk.sHtML

[T08] Kotlin：数据类
来源：http://mobile.yfazqb.com/Article/details/gjjdhsaxh.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.bbcook.cn/Article/details/giywkpyzw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.vehdjk.com/Article/details/goekvwibu.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.epnwcf.com/Article/details/gjnqwhtgx.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.yfazqb.com/Article/details/gpmdllbva.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.vehdjk.com/Article/details/gswyodxck.sHtML

[T11] Kotlin：协程
来源：http://blog.bbcook.cn/Article/details/gxninxmes.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.sjlbkw.cn/Article/details/galopimqu.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.bbcook.cn/Article/details/gnqryxpep.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gdbrbrdih.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.tarul.cn/Article/details/gjlkkydew.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.epnwcf.com/Article/details/gokzgrjhf.sHtML

[T14] Kotlin：循环
来源：http://baike.yfazqb.com/Article/details/gljqvnrac.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/guxuoywbd.sHtML

[T15] Kotlin：接口
来源：http://3g.yfazqb.com/Article/details/gssferrmi.sHtML

interface Shape { fun area(): Double }
来源：http://3g.yfazqb.com/Article/details/gmbfsvbtx.sHtML

[T16] Swift：Hello World
来源：http://www.share.bbcook.cn/Article/details/gjixphfrm.sHtML

print("Hello")
来源：http://m.share.vehdjk.com/Article/details/gigdzzmfi.sHtML

[T17] Swift：变量与常量
来源：http://wap.epnwcf.com/Article/details/grvmwfdrj.sHtML

var a = 1;  let b = 2
来源：http://www.share.tarul.cn/Article/details/ghzlyosvg.sHtML

[T18] Swift：字符串插值
来源：http://wap.tarul.cn/Article/details/gfbochwnt.sHtML

"值: \(b)"
来源：http://blog.yfazqb.com/Article/details/gleeisxcq.sHtML

[T19] Swift：可选绑定
来源：http://wap.vehdjk.com/Article/details/gxkblqxso.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fktsv.cn/Article/details/ghsvjjktc.sHtML

[T20] Swift：数组操作
来源：http://www.blog.sjlbkw.cn/Article/details/gaxehnnec.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.bbcook.cn/Article/details/gfanntqlx.sHtML

[T21] Swift：遍历
来源：http://www.share.sjlbkw.cn/Article/details/giplpyxtu.sHtML

for x in a { print(x) }
来源：http://www.m.share.epnwcf.com/Article/details/gapabyqne.sHtML

[T22] Swift：字典
来源：http://m.share.sjlbkw.cn/Article/details/gurajcopj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.epnwcf.com/Article/details/gxzapoavq.sHtML

[T23] Swift：函数
来源：http://baike.fktsv.cn/Article/details/gpenylbvs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.sjlbkw.cn/Article/details/ggwnifiig.sHtML

[T24] Swift：闭包
来源：http://www.blog.bbcook.cn/Article/details/gfdiisfwh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.yfazqb.com/Article/details/gtaumftvl.sHtML

[T25] Swift：结构体
来源：http://3g.fktsv.cn/Article/details/ggroavkvr.sHtML

struct P { var x: Int }
来源：http://wap.vehdjk.com/Article/details/gsxellbpn.sHtML

[T26] Swift：类与重写
来源：http://www.share.bbcook.cn/Article/details/ghaslpjdq.sHtML

class A: Base { override func f() {} }
来源：http://3g.vehdjk.com/Article/details/gztpjbkbi.sHtML

[T27] Swift：错误处理
来源：http://3g.epnwcf.com/Article/details/gnqraminz.sHtML

do { try f() } catch { print(error) }
来源：http://blog.yfazqb.com/Article/details/gmrwjiriy.sHtML

[T28] Swift：枚举
来源：http://www.share.fktsv.cn/Article/details/gkkjloiir.sHtML

enum Color { case red, green }
来源：http://wap.vehdjk.com/Article/details/golnwzyvx.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.yfazqb.com/Article/details/gdgsjujtu.sHtML

guard let x = opt else { return }
来源：http://www.share.fktsv.cn/Article/details/gyegggdwy.sHtML

[T30] Swift：协议
来源：http://www.m.share.fktsv.cn/Article/details/gbzdgcpij.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.tarul.cn/Article/details/ggewjazzg.sHtML

[T31] Lua：Hello World
来源：http://mobile.epnwcf.com/Article/details/gcrwgwcdm.sHtML

print("Hello")
来源：http://m.share.yfazqb.com/Article/details/glhdjddfu.sHtML

[T32] Lua：局部变量
来源：http://www.share.fktsv.cn/Article/details/gnwqbrkuu.sHtML

local a = 1
来源：http://wap.fktsv.cn/Article/details/gpyptgncp.sHtML

[T33] Lua：表（数组）
来源：http://baike.epnwcf.com/Article/details/gjphhajdu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.sjlbkw.cn/Article/details/giojmklkn.sHtML

[T34] Lua：遍历表
来源：http://read.share.fktsv.cn/Article/details/gmrjmveix.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.yfazqb.com/Article/details/ghgyacyox.sHtML

[T35] Lua：字典表
来源：http://read.share.vehdjk.com/Article/details/gdgsgsztf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.epnwcf.com/Article/details/gpxdtvbqt.sHtML

[T36] Lua：函数
来源：http://www.blog.vehdjk.com/Article/details/ggmffkgrh.sHtML

function add(a, b) return a + b end
来源：http://mobile.vehdjk.com/Article/details/gurtrhqpi.sHtML

[T37] Lua：字符串拼接
来源：http://baike.epnwcf.com/Article/details/guecuibci.sHtML

"a" .. "b"
来源：http://www.m.share.sjlbkw.cn/Article/details/giewzxhle.sHtML

[T38] Lua：条件
来源：http://read.share.sjlbkw.cn/Article/details/goexrbzux.sHtML

if x > 0 then print("正") end
来源：http://blog.sjlbkw.cn/Article/details/gqtqbjdvz.sHtML

[T39] Lua：模式匹配
来源：http://wap.yfazqb.com/Article/details/gwmbfadky.sHtML

string.find(s, "%d+")
来源：http://read.share.fktsv.cn/Article/details/gnowzprgd.sHtML

[T40] Lua：元表
来源：http://3g.vehdjk.com/Article/details/gvfovwrho.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.vehdjk.com/Article/details/gtrbuhocl.sHtML

[T41] Perl：Hello World
来源：http://www.share.vehdjk.com/Article/details/goluvbljy.sHtML

print "Hello\n";
来源：http://www.blog.vehdjk.com/Article/details/gwwceynzq.sHtML

[T42] Perl：变量类型
来源：http://www.share.fktsv.cn/Article/details/gwwsvrzik.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.tarul.cn/Article/details/gmqepiipc.sHtML

[T43] Perl：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gfqntdlkw.sHtML

"值: $a"
来源：http://m.share.tarul.cn/Article/details/gjfjrhxff.sHtML

[T44] Perl：条件
来源：http://blog.epnwcf.com/Article/details/gssnqisej.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.bbcook.cn/Article/details/gsnzarcmq.sHtML

[T45] Perl：数组遍历
来源：http://www.share.epnwcf.com/Article/details/giofiaxew.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.vehdjk.com/Article/details/gtiizootx.sHtML

[T46] Perl：哈希操作
来源：http://baike.sjlbkw.cn/Article/details/guulahorq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.bbcook.cn/Article/details/gwkjcbhtg.sHtML

[T47] Perl：正则捕获
来源：http://3g.epnwcf.com/Article/details/gxfohlpyw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.tarul.cn/Article/details/gbkmsgqbe.sHtML

[T48] Perl：正则替换
来源：http://www.blog.tarul.cn/Article/details/gfesdbsvk.sHtML

$s =~ s/old/new/g;
来源：http://3g.fktsv.cn/Article/details/glvzxrkxd.sHtML

[T49] Perl：函数
来源：http://www.blog.sjlbkw.cn/Article/details/ghdmfqxgc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gglpsvpcx.sHtML

[T50] Perl：逐行读文件
来源：http://blog.tarul.cn/Article/details/gbyqmgqce.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fktsv.cn/Article/details/gupporgyr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.sjlbkw.cn/Article/details/gpidgboxt.sHtML

[T51] Scala：Hello World
来源：http://m.share.epnwcf.com/Article/details/gtkuqewaj.sHtML

println("Hello")
来源：http://wap.bbcook.cn/Article/details/gkvpjbagm.sHtML

[T52] Scala：变量
来源：http://m.share.vehdjk.com/Article/details/gfdpgkilu.sHtML

val a = 1;  var b = 2
来源：http://wap.epnwcf.com/Article/details/glhnbvhgd.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/ggrpzvsxj.sHtML

s"值: $b"
来源：http://baike.fktsv.cn/Article/details/gfeccirvq.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.tarul.cn/Article/details/ghzwwhlwf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.bbcook.cn/Article/details/grjrztblh.sHtML

[T55] Scala：集合过滤
来源：http://www.share.epnwcf.com/Article/details/gvqrswnqd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.tarul.cn/Article/details/grcmwkunn.sHtML

[T56] Scala：样例类
来源：http://www.blog.tarul.cn/Article/details/gymnhsxrb.sHtML

case class User(name: String, age: Int)
来源：http://www.share.epnwcf.com/Article/details/gszlzravk.sHtML

[T57] Scala：模式匹配
来源：http://m.share.yfazqb.com/Article/details/ghcgxcvgw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.vehdjk.com/Article/details/gghiazqur.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fktsv.cn/Article/details/guqnjfttv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.vehdjk.com/Article/details/gryanbrfh.sHtML

[T59] Scala：循环
来源：http://baike.vehdjk.com/Article/details/glrymhqxt.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fktsv.cn/Article/details/gctepialv.sHtML

[T60] Scala：折叠
来源：http://blog.tarul.cn/Article/details/gfubchmqu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.bbcook.cn/Article/details/gysrraxsh.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gacnvdrjy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/gssjhcnql.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gmpoupouv.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.vehdjk.com/Article/details/ghfowfqte.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.epnwcf.com/Article/details/grocisjsm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.bbcook.cn/Article/details/geqhbrgno.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.vehdjk.com/Article/details/gtfywjqrj.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.tarul.cn/Article/details/goxbdbodb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.tarul.cn/Article/details/glbfpsmim.sHtML

[U04] Py：变量调试打印
来源：http://read.share.bbcook.cn/Article/details/gyimjsges.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.epnwcf.com/Article/details/gerjejcmw.sHtML

[U05] Py：列表去重且保序
来源：http://3g.bbcook.cn/Article/details/gjfxziezb.sHtML

list(dict.fromkeys(arr))
来源：http://blog.bbcook.cn/Article/details/gmtlzjlni.sHtML

[U06] Py：合并两个字典
来源：http://3g.sjlbkw.cn/Article/details/grioeshzv.sHtML

{**a, **b}
来源：http://mobile.epnwcf.com/Article/details/gounsirke.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.tarul.cn/Article/details/gelpplefh.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fktsv.cn/Article/details/giucxubaf.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.bbcook.cn/Article/details/gmpncqqrb.sHtML

[y for x in nested for y in x]
来源：http://3g.vehdjk.com/Article/details/gaulfjtys.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.vehdjk.com/Article/details/gauzavngh.sHtML

max(d, key=d.get)
来源：http://blog.fktsv.cn/Article/details/gzdbnogbr.sHtML

[U10] Py：按值排序字典
来源：http://baike.bbcook.cn/Article/details/gaatihoaf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.sjlbkw.cn/Article/details/gpvzldrse.sHtML

[U11] Py：生成器表达式
来源：http://blog.fktsv.cn/Article/details/gjfjxpcte.sHtML

(x * 2 for x in arr)
来源：http://mobile.tarul.cn/Article/details/grkkeqqyh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.epnwcf.com/Article/details/gxlxsluxu.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.bbcook.cn/Article/details/gevotuahs.sHtML

[U13] Py：固定长度队列
来源：http://3g.tarul.cn/Article/details/gyawsvgms.sHtML

deque(maxlen=10)
来源：http://wap.vehdjk.com/Article/details/gjyyhhqcj.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.epnwcf.com/Article/details/glkbemthm.sHtML

defaultdict(list)
来源：http://read.share.yfazqb.com/Article/details/gvejteypt.sHtML

[U15] Py：高精度计时
来源：http://baike.yfazqb.com/Article/details/gbzllzduk.sHtML

t = time.perf_counter()
来源：http://read.share.fktsv.cn/Article/details/gzhhgztri.sHtML

[U16] Py：命令行参数解析
来源：http://blog.vehdjk.com/Article/details/glfzxbyow.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.epnwcf.com/Article/details/gfmpbripb.sHtML

[U17] Py：初始化日志
来源：http://wap.vehdjk.com/Article/details/gzfinzmrf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.yfazqb.com/Article/details/gusqozaem.sHtML

[U18] Py：预编译正则
来源：http://3g.vehdjk.com/Article/details/gshjdjvhc.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.sjlbkw.cn/Article/details/gjtfnrmxb.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.yfazqb.com/Article/details/gsvvhdsps.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.yfazqb.com/Article/details/geabwrmww.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.bbcook.cn/Article/details/gcbmzlxvv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.sjlbkw.cn/Article/details/gbfybduue.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.epnwcf.com/Article/details/gohzkrzdg.sHtML

@contextlib.contextmanager
来源：http://wap.fktsv.cn/Article/details/geaszryaa.sHtML

[U22] Py：矩阵转置
来源：http://wap.yfazqb.com/Article/details/groqvxvnx.sHtML

list(zip(*m))
来源：http://3g.vehdjk.com/Article/details/gjvyyommc.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.vehdjk.com/Article/details/gopbqmrme.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.bbcook.cn/Article/details/gacaunsgv.sHtML

[U24] Py：路径操作
来源：http://www.m.share.tarul.cn/Article/details/gvudvxvzj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.yfazqb.com/Article/details/gtjepdtwa.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fktsv.cn/Article/details/guvatawbi.sHtML

csv.DictReader(f)
来源：http://baike.tarul.cn/Article/details/guszaikhd.sHtML

[U26] Py：并发下载
来源：http://www.share.tarul.cn/Article/details/gvfouscfd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.yfazqb.com/Article/details/gfwruioyg.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.tarul.cn/Article/details/gdwrtrekp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.yfazqb.com/Article/details/ghimnmxds.sHtML

[U28] Py：类型别名
来源：http://baike.sjlbkw.cn/Article/details/gbswhjwbl.sHtML

UserId = int
来源：http://3g.epnwcf.com/Article/details/gueplyvnl.sHtML

[U29] Py：属性校验
来源：http://mobile.sjlbkw.cn/Article/details/gdddgqida.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fktsv.cn/Article/details/gejwqyipa.sHtML

[U30] Py：数据类
来源：http://3g.vehdjk.com/Article/details/gwulmbtpl.sHtML

@dataclass(slots=True)
来源：http://www.blog.epnwcf.com/Article/details/grjeledrx.sHtML

[U31] Py：单测
来源：http://www.m.share.vehdjk.com/Article/details/gzatklxwi.sHtML

python -m pytest -q
来源：http://3g.yfazqb.com/Article/details/gxukyazou.sHtML

[U32] Py：代码格式化
来源：http://wap.tarul.cn/Article/details/gmyptrrcg.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.tarul.cn/Article/details/ggdypcdab.sHtML

[U33] Py：打包发布
来源：http://mobile.epnwcf.com/Article/details/gprglevcu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.bbcook.cn/Article/details/gpqhzbrit.sHtML

[U34] Py：判断编码
来源：http://mobile.vehdjk.com/Article/details/gcgtummjs.sHtML

chardet.detect(raw)
来源：http://www.share.sjlbkw.cn/Article/details/gjabapamg.sHtML

[U35] Py：发送邮件
来源：http://wap.epnwcf.com/Article/details/gapbzooph.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.vehdjk.com/Article/details/gezbbjhgs.sHtML

[U36] Py：定时任务
来源：http://www.share.tarul.cn/Article/details/gkntvpuxm.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.yfazqb.com/Article/details/gzfjheocn.sHtML

[U37] Py：读写 Excel
来源：http://blog.tarul.cn/Article/details/gqwkalnwt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fktsv.cn/Article/details/gjrthdkrw.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.bbcook.cn/Article/details/gaogsssoq.sHtML

Path(__file__).resolve().parent
来源：http://baike.fktsv.cn/Article/details/gigsecqvz.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.tarul.cn/Article/details/gfbrbojab.sHtML

sys.stdout.isatty()
来源：http://read.share.epnwcf.com/Article/details/gyusopfne.sHtML

[U40] Py：打印到标准错误
来源：http://baike.sjlbkw.cn/Article/details/gqobfxlsj.sHtML

print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/gfpyyufgr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.yfazqb.com/Article/details/gxqbpmvus.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.tarul.cn/Article/details/gyinazfzd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.sjlbkw.cn/Article/details/gghwyhogz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.epnwcf.com/Article/details/gjnvrqrbi.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.vehdjk.com/Article/details/ginelqckc.sHtML

namespace App\Http;
来源：http://m.share.tarul.cn/Article/details/gyihquimb.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.yfazqb.com/Article/details/gerauvdyv.sHtML

declare(strict_types=1);
来源：http://wap.tarul.cn/Article/details/gxhaiypfh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.yfazqb.com/Article/details/gihlsqyfv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gkfqhgicx.sHtML

[U46] PHP：可空类型
来源：http://3g.bbcook.cn/Article/details/ghtqpzjcd.sHtML

?string $name = null
来源：http://wap.yfazqb.com/Article/details/grkltdkpx.sHtML

[U47] PHP：联合类型
来源：http://m.share.fktsv.cn/Article/details/gstouufoq.sHtML

int|string $id
来源：http://read.share.fktsv.cn/Article/details/gharbfwqg.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fktsv.cn/Article/details/gsmynsflp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcbgsjih.sHtML

[U49] PHP：只读属性
来源：http://3g.yfazqb.com/Article/details/guqewpxzz.sHtML

public readonly string $name
来源：http://wap.tarul.cn/Article/details/gyzqmsglt.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.yfazqb.com/Article/details/gqdxgszyl.sHtML

public function __construct(private int $id) {}
来源：http://blog.sjlbkw.cn/Article/details/glybywuxy.sHtML

[U51] PHP：数组解构
来源：http://blog.vehdjk.com/Article/details/glawqnfzg.sHtML

[$a, $b] = $arr;
来源：http://wap.fktsv.cn/Article/details/gsimanhni.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.sjlbkw.cn/Article/details/grtsmjxqu.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.vehdjk.com/Article/details/gstfobuqa.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.epnwcf.com/Article/details/gzbwmtfoa.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.sjlbkw.cn/Article/details/gwvywuzic.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.vehdjk.com/Article/details/gjbmoolgj.sHtML

$obj?->method()
来源：http://blog.tarul.cn/Article/details/gaslbucus.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fktsv.cn/Article/details/gbgmrtxqd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.epnwcf.com/Article/details/gpwgmkpyx.sHtML

[U56] PHP：命名参数
来源：http://3g.tarul.cn/Article/details/glhmcdplb.sHtML

f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/gwxpvjltf.sHtML

[U57] PHP：字符串插值
来源：http://3g.epnwcf.com/Article/details/guyssoqta.sHtML

"值: {$a}"
来源：http://read.share.fktsv.cn/Article/details/gthftthtk.sHtML

[U58] PHP：数组三件套
来源：http://3g.tarul.cn/Article/details/gygoigame.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gpbpbxluk.sHtML

[U59] PHP：自定义排序
来源：http://wap.tarul.cn/Article/details/gwvezxtqn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.bbcook.cn/Article/details/gyrkiojzo.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.tarul.cn/Article/details/getmdnejy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.tarul.cn/Article/details/gaiihnmth.sHtML

[U61] PHP：正则
来源：http://mobile.sjlbkw.cn/Article/details/gvyaqaule.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.sjlbkw.cn/Article/details/geeopylzn.sHtML

[U62] PHP：日期对象
来源：http://wap.epnwcf.com/Article/details/gkgidwzmg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.epnwcf.com/Article/details/gfxjrkkyu.sHtML

[U63] PHP：文件读写
来源：http://blog.sjlbkw.cn/Article/details/gsthkhcuw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.yfazqb.com/Article/details/ginxlztkh.sHtML

[U64] PHP：目录遍历
来源：http://baike.bbcook.cn/Article/details/geiwhviot.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.sjlbkw.cn/Article/details/gzutqzhph.sHtML

[U65] PHP：会话
来源：http://blog.vehdjk.com/Article/details/glbeotzzo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fktsv.cn/Article/details/gowwlyemb.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fktsv.cn/Article/details/glnioddzc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.epnwcf.com/Article/details/gxwxdgibq.sHtML

[U67] PHP：处理文件上传
来源：http://blog.epnwcf.com/Article/details/gcjuizbdx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.tarul.cn/Article/details/goqkotntx.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.vehdjk.com/Article/details/guzcsyfuh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.yfazqb.com/Article/details/gneupxmaf.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fktsv.cn/Article/details/gkiotcnox.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.bbcook.cn/Article/details/gxpttrtua.sHtML

[U70] PHP：PDO 事务
来源：http://3g.sjlbkw.cn/Article/details/gfccsnxqb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.bbcook.cn/Article/details/ggcixivpg.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.bbcook.cn/Article/details/guaiuuexg.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.tarul.cn/Article/details/grubrivuu.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.epnwcf.com/Article/details/gdmequfin.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.vehdjk.com/Article/details/gqubyrfmj.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.vehdjk.com/Article/details/gsrfnvuhx.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fktsv.cn/Article/details/gudfvuawr.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fktsv.cn/Article/details/gvxcncrek.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fktsv.cn/Article/details/giqregfep.sHtML


<!-- 参考信息 -->