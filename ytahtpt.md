代发 wailian999

x |= (1 << 3);
来源：http://baike.vehdjk.com/Article/details/gxtcdhkvv.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gipqgsbfk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.yfazqb.com/Article/details/gyjjzyfel.sHtML

[S18] C：命令行参数
来源：http://www.m.share.tarul.cn/Article/details/gkjlgqgza.sHtML

int main(int argc, char **argv)
来源：http://3g.bbcook.cn/Article/details/gpmmojliz.sHtML

[S19] C：快速排序
来源：http://wap.vehdjk.com/Article/details/gnnhktfkq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/geandvylw.sHtML

[S20] C：二分查找
来源：http://mobile.fktsv.cn/Article/details/gfodjkoai.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gbmtmvtlm.sHtML

[S21] C：字符类别判断
来源：http://baike.fktsv.cn/Article/details/gfldnxton.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.bbcook.cn/Article/details/gibzkcdte.sHtML

[S22] C：字符串转数字
来源：http://blog.yfazqb.com/Article/details/glepztccj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.bbcook.cn/Article/details/gahieiccb.sHtML

[S23] C：随机数
来源：http://read.share.epnwcf.com/Article/details/gywwtijuc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fktsv.cn/Article/details/gyxzpabsm.sHtML

[S24] C：获取本地时间
来源：http://www.blog.sjlbkw.cn/Article/details/gukwavkro.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.tarul.cn/Article/details/gptztkbrx.sHtML

[S25] C：内存拷贝
来源：http://www.share.yfazqb.com/Article/details/gqxmyhkud.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.epnwcf.com/Article/details/gqwrmddry.sHtML

[S26] C：内存清零
来源：http://baike.yfazqb.com/Article/details/goidvoite.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.yfazqb.com/Article/details/gwsvkzqji.sHtML

[S27] C：定义常量
来源：http://www.m.share.sjlbkw.cn/Article/details/gbedvbzue.sHtML

const double PI = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gwsdrobhn.sHtML

[S28] C：静态变量
来源：http://www.blog.fktsv.cn/Article/details/gdjfihlrd.sHtML

static int counter = 0;
来源：http://wap.sjlbkw.cn/Article/details/gfzgtnczx.sHtML

[S29] C：变参函数
来源：http://m.share.epnwcf.com/Article/details/gxceplmmq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.sjlbkw.cn/Article/details/gqlpznihe.sHtML

[S30] C：头文件保护
来源：http://blog.vehdjk.com/Article/details/gvfcgmxkr.sHtML

#ifndef X_H
来源：http://mobile.tarul.cn/Article/details/gbxcjnaot.sHtML

#define X_H
来源：http://www.share.epnwcf.com/Article/details/groztdxbs.sHtML

#endif
来源：http://baike.tarul.cn/Article/details/gctfqomud.sHtML

[S31] C++：Hello World
来源：http://m.share.fktsv.cn/Article/details/gwjcgncql.sHtML

#include <iostream>
来源：http://3g.vehdjk.com/Article/details/gfotzpkrr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.tarul.cn/Article/details/gqwvzsdsk.sHtML

[S32] C++：字符串
来源：http://wap.tarul.cn/Article/details/gfhbalxgr.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fktsv.cn/Article/details/goswndokc.sHtML

[S33] C++：vector 增删
来源：http://blog.fktsv.cn/Article/details/gzxjfutvr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.tarul.cn/Article/details/gdflbbpio.sHtML

[S34] C++：遍历 vector
来源：http://3g.tarul.cn/Article/details/glodsficn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.tarul.cn/Article/details/gbrocvasr.sHtML

[S35] C++：map
来源：http://www.m.share.tarul.cn/Article/details/gevyiatkq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.tarul.cn/Article/details/gyqzdmzrv.sHtML

[S36] C++：unordered_map
来源：http://baike.bbcook.cn/Article/details/gtpgjcvwm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gqgkzeeby.sHtML

[S37] C++：set
来源：http://blog.epnwcf.com/Article/details/gavextdqu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.tarul.cn/Article/details/gyxgcmgny.sHtML

[S38] C++：排序
来源：http://www.blog.sjlbkw.cn/Article/details/gywhyhjpm.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.vehdjk.com/Article/details/gkjrollpy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.vehdjk.com/Article/details/gmfixclrc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.vehdjk.com/Article/details/gzdctcnzx.sHtML

[S40] C++：查找元素
来源：http://m.share.bbcook.cn/Article/details/gcwqcteqe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fktsv.cn/Article/details/gtwozyhja.sHtML

[S41] C++：类与构造函数
来源：http://baike.tarul.cn/Article/details/gbdcnmgog.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fktsv.cn/Article/details/golqtbvsq.sHtML

[S42] C++：继承与虚函数
来源：http://baike.epnwcf.com/Article/details/gvdbtjmpi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fktsv.cn/Article/details/gmxltpjnt.sHtML

[S43] C++：智能指针
来源：http://mobile.bbcook.cn/Article/details/gsxnvjwzo.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.sjlbkw.cn/Article/details/gacpordhp.sHtML

[S44] C++：引用传参
来源：http://baike.yfazqb.com/Article/details/gikqhknor.sHtML

void inc(int &x) { ++x; }
来源：http://3g.sjlbkw.cn/Article/details/gyiyvygfq.sHtML

[S45] C++：lambda
来源：http://www.blog.bbcook.cn/Article/details/gjqfununq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.sjlbkw.cn/Article/details/gipywhrlt.sHtML

[S46] C++：函数模板
来源：http://www.share.tarul.cn/Article/details/giiayjdxt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.bbcook.cn/Article/details/gahviamev.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.bbcook.cn/Article/details/gscmpfpgo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fktsv.cn/Article/details/givxspmwk.sHtML

[S48] C++：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gwymnmaty.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fktsv.cn/Article/details/gfcxdgrva.sHtML

while (std::getline(in, line)) { }
来源：http://baike.tarul.cn/Article/details/guefwcdut.sHtML

[S49] C++：写文件
来源：http://m.share.epnwcf.com/Article/details/gukppqswg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fktsv.cn/Article/details/ghmnadurw.sHtML

[S50] C++：格式化数字
来源：http://3g.yfazqb.com/Article/details/guisoaexc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.tarul.cn/Article/details/grkfzlpvt.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fktsv.cn/Article/details/gjkbiaakk.sHtML

static_cast<double>(a) / b
来源：http://www.blog.epnwcf.com/Article/details/gaadjamny.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.tarul.cn/Article/details/ghripojfz.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.sjlbkw.cn/Article/details/gduomenvq.sHtML

[S53] C++：移动语义
来源：http://baike.epnwcf.com/Article/details/gulxqqqwz.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.bbcook.cn/Article/details/goydnbdao.sHtML

[S54] C++：异常处理
来源：http://www.share.bbcook.cn/Article/details/gwljfszoz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.sjlbkw.cn/Article/details/gqnwtebww.sHtML

[S55] C++：结构化绑定
来源：http://read.share.epnwcf.com/Article/details/gxunxdnam.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.sjlbkw.cn/Article/details/gzecfmvnw.sHtML

[S56] C++：optional
来源：http://www.share.epnwcf.com/Article/details/gxwdvywjm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fktsv.cn/Article/details/glngsojuc.sHtML

[S57] C++：编译期常量
来源：http://read.share.fktsv.cn/Article/details/gkafpeidr.sHtML

constexpr int N = 10;
来源：http://baike.epnwcf.com/Article/details/gcwcceypt.sHtML

[S58] C++：命名空间
来源：http://www.share.yfazqb.com/Article/details/gibeoncfv.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.vehdjk.com/Article/details/gllwwrygl.sHtML

[S59] C++：静态断言
来源：http://3g.yfazqb.com/Article/details/gyywggfwv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.vehdjk.com/Article/details/gzoekxwcy.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.yfazqb.com/Article/details/gltbgnuqd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.tarul.cn/Article/details/gmumbkqck.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gpejvhhpg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.sjlbkw.cn/Article/details/gneyotlol.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gizszmvkt.sHtML

[T01] Kotlin：Hello World
来源：http://blog.tarul.cn/Article/details/goioldxpa.sHtML

println("Hello")
来源：http://baike.tarul.cn/Article/details/gooafculm.sHtML

[T02] Kotlin：变量
来源：http://www.blog.bbcook.cn/Article/details/gewgaxvgl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.sjlbkw.cn/Article/details/gvnqnbvnm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.epnwcf.com/Article/details/gilgrogou.sHtML

"值: $b"
来源：http://m.share.tarul.cn/Article/details/guyybfquf.sHtML

[T04] Kotlin：空安全
来源：http://www.share.vehdjk.com/Article/details/gigdqjvnq.sHtML

val n: String? = null;  n?.length
来源：http://m.share.vehdjk.com/Article/details/gsphgmopa.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.bbcook.cn/Article/details/gsjroeoki.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.vehdjk.com/Article/details/gnjqeemsq.sHtML

[T06] Kotlin：集合映射
来源：http://baike.sjlbkw.cn/Article/details/gllooxvtr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.bbcook.cn/Article/details/ghscrmghp.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.yfazqb.com/Article/details/gdqpunddr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.tarul.cn/Article/details/ghzohoalx.sHtML

[T08] Kotlin：数据类
来源：http://read.share.tarul.cn/Article/details/govynvoea.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fktsv.cn/Article/details/gxxvfxkvi.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.sjlbkw.cn/Article/details/gynbdbdtj.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.vehdjk.com/Article/details/gybarakve.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.yfazqb.com/Article/details/gprtryjdk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.yfazqb.com/Article/details/gwybdlerg.sHtML

[T11] Kotlin：协程
来源：http://baike.tarul.cn/Article/details/gnsygvcrl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.sjlbkw.cn/Article/details/gjzsosabo.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.sjlbkw.cn/Article/details/grqvxkzpn.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gynszxcot.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.tarul.cn/Article/details/gbpzemcdx.sHtML

val m = mapOf("a" to 1)
来源：http://baike.vehdjk.com/Article/details/gfsasueik.sHtML

[T14] Kotlin：循环
来源：http://www.share.yfazqb.com/Article/details/gvsfdaqpn.sHtML

for (i in 1..10) println(i)
来源：http://m.share.tarul.cn/Article/details/ggyiiyeol.sHtML

[T15] Kotlin：接口
来源：http://wap.bbcook.cn/Article/details/ggocolxsw.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.vehdjk.com/Article/details/gqxrtghfj.sHtML

[T16] Swift：Hello World
来源：http://wap.fktsv.cn/Article/details/gajomcsdg.sHtML

print("Hello")
来源：http://wap.sjlbkw.cn/Article/details/geiidvpxd.sHtML

[T17] Swift：变量与常量
来源：http://3g.tarul.cn/Article/details/gtkvvxjbj.sHtML

var a = 1;  let b = 2
来源：http://read.share.vehdjk.com/Article/details/gbwgdasgq.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gsnthlgac.sHtML

"值: \(b)"
来源：http://www.share.yfazqb.com/Article/details/gmxmfzwyc.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fktsv.cn/Article/details/gknqyjwms.sHtML

if let n = opt { print(n) }
来源：http://baike.tarul.cn/Article/details/gmhdrtuii.sHtML

[T20] Swift：数组操作
来源：http://mobile.bbcook.cn/Article/details/gouzrusvx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.sjlbkw.cn/Article/details/gfcfcooyu.sHtML

[T21] Swift：遍历
来源：http://baike.vehdjk.com/Article/details/genopgkwe.sHtML

for x in a { print(x) }
来源：http://www.blog.vehdjk.com/Article/details/gmejrghmd.sHtML

[T22] Swift：字典
来源：http://www.m.share.yfazqb.com/Article/details/gqixbbnjm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.tarul.cn/Article/details/gltprgtjl.sHtML

[T23] Swift：函数
来源：http://3g.fktsv.cn/Article/details/gbmpfowui.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fktsv.cn/Article/details/gwwuczkpc.sHtML

[T24] Swift：闭包
来源：http://www.blog.vehdjk.com/Article/details/gfutbzpzr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.tarul.cn/Article/details/gcbjysjjq.sHtML

[T25] Swift：结构体
来源：http://baike.tarul.cn/Article/details/guebstzbb.sHtML

struct P { var x: Int }
来源：http://www.share.tarul.cn/Article/details/gyjklhplz.sHtML

[T26] Swift：类与重写
来源：http://m.share.bbcook.cn/Article/details/gqhzgtvxl.sHtML

class A: Base { override func f() {} }
来源：http://baike.tarul.cn/Article/details/ghooesiht.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fktsv.cn/Article/details/ghnlxhnrz.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fktsv.cn/Article/details/gzryqmlob.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fktsv.cn/Article/details/gkqnkzzfh.sHtML

enum Color { case red, green }
来源：http://www.share.vehdjk.com/Article/details/gnmocryds.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.bbcook.cn/Article/details/gklfqbaou.sHtML

guard let x = opt else { return }
来源：http://m.share.fktsv.cn/Article/details/gnzebeclo.sHtML

[T30] Swift：协议
来源：http://wap.bbcook.cn/Article/details/gyuasbcht.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.vehdjk.com/Article/details/gvbzqjrvf.sHtML

[T31] Lua：Hello World
来源：http://read.share.fktsv.cn/Article/details/grbbyfiaf.sHtML

print("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/gsdiuiiwv.sHtML

[T32] Lua：局部变量
来源：http://blog.sjlbkw.cn/Article/details/gljiqtluv.sHtML

local a = 1
来源：http://read.share.yfazqb.com/Article/details/gqncdluvz.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.tarul.cn/Article/details/gnskbewde.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.tarul.cn/Article/details/gkzmwfaoj.sHtML

[T34] Lua：遍历表
来源：http://m.share.sjlbkw.cn/Article/details/grrtfymmj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.vehdjk.com/Article/details/gwuasrmrz.sHtML

[T35] Lua：字典表
来源：http://www.blog.yfazqb.com/Article/details/gtagbnarz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.bbcook.cn/Article/details/grwfduxwv.sHtML

[T36] Lua：函数
来源：http://read.share.yfazqb.com/Article/details/gdfmbuncb.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.vehdjk.com/Article/details/gftdwniel.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.vehdjk.com/Article/details/gnilotulx.sHtML

"a" .. "b"
来源：http://blog.yfazqb.com/Article/details/gqayuzcks.sHtML

[T38] Lua：条件
来源：http://www.blog.bbcook.cn/Article/details/gyjgeimdd.sHtML

if x > 0 then print("正") end
来源：http://blog.fktsv.cn/Article/details/gwcbfacyt.sHtML

[T39] Lua：模式匹配
来源：http://baike.yfazqb.com/Article/details/gfjyyrael.sHtML

string.find(s, "%d+")
来源：http://blog.fktsv.cn/Article/details/grdbvblty.sHtML

[T40] Lua：元表
来源：http://m.share.yfazqb.com/Article/details/gviyuupxi.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fktsv.cn/Article/details/gudbmbvej.sHtML

[T41] Perl：Hello World
来源：http://m.share.vehdjk.com/Article/details/gwoxvtfgb.sHtML

print "Hello\n";
来源：http://www.blog.yfazqb.com/Article/details/ggsjtdyzl.sHtML

[T42] Perl：变量类型
来源：http://www.blog.tarul.cn/Article/details/gmjpnbqsj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.epnwcf.com/Article/details/gwyymzpxs.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gbjjyhmnc.sHtML

"值: $a"
来源：http://3g.fktsv.cn/Article/details/gilkqpafm.sHtML

[T44] Perl：条件
来源：http://www.blog.epnwcf.com/Article/details/gdtqgiivn.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.tarul.cn/Article/details/gcysrttup.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.epnwcf.com/Article/details/gavnwmlgi.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.tarul.cn/Article/details/gbfiwqnrb.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.vehdjk.com/Article/details/gczkybcll.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.tarul.cn/Article/details/gvmiiczgb.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fktsv.cn/Article/details/gbyxfhsfq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.sjlbkw.cn/Article/details/gpdwznoow.sHtML

[T48] Perl：正则替换
来源：http://blog.bbcook.cn/Article/details/gwjmllzzn.sHtML

$s =~ s/old/new/g;
来源：http://baike.bbcook.cn/Article/details/gwcdznszu.sHtML

[T49] Perl：函数
来源：http://mobile.vehdjk.com/Article/details/gllmfxwha.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gioqorybc.sHtML

[T50] Perl：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gjtmjktnh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.tarul.cn/Article/details/glswhfjsu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.vehdjk.com/Article/details/gavxupcok.sHtML

[T51] Scala：Hello World
来源：http://baike.fktsv.cn/Article/details/gmimmdgpr.sHtML

println("Hello")
来源：http://mobile.vehdjk.com/Article/details/gjriwrsll.sHtML

[T52] Scala：变量
来源：http://www.m.share.yfazqb.com/Article/details/gknmjcnzg.sHtML

val a = 1;  var b = 2
来源：http://mobile.vehdjk.com/Article/details/gpblrazbw.sHtML

[T53] Scala：字符串插值
来源：http://wap.yfazqb.com/Article/details/gkatrcqry.sHtML

s"值: $b"
来源：http://m.share.fktsv.cn/Article/details/gjgpepvmi.sHtML

[T54] Scala：集合映射
来源：http://wap.epnwcf.com/Article/details/gbbkkrarr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gyrbikgus.sHtML

[T55] Scala：集合过滤
来源：http://read.share.vehdjk.com/Article/details/gaybsirnv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpzrdycw.sHtML

[T56] Scala：样例类
来源：http://baike.fktsv.cn/Article/details/gkbrsbaxq.sHtML

case class User(name: String, age: Int)
来源：http://read.share.sjlbkw.cn/Article/details/gdjjlpvcs.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.epnwcf.com/Article/details/ggiefaavd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.sjlbkw.cn/Article/details/gwbjeryct.sHtML

[T58] Scala：函数定义
来源：http://baike.tarul.cn/Article/details/gctrlorsu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.tarul.cn/Article/details/gqvrdoqym.sHtML

[T59] Scala：循环
来源：http://www.blog.yfazqb.com/Article/details/gnquzafpd.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.vehdjk.com/Article/details/gelfvafpj.sHtML

[T60] Scala：折叠
来源：http://mobile.epnwcf.com/Article/details/gttelwmwz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.tarul.cn/Article/details/ghnxicgmk.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gkbkgtdqj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.epnwcf.com/Article/details/ggnmgsojj.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gdfteiawz.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fktsv.cn/Article/details/govdtraoa.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.vehdjk.com/Article/details/geyglrazg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.vehdjk.com/Article/details/guvvkcxjb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.epnwcf.com/Article/details/gsjigiqqq.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fktsv.cn/Article/details/gxmuehozy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.epnwcf.com/Article/details/ghicwyffb.sHtML

[U04] Py：变量调试打印
来源：http://read.share.vehdjk.com/Article/details/gfpsphwht.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.epnwcf.com/Article/details/glmodhjda.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.tarul.cn/Article/details/gksggkyxh.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.vehdjk.com/Article/details/giomqegbg.sHtML

[U06] Py：合并两个字典
来源：http://blog.tarul.cn/Article/details/grjipvosg.sHtML

{**a, **b}
来源：http://baike.vehdjk.com/Article/details/gkizpchep.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.bbcook.cn/Article/details/gacmubtwr.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.vehdjk.com/Article/details/gufgsekzl.sHtML

[U08] Py：展平二维列表
来源：http://m.share.tarul.cn/Article/details/gudchyhsx.sHtML

[y for x in nested for y in x]
来源：http://blog.tarul.cn/Article/details/gtxutvtnx.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.yfazqb.com/Article/details/gywcmjvpd.sHtML

max(d, key=d.get)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqcedxpsd.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.vehdjk.com/Article/details/gfenygljm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.epnwcf.com/Article/details/gdlechtfc.sHtML

[U11] Py：生成器表达式
来源：http://wap.vehdjk.com/Article/details/grmpjnhpn.sHtML

(x * 2 for x in arr)
来源：http://wap.yfazqb.com/Article/details/gpzoaerkp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.epnwcf.com/Article/details/gagcbxtzh.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gtuyvhlim.sHtML

[U13] Py：固定长度队列
来源：http://wap.vehdjk.com/Article/details/gnmxlxfqk.sHtML

deque(maxlen=10)
来源：http://wap.sjlbkw.cn/Article/details/gyiqwkayq.sHtML

[U14] Py：分组收集到列表
来源：http://blog.bbcook.cn/Article/details/gfgpulzxz.sHtML

defaultdict(list)
来源：http://read.share.bbcook.cn/Article/details/gidvssxck.sHtML

[U15] Py：高精度计时
来源：http://baike.vehdjk.com/Article/details/gasckqxbt.sHtML

t = time.perf_counter()
来源：http://mobile.vehdjk.com/Article/details/ghmpjtncf.sHtML

[U16] Py：命令行参数解析
来源：http://blog.tarul.cn/Article/details/gxsorsrcv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fktsv.cn/Article/details/gymmlrbtx.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.bbcook.cn/Article/details/guljqvltt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.yfazqb.com/Article/details/ggrrnifef.sHtML

[U18] Py：预编译正则
来源：http://www.blog.yfazqb.com/Article/details/gjpkajbss.sHtML

pat = re.compile(r"\d+")
来源：http://blog.sjlbkw.cn/Article/details/gwjrprprw.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.yfazqb.com/Article/details/gyejubyfk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fktsv.cn/Article/details/goxbsusdz.sHtML

[U20] Py：缓存函数结果
来源：http://3g.epnwcf.com/Article/details/gflkysowy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.vehdjk.com/Article/details/gkvorfbtb.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.yfazqb.com/Article/details/gdyimrpnv.sHtML

@contextlib.contextmanager
来源：http://wap.bbcook.cn/Article/details/gpwpyevwe.sHtML

[U22] Py：矩阵转置
来源：http://www.share.bbcook.cn/Article/details/gyryjxhjz.sHtML

list(zip(*m))
来源：http://www.share.epnwcf.com/Article/details/gmfzxpgij.sHtML

[U23] Py：分块读取大文件
来源：http://3g.yfazqb.com/Article/details/gohhyxmnq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.yfazqb.com/Article/details/gxpkjvdyb.sHtML

[U24] Py：路径操作
来源：http://www.share.bbcook.cn/Article/details/gqhptoouw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.bbcook.cn/Article/details/gvmdwajyp.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.sjlbkw.cn/Article/details/ggbuxxfov.sHtML

csv.DictReader(f)
来源：http://www.share.fktsv.cn/Article/details/gkfcmtexn.sHtML

[U26] Py：并发下载
来源：http://m.share.fktsv.cn/Article/details/gwypczsts.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.sjlbkw.cn/Article/details/gdsmyhyal.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.epnwcf.com/Article/details/gaqzhzqmd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.yfazqb.com/Article/details/gwnybsprm.sHtML

[U28] Py：类型别名
来源：http://mobile.epnwcf.com/Article/details/gdnncckny.sHtML

UserId = int
来源：http://blog.sjlbkw.cn/Article/details/ghdukweuq.sHtML

[U29] Py：属性校验
来源：http://read.share.epnwcf.com/Article/details/gzxwaahwo.sHtML

@property 与 @x.setter 配合
来源：http://blog.yfazqb.com/Article/details/gwuedrgrs.sHtML

[U30] Py：数据类
来源：http://www.blog.epnwcf.com/Article/details/gnabtydum.sHtML

@dataclass(slots=True)
来源：http://www.blog.tarul.cn/Article/details/ghhxadzke.sHtML

[U31] Py：单测
来源：http://baike.epnwcf.com/Article/details/gzvdbjfbe.sHtML

python -m pytest -q
来源：http://3g.epnwcf.com/Article/details/gmenjmgqw.sHtML

[U32] Py：代码格式化
来源：http://blog.fktsv.cn/Article/details/ggqsehvfj.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.tarul.cn/Article/details/gnfhhxfer.sHtML

[U33] Py：打包发布
来源：http://baike.vehdjk.com/Article/details/goehhsgbc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.yfazqb.com/Article/details/gdtbgetaw.sHtML

[U34] Py：判断编码
来源：http://blog.bbcook.cn/Article/details/gmyediohi.sHtML

chardet.detect(raw)
来源：http://mobile.tarul.cn/Article/details/gdmqwtugj.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.vehdjk.com/Article/details/gmcbzbwps.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.vehdjk.com/Article/details/guqzzfyum.sHtML

[U36] Py：定时任务
来源：http://baike.vehdjk.com/Article/details/geclasaod.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.sjlbkw.cn/Article/details/ggzanuuqt.sHtML

[U37] Py：读写 Excel
来源：http://3g.tarul.cn/Article/details/gvstoisnj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.bbcook.cn/Article/details/gyiynjsno.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.bbcook.cn/Article/details/goqzqjotx.sHtML

Path(__file__).resolve().parent
来源：http://wap.tarul.cn/Article/details/guzlcmnee.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.tarul.cn/Article/details/gespwwmmn.sHtML

sys.stdout.isatty()
来源：http://wap.bbcook.cn/Article/details/gvdznvzcy.sHtML

[U40] Py：打印到标准错误
来源：http://blog.yfazqb.com/Article/details/gsncvrovg.sHtML

print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gahgyhzeg.sHtML


<!-- 参考信息 -->