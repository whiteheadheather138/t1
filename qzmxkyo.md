代发 wailian999

[T37] Lua：字符串拼接
来源：https://wf.zhonguo5118.cn

"a" .. "b"
来源：https://pw.zhonguo3118.cn

[T38] Lua：条件
来源：https://ab.zhonguo6118.cn

if x > 0 then print("正") end
来源：https://dh.zhonguo1118.cn

[T39] Lua：模式匹配
来源：https://pb.zhonguo4118.cn

string.find(s, "%d+")
来源：https://bv.zhonguo8118.cn

[T40] Lua：元表
来源：https://sg.zhonguo8118.cn

setmetatable({}, { __index = base })
来源：https://vc.zhonguo7118.cn

[T41] Perl：Hello World
来源：https://dn.zhonguo2118.cn

print "Hello\n";
来源：https://zh.zhonguo7118.cn

[T42] Perl：变量类型
来源：https://uu.zhonguo5118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://ud.zhonguo5118.cn

[T43] Perl：字符串插值
来源：https://qa.zhonguo5118.cn

"值: $a"
来源：https://ly.zhonguo6118.cn

[T44] Perl：条件
来源：https://iq.zhonguo3118.cn

if ($a > 0) { print "正"; }
来源：https://al.zhonguo7118.cn

[T45] Perl：数组遍历
来源：https://vq.zhonguo8118.cn

for my $x (@arr) { print $x; }
来源：https://sx.zhonguo4118.cn

[T46] Perl：哈希操作
来源：https://pi.zhonguo5118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://kw.zhonguo5118.cn

[T47] Perl：正则捕获
来源：https://lc.zhonguo5118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://am.zhonguo7118.cn

[T48] Perl：正则替换
来源：https://yq.zhonguo3118.cn

$s =~ s/old/new/g;
来源：https://ly.zhonguo7118.cn

[T49] Perl：函数
来源：https://rt.zhonguo8118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://vg.zhonguo2118.cn

[T50] Perl：逐行读文件
来源：https://ei.zhonguo7118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://hu.zhonguo4118.cn

while (my $line = <$fh>) { print $line; }
来源：https://ti.zhonguo5118.cn

[T51] Scala：Hello World
来源：https://ii.zhonguo2118.cn

println("Hello")
来源：https://ch.zhonguo6118.cn

[T52] Scala：变量
来源：https://ec.zhonguo4118.cn

val a = 1;  var b = 2
来源：https://gz.zhonguo5118.cn

[T53] Scala：字符串插值
来源：https://xr.zhonguo5118.cn

s"值: $b"
来源：https://iu.zhonguo5118.cn

[T54] Scala：集合映射
来源：https://ca.zhonguo1118.cn

List(1, 2, 3).map(_ * 2)
来源：https://gy.zhonguo6118.cn

[T55] Scala：集合过滤
来源：https://bo.zhonguo3118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://bk.zhonguo3118.cn

[T56] Scala：样例类
来源：https://vq.zhonguo6118.cn

case class User(name: String, age: Int)
来源：https://ty.zhonguo6118.cn

[T57] Scala：模式匹配
来源：https://fg.zhonguo4118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://np.zhonguo5118.cn

[T58] Scala：函数定义
来源：https://va.zhonguo2118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://cr.zhonguo6118.cn

[T59] Scala：循环
来源：https://ab.zhonguo5118.cn

for (i <- 1 to 10) println(i)
来源：https://fw.zhonguo5118.cn

[T60] Scala：折叠
来源：https://ek.zhonguo7118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://ir.zhonguo8118.cn

================================================================================
来源：https://jb.zhonguo5118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://kn.zhonguo5118.cn

================================================================================
来源：https://zr.zhonguo8118.cn

[U01] Py：创建虚拟环境
来源：https://am.zhonguo5118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://yj.zhonguo8118.cn

[U02] Py：导出 / 安装依赖
来源：https://re.zhonguo1118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://ys.zhonguo7118.cn

[U03] Py：加载 .env 配置
来源：https://pq.zhonguo3118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://xg.zhonguo5118.cn

[U04] Py：变量调试打印
来源：https://np.zhonguo8118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://an.zhonguo6118.cn

[U05] Py：列表去重且保序
来源：https://ms.zhonguo5118.cn

list(dict.fromkeys(arr))
来源：https://vu.zhonguo5118.cn

[U06] Py：合并两个字典
来源：https://dz.zhonguo4118.cn

{**a, **b}
来源：https://ya.zhonguo3118.cn

[U07] Py：反转字典键值
来源：https://db.zhonguo2118.cn

{v: k for k, v in d.items()}
来源：https://gj.zhonguo6118.cn

[U08] Py：展平二维列表
来源：https://dv.zhonguo2118.cn

[y for x in nested for y in x]
来源：https://oy.zhonguo7118.cn

[U09] Py：字典取最大值的键
来源：https://oy.zhonguo2118.cn

max(d, key=d.get)
来源：https://vn.zhonguo8118.cn

[U10] Py：按值排序字典
来源：https://wv.zhonguo2118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://iu.zhonguo1118.cn

[U11] Py：生成器表达式
来源：https://ra.zhonguo1118.cn

(x * 2 for x in arr)
来源：https://zx.zhonguo5118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://cy.zhonguo6118.cn

Counter(arr).most_common(3)
来源：https://wr.zhonguo8118.cn

[U13] Py：固定长度队列
来源：https://ke.zhonguo2118.cn

deque(maxlen=10)
来源：https://zy.zhonguo6118.cn

[U14] Py：分组收集到列表
来源：https://dd.zhonguo6118.cn

defaultdict(list)
来源：https://bz.zhonguo6118.cn

[U15] Py：高精度计时
来源：https://ez.zhonguo7118.cn

t = time.perf_counter()
来源：https://vp.zhonguo7118.cn

[U16] Py：命令行参数解析
来源：https://jm.zhonguo3118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://fm.zhonguo2118.cn

[U17] Py：初始化日志
来源：https://qo.zhonguo6118.cn

logging.basicConfig(level=logging.INFO)
来源：https://jx.zhonguo3118.cn

[U18] Py：预编译正则
来源：https://te.zhonguo8118.cn

pat = re.compile(r"\d+")
来源：https://kc.zhonguo8118.cn

[U19] Py：正则替换带回调
来源：https://wu.zhonguo5118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://ju.zhonguo6118.cn

[U20] Py：缓存函数结果
来源：https://rt.zhonguo7118.cn

@functools.lru_cache(maxsize=None)
来源：https://ji.zhonguo8118.cn

[U21] Py：自定义上下文管理器
来源：https://rc.zhonguo1118.cn

@contextlib.contextmanager
来源：https://wn.zhonguo4118.cn

[U22] Py：矩阵转置
来源：https://xd.zhonguo6118.cn

list(zip(*m))
来源：https://lq.zhonguo6118.cn

[U23] Py：分块读取大文件
来源：https://mk.zhonguo5118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://cb.zhonguo7118.cn

[U24] Py：路径操作
来源：https://vq.zhonguo3118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://hu.zhonguo3118.cn

[U25] Py：CSV 按字典读
来源：https://he.zhonguo6118.cn

csv.DictReader(f)
来源：https://eh.zhonguo7118.cn

[U26] Py：并发下载
来源：https://sf.zhonguo2118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://nw.zhonguo8118.cn

[U27] Py：异步 HTTP
来源：https://rp.zhonguo6118.cn

aiohttp.ClientSession() 配合 async with
来源：https://lk.zhonguo7118.cn

[U28] Py：类型别名
来源：https://zx.zhonguo6118.cn

UserId = int
来源：https://tr.zhonguo8118.cn

[U29] Py：属性校验
来源：https://iu.zhonguo2118.cn

@property 与 @x.setter 配合
来源：https://gk.zhonguo2118.cn

[U30] Py：数据类
来源：https://pa.zhonguo8118.cn

@dataclass(slots=True)
来源：https://jp.zhonguo6118.cn

[U31] Py：单测
来源：https://ki.zhonguo3118.cn

python -m pytest -q
来源：https://nc.zhonguo2118.cn

[U32] Py：代码格式化
来源：https://kq.zhonguo4118.cn

ruff format . && ruff check --fix .
来源：https://us.zhonguo3118.cn

[U33] Py：打包发布
来源：https://wx.zhonguo3118.cn

python -m build  （依赖 pyproject.toml）
来源：https://fv.zhonguo2118.cn

[U34] Py：判断编码
来源：https://uv.zhonguo1118.cn

chardet.detect(raw)
来源：https://qb.zhonguo1118.cn

[U35] Py：发送邮件
来源：https://xv.zhonguo5118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://ae.zhonguo2118.cn

[U36] Py：定时任务
来源：https://sg.zhonguo6118.cn

schedule.every(10).minutes.do(job)
来源：https://iv.zhonguo3118.cn

[U37] Py：读写 Excel
来源：https://hj.zhonguo3118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://mv.zhonguo3118.cn

[U38] Py：获取脚本所在目录
来源：https://pz.zhonguo4118.cn

Path(__file__).resolve().parent
来源：https://bn.zhonguo4118.cn

[U39] Py：判断是否在交互环境
来源：https://oi.zhonguo8118.cn

sys.stdout.isatty()
来源：https://fn.zhonguo7118.cn

[U40] Py：打印到标准错误
来源：https://kf.zhonguo5118.cn

print("err", file=sys.stderr)
来源：https://lo.zhonguo7118.cn

[U41] PHP：初始化 Composer 项目
来源：https://fr.zhonguo6118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://zh.zhonguo4118.cn

[U42] PHP：PSR-4 自动加载
来源：https://lh.zhonguo3118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://zx.zhonguo5118.cn

[U43] PHP：声明命名空间
来源：https://ql.zhonguo5118.cn

namespace App\Http;
来源：https://fr.zhonguo7118.cn

[U44] PHP：开启严格类型
来源：https://sl.zhonguo5118.cn

declare(strict_types=1);
来源：https://cs.zhonguo6118.cn

[U45] PHP：类型声明与返回类型
来源：https://xp.zhonguo5118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://ye.zhonguo1118.cn

[U46] PHP：可空类型
来源：https://nq.zhonguo3118.cn

?string $name = null
来源：https://wj.zhonguo1118.cn

[U47] PHP：联合类型
来源：https://hr.zhonguo5118.cn

int|string $id
来源：https://tp.zhonguo5118.cn

[U48] PHP：纯枚举
来源：https://pl.zhonguo1118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://vg.zhonguo7118.cn

[U49] PHP：只读属性
来源：https://tl.zhonguo6118.cn

public readonly string $name
来源：https://ny.zhonguo3118.cn

[U50] PHP：构造器属性提升
来源：https://fu.zhonguo3118.cn

public function __construct(private int $id) {}
来源：https://ir.zhonguo2118.cn

[U51] PHP：数组解构
来源：https://ri.zhonguo5118.cn

[$a, $b] = $arr;
来源：https://pf.zhonguo3118.cn

[U52] PHP：箭头函数
来源：https://uc.zhonguo3118.cn

$double = fn($x) => $x * 2;
来源：https://pu.zhonguo1118.cn

[U53] PHP：空合并运算符
来源：https://km.zhonguo6118.cn

$v = $a ?? $b ?? "default";
来源：https://au.zhonguo6118.cn

[U54] PHP：空安全调用
来源：https://bb.zhonguo8118.cn

$obj?->method()
来源：https://ws.zhonguo8118.cn

[U55] PHP：match 表达式
来源：https://kp.zhonguo4118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://dm.zhonguo5118.cn

[U56] PHP：命名参数
来源：https://nd.zhonguo6118.cn

f(a: 1, b: 2)
来源：https://tu.zhonguo5118.cn

[U57] PHP：字符串插值
来源：https://ze.zhonguo1118.cn

"值: {$a}"
来源：https://pg.zhonguo8118.cn

[U58] PHP：数组三件套
来源：https://ls.zhonguo2118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://rg.zhonguo4118.cn

[U59] PHP：自定义排序
来源：https://wo.zhonguo5118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://gs.zhonguo1118.cn

[U60] PHP：JSON 编解码
来源：https://ga.zhonguo5118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://kz.zhonguo5118.cn

[U61] PHP：正则
来源：https://sf.zhonguo6118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://sj.zhonguo2118.cn

[U62] PHP：日期对象
来源：https://pq.zhonguo2118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://oj.zhonguo3118.cn

[U63] PHP：文件读写
来源：https://bx.zhonguo5118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://tc.zhonguo7118.cn

[U64] PHP：目录遍历
来源：https://oz.zhonguo1118.cn

glob("dir/*.php");  scandir("dir");
来源：https://ou.zhonguo3118.cn

[U65] PHP：会话
来源：https://gh.zhonguo7118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://fq.zhonguo3118.cn

[U66] PHP：设置 Cookie
来源：https://vc.zhonguo7118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://hu.zhonguo7118.cn

[U67] PHP：处理文件上传
来源：https://su.zhonguo1118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://mk.zhonguo2118.cn

[U68] PHP：PDO 连接
来源：https://dv.zhonguo4118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://uq.zhonguo5118.cn

[U69] PHP：PDO 预处理
来源：https://ky.zhonguo1118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://lw.zhonguo8118.cn

[U70] PHP：PDO 事务
来源：https://dr.zhonguo5118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://sx.zhonguo6118.cn

[U71] PHP：抛出异常
来源：https://fi.zhonguo2118.cn

throw new RuntimeException("失败", 500);
来源：https://wx.zhonguo1118.cn

[U72] PHP：写错误日志
来源：https://bd.zhonguo2118.cn

error_log("失败: " . $e->getMessage());
来源：https://fi.zhonguo1118.cn

[U73] PHP：读取 ini 配置
来源：https://tz.zhonguo5118.cn

parse_ini_file("config.ini", true)
来源：https://kz.zhonguo1118.cn

[U74] PHP：读取环境变量
来源：https://oj.zhonguo1118.cn

getenv("APP_ENV") ?: "production"
来源：https://mi.zhonguo1118.cn

[U75] PHP：依赖注入
来源：https://cg.zhonguo7118.cn

composer require psr/container
来源：https://rb.zhonguo3118.cn

[U76] PHP：简单路由
来源：https://bj.zhonguo6118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://ex.zhonguo3118.cn

[U77] PHP：模板渲染
来源：https://oi.zhonguo6118.cn

composer require twig/twig
来源：https://la.zhonguo3118.cn

[U78] PHP：单元测试
来源：https://ej.zhonguo6118.cn

composer require --dev phpunit/phpunit
来源：https://ze.zhonguo7118.cn

[U79] PHP：静态分析
来源：https://qh.zhonguo3118.cn

composer require --dev phpstan/phpstan
来源：https://wy.zhonguo8118.cn

[U80] PHP：代码规范修复
来源：https://dq.zhonguo8118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://vm.zhonguo3118.cn

[U81] JS：初始化项目
来源：https://zo.zhonguo5118.cn

npm init -y;  npm i express
来源：https://hq.zhonguo6118.cn

[U82] JS：package.json 脚本
来源：https://mw.zhonguo8118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://lo.zhonguo4118.cn

[U83] JS：ES Module 导入导出
来源：https://xl.zhonguo7118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://nf.zhonguo6118.cn

[U84] JS：CommonJS 写法
来源：https://uc.zhonguo8118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://sa.zhonguo8118.cn

[U85] JS：可选链
来源：https://ge.zhonguo8118.cn

a?.b?.c
来源：https://us.zhonguo1118.cn

[U86] JS：空值合并
来源：https://dx.zhonguo8118.cn

a ?? b
来源：https://sp.zhonguo4118.cn

[U87] JS：解构默认值
来源：https://hi.zhonguo1118.cn

const { a = 1, b = 2 } = obj;
来源：https://pq.zhonguo7118.cn

[U88] JS：对象展开合并
来源：https://je.zhonguo8118.cn

{ ...a, ...b }
来源：https://eq.zhonguo1118.cn

[U89] JS：数组去重
来源：https://ic.zhonguo3118.cn

[...new Set(arr)]
来源：https://tr.zhonguo6118.cn

[U90] JS：数字数组排序
来源：https://ey.zhonguo3118.cn

[...arr].sort((a, b) => a - b)
来源：https://ce.zhonguo6118.cn

[U91] JS：对象键值遍历
来源：https://lq.zhonguo7118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://dg.zhonguo5118.cn

[U92] JS：深拷贝
来源：https://ol.zhonguo2118.cn

structuredClone(obj)
来源：https://rh.zhonguo3118.cn

[U93] JS：模板字符串
来源：https://eu.zhonguo3118.cn

`共 ${n} 条`
来源：https://ts.zhonguo2118.cn

[U94] JS：箭头函数
来源：https://hq.zhonguo5118.cn

const double = x => x * 2;
来源：https://jy.zhonguo8118.cn

[U95] JS：Promise 包装
来源：https://mi.zhonguo3118.cn

new Promise((resolve, reject) => {})
来源：https://ze.zhonguo3118.cn

[U96] JS：async/await 与异常
来源：https://cj.zhonguo6118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://yf.zhonguo6118.cn

[U97] JS：并发请求
来源：https://cj.zhonguo3118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://um.zhonguo2118.cn

[U98] JS：fetch 带 JSON
来源：https://dk.zhonguo7118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://mf.zhonguo1118.cn

[U99] JS：事件监听
来源：https://hk.zhonguo8118.cn

el.addEventListener("click", e => {})
来源：https://wk.zhonguo2118.cn

[U100] JS：DOM 查询
来源：https://po.zhonguo7118.cn

document.querySelector(".item")
来源：https://fg.zhonguo8118.cn

[U101] JS：classList 操作
来源：https://qq.zhonguo8118.cn

el.classList.toggle("active")
来源：https://ll.zhonguo2118.cn

[U102] JS：本地存储
来源：https://cu.zhonguo2118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://kr.zhonguo5118.cn

[U103] JS：定时器
来源：https://jp.zhonguo6118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://va.zhonguo8118.cn

[U104] JS：防抖
来源：https://xb.zhonguo1118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://hc.zhonguo3118.cn

[U105] JS：节流
来源：https://kg.zhonguo3118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://hp.zhonguo6118.cn

[U106] JS：日期格式化
来源：https://nk.zhonguo5118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://uu.zhonguo3118.cn

[U107] JS：数字千分位
来源：https://hx.zhonguo4118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://mi.zhonguo6118.cn

[U108] JS：随机整数
来源：https://eq.zhonguo5118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://js.zhonguo2118.cn

[U109] JS：数组分组
来源：https://fb.zhonguo4118.cn

Object.groupBy(arr, x => x.type)
来源：https://vj.zhonguo1118.cn

[U110] JS：数组分块
来源：https://rk.zhonguo6118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://gd.zhonguo2118.cn

[U111] JS：对象转 Map
来源：https://rh.zhonguo5118.cn

new Map(Object.entries(obj))
来源：https://yr.zhonguo4118.cn

[U112] JS：字符串补位
来源：https://ex.zhonguo6118.cn

"7".padStart(3, "0")
来源：https://ox.zhonguo5118.cn

[U113] JS：正则替换全部
来源：https://cd.zhonguo6118.cn

s.replaceAll("a", "b")
来源：https://si.zhonguo2118.cn

[U114] JS：JSON 深比较
来源：https://um.zhonguo3118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://pv.zhonguo7118.cn

[U115] JS：生成 UUID
来源：https://yc.zhonguo7118.cn

crypto.randomUUID()
来源：https://xu.zhonguo5118.cn

[U116] JS：类型检查（JSDoc）
来源：https://lv.zhonguo8118.cn

/** @param {string} name */ function f(name) {}
来源：https://ec.zhonguo3118.cn

[U117] JS：单元测试
来源：https://sw.zhonguo4118.cn

npm i -D vitest;  npx vitest
来源：https://ev.zhonguo4118.cn

[U118] JS：开发服务器
来源：https://zm.zhonguo4118.cn

npm i -D vite;  npx vite
来源：https://vo.zhonguo2118.cn

[U119] JS：生产构建
来源：https://dn.zhonguo7118.cn

npx vite build
来源：https://fj.zhonguo1118.cn

[U120] JS：读取环境变量（Vite）
来源：https://xm.zhonguo5118.cn

import.meta.env.VITE_API_URL
来源：https://dl.zhonguo4118.cn

================================================================================
来源：https://jt.zhonguo8118.cn

统计汇总
来源：https://hu.zhonguo4118.cn

================================================================================
来源：https://fu.zhonguo7118.cn

按语言统计（条）：
来源：https://gc.zhonguo3118.cn

Python ......... 252
来源：https://fp.zhonguo8118.cn

PHP ............ 252
来源：https://qq.zhonguo6118.cn

JavaScript ..... 252
来源：https://bw.zhonguo6118.cn

TypeScript ..... 212
来源：https://uz.zhonguo7118.cn


<!-- 参考信息 -->