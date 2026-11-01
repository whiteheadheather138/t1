代发 wailian999

[S39] C++：自定义比较器排序
来源：http://blog.fktsv.cn/Article/details/gjhphhnvj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.tarul.cn/Article/details/gvmezaaev.sHtML

[S40] C++：查找元素
来源：http://3g.epnwcf.com/Article/details/gwwvhqsdq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gjdflmhsc.sHtML

[S41] C++：类与构造函数
来源：http://wap.tarul.cn/Article/details/gmeqcbjzs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fktsv.cn/Article/details/gnicycvxy.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.sjlbkw.cn/Article/details/gzvlsinzd.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.bbcook.cn/Article/details/gwmbonpvg.sHtML

[S43] C++：智能指针
来源：http://3g.epnwcf.com/Article/details/glsapjdsd.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.tarul.cn/Article/details/gjwebpipe.sHtML

[S44] C++：引用传参
来源：http://read.share.tarul.cn/Article/details/gqiheugsb.sHtML

void inc(int &x) { ++x; }
来源：http://blog.yfazqb.com/Article/details/gkpftmvye.sHtML

[S45] C++：lambda
来源：http://mobile.tarul.cn/Article/details/gdawufnut.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.sjlbkw.cn/Article/details/gncfsadnt.sHtML

[S46] C++：函数模板
来源：http://m.share.bbcook.cn/Article/details/guhabxxap.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.yfazqb.com/Article/details/gcypsalhh.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fktsv.cn/Article/details/gcshwtzwp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.epnwcf.com/Article/details/gcymcqhdi.sHtML

[S48] C++：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gzzftiipu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fktsv.cn/Article/details/gbrnemegf.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.vehdjk.com/Article/details/ggdktdoqp.sHtML

[S49] C++：写文件
来源：http://wap.tarul.cn/Article/details/gkkhcvrom.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.bbcook.cn/Article/details/gjlrlvzxj.sHtML

[S50] C++：格式化数字
来源：http://blog.epnwcf.com/Article/details/gglpkcert.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.tarul.cn/Article/details/gzvmtcrhj.sHtML

[S51] C++：显式类型转换
来源：http://baike.vehdjk.com/Article/details/grdxtfwln.sHtML

static_cast<double>(a) / b
来源：http://mobile.bbcook.cn/Article/details/gyasnvzmj.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.sjlbkw.cn/Article/details/grooeqeao.sHtML

int size() const noexcept { return n_; }
来源：http://wap.epnwcf.com/Article/details/gysgwrglk.sHtML

[S53] C++：移动语义
来源：http://baike.fktsv.cn/Article/details/gfddqzsdk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.vehdjk.com/Article/details/gbsheeyaw.sHtML

[S54] C++：异常处理
来源：http://www.blog.yfazqb.com/Article/details/gojypaazx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fktsv.cn/Article/details/gmmxhmurm.sHtML

[S55] C++：结构化绑定
来源：http://read.share.bbcook.cn/Article/details/gcmjglzlu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.vehdjk.com/Article/details/gfrvoxaic.sHtML

[S56] C++：optional
来源：http://read.share.tarul.cn/Article/details/gprldqvep.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.epnwcf.com/Article/details/gwezqlsrs.sHtML

[S57] C++：编译期常量
来源：http://baike.yfazqb.com/Article/details/grvuguvtk.sHtML

constexpr int N = 10;
来源：http://www.blog.yfazqb.com/Article/details/gsmdhspjj.sHtML

[S58] C++：命名空间
来源：http://read.share.tarul.cn/Article/details/gfivmorxz.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.tarul.cn/Article/details/gkwctuwzy.sHtML

[S59] C++：静态断言
来源：http://blog.tarul.cn/Article/details/gjebjnboh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.epnwcf.com/Article/details/gwgtmnvsj.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.sjlbkw.cn/Article/details/ghbsmvqqv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fktsv.cn/Article/details/gtnyaxjwi.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/glddmjrxu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.bbcook.cn/Article/details/gygffhncf.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gzjskngyd.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.tarul.cn/Article/details/gvxulvpgw.sHtML

println("Hello")
来源：http://baike.tarul.cn/Article/details/gttipnvby.sHtML

[T02] Kotlin：变量
来源：http://www.share.vehdjk.com/Article/details/gfaqxklks.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.bbcook.cn/Article/details/gslcglzll.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fktsv.cn/Article/details/gbtfwaflb.sHtML

"值: $b"
来源：http://www.blog.yfazqb.com/Article/details/gkdyujhti.sHtML

[T04] Kotlin：空安全
来源：http://www.share.sjlbkw.cn/Article/details/gsyzjqqyi.sHtML

val n: String? = null;  n?.length
来源：http://www.share.bbcook.cn/Article/details/geqoydrni.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.yfazqb.com/Article/details/gdhrbovaa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.sjlbkw.cn/Article/details/gpxbxftre.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.vehdjk.com/Article/details/gyynpflau.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.tarul.cn/Article/details/glgywzinq.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.vehdjk.com/Article/details/gtgbycnei.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.tarul.cn/Article/details/gztecjrty.sHtML

[T08] Kotlin：数据类
来源：http://wap.yfazqb.com/Article/details/gfmxtgkwf.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.vehdjk.com/Article/details/gypbgzmtu.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.epnwcf.com/Article/details/gmavkkksm.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.tarul.cn/Article/details/gfqnspsns.sHtML

[T10] Kotlin：默认参数
来源：http://wap.tarul.cn/Article/details/guljmlypc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.tarul.cn/Article/details/gfveqdbsv.sHtML

[T11] Kotlin：协程
来源：http://www.share.tarul.cn/Article/details/ghaclzdco.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.tarul.cn/Article/details/gvznstkrn.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.epnwcf.com/Article/details/gmqvcefja.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.bbcook.cn/Article/details/gelksxlyp.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.bbcook.cn/Article/details/gjafafvjl.sHtML

val m = mapOf("a" to 1)
来源：http://3g.sjlbkw.cn/Article/details/gmnssaddj.sHtML

[T14] Kotlin：循环
来源：http://wap.tarul.cn/Article/details/gbjgafrtg.sHtML

for (i in 1..10) println(i)
来源：http://wap.sjlbkw.cn/Article/details/gaqzmqdny.sHtML

[T15] Kotlin：接口
来源：http://m.share.fktsv.cn/Article/details/gwlxccwbf.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.vehdjk.com/Article/details/grjbyfrtu.sHtML

[T16] Swift：Hello World
来源：http://blog.bbcook.cn/Article/details/gyegyxwoy.sHtML

print("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gsqlwbiie.sHtML

[T17] Swift：变量与常量
来源：http://read.share.yfazqb.com/Article/details/gfjqvdsom.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.vehdjk.com/Article/details/gyjueswyy.sHtML

[T18] Swift：字符串插值
来源：http://blog.yfazqb.com/Article/details/goycprjtd.sHtML

"值: \(b)"
来源：http://wap.epnwcf.com/Article/details/gtcyzfxnc.sHtML

[T19] Swift：可选绑定
来源：http://baike.sjlbkw.cn/Article/details/gktercnfs.sHtML

if let n = opt { print(n) }
来源：http://m.share.fktsv.cn/Article/details/gtrchkenr.sHtML

[T20] Swift：数组操作
来源：http://read.share.vehdjk.com/Article/details/gcesxrpva.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fktsv.cn/Article/details/gzyixqlsz.sHtML

[T21] Swift：遍历
来源：http://www.blog.epnwcf.com/Article/details/grdblskdb.sHtML

for x in a { print(x) }
来源：http://wap.epnwcf.com/Article/details/gcjuubgbw.sHtML

[T22] Swift：字典
来源：http://wap.tarul.cn/Article/details/gwpytcwom.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.tarul.cn/Article/details/gvcnnuatb.sHtML

[T23] Swift：函数
来源：http://mobile.vehdjk.com/Article/details/gmbwikykz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.bbcook.cn/Article/details/ggyzyhjdv.sHtML

[T24] Swift：闭包
来源：http://www.blog.vehdjk.com/Article/details/gynbtndvw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.tarul.cn/Article/details/gnsbmvxwk.sHtML

[T25] Swift：结构体
来源：http://3g.bbcook.cn/Article/details/gbevflrsw.sHtML

struct P { var x: Int }
来源：http://3g.vehdjk.com/Article/details/gtcutydxm.sHtML

[T26] Swift：类与重写
来源：http://baike.bbcook.cn/Article/details/grhowzfjv.sHtML

class A: Base { override func f() {} }
来源：http://3g.vehdjk.com/Article/details/gefmnnczo.sHtML

[T27] Swift：错误处理
来源：http://mobile.sjlbkw.cn/Article/details/gqpkuasov.sHtML

do { try f() } catch { print(error) }
来源：http://wap.yfazqb.com/Article/details/gzohjycvw.sHtML

[T28] Swift：枚举
来源：http://3g.bbcook.cn/Article/details/giqfajzms.sHtML

enum Color { case red, green }
来源：http://read.share.epnwcf.com/Article/details/gmqqpgcjx.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fktsv.cn/Article/details/ghrxqvmcw.sHtML

guard let x = opt else { return }
来源：http://wap.epnwcf.com/Article/details/gbphgmrzs.sHtML

[T30] Swift：协议
来源：http://www.share.vehdjk.com/Article/details/ghcpweswo.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fktsv.cn/Article/details/grhufbakp.sHtML

[T31] Lua：Hello World
来源：http://mobile.yfazqb.com/Article/details/gmynplcrs.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gonfcgzqq.sHtML

[T32] Lua：局部变量
来源：http://mobile.bbcook.cn/Article/details/gkobqghwc.sHtML

local a = 1
来源：http://read.share.tarul.cn/Article/details/ghqebfvqu.sHtML

[T33] Lua：表（数组）
来源：http://baike.yfazqb.com/Article/details/gouddzggn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.vehdjk.com/Article/details/glbskhiyw.sHtML

[T34] Lua：遍历表
来源：http://baike.tarul.cn/Article/details/gzfhenxpi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.epnwcf.com/Article/details/gsxsawhjs.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fktsv.cn/Article/details/gkiasuvij.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fktsv.cn/Article/details/gemefdqmg.sHtML

[T36] Lua：函数
来源：http://baike.epnwcf.com/Article/details/gdwewdewb.sHtML

function add(a, b) return a + b end
来源：http://blog.sjlbkw.cn/Article/details/gerxbtfrv.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.epnwcf.com/Article/details/gjhlwsqgg.sHtML

"a" .. "b"
来源：http://www.share.vehdjk.com/Article/details/ggqyeocgc.sHtML

[T38] Lua：条件
来源：http://wap.fktsv.cn/Article/details/ggjlnxoda.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.tarul.cn/Article/details/gxonmxeur.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fktsv.cn/Article/details/gfbjpvzud.sHtML

string.find(s, "%d+")
来源：http://baike.fktsv.cn/Article/details/gdzybitrj.sHtML

[T40] Lua：元表
来源：http://www.m.share.tarul.cn/Article/details/gxyurudno.sHtML

setmetatable({}, { __index = base })
来源：http://blog.vehdjk.com/Article/details/gxgyckhkc.sHtML

[T41] Perl：Hello World
来源：http://www.share.epnwcf.com/Article/details/gbbbdeupi.sHtML

print "Hello\n";
来源：http://www.m.share.yfazqb.com/Article/details/gwiyjsuoi.sHtML

[T42] Perl：变量类型
来源：http://wap.yfazqb.com/Article/details/gnhmcnfgv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.tarul.cn/Article/details/gintsdmnp.sHtML

[T43] Perl：字符串插值
来源：http://baike.vehdjk.com/Article/details/gfcmxgbwo.sHtML

"值: $a"
来源：http://www.share.epnwcf.com/Article/details/ggwjiwzar.sHtML

[T44] Perl：条件
来源：http://www.share.epnwcf.com/Article/details/gajqkrjzk.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fktsv.cn/Article/details/gimeetjlm.sHtML

[T45] Perl：数组遍历
来源：http://www.share.epnwcf.com/Article/details/glyfwtdpb.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fktsv.cn/Article/details/gykytwijw.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fktsv.cn/Article/details/gsikxmnot.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.epnwcf.com/Article/details/ggyaedjjl.sHtML

[T47] Perl：正则捕获
来源：http://blog.epnwcf.com/Article/details/gemrugpsp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fktsv.cn/Article/details/gewdegoqq.sHtML

[T48] Perl：正则替换
来源：http://m.share.tarul.cn/Article/details/gkndxftxw.sHtML

$s =~ s/old/new/g;
来源：http://wap.yfazqb.com/Article/details/gidvrwujz.sHtML

[T49] Perl：函数
来源：http://read.share.sjlbkw.cn/Article/details/grpzmatnd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/gadlhhpzg.sHtML

[T50] Perl：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gvhtgqnyq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.sjlbkw.cn/Article/details/goiawrshe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fktsv.cn/Article/details/gdhzwrzqz.sHtML

[T51] Scala：Hello World
来源：http://read.share.bbcook.cn/Article/details/gnrkmlaez.sHtML

println("Hello")
来源：http://m.share.yfazqb.com/Article/details/ggupyvodi.sHtML

[T52] Scala：变量
来源：http://read.share.epnwcf.com/Article/details/gbtagiujs.sHtML

val a = 1;  var b = 2
来源：http://blog.fktsv.cn/Article/details/gcbacndmy.sHtML

[T53] Scala：字符串插值
来源：http://read.share.tarul.cn/Article/details/guqasiymd.sHtML

s"值: $b"
来源：http://m.share.yfazqb.com/Article/details/ghnwtserj.sHtML

[T54] Scala：集合映射
来源：http://mobile.tarul.cn/Article/details/gcjuleeat.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.yfazqb.com/Article/details/gwonaukce.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gywatdghw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.tarul.cn/Article/details/gvjdxjzno.sHtML

[T56] Scala：样例类
来源：http://www.share.vehdjk.com/Article/details/ghiexbkzt.sHtML

case class User(name: String, age: Int)
来源：http://read.share.bbcook.cn/Article/details/gxpltnvgx.sHtML

[T57] Scala：模式匹配
来源：http://baike.vehdjk.com/Article/details/gleupwjgl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.yfazqb.com/Article/details/gycmimjxk.sHtML

[T58] Scala：函数定义
来源：http://baike.tarul.cn/Article/details/gcnurazdm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.yfazqb.com/Article/details/gqbbzasqt.sHtML

[T59] Scala：循环
来源：http://blog.yfazqb.com/Article/details/gcwekhmrl.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.epnwcf.com/Article/details/ghmgnojfb.sHtML

[T60] Scala：折叠
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmzawdep.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.bbcook.cn/Article/details/giyoibxus.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/guybnkypn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.vehdjk.com/Article/details/gcrvfnyrn.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gcbflcujn.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.vehdjk.com/Article/details/gpobxwbsc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.bbcook.cn/Article/details/gxwfbftqd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fktsv.cn/Article/details/giynlfgyx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.tarul.cn/Article/details/gynlnqcgb.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.epnwcf.com/Article/details/gmnkxmzbs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.sjlbkw.cn/Article/details/geqdjdhbl.sHtML

[U04] Py：变量调试打印
来源：http://www.share.yfazqb.com/Article/details/gfopgtmua.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.yfazqb.com/Article/details/gnamxcyvh.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.tarul.cn/Article/details/gxvuoitkg.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fktsv.cn/Article/details/gnwdkkfup.sHtML

[U06] Py：合并两个字典
来源：http://mobile.yfazqb.com/Article/details/gurqnceth.sHtML

{**a, **b}
来源：http://mobile.fktsv.cn/Article/details/goapbsfsh.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.bbcook.cn/Article/details/gwyhnjwcb.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.tarul.cn/Article/details/gdgydlkkt.sHtML

[U08] Py：展平二维列表
来源：http://m.share.tarul.cn/Article/details/goidnektm.sHtML

[y for x in nested for y in x]
来源：http://mobile.fktsv.cn/Article/details/gunlhnsfy.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.tarul.cn/Article/details/giihmdntt.sHtML

max(d, key=d.get)
来源：http://baike.bbcook.cn/Article/details/gleaqoxdy.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fktsv.cn/Article/details/gdyvonkqu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.bbcook.cn/Article/details/guldeskpe.sHtML

[U11] Py：生成器表达式
来源：http://wap.bbcook.cn/Article/details/grmcieozi.sHtML

(x * 2 for x in arr)
来源：http://mobile.fktsv.cn/Article/details/ggpilsraa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fktsv.cn/Article/details/gqzjxouip.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gdnzhzknr.sHtML

[U13] Py：固定长度队列
来源：http://3g.sjlbkw.cn/Article/details/gfitvlyxw.sHtML

deque(maxlen=10)
来源：http://wap.vehdjk.com/Article/details/gotmfzcdc.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.bbcook.cn/Article/details/gfakvtgnj.sHtML

defaultdict(list)
来源：http://mobile.fktsv.cn/Article/details/gukdbtllk.sHtML

[U15] Py：高精度计时
来源：http://baike.yfazqb.com/Article/details/grpbywcbi.sHtML

t = time.perf_counter()
来源：http://3g.epnwcf.com/Article/details/givckzpqc.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.vehdjk.com/Article/details/gaglnhavq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.bbcook.cn/Article/details/gxhmvnshk.sHtML

[U17] Py：初始化日志
来源：http://read.share.tarul.cn/Article/details/gaafwcfhd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.sjlbkw.cn/Article/details/gxqdladye.sHtML

[U18] Py：预编译正则
来源：http://m.share.epnwcf.com/Article/details/ghiqqnjnm.sHtML

pat = re.compile(r"\d+")
来源：http://baike.bbcook.cn/Article/details/gsadjssfd.sHtML

[U19] Py：正则替换带回调
来源：http://3g.sjlbkw.cn/Article/details/gqjtnofcb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.tarul.cn/Article/details/gdmlblxmt.sHtML

[U20] Py：缓存函数结果
来源：http://3g.yfazqb.com/Article/details/ghhenvnkw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.tarul.cn/Article/details/gecyqwhll.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.vehdjk.com/Article/details/ghidiijzp.sHtML

@contextlib.contextmanager
来源：http://baike.bbcook.cn/Article/details/gckfkwxcx.sHtML

[U22] Py：矩阵转置
来源：http://3g.fktsv.cn/Article/details/gaymgseeu.sHtML

list(zip(*m))
来源：http://mobile.yfazqb.com/Article/details/gymtytqgr.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.vehdjk.com/Article/details/gkhswyzgp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.yfazqb.com/Article/details/gufknofoz.sHtML

[U24] Py：路径操作
来源：http://wap.yfazqb.com/Article/details/gsqhpeelx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.bbcook.cn/Article/details/gswapbual.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fktsv.cn/Article/details/gdcotwjfu.sHtML

csv.DictReader(f)
来源：http://wap.tarul.cn/Article/details/gmrbhahvi.sHtML

[U26] Py：并发下载
来源：http://www.blog.yfazqb.com/Article/details/gtcpjkmuu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.epnwcf.com/Article/details/gbahhhmqa.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.sjlbkw.cn/Article/details/gnzjbadcb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.bbcook.cn/Article/details/gnlcbnslf.sHtML

[U28] Py：类型别名
来源：http://www.share.epnwcf.com/Article/details/gnnfmzzxd.sHtML

UserId = int
来源：http://baike.fktsv.cn/Article/details/gzkulajrg.sHtML

[U29] Py：属性校验
来源：http://mobile.vehdjk.com/Article/details/gyoxdzxgo.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fktsv.cn/Article/details/gxawyiyla.sHtML

[U30] Py：数据类
来源：http://3g.fktsv.cn/Article/details/gwgdxhcop.sHtML

@dataclass(slots=True)
来源：http://www.blog.vehdjk.com/Article/details/gkxbfcvlz.sHtML

[U31] Py：单测
来源：http://3g.fktsv.cn/Article/details/giqerszko.sHtML

python -m pytest -q
来源：http://www.share.fktsv.cn/Article/details/gmbwfncwv.sHtML

[U32] Py：代码格式化
来源：http://read.share.fktsv.cn/Article/details/gbhphwkoq.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.yfazqb.com/Article/details/gfoxuwiid.sHtML

[U33] Py：打包发布
来源：http://wap.epnwcf.com/Article/details/gnfviltrj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.bbcook.cn/Article/details/giuwmdavx.sHtML

[U34] Py：判断编码
来源：http://3g.yfazqb.com/Article/details/gbakrhrcs.sHtML

chardet.detect(raw)
来源：http://wap.sjlbkw.cn/Article/details/gpgqchzuv.sHtML

[U35] Py：发送邮件
来源：http://3g.bbcook.cn/Article/details/gvzafjbmk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.yfazqb.com/Article/details/gnusczdff.sHtML

[U36] Py：定时任务
来源：http://read.share.bbcook.cn/Article/details/gnkafrpma.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.tarul.cn/Article/details/geyrlwrob.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fktsv.cn/Article/details/gwoinjcbe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.bbcook.cn/Article/details/guhnjbfei.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.yfazqb.com/Article/details/gdkehqvzj.sHtML

Path(__file__).resolve().parent
来源：http://blog.fktsv.cn/Article/details/gxpgbaxtc.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.vehdjk.com/Article/details/gicxxgfmn.sHtML

sys.stdout.isatty()
来源：http://www.blog.epnwcf.com/Article/details/gcnewxayh.sHtML

[U40] Py：打印到标准错误
来源：http://wap.yfazqb.com/Article/details/gaklgqpsd.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fktsv.cn/Article/details/gklwlnuhs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.epnwcf.com/Article/details/gktulxsyt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.bbcook.cn/Article/details/gcpluygly.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fktsv.cn/Article/details/gdinpwdcy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.vehdjk.com/Article/details/gxqzxdhju.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.tarul.cn/Article/details/ghkpefclo.sHtML

namespace App\Http;
来源：http://www.blog.yfazqb.com/Article/details/ghwheeyrn.sHtML

[U44] PHP：开启严格类型
来源：http://blog.sjlbkw.cn/Article/details/giuwrqvzq.sHtML

declare(strict_types=1);
来源：http://m.share.sjlbkw.cn/Article/details/gfmgwdmed.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.yfazqb.com/Article/details/gnfndqvuo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gvdbjzipu.sHtML

[U46] PHP：可空类型
来源：http://read.share.fktsv.cn/Article/details/gplricgxv.sHtML

?string $name = null
来源：http://www.share.vehdjk.com/Article/details/gtnvwsyzn.sHtML

[U47] PHP：联合类型
来源：http://blog.vehdjk.com/Article/details/gxsoqunbv.sHtML

int|string $id
来源：http://blog.tarul.cn/Article/details/gvqecgwqp.sHtML

[U48] PHP：纯枚举
来源：http://baike.sjlbkw.cn/Article/details/gsetwzyzj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.bbcook.cn/Article/details/gklsgbtxt.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.epnwcf.com/Article/details/gplzeutgo.sHtML

public readonly string $name
来源：http://www.share.fktsv.cn/Article/details/gbllunxjd.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.tarul.cn/Article/details/gxbcetmbu.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fktsv.cn/Article/details/gqdrtamro.sHtML

[U51] PHP：数组解构
来源：http://www.blog.bbcook.cn/Article/details/gkuglsnpn.sHtML

[$a, $b] = $arr;
来源：http://baike.yfazqb.com/Article/details/gcgnezhdc.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.vehdjk.com/Article/details/gunmcsytw.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.sjlbkw.cn/Article/details/gjvgnuhyn.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.tarul.cn/Article/details/gxclmuhwx.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.tarul.cn/Article/details/giupvmbed.sHtML

[U54] PHP：空安全调用
来源：http://www.share.tarul.cn/Article/details/gsuyovlad.sHtML

$obj?->method()
来源：http://baike.sjlbkw.cn/Article/details/ghepyibvh.sHtML

[U55] PHP：match 表达式
来源：http://mobile.yfazqb.com/Article/details/ghufpqend.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.vehdjk.com/Article/details/gvyicimmv.sHtML

[U56] PHP：命名参数
来源：http://3g.tarul.cn/Article/details/gxoigqxff.sHtML

f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/gcuybmeha.sHtML

[U57] PHP：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gzdzbaigy.sHtML

"值: {$a}"
来源：http://baike.fktsv.cn/Article/details/gynyalycq.sHtML

[U58] PHP：数组三件套
来源：http://read.share.epnwcf.com/Article/details/gvzuhgpme.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.yfazqb.com/Article/details/gvzazhumt.sHtML

[U59] PHP：自定义排序
来源：http://blog.epnwcf.com/Article/details/ggbomakav.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.tarul.cn/Article/details/gyfbghevd.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.sjlbkw.cn/Article/details/gtowdkfnv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.sjlbkw.cn/Article/details/gegqufjfq.sHtML

[U61] PHP：正则
来源：http://3g.vehdjk.com/Article/details/gtthduwel.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gpdueuwqy.sHtML

[U62] PHP：日期对象
来源：http://baike.epnwcf.com/Article/details/gbpzpaxai.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.tarul.cn/Article/details/gzkhfujsj.sHtML

[U63] PHP：文件读写
来源：http://www.share.sjlbkw.cn/Article/details/gqugivdjo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.epnwcf.com/Article/details/goymksird.sHtML

[U64] PHP：目录遍历
来源：http://mobile.bbcook.cn/Article/details/gsvlzekzq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.bbcook.cn/Article/details/gqkepgagn.sHtML


<!-- 参考信息 -->