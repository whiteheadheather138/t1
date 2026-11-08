代发 wailian999

[T09] Kotlin：扩展函数
来源：https://wo.zhonguo6118.cn

fun String.exclaim() = this + "!"
来源：https://ol.zhonguo2118.cn

[T10] Kotlin：默认参数
来源：https://yu.zhonguo7118.cn

fun greet(name: String = "World") = "Hi $name"
来源：https://cn.zhonguo5118.cn

[T11] Kotlin：协程
来源：https://uu.zhonguo2118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://bg.zhonguo8118.cn

[T12] Kotlin：解构声明
来源：https://wy.zhonguo7118.cn

val (a, b) = Pair(1, 2)
来源：https://jt.zhonguo2118.cn

[T13] Kotlin：只读 Map
来源：https://gw.zhonguo6118.cn

val m = mapOf("a" to 1)
来源：https://ng.zhonguo3118.cn

[T14] Kotlin：循环
来源：https://od.zhonguo1118.cn

for (i in 1..10) println(i)
来源：https://kb.zhonguo4118.cn

[T15] Kotlin：接口
来源：https://zb.zhonguo6118.cn

interface Shape { fun area(): Double }
来源：https://mq.zhonguo3118.cn

[T16] Swift：Hello World
来源：https://yv.zhonguo5118.cn

print("Hello")
来源：https://zw.zhonguo5118.cn

[T17] Swift：变量与常量
来源：https://wc.zhonguo8118.cn

var a = 1;  let b = 2
来源：https://uh.zhonguo6118.cn

[T18] Swift：字符串插值
来源：https://fu.zhonguo6118.cn

"值: \(b)"
来源：https://ci.zhonguo1118.cn

[T19] Swift：可选绑定
来源：https://xs.zhonguo6118.cn

if let n = opt { print(n) }
来源：https://qk.zhonguo2118.cn

[T20] Swift：数组操作
来源：https://hj.zhonguo1118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://dw.zhonguo6118.cn

[T21] Swift：遍历
来源：https://an.zhonguo4118.cn

for x in a { print(x) }
来源：https://jt.zhonguo7118.cn

[T22] Swift：字典
来源：https://zi.zhonguo6118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://te.zhonguo6118.cn

[T23] Swift：函数
来源：https://pe.zhonguo4118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://oh.zhonguo4118.cn

[T24] Swift：闭包
来源：https://tg.zhonguo8118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://vz.zhonguo8118.cn

[T25] Swift：结构体
来源：https://cb.zhonguo7118.cn

struct P { var x: Int }
来源：https://kz.zhonguo2118.cn

[T26] Swift：类与重写
来源：https://uj.zhonguo1118.cn

class A: Base { override func f() {} }
来源：https://og.zhonguo5118.cn

[T27] Swift：错误处理
来源：https://km.zhonguo2118.cn

do { try f() } catch { print(error) }
来源：https://vn.zhonguo7118.cn

[T28] Swift：枚举
来源：https://zo.zhonguo7118.cn

enum Color { case red, green }
来源：https://xg.zhonguo1118.cn

[T29] Swift：guard 提前返回
来源：https://bv.zhonguo5118.cn

guard let x = opt else { return }
来源：https://gj.zhonguo5118.cn

[T30] Swift：协议
来源：https://ll.zhonguo1118.cn

protocol Shape { func area() -> Double }
来源：https://if.zhonguo4118.cn

[T31] Lua：Hello World
来源：https://yp.zhonguo3118.cn

print("Hello")
来源：https://wy.zhonguo6118.cn

[T32] Lua：局部变量
来源：https://ih.zhonguo1118.cn

local a = 1
来源：https://kg.zhonguo5118.cn

[T33] Lua：表（数组）
来源：https://km.zhonguo4118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://tb.zhonguo1118.cn

[T34] Lua：遍历表
来源：https://td.zhonguo1118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://wg.zhonguo1118.cn

[T35] Lua：字典表
来源：https://xn.zhonguo8118.cn

local d = { a = 1 };  d.b = 2
来源：https://di.zhonguo8118.cn

[T36] Lua：函数
来源：https://fj.zhonguo7118.cn

function add(a, b) return a + b end
来源：https://yh.zhonguo2118.cn

[T37] Lua：字符串拼接
来源：https://jt.zhonguo6118.cn

"a" .. "b"
来源：https://hm.zhonguo6118.cn

[T38] Lua：条件
来源：https://ru.zhonguo8118.cn

if x > 0 then print("正") end
来源：https://gw.zhonguo6118.cn

[T39] Lua：模式匹配
来源：https://rr.zhonguo4118.cn

string.find(s, "%d+")
来源：https://kt.zhonguo7118.cn

[T40] Lua：元表
来源：https://ud.zhonguo7118.cn

setmetatable({}, { __index = base })
来源：https://yx.zhonguo5118.cn

[T41] Perl：Hello World
来源：https://hc.zhonguo7118.cn

print "Hello\n";
来源：https://me.zhonguo8118.cn

[T42] Perl：变量类型
来源：https://ut.zhonguo1118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://zq.zhonguo3118.cn

[T43] Perl：字符串插值
来源：https://dv.zhonguo3118.cn

"值: $a"
来源：https://po.zhonguo4118.cn

[T44] Perl：条件
来源：https://wg.zhonguo3118.cn

if ($a > 0) { print "正"; }
来源：https://yn.zhonguo2118.cn

[T45] Perl：数组遍历
来源：https://ae.zhonguo3118.cn

for my $x (@arr) { print $x; }
来源：https://ps.zhonguo2118.cn

[T46] Perl：哈希操作
来源：https://ed.zhonguo4118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://gv.zhonguo6118.cn

[T47] Perl：正则捕获
来源：https://jg.zhonguo2118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://tq.zhonguo5118.cn

[T48] Perl：正则替换
来源：https://ce.zhonguo1118.cn

$s =~ s/old/new/g;
来源：https://zr.zhonguo6118.cn

[T49] Perl：函数
来源：https://ir.zhonguo6118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://rd.zhonguo4118.cn

[T50] Perl：逐行读文件
来源：https://rg.zhonguo4118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://my.zhonguo7118.cn

while (my $line = <$fh>) { print $line; }
来源：https://oe.zhonguo6118.cn

[T51] Scala：Hello World
来源：https://tu.zhonguo6118.cn

println("Hello")
来源：https://jv.zhonguo4118.cn

[T52] Scala：变量
来源：https://ov.zhonguo6118.cn

val a = 1;  var b = 2
来源：https://kh.zhonguo4118.cn

[T53] Scala：字符串插值
来源：https://gk.zhonguo1118.cn

s"值: $b"
来源：https://wz.zhonguo7118.cn

[T54] Scala：集合映射
来源：https://uq.zhonguo2118.cn

List(1, 2, 3).map(_ * 2)
来源：https://bs.zhonguo4118.cn

[T55] Scala：集合过滤
来源：https://cq.zhonguo4118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://qp.zhonguo3118.cn

[T56] Scala：样例类
来源：https://yn.zhonguo1118.cn

case class User(name: String, age: Int)
来源：https://ny.zhonguo6118.cn

[T57] Scala：模式匹配
来源：https://cw.zhonguo1118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://el.zhonguo3118.cn

[T58] Scala：函数定义
来源：https://mb.zhonguo6118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://as.zhonguo5118.cn

[T59] Scala：循环
来源：https://kg.zhonguo1118.cn

for (i <- 1 to 10) println(i)
来源：https://pp.zhonguo2118.cn

[T60] Scala：折叠
来源：https://mw.zhonguo2118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://sr.zhonguo1118.cn

================================================================================
来源：https://bq.zhonguo4118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://qw.zhonguo7118.cn

================================================================================
来源：https://hy.zhonguo6118.cn

[U01] Py：创建虚拟环境
来源：https://zf.zhonguo1118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://qd.zhonguo5118.cn

[U02] Py：导出 / 安装依赖
来源：https://mt.zhonguo7118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://lc.zhonguo4118.cn

[U03] Py：加载 .env 配置
来源：https://te.zhonguo6118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://be.zhonguo3118.cn

[U04] Py：变量调试打印
来源：https://hv.zhonguo1118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://np.zhonguo3118.cn

[U05] Py：列表去重且保序
来源：https://iu.zhonguo5118.cn

list(dict.fromkeys(arr))
来源：https://xo.zhonguo4118.cn

[U06] Py：合并两个字典
来源：https://nq.zhonguo6118.cn

{**a, **b}
来源：https://ak.zhonguo6118.cn

[U07] Py：反转字典键值
来源：https://ir.zhonguo4118.cn

{v: k for k, v in d.items()}
来源：https://cb.zhonguo5118.cn

[U08] Py：展平二维列表
来源：https://ul.zhonguo5118.cn

[y for x in nested for y in x]
来源：https://ib.zhonguo2118.cn

[U09] Py：字典取最大值的键
来源：https://az.zhonguo5118.cn

max(d, key=d.get)
来源：https://ts.zhonguo7118.cn

[U10] Py：按值排序字典
来源：https://yy.zhonguo1118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://vb.zhonguo4118.cn

[U11] Py：生成器表达式
来源：https://lq.zhonguo5118.cn

(x * 2 for x in arr)
来源：https://lj.zhonguo7118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://in.zhonguo3118.cn

Counter(arr).most_common(3)
来源：https://yi.zhonguo2118.cn

[U13] Py：固定长度队列
来源：https://dh.zhonguo8118.cn

deque(maxlen=10)
来源：https://it.zhonguo1118.cn

[U14] Py：分组收集到列表
来源：https://co.zhonguo2118.cn

defaultdict(list)
来源：https://yk.zhonguo6118.cn

[U15] Py：高精度计时
来源：https://fw.zhonguo4118.cn

t = time.perf_counter()
来源：https://cm.zhonguo5118.cn

[U16] Py：命令行参数解析
来源：https://rb.zhonguo6118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://eb.zhonguo2118.cn

[U17] Py：初始化日志
来源：https://ta.zhonguo8118.cn

logging.basicConfig(level=logging.INFO)
来源：https://fi.zhonguo5118.cn

[U18] Py：预编译正则
来源：https://qf.zhonguo3118.cn

pat = re.compile(r"\d+")
来源：https://qi.zhonguo1118.cn

[U19] Py：正则替换带回调
来源：https://fm.zhonguo3118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://nh.zhonguo4118.cn

[U20] Py：缓存函数结果
来源：https://gu.zhonguo5118.cn

@functools.lru_cache(maxsize=None)
来源：https://eu.zhonguo5118.cn

[U21] Py：自定义上下文管理器
来源：https://kn.zhonguo3118.cn

@contextlib.contextmanager
来源：https://gm.zhonguo7118.cn

[U22] Py：矩阵转置
来源：https://ja.zhonguo4118.cn

list(zip(*m))
来源：https://kv.zhonguo3118.cn

[U23] Py：分块读取大文件
来源：https://ld.zhonguo1118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://dw.zhonguo2118.cn

[U24] Py：路径操作
来源：https://wh.zhonguo4118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://wp.zhonguo1118.cn

[U25] Py：CSV 按字典读
来源：https://mj.zhonguo4118.cn

csv.DictReader(f)
来源：https://lu.zhonguo5118.cn

[U26] Py：并发下载
来源：https://vg.zhonguo1118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://jo.zhonguo5118.cn

[U27] Py：异步 HTTP
来源：https://qa.zhonguo4118.cn

aiohttp.ClientSession() 配合 async with
来源：https://xu.zhonguo2118.cn

[U28] Py：类型别名
来源：https://eb.zhonguo4118.cn

UserId = int
来源：https://ib.zhonguo7118.cn

[U29] Py：属性校验
来源：https://bb.zhonguo7118.cn

@property 与 @x.setter 配合
来源：https://fa.zhonguo2118.cn

[U30] Py：数据类
来源：https://df.zhonguo8118.cn

@dataclass(slots=True)
来源：https://sg.zhonguo7118.cn

[U31] Py：单测
来源：https://ni.zhonguo8118.cn

python -m pytest -q
来源：https://re.zhonguo3118.cn

[U32] Py：代码格式化
来源：https://qb.zhonguo8118.cn

ruff format . && ruff check --fix .
来源：https://cd.zhonguo1118.cn

[U33] Py：打包发布
来源：https://wj.zhonguo6118.cn

python -m build  （依赖 pyproject.toml）
来源：https://ik.zhonguo7118.cn

[U34] Py：判断编码
来源：https://jm.zhonguo7118.cn

chardet.detect(raw)
来源：https://ij.zhonguo3118.cn

[U35] Py：发送邮件
来源：https://qo.zhonguo4118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://jz.zhonguo1118.cn

[U36] Py：定时任务
来源：https://fp.zhonguo6118.cn

schedule.every(10).minutes.do(job)
来源：https://lv.zhonguo7118.cn

[U37] Py：读写 Excel
来源：https://di.zhonguo5118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://ok.zhonguo4118.cn

[U38] Py：获取脚本所在目录
来源：https://mj.zhonguo6118.cn

Path(__file__).resolve().parent
来源：https://ms.zhonguo7118.cn

[U39] Py：判断是否在交互环境
来源：https://gb.zhonguo6118.cn

sys.stdout.isatty()
来源：https://pi.zhonguo1118.cn

[U40] Py：打印到标准错误
来源：https://ll.zhonguo1118.cn

print("err", file=sys.stderr)
来源：https://iv.zhonguo4118.cn

[U41] PHP：初始化 Composer 项目
来源：https://ae.zhonguo2118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://qr.zhonguo6118.cn

[U42] PHP：PSR-4 自动加载
来源：https://yx.zhonguo3118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://dh.zhonguo1118.cn

[U43] PHP：声明命名空间
来源：https://qh.zhonguo7118.cn

namespace App\Http;
来源：https://fk.zhonguo8118.cn

[U44] PHP：开启严格类型
来源：https://yt.zhonguo4118.cn

declare(strict_types=1);
来源：https://nl.zhonguo7118.cn

[U45] PHP：类型声明与返回类型
来源：https://zj.zhonguo3118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://ct.zhonguo3118.cn

[U46] PHP：可空类型
来源：https://cq.zhonguo6118.cn

?string $name = null
来源：https://ns.zhonguo7118.cn

[U47] PHP：联合类型
来源：https://wr.zhonguo6118.cn

int|string $id
来源：https://pr.zhonguo5118.cn

[U48] PHP：纯枚举
来源：https://lf.zhonguo3118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://cx.zhonguo7118.cn

[U49] PHP：只读属性
来源：https://ia.zhonguo4118.cn

public readonly string $name
来源：https://lm.zhonguo2118.cn

[U50] PHP：构造器属性提升
来源：https://hk.zhonguo5118.cn

public function __construct(private int $id) {}
来源：https://rd.zhonguo5118.cn

[U51] PHP：数组解构
来源：https://rd.zhonguo8118.cn

[$a, $b] = $arr;
来源：https://bd.zhonguo7118.cn

[U52] PHP：箭头函数
来源：https://up.zhonguo4118.cn

$double = fn($x) => $x * 2;
来源：https://nz.zhonguo8118.cn

[U53] PHP：空合并运算符
来源：https://mq.zhonguo1118.cn

$v = $a ?? $b ?? "default";
来源：https://qc.zhonguo8118.cn

[U54] PHP：空安全调用
来源：https://fj.zhonguo1118.cn

$obj?->method()
来源：https://sq.zhonguo6118.cn

[U55] PHP：match 表达式
来源：https://po.zhonguo6118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://dd.zhonguo1118.cn

[U56] PHP：命名参数
来源：https://sd.zhonguo8118.cn

f(a: 1, b: 2)
来源：https://qr.zhonguo7118.cn

[U57] PHP：字符串插值
来源：https://nc.zhonguo4118.cn

"值: {$a}"
来源：https://eo.zhonguo1118.cn

[U58] PHP：数组三件套
来源：https://jr.zhonguo7118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://wb.zhonguo2118.cn

[U59] PHP：自定义排序
来源：https://pt.zhonguo7118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://du.zhonguo6118.cn

[U60] PHP：JSON 编解码
来源：https://cr.zhonguo1118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://be.zhonguo1118.cn

[U61] PHP：正则
来源：https://mc.zhonguo5118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://ru.zhonguo2118.cn

[U62] PHP：日期对象
来源：https://ht.zhonguo1118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://pl.zhonguo3118.cn

[U63] PHP：文件读写
来源：https://jc.zhonguo7118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://en.zhonguo5118.cn

[U64] PHP：目录遍历
来源：https://kq.zhonguo4118.cn

glob("dir/*.php");  scandir("dir");
来源：https://nq.zhonguo5118.cn

[U65] PHP：会话
来源：https://ij.zhonguo7118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://rk.zhonguo6118.cn

[U66] PHP：设置 Cookie
来源：https://gh.zhonguo2118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://pp.zhonguo1118.cn

[U67] PHP：处理文件上传
来源：https://pb.zhonguo3118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://pv.zhonguo6118.cn

[U68] PHP：PDO 连接
来源：https://mh.zhonguo3118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://ty.zhonguo4118.cn

[U69] PHP：PDO 预处理
来源：https://in.zhonguo3118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://dm.zhonguo6118.cn

[U70] PHP：PDO 事务
来源：https://hl.zhonguo2118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://ux.zhonguo7118.cn

[U71] PHP：抛出异常
来源：https://nb.zhonguo8118.cn

throw new RuntimeException("失败", 500);
来源：https://uo.zhonguo4118.cn

[U72] PHP：写错误日志
来源：https://az.zhonguo6118.cn

error_log("失败: " . $e->getMessage());
来源：https://fb.zhonguo4118.cn

[U73] PHP：读取 ini 配置
来源：https://fl.zhonguo6118.cn

parse_ini_file("config.ini", true)
来源：https://nq.zhonguo7118.cn

[U74] PHP：读取环境变量
来源：https://ne.zhonguo6118.cn

getenv("APP_ENV") ?: "production"
来源：https://yi.zhonguo4118.cn

[U75] PHP：依赖注入
来源：https://kh.zhonguo1118.cn

composer require psr/container
来源：https://dk.zhonguo1118.cn

[U76] PHP：简单路由
来源：https://qd.zhonguo1118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://xk.zhonguo2118.cn

[U77] PHP：模板渲染
来源：https://mk.zhonguo3118.cn

composer require twig/twig
来源：https://sc.zhonguo8118.cn

[U78] PHP：单元测试
来源：https://bm.zhonguo6118.cn

composer require --dev phpunit/phpunit
来源：https://rn.zhonguo3118.cn

[U79] PHP：静态分析
来源：https://ce.zhonguo4118.cn

composer require --dev phpstan/phpstan
来源：https://of.zhonguo7118.cn

[U80] PHP：代码规范修复
来源：https://dm.zhonguo5118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://ks.zhonguo5118.cn

[U81] JS：初始化项目
来源：https://wm.zhonguo7118.cn

npm init -y;  npm i express
来源：https://pd.zhonguo3118.cn

[U82] JS：package.json 脚本
来源：https://my.zhonguo1118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://cv.zhonguo6118.cn

[U83] JS：ES Module 导入导出
来源：https://zv.zhonguo7118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://um.zhonguo2118.cn

[U84] JS：CommonJS 写法
来源：https://hn.zhonguo5118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://kh.zhonguo4118.cn

[U85] JS：可选链
来源：https://xo.zhonguo5118.cn

a?.b?.c
来源：https://kg.zhonguo2118.cn

[U86] JS：空值合并
来源：https://nj.zhonguo8118.cn

a ?? b
来源：https://rx.zhonguo4118.cn

[U87] JS：解构默认值
来源：https://cu.zhonguo2118.cn

const { a = 1, b = 2 } = obj;
来源：https://no.zhonguo3118.cn

[U88] JS：对象展开合并
来源：https://ih.zhonguo7118.cn

{ ...a, ...b }
来源：https://ye.zhonguo3118.cn

[U89] JS：数组去重
来源：https://wd.zhonguo3118.cn

[...new Set(arr)]
来源：https://ge.zhonguo1118.cn

[U90] JS：数字数组排序
来源：https://ir.zhonguo4118.cn

[...arr].sort((a, b) => a - b)
来源：https://hl.zhonguo5118.cn

[U91] JS：对象键值遍历
来源：https://sp.zhonguo7118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://ym.zhonguo8118.cn

[U92] JS：深拷贝
来源：https://hl.zhonguo3118.cn

structuredClone(obj)
来源：https://tb.zhonguo7118.cn

[U93] JS：模板字符串
来源：https://hq.zhonguo4118.cn

`共 ${n} 条`
来源：https://cm.zhonguo3118.cn

[U94] JS：箭头函数
来源：https://ex.zhonguo3118.cn

const double = x => x * 2;
来源：https://jf.zhonguo8118.cn

[U95] JS：Promise 包装
来源：https://az.zhonguo5118.cn

new Promise((resolve, reject) => {})
来源：https://np.zhonguo3118.cn

[U96] JS：async/await 与异常
来源：https://ws.zhonguo7118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://nu.zhonguo6118.cn


<!-- 参考信息 -->