代发 wailian999

[U95] JS：Promise 包装
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxbvmdpm.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.sjlbkw.cn/Article/details/gumbhbocd.sHtML

[U96] JS：async/await 与异常
来源：http://baike.yfazqb.com/Article/details/gygmdqbet.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gloajoacz.sHtML

[U97] JS：并发请求
来源：http://read.share.yfazqb.com/Article/details/gnmwntaof.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/ggakfmtoj.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.epnwcf.com/Article/details/gqqhknpox.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.vehdjk.com/Article/details/gerjezmbh.sHtML

[U99] JS：事件监听
来源：http://www.blog.sjlbkw.cn/Article/details/gopsjbvmg.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.bbcook.cn/Article/details/gigfmrswc.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.sjlbkw.cn/Article/details/gfjwvwllh.sHtML

document.querySelector(".item")
来源：http://read.share.vehdjk.com/Article/details/gclbxyvcr.sHtML

[U101] JS：classList 操作
来源：http://3g.yfazqb.com/Article/details/gxybrlqra.sHtML

el.classList.toggle("active")
来源：http://www.m.share.bbcook.cn/Article/details/ghiiwxgef.sHtML

[U102] JS：本地存储
来源：http://www.blog.fktsv.cn/Article/details/gmduyjlrl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.tarul.cn/Article/details/gbwxwchqn.sHtML

[U103] JS：定时器
来源：http://baike.sjlbkw.cn/Article/details/gfwqbehdb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fktsv.cn/Article/details/grhpvchcu.sHtML

[U104] JS：防抖
来源：http://baike.yfazqb.com/Article/details/gnghnrmtd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/gmemamgod.sHtML

[U105] JS：节流
来源：http://www.share.tarul.cn/Article/details/gezwheadf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.tarul.cn/Article/details/garsycdor.sHtML

[U106] JS：日期格式化
来源：http://www.blog.bbcook.cn/Article/details/giaxaryvx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.tarul.cn/Article/details/gzjovtalr.sHtML

[U107] JS：数字千分位
来源：http://read.share.sjlbkw.cn/Article/details/galspqezy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.vehdjk.com/Article/details/ghcwnifen.sHtML

[U108] JS：随机整数
来源：http://www.share.vehdjk.com/Article/details/gjyzgzwuj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.tarul.cn/Article/details/gwfdxggjq.sHtML

[U109] JS：数组分组
来源：http://blog.sjlbkw.cn/Article/details/gqapyaaqk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.epnwcf.com/Article/details/gmdcajvbw.sHtML

[U110] JS：数组分块
来源：http://m.share.sjlbkw.cn/Article/details/gmrafhwiq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.epnwcf.com/Article/details/gnwfugbup.sHtML

[U111] JS：对象转 Map
来源：http://blog.bbcook.cn/Article/details/gskytqzji.sHtML

new Map(Object.entries(obj))
来源：http://baike.epnwcf.com/Article/details/gpykytvbz.sHtML

[U112] JS：字符串补位
来源：http://m.share.bbcook.cn/Article/details/gyjtqnsew.sHtML

"7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gqsbbjona.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.epnwcf.com/Article/details/gpelioqvf.sHtML

s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gmahanxtl.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.vehdjk.com/Article/details/gphmhphoz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/grcylveqb.sHtML

[U115] JS：生成 UUID
来源：http://read.share.vehdjk.com/Article/details/ghwrgkbmx.sHtML

crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/gdguqsdwp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.vehdjk.com/Article/details/geowjmrcx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.epnwcf.com/Article/details/ggnwjqtdk.sHtML

[U117] JS：单元测试
来源：http://www.blog.bbcook.cn/Article/details/gzzgfyvup.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.vehdjk.com/Article/details/gvvzvjhil.sHtML

[U118] JS：开发服务器
来源：http://www.blog.sjlbkw.cn/Article/details/gsepkgtfe.sHtML

npm i -D vite;  npx vite
来源：http://www.share.epnwcf.com/Article/details/gqywcypke.sHtML

[U119] JS：生产构建
来源：http://wap.epnwcf.com/Article/details/gphnvdpuy.sHtML

npx vite build
来源：http://www.blog.sjlbkw.cn/Article/details/gxlbjdmml.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.epnwcf.com/Article/details/gzuzbvniu.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.sjlbkw.cn/Article/details/ghorkddzn.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gwmeadhmq.sHtML

统计汇总
来源：http://www.blog.fktsv.cn/Article/details/gjfcgweoe.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gmrucqtax.sHtML

按语言统计（条）：
来源：http://3g.fktsv.cn/Article/details/glddosxzo.sHtML

Python ......... 252
来源：http://m.share.tarul.cn/Article/details/gegcpztot.sHtML

PHP ............ 252
来源：http://read.share.yfazqb.com/Article/details/giepvxaya.sHtML

JavaScript ..... 252
来源：http://wap.fktsv.cn/Article/details/gbkbuwvwv.sHtML

TypeScript ..... 212
来源：http://baike.epnwcf.com/Article/details/gstvugkco.sHtML

Java ........... 212
来源：http://blog.bbcook.cn/Article/details/gbtpiardf.sHtML

Go ............. 212
来源：http://www.share.sjlbkw.cn/Article/details/gcsxsozvu.sHtML

Ruby ........... 212
来源：http://www.m.share.fktsv.cn/Article/details/gltqlehrc.sHtML

C# ............. 212
来源：http://www.blog.epnwcf.com/Article/details/gssipfqzs.sHtML

C .............. 30
来源：http://www.blog.yfazqb.com/Article/details/gczilkung.sHtML

C++ ............ 30
来源：http://www.blog.vehdjk.com/Article/details/gcrbntcik.sHtML

SQL ............ 90
来源：http://m.share.epnwcf.com/Article/details/goyyxeafp.sHtML

Bash ........... 80
来源：http://wap.bbcook.cn/Article/details/gcrcijucr.sHtML

Kotlin ......... 15
来源：http://www.blog.sjlbkw.cn/Article/details/gzxgnpoqi.sHtML

Swift .......... 15
来源：http://mobile.sjlbkw.cn/Article/details/gesjikgfa.sHtML

Lua ............ 10
来源：http://baike.bbcook.cn/Article/details/gnapgjvjo.sHtML

Perl ........... 10
来源：http://wap.sjlbkw.cn/Article/details/gflbnxsjr.sHtML

Scala .......... 10
来源：http://3g.yfazqb.com/Article/details/gvknfijky.sHtML

------------------------------------
来源：http://blog.fktsv.cn/Article/details/gokrnucih.sHtML

合计 ........... 2106 条
来源：http://mobile.epnwcf.com/Article/details/gifxhvhqv.sHtML

按章节统计：
来源：http://www.share.vehdjk.com/Article/details/ggqierosd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.yfazqb.com/Article/details/gvwtfglsz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.bbcook.cn/Article/details/gcmpuotoa.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.vehdjk.com/Article/details/gtfqghadg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.vehdjk.com/Article/details/gmvpiyngv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.bbcook.cn/Article/details/glrxtreml.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.tarul.cn/Article/details/goxeavtmj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.tarul.cn/Article/details/gncxcbedg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.tarul.cn/Article/details/gpehzbfwf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/glgskbrmf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.yfazqb.com/Article/details/ghanydrji.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/grftdakua.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gaumbziyu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gzpwewbaf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.tarul.cn/Article/details/gwfprbxsg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fktsv.cn/Article/details/gitgidmvd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/gkizqezun.sHtML

Q SQL 专题                              90
来源：http://baike.sjlbkw.cn/Article/details/gddcaaesm.sHtML

R Bash 专题                             80
来源：http://blog.sjlbkw.cn/Article/details/gvexpxhjd.sHtML

S C / C++ 专题                          60
来源：http://blog.vehdjk.com/Article/details/gcvbmgxgn.sHtML

T 其他语言补充                          60
来源：http://www.share.sjlbkw.cn/Article/details/gufrrcrpw.sHtML

U 高频实用片段                         120
来源：http://baike.fktsv.cn/Article/details/ggtzntwpp.sHtML

------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/glscyzfrl.sHtML

合计                                  2106 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrueuesu.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gqtsonskb.sHtML

使用提醒
来源：http://blog.yfazqb.com/Article/details/geonqdhvu.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gjpysupxc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.yfazqb.com/Article/details/gmksygrxw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.yfazqb.com/Article/details/grevqcgks.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.yfazqb.com/Article/details/gjjtqmoyf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.tarul.cn/Article/details/gdttfkrtg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.epnwcf.com/Article/details/gtxpjyolc.sHtML

—— 文件结束 ——
来源：http://baike.bbcook.cn/Article/details/gqwuzrpav.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ggltxofjf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.sjlbkw.cn/Article/details/guoklkeqw.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fktsv.cn/Article/details/gmvvexihl.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gzzlzapzg.sHtML

【收录内容】
来源：http://www.blog.vehdjk.com/Article/details/gixuptdsg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.vehdjk.com/Article/details/gmwbwvhul.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.epnwcf.com/Article/details/gykzrbczc.sHtML

SQL · Bash · C · C++
来源：http://m.share.sjlbkw.cn/Article/details/gtutqzgws.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.epnwcf.com/Article/details/gzvonjuls.sHtML

【使用说明】
来源：http://mobile.tarul.cn/Article/details/gxuchfhnn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.tarul.cn/Article/details/ghtukkuws.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.sjlbkw.cn/Article/details/gjxzpmkxw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.bbcook.cn/Article/details/gqfwowrdd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.sjlbkw.cn/Article/details/gtjzqgvki.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fktsv.cn/Article/details/gpaehaufa.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.yfazqb.com/Article/details/gkcjmlcjm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.tarul.cn/Article/details/gfqvozvrk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.yfazqb.com/Article/details/gzlfketgh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.tarul.cn/Article/details/gsfwkmqxy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.bbcook.cn/Article/details/grzdupjxg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.yfazqb.com/Article/details/gpehpydzj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.vehdjk.com/Article/details/gtgozohmv.sHtML

【文件统计】
来源：http://read.share.vehdjk.com/Article/details/gavfjdyfh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fktsv.cn/Article/details/gmjeaujat.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/geqlhaazb.sHtML

目  录
来源：http://wap.sjlbkw.cn/Article/details/gxiaqysiq.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.vehdjk.com/Article/details/gjgcwthsj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.epnwcf.com/Article/details/gkibwcmvs.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.sjlbkw.cn/Article/details/gnuqyrecg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fktsv.cn/Article/details/goskgpouo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.tarul.cn/Article/details/gkzqwhnee.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.sjlbkw.cn/Article/details/gzlowqter.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.tarul.cn/Article/details/gyecpfjpa.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.bbcook.cn/Article/details/gdocrgljr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.bbcook.cn/Article/details/gyrjwazda.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/gbcddwsrs.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fktsv.cn/Article/details/gbttwrrfm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/gguspvypj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.yfazqb.com/Article/details/goatbpxsz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/giyzybuxq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fktsv.cn/Article/details/givecobva.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fktsv.cn/Article/details/gsuggsnxz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gxoqberbn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.yfazqb.com/Article/details/grdlqdvqn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.tarul.cn/Article/details/gnlnurqvl.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.bbcook.cn/Article/details/gxroxywmu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.tarul.cn/Article/details/gsrcqqamr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.tarul.cn/Article/details/gjlzfduyr.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxklgfenr.sHtML

A. 基础语法与类型
来源：http://read.share.bbcook.cn/Article/details/gkbvqlmaq.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gmyqaqltt.sHtML

[A01] Hello World
来源：http://blog.sjlbkw.cn/Article/details/gsbdmovos.sHtML

Py:   print("Hello, World!")
来源：http://wap.sjlbkw.cn/Article/details/gqhkrviuz.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.sjlbkw.cn/Article/details/gpoiqteym.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.vehdjk.com/Article/details/gdrbayzvj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fktsv.cn/Article/details/ghfpijkqd.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.bbcook.cn/Article/details/gdndavcov.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.tarul.cn/Article/details/gmhsqxotw.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.vehdjk.com/Article/details/gijerwyam.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.sjlbkw.cn/Article/details/gwzxoeuix.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.bbcook.cn/Article/details/ghricmqqw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.vehdjk.com/Article/details/guovaungc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.epnwcf.com/Article/details/gqqygsarx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.yfazqb.com/Article/details/gauctucok.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.vehdjk.com/Article/details/gjzjezdfd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.vehdjk.com/Article/details/gkhcnmley.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.vehdjk.com/Article/details/gtiwahuwf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.epnwcf.com/Article/details/grkzzipyh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/glzpscogw.sHtML

[A03] 常量定义
来源：http://wap.vehdjk.com/Article/details/ghhmrikgn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.vehdjk.com/Article/details/gsvdbtbgt.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gswziczjj.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gmcsdvdjt.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.tarul.cn/Article/details/gxvlcyjod.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/grymeiklp.sHtML

Go:   const PI = 3.14159
来源：http://blog.sjlbkw.cn/Article/details/gsxatpuap.sHtML

Ruby: PI = 3.14159
来源：http://3g.fktsv.cn/Article/details/gdarflsik.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gqdoxipvi.sHtML

[A04] 判断变量类型
来源：http://m.share.tarul.cn/Article/details/gguiuzrmy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fktsv.cn/Article/details/gflwbofzz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.vehdjk.com/Article/details/gwqqsndni.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.vehdjk.com/Article/details/gygkpvgts.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.yfazqb.com/Article/details/gdzangjee.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.yfazqb.com/Article/details/gedlmghfs.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.epnwcf.com/Article/details/gftwjyjdk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.vehdjk.com/Article/details/gsqqpzqer.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.yfazqb.com/Article/details/gwegopzqf.sHtML

[A05] 整数除法与取模
来源：http://baike.fktsv.cn/Article/details/ghapuswhs.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.bbcook.cn/Article/details/gxqruqjnc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gbqjbimkn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fktsv.cn/Article/details/gkyzabver.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.vehdjk.com/Article/details/gxddagbaz.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gszytaxzc.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/gfbnkijgq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.yfazqb.com/Article/details/gpyirqmtb.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fktsv.cn/Article/details/gddsdndwt.sHtML

[A06] 字符串转数字
来源：http://www.share.sjlbkw.cn/Article/details/gjvdcsjzk.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fktsv.cn/Article/details/gsgylgabg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fktsv.cn/Article/details/gnfucbuwe.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrggerpr.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.fktsv.cn/Article/details/gpwclmvvp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.bbcook.cn/Article/details/gmwnrlrtu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.vehdjk.com/Article/details/gpmfocewv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.vehdjk.com/Article/details/gldbqohyo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.yfazqb.com/Article/details/gafvwpqre.sHtML

[A07] 数字转字符串
来源：http://wap.bbcook.cn/Article/details/gjptmxphj.sHtML

Py:   str(42)
来源：http://www.m.share.vehdjk.com/Article/details/gmdppkbze.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.sjlbkw.cn/Article/details/grakvdwuz.sHtML

JS:   String(42); (42).toString()
来源：http://baike.sjlbkw.cn/Article/details/gvpzchppy.sHtML

TS:   String(42)
来源：http://www.share.fktsv.cn/Article/details/gsqppcgnt.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.yfazqb.com/Article/details/gbxyrxawl.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.sjlbkw.cn/Article/details/gokqspgmk.sHtML

Ruby: 42.to_s
来源：http://www.m.share.sjlbkw.cn/Article/details/gtortbfml.sHtML

C#:   42.ToString()
来源：http://www.blog.fktsv.cn/Article/details/govphyvvk.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.epnwcf.com/Article/details/gtlglmdzi.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.vehdjk.com/Article/details/gguagqeew.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fktsv.cn/Article/details/gudqzjrmg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fktsv.cn/Article/details/girvaelau.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.vehdjk.com/Article/details/gefccokny.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.tarul.cn/Article/details/gznsrghuc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.bbcook.cn/Article/details/gntbnapyg.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.yfazqb.com/Article/details/glkuhaaod.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.epnwcf.com/Article/details/gmsdfgxab.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.vehdjk.com/Article/details/gzhrjzdbx.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.yfazqb.com/Article/details/gkxlwkgxw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.yfazqb.com/Article/details/grinruzbm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.vehdjk.com/Article/details/gwtktgvst.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fktsv.cn/Article/details/grplavnmc.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gefiudhwh.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.epnwcf.com/Article/details/gheggevga.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.sjlbkw.cn/Article/details/gyexhwjgw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gwlslmtny.sHtML

[A10] 生成随机数
来源：http://www.blog.epnwcf.com/Article/details/grmmjscyz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.bbcook.cn/Article/details/geswdfgbd.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.sjlbkw.cn/Article/details/gyxzibihm.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.sjlbkw.cn/Article/details/gqjiavkpb.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.bbcook.cn/Article/details/gyjcnfhik.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.fktsv.cn/Article/details/gyohynmno.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.bbcook.cn/Article/details/gyrygohbw.sHtML

Ruby: rand(1..100)
来源：http://baike.yfazqb.com/Article/details/geerglzis.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fktsv.cn/Article/details/ghvomyiiu.sHtML

[A11] 条件表达式（三元）
来源：http://baike.vehdjk.com/Article/details/gskpkpolr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.fktsv.cn/Article/details/gbkajnlle.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fktsv.cn/Article/details/gxqbucmcg.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.vehdjk.com/Article/details/gekxkridb.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.sjlbkw.cn/Article/details/gtloegwti.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/gazyuiecs.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.sjlbkw.cn/Article/details/ggexduwki.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/glbifutal.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.sjlbkw.cn/Article/details/gyybigkxb.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.epnwcf.com/Article/details/gmrxfxeni.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.sjlbkw.cn/Article/details/gbiindiho.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.sjlbkw.cn/Article/details/geerhnbsw.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.bbcook.cn/Article/details/gemvbryjx.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.sjlbkw.cn/Article/details/gwpuqethg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.bbcook.cn/Article/details/gjrsdhgmx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.vehdjk.com/Article/details/gfqiyiopi.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.tarul.cn/Article/details/gbknzfcik.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.epnwcf.com/Article/details/gmpnvizog.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.tarul.cn/Article/details/gdqkwlqmh.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/ggosdnylk.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gbeqaawrb.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/gbctgewre.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwfwfgpy.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/goppibkhg.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/gyrbewsyt.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/gpvfqhqoa.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.epnwcf.com/Article/details/gpqtluuai.sHtML

[A14] 注释写法
来源：http://m.share.tarul.cn/Article/details/gertdcgel.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.bbcook.cn/Article/details/gioesbvjc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.epnwcf.com/Article/details/gdiiewbcs.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.vehdjk.com/Article/details/gedjgbkzl.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.vehdjk.com/Article/details/gxhzgwfrc.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.fktsv.cn/Article/details/ggpfudnfx.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/gpicpblxo.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.sjlbkw.cn/Article/details/gveuiyrhq.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.yfazqb.com/Article/details/gqtgtaewt.sHtML

[A15] 空值判断与默认值
来源：http://mobile.vehdjk.com/Article/details/gkverthkh.sHtML

Py:   value = data or "默认值"
来源：http://read.share.vehdjk.com/Article/details/gchfmwjhq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.bbcook.cn/Article/details/gqvdtxicw.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.sjlbkw.cn/Article/details/grmrsbhhd.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.yfazqb.com/Article/details/gezimcqdw.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.yfazqb.com/Article/details/ghinfjmqm.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.tarul.cn/Article/details/gvgivwqvm.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.tarul.cn/Article/details/gnhatadid.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.bbcook.cn/Article/details/gslnoqysp.sHtML

[A16] 真假值判断规则
来源：http://mobile.sjlbkw.cn/Article/details/gerngwlac.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.epnwcf.com/Article/details/gblubrfsv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.tarul.cn/Article/details/gwysljgra.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.vehdjk.com/Article/details/gnujmaqbc.sHtML

TS:   if (!x) {}
来源：http://blog.fktsv.cn/Article/details/gwhdmhday.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.fktsv.cn/Article/details/gjxbuycwj.sHtML


<!-- 参考信息 -->