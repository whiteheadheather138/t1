代发 wailian999

[U103] JS：定时器
来源：http://wap.sjlbkw.cn/Article/details/gkhlnedcl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fktsv.cn/Article/details/gfbidbqqy.sHtML

[U104] JS：防抖
来源：http://baike.bbcook.cn/Article/details/gcqbaybfo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.yfazqb.com/Article/details/gtknxejys.sHtML

[U105] JS：节流
来源：http://www.blog.epnwcf.com/Article/details/gjehukabo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fktsv.cn/Article/details/glbckqqwz.sHtML

[U106] JS：日期格式化
来源：http://blog.bbcook.cn/Article/details/gffxbxtvs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.epnwcf.com/Article/details/gmaladupr.sHtML

[U107] JS：数字千分位
来源：http://mobile.fktsv.cn/Article/details/gmjiuyxnf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.epnwcf.com/Article/details/gxbsfkekz.sHtML

[U108] JS：随机整数
来源：http://3g.vehdjk.com/Article/details/gvtynrwav.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.sjlbkw.cn/Article/details/gmptfaxne.sHtML

[U109] JS：数组分组
来源：http://wap.bbcook.cn/Article/details/gnjbojtjm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.sjlbkw.cn/Article/details/ggbcxyndh.sHtML

[U110] JS：数组分块
来源：http://wap.fktsv.cn/Article/details/geoousklu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.yfazqb.com/Article/details/gkxtfwqtd.sHtML

[U111] JS：对象转 Map
来源：http://blog.sjlbkw.cn/Article/details/gcuphdfaa.sHtML

new Map(Object.entries(obj))
来源：http://baike.yfazqb.com/Article/details/gqrmnsizb.sHtML

[U112] JS：字符串补位
来源：http://3g.sjlbkw.cn/Article/details/goceobqxv.sHtML

"7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gclhnaqts.sHtML

[U113] JS：正则替换全部
来源：http://m.share.sjlbkw.cn/Article/details/gvkyrfdle.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gsqefusqy.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fktsv.cn/Article/details/gpxavlzlf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.epnwcf.com/Article/details/guiyxmjmg.sHtML

[U115] JS：生成 UUID
来源：http://wap.vehdjk.com/Article/details/gweyxdcdl.sHtML

crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/gwcmamgwa.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.tarul.cn/Article/details/gyhuwovun.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.tarul.cn/Article/details/gzezsnmkd.sHtML

[U117] JS：单元测试
来源：http://m.share.sjlbkw.cn/Article/details/gsvadsnhi.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.bbcook.cn/Article/details/gfpvckrrr.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.epnwcf.com/Article/details/gzlgqsfza.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.epnwcf.com/Article/details/gwxwuqylk.sHtML

[U119] JS：生产构建
来源：http://3g.tarul.cn/Article/details/gintlnvti.sHtML

npx vite build
来源：http://blog.fktsv.cn/Article/details/gthadeckc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.tarul.cn/Article/details/guoilgfzw.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.tarul.cn/Article/details/gihvzlneb.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gnuwxtgfm.sHtML

统计汇总
来源：http://wap.tarul.cn/Article/details/gznplzgdj.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gogzusrmm.sHtML

按语言统计（条）：
来源：http://wap.epnwcf.com/Article/details/gccxbczty.sHtML

Python ......... 252
来源：http://read.share.vehdjk.com/Article/details/gvvedptni.sHtML

PHP ............ 252
来源：http://www.m.share.fktsv.cn/Article/details/gmkxojuyd.sHtML

JavaScript ..... 252
来源：http://www.m.share.yfazqb.com/Article/details/gcqjpaiws.sHtML

TypeScript ..... 212
来源：http://wap.tarul.cn/Article/details/guptmwhfh.sHtML

Java ........... 212
来源：http://baike.vehdjk.com/Article/details/gfwindoeq.sHtML

Go ............. 212
来源：http://read.share.sjlbkw.cn/Article/details/gsmvdiudu.sHtML

Ruby ........... 212
来源：http://wap.sjlbkw.cn/Article/details/gteqelyfh.sHtML

C# ............. 212
来源：http://www.blog.epnwcf.com/Article/details/gormmlnmu.sHtML

C .............. 30
来源：http://www.m.share.fktsv.cn/Article/details/gixlrxmza.sHtML

C++ ............ 30
来源：http://www.m.share.tarul.cn/Article/details/gfoztinns.sHtML

SQL ............ 90
来源：http://www.blog.tarul.cn/Article/details/gfgluzxpm.sHtML

Bash ........... 80
来源：http://www.m.share.sjlbkw.cn/Article/details/gytswleei.sHtML

Kotlin ......... 15
来源：http://mobile.sjlbkw.cn/Article/details/gxutzpcqh.sHtML

Swift .......... 15
来源：http://www.share.vehdjk.com/Article/details/gffujiwjb.sHtML

Lua ............ 10
来源：http://3g.tarul.cn/Article/details/gerzfpizj.sHtML

Perl ........... 10
来源：http://blog.epnwcf.com/Article/details/gukrecglc.sHtML

Scala .......... 10
来源：http://mobile.vehdjk.com/Article/details/gdardhbrs.sHtML

------------------------------------
来源：http://baike.fktsv.cn/Article/details/gwpyvgpbp.sHtML

合计 ........... 2106 条
来源：http://mobile.yfazqb.com/Article/details/gkpsjzssq.sHtML

按章节统计：
来源：http://www.m.share.fktsv.cn/Article/details/grwpgiclr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.epnwcf.com/Article/details/gocohvobb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gsxbanbrm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fktsv.cn/Article/details/gqkthyvyv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.sjlbkw.cn/Article/details/gehgmwvec.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.epnwcf.com/Article/details/goukibogw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.sjlbkw.cn/Article/details/gsshyavyj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fktsv.cn/Article/details/giyjrndsu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.tarul.cn/Article/details/ggutghkvy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gqjvofuti.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.epnwcf.com/Article/details/goibiudxt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gzxcqstlp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gosbvrcze.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/gponlyago.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.sjlbkw.cn/Article/details/gaurhwlth.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.epnwcf.com/Article/details/gvqpeikop.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/glzcyzrkl.sHtML

Q SQL 专题                              90
来源：http://www.blog.tarul.cn/Article/details/gqnxxmvly.sHtML

R Bash 专题                             80
来源：http://blog.vehdjk.com/Article/details/grqgtrxds.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.yfazqb.com/Article/details/gunlesthe.sHtML

T 其他语言补充                          60
来源：http://wap.epnwcf.com/Article/details/gkkvmmxnq.sHtML

U 高频实用片段                         120
来源：http://3g.fktsv.cn/Article/details/gpzeemovl.sHtML

------------------------------------
来源：http://wap.bbcook.cn/Article/details/gbwjgyzoc.sHtML

合计                                  2106 条
来源：http://www.m.share.epnwcf.com/Article/details/gysftoanl.sHtML

--------------------------------------------------------------------------------
来源：http://wap.tarul.cn/Article/details/gonfdvryv.sHtML

使用提醒
来源：http://blog.vehdjk.com/Article/details/gdvvltfla.sHtML

--------------------------------------------------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gczufyywq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fktsv.cn/Article/details/gpwxypzdf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.epnwcf.com/Article/details/gqselmtwf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fktsv.cn/Article/details/gxzaexuii.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.epnwcf.com/Article/details/gbwrwrodw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.yfazqb.com/Article/details/gcekdyjsq.sHtML

—— 文件结束 ——
来源：http://www.share.vehdjk.com/Article/details/gglhhgjmz.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gnocawvoy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.vehdjk.com/Article/details/gwexbmjjf.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.vehdjk.com/Article/details/gwhyiwjhe.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gbkijuzjs.sHtML

【收录内容】
来源：http://baike.tarul.cn/Article/details/gnewbapmg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fktsv.cn/Article/details/gxmcgzdaf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.yfazqb.com/Article/details/gmhculzny.sHtML

SQL · Bash · C · C++
来源：http://www.share.epnwcf.com/Article/details/gyhjboyrh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.bbcook.cn/Article/details/gatzanrqu.sHtML

【使用说明】
来源：http://www.share.bbcook.cn/Article/details/ggmffzrii.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.bbcook.cn/Article/details/gedpbbqoz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.vehdjk.com/Article/details/gsluevevk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.yfazqb.com/Article/details/gavpaejpc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.bbcook.cn/Article/details/gxpbdghmv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.tarul.cn/Article/details/gabxplbbn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.yfazqb.com/Article/details/gjftnpldl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.epnwcf.com/Article/details/gtmzlztmz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.yfazqb.com/Article/details/gwjpastzt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.epnwcf.com/Article/details/gwmmkeomq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.yfazqb.com/Article/details/gwfbhtyuj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.vehdjk.com/Article/details/gqtmhbbko.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.epnwcf.com/Article/details/gnqpjrzgm.sHtML

【文件统计】
来源：http://www.m.share.vehdjk.com/Article/details/gtvmevaku.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.yfazqb.com/Article/details/gcidwxkss.sHtML

--------------------------------------------------------------------------------
来源：http://3g.bbcook.cn/Article/details/giehzblav.sHtML

目  录
来源：http://www.m.share.fktsv.cn/Article/details/gdvdsifjy.sHtML

--------------------------------------------------------------------------------
来源：http://3g.bbcook.cn/Article/details/gojfhrmtk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.bbcook.cn/Article/details/gbuhihqxa.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrzzpacw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fktsv.cn/Article/details/grzclzbfn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.vehdjk.com/Article/details/gqdtvvbgi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.vehdjk.com/Article/details/gjitxhhcs.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fktsv.cn/Article/details/gktfruurj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.vehdjk.com/Article/details/gyfdyollr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.yfazqb.com/Article/details/gqjciwazd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.vehdjk.com/Article/details/gnonsvrmt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.vehdjk.com/Article/details/gnkghtpee.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/ggpnfqfee.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/gwxlpoazc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/gtpnqvwrx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.epnwcf.com/Article/details/gssvfxsub.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.vehdjk.com/Article/details/gjrfmerin.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/gxictxibd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fktsv.cn/Article/details/gamvqbvng.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.vehdjk.com/Article/details/gbxhzhmji.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.vehdjk.com/Article/details/gyuzbvyvs.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.epnwcf.com/Article/details/golopatlb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.epnwcf.com/Article/details/ghqlicmci.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gomletcgn.sHtML

A. 基础语法与类型
来源：http://m.share.bbcook.cn/Article/details/gqhdxbezr.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ggdrnurrf.sHtML

[A01] Hello World
来源：http://baike.sjlbkw.cn/Article/details/ggdruxehc.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fktsv.cn/Article/details/gwkrmlbdg.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.vehdjk.com/Article/details/gloyvywio.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.vehdjk.com/Article/details/gtftrcgqd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.bbcook.cn/Article/details/gwnenvujk.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.yfazqb.com/Article/details/gxnbgivio.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.vehdjk.com/Article/details/ghydqjptb.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.yfazqb.com/Article/details/gfkoormus.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.vehdjk.com/Article/details/gqwvcdqib.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.yfazqb.com/Article/details/gbnulodgi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.tarul.cn/Article/details/gzwfvsafu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.epnwcf.com/Article/details/godjroish.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.vehdjk.com/Article/details/gqhcscgsw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.tarul.cn/Article/details/gikccmtgb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.tarul.cn/Article/details/gbsddkzwn.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.tarul.cn/Article/details/gofqnjssq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.sjlbkw.cn/Article/details/gwrvkesrg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fktsv.cn/Article/details/gnkqqydyq.sHtML

[A03] 常量定义
来源：http://www.share.sjlbkw.cn/Article/details/gtgpcdxjc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.sjlbkw.cn/Article/details/gmwkbnola.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gojnbplfq.sHtML

JS:   const PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/gfgacyees.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fktsv.cn/Article/details/gmqhhjwgp.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gvzoqlmbb.sHtML

Go:   const PI = 3.14159
来源：http://baike.tarul.cn/Article/details/gjtuwhhfm.sHtML

Ruby: PI = 3.14159
来源：http://3g.fktsv.cn/Article/details/gjgkbmgdx.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gkuqbvvwd.sHtML

[A04] 判断变量类型
来源：http://wap.bbcook.cn/Article/details/ggkubmkoz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.bbcook.cn/Article/details/gjlnpcdix.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.sjlbkw.cn/Article/details/ggldkbasy.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fktsv.cn/Article/details/gjqznpfzg.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fktsv.cn/Article/details/gkwdtzbew.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.tarul.cn/Article/details/gluvbicdb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.sjlbkw.cn/Article/details/gapihdmyq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.vehdjk.com/Article/details/ghjbtjzjo.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.sjlbkw.cn/Article/details/gfewphztr.sHtML

[A05] 整数除法与取模
来源：http://m.share.vehdjk.com/Article/details/gafhzbsci.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrxzpimf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.bbcook.cn/Article/details/gxsorsipu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/guwkrspkr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.bbcook.cn/Article/details/gmqxzqiej.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.tarul.cn/Article/details/ghioqwexd.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fktsv.cn/Article/details/gbtiaqfek.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.vehdjk.com/Article/details/gzjcdcahi.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.epnwcf.com/Article/details/gmgsvoqia.sHtML

[A06] 字符串转数字
来源：http://m.share.yfazqb.com/Article/details/gshcuwkcl.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.bbcook.cn/Article/details/gpcmxtxrm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.sjlbkw.cn/Article/details/gedenpzmd.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.epnwcf.com/Article/details/gabicldnm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.yfazqb.com/Article/details/gadlwrvvm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.bbcook.cn/Article/details/gvaicpmyd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.epnwcf.com/Article/details/gwqeznsah.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.sjlbkw.cn/Article/details/gzhxfprhd.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.bbcook.cn/Article/details/gnnvxehwy.sHtML

[A07] 数字转字符串
来源：http://3g.epnwcf.com/Article/details/gqccvixjp.sHtML

Py:   str(42)
来源：http://m.share.vehdjk.com/Article/details/ggcwtyiiy.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.vehdjk.com/Article/details/geekxuxny.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.yfazqb.com/Article/details/ghfvqsrah.sHtML

TS:   String(42)
来源：http://mobile.vehdjk.com/Article/details/gqoyoykgu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.tarul.cn/Article/details/gwqarnana.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.yfazqb.com/Article/details/gxqpzrwcu.sHtML

Ruby: 42.to_s
来源：http://blog.epnwcf.com/Article/details/gmkgpxtes.sHtML

C#:   42.ToString()
来源：http://baike.yfazqb.com/Article/details/gercgfxlr.sHtML

[A08] 取整与四舍五入
来源：http://blog.sjlbkw.cn/Article/details/gvzeoyxvo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.sjlbkw.cn/Article/details/gjrdpdkja.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.sjlbkw.cn/Article/details/gzqkikvkh.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.sjlbkw.cn/Article/details/gipgffiyk.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.tarul.cn/Article/details/gvrvrqxxn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.bbcook.cn/Article/details/gomlkldkg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.tarul.cn/Article/details/gkwabouby.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.yfazqb.com/Article/details/geensmptj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.tarul.cn/Article/details/glilqdbnc.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.tarul.cn/Article/details/gwocdfckb.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gdhncdjfk.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gomyyaxda.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.vehdjk.com/Article/details/gpmrthspq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fktsv.cn/Article/details/gmiqqqalw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.vehdjk.com/Article/details/gezgfwqbz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.vehdjk.com/Article/details/gpkdnsxhr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.fktsv.cn/Article/details/glwsreiwe.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.vehdjk.com/Article/details/gkomqnhfb.sHtML

[A10] 生成随机数
来源：http://www.blog.fktsv.cn/Article/details/gkyghcscm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.yfazqb.com/Article/details/gvdxvyflr.sHtML

PHP:  random_int(1, 100);
来源：http://wap.vehdjk.com/Article/details/gvnbijjoz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.bbcook.cn/Article/details/ghfdxsupz.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.tarul.cn/Article/details/gxgrehviv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.yfazqb.com/Article/details/grfzlyscy.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.epnwcf.com/Article/details/gsjtnjnxx.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fktsv.cn/Article/details/gzccksjlc.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.vehdjk.com/Article/details/gmemzuwtt.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fktsv.cn/Article/details/gieilcopk.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.bbcook.cn/Article/details/ggzneqezw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fktsv.cn/Article/details/goytwspvx.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.yfazqb.com/Article/details/gxldmhddf.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.vehdjk.com/Article/details/gwiwzzqow.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.fktsv.cn/Article/details/gdqchqnlq.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.bbcook.cn/Article/details/ghbpvitis.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.tarul.cn/Article/details/gvxqhshrl.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.sjlbkw.cn/Article/details/gejrogwxq.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.tarul.cn/Article/details/gxdcxqvpq.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.bbcook.cn/Article/details/gmowhhtbg.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.tarul.cn/Article/details/gwfkzovdx.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.epnwcf.com/Article/details/gbxleigxn.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.sjlbkw.cn/Article/details/gxqeofoir.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.vehdjk.com/Article/details/gjsshtftg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.vehdjk.com/Article/details/gueumspeg.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.fktsv.cn/Article/details/gktpkoovy.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.yfazqb.com/Article/details/gnblrdcnz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.bbcook.cn/Article/details/gqjikscih.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gvvqzivkn.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/grhfznlym.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/gmxctmrnp.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/ghvcfzxvd.sHtML

Java: "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/gnuwuaxub.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/giglccues.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gpzaiqkti.sHtML

C#:   "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/grwjvgfrx.sHtML

[A14] 注释写法
来源：http://3g.fktsv.cn/Article/details/gnxinbjmb.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.epnwcf.com/Article/details/gkiqrwjzu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.yfazqb.com/Article/details/gwcspnjig.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.fktsv.cn/Article/details/guquufenm.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.vehdjk.com/Article/details/gtemjeoau.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fktsv.cn/Article/details/gvbomhjnm.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.fktsv.cn/Article/details/gjnkwtxwq.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.vehdjk.com/Article/details/gkouujwmy.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.bbcook.cn/Article/details/gwffigchh.sHtML

[A15] 空值判断与默认值
来源：http://3g.sjlbkw.cn/Article/details/gjjfbniqr.sHtML

Py:   value = data or "默认值"
来源：http://read.share.tarul.cn/Article/details/ggwhjfanh.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.yfazqb.com/Article/details/gevxwwsqd.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.epnwcf.com/Article/details/goryonakc.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.sjlbkw.cn/Article/details/gnwigdjut.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.epnwcf.com/Article/details/gnuwchsha.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.yfazqb.com/Article/details/gvjqxjsua.sHtML

Ruby: value = data || "默认值"
来源：http://baike.sjlbkw.cn/Article/details/gucxxuhxi.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.tarul.cn/Article/details/gjiddtmfm.sHtML

[A16] 真假值判断规则
来源：http://m.share.vehdjk.com/Article/details/gwjyhyzwz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.sjlbkw.cn/Article/details/gcrxejgmk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fktsv.cn/Article/details/gkzucucxh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.yfazqb.com/Article/details/gmuuqakwf.sHtML

TS:   if (!x) {}
来源：http://read.share.sjlbkw.cn/Article/details/gfgslsbnw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.epnwcf.com/Article/details/gllhunhhl.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.vehdjk.com/Article/details/gqmxhdbbd.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.fktsv.cn/Article/details/gamafvxlb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.fktsv.cn/Article/details/ghifmawfj.sHtML

[A17] 位运算
来源：http://blog.bbcook.cn/Article/details/gywhulutg.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gqfaifavi.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gvwrtjnqu.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/gpgwbsorq.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gevnmxgms.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.sjlbkw.cn/Article/details/giuhkwuwr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/ghybszjxf.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gtwkthdvu.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/gwgqmksnp.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.sjlbkw.cn/Article/details/gswzwudoc.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpldoume.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.bbcook.cn/Article/details/grsrxystl.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.vehdjk.com/Article/details/gxgcahtms.sHtML


<!-- 参考信息 -->