代发 wailian999

[U103] JS：定时器
来源：http://www.share.vehdjk.com/Article/details/gembzpylf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.yfazqb.com/Article/details/grrdflung.sHtML

[U104] JS：防抖
来源：http://baike.epnwcf.com/Article/details/gsitdusmy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.epnwcf.com/Article/details/ghrzhijtm.sHtML

[U105] JS：节流
来源：http://m.share.yfazqb.com/Article/details/gxgvocxxg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.sjlbkw.cn/Article/details/gjorjbgwc.sHtML

[U106] JS：日期格式化
来源：http://baike.vehdjk.com/Article/details/gdgjakvub.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.sjlbkw.cn/Article/details/gatgcekic.sHtML

[U107] JS：数字千分位
来源：http://www.share.epnwcf.com/Article/details/gdbduhkrp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gvyixonhk.sHtML

[U108] JS：随机整数
来源：http://blog.epnwcf.com/Article/details/gtzahruco.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.yfazqb.com/Article/details/gnkvarodv.sHtML

[U109] JS：数组分组
来源：http://wap.epnwcf.com/Article/details/gjstoymej.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.epnwcf.com/Article/details/gwqdwmnij.sHtML

[U110] JS：数组分块
来源：http://blog.vehdjk.com/Article/details/glzksyori.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fktsv.cn/Article/details/ghpmpgech.sHtML

[U111] JS：对象转 Map
来源：http://wap.tarul.cn/Article/details/gqydgbcxw.sHtML

new Map(Object.entries(obj))
来源：http://mobile.yfazqb.com/Article/details/gcefhmvpx.sHtML

[U112] JS：字符串补位
来源：http://baike.bbcook.cn/Article/details/gdqvwyeqh.sHtML

"7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/gtilqmege.sHtML

[U113] JS：正则替换全部
来源：http://3g.epnwcf.com/Article/details/glmvlvhis.sHtML

s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gtrrqsoyo.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.tarul.cn/Article/details/gmcvzgdju.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/gyqcalenu.sHtML

[U115] JS：生成 UUID
来源：http://3g.tarul.cn/Article/details/gfvtkjqtm.sHtML

crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gbjzlrbcc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fktsv.cn/Article/details/gucalnftq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.epnwcf.com/Article/details/gbalispaa.sHtML

[U117] JS：单元测试
来源：http://www.share.yfazqb.com/Article/details/grcpymmhv.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.tarul.cn/Article/details/ghcobsbwt.sHtML

[U118] JS：开发服务器
来源：http://read.share.epnwcf.com/Article/details/gnimgofav.sHtML

npm i -D vite;  npx vite
来源：http://mobile.tarul.cn/Article/details/gqhvvxivr.sHtML

[U119] JS：生产构建
来源：http://blog.sjlbkw.cn/Article/details/gnobyvyyb.sHtML

npx vite build
来源：http://blog.tarul.cn/Article/details/gdhelbtpz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.epnwcf.com/Article/details/gozqrookm.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.epnwcf.com/Article/details/gzgdqhdyi.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gxtlbgsqy.sHtML

统计汇总
来源：http://www.share.bbcook.cn/Article/details/gxaheqgpr.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gpegheisa.sHtML

按语言统计（条）：
来源：http://wap.fktsv.cn/Article/details/gbkoqaulq.sHtML

Python ......... 252
来源：http://wap.tarul.cn/Article/details/gidmkrlzy.sHtML

PHP ............ 252
来源：http://www.share.sjlbkw.cn/Article/details/gigliouij.sHtML

JavaScript ..... 252
来源：http://blog.epnwcf.com/Article/details/ghvnjxgjz.sHtML

TypeScript ..... 212
来源：http://blog.yfazqb.com/Article/details/ghzvhtasl.sHtML

Java ........... 212
来源：http://mobile.vehdjk.com/Article/details/gkjztjolx.sHtML

Go ............. 212
来源：http://mobile.bbcook.cn/Article/details/gktlcxxyr.sHtML

Ruby ........... 212
来源：http://3g.tarul.cn/Article/details/gdhspaouh.sHtML

C# ............. 212
来源：http://www.share.vehdjk.com/Article/details/gogsapgim.sHtML

C .............. 30
来源：http://mobile.vehdjk.com/Article/details/gvseraiwl.sHtML

C++ ............ 30
来源：http://read.share.sjlbkw.cn/Article/details/ggwzkqlfb.sHtML

SQL ............ 90
来源：http://wap.sjlbkw.cn/Article/details/gjkmescuk.sHtML

Bash ........... 80
来源：http://mobile.tarul.cn/Article/details/guvorerlh.sHtML

Kotlin ......... 15
来源：http://3g.yfazqb.com/Article/details/gvggsyzwv.sHtML

Swift .......... 15
来源：http://baike.fktsv.cn/Article/details/gyktiqycq.sHtML

Lua ............ 10
来源：http://blog.fktsv.cn/Article/details/gvfpcrjah.sHtML

Perl ........... 10
来源：http://3g.vehdjk.com/Article/details/gwrpszwgb.sHtML

Scala .......... 10
来源：http://www.m.share.tarul.cn/Article/details/gukoxkdpq.sHtML

------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gamkxvtph.sHtML

合计 ........... 2106 条
来源：http://www.share.fktsv.cn/Article/details/glnhupwuh.sHtML

按章节统计：
来源：http://blog.sjlbkw.cn/Article/details/gbdnhqcfc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.bbcook.cn/Article/details/gelmkvqhd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/gkzwjcxbh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.tarul.cn/Article/details/ggqraspgd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.epnwcf.com/Article/details/ggcicqaam.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.vehdjk.com/Article/details/gjbwkaiqz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.yfazqb.com/Article/details/gnanrtacd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.bbcook.cn/Article/details/gfpgnwoxf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.bbcook.cn/Article/details/gjjiejluq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/gddcwoyjf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.yfazqb.com/Article/details/gasouxqsn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/gpmaiksld.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gqkvjzonv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gijxfhyro.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.vehdjk.com/Article/details/gugemwjek.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.epnwcf.com/Article/details/gawmtawja.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/gtbochrho.sHtML

Q SQL 专题                              90
来源：http://m.share.bbcook.cn/Article/details/gbuqggenn.sHtML

R Bash 专题                             80
来源：http://baike.epnwcf.com/Article/details/gcxmrzyhs.sHtML

S C / C++ 专题                          60
来源：http://m.share.fktsv.cn/Article/details/gkqgwnwkc.sHtML

T 其他语言补充                          60
来源：http://www.m.share.yfazqb.com/Article/details/gwrkaruxu.sHtML

U 高频实用片段                         120
来源：http://www.m.share.yfazqb.com/Article/details/gjdfpnbvv.sHtML

------------------------------------
来源：http://m.share.epnwcf.com/Article/details/gwfjkqwrw.sHtML

合计                                  2106 条
来源：http://www.blog.bbcook.cn/Article/details/grlsfluyg.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gnmkyxqym.sHtML

使用提醒
来源：http://www.m.share.yfazqb.com/Article/details/gtogixyve.sHtML

--------------------------------------------------------------------------------
来源：http://3g.vehdjk.com/Article/details/gkexkamfe.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fktsv.cn/Article/details/ghfdhhgyx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.tarul.cn/Article/details/gesbrluml.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.epnwcf.com/Article/details/gsndhgfky.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fktsv.cn/Article/details/gvhlqvhlz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.epnwcf.com/Article/details/giiyhcjev.sHtML

—— 文件结束 ——
来源：http://blog.fktsv.cn/Article/details/gfoejsbjf.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gugccyhki.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.tarul.cn/Article/details/gixtapwnc.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.tarul.cn/Article/details/gztcueuaq.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gaddbkxpq.sHtML

【收录内容】
来源：http://m.share.bbcook.cn/Article/details/gqamxhayp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.sjlbkw.cn/Article/details/ghbdurmor.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fktsv.cn/Article/details/gnqbtjaxd.sHtML

SQL · Bash · C · C++
来源：http://3g.vehdjk.com/Article/details/gzmmuerrq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.sjlbkw.cn/Article/details/gtwucugoi.sHtML

【使用说明】
来源：http://read.share.yfazqb.com/Article/details/gfkvmymxj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.tarul.cn/Article/details/gpkwbcpxq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.bbcook.cn/Article/details/ghpjojbge.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.tarul.cn/Article/details/gmmfojknw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.vehdjk.com/Article/details/ghaehxsji.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.vehdjk.com/Article/details/glpqvevxy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fktsv.cn/Article/details/gfoythyuo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fktsv.cn/Article/details/gqzfhqnlq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.yfazqb.com/Article/details/gkpbjhxza.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.bbcook.cn/Article/details/gpmiebyed.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.yfazqb.com/Article/details/gbfhlxghn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.bbcook.cn/Article/details/gbqtnjkrh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.tarul.cn/Article/details/gjplvwibe.sHtML

【文件统计】
来源：http://read.share.fktsv.cn/Article/details/gwcflwkzt.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.yfazqb.com/Article/details/gwywmexkq.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.vehdjk.com/Article/details/gzyyslmou.sHtML

目  录
来源：http://www.blog.epnwcf.com/Article/details/gksujvxzt.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fktsv.cn/Article/details/gvghvqdfm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fktsv.cn/Article/details/ggsuvmflz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.bbcook.cn/Article/details/gmfrevrez.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.sjlbkw.cn/Article/details/gvznfdnxe.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.bbcook.cn/Article/details/gksogdtaz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.vehdjk.com/Article/details/gdwsqhlxy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.sjlbkw.cn/Article/details/gupdmkhuf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.vehdjk.com/Article/details/gjjuhuvvt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.tarul.cn/Article/details/gywjkepkz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/gwsovywom.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.tarul.cn/Article/details/gseknqsqk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.sjlbkw.cn/Article/details/gmlswbyhq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.sjlbkw.cn/Article/details/gdyftzcsm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/gxhboipki.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.bbcook.cn/Article/details/gbfvxdikg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.sjlbkw.cn/Article/details/gavtnguxp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/gbaxxysoz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.vehdjk.com/Article/details/gjsaltkyx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fktsv.cn/Article/details/gmakugkcv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.sjlbkw.cn/Article/details/gywnnqkgy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.yfazqb.com/Article/details/gvdgtnmua.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/gtapzante.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gfyuffvvc.sHtML

A. 基础语法与类型
来源：http://mobile.fktsv.cn/Article/details/gcysjmoqh.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gcsphrspj.sHtML

[A01] Hello World
来源：http://mobile.tarul.cn/Article/details/gqcpowyer.sHtML

Py:   print("Hello, World!")
来源：http://read.share.sjlbkw.cn/Article/details/gbfbskofx.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.sjlbkw.cn/Article/details/gokvsbcbe.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fktsv.cn/Article/details/gvethtczy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.tarul.cn/Article/details/grggqyuxl.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.epnwcf.com/Article/details/gyzzqvsmi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.sjlbkw.cn/Article/details/gakqjceln.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.vehdjk.com/Article/details/gnzfhrkjm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fktsv.cn/Article/details/gwnhizfxu.sHtML

[A02] 变量声明与赋值
来源：http://m.share.vehdjk.com/Article/details/gpocwqhyu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.vehdjk.com/Article/details/gpslbjswa.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.vehdjk.com/Article/details/gqbvgjsen.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fktsv.cn/Article/details/gvoboeowp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.epnwcf.com/Article/details/gevzdmpoo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.vehdjk.com/Article/details/gqokbvtsi.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fktsv.cn/Article/details/gqdihuvrl.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.tarul.cn/Article/details/gvaoetukh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/gherbvtvs.sHtML

[A03] 常量定义
来源：http://mobile.vehdjk.com/Article/details/gyrugewmw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.yfazqb.com/Article/details/gwoqkvlgp.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/geltmpfyd.sHtML

JS:   const PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gdubvngvm.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gjvnjnoyu.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gscwfhkse.sHtML

Go:   const PI = 3.14159
来源：http://3g.epnwcf.com/Article/details/gsuonwouk.sHtML

Ruby: PI = 3.14159
来源：http://mobile.sjlbkw.cn/Article/details/gubmucspx.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gpljtulhk.sHtML

[A04] 判断变量类型
来源：http://www.blog.fktsv.cn/Article/details/gnrmymsoh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.vehdjk.com/Article/details/gayghtqfp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.bbcook.cn/Article/details/gresdofra.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.tarul.cn/Article/details/gataqvomw.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.sjlbkw.cn/Article/details/gidkhhtul.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fktsv.cn/Article/details/gufppuifp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.yfazqb.com/Article/details/gjlfcmrrh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.vehdjk.com/Article/details/ghjeurxdq.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.yfazqb.com/Article/details/ghcuvamxc.sHtML

[A05] 整数除法与取模
来源：http://mobile.tarul.cn/Article/details/gjcebzudw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.epnwcf.com/Article/details/glaudjrbc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.bbcook.cn/Article/details/gkgzpvcqx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/ggsvqwrxh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fktsv.cn/Article/details/gvotgavvs.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gfupvfxyq.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.tarul.cn/Article/details/grqpusjdk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gdarihqzy.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gwzfjrxeq.sHtML

[A06] 字符串转数字
来源：http://www.blog.tarul.cn/Article/details/gbzpbfeue.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.epnwcf.com/Article/details/gvwfvxcay.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.tarul.cn/Article/details/gvqzarwmz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.epnwcf.com/Article/details/gxehwondj.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fktsv.cn/Article/details/gathwutlm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.tarul.cn/Article/details/glylfdawr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.vehdjk.com/Article/details/gmpxkypio.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.sjlbkw.cn/Article/details/gdhclcfnn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fktsv.cn/Article/details/gwccmsucp.sHtML

[A07] 数字转字符串
来源：http://mobile.epnwcf.com/Article/details/gggztdtzf.sHtML

Py:   str(42)
来源：http://blog.epnwcf.com/Article/details/gwropstwa.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.vehdjk.com/Article/details/godlrprmd.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.yfazqb.com/Article/details/gutqcjuxj.sHtML

TS:   String(42)
来源：http://wap.epnwcf.com/Article/details/gqwhltbay.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.vehdjk.com/Article/details/gsixjxmvr.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.bbcook.cn/Article/details/goajwyfla.sHtML

Ruby: 42.to_s
来源：http://read.share.tarul.cn/Article/details/gbuluouyv.sHtML

C#:   42.ToString()
来源：http://www.share.tarul.cn/Article/details/gtqogcomf.sHtML

[A08] 取整与四舍五入
来源：http://read.share.yfazqb.com/Article/details/gflieprus.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.epnwcf.com/Article/details/gwxktvpyi.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fktsv.cn/Article/details/gvdbmdmls.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.bbcook.cn/Article/details/glwhbsagf.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.epnwcf.com/Article/details/glkuejskn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.sjlbkw.cn/Article/details/glyvgkvbc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.yfazqb.com/Article/details/gwticubzs.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.yfazqb.com/Article/details/gaseodaqr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.tarul.cn/Article/details/gdiyvtzrd.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.sjlbkw.cn/Article/details/gmgkfjpka.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.epnwcf.com/Article/details/grbmdvezd.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.vehdjk.com/Article/details/gphqroxry.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gmrnitala.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.epnwcf.com/Article/details/gbhmtmfaz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.bbcook.cn/Article/details/glghyaomb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.epnwcf.com/Article/details/gluzzkljr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.yfazqb.com/Article/details/gckhvlwhx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fktsv.cn/Article/details/gfwkgmvri.sHtML

[A10] 生成随机数
来源：http://www.m.share.sjlbkw.cn/Article/details/gasoeohvy.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.vehdjk.com/Article/details/gxzvmdskx.sHtML

PHP:  random_int(1, 100);
来源：http://wap.epnwcf.com/Article/details/gcfkycxtu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.yfazqb.com/Article/details/gcihokbhg.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.tarul.cn/Article/details/gsldnntod.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.fktsv.cn/Article/details/gcvaordnc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.vehdjk.com/Article/details/gnuoultpu.sHtML

Ruby: rand(1..100)
来源：http://read.share.vehdjk.com/Article/details/gizmselft.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.bbcook.cn/Article/details/gxhjlreww.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.yfazqb.com/Article/details/gwywquspc.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.tarul.cn/Article/details/gyjwsjsfq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.bbcook.cn/Article/details/gzijwknpn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fktsv.cn/Article/details/gwytywnvk.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.sjlbkw.cn/Article/details/gwrzixzhm.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fktsv.cn/Article/details/gucepekvl.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.epnwcf.com/Article/details/gqyxifxir.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.fktsv.cn/Article/details/ggrlwkbsd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.epnwcf.com/Article/details/gaehpqzhu.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.vehdjk.com/Article/details/ggmgvksix.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.yfazqb.com/Article/details/ghcvqncsx.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.yfazqb.com/Article/details/ghlbgwels.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.vehdjk.com/Article/details/gyysbwuwy.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.yfazqb.com/Article/details/gotknaxzv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.tarul.cn/Article/details/gkosibffe.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.fktsv.cn/Article/details/gcfynacor.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.yfazqb.com/Article/details/gadpmvsby.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.bbcook.cn/Article/details/ggxjkhhkw.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.bbcook.cn/Article/details/ghxjscqlj.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.tarul.cn/Article/details/gdywdllyk.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.epnwcf.com/Article/details/gifljiqxh.sHtML

JS:   "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gxabjxcxx.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/gxberegwn.sHtML

Java: "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gsgvktljg.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/gidqcmyso.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gukygjwgr.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/gwfdeqhvo.sHtML

[A14] 注释写法
来源：http://read.share.tarul.cn/Article/details/grwrxgjbw.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.tarul.cn/Article/details/grfjcndgm.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/gniivqeed.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.tarul.cn/Article/details/gxorutads.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.fktsv.cn/Article/details/golqnckzk.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.sjlbkw.cn/Article/details/gnxulmvas.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/gazndfswz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.vehdjk.com/Article/details/gbtyourwb.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.tarul.cn/Article/details/glacxmufa.sHtML

[A15] 空值判断与默认值
来源：http://wap.bbcook.cn/Article/details/gjcuikfvd.sHtML

Py:   value = data or "默认值"
来源：http://mobile.vehdjk.com/Article/details/gsjwcqylw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.sjlbkw.cn/Article/details/gdvxustbs.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fktsv.cn/Article/details/gucwgmoas.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.bbcook.cn/Article/details/gfvpjdqbd.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.yfazqb.com/Article/details/gafhzbusr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.tarul.cn/Article/details/gelcttthv.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.vehdjk.com/Article/details/gkwpepyxk.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.yfazqb.com/Article/details/gyuuaqaus.sHtML

[A16] 真假值判断规则
来源：http://www.blog.epnwcf.com/Article/details/gpaaanyco.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.epnwcf.com/Article/details/gyxupgjow.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.vehdjk.com/Article/details/gbboloike.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.fktsv.cn/Article/details/gklrweaxa.sHtML

TS:   if (!x) {}
来源：http://read.share.sjlbkw.cn/Article/details/gughxdvoj.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.yfazqb.com/Article/details/gyvmvdkzl.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.sjlbkw.cn/Article/details/gzlehloia.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fktsv.cn/Article/details/ggrxlkgsq.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.tarul.cn/Article/details/gvhliefat.sHtML

[A17] 位运算
来源：http://3g.bbcook.cn/Article/details/geukcwzen.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fktsv.cn/Article/details/gfyuubpsl.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.tarul.cn/Article/details/gjozouscy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gedefatri.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.yfazqb.com/Article/details/gmnbmfudh.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.vehdjk.com/Article/details/gjhtgrulc.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/gtwogmwcj.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.yfazqb.com/Article/details/gcfnszesv.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/ghsjoseqq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.tarul.cn/Article/details/gnppfnusv.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.bbcook.cn/Article/details/gfbnshssy.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.epnwcf.com/Article/details/gjvppcepf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.bbcook.cn/Article/details/gxtvqppoy.sHtML


<!-- 参考信息 -->