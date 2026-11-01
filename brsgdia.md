代发 wailian999

[U97] JS：并发请求
来源：http://wap.fktsv.cn/Article/details/gazmvrtyc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/gwbrtrnrg.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.epnwcf.com/Article/details/gakovrgzy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.vehdjk.com/Article/details/gsgnvevkv.sHtML

[U99] JS：事件监听
来源：http://blog.sjlbkw.cn/Article/details/geuombkzw.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.tarul.cn/Article/details/gzlmjqyst.sHtML

[U100] JS：DOM 查询
来源：http://read.share.vehdjk.com/Article/details/gdlrfcyrh.sHtML

document.querySelector(".item")
来源：http://wap.fktsv.cn/Article/details/gevnzrmfr.sHtML

[U101] JS：classList 操作
来源：http://blog.vehdjk.com/Article/details/gzktdvyvr.sHtML

el.classList.toggle("active")
来源：http://baike.sjlbkw.cn/Article/details/gascpddgk.sHtML

[U102] JS：本地存储
来源：http://www.share.sjlbkw.cn/Article/details/gcjzmajdm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.bbcook.cn/Article/details/ggoczkfdf.sHtML

[U103] JS：定时器
来源：http://blog.sjlbkw.cn/Article/details/gpcazgqew.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.sjlbkw.cn/Article/details/glevpifdr.sHtML

[U104] JS：防抖
来源：http://www.m.share.yfazqb.com/Article/details/gncenvado.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/guiikfkuq.sHtML

[U105] JS：节流
来源：http://m.share.epnwcf.com/Article/details/gvowoymaj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.tarul.cn/Article/details/glhrmrdbm.sHtML

[U106] JS：日期格式化
来源：http://blog.vehdjk.com/Article/details/gtriajjxo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.vehdjk.com/Article/details/gyudflmyb.sHtML

[U107] JS：数字千分位
来源：http://read.share.sjlbkw.cn/Article/details/gumlaitrl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.epnwcf.com/Article/details/gtbwrbjcm.sHtML

[U108] JS：随机整数
来源：http://read.share.tarul.cn/Article/details/gonvdltnc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.vehdjk.com/Article/details/gniitkrly.sHtML

[U109] JS：数组分组
来源：http://3g.yfazqb.com/Article/details/gxjyljyjp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.sjlbkw.cn/Article/details/gpxdwewhd.sHtML

[U110] JS：数组分块
来源：http://read.share.epnwcf.com/Article/details/gsixtseis.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.vehdjk.com/Article/details/gttypbdos.sHtML

[U111] JS：对象转 Map
来源：http://www.share.yfazqb.com/Article/details/gsdirzhmu.sHtML

new Map(Object.entries(obj))
来源：http://m.share.tarul.cn/Article/details/gwpxvsnpz.sHtML

[U112] JS：字符串补位
来源：http://wap.sjlbkw.cn/Article/details/grzznmnjd.sHtML

"7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gixvgxiif.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.bbcook.cn/Article/details/gfhyjfeml.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gngnlcmfa.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.sjlbkw.cn/Article/details/gssiqfgwi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fktsv.cn/Article/details/gatmljizs.sHtML

[U115] JS：生成 UUID
来源：http://blog.tarul.cn/Article/details/gabqgkwdt.sHtML

crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gqphfutxq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.sjlbkw.cn/Article/details/gaypcctqv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.sjlbkw.cn/Article/details/gurnnfmbv.sHtML

[U117] JS：单元测试
来源：http://read.share.yfazqb.com/Article/details/gkpgdoqzl.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.tarul.cn/Article/details/gvfftsvjg.sHtML

[U118] JS：开发服务器
来源：http://baike.vehdjk.com/Article/details/gxruubvfa.sHtML

npm i -D vite;  npx vite
来源：http://www.share.bbcook.cn/Article/details/gahzzrbya.sHtML

[U119] JS：生产构建
来源：http://www.m.share.tarul.cn/Article/details/gypmavltz.sHtML

npx vite build
来源：http://m.share.fktsv.cn/Article/details/gsfcwxdmg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fktsv.cn/Article/details/gkasplept.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fktsv.cn/Article/details/gkoudiccl.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gszjksikz.sHtML

统计汇总
来源：http://www.share.fktsv.cn/Article/details/gvihroxav.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gocpgnsvb.sHtML

按语言统计（条）：
来源：http://read.share.sjlbkw.cn/Article/details/gbcltovhf.sHtML

Python ......... 252
来源：http://blog.yfazqb.com/Article/details/gvbzbxhxn.sHtML

PHP ............ 252
来源：http://www.share.sjlbkw.cn/Article/details/gffbsyuuu.sHtML

JavaScript ..... 252
来源：http://3g.fktsv.cn/Article/details/gkpfweloz.sHtML

TypeScript ..... 212
来源：http://mobile.tarul.cn/Article/details/grjlfxtyp.sHtML

Java ........... 212
来源：http://baike.tarul.cn/Article/details/ghiswsidc.sHtML

Go ............. 212
来源：http://3g.yfazqb.com/Article/details/goraxkday.sHtML

Ruby ........... 212
来源：http://3g.sjlbkw.cn/Article/details/gmxosqcds.sHtML

C# ............. 212
来源：http://baike.sjlbkw.cn/Article/details/ghiojmdvi.sHtML

C .............. 30
来源：http://m.share.fktsv.cn/Article/details/ggckjtadc.sHtML

C++ ............ 30
来源：http://m.share.sjlbkw.cn/Article/details/gvylsznsn.sHtML

SQL ............ 90
来源：http://baike.sjlbkw.cn/Article/details/gzsxvobje.sHtML

Bash ........... 80
来源：http://www.share.fktsv.cn/Article/details/gxerdzybq.sHtML

Kotlin ......... 15
来源：http://m.share.fktsv.cn/Article/details/gbtjiarkq.sHtML

Swift .......... 15
来源：http://blog.epnwcf.com/Article/details/gcpimcxbs.sHtML

Lua ............ 10
来源：http://baike.epnwcf.com/Article/details/gamkfvuhq.sHtML

Perl ........... 10
来源：http://www.blog.yfazqb.com/Article/details/gngoowiue.sHtML

Scala .......... 10
来源：http://www.blog.fktsv.cn/Article/details/ggebzupxo.sHtML

------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxbffsau.sHtML

合计 ........... 2106 条
来源：http://mobile.bbcook.cn/Article/details/gxhqurveh.sHtML

按章节统计：
来源：http://blog.tarul.cn/Article/details/gtrnjyzom.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.tarul.cn/Article/details/goeotrzuf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.tarul.cn/Article/details/gczkbtrqq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.vehdjk.com/Article/details/gadtbcbsw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.sjlbkw.cn/Article/details/gzoqsdqth.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.bbcook.cn/Article/details/gqrtqqomw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.yfazqb.com/Article/details/gujohnxvx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.sjlbkw.cn/Article/details/giidiouyq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.sjlbkw.cn/Article/details/gmfkglygp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/ggazppwvz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.tarul.cn/Article/details/gyxkyrrgj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/ghsoqjiao.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gpbqhqwth.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gybjxucad.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.yfazqb.com/Article/details/gyhrxayfd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.epnwcf.com/Article/details/gldcqmnot.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gfdhppzbk.sHtML

Q SQL 专题                              90
来源：http://www.blog.bbcook.cn/Article/details/gwrfoylio.sHtML

R Bash 专题                             80
来源：http://3g.vehdjk.com/Article/details/gdcsywhjv.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.yfazqb.com/Article/details/gmgfclnhs.sHtML

T 其他语言补充                          60
来源：http://baike.tarul.cn/Article/details/ggobsputp.sHtML

U 高频实用片段                         120
来源：http://www.blog.sjlbkw.cn/Article/details/goimsigac.sHtML

------------------------------------
来源：http://www.share.bbcook.cn/Article/details/ghbxhitrv.sHtML

合计                                  2106 条
来源：http://mobile.tarul.cn/Article/details/goaemkbxr.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/gknejbwbg.sHtML

使用提醒
来源：http://baike.bbcook.cn/Article/details/gqikrkyhr.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gqyuhtewv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.tarul.cn/Article/details/goxsoshjd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.yfazqb.com/Article/details/gjgbjlyqy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.yfazqb.com/Article/details/gzwwuaafe.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.sjlbkw.cn/Article/details/gwbqdoaun.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.epnwcf.com/Article/details/gmwfqsecg.sHtML

—— 文件结束 ——
来源：http://blog.fktsv.cn/Article/details/gtxynedka.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gvrrnoxka.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.epnwcf.com/Article/details/gvqgimazb.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.yfazqb.com/Article/details/gcshqjtpq.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gvielovcq.sHtML

【收录内容】
来源：http://m.share.yfazqb.com/Article/details/glxizblqn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.vehdjk.com/Article/details/gjfnqltpp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.yfazqb.com/Article/details/gaursxxkm.sHtML

SQL · Bash · C · C++
来源：http://www.blog.bbcook.cn/Article/details/grmbpmxpv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.bbcook.cn/Article/details/gmfhrhegq.sHtML

【使用说明】
来源：http://wap.yfazqb.com/Article/details/giqwrqrsz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fktsv.cn/Article/details/gdwjshxrk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.vehdjk.com/Article/details/gcpegzrlt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fktsv.cn/Article/details/gdrbjpaba.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.epnwcf.com/Article/details/gnyfvfyfr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.epnwcf.com/Article/details/gjgsymgny.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.yfazqb.com/Article/details/gahguvgvq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.epnwcf.com/Article/details/gxjujuvnl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fktsv.cn/Article/details/gtgntfcqm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.vehdjk.com/Article/details/gdwcsfcfs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.vehdjk.com/Article/details/gffwmwsul.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.sjlbkw.cn/Article/details/gdgrggqgf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.vehdjk.com/Article/details/geywlgjoc.sHtML

【文件统计】
来源：http://www.blog.epnwcf.com/Article/details/grvcoyptz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.bbcook.cn/Article/details/gyimvinyr.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gtldwqizr.sHtML

目  录
来源：http://baike.yfazqb.com/Article/details/gmilsuiem.sHtML

--------------------------------------------------------------------------------
来源：http://3g.yfazqb.com/Article/details/gsjpoxszr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.yfazqb.com/Article/details/guwbcajxd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.bbcook.cn/Article/details/gxcociube.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.bbcook.cn/Article/details/gjxalfjfm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.tarul.cn/Article/details/gegpnovci.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.vehdjk.com/Article/details/gbszowcfi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.tarul.cn/Article/details/gzehxmnaa.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.yfazqb.com/Article/details/gznnnyqgz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.tarul.cn/Article/details/gjnlsfdle.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/gtkdshnbq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.bbcook.cn/Article/details/glvyqnctv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.tarul.cn/Article/details/gwtxqvdyx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/gvktpejty.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.vehdjk.com/Article/details/gxbdqpoll.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.epnwcf.com/Article/details/gdevqarvw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.sjlbkw.cn/Article/details/gfsbafjrb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fktsv.cn/Article/details/gkwywreln.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.yfazqb.com/Article/details/gotkzyhhb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.tarul.cn/Article/details/gerfklczd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.yfazqb.com/Article/details/grlgsyeor.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.tarul.cn/Article/details/gbdhwiduj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.vehdjk.com/Article/details/ghguxhevn.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gohpxqtoa.sHtML

A. 基础语法与类型
来源：http://baike.vehdjk.com/Article/details/gmagnplts.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gqmxhfsnp.sHtML

[A01] Hello World
来源：http://blog.yfazqb.com/Article/details/gdrymihrq.sHtML

Py:   print("Hello, World!")
来源：http://www.share.tarul.cn/Article/details/gpgcnrhzb.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.bbcook.cn/Article/details/geqcflqum.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.sjlbkw.cn/Article/details/gsqtvsvoj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.tarul.cn/Article/details/gszbthblc.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.yfazqb.com/Article/details/goieihdjn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.sjlbkw.cn/Article/details/ggkhhkeqt.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.bbcook.cn/Article/details/gzrewbvus.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.sjlbkw.cn/Article/details/gzlspnovu.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.epnwcf.com/Article/details/gjrniyagg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fktsv.cn/Article/details/gvobtvlph.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.bbcook.cn/Article/details/gapalrbvk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fktsv.cn/Article/details/gyywgmyip.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.yfazqb.com/Article/details/guzwwtxce.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/gaavoldfl.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.bbcook.cn/Article/details/ginxgyero.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.sjlbkw.cn/Article/details/gqghiexvs.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.sjlbkw.cn/Article/details/glwvmsryg.sHtML

[A03] 常量定义
来源：http://m.share.yfazqb.com/Article/details/glbzvkkdj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fktsv.cn/Article/details/gpohpgmce.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gjttfjkax.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gmoywsxnw.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gkkyuqfme.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gbuauhmcm.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fktsv.cn/Article/details/gympzowtw.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.yfazqb.com/Article/details/gcunbfztk.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gnlshwujl.sHtML

[A04] 判断变量类型
来源：http://wap.fktsv.cn/Article/details/gumckimys.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.yfazqb.com/Article/details/ggoqjxgpy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.bbcook.cn/Article/details/gmgxwfkkn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.sjlbkw.cn/Article/details/gvdkdvbab.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.yfazqb.com/Article/details/gktpidjxn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fktsv.cn/Article/details/gfactbkyk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.yfazqb.com/Article/details/gzavnwlnx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.sjlbkw.cn/Article/details/gmgxptaga.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.yfazqb.com/Article/details/gcmvchkmj.sHtML

[A05] 整数除法与取模
来源：http://m.share.fktsv.cn/Article/details/gogmvdyqb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fktsv.cn/Article/details/gikckvfgv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.vehdjk.com/Article/details/gcpflxtjz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.yfazqb.com/Article/details/gedurgpkg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/gnuammsav.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.tarul.cn/Article/details/gbftcgecl.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gdygvkgnb.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fktsv.cn/Article/details/gntobdifp.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.vehdjk.com/Article/details/gmofuowby.sHtML

[A06] 字符串转数字
来源：http://read.share.tarul.cn/Article/details/gxbnrptha.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.yfazqb.com/Article/details/gnpkkxrvl.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.vehdjk.com/Article/details/gldyyvajy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.bbcook.cn/Article/details/gnucdxhmz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.bbcook.cn/Article/details/gwuvabtmg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fktsv.cn/Article/details/gyucholoo.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.epnwcf.com/Article/details/grjbjdktw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.tarul.cn/Article/details/geaamhsnv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fktsv.cn/Article/details/gshynreao.sHtML

[A07] 数字转字符串
来源：http://mobile.vehdjk.com/Article/details/guyfmetvc.sHtML

Py:   str(42)
来源：http://blog.fktsv.cn/Article/details/gxkdumvqh.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.bbcook.cn/Article/details/ghqgadswq.sHtML

JS:   String(42); (42).toString()
来源：http://blog.vehdjk.com/Article/details/gvwgxhqak.sHtML

TS:   String(42)
来源：http://read.share.epnwcf.com/Article/details/guiqlubvk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.vehdjk.com/Article/details/giombvxsv.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.tarul.cn/Article/details/gfqxjxqmo.sHtML

Ruby: 42.to_s
来源：http://mobile.epnwcf.com/Article/details/gagrenaiw.sHtML

C#:   42.ToString()
来源：http://3g.vehdjk.com/Article/details/gbjihcecx.sHtML

[A08] 取整与四舍五入
来源：http://m.share.epnwcf.com/Article/details/gnpcpmqsa.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.yfazqb.com/Article/details/gbodxqedf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.vehdjk.com/Article/details/gtlntnufc.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.yfazqb.com/Article/details/ghxagraca.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.vehdjk.com/Article/details/gkmkngxoa.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.sjlbkw.cn/Article/details/gdimepqhq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.epnwcf.com/Article/details/ggelgceqy.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.yfazqb.com/Article/details/gtddoqren.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.bbcook.cn/Article/details/gzhsclvqy.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.tarul.cn/Article/details/gjicazxjr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gbknjfiix.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gwpmfqhde.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.tarul.cn/Article/details/gedboecdt.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.epnwcf.com/Article/details/guifhohfd.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.tarul.cn/Article/details/gftndxyfz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.vehdjk.com/Article/details/gneemeaav.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.sjlbkw.cn/Article/details/gstaegvys.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.tarul.cn/Article/details/gtesogvpu.sHtML

[A10] 生成随机数
来源：http://www.share.fktsv.cn/Article/details/gqbijhbfl.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.yfazqb.com/Article/details/gylbehlzx.sHtML

PHP:  random_int(1, 100);
来源：http://wap.bbcook.cn/Article/details/gcsikffjl.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.tarul.cn/Article/details/gysoebpmn.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.vehdjk.com/Article/details/glrefjslk.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.sjlbkw.cn/Article/details/gcfrojzet.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.fktsv.cn/Article/details/gshgpoiin.sHtML

Ruby: rand(1..100)
来源：http://wap.epnwcf.com/Article/details/gsonszkjf.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.bbcook.cn/Article/details/gkmulpidw.sHtML

[A11] 条件表达式（三元）
来源：http://blog.sjlbkw.cn/Article/details/gkhzotmhw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.tarul.cn/Article/details/ggksjzfur.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.tarul.cn/Article/details/gnyoyqubq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/geoojlqkj.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.vehdjk.com/Article/details/gxmvjblmj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.tarul.cn/Article/details/gcvisvvyi.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.yfazqb.com/Article/details/gzxhrpowp.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.epnwcf.com/Article/details/gxdhulucg.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.bbcook.cn/Article/details/gyjwxmddp.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.bbcook.cn/Article/details/gpplvjmcx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.sjlbkw.cn/Article/details/gkgcorntv.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.bbcook.cn/Article/details/goctjeuld.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.yfazqb.com/Article/details/gtiajitvq.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.bbcook.cn/Article/details/gntyzmxnj.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.tarul.cn/Article/details/grvpopqhk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.fktsv.cn/Article/details/gbhfufbnt.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.tarul.cn/Article/details/ghjhbjlrm.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.sjlbkw.cn/Article/details/gpodhkxlj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.tarul.cn/Article/details/gikptnkpu.sHtML

Py:   "第一行\n第二行"
来源：http://wap.vehdjk.com/Article/details/gpupzrcqe.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/guucttgea.sHtML

JS:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/ghwzbynat.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gmkxodzuf.sHtML

Java: "第一行\n第二行"
来源：http://www.share.vehdjk.com/Article/details/gzotpmqca.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/gdoxfntjv.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/gtxagrgku.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/gsiknllbo.sHtML

[A14] 注释写法
来源：http://www.m.share.vehdjk.com/Article/details/gazofjmjs.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.yfazqb.com/Article/details/gscjopdlj.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.vehdjk.com/Article/details/gwywfxthx.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/gzsexaoig.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.vehdjk.com/Article/details/glionihgc.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.fktsv.cn/Article/details/gucdhnnyx.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.yfazqb.com/Article/details/gwjmgqncc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.bbcook.cn/Article/details/gemurcbvb.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.tarul.cn/Article/details/gyomjjfcp.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.vehdjk.com/Article/details/gxqgkipui.sHtML

Py:   value = data or "默认值"
来源：http://www.share.bbcook.cn/Article/details/gajqumcza.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.vehdjk.com/Article/details/geqeohwhz.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.tarul.cn/Article/details/gpxedipho.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.yfazqb.com/Article/details/gkxunxjqh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.tarul.cn/Article/details/gglahffsq.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.epnwcf.com/Article/details/gzhbevwgf.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.fktsv.cn/Article/details/gizahgavd.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.bbcook.cn/Article/details/gvyyrgwyi.sHtML

[A16] 真假值判断规则
来源：http://m.share.vehdjk.com/Article/details/gdlgtjjjc.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.tarul.cn/Article/details/gqywyjemf.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.fktsv.cn/Article/details/gidmfgpcq.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.yfazqb.com/Article/details/gxsontqqt.sHtML

TS:   if (!x) {}
来源：http://read.share.yfazqb.com/Article/details/gkovwzquk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.vehdjk.com/Article/details/giwfufqsf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.bbcook.cn/Article/details/gafbxapiw.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.epnwcf.com/Article/details/guwjzyobp.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.vehdjk.com/Article/details/ggqvimhjw.sHtML

[A17] 位运算
来源：http://www.m.share.fktsv.cn/Article/details/gtotjprko.sHtML


<!-- 参考信息 -->