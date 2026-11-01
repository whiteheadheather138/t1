代发 wailian999

int main(int argc, char **argv)
来源：http://wap.fktsv.cn/Article/details/gckrpkbts.sHtML

[S19] C：快速排序
来源：http://www.share.epnwcf.com/Article/details/gfxnhigzc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gsgrptsfp.sHtML

[S20] C：二分查找
来源：http://read.share.bbcook.cn/Article/details/gjqexfgdp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/gwfzjflko.sHtML

[S21] C：字符类别判断
来源：http://3g.vehdjk.com/Article/details/gcrgrhvrv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.sjlbkw.cn/Article/details/grqphbncw.sHtML

[S22] C：字符串转数字
来源：http://baike.tarul.cn/Article/details/gnkxdxciu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.yfazqb.com/Article/details/gckhxyulv.sHtML

[S23] C：随机数
来源：http://blog.sjlbkw.cn/Article/details/gryyvkvva.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.vehdjk.com/Article/details/gqtkndrlx.sHtML

[S24] C：获取本地时间
来源：http://www.blog.sjlbkw.cn/Article/details/gflwfzhpn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.tarul.cn/Article/details/glmebsdcs.sHtML

[S25] C：内存拷贝
来源：http://m.share.yfazqb.com/Article/details/gknpqdbvw.sHtML

memcpy(dst, src, n);
来源：http://m.share.tarul.cn/Article/details/gqxkotxtq.sHtML

[S26] C：内存清零
来源：http://blog.yfazqb.com/Article/details/grhvpyfyq.sHtML

memset(a, 0, sizeof a);
来源：http://baike.vehdjk.com/Article/details/gaunnfexv.sHtML

[S27] C：定义常量
来源：http://baike.bbcook.cn/Article/details/glhfviiht.sHtML

const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/giztfbkrp.sHtML

[S28] C：静态变量
来源：http://mobile.sjlbkw.cn/Article/details/gtvnqyhwn.sHtML

static int counter = 0;
来源：http://www.blog.sjlbkw.cn/Article/details/gvvbvcgei.sHtML

[S29] C：变参函数
来源：http://m.share.vehdjk.com/Article/details/guaafskea.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.sjlbkw.cn/Article/details/golvgjduy.sHtML

[S30] C：头文件保护
来源：http://wap.bbcook.cn/Article/details/gfwsiszpd.sHtML

#ifndef X_H
来源：http://www.m.share.fktsv.cn/Article/details/gdvubqjvy.sHtML

#define X_H
来源：http://www.share.yfazqb.com/Article/details/guxstukjw.sHtML

#endif
来源：http://www.m.share.bbcook.cn/Article/details/gqwjimimp.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/ggwmtezst.sHtML

#include <iostream>
来源：http://baike.vehdjk.com/Article/details/gdqngdhhr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.vehdjk.com/Article/details/gdjhuqcbx.sHtML

[S32] C++：字符串
来源：http://read.share.vehdjk.com/Article/details/gckvhyvlk.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.sjlbkw.cn/Article/details/gwgyeyyeq.sHtML

[S33] C++：vector 增删
来源：http://m.share.sjlbkw.cn/Article/details/gxwglffwn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.vehdjk.com/Article/details/gwohqbtix.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fktsv.cn/Article/details/garfjoxkn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.yfazqb.com/Article/details/glafarynw.sHtML

[S35] C++：map
来源：http://mobile.bbcook.cn/Article/details/goxifgncv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gkduhpdji.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fktsv.cn/Article/details/grloqrewe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gpcpffylr.sHtML

[S37] C++：set
来源：http://www.m.share.sjlbkw.cn/Article/details/gajylwlyq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.vehdjk.com/Article/details/gdulyyimg.sHtML

[S38] C++：排序
来源：http://read.share.sjlbkw.cn/Article/details/ggpoizcif.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.vehdjk.com/Article/details/gxublvqkh.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.sjlbkw.cn/Article/details/gnhncjchp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.tarul.cn/Article/details/gteoiudym.sHtML

[S40] C++：查找元素
来源：http://mobile.epnwcf.com/Article/details/gpegksqcn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.epnwcf.com/Article/details/gupbyqlfg.sHtML

[S41] C++：类与构造函数
来源：http://baike.fktsv.cn/Article/details/gmozxqdsu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.epnwcf.com/Article/details/gfwvfprpj.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.yfazqb.com/Article/details/gttxxcbkj.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fktsv.cn/Article/details/gnglykpek.sHtML

[S43] C++：智能指针
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfbxdnnu.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fktsv.cn/Article/details/gjskkwkox.sHtML

[S44] C++：引用传参
来源：http://www.blog.vehdjk.com/Article/details/gcttecidt.sHtML

void inc(int &x) { ++x; }
来源：http://wap.bbcook.cn/Article/details/guqmzzgpu.sHtML

[S45] C++：lambda
来源：http://read.share.yfazqb.com/Article/details/gtzohaivn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.tarul.cn/Article/details/gatwixjda.sHtML

[S46] C++：函数模板
来源：http://3g.tarul.cn/Article/details/gxyuqpdaq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.epnwcf.com/Article/details/gupnjsulu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fktsv.cn/Article/details/gdhxnckap.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.sjlbkw.cn/Article/details/grpulhlyl.sHtML

[S48] C++：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gzgyeltiy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.yfazqb.com/Article/details/gdqgnzrpm.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.vehdjk.com/Article/details/gwgjmuiqr.sHtML

[S49] C++：写文件
来源：http://baike.bbcook.cn/Article/details/gscmtuafr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.sjlbkw.cn/Article/details/gjauyigsd.sHtML

[S50] C++：格式化数字
来源：http://www.blog.yfazqb.com/Article/details/gbeskxmbx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fktsv.cn/Article/details/ghjvnotkm.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.vehdjk.com/Article/details/gyxwukytt.sHtML

static_cast<double>(a) / b
来源：http://blog.epnwcf.com/Article/details/gldlqekmh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.tarul.cn/Article/details/gkyavriwx.sHtML

int size() const noexcept { return n_; }
来源：http://baike.epnwcf.com/Article/details/gugiclxte.sHtML

[S53] C++：移动语义
来源：http://blog.epnwcf.com/Article/details/glmegckfq.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.yfazqb.com/Article/details/gqikuujtd.sHtML

[S54] C++：异常处理
来源：http://read.share.epnwcf.com/Article/details/gjdmslfyu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fktsv.cn/Article/details/gtlggaecc.sHtML

[S55] C++：结构化绑定
来源：http://3g.epnwcf.com/Article/details/gweqcuvsn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.epnwcf.com/Article/details/gowdcryny.sHtML

[S56] C++：optional
来源：http://baike.vehdjk.com/Article/details/gwcutpmnu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.tarul.cn/Article/details/gxbvxuman.sHtML

[S57] C++：编译期常量
来源：http://www.blog.yfazqb.com/Article/details/gtxyxwabi.sHtML

constexpr int N = 10;
来源：http://read.share.yfazqb.com/Article/details/gejmmcbtq.sHtML

[S58] C++：命名空间
来源：http://read.share.tarul.cn/Article/details/gkdzrifsz.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.sjlbkw.cn/Article/details/gensxffhf.sHtML

[S59] C++：静态断言
来源：http://baike.yfazqb.com/Article/details/gynbjmfrn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fktsv.cn/Article/details/gzqjvujoh.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.bbcook.cn/Article/details/gktujhrjs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.epnwcf.com/Article/details/gsommmwqf.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gwuhiikpo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.bbcook.cn/Article/details/gprqqunfq.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gpejqjcnw.sHtML

[T01] Kotlin：Hello World
来源：http://3g.bbcook.cn/Article/details/gtbvviplu.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/gohgmnkax.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.yfazqb.com/Article/details/gdrnrcijb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.vehdjk.com/Article/details/gpjviktdr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.vehdjk.com/Article/details/gypydlatm.sHtML

"值: $b"
来源：http://mobile.bbcook.cn/Article/details/gmshizzkg.sHtML

[T04] Kotlin：空安全
来源：http://read.share.sjlbkw.cn/Article/details/geodvnzqb.sHtML

val n: String? = null;  n?.length
来源：http://wap.sjlbkw.cn/Article/details/gbgpmdsmf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.bbcook.cn/Article/details/ghaabixel.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.yfazqb.com/Article/details/gjolshmyl.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.vehdjk.com/Article/details/godnlayef.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gtpgdaxwr.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.sjlbkw.cn/Article/details/gadlkhckn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.bbcook.cn/Article/details/gkiryadyg.sHtML

[T08] Kotlin：数据类
来源：http://read.share.bbcook.cn/Article/details/ggrwmccqo.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fktsv.cn/Article/details/gufgrizaz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.bbcook.cn/Article/details/gvrknmktd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.vehdjk.com/Article/details/gfuhntiqt.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.yfazqb.com/Article/details/gudfsomce.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.vehdjk.com/Article/details/guxxlzfxd.sHtML

[T11] Kotlin：协程
来源：http://wap.sjlbkw.cn/Article/details/gcyylwibf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.tarul.cn/Article/details/gogiwwmzg.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.sjlbkw.cn/Article/details/gqehqlzyu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gfbuquxmh.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.vehdjk.com/Article/details/gexkuslsc.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.tarul.cn/Article/details/gzmmajzsr.sHtML

[T14] Kotlin：循环
来源：http://baike.vehdjk.com/Article/details/gdftfenrr.sHtML

for (i in 1..10) println(i)
来源：http://www.share.bbcook.cn/Article/details/gangjecca.sHtML

[T15] Kotlin：接口
来源：http://www.share.yfazqb.com/Article/details/gkgetqpwk.sHtML

interface Shape { fun area(): Double }
来源：http://wap.yfazqb.com/Article/details/gvycksnax.sHtML

[T16] Swift：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gkuauahza.sHtML

print("Hello")
来源：http://mobile.yfazqb.com/Article/details/gxufxhzqo.sHtML

[T17] Swift：变量与常量
来源：http://baike.tarul.cn/Article/details/gxzbysrez.sHtML

var a = 1;  let b = 2
来源：http://baike.vehdjk.com/Article/details/gnxgywqzf.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gkhskayvd.sHtML

"值: \(b)"
来源：http://3g.tarul.cn/Article/details/gjedvrwhq.sHtML

[T19] Swift：可选绑定
来源：http://blog.vehdjk.com/Article/details/gsnkvljnu.sHtML

if let n = opt { print(n) }
来源：http://www.share.tarul.cn/Article/details/gpodtrkky.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.tarul.cn/Article/details/gotnrypko.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.sjlbkw.cn/Article/details/goviwzzlk.sHtML

[T21] Swift：遍历
来源：http://www.share.bbcook.cn/Article/details/gnudurohg.sHtML

for x in a { print(x) }
来源：http://mobile.bbcook.cn/Article/details/gmapbrbfb.sHtML

[T22] Swift：字典
来源：http://3g.tarul.cn/Article/details/giunfrmgl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.vehdjk.com/Article/details/grzhsuyws.sHtML

[T23] Swift：函数
来源：http://wap.yfazqb.com/Article/details/grkzsjmua.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.vehdjk.com/Article/details/gdkeievof.sHtML

[T24] Swift：闭包
来源：http://read.share.tarul.cn/Article/details/ghucqzjpl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.epnwcf.com/Article/details/gglqrdddd.sHtML

[T25] Swift：结构体
来源：http://blog.sjlbkw.cn/Article/details/gsjwjaenj.sHtML

struct P { var x: Int }
来源：http://m.share.sjlbkw.cn/Article/details/ggqpfehxw.sHtML

[T26] Swift：类与重写
来源：http://3g.vehdjk.com/Article/details/gqocopvce.sHtML

class A: Base { override func f() {} }
来源：http://baike.epnwcf.com/Article/details/gauoarcoo.sHtML

[T27] Swift：错误处理
来源：http://blog.tarul.cn/Article/details/gcadrgrms.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.tarul.cn/Article/details/gzobgicgx.sHtML

[T28] Swift：枚举
来源：http://m.share.bbcook.cn/Article/details/gmhxgwcez.sHtML

enum Color { case red, green }
来源：http://www.blog.yfazqb.com/Article/details/gekjskmkq.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.epnwcf.com/Article/details/gcipnsrpy.sHtML

guard let x = opt else { return }
来源：http://m.share.vehdjk.com/Article/details/gpfylgicj.sHtML

[T30] Swift：协议
来源：http://www.share.bbcook.cn/Article/details/gtlmiswpo.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.epnwcf.com/Article/details/gnvewqzqu.sHtML

[T31] Lua：Hello World
来源：http://3g.tarul.cn/Article/details/grdvqranv.sHtML

print("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gtipjgsth.sHtML

[T32] Lua：局部变量
来源：http://mobile.epnwcf.com/Article/details/gpsdelxoq.sHtML

local a = 1
来源：http://read.share.yfazqb.com/Article/details/gxqowpbij.sHtML

[T33] Lua：表（数组）
来源：http://3g.sjlbkw.cn/Article/details/gjhhfagaq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.vehdjk.com/Article/details/gsfytclht.sHtML

[T34] Lua：遍历表
来源：http://read.share.epnwcf.com/Article/details/gyzaveeib.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fktsv.cn/Article/details/gtfefecds.sHtML

[T35] Lua：字典表
来源：http://3g.bbcook.cn/Article/details/gkmjhqqxk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.bbcook.cn/Article/details/gbroxsrea.sHtML

[T36] Lua：函数
来源：http://blog.yfazqb.com/Article/details/gjznjzeat.sHtML

function add(a, b) return a + b end
来源：http://read.share.fktsv.cn/Article/details/gxioiezyg.sHtML

[T37] Lua：字符串拼接
来源：http://wap.epnwcf.com/Article/details/gvumznpvg.sHtML

"a" .. "b"
来源：http://www.share.tarul.cn/Article/details/gipnvvwzw.sHtML

[T38] Lua：条件
来源：http://read.share.yfazqb.com/Article/details/gohrczidh.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fktsv.cn/Article/details/ggkaczdpa.sHtML

[T39] Lua：模式匹配
来源：http://m.share.epnwcf.com/Article/details/gncfppuza.sHtML

string.find(s, "%d+")
来源：http://baike.sjlbkw.cn/Article/details/gogyxxjwr.sHtML

[T40] Lua：元表
来源：http://3g.sjlbkw.cn/Article/details/gabctfxmf.sHtML

setmetatable({}, { __index = base })
来源：http://baike.yfazqb.com/Article/details/gdgkbzgbx.sHtML

[T41] Perl：Hello World
来源：http://baike.vehdjk.com/Article/details/gmmnwxtnb.sHtML

print "Hello\n";
来源：http://www.blog.tarul.cn/Article/details/ghkhaggyq.sHtML

[T42] Perl：变量类型
来源：http://3g.vehdjk.com/Article/details/gnfmsenzd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.vehdjk.com/Article/details/gvtosmlji.sHtML

[T43] Perl：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gaqpjgppk.sHtML

"值: $a"
来源：http://www.m.share.fktsv.cn/Article/details/gvvlhgwhe.sHtML

[T44] Perl：条件
来源：http://blog.epnwcf.com/Article/details/gjuhiahqm.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdblfcto.sHtML

[T45] Perl：数组遍历
来源：http://baike.vehdjk.com/Article/details/gsmzsxqbo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.vehdjk.com/Article/details/gggdwbhsl.sHtML

[T46] Perl：哈希操作
来源：http://read.share.tarul.cn/Article/details/gqkdydhsc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.yfazqb.com/Article/details/gzlrdfsrf.sHtML

[T47] Perl：正则捕获
来源：http://mobile.yfazqb.com/Article/details/gxbjoiqpi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.yfazqb.com/Article/details/gesejlcwy.sHtML

[T48] Perl：正则替换
来源：http://m.share.fktsv.cn/Article/details/gkdzmpnxn.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fktsv.cn/Article/details/gzeitqbxq.sHtML

[T49] Perl：函数
来源：http://blog.fktsv.cn/Article/details/gwxnhzjkq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gtevitbys.sHtML

[T50] Perl：逐行读文件
来源：http://baike.bbcook.cn/Article/details/geqywldlu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.tarul.cn/Article/details/gqhunstkm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.vehdjk.com/Article/details/gvccaalzn.sHtML

[T51] Scala：Hello World
来源：http://3g.vehdjk.com/Article/details/gasudedbe.sHtML

println("Hello")
来源：http://www.share.tarul.cn/Article/details/gczplfrck.sHtML

[T52] Scala：变量
来源：http://blog.vehdjk.com/Article/details/gfvykposx.sHtML

val a = 1;  var b = 2
来源：http://baike.fktsv.cn/Article/details/gzrbflyvv.sHtML

[T53] Scala：字符串插值
来源：http://baike.fktsv.cn/Article/details/ggjatvdoh.sHtML

s"值: $b"
来源：http://m.share.yfazqb.com/Article/details/gdwauqwoh.sHtML

[T54] Scala：集合映射
来源：http://baike.epnwcf.com/Article/details/gchcexbme.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.sjlbkw.cn/Article/details/ghpnfkfag.sHtML

[T55] Scala：集合过滤
来源：http://m.share.epnwcf.com/Article/details/gejymxwdm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.vehdjk.com/Article/details/gsiuixhia.sHtML

[T56] Scala：样例类
来源：http://m.share.epnwcf.com/Article/details/gwxtqbxjs.sHtML

case class User(name: String, age: Int)
来源：http://mobile.yfazqb.com/Article/details/gnirqwibe.sHtML

[T57] Scala：模式匹配
来源：http://m.share.tarul.cn/Article/details/gcthaagxl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.tarul.cn/Article/details/ggkbxsdit.sHtML

[T58] Scala：函数定义
来源：http://wap.bbcook.cn/Article/details/grmhtojwc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.sjlbkw.cn/Article/details/gjyjorukl.sHtML

[T59] Scala：循环
来源：http://www.blog.bbcook.cn/Article/details/gkudslrgd.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.tarul.cn/Article/details/goaxebcxw.sHtML

[T60] Scala：折叠
来源：http://www.share.sjlbkw.cn/Article/details/gmwjgautl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.sjlbkw.cn/Article/details/gqjjzcomy.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gacxfisbv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.vehdjk.com/Article/details/ghrkuskgm.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gowvzogso.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.epnwcf.com/Article/details/ggzrgdkqv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.sjlbkw.cn/Article/details/gmohfdvcb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.bbcook.cn/Article/details/ggtofgmqa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.sjlbkw.cn/Article/details/gapafwkub.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.yfazqb.com/Article/details/gvidfwajf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.bbcook.cn/Article/details/gdaksvwwu.sHtML

[U04] Py：变量调试打印
来源：http://www.share.bbcook.cn/Article/details/gkbswtwnk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.sjlbkw.cn/Article/details/gnidwjwal.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.epnwcf.com/Article/details/gtodlgutf.sHtML

list(dict.fromkeys(arr))
来源：http://wap.yfazqb.com/Article/details/gfucywnnq.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fktsv.cn/Article/details/ggdopjhqv.sHtML

{**a, **b}
来源：http://baike.vehdjk.com/Article/details/gclnqpncm.sHtML

[U07] Py：反转字典键值
来源：http://baike.vehdjk.com/Article/details/grjyoqqqr.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fktsv.cn/Article/details/ggcyyuaht.sHtML

[U08] Py：展平二维列表
来源：http://mobile.sjlbkw.cn/Article/details/gnpmlrecp.sHtML

[y for x in nested for y in x]
来源：http://m.share.fktsv.cn/Article/details/gxxutvwtg.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.bbcook.cn/Article/details/gnspaioze.sHtML

max(d, key=d.get)
来源：http://m.share.epnwcf.com/Article/details/gtgsmrykr.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.tarul.cn/Article/details/gzddhamvi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.yfazqb.com/Article/details/gfaavsaro.sHtML

[U11] Py：生成器表达式
来源：http://read.share.epnwcf.com/Article/details/gpoxctrlz.sHtML

(x * 2 for x in arr)
来源：http://www.blog.epnwcf.com/Article/details/gzirgzbbv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.bbcook.cn/Article/details/gxotgzklw.sHtML

Counter(arr).most_common(3)
来源：http://m.share.sjlbkw.cn/Article/details/gpdjaozym.sHtML

[U13] Py：固定长度队列
来源：http://www.share.yfazqb.com/Article/details/ghbdjnymp.sHtML

deque(maxlen=10)
来源：http://3g.epnwcf.com/Article/details/geueychyd.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.tarul.cn/Article/details/gepitwfix.sHtML

defaultdict(list)
来源：http://3g.vehdjk.com/Article/details/gygletuzl.sHtML

[U15] Py：高精度计时
来源：http://m.share.epnwcf.com/Article/details/gplvzfpat.sHtML

t = time.perf_counter()
来源：http://wap.fktsv.cn/Article/details/gjxntyqmg.sHtML

[U16] Py：命令行参数解析
来源：http://wap.vehdjk.com/Article/details/ghdhdqxpc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fktsv.cn/Article/details/gwksorinv.sHtML

[U17] Py：初始化日志
来源：http://3g.yfazqb.com/Article/details/grglhtcit.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.vehdjk.com/Article/details/gpkrzxmvn.sHtML

[U18] Py：预编译正则
来源：http://m.share.tarul.cn/Article/details/gvgobhmof.sHtML

pat = re.compile(r"\d+")
来源：http://blog.yfazqb.com/Article/details/gwlhjaifo.sHtML

[U19] Py：正则替换带回调
来源：http://wap.yfazqb.com/Article/details/gdcowpuzt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.vehdjk.com/Article/details/ghvfhvxdo.sHtML

[U20] Py：缓存函数结果
来源：http://blog.epnwcf.com/Article/details/gyceqfdsm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.tarul.cn/Article/details/gcpgklxze.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.bbcook.cn/Article/details/gepzwzoap.sHtML

@contextlib.contextmanager
来源：http://read.share.epnwcf.com/Article/details/gogifkfkz.sHtML

[U22] Py：矩阵转置
来源：http://read.share.epnwcf.com/Article/details/gdmsbzfnr.sHtML

list(zip(*m))
来源：http://read.share.epnwcf.com/Article/details/gtoxlaqvj.sHtML

[U23] Py：分块读取大文件
来源：http://3g.epnwcf.com/Article/details/gzpliwzpc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.yfazqb.com/Article/details/guujlfgmk.sHtML

[U24] Py：路径操作
来源：http://www.blog.bbcook.cn/Article/details/gemmwneml.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.bbcook.cn/Article/details/gdogrmona.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.tarul.cn/Article/details/gmhchmkkj.sHtML

csv.DictReader(f)
来源：http://www.share.yfazqb.com/Article/details/gcbszdlly.sHtML

[U26] Py：并发下载
来源：http://mobile.fktsv.cn/Article/details/gatlhdikw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.bbcook.cn/Article/details/gqulzxzed.sHtML

[U27] Py：异步 HTTP
来源：http://wap.sjlbkw.cn/Article/details/gmkmmerwe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.vehdjk.com/Article/details/gdmtzblon.sHtML

[U28] Py：类型别名
来源：http://read.share.yfazqb.com/Article/details/gmeukeqqp.sHtML

UserId = int
来源：http://wap.vehdjk.com/Article/details/gadmdxuif.sHtML

[U29] Py：属性校验
来源：http://read.share.fktsv.cn/Article/details/gpsuntfjp.sHtML

@property 与 @x.setter 配合
来源：http://blog.bbcook.cn/Article/details/gtuliwkxz.sHtML

[U30] Py：数据类
来源：http://wap.sjlbkw.cn/Article/details/gzecuuhry.sHtML

@dataclass(slots=True)
来源：http://mobile.bbcook.cn/Article/details/gwnwnucka.sHtML

[U31] Py：单测
来源：http://m.share.yfazqb.com/Article/details/ghljkqehz.sHtML

python -m pytest -q
来源：http://m.share.vehdjk.com/Article/details/gwuxhnwzr.sHtML

[U32] Py：代码格式化
来源：http://wap.sjlbkw.cn/Article/details/gwkdamaoo.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.bbcook.cn/Article/details/gtemfhmxi.sHtML

[U33] Py：打包发布
来源：http://mobile.epnwcf.com/Article/details/gazudqvpl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.vehdjk.com/Article/details/gjswkmhzp.sHtML

[U34] Py：判断编码
来源：http://blog.sjlbkw.cn/Article/details/grkpckung.sHtML

chardet.detect(raw)
来源：http://www.m.share.vehdjk.com/Article/details/gyvjezbpi.sHtML

[U35] Py：发送邮件
来源：http://m.share.fktsv.cn/Article/details/ggkcknaxf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fktsv.cn/Article/details/gfdosgdsh.sHtML

[U36] Py：定时任务
来源：http://m.share.yfazqb.com/Article/details/gonivomxz.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.bbcook.cn/Article/details/guerbqstl.sHtML

[U37] Py：读写 Excel
来源：http://3g.vehdjk.com/Article/details/gucsnxean.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fktsv.cn/Article/details/glhulvsfh.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.sjlbkw.cn/Article/details/gjudhdslm.sHtML

Path(__file__).resolve().parent
来源：http://baike.vehdjk.com/Article/details/gxlqfeiqu.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.yfazqb.com/Article/details/gqkfjedpl.sHtML

sys.stdout.isatty()
来源：http://www.share.bbcook.cn/Article/details/ggrtodzyj.sHtML

[U40] Py：打印到标准错误
来源：http://baike.bbcook.cn/Article/details/ghvhhxvar.sHtML

print("err", file=sys.stderr)
来源：http://baike.sjlbkw.cn/Article/details/gjxnxzptq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.bbcook.cn/Article/details/gaigdechp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fktsv.cn/Article/details/gdkrcuwrd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.epnwcf.com/Article/details/gosvkiriv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.yfazqb.com/Article/details/gbeduclvy.sHtML


<!-- 参考信息 -->