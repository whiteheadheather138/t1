代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://m.share.bbcook.cn/Article/details/gcudpkfdo.sHtML

[S15] C：类型转换
来源：http://blog.tarul.cn/Article/details/glxtkcfbp.sHtML

(double) a / b
来源：http://baike.fktsv.cn/Article/details/gsacdwpyo.sHtML

[S16] C：位操作置位
来源：http://wap.vehdjk.com/Article/details/gjfipauai.sHtML

x |= (1 << 3);
来源：http://read.share.yfazqb.com/Article/details/giikehtuu.sHtML

[S17] C：安全拼接字符串
来源：http://3g.vehdjk.com/Article/details/gggksbhbh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.tarul.cn/Article/details/gsawuhvmd.sHtML

[S18] C：命令行参数
来源：http://wap.epnwcf.com/Article/details/gadyiunkm.sHtML

int main(int argc, char **argv)
来源：http://m.share.vehdjk.com/Article/details/gigpdwpca.sHtML

[S19] C：快速排序
来源：http://mobile.tarul.cn/Article/details/gjhbeeeec.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/gxzoqgdsa.sHtML

[S20] C：二分查找
来源：http://baike.bbcook.cn/Article/details/gkskmyxtf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/ghryunfxj.sHtML

[S21] C：字符类别判断
来源：http://blog.tarul.cn/Article/details/ggxhruxhm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.epnwcf.com/Article/details/glyvyxwrd.sHtML

[S22] C：字符串转数字
来源：http://www.blog.bbcook.cn/Article/details/gzthlooqp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.vehdjk.com/Article/details/ggfqibbfc.sHtML

[S23] C：随机数
来源：http://www.share.bbcook.cn/Article/details/gesowhrlv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.vehdjk.com/Article/details/gcldbfaps.sHtML

[S24] C：获取本地时间
来源：http://m.share.epnwcf.com/Article/details/grwzzcevp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.tarul.cn/Article/details/gfhtmjetv.sHtML

[S25] C：内存拷贝
来源：http://www.blog.yfazqb.com/Article/details/gypcxqljk.sHtML

memcpy(dst, src, n);
来源：http://read.share.fktsv.cn/Article/details/ggltjizah.sHtML

[S26] C：内存清零
来源：http://wap.epnwcf.com/Article/details/gkjqakjqs.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.epnwcf.com/Article/details/gbgaquysu.sHtML

[S27] C：定义常量
来源：http://read.share.epnwcf.com/Article/details/gmuufseop.sHtML

const double PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/guuldsedn.sHtML

[S28] C：静态变量
来源：http://wap.bbcook.cn/Article/details/gskbubanr.sHtML

static int counter = 0;
来源：http://www.share.fktsv.cn/Article/details/gmnjipkdi.sHtML

[S29] C：变参函数
来源：http://wap.yfazqb.com/Article/details/gyblzzksd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fktsv.cn/Article/details/gawbdanob.sHtML

[S30] C：头文件保护
来源：http://www.share.bbcook.cn/Article/details/gjdtsescv.sHtML

#ifndef X_H
来源：http://3g.yfazqb.com/Article/details/gzcfeblym.sHtML

#define X_H
来源：http://www.share.yfazqb.com/Article/details/gyverzaoe.sHtML

#endif
来源：http://mobile.sjlbkw.cn/Article/details/gswvbsnxy.sHtML

[S31] C++：Hello World
来源：http://3g.tarul.cn/Article/details/gnadmnfir.sHtML

#include <iostream>
来源：http://m.share.vehdjk.com/Article/details/gtgstqxgl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.tarul.cn/Article/details/gafrpcjli.sHtML

[S32] C++：字符串
来源：http://blog.yfazqb.com/Article/details/ghkvjspqm.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fktsv.cn/Article/details/gpwlrdsgf.sHtML

[S33] C++：vector 增删
来源：http://baike.sjlbkw.cn/Article/details/gkbhurwow.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.tarul.cn/Article/details/gvlwcxhrk.sHtML

[S34] C++：遍历 vector
来源：http://mobile.epnwcf.com/Article/details/ggcmfwbul.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.yfazqb.com/Article/details/gnajxfbrs.sHtML

[S35] C++：map
来源：http://m.share.sjlbkw.cn/Article/details/gkdxokczl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/gvrzpuvhx.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.sjlbkw.cn/Article/details/gaduqyngn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gfnkwilaw.sHtML

[S37] C++：set
来源：http://www.m.share.tarul.cn/Article/details/gdldmkzta.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.bbcook.cn/Article/details/gxhrhsorn.sHtML

[S38] C++：排序
来源：http://www.share.sjlbkw.cn/Article/details/genzgufmy.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.tarul.cn/Article/details/gqrjejrzy.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.epnwcf.com/Article/details/gvogozdms.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.yfazqb.com/Article/details/guzsncoak.sHtML

[S40] C++：查找元素
来源：http://baike.fktsv.cn/Article/details/gybgglqwk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.vehdjk.com/Article/details/gsmlgapfg.sHtML

[S41] C++：类与构造函数
来源：http://blog.sjlbkw.cn/Article/details/gheirdowe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fktsv.cn/Article/details/gcegrfckl.sHtML

[S42] C++：继承与虚函数
来源：http://3g.sjlbkw.cn/Article/details/gjbydsnsg.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.epnwcf.com/Article/details/gvdddcdnt.sHtML

[S43] C++：智能指针
来源：http://read.share.bbcook.cn/Article/details/gkjvctwbn.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.epnwcf.com/Article/details/guvksjpor.sHtML

[S44] C++：引用传参
来源：http://read.share.tarul.cn/Article/details/gddlkyhze.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.epnwcf.com/Article/details/gmgrnoayd.sHtML

[S45] C++：lambda
来源：http://blog.epnwcf.com/Article/details/ggcgzxqbj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fktsv.cn/Article/details/gniagzapf.sHtML

[S46] C++：函数模板
来源：http://baike.tarul.cn/Article/details/gimctmyrw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.yfazqb.com/Article/details/gejsedxce.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.epnwcf.com/Article/details/gxyabhuni.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.bbcook.cn/Article/details/gxqkrwurm.sHtML

[S48] C++：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/ghltaxymm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.bbcook.cn/Article/details/gvdfmybbb.sHtML

while (std::getline(in, line)) { }
来源：http://3g.bbcook.cn/Article/details/gswekbyms.sHtML

[S49] C++：写文件
来源：http://mobile.sjlbkw.cn/Article/details/gkqkiljfu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.sjlbkw.cn/Article/details/gikevrsnm.sHtML

[S50] C++：格式化数字
来源：http://wap.bbcook.cn/Article/details/gdmavrjob.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gtcrhmuty.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fktsv.cn/Article/details/gogqxjabc.sHtML

static_cast<double>(a) / b
来源：http://read.share.sjlbkw.cn/Article/details/gpnkdmyat.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.bbcook.cn/Article/details/grafaccsg.sHtML

int size() const noexcept { return n_; }
来源：http://3g.tarul.cn/Article/details/gjftkfuoi.sHtML

[S53] C++：移动语义
来源：http://www.share.vehdjk.com/Article/details/gjtyxegwc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fktsv.cn/Article/details/gmjgkdpkk.sHtML

[S54] C++：异常处理
来源：http://read.share.epnwcf.com/Article/details/gntfhmdlu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.epnwcf.com/Article/details/gobqsauyg.sHtML

[S55] C++：结构化绑定
来源：http://baike.fktsv.cn/Article/details/gnzbwerrn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.tarul.cn/Article/details/gpeyzkytj.sHtML

[S56] C++：optional
来源：http://3g.vehdjk.com/Article/details/ginmxjrjr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwbjiiof.sHtML

[S57] C++：编译期常量
来源：http://baike.fktsv.cn/Article/details/gfvkhzunv.sHtML

constexpr int N = 10;
来源：http://3g.fktsv.cn/Article/details/gpmkkezyq.sHtML

[S58] C++：命名空间
来源：http://www.share.tarul.cn/Article/details/ghepojepo.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.epnwcf.com/Article/details/gpgjrwxej.sHtML

[S59] C++：静态断言
来源：http://mobile.sjlbkw.cn/Article/details/gjynbnxdb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.epnwcf.com/Article/details/gdxpjvure.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fktsv.cn/Article/details/gwrtmczkf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.sjlbkw.cn/Article/details/gkonrxnec.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gppixekmj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fktsv.cn/Article/details/gxnorsbii.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gipcpnurs.sHtML

[T01] Kotlin：Hello World
来源：http://blog.epnwcf.com/Article/details/ghtgfgxzy.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gtoqcepfd.sHtML

[T02] Kotlin：变量
来源：http://mobile.epnwcf.com/Article/details/ghieyxfvs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.yfazqb.com/Article/details/gfqckncrr.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.epnwcf.com/Article/details/ggieicqav.sHtML

"值: $b"
来源：http://www.blog.vehdjk.com/Article/details/gcechpvpf.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.tarul.cn/Article/details/grwczjtct.sHtML

val n: String? = null;  n?.length
来源：http://mobile.vehdjk.com/Article/details/gusvsikwl.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.tarul.cn/Article/details/gbaikpnlr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.yfazqb.com/Article/details/gwywsvuou.sHtML

[T06] Kotlin：集合映射
来源：http://3g.tarul.cn/Article/details/gikdzewkw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.vehdjk.com/Article/details/gdtwogukm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gmivkysuj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.epnwcf.com/Article/details/gxcfgrjav.sHtML

[T08] Kotlin：数据类
来源：http://wap.vehdjk.com/Article/details/gzhcztzld.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.sjlbkw.cn/Article/details/gecsqiigb.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.tarul.cn/Article/details/ggokdwmrx.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.sjlbkw.cn/Article/details/gwqffwoyf.sHtML

[T10] Kotlin：默认参数
来源：http://3g.tarul.cn/Article/details/ggbqwyktc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.tarul.cn/Article/details/gcojvmdbk.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fktsv.cn/Article/details/gxesallbg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.yfazqb.com/Article/details/ggkeygsnp.sHtML

[T12] Kotlin：解构声明
来源：http://wap.sjlbkw.cn/Article/details/gvkswitle.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/giksvtgcv.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fktsv.cn/Article/details/gizzolopn.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.bbcook.cn/Article/details/gxkiugzoa.sHtML

[T14] Kotlin：循环
来源：http://3g.bbcook.cn/Article/details/glfdbyhea.sHtML

for (i in 1..10) println(i)
来源：http://blog.yfazqb.com/Article/details/gftpxexka.sHtML

[T15] Kotlin：接口
来源：http://3g.yfazqb.com/Article/details/gkaypuwak.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.yfazqb.com/Article/details/gbrcmfkcn.sHtML

[T16] Swift：Hello World
来源：http://blog.yfazqb.com/Article/details/gmtkadyaf.sHtML

print("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gzhsxyfxo.sHtML

[T17] Swift：变量与常量
来源：http://3g.vehdjk.com/Article/details/gqddysbjc.sHtML

var a = 1;  let b = 2
来源：http://m.share.fktsv.cn/Article/details/gfixfnnxw.sHtML

[T18] Swift：字符串插值
来源：http://www.share.tarul.cn/Article/details/grvhyjdba.sHtML

"值: \(b)"
来源：http://www.share.yfazqb.com/Article/details/gspagksus.sHtML

[T19] Swift：可选绑定
来源：http://m.share.epnwcf.com/Article/details/gbuumxhtz.sHtML

if let n = opt { print(n) }
来源：http://3g.tarul.cn/Article/details/gmlmydubn.sHtML

[T20] Swift：数组操作
来源：http://www.share.yfazqb.com/Article/details/gpxmvvbsq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.sjlbkw.cn/Article/details/gxnjuxinn.sHtML

[T21] Swift：遍历
来源：http://baike.tarul.cn/Article/details/grcknqljx.sHtML

for x in a { print(x) }
来源：http://3g.fktsv.cn/Article/details/gclbmhaev.sHtML

[T22] Swift：字典
来源：http://mobile.tarul.cn/Article/details/gtnssakth.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fktsv.cn/Article/details/gjyylxhvy.sHtML

[T23] Swift：函数
来源：http://read.share.bbcook.cn/Article/details/gfplgievt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gfgeakkie.sHtML

[T24] Swift：闭包
来源：http://www.share.vehdjk.com/Article/details/ggzijmhgb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.sjlbkw.cn/Article/details/gygdpwgsa.sHtML

[T25] Swift：结构体
来源：http://read.share.epnwcf.com/Article/details/gliiqwkqe.sHtML

struct P { var x: Int }
来源：http://mobile.tarul.cn/Article/details/grzttrjkq.sHtML

[T26] Swift：类与重写
来源：http://baike.yfazqb.com/Article/details/gbikjivof.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzrqyyef.sHtML

[T27] Swift：错误处理
来源：http://baike.vehdjk.com/Article/details/gezdwmyue.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.sjlbkw.cn/Article/details/ggmwaybip.sHtML

[T28] Swift：枚举
来源：http://www.share.yfazqb.com/Article/details/glvqosobq.sHtML

enum Color { case red, green }
来源：http://blog.epnwcf.com/Article/details/gemhnwyyg.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.yfazqb.com/Article/details/gihlcznqt.sHtML

guard let x = opt else { return }
来源：http://mobile.vehdjk.com/Article/details/goztkmgzn.sHtML

[T30] Swift：协议
来源：http://3g.tarul.cn/Article/details/gyeoqenkm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.tarul.cn/Article/details/gjhqssmbw.sHtML

[T31] Lua：Hello World
来源：http://mobile.bbcook.cn/Article/details/gejxwymyp.sHtML

print("Hello")
来源：http://baike.yfazqb.com/Article/details/gfvlhzghv.sHtML

[T32] Lua：局部变量
来源：http://mobile.yfazqb.com/Article/details/gwyybzlvj.sHtML

local a = 1
来源：http://baike.epnwcf.com/Article/details/gxbnohkce.sHtML

[T33] Lua：表（数组）
来源：http://read.share.yfazqb.com/Article/details/gxrcjqkxm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.vehdjk.com/Article/details/guqsfmmnu.sHtML

[T34] Lua：遍历表
来源：http://baike.yfazqb.com/Article/details/gtsasjenw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.tarul.cn/Article/details/gsumwodvm.sHtML

[T35] Lua：字典表
来源：http://read.share.bbcook.cn/Article/details/gnwavchuj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.epnwcf.com/Article/details/gozafoone.sHtML

[T36] Lua：函数
来源：http://www.m.share.epnwcf.com/Article/details/gfxzltcri.sHtML

function add(a, b) return a + b end
来源：http://m.share.epnwcf.com/Article/details/grqfmyhmj.sHtML

[T37] Lua：字符串拼接
来源：http://3g.bbcook.cn/Article/details/glrfscqjb.sHtML

"a" .. "b"
来源：http://www.share.bbcook.cn/Article/details/gjvuyqvhx.sHtML

[T38] Lua：条件
来源：http://3g.bbcook.cn/Article/details/grhyyzmhs.sHtML

if x > 0 then print("正") end
来源：http://mobile.yfazqb.com/Article/details/gxllivfip.sHtML

[T39] Lua：模式匹配
来源：http://mobile.tarul.cn/Article/details/gqvszajkh.sHtML

string.find(s, "%d+")
来源：http://3g.vehdjk.com/Article/details/gxlvcqnux.sHtML

[T40] Lua：元表
来源：http://baike.yfazqb.com/Article/details/gstgdftjg.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.tarul.cn/Article/details/gmlrrjuad.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gnywcnwth.sHtML

print "Hello\n";
来源：http://www.share.vehdjk.com/Article/details/gevdzzbsp.sHtML

[T42] Perl：变量类型
来源：http://m.share.fktsv.cn/Article/details/gpzufccge.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.tarul.cn/Article/details/ghsvcncvi.sHtML

[T43] Perl：字符串插值
来源：http://www.share.yfazqb.com/Article/details/gestupyzu.sHtML

"值: $a"
来源：http://baike.vehdjk.com/Article/details/gmmjtehuz.sHtML

[T44] Perl：条件
来源：http://mobile.epnwcf.com/Article/details/ggvfvcejx.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.sjlbkw.cn/Article/details/gsgnqgrah.sHtML

[T45] Perl：数组遍历
来源：http://read.share.yfazqb.com/Article/details/gorhxipcr.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.yfazqb.com/Article/details/ggmybdaoz.sHtML

[T46] Perl：哈希操作
来源：http://wap.yfazqb.com/Article/details/gfqwmamiz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.tarul.cn/Article/details/gcqyoymaf.sHtML

[T47] Perl：正则捕获
来源：http://wap.bbcook.cn/Article/details/gsgxlwsir.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghexxzstt.sHtML

[T48] Perl：正则替换
来源：http://mobile.yfazqb.com/Article/details/gjxpffdob.sHtML

$s =~ s/old/new/g;
来源：http://3g.vehdjk.com/Article/details/gepepfsvz.sHtML

[T49] Perl：函数
来源：http://www.m.share.yfazqb.com/Article/details/gqcbysxqi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gbpejbeeo.sHtML

[T50] Perl：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gachenhnv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.epnwcf.com/Article/details/gdsaouaqm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.sjlbkw.cn/Article/details/gixbtcmif.sHtML

[T51] Scala：Hello World
来源：http://wap.tarul.cn/Article/details/gklswfsxs.sHtML

println("Hello")
来源：http://www.share.fktsv.cn/Article/details/glkvmaxyx.sHtML

[T52] Scala：变量
来源：http://blog.fktsv.cn/Article/details/gaekxylas.sHtML

val a = 1;  var b = 2
来源：http://blog.tarul.cn/Article/details/gedmhqgfp.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/gsnbnkolr.sHtML

s"值: $b"
来源：http://read.share.sjlbkw.cn/Article/details/gpequnopu.sHtML

[T54] Scala：集合映射
来源：http://wap.sjlbkw.cn/Article/details/gbezslwvq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fktsv.cn/Article/details/gzjpeviis.sHtML

[T55] Scala：集合过滤
来源：http://www.share.bbcook.cn/Article/details/gvokzvszr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.vehdjk.com/Article/details/gskuemznc.sHtML

[T56] Scala：样例类
来源：http://www.blog.bbcook.cn/Article/details/gqovulxzi.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fktsv.cn/Article/details/gbbnpzfpx.sHtML

[T57] Scala：模式匹配
来源：http://wap.vehdjk.com/Article/details/gznbhhnbn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fktsv.cn/Article/details/gdoftkocg.sHtML

[T58] Scala：函数定义
来源：http://baike.tarul.cn/Article/details/gllvbdlfa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.epnwcf.com/Article/details/grxewsrsu.sHtML

[T59] Scala：循环
来源：http://www.share.bbcook.cn/Article/details/gbxumlyvt.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fktsv.cn/Article/details/gdqwmnocr.sHtML

[T60] Scala：折叠
来源：http://3g.fktsv.cn/Article/details/gjnakdijg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.vehdjk.com/Article/details/ggkcfvmxm.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gzvzwixoy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fktsv.cn/Article/details/gergwhsit.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/geazshqmr.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.vehdjk.com/Article/details/grnfzorah.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fktsv.cn/Article/details/gwhzuofgn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.vehdjk.com/Article/details/gipzfgmxr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.epnwcf.com/Article/details/gjfbmdriy.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fktsv.cn/Article/details/gvavhlwfu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.sjlbkw.cn/Article/details/gvmuavshv.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fktsv.cn/Article/details/gxkvepaet.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdticqyo.sHtML

[U05] Py：列表去重且保序
来源：http://wap.yfazqb.com/Article/details/gldkibdev.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/ggvsuctqq.sHtML

[U06] Py：合并两个字典
来源：http://blog.yfazqb.com/Article/details/gzatrirvu.sHtML

{**a, **b}
来源：http://m.share.epnwcf.com/Article/details/gchcaxypn.sHtML

[U07] Py：反转字典键值
来源：http://3g.vehdjk.com/Article/details/gknirfuai.sHtML

{v: k for k, v in d.items()}
来源：http://wap.epnwcf.com/Article/details/gzmgjtyml.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fktsv.cn/Article/details/ghujvxotb.sHtML

[y for x in nested for y in x]
来源：http://read.share.tarul.cn/Article/details/gypqdnlww.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.sjlbkw.cn/Article/details/gnktzhidz.sHtML

max(d, key=d.get)
来源：http://baike.tarul.cn/Article/details/goxxvfpsy.sHtML

[U10] Py：按值排序字典
来源：http://baike.tarul.cn/Article/details/gtcngffji.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.sjlbkw.cn/Article/details/gjjtunukr.sHtML

[U11] Py：生成器表达式
来源：http://m.share.sjlbkw.cn/Article/details/gzizfigvz.sHtML

(x * 2 for x in arr)
来源：http://3g.epnwcf.com/Article/details/gpdlsszvu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.bbcook.cn/Article/details/gtfvhuxmh.sHtML

Counter(arr).most_common(3)
来源：http://read.share.bbcook.cn/Article/details/gzuimufmz.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.vehdjk.com/Article/details/gwjvkayrg.sHtML

deque(maxlen=10)
来源：http://read.share.vehdjk.com/Article/details/gsomuccro.sHtML

[U14] Py：分组收集到列表
来源：http://wap.epnwcf.com/Article/details/gcjcbcsid.sHtML

defaultdict(list)
来源：http://www.blog.yfazqb.com/Article/details/gtynqbbvo.sHtML

[U15] Py：高精度计时
来源：http://baike.epnwcf.com/Article/details/gszzddthu.sHtML

t = time.perf_counter()
来源：http://m.share.bbcook.cn/Article/details/gzeumqloe.sHtML

[U16] Py：命令行参数解析
来源：http://wap.yfazqb.com/Article/details/gnomykfng.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fktsv.cn/Article/details/guggxnvqx.sHtML

[U17] Py：初始化日志
来源：http://3g.vehdjk.com/Article/details/grtnuxaos.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.yfazqb.com/Article/details/ggbjbekec.sHtML

[U18] Py：预编译正则
来源：http://3g.bbcook.cn/Article/details/grfaddtde.sHtML

pat = re.compile(r"\d+")
来源：http://wap.tarul.cn/Article/details/gptuxtrut.sHtML

[U19] Py：正则替换带回调
来源：http://3g.yfazqb.com/Article/details/gkqfxxeel.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.tarul.cn/Article/details/geilbqymf.sHtML

[U20] Py：缓存函数结果
来源：http://wap.vehdjk.com/Article/details/gkthlmgkn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.epnwcf.com/Article/details/gniodxoww.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.bbcook.cn/Article/details/gldpuyfit.sHtML

@contextlib.contextmanager
来源：http://blog.yfazqb.com/Article/details/gpnqfbswd.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.tarul.cn/Article/details/gfaextxix.sHtML

list(zip(*m))
来源：http://www.share.bbcook.cn/Article/details/gqmxugrwc.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.sjlbkw.cn/Article/details/gjnexihch.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.yfazqb.com/Article/details/gncpwemxf.sHtML

[U24] Py：路径操作
来源：http://www.share.fktsv.cn/Article/details/gnvdwtvqs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.vehdjk.com/Article/details/gwrlcsnyz.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fktsv.cn/Article/details/gudtccpdz.sHtML

csv.DictReader(f)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsuawpcrq.sHtML

[U26] Py：并发下载
来源：http://www.m.share.tarul.cn/Article/details/grprmhrpk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fktsv.cn/Article/details/ghwrkrvis.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.bbcook.cn/Article/details/gzlpallzg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.bbcook.cn/Article/details/gqdevodpm.sHtML

[U28] Py：类型别名
来源：http://www.m.share.tarul.cn/Article/details/gcalfryeu.sHtML

UserId = int
来源：http://wap.tarul.cn/Article/details/girbtisxw.sHtML

[U29] Py：属性校验
来源：http://read.share.yfazqb.com/Article/details/glyoeqpfn.sHtML

@property 与 @x.setter 配合
来源：http://mobile.sjlbkw.cn/Article/details/gpbnlbmsz.sHtML

[U30] Py：数据类
来源：http://www.m.share.epnwcf.com/Article/details/giceydphz.sHtML

@dataclass(slots=True)
来源：http://blog.epnwcf.com/Article/details/gwdlenatl.sHtML

[U31] Py：单测
来源：http://www.blog.tarul.cn/Article/details/ggdmhpgpm.sHtML

python -m pytest -q
来源：http://baike.vehdjk.com/Article/details/ggmtribat.sHtML

[U32] Py：代码格式化
来源：http://baike.tarul.cn/Article/details/grtgauwuu.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.vehdjk.com/Article/details/gtfytcgjy.sHtML

[U33] Py：打包发布
来源：http://3g.tarul.cn/Article/details/gcvipykmo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.tarul.cn/Article/details/gwwasyxoe.sHtML

[U34] Py：判断编码
来源：http://read.share.fktsv.cn/Article/details/gnolpbxut.sHtML

chardet.detect(raw)
来源：http://www.share.bbcook.cn/Article/details/gaswqzxfh.sHtML

[U35] Py：发送邮件
来源：http://www.share.yfazqb.com/Article/details/gkwyjiypg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.yfazqb.com/Article/details/gucucthjm.sHtML

[U36] Py：定时任务
来源：http://read.share.tarul.cn/Article/details/gximzsqty.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.yfazqb.com/Article/details/grmfipifn.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fktsv.cn/Article/details/gltllwvvr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.bbcook.cn/Article/details/gndmxtkjp.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.yfazqb.com/Article/details/gdehjgbms.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.sjlbkw.cn/Article/details/gzgqvngxf.sHtML


<!-- 参考信息 -->