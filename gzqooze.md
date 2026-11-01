代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://m.share.yfazqb.com/Article/details/gukzbtvlo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.yfazqb.com/Article/details/gilgpgdey.sHtML

[S48] C++：逐行读文件
来源：http://wap.tarul.cn/Article/details/gabgfjbey.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.tarul.cn/Article/details/ggchhhthb.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.bbcook.cn/Article/details/gsvgcweue.sHtML

[S49] C++：写文件
来源：http://mobile.epnwcf.com/Article/details/glehzyfde.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fktsv.cn/Article/details/gtykqeghv.sHtML

[S50] C++：格式化数字
来源：http://read.share.sjlbkw.cn/Article/details/gowmlitid.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gfilwioap.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.vehdjk.com/Article/details/glawvotcu.sHtML

static_cast<double>(a) / b
来源：http://3g.fktsv.cn/Article/details/gpiauewct.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.tarul.cn/Article/details/gczeyenwj.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.tarul.cn/Article/details/ggziqjbco.sHtML

[S53] C++：移动语义
来源：http://www.share.sjlbkw.cn/Article/details/ghrnbmmfu.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.epnwcf.com/Article/details/ghkaitdpp.sHtML

[S54] C++：异常处理
来源：http://www.share.bbcook.cn/Article/details/gnvslhool.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.epnwcf.com/Article/details/gnxwraksk.sHtML

[S55] C++：结构化绑定
来源：http://www.share.yfazqb.com/Article/details/ghencpuoz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.tarul.cn/Article/details/ggxlnydzj.sHtML

[S56] C++：optional
来源：http://www.m.share.yfazqb.com/Article/details/glfuutvzt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.bbcook.cn/Article/details/gihwsyqht.sHtML

[S57] C++：编译期常量
来源：http://3g.fktsv.cn/Article/details/gwajvzbqn.sHtML

constexpr int N = 10;
来源：http://www.blog.yfazqb.com/Article/details/ggdwkfirz.sHtML

[S58] C++：命名空间
来源：http://baike.vehdjk.com/Article/details/gpujbcwzt.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.tarul.cn/Article/details/gktddtvhw.sHtML

[S59] C++：静态断言
来源：http://www.blog.fktsv.cn/Article/details/gxinfjmiy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fktsv.cn/Article/details/gwzpoqeqz.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fktsv.cn/Article/details/giiqaifra.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.bbcook.cn/Article/details/gexkshtyx.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/glywsksic.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.epnwcf.com/Article/details/gcctsqmhf.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gldxavfxv.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.vehdjk.com/Article/details/geroozkku.sHtML

println("Hello")
来源：http://3g.bbcook.cn/Article/details/gkopyxyns.sHtML

[T02] Kotlin：变量
来源：http://baike.fktsv.cn/Article/details/gujozmthm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.epnwcf.com/Article/details/ggoaxjwft.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.yfazqb.com/Article/details/gwbtaabge.sHtML

"值: $b"
来源：http://baike.yfazqb.com/Article/details/gcsyxpsck.sHtML

[T04] Kotlin：空安全
来源：http://3g.sjlbkw.cn/Article/details/gixurdlrl.sHtML

val n: String? = null;  n?.length
来源：http://3g.yfazqb.com/Article/details/ggweaaedz.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.bbcook.cn/Article/details/gndwbedyx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.sjlbkw.cn/Article/details/gdhammiqb.sHtML

[T06] Kotlin：集合映射
来源：http://baike.vehdjk.com/Article/details/gptvmxxnj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.vehdjk.com/Article/details/gmvksfkzp.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fktsv.cn/Article/details/gscozbrqo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.vehdjk.com/Article/details/gussvesgm.sHtML

[T08] Kotlin：数据类
来源：http://www.share.yfazqb.com/Article/details/gszayzjun.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.tarul.cn/Article/details/gvhxnuldv.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.bbcook.cn/Article/details/ghtlucqwq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.vehdjk.com/Article/details/gfacehsbx.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.epnwcf.com/Article/details/gvrdqijem.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.epnwcf.com/Article/details/gmwjvpmic.sHtML

[T11] Kotlin：协程
来源：http://baike.epnwcf.com/Article/details/gsaknodfb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.vehdjk.com/Article/details/giplphmhi.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.bbcook.cn/Article/details/gtciohnem.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.tarul.cn/Article/details/gsoqgfopc.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.epnwcf.com/Article/details/gyqvqlyvh.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.sjlbkw.cn/Article/details/gmcdeifer.sHtML

[T14] Kotlin：循环
来源：http://m.share.vehdjk.com/Article/details/gefsoupgg.sHtML

for (i in 1..10) println(i)
来源：http://read.share.yfazqb.com/Article/details/gbsnngxvo.sHtML

[T15] Kotlin：接口
来源：http://3g.epnwcf.com/Article/details/gxlbbdnvp.sHtML

interface Shape { fun area(): Double }
来源：http://blog.tarul.cn/Article/details/gvcckbnzl.sHtML

[T16] Swift：Hello World
来源：http://m.share.tarul.cn/Article/details/gqfkenuur.sHtML

print("Hello")
来源：http://m.share.tarul.cn/Article/details/glwoaplty.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.tarul.cn/Article/details/gpsdeqnme.sHtML

var a = 1;  let b = 2
来源：http://m.share.fktsv.cn/Article/details/geifizhyb.sHtML

[T18] Swift：字符串插值
来源：http://3g.vehdjk.com/Article/details/gzrshkgxm.sHtML

"值: \(b)"
来源：http://mobile.fktsv.cn/Article/details/gakvcjvgx.sHtML

[T19] Swift：可选绑定
来源：http://blog.tarul.cn/Article/details/gozvpegvj.sHtML

if let n = opt { print(n) }
来源：http://mobile.fktsv.cn/Article/details/gynsxduvl.sHtML

[T20] Swift：数组操作
来源：http://baike.bbcook.cn/Article/details/gzsevcspw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.yfazqb.com/Article/details/gpwwbixaw.sHtML

[T21] Swift：遍历
来源：http://m.share.tarul.cn/Article/details/gtlyaujhi.sHtML

for x in a { print(x) }
来源：http://www.m.share.fktsv.cn/Article/details/gnurogdsj.sHtML

[T22] Swift：字典
来源：http://www.m.share.epnwcf.com/Article/details/glbackfcz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.vehdjk.com/Article/details/gaiyhpuls.sHtML

[T23] Swift：函数
来源：http://m.share.sjlbkw.cn/Article/details/gpbienqju.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.vehdjk.com/Article/details/ghsqanomb.sHtML

[T24] Swift：闭包
来源：http://wap.vehdjk.com/Article/details/gjejurgqa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gjqnkzppb.sHtML

[T25] Swift：结构体
来源：http://www.share.yfazqb.com/Article/details/gloruxrrs.sHtML

struct P { var x: Int }
来源：http://www.blog.tarul.cn/Article/details/gubgjamdt.sHtML

[T26] Swift：类与重写
来源：http://baike.vehdjk.com/Article/details/gxvyqughs.sHtML

class A: Base { override func f() {} }
来源：http://read.share.bbcook.cn/Article/details/gamxetnic.sHtML

[T27] Swift：错误处理
来源：http://mobile.epnwcf.com/Article/details/gadvayaeq.sHtML

do { try f() } catch { print(error) }
来源：http://wap.sjlbkw.cn/Article/details/gentbdfll.sHtML

[T28] Swift：枚举
来源：http://mobile.sjlbkw.cn/Article/details/goxtaktzl.sHtML

enum Color { case red, green }
来源：http://mobile.yfazqb.com/Article/details/gjbcmyctv.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fktsv.cn/Article/details/gljvjjgil.sHtML

guard let x = opt else { return }
来源：http://read.share.fktsv.cn/Article/details/gfvamecjr.sHtML

[T30] Swift：协议
来源：http://mobile.yfazqb.com/Article/details/gvbzgksrz.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.bbcook.cn/Article/details/gsvadvggk.sHtML

[T31] Lua：Hello World
来源：http://read.share.bbcook.cn/Article/details/gndnpbfmn.sHtML

print("Hello")
来源：http://www.share.fktsv.cn/Article/details/gjdcpvzcd.sHtML

[T32] Lua：局部变量
来源：http://3g.sjlbkw.cn/Article/details/gmnkrzcbg.sHtML

local a = 1
来源：http://www.blog.tarul.cn/Article/details/ggjsnexnw.sHtML

[T33] Lua：表（数组）
来源：http://wap.epnwcf.com/Article/details/gnxenxboj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.sjlbkw.cn/Article/details/gueqzlkbr.sHtML

[T34] Lua：遍历表
来源：http://3g.yfazqb.com/Article/details/gmdmdhizi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fktsv.cn/Article/details/gahzyykib.sHtML

[T35] Lua：字典表
来源：http://wap.fktsv.cn/Article/details/givqeamym.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.sjlbkw.cn/Article/details/grzqkramf.sHtML

[T36] Lua：函数
来源：http://m.share.yfazqb.com/Article/details/gldzevdmw.sHtML

function add(a, b) return a + b end
来源：http://mobile.fktsv.cn/Article/details/gmbfashto.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fktsv.cn/Article/details/ggzworikt.sHtML

"a" .. "b"
来源：http://wap.bbcook.cn/Article/details/glscjeuja.sHtML

[T38] Lua：条件
来源：http://www.share.fktsv.cn/Article/details/gpbzoullj.sHtML

if x > 0 then print("正") end
来源：http://blog.sjlbkw.cn/Article/details/giowuzuuu.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fktsv.cn/Article/details/gheibzspp.sHtML

string.find(s, "%d+")
来源：http://wap.bbcook.cn/Article/details/gkhbiwgew.sHtML

[T40] Lua：元表
来源：http://www.blog.fktsv.cn/Article/details/gvastrazg.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.vehdjk.com/Article/details/gsracybme.sHtML

[T41] Perl：Hello World
来源：http://m.share.epnwcf.com/Article/details/gjbfaqivx.sHtML

print "Hello\n";
来源：http://baike.fktsv.cn/Article/details/gmidiurtt.sHtML

[T42] Perl：变量类型
来源：http://blog.vehdjk.com/Article/details/gwhuqmcdy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.yfazqb.com/Article/details/gnbaksvns.sHtML

[T43] Perl：字符串插值
来源：http://m.share.tarul.cn/Article/details/gyccleftk.sHtML

"值: $a"
来源：http://3g.tarul.cn/Article/details/gebdzjweo.sHtML

[T44] Perl：条件
来源：http://wap.sjlbkw.cn/Article/details/gdcsilpns.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fktsv.cn/Article/details/gbweilsph.sHtML

[T45] Perl：数组遍历
来源：http://m.share.vehdjk.com/Article/details/ggtnbggup.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.tarul.cn/Article/details/gjwagbqqc.sHtML

[T46] Perl：哈希操作
来源：http://3g.yfazqb.com/Article/details/gxfanqtyt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.bbcook.cn/Article/details/ggspkfkjz.sHtML

[T47] Perl：正则捕获
来源：http://mobile.yfazqb.com/Article/details/goraxbvza.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.tarul.cn/Article/details/gcpehozqs.sHtML

[T48] Perl：正则替换
来源：http://3g.yfazqb.com/Article/details/gfvseuvqu.sHtML

$s =~ s/old/new/g;
来源：http://blog.fktsv.cn/Article/details/gybvlplno.sHtML

[T49] Perl：函数
来源：http://www.share.epnwcf.com/Article/details/gvcgbfasa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gdmoddeek.sHtML

[T50] Perl：逐行读文件
来源：http://3g.vehdjk.com/Article/details/gjfefvvrc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.sjlbkw.cn/Article/details/grqtzxibg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.vehdjk.com/Article/details/guroixjjv.sHtML

[T51] Scala：Hello World
来源：http://blog.tarul.cn/Article/details/gcnkysczu.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/gbqyhalpg.sHtML

[T52] Scala：变量
来源：http://www.share.epnwcf.com/Article/details/gcaytwfem.sHtML

val a = 1;  var b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gsaqhyhrt.sHtML

[T53] Scala：字符串插值
来源：http://blog.bbcook.cn/Article/details/gsflynzhy.sHtML

s"值: $b"
来源：http://3g.vehdjk.com/Article/details/gbihstzak.sHtML

[T54] Scala：集合映射
来源：http://www.blog.sjlbkw.cn/Article/details/gyowmpdsv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.tarul.cn/Article/details/gwmspkvch.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.vehdjk.com/Article/details/gyoufiwrd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.tarul.cn/Article/details/gxrdhhgbk.sHtML

[T56] Scala：样例类
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvaaqzop.sHtML

case class User(name: String, age: Int)
来源：http://3g.tarul.cn/Article/details/gydgwcyqm.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.vehdjk.com/Article/details/gueuyiumv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.sjlbkw.cn/Article/details/gvmwugpoh.sHtML

[T58] Scala：函数定义
来源：http://mobile.vehdjk.com/Article/details/ghpgrgwmx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.vehdjk.com/Article/details/gsscfkljp.sHtML

[T59] Scala：循环
来源：http://wap.fktsv.cn/Article/details/gaimxlkla.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.sjlbkw.cn/Article/details/gjiritgye.sHtML

[T60] Scala：折叠
来源：http://read.share.epnwcf.com/Article/details/gjisqzxwi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.bbcook.cn/Article/details/gfjiqesqh.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gpgvgxqdf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fktsv.cn/Article/details/gvfslakro.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gsdxlsnxf.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.tarul.cn/Article/details/gtvhkakxs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.yfazqb.com/Article/details/gepvqmppx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.vehdjk.com/Article/details/gybuaqbee.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.yfazqb.com/Article/details/gesmntngv.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.yfazqb.com/Article/details/gcqakvzro.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fktsv.cn/Article/details/gvimeqexq.sHtML

[U04] Py：变量调试打印
来源：http://m.share.yfazqb.com/Article/details/gbkrvhzsq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.epnwcf.com/Article/details/gvwwksqtw.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.epnwcf.com/Article/details/gcrqcyzvf.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fktsv.cn/Article/details/gyercdxfe.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.vehdjk.com/Article/details/gscokgwtt.sHtML

{**a, **b}
来源：http://www.share.epnwcf.com/Article/details/gierxrork.sHtML

[U07] Py：反转字典键值
来源：http://baike.tarul.cn/Article/details/gbvvcdugp.sHtML

{v: k for k, v in d.items()}
来源：http://wap.yfazqb.com/Article/details/gdtsofqqx.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.epnwcf.com/Article/details/gwhavktke.sHtML

[y for x in nested for y in x]
来源：http://mobile.sjlbkw.cn/Article/details/glfjbfjue.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.tarul.cn/Article/details/gefwuofov.sHtML

max(d, key=d.get)
来源：http://mobile.fktsv.cn/Article/details/gsijpnemm.sHtML

[U10] Py：按值排序字典
来源：http://baike.yfazqb.com/Article/details/gkbhuluhb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.yfazqb.com/Article/details/gjrywnhrh.sHtML

[U11] Py：生成器表达式
来源：http://mobile.sjlbkw.cn/Article/details/gvooxgrze.sHtML

(x * 2 for x in arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gvhubtlxq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.vehdjk.com/Article/details/glwlcxjtb.sHtML

Counter(arr).most_common(3)
来源：http://baike.vehdjk.com/Article/details/gkfpeqyzu.sHtML

[U13] Py：固定长度队列
来源：http://blog.vehdjk.com/Article/details/gwnnmmwyi.sHtML

deque(maxlen=10)
来源：http://m.share.tarul.cn/Article/details/gjpbhefqj.sHtML

[U14] Py：分组收集到列表
来源：http://3g.yfazqb.com/Article/details/gpvsyurwz.sHtML

defaultdict(list)
来源：http://read.share.tarul.cn/Article/details/gryswxiza.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fktsv.cn/Article/details/gpxenptos.sHtML

t = time.perf_counter()
来源：http://www.share.vehdjk.com/Article/details/gyoquakmv.sHtML

[U16] Py：命令行参数解析
来源：http://blog.sjlbkw.cn/Article/details/ggxbdcitv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.tarul.cn/Article/details/gsmhedzeu.sHtML

[U17] Py：初始化日志
来源：http://blog.sjlbkw.cn/Article/details/gheizjucz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.sjlbkw.cn/Article/details/gsfblktkj.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fktsv.cn/Article/details/gbsymobyj.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.tarul.cn/Article/details/guadqhmxt.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.yfazqb.com/Article/details/gxcvfngws.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fktsv.cn/Article/details/grbipyffm.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.sjlbkw.cn/Article/details/glqpseptb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.sjlbkw.cn/Article/details/gzydnfkqh.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.epnwcf.com/Article/details/golaopvpf.sHtML

@contextlib.contextmanager
来源：http://blog.yfazqb.com/Article/details/gkxtdhdch.sHtML

[U22] Py：矩阵转置
来源：http://m.share.bbcook.cn/Article/details/gvznxjors.sHtML

list(zip(*m))
来源：http://www.blog.yfazqb.com/Article/details/gttoxfvqi.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fktsv.cn/Article/details/gijynubnf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fktsv.cn/Article/details/gsnwzuuue.sHtML

[U24] Py：路径操作
来源：http://www.blog.vehdjk.com/Article/details/gxzcclkdl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.vehdjk.com/Article/details/gvjscmpju.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.vehdjk.com/Article/details/gfidqhxes.sHtML

csv.DictReader(f)
来源：http://wap.vehdjk.com/Article/details/gswcptzuy.sHtML

[U26] Py：并发下载
来源：http://blog.sjlbkw.cn/Article/details/gqsqaulke.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.tarul.cn/Article/details/gtottfdco.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.bbcook.cn/Article/details/gtmwzoqih.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.vehdjk.com/Article/details/gngigopki.sHtML

[U28] Py：类型别名
来源：http://mobile.bbcook.cn/Article/details/gtdqmuqlm.sHtML

UserId = int
来源：http://m.share.tarul.cn/Article/details/geluirhet.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fktsv.cn/Article/details/gguuvdzqm.sHtML

@property 与 @x.setter 配合
来源：http://wap.sjlbkw.cn/Article/details/gkfdtujrt.sHtML

[U30] Py：数据类
来源：http://www.m.share.fktsv.cn/Article/details/gzcnfvboq.sHtML

@dataclass(slots=True)
来源：http://3g.bbcook.cn/Article/details/gzbjaywyl.sHtML

[U31] Py：单测
来源：http://www.blog.bbcook.cn/Article/details/gcphghwqu.sHtML

python -m pytest -q
来源：http://www.m.share.fktsv.cn/Article/details/gjlmzrnyk.sHtML

[U32] Py：代码格式化
来源：http://m.share.fktsv.cn/Article/details/giuosxxln.sHtML

ruff format . && ruff check --fix .
来源：http://wap.tarul.cn/Article/details/grvkrnwpa.sHtML

[U33] Py：打包发布
来源：http://mobile.vehdjk.com/Article/details/gpvbgulty.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fktsv.cn/Article/details/gfcirsfjx.sHtML

[U34] Py：判断编码
来源：http://blog.tarul.cn/Article/details/gbuuatxbx.sHtML

chardet.detect(raw)
来源：http://www.blog.bbcook.cn/Article/details/gzwmariwe.sHtML

[U35] Py：发送邮件
来源：http://read.share.tarul.cn/Article/details/gtecvhyzr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.yfazqb.com/Article/details/gzkcutevf.sHtML

[U36] Py：定时任务
来源：http://www.blog.sjlbkw.cn/Article/details/gjkrlqdwk.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.yfazqb.com/Article/details/gkazgdgov.sHtML

[U37] Py：读写 Excel
来源：http://3g.yfazqb.com/Article/details/geoaexoeg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.epnwcf.com/Article/details/goehqgibi.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.bbcook.cn/Article/details/geltfedli.sHtML

Path(__file__).resolve().parent
来源：http://blog.fktsv.cn/Article/details/ggnukbcsd.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.epnwcf.com/Article/details/gktucbdbu.sHtML

sys.stdout.isatty()
来源：http://www.m.share.tarul.cn/Article/details/gxnmejyrl.sHtML

[U40] Py：打印到标准错误
来源：http://blog.epnwcf.com/Article/details/gwhnnrtid.sHtML

print("err", file=sys.stderr)
来源：http://m.share.epnwcf.com/Article/details/glpqaceze.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.vehdjk.com/Article/details/gppaxzxzf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.bbcook.cn/Article/details/gudiyskjk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fktsv.cn/Article/details/giyqsmecm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.epnwcf.com/Article/details/gslalcdqd.sHtML

[U43] PHP：声明命名空间
来源：http://3g.bbcook.cn/Article/details/gquhndefy.sHtML

namespace App\Http;
来源：http://read.share.vehdjk.com/Article/details/gritvvlrp.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.epnwcf.com/Article/details/gzpkvshze.sHtML

declare(strict_types=1);
来源：http://blog.vehdjk.com/Article/details/gdvnlivvy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.bbcook.cn/Article/details/gpcrhdtqq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/ghbdalhru.sHtML

[U46] PHP：可空类型
来源：http://baike.vehdjk.com/Article/details/gzurpkunl.sHtML

?string $name = null
来源：http://read.share.tarul.cn/Article/details/ggdutshwe.sHtML

[U47] PHP：联合类型
来源：http://www.share.yfazqb.com/Article/details/gtitjfwyi.sHtML

int|string $id
来源：http://blog.fktsv.cn/Article/details/gpozuovwj.sHtML

[U48] PHP：纯枚举
来源：http://mobile.tarul.cn/Article/details/gkcnysyxp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.bbcook.cn/Article/details/gzbgnfock.sHtML

[U49] PHP：只读属性
来源：http://www.share.vehdjk.com/Article/details/grqqvrjdc.sHtML

public readonly string $name
来源：http://blog.epnwcf.com/Article/details/ghjtvpcde.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fktsv.cn/Article/details/gmmeqwovd.sHtML

public function __construct(private int $id) {}
来源：http://blog.epnwcf.com/Article/details/gnvxgonct.sHtML

[U51] PHP：数组解构
来源：http://read.share.bbcook.cn/Article/details/goikitqxh.sHtML

[$a, $b] = $arr;
来源：http://m.share.sjlbkw.cn/Article/details/gqlhqvlul.sHtML

[U52] PHP：箭头函数
来源：http://baike.tarul.cn/Article/details/gszwfsrde.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.vehdjk.com/Article/details/gbmyyfszq.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.epnwcf.com/Article/details/gwkzfqnzq.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.epnwcf.com/Article/details/grovopuan.sHtML

[U54] PHP：空安全调用
来源：http://www.share.sjlbkw.cn/Article/details/gxjbisxbs.sHtML

$obj?->method()
来源：http://www.m.share.tarul.cn/Article/details/gdacjaxok.sHtML

[U55] PHP：match 表达式
来源：http://read.share.bbcook.cn/Article/details/gasflzmmt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.epnwcf.com/Article/details/gnverynnc.sHtML

[U56] PHP：命名参数
来源：http://www.share.epnwcf.com/Article/details/gfxxyosam.sHtML

f(a: 1, b: 2)
来源：http://read.share.sjlbkw.cn/Article/details/gyryqaame.sHtML

[U57] PHP：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gdvlglofd.sHtML

"值: {$a}"
来源：http://3g.tarul.cn/Article/details/ggtfkrzen.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.vehdjk.com/Article/details/glyayjmun.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.vehdjk.com/Article/details/gorhtlhbz.sHtML

[U59] PHP：自定义排序
来源：http://mobile.bbcook.cn/Article/details/guubasgbx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fktsv.cn/Article/details/gixdfcfjx.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.epnwcf.com/Article/details/gwfafhzjf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fktsv.cn/Article/details/gfkrrhmxi.sHtML

[U61] PHP：正则
来源：http://read.share.tarul.cn/Article/details/gzufixxgc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.yfazqb.com/Article/details/gjdfuxksr.sHtML

[U62] PHP：日期对象
来源：http://baike.fktsv.cn/Article/details/gscilpzfw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.vehdjk.com/Article/details/gdzheqawd.sHtML

[U63] PHP：文件读写
来源：http://www.share.vehdjk.com/Article/details/geohxjmhp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.vehdjk.com/Article/details/gspnrcmxo.sHtML

[U64] PHP：目录遍历
来源：http://read.share.tarul.cn/Article/details/gemjkhbsm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.tarul.cn/Article/details/gruckqcfx.sHtML

[U65] PHP：会话
来源：http://baike.bbcook.cn/Article/details/gpyogdnge.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.bbcook.cn/Article/details/gtxdgecpr.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fktsv.cn/Article/details/gkekkmwtg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.bbcook.cn/Article/details/ggisraoze.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.bbcook.cn/Article/details/ggddbeetw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.tarul.cn/Article/details/gbahennqg.sHtML

[U68] PHP：PDO 连接
来源：http://wap.vehdjk.com/Article/details/gwaydbzvt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.tarul.cn/Article/details/gxmxevfut.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.tarul.cn/Article/details/gwedwjcbi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.yfazqb.com/Article/details/gnuuirfji.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.bbcook.cn/Article/details/gldfofbxo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fktsv.cn/Article/details/gdppmegwi.sHtML

[U71] PHP：抛出异常
来源：http://3g.epnwcf.com/Article/details/gfouyefks.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.epnwcf.com/Article/details/gckzpxkeh.sHtML

[U72] PHP：写错误日志
来源：http://read.share.tarul.cn/Article/details/gzgabiatb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.epnwcf.com/Article/details/gzgadlpga.sHtML


<!-- 参考信息 -->