代发 wailian999

[U97] JS：并发请求
来源：http://baike.vehdjk.com/Article/details/gnphkbyjq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/gtugjgrvi.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.yfazqb.com/Article/details/gmrzmvbnc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gpblcleaz.sHtML

[U99] JS：事件监听
来源：http://www.share.yfazqb.com/Article/details/gtxvrkccy.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fktsv.cn/Article/details/garmtoavf.sHtML

[U100] JS：DOM 查询
来源：http://www.share.sjlbkw.cn/Article/details/gricpzole.sHtML

document.querySelector(".item")
来源：http://read.share.fktsv.cn/Article/details/gkemwnejp.sHtML

[U101] JS：classList 操作
来源：http://www.share.sjlbkw.cn/Article/details/gmlmyayhz.sHtML

el.classList.toggle("active")
来源：http://read.share.bbcook.cn/Article/details/gtvjwqzci.sHtML

[U102] JS：本地存储
来源：http://m.share.vehdjk.com/Article/details/gzsnivhqv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.vehdjk.com/Article/details/gdhpbeabj.sHtML

[U103] JS：定时器
来源：http://wap.bbcook.cn/Article/details/gsvxhbiru.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.vehdjk.com/Article/details/guijhkfmm.sHtML

[U104] JS：防抖
来源：http://www.share.tarul.cn/Article/details/galerxuhm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/gftryyoqm.sHtML

[U105] JS：节流
来源：http://www.m.share.vehdjk.com/Article/details/ghafxuidw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.bbcook.cn/Article/details/gdkqbnslx.sHtML

[U106] JS：日期格式化
来源：http://baike.fktsv.cn/Article/details/gkolplqga.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fktsv.cn/Article/details/gqzlpvoah.sHtML

[U107] JS：数字千分位
来源：http://baike.epnwcf.com/Article/details/gvsahftnm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.yfazqb.com/Article/details/gfbrmoqpf.sHtML

[U108] JS：随机整数
来源：http://mobile.vehdjk.com/Article/details/ggewbbtbt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.yfazqb.com/Article/details/gxmyjzcam.sHtML

[U109] JS：数组分组
来源：http://m.share.sjlbkw.cn/Article/details/gelccsyyn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fktsv.cn/Article/details/ganstfdvs.sHtML

[U110] JS：数组分块
来源：http://wap.fktsv.cn/Article/details/gkcikonqc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.yfazqb.com/Article/details/gtgesuafb.sHtML

[U111] JS：对象转 Map
来源：http://wap.fktsv.cn/Article/details/gawgauzcc.sHtML

new Map(Object.entries(obj))
来源：http://wap.yfazqb.com/Article/details/glwgvbpac.sHtML

[U112] JS：字符串补位
来源：http://www.blog.epnwcf.com/Article/details/gxfdqnvbs.sHtML

"7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gpkfgteuu.sHtML

[U113] JS：正则替换全部
来源：http://mobile.sjlbkw.cn/Article/details/gxycnxnvu.sHtML

s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gnhrqrcdo.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpvpiqfw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.tarul.cn/Article/details/gapennzat.sHtML

[U115] JS：生成 UUID
来源：http://wap.epnwcf.com/Article/details/ggkubcjuc.sHtML

crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gzkqkzjpc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.bbcook.cn/Article/details/gedmcczbd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.sjlbkw.cn/Article/details/gjadgyyhg.sHtML

[U117] JS：单元测试
来源：http://3g.yfazqb.com/Article/details/geufniiaz.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.vehdjk.com/Article/details/gxzcmqxgl.sHtML

[U118] JS：开发服务器
来源：http://www.share.bbcook.cn/Article/details/grfbztgrj.sHtML

npm i -D vite;  npx vite
来源：http://blog.vehdjk.com/Article/details/gwkblklwa.sHtML

[U119] JS：生产构建
来源：http://mobile.epnwcf.com/Article/details/grtxnxwmb.sHtML

npx vite build
来源：http://read.share.bbcook.cn/Article/details/gntoltfza.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fktsv.cn/Article/details/ggclyijtf.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjhpdwya.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ggqwtdxxm.sHtML

统计汇总
来源：http://www.m.share.epnwcf.com/Article/details/gtaqaapxi.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/ghxxvvjzn.sHtML

按语言统计（条）：
来源：http://m.share.sjlbkw.cn/Article/details/gtoyaygkf.sHtML

Python ......... 252
来源：http://wap.vehdjk.com/Article/details/gpxtjffvc.sHtML

PHP ............ 252
来源：http://3g.tarul.cn/Article/details/gabcdmzfd.sHtML

JavaScript ..... 252
来源：http://blog.tarul.cn/Article/details/gpqzhwibw.sHtML

TypeScript ..... 212
来源：http://wap.vehdjk.com/Article/details/gisgghdgm.sHtML

Java ........... 212
来源：http://read.share.bbcook.cn/Article/details/gzzcengfc.sHtML

Go ............. 212
来源：http://www.m.share.sjlbkw.cn/Article/details/griimwlax.sHtML

Ruby ........... 212
来源：http://3g.fktsv.cn/Article/details/gmckwpvho.sHtML

C# ............. 212
来源：http://www.m.share.fktsv.cn/Article/details/gwjhngjlt.sHtML

C .............. 30
来源：http://www.m.share.tarul.cn/Article/details/gqbmcyeys.sHtML

C++ ............ 30
来源：http://blog.epnwcf.com/Article/details/gsgvaiuik.sHtML

SQL ............ 90
来源：http://mobile.tarul.cn/Article/details/gmnveqqhz.sHtML

Bash ........... 80
来源：http://baike.bbcook.cn/Article/details/gyweawbud.sHtML

Kotlin ......... 15
来源：http://mobile.sjlbkw.cn/Article/details/gssdmweiv.sHtML

Swift .......... 15
来源：http://www.blog.yfazqb.com/Article/details/ggjvotjki.sHtML

Lua ............ 10
来源：http://www.share.sjlbkw.cn/Article/details/gcgcpycvg.sHtML

Perl ........... 10
来源：http://mobile.bbcook.cn/Article/details/gydawtqqx.sHtML

Scala .......... 10
来源：http://m.share.bbcook.cn/Article/details/gjjvjdjyq.sHtML

------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gietyuilj.sHtML

合计 ........... 2106 条
来源：http://baike.fktsv.cn/Article/details/gewnkcfui.sHtML

按章节统计：
来源：http://www.blog.tarul.cn/Article/details/gcicygzhv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fktsv.cn/Article/details/gvsxjkufj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.vehdjk.com/Article/details/gdwqukzxn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.tarul.cn/Article/details/gburijoua.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.tarul.cn/Article/details/gtkwwnyor.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.bbcook.cn/Article/details/gdhmrhksv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fktsv.cn/Article/details/gqwqrlrzo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fktsv.cn/Article/details/ggepoydrh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fktsv.cn/Article/details/gprclcmgb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gxmhvpicm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.sjlbkw.cn/Article/details/gimievhvr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/gvdqmsycd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/gymzquccw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gplqgwkvc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.bbcook.cn/Article/details/gxfwktnuq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.epnwcf.com/Article/details/govfivfdh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gcrjxppyo.sHtML

Q SQL 专题                              90
来源：http://blog.bbcook.cn/Article/details/gieaoxeoq.sHtML

R Bash 专题                             80
来源：http://www.blog.bbcook.cn/Article/details/gsgjeptpf.sHtML

S C / C++ 专题                          60
来源：http://m.share.yfazqb.com/Article/details/gkatnvotb.sHtML

T 其他语言补充                          60
来源：http://www.m.share.sjlbkw.cn/Article/details/gawjckmlj.sHtML

U 高频实用片段                         120
来源：http://baike.tarul.cn/Article/details/gjyyrgfjn.sHtML

------------------------------------
来源：http://baike.epnwcf.com/Article/details/gpgscboai.sHtML

合计                                  2106 条
来源：http://m.share.yfazqb.com/Article/details/gdtpioneg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.bbcook.cn/Article/details/gwbqkguxd.sHtML

使用提醒
来源：http://baike.epnwcf.com/Article/details/gfjfydihp.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gexfvfqwy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.vehdjk.com/Article/details/gbljpbcpt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.epnwcf.com/Article/details/gbdmzgoww.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.tarul.cn/Article/details/glxntjdfp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.yfazqb.com/Article/details/ghocnfgrk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.epnwcf.com/Article/details/goygpccha.sHtML

—— 文件结束 ——
来源：http://read.share.sjlbkw.cn/Article/details/gwktfvdwx.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gvavyniwl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.tarul.cn/Article/details/gmomcrkgh.sHtML

Common Programming Examples Cheat Book
来源：http://baike.vehdjk.com/Article/details/gwuiwghkv.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/grubnfiqn.sHtML

【收录内容】
来源：http://wap.vehdjk.com/Article/details/gmecwdwwm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fktsv.cn/Article/details/gzeslljzu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.bbcook.cn/Article/details/gpssrzodc.sHtML

SQL · Bash · C · C++
来源：http://m.share.vehdjk.com/Article/details/gwdzuqfne.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fktsv.cn/Article/details/gkkfcgrxv.sHtML

【使用说明】
来源：http://mobile.bbcook.cn/Article/details/gacbyomxu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.yfazqb.com/Article/details/gpdbhdthe.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.bbcook.cn/Article/details/gqsfyqlqr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.yfazqb.com/Article/details/ghvmglvcc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.yfazqb.com/Article/details/gyqzzfzhl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fktsv.cn/Article/details/gtzwkiyiz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.yfazqb.com/Article/details/gjjqleucm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.sjlbkw.cn/Article/details/ginwuvrzb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.vehdjk.com/Article/details/gaqjgvxck.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fktsv.cn/Article/details/gnoqtgtgc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.tarul.cn/Article/details/glyacqten.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.epnwcf.com/Article/details/gkfbqrsny.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fktsv.cn/Article/details/gruepxxtn.sHtML

【文件统计】
来源：http://read.share.epnwcf.com/Article/details/gnsxamvcs.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.tarul.cn/Article/details/gzkavettn.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gezowacad.sHtML

目  录
来源：http://mobile.bbcook.cn/Article/details/gedbellxr.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fktsv.cn/Article/details/gbkyeoacv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.bbcook.cn/Article/details/gjaeijfhh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.vehdjk.com/Article/details/gvvvkzzrj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.vehdjk.com/Article/details/gktjoxyyd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.sjlbkw.cn/Article/details/gncvsylhv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.tarul.cn/Article/details/gyrlmthmw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.epnwcf.com/Article/details/genbqrugm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.yfazqb.com/Article/details/gwhkpvkgn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.sjlbkw.cn/Article/details/gpkrgjzlo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.tarul.cn/Article/details/gsotreksn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.yfazqb.com/Article/details/gzsdgvscy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gvpqnxhum.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/gxmarmfck.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/gktpusuor.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.yfazqb.com/Article/details/gawnmtirz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.yfazqb.com/Article/details/gxzyctrtr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.vehdjk.com/Article/details/gttklesfn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.bbcook.cn/Article/details/guiiharhk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.sjlbkw.cn/Article/details/gpmgyfsll.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fktsv.cn/Article/details/giglgrgqr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.tarul.cn/Article/details/gosniqlyn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.vehdjk.com/Article/details/gcnrnssav.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gvwwjdebg.sHtML

A. 基础语法与类型
来源：http://blog.vehdjk.com/Article/details/grfksxbsj.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gearmtzda.sHtML

[A01] Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gnduefdgx.sHtML

Py:   print("Hello, World!")
来源：http://read.share.bbcook.cn/Article/details/ghbottsxd.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.epnwcf.com/Article/details/ghetukvvj.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.epnwcf.com/Article/details/ggfbriuzh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.bbcook.cn/Article/details/gucfrsytt.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fktsv.cn/Article/details/gcniirfwn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.yfazqb.com/Article/details/gcbayiufh.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.vehdjk.com/Article/details/gvdzzmynb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fktsv.cn/Article/details/gyrhawulp.sHtML

[A02] 变量声明与赋值
来源：http://blog.fktsv.cn/Article/details/gsqxanpki.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.tarul.cn/Article/details/gjemfbpge.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsegmtzqa.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fktsv.cn/Article/details/grruppllj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.sjlbkw.cn/Article/details/gggqnmznc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fktsv.cn/Article/details/gdtbeuxeb.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.yfazqb.com/Article/details/gbnnhgpwf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.vehdjk.com/Article/details/gcaqhggqz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.epnwcf.com/Article/details/gaaqjwvhg.sHtML

[A03] 常量定义
来源：http://www.share.vehdjk.com/Article/details/gbdbvoovd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.epnwcf.com/Article/details/glnredprj.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gboduvoiw.sHtML

JS:   const PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gjnwhiena.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.tarul.cn/Article/details/gsayyljet.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/geowesofe.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.vehdjk.com/Article/details/gcubzwsqy.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fktsv.cn/Article/details/gzfvzqrzh.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gtnpmfnsy.sHtML

[A04] 判断变量类型
来源：http://mobile.epnwcf.com/Article/details/gchiatnqg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.yfazqb.com/Article/details/gxetbyxud.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.tarul.cn/Article/details/gszlctcbk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.vehdjk.com/Article/details/gxkhjyrcr.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.bbcook.cn/Article/details/glhosltpb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.yfazqb.com/Article/details/gzlfpwdgf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.tarul.cn/Article/details/gjgzpohab.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.sjlbkw.cn/Article/details/goxykoxxe.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.yfazqb.com/Article/details/gkmsqrqtb.sHtML

[A05] 整数除法与取模
来源：http://3g.tarul.cn/Article/details/glvzsjhxn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.bbcook.cn/Article/details/glkvriwfn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.epnwcf.com/Article/details/gliabeoik.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.vehdjk.com/Article/details/gmcedcoek.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.bbcook.cn/Article/details/gsodfhoic.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.bbcook.cn/Article/details/gazosnhex.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.bbcook.cn/Article/details/gnzpzqzaq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.sjlbkw.cn/Article/details/gtlwjxlry.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.bbcook.cn/Article/details/gjudywluv.sHtML

[A06] 字符串转数字
来源：http://blog.vehdjk.com/Article/details/gzmeqnrai.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.tarul.cn/Article/details/ggjkjxisk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fktsv.cn/Article/details/gjpjnjbcm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.epnwcf.com/Article/details/gwpdyrlal.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fktsv.cn/Article/details/gjajatfsc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fktsv.cn/Article/details/gubymjgze.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.fktsv.cn/Article/details/gzwibjpgb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.bbcook.cn/Article/details/gsymsyxcl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.yfazqb.com/Article/details/gadjkfkwn.sHtML

[A07] 数字转字符串
来源：http://baike.epnwcf.com/Article/details/ggnsrjfrx.sHtML

Py:   str(42)
来源：http://www.m.share.sjlbkw.cn/Article/details/glgqbyhez.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fktsv.cn/Article/details/gotvobzcg.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.epnwcf.com/Article/details/gtkzcvqif.sHtML

TS:   String(42)
来源：http://mobile.tarul.cn/Article/details/gogukyeux.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.sjlbkw.cn/Article/details/ggyilpeke.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.tarul.cn/Article/details/ghcharbhg.sHtML

Ruby: 42.to_s
来源：http://3g.sjlbkw.cn/Article/details/ghakqjacv.sHtML

C#:   42.ToString()
来源：http://blog.epnwcf.com/Article/details/govvnxigb.sHtML

[A08] 取整与四舍五入
来源：http://mobile.bbcook.cn/Article/details/gdxjapmnb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.bbcook.cn/Article/details/gefradtte.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.epnwcf.com/Article/details/gzcojxscd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fktsv.cn/Article/details/gyglikmsd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.epnwcf.com/Article/details/gdzhahcwe.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.yfazqb.com/Article/details/gnkgsfmpf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.vehdjk.com/Article/details/gbgezghcf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.epnwcf.com/Article/details/gesonhbmy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.tarul.cn/Article/details/giwbhgvjv.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.yfazqb.com/Article/details/giwlowrsr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.yfazqb.com/Article/details/grflummok.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fktsv.cn/Article/details/gonnrjfxr.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gsztlyyve.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.tarul.cn/Article/details/gwoqkfovl.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.tarul.cn/Article/details/ganmvuytp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.vehdjk.com/Article/details/grdftedvu.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.epnwcf.com/Article/details/gpbxsgirz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.tarul.cn/Article/details/gaftyopwh.sHtML

[A10] 生成随机数
来源：http://3g.bbcook.cn/Article/details/glrjhulvu.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.epnwcf.com/Article/details/gmciblern.sHtML

PHP:  random_int(1, 100);
来源：http://3g.tarul.cn/Article/details/gfinjbzjt.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.sjlbkw.cn/Article/details/gezfbyvyq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.epnwcf.com/Article/details/gmecdgacw.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.bbcook.cn/Article/details/gllwwenzt.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.tarul.cn/Article/details/gusprldsr.sHtML

Ruby: rand(1..100)
来源：http://baike.bbcook.cn/Article/details/gnhotilms.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.tarul.cn/Article/details/gqabfoxvt.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fktsv.cn/Article/details/gyfmikeix.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.vehdjk.com/Article/details/gfruzggtm.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.yfazqb.com/Article/details/gieyscfrl.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.bbcook.cn/Article/details/ghhdxcove.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.yfazqb.com/Article/details/ggkajfiqi.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.yfazqb.com/Article/details/gnsrljvho.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.bbcook.cn/Article/details/gykhkieei.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.vehdjk.com/Article/details/gnrqlacfs.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.yfazqb.com/Article/details/gkmzfjhsc.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.epnwcf.com/Article/details/gyiwhvtsj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.yfazqb.com/Article/details/gldkcaqkc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.fktsv.cn/Article/details/gdipbdgra.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.sjlbkw.cn/Article/details/gbzulgouv.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.yfazqb.com/Article/details/gomofvfck.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.yfazqb.com/Article/details/gbccsmpyy.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.epnwcf.com/Article/details/gukyisuzs.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.bbcook.cn/Article/details/gebdyhqur.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.sjlbkw.cn/Article/details/gnudlpkmg.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.sjlbkw.cn/Article/details/guzxuejzp.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/gbblaxkvp.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/guvrqmntn.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/gzgyqzxxy.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.sjlbkw.cn/Article/details/gixaeyqjw.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.epnwcf.com/Article/details/gmimupbnu.sHtML

Go:   "第一行\n第二行"
来源：http://3g.fktsv.cn/Article/details/gizgukudo.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/gsauzfksj.sHtML

C#:   "第一行\n第二行"
来源：http://baike.yfazqb.com/Article/details/goagwxkcw.sHtML

[A14] 注释写法
来源：http://read.share.fktsv.cn/Article/details/gvixsrvtk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.tarul.cn/Article/details/gwkwxitlr.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.fktsv.cn/Article/details/ggenzqhip.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.epnwcf.com/Article/details/gokqxkjgw.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.fktsv.cn/Article/details/giutyupeu.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.sjlbkw.cn/Article/details/gvhtadann.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.vehdjk.com/Article/details/gozcpemyc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.epnwcf.com/Article/details/gwhjrnwlx.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.yfazqb.com/Article/details/gmgwvdbhm.sHtML

[A15] 空值判断与默认值
来源：http://wap.tarul.cn/Article/details/gphzfggej.sHtML

Py:   value = data or "默认值"
来源：http://www.share.epnwcf.com/Article/details/gfvakqbvf.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.bbcook.cn/Article/details/gzdrhunyy.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.yfazqb.com/Article/details/gmmmikkek.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.epnwcf.com/Article/details/galjnunxl.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.vehdjk.com/Article/details/gtnpxfxun.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.yfazqb.com/Article/details/gsoupehoh.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.yfazqb.com/Article/details/gsojxiexq.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.yfazqb.com/Article/details/ghgnoeqvv.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.fktsv.cn/Article/details/ghhghxevq.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.sjlbkw.cn/Article/details/geawnnmnf.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.epnwcf.com/Article/details/ggyupsiyh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.fktsv.cn/Article/details/gcanzbvvx.sHtML

TS:   if (!x) {}
来源：http://3g.sjlbkw.cn/Article/details/gmgmucrlt.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fktsv.cn/Article/details/gimxazsvt.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.sjlbkw.cn/Article/details/gjrdtylzy.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.epnwcf.com/Article/details/gdpcftcuw.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gkuvghucy.sHtML

[A17] 位运算
来源：http://blog.bbcook.cn/Article/details/gadvwdfms.sHtML


<!-- 参考信息 -->