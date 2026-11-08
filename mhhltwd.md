代发 wailian999

[U11] Py：生成器表达式
来源：https://ob.zhonguo3118.cn

(x * 2 for x in arr)
来源：https://km.zhonguo4118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://wg.zhonguo7118.cn

Counter(arr).most_common(3)
来源：https://ec.zhonguo6118.cn

[U13] Py：固定长度队列
来源：https://my.zhonguo1118.cn

deque(maxlen=10)
来源：https://op.zhonguo3118.cn

[U14] Py：分组收集到列表
来源：https://ys.zhonguo1118.cn

defaultdict(list)
来源：https://ud.zhonguo7118.cn

[U15] Py：高精度计时
来源：https://mp.zhonguo7118.cn

t = time.perf_counter()
来源：https://qd.zhonguo4118.cn

[U16] Py：命令行参数解析
来源：https://zh.zhonguo2118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://ha.zhonguo8118.cn

[U17] Py：初始化日志
来源：https://oo.zhonguo2118.cn

logging.basicConfig(level=logging.INFO)
来源：https://cd.zhonguo2118.cn

[U18] Py：预编译正则
来源：https://gz.zhonguo6118.cn

pat = re.compile(r"\d+")
来源：https://ge.zhonguo8118.cn

[U19] Py：正则替换带回调
来源：https://vu.zhonguo6118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://dc.zhonguo6118.cn

[U20] Py：缓存函数结果
来源：https://mv.zhonguo3118.cn

@functools.lru_cache(maxsize=None)
来源：https://ab.zhonguo3118.cn

[U21] Py：自定义上下文管理器
来源：https://is.zhonguo1118.cn

@contextlib.contextmanager
来源：https://ae.zhonguo3118.cn

[U22] Py：矩阵转置
来源：https://fc.zhonguo5118.cn

list(zip(*m))
来源：https://rm.zhonguo5118.cn

[U23] Py：分块读取大文件
来源：https://tx.zhonguo7118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://ni.zhonguo5118.cn

[U24] Py：路径操作
来源：https://uu.zhonguo2118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://ob.zhonguo5118.cn

[U25] Py：CSV 按字典读
来源：https://to.zhonguo5118.cn

csv.DictReader(f)
来源：https://op.zhonguo4118.cn

[U26] Py：并发下载
来源：https://tk.zhonguo7118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://ss.zhonguo4118.cn

[U27] Py：异步 HTTP
来源：https://fw.zhonguo5118.cn

aiohttp.ClientSession() 配合 async with
来源：https://hp.zhonguo7118.cn

[U28] Py：类型别名
来源：https://bm.zhonguo7118.cn

UserId = int
来源：https://cz.zhonguo2118.cn

[U29] Py：属性校验
来源：https://gh.zhonguo5118.cn

@property 与 @x.setter 配合
来源：https://tr.zhonguo7118.cn

[U30] Py：数据类
来源：https://ho.zhonguo6118.cn

@dataclass(slots=True)
来源：https://th.zhonguo1118.cn

[U31] Py：单测
来源：https://vi.zhonguo4118.cn

python -m pytest -q
来源：https://pb.zhonguo1118.cn

[U32] Py：代码格式化
来源：https://ua.zhonguo8118.cn

ruff format . && ruff check --fix .
来源：https://aw.zhonguo3118.cn

[U33] Py：打包发布
来源：https://we.zhonguo2118.cn

python -m build  （依赖 pyproject.toml）
来源：https://cg.zhonguo7118.cn

[U34] Py：判断编码
来源：https://io.zhonguo2118.cn

chardet.detect(raw)
来源：https://hr.zhonguo8118.cn

[U35] Py：发送邮件
来源：https://aa.zhonguo2118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://zy.zhonguo6118.cn

[U36] Py：定时任务
来源：https://il.zhonguo3118.cn

schedule.every(10).minutes.do(job)
来源：https://ly.zhonguo2118.cn

[U37] Py：读写 Excel
来源：https://lj.zhonguo3118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://ll.zhonguo1118.cn

[U38] Py：获取脚本所在目录
来源：https://rm.zhonguo3118.cn

Path(__file__).resolve().parent
来源：https://yr.zhonguo3118.cn

[U39] Py：判断是否在交互环境
来源：https://dr.zhonguo8118.cn

sys.stdout.isatty()
来源：https://qp.zhonguo5118.cn

[U40] Py：打印到标准错误
来源：https://xo.zhonguo2118.cn

print("err", file=sys.stderr)
来源：https://zy.zhonguo7118.cn

[U41] PHP：初始化 Composer 项目
来源：https://xg.zhonguo1118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://ec.zhonguo6118.cn

[U42] PHP：PSR-4 自动加载
来源：https://ep.zhonguo2118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://zz.zhonguo6118.cn

[U43] PHP：声明命名空间
来源：https://rp.zhonguo3118.cn

namespace App\Http;
来源：https://jq.zhonguo4118.cn

[U44] PHP：开启严格类型
来源：https://uu.zhonguo4118.cn

declare(strict_types=1);
来源：https://wu.zhonguo8118.cn

[U45] PHP：类型声明与返回类型
来源：https://rq.zhonguo3118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://sf.zhonguo6118.cn

[U46] PHP：可空类型
来源：https://gn.zhonguo8118.cn

?string $name = null
来源：https://rw.zhonguo3118.cn

[U47] PHP：联合类型
来源：https://oy.zhonguo4118.cn

int|string $id
来源：https://xu.zhonguo2118.cn

[U48] PHP：纯枚举
来源：https://jt.zhonguo1118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://xq.zhonguo8118.cn

[U49] PHP：只读属性
来源：https://iy.zhonguo3118.cn

public readonly string $name
来源：https://ps.zhonguo4118.cn

[U50] PHP：构造器属性提升
来源：https://lr.zhonguo6118.cn

public function __construct(private int $id) {}
来源：https://vq.zhonguo6118.cn

[U51] PHP：数组解构
来源：https://nc.zhonguo1118.cn

[$a, $b] = $arr;
来源：https://ll.zhonguo1118.cn

[U52] PHP：箭头函数
来源：https://ur.zhonguo2118.cn

$double = fn($x) => $x * 2;
来源：https://kg.zhonguo6118.cn

[U53] PHP：空合并运算符
来源：https://sv.zhonguo1118.cn

$v = $a ?? $b ?? "default";
来源：https://vt.zhonguo8118.cn

[U54] PHP：空安全调用
来源：https://zz.zhonguo2118.cn

$obj?->method()
来源：https://gw.zhonguo1118.cn

[U55] PHP：match 表达式
来源：https://sh.zhonguo3118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://gx.zhonguo7118.cn

[U56] PHP：命名参数
来源：https://tk.zhonguo8118.cn

f(a: 1, b: 2)
来源：https://ep.zhonguo7118.cn

[U57] PHP：字符串插值
来源：https://wx.zhonguo3118.cn

"值: {$a}"
来源：https://rz.zhonguo8118.cn

[U58] PHP：数组三件套
来源：https://sg.zhonguo6118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://dh.zhonguo8118.cn

[U59] PHP：自定义排序
来源：https://lz.zhonguo5118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://ad.zhonguo5118.cn

[U60] PHP：JSON 编解码
来源：https://tv.zhonguo7118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://xx.zhonguo7118.cn

[U61] PHP：正则
来源：https://ap.zhonguo5118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://es.zhonguo2118.cn

[U62] PHP：日期对象
来源：https://pb.zhonguo8118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://bv.zhonguo3118.cn

[U63] PHP：文件读写
来源：https://qt.zhonguo5118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://ae.zhonguo7118.cn

[U64] PHP：目录遍历
来源：https://ea.zhonguo4118.cn

glob("dir/*.php");  scandir("dir");
来源：https://dh.zhonguo4118.cn

[U65] PHP：会话
来源：https://zf.zhonguo2118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://fl.zhonguo6118.cn

[U66] PHP：设置 Cookie
来源：https://oo.zhonguo6118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://iq.zhonguo1118.cn

[U67] PHP：处理文件上传
来源：https://nj.zhonguo4118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://fq.zhonguo6118.cn

[U68] PHP：PDO 连接
来源：https://ug.zhonguo3118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://to.zhonguo1118.cn

[U69] PHP：PDO 预处理
来源：https://zz.zhonguo8118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://kc.zhonguo3118.cn

[U70] PHP：PDO 事务
来源：https://bj.zhonguo7118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://xs.zhonguo1118.cn

[U71] PHP：抛出异常
来源：https://al.zhonguo4118.cn

throw new RuntimeException("失败", 500);
来源：https://yt.zhonguo8118.cn

[U72] PHP：写错误日志
来源：https://wh.zhonguo5118.cn

error_log("失败: " . $e->getMessage());
来源：https://rp.zhonguo1118.cn

[U73] PHP：读取 ini 配置
来源：https://fo.zhonguo8118.cn

parse_ini_file("config.ini", true)
来源：https://ok.zhonguo1118.cn

[U74] PHP：读取环境变量
来源：https://of.zhonguo7118.cn

getenv("APP_ENV") ?: "production"
来源：https://lg.zhonguo3118.cn

[U75] PHP：依赖注入
来源：https://cg.zhonguo7118.cn

composer require psr/container
来源：https://hc.zhonguo3118.cn

[U76] PHP：简单路由
来源：https://tg.zhonguo5118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://pe.zhonguo3118.cn

[U77] PHP：模板渲染
来源：https://gx.zhonguo4118.cn

composer require twig/twig
来源：https://kz.zhonguo2118.cn

[U78] PHP：单元测试
来源：https://qe.zhonguo8118.cn

composer require --dev phpunit/phpunit
来源：https://wn.zhonguo2118.cn

[U79] PHP：静态分析
来源：https://rp.zhonguo5118.cn

composer require --dev phpstan/phpstan
来源：https://uq.zhonguo4118.cn

[U80] PHP：代码规范修复
来源：https://os.zhonguo8118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://dp.zhonguo5118.cn

[U81] JS：初始化项目
来源：https://zr.zhonguo1118.cn

npm init -y;  npm i express
来源：https://dg.zhonguo3118.cn

[U82] JS：package.json 脚本
来源：https://ld.zhonguo7118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://bc.zhonguo8118.cn

[U83] JS：ES Module 导入导出
来源：https://fp.zhonguo3118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://zc.zhonguo1118.cn

[U84] JS：CommonJS 写法
来源：https://ig.zhonguo7118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://rl.zhonguo3118.cn

[U85] JS：可选链
来源：https://qe.zhonguo3118.cn

a?.b?.c
来源：https://ht.zhonguo6118.cn

[U86] JS：空值合并
来源：https://so.zhonguo5118.cn

a ?? b
来源：https://fc.zhonguo6118.cn

[U87] JS：解构默认值
来源：https://pf.zhonguo4118.cn

const { a = 1, b = 2 } = obj;
来源：https://oz.zhonguo3118.cn

[U88] JS：对象展开合并
来源：https://dx.zhonguo2118.cn

{ ...a, ...b }
来源：https://wq.zhonguo6118.cn

[U89] JS：数组去重
来源：https://ge.zhonguo2118.cn

[...new Set(arr)]
来源：https://ea.zhonguo2118.cn

[U90] JS：数字数组排序
来源：https://jo.zhonguo4118.cn

[...arr].sort((a, b) => a - b)
来源：https://zn.zhonguo6118.cn

[U91] JS：对象键值遍历
来源：https://gn.zhonguo8118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://pn.zhonguo8118.cn

[U92] JS：深拷贝
来源：https://pd.zhonguo6118.cn

structuredClone(obj)
来源：https://wu.zhonguo6118.cn

[U93] JS：模板字符串
来源：https://aj.zhonguo6118.cn

`共 ${n} 条`
来源：https://ml.zhonguo5118.cn

[U94] JS：箭头函数
来源：https://lf.zhonguo1118.cn

const double = x => x * 2;
来源：https://lr.zhonguo3118.cn

[U95] JS：Promise 包装
来源：https://xk.zhonguo8118.cn

new Promise((resolve, reject) => {})
来源：https://cb.zhonguo7118.cn

[U96] JS：async/await 与异常
来源：https://sg.zhonguo4118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://sk.zhonguo1118.cn

[U97] JS：并发请求
来源：https://qc.zhonguo3118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://ad.zhonguo6118.cn

[U98] JS：fetch 带 JSON
来源：https://kx.zhonguo5118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://uo.zhonguo8118.cn

[U99] JS：事件监听
来源：https://am.zhonguo7118.cn

el.addEventListener("click", e => {})
来源：https://jq.zhonguo8118.cn

[U100] JS：DOM 查询
来源：https://sa.zhonguo1118.cn

document.querySelector(".item")
来源：https://ef.zhonguo3118.cn

[U101] JS：classList 操作
来源：https://so.zhonguo3118.cn

el.classList.toggle("active")
来源：https://ze.zhonguo2118.cn

[U102] JS：本地存储
来源：https://ek.zhonguo3118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://dj.zhonguo7118.cn

[U103] JS：定时器
来源：https://gf.zhonguo3118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://pw.zhonguo6118.cn

[U104] JS：防抖
来源：https://ea.zhonguo8118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://ad.zhonguo7118.cn

[U105] JS：节流
来源：https://lt.zhonguo2118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://jt.zhonguo8118.cn

[U106] JS：日期格式化
来源：https://eh.zhonguo7118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://un.zhonguo6118.cn

[U107] JS：数字千分位
来源：https://zr.zhonguo7118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://vb.zhonguo4118.cn

[U108] JS：随机整数
来源：https://ly.zhonguo8118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://qp.zhonguo7118.cn

[U109] JS：数组分组
来源：https://cl.zhonguo4118.cn

Object.groupBy(arr, x => x.type)
来源：https://fq.zhonguo7118.cn

[U110] JS：数组分块
来源：https://oq.zhonguo4118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://yu.zhonguo2118.cn

[U111] JS：对象转 Map
来源：https://mi.zhonguo5118.cn

new Map(Object.entries(obj))
来源：https://ym.zhonguo2118.cn

[U112] JS：字符串补位
来源：https://yc.zhonguo2118.cn

"7".padStart(3, "0")
来源：https://ly.zhonguo1118.cn

[U113] JS：正则替换全部
来源：https://sx.zhonguo5118.cn

s.replaceAll("a", "b")
来源：https://tx.zhonguo2118.cn

[U114] JS：JSON 深比较
来源：https://kh.zhonguo2118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://pq.zhonguo6118.cn

[U115] JS：生成 UUID
来源：https://yy.zhonguo1118.cn

crypto.randomUUID()
来源：https://gn.zhonguo7118.cn

[U116] JS：类型检查（JSDoc）
来源：https://gg.zhonguo7118.cn

/** @param {string} name */ function f(name) {}
来源：https://iz.zhonguo1118.cn

[U117] JS：单元测试
来源：https://fo.zhonguo5118.cn

npm i -D vitest;  npx vitest
来源：https://ya.zhonguo2118.cn

[U118] JS：开发服务器
来源：https://zg.zhonguo3118.cn

npm i -D vite;  npx vite
来源：https://bf.zhonguo8118.cn

[U119] JS：生产构建
来源：https://qy.zhonguo5118.cn

npx vite build
来源：https://ia.zhonguo5118.cn

[U120] JS：读取环境变量（Vite）
来源：https://yx.zhonguo3118.cn

import.meta.env.VITE_API_URL
来源：https://hn.zhonguo6118.cn

================================================================================
来源：https://gp.zhonguo8118.cn

统计汇总
来源：https://uy.zhonguo4118.cn

================================================================================
来源：https://xa.zhonguo8118.cn

按语言统计（条）：
来源：https://rb.zhonguo7118.cn

Python ......... 252
来源：https://sm.zhonguo2118.cn

PHP ............ 252
来源：https://tl.zhonguo2118.cn

JavaScript ..... 252
来源：https://ho.zhonguo4118.cn

TypeScript ..... 212
来源：https://fu.zhonguo8118.cn

Java ........... 212
来源：https://zt.zhonguo2118.cn

Go ............. 212
来源：https://ny.zhonguo6118.cn

Ruby ........... 212
来源：https://qz.zhonguo2118.cn

C# ............. 212
来源：https://sw.zhonguo8118.cn

C .............. 30
来源：https://po.zhonguo4118.cn

C++ ............ 30
来源：https://ox.zhonguo6118.cn

SQL ............ 90
来源：https://ax.zhonguo8118.cn

Bash ........... 80
来源：https://gz.zhonguo5118.cn

Kotlin ......... 15
来源：https://um.zhonguo8118.cn

Swift .......... 15
来源：https://bl.zhonguo7118.cn

Lua ............ 10
来源：https://gx.zhonguo3118.cn

Perl ........... 10
来源：https://lz.zhonguo8118.cn

Scala .......... 10
来源：https://oo.zhonguo6118.cn

------------------------------------
来源：https://ku.zhonguo2118.cn

合计 ........... 2106 条
来源：https://xt.zhonguo7118.cn

按章节统计：
来源：https://su.zhonguo5118.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：https://pc.zhonguo1118.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：https://hp.zhonguo2118.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：https://fs.zhonguo4118.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：https://cg.zhonguo1118.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：https://ew.zhonguo8118.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：https://uj.zhonguo1118.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：https://mk.zhonguo2118.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：https://ye.zhonguo3118.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：https://nv.zhonguo4118.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：https://mn.zhonguo2118.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：https://pb.zhonguo8118.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：https://ke.zhonguo1118.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：https://lb.zhonguo2118.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：https://wk.zhonguo7118.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：https://nv.zhonguo3118.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：https://uf.zhonguo6118.cn

Q SQL 专题                              90
来源：https://sl.zhonguo7118.cn

R Bash 专题                             80
来源：https://qs.zhonguo3118.cn

S C / C++ 专题                          60
来源：https://xd.zhonguo5118.cn

T 其他语言补充                          60
来源：https://cr.zhonguo3118.cn

U 高频实用片段                         120
来源：https://py.zhonguo5118.cn

------------------------------------
来源：https://fy.zhonguo3118.cn

合计                                  2106 条
来源：https://qt.zhonguo2118.cn

--------------------------------------------------------------------------------
来源：https://gx.zhonguo8118.cn

使用提醒
来源：https://mr.zhonguo7118.cn

--------------------------------------------------------------------------------
来源：https://or.zhonguo4118.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：https://zs.zhonguo8118.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：https://yv.zhonguo7118.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：https://il.zhonguo2118.cn

在旧版本上使用前请先确认语法支持情况。
来源：https://kj.zhonguo7118.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：https://ew.zhonguo5118.cn

—— 文件结束 ——
来源：https://js.zhonguo7118.cn

================================================================================
来源：https://ke.zhonguo7118.cn

程序语言常见例子速查手册（2024 版）
来源：https://wh.zhonguo8118.cn

Common Programming Examples Cheat Book
来源：https://qd.zhonguo3118.cn

================================================================================
来源：https://lj.zhonguo2118.cn

【收录内容】
来源：https://ns.zhonguo4118.cn

覆盖 12 种语言 / 语法与常见 API：
来源：https://lo.zhonguo3118.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：https://sw.zhonguo6118.cn

SQL · Bash · C · C++
来源：https://sr.zhonguo6118.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：https://ny.zhonguo5118.cn

【使用说明】
来源：https://kn.zhonguo3118.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：https://fn.zhonguo1118.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：https://ba.zhonguo4118.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：https://yf.zhonguo3118.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：https://ss.zhonguo2118.cn

Bash:  Shell         C:     C             C++:   C++
来源：https://mw.zhonguo5118.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：https://gk.zhonguo7118.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：https://wu.zhonguo7118.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：https://hb.zhonguo1118.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：https://qh.zhonguo7118.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：https://jr.zhonguo6118.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：https://uh.zhonguo1118.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：https://vy.zhonguo3118.cn

【文件统计】
来源：https://mp.zhonguo5118.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：https://ns.zhonguo8118.cn


<!-- 参考信息 -->