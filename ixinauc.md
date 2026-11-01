代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.tarul.cn/Article/details/gsvgtnekn.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fktsv.cn/Article/details/glufmwure.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.epnwcf.com/Article/details/gxrsunxfj.sHtML

[S22] C：字符串转数字
来源：http://www.blog.vehdjk.com/Article/details/gocylfljt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.epnwcf.com/Article/details/glwujbzdi.sHtML

[S23] C：随机数
来源：http://www.share.epnwcf.com/Article/details/gxroiwrzs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.epnwcf.com/Article/details/gecztmwaj.sHtML

[S24] C：获取本地时间
来源：http://wap.fktsv.cn/Article/details/gscbdbrrn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.yfazqb.com/Article/details/gpkyiqmix.sHtML

[S25] C：内存拷贝
来源：http://mobile.tarul.cn/Article/details/gulizwqjc.sHtML

memcpy(dst, src, n);
来源：http://mobile.bbcook.cn/Article/details/gduiwcaba.sHtML

[S26] C：内存清零
来源：http://www.share.vehdjk.com/Article/details/gfltvnchy.sHtML

memset(a, 0, sizeof a);
来源：http://blog.vehdjk.com/Article/details/gymybeikb.sHtML

[S27] C：定义常量
来源：http://3g.epnwcf.com/Article/details/gwymdccth.sHtML

const double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gipeocdyl.sHtML

[S28] C：静态变量
来源：http://blog.yfazqb.com/Article/details/gdxdyndhb.sHtML

static int counter = 0;
来源：http://m.share.tarul.cn/Article/details/gozsxszgx.sHtML

[S29] C：变参函数
来源：http://m.share.yfazqb.com/Article/details/gypgcxagb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.tarul.cn/Article/details/glrtjnwxn.sHtML

[S30] C：头文件保护
来源：http://www.m.share.tarul.cn/Article/details/gsnklnmmq.sHtML

#ifndef X_H
来源：http://mobile.bbcook.cn/Article/details/gjjscrdqi.sHtML

#define X_H
来源：http://m.share.yfazqb.com/Article/details/gtuphakbf.sHtML

#endif
来源：http://www.share.vehdjk.com/Article/details/gvnisrfmo.sHtML

[S31] C++：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gsezurlew.sHtML

#include <iostream>
来源：http://www.m.share.yfazqb.com/Article/details/gvufkvopx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fktsv.cn/Article/details/gqiqvrusz.sHtML

[S32] C++：字符串
来源：http://www.share.yfazqb.com/Article/details/gxnqgjusp.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.tarul.cn/Article/details/ggxanqevj.sHtML

[S33] C++：vector 增删
来源：http://www.share.yfazqb.com/Article/details/gwaobvbgh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fktsv.cn/Article/details/gjgcpmmzu.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fktsv.cn/Article/details/gfpvkfvbo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.epnwcf.com/Article/details/gvyxsezlk.sHtML

[S35] C++：map
来源：http://m.share.epnwcf.com/Article/details/goeqznzxd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fktsv.cn/Article/details/govahunos.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.sjlbkw.cn/Article/details/giwjshpwt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.epnwcf.com/Article/details/gbhztzmfr.sHtML

[S37] C++：set
来源：http://blog.bbcook.cn/Article/details/gyydkcxhc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.bbcook.cn/Article/details/giotauwmc.sHtML

[S38] C++：排序
来源：http://baike.vehdjk.com/Article/details/gspadmrbx.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.sjlbkw.cn/Article/details/gyosfhwmb.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fktsv.cn/Article/details/guwlmbjyy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.sjlbkw.cn/Article/details/gglacebix.sHtML

[S40] C++：查找元素
来源：http://www.blog.tarul.cn/Article/details/gvqtblgay.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.tarul.cn/Article/details/glrijthtk.sHtML

[S41] C++：类与构造函数
来源：http://baike.sjlbkw.cn/Article/details/gzzqdfoic.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fktsv.cn/Article/details/gxvlbyazo.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.bbcook.cn/Article/details/geucdwngu.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.sjlbkw.cn/Article/details/ghmkysnue.sHtML

[S43] C++：智能指针
来源：http://read.share.bbcook.cn/Article/details/ggadbivxv.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.vehdjk.com/Article/details/gvfjhqwxi.sHtML

[S44] C++：引用传参
来源：http://blog.tarul.cn/Article/details/glvlcnxeu.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.bbcook.cn/Article/details/gdbqsvecy.sHtML

[S45] C++：lambda
来源：http://www.share.epnwcf.com/Article/details/gwuizeccn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.yfazqb.com/Article/details/gomvzduvz.sHtML

[S46] C++：函数模板
来源：http://m.share.tarul.cn/Article/details/gpwaesefr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fktsv.cn/Article/details/ghoiiogdt.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.yfazqb.com/Article/details/ghogilpkt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.epnwcf.com/Article/details/gmfnnbmph.sHtML

[S48] C++：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gijzybcxp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.tarul.cn/Article/details/gjdagoztw.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.vehdjk.com/Article/details/gqmwyaile.sHtML

[S49] C++：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkbojnik.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.vehdjk.com/Article/details/gltgaphdm.sHtML

[S50] C++：格式化数字
来源：http://mobile.fktsv.cn/Article/details/gorckvway.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.yfazqb.com/Article/details/gorsgzkgs.sHtML

[S51] C++：显式类型转换
来源：http://wap.vehdjk.com/Article/details/gekqucihg.sHtML

static_cast<double>(a) / b
来源：http://www.blog.tarul.cn/Article/details/gpeolkvje.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.bbcook.cn/Article/details/gdityrwrv.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fktsv.cn/Article/details/gnonckwky.sHtML

[S53] C++：移动语义
来源：http://www.share.sjlbkw.cn/Article/details/gaebrlkyb.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fktsv.cn/Article/details/guldarfcv.sHtML

[S54] C++：异常处理
来源：http://m.share.fktsv.cn/Article/details/gqwfvzmva.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.epnwcf.com/Article/details/gyehqgkis.sHtML

[S55] C++：结构化绑定
来源：http://www.share.epnwcf.com/Article/details/gvcweuyop.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fktsv.cn/Article/details/glzyopepe.sHtML

[S56] C++：optional
来源：http://www.m.share.tarul.cn/Article/details/gvaxawomg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.sjlbkw.cn/Article/details/gyhgxbpvp.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fktsv.cn/Article/details/gxhsmmiob.sHtML

constexpr int N = 10;
来源：http://www.share.fktsv.cn/Article/details/gablhprtk.sHtML

[S58] C++：命名空间
来源：http://mobile.fktsv.cn/Article/details/gwjoytggs.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.epnwcf.com/Article/details/ghmsfbjie.sHtML

[S59] C++：静态断言
来源：http://mobile.bbcook.cn/Article/details/gwiuidqsa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.bbcook.cn/Article/details/gsbppguqf.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.epnwcf.com/Article/details/gwaxemdwx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.tarul.cn/Article/details/gvaekkmad.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gxqtewifj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.yfazqb.com/Article/details/geqozioje.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gbjlhemfu.sHtML

[T01] Kotlin：Hello World
来源：http://baike.tarul.cn/Article/details/glpmdebgk.sHtML

println("Hello")
来源：http://blog.fktsv.cn/Article/details/gqrbyskbq.sHtML

[T02] Kotlin：变量
来源：http://3g.tarul.cn/Article/details/ggbwbjeqi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.vehdjk.com/Article/details/gguvgxing.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.tarul.cn/Article/details/guotgeprx.sHtML

"值: $b"
来源：http://www.m.share.sjlbkw.cn/Article/details/goeprjfic.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.epnwcf.com/Article/details/gidhyvasm.sHtML

val n: String? = null;  n?.length
来源：http://blog.fktsv.cn/Article/details/gtuhwybvr.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.epnwcf.com/Article/details/gbwsdwpon.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.yfazqb.com/Article/details/gjpbgvwra.sHtML

[T06] Kotlin：集合映射
来源：http://baike.vehdjk.com/Article/details/grvivvhuq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gntdqgbzj.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.epnwcf.com/Article/details/gyxaleaec.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.epnwcf.com/Article/details/gakecdlxe.sHtML

[T08] Kotlin：数据类
来源：http://3g.yfazqb.com/Article/details/gofamljqo.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.tarul.cn/Article/details/gmebtarpx.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fktsv.cn/Article/details/gzdkmgaag.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.bbcook.cn/Article/details/gywseicfs.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fktsv.cn/Article/details/gdqufkjsx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.tarul.cn/Article/details/gsrwqlpbj.sHtML

[T11] Kotlin：协程
来源：http://m.share.yfazqb.com/Article/details/gqlwulbid.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.tarul.cn/Article/details/gynfsdfcv.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.yfazqb.com/Article/details/guertkore.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.yfazqb.com/Article/details/gowfxzxcq.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.epnwcf.com/Article/details/gvkacazca.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.epnwcf.com/Article/details/gpqkdnvzw.sHtML

[T14] Kotlin：循环
来源：http://read.share.epnwcf.com/Article/details/gqountyfg.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.bbcook.cn/Article/details/goeoymnge.sHtML

[T15] Kotlin：接口
来源：http://wap.fktsv.cn/Article/details/ggjoqwrav.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.vehdjk.com/Article/details/gmmzaxfcx.sHtML

[T16] Swift：Hello World
来源：http://www.share.tarul.cn/Article/details/gsljxkbxx.sHtML

print("Hello")
来源：http://m.share.yfazqb.com/Article/details/gteenioyq.sHtML

[T17] Swift：变量与常量
来源：http://3g.epnwcf.com/Article/details/grblatzwd.sHtML

var a = 1;  let b = 2
来源：http://www.share.vehdjk.com/Article/details/grlhxigky.sHtML

[T18] Swift：字符串插值
来源：http://3g.fktsv.cn/Article/details/ghmfhfgxv.sHtML

"值: \(b)"
来源：http://baike.epnwcf.com/Article/details/gkiwrkrif.sHtML

[T19] Swift：可选绑定
来源：http://www.share.bbcook.cn/Article/details/guptfjnid.sHtML

if let n = opt { print(n) }
来源：http://m.share.tarul.cn/Article/details/gbaqtsjht.sHtML

[T20] Swift：数组操作
来源：http://baike.tarul.cn/Article/details/gysbmdkdf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.yfazqb.com/Article/details/gwkkzjodv.sHtML

[T21] Swift：遍历
来源：http://3g.bbcook.cn/Article/details/gxhvvprge.sHtML

for x in a { print(x) }
来源：http://blog.bbcook.cn/Article/details/gjvuhbuwq.sHtML

[T22] Swift：字典
来源：http://blog.tarul.cn/Article/details/gsmwpedvi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fktsv.cn/Article/details/glqlwtacl.sHtML

[T23] Swift：函数
来源：http://blog.epnwcf.com/Article/details/gbowyqcat.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrqtxtba.sHtML

[T24] Swift：闭包
来源：http://m.share.yfazqb.com/Article/details/gwhmlgjjr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.yfazqb.com/Article/details/gryrxljte.sHtML

[T25] Swift：结构体
来源：http://wap.bbcook.cn/Article/details/gqufzssbd.sHtML

struct P { var x: Int }
来源：http://3g.epnwcf.com/Article/details/gizldkgwg.sHtML

[T26] Swift：类与重写
来源：http://m.share.sjlbkw.cn/Article/details/gsywpolgd.sHtML

class A: Base { override func f() {} }
来源：http://3g.epnwcf.com/Article/details/gfksmtdqi.sHtML

[T27] Swift：错误处理
来源：http://www.blog.tarul.cn/Article/details/gajgunjgr.sHtML

do { try f() } catch { print(error) }
来源：http://baike.vehdjk.com/Article/details/gezzwjukh.sHtML

[T28] Swift：枚举
来源：http://read.share.vehdjk.com/Article/details/grofenjrc.sHtML

enum Color { case red, green }
来源：http://wap.bbcook.cn/Article/details/gbqqtoegp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.bbcook.cn/Article/details/giuntycuh.sHtML

guard let x = opt else { return }
来源：http://www.m.share.vehdjk.com/Article/details/gejhfexky.sHtML

[T30] Swift：协议
来源：http://3g.epnwcf.com/Article/details/gdrcpoxhn.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.epnwcf.com/Article/details/gxwjawmea.sHtML

[T31] Lua：Hello World
来源：http://baike.epnwcf.com/Article/details/gkildfaqs.sHtML

print("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gypkafslw.sHtML

[T32] Lua：局部变量
来源：http://www.share.fktsv.cn/Article/details/gwpsbxowv.sHtML

local a = 1
来源：http://read.share.sjlbkw.cn/Article/details/gltjvlznm.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.vehdjk.com/Article/details/gymrofdzd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.bbcook.cn/Article/details/grjmkbnyt.sHtML

[T34] Lua：遍历表
来源：http://wap.bbcook.cn/Article/details/grlkeqqzv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.vehdjk.com/Article/details/gpmrwuose.sHtML

[T35] Lua：字典表
来源：http://www.m.share.yfazqb.com/Article/details/ggaacecad.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.epnwcf.com/Article/details/goysasohy.sHtML

[T36] Lua：函数
来源：http://www.m.share.bbcook.cn/Article/details/gpqgdqzdm.sHtML

function add(a, b) return a + b end
来源：http://m.share.fktsv.cn/Article/details/gzsrodryv.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gxgdgqohc.sHtML

"a" .. "b"
来源：http://blog.yfazqb.com/Article/details/gbjsxdkbp.sHtML

[T38] Lua：条件
来源：http://m.share.fktsv.cn/Article/details/gqsnxfcmv.sHtML

if x > 0 then print("正") end
来源：http://www.share.fktsv.cn/Article/details/gzzguzfcl.sHtML

[T39] Lua：模式匹配
来源：http://3g.yfazqb.com/Article/details/gjlpbedwe.sHtML

string.find(s, "%d+")
来源：http://3g.tarul.cn/Article/details/gpqnloium.sHtML

[T40] Lua：元表
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqmjpjnk.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.epnwcf.com/Article/details/gknmiahgb.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fktsv.cn/Article/details/ggygtkdkk.sHtML

print "Hello\n";
来源：http://3g.yfazqb.com/Article/details/glpjzyxia.sHtML

[T42] Perl：变量类型
来源：http://www.share.tarul.cn/Article/details/gkmhbwepf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fktsv.cn/Article/details/gjzcfacxm.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/goqtoenpn.sHtML

"值: $a"
来源：http://3g.bbcook.cn/Article/details/gozgtbkru.sHtML

[T44] Perl：条件
来源：http://3g.yfazqb.com/Article/details/guuorueux.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.yfazqb.com/Article/details/gelavkesz.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.bbcook.cn/Article/details/gklmtwzns.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fktsv.cn/Article/details/gckszpfnw.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.yfazqb.com/Article/details/gzlnbdxdh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.tarul.cn/Article/details/ggzjeeqxl.sHtML

[T47] Perl：正则捕获
来源：http://3g.epnwcf.com/Article/details/gkfviwzcb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.yfazqb.com/Article/details/gnuxxxvvt.sHtML

[T48] Perl：正则替换
来源：http://wap.yfazqb.com/Article/details/gdpeitlgw.sHtML

$s =~ s/old/new/g;
来源：http://read.share.sjlbkw.cn/Article/details/gvvlixdle.sHtML

[T49] Perl：函数
来源：http://mobile.sjlbkw.cn/Article/details/gkwlpfujl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/guamdnpjj.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gxkhdngdi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.bbcook.cn/Article/details/gdtwetxrn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.yfazqb.com/Article/details/ggkubeham.sHtML

[T51] Scala：Hello World
来源：http://mobile.fktsv.cn/Article/details/gzkotbpwx.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/glebrlmcd.sHtML

[T52] Scala：变量
来源：http://www.share.bbcook.cn/Article/details/glufdlvsy.sHtML

val a = 1;  var b = 2
来源：http://blog.epnwcf.com/Article/details/gykwdwvmv.sHtML

[T53] Scala：字符串插值
来源：http://read.share.tarul.cn/Article/details/gyxscaebi.sHtML

s"值: $b"
来源：http://3g.bbcook.cn/Article/details/gatsljtdl.sHtML

[T54] Scala：集合映射
来源：http://3g.sjlbkw.cn/Article/details/gitrukebc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.bbcook.cn/Article/details/gziiulqyp.sHtML

[T55] Scala：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/gwyfowlvu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.tarul.cn/Article/details/gdghwcbgl.sHtML

[T56] Scala：样例类
来源：http://read.share.vehdjk.com/Article/details/grsuhdhmy.sHtML

case class User(name: String, age: Int)
来源：http://m.share.vehdjk.com/Article/details/gnylrkajz.sHtML

[T57] Scala：模式匹配
来源：http://m.share.bbcook.cn/Article/details/gnlsugcks.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.bbcook.cn/Article/details/gflrazmsl.sHtML

[T58] Scala：函数定义
来源：http://m.share.vehdjk.com/Article/details/gxqnnodjt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fktsv.cn/Article/details/gftaucxlr.sHtML

[T59] Scala：循环
来源：http://www.m.share.tarul.cn/Article/details/gdcflzxxf.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.epnwcf.com/Article/details/gsheducqn.sHtML

[T60] Scala：折叠
来源：http://www.blog.epnwcf.com/Article/details/gpjefxrqn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fktsv.cn/Article/details/gvbfnsmju.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gbanniyxj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.epnwcf.com/Article/details/gtoypwind.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/guyrwvvxn.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.vehdjk.com/Article/details/gzsposqkp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.tarul.cn/Article/details/gsmwuwszy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fktsv.cn/Article/details/ggzgrjslt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.sjlbkw.cn/Article/details/gbpjpqufo.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.yfazqb.com/Article/details/guxyoccii.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.sjlbkw.cn/Article/details/gjmhcpksb.sHtML

[U04] Py：变量调试打印
来源：http://mobile.epnwcf.com/Article/details/gqpjvmnff.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.tarul.cn/Article/details/gxvhkkyiq.sHtML

[U05] Py：列表去重且保序
来源：http://3g.vehdjk.com/Article/details/gizgbcsvn.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fktsv.cn/Article/details/gbfbcsmxu.sHtML

[U06] Py：合并两个字典
来源：http://baike.tarul.cn/Article/details/gbwswxqby.sHtML

{**a, **b}
来源：http://m.share.epnwcf.com/Article/details/gtsgfltsg.sHtML

[U07] Py：反转字典键值
来源：http://read.share.sjlbkw.cn/Article/details/gfrdojubp.sHtML

{v: k for k, v in d.items()}
来源：http://blog.sjlbkw.cn/Article/details/gdstadtiu.sHtML

[U08] Py：展平二维列表
来源：http://mobile.bbcook.cn/Article/details/gyrvkztwb.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.tarul.cn/Article/details/gmstqjblj.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.tarul.cn/Article/details/geahoamxv.sHtML

max(d, key=d.get)
来源：http://m.share.sjlbkw.cn/Article/details/gcvdoztto.sHtML

[U10] Py：按值排序字典
来源：http://baike.bbcook.cn/Article/details/ghirjsrmr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.sjlbkw.cn/Article/details/gnagbjlps.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.bbcook.cn/Article/details/gewzansie.sHtML

(x * 2 for x in arr)
来源：http://blog.fktsv.cn/Article/details/gqkshstwq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.vehdjk.com/Article/details/gaiyqwvzn.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.vehdjk.com/Article/details/gensryrvn.sHtML

[U13] Py：固定长度队列
来源：http://baike.fktsv.cn/Article/details/gsdohrzkp.sHtML

deque(maxlen=10)
来源：http://m.share.vehdjk.com/Article/details/gxnfbiguc.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.epnwcf.com/Article/details/grvsrthyy.sHtML

defaultdict(list)
来源：http://blog.yfazqb.com/Article/details/gwcxoehjf.sHtML

[U15] Py：高精度计时
来源：http://mobile.fktsv.cn/Article/details/giyyuphud.sHtML

t = time.perf_counter()
来源：http://blog.vehdjk.com/Article/details/gjzhrfnmc.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.vehdjk.com/Article/details/gjxeauasw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.sjlbkw.cn/Article/details/gzkaueouz.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxfisjhf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.yfazqb.com/Article/details/gnyeruniz.sHtML

[U18] Py：预编译正则
来源：http://3g.yfazqb.com/Article/details/gieguzymy.sHtML

pat = re.compile(r"\d+")
来源：http://wap.vehdjk.com/Article/details/gkljnwffd.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fktsv.cn/Article/details/ghedvecwv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.tarul.cn/Article/details/gwqfcplxs.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fktsv.cn/Article/details/gcasyrrir.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.sjlbkw.cn/Article/details/gsqskjqbj.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.vehdjk.com/Article/details/gebtehsbj.sHtML

@contextlib.contextmanager
来源：http://wap.bbcook.cn/Article/details/gfbnusaiv.sHtML

[U22] Py：矩阵转置
来源：http://3g.sjlbkw.cn/Article/details/goqacaphn.sHtML

list(zip(*m))
来源：http://mobile.tarul.cn/Article/details/gswgaeibe.sHtML

[U23] Py：分块读取大文件
来源：http://blog.vehdjk.com/Article/details/ggurqqazn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.yfazqb.com/Article/details/grjhquuff.sHtML

[U24] Py：路径操作
来源：http://www.share.bbcook.cn/Article/details/gfjxssxrc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/ghlqyyufn.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.tarul.cn/Article/details/ghuxtyduj.sHtML

csv.DictReader(f)
来源：http://www.share.tarul.cn/Article/details/gecsglkyv.sHtML

[U26] Py：并发下载
来源：http://read.share.sjlbkw.cn/Article/details/glqkgsykn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.yfazqb.com/Article/details/gubtyxlis.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.epnwcf.com/Article/details/getjzqvyd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.epnwcf.com/Article/details/ghvlohbgk.sHtML

[U28] Py：类型别名
来源：http://blog.fktsv.cn/Article/details/galgsnyvh.sHtML

UserId = int
来源：http://www.m.share.fktsv.cn/Article/details/gakmnukop.sHtML

[U29] Py：属性校验
来源：http://read.share.vehdjk.com/Article/details/gmsmpszbm.sHtML

@property 与 @x.setter 配合
来源：http://m.share.tarul.cn/Article/details/gmevbarim.sHtML

[U30] Py：数据类
来源：http://m.share.epnwcf.com/Article/details/gnfzeehkz.sHtML

@dataclass(slots=True)
来源：http://3g.tarul.cn/Article/details/gitelzlmh.sHtML

[U31] Py：单测
来源：http://www.share.fktsv.cn/Article/details/guktjvqor.sHtML

python -m pytest -q
来源：http://m.share.vehdjk.com/Article/details/gyjvwyglq.sHtML

[U32] Py：代码格式化
来源：http://wap.tarul.cn/Article/details/gcxqqpvlb.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.sjlbkw.cn/Article/details/gyxmkbygi.sHtML

[U33] Py：打包发布
来源：http://blog.vehdjk.com/Article/details/grutqvwqp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.tarul.cn/Article/details/gaynlygtm.sHtML

[U34] Py：判断编码
来源：http://read.share.bbcook.cn/Article/details/gyyaooxok.sHtML

chardet.detect(raw)
来源：http://www.share.fktsv.cn/Article/details/gaullwuxg.sHtML

[U35] Py：发送邮件
来源：http://3g.yfazqb.com/Article/details/gungzuuav.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.tarul.cn/Article/details/gtckwptfa.sHtML

[U36] Py：定时任务
来源：http://baike.bbcook.cn/Article/details/gsjhbwsgq.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.yfazqb.com/Article/details/giuhhfjxj.sHtML

[U37] Py：读写 Excel
来源：http://m.share.vehdjk.com/Article/details/gjwtlzfnd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.yfazqb.com/Article/details/gejcnlkvr.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.yfazqb.com/Article/details/ghiklroaw.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.bbcook.cn/Article/details/gxwtzmzlu.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.tarul.cn/Article/details/gmvzysfxg.sHtML

sys.stdout.isatty()
来源：http://www.blog.epnwcf.com/Article/details/guhwdrxhl.sHtML

[U40] Py：打印到标准错误
来源：http://wap.yfazqb.com/Article/details/gnzviicty.sHtML

print("err", file=sys.stderr)
来源：http://read.share.yfazqb.com/Article/details/gncxigolz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.vehdjk.com/Article/details/gvxieqjlu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.vehdjk.com/Article/details/gwsmyywlo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.sjlbkw.cn/Article/details/gtnlmille.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.sjlbkw.cn/Article/details/gzsrefetr.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.yfazqb.com/Article/details/gwhflfnlu.sHtML

namespace App\Http;
来源：http://3g.epnwcf.com/Article/details/gvehrllam.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.epnwcf.com/Article/details/gyoolhdot.sHtML

declare(strict_types=1);
来源：http://www.blog.sjlbkw.cn/Article/details/gefybenzw.sHtML


<!-- 参考信息 -->