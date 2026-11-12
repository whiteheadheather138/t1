代发 wailian999

[U53] PHP：空合并运算符
来源：http://auy.birdmap.top

$v = $a ?? $b ?? "default";
来源：http://rck.hammf.cn

[U54] PHP：空安全调用
来源：http://vau.guowangkeji.top

$obj?->method()
来源：http://ukn.smart0.xyz

[U55] PHP：match 表达式
来源：http://iry.cashguo.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vpf.fehbvm.com

[U56] PHP：命名参数
来源：http://evf.fengsongda.top

f(a: 1, b: 2)
来源：http://pxc.aizwys.cn

[U57] PHP：字符串插值
来源：http://spy.yueranfly.top

"值: {$a}"
来源：http://gkj.jqgfzy.top

[U58] PHP：数组三件套
来源：http://qgn.hammf.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gtp.andypj.xyz

[U59] PHP：自定义排序
来源：http://clr.gogol.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ohd.jiagoushi.top

[U60] PHP：JSON 编解码
来源：http://sav.cheryme.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pej.fehbvm.com

[U61] PHP：正则
来源：http://qgm.vehdjk.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ngz.wangshuangyany.cn

[U62] PHP：日期对象
来源：http://kdn.yuxming.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yuy.yanxiufei.cn

[U63] PHP：文件读写
来源：http://pxj.wangdashe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qjb.zdbjq.cn

[U64] PHP：目录遍历
来源：http://wvw.gzhubu.top

glob("dir/*.php");  scandir("dir");
来源：http://edd.tianlin.xyz

[U65] PHP：会话
来源：http://ubk.svipenyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://iey.fehbvm.com

[U66] PHP：设置 Cookie
来源：http://lvd.pengpengdd.cyou

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nub.ydzc1.top

[U67] PHP：处理文件上传
来源：http://ocz.smart0.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nxs.zycfv.cn

[U68] PHP：PDO 连接
来源：http://fuz.hammf.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uia.cheryme.top

[U69] PHP：PDO 预处理
来源：http://gpx.aibaodan.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gof.tanke756.top

[U70] PHP：PDO 事务
来源：http://ssm.sweek.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wwc.pycfn.com

[U71] PHP：抛出异常
来源：http://vug.guowangkeji.top

throw new RuntimeException("失败", 500);
来源：http://vbq.jinqigufen.top

[U72] PHP：写错误日志
来源：http://xyn.fzhhl.top

error_log("失败: " . $e->getMessage());
来源：http://nrw.feifeiyinyue.top

[U73] PHP：读取 ini 配置
来源：http://hns.jlsjyb.cn

parse_ini_file("config.ini", true)
来源：http://hou.haohaochexian.top

[U74] PHP：读取环境变量
来源：http://znr.shangyingyoupin.top

getenv("APP_ENV") ?: "production"
来源：http://kom.jqgfzy.top

[U75] PHP：依赖注入
来源：http://rpx.yj202588.top

composer require psr/container
来源：http://aox.cucudq.cn

[U76] PHP：简单路由
来源：http://ecb.tianlin.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rdo.shanyushiyangkeji.top

[U77] PHP：模板渲染
来源：http://rtp.daxiang520.top

composer require twig/twig
来源：http://ydi.jinghuilouyu.cn

[U78] PHP：单元测试
来源：http://igr.tarul.cn

composer require --dev phpunit/phpunit
来源：http://hjh.cqqwz.cn

[U79] PHP：静态分析
来源：http://cvj.zhiwuduotai.top

composer require --dev phpstan/phpstan
来源：http://gfw.ppjwa.cn

[U80] PHP：代码规范修复
来源：http://tnb.jinghuilouyu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pjp.hfpthk.cn

[U81] JS：初始化项目
来源：http://ovp.vehdjk.com

npm init -y;  npm i express
来源：http://rol.jqgfzy.top

[U82] JS：package.json 脚本
来源：http://shs.ivvv.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://orz.hysaishi.cn

[U83] JS：ES Module 导入导出
来源：http://cwp.yj202588.top

export const a = 1;  import { a } from "./m.js";
来源：http://eoe.gotoacloud.top

[U84] JS：CommonJS 写法
来源：http://mek.hammf.cn

module.exports = { a };  const { a } = require("./m");
来源：http://guy.yueranfly.top

[U85] JS：可选链
来源：http://qsk.zhaomingkeji.xyz

a?.b?.c
来源：http://ynx.snrcjt.cn

[U86] JS：空值合并
来源：http://cty.xylfe.cn

a ?? b
来源：http://dke.xuanzx.com

[U87] JS：解构默认值
来源：http://cfx.zhiwuduotai.top

const { a = 1, b = 2 } = obj;
来源：http://oux.yj202588.top

[U88] JS：对象展开合并
来源：http://lox.ctjpmb.com

{ ...a, ...b }
来源：http://jxe.hnxiangtu.top

[U89] JS：数组去重
来源：http://deb.yj202588.top

[...new Set(arr)]
来源：http://xfo.hfpthk.cn

[U90] JS：数字数组排序
来源：http://ywv.ywan-chungtsiang.top

[...arr].sort((a, b) => a - b)
来源：http://ttn.tarul.cn

[U91] JS：对象键值遍历
来源：http://rqu.jinqigfzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xlx.zhijiandao.cn

[U92] JS：深拷贝
来源：http://irl.yj202588.top

structuredClone(obj)
来源：http://kqs.chenlongwang.top

[U93] JS：模板字符串
来源：http://dvl.yj20258.top

`共 ${n} 条`
来源：http://isq.gaohongyu789.top

[U94] JS：箭头函数
来源：http://fnv.jiagoushi.top

const double = x => x * 2;
来源：http://zfh.ydzc1.top

[U95] JS：Promise 包装
来源：http://cuk.bbcook.cn

new Promise((resolve, reject) => {})
来源：http://unp.zhixingplan.top

[U96] JS：async/await 与异常
来源：http://apw.9152youxi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yks.zhongyouzk.top

[U97] JS：并发请求
来源：http://ibk.uphjek.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://ick.tanke756.top

[U98] JS：fetch 带 JSON
来源：http://ujz.yj202588.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://arx.kuanghao11.cn

[U99] JS：事件监听
来源：http://ivg.jinqigufen.top

el.addEventListener("click", e => {})
来源：http://wji.hysaishi.cn

[U100] JS：DOM 查询
来源：http://opp.yj20258.top

document.querySelector(".item")
来源：http://bin.hnqzz.top

[U101] JS：classList 操作
来源：http://otp.aibaodan.cn

el.classList.toggle("active")
来源：http://ddr.gzhubu.top

[U102] JS：本地存储
来源：http://hlt.ctjpmb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://gaz.shangyingyoupin.top

[U103] JS：定时器
来源：http://oly.fengsongda.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uxs.yongpay.top

[U104] JS：防抖
来源：http://pwz.jinghuilouyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yns.cashguo.top

[U105] JS：节流
来源：http://xat.jqgfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tic.jianghu66.top

[U106] JS：日期格式化
来源：http://dma.uphjek.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://woi.yvedp.cn

[U107] JS：数字千分位
来源：http://fbe.cdnleiting.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bjo.ydzc1.top

[U108] JS：随机整数
来源：http://pzk.quarkkingdee.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ejb.zhongyouzk.top

[U109] JS：数组分组
来源：http://woj.havefunace.top

Object.groupBy(arr, x => x.type)
来源：http://bry.cdnleiting.top

[U110] JS：数组分块
来源：http://nxs.gotoacloud.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://miz.jianghu66.top

[U111] JS：对象转 Map
来源：http://vuu.jyoumei.cn

new Map(Object.entries(obj))
来源：http://bys.shangyingyoupin.top

[U112] JS：字符串补位
来源：http://zbd.yueranfly.top

"7".padStart(3, "0")
来源：http://dlq.zhixingplan.top

[U113] JS：正则替换全部
来源：http://nfk.cheryme.top

s.replaceAll("a", "b")
来源：http://pcu.0kj1m.cn

[U114] JS：JSON 深比较
来源：http://qnv.nanxinkj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rqk.xuanzx.com

[U115] JS：生成 UUID
来源：http://xhe.xuetiantiany.cn

crypto.randomUUID()
来源：http://ybe.kuanghao11.cn

[U116] JS：类型检查（JSDoc）
来源：http://pfr.chenlongwang.top

/** @param {string} name */ function f(name) {}
来源：http://mam.bbcook.cn

[U117] JS：单元测试
来源：http://rwq.tanke756.top

npm i -D vitest;  npx vitest
来源：http://lci.c1oappe.top

[U118] JS：开发服务器
来源：http://nlx.jianghu66.top

npm i -D vite;  npx vite
来源：http://ujj.316326.xyz

[U119] JS：生产构建
来源：http://emr.epnwcf.com

npx vite build
来源：http://qpu.quarkkingdee.top

[U120] JS：读取环境变量（Vite）
来源：http://mba.feifeiyinyue.top

import.meta.env.VITE_API_URL
来源：http://rlt.shangyingyoupin.top

================================================================================
来源：http://gye.fzhhl.top

统计汇总
来源：http://cex.yuxming.cn

================================================================================
来源：http://mmo.epnwcf.com

按语言统计（条）：
来源：http://gof.daxiang520.top

Python ......... 252
来源：http://gyy.uphjek.com

PHP ............ 252
来源：http://zrt.fehbvm.com

JavaScript ..... 252
来源：http://lgu.shanyushiyangkeji.top

TypeScript ..... 212
来源：http://ocs.hfpthk.cn

Java ........... 212
来源：http://hor.fzhhl.top

Go ............. 212
来源：http://ots.gogol.net.cn

Ruby ........... 212
来源：http://tth.quarkkingdee.top

C# ............. 212
来源：http://cgz.yuanzhike.top

C .............. 30
来源：http://cwn.wangdashe.top

C++ ............ 30
来源：http://bwi.iojbl.cn

SQL ............ 90
来源：http://iom.cdnleiting.top

Bash ........... 80
来源：http://dqv.hnqzz.top

Kotlin ......... 15
来源：http://tac.yj202588.top

Swift .......... 15
来源：http://qlv.wangshuangyany.cn

Lua ............ 10
来源：http://vmq.bjfxy.top

Perl ........... 10
来源：http://udx.cashguo.top

Scala .......... 10
来源：http://uwl.gaohongyu789.top

------------------------------------
来源：http://jul.fzhhl.top

合计 ........... 2106 条
来源：http://amq.daxiang520.top

按章节统计：
来源：http://znr.pengpengdd.cyou

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hww.cashguo.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wtw.feifeiyinyue.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nxl.shanyushiyangtech.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gdn.yonumen.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yef.cdnleiting.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wmh.hongshengwenyu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://odf.gotoacloud.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://veq.c1oappe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yyl.52xcode.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ecx.haohaochexian.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ybz.ivvv.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cnt.gogol.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wfh.sxryk.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://biq.shzxlz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pfd.sjlbkw.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://spv.9152youxi.cn

Q SQL 专题                              90
来源：http://opk.52xcode.cn

R Bash 专题                             80
来源：http://dtp.sjlbkw.cn

S C / C++ 专题                          60
来源：http://ixd.redwolf501.top

T 其他语言补充                          60
来源：http://yyx.zdbjq.cn

U 高频实用片段                         120
来源：http://sai.ehwqpu.com

------------------------------------
来源：http://cpp.vqdsnc.cn

合计                                  2106 条
来源：http://pdq.xziqi.cn

--------------------------------------------------------------------------------
来源：http://ony.chenzaomai.com

使用提醒
来源：http://zeo.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://kyh.sweek.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://khu.meibo888.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rwk.xingfuxueyuan.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zpz.ydzc1.top

在旧版本上使用前请先确认语法支持情况。
来源：http://wkn.yuxming.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pwu.tian-w.cn

—— 文件结束 ——
来源：http://gca.cdnleiting.top

================================================================================
来源：http://kul.gogol.net.cn

程序语言常见例子速查手册（2024 版）
来源：http://sbh.chenlongwang.top

Common Programming Examples Cheat Book
来源：http://ftk.cqqwz.cn

================================================================================
来源：http://bdx.fengsongda.top

【收录内容】
来源：http://bez.fzhhl.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://yvb.sufxvd.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xrc.zhengqikj.top

SQL · Bash · C · C++
来源：http://tiu.xuanzx.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gvg.zhongyouzk.top

【使用说明】
来源：http://tlu.nanxinkj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://umv.zdbjq.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dba.daria6918.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://frr.yonumen.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://owg.dashuyun.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lna.gaohongyu789.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tsb.pengpengdd.cyou

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://axr.yvedp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pwf.shangyingyoupin.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sdq.yonumen.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://toe.bbcook.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mgr.hywenlv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cds.zhixingplan.top

【文件统计】
来源：http://yyn.9152youxi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zsa.daxiang520.top

--------------------------------------------------------------------------------
来源：http://tqr.gaohongyu789.top

目  录
来源：http://gjz.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://hui.ehwqpu.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://msg.yangfankeji.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xeb.xingfuxueyuan.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xmr.gogol.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vwf.feifeiyinyue.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fzm.quarkkingdee.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kvi.jyoumei.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qnl.yonumen.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://voz.yuanzhike.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qti.havefunace.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yku.zhaomingkeji.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bze.chenjidiqi.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://eox.xylfe.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mas.jlsjyb.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tgg.daxiang520.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fbu.sjlbkw.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kqn.sweek.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yuv.316326.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://kin.guowangkeji.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pze.cucudq.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ehm.sxryk.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hib.yj202588.top

================================================================================
来源：http://hkt.snrcjt.cn

A. 基础语法与类型
来源：http://vsz.yj20258.top

================================================================================
来源：http://atn.xuetiantiany.cn

[A01] Hello World
来源：http://okp.9152youxi.cn

Py:   print("Hello, World!")
来源：http://ziy.vqdsnc.cn

PHP:  echo "Hello, World!";
来源：http://wbo.sxryk.cn

JS:   console.log("Hello, World!");
来源：http://nep.andypj.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ene.ehwqpu.com

Java: System.out.println("Hello, World!");
来源：http://owz.fengsongda.top

Go:   fmt.Println("Hello, World!")
来源：http://cae.feifeiyinyue.top

Ruby: puts "Hello, World!"
来源：http://zct.iojbl.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vow.zycfv.cn

[A02] 变量声明与赋值
来源：http://yyf.yj20258.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zsn.vehdjk.com

PHP:  $name = "Alex"; $age = 20;
来源：http://wow.ctjpmb.com

JS:   let name = "Alex"; const age = 20;
来源：http://nxy.wangdashe.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hxu.epnwcf.com

Java: String name = "Alex"; int age = 20;
来源：http://zwg.sysykeji.top

Go:   name := "Alex"; age := 20
来源：http://aqu.zhaomingkeji.xyz

Ruby: name = "Alex"; age = 20
来源：http://dbz.0kj1m.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ayz.yuanzhike.top

[A03] 常量定义
来源：http://xco.gzhubu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ihv.dashuyun.cn

PHP:  const PI = 3.14159;
来源：http://rus.tian-w.cn

JS:   const PI = 3.14159;
来源：http://cnp.cdnleiting.top

TS:   const PI: number = 3.14159;
来源：http://zqb.tarul.cn

Java: static final double PI = 3.14159;
来源：http://fca.fzhhl.top

Go:   const PI = 3.14159
来源：http://lut.hesvh.cn

Ruby: PI = 3.14159
来源：http://yzo.sjlbkw.cn

C#:   const double PI = 3.14159;
来源：http://ckh.gotoacloud.top

[A04] 判断变量类型
来源：http://tsp.yongpay.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://zxg.hysaishi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hnqzz.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://aso.zhijiandao.cn

TS:   typeof x; x instanceof Date
来源：http://dun.9152youxi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qbf.ydjk.org.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ehc.birdmap.top

Ruby: x.class; x.is_a?(Integer)
来源：http://cpl.jinqigufen.top

C#:   x.GetType().Name; x is int
来源：http://brm.cucudq.cn

[A05] 整数除法与取模
来源：http://mma.aizwys.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fji.chenzaomai.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://xei.gogol.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hig.nanxinkj.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bis.yvedp.cn

Java: 7 / 2; 7 % 2
来源：http://kxb.havefunace.top

Go:   7 / 2; 7 % 2
来源：http://pol.hywenlv.cn

Ruby: 7 / 2; 7 % 2
来源：http://mpj.cheryme.top

C#:   7 / 2; 7 % 2
来源：http://auy.c1oappe.top

[A06] 字符串转数字
来源：http://slo.vehdjk.com

Py:   int("42"); float("3.14")
来源：http://spx.nanxuanxn.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dgh.yj20258.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ycx.svipenyu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://dtk.mhx1999.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kvh.smart0.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kxx.pycfn.com

Ruby: "42".to_i; "3.14".to_f
来源：http://fgz.aizwys.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://okd.c1oappe.top

[A07] 数字转字符串
来源：http://eza.epnwcf.com

Py:   str(42)
来源：http://vwl.guannengcc.top

PHP:  (string) 42; strval(42)
来源：http://yvv.ywan-chungtsiang.top


<!-- 参考信息 -->