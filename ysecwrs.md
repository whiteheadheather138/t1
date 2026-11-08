代发 wailian999

[T33] Lua：表（数组）
来源：https://yv.zhonguo8118.cn

local t = {1, 2, 3};  t[4] = 4
来源：https://cg.zhonguo4118.cn

[T34] Lua：遍历表
来源：https://xv.zhonguo2118.cn

for i, v in ipairs(t) do print(i, v) end
来源：https://ib.zhonguo2118.cn

[T35] Lua：字典表
来源：https://qe.zhonguo2118.cn

local d = { a = 1 };  d.b = 2
来源：https://gg.zhonguo7118.cn

[T36] Lua：函数
来源：https://fx.zhonguo2118.cn

function add(a, b) return a + b end
来源：https://xn.zhonguo7118.cn

[T37] Lua：字符串拼接
来源：https://bp.zhonguo8118.cn

"a" .. "b"
来源：https://rb.zhonguo5118.cn

[T38] Lua：条件
来源：https://gi.zhonguo3118.cn

if x > 0 then print("正") end
来源：https://cj.zhonguo6118.cn

[T39] Lua：模式匹配
来源：https://va.zhonguo4118.cn

string.find(s, "%d+")
来源：https://sm.zhonguo3118.cn

[T40] Lua：元表
来源：https://br.zhonguo1118.cn

setmetatable({}, { __index = base })
来源：https://di.zhonguo7118.cn

[T41] Perl：Hello World
来源：https://ly.zhonguo7118.cn

print "Hello\n";
来源：https://km.zhonguo2118.cn

[T42] Perl：变量类型
来源：https://qh.zhonguo8118.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：https://ot.zhonguo4118.cn

[T43] Perl：字符串插值
来源：https://po.zhonguo6118.cn

"值: $a"
来源：https://ax.zhonguo3118.cn

[T44] Perl：条件
来源：https://zg.zhonguo7118.cn

if ($a > 0) { print "正"; }
来源：https://xi.zhonguo8118.cn

[T45] Perl：数组遍历
来源：https://dd.zhonguo7118.cn

for my $x (@arr) { print $x; }
来源：https://ig.zhonguo5118.cn

[T46] Perl：哈希操作
来源：https://wr.zhonguo3118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://mr.zhonguo5118.cn

[T47] Perl：正则捕获
来源：https://un.zhonguo4118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://pw.zhonguo2118.cn

[T48] Perl：正则替换
来源：https://re.zhonguo2118.cn

$s =~ s/old/new/g;
来源：https://wd.zhonguo1118.cn

[T49] Perl：函数
来源：https://qy.zhonguo2118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://cp.zhonguo7118.cn

[T50] Perl：逐行读文件
来源：https://qx.zhonguo5118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://mw.zhonguo7118.cn

while (my $line = <$fh>) { print $line; }
来源：https://vu.zhonguo1118.cn

[T51] Scala：Hello World
来源：https://hm.zhonguo5118.cn

println("Hello")
来源：https://jg.zhonguo2118.cn

[T52] Scala：变量
来源：https://lr.zhonguo7118.cn

val a = 1;  var b = 2
来源：https://bs.zhonguo6118.cn

[T53] Scala：字符串插值
来源：https://bo.zhonguo5118.cn

s"值: $b"
来源：https://dv.zhonguo4118.cn

[T54] Scala：集合映射
来源：https://kc.zhonguo4118.cn

List(1, 2, 3).map(_ * 2)
来源：https://ol.zhonguo8118.cn

[T55] Scala：集合过滤
来源：https://pc.zhonguo3118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://hf.zhonguo6118.cn

[T56] Scala：样例类
来源：https://ih.zhonguo1118.cn

case class User(name: String, age: Int)
来源：https://io.zhonguo2118.cn

[T57] Scala：模式匹配
来源：https://dp.zhonguo6118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://qm.zhonguo2118.cn

[T58] Scala：函数定义
来源：https://jx.zhonguo2118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://wz.zhonguo4118.cn

[T59] Scala：循环
来源：https://hj.zhonguo6118.cn

for (i <- 1 to 10) println(i)
来源：https://fd.zhonguo3118.cn

[T60] Scala：折叠
来源：https://hv.zhonguo2118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://dk.zhonguo7118.cn

================================================================================
来源：https://uz.zhonguo6118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://of.zhonguo8118.cn

================================================================================
来源：https://td.zhonguo2118.cn

[U01] Py：创建虚拟环境
来源：https://bu.zhonguo3118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://ge.zhonguo1118.cn

[U02] Py：导出 / 安装依赖
来源：https://vm.zhonguo4118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://on.zhonguo3118.cn

[U03] Py：加载 .env 配置
来源：https://lv.zhonguo6118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://xu.zhonguo2118.cn

[U04] Py：变量调试打印
来源：https://rk.zhonguo5118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://qq.zhonguo3118.cn

[U05] Py：列表去重且保序
来源：https://fs.zhonguo8118.cn

list(dict.fromkeys(arr))
来源：https://xb.zhonguo3118.cn

[U06] Py：合并两个字典
来源：https://qq.zhonguo2118.cn

{**a, **b}
来源：https://ge.zhonguo7118.cn

[U07] Py：反转字典键值
来源：https://tf.zhonguo5118.cn

{v: k for k, v in d.items()}
来源：https://yf.zhonguo6118.cn

[U08] Py：展平二维列表
来源：https://lp.zhonguo3118.cn

[y for x in nested for y in x]
来源：https://rs.zhonguo6118.cn

[U09] Py：字典取最大值的键
来源：https://ea.zhonguo4118.cn

max(d, key=d.get)
来源：https://nl.zhonguo1118.cn

[U10] Py：按值排序字典
来源：https://fb.zhonguo1118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://cp.zhonguo6118.cn

[U11] Py：生成器表达式
来源：https://yd.zhonguo5118.cn

(x * 2 for x in arr)
来源：https://xc.zhonguo6118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://cq.zhonguo7118.cn

Counter(arr).most_common(3)
来源：https://wn.zhonguo2118.cn

[U13] Py：固定长度队列
来源：https://te.zhonguo1118.cn

deque(maxlen=10)
来源：https://cn.zhonguo4118.cn

[U14] Py：分组收集到列表
来源：https://wu.zhonguo5118.cn

defaultdict(list)
来源：https://vn.zhonguo1118.cn

[U15] Py：高精度计时
来源：https://ui.zhonguo3118.cn

t = time.perf_counter()
来源：https://mj.zhonguo1118.cn

[U16] Py：命令行参数解析
来源：https://gk.zhonguo7118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://bt.zhonguo7118.cn

[U17] Py：初始化日志
来源：https://cw.zhonguo8118.cn

logging.basicConfig(level=logging.INFO)
来源：https://zs.zhonguo4118.cn

[U18] Py：预编译正则
来源：https://jh.zhonguo7118.cn

pat = re.compile(r"\d+")
来源：https://py.zhonguo8118.cn

[U19] Py：正则替换带回调
来源：https://rl.zhonguo5118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://hd.zhonguo5118.cn

[U20] Py：缓存函数结果
来源：https://pr.zhonguo6118.cn

@functools.lru_cache(maxsize=None)
来源：https://tn.zhonguo5118.cn

[U21] Py：自定义上下文管理器
来源：https://hk.zhonguo6118.cn

@contextlib.contextmanager
来源：https://kn.zhonguo6118.cn

[U22] Py：矩阵转置
来源：https://wh.zhonguo6118.cn

list(zip(*m))
来源：https://vi.zhonguo3118.cn

[U23] Py：分块读取大文件
来源：https://lk.zhonguo6118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://sy.zhonguo3118.cn

[U24] Py：路径操作
来源：https://ls.zhonguo3118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://kn.zhonguo5118.cn

[U25] Py：CSV 按字典读
来源：https://jm.zhonguo5118.cn

csv.DictReader(f)
来源：https://bt.zhonguo6118.cn

[U26] Py：并发下载
来源：https://on.zhonguo3118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://oe.zhonguo7118.cn

[U27] Py：异步 HTTP
来源：https://wa.zhonguo6118.cn

aiohttp.ClientSession() 配合 async with
来源：https://ft.zhonguo1118.cn

[U28] Py：类型别名
来源：https://hj.zhonguo2118.cn

UserId = int
来源：https://la.zhonguo4118.cn

[U29] Py：属性校验
来源：https://ve.zhonguo7118.cn

@property 与 @x.setter 配合
来源：https://dt.zhonguo3118.cn

[U30] Py：数据类
来源：https://zk.zhonguo8118.cn

@dataclass(slots=True)
来源：https://pc.zhonguo5118.cn

[U31] Py：单测
来源：https://fi.zhonguo6118.cn

python -m pytest -q
来源：https://ei.zhonguo8118.cn

[U32] Py：代码格式化
来源：https://tz.zhonguo6118.cn

ruff format . && ruff check --fix .
来源：https://qj.zhonguo2118.cn

[U33] Py：打包发布
来源：https://as.zhonguo3118.cn

python -m build  （依赖 pyproject.toml）
来源：https://py.zhonguo7118.cn

[U34] Py：判断编码
来源：https://ll.zhonguo4118.cn

chardet.detect(raw)
来源：https://pw.zhonguo1118.cn

[U35] Py：发送邮件
来源：https://fc.zhonguo8118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://re.zhonguo1118.cn

[U36] Py：定时任务
来源：https://xy.zhonguo3118.cn

schedule.every(10).minutes.do(job)
来源：https://ns.zhonguo2118.cn

[U37] Py：读写 Excel
来源：https://im.zhonguo1118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://eg.zhonguo8118.cn

[U38] Py：获取脚本所在目录
来源：https://tw.zhonguo8118.cn

Path(__file__).resolve().parent
来源：https://tx.zhonguo3118.cn

[U39] Py：判断是否在交互环境
来源：https://vb.zhonguo5118.cn

sys.stdout.isatty()
来源：https://xu.zhonguo6118.cn

[U40] Py：打印到标准错误
来源：https://zv.zhonguo4118.cn

print("err", file=sys.stderr)
来源：https://wn.zhonguo2118.cn

[U41] PHP：初始化 Composer 项目
来源：https://yh.zhonguo1118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://ar.zhonguo6118.cn

[U42] PHP：PSR-4 自动加载
来源：https://wi.zhonguo6118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://cb.zhonguo3118.cn

[U43] PHP：声明命名空间
来源：https://ze.zhonguo3118.cn

namespace App\Http;
来源：https://jd.zhonguo7118.cn

[U44] PHP：开启严格类型
来源：https://kh.zhonguo7118.cn

declare(strict_types=1);
来源：https://kh.zhonguo5118.cn

[U45] PHP：类型声明与返回类型
来源：https://my.zhonguo3118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://ge.zhonguo8118.cn

[U46] PHP：可空类型
来源：https://es.zhonguo5118.cn

?string $name = null
来源：https://rk.zhonguo8118.cn

[U47] PHP：联合类型
来源：https://qw.zhonguo8118.cn

int|string $id
来源：https://zo.zhonguo1118.cn

[U48] PHP：纯枚举
来源：https://fa.zhonguo5118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://ab.zhonguo2118.cn

[U49] PHP：只读属性
来源：https://il.zhonguo6118.cn

public readonly string $name
来源：https://bd.zhonguo8118.cn

[U50] PHP：构造器属性提升
来源：https://bd.zhonguo4118.cn

public function __construct(private int $id) {}
来源：https://ok.zhonguo1118.cn

[U51] PHP：数组解构
来源：https://hv.zhonguo6118.cn

[$a, $b] = $arr;
来源：https://qu.zhonguo5118.cn

[U52] PHP：箭头函数
来源：https://xt.zhonguo1118.cn

$double = fn($x) => $x * 2;
来源：https://oq.zhonguo8118.cn

[U53] PHP：空合并运算符
来源：https://ea.zhonguo8118.cn

$v = $a ?? $b ?? "default";
来源：https://hh.zhonguo2118.cn

[U54] PHP：空安全调用
来源：https://ox.zhonguo4118.cn

$obj?->method()
来源：https://fb.zhonguo6118.cn

[U55] PHP：match 表达式
来源：https://bu.zhonguo3118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://iv.zhonguo6118.cn

[U56] PHP：命名参数
来源：https://af.zhonguo7118.cn

f(a: 1, b: 2)
来源：https://ju.zhonguo4118.cn

[U57] PHP：字符串插值
来源：https://qo.zhonguo5118.cn

"值: {$a}"
来源：https://ak.zhonguo2118.cn

[U58] PHP：数组三件套
来源：https://ch.zhonguo2118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://if.zhonguo6118.cn

[U59] PHP：自定义排序
来源：https://ue.zhonguo4118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://hh.zhonguo1118.cn

[U60] PHP：JSON 编解码
来源：https://sq.zhonguo6118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://ha.zhonguo5118.cn

[U61] PHP：正则
来源：https://xl.zhonguo3118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://xo.zhonguo8118.cn

[U62] PHP：日期对象
来源：https://kw.zhonguo6118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://ep.zhonguo8118.cn

[U63] PHP：文件读写
来源：https://ei.zhonguo3118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://jy.zhonguo4118.cn

[U64] PHP：目录遍历
来源：https://dl.zhonguo2118.cn

glob("dir/*.php");  scandir("dir");
来源：https://gp.zhonguo5118.cn

[U65] PHP：会话
来源：https://kw.zhonguo4118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://uv.zhonguo6118.cn

[U66] PHP：设置 Cookie
来源：https://zm.zhonguo1118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://oq.zhonguo6118.cn

[U67] PHP：处理文件上传
来源：https://lr.zhonguo8118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://dm.zhonguo6118.cn

[U68] PHP：PDO 连接
来源：https://zg.zhonguo7118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://cg.zhonguo8118.cn

[U69] PHP：PDO 预处理
来源：https://sz.zhonguo6118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://sy.zhonguo2118.cn

[U70] PHP：PDO 事务
来源：https://la.zhonguo6118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://hk.zhonguo4118.cn

[U71] PHP：抛出异常
来源：https://uc.zhonguo7118.cn

throw new RuntimeException("失败", 500);
来源：https://af.zhonguo1118.cn

[U72] PHP：写错误日志
来源：https://xd.zhonguo4118.cn

error_log("失败: " . $e->getMessage());
来源：https://yb.zhonguo2118.cn

[U73] PHP：读取 ini 配置
来源：https://sg.zhonguo6118.cn

parse_ini_file("config.ini", true)
来源：https://ky.zhonguo7118.cn

[U74] PHP：读取环境变量
来源：https://fr.zhonguo4118.cn

getenv("APP_ENV") ?: "production"
来源：https://mc.zhonguo1118.cn

[U75] PHP：依赖注入
来源：https://pz.zhonguo5118.cn

composer require psr/container
来源：https://tk.zhonguo6118.cn

[U76] PHP：简单路由
来源：https://vx.zhonguo7118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://fu.zhonguo8118.cn

[U77] PHP：模板渲染
来源：https://wz.zhonguo8118.cn

composer require twig/twig
来源：https://zg.zhonguo4118.cn

[U78] PHP：单元测试
来源：https://fv.zhonguo1118.cn

composer require --dev phpunit/phpunit
来源：https://rv.zhonguo6118.cn

[U79] PHP：静态分析
来源：https://ky.zhonguo3118.cn

composer require --dev phpstan/phpstan
来源：https://lf.zhonguo2118.cn

[U80] PHP：代码规范修复
来源：https://et.zhonguo8118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://yk.zhonguo2118.cn

[U81] JS：初始化项目
来源：https://va.zhonguo1118.cn

npm init -y;  npm i express
来源：https://nu.zhonguo6118.cn

[U82] JS：package.json 脚本
来源：https://bn.zhonguo2118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://ss.zhonguo6118.cn

[U83] JS：ES Module 导入导出
来源：https://he.zhonguo7118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://bh.zhonguo7118.cn

[U84] JS：CommonJS 写法
来源：https://oi.zhonguo7118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://ro.zhonguo8118.cn

[U85] JS：可选链
来源：https://us.zhonguo2118.cn

a?.b?.c
来源：https://lv.zhonguo3118.cn

[U86] JS：空值合并
来源：https://sg.zhonguo7118.cn

a ?? b
来源：https://wf.zhonguo6118.cn

[U87] JS：解构默认值
来源：https://us.zhonguo1118.cn

const { a = 1, b = 2 } = obj;
来源：https://ds.zhonguo6118.cn

[U88] JS：对象展开合并
来源：https://bo.zhonguo8118.cn

{ ...a, ...b }
来源：https://fm.zhonguo7118.cn

[U89] JS：数组去重
来源：https://jm.zhonguo6118.cn

[...new Set(arr)]
来源：https://wy.zhonguo3118.cn

[U90] JS：数字数组排序
来源：https://oj.zhonguo3118.cn

[...arr].sort((a, b) => a - b)
来源：https://dg.zhonguo8118.cn

[U91] JS：对象键值遍历
来源：https://am.zhonguo7118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://yo.zhonguo8118.cn

[U92] JS：深拷贝
来源：https://wb.zhonguo3118.cn

structuredClone(obj)
来源：https://dv.zhonguo4118.cn

[U93] JS：模板字符串
来源：https://nh.zhonguo2118.cn

`共 ${n} 条`
来源：https://lr.zhonguo6118.cn

[U94] JS：箭头函数
来源：https://bw.zhonguo8118.cn

const double = x => x * 2;
来源：https://ji.zhonguo8118.cn

[U95] JS：Promise 包装
来源：https://kn.zhonguo2118.cn

new Promise((resolve, reject) => {})
来源：https://wx.zhonguo2118.cn

[U96] JS：async/await 与异常
来源：https://zz.zhonguo8118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://hd.zhonguo5118.cn

[U97] JS：并发请求
来源：https://ez.zhonguo2118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://fw.zhonguo4118.cn

[U98] JS：fetch 带 JSON
来源：https://zt.zhonguo5118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://rc.zhonguo6118.cn

[U99] JS：事件监听
来源：https://ht.zhonguo2118.cn

el.addEventListener("click", e => {})
来源：https://xo.zhonguo6118.cn

[U100] JS：DOM 查询
来源：https://wb.zhonguo3118.cn

document.querySelector(".item")
来源：https://dn.zhonguo6118.cn

[U101] JS：classList 操作
来源：https://ys.zhonguo8118.cn

el.classList.toggle("active")
来源：https://lk.zhonguo7118.cn

[U102] JS：本地存储
来源：https://wj.zhonguo5118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://sn.zhonguo4118.cn

[U103] JS：定时器
来源：https://eu.zhonguo2118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://ft.zhonguo8118.cn

[U104] JS：防抖
来源：https://ki.zhonguo8118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://cw.zhonguo8118.cn

[U105] JS：节流
来源：https://mm.zhonguo6118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://wu.zhonguo3118.cn

[U106] JS：日期格式化
来源：https://vh.zhonguo5118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://gj.zhonguo3118.cn

[U107] JS：数字千分位
来源：https://tw.zhonguo1118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://dk.zhonguo5118.cn

[U108] JS：随机整数
来源：https://pz.zhonguo5118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://te.zhonguo3118.cn

[U109] JS：数组分组
来源：https://xs.zhonguo6118.cn

Object.groupBy(arr, x => x.type)
来源：https://sk.zhonguo6118.cn

[U110] JS：数组分块
来源：https://ke.zhonguo7118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://su.zhonguo2118.cn

[U111] JS：对象转 Map
来源：https://bo.zhonguo3118.cn

new Map(Object.entries(obj))
来源：https://dd.zhonguo1118.cn

[U112] JS：字符串补位
来源：https://um.zhonguo1118.cn

"7".padStart(3, "0")
来源：https://cc.zhonguo4118.cn

[U113] JS：正则替换全部
来源：https://os.zhonguo7118.cn

s.replaceAll("a", "b")
来源：https://bm.zhonguo2118.cn

[U114] JS：JSON 深比较
来源：https://hu.zhonguo5118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://nf.zhonguo8118.cn

[U115] JS：生成 UUID
来源：https://sl.zhonguo7118.cn

crypto.randomUUID()
来源：https://jj.zhonguo4118.cn

[U116] JS：类型检查（JSDoc）
来源：https://gv.zhonguo2118.cn

/** @param {string} name */ function f(name) {}
来源：https://gp.zhonguo7118.cn

[U117] JS：单元测试
来源：https://mq.zhonguo1118.cn

npm i -D vitest;  npx vitest
来源：https://eq.zhonguo8118.cn

[U118] JS：开发服务器
来源：https://qk.zhonguo5118.cn

npm i -D vite;  npx vite
来源：https://sg.zhonguo4118.cn

[U119] JS：生产构建
来源：https://wu.zhonguo7118.cn

npx vite build
来源：https://sf.zhonguo7118.cn

[U120] JS：读取环境变量（Vite）
来源：https://lc.zhonguo4118.cn

import.meta.env.VITE_API_URL
来源：https://vf.zhonguo8118.cn


<!-- 参考信息 -->