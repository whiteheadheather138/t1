代发 wailian999

[U103] JS：定时器
来源：http://read.share.vehdjk.com/Article/details/gabvypjjt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.bbcook.cn/Article/details/gnsaqncqi.sHtML

[U104] JS：防抖
来源：http://wap.bbcook.cn/Article/details/gybidnwlx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/gufnrbheh.sHtML

[U105] JS：节流
来源：http://mobile.yfazqb.com/Article/details/gcsehzhsu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.bbcook.cn/Article/details/geauqbrib.sHtML

[U106] JS：日期格式化
来源：http://wap.vehdjk.com/Article/details/gpvnftkay.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.yfazqb.com/Article/details/gxpmkcgdf.sHtML

[U107] JS：数字千分位
来源：http://m.share.vehdjk.com/Article/details/gkrhclhcq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fktsv.cn/Article/details/glucnmhbi.sHtML

[U108] JS：随机整数
来源：http://3g.tarul.cn/Article/details/gfnmdytqu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.vehdjk.com/Article/details/gppljqvsi.sHtML

[U109] JS：数组分组
来源：http://read.share.yfazqb.com/Article/details/gtqcjscpz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.yfazqb.com/Article/details/gkuuwmgyp.sHtML

[U110] JS：数组分块
来源：http://3g.sjlbkw.cn/Article/details/gmnletmhg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.bbcook.cn/Article/details/grajxytsg.sHtML

[U111] JS：对象转 Map
来源：http://blog.vehdjk.com/Article/details/ggdybmguw.sHtML

new Map(Object.entries(obj))
来源：http://read.share.sjlbkw.cn/Article/details/gdcvsywmj.sHtML

[U112] JS：字符串补位
来源：http://baike.bbcook.cn/Article/details/gdsjnplkg.sHtML

"7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gbaozzjlq.sHtML

[U113] JS：正则替换全部
来源：http://blog.sjlbkw.cn/Article/details/gegyuvxqn.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gjbezaexs.sHtML

[U114] JS：JSON 深比较
来源：http://baike.tarul.cn/Article/details/glaucdgse.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fktsv.cn/Article/details/gxqlxmbqd.sHtML

[U115] JS：生成 UUID
来源：http://www.share.tarul.cn/Article/details/glbfowolb.sHtML

crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gorigzvka.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.tarul.cn/Article/details/geygpksgg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.epnwcf.com/Article/details/gqdpaionp.sHtML

[U117] JS：单元测试
来源：http://www.share.epnwcf.com/Article/details/ghmxareyr.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.vehdjk.com/Article/details/gbfezectw.sHtML

[U118] JS：开发服务器
来源：http://3g.tarul.cn/Article/details/goczakqip.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fktsv.cn/Article/details/gmtdgnrnk.sHtML

[U119] JS：生产构建
来源：http://read.share.tarul.cn/Article/details/gwemzacbo.sHtML

npx vite build
来源：http://3g.yfazqb.com/Article/details/giajqsmuq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.sjlbkw.cn/Article/details/gfdehdfbf.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.vehdjk.com/Article/details/gpexiouco.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gbaetlgey.sHtML

统计汇总
来源：http://m.share.epnwcf.com/Article/details/gvfzndniq.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gvljrfexa.sHtML

按语言统计（条）：
来源：http://blog.sjlbkw.cn/Article/details/ghqzvzogg.sHtML

Python ......... 252
来源：http://www.blog.epnwcf.com/Article/details/gvkwkngak.sHtML

PHP ............ 252
来源：http://baike.vehdjk.com/Article/details/giolilekb.sHtML

JavaScript ..... 252
来源：http://blog.sjlbkw.cn/Article/details/gzlcvcwdz.sHtML

TypeScript ..... 212
来源：http://mobile.fktsv.cn/Article/details/giwzhamgt.sHtML

Java ........... 212
来源：http://baike.vehdjk.com/Article/details/gblutwjhy.sHtML

Go ............. 212
来源：http://3g.bbcook.cn/Article/details/gxnhwvijo.sHtML

Ruby ........... 212
来源：http://www.m.share.bbcook.cn/Article/details/goxcdwlvm.sHtML

C# ............. 212
来源：http://read.share.epnwcf.com/Article/details/ghmmuhymv.sHtML

C .............. 30
来源：http://m.share.yfazqb.com/Article/details/gltpvicsd.sHtML

C++ ............ 30
来源：http://read.share.vehdjk.com/Article/details/gqjwtdoaa.sHtML

SQL ............ 90
来源：http://www.blog.yfazqb.com/Article/details/grkxlrvaf.sHtML

Bash ........... 80
来源：http://3g.sjlbkw.cn/Article/details/gggmqdswi.sHtML

Kotlin ......... 15
来源：http://baike.epnwcf.com/Article/details/gtqiyhjrg.sHtML

Swift .......... 15
来源：http://m.share.yfazqb.com/Article/details/gcdwrbptg.sHtML

Lua ............ 10
来源：http://blog.vehdjk.com/Article/details/gjogyglbm.sHtML

Perl ........... 10
来源：http://www.share.tarul.cn/Article/details/gzvcaepvo.sHtML

Scala .......... 10
来源：http://3g.vehdjk.com/Article/details/gcnqzglir.sHtML

------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gkivahwfw.sHtML

合计 ........... 2106 条
来源：http://read.share.fktsv.cn/Article/details/gqhwihrvd.sHtML

按章节统计：
来源：http://3g.epnwcf.com/Article/details/gtuytkviw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.bbcook.cn/Article/details/gkrcsrwcz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.bbcook.cn/Article/details/gknzrsvim.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.sjlbkw.cn/Article/details/gsjsjkbij.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.tarul.cn/Article/details/gkglskrxk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.epnwcf.com/Article/details/ggdmqdjly.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.tarul.cn/Article/details/gffjzvtmb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.epnwcf.com/Article/details/gmzbvrhxu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.tarul.cn/Article/details/gzdabqqkd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gsocjgexi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.yfazqb.com/Article/details/gdwxelxdd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gwlndzqhi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gdtjsuwtd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gadebxuri.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.epnwcf.com/Article/details/gdhkzpebs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.bbcook.cn/Article/details/gbddavroy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/gcylzodhf.sHtML

Q SQL 专题                              90
来源：http://blog.epnwcf.com/Article/details/gygbzhgxk.sHtML

R Bash 专题                             80
来源：http://m.share.fktsv.cn/Article/details/gxjznrqxn.sHtML

S C / C++ 专题                          60
来源：http://mobile.fktsv.cn/Article/details/grwexuuzp.sHtML

T 其他语言补充                          60
来源：http://3g.fktsv.cn/Article/details/gmbekeyid.sHtML

U 高频实用片段                         120
来源：http://www.share.fktsv.cn/Article/details/gblekfljc.sHtML

------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/gzgvcgiqt.sHtML

合计                                  2106 条
来源：http://wap.sjlbkw.cn/Article/details/gozliprxd.sHtML

--------------------------------------------------------------------------------
来源：http://baike.tarul.cn/Article/details/gzdxuthtj.sHtML

使用提醒
来源：http://blog.tarul.cn/Article/details/gvpxeqzho.sHtML

--------------------------------------------------------------------------------
来源：http://blog.epnwcf.com/Article/details/ghcjlcfgl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.bbcook.cn/Article/details/gsheckpdi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.sjlbkw.cn/Article/details/gqviabtyg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.sjlbkw.cn/Article/details/ghvrabaqi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fktsv.cn/Article/details/ghdgdydgd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fktsv.cn/Article/details/gokvjbuhg.sHtML

—— 文件结束 ——
来源：http://www.share.vehdjk.com/Article/details/glnjdcmlz.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gtplbnxlh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.yfazqb.com/Article/details/gtbdkrkxq.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.sjlbkw.cn/Article/details/gwknwjekf.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmxnpopmb.sHtML

【收录内容】
来源：http://www.m.share.epnwcf.com/Article/details/gjsgwevwf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.epnwcf.com/Article/details/ghwequkce.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.vehdjk.com/Article/details/gslzipjrw.sHtML

SQL · Bash · C · C++
来源：http://baike.bbcook.cn/Article/details/gamzfotqb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.epnwcf.com/Article/details/gogazqunl.sHtML

【使用说明】
来源：http://www.m.share.tarul.cn/Article/details/glqqbhugt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.yfazqb.com/Article/details/gagrsgqwh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.epnwcf.com/Article/details/gkrgplpae.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.tarul.cn/Article/details/ghpawynee.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.vehdjk.com/Article/details/gdgxmcksq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fktsv.cn/Article/details/gxraqsqgm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.vehdjk.com/Article/details/ghfcqyfeq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.sjlbkw.cn/Article/details/gwmidhmcn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fktsv.cn/Article/details/ggngveqeb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fktsv.cn/Article/details/gfcjeermw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.vehdjk.com/Article/details/gcinzoukh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.bbcook.cn/Article/details/grsuymxwu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.vehdjk.com/Article/details/goxdriyqu.sHtML

【文件统计】
来源：http://m.share.yfazqb.com/Article/details/gsbwnclmj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.bbcook.cn/Article/details/gbuawuupz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/gvtctswvq.sHtML

目  录
来源：http://www.share.vehdjk.com/Article/details/gsccvcoxa.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/grhgoefve.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.yfazqb.com/Article/details/gecxhdvvd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fktsv.cn/Article/details/goisdipmj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.yfazqb.com/Article/details/gavllplql.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fktsv.cn/Article/details/gwtarnbwq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.tarul.cn/Article/details/guexivpcy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.sjlbkw.cn/Article/details/gvcpnnqut.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.bbcook.cn/Article/details/gznitvian.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.epnwcf.com/Article/details/gwbhcaxbj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.epnwcf.com/Article/details/gaxuaqfwt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.vehdjk.com/Article/details/grpqulmlg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/glkzkuwdy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.sjlbkw.cn/Article/details/gadhbcdey.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/gxurzxqho.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.bbcook.cn/Article/details/ghpnmqtso.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjjyswfa.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fktsv.cn/Article/details/gkfcbpgyk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.epnwcf.com/Article/details/galtgxzzh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.vehdjk.com/Article/details/gbadoujnn.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.yfazqb.com/Article/details/gijxsrqhf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.bbcook.cn/Article/details/gjbdxpzta.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.vehdjk.com/Article/details/gbqvilyfh.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gnjihksni.sHtML

A. 基础语法与类型
来源：http://baike.vehdjk.com/Article/details/gpbefxecp.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gsiayqhhv.sHtML

[A01] Hello World
来源：http://3g.epnwcf.com/Article/details/gpchbaeia.sHtML

Py:   print("Hello, World!")
来源：http://mobile.sjlbkw.cn/Article/details/gwqwxkptz.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.sjlbkw.cn/Article/details/gqmhxwerb.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.vehdjk.com/Article/details/gohwlkxhg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.yfazqb.com/Article/details/gnaypfcse.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.epnwcf.com/Article/details/gqnefzqqo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.yfazqb.com/Article/details/gvfueafmx.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbxupnkz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.tarul.cn/Article/details/gjooscdzq.sHtML

[A02] 变量声明与赋值
来源：http://m.share.yfazqb.com/Article/details/gbshzijjb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.yfazqb.com/Article/details/gwobzgsrx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.vehdjk.com/Article/details/gmzmmdevb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.sjlbkw.cn/Article/details/gasntcvkk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.vehdjk.com/Article/details/gugyyvsmm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fktsv.cn/Article/details/gfkbsxurp.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.yfazqb.com/Article/details/geyvovngt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.vehdjk.com/Article/details/gtrnyydyp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.bbcook.cn/Article/details/goyklpsls.sHtML

[A03] 常量定义
来源：http://www.share.vehdjk.com/Article/details/gfsifqtdy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.bbcook.cn/Article/details/gqyngnhom.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/giropmnmk.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gyueujthg.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gbckbrvbh.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/gnaajifhi.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.sjlbkw.cn/Article/details/gffrxspwn.sHtML

Ruby: PI = 3.14159
来源：http://mobile.epnwcf.com/Article/details/gidhnxryu.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gxtakoyhb.sHtML

[A04] 判断变量类型
来源：http://www.m.share.yfazqb.com/Article/details/gbelrggjy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.sjlbkw.cn/Article/details/gjkqnjlud.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.bbcook.cn/Article/details/gfczfuugi.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.bbcook.cn/Article/details/ghzsuoiwd.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.sjlbkw.cn/Article/details/grtpozyax.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fktsv.cn/Article/details/gstdpqiit.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.yfazqb.com/Article/details/gpivqagtt.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.vehdjk.com/Article/details/gqkmmcsof.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.tarul.cn/Article/details/gvyeeqaca.sHtML

[A05] 整数除法与取模
来源：http://wap.tarul.cn/Article/details/ggsuhttku.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.epnwcf.com/Article/details/gjndlcxlp.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.bbcook.cn/Article/details/gpgrdufdx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.epnwcf.com/Article/details/gfskswyhs.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.yfazqb.com/Article/details/gpllwgkpg.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.bbcook.cn/Article/details/gmvdrhytc.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.tarul.cn/Article/details/gblkqahvy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.vehdjk.com/Article/details/gqecjhrbx.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gailhaezc.sHtML

[A06] 字符串转数字
来源：http://baike.fktsv.cn/Article/details/gcttxzfua.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.bbcook.cn/Article/details/gphpiocwy.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.vehdjk.com/Article/details/gandfigcu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.yfazqb.com/Article/details/glnldkiyi.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fktsv.cn/Article/details/gxgrmdepw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.bbcook.cn/Article/details/gdsimzbnl.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.vehdjk.com/Article/details/gqrpmiono.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.epnwcf.com/Article/details/gvavdkclx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.epnwcf.com/Article/details/gbwqgpbkw.sHtML

[A07] 数字转字符串
来源：http://baike.vehdjk.com/Article/details/gbcksntyu.sHtML

Py:   str(42)
来源：http://read.share.vehdjk.com/Article/details/gmrcfxfpo.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.yfazqb.com/Article/details/ghcernkiy.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fktsv.cn/Article/details/grbekiavm.sHtML

TS:   String(42)
来源：http://m.share.yfazqb.com/Article/details/gueeuwxwe.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.epnwcf.com/Article/details/gmsjqucto.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.vehdjk.com/Article/details/ggoedyduv.sHtML

Ruby: 42.to_s
来源：http://blog.vehdjk.com/Article/details/gzkhfabqq.sHtML

C#:   42.ToString()
来源：http://www.m.share.fktsv.cn/Article/details/gbemebjxo.sHtML

[A08] 取整与四舍五入
来源：http://baike.vehdjk.com/Article/details/gwkflhlvn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.sjlbkw.cn/Article/details/gipgmrpyy.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.yfazqb.com/Article/details/gzdjoacpo.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.vehdjk.com/Article/details/gbmdbvvev.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.epnwcf.com/Article/details/geonyptmy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/glxmsirpn.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.yfazqb.com/Article/details/glifoqsdu.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.vehdjk.com/Article/details/gxtdjkhms.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.yfazqb.com/Article/details/gwdclzkbc.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.tarul.cn/Article/details/gusejebaq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gnzgugfmd.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/grfswmqfh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.yfazqb.com/Article/details/gwzhoodeu.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.tarul.cn/Article/details/gokqpehrc.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.vehdjk.com/Article/details/gxvortvoh.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.epnwcf.com/Article/details/gkctqknhz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fktsv.cn/Article/details/gboydkyjd.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.fktsv.cn/Article/details/gsodlmhnq.sHtML

[A10] 生成随机数
来源：http://3g.vehdjk.com/Article/details/ghoghfxbg.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.yfazqb.com/Article/details/gjdbitrua.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.epnwcf.com/Article/details/gmjwooeoo.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.vehdjk.com/Article/details/gtwyaeoef.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.tarul.cn/Article/details/ghyddjffq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.yfazqb.com/Article/details/gehkmvnwj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.yfazqb.com/Article/details/gcrtlzygz.sHtML

Ruby: rand(1..100)
来源：http://baike.yfazqb.com/Article/details/gfqungypu.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.sjlbkw.cn/Article/details/guypegjdv.sHtML

[A11] 条件表达式（三元）
来源：http://blog.bbcook.cn/Article/details/glcewanct.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.epnwcf.com/Article/details/gluejildo.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.yfazqb.com/Article/details/guzlmbwdz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.fktsv.cn/Article/details/guvioqqkx.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fktsv.cn/Article/details/gwpkfnfgj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.yfazqb.com/Article/details/gnvktqlqm.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.bbcook.cn/Article/details/gvhrsdmbo.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.vehdjk.com/Article/details/giymzwvek.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.epnwcf.com/Article/details/gsfawowym.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.bbcook.cn/Article/details/grkrieswx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.tarul.cn/Article/details/gdyzeasmz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwaxzehmq.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.yfazqb.com/Article/details/gtdwhqwyr.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.tarul.cn/Article/details/ggkyeqetn.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.sjlbkw.cn/Article/details/gwapogade.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.bbcook.cn/Article/details/gbhgllzjx.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.vehdjk.com/Article/details/gnkiavvxl.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.sjlbkw.cn/Article/details/girdrreyw.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.sjlbkw.cn/Article/details/gupdyxqwx.sHtML

Py:   "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gvlcnzshx.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/gtbfewsaf.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/gywoezluj.sHtML

TS:   "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gikumcjyz.sHtML

Java: "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/grjzwiwan.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/giklncigz.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gbneiqgfl.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/gguandwrl.sHtML

[A14] 注释写法
来源：http://m.share.vehdjk.com/Article/details/ghjsozlnw.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.yfazqb.com/Article/details/goquaoaef.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fktsv.cn/Article/details/gzvkilfzq.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.vehdjk.com/Article/details/gwntypdrd.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.tarul.cn/Article/details/gfrknnval.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.sjlbkw.cn/Article/details/gatptlokd.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.yfazqb.com/Article/details/gkdkcunvf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.vehdjk.com/Article/details/gtjptuogq.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.tarul.cn/Article/details/gnvbxfewk.sHtML

[A15] 空值判断与默认值
来源：http://m.share.tarul.cn/Article/details/gpnvjxckq.sHtML

Py:   value = data or "默认值"
来源：http://www.share.vehdjk.com/Article/details/ghnvxevwl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.yfazqb.com/Article/details/garnegdnl.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.bbcook.cn/Article/details/gloqthjfl.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.epnwcf.com/Article/details/gitoxeanf.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.bbcook.cn/Article/details/guttadnfn.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fktsv.cn/Article/details/gshxidlcb.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.tarul.cn/Article/details/gbcpqxtyi.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.vehdjk.com/Article/details/geyzslqhg.sHtML

[A16] 真假值判断规则
来源：http://blog.fktsv.cn/Article/details/gmzaaxymy.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.bbcook.cn/Article/details/gneshsrha.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.sjlbkw.cn/Article/details/gtpbczire.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.tarul.cn/Article/details/gbrhqdqqq.sHtML

TS:   if (!x) {}
来源：http://read.share.yfazqb.com/Article/details/gqbbnyrvz.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.yfazqb.com/Article/details/gacoreyez.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.fktsv.cn/Article/details/gkxivklop.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.epnwcf.com/Article/details/giedrywxc.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.fktsv.cn/Article/details/gkomrxfve.sHtML

[A17] 位运算
来源：http://m.share.epnwcf.com/Article/details/gwwyjbqmm.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/giryyzpgp.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/getdoocuh.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gzitqxpzc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/giyphdiow.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gtxhwrxpo.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/gwqnjibad.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/gqgljiizd.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/gdjtnwsbb.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.bbcook.cn/Article/details/gmegotdmn.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.sjlbkw.cn/Article/details/gyjztyzcm.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.epnwcf.com/Article/details/gnkvwwoyn.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.yfazqb.com/Article/details/gdasexozr.sHtML


<!-- 参考信息 -->