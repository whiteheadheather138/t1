代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：https://ok.zhonguo3118.cn

[S23] C：随机数
来源：https://zx.zhonguo6118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://la.zhonguo8118.cn

[S24] C：获取本地时间
来源：https://is.zhonguo5118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://ct.zhonguo7118.cn

[S25] C：内存拷贝
来源：https://mw.zhonguo5118.cn

memcpy(dst, src, n);
来源：https://ll.zhonguo6118.cn

[S26] C：内存清零
来源：https://bo.zhonguo6118.cn

memset(a, 0, sizeof a);
来源：https://sc.zhonguo3118.cn

[S27] C：定义常量
来源：https://cp.zhonguo7118.cn

const double PI = 3.14159;
来源：https://xq.zhonguo5118.cn

[S28] C：静态变量
来源：https://ru.zhonguo2118.cn

static int counter = 0;
来源：https://zc.zhonguo2118.cn

[S29] C：变参函数
来源：https://zq.zhonguo8118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://ur.zhonguo2118.cn

[S30] C：头文件保护
来源：https://tk.zhonguo2118.cn

#ifndef X_H
来源：https://nt.zhonguo8118.cn

#define X_H
来源：https://ds.zhonguo3118.cn

#endif
来源：https://sk.zhonguo6118.cn

[S31] C++：Hello World
来源：https://gf.zhonguo5118.cn

#include <iostream>
来源：https://mu.zhonguo7118.cn

int main() { std::cout << "Hello\n"; }
来源：https://yn.zhonguo5118.cn

[S32] C++：字符串
来源：https://iy.zhonguo8118.cn

std::string s = "hi";  s += "!";
来源：https://pj.zhonguo1118.cn

[S33] C++：vector 增删
来源：https://lc.zhonguo5118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://eg.zhonguo3118.cn

[S34] C++：遍历 vector
来源：https://rj.zhonguo5118.cn

for (auto &x : v) { std::cout << x; }
来源：https://tp.zhonguo3118.cn

[S35] C++：map
来源：https://fz.zhonguo6118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://wr.zhonguo7118.cn

[S36] C++：unordered_map
来源：https://an.zhonguo1118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://go.zhonguo3118.cn

[S37] C++：set
来源：https://oa.zhonguo6118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://ko.zhonguo7118.cn

[S38] C++：排序
来源：https://ym.zhonguo7118.cn

std::sort(v.begin(), v.end());
来源：https://tp.zhonguo6118.cn

[S39] C++：自定义比较器排序
来源：https://zt.zhonguo5118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://yc.zhonguo1118.cn

[S40] C++：查找元素
来源：https://ta.zhonguo8118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://ok.zhonguo1118.cn

[S41] C++：类与构造函数
来源：https://ki.zhonguo1118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://qz.zhonguo6118.cn

[S42] C++：继承与虚函数
来源：https://ux.zhonguo2118.cn

class B : public Base { public: void f() override {} };
来源：https://pv.zhonguo1118.cn

[S43] C++：智能指针
来源：https://iu.zhonguo3118.cn

auto p = std::make_unique<int>(5);
来源：https://mx.zhonguo6118.cn

[S44] C++：引用传参
来源：https://qh.zhonguo5118.cn

void inc(int &x) { ++x; }
来源：https://kt.zhonguo8118.cn

[S45] C++：lambda
来源：https://oj.zhonguo6118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://sw.zhonguo7118.cn

[S46] C++：函数模板
来源：https://bp.zhonguo5118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://py.zhonguo4118.cn

[S47] C++：结构化绑定遍历
来源：https://cs.zhonguo3118.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：https://iz.zhonguo7118.cn

[S48] C++：逐行读文件
来源：https://qc.zhonguo8118.cn

std::ifstream in("a.txt");  std::string line;
来源：https://qq.zhonguo5118.cn

while (std::getline(in, line)) { }
来源：https://ub.zhonguo7118.cn

[S49] C++：写文件
来源：https://py.zhonguo1118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://xq.zhonguo2118.cn

[S50] C++：格式化数字
来源：https://ji.zhonguo2118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://zt.zhonguo3118.cn

[S51] C++：显式类型转换
来源：https://cp.zhonguo3118.cn

static_cast<double>(a) / b
来源：https://to.zhonguo8118.cn

[S52] C++：const 与 noexcept
来源：https://gz.zhonguo5118.cn

int size() const noexcept { return n_; }
来源：https://ax.zhonguo7118.cn

[S53] C++：移动语义
来源：https://jh.zhonguo7118.cn

std::vector<int> w = std::move(v);
来源：https://km.zhonguo4118.cn

[S54] C++：异常处理
来源：https://as.zhonguo3118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://wj.zhonguo2118.cn

[S55] C++：结构化绑定
来源：https://lp.zhonguo4118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://ag.zhonguo2118.cn

[S56] C++：optional
来源：https://dr.zhonguo5118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://ne.zhonguo1118.cn

[S57] C++：编译期常量
来源：https://kw.zhonguo6118.cn

constexpr int N = 10;
来源：https://at.zhonguo5118.cn

[S58] C++：命名空间
来源：https://me.zhonguo4118.cn

namespace ns { int f() { return 1; } }
来源：https://ev.zhonguo2118.cn

[S59] C++：静态断言
来源：https://ny.zhonguo3118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://ud.zhonguo7118.cn

[S60] C++：遍历并删除元素
来源：https://ep.zhonguo6118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://yu.zhonguo1118.cn

================================================================================
来源：https://ho.zhonguo6118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://iq.zhonguo1118.cn

================================================================================
来源：https://iv.zhonguo4118.cn

[T01] Kotlin：Hello World
来源：https://tf.zhonguo4118.cn

println("Hello")
来源：https://rv.zhonguo6118.cn

[T02] Kotlin：变量
来源：https://er.zhonguo5118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://gn.zhonguo6118.cn

[T03] Kotlin：字符串模板
来源：https://nv.zhonguo6118.cn

"值: $b"
来源：https://lf.zhonguo2118.cn

[T04] Kotlin：空安全
来源：https://ba.zhonguo5118.cn

val n: String? = null;  n?.length
来源：https://oz.zhonguo3118.cn

[T05] Kotlin：when 表达式
来源：https://lc.zhonguo4118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://xg.zhonguo8118.cn

[T06] Kotlin：集合映射
来源：https://vj.zhonguo5118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://il.zhonguo2118.cn

[T07] Kotlin：集合过滤
来源：https://qf.zhonguo3118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://bn.zhonguo5118.cn

[T08] Kotlin：数据类
来源：https://py.zhonguo5118.cn

data class User(val name: String, val age: Int)
来源：https://yz.zhonguo8118.cn

[T09] Kotlin：扩展函数
来源：https://yo.zhonguo3118.cn

fun String.exclaim() = this + "!"
来源：https://ad.zhonguo8118.cn

[T10] Kotlin：默认参数
来源：https://ds.zhonguo6118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://do.zhonguo8118.cn

[T11] Kotlin：协程
来源：https://tz.zhonguo7118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://mt.zhonguo4118.cn

[T12] Kotlin：解构声明
来源：https://gh.zhonguo8118.cn

val (a, b) = Pair(1, 2)
来源：https://fz.zhonguo7118.cn

[T13] Kotlin：只读 Map
来源：https://oj.zhonguo6118.cn

val m = mapOf("a" to 1)
来源：https://ix.zhonguo8118.cn

[T14] Kotlin：循环
来源：https://yt.zhonguo5118.cn

for (i in 1..10) println(i)
来源：https://ni.zhonguo1118.cn

[T15] Kotlin：接口
来源：https://bq.zhonguo3118.cn

interface Shape { fun area(): Double }
来源：https://dl.zhonguo3118.cn

[T16] Swift：Hello World
来源：https://fn.zhonguo7118.cn

print("Hello")
来源：https://mv.zhonguo1118.cn

[T17] Swift：变量与常量
来源：https://ua.zhonguo1118.cn

var a = 1;  let b = 2
来源：https://df.zhonguo8118.cn

[T18] Swift：字符串插值
来源：https://gh.zhonguo1118.cn

"值: \(b)"
来源：https://ti.zhonguo4118.cn

[T19] Swift：可选绑定
来源：https://dm.zhonguo8118.cn

if let n = opt { print(n) }
来源：https://nj.zhonguo7118.cn

[T20] Swift：数组操作
来源：https://gw.zhonguo3118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://ux.zhonguo4118.cn

[T21] Swift：遍历
来源：https://kd.zhonguo4118.cn

for x in a { print(x) }
来源：https://vw.zhonguo2118.cn

[T22] Swift：字典
来源：https://je.zhonguo1118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://lu.zhonguo2118.cn

[T23] Swift：函数
来源：https://hv.zhonguo5118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://xw.zhonguo4118.cn

[T24] Swift：闭包
来源：https://dh.zhonguo7118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://qb.zhonguo8118.cn

[T25] Swift：结构体
来源：https://an.zhonguo7118.cn

struct P { var x: Int }
来源：https://dr.zhonguo2118.cn

[T26] Swift：类与重写
来源：https://kw.zhonguo3118.cn

class A: Base { override func f() {} }
来源：https://po.zhonguo6118.cn

[T27] Swift：错误处理
来源：https://pj.zhonguo4118.cn

do { try f() } catch { print(error) }
来源：https://pu.zhonguo5118.cn

[T28] Swift：枚举
来源：https://nx.zhonguo6118.cn

enum Color { case red, green }
来源：https://ml.zhonguo1118.cn

[T29] Swift：guard 提前返回
来源：https://ys.zhonguo5118.cn

guard let x = opt else { return }
来源：https://xn.zhonguo3118.cn

[T30] Swift：协议
来源：https://np.zhonguo7118.cn

protocol Shape { func area() -> Double }
来源：https://bk.zhonguo1118.cn

[T31] Lua：Hello World
来源：https://vj.zhonguo5118.cn

print("Hello")
来源：https://ih.zhonguo6118.cn

[T32] Lua：局部变量
来源：https://tr.zhonguo4118.cn

local a = 1
来源：https://vt.zhonguo2118.cn

[T33] Lua：表（数组）
来源：https://us.zhonguo1118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://al.zhonguo7118.cn

[T34] Lua：遍历表
来源：https://lw.zhonguo2118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://qh.zhonguo5118.cn

[T35] Lua：字典表
来源：https://jj.zhonguo1118.cn

local d = { a = 1 };  d.b = 2
来源：https://pk.zhonguo5118.cn

[T36] Lua：函数
来源：https://lv.zhonguo6118.cn

function add(a, b) return a + b end
来源：https://bh.zhonguo6118.cn

[T37] Lua：字符串拼接
来源：https://rk.zhonguo4118.cn

"a" .. "b"
来源：https://mx.zhonguo4118.cn

[T38] Lua：条件
来源：https://at.zhonguo2118.cn

if x > 0 then print("正") end
来源：https://tb.zhonguo3118.cn

[T39] Lua：模式匹配
来源：https://lh.zhonguo4118.cn

string.find(s, "%d+")
来源：https://ke.zhonguo3118.cn

[T40] Lua：元表
来源：https://gy.zhonguo6118.cn

setmetatable({}, { __index = base })
来源：https://gi.zhonguo3118.cn

[T41] Perl：Hello World
来源：https://qj.zhonguo8118.cn

print "Hello\n";
来源：https://mx.zhonguo6118.cn

[T42] Perl：变量类型
来源：https://ng.zhonguo2118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://pm.zhonguo1118.cn

[T43] Perl：字符串插值
来源：https://rd.zhonguo3118.cn

"值: $a"
来源：https://ie.zhonguo2118.cn

[T44] Perl：条件
来源：https://dy.zhonguo8118.cn

if ($a > 0) { print "正"; }
来源：https://hh.zhonguo6118.cn

[T45] Perl：数组遍历
来源：https://ue.zhonguo5118.cn

for my $x (@arr) { print $x; }
来源：https://sp.zhonguo4118.cn

[T46] Perl：哈希操作
来源：https://kd.zhonguo2118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://dq.zhonguo6118.cn

[T47] Perl：正则捕获
来源：https://ds.zhonguo8118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://tx.zhonguo3118.cn

[T48] Perl：正则替换
来源：https://gh.zhonguo6118.cn

$s =~ s/old/new/g;
来源：https://nv.zhonguo4118.cn

[T49] Perl：函数
来源：https://ez.zhonguo3118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://hu.zhonguo5118.cn

[T50] Perl：逐行读文件
来源：https://qc.zhonguo7118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://ct.zhonguo8118.cn

while (my $line = <$fh>) { print $line; }
来源：https://eq.zhonguo3118.cn

[T51] Scala：Hello World
来源：https://pl.zhonguo2118.cn

println("Hello")
来源：https://uy.zhonguo1118.cn

[T52] Scala：变量
来源：https://oi.zhonguo5118.cn

val a = 1;  var b = 2
来源：https://ju.zhonguo3118.cn

[T53] Scala：字符串插值
来源：https://xj.zhonguo4118.cn

s"值: $b"
来源：https://ep.zhonguo1118.cn

[T54] Scala：集合映射
来源：https://mi.zhonguo4118.cn

List(1, 2, 3).map(_ * 2)
来源：https://tn.zhonguo8118.cn

[T55] Scala：集合过滤
来源：https://an.zhonguo2118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://cj.zhonguo4118.cn

[T56] Scala：样例类
来源：https://jx.zhonguo1118.cn

case class User(name: String, age: Int)
来源：https://gs.zhonguo7118.cn

[T57] Scala：模式匹配
来源：https://cv.zhonguo4118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://dl.zhonguo4118.cn

[T58] Scala：函数定义
来源：https://yc.zhonguo5118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://be.zhonguo2118.cn

[T59] Scala：循环
来源：https://da.zhonguo6118.cn

for (i <- 1 to 10) println(i)
来源：https://lv.zhonguo2118.cn

[T60] Scala：折叠
来源：https://pb.zhonguo5118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://en.zhonguo4118.cn

================================================================================
来源：https://ws.zhonguo6118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://om.zhonguo8118.cn

================================================================================
来源：https://pn.zhonguo5118.cn

[U01] Py：创建虚拟环境
来源：https://tx.zhonguo1118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://ae.zhonguo2118.cn

[U02] Py：导出 / 安装依赖
来源：https://xj.zhonguo4118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://xn.zhonguo6118.cn

[U03] Py：加载 .env 配置
来源：https://zh.zhonguo7118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://qb.zhonguo1118.cn

[U04] Py：变量调试打印
来源：https://jz.zhonguo1118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://jz.zhonguo3118.cn

[U05] Py：列表去重且保序
来源：https://cw.zhonguo6118.cn

list(dict.fromkeys(arr))
来源：https://by.zhonguo8118.cn

[U06] Py：合并两个字典
来源：https://xv.zhonguo8118.cn

{**a, **b}
来源：https://ht.zhonguo8118.cn

[U07] Py：反转字典键值
来源：https://oq.zhonguo3118.cn

{v: k for k, v in d.items()}
来源：https://ih.zhonguo6118.cn

[U08] Py：展平二维列表
来源：https://nq.zhonguo4118.cn

[y for x in nested for y in x]
来源：https://pc.zhonguo5118.cn

[U09] Py：字典取最大值的键
来源：https://tg.zhonguo3118.cn

max(d, key=d.get)
来源：https://ng.zhonguo5118.cn

[U10] Py：按值排序字典
来源：https://ax.zhonguo1118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://zt.zhonguo3118.cn

[U11] Py：生成器表达式
来源：https://oz.zhonguo1118.cn

(x * 2 for x in arr)
来源：https://bd.zhonguo5118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://uw.zhonguo2118.cn

Counter(arr).most_common(3)
来源：https://vs.zhonguo6118.cn

[U13] Py：固定长度队列
来源：https://vk.zhonguo7118.cn

deque(maxlen=10)
来源：https://ug.zhonguo3118.cn

[U14] Py：分组收集到列表
来源：https://ga.zhonguo1118.cn

defaultdict(list)
来源：https://tk.zhonguo3118.cn

[U15] Py：高精度计时
来源：https://cx.zhonguo1118.cn

t = time.perf_counter()
来源：https://rk.zhonguo1118.cn

[U16] Py：命令行参数解析
来源：https://se.zhonguo3118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://vw.zhonguo3118.cn

[U17] Py：初始化日志
来源：https://de.zhonguo3118.cn

logging.basicConfig(level=logging.INFO)
来源：https://kj.zhonguo6118.cn

[U18] Py：预编译正则
来源：https://iv.zhonguo5118.cn

pat = re.compile(r"\d+")
来源：https://as.zhonguo2118.cn

[U19] Py：正则替换带回调
来源：https://oj.zhonguo8118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://sf.zhonguo7118.cn

[U20] Py：缓存函数结果
来源：https://ry.zhonguo5118.cn

@functools.lru_cache(maxsize=None)
来源：https://lt.zhonguo8118.cn

[U21] Py：自定义上下文管理器
来源：https://yz.zhonguo8118.cn

@contextlib.contextmanager
来源：https://ku.zhonguo8118.cn

[U22] Py：矩阵转置
来源：https://jb.zhonguo5118.cn

list(zip(*m))
来源：https://wx.zhonguo7118.cn

[U23] Py：分块读取大文件
来源：https://nt.zhonguo3118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://aj.zhonguo8118.cn

[U24] Py：路径操作
来源：https://dt.zhonguo1118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://tt.zhonguo6118.cn

[U25] Py：CSV 按字典读
来源：https://ya.zhonguo3118.cn

csv.DictReader(f)
来源：https://xr.zhonguo8118.cn

[U26] Py：并发下载
来源：https://zb.zhonguo8118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://ee.zhonguo6118.cn

[U27] Py：异步 HTTP
来源：https://vf.zhonguo2118.cn

aiohttp.ClientSession() 配合 async with
来源：https://qb.zhonguo5118.cn

[U28] Py：类型别名
来源：https://fx.zhonguo5118.cn

UserId = int
来源：https://na.zhonguo3118.cn

[U29] Py：属性校验
来源：https://uo.zhonguo1118.cn

@property 与 @x.setter 配合
来源：https://ix.zhonguo1118.cn

[U30] Py：数据类
来源：https://tk.zhonguo1118.cn

@dataclass(slots=True)
来源：https://za.zhonguo8118.cn

[U31] Py：单测
来源：https://qc.zhonguo2118.cn

python -m pytest -q
来源：https://fy.zhonguo5118.cn

[U32] Py：代码格式化
来源：https://zn.zhonguo2118.cn

ruff format . && ruff check --fix .
来源：https://fm.zhonguo2118.cn

[U33] Py：打包发布
来源：https://sv.zhonguo1118.cn

python -m build  （依赖 pyproject.toml）
来源：https://jr.zhonguo7118.cn

[U34] Py：判断编码
来源：https://rz.zhonguo4118.cn

chardet.detect(raw)
来源：https://zl.zhonguo6118.cn

[U35] Py：发送邮件
来源：https://te.zhonguo1118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://yc.zhonguo7118.cn

[U36] Py：定时任务
来源：https://yn.zhonguo1118.cn

schedule.every(10).minutes.do(job)
来源：https://ke.zhonguo4118.cn

[U37] Py：读写 Excel
来源：https://or.zhonguo8118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://pr.zhonguo7118.cn

[U38] Py：获取脚本所在目录
来源：https://af.zhonguo5118.cn

Path(__file__).resolve().parent
来源：https://ac.zhonguo5118.cn

[U39] Py：判断是否在交互环境
来源：https://wk.zhonguo6118.cn

sys.stdout.isatty()
来源：https://sz.zhonguo3118.cn

[U40] Py：打印到标准错误
来源：https://jx.zhonguo3118.cn

print("err", file=sys.stderr)
来源：https://gp.zhonguo6118.cn

[U41] PHP：初始化 Composer 项目
来源：https://sp.zhonguo2118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://hd.zhonguo7118.cn

[U42] PHP：PSR-4 自动加载
来源：https://gy.zhonguo4118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://kj.zhonguo3118.cn

[U43] PHP：声明命名空间
来源：https://gg.zhonguo7118.cn

namespace App\Http;
来源：https://ip.zhonguo6118.cn

[U44] PHP：开启严格类型
来源：https://bo.zhonguo7118.cn

declare(strict_types=1);
来源：https://ex.zhonguo3118.cn

[U45] PHP：类型声明与返回类型
来源：https://tf.zhonguo6118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://me.zhonguo5118.cn

[U46] PHP：可空类型
来源：https://bt.zhonguo5118.cn

?string $name = null
来源：https://lx.zhonguo8118.cn


<!-- 参考信息 -->