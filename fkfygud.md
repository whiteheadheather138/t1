代发 wailian999

[U101] JS：classList 操作
来源：http://mobile.yfazqb.com/Article/details/grjcvqmoy.sHtML

el.classList.toggle("active")
来源：http://read.share.yfazqb.com/Article/details/gmjtpyfrn.sHtML

[U102] JS：本地存储
来源：http://www.m.share.yfazqb.com/Article/details/gndevzfdr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fktsv.cn/Article/details/gbzfvqrnc.sHtML

[U103] JS：定时器
来源：http://www.m.share.bbcook.cn/Article/details/giqypgiyv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.vehdjk.com/Article/details/gfozxbxvy.sHtML

[U104] JS：防抖
来源：http://www.share.vehdjk.com/Article/details/gilpigojr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/gyjxaqxsg.sHtML

[U105] JS：节流
来源：http://wap.yfazqb.com/Article/details/griszmofj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.yfazqb.com/Article/details/gvswejlzf.sHtML

[U106] JS：日期格式化
来源：http://www.share.epnwcf.com/Article/details/gvfxbinep.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.bbcook.cn/Article/details/gtcltlory.sHtML

[U107] JS：数字千分位
来源：http://www.share.tarul.cn/Article/details/gaupmrway.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.epnwcf.com/Article/details/gdfpcmxlh.sHtML

[U108] JS：随机整数
来源：http://read.share.sjlbkw.cn/Article/details/ghipmmbii.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.vehdjk.com/Article/details/gikaxwemq.sHtML

[U109] JS：数组分组
来源：http://www.m.share.bbcook.cn/Article/details/gysjtfoar.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.yfazqb.com/Article/details/gldthjvri.sHtML

[U110] JS：数组分块
来源：http://read.share.fktsv.cn/Article/details/gaiffbsha.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.sjlbkw.cn/Article/details/glpbasjff.sHtML

[U111] JS：对象转 Map
来源：http://www.share.sjlbkw.cn/Article/details/gkisvqwvc.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.epnwcf.com/Article/details/gzizdacpd.sHtML

[U112] JS：字符串补位
来源：http://blog.fktsv.cn/Article/details/gvqxtlgfs.sHtML

"7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gjvynlihs.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fktsv.cn/Article/details/geysrojno.sHtML

s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gkvtmgclc.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.epnwcf.com/Article/details/gmqcqhdhf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.yfazqb.com/Article/details/gqkeutlbj.sHtML

[U115] JS：生成 UUID
来源：http://read.share.sjlbkw.cn/Article/details/gkrkviypr.sHtML

crypto.randomUUID()
来源：http://www.m.share.vehdjk.com/Article/details/ggroontgo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.sjlbkw.cn/Article/details/gpqurzmyf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.yfazqb.com/Article/details/gtghpiyvl.sHtML

[U117] JS：单元测试
来源：http://www.share.bbcook.cn/Article/details/gjwulvbxs.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fktsv.cn/Article/details/gjcgocwgk.sHtML

[U118] JS：开发服务器
来源：http://www.share.bbcook.cn/Article/details/gyzzxfewm.sHtML

npm i -D vite;  npx vite
来源：http://www.share.tarul.cn/Article/details/gllmyvgqc.sHtML

[U119] JS：生产构建
来源：http://3g.tarul.cn/Article/details/gspdxjarj.sHtML

npx vite build
来源：http://blog.epnwcf.com/Article/details/gzxjrcsgd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.epnwcf.com/Article/details/gngdmttye.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.sjlbkw.cn/Article/details/grtnqtvrh.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gtuqkjqke.sHtML

统计汇总
来源：http://baike.bbcook.cn/Article/details/gmxmmvbsm.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/goicpvjxb.sHtML

按语言统计（条）：
来源：http://www.m.share.bbcook.cn/Article/details/gszcejuqj.sHtML

Python ......... 252
来源：http://m.share.bbcook.cn/Article/details/gyyenckpg.sHtML

PHP ............ 252
来源：http://www.blog.bbcook.cn/Article/details/ggcvkwabj.sHtML

JavaScript ..... 252
来源：http://wap.sjlbkw.cn/Article/details/glvrysgqx.sHtML

TypeScript ..... 212
来源：http://m.share.tarul.cn/Article/details/ggkzgiwje.sHtML

Java ........... 212
来源：http://wap.vehdjk.com/Article/details/gzhzkmmxr.sHtML

Go ............. 212
来源：http://3g.sjlbkw.cn/Article/details/gyjjcfzpi.sHtML

Ruby ........... 212
来源：http://mobile.sjlbkw.cn/Article/details/gchvbihqc.sHtML

C# ............. 212
来源：http://read.share.tarul.cn/Article/details/gtcceewmh.sHtML

C .............. 30
来源：http://mobile.tarul.cn/Article/details/gbmfcrglw.sHtML

C++ ............ 30
来源：http://read.share.bbcook.cn/Article/details/glrebnefe.sHtML

SQL ............ 90
来源：http://baike.vehdjk.com/Article/details/gnooupbik.sHtML

Bash ........... 80
来源：http://www.blog.vehdjk.com/Article/details/giqvthvjk.sHtML

Kotlin ......... 15
来源：http://m.share.vehdjk.com/Article/details/gfhxblyuc.sHtML

Swift .......... 15
来源：http://m.share.sjlbkw.cn/Article/details/gbrzujrxm.sHtML

Lua ............ 10
来源：http://3g.vehdjk.com/Article/details/gvzslcqry.sHtML

Perl ........... 10
来源：http://m.share.tarul.cn/Article/details/gyrzowgdp.sHtML

Scala .......... 10
来源：http://wap.bbcook.cn/Article/details/gflvqcwcu.sHtML

------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gqwnljjxr.sHtML

合计 ........... 2106 条
来源：http://m.share.fktsv.cn/Article/details/gqjxdveep.sHtML

按章节统计：
来源：http://blog.fktsv.cn/Article/details/ggjgobshs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.epnwcf.com/Article/details/guvjrknzc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fktsv.cn/Article/details/gvqqyduox.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.epnwcf.com/Article/details/gerpqvnig.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.sjlbkw.cn/Article/details/gechinwun.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.vehdjk.com/Article/details/gzqsvldeu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fktsv.cn/Article/details/gvscdmtro.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.yfazqb.com/Article/details/gmjpgajpd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.bbcook.cn/Article/details/giyapzpgh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/gvckuuric.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.epnwcf.com/Article/details/gwdkjvzhr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/gjvydkkbb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gazogapgb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gbtbffqcv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.bbcook.cn/Article/details/gatwwxkmq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.epnwcf.com/Article/details/giygkeyum.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/gmucmcarb.sHtML

Q SQL 专题                              90
来源：http://3g.yfazqb.com/Article/details/gnyofuqbh.sHtML

R Bash 专题                             80
来源：http://blog.epnwcf.com/Article/details/gvchjwwwn.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.sjlbkw.cn/Article/details/gcivxfdcp.sHtML

T 其他语言补充                          60
来源：http://3g.vehdjk.com/Article/details/gcohrvsdh.sHtML

U 高频实用片段                         120
来源：http://www.blog.bbcook.cn/Article/details/gunlgjwbo.sHtML

------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/galpcaclc.sHtML

合计                                  2106 条
来源：http://baike.epnwcf.com/Article/details/gqtbfvnue.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gkyjgpceu.sHtML

使用提醒
来源：http://blog.fktsv.cn/Article/details/gigybiram.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fktsv.cn/Article/details/gnngpjwpr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.bbcook.cn/Article/details/glzqvqunk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fktsv.cn/Article/details/ggolpajxc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.sjlbkw.cn/Article/details/gmpakaekq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.tarul.cn/Article/details/gkonbmcqy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.vehdjk.com/Article/details/gjsnskxgv.sHtML

—— 文件结束 ——
来源：http://wap.fktsv.cn/Article/details/grcrmftwx.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gzccxwrud.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.vehdjk.com/Article/details/gppseilzj.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.vehdjk.com/Article/details/geibpjdoo.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gmwfwrouz.sHtML

【收录内容】
来源：http://www.m.share.vehdjk.com/Article/details/glpdkkvpz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.sjlbkw.cn/Article/details/grwxryujl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.bbcook.cn/Article/details/gmpuagkzh.sHtML

SQL · Bash · C · C++
来源：http://www.share.fktsv.cn/Article/details/gnaqpjdyp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.vehdjk.com/Article/details/gkjcvddbh.sHtML

【使用说明】
来源：http://www.m.share.epnwcf.com/Article/details/griulupkw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.sjlbkw.cn/Article/details/gfljfhiwq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.bbcook.cn/Article/details/gibkjltfw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.vehdjk.com/Article/details/gvshrjpvb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.bbcook.cn/Article/details/gdkelmlgl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.bbcook.cn/Article/details/gexoxgklx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.bbcook.cn/Article/details/gzbzwynan.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.tarul.cn/Article/details/gnyloiwes.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.vehdjk.com/Article/details/gclyszzjj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.bbcook.cn/Article/details/ghibqgqzd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.tarul.cn/Article/details/ghygxdotk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.tarul.cn/Article/details/gclzwnvni.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.vehdjk.com/Article/details/gfawxdolv.sHtML

【文件统计】
来源：http://www.share.epnwcf.com/Article/details/ghqdjhzja.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.sjlbkw.cn/Article/details/grirwzqwm.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/gjwtxvfjy.sHtML

目  录
来源：http://blog.tarul.cn/Article/details/gyseizuqz.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gjfsjmbhw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.sjlbkw.cn/Article/details/gvaneuvpr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.epnwcf.com/Article/details/goycuajbz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.epnwcf.com/Article/details/gvwzgvfmn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.bbcook.cn/Article/details/gbnpnefjv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.vehdjk.com/Article/details/gsidkmbns.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.sjlbkw.cn/Article/details/gexisjonw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.bbcook.cn/Article/details/gmhoycidm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.vehdjk.com/Article/details/grssasqjs.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/gmmhrsvdn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fktsv.cn/Article/details/gqslasthf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.tarul.cn/Article/details/grbesovte.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/gdrvvldkh.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gduatlzyl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdzfezpr.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.vehdjk.com/Article/details/gvzyvhkwl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.vehdjk.com/Article/details/gwlvivzxh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.epnwcf.com/Article/details/gibsimqho.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.sjlbkw.cn/Article/details/gdligtlgw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.vehdjk.com/Article/details/ggjjgltby.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.epnwcf.com/Article/details/gfitvdtyq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.vehdjk.com/Article/details/gvunhlcql.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gcoqhfegm.sHtML

A. 基础语法与类型
来源：http://wap.sjlbkw.cn/Article/details/gtzgqoitq.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ghwdermgy.sHtML

[A01] Hello World
来源：http://www.blog.tarul.cn/Article/details/ghzngkrth.sHtML

Py:   print("Hello, World!")
来源：http://m.share.yfazqb.com/Article/details/gpytkxkbm.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.vehdjk.com/Article/details/gzeqptcmn.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.sjlbkw.cn/Article/details/gsixoulbi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.tarul.cn/Article/details/gdhutuicx.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.vehdjk.com/Article/details/gtodafnib.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.sjlbkw.cn/Article/details/grecsvtto.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fktsv.cn/Article/details/ganrvtfxi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.sjlbkw.cn/Article/details/gayorlzzu.sHtML

[A02] 变量声明与赋值
来源：http://mobile.bbcook.cn/Article/details/gotbajxrj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.tarul.cn/Article/details/gebodkoxe.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.bbcook.cn/Article/details/gwldxlrdc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.tarul.cn/Article/details/gscedhyqg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.tarul.cn/Article/details/gakrpwxny.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.vehdjk.com/Article/details/gwyqkvbre.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.bbcook.cn/Article/details/gulgzufcj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.epnwcf.com/Article/details/gnstqoudg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.epnwcf.com/Article/details/gbswpgerq.sHtML

[A03] 常量定义
来源：http://baike.fktsv.cn/Article/details/gswfemjxh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrjudvpr.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gscqnrcgo.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gnygpcklj.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gdpuxkjrt.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gijfcihws.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.bbcook.cn/Article/details/gqtfsuape.sHtML

Ruby: PI = 3.14159
来源：http://baike.vehdjk.com/Article/details/gcnbegdpq.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gnfmrbhij.sHtML

[A04] 判断变量类型
来源：http://www.m.share.bbcook.cn/Article/details/ghdnmttcx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.sjlbkw.cn/Article/details/gqgxkvaae.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.tarul.cn/Article/details/grwjdgrkm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fktsv.cn/Article/details/gmsnhkuod.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.bbcook.cn/Article/details/gakpwgcpu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.sjlbkw.cn/Article/details/gtadwuitn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.vehdjk.com/Article/details/gditrauei.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.yfazqb.com/Article/details/gpisekxvf.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fktsv.cn/Article/details/gpxyhaanx.sHtML

[A05] 整数除法与取模
来源：http://mobile.yfazqb.com/Article/details/gwtqdrugt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.yfazqb.com/Article/details/gxmllaslm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gptrdtkhl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fktsv.cn/Article/details/ggacbklai.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.yfazqb.com/Article/details/gufzviexz.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fktsv.cn/Article/details/gerpshleq.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.yfazqb.com/Article/details/gyzuniyie.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/ghindfpha.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.vehdjk.com/Article/details/gbkbdnpne.sHtML

[A06] 字符串转数字
来源：http://www.blog.tarul.cn/Article/details/gumuilplc.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.vehdjk.com/Article/details/gpypopcyb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.tarul.cn/Article/details/gsoqaizap.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.tarul.cn/Article/details/gwwvazafs.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.tarul.cn/Article/details/gjobmuasg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.epnwcf.com/Article/details/gpondbnrn.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fktsv.cn/Article/details/gzckjytxi.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.vehdjk.com/Article/details/gruamysol.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.sjlbkw.cn/Article/details/gkzgseorj.sHtML

[A07] 数字转字符串
来源：http://www.blog.epnwcf.com/Article/details/geqyglknh.sHtML

Py:   str(42)
来源：http://3g.yfazqb.com/Article/details/gxrwkbvzr.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.epnwcf.com/Article/details/gocbosqgc.sHtML

JS:   String(42); (42).toString()
来源：http://blog.yfazqb.com/Article/details/gggtwtdem.sHtML

TS:   String(42)
来源：http://m.share.tarul.cn/Article/details/gxiakovzb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.epnwcf.com/Article/details/guosbdbjw.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.fktsv.cn/Article/details/ggqamjulq.sHtML

Ruby: 42.to_s
来源：http://read.share.tarul.cn/Article/details/gpvuelwoe.sHtML

C#:   42.ToString()
来源：http://wap.fktsv.cn/Article/details/gfmggaffv.sHtML

[A08] 取整与四舍五入
来源：http://blog.fktsv.cn/Article/details/gnftcaioz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.epnwcf.com/Article/details/gkzyjfhjx.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.tarul.cn/Article/details/gakgnwdvc.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.vehdjk.com/Article/details/gmvzwjxkr.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.sjlbkw.cn/Article/details/giphxgkue.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.tarul.cn/Article/details/grhdgjgmr.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.vehdjk.com/Article/details/gcemptmup.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.bbcook.cn/Article/details/gampggxyg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fktsv.cn/Article/details/goiqqkygt.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.vehdjk.com/Article/details/ggqnsmjis.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fktsv.cn/Article/details/gnonmpnjc.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.tarul.cn/Article/details/gvtsisyxl.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.yfazqb.com/Article/details/gfrkrcaho.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gzllqrzoq.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.yfazqb.com/Article/details/ggqocwazb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.tarul.cn/Article/details/gdsadbntd.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.vehdjk.com/Article/details/gwejspeir.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gejrhrghp.sHtML

[A10] 生成随机数
来源：http://www.blog.fktsv.cn/Article/details/gajdcqnmr.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.yfazqb.com/Article/details/golhkvmsz.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.tarul.cn/Article/details/gfqmfwspp.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.vehdjk.com/Article/details/gurzisofi.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.bbcook.cn/Article/details/grkxulftp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.bbcook.cn/Article/details/gwgsipvzv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqybvguk.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.vehdjk.com/Article/details/gicpnhhdb.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.tarul.cn/Article/details/gyolxsbpz.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.bbcook.cn/Article/details/gaksiqafc.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.tarul.cn/Article/details/gxjbgmysw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.epnwcf.com/Article/details/grnbxwkbd.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.bbcook.cn/Article/details/gfppdefbd.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.yfazqb.com/Article/details/gbkrwyhif.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.tarul.cn/Article/details/geoalcnfr.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.epnwcf.com/Article/details/gjfzzbfma.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.vehdjk.com/Article/details/gocohmwsh.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.yfazqb.com/Article/details/gnarurxgd.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fktsv.cn/Article/details/gilqlvqyx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.fktsv.cn/Article/details/getxuwmwf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gftimaddq.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fktsv.cn/Article/details/gptuuuaan.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.vehdjk.com/Article/details/grhkjuevb.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.tarul.cn/Article/details/gfylapuxi.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.yfazqb.com/Article/details/gyfhkfugy.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.vehdjk.com/Article/details/ggwjdvxdm.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.epnwcf.com/Article/details/gzdeiklhd.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.epnwcf.com/Article/details/gsievgagb.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/ggifrypvz.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.tarul.cn/Article/details/gwnftpuqx.sHtML

JS:   "第一行\n第二行"
来源：http://baike.tarul.cn/Article/details/gtkirscuq.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/graiewqor.sHtML

Java: "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/gewvnsmbo.sHtML

Go:   "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gtdzxgufp.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gqahxpqur.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fktsv.cn/Article/details/gdwpeucbv.sHtML

[A14] 注释写法
来源：http://3g.epnwcf.com/Article/details/gdyozafmz.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.yfazqb.com/Article/details/gmkczbtkz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.epnwcf.com/Article/details/gwhikaqtx.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.tarul.cn/Article/details/gkyqdetav.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.yfazqb.com/Article/details/gcxgzrcoa.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.tarul.cn/Article/details/graoifags.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.sjlbkw.cn/Article/details/gjnomitxf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.epnwcf.com/Article/details/gtzbdcfmh.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.tarul.cn/Article/details/gfarcehee.sHtML

[A15] 空值判断与默认值
来源：http://baike.fktsv.cn/Article/details/gidlblgov.sHtML

Py:   value = data or "默认值"
来源：http://www.share.fktsv.cn/Article/details/ggirhubgy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.yfazqb.com/Article/details/gerdzmcel.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.yfazqb.com/Article/details/glhprfhtw.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.tarul.cn/Article/details/gzgxshjcx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.yfazqb.com/Article/details/gktznsmte.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.sjlbkw.cn/Article/details/gqgskkkpf.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.tarul.cn/Article/details/geuuqahzc.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.tarul.cn/Article/details/gxeqdksvz.sHtML

[A16] 真假值判断规则
来源：http://www.share.bbcook.cn/Article/details/gbrbudvbj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fktsv.cn/Article/details/gpjoevfzc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.epnwcf.com/Article/details/gdtkcicbk.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.epnwcf.com/Article/details/guhegitnp.sHtML

TS:   if (!x) {}
来源：http://www.share.vehdjk.com/Article/details/gobaunyla.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.epnwcf.com/Article/details/geuwktvvz.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.epnwcf.com/Article/details/gjozucrqe.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.vehdjk.com/Article/details/gemgrwfuv.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.vehdjk.com/Article/details/gogdoxuko.sHtML

[A17] 位运算
来源：http://www.m.share.epnwcf.com/Article/details/gavwpgunv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/gmrhfokaq.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.yfazqb.com/Article/details/gahhuraox.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gxmkqdiqp.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gwtncawhl.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/ggcwcnkzr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.vehdjk.com/Article/details/grfdupprc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.tarul.cn/Article/details/gsqrzmfzn.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/gtgrbsuwb.sHtML


<!-- 参考信息 -->