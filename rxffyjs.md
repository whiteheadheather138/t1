代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://3g.tarul.cn/Article/details/gquxdygma.sHtML

[S15] C：类型转换
来源：http://baike.vehdjk.com/Article/details/gidbqbuyd.sHtML

(double) a / b
来源：http://www.share.tarul.cn/Article/details/ginuyogcf.sHtML

[S16] C：位操作置位
来源：http://www.share.sjlbkw.cn/Article/details/gbuxgkpoo.sHtML

x |= (1 << 3);
来源：http://www.share.vehdjk.com/Article/details/govisnemg.sHtML

[S17] C：安全拼接字符串
来源：http://blog.bbcook.cn/Article/details/gtivatcmt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fktsv.cn/Article/details/gxthmcegc.sHtML

[S18] C：命令行参数
来源：http://m.share.vehdjk.com/Article/details/gtsufzefi.sHtML

int main(int argc, char **argv)
来源：http://www.share.bbcook.cn/Article/details/gbwjmkaac.sHtML

[S19] C：快速排序
来源：http://wap.bbcook.cn/Article/details/ggjrljlpj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/gklgydqew.sHtML

[S20] C：二分查找
来源：http://3g.fktsv.cn/Article/details/gzldgowhz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.vehdjk.com/Article/details/gxzzqxmpj.sHtML

[S21] C：字符类别判断
来源：http://blog.bbcook.cn/Article/details/gsrmxipie.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fktsv.cn/Article/details/gtcipjtqm.sHtML

[S22] C：字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gckqjxmwm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.bbcook.cn/Article/details/gbapwvccx.sHtML

[S23] C：随机数
来源：http://blog.vehdjk.com/Article/details/gmxenfvrz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.tarul.cn/Article/details/ghfrrherc.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.epnwcf.com/Article/details/gazjbapqi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.bbcook.cn/Article/details/gvoyjzntu.sHtML

[S25] C：内存拷贝
来源：http://3g.bbcook.cn/Article/details/guwcrjvfd.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fktsv.cn/Article/details/goxfvevyb.sHtML

[S26] C：内存清零
来源：http://www.blog.epnwcf.com/Article/details/gbasmtgrf.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.yfazqb.com/Article/details/gwkhilcnp.sHtML

[S27] C：定义常量
来源：http://wap.sjlbkw.cn/Article/details/gmzwiwbvu.sHtML

const double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gkebrpnil.sHtML

[S28] C：静态变量
来源：http://www.share.tarul.cn/Article/details/gvyxxvbra.sHtML

static int counter = 0;
来源：http://m.share.epnwcf.com/Article/details/gjitdnqjk.sHtML

[S29] C：变参函数
来源：http://mobile.yfazqb.com/Article/details/gvvdepmtn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fktsv.cn/Article/details/gemgnyait.sHtML

[S30] C：头文件保护
来源：http://baike.sjlbkw.cn/Article/details/gvgyyndrq.sHtML

#ifndef X_H
来源：http://3g.epnwcf.com/Article/details/gmsocqptz.sHtML

#define X_H
来源：http://read.share.vehdjk.com/Article/details/gxxixgsta.sHtML

#endif
来源：http://www.m.share.yfazqb.com/Article/details/gldetsbyv.sHtML

[S31] C++：Hello World
来源：http://read.share.fktsv.cn/Article/details/gwzjxixjq.sHtML

#include <iostream>
来源：http://baike.vehdjk.com/Article/details/gacmtsdwd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.vehdjk.com/Article/details/gfkzmraif.sHtML

[S32] C++：字符串
来源：http://read.share.tarul.cn/Article/details/gfpdmhnsy.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.tarul.cn/Article/details/grnvyshut.sHtML

[S33] C++：vector 增删
来源：http://baike.fktsv.cn/Article/details/ggyufcrkr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.sjlbkw.cn/Article/details/gnqdjkgqz.sHtML

[S34] C++：遍历 vector
来源：http://baike.yfazqb.com/Article/details/gibudwyyy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fktsv.cn/Article/details/gktmjbbkm.sHtML

[S35] C++：map
来源：http://mobile.bbcook.cn/Article/details/ggwzikint.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.tarul.cn/Article/details/glhaxtwfr.sHtML

[S36] C++：unordered_map
来源：http://read.share.tarul.cn/Article/details/gcfrtsqiw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fktsv.cn/Article/details/ggujnnqmd.sHtML

[S37] C++：set
来源：http://www.share.epnwcf.com/Article/details/ggrqovgmx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.tarul.cn/Article/details/gytdegkwc.sHtML

[S38] C++：排序
来源：http://mobile.yfazqb.com/Article/details/gpwmoarqj.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.yfazqb.com/Article/details/gyjdmofbm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.yfazqb.com/Article/details/grnwyfrnt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fktsv.cn/Article/details/gazvuevjm.sHtML

[S40] C++：查找元素
来源：http://3g.yfazqb.com/Article/details/gaxzneonq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.bbcook.cn/Article/details/gimubsufj.sHtML

[S41] C++：类与构造函数
来源：http://www.share.epnwcf.com/Article/details/gzaizdwxl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.yfazqb.com/Article/details/gnneohfbt.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fktsv.cn/Article/details/gmagaliax.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.vehdjk.com/Article/details/gwkajsglk.sHtML

[S43] C++：智能指针
来源：http://baike.tarul.cn/Article/details/gqqwfemca.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.vehdjk.com/Article/details/ghahmakjm.sHtML

[S44] C++：引用传参
来源：http://3g.fktsv.cn/Article/details/gmwbplyqt.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.sjlbkw.cn/Article/details/ghkadhyec.sHtML

[S45] C++：lambda
来源：http://www.m.share.tarul.cn/Article/details/gsnvfocnk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.yfazqb.com/Article/details/gzrpxiasg.sHtML

[S46] C++：函数模板
来源：http://baike.epnwcf.com/Article/details/gtjvqclcm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.vehdjk.com/Article/details/gfwedbbfs.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fktsv.cn/Article/details/gkrughpsi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.bbcook.cn/Article/details/gfjocicbs.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gdnrtsepw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.vehdjk.com/Article/details/gwbhlsyih.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.vehdjk.com/Article/details/gkmdifsfd.sHtML

[S49] C++：写文件
来源：http://baike.tarul.cn/Article/details/goupmamzr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fktsv.cn/Article/details/ghdyylrtm.sHtML

[S50] C++：格式化数字
来源：http://www.blog.yfazqb.com/Article/details/gycqqnzju.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gcljtbebc.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/gunwkbgol.sHtML

static_cast<double>(a) / b
来源：http://wap.fktsv.cn/Article/details/gelnquuxh.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.yfazqb.com/Article/details/glxcyglwg.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.bbcook.cn/Article/details/gxgciqtua.sHtML

[S53] C++：移动语义
来源：http://read.share.tarul.cn/Article/details/gytopspew.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.yfazqb.com/Article/details/gbvfmsmgs.sHtML

[S54] C++：异常处理
来源：http://blog.fktsv.cn/Article/details/glwscpnkd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.tarul.cn/Article/details/gdrihxvjs.sHtML

[S55] C++：结构化绑定
来源：http://baike.sjlbkw.cn/Article/details/gmdyhautm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.yfazqb.com/Article/details/gscvjihnt.sHtML

[S56] C++：optional
来源：http://mobile.bbcook.cn/Article/details/gprxmpdoo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.tarul.cn/Article/details/gxpribbko.sHtML

[S57] C++：编译期常量
来源：http://m.share.epnwcf.com/Article/details/gievwssyz.sHtML

constexpr int N = 10;
来源：http://mobile.bbcook.cn/Article/details/gbzajdfjd.sHtML

[S58] C++：命名空间
来源：http://www.share.tarul.cn/Article/details/gqqsddrih.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.epnwcf.com/Article/details/gplhmnzel.sHtML

[S59] C++：静态断言
来源：http://3g.tarul.cn/Article/details/gwxvxtcxf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fktsv.cn/Article/details/gxetscioj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fktsv.cn/Article/details/gmjsznpzo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/giolvtdpw.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gjykyxngt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.yfazqb.com/Article/details/gzdybqesx.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gogoqzxsc.sHtML

[T01] Kotlin：Hello World
来源：http://blog.epnwcf.com/Article/details/gowzvupfj.sHtML

println("Hello")
来源：http://blog.epnwcf.com/Article/details/guzzfmwpi.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/gcpaucikl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.sjlbkw.cn/Article/details/gywyambvz.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fktsv.cn/Article/details/gbjoqvqyf.sHtML

"值: $b"
来源：http://mobile.fktsv.cn/Article/details/gnonulvrj.sHtML

[T04] Kotlin：空安全
来源：http://blog.vehdjk.com/Article/details/ghfxtvdck.sHtML

val n: String? = null;  n?.length
来源：http://baike.bbcook.cn/Article/details/ggiiksxco.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.epnwcf.com/Article/details/gfeahihyw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.vehdjk.com/Article/details/gsilucaoi.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.yfazqb.com/Article/details/gdvwmyiqq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.bbcook.cn/Article/details/ghvtitfzi.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.bbcook.cn/Article/details/gygczbhwo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.yfazqb.com/Article/details/gcwowoldx.sHtML

[T08] Kotlin：数据类
来源：http://blog.fktsv.cn/Article/details/gjnkxxjtg.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.sjlbkw.cn/Article/details/gflxdupeg.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.sjlbkw.cn/Article/details/gasklkwdf.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.epnwcf.com/Article/details/gsfzisiwk.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.vehdjk.com/Article/details/ghcndzdgg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.vehdjk.com/Article/details/gwdaoybbl.sHtML

[T11] Kotlin：协程
来源：http://baike.yfazqb.com/Article/details/gxocdghth.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.vehdjk.com/Article/details/goxcpuqme.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.vehdjk.com/Article/details/gcujriito.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.tarul.cn/Article/details/gqkrbkoie.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.yfazqb.com/Article/details/gtslvrrxs.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.yfazqb.com/Article/details/gmlzbwtxy.sHtML

[T14] Kotlin：循环
来源：http://www.blog.sjlbkw.cn/Article/details/gmqprucxg.sHtML

for (i in 1..10) println(i)
来源：http://blog.fktsv.cn/Article/details/gmazihfew.sHtML

[T15] Kotlin：接口
来源：http://3g.tarul.cn/Article/details/gkwptpxis.sHtML

interface Shape { fun area(): Double }
来源：http://wap.bbcook.cn/Article/details/gqtovvmbu.sHtML

[T16] Swift：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gvvbxazap.sHtML

print("Hello")
来源：http://wap.tarul.cn/Article/details/gvnyjldod.sHtML

[T17] Swift：变量与常量
来源：http://blog.epnwcf.com/Article/details/gujhnpgwn.sHtML

var a = 1;  let b = 2
来源：http://baike.epnwcf.com/Article/details/ghlmxfdbx.sHtML

[T18] Swift：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gizmaesuc.sHtML

"值: \(b)"
来源：http://wap.bbcook.cn/Article/details/gbpkbbebe.sHtML

[T19] Swift：可选绑定
来源：http://3g.bbcook.cn/Article/details/gqffnclag.sHtML

if let n = opt { print(n) }
来源：http://www.blog.yfazqb.com/Article/details/gaibmikva.sHtML

[T20] Swift：数组操作
来源：http://www.blog.sjlbkw.cn/Article/details/gsljyzeri.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fktsv.cn/Article/details/gjzycuyyv.sHtML

[T21] Swift：遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gbgjoqnik.sHtML

for x in a { print(x) }
来源：http://www.blog.bbcook.cn/Article/details/gzyvbwygf.sHtML

[T22] Swift：字典
来源：http://www.blog.epnwcf.com/Article/details/grlmizksw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.epnwcf.com/Article/details/gtayehzep.sHtML

[T23] Swift：函数
来源：http://m.share.yfazqb.com/Article/details/gcihjngjt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.vehdjk.com/Article/details/guztfcawm.sHtML

[T24] Swift：闭包
来源：http://mobile.tarul.cn/Article/details/gngjuqdwq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fktsv.cn/Article/details/gwmakbluv.sHtML

[T25] Swift：结构体
来源：http://wap.tarul.cn/Article/details/giizwlbma.sHtML

struct P { var x: Int }
来源：http://3g.bbcook.cn/Article/details/gmbcsvcfp.sHtML

[T26] Swift：类与重写
来源：http://baike.yfazqb.com/Article/details/gqbaqmrrj.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fktsv.cn/Article/details/gewgrraye.sHtML

[T27] Swift：错误处理
来源：http://wap.vehdjk.com/Article/details/gzvdfsxiw.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.sjlbkw.cn/Article/details/guzlirzps.sHtML

[T28] Swift：枚举
来源：http://www.share.yfazqb.com/Article/details/gfvhsibqn.sHtML

enum Color { case red, green }
来源：http://wap.vehdjk.com/Article/details/geosmjnsq.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.bbcook.cn/Article/details/gxtvulxgf.sHtML

guard let x = opt else { return }
来源：http://3g.bbcook.cn/Article/details/gzvzauwye.sHtML

[T30] Swift：协议
来源：http://3g.fktsv.cn/Article/details/ghbnenonv.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.bbcook.cn/Article/details/grnvclcfo.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gsoveoixw.sHtML

print("Hello")
来源：http://www.share.tarul.cn/Article/details/grgujjaig.sHtML

[T32] Lua：局部变量
来源：http://baike.tarul.cn/Article/details/giydvqkyv.sHtML

local a = 1
来源：http://www.m.share.epnwcf.com/Article/details/ghtipohpe.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.vehdjk.com/Article/details/gokdnftpq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fktsv.cn/Article/details/glhhvoebr.sHtML

[T34] Lua：遍历表
来源：http://wap.yfazqb.com/Article/details/gncckapix.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.sjlbkw.cn/Article/details/gprpclvjx.sHtML

[T35] Lua：字典表
来源：http://www.blog.tarul.cn/Article/details/gepmuhwjm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.yfazqb.com/Article/details/gofbcwrfl.sHtML

[T36] Lua：函数
来源：http://read.share.tarul.cn/Article/details/gekytzedz.sHtML

function add(a, b) return a + b end
来源：http://baike.epnwcf.com/Article/details/gdygzpydc.sHtML

[T37] Lua：字符串拼接
来源：http://blog.bbcook.cn/Article/details/gsdrnmpzo.sHtML

"a" .. "b"
来源：http://www.m.share.yfazqb.com/Article/details/gbzyqlkks.sHtML

[T38] Lua：条件
来源：http://baike.epnwcf.com/Article/details/gqbulbtvy.sHtML

if x > 0 then print("正") end
来源：http://mobile.bbcook.cn/Article/details/gtksmkhlt.sHtML

[T39] Lua：模式匹配
来源：http://blog.bbcook.cn/Article/details/gxvvxbifl.sHtML

string.find(s, "%d+")
来源：http://blog.tarul.cn/Article/details/geqyunnpq.sHtML

[T40] Lua：元表
来源：http://m.share.tarul.cn/Article/details/gtgusksgy.sHtML

setmetatable({}, { __index = base })
来源：http://3g.sjlbkw.cn/Article/details/gwylnzipt.sHtML

[T41] Perl：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gskzwsjmz.sHtML

print "Hello\n";
来源：http://www.blog.epnwcf.com/Article/details/gqllwmmws.sHtML

[T42] Perl：变量类型
来源：http://www.share.yfazqb.com/Article/details/gfazwybzb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.epnwcf.com/Article/details/gbmdndhxn.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gqdevodln.sHtML

"值: $a"
来源：http://mobile.yfazqb.com/Article/details/gpslarrwn.sHtML

[T44] Perl：条件
来源：http://www.blog.tarul.cn/Article/details/gbebqsqcx.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.vehdjk.com/Article/details/gxcxghdvq.sHtML

[T45] Perl：数组遍历
来源：http://3g.fktsv.cn/Article/details/gzokuqmyh.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.tarul.cn/Article/details/gccifucoq.sHtML

[T46] Perl：哈希操作
来源：http://blog.bbcook.cn/Article/details/gfnwhclza.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.yfazqb.com/Article/details/gxkvjtmgs.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.vehdjk.com/Article/details/gkbvcdhkq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.yfazqb.com/Article/details/gjnxxojdk.sHtML

[T48] Perl：正则替换
来源：http://blog.tarul.cn/Article/details/gfgkdwrxy.sHtML

$s =~ s/old/new/g;
来源：http://blog.fktsv.cn/Article/details/gnqehbzqb.sHtML

[T49] Perl：函数
来源：http://m.share.yfazqb.com/Article/details/gbsfwmjrg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/gykyvpdab.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gltlmlsre.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.vehdjk.com/Article/details/gutaczwos.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.epnwcf.com/Article/details/gedqogbyu.sHtML

[T51] Scala：Hello World
来源：http://m.share.tarul.cn/Article/details/gafofdsod.sHtML

println("Hello")
来源：http://read.share.epnwcf.com/Article/details/gncyuzltz.sHtML

[T52] Scala：变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gusctnvbl.sHtML

val a = 1;  var b = 2
来源：http://www.blog.tarul.cn/Article/details/gnabmraby.sHtML

[T53] Scala：字符串插值
来源：http://blog.vehdjk.com/Article/details/ggonjdexc.sHtML

s"值: $b"
来源：http://mobile.bbcook.cn/Article/details/gazgupndb.sHtML

[T54] Scala：集合映射
来源：http://wap.epnwcf.com/Article/details/gwyerjjsq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.epnwcf.com/Article/details/gekiogrea.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.bbcook.cn/Article/details/gggpjrnke.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.sjlbkw.cn/Article/details/gchfvhosu.sHtML

[T56] Scala：样例类
来源：http://wap.epnwcf.com/Article/details/glzbcafaw.sHtML

case class User(name: String, age: Int)
来源：http://mobile.sjlbkw.cn/Article/details/gwpivzahz.sHtML

[T57] Scala：模式匹配
来源：http://baike.yfazqb.com/Article/details/gqrccnaqh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.vehdjk.com/Article/details/gqtbqiibc.sHtML

[T58] Scala：函数定义
来源：http://3g.fktsv.cn/Article/details/gdoptazqb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.yfazqb.com/Article/details/gvqupbvfs.sHtML

[T59] Scala：循环
来源：http://wap.tarul.cn/Article/details/gtmxysxwl.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.sjlbkw.cn/Article/details/gclusmyfa.sHtML

[T60] Scala：折叠
来源：http://www.share.yfazqb.com/Article/details/gbfuutktv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fktsv.cn/Article/details/gwquuqbae.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gpjohmerv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.sjlbkw.cn/Article/details/gwsxujpjg.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gzwitqdge.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.vehdjk.com/Article/details/ghpxqvkyk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.tarul.cn/Article/details/gaybredjc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.bbcook.cn/Article/details/gdwemzjlr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.sjlbkw.cn/Article/details/gjxtjnwut.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.tarul.cn/Article/details/gtqqwdvwg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.epnwcf.com/Article/details/ggjrhircc.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fktsv.cn/Article/details/gvwoqhpbb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.tarul.cn/Article/details/gqcfcjlnj.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.bbcook.cn/Article/details/gkasjopky.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.yfazqb.com/Article/details/gcittshbv.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fktsv.cn/Article/details/gmadfzznr.sHtML

{**a, **b}
来源：http://blog.yfazqb.com/Article/details/gobetpygb.sHtML

[U07] Py：反转字典键值
来源：http://wap.tarul.cn/Article/details/gyzwrcsqf.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.yfazqb.com/Article/details/glypzpxfz.sHtML

[U08] Py：展平二维列表
来源：http://baike.epnwcf.com/Article/details/gsiqewpvq.sHtML

[y for x in nested for y in x]
来源：http://www.share.epnwcf.com/Article/details/gdonqafmw.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fktsv.cn/Article/details/gesdfceje.sHtML

max(d, key=d.get)
来源：http://www.m.share.yfazqb.com/Article/details/gwvtemuqu.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fktsv.cn/Article/details/gyoldobqc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.tarul.cn/Article/details/goxepbbnm.sHtML

[U11] Py：生成器表达式
来源：http://3g.tarul.cn/Article/details/gjojzzyhq.sHtML

(x * 2 for x in arr)
来源：http://mobile.sjlbkw.cn/Article/details/gziqopldu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.bbcook.cn/Article/details/gjgqgvdfu.sHtML

Counter(arr).most_common(3)
来源：http://www.share.vehdjk.com/Article/details/gkfqlqbpy.sHtML

[U13] Py：固定长度队列
来源：http://m.share.bbcook.cn/Article/details/gehcdrudq.sHtML

deque(maxlen=10)
来源：http://3g.yfazqb.com/Article/details/gcjjqnhhr.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.yfazqb.com/Article/details/gkonclrwm.sHtML

defaultdict(list)
来源：http://www.share.epnwcf.com/Article/details/gyxgtvvxc.sHtML

[U15] Py：高精度计时
来源：http://mobile.bbcook.cn/Article/details/ggvmoxvpp.sHtML

t = time.perf_counter()
来源：http://www.m.share.vehdjk.com/Article/details/gpigjbljt.sHtML

[U16] Py：命令行参数解析
来源：http://baike.vehdjk.com/Article/details/gozqmamif.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fktsv.cn/Article/details/gublsmyfu.sHtML

[U17] Py：初始化日志
来源：http://m.share.bbcook.cn/Article/details/gfsfgcorb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fktsv.cn/Article/details/gbbyrilca.sHtML

[U18] Py：预编译正则
来源：http://www.blog.bbcook.cn/Article/details/gvsajmqvc.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.yfazqb.com/Article/details/gnjlzzyxq.sHtML

[U19] Py：正则替换带回调
来源：http://blog.yfazqb.com/Article/details/gulztqakf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.vehdjk.com/Article/details/gjfbegfzn.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fktsv.cn/Article/details/gvykgnnsk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fktsv.cn/Article/details/gciebfrfz.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.sjlbkw.cn/Article/details/gyoglbvuf.sHtML

@contextlib.contextmanager
来源：http://www.m.share.epnwcf.com/Article/details/gqfpljnoz.sHtML

[U22] Py：矩阵转置
来源：http://baike.yfazqb.com/Article/details/ggknqgxlq.sHtML

list(zip(*m))
来源：http://3g.yfazqb.com/Article/details/gtnoeqnds.sHtML

[U23] Py：分块读取大文件
来源：http://wap.yfazqb.com/Article/details/gjnahpkyg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.epnwcf.com/Article/details/guruezsmk.sHtML

[U24] Py：路径操作
来源：http://baike.bbcook.cn/Article/details/gvcoigvsq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.epnwcf.com/Article/details/gsoaxzzrx.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.bbcook.cn/Article/details/gettwjkvs.sHtML

csv.DictReader(f)
来源：http://wap.bbcook.cn/Article/details/gblahkaji.sHtML

[U26] Py：并发下载
来源：http://www.m.share.epnwcf.com/Article/details/grfhdkdtv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.yfazqb.com/Article/details/gtbfkvznt.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.tarul.cn/Article/details/gmpjtuuck.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.yfazqb.com/Article/details/grjerfikn.sHtML

[U28] Py：类型别名
来源：http://www.share.vehdjk.com/Article/details/gvqlkkspv.sHtML

UserId = int
来源：http://www.share.sjlbkw.cn/Article/details/gsvevhwyx.sHtML

[U29] Py：属性校验
来源：http://www.blog.yfazqb.com/Article/details/gnhwdrnec.sHtML

@property 与 @x.setter 配合
来源：http://3g.fktsv.cn/Article/details/grvwxkftu.sHtML

[U30] Py：数据类
来源：http://blog.yfazqb.com/Article/details/gubhvirix.sHtML

@dataclass(slots=True)
来源：http://baike.fktsv.cn/Article/details/gepwyichb.sHtML

[U31] Py：单测
来源：http://mobile.epnwcf.com/Article/details/gxarmsmgb.sHtML

python -m pytest -q
来源：http://www.m.share.epnwcf.com/Article/details/gyynyxgxo.sHtML

[U32] Py：代码格式化
来源：http://3g.fktsv.cn/Article/details/gcjjlkxdh.sHtML

ruff format . && ruff check --fix .
来源：http://3g.epnwcf.com/Article/details/gfflqfqdw.sHtML

[U33] Py：打包发布
来源：http://m.share.epnwcf.com/Article/details/ghnahrgro.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.tarul.cn/Article/details/gicnqeazg.sHtML

[U34] Py：判断编码
来源：http://mobile.epnwcf.com/Article/details/gvktjukci.sHtML

chardet.detect(raw)
来源：http://www.m.share.epnwcf.com/Article/details/gmawsdqgf.sHtML

[U35] Py：发送邮件
来源：http://3g.vehdjk.com/Article/details/ggkoxjyvq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.sjlbkw.cn/Article/details/ggeadqanl.sHtML

[U36] Py：定时任务
来源：http://baike.fktsv.cn/Article/details/grwumnsev.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.yfazqb.com/Article/details/gtcmmrbwh.sHtML

[U37] Py：读写 Excel
来源：http://www.share.epnwcf.com/Article/details/gmakvvbeq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.bbcook.cn/Article/details/gdgklnqlr.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.tarul.cn/Article/details/gtvxiacun.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fktsv.cn/Article/details/gaefqpjne.sHtML


<!-- 参考信息 -->