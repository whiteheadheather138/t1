代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/gjxvrbeua.sHtML

[S13] C：宏定义
来源：http://wap.sjlbkw.cn/Article/details/ghikisswt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.vehdjk.com/Article/details/gcfpcmihu.sHtML

[S14] C：枚举
来源：http://baike.bbcook.cn/Article/details/gkjfwtxsd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.tarul.cn/Article/details/gdkfetake.sHtML

[S15] C：类型转换
来源：http://mobile.vehdjk.com/Article/details/gptlsqlub.sHtML

(double) a / b
来源：http://read.share.bbcook.cn/Article/details/gqymswcpy.sHtML

[S16] C：位操作置位
来源：http://baike.vehdjk.com/Article/details/gbzrlfdvm.sHtML

x |= (1 << 3);
来源：http://www.share.sjlbkw.cn/Article/details/gelwwmdhp.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gugrvupuu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.yfazqb.com/Article/details/gkipuatcv.sHtML

[S18] C：命令行参数
来源：http://www.share.yfazqb.com/Article/details/ghekaskio.sHtML

int main(int argc, char **argv)
来源：http://m.share.fktsv.cn/Article/details/gqfcsmyvv.sHtML

[S19] C：快速排序
来源：http://www.blog.vehdjk.com/Article/details/ggimeybpi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gnqdcfesd.sHtML

[S20] C：二分查找
来源：http://blog.vehdjk.com/Article/details/ggubwtngb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/ghykubzrx.sHtML

[S21] C：字符类别判断
来源：http://read.share.vehdjk.com/Article/details/gybvxbqjq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.yfazqb.com/Article/details/gbbfdekej.sHtML

[S22] C：字符串转数字
来源：http://www.share.yfazqb.com/Article/details/gpxnxkhws.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.epnwcf.com/Article/details/gvfbsplax.sHtML

[S23] C：随机数
来源：http://baike.bbcook.cn/Article/details/gdzzicczi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fktsv.cn/Article/details/geqpfwptq.sHtML

[S24] C：获取本地时间
来源：http://3g.fktsv.cn/Article/details/glvhmyquz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fktsv.cn/Article/details/gcnwerfbi.sHtML

[S25] C：内存拷贝
来源：http://m.share.tarul.cn/Article/details/gweqpvxqu.sHtML

memcpy(dst, src, n);
来源：http://www.blog.sjlbkw.cn/Article/details/gsralcbtf.sHtML

[S26] C：内存清零
来源：http://www.share.fktsv.cn/Article/details/gzyyigpvq.sHtML

memset(a, 0, sizeof a);
来源：http://3g.vehdjk.com/Article/details/gxixjcibk.sHtML

[S27] C：定义常量
来源：http://mobile.bbcook.cn/Article/details/gsmjvehfv.sHtML

const double PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gaadjvppv.sHtML

[S28] C：静态变量
来源：http://wap.fktsv.cn/Article/details/gqvuszcti.sHtML

static int counter = 0;
来源：http://www.blog.fktsv.cn/Article/details/gcfcwisgv.sHtML

[S29] C：变参函数
来源：http://blog.fktsv.cn/Article/details/gozzllyge.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.yfazqb.com/Article/details/gxymgyari.sHtML

[S30] C：头文件保护
来源：http://mobile.tarul.cn/Article/details/gdioggfmj.sHtML

#ifndef X_H
来源：http://www.m.share.vehdjk.com/Article/details/guftutiwo.sHtML

#define X_H
来源：http://read.share.tarul.cn/Article/details/gsswskoxh.sHtML

#endif
来源：http://read.share.tarul.cn/Article/details/gnqnihhbn.sHtML

[S31] C++：Hello World
来源：http://m.share.tarul.cn/Article/details/gcjwkglko.sHtML

#include <iostream>
来源：http://www.share.vehdjk.com/Article/details/gaczltpgi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fktsv.cn/Article/details/gdlgiolyy.sHtML

[S32] C++：字符串
来源：http://read.share.epnwcf.com/Article/details/gmakxsfht.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.epnwcf.com/Article/details/gvkrpmofn.sHtML

[S33] C++：vector 增删
来源：http://blog.yfazqb.com/Article/details/gunmqufxv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.bbcook.cn/Article/details/gvbqsvjay.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.yfazqb.com/Article/details/gysizdlds.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.epnwcf.com/Article/details/geqbjkult.sHtML

[S35] C++：map
来源：http://mobile.bbcook.cn/Article/details/glbjucpif.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gletwkqrk.sHtML

[S36] C++：unordered_map
来源：http://m.share.fktsv.cn/Article/details/gtjarkbgh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/gabtaqsjy.sHtML

[S37] C++：set
来源：http://blog.vehdjk.com/Article/details/gekynchra.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fktsv.cn/Article/details/gmcejqzvn.sHtML

[S38] C++：排序
来源：http://baike.tarul.cn/Article/details/gqehzzmui.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.tarul.cn/Article/details/ghhnbeeel.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.tarul.cn/Article/details/gznjjpiqs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.yfazqb.com/Article/details/giihfdlum.sHtML

[S40] C++：查找元素
来源：http://www.blog.bbcook.cn/Article/details/gywwpxuvy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.vehdjk.com/Article/details/givbijjtv.sHtML

[S41] C++：类与构造函数
来源：http://blog.bbcook.cn/Article/details/gkbmqveve.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.bbcook.cn/Article/details/grfofbxgr.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.tarul.cn/Article/details/glgplouhy.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fktsv.cn/Article/details/gexpjriwi.sHtML

[S43] C++：智能指针
来源：http://www.share.bbcook.cn/Article/details/gbkhnptig.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.epnwcf.com/Article/details/gqzqtgbuj.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fktsv.cn/Article/details/gkvllvybc.sHtML

void inc(int &x) { ++x; }
来源：http://wap.epnwcf.com/Article/details/glypnrzhp.sHtML

[S45] C++：lambda
来源：http://mobile.bbcook.cn/Article/details/gfzemmxce.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fktsv.cn/Article/details/gcafjqtyr.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/gwxjaeykz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.epnwcf.com/Article/details/ghpwewncl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.bbcook.cn/Article/details/gulwxkwtb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.tarul.cn/Article/details/gxdwuufrs.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/giqmbvaln.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.yfazqb.com/Article/details/guatwcart.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpoapeypq.sHtML

[S49] C++：写文件
来源：http://m.share.tarul.cn/Article/details/gubnjqjws.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.tarul.cn/Article/details/guelajurg.sHtML

[S50] C++：格式化数字
来源：http://mobile.fktsv.cn/Article/details/gssvbskga.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gyhogilcy.sHtML

[S51] C++：显式类型转换
来源：http://read.share.sjlbkw.cn/Article/details/gasdexcmw.sHtML

static_cast<double>(a) / b
来源：http://wap.bbcook.cn/Article/details/gkrbttcsg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.epnwcf.com/Article/details/gwjjzwknq.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbpkasqgc.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fktsv.cn/Article/details/gwlbvnazh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.epnwcf.com/Article/details/gqfgnwtda.sHtML

[S54] C++：异常处理
来源：http://blog.tarul.cn/Article/details/gnhjsderp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fktsv.cn/Article/details/gvxbtvidd.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtcamzlp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gnzywbcvh.sHtML

[S56] C++：optional
来源：http://www.m.share.sjlbkw.cn/Article/details/gvyhoekxd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.yfazqb.com/Article/details/gvwlqtiaj.sHtML

[S57] C++：编译期常量
来源：http://wap.sjlbkw.cn/Article/details/ghytljqxn.sHtML

constexpr int N = 10;
来源：http://wap.vehdjk.com/Article/details/gpqbkxdeo.sHtML

[S58] C++：命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gvzdlucgf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyinxxzuf.sHtML

[S59] C++：静态断言
来源：http://mobile.fktsv.cn/Article/details/gunqxicsy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.tarul.cn/Article/details/gvwitkagp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.sjlbkw.cn/Article/details/gtklpcgpb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.bbcook.cn/Article/details/gghjnrlqm.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gfsodkcuq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.sjlbkw.cn/Article/details/gdpqdtasj.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/giemwagqm.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fktsv.cn/Article/details/gpgtndfyu.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gmylyidds.sHtML

[T02] Kotlin：变量
来源：http://blog.sjlbkw.cn/Article/details/gdzhufkpv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.tarul.cn/Article/details/ggdkrlfhl.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.vehdjk.com/Article/details/gkguvpjwb.sHtML

"值: $b"
来源：http://www.share.tarul.cn/Article/details/gcmliepra.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.vehdjk.com/Article/details/gywdngdfh.sHtML

val n: String? = null;  n?.length
来源：http://baike.yfazqb.com/Article/details/gdlrkccod.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gmjsolkvv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.yfazqb.com/Article/details/gzknoxkpa.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.tarul.cn/Article/details/gygvmdwut.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.tarul.cn/Article/details/grztrzrdl.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.tarul.cn/Article/details/giikrjrzz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.sjlbkw.cn/Article/details/gylwwkoje.sHtML

[T08] Kotlin：数据类
来源：http://wap.epnwcf.com/Article/details/gmvrtbcxk.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.epnwcf.com/Article/details/guulrogfr.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.vehdjk.com/Article/details/gnezlvuzc.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.yfazqb.com/Article/details/ghwbkurmj.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fktsv.cn/Article/details/gycvvwqky.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.tarul.cn/Article/details/gueqlkkdr.sHtML

[T11] Kotlin：协程
来源：http://wap.epnwcf.com/Article/details/gfhjpkfpn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.tarul.cn/Article/details/gmwwbvpqt.sHtML

[T12] Kotlin：解构声明
来源：http://wap.vehdjk.com/Article/details/gcjccycjy.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/gvegzjvyo.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.epnwcf.com/Article/details/gmgftzbyt.sHtML

val m = mapOf("a" to 1)
来源：http://3g.bbcook.cn/Article/details/gnvzirbaq.sHtML

[T14] Kotlin：循环
来源：http://3g.vehdjk.com/Article/details/gdaunncrk.sHtML

for (i in 1..10) println(i)
来源：http://3g.sjlbkw.cn/Article/details/ghwcdhddr.sHtML

[T15] Kotlin：接口
来源：http://wap.vehdjk.com/Article/details/grmewfccc.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.bbcook.cn/Article/details/gqgioqtky.sHtML

[T16] Swift：Hello World
来源：http://blog.tarul.cn/Article/details/gsvjinrjn.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/glrxwrbwd.sHtML

[T17] Swift：变量与常量
来源：http://blog.epnwcf.com/Article/details/gctmdrfpm.sHtML

var a = 1;  let b = 2
来源：http://m.share.vehdjk.com/Article/details/gtlshvpiv.sHtML

[T18] Swift：字符串插值
来源：http://wap.fktsv.cn/Article/details/gzmothuyt.sHtML

"值: \(b)"
来源：http://www.m.share.vehdjk.com/Article/details/gdjldlkip.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fktsv.cn/Article/details/gfhrjwadb.sHtML

if let n = opt { print(n) }
来源：http://mobile.epnwcf.com/Article/details/gnheraffj.sHtML

[T20] Swift：数组操作
来源：http://www.blog.tarul.cn/Article/details/gznehzfah.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.epnwcf.com/Article/details/gyhjvqiao.sHtML

[T21] Swift：遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gojexbwjr.sHtML

for x in a { print(x) }
来源：http://wap.yfazqb.com/Article/details/gwojqpywx.sHtML

[T22] Swift：字典
来源：http://baike.bbcook.cn/Article/details/gmxjvzgnm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.epnwcf.com/Article/details/gvjlychrt.sHtML

[T23] Swift：函数
来源：http://www.blog.tarul.cn/Article/details/gvgklcqfu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.yfazqb.com/Article/details/gbducvsvc.sHtML

[T24] Swift：闭包
来源：http://mobile.epnwcf.com/Article/details/gqhaqwzbt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.bbcook.cn/Article/details/ghxgmcwyd.sHtML

[T25] Swift：结构体
来源：http://mobile.sjlbkw.cn/Article/details/gwdvklprg.sHtML

struct P { var x: Int }
来源：http://mobile.yfazqb.com/Article/details/gznblqnsy.sHtML

[T26] Swift：类与重写
来源：http://mobile.epnwcf.com/Article/details/gdcqnehuf.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fktsv.cn/Article/details/gqyrpmbiv.sHtML

[T27] Swift：错误处理
来源：http://baike.tarul.cn/Article/details/gyktqrkgw.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.vehdjk.com/Article/details/gsorpgusp.sHtML

[T28] Swift：枚举
来源：http://3g.epnwcf.com/Article/details/gyfwrtwzi.sHtML

enum Color { case red, green }
来源：http://m.share.sjlbkw.cn/Article/details/giupqinbt.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.tarul.cn/Article/details/goxwnqzkp.sHtML

guard let x = opt else { return }
来源：http://m.share.bbcook.cn/Article/details/gpiwfzphm.sHtML

[T30] Swift：协议
来源：http://m.share.bbcook.cn/Article/details/gtqqwcqvp.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.epnwcf.com/Article/details/gqsrzgyme.sHtML

[T31] Lua：Hello World
来源：http://mobile.epnwcf.com/Article/details/gvrforufd.sHtML

print("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gxxgnzysk.sHtML

[T32] Lua：局部变量
来源：http://mobile.sjlbkw.cn/Article/details/gmkkmicib.sHtML

local a = 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gooqlgwdq.sHtML

[T33] Lua：表（数组）
来源：http://mobile.vehdjk.com/Article/details/gfkfecips.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.sjlbkw.cn/Article/details/gpyccncjk.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.sjlbkw.cn/Article/details/gxednnbsk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.bbcook.cn/Article/details/gzkhobjaw.sHtML

[T35] Lua：字典表
来源：http://m.share.vehdjk.com/Article/details/gpsyumswt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fktsv.cn/Article/details/gmzrytakv.sHtML

[T36] Lua：函数
来源：http://www.blog.fktsv.cn/Article/details/gkkfcokto.sHtML

function add(a, b) return a + b end
来源：http://3g.epnwcf.com/Article/details/ghbqgvqqt.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fktsv.cn/Article/details/gvkbciisc.sHtML

"a" .. "b"
来源：http://www.m.share.yfazqb.com/Article/details/gpaxgttgw.sHtML

[T38] Lua：条件
来源：http://3g.bbcook.cn/Article/details/ghrombfbr.sHtML

if x > 0 then print("正") end
来源：http://read.share.tarul.cn/Article/details/gbqjpppao.sHtML

[T39] Lua：模式匹配
来源：http://wap.yfazqb.com/Article/details/ggmhppygb.sHtML

string.find(s, "%d+")
来源：http://www.share.tarul.cn/Article/details/gkmfubpfk.sHtML

[T40] Lua：元表
来源：http://read.share.vehdjk.com/Article/details/gsmthwesn.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.yfazqb.com/Article/details/gwkzyhtac.sHtML

[T41] Perl：Hello World
来源：http://mobile.vehdjk.com/Article/details/gzdgkolmu.sHtML

print "Hello\n";
来源：http://www.blog.vehdjk.com/Article/details/gkjuftwkn.sHtML

[T42] Perl：变量类型
来源：http://read.share.bbcook.cn/Article/details/goqlurwwk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.sjlbkw.cn/Article/details/gudqktdqu.sHtML

[T43] Perl：字符串插值
来源：http://m.share.tarul.cn/Article/details/grkgrxpzi.sHtML

"值: $a"
来源：http://3g.epnwcf.com/Article/details/gursmbomx.sHtML

[T44] Perl：条件
来源：http://blog.vehdjk.com/Article/details/gwsqrfgfc.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.vehdjk.com/Article/details/gegklzelj.sHtML

[T45] Perl：数组遍历
来源：http://read.share.yfazqb.com/Article/details/gtiuvvwme.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.tarul.cn/Article/details/gfizlfcgf.sHtML

[T46] Perl：哈希操作
来源：http://m.share.sjlbkw.cn/Article/details/gmtennfvv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.bbcook.cn/Article/details/gmryfbpzh.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fktsv.cn/Article/details/gjspmadbp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.tarul.cn/Article/details/gsblcfvhg.sHtML

[T48] Perl：正则替换
来源：http://www.share.tarul.cn/Article/details/gkbudfmdb.sHtML

$s =~ s/old/new/g;
来源：http://read.share.tarul.cn/Article/details/gjporohyd.sHtML

[T49] Perl：函数
来源：http://www.blog.fktsv.cn/Article/details/gznyayvij.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gkdwtpnvi.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gbrlwutwk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fktsv.cn/Article/details/gkvfuxqhn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.tarul.cn/Article/details/gfnavtycd.sHtML

[T51] Scala：Hello World
来源：http://www.share.epnwcf.com/Article/details/gycpmehhp.sHtML

println("Hello")
来源：http://wap.fktsv.cn/Article/details/gmosuvnef.sHtML

[T52] Scala：变量
来源：http://mobile.tarul.cn/Article/details/gxozhaxrp.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fktsv.cn/Article/details/gdyjjlvmi.sHtML

[T53] Scala：字符串插值
来源：http://m.share.tarul.cn/Article/details/gbrcfglwu.sHtML

s"值: $b"
来源：http://wap.vehdjk.com/Article/details/gjmjkzzla.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fktsv.cn/Article/details/gsennhcom.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.bbcook.cn/Article/details/gjurufjbc.sHtML

[T55] Scala：集合过滤
来源：http://baike.yfazqb.com/Article/details/gvllyxean.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.vehdjk.com/Article/details/gzuaaxfuj.sHtML

[T56] Scala：样例类
来源：http://baike.bbcook.cn/Article/details/grqzfnexh.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fktsv.cn/Article/details/gznyuhjub.sHtML

[T57] Scala：模式匹配
来源：http://blog.fktsv.cn/Article/details/grcajcecx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.bbcook.cn/Article/details/giilczgpw.sHtML

[T58] Scala：函数定义
来源：http://baike.tarul.cn/Article/details/gpyarftmp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.sjlbkw.cn/Article/details/gkvuuwucn.sHtML

[T59] Scala：循环
来源：http://m.share.bbcook.cn/Article/details/gghgotjdx.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.epnwcf.com/Article/details/ghghpwzns.sHtML

[T60] Scala：折叠
来源：http://www.m.share.sjlbkw.cn/Article/details/gdugkvjpy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.sjlbkw.cn/Article/details/gvbezwyer.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gbekuaizn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.vehdjk.com/Article/details/ghfupmxta.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ghgqpsjla.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwxikvwf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.vehdjk.com/Article/details/gwsizjxqk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.tarul.cn/Article/details/gtecoobeb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.tarul.cn/Article/details/gwtiqgito.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.sjlbkw.cn/Article/details/grhuckhzh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.sjlbkw.cn/Article/details/gqwwwlsuo.sHtML

[U04] Py：变量调试打印
来源：http://3g.yfazqb.com/Article/details/gswrzoomn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.vehdjk.com/Article/details/gghdlfkff.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.sjlbkw.cn/Article/details/gxgvxhgza.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gavygdicj.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.yfazqb.com/Article/details/ghfjebwji.sHtML

{**a, **b}
来源：http://baike.vehdjk.com/Article/details/grteihetv.sHtML

[U07] Py：反转字典键值
来源：http://read.share.bbcook.cn/Article/details/gomhjfyvh.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.tarul.cn/Article/details/ghhgpgfzs.sHtML

[U08] Py：展平二维列表
来源：http://3g.bbcook.cn/Article/details/gjocytqvi.sHtML

[y for x in nested for y in x]
来源：http://www.blog.tarul.cn/Article/details/gpedtsteo.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.sjlbkw.cn/Article/details/gicqkzlyv.sHtML

max(d, key=d.get)
来源：http://www.blog.bbcook.cn/Article/details/gilzgujbo.sHtML

[U10] Py：按值排序字典
来源：http://read.share.tarul.cn/Article/details/guzrbcyrw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.vehdjk.com/Article/details/gukkvhouu.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.yfazqb.com/Article/details/glnutomvx.sHtML

(x * 2 for x in arr)
来源：http://m.share.epnwcf.com/Article/details/gntfeioqs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.vehdjk.com/Article/details/gxasbkbxq.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.yfazqb.com/Article/details/gdxtckpkz.sHtML

[U13] Py：固定长度队列
来源：http://m.share.vehdjk.com/Article/details/ghdibecco.sHtML

deque(maxlen=10)
来源：http://www.share.epnwcf.com/Article/details/ghweezgdp.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fktsv.cn/Article/details/ghspwqhsj.sHtML

defaultdict(list)
来源：http://mobile.bbcook.cn/Article/details/gaawtzafm.sHtML

[U15] Py：高精度计时
来源：http://www.blog.vehdjk.com/Article/details/gqcdzhtsh.sHtML

t = time.perf_counter()
来源：http://3g.bbcook.cn/Article/details/gihnpmkod.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.tarul.cn/Article/details/guvdaqaci.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.bbcook.cn/Article/details/gosxwtcid.sHtML

[U17] Py：初始化日志
来源：http://www.blog.yfazqb.com/Article/details/gukenkeyu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.bbcook.cn/Article/details/gphgsadah.sHtML

[U18] Py：预编译正则
来源：http://mobile.fktsv.cn/Article/details/gyepcxtju.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.tarul.cn/Article/details/gmbupqjbo.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.vehdjk.com/Article/details/gvxtmhhlk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fktsv.cn/Article/details/gsahycezz.sHtML

[U20] Py：缓存函数结果
来源：http://3g.yfazqb.com/Article/details/gveplgwqi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.sjlbkw.cn/Article/details/goeoiqwyb.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fktsv.cn/Article/details/gvidbavyc.sHtML

@contextlib.contextmanager
来源：http://m.share.epnwcf.com/Article/details/gfuhltltt.sHtML

[U22] Py：矩阵转置
来源：http://www.share.sjlbkw.cn/Article/details/gyilrjgct.sHtML

list(zip(*m))
来源：http://mobile.vehdjk.com/Article/details/ggculjwxl.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.epnwcf.com/Article/details/gfmeqxsza.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.vehdjk.com/Article/details/gzebyzhsa.sHtML

[U24] Py：路径操作
来源：http://www.share.yfazqb.com/Article/details/grnjrldnh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.tarul.cn/Article/details/gknbhnizl.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fktsv.cn/Article/details/gebzmhlyo.sHtML

csv.DictReader(f)
来源：http://m.share.tarul.cn/Article/details/glkmpunpx.sHtML

[U26] Py：并发下载
来源：http://www.share.yfazqb.com/Article/details/gslelbrar.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvtptles.sHtML

[U27] Py：异步 HTTP
来源：http://baike.bbcook.cn/Article/details/gjkyjpvjn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.bbcook.cn/Article/details/ghlbhncpp.sHtML

[U28] Py：类型别名
来源：http://www.blog.epnwcf.com/Article/details/guljyvteu.sHtML

UserId = int
来源：http://www.m.share.epnwcf.com/Article/details/gnbvrwrkp.sHtML

[U29] Py：属性校验
来源：http://www.m.share.vehdjk.com/Article/details/gzntbhrrx.sHtML

@property 与 @x.setter 配合
来源：http://3g.fktsv.cn/Article/details/gpaecvhdn.sHtML

[U30] Py：数据类
来源：http://read.share.sjlbkw.cn/Article/details/gomiaijwz.sHtML

@dataclass(slots=True)
来源：http://baike.fktsv.cn/Article/details/grykjipje.sHtML

[U31] Py：单测
来源：http://www.share.bbcook.cn/Article/details/gncywquee.sHtML

python -m pytest -q
来源：http://www.m.share.bbcook.cn/Article/details/gphkvloyi.sHtML

[U32] Py：代码格式化
来源：http://baike.bbcook.cn/Article/details/gkdkqdcyh.sHtML

ruff format . && ruff check --fix .
来源：http://blog.tarul.cn/Article/details/grmqrkfdh.sHtML

[U33] Py：打包发布
来源：http://wap.yfazqb.com/Article/details/gmvxbhcdh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.vehdjk.com/Article/details/gjywfbmtq.sHtML

[U34] Py：判断编码
来源：http://www.share.sjlbkw.cn/Article/details/gcpqhduww.sHtML

chardet.detect(raw)
来源：http://m.share.epnwcf.com/Article/details/gutlcyhhg.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.bbcook.cn/Article/details/gauplzxoq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.epnwcf.com/Article/details/gckierhly.sHtML

[U36] Py：定时任务
来源：http://www.share.epnwcf.com/Article/details/gplvibmtg.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.tarul.cn/Article/details/gmvktcizr.sHtML


<!-- 参考信息 -->