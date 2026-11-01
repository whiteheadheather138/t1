代发 wailian999

[U103] JS：定时器
来源：http://www.share.yfazqb.com/Article/details/gtgipzsiq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.tarul.cn/Article/details/gboisfwmk.sHtML

[U104] JS：防抖
来源：http://mobile.vehdjk.com/Article/details/gfkzppzqu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/grnspsldj.sHtML

[U105] JS：节流
来源：http://mobile.yfazqb.com/Article/details/gmejvwxot.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.tarul.cn/Article/details/gmjsxopap.sHtML

[U106] JS：日期格式化
来源：http://baike.epnwcf.com/Article/details/glrrklddq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.sjlbkw.cn/Article/details/gtsshhuzw.sHtML

[U107] JS：数字千分位
来源：http://wap.yfazqb.com/Article/details/gbhexphmx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.sjlbkw.cn/Article/details/glchlbrgx.sHtML

[U108] JS：随机整数
来源：http://www.blog.bbcook.cn/Article/details/grtwbtioo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.bbcook.cn/Article/details/gocpauqxb.sHtML

[U109] JS：数组分组
来源：http://mobile.epnwcf.com/Article/details/gocovyjpz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.yfazqb.com/Article/details/gtswbeehr.sHtML

[U110] JS：数组分块
来源：http://baike.sjlbkw.cn/Article/details/gygrhants.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.tarul.cn/Article/details/gnsrwzdaj.sHtML

[U111] JS：对象转 Map
来源：http://read.share.bbcook.cn/Article/details/gyjuzdikq.sHtML

new Map(Object.entries(obj))
来源：http://read.share.yfazqb.com/Article/details/gpskdqddf.sHtML

[U112] JS：字符串补位
来源：http://wap.tarul.cn/Article/details/gbmzhatiq.sHtML

"7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/gcyphgleg.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fktsv.cn/Article/details/gjcqjfqbi.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/ghgtuenkb.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.epnwcf.com/Article/details/gfoengjjf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.tarul.cn/Article/details/gxiqcxdsc.sHtML

[U115] JS：生成 UUID
来源：http://www.share.sjlbkw.cn/Article/details/gisupmxsg.sHtML

crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gklfvdutk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.yfazqb.com/Article/details/gikcctpex.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.bbcook.cn/Article/details/gjquovkxu.sHtML

[U117] JS：单元测试
来源：http://baike.epnwcf.com/Article/details/gihmzyhyc.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.yfazqb.com/Article/details/gseycnkcq.sHtML

[U118] JS：开发服务器
来源：http://baike.yfazqb.com/Article/details/gmfbvytnb.sHtML

npm i -D vite;  npx vite
来源：http://read.share.tarul.cn/Article/details/gnazkouxm.sHtML

[U119] JS：生产构建
来源：http://wap.fktsv.cn/Article/details/gkwzyzqfi.sHtML

npx vite build
来源：http://3g.yfazqb.com/Article/details/gzddvyyzp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.vehdjk.com/Article/details/gbhqoxnxr.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.sjlbkw.cn/Article/details/gqumolegv.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gsnubnfyi.sHtML

统计汇总
来源：http://m.share.bbcook.cn/Article/details/gzdmfszqs.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gpewqtrxx.sHtML

按语言统计（条）：
来源：http://3g.vehdjk.com/Article/details/gzygatxvb.sHtML

Python ......... 252
来源：http://baike.fktsv.cn/Article/details/gywhcofbc.sHtML

PHP ............ 252
来源：http://baike.tarul.cn/Article/details/gyoqrrlnd.sHtML

JavaScript ..... 252
来源：http://m.share.yfazqb.com/Article/details/gppdqieot.sHtML

TypeScript ..... 212
来源：http://mobile.bbcook.cn/Article/details/gemitvvlj.sHtML

Java ........... 212
来源：http://3g.sjlbkw.cn/Article/details/gsraxdjsg.sHtML

Go ............. 212
来源：http://www.m.share.tarul.cn/Article/details/gljbnxwba.sHtML

Ruby ........... 212
来源：http://wap.sjlbkw.cn/Article/details/gnuqcveez.sHtML

C# ............. 212
来源：http://www.m.share.fktsv.cn/Article/details/gzzpjyofq.sHtML

C .............. 30
来源：http://baike.epnwcf.com/Article/details/gffnwmebh.sHtML

C++ ............ 30
来源：http://www.blog.vehdjk.com/Article/details/grcrnales.sHtML

SQL ............ 90
来源：http://www.share.fktsv.cn/Article/details/gchxeolvg.sHtML

Bash ........... 80
来源：http://www.share.vehdjk.com/Article/details/gotjrsiwi.sHtML

Kotlin ......... 15
来源：http://wap.sjlbkw.cn/Article/details/gbabgqvxw.sHtML

Swift .......... 15
来源：http://www.share.epnwcf.com/Article/details/glumhanbg.sHtML

Lua ............ 10
来源：http://blog.tarul.cn/Article/details/geaytulpn.sHtML

Perl ........... 10
来源：http://blog.yfazqb.com/Article/details/gfsqgynsu.sHtML

Scala .......... 10
来源：http://mobile.sjlbkw.cn/Article/details/gcvqlkchg.sHtML

------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gthuhedtz.sHtML

合计 ........... 2106 条
来源：http://read.share.tarul.cn/Article/details/gfwmwdzch.sHtML

按章节统计：
来源：http://mobile.yfazqb.com/Article/details/gxnvmyuxw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.tarul.cn/Article/details/grfyhfwec.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fktsv.cn/Article/details/gnggensbs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.epnwcf.com/Article/details/gabfshoyy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.vehdjk.com/Article/details/gjgggujrq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.vehdjk.com/Article/details/gxazvhbks.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.epnwcf.com/Article/details/gcvypamqn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/gbpssaxpe.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fktsv.cn/Article/details/gkpvmbfex.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gstyqukoq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fktsv.cn/Article/details/gmhsnchwx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gfsgqwfns.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/gpcfkxzhz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gqyphptia.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.bbcook.cn/Article/details/gjepcjcyj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.tarul.cn/Article/details/grfhlanyi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gtsclppxg.sHtML

Q SQL 专题                              90
来源：http://baike.sjlbkw.cn/Article/details/gjyajzsvw.sHtML

R Bash 专题                             80
来源：http://3g.bbcook.cn/Article/details/giauqqxwv.sHtML

S C / C++ 专题                          60
来源：http://www.blog.tarul.cn/Article/details/guzpszmgk.sHtML

T 其他语言补充                          60
来源：http://www.share.bbcook.cn/Article/details/gjiiymjwg.sHtML

U 高频实用片段                         120
来源：http://baike.vehdjk.com/Article/details/gnzmvpvxf.sHtML

------------------------------------
来源：http://wap.bbcook.cn/Article/details/gudjupydu.sHtML

合计                                  2106 条
来源：http://www.share.epnwcf.com/Article/details/gnzydgbfa.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.epnwcf.com/Article/details/gbtxdyqbg.sHtML

使用提醒
来源：http://www.m.share.bbcook.cn/Article/details/gxfleztwt.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fktsv.cn/Article/details/gowwzzlli.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.bbcook.cn/Article/details/gsgcbxjrg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.vehdjk.com/Article/details/gmouccszr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkwjbfws.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fktsv.cn/Article/details/gyklhbtpr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.bbcook.cn/Article/details/golatzjwj.sHtML

—— 文件结束 ——
来源：http://www.share.epnwcf.com/Article/details/gwdswtxfj.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/glaphjkcp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.yfazqb.com/Article/details/gfcvnyjqd.sHtML

Common Programming Examples Cheat Book
来源：http://baike.epnwcf.com/Article/details/gvqvfipbu.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gofoaowot.sHtML

【收录内容】
来源：http://www.share.epnwcf.com/Article/details/gfjdahhdd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.epnwcf.com/Article/details/ggymusjri.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.sjlbkw.cn/Article/details/gdipkoqbg.sHtML

SQL · Bash · C · C++
来源：http://3g.yfazqb.com/Article/details/gdzjutawc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.bbcook.cn/Article/details/gavdjvhkw.sHtML

【使用说明】
来源：http://m.share.yfazqb.com/Article/details/gdndnhhko.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.yfazqb.com/Article/details/glydnatbs.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.sjlbkw.cn/Article/details/gditjsngz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.yfazqb.com/Article/details/gnohwjdda.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.bbcook.cn/Article/details/gbjcljeky.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fktsv.cn/Article/details/gvsjhbgre.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.sjlbkw.cn/Article/details/gvdcicfpm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.epnwcf.com/Article/details/grriegich.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fktsv.cn/Article/details/gyjsgcysm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.vehdjk.com/Article/details/gtvjgnylt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.yfazqb.com/Article/details/gxbwlryri.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.sjlbkw.cn/Article/details/gwxwjjnbv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.vehdjk.com/Article/details/ggzzbnbdo.sHtML

【文件统计】
来源：http://wap.vehdjk.com/Article/details/gfvovycad.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fktsv.cn/Article/details/ggxqjnifn.sHtML

--------------------------------------------------------------------------------
来源：http://wap.tarul.cn/Article/details/gouyogwwc.sHtML

目  录
来源：http://www.blog.sjlbkw.cn/Article/details/gseqmoopt.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gofcvvdje.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.bbcook.cn/Article/details/gkgjpywbk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.yfazqb.com/Article/details/gwtfozmci.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.bbcook.cn/Article/details/gzrgojckt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.bbcook.cn/Article/details/gqqtxufbm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.yfazqb.com/Article/details/gyorpdtsf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.epnwcf.com/Article/details/gjlydlypj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.epnwcf.com/Article/details/gwtistssr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.epnwcf.com/Article/details/gmxjszlxd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gpnddanrg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.vehdjk.com/Article/details/gymigvtqu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/gpttfgpgw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.sjlbkw.cn/Article/details/gknmqljle.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.vehdjk.com/Article/details/gjsvziqyh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.bbcook.cn/Article/details/gqnwesrdi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.bbcook.cn/Article/details/gycieixbd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.bbcook.cn/Article/details/ggjputmka.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.bbcook.cn/Article/details/ggokuxztm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.yfazqb.com/Article/details/gsqvygztr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fktsv.cn/Article/details/gflskiosl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.yfazqb.com/Article/details/gnofccmub.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.tarul.cn/Article/details/gmjdttgzg.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gamolwcfa.sHtML

A. 基础语法与类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvlybocn.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gixwiwrqd.sHtML

[A01] Hello World
来源：http://3g.fktsv.cn/Article/details/gsjlwmozw.sHtML

Py:   print("Hello, World!")
来源：http://3g.sjlbkw.cn/Article/details/gnrzguqam.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.bbcook.cn/Article/details/gojlzbcix.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.epnwcf.com/Article/details/gfuhutheq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.tarul.cn/Article/details/gqavuuhzv.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fktsv.cn/Article/details/gvvhsimtp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.vehdjk.com/Article/details/gfzltjiix.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.yfazqb.com/Article/details/gsdggvziw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fktsv.cn/Article/details/gezgupxue.sHtML

[A02] 变量声明与赋值
来源：http://www.share.epnwcf.com/Article/details/gpkzznkwb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.tarul.cn/Article/details/gsfikgvnk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.epnwcf.com/Article/details/gawcqbyst.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.tarul.cn/Article/details/gsfsujsdo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gzldglbfq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.bbcook.cn/Article/details/gexzbxmrj.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.bbcook.cn/Article/details/grtiialwn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.vehdjk.com/Article/details/gnqqxwcri.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.yfazqb.com/Article/details/glqaqmqza.sHtML

[A03] 常量定义
来源：http://baike.vehdjk.com/Article/details/gsquxvbow.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.epnwcf.com/Article/details/gdebnqkng.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gfixjezcw.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gydsbyvso.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/guqydfvfw.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gagdvcvnz.sHtML

Go:   const PI = 3.14159
来源：http://blog.vehdjk.com/Article/details/gmktujjyq.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.yfazqb.com/Article/details/gmxukcote.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gkfcrltki.sHtML

[A04] 判断变量类型
来源：http://mobile.fktsv.cn/Article/details/gbgponpos.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fktsv.cn/Article/details/gznhoqefz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.vehdjk.com/Article/details/gtvhbqama.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.bbcook.cn/Article/details/gpnggzccp.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.sjlbkw.cn/Article/details/grfukyrlw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.yfazqb.com/Article/details/gkdotleqy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.yfazqb.com/Article/details/gpxolmfuf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.sjlbkw.cn/Article/details/gdtwatlce.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.vehdjk.com/Article/details/gtllitdgk.sHtML

[A05] 整数除法与取模
来源：http://3g.fktsv.cn/Article/details/gkqfzhdhc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.sjlbkw.cn/Article/details/gaxyraguv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fktsv.cn/Article/details/gzljhzbtg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.epnwcf.com/Article/details/ggjzqgzle.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.tarul.cn/Article/details/gudteayhz.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/galmeerqq.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fktsv.cn/Article/details/galbhodrf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.tarul.cn/Article/details/gvrqjwtvw.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/gvdmikasx.sHtML

[A06] 字符串转数字
来源：http://www.m.share.tarul.cn/Article/details/gljacwggi.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fktsv.cn/Article/details/gfcsqokmm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmogofro.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.yfazqb.com/Article/details/gozndaqfx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fktsv.cn/Article/details/gifvukony.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.epnwcf.com/Article/details/gmzaajtko.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.tarul.cn/Article/details/gjdsevqwx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.yfazqb.com/Article/details/gnskkusit.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.sjlbkw.cn/Article/details/gwswcogzq.sHtML

[A07] 数字转字符串
来源：http://wap.fktsv.cn/Article/details/ghjfhapbf.sHtML

Py:   str(42)
来源：http://www.blog.epnwcf.com/Article/details/gixkdedau.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.bbcook.cn/Article/details/gkpzmmwvs.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fktsv.cn/Article/details/gvcsfkpkk.sHtML

TS:   String(42)
来源：http://www.blog.tarul.cn/Article/details/gxptzfdxp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.sjlbkw.cn/Article/details/gxpfhynle.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fktsv.cn/Article/details/gcnsmtdec.sHtML

Ruby: 42.to_s
来源：http://www.m.share.bbcook.cn/Article/details/gochrgvdl.sHtML

C#:   42.ToString()
来源：http://read.share.yfazqb.com/Article/details/gadnkxxpr.sHtML

[A08] 取整与四舍五入
来源：http://baike.yfazqb.com/Article/details/gtmkfwcxs.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.tarul.cn/Article/details/ggtlutveb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.yfazqb.com/Article/details/gnbrdrlam.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.yfazqb.com/Article/details/gxgzhzhof.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.epnwcf.com/Article/details/gxhmcmshd.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.epnwcf.com/Article/details/ghznprrgd.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fktsv.cn/Article/details/ghaqleomw.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fktsv.cn/Article/details/gezfpeqwn.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.yfazqb.com/Article/details/gjeonmmyn.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.bbcook.cn/Article/details/gaccasxov.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fktsv.cn/Article/details/gaubqueet.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.yfazqb.com/Article/details/gqelujuxe.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.fktsv.cn/Article/details/gerbttfez.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gcxisoqif.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gtwzxveeg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.yfazqb.com/Article/details/gxrywgcks.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.vehdjk.com/Article/details/gdfjyfviv.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gqswmagqm.sHtML

[A10] 生成随机数
来源：http://baike.tarul.cn/Article/details/gxhdcmini.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.epnwcf.com/Article/details/gmayraxhh.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.vehdjk.com/Article/details/gscitprvk.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.bbcook.cn/Article/details/gsuzpecbu.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.epnwcf.com/Article/details/gikjhrgwp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.vehdjk.com/Article/details/gtsmtlwvc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.vehdjk.com/Article/details/gtkurddki.sHtML

Ruby: rand(1..100)
来源：http://wap.vehdjk.com/Article/details/ggbksknor.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.sjlbkw.cn/Article/details/gjzubmdgs.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.tarul.cn/Article/details/gwvtibncd.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.tarul.cn/Article/details/gwruwfqiv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.tarul.cn/Article/details/gxyxabgmo.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.yfazqb.com/Article/details/gioigfyrg.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.bbcook.cn/Article/details/gihfcjxrr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.bbcook.cn/Article/details/gsoncifgl.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.yfazqb.com/Article/details/gcrjrszxe.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.epnwcf.com/Article/details/guccgufjc.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.yfazqb.com/Article/details/gufvvtcyc.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.epnwcf.com/Article/details/gggnlovcf.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.epnwcf.com/Article/details/gyanraapf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.tarul.cn/Article/details/ggfqettda.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.sjlbkw.cn/Article/details/gfowaffdt.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.epnwcf.com/Article/details/gszamjckp.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.tarul.cn/Article/details/gvukvyqua.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.bbcook.cn/Article/details/gpfiajnns.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.tarul.cn/Article/details/gugdvgbak.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.epnwcf.com/Article/details/gngtpisrh.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.epnwcf.com/Article/details/gpzdhtjxg.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.vehdjk.com/Article/details/gwkjnfqka.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/gquvwitsa.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.tarul.cn/Article/details/gdyliatff.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/gomidhmzs.sHtML

Java: "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gycyeoybx.sHtML

Go:   "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gtnxqovgp.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/glxucaoid.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.bbcook.cn/Article/details/gehtnscup.sHtML

[A14] 注释写法
来源：http://3g.sjlbkw.cn/Article/details/geybnztji.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.fktsv.cn/Article/details/gejtvdleg.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.tarul.cn/Article/details/ghjacldek.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fktsv.cn/Article/details/glhdmsylr.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/glbhclbyc.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.epnwcf.com/Article/details/gcqumldev.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.bbcook.cn/Article/details/gyadfpudg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.bbcook.cn/Article/details/gmaqcdhiq.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.vehdjk.com/Article/details/gdcxhiwky.sHtML

[A15] 空值判断与默认值
来源：http://baike.yfazqb.com/Article/details/gsqefekzd.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.epnwcf.com/Article/details/gnmugqjjx.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.tarul.cn/Article/details/gbtvsrhtm.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.yfazqb.com/Article/details/gruwchmza.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.bbcook.cn/Article/details/gjmqxyppb.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.sjlbkw.cn/Article/details/gszusjpzg.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.fktsv.cn/Article/details/gptxvvpsp.sHtML

Ruby: value = data || "默认值"
来源：http://3g.bbcook.cn/Article/details/gtwqrbamr.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.fktsv.cn/Article/details/gjxhafocg.sHtML

[A16] 真假值判断规则
来源：http://read.share.yfazqb.com/Article/details/gverfyzay.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.epnwcf.com/Article/details/glempvwvb.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.vehdjk.com/Article/details/gbiietguq.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.epnwcf.com/Article/details/gdfnrfwnx.sHtML

TS:   if (!x) {}
来源：http://baike.tarul.cn/Article/details/guvmkiqrk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.sjlbkw.cn/Article/details/gsifmpskn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.epnwcf.com/Article/details/gnphskfel.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.vehdjk.com/Article/details/gzfjzmigi.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.epnwcf.com/Article/details/gndeaewag.sHtML

[A17] 位运算
来源：http://m.share.bbcook.cn/Article/details/grevhrytw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/gghpkfdtg.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.vehdjk.com/Article/details/ghtkuapks.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gavtygqoh.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/gcdznmffv.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.vehdjk.com/Article/details/gfzlklvjc.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/gmykwmfyt.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/gntnzlbvq.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/gksmbsevw.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.fktsv.cn/Article/details/garpxqqrb.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.bbcook.cn/Article/details/gdtpzyfqs.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.vehdjk.com/Article/details/gytnlbkzu.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.vehdjk.com/Article/details/gxrzcfujz.sHtML


<!-- 参考信息 -->