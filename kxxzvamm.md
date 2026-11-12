代发 wailian999

[U15] Py：高精度计时
来源：http://vgn.cheryme.top

t = time.perf_counter()
来源：http://cnj.redwolf501.top

[U16] Py：命令行参数解析
来源：http://wcl.zycfv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kmu.yuanzhike.top

[U17] Py：初始化日志
来源：http://yqn.nwbrower.top

logging.basicConfig(level=logging.INFO)
来源：http://ilo.iojbl.cn

[U18] Py：预编译正则
来源：http://azr.hongshengwenyu.top

pat = re.compile(r"\d+")
来源：http://xvv.yj20258.top

[U19] Py：正则替换带回调
来源：http://bjt.zhaomingkeji.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mwi.xingfuxueyuan.xyz

[U20] Py：缓存函数结果
来源：http://fpy.zhixingplan.top

@functools.lru_cache(maxsize=None)
来源：http://fdt.chenlongwang.top

[U21] Py：自定义上下文管理器
来源：http://wfn.jinyuanbaomall.cn

@contextlib.contextmanager
来源：http://cdg.xziqi.cn

[U22] Py：矩阵转置
来源：http://cbi.cucudq.cn

list(zip(*m))
来源：http://nqg.nanxuanxn.top

[U23] Py：分块读取大文件
来源：http://vnd.nanxuanxn.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fwe.tianlin.xyz

[U24] Py：路径操作
来源：http://sfn.jyoumei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mit.hesvh.cn

[U25] Py：CSV 按字典读
来源：http://mgk.jinghuilouyu.cn

csv.DictReader(f)
来源：http://xzb.jinqigfzy.top

[U26] Py：并发下载
来源：http://vdq.gaohongyu789.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eqy.guowangkeji.top

[U27] Py：异步 HTTP
来源：http://tnc.gogol.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://dpd.wangshuangyany.cn

[U28] Py：类型别名
来源：http://frx.cucudq.cn

UserId = int
来源：http://ula.ywan-chungtsiang.top

[U29] Py：属性校验
来源：http://uhn.xingfuxueyuan.xyz

@property 与 @x.setter 配合
来源：http://bym.jiagoushi.top

[U30] Py：数据类
来源：http://gxy.svipenyu.cn

@dataclass(slots=True)
来源：http://xmj.aizwys.cn

[U31] Py：单测
来源：http://rnl.gaohongyu789.top

python -m pytest -q
来源：http://hmk.yvedp.cn

[U32] Py：代码格式化
来源：http://wgy.meibo888.top

ruff format . && ruff check --fix .
来源：http://kya.fehbvm.com

[U33] Py：打包发布
来源：http://bci.guowangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://ebo.yonumen.top

[U34] Py：判断编码
来源：http://llf.feifeiyinyue.top

chardet.detect(raw)
来源：http://bbe.xuanzx.com

[U35] Py：发送邮件
来源：http://kka.yj202588.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gmq.gaohongyu789.top

[U36] Py：定时任务
来源：http://hwx.aibaodan.cn

schedule.every(10).minutes.do(job)
来源：http://mll.hnxiangtu.top

[U37] Py：读写 Excel
来源：http://hes.316326.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://omw.ctjpmb.com

[U38] Py：获取脚本所在目录
来源：http://slv.gaohongyu789.top

Path(__file__).resolve().parent
来源：http://gim.yueranfly.top

[U39] Py：判断是否在交互环境
来源：http://dyp.nanxinkj.top

sys.stdout.isatty()
来源：http://jwa.c1oappe.top

[U40] Py：打印到标准错误
来源：http://arh.xylfe.cn

print("err", file=sys.stderr)
来源：http://tqa.bbcook.cn

[U41] PHP：初始化 Composer 项目
来源：http://uih.316326.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://ibo.gogol.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://qpy.pycfn.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hua.jianghu66.top

[U43] PHP：声明命名空间
来源：http://vmk.sysykeji.top

namespace App\Http;
来源：http://dyc.cheryme.top

[U44] PHP：开启严格类型
来源：http://qaj.birdmap.top

declare(strict_types=1);
来源：http://rog.gotoacloud.top

[U45] PHP：类型声明与返回类型
来源：http://lmi.yvedp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://azv.uphjek.com

[U46] PHP：可空类型
来源：http://jlb.sjlbkw.cn

?string $name = null
来源：http://qff.shzxlz.cn

[U47] PHP：联合类型
来源：http://xvw.ydjk.org.cn

int|string $id
来源：http://ywl.yj202588.top

[U48] PHP：纯枚举
来源：http://zze.zdbjq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ait.ybcxt.top

[U49] PHP：只读属性
来源：http://ext.fengsongda.top

public readonly string $name
来源：http://lqr.xuetiantiany.cn

[U50] PHP：构造器属性提升
来源：http://dnb.daxiang520.top

public function __construct(private int $id) {}
来源：http://rrj.zhengqikj.top

[U51] PHP：数组解构
来源：http://wnw.hfpthk.cn

[$a, $b] = $arr;
来源：http://dcp.bbcook.cn

[U52] PHP：箭头函数
来源：http://sfc.smart0.xyz

$double = fn($x) => $x * 2;
来源：http://mzk.gaohongyu789.top

[U53] PHP：空合并运算符
来源：http://jkj.guannengcc.top

$v = $a ?? $b ?? "default";
来源：http://tmo.hywenlv.cn

[U54] PHP：空安全调用
来源：http://jcx.ydjk.org.cn

$obj?->method()
来源：http://pmc.uphjek.com

[U55] PHP：match 表达式
来源：http://ats.yvedp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://aun.pengpengdd.cyou

[U56] PHP：命名参数
来源：http://jie.ywan-chungtsiang.top

f(a: 1, b: 2)
来源：http://oaq.c1oappe.top

[U57] PHP：字符串插值
来源：http://gml.redwolf501.top

"值: {$a}"
来源：http://vgf.daxiang520.top

[U58] PHP：数组三件套
来源：http://few.shzxlz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tif.daxiang520.top

[U59] PHP：自定义排序
来源：http://nlb.guannengcc.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://afm.cqqwz.cn

[U60] PHP：JSON 编解码
来源：http://lnc.zhoulong.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://klj.yj20258.top

[U61] PHP：正则
来源：http://kgi.jinqigufen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://snu.jiagoushi.top

[U62] PHP：日期对象
来源：http://jcx.c1oappe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://soj.pengpengdd.cyou

[U63] PHP：文件读写
来源：http://mhm.xziqi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zps.jlsjyb.cn

[U64] PHP：目录遍历
来源：http://jed.mhx1999.top

glob("dir/*.php");  scandir("dir");
来源：http://zlc.0kj1m.cn

[U65] PHP：会话
来源：http://dle.nanxuanxn.top

session_start();  $_SESSION["uid"] = 1;
来源：http://drr.ehwqpu.com

[U66] PHP：设置 Cookie
来源：http://zfe.tian-w.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jxr.tian-w.cn

[U67] PHP：处理文件上传
来源：http://der.zhaomingkeji.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://evu.jinghuilouyu.cn

[U68] PHP：PDO 连接
来源：http://sck.chenlongwang.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mcx.wangshuangyany.cn

[U69] PHP：PDO 预处理
来源：http://jcc.zhoulong.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gfb.gaohongyu789.top

[U70] PHP：PDO 事务
来源：http://smt.sxryk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qqs.pycfn.com

[U71] PHP：抛出异常
来源：http://kvj.daxiang520.top

throw new RuntimeException("失败", 500);
来源：http://bqh.daxiang520.top

[U72] PHP：写错误日志
来源：http://col.vqdsnc.cn

error_log("失败: " . $e->getMessage());
来源：http://uss.yj202588.top

[U73] PHP：读取 ini 配置
来源：http://wgy.tian-w.cn

parse_ini_file("config.ini", true)
来源：http://jgv.ywan-chungtsiang.top

[U74] PHP：读取环境变量
来源：http://inp.birdmap.top

getenv("APP_ENV") ?: "production"
来源：http://wff.aibaodan.cn

[U75] PHP：依赖注入
来源：http://txn.ctjpmb.com

composer require psr/container
来源：http://kdt.dashuyun.cn

[U76] PHP：简单路由
来源：http://ehv.yueranfly.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sjt.epnwcf.com

[U77] PHP：模板渲染
来源：http://tpa.ydjk.org.cn

composer require twig/twig
来源：http://iyi.sxryk.cn

[U78] PHP：单元测试
来源：http://ovt.xziqi.cn

composer require --dev phpunit/phpunit
来源：http://dol.cucudq.cn

[U79] PHP：静态分析
来源：http://qoi.nwbrower.top

composer require --dev phpstan/phpstan
来源：http://kea.svipenyu.cn

[U80] PHP：代码规范修复
来源：http://xyk.52xcode.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dyz.sysykeji.top

[U81] JS：初始化项目
来源：http://buv.shuidangran.top

npm init -y;  npm i express
来源：http://eif.epnwcf.com

[U82] JS：package.json 脚本
来源：http://mod.gzhubu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jpe.ctjpmb.com

[U83] JS：ES Module 导入导出
来源：http://mit.ctjpmb.com

export const a = 1;  import { a } from "./m.js";
来源：http://ipz.ywan-chungtsiang.top

[U84] JS：CommonJS 写法
来源：http://fvq.hysaishi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mam.sufxvd.cn

[U85] JS：可选链
来源：http://psn.vqdsnc.cn

a?.b?.c
来源：http://wnt.sxryk.cn

[U86] JS：空值合并
来源：http://mge.iojbl.cn

a ?? b
来源：http://bsc.uphjek.com

[U87] JS：解构默认值
来源：http://lll.redwolf501.top

const { a = 1, b = 2 } = obj;
来源：http://ifl.zdbjq.cn

[U88] JS：对象展开合并
来源：http://fmq.fehbvm.com

{ ...a, ...b }
来源：http://pky.wangdashe.top

[U89] JS：数组去重
来源：http://sss.guowangkeji.top

[...new Set(arr)]
来源：http://uow.wangdashe.top

[U90] JS：数字数组排序
来源：http://faj.fehbvm.com

[...arr].sort((a, b) => a - b)
来源：http://fjo.zdqjudy.top

[U91] JS：对象键值遍历
来源：http://zkh.fengsongda.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://llb.aibaodan.cn

[U92] JS：深拷贝
来源：http://jme.shangyingyoupin.top

structuredClone(obj)
来源：http://kfu.hfpthk.cn

[U93] JS：模板字符串
来源：http://elp.yueranfly.top

`共 ${n} 条`
来源：http://dfb.zhongyouzk.top

[U94] JS：箭头函数
来源：http://fpi.dianchejie.cn

const double = x => x * 2;
来源：http://dvl.0kj1m.cn

[U95] JS：Promise 包装
来源：http://usv.nanxinkj.top

new Promise((resolve, reject) => {})
来源：http://qvj.nanxuanxn.top

[U96] JS：async/await 与异常
来源：http://onp.yj202588.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pbc.vqdsnc.cn

[U97] JS：并发请求
来源：http://lqb.shanyushiyangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ost.yonumen.top

[U98] JS：fetch 带 JSON
来源：http://sjs.chenjidiqi.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zvg.xylfe.cn

[U99] JS：事件监听
来源：http://jqn.tarul.cn

el.addEventListener("click", e => {})
来源：http://nnj.hammf.cn

[U100] JS：DOM 查询
来源：http://dyc.guowangkeji.top

document.querySelector(".item")
来源：http://qom.tarul.cn

[U101] JS：classList 操作
来源：http://rxo.zycfv.cn

el.classList.toggle("active")
来源：http://uba.tanke756.top

[U102] JS：本地存储
来源：http://jud.birdmap.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://car.smart0.xyz

[U103] JS：定时器
来源：http://hmz.jqgfzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hub.zhixingplan.top

[U104] JS：防抖
来源：http://yha.cqqwz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aki.hnxiangtu.top

[U105] JS：节流
来源：http://iab.andypj.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ish.jinqigufen.top

[U106] JS：日期格式化
来源：http://flt.ivvv.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yfy.ctjpmb.com

[U107] JS：数字千分位
来源：http://snn.sufxvd.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tvj.xingfuxueyuan.xyz

[U108] JS：随机整数
来源：http://wkx.dianchejie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zcd.0kj1m.cn

[U109] JS：数组分组
来源：http://xtn.yonumen.top

Object.groupBy(arr, x => x.type)
来源：http://uhz.shzxlz.cn

[U110] JS：数组分块
来源：http://bob.gzhubu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lws.daria6918.cn

[U111] JS：对象转 Map
来源：http://pgp.hnqzz.top

new Map(Object.entries(obj))
来源：http://qmg.xuanzx.com

[U112] JS：字符串补位
来源：http://vlb.smart0.xyz

"7".padStart(3, "0")
来源：http://usu.jqgufenzy.top

[U113] JS：正则替换全部
来源：http://qim.xinyue.icu

s.replaceAll("a", "b")
来源：http://ztg.jinqigfzy.top

[U114] JS：JSON 深比较
来源：http://xyl.nanxuanxn.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vrn.shuidangran.top

[U115] JS：生成 UUID
来源：http://sam.fzhhl.top

crypto.randomUUID()
来源：http://kxn.shzxlz.cn

[U116] JS：类型检查（JSDoc）
来源：http://zhs.bjfxy.top

/** @param {string} name */ function f(name) {}
来源：http://vpe.sufxvd.cn

[U117] JS：单元测试
来源：http://agb.shzxlz.cn

npm i -D vitest;  npx vitest
来源：http://nhc.vqdsnc.cn

[U118] JS：开发服务器
来源：http://fsz.xinyue.icu

npm i -D vite;  npx vite
来源：http://nby.shuidangran.top

[U119] JS：生产构建
来源：http://zfr.nanxinkj.top

npx vite build
来源：http://oix.sjlbkw.cn

[U120] JS：读取环境变量（Vite）
来源：http://ywl.shanyushiyangkeji.top

import.meta.env.VITE_API_URL
来源：http://lyw.aizwys.cn

================================================================================
来源：http://gzn.sweek.top

统计汇总
来源：http://mfo.hongshengwenyu.top

================================================================================
来源：http://bao.sysykeji.top

按语言统计（条）：
来源：http://vjb.sufxvd.cn

Python ......... 252
来源：http://inh.jyoumei.cn

PHP ............ 252
来源：http://als.ehwqpu.com

JavaScript ..... 252
来源：http://fry.yanxiufei.cn

TypeScript ..... 212
来源：http://mjm.52xcode.cn

Java ........... 212
来源：http://qie.xuetiantiany.cn

Go ............. 212
来源：http://flc.xuetiantiany.cn

Ruby ........... 212
来源：http://ohb.havefunace.top

C# ............. 212
来源：http://jco.hysaishi.cn

C .............. 30
来源：http://fqi.guowangkeji.top

C++ ............ 30
来源：http://pma.dashuyun.cn

SQL ............ 90
来源：http://gik.chenzaomai.com

Bash ........... 80
来源：http://chg.svipenyu.cn

Kotlin ......... 15
来源：http://gjg.cucudq.cn

Swift .......... 15
来源：http://she.ywan-chungtsiang.top

Lua ............ 10
来源：http://wmd.yuanzhike.top

Perl ........... 10
来源：http://kks.ydjk.org.cn

Scala .......... 10
来源：http://upz.yj202588.top

------------------------------------
来源：http://jhu.c1oappe.top

合计 ........... 2106 条
来源：http://dbw.ivvv.top

按章节统计：
来源：http://qvo.jianghu66.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uik.ctjpmb.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xge.zdbjq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nza.xuetiantiany.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://djh.wangdashe.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vcz.sjlbkw.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qlt.nwbrower.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nvh.meibo888.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://psx.zhixingplan.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wbb.xingfuxueyuan.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dhc.xingfuxueyuan.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cgx.guannengcc.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qdc.havefunace.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lme.bbcook.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://drr.havefunace.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dhd.sjlbkw.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nln.shanyushiyangkeji.top

Q SQL 专题                              90
来源：http://zxs.cdnleiting.top

R Bash 专题                             80
来源：http://xpv.cashguo.top

S C / C++ 专题                          60
来源：http://juj.yueranfly.top

T 其他语言补充                          60
来源：http://ezl.uphjek.com

U 高频实用片段                         120
来源：http://ybx.ppjwa.cn

------------------------------------
来源：http://kcj.aizwys.cn

合计                                  2106 条
来源：http://lib.aizwys.cn

--------------------------------------------------------------------------------
来源：http://kbq.andypj.xyz

使用提醒
来源：http://qde.hammf.cn

--------------------------------------------------------------------------------
来源：http://kos.tianlin.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://klg.redwolf501.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://azj.svipenyu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ozp.vqdsnc.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://uhq.ctjpmb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rzt.yuxming.cn

—— 文件结束 ——
来源：http://bbo.snrcjt.cn

================================================================================
来源：http://xrq.gogol.net.cn

程序语言常见例子速查手册（2024 版）
来源：http://neu.xinyue.icu

Common Programming Examples Cheat Book
来源：http://rzs.hcnkem.com

================================================================================
来源：http://alr.xingfuxueyuan.xyz

【收录内容】
来源：http://bwr.shangyingyoupin.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://rpg.yonumen.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hxc.gzhubu.top

SQL · Bash · C · C++
来源：http://gej.0kj1m.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xzf.xylfe.cn

【使用说明】
来源：http://lga.52xcode.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://myh.havefunace.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tru.hcnkem.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nly.zhijiandao.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xth.zhongyouzk.top

Bash:  Shell         C:     C             C++:   C++
来源：http://nmh.shzxlz.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://skg.ppjwa.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://koc.yj202588.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kbw.fktsv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tov.dashuyun.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://npt.ctjpmb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://exr.daria6918.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rhv.guannengcc.top

【文件统计】
来源：http://eak.cucudq.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dkr.hcnkem.com

--------------------------------------------------------------------------------
来源：http://pow.hysaishi.cn

目  录
来源：http://gjn.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://myt.jqgfzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fpa.gaohongyu789.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ihl.ehwqpu.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bvx.snrcjt.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jpd.0kj1m.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rgf.yuxming.cn


<!-- 参考信息 -->