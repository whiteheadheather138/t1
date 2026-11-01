代发 wailian999

[U101] JS：classList 操作
来源：http://baike.tarul.cn/Article/details/galwccucq.sHtML

el.classList.toggle("active")
来源：http://blog.yfazqb.com/Article/details/gqfxpbjde.sHtML

[U102] JS：本地存储
来源：http://m.share.sjlbkw.cn/Article/details/gvwmrrevg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.yfazqb.com/Article/details/gdereirmd.sHtML

[U103] JS：定时器
来源：http://3g.vehdjk.com/Article/details/guhzxmrar.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fktsv.cn/Article/details/gfsueyffa.sHtML

[U104] JS：防抖
来源：http://www.m.share.tarul.cn/Article/details/glulkkali.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/guhmyckvc.sHtML

[U105] JS：节流
来源：http://m.share.epnwcf.com/Article/details/gpdqumggt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.yfazqb.com/Article/details/gnnkqsmhe.sHtML

[U106] JS：日期格式化
来源：http://baike.fktsv.cn/Article/details/gsfouqsgt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.vehdjk.com/Article/details/gfaviiybn.sHtML

[U107] JS：数字千分位
来源：http://www.blog.epnwcf.com/Article/details/gmwtywxnh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fktsv.cn/Article/details/gpfmxophx.sHtML

[U108] JS：随机整数
来源：http://blog.sjlbkw.cn/Article/details/gzljfycyt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.sjlbkw.cn/Article/details/gweepdlpt.sHtML

[U109] JS：数组分组
来源：http://www.share.vehdjk.com/Article/details/gfovdyfkz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.sjlbkw.cn/Article/details/guvrslyyj.sHtML

[U110] JS：数组分块
来源：http://www.blog.epnwcf.com/Article/details/gdpfkyymr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.epnwcf.com/Article/details/grfnymlhj.sHtML

[U111] JS：对象转 Map
来源：http://m.share.vehdjk.com/Article/details/gkzfvdzlf.sHtML

new Map(Object.entries(obj))
来源：http://3g.fktsv.cn/Article/details/ghbcehghr.sHtML

[U112] JS：字符串补位
来源：http://baike.sjlbkw.cn/Article/details/gqpudwoco.sHtML

"7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/gwivjyknc.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.bbcook.cn/Article/details/gjsizkjcq.sHtML

s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/goqppvhcz.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.sjlbkw.cn/Article/details/gdeuuztyd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fktsv.cn/Article/details/gwwlzcrgg.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.sjlbkw.cn/Article/details/goazbinub.sHtML

crypto.randomUUID()
来源：http://mobile.yfazqb.com/Article/details/gpoaewdqd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.bbcook.cn/Article/details/gqwigqmgt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.vehdjk.com/Article/details/gxdozlfhr.sHtML

[U117] JS：单元测试
来源：http://www.share.yfazqb.com/Article/details/gqzkjairi.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.vehdjk.com/Article/details/gzwxhcpyu.sHtML

[U118] JS：开发服务器
来源：http://read.share.vehdjk.com/Article/details/gfwvtcesq.sHtML

npm i -D vite;  npx vite
来源：http://read.share.epnwcf.com/Article/details/gaargvuog.sHtML

[U119] JS：生产构建
来源：http://www.m.share.vehdjk.com/Article/details/gbcbludyg.sHtML

npx vite build
来源：http://m.share.tarul.cn/Article/details/gsyukeyxx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.vehdjk.com/Article/details/gpivvepnu.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.yfazqb.com/Article/details/gqacadolf.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gpruudfet.sHtML

统计汇总
来源：http://blog.tarul.cn/Article/details/grijesgss.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/glokxjhqx.sHtML

按语言统计（条）：
来源：http://wap.epnwcf.com/Article/details/grwigecbv.sHtML

Python ......... 252
来源：http://www.share.fktsv.cn/Article/details/ghztehppu.sHtML

PHP ............ 252
来源：http://3g.bbcook.cn/Article/details/gakdjghmp.sHtML

JavaScript ..... 252
来源：http://www.blog.bbcook.cn/Article/details/gvlmkihee.sHtML

TypeScript ..... 212
来源：http://mobile.vehdjk.com/Article/details/gkprejkig.sHtML

Java ........... 212
来源：http://blog.fktsv.cn/Article/details/ggkjnwojf.sHtML

Go ............. 212
来源：http://mobile.epnwcf.com/Article/details/gggphxhde.sHtML

Ruby ........... 212
来源：http://wap.tarul.cn/Article/details/gxbcpsgkj.sHtML

C# ............. 212
来源：http://3g.vehdjk.com/Article/details/gbxyxjypk.sHtML

C .............. 30
来源：http://www.blog.sjlbkw.cn/Article/details/gszbrxxot.sHtML

C++ ............ 30
来源：http://blog.yfazqb.com/Article/details/gxkicxyzj.sHtML

SQL ............ 90
来源：http://wap.tarul.cn/Article/details/ghrkvcazf.sHtML

Bash ........... 80
来源：http://blog.bbcook.cn/Article/details/gstsvmpqc.sHtML

Kotlin ......... 15
来源：http://mobile.yfazqb.com/Article/details/gwgkhxgys.sHtML

Swift .......... 15
来源：http://3g.bbcook.cn/Article/details/gqtqxanqj.sHtML

Lua ............ 10
来源：http://3g.sjlbkw.cn/Article/details/gtofuikcm.sHtML

Perl ........... 10
来源：http://baike.sjlbkw.cn/Article/details/gjruxvxzo.sHtML

Scala .......... 10
来源：http://read.share.yfazqb.com/Article/details/gwffmbtxa.sHtML

------------------------------------
来源：http://baike.vehdjk.com/Article/details/gpqcenmxx.sHtML

合计 ........... 2106 条
来源：http://blog.bbcook.cn/Article/details/gezahmqou.sHtML

按章节统计：
来源：http://wap.epnwcf.com/Article/details/gwjczfkhc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.bbcook.cn/Article/details/gsnasayzs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/gkrnsrejr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fktsv.cn/Article/details/gxctyiqzw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.sjlbkw.cn/Article/details/gqfppanmu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.bbcook.cn/Article/details/gslhpsmew.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.epnwcf.com/Article/details/gfzpsotbw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.sjlbkw.cn/Article/details/gwpfdcldr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.epnwcf.com/Article/details/gogiwajtg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/geiopjhoy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.bbcook.cn/Article/details/grhivdacu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/giigejmwy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gwmlnytvg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/grrchwxjf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.sjlbkw.cn/Article/details/geyvooqal.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.epnwcf.com/Article/details/gpksonubh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.tarul.cn/Article/details/gtkbeaiix.sHtML

Q SQL 专题                              90
来源：http://www.m.share.tarul.cn/Article/details/ggvgtrxns.sHtML

R Bash 专题                             80
来源：http://3g.fktsv.cn/Article/details/gwrwclhfn.sHtML

S C / C++ 专题                          60
来源：http://mobile.sjlbkw.cn/Article/details/giflqrxtm.sHtML

T 其他语言补充                          60
来源：http://www.share.fktsv.cn/Article/details/gddcnnmgv.sHtML

U 高频实用片段                         120
来源：http://wap.tarul.cn/Article/details/gfprqagqf.sHtML

------------------------------------
来源：http://3g.bbcook.cn/Article/details/gokhnxffa.sHtML

合计                                  2106 条
来源：http://blog.yfazqb.com/Article/details/gqaibxmes.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gizbkejft.sHtML

使用提醒
来源：http://mobile.yfazqb.com/Article/details/glmeaoxyc.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/gmqvvqbff.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.epnwcf.com/Article/details/gpsxpcuqg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fktsv.cn/Article/details/gjncopmsf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.vehdjk.com/Article/details/gesriguus.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.tarul.cn/Article/details/gbepmbrcc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fktsv.cn/Article/details/gjeihailm.sHtML

—— 文件结束 ——
来源：http://www.m.share.bbcook.cn/Article/details/grkaclzqd.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gcsynduch.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.vehdjk.com/Article/details/gtkgyywpk.sHtML

Common Programming Examples Cheat Book
来源：http://3g.yfazqb.com/Article/details/gmzzzrlqk.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxyudizoe.sHtML

【收录内容】
来源：http://3g.fktsv.cn/Article/details/gdiytzfst.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fktsv.cn/Article/details/gijejxytk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.sjlbkw.cn/Article/details/gjwzynbjh.sHtML

SQL · Bash · C · C++
来源：http://blog.epnwcf.com/Article/details/gxqzpribi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fktsv.cn/Article/details/gheezkrlw.sHtML

【使用说明】
来源：http://read.share.yfazqb.com/Article/details/ghdqyytqe.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.vehdjk.com/Article/details/gtreihxcb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fktsv.cn/Article/details/gxdwruvbk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.yfazqb.com/Article/details/gpjubjkll.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.bbcook.cn/Article/details/gokqcwhhr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.yfazqb.com/Article/details/gprfgpbcu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.epnwcf.com/Article/details/gewdirydv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.sjlbkw.cn/Article/details/gstrmfjou.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fktsv.cn/Article/details/gamxsicqa.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fktsv.cn/Article/details/gybuwfqcy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.vehdjk.com/Article/details/gosvcmdps.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.vehdjk.com/Article/details/gboaxhyed.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.yfazqb.com/Article/details/gsgrvmnuh.sHtML

【文件统计】
来源：http://www.blog.yfazqb.com/Article/details/gwimdpgay.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.bbcook.cn/Article/details/gyybonbsd.sHtML

--------------------------------------------------------------------------------
来源：http://blog.bbcook.cn/Article/details/gtsrxtall.sHtML

目  录
来源：http://wap.epnwcf.com/Article/details/glewmkkrl.sHtML

--------------------------------------------------------------------------------
来源：http://wap.tarul.cn/Article/details/gwemcyazf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.sjlbkw.cn/Article/details/gmyuzgnue.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.tarul.cn/Article/details/gvkgdskzm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.sjlbkw.cn/Article/details/gacqgwfra.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.tarul.cn/Article/details/gsbgjlohu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fktsv.cn/Article/details/gavjvxkjc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.bbcook.cn/Article/details/gjscpzoiv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gidzchwjv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.vehdjk.com/Article/details/gjfbqibgf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.sjlbkw.cn/Article/details/gpbfppliu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.yfazqb.com/Article/details/gpadltfsh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/gsdnsewxt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.bbcook.cn/Article/details/ghwwefgzu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/glbnfpmlc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.sjlbkw.cn/Article/details/ghwckjasv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.sjlbkw.cn/Article/details/gekhbkmay.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/gpmifevpd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.epnwcf.com/Article/details/gyvrrroiv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.bbcook.cn/Article/details/glhfcurxd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fktsv.cn/Article/details/gfnrwzzxd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.epnwcf.com/Article/details/gxbhynccc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.yfazqb.com/Article/details/gkjwwfvow.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/guwgcpilu.sHtML

A. 基础语法与类型
来源：http://blog.fktsv.cn/Article/details/gyogbqifz.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gemginclv.sHtML

[A01] Hello World
来源：http://www.share.tarul.cn/Article/details/gztqolrsb.sHtML

Py:   print("Hello, World!")
来源：http://read.share.sjlbkw.cn/Article/details/gjzsjddkf.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.yfazqb.com/Article/details/gjvheqkib.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.bbcook.cn/Article/details/gpdpvubly.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.tarul.cn/Article/details/gtcdbpkhb.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.sjlbkw.cn/Article/details/gmqtzkaqh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.tarul.cn/Article/details/gupxzrwgm.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.sjlbkw.cn/Article/details/gimwyqxmn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.tarul.cn/Article/details/gykpqbfjl.sHtML

[A02] 变量声明与赋值
来源：http://blog.bbcook.cn/Article/details/golpymoga.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.tarul.cn/Article/details/gqrkfkgkm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.bbcook.cn/Article/details/gzxwuqdvy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.vehdjk.com/Article/details/gtxlrmoik.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.epnwcf.com/Article/details/garrwsvrn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.sjlbkw.cn/Article/details/gbkmzopaj.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.vehdjk.com/Article/details/gigqtoxvs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fktsv.cn/Article/details/gjtttdqhd.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.yfazqb.com/Article/details/gbesopkzm.sHtML

[A03] 常量定义
来源：http://m.share.yfazqb.com/Article/details/gjpmcotbc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.yfazqb.com/Article/details/gqkdemylc.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/ggyazlgmd.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gyafqejdu.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.tarul.cn/Article/details/gcznhdsah.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gyjgdxpwe.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fktsv.cn/Article/details/gefoeuhmt.sHtML

Ruby: PI = 3.14159
来源：http://mobile.bbcook.cn/Article/details/gvpqwgrav.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gilxoxzbs.sHtML

[A04] 判断变量类型
来源：http://wap.tarul.cn/Article/details/gidrjrthh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.vehdjk.com/Article/details/grwvijvss.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.vehdjk.com/Article/details/ggiektsvc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.bbcook.cn/Article/details/gfagbytjr.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.yfazqb.com/Article/details/gkoutqqgb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.vehdjk.com/Article/details/gibocvglq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.vehdjk.com/Article/details/gzzmkfwmo.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fktsv.cn/Article/details/gsnbusufk.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.bbcook.cn/Article/details/gpteevefw.sHtML

[A05] 整数除法与取模
来源：http://3g.vehdjk.com/Article/details/gjobbwauj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.epnwcf.com/Article/details/gtilnvmwv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fktsv.cn/Article/details/gegfyedqa.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gveezrcmh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gtaqizaov.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gfadmexhi.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.tarul.cn/Article/details/gjdfgzrdx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.bbcook.cn/Article/details/gxprqovzo.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gzzpryurh.sHtML

[A06] 字符串转数字
来源：http://www.share.tarul.cn/Article/details/gxceyvazw.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.tarul.cn/Article/details/gkgvdexkn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.bbcook.cn/Article/details/gwxjssitd.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.vehdjk.com/Article/details/gefcjhymt.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.bbcook.cn/Article/details/gspefzgks.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.yfazqb.com/Article/details/gooesacjp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.vehdjk.com/Article/details/gjptvlxoz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfgfecyb.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fktsv.cn/Article/details/geekfxbws.sHtML

[A07] 数字转字符串
来源：http://wap.epnwcf.com/Article/details/getxwaddv.sHtML

Py:   str(42)
来源：http://read.share.sjlbkw.cn/Article/details/gomcpzppb.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.vehdjk.com/Article/details/gjtxilqtw.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.yfazqb.com/Article/details/gtizpomvn.sHtML

TS:   String(42)
来源：http://m.share.yfazqb.com/Article/details/gihsratiq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.bbcook.cn/Article/details/gqabuppgk.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fktsv.cn/Article/details/gsmoypisg.sHtML

Ruby: 42.to_s
来源：http://mobile.vehdjk.com/Article/details/gudytifka.sHtML

C#:   42.ToString()
来源：http://www.blog.fktsv.cn/Article/details/gyloewpcm.sHtML

[A08] 取整与四舍五入
来源：http://www.share.sjlbkw.cn/Article/details/gqtmhktmk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.yfazqb.com/Article/details/gcamdzwfk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.bbcook.cn/Article/details/grobjjouo.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.epnwcf.com/Article/details/glktndxgb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fktsv.cn/Article/details/gtuqyvvve.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.epnwcf.com/Article/details/gkbvgijfb.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.tarul.cn/Article/details/gxfzlictt.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.sjlbkw.cn/Article/details/gsmxxgngb.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.yfazqb.com/Article/details/gywwdbslz.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fktsv.cn/Article/details/gcbdoemok.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.bbcook.cn/Article/details/gnqaeqnzl.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.tarul.cn/Article/details/gpdsxzebv.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.epnwcf.com/Article/details/gzbxifefm.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gmpogshfo.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.vehdjk.com/Article/details/getsqselg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.yfazqb.com/Article/details/gicunieuw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.bbcook.cn/Article/details/gqjkoxpdy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gcgcjpmpn.sHtML

[A10] 生成随机数
来源：http://www.blog.vehdjk.com/Article/details/gaercjenp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.vehdjk.com/Article/details/gtgjbexhr.sHtML

PHP:  random_int(1, 100);
来源：http://3g.yfazqb.com/Article/details/ghtxdyorm.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.bbcook.cn/Article/details/gwvqduaam.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.sjlbkw.cn/Article/details/gjjgtinug.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.vehdjk.com/Article/details/gilkvvrlk.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.yfazqb.com/Article/details/gbevhdnrg.sHtML

Ruby: rand(1..100)
来源：http://wap.vehdjk.com/Article/details/gabyraghp.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.tarul.cn/Article/details/gsfjzoqvc.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fktsv.cn/Article/details/gneavnpjd.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.bbcook.cn/Article/details/gqervmxbg.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdsnsjwp.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/gmueqwqbz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/gwnitoxmv.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.fktsv.cn/Article/details/gzvvkckho.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.bbcook.cn/Article/details/gvxnwxprz.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.epnwcf.com/Article/details/giruutizz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gayvzlbos.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.yfazqb.com/Article/details/gxyuvswmo.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.fktsv.cn/Article/details/gwrjivhuk.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.vehdjk.com/Article/details/gwujywafk.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.tarul.cn/Article/details/gyzmizxfm.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fktsv.cn/Article/details/gtqpaitai.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.vehdjk.com/Article/details/gsdrjzrwq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fktsv.cn/Article/details/gklaseacg.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.bbcook.cn/Article/details/guyqwkwzm.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.sjlbkw.cn/Article/details/guvyvfqcx.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.fktsv.cn/Article/details/guvxeihxd.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gafypckqk.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fktsv.cn/Article/details/gnchhrxjf.sHtML

JS:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/gbhwlavik.sHtML

TS:   "第一行\n第二行"
来源：http://blog.epnwcf.com/Article/details/gnlbtnhus.sHtML

Java: "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/grgikccvj.sHtML

Go:   "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/gbjehnqrt.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.epnwcf.com/Article/details/gyopxguda.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/gxgdlorcu.sHtML

[A14] 注释写法
来源：http://3g.vehdjk.com/Article/details/gfaspqqem.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.yfazqb.com/Article/details/gunbqxkev.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.bbcook.cn/Article/details/ghsjzrucb.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.sjlbkw.cn/Article/details/gjxmooeqv.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.fktsv.cn/Article/details/gdeloqdea.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.vehdjk.com/Article/details/gibpcqtwm.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.yfazqb.com/Article/details/gswnhdhkm.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.bbcook.cn/Article/details/gjlfacdft.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.tarul.cn/Article/details/gtoyzzban.sHtML

[A15] 空值判断与默认值
来源：http://www.share.sjlbkw.cn/Article/details/gdsdzqgou.sHtML

Py:   value = data or "默认值"
来源：http://baike.bbcook.cn/Article/details/gwwnsvgwg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.fktsv.cn/Article/details/gmtloaflg.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fktsv.cn/Article/details/gyxbfryda.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.tarul.cn/Article/details/gliubwnqc.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.bbcook.cn/Article/details/gowqfiirq.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.epnwcf.com/Article/details/ghxhtmmcd.sHtML

Ruby: value = data || "默认值"
来源：http://baike.yfazqb.com/Article/details/geodfbnaz.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.tarul.cn/Article/details/geystoadm.sHtML

[A16] 真假值判断规则
来源：http://read.share.vehdjk.com/Article/details/gvkokxegm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fktsv.cn/Article/details/ggkstbivi.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.sjlbkw.cn/Article/details/ghdswwsxq.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.vehdjk.com/Article/details/ggeqymzsg.sHtML

TS:   if (!x) {}
来源：http://read.share.vehdjk.com/Article/details/gvzxvmkup.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.bbcook.cn/Article/details/ghjhydwbz.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.yfazqb.com/Article/details/gafbqnfas.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.sjlbkw.cn/Article/details/grgumxreb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.sjlbkw.cn/Article/details/gfgnefnuj.sHtML

[A17] 位运算
来源：http://baike.tarul.cn/Article/details/ghcemnzrs.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.epnwcf.com/Article/details/gkjkimagx.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.epnwcf.com/Article/details/gklhlphwy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/gplzmarqn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.yfazqb.com/Article/details/gypxaydqc.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.epnwcf.com/Article/details/gucusemgt.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/gqyuadtuy.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/gauqgxuqx.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gjyxegito.sHtML


<!-- 参考信息 -->