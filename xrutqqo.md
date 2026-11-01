代发 wailian999

[U105] JS：节流
来源：http://www.blog.vehdjk.com/Article/details/gysnlseuh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.epnwcf.com/Article/details/gdwvxkkse.sHtML

[U106] JS：日期格式化
来源：http://3g.tarul.cn/Article/details/gbywiezoc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.bbcook.cn/Article/details/gtjhslzjc.sHtML

[U107] JS：数字千分位
来源：http://3g.yfazqb.com/Article/details/gajmbeclg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gnxojvuyr.sHtML

[U108] JS：随机整数
来源：http://read.share.epnwcf.com/Article/details/gmbmumjqi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fktsv.cn/Article/details/gcaekxmgw.sHtML

[U109] JS：数组分组
来源：http://m.share.fktsv.cn/Article/details/gssqeoszd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fktsv.cn/Article/details/gytnjsjpx.sHtML

[U110] JS：数组分块
来源：http://mobile.tarul.cn/Article/details/gubiffagy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.vehdjk.com/Article/details/gfkobksez.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.tarul.cn/Article/details/gqdeiewfh.sHtML

new Map(Object.entries(obj))
来源：http://3g.fktsv.cn/Article/details/gtadsplol.sHtML

[U112] JS：字符串补位
来源：http://wap.bbcook.cn/Article/details/gpdeyevox.sHtML

"7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/ghwmiqvtc.sHtML

[U113] JS：正则替换全部
来源：http://blog.bbcook.cn/Article/details/gcguugbcl.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gjkeumhhb.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.tarul.cn/Article/details/gnsfyuudc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.sjlbkw.cn/Article/details/gqbqqbjvj.sHtML

[U115] JS：生成 UUID
来源：http://read.share.epnwcf.com/Article/details/gweudtumt.sHtML

crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gkjyqouqe.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.vehdjk.com/Article/details/gbtkappyo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.bbcook.cn/Article/details/gfwuwtvkl.sHtML

[U117] JS：单元测试
来源：http://m.share.yfazqb.com/Article/details/ghrixzlku.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.epnwcf.com/Article/details/gdjbalxth.sHtML

[U118] JS：开发服务器
来源：http://www.blog.bbcook.cn/Article/details/gqulrbrzb.sHtML

npm i -D vite;  npx vite
来源：http://3g.bbcook.cn/Article/details/guxhftmks.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fktsv.cn/Article/details/gyfdkgfuy.sHtML

npx vite build
来源：http://3g.fktsv.cn/Article/details/gndxqjnzo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.epnwcf.com/Article/details/ggmlvcqpj.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.vehdjk.com/Article/details/gbaljbbzw.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gwqlglhjw.sHtML

统计汇总
来源：http://blog.bbcook.cn/Article/details/ggphatzuk.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/grehygkon.sHtML

按语言统计（条）：
来源：http://www.m.share.sjlbkw.cn/Article/details/giogxjckk.sHtML

Python ......... 252
来源：http://mobile.epnwcf.com/Article/details/gyzzacbfx.sHtML

PHP ............ 252
来源：http://blog.sjlbkw.cn/Article/details/gwkdaicmk.sHtML

JavaScript ..... 252
来源：http://mobile.bbcook.cn/Article/details/gyekjwqnm.sHtML

TypeScript ..... 212
来源：http://baike.epnwcf.com/Article/details/gsrehcqdq.sHtML

Java ........... 212
来源：http://www.m.share.yfazqb.com/Article/details/gghewenhu.sHtML

Go ............. 212
来源：http://mobile.bbcook.cn/Article/details/glttxnhwp.sHtML

Ruby ........... 212
来源：http://www.share.bbcook.cn/Article/details/gtesswzsb.sHtML

C# ............. 212
来源：http://m.share.tarul.cn/Article/details/gqieywote.sHtML

C .............. 30
来源：http://www.share.epnwcf.com/Article/details/guubmirgs.sHtML

C++ ............ 30
来源：http://3g.fktsv.cn/Article/details/gnavjpzti.sHtML

SQL ............ 90
来源：http://www.share.yfazqb.com/Article/details/gacnvcnvi.sHtML

Bash ........... 80
来源：http://wap.yfazqb.com/Article/details/gnhzdkxqx.sHtML

Kotlin ......... 15
来源：http://blog.epnwcf.com/Article/details/gxgsactch.sHtML

Swift .......... 15
来源：http://blog.bbcook.cn/Article/details/gommtcsuy.sHtML

Lua ............ 10
来源：http://mobile.bbcook.cn/Article/details/gqffdfxxe.sHtML

Perl ........... 10
来源：http://www.m.share.epnwcf.com/Article/details/guncwoncw.sHtML

Scala .......... 10
来源：http://read.share.bbcook.cn/Article/details/gcrokbmrv.sHtML

------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/ghmlpfhls.sHtML

合计 ........... 2106 条
来源：http://mobile.vehdjk.com/Article/details/gycyhrsqj.sHtML

按章节统计：
来源：http://read.share.tarul.cn/Article/details/goenanksg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.sjlbkw.cn/Article/details/gcfguiwgi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.tarul.cn/Article/details/gqseqwfwz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.vehdjk.com/Article/details/gnrvmmcmm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.sjlbkw.cn/Article/details/gpgpfldeg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fktsv.cn/Article/details/gxxgswakd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.yfazqb.com/Article/details/glrqvldtj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/gqsxtigcw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.epnwcf.com/Article/details/gaginqnvs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/gwxtwrvgk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.epnwcf.com/Article/details/gaurwxaqn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gppodyvsm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gthrotqdo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gfeydxdjc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.tarul.cn/Article/details/gtcabfkxg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.sjlbkw.cn/Article/details/ghilduoqo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gppkvwicd.sHtML

Q SQL 专题                              90
来源：http://m.share.epnwcf.com/Article/details/ghtiawcto.sHtML

R Bash 专题                             80
来源：http://www.blog.epnwcf.com/Article/details/gfqjumuac.sHtML

S C / C++ 专题                          60
来源：http://m.share.vehdjk.com/Article/details/gsljqqdqr.sHtML

T 其他语言补充                          60
来源：http://www.share.sjlbkw.cn/Article/details/gibcanriw.sHtML

U 高频实用片段                         120
来源：http://read.share.sjlbkw.cn/Article/details/gyvyhhodh.sHtML

------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gildasfae.sHtML

合计                                  2106 条
来源：http://mobile.yfazqb.com/Article/details/grtizrumj.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/gjdopkxzy.sHtML

使用提醒
来源：http://wap.vehdjk.com/Article/details/gnkiewert.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.tarul.cn/Article/details/gdlxrqojn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.bbcook.cn/Article/details/gnrwyatja.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fktsv.cn/Article/details/ghdxmkjia.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.bbcook.cn/Article/details/gsfichkni.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.sjlbkw.cn/Article/details/gznznhtjo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.yfazqb.com/Article/details/gmmpbgeln.sHtML

—— 文件结束 ——
来源：http://3g.fktsv.cn/Article/details/gpddpxfwy.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gxnhsxpaz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.epnwcf.com/Article/details/gtigjsbom.sHtML

Common Programming Examples Cheat Book
来源：http://3g.yfazqb.com/Article/details/gvchcumpg.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gjkfgwoge.sHtML

【收录内容】
来源：http://www.m.share.sjlbkw.cn/Article/details/giynreqxb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.yfazqb.com/Article/details/gkwazkgbn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.tarul.cn/Article/details/gtapqbmzx.sHtML

SQL · Bash · C · C++
来源：http://3g.sjlbkw.cn/Article/details/ggtkwhrid.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.yfazqb.com/Article/details/gqawaxrje.sHtML

【使用说明】
来源：http://www.blog.epnwcf.com/Article/details/ghzcvnsch.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.bbcook.cn/Article/details/glrbsdpwf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.tarul.cn/Article/details/gfporsjfh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fktsv.cn/Article/details/gjbfbodgc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.yfazqb.com/Article/details/gtdoqarew.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.vehdjk.com/Article/details/gexnlhwji.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyqgoips.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.vehdjk.com/Article/details/gmqigpmnz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.tarul.cn/Article/details/gzluuwzsc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.tarul.cn/Article/details/gcngcsews.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.sjlbkw.cn/Article/details/gbnrsbmzg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.epnwcf.com/Article/details/ghudtdair.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.yfazqb.com/Article/details/gmajwuhdw.sHtML

【文件统计】
来源：http://3g.yfazqb.com/Article/details/ghccispdu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.vehdjk.com/Article/details/gemtprhos.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gweogbgjv.sHtML

目  录
来源：http://blog.epnwcf.com/Article/details/geneeyzxe.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/gzdvtoftq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.bbcook.cn/Article/details/gmfgoopcl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.bbcook.cn/Article/details/gwvhmtlii.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.vehdjk.com/Article/details/gxqlqxzhg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.bbcook.cn/Article/details/gaxiuupha.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.yfazqb.com/Article/details/gjgioostk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fktsv.cn/Article/details/gycuvqmda.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.epnwcf.com/Article/details/gkunykdzy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.sjlbkw.cn/Article/details/glilduodp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.tarul.cn/Article/details/gxspuhren.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.sjlbkw.cn/Article/details/gsumjvlwm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gbvblgrqo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/gojuxvyiv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gnasnncnk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.bbcook.cn/Article/details/gvarhjhyr.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.tarul.cn/Article/details/gikaiwags.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.vehdjk.com/Article/details/gjgdkvnzg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.bbcook.cn/Article/details/gkzackxqn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.sjlbkw.cn/Article/details/gijncelkf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.epnwcf.com/Article/details/gycrunsmj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.vehdjk.com/Article/details/geqeamfqv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.tarul.cn/Article/details/geoyuofhc.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gbhehvlzc.sHtML

A. 基础语法与类型
来源：http://mobile.vehdjk.com/Article/details/gnkbfouha.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/goptnetlm.sHtML

[A01] Hello World
来源：http://read.share.epnwcf.com/Article/details/gttvyvpmz.sHtML

Py:   print("Hello, World!")
来源：http://m.share.vehdjk.com/Article/details/gsteklouq.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.tarul.cn/Article/details/ggldliytl.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fktsv.cn/Article/details/gztuvzwwy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.tarul.cn/Article/details/gvemqzpxl.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.epnwcf.com/Article/details/gmeachihm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.sjlbkw.cn/Article/details/gpltkakwt.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.yfazqb.com/Article/details/gqavkatja.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.tarul.cn/Article/details/godaykxkv.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fktsv.cn/Article/details/ggqjpvfbh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fktsv.cn/Article/details/gyqsiznvp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.sjlbkw.cn/Article/details/golknvdoh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gfmmzpkkt.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fktsv.cn/Article/details/glsglmkpx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fktsv.cn/Article/details/gnfgoimsc.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.yfazqb.com/Article/details/gfwxnhoiw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.epnwcf.com/Article/details/gtmapzbjq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.yfazqb.com/Article/details/gfbioswwr.sHtML

[A03] 常量定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gocjqtphu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.vehdjk.com/Article/details/gnhgtqisi.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/glsrtemmo.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/guiqnwjci.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gangmzhzm.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/grkuvjobd.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fktsv.cn/Article/details/gongmfcsr.sHtML

Ruby: PI = 3.14159
来源：http://blog.fktsv.cn/Article/details/gbyfvkqhg.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/goheocmqm.sHtML

[A04] 判断变量类型
来源：http://mobile.sjlbkw.cn/Article/details/gyborsliv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.yfazqb.com/Article/details/gkerjnref.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.vehdjk.com/Article/details/gwvuureoo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.tarul.cn/Article/details/ghdiauvgu.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.bbcook.cn/Article/details/gyfzfxdon.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.bbcook.cn/Article/details/gevuozjik.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.tarul.cn/Article/details/gkszwkroc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.tarul.cn/Article/details/gzjsrembj.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fktsv.cn/Article/details/gczjoihow.sHtML

[A05] 整数除法与取模
来源：http://www.share.sjlbkw.cn/Article/details/gsijakzpr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fktsv.cn/Article/details/grfgjuxuo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gjvgkdlqn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/gfpprwrml.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fktsv.cn/Article/details/gvfwtpjpe.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.tarul.cn/Article/details/gxgdvojdr.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.vehdjk.com/Article/details/ggehcgozy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.bbcook.cn/Article/details/gnjvxfihz.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.tarul.cn/Article/details/gymrcwqzh.sHtML

[A06] 字符串转数字
来源：http://www.share.epnwcf.com/Article/details/golzqpnzb.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.yfazqb.com/Article/details/gfsvakwwf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.yfazqb.com/Article/details/gfaklxwai.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.tarul.cn/Article/details/gwqqqieha.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fktsv.cn/Article/details/getdefpjx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.vehdjk.com/Article/details/gmynccdes.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.fktsv.cn/Article/details/gviysjlcs.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fktsv.cn/Article/details/giaycntup.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.epnwcf.com/Article/details/gkrgjtcsr.sHtML

[A07] 数字转字符串
来源：http://www.blog.yfazqb.com/Article/details/gncznvvnx.sHtML

Py:   str(42)
来源：http://3g.yfazqb.com/Article/details/glckymczq.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fktsv.cn/Article/details/gmrwoledn.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.vehdjk.com/Article/details/gyrcvinqe.sHtML

TS:   String(42)
来源：http://www.share.bbcook.cn/Article/details/gdfbextwc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.fktsv.cn/Article/details/gmbpizmdc.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.bbcook.cn/Article/details/gkmjrguoo.sHtML

Ruby: 42.to_s
来源：http://3g.fktsv.cn/Article/details/gndyjltsc.sHtML

C#:   42.ToString()
来源：http://3g.fktsv.cn/Article/details/gwouvuxhj.sHtML

[A08] 取整与四舍五入
来源：http://m.share.yfazqb.com/Article/details/gduoglsry.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/gvvmsurft.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fktsv.cn/Article/details/gbwejeczg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.bbcook.cn/Article/details/gwbyrqhag.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.yfazqb.com/Article/details/gydcypdmg.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.bbcook.cn/Article/details/gvxwjhgpm.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.yfazqb.com/Article/details/gzekavwau.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.bbcook.cn/Article/details/gnopvfitl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.tarul.cn/Article/details/goenndbqs.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.epnwcf.com/Article/details/gsrafdepm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.epnwcf.com/Article/details/gvqddimep.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.yfazqb.com/Article/details/gpmxrdbyx.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gqmjwcxgq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.vehdjk.com/Article/details/gitvbmxqt.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.yfazqb.com/Article/details/grqodfsbv.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.bbcook.cn/Article/details/gbgrxoqra.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.yfazqb.com/Article/details/galntcrsu.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gdvcmatbb.sHtML

[A10] 生成随机数
来源：http://wap.epnwcf.com/Article/details/gjgxymnqb.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.bbcook.cn/Article/details/gyppveail.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fktsv.cn/Article/details/gvwdzyryp.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.vehdjk.com/Article/details/gupxblxrc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.bbcook.cn/Article/details/gloddknpo.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.bbcook.cn/Article/details/ggkxszvxy.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.vehdjk.com/Article/details/gocjlhuoa.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.vehdjk.com/Article/details/gjvtpqrjs.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.vehdjk.com/Article/details/grxirafac.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.epnwcf.com/Article/details/grxxfvedc.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.fktsv.cn/Article/details/gyfklebul.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fktsv.cn/Article/details/gbwloucsm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.fktsv.cn/Article/details/gklclyomz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.fktsv.cn/Article/details/gvehnpwic.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.bbcook.cn/Article/details/ggoqyhhab.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.vehdjk.com/Article/details/gkogqxiyx.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.epnwcf.com/Article/details/gasjhwwzo.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.vehdjk.com/Article/details/gxaxfvvxr.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.vehdjk.com/Article/details/gqkjbqsvm.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fktsv.cn/Article/details/giptgtpwd.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.vehdjk.com/Article/details/gddaattlj.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.sjlbkw.cn/Article/details/gpcelplkh.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.yfazqb.com/Article/details/gjwoouevy.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.tarul.cn/Article/details/gchzakfvn.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.fktsv.cn/Article/details/grfczaagh.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.bbcook.cn/Article/details/gxjficifv.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.tarul.cn/Article/details/gshdloisi.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.fktsv.cn/Article/details/gbmtzgjvk.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/glcywhvqy.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/gmwspwtag.sHtML

JS:   "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/gvequmzjf.sHtML

TS:   "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gglpibhcg.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/gvfzmjtxz.sHtML

Go:   "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gjpsohajf.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gzzkhicnf.sHtML

C#:   "第一行\n第二行"
来源：http://baike.tarul.cn/Article/details/gwglueoab.sHtML

[A14] 注释写法
来源：http://www.share.bbcook.cn/Article/details/gcffugdko.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.sjlbkw.cn/Article/details/gorgmgrxv.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.vehdjk.com/Article/details/grplazxco.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.sjlbkw.cn/Article/details/gubhrvxyp.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.tarul.cn/Article/details/gphspnmdh.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.yfazqb.com/Article/details/gzycybura.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.yfazqb.com/Article/details/gfcpdckxe.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.bbcook.cn/Article/details/grgoategi.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.yfazqb.com/Article/details/glpxcfmuy.sHtML

[A15] 空值判断与默认值
来源：http://read.share.tarul.cn/Article/details/glfvyieqq.sHtML

Py:   value = data or "默认值"
来源：http://www.share.epnwcf.com/Article/details/gewapsbhj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.epnwcf.com/Article/details/gwhfplwtx.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.vehdjk.com/Article/details/gyjsvkbpo.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.sjlbkw.cn/Article/details/gcejevhlk.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.tarul.cn/Article/details/gturxwwqp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpeijvxx.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.bbcook.cn/Article/details/gyccisxtx.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.tarul.cn/Article/details/gztefykrs.sHtML

[A16] 真假值判断规则
来源：http://mobile.tarul.cn/Article/details/guindwjsy.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.epnwcf.com/Article/details/gpjjyukjy.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.sjlbkw.cn/Article/details/gquxsyzig.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.sjlbkw.cn/Article/details/gjeiujbtp.sHtML

TS:   if (!x) {}
来源：http://www.blog.vehdjk.com/Article/details/glwcsricm.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.sjlbkw.cn/Article/details/gmkafjlzc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.vehdjk.com/Article/details/gyzpdmgrn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.fktsv.cn/Article/details/gqnahahqb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.epnwcf.com/Article/details/gvmzrnvcu.sHtML

[A17] 位运算
来源：http://baike.yfazqb.com/Article/details/gyjkydssl.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/giwvuyxck.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/gexsgmduy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gjytwehvp.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/ggjbmwvls.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gjkvmjykx.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/gckcvlycv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.yfazqb.com/Article/details/gbdktnvtq.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.bbcook.cn/Article/details/gzkyokqlb.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.vehdjk.com/Article/details/gzjpymtyq.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.bbcook.cn/Article/details/goaonvojv.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.fktsv.cn/Article/details/grigtgbzn.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.sjlbkw.cn/Article/details/gjlcaklwl.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fktsv.cn/Article/details/guladrrht.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.tarul.cn/Article/details/gpjwshbrm.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.epnwcf.com/Article/details/gjbkbavle.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.fktsv.cn/Article/details/ginrolfpa.sHtML


<!-- 参考信息 -->