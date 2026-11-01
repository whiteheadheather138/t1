代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://mobile.sjlbkw.cn/Article/details/gfwomqegc.sHtML

[S15] C：类型转换
来源：http://3g.yfazqb.com/Article/details/gnwmzhdkn.sHtML

(double) a / b
来源：http://read.share.epnwcf.com/Article/details/gyclcvuba.sHtML

[S16] C：位操作置位
来源：http://mobile.vehdjk.com/Article/details/gkyhgazav.sHtML

x |= (1 << 3);
来源：http://3g.tarul.cn/Article/details/grbhjgtxu.sHtML

[S17] C：安全拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gsowhnqaj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fktsv.cn/Article/details/gtygzogno.sHtML

[S18] C：命令行参数
来源：http://www.share.bbcook.cn/Article/details/gxlukthel.sHtML

int main(int argc, char **argv)
来源：http://mobile.sjlbkw.cn/Article/details/gtfeaqmlx.sHtML

[S19] C：快速排序
来源：http://baike.sjlbkw.cn/Article/details/gnkxrviju.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.vehdjk.com/Article/details/gqgwoohnb.sHtML

[S20] C：二分查找
来源：http://www.blog.yfazqb.com/Article/details/gylwcdhas.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.vehdjk.com/Article/details/gnhnsswmm.sHtML

[S21] C：字符类别判断
来源：http://wap.tarul.cn/Article/details/gqgsgiyuh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.vehdjk.com/Article/details/gsxaxeala.sHtML

[S22] C：字符串转数字
来源：http://baike.epnwcf.com/Article/details/gftopmtho.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.sjlbkw.cn/Article/details/gitmzcgka.sHtML

[S23] C：随机数
来源：http://mobile.sjlbkw.cn/Article/details/guvhwerjx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.vehdjk.com/Article/details/ghbbsfsac.sHtML

[S24] C：获取本地时间
来源：http://read.share.tarul.cn/Article/details/ghnevlqos.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.vehdjk.com/Article/details/gqqiwovld.sHtML

[S25] C：内存拷贝
来源：http://3g.fktsv.cn/Article/details/gcooencih.sHtML

memcpy(dst, src, n);
来源：http://www.share.vehdjk.com/Article/details/gkwlmaasj.sHtML

[S26] C：内存清零
来源：http://3g.fktsv.cn/Article/details/gmzgwlchh.sHtML

memset(a, 0, sizeof a);
来源：http://wap.tarul.cn/Article/details/ggymnjcbb.sHtML

[S27] C：定义常量
来源：http://www.m.share.epnwcf.com/Article/details/gvmxoyzaa.sHtML

const double PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gvrrhnwyd.sHtML

[S28] C：静态变量
来源：http://www.m.share.epnwcf.com/Article/details/ggmxfjhao.sHtML

static int counter = 0;
来源：http://wap.sjlbkw.cn/Article/details/gynddumcg.sHtML

[S29] C：变参函数
来源：http://baike.epnwcf.com/Article/details/gdelkjhlp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.sjlbkw.cn/Article/details/gpoxmjuwp.sHtML

[S30] C：头文件保护
来源：http://read.share.sjlbkw.cn/Article/details/gbilazyfq.sHtML

#ifndef X_H
来源：http://read.share.tarul.cn/Article/details/gnlfznpji.sHtML

#define X_H
来源：http://read.share.vehdjk.com/Article/details/gynmcnbbp.sHtML

#endif
来源：http://read.share.fktsv.cn/Article/details/gxjhhvkjb.sHtML

[S31] C++：Hello World
来源：http://baike.yfazqb.com/Article/details/gojvtwezg.sHtML

#include <iostream>
来源：http://read.share.sjlbkw.cn/Article/details/gtsxvnvzq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.yfazqb.com/Article/details/gxaihwtre.sHtML

[S32] C++：字符串
来源：http://blog.sjlbkw.cn/Article/details/grncrberz.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.vehdjk.com/Article/details/guouytbgr.sHtML

[S33] C++：vector 增删
来源：http://wap.bbcook.cn/Article/details/ghvlmttun.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fktsv.cn/Article/details/gdythqxfa.sHtML

[S34] C++：遍历 vector
来源：http://m.share.epnwcf.com/Article/details/glqguhfnq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fktsv.cn/Article/details/gmcctupvv.sHtML

[S35] C++：map
来源：http://www.m.share.fktsv.cn/Article/details/gdpejczym.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gdblgwsym.sHtML

[S36] C++：unordered_map
来源：http://wap.yfazqb.com/Article/details/gwrlqpcpn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gjiuvwclp.sHtML

[S37] C++：set
来源：http://www.blog.vehdjk.com/Article/details/gdokvbovc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.epnwcf.com/Article/details/grvdtkend.sHtML

[S38] C++：排序
来源：http://mobile.vehdjk.com/Article/details/gricqdggc.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.bbcook.cn/Article/details/gujelzaox.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.sjlbkw.cn/Article/details/gbppxbwxe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fktsv.cn/Article/details/gqaewmgmm.sHtML

[S40] C++：查找元素
来源：http://m.share.epnwcf.com/Article/details/gghldcpjj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.tarul.cn/Article/details/gdjptbpzb.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.epnwcf.com/Article/details/gbergxscz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.vehdjk.com/Article/details/gtofznicb.sHtML

[S42] C++：继承与虚函数
来源：http://blog.epnwcf.com/Article/details/gqxocypiz.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.sjlbkw.cn/Article/details/ghsozxocv.sHtML

[S43] C++：智能指针
来源：http://blog.yfazqb.com/Article/details/gugnvgxun.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.epnwcf.com/Article/details/gkcwxcgfo.sHtML

[S44] C++：引用传参
来源：http://wap.bbcook.cn/Article/details/guiheavlk.sHtML

void inc(int &x) { ++x; }
来源：http://baike.sjlbkw.cn/Article/details/gpqkkbmlq.sHtML

[S45] C++：lambda
来源：http://blog.sjlbkw.cn/Article/details/gkjrmiipp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fktsv.cn/Article/details/gtltrztzo.sHtML

[S46] C++：函数模板
来源：http://wap.bbcook.cn/Article/details/gbphhyush.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.tarul.cn/Article/details/gcjgglqfw.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.vehdjk.com/Article/details/gexjsoxwg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.yfazqb.com/Article/details/ghrpxdfbl.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gjpyvvgpq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.vehdjk.com/Article/details/gstfehylw.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.tarul.cn/Article/details/gbiksmgbs.sHtML

[S49] C++：写文件
来源：http://3g.vehdjk.com/Article/details/gugyswtls.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fktsv.cn/Article/details/ggwztvcri.sHtML

[S50] C++：格式化数字
来源：http://m.share.fktsv.cn/Article/details/gewofexym.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.tarul.cn/Article/details/gyejjwmpw.sHtML

[S51] C++：显式类型转换
来源：http://3g.fktsv.cn/Article/details/gzqzbujrf.sHtML

static_cast<double>(a) / b
来源：http://www.blog.epnwcf.com/Article/details/gwxgpygij.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.epnwcf.com/Article/details/ghittzljt.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.vehdjk.com/Article/details/gwelbxrdw.sHtML

[S53] C++：移动语义
来源：http://www.share.tarul.cn/Article/details/ginbgutmh.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.tarul.cn/Article/details/girasopfa.sHtML

[S54] C++：异常处理
来源：http://www.share.yfazqb.com/Article/details/gftbpqjwi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.bbcook.cn/Article/details/gsxlmasxk.sHtML

[S55] C++：结构化绑定
来源：http://wap.tarul.cn/Article/details/gleeruelm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.bbcook.cn/Article/details/gqrpdmavi.sHtML

[S56] C++：optional
来源：http://blog.sjlbkw.cn/Article/details/gonxktwcb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.bbcook.cn/Article/details/gosqtyrkd.sHtML

[S57] C++：编译期常量
来源：http://read.share.tarul.cn/Article/details/glphhzsar.sHtML

constexpr int N = 10;
来源：http://blog.vehdjk.com/Article/details/gaydszrtx.sHtML

[S58] C++：命名空间
来源：http://www.m.share.epnwcf.com/Article/details/geqtglmwx.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.bbcook.cn/Article/details/gmlqyzqqa.sHtML

[S59] C++：静态断言
来源：http://read.share.tarul.cn/Article/details/goxktbgar.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fktsv.cn/Article/details/gzktafntd.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.vehdjk.com/Article/details/gawhzjbem.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.yfazqb.com/Article/details/gmqylwlrm.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gcshmkgwv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.yfazqb.com/Article/details/gmbajujxu.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gyvzptojj.sHtML

[T01] Kotlin：Hello World
来源：http://3g.yfazqb.com/Article/details/gvnlrmuzw.sHtML

println("Hello")
来源：http://wap.bbcook.cn/Article/details/gyuxlxclo.sHtML

[T02] Kotlin：变量
来源：http://www.blog.tarul.cn/Article/details/grbgpkmwn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.vehdjk.com/Article/details/gsbwbvwyu.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.vehdjk.com/Article/details/gwtuqidnc.sHtML

"值: $b"
来源：http://blog.yfazqb.com/Article/details/gaxaosbzr.sHtML

[T04] Kotlin：空安全
来源：http://baike.yfazqb.com/Article/details/gqjiinpvc.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fktsv.cn/Article/details/gyhyzzvhk.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.bbcook.cn/Article/details/gdttrjglm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.vehdjk.com/Article/details/gppkuxmaz.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.tarul.cn/Article/details/ggmqtrtzl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fktsv.cn/Article/details/gfsvfbmwr.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.vehdjk.com/Article/details/gulezoqzj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.tarul.cn/Article/details/grkcxiute.sHtML

[T08] Kotlin：数据类
来源：http://m.share.sjlbkw.cn/Article/details/gparcwzsg.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.tarul.cn/Article/details/gnftburzb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.yfazqb.com/Article/details/gvrwkfoio.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.bbcook.cn/Article/details/gvwjnyouz.sHtML

[T10] Kotlin：默认参数
来源：http://wap.epnwcf.com/Article/details/gfwfqpwih.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.tarul.cn/Article/details/gqhjtirki.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.vehdjk.com/Article/details/gfnuusihc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.epnwcf.com/Article/details/gvhqppvtf.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.yfazqb.com/Article/details/gdetlnswx.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/greogptdj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.tarul.cn/Article/details/gmghudiwp.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.tarul.cn/Article/details/gjtbuocun.sHtML

[T14] Kotlin：循环
来源：http://baike.vehdjk.com/Article/details/giazyhdaa.sHtML

for (i in 1..10) println(i)
来源：http://3g.epnwcf.com/Article/details/gjzcqxgaw.sHtML

[T15] Kotlin：接口
来源：http://www.blog.sjlbkw.cn/Article/details/ghgfpdkdw.sHtML

interface Shape { fun area(): Double }
来源：http://wap.vehdjk.com/Article/details/gvhkaxaxy.sHtML

[T16] Swift：Hello World
来源：http://m.share.tarul.cn/Article/details/glvqcdppo.sHtML

print("Hello")
来源：http://www.share.bbcook.cn/Article/details/gmfgkrxjm.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.vehdjk.com/Article/details/gurwqtccx.sHtML

var a = 1;  let b = 2
来源：http://3g.bbcook.cn/Article/details/gulpmgwln.sHtML

[T18] Swift：字符串插值
来源：http://wap.yfazqb.com/Article/details/grebpiuhk.sHtML

"值: \(b)"
来源：http://baike.sjlbkw.cn/Article/details/gghyvsjnu.sHtML

[T19] Swift：可选绑定
来源：http://mobile.vehdjk.com/Article/details/gloojowie.sHtML

if let n = opt { print(n) }
来源：http://mobile.tarul.cn/Article/details/gyotiqjdz.sHtML

[T20] Swift：数组操作
来源：http://blog.sjlbkw.cn/Article/details/ghzzktauq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fktsv.cn/Article/details/gklylnjkn.sHtML

[T21] Swift：遍历
来源：http://read.share.fktsv.cn/Article/details/gfvjdjool.sHtML

for x in a { print(x) }
来源：http://m.share.vehdjk.com/Article/details/gcrvovycr.sHtML

[T22] Swift：字典
来源：http://mobile.epnwcf.com/Article/details/gwlhlyxsy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.yfazqb.com/Article/details/gzlgxiyjw.sHtML

[T23] Swift：函数
来源：http://wap.epnwcf.com/Article/details/ggcypgxqt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.yfazqb.com/Article/details/gkxkphkaz.sHtML

[T24] Swift：闭包
来源：http://www.blog.fktsv.cn/Article/details/gievgojyp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.tarul.cn/Article/details/gzxvilhmb.sHtML

[T25] Swift：结构体
来源：http://blog.tarul.cn/Article/details/gackzkjzw.sHtML

struct P { var x: Int }
来源：http://blog.vehdjk.com/Article/details/grrgcucui.sHtML

[T26] Swift：类与重写
来源：http://blog.tarul.cn/Article/details/gncilwndn.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gioyonhyv.sHtML

[T27] Swift：错误处理
来源：http://3g.fktsv.cn/Article/details/gpalumnuq.sHtML

do { try f() } catch { print(error) }
来源：http://baike.vehdjk.com/Article/details/gvnwiykpw.sHtML

[T28] Swift：枚举
来源：http://www.m.share.epnwcf.com/Article/details/gwjschxfo.sHtML

enum Color { case red, green }
来源：http://baike.yfazqb.com/Article/details/ghlbamklp.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.bbcook.cn/Article/details/gdwmkrzam.sHtML

guard let x = opt else { return }
来源：http://www.m.share.yfazqb.com/Article/details/ggonpzgae.sHtML

[T30] Swift：协议
来源：http://wap.tarul.cn/Article/details/gmcteqhmp.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.vehdjk.com/Article/details/gnhhanqqv.sHtML

[T31] Lua：Hello World
来源：http://baike.yfazqb.com/Article/details/gkecgeaxa.sHtML

print("Hello")
来源：http://www.blog.bbcook.cn/Article/details/girsoprog.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.yfazqb.com/Article/details/gayoinntq.sHtML

local a = 1
来源：http://www.share.sjlbkw.cn/Article/details/gidghizsx.sHtML

[T33] Lua：表（数组）
来源：http://read.share.bbcook.cn/Article/details/gujtkvvyy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.sjlbkw.cn/Article/details/gjvieqxps.sHtML

[T34] Lua：遍历表
来源：http://wap.bbcook.cn/Article/details/gzwfmnfsn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fktsv.cn/Article/details/glgsvudbi.sHtML

[T35] Lua：字典表
来源：http://www.blog.yfazqb.com/Article/details/gaudblxee.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.vehdjk.com/Article/details/grhyfvioq.sHtML

[T36] Lua：函数
来源：http://m.share.yfazqb.com/Article/details/gtnczymrd.sHtML

function add(a, b) return a + b end
来源：http://www.share.sjlbkw.cn/Article/details/gpjmkqsbv.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.tarul.cn/Article/details/gdoysimgu.sHtML

"a" .. "b"
来源：http://mobile.bbcook.cn/Article/details/glrhhpumj.sHtML

[T38] Lua：条件
来源：http://www.share.yfazqb.com/Article/details/gknskgbii.sHtML

if x > 0 then print("正") end
来源：http://3g.bbcook.cn/Article/details/gmgwkmrvn.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.yfazqb.com/Article/details/gpduqghqn.sHtML

string.find(s, "%d+")
来源：http://mobile.fktsv.cn/Article/details/guxohzhsl.sHtML

[T40] Lua：元表
来源：http://baike.vehdjk.com/Article/details/gqsydjwri.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.yfazqb.com/Article/details/gglpdpuwf.sHtML

[T41] Perl：Hello World
来源：http://3g.epnwcf.com/Article/details/gygizvayk.sHtML

print "Hello\n";
来源：http://www.blog.tarul.cn/Article/details/gfypcjfsi.sHtML

[T42] Perl：变量类型
来源：http://3g.sjlbkw.cn/Article/details/gpcuhozrc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.sjlbkw.cn/Article/details/gbeznazfz.sHtML

[T43] Perl：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gmeoyrjyf.sHtML

"值: $a"
来源：http://m.share.tarul.cn/Article/details/gdeuceuwz.sHtML

[T44] Perl：条件
来源：http://read.share.tarul.cn/Article/details/gwapjxadz.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.epnwcf.com/Article/details/gzjjbmoaq.sHtML

[T45] Perl：数组遍历
来源：http://3g.yfazqb.com/Article/details/gfxidphsf.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fktsv.cn/Article/details/gftmiekym.sHtML

[T46] Perl：哈希操作
来源：http://read.share.bbcook.cn/Article/details/gorhjohnh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.epnwcf.com/Article/details/gvttrkdhl.sHtML

[T47] Perl：正则捕获
来源：http://read.share.sjlbkw.cn/Article/details/gphfenofj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.epnwcf.com/Article/details/gyplsecdx.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.tarul.cn/Article/details/gxxmhbqln.sHtML

$s =~ s/old/new/g;
来源：http://www.share.yfazqb.com/Article/details/gfpzkrrlp.sHtML

[T49] Perl：函数
来源：http://blog.epnwcf.com/Article/details/ggkpldkvp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gjxcgarqd.sHtML

[T50] Perl：逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/ganmeeimb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.vehdjk.com/Article/details/glyypuzrh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.bbcook.cn/Article/details/glpqfxxkk.sHtML

[T51] Scala：Hello World
来源：http://www.share.yfazqb.com/Article/details/ghvqrvexd.sHtML

println("Hello")
来源：http://3g.fktsv.cn/Article/details/gjkvdrbtc.sHtML

[T52] Scala：变量
来源：http://www.blog.bbcook.cn/Article/details/gpixqkgyn.sHtML

val a = 1;  var b = 2
来源：http://read.share.epnwcf.com/Article/details/ghhmenccr.sHtML

[T53] Scala：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/ggsvtvimj.sHtML

s"值: $b"
来源：http://wap.bbcook.cn/Article/details/gnisbzmti.sHtML

[T54] Scala：集合映射
来源：http://blog.vehdjk.com/Article/details/gkwlmcrrf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fktsv.cn/Article/details/gteysoccu.sHtML

[T55] Scala：集合过滤
来源：http://3g.tarul.cn/Article/details/gmshwxnvi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.bbcook.cn/Article/details/glsetlkxx.sHtML

[T56] Scala：样例类
来源：http://blog.tarul.cn/Article/details/gnvljglnk.sHtML

case class User(name: String, age: Int)
来源：http://wap.sjlbkw.cn/Article/details/gjtqnwnfg.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fktsv.cn/Article/details/geeujkjjp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.bbcook.cn/Article/details/ggvrkmloy.sHtML

[T58] Scala：函数定义
来源：http://blog.fktsv.cn/Article/details/gwrzifavl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.bbcook.cn/Article/details/glrdmgcnc.sHtML

[T59] Scala：循环
来源：http://read.share.fktsv.cn/Article/details/gmqiaoodu.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fktsv.cn/Article/details/gcmrdfbag.sHtML

[T60] Scala：折叠
来源：http://wap.sjlbkw.cn/Article/details/gcghvdoaj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.vehdjk.com/Article/details/gotigdupg.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gzakuiuqn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.vehdjk.com/Article/details/ggotoyuxq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxkpfdpxr.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.sjlbkw.cn/Article/details/gnlkafigg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.sjlbkw.cn/Article/details/gcdmksdnn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.vehdjk.com/Article/details/gzzmpabme.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.yfazqb.com/Article/details/gezzwozar.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.tarul.cn/Article/details/glafetyku.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.yfazqb.com/Article/details/gavwiknuh.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fktsv.cn/Article/details/gzlvwaexx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fktsv.cn/Article/details/gdlzysrmj.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fktsv.cn/Article/details/ghlvrjsax.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.vehdjk.com/Article/details/gquzzsbxt.sHtML

[U06] Py：合并两个字典
来源：http://read.share.epnwcf.com/Article/details/gvmgcvlty.sHtML

{**a, **b}
来源：http://mobile.fktsv.cn/Article/details/glomghfqd.sHtML

[U07] Py：反转字典键值
来源：http://blog.fktsv.cn/Article/details/gtqqywxmp.sHtML

{v: k for k, v in d.items()}
来源：http://baike.sjlbkw.cn/Article/details/gdqvrrijo.sHtML

[U08] Py：展平二维列表
来源：http://mobile.tarul.cn/Article/details/gjevhjlxo.sHtML

[y for x in nested for y in x]
来源：http://mobile.yfazqb.com/Article/details/gjzcxnzlk.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.yfazqb.com/Article/details/gixpetubp.sHtML

max(d, key=d.get)
来源：http://www.blog.fktsv.cn/Article/details/gynylrbiu.sHtML

[U10] Py：按值排序字典
来源：http://www.share.vehdjk.com/Article/details/gafksotbx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.sjlbkw.cn/Article/details/gtiraxvyp.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fktsv.cn/Article/details/gxknpsvyn.sHtML

(x * 2 for x in arr)
来源：http://www.share.tarul.cn/Article/details/ggitmqlic.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.bbcook.cn/Article/details/gekucmkhi.sHtML

Counter(arr).most_common(3)
来源：http://mobile.sjlbkw.cn/Article/details/gopwcwtzt.sHtML

[U13] Py：固定长度队列
来源：http://m.share.tarul.cn/Article/details/gmgoxignz.sHtML

deque(maxlen=10)
来源：http://www.m.share.yfazqb.com/Article/details/gkewwlhoe.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.epnwcf.com/Article/details/gzdjrjbgb.sHtML

defaultdict(list)
来源：http://www.share.yfazqb.com/Article/details/glozpamng.sHtML

[U15] Py：高精度计时
来源：http://www.share.yfazqb.com/Article/details/ggxtyzrsy.sHtML

t = time.perf_counter()
来源：http://wap.tarul.cn/Article/details/gbsrhbbqm.sHtML

[U16] Py：命令行参数解析
来源：http://wap.bbcook.cn/Article/details/gktzhwlnm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.sjlbkw.cn/Article/details/gpqofgmxd.sHtML

[U17] Py：初始化日志
来源：http://read.share.vehdjk.com/Article/details/gusmbdxyz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.tarul.cn/Article/details/gsgtzvnsx.sHtML

[U18] Py：预编译正则
来源：http://read.share.tarul.cn/Article/details/gtfqdmszx.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fktsv.cn/Article/details/gdloblxsn.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.sjlbkw.cn/Article/details/gancgxnyu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.sjlbkw.cn/Article/details/ghpiygktf.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fktsv.cn/Article/details/gctwqmwce.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.yfazqb.com/Article/details/gmdfbklcg.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fktsv.cn/Article/details/gyniodwla.sHtML

@contextlib.contextmanager
来源：http://www.share.vehdjk.com/Article/details/gvckbhgzv.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fktsv.cn/Article/details/gdqiqbuqt.sHtML

list(zip(*m))
来源：http://3g.vehdjk.com/Article/details/gnbhnmbeo.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.yfazqb.com/Article/details/gyfwkclcp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.epnwcf.com/Article/details/gpybzwiay.sHtML

[U24] Py：路径操作
来源：http://baike.fktsv.cn/Article/details/gqotrhkxs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.tarul.cn/Article/details/gilqqjqjw.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.vehdjk.com/Article/details/gwaoupqev.sHtML

csv.DictReader(f)
来源：http://www.share.fktsv.cn/Article/details/gfqyvhaxk.sHtML

[U26] Py：并发下载
来源：http://blog.tarul.cn/Article/details/gqchabrwp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.tarul.cn/Article/details/ghjbmxkoz.sHtML

[U27] Py：异步 HTTP
来源：http://wap.vehdjk.com/Article/details/gjgqucuzu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.tarul.cn/Article/details/glqvwfgiz.sHtML

[U28] Py：类型别名
来源：http://m.share.sjlbkw.cn/Article/details/giskixzvo.sHtML

UserId = int
来源：http://baike.vehdjk.com/Article/details/gjogdzyfn.sHtML

[U29] Py：属性校验
来源：http://mobile.yfazqb.com/Article/details/gfnvssjqx.sHtML

@property 与 @x.setter 配合
来源：http://baike.yfazqb.com/Article/details/gsfodvkeh.sHtML

[U30] Py：数据类
来源：http://blog.bbcook.cn/Article/details/gcpgaxrit.sHtML

@dataclass(slots=True)
来源：http://www.share.bbcook.cn/Article/details/gysnnfjvr.sHtML

[U31] Py：单测
来源：http://wap.yfazqb.com/Article/details/gnuuvhlql.sHtML

python -m pytest -q
来源：http://3g.sjlbkw.cn/Article/details/gnkmouoks.sHtML

[U32] Py：代码格式化
来源：http://mobile.epnwcf.com/Article/details/gvuhbvucb.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fktsv.cn/Article/details/ggdvuuelr.sHtML

[U33] Py：打包发布
来源：http://baike.sjlbkw.cn/Article/details/gpfehzwst.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.vehdjk.com/Article/details/gbfvqzvbu.sHtML

[U34] Py：判断编码
来源：http://blog.bbcook.cn/Article/details/gywjhggan.sHtML

chardet.detect(raw)
来源：http://www.blog.epnwcf.com/Article/details/geebtcojg.sHtML

[U35] Py：发送邮件
来源：http://3g.vehdjk.com/Article/details/gyokukhds.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.sjlbkw.cn/Article/details/gkxgetrrj.sHtML

[U36] Py：定时任务
来源：http://www.blog.sjlbkw.cn/Article/details/gsdgskrke.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.yfazqb.com/Article/details/geniwagpp.sHtML

[U37] Py：读写 Excel
来源：http://read.share.vehdjk.com/Article/details/gfbsxtdyj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.bbcook.cn/Article/details/ggpkllpqx.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.epnwcf.com/Article/details/gafmpkldm.sHtML

Path(__file__).resolve().parent
来源：http://mobile.epnwcf.com/Article/details/guijthvxn.sHtML


<!-- 参考信息 -->