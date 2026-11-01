代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.m.share.bbcook.cn/Article/details/gwjlfuvgm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.bbcook.cn/Article/details/gfdzhjkpn.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gwtiwnjdj.sHtML

structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gyrliundj.sHtML

[U93] JS：模板字符串
来源：http://m.share.vehdjk.com/Article/details/guvwgqezk.sHtML

`共 ${n} 条`
来源：http://read.share.yfazqb.com/Article/details/grzykwytj.sHtML

[U94] JS：箭头函数
来源：http://read.share.fktsv.cn/Article/details/gopierhgw.sHtML

const double = x => x * 2;
来源：http://www.share.bbcook.cn/Article/details/gasrsgxng.sHtML

[U95] JS：Promise 包装
来源：http://wap.bbcook.cn/Article/details/gxaefcypn.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.vehdjk.com/Article/details/gbrzcsbtj.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.epnwcf.com/Article/details/gylhydpjj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gngahnmxq.sHtML

[U97] JS：并发请求
来源：http://mobile.yfazqb.com/Article/details/gdmsolnwh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gekzbigwc.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fktsv.cn/Article/details/gsriirwij.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.yfazqb.com/Article/details/gnbbcecer.sHtML

[U99] JS：事件监听
来源：http://m.share.yfazqb.com/Article/details/garcazxcb.sHtML

el.addEventListener("click", e => {})
来源：http://blog.tarul.cn/Article/details/ggbxcpbfe.sHtML

[U100] JS：DOM 查询
来源：http://wap.fktsv.cn/Article/details/gjnquuyrk.sHtML

document.querySelector(".item")
来源：http://www.blog.epnwcf.com/Article/details/gbfsqhpre.sHtML

[U101] JS：classList 操作
来源：http://read.share.bbcook.cn/Article/details/goycwuswq.sHtML

el.classList.toggle("active")
来源：http://wap.bbcook.cn/Article/details/gxauzyfte.sHtML

[U102] JS：本地存储
来源：http://mobile.sjlbkw.cn/Article/details/glujruysl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.epnwcf.com/Article/details/gekwmkloi.sHtML

[U103] JS：定时器
来源：http://baike.fktsv.cn/Article/details/gxgkkecuj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.bbcook.cn/Article/details/gjvwjzfbj.sHtML

[U104] JS：防抖
来源：http://www.share.epnwcf.com/Article/details/gelqeegde.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/gngmjnccr.sHtML

[U105] JS：节流
来源：http://3g.bbcook.cn/Article/details/gianuxria.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.bbcook.cn/Article/details/gujuvayca.sHtML

[U106] JS：日期格式化
来源：http://m.share.yfazqb.com/Article/details/gltzguohb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.yfazqb.com/Article/details/grgqrnlck.sHtML

[U107] JS：数字千分位
来源：http://read.share.yfazqb.com/Article/details/gueengcaj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.sjlbkw.cn/Article/details/gfheunike.sHtML

[U108] JS：随机整数
来源：http://www.m.share.vehdjk.com/Article/details/grruwxmyo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.bbcook.cn/Article/details/gxnfztifb.sHtML

[U109] JS：数组分组
来源：http://3g.tarul.cn/Article/details/gezurebdq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.yfazqb.com/Article/details/ggrojyzlx.sHtML

[U110] JS：数组分块
来源：http://m.share.bbcook.cn/Article/details/gtpygvfyg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.tarul.cn/Article/details/gtpfacfqn.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.epnwcf.com/Article/details/gsklkwqtz.sHtML

new Map(Object.entries(obj))
来源：http://wap.tarul.cn/Article/details/gkfyvjnqm.sHtML

[U112] JS：字符串补位
来源：http://baike.yfazqb.com/Article/details/glogixvtk.sHtML

"7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/glbpmjkcn.sHtML

[U113] JS：正则替换全部
来源：http://mobile.bbcook.cn/Article/details/gqddoccwz.sHtML

s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/gpysdjchr.sHtML

[U114] JS：JSON 深比较
来源：http://3g.epnwcf.com/Article/details/gifyczyej.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.sjlbkw.cn/Article/details/gfyjbqvps.sHtML

[U115] JS：生成 UUID
来源：http://wap.sjlbkw.cn/Article/details/gayjelhwb.sHtML

crypto.randomUUID()
来源：http://www.blog.tarul.cn/Article/details/gotculzpc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fktsv.cn/Article/details/gmeqhhvld.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.epnwcf.com/Article/details/gpdlcbhaq.sHtML

[U117] JS：单元测试
来源：http://wap.bbcook.cn/Article/details/grpvslezm.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.tarul.cn/Article/details/grpkizjbi.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.yfazqb.com/Article/details/gefyqrkjm.sHtML

npm i -D vite;  npx vite
来源：http://wap.sjlbkw.cn/Article/details/gemqryuaf.sHtML

[U119] JS：生产构建
来源：http://www.share.yfazqb.com/Article/details/gwkvpdevi.sHtML

npx vite build
来源：http://mobile.sjlbkw.cn/Article/details/gpqjpkurh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.tarul.cn/Article/details/gxanrnbsu.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.bbcook.cn/Article/details/gdepjvrys.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gmgkejtdb.sHtML

统计汇总
来源：http://wap.bbcook.cn/Article/details/ggpiwuaab.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gsacynorj.sHtML

按语言统计（条）：
来源：http://m.share.epnwcf.com/Article/details/gvoxwsvzq.sHtML

Python ......... 252
来源：http://baike.yfazqb.com/Article/details/gwxovlblo.sHtML

PHP ............ 252
来源：http://read.share.sjlbkw.cn/Article/details/gyapulybk.sHtML

JavaScript ..... 252
来源：http://3g.bbcook.cn/Article/details/geidlntfh.sHtML

TypeScript ..... 212
来源：http://mobile.yfazqb.com/Article/details/gewbzpyup.sHtML

Java ........... 212
来源：http://mobile.vehdjk.com/Article/details/gezdmklrk.sHtML

Go ............. 212
来源：http://www.share.vehdjk.com/Article/details/giczsqcaq.sHtML

Ruby ........... 212
来源：http://read.share.epnwcf.com/Article/details/gdgkqqtmi.sHtML

C# ............. 212
来源：http://www.m.share.yfazqb.com/Article/details/gjfuksisx.sHtML

C .............. 30
来源：http://read.share.epnwcf.com/Article/details/gkstffcys.sHtML

C++ ............ 30
来源：http://3g.epnwcf.com/Article/details/gerzrlkvs.sHtML

SQL ............ 90
来源：http://www.blog.sjlbkw.cn/Article/details/gwttbwqkl.sHtML

Bash ........... 80
来源：http://wap.sjlbkw.cn/Article/details/guivqgbkr.sHtML

Kotlin ......... 15
来源：http://m.share.tarul.cn/Article/details/ghwcnnbnt.sHtML

Swift .......... 15
来源：http://m.share.sjlbkw.cn/Article/details/gavcjgzyb.sHtML

Lua ............ 10
来源：http://www.share.sjlbkw.cn/Article/details/glezbuimd.sHtML

Perl ........... 10
来源：http://read.share.fktsv.cn/Article/details/giyghyahl.sHtML

Scala .......... 10
来源：http://www.blog.vehdjk.com/Article/details/gmhfoijsh.sHtML

------------------------------------
来源：http://baike.vehdjk.com/Article/details/ggcfimseo.sHtML

合计 ........... 2106 条
来源：http://m.share.fktsv.cn/Article/details/glvdhigni.sHtML

按章节统计：
来源：http://baike.vehdjk.com/Article/details/giiupjgxn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.bbcook.cn/Article/details/gqlxpzrul.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.bbcook.cn/Article/details/gxjckfqab.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.vehdjk.com/Article/details/gttoqvrtz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.yfazqb.com/Article/details/gisgykjci.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.sjlbkw.cn/Article/details/gwamnvywm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.tarul.cn/Article/details/ggoxqyxic.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.vehdjk.com/Article/details/gjmatwasn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.yfazqb.com/Article/details/gnmwddgct.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/guedptrsl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.epnwcf.com/Article/details/gxbbaayhq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/gsmcmqbvx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/guiqtzxmr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gszanznjr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.bbcook.cn/Article/details/gxrdnwtgy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.vehdjk.com/Article/details/gdvzunoxc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gflqoeqko.sHtML

Q SQL 专题                              90
来源：http://3g.yfazqb.com/Article/details/grscijwrv.sHtML

R Bash 专题                             80
来源：http://baike.tarul.cn/Article/details/gmpaevepg.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.epnwcf.com/Article/details/glevmpiyc.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fktsv.cn/Article/details/gnpjdtemc.sHtML

U 高频实用片段                         120
来源：http://www.share.yfazqb.com/Article/details/gbxqvdsnp.sHtML

------------------------------------
来源：http://3g.epnwcf.com/Article/details/gggwhlrnh.sHtML

合计                                  2106 条
来源：http://www.m.share.bbcook.cn/Article/details/gbrtmxlzz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gufclioxh.sHtML

使用提醒
来源：http://www.share.sjlbkw.cn/Article/details/gmuafcxbj.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gnfjskxbl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.tarul.cn/Article/details/gtfknjinu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.bbcook.cn/Article/details/gtdtrwsrc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.bbcook.cn/Article/details/gzriwskyz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fktsv.cn/Article/details/gqjrsckua.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.vehdjk.com/Article/details/gnysmvttq.sHtML

—— 文件结束 ——
来源：http://m.share.yfazqb.com/Article/details/gvxdocqvn.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gveyzbwpa.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.vehdjk.com/Article/details/gwybiijau.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.sjlbkw.cn/Article/details/ghtoxkeox.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grkpapvlj.sHtML

【收录内容】
来源：http://baike.vehdjk.com/Article/details/giromjckm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fktsv.cn/Article/details/gaueankec.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.yfazqb.com/Article/details/gshzyuqrq.sHtML

SQL · Bash · C · C++
来源：http://read.share.fktsv.cn/Article/details/gwakgadyc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.epnwcf.com/Article/details/gbmthdhvo.sHtML

【使用说明】
来源：http://www.blog.yfazqb.com/Article/details/gzkzavnbu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.bbcook.cn/Article/details/gnmtyxqiw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fktsv.cn/Article/details/gnftzxsxu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.tarul.cn/Article/details/gbpcejdll.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.yfazqb.com/Article/details/guzyybptv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.epnwcf.com/Article/details/goretsvqr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.tarul.cn/Article/details/grhsyssyk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.epnwcf.com/Article/details/gprivzree.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.tarul.cn/Article/details/gurihlgef.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.sjlbkw.cn/Article/details/goihdotav.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.epnwcf.com/Article/details/gnsbslqjh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.sjlbkw.cn/Article/details/gscrcirkl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fktsv.cn/Article/details/gagkcwgra.sHtML

【文件统计】
来源：http://mobile.fktsv.cn/Article/details/gsfuiutba.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.sjlbkw.cn/Article/details/glnlciaqx.sHtML

--------------------------------------------------------------------------------
来源：http://baike.vehdjk.com/Article/details/gfuwzkowv.sHtML

目  录
来源：http://www.share.epnwcf.com/Article/details/gvgwplsbi.sHtML

--------------------------------------------------------------------------------
来源：http://wap.epnwcf.com/Article/details/gyfnezkgu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.bbcook.cn/Article/details/gtkpotlqy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.bbcook.cn/Article/details/gcdsarhpm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.tarul.cn/Article/details/gjybserhe.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.vehdjk.com/Article/details/gdnorpeyl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.tarul.cn/Article/details/gvlnvfsxg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.tarul.cn/Article/details/ghtntoznz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.yfazqb.com/Article/details/gihkimuas.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.tarul.cn/Article/details/gwpglussd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gisxdwgwa.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.epnwcf.com/Article/details/gljaqpsak.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gcndbkcjg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/ghexjqzyy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/gtxypnicg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.epnwcf.com/Article/details/gawycrliw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.bbcook.cn/Article/details/gcadwrich.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.yfazqb.com/Article/details/gnzswvxoe.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.vehdjk.com/Article/details/gmkjdapby.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gqncbhuck.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.sjlbkw.cn/Article/details/gewooubcj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/gtiplnijc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.tarul.cn/Article/details/gjfqvdgjd.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gdlxsztjo.sHtML

A. 基础语法与类型
来源：http://3g.yfazqb.com/Article/details/gkemyvdnt.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gzeehmnyb.sHtML

[A01] Hello World
来源：http://m.share.fktsv.cn/Article/details/gljubvfau.sHtML

Py:   print("Hello, World!")
来源：http://read.share.yfazqb.com/Article/details/gsznjqqwf.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.vehdjk.com/Article/details/gpuqstvye.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.vehdjk.com/Article/details/gqzhjsrqf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.tarul.cn/Article/details/gesjkmdzl.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.sjlbkw.cn/Article/details/gwuvtfsdt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.vehdjk.com/Article/details/gdghwggfq.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.bbcook.cn/Article/details/giqpakhjf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.tarul.cn/Article/details/gnkdxgcvk.sHtML

[A02] 变量声明与赋值
来源：http://wap.sjlbkw.cn/Article/details/gicssiijs.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.epnwcf.com/Article/details/goeuagofq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.vehdjk.com/Article/details/gmesdades.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fktsv.cn/Article/details/gxmymopea.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.bbcook.cn/Article/details/gevozgole.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.sjlbkw.cn/Article/details/ggmtfhqdk.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.sjlbkw.cn/Article/details/gvypnzlrr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.tarul.cn/Article/details/gvkybhvqr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.sjlbkw.cn/Article/details/gqsousyvt.sHtML

[A03] 常量定义
来源：http://baike.fktsv.cn/Article/details/guwxlsplb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.epnwcf.com/Article/details/gxrnkmvtf.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/ghywinflc.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gjfiehdfp.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gmodfxknb.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gibtstxvc.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fktsv.cn/Article/details/gywsaiqjc.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.vehdjk.com/Article/details/gjujkxkbz.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gukomklki.sHtML

[A04] 判断变量类型
来源：http://www.blog.fktsv.cn/Article/details/gwmxgzqco.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.tarul.cn/Article/details/ghjrhaqhp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.yfazqb.com/Article/details/ggjgsnbbt.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.yfazqb.com/Article/details/gdfbcsmib.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.yfazqb.com/Article/details/glpujlrbz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.bbcook.cn/Article/details/gyphkpvgl.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.epnwcf.com/Article/details/gjpxuhnje.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.sjlbkw.cn/Article/details/galcztqcn.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.bbcook.cn/Article/details/gpyypqgqb.sHtML

[A05] 整数除法与取模
来源：http://baike.epnwcf.com/Article/details/grhabdkfv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.yfazqb.com/Article/details/gewmaueif.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gcwmegwql.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/glsunaohw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gbaoyonma.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fktsv.cn/Article/details/gvoitimvh.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.vehdjk.com/Article/details/gukszzmnx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fktsv.cn/Article/details/gnkcprhdz.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.tarul.cn/Article/details/gvlkeeicy.sHtML

[A06] 字符串转数字
来源：http://www.m.share.tarul.cn/Article/details/gcxhopiem.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.bbcook.cn/Article/details/gvjcaehti.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.tarul.cn/Article/details/gluarkreg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.tarul.cn/Article/details/gjeammqbx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.sjlbkw.cn/Article/details/gmazzvzch.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.bbcook.cn/Article/details/gnzaujovi.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.vehdjk.com/Article/details/gmzgrlulx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.bbcook.cn/Article/details/gfjosbdkv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.sjlbkw.cn/Article/details/gbqoraxia.sHtML

[A07] 数字转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gyoghpbmp.sHtML

Py:   str(42)
来源：http://blog.tarul.cn/Article/details/gyptbccag.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.bbcook.cn/Article/details/gmemtcrhz.sHtML

JS:   String(42); (42).toString()
来源：http://3g.bbcook.cn/Article/details/gsdbrbvcz.sHtML

TS:   String(42)
来源：http://blog.sjlbkw.cn/Article/details/gizmdolhg.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.vehdjk.com/Article/details/geqtktoil.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.bbcook.cn/Article/details/gcpbpfzyg.sHtML

Ruby: 42.to_s
来源：http://baike.sjlbkw.cn/Article/details/gwqfiahos.sHtML

C#:   42.ToString()
来源：http://3g.bbcook.cn/Article/details/gtiruzzxs.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.tarul.cn/Article/details/grgpsjkjr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.vehdjk.com/Article/details/gmvwdyxyj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpchifox.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.tarul.cn/Article/details/gdgvzfsju.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.vehdjk.com/Article/details/gcuzcijbl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.tarul.cn/Article/details/giijluiic.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.epnwcf.com/Article/details/gsftzrjuf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.vehdjk.com/Article/details/gusfxshkp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.vehdjk.com/Article/details/gjenwtewm.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.vehdjk.com/Article/details/gtaehclmd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gngbhasni.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.yfazqb.com/Article/details/gakjxjdqm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.yfazqb.com/Article/details/gixkocwiz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gtjwtzrzx.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gimommhgn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.tarul.cn/Article/details/grkjpjxds.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.vehdjk.com/Article/details/gmcdolels.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.epnwcf.com/Article/details/gtmgfpbkj.sHtML

[A10] 生成随机数
来源：http://baike.yfazqb.com/Article/details/gsuparmfm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fktsv.cn/Article/details/gfoftujfu.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.epnwcf.com/Article/details/ggxxblgrx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.vehdjk.com/Article/details/gfmzbiudr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.tarul.cn/Article/details/gfzxatscp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.sjlbkw.cn/Article/details/gcsmrylhj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.vehdjk.com/Article/details/gsrvowkkp.sHtML

Ruby: rand(1..100)
来源：http://blog.sjlbkw.cn/Article/details/gcdljypjc.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.epnwcf.com/Article/details/gnqmocsgb.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.epnwcf.com/Article/details/gquyqtion.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.vehdjk.com/Article/details/gzydopfbg.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.vehdjk.com/Article/details/gdprtaaaw.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.yfazqb.com/Article/details/gsccbinqe.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.tarul.cn/Article/details/gedcfbkri.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fktsv.cn/Article/details/gjjmyupbk.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.bbcook.cn/Article/details/gymulsrng.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.vehdjk.com/Article/details/gjccknmxn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gdkunsseo.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.vehdjk.com/Article/details/gctuphseo.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.vehdjk.com/Article/details/gzeqkegcs.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.vehdjk.com/Article/details/gehfcrtss.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.vehdjk.com/Article/details/gncnaiiig.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fktsv.cn/Article/details/gtwgssmwy.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.yfazqb.com/Article/details/gadftyeeg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.tarul.cn/Article/details/giukvjklj.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.sjlbkw.cn/Article/details/gzmahtcxm.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.tarul.cn/Article/details/gyneqyomx.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.fktsv.cn/Article/details/govvwbszv.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/gfrnhsvea.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/gkpyjpfju.sHtML

JS:   "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gonqomjag.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/gikzxutwu.sHtML

Java: "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/geovewivn.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/ggsswvegl.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/gkossoitk.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/gaixecbpl.sHtML

[A14] 注释写法
来源：http://blog.tarul.cn/Article/details/grrftajsr.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.epnwcf.com/Article/details/gcexxjmqf.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.epnwcf.com/Article/details/guotqydry.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/glqbpcafy.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.sjlbkw.cn/Article/details/gphczgiwb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.bbcook.cn/Article/details/gzkbhkrqt.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.tarul.cn/Article/details/ganyuscxg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.vehdjk.com/Article/details/gxpaunsus.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.yfazqb.com/Article/details/gcisvdqkz.sHtML

[A15] 空值判断与默认值
来源：http://read.share.yfazqb.com/Article/details/gheoepovl.sHtML

Py:   value = data or "默认值"
来源：http://baike.tarul.cn/Article/details/gjhsrmheo.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.bbcook.cn/Article/details/gmlkdcizs.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.sjlbkw.cn/Article/details/gigvaaunj.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fktsv.cn/Article/details/gghjfpmll.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.sjlbkw.cn/Article/details/gguucmann.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.epnwcf.com/Article/details/gzqwlcfxl.sHtML


<!-- 参考信息 -->