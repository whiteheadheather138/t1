代发 wailian999

[U47] PHP：联合类型
来源：http://rup.tanke756.top

int|string $id
来源：http://wvd.ppjwa.cn

[U48] PHP：纯枚举
来源：http://ngh.zhengqikj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://elm.andypj.xyz

[U49] PHP：只读属性
来源：http://nmc.xziqi.cn

public readonly string $name
来源：http://lsw.guannengcc.top

[U50] PHP：构造器属性提升
来源：http://ops.chenjidiqi.icu

public function __construct(private int $id) {}
来源：http://cea.gaohongyu789.top

[U51] PHP：数组解构
来源：http://fph.jianghu66.top

[$a, $b] = $arr;
来源：http://swg.redwolf501.top

[U52] PHP：箭头函数
来源：http://lgi.tanke756.top

$double = fn($x) => $x * 2;
来源：http://eps.ywan-chungtsiang.top

[U53] PHP：空合并运算符
来源：http://tbk.iojbl.cn

$v = $a ?? $b ?? "default";
来源：http://qau.jinqigufen.top

[U54] PHP：空安全调用
来源：http://lky.hongshengwenyu.top

$obj?->method()
来源：http://hhp.c1oappe.top

[U55] PHP：match 表达式
来源：http://lsv.redwolf501.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zeu.hywenlv.cn

[U56] PHP：命名参数
来源：http://gse.jiagoushi.top

f(a: 1, b: 2)
来源：http://opu.yueranfly.top

[U57] PHP：字符串插值
来源：http://olc.fehbvm.com

"值: {$a}"
来源：http://jcg.hongshengwenyu.top

[U58] PHP：数组三件套
来源：http://doj.fktsv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ytm.zycfv.cn

[U59] PHP：自定义排序
来源：http://auh.shanyushiyangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dmu.chenjidiqi.icu

[U60] PHP：JSON 编解码
来源：http://pmy.wangdashe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eyd.xinyue.icu

[U61] PHP：正则
来源：http://yah.c1oappe.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://efh.ctjpmb.com

[U62] PHP：日期对象
来源：http://yab.jinghuilouyu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tct.cucudq.cn

[U63] PHP：文件读写
来源：http://sdz.kuanghao11.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ymd.jinqigufen.top

[U64] PHP：目录遍历
来源：http://yjh.zhoulong.xyz

glob("dir/*.php");  scandir("dir");
来源：http://bdu.xylfe.cn

[U65] PHP：会话
来源：http://tiu.shzxlz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rlw.tian-w.cn

[U66] PHP：设置 Cookie
来源：http://tmu.xylfe.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yqu.feifeiyinyue.top

[U67] PHP：处理文件上传
来源：http://qjb.epnwcf.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zvm.aibaodan.cn

[U68] PHP：PDO 连接
来源：http://tgo.nanxuanxn.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gdr.jiagoushi.top

[U69] PHP：PDO 预处理
来源：http://rbb.havefunace.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ugr.hnxiangtu.top

[U70] PHP：PDO 事务
来源：http://pkx.sjlbkw.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pqx.hysaishi.cn

[U71] PHP：抛出异常
来源：http://jgq.ywan-chungtsiang.top

throw new RuntimeException("失败", 500);
来源：http://yjw.xziqi.cn

[U72] PHP：写错误日志
来源：http://elc.zhongyouzk.top

error_log("失败: " . $e->getMessage());
来源：http://hhj.jinghuilouyu.cn

[U73] PHP：读取 ini 配置
来源：http://nfe.yfazqb.com

parse_ini_file("config.ini", true)
来源：http://qch.vehdjk.com

[U74] PHP：读取环境变量
来源：http://zok.havefunace.top

getenv("APP_ENV") ?: "production"
来源：http://sfc.sysykeji.top

[U75] PHP：依赖注入
来源：http://fup.gaohongyu789.top

composer require psr/container
来源：http://ckr.52xcode.cn

[U76] PHP：简单路由
来源：http://jjw.fehbvm.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dbh.quarkkingdee.top

[U77] PHP：模板渲染
来源：http://wme.dianchejie.cn

composer require twig/twig
来源：http://evh.yj20258888.top

[U78] PHP：单元测试
来源：http://vay.aizwys.cn

composer require --dev phpunit/phpunit
来源：http://sfz.daxiang520.top

[U79] PHP：静态分析
来源：http://pkr.0kj1m.cn

composer require --dev phpstan/phpstan
来源：http://bgc.vqdsnc.cn

[U80] PHP：代码规范修复
来源：http://gbg.bbcook.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pex.xziqi.cn

[U81] JS：初始化项目
来源：http://uei.yongpay.top

npm init -y;  npm i express
来源：http://pab.tianlin.xyz

[U82] JS：package.json 脚本
来源：http://bra.hysaishi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kqu.chenlongwang.top

[U83] JS：ES Module 导入导出
来源：http://bsl.jqgfzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://bya.ivvv.top

[U84] JS：CommonJS 写法
来源：http://rcd.shangyingyoupin.top

module.exports = { a };  const { a } = require("./m");
来源：http://art.c1oappe.top

[U85] JS：可选链
来源：http://xqo.iojbl.cn

a?.b?.c
来源：http://cgh.yangfankeji.com

[U86] JS：空值合并
来源：http://zjj.jqgfzy.top

a ?? b
来源：http://amo.yj202588.top

[U87] JS：解构默认值
来源：http://phq.yuanzhike.top

const { a = 1, b = 2 } = obj;
来源：http://fqh.fzhhl.top

[U88] JS：对象展开合并
来源：http://ght.jlsjyb.cn

{ ...a, ...b }
来源：http://wjr.hnqzz.top

[U89] JS：数组去重
来源：http://eaj.52xcode.cn

[...new Set(arr)]
来源：http://beu.guannengcc.top

[U90] JS：数字数组排序
来源：http://vun.ydzc1.top

[...arr].sort((a, b) => a - b)
来源：http://pyd.gogol.net.cn

[U91] JS：对象键值遍历
来源：http://qbi.xinyue.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kgm.bjfxy.top

[U92] JS：深拷贝
来源：http://btf.xylfe.cn

structuredClone(obj)
来源：http://pxp.jqgfzy.top

[U93] JS：模板字符串
来源：http://yve.tian-w.cn

`共 ${n} 条`
来源：http://tdd.yangfankeji.com

[U94] JS：箭头函数
来源：http://rhe.fehbvm.com

const double = x => x * 2;
来源：http://xlq.gotoacloud.top

[U95] JS：Promise 包装
来源：http://ndf.hammf.cn

new Promise((resolve, reject) => {})
来源：http://pii.dashuyun.cn

[U96] JS：async/await 与异常
来源：http://bvh.ivvv.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ahc.tian-w.cn

[U97] JS：并发请求
来源：http://uky.yuxming.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zaf.hnqzz.top

[U98] JS：fetch 带 JSON
来源：http://bjp.jiagoushi.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tzt.9152youxi.cn

[U99] JS：事件监听
来源：http://zgv.pengpengdd.cyou

el.addEventListener("click", e => {})
来源：http://zkm.hammf.cn

[U100] JS：DOM 查询
来源：http://cch.shuidangran.top

document.querySelector(".item")
来源：http://vvl.feifeiyinyue.top

[U101] JS：classList 操作
来源：http://qaf.xziqi.cn

el.classList.toggle("active")
来源：http://gjh.ydjk.org.cn

[U102] JS：本地存储
来源：http://etr.fktsv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://coj.daxiang520.top

[U103] JS：定时器
来源：http://gnn.nwbrower.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fko.zycfv.cn

[U104] JS：防抖
来源：http://zvy.guowangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ama.jinghuilouyu.cn

[U105] JS：节流
来源：http://zji.jinqigufen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://siu.haohaochexian.top

[U106] JS：日期格式化
来源：http://zbi.jinyuanbaomall.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rja.cqqwz.cn

[U107] JS：数字千分位
来源：http://yer.wangdashe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gjj.cashguo.top

[U108] JS：随机整数
来源：http://eox.smart0.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dbg.haohaochexian.top

[U109] JS：数组分组
来源：http://xhh.bbcook.cn

Object.groupBy(arr, x => x.type)
来源：http://hnt.ehwqpu.com

[U110] JS：数组分块
来源：http://rmj.jianghu66.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oqk.xziqi.cn

[U111] JS：对象转 Map
来源：http://lmv.nanxuanxn.top

new Map(Object.entries(obj))
来源：http://ffy.xuanzx.com

[U112] JS：字符串补位
来源：http://ehu.guowangkeji.top

"7".padStart(3, "0")
来源：http://yby.zhongyouzk.top

[U113] JS：正则替换全部
来源：http://fgl.yonumen.top

s.replaceAll("a", "b")
来源：http://ylk.gotoacloud.top

[U114] JS：JSON 深比较
来源：http://bnk.fktsv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cqp.sjlbkw.cn

[U115] JS：生成 UUID
来源：http://zfm.havefunace.top

crypto.randomUUID()
来源：http://meq.ywan-chungtsiang.top

[U116] JS：类型检查（JSDoc）
来源：http://urx.bjfxy.top

/** @param {string} name */ function f(name) {}
来源：http://ftl.guowangkeji.top

[U117] JS：单元测试
来源：http://fcm.hysaishi.cn

npm i -D vitest;  npx vitest
来源：http://zzk.yfazqb.com

[U118] JS：开发服务器
来源：http://pco.redwolf501.top

npm i -D vite;  npx vite
来源：http://wmx.yueranfly.top

[U119] JS：生产构建
来源：http://hby.redwolf501.top

npx vite build
来源：http://pqh.hywenlv.cn

[U120] JS：读取环境变量（Vite）
来源：http://wmg.haohaochexian.top

import.meta.env.VITE_API_URL
来源：http://llp.jianghu66.top

================================================================================
来源：http://yvf.nanxinkj.top

统计汇总
来源：http://dhv.hongshengwenyu.top

================================================================================
来源：http://ruu.cucudq.cn

按语言统计（条）：
来源：http://cdi.ehwqpu.com

Python ......... 252
来源：http://uds.jiagoushi.top

PHP ............ 252
来源：http://umk.ybcxt.top

JavaScript ..... 252
来源：http://lkb.guannengcc.top

TypeScript ..... 212
来源：http://fwn.ctjpmb.com

Java ........... 212
来源：http://yst.gzhubu.top

Go ............. 212
来源：http://nxc.yangfankeji.com

Ruby ........... 212
来源：http://yko.jqgufenzy.top

C# ............. 212
来源：http://vle.ppjwa.cn

C .............. 30
来源：http://bbc.gzhubu.top

C++ ............ 30
来源：http://cau.jianghu66.top

SQL ............ 90
来源：http://ici.aizwys.cn

Bash ........... 80
来源：http://cpi.xinyue.icu

Kotlin ......... 15
来源：http://bie.yueranfly.top

Swift .......... 15
来源：http://urf.fehbvm.com

Lua ............ 10
来源：http://vcf.hesvh.cn

Perl ........... 10
来源：http://ahp.shanyushiyangkeji.top

Scala .......... 10
来源：http://ufk.redwolf501.top

------------------------------------
来源：http://eoi.gzhubu.top

合计 ........... 2106 条
来源：http://wtz.nanxuanxn.top

按章节统计：
来源：http://wbo.jinqigfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uum.yvedp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wqx.fengsongda.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://iif.zdqjudy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hdd.ybcxt.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ext.wangdashe.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uho.feifeiyinyue.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uwn.nanxuanxn.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vri.chenzaomai.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zqd.zhiwuduotai.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wml.wangshuangyany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qpd.yonumen.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wle.quarkkingdee.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bag.epnwcf.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://naf.gaohongyu789.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rwm.yongpay.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://prm.feifeiyinyue.top

Q SQL 专题                              90
来源：http://xqv.jinghuilouyu.cn

R Bash 专题                             80
来源：http://gxy.ydjk.org.cn

S C / C++ 专题                          60
来源：http://eoo.fehbvm.com

T 其他语言补充                          60
来源：http://blb.shuidangran.top

U 高频实用片段                         120
来源：http://hli.tanke756.top

------------------------------------
来源：http://xxo.zhongyouzk.top

合计                                  2106 条
来源：http://wag.tian-w.cn

--------------------------------------------------------------------------------
来源：http://rww.cucudq.cn

使用提醒
来源：http://amv.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://snm.andypj.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://azf.andypj.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sfz.c1oappe.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ntq.jinyuanbaomall.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vev.smart0.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tdn.jinyuanbaomall.cn

—— 文件结束 ——
来源：http://tfx.birdmap.top

================================================================================
来源：http://ezz.xuanzx.com

程序语言常见例子速查手册（2024 版）
来源：http://vqs.yueranfly.top

Common Programming Examples Cheat Book
来源：http://opy.smart0.xyz

================================================================================
来源：http://bgv.jyoumei.cn

【收录内容】
来源：http://yuj.tanke756.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://afn.cashguo.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wgn.tian-w.cn

SQL · Bash · C · C++
来源：http://rsy.dashuyun.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qyp.guowangkeji.top

【使用说明】
来源：http://ipd.jinyuanbaomall.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pif.hfpthk.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zxt.uphjek.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ytx.cucudq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ovv.gaohongyu789.top

Bash:  Shell         C:     C             C++:   C++
来源：http://zqi.shangyingyoupin.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bmb.bjfxy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mhg.wangshuangyany.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wwa.meibo888.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ppg.ctjpmb.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nxh.feifeiyinyue.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xfi.fehbvm.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://eic.fktsv.cn

【文件统计】
来源：http://mct.bbcook.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hgy.tanke756.top

--------------------------------------------------------------------------------
来源：http://gea.ydjk.org.cn

目  录
来源：http://ets.ydzc1.top

--------------------------------------------------------------------------------
来源：http://qva.shanyushiyangkeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wny.cdnleiting.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dgt.shanyushiyangtech.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tjw.xuanzx.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mkb.chenzaomai.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://paz.jiagoushi.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qoj.zhixingplan.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bbn.chenlongwang.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://iil.9152youxi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eij.sysykeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fej.fehbvm.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wkf.ydzc1.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bki.chenzaomai.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ppg.dashuyun.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dhd.snrcjt.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ewu.ppjwa.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ojg.nanxinkj.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://czp.hongshengwenyu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://jzx.chenzaomai.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jwc.birdmap.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://voh.ydjk.org.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://why.hysaishi.cn

================================================================================
来源：http://rdc.jiagoushi.top

A. 基础语法与类型
来源：http://vje.dashuyun.cn

================================================================================
来源：http://kra.zycfv.cn

[A01] Hello World
来源：http://dfc.hnqzz.top

Py:   print("Hello, World!")
来源：http://joa.jiagoushi.top

PHP:  echo "Hello, World!";
来源：http://jsn.hfpthk.cn

JS:   console.log("Hello, World!");
来源：http://hap.bbcook.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hst.ywan-chungtsiang.top

Java: System.out.println("Hello, World!");
来源：http://xew.jianghu66.top

Go:   fmt.Println("Hello, World!")
来源：http://mnf.xylfe.cn

Ruby: puts "Hello, World!"
来源：http://ult.yuanzhike.top

C#:   Console.WriteLine("Hello, World!");
来源：http://nnq.xinyue.icu

[A02] 变量声明与赋值
来源：http://vnv.redwolf501.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ine.ydjk.org.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://olp.shzxlz.cn

JS:   let name = "Alex"; const age = 20;
来源：http://amv.ehwqpu.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fub.gzhubu.top

Java: String name = "Alex"; int age = 20;
来源：http://oav.yongpay.top

Go:   name := "Alex"; age := 20
来源：http://nmb.zhixingplan.top

Ruby: name = "Alex"; age = 20
来源：http://ipn.ivvv.top

C#:   string name = "Alex"; int age = 20;
来源：http://xas.yvedp.cn

[A03] 常量定义
来源：http://ffu.ctjpmb.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bmy.yfazqb.com

PHP:  const PI = 3.14159;
来源：http://uam.yangfankeji.com

JS:   const PI = 3.14159;
来源：http://aps.feifeiyinyue.top

TS:   const PI: number = 3.14159;
来源：http://dmk.yuxming.cn

Java: static final double PI = 3.14159;
来源：http://wmx.mhx1999.top

Go:   const PI = 3.14159
来源：http://rvc.guowangkeji.top

Ruby: PI = 3.14159
来源：http://zfp.0kj1m.cn

C#:   const double PI = 3.14159;
来源：http://mnd.nwbrower.top

[A04] 判断变量类型
来源：http://grq.cdnleiting.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://yfb.wangdashe.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ius.bbcook.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ywq.jqgufenzy.top

TS:   typeof x; x instanceof Date
来源：http://bvw.xinyue.icu

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vsm.yonumen.top

Go:   reflect.TypeOf(x).Name()
来源：http://ugp.dashuyun.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://obt.xinyue.icu

C#:   x.GetType().Name; x is int
来源：http://tkd.jinqigufen.top

[A05] 整数除法与取模
来源：http://wqm.vehdjk.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bdp.andypj.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://yum.snrcjt.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mer.dianchejie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xia.yj20258888.top

Java: 7 / 2; 7 % 2
来源：http://atj.hysaishi.cn

Go:   7 / 2; 7 % 2
来源：http://gjm.cqqwz.cn

Ruby: 7 / 2; 7 % 2
来源：http://iuy.shzxlz.cn

C#:   7 / 2; 7 % 2
来源：http://tmk.daria6918.cn


<!-- 参考信息 -->