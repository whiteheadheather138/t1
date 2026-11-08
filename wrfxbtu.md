代发 wailian999

val a = 1;  var b = 2
来源：https://sa.zhonguo7118.cn

[T53] Scala：字符串插值
来源：https://zh.zhonguo3118.cn

s"值: $b"
来源：https://jx.zhonguo4118.cn

[T54] Scala：集合映射
来源：https://uu.zhonguo4118.cn

List(1, 2, 3).map(_ * 2)
来源：https://kk.zhonguo1118.cn

[T55] Scala：集合过滤
来源：https://gk.zhonguo8118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://uv.zhonguo5118.cn

[T56] Scala：样例类
来源：https://um.zhonguo4118.cn

case class User(name: String, age: Int)
来源：https://hb.zhonguo8118.cn

[T57] Scala：模式匹配
来源：https://xh.zhonguo6118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://sj.zhonguo1118.cn

[T58] Scala：函数定义
来源：https://dl.zhonguo5118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://dx.zhonguo5118.cn

[T59] Scala：循环
来源：https://xg.zhonguo3118.cn

for (i <- 1 to 10) println(i)
来源：https://iy.zhonguo5118.cn

[T60] Scala：折叠
来源：https://po.zhonguo5118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://rj.zhonguo4118.cn

================================================================================
来源：https://rc.zhonguo2118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://it.zhonguo1118.cn

================================================================================
来源：https://gh.zhonguo7118.cn

[U01] Py：创建虚拟环境
来源：https://fz.zhonguo1118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://ox.zhonguo3118.cn

[U02] Py：导出 / 安装依赖
来源：https://yn.zhonguo8118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://bw.zhonguo8118.cn

[U03] Py：加载 .env 配置
来源：https://zc.zhonguo2118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://wt.zhonguo4118.cn

[U04] Py：变量调试打印
来源：https://jg.zhonguo3118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://fv.zhonguo7118.cn

[U05] Py：列表去重且保序
来源：https://kn.zhonguo2118.cn

list(dict.fromkeys(arr))
来源：https://fz.zhonguo5118.cn

[U06] Py：合并两个字典
来源：https://ea.zhonguo7118.cn

{**a, **b}
来源：https://xu.zhonguo2118.cn

[U07] Py：反转字典键值
来源：https://zo.zhonguo4118.cn

{v: k for k, v in d.items()}
来源：https://ip.zhonguo6118.cn

[U08] Py：展平二维列表
来源：https://zc.zhonguo8118.cn

[y for x in nested for y in x]
来源：https://sv.zhonguo6118.cn

[U09] Py：字典取最大值的键
来源：https://uh.zhonguo2118.cn

max(d, key=d.get)
来源：https://xp.zhonguo7118.cn

[U10] Py：按值排序字典
来源：https://ds.zhonguo5118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://mg.zhonguo1118.cn

[U11] Py：生成器表达式
来源：https://tj.zhonguo8118.cn

(x * 2 for x in arr)
来源：https://bc.zhonguo7118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://fc.zhonguo3118.cn

Counter(arr).most_common(3)
来源：https://xp.zhonguo8118.cn

[U13] Py：固定长度队列
来源：https://nx.zhonguo5118.cn

deque(maxlen=10)
来源：https://oa.zhonguo6118.cn

[U14] Py：分组收集到列表
来源：https://vi.zhonguo8118.cn

defaultdict(list)
来源：https://eu.zhonguo5118.cn

[U15] Py：高精度计时
来源：https://ff.zhonguo4118.cn

t = time.perf_counter()
来源：https://cl.zhonguo3118.cn

[U16] Py：命令行参数解析
来源：https://fi.zhonguo7118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://qr.zhonguo3118.cn

[U17] Py：初始化日志
来源：https://dl.zhonguo8118.cn

logging.basicConfig(level=logging.INFO)
来源：https://yx.zhonguo6118.cn

[U18] Py：预编译正则
来源：https://ld.zhonguo8118.cn

pat = re.compile(r"\d+")
来源：https://nq.zhonguo4118.cn

[U19] Py：正则替换带回调
来源：https://qw.zhonguo8118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://rx.zhonguo5118.cn

[U20] Py：缓存函数结果
来源：https://ju.zhonguo2118.cn

@functools.lru_cache(maxsize=None)
来源：https://ix.zhonguo2118.cn

[U21] Py：自定义上下文管理器
来源：https://xd.zhonguo3118.cn

@contextlib.contextmanager
来源：https://hq.zhonguo5118.cn

[U22] Py：矩阵转置
来源：https://cq.zhonguo8118.cn

list(zip(*m))
来源：https://qm.zhonguo5118.cn

[U23] Py：分块读取大文件
来源：https://dz.zhonguo3118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://hi.zhonguo7118.cn

[U24] Py：路径操作
来源：https://bt.zhonguo6118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://gk.zhonguo3118.cn

[U25] Py：CSV 按字典读
来源：https://eu.zhonguo3118.cn

csv.DictReader(f)
来源：https://vd.zhonguo8118.cn

[U26] Py：并发下载
来源：https://gz.zhonguo7118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://ae.zhonguo5118.cn

[U27] Py：异步 HTTP
来源：https://wm.zhonguo2118.cn

aiohttp.ClientSession() 配合 async with
来源：https://xk.zhonguo7118.cn

[U28] Py：类型别名
来源：https://io.zhonguo3118.cn

UserId = int
来源：https://od.zhonguo5118.cn

[U29] Py：属性校验
来源：https://pg.zhonguo5118.cn

@property 与 @x.setter 配合
来源：https://rg.zhonguo4118.cn

[U30] Py：数据类
来源：https://al.zhonguo3118.cn

@dataclass(slots=True)
来源：https://rw.zhonguo5118.cn

[U31] Py：单测
来源：https://hk.zhonguo3118.cn

python -m pytest -q
来源：https://mt.zhonguo8118.cn

[U32] Py：代码格式化
来源：https://vj.zhonguo8118.cn

ruff format . && ruff check --fix .
来源：https://qf.zhonguo2118.cn

[U33] Py：打包发布
来源：https://wi.zhonguo6118.cn

python -m build  （依赖 pyproject.toml）
来源：https://cn.zhonguo3118.cn

[U34] Py：判断编码
来源：https://et.zhonguo2118.cn

chardet.detect(raw)
来源：https://hr.zhonguo5118.cn

[U35] Py：发送邮件
来源：https://zu.zhonguo4118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://ur.zhonguo5118.cn

[U36] Py：定时任务
来源：https://fy.zhonguo5118.cn

schedule.every(10).minutes.do(job)
来源：https://hg.zhonguo4118.cn

[U37] Py：读写 Excel
来源：https://ez.zhonguo2118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://ub.zhonguo2118.cn

[U38] Py：获取脚本所在目录
来源：https://wl.zhonguo1118.cn

Path(__file__).resolve().parent
来源：https://xw.zhonguo6118.cn

[U39] Py：判断是否在交互环境
来源：https://sa.zhonguo7118.cn

sys.stdout.isatty()
来源：https://om.zhonguo3118.cn

[U40] Py：打印到标准错误
来源：https://bf.zhonguo4118.cn

print("err", file=sys.stderr)
来源：https://bt.zhonguo3118.cn

[U41] PHP：初始化 Composer 项目
来源：https://uo.zhonguo1118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://xp.zhonguo6118.cn

[U42] PHP：PSR-4 自动加载
来源：https://ch.zhonguo6118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://ii.zhonguo7118.cn

[U43] PHP：声明命名空间
来源：https://oj.zhonguo1118.cn

namespace App\Http;
来源：https://ks.zhonguo4118.cn

[U44] PHP：开启严格类型
来源：https://nb.zhonguo2118.cn

declare(strict_types=1);
来源：https://aj.zhonguo4118.cn

[U45] PHP：类型声明与返回类型
来源：https://rn.zhonguo7118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://rc.zhonguo8118.cn

[U46] PHP：可空类型
来源：https://xn.zhonguo6118.cn

?string $name = null
来源：https://dq.zhonguo2118.cn

[U47] PHP：联合类型
来源：https://jk.zhonguo2118.cn

int|string $id
来源：https://ze.zhonguo7118.cn

[U48] PHP：纯枚举
来源：https://jo.zhonguo5118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://ws.zhonguo5118.cn

[U49] PHP：只读属性
来源：https://na.zhonguo7118.cn

public readonly string $name
来源：https://id.zhonguo1118.cn

[U50] PHP：构造器属性提升
来源：https://rz.zhonguo3118.cn

public function __construct(private int $id) {}
来源：https://nu.zhonguo7118.cn

[U51] PHP：数组解构
来源：https://fy.zhonguo4118.cn

[$a, $b] = $arr;
来源：https://fn.zhonguo6118.cn

[U52] PHP：箭头函数
来源：https://rw.zhonguo7118.cn

$double = fn($x) => $x * 2;
来源：https://sa.zhonguo4118.cn

[U53] PHP：空合并运算符
来源：https://ne.zhonguo7118.cn

$v = $a ?? $b ?? "default";
来源：https://iu.zhonguo3118.cn

[U54] PHP：空安全调用
来源：https://ru.zhonguo6118.cn

$obj?->method()
来源：https://ut.zhonguo6118.cn

[U55] PHP：match 表达式
来源：https://wq.zhonguo2118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://cm.zhonguo4118.cn

[U56] PHP：命名参数
来源：https://we.zhonguo3118.cn

f(a: 1, b: 2)
来源：https://zt.zhonguo3118.cn

[U57] PHP：字符串插值
来源：https://fh.zhonguo5118.cn

"值: {$a}"
来源：https://za.zhonguo1118.cn

[U58] PHP：数组三件套
来源：https://ob.zhonguo8118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://vt.zhonguo2118.cn

[U59] PHP：自定义排序
来源：https://uc.zhonguo3118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://ip.zhonguo5118.cn

[U60] PHP：JSON 编解码
来源：https://fe.zhonguo1118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://py.zhonguo5118.cn

[U61] PHP：正则
来源：https://ft.zhonguo3118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://dq.zhonguo3118.cn

[U62] PHP：日期对象
来源：https://ti.zhonguo5118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://cv.zhonguo6118.cn

[U63] PHP：文件读写
来源：https://va.zhonguo4118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://rj.zhonguo3118.cn

[U64] PHP：目录遍历
来源：https://ug.zhonguo8118.cn

glob("dir/*.php");  scandir("dir");
来源：https://wa.zhonguo5118.cn

[U65] PHP：会话
来源：https://pz.zhonguo6118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://gw.zhonguo6118.cn

[U66] PHP：设置 Cookie
来源：https://ah.zhonguo1118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://vx.zhonguo5118.cn

[U67] PHP：处理文件上传
来源：https://lf.zhonguo8118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://ss.zhonguo4118.cn

[U68] PHP：PDO 连接
来源：https://yk.zhonguo6118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://ma.zhonguo7118.cn

[U69] PHP：PDO 预处理
来源：https://cr.zhonguo8118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://lr.zhonguo5118.cn

[U70] PHP：PDO 事务
来源：https://rd.zhonguo2118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://uz.zhonguo2118.cn

[U71] PHP：抛出异常
来源：https://nb.zhonguo2118.cn

throw new RuntimeException("失败", 500);
来源：https://kr.zhonguo6118.cn

[U72] PHP：写错误日志
来源：https://gy.zhonguo5118.cn

error_log("失败: " . $e->getMessage());
来源：https://ey.zhonguo8118.cn

[U73] PHP：读取 ini 配置
来源：https://rf.zhonguo5118.cn

parse_ini_file("config.ini", true)
来源：https://iw.zhonguo8118.cn

[U74] PHP：读取环境变量
来源：https://eo.zhonguo6118.cn

getenv("APP_ENV") ?: "production"
来源：https://nj.zhonguo1118.cn

[U75] PHP：依赖注入
来源：https://uu.zhonguo7118.cn

composer require psr/container
来源：https://nl.zhonguo6118.cn

[U76] PHP：简单路由
来源：https://ov.zhonguo2118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://nv.zhonguo7118.cn

[U77] PHP：模板渲染
来源：https://dz.zhonguo7118.cn

composer require twig/twig
来源：https://st.zhonguo7118.cn

[U78] PHP：单元测试
来源：https://ow.zhonguo1118.cn

composer require --dev phpunit/phpunit
来源：https://op.zhonguo2118.cn

[U79] PHP：静态分析
来源：https://vi.zhonguo2118.cn

composer require --dev phpstan/phpstan
来源：https://mz.zhonguo6118.cn

[U80] PHP：代码规范修复
来源：https://xt.zhonguo5118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://th.zhonguo7118.cn

[U81] JS：初始化项目
来源：https://ou.zhonguo8118.cn

npm init -y;  npm i express
来源：https://wg.zhonguo1118.cn

[U82] JS：package.json 脚本
来源：https://mj.zhonguo4118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://zo.zhonguo2118.cn

[U83] JS：ES Module 导入导出
来源：https://xh.zhonguo5118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://vo.zhonguo6118.cn

[U84] JS：CommonJS 写法
来源：https://ub.zhonguo5118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://dr.zhonguo8118.cn

[U85] JS：可选链
来源：https://lk.zhonguo2118.cn

a?.b?.c
来源：https://mb.zhonguo2118.cn

[U86] JS：空值合并
来源：https://uv.zhonguo4118.cn

a ?? b
来源：https://zr.zhonguo5118.cn

[U87] JS：解构默认值
来源：https://rx.zhonguo1118.cn

const { a = 1, b = 2 } = obj;
来源：https://rc.zhonguo1118.cn

[U88] JS：对象展开合并
来源：https://cc.zhonguo2118.cn

{ ...a, ...b }
来源：https://jc.zhonguo2118.cn

[U89] JS：数组去重
来源：https://lz.zhonguo2118.cn

[...new Set(arr)]
来源：https://wu.zhonguo6118.cn

[U90] JS：数字数组排序
来源：https://ru.zhonguo4118.cn

[...arr].sort((a, b) => a - b)
来源：https://ha.zhonguo6118.cn

[U91] JS：对象键值遍历
来源：https://in.zhonguo7118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://hw.zhonguo4118.cn

[U92] JS：深拷贝
来源：https://tw.zhonguo8118.cn

structuredClone(obj)
来源：https://wi.zhonguo3118.cn

[U93] JS：模板字符串
来源：https://nq.zhonguo8118.cn

`共 ${n} 条`
来源：https://jz.zhonguo4118.cn

[U94] JS：箭头函数
来源：https://nx.zhonguo4118.cn

const double = x => x * 2;
来源：https://kg.zhonguo2118.cn

[U95] JS：Promise 包装
来源：https://tm.zhonguo6118.cn

new Promise((resolve, reject) => {})
来源：https://xy.zhonguo5118.cn

[U96] JS：async/await 与异常
来源：https://nh.zhonguo1118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://ia.zhonguo5118.cn

[U97] JS：并发请求
来源：https://zh.zhonguo8118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://wa.zhonguo8118.cn

[U98] JS：fetch 带 JSON
来源：https://oj.zhonguo8118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://to.zhonguo1118.cn

[U99] JS：事件监听
来源：https://yw.zhonguo6118.cn

el.addEventListener("click", e => {})
来源：https://km.zhonguo6118.cn

[U100] JS：DOM 查询
来源：https://qv.zhonguo1118.cn

document.querySelector(".item")
来源：https://jc.zhonguo3118.cn

[U101] JS：classList 操作
来源：https://rv.zhonguo6118.cn

el.classList.toggle("active")
来源：https://ze.zhonguo6118.cn

[U102] JS：本地存储
来源：https://kh.zhonguo4118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://oj.zhonguo1118.cn

[U103] JS：定时器
来源：https://wr.zhonguo5118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://vj.zhonguo8118.cn

[U104] JS：防抖
来源：https://fa.zhonguo1118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://nh.zhonguo5118.cn

[U105] JS：节流
来源：https://xn.zhonguo2118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://uu.zhonguo6118.cn

[U106] JS：日期格式化
来源：https://iw.zhonguo4118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://eo.zhonguo3118.cn

[U107] JS：数字千分位
来源：https://az.zhonguo1118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://ra.zhonguo7118.cn

[U108] JS：随机整数
来源：https://hg.zhonguo1118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://ce.zhonguo4118.cn

[U109] JS：数组分组
来源：https://hl.zhonguo2118.cn

Object.groupBy(arr, x => x.type)
来源：https://ip.zhonguo3118.cn

[U110] JS：数组分块
来源：https://gt.zhonguo2118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://ks.zhonguo6118.cn

[U111] JS：对象转 Map
来源：https://ro.zhonguo4118.cn

new Map(Object.entries(obj))
来源：https://ct.zhonguo5118.cn

[U112] JS：字符串补位
来源：https://fb.zhonguo6118.cn

"7".padStart(3, "0")
来源：https://fr.zhonguo1118.cn

[U113] JS：正则替换全部
来源：https://mc.zhonguo8118.cn

s.replaceAll("a", "b")
来源：https://yl.zhonguo5118.cn

[U114] JS：JSON 深比较
来源：https://su.zhonguo7118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://nk.zhonguo4118.cn

[U115] JS：生成 UUID
来源：https://df.zhonguo5118.cn

crypto.randomUUID()
来源：https://wn.zhonguo3118.cn

[U116] JS：类型检查（JSDoc）
来源：https://np.zhonguo3118.cn

/** @param {string} name */ function f(name) {}
来源：https://ds.zhonguo4118.cn

[U117] JS：单元测试
来源：https://dk.zhonguo4118.cn

npm i -D vitest;  npx vitest
来源：https://mt.zhonguo3118.cn

[U118] JS：开发服务器
来源：https://so.zhonguo8118.cn

npm i -D vite;  npx vite
来源：https://ve.zhonguo5118.cn

[U119] JS：生产构建
来源：https://ew.zhonguo6118.cn

npx vite build
来源：https://mc.zhonguo8118.cn

[U120] JS：读取环境变量（Vite）
来源：https://hr.zhonguo1118.cn

import.meta.env.VITE_API_URL
来源：https://xn.zhonguo2118.cn

================================================================================
来源：https://pq.zhonguo6118.cn

统计汇总
来源：https://nl.zhonguo2118.cn

================================================================================
来源：https://hj.zhonguo8118.cn

按语言统计（条）：
来源：https://iz.zhonguo5118.cn

Python ......... 252
来源：https://if.zhonguo3118.cn

PHP ............ 252
来源：https://yu.zhonguo2118.cn

JavaScript ..... 252
来源：https://xd.zhonguo3118.cn

TypeScript ..... 212
来源：https://op.zhonguo4118.cn

Java ........... 212
来源：https://uw.zhonguo8118.cn

Go ............. 212
来源：https://wd.zhonguo6118.cn

Ruby ........... 212
来源：https://wn.zhonguo1118.cn

C# ............. 212
来源：https://mu.zhonguo8118.cn

C .............. 30
来源：https://jt.zhonguo8118.cn

C++ ............ 30
来源：https://ww.zhonguo2118.cn

SQL ............ 90
来源：https://fo.zhonguo1118.cn

Bash ........... 80
来源：https://ug.zhonguo8118.cn

Kotlin ......... 15
来源：https://zp.zhonguo4118.cn

Swift .......... 15
来源：https://bt.zhonguo6118.cn

Lua ............ 10
来源：https://hq.zhonguo1118.cn

Perl ........... 10
来源：https://xe.zhonguo8118.cn

Scala .......... 10
来源：https://lo.zhonguo7118.cn

------------------------------------
来源：https://em.zhonguo4118.cn

合计 ........... 2106 条
来源：https://wx.zhonguo8118.cn

按章节统计：
来源：https://yg.zhonguo6118.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：https://wq.zhonguo3118.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：https://nb.zhonguo8118.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：https://tl.zhonguo7118.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：https://xg.zhonguo8118.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：https://bt.zhonguo4118.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：https://mp.zhonguo6118.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：https://yw.zhonguo2118.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：https://xk.zhonguo3118.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：https://lg.zhonguo5118.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：https://no.zhonguo7118.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：https://uc.zhonguo3118.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：https://yy.zhonguo6118.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：https://ej.zhonguo8118.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：https://iq.zhonguo3118.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：https://gt.zhonguo7118.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：https://ro.zhonguo5118.cn


<!-- 参考信息 -->