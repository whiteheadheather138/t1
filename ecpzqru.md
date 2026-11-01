代发 wailian999

[S39] C++：自定义比较器排序
来源：http://read.share.vehdjk.com/Article/details/gcwncpuiv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fktsv.cn/Article/details/ggqtovvkq.sHtML

[S40] C++：查找元素
来源：http://www.m.share.vehdjk.com/Article/details/gqcwhmgba.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.bbcook.cn/Article/details/gpmmqqsmp.sHtML

[S41] C++：类与构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gmzvalrzg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.sjlbkw.cn/Article/details/gjgbnfkqu.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fktsv.cn/Article/details/gwnjqitpa.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.sjlbkw.cn/Article/details/gcyxcdbls.sHtML

[S43] C++：智能指针
来源：http://www.blog.yfazqb.com/Article/details/gengkzgbf.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fktsv.cn/Article/details/groucikhl.sHtML

[S44] C++：引用传参
来源：http://blog.sjlbkw.cn/Article/details/gdxdgeikf.sHtML

void inc(int &x) { ++x; }
来源：http://blog.yfazqb.com/Article/details/grsdrosic.sHtML

[S45] C++：lambda
来源：http://3g.tarul.cn/Article/details/gdqgnsbqb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fktsv.cn/Article/details/gqwpwwsfb.sHtML

[S46] C++：函数模板
来源：http://blog.yfazqb.com/Article/details/gvleyaiea.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.vehdjk.com/Article/details/gvxnqypxv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gjjfnbggj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.yfazqb.com/Article/details/gbbxxqajl.sHtML

[S48] C++：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gmepprshk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.vehdjk.com/Article/details/gphojgisp.sHtML

while (std::getline(in, line)) { }
来源：http://blog.tarul.cn/Article/details/ghfyuqrsu.sHtML

[S49] C++：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/grqixhufw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.tarul.cn/Article/details/gwcckghcf.sHtML

[S50] C++：格式化数字
来源：http://baike.sjlbkw.cn/Article/details/gsnumjeqs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.vehdjk.com/Article/details/ghwjnsykx.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.bbcook.cn/Article/details/gtwktjrmh.sHtML

static_cast<double>(a) / b
来源：http://m.share.epnwcf.com/Article/details/grhwvrlxc.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.vehdjk.com/Article/details/gskmfrxnn.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.vehdjk.com/Article/details/ghnoynkff.sHtML

[S53] C++：移动语义
来源：http://blog.yfazqb.com/Article/details/grcnlcjug.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.vehdjk.com/Article/details/gzrehxhrg.sHtML

[S54] C++：异常处理
来源：http://blog.vehdjk.com/Article/details/gqaaggkjo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.epnwcf.com/Article/details/gxwjaevyc.sHtML

[S55] C++：结构化绑定
来源：http://3g.bbcook.cn/Article/details/gmthjawzj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.sjlbkw.cn/Article/details/gnplmjjbc.sHtML

[S56] C++：optional
来源：http://mobile.sjlbkw.cn/Article/details/gdzcepllg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fktsv.cn/Article/details/gojvksrvx.sHtML

[S57] C++：编译期常量
来源：http://www.share.tarul.cn/Article/details/gcfnjecrg.sHtML

constexpr int N = 10;
来源：http://wap.sjlbkw.cn/Article/details/gdzitujjv.sHtML

[S58] C++：命名空间
来源：http://m.share.epnwcf.com/Article/details/grasixnup.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.vehdjk.com/Article/details/grsaojzls.sHtML

[S59] C++：静态断言
来源：http://baike.vehdjk.com/Article/details/gnqzkgjth.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fktsv.cn/Article/details/gfxhvkmui.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.tarul.cn/Article/details/govtmxlxs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.tarul.cn/Article/details/gzngltmbu.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gdarursfv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.tarul.cn/Article/details/gtpxsjqfd.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/guzognwdq.sHtML

[T01] Kotlin：Hello World
来源：http://blog.tarul.cn/Article/details/gaowovaph.sHtML

println("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gsdxiurls.sHtML

[T02] Kotlin：变量
来源：http://m.share.epnwcf.com/Article/details/gkdefreeq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.bbcook.cn/Article/details/gxnxyjosp.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.yfazqb.com/Article/details/gwvzugaxn.sHtML

"值: $b"
来源：http://www.share.vehdjk.com/Article/details/gfozmuami.sHtML

[T04] Kotlin：空安全
来源：http://read.share.yfazqb.com/Article/details/gfimvyrnq.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.vehdjk.com/Article/details/gmkpukovx.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.bbcook.cn/Article/details/gjfpaicfj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.bbcook.cn/Article/details/gxyvbqkps.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.bbcook.cn/Article/details/gulxhygov.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gukhdehen.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.vehdjk.com/Article/details/gqxlhagwm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.epnwcf.com/Article/details/gdyddevje.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fktsv.cn/Article/details/gmweqfywv.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.yfazqb.com/Article/details/gzxyiwvra.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.epnwcf.com/Article/details/gscxfqbbr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fktsv.cn/Article/details/giypfgnhr.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gerpeigqe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.yfazqb.com/Article/details/gqtxoilmr.sHtML

[T11] Kotlin：协程
来源：http://blog.tarul.cn/Article/details/gmebrempd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.sjlbkw.cn/Article/details/guzqdosqw.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.bbcook.cn/Article/details/grzpxngqr.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.yfazqb.com/Article/details/guieoekwm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.vehdjk.com/Article/details/gmlqvfonx.sHtML

val m = mapOf("a" to 1)
来源：http://3g.yfazqb.com/Article/details/gscylgozt.sHtML

[T14] Kotlin：循环
来源：http://m.share.yfazqb.com/Article/details/gtjxvesoc.sHtML

for (i in 1..10) println(i)
来源：http://www.share.bbcook.cn/Article/details/gbfaugovt.sHtML

[T15] Kotlin：接口
来源：http://3g.sjlbkw.cn/Article/details/gbvfcopog.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.yfazqb.com/Article/details/gjmjszpjn.sHtML

[T16] Swift：Hello World
来源：http://3g.sjlbkw.cn/Article/details/ggsmhkayi.sHtML

print("Hello")
来源：http://mobile.vehdjk.com/Article/details/gddbnluhk.sHtML

[T17] Swift：变量与常量
来源：http://baike.yfazqb.com/Article/details/gxqeeujtm.sHtML

var a = 1;  let b = 2
来源：http://wap.epnwcf.com/Article/details/gaefcqfyk.sHtML

[T18] Swift：字符串插值
来源：http://wap.yfazqb.com/Article/details/gkmqidanq.sHtML

"值: \(b)"
来源：http://m.share.yfazqb.com/Article/details/gbgmqysvq.sHtML

[T19] Swift：可选绑定
来源：http://blog.vehdjk.com/Article/details/giqumzqub.sHtML

if let n = opt { print(n) }
来源：http://blog.yfazqb.com/Article/details/gooldcdpm.sHtML

[T20] Swift：数组操作
来源：http://www.share.fktsv.cn/Article/details/gixycuvyr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.vehdjk.com/Article/details/gqobinais.sHtML

[T21] Swift：遍历
来源：http://baike.bbcook.cn/Article/details/gsjtibxda.sHtML

for x in a { print(x) }
来源：http://m.share.bbcook.cn/Article/details/ggthwmbwm.sHtML

[T22] Swift：字典
来源：http://read.share.bbcook.cn/Article/details/gbtxxdyzv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.sjlbkw.cn/Article/details/gyiyxxuvz.sHtML

[T23] Swift：函数
来源：http://3g.sjlbkw.cn/Article/details/gkbkmoytc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.vehdjk.com/Article/details/gpfjontxu.sHtML

[T24] Swift：闭包
来源：http://wap.fktsv.cn/Article/details/gschsccps.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.bbcook.cn/Article/details/gkzadsxgu.sHtML

[T25] Swift：结构体
来源：http://www.share.tarul.cn/Article/details/gyixitetc.sHtML

struct P { var x: Int }
来源：http://www.share.vehdjk.com/Article/details/gytlrkyxm.sHtML

[T26] Swift：类与重写
来源：http://read.share.fktsv.cn/Article/details/gknpdlfek.sHtML

class A: Base { override func f() {} }
来源：http://3g.tarul.cn/Article/details/gpkdrudbj.sHtML

[T27] Swift：错误处理
来源：http://www.share.yfazqb.com/Article/details/gqemrxrgt.sHtML

do { try f() } catch { print(error) }
来源：http://baike.sjlbkw.cn/Article/details/gfkhzwowf.sHtML

[T28] Swift：枚举
来源：http://read.share.sjlbkw.cn/Article/details/gfbkftsyz.sHtML

enum Color { case red, green }
来源：http://baike.bbcook.cn/Article/details/gmodcejab.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.bbcook.cn/Article/details/gfnlcwqth.sHtML

guard let x = opt else { return }
来源：http://baike.tarul.cn/Article/details/gkscqegsg.sHtML

[T30] Swift：协议
来源：http://blog.sjlbkw.cn/Article/details/grcqvmans.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.yfazqb.com/Article/details/gfzzigxbh.sHtML

[T31] Lua：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gzhbvbdkt.sHtML

print("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gagncxuhv.sHtML

[T32] Lua：局部变量
来源：http://mobile.sjlbkw.cn/Article/details/gfnlahcbf.sHtML

local a = 1
来源：http://www.share.tarul.cn/Article/details/gpstirrjm.sHtML

[T33] Lua：表（数组）
来源：http://3g.bbcook.cn/Article/details/gbfbpnxuw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.vehdjk.com/Article/details/gkyitpsdn.sHtML

[T34] Lua：遍历表
来源：http://mobile.vehdjk.com/Article/details/glirywdir.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.tarul.cn/Article/details/gacjqcwpj.sHtML

[T35] Lua：字典表
来源：http://www.share.yfazqb.com/Article/details/gkaenxopb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.yfazqb.com/Article/details/gpwvxxxnd.sHtML

[T36] Lua：函数
来源：http://www.blog.epnwcf.com/Article/details/gextuobme.sHtML

function add(a, b) return a + b end
来源：http://www.share.epnwcf.com/Article/details/ghrtvllrh.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.epnwcf.com/Article/details/gsjuecaqp.sHtML

"a" .. "b"
来源：http://read.share.vehdjk.com/Article/details/gngeoogup.sHtML

[T38] Lua：条件
来源：http://www.blog.fktsv.cn/Article/details/gxtzfnvuj.sHtML

if x > 0 then print("正") end
来源：http://m.share.fktsv.cn/Article/details/gogtlouue.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.epnwcf.com/Article/details/gqmkhkknj.sHtML

string.find(s, "%d+")
来源：http://3g.vehdjk.com/Article/details/gttbmswvh.sHtML

[T40] Lua：元表
来源：http://read.share.sjlbkw.cn/Article/details/gixnziuth.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.bbcook.cn/Article/details/gevhtdnqg.sHtML

[T41] Perl：Hello World
来源：http://wap.epnwcf.com/Article/details/gekyaftqm.sHtML

print "Hello\n";
来源：http://blog.vehdjk.com/Article/details/glaqeyitm.sHtML

[T42] Perl：变量类型
来源：http://read.share.epnwcf.com/Article/details/gudxoxtwh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.bbcook.cn/Article/details/gdenalvfp.sHtML

[T43] Perl：字符串插值
来源：http://baike.tarul.cn/Article/details/grbzdprjs.sHtML

"值: $a"
来源：http://www.share.yfazqb.com/Article/details/gfbsmryun.sHtML

[T44] Perl：条件
来源：http://www.share.sjlbkw.cn/Article/details/galqordbi.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.yfazqb.com/Article/details/gmrknrpsf.sHtML

[T45] Perl：数组遍历
来源：http://read.share.tarul.cn/Article/details/gbkboucoj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.epnwcf.com/Article/details/gajlxtviz.sHtML

[T46] Perl：哈希操作
来源：http://mobile.yfazqb.com/Article/details/gvatugbtg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.vehdjk.com/Article/details/gyouyrdtt.sHtML

[T47] Perl：正则捕获
来源：http://read.share.sjlbkw.cn/Article/details/gaqiufmbj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.vehdjk.com/Article/details/glaqqmoze.sHtML

[T48] Perl：正则替换
来源：http://mobile.epnwcf.com/Article/details/gbfrriaaw.sHtML

$s =~ s/old/new/g;
来源：http://3g.tarul.cn/Article/details/guxwehcnm.sHtML

[T49] Perl：函数
来源：http://wap.fktsv.cn/Article/details/geoyngwko.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gojqmsvjm.sHtML

[T50] Perl：逐行读文件
来源：http://wap.yfazqb.com/Article/details/ghdvovnoh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fktsv.cn/Article/details/gcjkgshla.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fktsv.cn/Article/details/gclukvzfl.sHtML

[T51] Scala：Hello World
来源：http://read.share.epnwcf.com/Article/details/gqxvudvmk.sHtML

println("Hello")
来源：http://blog.bbcook.cn/Article/details/gvmquclpl.sHtML

[T52] Scala：变量
来源：http://wap.bbcook.cn/Article/details/gujwfllkg.sHtML

val a = 1;  var b = 2
来源：http://wap.bbcook.cn/Article/details/ggfgssrcf.sHtML

[T53] Scala：字符串插值
来源：http://blog.bbcook.cn/Article/details/goxorqekz.sHtML

s"值: $b"
来源：http://read.share.tarul.cn/Article/details/gvufeccgr.sHtML

[T54] Scala：集合映射
来源：http://mobile.bbcook.cn/Article/details/gyfmanccz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.epnwcf.com/Article/details/grqkllzoh.sHtML

[T55] Scala：集合过滤
来源：http://m.share.tarul.cn/Article/details/gcwnxjzzg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.sjlbkw.cn/Article/details/ghkauunwg.sHtML

[T56] Scala：样例类
来源：http://www.m.share.bbcook.cn/Article/details/gldzeojpt.sHtML

case class User(name: String, age: Int)
来源：http://www.share.tarul.cn/Article/details/goaqkcagp.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.vehdjk.com/Article/details/gsmiqeiaw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.epnwcf.com/Article/details/gpmklnfpz.sHtML

[T58] Scala：函数定义
来源：http://baike.fktsv.cn/Article/details/glwachopd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fktsv.cn/Article/details/grwaoyink.sHtML

[T59] Scala：循环
来源：http://www.share.fktsv.cn/Article/details/gypqmfozp.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.vehdjk.com/Article/details/gsqohijaa.sHtML

[T60] Scala：折叠
来源：http://www.blog.fktsv.cn/Article/details/ghwccoliq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.tarul.cn/Article/details/gshzqkjhv.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gmilmiyxg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.vehdjk.com/Article/details/gvkpmthti.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gdgffiosh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.yfazqb.com/Article/details/gjyxwizcc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.yfazqb.com/Article/details/glfjupjnk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fktsv.cn/Article/details/gtgnyhufk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.bbcook.cn/Article/details/gruksgszz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.epnwcf.com/Article/details/gyxrkbuor.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.vehdjk.com/Article/details/gwobnmums.sHtML

[U04] Py：变量调试打印
来源：http://wap.vehdjk.com/Article/details/gnxjxkmiq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.bbcook.cn/Article/details/gpaslnroe.sHtML

[U05] Py：列表去重且保序
来源：http://3g.sjlbkw.cn/Article/details/gsruyqdpc.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.sjlbkw.cn/Article/details/gwecxgvzz.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.yfazqb.com/Article/details/gefkhkocy.sHtML

{**a, **b}
来源：http://baike.fktsv.cn/Article/details/gsainvqkk.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.vehdjk.com/Article/details/gnfsvrqxs.sHtML

{v: k for k, v in d.items()}
来源：http://3g.tarul.cn/Article/details/gmmzrmopt.sHtML

[U08] Py：展平二维列表
来源：http://blog.bbcook.cn/Article/details/gcspljysc.sHtML

[y for x in nested for y in x]
来源：http://baike.vehdjk.com/Article/details/gngwxuttl.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.epnwcf.com/Article/details/gbaccrdmc.sHtML

max(d, key=d.get)
来源：http://wap.epnwcf.com/Article/details/gbeywqaye.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.bbcook.cn/Article/details/glcykeumc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.epnwcf.com/Article/details/gowyvndhn.sHtML

[U11] Py：生成器表达式
来源：http://baike.yfazqb.com/Article/details/gtkuupnlr.sHtML

(x * 2 for x in arr)
来源：http://read.share.tarul.cn/Article/details/godhxlknw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fktsv.cn/Article/details/gnhmponzs.sHtML

Counter(arr).most_common(3)
来源：http://read.share.sjlbkw.cn/Article/details/gqrwqudev.sHtML

[U13] Py：固定长度队列
来源：http://mobile.sjlbkw.cn/Article/details/glhtqcqmq.sHtML

deque(maxlen=10)
来源：http://www.blog.sjlbkw.cn/Article/details/giqwutpji.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.sjlbkw.cn/Article/details/grbxephbf.sHtML

defaultdict(list)
来源：http://www.m.share.fktsv.cn/Article/details/gwwhzmyol.sHtML

[U15] Py：高精度计时
来源：http://www.blog.yfazqb.com/Article/details/ghjqyoesk.sHtML

t = time.perf_counter()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxugimlkc.sHtML

[U16] Py：命令行参数解析
来源：http://wap.tarul.cn/Article/details/grcopesyd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fktsv.cn/Article/details/goybsimwa.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fktsv.cn/Article/details/gohprzsub.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fktsv.cn/Article/details/gpumldfgp.sHtML

[U18] Py：预编译正则
来源：http://www.share.sjlbkw.cn/Article/details/gsjnmqzdw.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.tarul.cn/Article/details/ggdlmfwsg.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.vehdjk.com/Article/details/gjgqmaieo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.yfazqb.com/Article/details/gtunnrobe.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.vehdjk.com/Article/details/gkfbjtwht.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.epnwcf.com/Article/details/gqshxxxwq.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fktsv.cn/Article/details/gnofnutkm.sHtML

@contextlib.contextmanager
来源：http://m.share.sjlbkw.cn/Article/details/goshktzdx.sHtML

[U22] Py：矩阵转置
来源：http://wap.tarul.cn/Article/details/gerrumvgq.sHtML

list(zip(*m))
来源：http://blog.tarul.cn/Article/details/ggoarvvqb.sHtML

[U23] Py：分块读取大文件
来源：http://blog.tarul.cn/Article/details/gktdqyyfk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.sjlbkw.cn/Article/details/gdoglntnt.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fktsv.cn/Article/details/gwktqmsbs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.epnwcf.com/Article/details/gbeizelvc.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.sjlbkw.cn/Article/details/gybijcrep.sHtML

csv.DictReader(f)
来源：http://baike.epnwcf.com/Article/details/gnlhgpgar.sHtML

[U26] Py：并发下载
来源：http://mobile.sjlbkw.cn/Article/details/gljylqndr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.epnwcf.com/Article/details/gfdrgfbop.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.sjlbkw.cn/Article/details/gabnbnumb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.tarul.cn/Article/details/gyjpgeihh.sHtML

[U28] Py：类型别名
来源：http://www.m.share.sjlbkw.cn/Article/details/gndirmaji.sHtML

UserId = int
来源：http://www.share.bbcook.cn/Article/details/gusywkxxt.sHtML

[U29] Py：属性校验
来源：http://www.share.yfazqb.com/Article/details/geturhfbv.sHtML

@property 与 @x.setter 配合
来源：http://mobile.bbcook.cn/Article/details/gtzgduuwz.sHtML

[U30] Py：数据类
来源：http://www.share.vehdjk.com/Article/details/gmbsnikie.sHtML

@dataclass(slots=True)
来源：http://mobile.epnwcf.com/Article/details/ggdsswlkk.sHtML

[U31] Py：单测
来源：http://blog.bbcook.cn/Article/details/gkynccbme.sHtML

python -m pytest -q
来源：http://mobile.sjlbkw.cn/Article/details/gbijpfrby.sHtML

[U32] Py：代码格式化
来源：http://wap.yfazqb.com/Article/details/gfygoxvdr.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.sjlbkw.cn/Article/details/gycloquot.sHtML

[U33] Py：打包发布
来源：http://www.m.share.bbcook.cn/Article/details/ggwqgjgid.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.tarul.cn/Article/details/gwlvnksuu.sHtML

[U34] Py：判断编码
来源：http://m.share.fktsv.cn/Article/details/gwxmipqwy.sHtML

chardet.detect(raw)
来源：http://m.share.epnwcf.com/Article/details/gsnbedzzp.sHtML

[U35] Py：发送邮件
来源：http://www.share.epnwcf.com/Article/details/gdthjracy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.sjlbkw.cn/Article/details/gmciaxgek.sHtML

[U36] Py：定时任务
来源：http://baike.vehdjk.com/Article/details/gngalzteh.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.tarul.cn/Article/details/gnapbuosp.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.epnwcf.com/Article/details/gdhrrghyy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.sjlbkw.cn/Article/details/ghtcvkost.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.yfazqb.com/Article/details/ghmfvpzbn.sHtML

Path(__file__).resolve().parent
来源：http://3g.yfazqb.com/Article/details/geozzekuz.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fktsv.cn/Article/details/ggdgozsbs.sHtML

sys.stdout.isatty()
来源：http://wap.epnwcf.com/Article/details/gpzsescbh.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fktsv.cn/Article/details/ghgemxgbr.sHtML

print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/gspqsnvto.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.yfazqb.com/Article/details/gkzfdxhlz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.tarul.cn/Article/details/gtmqdsjxd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.vehdjk.com/Article/details/geawdgojz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.bbcook.cn/Article/details/gzrkmwmxw.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.epnwcf.com/Article/details/gnojyinly.sHtML

namespace App\Http;
来源：http://read.share.fktsv.cn/Article/details/gjghcbfbb.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.bbcook.cn/Article/details/gptivukmi.sHtML

declare(strict_types=1);
来源：http://3g.vehdjk.com/Article/details/gdrnoduzn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.bbcook.cn/Article/details/gidmjwnad.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/gyvhtseuk.sHtML

[U46] PHP：可空类型
来源：http://3g.bbcook.cn/Article/details/gaaqktjlw.sHtML

?string $name = null
来源：http://read.share.vehdjk.com/Article/details/gpktoynqq.sHtML

[U47] PHP：联合类型
来源：http://mobile.fktsv.cn/Article/details/gcwowrnwu.sHtML

int|string $id
来源：http://blog.bbcook.cn/Article/details/gdinbvsfb.sHtML

[U48] PHP：纯枚举
来源：http://3g.fktsv.cn/Article/details/gwrozqhcl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.sjlbkw.cn/Article/details/gbnirossr.sHtML

[U49] PHP：只读属性
来源：http://www.blog.tarul.cn/Article/details/gaauenwhy.sHtML

public readonly string $name
来源：http://wap.sjlbkw.cn/Article/details/gwbscekgp.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.tarul.cn/Article/details/grkpwelky.sHtML

public function __construct(private int $id) {}
来源：http://3g.bbcook.cn/Article/details/gscxbzaje.sHtML

[U51] PHP：数组解构
来源：http://baike.fktsv.cn/Article/details/grfuqxkpi.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fktsv.cn/Article/details/gyoswqvyq.sHtML

[U52] PHP：箭头函数
来源：http://3g.tarul.cn/Article/details/gkczjijov.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.bbcook.cn/Article/details/gywddecse.sHtML

[U53] PHP：空合并运算符
来源：http://wap.sjlbkw.cn/Article/details/gqrwdgzmm.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.yfazqb.com/Article/details/gptvxwrge.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.yfazqb.com/Article/details/gwcnowaig.sHtML

$obj?->method()
来源：http://blog.fktsv.cn/Article/details/ggbywgnxm.sHtML

[U55] PHP：match 表达式
来源：http://3g.tarul.cn/Article/details/gvxmwyojr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.yfazqb.com/Article/details/goglcyunu.sHtML

[U56] PHP：命名参数
来源：http://blog.bbcook.cn/Article/details/gbikadliu.sHtML

f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gaawlwhdb.sHtML

[U57] PHP：字符串插值
来源：http://baike.vehdjk.com/Article/details/geqswxhcv.sHtML

"值: {$a}"
来源：http://m.share.fktsv.cn/Article/details/gfeupdnyl.sHtML

[U58] PHP：数组三件套
来源：http://wap.tarul.cn/Article/details/gwddmtifz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.epnwcf.com/Article/details/gljnwcyme.sHtML

[U59] PHP：自定义排序
来源：http://blog.yfazqb.com/Article/details/gbklgrabm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.bbcook.cn/Article/details/gnksymyra.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.sjlbkw.cn/Article/details/gtvkeaoif.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.yfazqb.com/Article/details/gbmjjilxs.sHtML

[U61] PHP：正则
来源：http://baike.fktsv.cn/Article/details/ghanxeney.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.epnwcf.com/Article/details/ggfemqnvq.sHtML

[U62] PHP：日期对象
来源：http://www.share.yfazqb.com/Article/details/glipmpawv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.vehdjk.com/Article/details/gtawtnbsp.sHtML

[U63] PHP：文件读写
来源：http://3g.bbcook.cn/Article/details/gptkvlimq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fktsv.cn/Article/details/grhdpfrcc.sHtML

[U64] PHP：目录遍历
来源：http://3g.vehdjk.com/Article/details/gwurulwhy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.vehdjk.com/Article/details/gomdabgkp.sHtML


<!-- 参考信息 -->