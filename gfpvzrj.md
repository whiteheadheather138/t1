代发 wailian999

[U105] JS：节流
来源：http://3g.tarul.cn/Article/details/gmqfehwav.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.tarul.cn/Article/details/goqobosbn.sHtML

[U106] JS：日期格式化
来源：http://baike.tarul.cn/Article/details/grfagonms.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.sjlbkw.cn/Article/details/ghgvwlycr.sHtML

[U107] JS：数字千分位
来源：http://mobile.yfazqb.com/Article/details/gembldnmz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.epnwcf.com/Article/details/grmmkbzul.sHtML

[U108] JS：随机整数
来源：http://mobile.fktsv.cn/Article/details/gsemnjwha.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.bbcook.cn/Article/details/gjqvqrfqe.sHtML

[U109] JS：数组分组
来源：http://wap.sjlbkw.cn/Article/details/ggsjrhrvp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.epnwcf.com/Article/details/glqblvpxt.sHtML

[U110] JS：数组分块
来源：http://baike.tarul.cn/Article/details/gmcpdlfnz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.tarul.cn/Article/details/gzivhkknv.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/guwgyahbt.sHtML

new Map(Object.entries(obj))
来源：http://blog.tarul.cn/Article/details/grjbphomo.sHtML

[U112] JS：字符串补位
来源：http://blog.epnwcf.com/Article/details/guscglmtc.sHtML

"7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gbrsyblmp.sHtML

[U113] JS：正则替换全部
来源：http://blog.vehdjk.com/Article/details/genanofvy.sHtML

s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gvnaqmlxs.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.vehdjk.com/Article/details/glhwgymeg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.yfazqb.com/Article/details/ggosxouek.sHtML

[U115] JS：生成 UUID
来源：http://www.share.sjlbkw.cn/Article/details/ginevjnoh.sHtML

crypto.randomUUID()
来源：http://www.blog.tarul.cn/Article/details/ggmjqqijl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.bbcook.cn/Article/details/grvncfcjb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.epnwcf.com/Article/details/geydtlzeq.sHtML

[U117] JS：单元测试
来源：http://read.share.epnwcf.com/Article/details/gytrvsckn.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.sjlbkw.cn/Article/details/gffavlpkl.sHtML

[U118] JS：开发服务器
来源：http://3g.tarul.cn/Article/details/gdvhwdulj.sHtML

npm i -D vite;  npx vite
来源：http://read.share.vehdjk.com/Article/details/glyibrpnp.sHtML

[U119] JS：生产构建
来源：http://www.blog.bbcook.cn/Article/details/gzvxgjefm.sHtML

npx vite build
来源：http://3g.yfazqb.com/Article/details/gkjyynnnq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.tarul.cn/Article/details/gmuhgnyaa.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.vehdjk.com/Article/details/gsqqxlqje.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gpuqbcben.sHtML

统计汇总
来源：http://baike.vehdjk.com/Article/details/gdrwyafrh.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ghaattgda.sHtML

按语言统计（条）：
来源：http://blog.epnwcf.com/Article/details/gixrrxfiv.sHtML

Python ......... 252
来源：http://wap.fktsv.cn/Article/details/gnyuijmmv.sHtML

PHP ............ 252
来源：http://blog.bbcook.cn/Article/details/gkstiodjr.sHtML

JavaScript ..... 252
来源：http://www.blog.sjlbkw.cn/Article/details/gggrzaens.sHtML

TypeScript ..... 212
来源：http://www.share.tarul.cn/Article/details/gmxofggib.sHtML

Java ........... 212
来源：http://wap.fktsv.cn/Article/details/ggoittkzy.sHtML

Go ............. 212
来源：http://3g.epnwcf.com/Article/details/gfoysilxf.sHtML

Ruby ........... 212
来源：http://www.share.tarul.cn/Article/details/grvypufwk.sHtML

C# ............. 212
来源：http://3g.yfazqb.com/Article/details/gdkdobrlg.sHtML

C .............. 30
来源：http://www.blog.yfazqb.com/Article/details/gqockfvtk.sHtML

C++ ............ 30
来源：http://www.m.share.bbcook.cn/Article/details/gkzhdlipm.sHtML

SQL ............ 90
来源：http://m.share.fktsv.cn/Article/details/gmvhqgdkh.sHtML

Bash ........... 80
来源：http://m.share.fktsv.cn/Article/details/gyyhohazo.sHtML

Kotlin ......... 15
来源：http://www.blog.fktsv.cn/Article/details/gaxrjncva.sHtML

Swift .......... 15
来源：http://www.share.sjlbkw.cn/Article/details/gcdblabag.sHtML

Lua ............ 10
来源：http://blog.vehdjk.com/Article/details/gqlcctplt.sHtML

Perl ........... 10
来源：http://m.share.sjlbkw.cn/Article/details/gbymdxwqn.sHtML

Scala .......... 10
来源：http://baike.tarul.cn/Article/details/goyclkqos.sHtML

------------------------------------
来源：http://read.share.tarul.cn/Article/details/gvkglsmjd.sHtML

合计 ........... 2106 条
来源：http://wap.bbcook.cn/Article/details/gwwlqpglm.sHtML

按章节统计：
来源：http://www.blog.yfazqb.com/Article/details/gnlxsyqgl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.bbcook.cn/Article/details/gknlhhmtj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.yfazqb.com/Article/details/gphzvmazy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.sjlbkw.cn/Article/details/gckytekik.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.vehdjk.com/Article/details/gyyuuxzvp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.tarul.cn/Article/details/gyuulzpzv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.tarul.cn/Article/details/glzwgqbmv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.tarul.cn/Article/details/grgrvdfma.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.bbcook.cn/Article/details/gbnfhmlhd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gieihzfzo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.yfazqb.com/Article/details/gaufwmbjk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/geypaptlb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gmwkvogfe.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/gccygwlvi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.vehdjk.com/Article/details/gjcsoctgl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.yfazqb.com/Article/details/gamhluknl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/gbyifshng.sHtML

Q SQL 专题                              90
来源：http://www.m.share.bbcook.cn/Article/details/gcfueqwgz.sHtML

R Bash 专题                             80
来源：http://www.share.tarul.cn/Article/details/gmqweacde.sHtML

S C / C++ 专题                          60
来源：http://www.share.sjlbkw.cn/Article/details/gmfvfaamm.sHtML

T 其他语言补充                          60
来源：http://www.share.sjlbkw.cn/Article/details/gsfeczpei.sHtML

U 高频实用片段                         120
来源：http://blog.bbcook.cn/Article/details/gpqwhmwip.sHtML

------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gitkmazgg.sHtML

合计                                  2106 条
来源：http://blog.fktsv.cn/Article/details/ghinfequm.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fktsv.cn/Article/details/gocviykhf.sHtML

使用提醒
来源：http://mobile.tarul.cn/Article/details/gfurseuzu.sHtML

--------------------------------------------------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gjvmysifr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.sjlbkw.cn/Article/details/gfpfqoaoq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.sjlbkw.cn/Article/details/gvcmeiwaw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.yfazqb.com/Article/details/gninbuozc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.yfazqb.com/Article/details/ggyllicjq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.sjlbkw.cn/Article/details/gywucmqpp.sHtML

—— 文件结束 ——
来源：http://mobile.vehdjk.com/Article/details/gmoegvquu.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmtywygzi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.sjlbkw.cn/Article/details/gychgyvii.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.vehdjk.com/Article/details/gnbdnrtzv.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gkntimmtj.sHtML

【收录内容】
来源：http://www.share.tarul.cn/Article/details/gyaaxjvdc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.sjlbkw.cn/Article/details/graaymumi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.yfazqb.com/Article/details/gdexpozfh.sHtML

SQL · Bash · C · C++
来源：http://blog.sjlbkw.cn/Article/details/gkaucgbvx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.bbcook.cn/Article/details/gphdwubfd.sHtML

【使用说明】
来源：http://mobile.yfazqb.com/Article/details/gkiafzmho.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.tarul.cn/Article/details/gzzntpkxg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.sjlbkw.cn/Article/details/givkibhfz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fktsv.cn/Article/details/guawzkeku.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.yfazqb.com/Article/details/gvhoxhzzq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.bbcook.cn/Article/details/gitekvwsf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.yfazqb.com/Article/details/gpcwppdob.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.bbcook.cn/Article/details/gutotyloq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fktsv.cn/Article/details/gbryyyost.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.tarul.cn/Article/details/gvzcpcvio.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.bbcook.cn/Article/details/gpbbihmrv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.tarul.cn/Article/details/gjsntdebr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.tarul.cn/Article/details/gmhsfgfbc.sHtML

【文件统计】
来源：http://www.share.vehdjk.com/Article/details/gshcljufh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fktsv.cn/Article/details/ghlbdxnuo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gjxjxotsm.sHtML

目  录
来源：http://www.blog.yfazqb.com/Article/details/grmpgsxqa.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.epnwcf.com/Article/details/gzsafdhdz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.epnwcf.com/Article/details/gywetumpx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.vehdjk.com/Article/details/glqufkokd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.yfazqb.com/Article/details/gpwmajofw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gsetlxboz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.yfazqb.com/Article/details/grvguhahl.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.tarul.cn/Article/details/gktlumdes.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.bbcook.cn/Article/details/gdfdjilec.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.sjlbkw.cn/Article/details/gclptqalg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/gkxiqlphy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.epnwcf.com/Article/details/ghrnhlmqq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/gilqhzhws.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/gtrertcoh.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fktsv.cn/Article/details/gbyzhmisp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fktsv.cn/Article/details/gvfecubrf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/geermglia.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gezgmotft.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.yfazqb.com/Article/details/gomvctrbf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.yfazqb.com/Article/details/gpxjqunji.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.yfazqb.com/Article/details/gynrlctgk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.bbcook.cn/Article/details/gxelytmfm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.bbcook.cn/Article/details/glmlofhbq.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gnnxxdcqk.sHtML

A. 基础语法与类型
来源：http://www.m.share.fktsv.cn/Article/details/gnzkxyvrl.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gfxvartid.sHtML

[A01] Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gpptwjikg.sHtML

Py:   print("Hello, World!")
来源：http://wap.yfazqb.com/Article/details/gfolvjqwi.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.tarul.cn/Article/details/gjtfhnmne.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.vehdjk.com/Article/details/gmllxkzgz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.vehdjk.com/Article/details/gysyfxwam.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.tarul.cn/Article/details/glxrhxpjj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.bbcook.cn/Article/details/gqvupnenf.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fktsv.cn/Article/details/gpjqtjsue.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.bbcook.cn/Article/details/gtaptwubj.sHtML

[A02] 变量声明与赋值
来源：http://m.share.bbcook.cn/Article/details/gahipidnb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fktsv.cn/Article/details/goirisxgq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.vehdjk.com/Article/details/gqzdxhuzo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fktsv.cn/Article/details/gnqhzhwkj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.tarul.cn/Article/details/gcaaluged.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.tarul.cn/Article/details/gnniencyg.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fktsv.cn/Article/details/gzdvpchjj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fktsv.cn/Article/details/gsckfesfo.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.bbcook.cn/Article/details/gikgrdhei.sHtML

[A03] 常量定义
来源：http://www.m.share.epnwcf.com/Article/details/gjvvvwnwv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.tarul.cn/Article/details/gvohvbpml.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gidjcmqbm.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzugejwuy.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gdbfflkxv.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gcsdnrpft.sHtML

Go:   const PI = 3.14159
来源：http://read.share.yfazqb.com/Article/details/gxmwkzkyu.sHtML

Ruby: PI = 3.14159
来源：http://www.share.bbcook.cn/Article/details/gwommkfhp.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gdguhcaby.sHtML

[A04] 判断变量类型
来源：http://www.m.share.vehdjk.com/Article/details/gwrcqtmtg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.tarul.cn/Article/details/gorikmppb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.sjlbkw.cn/Article/details/gigpidbvh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fktsv.cn/Article/details/gvsvziuof.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.epnwcf.com/Article/details/grzmstytb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.vehdjk.com/Article/details/ghiwtmdjk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.vehdjk.com/Article/details/gmbtuzgud.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.epnwcf.com/Article/details/gyioqvxuv.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fktsv.cn/Article/details/gotmgwpia.sHtML

[A05] 整数除法与取模
来源：http://read.share.tarul.cn/Article/details/gswyfuirn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.yfazqb.com/Article/details/gzbfcmpmi.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.tarul.cn/Article/details/gqzmmrxhk.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gxjcukskm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.yfazqb.com/Article/details/gywjywwxv.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gjbqyjdwb.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.vehdjk.com/Article/details/giuavdgli.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.vehdjk.com/Article/details/gkarmkzys.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/glktoavso.sHtML

[A06] 字符串转数字
来源：http://read.share.bbcook.cn/Article/details/gnrjpewfq.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.sjlbkw.cn/Article/details/gswtjexqo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.sjlbkw.cn/Article/details/ghruwllsc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.epnwcf.com/Article/details/gxwskauwt.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fktsv.cn/Article/details/gjeyfhdrm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.epnwcf.com/Article/details/grzgesnom.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.epnwcf.com/Article/details/gvqmfnkfr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fktsv.cn/Article/details/gyynkyktd.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.bbcook.cn/Article/details/gqiaffmgc.sHtML

[A07] 数字转字符串
来源：http://mobile.bbcook.cn/Article/details/gylftwmyq.sHtML

Py:   str(42)
来源：http://blog.fktsv.cn/Article/details/gkmtmhouo.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.sjlbkw.cn/Article/details/gcmtqvkiv.sHtML

JS:   String(42); (42).toString()
来源：http://baike.vehdjk.com/Article/details/gxfzpcziu.sHtML

TS:   String(42)
来源：http://3g.tarul.cn/Article/details/gudvgcoqp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.vehdjk.com/Article/details/geuxaapno.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.yfazqb.com/Article/details/gqytpnpfw.sHtML

Ruby: 42.to_s
来源：http://mobile.epnwcf.com/Article/details/gpstfwzlx.sHtML

C#:   42.ToString()
来源：http://baike.vehdjk.com/Article/details/gxtfjyxcz.sHtML

[A08] 取整与四舍五入
来源：http://wap.fktsv.cn/Article/details/gxewrxsnb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.bbcook.cn/Article/details/ggumtlasv.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.fktsv.cn/Article/details/ghqsvfuej.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.tarul.cn/Article/details/gskjkykoj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.epnwcf.com/Article/details/gfftxzyqh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.epnwcf.com/Article/details/gqyvnelsq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.fktsv.cn/Article/details/ggtbwsnum.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.epnwcf.com/Article/details/gpnwqcryh.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.yfazqb.com/Article/details/ggddbfkzj.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.epnwcf.com/Article/details/ghcxuhlrs.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.yfazqb.com/Article/details/grpivwqis.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.tarul.cn/Article/details/gvrrabfax.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.fktsv.cn/Article/details/gfgihcobr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.vehdjk.com/Article/details/geqlxesuu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.tarul.cn/Article/details/gcmtvimxu.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.yfazqb.com/Article/details/gcyzpabwn.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.yfazqb.com/Article/details/gtmwvmopo.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.fktsv.cn/Article/details/gsuryeggj.sHtML

[A10] 生成随机数
来源：http://mobile.yfazqb.com/Article/details/godvthswi.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.yfazqb.com/Article/details/gqgxacbxd.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.bbcook.cn/Article/details/gihvbwltc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.epnwcf.com/Article/details/gkmidaybb.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.yfazqb.com/Article/details/gmtlgtssh.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.yfazqb.com/Article/details/glufhslyq.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.bbcook.cn/Article/details/gditgdlnl.sHtML

Ruby: rand(1..100)
来源：http://read.share.yfazqb.com/Article/details/gzfzjujaq.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.yfazqb.com/Article/details/giiefkztn.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.fktsv.cn/Article/details/gunmbltrj.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.yfazqb.com/Article/details/ghhvosfhs.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fktsv.cn/Article/details/glieokkjb.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.tarul.cn/Article/details/gqkhyeofa.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.epnwcf.com/Article/details/gmhlhqasx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.bbcook.cn/Article/details/gbbpuleyz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.sjlbkw.cn/Article/details/glekftttm.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.tarul.cn/Article/details/gxphxlvvz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.epnwcf.com/Article/details/gsibksumb.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fktsv.cn/Article/details/guzaoring.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.sjlbkw.cn/Article/details/guomqafqf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fktsv.cn/Article/details/gqmfaqtdg.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.bbcook.cn/Article/details/gujjrpoam.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.epnwcf.com/Article/details/gkmyxywdi.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.tarul.cn/Article/details/gelcfdbfb.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.tarul.cn/Article/details/gsmrjsnpl.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.yfazqb.com/Article/details/gkpjfnvaw.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.epnwcf.com/Article/details/gutjioykd.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.sjlbkw.cn/Article/details/gfgxrvqch.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/gkokqxajb.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/gcpjejpob.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/gmnepuboq.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/gjxemkagr.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/gvvuhdlxv.sHtML

Go:   "第一行\n第二行"
来源：http://wap.yfazqb.com/Article/details/gkwdeztpv.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/gjjssgltd.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/gdcowqfnd.sHtML

[A14] 注释写法
来源：http://wap.sjlbkw.cn/Article/details/gnzssjqdj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.tarul.cn/Article/details/gvunztiqn.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.epnwcf.com/Article/details/gmylonopw.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.vehdjk.com/Article/details/gsyyldykv.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/gbqjoxnse.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.bbcook.cn/Article/details/gubyjwgxk.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.epnwcf.com/Article/details/gvljseekz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.vehdjk.com/Article/details/gganrwhvl.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gipbqqqkm.sHtML

[A15] 空值判断与默认值
来源：http://wap.tarul.cn/Article/details/gineflcez.sHtML

Py:   value = data or "默认值"
来源：http://wap.epnwcf.com/Article/details/gyvpivqgl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.vehdjk.com/Article/details/giubeuqkm.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.sjlbkw.cn/Article/details/gwedhwczu.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.sjlbkw.cn/Article/details/grmngbjjq.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.vehdjk.com/Article/details/gukjohejk.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.tarul.cn/Article/details/goagogfxy.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.epnwcf.com/Article/details/gidwtvpdq.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.vehdjk.com/Article/details/gffxxtkdu.sHtML

[A16] 真假值判断规则
来源：http://www.share.bbcook.cn/Article/details/genbtjzix.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.tarul.cn/Article/details/gqkzrjjyq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.sjlbkw.cn/Article/details/givtalotl.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.vehdjk.com/Article/details/geabsqcos.sHtML

TS:   if (!x) {}
来源：http://www.share.tarul.cn/Article/details/giimctify.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.tarul.cn/Article/details/glcgnnzbu.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.fktsv.cn/Article/details/gbpdxgdsw.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.bbcook.cn/Article/details/gpwzagvlh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gymcljjmr.sHtML

[A17] 位运算
来源：http://read.share.sjlbkw.cn/Article/details/gpmchuzgn.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.bbcook.cn/Article/details/gsunapkmk.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fktsv.cn/Article/details/guvgwoglx.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.bbcook.cn/Article/details/gemtivagl.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/gtdryqnur.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/gvshzhuhv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gqmsixart.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/gcdojphpo.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gpzjypynz.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.sjlbkw.cn/Article/details/ggpyocjtv.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.sjlbkw.cn/Article/details/gxwhgvrct.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.sjlbkw.cn/Article/details/glkcbyrvm.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fktsv.cn/Article/details/gwjomoqrn.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.sjlbkw.cn/Article/details/giupiuwui.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.fktsv.cn/Article/details/gurgngxdu.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.fktsv.cn/Article/details/gshaczewj.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.bbcook.cn/Article/details/gvcsnhjdp.sHtML


<!-- 参考信息 -->