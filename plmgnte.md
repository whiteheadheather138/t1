代发 wailian999

[U13] Py：固定长度队列
来源：https://rp.zhonguo7118.cn

deque(maxlen=10)
来源：https://nt.zhonguo7118.cn

[U14] Py：分组收集到列表
来源：https://pj.zhonguo5118.cn

defaultdict(list)
来源：https://yc.zhonguo2118.cn

[U15] Py：高精度计时
来源：https://pz.zhonguo2118.cn

t = time.perf_counter()
来源：https://vo.zhonguo7118.cn

[U16] Py：命令行参数解析
来源：https://ec.zhonguo1118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://zo.zhonguo2118.cn

[U17] Py：初始化日志
来源：https://bc.zhonguo2118.cn

logging.basicConfig(level=logging.INFO)
来源：https://ow.zhonguo2118.cn

[U18] Py：预编译正则
来源：https://zf.zhonguo6118.cn

pat = re.compile(r"\d+")
来源：https://sl.zhonguo8118.cn

[U19] Py：正则替换带回调
来源：https://zd.zhonguo4118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://vq.zhonguo5118.cn

[U20] Py：缓存函数结果
来源：https://jk.zhonguo8118.cn

@functools.lru_cache(maxsize=None)
来源：https://wt.zhonguo6118.cn

[U21] Py：自定义上下文管理器
来源：https://ev.zhonguo6118.cn

@contextlib.contextmanager
来源：https://mh.zhonguo6118.cn

[U22] Py：矩阵转置
来源：https://en.zhonguo4118.cn

list(zip(*m))
来源：https://yq.zhonguo8118.cn

[U23] Py：分块读取大文件
来源：https://cw.zhonguo4118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://xt.zhonguo1118.cn

[U24] Py：路径操作
来源：https://ot.zhonguo5118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://yl.zhonguo6118.cn

[U25] Py：CSV 按字典读
来源：https://bz.zhonguo1118.cn

csv.DictReader(f)
来源：https://yf.zhonguo4118.cn

[U26] Py：并发下载
来源：https://ll.zhonguo3118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://bq.zhonguo3118.cn

[U27] Py：异步 HTTP
来源：https://dc.zhonguo5118.cn

aiohttp.ClientSession() 配合 async with
来源：https://fv.zhonguo7118.cn

[U28] Py：类型别名
来源：https://ld.zhonguo5118.cn

UserId = int
来源：https://zf.zhonguo2118.cn

[U29] Py：属性校验
来源：https://zq.zhonguo5118.cn

@property 与 @x.setter 配合
来源：https://rl.zhonguo7118.cn

[U30] Py：数据类
来源：https://it.zhonguo3118.cn

@dataclass(slots=True)
来源：https://yx.zhonguo1118.cn

[U31] Py：单测
来源：https://ct.zhonguo8118.cn

python -m pytest -q
来源：https://tq.zhonguo6118.cn

[U32] Py：代码格式化
来源：https://bb.zhonguo1118.cn

ruff format . && ruff check --fix .
来源：https://hf.zhonguo5118.cn

[U33] Py：打包发布
来源：https://uy.zhonguo3118.cn

python -m build  （依赖 pyproject.toml）
来源：https://qt.zhonguo5118.cn

[U34] Py：判断编码
来源：https://nj.zhonguo8118.cn

chardet.detect(raw)
来源：https://as.zhonguo1118.cn

[U35] Py：发送邮件
来源：https://oi.zhonguo3118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://to.zhonguo8118.cn

[U36] Py：定时任务
来源：https://wv.zhonguo7118.cn

schedule.every(10).minutes.do(job)
来源：https://vy.zhonguo4118.cn

[U37] Py：读写 Excel
来源：https://iz.zhonguo3118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://ug.zhonguo4118.cn

[U38] Py：获取脚本所在目录
来源：https://ms.zhonguo8118.cn

Path(__file__).resolve().parent
来源：https://hs.zhonguo5118.cn

[U39] Py：判断是否在交互环境
来源：https://mg.zhonguo1118.cn

sys.stdout.isatty()
来源：https://ub.zhonguo1118.cn

[U40] Py：打印到标准错误
来源：https://hd.zhonguo1118.cn

print("err", file=sys.stderr)
来源：https://by.zhonguo1118.cn

[U41] PHP：初始化 Composer 项目
来源：https://ze.zhonguo1118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://qd.zhonguo7118.cn

[U42] PHP：PSR-4 自动加载
来源：https://nc.zhonguo3118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://ey.zhonguo3118.cn

[U43] PHP：声明命名空间
来源：https://bl.zhonguo2118.cn

namespace App\Http;
来源：https://zg.zhonguo2118.cn

[U44] PHP：开启严格类型
来源：https://ex.zhonguo7118.cn

declare(strict_types=1);
来源：https://kx.zhonguo4118.cn

[U45] PHP：类型声明与返回类型
来源：https://eq.zhonguo8118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://hg.zhonguo7118.cn

[U46] PHP：可空类型
来源：https://tg.zhonguo4118.cn

?string $name = null
来源：https://mx.zhonguo7118.cn

[U47] PHP：联合类型
来源：https://bb.zhonguo7118.cn

int|string $id
来源：https://gw.zhonguo6118.cn

[U48] PHP：纯枚举
来源：https://iy.zhonguo5118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://uo.zhonguo1118.cn

[U49] PHP：只读属性
来源：https://df.zhonguo4118.cn

public readonly string $name
来源：https://xs.zhonguo2118.cn

[U50] PHP：构造器属性提升
来源：https://no.zhonguo3118.cn

public function __construct(private int $id) {}
来源：https://bm.zhonguo8118.cn

[U51] PHP：数组解构
来源：https://fd.zhonguo1118.cn

[$a, $b] = $arr;
来源：https://fp.zhonguo7118.cn

[U52] PHP：箭头函数
来源：https://lj.zhonguo8118.cn

$double = fn($x) => $x * 2;
来源：https://bg.zhonguo1118.cn

[U53] PHP：空合并运算符
来源：https://uw.zhonguo6118.cn

$v = $a ?? $b ?? "default";
来源：https://pd.zhonguo4118.cn

[U54] PHP：空安全调用
来源：https://ii.zhonguo2118.cn

$obj?->method()
来源：https://pb.zhonguo1118.cn

[U55] PHP：match 表达式
来源：https://bb.zhonguo8118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://fh.zhonguo5118.cn

[U56] PHP：命名参数
来源：https://po.zhonguo1118.cn

f(a: 1, b: 2)
来源：https://os.zhonguo6118.cn

[U57] PHP：字符串插值
来源：https://ln.zhonguo6118.cn

"值: {$a}"
来源：https://ca.zhonguo7118.cn

[U58] PHP：数组三件套
来源：https://rv.zhonguo8118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://wa.zhonguo8118.cn

[U59] PHP：自定义排序
来源：https://wo.zhonguo2118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://nb.zhonguo2118.cn

[U60] PHP：JSON 编解码
来源：https://nv.zhonguo4118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://lr.zhonguo7118.cn

[U61] PHP：正则
来源：https://ck.zhonguo8118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://kp.zhonguo6118.cn

[U62] PHP：日期对象
来源：https://rt.zhonguo4118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://it.zhonguo8118.cn

[U63] PHP：文件读写
来源：https://hy.zhonguo2118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://ye.zhonguo6118.cn

[U64] PHP：目录遍历
来源：https://np.zhonguo7118.cn

glob("dir/*.php");  scandir("dir");
来源：https://ku.zhonguo5118.cn

[U65] PHP：会话
来源：https://tv.zhonguo1118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://my.zhonguo3118.cn

[U66] PHP：设置 Cookie
来源：https://fn.zhonguo1118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://fr.zhonguo7118.cn

[U67] PHP：处理文件上传
来源：https://fi.zhonguo7118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://da.zhonguo2118.cn

[U68] PHP：PDO 连接
来源：https://si.zhonguo8118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://ub.zhonguo6118.cn

[U69] PHP：PDO 预处理
来源：https://vo.zhonguo2118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://cu.zhonguo7118.cn

[U70] PHP：PDO 事务
来源：https://vf.zhonguo2118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://ko.zhonguo3118.cn

[U71] PHP：抛出异常
来源：https://jm.zhonguo2118.cn

throw new RuntimeException("失败", 500);
来源：https://vm.zhonguo2118.cn

[U72] PHP：写错误日志
来源：https://nd.zhonguo7118.cn

error_log("失败: " . $e->getMessage());
来源：https://hy.zhonguo6118.cn

[U73] PHP：读取 ini 配置
来源：https://yd.zhonguo6118.cn

parse_ini_file("config.ini", true)
来源：https://zi.zhonguo2118.cn

[U74] PHP：读取环境变量
来源：https://pn.zhonguo8118.cn

getenv("APP_ENV") ?: "production"
来源：https://de.zhonguo1118.cn

[U75] PHP：依赖注入
来源：https://oj.zhonguo1118.cn

composer require psr/container
来源：https://jx.zhonguo4118.cn

[U76] PHP：简单路由
来源：https://xl.zhonguo1118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://rz.zhonguo5118.cn

[U77] PHP：模板渲染
来源：https://et.zhonguo5118.cn

composer require twig/twig
来源：https://si.zhonguo4118.cn

[U78] PHP：单元测试
来源：https://fa.zhonguo4118.cn

composer require --dev phpunit/phpunit
来源：https://bh.zhonguo1118.cn

[U79] PHP：静态分析
来源：https://po.zhonguo8118.cn

composer require --dev phpstan/phpstan
来源：https://kx.zhonguo4118.cn

[U80] PHP：代码规范修复
来源：https://di.zhonguo3118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://dw.zhonguo4118.cn

[U81] JS：初始化项目
来源：https://ug.zhonguo4118.cn

npm init -y;  npm i express
来源：https://dj.zhonguo3118.cn

[U82] JS：package.json 脚本
来源：https://ll.zhonguo8118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://te.zhonguo7118.cn

[U83] JS：ES Module 导入导出
来源：https://va.zhonguo1118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://tv.zhonguo3118.cn

[U84] JS：CommonJS 写法
来源：https://wc.zhonguo4118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://hc.zhonguo5118.cn

[U85] JS：可选链
来源：https://mu.zhonguo8118.cn

a?.b?.c
来源：https://zv.zhonguo6118.cn

[U86] JS：空值合并
来源：https://bm.zhonguo4118.cn

a ?? b
来源：https://mk.zhonguo5118.cn

[U87] JS：解构默认值
来源：https://cd.zhonguo6118.cn

const { a = 1, b = 2 } = obj;
来源：https://zh.zhonguo7118.cn

[U88] JS：对象展开合并
来源：https://zo.zhonguo1118.cn

{ ...a, ...b }
来源：https://bk.zhonguo3118.cn

[U89] JS：数组去重
来源：https://rl.zhonguo1118.cn

[...new Set(arr)]
来源：https://xv.zhonguo8118.cn

[U90] JS：数字数组排序
来源：https://ss.zhonguo5118.cn

[...arr].sort((a, b) => a - b)
来源：https://dp.zhonguo1118.cn

[U91] JS：对象键值遍历
来源：https://xv.zhonguo6118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://vq.zhonguo3118.cn

[U92] JS：深拷贝
来源：https://ro.zhonguo5118.cn

structuredClone(obj)
来源：https://rs.zhonguo6118.cn

[U93] JS：模板字符串
来源：https://se.zhonguo8118.cn

`共 ${n} 条`
来源：https://lf.zhonguo8118.cn

[U94] JS：箭头函数
来源：https://kc.zhonguo1118.cn

const double = x => x * 2;
来源：https://zk.zhonguo4118.cn

[U95] JS：Promise 包装
来源：https://up.zhonguo8118.cn

new Promise((resolve, reject) => {})
来源：https://ot.zhonguo5118.cn

[U96] JS：async/await 与异常
来源：https://xw.zhonguo1118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://ri.zhonguo4118.cn

[U97] JS：并发请求
来源：https://gt.zhonguo6118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://lx.zhonguo3118.cn

[U98] JS：fetch 带 JSON
来源：https://mp.zhonguo4118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://ph.zhonguo4118.cn

[U99] JS：事件监听
来源：https://jm.zhonguo1118.cn

el.addEventListener("click", e => {})
来源：https://of.zhonguo3118.cn

[U100] JS：DOM 查询
来源：https://tw.zhonguo7118.cn

document.querySelector(".item")
来源：https://in.zhonguo1118.cn

[U101] JS：classList 操作
来源：https://wj.zhonguo1118.cn

el.classList.toggle("active")
来源：https://rk.zhonguo8118.cn

[U102] JS：本地存储
来源：https://cb.zhonguo8118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://tm.zhonguo7118.cn

[U103] JS：定时器
来源：https://xw.zhonguo8118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://dk.zhonguo4118.cn

[U104] JS：防抖
来源：https://ya.zhonguo5118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://kt.zhonguo2118.cn

[U105] JS：节流
来源：https://qz.zhonguo3118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://qq.zhonguo3118.cn

[U106] JS：日期格式化
来源：https://af.zhonguo7118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://jm.zhonguo4118.cn

[U107] JS：数字千分位
来源：https://vh.zhonguo7118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://tq.zhonguo2118.cn

[U108] JS：随机整数
来源：https://sk.zhonguo3118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://do.zhonguo5118.cn

[U109] JS：数组分组
来源：https://pa.zhonguo3118.cn

Object.groupBy(arr, x => x.type)
来源：https://wn.zhonguo1118.cn

[U110] JS：数组分块
来源：https://bs.zhonguo6118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://tm.zhonguo6118.cn

[U111] JS：对象转 Map
来源：https://dy.zhonguo3118.cn

new Map(Object.entries(obj))
来源：https://zd.zhonguo3118.cn

[U112] JS：字符串补位
来源：https://jm.zhonguo6118.cn

"7".padStart(3, "0")
来源：https://no.zhonguo7118.cn

[U113] JS：正则替换全部
来源：https://zp.zhonguo1118.cn

s.replaceAll("a", "b")
来源：https://yo.zhonguo3118.cn

[U114] JS：JSON 深比较
来源：https://tt.zhonguo6118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://nt.zhonguo7118.cn

[U115] JS：生成 UUID
来源：https://ie.zhonguo1118.cn

crypto.randomUUID()
来源：https://pj.zhonguo1118.cn

[U116] JS：类型检查（JSDoc）
来源：https://ro.zhonguo2118.cn

/** @param {string} name */ function f(name) {}
来源：https://yi.zhonguo6118.cn

[U117] JS：单元测试
来源：https://il.zhonguo3118.cn

npm i -D vitest;  npx vitest
来源：https://yy.zhonguo6118.cn

[U118] JS：开发服务器
来源：https://al.zhonguo2118.cn

npm i -D vite;  npx vite
来源：https://ym.zhonguo3118.cn

[U119] JS：生产构建
来源：https://fd.zhonguo1118.cn

npx vite build
来源：https://sh.zhonguo8118.cn

[U120] JS：读取环境变量（Vite）
来源：https://zv.zhonguo1118.cn

import.meta.env.VITE_API_URL
来源：https://jh.zhonguo1118.cn

================================================================================
来源：https://km.zhonguo6118.cn

统计汇总
来源：https://em.zhonguo7118.cn

================================================================================
来源：https://ge.zhonguo8118.cn

按语言统计（条）：
来源：https://hn.zhonguo5118.cn

Python ......... 252
来源：https://rq.zhonguo3118.cn

PHP ............ 252
来源：https://ke.zhonguo5118.cn

JavaScript ..... 252
来源：https://hm.zhonguo1118.cn

TypeScript ..... 212
来源：https://ir.zhonguo7118.cn

Java ........... 212
来源：https://cr.zhonguo3118.cn

Go ............. 212
来源：https://ip.zhonguo4118.cn

Ruby ........... 212
来源：https://rc.zhonguo1118.cn

C# ............. 212
来源：https://xl.zhonguo7118.cn

C .............. 30
来源：https://st.zhonguo7118.cn

C++ ............ 30
来源：https://mq.zhonguo5118.cn

SQL ............ 90
来源：https://vc.zhonguo2118.cn

Bash ........... 80
来源：https://rb.zhonguo3118.cn

Kotlin ......... 15
来源：https://ep.zhonguo8118.cn

Swift .......... 15
来源：https://wm.zhonguo5118.cn

Lua ............ 10
来源：https://rn.zhonguo6118.cn

Perl ........... 10
来源：https://kr.zhonguo7118.cn

Scala .......... 10
来源：https://hz.zhonguo6118.cn

------------------------------------
来源：https://xe.zhonguo3118.cn

合计 ........... 2106 条
来源：https://uv.zhonguo4118.cn

按章节统计：
来源：https://nw.zhonguo1118.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：https://nw.zhonguo8118.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：https://ke.zhonguo1118.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：https://id.zhonguo2118.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：https://pd.zhonguo2118.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：https://hy.zhonguo3118.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：https://qg.zhonguo3118.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：https://sc.zhonguo1118.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：https://jg.zhonguo8118.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：https://dg.zhonguo5118.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：https://gi.zhonguo1118.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：https://ki.zhonguo4118.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：https://kv.zhonguo5118.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：https://qo.zhonguo3118.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：https://bm.zhonguo6118.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：https://cn.zhonguo4118.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：https://kz.zhonguo3118.cn

Q SQL 专题                              90
来源：https://fm.zhonguo8118.cn

R Bash 专题                             80
来源：https://de.zhonguo2118.cn

S C / C++ 专题                          60
来源：https://ns.zhonguo6118.cn

T 其他语言补充                          60
来源：https://uh.zhonguo7118.cn

U 高频实用片段                         120
来源：https://sj.zhonguo4118.cn

------------------------------------
来源：https://eu.zhonguo2118.cn

合计                                  2106 条
来源：https://dh.zhonguo3118.cn

--------------------------------------------------------------------------------
来源：https://vd.zhonguo2118.cn

使用提醒
来源：https://sc.zhonguo5118.cn

--------------------------------------------------------------------------------
来源：https://za.zhonguo1118.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：https://zl.zhonguo2118.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：https://gr.zhonguo6118.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：https://zk.zhonguo5118.cn

在旧版本上使用前请先确认语法支持情况。
来源：https://qn.zhonguo2118.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：https://ag.zhonguo2118.cn

—— 文件结束 ——
来源：https://cv.zhonguo2118.cn

================================================================================
来源：https://kf.zhonguo7118.cn

程序语言常见例子速查手册（2024 版）
来源：https://bm.zhonguo3118.cn

Common Programming Examples Cheat Book
来源：https://iu.zhonguo5118.cn

================================================================================
来源：https://ks.zhonguo8118.cn

【收录内容】
来源：https://fk.zhonguo6118.cn

覆盖 12 种语言 / 语法与常见 API：
来源：https://rw.zhonguo5118.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：https://iv.zhonguo5118.cn

SQL · Bash · C · C++
来源：https://ua.zhonguo7118.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：https://xq.zhonguo2118.cn

【使用说明】
来源：https://gh.zhonguo8118.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：https://iu.zhonguo5118.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：https://kb.zhonguo7118.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：https://xu.zhonguo6118.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：https://aj.zhonguo4118.cn

Bash:  Shell         C:     C             C++:   C++
来源：https://zi.zhonguo5118.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：https://ny.zhonguo2118.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：https://qo.zhonguo6118.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：https://tx.zhonguo1118.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：https://lf.zhonguo7118.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：https://ex.zhonguo4118.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：https://iy.zhonguo2118.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：https://wy.zhonguo1118.cn

【文件统计】
来源：https://gd.zhonguo3118.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：https://yt.zhonguo7118.cn

--------------------------------------------------------------------------------
来源：https://ws.zhonguo4118.cn

目  录
来源：https://ni.zhonguo1118.cn

--------------------------------------------------------------------------------
来源：https://ne.zhonguo6118.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：https://gt.zhonguo3118.cn


<!-- 参考信息 -->