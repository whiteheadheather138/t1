代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.yfazqb.com/Article/details/gzoivozdh.sHtML

[S21] C：字符类别判断
来源：http://read.share.yfazqb.com/Article/details/gkaoxteru.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fktsv.cn/Article/details/gnvwxyplz.sHtML

[S22] C：字符串转数字
来源：http://www.share.tarul.cn/Article/details/gtdyepbof.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.epnwcf.com/Article/details/gfopnykig.sHtML

[S23] C：随机数
来源：http://blog.vehdjk.com/Article/details/ghiplnild.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.vehdjk.com/Article/details/gylcunict.sHtML

[S24] C：获取本地时间
来源：http://wap.sjlbkw.cn/Article/details/grxxbvfdk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.bbcook.cn/Article/details/gprenhnmx.sHtML

[S25] C：内存拷贝
来源：http://blog.epnwcf.com/Article/details/gtagznrue.sHtML

memcpy(dst, src, n);
来源：http://baike.tarul.cn/Article/details/gutvfihjc.sHtML

[S26] C：内存清零
来源：http://blog.fktsv.cn/Article/details/gtoydprvs.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.tarul.cn/Article/details/gashhylpd.sHtML

[S27] C：定义常量
来源：http://www.blog.bbcook.cn/Article/details/gpqneaeps.sHtML

const double PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gihhnybqc.sHtML

[S28] C：静态变量
来源：http://read.share.sjlbkw.cn/Article/details/gflsgfsxq.sHtML

static int counter = 0;
来源：http://read.share.tarul.cn/Article/details/gewwfvopu.sHtML

[S29] C：变参函数
来源：http://www.blog.fktsv.cn/Article/details/gmkddhrjo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.bbcook.cn/Article/details/gbvvuinsu.sHtML

[S30] C：头文件保护
来源：http://www.m.share.sjlbkw.cn/Article/details/gxospfxwc.sHtML

#ifndef X_H
来源：http://mobile.vehdjk.com/Article/details/gmiunkcjr.sHtML

#define X_H
来源：http://blog.bbcook.cn/Article/details/ghseqrlqe.sHtML

#endif
来源：http://read.share.epnwcf.com/Article/details/ggseiaxcd.sHtML

[S31] C++：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gqmhptbsw.sHtML

#include <iostream>
来源：http://blog.epnwcf.com/Article/details/gcbcsdzmf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.bbcook.cn/Article/details/gkqludcwg.sHtML

[S32] C++：字符串
来源：http://m.share.sjlbkw.cn/Article/details/gvehftqnj.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.bbcook.cn/Article/details/gvkgolekc.sHtML

[S33] C++：vector 增删
来源：http://m.share.fktsv.cn/Article/details/gdorxpjvd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.yfazqb.com/Article/details/grophjfrt.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fktsv.cn/Article/details/gdgscubyf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.vehdjk.com/Article/details/gdcpmfluj.sHtML

[S35] C++：map
来源：http://www.blog.fktsv.cn/Article/details/gxircfjyt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fktsv.cn/Article/details/ggjzltchk.sHtML

[S36] C++：unordered_map
来源：http://blog.bbcook.cn/Article/details/gqtsjvvgc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gnamexyol.sHtML

[S37] C++：set
来源：http://baike.bbcook.cn/Article/details/gducrhkjl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fktsv.cn/Article/details/gqkpfsgfq.sHtML

[S38] C++：排序
来源：http://mobile.epnwcf.com/Article/details/gicivtphk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.tarul.cn/Article/details/gzkzdqana.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.bbcook.cn/Article/details/ghzeztptb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.yfazqb.com/Article/details/goevjmkxa.sHtML

[S40] C++：查找元素
来源：http://baike.bbcook.cn/Article/details/gakzvwlum.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.yfazqb.com/Article/details/gcnyeudak.sHtML

[S41] C++：类与构造函数
来源：http://blog.yfazqb.com/Article/details/gclelpmfx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.epnwcf.com/Article/details/gcrcidnlq.sHtML

[S42] C++：继承与虚函数
来源：http://baike.tarul.cn/Article/details/grrvymsus.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.bbcook.cn/Article/details/gdqngskuc.sHtML

[S43] C++：智能指针
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvkiotoz.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.yfazqb.com/Article/details/gqpbdpdnm.sHtML

[S44] C++：引用传参
来源：http://3g.tarul.cn/Article/details/gzuqobyrc.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fktsv.cn/Article/details/gzhceofvl.sHtML

[S45] C++：lambda
来源：http://mobile.yfazqb.com/Article/details/gjytjwxbx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.sjlbkw.cn/Article/details/gqghgovuq.sHtML

[S46] C++：函数模板
来源：http://baike.vehdjk.com/Article/details/gifhgvsul.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.sjlbkw.cn/Article/details/gwpcegkcq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.sjlbkw.cn/Article/details/groiyeiva.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.sjlbkw.cn/Article/details/gwrcufjiu.sHtML

[S48] C++：逐行读文件
来源：http://3g.tarul.cn/Article/details/guvtsjkxt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.yfazqb.com/Article/details/gdgbaapqj.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.yfazqb.com/Article/details/gkdbdrvpf.sHtML

[S49] C++：写文件
来源：http://blog.tarul.cn/Article/details/gbgeimxdc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.sjlbkw.cn/Article/details/gdxmpwugn.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.vehdjk.com/Article/details/gxiydivee.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fktsv.cn/Article/details/gmgdowvvu.sHtML

[S51] C++：显式类型转换
来源：http://baike.vehdjk.com/Article/details/gpqzixqgg.sHtML

static_cast<double>(a) / b
来源：http://mobile.tarul.cn/Article/details/gystnwyxr.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.bbcook.cn/Article/details/gcinbsfag.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.yfazqb.com/Article/details/gebdohffi.sHtML

[S53] C++：移动语义
来源：http://read.share.vehdjk.com/Article/details/gdparfbjf.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.bbcook.cn/Article/details/gecnjhzif.sHtML

[S54] C++：异常处理
来源：http://www.blog.tarul.cn/Article/details/ghlfwkkwj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.tarul.cn/Article/details/gaantsdmj.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fktsv.cn/Article/details/gsgzmqkfu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.tarul.cn/Article/details/gmaqgxvxu.sHtML

[S56] C++：optional
来源：http://www.m.share.epnwcf.com/Article/details/gwqljqbrg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.vehdjk.com/Article/details/glraxzmmc.sHtML

[S57] C++：编译期常量
来源：http://mobile.sjlbkw.cn/Article/details/gwivqoiim.sHtML

constexpr int N = 10;
来源：http://mobile.epnwcf.com/Article/details/gymhnuaik.sHtML

[S58] C++：命名空间
来源：http://baike.vehdjk.com/Article/details/ggzojmzfz.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.bbcook.cn/Article/details/gredctlew.sHtML

[S59] C++：静态断言
来源：http://mobile.bbcook.cn/Article/details/gzebfnzbj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.sjlbkw.cn/Article/details/gvryldxtw.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.tarul.cn/Article/details/gbubplovm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.bbcook.cn/Article/details/gzqttogot.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gznjvrrkc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.bbcook.cn/Article/details/gxvdprunk.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ghadoiccg.sHtML

[T01] Kotlin：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gytxfilyl.sHtML

println("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gukqrssub.sHtML

[T02] Kotlin：变量
来源：http://read.share.epnwcf.com/Article/details/gjomiepgn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fktsv.cn/Article/details/gzlxybsqp.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.sjlbkw.cn/Article/details/glxsgjpjl.sHtML

"值: $b"
来源：http://www.m.share.sjlbkw.cn/Article/details/grhhwqioo.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.bbcook.cn/Article/details/gtoitzoib.sHtML

val n: String? = null;  n?.length
来源：http://baike.yfazqb.com/Article/details/gidfuftcm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.yfazqb.com/Article/details/gcmjcfcnv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.bbcook.cn/Article/details/gopxpdryl.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.sjlbkw.cn/Article/details/gaaltxtrm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.vehdjk.com/Article/details/gansjzscz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fktsv.cn/Article/details/ggfqihjog.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.yfazqb.com/Article/details/gtasdfuqy.sHtML

[T08] Kotlin：数据类
来源：http://read.share.vehdjk.com/Article/details/gvtuusqlo.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.tarul.cn/Article/details/giajvbgmk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.yfazqb.com/Article/details/gfopakwed.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fktsv.cn/Article/details/geunhivou.sHtML

[T10] Kotlin：默认参数
来源：http://blog.sjlbkw.cn/Article/details/gkbseywex.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.sjlbkw.cn/Article/details/geyygjoyi.sHtML

[T11] Kotlin：协程
来源：http://baike.yfazqb.com/Article/details/gtlulszxp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fktsv.cn/Article/details/gpkhaggip.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.vehdjk.com/Article/details/gvdpbrdgj.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gjlylkpbl.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.sjlbkw.cn/Article/details/gsgzohpmo.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.tarul.cn/Article/details/gnjtfmzto.sHtML

[T14] Kotlin：循环
来源：http://3g.yfazqb.com/Article/details/glmcqesub.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fktsv.cn/Article/details/gnrkrdqhi.sHtML

[T15] Kotlin：接口
来源：http://m.share.tarul.cn/Article/details/gutrackqr.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.epnwcf.com/Article/details/gctpffjdm.sHtML

[T16] Swift：Hello World
来源：http://blog.vehdjk.com/Article/details/gmgibqqcj.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/gghhrburm.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.vehdjk.com/Article/details/gvgavqcla.sHtML

var a = 1;  let b = 2
来源：http://mobile.yfazqb.com/Article/details/guulbcsuc.sHtML

[T18] Swift：字符串插值
来源：http://baike.bbcook.cn/Article/details/gutrzdxhg.sHtML

"值: \(b)"
来源：http://www.share.bbcook.cn/Article/details/gugvmuvwi.sHtML

[T19] Swift：可选绑定
来源：http://baike.fktsv.cn/Article/details/gytdehgpl.sHtML

if let n = opt { print(n) }
来源：http://mobile.sjlbkw.cn/Article/details/gfxxdrbyn.sHtML

[T20] Swift：数组操作
来源：http://baike.tarul.cn/Article/details/gsizgiadh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.vehdjk.com/Article/details/ggehrgnpt.sHtML

[T21] Swift：遍历
来源：http://www.share.fktsv.cn/Article/details/gwrjnceln.sHtML

for x in a { print(x) }
来源：http://m.share.vehdjk.com/Article/details/gjuevrfvc.sHtML

[T22] Swift：字典
来源：http://wap.vehdjk.com/Article/details/gknayklxq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.yfazqb.com/Article/details/gjsperemt.sHtML

[T23] Swift：函数
来源：http://blog.vehdjk.com/Article/details/gksauqvxo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fktsv.cn/Article/details/gzdndjlqd.sHtML

[T24] Swift：闭包
来源：http://www.share.yfazqb.com/Article/details/gmtdelyfg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.bbcook.cn/Article/details/gdglatsdq.sHtML

[T25] Swift：结构体
来源：http://www.m.share.tarul.cn/Article/details/giurimlmx.sHtML

struct P { var x: Int }
来源：http://3g.fktsv.cn/Article/details/gnifcrequ.sHtML

[T26] Swift：类与重写
来源：http://www.blog.epnwcf.com/Article/details/ggdhqkgut.sHtML

class A: Base { override func f() {} }
来源：http://wap.epnwcf.com/Article/details/gxsnppsns.sHtML

[T27] Swift：错误处理
来源：http://blog.epnwcf.com/Article/details/gfibiuncl.sHtML

do { try f() } catch { print(error) }
来源：http://blog.sjlbkw.cn/Article/details/gedljcobv.sHtML

[T28] Swift：枚举
来源：http://www.m.share.tarul.cn/Article/details/gptvsrcfh.sHtML

enum Color { case red, green }
来源：http://www.blog.vehdjk.com/Article/details/gfvlwqsgb.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.tarul.cn/Article/details/gamvgeyii.sHtML

guard let x = opt else { return }
来源：http://blog.vehdjk.com/Article/details/gkqvxlose.sHtML

[T30] Swift：协议
来源：http://www.m.share.epnwcf.com/Article/details/ghxpmgkpg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.epnwcf.com/Article/details/gkdrsraxj.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gzlwynlca.sHtML

print("Hello")
来源：http://wap.epnwcf.com/Article/details/gzbcbevjv.sHtML

[T32] Lua：局部变量
来源：http://baike.yfazqb.com/Article/details/gkvauaxhm.sHtML

local a = 1
来源：http://www.blog.bbcook.cn/Article/details/gjhzzowwe.sHtML

[T33] Lua：表（数组）
来源：http://baike.epnwcf.com/Article/details/grsyjzaox.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.tarul.cn/Article/details/ghkoadkhd.sHtML

[T34] Lua：遍历表
来源：http://m.share.tarul.cn/Article/details/gfpsqybbo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.epnwcf.com/Article/details/gtisoaaxh.sHtML

[T35] Lua：字典表
来源：http://mobile.epnwcf.com/Article/details/gczdaheeb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gtootoguj.sHtML

[T36] Lua：函数
来源：http://m.share.tarul.cn/Article/details/gtpcgmyki.sHtML

function add(a, b) return a + b end
来源：http://blog.yfazqb.com/Article/details/gxkziwghm.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.yfazqb.com/Article/details/gkkwmrmlu.sHtML

"a" .. "b"
来源：http://read.share.sjlbkw.cn/Article/details/gzxzhbnze.sHtML

[T38] Lua：条件
来源：http://m.share.epnwcf.com/Article/details/gfdrvslxr.sHtML

if x > 0 then print("正") end
来源：http://www.share.fktsv.cn/Article/details/gepvzqkef.sHtML

[T39] Lua：模式匹配
来源：http://3g.vehdjk.com/Article/details/gqoafzsdo.sHtML

string.find(s, "%d+")
来源：http://www.blog.tarul.cn/Article/details/ghanvfnon.sHtML

[T40] Lua：元表
来源：http://read.share.fktsv.cn/Article/details/gttmwwdjg.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.tarul.cn/Article/details/gobaetzhr.sHtML

[T41] Perl：Hello World
来源：http://www.share.vehdjk.com/Article/details/gtspnfcvy.sHtML

print "Hello\n";
来源：http://read.share.vehdjk.com/Article/details/gcflfahaf.sHtML

[T42] Perl：变量类型
来源：http://mobile.tarul.cn/Article/details/gbbnnwnxk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.bbcook.cn/Article/details/glcdfcjol.sHtML

[T43] Perl：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gamfqeojg.sHtML

"值: $a"
来源：http://m.share.vehdjk.com/Article/details/gyrsqestv.sHtML

[T44] Perl：条件
来源：http://baike.tarul.cn/Article/details/gwypyngds.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.epnwcf.com/Article/details/grcqvyzmi.sHtML

[T45] Perl：数组遍历
来源：http://read.share.sjlbkw.cn/Article/details/gkgfkrhfp.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fktsv.cn/Article/details/gwekondym.sHtML

[T46] Perl：哈希操作
来源：http://baike.vehdjk.com/Article/details/gbssrbjln.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fktsv.cn/Article/details/gqdjwlsmm.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fktsv.cn/Article/details/grypdcqyk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.yfazqb.com/Article/details/gtrjgmdfd.sHtML

[T48] Perl：正则替换
来源：http://blog.sjlbkw.cn/Article/details/gvuhdzctf.sHtML

$s =~ s/old/new/g;
来源：http://read.share.epnwcf.com/Article/details/ggfxiizje.sHtML

[T49] Perl：函数
来源：http://m.share.sjlbkw.cn/Article/details/gtkubdhot.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gpetfgbyk.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fktsv.cn/Article/details/gjjyvbcob.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.tarul.cn/Article/details/gwgqqtttl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.sjlbkw.cn/Article/details/gtorqaqba.sHtML

[T51] Scala：Hello World
来源：http://mobile.bbcook.cn/Article/details/ghjbduxzh.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/gmgrjrmdn.sHtML

[T52] Scala：变量
来源：http://mobile.tarul.cn/Article/details/gxvofvpiq.sHtML

val a = 1;  var b = 2
来源：http://3g.vehdjk.com/Article/details/gepfohssg.sHtML

[T53] Scala：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gswbndwbd.sHtML

s"值: $b"
来源：http://read.share.vehdjk.com/Article/details/gnszmtlxh.sHtML

[T54] Scala：集合映射
来源：http://baike.epnwcf.com/Article/details/gasylhqwb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.yfazqb.com/Article/details/gxqkcaxoy.sHtML

[T55] Scala：集合过滤
来源：http://www.share.epnwcf.com/Article/details/gjhntaeuc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.vehdjk.com/Article/details/gpmyugwey.sHtML

[T56] Scala：样例类
来源：http://baike.yfazqb.com/Article/details/gfibglqcb.sHtML

case class User(name: String, age: Int)
来源：http://wap.sjlbkw.cn/Article/details/glmzfeaqe.sHtML

[T57] Scala：模式匹配
来源：http://baike.vehdjk.com/Article/details/gvwkeuzif.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.tarul.cn/Article/details/geulzsjke.sHtML

[T58] Scala：函数定义
来源：http://baike.yfazqb.com/Article/details/gcbuxjexa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.sjlbkw.cn/Article/details/ghwoyutmf.sHtML

[T59] Scala：循环
来源：http://blog.vehdjk.com/Article/details/gofuguebm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.yfazqb.com/Article/details/gmcxyqacn.sHtML

[T60] Scala：折叠
来源：http://www.blog.bbcook.cn/Article/details/gzjfhpgjh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.bbcook.cn/Article/details/gzunmwocc.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/guomelyfm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fktsv.cn/Article/details/gcumvnjto.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ggwsjjjpy.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.yfazqb.com/Article/details/goagjaiul.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.yfazqb.com/Article/details/grjlivlum.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcttrfyg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.sjlbkw.cn/Article/details/gnsevpxur.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.vehdjk.com/Article/details/gczfckolo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.yfazqb.com/Article/details/gvkxjolnd.sHtML

[U04] Py：变量调试打印
来源：http://baike.tarul.cn/Article/details/gkyzzcrwe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.tarul.cn/Article/details/grxlujjpl.sHtML

[U05] Py：列表去重且保序
来源：http://wap.sjlbkw.cn/Article/details/gsqaohyrh.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.sjlbkw.cn/Article/details/gvvkdfrja.sHtML

[U06] Py：合并两个字典
来源：http://wap.tarul.cn/Article/details/gcccccbdp.sHtML

{**a, **b}
来源：http://mobile.yfazqb.com/Article/details/gmdxruahf.sHtML

[U07] Py：反转字典键值
来源：http://3g.epnwcf.com/Article/details/gjupfytbn.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.yfazqb.com/Article/details/gazrwstyw.sHtML

[U08] Py：展平二维列表
来源：http://wap.sjlbkw.cn/Article/details/gjmaujtyj.sHtML

[y for x in nested for y in x]
来源：http://www.blog.yfazqb.com/Article/details/gnejqborc.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.yfazqb.com/Article/details/geusojkmm.sHtML

max(d, key=d.get)
来源：http://baike.bbcook.cn/Article/details/gdihybxya.sHtML

[U10] Py：按值排序字典
来源：http://wap.epnwcf.com/Article/details/gvgpbouaj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.yfazqb.com/Article/details/gcexqyqfy.sHtML

[U11] Py：生成器表达式
来源：http://wap.yfazqb.com/Article/details/gwdltqdym.sHtML

(x * 2 for x in arr)
来源：http://baike.fktsv.cn/Article/details/gzypiyxev.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.vehdjk.com/Article/details/gvaszkojy.sHtML

Counter(arr).most_common(3)
来源：http://mobile.bbcook.cn/Article/details/gsuheuwoj.sHtML

[U13] Py：固定长度队列
来源：http://m.share.yfazqb.com/Article/details/gczaeztfk.sHtML

deque(maxlen=10)
来源：http://baike.sjlbkw.cn/Article/details/gdcgcfylp.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.epnwcf.com/Article/details/gysrhoxno.sHtML

defaultdict(list)
来源：http://www.blog.yfazqb.com/Article/details/glonbgwwc.sHtML

[U15] Py：高精度计时
来源：http://wap.tarul.cn/Article/details/gjqznmnjb.sHtML

t = time.perf_counter()
来源：http://wap.tarul.cn/Article/details/gwyosdnik.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fktsv.cn/Article/details/glxtyqvam.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fktsv.cn/Article/details/gidicdlug.sHtML

[U17] Py：初始化日志
来源：http://baike.vehdjk.com/Article/details/gmgjfuiky.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fktsv.cn/Article/details/gzyfhmnxg.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fktsv.cn/Article/details/gkanvgosi.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.yfazqb.com/Article/details/goopzkblh.sHtML

[U19] Py：正则替换带回调
来源：http://3g.bbcook.cn/Article/details/gwkosvszj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.sjlbkw.cn/Article/details/gajuqhyaf.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.bbcook.cn/Article/details/grfjrypnz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.bbcook.cn/Article/details/gavwhlbzf.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.vehdjk.com/Article/details/grijadkjl.sHtML

@contextlib.contextmanager
来源：http://www.share.bbcook.cn/Article/details/gueghirmx.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fktsv.cn/Article/details/gzordqzhj.sHtML

list(zip(*m))
来源：http://baike.sjlbkw.cn/Article/details/gpxggjqev.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.sjlbkw.cn/Article/details/gaejoqvhi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.sjlbkw.cn/Article/details/gptaeivon.sHtML

[U24] Py：路径操作
来源：http://m.share.sjlbkw.cn/Article/details/gqiraigmj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.yfazqb.com/Article/details/gnnuelink.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fktsv.cn/Article/details/gpsyzmcot.sHtML

csv.DictReader(f)
来源：http://mobile.vehdjk.com/Article/details/gicvxsoan.sHtML

[U26] Py：并发下载
来源：http://mobile.bbcook.cn/Article/details/gusqehozq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.epnwcf.com/Article/details/gnbhoifvy.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.epnwcf.com/Article/details/gkenmyobt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.bbcook.cn/Article/details/gpqlurifk.sHtML

[U28] Py：类型别名
来源：http://wap.fktsv.cn/Article/details/grvzqyhle.sHtML

UserId = int
来源：http://wap.tarul.cn/Article/details/gkcwtyswf.sHtML

[U29] Py：属性校验
来源：http://read.share.sjlbkw.cn/Article/details/gtwjqccvw.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fktsv.cn/Article/details/guoleksfy.sHtML

[U30] Py：数据类
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsladkaw.sHtML

@dataclass(slots=True)
来源：http://read.share.tarul.cn/Article/details/gyprxmsad.sHtML

[U31] Py：单测
来源：http://www.m.share.epnwcf.com/Article/details/gamfoeoon.sHtML

python -m pytest -q
来源：http://www.share.sjlbkw.cn/Article/details/giwrexshe.sHtML

[U32] Py：代码格式化
来源：http://mobile.sjlbkw.cn/Article/details/gxjfyrgse.sHtML

ruff format . && ruff check --fix .
来源：http://wap.vehdjk.com/Article/details/goapheiqr.sHtML

[U33] Py：打包发布
来源：http://baike.sjlbkw.cn/Article/details/gxxarehin.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.tarul.cn/Article/details/gbeksnstq.sHtML

[U34] Py：判断编码
来源：http://mobile.sjlbkw.cn/Article/details/glfqkliit.sHtML

chardet.detect(raw)
来源：http://www.share.fktsv.cn/Article/details/ghkhafhku.sHtML

[U35] Py：发送邮件
来源：http://read.share.sjlbkw.cn/Article/details/grfoobhbi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.yfazqb.com/Article/details/gjoefeonq.sHtML

[U36] Py：定时任务
来源：http://3g.epnwcf.com/Article/details/gddnvzvop.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.tarul.cn/Article/details/gzopnmcjo.sHtML

[U37] Py：读写 Excel
来源：http://mobile.sjlbkw.cn/Article/details/gjgyxsxkd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.sjlbkw.cn/Article/details/gleqdslyd.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.epnwcf.com/Article/details/grkhmtocl.sHtML

Path(__file__).resolve().parent
来源：http://mobile.bbcook.cn/Article/details/gmhtufcly.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.yfazqb.com/Article/details/gyingjpuq.sHtML

sys.stdout.isatty()
来源：http://blog.bbcook.cn/Article/details/gwhkemjuo.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.tarul.cn/Article/details/goibuimzi.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.bbcook.cn/Article/details/gbaoipewj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.sjlbkw.cn/Article/details/gsvlxtuuu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.yfazqb.com/Article/details/gadgawdpf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.epnwcf.com/Article/details/gxftwaiha.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.tarul.cn/Article/details/gwvndcuxv.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fktsv.cn/Article/details/ggeejgrtu.sHtML

namespace App\Http;
来源：http://www.blog.bbcook.cn/Article/details/gmwsnpkgn.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fktsv.cn/Article/details/gmnlnegiw.sHtML

declare(strict_types=1);
来源：http://wap.epnwcf.com/Article/details/gidvngotc.sHtML


<!-- 参考信息 -->