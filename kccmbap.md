代发 wailian999

while (std::getline(in, line)) { }
来源：https://ro.zhonguo3118.cn

[S49] C++：写文件
来源：https://cf.zhonguo2118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://yo.zhonguo6118.cn

[S50] C++：格式化数字
来源：https://uv.zhonguo5118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://sx.zhonguo5118.cn

[S51] C++：显式类型转换
来源：https://pi.zhonguo2118.cn

static_cast<double>(a) / b
来源：https://cd.zhonguo6118.cn

[S52] C++：const 与 noexcept
来源：https://qs.zhonguo5118.cn

int size() const noexcept { return n_; }
来源：https://zu.zhonguo3118.cn

[S53] C++：移动语义
来源：https://kb.zhonguo1118.cn

std::vector<int> w = std::move(v);
来源：https://rg.zhonguo8118.cn

[S54] C++：异常处理
来源：https://dd.zhonguo7118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://xj.zhonguo4118.cn

[S55] C++：结构化绑定
来源：https://ft.zhonguo6118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://ty.zhonguo3118.cn

[S56] C++：optional
来源：https://me.zhonguo2118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://ww.zhonguo3118.cn

[S57] C++：编译期常量
来源：https://jk.zhonguo4118.cn

constexpr int N = 10;
来源：https://sb.zhonguo2118.cn

[S58] C++：命名空间
来源：https://iq.zhonguo6118.cn

namespace ns { int f() { return 1; } }
来源：https://xz.zhonguo6118.cn

[S59] C++：静态断言
来源：https://cs.zhonguo3118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://ha.zhonguo5118.cn

[S60] C++：遍历并删除元素
来源：https://iw.zhonguo4118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://dv.zhonguo6118.cn

================================================================================
来源：https://xj.zhonguo4118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://mt.zhonguo3118.cn

================================================================================
来源：https://vb.zhonguo6118.cn

[T01] Kotlin：Hello World
来源：https://fg.zhonguo2118.cn

println("Hello")
来源：https://hg.zhonguo5118.cn

[T02] Kotlin：变量
来源：https://og.zhonguo1118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://tj.zhonguo7118.cn

[T03] Kotlin：字符串模板
来源：https://bc.zhonguo6118.cn

"值: $b"
来源：https://dk.zhonguo8118.cn

[T04] Kotlin：空安全
来源：https://jg.zhonguo1118.cn

val n: String? = null;  n?.length
来源：https://ij.zhonguo3118.cn

[T05] Kotlin：when 表达式
来源：https://jf.zhonguo8118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://qp.zhonguo6118.cn

[T06] Kotlin：集合映射
来源：https://ka.zhonguo6118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://ca.zhonguo6118.cn

[T07] Kotlin：集合过滤
来源：https://lx.zhonguo5118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://ck.zhonguo7118.cn

[T08] Kotlin：数据类
来源：https://kv.zhonguo1118.cn

data class User(val name: String, val age: Int)
来源：https://ne.zhonguo8118.cn

[T09] Kotlin：扩展函数
来源：https://nx.zhonguo1118.cn

fun String.exclaim() = this + "!"
来源：https://db.zhonguo8118.cn

[T10] Kotlin：默认参数
来源：https://jn.zhonguo3118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://oj.zhonguo6118.cn

[T11] Kotlin：协程
来源：https://ll.zhonguo4118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://jp.zhonguo3118.cn

[T12] Kotlin：解构声明
来源：https://rk.zhonguo4118.cn

val (a, b) = Pair(1, 2)
来源：https://ln.zhonguo7118.cn

[T13] Kotlin：只读 Map
来源：https://zb.zhonguo4118.cn

val m = mapOf("a" to 1)
来源：https://od.zhonguo8118.cn

[T14] Kotlin：循环
来源：https://qy.zhonguo4118.cn

for (i in 1..10) println(i)
来源：https://fz.zhonguo4118.cn

[T15] Kotlin：接口
来源：https://ro.zhonguo7118.cn

interface Shape { fun area(): Double }
来源：https://gr.zhonguo1118.cn

[T16] Swift：Hello World
来源：https://dj.zhonguo5118.cn

print("Hello")
来源：https://qd.zhonguo6118.cn

[T17] Swift：变量与常量
来源：https://rw.zhonguo1118.cn

var a = 1;  let b = 2
来源：https://iw.zhonguo6118.cn

[T18] Swift：字符串插值
来源：https://dr.zhonguo5118.cn

"值: \(b)"
来源：https://nj.zhonguo6118.cn

[T19] Swift：可选绑定
来源：https://ls.zhonguo7118.cn

if let n = opt { print(n) }
来源：https://pq.zhonguo6118.cn

[T20] Swift：数组操作
来源：https://fn.zhonguo6118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://fw.zhonguo4118.cn

[T21] Swift：遍历
来源：https://tk.zhonguo2118.cn

for x in a { print(x) }
来源：https://my.zhonguo2118.cn

[T22] Swift：字典
来源：https://bb.zhonguo7118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://ai.zhonguo4118.cn

[T23] Swift：函数
来源：https://lx.zhonguo3118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://gv.zhonguo4118.cn

[T24] Swift：闭包
来源：https://vo.zhonguo6118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://uw.zhonguo7118.cn

[T25] Swift：结构体
来源：https://mv.zhonguo2118.cn

struct P { var x: Int }
来源：https://tr.zhonguo2118.cn

[T26] Swift：类与重写
来源：https://oq.zhonguo7118.cn

class A: Base { override func f() {} }
来源：https://wn.zhonguo8118.cn

[T27] Swift：错误处理
来源：https://dl.zhonguo3118.cn

do { try f() } catch { print(error) }
来源：https://ax.zhonguo8118.cn

[T28] Swift：枚举
来源：https://vx.zhonguo2118.cn

enum Color { case red, green }
来源：https://oo.zhonguo6118.cn

[T29] Swift：guard 提前返回
来源：https://wd.zhonguo3118.cn

guard let x = opt else { return }
来源：https://vg.zhonguo8118.cn

[T30] Swift：协议
来源：https://xo.zhonguo4118.cn

protocol Shape { func area() -> Double }
来源：https://se.zhonguo8118.cn

[T31] Lua：Hello World
来源：https://wm.zhonguo1118.cn

print("Hello")
来源：https://pp.zhonguo1118.cn

[T32] Lua：局部变量
来源：https://je.zhonguo1118.cn

local a = 1
来源：https://ml.zhonguo5118.cn

[T33] Lua：表（数组）
来源：https://zi.zhonguo1118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://uq.zhonguo4118.cn

[T34] Lua：遍历表
来源：https://ad.zhonguo6118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://yv.zhonguo8118.cn

[T35] Lua：字典表
来源：https://zx.zhonguo3118.cn

local d = { a = 1 };  d.b = 2
来源：https://qt.zhonguo6118.cn

[T36] Lua：函数
来源：https://oj.zhonguo4118.cn

function add(a, b) return a + b end
来源：https://mz.zhonguo2118.cn

[T37] Lua：字符串拼接
来源：https://ya.zhonguo8118.cn

"a" .. "b"
来源：https://ni.zhonguo5118.cn

[T38] Lua：条件
来源：https://hs.zhonguo3118.cn

if x > 0 then print("正") end
来源：https://ro.zhonguo5118.cn

[T39] Lua：模式匹配
来源：https://vi.zhonguo2118.cn

string.find(s, "%d+")
来源：https://ku.zhonguo4118.cn

[T40] Lua：元表
来源：https://fb.zhonguo3118.cn

setmetatable({}, { __index = base })
来源：https://vd.zhonguo5118.cn

[T41] Perl：Hello World
来源：https://rn.zhonguo3118.cn

print "Hello\n";
来源：https://gk.zhonguo1118.cn

[T42] Perl：变量类型
来源：https://jv.zhonguo3118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://vh.zhonguo8118.cn

[T43] Perl：字符串插值
来源：https://dm.zhonguo8118.cn

"值: $a"
来源：https://nm.zhonguo1118.cn

[T44] Perl：条件
来源：https://bp.zhonguo8118.cn

if ($a > 0) { print "正"; }
来源：https://pm.zhonguo6118.cn

[T45] Perl：数组遍历
来源：https://zz.zhonguo4118.cn

for my $x (@arr) { print $x; }
来源：https://qt.zhonguo5118.cn

[T46] Perl：哈希操作
来源：https://nm.zhonguo3118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://xw.zhonguo5118.cn

[T47] Perl：正则捕获
来源：https://ck.zhonguo6118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://mx.zhonguo4118.cn

[T48] Perl：正则替换
来源：https://mc.zhonguo1118.cn

$s =~ s/old/new/g;
来源：https://ex.zhonguo4118.cn

[T49] Perl：函数
来源：https://vh.zhonguo6118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://qt.zhonguo6118.cn

[T50] Perl：逐行读文件
来源：https://nr.zhonguo4118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://qt.zhonguo2118.cn

while (my $line = <$fh>) { print $line; }
来源：https://fm.zhonguo5118.cn

[T51] Scala：Hello World
来源：https://tg.zhonguo1118.cn

println("Hello")
来源：https://xj.zhonguo4118.cn

[T52] Scala：变量
来源：https://us.zhonguo1118.cn

val a = 1;  var b = 2
来源：https://sm.zhonguo5118.cn

[T53] Scala：字符串插值
来源：https://ki.zhonguo6118.cn

s"值: $b"
来源：https://ou.zhonguo5118.cn

[T54] Scala：集合映射
来源：https://qc.zhonguo3118.cn

List(1, 2, 3).map(_ * 2)
来源：https://do.zhonguo6118.cn

[T55] Scala：集合过滤
来源：https://dv.zhonguo5118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://fx.zhonguo1118.cn

[T56] Scala：样例类
来源：https://ag.zhonguo4118.cn

case class User(name: String, age: Int)
来源：https://nf.zhonguo2118.cn

[T57] Scala：模式匹配
来源：https://oo.zhonguo5118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://ud.zhonguo6118.cn

[T58] Scala：函数定义
来源：https://gj.zhonguo7118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://zx.zhonguo4118.cn

[T59] Scala：循环
来源：https://dh.zhonguo2118.cn

for (i <- 1 to 10) println(i)
来源：https://lu.zhonguo6118.cn

[T60] Scala：折叠
来源：https://nx.zhonguo7118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://se.zhonguo3118.cn

================================================================================
来源：https://ra.zhonguo5118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://eq.zhonguo6118.cn

================================================================================
来源：https://ag.zhonguo4118.cn

[U01] Py：创建虚拟环境
来源：https://pn.zhonguo4118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://dy.zhonguo1118.cn

[U02] Py：导出 / 安装依赖
来源：https://bh.zhonguo5118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://tc.zhonguo4118.cn

[U03] Py：加载 .env 配置
来源：https://qw.zhonguo5118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://jx.zhonguo7118.cn

[U04] Py：变量调试打印
来源：https://te.zhonguo7118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://eq.zhonguo7118.cn

[U05] Py：列表去重且保序
来源：https://ly.zhonguo7118.cn

list(dict.fromkeys(arr))
来源：https://fy.zhonguo2118.cn

[U06] Py：合并两个字典
来源：https://df.zhonguo7118.cn

{**a, **b}
来源：https://no.zhonguo5118.cn

[U07] Py：反转字典键值
来源：https://ou.zhonguo6118.cn

{v: k for k, v in d.items()}
来源：https://ru.zhonguo3118.cn

[U08] Py：展平二维列表
来源：https://df.zhonguo5118.cn

[y for x in nested for y in x]
来源：https://yt.zhonguo6118.cn

[U09] Py：字典取最大值的键
来源：https://pn.zhonguo5118.cn

max(d, key=d.get)
来源：https://fq.zhonguo2118.cn

[U10] Py：按值排序字典
来源：https://my.zhonguo8118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://pm.zhonguo2118.cn

[U11] Py：生成器表达式
来源：https://kz.zhonguo5118.cn

(x * 2 for x in arr)
来源：https://pa.zhonguo6118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://mt.zhonguo1118.cn

Counter(arr).most_common(3)
来源：https://ai.zhonguo5118.cn

[U13] Py：固定长度队列
来源：https://ka.zhonguo8118.cn

deque(maxlen=10)
来源：https://nc.zhonguo8118.cn

[U14] Py：分组收集到列表
来源：https://hc.zhonguo6118.cn

defaultdict(list)
来源：https://zs.zhonguo4118.cn

[U15] Py：高精度计时
来源：https://vw.zhonguo3118.cn

t = time.perf_counter()
来源：https://re.zhonguo1118.cn

[U16] Py：命令行参数解析
来源：https://hx.zhonguo6118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://uo.zhonguo2118.cn

[U17] Py：初始化日志
来源：https://cs.zhonguo1118.cn

logging.basicConfig(level=logging.INFO)
来源：https://gw.zhonguo7118.cn

[U18] Py：预编译正则
来源：https://hb.zhonguo2118.cn

pat = re.compile(r"\d+")
来源：https://da.zhonguo8118.cn

[U19] Py：正则替换带回调
来源：https://xt.zhonguo7118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://kr.zhonguo5118.cn

[U20] Py：缓存函数结果
来源：https://dm.zhonguo3118.cn

@functools.lru_cache(maxsize=None)
来源：https://kr.zhonguo5118.cn

[U21] Py：自定义上下文管理器
来源：https://id.zhonguo6118.cn

@contextlib.contextmanager
来源：https://cu.zhonguo8118.cn

[U22] Py：矩阵转置
来源：https://il.zhonguo2118.cn

list(zip(*m))
来源：https://kd.zhonguo5118.cn

[U23] Py：分块读取大文件
来源：https://qb.zhonguo6118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://jh.zhonguo4118.cn

[U24] Py：路径操作
来源：https://bl.zhonguo8118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://uk.zhonguo6118.cn

[U25] Py：CSV 按字典读
来源：https://ft.zhonguo6118.cn

csv.DictReader(f)
来源：https://hb.zhonguo1118.cn

[U26] Py：并发下载
来源：https://wq.zhonguo5118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://ld.zhonguo7118.cn

[U27] Py：异步 HTTP
来源：https://ns.zhonguo4118.cn

aiohttp.ClientSession() 配合 async with
来源：https://wy.zhonguo6118.cn

[U28] Py：类型别名
来源：https://jb.zhonguo5118.cn

UserId = int
来源：https://ip.zhonguo4118.cn

[U29] Py：属性校验
来源：https://gm.zhonguo5118.cn

@property 与 @x.setter 配合
来源：https://xv.zhonguo1118.cn

[U30] Py：数据类
来源：https://qg.zhonguo1118.cn

@dataclass(slots=True)
来源：https://qu.zhonguo2118.cn

[U31] Py：单测
来源：https://rv.zhonguo3118.cn

python -m pytest -q
来源：https://bp.zhonguo2118.cn

[U32] Py：代码格式化
来源：https://ze.zhonguo1118.cn

ruff format . && ruff check --fix .
来源：https://pu.zhonguo4118.cn

[U33] Py：打包发布
来源：https://pq.zhonguo2118.cn

python -m build  （依赖 pyproject.toml）
来源：https://sw.zhonguo1118.cn

[U34] Py：判断编码
来源：https://nf.zhonguo5118.cn

chardet.detect(raw)
来源：https://xg.zhonguo4118.cn

[U35] Py：发送邮件
来源：https://yy.zhonguo5118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://oq.zhonguo6118.cn

[U36] Py：定时任务
来源：https://pc.zhonguo2118.cn

schedule.every(10).minutes.do(job)
来源：https://jx.zhonguo6118.cn

[U37] Py：读写 Excel
来源：https://ly.zhonguo7118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://bv.zhonguo3118.cn

[U38] Py：获取脚本所在目录
来源：https://yq.zhonguo6118.cn

Path(__file__).resolve().parent
来源：https://mh.zhonguo2118.cn

[U39] Py：判断是否在交互环境
来源：https://he.zhonguo7118.cn

sys.stdout.isatty()
来源：https://le.zhonguo4118.cn

[U40] Py：打印到标准错误
来源：https://oq.zhonguo8118.cn

print("err", file=sys.stderr)
来源：https://jw.zhonguo2118.cn

[U41] PHP：初始化 Composer 项目
来源：https://pu.zhonguo6118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://fc.zhonguo6118.cn

[U42] PHP：PSR-4 自动加载
来源：https://jw.zhonguo7118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://mm.zhonguo6118.cn

[U43] PHP：声明命名空间
来源：https://mk.zhonguo4118.cn

namespace App\Http;
来源：https://zs.zhonguo2118.cn

[U44] PHP：开启严格类型
来源：https://yh.zhonguo3118.cn

declare(strict_types=1);
来源：https://fx.zhonguo7118.cn

[U45] PHP：类型声明与返回类型
来源：https://yd.zhonguo5118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://xq.zhonguo6118.cn

[U46] PHP：可空类型
来源：https://ud.zhonguo7118.cn

?string $name = null
来源：https://ke.zhonguo7118.cn

[U47] PHP：联合类型
来源：https://py.zhonguo3118.cn

int|string $id
来源：https://tp.zhonguo3118.cn

[U48] PHP：纯枚举
来源：https://jo.zhonguo7118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://kv.zhonguo6118.cn

[U49] PHP：只读属性
来源：https://tc.zhonguo1118.cn

public readonly string $name
来源：https://bb.zhonguo4118.cn

[U50] PHP：构造器属性提升
来源：https://qk.zhonguo4118.cn

public function __construct(private int $id) {}
来源：https://cf.zhonguo5118.cn

[U51] PHP：数组解构
来源：https://yu.zhonguo7118.cn

[$a, $b] = $arr;
来源：https://yi.zhonguo4118.cn

[U52] PHP：箭头函数
来源：https://ek.zhonguo2118.cn

$double = fn($x) => $x * 2;
来源：https://wm.zhonguo3118.cn

[U53] PHP：空合并运算符
来源：https://iz.zhonguo4118.cn

$v = $a ?? $b ?? "default";
来源：https://kx.zhonguo7118.cn

[U54] PHP：空安全调用
来源：https://yq.zhonguo8118.cn

$obj?->method()
来源：https://rn.zhonguo2118.cn

[U55] PHP：match 表达式
来源：https://rw.zhonguo5118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://ib.zhonguo4118.cn

[U56] PHP：命名参数
来源：https://sy.zhonguo2118.cn

f(a: 1, b: 2)
来源：https://gi.zhonguo4118.cn

[U57] PHP：字符串插值
来源：https://ky.zhonguo6118.cn

"值: {$a}"
来源：https://ze.zhonguo1118.cn

[U58] PHP：数组三件套
来源：https://hy.zhonguo2118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://eo.zhonguo7118.cn

[U59] PHP：自定义排序
来源：https://bh.zhonguo4118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://jl.zhonguo4118.cn

[U60] PHP：JSON 编解码
来源：https://rh.zhonguo2118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://bt.zhonguo8118.cn

[U61] PHP：正则
来源：https://ms.zhonguo3118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://th.zhonguo8118.cn

[U62] PHP：日期对象
来源：https://nl.zhonguo4118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://mu.zhonguo4118.cn

[U63] PHP：文件读写
来源：https://zi.zhonguo5118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://by.zhonguo7118.cn

[U64] PHP：目录遍历
来源：https://hm.zhonguo1118.cn

glob("dir/*.php");  scandir("dir");
来源：https://ys.zhonguo1118.cn

[U65] PHP：会话
来源：https://rf.zhonguo8118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://eg.zhonguo7118.cn

[U66] PHP：设置 Cookie
来源：https://oq.zhonguo5118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://rj.zhonguo3118.cn

[U67] PHP：处理文件上传
来源：https://wy.zhonguo6118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://no.zhonguo7118.cn

[U68] PHP：PDO 连接
来源：https://qx.zhonguo4118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://um.zhonguo3118.cn

[U69] PHP：PDO 预处理
来源：https://vn.zhonguo1118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://sl.zhonguo2118.cn

[U70] PHP：PDO 事务
来源：https://yy.zhonguo5118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://oc.zhonguo5118.cn

[U71] PHP：抛出异常
来源：https://hd.zhonguo5118.cn

throw new RuntimeException("失败", 500);
来源：https://tj.zhonguo3118.cn

[U72] PHP：写错误日志
来源：https://lq.zhonguo2118.cn

error_log("失败: " . $e->getMessage());
来源：https://rv.zhonguo5118.cn

[U73] PHP：读取 ini 配置
来源：https://pf.zhonguo8118.cn

parse_ini_file("config.ini", true)
来源：https://ap.zhonguo1118.cn

[U74] PHP：读取环境变量
来源：https://ik.zhonguo1118.cn

getenv("APP_ENV") ?: "production"
来源：https://ba.zhonguo6118.cn


<!-- 参考信息 -->