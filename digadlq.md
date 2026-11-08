代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：https://ul.zhonguo8118.cn

[S08] C：动态内存分配与释放
来源：https://uf.zhonguo7118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://mf.zhonguo1118.cn

[S09] C：结构体定义与初始化
来源：https://xu.zhonguo6118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://ee.zhonguo2118.cn

[S10] C：指针与解引用
来源：https://pu.zhonguo5118.cn

int *p = &a;  *p = 5;
来源：https://op.zhonguo6118.cn

[S11] C：逐行读文件
来源：https://xl.zhonguo4118.cn

FILE *f = fopen("a.txt", "r");
来源：https://ne.zhonguo6118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://wz.zhonguo2118.cn

fclose(f);
来源：https://nz.zhonguo2118.cn

[S12] C：写文件
来源：https://sr.zhonguo4118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://kc.zhonguo4118.cn

[S13] C：宏定义
来源：https://vz.zhonguo2118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://dz.zhonguo2118.cn

[S14] C：枚举
来源：https://yk.zhonguo5118.cn

enum Color { RED, GREEN, BLUE };
来源：https://fq.zhonguo1118.cn

[S15] C：类型转换
来源：https://bx.zhonguo6118.cn

(double) a / b
来源：https://zh.zhonguo2118.cn

[S16] C：位操作置位
来源：https://du.zhonguo2118.cn

x |= (1 << 3);
来源：https://rr.zhonguo6118.cn

[S17] C：安全拼接字符串
来源：https://kz.zhonguo8118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://ze.zhonguo5118.cn

[S18] C：命令行参数
来源：https://lg.zhonguo7118.cn

int main(int argc, char **argv)
来源：https://um.zhonguo4118.cn

[S19] C：快速排序
来源：https://mn.zhonguo3118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://xb.zhonguo1118.cn

[S20] C：二分查找
来源：https://dc.zhonguo2118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://dy.zhonguo4118.cn

[S21] C：字符类别判断
来源：https://au.zhonguo6118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://gt.zhonguo5118.cn

[S22] C：字符串转数字
来源：https://np.zhonguo1118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://qd.zhonguo7118.cn

[S23] C：随机数
来源：https://rw.zhonguo4118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://hw.zhonguo2118.cn

[S24] C：获取本地时间
来源：https://bi.zhonguo8118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://rq.zhonguo4118.cn

[S25] C：内存拷贝
来源：https://nk.zhonguo4118.cn

memcpy(dst, src, n);
来源：https://xu.zhonguo8118.cn

[S26] C：内存清零
来源：https://vl.zhonguo2118.cn

memset(a, 0, sizeof a);
来源：https://oi.zhonguo8118.cn

[S27] C：定义常量
来源：https://ld.zhonguo8118.cn

const double PI = 3.14159;
来源：https://rx.zhonguo4118.cn

[S28] C：静态变量
来源：https://ah.zhonguo2118.cn

static int counter = 0;
来源：https://uh.zhonguo2118.cn

[S29] C：变参函数
来源：https://he.zhonguo6118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://qh.zhonguo3118.cn

[S30] C：头文件保护
来源：https://km.zhonguo4118.cn

#ifndef X_H
来源：https://pr.zhonguo7118.cn

#define X_H
来源：https://ag.zhonguo2118.cn

#endif
来源：https://ox.zhonguo5118.cn

[S31] C++：Hello World
来源：https://sc.zhonguo8118.cn

#include <iostream>
来源：https://bi.zhonguo4118.cn

int main() { std::cout << "Hello\n"; }
来源：https://ru.zhonguo7118.cn

[S32] C++：字符串
来源：https://xm.zhonguo3118.cn

std::string s = "hi";  s += "!";
来源：https://ol.zhonguo4118.cn

[S33] C++：vector 增删
来源：https://zs.zhonguo2118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://ec.zhonguo6118.cn

[S34] C++：遍历 vector
来源：https://dy.zhonguo6118.cn

for (auto &x : v) { std::cout << x; }
来源：https://gd.zhonguo3118.cn

[S35] C++：map
来源：https://ru.zhonguo3118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://zi.zhonguo7118.cn

[S36] C++：unordered_map
来源：https://cm.zhonguo6118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://ik.zhonguo1118.cn

[S37] C++：set
来源：https://pr.zhonguo3118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://vx.zhonguo4118.cn

[S38] C++：排序
来源：https://hf.zhonguo7118.cn

std::sort(v.begin(), v.end());
来源：https://si.zhonguo7118.cn

[S39] C++：自定义比较器排序
来源：https://pn.zhonguo3118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://ly.zhonguo8118.cn

[S40] C++：查找元素
来源：https://yk.zhonguo6118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://mj.zhonguo4118.cn

[S41] C++：类与构造函数
来源：https://yy.zhonguo3118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://mq.zhonguo4118.cn

[S42] C++：继承与虚函数
来源：https://ka.zhonguo4118.cn

class B : public Base { public: void f() override {} };
来源：https://zr.zhonguo3118.cn

[S43] C++：智能指针
来源：https://fg.zhonguo5118.cn

auto p = std::make_unique<int>(5);
来源：https://ga.zhonguo2118.cn

[S44] C++：引用传参
来源：https://ac.zhonguo5118.cn

void inc(int &x) { ++x; }
来源：https://pt.zhonguo7118.cn

[S45] C++：lambda
来源：https://go.zhonguo4118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://wg.zhonguo3118.cn

[S46] C++：函数模板
来源：https://sv.zhonguo4118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://tf.zhonguo5118.cn

[S47] C++：结构化绑定遍历
来源：https://yv.zhonguo1118.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：https://hl.zhonguo6118.cn

[S48] C++：逐行读文件
来源：https://cl.zhonguo1118.cn

std::ifstream in("a.txt");  std::string line;
来源：https://pk.zhonguo8118.cn

while (std::getline(in, line)) { }
来源：https://yt.zhonguo1118.cn

[S49] C++：写文件
来源：https://br.zhonguo6118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://xj.zhonguo5118.cn

[S50] C++：格式化数字
来源：https://ym.zhonguo4118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://qz.zhonguo2118.cn

[S51] C++：显式类型转换
来源：https://yc.zhonguo1118.cn

static_cast<double>(a) / b
来源：https://dm.zhonguo2118.cn

[S52] C++：const 与 noexcept
来源：https://mb.zhonguo2118.cn

int size() const noexcept { return n_; }
来源：https://io.zhonguo4118.cn

[S53] C++：移动语义
来源：https://xy.zhonguo2118.cn

std::vector<int> w = std::move(v);
来源：https://dn.zhonguo3118.cn

[S54] C++：异常处理
来源：https://vi.zhonguo7118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://bv.zhonguo4118.cn

[S55] C++：结构化绑定
来源：https://kl.zhonguo7118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://cp.zhonguo6118.cn

[S56] C++：optional
来源：https://wy.zhonguo7118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://kk.zhonguo3118.cn

[S57] C++：编译期常量
来源：https://jn.zhonguo3118.cn

constexpr int N = 10;
来源：https://mv.zhonguo3118.cn

[S58] C++：命名空间
来源：https://sk.zhonguo3118.cn

namespace ns { int f() { return 1; } }
来源：https://wv.zhonguo7118.cn

[S59] C++：静态断言
来源：https://co.zhonguo5118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://pu.zhonguo2118.cn

[S60] C++：遍历并删除元素
来源：https://hr.zhonguo7118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://kb.zhonguo2118.cn

================================================================================
来源：https://fr.zhonguo2118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://bs.zhonguo3118.cn

================================================================================
来源：https://zj.zhonguo5118.cn

[T01] Kotlin：Hello World
来源：https://zs.zhonguo5118.cn

println("Hello")
来源：https://it.zhonguo7118.cn

[T02] Kotlin：变量
来源：https://yi.zhonguo3118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://vm.zhonguo6118.cn

[T03] Kotlin：字符串模板
来源：https://vu.zhonguo1118.cn

"值: $b"
来源：https://lx.zhonguo8118.cn

[T04] Kotlin：空安全
来源：https://ph.zhonguo7118.cn

val n: String? = null;  n?.length
来源：https://xd.zhonguo8118.cn

[T05] Kotlin：when 表达式
来源：https://iw.zhonguo3118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://qc.zhonguo7118.cn

[T06] Kotlin：集合映射
来源：https://nn.zhonguo2118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://kp.zhonguo2118.cn

[T07] Kotlin：集合过滤
来源：https://ss.zhonguo2118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://az.zhonguo1118.cn

[T08] Kotlin：数据类
来源：https://eo.zhonguo6118.cn

data class User(val name: String, val age: Int)
来源：https://dh.zhonguo2118.cn

[T09] Kotlin：扩展函数
来源：https://iy.zhonguo8118.cn

fun String.exclaim() = this + "!"
来源：https://hf.zhonguo3118.cn

[T10] Kotlin：默认参数
来源：https://no.zhonguo2118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://zo.zhonguo5118.cn

[T11] Kotlin：协程
来源：https://ds.zhonguo5118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://uv.zhonguo1118.cn

[T12] Kotlin：解构声明
来源：https://xp.zhonguo6118.cn

val (a, b) = Pair(1, 2)
来源：https://rh.zhonguo8118.cn

[T13] Kotlin：只读 Map
来源：https://pa.zhonguo3118.cn

val m = mapOf("a" to 1)
来源：https://po.zhonguo6118.cn

[T14] Kotlin：循环
来源：https://nu.zhonguo8118.cn

for (i in 1..10) println(i)
来源：https://tv.zhonguo8118.cn

[T15] Kotlin：接口
来源：https://fd.zhonguo4118.cn

interface Shape { fun area(): Double }
来源：https://xf.zhonguo3118.cn

[T16] Swift：Hello World
来源：https://zk.zhonguo8118.cn

print("Hello")
来源：https://im.zhonguo4118.cn

[T17] Swift：变量与常量
来源：https://xk.zhonguo2118.cn

var a = 1;  let b = 2
来源：https://kb.zhonguo6118.cn

[T18] Swift：字符串插值
来源：https://ph.zhonguo8118.cn

"值: \(b)"
来源：https://ey.zhonguo7118.cn

[T19] Swift：可选绑定
来源：https://me.zhonguo8118.cn

if let n = opt { print(n) }
来源：https://yc.zhonguo1118.cn

[T20] Swift：数组操作
来源：https://bh.zhonguo2118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://iv.zhonguo4118.cn

[T21] Swift：遍历
来源：https://jg.zhonguo2118.cn

for x in a { print(x) }
来源：https://kz.zhonguo4118.cn

[T22] Swift：字典
来源：https://cy.zhonguo7118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://dz.zhonguo4118.cn

[T23] Swift：函数
来源：https://ci.zhonguo2118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://is.zhonguo7118.cn

[T24] Swift：闭包
来源：https://if.zhonguo1118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://zo.zhonguo8118.cn

[T25] Swift：结构体
来源：https://td.zhonguo7118.cn

struct P { var x: Int }
来源：https://qf.zhonguo2118.cn

[T26] Swift：类与重写
来源：https://vn.zhonguo2118.cn

class A: Base { override func f() {} }
来源：https://co.zhonguo6118.cn

[T27] Swift：错误处理
来源：https://yn.zhonguo6118.cn

do { try f() } catch { print(error) }
来源：https://od.zhonguo4118.cn

[T28] Swift：枚举
来源：https://fu.zhonguo8118.cn

enum Color { case red, green }
来源：https://ge.zhonguo2118.cn

[T29] Swift：guard 提前返回
来源：https://ue.zhonguo7118.cn

guard let x = opt else { return }
来源：https://ot.zhonguo2118.cn

[T30] Swift：协议
来源：https://tv.zhonguo4118.cn

protocol Shape { func area() -> Double }
来源：https://vj.zhonguo3118.cn

[T31] Lua：Hello World
来源：https://ep.zhonguo8118.cn

print("Hello")
来源：https://mb.zhonguo1118.cn

[T32] Lua：局部变量
来源：https://hs.zhonguo2118.cn

local a = 1
来源：https://dr.zhonguo1118.cn

[T33] Lua：表（数组）
来源：https://uu.zhonguo5118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://rc.zhonguo7118.cn

[T34] Lua：遍历表
来源：https://io.zhonguo6118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://al.zhonguo5118.cn

[T35] Lua：字典表
来源：https://kj.zhonguo4118.cn

local d = { a = 1 };  d.b = 2
来源：https://ps.zhonguo6118.cn

[T36] Lua：函数
来源：https://dz.zhonguo1118.cn

function add(a, b) return a + b end
来源：https://tg.zhonguo6118.cn

[T37] Lua：字符串拼接
来源：https://df.zhonguo1118.cn

"a" .. "b"
来源：https://ne.zhonguo7118.cn

[T38] Lua：条件
来源：https://go.zhonguo2118.cn

if x > 0 then print("正") end
来源：https://jr.zhonguo3118.cn

[T39] Lua：模式匹配
来源：https://ir.zhonguo5118.cn

string.find(s, "%d+")
来源：https://ci.zhonguo4118.cn

[T40] Lua：元表
来源：https://qa.zhonguo6118.cn

setmetatable({}, { __index = base })
来源：https://ux.zhonguo4118.cn

[T41] Perl：Hello World
来源：https://de.zhonguo4118.cn

print "Hello\n";
来源：https://xk.zhonguo3118.cn

[T42] Perl：变量类型
来源：https://uh.zhonguo3118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://kt.zhonguo1118.cn

[T43] Perl：字符串插值
来源：https://ng.zhonguo3118.cn

"值: $a"
来源：https://pj.zhonguo4118.cn

[T44] Perl：条件
来源：https://ml.zhonguo4118.cn

if ($a > 0) { print "正"; }
来源：https://bw.zhonguo7118.cn

[T45] Perl：数组遍历
来源：https://ye.zhonguo5118.cn

for my $x (@arr) { print $x; }
来源：https://tb.zhonguo6118.cn

[T46] Perl：哈希操作
来源：https://pw.zhonguo4118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://bu.zhonguo3118.cn

[T47] Perl：正则捕获
来源：https://lh.zhonguo3118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://zn.zhonguo2118.cn

[T48] Perl：正则替换
来源：https://rq.zhonguo1118.cn

$s =~ s/old/new/g;
来源：https://cq.zhonguo5118.cn

[T49] Perl：函数
来源：https://mg.zhonguo1118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://du.zhonguo6118.cn

[T50] Perl：逐行读文件
来源：https://lg.zhonguo7118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://db.zhonguo5118.cn

while (my $line = <$fh>) { print $line; }
来源：https://dj.zhonguo3118.cn

[T51] Scala：Hello World
来源：https://gp.zhonguo1118.cn

println("Hello")
来源：https://bo.zhonguo1118.cn

[T52] Scala：变量
来源：https://pq.zhonguo5118.cn

val a = 1;  var b = 2
来源：https://vu.zhonguo5118.cn

[T53] Scala：字符串插值
来源：https://uj.zhonguo1118.cn

s"值: $b"
来源：https://wo.zhonguo8118.cn

[T54] Scala：集合映射
来源：https://lc.zhonguo1118.cn

List(1, 2, 3).map(_ * 2)
来源：https://si.zhonguo8118.cn

[T55] Scala：集合过滤
来源：https://gl.zhonguo6118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://km.zhonguo1118.cn

[T56] Scala：样例类
来源：https://th.zhonguo5118.cn

case class User(name: String, age: Int)
来源：https://zu.zhonguo2118.cn

[T57] Scala：模式匹配
来源：https://ej.zhonguo7118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://ha.zhonguo1118.cn

[T58] Scala：函数定义
来源：https://cn.zhonguo4118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://ks.zhonguo3118.cn

[T59] Scala：循环
来源：https://eb.zhonguo7118.cn

for (i <- 1 to 10) println(i)
来源：https://ci.zhonguo4118.cn

[T60] Scala：折叠
来源：https://xx.zhonguo6118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://bu.zhonguo2118.cn

================================================================================
来源：https://lc.zhonguo4118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://tr.zhonguo8118.cn

================================================================================
来源：https://uq.zhonguo2118.cn

[U01] Py：创建虚拟环境
来源：https://jr.zhonguo5118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://zl.zhonguo3118.cn

[U02] Py：导出 / 安装依赖
来源：https://fe.zhonguo7118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://oj.zhonguo2118.cn

[U03] Py：加载 .env 配置
来源：https://rt.zhonguo2118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://yv.zhonguo2118.cn

[U04] Py：变量调试打印
来源：https://ws.zhonguo6118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://zj.zhonguo6118.cn

[U05] Py：列表去重且保序
来源：https://vg.zhonguo8118.cn

list(dict.fromkeys(arr))
来源：https://lg.zhonguo3118.cn

[U06] Py：合并两个字典
来源：https://la.zhonguo2118.cn

{**a, **b}
来源：https://ro.zhonguo5118.cn

[U07] Py：反转字典键值
来源：https://qz.zhonguo2118.cn

{v: k for k, v in d.items()}
来源：https://ph.zhonguo1118.cn

[U08] Py：展平二维列表
来源：https://jc.zhonguo7118.cn

[y for x in nested for y in x]
来源：https://gq.zhonguo2118.cn

[U09] Py：字典取最大值的键
来源：https://eo.zhonguo5118.cn

max(d, key=d.get)
来源：https://me.zhonguo2118.cn

[U10] Py：按值排序字典
来源：https://rk.zhonguo2118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://vq.zhonguo8118.cn

[U11] Py：生成器表达式
来源：https://iv.zhonguo7118.cn

(x * 2 for x in arr)
来源：https://mx.zhonguo8118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://ge.zhonguo5118.cn

Counter(arr).most_common(3)
来源：https://tj.zhonguo8118.cn

[U13] Py：固定长度队列
来源：https://bk.zhonguo1118.cn

deque(maxlen=10)
来源：https://lv.zhonguo5118.cn

[U14] Py：分组收集到列表
来源：https://ry.zhonguo6118.cn

defaultdict(list)
来源：https://ax.zhonguo5118.cn

[U15] Py：高精度计时
来源：https://hf.zhonguo1118.cn

t = time.perf_counter()
来源：https://nw.zhonguo6118.cn

[U16] Py：命令行参数解析
来源：https://ce.zhonguo8118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://cu.zhonguo6118.cn

[U17] Py：初始化日志
来源：https://dj.zhonguo8118.cn

logging.basicConfig(level=logging.INFO)
来源：https://jk.zhonguo2118.cn

[U18] Py：预编译正则
来源：https://cq.zhonguo7118.cn

pat = re.compile(r"\d+")
来源：https://fk.zhonguo6118.cn

[U19] Py：正则替换带回调
来源：https://ro.zhonguo1118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://km.zhonguo8118.cn

[U20] Py：缓存函数结果
来源：https://bu.zhonguo3118.cn

@functools.lru_cache(maxsize=None)
来源：https://du.zhonguo6118.cn

[U21] Py：自定义上下文管理器
来源：https://up.zhonguo2118.cn

@contextlib.contextmanager
来源：https://kt.zhonguo5118.cn

[U22] Py：矩阵转置
来源：https://og.zhonguo3118.cn

list(zip(*m))
来源：https://pb.zhonguo3118.cn

[U23] Py：分块读取大文件
来源：https://em.zhonguo3118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://vn.zhonguo2118.cn

[U24] Py：路径操作
来源：https://jd.zhonguo7118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://sr.zhonguo5118.cn

[U25] Py：CSV 按字典读
来源：https://pi.zhonguo7118.cn

csv.DictReader(f)
来源：https://ed.zhonguo8118.cn

[U26] Py：并发下载
来源：https://bu.zhonguo1118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://fr.zhonguo5118.cn

[U27] Py：异步 HTTP
来源：https://qa.zhonguo1118.cn

aiohttp.ClientSession() 配合 async with
来源：https://to.zhonguo6118.cn

[U28] Py：类型别名
来源：https://ru.zhonguo5118.cn

UserId = int
来源：https://kl.zhonguo1118.cn

[U29] Py：属性校验
来源：https://ds.zhonguo1118.cn

@property 与 @x.setter 配合
来源：https://tx.zhonguo8118.cn

[U30] Py：数据类
来源：https://ra.zhonguo7118.cn

@dataclass(slots=True)
来源：https://ea.zhonguo6118.cn


<!-- 参考信息 -->