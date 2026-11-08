代发 wailian999

[T47] Perl：正则捕获
来源：https://iy.zhonguo6118.cn

if ($s =~ /(\d+)/) { print $1; }
来源：https://ap.zhonguo2118.cn

[T48] Perl：正则替换
来源：https://xu.zhonguo4118.cn

$s =~ s/old/new/g;
来源：https://bn.zhonguo5118.cn

[T49] Perl：函数
来源：https://ir.zhonguo2118.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：https://wk.zhonguo8118.cn

[T50] Perl：逐行读文件
来源：https://mp.zhonguo1118.cn

open my $fh, "<", "a.txt" or die $!;
来源：https://bu.zhonguo2118.cn

while (my $line = <$fh>) { print $line; }
来源：https://pw.zhonguo5118.cn

[T51] Scala：Hello World
来源：https://db.zhonguo5118.cn

println("Hello")
来源：https://ed.zhonguo1118.cn

[T52] Scala：变量
来源：https://qk.zhonguo7118.cn

val a = 1;  var b = 2
来源：https://aj.zhonguo1118.cn

[T53] Scala：字符串插值
来源：https://ji.zhonguo7118.cn

s"值: $b"
来源：https://uz.zhonguo7118.cn

[T54] Scala：集合映射
来源：https://ks.zhonguo4118.cn

List(1, 2, 3).map(_ * 2)
来源：https://mz.zhonguo2118.cn

[T55] Scala：集合过滤
来源：https://zf.zhonguo6118.cn

List(1, 2, 3).filter(_ > 1)
来源：https://ia.zhonguo5118.cn

[T56] Scala：样例类
来源：https://ic.zhonguo3118.cn

case class User(name: String, age: Int)
来源：https://fl.zhonguo4118.cn

[T57] Scala：模式匹配
来源：https://ia.zhonguo1118.cn

x match { case 1 => "一"; case _ => "其他" }
来源：https://dn.zhonguo1118.cn

[T58] Scala：函数定义
来源：https://df.zhonguo3118.cn

def add(a: Int, b: Int): Int = a + b
来源：https://ur.zhonguo3118.cn

[T59] Scala：循环
来源：https://wz.zhonguo6118.cn

for (i <- 1 to 10) println(i)
来源：https://ek.zhonguo2118.cn

[T60] Scala：折叠
来源：https://tf.zhonguo2118.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：https://ts.zhonguo3118.cn

================================================================================
来源：https://ku.zhonguo7118.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：https://ca.zhonguo7118.cn

================================================================================
来源：https://yo.zhonguo5118.cn

[U01] Py：创建虚拟环境
来源：https://xd.zhonguo5118.cn

python -m venv .venv && source .venv/bin/activate
来源：https://eq.zhonguo8118.cn

[U02] Py：导出 / 安装依赖
来源：https://ly.zhonguo1118.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：https://xs.zhonguo1118.cn

[U03] Py：加载 .env 配置
来源：https://ka.zhonguo5118.cn

from dotenv import load_dotenv; load_dotenv()
来源：https://fo.zhonguo2118.cn

[U04] Py：变量调试打印
来源：https://wm.zhonguo6118.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：https://gw.zhonguo6118.cn

[U05] Py：列表去重且保序
来源：https://ta.zhonguo4118.cn

list(dict.fromkeys(arr))
来源：https://bl.zhonguo6118.cn

[U06] Py：合并两个字典
来源：https://ve.zhonguo5118.cn

{**a, **b}
来源：https://gj.zhonguo3118.cn

[U07] Py：反转字典键值
来源：https://vr.zhonguo1118.cn

{v: k for k, v in d.items()}
来源：https://vp.zhonguo4118.cn

[U08] Py：展平二维列表
来源：https://qj.zhonguo1118.cn

[y for x in nested for y in x]
来源：https://pi.zhonguo4118.cn

[U09] Py：字典取最大值的键
来源：https://ef.zhonguo4118.cn

max(d, key=d.get)
来源：https://yg.zhonguo2118.cn

[U10] Py：按值排序字典
来源：https://tc.zhonguo2118.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：https://tf.zhonguo8118.cn

[U11] Py：生成器表达式
来源：https://af.zhonguo1118.cn

(x * 2 for x in arr)
来源：https://ig.zhonguo7118.cn

[U12] Py：取出现最多的 3 个元素
来源：https://xf.zhonguo2118.cn

Counter(arr).most_common(3)
来源：https://bx.zhonguo7118.cn

[U13] Py：固定长度队列
来源：https://uj.zhonguo8118.cn

deque(maxlen=10)
来源：https://ht.zhonguo5118.cn

[U14] Py：分组收集到列表
来源：https://dq.zhonguo1118.cn

defaultdict(list)
来源：https://hb.zhonguo2118.cn

[U15] Py：高精度计时
来源：https://eu.zhonguo5118.cn

t = time.perf_counter()
来源：https://ze.zhonguo3118.cn

[U16] Py：命令行参数解析
来源：https://jx.zhonguo3118.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：https://ch.zhonguo8118.cn

[U17] Py：初始化日志
来源：https://qa.zhonguo4118.cn

logging.basicConfig(level=logging.INFO)
来源：https://na.zhonguo6118.cn

[U18] Py：预编译正则
来源：https://fb.zhonguo5118.cn

pat = re.compile(r"\d+")
来源：https://ur.zhonguo4118.cn

[U19] Py：正则替换带回调
来源：https://tv.zhonguo6118.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：https://qt.zhonguo4118.cn

[U20] Py：缓存函数结果
来源：https://nk.zhonguo5118.cn

@functools.lru_cache(maxsize=None)
来源：https://sb.zhonguo7118.cn

[U21] Py：自定义上下文管理器
来源：https://sf.zhonguo4118.cn

@contextlib.contextmanager
来源：https://bs.zhonguo3118.cn

[U22] Py：矩阵转置
来源：https://wr.zhonguo3118.cn

list(zip(*m))
来源：https://cs.zhonguo1118.cn

[U23] Py：分块读取大文件
来源：https://gp.zhonguo2118.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：https://xz.zhonguo5118.cn

[U24] Py：路径操作
来源：https://ew.zhonguo8118.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：https://ag.zhonguo4118.cn

[U25] Py：CSV 按字典读
来源：https://in.zhonguo7118.cn

csv.DictReader(f)
来源：https://sv.zhonguo5118.cn

[U26] Py：并发下载
来源：https://xh.zhonguo5118.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：https://ti.zhonguo1118.cn

[U27] Py：异步 HTTP
来源：https://mh.zhonguo7118.cn

aiohttp.ClientSession() 配合 async with
来源：https://ab.zhonguo5118.cn

[U28] Py：类型别名
来源：https://fl.zhonguo1118.cn

UserId = int
来源：https://mj.zhonguo8118.cn

[U29] Py：属性校验
来源：https://ow.zhonguo8118.cn

@property 与 @x.setter 配合
来源：https://dm.zhonguo4118.cn

[U30] Py：数据类
来源：https://lr.zhonguo8118.cn

@dataclass(slots=True)
来源：https://zj.zhonguo2118.cn

[U31] Py：单测
来源：https://nr.zhonguo4118.cn

python -m pytest -q
来源：https://dz.zhonguo3118.cn

[U32] Py：代码格式化
来源：https://ht.zhonguo1118.cn

ruff format . && ruff check --fix .
来源：https://yz.zhonguo2118.cn

[U33] Py：打包发布
来源：https://is.zhonguo1118.cn

python -m build  （依赖 pyproject.toml）
来源：https://jg.zhonguo3118.cn

[U34] Py：判断编码
来源：https://xm.zhonguo3118.cn

chardet.detect(raw)
来源：https://eu.zhonguo3118.cn

[U35] Py：发送邮件
来源：https://hp.zhonguo1118.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：https://sf.zhonguo7118.cn

[U36] Py：定时任务
来源：https://ls.zhonguo5118.cn

schedule.every(10).minutes.do(job)
来源：https://oz.zhonguo2118.cn

[U37] Py：读写 Excel
来源：https://wk.zhonguo2118.cn

pandas.read_excel / DataFrame.to_excel
来源：https://zt.zhonguo4118.cn

[U38] Py：获取脚本所在目录
来源：https://kq.zhonguo4118.cn

Path(__file__).resolve().parent
来源：https://rx.zhonguo4118.cn

[U39] Py：判断是否在交互环境
来源：https://gm.zhonguo5118.cn

sys.stdout.isatty()
来源：https://rj.zhonguo1118.cn

[U40] Py：打印到标准错误
来源：https://jq.zhonguo2118.cn

print("err", file=sys.stderr)
来源：https://sn.zhonguo8118.cn

[U41] PHP：初始化 Composer 项目
来源：https://bh.zhonguo6118.cn

composer init;  composer require guzzlehttp/guzzle
来源：https://ya.zhonguo4118.cn

[U42] PHP：PSR-4 自动加载
来源：https://ja.zhonguo6118.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：https://ki.zhonguo6118.cn

[U43] PHP：声明命名空间
来源：https://ov.zhonguo3118.cn

namespace App\Http;
来源：https://gg.zhonguo4118.cn

[U44] PHP：开启严格类型
来源：https://kl.zhonguo6118.cn

declare(strict_types=1);
来源：https://ma.zhonguo2118.cn

[U45] PHP：类型声明与返回类型
来源：https://wk.zhonguo2118.cn

function add(int $a, int $b): int { return $a + $b; }
来源：https://ja.zhonguo1118.cn

[U46] PHP：可空类型
来源：https://ey.zhonguo8118.cn

?string $name = null
来源：https://kg.zhonguo3118.cn

[U47] PHP：联合类型
来源：https://nj.zhonguo1118.cn

int|string $id
来源：https://lg.zhonguo4118.cn

[U48] PHP：纯枚举
来源：https://xo.zhonguo4118.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：https://lr.zhonguo7118.cn

[U49] PHP：只读属性
来源：https://su.zhonguo5118.cn

public readonly string $name
来源：https://sh.zhonguo1118.cn

[U50] PHP：构造器属性提升
来源：https://uu.zhonguo4118.cn

public function __construct(private int $id) {}
来源：https://ho.zhonguo3118.cn

[U51] PHP：数组解构
来源：https://dx.zhonguo6118.cn

[$a, $b] = $arr;
来源：https://zs.zhonguo8118.cn

[U52] PHP：箭头函数
来源：https://zk.zhonguo5118.cn

$double = fn($x) => $x * 2;
来源：https://uu.zhonguo1118.cn

[U53] PHP：空合并运算符
来源：https://nv.zhonguo1118.cn

$v = $a ?? $b ?? "default";
来源：https://ui.zhonguo5118.cn

[U54] PHP：空安全调用
来源：https://iv.zhonguo6118.cn

$obj?->method()
来源：https://pk.zhonguo5118.cn

[U55] PHP：match 表达式
来源：https://km.zhonguo7118.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：https://cn.zhonguo5118.cn

[U56] PHP：命名参数
来源：https://zi.zhonguo4118.cn

f(a: 1, b: 2)
来源：https://da.zhonguo3118.cn

[U57] PHP：字符串插值
来源：https://ah.zhonguo8118.cn

"值: {$a}"
来源：https://yl.zhonguo5118.cn

[U58] PHP：数组三件套
来源：https://xp.zhonguo5118.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：https://de.zhonguo3118.cn

[U59] PHP：自定义排序
来源：https://ua.zhonguo1118.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://nr.zhonguo5118.cn

[U60] PHP：JSON 编解码
来源：https://cl.zhonguo1118.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：https://mz.zhonguo6118.cn

[U61] PHP：正则
来源：https://fg.zhonguo6118.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：https://bg.zhonguo5118.cn

[U62] PHP：日期对象
来源：https://hy.zhonguo1118.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：https://dn.zhonguo4118.cn

[U63] PHP：文件读写
来源：https://am.zhonguo4118.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：https://up.zhonguo4118.cn

[U64] PHP：目录遍历
来源：https://lz.zhonguo7118.cn

glob("dir/*.php");  scandir("dir");
来源：https://qx.zhonguo8118.cn

[U65] PHP：会话
来源：https://nq.zhonguo7118.cn

session_start();  $_SESSION["uid"] = 1;
来源：https://rj.zhonguo6118.cn

[U66] PHP：设置 Cookie
来源：https://gc.zhonguo1118.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：https://wr.zhonguo1118.cn

[U67] PHP：处理文件上传
来源：https://as.zhonguo2118.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：https://rf.zhonguo1118.cn

[U68] PHP：PDO 连接
来源：https://yi.zhonguo8118.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：https://sl.zhonguo1118.cn

[U69] PHP：PDO 预处理
来源：https://gt.zhonguo6118.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：https://if.zhonguo5118.cn

[U70] PHP：PDO 事务
来源：https://rq.zhonguo6118.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：https://qn.zhonguo6118.cn

[U71] PHP：抛出异常
来源：https://rq.zhonguo8118.cn

throw new RuntimeException("失败", 500);
来源：https://gw.zhonguo4118.cn

[U72] PHP：写错误日志
来源：https://vi.zhonguo4118.cn

error_log("失败: " . $e->getMessage());
来源：https://ch.zhonguo3118.cn

[U73] PHP：读取 ini 配置
来源：https://hy.zhonguo1118.cn

parse_ini_file("config.ini", true)
来源：https://qy.zhonguo4118.cn

[U74] PHP：读取环境变量
来源：https://jd.zhonguo1118.cn

getenv("APP_ENV") ?: "production"
来源：https://ty.zhonguo3118.cn

[U75] PHP：依赖注入
来源：https://im.zhonguo1118.cn

composer require psr/container
来源：https://st.zhonguo7118.cn

[U76] PHP：简单路由
来源：https://bn.zhonguo3118.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：https://kw.zhonguo1118.cn

[U77] PHP：模板渲染
来源：https://wn.zhonguo4118.cn

composer require twig/twig
来源：https://lp.zhonguo5118.cn

[U78] PHP：单元测试
来源：https://zy.zhonguo3118.cn

composer require --dev phpunit/phpunit
来源：https://az.zhonguo6118.cn

[U79] PHP：静态分析
来源：https://bk.zhonguo1118.cn

composer require --dev phpstan/phpstan
来源：https://xf.zhonguo3118.cn

[U80] PHP：代码规范修复
来源：https://xe.zhonguo3118.cn

composer require --dev friendsofphp/php-cs-fixer
来源：https://fe.zhonguo8118.cn

[U81] JS：初始化项目
来源：https://xn.zhonguo4118.cn

npm init -y;  npm i express
来源：https://it.zhonguo3118.cn

[U82] JS：package.json 脚本
来源：https://dq.zhonguo2118.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：https://ks.zhonguo2118.cn

[U83] JS：ES Module 导入导出
来源：https://vp.zhonguo8118.cn

export const a = 1;  import { a } from "./m.js";
来源：https://ys.zhonguo8118.cn

[U84] JS：CommonJS 写法
来源：https://uf.zhonguo2118.cn

module.exports = { a };  const { a } = require("./m");
来源：https://xe.zhonguo5118.cn

[U85] JS：可选链
来源：https://wg.zhonguo1118.cn

a?.b?.c
来源：https://ko.zhonguo1118.cn

[U86] JS：空值合并
来源：https://nj.zhonguo6118.cn

a ?? b
来源：https://ie.zhonguo2118.cn

[U87] JS：解构默认值
来源：https://dn.zhonguo6118.cn

const { a = 1, b = 2 } = obj;
来源：https://ra.zhonguo3118.cn

[U88] JS：对象展开合并
来源：https://gt.zhonguo1118.cn

{ ...a, ...b }
来源：https://vo.zhonguo2118.cn

[U89] JS：数组去重
来源：https://wb.zhonguo5118.cn

[...new Set(arr)]
来源：https://tw.zhonguo3118.cn

[U90] JS：数字数组排序
来源：https://zu.zhonguo6118.cn

[...arr].sort((a, b) => a - b)
来源：https://dh.zhonguo8118.cn

[U91] JS：对象键值遍历
来源：https://tf.zhonguo6118.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：https://in.zhonguo3118.cn

[U92] JS：深拷贝
来源：https://su.zhonguo7118.cn

structuredClone(obj)
来源：https://lu.zhonguo4118.cn

[U93] JS：模板字符串
来源：https://vi.zhonguo2118.cn

`共 ${n} 条`
来源：https://bh.zhonguo4118.cn

[U94] JS：箭头函数
来源：https://bj.zhonguo3118.cn

const double = x => x * 2;
来源：https://pn.zhonguo7118.cn

[U95] JS：Promise 包装
来源：https://hd.zhonguo6118.cn

new Promise((resolve, reject) => {})
来源：https://xx.zhonguo6118.cn

[U96] JS：async/await 与异常
来源：https://pc.zhonguo5118.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：https://qt.zhonguo5118.cn

[U97] JS：并发请求
来源：https://yy.zhonguo4118.cn

await Promise.all(urls.map(u => fetch(u)))
来源：https://xq.zhonguo4118.cn

[U98] JS：fetch 带 JSON
来源：https://rc.zhonguo3118.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：https://lw.zhonguo3118.cn

[U99] JS：事件监听
来源：https://qz.zhonguo6118.cn

el.addEventListener("click", e => {})
来源：https://ud.zhonguo8118.cn

[U100] JS：DOM 查询
来源：https://yg.zhonguo6118.cn

document.querySelector(".item")
来源：https://hx.zhonguo8118.cn

[U101] JS：classList 操作
来源：https://eb.zhonguo8118.cn

el.classList.toggle("active")
来源：https://hx.zhonguo7118.cn

[U102] JS：本地存储
来源：https://oj.zhonguo6118.cn

localStorage.setItem("k", JSON.stringify(v))
来源：https://rd.zhonguo8118.cn

[U103] JS：定时器
来源：https://iq.zhonguo8118.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：https://jg.zhonguo4118.cn

[U104] JS：防抖
来源：https://sj.zhonguo7118.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：https://zx.zhonguo1118.cn

[U105] JS：节流
来源：https://ef.zhonguo6118.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：https://lu.zhonguo1118.cn

[U106] JS：日期格式化
来源：https://qk.zhonguo2118.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：https://ez.zhonguo1118.cn

[U107] JS：数字千分位
来源：https://ok.zhonguo2118.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：https://gj.zhonguo2118.cn

[U108] JS：随机整数
来源：https://sr.zhonguo1118.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：https://te.zhonguo2118.cn

[U109] JS：数组分组
来源：https://zs.zhonguo5118.cn

Object.groupBy(arr, x => x.type)
来源：https://ic.zhonguo1118.cn

[U110] JS：数组分块
来源：https://fj.zhonguo1118.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：https://ps.zhonguo2118.cn

[U111] JS：对象转 Map
来源：https://kl.zhonguo5118.cn

new Map(Object.entries(obj))
来源：https://kp.zhonguo7118.cn

[U112] JS：字符串补位
来源：https://rl.zhonguo4118.cn

"7".padStart(3, "0")
来源：https://fm.zhonguo2118.cn

[U113] JS：正则替换全部
来源：https://ox.zhonguo2118.cn

s.replaceAll("a", "b")
来源：https://hr.zhonguo6118.cn

[U114] JS：JSON 深比较
来源：https://id.zhonguo2118.cn

JSON.stringify(a) === JSON.stringify(b)
来源：https://on.zhonguo2118.cn

[U115] JS：生成 UUID
来源：https://yn.zhonguo6118.cn

crypto.randomUUID()
来源：https://vh.zhonguo5118.cn

[U116] JS：类型检查（JSDoc）
来源：https://mr.zhonguo6118.cn

/** @param {string} name */ function f(name) {}
来源：https://yt.zhonguo6118.cn

[U117] JS：单元测试
来源：https://pd.zhonguo3118.cn

npm i -D vitest;  npx vitest
来源：https://bf.zhonguo1118.cn

[U118] JS：开发服务器
来源：https://ms.zhonguo2118.cn

npm i -D vite;  npx vite
来源：https://fk.zhonguo2118.cn

[U119] JS：生产构建
来源：https://sy.zhonguo1118.cn

npx vite build
来源：https://dv.zhonguo8118.cn

[U120] JS：读取环境变量（Vite）
来源：https://fd.zhonguo5118.cn

import.meta.env.VITE_API_URL
来源：https://iw.zhonguo7118.cn

================================================================================
来源：https://mc.zhonguo3118.cn

统计汇总
来源：https://om.zhonguo8118.cn

================================================================================
来源：https://al.zhonguo4118.cn

按语言统计（条）：
来源：https://ns.zhonguo5118.cn

Python ......... 252
来源：https://sc.zhonguo5118.cn

PHP ............ 252
来源：https://gm.zhonguo8118.cn

JavaScript ..... 252
来源：https://pg.zhonguo3118.cn

TypeScript ..... 212
来源：https://rl.zhonguo7118.cn

Java ........... 212
来源：https://gg.zhonguo6118.cn

Go ............. 212
来源：https://lu.zhonguo3118.cn

Ruby ........... 212
来源：https://zi.zhonguo2118.cn

C# ............. 212
来源：https://jl.zhonguo6118.cn

C .............. 30
来源：https://yl.zhonguo1118.cn

C++ ............ 30
来源：https://ga.zhonguo8118.cn

SQL ............ 90
来源：https://hz.zhonguo7118.cn

Bash ........... 80
来源：https://ly.zhonguo6118.cn

Kotlin ......... 15
来源：https://xx.zhonguo4118.cn

Swift .......... 15
来源：https://ff.zhonguo5118.cn

Lua ............ 10
来源：https://hw.zhonguo4118.cn

Perl ........... 10
来源：https://xt.zhonguo8118.cn

Scala .......... 10
来源：https://qp.zhonguo7118.cn

------------------------------------
来源：https://nu.zhonguo7118.cn

合计 ........... 2106 条
来源：https://og.zhonguo6118.cn

按章节统计：
来源：https://ko.zhonguo6118.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：https://jx.zhonguo2118.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：https://kp.zhonguo8118.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：https://ny.zhonguo8118.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：https://qd.zhonguo8118.cn


<!-- 参考信息 -->