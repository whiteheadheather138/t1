代发 wailian999

[T31] Lua：Hello World
来源：https://vg.zhonguo1118.cn

print("Hello")
来源：https://da.zhonguo6118.cn

[T32] Lua：局部变量
来源：https://wh.zhonguo1118.cn

local a = 1
来源：https://ye.zhonguo1118.cn

[T33] Lua：表（数组）
来源：https://za.zhonguo7118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://gc.zhonguo5118.cn

[T34] Lua：遍历表
来源：https://pt.zhonguo1118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://az.zhonguo7118.cn

[T35] Lua：字典表
来源：https://ss.zhonguo2118.cn

local d = { a = 1 };  d.b = 2
来源：https://bb.zhonguo8118.cn

[T36] Lua：函数
来源：https://nl.zhonguo1118.cn

function add(a, b) return a + b end
来源：https://nm.zhonguo3118.cn

[T37] Lua：字符串拼接
来源：https://rg.zhonguo6118.cn

"a" .. "b"
来源：https://yw.zhonguo1118.cn

[T38] Lua：条件
来源：https://ir.zhonguo3118.cn

if x > 0 then print("正") end
来源：https://bw.zhonguo6118.cn

[T39] Lua：模式匹配
来源：https://ae.zhonguo4118.cn

string.find(s, "%d+")
来源：https://cx.zhonguo6118.cn

[T40] Lua：元表
来源：https://pm.zhonguo4118.cn

setmetatable({}, { __index = base })
来源：https://gf.zhonguo5118.cn

[T41] Perl：Hello World
来源：https://vz.zhonguo7118.cn

print "Hello\n";
来源：https://jf.zhonguo7118.cn

[T42] Perl：变量类型
来源：https://mx.zhonguo8118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://px.zhonguo1118.cn

[T43] Perl：字符串插值
来源：https://ps.zhonguo5118.cn

"值: $a"
来源：https://fs.zhonguo1118.cn

[T44] Perl：条件
来源：https://ks.zhonguo6118.cn

if ($a > 0) { print "正"; }
来源：https://fj.zhonguo1118.cn

[T45] Perl：数组遍历
来源：https://kq.zhonguo7118.cn

for my $x (@arr) { print $x; }
来源：https://io.zhonguo6118.cn

[T46] Perl：哈希操作
来源：https://qt.zhonguo5118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://gg.zhonguo2118.cn

[T47] Perl：正则捕获
来源：https://az.zhonguo7118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://tk.zhonguo1118.cn

[T48] Perl：正则替换
来源：https://cn.zhonguo2118.cn

$s =~ s/old/new/g;
来源：https://hl.zhonguo5118.cn

[T49] Perl：函数
来源：https://yt.zhonguo2118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://sm.zhonguo4118.cn

[T50] Perl：逐行读文件
来源：https://zk.zhonguo6118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://nw.zhonguo8118.cn

while (my $line = <$fh>) { print $line; }
来源：https://rt.zhonguo6118.cn

[T51] Scala：Hello World
来源：https://xe.zhonguo6118.cn

println("Hello")
来源：https://fe.zhonguo6118.cn

[T52] Scala：变量
来源：https://um.zhonguo6118.cn

val a = 1;  var b = 2
来源：https://jn.zhonguo4118.cn

[T53] Scala：字符串插值
来源：https://aw.zhonguo3118.cn

s"值: $b"
来源：https://gf.zhonguo6118.cn

[T54] Scala：集合映射
来源：https://kn.zhonguo7118.cn

List(1, 2, 3).map(_ * 2)
来源：https://pd.zhonguo4118.cn

[T55] Scala：集合过滤
来源：https://mo.zhonguo3118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://cp.zhonguo1118.cn

[T56] Scala：样例类
来源：https://nc.zhonguo5118.cn

case class User(name: String, age: Int)
来源：https://qw.zhonguo8118.cn

[T57] Scala：模式匹配
来源：https://sh.zhonguo7118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://by.zhonguo2118.cn

[T58] Scala：函数定义
来源：https://dd.zhonguo7118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://dq.zhonguo7118.cn

[T59] Scala：循环
来源：https://cg.zhonguo5118.cn

for (i <- 1 to 10) println(i)
来源：https://qw.zhonguo1118.cn

[T60] Scala：折叠
来源：https://mr.zhonguo2118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://mr.zhonguo4118.cn

================================================================================
来源：https://cv.zhonguo4118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://gn.zhonguo5118.cn

================================================================================
来源：https://nr.zhonguo7118.cn

[U01] Py：创建虚拟环境
来源：https://mo.zhonguo4118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://sw.zhonguo6118.cn

[U02] Py：导出 / 安装依赖
来源：https://js.zhonguo3118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://ah.zhonguo6118.cn

[U03] Py：加载 .env 配置
来源：https://wo.zhonguo4118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://ok.zhonguo8118.cn

[U04] Py：变量调试打印
来源：https://cr.zhonguo1118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://ar.zhonguo6118.cn

[U05] Py：列表去重且保序
来源：https://db.zhonguo1118.cn

list(dict.fromkeys(arr))
来源：https://fx.zhonguo6118.cn

[U06] Py：合并两个字典
来源：https://ud.zhonguo5118.cn

{**a, **b}
来源：https://fh.zhonguo8118.cn

[U07] Py：反转字典键值
来源：https://ib.zhonguo5118.cn

{v: k for k, v in d.items()}
来源：https://xv.zhonguo1118.cn

[U08] Py：展平二维列表
来源：https://ra.zhonguo4118.cn

[y for x in nested for y in x]
来源：https://qq.zhonguo1118.cn

[U09] Py：字典取最大值的键
来源：https://ak.zhonguo5118.cn

max(d, key=d.get)
来源：https://zu.zhonguo2118.cn

[U10] Py：按值排序字典
来源：https://ay.zhonguo8118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://bo.zhonguo3118.cn

[U11] Py：生成器表达式
来源：https://gx.zhonguo2118.cn

(x * 2 for x in arr)
来源：https://ps.zhonguo6118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://im.zhonguo1118.cn

Counter(arr).most_common(3)
来源：https://mb.zhonguo8118.cn

[U13] Py：固定长度队列
来源：https://vc.zhonguo2118.cn

deque(maxlen=10)
来源：https://nn.zhonguo6118.cn

[U14] Py：分组收集到列表
来源：https://kj.zhonguo1118.cn

defaultdict(list)
来源：https://az.zhonguo1118.cn

[U15] Py：高精度计时
来源：https://ac.zhonguo3118.cn

t = time.perf_counter()
来源：https://ot.zhonguo6118.cn

[U16] Py：命令行参数解析
来源：https://pp.zhonguo4118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://fp.zhonguo2118.cn

[U17] Py：初始化日志
来源：https://cb.zhonguo3118.cn

logging.basicConfig(level=logging.INFO)
来源：https://hp.zhonguo7118.cn

[U18] Py：预编译正则
来源：https://ev.zhonguo6118.cn

pat = re.compile(r"\d+")
来源：https://ux.zhonguo3118.cn

[U19] Py：正则替换带回调
来源：https://vj.zhonguo6118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://wi.zhonguo2118.cn

[U20] Py：缓存函数结果
来源：https://fw.zhonguo3118.cn

@functools.lru_cache(maxsize=None)
来源：https://kn.zhonguo4118.cn

[U21] Py：自定义上下文管理器
来源：https://qt.zhonguo8118.cn

@contextlib.contextmanager
来源：https://zh.zhonguo7118.cn

[U22] Py：矩阵转置
来源：https://gm.zhonguo4118.cn

list(zip(*m))
来源：https://pv.zhonguo8118.cn

[U23] Py：分块读取大文件
来源：https://xz.zhonguo5118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://ew.zhonguo4118.cn

[U24] Py：路径操作
来源：https://ed.zhonguo8118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://wy.zhonguo5118.cn

[U25] Py：CSV 按字典读
来源：https://je.zhonguo8118.cn

csv.DictReader(f)
来源：https://yf.zhonguo7118.cn

[U26] Py：并发下载
来源：https://sl.zhonguo6118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://nx.zhonguo5118.cn

[U27] Py：异步 HTTP
来源：https://yw.zhonguo7118.cn

aiohttp.ClientSession() 配合 async with
来源：https://wf.zhonguo7118.cn

[U28] Py：类型别名
来源：https://wt.zhonguo5118.cn

UserId = int
来源：https://xu.zhonguo3118.cn

[U29] Py：属性校验
来源：https://dj.zhonguo5118.cn

@property 与 @x.setter 配合
来源：https://iz.zhonguo2118.cn

[U30] Py：数据类
来源：https://hx.zhonguo2118.cn

@dataclass(slots=True)
来源：https://sy.zhonguo2118.cn

[U31] Py：单测
来源：https://xo.zhonguo8118.cn

python -m pytest -q
来源：https://fc.zhonguo7118.cn

[U32] Py：代码格式化
来源：https://yj.zhonguo5118.cn

ruff format . && ruff check --fix .
来源：https://th.zhonguo4118.cn

[U33] Py：打包发布
来源：https://gl.zhonguo4118.cn

python -m build  （依赖 pyproject.toml）
来源：https://aq.zhonguo8118.cn

[U34] Py：判断编码
来源：https://hs.zhonguo1118.cn

chardet.detect(raw)
来源：https://cf.zhonguo2118.cn

[U35] Py：发送邮件
来源：https://vn.zhonguo6118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://kv.zhonguo6118.cn

[U36] Py：定时任务
来源：https://xn.zhonguo2118.cn

schedule.every(10).minutes.do(job)
来源：https://ut.zhonguo6118.cn

[U37] Py：读写 Excel
来源：https://wl.zhonguo2118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://ou.zhonguo4118.cn

[U38] Py：获取脚本所在目录
来源：https://tq.zhonguo8118.cn

Path(__file__).resolve().parent
来源：https://tt.zhonguo2118.cn

[U39] Py：判断是否在交互环境
来源：https://vy.zhonguo2118.cn

sys.stdout.isatty()
来源：https://to.zhonguo4118.cn

[U40] Py：打印到标准错误
来源：https://eh.zhonguo4118.cn

print("err", file=sys.stderr)
来源：https://zu.zhonguo8118.cn

[U41] PHP：初始化 Composer 项目
来源：https://rq.zhonguo3118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://wy.zhonguo8118.cn

[U42] PHP：PSR-4 自动加载
来源：https://se.zhonguo8118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://sf.zhonguo3118.cn

[U43] PHP：声明命名空间
来源：https://sr.zhonguo5118.cn

namespace App\Http;
来源：https://yf.zhonguo7118.cn

[U44] PHP：开启严格类型
来源：https://bc.zhonguo7118.cn

declare(strict_types=1);
来源：https://jy.zhonguo2118.cn

[U45] PHP：类型声明与返回类型
来源：https://wz.zhonguo1118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://be.zhonguo7118.cn

[U46] PHP：可空类型
来源：https://ww.zhonguo5118.cn

?string $name = null
来源：https://og.zhonguo4118.cn

[U47] PHP：联合类型
来源：https://mt.zhonguo7118.cn

int|string $id
来源：https://sb.zhonguo4118.cn

[U48] PHP：纯枚举
来源：https://cy.zhonguo3118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://ny.zhonguo7118.cn

[U49] PHP：只读属性
来源：https://qk.zhonguo1118.cn

public readonly string $name
来源：https://vs.zhonguo6118.cn

[U50] PHP：构造器属性提升
来源：https://mo.zhonguo1118.cn

public function __construct(private int $id) {}
来源：https://hj.zhonguo3118.cn

[U51] PHP：数组解构
来源：https://xo.zhonguo7118.cn

[$a, $b] = $arr;
来源：https://cw.zhonguo4118.cn

[U52] PHP：箭头函数
来源：https://lx.zhonguo3118.cn

$double = fn($x) => $x * 2;
来源：https://zv.zhonguo7118.cn

[U53] PHP：空合并运算符
来源：https://mn.zhonguo6118.cn

$v = $a ?? $b ?? "default";
来源：https://tk.zhonguo1118.cn

[U54] PHP：空安全调用
来源：https://qo.zhonguo7118.cn

$obj?->method()
来源：https://ha.zhonguo2118.cn

[U55] PHP：match 表达式
来源：https://um.zhonguo8118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://xm.zhonguo7118.cn

[U56] PHP：命名参数
来源：https://ik.zhonguo2118.cn

f(a: 1, b: 2)
来源：https://bb.zhonguo6118.cn

[U57] PHP：字符串插值
来源：https://qf.zhonguo8118.cn

"值: {$a}"
来源：https://hp.zhonguo7118.cn

[U58] PHP：数组三件套
来源：https://ia.zhonguo2118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://sc.zhonguo7118.cn

[U59] PHP：自定义排序
来源：https://xd.zhonguo4118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://wc.zhonguo1118.cn

[U60] PHP：JSON 编解码
来源：https://fk.zhonguo4118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://na.zhonguo6118.cn

[U61] PHP：正则
来源：https://dr.zhonguo2118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://uw.zhonguo6118.cn

[U62] PHP：日期对象
来源：https://cm.zhonguo2118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://lg.zhonguo6118.cn

[U63] PHP：文件读写
来源：https://vh.zhonguo3118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://xr.zhonguo8118.cn

[U64] PHP：目录遍历
来源：https://zm.zhonguo7118.cn

glob("dir/*.php");  scandir("dir");
来源：https://pv.zhonguo3118.cn

[U65] PHP：会话
来源：https://gr.zhonguo7118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://qc.zhonguo3118.cn

[U66] PHP：设置 Cookie
来源：https://sz.zhonguo3118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://oq.zhonguo8118.cn

[U67] PHP：处理文件上传
来源：https://kd.zhonguo5118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://ss.zhonguo8118.cn

[U68] PHP：PDO 连接
来源：https://hp.zhonguo5118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://hz.zhonguo3118.cn

[U69] PHP：PDO 预处理
来源：https://fd.zhonguo6118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://oj.zhonguo3118.cn

[U70] PHP：PDO 事务
来源：https://kq.zhonguo4118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://wd.zhonguo8118.cn

[U71] PHP：抛出异常
来源：https://ap.zhonguo8118.cn

throw new RuntimeException("失败", 500);
来源：https://fn.zhonguo4118.cn

[U72] PHP：写错误日志
来源：https://zp.zhonguo1118.cn

error_log("失败: " . $e->getMessage());
来源：https://uv.zhonguo5118.cn

[U73] PHP：读取 ini 配置
来源：https://yu.zhonguo5118.cn

parse_ini_file("config.ini", true)
来源：https://pm.zhonguo7118.cn

[U74] PHP：读取环境变量
来源：https://kn.zhonguo8118.cn

getenv("APP_ENV") ?: "production"
来源：https://ld.zhonguo6118.cn

[U75] PHP：依赖注入
来源：https://fr.zhonguo6118.cn

composer require psr/container
来源：https://gs.zhonguo6118.cn

[U76] PHP：简单路由
来源：https://zh.zhonguo7118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://ps.zhonguo3118.cn

[U77] PHP：模板渲染
来源：https://cf.zhonguo1118.cn

composer require twig/twig
来源：https://co.zhonguo2118.cn

[U78] PHP：单元测试
来源：https://py.zhonguo6118.cn

composer require --dev phpunit/phpunit
来源：https://yl.zhonguo5118.cn

[U79] PHP：静态分析
来源：https://sb.zhonguo6118.cn

composer require --dev phpstan/phpstan
来源：https://jv.zhonguo6118.cn

[U80] PHP：代码规范修复
来源：https://pg.zhonguo1118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://zc.zhonguo7118.cn

[U81] JS：初始化项目
来源：https://yz.zhonguo3118.cn

npm init -y;  npm i express
来源：https://mu.zhonguo2118.cn

[U82] JS：package.json 脚本
来源：https://fa.zhonguo7118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://lx.zhonguo3118.cn

[U83] JS：ES Module 导入导出
来源：https://ty.zhonguo1118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://dz.zhonguo1118.cn

[U84] JS：CommonJS 写法
来源：https://oh.zhonguo4118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://ol.zhonguo5118.cn

[U85] JS：可选链
来源：https://ri.zhonguo6118.cn

a?.b?.c
来源：https://wf.zhonguo3118.cn

[U86] JS：空值合并
来源：https://gg.zhonguo1118.cn

a ?? b
来源：https://hw.zhonguo4118.cn

[U87] JS：解构默认值
来源：https://bs.zhonguo3118.cn

const { a = 1, b = 2 } = obj;
来源：https://dv.zhonguo3118.cn

[U88] JS：对象展开合并
来源：https://bk.zhonguo6118.cn

{ ...a, ...b }
来源：https://hh.zhonguo8118.cn

[U89] JS：数组去重
来源：https://le.zhonguo2118.cn

[...new Set(arr)]
来源：https://gh.zhonguo7118.cn

[U90] JS：数字数组排序
来源：https://cb.zhonguo7118.cn

[...arr].sort((a, b) => a - b)
来源：https://ri.zhonguo3118.cn

[U91] JS：对象键值遍历
来源：https://zk.zhonguo8118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://xj.zhonguo6118.cn

[U92] JS：深拷贝
来源：https://yd.zhonguo1118.cn

structuredClone(obj)
来源：https://oc.zhonguo5118.cn

[U93] JS：模板字符串
来源：https://co.zhonguo3118.cn

`共 ${n} 条`
来源：https://vj.zhonguo3118.cn

[U94] JS：箭头函数
来源：https://gb.zhonguo1118.cn

const double = x => x * 2;
来源：https://vk.zhonguo7118.cn

[U95] JS：Promise 包装
来源：https://ck.zhonguo2118.cn

new Promise((resolve, reject) => {})
来源：https://sa.zhonguo1118.cn

[U96] JS：async/await 与异常
来源：https://gq.zhonguo4118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://eq.zhonguo6118.cn

[U97] JS：并发请求
来源：https://du.zhonguo1118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://en.zhonguo8118.cn

[U98] JS：fetch 带 JSON
来源：https://sr.zhonguo1118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://kx.zhonguo7118.cn

[U99] JS：事件监听
来源：https://xq.zhonguo3118.cn

el.addEventListener("click", e => {})
来源：https://jt.zhonguo3118.cn

[U100] JS：DOM 查询
来源：https://ng.zhonguo2118.cn

document.querySelector(".item")
来源：https://xw.zhonguo2118.cn

[U101] JS：classList 操作
来源：https://pq.zhonguo4118.cn

el.classList.toggle("active")
来源：https://pl.zhonguo4118.cn

[U102] JS：本地存储
来源：https://qc.zhonguo5118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://lv.zhonguo3118.cn

[U103] JS：定时器
来源：https://ge.zhonguo7118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://jt.zhonguo1118.cn

[U104] JS：防抖
来源：https://xw.zhonguo3118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://cm.zhonguo8118.cn

[U105] JS：节流
来源：https://hr.zhonguo3118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://yh.zhonguo1118.cn

[U106] JS：日期格式化
来源：https://jk.zhonguo2118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://wb.zhonguo4118.cn

[U107] JS：数字千分位
来源：https://ae.zhonguo4118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://pd.zhonguo7118.cn

[U108] JS：随机整数
来源：https://rd.zhonguo3118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://zn.zhonguo3118.cn

[U109] JS：数组分组
来源：https://bw.zhonguo5118.cn

Object.groupBy(arr, x => x.type)
来源：https://ns.zhonguo3118.cn

[U110] JS：数组分块
来源：https://zc.zhonguo4118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://jb.zhonguo5118.cn

[U111] JS：对象转 Map
来源：https://nr.zhonguo1118.cn

new Map(Object.entries(obj))
来源：https://vi.zhonguo3118.cn

[U112] JS：字符串补位
来源：https://fa.zhonguo2118.cn

"7".padStart(3, "0")
来源：https://xq.zhonguo3118.cn

[U113] JS：正则替换全部
来源：https://ko.zhonguo2118.cn

s.replaceAll("a", "b")
来源：https://hr.zhonguo6118.cn

[U114] JS：JSON 深比较
来源：https://jx.zhonguo3118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://ba.zhonguo6118.cn

[U115] JS：生成 UUID
来源：https://em.zhonguo1118.cn

crypto.randomUUID()
来源：https://ou.zhonguo2118.cn

[U116] JS：类型检查（JSDoc）
来源：https://vq.zhonguo1118.cn

/** @param {string} name */ function f(name) {}
来源：https://uj.zhonguo6118.cn

[U117] JS：单元测试
来源：https://xg.zhonguo2118.cn

npm i -D vitest;  npx vitest
来源：https://he.zhonguo6118.cn

[U118] JS：开发服务器
来源：https://gs.zhonguo7118.cn

npm i -D vite;  npx vite
来源：https://ny.zhonguo2118.cn


<!-- 参考信息 -->