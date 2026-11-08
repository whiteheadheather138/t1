代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：https://qg.zhonguo7118.cn

[S08] C：动态内存分配与释放
来源：https://xy.zhonguo8118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://ha.zhonguo6118.cn

[S09] C：结构体定义与初始化
来源：https://fd.zhonguo5118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://pa.zhonguo5118.cn

[S10] C：指针与解引用
来源：https://jz.zhonguo3118.cn

int *p = &a;  *p = 5;
来源：https://cz.zhonguo8118.cn

[S11] C：逐行读文件
来源：https://ox.zhonguo3118.cn

FILE *f = fopen("a.txt", "r");
来源：https://ty.zhonguo7118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://nu.zhonguo6118.cn

fclose(f);
来源：https://zj.zhonguo3118.cn

[S12] C：写文件
来源：https://iu.zhonguo3118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://be.zhonguo3118.cn

[S13] C：宏定义
来源：https://cv.zhonguo7118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://qf.zhonguo2118.cn

[S14] C：枚举
来源：https://ea.zhonguo2118.cn

enum Color { RED, GREEN, BLUE };
来源：https://xk.zhonguo4118.cn

[S15] C：类型转换
来源：https://ik.zhonguo7118.cn

(double) a / b
来源：https://eb.zhonguo7118.cn

[S16] C：位操作置位
来源：https://eb.zhonguo4118.cn

x |= (1 << 3);
来源：https://bf.zhonguo5118.cn

[S17] C：安全拼接字符串
来源：https://nb.zhonguo4118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://di.zhonguo7118.cn

[S18] C：命令行参数
来源：https://rt.zhonguo8118.cn

int main(int argc, char **argv)
来源：https://fx.zhonguo8118.cn

[S19] C：快速排序
来源：https://zj.zhonguo6118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://fl.zhonguo3118.cn

[S20] C：二分查找
来源：https://zq.zhonguo5118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://rl.zhonguo4118.cn

[S21] C：字符类别判断
来源：https://om.zhonguo4118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://xn.zhonguo7118.cn

[S22] C：字符串转数字
来源：https://rs.zhonguo4118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://mj.zhonguo1118.cn

[S23] C：随机数
来源：https://st.zhonguo6118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://gq.zhonguo4118.cn

[S24] C：获取本地时间
来源：https://uq.zhonguo7118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://ck.zhonguo5118.cn

[S25] C：内存拷贝
来源：https://um.zhonguo7118.cn

memcpy(dst, src, n);
来源：https://gq.zhonguo6118.cn

[S26] C：内存清零
来源：https://ux.zhonguo5118.cn

memset(a, 0, sizeof a);
来源：https://ja.zhonguo4118.cn

[S27] C：定义常量
来源：https://tn.zhonguo4118.cn

const double PI = 3.14159;
来源：https://zm.zhonguo3118.cn

[S28] C：静态变量
来源：https://ip.zhonguo4118.cn

static int counter = 0;
来源：https://yz.zhonguo4118.cn

[S29] C：变参函数
来源：https://gz.zhonguo2118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://pa.zhonguo4118.cn

[S30] C：头文件保护
来源：https://bl.zhonguo6118.cn

#ifndef X_H
来源：https://qr.zhonguo3118.cn

#define X_H
来源：https://md.zhonguo1118.cn

#endif
来源：https://hw.zhonguo7118.cn

[S31] C++：Hello World
来源：https://iu.zhonguo7118.cn

#include <iostream>
来源：https://oh.zhonguo3118.cn

int main() { std::cout << "Hello\n"; }
来源：https://mv.zhonguo1118.cn

[S32] C++：字符串
来源：https://so.zhonguo6118.cn

std::string s = "hi";  s += "!";
来源：https://ye.zhonguo4118.cn

[S33] C++：vector 增删
来源：https://su.zhonguo1118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://xs.zhonguo1118.cn

[S34] C++：遍历 vector
来源：https://po.zhonguo5118.cn

for (auto &x : v) { std::cout << x; }
来源：https://qy.zhonguo3118.cn

[S35] C++：map
来源：https://nn.zhonguo1118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://tv.zhonguo8118.cn

[S36] C++：unordered_map
来源：https://oo.zhonguo4118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://vs.zhonguo1118.cn

[S37] C++：set
来源：https://xv.zhonguo7118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://om.zhonguo2118.cn

[S38] C++：排序
来源：https://wc.zhonguo5118.cn

std::sort(v.begin(), v.end());
来源：https://bu.zhonguo6118.cn

[S39] C++：自定义比较器排序
来源：https://uv.zhonguo3118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://lp.zhonguo5118.cn

[S40] C++：查找元素
来源：https://tx.zhonguo5118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://uo.zhonguo1118.cn

[S41] C++：类与构造函数
来源：https://rp.zhonguo5118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://rg.zhonguo6118.cn

[S42] C++：继承与虚函数
来源：https://ou.zhonguo3118.cn

class B : public Base { public: void f() override {} };
来源：https://ju.zhonguo1118.cn

[S43] C++：智能指针
来源：https://bh.zhonguo6118.cn

auto p = std::make_unique<int>(5);
来源：https://qx.zhonguo3118.cn

[S44] C++：引用传参
来源：https://jk.zhonguo8118.cn

void inc(int &x) { ++x; }
来源：https://im.zhonguo1118.cn

[S45] C++：lambda
来源：https://od.zhonguo6118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://so.zhonguo7118.cn

[S46] C++：函数模板
来源：https://oi.zhonguo3118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://kg.zhonguo7118.cn

[S47] C++：结构化绑定遍历
来源：https://fz.zhonguo2118.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：https://es.zhonguo1118.cn

[S48] C++：逐行读文件
来源：https://ov.zhonguo2118.cn

std::ifstream in("a.txt");  std::string line;
来源：https://et.zhonguo8118.cn

while (std::getline(in, line)) { }
来源：https://ir.zhonguo8118.cn

[S49] C++：写文件
来源：https://wf.zhonguo1118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://hy.zhonguo5118.cn

[S50] C++：格式化数字
来源：https://lf.zhonguo6118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://ah.zhonguo1118.cn

[S51] C++：显式类型转换
来源：https://bx.zhonguo8118.cn

static_cast<double>(a) / b
来源：https://fe.zhonguo7118.cn

[S52] C++：const 与 noexcept
来源：https://vo.zhonguo8118.cn

int size() const noexcept { return n_; }
来源：https://yk.zhonguo5118.cn

[S53] C++：移动语义
来源：https://xu.zhonguo4118.cn

std::vector<int> w = std::move(v);
来源：https://xg.zhonguo5118.cn

[S54] C++：异常处理
来源：https://uh.zhonguo1118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://op.zhonguo7118.cn

[S55] C++：结构化绑定
来源：https://le.zhonguo6118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://to.zhonguo1118.cn

[S56] C++：optional
来源：https://xk.zhonguo6118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://ow.zhonguo6118.cn

[S57] C++：编译期常量
来源：https://cl.zhonguo2118.cn

constexpr int N = 10;
来源：https://qw.zhonguo7118.cn

[S58] C++：命名空间
来源：https://ra.zhonguo8118.cn

namespace ns { int f() { return 1; } }
来源：https://qw.zhonguo5118.cn

[S59] C++：静态断言
来源：https://vp.zhonguo8118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://jz.zhonguo5118.cn

[S60] C++：遍历并删除元素
来源：https://ip.zhonguo1118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://kz.zhonguo8118.cn

================================================================================
来源：https://el.zhonguo3118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://zz.zhonguo1118.cn

================================================================================
来源：https://pi.zhonguo3118.cn

[T01] Kotlin：Hello World
来源：https://jx.zhonguo3118.cn

println("Hello")
来源：https://pc.zhonguo7118.cn

[T02] Kotlin：变量
来源：https://mf.zhonguo4118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://fu.zhonguo8118.cn

[T03] Kotlin：字符串模板
来源：https://xj.zhonguo8118.cn

"值: $b"
来源：https://lg.zhonguo4118.cn

[T04] Kotlin：空安全
来源：https://ch.zhonguo2118.cn

val n: String? = null;  n?.length
来源：https://vv.zhonguo7118.cn

[T05] Kotlin：when 表达式
来源：https://id.zhonguo7118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://pg.zhonguo1118.cn

[T06] Kotlin：集合映射
来源：https://ty.zhonguo7118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://kd.zhonguo3118.cn

[T07] Kotlin：集合过滤
来源：https://qu.zhonguo6118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://sx.zhonguo6118.cn

[T08] Kotlin：数据类
来源：https://zn.zhonguo2118.cn

data class User(val name: String, val age: Int)
来源：https://hp.zhonguo8118.cn

[T09] Kotlin：扩展函数
来源：https://vr.zhonguo7118.cn

fun String.exclaim() = this + "!"
来源：https://rw.zhonguo2118.cn

[T10] Kotlin：默认参数
来源：https://vo.zhonguo5118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://ny.zhonguo7118.cn

[T11] Kotlin：协程
来源：https://cs.zhonguo2118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://to.zhonguo2118.cn

[T12] Kotlin：解构声明
来源：https://uv.zhonguo7118.cn

val (a, b) = Pair(1, 2)
来源：https://vb.zhonguo8118.cn

[T13] Kotlin：只读 Map
来源：https://lg.zhonguo3118.cn

val m = mapOf("a" to 1)
来源：https://aq.zhonguo6118.cn

[T14] Kotlin：循环
来源：https://yv.zhonguo8118.cn

for (i in 1..10) println(i)
来源：https://px.zhonguo6118.cn

[T15] Kotlin：接口
来源：https://rn.zhonguo7118.cn

interface Shape { fun area(): Double }
来源：https://ho.zhonguo8118.cn

[T16] Swift：Hello World
来源：https://rx.zhonguo1118.cn

print("Hello")
来源：https://vl.zhonguo2118.cn

[T17] Swift：变量与常量
来源：https://tk.zhonguo5118.cn

var a = 1;  let b = 2
来源：https://tb.zhonguo7118.cn

[T18] Swift：字符串插值
来源：https://kp.zhonguo6118.cn

"值: \(b)"
来源：https://vt.zhonguo5118.cn

[T19] Swift：可选绑定
来源：https://cl.zhonguo2118.cn

if let n = opt { print(n) }
来源：https://em.zhonguo3118.cn

[T20] Swift：数组操作
来源：https://xt.zhonguo8118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://up.zhonguo3118.cn

[T21] Swift：遍历
来源：https://ou.zhonguo8118.cn

for x in a { print(x) }
来源：https://kc.zhonguo1118.cn

[T22] Swift：字典
来源：https://so.zhonguo4118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://vl.zhonguo8118.cn

[T23] Swift：函数
来源：https://vy.zhonguo3118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://ds.zhonguo5118.cn

[T24] Swift：闭包
来源：https://fe.zhonguo4118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://qx.zhonguo2118.cn

[T25] Swift：结构体
来源：https://lh.zhonguo2118.cn

struct P { var x: Int }
来源：https://zk.zhonguo2118.cn

[T26] Swift：类与重写
来源：https://dq.zhonguo2118.cn

class A: Base { override func f() {} }
来源：https://xo.zhonguo8118.cn

[T27] Swift：错误处理
来源：https://wy.zhonguo2118.cn

do { try f() } catch { print(error) }
来源：https://rd.zhonguo3118.cn

[T28] Swift：枚举
来源：https://yl.zhonguo1118.cn

enum Color { case red, green }
来源：https://fj.zhonguo8118.cn

[T29] Swift：guard 提前返回
来源：https://wj.zhonguo3118.cn

guard let x = opt else { return }
来源：https://lu.zhonguo8118.cn

[T30] Swift：协议
来源：https://xb.zhonguo6118.cn

protocol Shape { func area() -> Double }
来源：https://ur.zhonguo3118.cn

[T31] Lua：Hello World
来源：https://or.zhonguo5118.cn

print("Hello")
来源：https://iv.zhonguo2118.cn

[T32] Lua：局部变量
来源：https://wa.zhonguo1118.cn

local a = 1
来源：https://ky.zhonguo6118.cn

[T33] Lua：表（数组）
来源：https://gu.zhonguo7118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://fi.zhonguo6118.cn

[T34] Lua：遍历表
来源：https://qm.zhonguo5118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://sn.zhonguo3118.cn

[T35] Lua：字典表
来源：https://he.zhonguo3118.cn

local d = { a = 1 };  d.b = 2
来源：https://xj.zhonguo6118.cn

[T36] Lua：函数
来源：https://ob.zhonguo5118.cn

function add(a, b) return a + b end
来源：https://fn.zhonguo7118.cn

[T37] Lua：字符串拼接
来源：https://vp.zhonguo5118.cn

"a" .. "b"
来源：https://mp.zhonguo7118.cn

[T38] Lua：条件
来源：https://td.zhonguo7118.cn

if x > 0 then print("正") end
来源：https://yh.zhonguo8118.cn

[T39] Lua：模式匹配
来源：https://sp.zhonguo4118.cn

string.find(s, "%d+")
来源：https://ka.zhonguo6118.cn

[T40] Lua：元表
来源：https://ns.zhonguo2118.cn

setmetatable({}, { __index = base })
来源：https://ol.zhonguo8118.cn

[T41] Perl：Hello World
来源：https://ee.zhonguo1118.cn

print "Hello\n";
来源：https://kd.zhonguo6118.cn

[T42] Perl：变量类型
来源：https://wm.zhonguo7118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://ih.zhonguo6118.cn

[T43] Perl：字符串插值
来源：https://ww.zhonguo2118.cn

"值: $a"
来源：https://me.zhonguo5118.cn

[T44] Perl：条件
来源：https://yg.zhonguo7118.cn

if ($a > 0) { print "正"; }
来源：https://mc.zhonguo1118.cn

[T45] Perl：数组遍历
来源：https://eo.zhonguo7118.cn

for my $x (@arr) { print $x; }
来源：https://ih.zhonguo5118.cn

[T46] Perl：哈希操作
来源：https://bg.zhonguo8118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://vx.zhonguo6118.cn

[T47] Perl：正则捕获
来源：https://zo.zhonguo6118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://fv.zhonguo5118.cn

[T48] Perl：正则替换
来源：https://hc.zhonguo5118.cn

$s =~ s/old/new/g;
来源：https://zs.zhonguo6118.cn

[T49] Perl：函数
来源：https://cz.zhonguo7118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://sw.zhonguo1118.cn

[T50] Perl：逐行读文件
来源：https://jn.zhonguo7118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://sm.zhonguo4118.cn

while (my $line = <$fh>) { print $line; }
来源：https://fu.zhonguo4118.cn

[T51] Scala：Hello World
来源：https://of.zhonguo8118.cn

println("Hello")
来源：https://mo.zhonguo4118.cn

[T52] Scala：变量
来源：https://ya.zhonguo3118.cn

val a = 1;  var b = 2
来源：https://ir.zhonguo5118.cn

[T53] Scala：字符串插值
来源：https://rw.zhonguo6118.cn

s"值: $b"
来源：https://dm.zhonguo7118.cn

[T54] Scala：集合映射
来源：https://qa.zhonguo8118.cn

List(1, 2, 3).map(_ * 2)
来源：https://qf.zhonguo4118.cn

[T55] Scala：集合过滤
来源：https://wn.zhonguo8118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://qb.zhonguo3118.cn

[T56] Scala：样例类
来源：https://ap.zhonguo4118.cn

case class User(name: String, age: Int)
来源：https://ud.zhonguo5118.cn

[T57] Scala：模式匹配
来源：https://dl.zhonguo7118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://sx.zhonguo3118.cn

[T58] Scala：函数定义
来源：https://sd.zhonguo6118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://mw.zhonguo7118.cn

[T59] Scala：循环
来源：https://dr.zhonguo1118.cn

for (i <- 1 to 10) println(i)
来源：https://xh.zhonguo4118.cn

[T60] Scala：折叠
来源：https://kh.zhonguo8118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://ct.zhonguo5118.cn

================================================================================
来源：https://no.zhonguo3118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://uv.zhonguo8118.cn

================================================================================
来源：https://ab.zhonguo3118.cn

[U01] Py：创建虚拟环境
来源：https://nl.zhonguo7118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://rr.zhonguo2118.cn

[U02] Py：导出 / 安装依赖
来源：https://ej.zhonguo1118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://ea.zhonguo5118.cn

[U03] Py：加载 .env 配置
来源：https://pt.zhonguo4118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://df.zhonguo6118.cn

[U04] Py：变量调试打印
来源：https://jz.zhonguo3118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://lt.zhonguo4118.cn

[U05] Py：列表去重且保序
来源：https://so.zhonguo1118.cn

list(dict.fromkeys(arr))
来源：https://gs.zhonguo2118.cn

[U06] Py：合并两个字典
来源：https://tp.zhonguo3118.cn

{**a, **b}
来源：https://em.zhonguo4118.cn

[U07] Py：反转字典键值
来源：https://up.zhonguo5118.cn

{v: k for k, v in d.items()}
来源：https://bi.zhonguo3118.cn

[U08] Py：展平二维列表
来源：https://so.zhonguo3118.cn

[y for x in nested for y in x]
来源：https://wa.zhonguo6118.cn

[U09] Py：字典取最大值的键
来源：https://rq.zhonguo2118.cn

max(d, key=d.get)
来源：https://bj.zhonguo1118.cn

[U10] Py：按值排序字典
来源：https://ts.zhonguo1118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://tz.zhonguo3118.cn

[U11] Py：生成器表达式
来源：https://jv.zhonguo5118.cn

(x * 2 for x in arr)
来源：https://mm.zhonguo1118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://oa.zhonguo6118.cn

Counter(arr).most_common(3)
来源：https://hp.zhonguo2118.cn

[U13] Py：固定长度队列
来源：https://fr.zhonguo3118.cn

deque(maxlen=10)
来源：https://wh.zhonguo7118.cn

[U14] Py：分组收集到列表
来源：https://ql.zhonguo7118.cn

defaultdict(list)
来源：https://pa.zhonguo6118.cn

[U15] Py：高精度计时
来源：https://wr.zhonguo8118.cn

t = time.perf_counter()
来源：https://fo.zhonguo8118.cn

[U16] Py：命令行参数解析
来源：https://qr.zhonguo7118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://dr.zhonguo1118.cn

[U17] Py：初始化日志
来源：https://wa.zhonguo5118.cn

logging.basicConfig(level=logging.INFO)
来源：https://dv.zhonguo3118.cn

[U18] Py：预编译正则
来源：https://po.zhonguo5118.cn

pat = re.compile(r"\d+")
来源：https://ds.zhonguo4118.cn

[U19] Py：正则替换带回调
来源：https://vu.zhonguo6118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://di.zhonguo5118.cn

[U20] Py：缓存函数结果
来源：https://zz.zhonguo6118.cn

@functools.lru_cache(maxsize=None)
来源：https://rq.zhonguo2118.cn

[U21] Py：自定义上下文管理器
来源：https://uj.zhonguo7118.cn

@contextlib.contextmanager
来源：https://iw.zhonguo4118.cn

[U22] Py：矩阵转置
来源：https://of.zhonguo3118.cn

list(zip(*m))
来源：https://xp.zhonguo7118.cn

[U23] Py：分块读取大文件
来源：https://lc.zhonguo4118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://tn.zhonguo2118.cn

[U24] Py：路径操作
来源：https://ez.zhonguo4118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://fa.zhonguo8118.cn

[U25] Py：CSV 按字典读
来源：https://em.zhonguo2118.cn

csv.DictReader(f)
来源：https://uk.zhonguo7118.cn

[U26] Py：并发下载
来源：https://ow.zhonguo3118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://qg.zhonguo1118.cn

[U27] Py：异步 HTTP
来源：https://vw.zhonguo7118.cn

aiohttp.ClientSession() 配合 async with
来源：https://vj.zhonguo1118.cn

[U28] Py：类型别名
来源：https://hu.zhonguo1118.cn

UserId = int
来源：https://ii.zhonguo8118.cn

[U29] Py：属性校验
来源：https://it.zhonguo7118.cn

@property 与 @x.setter 配合
来源：https://yy.zhonguo2118.cn

[U30] Py：数据类
来源：https://fo.zhonguo6118.cn

@dataclass(slots=True)
来源：https://ux.zhonguo2118.cn


<!-- 参考信息 -->