代发 wailian999

[U07] Py：反转字典键值
来源：https://jc.zhonguo5118.cn

{v: k for k, v in d.items()}
来源：https://km.zhonguo1118.cn

[U08] Py：展平二维列表
来源：https://hn.zhonguo3118.cn

[y for x in nested for y in x]
来源：https://tg.zhonguo4118.cn

[U09] Py：字典取最大值的键
来源：https://gp.zhonguo5118.cn

max(d, key=d.get)
来源：https://cr.zhonguo8118.cn

[U10] Py：按值排序字典
来源：https://wr.zhonguo1118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://yl.zhonguo1118.cn

[U11] Py：生成器表达式
来源：https://eq.zhonguo5118.cn

(x * 2 for x in arr)
来源：https://jb.zhonguo8118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://qr.zhonguo5118.cn

Counter(arr).most_common(3)
来源：https://pn.zhonguo8118.cn

[U13] Py：固定长度队列
来源：https://uz.zhonguo7118.cn

deque(maxlen=10)
来源：https://nz.zhonguo3118.cn

[U14] Py：分组收集到列表
来源：https://hc.zhonguo5118.cn

defaultdict(list)
来源：https://hf.zhonguo4118.cn

[U15] Py：高精度计时
来源：https://ju.zhonguo7118.cn

t = time.perf_counter()
来源：https://fp.zhonguo1118.cn

[U16] Py：命令行参数解析
来源：https://xx.zhonguo1118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://ok.zhonguo4118.cn

[U17] Py：初始化日志
来源：https://tu.zhonguo3118.cn

logging.basicConfig(level=logging.INFO)
来源：https://io.zhonguo4118.cn

[U18] Py：预编译正则
来源：https://br.zhonguo6118.cn

pat = re.compile(r"\d+")
来源：https://qq.zhonguo5118.cn

[U19] Py：正则替换带回调
来源：https://cc.zhonguo2118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://wh.zhonguo7118.cn

[U20] Py：缓存函数结果
来源：https://hi.zhonguo3118.cn

@functools.lru_cache(maxsize=None)
来源：https://bz.zhonguo7118.cn

[U21] Py：自定义上下文管理器
来源：https://gq.zhonguo4118.cn

@contextlib.contextmanager
来源：https://na.zhonguo4118.cn

[U22] Py：矩阵转置
来源：https://hj.zhonguo2118.cn

list(zip(*m))
来源：https://ch.zhonguo8118.cn

[U23] Py：分块读取大文件
来源：https://mx.zhonguo1118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://po.zhonguo2118.cn

[U24] Py：路径操作
来源：https://dj.zhonguo5118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://hd.zhonguo5118.cn

[U25] Py：CSV 按字典读
来源：https://bw.zhonguo1118.cn

csv.DictReader(f)
来源：https://un.zhonguo5118.cn

[U26] Py：并发下载
来源：https://js.zhonguo5118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://yn.zhonguo4118.cn

[U27] Py：异步 HTTP
来源：https://df.zhonguo1118.cn

aiohttp.ClientSession() 配合 async with
来源：https://hm.zhonguo3118.cn

[U28] Py：类型别名
来源：https://dd.zhonguo4118.cn

UserId = int
来源：https://dt.zhonguo6118.cn

[U29] Py：属性校验
来源：https://wm.zhonguo4118.cn

@property 与 @x.setter 配合
来源：https://sy.zhonguo7118.cn

[U30] Py：数据类
来源：https://tw.zhonguo5118.cn

@dataclass(slots=True)
来源：https://nz.zhonguo7118.cn

[U31] Py：单测
来源：https://ur.zhonguo4118.cn

python -m pytest -q
来源：https://xa.zhonguo1118.cn

[U32] Py：代码格式化
来源：https://sr.zhonguo8118.cn

ruff format . && ruff check --fix .
来源：https://me.zhonguo4118.cn

[U33] Py：打包发布
来源：https://qc.zhonguo6118.cn

python -m build  （依赖 pyproject.toml）
来源：https://pk.zhonguo4118.cn

[U34] Py：判断编码
来源：https://yn.zhonguo6118.cn

chardet.detect(raw)
来源：https://ge.zhonguo4118.cn

[U35] Py：发送邮件
来源：https://sr.zhonguo1118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://lj.zhonguo6118.cn

[U36] Py：定时任务
来源：https://mi.zhonguo6118.cn

schedule.every(10).minutes.do(job)
来源：https://vj.zhonguo7118.cn

[U37] Py：读写 Excel
来源：https://il.zhonguo7118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://au.zhonguo2118.cn

[U38] Py：获取脚本所在目录
来源：https://dd.zhonguo6118.cn

Path(__file__).resolve().parent
来源：https://za.zhonguo3118.cn

[U39] Py：判断是否在交互环境
来源：https://jv.zhonguo3118.cn

sys.stdout.isatty()
来源：https://by.zhonguo8118.cn

[U40] Py：打印到标准错误
来源：https://ks.zhonguo2118.cn

print("err", file=sys.stderr)
来源：https://ap.zhonguo2118.cn

[U41] PHP：初始化 Composer 项目
来源：https://fe.zhonguo1118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://ph.zhonguo1118.cn

[U42] PHP：PSR-4 自动加载
来源：https://jw.zhonguo1118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://sb.zhonguo8118.cn

[U43] PHP：声明命名空间
来源：https://bk.zhonguo5118.cn

namespace App\Http;
来源：https://xu.zhonguo8118.cn

[U44] PHP：开启严格类型
来源：https://qa.zhonguo3118.cn

declare(strict_types=1);
来源：https://yp.zhonguo1118.cn

[U45] PHP：类型声明与返回类型
来源：https://ja.zhonguo3118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://hl.zhonguo4118.cn

[U46] PHP：可空类型
来源：https://or.zhonguo8118.cn

?string $name = null
来源：https://tp.zhonguo1118.cn

[U47] PHP：联合类型
来源：https://wr.zhonguo6118.cn

int|string $id
来源：https://ks.zhonguo5118.cn

[U48] PHP：纯枚举
来源：https://pt.zhonguo7118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://sy.zhonguo4118.cn

[U49] PHP：只读属性
来源：https://pj.zhonguo1118.cn

public readonly string $name
来源：https://ai.zhonguo4118.cn

[U50] PHP：构造器属性提升
来源：https://em.zhonguo7118.cn

public function __construct(private int $id) {}
来源：https://fq.zhonguo5118.cn

[U51] PHP：数组解构
来源：https://xg.zhonguo1118.cn

[$a, $b] = $arr;
来源：https://fl.zhonguo2118.cn

[U52] PHP：箭头函数
来源：https://ed.zhonguo8118.cn

$double = fn($x) => $x * 2;
来源：https://hj.zhonguo4118.cn

[U53] PHP：空合并运算符
来源：https://zm.zhonguo3118.cn

$v = $a ?? $b ?? "default";
来源：https://ro.zhonguo7118.cn

[U54] PHP：空安全调用
来源：https://cq.zhonguo1118.cn

$obj?->method()
来源：https://hb.zhonguo3118.cn

[U55] PHP：match 表达式
来源：https://cb.zhonguo8118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://dn.zhonguo3118.cn

[U56] PHP：命名参数
来源：https://wk.zhonguo2118.cn

f(a: 1, b: 2)
来源：https://dv.zhonguo1118.cn

[U57] PHP：字符串插值
来源：https://wm.zhonguo2118.cn

"值: {$a}"
来源：https://fq.zhonguo5118.cn

[U58] PHP：数组三件套
来源：https://nk.zhonguo2118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://ii.zhonguo5118.cn

[U59] PHP：自定义排序
来源：https://wf.zhonguo4118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://tc.zhonguo1118.cn

[U60] PHP：JSON 编解码
来源：https://mt.zhonguo1118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://sd.zhonguo7118.cn

[U61] PHP：正则
来源：https://gr.zhonguo3118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://fd.zhonguo7118.cn

[U62] PHP：日期对象
来源：https://zi.zhonguo6118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://gm.zhonguo3118.cn

[U63] PHP：文件读写
来源：https://tr.zhonguo5118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://ig.zhonguo5118.cn

[U64] PHP：目录遍历
来源：https://gc.zhonguo5118.cn

glob("dir/*.php");  scandir("dir");
来源：https://la.zhonguo6118.cn

[U65] PHP：会话
来源：https://ts.zhonguo1118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://eu.zhonguo3118.cn

[U66] PHP：设置 Cookie
来源：https://sc.zhonguo4118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://ih.zhonguo7118.cn

[U67] PHP：处理文件上传
来源：https://qt.zhonguo1118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://eu.zhonguo1118.cn

[U68] PHP：PDO 连接
来源：https://yg.zhonguo8118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://ac.zhonguo1118.cn

[U69] PHP：PDO 预处理
来源：https://mq.zhonguo8118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://dt.zhonguo8118.cn

[U70] PHP：PDO 事务
来源：https://dy.zhonguo5118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://zc.zhonguo1118.cn

[U71] PHP：抛出异常
来源：https://lw.zhonguo4118.cn

throw new RuntimeException("失败", 500);
来源：https://za.zhonguo4118.cn

[U72] PHP：写错误日志
来源：https://ts.zhonguo7118.cn

error_log("失败: " . $e->getMessage());
来源：https://uv.zhonguo2118.cn

[U73] PHP：读取 ini 配置
来源：https://wa.zhonguo6118.cn

parse_ini_file("config.ini", true)
来源：https://fh.zhonguo6118.cn

[U74] PHP：读取环境变量
来源：https://pw.zhonguo4118.cn

getenv("APP_ENV") ?: "production"
来源：https://li.zhonguo8118.cn

[U75] PHP：依赖注入
来源：https://lk.zhonguo1118.cn

composer require psr/container
来源：https://hr.zhonguo7118.cn

[U76] PHP：简单路由
来源：https://km.zhonguo3118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://sq.zhonguo3118.cn

[U77] PHP：模板渲染
来源：https://pc.zhonguo1118.cn

composer require twig/twig
来源：https://lp.zhonguo8118.cn

[U78] PHP：单元测试
来源：https://zw.zhonguo8118.cn

composer require --dev phpunit/phpunit
来源：https://to.zhonguo6118.cn

[U79] PHP：静态分析
来源：https://vr.zhonguo7118.cn

composer require --dev phpstan/phpstan
来源：https://eg.zhonguo1118.cn

[U80] PHP：代码规范修复
来源：https://wv.zhonguo7118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://db.zhonguo8118.cn

[U81] JS：初始化项目
来源：https://vx.zhonguo4118.cn

npm init -y;  npm i express
来源：https://pk.zhonguo4118.cn

[U82] JS：package.json 脚本
来源：https://yw.zhonguo5118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://av.zhonguo3118.cn

[U83] JS：ES Module 导入导出
来源：https://gj.zhonguo1118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://lh.zhonguo5118.cn

[U84] JS：CommonJS 写法
来源：https://nc.zhonguo3118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://ie.zhonguo2118.cn

[U85] JS：可选链
来源：https://cx.zhonguo4118.cn

a?.b?.c
来源：https://fa.zhonguo3118.cn

[U86] JS：空值合并
来源：https://xt.zhonguo7118.cn

a ?? b
来源：https://ih.zhonguo8118.cn

[U87] JS：解构默认值
来源：https://il.zhonguo6118.cn

const { a = 1, b = 2 } = obj;
来源：https://db.zhonguo7118.cn

[U88] JS：对象展开合并
来源：https://tm.zhonguo2118.cn

{ ...a, ...b }
来源：https://qk.zhonguo7118.cn

[U89] JS：数组去重
来源：https://rl.zhonguo3118.cn

[...new Set(arr)]
来源：https://py.zhonguo8118.cn

[U90] JS：数字数组排序
来源：https://fm.zhonguo3118.cn

[...arr].sort((a, b) => a - b)
来源：https://du.zhonguo4118.cn

[U91] JS：对象键值遍历
来源：https://fb.zhonguo8118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://sn.zhonguo5118.cn

[U92] JS：深拷贝
来源：https://bq.zhonguo1118.cn

structuredClone(obj)
来源：https://qu.zhonguo7118.cn

[U93] JS：模板字符串
来源：https://dm.zhonguo2118.cn

`共 ${n} 条`
来源：https://lc.zhonguo7118.cn

[U94] JS：箭头函数
来源：https://lu.zhonguo7118.cn

const double = x => x * 2;
来源：https://ea.zhonguo1118.cn

[U95] JS：Promise 包装
来源：https://ga.zhonguo8118.cn

new Promise((resolve, reject) => {})
来源：https://bz.zhonguo8118.cn

[U96] JS：async/await 与异常
来源：https://ql.zhonguo5118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://hc.zhonguo4118.cn

[U97] JS：并发请求
来源：https://tn.zhonguo8118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://vi.zhonguo6118.cn

[U98] JS：fetch 带 JSON
来源：https://gz.zhonguo7118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://ym.zhonguo5118.cn

[U99] JS：事件监听
来源：https://it.zhonguo4118.cn

el.addEventListener("click", e => {})
来源：https://vx.zhonguo2118.cn

[U100] JS：DOM 查询
来源：https://bg.zhonguo5118.cn

document.querySelector(".item")
来源：https://yx.zhonguo2118.cn

[U101] JS：classList 操作
来源：https://is.zhonguo2118.cn

el.classList.toggle("active")
来源：https://vb.zhonguo3118.cn

[U102] JS：本地存储
来源：https://xa.zhonguo5118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://uo.zhonguo8118.cn

[U103] JS：定时器
来源：https://hp.zhonguo8118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://rz.zhonguo8118.cn

[U104] JS：防抖
来源：https://xq.zhonguo5118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://jf.zhonguo6118.cn

[U105] JS：节流
来源：https://bp.zhonguo7118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://ul.zhonguo4118.cn

[U106] JS：日期格式化
来源：https://sk.zhonguo4118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://qg.zhonguo6118.cn

[U107] JS：数字千分位
来源：https://od.zhonguo6118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://uc.zhonguo2118.cn

[U108] JS：随机整数
来源：https://jb.zhonguo5118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://vv.zhonguo5118.cn

[U109] JS：数组分组
来源：https://gq.zhonguo7118.cn

Object.groupBy(arr, x => x.type)
来源：https://ur.zhonguo6118.cn

[U110] JS：数组分块
来源：https://ts.zhonguo7118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://ow.zhonguo2118.cn

[U111] JS：对象转 Map
来源：https://hk.zhonguo2118.cn

new Map(Object.entries(obj))
来源：https://qo.zhonguo6118.cn

[U112] JS：字符串补位
来源：https://vf.zhonguo3118.cn

"7".padStart(3, "0")
来源：https://xc.zhonguo7118.cn

[U113] JS：正则替换全部
来源：https://zd.zhonguo6118.cn

s.replaceAll("a", "b")
来源：https://rw.zhonguo4118.cn

[U114] JS：JSON 深比较
来源：https://vy.zhonguo7118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://xv.zhonguo8118.cn

[U115] JS：生成 UUID
来源：https://zi.zhonguo8118.cn

crypto.randomUUID()
来源：https://wn.zhonguo2118.cn

[U116] JS：类型检查（JSDoc）
来源：https://zm.zhonguo2118.cn

/** @param {string} name */ function f(name) {}
来源：https://tt.zhonguo7118.cn

[U117] JS：单元测试
来源：https://zw.zhonguo5118.cn

npm i -D vitest;  npx vitest
来源：https://ht.zhonguo1118.cn

[U118] JS：开发服务器
来源：https://ym.zhonguo5118.cn

npm i -D vite;  npx vite
来源：https://wm.zhonguo5118.cn

[U119] JS：生产构建
来源：https://za.zhonguo4118.cn

npx vite build
来源：https://va.zhonguo2118.cn

[U120] JS：读取环境变量（Vite）
来源：https://zf.zhonguo6118.cn

import.meta.env.VITE_API_URL
来源：https://vq.zhonguo1118.cn

================================================================================
来源：https://gs.zhonguo8118.cn

统计汇总
来源：https://yt.zhonguo7118.cn

================================================================================
来源：https://pc.zhonguo1118.cn

按语言统计（条）：
来源：https://ku.zhonguo2118.cn

Python ......... 252
来源：https://zf.zhonguo7118.cn

PHP ............ 252
来源：https://jz.zhonguo6118.cn

JavaScript ..... 252
来源：https://td.zhonguo8118.cn

TypeScript ..... 212
来源：https://bk.zhonguo6118.cn

Java ........... 212
来源：https://le.zhonguo3118.cn

Go ............. 212
来源：https://uz.zhonguo8118.cn

Ruby ........... 212
来源：https://ty.zhonguo7118.cn

C# ............. 212
来源：https://cu.zhonguo3118.cn

C .............. 30
来源：https://lh.zhonguo1118.cn

C++ ............ 30
来源：https://en.zhonguo5118.cn

SQL ............ 90
来源：https://qk.zhonguo5118.cn

Bash ........... 80
来源：https://gj.zhonguo4118.cn

Kotlin ......... 15
来源：https://ab.zhonguo5118.cn

Swift .......... 15
来源：https://ux.zhonguo7118.cn

Lua ............ 10
来源：https://ow.zhonguo6118.cn

Perl ........... 10
来源：https://pa.zhonguo1118.cn

Scala .......... 10
来源：https://uw.zhonguo5118.cn

------------------------------------
来源：https://ys.zhonguo6118.cn

合计 ........... 2106 条
来源：https://ak.zhonguo1118.cn

按章节统计：
来源：https://jz.zhonguo3118.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：https://hf.zhonguo4118.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：https://or.zhonguo5118.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：https://wb.zhonguo4118.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：https://wc.zhonguo6118.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：https://xc.zhonguo6118.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：https://qx.zhonguo6118.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：https://tc.zhonguo4118.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：https://zd.zhonguo8118.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：https://qw.zhonguo1118.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：https://ev.zhonguo3118.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：https://kp.zhonguo5118.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：https://rt.zhonguo1118.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：https://we.zhonguo8118.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：https://cf.zhonguo3118.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：https://db.zhonguo3118.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：https://ex.zhonguo1118.cn

Q SQL 专题                              90
来源：https://ym.zhonguo5118.cn

R Bash 专题                             80
来源：https://my.zhonguo8118.cn

S C / C++ 专题                          60
来源：https://jj.zhonguo8118.cn

T 其他语言补充                          60
来源：https://pd.zhonguo7118.cn

U 高频实用片段                         120
来源：https://ct.zhonguo3118.cn

------------------------------------
来源：https://za.zhonguo5118.cn

合计                                  2106 条
来源：https://xd.zhonguo7118.cn

--------------------------------------------------------------------------------
来源：https://ky.zhonguo8118.cn

使用提醒
来源：https://ou.zhonguo6118.cn

--------------------------------------------------------------------------------
来源：https://oo.zhonguo7118.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：https://md.zhonguo7118.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：https://pj.zhonguo2118.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：https://nq.zhonguo8118.cn

在旧版本上使用前请先确认语法支持情况。
来源：https://jw.zhonguo7118.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：https://wg.zhonguo8118.cn

—— 文件结束 ——
来源：https://mn.zhonguo3118.cn

================================================================================
来源：https://vb.zhonguo1118.cn

程序语言常见例子速查手册（2024 版）
来源：https://ev.zhonguo2118.cn

Common Programming Examples Cheat Book
来源：https://xi.zhonguo6118.cn

================================================================================
来源：https://xq.zhonguo5118.cn

【收录内容】
来源：https://nx.zhonguo6118.cn

覆盖 12 种语言 / 语法与常见 API：
来源：https://re.zhonguo6118.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：https://xv.zhonguo1118.cn

SQL · Bash · C · C++
来源：https://yg.zhonguo6118.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：https://to.zhonguo5118.cn

【使用说明】
来源：https://xk.zhonguo3118.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：https://bb.zhonguo2118.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：https://jg.zhonguo2118.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：https://ey.zhonguo8118.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：https://qp.zhonguo7118.cn

Bash:  Shell         C:     C             C++:   C++
来源：https://sc.zhonguo6118.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：https://st.zhonguo4118.cn


<!-- 参考信息 -->