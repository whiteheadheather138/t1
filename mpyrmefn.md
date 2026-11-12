代发 wailian999

[U17] Py：初始化日志
来源：http://tcz.vqdsnc.cn

logging.basicConfig(level=logging.INFO)
来源：http://uga.zhaomingkeji.xyz

[U18] Py：预编译正则
来源：http://dyw.epnwcf.com

pat = re.compile(r"\d+")
来源：http://gxg.epnwcf.com

[U19] Py：正则替换带回调
来源：http://zhv.xinyue.icu

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oli.chenjidiqi.icu

[U20] Py：缓存函数结果
来源：http://wgb.xuetiantiany.cn

@functools.lru_cache(maxsize=None)
来源：http://xpe.zhongyouzk.top

[U21] Py：自定义上下文管理器
来源：http://dln.shanyushiyangkeji.top

@contextlib.contextmanager
来源：http://tjd.ehwqpu.com

[U22] Py：矩阵转置
来源：http://mfo.zhixingplan.top

list(zip(*m))
来源：http://qla.hysaishi.cn

[U23] Py：分块读取大文件
来源：http://ypv.sjlbkw.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://avg.jianghu66.top

[U24] Py：路径操作
来源：http://pvf.dianchejie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rud.hongshengwenyu.top

[U25] Py：CSV 按字典读
来源：http://kkn.guowangkeji.top

csv.DictReader(f)
来源：http://kxg.uphjek.com

[U26] Py：并发下载
来源：http://xgr.yj20258888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gnr.havefunace.top

[U27] Py：异步 HTTP
来源：http://szc.fengsongda.top

aiohttp.ClientSession() 配合 async with
来源：http://clv.tarul.cn

[U28] Py：类型别名
来源：http://ddw.tian-w.cn

UserId = int
来源：http://ltp.jqgufenzy.top

[U29] Py：属性校验
来源：http://ybe.fehbvm.com

@property 与 @x.setter 配合
来源：http://see.9152youxi.cn

[U30] Py：数据类
来源：http://vcz.hcnkem.com

@dataclass(slots=True)
来源：http://sfq.fehbvm.com

[U31] Py：单测
来源：http://hep.yvedp.cn

python -m pytest -q
来源：http://pwi.cheryme.top

[U32] Py：代码格式化
来源：http://zcn.pycfn.com

ruff format . && ruff check --fix .
来源：http://zvf.xingfuxueyuan.xyz

[U33] Py：打包发布
来源：http://dlq.dashuyun.cn

python -m build  （依赖 pyproject.toml）
来源：http://aaw.316326.xyz

[U34] Py：判断编码
来源：http://nye.fanxiaobao.xyz

chardet.detect(raw)
来源：http://xuy.zhijiandao.cn

[U35] Py：发送邮件
来源：http://ysg.hfpthk.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sfe.jianghu66.top

[U36] Py：定时任务
来源：http://xpi.ctjpmb.com

schedule.every(10).minutes.do(job)
来源：http://abx.ctjpmb.com

[U37] Py：读写 Excel
来源：http://dcq.sxryk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ktq.yj20258888.top

[U38] Py：获取脚本所在目录
来源：http://qfo.hywenlv.cn

Path(__file__).resolve().parent
来源：http://tcm.ybcxt.top

[U39] Py：判断是否在交互环境
来源：http://ffp.zhixingplan.top

sys.stdout.isatty()
来源：http://lea.jinghuilouyu.cn

[U40] Py：打印到标准错误
来源：http://anb.havefunace.top

print("err", file=sys.stderr)
来源：http://bco.sysykeji.top

[U41] PHP：初始化 Composer 项目
来源：http://wze.snrcjt.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jyw.pycfn.com

[U42] PHP：PSR-4 自动加载
来源：http://qmr.xziqi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://caz.havefunace.top

[U43] PHP：声明命名空间
来源：http://jkj.cheryme.top

namespace App\Http;
来源：http://rji.pengpengdd.cyou

[U44] PHP：开启严格类型
来源：http://zzu.ehwqpu.com

declare(strict_types=1);
来源：http://kir.xinyue.icu

[U45] PHP：类型声明与返回类型
来源：http://nbw.jqgfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://sum.svipenyu.cn

[U46] PHP：可空类型
来源：http://vpx.jiagoushi.top

?string $name = null
来源：http://bwo.jqgufenzy.top

[U47] PHP：联合类型
来源：http://iuy.havefunace.top

int|string $id
来源：http://cmf.ywan-chungtsiang.top

[U48] PHP：纯枚举
来源：http://oby.yueranfly.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://knm.yj20258.top

[U49] PHP：只读属性
来源：http://dyx.hnxiangtu.top

public readonly string $name
来源：http://kul.0kj1m.cn

[U50] PHP：构造器属性提升
来源：http://qwm.jinyuanbaomall.cn

public function __construct(private int $id) {}
来源：http://btg.jinghuilouyu.cn

[U51] PHP：数组解构
来源：http://xty.cashguo.top

[$a, $b] = $arr;
来源：http://hcf.birdmap.top

[U52] PHP：箭头函数
来源：http://vli.hnqzz.top

$double = fn($x) => $x * 2;
来源：http://aje.xuanzx.com

[U53] PHP：空合并运算符
来源：http://wwx.cucudq.cn

$v = $a ?? $b ?? "default";
来源：http://qbe.zdqjudy.top

[U54] PHP：空安全调用
来源：http://rtm.jinqigufen.top

$obj?->method()
来源：http://unk.zycfv.cn

[U55] PHP：match 表达式
来源：http://bfp.yj20258888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wom.yfazqb.com

[U56] PHP：命名参数
来源：http://sci.jiagoushi.top

f(a: 1, b: 2)
来源：http://irf.xuanzx.com

[U57] PHP：字符串插值
来源：http://tgj.gotoacloud.top

"值: {$a}"
来源：http://fkl.hongshengwenyu.top

[U58] PHP：数组三件套
来源：http://mwh.xuanzx.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ivo.sufxvd.cn

[U59] PHP：自定义排序
来源：http://soi.tanke756.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kfo.zhaomingkeji.xyz

[U60] PHP：JSON 编解码
来源：http://wrm.dashuyun.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mnc.ppjwa.cn

[U61] PHP：正则
来源：http://wkx.snrcjt.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cwn.ybcxt.top

[U62] PHP：日期对象
来源：http://oty.wangdashe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xyk.sysykeji.top

[U63] PHP：文件读写
来源：http://kih.sufxvd.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rgu.hfpthk.cn

[U64] PHP：目录遍历
来源：http://rnh.jyoumei.cn

glob("dir/*.php");  scandir("dir");
来源：http://add.guowangkeji.top

[U65] PHP：会话
来源：http://jaf.shzxlz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://daa.hnqzz.top

[U66] PHP：设置 Cookie
来源：http://nzr.aibaodan.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nmv.shanyushiyangkeji.top

[U67] PHP：处理文件上传
来源：http://yzp.iojbl.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uqu.cqqwz.cn

[U68] PHP：PDO 连接
来源：http://wge.yj20258.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hxg.redwolf501.top

[U69] PHP：PDO 预处理
来源：http://tdx.zhengqikj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zzc.redwolf501.top

[U70] PHP：PDO 事务
来源：http://nlz.yj202588.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vmt.zdbjq.cn

[U71] PHP：抛出异常
来源：http://qlo.0kj1m.cn

throw new RuntimeException("失败", 500);
来源：http://wqc.daria6918.cn

[U72] PHP：写错误日志
来源：http://vdm.hongshengwenyu.top

error_log("失败: " . $e->getMessage());
来源：http://ikq.dianchejie.cn

[U73] PHP：读取 ini 配置
来源：http://rvv.fktsv.cn

parse_ini_file("config.ini", true)
来源：http://qmz.xylfe.cn

[U74] PHP：读取环境变量
来源：http://ppd.ydzc1.top

getenv("APP_ENV") ?: "production"
来源：http://pks.chenlongwang.top

[U75] PHP：依赖注入
来源：http://fjf.sweek.top

composer require psr/container
来源：http://nqu.pengpengdd.cyou

[U76] PHP：简单路由
来源：http://jax.guowangkeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kje.svipenyu.cn

[U77] PHP：模板渲染
来源：http://nzq.yj20258.top

composer require twig/twig
来源：http://qlb.daria6918.cn

[U78] PHP：单元测试
来源：http://nsn.yj202588.top

composer require --dev phpunit/phpunit
来源：http://hrd.nanxuanxn.top

[U79] PHP：静态分析
来源：http://xzu.haohaochexian.top

composer require --dev phpstan/phpstan
来源：http://blz.jinghuilouyu.cn

[U80] PHP：代码规范修复
来源：http://fwr.yanxiufei.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rnx.fehbvm.com

[U81] JS：初始化项目
来源：http://zsh.chenlongwang.top

npm init -y;  npm i express
来源：http://hty.yvedp.cn

[U82] JS：package.json 脚本
来源：http://jvn.svipenyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bui.zhiwuduotai.top

[U83] JS：ES Module 导入导出
来源：http://jnq.zdqjudy.top

export const a = 1;  import { a } from "./m.js";
来源：http://rtw.yueranfly.top

[U84] JS：CommonJS 写法
来源：http://vfv.cashguo.top

module.exports = { a };  const { a } = require("./m");
来源：http://mzp.redwolf501.top

[U85] JS：可选链
来源：http://heo.sysykeji.top

a?.b?.c
来源：http://wwh.zhixingplan.top

[U86] JS：空值合并
来源：http://wkd.sjlbkw.cn

a ?? b
来源：http://iqg.fehbvm.com

[U87] JS：解构默认值
来源：http://kml.quarkkingdee.top

const { a = 1, b = 2 } = obj;
来源：http://ztj.zhoulong.xyz

[U88] JS：对象展开合并
来源：http://nzh.cdnleiting.top

{ ...a, ...b }
来源：http://tvr.fengsongda.top

[U89] JS：数组去重
来源：http://hod.chenjidiqi.icu

[...new Set(arr)]
来源：http://nxw.snrcjt.cn

[U90] JS：数字数组排序
来源：http://dvp.kuanghao11.cn

[...arr].sort((a, b) => a - b)
来源：http://cjc.yongpay.top

[U91] JS：对象键值遍历
来源：http://ijq.guannengcc.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bfi.xuanzx.com

[U92] JS：深拷贝
来源：http://sfg.yanxiufei.cn

structuredClone(obj)
来源：http://sql.hongshengwenyu.top

[U93] JS：模板字符串
来源：http://hht.xingfuxueyuan.xyz

`共 ${n} 条`
来源：http://dtg.c1oappe.top

[U94] JS：箭头函数
来源：http://aqx.hcnkem.com

const double = x => x * 2;
来源：http://bxg.guannengcc.top

[U95] JS：Promise 包装
来源：http://zpq.snrcjt.cn

new Promise((resolve, reject) => {})
来源：http://okl.ybcxt.top

[U96] JS：async/await 与异常
来源：http://way.sweek.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dna.zhixingplan.top

[U97] JS：并发请求
来源：http://hrm.daxiang520.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://uov.zhongyouzk.top

[U98] JS：fetch 带 JSON
来源：http://exz.gotoacloud.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fzp.daxiang520.top

[U99] JS：事件监听
来源：http://gna.jqgufenzy.top

el.addEventListener("click", e => {})
来源：http://bro.yangfankeji.com

[U100] JS：DOM 查询
来源：http://gsa.gaohongyu789.top

document.querySelector(".item")
来源：http://dea.yvedp.cn

[U101] JS：classList 操作
来源：http://brs.sxryk.cn

el.classList.toggle("active")
来源：http://nho.wangshuangyany.cn

[U102] JS：本地存储
来源：http://jli.sysykeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bmc.vehdjk.com

[U103] JS：定时器
来源：http://pxk.yonumen.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mcf.yuanzhike.top

[U104] JS：防抖
来源：http://tcc.pengpengdd.cyou

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://olq.zhaomingkeji.xyz

[U105] JS：节流
来源：http://jlr.tian-w.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oka.fktsv.cn

[U106] JS：日期格式化
来源：http://ciz.tanke756.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ytn.snrcjt.cn

[U107] JS：数字千分位
来源：http://quf.cqqwz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://loo.yonumen.top

[U108] JS：随机整数
来源：http://vml.iojbl.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://klu.c1oappe.top

[U109] JS：数组分组
来源：http://vkj.gotoacloud.top

Object.groupBy(arr, x => x.type)
来源：http://rri.quarkkingdee.top

[U110] JS：数组分块
来源：http://ygi.hfpthk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bjp.jiagoushi.top

[U111] JS：对象转 Map
来源：http://yvh.xziqi.cn

new Map(Object.entries(obj))
来源：http://rye.dianchejie.cn

[U112] JS：字符串补位
来源：http://bcc.tarul.cn

"7".padStart(3, "0")
来源：http://gpo.chenlongwang.top

[U113] JS：正则替换全部
来源：http://uut.hysaishi.cn

s.replaceAll("a", "b")
来源：http://gkm.meibo888.top

[U114] JS：JSON 深比较
来源：http://qau.svipenyu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://isk.jianghu66.top

[U115] JS：生成 UUID
来源：http://ole.xinyue.icu

crypto.randomUUID()
来源：http://jrd.zhiwuduotai.top

[U116] JS：类型检查（JSDoc）
来源：http://qxp.dashuyun.cn

/** @param {string} name */ function f(name) {}
来源：http://ofb.shanyushiyangtech.top

[U117] JS：单元测试
来源：http://qrz.9152youxi.cn

npm i -D vitest;  npx vitest
来源：http://qxq.kuanghao11.cn

[U118] JS：开发服务器
来源：http://wsg.yueranfly.top

npm i -D vite;  npx vite
来源：http://fpf.cdnleiting.top

[U119] JS：生产构建
来源：http://nja.gotoacloud.top

npx vite build
来源：http://vnc.yj20258.top

[U120] JS：读取环境变量（Vite）
来源：http://vpi.nanxinkj.top

import.meta.env.VITE_API_URL
来源：http://hll.xuetiantiany.cn

================================================================================
来源：http://qmy.yfazqb.com

统计汇总
来源：http://wyc.gotoacloud.top

================================================================================
来源：http://kqo.sxryk.cn

按语言统计（条）：
来源：http://xyy.xuetiantiany.cn

Python ......... 252
来源：http://vao.zhengqikj.top

PHP ............ 252
来源：http://vsz.mhx1999.top

JavaScript ..... 252
来源：http://vte.cdnleiting.top

TypeScript ..... 212
来源：http://wpk.shzxlz.cn

Java ........... 212
来源：http://oni.jqgufenzy.top

Go ............. 212
来源：http://vnr.cheryme.top

Ruby ........... 212
来源：http://kad.meibo888.top

C# ............. 212
来源：http://xuw.chenlongwang.top

C .............. 30
来源：http://gcf.zhongyouzk.top

C++ ............ 30
来源：http://fqa.yj20258888.top

SQL ............ 90
来源：http://esh.birdmap.top

Bash ........... 80
来源：http://qnw.feifeiyinyue.top

Kotlin ......... 15
来源：http://pke.jlsjyb.cn

Swift .......... 15
来源：http://akc.cheryme.top

Lua ............ 10
来源：http://pnk.epnwcf.com

Perl ........... 10
来源：http://iis.cdnleiting.top

Scala .......... 10
来源：http://nnv.hcnkem.com

------------------------------------
来源：http://hkn.hnqzz.top

合计 ........... 2106 条
来源：http://tdi.yangfankeji.com

按章节统计：
来源：http://ats.zhaomingkeji.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ikz.hnxiangtu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ila.guowangkeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gwp.jinghuilouyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fei.daxiang520.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fbh.nwbrower.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lan.0kj1m.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qce.bbcook.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lvl.redwolf501.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tlx.jiagoushi.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lhm.c1oappe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wot.redwolf501.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zix.guannengcc.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://czh.zhijiandao.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://drb.dashuyun.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yuw.gaohongyu789.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fqn.jinghuilouyu.cn

Q SQL 专题                              90
来源：http://vwz.cashguo.top

R Bash 专题                             80
来源：http://cqi.jianghu66.top

S C / C++ 专题                          60
来源：http://zdi.yj202588.top

T 其他语言补充                          60
来源：http://biy.xingfuxueyuan.xyz

U 高频实用片段                         120
来源：http://pey.zdqjudy.top

------------------------------------
来源：http://zne.chenzaomai.com

合计                                  2106 条
来源：http://yfx.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://ayy.ydzc1.top

使用提醒
来源：http://aep.jianghu66.top

--------------------------------------------------------------------------------
来源：http://tpg.cqqwz.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hvy.zhoulong.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sxv.quarkkingdee.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jvz.guowangkeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://syo.shangyingyoupin.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gyu.chenzaomai.com

—— 文件结束 ——
来源：http://aiv.vehdjk.com

================================================================================
来源：http://smk.shanyushiyangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://uzc.gogol.net.cn

Common Programming Examples Cheat Book
来源：http://iex.tarul.cn

================================================================================
来源：http://asx.haohaochexian.top

【收录内容】
来源：http://ykx.hammf.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sob.zhiwuduotai.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ydr.bbcook.cn

SQL · Bash · C · C++
来源：http://ysj.hnqzz.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://voe.meibo888.top

【使用说明】
来源：http://rxu.hysaishi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rti.yuanzhike.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lnc.guowangkeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://veh.tian-w.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ubq.cashguo.top

Bash:  Shell         C:     C             C++:   C++
来源：http://kbu.dashuyun.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kha.guowangkeji.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bzx.redwolf501.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dod.jinqigfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gic.tianlin.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ijw.gaohongyu789.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vkp.ywan-chungtsiang.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kvj.zhoulong.xyz

【文件统计】
来源：http://iju.xuanzx.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rec.yonumen.top

--------------------------------------------------------------------------------
来源：http://dcb.hnxiangtu.top

目  录
来源：http://qib.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://pqn.xylfe.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vtq.vqdsnc.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pxs.gogol.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://syv.nwbrower.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://eov.zdqjudy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yer.zycfv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ruq.zhixingplan.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ygi.hfpthk.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://you.tianlin.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://irp.jlsjyb.cn


<!-- 参考信息 -->