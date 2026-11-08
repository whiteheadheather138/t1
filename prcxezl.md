代发 wailian999

namespace ns { int f() { return 1; } }
来源：https://ts.zhonguo8118.cn

[S59] C++：静态断言
来源：https://aa.zhonguo8118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://uw.zhonguo3118.cn

[S60] C++：遍历并删除元素
来源：https://pt.zhonguo4118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://vp.zhonguo8118.cn

================================================================================
来源：https://ao.zhonguo3118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://pj.zhonguo5118.cn

================================================================================
来源：https://bv.zhonguo6118.cn

[T01] Kotlin：Hello World
来源：https://nf.zhonguo6118.cn

println("Hello")
来源：https://ld.zhonguo7118.cn

[T02] Kotlin：变量
来源：https://er.zhonguo3118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://dg.zhonguo3118.cn

[T03] Kotlin：字符串模板
来源：https://dq.zhonguo6118.cn

"值: $b"
来源：https://ui.zhonguo8118.cn

[T04] Kotlin：空安全
来源：https://gi.zhonguo1118.cn

val n: String? = null;  n?.length
来源：https://yb.zhonguo3118.cn

[T05] Kotlin：when 表达式
来源：https://or.zhonguo2118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://wa.zhonguo4118.cn

[T06] Kotlin：集合映射
来源：https://pg.zhonguo4118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://gb.zhonguo7118.cn

[T07] Kotlin：集合过滤
来源：https://bs.zhonguo6118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://rt.zhonguo6118.cn

[T08] Kotlin：数据类
来源：https://vy.zhonguo6118.cn

data class User(val name: String, val age: Int)
来源：https://ef.zhonguo4118.cn

[T09] Kotlin：扩展函数
来源：https://pb.zhonguo5118.cn

fun String.exclaim() = this + "!"
来源：https://bt.zhonguo7118.cn

[T10] Kotlin：默认参数
来源：https://jj.zhonguo6118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://mn.zhonguo7118.cn

[T11] Kotlin：协程
来源：https://op.zhonguo1118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://ki.zhonguo8118.cn

[T12] Kotlin：解构声明
来源：https://wm.zhonguo6118.cn

val (a, b) = Pair(1, 2)
来源：https://ge.zhonguo3118.cn

[T13] Kotlin：只读 Map
来源：https://ns.zhonguo3118.cn

val m = mapOf("a" to 1)
来源：https://se.zhonguo8118.cn

[T14] Kotlin：循环
来源：https://oj.zhonguo3118.cn

for (i in 1..10) println(i)
来源：https://ir.zhonguo5118.cn

[T15] Kotlin：接口
来源：https://nv.zhonguo7118.cn

interface Shape { fun area(): Double }
来源：https://du.zhonguo3118.cn

[T16] Swift：Hello World
来源：https://di.zhonguo6118.cn

print("Hello")
来源：https://xz.zhonguo4118.cn

[T17] Swift：变量与常量
来源：https://sf.zhonguo6118.cn

var a = 1;  let b = 2
来源：https://jr.zhonguo7118.cn

[T18] Swift：字符串插值
来源：https://jz.zhonguo2118.cn

"值: \(b)"
来源：https://lm.zhonguo6118.cn

[T19] Swift：可选绑定
来源：https://uc.zhonguo4118.cn

if let n = opt { print(n) }
来源：https://xr.zhonguo4118.cn

[T20] Swift：数组操作
来源：https://ir.zhonguo4118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://jd.zhonguo1118.cn

[T21] Swift：遍历
来源：https://iy.zhonguo5118.cn

for x in a { print(x) }
来源：https://nz.zhonguo5118.cn

[T22] Swift：字典
来源：https://kc.zhonguo1118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://jj.zhonguo1118.cn

[T23] Swift：函数
来源：https://ws.zhonguo3118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://xz.zhonguo1118.cn

[T24] Swift：闭包
来源：https://rm.zhonguo8118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://lv.zhonguo4118.cn

[T25] Swift：结构体
来源：https://ed.zhonguo1118.cn

struct P { var x: Int }
来源：https://ut.zhonguo2118.cn

[T26] Swift：类与重写
来源：https://im.zhonguo1118.cn

class A: Base { override func f() {} }
来源：https://ie.zhonguo6118.cn

[T27] Swift：错误处理
来源：https://tp.zhonguo7118.cn

do { try f() } catch { print(error) }
来源：https://ep.zhonguo3118.cn

[T28] Swift：枚举
来源：https://ny.zhonguo1118.cn

enum Color { case red, green }
来源：https://jc.zhonguo2118.cn

[T29] Swift：guard 提前返回
来源：https://bk.zhonguo5118.cn

guard let x = opt else { return }
来源：https://qw.zhonguo8118.cn

[T30] Swift：协议
来源：https://ut.zhonguo7118.cn

protocol Shape { func area() -> Double }
来源：https://vq.zhonguo2118.cn

[T31] Lua：Hello World
来源：https://jk.zhonguo8118.cn

print("Hello")
来源：https://ka.zhonguo8118.cn

[T32] Lua：局部变量
来源：https://cc.zhonguo8118.cn

local a = 1
来源：https://dr.zhonguo2118.cn

[T33] Lua：表（数组）
来源：https://tb.zhonguo1118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://sr.zhonguo5118.cn

[T34] Lua：遍历表
来源：https://ri.zhonguo1118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://di.zhonguo6118.cn

[T35] Lua：字典表
来源：https://tk.zhonguo4118.cn

local d = { a = 1 };  d.b = 2
来源：https://qr.zhonguo4118.cn

[T36] Lua：函数
来源：https://hv.zhonguo2118.cn

function add(a, b) return a + b end
来源：https://sg.zhonguo8118.cn

[T37] Lua：字符串拼接
来源：https://qz.zhonguo1118.cn

"a" .. "b"
来源：https://mt.zhonguo3118.cn

[T38] Lua：条件
来源：https://ff.zhonguo1118.cn

if x > 0 then print("正") end
来源：https://gn.zhonguo3118.cn

[T39] Lua：模式匹配
来源：https://gy.zhonguo4118.cn

string.find(s, "%d+")
来源：https://jl.zhonguo8118.cn

[T40] Lua：元表
来源：https://xi.zhonguo7118.cn

setmetatable({}, { __index = base })
来源：https://bm.zhonguo5118.cn

[T41] Perl：Hello World
来源：https://xy.zhonguo3118.cn

print "Hello\n";
来源：https://tw.zhonguo2118.cn

[T42] Perl：变量类型
来源：https://tm.zhonguo4118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://cl.zhonguo8118.cn

[T43] Perl：字符串插值
来源：https://pf.zhonguo7118.cn

"值: $a"
来源：https://an.zhonguo1118.cn

[T44] Perl：条件
来源：https://tn.zhonguo5118.cn

if ($a > 0) { print "正"; }
来源：https://hy.zhonguo4118.cn

[T45] Perl：数组遍历
来源：https://dv.zhonguo7118.cn

for my $x (@arr) { print $x; }
来源：https://oj.zhonguo3118.cn

[T46] Perl：哈希操作
来源：https://tt.zhonguo3118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://ub.zhonguo6118.cn

[T47] Perl：正则捕获
来源：https://aq.zhonguo2118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://nk.zhonguo8118.cn

[T48] Perl：正则替换
来源：https://kz.zhonguo5118.cn

$s =~ s/old/new/g;
来源：https://te.zhonguo1118.cn

[T49] Perl：函数
来源：https://fd.zhonguo8118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://kn.zhonguo3118.cn

[T50] Perl：逐行读文件
来源：https://ct.zhonguo7118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://fr.zhonguo8118.cn

while (my $line = <$fh>) { print $line; }
来源：https://nu.zhonguo1118.cn

[T51] Scala：Hello World
来源：https://xr.zhonguo1118.cn

println("Hello")
来源：https://bu.zhonguo1118.cn

[T52] Scala：变量
来源：https://lc.zhonguo8118.cn

val a = 1;  var b = 2
来源：https://nk.zhonguo2118.cn

[T53] Scala：字符串插值
来源：https://ru.zhonguo3118.cn

s"值: $b"
来源：https://fv.zhonguo4118.cn

[T54] Scala：集合映射
来源：https://zq.zhonguo2118.cn

List(1, 2, 3).map(_ * 2)
来源：https://mn.zhonguo8118.cn

[T55] Scala：集合过滤
来源：https://fw.zhonguo7118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://ew.zhonguo7118.cn

[T56] Scala：样例类
来源：https://cx.zhonguo8118.cn

case class User(name: String, age: Int)
来源：https://ci.zhonguo3118.cn

[T57] Scala：模式匹配
来源：https://sz.zhonguo6118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://fd.zhonguo8118.cn

[T58] Scala：函数定义
来源：https://gl.zhonguo8118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://wy.zhonguo3118.cn

[T59] Scala：循环
来源：https://my.zhonguo1118.cn

for (i <- 1 to 10) println(i)
来源：https://cy.zhonguo3118.cn

[T60] Scala：折叠
来源：https://ek.zhonguo4118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://qv.zhonguo4118.cn

================================================================================
来源：https://bp.zhonguo2118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://uc.zhonguo6118.cn

================================================================================
来源：https://bi.zhonguo4118.cn

[U01] Py：创建虚拟环境
来源：https://lr.zhonguo3118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://em.zhonguo2118.cn

[U02] Py：导出 / 安装依赖
来源：https://kt.zhonguo1118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://dp.zhonguo3118.cn

[U03] Py：加载 .env 配置
来源：https://aj.zhonguo3118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://yf.zhonguo1118.cn

[U04] Py：变量调试打印
来源：https://wk.zhonguo6118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://jt.zhonguo5118.cn

[U05] Py：列表去重且保序
来源：https://qb.zhonguo7118.cn

list(dict.fromkeys(arr))
来源：https://il.zhonguo8118.cn

[U06] Py：合并两个字典
来源：https://fs.zhonguo1118.cn

{**a, **b}
来源：https://pe.zhonguo3118.cn

[U07] Py：反转字典键值
来源：https://sr.zhonguo8118.cn

{v: k for k, v in d.items()}
来源：https://jt.zhonguo7118.cn

[U08] Py：展平二维列表
来源：https://ih.zhonguo6118.cn

[y for x in nested for y in x]
来源：https://rf.zhonguo6118.cn

[U09] Py：字典取最大值的键
来源：https://xh.zhonguo8118.cn

max(d, key=d.get)
来源：https://yf.zhonguo1118.cn

[U10] Py：按值排序字典
来源：https://of.zhonguo2118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://qs.zhonguo6118.cn

[U11] Py：生成器表达式
来源：https://zq.zhonguo2118.cn

(x * 2 for x in arr)
来源：https://hr.zhonguo2118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://lc.zhonguo5118.cn

Counter(arr).most_common(3)
来源：https://fa.zhonguo4118.cn

[U13] Py：固定长度队列
来源：https://re.zhonguo1118.cn

deque(maxlen=10)
来源：https://ah.zhonguo3118.cn

[U14] Py：分组收集到列表
来源：https://yq.zhonguo1118.cn

defaultdict(list)
来源：https://ll.zhonguo2118.cn

[U15] Py：高精度计时
来源：https://xt.zhonguo1118.cn

t = time.perf_counter()
来源：https://ra.zhonguo7118.cn

[U16] Py：命令行参数解析
来源：https://dc.zhonguo3118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://ac.zhonguo8118.cn

[U17] Py：初始化日志
来源：https://bs.zhonguo4118.cn

logging.basicConfig(level=logging.INFO)
来源：https://cl.zhonguo2118.cn

[U18] Py：预编译正则
来源：https://sk.zhonguo3118.cn

pat = re.compile(r"\d+")
来源：https://oa.zhonguo3118.cn

[U19] Py：正则替换带回调
来源：https://rw.zhonguo2118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://tx.zhonguo4118.cn

[U20] Py：缓存函数结果
来源：https://yj.zhonguo3118.cn

@functools.lru_cache(maxsize=None)
来源：https://fn.zhonguo4118.cn

[U21] Py：自定义上下文管理器
来源：https://zg.zhonguo6118.cn

@contextlib.contextmanager
来源：https://dv.zhonguo6118.cn

[U22] Py：矩阵转置
来源：https://rq.zhonguo5118.cn

list(zip(*m))
来源：https://sg.zhonguo8118.cn

[U23] Py：分块读取大文件
来源：https://xa.zhonguo1118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://hn.zhonguo3118.cn

[U24] Py：路径操作
来源：https://ic.zhonguo5118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://gb.zhonguo2118.cn

[U25] Py：CSV 按字典读
来源：https://kk.zhonguo6118.cn

csv.DictReader(f)
来源：https://se.zhonguo2118.cn

[U26] Py：并发下载
来源：https://yk.zhonguo4118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://cw.zhonguo2118.cn

[U27] Py：异步 HTTP
来源：https://kl.zhonguo8118.cn

aiohttp.ClientSession() 配合 async with
来源：https://ip.zhonguo3118.cn

[U28] Py：类型别名
来源：https://zq.zhonguo8118.cn

UserId = int
来源：https://ik.zhonguo8118.cn

[U29] Py：属性校验
来源：https://ml.zhonguo5118.cn

@property 与 @x.setter 配合
来源：https://bb.zhonguo3118.cn

[U30] Py：数据类
来源：https://kg.zhonguo6118.cn

@dataclass(slots=True)
来源：https://hc.zhonguo1118.cn

[U31] Py：单测
来源：https://ai.zhonguo4118.cn

python -m pytest -q
来源：https://jg.zhonguo1118.cn

[U32] Py：代码格式化
来源：https://nf.zhonguo6118.cn

ruff format . && ruff check --fix .
来源：https://io.zhonguo2118.cn

[U33] Py：打包发布
来源：https://ck.zhonguo5118.cn

python -m build  （依赖 pyproject.toml）
来源：https://ac.zhonguo1118.cn

[U34] Py：判断编码
来源：https://vb.zhonguo6118.cn

chardet.detect(raw)
来源：https://om.zhonguo5118.cn

[U35] Py：发送邮件
来源：https://eh.zhonguo8118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://nv.zhonguo4118.cn

[U36] Py：定时任务
来源：https://rk.zhonguo5118.cn

schedule.every(10).minutes.do(job)
来源：https://hu.zhonguo4118.cn

[U37] Py：读写 Excel
来源：https://gk.zhonguo8118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://ec.zhonguo1118.cn

[U38] Py：获取脚本所在目录
来源：https://oe.zhonguo3118.cn

Path(__file__).resolve().parent
来源：https://bm.zhonguo8118.cn

[U39] Py：判断是否在交互环境
来源：https://qf.zhonguo3118.cn

sys.stdout.isatty()
来源：https://df.zhonguo6118.cn

[U40] Py：打印到标准错误
来源：https://hh.zhonguo5118.cn

print("err", file=sys.stderr)
来源：https://so.zhonguo8118.cn

[U41] PHP：初始化 Composer 项目
来源：https://wa.zhonguo8118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://wd.zhonguo6118.cn

[U42] PHP：PSR-4 自动加载
来源：https://ph.zhonguo2118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://lt.zhonguo3118.cn

[U43] PHP：声明命名空间
来源：https://yk.zhonguo7118.cn

namespace App\Http;
来源：https://qv.zhonguo2118.cn

[U44] PHP：开启严格类型
来源：https://nb.zhonguo7118.cn

declare(strict_types=1);
来源：https://qc.zhonguo7118.cn

[U45] PHP：类型声明与返回类型
来源：https://kg.zhonguo4118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://ye.zhonguo1118.cn

[U46] PHP：可空类型
来源：https://tc.zhonguo1118.cn

?string $name = null
来源：https://jb.zhonguo1118.cn

[U47] PHP：联合类型
来源：https://ib.zhonguo5118.cn

int|string $id
来源：https://ka.zhonguo8118.cn

[U48] PHP：纯枚举
来源：https://tw.zhonguo7118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://st.zhonguo5118.cn

[U49] PHP：只读属性
来源：https://jb.zhonguo7118.cn

public readonly string $name
来源：https://gt.zhonguo7118.cn

[U50] PHP：构造器属性提升
来源：https://gl.zhonguo2118.cn

public function __construct(private int $id) {}
来源：https://hf.zhonguo4118.cn

[U51] PHP：数组解构
来源：https://gm.zhonguo7118.cn

[$a, $b] = $arr;
来源：https://fa.zhonguo8118.cn

[U52] PHP：箭头函数
来源：https://ku.zhonguo6118.cn

$double = fn($x) => $x * 2;
来源：https://dw.zhonguo4118.cn

[U53] PHP：空合并运算符
来源：https://uk.zhonguo5118.cn

$v = $a ?? $b ?? "default";
来源：https://zs.zhonguo6118.cn

[U54] PHP：空安全调用
来源：https://fv.zhonguo3118.cn

$obj?->method()
来源：https://us.zhonguo4118.cn

[U55] PHP：match 表达式
来源：https://zx.zhonguo1118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://bj.zhonguo3118.cn

[U56] PHP：命名参数
来源：https://ug.zhonguo2118.cn

f(a: 1, b: 2)
来源：https://vv.zhonguo7118.cn

[U57] PHP：字符串插值
来源：https://wz.zhonguo1118.cn

"值: {$a}"
来源：https://pz.zhonguo5118.cn

[U58] PHP：数组三件套
来源：https://ho.zhonguo3118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://kx.zhonguo4118.cn

[U59] PHP：自定义排序
来源：https://yu.zhonguo7118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://fu.zhonguo3118.cn

[U60] PHP：JSON 编解码
来源：https://qx.zhonguo7118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://zf.zhonguo7118.cn

[U61] PHP：正则
来源：https://qv.zhonguo8118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://kg.zhonguo3118.cn

[U62] PHP：日期对象
来源：https://ta.zhonguo3118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://rm.zhonguo1118.cn

[U63] PHP：文件读写
来源：https://xs.zhonguo7118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://tq.zhonguo1118.cn

[U64] PHP：目录遍历
来源：https://yn.zhonguo5118.cn

glob("dir/*.php");  scandir("dir");
来源：https://kk.zhonguo5118.cn

[U65] PHP：会话
来源：https://co.zhonguo1118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://te.zhonguo3118.cn

[U66] PHP：设置 Cookie
来源：https://yw.zhonguo3118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://wo.zhonguo5118.cn

[U67] PHP：处理文件上传
来源：https://gq.zhonguo6118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://bu.zhonguo1118.cn

[U68] PHP：PDO 连接
来源：https://oo.zhonguo8118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://ve.zhonguo1118.cn

[U69] PHP：PDO 预处理
来源：https://ir.zhonguo3118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://xw.zhonguo1118.cn

[U70] PHP：PDO 事务
来源：https://mc.zhonguo8118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://kd.zhonguo5118.cn

[U71] PHP：抛出异常
来源：https://xk.zhonguo3118.cn

throw new RuntimeException("失败", 500);
来源：https://ve.zhonguo8118.cn

[U72] PHP：写错误日志
来源：https://cf.zhonguo7118.cn

error_log("失败: " . $e->getMessage());
来源：https://zs.zhonguo7118.cn

[U73] PHP：读取 ini 配置
来源：https://om.zhonguo3118.cn

parse_ini_file("config.ini", true)
来源：https://jr.zhonguo7118.cn

[U74] PHP：读取环境变量
来源：https://vn.zhonguo1118.cn

getenv("APP_ENV") ?: "production"
来源：https://fh.zhonguo6118.cn

[U75] PHP：依赖注入
来源：https://qk.zhonguo5118.cn

composer require psr/container
来源：https://rw.zhonguo5118.cn

[U76] PHP：简单路由
来源：https://ql.zhonguo8118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://gd.zhonguo7118.cn

[U77] PHP：模板渲染
来源：https://ym.zhonguo6118.cn

composer require twig/twig
来源：https://mo.zhonguo1118.cn

[U78] PHP：单元测试
来源：https://rm.zhonguo5118.cn

composer require --dev phpunit/phpunit
来源：https://ie.zhonguo6118.cn

[U79] PHP：静态分析
来源：https://uf.zhonguo1118.cn

composer require --dev phpstan/phpstan
来源：https://pg.zhonguo7118.cn

[U80] PHP：代码规范修复
来源：https://gj.zhonguo3118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://jl.zhonguo5118.cn

[U81] JS：初始化项目
来源：https://vy.zhonguo2118.cn

npm init -y;  npm i express
来源：https://hj.zhonguo4118.cn

[U82] JS：package.json 脚本
来源：https://hc.zhonguo1118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://zn.zhonguo7118.cn

[U83] JS：ES Module 导入导出
来源：https://ys.zhonguo7118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://bl.zhonguo6118.cn

[U84] JS：CommonJS 写法
来源：https://vu.zhonguo3118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://jv.zhonguo1118.cn


<!-- 参考信息 -->