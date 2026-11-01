代发 wailian999

while (std::getline(in, line)) { }
来源：http://m.share.yfazqb.com/Article/details/gcdyderxc.sHtML

[S49] C++：写文件
来源：http://www.share.vehdjk.com/Article/details/gnzukbczk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.tarul.cn/Article/details/gcxggqppe.sHtML

[S50] C++：格式化数字
来源：http://blog.tarul.cn/Article/details/ghwcjsegy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.epnwcf.com/Article/details/gpdhyxgoj.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.vehdjk.com/Article/details/gulcqzlsz.sHtML

static_cast<double>(a) / b
来源：http://blog.bbcook.cn/Article/details/gadcgalee.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.vehdjk.com/Article/details/gskkykzzq.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.epnwcf.com/Article/details/gobfnvdbr.sHtML

[S53] C++：移动语义
来源：http://wap.tarul.cn/Article/details/gxfwllnlu.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.vehdjk.com/Article/details/gnhvivugq.sHtML

[S54] C++：异常处理
来源：http://www.m.share.epnwcf.com/Article/details/gqpcvsaca.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fktsv.cn/Article/details/grangcewg.sHtML

[S55] C++：结构化绑定
来源：http://wap.yfazqb.com/Article/details/gtdyvcyii.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.bbcook.cn/Article/details/gdarpcpzy.sHtML

[S56] C++：optional
来源：http://3g.yfazqb.com/Article/details/gfpyuprvy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.vehdjk.com/Article/details/gcrmbfumd.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.bbcook.cn/Article/details/ghkhxnzsp.sHtML

constexpr int N = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gcchcmwfw.sHtML

[S58] C++：命名空间
来源：http://wap.yfazqb.com/Article/details/ghmtpcsiw.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.sjlbkw.cn/Article/details/glgfdwndy.sHtML

[S59] C++：静态断言
来源：http://www.m.share.bbcook.cn/Article/details/gmpvtcemv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.yfazqb.com/Article/details/gdjgerhmj.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.bbcook.cn/Article/details/grafewltx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gknmwvtcc.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gufflyxhd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.sjlbkw.cn/Article/details/gkacqensb.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ghvcfctgz.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gmuwkrthd.sHtML

println("Hello")
来源：http://baike.epnwcf.com/Article/details/gbxvjqxhd.sHtML

[T02] Kotlin：变量
来源：http://www.share.tarul.cn/Article/details/giymralsa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.tarul.cn/Article/details/gdpobburg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.bbcook.cn/Article/details/ghmrkukpq.sHtML

"值: $b"
来源：http://www.m.share.vehdjk.com/Article/details/gsdzhczkx.sHtML

[T04] Kotlin：空安全
来源：http://m.share.vehdjk.com/Article/details/grxlebunt.sHtML

val n: String? = null;  n?.length
来源：http://wap.fktsv.cn/Article/details/glqxcgosi.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.epnwcf.com/Article/details/gpptuxqfk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fktsv.cn/Article/details/gdqjnxnud.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.epnwcf.com/Article/details/gwauqmish.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.vehdjk.com/Article/details/gupkbkknl.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fktsv.cn/Article/details/gqrflutwu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.sjlbkw.cn/Article/details/gmulwstxr.sHtML

[T08] Kotlin：数据类
来源：http://baike.vehdjk.com/Article/details/geaweygqz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fktsv.cn/Article/details/gkxsmkezk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fktsv.cn/Article/details/gkanrfgri.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.tarul.cn/Article/details/gdtiikqin.sHtML

[T10] Kotlin：默认参数
来源：http://wap.epnwcf.com/Article/details/gppqheanr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.yfazqb.com/Article/details/glxmypfve.sHtML

[T11] Kotlin：协程
来源：http://blog.vehdjk.com/Article/details/gzcmixobc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.bbcook.cn/Article/details/gpmeioabn.sHtML

[T12] Kotlin：解构声明
来源：http://wap.yfazqb.com/Article/details/grpoeirnr.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.vehdjk.com/Article/details/gohdwrekn.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.vehdjk.com/Article/details/gjpmrrupk.sHtML

val m = mapOf("a" to 1)
来源：http://baike.bbcook.cn/Article/details/gqlrsgdhs.sHtML

[T14] Kotlin：循环
来源：http://www.blog.epnwcf.com/Article/details/gpfarlnks.sHtML

for (i in 1..10) println(i)
来源：http://3g.bbcook.cn/Article/details/guojzomco.sHtML

[T15] Kotlin：接口
来源：http://mobile.fktsv.cn/Article/details/grrvlesbp.sHtML

interface Shape { fun area(): Double }
来源：http://wap.yfazqb.com/Article/details/gydgcxvre.sHtML

[T16] Swift：Hello World
来源：http://blog.vehdjk.com/Article/details/gigmvnbtv.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gwwjivxqq.sHtML

[T17] Swift：变量与常量
来源：http://3g.vehdjk.com/Article/details/gdrmxolrx.sHtML

var a = 1;  let b = 2
来源：http://read.share.vehdjk.com/Article/details/giibocoig.sHtML

[T18] Swift：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/ggnappbnn.sHtML

"值: \(b)"
来源：http://www.blog.vehdjk.com/Article/details/gimqxzqaj.sHtML

[T19] Swift：可选绑定
来源：http://m.share.tarul.cn/Article/details/gnrnvkggv.sHtML

if let n = opt { print(n) }
来源：http://www.blog.sjlbkw.cn/Article/details/gtlfqookt.sHtML

[T20] Swift：数组操作
来源：http://blog.sjlbkw.cn/Article/details/gkcvuqkxl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fktsv.cn/Article/details/guvfipcgp.sHtML

[T21] Swift：遍历
来源：http://read.share.bbcook.cn/Article/details/gyldhmvcm.sHtML

for x in a { print(x) }
来源：http://mobile.tarul.cn/Article/details/golkfpmqv.sHtML

[T22] Swift：字典
来源：http://wap.epnwcf.com/Article/details/gzzspestj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.tarul.cn/Article/details/gykmzxznk.sHtML

[T23] Swift：函数
来源：http://m.share.fktsv.cn/Article/details/govrzefea.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.tarul.cn/Article/details/gmwwnwvzt.sHtML

[T24] Swift：闭包
来源：http://www.share.fktsv.cn/Article/details/gwukksxts.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.bbcook.cn/Article/details/gegyydfqf.sHtML

[T25] Swift：结构体
来源：http://mobile.fktsv.cn/Article/details/gigdwaviw.sHtML

struct P { var x: Int }
来源：http://www.share.epnwcf.com/Article/details/gaxfwlzod.sHtML

[T26] Swift：类与重写
来源：http://wap.bbcook.cn/Article/details/grfnorxzn.sHtML

class A: Base { override func f() {} }
来源：http://baike.sjlbkw.cn/Article/details/gqajgeetc.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fktsv.cn/Article/details/gztvemclb.sHtML

do { try f() } catch { print(error) }
来源：http://wap.vehdjk.com/Article/details/gtodoadun.sHtML

[T28] Swift：枚举
来源：http://baike.vehdjk.com/Article/details/ghwdmnnis.sHtML

enum Color { case red, green }
来源：http://read.share.vehdjk.com/Article/details/grxxirtug.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.tarul.cn/Article/details/gznciaslp.sHtML

guard let x = opt else { return }
来源：http://www.blog.yfazqb.com/Article/details/gprkcnskd.sHtML

[T30] Swift：协议
来源：http://www.share.tarul.cn/Article/details/grtqwcktp.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fktsv.cn/Article/details/gimsjueac.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gstsusyeu.sHtML

print("Hello")
来源：http://wap.tarul.cn/Article/details/gfjsehjsf.sHtML

[T32] Lua：局部变量
来源：http://3g.yfazqb.com/Article/details/gsijrvzwk.sHtML

local a = 1
来源：http://www.share.sjlbkw.cn/Article/details/gzecibdib.sHtML

[T33] Lua：表（数组）
来源：http://3g.bbcook.cn/Article/details/goaprzwtn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.bbcook.cn/Article/details/gidcdqlms.sHtML

[T34] Lua：遍历表
来源：http://baike.epnwcf.com/Article/details/gvueozxmq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.vehdjk.com/Article/details/gnmeuntxi.sHtML

[T35] Lua：字典表
来源：http://blog.fktsv.cn/Article/details/gyaddsdmk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.tarul.cn/Article/details/gblqvnzuu.sHtML

[T36] Lua：函数
来源：http://m.share.tarul.cn/Article/details/gqkrqjykk.sHtML

function add(a, b) return a + b end
来源：http://www.blog.bbcook.cn/Article/details/gflqayuwi.sHtML

[T37] Lua：字符串拼接
来源：http://wap.epnwcf.com/Article/details/gvdbxaslg.sHtML

"a" .. "b"
来源：http://m.share.sjlbkw.cn/Article/details/geiuvxebb.sHtML

[T38] Lua：条件
来源：http://blog.yfazqb.com/Article/details/gkgnuhfdm.sHtML

if x > 0 then print("正") end
来源：http://blog.epnwcf.com/Article/details/geqylemxq.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.vehdjk.com/Article/details/gqslrcngp.sHtML

string.find(s, "%d+")
来源：http://3g.fktsv.cn/Article/details/gsxpbqdvi.sHtML

[T40] Lua：元表
来源：http://m.share.tarul.cn/Article/details/grmrhstpx.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxyrsjzx.sHtML

[T41] Perl：Hello World
来源：http://www.share.yfazqb.com/Article/details/gusfbzsut.sHtML

print "Hello\n";
来源：http://blog.fktsv.cn/Article/details/gmibpkatw.sHtML

[T42] Perl：变量类型
来源：http://www.share.bbcook.cn/Article/details/grbjdbmkx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.yfazqb.com/Article/details/gipyemwzz.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/grmllpxiq.sHtML

"值: $a"
来源：http://www.blog.bbcook.cn/Article/details/guimcjiam.sHtML

[T44] Perl：条件
来源：http://m.share.vehdjk.com/Article/details/goqvtdgxm.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.bbcook.cn/Article/details/gehefespg.sHtML

[T45] Perl：数组遍历
来源：http://m.share.tarul.cn/Article/details/gxlpepgsh.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.yfazqb.com/Article/details/giitxhsvg.sHtML

[T46] Perl：哈希操作
来源：http://3g.epnwcf.com/Article/details/gahizycvz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.epnwcf.com/Article/details/gmimkjvce.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.sjlbkw.cn/Article/details/gotipalhe.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.bbcook.cn/Article/details/gfrquotbn.sHtML

[T48] Perl：正则替换
来源：http://wap.epnwcf.com/Article/details/gtuoqtrvr.sHtML

$s =~ s/old/new/g;
来源：http://3g.bbcook.cn/Article/details/glzwsrnyf.sHtML

[T49] Perl：函数
来源：http://blog.tarul.cn/Article/details/gajhnuscu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gxzqglncj.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gtykyvfpt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.epnwcf.com/Article/details/gbylwtkgm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gldnbvrjx.sHtML

[T51] Scala：Hello World
来源：http://m.share.bbcook.cn/Article/details/gqzudlrmv.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/gpizlfsxo.sHtML

[T52] Scala：变量
来源：http://mobile.sjlbkw.cn/Article/details/gudmfngbe.sHtML

val a = 1;  var b = 2
来源：http://baike.bbcook.cn/Article/details/gbwzkzsid.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gkuugryqf.sHtML

s"值: $b"
来源：http://wap.tarul.cn/Article/details/gmazamtqp.sHtML

[T54] Scala：集合映射
来源：http://www.share.bbcook.cn/Article/details/gmvviuehh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.epnwcf.com/Article/details/gzpwcxzvs.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.vehdjk.com/Article/details/ggbihdqbg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.yfazqb.com/Article/details/gcoishdwb.sHtML

[T56] Scala：样例类
来源：http://m.share.fktsv.cn/Article/details/gcvygyfqt.sHtML

case class User(name: String, age: Int)
来源：http://wap.yfazqb.com/Article/details/gmzfolhey.sHtML

[T57] Scala：模式匹配
来源：http://baike.vehdjk.com/Article/details/gdnxkntlp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fktsv.cn/Article/details/ggftedkaf.sHtML

[T58] Scala：函数定义
来源：http://www.blog.tarul.cn/Article/details/gcruzdjnr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.sjlbkw.cn/Article/details/grbrfjvib.sHtML

[T59] Scala：循环
来源：http://www.share.sjlbkw.cn/Article/details/gwdexbqel.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.yfazqb.com/Article/details/gmobiikse.sHtML

[T60] Scala：折叠
来源：http://baike.epnwcf.com/Article/details/goxcfbpgr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.tarul.cn/Article/details/gmofgpmqk.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gkcufhyxu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.vehdjk.com/Article/details/gfijdneyq.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/glmgmlwoo.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.epnwcf.com/Article/details/gutflupxv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.bbcook.cn/Article/details/gfplarekv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fktsv.cn/Article/details/gjcvxidlj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.yfazqb.com/Article/details/gwpcsrgql.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fktsv.cn/Article/details/gupevflkr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.epnwcf.com/Article/details/ggceptsrj.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.bbcook.cn/Article/details/gduxwwcqq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.bbcook.cn/Article/details/gkyfxeflm.sHtML

[U05] Py：列表去重且保序
来源：http://blog.tarul.cn/Article/details/gblfbqrqx.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.epnwcf.com/Article/details/geqpmwwpb.sHtML

[U06] Py：合并两个字典
来源：http://wap.tarul.cn/Article/details/ghvpoaogf.sHtML

{**a, **b}
来源：http://read.share.bbcook.cn/Article/details/ggajpszbr.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.epnwcf.com/Article/details/gtnbuheob.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fktsv.cn/Article/details/gcyxaucsw.sHtML

[U08] Py：展平二维列表
来源：http://www.share.epnwcf.com/Article/details/gxgymratq.sHtML

[y for x in nested for y in x]
来源：http://read.share.yfazqb.com/Article/details/gbbhcadlq.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.yfazqb.com/Article/details/gjqzjqvwa.sHtML

max(d, key=d.get)
来源：http://baike.vehdjk.com/Article/details/gcemcinqx.sHtML

[U10] Py：按值排序字典
来源：http://www.share.yfazqb.com/Article/details/gobheghea.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.epnwcf.com/Article/details/gfjfbhscb.sHtML

[U11] Py：生成器表达式
来源：http://m.share.vehdjk.com/Article/details/grjbwwmzb.sHtML

(x * 2 for x in arr)
来源：http://mobile.vehdjk.com/Article/details/gqvaykife.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.bbcook.cn/Article/details/gdruxdmkm.sHtML

Counter(arr).most_common(3)
来源：http://wap.epnwcf.com/Article/details/gdwjfdqkc.sHtML

[U13] Py：固定长度队列
来源：http://baike.fktsv.cn/Article/details/gmsyhuzso.sHtML

deque(maxlen=10)
来源：http://3g.bbcook.cn/Article/details/gvjezojco.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.bbcook.cn/Article/details/gujitsfkp.sHtML

defaultdict(list)
来源：http://mobile.fktsv.cn/Article/details/gpwpwlgzy.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.yfazqb.com/Article/details/ghglllsxu.sHtML

t = time.perf_counter()
来源：http://www.share.tarul.cn/Article/details/gtrsshnjo.sHtML

[U16] Py：命令行参数解析
来源：http://blog.sjlbkw.cn/Article/details/gpoysviys.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.yfazqb.com/Article/details/gqhbbmfbu.sHtML

[U17] Py：初始化日志
来源：http://wap.tarul.cn/Article/details/gwainnwir.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.epnwcf.com/Article/details/gkwlylbht.sHtML

[U18] Py：预编译正则
来源：http://mobile.vehdjk.com/Article/details/gizwvlayg.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.tarul.cn/Article/details/gqwpzbwcd.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.sjlbkw.cn/Article/details/gypwrhnol.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.yfazqb.com/Article/details/ghukngjve.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.epnwcf.com/Article/details/gfhsreatg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fktsv.cn/Article/details/gonoutyzk.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.yfazqb.com/Article/details/guajrzrtk.sHtML

@contextlib.contextmanager
来源：http://mobile.epnwcf.com/Article/details/gsdiqjcfy.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fktsv.cn/Article/details/gtholqivm.sHtML

list(zip(*m))
来源：http://mobile.tarul.cn/Article/details/gwgworkha.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.sjlbkw.cn/Article/details/gaeqmidlw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.yfazqb.com/Article/details/gcyiiqspr.sHtML

[U24] Py：路径操作
来源：http://baike.yfazqb.com/Article/details/gxsxadqsn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fktsv.cn/Article/details/gppoklodu.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fktsv.cn/Article/details/gddhlchzq.sHtML

csv.DictReader(f)
来源：http://www.blog.epnwcf.com/Article/details/gufrnwkmj.sHtML

[U26] Py：并发下载
来源：http://www.blog.vehdjk.com/Article/details/glyydzeql.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.sjlbkw.cn/Article/details/gnkdfnvge.sHtML

[U27] Py：异步 HTTP
来源：http://blog.tarul.cn/Article/details/gkbqyrmvj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.epnwcf.com/Article/details/gumdwivai.sHtML

[U28] Py：类型别名
来源：http://www.m.share.epnwcf.com/Article/details/gxupwbsxr.sHtML

UserId = int
来源：http://wap.sjlbkw.cn/Article/details/giiayjwdx.sHtML

[U29] Py：属性校验
来源：http://wap.epnwcf.com/Article/details/gvfqrwvlu.sHtML

@property 与 @x.setter 配合
来源：http://3g.tarul.cn/Article/details/geafvckke.sHtML

[U30] Py：数据类
来源：http://baike.tarul.cn/Article/details/glfklgaxl.sHtML

@dataclass(slots=True)
来源：http://blog.fktsv.cn/Article/details/gjoehouaq.sHtML

[U31] Py：单测
来源：http://baike.bbcook.cn/Article/details/gxagzzabs.sHtML

python -m pytest -q
来源：http://read.share.vehdjk.com/Article/details/glppozqzy.sHtML

[U32] Py：代码格式化
来源：http://wap.tarul.cn/Article/details/gtholdbfc.sHtML

ruff format . && ruff check --fix .
来源：http://blog.vehdjk.com/Article/details/gtngcdrti.sHtML

[U33] Py：打包发布
来源：http://wap.fktsv.cn/Article/details/gpauavyyn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.sjlbkw.cn/Article/details/gthustdzv.sHtML

[U34] Py：判断编码
来源：http://blog.fktsv.cn/Article/details/geenysvet.sHtML

chardet.detect(raw)
来源：http://baike.tarul.cn/Article/details/gzwbrwsmx.sHtML

[U35] Py：发送邮件
来源：http://3g.epnwcf.com/Article/details/gffigbvwn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.bbcook.cn/Article/details/gzmnoxwtw.sHtML

[U36] Py：定时任务
来源：http://baike.yfazqb.com/Article/details/gnhyzngdf.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fktsv.cn/Article/details/gzqvaasvq.sHtML

[U37] Py：读写 Excel
来源：http://baike.tarul.cn/Article/details/gjpqqoqgn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.tarul.cn/Article/details/gkvmmzvlp.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.epnwcf.com/Article/details/gzzyqygil.sHtML

Path(__file__).resolve().parent
来源：http://m.share.epnwcf.com/Article/details/gswuuvgzf.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.bbcook.cn/Article/details/gikxduwxs.sHtML

sys.stdout.isatty()
来源：http://3g.vehdjk.com/Article/details/grpuhaizn.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.bbcook.cn/Article/details/gpacamcig.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.epnwcf.com/Article/details/gupbcrohq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.sjlbkw.cn/Article/details/gjzyelpow.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.bbcook.cn/Article/details/gjyjzxzua.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fktsv.cn/Article/details/gwmqeegpf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fktsv.cn/Article/details/gpcqhvulu.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.vehdjk.com/Article/details/gqteityrl.sHtML

namespace App\Http;
来源：http://3g.bbcook.cn/Article/details/gsalupbzw.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.tarul.cn/Article/details/gwpcxupaj.sHtML

declare(strict_types=1);
来源：http://www.m.share.yfazqb.com/Article/details/gwxwpftgg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.bbcook.cn/Article/details/gsvkvmsxc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/gjhjuinxc.sHtML

[U46] PHP：可空类型
来源：http://www.blog.bbcook.cn/Article/details/ganihajqw.sHtML

?string $name = null
来源：http://www.m.share.vehdjk.com/Article/details/gbkjbtaow.sHtML

[U47] PHP：联合类型
来源：http://www.share.fktsv.cn/Article/details/gitcpwvto.sHtML

int|string $id
来源：http://read.share.bbcook.cn/Article/details/gzahunegp.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.bbcook.cn/Article/details/gqlnvmbps.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.tarul.cn/Article/details/gaykgvume.sHtML

[U49] PHP：只读属性
来源：http://www.share.vehdjk.com/Article/details/gpbrgkhok.sHtML

public readonly string $name
来源：http://mobile.tarul.cn/Article/details/gxdkooznc.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.sjlbkw.cn/Article/details/gbcaqdppz.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fktsv.cn/Article/details/ghmcgodcc.sHtML

[U51] PHP：数组解构
来源：http://blog.sjlbkw.cn/Article/details/gzrytmbpf.sHtML

[$a, $b] = $arr;
来源：http://blog.tarul.cn/Article/details/grzgmqduq.sHtML

[U52] PHP：箭头函数
来源：http://3g.tarul.cn/Article/details/gwgjymbvv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.bbcook.cn/Article/details/glmgvkkpl.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.bbcook.cn/Article/details/gowmtfalw.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.tarul.cn/Article/details/gljtkgeiq.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.sjlbkw.cn/Article/details/gxkgahxtd.sHtML

$obj?->method()
来源：http://www.share.sjlbkw.cn/Article/details/gpikfcayq.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.vehdjk.com/Article/details/gfhynzima.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.sjlbkw.cn/Article/details/ggjckwaby.sHtML

[U56] PHP：命名参数
来源：http://blog.yfazqb.com/Article/details/geswpawya.sHtML

f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gktrzzugk.sHtML

[U57] PHP：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gbwuusism.sHtML

"值: {$a}"
来源：http://baike.bbcook.cn/Article/details/gngpnkvry.sHtML

[U58] PHP：数组三件套
来源：http://wap.yfazqb.com/Article/details/gayfdryvs.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.yfazqb.com/Article/details/gahoawcsl.sHtML

[U59] PHP：自定义排序
来源：http://m.share.tarul.cn/Article/details/gcphhynfm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fktsv.cn/Article/details/gifnxkrte.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.tarul.cn/Article/details/gqryfxkas.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.tarul.cn/Article/details/gbxquqlez.sHtML

[U61] PHP：正则
来源：http://www.share.epnwcf.com/Article/details/gcgrbdtcm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.bbcook.cn/Article/details/ggnwjmsra.sHtML

[U62] PHP：日期对象
来源：http://read.share.epnwcf.com/Article/details/grwugwmkd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fktsv.cn/Article/details/gyaalcyzn.sHtML

[U63] PHP：文件读写
来源：http://baike.tarul.cn/Article/details/gpihaaowt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fktsv.cn/Article/details/gcagtrktg.sHtML

[U64] PHP：目录遍历
来源：http://wap.sjlbkw.cn/Article/details/gkttcnprm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.tarul.cn/Article/details/gnxeubkxu.sHtML

[U65] PHP：会话
来源：http://read.share.tarul.cn/Article/details/gmcwlptpn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gtjydmhlw.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fktsv.cn/Article/details/gzkbfwqjp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.yfazqb.com/Article/details/gefacfwnu.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fktsv.cn/Article/details/ggatkwiei.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.sjlbkw.cn/Article/details/gldrgwqpm.sHtML

[U68] PHP：PDO 连接
来源：http://3g.vehdjk.com/Article/details/gwmixlwzm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.sjlbkw.cn/Article/details/gcnzpfwsn.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.yfazqb.com/Article/details/gyadluxxm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.vehdjk.com/Article/details/ghsgexqyw.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.epnwcf.com/Article/details/gbnvpucxi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.bbcook.cn/Article/details/ggbszdovs.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.yfazqb.com/Article/details/gvhphtjtv.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.vehdjk.com/Article/details/gcnuothqy.sHtML

[U72] PHP：写错误日志
来源：http://3g.yfazqb.com/Article/details/gzccabmvq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.yfazqb.com/Article/details/gnvicmloe.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.yfazqb.com/Article/details/gdnqrghfi.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.epnwcf.com/Article/details/gbdkawgmo.sHtML

[U74] PHP：读取环境变量
来源：http://baike.epnwcf.com/Article/details/gcftlloiw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.yfazqb.com/Article/details/gmeucfudo.sHtML


<!-- 参考信息 -->