代发 wailian999

[U49] PHP：只读属性
来源：http://vep.ppjwa.cn

public readonly string $name
来源：http://djy.haohaochexian.top

[U50] PHP：构造器属性提升
来源：http://tjb.pycfn.com

public function __construct(private int $id) {}
来源：http://poy.gaohongyu789.top

[U51] PHP：数组解构
来源：http://wnd.jqgufenzy.top

[$a, $b] = $arr;
来源：http://ovx.zdbjq.cn

[U52] PHP：箭头函数
来源：http://idp.tanke756.top

$double = fn($x) => $x * 2;
来源：http://jpb.xziqi.cn

[U53] PHP：空合并运算符
来源：http://jxb.zhongyouzk.top

$v = $a ?? $b ?? "default";
来源：http://ust.ydjk.org.cn

[U54] PHP：空安全调用
来源：http://soj.kuanghao11.cn

$obj?->method()
来源：http://kbo.cqqwz.cn

[U55] PHP：match 表达式
来源：http://loy.epnwcf.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iev.xziqi.cn

[U56] PHP：命名参数
来源：http://ftb.jinyuanbaomall.cn

f(a: 1, b: 2)
来源：http://fnl.shuidangran.top

[U57] PHP：字符串插值
来源：http://aiw.jinghuilouyu.cn

"值: {$a}"
来源：http://ikw.yanxiufei.cn

[U58] PHP：数组三件套
来源：http://ymc.ybcxt.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://spq.yangfankeji.com

[U59] PHP：自定义排序
来源：http://jcj.hesvh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bva.mhx1999.top

[U60] PHP：JSON 编解码
来源：http://ppz.yuxming.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uhz.guowangkeji.top

[U61] PHP：正则
来源：http://set.hywenlv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xqi.hongshengwenyu.top

[U62] PHP：日期对象
来源：http://pci.nanxinkj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jwa.ivvv.top

[U63] PHP：文件读写
来源：http://nzn.daria6918.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://osg.yj202588.top

[U64] PHP：目录遍历
来源：http://zow.xuanzx.com

glob("dir/*.php");  scandir("dir");
来源：http://oew.epnwcf.com

[U65] PHP：会话
来源：http://fgg.havefunace.top

session_start();  $_SESSION["uid"] = 1;
来源：http://tob.hongshengwenyu.top

[U66] PHP：设置 Cookie
来源：http://inp.zdbjq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://iwk.nanxinkj.top

[U67] PHP：处理文件上传
来源：http://xgb.feifeiyinyue.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ipp.ctjpmb.com

[U68] PHP：PDO 连接
来源：http://pxl.nanxuanxn.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vzd.xingfuxueyuan.xyz

[U69] PHP：PDO 预处理
来源：http://ayu.nwbrower.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dgd.chenlongwang.top

[U70] PHP：PDO 事务
来源：http://wku.52xcode.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zyw.xylfe.cn

[U71] PHP：抛出异常
来源：http://wll.pengpengdd.cyou

throw new RuntimeException("失败", 500);
来源：http://mod.cdnleiting.top

[U72] PHP：写错误日志
来源：http://ufc.shanyushiyangkeji.top

error_log("失败: " . $e->getMessage());
来源：http://hgm.yonumen.top

[U73] PHP：读取 ini 配置
来源：http://oew.hywenlv.cn

parse_ini_file("config.ini", true)
来源：http://uws.birdmap.top

[U74] PHP：读取环境变量
来源：http://esl.dashuyun.cn

getenv("APP_ENV") ?: "production"
来源：http://shk.xingfuxueyuan.xyz

[U75] PHP：依赖注入
来源：http://jin.aibaodan.cn

composer require psr/container
来源：http://aez.yj202588.top

[U76] PHP：简单路由
来源：http://vse.shangyingyoupin.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://brl.hywenlv.cn

[U77] PHP：模板渲染
来源：http://amx.aizwys.cn

composer require twig/twig
来源：http://puh.zdbjq.cn

[U78] PHP：单元测试
来源：http://xcc.yueranfly.top

composer require --dev phpunit/phpunit
来源：http://izs.wangdashe.top

[U79] PHP：静态分析
来源：http://jpn.birdmap.top

composer require --dev phpstan/phpstan
来源：http://etg.jinqigufen.top

[U80] PHP：代码规范修复
来源：http://keu.zhiwuduotai.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ivm.nanxinkj.top

[U81] JS：初始化项目
来源：http://chm.snrcjt.cn

npm init -y;  npm i express
来源：http://zni.mhx1999.top

[U82] JS：package.json 脚本
来源：http://dof.hnqzz.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://urg.xuanzx.com

[U83] JS：ES Module 导入导出
来源：http://jxs.yangfankeji.com

export const a = 1;  import { a } from "./m.js";
来源：http://zbt.vqdsnc.cn

[U84] JS：CommonJS 写法
来源：http://cxj.birdmap.top

module.exports = { a };  const { a } = require("./m");
来源：http://gtr.zhoulong.xyz

[U85] JS：可选链
来源：http://dqg.shzxlz.cn

a?.b?.c
来源：http://gin.yuanzhike.top

[U86] JS：空值合并
来源：http://ebx.fzhhl.top

a ?? b
来源：http://aqo.shzxlz.cn

[U87] JS：解构默认值
来源：http://jsv.snrcjt.cn

const { a = 1, b = 2 } = obj;
来源：http://egr.chenlongwang.top

[U88] JS：对象展开合并
来源：http://bvb.zhiwuduotai.top

{ ...a, ...b }
来源：http://qwb.iojbl.cn

[U89] JS：数组去重
来源：http://gdv.shanyushiyangtech.top

[...new Set(arr)]
来源：http://rzh.ehwqpu.com

[U90] JS：数字数组排序
来源：http://jkx.mhx1999.top

[...arr].sort((a, b) => a - b)
来源：http://vod.hywenlv.cn

[U91] JS：对象键值遍历
来源：http://qbc.zhengqikj.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ctt.chenjidiqi.icu

[U92] JS：深拷贝
来源：http://ltu.pycfn.com

structuredClone(obj)
来源：http://abd.jyoumei.cn

[U93] JS：模板字符串
来源：http://wre.hywenlv.cn

`共 ${n} 条`
来源：http://fcm.9152youxi.cn

[U94] JS：箭头函数
来源：http://xfx.mhx1999.top

const double = x => x * 2;
来源：http://wyh.yj202588.top

[U95] JS：Promise 包装
来源：http://kqc.ydzc1.top

new Promise((resolve, reject) => {})
来源：http://seb.zhongyouzk.top

[U96] JS：async/await 与异常
来源：http://yun.zhaomingkeji.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dwz.sufxvd.cn

[U97] JS：并发请求
来源：http://ykr.bjfxy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xlv.xinyue.icu

[U98] JS：fetch 带 JSON
来源：http://bky.sjlbkw.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gub.hnxiangtu.top

[U99] JS：事件监听
来源：http://mkx.gotoacloud.top

el.addEventListener("click", e => {})
来源：http://rkv.tian-w.cn

[U100] JS：DOM 查询
来源：http://pry.jinyuanbaomall.cn

document.querySelector(".item")
来源：http://yxn.jinqigfzy.top

[U101] JS：classList 操作
来源：http://jok.jinghuilouyu.cn

el.classList.toggle("active")
来源：http://sli.sysykeji.top

[U102] JS：本地存储
来源：http://tng.hammf.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://twg.fengsongda.top

[U103] JS：定时器
来源：http://uzd.feifeiyinyue.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vqq.fktsv.cn

[U104] JS：防抖
来源：http://vxf.aizwys.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://epw.ydjk.org.cn

[U105] JS：节流
来源：http://rfb.birdmap.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vem.yuanzhike.top

[U106] JS：日期格式化
来源：http://vjj.ctjpmb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wil.mhx1999.top

[U107] JS：数字千分位
来源：http://zrv.yj20258.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bos.aizwys.cn

[U108] JS：随机整数
来源：http://tau.tianlin.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fpm.tian-w.cn

[U109] JS：数组分组
来源：http://wmy.0kj1m.cn

Object.groupBy(arr, x => x.type)
来源：http://uvs.aizwys.cn

[U110] JS：数组分块
来源：http://xfx.xingfuxueyuan.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zam.nanxuanxn.top

[U111] JS：对象转 Map
来源：http://tcp.pycfn.com

new Map(Object.entries(obj))
来源：http://ufp.316326.xyz

[U112] JS：字符串补位
来源：http://trz.chenlongwang.top

"7".padStart(3, "0")
来源：http://uzz.fehbvm.com

[U113] JS：正则替换全部
来源：http://aei.cqqwz.cn

s.replaceAll("a", "b")
来源：http://nut.tian-w.cn

[U114] JS：JSON 深比较
来源：http://zzn.dashuyun.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://caf.chenlongwang.top

[U115] JS：生成 UUID
来源：http://mfc.fktsv.cn

crypto.randomUUID()
来源：http://keb.xuetiantiany.cn

[U116] JS：类型检查（JSDoc）
来源：http://ufd.yuxming.cn

/** @param {string} name */ function f(name) {}
来源：http://ikb.jqgfzy.top

[U117] JS：单元测试
来源：http://rwc.gzhubu.top

npm i -D vitest;  npx vitest
来源：http://cjv.fzhhl.top

[U118] JS：开发服务器
来源：http://plv.fengsongda.top

npm i -D vite;  npx vite
来源：http://vgv.52xcode.cn

[U119] JS：生产构建
来源：http://ubo.zdbjq.cn

npx vite build
来源：http://zcs.tanke756.top

[U120] JS：读取环境变量（Vite）
来源：http://ebw.vehdjk.com

import.meta.env.VITE_API_URL
来源：http://trm.cashguo.top

================================================================================
来源：http://cfb.andypj.xyz

统计汇总
来源：http://msn.nanxuanxn.top

================================================================================
来源：http://qru.cheryme.top

按语言统计（条）：
来源：http://uca.ppjwa.cn

Python ......... 252
来源：http://typ.ppjwa.cn

PHP ............ 252
来源：http://mel.zhengqikj.top

JavaScript ..... 252
来源：http://dom.0kj1m.cn

TypeScript ..... 212
来源：http://eop.zhongyouzk.top

Java ........... 212
来源：http://dmy.jinyuanbaomall.cn

Go ............. 212
来源：http://smg.hnqzz.top

Ruby ........... 212
来源：http://uvm.epnwcf.com

C# ............. 212
来源：http://zmb.52xcode.cn

C .............. 30
来源：http://poq.xuetiantiany.cn

C++ ............ 30
来源：http://rqz.fehbvm.com

SQL ............ 90
来源：http://gqx.shanyushiyangtech.top

Bash ........... 80
来源：http://kly.ydzc1.top

Kotlin ......... 15
来源：http://jlf.sxryk.cn

Swift .......... 15
来源：http://xpx.zhaomingkeji.xyz

Lua ............ 10
来源：http://gqm.snrcjt.cn

Perl ........... 10
来源：http://kfb.jqgfzy.top

Scala .......... 10
来源：http://vfg.shanyushiyangkeji.top

------------------------------------
来源：http://dpw.jinghuilouyu.cn

合计 ........... 2106 条
来源：http://nsc.sjlbkw.cn

按章节统计：
来源：http://hzr.zhongyouzk.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uqx.xziqi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://scv.ydjk.org.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ulb.daxiang520.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zyj.chenjidiqi.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dld.fengsongda.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rjx.xuetiantiany.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zjt.smart0.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ddt.sysykeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://huk.316326.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tgg.hywenlv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vfv.birdmap.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vrx.zhixingplan.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hgg.jlsjyb.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ntl.fengsongda.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gba.fanxiaobao.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tuw.hfpthk.cn

Q SQL 专题                              90
来源：http://tcn.tian-w.cn

R Bash 专题                             80
来源：http://lwv.52xcode.cn

S C / C++ 专题                          60
来源：http://wjc.cucudq.cn

T 其他语言补充                          60
来源：http://ulg.9152youxi.cn

U 高频实用片段                         120
来源：http://kyw.hesvh.cn

------------------------------------
来源：http://whm.hnqzz.top

合计                                  2106 条
来源：http://mxl.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://afu.ydzc1.top

使用提醒
来源：http://gee.fehbvm.com

--------------------------------------------------------------------------------
来源：http://ofm.hnqzz.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vnn.bjfxy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zol.ydzc1.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vdz.fanxiaobao.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://vqq.sjlbkw.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://clt.sweek.top

—— 文件结束 ——
来源：http://dqi.jlsjyb.cn

================================================================================
来源：http://sbl.aizwys.cn

程序语言常见例子速查手册（2024 版）
来源：http://zyd.dianchejie.cn

Common Programming Examples Cheat Book
来源：http://gvn.cdnleiting.top

================================================================================
来源：http://pbo.feifeiyinyue.top

【收录内容】
来源：http://vec.shanyushiyangtech.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://abu.ydjk.org.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hpe.gaohongyu789.top

SQL · Bash · C · C++
来源：http://fhn.gaohongyu789.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wwe.hcnkem.com

【使用说明】
来源：http://kuz.xuetiantiany.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://eft.sjlbkw.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xvq.sysykeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yve.zhiwuduotai.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qwh.ppjwa.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cfh.xinyue.icu

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wvr.yj20258888.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qfy.fengsongda.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nob.fengsongda.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://otz.hfpthk.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gng.hysaishi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pud.chenjidiqi.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uqi.hysaishi.cn

【文件统计】
来源：http://caj.hysaishi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pbv.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://erg.gaohongyu789.top

目  录
来源：http://kza.ybcxt.top

--------------------------------------------------------------------------------
来源：http://qrt.jqgufenzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://asj.316326.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bcc.aizwys.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hhl.feifeiyinyue.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rcl.yvedp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pyp.tian-w.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yvn.ppjwa.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vjl.shangyingyoupin.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hto.feifeiyinyue.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tnv.zhoulong.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ctp.daxiang520.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yck.cheryme.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tca.xylfe.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kio.birdmap.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ped.nwbrower.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sgb.fehbvm.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qjz.hnxiangtu.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qsf.ehwqpu.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://kia.quarkkingdee.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rtt.cqqwz.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://drr.hesvh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ntu.gotoacloud.top

================================================================================
来源：http://ctg.birdmap.top

A. 基础语法与类型
来源：http://alu.sufxvd.cn

================================================================================
来源：http://lbl.daxiang520.top

[A01] Hello World
来源：http://syh.jlsjyb.cn

Py:   print("Hello, World!")
来源：http://wkq.chenzaomai.com

PHP:  echo "Hello, World!";
来源：http://cus.ppjwa.cn

JS:   console.log("Hello, World!");
来源：http://jbb.jyoumei.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ekc.guowangkeji.top

Java: System.out.println("Hello, World!");
来源：http://ady.c1oappe.top

Go:   fmt.Println("Hello, World!")
来源：http://frs.xziqi.cn

Ruby: puts "Hello, World!"
来源：http://jjz.xinyue.icu

C#:   Console.WriteLine("Hello, World!");
来源：http://rwi.0kj1m.cn

[A02] 变量声明与赋值
来源：http://lab.gaohongyu789.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dhy.jqgfzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://lnz.yj202588.top

JS:   let name = "Alex"; const age = 20;
来源：http://olg.nanxinkj.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://njb.xylfe.cn

Java: String name = "Alex"; int age = 20;
来源：http://klm.jyoumei.cn

Go:   name := "Alex"; age := 20
来源：http://qrt.fktsv.cn

Ruby: name = "Alex"; age = 20
来源：http://hsl.hesvh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://lxs.daxiang520.top

[A03] 常量定义
来源：http://mpa.gzhubu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wsv.shangyingyoupin.top

PHP:  const PI = 3.14159;
来源：http://etk.jinghuilouyu.cn

JS:   const PI = 3.14159;
来源：http://uln.mhx1999.top

TS:   const PI: number = 3.14159;
来源：http://lhy.dashuyun.cn

Java: static final double PI = 3.14159;
来源：http://hhn.hcnkem.com

Go:   const PI = 3.14159
来源：http://ukj.daria6918.cn

Ruby: PI = 3.14159
来源：http://fat.bbcook.cn

C#:   const double PI = 3.14159;
来源：http://pzh.sjlbkw.cn

[A04] 判断变量类型
来源：http://edw.jinyuanbaomall.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mgv.yj20258.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vgp.hammf.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ppr.shanyushiyangtech.top

TS:   typeof x; x instanceof Date
来源：http://kzo.gzhubu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ilo.fktsv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ogc.tian-w.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fto.52xcode.cn

C#:   x.GetType().Name; x is int
来源：http://vea.kuanghao11.cn

[A05] 整数除法与取模
来源：http://kpk.yonumen.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://udk.yongpay.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jvv.redwolf501.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lbj.wangshuangyany.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dih.shanyushiyangkeji.top

Java: 7 / 2; 7 % 2
来源：http://ija.pengpengdd.cyou

Go:   7 / 2; 7 % 2
来源：http://vbk.andypj.xyz

Ruby: 7 / 2; 7 % 2
来源：http://fjx.cucudq.cn

C#:   7 / 2; 7 % 2
来源：http://vfe.daria6918.cn

[A06] 字符串转数字
来源：http://wsn.jianghu66.top

Py:   int("42"); float("3.14")
来源：http://fxx.iojbl.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gtl.yuanzhike.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tiq.epnwcf.com


<!-- 参考信息 -->