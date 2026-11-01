代发 wailian999

[U105] JS：节流
来源：http://3g.bbcook.cn/Article/details/gyaarnvlc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.sjlbkw.cn/Article/details/gnuypywme.sHtML

[U106] JS：日期格式化
来源：http://read.share.yfazqb.com/Article/details/gowbcrbwl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.sjlbkw.cn/Article/details/geciuizhi.sHtML

[U107] JS：数字千分位
来源：http://m.share.tarul.cn/Article/details/grrdhycbr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.yfazqb.com/Article/details/ghyokeeje.sHtML

[U108] JS：随机整数
来源：http://www.blog.sjlbkw.cn/Article/details/gmcktkcqp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.bbcook.cn/Article/details/gwxrzmrbq.sHtML

[U109] JS：数组分组
来源：http://blog.tarul.cn/Article/details/gnfloyngn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.sjlbkw.cn/Article/details/gonswrsdn.sHtML

[U110] JS：数组分块
来源：http://read.share.sjlbkw.cn/Article/details/gqthftogs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.yfazqb.com/Article/details/gtttvngct.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.tarul.cn/Article/details/gnqoyrcqx.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.vehdjk.com/Article/details/guiytcift.sHtML

[U112] JS：字符串补位
来源：http://baike.bbcook.cn/Article/details/graliqsmt.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/grtptqqxk.sHtML

[U113] JS：正则替换全部
来源：http://blog.epnwcf.com/Article/details/gxshyqozo.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/goytubyzx.sHtML

[U114] JS：JSON 深比较
来源：http://wap.bbcook.cn/Article/details/gmzmdizsm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fktsv.cn/Article/details/gkdehalai.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.epnwcf.com/Article/details/guqkgfzol.sHtML

crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/gbstfsgfi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.vehdjk.com/Article/details/glgpmsfgr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fktsv.cn/Article/details/ghreudryu.sHtML

[U117] JS：单元测试
来源：http://m.share.fktsv.cn/Article/details/gnhwjvplf.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.epnwcf.com/Article/details/gjuonzrlj.sHtML

[U118] JS：开发服务器
来源：http://read.share.fktsv.cn/Article/details/gnbydwdyo.sHtML

npm i -D vite;  npx vite
来源：http://baike.tarul.cn/Article/details/gijetjggd.sHtML

[U119] JS：生产构建
来源：http://3g.sjlbkw.cn/Article/details/gzkhwavqi.sHtML

npx vite build
来源：http://www.m.share.bbcook.cn/Article/details/gkosqrvvj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.vehdjk.com/Article/details/glqtrzkun.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.epnwcf.com/Article/details/gabyuqydf.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/glcpisjvc.sHtML

统计汇总
来源：http://m.share.bbcook.cn/Article/details/gslbbqvhw.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gtfzldiph.sHtML

按语言统计（条）：
来源：http://blog.epnwcf.com/Article/details/gzgyyrbvi.sHtML

Python ......... 252
来源：http://m.share.fktsv.cn/Article/details/gbeiajypv.sHtML

PHP ............ 252
来源：http://wap.sjlbkw.cn/Article/details/gmebaxsle.sHtML

JavaScript ..... 252
来源：http://baike.sjlbkw.cn/Article/details/gqzhzsyhu.sHtML

TypeScript ..... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjddlvaf.sHtML

Java ........... 212
来源：http://blog.epnwcf.com/Article/details/ggfhuknbt.sHtML

Go ............. 212
来源：http://mobile.fktsv.cn/Article/details/ggfklyuup.sHtML

Ruby ........... 212
来源：http://read.share.fktsv.cn/Article/details/gxjdiikru.sHtML

C# ............. 212
来源：http://mobile.fktsv.cn/Article/details/gptkkcdyi.sHtML

C .............. 30
来源：http://blog.yfazqb.com/Article/details/gotuhrfua.sHtML

C++ ............ 30
来源：http://blog.tarul.cn/Article/details/gvmblooun.sHtML

SQL ............ 90
来源：http://blog.yfazqb.com/Article/details/glyphwglt.sHtML

Bash ........... 80
来源：http://www.share.epnwcf.com/Article/details/gfdshzwrd.sHtML

Kotlin ......... 15
来源：http://mobile.sjlbkw.cn/Article/details/gvewipyce.sHtML

Swift .......... 15
来源：http://www.blog.bbcook.cn/Article/details/gibqkauxi.sHtML

Lua ............ 10
来源：http://www.share.epnwcf.com/Article/details/glwxavzbe.sHtML

Perl ........... 10
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxxqxdvl.sHtML

Scala .......... 10
来源：http://www.blog.epnwcf.com/Article/details/gpsdzazfv.sHtML

------------------------------------
来源：http://blog.fktsv.cn/Article/details/gnmclsigk.sHtML

合计 ........... 2106 条
来源：http://m.share.fktsv.cn/Article/details/gqzedcqso.sHtML

按章节统计：
来源：http://read.share.epnwcf.com/Article/details/gitfxqakz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.bbcook.cn/Article/details/govhizlde.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.sjlbkw.cn/Article/details/gnfgpmrfs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.tarul.cn/Article/details/gdkevhipl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.bbcook.cn/Article/details/gmpfqsith.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.epnwcf.com/Article/details/gphpkujco.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.epnwcf.com/Article/details/govksmwjl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.vehdjk.com/Article/details/gltzbdlaq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.vehdjk.com/Article/details/gtjqvbvdh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/glkqdtpgh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.vehdjk.com/Article/details/gtxvrzeyu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/gbgzxjkkk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gecpchovy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/gckrrisze.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.sjlbkw.cn/Article/details/grxgukbjz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fktsv.cn/Article/details/gwskubnsg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/gljinfwio.sHtML

Q SQL 专题                              90
来源：http://baike.vehdjk.com/Article/details/gdhcgfjzx.sHtML

R Bash 专题                             80
来源：http://blog.tarul.cn/Article/details/gqekecywf.sHtML

S C / C++ 专题                          60
来源：http://wap.vehdjk.com/Article/details/gxtvmyken.sHtML

T 其他语言补充                          60
来源：http://baike.bbcook.cn/Article/details/grysdlbqg.sHtML

U 高频实用片段                         120
来源：http://baike.bbcook.cn/Article/details/gxuhhjghx.sHtML

------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gqomxlobw.sHtML

合计                                  2106 条
来源：http://wap.vehdjk.com/Article/details/ghhtrlcbq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.tarul.cn/Article/details/gwgmryrbg.sHtML

使用提醒
来源：http://www.m.share.yfazqb.com/Article/details/gzzdkiakn.sHtML

--------------------------------------------------------------------------------
来源：http://3g.yfazqb.com/Article/details/gcnnhumtt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.yfazqb.com/Article/details/gntevgvss.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fktsv.cn/Article/details/gnmmgoeqr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.vehdjk.com/Article/details/gbqztbfqg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.sjlbkw.cn/Article/details/gjvjqatws.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.tarul.cn/Article/details/gbanvmdoz.sHtML

—— 文件结束 ——
来源：http://m.share.tarul.cn/Article/details/gjgdenjhf.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gkaxlrrpt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fktsv.cn/Article/details/grlqktorf.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.tarul.cn/Article/details/gpoqinlvj.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gkkzvpyqv.sHtML

【收录内容】
来源：http://read.share.bbcook.cn/Article/details/genimhgui.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.bbcook.cn/Article/details/gcbalaeey.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.epnwcf.com/Article/details/gcomlrazk.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.tarul.cn/Article/details/ghugcqtox.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.bbcook.cn/Article/details/gshnswdpf.sHtML

【使用说明】
来源：http://wap.vehdjk.com/Article/details/gduxsbvhc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fktsv.cn/Article/details/gymufwwjf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.vehdjk.com/Article/details/gxrzdjyqq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.vehdjk.com/Article/details/gbfmnblak.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fktsv.cn/Article/details/gctuxkjvu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.sjlbkw.cn/Article/details/guoeggnkd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fktsv.cn/Article/details/gyshvgnmw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.vehdjk.com/Article/details/gbgvndziv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.sjlbkw.cn/Article/details/ggbqrachu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.tarul.cn/Article/details/gvrtdnihb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.vehdjk.com/Article/details/gfnpbywea.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.tarul.cn/Article/details/gbztoqdcg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fktsv.cn/Article/details/gftjgoicr.sHtML

【文件统计】
来源：http://www.blog.yfazqb.com/Article/details/gwgohdsjy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.bbcook.cn/Article/details/grelfogja.sHtML

--------------------------------------------------------------------------------
来源：http://wap.vehdjk.com/Article/details/gypcauevj.sHtML

目  录
来源：http://read.share.sjlbkw.cn/Article/details/gfyaweuuu.sHtML

--------------------------------------------------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/grzkwprzp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fktsv.cn/Article/details/gtpxdgvbw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.sjlbkw.cn/Article/details/gomtwafek.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fktsv.cn/Article/details/gzbciyhfc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fktsv.cn/Article/details/gessqjsux.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.epnwcf.com/Article/details/ghwxgttuh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.vehdjk.com/Article/details/gmlzpavna.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fktsv.cn/Article/details/geuqsvbdd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.vehdjk.com/Article/details/gjutoopta.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/gacpsazua.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.tarul.cn/Article/details/gxysqicnc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/gvzzoupip.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fktsv.cn/Article/details/gqjfeefqi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.tarul.cn/Article/details/gwecohdhi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.tarul.cn/Article/details/gbyhmhake.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.vehdjk.com/Article/details/gmuwtawsl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/gsvqkeiqz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.sjlbkw.cn/Article/details/giujnogtv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.epnwcf.com/Article/details/gluwduwse.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.vehdjk.com/Article/details/gpodpprnx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.epnwcf.com/Article/details/gapnggbut.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.tarul.cn/Article/details/gbbagzgjs.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gobdqawgo.sHtML

A. 基础语法与类型
来源：http://www.blog.bbcook.cn/Article/details/ggokwallp.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gepickvsl.sHtML

[A01] Hello World
来源：http://3g.yfazqb.com/Article/details/gfvflkinm.sHtML

Py:   print("Hello, World!")
来源：http://3g.epnwcf.com/Article/details/ggwexnfac.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.vehdjk.com/Article/details/gxceijuow.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.vehdjk.com/Article/details/gjhpydnqv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.epnwcf.com/Article/details/gmfxnkobu.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.bbcook.cn/Article/details/gbcxcjclx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.yfazqb.com/Article/details/gljcxuewn.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.sjlbkw.cn/Article/details/gevoklrwz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fktsv.cn/Article/details/grszwamgb.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.yfazqb.com/Article/details/gyewtjfbs.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.yfazqb.com/Article/details/ghcfwraon.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.bbcook.cn/Article/details/grtzwejph.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/geapskava.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpgsqaut.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gefafiksi.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.tarul.cn/Article/details/gvpnbigoh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.yfazqb.com/Article/details/gllhwxdro.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gauxaovpl.sHtML

[A03] 常量定义
来源：http://mobile.yfazqb.com/Article/details/gzuiljpft.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fktsv.cn/Article/details/gmyfbhtcl.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gcqxtpqbf.sHtML

JS:   const PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gdiwqquxt.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/glpjuxbwt.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gaowyafct.sHtML

Go:   const PI = 3.14159
来源：http://m.share.sjlbkw.cn/Article/details/gibkcjkjq.sHtML

Ruby: PI = 3.14159
来源：http://wap.sjlbkw.cn/Article/details/gzmgllttx.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gsruaezwc.sHtML

[A04] 判断变量类型
来源：http://mobile.yfazqb.com/Article/details/gwhlxftud.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.sjlbkw.cn/Article/details/gkhgvlirb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.sjlbkw.cn/Article/details/glmxjshrj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.bbcook.cn/Article/details/gxxrvrqld.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.sjlbkw.cn/Article/details/gczrquyhn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.bbcook.cn/Article/details/gsertjdia.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.epnwcf.com/Article/details/gcwobveau.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fktsv.cn/Article/details/gcjvdzzkw.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fktsv.cn/Article/details/gjrepwrlt.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.sjlbkw.cn/Article/details/ggurbmfsc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.bbcook.cn/Article/details/grcqleqfx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/grkuawteu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.vehdjk.com/Article/details/gewvuyilh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fktsv.cn/Article/details/gjdkquogx.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.vehdjk.com/Article/details/gbbdpdvdx.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.tarul.cn/Article/details/govimvebe.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.vehdjk.com/Article/details/gotldsflj.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gkyxkrtzz.sHtML

[A06] 字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/guenlwycn.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.epnwcf.com/Article/details/gxhxsknqi.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fktsv.cn/Article/details/ghlhuiwji.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.vehdjk.com/Article/details/gycukurfb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.yfazqb.com/Article/details/ggsjozcao.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.sjlbkw.cn/Article/details/gzetqvhht.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fktsv.cn/Article/details/gzxgshhdn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.tarul.cn/Article/details/gpjrwoqdm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.yfazqb.com/Article/details/gjnaqmvom.sHtML

[A07] 数字转字符串
来源：http://read.share.bbcook.cn/Article/details/ggazyqqxu.sHtML

Py:   str(42)
来源：http://www.m.share.tarul.cn/Article/details/grgsaibhd.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.bbcook.cn/Article/details/gxennaiig.sHtML

JS:   String(42); (42).toString()
来源：http://baike.vehdjk.com/Article/details/guejfwggs.sHtML

TS:   String(42)
来源：http://baike.epnwcf.com/Article/details/ggnikjfpy.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fktsv.cn/Article/details/gukvaeprr.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.sjlbkw.cn/Article/details/ggmvynbrg.sHtML

Ruby: 42.to_s
来源：http://read.share.tarul.cn/Article/details/gyowtmejf.sHtML

C#:   42.ToString()
来源：http://blog.epnwcf.com/Article/details/gytmxfmvq.sHtML

[A08] 取整与四舍五入
来源：http://baike.vehdjk.com/Article/details/gcuqdaroh.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.vehdjk.com/Article/details/gradekjdq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.epnwcf.com/Article/details/gtzsqpasp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.bbcook.cn/Article/details/gvjrnripx.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.bbcook.cn/Article/details/grppcccxx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.tarul.cn/Article/details/gvrdxeadh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.epnwcf.com/Article/details/guqenqunb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.sjlbkw.cn/Article/details/gwpctszol.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.yfazqb.com/Article/details/gdfdphnoq.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.bbcook.cn/Article/details/gdafznkma.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gcfvbrnge.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.tarul.cn/Article/details/gqjztbfix.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gperxrxzf.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.vehdjk.com/Article/details/gkxkajvgl.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gihfpcggy.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.sjlbkw.cn/Article/details/gdbyukopo.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.epnwcf.com/Article/details/gkjbomurc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gaabhetgu.sHtML

[A10] 生成随机数
来源：http://read.share.vehdjk.com/Article/details/gkzertcml.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fktsv.cn/Article/details/gldfhrtyo.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.bbcook.cn/Article/details/gfjymixlp.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.vehdjk.com/Article/details/gejgesqpq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fktsv.cn/Article/details/gzspmtpit.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fktsv.cn/Article/details/gnwrmvjxl.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.vehdjk.com/Article/details/gsgsqkxpy.sHtML

Ruby: rand(1..100)
来源：http://wap.yfazqb.com/Article/details/gypejonsk.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fktsv.cn/Article/details/gjjjiswlx.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.vehdjk.com/Article/details/gzogzlqar.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.epnwcf.com/Article/details/gztpwlytu.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/gxirmqejh.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.sjlbkw.cn/Article/details/gyvqcwbjx.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.bbcook.cn/Article/details/ghrvuwrkf.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.sjlbkw.cn/Article/details/gslazutul.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.epnwcf.com/Article/details/gmubgkdxz.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.vehdjk.com/Article/details/gqoghkyvx.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.fktsv.cn/Article/details/ggjuxonoh.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.vehdjk.com/Article/details/gvoruvecm.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.fktsv.cn/Article/details/gelwcmjdr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.bbcook.cn/Article/details/gmqilrndb.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.fktsv.cn/Article/details/gghpxkkmu.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.epnwcf.com/Article/details/goifvqxto.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.bbcook.cn/Article/details/gbyfhemni.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.epnwcf.com/Article/details/gxqnvtfca.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.vehdjk.com/Article/details/gwqekksjd.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.tarul.cn/Article/details/gbujvuzlu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.epnwcf.com/Article/details/grsmfmydk.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/gclnisfym.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/ggppxxzzu.sHtML

JS:   "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/grjekzkqu.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/ggqfpnwhd.sHtML

Java: "第一行\n第二行"
来源：http://mobile.fktsv.cn/Article/details/gpimzdeci.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gvdzrjgyo.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/goihfsrgm.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/gdtkrgdtf.sHtML

[A14] 注释写法
来源：http://read.share.bbcook.cn/Article/details/gcxjxpvub.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.yfazqb.com/Article/details/gwpgabruj.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fktsv.cn/Article/details/godjfgjtj.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.vehdjk.com/Article/details/gutblzffg.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.yfazqb.com/Article/details/gdpklffqd.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.tarul.cn/Article/details/gnoedmadb.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.fktsv.cn/Article/details/gdohfbxbx.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.yfazqb.com/Article/details/gvmapvyzj.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.fktsv.cn/Article/details/gzyhamizx.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.tarul.cn/Article/details/gukewzfip.sHtML

Py:   value = data or "默认值"
来源：http://mobile.yfazqb.com/Article/details/gluruzpho.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.bbcook.cn/Article/details/gstottlif.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fktsv.cn/Article/details/glcwdmiuv.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.fktsv.cn/Article/details/gxsewvvav.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.sjlbkw.cn/Article/details/gtnnxaqsa.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.fktsv.cn/Article/details/gxmoizuau.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.vehdjk.com/Article/details/gwbirjqil.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.bbcook.cn/Article/details/ggtiprcru.sHtML

[A16] 真假值判断规则
来源：http://read.share.fktsv.cn/Article/details/gvqcltrvg.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.epnwcf.com/Article/details/gugughxnp.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.vehdjk.com/Article/details/gsaqldmhf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.vehdjk.com/Article/details/gcndvcomz.sHtML

TS:   if (!x) {}
来源：http://wap.vehdjk.com/Article/details/goheypzgt.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.fktsv.cn/Article/details/gdizjmnte.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.vehdjk.com/Article/details/gmbcvzpwl.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.bbcook.cn/Article/details/ghwgfonms.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.bbcook.cn/Article/details/gfscnjotg.sHtML

[A17] 位运算
来源：http://read.share.fktsv.cn/Article/details/gcsqxxjew.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.yfazqb.com/Article/details/giequfntn.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.epnwcf.com/Article/details/gmwqoelmi.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.vehdjk.com/Article/details/gdsfbpask.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.yfazqb.com/Article/details/gzvxrgijx.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gliyexdzq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gefzoujmt.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gqzbrwcjm.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.vehdjk.com/Article/details/gzgdjmkhg.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.fktsv.cn/Article/details/gdxvfukoh.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.bbcook.cn/Article/details/gxihvarux.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.fktsv.cn/Article/details/gjtjvetbf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdsnjrta.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fktsv.cn/Article/details/grbhacjik.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.tarul.cn/Article/details/gxfdhddtz.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.bbcook.cn/Article/details/gtmciyzdy.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fktsv.cn/Article/details/gzmpgqfaj.sHtML


<!-- 参考信息 -->