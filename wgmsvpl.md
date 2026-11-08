代发 wailian999

[T13] Kotlin：只读 Map
来源：https://tj.zhonguo1118.cn

val m = mapOf("a" to 1)
来源：https://fk.zhonguo2118.cn

[T14] Kotlin：循环
来源：https://dw.zhonguo7118.cn

for (i in 1..10) println(i)
来源：https://sc.zhonguo6118.cn

[T15] Kotlin：接口
来源：https://el.zhonguo7118.cn

interface Shape { fun area(): Double }
来源：https://qv.zhonguo2118.cn

[T16] Swift：Hello World
来源：https://sp.zhonguo3118.cn

print("Hello")
来源：https://kv.zhonguo1118.cn

[T17] Swift：变量与常量
来源：https://im.zhonguo6118.cn

var a = 1;  let b = 2
来源：https://cl.zhonguo7118.cn

[T18] Swift：字符串插值
来源：https://fy.zhonguo6118.cn

"值: \(b)"
来源：https://bv.zhonguo6118.cn

[T19] Swift：可选绑定
来源：https://ms.zhonguo1118.cn

if let n = opt { print(n) }
来源：https://xo.zhonguo2118.cn

[T20] Swift：数组操作
来源：https://ry.zhonguo6118.cn

var a = [1, 2, 3];  a.append(4)
来源：https://pb.zhonguo8118.cn

[T21] Swift：遍历
来源：https://su.zhonguo1118.cn

for x in a { print(x) }
来源：https://tn.zhonguo3118.cn

[T22] Swift：字典
来源：https://mb.zhonguo1118.cn

var d = ["a": 1];  d["b"] = 2
来源：https://zn.zhonguo4118.cn

[T23] Swift：函数
来源：https://mm.zhonguo6118.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：https://pd.zhonguo3118.cn

[T24] Swift：闭包
来源：https://mn.zhonguo7118.cn

let f = { (x: Int) -> Int in x * 2 }
来源：https://lo.zhonguo8118.cn

[T25] Swift：结构体
来源：https://pi.zhonguo2118.cn

struct P { var x: Int }
来源：https://pa.zhonguo3118.cn

[T26] Swift：类与重写
来源：https://oe.zhonguo7118.cn

class A: Base { override func f() {} }
来源：https://zc.zhonguo4118.cn

[T27] Swift：错误处理
来源：https://bj.zhonguo7118.cn

do { try f() } catch { print(error) }
来源：https://ad.zhonguo3118.cn

[T28] Swift：枚举
来源：https://cj.zhonguo8118.cn

enum Color { case red, green }
来源：https://dg.zhonguo5118.cn

[T29] Swift：guard 提前返回
来源：https://xe.zhonguo2118.cn

guard let x = opt else { return }
来源：https://dv.zhonguo3118.cn

[T30] Swift：协议
来源：https://mm.zhonguo2118.cn

protocol Shape { func area() -> Double }
来源：https://db.zhonguo4118.cn

[T31] Lua：Hello World
来源：https://bg.zhonguo5118.cn

print("Hello")
来源：https://gc.zhonguo3118.cn

[T32] Lua：局部变量
来源：https://sp.zhonguo1118.cn

local a = 1
来源：https://ln.zhonguo8118.cn

[T33] Lua：表（数组）
来源：https://xe.zhonguo4118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://qn.zhonguo2118.cn

[T34] Lua：遍历表
来源：https://lu.zhonguo3118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://nz.zhonguo6118.cn

[T35] Lua：字典表
来源：https://pi.zhonguo8118.cn

local d = { a = 1 };  d.b = 2
来源：https://tw.zhonguo2118.cn

[T36] Lua：函数
来源：https://pq.zhonguo8118.cn

function add(a, b) return a + b end
来源：https://mc.zhonguo8118.cn

[T37] Lua：字符串拼接
来源：https://qb.zhonguo7118.cn

"a" .. "b"
来源：https://mo.zhonguo3118.cn

[T38] Lua：条件
来源：https://hp.zhonguo1118.cn

if x > 0 then print("正") end
来源：https://df.zhonguo6118.cn

[T39] Lua：模式匹配
来源：https://ws.zhonguo4118.cn

string.find(s, "%d+")
来源：https://tp.zhonguo3118.cn

[T40] Lua：元表
来源：https://eu.zhonguo8118.cn

setmetatable({}, { __index = base })
来源：https://ak.zhonguo3118.cn

[T41] Perl：Hello World
来源：https://pr.zhonguo1118.cn

print "Hello\n";
来源：https://bx.zhonguo6118.cn

[T42] Perl：变量类型
来源：https://zk.zhonguo7118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://ov.zhonguo6118.cn

[T43] Perl：字符串插值
来源：https://ia.zhonguo1118.cn

"值: $a"
来源：https://eq.zhonguo1118.cn

[T44] Perl：条件
来源：https://ph.zhonguo8118.cn

if ($a > 0) { print "正"; }
来源：https://gs.zhonguo8118.cn

[T45] Perl：数组遍历
来源：https://yd.zhonguo1118.cn

for my $x (@arr) { print $x; }
来源：https://lt.zhonguo1118.cn

[T46] Perl：哈希操作
来源：https://wx.zhonguo5118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://ka.zhonguo6118.cn

[T47] Perl：正则捕获
来源：https://zf.zhonguo8118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://vp.zhonguo3118.cn

[T48] Perl：正则替换
来源：https://lr.zhonguo1118.cn

$s =~ s/old/new/g;
来源：https://fo.zhonguo4118.cn

[T49] Perl：函数
来源：https://yh.zhonguo3118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://rk.zhonguo3118.cn

[T50] Perl：逐行读文件
来源：https://pu.zhonguo6118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://kg.zhonguo5118.cn

while (my $line = <$fh>) { print $line; }
来源：https://en.zhonguo6118.cn

[T51] Scala：Hello World
来源：https://qd.zhonguo2118.cn

println("Hello")
来源：https://yn.zhonguo2118.cn

[T52] Scala：变量
来源：https://lq.zhonguo7118.cn

val a = 1;  var b = 2
来源：https://ch.zhonguo3118.cn

[T53] Scala：字符串插值
来源：https://np.zhonguo6118.cn

s"值: $b"
来源：https://vz.zhonguo7118.cn

[T54] Scala：集合映射
来源：https://ti.zhonguo3118.cn

List(1, 2, 3).map(_ * 2)
来源：https://yo.zhonguo6118.cn

[T55] Scala：集合过滤
来源：https://vy.zhonguo5118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://az.zhonguo1118.cn

[T56] Scala：样例类
来源：https://rh.zhonguo5118.cn

case class User(name: String, age: Int)
来源：https://xg.zhonguo4118.cn

[T57] Scala：模式匹配
来源：https://dd.zhonguo1118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://fo.zhonguo3118.cn

[T58] Scala：函数定义
来源：https://ri.zhonguo5118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://cx.zhonguo6118.cn

[T59] Scala：循环
来源：https://aj.zhonguo8118.cn

for (i <- 1 to 10) println(i)
来源：https://wv.zhonguo1118.cn

[T60] Scala：折叠
来源：https://vy.zhonguo7118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://nw.zhonguo4118.cn

================================================================================
来源：https://ve.zhonguo4118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://no.zhonguo5118.cn

================================================================================
来源：https://os.zhonguo1118.cn

[U01] Py：创建虚拟环境
来源：https://ar.zhonguo8118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://he.zhonguo7118.cn

[U02] Py：导出 / 安装依赖
来源：https://mi.zhonguo8118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://je.zhonguo6118.cn

[U03] Py：加载 .env 配置
来源：https://bf.zhonguo7118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://ij.zhonguo2118.cn

[U04] Py：变量调试打印
来源：https://ho.zhonguo4118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://ov.zhonguo5118.cn

[U05] Py：列表去重且保序
来源：https://oz.zhonguo3118.cn

list(dict.fromkeys(arr))
来源：https://kk.zhonguo2118.cn

[U06] Py：合并两个字典
来源：https://lg.zhonguo3118.cn

{**a, **b}
来源：https://ye.zhonguo6118.cn

[U07] Py：反转字典键值
来源：https://pj.zhonguo1118.cn

{v: k for k, v in d.items()}
来源：https://gi.zhonguo8118.cn

[U08] Py：展平二维列表
来源：https://ow.zhonguo8118.cn

[y for x in nested for y in x]
来源：https://si.zhonguo3118.cn

[U09] Py：字典取最大值的键
来源：https://af.zhonguo6118.cn

max(d, key=d.get)
来源：https://wc.zhonguo8118.cn

[U10] Py：按值排序字典
来源：https://ad.zhonguo3118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://eb.zhonguo1118.cn

[U11] Py：生成器表达式
来源：https://sy.zhonguo5118.cn

(x * 2 for x in arr)
来源：https://ne.zhonguo5118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://fi.zhonguo6118.cn

Counter(arr).most_common(3)
来源：https://fx.zhonguo6118.cn

[U13] Py：固定长度队列
来源：https://vf.zhonguo6118.cn

deque(maxlen=10)
来源：https://ql.zhonguo5118.cn

[U14] Py：分组收集到列表
来源：https://mi.zhonguo4118.cn

defaultdict(list)
来源：https://ei.zhonguo8118.cn

[U15] Py：高精度计时
来源：https://ek.zhonguo5118.cn

t = time.perf_counter()
来源：https://ht.zhonguo5118.cn

[U16] Py：命令行参数解析
来源：https://ri.zhonguo4118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://cj.zhonguo8118.cn

[U17] Py：初始化日志
来源：https://ru.zhonguo3118.cn

logging.basicConfig(level=logging.INFO)
来源：https://hf.zhonguo7118.cn

[U18] Py：预编译正则
来源：https://zc.zhonguo5118.cn

pat = re.compile(r"\d+")
来源：https://co.zhonguo4118.cn

[U19] Py：正则替换带回调
来源：https://vu.zhonguo3118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://wl.zhonguo8118.cn

[U20] Py：缓存函数结果
来源：https://io.zhonguo8118.cn

@functools.lru_cache(maxsize=None)
来源：https://ey.zhonguo3118.cn

[U21] Py：自定义上下文管理器
来源：https://sk.zhonguo2118.cn

@contextlib.contextmanager
来源：https://vw.zhonguo8118.cn

[U22] Py：矩阵转置
来源：https://kn.zhonguo5118.cn

list(zip(*m))
来源：https://ja.zhonguo4118.cn

[U23] Py：分块读取大文件
来源：https://vu.zhonguo3118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://fg.zhonguo3118.cn

[U24] Py：路径操作
来源：https://ld.zhonguo8118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://as.zhonguo1118.cn

[U25] Py：CSV 按字典读
来源：https://cm.zhonguo5118.cn

csv.DictReader(f)
来源：https://zo.zhonguo2118.cn

[U26] Py：并发下载
来源：https://kc.zhonguo7118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://wq.zhonguo2118.cn

[U27] Py：异步 HTTP
来源：https://ir.zhonguo5118.cn

aiohttp.ClientSession() 配合 async with
来源：https://iw.zhonguo5118.cn

[U28] Py：类型别名
来源：https://fc.zhonguo2118.cn

UserId = int
来源：https://uh.zhonguo4118.cn

[U29] Py：属性校验
来源：https://xq.zhonguo1118.cn

@property 与 @x.setter 配合
来源：https://vs.zhonguo4118.cn

[U30] Py：数据类
来源：https://iw.zhonguo3118.cn

@dataclass(slots=True)
来源：https://nu.zhonguo1118.cn

[U31] Py：单测
来源：https://jx.zhonguo6118.cn

python -m pytest -q
来源：https://mk.zhonguo8118.cn

[U32] Py：代码格式化
来源：https://pq.zhonguo5118.cn

ruff format . && ruff check --fix .
来源：https://wb.zhonguo6118.cn

[U33] Py：打包发布
来源：https://fw.zhonguo8118.cn

python -m build  （依赖 pyproject.toml）
来源：https://qa.zhonguo1118.cn

[U34] Py：判断编码
来源：https://gg.zhonguo7118.cn

chardet.detect(raw)
来源：https://az.zhonguo1118.cn

[U35] Py：发送邮件
来源：https://vp.zhonguo1118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://yh.zhonguo6118.cn

[U36] Py：定时任务
来源：https://dz.zhonguo6118.cn

schedule.every(10).minutes.do(job)
来源：https://vu.zhonguo4118.cn

[U37] Py：读写 Excel
来源：https://he.zhonguo8118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://ws.zhonguo7118.cn

[U38] Py：获取脚本所在目录
来源：https://dh.zhonguo6118.cn

Path(__file__).resolve().parent
来源：https://kx.zhonguo6118.cn

[U39] Py：判断是否在交互环境
来源：https://or.zhonguo3118.cn

sys.stdout.isatty()
来源：https://rf.zhonguo7118.cn

[U40] Py：打印到标准错误
来源：https://cc.zhonguo8118.cn

print("err", file=sys.stderr)
来源：https://yn.zhonguo7118.cn

[U41] PHP：初始化 Composer 项目
来源：https://fn.zhonguo5118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://px.zhonguo1118.cn

[U42] PHP：PSR-4 自动加载
来源：https://vh.zhonguo7118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://ro.zhonguo3118.cn

[U43] PHP：声明命名空间
来源：https://kq.zhonguo6118.cn

namespace App\Http;
来源：https://ew.zhonguo2118.cn

[U44] PHP：开启严格类型
来源：https://rb.zhonguo1118.cn

declare(strict_types=1);
来源：https://ie.zhonguo6118.cn

[U45] PHP：类型声明与返回类型
来源：https://wi.zhonguo5118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://pt.zhonguo7118.cn

[U46] PHP：可空类型
来源：https://bs.zhonguo2118.cn

?string $name = null
来源：https://ju.zhonguo2118.cn

[U47] PHP：联合类型
来源：https://vn.zhonguo5118.cn

int|string $id
来源：https://nc.zhonguo8118.cn

[U48] PHP：纯枚举
来源：https://dn.zhonguo8118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://wv.zhonguo3118.cn

[U49] PHP：只读属性
来源：https://rf.zhonguo5118.cn

public readonly string $name
来源：https://oe.zhonguo3118.cn

[U50] PHP：构造器属性提升
来源：https://yp.zhonguo1118.cn

public function __construct(private int $id) {}
来源：https://hg.zhonguo7118.cn

[U51] PHP：数组解构
来源：https://vq.zhonguo2118.cn

[$a, $b] = $arr;
来源：https://xt.zhonguo7118.cn

[U52] PHP：箭头函数
来源：https://li.zhonguo1118.cn

$double = fn($x) => $x * 2;
来源：https://lk.zhonguo6118.cn

[U53] PHP：空合并运算符
来源：https://ft.zhonguo8118.cn

$v = $a ?? $b ?? "default";
来源：https://uz.zhonguo8118.cn

[U54] PHP：空安全调用
来源：https://bf.zhonguo6118.cn

$obj?->method()
来源：https://of.zhonguo6118.cn

[U55] PHP：match 表达式
来源：https://wg.zhonguo8118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://of.zhonguo3118.cn

[U56] PHP：命名参数
来源：https://af.zhonguo8118.cn

f(a: 1, b: 2)
来源：https://qk.zhonguo6118.cn

[U57] PHP：字符串插值
来源：https://xs.zhonguo1118.cn

"值: {$a}"
来源：https://ik.zhonguo4118.cn

[U58] PHP：数组三件套
来源：https://aw.zhonguo7118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://dx.zhonguo6118.cn

[U59] PHP：自定义排序
来源：https://fa.zhonguo5118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://mm.zhonguo3118.cn

[U60] PHP：JSON 编解码
来源：https://te.zhonguo4118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://ji.zhonguo5118.cn

[U61] PHP：正则
来源：https://wc.zhonguo7118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://hu.zhonguo2118.cn

[U62] PHP：日期对象
来源：https://ma.zhonguo2118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://ug.zhonguo6118.cn

[U63] PHP：文件读写
来源：https://da.zhonguo2118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://yr.zhonguo7118.cn

[U64] PHP：目录遍历
来源：https://tn.zhonguo4118.cn

glob("dir/*.php");  scandir("dir");
来源：https://io.zhonguo7118.cn

[U65] PHP：会话
来源：https://ho.zhonguo2118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://sc.zhonguo7118.cn

[U66] PHP：设置 Cookie
来源：https://bw.zhonguo2118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://jj.zhonguo2118.cn

[U67] PHP：处理文件上传
来源：https://dj.zhonguo2118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://zs.zhonguo1118.cn

[U68] PHP：PDO 连接
来源：https://wp.zhonguo3118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://ga.zhonguo4118.cn

[U69] PHP：PDO 预处理
来源：https://ai.zhonguo2118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://vm.zhonguo1118.cn

[U70] PHP：PDO 事务
来源：https://dv.zhonguo3118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://js.zhonguo6118.cn

[U71] PHP：抛出异常
来源：https://ld.zhonguo8118.cn

throw new RuntimeException("失败", 500);
来源：https://ki.zhonguo3118.cn

[U72] PHP：写错误日志
来源：https://ql.zhonguo5118.cn

error_log("失败: " . $e->getMessage());
来源：https://tc.zhonguo8118.cn

[U73] PHP：读取 ini 配置
来源：https://bc.zhonguo7118.cn

parse_ini_file("config.ini", true)
来源：https://wg.zhonguo5118.cn

[U74] PHP：读取环境变量
来源：https://un.zhonguo8118.cn

getenv("APP_ENV") ?: "production"
来源：https://bh.zhonguo8118.cn

[U75] PHP：依赖注入
来源：https://uv.zhonguo2118.cn

composer require psr/container
来源：https://cy.zhonguo7118.cn

[U76] PHP：简单路由
来源：https://jo.zhonguo5118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://zs.zhonguo2118.cn

[U77] PHP：模板渲染
来源：https://jq.zhonguo8118.cn

composer require twig/twig
来源：https://sf.zhonguo7118.cn

[U78] PHP：单元测试
来源：https://kq.zhonguo5118.cn

composer require --dev phpunit/phpunit
来源：https://vo.zhonguo5118.cn

[U79] PHP：静态分析
来源：https://id.zhonguo4118.cn

composer require --dev phpstan/phpstan
来源：https://sj.zhonguo1118.cn

[U80] PHP：代码规范修复
来源：https://uo.zhonguo4118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://pg.zhonguo1118.cn

[U81] JS：初始化项目
来源：https://yx.zhonguo1118.cn

npm init -y;  npm i express
来源：https://is.zhonguo5118.cn

[U82] JS：package.json 脚本
来源：https://ew.zhonguo1118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://pb.zhonguo1118.cn

[U83] JS：ES Module 导入导出
来源：https://ym.zhonguo4118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://ab.zhonguo3118.cn

[U84] JS：CommonJS 写法
来源：https://vq.zhonguo3118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://xr.zhonguo1118.cn

[U85] JS：可选链
来源：https://sc.zhonguo6118.cn

a?.b?.c
来源：https://vo.zhonguo7118.cn

[U86] JS：空值合并
来源：https://bw.zhonguo8118.cn

a ?? b
来源：https://lu.zhonguo6118.cn

[U87] JS：解构默认值
来源：https://vc.zhonguo5118.cn

const { a = 1, b = 2 } = obj;
来源：https://ch.zhonguo7118.cn

[U88] JS：对象展开合并
来源：https://rr.zhonguo1118.cn

{ ...a, ...b }
来源：https://ob.zhonguo3118.cn

[U89] JS：数组去重
来源：https://pv.zhonguo1118.cn

[...new Set(arr)]
来源：https://tp.zhonguo2118.cn

[U90] JS：数字数组排序
来源：https://qe.zhonguo7118.cn

[...arr].sort((a, b) => a - b)
来源：https://ea.zhonguo8118.cn

[U91] JS：对象键值遍历
来源：https://gc.zhonguo8118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://xz.zhonguo3118.cn

[U92] JS：深拷贝
来源：https://qv.zhonguo8118.cn

structuredClone(obj)
来源：https://nx.zhonguo5118.cn

[U93] JS：模板字符串
来源：https://kz.zhonguo8118.cn

`共 ${n} 条`
来源：https://ld.zhonguo3118.cn

[U94] JS：箭头函数
来源：https://xk.zhonguo1118.cn

const double = x => x * 2;
来源：https://qj.zhonguo8118.cn

[U95] JS：Promise 包装
来源：https://nw.zhonguo4118.cn

new Promise((resolve, reject) => {})
来源：https://ni.zhonguo6118.cn

[U96] JS：async/await 与异常
来源：https://cy.zhonguo1118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://gq.zhonguo6118.cn

[U97] JS：并发请求
来源：https://jn.zhonguo6118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://io.zhonguo4118.cn

[U98] JS：fetch 带 JSON
来源：https://pv.zhonguo7118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://ti.zhonguo4118.cn

[U99] JS：事件监听
来源：https://gb.zhonguo6118.cn

el.addEventListener("click", e => {})
来源：https://hq.zhonguo2118.cn

[U100] JS：DOM 查询
来源：https://vp.zhonguo5118.cn

document.querySelector(".item")
来源：https://md.zhonguo6118.cn


<!-- 参考信息 -->