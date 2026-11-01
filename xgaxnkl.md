代发 wailian999

[U81] JS：初始化项目
来源：http://baike.sjlbkw.cn/Article/details/ghvdxtgay.sHtML

npm init -y;  npm i express
来源：http://www.share.tarul.cn/Article/details/gzlvnhqay.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.tarul.cn/Article/details/gvemgesrd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.sjlbkw.cn/Article/details/gdluwfwrr.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.yfazqb.com/Article/details/gorrtozum.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.vehdjk.com/Article/details/gotbjdmpj.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.yfazqb.com/Article/details/geviakctw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.tarul.cn/Article/details/gfgrwgyhb.sHtML

[U85] JS：可选链
来源：http://www.blog.epnwcf.com/Article/details/gwsmjigxs.sHtML

a?.b?.c
来源：http://www.share.bbcook.cn/Article/details/gbyzjbrue.sHtML

[U86] JS：空值合并
来源：http://wap.bbcook.cn/Article/details/gfjcvcfxv.sHtML

a ?? b
来源：http://www.share.bbcook.cn/Article/details/ghxvtnzuj.sHtML

[U87] JS：解构默认值
来源：http://read.share.bbcook.cn/Article/details/gibsgeqpu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.epnwcf.com/Article/details/gwtgeajva.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fktsv.cn/Article/details/gkggbcayl.sHtML

{ ...a, ...b }
来源：http://www.m.share.epnwcf.com/Article/details/gusghkecz.sHtML

[U89] JS：数组去重
来源：http://www.m.share.bbcook.cn/Article/details/gbrznffgo.sHtML

[...new Set(arr)]
来源：http://www.m.share.fktsv.cn/Article/details/gvlcqzmeh.sHtML

[U90] JS：数字数组排序
来源：http://read.share.vehdjk.com/Article/details/ghgewairk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/gdxgkandk.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.epnwcf.com/Article/details/gxtotfcfk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.epnwcf.com/Article/details/glvugjwnh.sHtML

[U92] JS：深拷贝
来源：http://wap.bbcook.cn/Article/details/gbcdxuihz.sHtML

structuredClone(obj)
来源：http://www.m.share.bbcook.cn/Article/details/givttmsiq.sHtML

[U93] JS：模板字符串
来源：http://www.share.bbcook.cn/Article/details/gfphrlasz.sHtML

`共 ${n} 条`
来源：http://read.share.vehdjk.com/Article/details/guczhtynd.sHtML

[U94] JS：箭头函数
来源：http://www.share.fktsv.cn/Article/details/gnttourjy.sHtML

const double = x => x * 2;
来源：http://read.share.vehdjk.com/Article/details/glqxkfesv.sHtML

[U95] JS：Promise 包装
来源：http://baike.epnwcf.com/Article/details/gclhscgmu.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.epnwcf.com/Article/details/glyjzgfrp.sHtML

[U96] JS：async/await 与异常
来源：http://baike.sjlbkw.cn/Article/details/gfopxogqe.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/gwggbdabk.sHtML

[U97] JS：并发请求
来源：http://baike.sjlbkw.cn/Article/details/gkfopomfx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/gtmittnnc.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fktsv.cn/Article/details/gjtrvxbky.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.bbcook.cn/Article/details/gfqiifdsr.sHtML

[U99] JS：事件监听
来源：http://m.share.tarul.cn/Article/details/gmzcuyfug.sHtML

el.addEventListener("click", e => {})
来源：http://blog.bbcook.cn/Article/details/gdqbtolgr.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.vehdjk.com/Article/details/gbuqgkchk.sHtML

document.querySelector(".item")
来源：http://wap.sjlbkw.cn/Article/details/gqsdgcyma.sHtML

[U101] JS：classList 操作
来源：http://wap.yfazqb.com/Article/details/gcufyiqmg.sHtML

el.classList.toggle("active")
来源：http://blog.vehdjk.com/Article/details/gqizmfued.sHtML

[U102] JS：本地存储
来源：http://3g.fktsv.cn/Article/details/gajwhotjf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.epnwcf.com/Article/details/gktfundky.sHtML

[U103] JS：定时器
来源：http://www.share.tarul.cn/Article/details/gjzwgxees.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.bbcook.cn/Article/details/gscpjwpuy.sHtML

[U104] JS：防抖
来源：http://www.share.sjlbkw.cn/Article/details/gvcarbrhb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/gxgbxxhtv.sHtML

[U105] JS：节流
来源：http://mobile.bbcook.cn/Article/details/gvqippjwm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.sjlbkw.cn/Article/details/gqveatusi.sHtML

[U106] JS：日期格式化
来源：http://blog.tarul.cn/Article/details/gyueuqdbs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.yfazqb.com/Article/details/gsfrzhxox.sHtML

[U107] JS：数字千分位
来源：http://m.share.yfazqb.com/Article/details/gdnxixahc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.bbcook.cn/Article/details/gxupxbntm.sHtML

[U108] JS：随机整数
来源：http://read.share.bbcook.cn/Article/details/gruvxkqed.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.epnwcf.com/Article/details/glawjrowt.sHtML

[U109] JS：数组分组
来源：http://mobile.epnwcf.com/Article/details/gawnuwgfx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.vehdjk.com/Article/details/grqabdqfm.sHtML

[U110] JS：数组分块
来源：http://mobile.bbcook.cn/Article/details/gkrknyque.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.yfazqb.com/Article/details/gcocivdts.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.bbcook.cn/Article/details/gunxmqbov.sHtML

new Map(Object.entries(obj))
来源：http://www.share.yfazqb.com/Article/details/ggsrastgs.sHtML

[U112] JS：字符串补位
来源：http://3g.epnwcf.com/Article/details/gipujtyxd.sHtML

"7".padStart(3, "0")
来源：http://www.share.fktsv.cn/Article/details/geexemgzq.sHtML

[U113] JS：正则替换全部
来源：http://3g.tarul.cn/Article/details/gysysgxsc.sHtML

s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/ghkwhnvsm.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.bbcook.cn/Article/details/giakejtze.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/gypmuatte.sHtML

[U115] JS：生成 UUID
来源：http://mobile.epnwcf.com/Article/details/geparfbfy.sHtML

crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/ghpkavbkt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.yfazqb.com/Article/details/gewmnluyx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.bbcook.cn/Article/details/gyzdokaaz.sHtML

[U117] JS：单元测试
来源：http://www.share.tarul.cn/Article/details/gigdlxqls.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.tarul.cn/Article/details/gawzvaiqx.sHtML

[U118] JS：开发服务器
来源：http://wap.tarul.cn/Article/details/gmqwifwja.sHtML

npm i -D vite;  npx vite
来源：http://read.share.bbcook.cn/Article/details/gweutjatt.sHtML

[U119] JS：生产构建
来源：http://www.share.sjlbkw.cn/Article/details/grigpyiks.sHtML

npx vite build
来源：http://read.share.sjlbkw.cn/Article/details/gtsqztwtw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.yfazqb.com/Article/details/gmkkkkyhw.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.tarul.cn/Article/details/gyfxxnpti.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ggtqhjfbk.sHtML

统计汇总
来源：http://blog.tarul.cn/Article/details/gdwehkopa.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gztauqxdf.sHtML

按语言统计（条）：
来源：http://wap.sjlbkw.cn/Article/details/gcspbubkn.sHtML

Python ......... 252
来源：http://blog.fktsv.cn/Article/details/guswupfud.sHtML

PHP ............ 252
来源：http://www.m.share.fktsv.cn/Article/details/gmxzvlqjm.sHtML

JavaScript ..... 252
来源：http://m.share.tarul.cn/Article/details/gncvqktex.sHtML

TypeScript ..... 212
来源：http://wap.sjlbkw.cn/Article/details/gybihrwjj.sHtML

Java ........... 212
来源：http://www.share.fktsv.cn/Article/details/gnebyhgvw.sHtML

Go ............. 212
来源：http://3g.fktsv.cn/Article/details/grqdlpbol.sHtML

Ruby ........... 212
来源：http://www.share.yfazqb.com/Article/details/gpsuqtzbd.sHtML

C# ............. 212
来源：http://blog.bbcook.cn/Article/details/gilctqkmf.sHtML

C .............. 30
来源：http://www.m.share.yfazqb.com/Article/details/gtoxxyzie.sHtML

C++ ............ 30
来源：http://read.share.sjlbkw.cn/Article/details/ghsgaitir.sHtML

SQL ............ 90
来源：http://wap.epnwcf.com/Article/details/gtezqxqkj.sHtML

Bash ........... 80
来源：http://m.share.epnwcf.com/Article/details/gjeqymkjn.sHtML

Kotlin ......... 15
来源：http://m.share.epnwcf.com/Article/details/gyqdqlhpi.sHtML

Swift .......... 15
来源：http://www.blog.tarul.cn/Article/details/ghqbqgenf.sHtML

Lua ............ 10
来源：http://read.share.fktsv.cn/Article/details/gwqddxtif.sHtML

Perl ........... 10
来源：http://3g.epnwcf.com/Article/details/gorcxjuht.sHtML

Scala .......... 10
来源：http://wap.vehdjk.com/Article/details/gcaltirxd.sHtML

------------------------------------
来源：http://www.share.tarul.cn/Article/details/gbnrtengo.sHtML

合计 ........... 2106 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpvdsify.sHtML

按章节统计：
来源：http://www.m.share.tarul.cn/Article/details/gfyreclwn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.sjlbkw.cn/Article/details/gscbsslyv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.vehdjk.com/Article/details/gbswfifdw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fktsv.cn/Article/details/gulrjjemv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.bbcook.cn/Article/details/gyzohjamq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.epnwcf.com/Article/details/ggvyyzdsj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.vehdjk.com/Article/details/gjvlbborp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.sjlbkw.cn/Article/details/gkghjapsc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.tarul.cn/Article/details/gueuhzynw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gykevkuwz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.vehdjk.com/Article/details/gisrytvww.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/geyljwoeg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gtytwohfu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fktsv.cn/Article/details/geyafpzkf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.epnwcf.com/Article/details/gerliysjd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.sjlbkw.cn/Article/details/gmktfcoqy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gzfsxkmva.sHtML

Q SQL 专题                              90
来源：http://baike.vehdjk.com/Article/details/gtcxdxsgk.sHtML

R Bash 专题                             80
来源：http://read.share.tarul.cn/Article/details/gupevpgto.sHtML

S C / C++ 专题                          60
来源：http://read.share.yfazqb.com/Article/details/gqrgrqrhd.sHtML

T 其他语言补充                          60
来源：http://baike.epnwcf.com/Article/details/gbsesrmpe.sHtML

U 高频实用片段                         120
来源：http://m.share.tarul.cn/Article/details/gjszxtdsa.sHtML

------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gstqbmnxf.sHtML

合计                                  2106 条
来源：http://blog.sjlbkw.cn/Article/details/gnqxlwtra.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gtoivuwxk.sHtML

使用提醒
来源：http://www.share.yfazqb.com/Article/details/gierxizlg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gitpryroi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.sjlbkw.cn/Article/details/gjgyhofjj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.tarul.cn/Article/details/gquzamcjv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.sjlbkw.cn/Article/details/gjezsvgnh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.sjlbkw.cn/Article/details/gesfcumid.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.bbcook.cn/Article/details/gzsaxhidf.sHtML

—— 文件结束 ——
来源：http://www.m.share.epnwcf.com/Article/details/gvdnfdcfz.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ggftzksvt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.bbcook.cn/Article/details/grdkylnum.sHtML

Common Programming Examples Cheat Book
来源：http://wap.bbcook.cn/Article/details/gpnmfpnaz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gumamqefa.sHtML

【收录内容】
来源：http://www.share.tarul.cn/Article/details/gfnoznddo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.epnwcf.com/Article/details/gnumybrfg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.vehdjk.com/Article/details/gzaxxnzbg.sHtML

SQL · Bash · C · C++
来源：http://baike.epnwcf.com/Article/details/gcomfgxmm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.tarul.cn/Article/details/gaacrmtgl.sHtML

【使用说明】
来源：http://blog.tarul.cn/Article/details/gwxclyopx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.yfazqb.com/Article/details/gqwhvgxvl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.epnwcf.com/Article/details/gedzcrvpe.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.epnwcf.com/Article/details/ghfgqvfah.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.bbcook.cn/Article/details/gmhqjgwiz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.sjlbkw.cn/Article/details/gguvvkqmp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fktsv.cn/Article/details/gscziwtln.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.tarul.cn/Article/details/gohsvcmry.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.tarul.cn/Article/details/grznsvvaj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.sjlbkw.cn/Article/details/geiphzxvq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.tarul.cn/Article/details/gvlvteaby.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.bbcook.cn/Article/details/gqtxzknbt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fktsv.cn/Article/details/gbqbagreq.sHtML

【文件统计】
来源：http://www.blog.sjlbkw.cn/Article/details/gawscgrxn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.tarul.cn/Article/details/gjfwvrets.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.tarul.cn/Article/details/ggohxriej.sHtML

目  录
来源：http://www.share.yfazqb.com/Article/details/gyisznnyt.sHtML

--------------------------------------------------------------------------------
来源：http://wap.yfazqb.com/Article/details/gubnunxub.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.yfazqb.com/Article/details/gugqiicxq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.yfazqb.com/Article/details/gzzhuczib.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fktsv.cn/Article/details/ghylpudel.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.epnwcf.com/Article/details/ggoavyoof.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.bbcook.cn/Article/details/guzfatdcz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fktsv.cn/Article/details/gwyfmbqrr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.bbcook.cn/Article/details/gpzuixwum.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.epnwcf.com/Article/details/gylexuusj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.epnwcf.com/Article/details/gwsynsruh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fktsv.cn/Article/details/gvzodfelg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.epnwcf.com/Article/details/ggdsvxjer.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/gyudjnjmh.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gmjsxrvyp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.tarul.cn/Article/details/gsdiehdaw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.tarul.cn/Article/details/gfqdxbvsw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.yfazqb.com/Article/details/gfcgudoab.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.vehdjk.com/Article/details/gxyrzhsmo.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fktsv.cn/Article/details/gdqzzsfuu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gkyfafwxi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.yfazqb.com/Article/details/guxwntwqi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.vehdjk.com/Article/details/gnxraztiq.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gkjoxqnui.sHtML

A. 基础语法与类型
来源：http://blog.yfazqb.com/Article/details/gtwdlopjg.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/guyuyzogz.sHtML

[A01] Hello World
来源：http://3g.vehdjk.com/Article/details/gvwhmqxjr.sHtML

Py:   print("Hello, World!")
来源：http://wap.sjlbkw.cn/Article/details/gifxpwjwu.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.bbcook.cn/Article/details/gaqmcveib.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.bbcook.cn/Article/details/glnomldta.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.tarul.cn/Article/details/gwjqnvtko.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.epnwcf.com/Article/details/gtrpgbjjp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.vehdjk.com/Article/details/ghulilket.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.vehdjk.com/Article/details/gduzmbdga.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fktsv.cn/Article/details/gouphhyre.sHtML

[A02] 变量声明与赋值
来源：http://m.share.sjlbkw.cn/Article/details/gkyxhymil.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fktsv.cn/Article/details/gmdyvczql.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.epnwcf.com/Article/details/gyeyrokuk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.epnwcf.com/Article/details/gliylnbuj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.yfazqb.com/Article/details/gequntvfh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.sjlbkw.cn/Article/details/guwsrudje.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.bbcook.cn/Article/details/grjpxibmh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.bbcook.cn/Article/details/gvhciwvqc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.yfazqb.com/Article/details/gorqfrjkp.sHtML

[A03] 常量定义
来源：http://baike.yfazqb.com/Article/details/gfydchcea.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.bbcook.cn/Article/details/gzamkravw.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gdozngawt.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/grshplcqi.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gvjsqjywi.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/grjlufikv.sHtML

Go:   const PI = 3.14159
来源：http://baike.epnwcf.com/Article/details/gzfqeilzp.sHtML

Ruby: PI = 3.14159
来源：http://m.share.tarul.cn/Article/details/gmdghgijj.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/giqslxdkb.sHtML

[A04] 判断变量类型
来源：http://read.share.epnwcf.com/Article/details/gycxqqugw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fktsv.cn/Article/details/gfpvecujy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.sjlbkw.cn/Article/details/gopwktsws.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.epnwcf.com/Article/details/gdkkgsjje.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.tarul.cn/Article/details/gdcovnjmh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.vehdjk.com/Article/details/giytzftde.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.yfazqb.com/Article/details/gimfirrla.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fktsv.cn/Article/details/gpscqxllu.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.vehdjk.com/Article/details/gqybdxhze.sHtML

[A05] 整数除法与取模
来源：http://3g.epnwcf.com/Article/details/gkgiogtru.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fktsv.cn/Article/details/gztofaytf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gtgqmkvqj.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fktsv.cn/Article/details/gdkywzlxe.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.bbcook.cn/Article/details/gkevgehcb.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.yfazqb.com/Article/details/gbjdkqeal.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gigzbbxna.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.tarul.cn/Article/details/giukczwvk.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fktsv.cn/Article/details/gtlvzstfa.sHtML

[A06] 字符串转数字
来源：http://mobile.bbcook.cn/Article/details/gtkhyufgf.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.tarul.cn/Article/details/gqerluqwd.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fktsv.cn/Article/details/glkrherhu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fktsv.cn/Article/details/gjnbacydp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fktsv.cn/Article/details/gonmcmokp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fktsv.cn/Article/details/goruiocaa.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.vehdjk.com/Article/details/gdrxifbye.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.vehdjk.com/Article/details/gesommezl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.fktsv.cn/Article/details/gbjxcblsz.sHtML

[A07] 数字转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gzmifkdsv.sHtML

Py:   str(42)
来源：http://blog.bbcook.cn/Article/details/gujjjgdue.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.bbcook.cn/Article/details/gcexlmmes.sHtML

JS:   String(42); (42).toString()
来源：http://baike.bbcook.cn/Article/details/gmonrzfll.sHtML

TS:   String(42)
来源：http://baike.fktsv.cn/Article/details/grfiswezr.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.sjlbkw.cn/Article/details/gobsajevw.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.yfazqb.com/Article/details/ggzzdkyko.sHtML

Ruby: 42.to_s
来源：http://mobile.sjlbkw.cn/Article/details/gkuernqlh.sHtML

C#:   42.ToString()
来源：http://blog.epnwcf.com/Article/details/gincrgwrv.sHtML

[A08] 取整与四舍五入
来源：http://m.share.sjlbkw.cn/Article/details/gasoriklx.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/gxzztpyka.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fktsv.cn/Article/details/gizcolbav.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.epnwcf.com/Article/details/gkpxvxkxi.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fktsv.cn/Article/details/gybtalbxq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/gbseqasta.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.epnwcf.com/Article/details/ggavpcmfd.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fktsv.cn/Article/details/gopgvmpln.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.yfazqb.com/Article/details/gufwmfznt.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.sjlbkw.cn/Article/details/ggeqjulbb.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gfsdddohr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.tarul.cn/Article/details/gxcaqeqmn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.vehdjk.com/Article/details/gufqkcbpi.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/gnvgxqrsz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.epnwcf.com/Article/details/ghmlobqvj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.tarul.cn/Article/details/gcsrerucl.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.epnwcf.com/Article/details/gjkxeajhh.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gwuapjbwo.sHtML

[A10] 生成随机数
来源：http://wap.yfazqb.com/Article/details/gdxrdfqnz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.sjlbkw.cn/Article/details/glaagzlfy.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.tarul.cn/Article/details/goimzxnvr.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.yfazqb.com/Article/details/gwootazac.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fktsv.cn/Article/details/gjptmvxmu.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.vehdjk.com/Article/details/gviovwyqa.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.yfazqb.com/Article/details/gsglnxkdt.sHtML

Ruby: rand(1..100)
来源：http://m.share.vehdjk.com/Article/details/gwgjofhuo.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.sjlbkw.cn/Article/details/gxgqgtivu.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.yfazqb.com/Article/details/gtnnvssvv.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.epnwcf.com/Article/details/godtlfssx.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.yfazqb.com/Article/details/gqjhahkgd.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.sjlbkw.cn/Article/details/gtkrymdxg.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.fktsv.cn/Article/details/gflnqnomn.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gentzpbhn.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.yfazqb.com/Article/details/gbrlbyyjg.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.tarul.cn/Article/details/gjyeupnas.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.fktsv.cn/Article/details/gmxlfxygj.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.sjlbkw.cn/Article/details/gysdrchjb.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fktsv.cn/Article/details/gssjcphcu.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.sjlbkw.cn/Article/details/gtxoaivjq.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.vehdjk.com/Article/details/guixvcvsp.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.bbcook.cn/Article/details/gfzkzvksh.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.tarul.cn/Article/details/gmpsmhatg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.vehdjk.com/Article/details/gfqjmxdxb.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fktsv.cn/Article/details/gkcgrmrij.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.bbcook.cn/Article/details/gfyfkcynw.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.vehdjk.com/Article/details/gnxkswszz.sHtML

Py:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gwqaxrhsq.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gqmrjvxuk.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gazuojroo.sHtML

TS:   "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/goamxmdhh.sHtML


<!-- 参考信息 -->