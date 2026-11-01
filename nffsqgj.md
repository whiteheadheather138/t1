代发 wailian999

[U89] JS：数组去重
来源：http://blog.bbcook.cn/Article/details/gyhuzrrma.sHtML

[...new Set(arr)]
来源：http://wap.fktsv.cn/Article/details/ghnfppkvz.sHtML

[U90] JS：数字数组排序
来源：http://3g.bbcook.cn/Article/details/gppaoeqab.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gztgccfpe.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.sjlbkw.cn/Article/details/gjqvaowxv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.epnwcf.com/Article/details/gimzufulu.sHtML

[U92] JS：深拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gycukfdxz.sHtML

structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/gorwsqtvm.sHtML

[U93] JS：模板字符串
来源：http://www.share.tarul.cn/Article/details/gytndtpuy.sHtML

`共 ${n} 条`
来源：http://m.share.bbcook.cn/Article/details/ggetiuypk.sHtML

[U94] JS：箭头函数
来源：http://baike.bbcook.cn/Article/details/gnadkapmm.sHtML

const double = x => x * 2;
来源：http://wap.bbcook.cn/Article/details/ghrotqpng.sHtML

[U95] JS：Promise 包装
来源：http://mobile.vehdjk.com/Article/details/ggywbfsws.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.bbcook.cn/Article/details/grllhyemk.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.yfazqb.com/Article/details/gwpnwgjjs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gzpzdauts.sHtML

[U97] JS：并发请求
来源：http://m.share.fktsv.cn/Article/details/gqtjpyglm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gefrkoicq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.tarul.cn/Article/details/gufnqypij.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.bbcook.cn/Article/details/guzgbkgbk.sHtML

[U99] JS：事件监听
来源：http://www.blog.epnwcf.com/Article/details/gefbwtxxg.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fktsv.cn/Article/details/gfjaxduqe.sHtML

[U100] JS：DOM 查询
来源：http://3g.tarul.cn/Article/details/ghznivrvj.sHtML

document.querySelector(".item")
来源：http://m.share.fktsv.cn/Article/details/gyydwllux.sHtML

[U101] JS：classList 操作
来源：http://m.share.vehdjk.com/Article/details/gdwmvyncs.sHtML

el.classList.toggle("active")
来源：http://www.m.share.epnwcf.com/Article/details/gencbmeep.sHtML

[U102] JS：本地存储
来源：http://read.share.epnwcf.com/Article/details/gcwqsusqr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.bbcook.cn/Article/details/gdxslopih.sHtML

[U103] JS：定时器
来源：http://www.blog.tarul.cn/Article/details/gvplzkzqz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.tarul.cn/Article/details/gwrnssumg.sHtML

[U104] JS：防抖
来源：http://www.blog.epnwcf.com/Article/details/gkcnkildl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gwwlxedet.sHtML

[U105] JS：节流
来源：http://3g.vehdjk.com/Article/details/gddzpabzu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.vehdjk.com/Article/details/ghhezpyzd.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gxprepypt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.sjlbkw.cn/Article/details/ggbosajzc.sHtML

[U107] JS：数字千分位
来源：http://blog.sjlbkw.cn/Article/details/gcmkcrelt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.epnwcf.com/Article/details/gptinohqa.sHtML

[U108] JS：随机整数
来源：http://blog.bbcook.cn/Article/details/gdpjvfmrh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.tarul.cn/Article/details/grkkawbay.sHtML

[U109] JS：数组分组
来源：http://read.share.sjlbkw.cn/Article/details/gtzgzbndq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.epnwcf.com/Article/details/gywdiuinq.sHtML

[U110] JS：数组分块
来源：http://www.blog.epnwcf.com/Article/details/gahbtaxts.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.sjlbkw.cn/Article/details/gqzmogria.sHtML

[U111] JS：对象转 Map
来源：http://read.share.sjlbkw.cn/Article/details/gctjhkqkh.sHtML

new Map(Object.entries(obj))
来源：http://baike.fktsv.cn/Article/details/gfrrgxelj.sHtML

[U112] JS：字符串补位
来源：http://read.share.bbcook.cn/Article/details/gkhngrbtv.sHtML

"7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gqkzatyia.sHtML

[U113] JS：正则替换全部
来源：http://mobile.tarul.cn/Article/details/gxsqagklz.sHtML

s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gvactrogu.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.epnwcf.com/Article/details/gcmttybuh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fktsv.cn/Article/details/gozkgsxbt.sHtML

[U115] JS：生成 UUID
来源：http://www.share.tarul.cn/Article/details/gfnybfasw.sHtML

crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/gzzinehap.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.yfazqb.com/Article/details/gywlvkhww.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.tarul.cn/Article/details/gfwpimkyw.sHtML

[U117] JS：单元测试
来源：http://wap.epnwcf.com/Article/details/ginmzrcsx.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.sjlbkw.cn/Article/details/gaibvxuez.sHtML

[U118] JS：开发服务器
来源：http://wap.yfazqb.com/Article/details/gtslrzrin.sHtML

npm i -D vite;  npx vite
来源：http://mobile.vehdjk.com/Article/details/gptnccgqk.sHtML

[U119] JS：生产构建
来源：http://read.share.tarul.cn/Article/details/gfumcnlgk.sHtML

npx vite build
来源：http://read.share.tarul.cn/Article/details/gjvdhbfyg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.bbcook.cn/Article/details/gtgqtdjeu.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.epnwcf.com/Article/details/gyfjbytya.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gtphxsjqg.sHtML

统计汇总
来源：http://www.m.share.fktsv.cn/Article/details/gjrjoaibm.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/goccdilcx.sHtML

按语言统计（条）：
来源：http://www.share.sjlbkw.cn/Article/details/gxazolgyg.sHtML

Python ......... 252
来源：http://www.m.share.tarul.cn/Article/details/gmxgcloiz.sHtML

PHP ............ 252
来源：http://read.share.epnwcf.com/Article/details/gljcqezsw.sHtML

JavaScript ..... 252
来源：http://mobile.sjlbkw.cn/Article/details/gnqbkyhtn.sHtML

TypeScript ..... 212
来源：http://blog.tarul.cn/Article/details/galhwauvl.sHtML

Java ........... 212
来源：http://3g.bbcook.cn/Article/details/ggwyesssj.sHtML

Go ............. 212
来源：http://read.share.epnwcf.com/Article/details/gpipnwdei.sHtML

Ruby ........... 212
来源：http://blog.yfazqb.com/Article/details/gditkybek.sHtML

C# ............. 212
来源：http://www.share.bbcook.cn/Article/details/gvutqjnri.sHtML

C .............. 30
来源：http://www.blog.bbcook.cn/Article/details/gbwovgeoz.sHtML

C++ ............ 30
来源：http://www.m.share.vehdjk.com/Article/details/ghkygrglm.sHtML

SQL ............ 90
来源：http://www.share.bbcook.cn/Article/details/glnzogbun.sHtML

Bash ........... 80
来源：http://3g.epnwcf.com/Article/details/gkesfdoer.sHtML

Kotlin ......... 15
来源：http://3g.vehdjk.com/Article/details/gpipytmuw.sHtML

Swift .......... 15
来源：http://m.share.tarul.cn/Article/details/gcqhmnwxj.sHtML

Lua ............ 10
来源：http://www.m.share.tarul.cn/Article/details/gyvvzqotp.sHtML

Perl ........... 10
来源：http://baike.epnwcf.com/Article/details/gdzrgljbq.sHtML

Scala .......... 10
来源：http://read.share.bbcook.cn/Article/details/golqrclsn.sHtML

------------------------------------
来源：http://www.share.epnwcf.com/Article/details/gtxukgbhs.sHtML

合计 ........... 2106 条
来源：http://www.m.share.yfazqb.com/Article/details/gpguuzocr.sHtML

按章节统计：
来源：http://blog.yfazqb.com/Article/details/gvpdvxqxg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.sjlbkw.cn/Article/details/gujlimjaq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.bbcook.cn/Article/details/ghhzqqnvp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/gzurtbood.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.yfazqb.com/Article/details/gzveksklc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.epnwcf.com/Article/details/ghjuljofn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.tarul.cn/Article/details/guyteqpwm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fktsv.cn/Article/details/gevrcxque.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.vehdjk.com/Article/details/gkwimkwqe.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gzblznrpe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.vehdjk.com/Article/details/guvbafkvc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/gdaxgwreq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gifftqgdr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gqeouuqxg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.epnwcf.com/Article/details/gltwzsqne.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fktsv.cn/Article/details/gmscetcps.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gsdaibnwk.sHtML

Q SQL 专题                              90
来源：http://mobile.vehdjk.com/Article/details/gtyxjstet.sHtML

R Bash 专题                             80
来源：http://blog.sjlbkw.cn/Article/details/gykzrratk.sHtML

S C / C++ 专题                          60
来源：http://m.share.bbcook.cn/Article/details/gmzdlmmej.sHtML

T 其他语言补充                          60
来源：http://baike.bbcook.cn/Article/details/gdkfuohot.sHtML

U 高频实用片段                         120
来源：http://www.blog.sjlbkw.cn/Article/details/gauriclji.sHtML

------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/gijixomyw.sHtML

合计                                  2106 条
来源：http://www.m.share.fktsv.cn/Article/details/ghxkfbnae.sHtML

--------------------------------------------------------------------------------
来源：http://3g.bbcook.cn/Article/details/gjmityrrb.sHtML

使用提醒
来源：http://www.share.bbcook.cn/Article/details/gdiwbdfqg.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gpppuxgea.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.vehdjk.com/Article/details/giqqyztgt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.vehdjk.com/Article/details/gsuhxytpr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.vehdjk.com/Article/details/govmopepm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.yfazqb.com/Article/details/gbmgyfmae.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.bbcook.cn/Article/details/gugsdyakw.sHtML

—— 文件结束 ——
来源：http://mobile.fktsv.cn/Article/details/gqfasabby.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gqoiawwhc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.yfazqb.com/Article/details/gcdwdbakp.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fktsv.cn/Article/details/gjaeavtge.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gpkcpjgzc.sHtML

【收录内容】
来源：http://read.share.vehdjk.com/Article/details/gulstmruh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.sjlbkw.cn/Article/details/gehvwnhjd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.vehdjk.com/Article/details/gigakpcxk.sHtML

SQL · Bash · C · C++
来源：http://baike.sjlbkw.cn/Article/details/gakakvmad.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.epnwcf.com/Article/details/gppffmdnp.sHtML

【使用说明】
来源：http://m.share.bbcook.cn/Article/details/gdiopfmaa.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fktsv.cn/Article/details/gwrdoyqqf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.epnwcf.com/Article/details/ghalctiuj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.vehdjk.com/Article/details/gyblyvktu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.yfazqb.com/Article/details/gclyizegq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fktsv.cn/Article/details/gmfbzvzvx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fktsv.cn/Article/details/gmowthvjw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.tarul.cn/Article/details/gcrllgbvn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.tarul.cn/Article/details/gxnzrshwc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fktsv.cn/Article/details/gkdytoafj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.sjlbkw.cn/Article/details/gpqwljgmz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.vehdjk.com/Article/details/gfvezflzc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.sjlbkw.cn/Article/details/gvxtchqhc.sHtML

【文件统计】
来源：http://3g.fktsv.cn/Article/details/geemvrpbo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.bbcook.cn/Article/details/gjpsngmfi.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/gqnlgssir.sHtML

目  录
来源：http://www.m.share.fktsv.cn/Article/details/gvylqryly.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.vehdjk.com/Article/details/gklwudpcb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.bbcook.cn/Article/details/gwmgnlzie.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.tarul.cn/Article/details/gvvzwmhfq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.epnwcf.com/Article/details/gxcrfxgxu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.vehdjk.com/Article/details/gucvvxetw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.vehdjk.com/Article/details/gqsirdyfs.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.epnwcf.com/Article/details/gaoifgqba.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fktsv.cn/Article/details/guxxtuktl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.tarul.cn/Article/details/gvnhsszyr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gkaisdewe.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.bbcook.cn/Article/details/gtwhjutyr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/gtkdaffhr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fktsv.cn/Article/details/gutkdizdf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.epnwcf.com/Article/details/gnckjqjzw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.vehdjk.com/Article/details/gdwqwobco.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.tarul.cn/Article/details/gkjnhsxkh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/gvkwbaduj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fktsv.cn/Article/details/gybhbaczz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.tarul.cn/Article/details/gfhweavlg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.bbcook.cn/Article/details/gtfiurhsq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.epnwcf.com/Article/details/gdlrdjtvs.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.sjlbkw.cn/Article/details/gxazckkby.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gyvalzmlu.sHtML

A. 基础语法与类型
来源：http://wap.tarul.cn/Article/details/gpwllkezo.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ghkvjllkn.sHtML

[A01] Hello World
来源：http://wap.yfazqb.com/Article/details/gdicuxizl.sHtML

Py:   print("Hello, World!")
来源：http://read.share.epnwcf.com/Article/details/gvfgcppgi.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.bbcook.cn/Article/details/gyhlsafjw.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.tarul.cn/Article/details/gxphnskjw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fktsv.cn/Article/details/gffswntka.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.vehdjk.com/Article/details/gvlpjronz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.epnwcf.com/Article/details/gvvmucbnx.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.tarul.cn/Article/details/gmbcfqajj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.vehdjk.com/Article/details/gbmnorwak.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fktsv.cn/Article/details/gkinoraen.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fktsv.cn/Article/details/gkiybxtvy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.epnwcf.com/Article/details/gkpxibifv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.epnwcf.com/Article/details/gxbwkjruj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.epnwcf.com/Article/details/gvlshbtmg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.epnwcf.com/Article/details/gvqtgtmhz.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.yfazqb.com/Article/details/gmtgdefzg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.yfazqb.com/Article/details/golseaxdm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.vehdjk.com/Article/details/gpitydynl.sHtML

[A03] 常量定义
来源：http://blog.sjlbkw.cn/Article/details/gwfikghxt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.yfazqb.com/Article/details/gigktsgra.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gpagzaoot.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gmuxtoszv.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/grvnsodtm.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gajfuqniw.sHtML

Go:   const PI = 3.14159
来源：http://read.share.tarul.cn/Article/details/gkdktvncy.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.bbcook.cn/Article/details/ghjncceos.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/ggzlvqwso.sHtML

[A04] 判断变量类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkcvzrxx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.yfazqb.com/Article/details/guxzbmyyn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.epnwcf.com/Article/details/ghizdftpe.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.sjlbkw.cn/Article/details/grkpzlqnz.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.bbcook.cn/Article/details/girfmyydz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.epnwcf.com/Article/details/gtkshsovs.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.tarul.cn/Article/details/gyujyibcj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.yfazqb.com/Article/details/gxmayeqrg.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.epnwcf.com/Article/details/geteqxmyd.sHtML

[A05] 整数除法与取模
来源：http://3g.fktsv.cn/Article/details/gdzgwgkhu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.sjlbkw.cn/Article/details/glrkksoed.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gkniqwgch.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.epnwcf.com/Article/details/gqbezqrlf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.epnwcf.com/Article/details/gxyxkrent.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gxmrneitv.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqebhbxq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gdecbjkpr.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fktsv.cn/Article/details/geffzdavt.sHtML

[A06] 字符串转数字
来源：http://blog.tarul.cn/Article/details/gumlyfsbu.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fktsv.cn/Article/details/gwbaopbxb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.tarul.cn/Article/details/grmcjviou.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.tarul.cn/Article/details/gjynyzrcx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.bbcook.cn/Article/details/ghmiciykl.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.sjlbkw.cn/Article/details/gytvzyzcm.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.epnwcf.com/Article/details/gjwvknxbw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.vehdjk.com/Article/details/gajuvrqbi.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fktsv.cn/Article/details/gjabrjybq.sHtML

[A07] 数字转字符串
来源：http://m.share.fktsv.cn/Article/details/gywiwayia.sHtML

Py:   str(42)
来源：http://blog.yfazqb.com/Article/details/gcvxmznyq.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.sjlbkw.cn/Article/details/gfnseagqm.sHtML

JS:   String(42); (42).toString()
来源：http://baike.tarul.cn/Article/details/glixerxus.sHtML

TS:   String(42)
来源：http://www.blog.bbcook.cn/Article/details/gckhirkpm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.vehdjk.com/Article/details/grszkedrc.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.sjlbkw.cn/Article/details/gpametwck.sHtML

Ruby: 42.to_s
来源：http://www.blog.fktsv.cn/Article/details/gunallbwm.sHtML

C#:   42.ToString()
来源：http://blog.sjlbkw.cn/Article/details/gruipvpjh.sHtML

[A08] 取整与四舍五入
来源：http://blog.bbcook.cn/Article/details/gtlbnrgno.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.vehdjk.com/Article/details/gcgryrgll.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fktsv.cn/Article/details/gzxgjtprz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.yfazqb.com/Article/details/gtlvlcydo.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.vehdjk.com/Article/details/gixgjnbck.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.yfazqb.com/Article/details/gaxzfgyow.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.yfazqb.com/Article/details/ghiplahff.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.yfazqb.com/Article/details/gwmdhynoe.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.vehdjk.com/Article/details/gwydlscgc.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.sjlbkw.cn/Article/details/gynmheiph.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.yfazqb.com/Article/details/gtwelabeo.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fktsv.cn/Article/details/gmvgyeqqr.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gmalamruo.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.yfazqb.com/Article/details/gsrdafcdy.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.yfazqb.com/Article/details/gtvghsqct.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fktsv.cn/Article/details/gnvbtbity.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.vehdjk.com/Article/details/grjirzmlr.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.epnwcf.com/Article/details/gshdavjdy.sHtML

[A10] 生成随机数
来源：http://3g.epnwcf.com/Article/details/ginrmblsh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fktsv.cn/Article/details/gojzudhmz.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.tarul.cn/Article/details/gdkignwvc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fktsv.cn/Article/details/gikrlidkt.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fktsv.cn/Article/details/gpsctjgrg.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.bbcook.cn/Article/details/gtetprxgp.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.vehdjk.com/Article/details/geakolvsa.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.epnwcf.com/Article/details/glugxlxge.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.vehdjk.com/Article/details/gbgvlgkau.sHtML

[A11] 条件表达式（三元）
来源：http://baike.tarul.cn/Article/details/gyrxliisb.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.yfazqb.com/Article/details/gmikkvqmn.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.epnwcf.com/Article/details/gswklmuwl.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.yfazqb.com/Article/details/gnjxglkpk.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.sjlbkw.cn/Article/details/grvkbikmj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.epnwcf.com/Article/details/gtlprpkio.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.tarul.cn/Article/details/gotzwkakw.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.bbcook.cn/Article/details/glskitxja.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.yfazqb.com/Article/details/gxbsizsmk.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.vehdjk.com/Article/details/gywwkknus.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.sjlbkw.cn/Article/details/gkijzwnrq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.bbcook.cn/Article/details/geisxonju.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.yfazqb.com/Article/details/ggriklviw.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.tarul.cn/Article/details/glmlyybqn.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.yfazqb.com/Article/details/gozkiahtl.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.tarul.cn/Article/details/gmdfciypf.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fktsv.cn/Article/details/gkdzziask.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.bbcook.cn/Article/details/gdfcxxist.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.sjlbkw.cn/Article/details/gexwhergx.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/gjpqxulcs.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/goajpxyuk.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/gavspocyv.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fktsv.cn/Article/details/gzvubawqz.sHtML

Java: "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/ghujtsjip.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.bbcook.cn/Article/details/gozaaaxkc.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/gjdhwptyw.sHtML

C#:   "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gnbewnhyz.sHtML

[A14] 注释写法
来源：http://www.m.share.epnwcf.com/Article/details/gqwraarqr.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.yfazqb.com/Article/details/giibircek.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/gqdxolrdo.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.sjlbkw.cn/Article/details/ghyqbcymv.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fktsv.cn/Article/details/gflfmlxes.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.yfazqb.com/Article/details/gdrdphexw.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.yfazqb.com/Article/details/gryczqbia.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fktsv.cn/Article/details/gurxttvdj.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.vehdjk.com/Article/details/gwzobjovc.sHtML

[A15] 空值判断与默认值
来源：http://baike.bbcook.cn/Article/details/gjaybvdso.sHtML

Py:   value = data or "默认值"
来源：http://wap.vehdjk.com/Article/details/gtrwhomig.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.tarul.cn/Article/details/glqijuzcs.sHtML


<!-- 参考信息 -->