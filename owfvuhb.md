代发 wailian999

[U89] JS：数组去重
来源：http://blog.bbcook.cn/Article/details/gbzcphzej.sHtML

[...new Set(arr)]
来源：http://www.m.share.yfazqb.com/Article/details/gsczzasqm.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.sjlbkw.cn/Article/details/ganweqqqv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/grpxqzkos.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fktsv.cn/Article/details/gbcetcybu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.vehdjk.com/Article/details/gulipvyrv.sHtML

[U92] JS：深拷贝
来源：http://baike.sjlbkw.cn/Article/details/ggwgroihn.sHtML

structuredClone(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gizhgkddr.sHtML

[U93] JS：模板字符串
来源：http://read.share.sjlbkw.cn/Article/details/gwiluutpx.sHtML

`共 ${n} 条`
来源：http://3g.fktsv.cn/Article/details/gjreksxfy.sHtML

[U94] JS：箭头函数
来源：http://3g.fktsv.cn/Article/details/gbpuqqasz.sHtML

const double = x => x * 2;
来源：http://www.share.yfazqb.com/Article/details/gebnurttw.sHtML

[U95] JS：Promise 包装
来源：http://www.share.vehdjk.com/Article/details/gprylbifq.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fktsv.cn/Article/details/gpefjqfbk.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.yfazqb.com/Article/details/gnwrxhvia.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/glozorviy.sHtML

[U97] JS：并发请求
来源：http://blog.epnwcf.com/Article/details/gdxhmqqst.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gvujfjxyo.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.epnwcf.com/Article/details/gvkwnliok.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.epnwcf.com/Article/details/gzivjskbb.sHtML

[U99] JS：事件监听
来源：http://www.share.yfazqb.com/Article/details/gbkufimzj.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.vehdjk.com/Article/details/gnahtfqlq.sHtML

[U100] JS：DOM 查询
来源：http://mobile.bbcook.cn/Article/details/gumuqgycs.sHtML

document.querySelector(".item")
来源：http://www.share.bbcook.cn/Article/details/gzfhzdscd.sHtML

[U101] JS：classList 操作
来源：http://3g.tarul.cn/Article/details/gjrxibjhb.sHtML

el.classList.toggle("active")
来源：http://www.share.sjlbkw.cn/Article/details/gszyzoayc.sHtML

[U102] JS：本地存储
来源：http://mobile.epnwcf.com/Article/details/gjlyqmhra.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fktsv.cn/Article/details/gcwkcvbbt.sHtML

[U103] JS：定时器
来源：http://blog.fktsv.cn/Article/details/gejrlyhiw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.sjlbkw.cn/Article/details/gwrlgfvjx.sHtML

[U104] JS：防抖
来源：http://www.share.fktsv.cn/Article/details/grbhrklfu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gjknuyior.sHtML

[U105] JS：节流
来源：http://read.share.tarul.cn/Article/details/gdjiufqhg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.tarul.cn/Article/details/gkspjoiue.sHtML

[U106] JS：日期格式化
来源：http://read.share.epnwcf.com/Article/details/ggkbdcumb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.tarul.cn/Article/details/gctaovxce.sHtML

[U107] JS：数字千分位
来源：http://www.share.bbcook.cn/Article/details/grzfsiylt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.vehdjk.com/Article/details/gamusqwsm.sHtML

[U108] JS：随机整数
来源：http://baike.fktsv.cn/Article/details/gnvftvavj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.bbcook.cn/Article/details/girvihxxa.sHtML

[U109] JS：数组分组
来源：http://m.share.yfazqb.com/Article/details/gqfszwpng.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fktsv.cn/Article/details/gzxycragu.sHtML

[U110] JS：数组分块
来源：http://www.blog.bbcook.cn/Article/details/gtwpeuuay.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.epnwcf.com/Article/details/glaewzrji.sHtML

[U111] JS：对象转 Map
来源：http://mobile.sjlbkw.cn/Article/details/gtzthyxyn.sHtML

new Map(Object.entries(obj))
来源：http://blog.bbcook.cn/Article/details/gqsoubtzz.sHtML

[U112] JS：字符串补位
来源：http://m.share.vehdjk.com/Article/details/gnkpycxsw.sHtML

"7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gfvqundqo.sHtML

[U113] JS：正则替换全部
来源：http://www.share.sjlbkw.cn/Article/details/gercddsum.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gzjgutbri.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fktsv.cn/Article/details/gvvbquldz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.bbcook.cn/Article/details/gyjsnetlv.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fktsv.cn/Article/details/gvjohhwne.sHtML

crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gcyifxznd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.tarul.cn/Article/details/godqzglvt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.sjlbkw.cn/Article/details/gupjvopxe.sHtML

[U117] JS：单元测试
来源：http://www.share.tarul.cn/Article/details/gmdhlrfeg.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.sjlbkw.cn/Article/details/gifbipzio.sHtML

[U118] JS：开发服务器
来源：http://3g.yfazqb.com/Article/details/gawnqkfxe.sHtML

npm i -D vite;  npx vite
来源：http://baike.sjlbkw.cn/Article/details/gwgluytjk.sHtML

[U119] JS：生产构建
来源：http://blog.bbcook.cn/Article/details/gusvfpbkf.sHtML

npx vite build
来源：http://blog.bbcook.cn/Article/details/gozhfmngf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fktsv.cn/Article/details/gkmmdvbzp.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.epnwcf.com/Article/details/gojgqxsrp.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ggzmopqrd.sHtML

统计汇总
来源：http://www.share.tarul.cn/Article/details/gqindanjj.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gcnlrvcwm.sHtML

按语言统计（条）：
来源：http://www.blog.fktsv.cn/Article/details/guruacswz.sHtML

Python ......... 252
来源：http://www.m.share.bbcook.cn/Article/details/gdueojyxr.sHtML

PHP ............ 252
来源：http://blog.epnwcf.com/Article/details/gjtydslca.sHtML

JavaScript ..... 252
来源：http://wap.fktsv.cn/Article/details/gwhjetgkw.sHtML

TypeScript ..... 212
来源：http://3g.tarul.cn/Article/details/ghfexuexj.sHtML

Java ........... 212
来源：http://www.m.share.bbcook.cn/Article/details/gzkdozizl.sHtML

Go ............. 212
来源：http://baike.fktsv.cn/Article/details/gujsctzoj.sHtML

Ruby ........... 212
来源：http://blog.bbcook.cn/Article/details/gxsxfkecg.sHtML

C# ............. 212
来源：http://mobile.tarul.cn/Article/details/gzlrjpjnj.sHtML

C .............. 30
来源：http://wap.tarul.cn/Article/details/glwvwchad.sHtML

C++ ............ 30
来源：http://wap.bbcook.cn/Article/details/gxjjjewhz.sHtML

SQL ............ 90
来源：http://www.blog.vehdjk.com/Article/details/grhurzqsv.sHtML

Bash ........... 80
来源：http://m.share.tarul.cn/Article/details/gaeqrbxwg.sHtML

Kotlin ......... 15
来源：http://3g.fktsv.cn/Article/details/gydiujwdc.sHtML

Swift .......... 15
来源：http://3g.vehdjk.com/Article/details/gddicjbfa.sHtML

Lua ............ 10
来源：http://baike.yfazqb.com/Article/details/gwkdbaiag.sHtML

Perl ........... 10
来源：http://www.blog.fktsv.cn/Article/details/gjhjvsxvl.sHtML

Scala .......... 10
来源：http://www.blog.tarul.cn/Article/details/gjgjvuhpx.sHtML

------------------------------------
来源：http://wap.bbcook.cn/Article/details/gbkcgsqju.sHtML

合计 ........... 2106 条
来源：http://read.share.yfazqb.com/Article/details/ghtujnrac.sHtML

按章节统计：
来源：http://mobile.vehdjk.com/Article/details/gjcbzaauu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.bbcook.cn/Article/details/gakizyczk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.tarul.cn/Article/details/gavduxgfw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.epnwcf.com/Article/details/gphqodytm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.tarul.cn/Article/details/gxwfldfal.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.sjlbkw.cn/Article/details/gxpajyams.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.yfazqb.com/Article/details/ggqauizuc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.vehdjk.com/Article/details/gahwxhvst.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.sjlbkw.cn/Article/details/gswhdtaeo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gbhpnyeog.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.sjlbkw.cn/Article/details/gujibonzr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gotceykmm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/gszrctfse.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/grxvcriie.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.sjlbkw.cn/Article/details/giwfgmibu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fktsv.cn/Article/details/gwhrndozk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/gtsgccduy.sHtML

Q SQL 专题                              90
来源：http://wap.yfazqb.com/Article/details/gxjcgpqio.sHtML

R Bash 专题                             80
来源：http://www.m.share.fktsv.cn/Article/details/ghewkkzcb.sHtML

S C / C++ 专题                          60
来源：http://www.share.vehdjk.com/Article/details/gpnpncdbe.sHtML

T 其他语言补充                          60
来源：http://www.share.bbcook.cn/Article/details/grescgghi.sHtML

U 高频实用片段                         120
来源：http://baike.yfazqb.com/Article/details/gmfqgjlhf.sHtML

------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gckfaxmfc.sHtML

合计                                  2106 条
来源：http://wap.yfazqb.com/Article/details/gqrhxssfh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gfowhicjc.sHtML

使用提醒
来源：http://read.share.bbcook.cn/Article/details/gtukfpswi.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gaftzhuar.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fktsv.cn/Article/details/gupxdhqna.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.bbcook.cn/Article/details/gvbpuuaau.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.yfazqb.com/Article/details/gmxusjkwb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fktsv.cn/Article/details/gnxfllohf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.vehdjk.com/Article/details/giizkqtxu.sHtML

—— 文件结束 ——
来源：http://m.share.yfazqb.com/Article/details/gaytppxkj.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gotuefmhk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fktsv.cn/Article/details/gworkoatc.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.epnwcf.com/Article/details/grbmlzerj.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gxukrjpwc.sHtML

【收录内容】
来源：http://read.share.yfazqb.com/Article/details/gmjqidyhf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.yfazqb.com/Article/details/gzoxtrbak.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.tarul.cn/Article/details/gwjrqcnmi.sHtML

SQL · Bash · C · C++
来源：http://3g.yfazqb.com/Article/details/gbtjdaeje.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.vehdjk.com/Article/details/gfzegwvuo.sHtML

【使用说明】
来源：http://www.blog.sjlbkw.cn/Article/details/gxgyzcjdp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.vehdjk.com/Article/details/gnaduavst.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.vehdjk.com/Article/details/gbqzmfbaz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.tarul.cn/Article/details/gletwmmuv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.sjlbkw.cn/Article/details/gfrnimegn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.bbcook.cn/Article/details/gmxisrmub.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.tarul.cn/Article/details/gtfpixvcn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.yfazqb.com/Article/details/ggnsprfjr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.epnwcf.com/Article/details/gnmvidusn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.tarul.cn/Article/details/gbhoernlo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.sjlbkw.cn/Article/details/gdrrwtuxp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.bbcook.cn/Article/details/gupswmdor.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.tarul.cn/Article/details/gjnwcfqfp.sHtML

【文件统计】
来源：http://www.share.vehdjk.com/Article/details/gjwisqzgy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fktsv.cn/Article/details/gkdwdvnvl.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gtauxqvqa.sHtML

目  录
来源：http://3g.vehdjk.com/Article/details/gahlpuiap.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/grgmljofg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.vehdjk.com/Article/details/gdzythatt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.yfazqb.com/Article/details/gmtnudkrs.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.yfazqb.com/Article/details/guzzoyleg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.vehdjk.com/Article/details/gbtyfqrqk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.yfazqb.com/Article/details/gczgkcfpd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.epnwcf.com/Article/details/gslnnndsu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/gziibketa.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.bbcook.cn/Article/details/gqcnwcjmg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fktsv.cn/Article/details/gjalkffgo.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fktsv.cn/Article/details/gzvxrfldy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gizexugxy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/gibhwbkhl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/ghcnzxmru.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.tarul.cn/Article/details/gpyrimsge.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.yfazqb.com/Article/details/gzdblkwaw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/glapfaqmx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.vehdjk.com/Article/details/gghkvpsso.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.bbcook.cn/Article/details/gqxlajbro.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.bbcook.cn/Article/details/golwvywlo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fktsv.cn/Article/details/gewppalvv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.yfazqb.com/Article/details/giwegswfm.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gewbpnblf.sHtML

A. 基础语法与类型
来源：http://wap.vehdjk.com/Article/details/gzcimvtje.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gtxlreklw.sHtML

[A01] Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gyrqpphdj.sHtML

Py:   print("Hello, World!")
来源：http://wap.yfazqb.com/Article/details/gzqucxsck.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.bbcook.cn/Article/details/gfsekoove.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.bbcook.cn/Article/details/gaqtewsqs.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.yfazqb.com/Article/details/goyqvprfj.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fktsv.cn/Article/details/gandvtnrn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.yfazqb.com/Article/details/grseahjqx.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.tarul.cn/Article/details/gtmszppkj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fktsv.cn/Article/details/gnfsmhdwu.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.tarul.cn/Article/details/gzfvzilww.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.yfazqb.com/Article/details/gweqflqli.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.epnwcf.com/Article/details/gwquhdnyl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.bbcook.cn/Article/details/gfcrutvoh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gnqwnifpc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fktsv.cn/Article/details/guybfrjga.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fktsv.cn/Article/details/gocewaynj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.epnwcf.com/Article/details/gbmcgfbly.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.bbcook.cn/Article/details/gltrlumgb.sHtML

[A03] 常量定义
来源：http://www.share.fktsv.cn/Article/details/gwffahfwo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.bbcook.cn/Article/details/goplaeeob.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gkghjhqrs.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/glrmympzl.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gkjxwvuni.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gunpbqnon.sHtML

Go:   const PI = 3.14159
来源：http://www.share.yfazqb.com/Article/details/gutvhyhfi.sHtML

Ruby: PI = 3.14159
来源：http://3g.bbcook.cn/Article/details/gzrtpubgw.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gkathxtlv.sHtML

[A04] 判断变量类型
来源：http://mobile.tarul.cn/Article/details/gcwcrkpuk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.tarul.cn/Article/details/gbjtdcxid.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.bbcook.cn/Article/details/geethtroh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fktsv.cn/Article/details/gctelneao.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.tarul.cn/Article/details/gzhlcurzn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.tarul.cn/Article/details/gkdqnuvcs.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.tarul.cn/Article/details/gldinnitg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fktsv.cn/Article/details/gtvadjsgi.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.tarul.cn/Article/details/gxewmykxj.sHtML

[A05] 整数除法与取模
来源：http://www.share.yfazqb.com/Article/details/gdojqqhgv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.bbcook.cn/Article/details/gyulisrui.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/guknhtkkl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/gkqyspbib.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gpzsdpool.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/githrmzob.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/glrnhkiin.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.bbcook.cn/Article/details/gwexnafoa.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gvukoaxey.sHtML

[A06] 字符串转数字
来源：http://read.share.epnwcf.com/Article/details/goemckjce.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.bbcook.cn/Article/details/gsjiknixr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.epnwcf.com/Article/details/gdwrrtqdf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.sjlbkw.cn/Article/details/gksvnihok.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.sjlbkw.cn/Article/details/gpazbxnmx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fktsv.cn/Article/details/glrzjpkhx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.fktsv.cn/Article/details/gxyjwcbna.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.sjlbkw.cn/Article/details/grexugyha.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.yfazqb.com/Article/details/glywjgrzd.sHtML

[A07] 数字转字符串
来源：http://3g.vehdjk.com/Article/details/gqpawgbpp.sHtML

Py:   str(42)
来源：http://wap.tarul.cn/Article/details/ggfxrgrbq.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.vehdjk.com/Article/details/gsypqyove.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fktsv.cn/Article/details/gbzplolsp.sHtML

TS:   String(42)
来源：http://www.m.share.bbcook.cn/Article/details/gwstzafnp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.bbcook.cn/Article/details/gxvmcdsya.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.yfazqb.com/Article/details/griwqchvo.sHtML

Ruby: 42.to_s
来源：http://wap.yfazqb.com/Article/details/gufgzcrkq.sHtML

C#:   42.ToString()
来源：http://www.share.fktsv.cn/Article/details/gahmwemzi.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.yfazqb.com/Article/details/getquptba.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.tarul.cn/Article/details/gxotkxcjn.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.vehdjk.com/Article/details/gswslraxn.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.epnwcf.com/Article/details/guylarwhr.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.sjlbkw.cn/Article/details/glcypzhud.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.sjlbkw.cn/Article/details/gpraswkem.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.fktsv.cn/Article/details/glfpxjzms.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.yfazqb.com/Article/details/ghgvgcjsn.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.bbcook.cn/Article/details/gvdxxxupt.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.vehdjk.com/Article/details/gunithosm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.yfazqb.com/Article/details/gboibonfr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gnnmcbeyz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gogkpzgkb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.tarul.cn/Article/details/gqdkhcegd.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.tarul.cn/Article/details/gtundeqac.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.bbcook.cn/Article/details/gjctzsqah.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.tarul.cn/Article/details/garhribgz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.vehdjk.com/Article/details/ghdqxadkl.sHtML

[A10] 生成随机数
来源：http://blog.bbcook.cn/Article/details/gmtyiwzzl.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fktsv.cn/Article/details/gkokngwzd.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.epnwcf.com/Article/details/gduskqcnc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.tarul.cn/Article/details/gggrwulgn.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fktsv.cn/Article/details/ggakhckqu.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.tarul.cn/Article/details/gokpqefty.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.vehdjk.com/Article/details/gddwlnfld.sHtML

Ruby: rand(1..100)
来源：http://blog.bbcook.cn/Article/details/gicsfswup.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fktsv.cn/Article/details/guycdmhct.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.sjlbkw.cn/Article/details/grkctfksr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.epnwcf.com/Article/details/gundobhdw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.yfazqb.com/Article/details/glghdozvp.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.yfazqb.com/Article/details/ghyqhjlxb.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.bbcook.cn/Article/details/gadlimhqa.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fktsv.cn/Article/details/gzvnjvqhm.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.fktsv.cn/Article/details/gdobjigut.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fktsv.cn/Article/details/gayenjleb.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.sjlbkw.cn/Article/details/gevvavufz.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.yfazqb.com/Article/details/gkxmvbhsg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.tarul.cn/Article/details/girgqurya.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.epnwcf.com/Article/details/gzoutkpok.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.bbcook.cn/Article/details/gjjkqkrza.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.tarul.cn/Article/details/gpplgqsqa.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.epnwcf.com/Article/details/gckkdyzbx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.sjlbkw.cn/Article/details/gqomrgoht.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.epnwcf.com/Article/details/gzlqgiolr.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.bbcook.cn/Article/details/gyfqnsjvt.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.yfazqb.com/Article/details/gfvhrlzlc.sHtML

Py:   "第一行\n第二行"
来源：http://wap.vehdjk.com/Article/details/gygsaexux.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.vehdjk.com/Article/details/gppfnlpvr.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/gbunyyzdt.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gqdjuvsdr.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/gzpxwazgb.sHtML

Go:   "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/ghscctmuw.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/ghsmacdfl.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/gpyuuxdnb.sHtML

[A14] 注释写法
来源：http://blog.tarul.cn/Article/details/gtabmjkvg.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.yfazqb.com/Article/details/gjgeaxthq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.vehdjk.com/Article/details/gueaexkcc.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.bbcook.cn/Article/details/gwzfpetqq.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/gdgqcfgtn.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.epnwcf.com/Article/details/gzdezdvur.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.vehdjk.com/Article/details/gatygbyda.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.vehdjk.com/Article/details/ghmbuonol.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.epnwcf.com/Article/details/gvdwveevr.sHtML

[A15] 空值判断与默认值
来源：http://read.share.sjlbkw.cn/Article/details/gqlqdpquq.sHtML

Py:   value = data or "默认值"
来源：http://m.share.epnwcf.com/Article/details/gnbmhuzjs.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.yfazqb.com/Article/details/gmyurarkd.sHtML


<!-- 参考信息 -->