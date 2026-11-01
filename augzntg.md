代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.m.share.bbcook.cn/Article/details/goonkmidk.sHtML

[S49] C++：写文件
来源：http://blog.bbcook.cn/Article/details/gsdcrrdba.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.epnwcf.com/Article/details/gtcssuhhc.sHtML

[S50] C++：格式化数字
来源：http://blog.epnwcf.com/Article/details/gccndldyp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gnjthgocl.sHtML

[S51] C++：显式类型转换
来源：http://baike.epnwcf.com/Article/details/giyqcncjx.sHtML

static_cast<double>(a) / b
来源：http://mobile.fktsv.cn/Article/details/gpdlsbkpj.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.sjlbkw.cn/Article/details/gkzgephzi.sHtML

int size() const noexcept { return n_; }
来源：http://wap.sjlbkw.cn/Article/details/gmhdrclly.sHtML

[S53] C++：移动语义
来源：http://m.share.bbcook.cn/Article/details/grdfhefmx.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.tarul.cn/Article/details/gsgckcnob.sHtML

[S54] C++：异常处理
来源：http://www.blog.vehdjk.com/Article/details/ghjwvpxmz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.vehdjk.com/Article/details/gaqcxqakx.sHtML

[S55] C++：结构化绑定
来源：http://mobile.bbcook.cn/Article/details/gonbpgucd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.bbcook.cn/Article/details/gpaxlbfbx.sHtML

[S56] C++：optional
来源：http://blog.sjlbkw.cn/Article/details/ggzkebulb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.tarul.cn/Article/details/gqgygfyvm.sHtML

[S57] C++：编译期常量
来源：http://mobile.fktsv.cn/Article/details/gqavppozi.sHtML

constexpr int N = 10;
来源：http://www.m.share.bbcook.cn/Article/details/goclbmwup.sHtML

[S58] C++：命名空间
来源：http://www.blog.fktsv.cn/Article/details/gdiygfcug.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.epnwcf.com/Article/details/gbobxqrdr.sHtML

[S59] C++：静态断言
来源：http://wap.tarul.cn/Article/details/gozbiuofs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.yfazqb.com/Article/details/gxekyqonz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.sjlbkw.cn/Article/details/glkaxtuml.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.epnwcf.com/Article/details/gsidxewqc.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gaohsxlfq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/gdzlagsqu.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gufnilwao.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fktsv.cn/Article/details/grriqbrdg.sHtML

println("Hello")
来源：http://blog.epnwcf.com/Article/details/gmaeaxqss.sHtML

[T02] Kotlin：变量
来源：http://read.share.tarul.cn/Article/details/gnuqznlmc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fktsv.cn/Article/details/grlorgwym.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fktsv.cn/Article/details/gtxrgqxfs.sHtML

"值: $b"
来源：http://3g.epnwcf.com/Article/details/gwezwemwt.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.yfazqb.com/Article/details/gnvbzfole.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.bbcook.cn/Article/details/gzpbdrhkj.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.tarul.cn/Article/details/gmssarltf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.vehdjk.com/Article/details/gabobduqc.sHtML

[T06] Kotlin：集合映射
来源：http://baike.yfazqb.com/Article/details/gkwcpyqal.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.vehdjk.com/Article/details/glkednwkt.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.vehdjk.com/Article/details/gtmzzunny.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.yfazqb.com/Article/details/gcvjvsqtd.sHtML

[T08] Kotlin：数据类
来源：http://read.share.yfazqb.com/Article/details/gupwcqwjd.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.yfazqb.com/Article/details/gkgesgfub.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.vehdjk.com/Article/details/gbjogrwsq.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fktsv.cn/Article/details/gbjqbggwx.sHtML

[T10] Kotlin：默认参数
来源：http://blog.vehdjk.com/Article/details/gvlapnrqi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fktsv.cn/Article/details/gaborioxb.sHtML

[T11] Kotlin：协程
来源：http://baike.yfazqb.com/Article/details/gkbfkxebe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.epnwcf.com/Article/details/gzgbxyzln.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.vehdjk.com/Article/details/gfntcvpbb.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.vehdjk.com/Article/details/gcvseyoli.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.epnwcf.com/Article/details/gzrfqddlk.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.tarul.cn/Article/details/glayznswm.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.yfazqb.com/Article/details/gxyzagkhi.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/gktvlvfqu.sHtML

[T15] Kotlin：接口
来源：http://www.share.epnwcf.com/Article/details/ggcpnihua.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.epnwcf.com/Article/details/gmtcccnoy.sHtML

[T16] Swift：Hello World
来源：http://read.share.fktsv.cn/Article/details/gxzubpjsd.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/gdmiawrio.sHtML

[T17] Swift：变量与常量
来源：http://mobile.bbcook.cn/Article/details/gncweisos.sHtML

var a = 1;  let b = 2
来源：http://mobile.fktsv.cn/Article/details/gsrhrmczt.sHtML

[T18] Swift：字符串插值
来源：http://blog.epnwcf.com/Article/details/gqjrbdqar.sHtML

"值: \(b)"
来源：http://wap.bbcook.cn/Article/details/goeifsvbp.sHtML

[T19] Swift：可选绑定
来源：http://m.share.tarul.cn/Article/details/gbypnhvsm.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.yfazqb.com/Article/details/gulfqjzik.sHtML

[T20] Swift：数组操作
来源：http://www.share.fktsv.cn/Article/details/gsawucnau.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.bbcook.cn/Article/details/gsetbhcqg.sHtML

[T21] Swift：遍历
来源：http://mobile.tarul.cn/Article/details/gjduixekd.sHtML

for x in a { print(x) }
来源：http://wap.bbcook.cn/Article/details/gifgqkzns.sHtML

[T22] Swift：字典
来源：http://baike.tarul.cn/Article/details/gqkmxeqxk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.vehdjk.com/Article/details/gioncjhki.sHtML

[T23] Swift：函数
来源：http://3g.bbcook.cn/Article/details/gnsyoyuqu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.sjlbkw.cn/Article/details/gcaoihilk.sHtML

[T24] Swift：闭包
来源：http://www.m.share.sjlbkw.cn/Article/details/gkapigrev.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.yfazqb.com/Article/details/gigrymruz.sHtML

[T25] Swift：结构体
来源：http://read.share.tarul.cn/Article/details/goxmggmof.sHtML

struct P { var x: Int }
来源：http://blog.sjlbkw.cn/Article/details/gmwpmpcpy.sHtML

[T26] Swift：类与重写
来源：http://baike.fktsv.cn/Article/details/gwzopvxvy.sHtML

class A: Base { override func f() {} }
来源：http://www.share.vehdjk.com/Article/details/gijvcfqlt.sHtML

[T27] Swift：错误处理
来源：http://wap.yfazqb.com/Article/details/gejtxdmmm.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fktsv.cn/Article/details/ggnvwtpgb.sHtML

[T28] Swift：枚举
来源：http://www.blog.epnwcf.com/Article/details/geuvlzady.sHtML

enum Color { case red, green }
来源：http://blog.bbcook.cn/Article/details/grntwynuw.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.vehdjk.com/Article/details/ggxqeanef.sHtML

guard let x = opt else { return }
来源：http://www.blog.vehdjk.com/Article/details/gvsufyuki.sHtML

[T30] Swift：协议
来源：http://m.share.epnwcf.com/Article/details/gwvjekuby.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.tarul.cn/Article/details/gipnjpfau.sHtML

[T31] Lua：Hello World
来源：http://www.share.yfazqb.com/Article/details/gldaomnrm.sHtML

print("Hello")
来源：http://www.share.tarul.cn/Article/details/gqhieaaoi.sHtML

[T32] Lua：局部变量
来源：http://m.share.tarul.cn/Article/details/gnoglnmpd.sHtML

local a = 1
来源：http://read.share.bbcook.cn/Article/details/gjivdkwlo.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fktsv.cn/Article/details/gorrkemgd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.vehdjk.com/Article/details/glpbnnwkc.sHtML

[T34] Lua：遍历表
来源：http://blog.epnwcf.com/Article/details/guetgpqpc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.tarul.cn/Article/details/gieudvxol.sHtML

[T35] Lua：字典表
来源：http://mobile.fktsv.cn/Article/details/gjvihxrti.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.epnwcf.com/Article/details/gsoyvsrfg.sHtML

[T36] Lua：函数
来源：http://mobile.yfazqb.com/Article/details/goyqxsrni.sHtML

function add(a, b) return a + b end
来源：http://m.share.sjlbkw.cn/Article/details/gpiboyycv.sHtML

[T37] Lua：字符串拼接
来源：http://blog.epnwcf.com/Article/details/gquqxmbsw.sHtML

"a" .. "b"
来源：http://www.blog.bbcook.cn/Article/details/ggfkwbltx.sHtML

[T38] Lua：条件
来源：http://www.share.bbcook.cn/Article/details/gvffjmxrg.sHtML

if x > 0 then print("正") end
来源：http://3g.sjlbkw.cn/Article/details/gaotcsbzk.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.epnwcf.com/Article/details/ghqreouks.sHtML

string.find(s, "%d+")
来源：http://wap.fktsv.cn/Article/details/gwvfdcswe.sHtML

[T40] Lua：元表
来源：http://wap.sjlbkw.cn/Article/details/gcpslhuhd.sHtML

setmetatable({}, { __index = base })
来源：http://3g.vehdjk.com/Article/details/ghbcnpqmo.sHtML

[T41] Perl：Hello World
来源：http://wap.epnwcf.com/Article/details/gthzfajer.sHtML

print "Hello\n";
来源：http://m.share.epnwcf.com/Article/details/gfvdlygfe.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.bbcook.cn/Article/details/gynsdpftk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.tarul.cn/Article/details/glcfgpgtg.sHtML

[T43] Perl：字符串插值
来源：http://read.share.tarul.cn/Article/details/gzdszytpu.sHtML

"值: $a"
来源：http://3g.vehdjk.com/Article/details/gjagxorar.sHtML

[T44] Perl：条件
来源：http://wap.epnwcf.com/Article/details/ghyvnvtkv.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.vehdjk.com/Article/details/gxytpnahm.sHtML

[T45] Perl：数组遍历
来源：http://m.share.tarul.cn/Article/details/grtxjtiry.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.bbcook.cn/Article/details/gqjesfcmd.sHtML

[T46] Perl：哈希操作
来源：http://mobile.vehdjk.com/Article/details/gkwrhmavn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.tarul.cn/Article/details/gmrrsayok.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.bbcook.cn/Article/details/greuzwpbl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.yfazqb.com/Article/details/gbyobylpd.sHtML

[T48] Perl：正则替换
来源：http://3g.vehdjk.com/Article/details/glctuppdb.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fktsv.cn/Article/details/gobfumrfi.sHtML

[T49] Perl：函数
来源：http://baike.fktsv.cn/Article/details/gwvhqzbbe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gmnkzmgto.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gaiivwmam.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.vehdjk.com/Article/details/gcwfknjwb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.bbcook.cn/Article/details/gcrzgljon.sHtML

[T51] Scala：Hello World
来源：http://3g.fktsv.cn/Article/details/gwgrstcvf.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/gfsxfhtgr.sHtML

[T52] Scala：变量
来源：http://wap.fktsv.cn/Article/details/giwzcojvt.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fktsv.cn/Article/details/gbtperhyp.sHtML

[T53] Scala：字符串插值
来源：http://wap.vehdjk.com/Article/details/gvxfsxewm.sHtML

s"值: $b"
来源：http://wap.vehdjk.com/Article/details/gcfckxfhj.sHtML

[T54] Scala：集合映射
来源：http://read.share.vehdjk.com/Article/details/glmawltrj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fktsv.cn/Article/details/gqxpwurnj.sHtML

[T55] Scala：集合过滤
来源：http://www.share.bbcook.cn/Article/details/gijtqsupz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.yfazqb.com/Article/details/glapeumse.sHtML

[T56] Scala：样例类
来源：http://read.share.yfazqb.com/Article/details/gpigrwcqg.sHtML

case class User(name: String, age: Int)
来源：http://blog.sjlbkw.cn/Article/details/ggrppmszz.sHtML

[T57] Scala：模式匹配
来源：http://blog.yfazqb.com/Article/details/ggbydyhcx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.yfazqb.com/Article/details/gkzhgkfqx.sHtML

[T58] Scala：函数定义
来源：http://mobile.vehdjk.com/Article/details/grkrmkjdu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.yfazqb.com/Article/details/gcxshrarf.sHtML

[T59] Scala：循环
来源：http://www.share.tarul.cn/Article/details/glwcgcxfv.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.tarul.cn/Article/details/gohmgifxp.sHtML

[T60] Scala：折叠
来源：http://read.share.tarul.cn/Article/details/gjzkegqlo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.bbcook.cn/Article/details/geqyqfeon.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gtcvntyov.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.epnwcf.com/Article/details/gihchxccj.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gshgsoifd.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.sjlbkw.cn/Article/details/givdwkmtu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.yfazqb.com/Article/details/gphijqfee.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.vehdjk.com/Article/details/gfzdsdvkz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.tarul.cn/Article/details/glilmssqt.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.vehdjk.com/Article/details/ghcxnmnbb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.yfazqb.com/Article/details/glbpobsub.sHtML

[U04] Py：变量调试打印
来源：http://mobile.vehdjk.com/Article/details/gwtgxbdyd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.tarul.cn/Article/details/gkourbwda.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.epnwcf.com/Article/details/gqnwdcnop.sHtML

list(dict.fromkeys(arr))
来源：http://wap.vehdjk.com/Article/details/ghjhcnhun.sHtML

[U06] Py：合并两个字典
来源：http://read.share.yfazqb.com/Article/details/ghppcjqvp.sHtML

{**a, **b}
来源：http://m.share.bbcook.cn/Article/details/gycdcrqaz.sHtML

[U07] Py：反转字典键值
来源：http://m.share.vehdjk.com/Article/details/gukzahrvx.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.yfazqb.com/Article/details/gpymjzaii.sHtML

[U08] Py：展平二维列表
来源：http://read.share.tarul.cn/Article/details/gwunafppd.sHtML

[y for x in nested for y in x]
来源：http://baike.vehdjk.com/Article/details/gougzsfkc.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.epnwcf.com/Article/details/gbvlxalom.sHtML

max(d, key=d.get)
来源：http://read.share.vehdjk.com/Article/details/gkwbultvm.sHtML

[U10] Py：按值排序字典
来源：http://wap.sjlbkw.cn/Article/details/gtabbccff.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.epnwcf.com/Article/details/gkwsypoqc.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.vehdjk.com/Article/details/gyiomwbec.sHtML

(x * 2 for x in arr)
来源：http://www.blog.bbcook.cn/Article/details/gbisexchl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.epnwcf.com/Article/details/ghmxubnzm.sHtML

Counter(arr).most_common(3)
来源：http://baike.bbcook.cn/Article/details/gosqrotjs.sHtML

[U13] Py：固定长度队列
来源：http://wap.fktsv.cn/Article/details/glgluxezi.sHtML

deque(maxlen=10)
来源：http://wap.yfazqb.com/Article/details/gtqlsdmnk.sHtML

[U14] Py：分组收集到列表
来源：http://3g.epnwcf.com/Article/details/gsxqybami.sHtML

defaultdict(list)
来源：http://baike.sjlbkw.cn/Article/details/gtfvvcriv.sHtML

[U15] Py：高精度计时
来源：http://www.blog.epnwcf.com/Article/details/gaugidkzr.sHtML

t = time.perf_counter()
来源：http://www.m.share.fktsv.cn/Article/details/gmkfripip.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.tarul.cn/Article/details/gzbdplezb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.yfazqb.com/Article/details/gmcsbbxrb.sHtML

[U17] Py：初始化日志
来源：http://baike.tarul.cn/Article/details/geiwwcfme.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.vehdjk.com/Article/details/gdhldzwsq.sHtML

[U18] Py：预编译正则
来源：http://3g.tarul.cn/Article/details/gwkhcvffd.sHtML

pat = re.compile(r"\d+")
来源：http://blog.vehdjk.com/Article/details/gdptgbqzc.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.epnwcf.com/Article/details/gzqygmzjk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fktsv.cn/Article/details/gjlwzdifj.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fktsv.cn/Article/details/gsrnooglb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fktsv.cn/Article/details/gsgsglarb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fktsv.cn/Article/details/givaheclu.sHtML

@contextlib.contextmanager
来源：http://3g.epnwcf.com/Article/details/gobdgxfjl.sHtML

[U22] Py：矩阵转置
来源：http://blog.fktsv.cn/Article/details/gkezishot.sHtML

list(zip(*m))
来源：http://wap.bbcook.cn/Article/details/gyjnvzbur.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.sjlbkw.cn/Article/details/gkynwuizz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.vehdjk.com/Article/details/gwqjfauru.sHtML

[U24] Py：路径操作
来源：http://read.share.tarul.cn/Article/details/gmvhqsrbz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/guriisyte.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.vehdjk.com/Article/details/gtyztuicc.sHtML

csv.DictReader(f)
来源：http://baike.tarul.cn/Article/details/gccmtdkrw.sHtML

[U26] Py：并发下载
来源：http://www.blog.epnwcf.com/Article/details/gbxzvruan.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.bbcook.cn/Article/details/gnqrtycwe.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.sjlbkw.cn/Article/details/gouvabbdm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.yfazqb.com/Article/details/geagrdjkk.sHtML

[U28] Py：类型别名
来源：http://www.share.vehdjk.com/Article/details/gyjezlalk.sHtML

UserId = int
来源：http://www.blog.tarul.cn/Article/details/gbrddvkxx.sHtML

[U29] Py：属性校验
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcktglzs.sHtML

@property 与 @x.setter 配合
来源：http://wap.vehdjk.com/Article/details/giutkxbdx.sHtML

[U30] Py：数据类
来源：http://read.share.bbcook.cn/Article/details/gafeglkfm.sHtML

@dataclass(slots=True)
来源：http://www.share.yfazqb.com/Article/details/gkhpchypf.sHtML

[U31] Py：单测
来源：http://mobile.epnwcf.com/Article/details/gnvpmnddg.sHtML

python -m pytest -q
来源：http://read.share.fktsv.cn/Article/details/gerftcalu.sHtML

[U32] Py：代码格式化
来源：http://www.share.yfazqb.com/Article/details/gzipdwcuj.sHtML

ruff format . && ruff check --fix .
来源：http://baike.bbcook.cn/Article/details/gmwbwmtfo.sHtML

[U33] Py：打包发布
来源：http://blog.vehdjk.com/Article/details/gjkadnnas.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.bbcook.cn/Article/details/godbrfwie.sHtML

[U34] Py：判断编码
来源：http://www.m.share.epnwcf.com/Article/details/gyurigsns.sHtML

chardet.detect(raw)
来源：http://baike.fktsv.cn/Article/details/geekjmiaf.sHtML

[U35] Py：发送邮件
来源：http://read.share.tarul.cn/Article/details/ggvuoyklg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.vehdjk.com/Article/details/gccsxlnuc.sHtML

[U36] Py：定时任务
来源：http://blog.yfazqb.com/Article/details/gerfsqbol.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.epnwcf.com/Article/details/gvbydbijk.sHtML

[U37] Py：读写 Excel
来源：http://mobile.bbcook.cn/Article/details/gmjwkalax.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.yfazqb.com/Article/details/grvykktow.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.bbcook.cn/Article/details/gdpgchyph.sHtML

Path(__file__).resolve().parent
来源：http://mobile.bbcook.cn/Article/details/godtvuodj.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.tarul.cn/Article/details/goxnvcgck.sHtML

sys.stdout.isatty()
来源：http://www.blog.yfazqb.com/Article/details/gtrlfqzbv.sHtML

[U40] Py：打印到标准错误
来源：http://blog.tarul.cn/Article/details/gnsutrpce.sHtML

print("err", file=sys.stderr)
来源：http://mobile.vehdjk.com/Article/details/gohzmjyhb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.tarul.cn/Article/details/gkekgwwiq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fktsv.cn/Article/details/ggwevrwzt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fktsv.cn/Article/details/gvmjqxrxb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnqnybjx.sHtML

[U43] PHP：声明命名空间
来源：http://3g.epnwcf.com/Article/details/gvuepurvt.sHtML

namespace App\Http;
来源：http://www.blog.sjlbkw.cn/Article/details/gcesosvkr.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.tarul.cn/Article/details/gsoqgvatl.sHtML

declare(strict_types=1);
来源：http://3g.vehdjk.com/Article/details/goyztogvo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.epnwcf.com/Article/details/gsrbvtcpk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/gchddjnbp.sHtML

[U46] PHP：可空类型
来源：http://www.blog.bbcook.cn/Article/details/gbkwwpfqo.sHtML

?string $name = null
来源：http://wap.fktsv.cn/Article/details/gjpahxrgn.sHtML

[U47] PHP：联合类型
来源：http://blog.vehdjk.com/Article/details/gahvkqubn.sHtML

int|string $id
来源：http://m.share.epnwcf.com/Article/details/gvgpzfuxz.sHtML

[U48] PHP：纯枚举
来源：http://m.share.epnwcf.com/Article/details/gwficlrbd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.yfazqb.com/Article/details/gtiokavtw.sHtML

[U49] PHP：只读属性
来源：http://blog.vehdjk.com/Article/details/grbczlmjy.sHtML

public readonly string $name
来源：http://www.m.share.epnwcf.com/Article/details/gsyctffrf.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.tarul.cn/Article/details/gruoilkvc.sHtML

public function __construct(private int $id) {}
来源：http://m.share.epnwcf.com/Article/details/gfecjfxrq.sHtML

[U51] PHP：数组解构
来源：http://3g.yfazqb.com/Article/details/gybntaalb.sHtML

[$a, $b] = $arr;
来源：http://3g.epnwcf.com/Article/details/gwaqitrri.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fktsv.cn/Article/details/gmiqtrtkg.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.vehdjk.com/Article/details/grdtwiwrk.sHtML

[U53] PHP：空合并运算符
来源：http://wap.bbcook.cn/Article/details/ghzgrzvcr.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.sjlbkw.cn/Article/details/ghnegkpeg.sHtML

[U54] PHP：空安全调用
来源：http://www.share.vehdjk.com/Article/details/gokmrzoio.sHtML

$obj?->method()
来源：http://wap.epnwcf.com/Article/details/gnwbzrmrf.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsrbozok.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.sjlbkw.cn/Article/details/gamrpqncv.sHtML

[U56] PHP：命名参数
来源：http://3g.bbcook.cn/Article/details/gyuzoxknj.sHtML

f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/gjpesmoin.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.epnwcf.com/Article/details/gcwxqtxmh.sHtML

"值: {$a}"
来源：http://www.blog.yfazqb.com/Article/details/gangfrtrr.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.bbcook.cn/Article/details/gbkgbuldc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gprfzozyq.sHtML

[U59] PHP：自定义排序
来源：http://3g.bbcook.cn/Article/details/gypxesexb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.tarul.cn/Article/details/gmffvfkvd.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.vehdjk.com/Article/details/gcjfoewhw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.sjlbkw.cn/Article/details/glawdvuax.sHtML

[U61] PHP：正则
来源：http://www.m.share.fktsv.cn/Article/details/gxmuopljb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.epnwcf.com/Article/details/gkwyjqqad.sHtML

[U62] PHP：日期对象
来源：http://www.share.sjlbkw.cn/Article/details/grarpupek.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.bbcook.cn/Article/details/gelriyusy.sHtML

[U63] PHP：文件读写
来源：http://www.share.bbcook.cn/Article/details/gjrxrbxlp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.yfazqb.com/Article/details/gsxazjwvj.sHtML

[U64] PHP：目录遍历
来源：http://read.share.vehdjk.com/Article/details/glrmccvuc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.bbcook.cn/Article/details/gmmqbzqro.sHtML

[U65] PHP：会话
来源：http://3g.vehdjk.com/Article/details/gytvhjhim.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.tarul.cn/Article/details/gbyriexje.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.tarul.cn/Article/details/gzfcinnrx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gpslzotsd.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.vehdjk.com/Article/details/gfzukikgu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.vehdjk.com/Article/details/gpvawafav.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.epnwcf.com/Article/details/gebwehsca.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fktsv.cn/Article/details/gqhmlgbqx.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.sjlbkw.cn/Article/details/gpngswicp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.epnwcf.com/Article/details/gqjxqxwmc.sHtML

[U70] PHP：PDO 事务
来源：http://wap.bbcook.cn/Article/details/gmjieobvj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.epnwcf.com/Article/details/gfmmaplnm.sHtML

[U71] PHP：抛出异常
来源：http://www.share.epnwcf.com/Article/details/gondtpekv.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.tarul.cn/Article/details/gpqmxmalt.sHtML

[U72] PHP：写错误日志
来源：http://www.share.epnwcf.com/Article/details/ghxipinua.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.yfazqb.com/Article/details/ggaumkxhf.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.vehdjk.com/Article/details/gptjozuye.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.sjlbkw.cn/Article/details/glikvawub.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.bbcook.cn/Article/details/gxdjufdgt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.epnwcf.com/Article/details/gmryxrlnu.sHtML


<!-- 参考信息 -->