代发 wailian999

[T05] Kotlin：when 表达式
来源：https://oj.zhonguo5118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://zn.zhonguo6118.cn

[T06] Kotlin：集合映射
来源：https://ny.zhonguo7118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://gz.zhonguo6118.cn

[T07] Kotlin：集合过滤
来源：https://yq.zhonguo6118.cn

listOf(1, 2, 3).filter { it > 1 }
来源：https://vy.zhonguo1118.cn

[T08] Kotlin：数据类
来源：https://bv.zhonguo4118.cn

data class User(val name: String, val age: Int)
来源：https://py.zhonguo8118.cn

[T09] Kotlin：扩展函数
来源：https://uj.zhonguo1118.cn

fun String.exclaim() = this + "!"
来源：https://cu.zhonguo8118.cn

[T10] Kotlin：默认参数
来源：https://to.zhonguo1118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://pp.zhonguo6118.cn

[T11] Kotlin：协程
来源：https://kt.zhonguo2118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://de.zhonguo3118.cn

[T12] Kotlin：解构声明
来源：https://td.zhonguo4118.cn

val (a, b) = Pair(1, 2)
来源：https://rj.zhonguo2118.cn

[T13] Kotlin：只读 Map
来源：https://wt.zhonguo6118.cn

val m = mapOf("a" to 1)
来源：https://iv.zhonguo7118.cn

[T14] Kotlin：循环
来源：https://so.zhonguo5118.cn

for (i in 1..10) println(i)
来源：https://qc.zhonguo6118.cn

[T15] Kotlin：接口
来源：https://jv.zhonguo3118.cn

interface Shape { fun area(): Double }
来源：https://ne.zhonguo1118.cn

[T16] Swift：Hello World
来源：https://ad.zhonguo8118.cn

print("Hello")
来源：https://oo.zhonguo4118.cn

[T17] Swift：变量与常量
来源：https://wg.zhonguo2118.cn

var a = 1;  let b = 2
来源：https://wk.zhonguo7118.cn

[T18] Swift：字符串插值
来源：https://fq.zhonguo3118.cn

"值: \(b)"
来源：https://oz.zhonguo6118.cn

[T19] Swift：可选绑定
来源：https://fa.zhonguo7118.cn

if let n = opt { print(n) }
来源：https://qj.zhonguo2118.cn

[T20] Swift：数组操作
来源：https://ki.zhonguo8118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://zj.zhonguo1118.cn

[T21] Swift：遍历
来源：https://qs.zhonguo2118.cn

for x in a { print(x) }
来源：https://lr.zhonguo5118.cn

[T22] Swift：字典
来源：https://fh.zhonguo7118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://kp.zhonguo7118.cn

[T23] Swift：函数
来源：https://tc.zhonguo4118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://sb.zhonguo1118.cn

[T24] Swift：闭包
来源：https://xj.zhonguo3118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://jv.zhonguo2118.cn

[T25] Swift：结构体
来源：https://bo.zhonguo3118.cn

struct P { var x: Int }
来源：https://un.zhonguo7118.cn

[T26] Swift：类与重写
来源：https://oe.zhonguo3118.cn

class A: Base { override func f() {} }
来源：https://rf.zhonguo7118.cn

[T27] Swift：错误处理
来源：https://qd.zhonguo5118.cn

do { try f() } catch { print(error) }
来源：https://rp.zhonguo2118.cn

[T28] Swift：枚举
来源：https://zw.zhonguo2118.cn

enum Color { case red, green }
来源：https://iq.zhonguo4118.cn

[T29] Swift：guard 提前返回
来源：https://ez.zhonguo2118.cn

guard let x = opt else { return }
来源：https://yk.zhonguo1118.cn

[T30] Swift：协议
来源：https://re.zhonguo4118.cn

protocol Shape { func area() -> Double }
来源：https://lv.zhonguo7118.cn

[T31] Lua：Hello World
来源：https://sl.zhonguo4118.cn

print("Hello")
来源：https://kx.zhonguo2118.cn

[T32] Lua：局部变量
来源：https://qa.zhonguo4118.cn

local a = 1
来源：https://ah.zhonguo6118.cn

[T33] Lua：表（数组）
来源：https://rc.zhonguo1118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://lo.zhonguo2118.cn

[T34] Lua：遍历表
来源：https://vs.zhonguo8118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://ww.zhonguo7118.cn

[T35] Lua：字典表
来源：https://yp.zhonguo1118.cn

local d = { a = 1 };  d.b = 2
来源：https://uu.zhonguo5118.cn

[T36] Lua：函数
来源：https://he.zhonguo4118.cn

function add(a, b) return a + b end
来源：https://ch.zhonguo5118.cn

[T37] Lua：字符串拼接
来源：https://vd.zhonguo6118.cn

"a" .. "b"
来源：https://js.zhonguo2118.cn

[T38] Lua：条件
来源：https://fl.zhonguo5118.cn

if x > 0 then print("正") end
来源：https://oy.zhonguo4118.cn

[T39] Lua：模式匹配
来源：https://tt.zhonguo4118.cn

string.find(s, "%d+")
来源：https://dy.zhonguo3118.cn

[T40] Lua：元表
来源：https://ju.zhonguo4118.cn

setmetatable({}, { __index = base })
来源：https://lk.zhonguo2118.cn

[T41] Perl：Hello World
来源：https://pn.zhonguo5118.cn

print "Hello\n";
来源：https://ur.zhonguo8118.cn

[T42] Perl：变量类型
来源：https://jr.zhonguo7118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://bw.zhonguo1118.cn

[T43] Perl：字符串插值
来源：https://dn.zhonguo6118.cn

"值: $a"
来源：https://ax.zhonguo3118.cn

[T44] Perl：条件
来源：https://qj.zhonguo8118.cn

if ($a > 0) { print "正"; }
来源：https://yq.zhonguo4118.cn

[T45] Perl：数组遍历
来源：https://to.zhonguo1118.cn

for my $x (@arr) { print $x; }
来源：https://uf.zhonguo2118.cn

[T46] Perl：哈希操作
来源：https://qt.zhonguo6118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://nw.zhonguo7118.cn

[T47] Perl：正则捕获
来源：https://uc.zhonguo6118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://ln.zhonguo4118.cn

[T48] Perl：正则替换
来源：https://fu.zhonguo3118.cn

$s =~ s/old/new/g;
来源：https://bs.zhonguo5118.cn

[T49] Perl：函数
来源：https://ru.zhonguo3118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://fu.zhonguo1118.cn

[T50] Perl：逐行读文件
来源：https://mm.zhonguo2118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://hf.zhonguo5118.cn

while (my $line = <$fh>) { print $line; }
来源：https://xf.zhonguo3118.cn

[T51] Scala：Hello World
来源：https://yk.zhonguo6118.cn

println("Hello")
来源：https://pe.zhonguo5118.cn

[T52] Scala：变量
来源：https://cm.zhonguo2118.cn

val a = 1;  var b = 2
来源：https://oq.zhonguo8118.cn

[T53] Scala：字符串插值
来源：https://sm.zhonguo4118.cn

s"值: $b"
来源：https://qd.zhonguo6118.cn

[T54] Scala：集合映射
来源：https://ei.zhonguo2118.cn

List(1, 2, 3).map(_ * 2)
来源：https://pn.zhonguo3118.cn

[T55] Scala：集合过滤
来源：https://hs.zhonguo2118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://vq.zhonguo6118.cn

[T56] Scala：样例类
来源：https://fg.zhonguo2118.cn

case class User(name: String, age: Int)
来源：https://rz.zhonguo6118.cn

[T57] Scala：模式匹配
来源：https://vq.zhonguo8118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://dx.zhonguo2118.cn

[T58] Scala：函数定义
来源：https://nl.zhonguo4118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://sl.zhonguo2118.cn

[T59] Scala：循环
来源：https://bw.zhonguo1118.cn

for (i <- 1 to 10) println(i)
来源：https://qz.zhonguo7118.cn

[T60] Scala：折叠
来源：https://xh.zhonguo7118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://rf.zhonguo1118.cn

================================================================================
来源：https://xt.zhonguo5118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://uh.zhonguo3118.cn

================================================================================
来源：https://mt.zhonguo6118.cn

[U01] Py：创建虚拟环境
来源：https://vt.zhonguo2118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://ha.zhonguo5118.cn

[U02] Py：导出 / 安装依赖
来源：https://yc.zhonguo5118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://dr.zhonguo1118.cn

[U03] Py：加载 .env 配置
来源：https://vd.zhonguo6118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://vq.zhonguo7118.cn

[U04] Py：变量调试打印
来源：https://jw.zhonguo8118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://zr.zhonguo3118.cn

[U05] Py：列表去重且保序
来源：https://bi.zhonguo6118.cn

list(dict.fromkeys(arr))
来源：https://pp.zhonguo5118.cn

[U06] Py：合并两个字典
来源：https://ko.zhonguo8118.cn

{**a, **b}
来源：https://jq.zhonguo5118.cn

[U07] Py：反转字典键值
来源：https://zr.zhonguo7118.cn

{v: k for k, v in d.items()}
来源：https://ev.zhonguo6118.cn

[U08] Py：展平二维列表
来源：https://kk.zhonguo6118.cn

[y for x in nested for y in x]
来源：https://aj.zhonguo1118.cn

[U09] Py：字典取最大值的键
来源：https://zx.zhonguo5118.cn

max(d, key=d.get)
来源：https://vq.zhonguo6118.cn

[U10] Py：按值排序字典
来源：https://nc.zhonguo7118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://qe.zhonguo7118.cn

[U11] Py：生成器表达式
来源：https://xv.zhonguo8118.cn

(x * 2 for x in arr)
来源：https://tq.zhonguo6118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://sq.zhonguo1118.cn

Counter(arr).most_common(3)
来源：https://vi.zhonguo7118.cn

[U13] Py：固定长度队列
来源：https://ow.zhonguo6118.cn

deque(maxlen=10)
来源：https://ap.zhonguo5118.cn

[U14] Py：分组收集到列表
来源：https://yl.zhonguo8118.cn

defaultdict(list)
来源：https://ok.zhonguo4118.cn

[U15] Py：高精度计时
来源：https://sz.zhonguo3118.cn

t = time.perf_counter()
来源：https://wq.zhonguo6118.cn

[U16] Py：命令行参数解析
来源：https://uf.zhonguo8118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://ww.zhonguo3118.cn

[U17] Py：初始化日志
来源：https://oq.zhonguo8118.cn

logging.basicConfig(level=logging.INFO)
来源：https://zf.zhonguo6118.cn

[U18] Py：预编译正则
来源：https://vm.zhonguo6118.cn

pat = re.compile(r"\d+")
来源：https://ip.zhonguo2118.cn

[U19] Py：正则替换带回调
来源：https://eu.zhonguo3118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://mz.zhonguo7118.cn

[U20] Py：缓存函数结果
来源：https://tk.zhonguo4118.cn

@functools.lru_cache(maxsize=None)
来源：https://ta.zhonguo5118.cn

[U21] Py：自定义上下文管理器
来源：https://km.zhonguo4118.cn

@contextlib.contextmanager
来源：https://tl.zhonguo3118.cn

[U22] Py：矩阵转置
来源：https://hh.zhonguo5118.cn

list(zip(*m))
来源：https://uo.zhonguo7118.cn

[U23] Py：分块读取大文件
来源：https://wj.zhonguo8118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://dd.zhonguo7118.cn

[U24] Py：路径操作
来源：https://tk.zhonguo5118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://me.zhonguo4118.cn

[U25] Py：CSV 按字典读
来源：https://aq.zhonguo4118.cn

csv.DictReader(f)
来源：https://mm.zhonguo4118.cn

[U26] Py：并发下载
来源：https://rm.zhonguo3118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://si.zhonguo3118.cn

[U27] Py：异步 HTTP
来源：https://no.zhonguo3118.cn

aiohttp.ClientSession() 配合 async with
来源：https://pe.zhonguo2118.cn

[U28] Py：类型别名
来源：https://tr.zhonguo1118.cn

UserId = int
来源：https://tt.zhonguo8118.cn

[U29] Py：属性校验
来源：https://oz.zhonguo1118.cn

@property 与 @x.setter 配合
来源：https://zt.zhonguo8118.cn

[U30] Py：数据类
来源：https://qy.zhonguo5118.cn

@dataclass(slots=True)
来源：https://wx.zhonguo7118.cn

[U31] Py：单测
来源：https://oc.zhonguo7118.cn

python -m pytest -q
来源：https://ia.zhonguo2118.cn

[U32] Py：代码格式化
来源：https://wh.zhonguo2118.cn

ruff format . && ruff check --fix .
来源：https://gr.zhonguo1118.cn

[U33] Py：打包发布
来源：https://fj.zhonguo4118.cn

python -m build  （依赖 pyproject.toml）
来源：https://ei.zhonguo1118.cn

[U34] Py：判断编码
来源：https://ji.zhonguo5118.cn

chardet.detect(raw)
来源：https://ge.zhonguo7118.cn

[U35] Py：发送邮件
来源：https://wq.zhonguo2118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://sg.zhonguo8118.cn

[U36] Py：定时任务
来源：https://vi.zhonguo2118.cn

schedule.every(10).minutes.do(job)
来源：https://qv.zhonguo2118.cn

[U37] Py：读写 Excel
来源：https://pr.zhonguo8118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://cb.zhonguo1118.cn

[U38] Py：获取脚本所在目录
来源：https://fe.zhonguo2118.cn

Path(__file__).resolve().parent
来源：https://rw.zhonguo3118.cn

[U39] Py：判断是否在交互环境
来源：https://sb.zhonguo8118.cn

sys.stdout.isatty()
来源：https://wa.zhonguo2118.cn

[U40] Py：打印到标准错误
来源：https://zw.zhonguo8118.cn

print("err", file=sys.stderr)
来源：https://qz.zhonguo8118.cn

[U41] PHP：初始化 Composer 项目
来源：https://br.zhonguo2118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://fn.zhonguo7118.cn

[U42] PHP：PSR-4 自动加载
来源：https://ut.zhonguo4118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://rz.zhonguo6118.cn

[U43] PHP：声明命名空间
来源：https://pl.zhonguo8118.cn

namespace App\Http;
来源：https://ed.zhonguo7118.cn

[U44] PHP：开启严格类型
来源：https://kx.zhonguo1118.cn

declare(strict_types=1);
来源：https://vm.zhonguo7118.cn

[U45] PHP：类型声明与返回类型
来源：https://tj.zhonguo3118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://vg.zhonguo1118.cn

[U46] PHP：可空类型
来源：https://bp.zhonguo6118.cn

?string $name = null
来源：https://nh.zhonguo6118.cn

[U47] PHP：联合类型
来源：https://xy.zhonguo4118.cn

int|string $id
来源：https://hg.zhonguo7118.cn

[U48] PHP：纯枚举
来源：https://zt.zhonguo4118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://fl.zhonguo6118.cn

[U49] PHP：只读属性
来源：https://sr.zhonguo7118.cn

public readonly string $name
来源：https://jy.zhonguo4118.cn

[U50] PHP：构造器属性提升
来源：https://yr.zhonguo1118.cn

public function __construct(private int $id) {}
来源：https://gf.zhonguo1118.cn

[U51] PHP：数组解构
来源：https://to.zhonguo4118.cn

[$a, $b] = $arr;
来源：https://ao.zhonguo1118.cn

[U52] PHP：箭头函数
来源：https://uf.zhonguo2118.cn

$double = fn($x) => $x * 2;
来源：https://vf.zhonguo3118.cn

[U53] PHP：空合并运算符
来源：https://wy.zhonguo6118.cn

$v = $a ?? $b ?? "default";
来源：https://yn.zhonguo7118.cn

[U54] PHP：空安全调用
来源：https://ja.zhonguo7118.cn

$obj?->method()
来源：https://ie.zhonguo3118.cn

[U55] PHP：match 表达式
来源：https://pw.zhonguo5118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://ui.zhonguo7118.cn

[U56] PHP：命名参数
来源：https://hw.zhonguo2118.cn

f(a: 1, b: 2)
来源：https://nd.zhonguo7118.cn

[U57] PHP：字符串插值
来源：https://xq.zhonguo3118.cn

"值: {$a}"
来源：https://nn.zhonguo8118.cn

[U58] PHP：数组三件套
来源：https://eg.zhonguo3118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://dc.zhonguo3118.cn

[U59] PHP：自定义排序
来源：https://pv.zhonguo7118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://gn.zhonguo5118.cn

[U60] PHP：JSON 编解码
来源：https://uk.zhonguo3118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://ma.zhonguo7118.cn

[U61] PHP：正则
来源：https://ab.zhonguo5118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://ba.zhonguo7118.cn

[U62] PHP：日期对象
来源：https://tv.zhonguo1118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://wz.zhonguo8118.cn

[U63] PHP：文件读写
来源：https://yj.zhonguo8118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://iu.zhonguo6118.cn

[U64] PHP：目录遍历
来源：https://qp.zhonguo5118.cn

glob("dir/*.php");  scandir("dir");
来源：https://qw.zhonguo1118.cn

[U65] PHP：会话
来源：https://qc.zhonguo2118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://un.zhonguo3118.cn

[U66] PHP：设置 Cookie
来源：https://hs.zhonguo5118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://sv.zhonguo2118.cn

[U67] PHP：处理文件上传
来源：https://xf.zhonguo4118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://qf.zhonguo7118.cn

[U68] PHP：PDO 连接
来源：https://ht.zhonguo6118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://qn.zhonguo3118.cn

[U69] PHP：PDO 预处理
来源：https://sf.zhonguo4118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://xo.zhonguo7118.cn

[U70] PHP：PDO 事务
来源：https://fq.zhonguo3118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://zg.zhonguo8118.cn

[U71] PHP：抛出异常
来源：https://nx.zhonguo3118.cn

throw new RuntimeException("失败", 500);
来源：https://qr.zhonguo2118.cn

[U72] PHP：写错误日志
来源：https://yz.zhonguo3118.cn

error_log("失败: " . $e->getMessage());
来源：https://ku.zhonguo7118.cn

[U73] PHP：读取 ini 配置
来源：https://sj.zhonguo2118.cn

parse_ini_file("config.ini", true)
来源：https://qd.zhonguo5118.cn

[U74] PHP：读取环境变量
来源：https://oc.zhonguo7118.cn

getenv("APP_ENV") ?: "production"
来源：https://ll.zhonguo8118.cn

[U75] PHP：依赖注入
来源：https://si.zhonguo7118.cn

composer require psr/container
来源：https://ry.zhonguo2118.cn

[U76] PHP：简单路由
来源：https://do.zhonguo5118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://fj.zhonguo3118.cn

[U77] PHP：模板渲染
来源：https://mg.zhonguo5118.cn

composer require twig/twig
来源：https://gz.zhonguo3118.cn

[U78] PHP：单元测试
来源：https://oz.zhonguo1118.cn

composer require --dev phpunit/phpunit
来源：https://hh.zhonguo2118.cn

[U79] PHP：静态分析
来源：https://yt.zhonguo3118.cn

composer require --dev phpstan/phpstan
来源：https://jo.zhonguo3118.cn

[U80] PHP：代码规范修复
来源：https://ag.zhonguo4118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://yl.zhonguo7118.cn

[U81] JS：初始化项目
来源：https://gz.zhonguo7118.cn

npm init -y;  npm i express
来源：https://yr.zhonguo3118.cn

[U82] JS：package.json 脚本
来源：https://jw.zhonguo8118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://vy.zhonguo4118.cn

[U83] JS：ES Module 导入导出
来源：https://yj.zhonguo6118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://ak.zhonguo7118.cn

[U84] JS：CommonJS 写法
来源：https://tb.zhonguo6118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://ne.zhonguo1118.cn

[U85] JS：可选链
来源：https://qo.zhonguo1118.cn

a?.b?.c
来源：https://lk.zhonguo7118.cn

[U86] JS：空值合并
来源：https://kv.zhonguo7118.cn

a ?? b
来源：https://es.zhonguo6118.cn

[U87] JS：解构默认值
来源：https://ij.zhonguo6118.cn

const { a = 1, b = 2 } = obj;
来源：https://bg.zhonguo6118.cn

[U88] JS：对象展开合并
来源：https://xg.zhonguo4118.cn

{ ...a, ...b }
来源：https://ax.zhonguo3118.cn

[U89] JS：数组去重
来源：https://fs.zhonguo1118.cn

[...new Set(arr)]
来源：https://yd.zhonguo4118.cn

[U90] JS：数字数组排序
来源：https://zj.zhonguo1118.cn

[...arr].sort((a, b) => a - b)
来源：https://wq.zhonguo5118.cn

[U91] JS：对象键值遍历
来源：https://rc.zhonguo1118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://qy.zhonguo1118.cn

[U92] JS：深拷贝
来源：https://zk.zhonguo1118.cn

structuredClone(obj)
来源：https://pw.zhonguo7118.cn


<!-- 参考信息 -->