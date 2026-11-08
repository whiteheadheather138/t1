代发 wailian999

[S37] C++：set
来源：https://tz.zhonguo4118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://sg.zhonguo7118.cn

[S38] C++：排序
来源：https://iy.zhonguo6118.cn

std::sort(v.begin(), v.end());
来源：https://fy.zhonguo4118.cn

[S39] C++：自定义比较器排序
来源：https://yn.zhonguo5118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://zu.zhonguo6118.cn

[S40] C++：查找元素
来源：https://vp.zhonguo7118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://bb.zhonguo1118.cn

[S41] C++：类与构造函数
来源：https://wp.zhonguo8118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://ny.zhonguo4118.cn

[S42] C++：继承与虚函数
来源：https://ch.zhonguo6118.cn

class B : public Base { public: void f() override {} };
来源：https://wh.zhonguo2118.cn

[S43] C++：智能指针
来源：https://qf.zhonguo8118.cn

auto p = std::make_unique<int>(5);
来源：https://lq.zhonguo3118.cn

[S44] C++：引用传参
来源：https://uu.zhonguo2118.cn

void inc(int &x) { ++x; }
来源：https://yi.zhonguo2118.cn

[S45] C++：lambda
来源：https://ul.zhonguo3118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://au.zhonguo7118.cn

[S46] C++：函数模板
来源：https://ju.zhonguo2118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://so.zhonguo3118.cn

[S47] C++：结构化绑定遍历
来源：https://dm.zhonguo8118.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：https://kh.zhonguo7118.cn

[S48] C++：逐行读文件
来源：https://pe.zhonguo4118.cn

std::ifstream in("a.txt");  std::string line;
来源：https://sr.zhonguo3118.cn

while (std::getline(in, line)) { }
来源：https://lg.zhonguo2118.cn

[S49] C++：写文件
来源：https://wl.zhonguo5118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://vd.zhonguo8118.cn

[S50] C++：格式化数字
来源：https://vw.zhonguo2118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://uy.zhonguo5118.cn

[S51] C++：显式类型转换
来源：https://tp.zhonguo2118.cn

static_cast<double>(a) / b
来源：https://ib.zhonguo2118.cn

[S52] C++：const 与 noexcept
来源：https://lh.zhonguo4118.cn

int size() const noexcept { return n_; }
来源：https://an.zhonguo1118.cn

[S53] C++：移动语义
来源：https://na.zhonguo4118.cn

std::vector<int> w = std::move(v);
来源：https://hr.zhonguo8118.cn

[S54] C++：异常处理
来源：https://xd.zhonguo2118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://kl.zhonguo4118.cn

[S55] C++：结构化绑定
来源：https://id.zhonguo1118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://ng.zhonguo1118.cn

[S56] C++：optional
来源：https://ld.zhonguo1118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://ht.zhonguo6118.cn

[S57] C++：编译期常量
来源：https://co.zhonguo6118.cn

constexpr int N = 10;
来源：https://wq.zhonguo3118.cn

[S58] C++：命名空间
来源：https://ig.zhonguo1118.cn

namespace ns { int f() { return 1; } }
来源：https://jr.zhonguo4118.cn

[S59] C++：静态断言
来源：https://nh.zhonguo3118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://kb.zhonguo1118.cn

[S60] C++：遍历并删除元素
来源：https://mq.zhonguo1118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://yl.zhonguo8118.cn

================================================================================
来源：https://jf.zhonguo1118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://ts.zhonguo3118.cn

================================================================================
来源：https://ff.zhonguo8118.cn

[T01] Kotlin：Hello World
来源：https://ox.zhonguo1118.cn

println("Hello")
来源：https://do.zhonguo3118.cn

[T02] Kotlin：变量
来源：https://vp.zhonguo1118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://zr.zhonguo4118.cn

[T03] Kotlin：字符串模板
来源：https://ae.zhonguo1118.cn

"值: $b"
来源：https://bb.zhonguo2118.cn

[T04] Kotlin：空安全
来源：https://ee.zhonguo6118.cn

val n: String? = null;  n?.length
来源：https://ej.zhonguo4118.cn

[T05] Kotlin：when 表达式
来源：https://nl.zhonguo7118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://si.zhonguo3118.cn

[T06] Kotlin：集合映射
来源：https://eb.zhonguo5118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://bm.zhonguo1118.cn

[T07] Kotlin：集合过滤
来源：https://zn.zhonguo2118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://vl.zhonguo3118.cn

[T08] Kotlin：数据类
来源：https://pe.zhonguo5118.cn

data class User(val name: String, val age: Int)
来源：https://on.zhonguo8118.cn

[T09] Kotlin：扩展函数
来源：https://op.zhonguo8118.cn

fun String.exclaim() = this + "!"
来源：https://xs.zhonguo5118.cn

[T10] Kotlin：默认参数
来源：https://pi.zhonguo8118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://nj.zhonguo2118.cn

[T11] Kotlin：协程
来源：https://oe.zhonguo5118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://bk.zhonguo2118.cn

[T12] Kotlin：解构声明
来源：https://xz.zhonguo3118.cn

val (a, b) = Pair(1, 2)
来源：https://ja.zhonguo7118.cn

[T13] Kotlin：只读 Map
来源：https://tt.zhonguo2118.cn

val m = mapOf("a" to 1)
来源：https://hx.zhonguo8118.cn

[T14] Kotlin：循环
来源：https://sp.zhonguo5118.cn

for (i in 1..10) println(i)
来源：https://ab.zhonguo4118.cn

[T15] Kotlin：接口
来源：https://be.zhonguo6118.cn

interface Shape { fun area(): Double }
来源：https://ua.zhonguo7118.cn

[T16] Swift：Hello World
来源：https://ne.zhonguo1118.cn

print("Hello")
来源：https://pv.zhonguo3118.cn

[T17] Swift：变量与常量
来源：https://ko.zhonguo6118.cn

var a = 1;  let b = 2
来源：https://vf.zhonguo4118.cn

[T18] Swift：字符串插值
来源：https://ds.zhonguo3118.cn

"值: \(b)"
来源：https://pu.zhonguo2118.cn

[T19] Swift：可选绑定
来源：https://fd.zhonguo5118.cn

if let n = opt { print(n) }
来源：https://cf.zhonguo3118.cn

[T20] Swift：数组操作
来源：https://iz.zhonguo1118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://cs.zhonguo1118.cn

[T21] Swift：遍历
来源：https://np.zhonguo8118.cn

for x in a { print(x) }
来源：https://wt.zhonguo4118.cn

[T22] Swift：字典
来源：https://qv.zhonguo6118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://mx.zhonguo1118.cn

[T23] Swift：函数
来源：https://je.zhonguo6118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://rs.zhonguo7118.cn

[T24] Swift：闭包
来源：https://fy.zhonguo7118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://nj.zhonguo6118.cn

[T25] Swift：结构体
来源：https://nk.zhonguo2118.cn

struct P { var x: Int }
来源：https://ri.zhonguo8118.cn

[T26] Swift：类与重写
来源：https://iy.zhonguo7118.cn

class A: Base { override func f() {} }
来源：https://dl.zhonguo6118.cn

[T27] Swift：错误处理
来源：https://tu.zhonguo1118.cn

do { try f() } catch { print(error) }
来源：https://xn.zhonguo7118.cn

[T28] Swift：枚举
来源：https://ed.zhonguo3118.cn

enum Color { case red, green }
来源：https://px.zhonguo4118.cn

[T29] Swift：guard 提前返回
来源：https://eg.zhonguo1118.cn

guard let x = opt else { return }
来源：https://au.zhonguo3118.cn

[T30] Swift：协议
来源：https://io.zhonguo5118.cn

protocol Shape { func area() -> Double }
来源：https://dg.zhonguo8118.cn

[T31] Lua：Hello World
来源：https://mh.zhonguo7118.cn

print("Hello")
来源：https://nv.zhonguo8118.cn

[T32] Lua：局部变量
来源：https://ck.zhonguo5118.cn

local a = 1
来源：https://dd.zhonguo3118.cn

[T33] Lua：表（数组）
来源：https://es.zhonguo2118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://dm.zhonguo3118.cn

[T34] Lua：遍历表
来源：https://hl.zhonguo5118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://vi.zhonguo7118.cn

[T35] Lua：字典表
来源：https://jg.zhonguo6118.cn

local d = { a = 1 };  d.b = 2
来源：https://wg.zhonguo7118.cn

[T36] Lua：函数
来源：https://tx.zhonguo7118.cn

function add(a, b) return a + b end
来源：https://hl.zhonguo2118.cn

[T37] Lua：字符串拼接
来源：https://qt.zhonguo2118.cn

"a" .. "b"
来源：https://dv.zhonguo4118.cn

[T38] Lua：条件
来源：https://bk.zhonguo8118.cn

if x > 0 then print("正") end
来源：https://bj.zhonguo8118.cn

[T39] Lua：模式匹配
来源：https://iy.zhonguo6118.cn

string.find(s, "%d+")
来源：https://hb.zhonguo8118.cn

[T40] Lua：元表
来源：https://vk.zhonguo4118.cn

setmetatable({}, { __index = base })
来源：https://xa.zhonguo4118.cn

[T41] Perl：Hello World
来源：https://um.zhonguo3118.cn

print "Hello\n";
来源：https://eb.zhonguo2118.cn

[T42] Perl：变量类型
来源：https://dk.zhonguo3118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://xh.zhonguo2118.cn

[T43] Perl：字符串插值
来源：https://si.zhonguo7118.cn

"值: $a"
来源：https://cf.zhonguo4118.cn

[T44] Perl：条件
来源：https://kw.zhonguo3118.cn

if ($a > 0) { print "正"; }
来源：https://pa.zhonguo7118.cn

[T45] Perl：数组遍历
来源：https://ds.zhonguo4118.cn

for my $x (@arr) { print $x; }
来源：https://gx.zhonguo8118.cn

[T46] Perl：哈希操作
来源：https://ee.zhonguo6118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://ql.zhonguo1118.cn

[T47] Perl：正则捕获
来源：https://mr.zhonguo2118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://mf.zhonguo6118.cn

[T48] Perl：正则替换
来源：https://ds.zhonguo3118.cn

$s =~ s/old/new/g;
来源：https://wx.zhonguo8118.cn

[T49] Perl：函数
来源：https://qc.zhonguo3118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://ge.zhonguo7118.cn

[T50] Perl：逐行读文件
来源：https://ag.zhonguo1118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://qd.zhonguo6118.cn

while (my $line = <$fh>) { print $line; }
来源：https://ln.zhonguo4118.cn

[T51] Scala：Hello World
来源：https://cl.zhonguo6118.cn

println("Hello")
来源：https://nr.zhonguo8118.cn

[T52] Scala：变量
来源：https://ok.zhonguo1118.cn

val a = 1;  var b = 2
来源：https://aa.zhonguo7118.cn

[T53] Scala：字符串插值
来源：https://by.zhonguo7118.cn

s"值: $b"
来源：https://bk.zhonguo7118.cn

[T54] Scala：集合映射
来源：https://kx.zhonguo3118.cn

List(1, 2, 3).map(_ * 2)
来源：https://ms.zhonguo5118.cn

[T55] Scala：集合过滤
来源：https://ll.zhonguo4118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://yd.zhonguo7118.cn

[T56] Scala：样例类
来源：https://qa.zhonguo8118.cn

case class User(name: String, age: Int)
来源：https://aw.zhonguo5118.cn

[T57] Scala：模式匹配
来源：https://qg.zhonguo8118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://qt.zhonguo1118.cn

[T58] Scala：函数定义
来源：https://eg.zhonguo1118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://dt.zhonguo7118.cn

[T59] Scala：循环
来源：https://qk.zhonguo2118.cn

for (i <- 1 to 10) println(i)
来源：https://bf.zhonguo3118.cn

[T60] Scala：折叠
来源：https://sg.zhonguo8118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://tl.zhonguo7118.cn

================================================================================
来源：https://xp.zhonguo2118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://hz.zhonguo4118.cn

================================================================================
来源：https://rp.zhonguo2118.cn

[U01] Py：创建虚拟环境
来源：https://nn.zhonguo2118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://ul.zhonguo2118.cn

[U02] Py：导出 / 安装依赖
来源：https://kc.zhonguo8118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://fj.zhonguo8118.cn

[U03] Py：加载 .env 配置
来源：https://ja.zhonguo3118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://ea.zhonguo2118.cn

[U04] Py：变量调试打印
来源：https://lk.zhonguo4118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://bf.zhonguo4118.cn

[U05] Py：列表去重且保序
来源：https://lm.zhonguo4118.cn

list(dict.fromkeys(arr))
来源：https://av.zhonguo6118.cn

[U06] Py：合并两个字典
来源：https://qa.zhonguo8118.cn

{**a, **b}
来源：https://ye.zhonguo3118.cn

[U07] Py：反转字典键值
来源：https://ml.zhonguo8118.cn

{v: k for k, v in d.items()}
来源：https://kt.zhonguo7118.cn

[U08] Py：展平二维列表
来源：https://uj.zhonguo5118.cn

[y for x in nested for y in x]
来源：https://fo.zhonguo6118.cn

[U09] Py：字典取最大值的键
来源：https://de.zhonguo7118.cn

max(d, key=d.get)
来源：https://ea.zhonguo3118.cn

[U10] Py：按值排序字典
来源：https://om.zhonguo7118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://aw.zhonguo1118.cn

[U11] Py：生成器表达式
来源：https://he.zhonguo1118.cn

(x * 2 for x in arr)
来源：https://by.zhonguo3118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://wa.zhonguo8118.cn

Counter(arr).most_common(3)
来源：https://pt.zhonguo5118.cn

[U13] Py：固定长度队列
来源：https://su.zhonguo8118.cn

deque(maxlen=10)
来源：https://fg.zhonguo6118.cn

[U14] Py：分组收集到列表
来源：https://vr.zhonguo7118.cn

defaultdict(list)
来源：https://ra.zhonguo7118.cn

[U15] Py：高精度计时
来源：https://ug.zhonguo4118.cn

t = time.perf_counter()
来源：https://lu.zhonguo4118.cn

[U16] Py：命令行参数解析
来源：https://cu.zhonguo1118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://yf.zhonguo6118.cn

[U17] Py：初始化日志
来源：https://vn.zhonguo4118.cn

logging.basicConfig(level=logging.INFO)
来源：https://bp.zhonguo5118.cn

[U18] Py：预编译正则
来源：https://ua.zhonguo8118.cn

pat = re.compile(r"\d+")
来源：https://zn.zhonguo8118.cn

[U19] Py：正则替换带回调
来源：https://ql.zhonguo6118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://wg.zhonguo4118.cn

[U20] Py：缓存函数结果
来源：https://jz.zhonguo2118.cn

@functools.lru_cache(maxsize=None)
来源：https://qq.zhonguo8118.cn

[U21] Py：自定义上下文管理器
来源：https://oh.zhonguo1118.cn

@contextlib.contextmanager
来源：https://is.zhonguo1118.cn

[U22] Py：矩阵转置
来源：https://gl.zhonguo4118.cn

list(zip(*m))
来源：https://jq.zhonguo7118.cn

[U23] Py：分块读取大文件
来源：https://aq.zhonguo7118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://nd.zhonguo6118.cn

[U24] Py：路径操作
来源：https://am.zhonguo1118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://by.zhonguo2118.cn

[U25] Py：CSV 按字典读
来源：https://if.zhonguo6118.cn

csv.DictReader(f)
来源：https://qn.zhonguo8118.cn

[U26] Py：并发下载
来源：https://bg.zhonguo6118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://kr.zhonguo5118.cn

[U27] Py：异步 HTTP
来源：https://qe.zhonguo7118.cn

aiohttp.ClientSession() 配合 async with
来源：https://xl.zhonguo2118.cn

[U28] Py：类型别名
来源：https://gf.zhonguo5118.cn

UserId = int
来源：https://nk.zhonguo4118.cn

[U29] Py：属性校验
来源：https://zn.zhonguo3118.cn

@property 与 @x.setter 配合
来源：https://rj.zhonguo6118.cn

[U30] Py：数据类
来源：https://az.zhonguo4118.cn

@dataclass(slots=True)
来源：https://ch.zhonguo8118.cn

[U31] Py：单测
来源：https://xh.zhonguo3118.cn

python -m pytest -q
来源：https://hs.zhonguo1118.cn

[U32] Py：代码格式化
来源：https://ro.zhonguo1118.cn

ruff format . && ruff check --fix .
来源：https://nv.zhonguo5118.cn

[U33] Py：打包发布
来源：https://qg.zhonguo4118.cn

python -m build  （依赖 pyproject.toml）
来源：https://cl.zhonguo8118.cn

[U34] Py：判断编码
来源：https://fb.zhonguo4118.cn

chardet.detect(raw)
来源：https://nw.zhonguo2118.cn

[U35] Py：发送邮件
来源：https://ej.zhonguo6118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://km.zhonguo4118.cn

[U36] Py：定时任务
来源：https://aa.zhonguo1118.cn

schedule.every(10).minutes.do(job)
来源：https://xe.zhonguo7118.cn

[U37] Py：读写 Excel
来源：https://ai.zhonguo5118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://vz.zhonguo4118.cn

[U38] Py：获取脚本所在目录
来源：https://uc.zhonguo5118.cn

Path(__file__).resolve().parent
来源：https://ki.zhonguo5118.cn

[U39] Py：判断是否在交互环境
来源：https://be.zhonguo7118.cn

sys.stdout.isatty()
来源：https://zl.zhonguo3118.cn

[U40] Py：打印到标准错误
来源：https://jg.zhonguo4118.cn

print("err", file=sys.stderr)
来源：https://db.zhonguo5118.cn

[U41] PHP：初始化 Composer 项目
来源：https://jm.zhonguo5118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://gi.zhonguo6118.cn

[U42] PHP：PSR-4 自动加载
来源：https://sq.zhonguo5118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://qa.zhonguo6118.cn

[U43] PHP：声明命名空间
来源：https://ib.zhonguo6118.cn

namespace App\Http;
来源：https://ch.zhonguo3118.cn

[U44] PHP：开启严格类型
来源：https://kf.zhonguo6118.cn

declare(strict_types=1);
来源：https://ko.zhonguo2118.cn

[U45] PHP：类型声明与返回类型
来源：https://xd.zhonguo5118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://uu.zhonguo4118.cn

[U46] PHP：可空类型
来源：https://si.zhonguo2118.cn

?string $name = null
来源：https://ni.zhonguo2118.cn

[U47] PHP：联合类型
来源：https://ve.zhonguo7118.cn

int|string $id
来源：https://nq.zhonguo3118.cn

[U48] PHP：纯枚举
来源：https://eb.zhonguo3118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://yv.zhonguo1118.cn

[U49] PHP：只读属性
来源：https://ht.zhonguo8118.cn

public readonly string $name
来源：https://lo.zhonguo4118.cn

[U50] PHP：构造器属性提升
来源：https://wt.zhonguo2118.cn

public function __construct(private int $id) {}
来源：https://wu.zhonguo2118.cn

[U51] PHP：数组解构
来源：https://ta.zhonguo4118.cn

[$a, $b] = $arr;
来源：https://ll.zhonguo8118.cn

[U52] PHP：箭头函数
来源：https://fc.zhonguo8118.cn

$double = fn($x) => $x * 2;
来源：https://uo.zhonguo6118.cn

[U53] PHP：空合并运算符
来源：https://ih.zhonguo6118.cn

$v = $a ?? $b ?? "default";
来源：https://os.zhonguo5118.cn

[U54] PHP：空安全调用
来源：https://kf.zhonguo3118.cn

$obj?->method()
来源：https://gx.zhonguo1118.cn

[U55] PHP：match 表达式
来源：https://qs.zhonguo3118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://wf.zhonguo5118.cn

[U56] PHP：命名参数
来源：https://mc.zhonguo5118.cn

f(a: 1, b: 2)
来源：https://ud.zhonguo1118.cn

[U57] PHP：字符串插值
来源：https://tt.zhonguo4118.cn

"值: {$a}"
来源：https://wm.zhonguo4118.cn

[U58] PHP：数组三件套
来源：https://af.zhonguo6118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://bc.zhonguo6118.cn

[U59] PHP：自定义排序
来源：https://dt.zhonguo6118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://dk.zhonguo8118.cn

[U60] PHP：JSON 编解码
来源：https://zh.zhonguo8118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://ud.zhonguo1118.cn

[U61] PHP：正则
来源：https://di.zhonguo5118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://yi.zhonguo5118.cn

[U62] PHP：日期对象
来源：https://vy.zhonguo1118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://sr.zhonguo7118.cn


<!-- 参考信息 -->