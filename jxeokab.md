代发 wailian999

[S45] C++：lambda
来源：http://mobile.bbcook.cn/Article/details/gvushpdag.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.sjlbkw.cn/Article/details/gnwqzhfzt.sHtML

[S46] C++：函数模板
来源：http://www.m.share.bbcook.cn/Article/details/grovnvafd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.sjlbkw.cn/Article/details/gorwhequy.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.bbcook.cn/Article/details/gdvpimmee.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.yfazqb.com/Article/details/gajfvmhpf.sHtML

[S48] C++：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gyqrbosbt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.yfazqb.com/Article/details/gsuonockv.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.vehdjk.com/Article/details/gzfwrszmq.sHtML

[S49] C++：写文件
来源：http://www.blog.epnwcf.com/Article/details/gewsypvjz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.epnwcf.com/Article/details/gbswfudjg.sHtML

[S50] C++：格式化数字
来源：http://wap.tarul.cn/Article/details/gsatblgbs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/glwwofoua.sHtML

[S51] C++：显式类型转换
来源：http://wap.bbcook.cn/Article/details/gfokvdalp.sHtML

static_cast<double>(a) / b
来源：http://www.blog.vehdjk.com/Article/details/glnrxenck.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.bbcook.cn/Article/details/glcbsczxx.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.sjlbkw.cn/Article/details/gopkrvnnh.sHtML

[S53] C++：移动语义
来源：http://m.share.vehdjk.com/Article/details/giidwtorj.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.vehdjk.com/Article/details/ggsrwowcj.sHtML

[S54] C++：异常处理
来源：http://www.share.vehdjk.com/Article/details/gjomreutq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fktsv.cn/Article/details/gguqgguos.sHtML

[S55] C++：结构化绑定
来源：http://read.share.tarul.cn/Article/details/gldvqoqox.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.vehdjk.com/Article/details/gyjhukarf.sHtML

[S56] C++：optional
来源：http://www.blog.vehdjk.com/Article/details/gtlkevuuv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fktsv.cn/Article/details/gayhkzqxy.sHtML

[S57] C++：编译期常量
来源：http://baike.fktsv.cn/Article/details/gciahxcew.sHtML

constexpr int N = 10;
来源：http://mobile.vehdjk.com/Article/details/garzdlktg.sHtML

[S58] C++：命名空间
来源：http://baike.bbcook.cn/Article/details/gicltnuve.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.epnwcf.com/Article/details/gqutzwejw.sHtML

[S59] C++：静态断言
来源：http://baike.vehdjk.com/Article/details/gclgoemya.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.bbcook.cn/Article/details/gdewuuzvw.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.epnwcf.com/Article/details/gdojwekoh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.tarul.cn/Article/details/gykggxcrf.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gyvikvgen.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.epnwcf.com/Article/details/gjoltsvxg.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gksklcdma.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.tarul.cn/Article/details/gvijupfvc.sHtML

println("Hello")
来源：http://3g.bbcook.cn/Article/details/gffyiskzv.sHtML

[T02] Kotlin：变量
来源：http://www.blog.tarul.cn/Article/details/gxyjcjupz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.yfazqb.com/Article/details/gzijeield.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.bbcook.cn/Article/details/gqdricyhv.sHtML

"值: $b"
来源：http://baike.tarul.cn/Article/details/gjxxkpnsr.sHtML

[T04] Kotlin：空安全
来源：http://m.share.bbcook.cn/Article/details/gokmlhlti.sHtML

val n: String? = null;  n?.length
来源：http://mobile.vehdjk.com/Article/details/gdmqgousa.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.epnwcf.com/Article/details/gpnwnshrw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.epnwcf.com/Article/details/gfoyvrxfl.sHtML

[T06] Kotlin：集合映射
来源：http://wap.sjlbkw.cn/Article/details/gxsiujqbq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.epnwcf.com/Article/details/gbhruuxav.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlqgmdog.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fktsv.cn/Article/details/gxoljxbes.sHtML

[T08] Kotlin：数据类
来源：http://mobile.sjlbkw.cn/Article/details/gngpcbknd.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.bbcook.cn/Article/details/gbvjkybwy.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.epnwcf.com/Article/details/gvtbthbfu.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.vehdjk.com/Article/details/giwfszofs.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.tarul.cn/Article/details/gvodpvdvv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.yfazqb.com/Article/details/gsgcomgbq.sHtML

[T11] Kotlin：协程
来源：http://mobile.fktsv.cn/Article/details/gnkxobovq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.vehdjk.com/Article/details/gamdodity.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.bbcook.cn/Article/details/gzozdotev.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gvjbucsjh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.yfazqb.com/Article/details/guvozqmom.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.yfazqb.com/Article/details/gsaycotzx.sHtML

[T14] Kotlin：循环
来源：http://mobile.sjlbkw.cn/Article/details/gfutvyjvh.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gymolevxo.sHtML

[T15] Kotlin：接口
来源：http://mobile.fktsv.cn/Article/details/glhaomafl.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.sjlbkw.cn/Article/details/gvpcsvkuj.sHtML

[T16] Swift：Hello World
来源：http://3g.epnwcf.com/Article/details/gmxixvvdf.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gvgsmevlx.sHtML

[T17] Swift：变量与常量
来源：http://m.share.yfazqb.com/Article/details/gbwdysuqy.sHtML

var a = 1;  let b = 2
来源：http://www.blog.epnwcf.com/Article/details/gqctqqbxz.sHtML

[T18] Swift：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/giospvopx.sHtML

"值: \(b)"
来源：http://www.blog.bbcook.cn/Article/details/gtwoenbhs.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrfipaxh.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyitivkyh.sHtML

[T20] Swift：数组操作
来源：http://mobile.yfazqb.com/Article/details/gepollolz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.tarul.cn/Article/details/gssinndgf.sHtML

[T21] Swift：遍历
来源：http://www.blog.bbcook.cn/Article/details/gxzsdcmok.sHtML

for x in a { print(x) }
来源：http://m.share.sjlbkw.cn/Article/details/gkwlyvsql.sHtML

[T22] Swift：字典
来源：http://www.m.share.fktsv.cn/Article/details/glppodcde.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.yfazqb.com/Article/details/gvkyrcxom.sHtML

[T23] Swift：函数
来源：http://www.blog.vehdjk.com/Article/details/gicaqtwpv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.yfazqb.com/Article/details/gahjhyxuv.sHtML

[T24] Swift：闭包
来源：http://blog.bbcook.cn/Article/details/gswzxnuwn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.yfazqb.com/Article/details/gkskqvlvp.sHtML

[T25] Swift：结构体
来源：http://www.blog.sjlbkw.cn/Article/details/glqegtsqe.sHtML

struct P { var x: Int }
来源：http://3g.yfazqb.com/Article/details/gfonryahg.sHtML

[T26] Swift：类与重写
来源：http://3g.sjlbkw.cn/Article/details/gpsknpotm.sHtML

class A: Base { override func f() {} }
来源：http://blog.yfazqb.com/Article/details/gmtywlppz.sHtML

[T27] Swift：错误处理
来源：http://m.share.epnwcf.com/Article/details/gmpkvzfee.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.sjlbkw.cn/Article/details/gdvapvktc.sHtML

[T28] Swift：枚举
来源：http://mobile.fktsv.cn/Article/details/ggifwwtzj.sHtML

enum Color { case red, green }
来源：http://www.share.epnwcf.com/Article/details/gnlmumkes.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.epnwcf.com/Article/details/gvfrlkfgd.sHtML

guard let x = opt else { return }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqyaamxfg.sHtML

[T30] Swift：协议
来源：http://mobile.epnwcf.com/Article/details/gaeesefgl.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.sjlbkw.cn/Article/details/ggwxeploe.sHtML

[T31] Lua：Hello World
来源：http://mobile.yfazqb.com/Article/details/gyujcopah.sHtML

print("Hello")
来源：http://blog.yfazqb.com/Article/details/ghmnmgkss.sHtML

[T32] Lua：局部变量
来源：http://www.share.epnwcf.com/Article/details/gqnwhvyya.sHtML

local a = 1
来源：http://mobile.epnwcf.com/Article/details/gzclshjli.sHtML

[T33] Lua：表（数组）
来源：http://read.share.tarul.cn/Article/details/gnwrzcrlj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.bbcook.cn/Article/details/gtxlvlvnb.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.vehdjk.com/Article/details/gakukbmlr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.vehdjk.com/Article/details/gvhntprkc.sHtML

[T35] Lua：字典表
来源：http://www.m.share.bbcook.cn/Article/details/gabasjwsf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.bbcook.cn/Article/details/gomibnofp.sHtML

[T36] Lua：函数
来源：http://read.share.tarul.cn/Article/details/gypkedvdp.sHtML

function add(a, b) return a + b end
来源：http://3g.fktsv.cn/Article/details/gycpifmtw.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.vehdjk.com/Article/details/gtpqftugl.sHtML

"a" .. "b"
来源：http://baike.epnwcf.com/Article/details/gtidefasn.sHtML

[T38] Lua：条件
来源：http://wap.tarul.cn/Article/details/gjcmvkzfs.sHtML

if x > 0 then print("正") end
来源：http://3g.sjlbkw.cn/Article/details/gullipqjx.sHtML

[T39] Lua：模式匹配
来源：http://wap.epnwcf.com/Article/details/gzhrdlufy.sHtML

string.find(s, "%d+")
来源：http://www.blog.tarul.cn/Article/details/gqytlyvzr.sHtML

[T40] Lua：元表
来源：http://wap.sjlbkw.cn/Article/details/ginfynzfx.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.epnwcf.com/Article/details/gkipnxrzp.sHtML

[T41] Perl：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/guzxzdesv.sHtML

print "Hello\n";
来源：http://www.blog.vehdjk.com/Article/details/gmnytdyfj.sHtML

[T42] Perl：变量类型
来源：http://m.share.vehdjk.com/Article/details/gurcmcbmr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.tarul.cn/Article/details/geesbmxmk.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gzywmulhr.sHtML

"值: $a"
来源：http://www.blog.fktsv.cn/Article/details/gezpjqdjx.sHtML

[T44] Perl：条件
来源：http://www.m.share.fktsv.cn/Article/details/gnfazyfyt.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.tarul.cn/Article/details/gnpcwhdzt.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fktsv.cn/Article/details/gsgocdrvd.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fktsv.cn/Article/details/gtjnvxvxt.sHtML

[T46] Perl：哈希操作
来源：http://baike.yfazqb.com/Article/details/gijjggmho.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.sjlbkw.cn/Article/details/gxgphpnum.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.bbcook.cn/Article/details/gypvaukzp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.sjlbkw.cn/Article/details/golsuuzbr.sHtML

[T48] Perl：正则替换
来源：http://blog.bbcook.cn/Article/details/gpkesajfw.sHtML

$s =~ s/old/new/g;
来源：http://baike.tarul.cn/Article/details/ghkvfhjth.sHtML

[T49] Perl：函数
来源：http://www.blog.fktsv.cn/Article/details/gioircchk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gtnfqsxrx.sHtML

[T50] Perl：逐行读文件
来源：http://blog.bbcook.cn/Article/details/gnqgpqjlm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.vehdjk.com/Article/details/gtrquddth.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.epnwcf.com/Article/details/gxmmfvczo.sHtML

[T51] Scala：Hello World
来源：http://3g.yfazqb.com/Article/details/gmobrrktp.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/gociovwgz.sHtML

[T52] Scala：变量
来源：http://www.blog.fktsv.cn/Article/details/gveoqaryy.sHtML

val a = 1;  var b = 2
来源：http://wap.bbcook.cn/Article/details/gntkkjpzs.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/giholezce.sHtML

s"值: $b"
来源：http://www.share.tarul.cn/Article/details/gjsejpryr.sHtML

[T54] Scala：集合映射
来源：http://blog.yfazqb.com/Article/details/govdwktea.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gcbsecedo.sHtML

[T55] Scala：集合过滤
来源：http://wap.tarul.cn/Article/details/gqggjtumz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.sjlbkw.cn/Article/details/gvojmgafe.sHtML

[T56] Scala：样例类
来源：http://mobile.tarul.cn/Article/details/gmxesuciq.sHtML

case class User(name: String, age: Int)
来源：http://m.share.yfazqb.com/Article/details/gziojeond.sHtML

[T57] Scala：模式匹配
来源：http://wap.yfazqb.com/Article/details/gxeglnznf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fktsv.cn/Article/details/gwozgfujy.sHtML

[T58] Scala：函数定义
来源：http://wap.fktsv.cn/Article/details/gmgiwfbyj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.epnwcf.com/Article/details/gcniwvuzm.sHtML

[T59] Scala：循环
来源：http://blog.yfazqb.com/Article/details/gricyfwsw.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.yfazqb.com/Article/details/gattefihg.sHtML

[T60] Scala：折叠
来源：http://blog.fktsv.cn/Article/details/gwmnlsvls.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.epnwcf.com/Article/details/gkkqimraf.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gmqehgtbk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fktsv.cn/Article/details/gapkevtaa.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ghutaaueh.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.tarul.cn/Article/details/grumqnuzu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fktsv.cn/Article/details/gahjapsrh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.sjlbkw.cn/Article/details/gjbfhtqjs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fktsv.cn/Article/details/gzhxgbvhw.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fktsv.cn/Article/details/ggytmwbax.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.vehdjk.com/Article/details/glxgtthas.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.bbcook.cn/Article/details/ggrhyktxt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.tarul.cn/Article/details/ghqizjxsv.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.tarul.cn/Article/details/ghbecnjyl.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.yfazqb.com/Article/details/gcjkpwmnd.sHtML

[U06] Py：合并两个字典
来源：http://baike.bbcook.cn/Article/details/gsjpajpqt.sHtML

{**a, **b}
来源：http://m.share.vehdjk.com/Article/details/gkyrsoppi.sHtML

[U07] Py：反转字典键值
来源：http://wap.bbcook.cn/Article/details/gpvhulohu.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.tarul.cn/Article/details/gcrdiuost.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.bbcook.cn/Article/details/gfoxgelrp.sHtML

[y for x in nested for y in x]
来源：http://www.share.fktsv.cn/Article/details/gldaaohrd.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.sjlbkw.cn/Article/details/gqqayhcsg.sHtML

max(d, key=d.get)
来源：http://m.share.yfazqb.com/Article/details/geooigcxa.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fktsv.cn/Article/details/gnmjvndea.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.sjlbkw.cn/Article/details/gyerorexf.sHtML

[U11] Py：生成器表达式
来源：http://www.share.yfazqb.com/Article/details/grbapsdfu.sHtML

(x * 2 for x in arr)
来源：http://blog.epnwcf.com/Article/details/gulhamqlv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.epnwcf.com/Article/details/ghvkhkpqo.sHtML

Counter(arr).most_common(3)
来源：http://read.share.sjlbkw.cn/Article/details/gnrhqfdqn.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.sjlbkw.cn/Article/details/gfirnufwi.sHtML

deque(maxlen=10)
来源：http://www.blog.sjlbkw.cn/Article/details/gjewewuvg.sHtML

[U14] Py：分组收集到列表
来源：http://baike.tarul.cn/Article/details/gyogzyrvh.sHtML

defaultdict(list)
来源：http://read.share.fktsv.cn/Article/details/gfvbnroqf.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.vehdjk.com/Article/details/gifpyoxpg.sHtML

t = time.perf_counter()
来源：http://www.share.epnwcf.com/Article/details/gobvbrlzx.sHtML

[U16] Py：命令行参数解析
来源：http://wap.yfazqb.com/Article/details/gargpduzf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.tarul.cn/Article/details/gojmcgjyp.sHtML

[U17] Py：初始化日志
来源：http://www.blog.tarul.cn/Article/details/gejgdprqn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.vehdjk.com/Article/details/gheotyosc.sHtML

[U18] Py：预编译正则
来源：http://baike.fktsv.cn/Article/details/gkboohnbq.sHtML

pat = re.compile(r"\d+")
来源：http://blog.sjlbkw.cn/Article/details/gdplfgnzr.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fktsv.cn/Article/details/gqxvhfoyg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.epnwcf.com/Article/details/gzbszbipp.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.epnwcf.com/Article/details/gwuvvcggu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.tarul.cn/Article/details/gjacktafk.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.vehdjk.com/Article/details/gjutfdzbh.sHtML

@contextlib.contextmanager
来源：http://www.share.epnwcf.com/Article/details/gdqqnrmum.sHtML

[U22] Py：矩阵转置
来源：http://m.share.bbcook.cn/Article/details/gqxdrsqya.sHtML

list(zip(*m))
来源：http://wap.bbcook.cn/Article/details/ghgkqalhi.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fktsv.cn/Article/details/gkubpfqri.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.bbcook.cn/Article/details/gpqegsyyz.sHtML

[U24] Py：路径操作
来源：http://www.share.fktsv.cn/Article/details/gfeaxvodi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/gihbtypvq.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fktsv.cn/Article/details/gdimksqdr.sHtML

csv.DictReader(f)
来源：http://mobile.vehdjk.com/Article/details/gznkefxuz.sHtML

[U26] Py：并发下载
来源：http://3g.tarul.cn/Article/details/gnpdfmjnn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.tarul.cn/Article/details/gwnffehjv.sHtML

[U27] Py：异步 HTTP
来源：http://wap.sjlbkw.cn/Article/details/gmnzryhsz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.tarul.cn/Article/details/gshvghtnw.sHtML

[U28] Py：类型别名
来源：http://www.share.sjlbkw.cn/Article/details/ghaypudqa.sHtML

UserId = int
来源：http://mobile.vehdjk.com/Article/details/gfjtrnrxj.sHtML

[U29] Py：属性校验
来源：http://m.share.fktsv.cn/Article/details/gktzkeoet.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fktsv.cn/Article/details/gkhxefrwu.sHtML

[U30] Py：数据类
来源：http://3g.tarul.cn/Article/details/gqqaxhpss.sHtML

@dataclass(slots=True)
来源：http://mobile.tarul.cn/Article/details/gpmjfmycv.sHtML

[U31] Py：单测
来源：http://www.blog.vehdjk.com/Article/details/gpzrzkefw.sHtML

python -m pytest -q
来源：http://www.m.share.fktsv.cn/Article/details/gekqjudzy.sHtML

[U32] Py：代码格式化
来源：http://mobile.vehdjk.com/Article/details/gzfgwberi.sHtML

ruff format . && ruff check --fix .
来源：http://baike.epnwcf.com/Article/details/grcyoxgew.sHtML

[U33] Py：打包发布
来源：http://baike.tarul.cn/Article/details/gxtknkclh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.yfazqb.com/Article/details/gdwemutkw.sHtML

[U34] Py：判断编码
来源：http://3g.fktsv.cn/Article/details/glgnyibrj.sHtML

chardet.detect(raw)
来源：http://mobile.fktsv.cn/Article/details/guehhqzdq.sHtML

[U35] Py：发送邮件
来源：http://wap.yfazqb.com/Article/details/gezrdjgmd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.bbcook.cn/Article/details/gpusehihu.sHtML

[U36] Py：定时任务
来源：http://baike.epnwcf.com/Article/details/gijglomqv.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.vehdjk.com/Article/details/gkukfinar.sHtML

[U37] Py：读写 Excel
来源：http://baike.sjlbkw.cn/Article/details/gkjouhbxk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fktsv.cn/Article/details/gjwdbjyrb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.bbcook.cn/Article/details/gkxcjrzcr.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.epnwcf.com/Article/details/ggsliwhiv.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.vehdjk.com/Article/details/gwsczpomf.sHtML

sys.stdout.isatty()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxwkromg.sHtML

[U40] Py：打印到标准错误
来源：http://blog.sjlbkw.cn/Article/details/gsdhmpwkl.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.yfazqb.com/Article/details/gpsgcvhxh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.bbcook.cn/Article/details/gflrbbseb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.sjlbkw.cn/Article/details/gtpdcznhd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.epnwcf.com/Article/details/gbtvssnfh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.yfazqb.com/Article/details/gmoyhwwrr.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.yfazqb.com/Article/details/ghbwnigno.sHtML

namespace App\Http;
来源：http://m.share.epnwcf.com/Article/details/gwxenrvty.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.tarul.cn/Article/details/gcqrjwesa.sHtML

declare(strict_types=1);
来源：http://www.m.share.epnwcf.com/Article/details/gaisjcryj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.sjlbkw.cn/Article/details/gjvrgejor.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gmkptuwqi.sHtML

[U46] PHP：可空类型
来源：http://3g.bbcook.cn/Article/details/gbjpvlvxg.sHtML

?string $name = null
来源：http://3g.tarul.cn/Article/details/gztmpgpdg.sHtML

[U47] PHP：联合类型
来源：http://mobile.sjlbkw.cn/Article/details/ghtfaoqvr.sHtML

int|string $id
来源：http://baike.sjlbkw.cn/Article/details/grcfbbelt.sHtML

[U48] PHP：纯枚举
来源：http://wap.tarul.cn/Article/details/gqncktmdr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.tarul.cn/Article/details/gpvyroubt.sHtML

[U49] PHP：只读属性
来源：http://baike.yfazqb.com/Article/details/gzrilnszk.sHtML

public readonly string $name
来源：http://baike.bbcook.cn/Article/details/glzwgkmcz.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fktsv.cn/Article/details/gfxxaotdc.sHtML

public function __construct(private int $id) {}
来源：http://blog.fktsv.cn/Article/details/gopgbephd.sHtML

[U51] PHP：数组解构
来源：http://wap.sjlbkw.cn/Article/details/gedgfwddx.sHtML

[$a, $b] = $arr;
来源：http://www.blog.bbcook.cn/Article/details/glodklflx.sHtML

[U52] PHP：箭头函数
来源：http://blog.sjlbkw.cn/Article/details/gkbpxxvgn.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.bbcook.cn/Article/details/gttuxbzgu.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fktsv.cn/Article/details/gjcdwtqor.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.epnwcf.com/Article/details/gtunhjyvg.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.yfazqb.com/Article/details/gunhzwavi.sHtML

$obj?->method()
来源：http://m.share.bbcook.cn/Article/details/gxtgmxbol.sHtML

[U55] PHP：match 表达式
来源：http://www.share.yfazqb.com/Article/details/gltuxvilb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.epnwcf.com/Article/details/gdzavdzyz.sHtML

[U56] PHP：命名参数
来源：http://3g.epnwcf.com/Article/details/gqbeaicnk.sHtML

f(a: 1, b: 2)
来源：http://www.share.vehdjk.com/Article/details/gzjbggouu.sHtML

[U57] PHP：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gjorhktzh.sHtML

"值: {$a}"
来源：http://www.blog.epnwcf.com/Article/details/gkapgrzql.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.yfazqb.com/Article/details/gztcaznem.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fktsv.cn/Article/details/gbefnbyyu.sHtML

[U59] PHP：自定义排序
来源：http://baike.tarul.cn/Article/details/gujkoiiep.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.vehdjk.com/Article/details/giianukme.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.yfazqb.com/Article/details/gjyvbzzrz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.yfazqb.com/Article/details/gxldzhwak.sHtML

[U61] PHP：正则
来源：http://blog.fktsv.cn/Article/details/gqojhwiia.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fktsv.cn/Article/details/golaeextp.sHtML

[U62] PHP：日期对象
来源：http://3g.epnwcf.com/Article/details/giesdvmso.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.tarul.cn/Article/details/gbmjlbeeg.sHtML

[U63] PHP：文件读写
来源：http://blog.tarul.cn/Article/details/ginbraujb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.vehdjk.com/Article/details/gcvpurnuf.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.bbcook.cn/Article/details/ggigmkwzd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.yfazqb.com/Article/details/gaggwziab.sHtML

[U65] PHP：会话
来源：http://www.m.share.sjlbkw.cn/Article/details/gaymweewt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gryfcevmg.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.tarul.cn/Article/details/gpumvalco.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.tarul.cn/Article/details/gqlyedbve.sHtML

[U67] PHP：处理文件上传
来源：http://blog.bbcook.cn/Article/details/goeowcuht.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fktsv.cn/Article/details/gbvofowic.sHtML

[U68] PHP：PDO 连接
来源：http://baike.sjlbkw.cn/Article/details/gjllngyzm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.sjlbkw.cn/Article/details/ghsiicgju.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.epnwcf.com/Article/details/gvrfafecw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.sjlbkw.cn/Article/details/gtmslkaxu.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.tarul.cn/Article/details/gplqevggo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.yfazqb.com/Article/details/gzecxmjad.sHtML


<!-- 参考信息 -->