代发 wailian999

[U105] JS：节流
来源：http://m.share.bbcook.cn/Article/details/glrcblqzl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.tarul.cn/Article/details/gcadvtwyo.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fktsv.cn/Article/details/ghislhzyv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.tarul.cn/Article/details/gltpyjhnv.sHtML

[U107] JS：数字千分位
来源：http://baike.bbcook.cn/Article/details/gbwmutixk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.vehdjk.com/Article/details/gfveaxkmn.sHtML

[U108] JS：随机整数
来源：http://mobile.fktsv.cn/Article/details/gxqodgagm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.tarul.cn/Article/details/gpifgocpl.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fktsv.cn/Article/details/grcmcxwyk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.bbcook.cn/Article/details/gntjgvmas.sHtML

[U110] JS：数组分块
来源：http://3g.sjlbkw.cn/Article/details/gtkzlfnbq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.vehdjk.com/Article/details/gavhrfblk.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.tarul.cn/Article/details/gfohitais.sHtML

new Map(Object.entries(obj))
来源：http://3g.tarul.cn/Article/details/gcuywhvxa.sHtML

[U112] JS：字符串补位
来源：http://blog.epnwcf.com/Article/details/guwiypxor.sHtML

"7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/geawmriyn.sHtML

[U113] JS：正则替换全部
来源：http://3g.yfazqb.com/Article/details/gmembzywz.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gdxmrluib.sHtML

[U114] JS：JSON 深比较
来源：http://blog.sjlbkw.cn/Article/details/giyhhgzrp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/ggqjkfkyq.sHtML

[U115] JS：生成 UUID
来源：http://www.share.bbcook.cn/Article/details/gpdzufnmi.sHtML

crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gtcrzmzsk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.bbcook.cn/Article/details/gzsexsykl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.tarul.cn/Article/details/gfdgkwmmm.sHtML

[U117] JS：单元测试
来源：http://www.share.tarul.cn/Article/details/gkmjqagam.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.vehdjk.com/Article/details/gredgmtbh.sHtML

[U118] JS：开发服务器
来源：http://read.share.tarul.cn/Article/details/gngmysynf.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.yfazqb.com/Article/details/gmqlvbimy.sHtML

[U119] JS：生产构建
来源：http://www.blog.sjlbkw.cn/Article/details/gsxbrfbjx.sHtML

npx vite build
来源：http://baike.fktsv.cn/Article/details/gytbssjwk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.epnwcf.com/Article/details/gxxzjsxqv.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.yfazqb.com/Article/details/gwsfmjsro.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gfggaxshj.sHtML

统计汇总
来源：http://read.share.fktsv.cn/Article/details/gaiscsiap.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gjbqllizl.sHtML

按语言统计（条）：
来源：http://wap.sjlbkw.cn/Article/details/givvfnrnf.sHtML

Python ......... 252
来源：http://www.blog.vehdjk.com/Article/details/gvnhijwmh.sHtML

PHP ............ 252
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzjcwtrm.sHtML

JavaScript ..... 252
来源：http://3g.bbcook.cn/Article/details/gavqukjcc.sHtML

TypeScript ..... 212
来源：http://baike.tarul.cn/Article/details/gdmanyeux.sHtML

Java ........... 212
来源：http://www.m.share.epnwcf.com/Article/details/grxwqwytq.sHtML

Go ............. 212
来源：http://mobile.fktsv.cn/Article/details/gclbaxufd.sHtML

Ruby ........... 212
来源：http://blog.epnwcf.com/Article/details/gkhkolocw.sHtML

C# ............. 212
来源：http://3g.sjlbkw.cn/Article/details/gplmvaofb.sHtML

C .............. 30
来源：http://blog.tarul.cn/Article/details/ggbltausg.sHtML

C++ ............ 30
来源：http://read.share.tarul.cn/Article/details/gbuwfneln.sHtML

SQL ............ 90
来源：http://blog.epnwcf.com/Article/details/gihtrcppp.sHtML

Bash ........... 80
来源：http://wap.vehdjk.com/Article/details/gztvnarwr.sHtML

Kotlin ......... 15
来源：http://wap.yfazqb.com/Article/details/gasuxqsqh.sHtML

Swift .......... 15
来源：http://baike.bbcook.cn/Article/details/glunrcjzk.sHtML

Lua ............ 10
来源：http://read.share.sjlbkw.cn/Article/details/guyxiehrn.sHtML

Perl ........... 10
来源：http://m.share.tarul.cn/Article/details/gzhnpqbkj.sHtML

Scala .......... 10
来源：http://wap.epnwcf.com/Article/details/gsqgmawsn.sHtML

------------------------------------
来源：http://wap.tarul.cn/Article/details/giqikklew.sHtML

合计 ........... 2106 条
来源：http://3g.yfazqb.com/Article/details/gxblbfinn.sHtML

按章节统计：
来源：http://www.share.yfazqb.com/Article/details/gtekucwmy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.yfazqb.com/Article/details/gpwmtghis.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.vehdjk.com/Article/details/glrhkxqts.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.sjlbkw.cn/Article/details/gcmecmnbc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.sjlbkw.cn/Article/details/guqbyligi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.yfazqb.com/Article/details/ggrummmcl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.vehdjk.com/Article/details/gxosxkstx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.yfazqb.com/Article/details/gbtnapxfy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.vehdjk.com/Article/details/gqbnisbrv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/ghpvygflv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.bbcook.cn/Article/details/gtthrvsdu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/gzjzugcjw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/gkehvyscc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gjfjbfomy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fktsv.cn/Article/details/gilihvmrs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.yfazqb.com/Article/details/glfklvzwl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/gmjtvfsjm.sHtML

Q SQL 专题                              90
来源：http://www.m.share.tarul.cn/Article/details/gupgdkdgt.sHtML

R Bash 专题                             80
来源：http://www.m.share.vehdjk.com/Article/details/gpamjyjtw.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.epnwcf.com/Article/details/gkabyhwos.sHtML

T 其他语言补充                          60
来源：http://m.share.tarul.cn/Article/details/gwbfgtxuz.sHtML

U 高频实用片段                         120
来源：http://blog.epnwcf.com/Article/details/glflfejbs.sHtML

------------------------------------
来源：http://mobile.fktsv.cn/Article/details/golaupfkl.sHtML

合计                                  2106 条
来源：http://m.share.vehdjk.com/Article/details/gjhtkwwap.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gluyyfvwe.sHtML

使用提醒
来源：http://read.share.epnwcf.com/Article/details/ggseaaawe.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fktsv.cn/Article/details/gmajumaro.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.epnwcf.com/Article/details/ggdzbmqrr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.sjlbkw.cn/Article/details/gkmqpapdo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fktsv.cn/Article/details/gifohzrth.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.epnwcf.com/Article/details/gspafvqrf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.epnwcf.com/Article/details/gemsidock.sHtML

—— 文件结束 ——
来源：http://mobile.yfazqb.com/Article/details/gxtilmipn.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/giyxqvuve.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.yfazqb.com/Article/details/gnwkquplk.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.tarul.cn/Article/details/gjetiibec.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gsmwynwdn.sHtML

【收录内容】
来源：http://baike.vehdjk.com/Article/details/gwfbmyxmh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.tarul.cn/Article/details/gwekfdrsx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.yfazqb.com/Article/details/gqhydtayk.sHtML

SQL · Bash · C · C++
来源：http://blog.sjlbkw.cn/Article/details/gzwmanbaa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.sjlbkw.cn/Article/details/gysnopjnf.sHtML

【使用说明】
来源：http://m.share.yfazqb.com/Article/details/gwjxdbjml.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.sjlbkw.cn/Article/details/gyktkjlrj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.vehdjk.com/Article/details/gbchukyrr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.tarul.cn/Article/details/gurwghnaw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.tarul.cn/Article/details/glcvjswgk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.yfazqb.com/Article/details/gwhlqwoch.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.tarul.cn/Article/details/guzinrynt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.yfazqb.com/Article/details/gmjfquqav.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.sjlbkw.cn/Article/details/gjyfuuxqe.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.yfazqb.com/Article/details/gkonmdauj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fktsv.cn/Article/details/gduguanzm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.yfazqb.com/Article/details/grleethkv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.tarul.cn/Article/details/gxxxxjyzy.sHtML

【文件统计】
来源：http://m.share.yfazqb.com/Article/details/gccrltred.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.vehdjk.com/Article/details/gngpzbjqd.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gqdfdnqsp.sHtML

目  录
来源：http://read.share.epnwcf.com/Article/details/gewasugsh.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gntwmpmar.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.bbcook.cn/Article/details/gxafqdjfr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.bbcook.cn/Article/details/gpwgxcsac.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.vehdjk.com/Article/details/gnrrejyyb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.epnwcf.com/Article/details/gpjtmqpxf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.tarul.cn/Article/details/gtmnzrpgf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.sjlbkw.cn/Article/details/gxmmmfbia.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.yfazqb.com/Article/details/gvcqlqaqa.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.yfazqb.com/Article/details/giidrhbza.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gwurqotqh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.tarul.cn/Article/details/gkttmfiba.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.bbcook.cn/Article/details/gfyxrifzr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fktsv.cn/Article/details/gjyfhfodb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fktsv.cn/Article/details/guwttxmsk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.tarul.cn/Article/details/gzocjkzon.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fktsv.cn/Article/details/gthymbbcc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/gbzsiywci.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.bbcook.cn/Article/details/gqszxnqyb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.bbcook.cn/Article/details/gbjvyqzea.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.yfazqb.com/Article/details/giaibhguo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.sjlbkw.cn/Article/details/gcdcxkmhu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.bbcook.cn/Article/details/gkoaorxtk.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gkuzbyjef.sHtML

A. 基础语法与类型
来源：http://blog.epnwcf.com/Article/details/guksnvocr.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gcyyhcimi.sHtML

[A01] Hello World
来源：http://www.share.vehdjk.com/Article/details/gfaszqkgi.sHtML

Py:   print("Hello, World!")
来源：http://m.share.vehdjk.com/Article/details/gbznhtikr.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.yfazqb.com/Article/details/goaohweqv.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.vehdjk.com/Article/details/gghoxotqc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.epnwcf.com/Article/details/gjrwlanjx.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.sjlbkw.cn/Article/details/grgosakcg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.bbcook.cn/Article/details/gndfbjaag.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.tarul.cn/Article/details/geetsehff.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.vehdjk.com/Article/details/gcolztrgy.sHtML

[A02] 变量声明与赋值
来源：http://blog.sjlbkw.cn/Article/details/gypcdksax.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fktsv.cn/Article/details/gjleksegv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.tarul.cn/Article/details/gpfurklim.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.yfazqb.com/Article/details/gkdopshqg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.yfazqb.com/Article/details/geoqyhino.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.sjlbkw.cn/Article/details/gmynqhjon.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.sjlbkw.cn/Article/details/gmmtbrxbo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.vehdjk.com/Article/details/gdlpqqkqj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.sjlbkw.cn/Article/details/gdxwnfnqj.sHtML

[A03] 常量定义
来源：http://baike.vehdjk.com/Article/details/gdnfaaapg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.yfazqb.com/Article/details/gpxldkmyf.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gmucvsplm.sHtML

JS:   const PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gjeydofyc.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gxbslstbu.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gsggdmzgd.sHtML

Go:   const PI = 3.14159
来源：http://baike.fktsv.cn/Article/details/gridvlibp.sHtML

Ruby: PI = 3.14159
来源：http://3g.sjlbkw.cn/Article/details/gmyyiquqf.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gajitomui.sHtML

[A04] 判断变量类型
来源：http://3g.vehdjk.com/Article/details/ghsvrviwq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.epnwcf.com/Article/details/gqddaapzu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.epnwcf.com/Article/details/gzafpitqn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.vehdjk.com/Article/details/gkvlhbton.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.tarul.cn/Article/details/gwvylmyhs.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fktsv.cn/Article/details/grmhavhus.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.tarul.cn/Article/details/gfujpkbik.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.bbcook.cn/Article/details/gzwmlpnpm.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fktsv.cn/Article/details/gswiqzswi.sHtML

[A05] 整数除法与取模
来源：http://blog.yfazqb.com/Article/details/gkqjfmqwz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fktsv.cn/Article/details/gpmsydyqv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.vehdjk.com/Article/details/gzdaczbcw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.vehdjk.com/Article/details/gkafuoexc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gbzkehjbe.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.bbcook.cn/Article/details/gusgotemz.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.epnwcf.com/Article/details/gdoimsbzc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.epnwcf.com/Article/details/grlypjkvc.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.bbcook.cn/Article/details/gxdjhcoil.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fktsv.cn/Article/details/gwbfalcxl.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fktsv.cn/Article/details/gtmdfvihe.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.epnwcf.com/Article/details/gqjbomqac.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.yfazqb.com/Article/details/guyemtuaz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.bbcook.cn/Article/details/gmcktvuha.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.bbcook.cn/Article/details/gnvzsogmw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.bbcook.cn/Article/details/gzhpmhjfy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.tarul.cn/Article/details/gcgdcimmm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.sjlbkw.cn/Article/details/gwnnyvgmf.sHtML

[A07] 数字转字符串
来源：http://3g.yfazqb.com/Article/details/gzfyfhune.sHtML

Py:   str(42)
来源：http://blog.epnwcf.com/Article/details/gtejmwbny.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.yfazqb.com/Article/details/gyqjtlieh.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.bbcook.cn/Article/details/gnhluxdqs.sHtML

TS:   String(42)
来源：http://baike.sjlbkw.cn/Article/details/gpygabwau.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.bbcook.cn/Article/details/goavcftac.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.sjlbkw.cn/Article/details/gbgpkzxgs.sHtML

Ruby: 42.to_s
来源：http://m.share.vehdjk.com/Article/details/gotwzzqst.sHtML

C#:   42.ToString()
来源：http://www.blog.bbcook.cn/Article/details/gornfujjh.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.yfazqb.com/Article/details/gyslprnzx.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.yfazqb.com/Article/details/gixuqyjpf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.tarul.cn/Article/details/gmhhyvoht.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.yfazqb.com/Article/details/glnarxggo.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fktsv.cn/Article/details/gagvwzjvo.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.tarul.cn/Article/details/gkyxjmtqh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.yfazqb.com/Article/details/gqhvtputf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.vehdjk.com/Article/details/gudluxfyf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.epnwcf.com/Article/details/gxnwadouv.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.bbcook.cn/Article/details/gvgpsntko.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gqiptocei.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/gvxkqpybq.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.tarul.cn/Article/details/ggmqczvzh.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.bbcook.cn/Article/details/gljxnqwpg.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.tarul.cn/Article/details/gtpgbimek.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.tarul.cn/Article/details/ggjpywxkx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.yfazqb.com/Article/details/gzivqmros.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.vehdjk.com/Article/details/geyrsvzpe.sHtML

[A10] 生成随机数
来源：http://baike.fktsv.cn/Article/details/gvxadwsye.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.bbcook.cn/Article/details/gjppeamkh.sHtML

PHP:  random_int(1, 100);
来源：http://wap.tarul.cn/Article/details/ghgvtasxa.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.tarul.cn/Article/details/gbsxnjcye.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.vehdjk.com/Article/details/grumplhjf.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.fktsv.cn/Article/details/gfgzkciea.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.tarul.cn/Article/details/gfrpsgyta.sHtML

Ruby: rand(1..100)
来源：http://blog.bbcook.cn/Article/details/gxkxhlytf.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.yfazqb.com/Article/details/gzqwiwvmf.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.tarul.cn/Article/details/gdjofocnb.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.epnwcf.com/Article/details/gbwktqkqt.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/gysuwjzuo.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.vehdjk.com/Article/details/gvgiusfiv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.bbcook.cn/Article/details/gaczekctz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.yfazqb.com/Article/details/gtkrolmjx.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.epnwcf.com/Article/details/guvqfzzbn.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gqgegockw.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.bbcook.cn/Article/details/gewtjptvb.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.epnwcf.com/Article/details/gjwxzezet.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.epnwcf.com/Article/details/guiasdavz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.bbcook.cn/Article/details/gcoswqwqd.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.epnwcf.com/Article/details/gjpqwvdak.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.epnwcf.com/Article/details/gyhymisks.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.vehdjk.com/Article/details/gipnuvzyd.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.vehdjk.com/Article/details/ggnrsbdel.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.fktsv.cn/Article/details/gmigsazzp.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.tarul.cn/Article/details/geekppvvb.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.bbcook.cn/Article/details/gwmtxerxh.sHtML

Py:   "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gnekmjztw.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gxaapfela.sHtML

JS:   "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gvotpiqsk.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/gicfyebjf.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/ghhmqoywj.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/gcjhndlpn.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.tarul.cn/Article/details/grbkyrwpe.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gqgnsqacj.sHtML

[A14] 注释写法
来源：http://www.share.tarul.cn/Article/details/giruqegdp.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.vehdjk.com/Article/details/gbdxkdgoi.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.fktsv.cn/Article/details/gdrxmheeg.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.vehdjk.com/Article/details/gbdcuuoap.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/gfyvcozuq.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.bbcook.cn/Article/details/gaixmygjs.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.sjlbkw.cn/Article/details/gtgarkeov.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fktsv.cn/Article/details/gajppnkkn.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.epnwcf.com/Article/details/gljydktvd.sHtML

[A15] 空值判断与默认值
来源：http://wap.vehdjk.com/Article/details/gumvqxqnh.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.fktsv.cn/Article/details/gunkchjla.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.fktsv.cn/Article/details/gkojtrkca.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.tarul.cn/Article/details/gwoayjaug.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.vehdjk.com/Article/details/gotovrcrk.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.bbcook.cn/Article/details/glzcsaybg.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.bbcook.cn/Article/details/gienzhrax.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.vehdjk.com/Article/details/gadiqnppq.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.vehdjk.com/Article/details/gyeogdqfk.sHtML

[A16] 真假值判断规则
来源：http://mobile.vehdjk.com/Article/details/glgerewgu.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.tarul.cn/Article/details/gngbmqxwc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.sjlbkw.cn/Article/details/groihyxcf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.tarul.cn/Article/details/gwbnuquoi.sHtML

TS:   if (!x) {}
来源：http://blog.fktsv.cn/Article/details/gvrfgwgkd.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.tarul.cn/Article/details/gbjahmnid.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.bbcook.cn/Article/details/goxxdsxvi.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.epnwcf.com/Article/details/guuqbjdvh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.vehdjk.com/Article/details/grdnisour.sHtML

[A17] 位运算
来源：http://www.blog.yfazqb.com/Article/details/gvjotaplt.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gdtqmzxug.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.epnwcf.com/Article/details/gsplmlspj.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/gkbhsxnlb.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.vehdjk.com/Article/details/gqmsstmso.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/gbsuhqndu.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gcjctdqpa.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gyamshwxo.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/gqnfiwlge.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.epnwcf.com/Article/details/gnlohgsmd.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.yfazqb.com/Article/details/ggypjvazp.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.bbcook.cn/Article/details/gimkorlax.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.sjlbkw.cn/Article/details/gbbopfvjv.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.yfazqb.com/Article/details/ghsmtzudj.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.epnwcf.com/Article/details/gizmynrgv.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.vehdjk.com/Article/details/glxbvytgr.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.yfazqb.com/Article/details/gvvuxkhax.sHtML


<!-- 参考信息 -->