代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://yu.zhonguo7118.cn

[S55] C++：结构化绑定
来源：https://aa.zhonguo1118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://be.zhonguo6118.cn

[S56] C++：optional
来源：https://tj.zhonguo8118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://io.zhonguo7118.cn

[S57] C++：编译期常量
来源：https://ip.zhonguo4118.cn

constexpr int N = 10;
来源：https://gu.zhonguo5118.cn

[S58] C++：命名空间
来源：https://yx.zhonguo7118.cn

namespace ns { int f() { return 1; } }
来源：https://ju.zhonguo1118.cn

[S59] C++：静态断言
来源：https://gl.zhonguo5118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://kq.zhonguo5118.cn

[S60] C++：遍历并删除元素
来源：https://hs.zhonguo5118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://kw.zhonguo2118.cn

================================================================================
来源：https://ay.zhonguo4118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://zp.zhonguo2118.cn

================================================================================
来源：https://tc.zhonguo8118.cn

[T01] Kotlin：Hello World
来源：https://vj.zhonguo3118.cn

println("Hello")
来源：https://te.zhonguo6118.cn

[T02] Kotlin：变量
来源：https://oz.zhonguo3118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://gm.zhonguo2118.cn

[T03] Kotlin：字符串模板
来源：https://di.zhonguo6118.cn

"值: $b"
来源：https://du.zhonguo5118.cn

[T04] Kotlin：空安全
来源：https://ic.zhonguo8118.cn

val n: String? = null;  n?.length
来源：https://eg.zhonguo3118.cn

[T05] Kotlin：when 表达式
来源：https://av.zhonguo5118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://wi.zhonguo4118.cn

[T06] Kotlin：集合映射
来源：https://fb.zhonguo1118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://co.zhonguo2118.cn

[T07] Kotlin：集合过滤
来源：https://zh.zhonguo7118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://wq.zhonguo5118.cn

[T08] Kotlin：数据类
来源：https://hv.zhonguo1118.cn

data class User(val name: String, val age: Int)
来源：https://hs.zhonguo5118.cn

[T09] Kotlin：扩展函数
来源：https://oc.zhonguo1118.cn

fun String.exclaim() = this + "!"
来源：https://wz.zhonguo8118.cn

[T10] Kotlin：默认参数
来源：https://ma.zhonguo8118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://mt.zhonguo1118.cn

[T11] Kotlin：协程
来源：https://av.zhonguo8118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://mu.zhonguo1118.cn

[T12] Kotlin：解构声明
来源：https://qj.zhonguo8118.cn

val (a, b) = Pair(1, 2)
来源：https://nx.zhonguo7118.cn

[T13] Kotlin：只读 Map
来源：https://xy.zhonguo5118.cn

val m = mapOf("a" to 1)
来源：https://tx.zhonguo5118.cn

[T14] Kotlin：循环
来源：https://ck.zhonguo2118.cn

for (i in 1..10) println(i)
来源：https://rj.zhonguo7118.cn

[T15] Kotlin：接口
来源：https://hw.zhonguo4118.cn

interface Shape { fun area(): Double }
来源：https://dt.zhonguo8118.cn

[T16] Swift：Hello World
来源：https://jg.zhonguo1118.cn

print("Hello")
来源：https://vh.zhonguo8118.cn

[T17] Swift：变量与常量
来源：https://mf.zhonguo7118.cn

var a = 1;  let b = 2
来源：https://nu.zhonguo6118.cn

[T18] Swift：字符串插值
来源：https://zw.zhonguo5118.cn

"值: \(b)"
来源：https://fm.zhonguo6118.cn

[T19] Swift：可选绑定
来源：https://be.zhonguo4118.cn

if let n = opt { print(n) }
来源：https://fh.zhonguo5118.cn

[T20] Swift：数组操作
来源：https://rz.zhonguo7118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://sd.zhonguo7118.cn

[T21] Swift：遍历
来源：https://cr.zhonguo1118.cn

for x in a { print(x) }
来源：https://ut.zhonguo6118.cn

[T22] Swift：字典
来源：https://qf.zhonguo2118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://no.zhonguo2118.cn

[T23] Swift：函数
来源：https://gk.zhonguo5118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://kb.zhonguo2118.cn

[T24] Swift：闭包
来源：https://kl.zhonguo6118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://hn.zhonguo3118.cn

[T25] Swift：结构体
来源：https://dr.zhonguo5118.cn

struct P { var x: Int }
来源：https://ah.zhonguo2118.cn

[T26] Swift：类与重写
来源：https://or.zhonguo2118.cn

class A: Base { override func f() {} }
来源：https://ya.zhonguo1118.cn

[T27] Swift：错误处理
来源：https://lg.zhonguo8118.cn

do { try f() } catch { print(error) }
来源：https://us.zhonguo5118.cn

[T28] Swift：枚举
来源：https://fc.zhonguo8118.cn

enum Color { case red, green }
来源：https://je.zhonguo2118.cn

[T29] Swift：guard 提前返回
来源：https://ks.zhonguo7118.cn

guard let x = opt else { return }
来源：https://dn.zhonguo6118.cn

[T30] Swift：协议
来源：https://qh.zhonguo2118.cn

protocol Shape { func area() -> Double }
来源：https://lm.zhonguo6118.cn

[T31] Lua：Hello World
来源：https://ix.zhonguo6118.cn

print("Hello")
来源：https://kj.zhonguo3118.cn

[T32] Lua：局部变量
来源：https://tg.zhonguo6118.cn

local a = 1
来源：https://jf.zhonguo3118.cn

[T33] Lua：表（数组）
来源：https://sn.zhonguo1118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://mc.zhonguo6118.cn

[T34] Lua：遍历表
来源：https://yk.zhonguo2118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://sp.zhonguo7118.cn

[T35] Lua：字典表
来源：https://vk.zhonguo8118.cn

local d = { a = 1 };  d.b = 2
来源：https://gg.zhonguo1118.cn

[T36] Lua：函数
来源：https://tw.zhonguo1118.cn

function add(a, b) return a + b end
来源：https://ry.zhonguo5118.cn

[T37] Lua：字符串拼接
来源：https://yn.zhonguo6118.cn

"a" .. "b"
来源：https://pp.zhonguo3118.cn

[T38] Lua：条件
来源：https://qo.zhonguo6118.cn

if x > 0 then print("正") end
来源：https://tw.zhonguo6118.cn

[T39] Lua：模式匹配
来源：https://xh.zhonguo7118.cn

string.find(s, "%d+")
来源：https://eq.zhonguo4118.cn

[T40] Lua：元表
来源：https://cv.zhonguo5118.cn

setmetatable({}, { __index = base })
来源：https://wr.zhonguo5118.cn

[T41] Perl：Hello World
来源：https://pi.zhonguo4118.cn

print "Hello\n";
来源：https://hi.zhonguo1118.cn

[T42] Perl：变量类型
来源：https://nx.zhonguo6118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://ve.zhonguo1118.cn

[T43] Perl：字符串插值
来源：https://to.zhonguo3118.cn

"值: $a"
来源：https://zt.zhonguo8118.cn

[T44] Perl：条件
来源：https://of.zhonguo2118.cn

if ($a > 0) { print "正"; }
来源：https://hg.zhonguo1118.cn

[T45] Perl：数组遍历
来源：https://db.zhonguo5118.cn

for my $x (@arr) { print $x; }
来源：https://qw.zhonguo4118.cn

[T46] Perl：哈希操作
来源：https://md.zhonguo5118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://yt.zhonguo4118.cn

[T47] Perl：正则捕获
来源：https://ki.zhonguo1118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://gp.zhonguo8118.cn

[T48] Perl：正则替换
来源：https://wq.zhonguo2118.cn

$s =~ s/old/new/g;
来源：https://oo.zhonguo2118.cn

[T49] Perl：函数
来源：https://lh.zhonguo4118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://cl.zhonguo1118.cn

[T50] Perl：逐行读文件
来源：https://rq.zhonguo1118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://rd.zhonguo4118.cn

while (my $line = <$fh>) { print $line; }
来源：https://jg.zhonguo4118.cn

[T51] Scala：Hello World
来源：https://kl.zhonguo5118.cn

println("Hello")
来源：https://as.zhonguo5118.cn

[T52] Scala：变量
来源：https://pp.zhonguo7118.cn

val a = 1;  var b = 2
来源：https://cy.zhonguo7118.cn

[T53] Scala：字符串插值
来源：https://gu.zhonguo3118.cn

s"值: $b"
来源：https://wt.zhonguo5118.cn

[T54] Scala：集合映射
来源：https://cj.zhonguo5118.cn

List(1, 2, 3).map(_ * 2)
来源：https://tc.zhonguo7118.cn

[T55] Scala：集合过滤
来源：https://ui.zhonguo7118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://ov.zhonguo4118.cn

[T56] Scala：样例类
来源：https://tn.zhonguo2118.cn

case class User(name: String, age: Int)
来源：https://vu.zhonguo3118.cn

[T57] Scala：模式匹配
来源：https://jn.zhonguo5118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://wd.zhonguo6118.cn

[T58] Scala：函数定义
来源：https://ea.zhonguo6118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://vr.zhonguo1118.cn

[T59] Scala：循环
来源：https://wx.zhonguo7118.cn

for (i <- 1 to 10) println(i)
来源：https://hi.zhonguo7118.cn

[T60] Scala：折叠
来源：https://ua.zhonguo2118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://wg.zhonguo3118.cn

================================================================================
来源：https://gw.zhonguo4118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://aj.zhonguo2118.cn

================================================================================
来源：https://qu.zhonguo2118.cn

[U01] Py：创建虚拟环境
来源：https://nf.zhonguo8118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://vr.zhonguo7118.cn

[U02] Py：导出 / 安装依赖
来源：https://ea.zhonguo6118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://kg.zhonguo5118.cn

[U03] Py：加载 .env 配置
来源：https://ba.zhonguo8118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://ji.zhonguo1118.cn

[U04] Py：变量调试打印
来源：https://cs.zhonguo5118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://wt.zhonguo1118.cn

[U05] Py：列表去重且保序
来源：https://jr.zhonguo2118.cn

list(dict.fromkeys(arr))
来源：https://jr.zhonguo7118.cn

[U06] Py：合并两个字典
来源：https://fd.zhonguo8118.cn

{**a, **b}
来源：https://zz.zhonguo2118.cn

[U07] Py：反转字典键值
来源：https://qj.zhonguo6118.cn

{v: k for k, v in d.items()}
来源：https://sp.zhonguo5118.cn

[U08] Py：展平二维列表
来源：https://zl.zhonguo1118.cn

[y for x in nested for y in x]
来源：https://jw.zhonguo5118.cn

[U09] Py：字典取最大值的键
来源：https://jn.zhonguo1118.cn

max(d, key=d.get)
来源：https://kt.zhonguo2118.cn

[U10] Py：按值排序字典
来源：https://dr.zhonguo4118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://mk.zhonguo3118.cn

[U11] Py：生成器表达式
来源：https://nj.zhonguo2118.cn

(x * 2 for x in arr)
来源：https://ko.zhonguo4118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://mq.zhonguo6118.cn

Counter(arr).most_common(3)
来源：https://uo.zhonguo2118.cn

[U13] Py：固定长度队列
来源：https://ir.zhonguo6118.cn

deque(maxlen=10)
来源：https://bg.zhonguo7118.cn

[U14] Py：分组收集到列表
来源：https://hk.zhonguo7118.cn

defaultdict(list)
来源：https://db.zhonguo3118.cn

[U15] Py：高精度计时
来源：https://we.zhonguo3118.cn

t = time.perf_counter()
来源：https://xz.zhonguo3118.cn

[U16] Py：命令行参数解析
来源：https://ug.zhonguo6118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://tx.zhonguo6118.cn

[U17] Py：初始化日志
来源：https://ai.zhonguo4118.cn

logging.basicConfig(level=logging.INFO)
来源：https://ru.zhonguo5118.cn

[U18] Py：预编译正则
来源：https://im.zhonguo4118.cn

pat = re.compile(r"\d+")
来源：https://ye.zhonguo1118.cn

[U19] Py：正则替换带回调
来源：https://mc.zhonguo4118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://nh.zhonguo1118.cn

[U20] Py：缓存函数结果
来源：https://kv.zhonguo2118.cn

@functools.lru_cache(maxsize=None)
来源：https://ud.zhonguo2118.cn

[U21] Py：自定义上下文管理器
来源：https://ej.zhonguo6118.cn

@contextlib.contextmanager
来源：https://za.zhonguo8118.cn

[U22] Py：矩阵转置
来源：https://ny.zhonguo2118.cn

list(zip(*m))
来源：https://gh.zhonguo5118.cn

[U23] Py：分块读取大文件
来源：https://br.zhonguo2118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://yu.zhonguo4118.cn

[U24] Py：路径操作
来源：https://th.zhonguo7118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://pr.zhonguo7118.cn

[U25] Py：CSV 按字典读
来源：https://cs.zhonguo6118.cn

csv.DictReader(f)
来源：https://nu.zhonguo3118.cn

[U26] Py：并发下载
来源：https://ve.zhonguo2118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://js.zhonguo8118.cn

[U27] Py：异步 HTTP
来源：https://lc.zhonguo8118.cn

aiohttp.ClientSession() 配合 async with
来源：https://mh.zhonguo2118.cn

[U28] Py：类型别名
来源：https://qk.zhonguo7118.cn

UserId = int
来源：https://pz.zhonguo4118.cn

[U29] Py：属性校验
来源：https://gh.zhonguo2118.cn

@property 与 @x.setter 配合
来源：https://re.zhonguo3118.cn

[U30] Py：数据类
来源：https://qf.zhonguo6118.cn

@dataclass(slots=True)
来源：https://xi.zhonguo5118.cn

[U31] Py：单测
来源：https://cl.zhonguo4118.cn

python -m pytest -q
来源：https://ue.zhonguo7118.cn

[U32] Py：代码格式化
来源：https://qm.zhonguo4118.cn

ruff format . && ruff check --fix .
来源：https://pk.zhonguo3118.cn

[U33] Py：打包发布
来源：https://io.zhonguo2118.cn

python -m build  （依赖 pyproject.toml）
来源：https://kq.zhonguo1118.cn

[U34] Py：判断编码
来源：https://ol.zhonguo7118.cn

chardet.detect(raw)
来源：https://kj.zhonguo7118.cn

[U35] Py：发送邮件
来源：https://mi.zhonguo5118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://hg.zhonguo4118.cn

[U36] Py：定时任务
来源：https://dg.zhonguo4118.cn

schedule.every(10).minutes.do(job)
来源：https://sd.zhonguo1118.cn

[U37] Py：读写 Excel
来源：https://mk.zhonguo8118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://rs.zhonguo5118.cn

[U38] Py：获取脚本所在目录
来源：https://kx.zhonguo7118.cn

Path(__file__).resolve().parent
来源：https://dd.zhonguo7118.cn

[U39] Py：判断是否在交互环境
来源：https://rz.zhonguo5118.cn

sys.stdout.isatty()
来源：https://im.zhonguo5118.cn

[U40] Py：打印到标准错误
来源：https://cr.zhonguo1118.cn

print("err", file=sys.stderr)
来源：https://lm.zhonguo5118.cn

[U41] PHP：初始化 Composer 项目
来源：https://ng.zhonguo1118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://po.zhonguo1118.cn

[U42] PHP：PSR-4 自动加载
来源：https://be.zhonguo2118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://kb.zhonguo1118.cn

[U43] PHP：声明命名空间
来源：https://gy.zhonguo7118.cn

namespace App\Http;
来源：https://qm.zhonguo2118.cn

[U44] PHP：开启严格类型
来源：https://tk.zhonguo4118.cn

declare(strict_types=1);
来源：https://gp.zhonguo4118.cn

[U45] PHP：类型声明与返回类型
来源：https://gp.zhonguo8118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://un.zhonguo7118.cn

[U46] PHP：可空类型
来源：https://br.zhonguo4118.cn

?string $name = null
来源：https://wk.zhonguo8118.cn

[U47] PHP：联合类型
来源：https://ih.zhonguo6118.cn

int|string $id
来源：https://gr.zhonguo2118.cn

[U48] PHP：纯枚举
来源：https://ad.zhonguo6118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://bt.zhonguo7118.cn

[U49] PHP：只读属性
来源：https://ib.zhonguo5118.cn

public readonly string $name
来源：https://bn.zhonguo3118.cn

[U50] PHP：构造器属性提升
来源：https://tn.zhonguo4118.cn

public function __construct(private int $id) {}
来源：https://ny.zhonguo8118.cn

[U51] PHP：数组解构
来源：https://jk.zhonguo1118.cn

[$a, $b] = $arr;
来源：https://cp.zhonguo1118.cn

[U52] PHP：箭头函数
来源：https://lm.zhonguo3118.cn

$double = fn($x) => $x * 2;
来源：https://fy.zhonguo1118.cn

[U53] PHP：空合并运算符
来源：https://zt.zhonguo6118.cn

$v = $a ?? $b ?? "default";
来源：https://ui.zhonguo4118.cn

[U54] PHP：空安全调用
来源：https://tp.zhonguo5118.cn

$obj?->method()
来源：https://xn.zhonguo8118.cn

[U55] PHP：match 表达式
来源：https://ud.zhonguo5118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://kc.zhonguo3118.cn

[U56] PHP：命名参数
来源：https://yu.zhonguo4118.cn

f(a: 1, b: 2)
来源：https://dg.zhonguo1118.cn

[U57] PHP：字符串插值
来源：https://eb.zhonguo6118.cn

"值: {$a}"
来源：https://el.zhonguo6118.cn

[U58] PHP：数组三件套
来源：https://rz.zhonguo8118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://zn.zhonguo3118.cn

[U59] PHP：自定义排序
来源：https://oe.zhonguo1118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://qn.zhonguo4118.cn

[U60] PHP：JSON 编解码
来源：https://ft.zhonguo1118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://ll.zhonguo5118.cn

[U61] PHP：正则
来源：https://ez.zhonguo7118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://hq.zhonguo2118.cn

[U62] PHP：日期对象
来源：https://xn.zhonguo7118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://iz.zhonguo7118.cn

[U63] PHP：文件读写
来源：https://bi.zhonguo3118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://gx.zhonguo7118.cn

[U64] PHP：目录遍历
来源：https://po.zhonguo4118.cn

glob("dir/*.php");  scandir("dir");
来源：https://ga.zhonguo3118.cn

[U65] PHP：会话
来源：https://vn.zhonguo7118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://qx.zhonguo5118.cn

[U66] PHP：设置 Cookie
来源：https://un.zhonguo3118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://rb.zhonguo3118.cn

[U67] PHP：处理文件上传
来源：https://qi.zhonguo6118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://iy.zhonguo8118.cn

[U68] PHP：PDO 连接
来源：https://yp.zhonguo4118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://iq.zhonguo4118.cn

[U69] PHP：PDO 预处理
来源：https://xp.zhonguo2118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://vw.zhonguo3118.cn

[U70] PHP：PDO 事务
来源：https://fs.zhonguo8118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://ci.zhonguo4118.cn

[U71] PHP：抛出异常
来源：https://kb.zhonguo4118.cn

throw new RuntimeException("失败", 500);
来源：https://ht.zhonguo2118.cn

[U72] PHP：写错误日志
来源：https://sf.zhonguo8118.cn

error_log("失败: " . $e->getMessage());
来源：https://ge.zhonguo1118.cn

[U73] PHP：读取 ini 配置
来源：https://gn.zhonguo1118.cn

parse_ini_file("config.ini", true)
来源：https://bu.zhonguo5118.cn

[U74] PHP：读取环境变量
来源：https://un.zhonguo6118.cn

getenv("APP_ENV") ?: "production"
来源：https://ap.zhonguo1118.cn

[U75] PHP：依赖注入
来源：https://ub.zhonguo4118.cn

composer require psr/container
来源：https://bg.zhonguo2118.cn

[U76] PHP：简单路由
来源：https://cy.zhonguo8118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://ct.zhonguo1118.cn

[U77] PHP：模板渲染
来源：https://zv.zhonguo1118.cn

composer require twig/twig
来源：https://vz.zhonguo3118.cn

[U78] PHP：单元测试
来源：https://vk.zhonguo2118.cn

composer require --dev phpunit/phpunit
来源：https://ca.zhonguo1118.cn

[U79] PHP：静态分析
来源：https://qe.zhonguo5118.cn

composer require --dev phpstan/phpstan
来源：https://uk.zhonguo1118.cn

[U80] PHP：代码规范修复
来源：https://es.zhonguo7118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://wm.zhonguo2118.cn


<!-- 参考信息 -->