代发 wailian999

[U31] Py：单测
来源：http://dbv.shuidangran.top

python -m pytest -q
来源：http://eqh.yuxming.cn

[U32] Py：代码格式化
来源：http://ave.yj20258888.top

ruff format . && ruff check --fix .
来源：http://vbu.bbcook.cn

[U33] Py：打包发布
来源：http://jad.bjfxy.top

python -m build  （依赖 pyproject.toml）
来源：http://cxk.xylfe.cn

[U34] Py：判断编码
来源：http://ctg.sxryk.cn

chardet.detect(raw)
来源：http://juh.tarul.cn

[U35] Py：发送邮件
来源：http://jnv.ydjk.org.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hjd.quarkkingdee.top

[U36] Py：定时任务
来源：http://qja.ydjk.org.cn

schedule.every(10).minutes.do(job)
来源：http://dwr.sysykeji.top

[U37] Py：读写 Excel
来源：http://nms.jinqigufen.top

pandas.read_excel / DataFrame.to_excel
来源：http://mzr.ydzc1.top

[U38] Py：获取脚本所在目录
来源：http://ewn.0kj1m.cn

Path(__file__).resolve().parent
来源：http://wqw.ctjpmb.com

[U39] Py：判断是否在交互环境
来源：http://ppl.xylfe.cn

sys.stdout.isatty()
来源：http://ocu.ivvv.top

[U40] Py：打印到标准错误
来源：http://aja.jlsjyb.cn

print("err", file=sys.stderr)
来源：http://clj.ctjpmb.com

[U41] PHP：初始化 Composer 项目
来源：http://zmj.aizwys.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://oni.fzhhl.top

[U42] PHP：PSR-4 自动加载
来源：http://ozw.zhijiandao.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vlw.xingfuxueyuan.xyz

[U43] PHP：声明命名空间
来源：http://neu.yangfankeji.com

namespace App\Http;
来源：http://ymq.yuanzhike.top

[U44] PHP：开启严格类型
来源：http://cua.bbcook.cn

declare(strict_types=1);
来源：http://xth.ctjpmb.com

[U45] PHP：类型声明与返回类型
来源：http://oln.jyoumei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vvy.havefunace.top

[U46] PHP：可空类型
来源：http://xxm.svipenyu.cn

?string $name = null
来源：http://jlc.guowangkeji.top

[U47] PHP：联合类型
来源：http://owx.hcnkem.com

int|string $id
来源：http://gir.meibo888.top

[U48] PHP：纯枚举
来源：http://sip.wangdashe.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nqs.ctjpmb.com

[U49] PHP：只读属性
来源：http://vcr.havefunace.top

public readonly string $name
来源：http://hxr.hammf.cn

[U50] PHP：构造器属性提升
来源：http://sia.zhengqikj.top

public function __construct(private int $id) {}
来源：http://hqu.chenlongwang.top

[U51] PHP：数组解构
来源：http://ssm.hywenlv.cn

[$a, $b] = $arr;
来源：http://mil.xziqi.cn

[U52] PHP：箭头函数
来源：http://agi.xylfe.cn

$double = fn($x) => $x * 2;
来源：http://gcz.cheryme.top

[U53] PHP：空合并运算符
来源：http://bdq.yvedp.cn

$v = $a ?? $b ?? "default";
来源：http://ule.zhaomingkeji.xyz

[U54] PHP：空安全调用
来源：http://ugx.bjfxy.top

$obj?->method()
来源：http://ilk.daxiang520.top

[U55] PHP：match 表达式
来源：http://yyv.yvedp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rtc.epnwcf.com

[U56] PHP：命名参数
来源：http://wcb.zhengqikj.top

f(a: 1, b: 2)
来源：http://knt.yfazqb.com

[U57] PHP：字符串插值
来源：http://whw.vqdsnc.cn

"值: {$a}"
来源：http://oee.hysaishi.cn

[U58] PHP：数组三件套
来源：http://gxi.xziqi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ltz.jinqigfzy.top

[U59] PHP：自定义排序
来源：http://hwz.xinyue.icu

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uhh.kuanghao11.cn

[U60] PHP：JSON 编解码
来源：http://aic.9152youxi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mdl.shanyushiyangkeji.top

[U61] PHP：正则
来源：http://zsf.tarul.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cyp.hcnkem.com

[U62] PHP：日期对象
来源：http://fdh.gogol.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rad.redwolf501.top

[U63] PHP：文件读写
来源：http://ypc.epnwcf.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dfe.cdnleiting.top

[U64] PHP：目录遍历
来源：http://cxg.shanyushiyangtech.top

glob("dir/*.php");  scandir("dir");
来源：http://brq.jianghu66.top

[U65] PHP：会话
来源：http://hca.sufxvd.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://atf.zhengqikj.top

[U66] PHP：设置 Cookie
来源：http://rac.pycfn.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jvd.wangshuangyany.cn

[U67] PHP：处理文件上传
来源：http://gcz.shangyingyoupin.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://win.wangdashe.top

[U68] PHP：PDO 连接
来源：http://cvb.jianghu66.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://quu.yanxiufei.cn

[U69] PHP：PDO 预处理
来源：http://shn.yj20258888.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baf.chenlongwang.top

[U70] PHP：PDO 事务
来源：http://bup.ehwqpu.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xpr.hesvh.cn

[U71] PHP：抛出异常
来源：http://efr.svipenyu.cn

throw new RuntimeException("失败", 500);
来源：http://qyc.zhijiandao.cn

[U72] PHP：写错误日志
来源：http://ecn.zycfv.cn

error_log("失败: " . $e->getMessage());
来源：http://gsc.vehdjk.com

[U73] PHP：读取 ini 配置
来源：http://guv.fanxiaobao.xyz

parse_ini_file("config.ini", true)
来源：http://qjy.ppjwa.cn

[U74] PHP：读取环境变量
来源：http://dnr.havefunace.top

getenv("APP_ENV") ?: "production"
来源：http://hid.hywenlv.cn

[U75] PHP：依赖注入
来源：http://rzw.mhx1999.top

composer require psr/container
来源：http://sas.jianghu66.top

[U76] PHP：简单路由
来源：http://xrj.jinqigufen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cgi.gaohongyu789.top

[U77] PHP：模板渲染
来源：http://eum.zhaomingkeji.xyz

composer require twig/twig
来源：http://alj.snrcjt.cn

[U78] PHP：单元测试
来源：http://ikq.yvedp.cn

composer require --dev phpunit/phpunit
来源：http://yvg.dianchejie.cn

[U79] PHP：静态分析
来源：http://vpq.nwbrower.top

composer require --dev phpstan/phpstan
来源：http://agu.jinghuilouyu.cn

[U80] PHP：代码规范修复
来源：http://ikq.bbcook.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://geq.pengpengdd.cyou

[U81] JS：初始化项目
来源：http://mre.shanyushiyangkeji.top

npm init -y;  npm i express
来源：http://jgo.shzxlz.cn

[U82] JS：package.json 脚本
来源：http://qow.0kj1m.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://djz.hcnkem.com

[U83] JS：ES Module 导入导出
来源：http://efz.vqdsnc.cn

export const a = 1;  import { a } from "./m.js";
来源：http://eag.jyoumei.cn

[U84] JS：CommonJS 写法
来源：http://unt.pycfn.com

module.exports = { a };  const { a } = require("./m");
来源：http://nnj.yongpay.top

[U85] JS：可选链
来源：http://apj.birdmap.top

a?.b?.c
来源：http://uii.hfpthk.cn

[U86] JS：空值合并
来源：http://ovp.xinyue.icu

a ?? b
来源：http://lob.mhx1999.top

[U87] JS：解构默认值
来源：http://rvj.haohaochexian.top

const { a = 1, b = 2 } = obj;
来源：http://lyn.yanxiufei.cn

[U88] JS：对象展开合并
来源：http://ruh.snrcjt.cn

{ ...a, ...b }
来源：http://kqd.sysykeji.top

[U89] JS：数组去重
来源：http://hxb.epnwcf.com

[...new Set(arr)]
来源：http://crn.jinghuilouyu.cn

[U90] JS：数字数组排序
来源：http://bjm.ydzc1.top

[...arr].sort((a, b) => a - b)
来源：http://tfk.zdqjudy.top

[U91] JS：对象键值遍历
来源：http://dpd.jlsjyb.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xmf.iojbl.cn

[U92] JS：深拷贝
来源：http://qzf.jqgfzy.top

structuredClone(obj)
来源：http://mht.xylfe.cn

[U93] JS：模板字符串
来源：http://bjg.zhiwuduotai.top

`共 ${n} 条`
来源：http://yrk.tianlin.xyz

[U94] JS：箭头函数
来源：http://rrs.cucudq.cn

const double = x => x * 2;
来源：http://zve.birdmap.top

[U95] JS：Promise 包装
来源：http://ewz.xylfe.cn

new Promise((resolve, reject) => {})
来源：http://rfp.jinqigfzy.top

[U96] JS：async/await 与异常
来源：http://kmq.jqgfzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tcq.cucudq.cn

[U97] JS：并发请求
来源：http://lda.hongshengwenyu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qmw.wangdashe.top

[U98] JS：fetch 带 JSON
来源：http://bqg.gzhubu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://utu.pycfn.com

[U99] JS：事件监听
来源：http://cnm.zhijiandao.cn

el.addEventListener("click", e => {})
来源：http://kmr.dianchejie.cn

[U100] JS：DOM 查询
来源：http://pxh.cashguo.top

document.querySelector(".item")
来源：http://jvj.ybcxt.top

[U101] JS：classList 操作
来源：http://bjr.hcnkem.com

el.classList.toggle("active")
来源：http://vkk.jqgufenzy.top

[U102] JS：本地存储
来源：http://dag.snrcjt.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tsb.shanyushiyangkeji.top

[U103] JS：定时器
来源：http://ebq.yuanzhike.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vpm.epnwcf.com

[U104] JS：防抖
来源：http://prd.chenlongwang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ije.mhx1999.top

[U105] JS：节流
来源：http://bay.zhijiandao.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mnf.pycfn.com

[U106] JS：日期格式化
来源：http://gtc.vehdjk.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rpw.guowangkeji.top

[U107] JS：数字千分位
来源：http://igd.daxiang520.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pwp.wangshuangyany.cn

[U108] JS：随机整数
来源：http://brk.uphjek.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kbs.yonumen.top

[U109] JS：数组分组
来源：http://vsz.sweek.top

Object.groupBy(arr, x => x.type)
来源：http://ilo.xylfe.cn

[U110] JS：数组分块
来源：http://jho.jyoumei.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bpq.hammf.cn

[U111] JS：对象转 Map
来源：http://lpx.uphjek.com

new Map(Object.entries(obj))
来源：http://nnm.9152youxi.cn

[U112] JS：字符串补位
来源：http://qsg.gzhubu.top

"7".padStart(3, "0")
来源：http://trw.chenzaomai.com

[U113] JS：正则替换全部
来源：http://lsr.chenzaomai.com

s.replaceAll("a", "b")
来源：http://zmy.andypj.xyz

[U114] JS：JSON 深比较
来源：http://neb.aizwys.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uss.mhx1999.top

[U115] JS：生成 UUID
来源：http://zxh.xuanzx.com

crypto.randomUUID()
来源：http://awu.smart0.xyz

[U116] JS：类型检查（JSDoc）
来源：http://hgm.fehbvm.com

/** @param {string} name */ function f(name) {}
来源：http://aqk.fktsv.cn

[U117] JS：单元测试
来源：http://iod.tianlin.xyz

npm i -D vitest;  npx vitest
来源：http://jkv.jinghuilouyu.cn

[U118] JS：开发服务器
来源：http://isa.meibo888.top

npm i -D vite;  npx vite
来源：http://xfr.cucudq.cn

[U119] JS：生产构建
来源：http://knl.0kj1m.cn

npx vite build
来源：http://kuj.jianghu66.top

[U120] JS：读取环境变量（Vite）
来源：http://zdd.zhiwuduotai.top

import.meta.env.VITE_API_URL
来源：http://ogj.jinghuilouyu.cn

================================================================================
来源：http://gwo.zhixingplan.top

统计汇总
来源：http://qhc.hongshengwenyu.top

================================================================================
来源：http://dsl.vehdjk.com

按语言统计（条）：
来源：http://byc.aizwys.cn

Python ......... 252
来源：http://kgq.nanxuanxn.top

PHP ............ 252
来源：http://dal.yangfankeji.com

JavaScript ..... 252
来源：http://zaa.cdnleiting.top

TypeScript ..... 212
来源：http://jtx.hcnkem.com

Java ........... 212
来源：http://qmo.gaohongyu789.top

Go ............. 212
来源：http://utg.ydjk.org.cn

Ruby ........... 212
来源：http://yny.316326.xyz

C# ............. 212
来源：http://mxz.shanyushiyangtech.top

C .............. 30
来源：http://olx.tarul.cn

C++ ............ 30
来源：http://evb.hammf.cn

SQL ............ 90
来源：http://vfv.kuanghao11.cn

Bash ........... 80
来源：http://bww.feifeiyinyue.top

Kotlin ......... 15
来源：http://kcq.cheryme.top

Swift .......... 15
来源：http://doz.chenjidiqi.icu

Lua ............ 10
来源：http://heg.gzhubu.top

Perl ........... 10
来源：http://air.kuanghao11.cn

Scala .......... 10
来源：http://xeh.sxryk.cn

------------------------------------
来源：http://pau.birdmap.top

合计 ........... 2106 条
来源：http://ima.xylfe.cn

按章节统计：
来源：http://ksf.52xcode.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ici.nwbrower.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rya.yongpay.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://joq.xuetiantiany.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xyp.ehwqpu.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xea.yfazqb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dyr.chenlongwang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pnl.jinyuanbaomall.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zmv.haohaochexian.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bin.quarkkingdee.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uau.zhengqikj.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uvb.vqdsnc.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ubf.c1oappe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xiz.zhaomingkeji.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fzg.fktsv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gza.xziqi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ill.0kj1m.cn

Q SQL 专题                              90
来源：http://bsn.cdnleiting.top

R Bash 专题                             80
来源：http://xzh.hongshengwenyu.top

S C / C++ 专题                          60
来源：http://oip.snrcjt.cn

T 其他语言补充                          60
来源：http://oit.chenzaomai.com

U 高频实用片段                         120
来源：http://tsf.jianghu66.top

------------------------------------
来源：http://bxi.hnxiangtu.top

合计                                  2106 条
来源：http://uhw.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://auy.gaohongyu789.top

使用提醒
来源：http://quw.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://xxh.guowangkeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zrn.ybcxt.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://eom.yfazqb.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ngn.jianghu66.top

在旧版本上使用前请先确认语法支持情况。
来源：http://rit.sufxvd.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vmh.tanke756.top

—— 文件结束 ——
来源：http://une.yuxming.cn

================================================================================
来源：http://odh.epnwcf.com

程序语言常见例子速查手册（2024 版）
来源：http://ndr.hnxiangtu.top

Common Programming Examples Cheat Book
来源：http://mwd.tianlin.xyz

================================================================================
来源：http://kvn.xuanzx.com

【收录内容】
来源：http://iuo.meibo888.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ehh.aibaodan.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://akk.ybcxt.top

SQL · Bash · C · C++
来源：http://aqr.nanxinkj.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qoi.zhixingplan.top

【使用说明】
来源：http://fyk.ctjpmb.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dii.hywenlv.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yov.pycfn.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jen.jlsjyb.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vvy.xylfe.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lhp.hesvh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nsa.yueranfly.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://imo.hcnkem.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sni.fengsongda.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hym.chenlongwang.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vko.pycfn.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cne.jqgufenzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uhx.tianlin.xyz

【文件统计】
来源：http://rme.daxiang520.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cnb.jianghu66.top

--------------------------------------------------------------------------------
来源：http://nbo.zhoulong.xyz

目  录
来源：http://krz.ctjpmb.com

--------------------------------------------------------------------------------
来源：http://ana.feifeiyinyue.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bxn.xingfuxueyuan.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gxo.hnxiangtu.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hta.gotoacloud.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bos.yonumen.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ctv.zycfv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bmb.zhiwuduotai.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fgz.dianchejie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hyc.zhoulong.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pnw.quarkkingdee.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xsq.snrcjt.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qsx.redwolf501.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vtu.xinyue.icu

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.ywan-chungtsiang.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://osg.cdnleiting.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://apt.pycfn.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jpc.fzhhl.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hol.yvedp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nbb.aibaodan.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cyq.sweek.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xnz.shuidangran.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://siu.fktsv.cn

================================================================================
来源：http://ktd.pengpengdd.cyou

A. 基础语法与类型
来源：http://wpb.tian-w.cn

================================================================================
来源：http://swe.shuidangran.top

[A01] Hello World
来源：http://chd.birdmap.top

Py:   print("Hello, World!")
来源：http://ldb.zdbjq.cn

PHP:  echo "Hello, World!";
来源：http://hnk.yangfankeji.com

JS:   console.log("Hello, World!");
来源：http://whn.yanxiufei.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://smd.bjfxy.top

Java: System.out.println("Hello, World!");
来源：http://gvl.hfpthk.cn

Go:   fmt.Println("Hello, World!")
来源：http://dyd.zhaomingkeji.xyz

Ruby: puts "Hello, World!"
来源：http://shb.yonumen.top

C#:   Console.WriteLine("Hello, World!");
来源：http://lqp.ydjk.org.cn

[A02] 变量声明与赋值
来源：http://tpe.bbcook.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://osh.pengpengdd.cyou

PHP:  $name = "Alex"; $age = 20;
来源：http://hnl.hongshengwenyu.top

JS:   let name = "Alex"; const age = 20;
来源：http://xkc.316326.xyz


<!-- 参考信息 -->