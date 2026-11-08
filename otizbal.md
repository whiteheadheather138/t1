代发 wailian999

[T43] Perl：字符串插值
来源：https://ew.zhonguo4118.cn

"值: $a"
来源：https://sl.zhonguo5118.cn

[T44] Perl：条件
来源：https://bu.zhonguo3118.cn

if ($a > 0) { print "正"; }
来源：https://gu.zhonguo1118.cn

[T45] Perl：数组遍历
来源：https://fs.zhonguo1118.cn

for my $x (@arr) { print $x; }
来源：https://yw.zhonguo6118.cn

[T46] Perl：哈希操作
来源：https://ja.zhonguo5118.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：https://ev.zhonguo3118.cn

[T47] Perl：正则捕获
来源：https://vi.zhonguo4118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://je.zhonguo7118.cn

[T48] Perl：正则替换
来源：https://qe.zhonguo8118.cn

$s =~ s/old/new/g;
来源：https://ca.zhonguo5118.cn

[T49] Perl：函数
来源：https://xl.zhonguo3118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://ri.zhonguo2118.cn

[T50] Perl：逐行读文件
来源：https://nc.zhonguo6118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://ik.zhonguo4118.cn

while (my $line = <$fh>) { print $line; }
来源：https://qm.zhonguo1118.cn

[T51] Scala：Hello World
来源：https://ov.zhonguo4118.cn

println("Hello")
来源：https://vc.zhonguo1118.cn

[T52] Scala：变量
来源：https://gt.zhonguo3118.cn

val a = 1;  var b = 2
来源：https://yr.zhonguo3118.cn

[T53] Scala：字符串插值
来源：https://xs.zhonguo5118.cn

s"值: $b"
来源：https://nl.zhonguo8118.cn

[T54] Scala：集合映射
来源：https://zy.zhonguo8118.cn

List(1, 2, 3).map(_ * 2)
来源：https://ob.zhonguo1118.cn

[T55] Scala：集合过滤
来源：https://ds.zhonguo2118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://mp.zhonguo1118.cn

[T56] Scala：样例类
来源：https://mm.zhonguo7118.cn

case class User(name: String, age: Int)
来源：https://as.zhonguo2118.cn

[T57] Scala：模式匹配
来源：https://tx.zhonguo2118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://bx.zhonguo1118.cn

[T58] Scala：函数定义
来源：https://sh.zhonguo7118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://zj.zhonguo3118.cn

[T59] Scala：循环
来源：https://ro.zhonguo6118.cn

for (i <- 1 to 10) println(i)
来源：https://cf.zhonguo3118.cn

[T60] Scala：折叠
来源：https://vd.zhonguo8118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://cr.zhonguo3118.cn

================================================================================
来源：https://lm.zhonguo6118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://lm.zhonguo1118.cn

================================================================================
来源：https://qp.zhonguo2118.cn

[U01] Py：创建虚拟环境
来源：https://dd.zhonguo4118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://jd.zhonguo3118.cn

[U02] Py：导出 / 安装依赖
来源：https://lz.zhonguo4118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://gr.zhonguo6118.cn

[U03] Py：加载 .env 配置
来源：https://tn.zhonguo5118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://jc.zhonguo1118.cn

[U04] Py：变量调试打印
来源：https://id.zhonguo4118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://ci.zhonguo4118.cn

[U05] Py：列表去重且保序
来源：https://vd.zhonguo6118.cn

list(dict.fromkeys(arr))
来源：https://xu.zhonguo6118.cn

[U06] Py：合并两个字典
来源：https://yt.zhonguo7118.cn

{**a, **b}
来源：https://gt.zhonguo6118.cn

[U07] Py：反转字典键值
来源：https://hf.zhonguo6118.cn

{v: k for k, v in d.items()}
来源：https://jz.zhonguo7118.cn

[U08] Py：展平二维列表
来源：https://pd.zhonguo1118.cn

[y for x in nested for y in x]
来源：https://vn.zhonguo8118.cn

[U09] Py：字典取最大值的键
来源：https://nw.zhonguo8118.cn

max(d, key=d.get)
来源：https://sm.zhonguo3118.cn

[U10] Py：按值排序字典
来源：https://sy.zhonguo8118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://pv.zhonguo3118.cn

[U11] Py：生成器表达式
来源：https://ts.zhonguo4118.cn

(x * 2 for x in arr)
来源：https://lu.zhonguo7118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://hc.zhonguo6118.cn

Counter(arr).most_common(3)
来源：https://da.zhonguo7118.cn

[U13] Py：固定长度队列
来源：https://oe.zhonguo4118.cn

deque(maxlen=10)
来源：https://kl.zhonguo2118.cn

[U14] Py：分组收集到列表
来源：https://nl.zhonguo5118.cn

defaultdict(list)
来源：https://sk.zhonguo1118.cn

[U15] Py：高精度计时
来源：https://pl.zhonguo5118.cn

t = time.perf_counter()
来源：https://tg.zhonguo3118.cn

[U16] Py：命令行参数解析
来源：https://sd.zhonguo4118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://su.zhonguo5118.cn

[U17] Py：初始化日志
来源：https://cn.zhonguo6118.cn

logging.basicConfig(level=logging.INFO)
来源：https://us.zhonguo8118.cn

[U18] Py：预编译正则
来源：https://gx.zhonguo2118.cn

pat = re.compile(r"\d+")
来源：https://va.zhonguo8118.cn

[U19] Py：正则替换带回调
来源：https://sh.zhonguo8118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://qe.zhonguo1118.cn

[U20] Py：缓存函数结果
来源：https://jp.zhonguo6118.cn

@functools.lru_cache(maxsize=None)
来源：https://pe.zhonguo5118.cn

[U21] Py：自定义上下文管理器
来源：https://uq.zhonguo8118.cn

@contextlib.contextmanager
来源：https://jo.zhonguo5118.cn

[U22] Py：矩阵转置
来源：https://mj.zhonguo3118.cn

list(zip(*m))
来源：https://uk.zhonguo4118.cn

[U23] Py：分块读取大文件
来源：https://yu.zhonguo8118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://yg.zhonguo8118.cn

[U24] Py：路径操作
来源：https://pw.zhonguo4118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://fo.zhonguo2118.cn

[U25] Py：CSV 按字典读
来源：https://np.zhonguo8118.cn

csv.DictReader(f)
来源：https://oi.zhonguo5118.cn

[U26] Py：并发下载
来源：https://nq.zhonguo5118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://pe.zhonguo6118.cn

[U27] Py：异步 HTTP
来源：https://pm.zhonguo7118.cn

aiohttp.ClientSession() 配合 async with
来源：https://nf.zhonguo2118.cn

[U28] Py：类型别名
来源：https://xl.zhonguo7118.cn

UserId = int
来源：https://kg.zhonguo4118.cn

[U29] Py：属性校验
来源：https://nx.zhonguo6118.cn

@property 与 @x.setter 配合
来源：https://ko.zhonguo6118.cn

[U30] Py：数据类
来源：https://ll.zhonguo4118.cn

@dataclass(slots=True)
来源：https://vv.zhonguo6118.cn

[U31] Py：单测
来源：https://id.zhonguo8118.cn

python -m pytest -q
来源：https://jr.zhonguo2118.cn

[U32] Py：代码格式化
来源：https://sf.zhonguo3118.cn

ruff format . && ruff check --fix .
来源：https://aa.zhonguo5118.cn

[U33] Py：打包发布
来源：https://kw.zhonguo4118.cn

python -m build  （依赖 pyproject.toml）
来源：https://oy.zhonguo7118.cn

[U34] Py：判断编码
来源：https://xp.zhonguo8118.cn

chardet.detect(raw)
来源：https://vb.zhonguo3118.cn

[U35] Py：发送邮件
来源：https://lx.zhonguo4118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://qg.zhonguo7118.cn

[U36] Py：定时任务
来源：https://vn.zhonguo6118.cn

schedule.every(10).minutes.do(job)
来源：https://kf.zhonguo4118.cn

[U37] Py：读写 Excel
来源：https://hh.zhonguo7118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://gb.zhonguo6118.cn

[U38] Py：获取脚本所在目录
来源：https://mq.zhonguo7118.cn

Path(__file__).resolve().parent
来源：https://is.zhonguo1118.cn

[U39] Py：判断是否在交互环境
来源：https://mx.zhonguo2118.cn

sys.stdout.isatty()
来源：https://no.zhonguo3118.cn

[U40] Py：打印到标准错误
来源：https://dv.zhonguo3118.cn

print("err", file=sys.stderr)
来源：https://tf.zhonguo6118.cn

[U41] PHP：初始化 Composer 项目
来源：https://ke.zhonguo6118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://iq.zhonguo2118.cn

[U42] PHP：PSR-4 自动加载
来源：https://am.zhonguo3118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://nu.zhonguo2118.cn

[U43] PHP：声明命名空间
来源：https://ri.zhonguo2118.cn

namespace App\Http;
来源：https://ux.zhonguo4118.cn

[U44] PHP：开启严格类型
来源：https://ma.zhonguo2118.cn

declare(strict_types=1);
来源：https://rs.zhonguo3118.cn

[U45] PHP：类型声明与返回类型
来源：https://bt.zhonguo3118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://ri.zhonguo7118.cn

[U46] PHP：可空类型
来源：https://lm.zhonguo4118.cn

?string $name = null
来源：https://rr.zhonguo3118.cn

[U47] PHP：联合类型
来源：https://dq.zhonguo4118.cn

int|string $id
来源：https://vf.zhonguo6118.cn

[U48] PHP：纯枚举
来源：https://sd.zhonguo7118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://ge.zhonguo1118.cn

[U49] PHP：只读属性
来源：https://um.zhonguo3118.cn

public readonly string $name
来源：https://nu.zhonguo1118.cn

[U50] PHP：构造器属性提升
来源：https://uu.zhonguo4118.cn

public function __construct(private int $id) {}
来源：https://my.zhonguo5118.cn

[U51] PHP：数组解构
来源：https://as.zhonguo5118.cn

[$a, $b] = $arr;
来源：https://ho.zhonguo6118.cn

[U52] PHP：箭头函数
来源：https://zz.zhonguo4118.cn

$double = fn($x) => $x * 2;
来源：https://cn.zhonguo1118.cn

[U53] PHP：空合并运算符
来源：https://dk.zhonguo5118.cn

$v = $a ?? $b ?? "default";
来源：https://qz.zhonguo5118.cn

[U54] PHP：空安全调用
来源：https://ds.zhonguo1118.cn

$obj?->method()
来源：https://qg.zhonguo3118.cn

[U55] PHP：match 表达式
来源：https://ut.zhonguo6118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://cv.zhonguo4118.cn

[U56] PHP：命名参数
来源：https://fh.zhonguo6118.cn

f(a: 1, b: 2)
来源：https://nm.zhonguo5118.cn

[U57] PHP：字符串插值
来源：https://sn.zhonguo7118.cn

"值: {$a}"
来源：https://lg.zhonguo5118.cn

[U58] PHP：数组三件套
来源：https://vf.zhonguo4118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://tq.zhonguo1118.cn

[U59] PHP：自定义排序
来源：https://jh.zhonguo2118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://ar.zhonguo4118.cn

[U60] PHP：JSON 编解码
来源：https://gx.zhonguo1118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://qz.zhonguo1118.cn

[U61] PHP：正则
来源：https://jk.zhonguo1118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://ez.zhonguo6118.cn

[U62] PHP：日期对象
来源：https://xm.zhonguo5118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://rw.zhonguo7118.cn

[U63] PHP：文件读写
来源：https://is.zhonguo2118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://gi.zhonguo3118.cn

[U64] PHP：目录遍历
来源：https://ht.zhonguo1118.cn

glob("dir/*.php");  scandir("dir");
来源：https://dn.zhonguo4118.cn

[U65] PHP：会话
来源：https://dl.zhonguo1118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://tg.zhonguo3118.cn

[U66] PHP：设置 Cookie
来源：https://pn.zhonguo1118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://hm.zhonguo3118.cn

[U67] PHP：处理文件上传
来源：https://lo.zhonguo5118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://xc.zhonguo8118.cn

[U68] PHP：PDO 连接
来源：https://rf.zhonguo6118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://rg.zhonguo1118.cn

[U69] PHP：PDO 预处理
来源：https://ml.zhonguo5118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://uo.zhonguo6118.cn

[U70] PHP：PDO 事务
来源：https://tp.zhonguo6118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://bk.zhonguo1118.cn

[U71] PHP：抛出异常
来源：https://rc.zhonguo2118.cn

throw new RuntimeException("失败", 500);
来源：https://fw.zhonguo7118.cn

[U72] PHP：写错误日志
来源：https://dl.zhonguo2118.cn

error_log("失败: " . $e->getMessage());
来源：https://ef.zhonguo7118.cn

[U73] PHP：读取 ini 配置
来源：https://iz.zhonguo2118.cn

parse_ini_file("config.ini", true)
来源：https://yw.zhonguo6118.cn

[U74] PHP：读取环境变量
来源：https://fd.zhonguo7118.cn

getenv("APP_ENV") ?: "production"
来源：https://at.zhonguo5118.cn

[U75] PHP：依赖注入
来源：https://jn.zhonguo8118.cn

composer require psr/container
来源：https://hg.zhonguo7118.cn

[U76] PHP：简单路由
来源：https://zq.zhonguo6118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://fz.zhonguo4118.cn

[U77] PHP：模板渲染
来源：https://tl.zhonguo4118.cn

composer require twig/twig
来源：https://fq.zhonguo8118.cn

[U78] PHP：单元测试
来源：https://at.zhonguo4118.cn

composer require --dev phpunit/phpunit
来源：https://bx.zhonguo5118.cn

[U79] PHP：静态分析
来源：https://rx.zhonguo8118.cn

composer require --dev phpstan/phpstan
来源：https://cv.zhonguo5118.cn

[U80] PHP：代码规范修复
来源：https://pz.zhonguo1118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://st.zhonguo3118.cn

[U81] JS：初始化项目
来源：https://je.zhonguo4118.cn

npm init -y;  npm i express
来源：https://tc.zhonguo4118.cn

[U82] JS：package.json 脚本
来源：https://jn.zhonguo8118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://xb.zhonguo3118.cn

[U83] JS：ES Module 导入导出
来源：https://al.zhonguo3118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://nx.zhonguo3118.cn

[U84] JS：CommonJS 写法
来源：https://cy.zhonguo8118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://bu.zhonguo4118.cn

[U85] JS：可选链
来源：https://ls.zhonguo4118.cn

a?.b?.c
来源：https://il.zhonguo5118.cn

[U86] JS：空值合并
来源：https://cl.zhonguo7118.cn

a ?? b
来源：https://dc.zhonguo4118.cn

[U87] JS：解构默认值
来源：https://wf.zhonguo5118.cn

const { a = 1, b = 2 } = obj;
来源：https://gs.zhonguo8118.cn

[U88] JS：对象展开合并
来源：https://zi.zhonguo5118.cn

{ ...a, ...b }
来源：https://xt.zhonguo7118.cn

[U89] JS：数组去重
来源：https://vq.zhonguo6118.cn

[...new Set(arr)]
来源：https://hg.zhonguo5118.cn

[U90] JS：数字数组排序
来源：https://xd.zhonguo4118.cn

[...arr].sort((a, b) => a - b)
来源：https://oe.zhonguo4118.cn

[U91] JS：对象键值遍历
来源：https://nq.zhonguo1118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://ev.zhonguo7118.cn

[U92] JS：深拷贝
来源：https://lp.zhonguo1118.cn

structuredClone(obj)
来源：https://ia.zhonguo1118.cn

[U93] JS：模板字符串
来源：https://fc.zhonguo5118.cn

`共 ${n} 条`
来源：https://mf.zhonguo5118.cn

[U94] JS：箭头函数
来源：https://rt.zhonguo3118.cn

const double = x => x * 2;
来源：https://vw.zhonguo2118.cn

[U95] JS：Promise 包装
来源：https://dm.zhonguo7118.cn

new Promise((resolve, reject) => {})
来源：https://cn.zhonguo2118.cn

[U96] JS：async/await 与异常
来源：https://hx.zhonguo4118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://qc.zhonguo2118.cn

[U97] JS：并发请求
来源：https://jn.zhonguo3118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://cd.zhonguo2118.cn

[U98] JS：fetch 带 JSON
来源：https://lf.zhonguo6118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://rz.zhonguo4118.cn

[U99] JS：事件监听
来源：https://rt.zhonguo5118.cn

el.addEventListener("click", e => {})
来源：https://vp.zhonguo4118.cn

[U100] JS：DOM 查询
来源：https://mw.zhonguo5118.cn

document.querySelector(".item")
来源：https://oe.zhonguo7118.cn

[U101] JS：classList 操作
来源：https://sa.zhonguo7118.cn

el.classList.toggle("active")
来源：https://op.zhonguo7118.cn

[U102] JS：本地存储
来源：https://xz.zhonguo7118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://aq.zhonguo3118.cn

[U103] JS：定时器
来源：https://eu.zhonguo1118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://rg.zhonguo3118.cn

[U104] JS：防抖
来源：https://aj.zhonguo8118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://bk.zhonguo8118.cn

[U105] JS：节流
来源：https://hp.zhonguo7118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://gq.zhonguo6118.cn

[U106] JS：日期格式化
来源：https://cl.zhonguo4118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://er.zhonguo3118.cn

[U107] JS：数字千分位
来源：https://zx.zhonguo8118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://ko.zhonguo1118.cn

[U108] JS：随机整数
来源：https://to.zhonguo6118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://hu.zhonguo6118.cn

[U109] JS：数组分组
来源：https://ly.zhonguo5118.cn

Object.groupBy(arr, x => x.type)
来源：https://sf.zhonguo2118.cn

[U110] JS：数组分块
来源：https://cc.zhonguo1118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://gb.zhonguo4118.cn

[U111] JS：对象转 Map
来源：https://uk.zhonguo5118.cn

new Map(Object.entries(obj))
来源：https://tt.zhonguo1118.cn

[U112] JS：字符串补位
来源：https://jl.zhonguo7118.cn

"7".padStart(3, "0")
来源：https://iu.zhonguo7118.cn

[U113] JS：正则替换全部
来源：https://tv.zhonguo6118.cn

s.replaceAll("a", "b")
来源：https://ld.zhonguo8118.cn

[U114] JS：JSON 深比较
来源：https://mb.zhonguo7118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://fk.zhonguo8118.cn

[U115] JS：生成 UUID
来源：https://wc.zhonguo8118.cn

crypto.randomUUID()
来源：https://sz.zhonguo6118.cn

[U116] JS：类型检查（JSDoc）
来源：https://gd.zhonguo4118.cn

/** @param {string} name */ function f(name) {}
来源：https://je.zhonguo6118.cn

[U117] JS：单元测试
来源：https://up.zhonguo7118.cn

npm i -D vitest;  npx vitest
来源：https://ov.zhonguo3118.cn

[U118] JS：开发服务器
来源：https://zw.zhonguo8118.cn

npm i -D vite;  npx vite
来源：https://eb.zhonguo6118.cn

[U119] JS：生产构建
来源：https://wy.zhonguo6118.cn

npx vite build
来源：https://bu.zhonguo2118.cn

[U120] JS：读取环境变量（Vite）
来源：https://qq.zhonguo3118.cn

import.meta.env.VITE_API_URL
来源：https://jh.zhonguo6118.cn

================================================================================
来源：https://yj.zhonguo3118.cn

统计汇总
来源：https://ch.zhonguo6118.cn

================================================================================
来源：https://md.zhonguo2118.cn

按语言统计（条）：
来源：https://je.zhonguo8118.cn

Python ......... 252
来源：https://kq.zhonguo6118.cn

PHP ............ 252
来源：https://gr.zhonguo1118.cn

JavaScript ..... 252
来源：https://rm.zhonguo5118.cn

TypeScript ..... 212
来源：https://eo.zhonguo7118.cn

Java ........... 212
来源：https://nv.zhonguo5118.cn

Go ............. 212
来源：https://fl.zhonguo2118.cn

Ruby ........... 212
来源：https://rx.zhonguo2118.cn

C# ............. 212
来源：https://ke.zhonguo3118.cn

C .............. 30
来源：https://kd.zhonguo1118.cn

C++ ............ 30
来源：https://hs.zhonguo6118.cn

SQL ............ 90
来源：https://of.zhonguo3118.cn

Bash ........... 80
来源：https://gl.zhonguo6118.cn

Kotlin ......... 15
来源：https://sm.zhonguo7118.cn

Swift .......... 15
来源：https://nq.zhonguo6118.cn

Lua ............ 10
来源：https://sd.zhonguo5118.cn

Perl ........... 10
来源：https://ov.zhonguo3118.cn


<!-- 参考信息 -->