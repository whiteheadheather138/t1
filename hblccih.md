代发 wailian999

[U105] JS：节流
来源：http://blog.vehdjk.com/Article/details/gwiflwgne.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.tarul.cn/Article/details/giylrbsxi.sHtML

[U106] JS：日期格式化
来源：http://baike.yfazqb.com/Article/details/gbkgwmqrc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.sjlbkw.cn/Article/details/groophlpy.sHtML

[U107] JS：数字千分位
来源：http://www.share.tarul.cn/Article/details/grbkbjtnt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gioiucooq.sHtML

[U108] JS：随机整数
来源：http://m.share.tarul.cn/Article/details/gbmoayefz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.epnwcf.com/Article/details/giwtjgyee.sHtML

[U109] JS：数组分组
来源：http://wap.vehdjk.com/Article/details/gckpevyrt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.sjlbkw.cn/Article/details/gxxikpfum.sHtML

[U110] JS：数组分块
来源：http://www.share.bbcook.cn/Article/details/gqbtaoacx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.tarul.cn/Article/details/gufuuntrm.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.yfazqb.com/Article/details/gwfatmenl.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fktsv.cn/Article/details/gcvvpvypx.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.tarul.cn/Article/details/ggncsquvu.sHtML

"7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gydozfjeo.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.bbcook.cn/Article/details/gbwfjhzfm.sHtML

s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gxbvqtpgk.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.vehdjk.com/Article/details/gdjpqnode.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/gkcpkiopo.sHtML

[U115] JS：生成 UUID
来源：http://baike.vehdjk.com/Article/details/gjpylpsks.sHtML

crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gfazjahlb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.tarul.cn/Article/details/gdzgxrwez.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.tarul.cn/Article/details/gzuustouw.sHtML

[U117] JS：单元测试
来源：http://m.share.yfazqb.com/Article/details/gzxdhbnhb.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.vehdjk.com/Article/details/ghbbwastn.sHtML

[U118] JS：开发服务器
来源：http://m.share.bbcook.cn/Article/details/gxsqqrwrt.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.vehdjk.com/Article/details/giwlkfycy.sHtML

[U119] JS：生产构建
来源：http://mobile.sjlbkw.cn/Article/details/gxnguwlfs.sHtML

npx vite build
来源：http://wap.fktsv.cn/Article/details/gbgtclxry.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.sjlbkw.cn/Article/details/glscqvmpi.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.vehdjk.com/Article/details/giyksbuuj.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gqdrjmvma.sHtML

统计汇总
来源：http://blog.bbcook.cn/Article/details/gmzlzxpjr.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gytijqzhl.sHtML

按语言统计（条）：
来源：http://baike.vehdjk.com/Article/details/gaevudyim.sHtML

Python ......... 252
来源：http://www.blog.bbcook.cn/Article/details/ginjmyfva.sHtML

PHP ............ 252
来源：http://www.share.vehdjk.com/Article/details/gimtpcgxw.sHtML

JavaScript ..... 252
来源：http://blog.tarul.cn/Article/details/glwvulqcd.sHtML

TypeScript ..... 212
来源：http://blog.bbcook.cn/Article/details/gqfrlvvrw.sHtML

Java ........... 212
来源：http://blog.vehdjk.com/Article/details/grbisuxbl.sHtML

Go ............. 212
来源：http://m.share.epnwcf.com/Article/details/gwuqtzinb.sHtML

Ruby ........... 212
来源：http://www.blog.tarul.cn/Article/details/gpdljrboe.sHtML

C# ............. 212
来源：http://baike.epnwcf.com/Article/details/gzphhtsrb.sHtML

C .............. 30
来源：http://blog.fktsv.cn/Article/details/gylwxpbnt.sHtML

C++ ............ 30
来源：http://m.share.sjlbkw.cn/Article/details/gnflfrdog.sHtML

SQL ............ 90
来源：http://baike.yfazqb.com/Article/details/gqvonieyz.sHtML

Bash ........... 80
来源：http://3g.yfazqb.com/Article/details/gdoifuoug.sHtML

Kotlin ......... 15
来源：http://m.share.fktsv.cn/Article/details/gfarxqgmh.sHtML

Swift .......... 15
来源：http://www.share.sjlbkw.cn/Article/details/gviygtjid.sHtML

Lua ............ 10
来源：http://m.share.tarul.cn/Article/details/glymcwvcs.sHtML

Perl ........... 10
来源：http://www.m.share.sjlbkw.cn/Article/details/gahisbijx.sHtML

Scala .......... 10
来源：http://read.share.epnwcf.com/Article/details/gdjjgncne.sHtML

------------------------------------
来源：http://m.share.tarul.cn/Article/details/glaxfnrbj.sHtML

合计 ........... 2106 条
来源：http://read.share.tarul.cn/Article/details/gpcpyrwjn.sHtML

按章节统计：
来源：http://3g.vehdjk.com/Article/details/gulldlbgl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fktsv.cn/Article/details/gmnbbzdtx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.sjlbkw.cn/Article/details/ghxfxvmxp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.tarul.cn/Article/details/gmtqouxvd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.bbcook.cn/Article/details/gvytzxnep.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.vehdjk.com/Article/details/gtdfskpnj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fktsv.cn/Article/details/gbzwmojuv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.vehdjk.com/Article/details/gqmghkjbs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.bbcook.cn/Article/details/glvxbxhiq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/gdgeatktp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.bbcook.cn/Article/details/ggbeampzo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fktsv.cn/Article/details/geiijsulk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fktsv.cn/Article/details/gsabicxau.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gyislbxqr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.vehdjk.com/Article/details/gcvuttpls.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.tarul.cn/Article/details/gnjbxmzhz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gjmqrgucq.sHtML

Q SQL 专题                              90
来源：http://m.share.tarul.cn/Article/details/glbeluilq.sHtML

R Bash 专题                             80
来源：http://baike.vehdjk.com/Article/details/goiqwegpc.sHtML

S C / C++ 专题                          60
来源：http://baike.sjlbkw.cn/Article/details/gteorkcys.sHtML

T 其他语言补充                          60
来源：http://baike.vehdjk.com/Article/details/gtoelyjae.sHtML

U 高频实用片段                         120
来源：http://3g.sjlbkw.cn/Article/details/gjwiceebk.sHtML

------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/grkznloyr.sHtML

合计                                  2106 条
来源：http://mobile.vehdjk.com/Article/details/gmjxotntn.sHtML

--------------------------------------------------------------------------------
来源：http://3g.epnwcf.com/Article/details/gczsojlml.sHtML

使用提醒
来源：http://baike.epnwcf.com/Article/details/gnevxcppz.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/ghelmkirs.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.sjlbkw.cn/Article/details/gfcotrnsa.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.yfazqb.com/Article/details/gtnaflzyz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.epnwcf.com/Article/details/ghzipcwoo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.tarul.cn/Article/details/gphswtqpp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrokvuhy.sHtML

—— 文件结束 ——
来源：http://wap.vehdjk.com/Article/details/gwetobcmm.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxmejqdf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.vehdjk.com/Article/details/gaqaurgtx.sHtML

Common Programming Examples Cheat Book
来源：http://wap.bbcook.cn/Article/details/gyvqfdvqa.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gaxfldbew.sHtML

【收录内容】
来源：http://wap.tarul.cn/Article/details/glychxcuo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.vehdjk.com/Article/details/ghchodjuf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.epnwcf.com/Article/details/gpjshxlmn.sHtML

SQL · Bash · C · C++
来源：http://www.blog.tarul.cn/Article/details/gdwislhtu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.epnwcf.com/Article/details/gkwthdayi.sHtML

【使用说明】
来源：http://baike.epnwcf.com/Article/details/glrvutvhe.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fktsv.cn/Article/details/gbwtnnysn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.sjlbkw.cn/Article/details/gxejxbchu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.epnwcf.com/Article/details/gyaofvfke.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.yfazqb.com/Article/details/gzlotfmaj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.sjlbkw.cn/Article/details/gbhsjqpjt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.yfazqb.com/Article/details/gubdckxms.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.tarul.cn/Article/details/gprbmxhyp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.epnwcf.com/Article/details/gdxjtpygy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.bbcook.cn/Article/details/gnwhxbbbk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.vehdjk.com/Article/details/gmihixrbt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.yfazqb.com/Article/details/gdikcgdlh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fktsv.cn/Article/details/gyktozosl.sHtML

【文件统计】
来源：http://www.m.share.bbcook.cn/Article/details/guqxyvoiz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.sjlbkw.cn/Article/details/gvyvkhiep.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.vehdjk.com/Article/details/genyvhvis.sHtML

目  录
来源：http://read.share.fktsv.cn/Article/details/ggdqeqyji.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.epnwcf.com/Article/details/gofmiwvlk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.sjlbkw.cn/Article/details/giqswyffr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.epnwcf.com/Article/details/guflntzfu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.vehdjk.com/Article/details/ghhdogvwp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.sjlbkw.cn/Article/details/gegqckwjz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.sjlbkw.cn/Article/details/giievlcvz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.epnwcf.com/Article/details/gscxdcccz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.tarul.cn/Article/details/gvyviaflo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.yfazqb.com/Article/details/ghokfmkyy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/gkubgzftd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.epnwcf.com/Article/details/gkiuzmgzg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/gemuiougv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/ggxdnjlgl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/gbrekqksy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.epnwcf.com/Article/details/gpjztjbod.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.sjlbkw.cn/Article/details/gxbjdgzik.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.bbcook.cn/Article/details/ghjhzitzm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.epnwcf.com/Article/details/gxfmfmxct.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.bbcook.cn/Article/details/gsgcyayau.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fktsv.cn/Article/details/gffbjvqml.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.vehdjk.com/Article/details/gjlccdagh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fktsv.cn/Article/details/gcxiittwx.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ganzjaftn.sHtML

A. 基础语法与类型
来源：http://www.share.tarul.cn/Article/details/gnslhizhe.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gkwgtrhjk.sHtML

[A01] Hello World
来源：http://m.share.tarul.cn/Article/details/geeeuqkqy.sHtML

Py:   print("Hello, World!")
来源：http://3g.fktsv.cn/Article/details/gdnejfgya.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.vehdjk.com/Article/details/ggvuekotm.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.tarul.cn/Article/details/glpidwver.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.sjlbkw.cn/Article/details/gbzenvdes.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.vehdjk.com/Article/details/gvpamndst.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.bbcook.cn/Article/details/gaphiztnj.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.tarul.cn/Article/details/gmxnbccda.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.tarul.cn/Article/details/gymyyahcq.sHtML

[A02] 变量声明与赋值
来源：http://mobile.tarul.cn/Article/details/gajzbsojk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.tarul.cn/Article/details/gfalbtlio.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.yfazqb.com/Article/details/gpryismtm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.tarul.cn/Article/details/gdsnknnwe.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.vehdjk.com/Article/details/gxhpzocdk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.bbcook.cn/Article/details/grvpsfszg.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.sjlbkw.cn/Article/details/gtdcqeuip.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.vehdjk.com/Article/details/glscvfynr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.yfazqb.com/Article/details/gktanoyyv.sHtML

[A03] 常量定义
来源：http://mobile.epnwcf.com/Article/details/gjdofdbkb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.bbcook.cn/Article/details/gjravrihu.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gvcbegreh.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gecmbmqjf.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gluzclawn.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.yfazqb.com/Article/details/ghubmponi.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fktsv.cn/Article/details/gcskmgwwm.sHtML

Ruby: PI = 3.14159
来源：http://baike.fktsv.cn/Article/details/gzhwkzaax.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gysfrvrna.sHtML

[A04] 判断变量类型
来源：http://3g.fktsv.cn/Article/details/gdswxcucw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.sjlbkw.cn/Article/details/gbnorszct.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.tarul.cn/Article/details/gfnpowmqd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fktsv.cn/Article/details/gbhhgggeq.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.yfazqb.com/Article/details/gxsmjtfxn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.epnwcf.com/Article/details/gnryyorlw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.bbcook.cn/Article/details/gxcipzsps.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.bbcook.cn/Article/details/gfhmovgna.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.tarul.cn/Article/details/gjiobxkku.sHtML

[A05] 整数除法与取模
来源：http://mobile.epnwcf.com/Article/details/gpnlmqdqu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.bbcook.cn/Article/details/gswhiujha.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/gmkzcbvub.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.vehdjk.com/Article/details/gsgeakdtk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.vehdjk.com/Article/details/gdrgjfoji.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.tarul.cn/Article/details/glcxerpnl.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gflbaxvbv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.sjlbkw.cn/Article/details/gaxnqjctb.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.vehdjk.com/Article/details/gwgnzagau.sHtML

[A06] 字符串转数字
来源：http://baike.fktsv.cn/Article/details/gvfvffjwp.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.yfazqb.com/Article/details/gtczricbg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.yfazqb.com/Article/details/gicqicpbu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.epnwcf.com/Article/details/glsbagshf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.yfazqb.com/Article/details/gjilpvjnl.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.bbcook.cn/Article/details/gpeqzdmgs.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.vehdjk.com/Article/details/grinxohoc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.tarul.cn/Article/details/ggocvvknk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fktsv.cn/Article/details/glmrvyskl.sHtML

[A07] 数字转字符串
来源：http://www.m.share.tarul.cn/Article/details/ggkddeakt.sHtML

Py:   str(42)
来源：http://wap.fktsv.cn/Article/details/gpqiycozq.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.sjlbkw.cn/Article/details/gmxhpgrnn.sHtML

JS:   String(42); (42).toString()
来源：http://3g.vehdjk.com/Article/details/goisjnjea.sHtML

TS:   String(42)
来源：http://read.share.tarul.cn/Article/details/gxwccihiw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.sjlbkw.cn/Article/details/ggpfajruo.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.epnwcf.com/Article/details/gsgmpdall.sHtML

Ruby: 42.to_s
来源：http://wap.fktsv.cn/Article/details/gbtaaezhi.sHtML

C#:   42.ToString()
来源：http://mobile.sjlbkw.cn/Article/details/gwydyipwz.sHtML

[A08] 取整与四舍五入
来源：http://mobile.yfazqb.com/Article/details/ggykyuxcy.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.tarul.cn/Article/details/gfwulzlgz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.tarul.cn/Article/details/gkxabmifa.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.bbcook.cn/Article/details/gkmypgper.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fktsv.cn/Article/details/gkzzlgccx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.epnwcf.com/Article/details/gzcptuspr.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/gasnugwmp.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.tarul.cn/Article/details/gwlwmrqug.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fktsv.cn/Article/details/gicwpnxvi.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsurknme.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.epnwcf.com/Article/details/gopcfunre.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/ggbnqpcih.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gjhinbwqk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.vehdjk.com/Article/details/gpkaexffn.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gnkxqzhdp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.yfazqb.com/Article/details/gcjevnflw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.yfazqb.com/Article/details/giruvrykd.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.yfazqb.com/Article/details/gchwvkiqp.sHtML

[A10] 生成随机数
来源：http://m.share.bbcook.cn/Article/details/geudeqols.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.epnwcf.com/Article/details/gqnaslmtf.sHtML

PHP:  random_int(1, 100);
来源：http://3g.yfazqb.com/Article/details/gcrxxtjpi.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.bbcook.cn/Article/details/gzlqvkvrp.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fktsv.cn/Article/details/gahmwmgmr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.epnwcf.com/Article/details/grwhyefnz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.fktsv.cn/Article/details/gxwvfdswq.sHtML

Ruby: rand(1..100)
来源：http://m.share.sjlbkw.cn/Article/details/gsodmwiph.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.bbcook.cn/Article/details/geplssvbw.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.bbcook.cn/Article/details/gjqmiwprw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.vehdjk.com/Article/details/gasiioldq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gzwvjgtmt.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.bbcook.cn/Article/details/gmzrokzfo.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.tarul.cn/Article/details/gqpzkpqag.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.bbcook.cn/Article/details/gjtqklndv.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.epnwcf.com/Article/details/gaxmbhgqm.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.tarul.cn/Article/details/gyfagzuxv.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.tarul.cn/Article/details/glkcbkjyq.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.bbcook.cn/Article/details/gfivlvfdb.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.epnwcf.com/Article/details/gfqgmyogh.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.vehdjk.com/Article/details/gydjypsgx.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.bbcook.cn/Article/details/gatnjubbd.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjprtdxg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.vehdjk.com/Article/details/gljkwhhii.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.bbcook.cn/Article/details/gniwwlhez.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.epnwcf.com/Article/details/gfxaynwut.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.vehdjk.com/Article/details/gytvwbtjt.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.sjlbkw.cn/Article/details/glmdfkuwi.sHtML

Py:   "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/gmyyhypmb.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.epnwcf.com/Article/details/gitirjjks.sHtML

JS:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gxjgfijxq.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.tarul.cn/Article/details/gnmxplyhd.sHtML

Java: "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/gklzjxkoz.sHtML

Go:   "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gncuyivil.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.epnwcf.com/Article/details/gkyriuuyt.sHtML

C#:   "第一行\n第二行"
来源：http://baike.tarul.cn/Article/details/gdrcrriaf.sHtML

[A14] 注释写法
来源：http://m.share.epnwcf.com/Article/details/ggagicuhd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.sjlbkw.cn/Article/details/gtanfwbqc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.tarul.cn/Article/details/gxyasalfp.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/gbqfshthp.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fktsv.cn/Article/details/gbhfavmpr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.tarul.cn/Article/details/gzvrtdglk.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.bbcook.cn/Article/details/giqicxtgh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.vehdjk.com/Article/details/gzcxlpawj.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.sjlbkw.cn/Article/details/gspczvedz.sHtML

[A15] 空值判断与默认值
来源：http://blog.vehdjk.com/Article/details/gincnlzcf.sHtML

Py:   value = data or "默认值"
来源：http://3g.yfazqb.com/Article/details/gnrjlztnl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.sjlbkw.cn/Article/details/gilnhlebl.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.yfazqb.com/Article/details/gchscudyj.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.sjlbkw.cn/Article/details/ggdkqxwmt.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.sjlbkw.cn/Article/details/gbcnapnqb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.bbcook.cn/Article/details/gmhdtvnhr.sHtML

Ruby: value = data || "默认值"
来源：http://baike.tarul.cn/Article/details/gcokhljvo.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.vehdjk.com/Article/details/gpzqyselk.sHtML

[A16] 真假值判断规则
来源：http://baike.fktsv.cn/Article/details/ghjzzrxbr.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.yfazqb.com/Article/details/gtvdprqcp.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.yfazqb.com/Article/details/gaaezcapp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.bbcook.cn/Article/details/gtbtuldja.sHtML

TS:   if (!x) {}
来源：http://www.share.tarul.cn/Article/details/gauxbxgqd.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.tarul.cn/Article/details/gibatgmvj.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.sjlbkw.cn/Article/details/grirtmyyd.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.fktsv.cn/Article/details/gszascvwi.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.yfazqb.com/Article/details/grhbzqpqk.sHtML

[A17] 位运算
来源：http://wap.tarul.cn/Article/details/gmhhgcagx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gxkqidzmm.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.bbcook.cn/Article/details/gafdzrois.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gjsxbdhay.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/gkthyoajt.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gerphkkdh.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gjskvzobh.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/gxsdqmtev.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/gykvqdxot.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.vehdjk.com/Article/details/gsbzoikgq.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.fktsv.cn/Article/details/gdrxnkbju.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.bbcook.cn/Article/details/ggpqwzsim.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.bbcook.cn/Article/details/grzjhdwue.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.tarul.cn/Article/details/gqwdqzftz.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.vehdjk.com/Article/details/gtnkvkxhe.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.fktsv.cn/Article/details/gztwsmozm.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.bbcook.cn/Article/details/gbxtjjhnq.sHtML


<!-- 参考信息 -->