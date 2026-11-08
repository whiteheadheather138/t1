代发 wailian999

[T33] Lua：表（数组）
来源：https://ol.zhonguo5118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://zn.zhonguo3118.cn

[T34] Lua：遍历表
来源：https://us.zhonguo7118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://iv.zhonguo2118.cn

[T35] Lua：字典表
来源：https://ep.zhonguo4118.cn

local d = { a = 1 };  d.b = 2
来源：https://of.zhonguo6118.cn

[T36] Lua：函数
来源：https://ns.zhonguo4118.cn

function add(a, b) return a + b end
来源：https://zf.zhonguo8118.cn

[T37] Lua：字符串拼接
来源：https://yr.zhonguo3118.cn

"a" .. "b"
来源：https://na.zhonguo2118.cn

[T38] Lua：条件
来源：https://yt.zhonguo2118.cn

if x > 0 then print("正") end
来源：https://ee.zhonguo5118.cn

[T39] Lua：模式匹配
来源：https://lr.zhonguo4118.cn

string.find(s, "%d+")
来源：https://yi.zhonguo5118.cn

[T40] Lua：元表
来源：https://ab.zhonguo1118.cn

setmetatable({}, { __index = base })
来源：https://dv.zhonguo2118.cn

[T41] Perl：Hello World
来源：https://kt.zhonguo6118.cn

print "Hello\n";
来源：https://jf.zhonguo5118.cn

[T42] Perl：变量类型
来源：https://nk.zhonguo4118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://uk.zhonguo7118.cn

[T43] Perl：字符串插值
来源：https://lk.zhonguo5118.cn

"值: $a"
来源：https://ig.zhonguo8118.cn

[T44] Perl：条件
来源：https://po.zhonguo1118.cn

if ($a > 0) { print "正"; }
来源：https://cj.zhonguo4118.cn

[T45] Perl：数组遍历
来源：https://os.zhonguo4118.cn

for my $x (@arr) { print $x; }
来源：https://ad.zhonguo2118.cn

[T46] Perl：哈希操作
来源：https://tu.zhonguo8118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://ky.zhonguo6118.cn

[T47] Perl：正则捕获
来源：https://ei.zhonguo1118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://ff.zhonguo3118.cn

[T48] Perl：正则替换
来源：https://xs.zhonguo4118.cn

$s =~ s/old/new/g;
来源：https://az.zhonguo7118.cn

[T49] Perl：函数
来源：https://ro.zhonguo1118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://es.zhonguo5118.cn

[T50] Perl：逐行读文件
来源：https://lj.zhonguo2118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://gg.zhonguo2118.cn

while (my $line = <$fh>) { print $line; }
来源：https://cx.zhonguo8118.cn

[T51] Scala：Hello World
来源：https://ev.zhonguo3118.cn

println("Hello")
来源：https://qr.zhonguo2118.cn

[T52] Scala：变量
来源：https://sw.zhonguo2118.cn

val a = 1;  var b = 2
来源：https://mx.zhonguo8118.cn

[T53] Scala：字符串插值
来源：https://zl.zhonguo1118.cn

s"值: $b"
来源：https://kb.zhonguo4118.cn

[T54] Scala：集合映射
来源：https://ht.zhonguo4118.cn

List(1, 2, 3).map(_ * 2)
来源：https://si.zhonguo6118.cn

[T55] Scala：集合过滤
来源：https://kk.zhonguo7118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://cr.zhonguo1118.cn

[T56] Scala：样例类
来源：https://mi.zhonguo2118.cn

case class User(name: String, age: Int)
来源：https://dj.zhonguo7118.cn

[T57] Scala：模式匹配
来源：https://ki.zhonguo3118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://xl.zhonguo1118.cn

[T58] Scala：函数定义
来源：https://dv.zhonguo2118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://tp.zhonguo3118.cn

[T59] Scala：循环
来源：https://rr.zhonguo5118.cn

for (i <- 1 to 10) println(i)
来源：https://hw.zhonguo2118.cn

[T60] Scala：折叠
来源：https://vj.zhonguo5118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://mu.zhonguo7118.cn

================================================================================
来源：https://lz.zhonguo7118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://rp.zhonguo5118.cn

================================================================================
来源：https://hg.zhonguo4118.cn

[U01] Py：创建虚拟环境
来源：https://nb.zhonguo2118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://ib.zhonguo5118.cn

[U02] Py：导出 / 安装依赖
来源：https://xr.zhonguo5118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://ne.zhonguo5118.cn

[U03] Py：加载 .env 配置
来源：https://sg.zhonguo7118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://cl.zhonguo7118.cn

[U04] Py：变量调试打印
来源：https://cd.zhonguo2118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://sg.zhonguo2118.cn

[U05] Py：列表去重且保序
来源：https://gp.zhonguo4118.cn

list(dict.fromkeys(arr))
来源：https://vd.zhonguo4118.cn

[U06] Py：合并两个字典
来源：https://az.zhonguo3118.cn

{**a, **b}
来源：https://ss.zhonguo6118.cn

[U07] Py：反转字典键值
来源：https://dm.zhonguo7118.cn

{v: k for k, v in d.items()}
来源：https://lc.zhonguo1118.cn

[U08] Py：展平二维列表
来源：https://ob.zhonguo6118.cn

[y for x in nested for y in x]
来源：https://yk.zhonguo5118.cn

[U09] Py：字典取最大值的键
来源：https://nd.zhonguo2118.cn

max(d, key=d.get)
来源：https://xd.zhonguo1118.cn

[U10] Py：按值排序字典
来源：https://iy.zhonguo3118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://hr.zhonguo4118.cn

[U11] Py：生成器表达式
来源：https://ds.zhonguo2118.cn

(x * 2 for x in arr)
来源：https://je.zhonguo1118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://le.zhonguo2118.cn

Counter(arr).most_common(3)
来源：https://rf.zhonguo6118.cn

[U13] Py：固定长度队列
来源：https://js.zhonguo2118.cn

deque(maxlen=10)
来源：https://xs.zhonguo4118.cn

[U14] Py：分组收集到列表
来源：https://gi.zhonguo4118.cn

defaultdict(list)
来源：https://dv.zhonguo4118.cn

[U15] Py：高精度计时
来源：https://pj.zhonguo6118.cn

t = time.perf_counter()
来源：https://hs.zhonguo2118.cn

[U16] Py：命令行参数解析
来源：https://tc.zhonguo1118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://kn.zhonguo1118.cn

[U17] Py：初始化日志
来源：https://kr.zhonguo5118.cn

logging.basicConfig(level=logging.INFO)
来源：https://mm.zhonguo1118.cn

[U18] Py：预编译正则
来源：https://ze.zhonguo7118.cn

pat = re.compile(r"\d+")
来源：https://yz.zhonguo5118.cn

[U19] Py：正则替换带回调
来源：https://xq.zhonguo8118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://eu.zhonguo8118.cn

[U20] Py：缓存函数结果
来源：https://kx.zhonguo6118.cn

@functools.lru_cache(maxsize=None)
来源：https://rk.zhonguo6118.cn

[U21] Py：自定义上下文管理器
来源：https://oq.zhonguo6118.cn

@contextlib.contextmanager
来源：https://ja.zhonguo6118.cn

[U22] Py：矩阵转置
来源：https://md.zhonguo4118.cn

list(zip(*m))
来源：https://qz.zhonguo7118.cn

[U23] Py：分块读取大文件
来源：https://jk.zhonguo5118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://cs.zhonguo1118.cn

[U24] Py：路径操作
来源：https://ou.zhonguo3118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://og.zhonguo1118.cn

[U25] Py：CSV 按字典读
来源：https://wu.zhonguo6118.cn

csv.DictReader(f)
来源：https://ou.zhonguo5118.cn

[U26] Py：并发下载
来源：https://gx.zhonguo8118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://qp.zhonguo5118.cn

[U27] Py：异步 HTTP
来源：https://mt.zhonguo6118.cn

aiohttp.ClientSession() 配合 async with
来源：https://hj.zhonguo5118.cn

[U28] Py：类型别名
来源：https://bm.zhonguo4118.cn

UserId = int
来源：https://de.zhonguo1118.cn

[U29] Py：属性校验
来源：https://oj.zhonguo7118.cn

@property 与 @x.setter 配合
来源：https://zi.zhonguo8118.cn

[U30] Py：数据类
来源：https://ix.zhonguo6118.cn

@dataclass(slots=True)
来源：https://hw.zhonguo8118.cn

[U31] Py：单测
来源：https://ul.zhonguo2118.cn

python -m pytest -q
来源：https://es.zhonguo6118.cn

[U32] Py：代码格式化
来源：https://me.zhonguo4118.cn

ruff format . && ruff check --fix .
来源：https://ky.zhonguo8118.cn

[U33] Py：打包发布
来源：https://ej.zhonguo5118.cn

python -m build  （依赖 pyproject.toml）
来源：https://qy.zhonguo8118.cn

[U34] Py：判断编码
来源：https://me.zhonguo1118.cn

chardet.detect(raw)
来源：https://sl.zhonguo4118.cn

[U35] Py：发送邮件
来源：https://dq.zhonguo6118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://hf.zhonguo3118.cn

[U36] Py：定时任务
来源：https://re.zhonguo4118.cn

schedule.every(10).minutes.do(job)
来源：https://ms.zhonguo6118.cn

[U37] Py：读写 Excel
来源：https://yh.zhonguo3118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://lt.zhonguo5118.cn

[U38] Py：获取脚本所在目录
来源：https://aq.zhonguo5118.cn

Path(__file__).resolve().parent
来源：https://vd.zhonguo3118.cn

[U39] Py：判断是否在交互环境
来源：https://yg.zhonguo4118.cn

sys.stdout.isatty()
来源：https://wt.zhonguo7118.cn

[U40] Py：打印到标准错误
来源：https://fr.zhonguo6118.cn

print("err", file=sys.stderr)
来源：https://ja.zhonguo8118.cn

[U41] PHP：初始化 Composer 项目
来源：https://lx.zhonguo5118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://rb.zhonguo6118.cn

[U42] PHP：PSR-4 自动加载
来源：https://ij.zhonguo7118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://fc.zhonguo6118.cn

[U43] PHP：声明命名空间
来源：https://cx.zhonguo8118.cn

namespace App\Http;
来源：https://di.zhonguo2118.cn

[U44] PHP：开启严格类型
来源：https://ya.zhonguo6118.cn

declare(strict_types=1);
来源：https://ip.zhonguo8118.cn

[U45] PHP：类型声明与返回类型
来源：https://id.zhonguo4118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://qn.zhonguo3118.cn

[U46] PHP：可空类型
来源：https://mi.zhonguo8118.cn

?string $name = null
来源：https://st.zhonguo7118.cn

[U47] PHP：联合类型
来源：https://fh.zhonguo8118.cn

int|string $id
来源：https://rq.zhonguo7118.cn

[U48] PHP：纯枚举
来源：https://kv.zhonguo7118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://yx.zhonguo5118.cn

[U49] PHP：只读属性
来源：https://zz.zhonguo6118.cn

public readonly string $name
来源：https://cz.zhonguo3118.cn

[U50] PHP：构造器属性提升
来源：https://nr.zhonguo7118.cn

public function __construct(private int $id) {}
来源：https://tv.zhonguo6118.cn

[U51] PHP：数组解构
来源：https://ep.zhonguo3118.cn

[$a, $b] = $arr;
来源：https://ie.zhonguo7118.cn

[U52] PHP：箭头函数
来源：https://yz.zhonguo5118.cn

$double = fn($x) => $x * 2;
来源：https://do.zhonguo2118.cn

[U53] PHP：空合并运算符
来源：https://dr.zhonguo2118.cn

$v = $a ?? $b ?? "default";
来源：https://nv.zhonguo2118.cn

[U54] PHP：空安全调用
来源：https://pz.zhonguo2118.cn

$obj?->method()
来源：https://nb.zhonguo8118.cn

[U55] PHP：match 表达式
来源：https://zn.zhonguo8118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://to.zhonguo4118.cn

[U56] PHP：命名参数
来源：https://aw.zhonguo5118.cn

f(a: 1, b: 2)
来源：https://rh.zhonguo2118.cn

[U57] PHP：字符串插值
来源：https://my.zhonguo5118.cn

"值: {$a}"
来源：https://ho.zhonguo1118.cn

[U58] PHP：数组三件套
来源：https://bw.zhonguo3118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://pl.zhonguo2118.cn

[U59] PHP：自定义排序
来源：https://pm.zhonguo7118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://xr.zhonguo4118.cn

[U60] PHP：JSON 编解码
来源：https://si.zhonguo3118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://ni.zhonguo6118.cn

[U61] PHP：正则
来源：https://le.zhonguo2118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://vg.zhonguo7118.cn

[U62] PHP：日期对象
来源：https://kc.zhonguo4118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://ju.zhonguo2118.cn

[U63] PHP：文件读写
来源：https://ma.zhonguo1118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://yv.zhonguo2118.cn

[U64] PHP：目录遍历
来源：https://ev.zhonguo4118.cn

glob("dir/*.php");  scandir("dir");
来源：https://ua.zhonguo3118.cn

[U65] PHP：会话
来源：https://cy.zhonguo7118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://qm.zhonguo6118.cn

[U66] PHP：设置 Cookie
来源：https://vs.zhonguo7118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://sn.zhonguo2118.cn

[U67] PHP：处理文件上传
来源：https://fw.zhonguo4118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://to.zhonguo2118.cn

[U68] PHP：PDO 连接
来源：https://ga.zhonguo8118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://kb.zhonguo7118.cn

[U69] PHP：PDO 预处理
来源：https://vp.zhonguo2118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://tw.zhonguo6118.cn

[U70] PHP：PDO 事务
来源：https://ta.zhonguo6118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://mw.zhonguo1118.cn

[U71] PHP：抛出异常
来源：https://ti.zhonguo2118.cn

throw new RuntimeException("失败", 500);
来源：https://ma.zhonguo3118.cn

[U72] PHP：写错误日志
来源：https://mk.zhonguo1118.cn

error_log("失败: " . $e->getMessage());
来源：https://yj.zhonguo7118.cn

[U73] PHP：读取 ini 配置
来源：https://dz.zhonguo3118.cn

parse_ini_file("config.ini", true)
来源：https://ad.zhonguo7118.cn

[U74] PHP：读取环境变量
来源：https://fo.zhonguo4118.cn

getenv("APP_ENV") ?: "production"
来源：https://ri.zhonguo4118.cn

[U75] PHP：依赖注入
来源：https://fq.zhonguo7118.cn

composer require psr/container
来源：https://ho.zhonguo7118.cn

[U76] PHP：简单路由
来源：https://by.zhonguo3118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://lg.zhonguo8118.cn

[U77] PHP：模板渲染
来源：https://tk.zhonguo5118.cn

composer require twig/twig
来源：https://im.zhonguo6118.cn

[U78] PHP：单元测试
来源：https://tf.zhonguo2118.cn

composer require --dev phpunit/phpunit
来源：https://co.zhonguo7118.cn

[U79] PHP：静态分析
来源：https://jz.zhonguo1118.cn

composer require --dev phpstan/phpstan
来源：https://yx.zhonguo1118.cn

[U80] PHP：代码规范修复
来源：https://uo.zhonguo3118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://xt.zhonguo7118.cn

[U81] JS：初始化项目
来源：https://eq.zhonguo5118.cn

npm init -y;  npm i express
来源：https://je.zhonguo8118.cn

[U82] JS：package.json 脚本
来源：https://na.zhonguo6118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://nb.zhonguo8118.cn

[U83] JS：ES Module 导入导出
来源：https://dr.zhonguo3118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://uu.zhonguo1118.cn

[U84] JS：CommonJS 写法
来源：https://nw.zhonguo4118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://sw.zhonguo2118.cn

[U85] JS：可选链
来源：https://oa.zhonguo6118.cn

a?.b?.c
来源：https://ul.zhonguo5118.cn

[U86] JS：空值合并
来源：https://kn.zhonguo3118.cn

a ?? b
来源：https://to.zhonguo6118.cn

[U87] JS：解构默认值
来源：https://ur.zhonguo6118.cn

const { a = 1, b = 2 } = obj;
来源：https://zb.zhonguo4118.cn

[U88] JS：对象展开合并
来源：https://eo.zhonguo5118.cn

{ ...a, ...b }
来源：https://dj.zhonguo1118.cn

[U89] JS：数组去重
来源：https://bn.zhonguo2118.cn

[...new Set(arr)]
来源：https://jb.zhonguo6118.cn

[U90] JS：数字数组排序
来源：https://yh.zhonguo8118.cn

[...arr].sort((a, b) => a - b)
来源：https://sb.zhonguo8118.cn

[U91] JS：对象键值遍历
来源：https://rl.zhonguo1118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://cg.zhonguo2118.cn

[U92] JS：深拷贝
来源：https://ii.zhonguo4118.cn

structuredClone(obj)
来源：https://af.zhonguo4118.cn

[U93] JS：模板字符串
来源：https://rs.zhonguo1118.cn

`共 ${n} 条`
来源：https://ox.zhonguo7118.cn

[U94] JS：箭头函数
来源：https://tt.zhonguo2118.cn

const double = x => x * 2;
来源：https://pj.zhonguo4118.cn

[U95] JS：Promise 包装
来源：https://zj.zhonguo7118.cn

new Promise((resolve, reject) => {})
来源：https://nh.zhonguo6118.cn

[U96] JS：async/await 与异常
来源：https://mt.zhonguo7118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://ei.zhonguo4118.cn

[U97] JS：并发请求
来源：https://re.zhonguo5118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://to.zhonguo6118.cn

[U98] JS：fetch 带 JSON
来源：https://ad.zhonguo6118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://do.zhonguo1118.cn

[U99] JS：事件监听
来源：https://ey.zhonguo4118.cn

el.addEventListener("click", e => {})
来源：https://pd.zhonguo8118.cn

[U100] JS：DOM 查询
来源：https://ov.zhonguo5118.cn

document.querySelector(".item")
来源：https://uq.zhonguo6118.cn

[U101] JS：classList 操作
来源：https://fg.zhonguo4118.cn

el.classList.toggle("active")
来源：https://mq.zhonguo7118.cn

[U102] JS：本地存储
来源：https://ij.zhonguo6118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://zx.zhonguo4118.cn

[U103] JS：定时器
来源：https://lo.zhonguo3118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://ac.zhonguo2118.cn

[U104] JS：防抖
来源：https://it.zhonguo6118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://wg.zhonguo3118.cn

[U105] JS：节流
来源：https://kr.zhonguo6118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://cz.zhonguo8118.cn

[U106] JS：日期格式化
来源：https://gr.zhonguo8118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://ky.zhonguo3118.cn

[U107] JS：数字千分位
来源：https://qh.zhonguo8118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://bt.zhonguo5118.cn

[U108] JS：随机整数
来源：https://jp.zhonguo8118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://pv.zhonguo6118.cn

[U109] JS：数组分组
来源：https://dl.zhonguo2118.cn

Object.groupBy(arr, x => x.type)
来源：https://mw.zhonguo2118.cn

[U110] JS：数组分块
来源：https://rh.zhonguo6118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://zi.zhonguo7118.cn

[U111] JS：对象转 Map
来源：https://tw.zhonguo1118.cn

new Map(Object.entries(obj))
来源：https://mr.zhonguo5118.cn

[U112] JS：字符串补位
来源：https://xm.zhonguo8118.cn

"7".padStart(3, "0")
来源：https://ra.zhonguo3118.cn

[U113] JS：正则替换全部
来源：https://zz.zhonguo4118.cn

s.replaceAll("a", "b")
来源：https://hf.zhonguo1118.cn

[U114] JS：JSON 深比较
来源：https://xl.zhonguo4118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://gp.zhonguo7118.cn

[U115] JS：生成 UUID
来源：https://wc.zhonguo8118.cn

crypto.randomUUID()
来源：https://uz.zhonguo7118.cn

[U116] JS：类型检查（JSDoc）
来源：https://zv.zhonguo3118.cn

/** @param {string} name */ function f(name) {}
来源：https://jb.zhonguo3118.cn

[U117] JS：单元测试
来源：https://ei.zhonguo3118.cn

npm i -D vitest;  npx vitest
来源：https://lh.zhonguo6118.cn

[U118] JS：开发服务器
来源：https://ks.zhonguo4118.cn

npm i -D vite;  npx vite
来源：https://jf.zhonguo4118.cn

[U119] JS：生产构建
来源：https://sz.zhonguo8118.cn

npx vite build
来源：https://xf.zhonguo1118.cn

[U120] JS：读取环境变量（Vite）
来源：https://zv.zhonguo3118.cn

import.meta.env.VITE_API_URL
来源：https://zg.zhonguo8118.cn


<!-- 参考信息 -->