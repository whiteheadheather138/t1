代发 wailian999

[S45] C++：lambda
来源：http://3g.sjlbkw.cn/Article/details/gfjwixnez.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.epnwcf.com/Article/details/gogznwqtq.sHtML

[S46] C++：函数模板
来源：http://www.share.epnwcf.com/Article/details/gskoiolvo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fktsv.cn/Article/details/gzroeyxvo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.vehdjk.com/Article/details/geclniefx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.epnwcf.com/Article/details/gcoovmyhk.sHtML

[S48] C++：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gewofuzmd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.tarul.cn/Article/details/gmzhitnes.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.epnwcf.com/Article/details/gqeqjbxed.sHtML

[S49] C++：写文件
来源：http://m.share.tarul.cn/Article/details/gomrylpzm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.tarul.cn/Article/details/gzleztdsg.sHtML

[S50] C++：格式化数字
来源：http://mobile.epnwcf.com/Article/details/gjoocsrza.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.vehdjk.com/Article/details/ghpktowcd.sHtML

[S51] C++：显式类型转换
来源：http://m.share.vehdjk.com/Article/details/guqmjbatg.sHtML

static_cast<double>(a) / b
来源：http://www.blog.vehdjk.com/Article/details/guzfibbjz.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.yfazqb.com/Article/details/gukzimfcx.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.tarul.cn/Article/details/gzselhgoi.sHtML

[S53] C++：移动语义
来源：http://wap.bbcook.cn/Article/details/girtnzasw.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.bbcook.cn/Article/details/gmsjagggr.sHtML

[S54] C++：异常处理
来源：http://mobile.sjlbkw.cn/Article/details/gedjyfktt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.bbcook.cn/Article/details/gqiizdtnc.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fktsv.cn/Article/details/gcvjlcufg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.bbcook.cn/Article/details/gzrsrxwnq.sHtML

[S56] C++：optional
来源：http://read.share.yfazqb.com/Article/details/guioidsgm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.sjlbkw.cn/Article/details/gchkckrws.sHtML

[S57] C++：编译期常量
来源：http://mobile.sjlbkw.cn/Article/details/gfdjtykkg.sHtML

constexpr int N = 10;
来源：http://wap.sjlbkw.cn/Article/details/glsxnbdge.sHtML

[S58] C++：命名空间
来源：http://www.m.share.epnwcf.com/Article/details/ghxarsice.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.bbcook.cn/Article/details/gqeftihpf.sHtML

[S59] C++：静态断言
来源：http://www.share.sjlbkw.cn/Article/details/giffqavji.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.epnwcf.com/Article/details/gesexlxpj.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.sjlbkw.cn/Article/details/gpcgscrrv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.bbcook.cn/Article/details/gfxmzfvxx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gsqciwhcn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.tarul.cn/Article/details/gwuvwdrjm.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gavwjyuga.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.tarul.cn/Article/details/grlphsqmu.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/gamdogygm.sHtML

[T02] Kotlin：变量
来源：http://m.share.tarul.cn/Article/details/gsktriidy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.bbcook.cn/Article/details/gjvwxlyjx.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fktsv.cn/Article/details/ghynpeeyi.sHtML

"值: $b"
来源：http://www.share.fktsv.cn/Article/details/gncpbjokh.sHtML

[T04] Kotlin：空安全
来源：http://blog.fktsv.cn/Article/details/gtzeodcgs.sHtML

val n: String? = null;  n?.length
来源：http://wap.epnwcf.com/Article/details/gcsmacpwn.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fktsv.cn/Article/details/ghhfaghrg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.vehdjk.com/Article/details/ggjbkngat.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.sjlbkw.cn/Article/details/gylxuaxmf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.tarul.cn/Article/details/glirkscnr.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fktsv.cn/Article/details/gejruzndy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.tarul.cn/Article/details/gwlibnhpp.sHtML

[T08] Kotlin：数据类
来源：http://blog.bbcook.cn/Article/details/gogcjswcv.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.bbcook.cn/Article/details/gougjgesr.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fktsv.cn/Article/details/gftzpyjbi.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.epnwcf.com/Article/details/garcmsmzr.sHtML

[T10] Kotlin：默认参数
来源：http://3g.sjlbkw.cn/Article/details/gurqxldtb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.vehdjk.com/Article/details/gpekiufnp.sHtML

[T11] Kotlin：协程
来源：http://blog.sjlbkw.cn/Article/details/gftwqzwya.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.epnwcf.com/Article/details/gcftdfutm.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fktsv.cn/Article/details/gizdhqiun.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gxfgapgbo.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.bbcook.cn/Article/details/gmrredzjo.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.bbcook.cn/Article/details/gwisfndaq.sHtML

[T14] Kotlin：循环
来源：http://www.blog.vehdjk.com/Article/details/gjamlxtnt.sHtML

for (i in 1..10) println(i)
来源：http://read.share.vehdjk.com/Article/details/gsjruywbo.sHtML

[T15] Kotlin：接口
来源：http://read.share.tarul.cn/Article/details/gkyzvfzfm.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.tarul.cn/Article/details/ggqomdkvy.sHtML

[T16] Swift：Hello World
来源：http://blog.epnwcf.com/Article/details/gszxlllrs.sHtML

print("Hello")
来源：http://wap.bbcook.cn/Article/details/gxeejdnrv.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fktsv.cn/Article/details/gurroyoij.sHtML

var a = 1;  let b = 2
来源：http://wap.tarul.cn/Article/details/gvzlcinrh.sHtML

[T18] Swift：字符串插值
来源：http://mobile.vehdjk.com/Article/details/glicyhwzf.sHtML

"值: \(b)"
来源：http://www.blog.yfazqb.com/Article/details/gfzxusaev.sHtML

[T19] Swift：可选绑定
来源：http://www.share.epnwcf.com/Article/details/gmdrsoohh.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.tarul.cn/Article/details/gcuzqqfuh.sHtML

[T20] Swift：数组操作
来源：http://mobile.sjlbkw.cn/Article/details/ggitbygxx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.epnwcf.com/Article/details/gqyexfukt.sHtML

[T21] Swift：遍历
来源：http://www.share.bbcook.cn/Article/details/gozivcdxa.sHtML

for x in a { print(x) }
来源：http://www.blog.epnwcf.com/Article/details/ggucklupd.sHtML

[T22] Swift：字典
来源：http://www.blog.fktsv.cn/Article/details/githqmfds.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.vehdjk.com/Article/details/gyaxoffta.sHtML

[T23] Swift：函数
来源：http://wap.fktsv.cn/Article/details/gyokqusqg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.vehdjk.com/Article/details/gnjedujvd.sHtML

[T24] Swift：闭包
来源：http://blog.bbcook.cn/Article/details/glzvzxoco.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.bbcook.cn/Article/details/gbovklavm.sHtML

[T25] Swift：结构体
来源：http://m.share.yfazqb.com/Article/details/gepovcolh.sHtML

struct P { var x: Int }
来源：http://www.blog.epnwcf.com/Article/details/gthunfhkp.sHtML

[T26] Swift：类与重写
来源：http://mobile.vehdjk.com/Article/details/ghtkonrxh.sHtML

class A: Base { override func f() {} }
来源：http://blog.epnwcf.com/Article/details/gvpnhgnac.sHtML

[T27] Swift：错误处理
来源：http://m.share.yfazqb.com/Article/details/gcmxjzevq.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.yfazqb.com/Article/details/gfqtddpdb.sHtML

[T28] Swift：枚举
来源：http://mobile.yfazqb.com/Article/details/gwwadssku.sHtML

enum Color { case red, green }
来源：http://wap.tarul.cn/Article/details/gqwugqvab.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.bbcook.cn/Article/details/gjmmodxvo.sHtML

guard let x = opt else { return }
来源：http://mobile.sjlbkw.cn/Article/details/gwmvoboen.sHtML

[T30] Swift：协议
来源：http://www.share.yfazqb.com/Article/details/ghkynbokv.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.vehdjk.com/Article/details/gjbpjmzgx.sHtML

[T31] Lua：Hello World
来源：http://blog.yfazqb.com/Article/details/gfiolkysf.sHtML

print("Hello")
来源：http://mobile.yfazqb.com/Article/details/gcxlnaham.sHtML

[T32] Lua：局部变量
来源：http://read.share.bbcook.cn/Article/details/gathlagfz.sHtML

local a = 1
来源：http://read.share.tarul.cn/Article/details/gvfqaufcx.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.epnwcf.com/Article/details/gaxcsvqed.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.epnwcf.com/Article/details/goaxxwfql.sHtML

[T34] Lua：遍历表
来源：http://m.share.fktsv.cn/Article/details/gzfsthpjx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.tarul.cn/Article/details/gljbucwgu.sHtML

[T35] Lua：字典表
来源：http://www.share.sjlbkw.cn/Article/details/gjcjkkqzm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fktsv.cn/Article/details/gbxofryxl.sHtML

[T36] Lua：函数
来源：http://www.share.fktsv.cn/Article/details/ghdmbrkjj.sHtML

function add(a, b) return a + b end
来源：http://mobile.tarul.cn/Article/details/gfpkdacek.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.epnwcf.com/Article/details/gxolsvnfr.sHtML

"a" .. "b"
来源：http://wap.epnwcf.com/Article/details/gwcwlgzfx.sHtML

[T38] Lua：条件
来源：http://baike.sjlbkw.cn/Article/details/gjemeabcf.sHtML

if x > 0 then print("正") end
来源：http://3g.epnwcf.com/Article/details/gaahrhtcf.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/glooufjlx.sHtML

string.find(s, "%d+")
来源：http://baike.yfazqb.com/Article/details/gclpfiyqi.sHtML

[T40] Lua：元表
来源：http://blog.epnwcf.com/Article/details/grwgmgrsx.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.bbcook.cn/Article/details/grvpvjtxh.sHtML

[T41] Perl：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gvyfvpsiw.sHtML

print "Hello\n";
来源：http://3g.tarul.cn/Article/details/gjnlkylhn.sHtML

[T42] Perl：变量类型
来源：http://3g.sjlbkw.cn/Article/details/gngszignm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.vehdjk.com/Article/details/gotravfzg.sHtML

[T43] Perl：字符串插值
来源：http://baike.tarul.cn/Article/details/gvhvpvhqs.sHtML

"值: $a"
来源：http://www.share.sjlbkw.cn/Article/details/gxmkqdqtb.sHtML

[T44] Perl：条件
来源：http://3g.vehdjk.com/Article/details/gsgohjhig.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.epnwcf.com/Article/details/gltmxutis.sHtML

[T45] Perl：数组遍历
来源：http://mobile.yfazqb.com/Article/details/ghvrzbaxj.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.tarul.cn/Article/details/gznzoxyji.sHtML

[T46] Perl：哈希操作
来源：http://mobile.vehdjk.com/Article/details/gqdorsjak.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.epnwcf.com/Article/details/gajjkmcuy.sHtML

[T47] Perl：正则捕获
来源：http://blog.yfazqb.com/Article/details/gxogoyrpp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.vehdjk.com/Article/details/gqrzcqnil.sHtML

[T48] Perl：正则替换
来源：http://blog.sjlbkw.cn/Article/details/govjgrhjd.sHtML

$s =~ s/old/new/g;
来源：http://wap.sjlbkw.cn/Article/details/gwxhalsbt.sHtML

[T49] Perl：函数
来源：http://wap.vehdjk.com/Article/details/gqdtggerb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gejuwceqp.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gylqpqbfl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fktsv.cn/Article/details/gqjuwqqpt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gnpmuvyuv.sHtML

[T51] Scala：Hello World
来源：http://m.share.yfazqb.com/Article/details/gvfirrdke.sHtML

println("Hello")
来源：http://m.share.vehdjk.com/Article/details/gbowqcdpf.sHtML

[T52] Scala：变量
来源：http://3g.epnwcf.com/Article/details/gabvpgnps.sHtML

val a = 1;  var b = 2
来源：http://www.share.bbcook.cn/Article/details/gwqmpqhjd.sHtML

[T53] Scala：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gauukgbtp.sHtML

s"值: $b"
来源：http://www.m.share.fktsv.cn/Article/details/gejdhdloc.sHtML

[T54] Scala：集合映射
来源：http://www.blog.tarul.cn/Article/details/giizyvgmz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.bbcook.cn/Article/details/gccexkfie.sHtML

[T55] Scala：集合过滤
来源：http://wap.vehdjk.com/Article/details/gbalnbjrm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.tarul.cn/Article/details/gykymdkli.sHtML

[T56] Scala：样例类
来源：http://blog.yfazqb.com/Article/details/gqxeykjmy.sHtML

case class User(name: String, age: Int)
来源：http://wap.tarul.cn/Article/details/gfjtkoydm.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.bbcook.cn/Article/details/gduoamxrz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.bbcook.cn/Article/details/gnxxarmbi.sHtML

[T58] Scala：函数定义
来源：http://mobile.epnwcf.com/Article/details/gpwgvojny.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.sjlbkw.cn/Article/details/gdwdfbhzu.sHtML

[T59] Scala：循环
来源：http://www.blog.yfazqb.com/Article/details/gesnmokcn.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.bbcook.cn/Article/details/gbnoiedok.sHtML

[T60] Scala：折叠
来源：http://www.blog.fktsv.cn/Article/details/gnxqlmkgz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.vehdjk.com/Article/details/gakcootav.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gzevdyxfu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.sjlbkw.cn/Article/details/gjnhdtrhj.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gnzgydnil.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.bbcook.cn/Article/details/gpvoidptz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.vehdjk.com/Article/details/gnjfjuvsq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fktsv.cn/Article/details/gmowsaijx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.tarul.cn/Article/details/grummdobv.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.tarul.cn/Article/details/gfbiygkma.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.vehdjk.com/Article/details/gbjrakmtt.sHtML

[U04] Py：变量调试打印
来源：http://blog.fktsv.cn/Article/details/ggvnzocex.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.sjlbkw.cn/Article/details/ggrpzpqlp.sHtML

[U05] Py：列表去重且保序
来源：http://3g.epnwcf.com/Article/details/gczixrbsb.sHtML

list(dict.fromkeys(arr))
来源：http://blog.tarul.cn/Article/details/guyjegrdk.sHtML

[U06] Py：合并两个字典
来源：http://www.share.yfazqb.com/Article/details/gyrsesnjx.sHtML

{**a, **b}
来源：http://www.share.fktsv.cn/Article/details/gujrfbmgc.sHtML

[U07] Py：反转字典键值
来源：http://m.share.yfazqb.com/Article/details/gxfdhxajd.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.tarul.cn/Article/details/gmfippnlj.sHtML

[U08] Py：展平二维列表
来源：http://read.share.bbcook.cn/Article/details/gifhmzwho.sHtML

[y for x in nested for y in x]
来源：http://baike.sjlbkw.cn/Article/details/gcntcfqbm.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.yfazqb.com/Article/details/ggxnnndhk.sHtML

max(d, key=d.get)
来源：http://read.share.yfazqb.com/Article/details/gmuctjxqs.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.sjlbkw.cn/Article/details/ghtcjbghn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.bbcook.cn/Article/details/gvrovcffu.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fktsv.cn/Article/details/gngfantoy.sHtML

(x * 2 for x in arr)
来源：http://www.blog.yfazqb.com/Article/details/gncijynzh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.tarul.cn/Article/details/ghcpopjjp.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.epnwcf.com/Article/details/gesomvixz.sHtML

[U13] Py：固定长度队列
来源：http://3g.vehdjk.com/Article/details/gbtnmzogp.sHtML

deque(maxlen=10)
来源：http://blog.sjlbkw.cn/Article/details/gdtnrwouu.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.yfazqb.com/Article/details/geljfbcjo.sHtML

defaultdict(list)
来源：http://3g.fktsv.cn/Article/details/gztkuxzly.sHtML

[U15] Py：高精度计时
来源：http://www.blog.vehdjk.com/Article/details/grutkmbyf.sHtML

t = time.perf_counter()
来源：http://3g.vehdjk.com/Article/details/gobemfydv.sHtML

[U16] Py：命令行参数解析
来源：http://3g.epnwcf.com/Article/details/gluwjowbr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fktsv.cn/Article/details/gjmbydqhb.sHtML

[U17] Py：初始化日志
来源：http://wap.bbcook.cn/Article/details/ghjelubyl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.bbcook.cn/Article/details/gdyrrxysr.sHtML

[U18] Py：预编译正则
来源：http://m.share.tarul.cn/Article/details/gvmpqwjhi.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.sjlbkw.cn/Article/details/gbvifvhyz.sHtML

[U19] Py：正则替换带回调
来源：http://3g.epnwcf.com/Article/details/gkstzqimh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.yfazqb.com/Article/details/gdknnlorb.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fktsv.cn/Article/details/gkecspuna.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fktsv.cn/Article/details/gzdzhxfto.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.tarul.cn/Article/details/giqromgop.sHtML

@contextlib.contextmanager
来源：http://read.share.yfazqb.com/Article/details/gvtkktrgi.sHtML

[U22] Py：矩阵转置
来源：http://www.share.vehdjk.com/Article/details/gxkxxkkwv.sHtML

list(zip(*m))
来源：http://www.m.share.bbcook.cn/Article/details/ghgreuozl.sHtML

[U23] Py：分块读取大文件
来源：http://wap.epnwcf.com/Article/details/ghoeviozq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.sjlbkw.cn/Article/details/gpwdwrfuz.sHtML

[U24] Py：路径操作
来源：http://m.share.fktsv.cn/Article/details/gcaklcjqv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/geqxsywsz.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.yfazqb.com/Article/details/gymeqxmzc.sHtML

csv.DictReader(f)
来源：http://read.share.fktsv.cn/Article/details/ghubzqhpa.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fktsv.cn/Article/details/grdupflke.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.vehdjk.com/Article/details/gnoxlyinv.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fktsv.cn/Article/details/gfzrpssnn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.bbcook.cn/Article/details/gqrjnuonx.sHtML

[U28] Py：类型别名
来源：http://www.m.share.bbcook.cn/Article/details/gfkrsigsw.sHtML

UserId = int
来源：http://www.blog.fktsv.cn/Article/details/geimcsffz.sHtML

[U29] Py：属性校验
来源：http://www.m.share.vehdjk.com/Article/details/gmmsktdvd.sHtML

@property 与 @x.setter 配合
来源：http://mobile.vehdjk.com/Article/details/gtzjroduq.sHtML

[U30] Py：数据类
来源：http://blog.yfazqb.com/Article/details/gjbjjlkgg.sHtML

@dataclass(slots=True)
来源：http://blog.yfazqb.com/Article/details/gwtxuopwi.sHtML

[U31] Py：单测
来源：http://www.share.fktsv.cn/Article/details/gyaqquaby.sHtML

python -m pytest -q
来源：http://m.share.yfazqb.com/Article/details/ghtlalyeb.sHtML

[U32] Py：代码格式化
来源：http://baike.vehdjk.com/Article/details/giapyoqej.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.vehdjk.com/Article/details/gkfbtproz.sHtML

[U33] Py：打包发布
来源：http://wap.tarul.cn/Article/details/gxgkllyvh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.tarul.cn/Article/details/guogsbqbu.sHtML

[U34] Py：判断编码
来源：http://www.share.tarul.cn/Article/details/goqfzhson.sHtML

chardet.detect(raw)
来源：http://www.blog.sjlbkw.cn/Article/details/gnragiyhe.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.bbcook.cn/Article/details/gcgujzjcd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.epnwcf.com/Article/details/gskfbccbj.sHtML

[U36] Py：定时任务
来源：http://mobile.vehdjk.com/Article/details/gqqtbktxy.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.epnwcf.com/Article/details/gactbmipr.sHtML

[U37] Py：读写 Excel
来源：http://blog.tarul.cn/Article/details/gylnwlanm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.epnwcf.com/Article/details/gskanyrhx.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.bbcook.cn/Article/details/gxeprhlkz.sHtML

Path(__file__).resolve().parent
来源：http://3g.bbcook.cn/Article/details/gevbkxrsa.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.yfazqb.com/Article/details/gphderzwu.sHtML

sys.stdout.isatty()
来源：http://www.m.share.epnwcf.com/Article/details/gtcydfgcr.sHtML

[U40] Py：打印到标准错误
来源：http://3g.vehdjk.com/Article/details/gaufjiptb.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.yfazqb.com/Article/details/gibvizclx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fktsv.cn/Article/details/gwttgtdcp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.sjlbkw.cn/Article/details/gdkwzktbv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.epnwcf.com/Article/details/gbkacycsc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.vehdjk.com/Article/details/ggzzzzgba.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fktsv.cn/Article/details/gnviwsvxp.sHtML

namespace App\Http;
来源：http://blog.vehdjk.com/Article/details/gvpxgynnp.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.bbcook.cn/Article/details/gafelbjlb.sHtML

declare(strict_types=1);
来源：http://www.share.fktsv.cn/Article/details/gejtqiyqq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fktsv.cn/Article/details/gmdagdgnq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/glacidewi.sHtML

[U46] PHP：可空类型
来源：http://wap.yfazqb.com/Article/details/ghrqhplkn.sHtML

?string $name = null
来源：http://mobile.yfazqb.com/Article/details/gcntniabg.sHtML

[U47] PHP：联合类型
来源：http://www.share.vehdjk.com/Article/details/gmdpfsgzm.sHtML

int|string $id
来源：http://www.m.share.sjlbkw.cn/Article/details/gzroiymyn.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.vehdjk.com/Article/details/gdzqzqmff.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.vehdjk.com/Article/details/ggbitvcre.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.bbcook.cn/Article/details/gkwyailzo.sHtML

public readonly string $name
来源：http://baike.bbcook.cn/Article/details/gkkstficn.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.tarul.cn/Article/details/givkrasil.sHtML

public function __construct(private int $id) {}
来源：http://wap.yfazqb.com/Article/details/gylpdlodf.sHtML

[U51] PHP：数组解构
来源：http://www.blog.vehdjk.com/Article/details/gjnultvdk.sHtML

[$a, $b] = $arr;
来源：http://read.share.epnwcf.com/Article/details/gtshdnwfa.sHtML

[U52] PHP：箭头函数
来源：http://mobile.sjlbkw.cn/Article/details/glcrwjvuq.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.bbcook.cn/Article/details/gszagiojq.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.sjlbkw.cn/Article/details/gogsszpvl.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.tarul.cn/Article/details/gvdepklah.sHtML

[U54] PHP：空安全调用
来源：http://mobile.sjlbkw.cn/Article/details/gtctrcfvl.sHtML

$obj?->method()
来源：http://www.share.bbcook.cn/Article/details/gopefpqtm.sHtML

[U55] PHP：match 表达式
来源：http://mobile.epnwcf.com/Article/details/gpvtbwazl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.tarul.cn/Article/details/gqcipicku.sHtML

[U56] PHP：命名参数
来源：http://www.blog.yfazqb.com/Article/details/gxmbkgeay.sHtML

f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gnqlsdaxc.sHtML

[U57] PHP：字符串插值
来源：http://baike.yfazqb.com/Article/details/gmhefykmq.sHtML

"值: {$a}"
来源：http://www.share.vehdjk.com/Article/details/gjlguatqw.sHtML

[U58] PHP：数组三件套
来源：http://3g.bbcook.cn/Article/details/gfcgnunna.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.epnwcf.com/Article/details/gwlohhkyp.sHtML

[U59] PHP：自定义排序
来源：http://mobile.epnwcf.com/Article/details/ghhpegegw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.vehdjk.com/Article/details/gcoklzbem.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.sjlbkw.cn/Article/details/goxislqov.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.yfazqb.com/Article/details/gwzugquqz.sHtML

[U61] PHP：正则
来源：http://www.share.epnwcf.com/Article/details/gnmivctzt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.tarul.cn/Article/details/gkiwosrxy.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.bbcook.cn/Article/details/gtijokomm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fktsv.cn/Article/details/gsbtmgszq.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.vehdjk.com/Article/details/gnjhjpupe.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.bbcook.cn/Article/details/geztkcold.sHtML

[U64] PHP：目录遍历
来源：http://3g.tarul.cn/Article/details/gxgmhtisr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.tarul.cn/Article/details/gjexsyouo.sHtML

[U65] PHP：会话
来源：http://www.share.sjlbkw.cn/Article/details/gtlpuwoyx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gvhnmkvks.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.tarul.cn/Article/details/gwqrahibo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.vehdjk.com/Article/details/gzbrmpivu.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.tarul.cn/Article/details/gdaovqwhn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.bbcook.cn/Article/details/gylqxeqvn.sHtML

[U68] PHP：PDO 连接
来源：http://wap.bbcook.cn/Article/details/gdxujiyor.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.vehdjk.com/Article/details/gykznwudq.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.epnwcf.com/Article/details/gymabjymn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.yfazqb.com/Article/details/glkfhruwr.sHtML

[U70] PHP：PDO 事务
来源：http://baike.sjlbkw.cn/Article/details/gsusqhvdg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.bbcook.cn/Article/details/ggnrqrczz.sHtML


<!-- 参考信息 -->