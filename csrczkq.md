代发 wailian999

[S41] C++：类与构造函数
来源：http://blog.bbcook.cn/Article/details/gufyfrcdf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.vehdjk.com/Article/details/gdzoyojsz.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fktsv.cn/Article/details/gojegvtvp.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.bbcook.cn/Article/details/gbtjlxyrl.sHtML

[S43] C++：智能指针
来源：http://m.share.epnwcf.com/Article/details/gcvrstevw.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.epnwcf.com/Article/details/gruuoydhp.sHtML

[S44] C++：引用传参
来源：http://baike.tarul.cn/Article/details/gmbrhawkp.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.yfazqb.com/Article/details/gzmpqzooz.sHtML

[S45] C++：lambda
来源：http://www.m.share.sjlbkw.cn/Article/details/gmylvmgza.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.bbcook.cn/Article/details/gmsycsmoy.sHtML

[S46] C++：函数模板
来源：http://read.share.tarul.cn/Article/details/grxvsacpn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fktsv.cn/Article/details/gnsllnywf.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.epnwcf.com/Article/details/gjrjhhypj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.sjlbkw.cn/Article/details/genarlyyr.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gmcdqdddu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.sjlbkw.cn/Article/details/gncyrkyfa.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.tarul.cn/Article/details/gahqtzocs.sHtML

[S49] C++：写文件
来源：http://read.share.yfazqb.com/Article/details/gcpkbjlcj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fktsv.cn/Article/details/glwylubjn.sHtML

[S50] C++：格式化数字
来源：http://wap.yfazqb.com/Article/details/gmaamxajg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.vehdjk.com/Article/details/gdxbdklml.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.yfazqb.com/Article/details/gyglkqjry.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.vehdjk.com/Article/details/gnuprgpqu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.vehdjk.com/Article/details/gqxjsictp.sHtML

int size() const noexcept { return n_; }
来源：http://blog.epnwcf.com/Article/details/gydyehbae.sHtML

[S53] C++：移动语义
来源：http://m.share.bbcook.cn/Article/details/ghilnhuxg.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.sjlbkw.cn/Article/details/gzvtxgwoe.sHtML

[S54] C++：异常处理
来源：http://blog.tarul.cn/Article/details/gjvqgoixn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.epnwcf.com/Article/details/godmbcuvo.sHtML

[S55] C++：结构化绑定
来源：http://mobile.sjlbkw.cn/Article/details/ghhssxkid.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.epnwcf.com/Article/details/gnlqdmbli.sHtML

[S56] C++：optional
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjseinok.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.bbcook.cn/Article/details/gciiyhktu.sHtML

[S57] C++：编译期常量
来源：http://read.share.epnwcf.com/Article/details/ghunuodqi.sHtML

constexpr int N = 10;
来源：http://www.blog.bbcook.cn/Article/details/gmdomyasx.sHtML

[S58] C++：命名空间
来源：http://mobile.yfazqb.com/Article/details/gptktibso.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.tarul.cn/Article/details/gkeclajds.sHtML

[S59] C++：静态断言
来源：http://www.blog.bbcook.cn/Article/details/gycjhidvo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.bbcook.cn/Article/details/grbllluti.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.sjlbkw.cn/Article/details/gspywylbp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.yfazqb.com/Article/details/gxpfzmnrm.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gxaiidmkk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.vehdjk.com/Article/details/gwjnotzxr.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gahocsmir.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.vehdjk.com/Article/details/gbtiyizsi.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/gullxqhju.sHtML

[T02] Kotlin：变量
来源：http://baike.bbcook.cn/Article/details/gphghlzte.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.bbcook.cn/Article/details/gzfkolhen.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.vehdjk.com/Article/details/gkkiflzwz.sHtML

"值: $b"
来源：http://m.share.bbcook.cn/Article/details/guagpbfkf.sHtML

[T04] Kotlin：空安全
来源：http://www.share.bbcook.cn/Article/details/gkoasvfgu.sHtML

val n: String? = null;  n?.length
来源：http://mobile.tarul.cn/Article/details/goctpwphw.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.yfazqb.com/Article/details/gawzzwbfv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.epnwcf.com/Article/details/gfajblgmb.sHtML

[T06] Kotlin：集合映射
来源：http://3g.yfazqb.com/Article/details/gciqpqraq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.bbcook.cn/Article/details/gmpddaaih.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.vehdjk.com/Article/details/gmcznjhrn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.tarul.cn/Article/details/gdbmnasuz.sHtML

[T08] Kotlin：数据类
来源：http://m.share.bbcook.cn/Article/details/grdhovfgg.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.sjlbkw.cn/Article/details/gswcimogx.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.vehdjk.com/Article/details/ggvziegbq.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.yfazqb.com/Article/details/gznyrwmje.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.vehdjk.com/Article/details/gvssudctf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.vehdjk.com/Article/details/gjalzxqhg.sHtML

[T11] Kotlin：协程
来源：http://read.share.vehdjk.com/Article/details/gxdyijcci.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fktsv.cn/Article/details/gygjquqex.sHtML

[T12] Kotlin：解构声明
来源：http://blog.yfazqb.com/Article/details/gbyvaxfno.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gjotpnbxo.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.vehdjk.com/Article/details/gwibpswmu.sHtML

val m = mapOf("a" to 1)
来源：http://wap.sjlbkw.cn/Article/details/gqynprsgi.sHtML

[T14] Kotlin：循环
来源：http://www.blog.epnwcf.com/Article/details/gdhgzrltz.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gveyemgyw.sHtML

[T15] Kotlin：接口
来源：http://baike.yfazqb.com/Article/details/goiaeszrk.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.vehdjk.com/Article/details/ggbvwrnsk.sHtML

[T16] Swift：Hello World
来源：http://www.share.vehdjk.com/Article/details/gqagfuuhm.sHtML

print("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gdhwvioru.sHtML

[T17] Swift：变量与常量
来源：http://baike.epnwcf.com/Article/details/grvbogucb.sHtML

var a = 1;  let b = 2
来源：http://www.blog.vehdjk.com/Article/details/gzbfvgash.sHtML

[T18] Swift：字符串插值
来源：http://3g.vehdjk.com/Article/details/gtkpjjpbq.sHtML

"值: \(b)"
来源：http://read.share.tarul.cn/Article/details/gpcclleyu.sHtML

[T19] Swift：可选绑定
来源：http://read.share.vehdjk.com/Article/details/gmeachloo.sHtML

if let n = opt { print(n) }
来源：http://3g.tarul.cn/Article/details/griuwfjqk.sHtML

[T20] Swift：数组操作
来源：http://www.share.yfazqb.com/Article/details/ghiideuny.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.bbcook.cn/Article/details/gmcqftwpr.sHtML

[T21] Swift：遍历
来源：http://www.blog.bbcook.cn/Article/details/goisevywj.sHtML

for x in a { print(x) }
来源：http://blog.bbcook.cn/Article/details/ggmsqkojt.sHtML

[T22] Swift：字典
来源：http://www.share.tarul.cn/Article/details/gwopaihyq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.sjlbkw.cn/Article/details/gwkweojsh.sHtML

[T23] Swift：函数
来源：http://read.share.vehdjk.com/Article/details/gvkwwafsc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fktsv.cn/Article/details/ghmzuwzyg.sHtML

[T24] Swift：闭包
来源：http://baike.epnwcf.com/Article/details/gdgsfqgmx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fktsv.cn/Article/details/gwtasoftz.sHtML

[T25] Swift：结构体
来源：http://mobile.vehdjk.com/Article/details/gzpbsvbho.sHtML

struct P { var x: Int }
来源：http://www.blog.tarul.cn/Article/details/gnpvasaeb.sHtML

[T26] Swift：类与重写
来源：http://www.share.yfazqb.com/Article/details/gvhwhbsol.sHtML

class A: Base { override func f() {} }
来源：http://3g.bbcook.cn/Article/details/gxbuyrznm.sHtML

[T27] Swift：错误处理
来源：http://mobile.yfazqb.com/Article/details/gzwjiiyzf.sHtML

do { try f() } catch { print(error) }
来源：http://blog.sjlbkw.cn/Article/details/gpnobhuqv.sHtML

[T28] Swift：枚举
来源：http://wap.epnwcf.com/Article/details/gyasasdmy.sHtML

enum Color { case red, green }
来源：http://www.share.vehdjk.com/Article/details/gxnlxfcpa.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.epnwcf.com/Article/details/ghlxemnai.sHtML

guard let x = opt else { return }
来源：http://www.share.yfazqb.com/Article/details/genwxhcya.sHtML

[T30] Swift：协议
来源：http://baike.epnwcf.com/Article/details/gigerhvuv.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fktsv.cn/Article/details/gzqzyidxu.sHtML

[T31] Lua：Hello World
来源：http://wap.epnwcf.com/Article/details/giozztpku.sHtML

print("Hello")
来源：http://3g.fktsv.cn/Article/details/guyhdnvsk.sHtML

[T32] Lua：局部变量
来源：http://wap.vehdjk.com/Article/details/gdtmvlgio.sHtML

local a = 1
来源：http://www.blog.vehdjk.com/Article/details/gozsbzdcg.sHtML

[T33] Lua：表（数组）
来源：http://blog.epnwcf.com/Article/details/geirbprcm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.epnwcf.com/Article/details/giowlbmbz.sHtML

[T34] Lua：遍历表
来源：http://blog.vehdjk.com/Article/details/ggxqfesbm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.sjlbkw.cn/Article/details/gbrclylyy.sHtML

[T35] Lua：字典表
来源：http://www.share.epnwcf.com/Article/details/gatloxezs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.epnwcf.com/Article/details/gwqsgxfhz.sHtML

[T36] Lua：函数
来源：http://www.m.share.tarul.cn/Article/details/grerrbwfb.sHtML

function add(a, b) return a + b end
来源：http://blog.sjlbkw.cn/Article/details/gdpumnfys.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.bbcook.cn/Article/details/gmzdpfswd.sHtML

"a" .. "b"
来源：http://3g.epnwcf.com/Article/details/gmqubvaec.sHtML

[T38] Lua：条件
来源：http://baike.vehdjk.com/Article/details/gaauqwauj.sHtML

if x > 0 then print("正") end
来源：http://wap.fktsv.cn/Article/details/gakzoarto.sHtML

[T39] Lua：模式匹配
来源：http://baike.bbcook.cn/Article/details/gvikfwmot.sHtML

string.find(s, "%d+")
来源：http://m.share.sjlbkw.cn/Article/details/grxmjwpwr.sHtML

[T40] Lua：元表
来源：http://mobile.tarul.cn/Article/details/gphakmpmt.sHtML

setmetatable({}, { __index = base })
来源：http://blog.yfazqb.com/Article/details/gluttmdio.sHtML

[T41] Perl：Hello World
来源：http://mobile.bbcook.cn/Article/details/gjuuctppb.sHtML

print "Hello\n";
来源：http://baike.bbcook.cn/Article/details/gnvzwnlac.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fktsv.cn/Article/details/gkqagzzig.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.epnwcf.com/Article/details/gsfwacuhu.sHtML

[T43] Perl：字符串插值
来源：http://baike.fktsv.cn/Article/details/gwfborapv.sHtML

"值: $a"
来源：http://3g.tarul.cn/Article/details/gzntybzlu.sHtML

[T44] Perl：条件
来源：http://www.share.tarul.cn/Article/details/ghzxkwpjj.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.vehdjk.com/Article/details/gmvpahyri.sHtML

[T45] Perl：数组遍历
来源：http://m.share.bbcook.cn/Article/details/giopbzjgk.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.epnwcf.com/Article/details/gyoylosyn.sHtML

[T46] Perl：哈希操作
来源：http://wap.sjlbkw.cn/Article/details/gikbspenx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.sjlbkw.cn/Article/details/gckxorxkx.sHtML

[T47] Perl：正则捕获
来源：http://www.share.vehdjk.com/Article/details/gtdilwnhm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.bbcook.cn/Article/details/gtfeweeao.sHtML

[T48] Perl：正则替换
来源：http://m.share.fktsv.cn/Article/details/gqqlmfwyp.sHtML

$s =~ s/old/new/g;
来源：http://baike.bbcook.cn/Article/details/gexjvwzqf.sHtML

[T49] Perl：函数
来源：http://3g.yfazqb.com/Article/details/gsizngpcw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/ggsvxdsjg.sHtML

[T50] Perl：逐行读文件
来源：http://blog.yfazqb.com/Article/details/gnerxblfy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.vehdjk.com/Article/details/glrlvagnu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.bbcook.cn/Article/details/gbkguypow.sHtML

[T51] Scala：Hello World
来源：http://wap.yfazqb.com/Article/details/gqtomfxek.sHtML

println("Hello")
来源：http://wap.tarul.cn/Article/details/gjowloocw.sHtML

[T52] Scala：变量
来源：http://read.share.fktsv.cn/Article/details/gftiavyqw.sHtML

val a = 1;  var b = 2
来源：http://www.share.epnwcf.com/Article/details/gkfdielhj.sHtML

[T53] Scala：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/glzyvylzn.sHtML

s"值: $b"
来源：http://blog.fktsv.cn/Article/details/gfmrwlqgm.sHtML

[T54] Scala：集合映射
来源：http://wap.bbcook.cn/Article/details/gebufecyh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.yfazqb.com/Article/details/glcgikshn.sHtML

[T55] Scala：集合过滤
来源：http://read.share.sjlbkw.cn/Article/details/ghcmylzqc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.sjlbkw.cn/Article/details/ghhombccd.sHtML

[T56] Scala：样例类
来源：http://www.blog.fktsv.cn/Article/details/gwiqtingj.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.sjlbkw.cn/Article/details/gkguotgpm.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/glpezutoc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.bbcook.cn/Article/details/gevtgruuq.sHtML

[T58] Scala：函数定义
来源：http://blog.yfazqb.com/Article/details/gyqkoikec.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.sjlbkw.cn/Article/details/gkjesadys.sHtML

[T59] Scala：循环
来源：http://m.share.sjlbkw.cn/Article/details/gobooszft.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/gbnjpcccf.sHtML

[T60] Scala：折叠
来源：http://mobile.vehdjk.com/Article/details/gstqvnter.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.bbcook.cn/Article/details/gdnkrimvp.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gjnerumze.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.yfazqb.com/Article/details/gbdydtjki.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/golweuwvt.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.bbcook.cn/Article/details/gfmmdbvic.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fktsv.cn/Article/details/gmwlyralo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.vehdjk.com/Article/details/gtllpzqfy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.tarul.cn/Article/details/gvyhxsiqb.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.yfazqb.com/Article/details/grfuhzyex.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.vehdjk.com/Article/details/gwdcminwg.sHtML

[U04] Py：变量调试打印
来源：http://m.share.yfazqb.com/Article/details/gndefgaoz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.sjlbkw.cn/Article/details/gmphvjxeq.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.tarul.cn/Article/details/gjdpfydtn.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fktsv.cn/Article/details/glybqwoyl.sHtML

[U06] Py：合并两个字典
来源：http://baike.vehdjk.com/Article/details/gobpyluxk.sHtML

{**a, **b}
来源：http://www.blog.fktsv.cn/Article/details/gcmycityb.sHtML

[U07] Py：反转字典键值
来源：http://mobile.yfazqb.com/Article/details/gxouhwtaw.sHtML

{v: k for k, v in d.items()}
来源：http://blog.yfazqb.com/Article/details/gbuvnqejx.sHtML

[U08] Py：展平二维列表
来源：http://baike.vehdjk.com/Article/details/gaqqbhynt.sHtML

[y for x in nested for y in x]
来源：http://wap.tarul.cn/Article/details/gwatvgnag.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.vehdjk.com/Article/details/gtcbqcrks.sHtML

max(d, key=d.get)
来源：http://blog.sjlbkw.cn/Article/details/gjltvhqck.sHtML

[U10] Py：按值排序字典
来源：http://www.share.bbcook.cn/Article/details/gvclvrxfx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.sjlbkw.cn/Article/details/gqswaxllx.sHtML

[U11] Py：生成器表达式
来源：http://m.share.sjlbkw.cn/Article/details/gtqdubvpn.sHtML

(x * 2 for x in arr)
来源：http://wap.bbcook.cn/Article/details/gjzigmlqq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.tarul.cn/Article/details/gofxhyejz.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.epnwcf.com/Article/details/gdodomskj.sHtML

[U13] Py：固定长度队列
来源：http://blog.fktsv.cn/Article/details/ghinnprxy.sHtML

deque(maxlen=10)
来源：http://3g.epnwcf.com/Article/details/gbplogxzj.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.tarul.cn/Article/details/gcvixwlvi.sHtML

defaultdict(list)
来源：http://www.share.fktsv.cn/Article/details/gznohzlwe.sHtML

[U15] Py：高精度计时
来源：http://www.share.epnwcf.com/Article/details/gtxgstftj.sHtML

t = time.perf_counter()
来源：http://www.blog.tarul.cn/Article/details/gbgwxwqhv.sHtML

[U16] Py：命令行参数解析
来源：http://3g.tarul.cn/Article/details/gcwfwbeto.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fktsv.cn/Article/details/gwtspaitb.sHtML

[U17] Py：初始化日志
来源：http://wap.yfazqb.com/Article/details/glgqiwplp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.yfazqb.com/Article/details/guiwkdtpq.sHtML

[U18] Py：预编译正则
来源：http://wap.epnwcf.com/Article/details/gdbcdquqs.sHtML

pat = re.compile(r"\d+")
来源：http://baike.sjlbkw.cn/Article/details/gttlubbuh.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.yfazqb.com/Article/details/gwdgtmppf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.yfazqb.com/Article/details/gfavnnust.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fktsv.cn/Article/details/gvqqvwvbh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.yfazqb.com/Article/details/gswelsqzw.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.vehdjk.com/Article/details/gnnkcmnei.sHtML

@contextlib.contextmanager
来源：http://m.share.epnwcf.com/Article/details/gkfepzsnp.sHtML

[U22] Py：矩阵转置
来源：http://wap.epnwcf.com/Article/details/gmpmmlsry.sHtML

list(zip(*m))
来源：http://mobile.sjlbkw.cn/Article/details/gfinkztum.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.epnwcf.com/Article/details/gnaoobgjf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.bbcook.cn/Article/details/ghfgmjwwb.sHtML

[U24] Py：路径操作
来源：http://wap.fktsv.cn/Article/details/gdmkghuki.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.bbcook.cn/Article/details/gviyxxoxe.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.sjlbkw.cn/Article/details/gxxeeyfjm.sHtML

csv.DictReader(f)
来源：http://mobile.vehdjk.com/Article/details/gldzbfppw.sHtML

[U26] Py：并发下载
来源：http://3g.sjlbkw.cn/Article/details/gvyhaaimf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.yfazqb.com/Article/details/gogpshlrs.sHtML

[U27] Py：异步 HTTP
来源：http://wap.sjlbkw.cn/Article/details/gvaqqvgsf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.bbcook.cn/Article/details/gwbpjwtot.sHtML

[U28] Py：类型别名
来源：http://read.share.vehdjk.com/Article/details/gwnwxxjlw.sHtML

UserId = int
来源：http://mobile.bbcook.cn/Article/details/gacxuvayt.sHtML

[U29] Py：属性校验
来源：http://www.share.epnwcf.com/Article/details/gpglnleit.sHtML

@property 与 @x.setter 配合
来源：http://blog.tarul.cn/Article/details/garpbbzoz.sHtML

[U30] Py：数据类
来源：http://read.share.fktsv.cn/Article/details/ggytchzgk.sHtML

@dataclass(slots=True)
来源：http://blog.fktsv.cn/Article/details/grtfdmoif.sHtML

[U31] Py：单测
来源：http://wap.vehdjk.com/Article/details/ggelwzgte.sHtML

python -m pytest -q
来源：http://mobile.vehdjk.com/Article/details/gbmfyzhhp.sHtML

[U32] Py：代码格式化
来源：http://www.share.yfazqb.com/Article/details/gsexawidl.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.bbcook.cn/Article/details/gzvqwfods.sHtML

[U33] Py：打包发布
来源：http://read.share.epnwcf.com/Article/details/geamstyjj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.sjlbkw.cn/Article/details/gkffsmzzr.sHtML

[U34] Py：判断编码
来源：http://www.m.share.sjlbkw.cn/Article/details/gelqzyjin.sHtML

chardet.detect(raw)
来源：http://www.blog.tarul.cn/Article/details/gbljrqaup.sHtML

[U35] Py：发送邮件
来源：http://www.blog.bbcook.cn/Article/details/gyhbfamqn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.sjlbkw.cn/Article/details/goysygxey.sHtML

[U36] Py：定时任务
来源：http://www.share.epnwcf.com/Article/details/ghyijzdlz.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.tarul.cn/Article/details/gjkipdldv.sHtML

[U37] Py：读写 Excel
来源：http://read.share.vehdjk.com/Article/details/gypbqofzj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fktsv.cn/Article/details/gdcsrsluk.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.epnwcf.com/Article/details/gjoqmhcod.sHtML

Path(__file__).resolve().parent
来源：http://3g.fktsv.cn/Article/details/gumisszlu.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.epnwcf.com/Article/details/gogtpkovl.sHtML

sys.stdout.isatty()
来源：http://read.share.epnwcf.com/Article/details/gudcryxut.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.bbcook.cn/Article/details/gjvfrfvub.sHtML

print("err", file=sys.stderr)
来源：http://www.share.tarul.cn/Article/details/gxalhdkhp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.vehdjk.com/Article/details/gfhqtgkfj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.tarul.cn/Article/details/gvlctbgqg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fktsv.cn/Article/details/gsugzesug.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.vehdjk.com/Article/details/gqgculgpd.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.yfazqb.com/Article/details/gwtgtcjix.sHtML

namespace App\Http;
来源：http://m.share.yfazqb.com/Article/details/gdoovnojy.sHtML

[U44] PHP：开启严格类型
来源：http://blog.yfazqb.com/Article/details/gilghyysv.sHtML

declare(strict_types=1);
来源：http://www.blog.vehdjk.com/Article/details/gwwxacpsa.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.epnwcf.com/Article/details/gjctmzdcj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gluiovjkx.sHtML

[U46] PHP：可空类型
来源：http://www.blog.yfazqb.com/Article/details/gaaewsoar.sHtML

?string $name = null
来源：http://www.m.share.epnwcf.com/Article/details/gbjlyyjip.sHtML

[U47] PHP：联合类型
来源：http://read.share.yfazqb.com/Article/details/gphrauamz.sHtML

int|string $id
来源：http://baike.epnwcf.com/Article/details/gwxkpnldb.sHtML

[U48] PHP：纯枚举
来源：http://wap.sjlbkw.cn/Article/details/goihbaovw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fktsv.cn/Article/details/gkfgeqhro.sHtML

[U49] PHP：只读属性
来源：http://3g.bbcook.cn/Article/details/ggocknagn.sHtML

public readonly string $name
来源：http://wap.vehdjk.com/Article/details/ggapuccuo.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.tarul.cn/Article/details/gznpvjhvp.sHtML

public function __construct(private int $id) {}
来源：http://3g.epnwcf.com/Article/details/gbjqioaac.sHtML

[U51] PHP：数组解构
来源：http://read.share.yfazqb.com/Article/details/gsbchqvqj.sHtML

[$a, $b] = $arr;
来源：http://m.share.yfazqb.com/Article/details/gkahqveis.sHtML

[U52] PHP：箭头函数
来源：http://www.share.sjlbkw.cn/Article/details/gkydcislt.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.bbcook.cn/Article/details/gitqpotxm.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.bbcook.cn/Article/details/gdxymciru.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fktsv.cn/Article/details/gyescsjjc.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.bbcook.cn/Article/details/gpfjtttkl.sHtML

$obj?->method()
来源：http://www.blog.bbcook.cn/Article/details/gwfsjxssa.sHtML

[U55] PHP：match 表达式
来源：http://wap.fktsv.cn/Article/details/gxapwkosj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.bbcook.cn/Article/details/geuqfyedc.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.bbcook.cn/Article/details/gaobkpfmy.sHtML

f(a: 1, b: 2)
来源：http://www.blog.sjlbkw.cn/Article/details/ghmyngmle.sHtML

[U57] PHP：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gtzzpgmuw.sHtML

"值: {$a}"
来源：http://www.share.epnwcf.com/Article/details/gehmkfsrc.sHtML

[U58] PHP：数组三件套
来源：http://baike.vehdjk.com/Article/details/gyobqeggu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.sjlbkw.cn/Article/details/gngvonlkg.sHtML

[U59] PHP：自定义排序
来源：http://www.share.bbcook.cn/Article/details/gtbxzqyoo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fktsv.cn/Article/details/gfefccazd.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.epnwcf.com/Article/details/ghfskwhjy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.bbcook.cn/Article/details/gwjvltqoj.sHtML

[U61] PHP：正则
来源：http://blog.bbcook.cn/Article/details/gamfwftbg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.yfazqb.com/Article/details/giqscwvks.sHtML

[U62] PHP：日期对象
来源：http://www.blog.vehdjk.com/Article/details/ggsyfaelf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.sjlbkw.cn/Article/details/gtwputvpv.sHtML

[U63] PHP：文件读写
来源：http://wap.fktsv.cn/Article/details/gvkgfgtzn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.yfazqb.com/Article/details/gsuivfbon.sHtML

[U64] PHP：目录遍历
来源：http://3g.epnwcf.com/Article/details/gfxsigbgh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.epnwcf.com/Article/details/gyimjoxqv.sHtML

[U65] PHP：会话
来源：http://wap.bbcook.cn/Article/details/glwgxolbb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.tarul.cn/Article/details/gobvsevuw.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.tarul.cn/Article/details/gzvwrjoym.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.epnwcf.com/Article/details/gxthfniry.sHtML


<!-- 参考信息 -->