代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://ua.zhonguo7118.cn

[S25] C：内存拷贝
来源：https://rh.zhonguo8118.cn

memcpy(dst, src, n);
来源：https://mn.zhonguo1118.cn

[S26] C：内存清零
来源：https://hb.zhonguo7118.cn

memset(a, 0, sizeof a);
来源：https://it.zhonguo3118.cn

[S27] C：定义常量
来源：https://lg.zhonguo5118.cn

const double PI = 3.14159;
来源：https://lc.zhonguo7118.cn

[S28] C：静态变量
来源：https://hl.zhonguo3118.cn

static int counter = 0;
来源：https://rq.zhonguo7118.cn

[S29] C：变参函数
来源：https://wn.zhonguo1118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://vy.zhonguo3118.cn

[S30] C：头文件保护
来源：https://cv.zhonguo4118.cn

#ifndef X_H
来源：https://xg.zhonguo3118.cn

#define X_H
来源：https://va.zhonguo5118.cn

#endif
来源：https://ue.zhonguo5118.cn

[S31] C++：Hello World
来源：https://ys.zhonguo5118.cn

#include <iostream>
来源：https://kb.zhonguo1118.cn

int main() { std::cout << "Hello\n"; }
来源：https://az.zhonguo2118.cn

[S32] C++：字符串
来源：https://pg.zhonguo6118.cn

std::string s = "hi";  s += "!";
来源：https://ll.zhonguo5118.cn

[S33] C++：vector 增删
来源：https://sk.zhonguo2118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://sa.zhonguo7118.cn

[S34] C++：遍历 vector
来源：https://vk.zhonguo1118.cn

for (auto &x : v) { std::cout << x; }
来源：https://ql.zhonguo1118.cn

[S35] C++：map
来源：https://hd.zhonguo8118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://au.zhonguo4118.cn

[S36] C++：unordered_map
来源：https://ea.zhonguo7118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://ep.zhonguo1118.cn

[S37] C++：set
来源：https://vm.zhonguo7118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://ns.zhonguo3118.cn

[S38] C++：排序
来源：https://jw.zhonguo4118.cn

std::sort(v.begin(), v.end());
来源：https://yx.zhonguo8118.cn

[S39] C++：自定义比较器排序
来源：https://qm.zhonguo4118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://zs.zhonguo7118.cn

[S40] C++：查找元素
来源：https://xd.zhonguo4118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://dz.zhonguo5118.cn

[S41] C++：类与构造函数
来源：https://cd.zhonguo1118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://hi.zhonguo4118.cn

[S42] C++：继承与虚函数
来源：https://ue.zhonguo1118.cn

class B : public Base { public: void f() override {} };
来源：https://kc.zhonguo4118.cn

[S43] C++：智能指针
来源：https://qw.zhonguo1118.cn

auto p = std::make_unique<int>(5);
来源：https://av.zhonguo4118.cn

[S44] C++：引用传参
来源：https://ke.zhonguo1118.cn

void inc(int &x) { ++x; }
来源：https://il.zhonguo6118.cn

[S45] C++：lambda
来源：https://pz.zhonguo4118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://fw.zhonguo5118.cn

[S46] C++：函数模板
来源：https://lh.zhonguo6118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://ow.zhonguo7118.cn

[S47] C++：结构化绑定遍历
来源：https://nn.zhonguo2118.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：https://zb.zhonguo2118.cn

[S48] C++：逐行读文件
来源：https://qx.zhonguo8118.cn

std::ifstream in("a.txt");  std::string line;
来源：https://lj.zhonguo7118.cn

while (std::getline(in, line)) { }
来源：https://xz.zhonguo4118.cn

[S49] C++：写文件
来源：https://nm.zhonguo3118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://ug.zhonguo2118.cn

[S50] C++：格式化数字
来源：https://wg.zhonguo4118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://rc.zhonguo3118.cn

[S51] C++：显式类型转换
来源：https://yd.zhonguo5118.cn

static_cast<double>(a) / b
来源：https://on.zhonguo3118.cn

[S52] C++：const 与 noexcept
来源：https://mi.zhonguo1118.cn

int size() const noexcept { return n_; }
来源：https://me.zhonguo7118.cn

[S53] C++：移动语义
来源：https://gc.zhonguo4118.cn

std::vector<int> w = std::move(v);
来源：https://ii.zhonguo6118.cn

[S54] C++：异常处理
来源：https://mc.zhonguo3118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://kx.zhonguo2118.cn

[S55] C++：结构化绑定
来源：https://aj.zhonguo3118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://tf.zhonguo3118.cn

[S56] C++：optional
来源：https://em.zhonguo3118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://rh.zhonguo1118.cn

[S57] C++：编译期常量
来源：https://sy.zhonguo6118.cn

constexpr int N = 10;
来源：https://nm.zhonguo4118.cn

[S58] C++：命名空间
来源：https://bf.zhonguo6118.cn

namespace ns { int f() { return 1; } }
来源：https://xh.zhonguo1118.cn

[S59] C++：静态断言
来源：https://ki.zhonguo2118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://rd.zhonguo7118.cn

[S60] C++：遍历并删除元素
来源：https://wq.zhonguo8118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://vb.zhonguo5118.cn

================================================================================
来源：https://lq.zhonguo7118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://kl.zhonguo3118.cn

================================================================================
来源：https://dl.zhonguo7118.cn

[T01] Kotlin：Hello World
来源：https://jf.zhonguo1118.cn

println("Hello")
来源：https://et.zhonguo1118.cn

[T02] Kotlin：变量
来源：https://za.zhonguo7118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://bw.zhonguo5118.cn

[T03] Kotlin：字符串模板
来源：https://dr.zhonguo2118.cn

"值: $b"
来源：https://sn.zhonguo7118.cn

[T04] Kotlin：空安全
来源：https://jg.zhonguo8118.cn

val n: String? = null;  n?.length
来源：https://uj.zhonguo1118.cn

[T05] Kotlin：when 表达式
来源：https://rd.zhonguo2118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://en.zhonguo6118.cn

[T06] Kotlin：集合映射
来源：https://hh.zhonguo6118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://vf.zhonguo5118.cn

[T07] Kotlin：集合过滤
来源：https://mx.zhonguo4118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://oq.zhonguo8118.cn

[T08] Kotlin：数据类
来源：https://cl.zhonguo2118.cn

data class User(val name: String, val age: Int)
来源：https://yj.zhonguo6118.cn

[T09] Kotlin：扩展函数
来源：https://bc.zhonguo7118.cn

fun String.exclaim() = this + "!"
来源：https://vd.zhonguo4118.cn

[T10] Kotlin：默认参数
来源：https://fd.zhonguo8118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://wp.zhonguo3118.cn

[T11] Kotlin：协程
来源：https://uk.zhonguo8118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://ir.zhonguo5118.cn

[T12] Kotlin：解构声明
来源：https://rs.zhonguo4118.cn

val (a, b) = Pair(1, 2)
来源：https://tm.zhonguo4118.cn

[T13] Kotlin：只读 Map
来源：https://vy.zhonguo8118.cn

val m = mapOf("a" to 1)
来源：https://wv.zhonguo2118.cn

[T14] Kotlin：循环
来源：https://wx.zhonguo1118.cn

for (i in 1..10) println(i)
来源：https://rd.zhonguo3118.cn

[T15] Kotlin：接口
来源：https://il.zhonguo3118.cn

interface Shape { fun area(): Double }
来源：https://uh.zhonguo7118.cn

[T16] Swift：Hello World
来源：https://nq.zhonguo3118.cn

print("Hello")
来源：https://gl.zhonguo6118.cn

[T17] Swift：变量与常量
来源：https://fs.zhonguo6118.cn

var a = 1;  let b = 2
来源：https://be.zhonguo3118.cn

[T18] Swift：字符串插值
来源：https://sq.zhonguo4118.cn

"值: \(b)"
来源：https://db.zhonguo5118.cn

[T19] Swift：可选绑定
来源：https://ne.zhonguo6118.cn

if let n = opt { print(n) }
来源：https://pq.zhonguo3118.cn

[T20] Swift：数组操作
来源：https://en.zhonguo4118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://wr.zhonguo3118.cn

[T21] Swift：遍历
来源：https://ao.zhonguo6118.cn

for x in a { print(x) }
来源：https://qw.zhonguo8118.cn

[T22] Swift：字典
来源：https://xk.zhonguo1118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://ev.zhonguo6118.cn

[T23] Swift：函数
来源：https://go.zhonguo3118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://gq.zhonguo7118.cn

[T24] Swift：闭包
来源：https://ij.zhonguo8118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://ed.zhonguo3118.cn

[T25] Swift：结构体
来源：https://ix.zhonguo3118.cn

struct P { var x: Int }
来源：https://ej.zhonguo7118.cn

[T26] Swift：类与重写
来源：https://on.zhonguo6118.cn

class A: Base { override func f() {} }
来源：https://xv.zhonguo8118.cn

[T27] Swift：错误处理
来源：https://wd.zhonguo4118.cn

do { try f() } catch { print(error) }
来源：https://qr.zhonguo3118.cn

[T28] Swift：枚举
来源：https://qr.zhonguo6118.cn

enum Color { case red, green }
来源：https://bp.zhonguo7118.cn

[T29] Swift：guard 提前返回
来源：https://nw.zhonguo4118.cn

guard let x = opt else { return }
来源：https://ux.zhonguo1118.cn

[T30] Swift：协议
来源：https://jb.zhonguo4118.cn

protocol Shape { func area() -> Double }
来源：https://gd.zhonguo6118.cn

[T31] Lua：Hello World
来源：https://jo.zhonguo4118.cn

print("Hello")
来源：https://fr.zhonguo7118.cn

[T32] Lua：局部变量
来源：https://od.zhonguo1118.cn

local a = 1
来源：https://wr.zhonguo1118.cn

[T33] Lua：表（数组）
来源：https://ph.zhonguo2118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://xy.zhonguo1118.cn

[T34] Lua：遍历表
来源：https://fz.zhonguo3118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://tq.zhonguo5118.cn

[T35] Lua：字典表
来源：https://hh.zhonguo5118.cn

local d = { a = 1 };  d.b = 2
来源：https://im.zhonguo8118.cn

[T36] Lua：函数
来源：https://wr.zhonguo8118.cn

function add(a, b) return a + b end
来源：https://dn.zhonguo3118.cn

[T37] Lua：字符串拼接
来源：https://yl.zhonguo3118.cn

"a" .. "b"
来源：https://fv.zhonguo3118.cn

[T38] Lua：条件
来源：https://lv.zhonguo7118.cn

if x > 0 then print("正") end
来源：https://tx.zhonguo3118.cn

[T39] Lua：模式匹配
来源：https://ot.zhonguo8118.cn

string.find(s, "%d+")
来源：https://vb.zhonguo1118.cn

[T40] Lua：元表
来源：https://mh.zhonguo5118.cn

setmetatable({}, { __index = base })
来源：https://jq.zhonguo5118.cn

[T41] Perl：Hello World
来源：https://vs.zhonguo1118.cn

print "Hello\n";
来源：https://ss.zhonguo4118.cn

[T42] Perl：变量类型
来源：https://wv.zhonguo6118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://zk.zhonguo2118.cn

[T43] Perl：字符串插值
来源：https://yu.zhonguo4118.cn

"值: $a"
来源：https://ae.zhonguo4118.cn

[T44] Perl：条件
来源：https://dw.zhonguo3118.cn

if ($a > 0) { print "正"; }
来源：https://jl.zhonguo1118.cn

[T45] Perl：数组遍历
来源：https://lh.zhonguo7118.cn

for my $x (@arr) { print $x; }
来源：https://du.zhonguo2118.cn

[T46] Perl：哈希操作
来源：https://sq.zhonguo3118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://op.zhonguo2118.cn

[T47] Perl：正则捕获
来源：https://fo.zhonguo2118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://cm.zhonguo6118.cn

[T48] Perl：正则替换
来源：https://my.zhonguo2118.cn

$s =~ s/old/new/g;
来源：https://vs.zhonguo2118.cn

[T49] Perl：函数
来源：https://ed.zhonguo7118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://dy.zhonguo8118.cn

[T50] Perl：逐行读文件
来源：https://ci.zhonguo4118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://hx.zhonguo8118.cn

while (my $line = <$fh>) { print $line; }
来源：https://rb.zhonguo5118.cn

[T51] Scala：Hello World
来源：https://gc.zhonguo1118.cn

println("Hello")
来源：https://yl.zhonguo8118.cn

[T52] Scala：变量
来源：https://qg.zhonguo1118.cn

val a = 1;  var b = 2
来源：https://yi.zhonguo6118.cn

[T53] Scala：字符串插值
来源：https://ue.zhonguo1118.cn

s"值: $b"
来源：https://bg.zhonguo8118.cn

[T54] Scala：集合映射
来源：https://yw.zhonguo3118.cn

List(1, 2, 3).map(_ * 2)
来源：https://vn.zhonguo1118.cn

[T55] Scala：集合过滤
来源：https://us.zhonguo8118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://xh.zhonguo3118.cn

[T56] Scala：样例类
来源：https://ln.zhonguo6118.cn

case class User(name: String, age: Int)
来源：https://rq.zhonguo1118.cn

[T57] Scala：模式匹配
来源：https://om.zhonguo6118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://vl.zhonguo1118.cn

[T58] Scala：函数定义
来源：https://cm.zhonguo1118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://hq.zhonguo1118.cn

[T59] Scala：循环
来源：https://xa.zhonguo7118.cn

for (i <- 1 to 10) println(i)
来源：https://qf.zhonguo6118.cn

[T60] Scala：折叠
来源：https://rf.zhonguo1118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://nv.zhonguo8118.cn

================================================================================
来源：https://bi.zhonguo4118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://rk.zhonguo4118.cn

================================================================================
来源：https://su.zhonguo1118.cn

[U01] Py：创建虚拟环境
来源：https://bm.zhonguo4118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://vs.zhonguo5118.cn

[U02] Py：导出 / 安装依赖
来源：https://tc.zhonguo7118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://oy.zhonguo8118.cn

[U03] Py：加载 .env 配置
来源：https://ay.zhonguo8118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://zs.zhonguo7118.cn

[U04] Py：变量调试打印
来源：https://rd.zhonguo7118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://da.zhonguo4118.cn

[U05] Py：列表去重且保序
来源：https://uw.zhonguo6118.cn

list(dict.fromkeys(arr))
来源：https://sn.zhonguo2118.cn

[U06] Py：合并两个字典
来源：https://hk.zhonguo7118.cn

{**a, **b}
来源：https://xj.zhonguo3118.cn

[U07] Py：反转字典键值
来源：https://gr.zhonguo6118.cn

{v: k for k, v in d.items()}
来源：https://pc.zhonguo4118.cn

[U08] Py：展平二维列表
来源：https://vl.zhonguo7118.cn

[y for x in nested for y in x]
来源：https://zb.zhonguo1118.cn

[U09] Py：字典取最大值的键
来源：https://vp.zhonguo4118.cn

max(d, key=d.get)
来源：https://hh.zhonguo8118.cn

[U10] Py：按值排序字典
来源：https://ic.zhonguo4118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://cr.zhonguo7118.cn

[U11] Py：生成器表达式
来源：https://jm.zhonguo3118.cn

(x * 2 for x in arr)
来源：https://ps.zhonguo7118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://iy.zhonguo6118.cn

Counter(arr).most_common(3)
来源：https://ne.zhonguo3118.cn

[U13] Py：固定长度队列
来源：https://gl.zhonguo4118.cn

deque(maxlen=10)
来源：https://fw.zhonguo3118.cn

[U14] Py：分组收集到列表
来源：https://po.zhonguo7118.cn

defaultdict(list)
来源：https://ty.zhonguo5118.cn

[U15] Py：高精度计时
来源：https://mj.zhonguo6118.cn

t = time.perf_counter()
来源：https://pe.zhonguo8118.cn

[U16] Py：命令行参数解析
来源：https://vb.zhonguo4118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://tf.zhonguo2118.cn

[U17] Py：初始化日志
来源：https://ih.zhonguo3118.cn

logging.basicConfig(level=logging.INFO)
来源：https://io.zhonguo4118.cn

[U18] Py：预编译正则
来源：https://px.zhonguo7118.cn

pat = re.compile(r"\d+")
来源：https://mq.zhonguo8118.cn

[U19] Py：正则替换带回调
来源：https://di.zhonguo2118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://od.zhonguo6118.cn

[U20] Py：缓存函数结果
来源：https://jv.zhonguo4118.cn

@functools.lru_cache(maxsize=None)
来源：https://py.zhonguo6118.cn

[U21] Py：自定义上下文管理器
来源：https://qm.zhonguo4118.cn

@contextlib.contextmanager
来源：https://ws.zhonguo2118.cn

[U22] Py：矩阵转置
来源：https://dl.zhonguo2118.cn

list(zip(*m))
来源：https://sh.zhonguo5118.cn

[U23] Py：分块读取大文件
来源：https://xh.zhonguo2118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://rp.zhonguo1118.cn

[U24] Py：路径操作
来源：https://fb.zhonguo7118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://jz.zhonguo1118.cn

[U25] Py：CSV 按字典读
来源：https://qj.zhonguo8118.cn

csv.DictReader(f)
来源：https://km.zhonguo4118.cn

[U26] Py：并发下载
来源：https://ig.zhonguo8118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://gu.zhonguo1118.cn

[U27] Py：异步 HTTP
来源：https://ul.zhonguo7118.cn

aiohttp.ClientSession() 配合 async with
来源：https://kt.zhonguo8118.cn

[U28] Py：类型别名
来源：https://bo.zhonguo6118.cn

UserId = int
来源：https://mx.zhonguo6118.cn

[U29] Py：属性校验
来源：https://ef.zhonguo1118.cn

@property 与 @x.setter 配合
来源：https://dk.zhonguo4118.cn

[U30] Py：数据类
来源：https://ck.zhonguo1118.cn

@dataclass(slots=True)
来源：https://qj.zhonguo7118.cn

[U31] Py：单测
来源：https://ua.zhonguo4118.cn

python -m pytest -q
来源：https://bj.zhonguo6118.cn

[U32] Py：代码格式化
来源：https://zs.zhonguo7118.cn

ruff format . && ruff check --fix .
来源：https://rg.zhonguo3118.cn

[U33] Py：打包发布
来源：https://fh.zhonguo6118.cn

python -m build  （依赖 pyproject.toml）
来源：https://cl.zhonguo4118.cn

[U34] Py：判断编码
来源：https://kz.zhonguo2118.cn

chardet.detect(raw)
来源：https://sk.zhonguo5118.cn

[U35] Py：发送邮件
来源：https://pw.zhonguo6118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://ke.zhonguo2118.cn

[U36] Py：定时任务
来源：https://xc.zhonguo5118.cn

schedule.every(10).minutes.do(job)
来源：https://fm.zhonguo7118.cn

[U37] Py：读写 Excel
来源：https://rm.zhonguo2118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://xy.zhonguo2118.cn

[U38] Py：获取脚本所在目录
来源：https://ws.zhonguo5118.cn

Path(__file__).resolve().parent
来源：https://aw.zhonguo6118.cn

[U39] Py：判断是否在交互环境
来源：https://ag.zhonguo3118.cn

sys.stdout.isatty()
来源：https://vj.zhonguo5118.cn

[U40] Py：打印到标准错误
来源：https://ld.zhonguo2118.cn

print("err", file=sys.stderr)
来源：https://az.zhonguo1118.cn

[U41] PHP：初始化 Composer 项目
来源：https://ww.zhonguo4118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://at.zhonguo5118.cn

[U42] PHP：PSR-4 自动加载
来源：https://pv.zhonguo6118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://tm.zhonguo6118.cn

[U43] PHP：声明命名空间
来源：https://xa.zhonguo2118.cn

namespace App\Http;
来源：https://gy.zhonguo1118.cn

[U44] PHP：开启严格类型
来源：https://xn.zhonguo5118.cn

declare(strict_types=1);
来源：https://em.zhonguo7118.cn

[U45] PHP：类型声明与返回类型
来源：https://xj.zhonguo6118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://sl.zhonguo2118.cn

[U46] PHP：可空类型
来源：https://ye.zhonguo6118.cn

?string $name = null
来源：https://xa.zhonguo8118.cn

[U47] PHP：联合类型
来源：https://ug.zhonguo8118.cn

int|string $id
来源：https://tr.zhonguo4118.cn

[U48] PHP：纯枚举
来源：https://bi.zhonguo8118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://ew.zhonguo2118.cn


<!-- 参考信息 -->