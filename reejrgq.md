代发 wailian999

[U103] JS：定时器
来源：http://www.share.vehdjk.com/Article/details/gjwqkwfqr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.epnwcf.com/Article/details/gxhzjgdoj.sHtML

[U104] JS：防抖
来源：http://mobile.vehdjk.com/Article/details/gjpzoeceb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/gxsvgfsrz.sHtML

[U105] JS：节流
来源：http://blog.tarul.cn/Article/details/ginvknayr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.vehdjk.com/Article/details/gjeehjomb.sHtML

[U106] JS：日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gummbqhet.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.tarul.cn/Article/details/gsicqxcbo.sHtML

[U107] JS：数字千分位
来源：http://baike.tarul.cn/Article/details/gdfpjsgjz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.yfazqb.com/Article/details/gzdaicoiq.sHtML

[U108] JS：随机整数
来源：http://www.blog.sjlbkw.cn/Article/details/grkqodtqe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.yfazqb.com/Article/details/grvynozab.sHtML

[U109] JS：数组分组
来源：http://www.m.share.epnwcf.com/Article/details/gjwvhoxui.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/ggvgwajjv.sHtML

[U110] JS：数组分块
来源：http://baike.yfazqb.com/Article/details/grbmonmit.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.yfazqb.com/Article/details/gdkbssevd.sHtML

[U111] JS：对象转 Map
来源：http://baike.bbcook.cn/Article/details/gsvhfhyoj.sHtML

new Map(Object.entries(obj))
来源：http://www.share.sjlbkw.cn/Article/details/gdonolusd.sHtML

[U112] JS：字符串补位
来源：http://www.share.fktsv.cn/Article/details/ghpgeovcd.sHtML

"7".padStart(3, "0")
来源：http://3g.fktsv.cn/Article/details/gxlomhgym.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fktsv.cn/Article/details/gvnwcocql.sHtML

s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/grtuzjjvy.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.vehdjk.com/Article/details/gbjlklozf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.bbcook.cn/Article/details/gklnciyso.sHtML

[U115] JS：生成 UUID
来源：http://read.share.tarul.cn/Article/details/gqbuoyuvj.sHtML

crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/gbwawmmdi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.vehdjk.com/Article/details/gkhwkwhrr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/ghyokwdfg.sHtML

[U117] JS：单元测试
来源：http://m.share.bbcook.cn/Article/details/gjetczcsk.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.epnwcf.com/Article/details/gfzvvlqbl.sHtML

[U118] JS：开发服务器
来源：http://www.blog.epnwcf.com/Article/details/gyaltdsvy.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.vehdjk.com/Article/details/gpjmghbki.sHtML

[U119] JS：生产构建
来源：http://wap.tarul.cn/Article/details/gvidtijda.sHtML

npx vite build
来源：http://www.share.sjlbkw.cn/Article/details/gtspvytbz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.vehdjk.com/Article/details/glyecneda.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.yfazqb.com/Article/details/gjgfrpdyb.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/glzbgdcog.sHtML

统计汇总
来源：http://3g.epnwcf.com/Article/details/gpyounubn.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gtmnzqnbn.sHtML

按语言统计（条）：
来源：http://3g.vehdjk.com/Article/details/gzkjlxjjk.sHtML

Python ......... 252
来源：http://baike.yfazqb.com/Article/details/gvkwsppur.sHtML

PHP ............ 252
来源：http://baike.vehdjk.com/Article/details/ghphsrqlg.sHtML

JavaScript ..... 252
来源：http://baike.sjlbkw.cn/Article/details/gpablfxts.sHtML

TypeScript ..... 212
来源：http://wap.fktsv.cn/Article/details/gljpjmtgv.sHtML

Java ........... 212
来源：http://www.share.bbcook.cn/Article/details/gmsdlkpgz.sHtML

Go ............. 212
来源：http://blog.tarul.cn/Article/details/gosybtgqc.sHtML

Ruby ........... 212
来源：http://blog.sjlbkw.cn/Article/details/gndwyfnkt.sHtML

C# ............. 212
来源：http://wap.yfazqb.com/Article/details/gvyuaiiof.sHtML

C .............. 30
来源：http://read.share.sjlbkw.cn/Article/details/gqczxcevo.sHtML

C++ ............ 30
来源：http://mobile.sjlbkw.cn/Article/details/gtouvqtut.sHtML

SQL ............ 90
来源：http://baike.tarul.cn/Article/details/glqqyxssd.sHtML

Bash ........... 80
来源：http://mobile.fktsv.cn/Article/details/gfquxcheh.sHtML

Kotlin ......... 15
来源：http://wap.tarul.cn/Article/details/ghgduknzk.sHtML

Swift .......... 15
来源：http://www.share.vehdjk.com/Article/details/gdylvekxj.sHtML

Lua ............ 10
来源：http://baike.fktsv.cn/Article/details/grmutcteq.sHtML

Perl ........... 10
来源：http://blog.yfazqb.com/Article/details/gskznmluu.sHtML

Scala .......... 10
来源：http://blog.vehdjk.com/Article/details/grucprvcm.sHtML

------------------------------------
来源：http://blog.vehdjk.com/Article/details/gdgesfhtx.sHtML

合计 ........... 2106 条
来源：http://3g.epnwcf.com/Article/details/gsrfqxhaf.sHtML

按章节统计：
来源：http://www.blog.fktsv.cn/Article/details/gtzxxkhtk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.vehdjk.com/Article/details/gcgmyjvje.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.tarul.cn/Article/details/gxrzzcycj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fktsv.cn/Article/details/gzahliigb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.sjlbkw.cn/Article/details/gcgurhyuh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.bbcook.cn/Article/details/gzmjcgcmw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.tarul.cn/Article/details/gxzvvptoa.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.vehdjk.com/Article/details/ghairrhdl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.bbcook.cn/Article/details/gbiyviscs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gfywugczf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.tarul.cn/Article/details/gibxdndom.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/glekrupci.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gweoslmeq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/gbdyucqrk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.sjlbkw.cn/Article/details/gvtuxvfnn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.bbcook.cn/Article/details/gglziltzl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/gzgnkpfai.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fktsv.cn/Article/details/gwwkrdyvb.sHtML

R Bash 专题                             80
来源：http://3g.fktsv.cn/Article/details/giwqipvwh.sHtML

S C / C++ 专题                          60
来源：http://mobile.vehdjk.com/Article/details/gqhlzthpg.sHtML

T 其他语言补充                          60
来源：http://www.m.share.vehdjk.com/Article/details/gyossedsz.sHtML

U 高频实用片段                         120
来源：http://read.share.sjlbkw.cn/Article/details/geyiisvix.sHtML

------------------------------------
来源：http://blog.vehdjk.com/Article/details/grduthmxu.sHtML

合计                                  2106 条
来源：http://www.share.epnwcf.com/Article/details/gkobrcufc.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/guvxmiqha.sHtML

使用提醒
来源：http://www.blog.epnwcf.com/Article/details/gerhmgcdo.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gzonbouyq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.bbcook.cn/Article/details/ghlszbbkx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.tarul.cn/Article/details/gqdsujnve.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.sjlbkw.cn/Article/details/gxkyvrzis.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.vehdjk.com/Article/details/gitifwglc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.yfazqb.com/Article/details/gkyvaofhu.sHtML

—— 文件结束 ——
来源：http://m.share.vehdjk.com/Article/details/gtajmwfba.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/giyurmjlq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.bbcook.cn/Article/details/gtmgydbgk.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fktsv.cn/Article/details/gkbnodexm.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gkjcexsgf.sHtML

【收录内容】
来源：http://3g.epnwcf.com/Article/details/ggyiyigiy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.bbcook.cn/Article/details/gbwxjefnp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.yfazqb.com/Article/details/gtpwqejfb.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.sjlbkw.cn/Article/details/gticwfuih.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.tarul.cn/Article/details/gfisoryyc.sHtML

【使用说明】
来源：http://www.share.sjlbkw.cn/Article/details/gmdwjaigs.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fktsv.cn/Article/details/gorhhcybg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.bbcook.cn/Article/details/gsgjwxljr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.bbcook.cn/Article/details/gvfsuiggn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.tarul.cn/Article/details/gjudzepch.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.tarul.cn/Article/details/gvaedyhze.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fktsv.cn/Article/details/gxvsoedcl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.bbcook.cn/Article/details/gwegacuhq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.vehdjk.com/Article/details/gxtlxeczw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.epnwcf.com/Article/details/gbupwfojt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.yfazqb.com/Article/details/gqrsufxtd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.vehdjk.com/Article/details/gndwivldm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.yfazqb.com/Article/details/gipuzqpto.sHtML

【文件统计】
来源：http://blog.epnwcf.com/Article/details/gyqckvvzz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.tarul.cn/Article/details/gdkyxmucx.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gdasvqzsr.sHtML

目  录
来源：http://www.share.tarul.cn/Article/details/guapcbfny.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/gvxowksdu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpzucdnd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fktsv.cn/Article/details/gufbgokbh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.bbcook.cn/Article/details/glnrgqlts.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.sjlbkw.cn/Article/details/gbvixduro.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.yfazqb.com/Article/details/gvwdchamp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.sjlbkw.cn/Article/details/gwobpbbyu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.tarul.cn/Article/details/goyxafmnj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.vehdjk.com/Article/details/grlgglhei.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.tarul.cn/Article/details/gbsslyhsm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.vehdjk.com/Article/details/glfxvmddd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.bbcook.cn/Article/details/glxrxirfy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/gidheugrq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/gyujrggid.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.yfazqb.com/Article/details/gkbyqmmhf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fktsv.cn/Article/details/gwmumxcjv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/gmuqgdbhm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fktsv.cn/Article/details/gbtuxysqq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.tarul.cn/Article/details/grckxjxfd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.epnwcf.com/Article/details/gferbquae.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/gcctvibil.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.epnwcf.com/Article/details/gmczjlami.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gmrpgdaer.sHtML

A. 基础语法与类型
来源：http://m.share.epnwcf.com/Article/details/gmoshckab.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gngzqjnji.sHtML

[A01] Hello World
来源：http://baike.tarul.cn/Article/details/gviarvrzw.sHtML

Py:   print("Hello, World!")
来源：http://www.share.yfazqb.com/Article/details/gwjqanhcr.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fktsv.cn/Article/details/ggqvqealh.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.sjlbkw.cn/Article/details/gijasdnix.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.tarul.cn/Article/details/gsdbpssfk.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.epnwcf.com/Article/details/gyhlvopyh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkggsrgom.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.yfazqb.com/Article/details/gsbvxtqbl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.tarul.cn/Article/details/ghguswkju.sHtML

[A02] 变量声明与赋值
来源：http://mobile.vehdjk.com/Article/details/gbnsffccm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.yfazqb.com/Article/details/ghuiffvke.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.tarul.cn/Article/details/gllfqcrtb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.bbcook.cn/Article/details/gqkobyrlf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.vehdjk.com/Article/details/gcmgrnxrl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fktsv.cn/Article/details/gxltjnckg.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fktsv.cn/Article/details/guimihykp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.epnwcf.com/Article/details/gtqrgjmfh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.yfazqb.com/Article/details/gvyawczzr.sHtML

[A03] 常量定义
来源：http://baike.vehdjk.com/Article/details/gvxgqwxum.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.tarul.cn/Article/details/gnyuauutr.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gnrwyowmh.sHtML

JS:   const PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gnposfjom.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gqandpkmq.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/gruhwncfi.sHtML

Go:   const PI = 3.14159
来源：http://m.share.epnwcf.com/Article/details/gxzcxczji.sHtML

Ruby: PI = 3.14159
来源：http://read.share.tarul.cn/Article/details/gcolwfqcp.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/glhrdmrwz.sHtML

[A04] 判断变量类型
来源：http://www.share.bbcook.cn/Article/details/gqzvmvdxd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.tarul.cn/Article/details/gfmijdcir.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.yfazqb.com/Article/details/gfmzkaqrn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.tarul.cn/Article/details/guyruqfqt.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fktsv.cn/Article/details/gskpyqwzu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.tarul.cn/Article/details/gecaiazjh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.tarul.cn/Article/details/gfwccoyln.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.vehdjk.com/Article/details/gjqigcawl.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fktsv.cn/Article/details/ggfnroazu.sHtML

[A05] 整数除法与取模
来源：http://wap.bbcook.cn/Article/details/grtttabro.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.bbcook.cn/Article/details/gsygbigwi.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.vehdjk.com/Article/details/gbayifffi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.vehdjk.com/Article/details/gforkqkcf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gzrvhkxcs.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.bbcook.cn/Article/details/ggcqzovji.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.bbcook.cn/Article/details/gpareyups.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.yfazqb.com/Article/details/gzcqngbxz.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.bbcook.cn/Article/details/gvvtsazgi.sHtML

[A06] 字符串转数字
来源：http://mobile.tarul.cn/Article/details/glvlyikar.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.tarul.cn/Article/details/gcvcmiqgx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.bbcook.cn/Article/details/gmfehnjcf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.sjlbkw.cn/Article/details/geygpqtnl.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.tarul.cn/Article/details/glepvcnyw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.sjlbkw.cn/Article/details/gvarghdtq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.yfazqb.com/Article/details/ghbztikbw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.vehdjk.com/Article/details/gtzmumrxy.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.tarul.cn/Article/details/ghtsjxioc.sHtML

[A07] 数字转字符串
来源：http://3g.tarul.cn/Article/details/giclnmcga.sHtML

Py:   str(42)
来源：http://www.m.share.vehdjk.com/Article/details/ggpboeoig.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.tarul.cn/Article/details/gjgidqwmz.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.bbcook.cn/Article/details/gqpcivuxz.sHtML

TS:   String(42)
来源：http://baike.bbcook.cn/Article/details/gcpxilpqx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.tarul.cn/Article/details/gbyuybdsg.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.tarul.cn/Article/details/gowfvqtid.sHtML

Ruby: 42.to_s
来源：http://www.share.tarul.cn/Article/details/gzrrycmid.sHtML

C#:   42.ToString()
来源：http://read.share.epnwcf.com/Article/details/gnktznnpf.sHtML

[A08] 取整与四舍五入
来源：http://baike.vehdjk.com/Article/details/gimnjdrpv.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.yfazqb.com/Article/details/gtcfbpxfp.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fktsv.cn/Article/details/gxfzbtwpj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.bbcook.cn/Article/details/gvszbmtsz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.bbcook.cn/Article/details/geabmzryd.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.sjlbkw.cn/Article/details/gpmtzddph.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/gusnkmxbz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.tarul.cn/Article/details/gxozlffsb.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fktsv.cn/Article/details/givvnlytg.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.vehdjk.com/Article/details/gkpxcskuw.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.bbcook.cn/Article/details/gcccjtcfa.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gwiwhaqyr.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.epnwcf.com/Article/details/goepeaxqs.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/griqkhryh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.tarul.cn/Article/details/gfahjyghg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.yfazqb.com/Article/details/geblpoitr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.fktsv.cn/Article/details/gepekzhul.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.fktsv.cn/Article/details/ggodjvvrk.sHtML

[A10] 生成随机数
来源：http://www.m.share.epnwcf.com/Article/details/gtktlfgyg.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.tarul.cn/Article/details/gxzkxaehe.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.yfazqb.com/Article/details/gnslnntei.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.epnwcf.com/Article/details/gliwqksuw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.epnwcf.com/Article/details/gvibdqfof.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.vehdjk.com/Article/details/gzluktvbv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.yfazqb.com/Article/details/gcyotduga.sHtML

Ruby: rand(1..100)
来源：http://wap.tarul.cn/Article/details/gzudwpvso.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.yfazqb.com/Article/details/gyuufsykt.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.sjlbkw.cn/Article/details/gfgupfzcn.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.epnwcf.com/Article/details/gzorwnwkr.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.sjlbkw.cn/Article/details/goqnnwuts.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.bbcook.cn/Article/details/gnhardtkn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.vehdjk.com/Article/details/gbtqszztb.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.bbcook.cn/Article/details/gkespkiwf.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.fktsv.cn/Article/details/gtawpwjlu.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.bbcook.cn/Article/details/gdxctvxab.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.tarul.cn/Article/details/ghvjvitio.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.yfazqb.com/Article/details/gengkoxpd.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.epnwcf.com/Article/details/gegyccrql.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.bbcook.cn/Article/details/gwtlaeejm.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fktsv.cn/Article/details/gyhtfvomv.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.vehdjk.com/Article/details/gojnxfqxp.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.bbcook.cn/Article/details/gfuawnkvn.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.bbcook.cn/Article/details/gotfskuvb.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.bbcook.cn/Article/details/gwydqieui.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.epnwcf.com/Article/details/gosydjikl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.vehdjk.com/Article/details/grynqavsg.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gzkjiiyiv.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/gsglkgyyx.sHtML

JS:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/gerbzdrxu.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/gfcfpfufz.sHtML

Java: "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/gdbgraazp.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/gqmkdminz.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/grhdgefxa.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/gqlpkqrfx.sHtML

[A14] 注释写法
来源：http://www.share.sjlbkw.cn/Article/details/gfycikpbv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.epnwcf.com/Article/details/ghaphmqdj.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.sjlbkw.cn/Article/details/gfuvtuvvs.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.tarul.cn/Article/details/gaahgectb.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.sjlbkw.cn/Article/details/gbrvvhsuf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.fktsv.cn/Article/details/glzmrjxhk.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.epnwcf.com/Article/details/gbecmroxz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.bbcook.cn/Article/details/gfeadvotx.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.sjlbkw.cn/Article/details/gtzvqgygt.sHtML

[A15] 空值判断与默认值
来源：http://3g.epnwcf.com/Article/details/gijufwgex.sHtML

Py:   value = data or "默认值"
来源：http://www.share.epnwcf.com/Article/details/glqzkcugf.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fktsv.cn/Article/details/gopdsbang.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.epnwcf.com/Article/details/gbgtwzdxo.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.sjlbkw.cn/Article/details/grbbwzayn.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.epnwcf.com/Article/details/gjrwvstvw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fktsv.cn/Article/details/gkvmvjeju.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.tarul.cn/Article/details/gkanamofh.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.epnwcf.com/Article/details/gwvaojujl.sHtML

[A16] 真假值判断规则
来源：http://baike.epnwcf.com/Article/details/gbxbmaiuw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.epnwcf.com/Article/details/guqcxdsmd.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.yfazqb.com/Article/details/googlsqlv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.sjlbkw.cn/Article/details/gtvkifhor.sHtML

TS:   if (!x) {}
来源：http://mobile.tarul.cn/Article/details/gcyqaulsj.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.epnwcf.com/Article/details/gtubioglm.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.vehdjk.com/Article/details/gdayznava.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.yfazqb.com/Article/details/gljcbumaj.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.vehdjk.com/Article/details/glpqmgvvk.sHtML

[A17] 位运算
来源：http://baike.vehdjk.com/Article/details/glqgyzhlj.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gtpiwiftb.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.bbcook.cn/Article/details/gkvgeoqvw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/gplgqfqqh.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fktsv.cn/Article/details/gjglsyadn.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.sjlbkw.cn/Article/details/gswssyyty.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.yfazqb.com/Article/details/gvbldyuik.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/giqipyidy.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.vehdjk.com/Article/details/gyqfycqpk.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.vehdjk.com/Article/details/gbdbpbkpy.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.bbcook.cn/Article/details/gnueiacvr.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.epnwcf.com/Article/details/gtepdxezj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fktsv.cn/Article/details/gqgvdhwlf.sHtML


<!-- 参考信息 -->