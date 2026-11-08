代发 wailian999

[T27] Swift：错误处理
来源：https://qw.zhonguo1118.cn

do { try f() } catch { print(error) }
来源：https://kj.zhonguo1118.cn

[T28] Swift：枚举
来源：https://se.zhonguo1118.cn

enum Color { case red, green }
来源：https://pt.zhonguo7118.cn

[T29] Swift：guard 提前返回
来源：https://lc.zhonguo5118.cn

guard let x = opt else { return }
来源：https://ha.zhonguo8118.cn

[T30] Swift：协议
来源：https://lm.zhonguo5118.cn

protocol Shape { func area() -> Double }
来源：https://hp.zhonguo8118.cn

[T31] Lua：Hello World
来源：https://vp.zhonguo1118.cn

print("Hello")
来源：https://wc.zhonguo8118.cn

[T32] Lua：局部变量
来源：https://fg.zhonguo1118.cn

local a = 1
来源：https://bo.zhonguo8118.cn

[T33] Lua：表（数组）
来源：https://bi.zhonguo7118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://wd.zhonguo4118.cn

[T34] Lua：遍历表
来源：https://ba.zhonguo3118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://xp.zhonguo6118.cn

[T35] Lua：字典表
来源：https://my.zhonguo7118.cn

local d = { a = 1 };  d.b = 2
来源：https://vu.zhonguo1118.cn

[T36] Lua：函数
来源：https://ih.zhonguo2118.cn

function add(a, b) return a + b end
来源：https://by.zhonguo6118.cn

[T37] Lua：字符串拼接
来源：https://dd.zhonguo2118.cn

"a" .. "b"
来源：https://mj.zhonguo2118.cn

[T38] Lua：条件
来源：https://cv.zhonguo8118.cn

if x > 0 then print("正") end
来源：https://ww.zhonguo5118.cn

[T39] Lua：模式匹配
来源：https://vy.zhonguo7118.cn

string.find(s, "%d+")
来源：https://wr.zhonguo3118.cn

[T40] Lua：元表
来源：https://wy.zhonguo4118.cn

setmetatable({}, { __index = base })
来源：https://ad.zhonguo2118.cn

[T41] Perl：Hello World
来源：https://cm.zhonguo4118.cn

print "Hello\n";
来源：https://nx.zhonguo4118.cn

[T42] Perl：变量类型
来源：https://yc.zhonguo2118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://mn.zhonguo5118.cn

[T43] Perl：字符串插值
来源：https://li.zhonguo3118.cn

"值: $a"
来源：https://zx.zhonguo3118.cn

[T44] Perl：条件
来源：https://sv.zhonguo5118.cn

if ($a > 0) { print "正"; }
来源：https://ce.zhonguo5118.cn

[T45] Perl：数组遍历
来源：https://da.zhonguo1118.cn

for my $x (@arr) { print $x; }
来源：https://rd.zhonguo3118.cn

[T46] Perl：哈希操作
来源：https://nv.zhonguo2118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://fn.zhonguo3118.cn

[T47] Perl：正则捕获
来源：https://xm.zhonguo1118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://uo.zhonguo5118.cn

[T48] Perl：正则替换
来源：https://pk.zhonguo6118.cn

$s =~ s/old/new/g;
来源：https://zu.zhonguo3118.cn

[T49] Perl：函数
来源：https://kt.zhonguo3118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://jb.zhonguo5118.cn

[T50] Perl：逐行读文件
来源：https://pn.zhonguo1118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://as.zhonguo6118.cn

while (my $line = <$fh>) { print $line; }
来源：https://sr.zhonguo8118.cn

[T51] Scala：Hello World
来源：https://vg.zhonguo2118.cn

println("Hello")
来源：https://sn.zhonguo7118.cn

[T52] Scala：变量
来源：https://sd.zhonguo5118.cn

val a = 1;  var b = 2
来源：https://dr.zhonguo8118.cn

[T53] Scala：字符串插值
来源：https://wv.zhonguo1118.cn

s"值: $b"
来源：https://ws.zhonguo8118.cn

[T54] Scala：集合映射
来源：https://zo.zhonguo5118.cn

List(1, 2, 3).map(_ * 2)
来源：https://cg.zhonguo5118.cn

[T55] Scala：集合过滤
来源：https://mb.zhonguo3118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://pl.zhonguo3118.cn

[T56] Scala：样例类
来源：https://de.zhonguo5118.cn

case class User(name: String, age: Int)
来源：https://gd.zhonguo5118.cn

[T57] Scala：模式匹配
来源：https://vw.zhonguo8118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://me.zhonguo5118.cn

[T58] Scala：函数定义
来源：https://um.zhonguo6118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://ab.zhonguo5118.cn

[T59] Scala：循环
来源：https://ua.zhonguo2118.cn

for (i <- 1 to 10) println(i)
来源：https://nj.zhonguo7118.cn

[T60] Scala：折叠
来源：https://fp.zhonguo1118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://ar.zhonguo3118.cn

================================================================================
来源：https://au.zhonguo1118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://gz.zhonguo1118.cn

================================================================================
来源：https://nf.zhonguo7118.cn

[U01] Py：创建虚拟环境
来源：https://db.zhonguo5118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://lk.zhonguo7118.cn

[U02] Py：导出 / 安装依赖
来源：https://nq.zhonguo1118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://hu.zhonguo8118.cn

[U03] Py：加载 .env 配置
来源：https://jt.zhonguo7118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://gz.zhonguo4118.cn

[U04] Py：变量调试打印
来源：https://uj.zhonguo3118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://rx.zhonguo2118.cn

[U05] Py：列表去重且保序
来源：https://us.zhonguo2118.cn

list(dict.fromkeys(arr))
来源：https://gb.zhonguo6118.cn

[U06] Py：合并两个字典
来源：https://rs.zhonguo2118.cn

{**a, **b}
来源：https://os.zhonguo3118.cn

[U07] Py：反转字典键值
来源：https://zg.zhonguo4118.cn

{v: k for k, v in d.items()}
来源：https://yi.zhonguo7118.cn

[U08] Py：展平二维列表
来源：https://pr.zhonguo1118.cn

[y for x in nested for y in x]
来源：https://en.zhonguo1118.cn

[U09] Py：字典取最大值的键
来源：https://df.zhonguo4118.cn

max(d, key=d.get)
来源：https://zq.zhonguo4118.cn

[U10] Py：按值排序字典
来源：https://pn.zhonguo1118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://qm.zhonguo2118.cn

[U11] Py：生成器表达式
来源：https://ot.zhonguo8118.cn

(x * 2 for x in arr)
来源：https://oh.zhonguo5118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://hp.zhonguo3118.cn

Counter(arr).most_common(3)
来源：https://hh.zhonguo1118.cn

[U13] Py：固定长度队列
来源：https://xe.zhonguo4118.cn

deque(maxlen=10)
来源：https://sr.zhonguo7118.cn

[U14] Py：分组收集到列表
来源：https://qw.zhonguo4118.cn

defaultdict(list)
来源：https://jb.zhonguo6118.cn

[U15] Py：高精度计时
来源：https://sv.zhonguo5118.cn

t = time.perf_counter()
来源：https://qt.zhonguo5118.cn

[U16] Py：命令行参数解析
来源：https://af.zhonguo3118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://pj.zhonguo5118.cn

[U17] Py：初始化日志
来源：https://pd.zhonguo3118.cn

logging.basicConfig(level=logging.INFO)
来源：https://gk.zhonguo2118.cn

[U18] Py：预编译正则
来源：https://mv.zhonguo8118.cn

pat = re.compile(r"\d+")
来源：https://pi.zhonguo3118.cn

[U19] Py：正则替换带回调
来源：https://mc.zhonguo2118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://pe.zhonguo4118.cn

[U20] Py：缓存函数结果
来源：https://ud.zhonguo4118.cn

@functools.lru_cache(maxsize=None)
来源：https://nj.zhonguo1118.cn

[U21] Py：自定义上下文管理器
来源：https://ew.zhonguo3118.cn

@contextlib.contextmanager
来源：https://ol.zhonguo5118.cn

[U22] Py：矩阵转置
来源：https://vs.zhonguo1118.cn

list(zip(*m))
来源：https://ui.zhonguo8118.cn

[U23] Py：分块读取大文件
来源：https://ae.zhonguo5118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://oj.zhonguo4118.cn

[U24] Py：路径操作
来源：https://oh.zhonguo6118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://na.zhonguo6118.cn

[U25] Py：CSV 按字典读
来源：https://ht.zhonguo8118.cn

csv.DictReader(f)
来源：https://xt.zhonguo7118.cn

[U26] Py：并发下载
来源：https://tm.zhonguo5118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://rm.zhonguo3118.cn

[U27] Py：异步 HTTP
来源：https://xo.zhonguo4118.cn

aiohttp.ClientSession() 配合 async with
来源：https://ft.zhonguo6118.cn

[U28] Py：类型别名
来源：https://lr.zhonguo5118.cn

UserId = int
来源：https://na.zhonguo6118.cn

[U29] Py：属性校验
来源：https://kc.zhonguo6118.cn

@property 与 @x.setter 配合
来源：https://ze.zhonguo4118.cn

[U30] Py：数据类
来源：https://yq.zhonguo6118.cn

@dataclass(slots=True)
来源：https://iy.zhonguo3118.cn

[U31] Py：单测
来源：https://cv.zhonguo8118.cn

python -m pytest -q
来源：https://bb.zhonguo2118.cn

[U32] Py：代码格式化
来源：https://gc.zhonguo8118.cn

ruff format . && ruff check --fix .
来源：https://yc.zhonguo8118.cn

[U33] Py：打包发布
来源：https://tn.zhonguo3118.cn

python -m build  （依赖 pyproject.toml）
来源：https://iz.zhonguo7118.cn

[U34] Py：判断编码
来源：https://li.zhonguo7118.cn

chardet.detect(raw)
来源：https://bt.zhonguo1118.cn

[U35] Py：发送邮件
来源：https://fn.zhonguo7118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://jl.zhonguo4118.cn

[U36] Py：定时任务
来源：https://vq.zhonguo7118.cn

schedule.every(10).minutes.do(job)
来源：https://vl.zhonguo4118.cn

[U37] Py：读写 Excel
来源：https://qf.zhonguo7118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://ex.zhonguo8118.cn

[U38] Py：获取脚本所在目录
来源：https://hz.zhonguo2118.cn

Path(__file__).resolve().parent
来源：https://je.zhonguo2118.cn

[U39] Py：判断是否在交互环境
来源：https://aw.zhonguo4118.cn

sys.stdout.isatty()
来源：https://lv.zhonguo5118.cn

[U40] Py：打印到标准错误
来源：https://us.zhonguo6118.cn

print("err", file=sys.stderr)
来源：https://gs.zhonguo8118.cn

[U41] PHP：初始化 Composer 项目
来源：https://lw.zhonguo5118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://rr.zhonguo8118.cn

[U42] PHP：PSR-4 自动加载
来源：https://wf.zhonguo6118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://qd.zhonguo2118.cn

[U43] PHP：声明命名空间
来源：https://lm.zhonguo4118.cn

namespace App\Http;
来源：https://di.zhonguo8118.cn

[U44] PHP：开启严格类型
来源：https://in.zhonguo1118.cn

declare(strict_types=1);
来源：https://ha.zhonguo8118.cn

[U45] PHP：类型声明与返回类型
来源：https://mh.zhonguo3118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://qn.zhonguo5118.cn

[U46] PHP：可空类型
来源：https://te.zhonguo2118.cn

?string $name = null
来源：https://lw.zhonguo8118.cn

[U47] PHP：联合类型
来源：https://gv.zhonguo4118.cn

int|string $id
来源：https://rr.zhonguo7118.cn

[U48] PHP：纯枚举
来源：https://df.zhonguo8118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://go.zhonguo7118.cn

[U49] PHP：只读属性
来源：https://kw.zhonguo6118.cn

public readonly string $name
来源：https://qe.zhonguo1118.cn

[U50] PHP：构造器属性提升
来源：https://uu.zhonguo5118.cn

public function __construct(private int $id) {}
来源：https://rp.zhonguo7118.cn

[U51] PHP：数组解构
来源：https://yp.zhonguo1118.cn

[$a, $b] = $arr;
来源：https://jm.zhonguo5118.cn

[U52] PHP：箭头函数
来源：https://tx.zhonguo7118.cn

$double = fn($x) => $x * 2;
来源：https://vt.zhonguo2118.cn

[U53] PHP：空合并运算符
来源：https://wl.zhonguo2118.cn

$v = $a ?? $b ?? "default";
来源：https://ma.zhonguo7118.cn

[U54] PHP：空安全调用
来源：https://gc.zhonguo7118.cn

$obj?->method()
来源：https://kd.zhonguo6118.cn

[U55] PHP：match 表达式
来源：https://sv.zhonguo1118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://it.zhonguo7118.cn

[U56] PHP：命名参数
来源：https://rk.zhonguo6118.cn

f(a: 1, b: 2)
来源：https://dn.zhonguo7118.cn

[U57] PHP：字符串插值
来源：https://vd.zhonguo6118.cn

"值: {$a}"
来源：https://yy.zhonguo7118.cn

[U58] PHP：数组三件套
来源：https://th.zhonguo1118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://gk.zhonguo1118.cn

[U59] PHP：自定义排序
来源：https://yf.zhonguo2118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://dl.zhonguo3118.cn

[U60] PHP：JSON 编解码
来源：https://fp.zhonguo7118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://dj.zhonguo6118.cn

[U61] PHP：正则
来源：https://ke.zhonguo7118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://li.zhonguo4118.cn

[U62] PHP：日期对象
来源：https://gz.zhonguo3118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://rq.zhonguo7118.cn

[U63] PHP：文件读写
来源：https://wn.zhonguo6118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://ug.zhonguo2118.cn

[U64] PHP：目录遍历
来源：https://cf.zhonguo7118.cn

glob("dir/*.php");  scandir("dir");
来源：https://ff.zhonguo5118.cn

[U65] PHP：会话
来源：https://py.zhonguo5118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://zq.zhonguo1118.cn

[U66] PHP：设置 Cookie
来源：https://he.zhonguo4118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://xf.zhonguo2118.cn

[U67] PHP：处理文件上传
来源：https://ho.zhonguo4118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://od.zhonguo8118.cn

[U68] PHP：PDO 连接
来源：https://oy.zhonguo2118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://ei.zhonguo5118.cn

[U69] PHP：PDO 预处理
来源：https://er.zhonguo6118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://rj.zhonguo5118.cn

[U70] PHP：PDO 事务
来源：https://id.zhonguo2118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://dc.zhonguo1118.cn

[U71] PHP：抛出异常
来源：https://pv.zhonguo5118.cn

throw new RuntimeException("失败", 500);
来源：https://gv.zhonguo4118.cn

[U72] PHP：写错误日志
来源：https://rw.zhonguo1118.cn

error_log("失败: " . $e->getMessage());
来源：https://rg.zhonguo6118.cn

[U73] PHP：读取 ini 配置
来源：https://uc.zhonguo4118.cn

parse_ini_file("config.ini", true)
来源：https://qt.zhonguo8118.cn

[U74] PHP：读取环境变量
来源：https://or.zhonguo4118.cn

getenv("APP_ENV") ?: "production"
来源：https://vj.zhonguo6118.cn

[U75] PHP：依赖注入
来源：https://ng.zhonguo6118.cn

composer require psr/container
来源：https://vd.zhonguo4118.cn

[U76] PHP：简单路由
来源：https://gh.zhonguo5118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://cj.zhonguo2118.cn

[U77] PHP：模板渲染
来源：https://cy.zhonguo3118.cn

composer require twig/twig
来源：https://dr.zhonguo6118.cn

[U78] PHP：单元测试
来源：https://co.zhonguo7118.cn

composer require --dev phpunit/phpunit
来源：https://nb.zhonguo1118.cn

[U79] PHP：静态分析
来源：https://qi.zhonguo2118.cn

composer require --dev phpstan/phpstan
来源：https://xe.zhonguo8118.cn

[U80] PHP：代码规范修复
来源：https://rq.zhonguo7118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://jc.zhonguo2118.cn

[U81] JS：初始化项目
来源：https://kl.zhonguo8118.cn

npm init -y;  npm i express
来源：https://yc.zhonguo3118.cn

[U82] JS：package.json 脚本
来源：https://ai.zhonguo8118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://gi.zhonguo5118.cn

[U83] JS：ES Module 导入导出
来源：https://kw.zhonguo7118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://ye.zhonguo5118.cn

[U84] JS：CommonJS 写法
来源：https://pd.zhonguo7118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://fk.zhonguo6118.cn

[U85] JS：可选链
来源：https://ff.zhonguo3118.cn

a?.b?.c
来源：https://oz.zhonguo6118.cn

[U86] JS：空值合并
来源：https://dw.zhonguo1118.cn

a ?? b
来源：https://wi.zhonguo4118.cn

[U87] JS：解构默认值
来源：https://iy.zhonguo2118.cn

const { a = 1, b = 2 } = obj;
来源：https://fq.zhonguo6118.cn

[U88] JS：对象展开合并
来源：https://jy.zhonguo7118.cn

{ ...a, ...b }
来源：https://sw.zhonguo2118.cn

[U89] JS：数组去重
来源：https://xg.zhonguo4118.cn

[...new Set(arr)]
来源：https://dn.zhonguo4118.cn

[U90] JS：数字数组排序
来源：https://vf.zhonguo4118.cn

[...arr].sort((a, b) => a - b)
来源：https://yw.zhonguo5118.cn

[U91] JS：对象键值遍历
来源：https://uc.zhonguo8118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://bn.zhonguo3118.cn

[U92] JS：深拷贝
来源：https://nf.zhonguo8118.cn

structuredClone(obj)
来源：https://nq.zhonguo1118.cn

[U93] JS：模板字符串
来源：https://gf.zhonguo1118.cn

`共 ${n} 条`
来源：https://yy.zhonguo2118.cn

[U94] JS：箭头函数
来源：https://fj.zhonguo4118.cn

const double = x => x * 2;
来源：https://ze.zhonguo2118.cn

[U95] JS：Promise 包装
来源：https://xj.zhonguo2118.cn

new Promise((resolve, reject) => {})
来源：https://if.zhonguo2118.cn

[U96] JS：async/await 与异常
来源：https://dt.zhonguo2118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://ub.zhonguo2118.cn

[U97] JS：并发请求
来源：https://yh.zhonguo5118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://vq.zhonguo3118.cn

[U98] JS：fetch 带 JSON
来源：https://xx.zhonguo7118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://tp.zhonguo1118.cn

[U99] JS：事件监听
来源：https://sv.zhonguo1118.cn

el.addEventListener("click", e => {})
来源：https://cz.zhonguo6118.cn

[U100] JS：DOM 查询
来源：https://ys.zhonguo7118.cn

document.querySelector(".item")
来源：https://am.zhonguo1118.cn

[U101] JS：classList 操作
来源：https://am.zhonguo8118.cn

el.classList.toggle("active")
来源：https://ez.zhonguo6118.cn

[U102] JS：本地存储
来源：https://qu.zhonguo8118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://xa.zhonguo6118.cn

[U103] JS：定时器
来源：https://wn.zhonguo8118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://rm.zhonguo2118.cn

[U104] JS：防抖
来源：https://ou.zhonguo3118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://wc.zhonguo3118.cn

[U105] JS：节流
来源：https://je.zhonguo4118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://is.zhonguo5118.cn

[U106] JS：日期格式化
来源：https://xq.zhonguo8118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://uo.zhonguo2118.cn

[U107] JS：数字千分位
来源：https://uj.zhonguo1118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://tf.zhonguo5118.cn

[U108] JS：随机整数
来源：https://hu.zhonguo1118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://jo.zhonguo4118.cn

[U109] JS：数组分组
来源：https://sn.zhonguo7118.cn

Object.groupBy(arr, x => x.type)
来源：https://jy.zhonguo1118.cn

[U110] JS：数组分块
来源：https://rh.zhonguo2118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://nt.zhonguo3118.cn

[U111] JS：对象转 Map
来源：https://vc.zhonguo3118.cn

new Map(Object.entries(obj))
来源：https://pw.zhonguo3118.cn

[U112] JS：字符串补位
来源：https://xj.zhonguo6118.cn

"7".padStart(3, "0")
来源：https://uc.zhonguo7118.cn

[U113] JS：正则替换全部
来源：https://bb.zhonguo2118.cn

s.replaceAll("a", "b")
来源：https://lw.zhonguo6118.cn

[U114] JS：JSON 深比较
来源：https://ew.zhonguo1118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://lb.zhonguo4118.cn


<!-- 参考信息 -->