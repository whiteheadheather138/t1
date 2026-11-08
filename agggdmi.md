代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://sp.zhonguo7118.cn

[S51] C++：显式类型转换
来源：https://jh.zhonguo6118.cn

static_cast<double>(a) / b
来源：https://cu.zhonguo3118.cn

[S52] C++：const 与 noexcept
来源：https://xe.zhonguo2118.cn

int size() const noexcept { return n_; }
来源：https://yf.zhonguo1118.cn

[S53] C++：移动语义
来源：https://la.zhonguo2118.cn

std::vector<int> w = std::move(v);
来源：https://sj.zhonguo2118.cn

[S54] C++：异常处理
来源：https://xa.zhonguo3118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://zg.zhonguo4118.cn

[S55] C++：结构化绑定
来源：https://jr.zhonguo2118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://xq.zhonguo1118.cn

[S56] C++：optional
来源：https://bt.zhonguo8118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://bw.zhonguo3118.cn

[S57] C++：编译期常量
来源：https://ju.zhonguo2118.cn

constexpr int N = 10;
来源：https://ep.zhonguo6118.cn

[S58] C++：命名空间
来源：https://hz.zhonguo5118.cn

namespace ns { int f() { return 1; } }
来源：https://qn.zhonguo2118.cn

[S59] C++：静态断言
来源：https://cv.zhonguo1118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://ce.zhonguo6118.cn

[S60] C++：遍历并删除元素
来源：https://jz.zhonguo7118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://dc.zhonguo6118.cn

================================================================================
来源：https://ej.zhonguo5118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://hk.zhonguo1118.cn

================================================================================
来源：https://da.zhonguo1118.cn

[T01] Kotlin：Hello World
来源：https://qp.zhonguo7118.cn

println("Hello")
来源：https://gk.zhonguo7118.cn

[T02] Kotlin：变量
来源：https://mr.zhonguo7118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://hv.zhonguo2118.cn

[T03] Kotlin：字符串模板
来源：https://gy.zhonguo8118.cn

"值: $b"
来源：https://by.zhonguo4118.cn

[T04] Kotlin：空安全
来源：https://bh.zhonguo3118.cn

val n: String? = null;  n?.length
来源：https://ym.zhonguo5118.cn

[T05] Kotlin：when 表达式
来源：https://ii.zhonguo6118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://uq.zhonguo1118.cn

[T06] Kotlin：集合映射
来源：https://za.zhonguo5118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://fq.zhonguo4118.cn

[T07] Kotlin：集合过滤
来源：https://va.zhonguo8118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://ae.zhonguo4118.cn

[T08] Kotlin：数据类
来源：https://zi.zhonguo6118.cn

data class User(val name: String, val age: Int)
来源：https://hx.zhonguo1118.cn

[T09] Kotlin：扩展函数
来源：https://bp.zhonguo4118.cn

fun String.exclaim() = this + "!"
来源：https://gj.zhonguo6118.cn

[T10] Kotlin：默认参数
来源：https://hy.zhonguo7118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://ow.zhonguo6118.cn

[T11] Kotlin：协程
来源：https://sv.zhonguo4118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://ye.zhonguo4118.cn

[T12] Kotlin：解构声明
来源：https://kd.zhonguo8118.cn

val (a, b) = Pair(1, 2)
来源：https://lj.zhonguo3118.cn

[T13] Kotlin：只读 Map
来源：https://qv.zhonguo6118.cn

val m = mapOf("a" to 1)
来源：https://so.zhonguo1118.cn

[T14] Kotlin：循环
来源：https://mz.zhonguo7118.cn

for (i in 1..10) println(i)
来源：https://ae.zhonguo6118.cn

[T15] Kotlin：接口
来源：https://yt.zhonguo8118.cn

interface Shape { fun area(): Double }
来源：https://xo.zhonguo8118.cn

[T16] Swift：Hello World
来源：https://ap.zhonguo7118.cn

print("Hello")
来源：https://zr.zhonguo5118.cn

[T17] Swift：变量与常量
来源：https://si.zhonguo8118.cn

var a = 1;  let b = 2
来源：https://cq.zhonguo2118.cn

[T18] Swift：字符串插值
来源：https://nk.zhonguo7118.cn

"值: \(b)"
来源：https://fk.zhonguo6118.cn

[T19] Swift：可选绑定
来源：https://qv.zhonguo3118.cn

if let n = opt { print(n) }
来源：https://bp.zhonguo7118.cn

[T20] Swift：数组操作
来源：https://ls.zhonguo7118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://bl.zhonguo7118.cn

[T21] Swift：遍历
来源：https://pl.zhonguo3118.cn

for x in a { print(x) }
来源：https://vm.zhonguo7118.cn

[T22] Swift：字典
来源：https://sv.zhonguo7118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://xt.zhonguo5118.cn

[T23] Swift：函数
来源：https://xm.zhonguo3118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://lc.zhonguo5118.cn

[T24] Swift：闭包
来源：https://nh.zhonguo6118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://ta.zhonguo5118.cn

[T25] Swift：结构体
来源：https://la.zhonguo2118.cn

struct P { var x: Int }
来源：https://sn.zhonguo3118.cn

[T26] Swift：类与重写
来源：https://ni.zhonguo6118.cn

class A: Base { override func f() {} }
来源：https://rl.zhonguo8118.cn

[T27] Swift：错误处理
来源：https://ny.zhonguo2118.cn

do { try f() } catch { print(error) }
来源：https://pa.zhonguo5118.cn

[T28] Swift：枚举
来源：https://mz.zhonguo3118.cn

enum Color { case red, green }
来源：https://zr.zhonguo3118.cn

[T29] Swift：guard 提前返回
来源：https://bk.zhonguo6118.cn

guard let x = opt else { return }
来源：https://qt.zhonguo2118.cn

[T30] Swift：协议
来源：https://jk.zhonguo2118.cn

protocol Shape { func area() -> Double }
来源：https://ap.zhonguo6118.cn

[T31] Lua：Hello World
来源：https://lm.zhonguo2118.cn

print("Hello")
来源：https://es.zhonguo6118.cn

[T32] Lua：局部变量
来源：https://wf.zhonguo7118.cn

local a = 1
来源：https://ax.zhonguo4118.cn

[T33] Lua：表（数组）
来源：https://zx.zhonguo3118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://hw.zhonguo5118.cn

[T34] Lua：遍历表
来源：https://al.zhonguo4118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://hm.zhonguo6118.cn

[T35] Lua：字典表
来源：https://mh.zhonguo1118.cn

local d = { a = 1 };  d.b = 2
来源：https://it.zhonguo4118.cn

[T36] Lua：函数
来源：https://ab.zhonguo2118.cn

function add(a, b) return a + b end
来源：https://tf.zhonguo4118.cn

[T37] Lua：字符串拼接
来源：https://xf.zhonguo8118.cn

"a" .. "b"
来源：https://ye.zhonguo3118.cn

[T38] Lua：条件
来源：https://vd.zhonguo2118.cn

if x > 0 then print("正") end
来源：https://it.zhonguo5118.cn

[T39] Lua：模式匹配
来源：https://cn.zhonguo6118.cn

string.find(s, "%d+")
来源：https://dn.zhonguo3118.cn

[T40] Lua：元表
来源：https://kb.zhonguo5118.cn

setmetatable({}, { __index = base })
来源：https://sb.zhonguo5118.cn

[T41] Perl：Hello World
来源：https://es.zhonguo2118.cn

print "Hello\n";
来源：https://iv.zhonguo4118.cn

[T42] Perl：变量类型
来源：https://sy.zhonguo6118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://fh.zhonguo7118.cn

[T43] Perl：字符串插值
来源：https://gt.zhonguo6118.cn

"值: $a"
来源：https://gm.zhonguo2118.cn

[T44] Perl：条件
来源：https://ut.zhonguo6118.cn

if ($a > 0) { print "正"; }
来源：https://qq.zhonguo7118.cn

[T45] Perl：数组遍历
来源：https://qj.zhonguo6118.cn

for my $x (@arr) { print $x; }
来源：https://ik.zhonguo5118.cn

[T46] Perl：哈希操作
来源：https://lj.zhonguo4118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://ch.zhonguo3118.cn

[T47] Perl：正则捕获
来源：https://vg.zhonguo4118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://pm.zhonguo6118.cn

[T48] Perl：正则替换
来源：https://sw.zhonguo6118.cn

$s =~ s/old/new/g;
来源：https://il.zhonguo7118.cn

[T49] Perl：函数
来源：https://tu.zhonguo4118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://wr.zhonguo5118.cn

[T50] Perl：逐行读文件
来源：https://er.zhonguo4118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://pu.zhonguo1118.cn

while (my $line = <$fh>) { print $line; }
来源：https://le.zhonguo1118.cn

[T51] Scala：Hello World
来源：https://bs.zhonguo1118.cn

println("Hello")
来源：https://xc.zhonguo6118.cn

[T52] Scala：变量
来源：https://aw.zhonguo1118.cn

val a = 1;  var b = 2
来源：https://nz.zhonguo6118.cn

[T53] Scala：字符串插值
来源：https://ot.zhonguo8118.cn

s"值: $b"
来源：https://ov.zhonguo6118.cn

[T54] Scala：集合映射
来源：https://qo.zhonguo5118.cn

List(1, 2, 3).map(_ * 2)
来源：https://ip.zhonguo2118.cn

[T55] Scala：集合过滤
来源：https://em.zhonguo1118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://ei.zhonguo5118.cn

[T56] Scala：样例类
来源：https://hb.zhonguo5118.cn

case class User(name: String, age: Int)
来源：https://km.zhonguo3118.cn

[T57] Scala：模式匹配
来源：https://kj.zhonguo5118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://vl.zhonguo1118.cn

[T58] Scala：函数定义
来源：https://ly.zhonguo3118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://gh.zhonguo8118.cn

[T59] Scala：循环
来源：https://xr.zhonguo3118.cn

for (i <- 1 to 10) println(i)
来源：https://oj.zhonguo5118.cn

[T60] Scala：折叠
来源：https://lj.zhonguo6118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://er.zhonguo4118.cn

================================================================================
来源：https://ti.zhonguo7118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://ik.zhonguo7118.cn

================================================================================
来源：https://dk.zhonguo3118.cn

[U01] Py：创建虚拟环境
来源：https://aq.zhonguo4118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://py.zhonguo8118.cn

[U02] Py：导出 / 安装依赖
来源：https://lh.zhonguo7118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://rl.zhonguo6118.cn

[U03] Py：加载 .env 配置
来源：https://tf.zhonguo3118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://qp.zhonguo5118.cn

[U04] Py：变量调试打印
来源：https://tz.zhonguo4118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://gl.zhonguo5118.cn

[U05] Py：列表去重且保序
来源：https://cg.zhonguo7118.cn

list(dict.fromkeys(arr))
来源：https://ko.zhonguo7118.cn

[U06] Py：合并两个字典
来源：https://ic.zhonguo2118.cn

{**a, **b}
来源：https://gz.zhonguo5118.cn

[U07] Py：反转字典键值
来源：https://fh.zhonguo2118.cn

{v: k for k, v in d.items()}
来源：https://ev.zhonguo2118.cn

[U08] Py：展平二维列表
来源：https://yi.zhonguo8118.cn

[y for x in nested for y in x]
来源：https://xj.zhonguo6118.cn

[U09] Py：字典取最大值的键
来源：https://rl.zhonguo1118.cn

max(d, key=d.get)
来源：https://ek.zhonguo8118.cn

[U10] Py：按值排序字典
来源：https://cu.zhonguo4118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://pq.zhonguo7118.cn

[U11] Py：生成器表达式
来源：https://zl.zhonguo5118.cn

(x * 2 for x in arr)
来源：https://oj.zhonguo7118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://um.zhonguo5118.cn

Counter(arr).most_common(3)
来源：https://tm.zhonguo1118.cn

[U13] Py：固定长度队列
来源：https://dx.zhonguo5118.cn

deque(maxlen=10)
来源：https://rh.zhonguo7118.cn

[U14] Py：分组收集到列表
来源：https://ye.zhonguo8118.cn

defaultdict(list)
来源：https://zw.zhonguo4118.cn

[U15] Py：高精度计时
来源：https://ri.zhonguo1118.cn

t = time.perf_counter()
来源：https://or.zhonguo5118.cn

[U16] Py：命令行参数解析
来源：https://bg.zhonguo1118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://uk.zhonguo6118.cn

[U17] Py：初始化日志
来源：https://vo.zhonguo5118.cn

logging.basicConfig(level=logging.INFO)
来源：https://gi.zhonguo1118.cn

[U18] Py：预编译正则
来源：https://np.zhonguo7118.cn

pat = re.compile(r"\d+")
来源：https://uz.zhonguo5118.cn

[U19] Py：正则替换带回调
来源：https://xp.zhonguo5118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://bu.zhonguo8118.cn

[U20] Py：缓存函数结果
来源：https://lw.zhonguo7118.cn

@functools.lru_cache(maxsize=None)
来源：https://lx.zhonguo2118.cn

[U21] Py：自定义上下文管理器
来源：https://gf.zhonguo7118.cn

@contextlib.contextmanager
来源：https://vv.zhonguo7118.cn

[U22] Py：矩阵转置
来源：https://nl.zhonguo1118.cn

list(zip(*m))
来源：https://fv.zhonguo2118.cn

[U23] Py：分块读取大文件
来源：https://vu.zhonguo8118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://bg.zhonguo7118.cn

[U24] Py：路径操作
来源：https://um.zhonguo3118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://ul.zhonguo5118.cn

[U25] Py：CSV 按字典读
来源：https://do.zhonguo8118.cn

csv.DictReader(f)
来源：https://se.zhonguo1118.cn

[U26] Py：并发下载
来源：https://me.zhonguo2118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://tv.zhonguo6118.cn

[U27] Py：异步 HTTP
来源：https://qr.zhonguo8118.cn

aiohttp.ClientSession() 配合 async with
来源：https://dv.zhonguo8118.cn

[U28] Py：类型别名
来源：https://ua.zhonguo3118.cn

UserId = int
来源：https://zn.zhonguo6118.cn

[U29] Py：属性校验
来源：https://mj.zhonguo3118.cn

@property 与 @x.setter 配合
来源：https://pr.zhonguo2118.cn

[U30] Py：数据类
来源：https://sv.zhonguo1118.cn

@dataclass(slots=True)
来源：https://uq.zhonguo3118.cn

[U31] Py：单测
来源：https://yn.zhonguo4118.cn

python -m pytest -q
来源：https://wy.zhonguo7118.cn

[U32] Py：代码格式化
来源：https://us.zhonguo2118.cn

ruff format . && ruff check --fix .
来源：https://le.zhonguo3118.cn

[U33] Py：打包发布
来源：https://yg.zhonguo3118.cn

python -m build  （依赖 pyproject.toml）
来源：https://tn.zhonguo5118.cn

[U34] Py：判断编码
来源：https://hx.zhonguo8118.cn

chardet.detect(raw)
来源：https://ia.zhonguo8118.cn

[U35] Py：发送邮件
来源：https://ge.zhonguo1118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://xf.zhonguo2118.cn

[U36] Py：定时任务
来源：https://fh.zhonguo5118.cn

schedule.every(10).minutes.do(job)
来源：https://px.zhonguo2118.cn

[U37] Py：读写 Excel
来源：https://lz.zhonguo4118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://pj.zhonguo3118.cn

[U38] Py：获取脚本所在目录
来源：https://yo.zhonguo4118.cn

Path(__file__).resolve().parent
来源：https://qz.zhonguo4118.cn

[U39] Py：判断是否在交互环境
来源：https://zo.zhonguo2118.cn

sys.stdout.isatty()
来源：https://nb.zhonguo4118.cn

[U40] Py：打印到标准错误
来源：https://of.zhonguo8118.cn

print("err", file=sys.stderr)
来源：https://yt.zhonguo8118.cn

[U41] PHP：初始化 Composer 项目
来源：https://kf.zhonguo6118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://cf.zhonguo7118.cn

[U42] PHP：PSR-4 自动加载
来源：https://tl.zhonguo8118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://da.zhonguo3118.cn

[U43] PHP：声明命名空间
来源：https://jl.zhonguo3118.cn

namespace App\Http;
来源：https://bg.zhonguo8118.cn

[U44] PHP：开启严格类型
来源：https://ic.zhonguo5118.cn

declare(strict_types=1);
来源：https://dz.zhonguo8118.cn

[U45] PHP：类型声明与返回类型
来源：https://xn.zhonguo1118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://xv.zhonguo5118.cn

[U46] PHP：可空类型
来源：https://gt.zhonguo6118.cn

?string $name = null
来源：https://xo.zhonguo5118.cn

[U47] PHP：联合类型
来源：https://xy.zhonguo7118.cn

int|string $id
来源：https://ie.zhonguo5118.cn

[U48] PHP：纯枚举
来源：https://aq.zhonguo4118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://ic.zhonguo7118.cn

[U49] PHP：只读属性
来源：https://qp.zhonguo8118.cn

public readonly string $name
来源：https://ml.zhonguo3118.cn

[U50] PHP：构造器属性提升
来源：https://cr.zhonguo5118.cn

public function __construct(private int $id) {}
来源：https://ff.zhonguo8118.cn

[U51] PHP：数组解构
来源：https://oz.zhonguo2118.cn

[$a, $b] = $arr;
来源：https://tw.zhonguo3118.cn

[U52] PHP：箭头函数
来源：https://xy.zhonguo4118.cn

$double = fn($x) => $x * 2;
来源：https://zy.zhonguo3118.cn

[U53] PHP：空合并运算符
来源：https://yp.zhonguo5118.cn

$v = $a ?? $b ?? "default";
来源：https://pk.zhonguo6118.cn

[U54] PHP：空安全调用
来源：https://ez.zhonguo1118.cn

$obj?->method()
来源：https://mf.zhonguo4118.cn

[U55] PHP：match 表达式
来源：https://vl.zhonguo2118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://gk.zhonguo1118.cn

[U56] PHP：命名参数
来源：https://lt.zhonguo7118.cn

f(a: 1, b: 2)
来源：https://bg.zhonguo2118.cn

[U57] PHP：字符串插值
来源：https://jo.zhonguo5118.cn

"值: {$a}"
来源：https://rv.zhonguo6118.cn

[U58] PHP：数组三件套
来源：https://pj.zhonguo2118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://dl.zhonguo1118.cn

[U59] PHP：自定义排序
来源：https://gx.zhonguo6118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://bs.zhonguo8118.cn

[U60] PHP：JSON 编解码
来源：https://ga.zhonguo4118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://tj.zhonguo2118.cn

[U61] PHP：正则
来源：https://co.zhonguo3118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://re.zhonguo3118.cn

[U62] PHP：日期对象
来源：https://bd.zhonguo8118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://pt.zhonguo5118.cn

[U63] PHP：文件读写
来源：https://xb.zhonguo5118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://av.zhonguo1118.cn

[U64] PHP：目录遍历
来源：https://je.zhonguo8118.cn

glob("dir/*.php");  scandir("dir");
来源：https://wd.zhonguo4118.cn

[U65] PHP：会话
来源：https://fl.zhonguo3118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://ay.zhonguo3118.cn

[U66] PHP：设置 Cookie
来源：https://vd.zhonguo5118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://ex.zhonguo2118.cn

[U67] PHP：处理文件上传
来源：https://vd.zhonguo8118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://qd.zhonguo5118.cn

[U68] PHP：PDO 连接
来源：https://ti.zhonguo5118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://ld.zhonguo5118.cn

[U69] PHP：PDO 预处理
来源：https://ih.zhonguo4118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://dj.zhonguo7118.cn

[U70] PHP：PDO 事务
来源：https://kp.zhonguo2118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://me.zhonguo8118.cn

[U71] PHP：抛出异常
来源：https://kh.zhonguo5118.cn

throw new RuntimeException("失败", 500);
来源：https://ve.zhonguo4118.cn

[U72] PHP：写错误日志
来源：https://ty.zhonguo7118.cn

error_log("失败: " . $e->getMessage());
来源：https://lv.zhonguo7118.cn

[U73] PHP：读取 ini 配置
来源：https://hv.zhonguo6118.cn

parse_ini_file("config.ini", true)
来源：https://za.zhonguo5118.cn

[U74] PHP：读取环境变量
来源：https://bj.zhonguo1118.cn

getenv("APP_ENV") ?: "production"
来源：https://bi.zhonguo4118.cn

[U75] PHP：依赖注入
来源：https://tu.zhonguo8118.cn

composer require psr/container
来源：https://di.zhonguo7118.cn

[U76] PHP：简单路由
来源：https://yj.zhonguo8118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://xg.zhonguo2118.cn


<!-- 参考信息 -->