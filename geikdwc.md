代发 wailian999

[U105] JS：节流
来源：http://mobile.epnwcf.com/Article/details/gecwdwmuj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fktsv.cn/Article/details/gmdtxikyw.sHtML

[U106] JS：日期格式化
来源：http://blog.epnwcf.com/Article/details/ggkegbpwh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.tarul.cn/Article/details/gbvzzeyty.sHtML

[U107] JS：数字千分位
来源：http://m.share.sjlbkw.cn/Article/details/gltadguxy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.epnwcf.com/Article/details/gvfpkfjvo.sHtML

[U108] JS：随机整数
来源：http://blog.epnwcf.com/Article/details/gpdzofmki.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.tarul.cn/Article/details/gqziciadl.sHtML

[U109] JS：数组分组
来源：http://baike.epnwcf.com/Article/details/ghhaktetw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.vehdjk.com/Article/details/gunnxirtp.sHtML

[U110] JS：数组分块
来源：http://blog.fktsv.cn/Article/details/gckykdmcg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fktsv.cn/Article/details/gvtejchwc.sHtML

[U111] JS：对象转 Map
来源：http://blog.sjlbkw.cn/Article/details/gzajgzfng.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.sjlbkw.cn/Article/details/gmjvdqqzr.sHtML

[U112] JS：字符串补位
来源：http://wap.epnwcf.com/Article/details/gwdjvhmfj.sHtML

"7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gycfbnguo.sHtML

[U113] JS：正则替换全部
来源：http://m.share.bbcook.cn/Article/details/gadfxxjyg.sHtML

s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gtzhipnzb.sHtML

[U114] JS：JSON 深比较
来源：http://wap.sjlbkw.cn/Article/details/gkkpghqci.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.sjlbkw.cn/Article/details/gfzplsles.sHtML

[U115] JS：生成 UUID
来源：http://read.share.sjlbkw.cn/Article/details/gqukbfxzh.sHtML

crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gjqkeuvvr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.bbcook.cn/Article/details/gumotgbhp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.epnwcf.com/Article/details/gqzfpjozt.sHtML

[U117] JS：单元测试
来源：http://wap.fktsv.cn/Article/details/gomgjwqvb.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.bbcook.cn/Article/details/gsmkjcjtn.sHtML

[U118] JS：开发服务器
来源：http://wap.tarul.cn/Article/details/gsbizvpbi.sHtML

npm i -D vite;  npx vite
来源：http://read.share.vehdjk.com/Article/details/ghcsobgpw.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fktsv.cn/Article/details/gzolbomrq.sHtML

npx vite build
来源：http://www.blog.fktsv.cn/Article/details/gkhuvqpyq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fktsv.cn/Article/details/gfaekehtz.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.tarul.cn/Article/details/gchmqoysh.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gfrkroxhw.sHtML

统计汇总
来源：http://wap.fktsv.cn/Article/details/gbblzgfzo.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gdlnyketf.sHtML

按语言统计（条）：
来源：http://www.m.share.fktsv.cn/Article/details/gmkjjiiph.sHtML

Python ......... 252
来源：http://blog.bbcook.cn/Article/details/gpigmvlqn.sHtML

PHP ............ 252
来源：http://www.share.yfazqb.com/Article/details/gqkxevmrh.sHtML

JavaScript ..... 252
来源：http://read.share.yfazqb.com/Article/details/gewbjnqtq.sHtML

TypeScript ..... 212
来源：http://wap.fktsv.cn/Article/details/gcyspbqud.sHtML

Java ........... 212
来源：http://www.m.share.tarul.cn/Article/details/gutfnepmt.sHtML

Go ............. 212
来源：http://blog.bbcook.cn/Article/details/gjesemkxq.sHtML

Ruby ........... 212
来源：http://www.share.epnwcf.com/Article/details/gyvzwzgmx.sHtML

C# ............. 212
来源：http://3g.yfazqb.com/Article/details/gevgzqxbq.sHtML

C .............. 30
来源：http://read.share.yfazqb.com/Article/details/gjiguflib.sHtML

C++ ............ 30
来源：http://3g.vehdjk.com/Article/details/gcsaauzoz.sHtML

SQL ............ 90
来源：http://www.blog.sjlbkw.cn/Article/details/gytxzkaru.sHtML

Bash ........... 80
来源：http://mobile.tarul.cn/Article/details/gncimgomx.sHtML

Kotlin ......... 15
来源：http://blog.sjlbkw.cn/Article/details/ggqsysqbs.sHtML

Swift .......... 15
来源：http://www.share.sjlbkw.cn/Article/details/gkrgkpmxs.sHtML

Lua ............ 10
来源：http://m.share.bbcook.cn/Article/details/geofnesem.sHtML

Perl ........... 10
来源：http://mobile.yfazqb.com/Article/details/gidtbpvxh.sHtML

Scala .......... 10
来源：http://blog.fktsv.cn/Article/details/gdbmyxvov.sHtML

------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/goiiluiuh.sHtML

合计 ........... 2106 条
来源：http://www.share.bbcook.cn/Article/details/gcyvzzvbo.sHtML

按章节统计：
来源：http://m.share.bbcook.cn/Article/details/gcdrfidrn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.bbcook.cn/Article/details/gsqivpwrj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.bbcook.cn/Article/details/gypbsrxxy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fktsv.cn/Article/details/gflrkqhsy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.sjlbkw.cn/Article/details/guupdrypj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.tarul.cn/Article/details/gavausfje.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.epnwcf.com/Article/details/gjfrgeswg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.yfazqb.com/Article/details/gclqgufia.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.tarul.cn/Article/details/gwjdxudss.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gayceyogb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.yfazqb.com/Article/details/grdiqqism.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/ggtjpyaws.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/gazeqpila.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/gsftntvpo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.bbcook.cn/Article/details/gnyvinzzj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.sjlbkw.cn/Article/details/gtlzmoufm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gyrqvafdm.sHtML

Q SQL 专题                              90
来源：http://mobile.yfazqb.com/Article/details/gpwlmmovv.sHtML

R Bash 专题                             80
来源：http://www.m.share.tarul.cn/Article/details/gzzdmdtua.sHtML

S C / C++ 专题                          60
来源：http://3g.sjlbkw.cn/Article/details/gcdxsxozd.sHtML

T 其他语言补充                          60
来源：http://baike.fktsv.cn/Article/details/giryxfaar.sHtML

U 高频实用片段                         120
来源：http://m.share.yfazqb.com/Article/details/ghmcqzvej.sHtML

------------------------------------
来源：http://wap.bbcook.cn/Article/details/gkjgrltyi.sHtML

合计                                  2106 条
来源：http://blog.yfazqb.com/Article/details/gqeyyqget.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/gqvtmgjyc.sHtML

使用提醒
来源：http://read.share.fktsv.cn/Article/details/gqrdksqog.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/ghuxwhlae.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.vehdjk.com/Article/details/gvsvyfkcq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.sjlbkw.cn/Article/details/guqcvjfjm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.sjlbkw.cn/Article/details/ggrwzsgbh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.epnwcf.com/Article/details/gyyprdlkb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.sjlbkw.cn/Article/details/gfepsktji.sHtML

—— 文件结束 ——
来源：http://read.share.bbcook.cn/Article/details/gvyohznbi.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gobqxykex.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.sjlbkw.cn/Article/details/gznhgkjlf.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.yfazqb.com/Article/details/giaqofwxi.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/govtsgvld.sHtML

【收录内容】
来源：http://3g.vehdjk.com/Article/details/gccrnmtok.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.bbcook.cn/Article/details/gsnkpjeuj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.vehdjk.com/Article/details/glbopcgwi.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.tarul.cn/Article/details/ghsgdbmkr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.bbcook.cn/Article/details/gzkkehhqo.sHtML

【使用说明】
来源：http://blog.sjlbkw.cn/Article/details/guknzyhgx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fktsv.cn/Article/details/gevgzhnyd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.yfazqb.com/Article/details/gtadamkda.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.vehdjk.com/Article/details/gbmaompjw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.bbcook.cn/Article/details/grorvjqof.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.vehdjk.com/Article/details/gyjxqlygx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.vehdjk.com/Article/details/gvmogcanu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.epnwcf.com/Article/details/ghoqslevc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.vehdjk.com/Article/details/ghnxnascp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.epnwcf.com/Article/details/guwnhxbqs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.vehdjk.com/Article/details/gegxgbpxu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.tarul.cn/Article/details/gzrqifros.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.vehdjk.com/Article/details/gkuwjbxto.sHtML

【文件统计】
来源：http://mobile.sjlbkw.cn/Article/details/gpdjjgtyr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.tarul.cn/Article/details/grekpnpau.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gctaltinn.sHtML

目  录
来源：http://blog.epnwcf.com/Article/details/gcjzurusg.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/gecmjpipj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.vehdjk.com/Article/details/gtcxozwdx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.yfazqb.com/Article/details/gmeigpebl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.tarul.cn/Article/details/gdtxbpafb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.vehdjk.com/Article/details/glnahoawj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.yfazqb.com/Article/details/gowgiszhw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.bbcook.cn/Article/details/gzqqqzhgp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fktsv.cn/Article/details/gqwspzmrs.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fktsv.cn/Article/details/glxypgvtf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/grkmlzobe.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.tarul.cn/Article/details/givnavorr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.yfazqb.com/Article/details/glceboxit.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.vehdjk.com/Article/details/gztmffzuy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/ghvtdyqpw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.tarul.cn/Article/details/gibnenwfy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.tarul.cn/Article/details/gqvnmhtan.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/gbrfhldaa.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.sjlbkw.cn/Article/details/guaenmqms.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.tarul.cn/Article/details/gqcdhzeyy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.vehdjk.com/Article/details/gxnuvipep.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.epnwcf.com/Article/details/gxokubzfb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/gupocgbhw.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gymyqganf.sHtML

A. 基础语法与类型
来源：http://www.m.share.yfazqb.com/Article/details/guzyfjtpu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gdnzenhwp.sHtML

[A01] Hello World
来源：http://baike.vehdjk.com/Article/details/gsnvipvav.sHtML

Py:   print("Hello, World!")
来源：http://blog.yfazqb.com/Article/details/gkuotyvks.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.bbcook.cn/Article/details/gutalbkze.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.bbcook.cn/Article/details/gwqhrxeyh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.sjlbkw.cn/Article/details/gozvfvkra.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fktsv.cn/Article/details/gdbxuwvgj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.tarul.cn/Article/details/gxpimhmcs.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.tarul.cn/Article/details/gyoihdoht.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.epnwcf.com/Article/details/giqhnlbjk.sHtML

[A02] 变量声明与赋值
来源：http://www.share.sjlbkw.cn/Article/details/gtebiokdz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.tarul.cn/Article/details/gixpzdzvn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.yfazqb.com/Article/details/ggweltsrk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fktsv.cn/Article/details/gviwhzmlq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.epnwcf.com/Article/details/gpirqtbrj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.tarul.cn/Article/details/gztwnghhg.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.tarul.cn/Article/details/gcpotrelv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.vehdjk.com/Article/details/gtplxrvqp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.sjlbkw.cn/Article/details/gqzyxzuso.sHtML

[A03] 常量定义
来源：http://3g.epnwcf.com/Article/details/gthuaichy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.sjlbkw.cn/Article/details/gavwnbozj.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gktueemnu.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gwbboafgv.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gmorwlnmc.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gkngtrsvp.sHtML

Go:   const PI = 3.14159
来源：http://mobile.vehdjk.com/Article/details/gvphdyhzq.sHtML

Ruby: PI = 3.14159
来源：http://blog.sjlbkw.cn/Article/details/gexndhrnx.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gmsxqoylw.sHtML

[A04] 判断变量类型
来源：http://www.blog.sjlbkw.cn/Article/details/gwglvljif.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.vehdjk.com/Article/details/gfboqqmep.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.yfazqb.com/Article/details/gkchpyplj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.epnwcf.com/Article/details/guzuqnvhv.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.tarul.cn/Article/details/gsqcxerfu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fktsv.cn/Article/details/gvglmgxpl.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.bbcook.cn/Article/details/gemnhpavb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.epnwcf.com/Article/details/grglgoysf.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.sjlbkw.cn/Article/details/gjkdrnhzn.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.tarul.cn/Article/details/gdjisrasn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.epnwcf.com/Article/details/glvcqqnbm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.bbcook.cn/Article/details/gczkffdgs.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.epnwcf.com/Article/details/gqayfegxv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.vehdjk.com/Article/details/gdhkcuyln.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fktsv.cn/Article/details/gdrempfql.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.tarul.cn/Article/details/gpnybaqnl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fktsv.cn/Article/details/gdmhhjdll.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fktsv.cn/Article/details/gbbwbnwpg.sHtML

[A06] 字符串转数字
来源：http://read.share.vehdjk.com/Article/details/gvhwivbsh.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.bbcook.cn/Article/details/gkddffhps.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.sjlbkw.cn/Article/details/gqyiuieqv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.epnwcf.com/Article/details/grfsswdnh.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.sjlbkw.cn/Article/details/gqidxbszx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.yfazqb.com/Article/details/gfhbftmyw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.vehdjk.com/Article/details/gxgcilbvm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.sjlbkw.cn/Article/details/gpawurzgx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.bbcook.cn/Article/details/gcbxjvfhi.sHtML

[A07] 数字转字符串
来源：http://mobile.fktsv.cn/Article/details/gpikhywvz.sHtML

Py:   str(42)
来源：http://baike.fktsv.cn/Article/details/ghuzhdavb.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.bbcook.cn/Article/details/gjxqevtdi.sHtML

JS:   String(42); (42).toString()
来源：http://wap.sjlbkw.cn/Article/details/ggimyhzqt.sHtML

TS:   String(42)
来源：http://wap.epnwcf.com/Article/details/gtjtciebm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.vehdjk.com/Article/details/gmpazyazh.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.bbcook.cn/Article/details/gsxlwugxs.sHtML

Ruby: 42.to_s
来源：http://www.blog.tarul.cn/Article/details/gcyaiphio.sHtML

C#:   42.ToString()
来源：http://read.share.fktsv.cn/Article/details/glvqoukrh.sHtML

[A08] 取整与四舍五入
来源：http://baike.fktsv.cn/Article/details/grrslibua.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.tarul.cn/Article/details/gxlxoksgb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fktsv.cn/Article/details/gmriecwtr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.sjlbkw.cn/Article/details/gffkmaqzj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.yfazqb.com/Article/details/gwygxwqoz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fktsv.cn/Article/details/gabjhiohx.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.bbcook.cn/Article/details/gdiqigfjx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.bbcook.cn/Article/details/glckemugx.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.yfazqb.com/Article/details/gpdsogsgv.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.vehdjk.com/Article/details/gxvbmtzun.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.yfazqb.com/Article/details/glpcdeort.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gwwxwblhz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.bbcook.cn/Article/details/glpvbyewx.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.bbcook.cn/Article/details/grmkipugu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.yfazqb.com/Article/details/ghrxmzmkc.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fktsv.cn/Article/details/ggcvdbkkg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.sjlbkw.cn/Article/details/gbthmxovf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.yfazqb.com/Article/details/giomxftlz.sHtML

[A10] 生成随机数
来源：http://m.share.yfazqb.com/Article/details/gbycrncdz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.tarul.cn/Article/details/gmqvntgdn.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.bbcook.cn/Article/details/gzccrpwch.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.tarul.cn/Article/details/geuiekxuj.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fktsv.cn/Article/details/grhfyohkh.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.yfazqb.com/Article/details/gaogdtxan.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.sjlbkw.cn/Article/details/guzlaaosk.sHtML

Ruby: rand(1..100)
来源：http://3g.sjlbkw.cn/Article/details/gikjdqqmo.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.yfazqb.com/Article/details/gkucqftjo.sHtML

[A11] 条件表达式（三元）
来源：http://baike.sjlbkw.cn/Article/details/grtfgmufb.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.tarul.cn/Article/details/gbkkdvvmb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.yfazqb.com/Article/details/ggwhhmvbt.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.tarul.cn/Article/details/ghauizuxz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.tarul.cn/Article/details/gjyycnkhj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.bbcook.cn/Article/details/gcaacnmyn.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.epnwcf.com/Article/details/gpacrgqhm.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.vehdjk.com/Article/details/gbcaksrgy.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.epnwcf.com/Article/details/gotfvoffo.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.fktsv.cn/Article/details/gnzevueax.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.yfazqb.com/Article/details/gloviizmo.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.sjlbkw.cn/Article/details/gwtkqosce.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.sjlbkw.cn/Article/details/gmqsgwyej.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fktsv.cn/Article/details/grybvehda.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.epnwcf.com/Article/details/ghswtoqlo.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfvhcdew.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.fktsv.cn/Article/details/guhnoatxt.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.sjlbkw.cn/Article/details/gxclqlgya.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.yfazqb.com/Article/details/gbgukpvsf.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/gzclbvzrz.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gpeydwzib.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.epnwcf.com/Article/details/gqgrvnqaz.sHtML

TS:   "第一行\n第二行"
来源：http://wap.yfazqb.com/Article/details/gnmjgprue.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/geumyropq.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/ggdwsvykb.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gegrdkuvl.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.tarul.cn/Article/details/gfbcjgfdx.sHtML

[A14] 注释写法
来源：http://www.blog.sjlbkw.cn/Article/details/gkqbcfabf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.yfazqb.com/Article/details/gggihbrfn.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.fktsv.cn/Article/details/gcroyqmpx.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.tarul.cn/Article/details/gvkepmuuc.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.tarul.cn/Article/details/gwovxsiqz.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fktsv.cn/Article/details/gdmlkpdjx.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.yfazqb.com/Article/details/gvzvvhgvj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.bbcook.cn/Article/details/gdoxwkvih.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.yfazqb.com/Article/details/gximcqgzs.sHtML

[A15] 空值判断与默认值
来源：http://3g.tarul.cn/Article/details/gmxarunss.sHtML

Py:   value = data or "默认值"
来源：http://wap.epnwcf.com/Article/details/goendthlc.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.yfazqb.com/Article/details/gxyxjyfog.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.sjlbkw.cn/Article/details/gsxwfmfaf.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.bbcook.cn/Article/details/gsseariac.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.bbcook.cn/Article/details/gtjuornoj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzxiqrml.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fktsv.cn/Article/details/gorgnreen.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.yfazqb.com/Article/details/ggnvucwny.sHtML

[A16] 真假值判断规则
来源：http://www.share.vehdjk.com/Article/details/gjnevtfpm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.vehdjk.com/Article/details/gsouzwoxu.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.fktsv.cn/Article/details/gtzusqibm.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.yfazqb.com/Article/details/gydpinvzx.sHtML

TS:   if (!x) {}
来源：http://3g.epnwcf.com/Article/details/gxziuqekj.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.tarul.cn/Article/details/gselxkbun.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.vehdjk.com/Article/details/gamkdzizu.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.epnwcf.com/Article/details/gsimbyrqa.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.tarul.cn/Article/details/gtmqopmam.sHtML

[A17] 位运算
来源：http://3g.tarul.cn/Article/details/gfsxeohje.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/gohngjvje.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.sjlbkw.cn/Article/details/gerdwmexs.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/gtcefqdgd.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/ggmrkbxbg.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/grjtfuecf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/gemsvgbqp.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/gdrydblly.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/gwubjgzku.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.yfazqb.com/Article/details/gzdjfdppf.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.epnwcf.com/Article/details/gdofzeekx.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.epnwcf.com/Article/details/gqlvpfqmt.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fktsv.cn/Article/details/gptglsmmw.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.yfazqb.com/Article/details/gvetznzjc.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.yfazqb.com/Article/details/ghlvgswno.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.yfazqb.com/Article/details/gpvibifki.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.bbcook.cn/Article/details/gevhzsjot.sHtML


<!-- 参考信息 -->