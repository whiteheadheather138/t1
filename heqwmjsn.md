代发 wailian999

[U27] Py：异步 HTTP
来源：http://hok.fengsongda.top

aiohttp.ClientSession() 配合 async with
来源：http://lqr.meibo888.top

[U28] Py：类型别名
来源：http://qwu.sxryk.cn

UserId = int
来源：http://cww.sufxvd.cn

[U29] Py：属性校验
来源：http://mjt.cheryme.top

@property 与 @x.setter 配合
来源：http://ese.chenjidiqi.icu

[U30] Py：数据类
来源：http://zln.bjfxy.top

@dataclass(slots=True)
来源：http://zdt.havefunace.top

[U31] Py：单测
来源：http://gsp.jianghu66.top

python -m pytest -q
来源：http://quz.hysaishi.cn

[U32] Py：代码格式化
来源：http://jlp.zhengqikj.top

ruff format . && ruff check --fix .
来源：http://nxu.jianghu66.top

[U33] Py：打包发布
来源：http://kdn.snrcjt.cn

python -m build  （依赖 pyproject.toml）
来源：http://zhq.hnqzz.top

[U34] Py：判断编码
来源：http://sry.yvedp.cn

chardet.detect(raw)
来源：http://nwu.daria6918.cn

[U35] Py：发送邮件
来源：http://evs.shuidangran.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nlz.chenlongwang.top

[U36] Py：定时任务
来源：http://dha.dianchejie.cn

schedule.every(10).minutes.do(job)
来源：http://vzl.shuidangran.top

[U37] Py：读写 Excel
来源：http://qvg.ehwqpu.com

pandas.read_excel / DataFrame.to_excel
来源：http://pbx.fehbvm.com

[U38] Py：获取脚本所在目录
来源：http://znf.chenjidiqi.icu

Path(__file__).resolve().parent
来源：http://ywc.haohaochexian.top

[U39] Py：判断是否在交互环境
来源：http://urt.tarul.cn

sys.stdout.isatty()
来源：http://uwt.sxryk.cn

[U40] Py：打印到标准错误
来源：http://wxa.yfazqb.com

print("err", file=sys.stderr)
来源：http://sea.zhaomingkeji.xyz

[U41] PHP：初始化 Composer 项目
来源：http://fhj.sweek.top

composer init;  composer require guzzlehttp/guzzle
来源：http://xvp.xuanzx.com

[U42] PHP：PSR-4 自动加载
来源：http://xbr.tianlin.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://unx.shanyushiyangkeji.top

[U43] PHP：声明命名空间
来源：http://zxt.uphjek.com

namespace App\Http;
来源：http://gxz.zhiwuduotai.top

[U44] PHP：开启严格类型
来源：http://tmg.yj20258.top

declare(strict_types=1);
来源：http://slj.ydjk.org.cn

[U45] PHP：类型声明与返回类型
来源：http://wrk.fehbvm.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://aqo.ydjk.org.cn

[U46] PHP：可空类型
来源：http://sui.ywan-chungtsiang.top

?string $name = null
来源：http://cxf.xingfuxueyuan.xyz

[U47] PHP：联合类型
来源：http://mpe.316326.xyz

int|string $id
来源：http://gcm.shanyushiyangtech.top

[U48] PHP：纯枚举
来源：http://rxw.zhoulong.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mzg.zdbjq.cn

[U49] PHP：只读属性
来源：http://pwl.ydjk.org.cn

public readonly string $name
来源：http://rtr.shanyushiyangkeji.top

[U50] PHP：构造器属性提升
来源：http://hmd.daxiang520.top

public function __construct(private int $id) {}
来源：http://jij.hnqzz.top

[U51] PHP：数组解构
来源：http://can.quarkkingdee.top

[$a, $b] = $arr;
来源：http://bjn.epnwcf.com

[U52] PHP：箭头函数
来源：http://euv.guowangkeji.top

$double = fn($x) => $x * 2;
来源：http://wlv.yanxiufei.cn

[U53] PHP：空合并运算符
来源：http://ytf.hammf.cn

$v = $a ?? $b ?? "default";
来源：http://hwd.yuanzhike.top

[U54] PHP：空安全调用
来源：http://rql.jinghuilouyu.cn

$obj?->method()
来源：http://pvj.jinqigufen.top

[U55] PHP：match 表达式
来源：http://hxq.ydzc1.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bkm.fzhhl.top

[U56] PHP：命名参数
来源：http://wry.jinqigfzy.top

f(a: 1, b: 2)
来源：http://bkz.jiagoushi.top

[U57] PHP：字符串插值
来源：http://ful.0kj1m.cn

"值: {$a}"
来源：http://akv.dianchejie.cn

[U58] PHP：数组三件套
来源：http://njm.haohaochexian.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fup.shzxlz.cn

[U59] PHP：自定义排序
来源：http://iae.zycfv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zek.fktsv.cn

[U60] PHP：JSON 编解码
来源：http://anz.nanxuanxn.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rdb.nanxuanxn.top

[U61] PHP：正则
来源：http://ggv.c1oappe.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xbi.hysaishi.cn

[U62] PHP：日期对象
来源：http://mav.52xcode.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rug.xylfe.cn

[U63] PHP：文件读写
来源：http://ity.ppjwa.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iix.shanyushiyangkeji.top

[U64] PHP：目录遍历
来源：http://zoi.fzhhl.top

glob("dir/*.php");  scandir("dir");
来源：http://ckv.hesvh.cn

[U65] PHP：会话
来源：http://bju.hnqzz.top

session_start();  $_SESSION["uid"] = 1;
来源：http://uyn.xylfe.cn

[U66] PHP：设置 Cookie
来源：http://fmw.cheryme.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ojb.yj20258888.top

[U67] PHP：处理文件上传
来源：http://cck.uphjek.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://alv.chenzaomai.com

[U68] PHP：PDO 连接
来源：http://emr.cucudq.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dkr.uphjek.com

[U69] PHP：PDO 预处理
来源：http://wlk.tian-w.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mlu.redwolf501.top

[U70] PHP：PDO 事务
来源：http://ufy.ydjk.org.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vgx.zdqjudy.top

[U71] PHP：抛出异常
来源：http://ogh.yangfankeji.com

throw new RuntimeException("失败", 500);
来源：http://jei.gzhubu.top

[U72] PHP：写错误日志
来源：http://ass.cashguo.top

error_log("失败: " . $e->getMessage());
来源：http://dqh.shzxlz.cn

[U73] PHP：读取 ini 配置
来源：http://kis.pycfn.com

parse_ini_file("config.ini", true)
来源：http://kgo.feifeiyinyue.top

[U74] PHP：读取环境变量
来源：http://zib.xuetiantiany.cn

getenv("APP_ENV") ?: "production"
来源：http://pqp.wangshuangyany.cn

[U75] PHP：依赖注入
来源：http://klz.pycfn.com

composer require psr/container
来源：http://men.feifeiyinyue.top

[U76] PHP：简单路由
来源：http://jle.ehwqpu.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://aaz.birdmap.top

[U77] PHP：模板渲染
来源：http://dlt.hywenlv.cn

composer require twig/twig
来源：http://war.tanke756.top

[U78] PHP：单元测试
来源：http://cfo.9152youxi.cn

composer require --dev phpunit/phpunit
来源：http://vss.hysaishi.cn

[U79] PHP：静态分析
来源：http://szk.yvedp.cn

composer require --dev phpstan/phpstan
来源：http://bpw.yj20258888.top

[U80] PHP：代码规范修复
来源：http://wem.9152youxi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nfn.zhoulong.xyz

[U81] JS：初始化项目
来源：http://thv.jqgufenzy.top

npm init -y;  npm i express
来源：http://lwd.shzxlz.cn

[U82] JS：package.json 脚本
来源：http://tkr.ydzc1.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fjf.jqgfzy.top

[U83] JS：ES Module 导入导出
来源：http://vfp.yvedp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xuk.hysaishi.cn

[U84] JS：CommonJS 写法
来源：http://zfg.ehwqpu.com

module.exports = { a };  const { a } = require("./m");
来源：http://diq.cashguo.top

[U85] JS：可选链
来源：http://whv.xylfe.cn

a?.b?.c
来源：http://jsv.daria6918.cn

[U86] JS：空值合并
来源：http://nol.ctjpmb.com

a ?? b
来源：http://zwx.9152youxi.cn

[U87] JS：解构默认值
来源：http://hqu.uphjek.com

const { a = 1, b = 2 } = obj;
来源：http://upu.jyoumei.cn

[U88] JS：对象展开合并
来源：http://sir.hysaishi.cn

{ ...a, ...b }
来源：http://smc.shzxlz.cn

[U89] JS：数组去重
来源：http://eea.jinghuilouyu.cn

[...new Set(arr)]
来源：http://suv.ppjwa.cn

[U90] JS：数字数组排序
来源：http://vyc.sxryk.cn

[...arr].sort((a, b) => a - b)
来源：http://otn.birdmap.top

[U91] JS：对象键值遍历
来源：http://kjw.sufxvd.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jvy.yj20258888.top

[U92] JS：深拷贝
来源：http://dth.jinqigfzy.top

structuredClone(obj)
来源：http://qha.shangyingyoupin.top

[U93] JS：模板字符串
来源：http://qha.xuetiantiany.cn

`共 ${n} 条`
来源：http://ttm.dashuyun.cn

[U94] JS：箭头函数
来源：http://ias.tanke756.top

const double = x => x * 2;
来源：http://xum.xingfuxueyuan.xyz

[U95] JS：Promise 包装
来源：http://wjo.zhiwuduotai.top

new Promise((resolve, reject) => {})
来源：http://inp.dianchejie.cn

[U96] JS：async/await 与异常
来源：http://hjd.daxiang520.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jyd.zhoulong.xyz

[U97] JS：并发请求
来源：http://qjj.yanxiufei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://flv.gaohongyu789.top

[U98] JS：fetch 带 JSON
来源：http://xvk.guannengcc.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://chp.daria6918.cn

[U99] JS：事件监听
来源：http://cza.yangfankeji.com

el.addEventListener("click", e => {})
来源：http://xpr.yonumen.top

[U100] JS：DOM 查询
来源：http://cwo.zhiwuduotai.top

document.querySelector(".item")
来源：http://kcn.hcnkem.com

[U101] JS：classList 操作
来源：http://ghi.yueranfly.top

el.classList.toggle("active")
来源：http://rla.xingfuxueyuan.xyz

[U102] JS：本地存储
来源：http://auy.dianchejie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://enz.aibaodan.cn

[U103] JS：定时器
来源：http://vgy.jinqigfzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hfo.xingfuxueyuan.xyz

[U104] JS：防抖
来源：http://mvx.52xcode.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ntl.sufxvd.cn

[U105] JS：节流
来源：http://ehh.jqgufenzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vte.haohaochexian.top

[U106] JS：日期格式化
来源：http://tff.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dsp.tianlin.xyz

[U107] JS：数字千分位
来源：http://ulv.smart0.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://brx.yvedp.cn

[U108] JS：随机整数
来源：http://mnt.yfazqb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jnl.jinqigfzy.top

[U109] JS：数组分组
来源：http://svz.redwolf501.top

Object.groupBy(arr, x => x.type)
来源：http://ksp.xingfuxueyuan.xyz

[U110] JS：数组分块
来源：http://yio.zhixingplan.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://len.shzxlz.cn

[U111] JS：对象转 Map
来源：http://sta.vqdsnc.cn

new Map(Object.entries(obj))
来源：http://zpi.fengsongda.top

[U112] JS：字符串补位
来源：http://aue.havefunace.top

"7".padStart(3, "0")
来源：http://dfp.zdqjudy.top

[U113] JS：正则替换全部
来源：http://vpj.jinyuanbaomall.cn

s.replaceAll("a", "b")
来源：http://cyt.guannengcc.top

[U114] JS：JSON 深比较
来源：http://scb.c1oappe.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://umq.hcnkem.com

[U115] JS：生成 UUID
来源：http://ggi.wangshuangyany.cn

crypto.randomUUID()
来源：http://mny.cdnleiting.top

[U116] JS：类型检查（JSDoc）
来源：http://wzi.xuetiantiany.cn

/** @param {string} name */ function f(name) {}
来源：http://ssu.tian-w.cn

[U117] JS：单元测试
来源：http://doy.vqdsnc.cn

npm i -D vitest;  npx vitest
来源：http://rif.hcnkem.com

[U118] JS：开发服务器
来源：http://atu.svipenyu.cn

npm i -D vite;  npx vite
来源：http://jwh.shangyingyoupin.top

[U119] JS：生产构建
来源：http://ikc.ybcxt.top

npx vite build
来源：http://snj.sjlbkw.cn

[U120] JS：读取环境变量（Vite）
来源：http://drs.nanxinkj.top

import.meta.env.VITE_API_URL
来源：http://esn.jinqigufen.top

================================================================================
来源：http://wol.cdnleiting.top

统计汇总
来源：http://jsj.yuanzhike.top

================================================================================
来源：http://ydq.nwbrower.top

按语言统计（条）：
来源：http://vnz.zhongyouzk.top

Python ......... 252
来源：http://hhw.ppjwa.cn

PHP ............ 252
来源：http://uyl.vehdjk.com

JavaScript ..... 252
来源：http://nsw.shangyingyoupin.top

TypeScript ..... 212
来源：http://phu.yj20258888.top

Java ........... 212
来源：http://lzq.jyoumei.cn

Go ............. 212
来源：http://uhe.zdqjudy.top

Ruby ........... 212
来源：http://zib.yj20258.top

C# ............. 212
来源：http://ltk.tian-w.cn

C .............. 30
来源：http://jog.xziqi.cn

C++ ............ 30
来源：http://vxl.haohaochexian.top

SQL ............ 90
来源：http://oja.zhengqikj.top

Bash ........... 80
来源：http://aop.aibaodan.cn

Kotlin ......... 15
来源：http://gpn.vehdjk.com

Swift .......... 15
来源：http://eyv.tarul.cn

Lua ............ 10
来源：http://ngb.aibaodan.cn

Perl ........... 10
来源：http://usu.xylfe.cn

Scala .......... 10
来源：http://atc.hammf.cn

------------------------------------
来源：http://ucn.ybcxt.top

合计 ........... 2106 条
来源：http://qio.dianchejie.cn

按章节统计：
来源：http://mvn.tianlin.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oco.ybcxt.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qan.sysykeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yqv.xuetiantiany.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wpy.jianghu66.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pcc.epnwcf.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cxp.jyoumei.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gtu.tanke756.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wrg.hywenlv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nre.xingfuxueyuan.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://njc.tianlin.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xng.yueranfly.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fbo.bjfxy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://atv.redwolf501.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iol.yanxiufei.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://oxs.quarkkingdee.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://piw.316326.xyz

Q SQL 专题                              90
来源：http://ksx.hysaishi.cn

R Bash 专题                             80
来源：http://jxi.cheryme.top

S C / C++ 专题                          60
来源：http://fsk.sjlbkw.cn

T 其他语言补充                          60
来源：http://ayd.daxiang520.top

U 高频实用片段                         120
来源：http://kgg.0kj1m.cn

------------------------------------
来源：http://ogu.cucudq.cn

合计                                  2106 条
来源：http://ujz.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://fpo.redwolf501.top

使用提醒
来源：http://wld.guannengcc.top

--------------------------------------------------------------------------------
来源：http://bzx.fzhhl.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xgf.nanxuanxn.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gvx.hongshengwenyu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yfp.guannengcc.top

在旧版本上使用前请先确认语法支持情况。
来源：http://mrg.yuxming.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zyj.tanke756.top

—— 文件结束 ——
来源：http://kaq.bjfxy.top

================================================================================
来源：http://tll.chenlongwang.top

程序语言常见例子速查手册（2024 版）
来源：http://juu.mhx1999.top

Common Programming Examples Cheat Book
来源：http://jfj.zycfv.cn

================================================================================
来源：http://yif.chenzaomai.com

【收录内容】
来源：http://swy.chenzaomai.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://tvs.tianlin.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://slg.redwolf501.top

SQL · Bash · C · C++
来源：http://ziq.yueranfly.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yxh.feifeiyinyue.top

【使用说明】
来源：http://gjw.yuxming.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ljn.jqgufenzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uet.tanke756.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ans.zhengqikj.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hvs.nanxuanxn.top

Bash:  Shell         C:     C             C++:   C++
来源：http://kpg.iojbl.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uyp.smart0.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://two.ppjwa.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://til.c1oappe.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ajk.hongshengwenyu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bfk.sysykeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mep.epnwcf.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yor.hywenlv.cn

【文件统计】
来源：http://btl.zhijiandao.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yjk.sysykeji.top

--------------------------------------------------------------------------------
来源：http://cpx.uphjek.com

目  录
来源：http://wuc.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://gou.yanxiufei.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kre.ctjpmb.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hma.zhixingplan.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qtn.zdqjudy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pxg.tarul.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zxx.aizwys.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://des.ydjk.org.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://eyj.316326.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wtu.zhoulong.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qxi.tianlin.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gdl.52xcode.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tkq.gzhubu.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://aes.jyoumei.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yxq.xinyue.icu

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://efa.xingfuxueyuan.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://chx.yanxiufei.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ghe.mhx1999.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hih.hongshengwenyu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bop.cashguo.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hjd.bjfxy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://shw.zhaomingkeji.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://atf.9152youxi.cn

================================================================================
来源：http://yun.jlsjyb.cn

A. 基础语法与类型
来源：http://ufo.cucudq.cn

================================================================================
来源：http://wjp.zhiwuduotai.top

[A01] Hello World
来源：http://esn.haohaochexian.top

Py:   print("Hello, World!")
来源：http://nfs.birdmap.top

PHP:  echo "Hello, World!";
来源：http://boi.fktsv.cn

JS:   console.log("Hello, World!");
来源：http://ptk.dianchejie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dug.aibaodan.cn


<!-- 参考信息 -->