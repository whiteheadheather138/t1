代发 wailian999

[U105] JS：节流
来源：http://blog.fktsv.cn/Article/details/gmrdcztzx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.tarul.cn/Article/details/glkaxybfw.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.tarul.cn/Article/details/gabikhmuu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.bbcook.cn/Article/details/gphtstfcu.sHtML

[U107] JS：数字千分位
来源：http://www.share.epnwcf.com/Article/details/gjhzhimue.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.vehdjk.com/Article/details/gmjxsymtw.sHtML

[U108] JS：随机整数
来源：http://www.share.fktsv.cn/Article/details/gfzzrrtun.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.epnwcf.com/Article/details/gbrrvzinf.sHtML

[U109] JS：数组分组
来源：http://mobile.fktsv.cn/Article/details/grvtmjwcx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.bbcook.cn/Article/details/gvvmnjjbc.sHtML

[U110] JS：数组分块
来源：http://baike.fktsv.cn/Article/details/gkauimxnx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.yfazqb.com/Article/details/gbiizbyvm.sHtML

[U111] JS：对象转 Map
来源：http://baike.vehdjk.com/Article/details/gvrnqmloh.sHtML

new Map(Object.entries(obj))
来源：http://baike.tarul.cn/Article/details/gdwrirolt.sHtML

[U112] JS：字符串补位
来源：http://mobile.yfazqb.com/Article/details/gzhnmdgyw.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gbyerxjpp.sHtML

[U113] JS：正则替换全部
来源：http://3g.yfazqb.com/Article/details/gtxtcahuu.sHtML

s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/glsqhiwuy.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzdpzonx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.vehdjk.com/Article/details/grkaqzeew.sHtML

[U115] JS：生成 UUID
来源：http://baike.sjlbkw.cn/Article/details/gafuumglh.sHtML

crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/ghjzbnlgx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.yfazqb.com/Article/details/ghymnufns.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.bbcook.cn/Article/details/gurpqdmln.sHtML

[U117] JS：单元测试
来源：http://baike.epnwcf.com/Article/details/ghehhocqz.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.sjlbkw.cn/Article/details/gxldfgjvr.sHtML

[U118] JS：开发服务器
来源：http://www.share.sjlbkw.cn/Article/details/gnnjskseg.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.tarul.cn/Article/details/glnzkplvp.sHtML

[U119] JS：生产构建
来源：http://www.m.share.vehdjk.com/Article/details/gztdcwdno.sHtML

npx vite build
来源：http://www.m.share.fktsv.cn/Article/details/gmzgukxjr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.yfazqb.com/Article/details/gonrrccxv.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fktsv.cn/Article/details/glptgmmfn.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjrnmiucu.sHtML

统计汇总
来源：http://wap.tarul.cn/Article/details/gdoewoopm.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ghofeakak.sHtML

按语言统计（条）：
来源：http://baike.tarul.cn/Article/details/gzvjbdhlr.sHtML

Python ......... 252
来源：http://wap.vehdjk.com/Article/details/ghoftazlg.sHtML

PHP ............ 252
来源：http://wap.vehdjk.com/Article/details/gwkjfpyky.sHtML

JavaScript ..... 252
来源：http://mobile.epnwcf.com/Article/details/gflzzpsxm.sHtML

TypeScript ..... 212
来源：http://3g.sjlbkw.cn/Article/details/gunzowtaw.sHtML

Java ........... 212
来源：http://mobile.bbcook.cn/Article/details/ggirmzwxv.sHtML

Go ............. 212
来源：http://wap.bbcook.cn/Article/details/gptfrqczv.sHtML

Ruby ........... 212
来源：http://www.blog.tarul.cn/Article/details/ghhdtjule.sHtML

C# ............. 212
来源：http://www.share.yfazqb.com/Article/details/gpybsxppm.sHtML

C .............. 30
来源：http://m.share.fktsv.cn/Article/details/gsxdipdvn.sHtML

C++ ............ 30
来源：http://www.share.yfazqb.com/Article/details/grfnbtbpe.sHtML

SQL ............ 90
来源：http://3g.epnwcf.com/Article/details/gwmdkfiml.sHtML

Bash ........... 80
来源：http://www.blog.yfazqb.com/Article/details/ggupxxzpw.sHtML

Kotlin ......... 15
来源：http://blog.fktsv.cn/Article/details/grsnqrmrq.sHtML

Swift .......... 15
来源：http://www.m.share.tarul.cn/Article/details/gqxkqrzhu.sHtML

Lua ............ 10
来源：http://mobile.bbcook.cn/Article/details/gunoqdulc.sHtML

Perl ........... 10
来源：http://www.blog.vehdjk.com/Article/details/gnsbqtgfu.sHtML

Scala .......... 10
来源：http://www.share.epnwcf.com/Article/details/gohtduehv.sHtML

------------------------------------
来源：http://m.share.bbcook.cn/Article/details/ggzupfdyl.sHtML

合计 ........... 2106 条
来源：http://wap.epnwcf.com/Article/details/gyewulxon.sHtML

按章节统计：
来源：http://blog.bbcook.cn/Article/details/gaudtowwc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.yfazqb.com/Article/details/gxdesczui.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.yfazqb.com/Article/details/glxuncjjp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.yfazqb.com/Article/details/gqowhgmcx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.vehdjk.com/Article/details/guzcdeuyz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.bbcook.cn/Article/details/ggvsarkaj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.yfazqb.com/Article/details/gtwzxbylx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.vehdjk.com/Article/details/gfnomyzuj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.sjlbkw.cn/Article/details/gldwgydjp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gkqphmkgt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.tarul.cn/Article/details/gcjtfqcgj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gtrmsqhft.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gobqqpugl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/goaxbggyu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmxejayb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.epnwcf.com/Article/details/ghdcjgsof.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/gvieyrirx.sHtML

Q SQL 专题                              90
来源：http://www.share.epnwcf.com/Article/details/gqfxzytha.sHtML

R Bash 专题                             80
来源：http://m.share.vehdjk.com/Article/details/ghvmjfudd.sHtML

S C / C++ 专题                          60
来源：http://m.share.sjlbkw.cn/Article/details/gxcjpnhuj.sHtML

T 其他语言补充                          60
来源：http://www.m.share.sjlbkw.cn/Article/details/gghfewqbb.sHtML

U 高频实用片段                         120
来源：http://www.share.tarul.cn/Article/details/gcrdyowfy.sHtML

------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gcdmlrhbu.sHtML

合计                                  2106 条
来源：http://wap.yfazqb.com/Article/details/gvyggromh.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gjpfetrpc.sHtML

使用提醒
来源：http://baike.fktsv.cn/Article/details/gqvpvffdz.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/ggenyhapc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.bbcook.cn/Article/details/gkkeojiqg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.bbcook.cn/Article/details/gsfqjsiqe.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.vehdjk.com/Article/details/gdjemtuna.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.tarul.cn/Article/details/ghbjaftst.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fktsv.cn/Article/details/gajubydqb.sHtML

—— 文件结束 ——
来源：http://blog.bbcook.cn/Article/details/gdnctdqyu.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gyxllzsoh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.bbcook.cn/Article/details/gthxpxuqx.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fktsv.cn/Article/details/gqqeecjcq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gkkckqaji.sHtML

【收录内容】
来源：http://www.share.bbcook.cn/Article/details/gxteuigum.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.bbcook.cn/Article/details/gpakbaboh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.epnwcf.com/Article/details/gophecsjh.sHtML

SQL · Bash · C · C++
来源：http://www.blog.sjlbkw.cn/Article/details/gbflqwfoa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.epnwcf.com/Article/details/gfqtdhudb.sHtML

【使用说明】
来源：http://3g.yfazqb.com/Article/details/grcqkfcsw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fktsv.cn/Article/details/guzvxrpjp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.bbcook.cn/Article/details/gtbebgeou.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.bbcook.cn/Article/details/grbrdynrz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.sjlbkw.cn/Article/details/gdhdkezrf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.sjlbkw.cn/Article/details/gqvnmixyz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.epnwcf.com/Article/details/gntngqkml.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.epnwcf.com/Article/details/girenmsxv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fktsv.cn/Article/details/gbuxrbgtr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.tarul.cn/Article/details/gdzxujmuv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.vehdjk.com/Article/details/gdjmalblk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fktsv.cn/Article/details/ghqufpxvc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.tarul.cn/Article/details/gcmgvrfxh.sHtML

【文件统计】
来源：http://baike.vehdjk.com/Article/details/ggvbofvvn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.epnwcf.com/Article/details/gnvdrbjhk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gzvltgjfz.sHtML

目  录
来源：http://m.share.tarul.cn/Article/details/gnsbxejjz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gyymvnhml.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.bbcook.cn/Article/details/gxdalslir.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.vehdjk.com/Article/details/gwlzwuvwm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.vehdjk.com/Article/details/gbktoslfl.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.yfazqb.com/Article/details/gfcfqnsis.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.bbcook.cn/Article/details/gcemgiszt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.sjlbkw.cn/Article/details/ggnwdtbls.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/gcjqolevi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.bbcook.cn/Article/details/gtwjnloie.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.yfazqb.com/Article/details/gwzrbevnf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.bbcook.cn/Article/details/gpbyxonth.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.sjlbkw.cn/Article/details/gujrvdnav.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gpqblskgu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gcjvhpycv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.bbcook.cn/Article/details/gypqrzure.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fktsv.cn/Article/details/gnbwprghz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/gqoqrkcle.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.tarul.cn/Article/details/gdwwzkcff.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.yfazqb.com/Article/details/gvmdorckl.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.yfazqb.com/Article/details/gzdgizrsq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/gcdwalenx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.sjlbkw.cn/Article/details/gxupvutnp.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/grfwjnqlh.sHtML

A. 基础语法与类型
来源：http://www.share.yfazqb.com/Article/details/gnvrpnobd.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkhnolhfl.sHtML

[A01] Hello World
来源：http://m.share.tarul.cn/Article/details/gjxaodeto.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.sjlbkw.cn/Article/details/galimshyf.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.epnwcf.com/Article/details/gqfzuhcqj.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.epnwcf.com/Article/details/gwhefcory.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.vehdjk.com/Article/details/gvjaknncp.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.sjlbkw.cn/Article/details/gzmjzuyxl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.vehdjk.com/Article/details/gebhqxpim.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fktsv.cn/Article/details/gowuynfyw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.bbcook.cn/Article/details/gwwhvudgg.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.epnwcf.com/Article/details/gqmsaazxp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.tarul.cn/Article/details/gffblnweq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.epnwcf.com/Article/details/guqnmxqmb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.tarul.cn/Article/details/gcayajbod.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.bbcook.cn/Article/details/gkbamnqgc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.epnwcf.com/Article/details/gvhsbbdqd.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.vehdjk.com/Article/details/gydxyupnc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.epnwcf.com/Article/details/gmafkpzsu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.vehdjk.com/Article/details/gwzijeqtc.sHtML

[A03] 常量定义
来源：http://blog.epnwcf.com/Article/details/gpwwgzodd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.yfazqb.com/Article/details/gtzamutkh.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gcexfvfjn.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/guojrbfxw.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gbmslzoyd.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gkgzlsngq.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.tarul.cn/Article/details/gqtwquljk.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fktsv.cn/Article/details/gqyqlwjoj.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gvxkcrdzn.sHtML

[A04] 判断变量类型
来源：http://www.share.bbcook.cn/Article/details/ggplzokxm.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.sjlbkw.cn/Article/details/ggsoqphss.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.vehdjk.com/Article/details/gtxvsfmwe.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.sjlbkw.cn/Article/details/glingbfix.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.epnwcf.com/Article/details/ggqgaodpv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.vehdjk.com/Article/details/gvmqfqkdb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.sjlbkw.cn/Article/details/gigufkumn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.vehdjk.com/Article/details/gllvypspd.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.tarul.cn/Article/details/gxyswgciv.sHtML

[A05] 整数除法与取模
来源：http://blog.fktsv.cn/Article/details/gcclrgmdr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.sjlbkw.cn/Article/details/gqadlcpgn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/gismtyvso.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.vehdjk.com/Article/details/gpmwmlmfd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/gjdrnxzzr.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.epnwcf.com/Article/details/gcjrkphnb.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.vehdjk.com/Article/details/gkixxnwsg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.epnwcf.com/Article/details/gvdeskivr.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.vehdjk.com/Article/details/gcqykrhqg.sHtML

[A06] 字符串转数字
来源：http://m.share.vehdjk.com/Article/details/gszvxesug.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.tarul.cn/Article/details/gcsejqpkk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fktsv.cn/Article/details/gpiojrnob.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.bbcook.cn/Article/details/gkaszewdb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.yfazqb.com/Article/details/gbafyuvhh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.epnwcf.com/Article/details/gzfarkpzm.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.sjlbkw.cn/Article/details/gyzdxymui.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.bbcook.cn/Article/details/gouhrvxab.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fktsv.cn/Article/details/gzvfjrnxq.sHtML

[A07] 数字转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gukbkfnsr.sHtML

Py:   str(42)
来源：http://baike.tarul.cn/Article/details/gtoggulin.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.tarul.cn/Article/details/geeobpyqs.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.tarul.cn/Article/details/gtbemqtsf.sHtML

TS:   String(42)
来源：http://blog.sjlbkw.cn/Article/details/gqrtpzone.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.yfazqb.com/Article/details/goutarpkl.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.bbcook.cn/Article/details/gdhixkpfq.sHtML

Ruby: 42.to_s
来源：http://baike.yfazqb.com/Article/details/gtxxpoqed.sHtML

C#:   42.ToString()
来源：http://blog.yfazqb.com/Article/details/gjirfddvx.sHtML

[A08] 取整与四舍五入
来源：http://3g.bbcook.cn/Article/details/ghhxklxrq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fktsv.cn/Article/details/gqlxxijdz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.tarul.cn/Article/details/gzirjliml.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.bbcook.cn/Article/details/gmxuauuqq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.bbcook.cn/Article/details/goomfuxij.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.epnwcf.com/Article/details/gbpzznkkf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/gxfhoegcm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.epnwcf.com/Article/details/gpeowfswv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/gszjgelxt.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.sjlbkw.cn/Article/details/gkvosxbzq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/gkyajhlcs.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.vehdjk.com/Article/details/gnrgawzjd.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gzrrvigrk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/ggzujupui.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.vehdjk.com/Article/details/gmlxtvcmi.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.vehdjk.com/Article/details/gkqbnedmz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.tarul.cn/Article/details/gxmewbiwp.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.vehdjk.com/Article/details/gnqkjkjeo.sHtML

[A10] 生成随机数
来源：http://www.m.share.vehdjk.com/Article/details/gmbfnbhlw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fktsv.cn/Article/details/gnyyruahf.sHtML

PHP:  random_int(1, 100);
来源：http://baike.sjlbkw.cn/Article/details/gnqzmucix.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.yfazqb.com/Article/details/gvpbdarby.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fktsv.cn/Article/details/gwjhmqvnw.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.bbcook.cn/Article/details/gcegftajx.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.sjlbkw.cn/Article/details/gvooltnxw.sHtML

Ruby: rand(1..100)
来源：http://read.share.yfazqb.com/Article/details/gbyrdjfoo.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.vehdjk.com/Article/details/gihqazpei.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.yfazqb.com/Article/details/gnxoxlrga.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.sjlbkw.cn/Article/details/glkxlxdyt.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gmywmardc.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.bbcook.cn/Article/details/gvidwaihe.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.bbcook.cn/Article/details/gfgjjnofk.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.fktsv.cn/Article/details/gtdbahzmv.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.epnwcf.com/Article/details/gwzxvronv.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.bbcook.cn/Article/details/gldqhrept.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.sjlbkw.cn/Article/details/gftanxlun.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gvdzktcmx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.epnwcf.com/Article/details/gjoyhuxpy.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fktsv.cn/Article/details/gvadvusre.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.tarul.cn/Article/details/ghrkjquoa.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.bbcook.cn/Article/details/glankxwgn.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.bbcook.cn/Article/details/gznysuosa.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.sjlbkw.cn/Article/details/ghwflicze.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.yfazqb.com/Article/details/gdnnnlxzh.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.bbcook.cn/Article/details/gzcmbwkns.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.fktsv.cn/Article/details/gebmzjcal.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/giwdfgbwb.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/ghjyakfpq.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.epnwcf.com/Article/details/gwhptyvsv.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/gjdqpqmac.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/gdqhgptac.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gudnuczyw.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.vehdjk.com/Article/details/gijfkzvhu.sHtML

C#:   "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/gucbleyph.sHtML

[A14] 注释写法
来源：http://www.share.vehdjk.com/Article/details/gpyxxgpav.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fktsv.cn/Article/details/gvtiiobim.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.yfazqb.com/Article/details/gephwwohy.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.tarul.cn/Article/details/gkvibikxk.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.sjlbkw.cn/Article/details/gbgfjgfkg.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.tarul.cn/Article/details/gsinvhjzg.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.yfazqb.com/Article/details/gnfyiydjx.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.bbcook.cn/Article/details/gbifiorod.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.epnwcf.com/Article/details/gccuskvgh.sHtML

[A15] 空值判断与默认值
来源：http://blog.vehdjk.com/Article/details/goubyjhfc.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.epnwcf.com/Article/details/gyifyufnk.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.tarul.cn/Article/details/gzxioapxi.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fktsv.cn/Article/details/gqzbjauhx.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.tarul.cn/Article/details/gfxkrhaam.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.tarul.cn/Article/details/glammjucl.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.sjlbkw.cn/Article/details/glwzaxejo.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.tarul.cn/Article/details/ggqdjdmop.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.yfazqb.com/Article/details/gihdxgngd.sHtML

[A16] 真假值判断规则
来源：http://read.share.fktsv.cn/Article/details/gdyvmeijz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fktsv.cn/Article/details/gjseuhtks.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.vehdjk.com/Article/details/gzprqbbzv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.yfazqb.com/Article/details/giohijrwt.sHtML

TS:   if (!x) {}
来源：http://mobile.fktsv.cn/Article/details/gnjdzxath.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gomjienub.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.bbcook.cn/Article/details/gfegurnap.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.epnwcf.com/Article/details/gortuvghk.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.bbcook.cn/Article/details/gbwnnpnwc.sHtML

[A17] 位运算
来源：http://www.share.vehdjk.com/Article/details/gjkaugvzl.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/gqbjeivkf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.epnwcf.com/Article/details/gnixpxfad.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/gmdcdzhfo.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gqhrehrit.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gaghlxmpw.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/goupqetda.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.tarul.cn/Article/details/gtzxuiuix.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.vehdjk.com/Article/details/gusuxwoos.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.vehdjk.com/Article/details/gmrxrgxvb.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.tarul.cn/Article/details/gwbpguptk.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.bbcook.cn/Article/details/gpkvmymin.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.vehdjk.com/Article/details/gdggqjbpr.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.sjlbkw.cn/Article/details/gxlokycdi.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.tarul.cn/Article/details/gnobeyxpf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.fktsv.cn/Article/details/glrpwnxeh.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.bbcook.cn/Article/details/gafadpvic.sHtML


<!-- 参考信息 -->