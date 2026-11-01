代发 wailian999

[U105] JS：节流
来源：http://read.share.bbcook.cn/Article/details/gfznsqqkp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fktsv.cn/Article/details/govywtzer.sHtML

[U106] JS：日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gjtlqyeqw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.sjlbkw.cn/Article/details/ggcuxgcjk.sHtML

[U107] JS：数字千分位
来源：http://m.share.vehdjk.com/Article/details/gnwafhnjq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.vehdjk.com/Article/details/glhzbyvfo.sHtML

[U108] JS：随机整数
来源：http://baike.sjlbkw.cn/Article/details/grkqgnjcm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.tarul.cn/Article/details/givzfnyqy.sHtML

[U109] JS：数组分组
来源：http://blog.epnwcf.com/Article/details/gnhepbazy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.bbcook.cn/Article/details/gbkwsonin.sHtML

[U110] JS：数组分块
来源：http://read.share.fktsv.cn/Article/details/grmyzydnp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fktsv.cn/Article/details/gxwdlbwuo.sHtML

[U111] JS：对象转 Map
来源：http://3g.bbcook.cn/Article/details/gczltrrub.sHtML

new Map(Object.entries(obj))
来源：http://blog.bbcook.cn/Article/details/gukvrqfct.sHtML

[U112] JS：字符串补位
来源：http://mobile.bbcook.cn/Article/details/glioybohs.sHtML

"7".padStart(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/grohypiwx.sHtML

[U113] JS：正则替换全部
来源：http://mobile.sjlbkw.cn/Article/details/gineoplpn.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gpkthfrzv.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.bbcook.cn/Article/details/gfbcclsuu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.yfazqb.com/Article/details/gmilvlonv.sHtML

[U115] JS：生成 UUID
来源：http://www.share.sjlbkw.cn/Article/details/gvemfqmvx.sHtML

crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gmptfvimj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fktsv.cn/Article/details/gpyltrdkm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.yfazqb.com/Article/details/gwlokevrf.sHtML

[U117] JS：单元测试
来源：http://3g.epnwcf.com/Article/details/gzmrdijjh.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fktsv.cn/Article/details/gqntmjppd.sHtML

[U118] JS：开发服务器
来源：http://m.share.epnwcf.com/Article/details/gscexnume.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fktsv.cn/Article/details/guvxuuito.sHtML

[U119] JS：生产构建
来源：http://m.share.epnwcf.com/Article/details/gtvhthbdz.sHtML

npx vite build
来源：http://read.share.fktsv.cn/Article/details/gjymtcmct.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.sjlbkw.cn/Article/details/garndotak.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.vehdjk.com/Article/details/ginpibvex.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/grprjvcii.sHtML

统计汇总
来源：http://www.blog.fktsv.cn/Article/details/grpndqwcp.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gtpyjzrhy.sHtML

按语言统计（条）：
来源：http://baike.sjlbkw.cn/Article/details/gntlcldau.sHtML

Python ......... 252
来源：http://www.share.tarul.cn/Article/details/ggzqaopap.sHtML

PHP ............ 252
来源：http://www.blog.bbcook.cn/Article/details/gbindomnc.sHtML

JavaScript ..... 252
来源：http://www.m.share.bbcook.cn/Article/details/gdjoiwxsa.sHtML

TypeScript ..... 212
来源：http://read.share.fktsv.cn/Article/details/gahejvcby.sHtML

Java ........... 212
来源：http://mobile.bbcook.cn/Article/details/gcsyptfha.sHtML

Go ............. 212
来源：http://mobile.epnwcf.com/Article/details/gcucqgkgr.sHtML

Ruby ........... 212
来源：http://blog.vehdjk.com/Article/details/gabjskuio.sHtML

C# ............. 212
来源：http://www.share.fktsv.cn/Article/details/gjcyqgmun.sHtML

C .............. 30
来源：http://baike.fktsv.cn/Article/details/gqyuvlyeg.sHtML

C++ ............ 30
来源：http://read.share.yfazqb.com/Article/details/gyuaofgtg.sHtML

SQL ............ 90
来源：http://mobile.epnwcf.com/Article/details/guqvbdthp.sHtML

Bash ........... 80
来源：http://read.share.vehdjk.com/Article/details/guoqoaods.sHtML

Kotlin ......... 15
来源：http://mobile.epnwcf.com/Article/details/gadopnzmb.sHtML

Swift .......... 15
来源：http://blog.bbcook.cn/Article/details/gjfbzcmja.sHtML

Lua ............ 10
来源：http://wap.epnwcf.com/Article/details/gefpklgll.sHtML

Perl ........... 10
来源：http://www.m.share.sjlbkw.cn/Article/details/gndkycesu.sHtML

Scala .......... 10
来源：http://wap.bbcook.cn/Article/details/gronddrbw.sHtML

------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gkdkzpvfr.sHtML

合计 ........... 2106 条
来源：http://mobile.yfazqb.com/Article/details/gsoszoxdc.sHtML

按章节统计：
来源：http://m.share.sjlbkw.cn/Article/details/gcoudjquw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.bbcook.cn/Article/details/gbthsbjdt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.vehdjk.com/Article/details/gsxdrlptq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.epnwcf.com/Article/details/gskwiofid.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.vehdjk.com/Article/details/gpcayvrvc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.tarul.cn/Article/details/grkdwicgv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.yfazqb.com/Article/details/gmczvuilq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.epnwcf.com/Article/details/gsggbcdig.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.bbcook.cn/Article/details/gvuekwlzg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gwqmfsoyc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fktsv.cn/Article/details/geoxpliff.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.bbcook.cn/Article/details/glzquypuv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/gjcimjkgc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.tarul.cn/Article/details/gmsxhaggd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.sjlbkw.cn/Article/details/gszzgotsd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.tarul.cn/Article/details/giveegvkm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gwjpqqihl.sHtML

Q SQL 专题                              90
来源：http://www.blog.epnwcf.com/Article/details/gydlakqpp.sHtML

R Bash 专题                             80
来源：http://blog.yfazqb.com/Article/details/gicyjzkdc.sHtML

S C / C++ 专题                          60
来源：http://www.share.sjlbkw.cn/Article/details/gjcwmopco.sHtML

T 其他语言补充                          60
来源：http://m.share.bbcook.cn/Article/details/gtmcsgeuv.sHtML

U 高频实用片段                         120
来源：http://3g.yfazqb.com/Article/details/gwdxcosuj.sHtML

------------------------------------
来源：http://www.blog.tarul.cn/Article/details/gjjayjkug.sHtML

合计                                  2106 条
来源：http://read.share.bbcook.cn/Article/details/geiocnoud.sHtML

--------------------------------------------------------------------------------
来源：http://wap.yfazqb.com/Article/details/grcnmmpwq.sHtML

使用提醒
来源：http://baike.fktsv.cn/Article/details/gghqdkpsl.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gwuyxzxkt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.vehdjk.com/Article/details/gqohpvzlk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.vehdjk.com/Article/details/grpekfyxq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.tarul.cn/Article/details/gqngaokju.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.sjlbkw.cn/Article/details/guxdjenyp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.tarul.cn/Article/details/gmqtgqaee.sHtML

—— 文件结束 ——
来源：http://www.m.share.vehdjk.com/Article/details/gkersmvmt.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ghzvacgyl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.tarul.cn/Article/details/gwfilutkv.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.vehdjk.com/Article/details/gsasvzlxb.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gypglafyl.sHtML

【收录内容】
来源：http://wap.bbcook.cn/Article/details/gtuhvqmrx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.bbcook.cn/Article/details/gknfxrplk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.sjlbkw.cn/Article/details/gxbnqnjje.sHtML

SQL · Bash · C · C++
来源：http://baike.fktsv.cn/Article/details/gystbazez.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.yfazqb.com/Article/details/geegiwaqo.sHtML

【使用说明】
来源：http://read.share.tarul.cn/Article/details/gxnzffjeg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.bbcook.cn/Article/details/guepegisi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.tarul.cn/Article/details/gnabftcrj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fktsv.cn/Article/details/gnnpszuea.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.bbcook.cn/Article/details/gmrcvuzes.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.bbcook.cn/Article/details/gllyjdssl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.yfazqb.com/Article/details/gypidsuhr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.epnwcf.com/Article/details/gnaukrkkz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.sjlbkw.cn/Article/details/gtybawehb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.vehdjk.com/Article/details/gmsftofim.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.epnwcf.com/Article/details/gnwsmwrzh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.bbcook.cn/Article/details/gitnsxlgt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.tarul.cn/Article/details/gymyptzbb.sHtML

【文件统计】
来源：http://m.share.bbcook.cn/Article/details/gmxlmnery.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fktsv.cn/Article/details/gvbmzvieh.sHtML

--------------------------------------------------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gnpzjcxkm.sHtML

目  录
来源：http://blog.epnwcf.com/Article/details/gsdzdlnyj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gsckdemyz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.epnwcf.com/Article/details/glehtvhwe.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.epnwcf.com/Article/details/gunvgtaiq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.vehdjk.com/Article/details/gvsjtglsq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.vehdjk.com/Article/details/gonbgjzxq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.tarul.cn/Article/details/gjzsrabwd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.sjlbkw.cn/Article/details/gjfbquhva.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.bbcook.cn/Article/details/gzqgakuvy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.tarul.cn/Article/details/gsdofrfal.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gmbfccrzy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.yfazqb.com/Article/details/gzsfgabds.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/gttnhwpyd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/gnxcwkmip.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/gxpxgrxjn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gsojnhrdq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fktsv.cn/Article/details/glomibpvb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.bbcook.cn/Article/details/gfkfrowku.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.epnwcf.com/Article/details/gfphuzgvn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.bbcook.cn/Article/details/gtgovshbv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.vehdjk.com/Article/details/gfxfofflr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.tarul.cn/Article/details/gpmnfapzp.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.tarul.cn/Article/details/gfhvjwkzx.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gnszenzra.sHtML

A. 基础语法与类型
来源：http://m.share.fktsv.cn/Article/details/gvvmbtocr.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gfkspjbpx.sHtML

[A01] Hello World
来源：http://wap.tarul.cn/Article/details/godvfjaxt.sHtML

Py:   print("Hello, World!")
来源：http://3g.tarul.cn/Article/details/gtvntbskk.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.yfazqb.com/Article/details/gagebilho.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.bbcook.cn/Article/details/gphqlfxin.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fktsv.cn/Article/details/giruiitjm.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.epnwcf.com/Article/details/gfqwiodpz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.tarul.cn/Article/details/gdlyhbkxj.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.sjlbkw.cn/Article/details/gtsuuynwi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.vehdjk.com/Article/details/gxqqwumds.sHtML

[A02] 变量声明与赋值
来源：http://blog.tarul.cn/Article/details/gomvtskfs.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.tarul.cn/Article/details/gtzekrynw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.yfazqb.com/Article/details/gzjunpohd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.yfazqb.com/Article/details/grxnybtbs.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.yfazqb.com/Article/details/gteardxek.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fktsv.cn/Article/details/gyjgrdfzb.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fktsv.cn/Article/details/gzyycztqt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.fktsv.cn/Article/details/gqnmojhzi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.tarul.cn/Article/details/gbwwuzlqn.sHtML

[A03] 常量定义
来源：http://wap.epnwcf.com/Article/details/gelgndyzk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fktsv.cn/Article/details/gyymvhomb.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gbkegqwrh.sHtML

JS:   const PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gkqfkapkp.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/ghiwdxjwd.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gzkurfpmu.sHtML

Go:   const PI = 3.14159
来源：http://wap.fktsv.cn/Article/details/gnkivnqms.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fktsv.cn/Article/details/glhboqgrl.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gxlfzfygw.sHtML

[A04] 判断变量类型
来源：http://3g.vehdjk.com/Article/details/gabhsyqbw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.vehdjk.com/Article/details/gvjdpcsrz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.tarul.cn/Article/details/gpgakjrho.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.yfazqb.com/Article/details/gqaqubpep.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.yfazqb.com/Article/details/gmgfqzzrv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.bbcook.cn/Article/details/gbylprdcv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.bbcook.cn/Article/details/gfxrgfvyl.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fktsv.cn/Article/details/geggtagfh.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fktsv.cn/Article/details/gcbrdiaen.sHtML

[A05] 整数除法与取模
来源：http://www.share.yfazqb.com/Article/details/gszicocrr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.bbcook.cn/Article/details/gbqaexsio.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.tarul.cn/Article/details/gagvvuhta.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gjxxeeolj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fktsv.cn/Article/details/ghomjqtgv.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/ggxokhgzb.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.bbcook.cn/Article/details/gsghrhcze.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gpeaqnskv.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.epnwcf.com/Article/details/gdrbelkfe.sHtML

[A06] 字符串转数字
来源：http://www.share.bbcook.cn/Article/details/gfiyzkmnr.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.bbcook.cn/Article/details/gbvlnknxs.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fktsv.cn/Article/details/gehkfjdxn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.vehdjk.com/Article/details/ggcayyabm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.tarul.cn/Article/details/gzaynnpnh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.yfazqb.com/Article/details/gxydkopqw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.sjlbkw.cn/Article/details/gmdsdakbu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.yfazqb.com/Article/details/goqgqasop.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.vehdjk.com/Article/details/gfcwhvcyo.sHtML

[A07] 数字转字符串
来源：http://mobile.tarul.cn/Article/details/ggwrurrio.sHtML

Py:   str(42)
来源：http://www.share.yfazqb.com/Article/details/gfbtsrwqt.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.bbcook.cn/Article/details/gertipqle.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.epnwcf.com/Article/details/gsupfjjyd.sHtML

TS:   String(42)
来源：http://read.share.epnwcf.com/Article/details/gnwmfqotu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.vehdjk.com/Article/details/gzcthszzx.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.epnwcf.com/Article/details/gtsxuiakt.sHtML

Ruby: 42.to_s
来源：http://mobile.epnwcf.com/Article/details/gvrrpxjbu.sHtML

C#:   42.ToString()
来源：http://read.share.sjlbkw.cn/Article/details/gixpryrfk.sHtML

[A08] 取整与四舍五入
来源：http://wap.epnwcf.com/Article/details/gxczbfmxn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.yfazqb.com/Article/details/gcoeyesdb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.bbcook.cn/Article/details/gzwvkncws.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.vehdjk.com/Article/details/gbcmsncpv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.epnwcf.com/Article/details/gyfesbrvp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/gijrjijhj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.tarul.cn/Article/details/gikgubuhq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.epnwcf.com/Article/details/glkfwezqf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.sjlbkw.cn/Article/details/gdgetsolk.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fktsv.cn/Article/details/grstspyxf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gtdlodlda.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fktsv.cn/Article/details/grjzsjsop.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.epnwcf.com/Article/details/gguhtrgqt.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gssdifhsc.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gbmzryllo.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fktsv.cn/Article/details/gnsxkytjv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.epnwcf.com/Article/details/gbjbmhcxx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.epnwcf.com/Article/details/gxbsenlet.sHtML

[A10] 生成随机数
来源：http://www.blog.epnwcf.com/Article/details/gjcfdsilo.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.vehdjk.com/Article/details/gwwpwvxcx.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.vehdjk.com/Article/details/ghojmbuao.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fktsv.cn/Article/details/grqqxxvlg.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.epnwcf.com/Article/details/ggeqgovck.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.bbcook.cn/Article/details/gjblwsfcz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.sjlbkw.cn/Article/details/gdyanfgnw.sHtML

Ruby: rand(1..100)
来源：http://mobile.fktsv.cn/Article/details/gaozibweu.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.fktsv.cn/Article/details/gnfukhhyh.sHtML

[A11] 条件表达式（三元）
来源：http://wap.yfazqb.com/Article/details/glhozdzlp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.epnwcf.com/Article/details/grmpaajrm.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.fktsv.cn/Article/details/gfvclxymv.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.bbcook.cn/Article/details/guwwohfit.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.vehdjk.com/Article/details/gpqjhgata.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fktsv.cn/Article/details/gukgvxvow.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.epnwcf.com/Article/details/gkjrbwixg.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.bbcook.cn/Article/details/gaahibgcn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.sjlbkw.cn/Article/details/gesapcuom.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.epnwcf.com/Article/details/gqfxkmbuy.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.sjlbkw.cn/Article/details/guknrahho.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.bbcook.cn/Article/details/gjfnsjnwk.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.yfazqb.com/Article/details/giltnlnab.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.vehdjk.com/Article/details/gdjagwplp.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.vehdjk.com/Article/details/grlcqajab.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.sjlbkw.cn/Article/details/gxcilaobs.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.vehdjk.com/Article/details/gdkhepzpa.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.vehdjk.com/Article/details/gkxlsacbi.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.epnwcf.com/Article/details/gpjvnvhen.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gsuxnompd.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.tarul.cn/Article/details/gftfsbpaw.sHtML

JS:   "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gnwtrfbrp.sHtML

TS:   "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gahtbkoqu.sHtML

Java: "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gxjtxdutd.sHtML

Go:   "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/gsdysnvyq.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gcnbebakx.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gbkgoqfdv.sHtML

[A14] 注释写法
来源：http://www.m.share.yfazqb.com/Article/details/gkcxbddbs.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.vehdjk.com/Article/details/gutowhyil.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.bbcook.cn/Article/details/gzfhdcjjm.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.bbcook.cn/Article/details/gbzamsnlh.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.bbcook.cn/Article/details/gvmtljwjq.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.fktsv.cn/Article/details/gbttwpfds.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/gffvmwzwo.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.sjlbkw.cn/Article/details/gfraxlgea.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/glxvngwya.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.fktsv.cn/Article/details/ghutsgltz.sHtML

Py:   value = data or "默认值"
来源：http://read.share.epnwcf.com/Article/details/grkorlazt.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fktsv.cn/Article/details/guorxirnz.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.epnwcf.com/Article/details/gtsxhfqct.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.sjlbkw.cn/Article/details/gfyhxlngn.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.tarul.cn/Article/details/gyoadprom.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.vehdjk.com/Article/details/gjiijdclr.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.yfazqb.com/Article/details/gcsqobrtf.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.tarul.cn/Article/details/gviiwpbil.sHtML

[A16] 真假值判断规则
来源：http://read.share.epnwcf.com/Article/details/gjpdqugzu.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.epnwcf.com/Article/details/gurldcaom.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.bbcook.cn/Article/details/gsdxdhndc.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.fktsv.cn/Article/details/gyrxdopoo.sHtML

TS:   if (!x) {}
来源：http://baike.vehdjk.com/Article/details/gezlipnro.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.epnwcf.com/Article/details/gugaoxttz.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.sjlbkw.cn/Article/details/gonowcznr.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.tarul.cn/Article/details/gacvhmchf.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.fktsv.cn/Article/details/gqnycmgrj.sHtML

[A17] 位运算
来源：http://www.share.vehdjk.com/Article/details/gbfrjrxzf.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gyxgbrgee.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gsmqhujxe.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gzwpqawsy.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.sjlbkw.cn/Article/details/gnjqoxzvs.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.epnwcf.com/Article/details/gfphwbave.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.tarul.cn/Article/details/gbahpirnn.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/geejjeoos.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/gorrrznzk.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.fktsv.cn/Article/details/gxcubrxiv.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.vehdjk.com/Article/details/gvvbywrqv.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.bbcook.cn/Article/details/gyahxhrdl.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.sjlbkw.cn/Article/details/gdrtnrhiz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.sjlbkw.cn/Article/details/grndkceed.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.vehdjk.com/Article/details/gqtftdxbs.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.fktsv.cn/Article/details/gcvrdcqnr.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.fktsv.cn/Article/details/grakpqpcs.sHtML


<!-- 参考信息 -->