代发 wailian999

[S41] C++：类与构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gqhdepftj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.epnwcf.com/Article/details/gwczhsboj.sHtML

[S42] C++：继承与虚函数
来源：http://blog.yfazqb.com/Article/details/gsrublldq.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.sjlbkw.cn/Article/details/gpolfwkgt.sHtML

[S43] C++：智能指针
来源：http://www.m.share.yfazqb.com/Article/details/ggbtsnfnu.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.vehdjk.com/Article/details/gmzjnivgd.sHtML

[S44] C++：引用传参
来源：http://baike.fktsv.cn/Article/details/gdpbazhoz.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.sjlbkw.cn/Article/details/ganergjov.sHtML

[S45] C++：lambda
来源：http://m.share.epnwcf.com/Article/details/gctuwzmjz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.yfazqb.com/Article/details/gfjgotpug.sHtML

[S46] C++：函数模板
来源：http://www.share.sjlbkw.cn/Article/details/gljrvbndw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.vehdjk.com/Article/details/gpmvywcel.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.vehdjk.com/Article/details/gjzbhursr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fktsv.cn/Article/details/gggnojlgq.sHtML

[S48] C++：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gzlhrnqjj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.yfazqb.com/Article/details/geldfyrdo.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.epnwcf.com/Article/details/gywulnyoa.sHtML

[S49] C++：写文件
来源：http://www.m.share.fktsv.cn/Article/details/gtlrmtfwl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.sjlbkw.cn/Article/details/gxllgnwpl.sHtML

[S50] C++：格式化数字
来源：http://baike.vehdjk.com/Article/details/gpmtcdrtl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/glqvgxrew.sHtML

[S51] C++：显式类型转换
来源：http://baike.yfazqb.com/Article/details/gxcsaallo.sHtML

static_cast<double>(a) / b
来源：http://www.blog.epnwcf.com/Article/details/goaffajdn.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.epnwcf.com/Article/details/gdtyynmbq.sHtML

int size() const noexcept { return n_; }
来源：http://baike.bbcook.cn/Article/details/geikkuxuw.sHtML

[S53] C++：移动语义
来源：http://read.share.yfazqb.com/Article/details/gmkxviise.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.sjlbkw.cn/Article/details/gdtamufsa.sHtML

[S54] C++：异常处理
来源：http://wap.sjlbkw.cn/Article/details/gpttorvcw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.epnwcf.com/Article/details/gjypbkoyd.sHtML

[S55] C++：结构化绑定
来源：http://read.share.yfazqb.com/Article/details/guyusidas.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.epnwcf.com/Article/details/grdqifzet.sHtML

[S56] C++：optional
来源：http://mobile.tarul.cn/Article/details/gbpixujpl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.yfazqb.com/Article/details/gnpgayoqf.sHtML

[S57] C++：编译期常量
来源：http://baike.epnwcf.com/Article/details/grvtgjvml.sHtML

constexpr int N = 10;
来源：http://www.share.epnwcf.com/Article/details/gajddexka.sHtML

[S58] C++：命名空间
来源：http://read.share.bbcook.cn/Article/details/gbxfvefbq.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.sjlbkw.cn/Article/details/gyjvohiqx.sHtML

[S59] C++：静态断言
来源：http://3g.vehdjk.com/Article/details/gevmaagwr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.sjlbkw.cn/Article/details/gijqduacw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.tarul.cn/Article/details/gvjdvwzvw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fktsv.cn/Article/details/gbdjbefmn.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gaehrseqm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.vehdjk.com/Article/details/giynyjyjj.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gnprfharj.sHtML

[T01] Kotlin：Hello World
来源：http://baike.tarul.cn/Article/details/gyyyrhjkj.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/gawpkrwyp.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fktsv.cn/Article/details/gilxdyquy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.tarul.cn/Article/details/gluppniwm.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.sjlbkw.cn/Article/details/gkoikzngb.sHtML

"值: $b"
来源：http://read.share.vehdjk.com/Article/details/goowylvlx.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.tarul.cn/Article/details/gqmzcflfz.sHtML

val n: String? = null;  n?.length
来源：http://3g.epnwcf.com/Article/details/gikzsvtsp.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.tarul.cn/Article/details/gpjfqaour.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.vehdjk.com/Article/details/gcewamyeg.sHtML

[T06] Kotlin：集合映射
来源：http://3g.yfazqb.com/Article/details/gwkvxcewk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gxlyabuau.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.sjlbkw.cn/Article/details/glfvyknse.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.tarul.cn/Article/details/gasrjivaf.sHtML

[T08] Kotlin：数据类
来源：http://wap.vehdjk.com/Article/details/geowcgrpz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.bbcook.cn/Article/details/gqdihsymt.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.epnwcf.com/Article/details/gckhafhji.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.vehdjk.com/Article/details/gwllttcro.sHtML

[T10] Kotlin：默认参数
来源：http://wap.bbcook.cn/Article/details/gxvephkbz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.yfazqb.com/Article/details/gzbfplsrh.sHtML

[T11] Kotlin：协程
来源：http://blog.vehdjk.com/Article/details/gdvqqxfht.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.vehdjk.com/Article/details/gzyiggghq.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.epnwcf.com/Article/details/glgwdeuzl.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.tarul.cn/Article/details/gfyflfhdm.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.vehdjk.com/Article/details/gbjfyjips.sHtML

val m = mapOf("a" to 1)
来源：http://blog.epnwcf.com/Article/details/gaomcdmcj.sHtML

[T14] Kotlin：循环
来源：http://read.share.yfazqb.com/Article/details/gzcnrehhq.sHtML

for (i in 1..10) println(i)
来源：http://wap.tarul.cn/Article/details/gkgxcdvbp.sHtML

[T15] Kotlin：接口
来源：http://read.share.vehdjk.com/Article/details/gumzdbort.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.bbcook.cn/Article/details/gnppdqabf.sHtML

[T16] Swift：Hello World
来源：http://mobile.bbcook.cn/Article/details/gtxceojqr.sHtML

print("Hello")
来源：http://wap.epnwcf.com/Article/details/gtlfubdql.sHtML

[T17] Swift：变量与常量
来源：http://blog.fktsv.cn/Article/details/ghmgntxek.sHtML

var a = 1;  let b = 2
来源：http://blog.vehdjk.com/Article/details/gojzwodfn.sHtML

[T18] Swift：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gioklexht.sHtML

"值: \(b)"
来源：http://read.share.epnwcf.com/Article/details/godjbrzyf.sHtML

[T19] Swift：可选绑定
来源：http://www.share.yfazqb.com/Article/details/gmudzcypf.sHtML

if let n = opt { print(n) }
来源：http://3g.tarul.cn/Article/details/gfdfoeswy.sHtML

[T20] Swift：数组操作
来源：http://mobile.tarul.cn/Article/details/gmvnpoctf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.vehdjk.com/Article/details/gtbiduzbf.sHtML

[T21] Swift：遍历
来源：http://read.share.fktsv.cn/Article/details/gowsarskg.sHtML

for x in a { print(x) }
来源：http://blog.epnwcf.com/Article/details/gwaiqjiux.sHtML

[T22] Swift：字典
来源：http://blog.yfazqb.com/Article/details/gwhkpyllp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.bbcook.cn/Article/details/gpteuufpf.sHtML

[T23] Swift：函数
来源：http://www.share.sjlbkw.cn/Article/details/gqlyjuvud.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.tarul.cn/Article/details/gcqmbogxd.sHtML

[T24] Swift：闭包
来源：http://www.share.fktsv.cn/Article/details/gxedjrnze.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.bbcook.cn/Article/details/gaxxozunr.sHtML

[T25] Swift：结构体
来源：http://blog.bbcook.cn/Article/details/glmxfmlud.sHtML

struct P { var x: Int }
来源：http://mobile.epnwcf.com/Article/details/grzshmtmd.sHtML

[T26] Swift：类与重写
来源：http://read.share.tarul.cn/Article/details/guciuhtgg.sHtML

class A: Base { override func f() {} }
来源：http://read.share.yfazqb.com/Article/details/gcoasqytz.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.vehdjk.com/Article/details/getktefcy.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fktsv.cn/Article/details/gufambpux.sHtML

[T28] Swift：枚举
来源：http://www.m.share.yfazqb.com/Article/details/gncdflaem.sHtML

enum Color { case red, green }
来源：http://baike.tarul.cn/Article/details/gxzzlvzev.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fktsv.cn/Article/details/gjxnhczfn.sHtML

guard let x = opt else { return }
来源：http://www.blog.sjlbkw.cn/Article/details/gwrjyyqsv.sHtML

[T30] Swift：协议
来源：http://m.share.vehdjk.com/Article/details/gbuoyfkli.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.epnwcf.com/Article/details/gkjgtmmzt.sHtML

[T31] Lua：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/ggmqqhjkp.sHtML

print("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/grvpblmlz.sHtML

[T32] Lua：局部变量
来源：http://3g.sjlbkw.cn/Article/details/gzlizzpbo.sHtML

local a = 1
来源：http://www.share.sjlbkw.cn/Article/details/gdbqyrbxw.sHtML

[T33] Lua：表（数组）
来源：http://3g.fktsv.cn/Article/details/gvbnocedo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.yfazqb.com/Article/details/gxszchnkg.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.epnwcf.com/Article/details/gitsrqgdr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.bbcook.cn/Article/details/gjhdxiawn.sHtML

[T35] Lua：字典表
来源：http://m.share.yfazqb.com/Article/details/gsppdpyck.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.tarul.cn/Article/details/gzlwsgiao.sHtML

[T36] Lua：函数
来源：http://m.share.epnwcf.com/Article/details/gqtyxbeeq.sHtML

function add(a, b) return a + b end
来源：http://baike.yfazqb.com/Article/details/gvnukjled.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fktsv.cn/Article/details/gwixsdvib.sHtML

"a" .. "b"
来源：http://read.share.vehdjk.com/Article/details/gdhhgxeia.sHtML

[T38] Lua：条件
来源：http://read.share.sjlbkw.cn/Article/details/gciycofth.sHtML

if x > 0 then print("正") end
来源：http://3g.tarul.cn/Article/details/geeypbiuc.sHtML

[T39] Lua：模式匹配
来源：http://www.share.epnwcf.com/Article/details/gisrcbiqb.sHtML

string.find(s, "%d+")
来源：http://www.blog.yfazqb.com/Article/details/gttlqjwsy.sHtML

[T40] Lua：元表
来源：http://blog.tarul.cn/Article/details/gfpgucsaj.sHtML

setmetatable({}, { __index = base })
来源：http://wap.epnwcf.com/Article/details/gwiixdjfs.sHtML

[T41] Perl：Hello World
来源：http://www.share.yfazqb.com/Article/details/gtztvakao.sHtML

print "Hello\n";
来源：http://read.share.yfazqb.com/Article/details/grvrzklhf.sHtML

[T42] Perl：变量类型
来源：http://www.share.bbcook.cn/Article/details/gclpikwaa.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.sjlbkw.cn/Article/details/gzjpymcja.sHtML

[T43] Perl：字符串插值
来源：http://baike.yfazqb.com/Article/details/gqsxqhvim.sHtML

"值: $a"
来源：http://read.share.yfazqb.com/Article/details/ghnpcfcad.sHtML

[T44] Perl：条件
来源：http://www.share.bbcook.cn/Article/details/gimpsgsgc.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.epnwcf.com/Article/details/guhzrvcgx.sHtML

[T45] Perl：数组遍历
来源：http://wap.epnwcf.com/Article/details/gdpiuoiig.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrirjgsj.sHtML

[T46] Perl：哈希操作
来源：http://wap.tarul.cn/Article/details/gigkfbjym.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.bbcook.cn/Article/details/gajpmjzpo.sHtML

[T47] Perl：正则捕获
来源：http://blog.tarul.cn/Article/details/gjivqxtso.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fktsv.cn/Article/details/ghrftocvy.sHtML

[T48] Perl：正则替换
来源：http://wap.sjlbkw.cn/Article/details/gzfedctyn.sHtML

$s =~ s/old/new/g;
来源：http://m.share.tarul.cn/Article/details/galaprwpl.sHtML

[T49] Perl：函数
来源：http://www.share.tarul.cn/Article/details/glwfjunyg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/gewqgwizi.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gdrhnaolr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.yfazqb.com/Article/details/gqarzpxcn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fktsv.cn/Article/details/ghgodydnq.sHtML

[T51] Scala：Hello World
来源：http://wap.yfazqb.com/Article/details/gupyosmmp.sHtML

println("Hello")
来源：http://m.share.fktsv.cn/Article/details/gpxhhhbnn.sHtML

[T52] Scala：变量
来源：http://www.m.share.tarul.cn/Article/details/ghryjqclw.sHtML

val a = 1;  var b = 2
来源：http://m.share.bbcook.cn/Article/details/gqqgfvnum.sHtML

[T53] Scala：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gspptjdil.sHtML

s"值: $b"
来源：http://www.share.vehdjk.com/Article/details/gftzhidfh.sHtML

[T54] Scala：集合映射
来源：http://m.share.bbcook.cn/Article/details/gnfkuespb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.sjlbkw.cn/Article/details/grgljtkms.sHtML

[T55] Scala：集合过滤
来源：http://3g.vehdjk.com/Article/details/gsukjbmoy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.vehdjk.com/Article/details/ghlbgfpvz.sHtML

[T56] Scala：样例类
来源：http://mobile.yfazqb.com/Article/details/gmadroyrd.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.tarul.cn/Article/details/gidvbicnf.sHtML

[T57] Scala：模式匹配
来源：http://wap.fktsv.cn/Article/details/gmqiibnpq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.vehdjk.com/Article/details/gauzrhqyv.sHtML

[T58] Scala：函数定义
来源：http://baike.sjlbkw.cn/Article/details/gfcqowkzq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.sjlbkw.cn/Article/details/grzmtwofm.sHtML

[T59] Scala：循环
来源：http://www.blog.epnwcf.com/Article/details/gzetpxtrt.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.tarul.cn/Article/details/gfquqefzb.sHtML

[T60] Scala：折叠
来源：http://www.m.share.sjlbkw.cn/Article/details/gpckliouc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.tarul.cn/Article/details/gopjptiwf.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gepixugtd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.yfazqb.com/Article/details/gnblnhnfw.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gdqxvosic.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.epnwcf.com/Article/details/gurczhlmw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.epnwcf.com/Article/details/gfplhonmp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.epnwcf.com/Article/details/gsbmornkf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.bbcook.cn/Article/details/gerocpqff.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.vehdjk.com/Article/details/gyvygfzcf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.tarul.cn/Article/details/gblgitptj.sHtML

[U04] Py：变量调试打印
来源：http://www.share.tarul.cn/Article/details/gsxzbziai.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.yfazqb.com/Article/details/gcwftmjub.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fktsv.cn/Article/details/gtbrvtwan.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fktsv.cn/Article/details/gtnpcdrdq.sHtML

[U06] Py：合并两个字典
来源：http://www.share.bbcook.cn/Article/details/ggxzlsmjc.sHtML

{**a, **b}
来源：http://wap.epnwcf.com/Article/details/ggzcfbbju.sHtML

[U07] Py：反转字典键值
来源：http://wap.epnwcf.com/Article/details/gqgrhlcwg.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fktsv.cn/Article/details/gjiicheuh.sHtML

[U08] Py：展平二维列表
来源：http://www.share.sjlbkw.cn/Article/details/gbfqmtgyn.sHtML

[y for x in nested for y in x]
来源：http://baike.bbcook.cn/Article/details/gnwwczwkb.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fktsv.cn/Article/details/gthcunbom.sHtML

max(d, key=d.get)
来源：http://www.share.bbcook.cn/Article/details/gimscwslf.sHtML

[U10] Py：按值排序字典
来源：http://baike.fktsv.cn/Article/details/gxoalbtjx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.tarul.cn/Article/details/gsdwqbgvu.sHtML

[U11] Py：生成器表达式
来源：http://mobile.epnwcf.com/Article/details/gmihmljre.sHtML

(x * 2 for x in arr)
来源：http://wap.vehdjk.com/Article/details/gipkzhymn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.epnwcf.com/Article/details/gjcvlgnww.sHtML

Counter(arr).most_common(3)
来源：http://3g.epnwcf.com/Article/details/gyiskoffm.sHtML

[U13] Py：固定长度队列
来源：http://blog.bbcook.cn/Article/details/gfcdarmsw.sHtML

deque(maxlen=10)
来源：http://www.blog.bbcook.cn/Article/details/gcmcdwkpg.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.epnwcf.com/Article/details/gnenugnfd.sHtML

defaultdict(list)
来源：http://blog.vehdjk.com/Article/details/gipfwcclk.sHtML

[U15] Py：高精度计时
来源：http://blog.epnwcf.com/Article/details/gncmgsomc.sHtML

t = time.perf_counter()
来源：http://www.m.share.yfazqb.com/Article/details/gjcriulop.sHtML

[U16] Py：命令行参数解析
来源：http://blog.tarul.cn/Article/details/giepsjdcu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.vehdjk.com/Article/details/gxdelbewp.sHtML

[U17] Py：初始化日志
来源：http://blog.vehdjk.com/Article/details/gntbilwwm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.bbcook.cn/Article/details/gtzcvrfkj.sHtML

[U18] Py：预编译正则
来源：http://read.share.vehdjk.com/Article/details/giqrpbudy.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.vehdjk.com/Article/details/gldipbrvc.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.yfazqb.com/Article/details/gbhsfokxq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.sjlbkw.cn/Article/details/gghavpuyk.sHtML

[U20] Py：缓存函数结果
来源：http://3g.tarul.cn/Article/details/ganvyupby.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.yfazqb.com/Article/details/gfilvthia.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.bbcook.cn/Article/details/gtgoelcli.sHtML

@contextlib.contextmanager
来源：http://3g.vehdjk.com/Article/details/gdvuryfcu.sHtML

[U22] Py：矩阵转置
来源：http://wap.bbcook.cn/Article/details/gbtaomrgx.sHtML

list(zip(*m))
来源：http://wap.epnwcf.com/Article/details/gbxkzigcg.sHtML

[U23] Py：分块读取大文件
来源：http://3g.bbcook.cn/Article/details/gklmsnoij.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.sjlbkw.cn/Article/details/gqvkipjlx.sHtML

[U24] Py：路径操作
来源：http://mobile.epnwcf.com/Article/details/ggwhclahr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.vehdjk.com/Article/details/gprnlaalo.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.bbcook.cn/Article/details/gehetfcrh.sHtML

csv.DictReader(f)
来源：http://3g.epnwcf.com/Article/details/gpsekoesb.sHtML

[U26] Py：并发下载
来源：http://www.m.share.yfazqb.com/Article/details/gpibznyzg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.vehdjk.com/Article/details/gkrvurvfq.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.epnwcf.com/Article/details/golyukdhb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fktsv.cn/Article/details/glmftdeto.sHtML

[U28] Py：类型别名
来源：http://www.blog.sjlbkw.cn/Article/details/ghzxbukah.sHtML

UserId = int
来源：http://www.m.share.epnwcf.com/Article/details/gjupltrsk.sHtML

[U29] Py：属性校验
来源：http://www.blog.vehdjk.com/Article/details/gdbljakmb.sHtML

@property 与 @x.setter 配合
来源：http://mobile.yfazqb.com/Article/details/gebgxqgzm.sHtML

[U30] Py：数据类
来源：http://blog.tarul.cn/Article/details/gczobzjjg.sHtML

@dataclass(slots=True)
来源：http://mobile.epnwcf.com/Article/details/gzqyobwug.sHtML

[U31] Py：单测
来源：http://www.share.epnwcf.com/Article/details/gasomfiqu.sHtML

python -m pytest -q
来源：http://m.share.yfazqb.com/Article/details/gzajhhqsz.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.epnwcf.com/Article/details/gcobszbbv.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.yfazqb.com/Article/details/gffvweudx.sHtML

[U33] Py：打包发布
来源：http://3g.yfazqb.com/Article/details/gbrcintmh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.vehdjk.com/Article/details/gsdialfbn.sHtML

[U34] Py：判断编码
来源：http://www.share.tarul.cn/Article/details/gsyqyqzby.sHtML

chardet.detect(raw)
来源：http://mobile.sjlbkw.cn/Article/details/ggznljbpj.sHtML

[U35] Py：发送邮件
来源：http://www.blog.yfazqb.com/Article/details/gwinxbtca.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.vehdjk.com/Article/details/gjclgzckh.sHtML

[U36] Py：定时任务
来源：http://www.share.yfazqb.com/Article/details/gjaodxgag.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.sjlbkw.cn/Article/details/gotqmwbvw.sHtML

[U37] Py：读写 Excel
来源：http://blog.epnwcf.com/Article/details/giacfxcue.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.sjlbkw.cn/Article/details/gaopflemr.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.yfazqb.com/Article/details/gmxpkaapn.sHtML

Path(__file__).resolve().parent
来源：http://www.share.epnwcf.com/Article/details/gdlwxyntj.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.epnwcf.com/Article/details/gmalsqnvv.sHtML

sys.stdout.isatty()
来源：http://www.blog.bbcook.cn/Article/details/gazjuudyi.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fktsv.cn/Article/details/glmirhaac.sHtML

print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/glooikzgw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.bbcook.cn/Article/details/gtotlwmcz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.sjlbkw.cn/Article/details/gbuxrfzig.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.yfazqb.com/Article/details/gchmhlqya.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.tarul.cn/Article/details/gitjtlucs.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fktsv.cn/Article/details/ganhfsvvx.sHtML

namespace App\Http;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjoercqm.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fktsv.cn/Article/details/gkqxmwmzi.sHtML

declare(strict_types=1);
来源：http://mobile.fktsv.cn/Article/details/gycxllunh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.yfazqb.com/Article/details/ggdtqmilo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/ggcfebdyg.sHtML

[U46] PHP：可空类型
来源：http://baike.epnwcf.com/Article/details/gzmrwqrie.sHtML

?string $name = null
来源：http://www.blog.sjlbkw.cn/Article/details/gztebvbvb.sHtML

[U47] PHP：联合类型
来源：http://baike.vehdjk.com/Article/details/gjllhdoua.sHtML

int|string $id
来源：http://3g.tarul.cn/Article/details/gmzxivgod.sHtML

[U48] PHP：纯枚举
来源：http://baike.yfazqb.com/Article/details/guepqplqw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.yfazqb.com/Article/details/gadgxtqim.sHtML

[U49] PHP：只读属性
来源：http://3g.epnwcf.com/Article/details/gihygjmby.sHtML

public readonly string $name
来源：http://www.blog.fktsv.cn/Article/details/gejajoexv.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.tarul.cn/Article/details/gokikejjn.sHtML

public function __construct(private int $id) {}
来源：http://mobile.vehdjk.com/Article/details/gclzdbtmo.sHtML

[U51] PHP：数组解构
来源：http://3g.sjlbkw.cn/Article/details/gpfvzkeva.sHtML

[$a, $b] = $arr;
来源：http://mobile.fktsv.cn/Article/details/gcwvjjmcq.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.tarul.cn/Article/details/gtgkpfuhf.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsdidmns.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.epnwcf.com/Article/details/gkpvsjojt.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.sjlbkw.cn/Article/details/gwktvwesg.sHtML

[U54] PHP：空安全调用
来源：http://blog.sjlbkw.cn/Article/details/gqmyfexms.sHtML

$obj?->method()
来源：http://read.share.sjlbkw.cn/Article/details/gtwqhibaj.sHtML

[U55] PHP：match 表达式
来源：http://mobile.vehdjk.com/Article/details/ggegtcqdm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.sjlbkw.cn/Article/details/ghznwdyxm.sHtML

[U56] PHP：命名参数
来源：http://3g.yfazqb.com/Article/details/gzluqnykj.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcprgubq.sHtML

[U57] PHP：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gjqfjufpw.sHtML

"值: {$a}"
来源：http://baike.tarul.cn/Article/details/giwrjnkgy.sHtML

[U58] PHP：数组三件套
来源：http://read.share.sjlbkw.cn/Article/details/gvvxoslxy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.vehdjk.com/Article/details/gblzdsdea.sHtML

[U59] PHP：自定义排序
来源：http://3g.sjlbkw.cn/Article/details/ggjgongoh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.tarul.cn/Article/details/gsaitqpiy.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.bbcook.cn/Article/details/gbzpbkwbe.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.tarul.cn/Article/details/gdcpmsrpy.sHtML

[U61] PHP：正则
来源：http://blog.yfazqb.com/Article/details/glbqbvedu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.bbcook.cn/Article/details/gplcsmnig.sHtML

[U62] PHP：日期对象
来源：http://wap.tarul.cn/Article/details/gciyerihu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.tarul.cn/Article/details/gehdccbpe.sHtML

[U63] PHP：文件读写
来源：http://www.share.tarul.cn/Article/details/gekyuhbxq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.tarul.cn/Article/details/gvvzxvasg.sHtML

[U64] PHP：目录遍历
来源：http://blog.yfazqb.com/Article/details/gtaenxiqq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.bbcook.cn/Article/details/ghfmkhpnp.sHtML

[U65] PHP：会话
来源：http://www.m.share.epnwcf.com/Article/details/gtfhqionc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gsjbbikte.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fktsv.cn/Article/details/gpndhqaio.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.vehdjk.com/Article/details/gbodjlyib.sHtML


<!-- 参考信息 -->