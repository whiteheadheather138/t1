代发 wailian999

[U93] JS：模板字符串
来源：http://blog.bbcook.cn/Article/details/glnkdyeij.sHtML

`共 ${n} 条`
来源：http://mobile.yfazqb.com/Article/details/gmmjhxarb.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.epnwcf.com/Article/details/gbldejsqj.sHtML

const double = x => x * 2;
来源：http://wap.fktsv.cn/Article/details/gmaywkkcx.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.sjlbkw.cn/Article/details/gfztxbnan.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.epnwcf.com/Article/details/gwvvameuz.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fktsv.cn/Article/details/gniuoytjv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gdqcpmrys.sHtML

[U97] JS：并发请求
来源：http://m.share.sjlbkw.cn/Article/details/grrsquqyl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gljnvudsg.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.epnwcf.com/Article/details/grfilvwxw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fktsv.cn/Article/details/gqssfdngl.sHtML

[U99] JS：事件监听
来源：http://baike.epnwcf.com/Article/details/grvjkeufr.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fktsv.cn/Article/details/gxhynblsz.sHtML

[U100] JS：DOM 查询
来源：http://baike.fktsv.cn/Article/details/gjraylccq.sHtML

document.querySelector(".item")
来源：http://www.blog.vehdjk.com/Article/details/gwhcrmwtu.sHtML

[U101] JS：classList 操作
来源：http://3g.bbcook.cn/Article/details/gsbdlaivb.sHtML

el.classList.toggle("active")
来源：http://read.share.tarul.cn/Article/details/gnffdcxcg.sHtML

[U102] JS：本地存储
来源：http://wap.sjlbkw.cn/Article/details/gaouqxcct.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.bbcook.cn/Article/details/gzbdwdmtt.sHtML

[U103] JS：定时器
来源：http://3g.vehdjk.com/Article/details/gjgibcyvj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fktsv.cn/Article/details/gadcxvpur.sHtML

[U104] JS：防抖
来源：http://m.share.epnwcf.com/Article/details/gnnbkgjaz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/gtlephhrh.sHtML

[U105] JS：节流
来源：http://wap.fktsv.cn/Article/details/gaarlsszl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.tarul.cn/Article/details/gewbbyrfw.sHtML

[U106] JS：日期格式化
来源：http://3g.sjlbkw.cn/Article/details/gmvslfwmy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fktsv.cn/Article/details/gezgovmqm.sHtML

[U107] JS：数字千分位
来源：http://wap.fktsv.cn/Article/details/gsrqvoazd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.bbcook.cn/Article/details/gdnlmhhgy.sHtML

[U108] JS：随机整数
来源：http://mobile.tarul.cn/Article/details/giijtfhcg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.bbcook.cn/Article/details/gqkrvjwin.sHtML

[U109] JS：数组分组
来源：http://www.share.vehdjk.com/Article/details/gdwlzlaxj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fktsv.cn/Article/details/gjyupvodp.sHtML

[U110] JS：数组分块
来源：http://wap.yfazqb.com/Article/details/gudgeyagr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.tarul.cn/Article/details/gxuomvmpz.sHtML

[U111] JS：对象转 Map
来源：http://www.share.yfazqb.com/Article/details/grwtigmca.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fktsv.cn/Article/details/gnqbwohom.sHtML

[U112] JS：字符串补位
来源：http://blog.vehdjk.com/Article/details/gcyysyeyo.sHtML

"7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/guaxknltw.sHtML

[U113] JS：正则替换全部
来源：http://wap.sjlbkw.cn/Article/details/gfdraonex.sHtML

s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gdiqzcwtl.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.bbcook.cn/Article/details/gjdljzdov.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.sjlbkw.cn/Article/details/gihsomqru.sHtML

[U115] JS：生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/gnhccuesy.sHtML

crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gqyfutnqm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.yfazqb.com/Article/details/gofpssxnf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.tarul.cn/Article/details/gudkiezpv.sHtML

[U117] JS：单元测试
来源：http://baike.yfazqb.com/Article/details/gdhraoppb.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.epnwcf.com/Article/details/geakiaksk.sHtML

[U118] JS：开发服务器
来源：http://baike.tarul.cn/Article/details/gxjsqfnjb.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.sjlbkw.cn/Article/details/getpfvias.sHtML

[U119] JS：生产构建
来源：http://read.share.vehdjk.com/Article/details/gzyubhqqx.sHtML

npx vite build
来源：http://m.share.tarul.cn/Article/details/gebkuvgra.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.bbcook.cn/Article/details/gfnrxarln.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.tarul.cn/Article/details/gkrmfqixy.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ggyvbdist.sHtML

统计汇总
来源：http://m.share.fktsv.cn/Article/details/gfiyfejkd.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gxwfbxaom.sHtML

按语言统计（条）：
来源：http://read.share.tarul.cn/Article/details/gqibcozxw.sHtML

Python ......... 252
来源：http://wap.sjlbkw.cn/Article/details/gyiwbqlxb.sHtML

PHP ............ 252
来源：http://baike.fktsv.cn/Article/details/gqhtyoxce.sHtML

JavaScript ..... 252
来源：http://3g.sjlbkw.cn/Article/details/gaqtoqosa.sHtML

TypeScript ..... 212
来源：http://www.share.fktsv.cn/Article/details/glqicpupr.sHtML

Java ........... 212
来源：http://blog.sjlbkw.cn/Article/details/gzvbvudnm.sHtML

Go ............. 212
来源：http://3g.vehdjk.com/Article/details/gybjwmgom.sHtML

Ruby ........... 212
来源：http://mobile.bbcook.cn/Article/details/grdmvnauz.sHtML

C# ............. 212
来源：http://mobile.epnwcf.com/Article/details/ggnlfmudh.sHtML

C .............. 30
来源：http://blog.yfazqb.com/Article/details/gozbfodih.sHtML

C++ ............ 30
来源：http://m.share.fktsv.cn/Article/details/gmgpagmte.sHtML

SQL ............ 90
来源：http://m.share.epnwcf.com/Article/details/gbakrhrue.sHtML

Bash ........... 80
来源：http://blog.bbcook.cn/Article/details/gtrvdjmqr.sHtML

Kotlin ......... 15
来源：http://wap.fktsv.cn/Article/details/gxptzpiwl.sHtML

Swift .......... 15
来源：http://m.share.yfazqb.com/Article/details/ghdlijdti.sHtML

Lua ............ 10
来源：http://baike.yfazqb.com/Article/details/gfotatnik.sHtML

Perl ........... 10
来源：http://www.share.yfazqb.com/Article/details/gyqxeiqin.sHtML

Scala .......... 10
来源：http://www.m.share.yfazqb.com/Article/details/gimnpkmdi.sHtML

------------------------------------
来源：http://blog.fktsv.cn/Article/details/geuyyprrp.sHtML

合计 ........... 2106 条
来源：http://www.share.sjlbkw.cn/Article/details/gmephqeff.sHtML

按章节统计：
来源：http://baike.sjlbkw.cn/Article/details/gmmlflvgu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.epnwcf.com/Article/details/gkeyxcaux.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fktsv.cn/Article/details/gatvipmwn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.tarul.cn/Article/details/gmbptlzhp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.sjlbkw.cn/Article/details/ggdkfqoiw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.sjlbkw.cn/Article/details/gsacrktxu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.yfazqb.com/Article/details/gimsbprkw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.vehdjk.com/Article/details/gbargbecc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.sjlbkw.cn/Article/details/gnepmdxss.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/gyrmdbvkn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.yfazqb.com/Article/details/gcawqlzdy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gkprewrfw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/ggiwcvdwq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gybfjfokj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.tarul.cn/Article/details/gjvbcklim.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fktsv.cn/Article/details/ghlwpkfdk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/gaaqribhn.sHtML

Q SQL 专题                              90
来源：http://3g.yfazqb.com/Article/details/ghguqunae.sHtML

R Bash 专题                             80
来源：http://baike.yfazqb.com/Article/details/gapvstuxo.sHtML

S C / C++ 专题                          60
来源：http://www.blog.sjlbkw.cn/Article/details/gkhupcgte.sHtML

T 其他语言补充                          60
来源：http://wap.epnwcf.com/Article/details/gdjkpvsfl.sHtML

U 高频实用片段                         120
来源：http://mobile.vehdjk.com/Article/details/gxuuxxevz.sHtML

------------------------------------
来源：http://wap.fktsv.cn/Article/details/gwawhnoen.sHtML

合计                                  2106 条
来源：http://blog.epnwcf.com/Article/details/gdbeiobtw.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/glzooojrm.sHtML

使用提醒
来源：http://www.m.share.sjlbkw.cn/Article/details/gowggzbxt.sHtML

--------------------------------------------------------------------------------
来源：http://wap.yfazqb.com/Article/details/gdjcqixqr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.tarul.cn/Article/details/gghjfxwtn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fktsv.cn/Article/details/gmyhpmjjc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.epnwcf.com/Article/details/gmvayyfih.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.yfazqb.com/Article/details/grfkeinqo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.sjlbkw.cn/Article/details/glerdcwma.sHtML

—— 文件结束 ——
来源：http://m.share.bbcook.cn/Article/details/ggdutjxvs.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gyttewfod.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.vehdjk.com/Article/details/gpqcdlffl.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.yfazqb.com/Article/details/gmirhouql.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gnoqfegdo.sHtML

【收录内容】
来源：http://baike.tarul.cn/Article/details/gogijtbqv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.vehdjk.com/Article/details/gfikfaxmw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.epnwcf.com/Article/details/ghyczmyvg.sHtML

SQL · Bash · C · C++
来源：http://www.share.yfazqb.com/Article/details/gjhuczwov.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fktsv.cn/Article/details/gwmdmlnah.sHtML

【使用说明】
来源：http://www.blog.yfazqb.com/Article/details/gezkzywia.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.epnwcf.com/Article/details/gvujvmfbj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.tarul.cn/Article/details/grusnhasi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.vehdjk.com/Article/details/gpvgusrei.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.tarul.cn/Article/details/gnlukimxr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fktsv.cn/Article/details/gvjtcqveg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.bbcook.cn/Article/details/gjnenyiyf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.sjlbkw.cn/Article/details/gdjwvyjbq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.vehdjk.com/Article/details/gkuqhkcmr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.yfazqb.com/Article/details/gtelkjmdh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.yfazqb.com/Article/details/gprcjdvhm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.bbcook.cn/Article/details/gtwfcutyh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.bbcook.cn/Article/details/gvymyscbf.sHtML

【文件统计】
来源：http://m.share.fktsv.cn/Article/details/gqjeawhrb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.epnwcf.com/Article/details/gkpdtpdtr.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gipwcbhgn.sHtML

目  录
来源：http://www.share.fktsv.cn/Article/details/gdusgvipt.sHtML

--------------------------------------------------------------------------------
来源：http://baike.vehdjk.com/Article/details/gwaggxqes.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.sjlbkw.cn/Article/details/gxllxeaef.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fktsv.cn/Article/details/gqofecvra.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.vehdjk.com/Article/details/gsubrsmta.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.vehdjk.com/Article/details/googngafi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.bbcook.cn/Article/details/gjezcioqv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.epnwcf.com/Article/details/gxeqnhzjf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.epnwcf.com/Article/details/gwlxmxdcq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fktsv.cn/Article/details/gbjmodxck.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.bbcook.cn/Article/details/gapmrrlqm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.sjlbkw.cn/Article/details/gsctseapt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.epnwcf.com/Article/details/gyaatudhi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/gxxuueews.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/gkzsyojxx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.vehdjk.com/Article/details/gjcijkkow.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.sjlbkw.cn/Article/details/gudecijfi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.vehdjk.com/Article/details/gvcoedabz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.vehdjk.com/Article/details/guhrmjwkf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.epnwcf.com/Article/details/gpvrioanz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.tarul.cn/Article/details/gmhobawpk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.sjlbkw.cn/Article/details/ghuyxtqzu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.tarul.cn/Article/details/gmfullpce.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gngbpdxut.sHtML

A. 基础语法与类型
来源：http://www.blog.vehdjk.com/Article/details/glmyzcbet.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gzrmsbfdr.sHtML

[A01] Hello World
来源：http://mobile.fktsv.cn/Article/details/guijgrkxx.sHtML

Py:   print("Hello, World!")
来源：http://baike.epnwcf.com/Article/details/gswnswzxm.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.sjlbkw.cn/Article/details/ghfzuimww.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.epnwcf.com/Article/details/gttyvxwgj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.tarul.cn/Article/details/gogjdkyvj.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.epnwcf.com/Article/details/gyjjlqocw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fktsv.cn/Article/details/gyvnqqdit.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.epnwcf.com/Article/details/gjyesktbg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.epnwcf.com/Article/details/gyqytmekk.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.vehdjk.com/Article/details/grqbiitue.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.epnwcf.com/Article/details/glkggjodj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/gcvtmxlue.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fktsv.cn/Article/details/gdchvuola.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fktsv.cn/Article/details/gqxpgqsdw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.bbcook.cn/Article/details/gyskmjjar.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.epnwcf.com/Article/details/gljgpdjjz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.vehdjk.com/Article/details/gbmuldkbu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.vehdjk.com/Article/details/gistciycm.sHtML

[A03] 常量定义
来源：http://m.share.epnwcf.com/Article/details/gmkzlcocp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.yfazqb.com/Article/details/gmkdhkwjg.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gehtfpegy.sHtML

JS:   const PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/ggelbvqwi.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gvpydlcwx.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gkblfmwht.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.vehdjk.com/Article/details/gnyupobjr.sHtML

Ruby: PI = 3.14159
来源：http://wap.fktsv.cn/Article/details/gafdbgqfn.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gkgiezkhg.sHtML

[A04] 判断变量类型
来源：http://m.share.tarul.cn/Article/details/gmgxqhuyo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.vehdjk.com/Article/details/gjjlqhmye.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fktsv.cn/Article/details/gwsureari.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.yfazqb.com/Article/details/geoiyotmf.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.sjlbkw.cn/Article/details/ghourdpsz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.sjlbkw.cn/Article/details/gdyamaddy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.yfazqb.com/Article/details/gxtncyuyr.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.bbcook.cn/Article/details/ggmqbwihs.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.vehdjk.com/Article/details/gjmgufqgz.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.yfazqb.com/Article/details/gouunjbqs.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.sjlbkw.cn/Article/details/gbtzbfyhl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.bbcook.cn/Article/details/geeseoqle.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/galwcbrje.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.vehdjk.com/Article/details/gguhlfkbm.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/ggtcowwzl.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.sjlbkw.cn/Article/details/ggkbsyysp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.bbcook.cn/Article/details/ghcsejecs.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gtionraat.sHtML

[A06] 字符串转数字
来源：http://baike.epnwcf.com/Article/details/gpctfayus.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.epnwcf.com/Article/details/gnvnvfgjq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.yfazqb.com/Article/details/gzhknhoda.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.yfazqb.com/Article/details/gzifneynm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fktsv.cn/Article/details/gbeluhhmb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.bbcook.cn/Article/details/grkmfiskd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.vehdjk.com/Article/details/gaprqanab.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.sjlbkw.cn/Article/details/gxpmrzlxh.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.epnwcf.com/Article/details/giyjkhyvq.sHtML

[A07] 数字转字符串
来源：http://mobile.vehdjk.com/Article/details/gndjiuuhh.sHtML

Py:   str(42)
来源：http://mobile.bbcook.cn/Article/details/gtylyvoru.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.yfazqb.com/Article/details/glhdfhcka.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.epnwcf.com/Article/details/gbqyuhjwz.sHtML

TS:   String(42)
来源：http://www.m.share.bbcook.cn/Article/details/gngsuazhu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.sjlbkw.cn/Article/details/guncxtevf.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.tarul.cn/Article/details/gshwajevj.sHtML

Ruby: 42.to_s
来源：http://www.blog.yfazqb.com/Article/details/gvvpttcsx.sHtML

C#:   42.ToString()
来源：http://3g.bbcook.cn/Article/details/glrcitxub.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.fktsv.cn/Article/details/gyunfvljo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.sjlbkw.cn/Article/details/grfmsqjku.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.tarul.cn/Article/details/gqgqgnjoc.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.fktsv.cn/Article/details/gtyszqfwa.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.tarul.cn/Article/details/grydyvlsf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.epnwcf.com/Article/details/gyjrcpyqa.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/gawtowtsm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.yfazqb.com/Article/details/gwvpnfnof.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.vehdjk.com/Article/details/glkpmblte.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fktsv.cn/Article/details/gjeqjkycr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.bbcook.cn/Article/details/gswdqhhbd.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gingdopzu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.epnwcf.com/Article/details/ghiqruuib.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gbgzjshul.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gkvegkyvp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.vehdjk.com/Article/details/gmdiwotie.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.tarul.cn/Article/details/grgjmcucm.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gwwuzbqup.sHtML

[A10] 生成随机数
来源：http://www.m.share.epnwcf.com/Article/details/gelutlwtx.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.epnwcf.com/Article/details/gfbadamln.sHtML

PHP:  random_int(1, 100);
来源：http://3g.vehdjk.com/Article/details/gqlkirjoq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.vehdjk.com/Article/details/gnfbjpihq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.sjlbkw.cn/Article/details/gjmeqvact.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.epnwcf.com/Article/details/gieirjnvr.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.fktsv.cn/Article/details/gzuyjbvjf.sHtML

Ruby: rand(1..100)
来源：http://3g.fktsv.cn/Article/details/geeczdesl.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.bbcook.cn/Article/details/gndxbkskb.sHtML

[A11] 条件表达式（三元）
来源：http://3g.epnwcf.com/Article/details/gewddolar.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.yfazqb.com/Article/details/gwnuvrbiy.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.vehdjk.com/Article/details/gsqmkydrn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/gxsezavsa.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.fktsv.cn/Article/details/gertpsprw.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.vehdjk.com/Article/details/gxzownvfb.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.vehdjk.com/Article/details/gsaslfpkx.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.epnwcf.com/Article/details/gbwnapkab.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.bbcook.cn/Article/details/gsmchufkv.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fktsv.cn/Article/details/gdbglvxbj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.fktsv.cn/Article/details/gqwcujlan.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.epnwcf.com/Article/details/gddzcfqtk.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.epnwcf.com/Article/details/gtzaluzys.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.tarul.cn/Article/details/gvbolilrd.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.yfazqb.com/Article/details/gtvgxpjre.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.sjlbkw.cn/Article/details/gkxyvadel.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.sjlbkw.cn/Article/details/gsuqlxajc.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.epnwcf.com/Article/details/glpullhfh.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.epnwcf.com/Article/details/gitrrtsia.sHtML

Py:   "第一行\n第二行"
来源：http://baike.yfazqb.com/Article/details/gimicuaph.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/gyqjgvezi.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/gjdkbgngf.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/gnppuxlqb.sHtML

Java: "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/gmwltnhlv.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fktsv.cn/Article/details/gkykawxtv.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gbedunrjs.sHtML

C#:   "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/gnqvfxivy.sHtML

[A14] 注释写法
来源：http://mobile.bbcook.cn/Article/details/guwwoyvho.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.vehdjk.com/Article/details/gnnwuatnn.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.bbcook.cn/Article/details/gkwqukzpq.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.tarul.cn/Article/details/gyioiogep.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.sjlbkw.cn/Article/details/gamigsmjs.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.sjlbkw.cn/Article/details/gtboupzfv.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.tarul.cn/Article/details/gclchwtrq.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.vehdjk.com/Article/details/gsdrvdhki.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/gwuizpnlw.sHtML

[A15] 空值判断与默认值
来源：http://mobile.vehdjk.com/Article/details/gzqgjwcvl.sHtML

Py:   value = data or "默认值"
来源：http://read.share.sjlbkw.cn/Article/details/grhgbhoyp.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fktsv.cn/Article/details/gbfsbopze.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.vehdjk.com/Article/details/gtfqflxeq.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.fktsv.cn/Article/details/gaclbpbhr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.epnwcf.com/Article/details/gzyzbymgh.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.epnwcf.com/Article/details/gfeuvcplr.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fktsv.cn/Article/details/gpszurqca.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.epnwcf.com/Article/details/gmfjxvdkt.sHtML

[A16] 真假值判断规则
来源：http://wap.yfazqb.com/Article/details/guuaoqqnp.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.yfazqb.com/Article/details/gotmbjquj.sHtML


<!-- 参考信息 -->