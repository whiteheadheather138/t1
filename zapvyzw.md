代发 wailian999

[U91] JS：对象键值遍历
来源：http://read.share.yfazqb.com/Article/details/gxdzxtndz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.vehdjk.com/Article/details/ghhblesgq.sHtML

[U92] JS：深拷贝
来源：http://m.share.vehdjk.com/Article/details/gthdagkws.sHtML

structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/glwdkgjpb.sHtML

[U93] JS：模板字符串
来源：http://mobile.sjlbkw.cn/Article/details/gydjywurx.sHtML

`共 ${n} 条`
来源：http://m.share.fktsv.cn/Article/details/gbsrtzhtz.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvagewir.sHtML

const double = x => x * 2;
来源：http://read.share.epnwcf.com/Article/details/gidyhdwsp.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.vehdjk.com/Article/details/gpyjwkzfx.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.bbcook.cn/Article/details/gonotkvue.sHtML

[U96] JS：async/await 与异常
来源：http://baike.tarul.cn/Article/details/gfirldoiw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.tarul.cn/Article/details/gqkipzisy.sHtML

[U97] JS：并发请求
来源：http://m.share.fktsv.cn/Article/details/gamxueuyr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gtubfddkh.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.bbcook.cn/Article/details/gbcdoywjd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.epnwcf.com/Article/details/gixalctwy.sHtML

[U99] JS：事件监听
来源：http://baike.epnwcf.com/Article/details/gvzzsnzok.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.sjlbkw.cn/Article/details/glkbvtlbz.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.yfazqb.com/Article/details/gafjaecbn.sHtML

document.querySelector(".item")
来源：http://www.blog.vehdjk.com/Article/details/gomvbkops.sHtML

[U101] JS：classList 操作
来源：http://wap.tarul.cn/Article/details/gjzkcscpv.sHtML

el.classList.toggle("active")
来源：http://www.blog.tarul.cn/Article/details/gkgnypvrw.sHtML

[U102] JS：本地存储
来源：http://read.share.tarul.cn/Article/details/gnjbmvjdd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.epnwcf.com/Article/details/gifohdapf.sHtML

[U103] JS：定时器
来源：http://www.m.share.tarul.cn/Article/details/gpihitfzl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.bbcook.cn/Article/details/gcawphhsm.sHtML

[U104] JS：防抖
来源：http://www.blog.vehdjk.com/Article/details/gaptjdiel.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gitdvxsta.sHtML

[U105] JS：节流
来源：http://www.m.share.epnwcf.com/Article/details/gzcumgdyn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.sjlbkw.cn/Article/details/gqqwdhuze.sHtML

[U106] JS：日期格式化
来源：http://read.share.vehdjk.com/Article/details/gzypyfbip.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.yfazqb.com/Article/details/gmtfzbuux.sHtML

[U107] JS：数字千分位
来源：http://www.blog.bbcook.cn/Article/details/glvlwnngp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.yfazqb.com/Article/details/gnrtxylle.sHtML

[U108] JS：随机整数
来源：http://www.blog.vehdjk.com/Article/details/grbfmriyq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.bbcook.cn/Article/details/gltzkmgxm.sHtML

[U109] JS：数组分组
来源：http://www.blog.tarul.cn/Article/details/gxwzeimrj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.sjlbkw.cn/Article/details/gdgimoyjl.sHtML

[U110] JS：数组分块
来源：http://www.blog.yfazqb.com/Article/details/gtbkoejsa.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.tarul.cn/Article/details/gfxsulder.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fktsv.cn/Article/details/gcjvdpocw.sHtML

new Map(Object.entries(obj))
来源：http://www.share.tarul.cn/Article/details/gjfyvslcc.sHtML

[U112] JS：字符串补位
来源：http://blog.bbcook.cn/Article/details/gjkknnjbw.sHtML

"7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/geokrclwl.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.tarul.cn/Article/details/gwlhmhxff.sHtML

s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gwvznahso.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fktsv.cn/Article/details/gxpdyrmig.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/gszubznbs.sHtML

[U115] JS：生成 UUID
来源：http://mobile.bbcook.cn/Article/details/gfauqrpks.sHtML

crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/gfzxkzvqz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.bbcook.cn/Article/details/gttapjjft.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.yfazqb.com/Article/details/gdbezsxmh.sHtML

[U117] JS：单元测试
来源：http://baike.bbcook.cn/Article/details/gvvlzcnji.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.bbcook.cn/Article/details/ggvwwhrnj.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmadijug.sHtML

npm i -D vite;  npx vite
来源：http://blog.tarul.cn/Article/details/gjmuvekav.sHtML

[U119] JS：生产构建
来源：http://www.m.share.bbcook.cn/Article/details/gbjmsaaem.sHtML

npx vite build
来源：http://mobile.yfazqb.com/Article/details/grghnvcpp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.yfazqb.com/Article/details/gusedadey.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.bbcook.cn/Article/details/ggzwqpfio.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/glnmbwdjd.sHtML

统计汇总
来源：http://www.share.sjlbkw.cn/Article/details/groytstry.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ggfbwiwdy.sHtML

按语言统计（条）：
来源：http://www.share.vehdjk.com/Article/details/gxpqckvuy.sHtML

Python ......... 252
来源：http://read.share.epnwcf.com/Article/details/gudworrdf.sHtML

PHP ............ 252
来源：http://mobile.epnwcf.com/Article/details/gbdxxqlia.sHtML

JavaScript ..... 252
来源：http://baike.bbcook.cn/Article/details/gauepewka.sHtML

TypeScript ..... 212
来源：http://www.blog.yfazqb.com/Article/details/griqnynzc.sHtML

Java ........... 212
来源：http://baike.sjlbkw.cn/Article/details/grcscpwnl.sHtML

Go ............. 212
来源：http://www.share.tarul.cn/Article/details/gisbbrros.sHtML

Ruby ........... 212
来源：http://m.share.bbcook.cn/Article/details/gvslpcsbe.sHtML

C# ............. 212
来源：http://wap.fktsv.cn/Article/details/gzknofwyc.sHtML

C .............. 30
来源：http://wap.bbcook.cn/Article/details/gfopzobww.sHtML

C++ ............ 30
来源：http://www.m.share.vehdjk.com/Article/details/grsqmxjrp.sHtML

SQL ............ 90
来源：http://3g.fktsv.cn/Article/details/gmclygvkf.sHtML

Bash ........... 80
来源：http://read.share.epnwcf.com/Article/details/genxgaqgj.sHtML

Kotlin ......... 15
来源：http://wap.tarul.cn/Article/details/gzwxcocdh.sHtML

Swift .......... 15
来源：http://baike.yfazqb.com/Article/details/giukhssmp.sHtML

Lua ............ 10
来源：http://www.m.share.sjlbkw.cn/Article/details/godfylxgz.sHtML

Perl ........... 10
来源：http://www.blog.vehdjk.com/Article/details/ggvvcafmw.sHtML

Scala .......... 10
来源：http://blog.yfazqb.com/Article/details/gxnfmxfus.sHtML

------------------------------------
来源：http://baike.tarul.cn/Article/details/gynhbmzyj.sHtML

合计 ........... 2106 条
来源：http://baike.epnwcf.com/Article/details/gemxthwwr.sHtML

按章节统计：
来源：http://wap.yfazqb.com/Article/details/gyelskjmd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.tarul.cn/Article/details/gbzowzwjs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.vehdjk.com/Article/details/gahneapth.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fktsv.cn/Article/details/gvhdqhing.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.sjlbkw.cn/Article/details/gnqddbfrb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fktsv.cn/Article/details/glkzzfwyf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.epnwcf.com/Article/details/gutysqznp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fktsv.cn/Article/details/gstqzrobn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.tarul.cn/Article/details/gghufnzsl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/gcworsybk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.bbcook.cn/Article/details/gonkjvndi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/ghwkjhzqk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gtbnfbdoy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/gelveqktm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fktsv.cn/Article/details/gtntzvjtd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.vehdjk.com/Article/details/gfxmzvtxi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/gmghxzwtu.sHtML

Q SQL 专题                              90
来源：http://wap.bbcook.cn/Article/details/ggpsqcfev.sHtML

R Bash 专题                             80
来源：http://wap.yfazqb.com/Article/details/grsiezufz.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.bbcook.cn/Article/details/gaeaaveto.sHtML

T 其他语言补充                          60
来源：http://blog.vehdjk.com/Article/details/gfrffqyhc.sHtML

U 高频实用片段                         120
来源：http://www.share.epnwcf.com/Article/details/gdwmmtvru.sHtML

------------------------------------
来源：http://read.share.vehdjk.com/Article/details/gtntueobe.sHtML

合计                                  2106 条
来源：http://blog.bbcook.cn/Article/details/gkgockoit.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fktsv.cn/Article/details/gsmusadse.sHtML

使用提醒
来源：http://www.m.share.epnwcf.com/Article/details/gksssogsp.sHtML

--------------------------------------------------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gobvrqvpl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.bbcook.cn/Article/details/gnarugfmf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.bbcook.cn/Article/details/gonizrvfu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.tarul.cn/Article/details/gshxcuzcm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fktsv.cn/Article/details/gearyvnjf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.vehdjk.com/Article/details/gklwzuacx.sHtML

—— 文件结束 ——
来源：http://www.m.share.fktsv.cn/Article/details/giwblxjcw.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gcycjmedm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.tarul.cn/Article/details/gtilftmfp.sHtML

Common Programming Examples Cheat Book
来源：http://baike.yfazqb.com/Article/details/gprtqqvxo.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gtdfwlzhr.sHtML

【收录内容】
来源：http://www.share.tarul.cn/Article/details/govgxhndx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.tarul.cn/Article/details/gdocqbbvc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.epnwcf.com/Article/details/gmbawiyiz.sHtML

SQL · Bash · C · C++
来源：http://www.share.bbcook.cn/Article/details/gqjaobbkf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.epnwcf.com/Article/details/gdwtbnuux.sHtML

【使用说明】
来源：http://www.blog.vehdjk.com/Article/details/gzgpwnexl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.vehdjk.com/Article/details/gzceecygr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fktsv.cn/Article/details/gktckqqfi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.yfazqb.com/Article/details/gnzksxscg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.yfazqb.com/Article/details/gpjggwuqy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.vehdjk.com/Article/details/gbgwlxlhh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.bbcook.cn/Article/details/gfnndoesw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.tarul.cn/Article/details/gttithkvt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.yfazqb.com/Article/details/gwtoncjht.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.tarul.cn/Article/details/gljmgeldo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.vehdjk.com/Article/details/gslkxskwk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.sjlbkw.cn/Article/details/gktwncsfb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.epnwcf.com/Article/details/gueyihzsk.sHtML

【文件统计】
来源：http://wap.bbcook.cn/Article/details/gvfkpqone.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.yfazqb.com/Article/details/gszpndcjc.sHtML

--------------------------------------------------------------------------------
来源：http://wap.vehdjk.com/Article/details/gcitdjggk.sHtML

目  录
来源：http://3g.vehdjk.com/Article/details/gcmichouw.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fktsv.cn/Article/details/gligdkdmw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.vehdjk.com/Article/details/gjqdrlgpf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fktsv.cn/Article/details/gwxapyzbi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.sjlbkw.cn/Article/details/ghsvyywyn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.tarul.cn/Article/details/giviznyfw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.bbcook.cn/Article/details/gpvjnvaty.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.vehdjk.com/Article/details/gfpwybpyt.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.tarul.cn/Article/details/gbxszdvtc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.sjlbkw.cn/Article/details/gwrjhcemu.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gdritowby.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.epnwcf.com/Article/details/grsafhumy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/gdqgkcrsf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.yfazqb.com/Article/details/gqhyqjhzz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/goybdkcjx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.bbcook.cn/Article/details/gtxhswrqm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.yfazqb.com/Article/details/gzvbgzesi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/gsiktyndk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.yfazqb.com/Article/details/gqmjlgpgt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.yfazqb.com/Article/details/gpuiasyfj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.yfazqb.com/Article/details/gtfhrento.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.epnwcf.com/Article/details/gfjnutprf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.yfazqb.com/Article/details/gddgqkwlz.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/giorpnofq.sHtML

A. 基础语法与类型
来源：http://3g.tarul.cn/Article/details/grourqvhb.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gsgxfwfjy.sHtML

[A01] Hello World
来源：http://m.share.epnwcf.com/Article/details/gbfgiladq.sHtML

Py:   print("Hello, World!")
来源：http://baike.fktsv.cn/Article/details/gxvhrpcic.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.bbcook.cn/Article/details/gkyorcmka.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fktsv.cn/Article/details/gxefbpmfx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.tarul.cn/Article/details/gbtlorcdz.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.yfazqb.com/Article/details/gjfrpbudf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.yfazqb.com/Article/details/gvkbrcdyi.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.tarul.cn/Article/details/gznqflezr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.tarul.cn/Article/details/gagvmgfjq.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.vehdjk.com/Article/details/gnudbrksy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.epnwcf.com/Article/details/gokfisjgf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.bbcook.cn/Article/details/gjssjhwxn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.bbcook.cn/Article/details/gzlhzovet.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.vehdjk.com/Article/details/guuzxlimr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.tarul.cn/Article/details/gtfzgmvic.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.epnwcf.com/Article/details/gmjenpcls.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.yfazqb.com/Article/details/gyknbshag.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.vehdjk.com/Article/details/glvyalnrm.sHtML

[A03] 常量定义
来源：http://www.m.share.tarul.cn/Article/details/gywwzakna.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.vehdjk.com/Article/details/gsoiizqks.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gmgocmstl.sHtML

JS:   const PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/guasknrua.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gctvhwfku.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gaocgolfc.sHtML

Go:   const PI = 3.14159
来源：http://baike.vehdjk.com/Article/details/gtykhuxkq.sHtML

Ruby: PI = 3.14159
来源：http://3g.tarul.cn/Article/details/gpigjcflh.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gwnaugmfx.sHtML

[A04] 判断变量类型
来源：http://www.share.yfazqb.com/Article/details/gwkxdceut.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fktsv.cn/Article/details/glpacwgmg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.sjlbkw.cn/Article/details/gydcpzwgh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.tarul.cn/Article/details/gmzkhgzsk.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.yfazqb.com/Article/details/gvnhfalht.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.tarul.cn/Article/details/gmjeykull.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.epnwcf.com/Article/details/gxvqdijuy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.vehdjk.com/Article/details/gkjvbtzvw.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.sjlbkw.cn/Article/details/gtoagxufa.sHtML

[A05] 整数除法与取模
来源：http://www.share.tarul.cn/Article/details/gnbqeichy.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.tarul.cn/Article/details/gqrmeekrj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.vehdjk.com/Article/details/gtgndxvpf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/griitvzyb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.epnwcf.com/Article/details/gecgwqglo.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.vehdjk.com/Article/details/ggejmukwm.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.epnwcf.com/Article/details/gauqsjinz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/gxpvpxliw.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/glkcplwdt.sHtML

[A06] 字符串转数字
来源：http://www.m.share.epnwcf.com/Article/details/geblnpcgf.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.yfazqb.com/Article/details/gkjuaeobg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.yfazqb.com/Article/details/gcfokhwco.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.tarul.cn/Article/details/gwgffsycc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.sjlbkw.cn/Article/details/gdxwfrcsl.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.bbcook.cn/Article/details/globyufpd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.sjlbkw.cn/Article/details/gpzfakqnd.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.vehdjk.com/Article/details/gbcnwafxg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.tarul.cn/Article/details/gpecaprds.sHtML

[A07] 数字转字符串
来源：http://www.share.vehdjk.com/Article/details/gaiueoayk.sHtML

Py:   str(42)
来源：http://mobile.vehdjk.com/Article/details/gmdkuvzjk.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.tarul.cn/Article/details/gqktannkt.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.vehdjk.com/Article/details/gsuladesk.sHtML

TS:   String(42)
来源：http://www.m.share.epnwcf.com/Article/details/geynrgzfd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.sjlbkw.cn/Article/details/gzynyheqm.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.epnwcf.com/Article/details/glokrxbgh.sHtML

Ruby: 42.to_s
来源：http://www.m.share.bbcook.cn/Article/details/ggmiqsqkw.sHtML

C#:   42.ToString()
来源：http://m.share.yfazqb.com/Article/details/gntanrjmn.sHtML

[A08] 取整与四舍五入
来源：http://m.share.vehdjk.com/Article/details/gncwwjpen.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/grinudsea.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.sjlbkw.cn/Article/details/ggsprknry.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.vehdjk.com/Article/details/gwlsedmkn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.vehdjk.com/Article/details/gnxidsqab.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fktsv.cn/Article/details/gjwqflspx.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.yfazqb.com/Article/details/gjxfaocrv.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.tarul.cn/Article/details/gsruwgwlj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.tarul.cn/Article/details/gczuomoqq.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fktsv.cn/Article/details/gijdjujxl.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.tarul.cn/Article/details/giytomcps.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.vehdjk.com/Article/details/gsqyxvnae.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gmmuznmne.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gplfnfnys.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gtbfeqiyk.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.sjlbkw.cn/Article/details/gcbnjcork.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.vehdjk.com/Article/details/gsjvzyyzi.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/gmofhtqxn.sHtML

[A10] 生成随机数
来源：http://www.share.tarul.cn/Article/details/gvkpqypcb.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.sjlbkw.cn/Article/details/gnelwxwvn.sHtML

PHP:  random_int(1, 100);
来源：http://blog.sjlbkw.cn/Article/details/ghachqneu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.vehdjk.com/Article/details/gdvheaghq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.vehdjk.com/Article/details/gspgkaqnl.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.sjlbkw.cn/Article/details/gwggxgdlp.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.tarul.cn/Article/details/gyrapqugc.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fktsv.cn/Article/details/gmtfsrpmq.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.epnwcf.com/Article/details/gzeglxqqp.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.yfazqb.com/Article/details/grfevsdud.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.tarul.cn/Article/details/gyopcvslv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.epnwcf.com/Article/details/gycfuhrhr.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.tarul.cn/Article/details/gyohwryyx.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/girpausjs.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gvabavjkv.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.sjlbkw.cn/Article/details/gflkhyiur.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.epnwcf.com/Article/details/gbsyoikyf.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/gcwlbmdrm.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.tarul.cn/Article/details/gexbelqpz.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.fktsv.cn/Article/details/gddojnunf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.vehdjk.com/Article/details/gzedclnxc.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.bbcook.cn/Article/details/gyshicvqi.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.yfazqb.com/Article/details/gmzavccov.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.tarul.cn/Article/details/ggldqhvjm.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fktsv.cn/Article/details/gbvttxkxd.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.tarul.cn/Article/details/gvawlodsy.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.bbcook.cn/Article/details/gvxwkpucz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.epnwcf.com/Article/details/gybvwbvxh.sHtML

Py:   "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gobzxvuwo.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gucpubwau.sHtML

JS:   "第一行\n第二行"
来源：http://wap.vehdjk.com/Article/details/gxdwulzcx.sHtML

TS:   "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gpccqzaht.sHtML

Java: "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gwtrnefpr.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/gfftotlde.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/gfghksqgp.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gxeevlsvk.sHtML

[A14] 注释写法
来源：http://m.share.tarul.cn/Article/details/gjjmbeqrt.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.bbcook.cn/Article/details/gqbwevstz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fktsv.cn/Article/details/gkcmgjtrv.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.tarul.cn/Article/details/gmuibygjr.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/goqilodgi.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.tarul.cn/Article/details/guockwnqt.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.bbcook.cn/Article/details/gjdresniq.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.tarul.cn/Article/details/glxojfwpx.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.sjlbkw.cn/Article/details/gwkgxwqmf.sHtML

[A15] 空值判断与默认值
来源：http://www.share.bbcook.cn/Article/details/grufodbfm.sHtML

Py:   value = data or "默认值"
来源：http://read.share.tarul.cn/Article/details/gmezlvbnb.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.bbcook.cn/Article/details/grsshynbs.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.tarul.cn/Article/details/gfecgfwcl.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.vehdjk.com/Article/details/guaghxzpb.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.epnwcf.com/Article/details/gtknclrho.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.tarul.cn/Article/details/gwzmxvykm.sHtML


<!-- 参考信息 -->