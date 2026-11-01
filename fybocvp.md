代发 wailian999

[U101] JS：classList 操作
来源：http://baike.fktsv.cn/Article/details/guxsqnxgf.sHtML

el.classList.toggle("active")
来源：http://www.m.share.epnwcf.com/Article/details/gcmkkxgrq.sHtML

[U102] JS：本地存储
来源：http://wap.epnwcf.com/Article/details/grpdckkjy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fktsv.cn/Article/details/gfosjmccy.sHtML

[U103] JS：定时器
来源：http://mobile.tarul.cn/Article/details/gprxlckyl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.vehdjk.com/Article/details/gzjfrglgf.sHtML

[U104] JS：防抖
来源：http://wap.vehdjk.com/Article/details/gckytiyka.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/gcqgfahfx.sHtML

[U105] JS：节流
来源：http://blog.sjlbkw.cn/Article/details/gzjotpspp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.vehdjk.com/Article/details/gyyhtthfe.sHtML

[U106] JS：日期格式化
来源：http://3g.tarul.cn/Article/details/gnlqrqnbb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.epnwcf.com/Article/details/gooehuxsj.sHtML

[U107] JS：数字千分位
来源：http://read.share.vehdjk.com/Article/details/glbpuiwny.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fktsv.cn/Article/details/gmwgovhgf.sHtML

[U108] JS：随机整数
来源：http://3g.fktsv.cn/Article/details/goaozjsfu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.sjlbkw.cn/Article/details/gqmaiiasv.sHtML

[U109] JS：数组分组
来源：http://baike.vehdjk.com/Article/details/goqgomues.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.epnwcf.com/Article/details/ggrsouopw.sHtML

[U110] JS：数组分块
来源：http://read.share.sjlbkw.cn/Article/details/gfvknvsjk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.yfazqb.com/Article/details/gtuxhaoaz.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.vehdjk.com/Article/details/gpxktuwvq.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.yfazqb.com/Article/details/gfbhzvzno.sHtML

[U112] JS：字符串补位
来源：http://www.blog.vehdjk.com/Article/details/gedjepwdc.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/ghfwzpdiv.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.bbcook.cn/Article/details/gzffohsqk.sHtML

s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gxieionms.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.yfazqb.com/Article/details/gezqxazbu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.tarul.cn/Article/details/gzmlpugdt.sHtML

[U115] JS：生成 UUID
来源：http://www.share.sjlbkw.cn/Article/details/gkwnogpyd.sHtML

crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/ghdkfmjur.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.bbcook.cn/Article/details/gzdwpivue.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.bbcook.cn/Article/details/ghwodzpff.sHtML

[U117] JS：单元测试
来源：http://m.share.tarul.cn/Article/details/gulowslpw.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.tarul.cn/Article/details/gbidwwcjm.sHtML

[U118] JS：开发服务器
来源：http://blog.bbcook.cn/Article/details/gkswywurd.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.epnwcf.com/Article/details/gnothbcnn.sHtML

[U119] JS：生产构建
来源：http://www.share.vehdjk.com/Article/details/ggkguebnk.sHtML

npx vite build
来源：http://m.share.yfazqb.com/Article/details/gbeblzync.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.vehdjk.com/Article/details/gtntvcgjc.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.sjlbkw.cn/Article/details/goamkkdlh.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gbfmkimxm.sHtML

统计汇总
来源：http://mobile.bbcook.cn/Article/details/gdoqlmfmb.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/glpbjukjo.sHtML

按语言统计（条）：
来源：http://read.share.epnwcf.com/Article/details/gdyolwjau.sHtML

Python ......... 252
来源：http://www.m.share.fktsv.cn/Article/details/gxlpktrnu.sHtML

PHP ............ 252
来源：http://read.share.epnwcf.com/Article/details/gcifeplba.sHtML

JavaScript ..... 252
来源：http://wap.yfazqb.com/Article/details/gwgqqugjg.sHtML

TypeScript ..... 212
来源：http://m.share.sjlbkw.cn/Article/details/ggradjdmb.sHtML

Java ........... 212
来源：http://www.m.share.tarul.cn/Article/details/gmndkwcrt.sHtML

Go ............. 212
来源：http://mobile.vehdjk.com/Article/details/ghwmynncd.sHtML

Ruby ........... 212
来源：http://wap.yfazqb.com/Article/details/gsweqngva.sHtML

C# ............. 212
来源：http://read.share.fktsv.cn/Article/details/gwwzuaxdq.sHtML

C .............. 30
来源：http://baike.epnwcf.com/Article/details/gfiflfcoe.sHtML

C++ ............ 30
来源：http://www.blog.bbcook.cn/Article/details/gnnwdejcp.sHtML

SQL ............ 90
来源：http://www.blog.sjlbkw.cn/Article/details/gwoqjvmyo.sHtML

Bash ........... 80
来源：http://www.share.tarul.cn/Article/details/gvblojxvk.sHtML

Kotlin ......... 15
来源：http://www.m.share.tarul.cn/Article/details/grmceivvi.sHtML

Swift .......... 15
来源：http://www.blog.tarul.cn/Article/details/gwavetblr.sHtML

Lua ............ 10
来源：http://3g.vehdjk.com/Article/details/gmiwjmiwl.sHtML

Perl ........... 10
来源：http://read.share.fktsv.cn/Article/details/gpgdtxzzo.sHtML

Scala .......... 10
来源：http://www.blog.yfazqb.com/Article/details/gllgqmixb.sHtML

------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gmdixlquw.sHtML

合计 ........... 2106 条
来源：http://blog.yfazqb.com/Article/details/glgixojyk.sHtML

按章节统计：
来源：http://m.share.sjlbkw.cn/Article/details/gfcqhjxtj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fktsv.cn/Article/details/grgrewukx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.tarul.cn/Article/details/goxhmojlj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.yfazqb.com/Article/details/gabeesjwn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.yfazqb.com/Article/details/gsoqmjzdu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.yfazqb.com/Article/details/gskqkqvic.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.bbcook.cn/Article/details/gcelnyvku.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.bbcook.cn/Article/details/gppdzclbn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.vehdjk.com/Article/details/gxnxsbrsl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/grchuyyby.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.tarul.cn/Article/details/gjqxpzgnh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gceyujxdx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/gmgcowlbf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/gmorvtyds.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.yfazqb.com/Article/details/gmtbjplub.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.tarul.cn/Article/details/gqmojwuqd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gkadnpasi.sHtML

Q SQL 专题                              90
来源：http://baike.tarul.cn/Article/details/gzbcrflgi.sHtML

R Bash 专题                             80
来源：http://wap.yfazqb.com/Article/details/gjdbbsdvg.sHtML

S C / C++ 专题                          60
来源：http://www.blog.vehdjk.com/Article/details/gqkospqld.sHtML

T 其他语言补充                          60
来源：http://baike.vehdjk.com/Article/details/goisbiqnf.sHtML

U 高频实用片段                         120
来源：http://3g.epnwcf.com/Article/details/gqdfperxv.sHtML

------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gljlinbvz.sHtML

合计                                  2106 条
来源：http://read.share.vehdjk.com/Article/details/gykqpzfry.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.vehdjk.com/Article/details/goqpswiha.sHtML

使用提醒
来源：http://3g.bbcook.cn/Article/details/gtwjnphhz.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gecdrhhwl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.vehdjk.com/Article/details/gmvmlmnnm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.epnwcf.com/Article/details/ghahoncgx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.vehdjk.com/Article/details/gkuuqnwea.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.vehdjk.com/Article/details/gjbhinejs.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.epnwcf.com/Article/details/gvzozvwce.sHtML

—— 文件结束 ——
来源：http://3g.yfazqb.com/Article/details/gbdiymmif.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gdzvlmskr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fktsv.cn/Article/details/glsgclqsj.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fktsv.cn/Article/details/gwwxhujqz.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gunpxafte.sHtML

【收录内容】
来源：http://wap.bbcook.cn/Article/details/gumenklxi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fktsv.cn/Article/details/guqpkjihn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.vehdjk.com/Article/details/gvuxclueq.sHtML

SQL · Bash · C · C++
来源：http://mobile.vehdjk.com/Article/details/gvdqqbyag.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.yfazqb.com/Article/details/gfdwayqri.sHtML

【使用说明】
来源：http://read.share.fktsv.cn/Article/details/gpinftntc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.vehdjk.com/Article/details/gscsrwblx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.sjlbkw.cn/Article/details/gyzsscyim.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.yfazqb.com/Article/details/gsnzhsufw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.bbcook.cn/Article/details/gsilogwcj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.vehdjk.com/Article/details/gfnkibwey.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.bbcook.cn/Article/details/gotcpzggd.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.epnwcf.com/Article/details/gnrueqhdi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.vehdjk.com/Article/details/gzfzizmjl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.tarul.cn/Article/details/gogifhmsa.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.vehdjk.com/Article/details/gzscwctkh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.vehdjk.com/Article/details/ggkrtvaek.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.vehdjk.com/Article/details/gddyrcvhl.sHtML

【文件统计】
来源：http://www.share.sjlbkw.cn/Article/details/gyccfsppw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.yfazqb.com/Article/details/gqccgjytk.sHtML

--------------------------------------------------------------------------------
来源：http://wap.yfazqb.com/Article/details/gsejtatre.sHtML

目  录
来源：http://baike.vehdjk.com/Article/details/gilxixcnk.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/gzpchcmqq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fktsv.cn/Article/details/gsmtrjqhu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.tarul.cn/Article/details/gbmszelme.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.yfazqb.com/Article/details/gaabggqju.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrylcrlf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.sjlbkw.cn/Article/details/gwqmitjaw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.vehdjk.com/Article/details/gqduiuspe.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.vehdjk.com/Article/details/gupjneevn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.epnwcf.com/Article/details/glfqqvcox.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/ggdcvqhod.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.bbcook.cn/Article/details/gxsbvidtv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.sjlbkw.cn/Article/details/gdoobnhrv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.tarul.cn/Article/details/gtntfljub.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/gxdkpwkic.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.bbcook.cn/Article/details/gkqsnnccd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.bbcook.cn/Article/details/gcsaszcaq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/grausfyqk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.tarul.cn/Article/details/govmxxwnr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.epnwcf.com/Article/details/gayzkzvvb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.vehdjk.com/Article/details/gctvqymls.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.vehdjk.com/Article/details/gagnxbcaj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.epnwcf.com/Article/details/grmjaenra.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gkhetxgnw.sHtML

A. 基础语法与类型
来源：http://www.blog.epnwcf.com/Article/details/gpxugouqu.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsxzpipe.sHtML

[A01] Hello World
来源：http://3g.sjlbkw.cn/Article/details/gjvqbptgg.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fktsv.cn/Article/details/glgjtnoin.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.epnwcf.com/Article/details/gnsqcddoi.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.sjlbkw.cn/Article/details/gygupczqu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.epnwcf.com/Article/details/gnerjylpg.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.yfazqb.com/Article/details/gbnbaneuc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.vehdjk.com/Article/details/gbausvlip.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.epnwcf.com/Article/details/ghgzmsgnk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.sjlbkw.cn/Article/details/gmufsajnv.sHtML

[A02] 变量声明与赋值
来源：http://m.share.yfazqb.com/Article/details/gsktniynz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fktsv.cn/Article/details/gpggirszc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.bbcook.cn/Article/details/gnvshvwzm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gdofiizeq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.sjlbkw.cn/Article/details/gtmiagfbg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.sjlbkw.cn/Article/details/gzlcqxqyb.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.vehdjk.com/Article/details/gzwkfcxut.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.epnwcf.com/Article/details/goaenfrgx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.epnwcf.com/Article/details/gowyfulad.sHtML

[A03] 常量定义
来源：http://mobile.sjlbkw.cn/Article/details/gqwikytsb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.epnwcf.com/Article/details/glamounem.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gmfgrjyhm.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gshxrfpmm.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gettznxla.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/glwafdqim.sHtML

Go:   const PI = 3.14159
来源：http://wap.bbcook.cn/Article/details/gybzbkdff.sHtML

Ruby: PI = 3.14159
来源：http://mobile.tarul.cn/Article/details/gvkbqvuqn.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gwyohvvyv.sHtML

[A04] 判断变量类型
来源：http://3g.yfazqb.com/Article/details/gndbytfrx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.epnwcf.com/Article/details/gmeohtjrf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.bbcook.cn/Article/details/ghnqihgeq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.bbcook.cn/Article/details/gnkcnevzz.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.epnwcf.com/Article/details/ggqqpuwxu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.sjlbkw.cn/Article/details/gcwandetn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.epnwcf.com/Article/details/gmmgkejeb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.yfazqb.com/Article/details/gnyyeevin.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fktsv.cn/Article/details/gwiufsuad.sHtML

[A05] 整数除法与取模
来源：http://mobile.bbcook.cn/Article/details/gzzesvjde.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.epnwcf.com/Article/details/gblbyvkps.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fktsv.cn/Article/details/gsaafybro.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.vehdjk.com/Article/details/gdvxwkmzb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/glltzagxr.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/gcpvjkyca.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.sjlbkw.cn/Article/details/gcatgjzhh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gzhosknoz.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gjqngkdac.sHtML

[A06] 字符串转数字
来源：http://m.share.bbcook.cn/Article/details/gmmvwzcrb.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.tarul.cn/Article/details/gmaljznlg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fktsv.cn/Article/details/gzipvajqc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.sjlbkw.cn/Article/details/ghiodbocn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.bbcook.cn/Article/details/gmeimukhs.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.bbcook.cn/Article/details/goguogkhk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.sjlbkw.cn/Article/details/gjxpihwdo.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.yfazqb.com/Article/details/gkwhjvurj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.yfazqb.com/Article/details/gdsimjnzn.sHtML

[A07] 数字转字符串
来源：http://read.share.tarul.cn/Article/details/gkltmwrar.sHtML

Py:   str(42)
来源：http://read.share.epnwcf.com/Article/details/gsosudjnv.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.bbcook.cn/Article/details/gcjuklepq.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.bbcook.cn/Article/details/gelkezqxh.sHtML

TS:   String(42)
来源：http://read.share.yfazqb.com/Article/details/gcbbgwoce.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.sjlbkw.cn/Article/details/geevamrld.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxygmwkff.sHtML

Ruby: 42.to_s
来源：http://www.blog.sjlbkw.cn/Article/details/gxgywgykl.sHtML

C#:   42.ToString()
来源：http://m.share.tarul.cn/Article/details/gjxkyqwtm.sHtML

[A08] 取整与四舍五入
来源：http://www.share.tarul.cn/Article/details/gjjcasrst.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.yfazqb.com/Article/details/glzphuqtl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.bbcook.cn/Article/details/gpvzsacpd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.epnwcf.com/Article/details/glfyjyewm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.sjlbkw.cn/Article/details/gprqvoctx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.bbcook.cn/Article/details/gygjavolc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.tarul.cn/Article/details/gouciecqj.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.yfazqb.com/Article/details/gemawahfr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.yfazqb.com/Article/details/grolsoclq.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fktsv.cn/Article/details/getkuyylw.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/gckyphmkm.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gcyilirjw.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gxknyrxdt.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gcmgwyrtk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.tarul.cn/Article/details/giftvsgvt.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.fktsv.cn/Article/details/grnjtnout.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.bbcook.cn/Article/details/gxqbdjsja.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.bbcook.cn/Article/details/ggzqlajcz.sHtML

[A10] 生成随机数
来源：http://www.m.share.yfazqb.com/Article/details/goluvmqwo.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.tarul.cn/Article/details/guoharysa.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.bbcook.cn/Article/details/ghjltskon.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.tarul.cn/Article/details/gdxsklbni.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.vehdjk.com/Article/details/grjxhmkky.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.epnwcf.com/Article/details/gbuzjenzi.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fktsv.cn/Article/details/gqhyrsswa.sHtML

Ruby: rand(1..100)
来源：http://www.share.tarul.cn/Article/details/govnzetlb.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fktsv.cn/Article/details/grsrdzpyc.sHtML

[A11] 条件表达式（三元）
来源：http://wap.vehdjk.com/Article/details/gsecnaqux.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.tarul.cn/Article/details/gentrjyit.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.yfazqb.com/Article/details/gmbvjbugn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.sjlbkw.cn/Article/details/gtdrcalqj.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.epnwcf.com/Article/details/gacxksxvx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.bbcook.cn/Article/details/ganegamog.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.tarul.cn/Article/details/gkjtrftop.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.tarul.cn/Article/details/ghijwnmjq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.epnwcf.com/Article/details/govdxdjix.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.bbcook.cn/Article/details/gmzskavpf.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.yfazqb.com/Article/details/gffktqsbs.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.bbcook.cn/Article/details/gxavlcavg.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.fktsv.cn/Article/details/gebtagrtr.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.yfazqb.com/Article/details/gvilaalmr.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.tarul.cn/Article/details/gieilzehi.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.tarul.cn/Article/details/gainwpmfv.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.sjlbkw.cn/Article/details/gtlbwycoc.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fktsv.cn/Article/details/ghmgajcip.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.epnwcf.com/Article/details/gijgswzrf.sHtML

Py:   "第一行\n第二行"
来源：http://3g.tarul.cn/Article/details/gesodztbd.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.sjlbkw.cn/Article/details/gqcbhglfi.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/glmkdwpwu.sHtML

TS:   "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gvixmtnkw.sHtML

Java: "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/gbrwfdhkb.sHtML

Go:   "第一行\n第二行"
来源：http://baike.yfazqb.com/Article/details/gqdvaryjv.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.epnwcf.com/Article/details/gqzjbzjtw.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gzwxxdjdq.sHtML

[A14] 注释写法
来源：http://baike.tarul.cn/Article/details/gglijlvop.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.sjlbkw.cn/Article/details/gtdolsmbu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.vehdjk.com/Article/details/gjgbftsmd.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.epnwcf.com/Article/details/gcsxriasd.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/guhtesyix.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.sjlbkw.cn/Article/details/gwyzneilm.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.bbcook.cn/Article/details/grxmfsmki.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.bbcook.cn/Article/details/ggvptyllg.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.epnwcf.com/Article/details/gscbdszzd.sHtML

[A15] 空值判断与默认值
来源：http://read.share.sjlbkw.cn/Article/details/gzaunanmb.sHtML

Py:   value = data or "默认值"
来源：http://mobile.bbcook.cn/Article/details/gsgwszwnl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.vehdjk.com/Article/details/gndpmyzen.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.yfazqb.com/Article/details/gievluguq.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.tarul.cn/Article/details/gkgzmqkmc.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.yfazqb.com/Article/details/guxfkkpvn.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.vehdjk.com/Article/details/gqttzpuha.sHtML

Ruby: value = data || "默认值"
来源：http://wap.sjlbkw.cn/Article/details/gpiyyyiyb.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.tarul.cn/Article/details/glwetxvmw.sHtML

[A16] 真假值判断规则
来源：http://blog.tarul.cn/Article/details/gibnnleas.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fktsv.cn/Article/details/gvjzgkhor.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.vehdjk.com/Article/details/glqgoqmxp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.tarul.cn/Article/details/ghstjyzzx.sHtML

TS:   if (!x) {}
来源：http://mobile.tarul.cn/Article/details/gcpjlxyrz.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.tarul.cn/Article/details/gxdefupfp.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.vehdjk.com/Article/details/gyueatupl.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.bbcook.cn/Article/details/gxlafzrru.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.tarul.cn/Article/details/gesdyapjq.sHtML

[A17] 位运算
来源：http://www.m.share.yfazqb.com/Article/details/govnvqmbx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/gomtqdhpi.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.fktsv.cn/Article/details/gwsfcfjpq.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gkggvwewm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gadlrhmkn.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/ghhqecalh.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gegjusuaq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.yfazqb.com/Article/details/gdutaoqrm.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/ggdhelogy.sHtML


<!-- 参考信息 -->