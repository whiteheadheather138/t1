代发 wailian999

[T11] Kotlin：协程
来源：https://td.zhonguo2118.cn

GlobalScope.launch { delay(1000); println("done") }
来源：https://pu.zhonguo2118.cn

[T12] Kotlin：解构声明
来源：https://mf.zhonguo1118.cn

val (a, b) = Pair(1, 2)
来源：https://bg.zhonguo3118.cn

[T13] Kotlin：只读 Map
来源：https://es.zhonguo2118.cn

val m = mapOf("a" to 1)
来源：https://zz.zhonguo1118.cn

[T14] Kotlin：循环
来源：https://jg.zhonguo8118.cn

for (i in 1..10) println(i)
来源：https://ly.zhonguo4118.cn

[T15] Kotlin：接口
来源：https://nd.zhonguo4118.cn

interface Shape { fun area(): Double }
来源：https://pb.zhonguo8118.cn

[T16] Swift：Hello World
来源：https://dk.zhonguo7118.cn

print("Hello")
来源：https://iw.zhonguo8118.cn

[T17] Swift：变量与常量
来源：https://ie.zhonguo6118.cn

var a = 1;  let b = 2
来源：https://nn.zhonguo6118.cn

[T18] Swift：字符串插值
来源：https://qc.zhonguo6118.cn

"值: \(b)"
来源：https://vs.zhonguo6118.cn

[T19] Swift：可选绑定
来源：https://ef.zhonguo7118.cn

if let n = opt { print(n) }
来源：https://tb.zhonguo3118.cn

[T20] Swift：数组操作
来源：https://mm.zhonguo3118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://nq.zhonguo3118.cn

[T21] Swift：遍历
来源：https://oc.zhonguo2118.cn

for x in a { print(x) }
来源：https://oz.zhonguo2118.cn

[T22] Swift：字典
来源：https://zp.zhonguo1118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://bm.zhonguo2118.cn

[T23] Swift：函数
来源：https://ti.zhonguo6118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://sg.zhonguo5118.cn

[T24] Swift：闭包
来源：https://cl.zhonguo6118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://bk.zhonguo3118.cn

[T25] Swift：结构体
来源：https://lw.zhonguo5118.cn

struct P { var x: Int }
来源：https://ud.zhonguo3118.cn

[T26] Swift：类与重写
来源：https://tk.zhonguo2118.cn

class A: Base { override func f() {} }
来源：https://ns.zhonguo6118.cn

[T27] Swift：错误处理
来源：https://rg.zhonguo7118.cn

do { try f() } catch { print(error) }
来源：https://bj.zhonguo1118.cn

[T28] Swift：枚举
来源：https://eq.zhonguo8118.cn

enum Color { case red, green }
来源：https://yx.zhonguo1118.cn

[T29] Swift：guard 提前返回
来源：https://nj.zhonguo2118.cn

guard let x = opt else { return }
来源：https://kg.zhonguo5118.cn

[T30] Swift：协议
来源：https://ui.zhonguo6118.cn

protocol Shape { func area() -> Double }
来源：https://hb.zhonguo6118.cn

[T31] Lua：Hello World
来源：https://tq.zhonguo6118.cn

print("Hello")
来源：https://pu.zhonguo6118.cn

[T32] Lua：局部变量
来源：https://nk.zhonguo1118.cn

local a = 1
来源：https://sz.zhonguo5118.cn

[T33] Lua：表（数组）
来源：https://ng.zhonguo1118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://rz.zhonguo8118.cn

[T34] Lua：遍历表
来源：https://wm.zhonguo8118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://la.zhonguo8118.cn

[T35] Lua：字典表
来源：https://dx.zhonguo5118.cn

local d = { a = 1 };  d.b = 2
来源：https://qi.zhonguo6118.cn

[T36] Lua：函数
来源：https://nz.zhonguo3118.cn

function add(a, b) return a + b end
来源：https://mp.zhonguo2118.cn

[T37] Lua：字符串拼接
来源：https://kt.zhonguo2118.cn

"a" .. "b"
来源：https://hb.zhonguo3118.cn

[T38] Lua：条件
来源：https://mx.zhonguo4118.cn

if x > 0 then print("正") end
来源：https://zw.zhonguo5118.cn

[T39] Lua：模式匹配
来源：https://yv.zhonguo3118.cn

string.find(s, "%d+")
来源：https://lj.zhonguo1118.cn

[T40] Lua：元表
来源：https://xw.zhonguo7118.cn

setmetatable({}, { __index = base })
来源：https://hh.zhonguo1118.cn

[T41] Perl：Hello World
来源：https://rp.zhonguo1118.cn

print "Hello\n";
来源：https://by.zhonguo4118.cn

[T42] Perl：变量类型
来源：https://zc.zhonguo5118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://kz.zhonguo7118.cn

[T43] Perl：字符串插值
来源：https://mz.zhonguo2118.cn

"值: $a"
来源：https://iq.zhonguo7118.cn

[T44] Perl：条件
来源：https://ts.zhonguo5118.cn

if ($a > 0) { print "正"; }
来源：https://hc.zhonguo3118.cn

[T45] Perl：数组遍历
来源：https://cy.zhonguo7118.cn

for my $x (@arr) { print $x; }
来源：https://mm.zhonguo5118.cn

[T46] Perl：哈希操作
来源：https://pn.zhonguo8118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://jv.zhonguo3118.cn

[T47] Perl：正则捕获
来源：https://yj.zhonguo2118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://jz.zhonguo2118.cn

[T48] Perl：正则替换
来源：https://xl.zhonguo7118.cn

$s =~ s/old/new/g;
来源：https://tf.zhonguo5118.cn

[T49] Perl：函数
来源：https://ne.zhonguo7118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://tt.zhonguo1118.cn

[T50] Perl：逐行读文件
来源：https://oc.zhonguo8118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://ys.zhonguo2118.cn

while (my $line = <$fh>) { print $line; }
来源：https://vk.zhonguo5118.cn

[T51] Scala：Hello World
来源：https://id.zhonguo4118.cn

println("Hello")
来源：https://tq.zhonguo4118.cn

[T52] Scala：变量
来源：https://rk.zhonguo6118.cn

val a = 1;  var b = 2
来源：https://yt.zhonguo7118.cn

[T53] Scala：字符串插值
来源：https://qk.zhonguo4118.cn

s"值: $b"
来源：https://he.zhonguo8118.cn

[T54] Scala：集合映射
来源：https://dl.zhonguo5118.cn

List(1, 2, 3).map(_ * 2)
来源：https://oa.zhonguo6118.cn

[T55] Scala：集合过滤
来源：https://lq.zhonguo2118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://mq.zhonguo2118.cn

[T56] Scala：样例类
来源：https://nt.zhonguo1118.cn

case class User(name: String, age: Int)
来源：https://xb.zhonguo1118.cn

[T57] Scala：模式匹配
来源：https://ni.zhonguo8118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://vr.zhonguo4118.cn

[T58] Scala：函数定义
来源：https://xj.zhonguo3118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://ez.zhonguo8118.cn

[T59] Scala：循环
来源：https://cm.zhonguo6118.cn

for (i <- 1 to 10) println(i)
来源：https://dm.zhonguo8118.cn

[T60] Scala：折叠
来源：https://ww.zhonguo7118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://ro.zhonguo3118.cn

================================================================================
来源：https://zi.zhonguo6118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://xg.zhonguo2118.cn

================================================================================
来源：https://th.zhonguo3118.cn

[U01] Py：创建虚拟环境
来源：https://av.zhonguo2118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://fi.zhonguo6118.cn

[U02] Py：导出 / 安装依赖
来源：https://fq.zhonguo5118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://lt.zhonguo6118.cn

[U03] Py：加载 .env 配置
来源：https://wm.zhonguo6118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://ot.zhonguo8118.cn

[U04] Py：变量调试打印
来源：https://tl.zhonguo4118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://rj.zhonguo4118.cn

[U05] Py：列表去重且保序
来源：https://ub.zhonguo2118.cn

list(dict.fromkeys(arr))
来源：https://de.zhonguo6118.cn

[U06] Py：合并两个字典
来源：https://li.zhonguo3118.cn

{**a, **b}
来源：https://it.zhonguo4118.cn

[U07] Py：反转字典键值
来源：https://kz.zhonguo8118.cn

{v: k for k, v in d.items()}
来源：https://rx.zhonguo3118.cn

[U08] Py：展平二维列表
来源：https://zl.zhonguo5118.cn

[y for x in nested for y in x]
来源：https://tk.zhonguo1118.cn

[U09] Py：字典取最大值的键
来源：https://uw.zhonguo5118.cn

max(d, key=d.get)
来源：https://sb.zhonguo7118.cn

[U10] Py：按值排序字典
来源：https://ep.zhonguo5118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://fn.zhonguo5118.cn

[U11] Py：生成器表达式
来源：https://eb.zhonguo8118.cn

(x * 2 for x in arr)
来源：https://fg.zhonguo8118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://kk.zhonguo3118.cn

Counter(arr).most_common(3)
来源：https://jj.zhonguo5118.cn

[U13] Py：固定长度队列
来源：https://gd.zhonguo2118.cn

deque(maxlen=10)
来源：https://nh.zhonguo7118.cn

[U14] Py：分组收集到列表
来源：https://yl.zhonguo5118.cn

defaultdict(list)
来源：https://kx.zhonguo4118.cn

[U15] Py：高精度计时
来源：https://io.zhonguo7118.cn

t = time.perf_counter()
来源：https://ck.zhonguo4118.cn

[U16] Py：命令行参数解析
来源：https://pj.zhonguo3118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://bj.zhonguo7118.cn

[U17] Py：初始化日志
来源：https://fy.zhonguo4118.cn

logging.basicConfig(level=logging.INFO)
来源：https://so.zhonguo7118.cn

[U18] Py：预编译正则
来源：https://cy.zhonguo7118.cn

pat = re.compile(r"\d+")
来源：https://lv.zhonguo1118.cn

[U19] Py：正则替换带回调
来源：https://gj.zhonguo5118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://yl.zhonguo7118.cn

[U20] Py：缓存函数结果
来源：https://hr.zhonguo6118.cn

@functools.lru_cache(maxsize=None)
来源：https://as.zhonguo2118.cn

[U21] Py：自定义上下文管理器
来源：https://hu.zhonguo4118.cn

@contextlib.contextmanager
来源：https://fj.zhonguo2118.cn

[U22] Py：矩阵转置
来源：https://lb.zhonguo1118.cn

list(zip(*m))
来源：https://yq.zhonguo3118.cn

[U23] Py：分块读取大文件
来源：https://mk.zhonguo8118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://zh.zhonguo5118.cn

[U24] Py：路径操作
来源：https://gh.zhonguo6118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://tz.zhonguo8118.cn

[U25] Py：CSV 按字典读
来源：https://pt.zhonguo4118.cn

csv.DictReader(f)
来源：https://ds.zhonguo6118.cn

[U26] Py：并发下载
来源：https://rx.zhonguo4118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://uv.zhonguo8118.cn

[U27] Py：异步 HTTP
来源：https://wj.zhonguo3118.cn

aiohttp.ClientSession() 配合 async with
来源：https://yh.zhonguo8118.cn

[U28] Py：类型别名
来源：https://ff.zhonguo7118.cn

UserId = int
来源：https://fy.zhonguo7118.cn

[U29] Py：属性校验
来源：https://hi.zhonguo2118.cn

@property 与 @x.setter 配合
来源：https://nf.zhonguo1118.cn

[U30] Py：数据类
来源：https://ag.zhonguo8118.cn

@dataclass(slots=True)
来源：https://iv.zhonguo3118.cn

[U31] Py：单测
来源：https://ki.zhonguo5118.cn

python -m pytest -q
来源：https://xh.zhonguo8118.cn

[U32] Py：代码格式化
来源：https://se.zhonguo1118.cn

ruff format . && ruff check --fix .
来源：https://xu.zhonguo6118.cn

[U33] Py：打包发布
来源：https://mr.zhonguo7118.cn

python -m build  （依赖 pyproject.toml）
来源：https://dn.zhonguo4118.cn

[U34] Py：判断编码
来源：https://vs.zhonguo7118.cn

chardet.detect(raw)
来源：https://yg.zhonguo7118.cn

[U35] Py：发送邮件
来源：https://pl.zhonguo3118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://la.zhonguo5118.cn

[U36] Py：定时任务
来源：https://rf.zhonguo3118.cn

schedule.every(10).minutes.do(job)
来源：https://wc.zhonguo5118.cn

[U37] Py：读写 Excel
来源：https://ux.zhonguo4118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://fo.zhonguo4118.cn

[U38] Py：获取脚本所在目录
来源：https://ml.zhonguo7118.cn

Path(__file__).resolve().parent
来源：https://xy.zhonguo4118.cn

[U39] Py：判断是否在交互环境
来源：https://ch.zhonguo8118.cn

sys.stdout.isatty()
来源：https://oa.zhonguo5118.cn

[U40] Py：打印到标准错误
来源：https://my.zhonguo6118.cn

print("err", file=sys.stderr)
来源：https://vn.zhonguo2118.cn

[U41] PHP：初始化 Composer 项目
来源：https://hw.zhonguo7118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://wa.zhonguo3118.cn

[U42] PHP：PSR-4 自动加载
来源：https://rl.zhonguo3118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://dn.zhonguo7118.cn

[U43] PHP：声明命名空间
来源：https://ug.zhonguo3118.cn

namespace App\Http;
来源：https://uf.zhonguo4118.cn

[U44] PHP：开启严格类型
来源：https://ya.zhonguo2118.cn

declare(strict_types=1);
来源：https://uz.zhonguo3118.cn

[U45] PHP：类型声明与返回类型
来源：https://rp.zhonguo5118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://te.zhonguo6118.cn

[U46] PHP：可空类型
来源：https://du.zhonguo3118.cn

?string $name = null
来源：https://tb.zhonguo7118.cn

[U47] PHP：联合类型
来源：https://en.zhonguo3118.cn

int|string $id
来源：https://bi.zhonguo7118.cn

[U48] PHP：纯枚举
来源：https://hk.zhonguo6118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://aa.zhonguo4118.cn

[U49] PHP：只读属性
来源：https://bj.zhonguo5118.cn

public readonly string $name
来源：https://kx.zhonguo5118.cn

[U50] PHP：构造器属性提升
来源：https://gr.zhonguo8118.cn

public function __construct(private int $id) {}
来源：https://qe.zhonguo2118.cn

[U51] PHP：数组解构
来源：https://qt.zhonguo3118.cn

[$a, $b] = $arr;
来源：https://iv.zhonguo6118.cn

[U52] PHP：箭头函数
来源：https://db.zhonguo8118.cn

$double = fn($x) => $x * 2;
来源：https://yb.zhonguo1118.cn

[U53] PHP：空合并运算符
来源：https://sg.zhonguo3118.cn

$v = $a ?? $b ?? "default";
来源：https://rl.zhonguo5118.cn

[U54] PHP：空安全调用
来源：https://ts.zhonguo8118.cn

$obj?->method()
来源：https://rg.zhonguo3118.cn

[U55] PHP：match 表达式
来源：https://kd.zhonguo7118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://lj.zhonguo4118.cn

[U56] PHP：命名参数
来源：https://hq.zhonguo8118.cn

f(a: 1, b: 2)
来源：https://wp.zhonguo8118.cn

[U57] PHP：字符串插值
来源：https://ov.zhonguo3118.cn

"值: {$a}"
来源：https://om.zhonguo8118.cn

[U58] PHP：数组三件套
来源：https://ls.zhonguo5118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://hd.zhonguo2118.cn

[U59] PHP：自定义排序
来源：https://gw.zhonguo7118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://rf.zhonguo3118.cn

[U60] PHP：JSON 编解码
来源：https://kk.zhonguo4118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://bi.zhonguo1118.cn

[U61] PHP：正则
来源：https://os.zhonguo1118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://ff.zhonguo2118.cn

[U62] PHP：日期对象
来源：https://zt.zhonguo7118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://nv.zhonguo2118.cn

[U63] PHP：文件读写
来源：https://ib.zhonguo2118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://ol.zhonguo7118.cn

[U64] PHP：目录遍历
来源：https://gy.zhonguo1118.cn

glob("dir/*.php");  scandir("dir");
来源：https://xp.zhonguo4118.cn

[U65] PHP：会话
来源：https://wo.zhonguo2118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://ku.zhonguo8118.cn

[U66] PHP：设置 Cookie
来源：https://pm.zhonguo7118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://uz.zhonguo8118.cn

[U67] PHP：处理文件上传
来源：https://fp.zhonguo3118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://mi.zhonguo5118.cn

[U68] PHP：PDO 连接
来源：https://ra.zhonguo5118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://il.zhonguo3118.cn

[U69] PHP：PDO 预处理
来源：https://zb.zhonguo7118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://sv.zhonguo2118.cn

[U70] PHP：PDO 事务
来源：https://sr.zhonguo4118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://bk.zhonguo3118.cn

[U71] PHP：抛出异常
来源：https://bi.zhonguo3118.cn

throw new RuntimeException("失败", 500);
来源：https://iw.zhonguo4118.cn

[U72] PHP：写错误日志
来源：https://gd.zhonguo6118.cn

error_log("失败: " . $e->getMessage());
来源：https://ei.zhonguo4118.cn

[U73] PHP：读取 ini 配置
来源：https://uc.zhonguo1118.cn

parse_ini_file("config.ini", true)
来源：https://ll.zhonguo2118.cn

[U74] PHP：读取环境变量
来源：https://mm.zhonguo1118.cn

getenv("APP_ENV") ?: "production"
来源：https://yh.zhonguo1118.cn

[U75] PHP：依赖注入
来源：https://by.zhonguo7118.cn

composer require psr/container
来源：https://or.zhonguo1118.cn

[U76] PHP：简单路由
来源：https://qe.zhonguo1118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://lh.zhonguo2118.cn

[U77] PHP：模板渲染
来源：https://jn.zhonguo3118.cn

composer require twig/twig
来源：https://yq.zhonguo4118.cn

[U78] PHP：单元测试
来源：https://up.zhonguo1118.cn

composer require --dev phpunit/phpunit
来源：https://qd.zhonguo6118.cn

[U79] PHP：静态分析
来源：https://ik.zhonguo3118.cn

composer require --dev phpstan/phpstan
来源：https://fh.zhonguo6118.cn

[U80] PHP：代码规范修复
来源：https://et.zhonguo4118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://wi.zhonguo7118.cn

[U81] JS：初始化项目
来源：https://up.zhonguo1118.cn

npm init -y;  npm i express
来源：https://ii.zhonguo8118.cn

[U82] JS：package.json 脚本
来源：https://gx.zhonguo1118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://wo.zhonguo1118.cn

[U83] JS：ES Module 导入导出
来源：https://my.zhonguo6118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://bp.zhonguo2118.cn

[U84] JS：CommonJS 写法
来源：https://mn.zhonguo4118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://qw.zhonguo8118.cn

[U85] JS：可选链
来源：https://xe.zhonguo8118.cn

a?.b?.c
来源：https://jz.zhonguo3118.cn

[U86] JS：空值合并
来源：https://za.zhonguo5118.cn

a ?? b
来源：https://zc.zhonguo8118.cn

[U87] JS：解构默认值
来源：https://wi.zhonguo4118.cn

const { a = 1, b = 2 } = obj;
来源：https://pf.zhonguo2118.cn

[U88] JS：对象展开合并
来源：https://po.zhonguo7118.cn

{ ...a, ...b }
来源：https://ar.zhonguo8118.cn

[U89] JS：数组去重
来源：https://lz.zhonguo7118.cn

[...new Set(arr)]
来源：https://ik.zhonguo2118.cn

[U90] JS：数字数组排序
来源：https://ww.zhonguo7118.cn

[...arr].sort((a, b) => a - b)
来源：https://np.zhonguo6118.cn

[U91] JS：对象键值遍历
来源：https://wo.zhonguo3118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://cp.zhonguo6118.cn

[U92] JS：深拷贝
来源：https://cn.zhonguo1118.cn

structuredClone(obj)
来源：https://qy.zhonguo4118.cn

[U93] JS：模板字符串
来源：https://nz.zhonguo5118.cn

`共 ${n} 条`
来源：https://is.zhonguo6118.cn

[U94] JS：箭头函数
来源：https://oj.zhonguo4118.cn

const double = x => x * 2;
来源：https://pe.zhonguo3118.cn

[U95] JS：Promise 包装
来源：https://rp.zhonguo4118.cn

new Promise((resolve, reject) => {})
来源：https://qm.zhonguo5118.cn

[U96] JS：async/await 与异常
来源：https://ii.zhonguo8118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://md.zhonguo2118.cn

[U97] JS：并发请求
来源：https://ie.zhonguo6118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://cw.zhonguo1118.cn

[U98] JS：fetch 带 JSON
来源：https://kg.zhonguo6118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://bg.zhonguo4118.cn


<!-- 参考信息 -->