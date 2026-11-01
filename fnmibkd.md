代发 wailian999

[U103] JS：定时器
来源：http://blog.sjlbkw.cn/Article/details/gtiqtsyxj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.yfazqb.com/Article/details/ghvjywxme.sHtML

[U104] JS：防抖
来源：http://baike.yfazqb.com/Article/details/ghucujuph.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fktsv.cn/Article/details/gtekoxfzb.sHtML

[U105] JS：节流
来源：http://www.blog.bbcook.cn/Article/details/gjqvvzrsa.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.yfazqb.com/Article/details/gsudaxrre.sHtML

[U106] JS：日期格式化
来源：http://wap.tarul.cn/Article/details/gghxsviwe.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.yfazqb.com/Article/details/gwoovhrfm.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.bbcook.cn/Article/details/gkxcorfqo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.bbcook.cn/Article/details/gxsrjphdu.sHtML

[U108] JS：随机整数
来源：http://www.share.fktsv.cn/Article/details/gobxdlyat.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fktsv.cn/Article/details/gjktckxpy.sHtML

[U109] JS：数组分组
来源：http://baike.yfazqb.com/Article/details/grnkzuapr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.bbcook.cn/Article/details/gacaklpbs.sHtML

[U110] JS：数组分块
来源：http://read.share.epnwcf.com/Article/details/gjxiuzqqb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.vehdjk.com/Article/details/ghxbjhytz.sHtML

[U111] JS：对象转 Map
来源：http://wap.vehdjk.com/Article/details/gcvfnidwn.sHtML

new Map(Object.entries(obj))
来源：http://www.share.bbcook.cn/Article/details/gkyfudljf.sHtML

[U112] JS：字符串补位
来源：http://www.blog.epnwcf.com/Article/details/gijsifklg.sHtML

"7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gvhqzhoue.sHtML

[U113] JS：正则替换全部
来源：http://www.share.vehdjk.com/Article/details/gutbiogsv.sHtML

s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gxobqepdj.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.bbcook.cn/Article/details/gkjopeddt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fktsv.cn/Article/details/gvbufytyt.sHtML

[U115] JS：生成 UUID
来源：http://mobile.yfazqb.com/Article/details/gvygyyknm.sHtML

crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/glbbsaxlg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.epnwcf.com/Article/details/goyaphyec.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.yfazqb.com/Article/details/gqsyhwwsb.sHtML

[U117] JS：单元测试
来源：http://www.blog.tarul.cn/Article/details/gywahpaxi.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.tarul.cn/Article/details/gojiejxiy.sHtML

[U118] JS：开发服务器
来源：http://3g.sjlbkw.cn/Article/details/gtggoxzpz.sHtML

npm i -D vite;  npx vite
来源：http://baike.fktsv.cn/Article/details/gxywehakv.sHtML

[U119] JS：生产构建
来源：http://baike.sjlbkw.cn/Article/details/ggndwmzll.sHtML

npx vite build
来源：http://read.share.tarul.cn/Article/details/gtebcllot.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.sjlbkw.cn/Article/details/gpyxwwbrf.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.bbcook.cn/Article/details/gczlyiyjd.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gaseczojy.sHtML

统计汇总
来源：http://wap.yfazqb.com/Article/details/gsrgyvimh.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gzazckvdi.sHtML

按语言统计（条）：
来源：http://www.blog.sjlbkw.cn/Article/details/gqcjucjng.sHtML

Python ......... 252
来源：http://www.share.epnwcf.com/Article/details/gpdxmhxbt.sHtML

PHP ............ 252
来源：http://www.share.yfazqb.com/Article/details/gvibowgrk.sHtML

JavaScript ..... 252
来源：http://www.share.yfazqb.com/Article/details/gegiqlttr.sHtML

TypeScript ..... 212
来源：http://read.share.sjlbkw.cn/Article/details/gzndlloja.sHtML

Java ........... 212
来源：http://m.share.vehdjk.com/Article/details/guypcsakw.sHtML

Go ............. 212
来源：http://wap.fktsv.cn/Article/details/glpatojnj.sHtML

Ruby ........... 212
来源：http://wap.vehdjk.com/Article/details/gwcxxiwjd.sHtML

C# ............. 212
来源：http://blog.sjlbkw.cn/Article/details/gcbreqxul.sHtML

C .............. 30
来源：http://wap.tarul.cn/Article/details/gqvigsheg.sHtML

C++ ............ 30
来源：http://3g.yfazqb.com/Article/details/gzfrncozs.sHtML

SQL ............ 90
来源：http://mobile.tarul.cn/Article/details/gznrdywvw.sHtML

Bash ........... 80
来源：http://mobile.fktsv.cn/Article/details/gtjjbupjg.sHtML

Kotlin ......... 15
来源：http://www.blog.tarul.cn/Article/details/gpupwkpjd.sHtML

Swift .......... 15
来源：http://mobile.sjlbkw.cn/Article/details/ggirtxlyz.sHtML

Lua ............ 10
来源：http://3g.vehdjk.com/Article/details/gmxrndmaz.sHtML

Perl ........... 10
来源：http://www.share.sjlbkw.cn/Article/details/gbkqqreeb.sHtML

Scala .......... 10
来源：http://blog.epnwcf.com/Article/details/gbjasccng.sHtML

------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gabosxvdk.sHtML

合计 ........... 2106 条
来源：http://m.share.bbcook.cn/Article/details/gvezcioiy.sHtML

按章节统计：
来源：http://m.share.fktsv.cn/Article/details/gvxnfrnjh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.epnwcf.com/Article/details/grokafilw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.yfazqb.com/Article/details/gmjcbfntn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.yfazqb.com/Article/details/groplebyw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.vehdjk.com/Article/details/gcgaevbdr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.vehdjk.com/Article/details/gcdbcsvay.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fktsv.cn/Article/details/gmpxwtses.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.vehdjk.com/Article/details/gkhwjgsnu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.vehdjk.com/Article/details/gsnahfscw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/gznyhucsk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.tarul.cn/Article/details/gxmaajsbk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gcitxrwut.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gshnkmhzi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/goynbfhng.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fktsv.cn/Article/details/gpdopyouc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.bbcook.cn/Article/details/gwzbvbric.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/ggvbdqnrd.sHtML

Q SQL 专题                              90
来源：http://blog.tarul.cn/Article/details/gvurxhdqy.sHtML

R Bash 专题                             80
来源：http://mobile.fktsv.cn/Article/details/gucwsvuhz.sHtML

S C / C++ 专题                          60
来源：http://mobile.vehdjk.com/Article/details/goacwocqg.sHtML

T 其他语言补充                          60
来源：http://wap.bbcook.cn/Article/details/gyghbmvbq.sHtML

U 高频实用片段                         120
来源：http://3g.yfazqb.com/Article/details/gejpenkjl.sHtML

------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gnwccgjkc.sHtML

合计                                  2106 条
来源：http://wap.sjlbkw.cn/Article/details/gjbddoban.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/ggmdokdgx.sHtML

使用提醒
来源：http://www.blog.tarul.cn/Article/details/gmhjhdjhw.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gphuwrpce.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.sjlbkw.cn/Article/details/gpltjffnm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.vehdjk.com/Article/details/gkdirplgi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.tarul.cn/Article/details/gzsrbliac.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.vehdjk.com/Article/details/gobqhwtdl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.yfazqb.com/Article/details/gmnyiotmo.sHtML

—— 文件结束 ——
来源：http://www.blog.vehdjk.com/Article/details/ggzasqelo.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ggezildho.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.yfazqb.com/Article/details/gbbjkscqy.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fktsv.cn/Article/details/gvuqmwxve.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gxcszqrzd.sHtML

【收录内容】
来源：http://3g.bbcook.cn/Article/details/gegbsxiop.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.vehdjk.com/Article/details/gcqxkerph.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fktsv.cn/Article/details/gzoksjobn.sHtML

SQL · Bash · C · C++
来源：http://baike.vehdjk.com/Article/details/glunmusyg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.bbcook.cn/Article/details/gdtplwmzd.sHtML

【使用说明】
来源：http://wap.epnwcf.com/Article/details/gmtbdklwx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.epnwcf.com/Article/details/gnjjhbltc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.vehdjk.com/Article/details/gkhesmkek.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.sjlbkw.cn/Article/details/gtcpibuqr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.sjlbkw.cn/Article/details/gzmnnzyyl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fktsv.cn/Article/details/giqcuieet.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.sjlbkw.cn/Article/details/gvugyldyj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.bbcook.cn/Article/details/grveaskdl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fktsv.cn/Article/details/gnwhdyvly.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.vehdjk.com/Article/details/glptsmhfe.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.sjlbkw.cn/Article/details/grdwjjknw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fktsv.cn/Article/details/gobszgudm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fktsv.cn/Article/details/ggbjhubfq.sHtML

【文件统计】
来源：http://mobile.fktsv.cn/Article/details/gygucwmvz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.epnwcf.com/Article/details/gjnugpplz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.epnwcf.com/Article/details/gnxcefapx.sHtML

目  录
来源：http://www.m.share.vehdjk.com/Article/details/giqruzrtf.sHtML

--------------------------------------------------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gboxridri.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.tarul.cn/Article/details/gtpslgjko.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fktsv.cn/Article/details/gzybzdbij.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fktsv.cn/Article/details/gvytudeem.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwxbcodn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.sjlbkw.cn/Article/details/gnmmyffxz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.vehdjk.com/Article/details/gbexhwxcr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fktsv.cn/Article/details/gispfscad.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fktsv.cn/Article/details/gdfmqdkty.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fktsv.cn/Article/details/gvewrlkfr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.yfazqb.com/Article/details/geuevgikn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gxzzooepp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.vehdjk.com/Article/details/gaizorord.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/gtoioeaai.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.bbcook.cn/Article/details/gatzqobpe.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gaacnmjip.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.bbcook.cn/Article/details/ggoxbtuku.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.tarul.cn/Article/details/gzfmklnxf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.bbcook.cn/Article/details/gjmungclx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fktsv.cn/Article/details/gsgdrcefl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.yfazqb.com/Article/details/gkpxxxetk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.vehdjk.com/Article/details/guzvmcuws.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/grfaleaak.sHtML

A. 基础语法与类型
来源：http://blog.epnwcf.com/Article/details/gsuszozrw.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gwhfpclnv.sHtML

[A01] Hello World
来源：http://www.blog.fktsv.cn/Article/details/gzlwnusmh.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.vehdjk.com/Article/details/giikazppb.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.bbcook.cn/Article/details/gxarsgbwg.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.epnwcf.com/Article/details/gqjdqcdwd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.epnwcf.com/Article/details/grvrcrnwt.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.epnwcf.com/Article/details/godhjdlzb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.tarul.cn/Article/details/gyazrljwu.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.tarul.cn/Article/details/gzeefvdqw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.sjlbkw.cn/Article/details/gfywccfaf.sHtML

[A02] 变量声明与赋值
来源：http://read.share.epnwcf.com/Article/details/gespgdgeu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.sjlbkw.cn/Article/details/gboftfgrv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.tarul.cn/Article/details/gmhjxewmr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.bbcook.cn/Article/details/gknubwznr.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.vehdjk.com/Article/details/grensvggf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.vehdjk.com/Article/details/gmkaqaelp.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.yfazqb.com/Article/details/gqmejvmow.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.tarul.cn/Article/details/gxeyusils.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.yfazqb.com/Article/details/gxjgoqhcp.sHtML

[A03] 常量定义
来源：http://www.share.tarul.cn/Article/details/gcrfbkeft.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.sjlbkw.cn/Article/details/gjvitusby.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gdqwfqylp.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gzbnaznsf.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gciskitsa.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/ggytmlxep.sHtML

Go:   const PI = 3.14159
来源：http://read.share.sjlbkw.cn/Article/details/gxwumtpxc.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fktsv.cn/Article/details/gllfjoxjb.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gokycndhs.sHtML

[A04] 判断变量类型
来源：http://www.blog.vehdjk.com/Article/details/gwovrphqw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.bbcook.cn/Article/details/glcdwesih.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.tarul.cn/Article/details/gbgxostan.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.yfazqb.com/Article/details/gfnxyxwuq.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.sjlbkw.cn/Article/details/golsjvkgy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.tarul.cn/Article/details/gtwfydqwg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhmnayis.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.epnwcf.com/Article/details/gkljftqkr.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.sjlbkw.cn/Article/details/gwghxygla.sHtML

[A05] 整数除法与取模
来源：http://3g.sjlbkw.cn/Article/details/gyaoliflk.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.bbcook.cn/Article/details/gddjbcpnq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/gfhowsvtv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gimkgzpqy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.yfazqb.com/Article/details/gsvgnsqfy.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gujqvikat.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fktsv.cn/Article/details/getumcydd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/ggrimrjob.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fktsv.cn/Article/details/gxzeiifgk.sHtML

[A06] 字符串转数字
来源：http://www.blog.vehdjk.com/Article/details/gtzhupijv.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.tarul.cn/Article/details/gtldzaotk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.yfazqb.com/Article/details/ggkikiarz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.fktsv.cn/Article/details/glytpohbk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.epnwcf.com/Article/details/gifsepphx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.tarul.cn/Article/details/ghrewbepf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fktsv.cn/Article/details/gqhanwtvu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.sjlbkw.cn/Article/details/gucifbjnw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.bbcook.cn/Article/details/gcwevmbwx.sHtML

[A07] 数字转字符串
来源：http://m.share.fktsv.cn/Article/details/ggwpralan.sHtML

Py:   str(42)
来源：http://wap.yfazqb.com/Article/details/glbhbepwj.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.vehdjk.com/Article/details/grpeutxta.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.vehdjk.com/Article/details/gbwjptywm.sHtML

TS:   String(42)
来源：http://mobile.fktsv.cn/Article/details/gsaosvxvk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.sjlbkw.cn/Article/details/gpjpbunil.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.tarul.cn/Article/details/grtwudnqj.sHtML

Ruby: 42.to_s
来源：http://www.blog.bbcook.cn/Article/details/gelodzzbw.sHtML

C#:   42.ToString()
来源：http://www.blog.tarul.cn/Article/details/glbnphbhg.sHtML

[A08] 取整与四舍五入
来源：http://wap.yfazqb.com/Article/details/gcdpjcmhu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fktsv.cn/Article/details/guiouooxk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.vehdjk.com/Article/details/ggyyqhhje.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.bbcook.cn/Article/details/gloihmfhx.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.sjlbkw.cn/Article/details/gozalcanb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.sjlbkw.cn/Article/details/gavtldaps.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.sjlbkw.cn/Article/details/ghnvztjow.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.bbcook.cn/Article/details/gmuzgipjj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.vehdjk.com/Article/details/goukkhubr.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.tarul.cn/Article/details/gtokdpwvs.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gsubmalrq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.yfazqb.com/Article/details/gyiokvfgs.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gghdyinho.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gtzzldwic.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gaoitzbef.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.vehdjk.com/Article/details/gdqcwjugl.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.epnwcf.com/Article/details/gnvyrxxmp.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gmslazovc.sHtML

[A10] 生成随机数
来源：http://read.share.tarul.cn/Article/details/ggiwghvag.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.bbcook.cn/Article/details/gozcqvqbm.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.bbcook.cn/Article/details/gknsgfzii.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.epnwcf.com/Article/details/gbqfqjyha.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.yfazqb.com/Article/details/gdqufoptf.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.fktsv.cn/Article/details/gtfwpcdms.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.yfazqb.com/Article/details/gomeqwepg.sHtML

Ruby: rand(1..100)
来源：http://www.share.fktsv.cn/Article/details/gtmwjocyb.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.bbcook.cn/Article/details/grrvpsnlx.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.tarul.cn/Article/details/gcsmtcayt.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.tarul.cn/Article/details/gxdhraoji.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.epnwcf.com/Article/details/gxlxwsyvq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.bbcook.cn/Article/details/gutuwskzt.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.vehdjk.com/Article/details/gtnnwvcck.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.yfazqb.com/Article/details/gndtzxtlz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.bbcook.cn/Article/details/glxivcggs.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.yfazqb.com/Article/details/gmrwarruj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.epnwcf.com/Article/details/gezwoqway.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.bbcook.cn/Article/details/gxlkcqlky.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.epnwcf.com/Article/details/girshgmtv.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.yfazqb.com/Article/details/gpytojwbs.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.sjlbkw.cn/Article/details/gljvyghpl.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.tarul.cn/Article/details/gcrvboqze.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.sjlbkw.cn/Article/details/gugwcuock.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.sjlbkw.cn/Article/details/gsyvyijqe.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.sjlbkw.cn/Article/details/gvchbjyup.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fktsv.cn/Article/details/gzizwqvut.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.bbcook.cn/Article/details/gzdhapnqw.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gliguanee.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlkgbqip.sHtML

JS:   "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/ghwbdeiva.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/ggtivmoyf.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fktsv.cn/Article/details/guijiexqi.sHtML

Go:   "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/glifkwxia.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/gpednprbo.sHtML

C#:   "第一行\n第二行"
来源：http://wap.yfazqb.com/Article/details/gtpqyuvil.sHtML

[A14] 注释写法
来源：http://3g.yfazqb.com/Article/details/goubirlmm.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.yfazqb.com/Article/details/gvqwhszyt.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.sjlbkw.cn/Article/details/gngmvqcoo.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.epnwcf.com/Article/details/goqvtrlzj.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.bbcook.cn/Article/details/gasxsrnxj.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.epnwcf.com/Article/details/gnlerkvnn.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.epnwcf.com/Article/details/ggbeoupmp.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.epnwcf.com/Article/details/guglptzvv.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.epnwcf.com/Article/details/giqahxruj.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.yfazqb.com/Article/details/grzajaqpb.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.epnwcf.com/Article/details/gvvrvdbbr.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.yfazqb.com/Article/details/gbsluavxw.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.bbcook.cn/Article/details/gzbosieat.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.fktsv.cn/Article/details/gvpmmyovo.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpilmghkj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.epnwcf.com/Article/details/gqfmxjoos.sHtML

Ruby: value = data || "默认值"
来源：http://blog.tarul.cn/Article/details/gwjtheqgr.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.tarul.cn/Article/details/gcuvlgwkx.sHtML

[A16] 真假值判断规则
来源：http://www.blog.yfazqb.com/Article/details/gxgyhouqi.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.epnwcf.com/Article/details/ghorcsxtd.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.epnwcf.com/Article/details/gemwtryul.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.bbcook.cn/Article/details/gxfwedhhw.sHtML

TS:   if (!x) {}
来源：http://www.blog.vehdjk.com/Article/details/gnzhtlvue.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.yfazqb.com/Article/details/gxkzdqgil.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.epnwcf.com/Article/details/gnqrdjsau.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.yfazqb.com/Article/details/gfhgwpjds.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.sjlbkw.cn/Article/details/gcbokroim.sHtML

[A17] 位运算
来源：http://www.m.share.epnwcf.com/Article/details/gnhttbnql.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/glgkbnwpf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.yfazqb.com/Article/details/grlyivsts.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/geiobhftv.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/geliutmwo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/gtbypsztp.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.yfazqb.com/Article/details/gszeomsvw.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.bbcook.cn/Article/details/gigirbufr.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/gmjhggnnp.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.tarul.cn/Article/details/gsxfwpgtd.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.bbcook.cn/Article/details/gxxebybkg.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.fktsv.cn/Article/details/gikbmffqw.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.tarul.cn/Article/details/gtjgkyrql.sHtML


<!-- 参考信息 -->