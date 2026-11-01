代发 wailian999

[U101] JS：classList 操作
来源：http://3g.fktsv.cn/Article/details/gfftwpjcb.sHtML

el.classList.toggle("active")
来源：http://blog.tarul.cn/Article/details/gtvagawfv.sHtML

[U102] JS：本地存储
来源：http://wap.epnwcf.com/Article/details/ggisdavkd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.vehdjk.com/Article/details/gzupynylk.sHtML

[U103] JS：定时器
来源：http://baike.epnwcf.com/Article/details/gbnazcytu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.yfazqb.com/Article/details/gmosyqfyd.sHtML

[U104] JS：防抖
来源：http://m.share.vehdjk.com/Article/details/gddkxgqfo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/ghygcjdax.sHtML

[U105] JS：节流
来源：http://read.share.bbcook.cn/Article/details/gfngfpcqp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.sjlbkw.cn/Article/details/ghnejrmsg.sHtML

[U106] JS：日期格式化
来源：http://blog.fktsv.cn/Article/details/gjtnmmkhg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.bbcook.cn/Article/details/gadzrlvck.sHtML

[U107] JS：数字千分位
来源：http://blog.tarul.cn/Article/details/gymerxjhn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fktsv.cn/Article/details/gsyqxnzxr.sHtML

[U108] JS：随机整数
来源：http://www.share.fktsv.cn/Article/details/geflibvgc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.epnwcf.com/Article/details/gcnzhepca.sHtML

[U109] JS：数组分组
来源：http://www.share.bbcook.cn/Article/details/gwyatscur.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.yfazqb.com/Article/details/gddplfupe.sHtML

[U110] JS：数组分块
来源：http://www.share.vehdjk.com/Article/details/gdjspnlzu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.yfazqb.com/Article/details/gbvepqqjf.sHtML

[U111] JS：对象转 Map
来源：http://m.share.yfazqb.com/Article/details/gyrikqixn.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.tarul.cn/Article/details/gofmavpvh.sHtML

[U112] JS：字符串补位
来源：http://wap.yfazqb.com/Article/details/gnendsmfv.sHtML

"7".padStart(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/gaaexacrz.sHtML

[U113] JS：正则替换全部
来源：http://3g.bbcook.cn/Article/details/gaispaqus.sHtML

s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gdumamoyb.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fktsv.cn/Article/details/gxilubzir.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fktsv.cn/Article/details/goxuxxzwe.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fktsv.cn/Article/details/gpxwkfwwx.sHtML

crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/gktdluaky.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.sjlbkw.cn/Article/details/grxwgwlmw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.yfazqb.com/Article/details/glyduyhox.sHtML

[U117] JS：单元测试
来源：http://read.share.epnwcf.com/Article/details/gfsarkfso.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.sjlbkw.cn/Article/details/glgkfzrdf.sHtML

[U118] JS：开发服务器
来源：http://mobile.vehdjk.com/Article/details/gnfdzggrc.sHtML

npm i -D vite;  npx vite
来源：http://mobile.vehdjk.com/Article/details/gtsyurglu.sHtML

[U119] JS：生产构建
来源：http://www.blog.epnwcf.com/Article/details/gpchhjxxw.sHtML

npx vite build
来源：http://www.blog.tarul.cn/Article/details/gjdtrxuub.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.yfazqb.com/Article/details/gqvorzjso.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.yfazqb.com/Article/details/gvydbsuhw.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gxgwppdpb.sHtML

统计汇总
来源：http://www.m.share.tarul.cn/Article/details/gcnmeapth.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gixzpplko.sHtML

按语言统计（条）：
来源：http://www.m.share.epnwcf.com/Article/details/gzblsmeuj.sHtML

Python ......... 252
来源：http://blog.tarul.cn/Article/details/gnzktobnb.sHtML

PHP ............ 252
来源：http://mobile.sjlbkw.cn/Article/details/gisjzjrrl.sHtML

JavaScript ..... 252
来源：http://www.m.share.fktsv.cn/Article/details/gdafqkwqp.sHtML

TypeScript ..... 212
来源：http://www.m.share.epnwcf.com/Article/details/gccvhvfen.sHtML

Java ........... 212
来源：http://wap.fktsv.cn/Article/details/gwbbobsdv.sHtML

Go ............. 212
来源：http://wap.tarul.cn/Article/details/gpamxokfm.sHtML

Ruby ........... 212
来源：http://www.share.fktsv.cn/Article/details/ggoyyzpzj.sHtML

C# ............. 212
来源：http://3g.tarul.cn/Article/details/gllgjuvba.sHtML

C .............. 30
来源：http://mobile.fktsv.cn/Article/details/gcvbytymt.sHtML

C++ ............ 30
来源：http://blog.bbcook.cn/Article/details/gqsbokfji.sHtML

SQL ............ 90
来源：http://3g.yfazqb.com/Article/details/gthdeopyc.sHtML

Bash ........... 80
来源：http://www.blog.tarul.cn/Article/details/gsjpzmevx.sHtML

Kotlin ......... 15
来源：http://baike.sjlbkw.cn/Article/details/gexfghrhl.sHtML

Swift .......... 15
来源：http://baike.yfazqb.com/Article/details/gganbjgmw.sHtML

Lua ............ 10
来源：http://read.share.vehdjk.com/Article/details/gkthymyhu.sHtML

Perl ........... 10
来源：http://m.share.sjlbkw.cn/Article/details/gxvpyzveq.sHtML

Scala .......... 10
来源：http://www.m.share.yfazqb.com/Article/details/grrfnytbu.sHtML

------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gpvivghtq.sHtML

合计 ........... 2106 条
来源：http://www.share.vehdjk.com/Article/details/gaekmksly.sHtML

按章节统计：
来源：http://read.share.yfazqb.com/Article/details/gyczbofek.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.bbcook.cn/Article/details/gmitvnhbo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fktsv.cn/Article/details/goekxcnev.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.yfazqb.com/Article/details/ggnidowru.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.bbcook.cn/Article/details/gwquwsose.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.epnwcf.com/Article/details/glibsopwk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.sjlbkw.cn/Article/details/gffzqxmpm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.bbcook.cn/Article/details/gkhbpesqd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.tarul.cn/Article/details/gvocsqrhx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gcdtjzwgn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.sjlbkw.cn/Article/details/gptyqapzi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gvtcorjrq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/guxobjpug.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/gpenaojfy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.bbcook.cn/Article/details/gfqvtjxtx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.yfazqb.com/Article/details/gdsitbjud.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/golqeafbm.sHtML

Q SQL 专题                              90
来源：http://baike.sjlbkw.cn/Article/details/gueejyayv.sHtML

R Bash 专题                             80
来源：http://blog.yfazqb.com/Article/details/gxbrbgpyy.sHtML

S C / C++ 专题                          60
来源：http://baike.sjlbkw.cn/Article/details/gidfxgygc.sHtML

T 其他语言补充                          60
来源：http://3g.yfazqb.com/Article/details/gwssojatv.sHtML

U 高频实用片段                         120
来源：http://www.share.epnwcf.com/Article/details/grugqsmqr.sHtML

------------------------------------
来源：http://blog.vehdjk.com/Article/details/gvdjqpqdi.sHtML

合计                                  2106 条
来源：http://baike.vehdjk.com/Article/details/gtmjfqesi.sHtML

--------------------------------------------------------------------------------
来源：http://3g.epnwcf.com/Article/details/gkpevghlv.sHtML

使用提醒
来源：http://blog.fktsv.cn/Article/details/gshahnnst.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gwreltain.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.yfazqb.com/Article/details/gncldyfdq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.vehdjk.com/Article/details/gbvturhpe.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.bbcook.cn/Article/details/gcxigdyei.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.bbcook.cn/Article/details/gxyzwdhpu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.epnwcf.com/Article/details/giipuxsag.sHtML

—— 文件结束 ——
来源：http://baike.tarul.cn/Article/details/gblvszfmw.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gemcfqqkr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fktsv.cn/Article/details/glkxkguxn.sHtML

Common Programming Examples Cheat Book
来源：http://wap.vehdjk.com/Article/details/gcrvhfpfi.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gnvsxwtsg.sHtML

【收录内容】
来源：http://wap.fktsv.cn/Article/details/gbjiqywrn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.sjlbkw.cn/Article/details/gpfthjlzr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.sjlbkw.cn/Article/details/gcuuimjio.sHtML

SQL · Bash · C · C++
来源：http://3g.fktsv.cn/Article/details/gtbwyvskl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.tarul.cn/Article/details/gvaahyloo.sHtML

【使用说明】
来源：http://blog.bbcook.cn/Article/details/gqvxmsabi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.yfazqb.com/Article/details/gxcenpkac.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.epnwcf.com/Article/details/grgjjbdpb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.epnwcf.com/Article/details/giccspevw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.vehdjk.com/Article/details/gtjiyylrn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.bbcook.cn/Article/details/gpiiitpnd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.bbcook.cn/Article/details/gsligughp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fktsv.cn/Article/details/gjhvbzgnb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.vehdjk.com/Article/details/gbdkqzzaw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.bbcook.cn/Article/details/gpouucukb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.vehdjk.com/Article/details/gxzidseel.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.vehdjk.com/Article/details/gjrbugrwc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.epnwcf.com/Article/details/guknmusrj.sHtML

【文件统计】
来源：http://m.share.yfazqb.com/Article/details/ggxpunsqw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.epnwcf.com/Article/details/gpetgthyr.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gevauzwks.sHtML

目  录
来源：http://baike.fktsv.cn/Article/details/gwicnxkcr.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.epnwcf.com/Article/details/gbkacbxvz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.yfazqb.com/Article/details/gruvyvffg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.yfazqb.com/Article/details/gyigqxubk.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.tarul.cn/Article/details/gpxvzyjpi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.epnwcf.com/Article/details/gsmlrnugb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.bbcook.cn/Article/details/gkybcxnuy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.bbcook.cn/Article/details/gveofgyzi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.bbcook.cn/Article/details/gytrnspjk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.tarul.cn/Article/details/gvzlckxue.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.epnwcf.com/Article/details/gjlvsdoqv.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.sjlbkw.cn/Article/details/gdopmwijz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbiqwlsg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/geumjgjqh.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/gmuvefafz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.vehdjk.com/Article/details/ghfflmpxh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.vehdjk.com/Article/details/gecfaqgve.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.yfazqb.com/Article/details/gxxgugmct.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.yfazqb.com/Article/details/gkvmpqnpz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.bbcook.cn/Article/details/gdzkaulso.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.bbcook.cn/Article/details/gukoneysk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gpkmtcqcv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.sjlbkw.cn/Article/details/gzioqygwz.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gosjbumpx.sHtML

A. 基础语法与类型
来源：http://www.blog.bbcook.cn/Article/details/gakkrebmy.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gszggnzkc.sHtML

[A01] Hello World
来源：http://www.blog.vehdjk.com/Article/details/ggadvprqd.sHtML

Py:   print("Hello, World!")
来源：http://baike.bbcook.cn/Article/details/gobpnepwq.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.vehdjk.com/Article/details/gowvpxmtc.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.sjlbkw.cn/Article/details/gsprrhlbq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fktsv.cn/Article/details/gjgxfetss.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.epnwcf.com/Article/details/gwuguaxwd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.tarul.cn/Article/details/gtwafwdnt.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.epnwcf.com/Article/details/ghwmhqjfn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.bbcook.cn/Article/details/gxhwzdzji.sHtML

[A02] 变量声明与赋值
来源：http://baike.bbcook.cn/Article/details/gphjywvnq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.yfazqb.com/Article/details/gdzscdezh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.bbcook.cn/Article/details/ghisbmkww.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fktsv.cn/Article/details/gzjmqegrw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.sjlbkw.cn/Article/details/gnnnfzahv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fktsv.cn/Article/details/gmbxxtomg.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.tarul.cn/Article/details/gnxigywrw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.bbcook.cn/Article/details/gdnqifuaq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fktsv.cn/Article/details/gyxblfhxk.sHtML

[A03] 常量定义
来源：http://3g.bbcook.cn/Article/details/gkytaebno.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.bbcook.cn/Article/details/gbzzhlyca.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gwjvgoxjx.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gihdkkqoh.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.yfazqb.com/Article/details/grjqrqjkw.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gvxrkchfh.sHtML

Go:   const PI = 3.14159
来源：http://blog.tarul.cn/Article/details/gdqvtghfx.sHtML

Ruby: PI = 3.14159
来源：http://mobile.vehdjk.com/Article/details/grmawmsof.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gpveqfjuf.sHtML

[A04] 判断变量类型
来源：http://baike.sjlbkw.cn/Article/details/gucllrxbs.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.bbcook.cn/Article/details/gzrgpgdwb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.vehdjk.com/Article/details/gbetyptyg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.vehdjk.com/Article/details/ghormqdbn.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.sjlbkw.cn/Article/details/ggrgmtaej.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.yfazqb.com/Article/details/gnjwkhcim.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.yfazqb.com/Article/details/grnckcdds.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.vehdjk.com/Article/details/gpbtixlla.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.bbcook.cn/Article/details/gzqawrnil.sHtML

[A05] 整数除法与取模
来源：http://mobile.vehdjk.com/Article/details/ggwzrtnah.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.bbcook.cn/Article/details/gocmlvujk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.vehdjk.com/Article/details/gflgqhktb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.yfazqb.com/Article/details/gcluzxzkg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.vehdjk.com/Article/details/gjtcnovye.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.bbcook.cn/Article/details/gdutsxtgh.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/glhnbtcsy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.vehdjk.com/Article/details/gdxieeyta.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.epnwcf.com/Article/details/ggvwbmine.sHtML

[A06] 字符串转数字
来源：http://www.share.bbcook.cn/Article/details/grqbfwfvx.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.vehdjk.com/Article/details/gouiswxhv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.yfazqb.com/Article/details/ggcxnfinw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.sjlbkw.cn/Article/details/gtliwrkuv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.yfazqb.com/Article/details/gvllgkhwr.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.tarul.cn/Article/details/gzjwonqvf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.yfazqb.com/Article/details/gajkmqulb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.sjlbkw.cn/Article/details/gqnmzfdto.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.vehdjk.com/Article/details/gmbiqzoyc.sHtML

[A07] 数字转字符串
来源：http://m.share.vehdjk.com/Article/details/gyzgklvyz.sHtML

Py:   str(42)
来源：http://www.blog.fktsv.cn/Article/details/gougwmlcn.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.sjlbkw.cn/Article/details/gxnwcgcta.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.yfazqb.com/Article/details/gtyhwkbti.sHtML

TS:   String(42)
来源：http://mobile.fktsv.cn/Article/details/gmhljsuth.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.vehdjk.com/Article/details/gbypsynzs.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.bbcook.cn/Article/details/gdpbsnojj.sHtML

Ruby: 42.to_s
来源：http://read.share.vehdjk.com/Article/details/guezvfwsa.sHtML

C#:   42.ToString()
来源：http://www.blog.tarul.cn/Article/details/gfnggzmzl.sHtML

[A08] 取整与四舍五入
来源：http://read.share.epnwcf.com/Article/details/gryswpdfo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/gzpcfsjia.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fktsv.cn/Article/details/gqqmmvldc.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fktsv.cn/Article/details/gbbjehpav.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.epnwcf.com/Article/details/gklxdvwht.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.sjlbkw.cn/Article/details/gdlyfqmoc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.yfazqb.com/Article/details/gdornupzh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.yfazqb.com/Article/details/ggxaluizh.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/gnhgivdms.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.tarul.cn/Article/details/grjcytdbr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.sjlbkw.cn/Article/details/greepvoiq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gnddxoydj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gkhmyepxk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.tarul.cn/Article/details/gkwlorxhl.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.vehdjk.com/Article/details/ghtutscxe.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.yfazqb.com/Article/details/ggaextghe.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.epnwcf.com/Article/details/gezjmzgwm.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.tarul.cn/Article/details/gmzqoiufm.sHtML

[A10] 生成随机数
来源：http://m.share.yfazqb.com/Article/details/gyltxmyiu.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.epnwcf.com/Article/details/glsiswufy.sHtML

PHP:  random_int(1, 100);
来源：http://blog.tarul.cn/Article/details/gpqqfvohz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.vehdjk.com/Article/details/gsawmztyr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.tarul.cn/Article/details/gqtfaokid.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.tarul.cn/Article/details/gwanxmlpg.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.tarul.cn/Article/details/gdzojkupk.sHtML

Ruby: rand(1..100)
来源：http://read.share.yfazqb.com/Article/details/gqyhgwcwq.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.epnwcf.com/Article/details/gyeehhlus.sHtML

[A11] 条件表达式（三元）
来源：http://baike.tarul.cn/Article/details/gzvfxubyr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.sjlbkw.cn/Article/details/gipjtyjmj.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/gouaomgrp.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.epnwcf.com/Article/details/goffjxwca.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.vehdjk.com/Article/details/gldhkktqa.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.bbcook.cn/Article/details/gojkvdbci.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fktsv.cn/Article/details/gldrzfmpl.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.vehdjk.com/Article/details/gqlgelmbd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.bbcook.cn/Article/details/gvddgvnle.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.sjlbkw.cn/Article/details/gegozhzyt.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.bbcook.cn/Article/details/grfpeepre.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.tarul.cn/Article/details/gnmnlohek.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.tarul.cn/Article/details/guyxqaptd.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcphqkhg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.bbcook.cn/Article/details/gglcclneh.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fktsv.cn/Article/details/gyhmqtndt.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.tarul.cn/Article/details/gjizjwwyp.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.fktsv.cn/Article/details/gsvnonftj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.vehdjk.com/Article/details/gnhxoqekw.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gbqbbhxpg.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gkareshbh.sHtML

JS:   "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/goqoqbpek.sHtML

TS:   "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gssjysyij.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gkwrytoht.sHtML

Go:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gwktquyjs.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/gwscqwmwr.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.tarul.cn/Article/details/gwvndzxgj.sHtML

[A14] 注释写法
来源：http://m.share.fktsv.cn/Article/details/gyuwxmlzw.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.epnwcf.com/Article/details/gnkzhpiyq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/guwcbdlqg.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.bbcook.cn/Article/details/gethldlsc.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.yfazqb.com/Article/details/gdmzbevta.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.tarul.cn/Article/details/ghzofhhqo.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.sjlbkw.cn/Article/details/grfmibvoh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.vehdjk.com/Article/details/ggozkixhl.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/gfxemqycw.sHtML

[A15] 空值判断与默认值
来源：http://mobile.bbcook.cn/Article/details/gimvulsmi.sHtML

Py:   value = data or "默认值"
来源：http://3g.sjlbkw.cn/Article/details/gtqdtcpww.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.tarul.cn/Article/details/gcaatdgux.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fktsv.cn/Article/details/gwryrzksm.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.bbcook.cn/Article/details/gbbumsumg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.epnwcf.com/Article/details/gcvcyohbb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.epnwcf.com/Article/details/gsshgufzr.sHtML

Ruby: value = data || "默认值"
来源：http://baike.sjlbkw.cn/Article/details/gopdnneeq.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.tarul.cn/Article/details/gsckheqko.sHtML

[A16] 真假值判断规则
来源：http://wap.bbcook.cn/Article/details/gppfzdwwh.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.tarul.cn/Article/details/gxayhlgbh.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.sjlbkw.cn/Article/details/gdmdgzsxg.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.vehdjk.com/Article/details/genzushpp.sHtML

TS:   if (!x) {}
来源：http://read.share.tarul.cn/Article/details/gtrtluklt.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.tarul.cn/Article/details/gpfusyuux.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.vehdjk.com/Article/details/gcdehywdx.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.tarul.cn/Article/details/gchbwocuq.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.epnwcf.com/Article/details/gqbeinjni.sHtML

[A17] 位运算
来源：http://www.share.epnwcf.com/Article/details/gluubyzgx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gcmtyctkw.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.yfazqb.com/Article/details/gjkshhmzu.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/gxfwrozhn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/grfcglemy.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.vehdjk.com/Article/details/gvdojzlku.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.yfazqb.com/Article/details/gutsnspnx.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/gswvjrwkt.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/gaivbohpr.sHtML


<!-- 参考信息 -->