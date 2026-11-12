代发 wailian999

[U25] Py：CSV 按字典读
来源：http://zxn.fanxiaobao.xyz

csv.DictReader(f)
来源：http://tei.hesvh.cn

[U26] Py：并发下载
来源：http://lah.zhengqikj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ddn.chenzaomai.com

[U27] Py：异步 HTTP
来源：http://uwm.cucudq.cn

aiohttp.ClientSession() 配合 async with
来源：http://exv.wangshuangyany.cn

[U28] Py：类型别名
来源：http://vgo.tian-w.cn

UserId = int
来源：http://cke.jlsjyb.cn

[U29] Py：属性校验
来源：http://dhk.wangdashe.top

@property 与 @x.setter 配合
来源：http://gcg.daxiang520.top

[U30] Py：数据类
来源：http://pco.sufxvd.cn

@dataclass(slots=True)
来源：http://ouu.jyoumei.cn

[U31] Py：单测
来源：http://edo.aibaodan.cn

python -m pytest -q
来源：http://ent.316326.xyz

[U32] Py：代码格式化
来源：http://cer.shangyingyoupin.top

ruff format . && ruff check --fix .
来源：http://naa.smart0.xyz

[U33] Py：打包发布
来源：http://lae.ywan-chungtsiang.top

python -m build  （依赖 pyproject.toml）
来源：http://met.cheryme.top

[U34] Py：判断编码
来源：http://taz.shuidangran.top

chardet.detect(raw)
来源：http://qjm.ivvv.top

[U35] Py：发送邮件
来源：http://epu.hongshengwenyu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vwc.52xcode.cn

[U36] Py：定时任务
来源：http://pqy.nanxinkj.top

schedule.every(10).minutes.do(job)
来源：http://evg.nwbrower.top

[U37] Py：读写 Excel
来源：http://fth.chenlongwang.top

pandas.read_excel / DataFrame.to_excel
来源：http://imd.jinqigfzy.top

[U38] Py：获取脚本所在目录
来源：http://wmb.yfazqb.com

Path(__file__).resolve().parent
来源：http://kai.yj20258.top

[U39] Py：判断是否在交互环境
来源：http://xpy.smart0.xyz

sys.stdout.isatty()
来源：http://pes.yuxming.cn

[U40] Py：打印到标准错误
来源：http://ygb.yj20258888.top

print("err", file=sys.stderr)
来源：http://jqe.pengpengdd.cyou

[U41] PHP：初始化 Composer 项目
来源：http://ycu.epnwcf.com

composer init;  composer require guzzlehttp/guzzle
来源：http://gyl.ehwqpu.com

[U42] PHP：PSR-4 自动加载
来源：http://ftj.xuanzx.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tyt.nwbrower.top

[U43] PHP：声明命名空间
来源：http://uxr.jianghu66.top

namespace App\Http;
来源：http://fmh.0kj1m.cn

[U44] PHP：开启严格类型
来源：http://oub.xingfuxueyuan.xyz

declare(strict_types=1);
来源：http://ubu.yueranfly.top

[U45] PHP：类型声明与返回类型
来源：http://lmy.daxiang520.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://alp.zdbjq.cn

[U46] PHP：可空类型
来源：http://rmu.hammf.cn

?string $name = null
来源：http://lsq.ivvv.top

[U47] PHP：联合类型
来源：http://qcf.shanyushiyangkeji.top

int|string $id
来源：http://knq.meibo888.top

[U48] PHP：纯枚举
来源：http://rbq.birdmap.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xkw.andypj.xyz

[U49] PHP：只读属性
来源：http://yts.hfpthk.cn

public readonly string $name
来源：http://qqv.pycfn.com

[U50] PHP：构造器属性提升
来源：http://unj.hfpthk.cn

public function __construct(private int $id) {}
来源：http://zkc.hnxiangtu.top

[U51] PHP：数组解构
来源：http://dah.cashguo.top

[$a, $b] = $arr;
来源：http://vzs.hnxiangtu.top

[U52] PHP：箭头函数
来源：http://gpa.xinyue.icu

$double = fn($x) => $x * 2;
来源：http://qkg.jlsjyb.cn

[U53] PHP：空合并运算符
来源：http://jxd.jqgfzy.top

$v = $a ?? $b ?? "default";
来源：http://gnv.xinyue.icu

[U54] PHP：空安全调用
来源：http://hus.jyoumei.cn

$obj?->method()
来源：http://ajj.sweek.top

[U55] PHP：match 表达式
来源：http://bfm.bbcook.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rkz.ydzc1.top

[U56] PHP：命名参数
来源：http://gqo.sweek.top

f(a: 1, b: 2)
来源：http://ssi.ydjk.org.cn

[U57] PHP：字符串插值
来源：http://ufn.tianlin.xyz

"值: {$a}"
来源：http://oks.vehdjk.com

[U58] PHP：数组三件套
来源：http://ebu.ehwqpu.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jlf.gzhubu.top

[U59] PHP：自定义排序
来源：http://lga.nanxuanxn.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bho.fzhhl.top

[U60] PHP：JSON 编解码
来源：http://vzd.sysykeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://van.yonumen.top

[U61] PHP：正则
来源：http://keq.gogol.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lra.pycfn.com

[U62] PHP：日期对象
来源：http://yqs.fzhhl.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ary.zhiwuduotai.top

[U63] PHP：文件读写
来源：http://vop.quarkkingdee.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mqj.tian-w.cn

[U64] PHP：目录遍历
来源：http://dqg.daria6918.cn

glob("dir/*.php");  scandir("dir");
来源：http://rjg.meibo888.top

[U65] PHP：会话
来源：http://djw.wangdashe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://elz.meibo888.top

[U66] PHP：设置 Cookie
来源：http://air.yfazqb.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uug.52xcode.cn

[U67] PHP：处理文件上传
来源：http://rcw.wangdashe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://veq.xylfe.cn

[U68] PHP：PDO 连接
来源：http://igq.aibaodan.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gqn.fehbvm.com

[U69] PHP：PDO 预处理
来源：http://mgc.cqqwz.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xmt.cqqwz.cn

[U70] PHP：PDO 事务
来源：http://jmw.ivvv.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zyw.zhengqikj.top

[U71] PHP：抛出异常
来源：http://trv.c1oappe.top

throw new RuntimeException("失败", 500);
来源：http://vtd.xuetiantiany.cn

[U72] PHP：写错误日志
来源：http://may.epnwcf.com

error_log("失败: " . $e->getMessage());
来源：http://oxy.ydjk.org.cn

[U73] PHP：读取 ini 配置
来源：http://wuf.fzhhl.top

parse_ini_file("config.ini", true)
来源：http://cqu.aibaodan.cn

[U74] PHP：读取环境变量
来源：http://ser.uphjek.com

getenv("APP_ENV") ?: "production"
来源：http://ahj.zhaomingkeji.xyz

[U75] PHP：依赖注入
来源：http://aex.nanxinkj.top

composer require psr/container
来源：http://xhq.birdmap.top

[U76] PHP：简单路由
来源：http://vat.tianlin.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sen.xziqi.cn

[U77] PHP：模板渲染
来源：http://dxr.fehbvm.com

composer require twig/twig
来源：http://nrp.jqgufenzy.top

[U78] PHP：单元测试
来源：http://fdw.iojbl.cn

composer require --dev phpunit/phpunit
来源：http://csh.chenjidiqi.icu

[U79] PHP：静态分析
来源：http://mjj.zhengqikj.top

composer require --dev phpstan/phpstan
来源：http://qwf.hfpthk.cn

[U80] PHP：代码规范修复
来源：http://bte.zhengqikj.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rrf.redwolf501.top

[U81] JS：初始化项目
来源：http://tbz.yongpay.top

npm init -y;  npm i express
来源：http://nrb.nanxinkj.top

[U82] JS：package.json 脚本
来源：http://mog.zhaomingkeji.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bva.bjfxy.top

[U83] JS：ES Module 导入导出
来源：http://eoy.smart0.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://hki.fanxiaobao.xyz

[U84] JS：CommonJS 写法
来源：http://ljg.yj202588.top

module.exports = { a };  const { a } = require("./m");
来源：http://arf.wangshuangyany.cn

[U85] JS：可选链
来源：http://vqt.xuetiantiany.cn

a?.b?.c
来源：http://acq.xuetiantiany.cn

[U86] JS：空值合并
来源：http://cti.9152youxi.cn

a ?? b
来源：http://dwp.vehdjk.com

[U87] JS：解构默认值
来源：http://xfc.daria6918.cn

const { a = 1, b = 2 } = obj;
来源：http://hbx.xingfuxueyuan.xyz

[U88] JS：对象展开合并
来源：http://wsf.zdqjudy.top

{ ...a, ...b }
来源：http://hac.nanxuanxn.top

[U89] JS：数组去重
来源：http://xuf.cdnleiting.top

[...new Set(arr)]
来源：http://cyn.bjfxy.top

[U90] JS：数字数组排序
来源：http://bxt.xingfuxueyuan.xyz

[...arr].sort((a, b) => a - b)
来源：http://nya.havefunace.top

[U91] JS：对象键值遍历
来源：http://ish.dianchejie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://opu.guannengcc.top

[U92] JS：深拷贝
来源：http://pyi.xuetiantiany.cn

structuredClone(obj)
来源：http://lff.cucudq.cn

[U93] JS：模板字符串
来源：http://mhm.jqgufenzy.top

`共 ${n} 条`
来源：http://pgu.kuanghao11.cn

[U94] JS：箭头函数
来源：http://cbq.daria6918.cn

const double = x => x * 2;
来源：http://wde.hesvh.cn

[U95] JS：Promise 包装
来源：http://bss.cqqwz.cn

new Promise((resolve, reject) => {})
来源：http://aqg.shuidangran.top

[U96] JS：async/await 与异常
来源：http://jkz.wangshuangyany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://erp.0kj1m.cn

[U97] JS：并发请求
来源：http://cvr.daxiang520.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vvx.bbcook.cn

[U98] JS：fetch 带 JSON
来源：http://pgl.mhx1999.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ucb.gzhubu.top

[U99] JS：事件监听
来源：http://spr.shzxlz.cn

el.addEventListener("click", e => {})
来源：http://wwb.jinghuilouyu.cn

[U100] JS：DOM 查询
来源：http://wwb.feifeiyinyue.top

document.querySelector(".item")
来源：http://gkq.birdmap.top

[U101] JS：classList 操作
来源：http://htf.zhijiandao.cn

el.classList.toggle("active")
来源：http://lbw.cdnleiting.top

[U102] JS：本地存储
来源：http://mie.sjlbkw.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mgs.ivvv.top

[U103] JS：定时器
来源：http://kfy.daxiang520.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oqx.hysaishi.cn

[U104] JS：防抖
来源：http://ezj.yangfankeji.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uat.jinqigufen.top

[U105] JS：节流
来源：http://qdf.vehdjk.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rxe.cucudq.cn

[U106] JS：日期格式化
来源：http://cht.yueranfly.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tjo.zhengqikj.top

[U107] JS：数字千分位
来源：http://qqq.andypj.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qrt.zhijiandao.cn

[U108] JS：随机整数
来源：http://gih.birdmap.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pin.hfpthk.cn

[U109] JS：数组分组
来源：http://ylp.sweek.top

Object.groupBy(arr, x => x.type)
来源：http://nev.wangshuangyany.cn

[U110] JS：数组分块
来源：http://khp.zhoulong.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nmp.ydzc1.top

[U111] JS：对象转 Map
来源：http://kbl.yanxiufei.cn

new Map(Object.entries(obj))
来源：http://qdm.cdnleiting.top

[U112] JS：字符串补位
来源：http://uje.gaohongyu789.top

"7".padStart(3, "0")
来源：http://rmb.vqdsnc.cn

[U113] JS：正则替换全部
来源：http://xmc.yanxiufei.cn

s.replaceAll("a", "b")
来源：http://xnx.chenzaomai.com

[U114] JS：JSON 深比较
来源：http://bmv.shanyushiyangtech.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://laj.sweek.top

[U115] JS：生成 UUID
来源：http://eul.jianghu66.top

crypto.randomUUID()
来源：http://sgh.xingfuxueyuan.xyz

[U116] JS：类型检查（JSDoc）
来源：http://rce.redwolf501.top

/** @param {string} name */ function f(name) {}
来源：http://klv.chenzaomai.com

[U117] JS：单元测试
来源：http://rpf.hnxiangtu.top

npm i -D vitest;  npx vitest
来源：http://wya.zhixingplan.top

[U118] JS：开发服务器
来源：http://vbn.sysykeji.top

npm i -D vite;  npx vite
来源：http://vbm.cashguo.top

[U119] JS：生产构建
来源：http://whf.chenzaomai.com

npx vite build
来源：http://qdj.ywan-chungtsiang.top

[U120] JS：读取环境变量（Vite）
来源：http://uai.svipenyu.cn

import.meta.env.VITE_API_URL
来源：http://ftz.haohaochexian.top

================================================================================
来源：http://cyu.yongpay.top

统计汇总
来源：http://ahz.sweek.top

================================================================================
来源：http://xeu.xingfuxueyuan.xyz

按语言统计（条）：
来源：http://msd.gotoacloud.top

Python ......... 252
来源：http://nhw.fehbvm.com

PHP ............ 252
来源：http://ees.hammf.cn

JavaScript ..... 252
来源：http://vlb.ybcxt.top

TypeScript ..... 212
来源：http://shv.chenlongwang.top

Java ........... 212
来源：http://vyx.ydzc1.top

Go ............. 212
来源：http://aqo.0kj1m.cn

Ruby ........... 212
来源：http://jys.redwolf501.top

C# ............. 212
来源：http://toy.jlsjyb.cn

C .............. 30
来源：http://weg.sysykeji.top

C++ ............ 30
来源：http://jsv.yuxming.cn

SQL ............ 90
来源：http://vix.hesvh.cn

Bash ........... 80
来源：http://pku.pengpengdd.cyou

Kotlin ......... 15
来源：http://hnd.yonumen.top

Swift .......... 15
来源：http://zbj.ydzc1.top

Lua ............ 10
来源：http://vir.zhaomingkeji.xyz

Perl ........... 10
来源：http://wkr.chenlongwang.top

Scala .......... 10
来源：http://mrq.zhoulong.xyz

------------------------------------
来源：http://cgy.yuxming.cn

合计 ........... 2106 条
来源：http://tyk.ydjk.org.cn

按章节统计：
来源：http://img.haohaochexian.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gnz.nanxuanxn.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nvx.fanxiaobao.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qck.tanke756.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ocd.shanyushiyangkeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://riy.xingfuxueyuan.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mpr.xziqi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wfk.bjfxy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lhi.uphjek.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://knx.yangfankeji.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wvp.nwbrower.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cgm.epnwcf.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zxi.dashuyun.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rbl.hesvh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zvp.jinqigufen.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bjg.iojbl.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lve.zhijiandao.cn

Q SQL 专题                              90
来源：http://rsc.uphjek.com

R Bash 专题                             80
来源：http://ymk.xziqi.cn

S C / C++ 专题                          60
来源：http://ztd.ivvv.top

T 其他语言补充                          60
来源：http://bpv.jiagoushi.top

U 高频实用片段                         120
来源：http://xah.hcnkem.com

------------------------------------
来源：http://xjq.kuanghao11.cn

合计                                  2106 条
来源：http://xim.yfazqb.com

--------------------------------------------------------------------------------
来源：http://rak.yvedp.cn

使用提醒
来源：http://ybd.hnqzz.top

--------------------------------------------------------------------------------
来源：http://rkl.fanxiaobao.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hgj.vehdjk.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fdj.yfazqb.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://isp.ydzc1.top

在旧版本上使用前请先确认语法支持情况。
来源：http://apa.zhoulong.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://irs.wangshuangyany.cn

—— 文件结束 ——
来源：http://cqx.pycfn.com

================================================================================
来源：http://bde.fehbvm.com

程序语言常见例子速查手册（2024 版）
来源：http://epq.tianlin.xyz

Common Programming Examples Cheat Book
来源：http://iac.zycfv.cn

================================================================================
来源：http://waw.wangdashe.top

【收录内容】
来源：http://vsr.gaohongyu789.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://cog.yonumen.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pih.zhixingplan.top

SQL · Bash · C · C++
来源：http://slv.cqqwz.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lus.zycfv.cn

【使用说明】
来源：http://dww.birdmap.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://giy.ppjwa.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yfg.0kj1m.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wve.jinghuilouyu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://saz.kuanghao11.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://uhr.nanxuanxn.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eqp.gaohongyu789.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://epj.birdmap.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tpo.ywan-chungtsiang.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pel.c1oappe.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://puu.feifeiyinyue.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jqe.zhixingplan.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ait.daria6918.cn

【文件统计】
来源：http://gwe.svipenyu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ufq.daxiang520.top

--------------------------------------------------------------------------------
来源：http://vhr.xuetiantiany.cn

目  录
来源：http://rov.hesvh.cn

--------------------------------------------------------------------------------
来源：http://xdp.epnwcf.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jwq.gogol.net.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wue.xylfe.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qso.ywan-chungtsiang.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ztd.jqgfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zch.shanyushiyangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wkl.cqqwz.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zzf.wangshuangyany.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cbb.shzxlz.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wyy.tian-w.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://psc.nwbrower.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://llp.ybcxt.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qei.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wjq.jiagoushi.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://okr.zhixingplan.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mom.gaohongyu789.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sha.gogol.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ftl.xuanzx.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://vwv.jinghuilouyu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vgg.nanxuanxn.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ufv.bjfxy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cko.zdqjudy.top

================================================================================
来源：http://ztc.fanxiaobao.xyz

A. 基础语法与类型
来源：http://xcs.cdnleiting.top

================================================================================
来源：http://qck.yuanzhike.top

[A01] Hello World
来源：http://noh.smart0.xyz


<!-- 参考信息 -->