代发 wailian999

[U103] JS：定时器
来源：http://baike.epnwcf.com/Article/details/glueckfcf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.vehdjk.com/Article/details/gcdyqizwe.sHtML

[U104] JS：防抖
来源：http://read.share.bbcook.cn/Article/details/gzeiqwzqe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/gwqubqxis.sHtML

[U105] JS：节流
来源：http://mobile.fktsv.cn/Article/details/gsbkaouvl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.bbcook.cn/Article/details/golxzmxlt.sHtML

[U106] JS：日期格式化
来源：http://www.share.bbcook.cn/Article/details/gpxeymham.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.tarul.cn/Article/details/gqinlrdmr.sHtML

[U107] JS：数字千分位
来源：http://blog.epnwcf.com/Article/details/gbxkdbkfl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.bbcook.cn/Article/details/ggggdgeis.sHtML

[U108] JS：随机整数
来源：http://read.share.yfazqb.com/Article/details/gbqhonxqh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.epnwcf.com/Article/details/ggyyparxm.sHtML

[U109] JS：数组分组
来源：http://mobile.vehdjk.com/Article/details/gnjxldagx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.epnwcf.com/Article/details/gqatsbitg.sHtML

[U110] JS：数组分块
来源：http://wap.sjlbkw.cn/Article/details/gqtaomnlp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.vehdjk.com/Article/details/gzbevulma.sHtML

[U111] JS：对象转 Map
来源：http://m.share.sjlbkw.cn/Article/details/guacmawdz.sHtML

new Map(Object.entries(obj))
来源：http://3g.fktsv.cn/Article/details/gbjwmmebd.sHtML

[U112] JS：字符串补位
来源：http://baike.fktsv.cn/Article/details/gfyoplkqy.sHtML

"7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gnfbxbddm.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.sjlbkw.cn/Article/details/gjavjnlpw.sHtML

s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/ghnyizhlj.sHtML

[U114] JS：JSON 深比较
来源：http://3g.vehdjk.com/Article/details/grladyjti.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/gntwflyhr.sHtML

[U115] JS：生成 UUID
来源：http://www.share.tarul.cn/Article/details/gursqanna.sHtML

crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gwammgyla.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.bbcook.cn/Article/details/gtkcxwtcy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.epnwcf.com/Article/details/glpziafoc.sHtML

[U117] JS：单元测试
来源：http://read.share.fktsv.cn/Article/details/gxqtplnzt.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.vehdjk.com/Article/details/gujypblbi.sHtML

[U118] JS：开发服务器
来源：http://mobile.bbcook.cn/Article/details/guieurmxr.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.yfazqb.com/Article/details/gcoqayfhy.sHtML

[U119] JS：生产构建
来源：http://m.share.epnwcf.com/Article/details/gqerinwbv.sHtML

npx vite build
来源：http://www.share.tarul.cn/Article/details/gdazvjxik.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.vehdjk.com/Article/details/gifhlfzaq.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.epnwcf.com/Article/details/gpaatemjz.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gwfkpzrom.sHtML

统计汇总
来源：http://www.blog.vehdjk.com/Article/details/ggcwvebtc.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gdeimwzrg.sHtML

按语言统计（条）：
来源：http://read.share.sjlbkw.cn/Article/details/gnhvovffs.sHtML

Python ......... 252
来源：http://blog.epnwcf.com/Article/details/grgvbpyew.sHtML

PHP ............ 252
来源：http://www.blog.epnwcf.com/Article/details/grkczkego.sHtML

JavaScript ..... 252
来源：http://mobile.bbcook.cn/Article/details/gqrpvvsdw.sHtML

TypeScript ..... 212
来源：http://wap.fktsv.cn/Article/details/gblfmzkrm.sHtML

Java ........... 212
来源：http://www.blog.vehdjk.com/Article/details/gwiryszte.sHtML

Go ............. 212
来源：http://wap.tarul.cn/Article/details/gsfcyqzvw.sHtML

Ruby ........... 212
来源：http://3g.vehdjk.com/Article/details/gtknlnjsw.sHtML

C# ............. 212
来源：http://blog.yfazqb.com/Article/details/gyqmjfriy.sHtML

C .............. 30
来源：http://read.share.bbcook.cn/Article/details/gbtwnlvbu.sHtML

C++ ............ 30
来源：http://www.blog.bbcook.cn/Article/details/gzaymiuuj.sHtML

SQL ............ 90
来源：http://blog.sjlbkw.cn/Article/details/gbfjvmqqn.sHtML

Bash ........... 80
来源：http://3g.epnwcf.com/Article/details/gjtllnpbf.sHtML

Kotlin ......... 15
来源：http://www.m.share.fktsv.cn/Article/details/gqdzzcvbk.sHtML

Swift .......... 15
来源：http://3g.tarul.cn/Article/details/gyaebuhbb.sHtML

Lua ............ 10
来源：http://3g.bbcook.cn/Article/details/gjjlscxxt.sHtML

Perl ........... 10
来源：http://wap.fktsv.cn/Article/details/gbbycadhv.sHtML

Scala .......... 10
来源：http://www.blog.fktsv.cn/Article/details/gocbgfgpi.sHtML

------------------------------------
来源：http://www.share.epnwcf.com/Article/details/glwatzhib.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fktsv.cn/Article/details/gdruvmsna.sHtML

按章节统计：
来源：http://read.share.sjlbkw.cn/Article/details/gohaccolm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fktsv.cn/Article/details/gmejvcyxk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.bbcook.cn/Article/details/grcjankyy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.tarul.cn/Article/details/gmytcfsfe.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.tarul.cn/Article/details/gavzpqjoy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fktsv.cn/Article/details/gynisqqdn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.bbcook.cn/Article/details/gihjqfcdo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.vehdjk.com/Article/details/gzcacqfmz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.tarul.cn/Article/details/gzhghorpu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gatrzxbbv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.sjlbkw.cn/Article/details/galtlgqlx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gzgjaamai.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/gzpdqrniq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/gotfujrxy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.bbcook.cn/Article/details/gguvzbsry.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.vehdjk.com/Article/details/gikumqqog.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/gixyjcrqo.sHtML

Q SQL 专题                              90
来源：http://blog.vehdjk.com/Article/details/gfvelyfba.sHtML

R Bash 专题                             80
来源：http://m.share.vehdjk.com/Article/details/grihvgecr.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fktsv.cn/Article/details/ghtlmviyj.sHtML

T 其他语言补充                          60
来源：http://mobile.yfazqb.com/Article/details/glhjvewhr.sHtML

U 高频实用片段                         120
来源：http://m.share.tarul.cn/Article/details/glhsbrrgn.sHtML

------------------------------------
来源：http://3g.fktsv.cn/Article/details/gpcfwcghe.sHtML

合计                                  2106 条
来源：http://3g.sjlbkw.cn/Article/details/greiqxosg.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.tarul.cn/Article/details/gddpodwbu.sHtML

使用提醒
来源：http://www.m.share.tarul.cn/Article/details/gzjivstfl.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gmooxaikl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fktsv.cn/Article/details/gxpakkjkk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.yfazqb.com/Article/details/gsgkgktjn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.tarul.cn/Article/details/gbbjerhsg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.tarul.cn/Article/details/gwwfuvdmp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.sjlbkw.cn/Article/details/giugztoik.sHtML

—— 文件结束 ——
来源：http://wap.tarul.cn/Article/details/gyvqtzdbo.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gxvcmtsyr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.sjlbkw.cn/Article/details/gmxwqimtr.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.epnwcf.com/Article/details/godybtodj.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gsgcvrihk.sHtML

【收录内容】
来源：http://read.share.fktsv.cn/Article/details/guhwxeffb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.bbcook.cn/Article/details/gtosmgdue.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.yfazqb.com/Article/details/gkbsxopff.sHtML

SQL · Bash · C · C++
来源：http://wap.sjlbkw.cn/Article/details/gmfkxfhmo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.sjlbkw.cn/Article/details/gjktycyoc.sHtML

【使用说明】
来源：http://3g.epnwcf.com/Article/details/gbvdpnddi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.yfazqb.com/Article/details/gsmbvxdpy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.yfazqb.com/Article/details/gmccptxdt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.vehdjk.com/Article/details/gubfhknkl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.bbcook.cn/Article/details/gxspjzplw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.epnwcf.com/Article/details/gpaivodwz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.yfazqb.com/Article/details/goggkxenx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.tarul.cn/Article/details/gglcssbwt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.epnwcf.com/Article/details/gifhisisv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.epnwcf.com/Article/details/gvrbpdzir.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fktsv.cn/Article/details/gqwlgbzwa.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.sjlbkw.cn/Article/details/gwbcqzvbr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.epnwcf.com/Article/details/gweqnotah.sHtML

【文件统计】
来源：http://3g.bbcook.cn/Article/details/gidposfzu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.epnwcf.com/Article/details/gohrmxxvl.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fktsv.cn/Article/details/gidrmynmc.sHtML

目  录
来源：http://read.share.bbcook.cn/Article/details/gfrnjgyko.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.tarul.cn/Article/details/grnbkaqql.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.tarul.cn/Article/details/gffngqqtl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fktsv.cn/Article/details/ghlcludrn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.epnwcf.com/Article/details/gvbbuxitq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.vehdjk.com/Article/details/gkarphhat.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.bbcook.cn/Article/details/gsojpnmvk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.yfazqb.com/Article/details/gnjyqaewb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.tarul.cn/Article/details/gxmjdesul.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.yfazqb.com/Article/details/gtnfgioje.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/gllvskyyc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.tarul.cn/Article/details/ggwtnbmrp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.yfazqb.com/Article/details/gbquvbwqm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.vehdjk.com/Article/details/giaaztbgz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.bbcook.cn/Article/details/gyrnjmxqj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.yfazqb.com/Article/details/gempcdpoi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.tarul.cn/Article/details/gacrxwnfz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.bbcook.cn/Article/details/guuttdviv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.bbcook.cn/Article/details/gkhdruyol.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fktsv.cn/Article/details/gfelwlvfl.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.yfazqb.com/Article/details/gyrbxanly.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.yfazqb.com/Article/details/gjbrtowsd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.sjlbkw.cn/Article/details/grphonygk.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gltcestsg.sHtML

A. 基础语法与类型
来源：http://m.share.yfazqb.com/Article/details/gzvzssemj.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gligcvdow.sHtML

[A01] Hello World
来源：http://3g.tarul.cn/Article/details/gbsrsamhe.sHtML

Py:   print("Hello, World!")
来源：http://3g.fktsv.cn/Article/details/gbjuwcgrs.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.yfazqb.com/Article/details/gentmmssb.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.vehdjk.com/Article/details/ghcjeucay.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.tarul.cn/Article/details/gxxkgcqbv.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.vehdjk.com/Article/details/gidazlxsg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.vehdjk.com/Article/details/gzpaadjht.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.epnwcf.com/Article/details/gbvvymgfz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.tarul.cn/Article/details/gpurlygle.sHtML

[A02] 变量声明与赋值
来源：http://read.share.bbcook.cn/Article/details/gjkbknuvy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fktsv.cn/Article/details/gqkvuiwkx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.bbcook.cn/Article/details/gnqlcnmyj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.bbcook.cn/Article/details/gbhfcxlos.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.tarul.cn/Article/details/gwppfqbju.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fktsv.cn/Article/details/ggrhhhkvn.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fktsv.cn/Article/details/gwekckvbt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.tarul.cn/Article/details/gmkdiuiwv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.sjlbkw.cn/Article/details/gmsghwqxb.sHtML

[A03] 常量定义
来源：http://3g.tarul.cn/Article/details/gdwrfcckj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.vehdjk.com/Article/details/gmdrfgqyq.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gaefbtmns.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fktsv.cn/Article/details/gprhrzjiy.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gfawzxmyt.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gdowegfra.sHtML

Go:   const PI = 3.14159
来源：http://mobile.tarul.cn/Article/details/gzekzfojs.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.yfazqb.com/Article/details/ghbkryjjl.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/glivigdzo.sHtML

[A04] 判断变量类型
来源：http://www.blog.tarul.cn/Article/details/ggameltcm.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.vehdjk.com/Article/details/gswgzcpey.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.epnwcf.com/Article/details/gyosydkgh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.vehdjk.com/Article/details/ggrqbojws.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.bbcook.cn/Article/details/ghjzrxsdo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.epnwcf.com/Article/details/gbldohiku.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fktsv.cn/Article/details/gxrwlwxma.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.epnwcf.com/Article/details/gyvjzsodq.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fktsv.cn/Article/details/gnayiwpah.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.vehdjk.com/Article/details/galegdmjk.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.bbcook.cn/Article/details/gstfrjecn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gkecrfavz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.yfazqb.com/Article/details/gyrzgbxmv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.vehdjk.com/Article/details/gqwbnmkzy.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gcjhjbgwy.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/gjunmjzzn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.epnwcf.com/Article/details/glfecpkbe.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.yfazqb.com/Article/details/grtlhwkhw.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fktsv.cn/Article/details/gxokqhrjm.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.tarul.cn/Article/details/gtodfvnqz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.sjlbkw.cn/Article/details/gdwcqaswa.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.bbcook.cn/Article/details/gcrbkbekz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fktsv.cn/Article/details/gdfosofqd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.bbcook.cn/Article/details/guvmvpteh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.tarul.cn/Article/details/gdltoiate.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.sjlbkw.cn/Article/details/gpvxwemrp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.vehdjk.com/Article/details/gkjknemds.sHtML

[A07] 数字转字符串
来源：http://mobile.bbcook.cn/Article/details/gmogpgbwp.sHtML

Py:   str(42)
来源：http://3g.sjlbkw.cn/Article/details/gzmjdgnnd.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.tarul.cn/Article/details/gpsqfbmle.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fktsv.cn/Article/details/guzfsyfyb.sHtML

TS:   String(42)
来源：http://blog.tarul.cn/Article/details/gxwhctwkf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.yfazqb.com/Article/details/gxihszewv.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fktsv.cn/Article/details/gocwsirpx.sHtML

Ruby: 42.to_s
来源：http://mobile.sjlbkw.cn/Article/details/gaavmgazg.sHtML

C#:   42.ToString()
来源：http://www.m.share.vehdjk.com/Article/details/gykridxnh.sHtML

[A08] 取整与四舍五入
来源：http://read.share.yfazqb.com/Article/details/gpvidreui.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.sjlbkw.cn/Article/details/gbanfskjf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.bbcook.cn/Article/details/gikmbqdgl.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.epnwcf.com/Article/details/gqjgsbvog.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.fktsv.cn/Article/details/gcsvklush.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.vehdjk.com/Article/details/gudxoqwbe.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.bbcook.cn/Article/details/gauflibrz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.yfazqb.com/Article/details/gfqqwufzl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fktsv.cn/Article/details/giiiawcve.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fktsv.cn/Article/details/gmbpoiyzs.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.vehdjk.com/Article/details/gelqzgnqn.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gspqxftmu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.tarul.cn/Article/details/gvybeoeqs.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.epnwcf.com/Article/details/ghzczpxry.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gtoiqhrxv.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.bbcook.cn/Article/details/goangyhvc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.epnwcf.com/Article/details/gvqyozemk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/glwwtyrjo.sHtML

[A10] 生成随机数
来源：http://3g.sjlbkw.cn/Article/details/gnwvzenze.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fktsv.cn/Article/details/gfgmtqwyn.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.tarul.cn/Article/details/gyaivortu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.epnwcf.com/Article/details/gwxeldcmz.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.bbcook.cn/Article/details/gqheyjxct.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.bbcook.cn/Article/details/gpketzbek.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.vehdjk.com/Article/details/gskwmvybx.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.tarul.cn/Article/details/giysahtie.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.tarul.cn/Article/details/gukujgyeb.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.tarul.cn/Article/details/glifumeqk.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.tarul.cn/Article/details/geoalrygx.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.yfazqb.com/Article/details/gxcnjrpkm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.vehdjk.com/Article/details/ggfepxtqp.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.fktsv.cn/Article/details/gdmfgsoqm.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.bbcook.cn/Article/details/gjvmfywjt.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.tarul.cn/Article/details/gswaphxqs.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.vehdjk.com/Article/details/gyhrlvuyy.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.sjlbkw.cn/Article/details/gwvetnpbz.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.tarul.cn/Article/details/gmmlagjpa.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fktsv.cn/Article/details/ghkxdlddc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fktsv.cn/Article/details/gkqntcwde.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.sjlbkw.cn/Article/details/gktughjry.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.bbcook.cn/Article/details/grdrkjrgv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.tarul.cn/Article/details/gxjdiwlbp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.fktsv.cn/Article/details/gqxdussro.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.sjlbkw.cn/Article/details/gxihprqzu.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.vehdjk.com/Article/details/garswlopb.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.yfazqb.com/Article/details/gbtslwosq.sHtML

Py:   "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gbkupjfcp.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.vehdjk.com/Article/details/gcugalpyl.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/gjhqdgqrr.sHtML

TS:   "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gifsgbpyt.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.sjlbkw.cn/Article/details/gbrwexaor.sHtML

Go:   "第一行\n第二行"
来源：http://blog.epnwcf.com/Article/details/gejdfnatl.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/gzfgivaql.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/gbogstszj.sHtML

[A14] 注释写法
来源：http://3g.sjlbkw.cn/Article/details/gziyeeqzm.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.tarul.cn/Article/details/gbmoxkdlj.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.yfazqb.com/Article/details/gqubgxazk.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.yfazqb.com/Article/details/ghcesdtnh.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.tarul.cn/Article/details/gqlwozgxe.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.tarul.cn/Article/details/gqahkaoek.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.epnwcf.com/Article/details/gljprwuvf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.vehdjk.com/Article/details/gnwqjsqju.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwamvnnk.sHtML

[A15] 空值判断与默认值
来源：http://www.share.yfazqb.com/Article/details/gzhqicudx.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.vehdjk.com/Article/details/gtzxlamin.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.tarul.cn/Article/details/gatobzvmf.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.sjlbkw.cn/Article/details/gdvpgszbx.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.tarul.cn/Article/details/gbwqqcnhr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.epnwcf.com/Article/details/ghdsgxhqq.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.vehdjk.com/Article/details/ggdkluxpd.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.tarul.cn/Article/details/glsscdard.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.epnwcf.com/Article/details/gocsloafh.sHtML

[A16] 真假值判断规则
来源：http://www.share.tarul.cn/Article/details/gecdsebxy.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.tarul.cn/Article/details/guxbkblkc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.epnwcf.com/Article/details/gimcvcmuj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fktsv.cn/Article/details/gicrargzl.sHtML

TS:   if (!x) {}
来源：http://wap.fktsv.cn/Article/details/giviyrjcc.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.vehdjk.com/Article/details/gevrfoslf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.sjlbkw.cn/Article/details/ghnwnsrva.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.bbcook.cn/Article/details/gsmipjwfa.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fktsv.cn/Article/details/gjjyhrfkx.sHtML

[A17] 位运算
来源：http://read.share.fktsv.cn/Article/details/grsepclud.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/geavxdqwc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fktsv.cn/Article/details/gkswgjhpm.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.vehdjk.com/Article/details/guntzdfgu.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/gfdgntgck.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/gbbxszydt.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gepszteiw.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gefylyxwu.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gehbqipmx.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.sjlbkw.cn/Article/details/getdbxkcr.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.vehdjk.com/Article/details/gdnbjynrf.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.sjlbkw.cn/Article/details/gbanbreei.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.yfazqb.com/Article/details/gmuvhbdgv.sHtML


<!-- 参考信息 -->