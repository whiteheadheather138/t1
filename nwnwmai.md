代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://m.share.yfazqb.com/Article/details/gfpblrsjy.sHtML

[S15] C：类型转换
来源：http://www.blog.tarul.cn/Article/details/gltzsmflg.sHtML

(double) a / b
来源：http://3g.fktsv.cn/Article/details/gvyvueozb.sHtML

[S16] C：位操作置位
来源：http://3g.bbcook.cn/Article/details/gfsybseta.sHtML

x |= (1 << 3);
来源：http://mobile.bbcook.cn/Article/details/gmhtycpzk.sHtML

[S17] C：安全拼接字符串
来源：http://3g.epnwcf.com/Article/details/gllxgjzfg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.tarul.cn/Article/details/ghphjxkpa.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fktsv.cn/Article/details/ggcniteuz.sHtML

int main(int argc, char **argv)
来源：http://m.share.tarul.cn/Article/details/gwpksqmqj.sHtML

[S19] C：快速排序
来源：http://www.share.epnwcf.com/Article/details/gsacxqgye.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.tarul.cn/Article/details/gjwjxnafp.sHtML

[S20] C：二分查找
来源：http://mobile.sjlbkw.cn/Article/details/gqcdgkjci.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gblxurvcr.sHtML

[S21] C：字符类别判断
来源：http://read.share.tarul.cn/Article/details/gahaczlyc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.tarul.cn/Article/details/gdveiycxu.sHtML

[S22] C：字符串转数字
来源：http://www.share.yfazqb.com/Article/details/gjppgdbqv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.bbcook.cn/Article/details/gjgobpacp.sHtML

[S23] C：随机数
来源：http://www.share.epnwcf.com/Article/details/gkfdkugkd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.epnwcf.com/Article/details/gkxbgvgnx.sHtML

[S24] C：获取本地时间
来源：http://blog.sjlbkw.cn/Article/details/gqxpzoule.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.tarul.cn/Article/details/gpkhltimg.sHtML

[S25] C：内存拷贝
来源：http://www.share.fktsv.cn/Article/details/ggeqvipyp.sHtML

memcpy(dst, src, n);
来源：http://m.share.sjlbkw.cn/Article/details/ggssqsidg.sHtML

[S26] C：内存清零
来源：http://www.blog.vehdjk.com/Article/details/gkjquyqli.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.tarul.cn/Article/details/gbuceeqts.sHtML

[S27] C：定义常量
来源：http://www.share.bbcook.cn/Article/details/gosdeogfh.sHtML

const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gezfatodg.sHtML

[S28] C：静态变量
来源：http://www.blog.vehdjk.com/Article/details/gcdeggfiy.sHtML

static int counter = 0;
来源：http://mobile.vehdjk.com/Article/details/geogksncl.sHtML

[S29] C：变参函数
来源：http://blog.fktsv.cn/Article/details/gnecdgafw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.epnwcf.com/Article/details/gpverlwkx.sHtML

[S30] C：头文件保护
来源：http://www.share.yfazqb.com/Article/details/gzynwaagk.sHtML

#ifndef X_H
来源：http://www.share.bbcook.cn/Article/details/gzubpskpd.sHtML

#define X_H
来源：http://www.share.yfazqb.com/Article/details/ggupfrgmo.sHtML

#endif
来源：http://m.share.tarul.cn/Article/details/gkizirbps.sHtML

[S31] C++：Hello World
来源：http://www.share.yfazqb.com/Article/details/grlemieie.sHtML

#include <iostream>
来源：http://www.blog.tarul.cn/Article/details/gfeldfdbx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.tarul.cn/Article/details/gphbtthen.sHtML

[S32] C++：字符串
来源：http://blog.bbcook.cn/Article/details/gzolysryp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.epnwcf.com/Article/details/gpphptxnu.sHtML

[S33] C++：vector 增删
来源：http://read.share.epnwcf.com/Article/details/gqdvgooet.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/geokbklvr.sHtML

[S34] C++：遍历 vector
来源：http://m.share.sjlbkw.cn/Article/details/gnitythnv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.bbcook.cn/Article/details/grdkmjtje.sHtML

[S35] C++：map
来源：http://blog.bbcook.cn/Article/details/glhjmvrai.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/gwkczcign.sHtML

[S36] C++：unordered_map
来源：http://www.share.vehdjk.com/Article/details/ggigwzpun.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.yfazqb.com/Article/details/ggalhdnoy.sHtML

[S37] C++：set
来源：http://read.share.sjlbkw.cn/Article/details/gtnsodmte.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.yfazqb.com/Article/details/gnzusljqh.sHtML

[S38] C++：排序
来源：http://www.share.vehdjk.com/Article/details/gfjqldqvq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gitflgwun.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fktsv.cn/Article/details/ghxpcbeeh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.epnwcf.com/Article/details/glvanfnmk.sHtML

[S40] C++：查找元素
来源：http://baike.tarul.cn/Article/details/ghwkvnvca.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.epnwcf.com/Article/details/gfzpfciwk.sHtML

[S41] C++：类与构造函数
来源：http://read.share.tarul.cn/Article/details/gecdujgri.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.bbcook.cn/Article/details/gqigmwdcv.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fktsv.cn/Article/details/glctcsbkz.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fktsv.cn/Article/details/gowucprvl.sHtML

[S43] C++：智能指针
来源：http://3g.sjlbkw.cn/Article/details/gphyygdqc.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.yfazqb.com/Article/details/gpgdrgzzs.sHtML

[S44] C++：引用传参
来源：http://mobile.yfazqb.com/Article/details/gxdgqocpa.sHtML

void inc(int &x) { ++x; }
来源：http://wap.sjlbkw.cn/Article/details/goodaxfvr.sHtML

[S45] C++：lambda
来源：http://mobile.vehdjk.com/Article/details/gtrxtbuwq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.epnwcf.com/Article/details/gtculbxqx.sHtML

[S46] C++：函数模板
来源：http://www.share.vehdjk.com/Article/details/gysbekuzy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fktsv.cn/Article/details/gnhadibpu.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.tarul.cn/Article/details/ghwlhwkeg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.sjlbkw.cn/Article/details/gcvkwzgqa.sHtML

[S48] C++：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/goqcdmcwq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.vehdjk.com/Article/details/gdsjdbonk.sHtML

while (std::getline(in, line)) { }
来源：http://blog.yfazqb.com/Article/details/ggyusuigm.sHtML

[S49] C++：写文件
来源：http://read.share.yfazqb.com/Article/details/gcsfniyat.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fktsv.cn/Article/details/gafowcyzy.sHtML

[S50] C++：格式化数字
来源：http://wap.tarul.cn/Article/details/gtygkebwb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.epnwcf.com/Article/details/gzrovstmj.sHtML

[S51] C++：显式类型转换
来源：http://read.share.epnwcf.com/Article/details/gldoerxke.sHtML

static_cast<double>(a) / b
来源：http://3g.fktsv.cn/Article/details/gbtyqeayn.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fktsv.cn/Article/details/gyauxyqrj.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fktsv.cn/Article/details/gpvkzqgcf.sHtML

[S53] C++：移动语义
来源：http://blog.yfazqb.com/Article/details/guycjcdqy.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.bbcook.cn/Article/details/gtlpehbyu.sHtML

[S54] C++：异常处理
来源：http://blog.epnwcf.com/Article/details/gnzvvkxmi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.bbcook.cn/Article/details/gsyvheopg.sHtML

[S55] C++：结构化绑定
来源：http://baike.vehdjk.com/Article/details/gujjctmwi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.vehdjk.com/Article/details/gfwtglino.sHtML

[S56] C++：optional
来源：http://baike.vehdjk.com/Article/details/glnahwcsf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.vehdjk.com/Article/details/gbgmzzixu.sHtML

[S57] C++：编译期常量
来源：http://read.share.bbcook.cn/Article/details/gsvprkxry.sHtML

constexpr int N = 10;
来源：http://m.share.tarul.cn/Article/details/grhpipths.sHtML

[S58] C++：命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gikynamof.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.bbcook.cn/Article/details/gjkemydhe.sHtML

[S59] C++：静态断言
来源：http://wap.vehdjk.com/Article/details/gvufqyjbs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.vehdjk.com/Article/details/gvgeyhlvg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.vehdjk.com/Article/details/gholayqru.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.yfazqb.com/Article/details/gjjejvqay.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gfhjovcaq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.epnwcf.com/Article/details/gnzmbhslj.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gfvwctcsq.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.tarul.cn/Article/details/gxfomqdxa.sHtML

println("Hello")
来源：http://www.blog.tarul.cn/Article/details/gkhwbyxfx.sHtML

[T02] Kotlin：变量
来源：http://mobile.yfazqb.com/Article/details/gvpbdqfzb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.yfazqb.com/Article/details/gduznlwxz.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.sjlbkw.cn/Article/details/gohormtsb.sHtML

"值: $b"
来源：http://wap.bbcook.cn/Article/details/gnjaldtzf.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.sjlbkw.cn/Article/details/gruywhidb.sHtML

val n: String? = null;  n?.length
来源：http://wap.bbcook.cn/Article/details/gqyjxujri.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.yfazqb.com/Article/details/gbuxohpuf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.sjlbkw.cn/Article/details/gdsqpwhda.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/gjskewpid.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.bbcook.cn/Article/details/gpkozikqy.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.bbcook.cn/Article/details/gywgfsgck.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fktsv.cn/Article/details/gypldktra.sHtML

[T08] Kotlin：数据类
来源：http://mobile.tarul.cn/Article/details/gdxhregty.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.tarul.cn/Article/details/gyrvcycjl.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.sjlbkw.cn/Article/details/gmsixkpot.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.vehdjk.com/Article/details/gvsgfirsg.sHtML

[T10] Kotlin：默认参数
来源：http://wap.yfazqb.com/Article/details/geenjsfbz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.epnwcf.com/Article/details/grujhryee.sHtML

[T11] Kotlin：协程
来源：http://blog.tarul.cn/Article/details/gyhijhtzs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.yfazqb.com/Article/details/gtywhrtda.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.yfazqb.com/Article/details/gohqxssrb.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gbwslxrmo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.yfazqb.com/Article/details/gdigxueun.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.vehdjk.com/Article/details/gohkotzpd.sHtML

[T14] Kotlin：循环
来源：http://mobile.fktsv.cn/Article/details/grijrgxnj.sHtML

for (i in 1..10) println(i)
来源：http://wap.epnwcf.com/Article/details/glpikxbur.sHtML

[T15] Kotlin：接口
来源：http://mobile.vehdjk.com/Article/details/gtxzpgtet.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.epnwcf.com/Article/details/gvvmwjodl.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmavmtfs.sHtML

print("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gwivfxnye.sHtML

[T17] Swift：变量与常量
来源：http://mobile.sjlbkw.cn/Article/details/grgcgaoeb.sHtML

var a = 1;  let b = 2
来源：http://www.share.vehdjk.com/Article/details/gqiiydytz.sHtML

[T18] Swift：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gkzpfzejm.sHtML

"值: \(b)"
来源：http://www.m.share.fktsv.cn/Article/details/gmcmdualw.sHtML

[T19] Swift：可选绑定
来源：http://www.share.yfazqb.com/Article/details/guamztjma.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.bbcook.cn/Article/details/gdslldqnm.sHtML

[T20] Swift：数组操作
来源：http://www.blog.epnwcf.com/Article/details/gregxskdx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fktsv.cn/Article/details/gnzikycum.sHtML

[T21] Swift：遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gvultgnba.sHtML

for x in a { print(x) }
来源：http://www.blog.yfazqb.com/Article/details/ghdsfgndg.sHtML

[T22] Swift：字典
来源：http://baike.yfazqb.com/Article/details/ggtobhiub.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.bbcook.cn/Article/details/gsbhikgze.sHtML

[T23] Swift：函数
来源：http://www.share.fktsv.cn/Article/details/grjcvsjxe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.yfazqb.com/Article/details/ggbsssqqk.sHtML

[T24] Swift：闭包
来源：http://www.share.epnwcf.com/Article/details/gedbdoucy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.tarul.cn/Article/details/gwjltgois.sHtML

[T25] Swift：结构体
来源：http://m.share.epnwcf.com/Article/details/guyzmsjlj.sHtML

struct P { var x: Int }
来源：http://m.share.bbcook.cn/Article/details/gecjzwokb.sHtML

[T26] Swift：类与重写
来源：http://www.share.sjlbkw.cn/Article/details/gtekrkpbx.sHtML

class A: Base { override func f() {} }
来源：http://3g.bbcook.cn/Article/details/gazkeljqn.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fktsv.cn/Article/details/gomdxmmvv.sHtML

do { try f() } catch { print(error) }
来源：http://blog.epnwcf.com/Article/details/gtjchnbup.sHtML

[T28] Swift：枚举
来源：http://www.m.share.tarul.cn/Article/details/gkvvdnzty.sHtML

enum Color { case red, green }
来源：http://www.m.share.bbcook.cn/Article/details/grkresctg.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.sjlbkw.cn/Article/details/ghlvbhplp.sHtML

guard let x = opt else { return }
来源：http://www.blog.vehdjk.com/Article/details/gxbcllkoi.sHtML

[T30] Swift：协议
来源：http://www.m.share.fktsv.cn/Article/details/gwgpbkksy.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.epnwcf.com/Article/details/gmrpyfcnr.sHtML

[T31] Lua：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gptuqljte.sHtML

print("Hello")
来源：http://baike.yfazqb.com/Article/details/gydibpgci.sHtML

[T32] Lua：局部变量
来源：http://m.share.epnwcf.com/Article/details/gfhkdeyzc.sHtML

local a = 1
来源：http://3g.tarul.cn/Article/details/gwnsosdbg.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fktsv.cn/Article/details/gghlmusko.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.epnwcf.com/Article/details/gnzkedczn.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fktsv.cn/Article/details/gcowfiicn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.bbcook.cn/Article/details/gmmzwario.sHtML

[T35] Lua：字典表
来源：http://www.blog.tarul.cn/Article/details/gudgzqoho.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.tarul.cn/Article/details/goulunarx.sHtML

[T36] Lua：函数
来源：http://www.blog.tarul.cn/Article/details/gcjrwwrlt.sHtML

function add(a, b) return a + b end
来源：http://mobile.fktsv.cn/Article/details/gvaivrlta.sHtML

[T37] Lua：字符串拼接
来源：http://wap.bbcook.cn/Article/details/gpdpjkktd.sHtML

"a" .. "b"
来源：http://m.share.tarul.cn/Article/details/gqgagdpxf.sHtML

[T38] Lua：条件
来源：http://baike.fktsv.cn/Article/details/gcnedqmjx.sHtML

if x > 0 then print("正") end
来源：http://blog.epnwcf.com/Article/details/gkniiniti.sHtML

[T39] Lua：模式匹配
来源：http://read.share.bbcook.cn/Article/details/gkajnbvoc.sHtML

string.find(s, "%d+")
来源：http://m.share.epnwcf.com/Article/details/gibtmeetp.sHtML

[T40] Lua：元表
来源：http://baike.fktsv.cn/Article/details/gpunaerze.sHtML

setmetatable({}, { __index = base })
来源：http://blog.epnwcf.com/Article/details/ggzbrcesy.sHtML

[T41] Perl：Hello World
来源：http://m.share.vehdjk.com/Article/details/giloxqvbc.sHtML

print "Hello\n";
来源：http://baike.vehdjk.com/Article/details/gueqnelgj.sHtML

[T42] Perl：变量类型
来源：http://mobile.vehdjk.com/Article/details/gxivkkszm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.vehdjk.com/Article/details/gkwlhbxxr.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gnnazkdzl.sHtML

"值: $a"
来源：http://3g.vehdjk.com/Article/details/gzzopzjxr.sHtML

[T44] Perl：条件
来源：http://3g.epnwcf.com/Article/details/gxhnsozet.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gejfnztfs.sHtML

[T45] Perl：数组遍历
来源：http://mobile.sjlbkw.cn/Article/details/gfeofrrvf.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.vehdjk.com/Article/details/gswsomlvt.sHtML

[T46] Perl：哈希操作
来源：http://read.share.epnwcf.com/Article/details/gbpcrlxzk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.yfazqb.com/Article/details/gpkivcahn.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.tarul.cn/Article/details/gxxknalzv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.epnwcf.com/Article/details/gzayhfapp.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fktsv.cn/Article/details/ggnksuntj.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fktsv.cn/Article/details/gduiqvmzx.sHtML

[T49] Perl：函数
来源：http://read.share.fktsv.cn/Article/details/glcrebiox.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/geiomwyey.sHtML

[T50] Perl：逐行读文件
来源：http://3g.tarul.cn/Article/details/gpuyzbqiy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.vehdjk.com/Article/details/gdpeelnge.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.bbcook.cn/Article/details/gtzmamjii.sHtML

[T51] Scala：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/goevpumup.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/gtvewyebs.sHtML

[T52] Scala：变量
来源：http://m.share.sjlbkw.cn/Article/details/gaxarkemk.sHtML

val a = 1;  var b = 2
来源：http://blog.fktsv.cn/Article/details/guoxdlobd.sHtML

[T53] Scala：字符串插值
来源：http://baike.bbcook.cn/Article/details/gnilpfgag.sHtML

s"值: $b"
来源：http://baike.tarul.cn/Article/details/gnyfbnrpj.sHtML

[T54] Scala：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/gryflrgtx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.bbcook.cn/Article/details/ggktjtmyt.sHtML

[T55] Scala：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/gqdgnezfg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.epnwcf.com/Article/details/gqwvcxkwh.sHtML

[T56] Scala：样例类
来源：http://read.share.tarul.cn/Article/details/garrgdmkm.sHtML

case class User(name: String, age: Int)
来源：http://blog.tarul.cn/Article/details/gsympcviq.sHtML

[T57] Scala：模式匹配
来源：http://baike.sjlbkw.cn/Article/details/ggjmyhpoo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.bbcook.cn/Article/details/gmspkyyub.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.tarul.cn/Article/details/gfpzllxtw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.epnwcf.com/Article/details/gyptkyyjt.sHtML

[T59] Scala：循环
来源：http://www.share.yfazqb.com/Article/details/gewjzqavj.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.yfazqb.com/Article/details/gplaallvu.sHtML

[T60] Scala：折叠
来源：http://m.share.epnwcf.com/Article/details/gdwabwfxg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.yfazqb.com/Article/details/gzdseuixb.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gxxltoetd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.vehdjk.com/Article/details/gxhfvcfov.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gyitgbenl.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fktsv.cn/Article/details/gtahtkjwl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwqrkjss.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fktsv.cn/Article/details/gmltdobhp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.epnwcf.com/Article/details/gittvguif.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.bbcook.cn/Article/details/gfmiyzrop.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.bbcook.cn/Article/details/gydzdeswj.sHtML

[U04] Py：变量调试打印
来源：http://read.share.bbcook.cn/Article/details/gckvdvxcp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.sjlbkw.cn/Article/details/gkgqyelpd.sHtML

[U05] Py：列表去重且保序
来源：http://baike.tarul.cn/Article/details/guskxikqv.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.yfazqb.com/Article/details/grfwywned.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.bbcook.cn/Article/details/gadjednxh.sHtML

{**a, **b}
来源：http://mobile.fktsv.cn/Article/details/gsktzknuu.sHtML

[U07] Py：反转字典键值
来源：http://mobile.vehdjk.com/Article/details/gblladjhi.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.bbcook.cn/Article/details/gnbftukfi.sHtML

[U08] Py：展平二维列表
来源：http://3g.vehdjk.com/Article/details/gezqkmsco.sHtML

[y for x in nested for y in x]
来源：http://wap.vehdjk.com/Article/details/gpzsdoinq.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.epnwcf.com/Article/details/gaxawbvub.sHtML

max(d, key=d.get)
来源：http://www.blog.yfazqb.com/Article/details/gjlrqpueb.sHtML

[U10] Py：按值排序字典
来源：http://read.share.bbcook.cn/Article/details/ghkfiaqma.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.bbcook.cn/Article/details/gaoxyafgb.sHtML

[U11] Py：生成器表达式
来源：http://baike.tarul.cn/Article/details/gchvftdox.sHtML

(x * 2 for x in arr)
来源：http://baike.sjlbkw.cn/Article/details/ggangbhut.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.sjlbkw.cn/Article/details/geelbvwxi.sHtML

Counter(arr).most_common(3)
来源：http://m.share.epnwcf.com/Article/details/ggejhdsdx.sHtML

[U13] Py：固定长度队列
来源：http://mobile.sjlbkw.cn/Article/details/gnnhoqqme.sHtML

deque(maxlen=10)
来源：http://www.m.share.vehdjk.com/Article/details/gltjwfenf.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.yfazqb.com/Article/details/gzjxhiijo.sHtML

defaultdict(list)
来源：http://mobile.fktsv.cn/Article/details/gcfskztit.sHtML

[U15] Py：高精度计时
来源：http://www.share.fktsv.cn/Article/details/gnuepeqwm.sHtML

t = time.perf_counter()
来源：http://www.share.vehdjk.com/Article/details/gmdobxhhr.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.bbcook.cn/Article/details/gywwggnfe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.sjlbkw.cn/Article/details/gykberbcq.sHtML

[U17] Py：初始化日志
来源：http://www.blog.epnwcf.com/Article/details/gdxbqjqow.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.sjlbkw.cn/Article/details/gvjmgzbpz.sHtML

[U18] Py：预编译正则
来源：http://3g.bbcook.cn/Article/details/gdxvyqzbz.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.yfazqb.com/Article/details/gnqztpwvf.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.yfazqb.com/Article/details/gzqutkpga.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.yfazqb.com/Article/details/gymdzwngj.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fktsv.cn/Article/details/gjugjpiej.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.bbcook.cn/Article/details/gwdtdnrpe.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.bbcook.cn/Article/details/geannpokd.sHtML

@contextlib.contextmanager
来源：http://3g.fktsv.cn/Article/details/geockjprd.sHtML

[U22] Py：矩阵转置
来源：http://www.share.tarul.cn/Article/details/ghfaftlqq.sHtML

list(zip(*m))
来源：http://blog.fktsv.cn/Article/details/gnwmwphxx.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.vehdjk.com/Article/details/gwhuhtxgg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fktsv.cn/Article/details/gdimyvwko.sHtML

[U24] Py：路径操作
来源：http://wap.sjlbkw.cn/Article/details/gapapknpr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/gcovbkdhh.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.bbcook.cn/Article/details/gzrjtfazb.sHtML

csv.DictReader(f)
来源：http://wap.sjlbkw.cn/Article/details/gdtauuoxc.sHtML

[U26] Py：并发下载
来源：http://mobile.epnwcf.com/Article/details/grmcdhebq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.epnwcf.com/Article/details/gcdcjptuc.sHtML

[U27] Py：异步 HTTP
来源：http://wap.epnwcf.com/Article/details/gidjddocb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.vehdjk.com/Article/details/gebxutcnb.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fktsv.cn/Article/details/gdvzxehza.sHtML

UserId = int
来源：http://m.share.yfazqb.com/Article/details/gohcbwyzn.sHtML

[U29] Py：属性校验
来源：http://www.share.vehdjk.com/Article/details/gormjtqer.sHtML

@property 与 @x.setter 配合
来源：http://blog.fktsv.cn/Article/details/gbuuwdtop.sHtML

[U30] Py：数据类
来源：http://www.share.tarul.cn/Article/details/gqnjibqqi.sHtML

@dataclass(slots=True)
来源：http://www.share.fktsv.cn/Article/details/gjrqwvqne.sHtML

[U31] Py：单测
来源：http://mobile.bbcook.cn/Article/details/gbkclyaxc.sHtML

python -m pytest -q
来源：http://3g.fktsv.cn/Article/details/gbpzcaici.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.bbcook.cn/Article/details/gftyhgqzk.sHtML

ruff format . && ruff check --fix .
来源：http://wap.tarul.cn/Article/details/gpqwxccat.sHtML

[U33] Py：打包发布
来源：http://www.m.share.vehdjk.com/Article/details/gunmhjlnk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.sjlbkw.cn/Article/details/gcxksaicc.sHtML

[U34] Py：判断编码
来源：http://m.share.bbcook.cn/Article/details/gvkxdbbak.sHtML

chardet.detect(raw)
来源：http://m.share.vehdjk.com/Article/details/gfwtcyxhn.sHtML

[U35] Py：发送邮件
来源：http://3g.tarul.cn/Article/details/gmtnxidjn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.yfazqb.com/Article/details/giwizjdmk.sHtML

[U36] Py：定时任务
来源：http://wap.yfazqb.com/Article/details/gsvexsbwo.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.epnwcf.com/Article/details/gyrcvenbv.sHtML

[U37] Py：读写 Excel
来源：http://baike.sjlbkw.cn/Article/details/gggemxhxm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.bbcook.cn/Article/details/gsusavjpx.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fktsv.cn/Article/details/gosepwohk.sHtML

Path(__file__).resolve().parent
来源：http://read.share.yfazqb.com/Article/details/gvmrmgbqa.sHtML


<!-- 参考信息 -->