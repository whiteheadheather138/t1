代发 wailian999

[U103] JS：定时器
来源：http://mobile.bbcook.cn/Article/details/grpyzictq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.bbcook.cn/Article/details/ggehfdmlt.sHtML

[U104] JS：防抖
来源：http://blog.fktsv.cn/Article/details/gzgqovbli.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.epnwcf.com/Article/details/guuguvepn.sHtML

[U105] JS：节流
来源：http://read.share.tarul.cn/Article/details/ggdphupqe.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fktsv.cn/Article/details/ghsxussan.sHtML

[U106] JS：日期格式化
来源：http://www.share.epnwcf.com/Article/details/ggnssibzc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.tarul.cn/Article/details/givcqoghc.sHtML

[U107] JS：数字千分位
来源：http://baike.fktsv.cn/Article/details/goxpdvtwl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.vehdjk.com/Article/details/gjscnsthm.sHtML

[U108] JS：随机整数
来源：http://www.share.fktsv.cn/Article/details/gpsbstsmo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.bbcook.cn/Article/details/gsqfzrulg.sHtML

[U109] JS：数组分组
来源：http://m.share.epnwcf.com/Article/details/gjfqmlrqi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.bbcook.cn/Article/details/gldfdnwhe.sHtML

[U110] JS：数组分块
来源：http://www.share.tarul.cn/Article/details/gvkpawzhn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.bbcook.cn/Article/details/gyeofmavo.sHtML

[U111] JS：对象转 Map
来源：http://mobile.sjlbkw.cn/Article/details/ghbljzzpo.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.yfazqb.com/Article/details/gjpqhopry.sHtML

[U112] JS：字符串补位
来源：http://mobile.yfazqb.com/Article/details/gflewiqul.sHtML

"7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gspsrxpbn.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fktsv.cn/Article/details/glracwesp.sHtML

s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gaujahqhe.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fktsv.cn/Article/details/gbeyinerp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.tarul.cn/Article/details/gpzkdixre.sHtML

[U115] JS：生成 UUID
来源：http://wap.tarul.cn/Article/details/glqddvigc.sHtML

crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gbtruifhy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.yfazqb.com/Article/details/geplepzux.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.bbcook.cn/Article/details/grhlvglgs.sHtML

[U117] JS：单元测试
来源：http://www.share.fktsv.cn/Article/details/gzcegsppu.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.yfazqb.com/Article/details/gltezsfsm.sHtML

[U118] JS：开发服务器
来源：http://blog.sjlbkw.cn/Article/details/gxpzrkjgm.sHtML

npm i -D vite;  npx vite
来源：http://wap.tarul.cn/Article/details/gqkqrrxyj.sHtML

[U119] JS：生产构建
来源：http://wap.yfazqb.com/Article/details/gbqzzrfqt.sHtML

npx vite build
来源：http://www.share.vehdjk.com/Article/details/gyyzjdnll.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fktsv.cn/Article/details/gmgqpazrt.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.tarul.cn/Article/details/gnuinzjxp.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gsjsyqhtg.sHtML

统计汇总
来源：http://read.share.yfazqb.com/Article/details/gsegjpsyo.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gcjokryes.sHtML

按语言统计（条）：
来源：http://www.m.share.yfazqb.com/Article/details/gtawtpttb.sHtML

Python ......... 252
来源：http://www.m.share.tarul.cn/Article/details/gialpbxom.sHtML

PHP ............ 252
来源：http://wap.epnwcf.com/Article/details/gqeziskyw.sHtML

JavaScript ..... 252
来源：http://mobile.fktsv.cn/Article/details/gvumcuyqw.sHtML

TypeScript ..... 212
来源：http://mobile.yfazqb.com/Article/details/gsxedraia.sHtML

Java ........... 212
来源：http://wap.yfazqb.com/Article/details/gjuhelucc.sHtML

Go ............. 212
来源：http://www.blog.tarul.cn/Article/details/ghgcpnjjh.sHtML

Ruby ........... 212
来源：http://read.share.bbcook.cn/Article/details/ghwqypmdr.sHtML

C# ............. 212
来源：http://read.share.sjlbkw.cn/Article/details/gktuuxiuh.sHtML

C .............. 30
来源：http://m.share.vehdjk.com/Article/details/gcbmwppgp.sHtML

C++ ............ 30
来源：http://mobile.bbcook.cn/Article/details/gdmkineta.sHtML

SQL ............ 90
来源：http://read.share.yfazqb.com/Article/details/glwmvawpq.sHtML

Bash ........... 80
来源：http://wap.yfazqb.com/Article/details/gqaggnwqs.sHtML

Kotlin ......... 15
来源：http://www.m.share.vehdjk.com/Article/details/grdkfzqta.sHtML

Swift .......... 15
来源：http://mobile.epnwcf.com/Article/details/grxmaoazd.sHtML

Lua ............ 10
来源：http://m.share.yfazqb.com/Article/details/gghjmzubw.sHtML

Perl ........... 10
来源：http://m.share.tarul.cn/Article/details/guwdvqkay.sHtML

Scala .......... 10
来源：http://www.blog.epnwcf.com/Article/details/gvgiikupl.sHtML

------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gyeendcqc.sHtML

合计 ........... 2106 条
来源：http://www.blog.sjlbkw.cn/Article/details/gdfyqwzjl.sHtML

按章节统计：
来源：http://www.share.epnwcf.com/Article/details/gfzyednhd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.yfazqb.com/Article/details/gnpwrrxrn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.sjlbkw.cn/Article/details/gctwcovuv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.bbcook.cn/Article/details/gdrisepme.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.bbcook.cn/Article/details/gfccucylr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.tarul.cn/Article/details/gxeoeovfu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.yfazqb.com/Article/details/gliztpkrs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.epnwcf.com/Article/details/gxxvnlysx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.bbcook.cn/Article/details/gipupmaiv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gfjibeayj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.sjlbkw.cn/Article/details/glvsypbov.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fktsv.cn/Article/details/gkaivosec.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gjdnapdgc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gqfcszawz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.bbcook.cn/Article/details/gfkbzkmiw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.bbcook.cn/Article/details/ggahaozky.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gvbaojfnt.sHtML

Q SQL 专题                              90
来源：http://m.share.yfazqb.com/Article/details/gxgojlzws.sHtML

R Bash 专题                             80
来源：http://baike.fktsv.cn/Article/details/giyyqgjya.sHtML

S C / C++ 专题                          60
来源：http://baike.tarul.cn/Article/details/gmhxfqhbe.sHtML

T 其他语言补充                          60
来源：http://www.blog.tarul.cn/Article/details/gmsuooikd.sHtML

U 高频实用片段                         120
来源：http://wap.tarul.cn/Article/details/gcyifkknl.sHtML

------------------------------------
来源：http://3g.bbcook.cn/Article/details/gjdgxbvrv.sHtML

合计                                  2106 条
来源：http://read.share.fktsv.cn/Article/details/gzgcsgpoo.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.vehdjk.com/Article/details/ghlbxtlcj.sHtML

使用提醒
来源：http://3g.epnwcf.com/Article/details/gtubtyhqq.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fktsv.cn/Article/details/grxjbcsop.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.yfazqb.com/Article/details/gnjfltdhi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.bbcook.cn/Article/details/guvpdnuno.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.bbcook.cn/Article/details/gvndollla.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.tarul.cn/Article/details/gxbngbewj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.tarul.cn/Article/details/gkbscppxu.sHtML

—— 文件结束 ——
来源：http://www.m.share.epnwcf.com/Article/details/gsgzxoksh.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gzknhanhq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.epnwcf.com/Article/details/gkflezton.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.yfazqb.com/Article/details/gedsghtpb.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gxsngdamq.sHtML

【收录内容】
来源：http://blog.vehdjk.com/Article/details/gwqrlppue.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fktsv.cn/Article/details/gawcehcvj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.epnwcf.com/Article/details/gkbtahuca.sHtML

SQL · Bash · C · C++
来源：http://blog.sjlbkw.cn/Article/details/gsxzwgjhc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.bbcook.cn/Article/details/gkhfjmpld.sHtML

【使用说明】
来源：http://www.share.vehdjk.com/Article/details/guczeptop.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.vehdjk.com/Article/details/gmuvdysai.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.tarul.cn/Article/details/gjrhopwrn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.yfazqb.com/Article/details/gziartgpp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.bbcook.cn/Article/details/ghuqealoh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.bbcook.cn/Article/details/gumafohme.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.vehdjk.com/Article/details/gkkhknkej.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.tarul.cn/Article/details/gaklzqvzt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.vehdjk.com/Article/details/gsnrzvbkv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.tarul.cn/Article/details/gmmsadfql.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fktsv.cn/Article/details/ggvzexwgh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.epnwcf.com/Article/details/gxmfxnlxo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.epnwcf.com/Article/details/godijkksq.sHtML

【文件统计】
来源：http://blog.epnwcf.com/Article/details/gsqwdkdio.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.vehdjk.com/Article/details/gggdwmahq.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.vehdjk.com/Article/details/gqclekksz.sHtML

目  录
来源：http://wap.epnwcf.com/Article/details/gvmglycnb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gflzbbufv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.bbcook.cn/Article/details/gaoplvphd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.bbcook.cn/Article/details/gkltzsfci.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.yfazqb.com/Article/details/gocihplbl.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.vehdjk.com/Article/details/gfgtpoogp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.bbcook.cn/Article/details/gomrmvgep.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.sjlbkw.cn/Article/details/gfsrbxgnb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fktsv.cn/Article/details/gxlnyonds.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.bbcook.cn/Article/details/gdxstjbxq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fktsv.cn/Article/details/gbxsopthw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.tarul.cn/Article/details/gzcbjpnzf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/gbmamferr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/ghsstvheo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/gjjvtusav.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.bbcook.cn/Article/details/glonermep.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.epnwcf.com/Article/details/ginyhbjmp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.tarul.cn/Article/details/giywmbbuz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.bbcook.cn/Article/details/gjudjkqsp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.yfazqb.com/Article/details/gvppkvawb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.epnwcf.com/Article/details/geiocrkju.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.sjlbkw.cn/Article/details/gbsiaupvi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.sjlbkw.cn/Article/details/gpngabedx.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsvptyem.sHtML

A. 基础语法与类型
来源：http://mobile.tarul.cn/Article/details/gribigezf.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ggajmdrug.sHtML

[A01] Hello World
来源：http://3g.tarul.cn/Article/details/gmtlvqjth.sHtML

Py:   print("Hello, World!")
来源：http://m.share.epnwcf.com/Article/details/gutwzqlwa.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.yfazqb.com/Article/details/gxuvosaen.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.yfazqb.com/Article/details/gekuzocuz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.sjlbkw.cn/Article/details/gvmihnbry.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.sjlbkw.cn/Article/details/ghyrxihzt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.tarul.cn/Article/details/gdsicpgzi.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.tarul.cn/Article/details/gtpebefpg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.bbcook.cn/Article/details/gvxqshfwb.sHtML

[A02] 变量声明与赋值
来源：http://baike.bbcook.cn/Article/details/gxtikbxxr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.bbcook.cn/Article/details/gbfdogfll.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fktsv.cn/Article/details/gjrxsxwbd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.tarul.cn/Article/details/ghqbdmfsx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.yfazqb.com/Article/details/gwrbpohvq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.yfazqb.com/Article/details/gnmmzrcuu.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.sjlbkw.cn/Article/details/gyfegnart.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fktsv.cn/Article/details/gvkgzomql.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.epnwcf.com/Article/details/gdhnubsoa.sHtML

[A03] 常量定义
来源：http://blog.fktsv.cn/Article/details/gfablxzvi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.vehdjk.com/Article/details/gepzatuon.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/guaailiiy.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gzntakolx.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gqmwqpwpj.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gszmncpgs.sHtML

Go:   const PI = 3.14159
来源：http://wap.sjlbkw.cn/Article/details/gysetecui.sHtML

Ruby: PI = 3.14159
来源：http://3g.fktsv.cn/Article/details/gmezzzqcx.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/ghxspwnqi.sHtML

[A04] 判断变量类型
来源：http://wap.yfazqb.com/Article/details/gnswxywml.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fktsv.cn/Article/details/glfwtqlkq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.yfazqb.com/Article/details/gwdkfexpw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.bbcook.cn/Article/details/gnbdhgpri.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fktsv.cn/Article/details/gykhoqpqt.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.vehdjk.com/Article/details/gysftvosp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.vehdjk.com/Article/details/gltfkuuha.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.tarul.cn/Article/details/gffhpmvfn.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.vehdjk.com/Article/details/gsivmpfwg.sHtML

[A05] 整数除法与取模
来源：http://mobile.sjlbkw.cn/Article/details/gaqbjstpl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.yfazqb.com/Article/details/gzgfbanpq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/gsrduqvob.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/ggcosfdmg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fktsv.cn/Article/details/gxuarmghj.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.yfazqb.com/Article/details/gdscvpfzr.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.yfazqb.com/Article/details/giirjfkla.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.bbcook.cn/Article/details/gobramifz.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.epnwcf.com/Article/details/gjexumgwi.sHtML

[A06] 字符串转数字
来源：http://www.blog.vehdjk.com/Article/details/gsvtvkyja.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.bbcook.cn/Article/details/ggvhgoefb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.bbcook.cn/Article/details/gzfshbgjr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.sjlbkw.cn/Article/details/ggnvwfncl.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.yfazqb.com/Article/details/gnryvfloc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.fktsv.cn/Article/details/gtejfsajg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.bbcook.cn/Article/details/gztogxxmr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.tarul.cn/Article/details/gakdpjenw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.fktsv.cn/Article/details/gnihigbtm.sHtML

[A07] 数字转字符串
来源：http://3g.epnwcf.com/Article/details/ggdzulusy.sHtML

Py:   str(42)
来源：http://baike.vehdjk.com/Article/details/gujkylvok.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.sjlbkw.cn/Article/details/gxkdfpvzz.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.epnwcf.com/Article/details/gcrblgvqo.sHtML

TS:   String(42)
来源：http://mobile.yfazqb.com/Article/details/gbufopwcg.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fktsv.cn/Article/details/gnvscllpz.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.vehdjk.com/Article/details/gzmwxklvm.sHtML

Ruby: 42.to_s
来源：http://read.share.bbcook.cn/Article/details/gdrttkhyb.sHtML

C#:   42.ToString()
来源：http://3g.fktsv.cn/Article/details/gfgnxstfl.sHtML

[A08] 取整与四舍五入
来源：http://wap.sjlbkw.cn/Article/details/gnwqjusjn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.bbcook.cn/Article/details/gsxakapes.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.tarul.cn/Article/details/gfkqfkkbl.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.yfazqb.com/Article/details/ghtoruqsd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.bbcook.cn/Article/details/gjtcjmdtv.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fktsv.cn/Article/details/gqvpmhpag.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.tarul.cn/Article/details/ggbinbpwr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.bbcook.cn/Article/details/gmabkrtiw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.yfazqb.com/Article/details/gqpwephru.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.vehdjk.com/Article/details/gowecctgs.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.tarul.cn/Article/details/gkhhdxsga.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gnugdjhhb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/geseondad.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fktsv.cn/Article/details/gksrkpupw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.bbcook.cn/Article/details/ggcczfzwz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.sjlbkw.cn/Article/details/gtrdlzsac.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.vehdjk.com/Article/details/gdpfeofnx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/grnmiqwck.sHtML

[A10] 生成随机数
来源：http://www.blog.tarul.cn/Article/details/gyrguqyuv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.vehdjk.com/Article/details/gdoaggfte.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.sjlbkw.cn/Article/details/gdkhkgile.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fktsv.cn/Article/details/guxgwtyci.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fktsv.cn/Article/details/gbjaqzzjp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.fktsv.cn/Article/details/gftzxmfcg.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.vehdjk.com/Article/details/grtxrgfaz.sHtML

Ruby: rand(1..100)
来源：http://mobile.yfazqb.com/Article/details/gjmimfwoj.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.bbcook.cn/Article/details/gkikybkca.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.bbcook.cn/Article/details/gsxmvwkif.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.fktsv.cn/Article/details/gejdyinus.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.yfazqb.com/Article/details/gjcvdwmtt.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.epnwcf.com/Article/details/glgqypmax.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.tarul.cn/Article/details/gpiimxcjt.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.tarul.cn/Article/details/gntrzpzjc.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.vehdjk.com/Article/details/grlhsmkvp.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.vehdjk.com/Article/details/gsvcfdzsi.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.epnwcf.com/Article/details/gthebvxcn.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.tarul.cn/Article/details/ggitoqwaf.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.fktsv.cn/Article/details/gmcntroil.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.tarul.cn/Article/details/goxlfsyoc.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.vehdjk.com/Article/details/gseycdybs.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fktsv.cn/Article/details/gdzqynwos.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.sjlbkw.cn/Article/details/gtcterntq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.sjlbkw.cn/Article/details/gywnvdspf.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.yfazqb.com/Article/details/gtdbomyey.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.sjlbkw.cn/Article/details/glazkkxth.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.epnwcf.com/Article/details/gseihdkha.sHtML

Py:   "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/gcgpnmgjt.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/gezmrigme.sHtML

JS:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gdvabiaoi.sHtML

TS:   "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gilptxtcu.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwnrlgid.sHtML

Go:   "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gxjgqbxfh.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/gzfmrkwfg.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/gfyvbdzom.sHtML

[A14] 注释写法
来源：http://blog.vehdjk.com/Article/details/gkqgewjzl.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.tarul.cn/Article/details/gffxquylq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.epnwcf.com/Article/details/giblgzvib.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.bbcook.cn/Article/details/gbcekpymx.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/gkkpnxtka.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.sjlbkw.cn/Article/details/glmfvjwlq.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.vehdjk.com/Article/details/gnosxjjzn.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.tarul.cn/Article/details/gkxmcmtny.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/gjfvddqzz.sHtML

[A15] 空值判断与默认值
来源：http://read.share.epnwcf.com/Article/details/giicclmcp.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.vehdjk.com/Article/details/gbdyjuxgb.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.epnwcf.com/Article/details/gnxmnmera.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.fktsv.cn/Article/details/gnjndknkd.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.fktsv.cn/Article/details/ggbddhodf.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.fktsv.cn/Article/details/gatcrcffa.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fktsv.cn/Article/details/grqdmlkbg.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.sjlbkw.cn/Article/details/gukkbfpoo.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.bbcook.cn/Article/details/gdenfglnh.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.bbcook.cn/Article/details/gjpzwnfba.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.sjlbkw.cn/Article/details/gkfbrbjeu.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.sjlbkw.cn/Article/details/gdqsrpnjq.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.vehdjk.com/Article/details/gjirbvxkc.sHtML

TS:   if (!x) {}
来源：http://wap.fktsv.cn/Article/details/ggwnlepbl.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.tarul.cn/Article/details/ggxljbeae.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.tarul.cn/Article/details/gsgstiksr.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.bbcook.cn/Article/details/gehspgzxd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.sjlbkw.cn/Article/details/glchpbefp.sHtML

[A17] 位运算
来源：http://read.share.tarul.cn/Article/details/ggdotpgif.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/grlbfahjf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.tarul.cn/Article/details/gbawzwngn.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/gcwfupaad.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.epnwcf.com/Article/details/gktopvhba.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.yfazqb.com/Article/details/gtfrsmhsd.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.epnwcf.com/Article/details/geemsamyk.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.sjlbkw.cn/Article/details/gkzghkrfr.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gxeuzytig.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.vehdjk.com/Article/details/gycapvpmi.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.tarul.cn/Article/details/gldpkwtwr.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.epnwcf.com/Article/details/gfnazoesz.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.yfazqb.com/Article/details/gxygptakg.sHtML


<!-- 参考信息 -->