代发 wailian999

[U09] Py：字典取最大值的键
来源：https://rm.zhonguo3118.cn

max(d, key=d.get)
来源：https://iv.zhonguo6118.cn

[U10] Py：按值排序字典
来源：https://ii.zhonguo7118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://qf.zhonguo3118.cn

[U11] Py：生成器表达式
来源：https://mx.zhonguo2118.cn

(x * 2 for x in arr)
来源：https://uj.zhonguo7118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://iq.zhonguo7118.cn

Counter(arr).most_common(3)
来源：https://vf.zhonguo8118.cn

[U13] Py：固定长度队列
来源：https://vh.zhonguo3118.cn

deque(maxlen=10)
来源：https://sz.zhonguo3118.cn

[U14] Py：分组收集到列表
来源：https://me.zhonguo4118.cn

defaultdict(list)
来源：https://ka.zhonguo5118.cn

[U15] Py：高精度计时
来源：https://un.zhonguo5118.cn

t = time.perf_counter()
来源：https://cu.zhonguo1118.cn

[U16] Py：命令行参数解析
来源：https://sz.zhonguo2118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://ob.zhonguo4118.cn

[U17] Py：初始化日志
来源：https://yj.zhonguo5118.cn

logging.basicConfig(level=logging.INFO)
来源：https://rj.zhonguo5118.cn

[U18] Py：预编译正则
来源：https://oz.zhonguo7118.cn

pat = re.compile(r"\d+")
来源：https://va.zhonguo2118.cn

[U19] Py：正则替换带回调
来源：https://ka.zhonguo5118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://iz.zhonguo8118.cn

[U20] Py：缓存函数结果
来源：https://rp.zhonguo2118.cn

@functools.lru_cache(maxsize=None)
来源：https://xi.zhonguo3118.cn

[U21] Py：自定义上下文管理器
来源：https://pm.zhonguo6118.cn

@contextlib.contextmanager
来源：https://ub.zhonguo3118.cn

[U22] Py：矩阵转置
来源：https://ms.zhonguo2118.cn

list(zip(*m))
来源：https://dr.zhonguo1118.cn

[U23] Py：分块读取大文件
来源：https://bw.zhonguo7118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://ii.zhonguo5118.cn

[U24] Py：路径操作
来源：https://nl.zhonguo3118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://qy.zhonguo8118.cn

[U25] Py：CSV 按字典读
来源：https://qa.zhonguo7118.cn

csv.DictReader(f)
来源：https://pb.zhonguo7118.cn

[U26] Py：并发下载
来源：https://qu.zhonguo7118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://dz.zhonguo2118.cn

[U27] Py：异步 HTTP
来源：https://le.zhonguo7118.cn

aiohttp.ClientSession() 配合 async with
来源：https://zp.zhonguo3118.cn

[U28] Py：类型别名
来源：https://ff.zhonguo7118.cn

UserId = int
来源：https://bc.zhonguo4118.cn

[U29] Py：属性校验
来源：https://vi.zhonguo3118.cn

@property 与 @x.setter 配合
来源：https://nm.zhonguo1118.cn

[U30] Py：数据类
来源：https://iv.zhonguo1118.cn

@dataclass(slots=True)
来源：https://uy.zhonguo8118.cn

[U31] Py：单测
来源：https://xl.zhonguo7118.cn

python -m pytest -q
来源：https://gz.zhonguo2118.cn

[U32] Py：代码格式化
来源：https://nt.zhonguo7118.cn

ruff format . && ruff check --fix .
来源：https://ba.zhonguo1118.cn

[U33] Py：打包发布
来源：https://ew.zhonguo7118.cn

python -m build  （依赖 pyproject.toml）
来源：https://tx.zhonguo8118.cn

[U34] Py：判断编码
来源：https://je.zhonguo7118.cn

chardet.detect(raw)
来源：https://tm.zhonguo4118.cn

[U35] Py：发送邮件
来源：https://iz.zhonguo2118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://ck.zhonguo3118.cn

[U36] Py：定时任务
来源：https://jc.zhonguo6118.cn

schedule.every(10).minutes.do(job)
来源：https://ne.zhonguo3118.cn

[U37] Py：读写 Excel
来源：https://zq.zhonguo7118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://nb.zhonguo8118.cn

[U38] Py：获取脚本所在目录
来源：https://wg.zhonguo4118.cn

Path(__file__).resolve().parent
来源：https://br.zhonguo7118.cn

[U39] Py：判断是否在交互环境
来源：https://ox.zhonguo3118.cn

sys.stdout.isatty()
来源：https://zn.zhonguo2118.cn

[U40] Py：打印到标准错误
来源：https://lf.zhonguo8118.cn

print("err", file=sys.stderr)
来源：https://ge.zhonguo8118.cn

[U41] PHP：初始化 Composer 项目
来源：https://kc.zhonguo1118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://rp.zhonguo6118.cn

[U42] PHP：PSR-4 自动加载
来源：https://es.zhonguo3118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://wi.zhonguo6118.cn

[U43] PHP：声明命名空间
来源：https://dg.zhonguo3118.cn

namespace App\Http;
来源：https://uw.zhonguo8118.cn

[U44] PHP：开启严格类型
来源：https://ef.zhonguo1118.cn

declare(strict_types=1);
来源：https://km.zhonguo6118.cn

[U45] PHP：类型声明与返回类型
来源：https://bx.zhonguo4118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://ov.zhonguo1118.cn

[U46] PHP：可空类型
来源：https://ul.zhonguo3118.cn

?string $name = null
来源：https://uf.zhonguo2118.cn

[U47] PHP：联合类型
来源：https://yq.zhonguo6118.cn

int|string $id
来源：https://gi.zhonguo1118.cn

[U48] PHP：纯枚举
来源：https://sn.zhonguo8118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://ef.zhonguo3118.cn

[U49] PHP：只读属性
来源：https://zs.zhonguo5118.cn

public readonly string $name
来源：https://nb.zhonguo2118.cn

[U50] PHP：构造器属性提升
来源：https://pp.zhonguo6118.cn

public function __construct(private int $id) {}
来源：https://vj.zhonguo8118.cn

[U51] PHP：数组解构
来源：https://zo.zhonguo7118.cn

[$a, $b] = $arr;
来源：https://yd.zhonguo4118.cn

[U52] PHP：箭头函数
来源：https://my.zhonguo3118.cn

$double = fn($x) => $x * 2;
来源：https://sj.zhonguo5118.cn

[U53] PHP：空合并运算符
来源：https://fy.zhonguo5118.cn

$v = $a ?? $b ?? "default";
来源：https://kt.zhonguo7118.cn

[U54] PHP：空安全调用
来源：https://nd.zhonguo6118.cn

$obj?->method()
来源：https://oo.zhonguo5118.cn

[U55] PHP：match 表达式
来源：https://fh.zhonguo2118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://md.zhonguo3118.cn

[U56] PHP：命名参数
来源：https://uf.zhonguo7118.cn

f(a: 1, b: 2)
来源：https://kr.zhonguo7118.cn

[U57] PHP：字符串插值
来源：https://bl.zhonguo5118.cn

"值: {$a}"
来源：https://is.zhonguo4118.cn

[U58] PHP：数组三件套
来源：https://ue.zhonguo3118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://dp.zhonguo8118.cn

[U59] PHP：自定义排序
来源：https://jg.zhonguo1118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://vi.zhonguo8118.cn

[U60] PHP：JSON 编解码
来源：https://ee.zhonguo7118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://jp.zhonguo8118.cn

[U61] PHP：正则
来源：https://wl.zhonguo7118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://iu.zhonguo6118.cn

[U62] PHP：日期对象
来源：https://ow.zhonguo7118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://lq.zhonguo3118.cn

[U63] PHP：文件读写
来源：https://ou.zhonguo2118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://uf.zhonguo6118.cn

[U64] PHP：目录遍历
来源：https://xa.zhonguo1118.cn

glob("dir/*.php");  scandir("dir");
来源：https://qw.zhonguo6118.cn

[U65] PHP：会话
来源：https://zd.zhonguo1118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://yq.zhonguo5118.cn

[U66] PHP：设置 Cookie
来源：https://jg.zhonguo4118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://gv.zhonguo7118.cn

[U67] PHP：处理文件上传
来源：https://wa.zhonguo7118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://sg.zhonguo7118.cn

[U68] PHP：PDO 连接
来源：https://es.zhonguo5118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://jh.zhonguo6118.cn

[U69] PHP：PDO 预处理
来源：https://da.zhonguo2118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://cu.zhonguo4118.cn

[U70] PHP：PDO 事务
来源：https://dp.zhonguo2118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://mn.zhonguo3118.cn

[U71] PHP：抛出异常
来源：https://jq.zhonguo2118.cn

throw new RuntimeException("失败", 500);
来源：https://rd.zhonguo8118.cn

[U72] PHP：写错误日志
来源：https://ft.zhonguo6118.cn

error_log("失败: " . $e->getMessage());
来源：https://yq.zhonguo4118.cn

[U73] PHP：读取 ini 配置
来源：https://yi.zhonguo3118.cn

parse_ini_file("config.ini", true)
来源：https://zo.zhonguo4118.cn

[U74] PHP：读取环境变量
来源：https://wu.zhonguo8118.cn

getenv("APP_ENV") ?: "production"
来源：https://xq.zhonguo1118.cn

[U75] PHP：依赖注入
来源：https://bb.zhonguo5118.cn

composer require psr/container
来源：https://rt.zhonguo7118.cn

[U76] PHP：简单路由
来源：https://tp.zhonguo6118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://ws.zhonguo4118.cn

[U77] PHP：模板渲染
来源：https://ip.zhonguo6118.cn

composer require twig/twig
来源：https://ba.zhonguo3118.cn

[U78] PHP：单元测试
来源：https://wn.zhonguo1118.cn

composer require --dev phpunit/phpunit
来源：https://zh.zhonguo3118.cn

[U79] PHP：静态分析
来源：https://mf.zhonguo4118.cn

composer require --dev phpstan/phpstan
来源：https://lf.zhonguo5118.cn

[U80] PHP：代码规范修复
来源：https://mq.zhonguo6118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://rd.zhonguo4118.cn

[U81] JS：初始化项目
来源：https://nu.zhonguo8118.cn

npm init -y;  npm i express
来源：https://ix.zhonguo4118.cn

[U82] JS：package.json 脚本
来源：https://jv.zhonguo7118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://ki.zhonguo2118.cn

[U83] JS：ES Module 导入导出
来源：https://wa.zhonguo4118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://gr.zhonguo4118.cn

[U84] JS：CommonJS 写法
来源：https://yd.zhonguo8118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://ji.zhonguo3118.cn

[U85] JS：可选链
来源：https://br.zhonguo4118.cn

a?.b?.c
来源：https://fn.zhonguo8118.cn

[U86] JS：空值合并
来源：https://rr.zhonguo8118.cn

a ?? b
来源：https://ma.zhonguo7118.cn

[U87] JS：解构默认值
来源：https://ev.zhonguo3118.cn

const { a = 1, b = 2 } = obj;
来源：https://dk.zhonguo2118.cn

[U88] JS：对象展开合并
来源：https://oy.zhonguo3118.cn

{ ...a, ...b }
来源：https://jp.zhonguo2118.cn

[U89] JS：数组去重
来源：https://ta.zhonguo7118.cn

[...new Set(arr)]
来源：https://ke.zhonguo5118.cn

[U90] JS：数字数组排序
来源：https://uo.zhonguo6118.cn

[...arr].sort((a, b) => a - b)
来源：https://ci.zhonguo5118.cn

[U91] JS：对象键值遍历
来源：https://pj.zhonguo1118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://xx.zhonguo7118.cn

[U92] JS：深拷贝
来源：https://sl.zhonguo6118.cn

structuredClone(obj)
来源：https://sw.zhonguo6118.cn

[U93] JS：模板字符串
来源：https://mo.zhonguo3118.cn

`共 ${n} 条`
来源：https://sw.zhonguo1118.cn

[U94] JS：箭头函数
来源：https://he.zhonguo7118.cn

const double = x => x * 2;
来源：https://zj.zhonguo3118.cn

[U95] JS：Promise 包装
来源：https://zw.zhonguo3118.cn

new Promise((resolve, reject) => {})
来源：https://kb.zhonguo5118.cn

[U96] JS：async/await 与异常
来源：https://fo.zhonguo1118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://xx.zhonguo1118.cn

[U97] JS：并发请求
来源：https://tc.zhonguo7118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://bl.zhonguo7118.cn

[U98] JS：fetch 带 JSON
来源：https://jv.zhonguo4118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://ly.zhonguo5118.cn

[U99] JS：事件监听
来源：https://is.zhonguo6118.cn

el.addEventListener("click", e => {})
来源：https://mv.zhonguo4118.cn

[U100] JS：DOM 查询
来源：https://uu.zhonguo5118.cn

document.querySelector(".item")
来源：https://dj.zhonguo1118.cn

[U101] JS：classList 操作
来源：https://zz.zhonguo7118.cn

el.classList.toggle("active")
来源：https://sa.zhonguo2118.cn

[U102] JS：本地存储
来源：https://zs.zhonguo4118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://yt.zhonguo8118.cn

[U103] JS：定时器
来源：https://lm.zhonguo4118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://wq.zhonguo4118.cn

[U104] JS：防抖
来源：https://ju.zhonguo2118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://qs.zhonguo7118.cn

[U105] JS：节流
来源：https://ot.zhonguo5118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://iy.zhonguo5118.cn

[U106] JS：日期格式化
来源：https://se.zhonguo7118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://yx.zhonguo8118.cn

[U107] JS：数字千分位
来源：https://zf.zhonguo2118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://zk.zhonguo4118.cn

[U108] JS：随机整数
来源：https://yi.zhonguo6118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://bm.zhonguo8118.cn

[U109] JS：数组分组
来源：https://iy.zhonguo3118.cn

Object.groupBy(arr, x => x.type)
来源：https://zg.zhonguo1118.cn

[U110] JS：数组分块
来源：https://jy.zhonguo2118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://vp.zhonguo1118.cn

[U111] JS：对象转 Map
来源：https://ce.zhonguo7118.cn

new Map(Object.entries(obj))
来源：https://js.zhonguo6118.cn

[U112] JS：字符串补位
来源：https://yq.zhonguo4118.cn

"7".padStart(3, "0")
来源：https://ne.zhonguo2118.cn

[U113] JS：正则替换全部
来源：https://ic.zhonguo3118.cn

s.replaceAll("a", "b")
来源：https://oe.zhonguo2118.cn

[U114] JS：JSON 深比较
来源：https://br.zhonguo3118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://hs.zhonguo8118.cn

[U115] JS：生成 UUID
来源：https://bl.zhonguo5118.cn

crypto.randomUUID()
来源：https://eg.zhonguo6118.cn

[U116] JS：类型检查（JSDoc）
来源：https://gt.zhonguo5118.cn

/** @param {string} name */ function f(name) {}
来源：https://bc.zhonguo3118.cn

[U117] JS：单元测试
来源：https://sz.zhonguo8118.cn

npm i -D vitest;  npx vitest
来源：https://io.zhonguo7118.cn

[U118] JS：开发服务器
来源：https://hl.zhonguo4118.cn

npm i -D vite;  npx vite
来源：https://td.zhonguo8118.cn

[U119] JS：生产构建
来源：https://ir.zhonguo1118.cn

npx vite build
来源：https://uz.zhonguo2118.cn

[U120] JS：读取环境变量（Vite）
来源：https://mx.zhonguo3118.cn

import.meta.env.VITE_API_URL
来源：https://ru.zhonguo3118.cn

================================================================================
来源：https://pk.zhonguo8118.cn

统计汇总
来源：https://vy.zhonguo5118.cn

================================================================================
来源：https://rm.zhonguo7118.cn

按语言统计（条）：
来源：https://kc.zhonguo2118.cn

Python ......... 252
来源：https://yw.zhonguo5118.cn

PHP ............ 252
来源：https://af.zhonguo3118.cn

JavaScript ..... 252
来源：https://wl.zhonguo3118.cn

TypeScript ..... 212
来源：https://tu.zhonguo3118.cn

Java ........... 212
来源：https://nq.zhonguo6118.cn

Go ............. 212
来源：https://wf.zhonguo8118.cn

Ruby ........... 212
来源：https://qk.zhonguo1118.cn

C# ............. 212
来源：https://ux.zhonguo5118.cn

C .............. 30
来源：https://hj.zhonguo8118.cn

C++ ............ 30
来源：https://fz.zhonguo6118.cn

SQL ............ 90
来源：https://fx.zhonguo7118.cn

Bash ........... 80
来源：https://gb.zhonguo1118.cn

Kotlin ......... 15
来源：https://fo.zhonguo5118.cn

Swift .......... 15
来源：https://bv.zhonguo4118.cn

Lua ............ 10
来源：https://dt.zhonguo2118.cn

Perl ........... 10
来源：https://nb.zhonguo8118.cn

Scala .......... 10
来源：https://kf.zhonguo3118.cn

------------------------------------
来源：https://en.zhonguo1118.cn

合计 ........... 2106 条
来源：https://og.zhonguo1118.cn

按章节统计：
来源：https://hg.zhonguo8118.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：https://qy.zhonguo4118.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：https://ru.zhonguo4118.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：https://dh.zhonguo6118.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：https://wj.zhonguo5118.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：https://sw.zhonguo7118.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：https://dv.zhonguo1118.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：https://jp.zhonguo5118.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：https://jl.zhonguo3118.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：https://hs.zhonguo8118.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：https://qq.zhonguo8118.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：https://gh.zhonguo1118.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：https://xf.zhonguo4118.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：https://jg.zhonguo3118.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：https://xs.zhonguo8118.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：https://kr.zhonguo6118.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：https://ss.zhonguo5118.cn

Q SQL 专题                              90
来源：https://ct.zhonguo2118.cn

R Bash 专题                             80
来源：https://oi.zhonguo4118.cn

S C / C++ 专题                          60
来源：https://op.zhonguo4118.cn

T 其他语言补充                          60
来源：https://mz.zhonguo8118.cn

U 高频实用片段                         120
来源：https://px.zhonguo1118.cn

------------------------------------
来源：https://lx.zhonguo4118.cn

合计                                  2106 条
来源：https://ij.zhonguo8118.cn

--------------------------------------------------------------------------------
来源：https://rj.zhonguo6118.cn

使用提醒
来源：https://xj.zhonguo7118.cn

--------------------------------------------------------------------------------
来源：https://nu.zhonguo1118.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：https://te.zhonguo8118.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：https://zu.zhonguo3118.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：https://zp.zhonguo7118.cn

在旧版本上使用前请先确认语法支持情况。
来源：https://gy.zhonguo4118.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：https://nw.zhonguo6118.cn

—— 文件结束 ——
来源：https://gl.zhonguo7118.cn

================================================================================
来源：https://im.zhonguo4118.cn

程序语言常见例子速查手册（2024 版）
来源：https://zb.zhonguo8118.cn

Common Programming Examples Cheat Book
来源：https://xx.zhonguo6118.cn

================================================================================
来源：https://ft.zhonguo1118.cn

【收录内容】
来源：https://ge.zhonguo6118.cn

覆盖 12 种语言 / 语法与常见 API：
来源：https://sl.zhonguo6118.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：https://en.zhonguo6118.cn

SQL · Bash · C · C++
来源：https://ji.zhonguo3118.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：https://uy.zhonguo3118.cn

【使用说明】
来源：https://kb.zhonguo1118.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：https://ni.zhonguo4118.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：https://wo.zhonguo1118.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：https://hm.zhonguo3118.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：https://bp.zhonguo1118.cn

Bash:  Shell         C:     C             C++:   C++
来源：https://ci.zhonguo7118.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：https://et.zhonguo2118.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：https://qe.zhonguo5118.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：https://bs.zhonguo7118.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：https://mw.zhonguo1118.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：https://di.zhonguo8118.cn


<!-- 参考信息 -->