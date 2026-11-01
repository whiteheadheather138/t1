代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://mobile.bbcook.cn/Article/details/gomifrxiz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.tarul.cn/Article/details/gdyozmxcu.sHtML

[S48] C++：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gqseiqwfp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.vehdjk.com/Article/details/gvmnjtvch.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.yfazqb.com/Article/details/gldsizjwq.sHtML

[S49] C++：写文件
来源：http://3g.yfazqb.com/Article/details/gvrwbusul.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.epnwcf.com/Article/details/gxkiuoppk.sHtML

[S50] C++：格式化数字
来源：http://read.share.epnwcf.com/Article/details/gbrfrhuur.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gbyxrdylu.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.tarul.cn/Article/details/gjdskeqlj.sHtML

static_cast<double>(a) / b
来源：http://baike.bbcook.cn/Article/details/geghdtlva.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.tarul.cn/Article/details/gyaprgezp.sHtML

int size() const noexcept { return n_; }
来源：http://wap.vehdjk.com/Article/details/gsdirzgcz.sHtML

[S53] C++：移动语义
来源：http://www.share.bbcook.cn/Article/details/gejnklgtp.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.bbcook.cn/Article/details/gtemazkmg.sHtML

[S54] C++：异常处理
来源：http://3g.epnwcf.com/Article/details/glqleavjb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.bbcook.cn/Article/details/gygxunqot.sHtML

[S55] C++：结构化绑定
来源：http://wap.vehdjk.com/Article/details/gtkckamgv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fktsv.cn/Article/details/ghnjhvscz.sHtML

[S56] C++：optional
来源：http://www.blog.sjlbkw.cn/Article/details/gmnzxyday.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.bbcook.cn/Article/details/gxltdbyfc.sHtML

[S57] C++：编译期常量
来源：http://read.share.vehdjk.com/Article/details/ghmjtalyf.sHtML

constexpr int N = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtplendfq.sHtML

[S58] C++：命名空间
来源：http://blog.sjlbkw.cn/Article/details/gjavhedvp.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.tarul.cn/Article/details/gmuiundpy.sHtML

[S59] C++：静态断言
来源：http://read.share.epnwcf.com/Article/details/gkremigko.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.bbcook.cn/Article/details/gleaqfios.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.vehdjk.com/Article/details/gzlmkwyku.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.bbcook.cn/Article/details/gqjhqpzag.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/grnpglutb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.bbcook.cn/Article/details/gocmebool.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gxwqayhcr.sHtML

[T01] Kotlin：Hello World
来源：http://3g.bbcook.cn/Article/details/gcsklfilo.sHtML

println("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/ghnmysnbh.sHtML

[T02] Kotlin：变量
来源：http://wap.sjlbkw.cn/Article/details/gpszhuukc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.vehdjk.com/Article/details/gwxfhvmgn.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.epnwcf.com/Article/details/gbkshzmed.sHtML

"值: $b"
来源：http://www.share.tarul.cn/Article/details/gquylrcjn.sHtML

[T04] Kotlin：空安全
来源：http://baike.epnwcf.com/Article/details/godrcdkmm.sHtML

val n: String? = null;  n?.length
来源：http://mobile.vehdjk.com/Article/details/gmfltyzpi.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gujswkhha.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.tarul.cn/Article/details/gdnqfnbim.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fktsv.cn/Article/details/gapvvddyi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fktsv.cn/Article/details/ggiapjubi.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.epnwcf.com/Article/details/gkgfwtmzy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.bbcook.cn/Article/details/gpgcvkygd.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.vehdjk.com/Article/details/gkupgjirj.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fktsv.cn/Article/details/grtkbipzr.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.vehdjk.com/Article/details/gzsrdxhpw.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.tarul.cn/Article/details/gbmmdhccy.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.sjlbkw.cn/Article/details/gsgcmmbmp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fktsv.cn/Article/details/grsokefic.sHtML

[T11] Kotlin：协程
来源：http://mobile.bbcook.cn/Article/details/gvzmravpc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.epnwcf.com/Article/details/gxhjqcwrf.sHtML

[T12] Kotlin：解构声明
来源：http://3g.tarul.cn/Article/details/glnewagqz.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.yfazqb.com/Article/details/gwtualjhj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.bbcook.cn/Article/details/gbqplpsnx.sHtML

val m = mapOf("a" to 1)
来源：http://blog.tarul.cn/Article/details/glylutbbb.sHtML

[T14] Kotlin：循环
来源：http://blog.vehdjk.com/Article/details/gouhzwxke.sHtML

for (i in 1..10) println(i)
来源：http://mobile.bbcook.cn/Article/details/girxvplcn.sHtML

[T15] Kotlin：接口
来源：http://blog.yfazqb.com/Article/details/gnledrwzh.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.tarul.cn/Article/details/gofveckgq.sHtML

[T16] Swift：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gsxkkcfat.sHtML

print("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/gopnphcwc.sHtML

[T17] Swift：变量与常量
来源：http://blog.fktsv.cn/Article/details/gdmmjapzl.sHtML

var a = 1;  let b = 2
来源：http://www.blog.tarul.cn/Article/details/gubbfhasi.sHtML

[T18] Swift：字符串插值
来源：http://www.share.tarul.cn/Article/details/gaotuadna.sHtML

"值: \(b)"
来源：http://3g.tarul.cn/Article/details/giwshvact.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.bbcook.cn/Article/details/gslqmbjce.sHtML

if let n = opt { print(n) }
来源：http://3g.fktsv.cn/Article/details/ghowuxmvs.sHtML

[T20] Swift：数组操作
来源：http://read.share.epnwcf.com/Article/details/gedmlpgvv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.vehdjk.com/Article/details/geahglxie.sHtML

[T21] Swift：遍历
来源：http://www.blog.yfazqb.com/Article/details/gxqdtogjq.sHtML

for x in a { print(x) }
来源：http://www.share.bbcook.cn/Article/details/gcpsaskgj.sHtML

[T22] Swift：字典
来源：http://m.share.bbcook.cn/Article/details/gxegrmpfp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.yfazqb.com/Article/details/gwigkbtvw.sHtML

[T23] Swift：函数
来源：http://m.share.epnwcf.com/Article/details/gmberxleo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.tarul.cn/Article/details/gsgpglexx.sHtML

[T24] Swift：闭包
来源：http://3g.bbcook.cn/Article/details/gpyklcumw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fktsv.cn/Article/details/grlckcdih.sHtML

[T25] Swift：结构体
来源：http://www.share.tarul.cn/Article/details/gzormyvpf.sHtML

struct P { var x: Int }
来源：http://baike.fktsv.cn/Article/details/gwfpsmxef.sHtML

[T26] Swift：类与重写
来源：http://www.blog.bbcook.cn/Article/details/gigmmkxfe.sHtML

class A: Base { override func f() {} }
来源：http://read.share.vehdjk.com/Article/details/gzbvjpogi.sHtML

[T27] Swift：错误处理
来源：http://read.share.epnwcf.com/Article/details/ggycyughs.sHtML

do { try f() } catch { print(error) }
来源：http://blog.vehdjk.com/Article/details/gmoxsmsul.sHtML

[T28] Swift：枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gocuuaahc.sHtML

enum Color { case red, green }
来源：http://baike.yfazqb.com/Article/details/gneidhqzr.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fktsv.cn/Article/details/gnjuxeeyx.sHtML

guard let x = opt else { return }
来源：http://www.share.fktsv.cn/Article/details/gwvhxcuol.sHtML

[T30] Swift：协议
来源：http://3g.bbcook.cn/Article/details/gorboiebf.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.bbcook.cn/Article/details/ghjucbosf.sHtML

[T31] Lua：Hello World
来源：http://mobile.bbcook.cn/Article/details/gggqmwvkr.sHtML

print("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkyoviysi.sHtML

[T32] Lua：局部变量
来源：http://wap.yfazqb.com/Article/details/gronvjmke.sHtML

local a = 1
来源：http://www.blog.epnwcf.com/Article/details/glmasccdp.sHtML

[T33] Lua：表（数组）
来源：http://wap.vehdjk.com/Article/details/gkvxfwnbk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.bbcook.cn/Article/details/gscjjwkyw.sHtML

[T34] Lua：遍历表
来源：http://www.share.fktsv.cn/Article/details/gxpuwzmgg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.yfazqb.com/Article/details/gjbucmxqr.sHtML

[T35] Lua：字典表
来源：http://baike.fktsv.cn/Article/details/gmgqwauau.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.tarul.cn/Article/details/gsyonsorq.sHtML

[T36] Lua：函数
来源：http://m.share.fktsv.cn/Article/details/gblelgedf.sHtML

function add(a, b) return a + b end
来源：http://www.share.yfazqb.com/Article/details/gvqdeiwro.sHtML

[T37] Lua：字符串拼接
来源：http://wap.epnwcf.com/Article/details/gpjbjimhx.sHtML

"a" .. "b"
来源：http://wap.epnwcf.com/Article/details/gspttozaa.sHtML

[T38] Lua：条件
来源：http://www.share.yfazqb.com/Article/details/gohsnhbmw.sHtML

if x > 0 then print("正") end
来源：http://baike.vehdjk.com/Article/details/gnhxxerij.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/guyqwiaop.sHtML

string.find(s, "%d+")
来源：http://read.share.tarul.cn/Article/details/gzlmtjboj.sHtML

[T40] Lua：元表
来源：http://www.share.yfazqb.com/Article/details/gnonubucq.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.yfazqb.com/Article/details/gtilzlgnp.sHtML

[T41] Perl：Hello World
来源：http://read.share.tarul.cn/Article/details/gizlgihho.sHtML

print "Hello\n";
来源：http://wap.sjlbkw.cn/Article/details/gjwjxwvhl.sHtML

[T42] Perl：变量类型
来源：http://3g.vehdjk.com/Article/details/godnkhati.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.bbcook.cn/Article/details/gbdynuvaj.sHtML

[T43] Perl：字符串插值
来源：http://baike.fktsv.cn/Article/details/ggakyrspi.sHtML

"值: $a"
来源：http://read.share.epnwcf.com/Article/details/gxrsaezhu.sHtML

[T44] Perl：条件
来源：http://www.m.share.yfazqb.com/Article/details/grzkphmpn.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.yfazqb.com/Article/details/gfxigikxz.sHtML

[T45] Perl：数组遍历
来源：http://blog.tarul.cn/Article/details/gihrbyted.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fktsv.cn/Article/details/gnjwwmpff.sHtML

[T46] Perl：哈希操作
来源：http://mobile.tarul.cn/Article/details/gujwngchv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.bbcook.cn/Article/details/gaisqjron.sHtML

[T47] Perl：正则捕获
来源：http://read.share.tarul.cn/Article/details/gbapmpero.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.epnwcf.com/Article/details/gqpsuaqzs.sHtML

[T48] Perl：正则替换
来源：http://www.blog.tarul.cn/Article/details/ggtrhgvwk.sHtML

$s =~ s/old/new/g;
来源：http://read.share.sjlbkw.cn/Article/details/gdrqnpuhi.sHtML

[T49] Perl：函数
来源：http://www.share.fktsv.cn/Article/details/gkvyaztrd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.tarul.cn/Article/details/gxcwiuxny.sHtML

[T50] Perl：逐行读文件
来源：http://blog.epnwcf.com/Article/details/glkyspdti.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fktsv.cn/Article/details/gjbybaeox.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.bbcook.cn/Article/details/gaiizypzs.sHtML

[T51] Scala：Hello World
来源：http://wap.vehdjk.com/Article/details/gnekipxva.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/gabkfmkpc.sHtML

[T52] Scala：变量
来源：http://3g.yfazqb.com/Article/details/gscmiosec.sHtML

val a = 1;  var b = 2
来源：http://mobile.fktsv.cn/Article/details/gqccureeq.sHtML

[T53] Scala：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gbcoaspuk.sHtML

s"值: $b"
来源：http://wap.epnwcf.com/Article/details/ghpbgksko.sHtML

[T54] Scala：集合映射
来源：http://m.share.epnwcf.com/Article/details/gzytqhzas.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gktskkxso.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.vehdjk.com/Article/details/gcqxevkjw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.tarul.cn/Article/details/gczgvkjcq.sHtML

[T56] Scala：样例类
来源：http://m.share.fktsv.cn/Article/details/gjlpahfph.sHtML

case class User(name: String, age: Int)
来源：http://baike.bbcook.cn/Article/details/gccevyfpn.sHtML

[T57] Scala：模式匹配
来源：http://3g.vehdjk.com/Article/details/geuatjcju.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.bbcook.cn/Article/details/gzfhjtiyp.sHtML

[T58] Scala：函数定义
来源：http://www.share.sjlbkw.cn/Article/details/gxdlvbyfu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.yfazqb.com/Article/details/gpxxtcjec.sHtML

[T59] Scala：循环
来源：http://www.share.fktsv.cn/Article/details/gityaqyva.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.yfazqb.com/Article/details/gfkowneon.sHtML

[T60] Scala：折叠
来源：http://wap.vehdjk.com/Article/details/gsqxmuzov.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.vehdjk.com/Article/details/gvpanlsyw.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gjzrosfgw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.sjlbkw.cn/Article/details/gqsyarqkz.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gvoktlxtl.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.bbcook.cn/Article/details/glrkgfqfa.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.bbcook.cn/Article/details/goyvmquvx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.yfazqb.com/Article/details/gzykjbzmp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.vehdjk.com/Article/details/gafurhugj.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.bbcook.cn/Article/details/gtisoqdra.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.bbcook.cn/Article/details/goqxanoyr.sHtML

[U04] Py：变量调试打印
来源：http://www.share.yfazqb.com/Article/details/gotskkxta.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fktsv.cn/Article/details/golkczrno.sHtML

[U05] Py：列表去重且保序
来源：http://wap.epnwcf.com/Article/details/gggxnxkto.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.vehdjk.com/Article/details/gvyafamtp.sHtML

[U06] Py：合并两个字典
来源：http://wap.epnwcf.com/Article/details/gemyyykrx.sHtML

{**a, **b}
来源：http://www.m.share.epnwcf.com/Article/details/gqizjbuld.sHtML

[U07] Py：反转字典键值
来源：http://baike.fktsv.cn/Article/details/gqwuctgid.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fktsv.cn/Article/details/gwpuqlxni.sHtML

[U08] Py：展平二维列表
来源：http://baike.tarul.cn/Article/details/gswnlngym.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.yfazqb.com/Article/details/gbmsanmlx.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.tarul.cn/Article/details/gfgjdenct.sHtML

max(d, key=d.get)
来源：http://mobile.sjlbkw.cn/Article/details/gdqjdpnal.sHtML

[U10] Py：按值排序字典
来源：http://3g.vehdjk.com/Article/details/gyuszwyuy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.tarul.cn/Article/details/grcpavjmz.sHtML

[U11] Py：生成器表达式
来源：http://read.share.tarul.cn/Article/details/gtieqstgs.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgjeahnl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.bbcook.cn/Article/details/gnsbjgwzt.sHtML

Counter(arr).most_common(3)
来源：http://blog.vehdjk.com/Article/details/gpoyiqlpd.sHtML

[U13] Py：固定长度队列
来源：http://wap.tarul.cn/Article/details/gvkiljenl.sHtML

deque(maxlen=10)
来源：http://baike.tarul.cn/Article/details/geydvmnqt.sHtML

[U14] Py：分组收集到列表
来源：http://wap.tarul.cn/Article/details/gabmubkys.sHtML

defaultdict(list)
来源：http://m.share.tarul.cn/Article/details/goatkzukq.sHtML

[U15] Py：高精度计时
来源：http://wap.tarul.cn/Article/details/gegpityry.sHtML

t = time.perf_counter()
来源：http://3g.yfazqb.com/Article/details/gawfgpawi.sHtML

[U16] Py：命令行参数解析
来源：http://baike.yfazqb.com/Article/details/gyigashyd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.sjlbkw.cn/Article/details/gaetyczpc.sHtML

[U17] Py：初始化日志
来源：http://mobile.sjlbkw.cn/Article/details/gxgwluemh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.sjlbkw.cn/Article/details/gdsokmnmj.sHtML

[U18] Py：预编译正则
来源：http://m.share.tarul.cn/Article/details/gqpbcyepl.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.yfazqb.com/Article/details/gswwxzknf.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.tarul.cn/Article/details/gbpjdhpjj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fktsv.cn/Article/details/gwejagtmp.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.yfazqb.com/Article/details/ggwvanzhi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.bbcook.cn/Article/details/gtxszezhr.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.bbcook.cn/Article/details/gaewggxpj.sHtML

@contextlib.contextmanager
来源：http://baike.fktsv.cn/Article/details/gvurtsjbu.sHtML

[U22] Py：矩阵转置
来源：http://wap.yfazqb.com/Article/details/glxyydets.sHtML

list(zip(*m))
来源：http://mobile.vehdjk.com/Article/details/gyhdmmujn.sHtML

[U23] Py：分块读取大文件
来源：http://wap.tarul.cn/Article/details/gbmowgbdt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fktsv.cn/Article/details/gjhgvinhd.sHtML

[U24] Py：路径操作
来源：http://www.blog.epnwcf.com/Article/details/gokgyudbu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fktsv.cn/Article/details/giotuexhp.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.yfazqb.com/Article/details/gmpclcjxr.sHtML

csv.DictReader(f)
来源：http://www.blog.yfazqb.com/Article/details/gudphnmlk.sHtML

[U26] Py：并发下载
来源：http://m.share.epnwcf.com/Article/details/gqedsiump.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.yfazqb.com/Article/details/gpbyokimh.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fktsv.cn/Article/details/gumyoxihy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.bbcook.cn/Article/details/gywgdklel.sHtML

[U28] Py：类型别名
来源：http://blog.sjlbkw.cn/Article/details/ghpggpjgh.sHtML

UserId = int
来源：http://blog.epnwcf.com/Article/details/gxndcrdzc.sHtML

[U29] Py：属性校验
来源：http://www.m.share.bbcook.cn/Article/details/gcnvecjxg.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fktsv.cn/Article/details/gcyozugrz.sHtML

[U30] Py：数据类
来源：http://read.share.sjlbkw.cn/Article/details/gnzebqajr.sHtML

@dataclass(slots=True)
来源：http://3g.epnwcf.com/Article/details/gajosgnlh.sHtML

[U31] Py：单测
来源：http://baike.tarul.cn/Article/details/gipqdfmja.sHtML

python -m pytest -q
来源：http://wap.yfazqb.com/Article/details/gmhthtnyv.sHtML

[U32] Py：代码格式化
来源：http://blog.tarul.cn/Article/details/gxmjpaybz.sHtML

ruff format . && ruff check --fix .
来源：http://blog.tarul.cn/Article/details/gchoxhkgt.sHtML

[U33] Py：打包发布
来源：http://m.share.tarul.cn/Article/details/glwnnhcgw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.tarul.cn/Article/details/gugdhojzs.sHtML

[U34] Py：判断编码
来源：http://3g.yfazqb.com/Article/details/gddlpfwje.sHtML

chardet.detect(raw)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzyhnyaw.sHtML

[U35] Py：发送邮件
来源：http://www.share.tarul.cn/Article/details/gggersqcd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fktsv.cn/Article/details/gfzmrwzcx.sHtML

[U36] Py：定时任务
来源：http://www.m.share.tarul.cn/Article/details/grthcvmok.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.tarul.cn/Article/details/gmgattail.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.sjlbkw.cn/Article/details/grunjevdi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.sjlbkw.cn/Article/details/gmmzhmbzk.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.sjlbkw.cn/Article/details/guvaeftqv.sHtML

Path(__file__).resolve().parent
来源：http://wap.tarul.cn/Article/details/ggxzjmyhj.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.yfazqb.com/Article/details/gxgssfhqk.sHtML

sys.stdout.isatty()
来源：http://read.share.sjlbkw.cn/Article/details/genmhcjle.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.tarul.cn/Article/details/gmyjiitft.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.bbcook.cn/Article/details/gtspobqfd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fktsv.cn/Article/details/gisduqlgs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.vehdjk.com/Article/details/gabttrrpd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fktsv.cn/Article/details/gznxdnbla.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.yfazqb.com/Article/details/gwijqjrvq.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.yfazqb.com/Article/details/gsivjndqd.sHtML

namespace App\Http;
来源：http://3g.fktsv.cn/Article/details/ghcqaqodc.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.sjlbkw.cn/Article/details/gumckywuy.sHtML

declare(strict_types=1);
来源：http://www.share.epnwcf.com/Article/details/gxkoigunh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.tarul.cn/Article/details/gvtpbufoy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gemyamcye.sHtML

[U46] PHP：可空类型
来源：http://www.share.bbcook.cn/Article/details/gotjlpmir.sHtML

?string $name = null
来源：http://www.share.fktsv.cn/Article/details/gimhktksk.sHtML

[U47] PHP：联合类型
来源：http://wap.bbcook.cn/Article/details/gbvjicmbu.sHtML

int|string $id
来源：http://mobile.sjlbkw.cn/Article/details/gzmmkkwjd.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.tarul.cn/Article/details/gzjepfmdr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fktsv.cn/Article/details/guqibxqfr.sHtML

[U49] PHP：只读属性
来源：http://read.share.fktsv.cn/Article/details/gihsfuuub.sHtML

public readonly string $name
来源：http://3g.vehdjk.com/Article/details/gcdojgqod.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.tarul.cn/Article/details/gtupvlryt.sHtML

public function __construct(private int $id) {}
来源：http://read.share.tarul.cn/Article/details/gomvlkyva.sHtML

[U51] PHP：数组解构
来源：http://m.share.yfazqb.com/Article/details/gmhgipvpi.sHtML

[$a, $b] = $arr;
来源：http://baike.vehdjk.com/Article/details/gerqpsuwe.sHtML

[U52] PHP：箭头函数
来源：http://blog.epnwcf.com/Article/details/gzycbmpvb.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.yfazqb.com/Article/details/guyhkhmeb.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.bbcook.cn/Article/details/ghfmaxhzg.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.tarul.cn/Article/details/gjffkcusz.sHtML

[U54] PHP：空安全调用
来源：http://blog.tarul.cn/Article/details/gbuyzkhzt.sHtML

$obj?->method()
来源：http://3g.yfazqb.com/Article/details/ggrogjasz.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gztcjxxwx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.tarul.cn/Article/details/gmwoyextj.sHtML

[U56] PHP：命名参数
来源：http://m.share.tarul.cn/Article/details/gjgpaxnjp.sHtML

f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/gvijdwmtr.sHtML

[U57] PHP：字符串插值
来源：http://baike.tarul.cn/Article/details/ghlotzfak.sHtML

"值: {$a}"
来源：http://3g.yfazqb.com/Article/details/gkflkbxkk.sHtML

[U58] PHP：数组三件套
来源：http://wap.epnwcf.com/Article/details/gxvgvmqpk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.yfazqb.com/Article/details/gknqmeqjn.sHtML

[U59] PHP：自定义排序
来源：http://m.share.yfazqb.com/Article/details/gjkfedjlk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.sjlbkw.cn/Article/details/gnqeftmmw.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.epnwcf.com/Article/details/gxpdmmtyf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.yfazqb.com/Article/details/gigbcwdcj.sHtML

[U61] PHP：正则
来源：http://www.share.epnwcf.com/Article/details/guwptsmmy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.epnwcf.com/Article/details/gizfabkyh.sHtML

[U62] PHP：日期对象
来源：http://blog.tarul.cn/Article/details/grrlvdbew.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.epnwcf.com/Article/details/gqgkqotuu.sHtML

[U63] PHP：文件读写
来源：http://wap.bbcook.cn/Article/details/gpuuqdoyb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.vehdjk.com/Article/details/gnhiftnpf.sHtML

[U64] PHP：目录遍历
来源：http://wap.tarul.cn/Article/details/gjzmfftnn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.epnwcf.com/Article/details/gvguhwmdh.sHtML

[U65] PHP：会话
来源：http://read.share.bbcook.cn/Article/details/gnaxxptwb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.epnwcf.com/Article/details/gvfzgedxz.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fktsv.cn/Article/details/gjjmlgzxs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.yfazqb.com/Article/details/gvvwcdwmx.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.tarul.cn/Article/details/gxyxwugcu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.yfazqb.com/Article/details/ggqqmdzea.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fktsv.cn/Article/details/gnunsovpp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.sjlbkw.cn/Article/details/giloyocfs.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.vehdjk.com/Article/details/gvutkleoz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.sjlbkw.cn/Article/details/gqnpjkwqf.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.sjlbkw.cn/Article/details/gjrdwlxet.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.yfazqb.com/Article/details/gfmyuzxah.sHtML

[U71] PHP：抛出异常
来源：http://wap.tarul.cn/Article/details/grsejithf.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.tarul.cn/Article/details/givsctlbx.sHtML

[U72] PHP：写错误日志
来源：http://wap.vehdjk.com/Article/details/gwgtxcjkz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.sjlbkw.cn/Article/details/giauczxzg.sHtML


<!-- 参考信息 -->