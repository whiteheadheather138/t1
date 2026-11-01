代发 wailian999

[S45] C++：lambda
来源：http://www.m.share.tarul.cn/Article/details/gnkwfqsmt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.yfazqb.com/Article/details/gtlgxjqiz.sHtML

[S46] C++：函数模板
来源：http://blog.tarul.cn/Article/details/gsiskmcsn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.yfazqb.com/Article/details/gqlowshmb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.epnwcf.com/Article/details/geuliukny.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.sjlbkw.cn/Article/details/gkacbwiol.sHtML

[S48] C++：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gcpuhcegy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.yfazqb.com/Article/details/gukfmcwbl.sHtML

while (std::getline(in, line)) { }
来源：http://baike.tarul.cn/Article/details/gvykqunlk.sHtML

[S49] C++：写文件
来源：http://read.share.fktsv.cn/Article/details/ghsaypndd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.bbcook.cn/Article/details/googkseyt.sHtML

[S50] C++：格式化数字
来源：http://www.blog.sjlbkw.cn/Article/details/gjznsfwnt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gdmfkbltf.sHtML

[S51] C++：显式类型转换
来源：http://m.share.bbcook.cn/Article/details/gqjxtcfko.sHtML

static_cast<double>(a) / b
来源：http://mobile.tarul.cn/Article/details/ggnwjjwck.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.epnwcf.com/Article/details/gvdxssjec.sHtML

int size() const noexcept { return n_; }
来源：http://blog.bbcook.cn/Article/details/gxfmdxggc.sHtML

[S53] C++：移动语义
来源：http://m.share.sjlbkw.cn/Article/details/gakebbwbu.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.yfazqb.com/Article/details/gexvoiokb.sHtML

[S54] C++：异常处理
来源：http://m.share.vehdjk.com/Article/details/gfzvgmptv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fktsv.cn/Article/details/gcsniaxns.sHtML

[S55] C++：结构化绑定
来源：http://www.share.sjlbkw.cn/Article/details/gljtwowvv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.tarul.cn/Article/details/gntgbuuhk.sHtML

[S56] C++：optional
来源：http://m.share.vehdjk.com/Article/details/gijpubdkw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fktsv.cn/Article/details/gaunsypxf.sHtML

[S57] C++：编译期常量
来源：http://read.share.epnwcf.com/Article/details/gzzlwpsay.sHtML

constexpr int N = 10;
来源：http://www.share.epnwcf.com/Article/details/guwkrlzem.sHtML

[S58] C++：命名空间
来源：http://blog.fktsv.cn/Article/details/gfyoylmzz.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.sjlbkw.cn/Article/details/gwfzorejl.sHtML

[S59] C++：静态断言
来源：http://read.share.yfazqb.com/Article/details/gsrtugtzq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.yfazqb.com/Article/details/guwljkqel.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fktsv.cn/Article/details/gdvgosrfy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.vehdjk.com/Article/details/gyjxcunyh.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gxlgegwyv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.bbcook.cn/Article/details/gbnutkxyh.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ghnobjajl.sHtML

[T01] Kotlin：Hello World
来源：http://wap.yfazqb.com/Article/details/ggqvymeuy.sHtML

println("Hello")
来源：http://read.share.yfazqb.com/Article/details/goizaxmrq.sHtML

[T02] Kotlin：变量
来源：http://wap.fktsv.cn/Article/details/goghnplox.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fktsv.cn/Article/details/ggfnfdlbh.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.vehdjk.com/Article/details/gjdulusjn.sHtML

"值: $b"
来源：http://blog.yfazqb.com/Article/details/gqxmkcern.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fktsv.cn/Article/details/gcxztxbpn.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.yfazqb.com/Article/details/gmevvacmv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.vehdjk.com/Article/details/gkllchjyr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.yfazqb.com/Article/details/gsnsavlag.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fktsv.cn/Article/details/guxxldhhe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.bbcook.cn/Article/details/gefphnyfp.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.yfazqb.com/Article/details/gapcowggn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fktsv.cn/Article/details/guomcsftd.sHtML

[T08] Kotlin：数据类
来源：http://read.share.epnwcf.com/Article/details/gxlnjlvsl.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fktsv.cn/Article/details/gmfmvkxws.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.bbcook.cn/Article/details/gjbqfioll.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.epnwcf.com/Article/details/gcxkmjjdc.sHtML

[T10] Kotlin：默认参数
来源：http://baike.tarul.cn/Article/details/gkopkqkjw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.vehdjk.com/Article/details/gtfdfwkqf.sHtML

[T11] Kotlin：协程
来源：http://wap.sjlbkw.cn/Article/details/grfyulfda.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.tarul.cn/Article/details/gpecurreb.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.yfazqb.com/Article/details/gcfrsmwuv.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.tarul.cn/Article/details/gckxmlodm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.sjlbkw.cn/Article/details/gwjdbtwol.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.sjlbkw.cn/Article/details/gwusxhlwx.sHtML

[T14] Kotlin：循环
来源：http://www.blog.vehdjk.com/Article/details/geozwidcz.sHtML

for (i in 1..10) println(i)
来源：http://mobile.tarul.cn/Article/details/gnopcsdfd.sHtML

[T15] Kotlin：接口
来源：http://www.blog.tarul.cn/Article/details/gparbbhst.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.vehdjk.com/Article/details/gjtbxarbx.sHtML

[T16] Swift：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gqprsthah.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/gtoalyncz.sHtML

[T17] Swift：变量与常量
来源：http://3g.tarul.cn/Article/details/gqjwewajk.sHtML

var a = 1;  let b = 2
来源：http://www.blog.epnwcf.com/Article/details/gfdhzgreq.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gmvanlsjl.sHtML

"值: \(b)"
来源：http://www.blog.sjlbkw.cn/Article/details/grkrorvzi.sHtML

[T19] Swift：可选绑定
来源：http://baike.vehdjk.com/Article/details/gbrkxlxtz.sHtML

if let n = opt { print(n) }
来源：http://read.share.vehdjk.com/Article/details/gngmtmyew.sHtML

[T20] Swift：数组操作
来源：http://read.share.fktsv.cn/Article/details/gifrakyty.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.tarul.cn/Article/details/gxnogkcpd.sHtML

[T21] Swift：遍历
来源：http://3g.bbcook.cn/Article/details/gatfhexnl.sHtML

for x in a { print(x) }
来源：http://3g.vehdjk.com/Article/details/gqlwnaruc.sHtML

[T22] Swift：字典
来源：http://www.m.share.bbcook.cn/Article/details/gfcunrbhl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.epnwcf.com/Article/details/gufjzkpss.sHtML

[T23] Swift：函数
来源：http://baike.bbcook.cn/Article/details/gustfuyjj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.vehdjk.com/Article/details/gyqfgedsj.sHtML

[T24] Swift：闭包
来源：http://m.share.epnwcf.com/Article/details/gfpkeikxk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.yfazqb.com/Article/details/gnqwyutnv.sHtML

[T25] Swift：结构体
来源：http://www.blog.vehdjk.com/Article/details/glzndyhfw.sHtML

struct P { var x: Int }
来源：http://baike.yfazqb.com/Article/details/gpruvcctc.sHtML

[T26] Swift：类与重写
来源：http://www.blog.vehdjk.com/Article/details/gzzmnmnqm.sHtML

class A: Base { override func f() {} }
来源：http://wap.yfazqb.com/Article/details/gbdukobvm.sHtML

[T27] Swift：错误处理
来源：http://3g.sjlbkw.cn/Article/details/gcshacepa.sHtML

do { try f() } catch { print(error) }
来源：http://baike.sjlbkw.cn/Article/details/ghlmlzpea.sHtML

[T28] Swift：枚举
来源：http://www.blog.fktsv.cn/Article/details/gyiepevuk.sHtML

enum Color { case red, green }
来源：http://read.share.sjlbkw.cn/Article/details/gaqpevkgs.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.sjlbkw.cn/Article/details/gvlaltwqn.sHtML

guard let x = opt else { return }
来源：http://baike.sjlbkw.cn/Article/details/gswffpqzr.sHtML

[T30] Swift：协议
来源：http://www.share.epnwcf.com/Article/details/gozdwzxiw.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.epnwcf.com/Article/details/gfffektdt.sHtML

[T31] Lua：Hello World
来源：http://mobile.vehdjk.com/Article/details/giaqyccpv.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/gtgksymci.sHtML

[T32] Lua：局部变量
来源：http://wap.bbcook.cn/Article/details/grzbtzegb.sHtML

local a = 1
来源：http://baike.vehdjk.com/Article/details/glnvhxeki.sHtML

[T33] Lua：表（数组）
来源：http://blog.bbcook.cn/Article/details/gxhvbwsas.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.yfazqb.com/Article/details/gbzwvqheq.sHtML

[T34] Lua：遍历表
来源：http://baike.epnwcf.com/Article/details/goiqtynwn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.bbcook.cn/Article/details/gagbetymp.sHtML

[T35] Lua：字典表
来源：http://wap.epnwcf.com/Article/details/gvbdllqhb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.tarul.cn/Article/details/gdnpvsoum.sHtML

[T36] Lua：函数
来源：http://baike.tarul.cn/Article/details/gutpazmqf.sHtML

function add(a, b) return a + b end
来源：http://www.blog.sjlbkw.cn/Article/details/gkoggfuuy.sHtML

[T37] Lua：字符串拼接
来源：http://3g.sjlbkw.cn/Article/details/gtsrrunnq.sHtML

"a" .. "b"
来源：http://m.share.yfazqb.com/Article/details/gfpsovnxw.sHtML

[T38] Lua：条件
来源：http://3g.bbcook.cn/Article/details/gmgwuynbw.sHtML

if x > 0 then print("正") end
来源：http://www.share.fktsv.cn/Article/details/gbwlfzkgl.sHtML

[T39] Lua：模式匹配
来源：http://read.share.yfazqb.com/Article/details/gsvothaaq.sHtML

string.find(s, "%d+")
来源：http://3g.sjlbkw.cn/Article/details/ggnuvdndm.sHtML

[T40] Lua：元表
来源：http://m.share.tarul.cn/Article/details/gcdmmbhaz.sHtML

setmetatable({}, { __index = base })
来源：http://wap.epnwcf.com/Article/details/gwzgmidbu.sHtML

[T41] Perl：Hello World
来源：http://www.blog.tarul.cn/Article/details/gjlrvdgya.sHtML

print "Hello\n";
来源：http://www.share.yfazqb.com/Article/details/gxrsvvfre.sHtML

[T42] Perl：变量类型
来源：http://3g.tarul.cn/Article/details/gpmrawkgh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.tarul.cn/Article/details/gngjtawmv.sHtML

[T43] Perl：字符串插值
来源：http://3g.vehdjk.com/Article/details/ghohikbns.sHtML

"值: $a"
来源：http://www.share.fktsv.cn/Article/details/gzhypfyeh.sHtML

[T44] Perl：条件
来源：http://www.m.share.fktsv.cn/Article/details/guchddrve.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.yfazqb.com/Article/details/gmejfzmub.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.bbcook.cn/Article/details/genxqjohv.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.vehdjk.com/Article/details/gvdgnmkjk.sHtML

[T46] Perl：哈希操作
来源：http://3g.tarul.cn/Article/details/gpkfqwbjt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.bbcook.cn/Article/details/gzyejsxhb.sHtML

[T47] Perl：正则捕获
来源：http://wap.sjlbkw.cn/Article/details/gpbadppom.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.epnwcf.com/Article/details/gplajgike.sHtML

[T48] Perl：正则替换
来源：http://wap.epnwcf.com/Article/details/gjlotkrbf.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.epnwcf.com/Article/details/gdiphuwhu.sHtML

[T49] Perl：函数
来源：http://www.m.share.epnwcf.com/Article/details/gazzpukup.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gfughsudp.sHtML

[T50] Perl：逐行读文件
来源：http://wap.epnwcf.com/Article/details/gxkvblbbt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fktsv.cn/Article/details/gikrfuafh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.vehdjk.com/Article/details/gilqvwikw.sHtML

[T51] Scala：Hello World
来源：http://m.share.yfazqb.com/Article/details/ghqqcvyjb.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/gapgbkvcn.sHtML

[T52] Scala：变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdyjyjsm.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fktsv.cn/Article/details/gbjaqcioh.sHtML

[T53] Scala：字符串插值
来源：http://blog.bbcook.cn/Article/details/gmrxadgde.sHtML

s"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/gpfipkyst.sHtML

[T54] Scala：集合映射
来源：http://blog.bbcook.cn/Article/details/gisnldygp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.vehdjk.com/Article/details/glvsovumx.sHtML

[T55] Scala：集合过滤
来源：http://blog.bbcook.cn/Article/details/gziwczeht.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.sjlbkw.cn/Article/details/glqjenqlg.sHtML

[T56] Scala：样例类
来源：http://www.m.share.tarul.cn/Article/details/ggenerker.sHtML

case class User(name: String, age: Int)
来源：http://3g.vehdjk.com/Article/details/gbhqukwdr.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.tarul.cn/Article/details/gimzjjfcy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.vehdjk.com/Article/details/ggiqpsefg.sHtML

[T58] Scala：函数定义
来源：http://mobile.tarul.cn/Article/details/gdelstwid.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.vehdjk.com/Article/details/gcpkwhmud.sHtML

[T59] Scala：循环
来源：http://read.share.sjlbkw.cn/Article/details/glggydlop.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fktsv.cn/Article/details/gefznrkfd.sHtML

[T60] Scala：折叠
来源：http://baike.sjlbkw.cn/Article/details/gzqfnedhj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.tarul.cn/Article/details/gxwfydvhm.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gelcyouer.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.epnwcf.com/Article/details/ghpyqvtez.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gqnovrclb.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.bbcook.cn/Article/details/gocabftlw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.sjlbkw.cn/Article/details/gyvbqbdgt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.tarul.cn/Article/details/gubmmpnib.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.yfazqb.com/Article/details/ggdvkzqbc.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.bbcook.cn/Article/details/gweraechr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.sjlbkw.cn/Article/details/gjwcpjffd.sHtML

[U04] Py：变量调试打印
来源：http://read.share.bbcook.cn/Article/details/gzfkfiwjh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.bbcook.cn/Article/details/gaiyaltka.sHtML

[U05] Py：列表去重且保序
来源：http://wap.bbcook.cn/Article/details/gxqgelfmo.sHtML

list(dict.fromkeys(arr))
来源：http://baike.tarul.cn/Article/details/gzlpvemcv.sHtML

[U06] Py：合并两个字典
来源：http://baike.fktsv.cn/Article/details/gcfpcqxgb.sHtML

{**a, **b}
来源：http://blog.yfazqb.com/Article/details/gpnqypazp.sHtML

[U07] Py：反转字典键值
来源：http://mobile.vehdjk.com/Article/details/gvcomteke.sHtML

{v: k for k, v in d.items()}
来源：http://wap.tarul.cn/Article/details/gdqoydtho.sHtML

[U08] Py：展平二维列表
来源：http://read.share.tarul.cn/Article/details/grgihghyj.sHtML

[y for x in nested for y in x]
来源：http://m.share.sjlbkw.cn/Article/details/gxjyqrpir.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.sjlbkw.cn/Article/details/gkmcyspwi.sHtML

max(d, key=d.get)
来源：http://www.share.yfazqb.com/Article/details/gzrwrrbge.sHtML

[U10] Py：按值排序字典
来源：http://blog.tarul.cn/Article/details/gmfmfggxu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.epnwcf.com/Article/details/gyforbavn.sHtML

[U11] Py：生成器表达式
来源：http://blog.epnwcf.com/Article/details/glbqffrsb.sHtML

(x * 2 for x in arr)
来源：http://www.share.tarul.cn/Article/details/ghzpumecb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fktsv.cn/Article/details/gymcthomp.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fktsv.cn/Article/details/gnplqviwq.sHtML

[U13] Py：固定长度队列
来源：http://baike.fktsv.cn/Article/details/gkrobfonl.sHtML

deque(maxlen=10)
来源：http://www.m.share.tarul.cn/Article/details/ghuwscgbw.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.vehdjk.com/Article/details/gaztjljoi.sHtML

defaultdict(list)
来源：http://read.share.bbcook.cn/Article/details/gntqtvfyq.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.yfazqb.com/Article/details/gcpnpbzkm.sHtML

t = time.perf_counter()
来源：http://read.share.sjlbkw.cn/Article/details/gjdaxaiwb.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.bbcook.cn/Article/details/gngdclejj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fktsv.cn/Article/details/gotyrteli.sHtML

[U17] Py：初始化日志
来源：http://3g.yfazqb.com/Article/details/gbsybrdfe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.epnwcf.com/Article/details/geczutmgd.sHtML

[U18] Py：预编译正则
来源：http://m.share.sjlbkw.cn/Article/details/gqafhtssw.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fktsv.cn/Article/details/gddgsejgp.sHtML

[U19] Py：正则替换带回调
来源：http://wap.sjlbkw.cn/Article/details/gbnmuzetb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fktsv.cn/Article/details/gsaydvjtq.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fktsv.cn/Article/details/gqxiqpukb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.vehdjk.com/Article/details/gvfbztxvr.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.epnwcf.com/Article/details/gppgtvwtu.sHtML

@contextlib.contextmanager
来源：http://3g.vehdjk.com/Article/details/gnqgvzcxt.sHtML

[U22] Py：矩阵转置
来源：http://read.share.tarul.cn/Article/details/gwssjvilk.sHtML

list(zip(*m))
来源：http://www.share.sjlbkw.cn/Article/details/gbcsxtfjo.sHtML

[U23] Py：分块读取大文件
来源：http://blog.epnwcf.com/Article/details/gmjhthvpq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.bbcook.cn/Article/details/ghoglfwdp.sHtML

[U24] Py：路径操作
来源：http://baike.yfazqb.com/Article/details/gsqhcymjl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fktsv.cn/Article/details/ghbbsyhpj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.bbcook.cn/Article/details/gvdsqugbe.sHtML

csv.DictReader(f)
来源：http://mobile.fktsv.cn/Article/details/gphyywbvy.sHtML

[U26] Py：并发下载
来源：http://m.share.yfazqb.com/Article/details/ghtxwxhfc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.tarul.cn/Article/details/gqnmjemun.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.sjlbkw.cn/Article/details/gnkbsokbj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.vehdjk.com/Article/details/gbfqfjiin.sHtML

[U28] Py：类型别名
来源：http://www.m.share.yfazqb.com/Article/details/glhajdkoh.sHtML

UserId = int
来源：http://mobile.vehdjk.com/Article/details/gqgbgpkue.sHtML

[U29] Py：属性校验
来源：http://baike.vehdjk.com/Article/details/glfmudolt.sHtML

@property 与 @x.setter 配合
来源：http://read.share.epnwcf.com/Article/details/gcdosuqtl.sHtML

[U30] Py：数据类
来源：http://m.share.vehdjk.com/Article/details/gcxemyikp.sHtML

@dataclass(slots=True)
来源：http://3g.yfazqb.com/Article/details/gmidskqyq.sHtML

[U31] Py：单测
来源：http://blog.bbcook.cn/Article/details/gkhuprlwk.sHtML

python -m pytest -q
来源：http://mobile.bbcook.cn/Article/details/gkpahdpvo.sHtML

[U32] Py：代码格式化
来源：http://www.share.fktsv.cn/Article/details/gbvhytkvs.sHtML

ruff format . && ruff check --fix .
来源：http://3g.epnwcf.com/Article/details/gngihrrfj.sHtML

[U33] Py：打包发布
来源：http://wap.fktsv.cn/Article/details/gkubxicjv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.sjlbkw.cn/Article/details/gjigoetwo.sHtML

[U34] Py：判断编码
来源：http://www.m.share.vehdjk.com/Article/details/gzvaedyei.sHtML

chardet.detect(raw)
来源：http://www.share.sjlbkw.cn/Article/details/gznaimmes.sHtML

[U35] Py：发送邮件
来源：http://read.share.fktsv.cn/Article/details/gfxzxsyho.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.sjlbkw.cn/Article/details/gfajpswob.sHtML

[U36] Py：定时任务
来源：http://3g.epnwcf.com/Article/details/gqsdctucf.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.epnwcf.com/Article/details/gdtsmetyo.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.yfazqb.com/Article/details/gsywgsryw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.vehdjk.com/Article/details/glzrlfwnw.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.vehdjk.com/Article/details/gwxcrmgjs.sHtML

Path(__file__).resolve().parent
来源：http://m.share.tarul.cn/Article/details/gknqkvbah.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.epnwcf.com/Article/details/gjpybqmpo.sHtML

sys.stdout.isatty()
来源：http://www.blog.yfazqb.com/Article/details/gbihtqnle.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.yfazqb.com/Article/details/gpuhylsgn.sHtML

print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/gscmhkvxf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.epnwcf.com/Article/details/gvczizhyv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fktsv.cn/Article/details/gtckzyjpk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.bbcook.cn/Article/details/gnuwffgzl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.vehdjk.com/Article/details/gijugypaf.sHtML

[U43] PHP：声明命名空间
来源：http://baike.bbcook.cn/Article/details/gaymzpmxw.sHtML

namespace App\Http;
来源：http://m.share.vehdjk.com/Article/details/gdnjiokqi.sHtML

[U44] PHP：开启严格类型
来源：http://blog.sjlbkw.cn/Article/details/gzoxaulbi.sHtML

declare(strict_types=1);
来源：http://m.share.tarul.cn/Article/details/guieqdyfm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.epnwcf.com/Article/details/glqgrseah.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gangflovh.sHtML

[U46] PHP：可空类型
来源：http://www.share.tarul.cn/Article/details/gdrrjiqma.sHtML

?string $name = null
来源：http://3g.yfazqb.com/Article/details/gbzevudkq.sHtML

[U47] PHP：联合类型
来源：http://mobile.bbcook.cn/Article/details/grnehvkxb.sHtML

int|string $id
来源：http://mobile.bbcook.cn/Article/details/gwetguwyi.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gwgogwwdl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.vehdjk.com/Article/details/ghwsxizoe.sHtML

[U49] PHP：只读属性
来源：http://blog.epnwcf.com/Article/details/goqnqqvnv.sHtML

public readonly string $name
来源：http://blog.tarul.cn/Article/details/gfyqvjojb.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.vehdjk.com/Article/details/gvlmthodt.sHtML

public function __construct(private int $id) {}
来源：http://3g.tarul.cn/Article/details/gbzgnrlly.sHtML

[U51] PHP：数组解构
来源：http://m.share.sjlbkw.cn/Article/details/gbxecmjza.sHtML

[$a, $b] = $arr;
来源：http://wap.yfazqb.com/Article/details/gvethzgpl.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fktsv.cn/Article/details/gnkekkrra.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.vehdjk.com/Article/details/gwvymysns.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.vehdjk.com/Article/details/ggfkeqllz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.vehdjk.com/Article/details/gfscuyzif.sHtML

[U54] PHP：空安全调用
来源：http://3g.tarul.cn/Article/details/gltmfmvqv.sHtML

$obj?->method()
来源：http://wap.vehdjk.com/Article/details/gixxmeuxr.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fktsv.cn/Article/details/gvhquexbn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.yfazqb.com/Article/details/gvmtbgmzc.sHtML

[U56] PHP：命名参数
来源：http://read.share.tarul.cn/Article/details/gkllnvcoa.sHtML

f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gzdkavvmi.sHtML

[U57] PHP：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gdbkwfrfh.sHtML

"值: {$a}"
来源：http://blog.tarul.cn/Article/details/gkfznqvqo.sHtML

[U58] PHP：数组三件套
来源：http://m.share.yfazqb.com/Article/details/gxtueucjr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gbydmphub.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.tarul.cn/Article/details/gtdjdwboj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fktsv.cn/Article/details/ghqgvrhfj.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.bbcook.cn/Article/details/gcckshbta.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.vehdjk.com/Article/details/gwkhwbbon.sHtML

[U61] PHP：正则
来源：http://3g.sjlbkw.cn/Article/details/ggmrjurun.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.bbcook.cn/Article/details/gxhpctnjg.sHtML

[U62] PHP：日期对象
来源：http://3g.tarul.cn/Article/details/gashbktkj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.yfazqb.com/Article/details/gndwkwgcr.sHtML

[U63] PHP：文件读写
来源：http://baike.vehdjk.com/Article/details/ghljlkyco.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.sjlbkw.cn/Article/details/gztolzniq.sHtML

[U64] PHP：目录遍历
来源：http://baike.sjlbkw.cn/Article/details/gkeabxlkk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.tarul.cn/Article/details/gynxrvnas.sHtML

[U65] PHP：会话
来源：http://wap.fktsv.cn/Article/details/gaxludsge.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.vehdjk.com/Article/details/gevdcuduu.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.yfazqb.com/Article/details/gnjasfmht.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.tarul.cn/Article/details/gcqqztcys.sHtML

[U67] PHP：处理文件上传
来源：http://baike.tarul.cn/Article/details/gjanrtqgv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.tarul.cn/Article/details/gawwqwmth.sHtML

[U68] PHP：PDO 连接
来源：http://3g.epnwcf.com/Article/details/gcdrhvdgy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.bbcook.cn/Article/details/gpzdgjssr.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fktsv.cn/Article/details/gzyfdxhcb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.yfazqb.com/Article/details/gfymfydmw.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.bbcook.cn/Article/details/gyoibwsav.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.sjlbkw.cn/Article/details/gsobkyjza.sHtML


<!-- 参考信息 -->