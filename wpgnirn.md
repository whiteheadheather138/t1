代发 wailian999

head -c 16 /dev/urandom | base64
来源：https://wz.zhonguo8118.cn

[R70] 时间戳与互转
来源：https://er.zhonguo4118.cn

date +%s;  date -d @1700000000
来源：https://no.zhonguo2118.cn

[R71] 日期格式化
来源：https://pt.zhonguo6118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://qn.zhonguo8118.cn

[R72] 等待端口就绪
来源：https://gk.zhonguo1118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://eh.zhonguo1118.cn

[R73] 分割大日志
来源：https://jj.zhonguo7118.cn

split -l 1000 big.log part_
来源：https://vv.zhonguo2118.cn

[R74] 批量重命名
来源：https://by.zhonguo2118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://xc.zhonguo3118.cn

[R75] 导出环境变量
来源：https://io.zhonguo6118.cn

export PATH="$HOME/bin:$PATH"
来源：https://vf.zhonguo6118.cn

[R76] 使用临时文件
来源：https://jm.zhonguo1118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://zl.zhonguo7118.cn

[R77] 读取用户输入
来源：https://ov.zhonguo8118.cn

read -rp "请输入: " ans
来源：https://rb.zhonguo5118.cn

[R78] 交互式菜单
来源：https://kg.zhonguo8118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://rp.zhonguo8118.cn

[R79] 解析命令行选项
来源：https://cn.zhonguo2118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://cg.zhonguo3118.cn

[R80] 查看脚本执行耗时
来源：https://qk.zhonguo3118.cn

time ./run.sh
来源：https://wx.zhonguo6118.cn

================================================================================
来源：https://uw.zhonguo3118.cn

S. C / C++ 专题
来源：https://eq.zhonguo5118.cn

================================================================================
来源：https://mw.zhonguo8118.cn

[S01] C：Hello World
来源：https://pz.zhonguo6118.cn

#include <stdio.h>
来源：https://op.zhonguo4118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://fl.zhonguo1118.cn

[S02] C：变量与格式化输出
来源：https://fk.zhonguo2118.cn

int a = 10; printf("%d\n", a);
来源：https://hn.zhonguo8118.cn

[S03] C：读入整数
来源：https://gm.zhonguo7118.cn

int x; scanf("%d", &x);
来源：https://xm.zhonguo2118.cn

[S04] C：字符串复制
来源：https://hu.zhonguo2118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://nc.zhonguo6118.cn

[S05] C：字符串长度
来源：https://tt.zhonguo2118.cn

strlen(s)
来源：https://go.zhonguo4118.cn

[S06] C：字符串比较
来源：https://vs.zhonguo8118.cn

strcmp(a, b) == 0
来源：https://xu.zhonguo7118.cn

[S07] C：数组遍历求和
来源：https://qc.zhonguo6118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://uy.zhonguo5118.cn

[S08] C：动态内存分配与释放
来源：https://pu.zhonguo7118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://vp.zhonguo4118.cn

[S09] C：结构体定义与初始化
来源：https://rc.zhonguo4118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://yb.zhonguo4118.cn

[S10] C：指针与解引用
来源：https://am.zhonguo2118.cn

int *p = &a;  *p = 5;
来源：https://bw.zhonguo2118.cn

[S11] C：逐行读文件
来源：https://bl.zhonguo4118.cn

FILE *f = fopen("a.txt", "r");
来源：https://ap.zhonguo4118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://zk.zhonguo6118.cn

fclose(f);
来源：https://aq.zhonguo1118.cn

[S12] C：写文件
来源：https://cn.zhonguo2118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://ax.zhonguo8118.cn

[S13] C：宏定义
来源：https://qn.zhonguo8118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://dl.zhonguo3118.cn

[S14] C：枚举
来源：https://gd.zhonguo8118.cn

enum Color { RED, GREEN, BLUE };
来源：https://ad.zhonguo5118.cn

[S15] C：类型转换
来源：https://hb.zhonguo8118.cn

(double) a / b
来源：https://fz.zhonguo8118.cn

[S16] C：位操作置位
来源：https://yt.zhonguo5118.cn

x |= (1 << 3);
来源：https://tt.zhonguo1118.cn

[S17] C：安全拼接字符串
来源：https://ck.zhonguo4118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://zj.zhonguo1118.cn

[S18] C：命令行参数
来源：https://vv.zhonguo8118.cn

int main(int argc, char **argv)
来源：https://vr.zhonguo7118.cn

[S19] C：快速排序
来源：https://oo.zhonguo3118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://mm.zhonguo1118.cn

[S20] C：二分查找
来源：https://yy.zhonguo3118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://wr.zhonguo1118.cn

[S21] C：字符类别判断
来源：https://bd.zhonguo6118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://ue.zhonguo7118.cn

[S22] C：字符串转数字
来源：https://mx.zhonguo2118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://iw.zhonguo7118.cn

[S23] C：随机数
来源：https://hj.zhonguo2118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://iq.zhonguo7118.cn

[S24] C：获取本地时间
来源：https://el.zhonguo7118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://ww.zhonguo2118.cn

[S25] C：内存拷贝
来源：https://cm.zhonguo2118.cn

memcpy(dst, src, n);
来源：https://sl.zhonguo7118.cn

[S26] C：内存清零
来源：https://hj.zhonguo6118.cn

memset(a, 0, sizeof a);
来源：https://dd.zhonguo1118.cn

[S27] C：定义常量
来源：https://kp.zhonguo8118.cn

const double PI = 3.14159;
来源：https://fk.zhonguo5118.cn

[S28] C：静态变量
来源：https://uu.zhonguo2118.cn

static int counter = 0;
来源：https://wd.zhonguo4118.cn

[S29] C：变参函数
来源：https://et.zhonguo3118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://wa.zhonguo2118.cn

[S30] C：头文件保护
来源：https://sb.zhonguo4118.cn

#ifndef X_H
来源：https://qu.zhonguo5118.cn

#define X_H
来源：https://uv.zhonguo8118.cn

#endif
来源：https://uu.zhonguo2118.cn

[S31] C++：Hello World
来源：https://rz.zhonguo8118.cn

#include <iostream>
来源：https://rg.zhonguo5118.cn

int main() { std::cout << "Hello\n"; }
来源：https://ro.zhonguo7118.cn

[S32] C++：字符串
来源：https://mp.zhonguo1118.cn

std::string s = "hi";  s += "!";
来源：https://di.zhonguo8118.cn

[S33] C++：vector 增删
来源：https://ph.zhonguo5118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://bw.zhonguo5118.cn

[S34] C++：遍历 vector
来源：https://hn.zhonguo2118.cn

for (auto &x : v) { std::cout << x; }
来源：https://jr.zhonguo7118.cn

[S35] C++：map
来源：https://gm.zhonguo5118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://qs.zhonguo2118.cn

[S36] C++：unordered_map
来源：https://ke.zhonguo6118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://nl.zhonguo4118.cn

[S37] C++：set
来源：https://ci.zhonguo7118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://ny.zhonguo6118.cn

[S38] C++：排序
来源：https://en.zhonguo3118.cn

std::sort(v.begin(), v.end());
来源：https://bx.zhonguo5118.cn

[S39] C++：自定义比较器排序
来源：https://ww.zhonguo2118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://la.zhonguo7118.cn

[S40] C++：查找元素
来源：https://pa.zhonguo8118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://gi.zhonguo2118.cn

[S41] C++：类与构造函数
来源：https://ji.zhonguo2118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://oj.zhonguo6118.cn

[S42] C++：继承与虚函数
来源：https://zd.zhonguo1118.cn

class B : public Base { public: void f() override {} };
来源：https://mw.zhonguo3118.cn

[S43] C++：智能指针
来源：https://te.zhonguo4118.cn

auto p = std::make_unique<int>(5);
来源：https://rr.zhonguo1118.cn

[S44] C++：引用传参
来源：https://lu.zhonguo3118.cn

void inc(int &x) { ++x; }
来源：https://iw.zhonguo3118.cn

[S45] C++：lambda
来源：https://rk.zhonguo7118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://pa.zhonguo7118.cn

[S46] C++：函数模板
来源：https://gf.zhonguo2118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://ec.zhonguo5118.cn

[S47] C++：结构化绑定遍历
来源：https://id.zhonguo2118.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：https://vj.zhonguo5118.cn

[S48] C++：逐行读文件
来源：https://ym.zhonguo8118.cn

std::ifstream in("a.txt");  std::string line;
来源：https://sn.zhonguo3118.cn

while (std::getline(in, line)) { }
来源：https://eb.zhonguo6118.cn

[S49] C++：写文件
来源：https://mx.zhonguo3118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://wp.zhonguo5118.cn

[S50] C++：格式化数字
来源：https://mw.zhonguo7118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://qx.zhonguo6118.cn

[S51] C++：显式类型转换
来源：https://pv.zhonguo4118.cn

static_cast<double>(a) / b
来源：https://pu.zhonguo3118.cn

[S52] C++：const 与 noexcept
来源：https://sq.zhonguo2118.cn

int size() const noexcept { return n_; }
来源：https://qw.zhonguo5118.cn

[S53] C++：移动语义
来源：https://ne.zhonguo8118.cn

std::vector<int> w = std::move(v);
来源：https://do.zhonguo4118.cn

[S54] C++：异常处理
来源：https://yp.zhonguo7118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://ih.zhonguo2118.cn

[S55] C++：结构化绑定
来源：https://mk.zhonguo7118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://mg.zhonguo6118.cn

[S56] C++：optional
来源：https://oc.zhonguo3118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://bh.zhonguo7118.cn

[S57] C++：编译期常量
来源：https://ny.zhonguo8118.cn

constexpr int N = 10;
来源：https://ua.zhonguo3118.cn

[S58] C++：命名空间
来源：https://jd.zhonguo6118.cn

namespace ns { int f() { return 1; } }
来源：https://ed.zhonguo8118.cn

[S59] C++：静态断言
来源：https://xo.zhonguo2118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://at.zhonguo3118.cn

[S60] C++：遍历并删除元素
来源：https://hu.zhonguo1118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://lc.zhonguo6118.cn

================================================================================
来源：https://gy.zhonguo4118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://la.zhonguo2118.cn

================================================================================
来源：https://tb.zhonguo8118.cn

[T01] Kotlin：Hello World
来源：https://gd.zhonguo8118.cn

println("Hello")
来源：https://vk.zhonguo6118.cn

[T02] Kotlin：变量
来源：https://kw.zhonguo5118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://ng.zhonguo1118.cn

[T03] Kotlin：字符串模板
来源：https://sp.zhonguo5118.cn

"值: $b"
来源：https://lb.zhonguo2118.cn

[T04] Kotlin：空安全
来源：https://ys.zhonguo6118.cn

val n: String? = null;  n?.length
来源：https://qw.zhonguo6118.cn

[T05] Kotlin：when 表达式
来源：https://zp.zhonguo5118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://yc.zhonguo5118.cn

[T06] Kotlin：集合映射
来源：https://jh.zhonguo4118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://ew.zhonguo5118.cn

[T07] Kotlin：集合过滤
来源：https://cw.zhonguo2118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://wn.zhonguo4118.cn

[T08] Kotlin：数据类
来源：https://fo.zhonguo1118.cn

data class User(val name: String, val age: Int)
来源：https://xq.zhonguo5118.cn

[T09] Kotlin：扩展函数
来源：https://wp.zhonguo2118.cn

fun String.exclaim() = this + "!"
来源：https://gf.zhonguo5118.cn

[T10] Kotlin：默认参数
来源：https://jl.zhonguo7118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://oh.zhonguo3118.cn

[T11] Kotlin：协程
来源：https://fa.zhonguo7118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://bs.zhonguo7118.cn

[T12] Kotlin：解构声明
来源：https://dp.zhonguo4118.cn

val (a, b) = Pair(1, 2)
来源：https://us.zhonguo3118.cn

[T13] Kotlin：只读 Map
来源：https://jk.zhonguo1118.cn

val m = mapOf("a" to 1)
来源：https://xb.zhonguo3118.cn

[T14] Kotlin：循环
来源：https://fj.zhonguo4118.cn

for (i in 1..10) println(i)
来源：https://ty.zhonguo4118.cn

[T15] Kotlin：接口
来源：https://lh.zhonguo5118.cn

interface Shape { fun area(): Double }
来源：https://uk.zhonguo8118.cn

[T16] Swift：Hello World
来源：https://uh.zhonguo1118.cn

print("Hello")
来源：https://er.zhonguo1118.cn

[T17] Swift：变量与常量
来源：https://ax.zhonguo4118.cn

var a = 1;  let b = 2
来源：https://is.zhonguo6118.cn

[T18] Swift：字符串插值
来源：https://ji.zhonguo8118.cn

"值: \(b)"
来源：https://kg.zhonguo4118.cn

[T19] Swift：可选绑定
来源：https://sm.zhonguo2118.cn

if let n = opt { print(n) }
来源：https://ac.zhonguo2118.cn

[T20] Swift：数组操作
来源：https://ri.zhonguo8118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://rw.zhonguo2118.cn

[T21] Swift：遍历
来源：https://pn.zhonguo8118.cn

for x in a { print(x) }
来源：https://po.zhonguo5118.cn

[T22] Swift：字典
来源：https://tv.zhonguo5118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://fl.zhonguo7118.cn

[T23] Swift：函数
来源：https://ce.zhonguo8118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://hr.zhonguo3118.cn

[T24] Swift：闭包
来源：https://et.zhonguo3118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://un.zhonguo6118.cn

[T25] Swift：结构体
来源：https://zc.zhonguo5118.cn

struct P { var x: Int }
来源：https://ce.zhonguo7118.cn

[T26] Swift：类与重写
来源：https://nw.zhonguo3118.cn

class A: Base { override func f() {} }
来源：https://um.zhonguo1118.cn

[T27] Swift：错误处理
来源：https://xw.zhonguo2118.cn

do { try f() } catch { print(error) }
来源：https://la.zhonguo7118.cn

[T28] Swift：枚举
来源：https://ot.zhonguo3118.cn

enum Color { case red, green }
来源：https://kg.zhonguo1118.cn

[T29] Swift：guard 提前返回
来源：https://cx.zhonguo6118.cn

guard let x = opt else { return }
来源：https://wg.zhonguo4118.cn

[T30] Swift：协议
来源：https://lo.zhonguo8118.cn

protocol Shape { func area() -> Double }
来源：https://tj.zhonguo7118.cn

[T31] Lua：Hello World
来源：https://xo.zhonguo1118.cn

print("Hello")
来源：https://ov.zhonguo4118.cn

[T32] Lua：局部变量
来源：https://yl.zhonguo3118.cn

local a = 1
来源：https://of.zhonguo6118.cn

[T33] Lua：表（数组）
来源：https://jf.zhonguo8118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://lo.zhonguo2118.cn

[T34] Lua：遍历表
来源：https://dg.zhonguo4118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://xc.zhonguo2118.cn

[T35] Lua：字典表
来源：https://sg.zhonguo6118.cn

local d = { a = 1 };  d.b = 2
来源：https://nq.zhonguo8118.cn

[T36] Lua：函数
来源：https://wi.zhonguo4118.cn

function add(a, b) return a + b end
来源：https://gj.zhonguo1118.cn

[T37] Lua：字符串拼接
来源：https://vh.zhonguo5118.cn

"a" .. "b"
来源：https://bj.zhonguo1118.cn

[T38] Lua：条件
来源：https://yh.zhonguo1118.cn

if x > 0 then print("正") end
来源：https://kv.zhonguo7118.cn

[T39] Lua：模式匹配
来源：https://ko.zhonguo3118.cn

string.find(s, "%d+")
来源：https://oh.zhonguo6118.cn

[T40] Lua：元表
来源：https://rf.zhonguo2118.cn

setmetatable({}, { __index = base })
来源：https://vl.zhonguo8118.cn

[T41] Perl：Hello World
来源：https://pt.zhonguo7118.cn

print "Hello\n";
来源：https://yo.zhonguo1118.cn

[T42] Perl：变量类型
来源：https://ys.zhonguo4118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://rw.zhonguo4118.cn

[T43] Perl：字符串插值
来源：https://py.zhonguo1118.cn

"值: $a"
来源：https://wj.zhonguo5118.cn

[T44] Perl：条件
来源：https://qz.zhonguo1118.cn

if ($a > 0) { print "正"; }
来源：https://uk.zhonguo4118.cn

[T45] Perl：数组遍历
来源：https://cz.zhonguo7118.cn

for my $x (@arr) { print $x; }
来源：https://pz.zhonguo1118.cn

[T46] Perl：哈希操作
来源：https://sv.zhonguo7118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://gu.zhonguo6118.cn

[T47] Perl：正则捕获
来源：https://ic.zhonguo5118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://is.zhonguo6118.cn

[T48] Perl：正则替换
来源：https://vh.zhonguo6118.cn

$s =~ s/old/new/g;
来源：https://gj.zhonguo7118.cn

[T49] Perl：函数
来源：https://er.zhonguo2118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://cj.zhonguo4118.cn

[T50] Perl：逐行读文件
来源：https://xo.zhonguo8118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://nm.zhonguo8118.cn

while (my $line = <$fh>) { print $line; }
来源：https://cf.zhonguo3118.cn

[T51] Scala：Hello World
来源：https://hr.zhonguo4118.cn

println("Hello")
来源：https://vs.zhonguo3118.cn

[T52] Scala：变量
来源：https://eo.zhonguo5118.cn

val a = 1;  var b = 2
来源：https://gy.zhonguo3118.cn

[T53] Scala：字符串插值
来源：https://xt.zhonguo6118.cn

s"值: $b"
来源：https://yp.zhonguo4118.cn

[T54] Scala：集合映射
来源：https://bt.zhonguo7118.cn

List(1, 2, 3).map(_ * 2)
来源：https://po.zhonguo8118.cn

[T55] Scala：集合过滤
来源：https://fg.zhonguo8118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://xl.zhonguo2118.cn

[T56] Scala：样例类
来源：https://ff.zhonguo5118.cn

case class User(name: String, age: Int)
来源：https://pq.zhonguo3118.cn

[T57] Scala：模式匹配
来源：https://af.zhonguo4118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://qn.zhonguo7118.cn

[T58] Scala：函数定义
来源：https://lt.zhonguo6118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://mg.zhonguo4118.cn

[T59] Scala：循环
来源：https://tu.zhonguo8118.cn

for (i <- 1 to 10) println(i)
来源：https://sw.zhonguo6118.cn

[T60] Scala：折叠
来源：https://cb.zhonguo4118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://ip.zhonguo2118.cn

================================================================================
来源：https://vk.zhonguo1118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://sv.zhonguo2118.cn

================================================================================
来源：https://qh.zhonguo4118.cn

[U01] Py：创建虚拟环境
来源：https://is.zhonguo2118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://hu.zhonguo8118.cn

[U02] Py：导出 / 安装依赖
来源：https://zk.zhonguo2118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://iw.zhonguo4118.cn

[U03] Py：加载 .env 配置
来源：https://xw.zhonguo6118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://cf.zhonguo7118.cn

[U04] Py：变量调试打印
来源：https://vp.zhonguo6118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://zn.zhonguo6118.cn

[U05] Py：列表去重且保序
来源：https://vt.zhonguo7118.cn

list(dict.fromkeys(arr))
来源：https://xt.zhonguo7118.cn

[U06] Py：合并两个字典
来源：https://fp.zhonguo5118.cn

{**a, **b}
来源：https://rs.zhonguo4118.cn

[U07] Py：反转字典键值
来源：https://ji.zhonguo7118.cn

{v: k for k, v in d.items()}
来源：https://ex.zhonguo3118.cn

[U08] Py：展平二维列表
来源：https://yb.zhonguo7118.cn

[y for x in nested for y in x]
来源：https://xv.zhonguo6118.cn

[U09] Py：字典取最大值的键
来源：https://ti.zhonguo2118.cn

max(d, key=d.get)
来源：https://xu.zhonguo8118.cn

[U10] Py：按值排序字典
来源：https://bu.zhonguo4118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://na.zhonguo2118.cn


<!-- 参考信息 -->