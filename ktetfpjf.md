代发 wailian999

[U19] Py：正则替换带回调
来源：http://bot.yvedp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kgc.shzxlz.cn

[U20] Py：缓存函数结果
来源：http://agw.gotoacloud.top

@functools.lru_cache(maxsize=None)
来源：http://tmx.cqqwz.cn

[U21] Py：自定义上下文管理器
来源：http://twc.gaohongyu789.top

@contextlib.contextmanager
来源：http://jez.ydzc1.top

[U22] Py：矩阵转置
来源：http://ibx.zhoulong.xyz

list(zip(*m))
来源：http://sjn.xingfuxueyuan.xyz

[U23] Py：分块读取大文件
来源：http://fxx.iojbl.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wyo.tianlin.xyz

[U24] Py：路径操作
来源：http://ojp.guowangkeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://urp.guowangkeji.top

[U25] Py：CSV 按字典读
来源：http://gnp.fanxiaobao.xyz

csv.DictReader(f)
来源：http://frk.shanyushiyangtech.top

[U26] Py：并发下载
来源：http://qlj.nanxinkj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fgr.zdbjq.cn

[U27] Py：异步 HTTP
来源：http://vik.bbcook.cn

aiohttp.ClientSession() 配合 async with
来源：http://vlc.sxryk.cn

[U28] Py：类型别名
来源：http://mqr.zhongyouzk.top

UserId = int
来源：http://bls.sweek.top

[U29] Py：属性校验
来源：http://orp.gogol.net.cn

@property 与 @x.setter 配合
来源：http://lzy.kuanghao11.cn

[U30] Py：数据类
来源：http://sze.yfazqb.com

@dataclass(slots=True)
来源：http://cuj.pycfn.com

[U31] Py：单测
来源：http://zld.guannengcc.top

python -m pytest -q
来源：http://mfh.hongshengwenyu.top

[U32] Py：代码格式化
来源：http://zin.jinqigfzy.top

ruff format . && ruff check --fix .
来源：http://etz.nanxinkj.top

[U33] Py：打包发布
来源：http://edu.hysaishi.cn

python -m build  （依赖 pyproject.toml）
来源：http://fct.ywan-chungtsiang.top

[U34] Py：判断编码
来源：http://ein.fanxiaobao.xyz

chardet.detect(raw)
来源：http://ztk.gotoacloud.top

[U35] Py：发送邮件
来源：http://dld.gzhubu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hyw.jqgufenzy.top

[U36] Py：定时任务
来源：http://udr.sjlbkw.cn

schedule.every(10).minutes.do(job)
来源：http://vbf.jinghuilouyu.cn

[U37] Py：读写 Excel
来源：http://sqb.aizwys.cn

pandas.read_excel / DataFrame.to_excel
来源：http://aet.ywan-chungtsiang.top

[U38] Py：获取脚本所在目录
来源：http://ojx.cashguo.top

Path(__file__).resolve().parent
来源：http://fjm.ehwqpu.com

[U39] Py：判断是否在交互环境
来源：http://paf.cheryme.top

sys.stdout.isatty()
来源：http://wbl.dashuyun.cn

[U40] Py：打印到标准错误
来源：http://ztv.gotoacloud.top

print("err", file=sys.stderr)
来源：http://knt.zhixingplan.top

[U41] PHP：初始化 Composer 项目
来源：http://inq.jyoumei.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dsn.jiagoushi.top

[U42] PHP：PSR-4 自动加载
来源：http://sce.xylfe.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bxq.daria6918.cn

[U43] PHP：声明命名空间
来源：http://viw.shangyingyoupin.top

namespace App\Http;
来源：http://voq.ydjk.org.cn

[U44] PHP：开启严格类型
来源：http://ezx.gotoacloud.top

declare(strict_types=1);
来源：http://rqr.yfazqb.com

[U45] PHP：类型声明与返回类型
来源：http://wne.tanke756.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://gzu.vqdsnc.cn

[U46] PHP：可空类型
来源：http://qie.zhongyouzk.top

?string $name = null
来源：http://rwe.gogol.net.cn

[U47] PHP：联合类型
来源：http://ugg.epnwcf.com

int|string $id
来源：http://ibt.sxryk.cn

[U48] PHP：纯枚举
来源：http://dbm.daria6918.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kdu.hcnkem.com

[U49] PHP：只读属性
来源：http://zqt.aizwys.cn

public readonly string $name
来源：http://nen.ppjwa.cn

[U50] PHP：构造器属性提升
来源：http://hva.shanyushiyangkeji.top

public function __construct(private int $id) {}
来源：http://swj.meibo888.top

[U51] PHP：数组解构
来源：http://qdy.jiagoushi.top

[$a, $b] = $arr;
来源：http://zng.chenjidiqi.icu

[U52] PHP：箭头函数
来源：http://foo.hfpthk.cn

$double = fn($x) => $x * 2;
来源：http://ggx.xuanzx.com

[U53] PHP：空合并运算符
来源：http://byt.jqgufenzy.top

$v = $a ?? $b ?? "default";
来源：http://aof.fehbvm.com

[U54] PHP：空安全调用
来源：http://yei.guowangkeji.top

$obj?->method()
来源：http://ovm.ydjk.org.cn

[U55] PHP：match 表达式
来源：http://iem.9152youxi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ggc.yfazqb.com

[U56] PHP：命名参数
来源：http://hcr.xylfe.cn

f(a: 1, b: 2)
来源：http://uif.zhijiandao.cn

[U57] PHP：字符串插值
来源：http://wdw.kuanghao11.cn

"值: {$a}"
来源：http://pmb.shanyushiyangkeji.top

[U58] PHP：数组三件套
来源：http://nzz.svipenyu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://soe.smart0.xyz

[U59] PHP：自定义排序
来源：http://ptd.fzhhl.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tvc.vqdsnc.cn

[U60] PHP：JSON 编解码
来源：http://nyd.yongpay.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ute.yuxming.cn

[U61] PHP：正则
来源：http://afm.tianlin.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nfi.tianlin.xyz

[U62] PHP：日期对象
来源：http://gzn.gzhubu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cxg.ctjpmb.com

[U63] PHP：文件读写
来源：http://fpj.hywenlv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cad.ydjk.org.cn

[U64] PHP：目录遍历
来源：http://gxp.hfpthk.cn

glob("dir/*.php");  scandir("dir");
来源：http://jxw.ehwqpu.com

[U65] PHP：会话
来源：http://clz.hywenlv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nzi.smart0.xyz

[U66] PHP：设置 Cookie
来源：http://ono.nwbrower.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://typ.vehdjk.com

[U67] PHP：处理文件上传
来源：http://zfs.vehdjk.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fvz.yvedp.cn

[U68] PHP：PDO 连接
来源：http://zot.yvedp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nnp.yongpay.top

[U69] PHP：PDO 预处理
来源：http://wle.nanxuanxn.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fuh.tarul.cn

[U70] PHP：PDO 事务
来源：http://nhg.feifeiyinyue.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jiw.nanxuanxn.top

[U71] PHP：抛出异常
来源：http://gqu.yvedp.cn

throw new RuntimeException("失败", 500);
来源：http://qae.yonumen.top

[U72] PHP：写错误日志
来源：http://hza.hnqzz.top

error_log("失败: " . $e->getMessage());
来源：http://mmo.feifeiyinyue.top

[U73] PHP：读取 ini 配置
来源：http://gpi.zhongyouzk.top

parse_ini_file("config.ini", true)
来源：http://xoz.zycfv.cn

[U74] PHP：读取环境变量
来源：http://hpr.hammf.cn

getenv("APP_ENV") ?: "production"
来源：http://zmj.hongshengwenyu.top

[U75] PHP：依赖注入
来源：http://rse.hysaishi.cn

composer require psr/container
来源：http://amu.gzhubu.top

[U76] PHP：简单路由
来源：http://voh.jinqigufen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mmj.yfazqb.com

[U77] PHP：模板渲染
来源：http://ots.pycfn.com

composer require twig/twig
来源：http://nty.tian-w.cn

[U78] PHP：单元测试
来源：http://dvz.iojbl.cn

composer require --dev phpunit/phpunit
来源：http://pdf.sufxvd.cn

[U79] PHP：静态分析
来源：http://gck.yj20258888.top

composer require --dev phpstan/phpstan
来源：http://jnr.guannengcc.top

[U80] PHP：代码规范修复
来源：http://oal.hywenlv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ylf.nanxinkj.top

[U81] JS：初始化项目
来源：http://aha.hnqzz.top

npm init -y;  npm i express
来源：http://sck.ppjwa.cn

[U82] JS：package.json 脚本
来源：http://ymd.feifeiyinyue.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lbk.ppjwa.cn

[U83] JS：ES Module 导入导出
来源：http://uqj.feifeiyinyue.top

export const a = 1;  import { a } from "./m.js";
来源：http://nra.redwolf501.top

[U84] JS：CommonJS 写法
来源：http://per.cqqwz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fbl.feifeiyinyue.top

[U85] JS：可选链
来源：http://hjf.52xcode.cn

a?.b?.c
来源：http://gou.jinyuanbaomall.cn

[U86] JS：空值合并
来源：http://qqo.vehdjk.com

a ?? b
来源：http://kle.yj202588.top

[U87] JS：解构默认值
来源：http://hdb.pengpengdd.cyou

const { a = 1, b = 2 } = obj;
来源：http://mpm.pycfn.com

[U88] JS：对象展开合并
来源：http://xkq.birdmap.top

{ ...a, ...b }
来源：http://vdi.cucudq.cn

[U89] JS：数组去重
来源：http://ize.cqqwz.cn

[...new Set(arr)]
来源：http://czo.jinqigufen.top

[U90] JS：数字数组排序
来源：http://mfq.fehbvm.com

[...arr].sort((a, b) => a - b)
来源：http://psz.shanyushiyangkeji.top

[U91] JS：对象键值遍历
来源：http://dkv.0kj1m.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://urt.ivvv.top

[U92] JS：深拷贝
来源：http://eqy.52xcode.cn

structuredClone(obj)
来源：http://ofj.birdmap.top

[U93] JS：模板字符串
来源：http://dhg.yvedp.cn

`共 ${n} 条`
来源：http://wrr.sxryk.cn

[U94] JS：箭头函数
来源：http://fml.fktsv.cn

const double = x => x * 2;
来源：http://bmg.aizwys.cn

[U95] JS：Promise 包装
来源：http://qbx.yangfankeji.com

new Promise((resolve, reject) => {})
来源：http://tdr.pengpengdd.cyou

[U96] JS：async/await 与异常
来源：http://gje.jiagoushi.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kqx.feifeiyinyue.top

[U97] JS：并发请求
来源：http://jlg.redwolf501.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kag.chenjidiqi.icu

[U98] JS：fetch 带 JSON
来源：http://orc.gogol.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kgx.feifeiyinyue.top

[U99] JS：事件监听
来源：http://tas.wangdashe.top

el.addEventListener("click", e => {})
来源：http://rmt.9152youxi.cn

[U100] JS：DOM 查询
来源：http://jqj.snrcjt.cn

document.querySelector(".item")
来源：http://ypi.gotoacloud.top

[U101] JS：classList 操作
来源：http://nnt.meibo888.top

el.classList.toggle("active")
来源：http://cbc.zhongyouzk.top

[U102] JS：本地存储
来源：http://tzw.yj20258888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://whw.xuanzx.com

[U103] JS：定时器
来源：http://qjb.guannengcc.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lth.xylfe.cn

[U104] JS：防抖
来源：http://tlp.chenjidiqi.icu

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://osv.zdbjq.cn

[U105] JS：节流
来源：http://suy.dianchejie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://upv.fehbvm.com

[U106] JS：日期格式化
来源：http://ktt.nanxuanxn.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dxy.jiagoushi.top

[U107] JS：数字千分位
来源：http://zhx.jiagoushi.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ltr.yuxming.cn

[U108] JS：随机整数
来源：http://mvh.havefunace.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ihz.zycfv.cn

[U109] JS：数组分组
来源：http://pnz.hongshengwenyu.top

Object.groupBy(arr, x => x.type)
来源：http://jgn.feifeiyinyue.top

[U110] JS：数组分块
来源：http://qvl.fengsongda.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oru.daxiang520.top

[U111] JS：对象转 Map
来源：http://zyr.svipenyu.cn

new Map(Object.entries(obj))
来源：http://fsy.smart0.xyz

[U112] JS：字符串补位
来源：http://puf.yonumen.top

"7".padStart(3, "0")
来源：http://kdg.ivvv.top

[U113] JS：正则替换全部
来源：http://zmq.jyoumei.cn

s.replaceAll("a", "b")
来源：http://sdk.yueranfly.top

[U114] JS：JSON 深比较
来源：http://vfk.jianghu66.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://yje.dashuyun.cn

[U115] JS：生成 UUID
来源：http://nwa.gotoacloud.top

crypto.randomUUID()
来源：http://uum.zhijiandao.cn

[U116] JS：类型检查（JSDoc）
来源：http://bwi.ydzc1.top

/** @param {string} name */ function f(name) {}
来源：http://hyp.smart0.xyz

[U117] JS：单元测试
来源：http://ijv.jinghuilouyu.cn

npm i -D vitest;  npx vitest
来源：http://bqc.hammf.cn

[U118] JS：开发服务器
来源：http://hwm.svipenyu.cn

npm i -D vite;  npx vite
来源：http://mxw.hongshengwenyu.top

[U119] JS：生产构建
来源：http://oky.shzxlz.cn

npx vite build
来源：http://urf.svipenyu.cn

[U120] JS：读取环境变量（Vite）
来源：http://det.haohaochexian.top

import.meta.env.VITE_API_URL
来源：http://bnc.svipenyu.cn

================================================================================
来源：http://nxw.redwolf501.top

统计汇总
来源：http://naw.ivvv.top

================================================================================
来源：http://hwb.zhongyouzk.top

按语言统计（条）：
来源：http://voq.xinyue.icu

Python ......... 252
来源：http://jhp.vehdjk.com

PHP ............ 252
来源：http://ddj.yvedp.cn

JavaScript ..... 252
来源：http://xai.ivvv.top

TypeScript ..... 212
来源：http://trq.xuetiantiany.cn

Java ........... 212
来源：http://oqw.chenlongwang.top

Go ............. 212
来源：http://usl.sufxvd.cn

Ruby ........... 212
来源：http://xqe.jinqigufen.top

C# ............. 212
来源：http://rgc.dashuyun.cn

C .............. 30
来源：http://nas.yuxming.cn

C++ ............ 30
来源：http://ebs.zhixingplan.top

SQL ............ 90
来源：http://lhj.fehbvm.com

Bash ........... 80
来源：http://rty.gaohongyu789.top

Kotlin ......... 15
来源：http://xvh.haohaochexian.top

Swift .......... 15
来源：http://lnp.jinghuilouyu.cn

Lua ............ 10
来源：http://lrv.ybcxt.top

Perl ........... 10
来源：http://wva.daria6918.cn

Scala .......... 10
来源：http://huc.jqgufenzy.top

------------------------------------
来源：http://wsr.hesvh.cn

合计 ........... 2106 条
来源：http://wfh.cdnleiting.top

按章节统计：
来源：http://fjm.snrcjt.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hho.hongshengwenyu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qji.yueranfly.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://urg.feifeiyinyue.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ekv.xuetiantiany.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://aoy.jqgufenzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pkr.sweek.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cnf.kuanghao11.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://eok.daria6918.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ipd.meibo888.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tpa.zhoulong.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oru.quarkkingdee.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nzh.sxryk.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wch.haohaochexian.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://woc.yangfankeji.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bsm.cdnleiting.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://obl.nwbrower.top

Q SQL 专题                              90
来源：http://fkp.fzhhl.top

R Bash 专题                             80
来源：http://huh.52xcode.cn

S C / C++ 专题                          60
来源：http://skv.yfazqb.com

T 其他语言补充                          60
来源：http://sgv.jinqigfzy.top

U 高频实用片段                         120
来源：http://bgq.ehwqpu.com

------------------------------------
来源：http://dgn.xingfuxueyuan.xyz

合计                                  2106 条
来源：http://sdt.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://epe.jqgfzy.top

使用提醒
来源：http://kma.fzhhl.top

--------------------------------------------------------------------------------
来源：http://cdr.jqgufenzy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xel.hfpthk.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lli.sxryk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jfu.zhoulong.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://lns.chenlongwang.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mvd.daria6918.cn

—— 文件结束 ——
来源：http://tti.0kj1m.cn

================================================================================
来源：http://jzg.ywan-chungtsiang.top

程序语言常见例子速查手册（2024 版）
来源：http://alf.zhijiandao.cn

Common Programming Examples Cheat Book
来源：http://gfk.316326.xyz

================================================================================
来源：http://ilg.ybcxt.top

【收录内容】
来源：http://ugp.hammf.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dul.iojbl.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pxw.yvedp.cn

SQL · Bash · C · C++
来源：http://hwg.meibo888.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://why.chenlongwang.top

【使用说明】
来源：http://vmn.tianlin.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://uoy.zycfv.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tgd.sufxvd.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dmz.hcnkem.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nry.tianlin.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://yhv.haohaochexian.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qun.tanke756.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://acz.birdmap.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://omo.zhiwuduotai.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vyg.xylfe.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dxj.sufxvd.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://moe.yonumen.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ayj.meibo888.top

【文件统计】
来源：http://uun.chenjidiqi.icu

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uyn.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://nyk.yj20258888.top

目  录
来源：http://nsc.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://kns.jinqigfzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://avj.yanxiufei.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://efc.haohaochexian.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pff.pengpengdd.cyou

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pxn.yj20258888.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iuh.shangyingyoupin.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fgb.fengsongda.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cks.bbcook.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jyp.hnqzz.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tes.zhoulong.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lpw.sysykeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zjq.xingfuxueyuan.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mbk.hfpthk.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://diu.zhoulong.xyz


<!-- 参考信息 -->