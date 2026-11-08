代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：https://vv.zhonguo5118.cn

[S02] C：变量与格式化输出
来源：https://bf.zhonguo2118.cn

int a = 10; printf("%d\n", a);
来源：https://yt.zhonguo4118.cn

[S03] C：读入整数
来源：https://ao.zhonguo2118.cn

int x; scanf("%d", &x);
来源：https://rf.zhonguo3118.cn

[S04] C：字符串复制
来源：https://uh.zhonguo8118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://iz.zhonguo5118.cn

[S05] C：字符串长度
来源：https://xu.zhonguo6118.cn

strlen(s)
来源：https://wt.zhonguo5118.cn

[S06] C：字符串比较
来源：https://qh.zhonguo7118.cn

strcmp(a, b) == 0
来源：https://vg.zhonguo2118.cn

[S07] C：数组遍历求和
来源：https://db.zhonguo8118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://ij.zhonguo8118.cn

[S08] C：动态内存分配与释放
来源：https://pf.zhonguo6118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://rj.zhonguo6118.cn

[S09] C：结构体定义与初始化
来源：https://ds.zhonguo2118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://ec.zhonguo3118.cn

[S10] C：指针与解引用
来源：https://cl.zhonguo4118.cn

int *p = &a;  *p = 5;
来源：https://so.zhonguo7118.cn

[S11] C：逐行读文件
来源：https://ps.zhonguo4118.cn

FILE *f = fopen("a.txt", "r");
来源：https://qo.zhonguo7118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://lh.zhonguo6118.cn

fclose(f);
来源：https://bz.zhonguo7118.cn

[S12] C：写文件
来源：https://eb.zhonguo7118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://jw.zhonguo7118.cn

[S13] C：宏定义
来源：https://zw.zhonguo7118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://zm.zhonguo7118.cn

[S14] C：枚举
来源：https://ff.zhonguo2118.cn

enum Color { RED, GREEN, BLUE };
来源：https://kd.zhonguo1118.cn

[S15] C：类型转换
来源：https://ie.zhonguo2118.cn

(double) a / b
来源：https://ys.zhonguo7118.cn

[S16] C：位操作置位
来源：https://pb.zhonguo7118.cn

x |= (1 << 3);
来源：https://wr.zhonguo4118.cn

[S17] C：安全拼接字符串
来源：https://xr.zhonguo6118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://yz.zhonguo2118.cn

[S18] C：命令行参数
来源：https://td.zhonguo7118.cn

int main(int argc, char **argv)
来源：https://zg.zhonguo3118.cn

[S19] C：快速排序
来源：https://rp.zhonguo7118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://xz.zhonguo7118.cn

[S20] C：二分查找
来源：https://tw.zhonguo8118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://bx.zhonguo8118.cn

[S21] C：字符类别判断
来源：https://jc.zhonguo3118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://wp.zhonguo5118.cn

[S22] C：字符串转数字
来源：https://ib.zhonguo1118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://ll.zhonguo5118.cn

[S23] C：随机数
来源：https://or.zhonguo8118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://kf.zhonguo3118.cn

[S24] C：获取本地时间
来源：https://bw.zhonguo6118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://uw.zhonguo1118.cn

[S25] C：内存拷贝
来源：https://ou.zhonguo4118.cn

memcpy(dst, src, n);
来源：https://ei.zhonguo4118.cn

[S26] C：内存清零
来源：https://jv.zhonguo7118.cn

memset(a, 0, sizeof a);
来源：https://fp.zhonguo2118.cn

[S27] C：定义常量
来源：https://bh.zhonguo1118.cn

const double PI = 3.14159;
来源：https://hz.zhonguo6118.cn

[S28] C：静态变量
来源：https://qs.zhonguo1118.cn

static int counter = 0;
来源：https://fa.zhonguo1118.cn

[S29] C：变参函数
来源：https://ok.zhonguo7118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://vj.zhonguo6118.cn

[S30] C：头文件保护
来源：https://ng.zhonguo1118.cn

#ifndef X_H
来源：https://hb.zhonguo3118.cn

#define X_H
来源：https://fy.zhonguo5118.cn

#endif
来源：https://kd.zhonguo4118.cn

[S31] C++：Hello World
来源：https://zp.zhonguo3118.cn

#include <iostream>
来源：https://af.zhonguo6118.cn

int main() { std::cout << "Hello\n"; }
来源：https://sg.zhonguo4118.cn

[S32] C++：字符串
来源：https://ae.zhonguo1118.cn

std::string s = "hi";  s += "!";
来源：https://ov.zhonguo7118.cn

[S33] C++：vector 增删
来源：https://cu.zhonguo2118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://rj.zhonguo8118.cn

[S34] C++：遍历 vector
来源：https://uq.zhonguo7118.cn

for (auto &x : v) { std::cout << x; }
来源：https://zs.zhonguo3118.cn

[S35] C++：map
来源：https://qp.zhonguo1118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://lm.zhonguo3118.cn

[S36] C++：unordered_map
来源：https://uq.zhonguo1118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://hb.zhonguo3118.cn

[S37] C++：set
来源：https://lp.zhonguo8118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://xj.zhonguo4118.cn

[S38] C++：排序
来源：https://qn.zhonguo2118.cn

std::sort(v.begin(), v.end());
来源：https://ep.zhonguo8118.cn

[S39] C++：自定义比较器排序
来源：https://jt.zhonguo8118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://yc.zhonguo7118.cn

[S40] C++：查找元素
来源：https://fw.zhonguo6118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://th.zhonguo5118.cn

[S41] C++：类与构造函数
来源：https://xf.zhonguo6118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://th.zhonguo6118.cn

[S42] C++：继承与虚函数
来源：https://hg.zhonguo6118.cn

class B : public Base { public: void f() override {} };
来源：https://li.zhonguo2118.cn

[S43] C++：智能指针
来源：https://ad.zhonguo5118.cn

auto p = std::make_unique<int>(5);
来源：https://gl.zhonguo8118.cn

[S44] C++：引用传参
来源：https://xn.zhonguo7118.cn

void inc(int &x) { ++x; }
来源：https://mq.zhonguo8118.cn

[S45] C++：lambda
来源：https://lp.zhonguo7118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://wx.zhonguo7118.cn

[S46] C++：函数模板
来源：https://un.zhonguo1118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://wb.zhonguo3118.cn

[S47] C++：结构化绑定遍历
来源：https://kp.zhonguo5118.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：https://do.zhonguo3118.cn

[S48] C++：逐行读文件
来源：https://pe.zhonguo3118.cn

std::ifstream in("a.txt");  std::string line;
来源：https://bb.zhonguo4118.cn

while (std::getline(in, line)) { }
来源：https://bg.zhonguo2118.cn

[S49] C++：写文件
来源：https://iu.zhonguo1118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://ah.zhonguo3118.cn

[S50] C++：格式化数字
来源：https://ab.zhonguo7118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://ig.zhonguo4118.cn

[S51] C++：显式类型转换
来源：https://hy.zhonguo1118.cn

static_cast<double>(a) / b
来源：https://zx.zhonguo4118.cn

[S52] C++：const 与 noexcept
来源：https://fn.zhonguo3118.cn

int size() const noexcept { return n_; }
来源：https://ut.zhonguo1118.cn

[S53] C++：移动语义
来源：https://ic.zhonguo7118.cn

std::vector<int> w = std::move(v);
来源：https://uv.zhonguo4118.cn

[S54] C++：异常处理
来源：https://fu.zhonguo7118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://zr.zhonguo5118.cn

[S55] C++：结构化绑定
来源：https://sp.zhonguo1118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://qd.zhonguo2118.cn

[S56] C++：optional
来源：https://gm.zhonguo5118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://iq.zhonguo2118.cn

[S57] C++：编译期常量
来源：https://ew.zhonguo8118.cn

constexpr int N = 10;
来源：https://ys.zhonguo6118.cn

[S58] C++：命名空间
来源：https://ml.zhonguo7118.cn

namespace ns { int f() { return 1; } }
来源：https://sb.zhonguo6118.cn

[S59] C++：静态断言
来源：https://az.zhonguo5118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://db.zhonguo3118.cn

[S60] C++：遍历并删除元素
来源：https://yi.zhonguo1118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://dt.zhonguo3118.cn

================================================================================
来源：https://ug.zhonguo8118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://ap.zhonguo1118.cn

================================================================================
来源：https://kp.zhonguo7118.cn

[T01] Kotlin：Hello World
来源：https://kf.zhonguo6118.cn

println("Hello")
来源：https://nx.zhonguo8118.cn

[T02] Kotlin：变量
来源：https://gs.zhonguo3118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://se.zhonguo5118.cn

[T03] Kotlin：字符串模板
来源：https://ut.zhonguo7118.cn

"值: $b"
来源：https://tz.zhonguo2118.cn

[T04] Kotlin：空安全
来源：https://dj.zhonguo7118.cn

val n: String? = null;  n?.length
来源：https://ld.zhonguo3118.cn

[T05] Kotlin：when 表达式
来源：https://ek.zhonguo6118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://wg.zhonguo6118.cn

[T06] Kotlin：集合映射
来源：https://uy.zhonguo5118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://mt.zhonguo2118.cn

[T07] Kotlin：集合过滤
来源：https://uq.zhonguo4118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://sf.zhonguo5118.cn

[T08] Kotlin：数据类
来源：https://ev.zhonguo4118.cn

data class User(val name: String, val age: Int)
来源：https://nv.zhonguo7118.cn

[T09] Kotlin：扩展函数
来源：https://mo.zhonguo8118.cn

fun String.exclaim() = this + "!"
来源：https://oo.zhonguo2118.cn

[T10] Kotlin：默认参数
来源：https://qb.zhonguo5118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://fd.zhonguo3118.cn

[T11] Kotlin：协程
来源：https://pi.zhonguo7118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://zb.zhonguo2118.cn

[T12] Kotlin：解构声明
来源：https://hg.zhonguo6118.cn

val (a, b) = Pair(1, 2)
来源：https://ul.zhonguo5118.cn

[T13] Kotlin：只读 Map
来源：https://rz.zhonguo2118.cn

val m = mapOf("a" to 1)
来源：https://gn.zhonguo3118.cn

[T14] Kotlin：循环
来源：https://pp.zhonguo2118.cn

for (i in 1..10) println(i)
来源：https://mn.zhonguo6118.cn

[T15] Kotlin：接口
来源：https://uy.zhonguo7118.cn

interface Shape { fun area(): Double }
来源：https://vp.zhonguo1118.cn

[T16] Swift：Hello World
来源：https://iz.zhonguo4118.cn

print("Hello")
来源：https://ut.zhonguo8118.cn

[T17] Swift：变量与常量
来源：https://fu.zhonguo3118.cn

var a = 1;  let b = 2
来源：https://mp.zhonguo2118.cn

[T18] Swift：字符串插值
来源：https://ku.zhonguo3118.cn

"值: \(b)"
来源：https://ec.zhonguo7118.cn

[T19] Swift：可选绑定
来源：https://dy.zhonguo6118.cn

if let n = opt { print(n) }
来源：https://nm.zhonguo6118.cn

[T20] Swift：数组操作
来源：https://zt.zhonguo6118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://xy.zhonguo8118.cn

[T21] Swift：遍历
来源：https://we.zhonguo4118.cn

for x in a { print(x) }
来源：https://uy.zhonguo3118.cn

[T22] Swift：字典
来源：https://qv.zhonguo5118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://fg.zhonguo7118.cn

[T23] Swift：函数
来源：https://so.zhonguo5118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://xx.zhonguo7118.cn

[T24] Swift：闭包
来源：https://gh.zhonguo3118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://pd.zhonguo5118.cn

[T25] Swift：结构体
来源：https://dr.zhonguo5118.cn

struct P { var x: Int }
来源：https://dr.zhonguo3118.cn

[T26] Swift：类与重写
来源：https://er.zhonguo5118.cn

class A: Base { override func f() {} }
来源：https://wf.zhonguo4118.cn

[T27] Swift：错误处理
来源：https://po.zhonguo5118.cn

do { try f() } catch { print(error) }
来源：https://rx.zhonguo2118.cn

[T28] Swift：枚举
来源：https://ys.zhonguo6118.cn

enum Color { case red, green }
来源：https://ix.zhonguo4118.cn

[T29] Swift：guard 提前返回
来源：https://pg.zhonguo2118.cn

guard let x = opt else { return }
来源：https://sf.zhonguo4118.cn

[T30] Swift：协议
来源：https://us.zhonguo4118.cn

protocol Shape { func area() -> Double }
来源：https://rr.zhonguo1118.cn

[T31] Lua：Hello World
来源：https://ra.zhonguo4118.cn

print("Hello")
来源：https://ab.zhonguo3118.cn

[T32] Lua：局部变量
来源：https://sr.zhonguo8118.cn

local a = 1
来源：https://xo.zhonguo3118.cn

[T33] Lua：表（数组）
来源：https://ws.zhonguo4118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://cz.zhonguo1118.cn

[T34] Lua：遍历表
来源：https://cf.zhonguo5118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://py.zhonguo1118.cn

[T35] Lua：字典表
来源：https://lw.zhonguo5118.cn

local d = { a = 1 };  d.b = 2
来源：https://gz.zhonguo1118.cn

[T36] Lua：函数
来源：https://qo.zhonguo3118.cn

function add(a, b) return a + b end
来源：https://bh.zhonguo8118.cn

[T37] Lua：字符串拼接
来源：https://kd.zhonguo1118.cn

"a" .. "b"
来源：https://uv.zhonguo4118.cn

[T38] Lua：条件
来源：https://rx.zhonguo2118.cn

if x > 0 then print("正") end
来源：https://kn.zhonguo2118.cn

[T39] Lua：模式匹配
来源：https://nc.zhonguo2118.cn

string.find(s, "%d+")
来源：https://ew.zhonguo6118.cn

[T40] Lua：元表
来源：https://so.zhonguo4118.cn

setmetatable({}, { __index = base })
来源：https://ay.zhonguo8118.cn

[T41] Perl：Hello World
来源：https://wj.zhonguo7118.cn

print "Hello\n";
来源：https://mu.zhonguo8118.cn

[T42] Perl：变量类型
来源：https://am.zhonguo6118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://ti.zhonguo5118.cn

[T43] Perl：字符串插值
来源：https://vy.zhonguo1118.cn

"值: $a"
来源：https://mj.zhonguo8118.cn

[T44] Perl：条件
来源：https://xu.zhonguo5118.cn

if ($a > 0) { print "正"; }
来源：https://nz.zhonguo7118.cn

[T45] Perl：数组遍历
来源：https://qj.zhonguo1118.cn

for my $x (@arr) { print $x; }
来源：https://mk.zhonguo6118.cn

[T46] Perl：哈希操作
来源：https://lv.zhonguo1118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://se.zhonguo1118.cn

[T47] Perl：正则捕获
来源：https://gr.zhonguo2118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://bk.zhonguo1118.cn

[T48] Perl：正则替换
来源：https://eu.zhonguo5118.cn

$s =~ s/old/new/g;
来源：https://zm.zhonguo4118.cn

[T49] Perl：函数
来源：https://im.zhonguo1118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://nz.zhonguo2118.cn

[T50] Perl：逐行读文件
来源：https://zs.zhonguo6118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://rx.zhonguo2118.cn

while (my $line = <$fh>) { print $line; }
来源：https://bq.zhonguo4118.cn

[T51] Scala：Hello World
来源：https://qt.zhonguo1118.cn

println("Hello")
来源：https://et.zhonguo4118.cn

[T52] Scala：变量
来源：https://jp.zhonguo1118.cn

val a = 1;  var b = 2
来源：https://xe.zhonguo1118.cn

[T53] Scala：字符串插值
来源：https://ch.zhonguo5118.cn

s"值: $b"
来源：https://ly.zhonguo8118.cn

[T54] Scala：集合映射
来源：https://ga.zhonguo6118.cn

List(1, 2, 3).map(_ * 2)
来源：https://ms.zhonguo4118.cn

[T55] Scala：集合过滤
来源：https://ul.zhonguo6118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://ve.zhonguo4118.cn

[T56] Scala：样例类
来源：https://ds.zhonguo2118.cn

case class User(name: String, age: Int)
来源：https://uc.zhonguo2118.cn

[T57] Scala：模式匹配
来源：https://sm.zhonguo1118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://kf.zhonguo6118.cn

[T58] Scala：函数定义
来源：https://tq.zhonguo5118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://kc.zhonguo2118.cn

[T59] Scala：循环
来源：https://op.zhonguo5118.cn

for (i <- 1 to 10) println(i)
来源：https://dt.zhonguo8118.cn

[T60] Scala：折叠
来源：https://hj.zhonguo5118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://qp.zhonguo8118.cn

================================================================================
来源：https://ou.zhonguo8118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://if.zhonguo6118.cn

================================================================================
来源：https://us.zhonguo3118.cn

[U01] Py：创建虚拟环境
来源：https://oi.zhonguo8118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://zr.zhonguo7118.cn

[U02] Py：导出 / 安装依赖
来源：https://ms.zhonguo1118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://al.zhonguo8118.cn

[U03] Py：加载 .env 配置
来源：https://zx.zhonguo3118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://tt.zhonguo3118.cn

[U04] Py：变量调试打印
来源：https://ib.zhonguo7118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://cv.zhonguo8118.cn

[U05] Py：列表去重且保序
来源：https://ii.zhonguo5118.cn

list(dict.fromkeys(arr))
来源：https://tj.zhonguo2118.cn

[U06] Py：合并两个字典
来源：https://rj.zhonguo7118.cn

{**a, **b}
来源：https://uu.zhonguo1118.cn

[U07] Py：反转字典键值
来源：https://kw.zhonguo8118.cn

{v: k for k, v in d.items()}
来源：https://fi.zhonguo2118.cn

[U08] Py：展平二维列表
来源：https://am.zhonguo8118.cn

[y for x in nested for y in x]
来源：https://pf.zhonguo7118.cn

[U09] Py：字典取最大值的键
来源：https://re.zhonguo6118.cn

max(d, key=d.get)
来源：https://vg.zhonguo6118.cn

[U10] Py：按值排序字典
来源：https://ej.zhonguo8118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://ld.zhonguo8118.cn

[U11] Py：生成器表达式
来源：https://yx.zhonguo8118.cn

(x * 2 for x in arr)
来源：https://ps.zhonguo5118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://ir.zhonguo3118.cn

Counter(arr).most_common(3)
来源：https://da.zhonguo2118.cn

[U13] Py：固定长度队列
来源：https://aw.zhonguo4118.cn

deque(maxlen=10)
来源：https://fa.zhonguo8118.cn

[U14] Py：分组收集到列表
来源：https://la.zhonguo3118.cn

defaultdict(list)
来源：https://vd.zhonguo6118.cn

[U15] Py：高精度计时
来源：https://mn.zhonguo1118.cn

t = time.perf_counter()
来源：https://aw.zhonguo1118.cn

[U16] Py：命令行参数解析
来源：https://ze.zhonguo6118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://uo.zhonguo8118.cn

[U17] Py：初始化日志
来源：https://yl.zhonguo8118.cn

logging.basicConfig(level=logging.INFO)
来源：https://fv.zhonguo1118.cn

[U18] Py：预编译正则
来源：https://iq.zhonguo4118.cn

pat = re.compile(r"\d+")
来源：https://zm.zhonguo5118.cn

[U19] Py：正则替换带回调
来源：https://yz.zhonguo8118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://qo.zhonguo3118.cn

[U20] Py：缓存函数结果
来源：https://kj.zhonguo4118.cn

@functools.lru_cache(maxsize=None)
来源：https://qy.zhonguo1118.cn

[U21] Py：自定义上下文管理器
来源：https://ls.zhonguo3118.cn

@contextlib.contextmanager
来源：https://fr.zhonguo7118.cn

[U22] Py：矩阵转置
来源：https://yh.zhonguo7118.cn

list(zip(*m))
来源：https://yr.zhonguo8118.cn

[U23] Py：分块读取大文件
来源：https://ch.zhonguo8118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://rk.zhonguo1118.cn

[U24] Py：路径操作
来源：https://mo.zhonguo8118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://av.zhonguo2118.cn


<!-- 参考信息 -->