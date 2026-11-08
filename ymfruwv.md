代发 wailian999

namespace ns { int f() { return 1; } }
来源：https://fo.zhonguo4118.cn

[S59] C++：静态断言
来源：https://an.zhonguo8118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://gw.zhonguo2118.cn

[S60] C++：遍历并删除元素
来源：https://oe.zhonguo6118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://cb.zhonguo1118.cn

================================================================================
来源：https://ve.zhonguo6118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://ih.zhonguo1118.cn

================================================================================
来源：https://qj.zhonguo2118.cn

[T01] Kotlin：Hello World
来源：https://yl.zhonguo5118.cn

println("Hello")
来源：https://sl.zhonguo2118.cn

[T02] Kotlin：变量
来源：https://xd.zhonguo1118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://yp.zhonguo5118.cn

[T03] Kotlin：字符串模板
来源：https://gf.zhonguo3118.cn

"值: $b"
来源：https://cw.zhonguo8118.cn

[T04] Kotlin：空安全
来源：https://at.zhonguo5118.cn

val n: String? = null;  n?.length
来源：https://gr.zhonguo7118.cn

[T05] Kotlin：when 表达式
来源：https://xg.zhonguo5118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://qs.zhonguo7118.cn

[T06] Kotlin：集合映射
来源：https://ty.zhonguo3118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://pr.zhonguo4118.cn

[T07] Kotlin：集合过滤
来源：https://jw.zhonguo6118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://rt.zhonguo3118.cn

[T08] Kotlin：数据类
来源：https://yb.zhonguo7118.cn

data class User(val name: String, val age: Int)
来源：https://qk.zhonguo2118.cn

[T09] Kotlin：扩展函数
来源：https://rp.zhonguo8118.cn

fun String.exclaim() = this + "!"
来源：https://vb.zhonguo3118.cn

[T10] Kotlin：默认参数
来源：https://ew.zhonguo1118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://ez.zhonguo7118.cn

[T11] Kotlin：协程
来源：https://vh.zhonguo8118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://qe.zhonguo2118.cn

[T12] Kotlin：解构声明
来源：https://rv.zhonguo3118.cn

val (a, b) = Pair(1, 2)
来源：https://nr.zhonguo8118.cn

[T13] Kotlin：只读 Map
来源：https://tw.zhonguo5118.cn

val m = mapOf("a" to 1)
来源：https://zx.zhonguo3118.cn

[T14] Kotlin：循环
来源：https://wl.zhonguo7118.cn

for (i in 1..10) println(i)
来源：https://eq.zhonguo3118.cn

[T15] Kotlin：接口
来源：https://se.zhonguo7118.cn

interface Shape { fun area(): Double }
来源：https://fp.zhonguo6118.cn

[T16] Swift：Hello World
来源：https://re.zhonguo5118.cn

print("Hello")
来源：https://jr.zhonguo2118.cn

[T17] Swift：变量与常量
来源：https://or.zhonguo6118.cn

var a = 1;  let b = 2
来源：https://et.zhonguo3118.cn

[T18] Swift：字符串插值
来源：https://qi.zhonguo2118.cn

"值: \(b)"
来源：https://uy.zhonguo1118.cn

[T19] Swift：可选绑定
来源：https://mx.zhonguo2118.cn

if let n = opt { print(n) }
来源：https://kl.zhonguo5118.cn

[T20] Swift：数组操作
来源：https://xn.zhonguo7118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://rt.zhonguo5118.cn

[T21] Swift：遍历
来源：https://xc.zhonguo5118.cn

for x in a { print(x) }
来源：https://kf.zhonguo7118.cn

[T22] Swift：字典
来源：https://oq.zhonguo6118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://ny.zhonguo7118.cn

[T23] Swift：函数
来源：https://pf.zhonguo6118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://hd.zhonguo8118.cn

[T24] Swift：闭包
来源：https://uu.zhonguo3118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://rd.zhonguo8118.cn

[T25] Swift：结构体
来源：https://di.zhonguo1118.cn

struct P { var x: Int }
来源：https://px.zhonguo2118.cn

[T26] Swift：类与重写
来源：https://jd.zhonguo4118.cn

class A: Base { override func f() {} }
来源：https://ta.zhonguo1118.cn

[T27] Swift：错误处理
来源：https://nj.zhonguo8118.cn

do { try f() } catch { print(error) }
来源：https://ji.zhonguo8118.cn

[T28] Swift：枚举
来源：https://uv.zhonguo7118.cn

enum Color { case red, green }
来源：https://ww.zhonguo6118.cn

[T29] Swift：guard 提前返回
来源：https://bm.zhonguo8118.cn

guard let x = opt else { return }
来源：https://mt.zhonguo4118.cn

[T30] Swift：协议
来源：https://mg.zhonguo3118.cn

protocol Shape { func area() -> Double }
来源：https://sa.zhonguo8118.cn

[T31] Lua：Hello World
来源：https://io.zhonguo1118.cn

print("Hello")
来源：https://vd.zhonguo4118.cn

[T32] Lua：局部变量
来源：https://vz.zhonguo1118.cn

local a = 1
来源：https://hj.zhonguo3118.cn

[T33] Lua：表（数组）
来源：https://xy.zhonguo2118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://ia.zhonguo1118.cn

[T34] Lua：遍历表
来源：https://fh.zhonguo8118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://un.zhonguo8118.cn

[T35] Lua：字典表
来源：https://pt.zhonguo2118.cn

local d = { a = 1 };  d.b = 2
来源：https://le.zhonguo4118.cn

[T36] Lua：函数
来源：https://pr.zhonguo1118.cn

function add(a, b) return a + b end
来源：https://an.zhonguo3118.cn

[T37] Lua：字符串拼接
来源：https://li.zhonguo4118.cn

"a" .. "b"
来源：https://gq.zhonguo8118.cn

[T38] Lua：条件
来源：https://cy.zhonguo1118.cn

if x > 0 then print("正") end
来源：https://mm.zhonguo8118.cn

[T39] Lua：模式匹配
来源：https://ux.zhonguo8118.cn

string.find(s, "%d+")
来源：https://dl.zhonguo4118.cn

[T40] Lua：元表
来源：https://wf.zhonguo3118.cn

setmetatable({}, { __index = base })
来源：https://mn.zhonguo1118.cn

[T41] Perl：Hello World
来源：https://nn.zhonguo7118.cn

print "Hello\n";
来源：https://vb.zhonguo7118.cn

[T42] Perl：变量类型
来源：https://av.zhonguo7118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://pa.zhonguo7118.cn

[T43] Perl：字符串插值
来源：https://mb.zhonguo3118.cn

"值: $a"
来源：https://by.zhonguo8118.cn

[T44] Perl：条件
来源：https://ds.zhonguo4118.cn

if ($a > 0) { print "正"; }
来源：https://ev.zhonguo7118.cn

[T45] Perl：数组遍历
来源：https://ls.zhonguo7118.cn

for my $x (@arr) { print $x; }
来源：https://ee.zhonguo3118.cn

[T46] Perl：哈希操作
来源：https://xi.zhonguo6118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://wh.zhonguo6118.cn

[T47] Perl：正则捕获
来源：https://sh.zhonguo6118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://wc.zhonguo4118.cn

[T48] Perl：正则替换
来源：https://at.zhonguo8118.cn

$s =~ s/old/new/g;
来源：https://jr.zhonguo8118.cn

[T49] Perl：函数
来源：https://pg.zhonguo2118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://lt.zhonguo6118.cn

[T50] Perl：逐行读文件
来源：https://al.zhonguo7118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://bc.zhonguo1118.cn

while (my $line = <$fh>) { print $line; }
来源：https://yv.zhonguo4118.cn

[T51] Scala：Hello World
来源：https://pr.zhonguo7118.cn

println("Hello")
来源：https://hd.zhonguo1118.cn

[T52] Scala：变量
来源：https://nb.zhonguo3118.cn

val a = 1;  var b = 2
来源：https://mw.zhonguo3118.cn

[T53] Scala：字符串插值
来源：https://ne.zhonguo1118.cn

s"值: $b"
来源：https://ai.zhonguo4118.cn

[T54] Scala：集合映射
来源：https://wg.zhonguo5118.cn

List(1, 2, 3).map(_ * 2)
来源：https://ew.zhonguo7118.cn

[T55] Scala：集合过滤
来源：https://dv.zhonguo5118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://rv.zhonguo7118.cn

[T56] Scala：样例类
来源：https://ya.zhonguo2118.cn

case class User(name: String, age: Int)
来源：https://nc.zhonguo5118.cn

[T57] Scala：模式匹配
来源：https://ql.zhonguo7118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://lg.zhonguo1118.cn

[T58] Scala：函数定义
来源：https://qj.zhonguo5118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://ie.zhonguo8118.cn

[T59] Scala：循环
来源：https://wm.zhonguo8118.cn

for (i <- 1 to 10) println(i)
来源：https://oy.zhonguo3118.cn

[T60] Scala：折叠
来源：https://oh.zhonguo3118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://tr.zhonguo2118.cn

================================================================================
来源：https://wr.zhonguo4118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://vv.zhonguo4118.cn

================================================================================
来源：https://rj.zhonguo7118.cn

[U01] Py：创建虚拟环境
来源：https://lz.zhonguo1118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://sp.zhonguo5118.cn

[U02] Py：导出 / 安装依赖
来源：https://vr.zhonguo1118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://gr.zhonguo1118.cn

[U03] Py：加载 .env 配置
来源：https://ho.zhonguo2118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://vx.zhonguo2118.cn

[U04] Py：变量调试打印
来源：https://im.zhonguo3118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://gl.zhonguo3118.cn

[U05] Py：列表去重且保序
来源：https://cx.zhonguo5118.cn

list(dict.fromkeys(arr))
来源：https://gs.zhonguo6118.cn

[U06] Py：合并两个字典
来源：https://ti.zhonguo5118.cn

{**a, **b}
来源：https://ua.zhonguo3118.cn

[U07] Py：反转字典键值
来源：https://js.zhonguo8118.cn

{v: k for k, v in d.items()}
来源：https://yp.zhonguo6118.cn

[U08] Py：展平二维列表
来源：https://nh.zhonguo2118.cn

[y for x in nested for y in x]
来源：https://fz.zhonguo6118.cn

[U09] Py：字典取最大值的键
来源：https://il.zhonguo1118.cn

max(d, key=d.get)
来源：https://up.zhonguo4118.cn

[U10] Py：按值排序字典
来源：https://go.zhonguo2118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://fn.zhonguo8118.cn

[U11] Py：生成器表达式
来源：https://bg.zhonguo3118.cn

(x * 2 for x in arr)
来源：https://tm.zhonguo1118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://ud.zhonguo4118.cn

Counter(arr).most_common(3)
来源：https://gj.zhonguo7118.cn

[U13] Py：固定长度队列
来源：https://vy.zhonguo2118.cn

deque(maxlen=10)
来源：https://yx.zhonguo4118.cn

[U14] Py：分组收集到列表
来源：https://kv.zhonguo6118.cn

defaultdict(list)
来源：https://ag.zhonguo2118.cn

[U15] Py：高精度计时
来源：https://dr.zhonguo3118.cn

t = time.perf_counter()
来源：https://ku.zhonguo2118.cn

[U16] Py：命令行参数解析
来源：https://qs.zhonguo5118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://cg.zhonguo3118.cn

[U17] Py：初始化日志
来源：https://qw.zhonguo1118.cn

logging.basicConfig(level=logging.INFO)
来源：https://ps.zhonguo1118.cn

[U18] Py：预编译正则
来源：https://ht.zhonguo2118.cn

pat = re.compile(r"\d+")
来源：https://yu.zhonguo7118.cn

[U19] Py：正则替换带回调
来源：https://yg.zhonguo2118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://cw.zhonguo7118.cn

[U20] Py：缓存函数结果
来源：https://ee.zhonguo6118.cn

@functools.lru_cache(maxsize=None)
来源：https://jv.zhonguo3118.cn

[U21] Py：自定义上下文管理器
来源：https://jk.zhonguo2118.cn

@contextlib.contextmanager
来源：https://ng.zhonguo6118.cn

[U22] Py：矩阵转置
来源：https://pj.zhonguo5118.cn

list(zip(*m))
来源：https://ia.zhonguo5118.cn

[U23] Py：分块读取大文件
来源：https://cd.zhonguo3118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://eb.zhonguo5118.cn

[U24] Py：路径操作
来源：https://fv.zhonguo8118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://ha.zhonguo3118.cn

[U25] Py：CSV 按字典读
来源：https://wo.zhonguo4118.cn

csv.DictReader(f)
来源：https://kc.zhonguo4118.cn

[U26] Py：并发下载
来源：https://ui.zhonguo4118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://jk.zhonguo5118.cn

[U27] Py：异步 HTTP
来源：https://ew.zhonguo2118.cn

aiohttp.ClientSession() 配合 async with
来源：https://kh.zhonguo8118.cn

[U28] Py：类型别名
来源：https://lv.zhonguo3118.cn

UserId = int
来源：https://ym.zhonguo7118.cn

[U29] Py：属性校验
来源：https://qf.zhonguo6118.cn

@property 与 @x.setter 配合
来源：https://sj.zhonguo6118.cn

[U30] Py：数据类
来源：https://yr.zhonguo6118.cn

@dataclass(slots=True)
来源：https://ha.zhonguo5118.cn

[U31] Py：单测
来源：https://ro.zhonguo6118.cn

python -m pytest -q
来源：https://vz.zhonguo2118.cn

[U32] Py：代码格式化
来源：https://jo.zhonguo2118.cn

ruff format . && ruff check --fix .
来源：https://cu.zhonguo4118.cn

[U33] Py：打包发布
来源：https://rg.zhonguo8118.cn

python -m build  （依赖 pyproject.toml）
来源：https://hj.zhonguo8118.cn

[U34] Py：判断编码
来源：https://jd.zhonguo4118.cn

chardet.detect(raw)
来源：https://lj.zhonguo8118.cn

[U35] Py：发送邮件
来源：https://gs.zhonguo6118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://be.zhonguo8118.cn

[U36] Py：定时任务
来源：https://eg.zhonguo1118.cn

schedule.every(10).minutes.do(job)
来源：https://rn.zhonguo6118.cn

[U37] Py：读写 Excel
来源：https://pp.zhonguo6118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://zd.zhonguo4118.cn

[U38] Py：获取脚本所在目录
来源：https://ic.zhonguo1118.cn

Path(__file__).resolve().parent
来源：https://go.zhonguo1118.cn

[U39] Py：判断是否在交互环境
来源：https://vx.zhonguo1118.cn

sys.stdout.isatty()
来源：https://po.zhonguo7118.cn

[U40] Py：打印到标准错误
来源：https://ay.zhonguo4118.cn

print("err", file=sys.stderr)
来源：https://bx.zhonguo7118.cn

[U41] PHP：初始化 Composer 项目
来源：https://sb.zhonguo2118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://wd.zhonguo3118.cn

[U42] PHP：PSR-4 自动加载
来源：https://ho.zhonguo3118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://rd.zhonguo1118.cn

[U43] PHP：声明命名空间
来源：https://rh.zhonguo7118.cn

namespace App\Http;
来源：https://oo.zhonguo8118.cn

[U44] PHP：开启严格类型
来源：https://nj.zhonguo3118.cn

declare(strict_types=1);
来源：https://rh.zhonguo2118.cn

[U45] PHP：类型声明与返回类型
来源：https://jx.zhonguo7118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://iz.zhonguo1118.cn

[U46] PHP：可空类型
来源：https://cc.zhonguo8118.cn

?string $name = null
来源：https://pf.zhonguo6118.cn

[U47] PHP：联合类型
来源：https://kw.zhonguo8118.cn

int|string $id
来源：https://uv.zhonguo6118.cn

[U48] PHP：纯枚举
来源：https://je.zhonguo5118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://mj.zhonguo4118.cn

[U49] PHP：只读属性
来源：https://qw.zhonguo8118.cn

public readonly string $name
来源：https://jc.zhonguo8118.cn

[U50] PHP：构造器属性提升
来源：https://ma.zhonguo6118.cn

public function __construct(private int $id) {}
来源：https://mf.zhonguo4118.cn

[U51] PHP：数组解构
来源：https://te.zhonguo8118.cn

[$a, $b] = $arr;
来源：https://lh.zhonguo8118.cn

[U52] PHP：箭头函数
来源：https://nj.zhonguo6118.cn

$double = fn($x) => $x * 2;
来源：https://nc.zhonguo7118.cn

[U53] PHP：空合并运算符
来源：https://rs.zhonguo6118.cn

$v = $a ?? $b ?? "default";
来源：https://kf.zhonguo7118.cn

[U54] PHP：空安全调用
来源：https://ez.zhonguo5118.cn

$obj?->method()
来源：https://lv.zhonguo7118.cn

[U55] PHP：match 表达式
来源：https://dp.zhonguo2118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://hp.zhonguo1118.cn

[U56] PHP：命名参数
来源：https://ur.zhonguo7118.cn

f(a: 1, b: 2)
来源：https://uc.zhonguo1118.cn

[U57] PHP：字符串插值
来源：https://gk.zhonguo1118.cn

"值: {$a}"
来源：https://dw.zhonguo5118.cn

[U58] PHP：数组三件套
来源：https://ok.zhonguo8118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://es.zhonguo2118.cn

[U59] PHP：自定义排序
来源：https://yw.zhonguo5118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://ix.zhonguo5118.cn

[U60] PHP：JSON 编解码
来源：https://vc.zhonguo1118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://sc.zhonguo2118.cn

[U61] PHP：正则
来源：https://df.zhonguo5118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://fc.zhonguo6118.cn

[U62] PHP：日期对象
来源：https://aq.zhonguo4118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://wy.zhonguo4118.cn

[U63] PHP：文件读写
来源：https://aj.zhonguo5118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://uv.zhonguo3118.cn

[U64] PHP：目录遍历
来源：https://ri.zhonguo6118.cn

glob("dir/*.php");  scandir("dir");
来源：https://cf.zhonguo4118.cn

[U65] PHP：会话
来源：https://qz.zhonguo1118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://cu.zhonguo7118.cn

[U66] PHP：设置 Cookie
来源：https://nt.zhonguo2118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://mv.zhonguo1118.cn

[U67] PHP：处理文件上传
来源：https://hs.zhonguo7118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://nr.zhonguo4118.cn

[U68] PHP：PDO 连接
来源：https://ic.zhonguo6118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://xx.zhonguo7118.cn

[U69] PHP：PDO 预处理
来源：https://ok.zhonguo4118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://zn.zhonguo5118.cn

[U70] PHP：PDO 事务
来源：https://fa.zhonguo1118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://tr.zhonguo2118.cn

[U71] PHP：抛出异常
来源：https://bw.zhonguo8118.cn

throw new RuntimeException("失败", 500);
来源：https://zd.zhonguo5118.cn

[U72] PHP：写错误日志
来源：https://cg.zhonguo2118.cn

error_log("失败: " . $e->getMessage());
来源：https://wo.zhonguo7118.cn

[U73] PHP：读取 ini 配置
来源：https://sa.zhonguo2118.cn

parse_ini_file("config.ini", true)
来源：https://dr.zhonguo6118.cn

[U74] PHP：读取环境变量
来源：https://oq.zhonguo2118.cn

getenv("APP_ENV") ?: "production"
来源：https://hy.zhonguo1118.cn

[U75] PHP：依赖注入
来源：https://vm.zhonguo5118.cn

composer require psr/container
来源：https://kh.zhonguo1118.cn

[U76] PHP：简单路由
来源：https://fj.zhonguo6118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://ai.zhonguo1118.cn

[U77] PHP：模板渲染
来源：https://la.zhonguo2118.cn

composer require twig/twig
来源：https://fp.zhonguo2118.cn

[U78] PHP：单元测试
来源：https://sf.zhonguo5118.cn

composer require --dev phpunit/phpunit
来源：https://ts.zhonguo2118.cn

[U79] PHP：静态分析
来源：https://zj.zhonguo4118.cn

composer require --dev phpstan/phpstan
来源：https://ys.zhonguo3118.cn

[U80] PHP：代码规范修复
来源：https://cf.zhonguo8118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://nh.zhonguo3118.cn

[U81] JS：初始化项目
来源：https://eo.zhonguo4118.cn

npm init -y;  npm i express
来源：https://uh.zhonguo6118.cn

[U82] JS：package.json 脚本
来源：https://tq.zhonguo6118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://eb.zhonguo8118.cn

[U83] JS：ES Module 导入导出
来源：https://mg.zhonguo1118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://hn.zhonguo7118.cn

[U84] JS：CommonJS 写法
来源：https://nm.zhonguo2118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://ub.zhonguo5118.cn


<!-- 参考信息 -->