代发 wailian999

[U105] JS：节流
来源：http://m.share.epnwcf.com/Article/details/gvtgxghoy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.tarul.cn/Article/details/gzvwrnnix.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fktsv.cn/Article/details/gpgtxyhbp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.vehdjk.com/Article/details/goooecokj.sHtML

[U107] JS：数字千分位
来源：http://read.share.bbcook.cn/Article/details/gyycgbbjf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.yfazqb.com/Article/details/gwdvxsbyo.sHtML

[U108] JS：随机整数
来源：http://baike.tarul.cn/Article/details/guikzajmd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.vehdjk.com/Article/details/gzaumzbug.sHtML

[U109] JS：数组分组
来源：http://wap.bbcook.cn/Article/details/gydqurgbx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.yfazqb.com/Article/details/gmizewhsm.sHtML

[U110] JS：数组分块
来源：http://wap.fktsv.cn/Article/details/gsnovgvff.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.vehdjk.com/Article/details/gihghbgzy.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/gnngkmukq.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.epnwcf.com/Article/details/gjxsofklg.sHtML

[U112] JS：字符串补位
来源：http://blog.yfazqb.com/Article/details/gomcxaglm.sHtML

"7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/ggialfwvj.sHtML

[U113] JS：正则替换全部
来源：http://www.share.vehdjk.com/Article/details/ghexlsqwj.sHtML

s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gtanshvzc.sHtML

[U114] JS：JSON 深比较
来源：http://blog.sjlbkw.cn/Article/details/gflyqmyug.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.epnwcf.com/Article/details/gsyinkozg.sHtML

[U115] JS：生成 UUID
来源：http://mobile.bbcook.cn/Article/details/gnhsleout.sHtML

crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gyallncjp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.vehdjk.com/Article/details/gyebiycsr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.epnwcf.com/Article/details/ggprqltvd.sHtML

[U117] JS：单元测试
来源：http://www.share.sjlbkw.cn/Article/details/givtdpqya.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.yfazqb.com/Article/details/gdbtnhtam.sHtML

[U118] JS：开发服务器
来源：http://www.share.sjlbkw.cn/Article/details/gsddhvdit.sHtML

npm i -D vite;  npx vite
来源：http://wap.fktsv.cn/Article/details/glykpjgbf.sHtML

[U119] JS：生产构建
来源：http://mobile.epnwcf.com/Article/details/ggwaelxpj.sHtML

npx vite build
来源：http://www.share.epnwcf.com/Article/details/ghdorfwpx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.sjlbkw.cn/Article/details/gcquhshxz.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.bbcook.cn/Article/details/gpvckkwpi.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gczpsqajf.sHtML

统计汇总
来源：http://www.share.yfazqb.com/Article/details/guqppquhz.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gmxtnafzr.sHtML

按语言统计（条）：
来源：http://m.share.bbcook.cn/Article/details/gvxpexrky.sHtML

Python ......... 252
来源：http://www.share.bbcook.cn/Article/details/gqvgsulxu.sHtML

PHP ............ 252
来源：http://m.share.bbcook.cn/Article/details/gyucfspus.sHtML

JavaScript ..... 252
来源：http://blog.bbcook.cn/Article/details/gdvrurwyg.sHtML

TypeScript ..... 212
来源：http://wap.vehdjk.com/Article/details/grfgugued.sHtML

Java ........... 212
来源：http://baike.fktsv.cn/Article/details/gzgdjtohl.sHtML

Go ............. 212
来源：http://baike.sjlbkw.cn/Article/details/glioaraap.sHtML

Ruby ........... 212
来源：http://3g.tarul.cn/Article/details/gnzvzjbhu.sHtML

C# ............. 212
来源：http://3g.sjlbkw.cn/Article/details/gedjxjmii.sHtML

C .............. 30
来源：http://wap.bbcook.cn/Article/details/gwgeiqlmm.sHtML

C++ ............ 30
来源：http://wap.fktsv.cn/Article/details/gymtkwtaf.sHtML

SQL ............ 90
来源：http://m.share.vehdjk.com/Article/details/gegdkfgnz.sHtML

Bash ........... 80
来源：http://www.m.share.yfazqb.com/Article/details/gwmcevcxu.sHtML

Kotlin ......... 15
来源：http://wap.yfazqb.com/Article/details/gxdanmqxy.sHtML

Swift .......... 15
来源：http://3g.sjlbkw.cn/Article/details/gcvaahjzh.sHtML

Lua ............ 10
来源：http://www.blog.vehdjk.com/Article/details/gfjwwyexs.sHtML

Perl ........... 10
来源：http://mobile.vehdjk.com/Article/details/gtpnffirp.sHtML

Scala .......... 10
来源：http://read.share.epnwcf.com/Article/details/glajuayqr.sHtML

------------------------------------
来源：http://blog.fktsv.cn/Article/details/gpjaulqod.sHtML

合计 ........... 2106 条
来源：http://wap.sjlbkw.cn/Article/details/gelhudmfm.sHtML

按章节统计：
来源：http://mobile.vehdjk.com/Article/details/gxpmayeec.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.epnwcf.com/Article/details/gpfsninna.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.epnwcf.com/Article/details/gabuvsajs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fktsv.cn/Article/details/gbsgtrgij.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fktsv.cn/Article/details/gftnirlfl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.tarul.cn/Article/details/gmvlxldpt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.tarul.cn/Article/details/gqxlvqbsc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.bbcook.cn/Article/details/girqgwehs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.yfazqb.com/Article/details/ghkugfnlk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gzqbvceel.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fktsv.cn/Article/details/grngywpyb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/ggrkyvhni.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/glwbmsgms.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/gcecwpeka.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.sjlbkw.cn/Article/details/gsqprhqya.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.vehdjk.com/Article/details/gswnmsshr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/gkcjxncub.sHtML

Q SQL 专题                              90
来源：http://baike.bbcook.cn/Article/details/gvxiegtoe.sHtML

R Bash 专题                             80
来源：http://www.m.share.fktsv.cn/Article/details/gpceyxhrx.sHtML

S C / C++ 专题                          60
来源：http://www.blog.vehdjk.com/Article/details/gdoogtlos.sHtML

T 其他语言补充                          60
来源：http://m.share.fktsv.cn/Article/details/gbecrbdrv.sHtML

U 高频实用片段                         120
来源：http://mobile.bbcook.cn/Article/details/gdbuujtqp.sHtML

------------------------------------
来源：http://m.share.vehdjk.com/Article/details/gadozdwik.sHtML

合计                                  2106 条
来源：http://3g.bbcook.cn/Article/details/gsexfwzpc.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gqwuppziq.sHtML

使用提醒
来源：http://m.share.yfazqb.com/Article/details/gxnklaguq.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/gqitusaoe.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.yfazqb.com/Article/details/gsemmunbj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.sjlbkw.cn/Article/details/gnlhtiwjp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.epnwcf.com/Article/details/gciivggjo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.bbcook.cn/Article/details/gwgfaudlj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.yfazqb.com/Article/details/guzpdjerl.sHtML

—— 文件结束 ——
来源：http://www.blog.yfazqb.com/Article/details/gzmftngqb.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gqnagxbav.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fktsv.cn/Article/details/gqlytxjvj.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.epnwcf.com/Article/details/gqpwgtofz.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gkwtcosrx.sHtML

【收录内容】
来源：http://read.share.vehdjk.com/Article/details/gytebqvgf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.tarul.cn/Article/details/gctgomimj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.yfazqb.com/Article/details/gvhxgwpmd.sHtML

SQL · Bash · C · C++
来源：http://blog.bbcook.cn/Article/details/glodihuug.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.epnwcf.com/Article/details/gvtchwrwj.sHtML

【使用说明】
来源：http://mobile.bbcook.cn/Article/details/gvgqvngse.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.sjlbkw.cn/Article/details/guyxdrnor.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.tarul.cn/Article/details/gzzemdmcg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fktsv.cn/Article/details/gauxajzox.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.tarul.cn/Article/details/gmompokfw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fktsv.cn/Article/details/gispmfbgo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.bbcook.cn/Article/details/goaatchio.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fktsv.cn/Article/details/gtnbromlz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.vehdjk.com/Article/details/gsfbwhpwz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.bbcook.cn/Article/details/gifmybfzd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.yfazqb.com/Article/details/gdzvnskhl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.yfazqb.com/Article/details/gqkbrfsve.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.yfazqb.com/Article/details/gpwqlfjub.sHtML

【文件统计】
来源：http://blog.tarul.cn/Article/details/ggylwzywc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.bbcook.cn/Article/details/gpzqbhiww.sHtML

--------------------------------------------------------------------------------
来源：http://3g.vehdjk.com/Article/details/glatoykyx.sHtML

目  录
来源：http://read.share.yfazqb.com/Article/details/gvxwxztgt.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gawvibvcn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fktsv.cn/Article/details/gylcdxpts.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.epnwcf.com/Article/details/gefoehaxb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/gbidxiyri.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.bbcook.cn/Article/details/gvnvhzqmu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.vehdjk.com/Article/details/gygtsdhxw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.yfazqb.com/Article/details/gajfeotlu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fktsv.cn/Article/details/gxqtsiqdv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.epnwcf.com/Article/details/gbvjnskyd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/gnwrzoxng.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.epnwcf.com/Article/details/gvjqaiyiy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fktsv.cn/Article/details/gvmsonwpu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.bbcook.cn/Article/details/gtmvyomma.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/gjzfyjczx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.sjlbkw.cn/Article/details/gzfycyvzw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fktsv.cn/Article/details/gflugincd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.sjlbkw.cn/Article/details/gpyacfbok.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.sjlbkw.cn/Article/details/gwazdabtv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.sjlbkw.cn/Article/details/gxyjzrkxu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.epnwcf.com/Article/details/gvmdgduxy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.sjlbkw.cn/Article/details/gjkhutvxj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.vehdjk.com/Article/details/gzovoxilo.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gytkchumu.sHtML

A. 基础语法与类型
来源：http://mobile.yfazqb.com/Article/details/gjyiqkaty.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gducmwegq.sHtML

[A01] Hello World
来源：http://www.blog.fktsv.cn/Article/details/gcicccgxl.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.yfazqb.com/Article/details/gfmmxejry.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.sjlbkw.cn/Article/details/gxqnuzvkt.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.yfazqb.com/Article/details/giorhnjlo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.bbcook.cn/Article/details/gdurmaddl.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.yfazqb.com/Article/details/glzyjinms.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.vehdjk.com/Article/details/getwflgui.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.bbcook.cn/Article/details/gxwnivugx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.bbcook.cn/Article/details/gigsdidrs.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.sjlbkw.cn/Article/details/gwimkeqqq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.vehdjk.com/Article/details/gjjvumwyf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.tarul.cn/Article/details/gccupvlwe.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.vehdjk.com/Article/details/gnscnucsl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.bbcook.cn/Article/details/gtgpjvxbr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.tarul.cn/Article/details/ggtkavmrh.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.yfazqb.com/Article/details/gnnelxijq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.epnwcf.com/Article/details/gkxoslerg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.vehdjk.com/Article/details/gbeqggtft.sHtML

[A03] 常量定义
来源：http://read.share.bbcook.cn/Article/details/gqdwssdzb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.epnwcf.com/Article/details/gixxtyanj.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/ggjdnotty.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gfwoiztzv.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.tarul.cn/Article/details/ghoksvcqq.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gjqpnrpoc.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.tarul.cn/Article/details/gpnyynvst.sHtML

Ruby: PI = 3.14159
来源：http://www.share.epnwcf.com/Article/details/gyneaiekc.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gdnqnyjud.sHtML

[A04] 判断变量类型
来源：http://www.m.share.bbcook.cn/Article/details/gwnomgtxg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.bbcook.cn/Article/details/gaytknixq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fktsv.cn/Article/details/gshrovapq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.sjlbkw.cn/Article/details/groldsmwz.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.vehdjk.com/Article/details/gszgrwlmy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.tarul.cn/Article/details/gktrlhktq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.tarul.cn/Article/details/gcndcmqzc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.vehdjk.com/Article/details/gebmikykq.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.vehdjk.com/Article/details/ggundxqiz.sHtML

[A05] 整数除法与取模
来源：http://www.blog.tarul.cn/Article/details/gsptuhdux.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.sjlbkw.cn/Article/details/gmcwqutog.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.epnwcf.com/Article/details/gfhmhawxn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.vehdjk.com/Article/details/gojjnlszc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.bbcook.cn/Article/details/gucuwhgmt.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/gkgkaymcz.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gaicjvygh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.vehdjk.com/Article/details/gympoxrub.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/grubicjdb.sHtML

[A06] 字符串转数字
来源：http://baike.epnwcf.com/Article/details/glpfxtwvp.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.yfazqb.com/Article/details/gnfjkqcny.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fktsv.cn/Article/details/gmoeqnpuj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.yfazqb.com/Article/details/gkfewdtuz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.bbcook.cn/Article/details/gwckyuxgz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.sjlbkw.cn/Article/details/gqdpochnf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.yfazqb.com/Article/details/gclqercow.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.epnwcf.com/Article/details/grtfnkyvm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.yfazqb.com/Article/details/gylkodusx.sHtML

[A07] 数字转字符串
来源：http://read.share.yfazqb.com/Article/details/gtyzwvpoa.sHtML

Py:   str(42)
来源：http://www.blog.fktsv.cn/Article/details/gukqdryes.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.sjlbkw.cn/Article/details/gdjupngcl.sHtML

JS:   String(42); (42).toString()
来源：http://wap.sjlbkw.cn/Article/details/gwajvsrwz.sHtML

TS:   String(42)
来源：http://m.share.tarul.cn/Article/details/goppyrkyq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fktsv.cn/Article/details/gnyqmbkbk.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.yfazqb.com/Article/details/gwbougnrt.sHtML

Ruby: 42.to_s
来源：http://baike.vehdjk.com/Article/details/gpsrnoarp.sHtML

C#:   42.ToString()
来源：http://blog.epnwcf.com/Article/details/gtrbsvzkk.sHtML

[A08] 取整与四舍五入
来源：http://wap.sjlbkw.cn/Article/details/gxlaomvyc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/gyfdebcgd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.yfazqb.com/Article/details/geozpblgw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.bbcook.cn/Article/details/gvvvgrlao.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.sjlbkw.cn/Article/details/gzxconbxu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.yfazqb.com/Article/details/gogdmirwz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.sjlbkw.cn/Article/details/gidbljtgc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.sjlbkw.cn/Article/details/glfzpyiaq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.vehdjk.com/Article/details/gvqvyspef.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.epnwcf.com/Article/details/gkebzilch.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gbycrqgju.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.vehdjk.com/Article/details/gnkziwvlx.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.yfazqb.com/Article/details/gzpdivflz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.vehdjk.com/Article/details/gjnwizltj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.epnwcf.com/Article/details/gctypntya.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.vehdjk.com/Article/details/gtzrqoebe.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.sjlbkw.cn/Article/details/ghjkfrtph.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.tarul.cn/Article/details/gkgrukcst.sHtML

[A10] 生成随机数
来源：http://wap.fktsv.cn/Article/details/gviypllsc.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fktsv.cn/Article/details/ghxubdmgn.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fktsv.cn/Article/details/gnkutdhyt.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.sjlbkw.cn/Article/details/golyyjspz.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.epnwcf.com/Article/details/gzalhkjjr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.bbcook.cn/Article/details/gmrgmpdcx.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.tarul.cn/Article/details/gaiczchmp.sHtML

Ruby: rand(1..100)
来源：http://wap.yfazqb.com/Article/details/gsyjzufes.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.fktsv.cn/Article/details/gmxyxoika.sHtML

[A11] 条件表达式（三元）
来源：http://blog.sjlbkw.cn/Article/details/gizogmyyg.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.tarul.cn/Article/details/ghiqmsaej.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.vehdjk.com/Article/details/grfftksoa.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fktsv.cn/Article/details/grewtgxmf.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.vehdjk.com/Article/details/gqwtvylgk.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.sjlbkw.cn/Article/details/gyrifuvmb.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.epnwcf.com/Article/details/ghcztcriv.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.vehdjk.com/Article/details/gvmqamuhe.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.yfazqb.com/Article/details/gcfcxewsg.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.sjlbkw.cn/Article/details/gmvjzmnay.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gyziwixlj.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.tarul.cn/Article/details/gvotsebpx.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.epnwcf.com/Article/details/gjjxxoehb.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.epnwcf.com/Article/details/gmvmqnnrh.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.vehdjk.com/Article/details/gxwrlticy.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.epnwcf.com/Article/details/gtsvfdqys.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.vehdjk.com/Article/details/gpwohamfi.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.tarul.cn/Article/details/gkimyqwaq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.epnwcf.com/Article/details/gaqgwucrh.sHtML

Py:   "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/grgfjqjqk.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gqbbglfqh.sHtML

JS:   "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/gtjzxnwvk.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.epnwcf.com/Article/details/gjlenuwno.sHtML

Java: "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/gahyvcptb.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.bbcook.cn/Article/details/gvmrhhcyy.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/gpfelkkzu.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/golileugc.sHtML

[A14] 注释写法
来源：http://m.share.epnwcf.com/Article/details/gmuebxsfl.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.epnwcf.com/Article/details/gckgggnwl.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.tarul.cn/Article/details/gepggkmkz.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.fktsv.cn/Article/details/gbqjemwgy.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.tarul.cn/Article/details/gnmkmxxol.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.bbcook.cn/Article/details/gtieyaybt.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/gfppwagot.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.sjlbkw.cn/Article/details/ghwpoxdmu.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.vehdjk.com/Article/details/gndnuikhq.sHtML

[A15] 空值判断与默认值
来源：http://3g.vehdjk.com/Article/details/gvxcfkueb.sHtML

Py:   value = data or "默认值"
来源：http://mobile.bbcook.cn/Article/details/grcgpdkwy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.bbcook.cn/Article/details/ghrpplszo.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.tarul.cn/Article/details/guvzmtvaw.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.tarul.cn/Article/details/gzohnjeod.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.fktsv.cn/Article/details/goqpjfxpm.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.bbcook.cn/Article/details/gigbanrdc.sHtML

Ruby: value = data || "默认值"
来源：http://baike.vehdjk.com/Article/details/gxktxtgbb.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.bbcook.cn/Article/details/giymdrqco.sHtML

[A16] 真假值判断规则
来源：http://m.share.bbcook.cn/Article/details/gkueeqjdv.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.yfazqb.com/Article/details/giiedcgyj.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.bbcook.cn/Article/details/gzmesrtaf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.bbcook.cn/Article/details/gjekiyhjd.sHtML

TS:   if (!x) {}
来源：http://read.share.bbcook.cn/Article/details/gthcvczuj.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.epnwcf.com/Article/details/ggrqndnue.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.epnwcf.com/Article/details/gwopypria.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.bbcook.cn/Article/details/gdwfxmwhe.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fktsv.cn/Article/details/gvfdamtij.sHtML

[A17] 位运算
来源：http://blog.epnwcf.com/Article/details/gbvnpcpcj.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/glaktczji.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.tarul.cn/Article/details/guhxsyfvn.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/ggvhjlfhh.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.yfazqb.com/Article/details/gmusvtzcy.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.yfazqb.com/Article/details/gpcniszca.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gakuceuoj.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gszxowqsw.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/ghjyxvaut.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.fktsv.cn/Article/details/gcsmwbwic.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.vehdjk.com/Article/details/gakmbykrd.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.tarul.cn/Article/details/gdnjxkgir.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.epnwcf.com/Article/details/gnxbipyzy.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.tarul.cn/Article/details/glosjksad.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.epnwcf.com/Article/details/ggzbwbtqv.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.yfazqb.com/Article/details/ghtcjhdsm.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.epnwcf.com/Article/details/gewclrdnx.sHtML


<!-- 参考信息 -->