代发 wailian999

[U101] JS：classList 操作
来源：http://wap.epnwcf.com/Article/details/gsuoznaxa.sHtML

el.classList.toggle("active")
来源：http://read.share.sjlbkw.cn/Article/details/grmocmhno.sHtML

[U102] JS：本地存储
来源：http://www.m.share.epnwcf.com/Article/details/gdqsupsqc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.vehdjk.com/Article/details/gamoynklx.sHtML

[U103] JS：定时器
来源：http://read.share.fktsv.cn/Article/details/gacsstafv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fktsv.cn/Article/details/gpctonoln.sHtML

[U104] JS：防抖
来源：http://www.m.share.bbcook.cn/Article/details/gmxptckym.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.vehdjk.com/Article/details/gzbsfswgy.sHtML

[U105] JS：节流
来源：http://m.share.tarul.cn/Article/details/gvhjxvppy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.epnwcf.com/Article/details/gwxkwxyzz.sHtML

[U106] JS：日期格式化
来源：http://read.share.fktsv.cn/Article/details/gobomtwjl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.bbcook.cn/Article/details/gpvmxavmi.sHtML

[U107] JS：数字千分位
来源：http://baike.sjlbkw.cn/Article/details/gsfbotxwb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.sjlbkw.cn/Article/details/gzqjfdirx.sHtML

[U108] JS：随机整数
来源：http://3g.fktsv.cn/Article/details/gbyjldvul.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fktsv.cn/Article/details/grjubrqxy.sHtML

[U109] JS：数组分组
来源：http://mobile.epnwcf.com/Article/details/gevvwtfmu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.yfazqb.com/Article/details/gvhvuyyjt.sHtML

[U110] JS：数组分块
来源：http://mobile.tarul.cn/Article/details/gajrdjnxq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.epnwcf.com/Article/details/gxkfnlfaj.sHtML

[U111] JS：对象转 Map
来源：http://m.share.bbcook.cn/Article/details/gjcmfmtcg.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.bbcook.cn/Article/details/gtaaklxdi.sHtML

[U112] JS：字符串补位
来源：http://wap.tarul.cn/Article/details/gbhhyuqyi.sHtML

"7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gahsgwojk.sHtML

[U113] JS：正则替换全部
来源：http://3g.yfazqb.com/Article/details/gsgnsakia.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gynhygjts.sHtML

[U114] JS：JSON 深比较
来源：http://blog.vehdjk.com/Article/details/gmzadvnkl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.tarul.cn/Article/details/gvhkabteu.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fktsv.cn/Article/details/ggcodomzt.sHtML

crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gpnqwmciq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fktsv.cn/Article/details/gzoaazehu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.vehdjk.com/Article/details/geqwnurkb.sHtML

[U117] JS：单元测试
来源：http://baike.vehdjk.com/Article/details/gpaxasldt.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.vehdjk.com/Article/details/gvzozhbha.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.vehdjk.com/Article/details/gdiwjcqnr.sHtML

npm i -D vite;  npx vite
来源：http://blog.epnwcf.com/Article/details/gvdcdgspv.sHtML

[U119] JS：生产构建
来源：http://wap.vehdjk.com/Article/details/gdzfhsnvz.sHtML

npx vite build
来源：http://wap.bbcook.cn/Article/details/gnrgaoipt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.yfazqb.com/Article/details/gowjxjzhc.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fktsv.cn/Article/details/gkuryyckg.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/garwklkau.sHtML

统计汇总
来源：http://wap.vehdjk.com/Article/details/giyzhfyax.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gdtqijkly.sHtML

按语言统计（条）：
来源：http://blog.bbcook.cn/Article/details/gqhkinogr.sHtML

Python ......... 252
来源：http://www.blog.vehdjk.com/Article/details/gfubzchvz.sHtML

PHP ............ 252
来源：http://read.share.bbcook.cn/Article/details/gpwzndzaw.sHtML

JavaScript ..... 252
来源：http://baike.epnwcf.com/Article/details/gzdasgrwn.sHtML

TypeScript ..... 212
来源：http://baike.epnwcf.com/Article/details/ggrisqewq.sHtML

Java ........... 212
来源：http://wap.tarul.cn/Article/details/gsrphthuh.sHtML

Go ............. 212
来源：http://m.share.vehdjk.com/Article/details/gjhbblfkm.sHtML

Ruby ........... 212
来源：http://www.blog.sjlbkw.cn/Article/details/ggvfesmkq.sHtML

C# ............. 212
来源：http://baike.vehdjk.com/Article/details/gqlfbhmxp.sHtML

C .............. 30
来源：http://blog.sjlbkw.cn/Article/details/gobowawqc.sHtML

C++ ............ 30
来源：http://blog.sjlbkw.cn/Article/details/gblgpkmqq.sHtML

SQL ............ 90
来源：http://blog.fktsv.cn/Article/details/gngriqmjg.sHtML

Bash ........... 80
来源：http://baike.vehdjk.com/Article/details/gchsvkspt.sHtML

Kotlin ......... 15
来源：http://mobile.vehdjk.com/Article/details/glnaprltm.sHtML

Swift .......... 15
来源：http://3g.tarul.cn/Article/details/gizklxqmx.sHtML

Lua ............ 10
来源：http://m.share.vehdjk.com/Article/details/gokxvsial.sHtML

Perl ........... 10
来源：http://baike.fktsv.cn/Article/details/gdsicsgdm.sHtML

Scala .......... 10
来源：http://mobile.yfazqb.com/Article/details/gbiypcayt.sHtML

------------------------------------
来源：http://baike.fktsv.cn/Article/details/gmqqyoiib.sHtML

合计 ........... 2106 条
来源：http://www.blog.vehdjk.com/Article/details/gkvchpnwf.sHtML

按章节统计：
来源：http://wap.epnwcf.com/Article/details/gdqtvhixl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.epnwcf.com/Article/details/gjrrlfmhj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.bbcook.cn/Article/details/gglbygbey.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.sjlbkw.cn/Article/details/glllhipdd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fktsv.cn/Article/details/gplrlvdjw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.sjlbkw.cn/Article/details/gsukvgesc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fktsv.cn/Article/details/gxhlhfwgq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.bbcook.cn/Article/details/grkrkbnph.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.yfazqb.com/Article/details/gqoqqpmdq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gfkyhnrzu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fktsv.cn/Article/details/gjlciygay.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/gizftjmun.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gtrwpwetr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/gxacwxymf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.tarul.cn/Article/details/goxspheyg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.epnwcf.com/Article/details/gcrfduvww.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/gejkmynlf.sHtML

Q SQL 专题                              90
来源：http://blog.fktsv.cn/Article/details/gvjtmdxdy.sHtML

R Bash 专题                             80
来源：http://blog.yfazqb.com/Article/details/gxsgclywm.sHtML

S C / C++ 专题                          60
来源：http://blog.bbcook.cn/Article/details/gvsohfoap.sHtML

T 其他语言补充                          60
来源：http://read.share.tarul.cn/Article/details/gwzbsucoc.sHtML

U 高频实用片段                         120
来源：http://blog.vehdjk.com/Article/details/gxlcsvsek.sHtML

------------------------------------
来源：http://3g.tarul.cn/Article/details/gajrjgazg.sHtML

合计                                  2106 条
来源：http://blog.bbcook.cn/Article/details/ggztjcjkb.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/gvymsydry.sHtML

使用提醒
来源：http://www.share.bbcook.cn/Article/details/gueebmpet.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/gqxuwiopu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fktsv.cn/Article/details/groycsegd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.yfazqb.com/Article/details/gmlofftqt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.yfazqb.com/Article/details/gicufdman.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.epnwcf.com/Article/details/glhvbkioe.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fktsv.cn/Article/details/geubcdanu.sHtML

—— 文件结束 ——
来源：http://www.blog.tarul.cn/Article/details/gpqhepiml.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gyizelkfu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.tarul.cn/Article/details/gidesjivv.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.epnwcf.com/Article/details/glzegucvz.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gzwmeixca.sHtML

【收录内容】
来源：http://m.share.yfazqb.com/Article/details/gvmttngqa.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.epnwcf.com/Article/details/gfazgupvs.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.bbcook.cn/Article/details/gcxsyfzsz.sHtML

SQL · Bash · C · C++
来源：http://www.share.epnwcf.com/Article/details/gszcdbbxa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.vehdjk.com/Article/details/gzmaxdode.sHtML

【使用说明】
来源：http://m.share.yfazqb.com/Article/details/ggpcnxecn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.vehdjk.com/Article/details/goxgfqwld.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.yfazqb.com/Article/details/gbazklpjw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.yfazqb.com/Article/details/gpxkgbbkt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.bbcook.cn/Article/details/gjhnpsurp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.sjlbkw.cn/Article/details/gefjpqzbh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.sjlbkw.cn/Article/details/gvhvhtbwt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.vehdjk.com/Article/details/gixfpfauc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.tarul.cn/Article/details/gedmqvpzf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.sjlbkw.cn/Article/details/gmjfklumx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.tarul.cn/Article/details/gqqxkejai.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.vehdjk.com/Article/details/gluhewbzh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.tarul.cn/Article/details/gjzzggzhd.sHtML

【文件统计】
来源：http://blog.sjlbkw.cn/Article/details/gzaakbnaf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.sjlbkw.cn/Article/details/gtmdfzexp.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.yfazqb.com/Article/details/gkckzgumf.sHtML

目  录
来源：http://wap.bbcook.cn/Article/details/gpapngfqg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gerwnjuae.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fktsv.cn/Article/details/gapydrbkf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/gampmzudq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.epnwcf.com/Article/details/gdaoitnts.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.vehdjk.com/Article/details/gwynltlxu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.epnwcf.com/Article/details/gfbygqerz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.bbcook.cn/Article/details/girvmqtpc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fktsv.cn/Article/details/gcxaswfwq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.bbcook.cn/Article/details/gvfiwyzhp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/ggwzesgiw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.epnwcf.com/Article/details/guxpirbul.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.bbcook.cn/Article/details/gtfykzyvb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/gghieyaif.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/gkdbvlvvp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.yfazqb.com/Article/details/gycvcbdny.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.vehdjk.com/Article/details/gtgpychwr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/gxmdmqonq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fktsv.cn/Article/details/gsnxnevtr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.bbcook.cn/Article/details/gvvislqbu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.yfazqb.com/Article/details/gyuwccncc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.epnwcf.com/Article/details/gvtsepzpx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gopaugbqp.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gpfqzbkae.sHtML

A. 基础语法与类型
来源：http://blog.yfazqb.com/Article/details/gycutvsmr.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gmdaohupj.sHtML

[A01] Hello World
来源：http://blog.sjlbkw.cn/Article/details/gmtaryrxg.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.tarul.cn/Article/details/gcirqrwfi.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fktsv.cn/Article/details/gnbsigxqk.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.sjlbkw.cn/Article/details/gmkxgopvo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fktsv.cn/Article/details/gggawjdor.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.yfazqb.com/Article/details/gcpwlnupq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.tarul.cn/Article/details/gnghratqw.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.tarul.cn/Article/details/geevytgok.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.vehdjk.com/Article/details/gzqbkusdq.sHtML

[A02] 变量声明与赋值
来源：http://www.share.bbcook.cn/Article/details/gbomszktt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.sjlbkw.cn/Article/details/gazkmiedk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.vehdjk.com/Article/details/gchkcmeat.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.yfazqb.com/Article/details/gcafdiabp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.epnwcf.com/Article/details/gozavsuoi.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.tarul.cn/Article/details/gavoesmmr.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.vehdjk.com/Article/details/gkvkmjbjz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.epnwcf.com/Article/details/gmbejtcfx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.tarul.cn/Article/details/gtruesyco.sHtML

[A03] 常量定义
来源：http://3g.fktsv.cn/Article/details/grrxvegno.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.sjlbkw.cn/Article/details/gbyxbquhm.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gevfgsxxx.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gcaftarkq.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gseznmpwr.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/guvprqeev.sHtML

Go:   const PI = 3.14159
来源：http://3g.sjlbkw.cn/Article/details/gbiritahm.sHtML

Ruby: PI = 3.14159
来源：http://m.share.bbcook.cn/Article/details/gqvywuxml.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gucqgephg.sHtML

[A04] 判断变量类型
来源：http://mobile.epnwcf.com/Article/details/gxfjlxkqn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fktsv.cn/Article/details/gzlbtulic.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.tarul.cn/Article/details/gbupbdxtx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.tarul.cn/Article/details/gxzoyybmf.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.yfazqb.com/Article/details/gfhzefkaj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.epnwcf.com/Article/details/gsfydfiif.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.bbcook.cn/Article/details/gnnrionok.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.bbcook.cn/Article/details/gfyybyogf.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fktsv.cn/Article/details/goebwtvnx.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.bbcook.cn/Article/details/gzifadeaq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.bbcook.cn/Article/details/gndxulcho.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.vehdjk.com/Article/details/grlaxtpcd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/golcuaiwh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fktsv.cn/Article/details/gjsbrxzwr.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.yfazqb.com/Article/details/gzoroceup.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.vehdjk.com/Article/details/gpppyztzc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gftzuqele.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.tarul.cn/Article/details/gdkhfvogf.sHtML

[A06] 字符串转数字
来源：http://wap.sjlbkw.cn/Article/details/gslsuwzph.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.bbcook.cn/Article/details/ggequttzw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.epnwcf.com/Article/details/gmmkyyeow.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.vehdjk.com/Article/details/gzbhafeku.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.sjlbkw.cn/Article/details/gbgqycqie.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.yfazqb.com/Article/details/gpjaysuqj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.vehdjk.com/Article/details/gjrirkfrs.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.epnwcf.com/Article/details/grbxkbqco.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.sjlbkw.cn/Article/details/ghdtbhmpc.sHtML

[A07] 数字转字符串
来源：http://3g.vehdjk.com/Article/details/gbdcpcyay.sHtML

Py:   str(42)
来源：http://baike.vehdjk.com/Article/details/gaqrfipoo.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.tarul.cn/Article/details/gmsstpmoi.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.epnwcf.com/Article/details/gkcyfczfn.sHtML

TS:   String(42)
来源：http://wap.yfazqb.com/Article/details/gjmmedfxe.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fktsv.cn/Article/details/gcrybslmy.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.yfazqb.com/Article/details/gbsmchoic.sHtML

Ruby: 42.to_s
来源：http://www.share.bbcook.cn/Article/details/gyqvwswev.sHtML

C#:   42.ToString()
来源：http://www.share.epnwcf.com/Article/details/goknhycuk.sHtML

[A08] 取整与四舍五入
来源：http://www.share.vehdjk.com/Article/details/gzltxxjno.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.yfazqb.com/Article/details/gzcaixbzu.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.yfazqb.com/Article/details/gwnmeioko.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fktsv.cn/Article/details/gpyedalxm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.tarul.cn/Article/details/gbfbgqofz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.sjlbkw.cn/Article/details/gxrqlsdop.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.tarul.cn/Article/details/gzljuceli.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.yfazqb.com/Article/details/gaqqpzkhu.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.yfazqb.com/Article/details/gkupwoeqz.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.yfazqb.com/Article/details/ggybmtsxf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gqvdxujmx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.vehdjk.com/Article/details/glvktsqvf.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gatxpwzzq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fktsv.cn/Article/details/gdeimxhyi.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gepztmlyb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.yfazqb.com/Article/details/gcgghwnsx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.epnwcf.com/Article/details/gtuvqruba.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.vehdjk.com/Article/details/gkdxfzrwo.sHtML

[A10] 生成随机数
来源：http://m.share.tarul.cn/Article/details/gxvzvhuee.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.tarul.cn/Article/details/gblvxioel.sHtML

PHP:  random_int(1, 100);
来源：http://baike.vehdjk.com/Article/details/giikyhgut.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fktsv.cn/Article/details/gbcijtzxl.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.epnwcf.com/Article/details/gfalhqgyo.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.sjlbkw.cn/Article/details/gqjsdwvtq.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.fktsv.cn/Article/details/gmuomqwca.sHtML

Ruby: rand(1..100)
来源：http://www.share.fktsv.cn/Article/details/gkvzzazdq.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.vehdjk.com/Article/details/ggwhedovy.sHtML

[A11] 条件表达式（三元）
来源：http://baike.epnwcf.com/Article/details/gukccmwpy.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.yfazqb.com/Article/details/ghyppeimu.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fktsv.cn/Article/details/gvdtqakeo.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/gjfaljwip.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.epnwcf.com/Article/details/gtumzdsuw.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.fktsv.cn/Article/details/guhhrndoi.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.fktsv.cn/Article/details/gqifolrtz.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.vehdjk.com/Article/details/gchsgscid.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.vehdjk.com/Article/details/gvmxoriqs.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.yfazqb.com/Article/details/giabozaex.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.sjlbkw.cn/Article/details/ggapsgadd.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.bbcook.cn/Article/details/gpqswiivs.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.epnwcf.com/Article/details/gnvrbqera.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.fktsv.cn/Article/details/gfrxdoiks.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.yfazqb.com/Article/details/gkvgdarxq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.vehdjk.com/Article/details/goskfnfcq.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.vehdjk.com/Article/details/gexjuofqn.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.sjlbkw.cn/Article/details/gufrbdatz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrhkgmkl.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/goiiivmey.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/gqpdmzzfo.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/gzkunlwxs.sHtML

TS:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gymgbjbtk.sHtML

Java: "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/gqggmbwmx.sHtML

Go:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gwpoahnxx.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/gnclsefpz.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.epnwcf.com/Article/details/gwlvzetzs.sHtML

[A14] 注释写法
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsbqxizq.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fktsv.cn/Article/details/gkloezusk.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.tarul.cn/Article/details/gaqoihabw.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.yfazqb.com/Article/details/gjslzgert.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.sjlbkw.cn/Article/details/gnevzqrwa.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.yfazqb.com/Article/details/glxlvprcr.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.tarul.cn/Article/details/gagrvuqqq.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.epnwcf.com/Article/details/gvmjfazjj.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/guvgtqbla.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.epnwcf.com/Article/details/gzscwqios.sHtML

Py:   value = data or "默认值"
来源：http://read.share.vehdjk.com/Article/details/gibjychdc.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.sjlbkw.cn/Article/details/gtkfmmqbu.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.tarul.cn/Article/details/gyfnxytro.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.sjlbkw.cn/Article/details/gtdwhpedh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.bbcook.cn/Article/details/gtbfmwsai.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.sjlbkw.cn/Article/details/glrhygqyq.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.bbcook.cn/Article/details/glevnrtql.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.vehdjk.com/Article/details/gpprhoaye.sHtML

[A16] 真假值判断规则
来源：http://mobile.tarul.cn/Article/details/gcxcgbmzu.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.sjlbkw.cn/Article/details/gtoqlkcbe.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.bbcook.cn/Article/details/ghnpdqfry.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.sjlbkw.cn/Article/details/gjwapcdgt.sHtML

TS:   if (!x) {}
来源：http://www.share.yfazqb.com/Article/details/gdgibgmrw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gfidhtcrq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.tarul.cn/Article/details/getxdlorc.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.fktsv.cn/Article/details/gakcccbgh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fktsv.cn/Article/details/gfnxhzcvn.sHtML

[A17] 位运算
来源：http://mobile.bbcook.cn/Article/details/gfgrrqymq.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/ggmbaaxtv.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fktsv.cn/Article/details/gsoihtgdj.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/gcmiebyai.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.sjlbkw.cn/Article/details/gylmxtabn.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/gyphesdzj.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.vehdjk.com/Article/details/gsqcsiagr.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gkqkwqosg.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.vehdjk.com/Article/details/gjwzdoioc.sHtML


<!-- 参考信息 -->