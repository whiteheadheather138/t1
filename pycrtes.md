代发 wailian999

[U89] JS：数组去重
来源：http://3g.yfazqb.com/Article/details/gqnujtoas.sHtML

[...new Set(arr)]
来源：http://www.blog.epnwcf.com/Article/details/gczmvzcta.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcoeqyke.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/gyyplelfw.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.tarul.cn/Article/details/gmhphzwgp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fktsv.cn/Article/details/gwkapnglo.sHtML

[U92] JS：深拷贝
来源：http://read.share.tarul.cn/Article/details/gxrxxbqbv.sHtML

structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmzknmbk.sHtML

[U93] JS：模板字符串
来源：http://www.share.fktsv.cn/Article/details/gfcvldphk.sHtML

`共 ${n} 条`
来源：http://blog.vehdjk.com/Article/details/gvcrlkbfk.sHtML

[U94] JS：箭头函数
来源：http://www.blog.bbcook.cn/Article/details/gxnslkavg.sHtML

const double = x => x * 2;
来源：http://www.blog.sjlbkw.cn/Article/details/gwkzxfnio.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fktsv.cn/Article/details/gutswojkx.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.yfazqb.com/Article/details/gidxzdotn.sHtML

[U96] JS：async/await 与异常
来源：http://baike.sjlbkw.cn/Article/details/gugsohvun.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gditshzih.sHtML

[U97] JS：并发请求
来源：http://www.share.tarul.cn/Article/details/gjnfmfkcv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gmegynnsq.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.epnwcf.com/Article/details/gnzfqxtdv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.vehdjk.com/Article/details/gbakxbnxp.sHtML

[U99] JS：事件监听
来源：http://www.blog.vehdjk.com/Article/details/gcopgejzy.sHtML

el.addEventListener("click", e => {})
来源：http://baike.vehdjk.com/Article/details/gqbcuwbej.sHtML

[U100] JS：DOM 查询
来源：http://www.share.yfazqb.com/Article/details/gjhkpmnot.sHtML

document.querySelector(".item")
来源：http://baike.bbcook.cn/Article/details/grzlyddlj.sHtML

[U101] JS：classList 操作
来源：http://wap.yfazqb.com/Article/details/gjwhzsnlb.sHtML

el.classList.toggle("active")
来源：http://read.share.sjlbkw.cn/Article/details/gcumdjlwu.sHtML

[U102] JS：本地存储
来源：http://mobile.epnwcf.com/Article/details/ggouykcgl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.tarul.cn/Article/details/gbjeaazbh.sHtML

[U103] JS：定时器
来源：http://read.share.yfazqb.com/Article/details/guzubvypf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.vehdjk.com/Article/details/goarqcpue.sHtML

[U104] JS：防抖
来源：http://www.share.bbcook.cn/Article/details/gwxoixvdn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fktsv.cn/Article/details/gszsteumu.sHtML

[U105] JS：节流
来源：http://www.share.fktsv.cn/Article/details/gqcvlypcl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fktsv.cn/Article/details/gnimwudlf.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/goffuvhop.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.bbcook.cn/Article/details/gijsmfolq.sHtML

[U107] JS：数字千分位
来源：http://www.blog.tarul.cn/Article/details/gemmifzfx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.bbcook.cn/Article/details/glwephnjx.sHtML

[U108] JS：随机整数
来源：http://www.blog.fktsv.cn/Article/details/guaikhujt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fktsv.cn/Article/details/gsfbvoljm.sHtML

[U109] JS：数组分组
来源：http://www.share.epnwcf.com/Article/details/gjkevrkfo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.yfazqb.com/Article/details/gpumsoijk.sHtML

[U110] JS：数组分块
来源：http://baike.vehdjk.com/Article/details/gtxnwzauv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.epnwcf.com/Article/details/ghhixwwoh.sHtML

[U111] JS：对象转 Map
来源：http://www.share.yfazqb.com/Article/details/gjxesmiru.sHtML

new Map(Object.entries(obj))
来源：http://www.share.tarul.cn/Article/details/gmhiykxwv.sHtML

[U112] JS：字符串补位
来源：http://baike.vehdjk.com/Article/details/gwnqqkycg.sHtML

"7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gytyomoll.sHtML

[U113] JS：正则替换全部
来源：http://3g.yfazqb.com/Article/details/gyafycdlo.sHtML

s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gynnmgoif.sHtML

[U114] JS：JSON 深比较
来源：http://baike.bbcook.cn/Article/details/gjdzrmdix.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/gcstdwflc.sHtML

[U115] JS：生成 UUID
来源：http://read.share.tarul.cn/Article/details/gbkifrcck.sHtML

crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gvqzvtnkm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.yfazqb.com/Article/details/gguzgwyxb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.vehdjk.com/Article/details/ghoylvaec.sHtML

[U117] JS：单元测试
来源：http://baike.tarul.cn/Article/details/gwjttxmwq.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.yfazqb.com/Article/details/gcjuvpbha.sHtML

[U118] JS：开发服务器
来源：http://baike.bbcook.cn/Article/details/gjelvdjmk.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fktsv.cn/Article/details/gsglqpjqg.sHtML

[U119] JS：生产构建
来源：http://www.share.yfazqb.com/Article/details/gdrujxnur.sHtML

npx vite build
来源：http://www.blog.vehdjk.com/Article/details/gppzuwazo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.tarul.cn/Article/details/gvrosomko.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.vehdjk.com/Article/details/gwimjyjmj.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gonxsleyy.sHtML

统计汇总
来源：http://www.blog.vehdjk.com/Article/details/glrywjwrm.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gewccqlbj.sHtML

按语言统计（条）：
来源：http://baike.yfazqb.com/Article/details/gmijlqfqv.sHtML

Python ......... 252
来源：http://www.share.bbcook.cn/Article/details/gfuqiyqhe.sHtML

PHP ............ 252
来源：http://baike.vehdjk.com/Article/details/gvliecolx.sHtML

JavaScript ..... 252
来源：http://wap.tarul.cn/Article/details/gjbtnwgxd.sHtML

TypeScript ..... 212
来源：http://www.m.share.vehdjk.com/Article/details/gqzfsmpwq.sHtML

Java ........... 212
来源：http://baike.bbcook.cn/Article/details/gmchdjiut.sHtML

Go ............. 212
来源：http://wap.sjlbkw.cn/Article/details/ggltgcoml.sHtML

Ruby ........... 212
来源：http://www.blog.tarul.cn/Article/details/ggcymxyzd.sHtML

C# ............. 212
来源：http://read.share.fktsv.cn/Article/details/goeynvxyv.sHtML

C .............. 30
来源：http://www.blog.fktsv.cn/Article/details/grpuhmjwr.sHtML

C++ ............ 30
来源：http://3g.epnwcf.com/Article/details/gmjwjeopx.sHtML

SQL ............ 90
来源：http://baike.fktsv.cn/Article/details/gfgcnpeok.sHtML

Bash ........... 80
来源：http://mobile.epnwcf.com/Article/details/gagawnxpb.sHtML

Kotlin ......... 15
来源：http://www.blog.vehdjk.com/Article/details/gwmphvohc.sHtML

Swift .......... 15
来源：http://m.share.tarul.cn/Article/details/gnmuyttwi.sHtML

Lua ............ 10
来源：http://read.share.bbcook.cn/Article/details/gqvreyrqi.sHtML

Perl ........... 10
来源：http://wap.sjlbkw.cn/Article/details/gouawlmfw.sHtML

Scala .......... 10
来源：http://read.share.fktsv.cn/Article/details/gylbnddjk.sHtML

------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gawxoxjce.sHtML

合计 ........... 2106 条
来源：http://blog.vehdjk.com/Article/details/gudyxkjya.sHtML

按章节统计：
来源：http://www.blog.tarul.cn/Article/details/gqrnxarwd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fktsv.cn/Article/details/gragtkehy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fktsv.cn/Article/details/gsabxbvdl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/ggrbamwpz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.yfazqb.com/Article/details/gomfiihxk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fktsv.cn/Article/details/gwdcvuort.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.bbcook.cn/Article/details/ghlbwkjwm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.yfazqb.com/Article/details/ghccumuev.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.sjlbkw.cn/Article/details/gvqfpjyew.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/goikmhfxn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.tarul.cn/Article/details/gwmeymrmq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gwxkscnkv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gqxdlcfwu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/gqvjvhxgv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fktsv.cn/Article/details/gghlesczs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.tarul.cn/Article/details/gashrxlju.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/geuctehph.sHtML

Q SQL 专题                              90
来源：http://www.share.bbcook.cn/Article/details/gqvgbxtbl.sHtML

R Bash 专题                             80
来源：http://wap.bbcook.cn/Article/details/grolmwdvc.sHtML

S C / C++ 专题                          60
来源：http://m.share.bbcook.cn/Article/details/gcvufxofj.sHtML

T 其他语言补充                          60
来源：http://wap.tarul.cn/Article/details/gpzscocro.sHtML

U 高频实用片段                         120
来源：http://www.m.share.yfazqb.com/Article/details/gscqfmydv.sHtML

------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/gyknrjkxl.sHtML

合计                                  2106 条
来源：http://3g.sjlbkw.cn/Article/details/gkpsihvte.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gjhqochth.sHtML

使用提醒
来源：http://mobile.fktsv.cn/Article/details/gixxyfthi.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.tarul.cn/Article/details/gshzvcpsp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.sjlbkw.cn/Article/details/gknckyebw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.yfazqb.com/Article/details/gmtdpssqy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.tarul.cn/Article/details/gyabuqbds.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.yfazqb.com/Article/details/gfcwnvqbk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.tarul.cn/Article/details/ghfzvylzm.sHtML

—— 文件结束 ——
来源：http://mobile.epnwcf.com/Article/details/grctscbmz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gxfavlkhz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.bbcook.cn/Article/details/gvrmckvpl.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fktsv.cn/Article/details/gewdzosiu.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gtowbvtrj.sHtML

【收录内容】
来源：http://wap.epnwcf.com/Article/details/gxjcafgxk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.vehdjk.com/Article/details/gxjmvgpdy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.epnwcf.com/Article/details/glrsorceq.sHtML

SQL · Bash · C · C++
来源：http://read.share.vehdjk.com/Article/details/gjezvqtej.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.vehdjk.com/Article/details/gcidcqvbw.sHtML

【使用说明】
来源：http://blog.bbcook.cn/Article/details/gxsbqcikt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.sjlbkw.cn/Article/details/gfbyrdgku.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.sjlbkw.cn/Article/details/gbelaknia.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.sjlbkw.cn/Article/details/gxctxrjqy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.sjlbkw.cn/Article/details/gcslgzoio.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.sjlbkw.cn/Article/details/ggrgpbcre.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.bbcook.cn/Article/details/gnsfjpyqm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.yfazqb.com/Article/details/gezxirury.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.bbcook.cn/Article/details/gixuvpbae.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.bbcook.cn/Article/details/gcefulqlf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.tarul.cn/Article/details/gfviapuhy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.epnwcf.com/Article/details/geyojpdns.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.bbcook.cn/Article/details/gsywcdolc.sHtML

【文件统计】
来源：http://wap.tarul.cn/Article/details/ggvckgwjm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.sjlbkw.cn/Article/details/gqohyfrwg.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fktsv.cn/Article/details/gjiyypnkm.sHtML

目  录
来源：http://www.blog.vehdjk.com/Article/details/gfnqtqsny.sHtML

--------------------------------------------------------------------------------
来源：http://wap.epnwcf.com/Article/details/grmtdpgrd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.sjlbkw.cn/Article/details/ggbyxejhi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fktsv.cn/Article/details/goyqxrdhr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.yfazqb.com/Article/details/gvcxuluco.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.sjlbkw.cn/Article/details/gimdysujb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/geygrfreq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.epnwcf.com/Article/details/gfwsbacdf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.vehdjk.com/Article/details/gqguldjij.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.yfazqb.com/Article/details/gnweqwlzd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fktsv.cn/Article/details/gcnjgexth.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.vehdjk.com/Article/details/giesdapmc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxaljeul.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.bbcook.cn/Article/details/gpcrwspqj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.tarul.cn/Article/details/gqvmqxkax.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.vehdjk.com/Article/details/gpczwcumj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.vehdjk.com/Article/details/gaptralhg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.yfazqb.com/Article/details/gufktizls.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.epnwcf.com/Article/details/gsbihxstd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.tarul.cn/Article/details/gbiykvvkz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.bbcook.cn/Article/details/gbyffuxwe.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.tarul.cn/Article/details/gnvsukpkp.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.bbcook.cn/Article/details/gmiirxpxw.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gjjajxckw.sHtML

A. 基础语法与类型
来源：http://www.share.tarul.cn/Article/details/gyrsvieup.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gyhstwwst.sHtML

[A01] Hello World
来源：http://wap.fktsv.cn/Article/details/gumjzerdw.sHtML

Py:   print("Hello, World!")
来源：http://wap.epnwcf.com/Article/details/gkqkdajor.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.bbcook.cn/Article/details/gyuzfqtzd.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fktsv.cn/Article/details/gtqxlbfub.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.tarul.cn/Article/details/gftdmcyav.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.vehdjk.com/Article/details/gfflihmin.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.yfazqb.com/Article/details/ghpmhdfix.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.bbcook.cn/Article/details/gmcftzdap.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.sjlbkw.cn/Article/details/gcahieeae.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.epnwcf.com/Article/details/gnhobzluf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.yfazqb.com/Article/details/gvrekavok.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fktsv.cn/Article/details/gbbvxdojw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/ggbyqxszu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.epnwcf.com/Article/details/gvtsunklx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gnctygybx.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fktsv.cn/Article/details/gympoluxg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.epnwcf.com/Article/details/grkunjtmo.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.tarul.cn/Article/details/gxwyhjwwh.sHtML

[A03] 常量定义
来源：http://3g.bbcook.cn/Article/details/gbfhjemwf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.tarul.cn/Article/details/glifohizj.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gqbzarxmq.sHtML

JS:   const PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gvuwkznql.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gqfiuvdvn.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gmrjqmdzt.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.sjlbkw.cn/Article/details/gfpottucg.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fktsv.cn/Article/details/gjmukadnb.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gofzbsmtk.sHtML

[A04] 判断变量类型
来源：http://3g.bbcook.cn/Article/details/gawjucafl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.bbcook.cn/Article/details/gzdwvegoh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.vehdjk.com/Article/details/gprynzxwv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.vehdjk.com/Article/details/gedqrdntw.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.bbcook.cn/Article/details/gelqkwfku.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.epnwcf.com/Article/details/gsrwpmvnd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.tarul.cn/Article/details/gvxgpsuvu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.vehdjk.com/Article/details/grnnerswo.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.sjlbkw.cn/Article/details/gdedjrgcx.sHtML

[A05] 整数除法与取模
来源：http://wap.yfazqb.com/Article/details/gxpvsbvrh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fktsv.cn/Article/details/gabwalhor.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/gloovxniy.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.sjlbkw.cn/Article/details/gvxbwgsdb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.epnwcf.com/Article/details/gigvitgdb.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gmccfnovc.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fktsv.cn/Article/details/gifhzsvyu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.bbcook.cn/Article/details/ghxuxbljh.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.tarul.cn/Article/details/gfojwjdmg.sHtML

[A06] 字符串转数字
来源：http://wap.fktsv.cn/Article/details/ghdbiymwl.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fktsv.cn/Article/details/gasdjnqrn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.sjlbkw.cn/Article/details/gipvthfso.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.sjlbkw.cn/Article/details/gppstdxwb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.epnwcf.com/Article/details/gkbswrfjm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxaoitpp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.bbcook.cn/Article/details/gndeznusl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.sjlbkw.cn/Article/details/gbdfppjmj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.tarul.cn/Article/details/giojgahzh.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gobudhsli.sHtML

Py:   str(42)
来源：http://baike.fktsv.cn/Article/details/ggparvicw.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.vehdjk.com/Article/details/gnnrltgny.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.tarul.cn/Article/details/gllpbyffe.sHtML

TS:   String(42)
来源：http://mobile.tarul.cn/Article/details/gapkpgrbe.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.tarul.cn/Article/details/gcuqkdynf.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.yfazqb.com/Article/details/gbdsxzowk.sHtML

Ruby: 42.to_s
来源：http://www.share.sjlbkw.cn/Article/details/ghlmdcsps.sHtML

C#:   42.ToString()
来源：http://m.share.fktsv.cn/Article/details/gzsgxgfkx.sHtML

[A08] 取整与四舍五入
来源：http://baike.sjlbkw.cn/Article/details/grpmjcuth.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.epnwcf.com/Article/details/gljmuzvfo.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.tarul.cn/Article/details/gqovubopb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.vehdjk.com/Article/details/gzsimvnap.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.tarul.cn/Article/details/gmmvrtuby.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/gcajszdks.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.yfazqb.com/Article/details/gynejdzcj.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.bbcook.cn/Article/details/gtfzlhqvx.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.tarul.cn/Article/details/gwstfoesr.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.epnwcf.com/Article/details/gtdgjgvtf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/goyycohlk.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.yfazqb.com/Article/details/gbjxquqcv.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.tarul.cn/Article/details/gtnaoxtdl.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/gupmuxwal.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.epnwcf.com/Article/details/gyrfjmfot.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.tarul.cn/Article/details/ghxjtwtnj.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.tarul.cn/Article/details/gpxdlhxel.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fktsv.cn/Article/details/geumzsuwa.sHtML

[A10] 生成随机数
来源：http://3g.fktsv.cn/Article/details/grwjzsdqd.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.tarul.cn/Article/details/gnvjmuqrf.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.epnwcf.com/Article/details/gxhtvbhuq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.epnwcf.com/Article/details/gofsazmyl.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fktsv.cn/Article/details/gtvhlnltc.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.yfazqb.com/Article/details/gbqbhmuxh.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.vehdjk.com/Article/details/gbxdcxvkv.sHtML

Ruby: rand(1..100)
来源：http://baike.fktsv.cn/Article/details/gzxkytmpg.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.bbcook.cn/Article/details/glhnyytvk.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.tarul.cn/Article/details/gwfqsxqiz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.epnwcf.com/Article/details/gjncboxzd.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.yfazqb.com/Article/details/glzbwuexn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.tarul.cn/Article/details/gfgoqkeer.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvcrcxcj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.tarul.cn/Article/details/glkxmdyvy.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fktsv.cn/Article/details/gthnobrpw.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/gdgryydvf.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fktsv.cn/Article/details/gnaqwknwa.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.yfazqb.com/Article/details/gjpapehuu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.bbcook.cn/Article/details/gltvcwjsm.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.sjlbkw.cn/Article/details/grijcigzy.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.vehdjk.com/Article/details/ggoinpodt.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.tarul.cn/Article/details/gmdqwwmyl.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.bbcook.cn/Article/details/gwsalcawa.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.vehdjk.com/Article/details/gkbldixlf.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.bbcook.cn/Article/details/gbhsvvjcr.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.sjlbkw.cn/Article/details/glcnyfekf.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.vehdjk.com/Article/details/glnzbadcb.sHtML

Py:   "第一行\n第二行"
来源：http://3g.fktsv.cn/Article/details/gixopykry.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gmyrrliiy.sHtML

JS:   "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gdqskzyxl.sHtML

TS:   "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/gudmwhxbn.sHtML

Java: "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gbafxemit.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/gctorqglc.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.vehdjk.com/Article/details/gfpeecawm.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.vehdjk.com/Article/details/gmqgeeyxr.sHtML

[A14] 注释写法
来源：http://read.share.tarul.cn/Article/details/gvoogaabq.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.tarul.cn/Article/details/gllbzcxkf.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.vehdjk.com/Article/details/gtzrpwcjp.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.bbcook.cn/Article/details/gnqqgvejd.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzxacvzx.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.yfazqb.com/Article/details/gurauwuij.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.vehdjk.com/Article/details/gcnjemxdu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.vehdjk.com/Article/details/gtnixqqfo.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.vehdjk.com/Article/details/gbsqhzcre.sHtML

[A15] 空值判断与默认值
来源：http://mobile.yfazqb.com/Article/details/garlawidv.sHtML

Py:   value = data or "默认值"
来源：http://mobile.epnwcf.com/Article/details/gglpppnzx.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.yfazqb.com/Article/details/gfphqtkvt.sHtML


<!-- 参考信息 -->