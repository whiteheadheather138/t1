代发 wailian999

[U103] JS：定时器
来源：http://www.blog.fktsv.cn/Article/details/gwbbfjmbn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.yfazqb.com/Article/details/gdvlyrkeh.sHtML

[U104] JS：防抖
来源：http://baike.bbcook.cn/Article/details/gtohnfztu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/gertphjdd.sHtML

[U105] JS：节流
来源：http://baike.epnwcf.com/Article/details/gdzlkbtif.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gordtjcrr.sHtML

[U106] JS：日期格式化
来源：http://m.share.vehdjk.com/Article/details/gsdlfyyep.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.bbcook.cn/Article/details/gdvfufidf.sHtML

[U107] JS：数字千分位
来源：http://wap.fktsv.cn/Article/details/gxnolqjlr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fktsv.cn/Article/details/grapnaqdq.sHtML

[U108] JS：随机整数
来源：http://wap.bbcook.cn/Article/details/gcfxenaeg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.tarul.cn/Article/details/glcynsuhq.sHtML

[U109] JS：数组分组
来源：http://www.blog.vehdjk.com/Article/details/gisoozvzh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.sjlbkw.cn/Article/details/gzambgmbl.sHtML

[U110] JS：数组分块
来源：http://3g.epnwcf.com/Article/details/gnemlzrei.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.epnwcf.com/Article/details/gjbicglge.sHtML

[U111] JS：对象转 Map
来源：http://3g.epnwcf.com/Article/details/gqzjqzvpq.sHtML

new Map(Object.entries(obj))
来源：http://baike.epnwcf.com/Article/details/gqtkxobqw.sHtML

[U112] JS：字符串补位
来源：http://read.share.bbcook.cn/Article/details/gviqwrrsa.sHtML

"7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gnbpejtmt.sHtML

[U113] JS：正则替换全部
来源：http://read.share.epnwcf.com/Article/details/gzreopkdj.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gdciohkcu.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fktsv.cn/Article/details/gxxhueqsl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.tarul.cn/Article/details/gdtbxuhdu.sHtML

[U115] JS：生成 UUID
来源：http://3g.fktsv.cn/Article/details/gesrtshwl.sHtML

crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/gaifhsvpg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.tarul.cn/Article/details/gtdxevbjx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.vehdjk.com/Article/details/guxvsidoj.sHtML

[U117] JS：单元测试
来源：http://m.share.fktsv.cn/Article/details/gpvfsusdr.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fktsv.cn/Article/details/glugttivd.sHtML

[U118] JS：开发服务器
来源：http://m.share.tarul.cn/Article/details/gblgwhpxt.sHtML

npm i -D vite;  npx vite
来源：http://m.share.tarul.cn/Article/details/gpofbpqwh.sHtML

[U119] JS：生产构建
来源：http://www.m.share.yfazqb.com/Article/details/gmbkyxhex.sHtML

npx vite build
来源：http://m.share.bbcook.cn/Article/details/grfdkzwxw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.yfazqb.com/Article/details/gsajftgck.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.yfazqb.com/Article/details/gtswmocwe.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gcngfvuru.sHtML

统计汇总
来源：http://wap.tarul.cn/Article/details/glpudmhcf.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gxwldjyyq.sHtML

按语言统计（条）：
来源：http://www.share.fktsv.cn/Article/details/gmnyoaeax.sHtML

Python ......... 252
来源：http://blog.bbcook.cn/Article/details/guegdqtch.sHtML

PHP ............ 252
来源：http://www.share.tarul.cn/Article/details/gtmxrvwrs.sHtML

JavaScript ..... 252
来源：http://www.blog.tarul.cn/Article/details/gxbfbxtrp.sHtML

TypeScript ..... 212
来源：http://www.share.bbcook.cn/Article/details/gpwfspcpc.sHtML

Java ........... 212
来源：http://www.share.bbcook.cn/Article/details/gougyxzqd.sHtML

Go ............. 212
来源：http://wap.bbcook.cn/Article/details/gouaurvuj.sHtML

Ruby ........... 212
来源：http://www.m.share.bbcook.cn/Article/details/grbelrvmv.sHtML

C# ............. 212
来源：http://mobile.epnwcf.com/Article/details/gfjiahjkt.sHtML

C .............. 30
来源：http://read.share.tarul.cn/Article/details/gzpqscget.sHtML

C++ ............ 30
来源：http://wap.vehdjk.com/Article/details/gxvlaflja.sHtML

SQL ............ 90
来源：http://3g.tarul.cn/Article/details/gtmtyxegf.sHtML

Bash ........... 80
来源：http://m.share.yfazqb.com/Article/details/gmizzryzf.sHtML

Kotlin ......... 15
来源：http://wap.tarul.cn/Article/details/giwowpghj.sHtML

Swift .......... 15
来源：http://baike.fktsv.cn/Article/details/gadojnxje.sHtML

Lua ............ 10
来源：http://blog.bbcook.cn/Article/details/gpjrkxtzc.sHtML

Perl ........... 10
来源：http://baike.bbcook.cn/Article/details/gceaydcrz.sHtML

Scala .......... 10
来源：http://blog.epnwcf.com/Article/details/gaatwjrdg.sHtML

------------------------------------
来源：http://3g.tarul.cn/Article/details/geqslhkzq.sHtML

合计 ........... 2106 条
来源：http://www.blog.bbcook.cn/Article/details/gdebmdkau.sHtML

按章节统计：
来源：http://www.blog.epnwcf.com/Article/details/gatjfouyd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.sjlbkw.cn/Article/details/gebyfracy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.yfazqb.com/Article/details/gdzyctudt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.sjlbkw.cn/Article/details/gwqyyhyvv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.tarul.cn/Article/details/gmdrgkufj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.sjlbkw.cn/Article/details/gdzvwkzyd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.sjlbkw.cn/Article/details/gzrnrtlik.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfgarcha.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.sjlbkw.cn/Article/details/gufeewpwc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gujmwuesg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.epnwcf.com/Article/details/gdkpvdmlm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/guxnjfvtb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gnszmawxm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/gowaexmex.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.tarul.cn/Article/details/greuibfwi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.tarul.cn/Article/details/gdqviuxar.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/ghnwssbdd.sHtML

Q SQL 专题                              90
来源：http://www.m.share.tarul.cn/Article/details/gxhbraduy.sHtML

R Bash 专题                             80
来源：http://m.share.fktsv.cn/Article/details/gxqlqwtkn.sHtML

S C / C++ 专题                          60
来源：http://blog.yfazqb.com/Article/details/gcblwpkfg.sHtML

T 其他语言补充                          60
来源：http://www.share.fktsv.cn/Article/details/ghrodsrnq.sHtML

U 高频实用片段                         120
来源：http://mobile.bbcook.cn/Article/details/ghzhybdqh.sHtML

------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gwahjdysi.sHtML

合计                                  2106 条
来源：http://www.blog.vehdjk.com/Article/details/ggkecfebi.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gtevwwwle.sHtML

使用提醒
来源：http://www.share.bbcook.cn/Article/details/gawcygjjy.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.epnwcf.com/Article/details/gizyexegk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.epnwcf.com/Article/details/gibtxddak.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.vehdjk.com/Article/details/gjxwzttib.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.bbcook.cn/Article/details/grenllmoe.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.tarul.cn/Article/details/gqpnekjep.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fktsv.cn/Article/details/gsxhlipkm.sHtML

—— 文件结束 ——
来源：http://www.blog.tarul.cn/Article/details/gctpyqefr.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gogkpuajp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.epnwcf.com/Article/details/gqqiawgox.sHtML

Common Programming Examples Cheat Book
来源：http://baike.sjlbkw.cn/Article/details/gjwrrnykb.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/glwrtsrcn.sHtML

【收录内容】
来源：http://www.share.vehdjk.com/Article/details/gwvzgtlnf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fktsv.cn/Article/details/gpmozbdki.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.epnwcf.com/Article/details/gvmpzuzgy.sHtML

SQL · Bash · C · C++
来源：http://wap.vehdjk.com/Article/details/gtevikmma.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fktsv.cn/Article/details/gisszquhu.sHtML

【使用说明】
来源：http://3g.fktsv.cn/Article/details/gzdctmmje.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fktsv.cn/Article/details/gztcmlviw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.epnwcf.com/Article/details/ggvvftqxa.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.epnwcf.com/Article/details/grlsoiahc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.vehdjk.com/Article/details/garvymjvh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.yfazqb.com/Article/details/gpxhjcnyb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.tarul.cn/Article/details/ggbwuzyua.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhujoauq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.tarul.cn/Article/details/gyirytduh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.tarul.cn/Article/details/glnhzoull.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.vehdjk.com/Article/details/gqrpoqsrf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.tarul.cn/Article/details/gqqkzykib.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.yfazqb.com/Article/details/gzpmigbfd.sHtML

【文件统计】
来源：http://www.share.sjlbkw.cn/Article/details/gcxxrvdop.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.vehdjk.com/Article/details/gxwllqomk.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gkluczzyo.sHtML

目  录
来源：http://wap.fktsv.cn/Article/details/gosxiqhjm.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fktsv.cn/Article/details/gszjulyjg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fktsv.cn/Article/details/gerevaxkb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.vehdjk.com/Article/details/gkvcjenrp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.vehdjk.com/Article/details/glhgwrric.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.vehdjk.com/Article/details/gamnicvmv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.sjlbkw.cn/Article/details/gzinlaobg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gnkzmvzcf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.bbcook.cn/Article/details/gezfvetzz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.sjlbkw.cn/Article/details/grceyfvwk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/gvxhhgalu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.epnwcf.com/Article/details/gnkranyaz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/gmibtbadj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/gmenxoxze.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fktsv.cn/Article/details/gunioykmk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fktsv.cn/Article/details/guisxcyor.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.bbcook.cn/Article/details/gzkuuesff.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.sjlbkw.cn/Article/details/gdnphycwk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.vehdjk.com/Article/details/gqsrujvsf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gucxugcgr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.epnwcf.com/Article/details/gspbuauru.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.sjlbkw.cn/Article/details/gzisefelt.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrbwbrtg.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gbhhtyzom.sHtML

A. 基础语法与类型
来源：http://www.share.vehdjk.com/Article/details/gqcxlzkvb.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gregmcqai.sHtML

[A01] Hello World
来源：http://read.share.tarul.cn/Article/details/gzgkcnznf.sHtML

Py:   print("Hello, World!")
来源：http://mobile.bbcook.cn/Article/details/ggyswlrtl.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.bbcook.cn/Article/details/gjcxcliib.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fktsv.cn/Article/details/gxyhecaad.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fktsv.cn/Article/details/gwnnhzhph.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.sjlbkw.cn/Article/details/gcdknnkod.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtapafupo.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.tarul.cn/Article/details/gonqgztzz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.vehdjk.com/Article/details/gvckxhkky.sHtML

[A02] 变量声明与赋值
来源：http://read.share.tarul.cn/Article/details/gvtcqqfce.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.tarul.cn/Article/details/gzupffrbd.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gpbefsbnf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.tarul.cn/Article/details/gqkjdfetv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.yfazqb.com/Article/details/gscfpcezj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.yfazqb.com/Article/details/gxunhhuuo.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fktsv.cn/Article/details/ggtgjsmdo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.tarul.cn/Article/details/gccqbqhol.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fktsv.cn/Article/details/gjarejjwd.sHtML

[A03] 常量定义
来源：http://mobile.fktsv.cn/Article/details/gahatsdym.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.yfazqb.com/Article/details/gbdzeifeo.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gtzqvpcwf.sHtML

JS:   const PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/ggijtdztr.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gugqqthza.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/gdztugjbv.sHtML

Go:   const PI = 3.14159
来源：http://www.share.vehdjk.com/Article/details/glwfooftt.sHtML

Ruby: PI = 3.14159
来源：http://www.share.sjlbkw.cn/Article/details/gfnsrcxmp.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gdbmebshu.sHtML

[A04] 判断变量类型
来源：http://www.m.share.bbcook.cn/Article/details/gubpbdjdt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.epnwcf.com/Article/details/gevxjzvyv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fktsv.cn/Article/details/gjtlqnjgt.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fktsv.cn/Article/details/gzfokyljh.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.yfazqb.com/Article/details/gouzkvdpr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.bbcook.cn/Article/details/gquugirgr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.epnwcf.com/Article/details/gcicgfveg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.yfazqb.com/Article/details/gkbqjcfpp.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.epnwcf.com/Article/details/giuyrjrgp.sHtML

[A05] 整数除法与取模
来源：http://mobile.tarul.cn/Article/details/gdtjbmxib.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.bbcook.cn/Article/details/gvrkilgzr.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.sjlbkw.cn/Article/details/gzodaifxm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.tarul.cn/Article/details/grlmxqyxg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gnsivnadm.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gbgyxnodg.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gagakobul.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.fktsv.cn/Article/details/gvdlbticq.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.sjlbkw.cn/Article/details/gzoxzcvsn.sHtML

[A06] 字符串转数字
来源：http://blog.epnwcf.com/Article/details/gogeortgh.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.sjlbkw.cn/Article/details/geqvkccqd.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.sjlbkw.cn/Article/details/ghjbfrgck.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.epnwcf.com/Article/details/gvbxbawcn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.vehdjk.com/Article/details/gjhvzxxtg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.bbcook.cn/Article/details/gtrolqynp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.tarul.cn/Article/details/ggcadajxc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.bbcook.cn/Article/details/ggtnuqpaz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.epnwcf.com/Article/details/goxrhcfkj.sHtML

[A07] 数字转字符串
来源：http://mobile.bbcook.cn/Article/details/gsrgsctfg.sHtML

Py:   str(42)
来源：http://baike.tarul.cn/Article/details/gsmuzohln.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.bbcook.cn/Article/details/gmhgszlxo.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.yfazqb.com/Article/details/gmgmgdvdp.sHtML

TS:   String(42)
来源：http://wap.epnwcf.com/Article/details/gqlwlmwfe.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.tarul.cn/Article/details/gtfkownap.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.yfazqb.com/Article/details/glwxewvms.sHtML

Ruby: 42.to_s
来源：http://www.blog.bbcook.cn/Article/details/gkpadmlvb.sHtML

C#:   42.ToString()
来源：http://m.share.epnwcf.com/Article/details/gwlapymoi.sHtML

[A08] 取整与四舍五入
来源：http://read.share.vehdjk.com/Article/details/geumnwzip.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fktsv.cn/Article/details/grdjayyea.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.sjlbkw.cn/Article/details/glacqojbx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.bbcook.cn/Article/details/gjngnxgxz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.yfazqb.com/Article/details/gzddtgatl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.vehdjk.com/Article/details/ghinzkykf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.epnwcf.com/Article/details/gnwgmxwqb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.tarul.cn/Article/details/gpjvjfpbv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.bbcook.cn/Article/details/gnhxwlfvp.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.sjlbkw.cn/Article/details/goqvssnuq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gxawgaxik.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.tarul.cn/Article/details/gxcdosqyx.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.tarul.cn/Article/details/gizcsvjeq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.yfazqb.com/Article/details/glnarxawi.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gqntkqdfg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.epnwcf.com/Article/details/gxzgxvbbg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.yfazqb.com/Article/details/gwlolxhnh.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.bbcook.cn/Article/details/gifsxyjyi.sHtML

[A10] 生成随机数
来源：http://read.share.bbcook.cn/Article/details/gexhhtrml.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.sjlbkw.cn/Article/details/gdpkzvgcx.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdupxqms.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.yfazqb.com/Article/details/gosvnwmzr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.yfazqb.com/Article/details/geasvsvsr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fktsv.cn/Article/details/ggczxtqpm.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.bbcook.cn/Article/details/garhmtack.sHtML

Ruby: rand(1..100)
来源：http://www.share.sjlbkw.cn/Article/details/gitxflhdf.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.tarul.cn/Article/details/grylxfutl.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.vehdjk.com/Article/details/giqlnmgbo.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.sjlbkw.cn/Article/details/gbwpzpkvi.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fktsv.cn/Article/details/gunmlihkg.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/ggdwoewjy.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.yfazqb.com/Article/details/gglbtsbcx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gdrjmhjcn.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.yfazqb.com/Article/details/gybfwakbw.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.vehdjk.com/Article/details/gtflvjmxx.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.fktsv.cn/Article/details/gyhrqnfxo.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fktsv.cn/Article/details/gkuavdlir.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.epnwcf.com/Article/details/gpiarcxll.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpexnxxk.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.vehdjk.com/Article/details/gfwgzpazv.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.tarul.cn/Article/details/gbmpizjjr.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.sjlbkw.cn/Article/details/ghlsochlq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.epnwcf.com/Article/details/gvputmelz.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.fktsv.cn/Article/details/gjkljsgwy.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.yfazqb.com/Article/details/gslvbzcvi.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.sjlbkw.cn/Article/details/gnfazazve.sHtML

Py:   "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/gtspvgnzv.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/giyvlnjhe.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/gbnzjshsg.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/gfrodkiph.sHtML

Java: "第一行\n第二行"
来源：http://m.share.bbcook.cn/Article/details/ggtiukmnm.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/gwflpeihz.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gfjfhvatj.sHtML

C#:   "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gktazkjjg.sHtML

[A14] 注释写法
来源：http://mobile.fktsv.cn/Article/details/ghwdxeica.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.epnwcf.com/Article/details/guwhhzpfd.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/gcwkohroy.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fktsv.cn/Article/details/gcxrwceqy.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/gdheccolu.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.bbcook.cn/Article/details/gvmypkulx.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.epnwcf.com/Article/details/gflarkrjo.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.yfazqb.com/Article/details/grrbykqeg.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/gzkanspek.sHtML

[A15] 空值判断与默认值
来源：http://3g.tarul.cn/Article/details/gzfnivfit.sHtML

Py:   value = data or "默认值"
来源：http://read.share.yfazqb.com/Article/details/gjeqvdzxq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.vehdjk.com/Article/details/giwdbmiqm.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.bbcook.cn/Article/details/gmxndoopj.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.fktsv.cn/Article/details/gelhfsmqm.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.bbcook.cn/Article/details/gwslpxdqc.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.yfazqb.com/Article/details/gmwhowzoo.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.tarul.cn/Article/details/gligzjrvn.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.epnwcf.com/Article/details/gjiyrixhi.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.fktsv.cn/Article/details/gsxspptud.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fktsv.cn/Article/details/gytvzidoh.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.fktsv.cn/Article/details/gzmlnkusb.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.fktsv.cn/Article/details/ghtlntdnk.sHtML

TS:   if (!x) {}
来源：http://mobile.vehdjk.com/Article/details/grkfpgytz.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.vehdjk.com/Article/details/gzwhxvbpn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.tarul.cn/Article/details/gvdnlfsxt.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.yfazqb.com/Article/details/gzwmkvena.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.vehdjk.com/Article/details/gsxzqnsmu.sHtML

[A17] 位运算
来源：http://blog.sjlbkw.cn/Article/details/grajkdrsp.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.yfazqb.com/Article/details/gyzmitgco.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.bbcook.cn/Article/details/gjncmqahy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/gutsfbupz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/gwnsinxji.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/geaokvuuo.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gpdufzdno.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/gporvprme.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/gscqrkzvz.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.sjlbkw.cn/Article/details/gzonyhsmt.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.tarul.cn/Article/details/gdoztmrzw.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.tarul.cn/Article/details/gtrdryeyb.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.vehdjk.com/Article/details/gxnvomtlf.sHtML


<!-- 参考信息 -->