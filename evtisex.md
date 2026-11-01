代发 wailian999

[U99] JS：事件监听
来源：http://blog.sjlbkw.cn/Article/details/gaibtruai.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.vehdjk.com/Article/details/gszuxbrag.sHtML

[U100] JS：DOM 查询
来源：http://baike.bbcook.cn/Article/details/gstyoaqkm.sHtML

document.querySelector(".item")
来源：http://www.share.vehdjk.com/Article/details/gravlvlps.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.epnwcf.com/Article/details/gdjsqrlmk.sHtML

el.classList.toggle("active")
来源：http://blog.sjlbkw.cn/Article/details/gpgqzpvou.sHtML

[U102] JS：本地存储
来源：http://read.share.vehdjk.com/Article/details/gfvruvzve.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.vehdjk.com/Article/details/ghtinfqcj.sHtML

[U103] JS：定时器
来源：http://www.share.tarul.cn/Article/details/gpukxylif.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.bbcook.cn/Article/details/gpxrnebri.sHtML

[U104] JS：防抖
来源：http://www.share.vehdjk.com/Article/details/gnwmfzapx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/gxhqsbceu.sHtML

[U105] JS：节流
来源：http://wap.fktsv.cn/Article/details/gsbxhjcke.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.epnwcf.com/Article/details/gqemutult.sHtML

[U106] JS：日期格式化
来源：http://m.share.tarul.cn/Article/details/gaamdhhby.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.bbcook.cn/Article/details/gdhicrnfj.sHtML

[U107] JS：数字千分位
来源：http://wap.fktsv.cn/Article/details/gafubzmbp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fktsv.cn/Article/details/gwgwblpob.sHtML

[U108] JS：随机整数
来源：http://wap.sjlbkw.cn/Article/details/gcrqwzoqw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.tarul.cn/Article/details/gdmfseyfj.sHtML

[U109] JS：数组分组
来源：http://www.blog.yfazqb.com/Article/details/ggcqjzysf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.vehdjk.com/Article/details/gimmeofdr.sHtML

[U110] JS：数组分块
来源：http://3g.fktsv.cn/Article/details/gitpuuqzj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.epnwcf.com/Article/details/gciqkxwva.sHtML

[U111] JS：对象转 Map
来源：http://m.share.bbcook.cn/Article/details/gvhvblfxy.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fktsv.cn/Article/details/ghilvrmwb.sHtML

[U112] JS：字符串补位
来源：http://www.share.epnwcf.com/Article/details/gidtzrxwe.sHtML

"7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/gmeflusyb.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.sjlbkw.cn/Article/details/gogyaecmz.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gyrlwqikn.sHtML

[U114] JS：JSON 深比较
来源：http://blog.yfazqb.com/Article/details/gnopnsvgv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.sjlbkw.cn/Article/details/gmjosegrr.sHtML

[U115] JS：生成 UUID
来源：http://3g.epnwcf.com/Article/details/gqqenkznv.sHtML

crypto.randomUUID()
来源：http://www.blog.tarul.cn/Article/details/gthmdanpe.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.epnwcf.com/Article/details/gmzwpujkl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.sjlbkw.cn/Article/details/gcdmbhubk.sHtML

[U117] JS：单元测试
来源：http://mobile.fktsv.cn/Article/details/gwoonibqp.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.epnwcf.com/Article/details/gyaumudyh.sHtML

[U118] JS：开发服务器
来源：http://blog.epnwcf.com/Article/details/glsbxxlkt.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fktsv.cn/Article/details/gqcrrlsyj.sHtML

[U119] JS：生产构建
来源：http://baike.bbcook.cn/Article/details/givdzkrws.sHtML

npx vite build
来源：http://www.m.share.tarul.cn/Article/details/gypncqxet.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.vehdjk.com/Article/details/gpdormddl.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fktsv.cn/Article/details/gcdnhsymt.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gltbhjpty.sHtML

统计汇总
来源：http://blog.epnwcf.com/Article/details/gzskihrhh.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gbcpnblac.sHtML

按语言统计（条）：
来源：http://mobile.bbcook.cn/Article/details/ghrndvrcg.sHtML

Python ......... 252
来源：http://www.blog.vehdjk.com/Article/details/gisuvljdf.sHtML

PHP ............ 252
来源：http://www.blog.vehdjk.com/Article/details/gtbvzievj.sHtML

JavaScript ..... 252
来源：http://m.share.bbcook.cn/Article/details/gikdlwspr.sHtML

TypeScript ..... 212
来源：http://wap.tarul.cn/Article/details/gmasuyvil.sHtML

Java ........... 212
来源：http://blog.bbcook.cn/Article/details/ggcinmhxt.sHtML

Go ............. 212
来源：http://m.share.bbcook.cn/Article/details/gufnipbmr.sHtML

Ruby ........... 212
来源：http://mobile.vehdjk.com/Article/details/gcijwlscx.sHtML

C# ............. 212
来源：http://wap.yfazqb.com/Article/details/guhllxgyq.sHtML

C .............. 30
来源：http://mobile.bbcook.cn/Article/details/gjbufddfw.sHtML

C++ ............ 30
来源：http://3g.sjlbkw.cn/Article/details/gahttmnuv.sHtML

SQL ............ 90
来源：http://3g.fktsv.cn/Article/details/gdgwzcaiz.sHtML

Bash ........... 80
来源：http://www.blog.vehdjk.com/Article/details/gvfqkcwjk.sHtML

Kotlin ......... 15
来源：http://www.m.share.epnwcf.com/Article/details/gqsbbeskt.sHtML

Swift .......... 15
来源：http://www.m.share.bbcook.cn/Article/details/gskdujope.sHtML

Lua ............ 10
来源：http://wap.sjlbkw.cn/Article/details/gykevcajf.sHtML

Perl ........... 10
来源：http://m.share.yfazqb.com/Article/details/goxewbwwg.sHtML

Scala .......... 10
来源：http://www.blog.vehdjk.com/Article/details/gqkcogjfk.sHtML

------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gpbwetpbc.sHtML

合计 ........... 2106 条
来源：http://baike.sjlbkw.cn/Article/details/gicmkhpmb.sHtML

按章节统计：
来源：http://m.share.epnwcf.com/Article/details/gltdomvqh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.tarul.cn/Article/details/gmvobispx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.bbcook.cn/Article/details/gqjwnsquq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.tarul.cn/Article/details/gkcvnglmb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.vehdjk.com/Article/details/gljotajap.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.bbcook.cn/Article/details/grxhqalel.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.bbcook.cn/Article/details/gvqvslvhv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.tarul.cn/Article/details/gtotvzzwk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.tarul.cn/Article/details/gzpnxsopg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/goqytzfcx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.epnwcf.com/Article/details/gpkjmnies.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/gtqlbjmgx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/gnzewtymo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/gbxjfrvva.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.bbcook.cn/Article/details/gtioaojum.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fktsv.cn/Article/details/gbxvaxyhj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gwtmhwnas.sHtML

Q SQL 专题                              90
来源：http://www.m.share.epnwcf.com/Article/details/gyuoyjiyu.sHtML

R Bash 专题                             80
来源：http://m.share.sjlbkw.cn/Article/details/ggwquotlt.sHtML

S C / C++ 专题                          60
来源：http://wap.vehdjk.com/Article/details/gtdccuasw.sHtML

T 其他语言补充                          60
来源：http://www.blog.epnwcf.com/Article/details/glvaiwljl.sHtML

U 高频实用片段                         120
来源：http://baike.yfazqb.com/Article/details/glzixlahx.sHtML

------------------------------------
来源：http://read.share.tarul.cn/Article/details/gnryjxzer.sHtML

合计                                  2106 条
来源：http://m.share.epnwcf.com/Article/details/gqtmqfcmi.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gnjxkqbrt.sHtML

使用提醒
来源：http://blog.fktsv.cn/Article/details/gssfebebj.sHtML

--------------------------------------------------------------------------------
来源：http://baike.bbcook.cn/Article/details/gzppndtwu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.epnwcf.com/Article/details/ghlvjvcxf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.sjlbkw.cn/Article/details/gamvwieux.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.yfazqb.com/Article/details/gvawiaegf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fktsv.cn/Article/details/goqqmzese.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.vehdjk.com/Article/details/gatjrciqd.sHtML

—— 文件结束 ——
来源：http://wap.fktsv.cn/Article/details/gmelqsjsw.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gxwamcjpa.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.epnwcf.com/Article/details/gihonojdg.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fktsv.cn/Article/details/glkhwufdc.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gzppgalwd.sHtML

【收录内容】
来源：http://3g.sjlbkw.cn/Article/details/gtvgxdkpn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fktsv.cn/Article/details/gbggnuzgb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.sjlbkw.cn/Article/details/goxnoebri.sHtML

SQL · Bash · C · C++
来源：http://baike.sjlbkw.cn/Article/details/gedjoidce.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.tarul.cn/Article/details/gdewczinf.sHtML

【使用说明】
来源：http://www.blog.yfazqb.com/Article/details/gnogffhnw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.sjlbkw.cn/Article/details/gewshizyz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.epnwcf.com/Article/details/gxerangad.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.vehdjk.com/Article/details/gmafrlnvg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.yfazqb.com/Article/details/gcluqcyip.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.vehdjk.com/Article/details/gbshwsgsc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fktsv.cn/Article/details/grjltmlrp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.yfazqb.com/Article/details/gzejutfcj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.yfazqb.com/Article/details/gxwlhruom.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.vehdjk.com/Article/details/gprwpbtoz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.yfazqb.com/Article/details/gfkemtiza.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.bbcook.cn/Article/details/gelaxfhjq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.vehdjk.com/Article/details/gsyfhwvav.sHtML

【文件统计】
来源：http://www.m.share.sjlbkw.cn/Article/details/grqzyyfdc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.bbcook.cn/Article/details/gxvkwgdlv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.tarul.cn/Article/details/gvzpemigg.sHtML

目  录
来源：http://www.share.vehdjk.com/Article/details/gempxirqg.sHtML

--------------------------------------------------------------------------------
来源：http://baike.vehdjk.com/Article/details/ggtafbisf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.epnwcf.com/Article/details/gahchvpwz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.yfazqb.com/Article/details/gkpfcqwvj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.epnwcf.com/Article/details/ghpennnwk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.sjlbkw.cn/Article/details/gjhqiossm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.yfazqb.com/Article/details/gicgsefmu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.vehdjk.com/Article/details/gnoadxihm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.yfazqb.com/Article/details/gsppvuvve.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.bbcook.cn/Article/details/gasbugsrn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.yfazqb.com/Article/details/gcdsyjsvp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.yfazqb.com/Article/details/gcxqzbmlb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.tarul.cn/Article/details/gveibuvtv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.tarul.cn/Article/details/gmccktpgu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.sjlbkw.cn/Article/details/ganbdiqnj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.bbcook.cn/Article/details/gfcbpngln.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.epnwcf.com/Article/details/gmbkyuhzj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.tarul.cn/Article/details/gbrvccmhi.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.bbcook.cn/Article/details/glhdqczfz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.bbcook.cn/Article/details/gjvstxccr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fktsv.cn/Article/details/gdaxoflkw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fktsv.cn/Article/details/gcgookgsi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.vehdjk.com/Article/details/gghvolmwu.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gyxeaqksh.sHtML

A. 基础语法与类型
来源：http://blog.tarul.cn/Article/details/gjewndoqx.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/giihrckud.sHtML

[A01] Hello World
来源：http://mobile.vehdjk.com/Article/details/gzjtxmhpa.sHtML

Py:   print("Hello, World!")
来源：http://mobile.vehdjk.com/Article/details/gmdrfqaxw.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fktsv.cn/Article/details/gtocqtrtf.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fktsv.cn/Article/details/ggfhvwiub.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fktsv.cn/Article/details/gwvdzpjac.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.vehdjk.com/Article/details/gdnzchyft.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.vehdjk.com/Article/details/gvqpzqwuq.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.vehdjk.com/Article/details/gxqyzmptw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.yfazqb.com/Article/details/gqzmdesqs.sHtML

[A02] 变量声明与赋值
来源：http://www.share.bbcook.cn/Article/details/gtrsgviux.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.epnwcf.com/Article/details/gwxbvihpx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gqxfmdtrp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.bbcook.cn/Article/details/glsybzvus.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.epnwcf.com/Article/details/gpsirmghr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.sjlbkw.cn/Article/details/gmkuuxudl.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.vehdjk.com/Article/details/gipdvknxe.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmjtmlvl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.bbcook.cn/Article/details/gzvzoiaqi.sHtML

[A03] 常量定义
来源：http://3g.vehdjk.com/Article/details/gurqyfopi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.sjlbkw.cn/Article/details/gtsuiqsvs.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gyzjxaxlg.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/ghjnoftpk.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gcgagwoxf.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gcgkalthk.sHtML

Go:   const PI = 3.14159
来源：http://www.share.epnwcf.com/Article/details/glqzuorsn.sHtML

Ruby: PI = 3.14159
来源：http://3g.sjlbkw.cn/Article/details/gifvsxjgh.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gshwclxhy.sHtML

[A04] 判断变量类型
来源：http://www.blog.bbcook.cn/Article/details/grmnittbb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.epnwcf.com/Article/details/gzuqmozwk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.vehdjk.com/Article/details/glzfrylrw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.bbcook.cn/Article/details/gxigdwllf.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.yfazqb.com/Article/details/gfgacbull.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.tarul.cn/Article/details/ghkvyuazm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.tarul.cn/Article/details/gyozvhxql.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.tarul.cn/Article/details/geibybihs.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.tarul.cn/Article/details/gtafohnme.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.vehdjk.com/Article/details/gpggjaanr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.vehdjk.com/Article/details/gstqwyzsn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.sjlbkw.cn/Article/details/gtyqrqrfg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.vehdjk.com/Article/details/gfeuckbrt.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.bbcook.cn/Article/details/grmchatpj.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.epnwcf.com/Article/details/giotimjmb.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/gasmlzycy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.yfazqb.com/Article/details/gvuhnpqxj.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/gabvyrzzu.sHtML

[A06] 字符串转数字
来源：http://mobile.bbcook.cn/Article/details/germqkvrf.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.bbcook.cn/Article/details/gbdrrxkfr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.epnwcf.com/Article/details/gjpkoecwv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.bbcook.cn/Article/details/gexnqzeud.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.sjlbkw.cn/Article/details/gwktmnqyt.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.yfazqb.com/Article/details/gvbsltbyz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.tarul.cn/Article/details/gslwfyybz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.bbcook.cn/Article/details/gjkguofgx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.sjlbkw.cn/Article/details/gljnlinpo.sHtML

[A07] 数字转字符串
来源：http://baike.tarul.cn/Article/details/gotuiedfi.sHtML

Py:   str(42)
来源：http://m.share.yfazqb.com/Article/details/gdqxcxqiy.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.epnwcf.com/Article/details/gwcwjpxnm.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.sjlbkw.cn/Article/details/gdfofexqr.sHtML

TS:   String(42)
来源：http://3g.tarul.cn/Article/details/gvzdassig.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.yfazqb.com/Article/details/gvcosxpqm.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.epnwcf.com/Article/details/gjhqrfegq.sHtML

Ruby: 42.to_s
来源：http://blog.yfazqb.com/Article/details/gcybngojx.sHtML

C#:   42.ToString()
来源：http://m.share.fktsv.cn/Article/details/gubiprznd.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fktsv.cn/Article/details/grjeyevsd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmzhhocw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.epnwcf.com/Article/details/gykcgzrst.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fktsv.cn/Article/details/gweehxtxa.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.yfazqb.com/Article/details/gxskhndbg.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.tarul.cn/Article/details/gnwpksgsl.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.fktsv.cn/Article/details/gztlpmqvm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.epnwcf.com/Article/details/gyzefospg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fktsv.cn/Article/details/gznkqvyew.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.tarul.cn/Article/details/gesuglayx.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.epnwcf.com/Article/details/gnpbxnodm.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gqmutaeap.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.vehdjk.com/Article/details/giobixicj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gtxqmxxwg.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gutqkwiat.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fktsv.cn/Article/details/gchnkvpgv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.bbcook.cn/Article/details/gqpyretfz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gbyicsxof.sHtML

[A10] 生成随机数
来源：http://wap.yfazqb.com/Article/details/gdacqyvex.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.bbcook.cn/Article/details/grlwclzkk.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.vehdjk.com/Article/details/glnmlwmme.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.tarul.cn/Article/details/gennrejql.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.epnwcf.com/Article/details/gfmheqmak.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.epnwcf.com/Article/details/gkwohnudb.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.vehdjk.com/Article/details/gvaixuaxq.sHtML

Ruby: rand(1..100)
来源：http://mobile.tarul.cn/Article/details/gsolzsymm.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.vehdjk.com/Article/details/gwrpjogxi.sHtML

[A11] 条件表达式（三元）
来源：http://blog.bbcook.cn/Article/details/guvzwzuxp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.vehdjk.com/Article/details/gpdvfohfn.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.bbcook.cn/Article/details/gfuijgxog.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.vehdjk.com/Article/details/ghiqnrotp.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.sjlbkw.cn/Article/details/gfwgegayx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/gudhgysyf.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.tarul.cn/Article/details/gzlkyahzy.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.bbcook.cn/Article/details/grsbmpdtn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gfzgtihsg.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.bbcook.cn/Article/details/gondjwpgd.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.epnwcf.com/Article/details/ghslhwdvr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.yfazqb.com/Article/details/gtytmfnor.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.tarul.cn/Article/details/gpuaeqbsd.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.vehdjk.com/Article/details/gcrylvbwn.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxftkvrt.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.vehdjk.com/Article/details/gzzvwxyqq.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.bbcook.cn/Article/details/gvutyqqrq.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.yfazqb.com/Article/details/gqvojzfok.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fktsv.cn/Article/details/gzeiasbzm.sHtML

Py:   "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/gfkumcjdz.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.yfazqb.com/Article/details/gfkalfokv.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/gsmuzzbhe.sHtML

TS:   "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gfuhcrecx.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.epnwcf.com/Article/details/gvyzfnqqt.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/geffduwtp.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gaqkfcskv.sHtML

C#:   "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/gmpcqzzna.sHtML

[A14] 注释写法
来源：http://www.blog.epnwcf.com/Article/details/gqsdgsydj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fktsv.cn/Article/details/gwcyaaxtf.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.yfazqb.com/Article/details/gampmvyzz.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.yfazqb.com/Article/details/gmcsktezd.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.tarul.cn/Article/details/gkrjkxpqm.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fktsv.cn/Article/details/grlpdfaxv.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/gmdmaxvdj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.bbcook.cn/Article/details/gnffchotk.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.vehdjk.com/Article/details/gadlnzgen.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.bbcook.cn/Article/details/gmopwrbow.sHtML

Py:   value = data or "默认值"
来源：http://blog.tarul.cn/Article/details/gujndwayl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.epnwcf.com/Article/details/glcrbleqm.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.sjlbkw.cn/Article/details/gpzwhejuj.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.sjlbkw.cn/Article/details/gzpxizkws.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzdisnrc.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.tarul.cn/Article/details/gfixqubnf.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.tarul.cn/Article/details/gvpiqajot.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.bbcook.cn/Article/details/gclfzjaov.sHtML

[A16] 真假值判断规则
来源：http://read.share.bbcook.cn/Article/details/gskpspjjy.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.bbcook.cn/Article/details/gjiijszhb.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.yfazqb.com/Article/details/gyliitzor.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.vehdjk.com/Article/details/grnfjpunk.sHtML

TS:   if (!x) {}
来源：http://baike.sjlbkw.cn/Article/details/gkrinxkmh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.epnwcf.com/Article/details/gqgtpxgzj.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.fktsv.cn/Article/details/giyiwckna.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.epnwcf.com/Article/details/gxhbotgyf.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.vehdjk.com/Article/details/gdzifqppr.sHtML

[A17] 位运算
来源：http://wap.yfazqb.com/Article/details/gpytpbhax.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/ghknepbib.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.vehdjk.com/Article/details/gwwdzwigu.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.tarul.cn/Article/details/gabdqvnyp.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/gxepuhyqy.sHtML


<!-- 参考信息 -->