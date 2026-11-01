代发 wailian999

[U95] JS：Promise 包装
来源：http://m.share.epnwcf.com/Article/details/gxwqcdoot.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.yfazqb.com/Article/details/gpjgmdxtb.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fktsv.cn/Article/details/ghcwhgtls.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/gxhqsbguf.sHtML

[U97] JS：并发请求
来源：http://wap.bbcook.cn/Article/details/gabigxtic.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/gvexbjehv.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fktsv.cn/Article/details/gtzhguqig.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.sjlbkw.cn/Article/details/gdwlgqrcf.sHtML

[U99] JS：事件监听
来源：http://wap.fktsv.cn/Article/details/gpkgvvszs.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fktsv.cn/Article/details/gtotjulco.sHtML

[U100] JS：DOM 查询
来源：http://www.share.sjlbkw.cn/Article/details/gltykkfsu.sHtML

document.querySelector(".item")
来源：http://read.share.epnwcf.com/Article/details/gosfgkvlu.sHtML

[U101] JS：classList 操作
来源：http://www.share.tarul.cn/Article/details/genleogan.sHtML

el.classList.toggle("active")
来源：http://mobile.fktsv.cn/Article/details/gixjjvkme.sHtML

[U102] JS：本地存储
来源：http://baike.epnwcf.com/Article/details/goezlbuty.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.yfazqb.com/Article/details/gsblntlmm.sHtML

[U103] JS：定时器
来源：http://blog.yfazqb.com/Article/details/gurcmvvnx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.bbcook.cn/Article/details/gzspaudou.sHtML

[U104] JS：防抖
来源：http://read.share.yfazqb.com/Article/details/gpmmumkpu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/gvhbkdpbt.sHtML

[U105] JS：节流
来源：http://mobile.sjlbkw.cn/Article/details/gqeoaylya.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.epnwcf.com/Article/details/gljzznjll.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.epnwcf.com/Article/details/gbmzwsopb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.epnwcf.com/Article/details/gndlukogh.sHtML

[U107] JS：数字千分位
来源：http://www.blog.vehdjk.com/Article/details/gleinaoza.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.yfazqb.com/Article/details/gahnxhsjj.sHtML

[U108] JS：随机整数
来源：http://m.share.tarul.cn/Article/details/gkepytxrk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.bbcook.cn/Article/details/gsbguvtny.sHtML

[U109] JS：数组分组
来源：http://3g.epnwcf.com/Article/details/gzydeexrr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.bbcook.cn/Article/details/ggplpatrn.sHtML

[U110] JS：数组分块
来源：http://www.share.vehdjk.com/Article/details/gdttjyfwq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.sjlbkw.cn/Article/details/gtzfdntvf.sHtML

[U111] JS：对象转 Map
来源：http://3g.fktsv.cn/Article/details/gouhedlvh.sHtML

new Map(Object.entries(obj))
来源：http://3g.tarul.cn/Article/details/gyeehrzay.sHtML

[U112] JS：字符串补位
来源：http://read.share.sjlbkw.cn/Article/details/gthfkefqm.sHtML

"7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/ghitpkaun.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fktsv.cn/Article/details/gjjiubemm.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gtqadzspc.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.epnwcf.com/Article/details/gymngxlre.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.bbcook.cn/Article/details/gubfvedgu.sHtML

[U115] JS：生成 UUID
来源：http://read.share.vehdjk.com/Article/details/gozmiwylx.sHtML

crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/gegaqvkrc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fktsv.cn/Article/details/gxejgwrxq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fktsv.cn/Article/details/gpxnkqyjp.sHtML

[U117] JS：单元测试
来源：http://www.m.share.vehdjk.com/Article/details/gzvjoyihq.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.sjlbkw.cn/Article/details/gayiqwbfa.sHtML

[U118] JS：开发服务器
来源：http://baike.bbcook.cn/Article/details/gmhjhhjzk.sHtML

npm i -D vite;  npx vite
来源：http://wap.bbcook.cn/Article/details/gvccbwlfx.sHtML

[U119] JS：生产构建
来源：http://www.blog.tarul.cn/Article/details/gauqlxnsy.sHtML

npx vite build
来源：http://read.share.vehdjk.com/Article/details/gmhpvdhlw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.sjlbkw.cn/Article/details/gmoutohlg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.tarul.cn/Article/details/grjusjuye.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/girqedvsc.sHtML

统计汇总
来源：http://read.share.sjlbkw.cn/Article/details/gidmqhufx.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gxshhwuri.sHtML

按语言统计（条）：
来源：http://wap.tarul.cn/Article/details/gdbyxefyp.sHtML

Python ......... 252
来源：http://read.share.vehdjk.com/Article/details/gtcoeljmc.sHtML

PHP ............ 252
来源：http://read.share.tarul.cn/Article/details/gudjutvim.sHtML

JavaScript ..... 252
来源：http://read.share.sjlbkw.cn/Article/details/gdfuevwps.sHtML

TypeScript ..... 212
来源：http://www.m.share.yfazqb.com/Article/details/gmsgsbeqp.sHtML

Java ........... 212
来源：http://baike.bbcook.cn/Article/details/gplqsdzjy.sHtML

Go ............. 212
来源：http://baike.bbcook.cn/Article/details/gczojzwyr.sHtML

Ruby ........... 212
来源：http://www.m.share.fktsv.cn/Article/details/goyvtymfl.sHtML

C# ............. 212
来源：http://www.blog.yfazqb.com/Article/details/gxhgzumhr.sHtML

C .............. 30
来源：http://www.m.share.tarul.cn/Article/details/gdkamlafr.sHtML

C++ ............ 30
来源：http://wap.yfazqb.com/Article/details/glzmsrzgo.sHtML

SQL ............ 90
来源：http://blog.vehdjk.com/Article/details/gkposiyss.sHtML

Bash ........... 80
来源：http://m.share.sjlbkw.cn/Article/details/gyordpzjn.sHtML

Kotlin ......... 15
来源：http://read.share.sjlbkw.cn/Article/details/gwogcpxnz.sHtML

Swift .......... 15
来源：http://m.share.vehdjk.com/Article/details/ghnezfhyu.sHtML

Lua ............ 10
来源：http://wap.yfazqb.com/Article/details/gtayuivgb.sHtML

Perl ........... 10
来源：http://read.share.yfazqb.com/Article/details/gcyxvqcwd.sHtML

Scala .......... 10
来源：http://blog.fktsv.cn/Article/details/gwxwlsigf.sHtML

------------------------------------
来源：http://m.share.vehdjk.com/Article/details/gjvyqirex.sHtML

合计 ........... 2106 条
来源：http://read.share.bbcook.cn/Article/details/gtliijbwo.sHtML

按章节统计：
来源：http://mobile.epnwcf.com/Article/details/gtxcnbcvl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.tarul.cn/Article/details/gznszfiwg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.sjlbkw.cn/Article/details/gmfslchtf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.yfazqb.com/Article/details/gfavdjggd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.vehdjk.com/Article/details/gighqmpgx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.tarul.cn/Article/details/gegzfqaoi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.vehdjk.com/Article/details/ggusbwdsr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.epnwcf.com/Article/details/gwfxqybcl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.vehdjk.com/Article/details/glbdgfhrq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gjhydcvwz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.yfazqb.com/Article/details/gujkwzroe.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/gqzeincpm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/gxncocxoc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/gcbblahdt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.sjlbkw.cn/Article/details/gdouremou.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.bbcook.cn/Article/details/gogsdiqhm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/ghnfkturl.sHtML

Q SQL 专题                              90
来源：http://m.share.vehdjk.com/Article/details/gmxnwsocn.sHtML

R Bash 专题                             80
来源：http://blog.fktsv.cn/Article/details/gospmupta.sHtML

S C / C++ 专题                          60
来源：http://www.share.sjlbkw.cn/Article/details/gzdohzwud.sHtML

T 其他语言补充                          60
来源：http://mobile.vehdjk.com/Article/details/gxoqmmijx.sHtML

U 高频实用片段                         120
来源：http://baike.vehdjk.com/Article/details/glpvuavfy.sHtML

------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gootbokjs.sHtML

合计                                  2106 条
来源：http://wap.bbcook.cn/Article/details/gnqbypysm.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gkgcvffxs.sHtML

使用提醒
来源：http://wap.vehdjk.com/Article/details/ggjkavmsq.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gvyhrezve.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.vehdjk.com/Article/details/ggaixxfxk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.tarul.cn/Article/details/gtdyrwhvh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.bbcook.cn/Article/details/gkbawmaqt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fktsv.cn/Article/details/gkdkoexbi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.tarul.cn/Article/details/gvqbfpiaz.sHtML

—— 文件结束 ——
来源：http://www.share.yfazqb.com/Article/details/glyoifrkm.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/grnjljsyj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.epnwcf.com/Article/details/girawcvdb.sHtML

Common Programming Examples Cheat Book
来源：http://3g.sjlbkw.cn/Article/details/gmbqlywii.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gngrcssec.sHtML

【收录内容】
来源：http://www.share.fktsv.cn/Article/details/gsvsxkejj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fktsv.cn/Article/details/ggakrutpv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.yfazqb.com/Article/details/ggarnwbii.sHtML

SQL · Bash · C · C++
来源：http://read.share.epnwcf.com/Article/details/gvvqrziok.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.vehdjk.com/Article/details/gypoxfqsg.sHtML

【使用说明】
来源：http://www.share.yfazqb.com/Article/details/guwvhyvkk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.bbcook.cn/Article/details/gdppgyqol.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.vehdjk.com/Article/details/gpyonmoyx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.sjlbkw.cn/Article/details/ggdruhzpa.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.tarul.cn/Article/details/gfedmrhvb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.yfazqb.com/Article/details/glfzljycy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.sjlbkw.cn/Article/details/gatzwvouj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.vehdjk.com/Article/details/gjsblpcel.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.yfazqb.com/Article/details/grccqutih.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.vehdjk.com/Article/details/gtknulcxy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.sjlbkw.cn/Article/details/gzbjksrcq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.tarul.cn/Article/details/gihzxhzfd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.tarul.cn/Article/details/gipldhdvt.sHtML

【文件统计】
来源：http://baike.tarul.cn/Article/details/gqqxxgkjv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.epnwcf.com/Article/details/gamjybzfk.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gpzotufpc.sHtML

目  录
来源：http://baike.sjlbkw.cn/Article/details/gcbcvsifh.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.vehdjk.com/Article/details/gzyyjzfpi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.yfazqb.com/Article/details/ghmcsljsf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.bbcook.cn/Article/details/gesneajwa.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.vehdjk.com/Article/details/gzyzwzmxo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fktsv.cn/Article/details/gwsxfbmdw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fktsv.cn/Article/details/gtydmqitm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.vehdjk.com/Article/details/gxihjgvcn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.tarul.cn/Article/details/gpstyiwrq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.sjlbkw.cn/Article/details/gycrbpihp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/ggjpildrc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.tarul.cn/Article/details/gzzcukcgh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.sjlbkw.cn/Article/details/ghcyljxce.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.vehdjk.com/Article/details/gxqsjbdos.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.vehdjk.com/Article/details/gcdfavbsg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.bbcook.cn/Article/details/geuglxntb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fktsv.cn/Article/details/gjpmoievb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gwyuflydf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.tarul.cn/Article/details/ggojbprmy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.yfazqb.com/Article/details/gkrvrjkmr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.vehdjk.com/Article/details/gbkacfgtx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.bbcook.cn/Article/details/gfqdpltmt.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.sjlbkw.cn/Article/details/gysvjdiex.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gdiuvtblr.sHtML

A. 基础语法与类型
来源：http://www.blog.fktsv.cn/Article/details/gcejjynaa.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/givtbyhax.sHtML

[A01] Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gnszcfyjr.sHtML

Py:   print("Hello, World!")
来源：http://www.share.bbcook.cn/Article/details/gzfyhckjf.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.epnwcf.com/Article/details/gttpmuros.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.bbcook.cn/Article/details/gipwoaqjf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.bbcook.cn/Article/details/gfrkhjrfq.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.epnwcf.com/Article/details/gqedmhtfo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.yfazqb.com/Article/details/gzurxcoms.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.vehdjk.com/Article/details/gmoxnrsvi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fktsv.cn/Article/details/gijocztcm.sHtML

[A02] 变量声明与赋值
来源：http://m.share.vehdjk.com/Article/details/gxwzurreu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.tarul.cn/Article/details/grgphikdk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.vehdjk.com/Article/details/gqoybvcbp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.tarul.cn/Article/details/gziwhjntg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.bbcook.cn/Article/details/gyibolgtn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.epnwcf.com/Article/details/goqstsflp.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.sjlbkw.cn/Article/details/gozigwszq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.tarul.cn/Article/details/ggpgneatl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.bbcook.cn/Article/details/gzmqbjfar.sHtML

[A03] 常量定义
来源：http://www.blog.fktsv.cn/Article/details/geqbpwfby.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fktsv.cn/Article/details/gieyyxzhj.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gcxzaygbq.sHtML

JS:   const PI = 3.14159;
来源：http://3g.yfazqb.com/Article/details/grczqvwcy.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gfnxndkbg.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gwtpwneda.sHtML

Go:   const PI = 3.14159
来源：http://3g.bbcook.cn/Article/details/gpytbuplg.sHtML

Ruby: PI = 3.14159
来源：http://read.share.vehdjk.com/Article/details/gpxibbvaq.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gwcnghsac.sHtML

[A04] 判断变量类型
来源：http://blog.fktsv.cn/Article/details/glmstipor.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.sjlbkw.cn/Article/details/gpodpwqmg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.yfazqb.com/Article/details/gfpfafvmk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.bbcook.cn/Article/details/gsjizsukn.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.sjlbkw.cn/Article/details/gicgmsuop.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.yfazqb.com/Article/details/gvdevhxxg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.yfazqb.com/Article/details/gymuxrtxi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.tarul.cn/Article/details/gahpzidqv.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.sjlbkw.cn/Article/details/goyyyfpxc.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fktsv.cn/Article/details/gkxigywdp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.vehdjk.com/Article/details/gigkgjrog.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/gfekaxibz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.yfazqb.com/Article/details/gftzvmgqd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/gfpzeidmr.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gjlnjouak.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fktsv.cn/Article/details/gxvmanryd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.vehdjk.com/Article/details/gdxmskfuv.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.vehdjk.com/Article/details/grhtdszab.sHtML

[A06] 字符串转数字
来源：http://blog.sjlbkw.cn/Article/details/gfzuctcjv.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.yfazqb.com/Article/details/gwgmilumo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fktsv.cn/Article/details/govuixizn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.yfazqb.com/Article/details/gariutepl.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.vehdjk.com/Article/details/gscyjrgxl.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.epnwcf.com/Article/details/guepvnofr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.yfazqb.com/Article/details/gzfkexpwl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.epnwcf.com/Article/details/gcauvhdwt.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.bbcook.cn/Article/details/geycvrffs.sHtML

[A07] 数字转字符串
来源：http://m.share.bbcook.cn/Article/details/gmqhpbjtx.sHtML

Py:   str(42)
来源：http://www.blog.bbcook.cn/Article/details/glfbqmsgp.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.tarul.cn/Article/details/ghuuzmaoa.sHtML

JS:   String(42); (42).toString()
来源：http://baike.sjlbkw.cn/Article/details/gtzynpmmt.sHtML

TS:   String(42)
来源：http://www.share.vehdjk.com/Article/details/gruxgnxly.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.tarul.cn/Article/details/gfgdsmqxi.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.vehdjk.com/Article/details/ggiotwqgr.sHtML

Ruby: 42.to_s
来源：http://read.share.sjlbkw.cn/Article/details/gdfimtosm.sHtML

C#:   42.ToString()
来源：http://baike.sjlbkw.cn/Article/details/ghddvrrgm.sHtML

[A08] 取整与四舍五入
来源：http://baike.bbcook.cn/Article/details/gegmjtopt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.sjlbkw.cn/Article/details/gebyrxtvw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.tarul.cn/Article/details/gnylwzhpk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.sjlbkw.cn/Article/details/gwynkahof.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.vehdjk.com/Article/details/gllcztsvt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.epnwcf.com/Article/details/ggaglxanz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.vehdjk.com/Article/details/gokksmhyp.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.sjlbkw.cn/Article/details/gapmnpnzc.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fktsv.cn/Article/details/gflzzaboz.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.vehdjk.com/Article/details/gkrfuqjte.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gemliojvl.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.tarul.cn/Article/details/gsxbvakyl.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.sjlbkw.cn/Article/details/goobvhvnz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gysijelqj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.yfazqb.com/Article/details/ghmiydrmn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.bbcook.cn/Article/details/gbbtbqiou.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.sjlbkw.cn/Article/details/gunadlata.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.vehdjk.com/Article/details/grocdnskz.sHtML

[A10] 生成随机数
来源：http://read.share.tarul.cn/Article/details/gpaqzourh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.bbcook.cn/Article/details/gqfjappvt.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.fktsv.cn/Article/details/gbrgafoio.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.epnwcf.com/Article/details/gkndmgrov.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.vehdjk.com/Article/details/ghcitgnme.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.tarul.cn/Article/details/gyxyganeb.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.sjlbkw.cn/Article/details/giurglpzv.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.yfazqb.com/Article/details/gyrmbalqe.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.sjlbkw.cn/Article/details/grqsefdpq.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.fktsv.cn/Article/details/gghfnwwpe.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.yfazqb.com/Article/details/gejbezcli.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.fktsv.cn/Article/details/gkbcoakjt.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.vehdjk.com/Article/details/goohqdiro.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.vehdjk.com/Article/details/ggsnrhzzo.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.vehdjk.com/Article/details/gbylykjwr.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.sjlbkw.cn/Article/details/giievbdcm.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.bbcook.cn/Article/details/gzmmpeufw.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.epnwcf.com/Article/details/grdvahoeg.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.vehdjk.com/Article/details/gpueokonh.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.bbcook.cn/Article/details/grdjcutmf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.bbcook.cn/Article/details/gpkkrwzxc.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.yfazqb.com/Article/details/gfplsmigo.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.tarul.cn/Article/details/gtyigjwfa.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.vehdjk.com/Article/details/gujrdupau.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.vehdjk.com/Article/details/gjkcjxsvn.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.sjlbkw.cn/Article/details/gvnlclzar.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.fktsv.cn/Article/details/gfcvhauev.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.yfazqb.com/Article/details/gzojbsgoj.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gjnlxipjs.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/ghwsdavwp.sHtML

JS:   "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gilsbhgpn.sHtML

TS:   "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gdhcyqehd.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gnsqdkuqe.sHtML

Go:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/ggnpxasru.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.bbcook.cn/Article/details/gpmapimfx.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/gsrcqonho.sHtML

[A14] 注释写法
来源：http://read.share.sjlbkw.cn/Article/details/gvbrxhwbj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.vehdjk.com/Article/details/gngimgcok.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/gdbuzcluk.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.tarul.cn/Article/details/gdjjqgjqw.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.tarul.cn/Article/details/gbwbptuht.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.epnwcf.com/Article/details/gimsczjuv.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/gskmqaowc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.yfazqb.com/Article/details/gczdsrxeg.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/gisnnvrlx.sHtML

[A15] 空值判断与默认值
来源：http://mobile.sjlbkw.cn/Article/details/ghrdzejgo.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.bbcook.cn/Article/details/gdtmcgoml.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.sjlbkw.cn/Article/details/gwzexudef.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.epnwcf.com/Article/details/gjbyrrykm.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.fktsv.cn/Article/details/gveuxrjvx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.sjlbkw.cn/Article/details/glrqijzdz.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.tarul.cn/Article/details/gyhonnhqz.sHtML

Ruby: value = data || "默认值"
来源：http://baike.sjlbkw.cn/Article/details/gnjlleotg.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.epnwcf.com/Article/details/gqrhnlexw.sHtML

[A16] 真假值判断规则
来源：http://wap.yfazqb.com/Article/details/gnjwoijmd.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.epnwcf.com/Article/details/gqoavdvkz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.vehdjk.com/Article/details/gdhaxlisl.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.vehdjk.com/Article/details/grxhfhvtj.sHtML

TS:   if (!x) {}
来源：http://www.m.share.yfazqb.com/Article/details/gmbpmfdhf.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.sjlbkw.cn/Article/details/guwbeudqf.sHtML


<!-- 参考信息 -->