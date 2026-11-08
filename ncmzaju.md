代发 wailian999

[T25] Swift：结构体
来源：https://nh.zhonguo6118.cn

struct P { var x: Int }
来源：https://oo.zhonguo4118.cn

[T26] Swift：类与重写
来源：https://ei.zhonguo3118.cn

class A: Base { override func f() {} }
来源：https://ec.zhonguo5118.cn

[T27] Swift：错误处理
来源：https://bb.zhonguo7118.cn

do { try f() } catch { print(error) }
来源：https://wt.zhonguo6118.cn

[T28] Swift：枚举
来源：https://st.zhonguo2118.cn

enum Color { case red, green }
来源：https://zl.zhonguo6118.cn

[T29] Swift：guard 提前返回
来源：https://hv.zhonguo1118.cn

guard let x = opt else { return }
来源：https://ac.zhonguo8118.cn

[T30] Swift：协议
来源：https://nh.zhonguo1118.cn

protocol Shape { func area() -> Double }
来源：https://yk.zhonguo5118.cn

[T31] Lua：Hello World
来源：https://lw.zhonguo4118.cn

print("Hello")
来源：https://za.zhonguo6118.cn

[T32] Lua：局部变量
来源：https://fp.zhonguo3118.cn

local a = 1
来源：https://rx.zhonguo5118.cn

[T33] Lua：表（数组）
来源：https://my.zhonguo1118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://et.zhonguo6118.cn

[T34] Lua：遍历表
来源：https://ip.zhonguo7118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://mh.zhonguo3118.cn

[T35] Lua：字典表
来源：https://wp.zhonguo3118.cn

local d = { a = 1 };  d.b = 2
来源：https://wr.zhonguo7118.cn

[T36] Lua：函数
来源：https://zf.zhonguo6118.cn

function add(a, b) return a + b end
来源：https://zg.zhonguo2118.cn

[T37] Lua：字符串拼接
来源：https://lo.zhonguo6118.cn

"a" .. "b"
来源：https://nc.zhonguo1118.cn

[T38] Lua：条件
来源：https://xd.zhonguo3118.cn

if x > 0 then print("正") end
来源：https://cz.zhonguo8118.cn

[T39] Lua：模式匹配
来源：https://vf.zhonguo7118.cn

string.find(s, "%d+")
来源：https://fv.zhonguo1118.cn

[T40] Lua：元表
来源：https://jl.zhonguo3118.cn

setmetatable({}, { __index = base })
来源：https://ac.zhonguo6118.cn

[T41] Perl：Hello World
来源：https://mu.zhonguo4118.cn

print "Hello\n";
来源：https://mh.zhonguo4118.cn

[T42] Perl：变量类型
来源：https://yw.zhonguo8118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://uf.zhonguo2118.cn

[T43] Perl：字符串插值
来源：https://di.zhonguo3118.cn

"值: $a"
来源：https://xw.zhonguo2118.cn

[T44] Perl：条件
来源：https://pa.zhonguo6118.cn

if ($a > 0) { print "正"; }
来源：https://mr.zhonguo1118.cn

[T45] Perl：数组遍历
来源：https://pl.zhonguo7118.cn

for my $x (@arr) { print $x; }
来源：https://js.zhonguo2118.cn

[T46] Perl：哈希操作
来源：https://bp.zhonguo4118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://bq.zhonguo8118.cn

[T47] Perl：正则捕获
来源：https://eu.zhonguo2118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://ct.zhonguo7118.cn

[T48] Perl：正则替换
来源：https://gh.zhonguo5118.cn

$s =~ s/old/new/g;
来源：https://aq.zhonguo6118.cn

[T49] Perl：函数
来源：https://gv.zhonguo7118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://qf.zhonguo8118.cn

[T50] Perl：逐行读文件
来源：https://xj.zhonguo1118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://rn.zhonguo8118.cn

while (my $line = <$fh>) { print $line; }
来源：https://df.zhonguo2118.cn

[T51] Scala：Hello World
来源：https://gc.zhonguo8118.cn

println("Hello")
来源：https://ck.zhonguo6118.cn

[T52] Scala：变量
来源：https://ig.zhonguo3118.cn

val a = 1;  var b = 2
来源：https://mc.zhonguo4118.cn

[T53] Scala：字符串插值
来源：https://vw.zhonguo6118.cn

s"值: $b"
来源：https://ee.zhonguo1118.cn

[T54] Scala：集合映射
来源：https://av.zhonguo8118.cn

List(1, 2, 3).map(_ * 2)
来源：https://pi.zhonguo6118.cn

[T55] Scala：集合过滤
来源：https://nm.zhonguo4118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://zb.zhonguo7118.cn

[T56] Scala：样例类
来源：https://bd.zhonguo4118.cn

case class User(name: String, age: Int)
来源：https://fp.zhonguo4118.cn

[T57] Scala：模式匹配
来源：https://da.zhonguo1118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://fj.zhonguo7118.cn

[T58] Scala：函数定义
来源：https://iy.zhonguo3118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://yr.zhonguo3118.cn

[T59] Scala：循环
来源：https://vh.zhonguo8118.cn

for (i <- 1 to 10) println(i)
来源：https://uq.zhonguo4118.cn

[T60] Scala：折叠
来源：https://gh.zhonguo6118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://uk.zhonguo2118.cn

================================================================================
来源：https://gj.zhonguo3118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://qn.zhonguo8118.cn

================================================================================
来源：https://rb.zhonguo2118.cn

[U01] Py：创建虚拟环境
来源：https://gz.zhonguo3118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://zi.zhonguo6118.cn

[U02] Py：导出 / 安装依赖
来源：https://sq.zhonguo5118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://uf.zhonguo8118.cn

[U03] Py：加载 .env 配置
来源：https://wt.zhonguo1118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://dj.zhonguo1118.cn

[U04] Py：变量调试打印
来源：https://ds.zhonguo6118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://uy.zhonguo6118.cn

[U05] Py：列表去重且保序
来源：https://lb.zhonguo4118.cn

list(dict.fromkeys(arr))
来源：https://bf.zhonguo1118.cn

[U06] Py：合并两个字典
来源：https://dy.zhonguo2118.cn

{**a, **b}
来源：https://xg.zhonguo3118.cn

[U07] Py：反转字典键值
来源：https://ut.zhonguo8118.cn

{v: k for k, v in d.items()}
来源：https://li.zhonguo7118.cn

[U08] Py：展平二维列表
来源：https://fz.zhonguo5118.cn

[y for x in nested for y in x]
来源：https://es.zhonguo8118.cn

[U09] Py：字典取最大值的键
来源：https://lw.zhonguo2118.cn

max(d, key=d.get)
来源：https://dj.zhonguo7118.cn

[U10] Py：按值排序字典
来源：https://xs.zhonguo3118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://he.zhonguo1118.cn

[U11] Py：生成器表达式
来源：https://hy.zhonguo5118.cn

(x * 2 for x in arr)
来源：https://gu.zhonguo4118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://ng.zhonguo4118.cn

Counter(arr).most_common(3)
来源：https://iq.zhonguo7118.cn

[U13] Py：固定长度队列
来源：https://yn.zhonguo8118.cn

deque(maxlen=10)
来源：https://zk.zhonguo8118.cn

[U14] Py：分组收集到列表
来源：https://vc.zhonguo2118.cn

defaultdict(list)
来源：https://na.zhonguo3118.cn

[U15] Py：高精度计时
来源：https://wd.zhonguo7118.cn

t = time.perf_counter()
来源：https://mu.zhonguo8118.cn

[U16] Py：命令行参数解析
来源：https://ec.zhonguo5118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://tr.zhonguo4118.cn

[U17] Py：初始化日志
来源：https://rn.zhonguo8118.cn

logging.basicConfig(level=logging.INFO)
来源：https://py.zhonguo7118.cn

[U18] Py：预编译正则
来源：https://go.zhonguo6118.cn

pat = re.compile(r"\d+")
来源：https://zj.zhonguo2118.cn

[U19] Py：正则替换带回调
来源：https://tt.zhonguo4118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://ix.zhonguo7118.cn

[U20] Py：缓存函数结果
来源：https://dm.zhonguo6118.cn

@functools.lru_cache(maxsize=None)
来源：https://mq.zhonguo4118.cn

[U21] Py：自定义上下文管理器
来源：https://fn.zhonguo3118.cn

@contextlib.contextmanager
来源：https://pe.zhonguo5118.cn

[U22] Py：矩阵转置
来源：https://yt.zhonguo8118.cn

list(zip(*m))
来源：https://kx.zhonguo3118.cn

[U23] Py：分块读取大文件
来源：https://cr.zhonguo6118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://mu.zhonguo5118.cn

[U24] Py：路径操作
来源：https://ak.zhonguo5118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://sb.zhonguo5118.cn

[U25] Py：CSV 按字典读
来源：https://aj.zhonguo7118.cn

csv.DictReader(f)
来源：https://mx.zhonguo3118.cn

[U26] Py：并发下载
来源：https://sz.zhonguo5118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://lc.zhonguo1118.cn

[U27] Py：异步 HTTP
来源：https://sa.zhonguo8118.cn

aiohttp.ClientSession() 配合 async with
来源：https://yy.zhonguo4118.cn

[U28] Py：类型别名
来源：https://qt.zhonguo8118.cn

UserId = int
来源：https://mp.zhonguo2118.cn

[U29] Py：属性校验
来源：https://ct.zhonguo1118.cn

@property 与 @x.setter 配合
来源：https://oe.zhonguo5118.cn

[U30] Py：数据类
来源：https://wj.zhonguo3118.cn

@dataclass(slots=True)
来源：https://zv.zhonguo5118.cn

[U31] Py：单测
来源：https://ws.zhonguo2118.cn

python -m pytest -q
来源：https://bi.zhonguo1118.cn

[U32] Py：代码格式化
来源：https://hb.zhonguo3118.cn

ruff format . && ruff check --fix .
来源：https://jl.zhonguo2118.cn

[U33] Py：打包发布
来源：https://sn.zhonguo8118.cn

python -m build  （依赖 pyproject.toml）
来源：https://lu.zhonguo4118.cn

[U34] Py：判断编码
来源：https://vr.zhonguo3118.cn

chardet.detect(raw)
来源：https://xv.zhonguo6118.cn

[U35] Py：发送邮件
来源：https://je.zhonguo8118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://ct.zhonguo8118.cn

[U36] Py：定时任务
来源：https://qj.zhonguo4118.cn

schedule.every(10).minutes.do(job)
来源：https://ma.zhonguo7118.cn

[U37] Py：读写 Excel
来源：https://ht.zhonguo5118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://aa.zhonguo8118.cn

[U38] Py：获取脚本所在目录
来源：https://sm.zhonguo3118.cn

Path(__file__).resolve().parent
来源：https://mt.zhonguo4118.cn

[U39] Py：判断是否在交互环境
来源：https://za.zhonguo6118.cn

sys.stdout.isatty()
来源：https://zf.zhonguo3118.cn

[U40] Py：打印到标准错误
来源：https://fl.zhonguo7118.cn

print("err", file=sys.stderr)
来源：https://xk.zhonguo6118.cn

[U41] PHP：初始化 Composer 项目
来源：https://ts.zhonguo1118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://ei.zhonguo3118.cn

[U42] PHP：PSR-4 自动加载
来源：https://rc.zhonguo8118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://ol.zhonguo5118.cn

[U43] PHP：声明命名空间
来源：https://vw.zhonguo8118.cn

namespace App\Http;
来源：https://fo.zhonguo2118.cn

[U44] PHP：开启严格类型
来源：https://jm.zhonguo8118.cn

declare(strict_types=1);
来源：https://jq.zhonguo3118.cn

[U45] PHP：类型声明与返回类型
来源：https://pb.zhonguo1118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://uc.zhonguo8118.cn

[U46] PHP：可空类型
来源：https://ad.zhonguo4118.cn

?string $name = null
来源：https://nd.zhonguo8118.cn

[U47] PHP：联合类型
来源：https://vf.zhonguo5118.cn

int|string $id
来源：https://oe.zhonguo8118.cn

[U48] PHP：纯枚举
来源：https://rn.zhonguo4118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://nl.zhonguo6118.cn

[U49] PHP：只读属性
来源：https://uh.zhonguo4118.cn

public readonly string $name
来源：https://gc.zhonguo5118.cn

[U50] PHP：构造器属性提升
来源：https://px.zhonguo7118.cn

public function __construct(private int $id) {}
来源：https://se.zhonguo4118.cn

[U51] PHP：数组解构
来源：https://py.zhonguo6118.cn

[$a, $b] = $arr;
来源：https://uw.zhonguo7118.cn

[U52] PHP：箭头函数
来源：https://sv.zhonguo4118.cn

$double = fn($x) => $x * 2;
来源：https://qj.zhonguo1118.cn

[U53] PHP：空合并运算符
来源：https://yb.zhonguo2118.cn

$v = $a ?? $b ?? "default";
来源：https://ks.zhonguo5118.cn

[U54] PHP：空安全调用
来源：https://hv.zhonguo4118.cn

$obj?->method()
来源：https://yl.zhonguo4118.cn

[U55] PHP：match 表达式
来源：https://nb.zhonguo7118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://lk.zhonguo8118.cn

[U56] PHP：命名参数
来源：https://xm.zhonguo6118.cn

f(a: 1, b: 2)
来源：https://qw.zhonguo3118.cn

[U57] PHP：字符串插值
来源：https://al.zhonguo1118.cn

"值: {$a}"
来源：https://rq.zhonguo7118.cn

[U58] PHP：数组三件套
来源：https://mi.zhonguo7118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://zz.zhonguo3118.cn

[U59] PHP：自定义排序
来源：https://df.zhonguo6118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://fe.zhonguo8118.cn

[U60] PHP：JSON 编解码
来源：https://dx.zhonguo6118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://nx.zhonguo6118.cn

[U61] PHP：正则
来源：https://xk.zhonguo2118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://ca.zhonguo7118.cn

[U62] PHP：日期对象
来源：https://kf.zhonguo3118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://yo.zhonguo8118.cn

[U63] PHP：文件读写
来源：https://zg.zhonguo1118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://ep.zhonguo5118.cn

[U64] PHP：目录遍历
来源：https://bl.zhonguo7118.cn

glob("dir/*.php");  scandir("dir");
来源：https://ir.zhonguo6118.cn

[U65] PHP：会话
来源：https://qh.zhonguo1118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://zh.zhonguo1118.cn

[U66] PHP：设置 Cookie
来源：https://pn.zhonguo7118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://kt.zhonguo7118.cn

[U67] PHP：处理文件上传
来源：https://tt.zhonguo4118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://au.zhonguo4118.cn

[U68] PHP：PDO 连接
来源：https://je.zhonguo5118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://cx.zhonguo2118.cn

[U69] PHP：PDO 预处理
来源：https://ix.zhonguo4118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://eh.zhonguo6118.cn

[U70] PHP：PDO 事务
来源：https://pv.zhonguo8118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://ex.zhonguo3118.cn

[U71] PHP：抛出异常
来源：https://ka.zhonguo4118.cn

throw new RuntimeException("失败", 500);
来源：https://ii.zhonguo2118.cn

[U72] PHP：写错误日志
来源：https://ws.zhonguo7118.cn

error_log("失败: " . $e->getMessage());
来源：https://bo.zhonguo8118.cn

[U73] PHP：读取 ini 配置
来源：https://ec.zhonguo8118.cn

parse_ini_file("config.ini", true)
来源：https://ts.zhonguo2118.cn

[U74] PHP：读取环境变量
来源：https://nj.zhonguo6118.cn

getenv("APP_ENV") ?: "production"
来源：https://lu.zhonguo1118.cn

[U75] PHP：依赖注入
来源：https://qf.zhonguo4118.cn

composer require psr/container
来源：https://ws.zhonguo4118.cn

[U76] PHP：简单路由
来源：https://um.zhonguo6118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://yf.zhonguo5118.cn

[U77] PHP：模板渲染
来源：https://kl.zhonguo1118.cn

composer require twig/twig
来源：https://fl.zhonguo6118.cn

[U78] PHP：单元测试
来源：https://yw.zhonguo6118.cn

composer require --dev phpunit/phpunit
来源：https://un.zhonguo1118.cn

[U79] PHP：静态分析
来源：https://nd.zhonguo2118.cn

composer require --dev phpstan/phpstan
来源：https://nb.zhonguo1118.cn

[U80] PHP：代码规范修复
来源：https://fz.zhonguo7118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://dm.zhonguo2118.cn

[U81] JS：初始化项目
来源：https://zf.zhonguo8118.cn

npm init -y;  npm i express
来源：https://gh.zhonguo7118.cn

[U82] JS：package.json 脚本
来源：https://bx.zhonguo6118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://wr.zhonguo6118.cn

[U83] JS：ES Module 导入导出
来源：https://ts.zhonguo5118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://wb.zhonguo4118.cn

[U84] JS：CommonJS 写法
来源：https://px.zhonguo7118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://ch.zhonguo4118.cn

[U85] JS：可选链
来源：https://sg.zhonguo7118.cn

a?.b?.c
来源：https://bw.zhonguo3118.cn

[U86] JS：空值合并
来源：https://ff.zhonguo4118.cn

a ?? b
来源：https://im.zhonguo1118.cn

[U87] JS：解构默认值
来源：https://ht.zhonguo4118.cn

const { a = 1, b = 2 } = obj;
来源：https://tg.zhonguo6118.cn

[U88] JS：对象展开合并
来源：https://dj.zhonguo7118.cn

{ ...a, ...b }
来源：https://wr.zhonguo1118.cn

[U89] JS：数组去重
来源：https://nu.zhonguo7118.cn

[...new Set(arr)]
来源：https://wr.zhonguo4118.cn

[U90] JS：数字数组排序
来源：https://cy.zhonguo4118.cn

[...arr].sort((a, b) => a - b)
来源：https://nn.zhonguo5118.cn

[U91] JS：对象键值遍历
来源：https://xc.zhonguo1118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://ep.zhonguo4118.cn

[U92] JS：深拷贝
来源：https://yt.zhonguo3118.cn

structuredClone(obj)
来源：https://pm.zhonguo8118.cn

[U93] JS：模板字符串
来源：https://re.zhonguo7118.cn

`共 ${n} 条`
来源：https://oy.zhonguo5118.cn

[U94] JS：箭头函数
来源：https://rd.zhonguo3118.cn

const double = x => x * 2;
来源：https://jv.zhonguo4118.cn

[U95] JS：Promise 包装
来源：https://sc.zhonguo3118.cn

new Promise((resolve, reject) => {})
来源：https://ua.zhonguo3118.cn

[U96] JS：async/await 与异常
来源：https://yd.zhonguo3118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://yb.zhonguo6118.cn

[U97] JS：并发请求
来源：https://et.zhonguo8118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://vl.zhonguo2118.cn

[U98] JS：fetch 带 JSON
来源：https://jd.zhonguo6118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://kh.zhonguo3118.cn

[U99] JS：事件监听
来源：https://us.zhonguo8118.cn

el.addEventListener("click", e => {})
来源：https://le.zhonguo4118.cn

[U100] JS：DOM 查询
来源：https://ct.zhonguo5118.cn

document.querySelector(".item")
来源：https://qc.zhonguo7118.cn

[U101] JS：classList 操作
来源：https://nv.zhonguo3118.cn

el.classList.toggle("active")
来源：https://lt.zhonguo1118.cn

[U102] JS：本地存储
来源：https://mq.zhonguo1118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://cn.zhonguo1118.cn

[U103] JS：定时器
来源：https://oc.zhonguo1118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://tu.zhonguo4118.cn

[U104] JS：防抖
来源：https://mj.zhonguo1118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://md.zhonguo4118.cn

[U105] JS：节流
来源：https://hv.zhonguo1118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://qh.zhonguo8118.cn

[U106] JS：日期格式化
来源：https://py.zhonguo1118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://qh.zhonguo8118.cn

[U107] JS：数字千分位
来源：https://cx.zhonguo6118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://yu.zhonguo5118.cn

[U108] JS：随机整数
来源：https://xx.zhonguo6118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://qj.zhonguo2118.cn

[U109] JS：数组分组
来源：https://zt.zhonguo5118.cn

Object.groupBy(arr, x => x.type)
来源：https://mg.zhonguo7118.cn

[U110] JS：数组分块
来源：https://dx.zhonguo3118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://gs.zhonguo7118.cn

[U111] JS：对象转 Map
来源：https://fa.zhonguo2118.cn

new Map(Object.entries(obj))
来源：https://od.zhonguo6118.cn

[U112] JS：字符串补位
来源：https://qc.zhonguo2118.cn

"7".padStart(3, "0")
来源：https://kb.zhonguo8118.cn


<!-- 参考信息 -->