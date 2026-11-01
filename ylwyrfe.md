代发 wailian999

[S45] C++：lambda
来源：http://m.share.fktsv.cn/Article/details/gqzgonjbf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.tarul.cn/Article/details/guvqmfdct.sHtML

[S46] C++：函数模板
来源：http://mobile.fktsv.cn/Article/details/grapanple.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.epnwcf.com/Article/details/gwvvneewi.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.epnwcf.com/Article/details/gtblpujhp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.vehdjk.com/Article/details/gvkkclhjd.sHtML

[S48] C++：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gjrodndet.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.bbcook.cn/Article/details/ghvzgtmgv.sHtML

while (std::getline(in, line)) { }
来源：http://blog.bbcook.cn/Article/details/gbmrzybmj.sHtML

[S49] C++：写文件
来源：http://www.blog.epnwcf.com/Article/details/gybiplulm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.vehdjk.com/Article/details/gwxnthmdl.sHtML

[S50] C++：格式化数字
来源：http://www.share.fktsv.cn/Article/details/gjjgulhcz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gszjcxagw.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fktsv.cn/Article/details/ghrqbxmhj.sHtML

static_cast<double>(a) / b
来源：http://blog.fktsv.cn/Article/details/gekhfeazj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.bbcook.cn/Article/details/gjkstwlbl.sHtML

int size() const noexcept { return n_; }
来源：http://3g.vehdjk.com/Article/details/gimeeanuj.sHtML

[S53] C++：移动语义
来源：http://www.blog.vehdjk.com/Article/details/gihilwodl.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.vehdjk.com/Article/details/gpcgnbubo.sHtML

[S54] C++：异常处理
来源：http://mobile.epnwcf.com/Article/details/gvqxgrvwh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.yfazqb.com/Article/details/gqruxptmj.sHtML

[S55] C++：结构化绑定
来源：http://read.share.vehdjk.com/Article/details/gatveeczm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.bbcook.cn/Article/details/gmibhpfed.sHtML

[S56] C++：optional
来源：http://www.share.fktsv.cn/Article/details/gdottxvtz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.yfazqb.com/Article/details/gbrqrwxbf.sHtML

[S57] C++：编译期常量
来源：http://blog.bbcook.cn/Article/details/gfjucywve.sHtML

constexpr int N = 10;
来源：http://wap.yfazqb.com/Article/details/gjabjscti.sHtML

[S58] C++：命名空间
来源：http://mobile.yfazqb.com/Article/details/glkbfzuih.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.vehdjk.com/Article/details/goeoglbwq.sHtML

[S59] C++：静态断言
来源：http://m.share.bbcook.cn/Article/details/gopvuiltm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.yfazqb.com/Article/details/gktecirgl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.epnwcf.com/Article/details/grdgxnvuz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fktsv.cn/Article/details/gyizyqxfb.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gkoxylkya.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.vehdjk.com/Article/details/gckjiojrz.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqeuhijmz.sHtML

[T01] Kotlin：Hello World
来源：http://wap.yfazqb.com/Article/details/gqujkokbg.sHtML

println("Hello")
来源：http://wap.tarul.cn/Article/details/gvbizoedo.sHtML

[T02] Kotlin：变量
来源：http://www.share.vehdjk.com/Article/details/gldfcrfyj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.tarul.cn/Article/details/guholqggy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.epnwcf.com/Article/details/gjepivmrw.sHtML

"值: $b"
来源：http://wap.bbcook.cn/Article/details/grmvumlrs.sHtML

[T04] Kotlin：空安全
来源：http://www.share.vehdjk.com/Article/details/ggmryivrx.sHtML

val n: String? = null;  n?.length
来源：http://www.share.sjlbkw.cn/Article/details/gkmslsfxl.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.vehdjk.com/Article/details/gebpgmnxo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.bbcook.cn/Article/details/glcvterse.sHtML

[T06] Kotlin：集合映射
来源：http://baike.sjlbkw.cn/Article/details/grwooxppi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.epnwcf.com/Article/details/gcrrtzhqc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fktsv.cn/Article/details/gdcrrmeao.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.yfazqb.com/Article/details/gisavhvtw.sHtML

[T08] Kotlin：数据类
来源：http://read.share.tarul.cn/Article/details/gvjoqfbmp.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.bbcook.cn/Article/details/gijaulucb.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.bbcook.cn/Article/details/gagonngvw.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.yfazqb.com/Article/details/gmgojsgwx.sHtML

[T10] Kotlin：默认参数
来源：http://blog.yfazqb.com/Article/details/gtdpzwtgx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.tarul.cn/Article/details/gaunhgduq.sHtML

[T11] Kotlin：协程
来源：http://www.share.vehdjk.com/Article/details/gccpyrwxc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.bbcook.cn/Article/details/gmgravysy.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.sjlbkw.cn/Article/details/gyqfapiiv.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gpbhwwulx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/gspjrkuhp.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.yfazqb.com/Article/details/gjuftzsic.sHtML

[T14] Kotlin：循环
来源：http://mobile.vehdjk.com/Article/details/govwjmaao.sHtML

for (i in 1..10) println(i)
来源：http://read.share.yfazqb.com/Article/details/gepyapcqp.sHtML

[T15] Kotlin：接口
来源：http://www.share.sjlbkw.cn/Article/details/ggcjqshzk.sHtML

interface Shape { fun area(): Double }
来源：http://blog.epnwcf.com/Article/details/gtecjopkl.sHtML

[T16] Swift：Hello World
来源：http://www.blog.vehdjk.com/Article/details/ghdnklbcl.sHtML

print("Hello")
来源：http://3g.yfazqb.com/Article/details/gvnszcvrx.sHtML

[T17] Swift：变量与常量
来源：http://blog.fktsv.cn/Article/details/gkxigpote.sHtML

var a = 1;  let b = 2
来源：http://wap.bbcook.cn/Article/details/gelpgunqy.sHtML

[T18] Swift：字符串插值
来源：http://read.share.epnwcf.com/Article/details/ghrncitaf.sHtML

"值: \(b)"
来源：http://blog.sjlbkw.cn/Article/details/gtfwlabac.sHtML

[T19] Swift：可选绑定
来源：http://m.share.vehdjk.com/Article/details/gyhrcrqny.sHtML

if let n = opt { print(n) }
来源：http://mobile.tarul.cn/Article/details/gasqfyuph.sHtML

[T20] Swift：数组操作
来源：http://baike.epnwcf.com/Article/details/geqqsyozh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fktsv.cn/Article/details/grzbtlbrd.sHtML

[T21] Swift：遍历
来源：http://3g.yfazqb.com/Article/details/ggrmqylrz.sHtML

for x in a { print(x) }
来源：http://baike.epnwcf.com/Article/details/gezxjyydg.sHtML

[T22] Swift：字典
来源：http://www.share.epnwcf.com/Article/details/gbtxxmvjk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.epnwcf.com/Article/details/gaqyteuiq.sHtML

[T23] Swift：函数
来源：http://baike.yfazqb.com/Article/details/gnwsfvpai.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fktsv.cn/Article/details/gwtxadfht.sHtML

[T24] Swift：闭包
来源：http://m.share.epnwcf.com/Article/details/gvqigzmvu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.yfazqb.com/Article/details/guzxuynkt.sHtML

[T25] Swift：结构体
来源：http://read.share.epnwcf.com/Article/details/gzzbuxaek.sHtML

struct P { var x: Int }
来源：http://www.share.sjlbkw.cn/Article/details/gazsarkrm.sHtML

[T26] Swift：类与重写
来源：http://read.share.tarul.cn/Article/details/gveuvjfzp.sHtML

class A: Base { override func f() {} }
来源：http://m.share.epnwcf.com/Article/details/gvahxapwy.sHtML

[T27] Swift：错误处理
来源：http://m.share.vehdjk.com/Article/details/gunjbyamx.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fktsv.cn/Article/details/gaeirphaf.sHtML

[T28] Swift：枚举
来源：http://www.blog.epnwcf.com/Article/details/gepwxdcfj.sHtML

enum Color { case red, green }
来源：http://read.share.yfazqb.com/Article/details/gknrqotwd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fktsv.cn/Article/details/gvwqkpulg.sHtML

guard let x = opt else { return }
来源：http://www.blog.vehdjk.com/Article/details/gohxxwtwi.sHtML

[T30] Swift：协议
来源：http://mobile.yfazqb.com/Article/details/gmojcceel.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fktsv.cn/Article/details/gtbbvyoeh.sHtML

[T31] Lua：Hello World
来源：http://baike.fktsv.cn/Article/details/glfmzxnrt.sHtML

print("Hello")
来源：http://read.share.bbcook.cn/Article/details/gdhaphzuq.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.epnwcf.com/Article/details/gnpzrwxke.sHtML

local a = 1
来源：http://baike.yfazqb.com/Article/details/gjehfnjtl.sHtML

[T33] Lua：表（数组）
来源：http://www.share.bbcook.cn/Article/details/gmyzunhyx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.yfazqb.com/Article/details/gdbdkobnj.sHtML

[T34] Lua：遍历表
来源：http://m.share.epnwcf.com/Article/details/gzpwxqwtc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.yfazqb.com/Article/details/gcdrugviy.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fktsv.cn/Article/details/gbqsfrcct.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.yfazqb.com/Article/details/gtqqqjuem.sHtML

[T36] Lua：函数
来源：http://wap.vehdjk.com/Article/details/gtfblsewu.sHtML

function add(a, b) return a + b end
来源：http://m.share.tarul.cn/Article/details/gelxgrbyi.sHtML

[T37] Lua：字符串拼接
来源：http://baike.epnwcf.com/Article/details/ggdsfyndr.sHtML

"a" .. "b"
来源：http://www.share.sjlbkw.cn/Article/details/ggxllcqxb.sHtML

[T38] Lua：条件
来源：http://mobile.fktsv.cn/Article/details/gmlqlvepw.sHtML

if x > 0 then print("正") end
来源：http://mobile.fktsv.cn/Article/details/grjaillfh.sHtML

[T39] Lua：模式匹配
来源：http://wap.bbcook.cn/Article/details/gtnozshuj.sHtML

string.find(s, "%d+")
来源：http://wap.epnwcf.com/Article/details/gkdravlbe.sHtML

[T40] Lua：元表
来源：http://wap.vehdjk.com/Article/details/ggxutjnwn.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.sjlbkw.cn/Article/details/grieyrvjr.sHtML

[T41] Perl：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/grpoeuinl.sHtML

print "Hello\n";
来源：http://m.share.sjlbkw.cn/Article/details/glzmpzsjp.sHtML

[T42] Perl：变量类型
来源：http://read.share.epnwcf.com/Article/details/glehznemp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.tarul.cn/Article/details/grkkzzfni.sHtML

[T43] Perl：字符串插值
来源：http://mobile.bbcook.cn/Article/details/gxqddzmaj.sHtML

"值: $a"
来源：http://www.m.share.yfazqb.com/Article/details/ggjbxbwuv.sHtML

[T44] Perl：条件
来源：http://www.share.sjlbkw.cn/Article/details/gmhavvarf.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fktsv.cn/Article/details/gqhsrnmcy.sHtML

[T45] Perl：数组遍历
来源：http://blog.tarul.cn/Article/details/gnofuedfk.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.tarul.cn/Article/details/gfmtpflph.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.vehdjk.com/Article/details/gqnkoiyvx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.yfazqb.com/Article/details/gpeehtwxq.sHtML

[T47] Perl：正则捕获
来源：http://blog.epnwcf.com/Article/details/gfelmhczr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.sjlbkw.cn/Article/details/grwuhjgwp.sHtML

[T48] Perl：正则替换
来源：http://3g.fktsv.cn/Article/details/gwitbltwa.sHtML

$s =~ s/old/new/g;
来源：http://wap.tarul.cn/Article/details/gygrbsxjq.sHtML

[T49] Perl：函数
来源：http://baike.bbcook.cn/Article/details/gxxsdsocx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gzydafbux.sHtML

[T50] Perl：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gtdpfjrud.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.yfazqb.com/Article/details/gqgxldpjq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.yfazqb.com/Article/details/gprovnelm.sHtML

[T51] Scala：Hello World
来源：http://www.share.bbcook.cn/Article/details/gpkrurzxm.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/gbhteiqdu.sHtML

[T52] Scala：变量
来源：http://m.share.tarul.cn/Article/details/gglltyqwi.sHtML

val a = 1;  var b = 2
来源：http://baike.bbcook.cn/Article/details/gbdwvlvww.sHtML

[T53] Scala：字符串插值
来源：http://baike.epnwcf.com/Article/details/gjdxkvkqx.sHtML

s"值: $b"
来源：http://www.blog.yfazqb.com/Article/details/gjbdvgeja.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.tarul.cn/Article/details/grxcrtzex.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fktsv.cn/Article/details/gobbjdear.sHtML

[T55] Scala：集合过滤
来源：http://wap.fktsv.cn/Article/details/ggvjehoqh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.sjlbkw.cn/Article/details/gbvmbaisn.sHtML

[T56] Scala：样例类
来源：http://blog.tarul.cn/Article/details/ggxmwdege.sHtML

case class User(name: String, age: Int)
来源：http://wap.vehdjk.com/Article/details/gijpetujg.sHtML

[T57] Scala：模式匹配
来源：http://3g.epnwcf.com/Article/details/gyoypclaz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.vehdjk.com/Article/details/gaidofziv.sHtML

[T58] Scala：函数定义
来源：http://blog.tarul.cn/Article/details/goktjpuet.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.vehdjk.com/Article/details/gnlnauxrf.sHtML

[T59] Scala：循环
来源：http://www.m.share.tarul.cn/Article/details/gzoygsgyv.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.sjlbkw.cn/Article/details/gzoqccoun.sHtML

[T60] Scala：折叠
来源：http://3g.vehdjk.com/Article/details/gkidzfarp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.yfazqb.com/Article/details/ggizocjak.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gpdzncrkx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.epnwcf.com/Article/details/goqktwzxb.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gdxbbflpj.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.tarul.cn/Article/details/grodcvreg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.vehdjk.com/Article/details/gojywymgg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.vehdjk.com/Article/details/gkyrrbvgt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.bbcook.cn/Article/details/ghmwpynig.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.vehdjk.com/Article/details/gxpqaenbj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.sjlbkw.cn/Article/details/gqxqnevgi.sHtML

[U04] Py：变量调试打印
来源：http://blog.sjlbkw.cn/Article/details/gmaayhxda.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fktsv.cn/Article/details/gjiqoyfya.sHtML

[U05] Py：列表去重且保序
来源：http://blog.sjlbkw.cn/Article/details/gqglfobbb.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/geigrqyzw.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fktsv.cn/Article/details/gcufawway.sHtML

{**a, **b}
来源：http://m.share.sjlbkw.cn/Article/details/gbhpldmhi.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fktsv.cn/Article/details/gdlynaoon.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fktsv.cn/Article/details/gewshgunz.sHtML

[U08] Py：展平二维列表
来源：http://blog.fktsv.cn/Article/details/gumgvvcrj.sHtML

[y for x in nested for y in x]
来源：http://baike.tarul.cn/Article/details/ghezosvuz.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fktsv.cn/Article/details/gittiprcs.sHtML

max(d, key=d.get)
来源：http://read.share.tarul.cn/Article/details/geoozzxta.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fktsv.cn/Article/details/gajmotexb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.tarul.cn/Article/details/gcbxcmzmh.sHtML

[U11] Py：生成器表达式
来源：http://mobile.bbcook.cn/Article/details/gjdclwezl.sHtML

(x * 2 for x in arr)
来源：http://3g.bbcook.cn/Article/details/grssfqiwc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.sjlbkw.cn/Article/details/gzhdytdql.sHtML

Counter(arr).most_common(3)
来源：http://m.share.bbcook.cn/Article/details/gngefwowx.sHtML

[U13] Py：固定长度队列
来源：http://www.share.vehdjk.com/Article/details/guazzgpxq.sHtML

deque(maxlen=10)
来源：http://3g.yfazqb.com/Article/details/grvjclcsw.sHtML

[U14] Py：分组收集到列表
来源：http://wap.epnwcf.com/Article/details/gddvtsyoj.sHtML

defaultdict(list)
来源：http://wap.bbcook.cn/Article/details/gdljocjhk.sHtML

[U15] Py：高精度计时
来源：http://m.share.sjlbkw.cn/Article/details/gsyrhauwr.sHtML

t = time.perf_counter()
来源：http://blog.epnwcf.com/Article/details/grlcncsjr.sHtML

[U16] Py：命令行参数解析
来源：http://baike.sjlbkw.cn/Article/details/gwgxrreow.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.vehdjk.com/Article/details/gzpwoskqe.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.epnwcf.com/Article/details/gukrymxjr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.epnwcf.com/Article/details/gtlsnyxcd.sHtML

[U18] Py：预编译正则
来源：http://3g.vehdjk.com/Article/details/gmmliibll.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.yfazqb.com/Article/details/gpjvauytp.sHtML

[U19] Py：正则替换带回调
来源：http://wap.bbcook.cn/Article/details/goasysqkq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.sjlbkw.cn/Article/details/ghkmmcbnf.sHtML

[U20] Py：缓存函数结果
来源：http://blog.vehdjk.com/Article/details/gmtejzbor.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.vehdjk.com/Article/details/geqxhuqoz.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.epnwcf.com/Article/details/gggrjbldb.sHtML

@contextlib.contextmanager
来源：http://baike.yfazqb.com/Article/details/gddcftzme.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fktsv.cn/Article/details/gscpxjklk.sHtML

list(zip(*m))
来源：http://wap.sjlbkw.cn/Article/details/gnlqbezsc.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.vehdjk.com/Article/details/gbzspotnz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.bbcook.cn/Article/details/gznwulcjk.sHtML

[U24] Py：路径操作
来源：http://mobile.tarul.cn/Article/details/gsrjymoej.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.sjlbkw.cn/Article/details/grxbskuex.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.bbcook.cn/Article/details/gqaepsowz.sHtML

csv.DictReader(f)
来源：http://3g.epnwcf.com/Article/details/gkpwbfedl.sHtML

[U26] Py：并发下载
来源：http://3g.epnwcf.com/Article/details/gxoxiqrir.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.sjlbkw.cn/Article/details/geqkyktdi.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fktsv.cn/Article/details/giynajlaz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fktsv.cn/Article/details/gjxtjoatc.sHtML

[U28] Py：类型别名
来源：http://www.blog.yfazqb.com/Article/details/gassajsqb.sHtML

UserId = int
来源：http://mobile.epnwcf.com/Article/details/gsxbglofe.sHtML

[U29] Py：属性校验
来源：http://mobile.sjlbkw.cn/Article/details/gcoohxejg.sHtML

@property 与 @x.setter 配合
来源：http://baike.vehdjk.com/Article/details/grjxoaxau.sHtML

[U30] Py：数据类
来源：http://m.share.yfazqb.com/Article/details/gdzdyzzel.sHtML

@dataclass(slots=True)
来源：http://blog.yfazqb.com/Article/details/gctuwqvne.sHtML

[U31] Py：单测
来源：http://baike.fktsv.cn/Article/details/ggmvizjzu.sHtML

python -m pytest -q
来源：http://mobile.tarul.cn/Article/details/gpndufcqf.sHtML

[U32] Py：代码格式化
来源：http://www.share.vehdjk.com/Article/details/gacdvfycb.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.epnwcf.com/Article/details/gtjhjpchq.sHtML

[U33] Py：打包发布
来源：http://m.share.tarul.cn/Article/details/giozptbkm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.epnwcf.com/Article/details/gefzexykh.sHtML

[U34] Py：判断编码
来源：http://baike.yfazqb.com/Article/details/ghwfazryy.sHtML

chardet.detect(raw)
来源：http://www.share.sjlbkw.cn/Article/details/ghksokibr.sHtML

[U35] Py：发送邮件
来源：http://m.share.tarul.cn/Article/details/gzkegkxpg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.tarul.cn/Article/details/gtsodhmoj.sHtML

[U36] Py：定时任务
来源：http://www.share.yfazqb.com/Article/details/gmrjamqdu.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fktsv.cn/Article/details/gqqzzgskk.sHtML

[U37] Py：读写 Excel
来源：http://www.share.vehdjk.com/Article/details/geuytmqyn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fktsv.cn/Article/details/gnpuvmylp.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.yfazqb.com/Article/details/gjsfhtxmh.sHtML

Path(__file__).resolve().parent
来源：http://www.share.bbcook.cn/Article/details/gycmvjmap.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.sjlbkw.cn/Article/details/gaoglupmz.sHtML

sys.stdout.isatty()
来源：http://mobile.fktsv.cn/Article/details/gslsnjhqy.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.epnwcf.com/Article/details/guekpipdy.sHtML

print("err", file=sys.stderr)
来源：http://m.share.bbcook.cn/Article/details/gjtziehtd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.epnwcf.com/Article/details/gtflnvdqm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.sjlbkw.cn/Article/details/ggxqifmck.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.epnwcf.com/Article/details/gslgoylbd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.yfazqb.com/Article/details/gktmjyqfy.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.sjlbkw.cn/Article/details/gpdcotlbr.sHtML

namespace App\Http;
来源：http://blog.tarul.cn/Article/details/grtlylrxk.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.vehdjk.com/Article/details/gocpcqibb.sHtML

declare(strict_types=1);
来源：http://m.share.sjlbkw.cn/Article/details/gtgcdyafg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.vehdjk.com/Article/details/gyaykgzpy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/grniwunsd.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.vehdjk.com/Article/details/gabwstepo.sHtML

?string $name = null
来源：http://3g.vehdjk.com/Article/details/giamihhhx.sHtML

[U47] PHP：联合类型
来源：http://blog.vehdjk.com/Article/details/gejunywbh.sHtML

int|string $id
来源：http://www.m.share.tarul.cn/Article/details/gdsofidmp.sHtML

[U48] PHP：纯枚举
来源：http://baike.bbcook.cn/Article/details/gbullongg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.vehdjk.com/Article/details/gluibwdtx.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.tarul.cn/Article/details/gmernmrvz.sHtML

public readonly string $name
来源：http://mobile.sjlbkw.cn/Article/details/gvjfziehy.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.vehdjk.com/Article/details/gcfpmwhol.sHtML

public function __construct(private int $id) {}
来源：http://mobile.epnwcf.com/Article/details/ghusnefzc.sHtML

[U51] PHP：数组解构
来源：http://baike.tarul.cn/Article/details/ghjpwpfmd.sHtML

[$a, $b] = $arr;
来源：http://www.share.epnwcf.com/Article/details/gortkytmg.sHtML

[U52] PHP：箭头函数
来源：http://3g.tarul.cn/Article/details/gdileqqor.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fktsv.cn/Article/details/gxevqopbb.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.epnwcf.com/Article/details/gdkcmbfij.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fktsv.cn/Article/details/gyuyihukp.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.vehdjk.com/Article/details/genxczzzg.sHtML

$obj?->method()
来源：http://baike.bbcook.cn/Article/details/gelbbboob.sHtML

[U55] PHP：match 表达式
来源：http://mobile.tarul.cn/Article/details/gwfzncojt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.epnwcf.com/Article/details/gmqdccmbv.sHtML

[U56] PHP：命名参数
来源：http://blog.sjlbkw.cn/Article/details/gwjfcdizz.sHtML

f(a: 1, b: 2)
来源：http://baike.tarul.cn/Article/details/gnnvipinv.sHtML

[U57] PHP：字符串插值
来源：http://baike.fktsv.cn/Article/details/gjsovtihu.sHtML

"值: {$a}"
来源：http://3g.fktsv.cn/Article/details/gtuiuseis.sHtML

[U58] PHP：数组三件套
来源：http://m.share.epnwcf.com/Article/details/gmnxhklul.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.bbcook.cn/Article/details/gtmelhfsp.sHtML

[U59] PHP：自定义排序
来源：http://3g.yfazqb.com/Article/details/grfetwxxo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.vehdjk.com/Article/details/gdpxyfxgx.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.epnwcf.com/Article/details/grxyfyzkg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.bbcook.cn/Article/details/gunqecrsu.sHtML

[U61] PHP：正则
来源：http://www.m.share.vehdjk.com/Article/details/gxywjnmkf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.bbcook.cn/Article/details/grsupjvjf.sHtML

[U62] PHP：日期对象
来源：http://blog.fktsv.cn/Article/details/gildgwjye.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.tarul.cn/Article/details/gudhahxbq.sHtML

[U63] PHP：文件读写
来源：http://wap.tarul.cn/Article/details/gqnhucxzx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.tarul.cn/Article/details/gerfucqvv.sHtML

[U64] PHP：目录遍历
来源：http://wap.vehdjk.com/Article/details/gqhaospic.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.yfazqb.com/Article/details/gquyvfyjn.sHtML

[U65] PHP：会话
来源：http://mobile.tarul.cn/Article/details/gkitoezyb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gzmpgpkxw.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.epnwcf.com/Article/details/gwhthakgx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.tarul.cn/Article/details/gzzqqkdgk.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fktsv.cn/Article/details/gkeuzfgpw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.tarul.cn/Article/details/gigalmuso.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.vehdjk.com/Article/details/gxptrohic.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.bbcook.cn/Article/details/glpzupqre.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.epnwcf.com/Article/details/gnddgejhb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.vehdjk.com/Article/details/gcammmmro.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gbajbwgoz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.tarul.cn/Article/details/gtdowgwrh.sHtML


<!-- 参考信息 -->