代发 wailian999

[U95] JS：Promise 包装
来源：http://m.share.yfazqb.com/Article/details/gvjzkebtp.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.vehdjk.com/Article/details/gziaizqwr.sHtML

[U96] JS：async/await 与异常
来源：http://blog.tarul.cn/Article/details/gtsditmfn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/ghscxenhe.sHtML

[U97] JS：并发请求
来源：http://baike.tarul.cn/Article/details/ghxmxndlo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/guobqtdst.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.yfazqb.com/Article/details/gqymjzlrp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.sjlbkw.cn/Article/details/gioeczzgy.sHtML

[U99] JS：事件监听
来源：http://blog.epnwcf.com/Article/details/gmypyqoqx.sHtML

el.addEventListener("click", e => {})
来源：http://baike.yfazqb.com/Article/details/glcughbhv.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fktsv.cn/Article/details/gwdnoqtuy.sHtML

document.querySelector(".item")
来源：http://www.m.share.fktsv.cn/Article/details/gabihyyov.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.tarul.cn/Article/details/geuqwwqfn.sHtML

el.classList.toggle("active")
来源：http://www.share.epnwcf.com/Article/details/ggvzbsspm.sHtML

[U102] JS：本地存储
来源：http://www.share.yfazqb.com/Article/details/glfpdcjwn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.yfazqb.com/Article/details/gntdyrilg.sHtML

[U103] JS：定时器
来源：http://read.share.yfazqb.com/Article/details/gxtcxegfd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.vehdjk.com/Article/details/gullblskk.sHtML

[U104] JS：防抖
来源：http://baike.bbcook.cn/Article/details/gkbcvwnsx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/gohkauycq.sHtML

[U105] JS：节流
来源：http://m.share.vehdjk.com/Article/details/gkaprhsjx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.yfazqb.com/Article/details/gndgutmhw.sHtML

[U106] JS：日期格式化
来源：http://www.share.epnwcf.com/Article/details/gbxqowyti.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.yfazqb.com/Article/details/gkzmokwtm.sHtML

[U107] JS：数字千分位
来源：http://m.share.sjlbkw.cn/Article/details/ghvzpcdtb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/ghkzqymkg.sHtML

[U108] JS：随机整数
来源：http://www.m.share.epnwcf.com/Article/details/gyctaenpk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.vehdjk.com/Article/details/glvfmtzuu.sHtML

[U109] JS：数组分组
来源：http://baike.vehdjk.com/Article/details/gpwjaucmf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fktsv.cn/Article/details/gvvxejbih.sHtML

[U110] JS：数组分块
来源：http://3g.epnwcf.com/Article/details/gmwnnyhzd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fktsv.cn/Article/details/grridzbtq.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fktsv.cn/Article/details/giaeppltb.sHtML

new Map(Object.entries(obj))
来源：http://blog.bbcook.cn/Article/details/gipfrpqew.sHtML

[U112] JS：字符串补位
来源：http://www.blog.bbcook.cn/Article/details/gndztkivw.sHtML

"7".padStart(3, "0")
来源：http://3g.vehdjk.com/Article/details/gniuknptr.sHtML

[U113] JS：正则替换全部
来源：http://www.share.yfazqb.com/Article/details/glvtcvcov.sHtML

s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gnkvmdmdj.sHtML

[U114] JS：JSON 深比较
来源：http://3g.vehdjk.com/Article/details/gpvfrjlpd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.tarul.cn/Article/details/gbieazdan.sHtML

[U115] JS：生成 UUID
来源：http://m.share.yfazqb.com/Article/details/gobbwqyyw.sHtML

crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gcpubvfzh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.epnwcf.com/Article/details/gszfdzuzc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fktsv.cn/Article/details/gfisorkkh.sHtML

[U117] JS：单元测试
来源：http://www.share.fktsv.cn/Article/details/gbaqzcxdq.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.epnwcf.com/Article/details/gqwfksaiu.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.vehdjk.com/Article/details/glbjdadjm.sHtML

npm i -D vite;  npx vite
来源：http://wap.fktsv.cn/Article/details/gadnmgsrw.sHtML

[U119] JS：生产构建
来源：http://blog.epnwcf.com/Article/details/gssxmsgle.sHtML

npx vite build
来源：http://www.blog.sjlbkw.cn/Article/details/gjlxdsklp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.epnwcf.com/Article/details/geietvryb.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fktsv.cn/Article/details/gltevaiqi.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gprgmthdf.sHtML

统计汇总
来源：http://m.share.bbcook.cn/Article/details/griyqfibc.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gdpelrkal.sHtML

按语言统计（条）：
来源：http://www.m.share.vehdjk.com/Article/details/gzrjiqxul.sHtML

Python ......... 252
来源：http://3g.epnwcf.com/Article/details/gvtyqfiyx.sHtML

PHP ............ 252
来源：http://m.share.epnwcf.com/Article/details/gszsrdmpv.sHtML

JavaScript ..... 252
来源：http://3g.yfazqb.com/Article/details/gnguvsxzy.sHtML

TypeScript ..... 212
来源：http://www.blog.bbcook.cn/Article/details/gvctmpwvw.sHtML

Java ........... 212
来源：http://blog.sjlbkw.cn/Article/details/gnsmwgjtq.sHtML

Go ............. 212
来源：http://www.share.vehdjk.com/Article/details/gyptuvrmj.sHtML

Ruby ........... 212
来源：http://read.share.epnwcf.com/Article/details/gkgcmvjyl.sHtML

C# ............. 212
来源：http://wap.epnwcf.com/Article/details/gdjdmmpkr.sHtML

C .............. 30
来源：http://m.share.epnwcf.com/Article/details/ggyjcdvgz.sHtML

C++ ............ 30
来源：http://www.blog.yfazqb.com/Article/details/gshighkxa.sHtML

SQL ............ 90
来源：http://wap.fktsv.cn/Article/details/gpguvwzjh.sHtML

Bash ........... 80
来源：http://read.share.bbcook.cn/Article/details/gigdydcgf.sHtML

Kotlin ......... 15
来源：http://www.blog.fktsv.cn/Article/details/gappiragp.sHtML

Swift .......... 15
来源：http://read.share.tarul.cn/Article/details/gvorfvmkc.sHtML

Lua ............ 10
来源：http://www.blog.yfazqb.com/Article/details/gocdapbjv.sHtML

Perl ........... 10
来源：http://www.blog.vehdjk.com/Article/details/gmlprrqlc.sHtML

Scala .......... 10
来源：http://wap.bbcook.cn/Article/details/gzysxhcff.sHtML

------------------------------------
来源：http://www.share.epnwcf.com/Article/details/ggfhhjaxr.sHtML

合计 ........... 2106 条
来源：http://3g.yfazqb.com/Article/details/ggfdeuuqb.sHtML

按章节统计：
来源：http://m.share.fktsv.cn/Article/details/gzrhvafrj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.sjlbkw.cn/Article/details/gpoqypdai.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gtggjumxx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.epnwcf.com/Article/details/gkghamxhq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.tarul.cn/Article/details/gvyjkbbnx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.tarul.cn/Article/details/gftluqqxk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.epnwcf.com/Article/details/gmrjedqkq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.bbcook.cn/Article/details/getbsojvw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.bbcook.cn/Article/details/grjzxolub.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gsrxemrkb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.tarul.cn/Article/details/gznovffbe.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gadwrmcdk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/ggvxgqkpr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gakmuitwp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.vehdjk.com/Article/details/gqtzjmwek.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.bbcook.cn/Article/details/gaeuctbcm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fktsv.cn/Article/details/gguqkgicr.sHtML

Q SQL 专题                              90
来源：http://3g.epnwcf.com/Article/details/gdioyayjr.sHtML

R Bash 专题                             80
来源：http://blog.vehdjk.com/Article/details/ghmzuiisq.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fktsv.cn/Article/details/gfqgddoaw.sHtML

T 其他语言补充                          60
来源：http://www.share.bbcook.cn/Article/details/gvwlecekj.sHtML

U 高频实用片段                         120
来源：http://read.share.yfazqb.com/Article/details/guhvalyis.sHtML

------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gzxwosrse.sHtML

合计                                  2106 条
来源：http://3g.yfazqb.com/Article/details/gfvrcdxyw.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gndwkrdru.sHtML

使用提醒
来源：http://baike.bbcook.cn/Article/details/goywonhfy.sHtML

--------------------------------------------------------------------------------
来源：http://wap.vehdjk.com/Article/details/gurabyekt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.vehdjk.com/Article/details/gutqvxvru.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fktsv.cn/Article/details/gutnowyqe.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.yfazqb.com/Article/details/gphishqdd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.yfazqb.com/Article/details/glagtzuxb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.tarul.cn/Article/details/gpfzcbybr.sHtML

—— 文件结束 ——
来源：http://mobile.sjlbkw.cn/Article/details/gkkeomozd.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/giqxlwesg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.vehdjk.com/Article/details/gxvvpawxz.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.tarul.cn/Article/details/gwfusbxtq.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/glynjpbxd.sHtML

【收录内容】
来源：http://www.blog.fktsv.cn/Article/details/ggqeitpjq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.yfazqb.com/Article/details/gyrayozel.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.yfazqb.com/Article/details/gdjsalsjh.sHtML

SQL · Bash · C · C++
来源：http://m.share.vehdjk.com/Article/details/gqzjsmoon.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.sjlbkw.cn/Article/details/gavgayvhi.sHtML

【使用说明】
来源：http://blog.tarul.cn/Article/details/gzasheanc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.epnwcf.com/Article/details/gjvzppqlx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fktsv.cn/Article/details/gaxmzzqaq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.sjlbkw.cn/Article/details/gvxksvowv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.sjlbkw.cn/Article/details/gjrvexlha.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.vehdjk.com/Article/details/glmxhdmen.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.epnwcf.com/Article/details/gryqoqkha.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.tarul.cn/Article/details/gbvvnntiy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.epnwcf.com/Article/details/gycgzxqsm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.epnwcf.com/Article/details/giscicrtx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.sjlbkw.cn/Article/details/giixhgqsc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.sjlbkw.cn/Article/details/gbcylzmwj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.tarul.cn/Article/details/gppinrujk.sHtML

【文件统计】
来源：http://read.share.tarul.cn/Article/details/givxxxszd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.vehdjk.com/Article/details/gksjczrux.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.vehdjk.com/Article/details/ghspupuue.sHtML

目  录
来源：http://www.share.tarul.cn/Article/details/genkyslfh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gvwmkotrm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.epnwcf.com/Article/details/gwvsarjok.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gqoxbwhua.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.epnwcf.com/Article/details/gnqqgftdt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.bbcook.cn/Article/details/gcuqwckds.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.epnwcf.com/Article/details/gsxijmsel.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.bbcook.cn/Article/details/gnbplqtak.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fktsv.cn/Article/details/gatdvgxhb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.epnwcf.com/Article/details/gatklxeoo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/gugjwfxbj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.sjlbkw.cn/Article/details/gnwzcgcwd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gmsbkkpbv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/gwakxdnsa.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.bbcook.cn/Article/details/gtobfrbaj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.sjlbkw.cn/Article/details/guojsemdd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.tarul.cn/Article/details/gbdqmhnxj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.sjlbkw.cn/Article/details/gpautskuw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fktsv.cn/Article/details/gzofvrogs.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.epnwcf.com/Article/details/grhfqmcvi.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.vehdjk.com/Article/details/gziixppzr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fktsv.cn/Article/details/gkhdtsdjq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.sjlbkw.cn/Article/details/gmiufmzqq.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gfsrscccv.sHtML

A. 基础语法与类型
来源：http://read.share.tarul.cn/Article/details/gjywsujqz.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gogjpsxhc.sHtML

[A01] Hello World
来源：http://blog.epnwcf.com/Article/details/glcducjqm.sHtML

Py:   print("Hello, World!")
来源：http://m.share.epnwcf.com/Article/details/ggswvhjmm.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.bbcook.cn/Article/details/ggqawzsqy.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.sjlbkw.cn/Article/details/grxzzqrti.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fktsv.cn/Article/details/gykcvmtzg.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.yfazqb.com/Article/details/gizshsfls.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.bbcook.cn/Article/details/gqaazqcci.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.vehdjk.com/Article/details/gkisdsilf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.bbcook.cn/Article/details/gbwejefdx.sHtML

[A02] 变量声明与赋值
来源：http://mobile.yfazqb.com/Article/details/gdpozbinf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fktsv.cn/Article/details/gaxmnlgap.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.epnwcf.com/Article/details/gafggqdot.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.bbcook.cn/Article/details/gltrlxmhz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.vehdjk.com/Article/details/govnyygrx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.bbcook.cn/Article/details/glhtdxxfl.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.tarul.cn/Article/details/gwqjzfkek.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.sjlbkw.cn/Article/details/gdenwsqti.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fktsv.cn/Article/details/gfmhbovzq.sHtML

[A03] 常量定义
来源：http://blog.vehdjk.com/Article/details/gjcivirgl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.yfazqb.com/Article/details/gijlkypcc.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gctbjogxi.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gcrtxhwns.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gqyzvzwmf.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gjsllulgt.sHtML

Go:   const PI = 3.14159
来源：http://3g.epnwcf.com/Article/details/grkkrmgke.sHtML

Ruby: PI = 3.14159
来源：http://read.share.epnwcf.com/Article/details/gftoebwnc.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gemxkbkpx.sHtML

[A04] 判断变量类型
来源：http://baike.vehdjk.com/Article/details/gtckukfrk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fktsv.cn/Article/details/gamaqteqp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.sjlbkw.cn/Article/details/gmkafpepi.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fktsv.cn/Article/details/gxeexbttf.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.vehdjk.com/Article/details/goomfjwpr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.bbcook.cn/Article/details/gnnquztob.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.tarul.cn/Article/details/gjnylnrhm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.yfazqb.com/Article/details/gblrlpzps.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.yfazqb.com/Article/details/gpdqztxex.sHtML

[A05] 整数除法与取模
来源：http://blog.bbcook.cn/Article/details/giyxutfqg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.sjlbkw.cn/Article/details/gjjhmshhs.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fktsv.cn/Article/details/grofijzux.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/gckttvmis.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gmckcbwgf.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.bbcook.cn/Article/details/grrajmcpw.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fktsv.cn/Article/details/gmquywwbp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gcwozeygj.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gmhtlwuad.sHtML

[A06] 字符串转数字
来源：http://mobile.fktsv.cn/Article/details/ggxubbyaw.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.tarul.cn/Article/details/ggxsadhgb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.bbcook.cn/Article/details/gwwznvyts.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.tarul.cn/Article/details/gywtkyxur.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.yfazqb.com/Article/details/gajzhievh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.tarul.cn/Article/details/gqfxltohn.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.epnwcf.com/Article/details/gzzfrmsel.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.sjlbkw.cn/Article/details/giazazbbt.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.yfazqb.com/Article/details/gorgiayaj.sHtML

[A07] 数字转字符串
来源：http://www.share.yfazqb.com/Article/details/gqdqiuquj.sHtML

Py:   str(42)
来源：http://www.blog.epnwcf.com/Article/details/gohswaoub.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.yfazqb.com/Article/details/gsihhgioy.sHtML

JS:   String(42); (42).toString()
来源：http://3g.sjlbkw.cn/Article/details/girrlkknt.sHtML

TS:   String(42)
来源：http://read.share.bbcook.cn/Article/details/gctjanjmt.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.vehdjk.com/Article/details/grjheqzbp.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.vehdjk.com/Article/details/gfplbiulj.sHtML

Ruby: 42.to_s
来源：http://www.blog.fktsv.cn/Article/details/gsveikxft.sHtML

C#:   42.ToString()
来源：http://m.share.bbcook.cn/Article/details/gonfvailm.sHtML

[A08] 取整与四舍五入
来源：http://blog.sjlbkw.cn/Article/details/gbmllkoyo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fktsv.cn/Article/details/ghyoqcogh.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.bbcook.cn/Article/details/guzptjqmq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.bbcook.cn/Article/details/gelngjrxn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.bbcook.cn/Article/details/gtuepsrkq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.yfazqb.com/Article/details/gsldbmpeo.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.yfazqb.com/Article/details/ghohxcaww.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.sjlbkw.cn/Article/details/gakgmszjf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.yfazqb.com/Article/details/gerkdjjfq.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.fktsv.cn/Article/details/gxfemohlq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/ghsznvaua.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.yfazqb.com/Article/details/ghmksfjwq.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.vehdjk.com/Article/details/glfcxxghe.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.vehdjk.com/Article/details/gpvuqvtjr.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.vehdjk.com/Article/details/gchaundqs.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.bbcook.cn/Article/details/gscbnxuvz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.tarul.cn/Article/details/gdpcsajts.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/gmtfdbtmz.sHtML

[A10] 生成随机数
来源：http://baike.bbcook.cn/Article/details/gdokbzqbw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.bbcook.cn/Article/details/gawllsehl.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.yfazqb.com/Article/details/gartozmfl.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.bbcook.cn/Article/details/gxkdjuusw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fktsv.cn/Article/details/gzgyjciqi.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.sjlbkw.cn/Article/details/gonyuixcm.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.yfazqb.com/Article/details/gbmgcwxzu.sHtML

Ruby: rand(1..100)
来源：http://baike.epnwcf.com/Article/details/glthfvvxa.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.fktsv.cn/Article/details/gbkbfqzrb.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.yfazqb.com/Article/details/grursmjdf.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.bbcook.cn/Article/details/gdlzxewck.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.bbcook.cn/Article/details/gozsjegpn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.vehdjk.com/Article/details/gsvemkcdx.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gxizmxgou.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.epnwcf.com/Article/details/gliwjmiej.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.sjlbkw.cn/Article/details/gxzwptyoh.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.fktsv.cn/Article/details/gunwohgib.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.yfazqb.com/Article/details/gfdnbyjwa.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.vehdjk.com/Article/details/gmciinlqu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.tarul.cn/Article/details/gdtpwljvc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.tarul.cn/Article/details/gdlkogzhx.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.yfazqb.com/Article/details/gopkawedr.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.epnwcf.com/Article/details/gwkvispit.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.fktsv.cn/Article/details/giqxjpput.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.bbcook.cn/Article/details/gcbeapjdj.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.epnwcf.com/Article/details/gmhklqpfa.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.sjlbkw.cn/Article/details/gveznutab.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.bbcook.cn/Article/details/glvnwsehj.sHtML

Py:   "第一行\n第二行"
来源：http://3g.tarul.cn/Article/details/gkubpjrio.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/gdpiyqymt.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/gfansrlgn.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/gkeuohovh.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.sjlbkw.cn/Article/details/gpoiuwesv.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gnclhmscy.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/gdjqaidll.sHtML

C#:   "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/gfmtycfsz.sHtML

[A14] 注释写法
来源：http://wap.fktsv.cn/Article/details/gfsswzrai.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.tarul.cn/Article/details/gojmskukj.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/ggbntipqi.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.tarul.cn/Article/details/goaledvkb.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fktsv.cn/Article/details/gsipbrggv.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.fktsv.cn/Article/details/garokeimo.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.tarul.cn/Article/details/gmwjzoclk.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.tarul.cn/Article/details/gchrohsio.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.fktsv.cn/Article/details/gdxwtcklv.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.vehdjk.com/Article/details/gtkxadmqw.sHtML

Py:   value = data or "默认值"
来源：http://wap.bbcook.cn/Article/details/gjspofvff.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.vehdjk.com/Article/details/grwgydxvc.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.yfazqb.com/Article/details/ggkgcajfn.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.yfazqb.com/Article/details/gkwmltyiy.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.sjlbkw.cn/Article/details/ggzetnrra.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.bbcook.cn/Article/details/gfqsdafbq.sHtML

Ruby: value = data || "默认值"
来源：http://wap.sjlbkw.cn/Article/details/goffxbsnd.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.tarul.cn/Article/details/goccoeimc.sHtML

[A16] 真假值判断规则
来源：http://3g.tarul.cn/Article/details/gbguqmgit.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.bbcook.cn/Article/details/gytmcsffj.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.tarul.cn/Article/details/giqmzkuha.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.fktsv.cn/Article/details/gwablswed.sHtML

TS:   if (!x) {}
来源：http://wap.vehdjk.com/Article/details/gzmawnmew.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.bbcook.cn/Article/details/gznnolwtv.sHtML


<!-- 参考信息 -->