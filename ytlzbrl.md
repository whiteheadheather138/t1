代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://xi.zhonguo6118.cn

[S57] C++：编译期常量
来源：https://zg.zhonguo1118.cn

constexpr int N = 10;
来源：https://ut.zhonguo3118.cn

[S58] C++：命名空间
来源：https://ay.zhonguo2118.cn

namespace ns { int f() { return 1; } }
来源：https://fr.zhonguo5118.cn

[S59] C++：静态断言
来源：https://pn.zhonguo2118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://we.zhonguo6118.cn

[S60] C++：遍历并删除元素
来源：https://zc.zhonguo3118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://me.zhonguo6118.cn

================================================================================
来源：https://zh.zhonguo3118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://fi.zhonguo7118.cn

================================================================================
来源：https://nu.zhonguo8118.cn

[T01] Kotlin：Hello World
来源：https://fu.zhonguo2118.cn

println("Hello")
来源：https://pn.zhonguo7118.cn

[T02] Kotlin：变量
来源：https://oh.zhonguo2118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://vg.zhonguo1118.cn

[T03] Kotlin：字符串模板
来源：https://gp.zhonguo1118.cn

"值: $b"
来源：https://as.zhonguo4118.cn

[T04] Kotlin：空安全
来源：https://cc.zhonguo3118.cn

val n: String? = null;  n?.length
来源：https://fo.zhonguo6118.cn

[T05] Kotlin：when 表达式
来源：https://id.zhonguo8118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://ll.zhonguo4118.cn

[T06] Kotlin：集合映射
来源：https://bl.zhonguo4118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://js.zhonguo3118.cn

[T07] Kotlin：集合过滤
来源：https://nl.zhonguo7118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://ea.zhonguo4118.cn

[T08] Kotlin：数据类
来源：https://yr.zhonguo3118.cn

data class User(val name: String, val age: Int)
来源：https://gu.zhonguo6118.cn

[T09] Kotlin：扩展函数
来源：https://cp.zhonguo5118.cn

fun String.exclaim() = this + "!"
来源：https://nm.zhonguo4118.cn

[T10] Kotlin：默认参数
来源：https://ve.zhonguo1118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://wn.zhonguo1118.cn

[T11] Kotlin：协程
来源：https://yw.zhonguo3118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://um.zhonguo4118.cn

[T12] Kotlin：解构声明
来源：https://dd.zhonguo6118.cn

val (a, b) = Pair(1, 2)
来源：https://vt.zhonguo2118.cn

[T13] Kotlin：只读 Map
来源：https://lu.zhonguo4118.cn

val m = mapOf("a" to 1)
来源：https://sc.zhonguo5118.cn

[T14] Kotlin：循环
来源：https://gb.zhonguo7118.cn

for (i in 1..10) println(i)
来源：https://ut.zhonguo2118.cn

[T15] Kotlin：接口
来源：https://il.zhonguo6118.cn

interface Shape { fun area(): Double }
来源：https://zz.zhonguo5118.cn

[T16] Swift：Hello World
来源：https://jd.zhonguo4118.cn

print("Hello")
来源：https://fw.zhonguo8118.cn

[T17] Swift：变量与常量
来源：https://ua.zhonguo4118.cn

var a = 1;  let b = 2
来源：https://og.zhonguo3118.cn

[T18] Swift：字符串插值
来源：https://iv.zhonguo3118.cn

"值: \(b)"
来源：https://jq.zhonguo5118.cn

[T19] Swift：可选绑定
来源：https://mb.zhonguo6118.cn

if let n = opt { print(n) }
来源：https://pm.zhonguo8118.cn

[T20] Swift：数组操作
来源：https://ng.zhonguo3118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://oi.zhonguo1118.cn

[T21] Swift：遍历
来源：https://ou.zhonguo6118.cn

for x in a { print(x) }
来源：https://fc.zhonguo4118.cn

[T22] Swift：字典
来源：https://tj.zhonguo4118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://se.zhonguo7118.cn

[T23] Swift：函数
来源：https://md.zhonguo4118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://yi.zhonguo5118.cn

[T24] Swift：闭包
来源：https://ai.zhonguo3118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://rv.zhonguo8118.cn

[T25] Swift：结构体
来源：https://jb.zhonguo2118.cn

struct P { var x: Int }
来源：https://td.zhonguo4118.cn

[T26] Swift：类与重写
来源：https://wd.zhonguo8118.cn

class A: Base { override func f() {} }
来源：https://oh.zhonguo6118.cn

[T27] Swift：错误处理
来源：https://zh.zhonguo2118.cn

do { try f() } catch { print(error) }
来源：https://eg.zhonguo8118.cn

[T28] Swift：枚举
来源：https://yh.zhonguo1118.cn

enum Color { case red, green }
来源：https://af.zhonguo2118.cn

[T29] Swift：guard 提前返回
来源：https://rr.zhonguo4118.cn

guard let x = opt else { return }
来源：https://fx.zhonguo6118.cn

[T30] Swift：协议
来源：https://jc.zhonguo7118.cn

protocol Shape { func area() -> Double }
来源：https://fh.zhonguo4118.cn

[T31] Lua：Hello World
来源：https://dl.zhonguo1118.cn

print("Hello")
来源：https://ri.zhonguo4118.cn

[T32] Lua：局部变量
来源：https://hm.zhonguo8118.cn

local a = 1
来源：https://kr.zhonguo3118.cn

[T33] Lua：表（数组）
来源：https://nw.zhonguo4118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://lr.zhonguo6118.cn

[T34] Lua：遍历表
来源：https://jm.zhonguo3118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://qi.zhonguo1118.cn

[T35] Lua：字典表
来源：https://ms.zhonguo8118.cn

local d = { a = 1 };  d.b = 2
来源：https://in.zhonguo5118.cn

[T36] Lua：函数
来源：https://mh.zhonguo6118.cn

function add(a, b) return a + b end
来源：https://xk.zhonguo7118.cn

[T37] Lua：字符串拼接
来源：https://pr.zhonguo1118.cn

"a" .. "b"
来源：https://fu.zhonguo5118.cn

[T38] Lua：条件
来源：https://xw.zhonguo5118.cn

if x > 0 then print("正") end
来源：https://wp.zhonguo6118.cn

[T39] Lua：模式匹配
来源：https://ez.zhonguo5118.cn

string.find(s, "%d+")
来源：https://bi.zhonguo4118.cn

[T40] Lua：元表
来源：https://or.zhonguo8118.cn

setmetatable({}, { __index = base })
来源：https://nh.zhonguo2118.cn

[T41] Perl：Hello World
来源：https://xi.zhonguo7118.cn

print "Hello\n";
来源：https://ks.zhonguo3118.cn

[T42] Perl：变量类型
来源：https://ty.zhonguo3118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://bk.zhonguo4118.cn

[T43] Perl：字符串插值
来源：https://fx.zhonguo1118.cn

"值: $a"
来源：https://by.zhonguo7118.cn

[T44] Perl：条件
来源：https://ty.zhonguo4118.cn

if ($a > 0) { print "正"; }
来源：https://ov.zhonguo6118.cn

[T45] Perl：数组遍历
来源：https://yg.zhonguo3118.cn

for my $x (@arr) { print $x; }
来源：https://eb.zhonguo4118.cn

[T46] Perl：哈希操作
来源：https://ej.zhonguo2118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://iy.zhonguo6118.cn

[T47] Perl：正则捕获
来源：https://bz.zhonguo4118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://yi.zhonguo2118.cn

[T48] Perl：正则替换
来源：https://rn.zhonguo8118.cn

$s =~ s/old/new/g;
来源：https://xx.zhonguo7118.cn

[T49] Perl：函数
来源：https://kn.zhonguo4118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://yj.zhonguo7118.cn

[T50] Perl：逐行读文件
来源：https://ct.zhonguo6118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://vq.zhonguo7118.cn

while (my $line = <$fh>) { print $line; }
来源：https://dq.zhonguo8118.cn

[T51] Scala：Hello World
来源：https://ja.zhonguo3118.cn

println("Hello")
来源：https://fm.zhonguo5118.cn

[T52] Scala：变量
来源：https://wy.zhonguo3118.cn

val a = 1;  var b = 2
来源：https://tk.zhonguo5118.cn

[T53] Scala：字符串插值
来源：https://th.zhonguo3118.cn

s"值: $b"
来源：https://lo.zhonguo5118.cn

[T54] Scala：集合映射
来源：https://od.zhonguo3118.cn

List(1, 2, 3).map(_ * 2)
来源：https://eq.zhonguo1118.cn

[T55] Scala：集合过滤
来源：https://ed.zhonguo5118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://rq.zhonguo5118.cn

[T56] Scala：样例类
来源：https://mz.zhonguo3118.cn

case class User(name: String, age: Int)
来源：https://xe.zhonguo6118.cn

[T57] Scala：模式匹配
来源：https://uu.zhonguo3118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://is.zhonguo3118.cn

[T58] Scala：函数定义
来源：https://jo.zhonguo5118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://iu.zhonguo5118.cn

[T59] Scala：循环
来源：https://ym.zhonguo6118.cn

for (i <- 1 to 10) println(i)
来源：https://va.zhonguo3118.cn

[T60] Scala：折叠
来源：https://gm.zhonguo7118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://bm.zhonguo5118.cn

================================================================================
来源：https://rg.zhonguo3118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://ht.zhonguo4118.cn

================================================================================
来源：https://gq.zhonguo7118.cn

[U01] Py：创建虚拟环境
来源：https://yy.zhonguo2118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://uu.zhonguo3118.cn

[U02] Py：导出 / 安装依赖
来源：https://xr.zhonguo6118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://cb.zhonguo6118.cn

[U03] Py：加载 .env 配置
来源：https://wj.zhonguo3118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://dl.zhonguo8118.cn

[U04] Py：变量调试打印
来源：https://xy.zhonguo1118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://gq.zhonguo6118.cn

[U05] Py：列表去重且保序
来源：https://ry.zhonguo6118.cn

list(dict.fromkeys(arr))
来源：https://pc.zhonguo6118.cn

[U06] Py：合并两个字典
来源：https://im.zhonguo8118.cn

{**a, **b}
来源：https://ub.zhonguo7118.cn

[U07] Py：反转字典键值
来源：https://wt.zhonguo2118.cn

{v: k for k, v in d.items()}
来源：https://mg.zhonguo5118.cn

[U08] Py：展平二维列表
来源：https://aa.zhonguo7118.cn

[y for x in nested for y in x]
来源：https://oa.zhonguo3118.cn

[U09] Py：字典取最大值的键
来源：https://sj.zhonguo3118.cn

max(d, key=d.get)
来源：https://yd.zhonguo7118.cn

[U10] Py：按值排序字典
来源：https://hf.zhonguo7118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://sx.zhonguo4118.cn

[U11] Py：生成器表达式
来源：https://ro.zhonguo6118.cn

(x * 2 for x in arr)
来源：https://ac.zhonguo7118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://uh.zhonguo1118.cn

Counter(arr).most_common(3)
来源：https://gk.zhonguo1118.cn

[U13] Py：固定长度队列
来源：https://nz.zhonguo2118.cn

deque(maxlen=10)
来源：https://yj.zhonguo5118.cn

[U14] Py：分组收集到列表
来源：https://zu.zhonguo4118.cn

defaultdict(list)
来源：https://te.zhonguo2118.cn

[U15] Py：高精度计时
来源：https://lh.zhonguo6118.cn

t = time.perf_counter()
来源：https://ix.zhonguo8118.cn

[U16] Py：命令行参数解析
来源：https://dm.zhonguo6118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://pe.zhonguo5118.cn

[U17] Py：初始化日志
来源：https://ep.zhonguo3118.cn

logging.basicConfig(level=logging.INFO)
来源：https://nc.zhonguo6118.cn

[U18] Py：预编译正则
来源：https://ma.zhonguo2118.cn

pat = re.compile(r"\d+")
来源：https://lu.zhonguo3118.cn

[U19] Py：正则替换带回调
来源：https://ra.zhonguo1118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://fo.zhonguo2118.cn

[U20] Py：缓存函数结果
来源：https://ke.zhonguo8118.cn

@functools.lru_cache(maxsize=None)
来源：https://cn.zhonguo8118.cn

[U21] Py：自定义上下文管理器
来源：https://id.zhonguo3118.cn

@contextlib.contextmanager
来源：https://yp.zhonguo3118.cn

[U22] Py：矩阵转置
来源：https://gh.zhonguo7118.cn

list(zip(*m))
来源：https://aq.zhonguo3118.cn

[U23] Py：分块读取大文件
来源：https://tu.zhonguo4118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://tb.zhonguo8118.cn

[U24] Py：路径操作
来源：https://xb.zhonguo7118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://pf.zhonguo4118.cn

[U25] Py：CSV 按字典读
来源：https://oq.zhonguo2118.cn

csv.DictReader(f)
来源：https://xg.zhonguo8118.cn

[U26] Py：并发下载
来源：https://im.zhonguo2118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://oy.zhonguo7118.cn

[U27] Py：异步 HTTP
来源：https://be.zhonguo6118.cn

aiohttp.ClientSession() 配合 async with
来源：https://nq.zhonguo6118.cn

[U28] Py：类型别名
来源：https://kx.zhonguo8118.cn

UserId = int
来源：https://lg.zhonguo6118.cn

[U29] Py：属性校验
来源：https://zi.zhonguo6118.cn

@property 与 @x.setter 配合
来源：https://vl.zhonguo3118.cn

[U30] Py：数据类
来源：https://hj.zhonguo2118.cn

@dataclass(slots=True)
来源：https://le.zhonguo8118.cn

[U31] Py：单测
来源：https://ge.zhonguo3118.cn

python -m pytest -q
来源：https://ca.zhonguo6118.cn

[U32] Py：代码格式化
来源：https://fi.zhonguo7118.cn

ruff format . && ruff check --fix .
来源：https://fe.zhonguo5118.cn

[U33] Py：打包发布
来源：https://mp.zhonguo4118.cn

python -m build  （依赖 pyproject.toml）
来源：https://qu.zhonguo2118.cn

[U34] Py：判断编码
来源：https://go.zhonguo4118.cn

chardet.detect(raw)
来源：https://nk.zhonguo5118.cn

[U35] Py：发送邮件
来源：https://ig.zhonguo2118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://sf.zhonguo1118.cn

[U36] Py：定时任务
来源：https://sg.zhonguo5118.cn

schedule.every(10).minutes.do(job)
来源：https://cr.zhonguo3118.cn

[U37] Py：读写 Excel
来源：https://vc.zhonguo8118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://jx.zhonguo1118.cn

[U38] Py：获取脚本所在目录
来源：https://cy.zhonguo4118.cn

Path(__file__).resolve().parent
来源：https://gh.zhonguo6118.cn

[U39] Py：判断是否在交互环境
来源：https://li.zhonguo1118.cn

sys.stdout.isatty()
来源：https://wm.zhonguo2118.cn

[U40] Py：打印到标准错误
来源：https://iq.zhonguo8118.cn

print("err", file=sys.stderr)
来源：https://hw.zhonguo5118.cn

[U41] PHP：初始化 Composer 项目
来源：https://qf.zhonguo7118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://pz.zhonguo5118.cn

[U42] PHP：PSR-4 自动加载
来源：https://td.zhonguo2118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://ra.zhonguo1118.cn

[U43] PHP：声明命名空间
来源：https://vv.zhonguo4118.cn

namespace App\Http;
来源：https://sb.zhonguo4118.cn

[U44] PHP：开启严格类型
来源：https://zv.zhonguo2118.cn

declare(strict_types=1);
来源：https://tv.zhonguo1118.cn

[U45] PHP：类型声明与返回类型
来源：https://ai.zhonguo2118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://ni.zhonguo1118.cn

[U46] PHP：可空类型
来源：https://eq.zhonguo8118.cn

?string $name = null
来源：https://lc.zhonguo8118.cn

[U47] PHP：联合类型
来源：https://ga.zhonguo1118.cn

int|string $id
来源：https://mh.zhonguo6118.cn

[U48] PHP：纯枚举
来源：https://mx.zhonguo8118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://qw.zhonguo7118.cn

[U49] PHP：只读属性
来源：https://lh.zhonguo3118.cn

public readonly string $name
来源：https://yv.zhonguo3118.cn

[U50] PHP：构造器属性提升
来源：https://wi.zhonguo7118.cn

public function __construct(private int $id) {}
来源：https://ye.zhonguo4118.cn

[U51] PHP：数组解构
来源：https://at.zhonguo7118.cn

[$a, $b] = $arr;
来源：https://kh.zhonguo6118.cn

[U52] PHP：箭头函数
来源：https://fw.zhonguo3118.cn

$double = fn($x) => $x * 2;
来源：https://tm.zhonguo3118.cn

[U53] PHP：空合并运算符
来源：https://dy.zhonguo4118.cn

$v = $a ?? $b ?? "default";
来源：https://em.zhonguo6118.cn

[U54] PHP：空安全调用
来源：https://er.zhonguo1118.cn

$obj?->method()
来源：https://sk.zhonguo2118.cn

[U55] PHP：match 表达式
来源：https://ic.zhonguo3118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://eg.zhonguo6118.cn

[U56] PHP：命名参数
来源：https://cm.zhonguo1118.cn

f(a: 1, b: 2)
来源：https://jg.zhonguo5118.cn

[U57] PHP：字符串插值
来源：https://zv.zhonguo4118.cn

"值: {$a}"
来源：https://gx.zhonguo7118.cn

[U58] PHP：数组三件套
来源：https://cf.zhonguo3118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://wd.zhonguo5118.cn

[U59] PHP：自定义排序
来源：https://qb.zhonguo2118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://ce.zhonguo6118.cn

[U60] PHP：JSON 编解码
来源：https://nh.zhonguo7118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://it.zhonguo5118.cn

[U61] PHP：正则
来源：https://vi.zhonguo3118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://ke.zhonguo1118.cn

[U62] PHP：日期对象
来源：https://sy.zhonguo8118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://nj.zhonguo6118.cn

[U63] PHP：文件读写
来源：https://lw.zhonguo8118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://fj.zhonguo8118.cn

[U64] PHP：目录遍历
来源：https://nm.zhonguo8118.cn

glob("dir/*.php");  scandir("dir");
来源：https://so.zhonguo5118.cn

[U65] PHP：会话
来源：https://qt.zhonguo3118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://tr.zhonguo1118.cn

[U66] PHP：设置 Cookie
来源：https://mz.zhonguo8118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://wp.zhonguo5118.cn

[U67] PHP：处理文件上传
来源：https://zz.zhonguo2118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://ly.zhonguo4118.cn

[U68] PHP：PDO 连接
来源：https://ow.zhonguo6118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://jx.zhonguo8118.cn

[U69] PHP：PDO 预处理
来源：https://je.zhonguo2118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://eu.zhonguo7118.cn

[U70] PHP：PDO 事务
来源：https://pt.zhonguo3118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://yx.zhonguo3118.cn

[U71] PHP：抛出异常
来源：https://mt.zhonguo2118.cn

throw new RuntimeException("失败", 500);
来源：https://os.zhonguo4118.cn

[U72] PHP：写错误日志
来源：https://bb.zhonguo8118.cn

error_log("失败: " . $e->getMessage());
来源：https://lc.zhonguo6118.cn

[U73] PHP：读取 ini 配置
来源：https://rs.zhonguo8118.cn

parse_ini_file("config.ini", true)
来源：https://vg.zhonguo5118.cn

[U74] PHP：读取环境变量
来源：https://gb.zhonguo4118.cn

getenv("APP_ENV") ?: "production"
来源：https://ha.zhonguo3118.cn

[U75] PHP：依赖注入
来源：https://wk.zhonguo6118.cn

composer require psr/container
来源：https://vk.zhonguo2118.cn

[U76] PHP：简单路由
来源：https://kr.zhonguo1118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://nl.zhonguo1118.cn

[U77] PHP：模板渲染
来源：https://ov.zhonguo5118.cn

composer require twig/twig
来源：https://nf.zhonguo7118.cn

[U78] PHP：单元测试
来源：https://bd.zhonguo6118.cn

composer require --dev phpunit/phpunit
来源：https://tw.zhonguo6118.cn

[U79] PHP：静态分析
来源：https://rn.zhonguo7118.cn

composer require --dev phpstan/phpstan
来源：https://xn.zhonguo8118.cn

[U80] PHP：代码规范修复
来源：https://zy.zhonguo8118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://ep.zhonguo4118.cn

[U81] JS：初始化项目
来源：https://pi.zhonguo6118.cn

npm init -y;  npm i express
来源：https://za.zhonguo7118.cn

[U82] JS：package.json 脚本
来源：https://bi.zhonguo1118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://nc.zhonguo5118.cn


<!-- 参考信息 -->