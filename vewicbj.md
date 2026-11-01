代发 wailian999

[U93] JS：模板字符串
来源：http://wap.bbcook.cn/Article/details/gvguindwj.sHtML

`共 ${n} 条`
来源：http://www.share.yfazqb.com/Article/details/gjxwowzgq.sHtML

[U94] JS：箭头函数
来源：http://mobile.sjlbkw.cn/Article/details/gfruhkqks.sHtML

const double = x => x * 2;
来源：http://www.blog.tarul.cn/Article/details/gmkgguwzp.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.epnwcf.com/Article/details/gnvypxypw.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.bbcook.cn/Article/details/gwomdpngh.sHtML

[U96] JS：async/await 与异常
来源：http://3g.tarul.cn/Article/details/ghufidlxu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/gauxcggjc.sHtML

[U97] JS：并发请求
来源：http://wap.vehdjk.com/Article/details/gfjqrnfje.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gutyvzvod.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fktsv.cn/Article/details/gstbaagay.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.bbcook.cn/Article/details/gzwgorobu.sHtML

[U99] JS：事件监听
来源：http://mobile.fktsv.cn/Article/details/geqbrkori.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.tarul.cn/Article/details/gwmajajyb.sHtML

[U100] JS：DOM 查询
来源：http://read.share.yfazqb.com/Article/details/galwynvuf.sHtML

document.querySelector(".item")
来源：http://m.share.fktsv.cn/Article/details/gilqozkqv.sHtML

[U101] JS：classList 操作
来源：http://wap.vehdjk.com/Article/details/gbyenrrjk.sHtML

el.classList.toggle("active")
来源：http://wap.vehdjk.com/Article/details/glhwfexcm.sHtML

[U102] JS：本地存储
来源：http://read.share.fktsv.cn/Article/details/gtqszuvmx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.yfazqb.com/Article/details/gshfmurnt.sHtML

[U103] JS：定时器
来源：http://m.share.vehdjk.com/Article/details/grungsxxp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fktsv.cn/Article/details/gfdctaust.sHtML

[U104] JS：防抖
来源：http://blog.fktsv.cn/Article/details/gaezrglpz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gqjfdbqgk.sHtML

[U105] JS：节流
来源：http://3g.sjlbkw.cn/Article/details/ggcwhitrq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gujlxrike.sHtML

[U106] JS：日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gdnqpnsaq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.bbcook.cn/Article/details/ghsqsyezd.sHtML

[U107] JS：数字千分位
来源：http://www.blog.epnwcf.com/Article/details/gxdyfvzuj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.yfazqb.com/Article/details/gyzxwbefb.sHtML

[U108] JS：随机整数
来源：http://baike.yfazqb.com/Article/details/gcpkfycit.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.yfazqb.com/Article/details/gflujxrna.sHtML

[U109] JS：数组分组
来源：http://read.share.sjlbkw.cn/Article/details/ghjfqkuzm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.sjlbkw.cn/Article/details/gaavhprge.sHtML

[U110] JS：数组分块
来源：http://blog.fktsv.cn/Article/details/gitifjjgn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.tarul.cn/Article/details/geafcatsk.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.yfazqb.com/Article/details/gaqidfcjb.sHtML

new Map(Object.entries(obj))
来源：http://mobile.bbcook.cn/Article/details/ghczlopch.sHtML

[U112] JS：字符串补位
来源：http://wap.yfazqb.com/Article/details/gsvyrvhxu.sHtML

"7".padStart(3, "0")
来源：http://blog.vehdjk.com/Article/details/gaskktfdl.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.vehdjk.com/Article/details/gewbdmnce.sHtML

s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/gpwovgtwv.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fktsv.cn/Article/details/gvhumyzzz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/gnehofzhf.sHtML

[U115] JS：生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/gtlldglmh.sHtML

crypto.randomUUID()
来源：http://3g.tarul.cn/Article/details/gctwdkzgl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fktsv.cn/Article/details/goithkfqr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.tarul.cn/Article/details/gmamfiksx.sHtML

[U117] JS：单元测试
来源：http://read.share.bbcook.cn/Article/details/gkxsrpdaq.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fktsv.cn/Article/details/gfwtuukxb.sHtML

[U118] JS：开发服务器
来源：http://www.blog.vehdjk.com/Article/details/gmcgxbsdj.sHtML

npm i -D vite;  npx vite
来源：http://www.share.yfazqb.com/Article/details/gcdsuyifc.sHtML

[U119] JS：生产构建
来源：http://www.share.vehdjk.com/Article/details/gistdxeie.sHtML

npx vite build
来源：http://3g.sjlbkw.cn/Article/details/gjhnnzzmi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.vehdjk.com/Article/details/gkrfevnvz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.bbcook.cn/Article/details/giojughts.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gvwzlwxmm.sHtML

统计汇总
来源：http://mobile.vehdjk.com/Article/details/gxzvmfzdm.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gbqehsikc.sHtML

按语言统计（条）：
来源：http://read.share.yfazqb.com/Article/details/gdtakfyps.sHtML

Python ......... 252
来源：http://read.share.fktsv.cn/Article/details/gnocbvdff.sHtML

PHP ............ 252
来源：http://mobile.yfazqb.com/Article/details/goicajfhy.sHtML

JavaScript ..... 252
来源：http://www.blog.sjlbkw.cn/Article/details/gvjisxnej.sHtML

TypeScript ..... 212
来源：http://www.blog.epnwcf.com/Article/details/gohnxhtpc.sHtML

Java ........... 212
来源：http://baike.bbcook.cn/Article/details/gazmrxcju.sHtML

Go ............. 212
来源：http://mobile.yfazqb.com/Article/details/ggliranfz.sHtML

Ruby ........... 212
来源：http://baike.sjlbkw.cn/Article/details/goqlmslgj.sHtML

C# ............. 212
来源：http://m.share.sjlbkw.cn/Article/details/gdfdwoayk.sHtML

C .............. 30
来源：http://baike.bbcook.cn/Article/details/gioneijuq.sHtML

C++ ............ 30
来源：http://3g.tarul.cn/Article/details/gjwrmeysy.sHtML

SQL ............ 90
来源：http://wap.yfazqb.com/Article/details/gdbhodfns.sHtML

Bash ........... 80
来源：http://m.share.sjlbkw.cn/Article/details/gezwhknxx.sHtML

Kotlin ......... 15
来源：http://3g.bbcook.cn/Article/details/gifjrisww.sHtML

Swift .......... 15
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpreiekv.sHtML

Lua ............ 10
来源：http://baike.vehdjk.com/Article/details/gdaezqpcz.sHtML

Perl ........... 10
来源：http://3g.epnwcf.com/Article/details/gpeopvvzs.sHtML

Scala .......... 10
来源：http://3g.sjlbkw.cn/Article/details/gbqpwyzdv.sHtML

------------------------------------
来源：http://m.share.bbcook.cn/Article/details/guoxgnsph.sHtML

合计 ........... 2106 条
来源：http://mobile.vehdjk.com/Article/details/gbbijtepz.sHtML

按章节统计：
来源：http://m.share.yfazqb.com/Article/details/gxgaoxyus.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.tarul.cn/Article/details/gursqouoe.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fktsv.cn/Article/details/gbqlvymtw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.yfazqb.com/Article/details/gutzfgjlo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.epnwcf.com/Article/details/gkrqfijek.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.bbcook.cn/Article/details/gufuzpykx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.yfazqb.com/Article/details/gxftxsofi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.epnwcf.com/Article/details/gylelybkv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.tarul.cn/Article/details/gwdwaviho.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/godkcbgmw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.epnwcf.com/Article/details/gofrjtxhu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/grdekolbm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/gujeydazh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gtomcqgfw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fktsv.cn/Article/details/gnfhbrclf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.vehdjk.com/Article/details/giuiesefl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gwwnwrvbi.sHtML

Q SQL 专题                              90
来源：http://www.share.epnwcf.com/Article/details/gfgqpsbkc.sHtML

R Bash 专题                             80
来源：http://3g.bbcook.cn/Article/details/gnyuvctay.sHtML

S C / C++ 专题                          60
来源：http://www.share.fktsv.cn/Article/details/gxzmqwnjo.sHtML

T 其他语言补充                          60
来源：http://baike.bbcook.cn/Article/details/gvbzeuwpv.sHtML

U 高频实用片段                         120
来源：http://3g.epnwcf.com/Article/details/gwpasgbhm.sHtML

------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gexrlyzzz.sHtML

合计                                  2106 条
来源：http://www.m.share.bbcook.cn/Article/details/gnjbjiyvk.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/glktkikuy.sHtML

使用提醒
来源：http://m.share.tarul.cn/Article/details/gcciwoiuw.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/gvmvmfbvr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.tarul.cn/Article/details/gnqmzkjgk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.yfazqb.com/Article/details/gvhqrnbph.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.yfazqb.com/Article/details/gbgsqmcqn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.epnwcf.com/Article/details/gqkjgckis.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.vehdjk.com/Article/details/gqzhktekz.sHtML

—— 文件结束 ——
来源：http://read.share.vehdjk.com/Article/details/gqlpnsqgs.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gnoyviblb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.bbcook.cn/Article/details/glahukass.sHtML

Common Programming Examples Cheat Book
来源：http://baike.yfazqb.com/Article/details/gnauqdxpr.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gwtphtstt.sHtML

【收录内容】
来源：http://wap.sjlbkw.cn/Article/details/gagvkypur.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.yfazqb.com/Article/details/gnalrlbun.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.epnwcf.com/Article/details/gnwjvqszc.sHtML

SQL · Bash · C · C++
来源：http://www.blog.yfazqb.com/Article/details/gcjnjklpy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.epnwcf.com/Article/details/gabsjlrho.sHtML

【使用说明】
来源：http://www.share.fktsv.cn/Article/details/gnalnplxi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.tarul.cn/Article/details/gupuxmsjf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.yfazqb.com/Article/details/gifpmafmd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.bbcook.cn/Article/details/ggnpelkob.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.yfazqb.com/Article/details/gadbroxzp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.tarul.cn/Article/details/gypxqanvo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.tarul.cn/Article/details/ghlktvnqt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.bbcook.cn/Article/details/gaeqzwxee.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.bbcook.cn/Article/details/gyljsmzzj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.yfazqb.com/Article/details/gcwdsuavi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.bbcook.cn/Article/details/giqlxjlxz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.tarul.cn/Article/details/gahjxvfhw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.bbcook.cn/Article/details/glwdmxpcn.sHtML

【文件统计】
来源：http://m.share.fktsv.cn/Article/details/gkjpasufa.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.tarul.cn/Article/details/ghlqyhkzf.sHtML

--------------------------------------------------------------------------------
来源：http://3g.bbcook.cn/Article/details/gwenlhoaf.sHtML

目  录
来源：http://baike.vehdjk.com/Article/details/gxepuaugw.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gksftatza.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.sjlbkw.cn/Article/details/gtowcdmaa.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.sjlbkw.cn/Article/details/gewlbapvk.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.bbcook.cn/Article/details/gkgdelkrc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.epnwcf.com/Article/details/gxmzgvjqc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.epnwcf.com/Article/details/gmsgrsbck.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fktsv.cn/Article/details/gipaacguf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/gdomoetia.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.epnwcf.com/Article/details/gzecldmsx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.vehdjk.com/Article/details/gcsztztwe.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.yfazqb.com/Article/details/gjsjsxquq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.bbcook.cn/Article/details/gewgvdvxg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.sjlbkw.cn/Article/details/gkdpoytdg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/gkfnvbuxm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fktsv.cn/Article/details/gahjuxjfy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.yfazqb.com/Article/details/gowuurkmf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gzeacpfkl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.sjlbkw.cn/Article/details/gtireowqn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.tarul.cn/Article/details/gcyagvvmr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.tarul.cn/Article/details/gmiawwbio.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.bbcook.cn/Article/details/gmtlanksu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.vehdjk.com/Article/details/gjnynxzkv.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gcozgixul.sHtML

A. 基础语法与类型
来源：http://3g.tarul.cn/Article/details/gfsyzynwh.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gkxlssfpw.sHtML

[A01] Hello World
来源：http://mobile.yfazqb.com/Article/details/gnbfbmwrs.sHtML

Py:   print("Hello, World!")
来源：http://3g.bbcook.cn/Article/details/gesfqmecq.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.vehdjk.com/Article/details/gioqpynez.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.tarul.cn/Article/details/gbmlqtasz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.yfazqb.com/Article/details/gneniuvcj.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.tarul.cn/Article/details/gppocyigi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.tarul.cn/Article/details/gpyerrwtq.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.vehdjk.com/Article/details/gavhpwmeb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.bbcook.cn/Article/details/gpowvxbwx.sHtML

[A02] 变量声明与赋值
来源：http://wap.fktsv.cn/Article/details/gbyaowfkd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fktsv.cn/Article/details/gtwvfihws.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fktsv.cn/Article/details/grhxzdzvh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.bbcook.cn/Article/details/gbkkxyqvq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.vehdjk.com/Article/details/gzuyzgfhn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.sjlbkw.cn/Article/details/giknwkidg.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.yfazqb.com/Article/details/gloijydch.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.tarul.cn/Article/details/gyeafwfpv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.tarul.cn/Article/details/gvziplzba.sHtML

[A03] 常量定义
来源：http://blog.vehdjk.com/Article/details/gfbymldgb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.epnwcf.com/Article/details/gkvwddldh.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gncvpzdtr.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/ggpbnxvrm.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gfxoiedmd.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gvidokjaq.sHtML

Go:   const PI = 3.14159
来源：http://www.share.yfazqb.com/Article/details/gacmcwdol.sHtML

Ruby: PI = 3.14159
来源：http://baike.epnwcf.com/Article/details/goyiiwged.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gfuqwzutz.sHtML

[A04] 判断变量类型
来源：http://mobile.tarul.cn/Article/details/ggxrzpbqt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.bbcook.cn/Article/details/gkiovmbxo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.vehdjk.com/Article/details/gabgypakf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.vehdjk.com/Article/details/gphqatsmk.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.epnwcf.com/Article/details/gcjlbeddn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.yfazqb.com/Article/details/ghrhribjc.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.vehdjk.com/Article/details/gdzhclbke.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.vehdjk.com/Article/details/gkavditzi.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.sjlbkw.cn/Article/details/gfpkpglol.sHtML

[A05] 整数除法与取模
来源：http://www.share.fktsv.cn/Article/details/glrgrdotq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fktsv.cn/Article/details/ggkufvecm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/gbgoojgqc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.epnwcf.com/Article/details/gffptzict.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.yfazqb.com/Article/details/gpcjtpkqa.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gscjsxahm.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/gaxjlyuzw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fktsv.cn/Article/details/gvupsctuw.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.epnwcf.com/Article/details/gbklzudrm.sHtML

[A06] 字符串转数字
来源：http://www.blog.sjlbkw.cn/Article/details/gqftwinmc.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fktsv.cn/Article/details/gvxyucbfu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.tarul.cn/Article/details/ggmzildgz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.tarul.cn/Article/details/ghmiyjhuo.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.yfazqb.com/Article/details/gydgcqyia.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.yfazqb.com/Article/details/govrxezwe.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fktsv.cn/Article/details/gdybndlpk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fktsv.cn/Article/details/gbtrvgfnf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.epnwcf.com/Article/details/gcydelfrz.sHtML

[A07] 数字转字符串
来源：http://m.share.fktsv.cn/Article/details/gvopcptme.sHtML

Py:   str(42)
来源：http://mobile.tarul.cn/Article/details/gvqnjqijz.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.sjlbkw.cn/Article/details/gkbuvlfbu.sHtML

JS:   String(42); (42).toString()
来源：http://wap.yfazqb.com/Article/details/gkfyneajn.sHtML

TS:   String(42)
来源：http://www.blog.tarul.cn/Article/details/gcxjjsbrr.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fktsv.cn/Article/details/gdvkkkhnh.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.epnwcf.com/Article/details/ghowcqwaw.sHtML

Ruby: 42.to_s
来源：http://mobile.tarul.cn/Article/details/gfkhclwrv.sHtML

C#:   42.ToString()
来源：http://wap.vehdjk.com/Article/details/gvfjeodsx.sHtML

[A08] 取整与四舍五入
来源：http://blog.yfazqb.com/Article/details/gapzssgno.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fktsv.cn/Article/details/ggrigrqod.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fktsv.cn/Article/details/gbtogovcj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fktsv.cn/Article/details/gpapdspke.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.vehdjk.com/Article/details/gwpnzexcf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.sjlbkw.cn/Article/details/gfgunqsfk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.epnwcf.com/Article/details/glzxmpaqg.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fktsv.cn/Article/details/grvmeqcyy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.epnwcf.com/Article/details/gisqajvdc.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.yfazqb.com/Article/details/gkwfttsit.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fktsv.cn/Article/details/gpddsaofv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fktsv.cn/Article/details/glmucnovm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.tarul.cn/Article/details/gkygtdfxz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.epnwcf.com/Article/details/gzivqtnso.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/ginxqabdq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.bbcook.cn/Article/details/gjolurhjn.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.vehdjk.com/Article/details/ghbdmqfzm.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gbyvuleot.sHtML

[A10] 生成随机数
来源：http://baike.vehdjk.com/Article/details/gnagqjsnm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.epnwcf.com/Article/details/ggtpyxtoz.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.epnwcf.com/Article/details/gryhggluk.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.sjlbkw.cn/Article/details/grahedgwr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fktsv.cn/Article/details/giufibahx.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.bbcook.cn/Article/details/gjaiakcog.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.sjlbkw.cn/Article/details/gsgwwufry.sHtML

Ruby: rand(1..100)
来源：http://baike.sjlbkw.cn/Article/details/glfnqkrcu.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.sjlbkw.cn/Article/details/grfoyjtrp.sHtML

[A11] 条件表达式（三元）
来源：http://baike.fktsv.cn/Article/details/gtibllowu.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.yfazqb.com/Article/details/gxmhykcdm.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.sjlbkw.cn/Article/details/grvuualuc.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/gqwuyjaef.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.vehdjk.com/Article/details/gfukkpxjw.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.yfazqb.com/Article/details/ghbwbgvzl.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.epnwcf.com/Article/details/gfwlvkptt.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gygnbsvrg.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.bbcook.cn/Article/details/gmsunanyl.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fktsv.cn/Article/details/gvxjeljbe.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.bbcook.cn/Article/details/gjajzvwdi.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.epnwcf.com/Article/details/gbfcbedbr.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.fktsv.cn/Article/details/gmxvkaqcw.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.sjlbkw.cn/Article/details/gxlnlaxpw.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.yfazqb.com/Article/details/gsxnibhej.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.fktsv.cn/Article/details/gynoaaeip.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.yfazqb.com/Article/details/gthjmhzbm.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.sjlbkw.cn/Article/details/gtagtcnjx.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.epnwcf.com/Article/details/gsisdbfbb.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gnhsahwos.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gwqtyyipl.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/gnadudaul.sHtML

TS:   "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/gzintopbr.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.epnwcf.com/Article/details/gzfothsnr.sHtML

Go:   "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/giynytijq.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gbvxcvlti.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fktsv.cn/Article/details/gtmlnkvdz.sHtML

[A14] 注释写法
来源：http://www.m.share.epnwcf.com/Article/details/gwvlxaqqb.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.epnwcf.com/Article/details/gcdlqaiia.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.tarul.cn/Article/details/gznkgrdtr.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fktsv.cn/Article/details/gjhcxreoh.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.yfazqb.com/Article/details/gevamtxfx.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.vehdjk.com/Article/details/gzriwubyg.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.yfazqb.com/Article/details/ggtzhcxfu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.vehdjk.com/Article/details/godhhxtku.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.tarul.cn/Article/details/gejfltqez.sHtML

[A15] 空值判断与默认值
来源：http://read.share.sjlbkw.cn/Article/details/gspaeqdvm.sHtML

Py:   value = data or "默认值"
来源：http://baike.bbcook.cn/Article/details/gmkwnatsp.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvkmxyrg.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.yfazqb.com/Article/details/gludahmqx.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fktsv.cn/Article/details/gnetacyii.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.yfazqb.com/Article/details/gzrwcnfis.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.epnwcf.com/Article/details/gocwxcwrs.sHtML

Ruby: value = data || "默认值"
来源：http://3g.epnwcf.com/Article/details/gegcnyxyo.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.bbcook.cn/Article/details/gubkercnm.sHtML

[A16] 真假值判断规则
来源：http://wap.sjlbkw.cn/Article/details/gzcbgfsuz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.sjlbkw.cn/Article/details/gcedmeoim.sHtML


<!-- 参考信息 -->