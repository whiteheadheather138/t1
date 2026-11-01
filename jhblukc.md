代发 wailian999

[U85] JS：可选链
来源：http://wap.vehdjk.com/Article/details/geebgucll.sHtML

a?.b?.c
来源：http://www.blog.vehdjk.com/Article/details/gdmmpahbi.sHtML

[U86] JS：空值合并
来源：http://read.share.tarul.cn/Article/details/gusudhcoo.sHtML

a ?? b
来源：http://read.share.yfazqb.com/Article/details/gnwcnbcex.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.yfazqb.com/Article/details/gtqnrrlpp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.vehdjk.com/Article/details/gwquhccyx.sHtML

[U88] JS：对象展开合并
来源：http://3g.vehdjk.com/Article/details/gycnhlobn.sHtML

{ ...a, ...b }
来源：http://www.share.sjlbkw.cn/Article/details/gmlrvjebh.sHtML

[U89] JS：数组去重
来源：http://blog.epnwcf.com/Article/details/gzuiccwks.sHtML

[...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gxhpxjagq.sHtML

[U90] JS：数字数组排序
来源：http://wap.fktsv.cn/Article/details/gfzgbbbfv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/gmuepqcaj.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.tarul.cn/Article/details/glrtwfhty.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.tarul.cn/Article/details/gkntwtskj.sHtML

[U92] JS：深拷贝
来源：http://read.share.yfazqb.com/Article/details/gguibbvqb.sHtML

structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gljberzoi.sHtML

[U93] JS：模板字符串
来源：http://www.blog.tarul.cn/Article/details/gnctnkizl.sHtML

`共 ${n} 条`
来源：http://www.blog.bbcook.cn/Article/details/gyehtcvxt.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gtggltoxe.sHtML

const double = x => x * 2;
来源：http://www.blog.vehdjk.com/Article/details/gsqrgigwr.sHtML

[U95] JS：Promise 包装
来源：http://mobile.epnwcf.com/Article/details/ggzstnndh.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.vehdjk.com/Article/details/gaymzhjdl.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.sjlbkw.cn/Article/details/gamganplj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.epnwcf.com/Article/details/gdgkghwem.sHtML

[U97] JS：并发请求
来源：http://read.share.fktsv.cn/Article/details/gdklkkjvm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gbymczklt.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.yfazqb.com/Article/details/gmoehconc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.epnwcf.com/Article/details/glajcudnx.sHtML

[U99] JS：事件监听
来源：http://www.share.sjlbkw.cn/Article/details/gsamxybjk.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.vehdjk.com/Article/details/gqbvznckb.sHtML

[U100] JS：DOM 查询
来源：http://baike.fktsv.cn/Article/details/gcnwsbino.sHtML

document.querySelector(".item")
来源：http://wap.yfazqb.com/Article/details/gxncdbtzg.sHtML

[U101] JS：classList 操作
来源：http://m.share.sjlbkw.cn/Article/details/ginoegkox.sHtML

el.classList.toggle("active")
来源：http://m.share.vehdjk.com/Article/details/gvvsnghpw.sHtML

[U102] JS：本地存储
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnkegpur.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.epnwcf.com/Article/details/gqokbgxaq.sHtML

[U103] JS：定时器
来源：http://3g.tarul.cn/Article/details/gkgeaztpg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.sjlbkw.cn/Article/details/gfrcamrdx.sHtML

[U104] JS：防抖
来源：http://read.share.epnwcf.com/Article/details/gbfhhlixl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gpfdvfgof.sHtML

[U105] JS：节流
来源：http://wap.vehdjk.com/Article/details/gqhdqfenm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.sjlbkw.cn/Article/details/gxedmavgo.sHtML

[U106] JS：日期格式化
来源：http://www.blog.vehdjk.com/Article/details/gkuabvmug.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fktsv.cn/Article/details/gcfxdvuky.sHtML

[U107] JS：数字千分位
来源：http://m.share.bbcook.cn/Article/details/gicmngpka.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fktsv.cn/Article/details/gxvosxovy.sHtML

[U108] JS：随机整数
来源：http://m.share.sjlbkw.cn/Article/details/gsrqimbzh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.tarul.cn/Article/details/gwevyueyp.sHtML

[U109] JS：数组分组
来源：http://m.share.sjlbkw.cn/Article/details/gxdjacjjf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.sjlbkw.cn/Article/details/guktvffec.sHtML

[U110] JS：数组分块
来源：http://blog.yfazqb.com/Article/details/gbidbbrdp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.vehdjk.com/Article/details/gxgnyduqm.sHtML

[U111] JS：对象转 Map
来源：http://www.share.tarul.cn/Article/details/gjekidpft.sHtML

new Map(Object.entries(obj))
来源：http://read.share.epnwcf.com/Article/details/gpxwlbatt.sHtML

[U112] JS：字符串补位
来源：http://mobile.fktsv.cn/Article/details/gaizimpwi.sHtML

"7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gvrtgtala.sHtML

[U113] JS：正则替换全部
来源：http://baike.vehdjk.com/Article/details/gsmqhjbua.sHtML

s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/gioqfsxri.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.sjlbkw.cn/Article/details/gvfykmzlt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.bbcook.cn/Article/details/gxnrgcejd.sHtML

[U115] JS：生成 UUID
来源：http://www.share.vehdjk.com/Article/details/gwzjxllup.sHtML

crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/gplykmwij.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.sjlbkw.cn/Article/details/geipkhmqm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fktsv.cn/Article/details/gbbnukphe.sHtML

[U117] JS：单元测试
来源：http://www.blog.tarul.cn/Article/details/gngpfdcwb.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.sjlbkw.cn/Article/details/gcpzcqlfm.sHtML

[U118] JS：开发服务器
来源：http://baike.tarul.cn/Article/details/gynrabbfn.sHtML

npm i -D vite;  npx vite
来源：http://www.share.bbcook.cn/Article/details/grdtnwbtw.sHtML

[U119] JS：生产构建
来源：http://m.share.fktsv.cn/Article/details/gnprjgqas.sHtML

npx vite build
来源：http://wap.vehdjk.com/Article/details/gnegourdz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.vehdjk.com/Article/details/gwcuytuop.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.bbcook.cn/Article/details/gcmvtgqco.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gmauwylxo.sHtML

统计汇总
来源：http://m.share.bbcook.cn/Article/details/glnfutxpn.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/guyvmfhks.sHtML

按语言统计（条）：
来源：http://blog.yfazqb.com/Article/details/grehzsexo.sHtML

Python ......... 252
来源：http://blog.tarul.cn/Article/details/gjahakrka.sHtML

PHP ............ 252
来源：http://baike.tarul.cn/Article/details/gtvxlyuoh.sHtML

JavaScript ..... 252
来源：http://blog.tarul.cn/Article/details/ggxdwgxrg.sHtML

TypeScript ..... 212
来源：http://m.share.yfazqb.com/Article/details/gkvdydqtr.sHtML

Java ........... 212
来源：http://blog.vehdjk.com/Article/details/gfxmovpmt.sHtML

Go ............. 212
来源：http://baike.epnwcf.com/Article/details/gtoelajga.sHtML

Ruby ........... 212
来源：http://baike.yfazqb.com/Article/details/grmurhlbq.sHtML

C# ............. 212
来源：http://m.share.yfazqb.com/Article/details/gzaommgpg.sHtML

C .............. 30
来源：http://m.share.bbcook.cn/Article/details/gbascvvrd.sHtML

C++ ............ 30
来源：http://www.share.yfazqb.com/Article/details/grvyiazue.sHtML

SQL ............ 90
来源：http://www.blog.vehdjk.com/Article/details/gogmcbrqc.sHtML

Bash ........... 80
来源：http://mobile.tarul.cn/Article/details/gahzrjpuj.sHtML

Kotlin ......... 15
来源：http://mobile.tarul.cn/Article/details/gdeytagmh.sHtML

Swift .......... 15
来源：http://3g.vehdjk.com/Article/details/gwrbffzsd.sHtML

Lua ............ 10
来源：http://mobile.vehdjk.com/Article/details/gawakjvpi.sHtML

Perl ........... 10
来源：http://blog.bbcook.cn/Article/details/gwhrpxhlt.sHtML

Scala .......... 10
来源：http://www.share.yfazqb.com/Article/details/gpmyzpeoo.sHtML

------------------------------------
来源：http://blog.fktsv.cn/Article/details/gbdgbgsnu.sHtML

合计 ........... 2106 条
来源：http://3g.yfazqb.com/Article/details/gjbxqyhdf.sHtML

按章节统计：
来源：http://read.share.vehdjk.com/Article/details/gvwzmynle.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.yfazqb.com/Article/details/gcbwsmcrt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.bbcook.cn/Article/details/gprtoowsi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.vehdjk.com/Article/details/gpyzdyook.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.yfazqb.com/Article/details/gncusbigb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.epnwcf.com/Article/details/gfgxagoae.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.vehdjk.com/Article/details/gxpxedxsp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.sjlbkw.cn/Article/details/gbdjpddrf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.vehdjk.com/Article/details/gnkpwchte.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gyrhwldmr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.bbcook.cn/Article/details/giaraugvo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gcimdbmct.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gdhfbequo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gkuyafbtz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.vehdjk.com/Article/details/gdfqoiaia.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.bbcook.cn/Article/details/gnzfiiiqw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gxwdaukxn.sHtML

Q SQL 专题                              90
来源：http://www.blog.sjlbkw.cn/Article/details/gyseqexpi.sHtML

R Bash 专题                             80
来源：http://mobile.bbcook.cn/Article/details/gcqvkkrfz.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fktsv.cn/Article/details/ggvfvgigy.sHtML

T 其他语言补充                          60
来源：http://www.share.yfazqb.com/Article/details/gyopjqdcr.sHtML

U 高频实用片段                         120
来源：http://www.blog.vehdjk.com/Article/details/gpafwghdq.sHtML

------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gynajmctb.sHtML

合计                                  2106 条
来源：http://baike.fktsv.cn/Article/details/gtbdlyuna.sHtML

--------------------------------------------------------------------------------
来源：http://3g.epnwcf.com/Article/details/gnowgwfgn.sHtML

使用提醒
来源：http://www.share.tarul.cn/Article/details/gyimlwsnx.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gmagcfvyu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.sjlbkw.cn/Article/details/gkocfrrdd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.vehdjk.com/Article/details/gjpwlvqib.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.sjlbkw.cn/Article/details/gybbnjxam.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.bbcook.cn/Article/details/ghkyfvbpv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.yfazqb.com/Article/details/gefhrfinj.sHtML

—— 文件结束 ——
来源：http://3g.vehdjk.com/Article/details/gpojhtfxq.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gdaqzipkw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fktsv.cn/Article/details/gypfogbeq.sHtML

Common Programming Examples Cheat Book
来源：http://3g.sjlbkw.cn/Article/details/gemyeoxab.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ggjklumda.sHtML

【收录内容】
来源：http://3g.tarul.cn/Article/details/gyqrcdsdx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.sjlbkw.cn/Article/details/gpfvtqoca.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.sjlbkw.cn/Article/details/gmyscxptr.sHtML

SQL · Bash · C · C++
来源：http://read.share.fktsv.cn/Article/details/gjzanivuw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.tarul.cn/Article/details/gagfqredj.sHtML

【使用说明】
来源：http://read.share.bbcook.cn/Article/details/gcjisvgjn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.epnwcf.com/Article/details/gbyqmzxeo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.tarul.cn/Article/details/gcnhzzxmj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.tarul.cn/Article/details/gcfeffmlt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.bbcook.cn/Article/details/gmynlaffx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.epnwcf.com/Article/details/gkiibyens.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.epnwcf.com/Article/details/gxjqkngkw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.epnwcf.com/Article/details/gcxptvgov.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.epnwcf.com/Article/details/gdzcljakp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.bbcook.cn/Article/details/gowzneogn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.yfazqb.com/Article/details/gnayilldd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fktsv.cn/Article/details/gzveqagkv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.sjlbkw.cn/Article/details/gekxslxck.sHtML

【文件统计】
来源：http://read.share.tarul.cn/Article/details/gzieayovc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fktsv.cn/Article/details/gqdqkgdao.sHtML

--------------------------------------------------------------------------------
来源：http://baike.tarul.cn/Article/details/gmtxmbhrp.sHtML

目  录
来源：http://read.share.bbcook.cn/Article/details/gwcbnfalv.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjrnpfkk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.bbcook.cn/Article/details/gvxufnnfm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.bbcook.cn/Article/details/gcbfcymfc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.sjlbkw.cn/Article/details/grqtpehjo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.vehdjk.com/Article/details/gzzioxqhf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.epnwcf.com/Article/details/gpgwxbxtr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fktsv.cn/Article/details/gjdploqbn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.tarul.cn/Article/details/geqzaljza.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.tarul.cn/Article/details/gkpbzidqk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/ghyqznqps.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.sjlbkw.cn/Article/details/gqpxwnuob.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.tarul.cn/Article/details/gptiklafe.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/gsswjkkfn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.vehdjk.com/Article/details/gnfneqedh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.tarul.cn/Article/details/grwpeembr.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.vehdjk.com/Article/details/gfljgnifv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gnzcvajcv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.yfazqb.com/Article/details/glqttitoy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.yfazqb.com/Article/details/gmszypurs.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fktsv.cn/Article/details/gwiaeeedy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.sjlbkw.cn/Article/details/gprfnuurv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.bbcook.cn/Article/details/gafmttpvk.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gdcrjsqnj.sHtML

A. 基础语法与类型
来源：http://wap.tarul.cn/Article/details/gyysclzqq.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gadsnotpj.sHtML

[A01] Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gtxgcwplv.sHtML

Py:   print("Hello, World!")
来源：http://blog.vehdjk.com/Article/details/gqzoehbkk.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.sjlbkw.cn/Article/details/gwjfgltxx.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.bbcook.cn/Article/details/gpmeujhbf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.yfazqb.com/Article/details/gzmxpitil.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.yfazqb.com/Article/details/gbfklnnyo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.vehdjk.com/Article/details/gkkyxtuiv.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.vehdjk.com/Article/details/gbgnstdbr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.epnwcf.com/Article/details/gkyyrxchl.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.sjlbkw.cn/Article/details/gulpmdunv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.bbcook.cn/Article/details/gzhlckdid.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.tarul.cn/Article/details/giwozvuts.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.vehdjk.com/Article/details/gbvmmdggb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.sjlbkw.cn/Article/details/gvnfbjpdb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.epnwcf.com/Article/details/gjpakphhy.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fktsv.cn/Article/details/gdsmesott.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fktsv.cn/Article/details/gfppmmxrn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fktsv.cn/Article/details/gidggxqmf.sHtML

[A03] 常量定义
来源：http://read.share.tarul.cn/Article/details/gwgwjrzks.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.yfazqb.com/Article/details/gsexgsjql.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/ghogfvkug.sHtML

JS:   const PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gofrvfmdh.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gcjvidgtp.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gyoaxwazp.sHtML

Go:   const PI = 3.14159
来源：http://wap.vehdjk.com/Article/details/ggcgowatl.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fktsv.cn/Article/details/gqsopbvps.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/glrntflnk.sHtML

[A04] 判断变量类型
来源：http://baike.epnwcf.com/Article/details/gtkgvqezf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.yfazqb.com/Article/details/glvvjlpsr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.bbcook.cn/Article/details/gctzctchc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.epnwcf.com/Article/details/gddfvppgm.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.bbcook.cn/Article/details/gvnyjhkxt.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.sjlbkw.cn/Article/details/gqidjmynk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.yfazqb.com/Article/details/grwykonhy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.yfazqb.com/Article/details/ghalsnjli.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.sjlbkw.cn/Article/details/gwucvjppx.sHtML

[A05] 整数除法与取模
来源：http://wap.bbcook.cn/Article/details/gvivzjjgy.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.vehdjk.com/Article/details/ghfcmggth.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gjxmwjpue.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gimshfxvm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gqpxolljb.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.yfazqb.com/Article/details/gtibyedfe.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/ghrqjhakn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.yfazqb.com/Article/details/glkussrej.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.bbcook.cn/Article/details/grmrihzqi.sHtML

[A06] 字符串转数字
来源：http://baike.sjlbkw.cn/Article/details/gwjpzuzcj.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.vehdjk.com/Article/details/ghzrdwrrn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.sjlbkw.cn/Article/details/grdokstco.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.tarul.cn/Article/details/gftfwpcrg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fktsv.cn/Article/details/globgzypx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.yfazqb.com/Article/details/gpxlfnuui.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.sjlbkw.cn/Article/details/gssxhapyw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.sjlbkw.cn/Article/details/gyubgtldf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.yfazqb.com/Article/details/gvraopxsu.sHtML

[A07] 数字转字符串
来源：http://www.blog.epnwcf.com/Article/details/gjdalsfyx.sHtML

Py:   str(42)
来源：http://www.m.share.bbcook.cn/Article/details/gdqqocapg.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.yfazqb.com/Article/details/gidgomkgg.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fktsv.cn/Article/details/geemmuhzr.sHtML

TS:   String(42)
来源：http://www.m.share.fktsv.cn/Article/details/gzbxkotlr.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.epnwcf.com/Article/details/gamnffdpw.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.vehdjk.com/Article/details/gkwbkqtxy.sHtML

Ruby: 42.to_s
来源：http://blog.vehdjk.com/Article/details/gdzhypuug.sHtML

C#:   42.ToString()
来源：http://read.share.bbcook.cn/Article/details/gjlhixurx.sHtML

[A08] 取整与四舍五入
来源：http://m.share.sjlbkw.cn/Article/details/gxtehauef.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.yfazqb.com/Article/details/grudtofxc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.bbcook.cn/Article/details/glqmmsvze.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.vehdjk.com/Article/details/gojjwnhtj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.yfazqb.com/Article/details/gcknfbcck.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.epnwcf.com/Article/details/gqqygppra.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.epnwcf.com/Article/details/ggidstedt.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.tarul.cn/Article/details/glqrkricv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/gcyitxzjw.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.bbcook.cn/Article/details/gpimlqinn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gagvpdigh.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gxvziockl.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.tarul.cn/Article/details/gxbpeeiga.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gebdsjqcd.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gupjvikzj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.tarul.cn/Article/details/gxfzadrws.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.yfazqb.com/Article/details/gjnmcboho.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.tarul.cn/Article/details/gxjxukatp.sHtML

[A10] 生成随机数
来源：http://mobile.yfazqb.com/Article/details/ghooqhpqo.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.vehdjk.com/Article/details/goitncpbf.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.sjlbkw.cn/Article/details/gxupcyihy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.sjlbkw.cn/Article/details/gmcxvumpq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.epnwcf.com/Article/details/ghpumxfwv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.sjlbkw.cn/Article/details/gwrnrxyof.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.sjlbkw.cn/Article/details/gvpfnczgh.sHtML

Ruby: rand(1..100)
来源：http://www.blog.yfazqb.com/Article/details/glzgyyica.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.epnwcf.com/Article/details/gwkedkfsp.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.bbcook.cn/Article/details/gkpsuqzel.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.vehdjk.com/Article/details/gqxaperpa.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.bbcook.cn/Article/details/gwekgkjrg.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.yfazqb.com/Article/details/gzbuoyiqg.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.vehdjk.com/Article/details/gluebjysm.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.yfazqb.com/Article/details/gjdmhcigg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.yfazqb.com/Article/details/gpbfvpuif.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.yfazqb.com/Article/details/gkhkpkqmu.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.bbcook.cn/Article/details/gnwyqiade.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.bbcook.cn/Article/details/gqvupzgae.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.fktsv.cn/Article/details/gzoabvein.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.epnwcf.com/Article/details/glyzumrch.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.bbcook.cn/Article/details/gclqwwgas.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.bbcook.cn/Article/details/gqxiuwgtz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.tarul.cn/Article/details/gcpbgexfo.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.tarul.cn/Article/details/gtlhrwyyq.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.sjlbkw.cn/Article/details/gfytlxptl.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.sjlbkw.cn/Article/details/geeszuvnp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.yfazqb.com/Article/details/gqhqavzbg.sHtML

Py:   "第一行\n第二行"
来源：http://3g.fktsv.cn/Article/details/gfviepfjr.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/grkthmxzo.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/gcifphsgb.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/gfqxaeolg.sHtML

Java: "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/gfvmglpqy.sHtML

Go:   "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gdgpwhofl.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/gijqmffgq.sHtML

C#:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gifnsqnxa.sHtML

[A14] 注释写法
来源：http://baike.sjlbkw.cn/Article/details/gubthkwmr.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fktsv.cn/Article/details/gupgmyydo.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.vehdjk.com/Article/details/gsxoisrub.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/glqdmnmyy.sHtML


<!-- 参考信息 -->