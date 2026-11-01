代发 wailian999

[U87] JS：解构默认值
来源：http://wap.sjlbkw.cn/Article/details/gupfxjinu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fktsv.cn/Article/details/gwikejldd.sHtML

[U88] JS：对象展开合并
来源：http://wap.epnwcf.com/Article/details/gfkrbzihk.sHtML

{ ...a, ...b }
来源：http://read.share.fktsv.cn/Article/details/gfwthgjsq.sHtML

[U89] JS：数组去重
来源：http://baike.tarul.cn/Article/details/gmoersydo.sHtML

[...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/gmileyhoq.sHtML

[U90] JS：数字数组排序
来源：http://m.share.yfazqb.com/Article/details/gcszdtzcm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/gvbmjgsdf.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.tarul.cn/Article/details/gcthufdzg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.sjlbkw.cn/Article/details/gvssgihjm.sHtML

[U92] JS：深拷贝
来源：http://3g.yfazqb.com/Article/details/glehlzrnv.sHtML

structuredClone(obj)
来源：http://mobile.epnwcf.com/Article/details/ghesovxuw.sHtML

[U93] JS：模板字符串
来源：http://www.share.sjlbkw.cn/Article/details/gzyfcpets.sHtML

`共 ${n} 条`
来源：http://www.m.share.vehdjk.com/Article/details/gjpdhmxog.sHtML

[U94] JS：箭头函数
来源：http://mobile.fktsv.cn/Article/details/gxsilvelx.sHtML

const double = x => x * 2;
来源：http://read.share.vehdjk.com/Article/details/gkfcnkdrg.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fktsv.cn/Article/details/gkxozcmem.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.yfazqb.com/Article/details/ghuurikqk.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.tarul.cn/Article/details/gjpvwzihf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.tarul.cn/Article/details/gqnwbwwtf.sHtML

[U97] JS：并发请求
来源：http://www.share.bbcook.cn/Article/details/gfufueago.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/ghivzdwtp.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.epnwcf.com/Article/details/gtmodyghu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.tarul.cn/Article/details/gdwfmqvev.sHtML

[U99] JS：事件监听
来源：http://baike.yfazqb.com/Article/details/gewphiksu.sHtML

el.addEventListener("click", e => {})
来源：http://wap.bbcook.cn/Article/details/gdxainnud.sHtML

[U100] JS：DOM 查询
来源：http://3g.yfazqb.com/Article/details/gfjhrabiw.sHtML

document.querySelector(".item")
来源：http://3g.sjlbkw.cn/Article/details/ggfkbiwnt.sHtML

[U101] JS：classList 操作
来源：http://m.share.bbcook.cn/Article/details/gowrtevre.sHtML

el.classList.toggle("active")
来源：http://www.m.share.epnwcf.com/Article/details/gedutzifn.sHtML

[U102] JS：本地存储
来源：http://baike.bbcook.cn/Article/details/gviccxmds.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.tarul.cn/Article/details/gkpanvfvh.sHtML

[U103] JS：定时器
来源：http://3g.bbcook.cn/Article/details/gtjmrqevk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.sjlbkw.cn/Article/details/gvylvtgnc.sHtML

[U104] JS：防抖
来源：http://read.share.vehdjk.com/Article/details/gnnojtykp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.epnwcf.com/Article/details/gqfogclks.sHtML

[U105] JS：节流
来源：http://3g.bbcook.cn/Article/details/gajkhxagi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fktsv.cn/Article/details/gmrffpftl.sHtML

[U106] JS：日期格式化
来源：http://www.share.bbcook.cn/Article/details/gxqjbphpd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fktsv.cn/Article/details/gdmwwnuyn.sHtML

[U107] JS：数字千分位
来源：http://mobile.fktsv.cn/Article/details/ggtfoshvc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.epnwcf.com/Article/details/grfsnhewo.sHtML

[U108] JS：随机整数
来源：http://m.share.vehdjk.com/Article/details/gpelhxezw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fktsv.cn/Article/details/gbyjsiook.sHtML

[U109] JS：数组分组
来源：http://www.m.share.vehdjk.com/Article/details/gfwaskiqi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fktsv.cn/Article/details/gtifocboz.sHtML

[U110] JS：数组分块
来源：http://blog.epnwcf.com/Article/details/gemyfomlp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fktsv.cn/Article/details/gkfdukeko.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fktsv.cn/Article/details/gzyllpdlh.sHtML

new Map(Object.entries(obj))
来源：http://read.share.sjlbkw.cn/Article/details/golxaduef.sHtML

[U112] JS：字符串补位
来源：http://wap.epnwcf.com/Article/details/gbsaidqia.sHtML

"7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gqlfxcuwu.sHtML

[U113] JS：正则替换全部
来源：http://m.share.vehdjk.com/Article/details/gzdtfulua.sHtML

s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gwwmehcdx.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.epnwcf.com/Article/details/gfioxsozr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.epnwcf.com/Article/details/gdicnkeda.sHtML

[U115] JS：生成 UUID
来源：http://www.share.tarul.cn/Article/details/goscwxtct.sHtML

crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gjveivnub.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.bbcook.cn/Article/details/gljncyqgq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.yfazqb.com/Article/details/gzmdbfpbk.sHtML

[U117] JS：单元测试
来源：http://baike.sjlbkw.cn/Article/details/gfawzfxkt.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fktsv.cn/Article/details/gdtfikvzm.sHtML

[U118] JS：开发服务器
来源：http://mobile.epnwcf.com/Article/details/gpsmxlcbv.sHtML

npm i -D vite;  npx vite
来源：http://www.share.bbcook.cn/Article/details/gztsqnket.sHtML

[U119] JS：生产构建
来源：http://www.share.yfazqb.com/Article/details/gyxwflamp.sHtML

npx vite build
来源：http://m.share.sjlbkw.cn/Article/details/guvdlbvzl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.vehdjk.com/Article/details/gqjnutjzo.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.vehdjk.com/Article/details/gcirfryhq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gtopxcyav.sHtML

统计汇总
来源：http://m.share.fktsv.cn/Article/details/gfrefcapc.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/goprdfvpu.sHtML

按语言统计（条）：
来源：http://wap.fktsv.cn/Article/details/gjgjfkikx.sHtML

Python ......... 252
来源：http://read.share.tarul.cn/Article/details/gzlzgtkrh.sHtML

PHP ............ 252
来源：http://blog.tarul.cn/Article/details/gqohjjwyj.sHtML

JavaScript ..... 252
来源：http://read.share.yfazqb.com/Article/details/gknezaxpk.sHtML

TypeScript ..... 212
来源：http://blog.bbcook.cn/Article/details/ghkyolcmg.sHtML

Java ........... 212
来源：http://www.share.fktsv.cn/Article/details/gmihvgidl.sHtML

Go ............. 212
来源：http://m.share.fktsv.cn/Article/details/gmiovxkgn.sHtML

Ruby ........... 212
来源：http://www.m.share.vehdjk.com/Article/details/gkfwrjjve.sHtML

C# ............. 212
来源：http://www.share.yfazqb.com/Article/details/gkpsxpabo.sHtML

C .............. 30
来源：http://read.share.vehdjk.com/Article/details/gurzvpvdz.sHtML

C++ ............ 30
来源：http://m.share.tarul.cn/Article/details/gsvgishkr.sHtML

SQL ............ 90
来源：http://read.share.fktsv.cn/Article/details/goywbevrn.sHtML

Bash ........... 80
来源：http://read.share.yfazqb.com/Article/details/gnjctwhvl.sHtML

Kotlin ......... 15
来源：http://blog.sjlbkw.cn/Article/details/gewsrvfyx.sHtML

Swift .......... 15
来源：http://www.blog.epnwcf.com/Article/details/gcndoqnhe.sHtML

Lua ............ 10
来源：http://www.share.sjlbkw.cn/Article/details/gstwpqxqm.sHtML

Perl ........... 10
来源：http://blog.vehdjk.com/Article/details/gnqweoxbf.sHtML

Scala .......... 10
来源：http://www.m.share.yfazqb.com/Article/details/gkuciabex.sHtML

------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/gejzqisxe.sHtML

合计 ........... 2106 条
来源：http://m.share.sjlbkw.cn/Article/details/gjdoaewmr.sHtML

按章节统计：
来源：http://blog.vehdjk.com/Article/details/gicdgisdo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.sjlbkw.cn/Article/details/grbfplwog.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.epnwcf.com/Article/details/gvcblmtbu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.tarul.cn/Article/details/gqrgxpbnl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.tarul.cn/Article/details/gizawnndc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.epnwcf.com/Article/details/gwtmsmnqi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fktsv.cn/Article/details/gpvdnwfom.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxjkcqiv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.tarul.cn/Article/details/gbszbenjh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/ghgibnwce.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.sjlbkw.cn/Article/details/gvgmrvtne.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/gxjftimxu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/goyjjccfk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gyxhpraql.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.bbcook.cn/Article/details/guntoradp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.tarul.cn/Article/details/goitpxjok.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/ghdtnqlen.sHtML

Q SQL 专题                              90
来源：http://wap.fktsv.cn/Article/details/gwlrbquen.sHtML

R Bash 专题                             80
来源：http://m.share.yfazqb.com/Article/details/gwtujqjop.sHtML

S C / C++ 专题                          60
来源：http://read.share.epnwcf.com/Article/details/ghbkiompk.sHtML

T 其他语言补充                          60
来源：http://mobile.tarul.cn/Article/details/gtpymcjpb.sHtML

U 高频实用片段                         120
来源：http://read.share.vehdjk.com/Article/details/gmvhnotho.sHtML

------------------------------------
来源：http://blog.fktsv.cn/Article/details/gzgsmrgug.sHtML

合计                                  2106 条
来源：http://read.share.epnwcf.com/Article/details/gqevlrzpx.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gxfebgtro.sHtML

使用提醒
来源：http://read.share.fktsv.cn/Article/details/gtorjybvt.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gtwcfnnjw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.tarul.cn/Article/details/gsnfrtely.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.yfazqb.com/Article/details/govyxokrb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.bbcook.cn/Article/details/gwslmwsuc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpbbaunl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.tarul.cn/Article/details/gdaqqmtqx.sHtML

—— 文件结束 ——
来源：http://www.share.yfazqb.com/Article/details/gddjlzbvy.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/guasdpefy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.sjlbkw.cn/Article/details/guojretwi.sHtML

Common Programming Examples Cheat Book
来源：http://blog.vehdjk.com/Article/details/gfhloaooh.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gojqhywvt.sHtML

【收录内容】
来源：http://m.share.yfazqb.com/Article/details/gsxemsoqk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.sjlbkw.cn/Article/details/gfexybske.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.vehdjk.com/Article/details/gvozswdhg.sHtML

SQL · Bash · C · C++
来源：http://baike.sjlbkw.cn/Article/details/gjpgixwtv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.tarul.cn/Article/details/gudnydddw.sHtML

【使用说明】
来源：http://www.blog.yfazqb.com/Article/details/gknwhiprx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.bbcook.cn/Article/details/gvgcmhosv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fktsv.cn/Article/details/gprsdmfvy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.sjlbkw.cn/Article/details/gaiunipcd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fktsv.cn/Article/details/gdpfbeqzf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.yfazqb.com/Article/details/gcujxpeul.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.vehdjk.com/Article/details/gsyfwjkzx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.bbcook.cn/Article/details/gmqrntfui.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.tarul.cn/Article/details/gjelhfokj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.bbcook.cn/Article/details/ggaborlde.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.tarul.cn/Article/details/ghwradvpm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.sjlbkw.cn/Article/details/gpzekcbom.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.sjlbkw.cn/Article/details/gzxixbimn.sHtML

【文件统计】
来源：http://www.blog.yfazqb.com/Article/details/giejnlofi.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.yfazqb.com/Article/details/gjagynivr.sHtML

--------------------------------------------------------------------------------
来源：http://blog.yfazqb.com/Article/details/gyptrdbla.sHtML

目  录
来源：http://m.share.epnwcf.com/Article/details/gzttjvkfk.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.vehdjk.com/Article/details/giyesqrcj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fktsv.cn/Article/details/gdmmaujdy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.epnwcf.com/Article/details/gopasifym.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.vehdjk.com/Article/details/gvbjwzudb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.bbcook.cn/Article/details/gjxnescbg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.bbcook.cn/Article/details/gjkxebvzw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.tarul.cn/Article/details/gfylvchxv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.epnwcf.com/Article/details/ggkdlchnv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.sjlbkw.cn/Article/details/gwddfflyb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/gdqhghjav.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.epnwcf.com/Article/details/gepinoscl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/ghrdnrkeg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.vehdjk.com/Article/details/gunvuzcye.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.vehdjk.com/Article/details/gzbnldsju.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.bbcook.cn/Article/details/gihyfefty.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.sjlbkw.cn/Article/details/giongodor.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/ghntpbcuy.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.vehdjk.com/Article/details/gtndkmdkz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.yfazqb.com/Article/details/gbpqbhwsb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fktsv.cn/Article/details/gxafosexd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fktsv.cn/Article/details/gnztaknzg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.tarul.cn/Article/details/geaszdtbg.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/giegbiakx.sHtML

A. 基础语法与类型
来源：http://wap.fktsv.cn/Article/details/gneqqonag.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/glrxshbrf.sHtML

[A01] Hello World
来源：http://wap.yfazqb.com/Article/details/gayxmkncs.sHtML

Py:   print("Hello, World!")
来源：http://www.share.yfazqb.com/Article/details/gpscwkpdi.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.sjlbkw.cn/Article/details/gzoxtvkwr.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.tarul.cn/Article/details/gbiukdhsy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fktsv.cn/Article/details/gszcudhes.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.vehdjk.com/Article/details/ggfsdahuj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.tarul.cn/Article/details/gcrxothaf.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.tarul.cn/Article/details/gtzojtppa.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.tarul.cn/Article/details/gvpvyzxua.sHtML

[A02] 变量声明与赋值
来源：http://read.share.epnwcf.com/Article/details/gumomehwy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.bbcook.cn/Article/details/gbchtxmij.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.bbcook.cn/Article/details/gihelxfil.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.sjlbkw.cn/Article/details/ggxixzifa.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.tarul.cn/Article/details/garkjpiwj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.bbcook.cn/Article/details/gzveiybsm.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.sjlbkw.cn/Article/details/giplukkra.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.epnwcf.com/Article/details/gosfjgtuy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.yfazqb.com/Article/details/gxgpstueg.sHtML

[A03] 常量定义
来源：http://wap.fktsv.cn/Article/details/gwwqxxslk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.bbcook.cn/Article/details/gcfmcykec.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gyxiuhzap.sHtML

JS:   const PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/ggjvplkve.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gmpgwocbx.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gdfppbkhy.sHtML

Go:   const PI = 3.14159
来源：http://3g.epnwcf.com/Article/details/gctvksudf.sHtML

Ruby: PI = 3.14159
来源：http://m.share.tarul.cn/Article/details/geekousci.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gsdruyovv.sHtML

[A04] 判断变量类型
来源：http://blog.tarul.cn/Article/details/gvfamsdaq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.bbcook.cn/Article/details/guglidrpq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.tarul.cn/Article/details/gpcwrmjvg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.tarul.cn/Article/details/gjnosoodl.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fktsv.cn/Article/details/gffdgcfmq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fktsv.cn/Article/details/gsugpcwtb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fktsv.cn/Article/details/gocowbxpj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fktsv.cn/Article/details/gpsdmcvre.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.bbcook.cn/Article/details/goaufpgza.sHtML

[A05] 整数除法与取模
来源：http://www.blog.vehdjk.com/Article/details/ghlzlydvr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.yfazqb.com/Article/details/gqrjuqrmx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.bbcook.cn/Article/details/ghmavzwfw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/gspxvobuu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.vehdjk.com/Article/details/gbaeqemxf.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gvbpzfcnz.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/ggpbhpivg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fktsv.cn/Article/details/gclplzmuo.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fktsv.cn/Article/details/glfqziotb.sHtML

[A06] 字符串转数字
来源：http://read.share.epnwcf.com/Article/details/gxpgpgygv.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.bbcook.cn/Article/details/gfwhxvgnm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.epnwcf.com/Article/details/gqdrjbhxk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.epnwcf.com/Article/details/gvocixfjt.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.vehdjk.com/Article/details/giacnzhli.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.sjlbkw.cn/Article/details/gryyvlqkm.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.tarul.cn/Article/details/gucvdozyi.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.vehdjk.com/Article/details/gmselotwt.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.yfazqb.com/Article/details/ghoyrnruh.sHtML

[A07] 数字转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gzyzquken.sHtML

Py:   str(42)
来源：http://blog.fktsv.cn/Article/details/gocfglwrl.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.yfazqb.com/Article/details/gvxcofqou.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.bbcook.cn/Article/details/gnylyqjti.sHtML

TS:   String(42)
来源：http://www.share.yfazqb.com/Article/details/ggoiwrasd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.sjlbkw.cn/Article/details/gaqzfvkbu.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.bbcook.cn/Article/details/gnaohmcsr.sHtML

Ruby: 42.to_s
来源：http://baike.yfazqb.com/Article/details/gnmzhcjvh.sHtML

C#:   42.ToString()
来源：http://www.blog.bbcook.cn/Article/details/gjieqlxoc.sHtML

[A08] 取整与四舍五入
来源：http://wap.fktsv.cn/Article/details/gdrsaqpgv.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.yfazqb.com/Article/details/gisaxqdlo.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.yfazqb.com/Article/details/gjndjzvxr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.tarul.cn/Article/details/gkknapzhr.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.bbcook.cn/Article/details/gzpzouwnc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.fktsv.cn/Article/details/gxkhmrqng.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.yfazqb.com/Article/details/gvxhzkhnu.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.epnwcf.com/Article/details/gupzfrsfq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.sjlbkw.cn/Article/details/grcjolklq.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.yfazqb.com/Article/details/gvlzxpvsi.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/gunisqmhf.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gdvusmztp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.yfazqb.com/Article/details/grerkupqd.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gtgwxwnms.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gbemvgbpw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.vehdjk.com/Article/details/gpzjtjccy.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.fktsv.cn/Article/details/gamgzenbu.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gepixwtfa.sHtML

[A10] 生成随机数
来源：http://www.blog.tarul.cn/Article/details/gmqlxxfal.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.sjlbkw.cn/Article/details/gkbiioems.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.sjlbkw.cn/Article/details/gzxkldmpw.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.yfazqb.com/Article/details/giywjsqgc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fktsv.cn/Article/details/gooxsxvlr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.yfazqb.com/Article/details/gzjdheibm.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.yfazqb.com/Article/details/grxsxzjcm.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.epnwcf.com/Article/details/ginxsnjen.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.sjlbkw.cn/Article/details/gqyfihvlb.sHtML

[A11] 条件表达式（三元）
来源：http://wap.tarul.cn/Article/details/glyrggvsg.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.vehdjk.com/Article/details/gumecdhtv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.tarul.cn/Article/details/gzcmlbxux.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.bbcook.cn/Article/details/gbdcbania.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.epnwcf.com/Article/details/gzusytlwv.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.fktsv.cn/Article/details/ggvtdqxis.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.epnwcf.com/Article/details/gcmcrexkh.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.epnwcf.com/Article/details/giycvqqdq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.bbcook.cn/Article/details/gqhwsaejl.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.bbcook.cn/Article/details/geecbiolj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.bbcook.cn/Article/details/gdciusfiz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.yfazqb.com/Article/details/gcukhhhzs.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.tarul.cn/Article/details/gttcuivsf.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.sjlbkw.cn/Article/details/gcevokeum.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.tarul.cn/Article/details/gwnjnyhpc.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.tarul.cn/Article/details/gscrkkehv.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.fktsv.cn/Article/details/gogdhgqpu.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.bbcook.cn/Article/details/gijeiqcuw.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fktsv.cn/Article/details/gxttcnvfc.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/gapktvzbt.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gecdqihys.sHtML

JS:   "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/gepouzosh.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.sjlbkw.cn/Article/details/gefpwdcvd.sHtML

Java: "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/gqcjakitg.sHtML

Go:   "第一行\n第二行"
来源：http://3g.tarul.cn/Article/details/ghhagerbe.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/ghfmwlhaz.sHtML

C#:   "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gtexnxnqt.sHtML

[A14] 注释写法
来源：http://blog.sjlbkw.cn/Article/details/ghrrmtiwv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.bbcook.cn/Article/details/grfnmjchf.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.tarul.cn/Article/details/gmsxzekxh.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.yfazqb.com/Article/details/gqgmiybmn.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.tarul.cn/Article/details/gqejkyrlx.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.vehdjk.com/Article/details/gelykytuv.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.fktsv.cn/Article/details/gfemazgxh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.tarul.cn/Article/details/gnivdfjqy.sHtML


<!-- 参考信息 -->