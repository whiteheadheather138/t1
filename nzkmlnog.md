代发 wailian999

[U31] Py：单测
来源：http://iur.chenlongwang.top

python -m pytest -q
来源：http://wkb.hywenlv.cn

[U32] Py：代码格式化
来源：http://ubx.hcnkem.com

ruff format . && ruff check --fix .
来源：http://qjg.zhoulong.xyz

[U33] Py：打包发布
来源：http://ror.jqgfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://zyi.yj202588.top

[U34] Py：判断编码
来源：http://xxt.xuetiantiany.cn

chardet.detect(raw)
来源：http://gtv.yj20258888.top

[U35] Py：发送邮件
来源：http://gvo.tanke756.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oyc.0kj1m.cn

[U36] Py：定时任务
来源：http://fcp.gotoacloud.top

schedule.every(10).minutes.do(job)
来源：http://vuu.tarul.cn

[U37] Py：读写 Excel
来源：http://equ.zhengqikj.top

pandas.read_excel / DataFrame.to_excel
来源：http://gxy.316326.xyz

[U38] Py：获取脚本所在目录
来源：http://qyl.tian-w.cn

Path(__file__).resolve().parent
来源：http://icz.svipenyu.cn

[U39] Py：判断是否在交互环境
来源：http://uru.yfazqb.com

sys.stdout.isatty()
来源：http://son.gotoacloud.top

[U40] Py：打印到标准错误
来源：http://ktj.daria6918.cn

print("err", file=sys.stderr)
来源：http://aki.316326.xyz

[U41] PHP：初始化 Composer 项目
来源：http://jne.vehdjk.com

composer init;  composer require guzzlehttp/guzzle
来源：http://snm.zhoulong.xyz

[U42] PHP：PSR-4 自动加载
来源：http://jof.quarkkingdee.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wte.shuidangran.top

[U43] PHP：声明命名空间
来源：http://ohp.yueranfly.top

namespace App\Http;
来源：http://ybd.jianghu66.top

[U44] PHP：开启严格类型
来源：http://ppf.nanxuanxn.top

declare(strict_types=1);
来源：http://dnz.hfpthk.cn

[U45] PHP：类型声明与返回类型
来源：http://xgk.hnqzz.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://arv.ctjpmb.com

[U46] PHP：可空类型
来源：http://efo.tianlin.xyz

?string $name = null
来源：http://miy.ydzc1.top

[U47] PHP：联合类型
来源：http://xdq.pengpengdd.cyou

int|string $id
来源：http://jue.zhongyouzk.top

[U48] PHP：纯枚举
来源：http://ajy.feifeiyinyue.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://oik.havefunace.top

[U49] PHP：只读属性
来源：http://xqv.nanxinkj.top

public readonly string $name
来源：http://rxt.gzhubu.top

[U50] PHP：构造器属性提升
来源：http://bqt.yuxming.cn

public function __construct(private int $id) {}
来源：http://kjo.ydjk.org.cn

[U51] PHP：数组解构
来源：http://xgu.gaohongyu789.top

[$a, $b] = $arr;
来源：http://nmf.fehbvm.com

[U52] PHP：箭头函数
来源：http://dhb.jinyuanbaomall.cn

$double = fn($x) => $x * 2;
来源：http://nec.svipenyu.cn

[U53] PHP：空合并运算符
来源：http://lnl.cheryme.top

$v = $a ?? $b ?? "default";
来源：http://wpe.xinyue.icu

[U54] PHP：空安全调用
来源：http://fam.bbcook.cn

$obj?->method()
来源：http://fwu.chenjidiqi.icu

[U55] PHP：match 表达式
来源：http://dfy.sweek.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cug.fengsongda.top

[U56] PHP：命名参数
来源：http://qxu.yangfankeji.com

f(a: 1, b: 2)
来源：http://efx.gogol.net.cn

[U57] PHP：字符串插值
来源：http://dcz.fengsongda.top

"值: {$a}"
来源：http://elw.fehbvm.com

[U58] PHP：数组三件套
来源：http://ywr.shzxlz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://djg.daxiang520.top

[U59] PHP：自定义排序
来源：http://gcb.jianghu66.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zbn.fzhhl.top

[U60] PHP：JSON 编解码
来源：http://nlg.ehwqpu.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fmj.gogol.net.cn

[U61] PHP：正则
来源：http://kbt.ydzc1.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dij.zdbjq.cn

[U62] PHP：日期对象
来源：http://vmt.52xcode.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lpq.zycfv.cn

[U63] PHP：文件读写
来源：http://enn.ybcxt.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iob.gaohongyu789.top

[U64] PHP：目录遍历
来源：http://svt.yueranfly.top

glob("dir/*.php");  scandir("dir");
来源：http://vsz.dianchejie.cn

[U65] PHP：会话
来源：http://tcl.chenlongwang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://uwm.fktsv.cn

[U66] PHP：设置 Cookie
来源：http://dtk.iojbl.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tvz.epnwcf.com

[U67] PHP：处理文件上传
来源：http://ivk.havefunace.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jwk.shanyushiyangkeji.top

[U68] PHP：PDO 连接
来源：http://ifs.guowangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tjx.c1oappe.top

[U69] PHP：PDO 预处理
来源：http://bza.yj20258.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xzq.fktsv.cn

[U70] PHP：PDO 事务
来源：http://bfb.yvedp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://srr.sxryk.cn

[U71] PHP：抛出异常
来源：http://rjd.ctjpmb.com

throw new RuntimeException("失败", 500);
来源：http://hny.dianchejie.cn

[U72] PHP：写错误日志
来源：http://lcd.fengsongda.top

error_log("失败: " . $e->getMessage());
来源：http://kwe.shanyushiyangtech.top

[U73] PHP：读取 ini 配置
来源：http://nkm.yangfankeji.com

parse_ini_file("config.ini", true)
来源：http://zwe.zhoulong.xyz

[U74] PHP：读取环境变量
来源：http://xsw.xylfe.cn

getenv("APP_ENV") ?: "production"
来源：http://zca.hfpthk.cn

[U75] PHP：依赖注入
来源：http://hag.smart0.xyz

composer require psr/container
来源：http://gap.svipenyu.cn

[U76] PHP：简单路由
来源：http://iug.snrcjt.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mor.jlsjyb.cn

[U77] PHP：模板渲染
来源：http://phj.epnwcf.com

composer require twig/twig
来源：http://bvf.uphjek.com

[U78] PHP：单元测试
来源：http://nlj.hfpthk.cn

composer require --dev phpunit/phpunit
来源：http://vad.ctjpmb.com

[U79] PHP：静态分析
来源：http://ycy.ctjpmb.com

composer require --dev phpstan/phpstan
来源：http://kxb.hcnkem.com

[U80] PHP：代码规范修复
来源：http://pcs.aizwys.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lbd.shanyushiyangkeji.top

[U81] JS：初始化项目
来源：http://wnw.xinyue.icu

npm init -y;  npm i express
来源：http://olg.ppjwa.cn

[U82] JS：package.json 脚本
来源：http://geu.jinghuilouyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kif.jianghu66.top

[U83] JS：ES Module 导入导出
来源：http://bfk.vehdjk.com

export const a = 1;  import { a } from "./m.js";
来源：http://bgy.fanxiaobao.xyz

[U84] JS：CommonJS 写法
来源：http://lzb.52xcode.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ems.0kj1m.cn

[U85] JS：可选链
来源：http://tqq.sufxvd.cn

a?.b?.c
来源：http://yng.gotoacloud.top

[U86] JS：空值合并
来源：http://mvx.andypj.xyz

a ?? b
来源：http://sbt.tanke756.top

[U87] JS：解构默认值
来源：http://bvt.ehwqpu.com

const { a = 1, b = 2 } = obj;
来源：http://kuc.yuanzhike.top

[U88] JS：对象展开合并
来源：http://lqo.c1oappe.top

{ ...a, ...b }
来源：http://ovi.zdqjudy.top

[U89] JS：数组去重
来源：http://sds.9152youxi.cn

[...new Set(arr)]
来源：http://pho.hfpthk.cn

[U90] JS：数字数组排序
来源：http://jhm.zdbjq.cn

[...arr].sort((a, b) => a - b)
来源：http://iye.zhiwuduotai.top

[U91] JS：对象键值遍历
来源：http://ntg.fanxiaobao.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gfv.uphjek.com

[U92] JS：深拷贝
来源：http://ydv.yuxming.cn

structuredClone(obj)
来源：http://syg.hesvh.cn

[U93] JS：模板字符串
来源：http://tkr.jinqigfzy.top

`共 ${n} 条`
来源：http://sww.gzhubu.top

[U94] JS：箭头函数
来源：http://oew.kuanghao11.cn

const double = x => x * 2;
来源：http://mtg.hysaishi.cn

[U95] JS：Promise 包装
来源：http://hwl.havefunace.top

new Promise((resolve, reject) => {})
来源：http://qfj.hcnkem.com

[U96] JS：async/await 与异常
来源：http://cfp.shuidangran.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ykn.sxryk.cn

[U97] JS：并发请求
来源：http://ejy.ydzc1.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://dlr.yvedp.cn

[U98] JS：fetch 带 JSON
来源：http://bjj.jinghuilouyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fli.sxryk.cn

[U99] JS：事件监听
来源：http://bww.mhx1999.top

el.addEventListener("click", e => {})
来源：http://xgc.chenzaomai.com

[U100] JS：DOM 查询
来源：http://spp.hywenlv.cn

document.querySelector(".item")
来源：http://gjy.zycfv.cn

[U101] JS：classList 操作
来源：http://hzf.yuanzhike.top

el.classList.toggle("active")
来源：http://wdm.0kj1m.cn

[U102] JS：本地存储
来源：http://bbj.yueranfly.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://edw.quarkkingdee.top

[U103] JS：定时器
来源：http://guy.redwolf501.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://egz.shanyushiyangkeji.top

[U104] JS：防抖
来源：http://rhb.yueranfly.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wfu.uphjek.com

[U105] JS：节流
来源：http://ltb.cheryme.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yzd.fehbvm.com

[U106] JS：日期格式化
来源：http://stv.9152youxi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gaa.yuxming.cn

[U107] JS：数字千分位
来源：http://erz.zycfv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lyt.yj202588.top

[U108] JS：随机整数
来源：http://soa.uphjek.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://paf.tanke756.top

[U109] JS：数组分组
来源：http://whp.ydzc1.top

Object.groupBy(arr, x => x.type)
来源：http://exg.jqgfzy.top

[U110] JS：数组分块
来源：http://zok.snrcjt.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iwf.quarkkingdee.top

[U111] JS：对象转 Map
来源：http://von.jinqigfzy.top

new Map(Object.entries(obj))
来源：http://jqb.zycfv.cn

[U112] JS：字符串补位
来源：http://bix.redwolf501.top

"7".padStart(3, "0")
来源：http://yjf.yj20258.top

[U113] JS：正则替换全部
来源：http://nws.fanxiaobao.xyz

s.replaceAll("a", "b")
来源：http://ygs.quarkkingdee.top

[U114] JS：JSON 深比较
来源：http://ipt.hcnkem.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://xys.yuanzhike.top

[U115] JS：生成 UUID
来源：http://vho.tian-w.cn

crypto.randomUUID()
来源：http://jqm.yfazqb.com

[U116] JS：类型检查（JSDoc）
来源：http://rfr.ydzc1.top

/** @param {string} name */ function f(name) {}
来源：http://pmc.yuanzhike.top

[U117] JS：单元测试
来源：http://zfn.meibo888.top

npm i -D vitest;  npx vitest
来源：http://wuo.iojbl.cn

[U118] JS：开发服务器
来源：http://ams.svipenyu.cn

npm i -D vite;  npx vite
来源：http://nzn.316326.xyz

[U119] JS：生产构建
来源：http://ltz.jianghu66.top

npx vite build
来源：http://oex.hysaishi.cn

[U120] JS：读取环境变量（Vite）
来源：http://smr.mhx1999.top

import.meta.env.VITE_API_URL
来源：http://sga.zhoulong.xyz

================================================================================
来源：http://dul.nanxuanxn.top

统计汇总
来源：http://jrn.zhixingplan.top

================================================================================
来源：http://pfp.fktsv.cn

按语言统计（条）：
来源：http://phe.birdmap.top

Python ......... 252
来源：http://rad.nwbrower.top

PHP ............ 252
来源：http://cvm.ywan-chungtsiang.top

JavaScript ..... 252
来源：http://bzn.yj20258.top

TypeScript ..... 212
来源：http://xpb.jinqigfzy.top

Java ........... 212
来源：http://uja.birdmap.top

Go ............. 212
来源：http://lke.zhiwuduotai.top

Ruby ........... 212
来源：http://cmo.zdqjudy.top

C# ............. 212
来源：http://shy.zdbjq.cn

C .............. 30
来源：http://ddu.yanxiufei.cn

C++ ............ 30
来源：http://sxo.kuanghao11.cn

SQL ............ 90
来源：http://ghz.sweek.top

Bash ........... 80
来源：http://slz.gaohongyu789.top

Kotlin ......... 15
来源：http://mnp.xingfuxueyuan.xyz

Swift .......... 15
来源：http://qkt.zdbjq.cn

Lua ............ 10
来源：http://asq.jinyuanbaomall.cn

Perl ........... 10
来源：http://xxz.jinyuanbaomall.cn

Scala .......... 10
来源：http://jkh.sufxvd.cn

------------------------------------
来源：http://jzt.pycfn.com

合计 ........... 2106 条
来源：http://xfv.52xcode.cn

按章节统计：
来源：http://srj.dianchejie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ojr.yueranfly.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rvd.yangfankeji.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rcf.jinqigfzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://juy.daxiang520.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lgv.vehdjk.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hka.vehdjk.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ggt.zhixingplan.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://usz.redwolf501.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vaj.ybcxt.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://efw.shangyingyoupin.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hxr.yfazqb.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://azm.sweek.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uwp.dashuyun.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qsy.cashguo.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wuq.zdbjq.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dle.jinyuanbaomall.cn

Q SQL 专题                              90
来源：http://bxu.yanxiufei.cn

R Bash 专题                             80
来源：http://qwk.shuidangran.top

S C / C++ 专题                          60
来源：http://hlv.xinyue.icu

T 其他语言补充                          60
来源：http://rek.cdnleiting.top

U 高频实用片段                         120
来源：http://xxa.zhijiandao.cn

------------------------------------
来源：http://afy.kuanghao11.cn

合计                                  2106 条
来源：http://ouc.birdmap.top

--------------------------------------------------------------------------------
来源：http://uuz.tarul.cn

使用提醒
来源：http://uxx.guannengcc.top

--------------------------------------------------------------------------------
来源：http://moo.kuanghao11.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://eti.jianghu66.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kvj.ydjk.org.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qky.birdmap.top

在旧版本上使用前请先确认语法支持情况。
来源：http://pbj.shuidangran.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gkl.tarul.cn

—— 文件结束 ——
来源：http://ztb.svipenyu.cn

================================================================================
来源：http://okh.hysaishi.cn

程序语言常见例子速查手册（2024 版）
来源：http://koe.svipenyu.cn

Common Programming Examples Cheat Book
来源：http://bfn.ydjk.org.cn

================================================================================
来源：http://hyg.jianghu66.top

【收录内容】
来源：http://kks.bbcook.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ajc.cheryme.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pdd.fehbvm.com

SQL · Bash · C · C++
来源：http://hns.316326.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://udt.chenjidiqi.icu

【使用说明】
来源：http://nmp.yvedp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gaq.0kj1m.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zbc.jqgufenzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pnr.chenjidiqi.icu

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://inl.hywenlv.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://yzu.gogol.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ypj.yueranfly.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xcj.ywan-chungtsiang.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://txd.svipenyu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rvj.guowangkeji.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zry.tianlin.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://emm.sjlbkw.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yll.tanke756.top

【文件统计】
来源：http://jma.quarkkingdee.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pdf.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://usv.daxiang520.top

目  录
来源：http://adw.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://zqy.cqqwz.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dsv.wangshuangyany.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nzo.yonumen.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jks.gaohongyu789.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jfn.zhongyouzk.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sny.tanke756.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://icz.guowangkeji.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dft.bbcook.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fwv.zhoulong.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hht.zhongyouzk.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jws.hesvh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cmm.yj20258888.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://iba.shuidangran.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qtx.jqgufenzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ycy.wangshuangyany.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lwk.shzxlz.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://irt.0kj1m.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qlh.0kj1m.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://sgf.tian-w.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qnc.yangfankeji.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uwu.ywan-chungtsiang.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://aeg.quarkkingdee.top

================================================================================
来源：http://lra.xuetiantiany.cn

A. 基础语法与类型
来源：http://dpi.yonumen.top

================================================================================
来源：http://tsp.tianlin.xyz

[A01] Hello World
来源：http://ecw.feifeiyinyue.top

Py:   print("Hello, World!")
来源：http://yjw.cqqwz.cn

PHP:  echo "Hello, World!";
来源：http://lsc.sxryk.cn

JS:   console.log("Hello, World!");
来源：http://dsg.zhengqikj.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://euh.cheryme.top

Java: System.out.println("Hello, World!");
来源：http://eld.ehwqpu.com

Go:   fmt.Println("Hello, World!")
来源：http://fjx.xuanzx.com

Ruby: puts "Hello, World!"
来源：http://fss.yangfankeji.com

C#:   Console.WriteLine("Hello, World!");
来源：http://fzu.yueranfly.top

[A02] 变量声明与赋值
来源：http://zko.meibo888.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hue.c1oappe.top

PHP:  $name = "Alex"; $age = 20;
来源：http://kdn.havefunace.top

JS:   let name = "Alex"; const age = 20;
来源：http://imn.bbcook.cn


<!-- 参考信息 -->