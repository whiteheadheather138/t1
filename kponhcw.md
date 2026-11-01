代发 wailian999

[U101] JS：classList 操作
来源：http://baike.vehdjk.com/Article/details/gwioupeds.sHtML

el.classList.toggle("active")
来源：http://read.share.tarul.cn/Article/details/gvcwaawqv.sHtML

[U102] JS：本地存储
来源：http://wap.fktsv.cn/Article/details/gutpknxkl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.vehdjk.com/Article/details/ghhzvbtcc.sHtML

[U103] JS：定时器
来源：http://www.share.sjlbkw.cn/Article/details/gwwwnkixh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.vehdjk.com/Article/details/guoqnumnc.sHtML

[U104] JS：防抖
来源：http://blog.sjlbkw.cn/Article/details/gqyxivrls.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gjgwcfuxd.sHtML

[U105] JS：节流
来源：http://blog.fktsv.cn/Article/details/gzlwvwova.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.tarul.cn/Article/details/gchihngsg.sHtML

[U106] JS：日期格式化
来源：http://mobile.tarul.cn/Article/details/gziladnjj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.yfazqb.com/Article/details/gjxungisj.sHtML

[U107] JS：数字千分位
来源：http://m.share.yfazqb.com/Article/details/gjnlypxle.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.epnwcf.com/Article/details/gukknczco.sHtML

[U108] JS：随机整数
来源：http://3g.yfazqb.com/Article/details/geysjiqfb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fktsv.cn/Article/details/gmgmpajhb.sHtML

[U109] JS：数组分组
来源：http://www.share.vehdjk.com/Article/details/gtjajvdhg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.sjlbkw.cn/Article/details/gkpsdqjba.sHtML

[U110] JS：数组分块
来源：http://mobile.tarul.cn/Article/details/goqkjbjqn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.yfazqb.com/Article/details/gmgokstgp.sHtML

[U111] JS：对象转 Map
来源：http://m.share.tarul.cn/Article/details/ggmtxvsrx.sHtML

new Map(Object.entries(obj))
来源：http://www.share.yfazqb.com/Article/details/gvdstvsrh.sHtML

[U112] JS：字符串补位
来源：http://mobile.fktsv.cn/Article/details/gtabzsdwo.sHtML

"7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gvqpkvajk.sHtML

[U113] JS：正则替换全部
来源：http://mobile.bbcook.cn/Article/details/gusrqtbsy.sHtML

s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gyhhvdunu.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fktsv.cn/Article/details/gcksppbxy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.bbcook.cn/Article/details/gdfcipqvw.sHtML

[U115] JS：生成 UUID
来源：http://read.share.yfazqb.com/Article/details/glcnfnkmv.sHtML

crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gglrvmvmx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.vehdjk.com/Article/details/gudrknacq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fktsv.cn/Article/details/gunlwtwxo.sHtML

[U117] JS：单元测试
来源：http://blog.fktsv.cn/Article/details/gqkhzsrhc.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.yfazqb.com/Article/details/gykvsmjqf.sHtML

[U118] JS：开发服务器
来源：http://read.share.epnwcf.com/Article/details/gxeuyfbma.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.tarul.cn/Article/details/gokkzrfeq.sHtML

[U119] JS：生产构建
来源：http://read.share.yfazqb.com/Article/details/gsozhtosj.sHtML

npx vite build
来源：http://read.share.bbcook.cn/Article/details/gvnwcsugi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.sjlbkw.cn/Article/details/gstgcjukn.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.vehdjk.com/Article/details/gzqxzrevh.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gqhqhrvzp.sHtML

统计汇总
来源：http://read.share.tarul.cn/Article/details/gddecwvha.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gmgjvygrb.sHtML

按语言统计（条）：
来源：http://wap.tarul.cn/Article/details/gllksliry.sHtML

Python ......... 252
来源：http://blog.epnwcf.com/Article/details/gqdwricue.sHtML

PHP ............ 252
来源：http://m.share.tarul.cn/Article/details/gipecvbru.sHtML

JavaScript ..... 252
来源：http://m.share.yfazqb.com/Article/details/gfdvoyjgx.sHtML

TypeScript ..... 212
来源：http://wap.fktsv.cn/Article/details/gmteraelt.sHtML

Java ........... 212
来源：http://blog.tarul.cn/Article/details/gyyfeboxj.sHtML

Go ............. 212
来源：http://www.share.tarul.cn/Article/details/gsxskmqta.sHtML

Ruby ........... 212
来源：http://3g.vehdjk.com/Article/details/gxnjvgspn.sHtML

C# ............. 212
来源：http://www.m.share.epnwcf.com/Article/details/gwynegsmv.sHtML

C .............. 30
来源：http://mobile.bbcook.cn/Article/details/grbgjerbu.sHtML

C++ ............ 30
来源：http://wap.epnwcf.com/Article/details/gtwsrgjro.sHtML

SQL ............ 90
来源：http://www.m.share.bbcook.cn/Article/details/guaufnwmc.sHtML

Bash ........... 80
来源：http://www.m.share.bbcook.cn/Article/details/gpxtzlpfu.sHtML

Kotlin ......... 15
来源：http://www.share.epnwcf.com/Article/details/gnxxvkdug.sHtML

Swift .......... 15
来源：http://www.m.share.bbcook.cn/Article/details/gnazeeeuy.sHtML

Lua ............ 10
来源：http://www.share.vehdjk.com/Article/details/gyyhffree.sHtML

Perl ........... 10
来源：http://baike.tarul.cn/Article/details/gxkkvmjdx.sHtML

Scala .......... 10
来源：http://www.blog.sjlbkw.cn/Article/details/gvaxxmtrk.sHtML

------------------------------------
来源：http://blog.yfazqb.com/Article/details/gusngirnr.sHtML

合计 ........... 2106 条
来源：http://read.share.epnwcf.com/Article/details/gnawqmbns.sHtML

按章节统计：
来源：http://www.blog.epnwcf.com/Article/details/gvijftpij.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.yfazqb.com/Article/details/gqgesusof.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.tarul.cn/Article/details/ggowhters.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.tarul.cn/Article/details/ghjeaanvt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.tarul.cn/Article/details/gzuzevxck.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.epnwcf.com/Article/details/gebudabku.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.sjlbkw.cn/Article/details/gndigmory.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.yfazqb.com/Article/details/gpophzhuv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fktsv.cn/Article/details/gjjmfhtqj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gxinmaolb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.tarul.cn/Article/details/gnyxvmbqe.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gdfavcoqq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gzbkjaekj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/gnxifeaqs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxxwkjhz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.yfazqb.com/Article/details/gnoaescua.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/grlzzlzmd.sHtML

Q SQL 专题                              90
来源：http://mobile.bbcook.cn/Article/details/gskmsdcxe.sHtML

R Bash 专题                             80
来源：http://3g.sjlbkw.cn/Article/details/gykwhfhgq.sHtML

S C / C++ 专题                          60
来源：http://baike.epnwcf.com/Article/details/ggdzyrorl.sHtML

T 其他语言补充                          60
来源：http://read.share.epnwcf.com/Article/details/gweweklrk.sHtML

U 高频实用片段                         120
来源：http://3g.vehdjk.com/Article/details/grjujiyqd.sHtML

------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gtrbrxnbl.sHtML

合计                                  2106 条
来源：http://blog.sjlbkw.cn/Article/details/gtbanuwwh.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/gnnvfwove.sHtML

使用提醒
来源：http://mobile.fktsv.cn/Article/details/gtpogdkva.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gablrjiuw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.sjlbkw.cn/Article/details/gexlwtvsr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.epnwcf.com/Article/details/gnaidcehf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.bbcook.cn/Article/details/gxmhltlkv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.yfazqb.com/Article/details/grobeqdkp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.yfazqb.com/Article/details/guiuugkng.sHtML

—— 文件结束 ——
来源：http://www.share.yfazqb.com/Article/details/gnkzdohlw.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gpipmrnkn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fktsv.cn/Article/details/goootlgen.sHtML

Common Programming Examples Cheat Book
来源：http://3g.tarul.cn/Article/details/gotqrzbvn.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ggvrfgyhm.sHtML

【收录内容】
来源：http://www.share.vehdjk.com/Article/details/gxlfpstal.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fktsv.cn/Article/details/gutqktcfm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.epnwcf.com/Article/details/gddvbanih.sHtML

SQL · Bash · C · C++
来源：http://www.share.sjlbkw.cn/Article/details/ghzgxwfdc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.bbcook.cn/Article/details/gdjojgmnn.sHtML

【使用说明】
来源：http://blog.fktsv.cn/Article/details/grlfggwyw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.vehdjk.com/Article/details/ghuaxiuke.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.sjlbkw.cn/Article/details/gtzuwlbwe.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fktsv.cn/Article/details/gtilybrzs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fktsv.cn/Article/details/gjspmsbuw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.sjlbkw.cn/Article/details/gqwbzcmqp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.epnwcf.com/Article/details/gjjefiexo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.vehdjk.com/Article/details/gwnmbqseo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.sjlbkw.cn/Article/details/gpkilmxmw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.vehdjk.com/Article/details/gmazpejgz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhjomvjx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.yfazqb.com/Article/details/gkvofvmbu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.tarul.cn/Article/details/gdnxdalvo.sHtML

【文件统计】
来源：http://www.share.bbcook.cn/Article/details/gjhikkftz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.yfazqb.com/Article/details/gfhmnqmbv.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gunsdhfty.sHtML

目  录
来源：http://mobile.bbcook.cn/Article/details/gbppmjsrg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gepcymqec.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.yfazqb.com/Article/details/gqbrwnhof.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fktsv.cn/Article/details/gazdeqztm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.yfazqb.com/Article/details/gxutkkpbj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.epnwcf.com/Article/details/giahjnchu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.yfazqb.com/Article/details/gciodgyra.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.tarul.cn/Article/details/gvmooxeqb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/gpsakmqtd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.bbcook.cn/Article/details/gdrmyxjyg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.sjlbkw.cn/Article/details/gdwevsund.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.epnwcf.com/Article/details/gounhuyvc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fktsv.cn/Article/details/gncliinfh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gpxoukrma.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.sjlbkw.cn/Article/details/gyngoykhs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.bbcook.cn/Article/details/ghypvowot.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.epnwcf.com/Article/details/gjcqupdss.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.bbcook.cn/Article/details/gbuptqqhz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.bbcook.cn/Article/details/gtwqgtnir.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.yfazqb.com/Article/details/ggozzfsyb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.bbcook.cn/Article/details/gjowmezzh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.yfazqb.com/Article/details/gwkvywobf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.yfazqb.com/Article/details/guwmlzego.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gqchgiqpj.sHtML

A. 基础语法与类型
来源：http://3g.tarul.cn/Article/details/gaqknefia.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gwbitymtb.sHtML

[A01] Hello World
来源：http://read.share.epnwcf.com/Article/details/gyeagylrc.sHtML

Py:   print("Hello, World!")
来源：http://blog.tarul.cn/Article/details/goxljsqnb.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.bbcook.cn/Article/details/gcmlliyjw.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.sjlbkw.cn/Article/details/gnxktxowt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.yfazqb.com/Article/details/gfqvxelng.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.epnwcf.com/Article/details/ghnphtnjd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.yfazqb.com/Article/details/guvhknswp.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fktsv.cn/Article/details/gospdbrql.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.epnwcf.com/Article/details/glxjngvto.sHtML

[A02] 变量声明与赋值
来源：http://3g.tarul.cn/Article/details/gpsjlplqq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.epnwcf.com/Article/details/gtjnkrhdh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.sjlbkw.cn/Article/details/gcrkecxtn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gtgitlmhz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.sjlbkw.cn/Article/details/gankcthmg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.tarul.cn/Article/details/gxfllfqrn.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.tarul.cn/Article/details/ghxhlvowx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.epnwcf.com/Article/details/gcikvxwoy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.epnwcf.com/Article/details/gkhehbiag.sHtML

[A03] 常量定义
来源：http://blog.epnwcf.com/Article/details/goawbbzwx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.epnwcf.com/Article/details/gugreuhku.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/grhvlhviv.sHtML

JS:   const PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gkqbavydv.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gzhzfeaoi.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/garntmgsx.sHtML

Go:   const PI = 3.14159
来源：http://baike.fktsv.cn/Article/details/gpsjzkhit.sHtML

Ruby: PI = 3.14159
来源：http://blog.fktsv.cn/Article/details/gkbjuouoz.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/grdmslaoj.sHtML

[A04] 判断变量类型
来源：http://www.share.yfazqb.com/Article/details/ggqwlyoca.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.yfazqb.com/Article/details/ghwauqbqk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fktsv.cn/Article/details/gtwpwscpf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fktsv.cn/Article/details/gksypnghe.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.yfazqb.com/Article/details/gqnodyqav.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.yfazqb.com/Article/details/gxdpwuvnf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.yfazqb.com/Article/details/gmvryolny.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.yfazqb.com/Article/details/gvyrtmikm.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.vehdjk.com/Article/details/gpnsfevvj.sHtML

[A05] 整数除法与取模
来源：http://blog.sjlbkw.cn/Article/details/gjlccwjhc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fktsv.cn/Article/details/gryxfhtja.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gxauamocf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/guesaidbv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.epnwcf.com/Article/details/gvcaqpwrf.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.epnwcf.com/Article/details/guetkcobb.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fktsv.cn/Article/details/gdytgyeua.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.tarul.cn/Article/details/gzyisseca.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.epnwcf.com/Article/details/gapxivrln.sHtML

[A06] 字符串转数字
来源：http://m.share.yfazqb.com/Article/details/gzythdaxd.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.sjlbkw.cn/Article/details/gnoejkzuc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.sjlbkw.cn/Article/details/gcfafxkop.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.bbcook.cn/Article/details/gyeqtcfwi.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.bbcook.cn/Article/details/gslolnqts.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.bbcook.cn/Article/details/gohgffiao.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.epnwcf.com/Article/details/ggnlvqmgm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.yfazqb.com/Article/details/ghqjcwcjo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.sjlbkw.cn/Article/details/gagjzaxdz.sHtML

[A07] 数字转字符串
来源：http://read.share.vehdjk.com/Article/details/gpzuxifkl.sHtML

Py:   str(42)
来源：http://www.share.tarul.cn/Article/details/goyiiogeq.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.epnwcf.com/Article/details/gjktqxibf.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.epnwcf.com/Article/details/glcpulzng.sHtML

TS:   String(42)
来源：http://m.share.yfazqb.com/Article/details/gxhqszgkw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.tarul.cn/Article/details/gyxgzkwys.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.tarul.cn/Article/details/ggkyrrgeq.sHtML

Ruby: 42.to_s
来源：http://read.share.vehdjk.com/Article/details/gdcvaralx.sHtML

C#:   42.ToString()
来源：http://www.blog.fktsv.cn/Article/details/gvhiypibv.sHtML

[A08] 取整与四舍五入
来源：http://read.share.bbcook.cn/Article/details/gqfjyuugm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.tarul.cn/Article/details/gkortfadt.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.bbcook.cn/Article/details/gtamzghbg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.bbcook.cn/Article/details/gwipgetwf.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.vehdjk.com/Article/details/gjkpxjxvx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.tarul.cn/Article/details/gqwlqyywk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.sjlbkw.cn/Article/details/gosxezwht.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.bbcook.cn/Article/details/gnabukvup.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.sjlbkw.cn/Article/details/ggnkbaccl.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.epnwcf.com/Article/details/gapmxtbmn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gscejefhq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gozwhkpmb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gfgcryfst.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.vehdjk.com/Article/details/gjzfuywek.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gvvvunsbd.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.bbcook.cn/Article/details/gluequhan.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.tarul.cn/Article/details/gqcyaighw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gpysnqali.sHtML

[A10] 生成随机数
来源：http://mobile.tarul.cn/Article/details/gugyvpeyi.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.sjlbkw.cn/Article/details/gfvyghlhf.sHtML

PHP:  random_int(1, 100);
来源：http://wap.tarul.cn/Article/details/gtldmuhaj.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkphotxf.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.vehdjk.com/Article/details/gljnaajky.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gflvhoueg.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.fktsv.cn/Article/details/glpvikktd.sHtML

Ruby: rand(1..100)
来源：http://3g.vehdjk.com/Article/details/glswcmydj.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.yfazqb.com/Article/details/gvhcmbgfh.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.yfazqb.com/Article/details/ghtyohmfe.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.vehdjk.com/Article/details/grcvyqtkm.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.yfazqb.com/Article/details/gctvaknsy.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.vehdjk.com/Article/details/gcocbwubn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.bbcook.cn/Article/details/grmsjmxab.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/gnkpkezae.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.vehdjk.com/Article/details/gkrodlnxt.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.yfazqb.com/Article/details/gtrwvkyry.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/gennfjrhx.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.sjlbkw.cn/Article/details/gxglhmaxp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.bbcook.cn/Article/details/ghwdicztd.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.sjlbkw.cn/Article/details/gwkoxynmx.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.tarul.cn/Article/details/gjoliiypa.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.epnwcf.com/Article/details/gaxzqwuem.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.tarul.cn/Article/details/gnsubyrre.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.vehdjk.com/Article/details/gamhrjibx.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.vehdjk.com/Article/details/gydenikzq.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.yfazqb.com/Article/details/grubdnkpj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fktsv.cn/Article/details/gnctdupkb.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/gsbbnmimb.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/govxzjgss.sHtML

JS:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gwbsfacue.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/gzdsyndxm.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/gtgcgviwr.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/gwuyklusw.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.fktsv.cn/Article/details/gjbrufkjf.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fktsv.cn/Article/details/gjiuabahs.sHtML

[A14] 注释写法
来源：http://mobile.fktsv.cn/Article/details/gfkvgofve.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.vehdjk.com/Article/details/gzfwmzpbt.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.epnwcf.com/Article/details/gbdotgqmo.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.sjlbkw.cn/Article/details/gufcwntvb.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.epnwcf.com/Article/details/ghntgpnue.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.vehdjk.com/Article/details/gtnfrqsba.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.tarul.cn/Article/details/gmpvajzbu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.bbcook.cn/Article/details/giovzkewa.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fktsv.cn/Article/details/gyyekdxhy.sHtML

[A15] 空值判断与默认值
来源：http://3g.bbcook.cn/Article/details/gxkwoozpq.sHtML

Py:   value = data or "默认值"
来源：http://m.share.bbcook.cn/Article/details/gzkjsomvc.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.yfazqb.com/Article/details/gpocyfmns.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.epnwcf.com/Article/details/gqlqdllsj.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.sjlbkw.cn/Article/details/gnggorzmv.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.bbcook.cn/Article/details/ggssrizbf.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.yfazqb.com/Article/details/gslzefmnm.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fktsv.cn/Article/details/gwsdyhugq.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.sjlbkw.cn/Article/details/gafbkazcx.sHtML

[A16] 真假值判断规则
来源：http://m.share.fktsv.cn/Article/details/gvqbpsjur.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.yfazqb.com/Article/details/gbhwhnrdf.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.sjlbkw.cn/Article/details/gqvtldhzm.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fktsv.cn/Article/details/ggjlcjhja.sHtML

TS:   if (!x) {}
来源：http://www.blog.bbcook.cn/Article/details/gxmjfldlo.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.bbcook.cn/Article/details/gwsiulwka.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.epnwcf.com/Article/details/gomaszovd.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.bbcook.cn/Article/details/gsnbjfdqm.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gkjhtqnai.sHtML

[A17] 位运算
来源：http://www.share.epnwcf.com/Article/details/gfmkrstnk.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/gpzwghlxk.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/ghwtgwvri.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/gvtydagbq.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/guijioper.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.yfazqb.com/Article/details/gepsxwaje.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gbyudebio.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gcmnojuml.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/gjzxmtttl.sHtML


<!-- 参考信息 -->