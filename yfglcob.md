代发 wailian999

read -rp "请输入: " ans
来源：https://jo.zhonguo8118.cn

[R78] 交互式菜单
来源：https://ty.zhonguo5118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://er.zhonguo5118.cn

[R79] 解析命令行选项
来源：https://cy.zhonguo6118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://jn.zhonguo7118.cn

[R80] 查看脚本执行耗时
来源：https://ui.zhonguo6118.cn

time ./run.sh
来源：https://km.zhonguo7118.cn

================================================================================
来源：https://ff.zhonguo8118.cn

S. C / C++ 专题
来源：https://kd.zhonguo1118.cn

================================================================================
来源：https://ew.zhonguo3118.cn

[S01] C：Hello World
来源：https://fy.zhonguo7118.cn

#include <stdio.h>
来源：https://oy.zhonguo2118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://wa.zhonguo1118.cn

[S02] C：变量与格式化输出
来源：https://yv.zhonguo5118.cn

int a = 10; printf("%d\n", a);
来源：https://yv.zhonguo7118.cn

[S03] C：读入整数
来源：https://sm.zhonguo4118.cn

int x; scanf("%d", &x);
来源：https://ml.zhonguo6118.cn

[S04] C：字符串复制
来源：https://ww.zhonguo7118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://kk.zhonguo5118.cn

[S05] C：字符串长度
来源：https://mk.zhonguo1118.cn

strlen(s)
来源：https://wd.zhonguo3118.cn

[S06] C：字符串比较
来源：https://nt.zhonguo1118.cn

strcmp(a, b) == 0
来源：https://ah.zhonguo3118.cn

[S07] C：数组遍历求和
来源：https://fl.zhonguo2118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://xz.zhonguo1118.cn

[S08] C：动态内存分配与释放
来源：https://ge.zhonguo3118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://pn.zhonguo1118.cn

[S09] C：结构体定义与初始化
来源：https://bh.zhonguo5118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://hr.zhonguo6118.cn

[S10] C：指针与解引用
来源：https://pw.zhonguo6118.cn

int *p = &a;  *p = 5;
来源：https://ln.zhonguo4118.cn

[S11] C：逐行读文件
来源：https://rv.zhonguo3118.cn

FILE *f = fopen("a.txt", "r");
来源：https://yk.zhonguo8118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://rd.zhonguo7118.cn

fclose(f);
来源：https://yh.zhonguo7118.cn

[S12] C：写文件
来源：https://jc.zhonguo5118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://sf.zhonguo4118.cn

[S13] C：宏定义
来源：https://pr.zhonguo4118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://nx.zhonguo8118.cn

[S14] C：枚举
来源：https://sc.zhonguo1118.cn

enum Color { RED, GREEN, BLUE };
来源：https://ii.zhonguo7118.cn

[S15] C：类型转换
来源：https://qx.zhonguo5118.cn

(double) a / b
来源：https://hj.zhonguo8118.cn

[S16] C：位操作置位
来源：https://pi.zhonguo4118.cn

x |= (1 << 3);
来源：https://mq.zhonguo6118.cn

[S17] C：安全拼接字符串
来源：https://se.zhonguo3118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://qv.zhonguo7118.cn

[S18] C：命令行参数
来源：https://gk.zhonguo3118.cn

int main(int argc, char **argv)
来源：https://lj.zhonguo1118.cn

[S19] C：快速排序
来源：https://xt.zhonguo5118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://su.zhonguo3118.cn

[S20] C：二分查找
来源：https://eg.zhonguo4118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://sj.zhonguo1118.cn

[S21] C：字符类别判断
来源：https://bx.zhonguo7118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://kn.zhonguo1118.cn

[S22] C：字符串转数字
来源：https://lr.zhonguo1118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://gg.zhonguo5118.cn

[S23] C：随机数
来源：https://or.zhonguo1118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://cq.zhonguo2118.cn

[S24] C：获取本地时间
来源：https://eh.zhonguo6118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://ap.zhonguo6118.cn

[S25] C：内存拷贝
来源：https://rb.zhonguo3118.cn

memcpy(dst, src, n);
来源：https://zn.zhonguo3118.cn

[S26] C：内存清零
来源：https://kh.zhonguo3118.cn

memset(a, 0, sizeof a);
来源：https://ml.zhonguo1118.cn

[S27] C：定义常量
来源：https://rf.zhonguo8118.cn

const double PI = 3.14159;
来源：https://rw.zhonguo1118.cn

[S28] C：静态变量
来源：https://fj.zhonguo8118.cn

static int counter = 0;
来源：https://kf.zhonguo2118.cn

[S29] C：变参函数
来源：https://jk.zhonguo7118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://ca.zhonguo6118.cn

[S30] C：头文件保护
来源：https://xm.zhonguo4118.cn

#ifndef X_H
来源：https://dq.zhonguo6118.cn

#define X_H
来源：https://qi.zhonguo7118.cn

#endif
来源：https://dw.zhonguo6118.cn

[S31] C++：Hello World
来源：https://yc.zhonguo5118.cn

#include <iostream>
来源：https://sg.zhonguo6118.cn

int main() { std::cout << "Hello\n"; }
来源：https://ae.zhonguo8118.cn

[S32] C++：字符串
来源：https://nr.zhonguo3118.cn

std::string s = "hi";  s += "!";
来源：https://kk.zhonguo5118.cn

[S33] C++：vector 增删
来源：https://wi.zhonguo8118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://px.zhonguo4118.cn

[S34] C++：遍历 vector
来源：https://ba.zhonguo7118.cn

for (auto &x : v) { std::cout << x; }
来源：https://zn.zhonguo7118.cn

[S35] C++：map
来源：https://gw.zhonguo2118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://tb.zhonguo5118.cn

[S36] C++：unordered_map
来源：https://up.zhonguo2118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://ib.zhonguo7118.cn

[S37] C++：set
来源：https://gq.zhonguo6118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://ny.zhonguo1118.cn

[S38] C++：排序
来源：https://ro.zhonguo5118.cn

std::sort(v.begin(), v.end());
来源：https://gb.zhonguo6118.cn

[S39] C++：自定义比较器排序
来源：https://xb.zhonguo1118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://fe.zhonguo8118.cn

[S40] C++：查找元素
来源：https://qt.zhonguo2118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://ou.zhonguo3118.cn

[S41] C++：类与构造函数
来源：https://qz.zhonguo5118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://vu.zhonguo1118.cn

[S42] C++：继承与虚函数
来源：https://do.zhonguo2118.cn

class B : public Base { public: void f() override {} };
来源：https://qa.zhonguo1118.cn

[S43] C++：智能指针
来源：https://gk.zhonguo2118.cn

auto p = std::make_unique<int>(5);
来源：https://vf.zhonguo2118.cn

[S44] C++：引用传参
来源：https://pq.zhonguo8118.cn

void inc(int &x) { ++x; }
来源：https://xp.zhonguo5118.cn

[S45] C++：lambda
来源：https://ui.zhonguo8118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://vt.zhonguo6118.cn

[S46] C++：函数模板
来源：https://lj.zhonguo2118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://hj.zhonguo4118.cn

[S47] C++：结构化绑定遍历
来源：https://nt.zhonguo5118.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：https://jx.zhonguo7118.cn

[S48] C++：逐行读文件
来源：https://sn.zhonguo1118.cn

std::ifstream in("a.txt");  std::string line;
来源：https://sw.zhonguo3118.cn

while (std::getline(in, line)) { }
来源：https://zs.zhonguo1118.cn

[S49] C++：写文件
来源：https://wg.zhonguo2118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://au.zhonguo8118.cn

[S50] C++：格式化数字
来源：https://oz.zhonguo3118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://qs.zhonguo1118.cn

[S51] C++：显式类型转换
来源：https://mh.zhonguo2118.cn

static_cast<double>(a) / b
来源：https://al.zhonguo8118.cn

[S52] C++：const 与 noexcept
来源：https://zw.zhonguo3118.cn

int size() const noexcept { return n_; }
来源：https://hh.zhonguo8118.cn

[S53] C++：移动语义
来源：https://rn.zhonguo3118.cn

std::vector<int> w = std::move(v);
来源：https://ui.zhonguo5118.cn

[S54] C++：异常处理
来源：https://cy.zhonguo8118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://ta.zhonguo5118.cn

[S55] C++：结构化绑定
来源：https://ca.zhonguo5118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://fh.zhonguo8118.cn

[S56] C++：optional
来源：https://xc.zhonguo3118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://wu.zhonguo2118.cn

[S57] C++：编译期常量
来源：https://rb.zhonguo5118.cn

constexpr int N = 10;
来源：https://vv.zhonguo3118.cn

[S58] C++：命名空间
来源：https://mo.zhonguo5118.cn

namespace ns { int f() { return 1; } }
来源：https://pb.zhonguo6118.cn

[S59] C++：静态断言
来源：https://hb.zhonguo3118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://tx.zhonguo3118.cn

[S60] C++：遍历并删除元素
来源：https://bt.zhonguo3118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://ye.zhonguo6118.cn

================================================================================
来源：https://sd.zhonguo5118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://xv.zhonguo7118.cn

================================================================================
来源：https://cw.zhonguo3118.cn

[T01] Kotlin：Hello World
来源：https://nx.zhonguo6118.cn

println("Hello")
来源：https://lp.zhonguo1118.cn

[T02] Kotlin：变量
来源：https://tn.zhonguo3118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://xf.zhonguo5118.cn

[T03] Kotlin：字符串模板
来源：https://hw.zhonguo2118.cn

"值: $b"
来源：https://uk.zhonguo8118.cn

[T04] Kotlin：空安全
来源：https://br.zhonguo4118.cn

val n: String? = null;  n?.length
来源：https://mp.zhonguo8118.cn

[T05] Kotlin：when 表达式
来源：https://uy.zhonguo1118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://us.zhonguo4118.cn

[T06] Kotlin：集合映射
来源：https://cv.zhonguo7118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://gp.zhonguo1118.cn

[T07] Kotlin：集合过滤
来源：https://ej.zhonguo3118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://tk.zhonguo1118.cn

[T08] Kotlin：数据类
来源：https://ij.zhonguo1118.cn

data class User(val name: String, val age: Int)
来源：https://th.zhonguo4118.cn

[T09] Kotlin：扩展函数
来源：https://so.zhonguo6118.cn

fun String.exclaim() = this + "!"
来源：https://xg.zhonguo8118.cn

[T10] Kotlin：默认参数
来源：https://py.zhonguo6118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://no.zhonguo1118.cn

[T11] Kotlin：协程
来源：https://ok.zhonguo4118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://vx.zhonguo4118.cn

[T12] Kotlin：解构声明
来源：https://jh.zhonguo5118.cn

val (a, b) = Pair(1, 2)
来源：https://fo.zhonguo4118.cn

[T13] Kotlin：只读 Map
来源：https://kt.zhonguo5118.cn

val m = mapOf("a" to 1)
来源：https://km.zhonguo4118.cn

[T14] Kotlin：循环
来源：https://fp.zhonguo5118.cn

for (i in 1..10) println(i)
来源：https://kc.zhonguo3118.cn

[T15] Kotlin：接口
来源：https://cp.zhonguo1118.cn

interface Shape { fun area(): Double }
来源：https://de.zhonguo3118.cn

[T16] Swift：Hello World
来源：https://bm.zhonguo7118.cn

print("Hello")
来源：https://sw.zhonguo3118.cn

[T17] Swift：变量与常量
来源：https://un.zhonguo1118.cn

var a = 1;  let b = 2
来源：https://it.zhonguo8118.cn

[T18] Swift：字符串插值
来源：https://cu.zhonguo2118.cn

"值: \(b)"
来源：https://lc.zhonguo5118.cn

[T19] Swift：可选绑定
来源：https://zy.zhonguo2118.cn

if let n = opt { print(n) }
来源：https://sz.zhonguo5118.cn

[T20] Swift：数组操作
来源：https://ei.zhonguo4118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://fo.zhonguo8118.cn

[T21] Swift：遍历
来源：https://dc.zhonguo5118.cn

for x in a { print(x) }
来源：https://xb.zhonguo1118.cn

[T22] Swift：字典
来源：https://ai.zhonguo3118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://al.zhonguo3118.cn

[T23] Swift：函数
来源：https://ux.zhonguo7118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://vb.zhonguo2118.cn

[T24] Swift：闭包
来源：https://qe.zhonguo4118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://at.zhonguo1118.cn

[T25] Swift：结构体
来源：https://zv.zhonguo7118.cn

struct P { var x: Int }
来源：https://ng.zhonguo3118.cn

[T26] Swift：类与重写
来源：https://pv.zhonguo5118.cn

class A: Base { override func f() {} }
来源：https://ru.zhonguo1118.cn

[T27] Swift：错误处理
来源：https://zl.zhonguo1118.cn

do { try f() } catch { print(error) }
来源：https://cz.zhonguo4118.cn

[T28] Swift：枚举
来源：https://jn.zhonguo8118.cn

enum Color { case red, green }
来源：https://vj.zhonguo2118.cn

[T29] Swift：guard 提前返回
来源：https://zs.zhonguo2118.cn

guard let x = opt else { return }
来源：https://bz.zhonguo8118.cn

[T30] Swift：协议
来源：https://hg.zhonguo1118.cn

protocol Shape { func area() -> Double }
来源：https://ql.zhonguo2118.cn

[T31] Lua：Hello World
来源：https://vx.zhonguo7118.cn

print("Hello")
来源：https://yx.zhonguo6118.cn

[T32] Lua：局部变量
来源：https://sf.zhonguo6118.cn

local a = 1
来源：https://nx.zhonguo5118.cn

[T33] Lua：表（数组）
来源：https://iz.zhonguo8118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://ge.zhonguo6118.cn

[T34] Lua：遍历表
来源：https://ev.zhonguo6118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://ef.zhonguo2118.cn

[T35] Lua：字典表
来源：https://qt.zhonguo8118.cn

local d = { a = 1 };  d.b = 2
来源：https://sw.zhonguo6118.cn

[T36] Lua：函数
来源：https://bn.zhonguo5118.cn

function add(a, b) return a + b end
来源：https://yi.zhonguo3118.cn

[T37] Lua：字符串拼接
来源：https://ks.zhonguo3118.cn

"a" .. "b"
来源：https://cz.zhonguo3118.cn

[T38] Lua：条件
来源：https://gj.zhonguo8118.cn

if x > 0 then print("正") end
来源：https://oq.zhonguo7118.cn

[T39] Lua：模式匹配
来源：https://pv.zhonguo1118.cn

string.find(s, "%d+")
来源：https://ec.zhonguo3118.cn

[T40] Lua：元表
来源：https://ib.zhonguo1118.cn

setmetatable({}, { __index = base })
来源：https://hl.zhonguo3118.cn

[T41] Perl：Hello World
来源：https://en.zhonguo5118.cn

print "Hello\n";
来源：https://xt.zhonguo3118.cn

[T42] Perl：变量类型
来源：https://bt.zhonguo8118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://ju.zhonguo6118.cn

[T43] Perl：字符串插值
来源：https://yn.zhonguo2118.cn

"值: $a"
来源：https://ii.zhonguo6118.cn

[T44] Perl：条件
来源：https://ky.zhonguo6118.cn

if ($a > 0) { print "正"; }
来源：https://mp.zhonguo1118.cn

[T45] Perl：数组遍历
来源：https://vd.zhonguo8118.cn

for my $x (@arr) { print $x; }
来源：https://ig.zhonguo3118.cn

[T46] Perl：哈希操作
来源：https://og.zhonguo4118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://pv.zhonguo4118.cn

[T47] Perl：正则捕获
来源：https://vk.zhonguo8118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://bd.zhonguo1118.cn

[T48] Perl：正则替换
来源：https://iu.zhonguo8118.cn

$s =~ s/old/new/g;
来源：https://al.zhonguo1118.cn

[T49] Perl：函数
来源：https://ey.zhonguo2118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://la.zhonguo4118.cn

[T50] Perl：逐行读文件
来源：https://dm.zhonguo7118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://pw.zhonguo7118.cn

while (my $line = <$fh>) { print $line; }
来源：https://uu.zhonguo3118.cn

[T51] Scala：Hello World
来源：https://sh.zhonguo7118.cn

println("Hello")
来源：https://sp.zhonguo2118.cn

[T52] Scala：变量
来源：https://dx.zhonguo7118.cn

val a = 1;  var b = 2
来源：https://it.zhonguo4118.cn

[T53] Scala：字符串插值
来源：https://jj.zhonguo7118.cn

s"值: $b"
来源：https://wo.zhonguo5118.cn

[T54] Scala：集合映射
来源：https://jn.zhonguo6118.cn

List(1, 2, 3).map(_ * 2)
来源：https://ou.zhonguo1118.cn

[T55] Scala：集合过滤
来源：https://sn.zhonguo1118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://va.zhonguo4118.cn

[T56] Scala：样例类
来源：https://xt.zhonguo6118.cn

case class User(name: String, age: Int)
来源：https://jc.zhonguo5118.cn

[T57] Scala：模式匹配
来源：https://gr.zhonguo7118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://lq.zhonguo6118.cn

[T58] Scala：函数定义
来源：https://xg.zhonguo8118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://zv.zhonguo1118.cn

[T59] Scala：循环
来源：https://do.zhonguo2118.cn

for (i <- 1 to 10) println(i)
来源：https://rj.zhonguo6118.cn

[T60] Scala：折叠
来源：https://fc.zhonguo8118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://pm.zhonguo4118.cn

================================================================================
来源：https://ju.zhonguo6118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://ji.zhonguo8118.cn

================================================================================
来源：https://ol.zhonguo4118.cn

[U01] Py：创建虚拟环境
来源：https://ci.zhonguo3118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://pz.zhonguo6118.cn

[U02] Py：导出 / 安装依赖
来源：https://gf.zhonguo5118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://qx.zhonguo8118.cn

[U03] Py：加载 .env 配置
来源：https://oc.zhonguo8118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://qf.zhonguo8118.cn

[U04] Py：变量调试打印
来源：https://xi.zhonguo1118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://ht.zhonguo7118.cn

[U05] Py：列表去重且保序
来源：https://vz.zhonguo5118.cn

list(dict.fromkeys(arr))
来源：https://um.zhonguo8118.cn

[U06] Py：合并两个字典
来源：https://jh.zhonguo3118.cn

{**a, **b}
来源：https://qq.zhonguo5118.cn

[U07] Py：反转字典键值
来源：https://xo.zhonguo5118.cn

{v: k for k, v in d.items()}
来源：https://gx.zhonguo6118.cn

[U08] Py：展平二维列表
来源：https://wu.zhonguo6118.cn

[y for x in nested for y in x]
来源：https://dk.zhonguo7118.cn

[U09] Py：字典取最大值的键
来源：https://ow.zhonguo7118.cn

max(d, key=d.get)
来源：https://wc.zhonguo3118.cn

[U10] Py：按值排序字典
来源：https://pg.zhonguo6118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://ia.zhonguo5118.cn

[U11] Py：生成器表达式
来源：https://gm.zhonguo4118.cn

(x * 2 for x in arr)
来源：https://hh.zhonguo4118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://jj.zhonguo3118.cn

Counter(arr).most_common(3)
来源：https://yv.zhonguo2118.cn

[U13] Py：固定长度队列
来源：https://yf.zhonguo5118.cn

deque(maxlen=10)
来源：https://te.zhonguo6118.cn

[U14] Py：分组收集到列表
来源：https://mf.zhonguo6118.cn

defaultdict(list)
来源：https://cv.zhonguo1118.cn

[U15] Py：高精度计时
来源：https://bx.zhonguo4118.cn

t = time.perf_counter()
来源：https://tg.zhonguo6118.cn

[U16] Py：命令行参数解析
来源：https://py.zhonguo1118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://uk.zhonguo5118.cn

[U17] Py：初始化日志
来源：https://mm.zhonguo4118.cn

logging.basicConfig(level=logging.INFO)
来源：https://cd.zhonguo3118.cn

[U18] Py：预编译正则
来源：https://cu.zhonguo6118.cn

pat = re.compile(r"\d+")
来源：https://ui.zhonguo2118.cn


<!-- 参考信息 -->