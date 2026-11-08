代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：https://tf.zhonguo6118.cn

[S08] C：动态内存分配与释放
来源：https://fj.zhonguo6118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://xo.zhonguo8118.cn

[S09] C：结构体定义与初始化
来源：https://qo.zhonguo8118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://ds.zhonguo8118.cn

[S10] C：指针与解引用
来源：https://dn.zhonguo7118.cn

int *p = &a;  *p = 5;
来源：https://cv.zhonguo1118.cn

[S11] C：逐行读文件
来源：https://ob.zhonguo1118.cn

FILE *f = fopen("a.txt", "r");
来源：https://pp.zhonguo1118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://fn.zhonguo5118.cn

fclose(f);
来源：https://qd.zhonguo3118.cn

[S12] C：写文件
来源：https://eg.zhonguo4118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://db.zhonguo6118.cn

[S13] C：宏定义
来源：https://kv.zhonguo4118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://qe.zhonguo2118.cn

[S14] C：枚举
来源：https://wl.zhonguo3118.cn

enum Color { RED, GREEN, BLUE };
来源：https://ik.zhonguo3118.cn

[S15] C：类型转换
来源：https://yd.zhonguo4118.cn

(double) a / b
来源：https://dn.zhonguo6118.cn

[S16] C：位操作置位
来源：https://iq.zhonguo5118.cn

x |= (1 << 3);
来源：https://gf.zhonguo4118.cn

[S17] C：安全拼接字符串
来源：https://oc.zhonguo2118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://xy.zhonguo4118.cn

[S18] C：命令行参数
来源：https://in.zhonguo3118.cn

int main(int argc, char **argv)
来源：https://of.zhonguo6118.cn

[S19] C：快速排序
来源：https://jr.zhonguo7118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://up.zhonguo7118.cn

[S20] C：二分查找
来源：https://ld.zhonguo7118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://up.zhonguo8118.cn

[S21] C：字符类别判断
来源：https://ah.zhonguo5118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://cj.zhonguo8118.cn

[S22] C：字符串转数字
来源：https://kp.zhonguo1118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://ek.zhonguo1118.cn

[S23] C：随机数
来源：https://xb.zhonguo3118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://yq.zhonguo3118.cn

[S24] C：获取本地时间
来源：https://dc.zhonguo2118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://sy.zhonguo4118.cn

[S25] C：内存拷贝
来源：https://eg.zhonguo7118.cn

memcpy(dst, src, n);
来源：https://bb.zhonguo5118.cn

[S26] C：内存清零
来源：https://ot.zhonguo3118.cn

memset(a, 0, sizeof a);
来源：https://hm.zhonguo1118.cn

[S27] C：定义常量
来源：https://sg.zhonguo4118.cn

const double PI = 3.14159;
来源：https://by.zhonguo2118.cn

[S28] C：静态变量
来源：https://ns.zhonguo8118.cn

static int counter = 0;
来源：https://go.zhonguo4118.cn

[S29] C：变参函数
来源：https://ps.zhonguo3118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://zu.zhonguo3118.cn

[S30] C：头文件保护
来源：https://td.zhonguo3118.cn

#ifndef X_H
来源：https://cx.zhonguo1118.cn

#define X_H
来源：https://lz.zhonguo7118.cn

#endif
来源：https://zv.zhonguo3118.cn

[S31] C++：Hello World
来源：https://rh.zhonguo2118.cn

#include <iostream>
来源：https://zm.zhonguo4118.cn

int main() { std::cout << "Hello\n"; }
来源：https://bz.zhonguo8118.cn

[S32] C++：字符串
来源：https://zm.zhonguo7118.cn

std::string s = "hi";  s += "!";
来源：https://qb.zhonguo5118.cn

[S33] C++：vector 增删
来源：https://oj.zhonguo7118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://pn.zhonguo8118.cn

[S34] C++：遍历 vector
来源：https://bs.zhonguo6118.cn

for (auto &x : v) { std::cout << x; }
来源：https://mu.zhonguo6118.cn

[S35] C++：map
来源：https://dg.zhonguo7118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://pc.zhonguo7118.cn

[S36] C++：unordered_map
来源：https://wb.zhonguo1118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://ju.zhonguo8118.cn

[S37] C++：set
来源：https://du.zhonguo2118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://dp.zhonguo8118.cn

[S38] C++：排序
来源：https://he.zhonguo3118.cn

std::sort(v.begin(), v.end());
来源：https://yi.zhonguo4118.cn

[S39] C++：自定义比较器排序
来源：https://ge.zhonguo5118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://gc.zhonguo7118.cn

[S40] C++：查找元素
来源：https://ko.zhonguo1118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://yi.zhonguo2118.cn

[S41] C++：类与构造函数
来源：https://ls.zhonguo3118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://ff.zhonguo3118.cn

[S42] C++：继承与虚函数
来源：https://ma.zhonguo8118.cn

class B : public Base { public: void f() override {} };
来源：https://qf.zhonguo5118.cn

[S43] C++：智能指针
来源：https://to.zhonguo7118.cn

auto p = std::make_unique<int>(5);
来源：https://ka.zhonguo2118.cn

[S44] C++：引用传参
来源：https://ax.zhonguo3118.cn

void inc(int &x) { ++x; }
来源：https://ir.zhonguo6118.cn

[S45] C++：lambda
来源：https://bs.zhonguo4118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://tu.zhonguo1118.cn

[S46] C++：函数模板
来源：https://sa.zhonguo4118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://uk.zhonguo3118.cn

[S47] C++：结构化绑定遍历
来源：https://wq.zhonguo6118.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：https://py.zhonguo2118.cn

[S48] C++：逐行读文件
来源：https://zd.zhonguo3118.cn

std::ifstream in("a.txt");  std::string line;
来源：https://nj.zhonguo3118.cn

while (std::getline(in, line)) { }
来源：https://ae.zhonguo8118.cn

[S49] C++：写文件
来源：https://wj.zhonguo5118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://nr.zhonguo7118.cn

[S50] C++：格式化数字
来源：https://mq.zhonguo6118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://xt.zhonguo2118.cn

[S51] C++：显式类型转换
来源：https://kx.zhonguo7118.cn

static_cast<double>(a) / b
来源：https://iy.zhonguo3118.cn

[S52] C++：const 与 noexcept
来源：https://sa.zhonguo1118.cn

int size() const noexcept { return n_; }
来源：https://ze.zhonguo8118.cn

[S53] C++：移动语义
来源：https://fg.zhonguo2118.cn

std::vector<int> w = std::move(v);
来源：https://rm.zhonguo5118.cn

[S54] C++：异常处理
来源：https://cl.zhonguo5118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://hi.zhonguo8118.cn

[S55] C++：结构化绑定
来源：https://ij.zhonguo1118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://zq.zhonguo4118.cn

[S56] C++：optional
来源：https://bb.zhonguo8118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://bu.zhonguo1118.cn

[S57] C++：编译期常量
来源：https://yb.zhonguo8118.cn

constexpr int N = 10;
来源：https://pc.zhonguo8118.cn

[S58] C++：命名空间
来源：https://mj.zhonguo4118.cn

namespace ns { int f() { return 1; } }
来源：https://ee.zhonguo2118.cn

[S59] C++：静态断言
来源：https://mx.zhonguo5118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://zj.zhonguo7118.cn

[S60] C++：遍历并删除元素
来源：https://cw.zhonguo6118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://rh.zhonguo3118.cn

================================================================================
来源：https://lr.zhonguo7118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://rt.zhonguo4118.cn

================================================================================
来源：https://yn.zhonguo1118.cn

[T01] Kotlin：Hello World
来源：https://ih.zhonguo3118.cn

println("Hello")
来源：https://ds.zhonguo5118.cn

[T02] Kotlin：变量
来源：https://zy.zhonguo7118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://dq.zhonguo7118.cn

[T03] Kotlin：字符串模板
来源：https://bu.zhonguo1118.cn

"值: $b"
来源：https://vd.zhonguo1118.cn

[T04] Kotlin：空安全
来源：https://zm.zhonguo7118.cn

val n: String? = null;  n?.length
来源：https://ec.zhonguo7118.cn

[T05] Kotlin：when 表达式
来源：https://be.zhonguo8118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://wz.zhonguo5118.cn

[T06] Kotlin：集合映射
来源：https://is.zhonguo4118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://er.zhonguo3118.cn

[T07] Kotlin：集合过滤
来源：https://gg.zhonguo4118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://qy.zhonguo5118.cn

[T08] Kotlin：数据类
来源：https://tt.zhonguo4118.cn

data class User(val name: String, val age: Int)
来源：https://gf.zhonguo2118.cn

[T09] Kotlin：扩展函数
来源：https://lu.zhonguo3118.cn

fun String.exclaim() = this + "!"
来源：https://qt.zhonguo3118.cn

[T10] Kotlin：默认参数
来源：https://yz.zhonguo6118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://wq.zhonguo4118.cn

[T11] Kotlin：协程
来源：https://fs.zhonguo3118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://jk.zhonguo6118.cn

[T12] Kotlin：解构声明
来源：https://og.zhonguo6118.cn

val (a, b) = Pair(1, 2)
来源：https://kg.zhonguo7118.cn

[T13] Kotlin：只读 Map
来源：https://sn.zhonguo6118.cn

val m = mapOf("a" to 1)
来源：https://fg.zhonguo1118.cn

[T14] Kotlin：循环
来源：https://kf.zhonguo6118.cn

for (i in 1..10) println(i)
来源：https://tz.zhonguo4118.cn

[T15] Kotlin：接口
来源：https://lg.zhonguo1118.cn

interface Shape { fun area(): Double }
来源：https://bb.zhonguo1118.cn

[T16] Swift：Hello World
来源：https://fw.zhonguo4118.cn

print("Hello")
来源：https://df.zhonguo1118.cn

[T17] Swift：变量与常量
来源：https://tw.zhonguo6118.cn

var a = 1;  let b = 2
来源：https://pm.zhonguo6118.cn

[T18] Swift：字符串插值
来源：https://gt.zhonguo2118.cn

"值: \(b)"
来源：https://vp.zhonguo1118.cn

[T19] Swift：可选绑定
来源：https://rj.zhonguo7118.cn

if let n = opt { print(n) }
来源：https://us.zhonguo1118.cn

[T20] Swift：数组操作
来源：https://sz.zhonguo3118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://ct.zhonguo6118.cn

[T21] Swift：遍历
来源：https://nq.zhonguo5118.cn

for x in a { print(x) }
来源：https://hx.zhonguo3118.cn

[T22] Swift：字典
来源：https://sv.zhonguo1118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://yg.zhonguo7118.cn

[T23] Swift：函数
来源：https://oa.zhonguo2118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://ig.zhonguo4118.cn

[T24] Swift：闭包
来源：https://ac.zhonguo6118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://ar.zhonguo3118.cn

[T25] Swift：结构体
来源：https://hx.zhonguo8118.cn

struct P { var x: Int }
来源：https://sy.zhonguo7118.cn

[T26] Swift：类与重写
来源：https://bj.zhonguo1118.cn

class A: Base { override func f() {} }
来源：https://yy.zhonguo7118.cn

[T27] Swift：错误处理
来源：https://yj.zhonguo6118.cn

do { try f() } catch { print(error) }
来源：https://yr.zhonguo6118.cn

[T28] Swift：枚举
来源：https://av.zhonguo1118.cn

enum Color { case red, green }
来源：https://mi.zhonguo6118.cn

[T29] Swift：guard 提前返回
来源：https://sm.zhonguo5118.cn

guard let x = opt else { return }
来源：https://uy.zhonguo6118.cn

[T30] Swift：协议
来源：https://ws.zhonguo6118.cn

protocol Shape { func area() -> Double }
来源：https://fi.zhonguo6118.cn

[T31] Lua：Hello World
来源：https://gs.zhonguo8118.cn

print("Hello")
来源：https://vy.zhonguo8118.cn

[T32] Lua：局部变量
来源：https://rh.zhonguo2118.cn

local a = 1
来源：https://wy.zhonguo6118.cn

[T33] Lua：表（数组）
来源：https://wq.zhonguo5118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://by.zhonguo7118.cn

[T34] Lua：遍历表
来源：https://lt.zhonguo2118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://yb.zhonguo7118.cn

[T35] Lua：字典表
来源：https://yj.zhonguo1118.cn

local d = { a = 1 };  d.b = 2
来源：https://nv.zhonguo7118.cn

[T36] Lua：函数
来源：https://dz.zhonguo2118.cn

function add(a, b) return a + b end
来源：https://oy.zhonguo5118.cn

[T37] Lua：字符串拼接
来源：https://mq.zhonguo4118.cn

"a" .. "b"
来源：https://aw.zhonguo6118.cn

[T38] Lua：条件
来源：https://cf.zhonguo7118.cn

if x > 0 then print("正") end
来源：https://zw.zhonguo2118.cn

[T39] Lua：模式匹配
来源：https://mh.zhonguo4118.cn

string.find(s, "%d+")
来源：https://rv.zhonguo2118.cn

[T40] Lua：元表
来源：https://sr.zhonguo4118.cn

setmetatable({}, { __index = base })
来源：https://uf.zhonguo4118.cn

[T41] Perl：Hello World
来源：https://sk.zhonguo8118.cn

print "Hello\n";
来源：https://hh.zhonguo1118.cn

[T42] Perl：变量类型
来源：https://ue.zhonguo4118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://tp.zhonguo8118.cn

[T43] Perl：字符串插值
来源：https://jr.zhonguo1118.cn

"值: $a"
来源：https://wr.zhonguo4118.cn

[T44] Perl：条件
来源：https://my.zhonguo8118.cn

if ($a > 0) { print "正"; }
来源：https://cs.zhonguo1118.cn

[T45] Perl：数组遍历
来源：https://wc.zhonguo2118.cn

for my $x (@arr) { print $x; }
来源：https://tg.zhonguo1118.cn

[T46] Perl：哈希操作
来源：https://kx.zhonguo5118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://yt.zhonguo3118.cn

[T47] Perl：正则捕获
来源：https://wi.zhonguo8118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://jw.zhonguo8118.cn

[T48] Perl：正则替换
来源：https://xo.zhonguo6118.cn

$s =~ s/old/new/g;
来源：https://jl.zhonguo6118.cn

[T49] Perl：函数
来源：https://wq.zhonguo5118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://zi.zhonguo2118.cn

[T50] Perl：逐行读文件
来源：https://qy.zhonguo6118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://ko.zhonguo2118.cn

while (my $line = <$fh>) { print $line; }
来源：https://me.zhonguo6118.cn

[T51] Scala：Hello World
来源：https://oh.zhonguo8118.cn

println("Hello")
来源：https://vi.zhonguo6118.cn

[T52] Scala：变量
来源：https://zf.zhonguo6118.cn

val a = 1;  var b = 2
来源：https://vm.zhonguo3118.cn

[T53] Scala：字符串插值
来源：https://xe.zhonguo5118.cn

s"值: $b"
来源：https://go.zhonguo6118.cn

[T54] Scala：集合映射
来源：https://ev.zhonguo6118.cn

List(1, 2, 3).map(_ * 2)
来源：https://ce.zhonguo3118.cn

[T55] Scala：集合过滤
来源：https://xm.zhonguo2118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://gl.zhonguo5118.cn

[T56] Scala：样例类
来源：https://ij.zhonguo7118.cn

case class User(name: String, age: Int)
来源：https://ql.zhonguo4118.cn

[T57] Scala：模式匹配
来源：https://hh.zhonguo2118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://yo.zhonguo5118.cn

[T58] Scala：函数定义
来源：https://xe.zhonguo8118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://pf.zhonguo6118.cn

[T59] Scala：循环
来源：https://pj.zhonguo8118.cn

for (i <- 1 to 10) println(i)
来源：https://nz.zhonguo3118.cn

[T60] Scala：折叠
来源：https://jy.zhonguo1118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://xw.zhonguo6118.cn

================================================================================
来源：https://ii.zhonguo2118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://ve.zhonguo4118.cn

================================================================================
来源：https://vk.zhonguo5118.cn

[U01] Py：创建虚拟环境
来源：https://nk.zhonguo4118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://hn.zhonguo5118.cn

[U02] Py：导出 / 安装依赖
来源：https://na.zhonguo2118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://rn.zhonguo5118.cn

[U03] Py：加载 .env 配置
来源：https://vs.zhonguo1118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://vi.zhonguo4118.cn

[U04] Py：变量调试打印
来源：https://un.zhonguo5118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://dp.zhonguo7118.cn

[U05] Py：列表去重且保序
来源：https://jt.zhonguo8118.cn

list(dict.fromkeys(arr))
来源：https://nq.zhonguo4118.cn

[U06] Py：合并两个字典
来源：https://pm.zhonguo7118.cn

{**a, **b}
来源：https://ds.zhonguo2118.cn

[U07] Py：反转字典键值
来源：https://sy.zhonguo7118.cn

{v: k for k, v in d.items()}
来源：https://tt.zhonguo6118.cn

[U08] Py：展平二维列表
来源：https://ty.zhonguo8118.cn

[y for x in nested for y in x]
来源：https://wi.zhonguo2118.cn

[U09] Py：字典取最大值的键
来源：https://jg.zhonguo2118.cn

max(d, key=d.get)
来源：https://ab.zhonguo4118.cn

[U10] Py：按值排序字典
来源：https://ro.zhonguo2118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://vo.zhonguo1118.cn

[U11] Py：生成器表达式
来源：https://nr.zhonguo3118.cn

(x * 2 for x in arr)
来源：https://gr.zhonguo7118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://ts.zhonguo3118.cn

Counter(arr).most_common(3)
来源：https://we.zhonguo7118.cn

[U13] Py：固定长度队列
来源：https://up.zhonguo2118.cn

deque(maxlen=10)
来源：https://kc.zhonguo8118.cn

[U14] Py：分组收集到列表
来源：https://fl.zhonguo5118.cn

defaultdict(list)
来源：https://ct.zhonguo4118.cn

[U15] Py：高精度计时
来源：https://rn.zhonguo1118.cn

t = time.perf_counter()
来源：https://ky.zhonguo6118.cn

[U16] Py：命令行参数解析
来源：https://ak.zhonguo7118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://cu.zhonguo3118.cn

[U17] Py：初始化日志
来源：https://rh.zhonguo5118.cn

logging.basicConfig(level=logging.INFO)
来源：https://hj.zhonguo7118.cn

[U18] Py：预编译正则
来源：https://ck.zhonguo7118.cn

pat = re.compile(r"\d+")
来源：https://pa.zhonguo2118.cn

[U19] Py：正则替换带回调
来源：https://el.zhonguo5118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://zl.zhonguo1118.cn

[U20] Py：缓存函数结果
来源：https://yg.zhonguo6118.cn

@functools.lru_cache(maxsize=None)
来源：https://fv.zhonguo1118.cn

[U21] Py：自定义上下文管理器
来源：https://zb.zhonguo2118.cn

@contextlib.contextmanager
来源：https://kz.zhonguo1118.cn

[U22] Py：矩阵转置
来源：https://ez.zhonguo2118.cn

list(zip(*m))
来源：https://ca.zhonguo5118.cn

[U23] Py：分块读取大文件
来源：https://fg.zhonguo7118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://yt.zhonguo3118.cn

[U24] Py：路径操作
来源：https://xr.zhonguo3118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://nj.zhonguo5118.cn

[U25] Py：CSV 按字典读
来源：https://ss.zhonguo5118.cn

csv.DictReader(f)
来源：https://hu.zhonguo4118.cn

[U26] Py：并发下载
来源：https://qq.zhonguo8118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://pm.zhonguo6118.cn

[U27] Py：异步 HTTP
来源：https://wh.zhonguo3118.cn

aiohttp.ClientSession() 配合 async with
来源：https://sl.zhonguo1118.cn

[U28] Py：类型别名
来源：https://zu.zhonguo6118.cn

UserId = int
来源：https://su.zhonguo1118.cn

[U29] Py：属性校验
来源：https://mi.zhonguo4118.cn

@property 与 @x.setter 配合
来源：https://ag.zhonguo5118.cn

[U30] Py：数据类
来源：https://fh.zhonguo6118.cn

@dataclass(slots=True)
来源：https://ld.zhonguo7118.cn


<!-- 参考信息 -->