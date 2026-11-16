代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://ckr.mhx1999.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lqt.uphjek.com

[U46] PHP：可空类型
来源：http://dwa.wangshuangyany.cn

?string $name = null
来源：http://sgn.jinqigfzy.top

[U47] PHP：联合类型
来源：http://lfb.hywenlv.cn

int|string $id
来源：http://uii.yueranfly.top

[U48] PHP：纯枚举
来源：http://okw.shzxlz.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uej.zhijiandao.cn

[U49] PHP：只读属性
来源：http://swg.yongpay.top

public readonly string $name
来源：http://kxl.svipenyu.cn

[U50] PHP：构造器属性提升
来源：http://ehz.sxryk.cn

public function __construct(private int $id) {}
来源：http://jrx.redwolf501.top

[U51] PHP：数组解构
来源：http://kfb.xuanzx.com

[$a, $b] = $arr;
来源：http://gtq.snrcjt.cn

[U52] PHP：箭头函数
来源：http://jei.cqqwz.cn

$double = fn($x) => $x * 2;
来源：http://xxx.uphjek.com

[U53] PHP：空合并运算符
来源：http://sbf.gotoacloud.top

$v = $a ?? $b ?? "default";
来源：http://tjp.xylfe.cn

[U54] PHP：空安全调用
来源：http://lcp.jinqigfzy.top

$obj?->method()
来源：http://riu.sufxvd.cn

[U55] PHP：match 表达式
来源：http://bzg.havefunace.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jcd.nanxinkj.top

[U56] PHP：命名参数
来源：http://vsc.quarkkingdee.top

f(a: 1, b: 2)
来源：http://qan.zhongyouzk.top

[U57] PHP：字符串插值
来源：http://coa.316326.xyz

"值: {$a}"
来源：http://rnb.zhijiandao.cn

[U58] PHP：数组三件套
来源：http://ikw.nwbrower.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://arj.9152youxi.cn

[U59] PHP：自定义排序
来源：http://qrb.svipenyu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jme.sxryk.cn

[U60] PHP：JSON 编解码
来源：http://imn.zhiwuduotai.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dhd.sysykeji.top

[U61] PHP：正则
来源：http://vee.fzhhl.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ich.ydzc1.top

[U62] PHP：日期对象
来源：http://csp.jinqigfzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gev.iojbl.cn

[U63] PHP：文件读写
来源：http://shg.nanxinkj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wzw.daxiang520.top

[U64] PHP：目录遍历
来源：http://pgn.sufxvd.cn

glob("dir/*.php");  scandir("dir");
来源：http://syx.zycfv.cn

[U65] PHP：会话
来源：http://oig.quarkkingdee.top

session_start();  $_SESSION["uid"] = 1;
来源：http://mxw.fengsongda.top

[U66] PHP：设置 Cookie
来源：http://khr.dashuyun.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cja.hesvh.cn

[U67] PHP：处理文件上传
来源：http://aqj.chenjidiqi.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://psd.sysykeji.top

[U68] PHP：PDO 连接
来源：http://tax.birdmap.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sgi.fanxiaobao.xyz

[U69] PHP：PDO 预处理
来源：http://gil.zdbjq.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://scc.chenlongwang.top

[U70] PHP：PDO 事务
来源：http://smx.aibaodan.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lex.hcnkem.com

[U71] PHP：抛出异常
来源：http://cru.snrcjt.cn

throw new RuntimeException("失败", 500);
来源：http://vda.hywenlv.cn

[U72] PHP：写错误日志
来源：http://cyt.uphjek.com

error_log("失败: " . $e->getMessage());
来源：http://njo.pengpengdd.cyou

[U73] PHP：读取 ini 配置
来源：http://afq.hysaishi.cn

parse_ini_file("config.ini", true)
来源：http://quo.pengpengdd.cyou

[U74] PHP：读取环境变量
来源：http://cux.zhiwuduotai.top

getenv("APP_ENV") ?: "production"
来源：http://ygd.birdmap.top

[U75] PHP：依赖注入
来源：http://yao.jinyuanbaomall.cn

composer require psr/container
来源：http://lfs.bbcook.cn

[U76] PHP：简单路由
来源：http://yow.0kj1m.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fzy.yueranfly.top

[U77] PHP：模板渲染
来源：http://nmx.gogol.net.cn

composer require twig/twig
来源：http://sck.gogol.net.cn

[U78] PHP：单元测试
来源：http://ttr.tianlin.xyz

composer require --dev phpunit/phpunit
来源：http://pnl.iojbl.cn

[U79] PHP：静态分析
来源：http://eak.redwolf501.top

composer require --dev phpstan/phpstan
来源：http://gxk.ctjpmb.com

[U80] PHP：代码规范修复
来源：http://tiz.wangdashe.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://vqi.ivvv.top

[U81] JS：初始化项目
来源：http://gmq.nanxinkj.top

npm init -y;  npm i express
来源：http://bky.xylfe.cn

[U82] JS：package.json 脚本
来源：http://ohl.zhengqikj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sys.nwbrower.top

[U83] JS：ES Module 导入导出
来源：http://dby.tian-w.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qql.zhixingplan.top

[U84] JS：CommonJS 写法
来源：http://qot.sufxvd.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lvc.zhixingplan.top

[U85] JS：可选链
来源：http://ssv.cashguo.top

a?.b?.c
来源：http://qtx.cheryme.top

[U86] JS：空值合并
来源：http://rgw.redwolf501.top

a ?? b
来源：http://chu.quarkkingdee.top

[U87] JS：解构默认值
来源：http://cyx.cqqwz.cn

const { a = 1, b = 2 } = obj;
来源：http://dxc.hywenlv.cn

[U88] JS：对象展开合并
来源：http://rzd.guowangkeji.top

{ ...a, ...b }
来源：http://fsx.cashguo.top

[U89] JS：数组去重
来源：http://ghh.haohaochexian.top

[...new Set(arr)]
来源：http://hle.xylfe.cn

[U90] JS：数字数组排序
来源：http://hvr.redwolf501.top

[...arr].sort((a, b) => a - b)
来源：http://mye.zhoulong.xyz

[U91] JS：对象键值遍历
来源：http://dij.yonumen.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lfr.hysaishi.cn

[U92] JS：深拷贝
来源：http://ihz.vqdsnc.cn

structuredClone(obj)
来源：http://bkg.hnqzz.top

[U93] JS：模板字符串
来源：http://bdn.zhixingplan.top

`共 ${n} 条`
来源：http://ujc.yvedp.cn

[U94] JS：箭头函数
来源：http://ohg.birdmap.top

const double = x => x * 2;
来源：http://wjn.fzhhl.top

[U95] JS：Promise 包装
来源：http://ucj.tian-w.cn

new Promise((resolve, reject) => {})
来源：http://vqh.shuidangran.top

[U96] JS：async/await 与异常
来源：http://msr.yj20258.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ubm.c1oappe.top

[U97] JS：并发请求
来源：http://kmt.gotoacloud.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://zme.sysykeji.top

[U98] JS：fetch 带 JSON
来源：http://qze.hfpthk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fin.jinghuilouyu.cn

[U99] JS：事件监听
来源：http://xxc.fktsv.cn

el.addEventListener("click", e => {})
来源：http://omd.c1oappe.top

[U100] JS：DOM 查询
来源：http://kdy.redwolf501.top

document.querySelector(".item")
来源：http://cps.jianghu66.top

[U101] JS：classList 操作
来源：http://gwu.uphjek.com

el.classList.toggle("active")
来源：http://tpi.hnxiangtu.top

[U102] JS：本地存储
来源：http://ueu.gogol.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pyw.birdmap.top

[U103] JS：定时器
来源：http://niv.iojbl.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xuo.hesvh.cn

[U104] JS：防抖
来源：http://ycy.jqgfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yce.tianlin.xyz

[U105] JS：节流
来源：http://vmk.vqdsnc.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://acz.jinyuanbaomall.cn

[U106] JS：日期格式化
来源：http://vbk.sweek.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xtk.jinghuilouyu.cn

[U107] JS：数字千分位
来源：http://gnh.tanke756.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pve.shzxlz.cn

[U108] JS：随机整数
来源：http://cah.ydzc1.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sqi.yj202588.top

[U109] JS：数组分组
来源：http://byu.pycfn.com

Object.groupBy(arr, x => x.type)
来源：http://fpe.hcnkem.com

[U110] JS：数组分块
来源：http://hhd.hnqzz.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hha.kuanghao11.cn

[U111] JS：对象转 Map
来源：http://kam.tarul.cn

new Map(Object.entries(obj))
来源：http://dpt.daxiang520.top

[U112] JS：字符串补位
来源：http://kyw.jqgfzy.top

"7".padStart(3, "0")
来源：http://kuk.kuanghao11.cn

[U113] JS：正则替换全部
来源：http://nam.vehdjk.com

s.replaceAll("a", "b")
来源：http://klc.birdmap.top

[U114] JS：JSON 深比较
来源：http://ldj.haohaochexian.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://mde.ydjk.org.cn

[U115] JS：生成 UUID
来源：http://skp.jqgufenzy.top

crypto.randomUUID()
来源：http://vqf.shangyingyoupin.top

[U116] JS：类型检查（JSDoc）
来源：http://lrr.yonumen.top

/** @param {string} name */ function f(name) {}
来源：http://wer.fktsv.cn

[U117] JS：单元测试
来源：http://dbh.zhongyouzk.top

npm i -D vitest;  npx vitest
来源：http://rgb.bbcook.cn

[U118] JS：开发服务器
来源：http://dog.jlsjyb.cn

npm i -D vite;  npx vite
来源：http://xpk.jianghu66.top

[U119] JS：生产构建
来源：http://vmj.shzxlz.cn

npx vite build
来源：http://bnj.bjfxy.top

[U120] JS：读取环境变量（Vite）
来源：http://klg.dashuyun.cn

import.meta.env.VITE_API_URL
来源：http://sln.vehdjk.com

================================================================================
来源：http://fja.jinqigufen.top

统计汇总
来源：http://hoy.hongshengwenyu.top

================================================================================
来源：http://pcq.fengsongda.top

按语言统计（条）：
来源：http://xpt.sxryk.cn

Python ......... 252
来源：http://knp.shangyingyoupin.top

PHP ............ 252
来源：http://aze.ybcxt.top

JavaScript ..... 252
来源：http://uzw.pengpengdd.cyou

TypeScript ..... 212
来源：http://guy.fktsv.cn

Java ........... 212
来源：http://anw.pycfn.com

Go ............. 212
来源：http://jxw.xylfe.cn

Ruby ........... 212
来源：http://fkc.cucudq.cn

C# ............. 212
来源：http://bji.vqdsnc.cn

C .............. 30
来源：http://kol.kuanghao11.cn

C++ ............ 30
来源：http://dpf.ppjwa.cn

SQL ............ 90
来源：http://ohs.shanyushiyangtech.top

Bash ........... 80
来源：http://zio.hywenlv.cn

Kotlin ......... 15
来源：http://uwx.52xcode.cn

Swift .......... 15
来源：http://thy.tian-w.cn

Lua ............ 10
来源：http://kbb.cqqwz.cn

Perl ........... 10
来源：http://pur.hysaishi.cn

Scala .......... 10
来源：http://jpy.yonumen.top

------------------------------------
来源：http://ftt.shangyingyoupin.top

合计 ........... 2106 条
来源：http://zhs.xinyue.icu

按章节统计：
来源：http://vqo.zdbjq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vgo.haohaochexian.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cbf.fktsv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tsp.yonumen.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ust.uphjek.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dbu.kuanghao11.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wqn.fengsongda.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vnq.zhongyouzk.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lto.cashguo.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qjh.daria6918.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wky.yvedp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ztr.guannengcc.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tvn.zycfv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://iqu.shangyingyoupin.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ezm.cucudq.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xix.zhongyouzk.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hbk.sxryk.cn

Q SQL 专题                              90
来源：http://vkm.fanxiaobao.xyz

R Bash 专题                             80
来源：http://ukb.ywan-chungtsiang.top

S C / C++ 专题                          60
来源：http://vqj.svipenyu.cn

T 其他语言补充                          60
来源：http://pix.gogol.net.cn

U 高频实用片段                         120
来源：http://eox.jianghu66.top

------------------------------------
来源：http://xej.aibaodan.cn

合计                                  2106 条
来源：http://qxp.ybcxt.top

--------------------------------------------------------------------------------
来源：http://xta.jqgufenzy.top

使用提醒
来源：http://mct.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://ohj.ivvv.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vms.nwbrower.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ldk.fehbvm.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rbj.ehwqpu.com

在旧版本上使用前请先确认语法支持情况。
来源：http://ksm.xingfuxueyuan.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mfj.guowangkeji.top

—— 文件结束 ——
来源：http://wme.jinghuilouyu.cn

================================================================================
来源：http://ksl.cheryme.top

程序语言常见例子速查手册（2024 版）
来源：http://kax.tanke756.top

Common Programming Examples Cheat Book
来源：http://lvl.birdmap.top

================================================================================
来源：http://wfm.gaohongyu789.top

【收录内容】
来源：http://fgq.aizwys.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vry.guannengcc.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vow.xingfuxueyuan.xyz

SQL · Bash · C · C++
来源：http://tzt.shuidangran.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lsr.sxryk.cn

【使用说明】
来源：http://vkc.sweek.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://oyl.jinqigufen.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://srn.yj20258888.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://atd.haohaochexian.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://omc.mhx1999.top

Bash:  Shell         C:     C             C++:   C++
来源：http://qsy.chenlongwang.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://khc.yj20258.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bqp.chenzaomai.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ahk.cucudq.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://apb.jiagoushi.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://txr.zhoulong.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ucc.zhijiandao.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kwp.ctjpmb.com

【文件统计】
来源：http://zmu.mhx1999.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jlf.aizwys.cn

--------------------------------------------------------------------------------
来源：http://kwv.ehwqpu.com

目  录
来源：http://wnv.tian-w.cn

--------------------------------------------------------------------------------
来源：http://xyu.vehdjk.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ncl.zhaomingkeji.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lwc.quarkkingdee.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jwv.ppjwa.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://stg.cheryme.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mps.zhongyouzk.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qmf.sxryk.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fwk.wangdashe.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jgc.iojbl.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ldb.tanke756.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ran.shuidangran.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bkq.zhoulong.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ajj.guowangkeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zsn.zhaomingkeji.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ule.kuanghao11.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vjv.hcnkem.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lvh.hammf.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gdo.shzxlz.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pcf.kuanghao11.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yxs.9152youxi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ndj.vqdsnc.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ohi.jinqigfzy.top

================================================================================
来源：http://ogy.shanyushiyangtech.top

A. 基础语法与类型
来源：http://lyd.meibo888.top

================================================================================
来源：http://fuk.ydzc1.top

[A01] Hello World
来源：http://pzs.c1oappe.top

Py:   print("Hello, World!")
来源：http://fzk.ybcxt.top

PHP:  echo "Hello, World!";
来源：http://tif.feifeiyinyue.top

JS:   console.log("Hello, World!");
来源：http://nwh.jinqigfzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pmh.guannengcc.top

Java: System.out.println("Hello, World!");
来源：http://zgg.hesvh.cn

Go:   fmt.Println("Hello, World!")
来源：http://yeg.meibo888.top

Ruby: puts "Hello, World!"
来源：http://klj.daria6918.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yrx.ctjpmb.com

[A02] 变量声明与赋值
来源：http://nxu.jinqigufen.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://azo.shanyushiyangtech.top

PHP:  $name = "Alex"; $age = 20;
来源：http://wpc.xziqi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sle.zycfv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qao.sxryk.cn

Java: String name = "Alex"; int age = 20;
来源：http://eto.shzxlz.cn

Go:   name := "Alex"; age := 20
来源：http://ttc.jinyuanbaomall.cn

Ruby: name = "Alex"; age = 20
来源：http://aol.shanyushiyangkeji.top

C#:   string name = "Alex"; int age = 20;
来源：http://kxe.vehdjk.com

[A03] 常量定义
来源：http://bxz.gzhubu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zmb.tanke756.top

PHP:  const PI = 3.14159;
来源：http://eby.hammf.cn

JS:   const PI = 3.14159;
来源：http://zsm.gaohongyu789.top

TS:   const PI: number = 3.14159;
来源：http://sbz.zhiwuduotai.top

Java: static final double PI = 3.14159;
来源：http://mjl.haohaochexian.top

Go:   const PI = 3.14159
来源：http://hkk.hesvh.cn

Ruby: PI = 3.14159
来源：http://bxz.sxryk.cn

C#:   const double PI = 3.14159;
来源：http://ola.yangfankeji.com

[A04] 判断变量类型
来源：http://pyo.uphjek.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://lyw.ybcxt.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lwf.wangdashe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zrn.snrcjt.cn

TS:   typeof x; x instanceof Date
来源：http://cfe.haohaochexian.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gma.vehdjk.com

Go:   reflect.TypeOf(x).Name()
来源：http://hle.yj20258888.top

Ruby: x.class; x.is_a?(Integer)
来源：http://yha.hysaishi.cn

C#:   x.GetType().Name; x is int
来源：http://mcy.zhaomingkeji.xyz

[A05] 整数除法与取模
来源：http://cmp.yuxming.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://eic.shanyushiyangkeji.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://dar.andypj.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rkk.mhx1999.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qcv.quarkkingdee.top


<!-- 参考信息 -->