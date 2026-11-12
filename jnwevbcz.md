代发 wailian999

[U17] Py：初始化日志
来源：http://kvr.yj20258888.top

logging.basicConfig(level=logging.INFO)
来源：http://nzc.shuidangran.top

[U18] Py：预编译正则
来源：http://rgh.cheryme.top

pat = re.compile(r"\d+")
来源：http://gyw.cdnleiting.top

[U19] Py：正则替换带回调
来源：http://uab.jqgufenzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mzk.jqgufenzy.top

[U20] Py：缓存函数结果
来源：http://ksv.hongshengwenyu.top

@functools.lru_cache(maxsize=None)
来源：http://yms.xuanzx.com

[U21] Py：自定义上下文管理器
来源：http://tve.guannengcc.top

@contextlib.contextmanager
来源：http://jvo.wangshuangyany.cn

[U22] Py：矩阵转置
来源：http://kbj.feifeiyinyue.top

list(zip(*m))
来源：http://lev.quarkkingdee.top

[U23] Py：分块读取大文件
来源：http://zur.epnwcf.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://asu.fzhhl.top

[U24] Py：路径操作
来源：http://mje.yj20258888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kpv.zhijiandao.cn

[U25] Py：CSV 按字典读
来源：http://inf.chenjidiqi.icu

csv.DictReader(f)
来源：http://ndj.uphjek.com

[U26] Py：并发下载
来源：http://pcu.xinyue.icu

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rth.yueranfly.top

[U27] Py：异步 HTTP
来源：http://dip.cqqwz.cn

aiohttp.ClientSession() 配合 async with
来源：http://yoo.jqgfzy.top

[U28] Py：类型别名
来源：http://jgm.vqdsnc.cn

UserId = int
来源：http://ytt.bjfxy.top

[U29] Py：属性校验
来源：http://czr.shanyushiyangtech.top

@property 与 @x.setter 配合
来源：http://yka.sxryk.cn

[U30] Py：数据类
来源：http://jyl.yuxming.cn

@dataclass(slots=True)
来源：http://xko.yanxiufei.cn

[U31] Py：单测
来源：http://rkx.yongpay.top

python -m pytest -q
来源：http://mpw.bbcook.cn

[U32] Py：代码格式化
来源：http://tqc.dashuyun.cn

ruff format . && ruff check --fix .
来源：http://ign.shanyushiyangtech.top

[U33] Py：打包发布
来源：http://jet.yuxming.cn

python -m build  （依赖 pyproject.toml）
来源：http://wtg.zhiwuduotai.top

[U34] Py：判断编码
来源：http://ptb.tian-w.cn

chardet.detect(raw)
来源：http://vxy.smart0.xyz

[U35] Py：发送邮件
来源：http://ytw.fengsongda.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qwd.fzhhl.top

[U36] Py：定时任务
来源：http://pzx.fehbvm.com

schedule.every(10).minutes.do(job)
来源：http://lxo.andypj.xyz

[U37] Py：读写 Excel
来源：http://tgf.ybcxt.top

pandas.read_excel / DataFrame.to_excel
来源：http://sbj.uphjek.com

[U38] Py：获取脚本所在目录
来源：http://qdj.c1oappe.top

Path(__file__).resolve().parent
来源：http://vtu.gaohongyu789.top

[U39] Py：判断是否在交互环境
来源：http://dda.fehbvm.com

sys.stdout.isatty()
来源：http://ywz.hammf.cn

[U40] Py：打印到标准错误
来源：http://mvu.cucudq.cn

print("err", file=sys.stderr)
来源：http://mcu.jianghu66.top

[U41] PHP：初始化 Composer 项目
来源：http://ycd.birdmap.top

composer init;  composer require guzzlehttp/guzzle
来源：http://hfo.ydjk.org.cn

[U42] PHP：PSR-4 自动加载
来源：http://aws.yongpay.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rmb.yvedp.cn

[U43] PHP：声明命名空间
来源：http://set.dianchejie.cn

namespace App\Http;
来源：http://eek.ivvv.top

[U44] PHP：开启严格类型
来源：http://bbx.fanxiaobao.xyz

declare(strict_types=1);
来源：http://pba.chenjidiqi.icu

[U45] PHP：类型声明与返回类型
来源：http://cxm.zhengqikj.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jee.hammf.cn

[U46] PHP：可空类型
来源：http://bpl.chenlongwang.top

?string $name = null
来源：http://xlm.guannengcc.top

[U47] PHP：联合类型
来源：http://blw.tarul.cn

int|string $id
来源：http://yie.jinghuilouyu.cn

[U48] PHP：纯枚举
来源：http://stv.xuanzx.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vww.ydjk.org.cn

[U49] PHP：只读属性
来源：http://wjx.zdbjq.cn

public readonly string $name
来源：http://mwj.fanxiaobao.xyz

[U50] PHP：构造器属性提升
来源：http://qxp.jlsjyb.cn

public function __construct(private int $id) {}
来源：http://bnx.fanxiaobao.xyz

[U51] PHP：数组解构
来源：http://ecj.cucudq.cn

[$a, $b] = $arr;
来源：http://jhp.yuanzhike.top

[U52] PHP：箭头函数
来源：http://xwc.jinghuilouyu.cn

$double = fn($x) => $x * 2;
来源：http://cme.yj20258.top

[U53] PHP：空合并运算符
来源：http://mfs.zdqjudy.top

$v = $a ?? $b ?? "default";
来源：http://azp.gogol.net.cn

[U54] PHP：空安全调用
来源：http://fib.shanyushiyangkeji.top

$obj?->method()
来源：http://wji.cheryme.top

[U55] PHP：match 表达式
来源：http://lev.uphjek.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lvz.uphjek.com

[U56] PHP：命名参数
来源：http://wxh.hongshengwenyu.top

f(a: 1, b: 2)
来源：http://tdi.nwbrower.top

[U57] PHP：字符串插值
来源：http://cnu.andypj.xyz

"值: {$a}"
来源：http://qeo.cqqwz.cn

[U58] PHP：数组三件套
来源：http://gce.jinqigfzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://oxi.hnxiangtu.top

[U59] PHP：自定义排序
来源：http://xud.guannengcc.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bzs.tianlin.xyz

[U60] PHP：JSON 编解码
来源：http://fbs.yj20258.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zlq.tian-w.cn

[U61] PHP：正则
来源：http://lia.9152youxi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://szq.jinqigfzy.top

[U62] PHP：日期对象
来源：http://uwb.ivvv.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kuk.guannengcc.top

[U63] PHP：文件读写
来源：http://dig.zycfv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fat.yuanzhike.top

[U64] PHP：目录遍历
来源：http://myw.cdnleiting.top

glob("dir/*.php");  scandir("dir");
来源：http://nmf.fktsv.cn

[U65] PHP：会话
来源：http://opz.tian-w.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rtt.nanxuanxn.top

[U66] PHP：设置 Cookie
来源：http://gma.vqdsnc.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eap.redwolf501.top

[U67] PHP：处理文件上传
来源：http://pzp.sjlbkw.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dpv.snrcjt.cn

[U68] PHP：PDO 连接
来源：http://wan.jqgufenzy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zsk.tian-w.cn

[U69] PHP：PDO 预处理
来源：http://alr.jlsjyb.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qdi.pengpengdd.cyou

[U70] PHP：PDO 事务
来源：http://neh.0kj1m.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wpw.andypj.xyz

[U71] PHP：抛出异常
来源：http://rou.dianchejie.cn

throw new RuntimeException("失败", 500);
来源：http://xzs.guowangkeji.top

[U72] PHP：写错误日志
来源：http://zmt.zdbjq.cn

error_log("失败: " . $e->getMessage());
来源：http://qys.xinyue.icu

[U73] PHP：读取 ini 配置
来源：http://ogl.hnqzz.top

parse_ini_file("config.ini", true)
来源：http://qnq.sxryk.cn

[U74] PHP：读取环境变量
来源：http://dlc.shanyushiyangtech.top

getenv("APP_ENV") ?: "production"
来源：http://vmb.yangfankeji.com

[U75] PHP：依赖注入
来源：http://lve.hammf.cn

composer require psr/container
来源：http://vyu.yfazqb.com

[U76] PHP：简单路由
来源：http://bjt.fehbvm.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sjr.kuanghao11.cn

[U77] PHP：模板渲染
来源：http://wsx.jiagoushi.top

composer require twig/twig
来源：http://zkq.jinqigufen.top

[U78] PHP：单元测试
来源：http://mqg.fengsongda.top

composer require --dev phpunit/phpunit
来源：http://yvf.hnxiangtu.top

[U79] PHP：静态分析
来源：http://dzr.shzxlz.cn

composer require --dev phpstan/phpstan
来源：http://snj.ywan-chungtsiang.top

[U80] PHP：代码规范修复
来源：http://ojh.yj202588.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://kkd.316326.xyz

[U81] JS：初始化项目
来源：http://jqk.0kj1m.cn

npm init -y;  npm i express
来源：http://tkz.cqqwz.cn

[U82] JS：package.json 脚本
来源：http://rap.xinyue.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ytu.tianlin.xyz

[U83] JS：ES Module 导入导出
来源：http://htn.yuxming.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qkd.jlsjyb.cn

[U84] JS：CommonJS 写法
来源：http://rte.zhiwuduotai.top

module.exports = { a };  const { a } = require("./m");
来源：http://wui.fengsongda.top

[U85] JS：可选链
来源：http://mpf.shzxlz.cn

a?.b?.c
来源：http://hoe.zhengqikj.top

[U86] JS：空值合并
来源：http://kjs.ydjk.org.cn

a ?? b
来源：http://zia.xuetiantiany.cn

[U87] JS：解构默认值
来源：http://han.fengsongda.top

const { a = 1, b = 2 } = obj;
来源：http://vtd.wangshuangyany.cn

[U88] JS：对象展开合并
来源：http://ftu.sjlbkw.cn

{ ...a, ...b }
来源：http://qno.hfpthk.cn

[U89] JS：数组去重
来源：http://rsy.gaohongyu789.top

[...new Set(arr)]
来源：http://zqh.c1oappe.top

[U90] JS：数字数组排序
来源：http://nlj.hnqzz.top

[...arr].sort((a, b) => a - b)
来源：http://jjz.gaohongyu789.top

[U91] JS：对象键值遍历
来源：http://flj.mhx1999.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nku.nanxinkj.top

[U92] JS：深拷贝
来源：http://bxm.bjfxy.top

structuredClone(obj)
来源：http://aeq.zhengqikj.top

[U93] JS：模板字符串
来源：http://mtv.zhongyouzk.top

`共 ${n} 条`
来源：http://stl.bbcook.cn

[U94] JS：箭头函数
来源：http://fon.0kj1m.cn

const double = x => x * 2;
来源：http://qdf.chenjidiqi.icu

[U95] JS：Promise 包装
来源：http://flh.zhoulong.xyz

new Promise((resolve, reject) => {})
来源：http://ybm.bbcook.cn

[U96] JS：async/await 与异常
来源：http://zpt.hesvh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sou.wangshuangyany.cn

[U97] JS：并发请求
来源：http://msx.sweek.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://hcu.zhaomingkeji.xyz

[U98] JS：fetch 带 JSON
来源：http://fex.bjfxy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zba.iojbl.cn

[U99] JS：事件监听
来源：http://iwp.bbcook.cn

el.addEventListener("click", e => {})
来源：http://aou.cqqwz.cn

[U100] JS：DOM 查询
来源：http://buu.yongpay.top

document.querySelector(".item")
来源：http://fgn.jqgfzy.top

[U101] JS：classList 操作
来源：http://int.fktsv.cn

el.classList.toggle("active")
来源：http://afk.shanyushiyangkeji.top

[U102] JS：本地存储
来源：http://gpu.epnwcf.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://dzv.guannengcc.top

[U103] JS：定时器
来源：http://vto.yuanzhike.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://apt.tarul.cn

[U104] JS：防抖
来源：http://tyd.fengsongda.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nyf.haohaochexian.top

[U105] JS：节流
来源：http://lzs.chenjidiqi.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://agl.wangdashe.top

[U106] JS：日期格式化
来源：http://xlr.xylfe.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hjd.yongpay.top

[U107] JS：数字千分位
来源：http://lyo.shanyushiyangkeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nje.xuanzx.com

[U108] JS：随机整数
来源：http://pqe.shanyushiyangtech.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rbq.jiagoushi.top

[U109] JS：数组分组
来源：http://skp.sufxvd.cn

Object.groupBy(arr, x => x.type)
来源：http://cbi.0kj1m.cn

[U110] JS：数组分块
来源：http://dsr.dashuyun.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mtb.xingfuxueyuan.xyz

[U111] JS：对象转 Map
来源：http://rlr.c1oappe.top

new Map(Object.entries(obj))
来源：http://ojh.zhijiandao.cn

[U112] JS：字符串补位
来源：http://nmq.smart0.xyz

"7".padStart(3, "0")
来源：http://rlm.ctjpmb.com

[U113] JS：正则替换全部
来源：http://tjx.yfazqb.com

s.replaceAll("a", "b")
来源：http://act.fzhhl.top

[U114] JS：JSON 深比较
来源：http://ijj.cdnleiting.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://agb.ivvv.top

[U115] JS：生成 UUID
来源：http://icr.yueranfly.top

crypto.randomUUID()
来源：http://kkp.jinqigufen.top

[U116] JS：类型检查（JSDoc）
来源：http://uki.jinqigufen.top

/** @param {string} name */ function f(name) {}
来源：http://mql.yvedp.cn

[U117] JS：单元测试
来源：http://pgj.gotoacloud.top

npm i -D vitest;  npx vitest
来源：http://wjb.gaohongyu789.top

[U118] JS：开发服务器
来源：http://ota.xziqi.cn

npm i -D vite;  npx vite
来源：http://ocn.hongshengwenyu.top

[U119] JS：生产构建
来源：http://spo.feifeiyinyue.top

npx vite build
来源：http://smm.shangyingyoupin.top

[U120] JS：读取环境变量（Vite）
来源：http://szc.hnqzz.top

import.meta.env.VITE_API_URL
来源：http://qen.gzhubu.top

================================================================================
来源：http://obu.nanxuanxn.top

统计汇总
来源：http://nuz.shangyingyoupin.top

================================================================================
来源：http://sqt.dashuyun.cn

按语言统计（条）：
来源：http://pcr.sysykeji.top

Python ......... 252
来源：http://sqj.hongshengwenyu.top

PHP ............ 252
来源：http://uea.hnxiangtu.top

JavaScript ..... 252
来源：http://viw.yuxming.cn

TypeScript ..... 212
来源：http://mve.yuxming.cn

Java ........... 212
来源：http://qlx.cqqwz.cn

Go ............. 212
来源：http://nqu.gogol.net.cn

Ruby ........... 212
来源：http://tot.xuanzx.com

C# ............. 212
来源：http://pfc.ppjwa.cn

C .............. 30
来源：http://vda.ehwqpu.com

C++ ............ 30
来源：http://ihp.yvedp.cn

SQL ............ 90
来源：http://npd.zhixingplan.top

Bash ........... 80
来源：http://bwp.pengpengdd.cyou

Kotlin ......... 15
来源：http://hkm.wangdashe.top

Swift .......... 15
来源：http://xty.daxiang520.top

Lua ............ 10
来源：http://emb.ybcxt.top

Perl ........... 10
来源：http://ian.uphjek.com

Scala .......... 10
来源：http://fjk.hysaishi.cn

------------------------------------
来源：http://zkm.zhoulong.xyz

合计 ........... 2106 条
来源：http://ypn.tian-w.cn

按章节统计：
来源：http://bjy.hywenlv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ark.xuanzx.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ufv.daxiang520.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://teo.yanxiufei.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dvg.zhongyouzk.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rfs.zycfv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://oqe.dianchejie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://npt.xylfe.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wdb.zhiwuduotai.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://anr.jyoumei.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ruz.vqdsnc.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lzq.9152youxi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nut.0kj1m.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://usd.chenlongwang.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rcd.guannengcc.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jdk.kuanghao11.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://twt.ppjwa.cn

Q SQL 专题                              90
来源：http://ioj.epnwcf.com

R Bash 专题                             80
来源：http://kmi.gogol.net.cn

S C / C++ 专题                          60
来源：http://bnb.andypj.xyz

T 其他语言补充                          60
来源：http://weu.shangyingyoupin.top

U 高频实用片段                         120
来源：http://kca.cheryme.top

------------------------------------
来源：http://qer.fktsv.cn

合计                                  2106 条
来源：http://qvl.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://bfo.xziqi.cn

使用提醒
来源：http://hco.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://hig.ydjk.org.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ubr.dashuyun.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yws.dashuyun.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://awh.zdbjq.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vgz.hywenlv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://myq.iojbl.cn

—— 文件结束 ——
来源：http://kcq.fehbvm.com

================================================================================
来源：http://eag.yuxming.cn

程序语言常见例子速查手册（2024 版）
来源：http://kal.meibo888.top

Common Programming Examples Cheat Book
来源：http://hjl.c1oappe.top

================================================================================
来源：http://nyc.xziqi.cn

【收录内容】
来源：http://zpx.fktsv.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://uxo.shuidangran.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lwj.gotoacloud.top

SQL · Bash · C · C++
来源：http://vhu.zhaomingkeji.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pqo.jiagoushi.top

【使用说明】
来源：http://jwj.cashguo.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ygs.jinghuilouyu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nod.jyoumei.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iht.ppjwa.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://suw.c1oappe.top

Bash:  Shell         C:     C             C++:   C++
来源：http://jow.pengpengdd.cyou

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vtn.sxryk.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rcy.zhixingplan.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qxg.shanyushiyangkeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://whg.hongshengwenyu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vpo.guannengcc.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bni.meibo888.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mce.guowangkeji.top

【文件统计】
来源：http://qef.yangfankeji.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ykt.yuxming.cn

--------------------------------------------------------------------------------
来源：http://ias.yueranfly.top

目  录
来源：http://ebi.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://rzc.uphjek.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://txo.ctjpmb.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://oxc.daria6918.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cqz.yvedp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hdw.sweek.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://aeq.hnxiangtu.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bsx.ehwqpu.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://szf.52xcode.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zxl.yvedp.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uvl.yj20258888.top


<!-- 参考信息 -->