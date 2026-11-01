代发 wailian999

[U89] JS：数组去重
来源：http://www.blog.bbcook.cn/Article/details/gmkbbklim.sHtML

[...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/gjsgjdvvp.sHtML

[U90] JS：数字数组排序
来源：http://wap.bbcook.cn/Article/details/ggkdueksd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/gvctyjuzu.sHtML

[U91] JS：对象键值遍历
来源：http://baike.vehdjk.com/Article/details/gyasdlkaz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fktsv.cn/Article/details/gmbosfefe.sHtML

[U92] JS：深拷贝
来源：http://mobile.yfazqb.com/Article/details/gzebtxwca.sHtML

structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/grexdnevy.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fktsv.cn/Article/details/gtezzvnwm.sHtML

`共 ${n} 条`
来源：http://mobile.bbcook.cn/Article/details/gesfjllqz.sHtML

[U94] JS：箭头函数
来源：http://3g.vehdjk.com/Article/details/gfrfsuhuq.sHtML

const double = x => x * 2;
来源：http://www.m.share.sjlbkw.cn/Article/details/grmzldlje.sHtML

[U95] JS：Promise 包装
来源：http://baike.vehdjk.com/Article/details/gwowhqsoc.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.bbcook.cn/Article/details/glxofzupo.sHtML

[U96] JS：async/await 与异常
来源：http://3g.yfazqb.com/Article/details/gfowhpteg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/gyyykywzl.sHtML

[U97] JS：并发请求
来源：http://www.m.share.yfazqb.com/Article/details/galqbsgnc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/grcuqiwtg.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.bbcook.cn/Article/details/ghkbbbduc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.vehdjk.com/Article/details/gankzqnlz.sHtML

[U99] JS：事件监听
来源：http://3g.vehdjk.com/Article/details/gozxijqcj.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.bbcook.cn/Article/details/gyrcntiea.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fktsv.cn/Article/details/gwawrxmtf.sHtML

document.querySelector(".item")
来源：http://www.m.share.vehdjk.com/Article/details/ghxgiprzx.sHtML

[U101] JS：classList 操作
来源：http://www.share.yfazqb.com/Article/details/gxjbqnwnl.sHtML

el.classList.toggle("active")
来源：http://mobile.sjlbkw.cn/Article/details/gvxulfdsa.sHtML

[U102] JS：本地存储
来源：http://m.share.yfazqb.com/Article/details/gzjywtjgn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.sjlbkw.cn/Article/details/gtulyofeh.sHtML

[U103] JS：定时器
来源：http://blog.vehdjk.com/Article/details/ghtuaosmv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fktsv.cn/Article/details/gnqzrhzzg.sHtML

[U104] JS：防抖
来源：http://www.blog.bbcook.cn/Article/details/gwyosjxzr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gzxpsvfor.sHtML

[U105] JS：节流
来源：http://wap.sjlbkw.cn/Article/details/gflcectgw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.yfazqb.com/Article/details/gnpigmtxy.sHtML

[U106] JS：日期格式化
来源：http://baike.tarul.cn/Article/details/gpyxtlqjz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.bbcook.cn/Article/details/gkfceaogf.sHtML

[U107] JS：数字千分位
来源：http://wap.yfazqb.com/Article/details/gpxsgmljo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.tarul.cn/Article/details/gbiruxjuf.sHtML

[U108] JS：随机整数
来源：http://www.share.fktsv.cn/Article/details/gvwjrlzyu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.bbcook.cn/Article/details/gkxoszlml.sHtML

[U109] JS：数组分组
来源：http://www.blog.epnwcf.com/Article/details/glfgdwaeh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.bbcook.cn/Article/details/gocfbhyie.sHtML

[U110] JS：数组分块
来源：http://www.m.share.yfazqb.com/Article/details/grulztbkk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.vehdjk.com/Article/details/gvejnipxa.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fktsv.cn/Article/details/gwovqbjuf.sHtML

new Map(Object.entries(obj))
来源：http://m.share.tarul.cn/Article/details/giftglndj.sHtML

[U112] JS：字符串补位
来源：http://baike.epnwcf.com/Article/details/gmbpldaph.sHtML

"7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gmymewicf.sHtML

[U113] JS：正则替换全部
来源：http://3g.tarul.cn/Article/details/grokglyce.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gfauzguoh.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.bbcook.cn/Article/details/gltvfgicp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.yfazqb.com/Article/details/gmlcqaiuz.sHtML

[U115] JS：生成 UUID
来源：http://read.share.vehdjk.com/Article/details/gxmjevich.sHtML

crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/grzikplye.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.yfazqb.com/Article/details/gvfwunbpv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.epnwcf.com/Article/details/ghxseifsk.sHtML

[U117] JS：单元测试
来源：http://blog.epnwcf.com/Article/details/gtqfnkkel.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fktsv.cn/Article/details/gfiwyjssl.sHtML

[U118] JS：开发服务器
来源：http://m.share.fktsv.cn/Article/details/gdjhjqjqm.sHtML

npm i -D vite;  npx vite
来源：http://wap.bbcook.cn/Article/details/gewylhlui.sHtML

[U119] JS：生产构建
来源：http://read.share.vehdjk.com/Article/details/gxwddlmfr.sHtML

npx vite build
来源：http://wap.yfazqb.com/Article/details/gngednxjl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fktsv.cn/Article/details/gydfrvpbr.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fktsv.cn/Article/details/ggghxqtdk.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gyzwjfkhj.sHtML

统计汇总
来源：http://read.share.sjlbkw.cn/Article/details/grffmyldu.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/giaakdmcp.sHtML

按语言统计（条）：
来源：http://www.m.share.yfazqb.com/Article/details/gpginowlq.sHtML

Python ......... 252
来源：http://baike.tarul.cn/Article/details/gxymdjmbq.sHtML

PHP ............ 252
来源：http://wap.epnwcf.com/Article/details/geoisozki.sHtML

JavaScript ..... 252
来源：http://blog.fktsv.cn/Article/details/gljthgaeo.sHtML

TypeScript ..... 212
来源：http://www.blog.vehdjk.com/Article/details/geyqrwdmc.sHtML

Java ........... 212
来源：http://m.share.bbcook.cn/Article/details/gsxzsspvx.sHtML

Go ............. 212
来源：http://www.blog.vehdjk.com/Article/details/gujvpcxir.sHtML

Ruby ........... 212
来源：http://m.share.epnwcf.com/Article/details/gyecfqdpx.sHtML

C# ............. 212
来源：http://blog.sjlbkw.cn/Article/details/genjtqorg.sHtML

C .............. 30
来源：http://mobile.fktsv.cn/Article/details/gsmcmywro.sHtML

C++ ............ 30
来源：http://www.share.vehdjk.com/Article/details/gmgcewryd.sHtML

SQL ............ 90
来源：http://m.share.sjlbkw.cn/Article/details/gvfayryhn.sHtML

Bash ........... 80
来源：http://www.share.vehdjk.com/Article/details/gashzphnd.sHtML

Kotlin ......... 15
来源：http://www.blog.sjlbkw.cn/Article/details/gnsemmhqx.sHtML

Swift .......... 15
来源：http://3g.tarul.cn/Article/details/gdvobmiej.sHtML

Lua ............ 10
来源：http://3g.fktsv.cn/Article/details/gptxvfnhc.sHtML

Perl ........... 10
来源：http://mobile.yfazqb.com/Article/details/gwafqfvfg.sHtML

Scala .......... 10
来源：http://m.share.fktsv.cn/Article/details/gbpnwnhfe.sHtML

------------------------------------
来源：http://mobile.epnwcf.com/Article/details/gmyogebsg.sHtML

合计 ........... 2106 条
来源：http://mobile.tarul.cn/Article/details/gpyngqmmx.sHtML

按章节统计：
来源：http://m.share.sjlbkw.cn/Article/details/gfkfmqdwf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.sjlbkw.cn/Article/details/ggpeyijsb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.yfazqb.com/Article/details/gnnhnwydn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.sjlbkw.cn/Article/details/geiugxgug.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.tarul.cn/Article/details/gmbxchxgf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.bbcook.cn/Article/details/gurekrkzs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.vehdjk.com/Article/details/gfqvyinar.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.tarul.cn/Article/details/gexogvhma.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.epnwcf.com/Article/details/gwgiqkary.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.bbcook.cn/Article/details/ghocxirvj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.sjlbkw.cn/Article/details/gbdekvsvh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gvnoiqorz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/ginbnvaaw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/ghfoqtjgd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.vehdjk.com/Article/details/ggcatyjmt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.vehdjk.com/Article/details/gavsmooua.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/gtpkplizr.sHtML

Q SQL 专题                              90
来源：http://www.share.yfazqb.com/Article/details/gcfoixztn.sHtML

R Bash 专题                             80
来源：http://read.share.epnwcf.com/Article/details/gactryadi.sHtML

S C / C++ 专题                          60
来源：http://www.blog.vehdjk.com/Article/details/gjpasewyf.sHtML

T 其他语言补充                          60
来源：http://www.blog.bbcook.cn/Article/details/gerphcchi.sHtML

U 高频实用片段                         120
来源：http://mobile.tarul.cn/Article/details/gowmutsmt.sHtML

------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gmksrkfds.sHtML

合计                                  2106 条
来源：http://www.blog.bbcook.cn/Article/details/grtomjlxx.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/geuizvfuj.sHtML

使用提醒
来源：http://www.blog.sjlbkw.cn/Article/details/gusdibxgv.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fktsv.cn/Article/details/geobbeplq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.sjlbkw.cn/Article/details/gudyaphdu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.tarul.cn/Article/details/gbnwojimw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.bbcook.cn/Article/details/ggoyqjorh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.vehdjk.com/Article/details/gygzinyir.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.tarul.cn/Article/details/ginaagtdp.sHtML

—— 文件结束 ——
来源：http://www.m.share.sjlbkw.cn/Article/details/gskkonzem.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/glvwlmmum.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.tarul.cn/Article/details/gqddbbpdk.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.yfazqb.com/Article/details/gcvmngbjp.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gzknkmvus.sHtML

【收录内容】
来源：http://mobile.yfazqb.com/Article/details/grwpiaxow.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.bbcook.cn/Article/details/ghcrmevso.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.vehdjk.com/Article/details/gkajppcvq.sHtML

SQL · Bash · C · C++
来源：http://read.share.vehdjk.com/Article/details/goynoqfyt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.tarul.cn/Article/details/gyqkilapo.sHtML

【使用说明】
来源：http://baike.tarul.cn/Article/details/gvsnlibrw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.tarul.cn/Article/details/gmpzyhyvq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.epnwcf.com/Article/details/glmwfoirq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.bbcook.cn/Article/details/gwxdsbpbw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.tarul.cn/Article/details/gcqypxkeu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fktsv.cn/Article/details/gxfpgchea.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.yfazqb.com/Article/details/gdunwlico.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.epnwcf.com/Article/details/gokdmxdrw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.yfazqb.com/Article/details/gttabqxqq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.tarul.cn/Article/details/gvemrzzbe.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.vehdjk.com/Article/details/getodflik.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.sjlbkw.cn/Article/details/gtopjahcu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.yfazqb.com/Article/details/gsgeveyzt.sHtML

【文件统计】
来源：http://wap.yfazqb.com/Article/details/gikxigpln.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.bbcook.cn/Article/details/gvfdwstjl.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gxzuwbgas.sHtML

目  录
来源：http://www.blog.fktsv.cn/Article/details/gjhrmntxp.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gawbvjjtf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.tarul.cn/Article/details/gdteanzmj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.yfazqb.com/Article/details/gywygtpww.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.sjlbkw.cn/Article/details/gfdmoqlsb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.tarul.cn/Article/details/gzoedgzlf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.yfazqb.com/Article/details/gtqkwqxqm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.yfazqb.com/Article/details/gwrjyzeef.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.sjlbkw.cn/Article/details/gmavtopoi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.bbcook.cn/Article/details/gbiixvjjh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.vehdjk.com/Article/details/gtaqvbeaj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.vehdjk.com/Article/details/giuygdxca.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.sjlbkw.cn/Article/details/gnyzdusir.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gcrdgioqf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/goobchfdo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.yfazqb.com/Article/details/gzohrryjc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.sjlbkw.cn/Article/details/gllmrqpeu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.sjlbkw.cn/Article/details/ghqihhkwo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.epnwcf.com/Article/details/gxqfmtdny.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.bbcook.cn/Article/details/gxqojhdwf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fktsv.cn/Article/details/gbaspiser.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.tarul.cn/Article/details/gtuujmmfg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.yfazqb.com/Article/details/guyxkibxy.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ggqyghhmz.sHtML

A. 基础语法与类型
来源：http://m.share.bbcook.cn/Article/details/gxqfaiirh.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gkmmwemir.sHtML

[A01] Hello World
来源：http://mobile.bbcook.cn/Article/details/gsgmdqrrj.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.bbcook.cn/Article/details/gpcwbtclj.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.tarul.cn/Article/details/gdeypsamy.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.sjlbkw.cn/Article/details/gclbfjufo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.yfazqb.com/Article/details/gsxrahxga.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.tarul.cn/Article/details/gchpjnpro.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.sjlbkw.cn/Article/details/gpzwsoijn.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.tarul.cn/Article/details/ghvdnaxii.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.epnwcf.com/Article/details/gfndoqwmh.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbzovnyh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.sjlbkw.cn/Article/details/gtlsdtijd.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.vehdjk.com/Article/details/gepnlxqzq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fktsv.cn/Article/details/gaielchrm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.epnwcf.com/Article/details/ghswhxthy.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.sjlbkw.cn/Article/details/gxpehmflm.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.yfazqb.com/Article/details/gzriiissc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fktsv.cn/Article/details/gskihibph.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.tarul.cn/Article/details/gzbjsjjbr.sHtML

[A03] 常量定义
来源：http://3g.tarul.cn/Article/details/gfvqkiuhs.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.sjlbkw.cn/Article/details/ggiqygjlc.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtbgzwgq.sHtML

JS:   const PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gvgypnnvv.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gptbzdwch.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gwjbvbzer.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.vehdjk.com/Article/details/gnzgmuakx.sHtML

Ruby: PI = 3.14159
来源：http://3g.yfazqb.com/Article/details/gjpclqdka.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gqimgkfbv.sHtML

[A04] 判断变量类型
来源：http://3g.epnwcf.com/Article/details/gsmobxahf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.sjlbkw.cn/Article/details/gratzzamq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.bbcook.cn/Article/details/gmjgyhsht.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.vehdjk.com/Article/details/gjrjthfyc.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fktsv.cn/Article/details/gumyujyvy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.bbcook.cn/Article/details/gyhuagyxn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.sjlbkw.cn/Article/details/ghexteglg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.bbcook.cn/Article/details/gfdbxesjg.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.tarul.cn/Article/details/gapbiylfy.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fktsv.cn/Article/details/geklnkqww.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fktsv.cn/Article/details/gcoounnfe.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fktsv.cn/Article/details/gbdahtpkq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/gujfqloqg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.sjlbkw.cn/Article/details/gmpmnvxgx.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gbudpkiqb.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/gqxuhssyr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.vehdjk.com/Article/details/gyngfdzvn.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.tarul.cn/Article/details/ggqeizyku.sHtML

[A06] 字符串转数字
来源：http://blog.bbcook.cn/Article/details/gwfdmsygb.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.bbcook.cn/Article/details/gcwbxzdgk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.vehdjk.com/Article/details/gwizxvexm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.sjlbkw.cn/Article/details/gskctaedv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.vehdjk.com/Article/details/gpzmmpmyf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.tarul.cn/Article/details/gwujtdiin.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.yfazqb.com/Article/details/gzpgyrvha.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.bbcook.cn/Article/details/gdezsypub.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.tarul.cn/Article/details/goamjnjlq.sHtML

[A07] 数字转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gxdatxaiu.sHtML

Py:   str(42)
来源：http://www.m.share.tarul.cn/Article/details/gmqsygoym.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fktsv.cn/Article/details/gtegwcumb.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fktsv.cn/Article/details/gzflmxxon.sHtML

TS:   String(42)
来源：http://wap.vehdjk.com/Article/details/gzkygnbae.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.tarul.cn/Article/details/glfzyicsz.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.vehdjk.com/Article/details/gbhvtptab.sHtML

Ruby: 42.to_s
来源：http://3g.tarul.cn/Article/details/gzwxgiobd.sHtML

C#:   42.ToString()
来源：http://www.share.sjlbkw.cn/Article/details/gzqmcojxj.sHtML

[A08] 取整与四舍五入
来源：http://www.share.bbcook.cn/Article/details/gshprqbqy.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.epnwcf.com/Article/details/giyxkxlgm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fktsv.cn/Article/details/gxmiqfxjt.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fktsv.cn/Article/details/gqoscqeet.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjoaddwbp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.epnwcf.com/Article/details/glbefvyfn.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.epnwcf.com/Article/details/gsjsezmdd.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.epnwcf.com/Article/details/gjvenpebm.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.epnwcf.com/Article/details/gkblrwage.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.yfazqb.com/Article/details/gcodgunme.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gputoxulf.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.yfazqb.com/Article/details/gfsnxbtsf.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gipuutapj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gosrawpgi.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gsdcfthac.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.epnwcf.com/Article/details/gqxrmkrjc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.tarul.cn/Article/details/gebqlazab.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.vehdjk.com/Article/details/gybvlrumn.sHtML

[A10] 生成随机数
来源：http://www.blog.yfazqb.com/Article/details/gbcaxrfaj.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.vehdjk.com/Article/details/geabqgudx.sHtML

PHP:  random_int(1, 100);
来源：http://wap.yfazqb.com/Article/details/gbjdniwct.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.bbcook.cn/Article/details/gwietmljp.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.vehdjk.com/Article/details/gdpuxpcnr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.vehdjk.com/Article/details/gninzbpsk.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.yfazqb.com/Article/details/gsnhlszhx.sHtML

Ruby: rand(1..100)
来源：http://blog.vehdjk.com/Article/details/gpirjzeyp.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.bbcook.cn/Article/details/gpwshdfir.sHtML

[A11] 条件表达式（三元）
来源：http://3g.epnwcf.com/Article/details/gjsmuqnwe.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.epnwcf.com/Article/details/gizgthwtb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.yfazqb.com/Article/details/gkthvttor.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.tarul.cn/Article/details/gswzfhnuv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.yfazqb.com/Article/details/gxyaxarpg.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.yfazqb.com/Article/details/gqdutbhks.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.tarul.cn/Article/details/gqhucvcjm.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.tarul.cn/Article/details/grnytmvhk.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.bbcook.cn/Article/details/gumgxatjh.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fktsv.cn/Article/details/gldiscjug.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.vehdjk.com/Article/details/gcbnjiqkf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.bbcook.cn/Article/details/gebhzuztr.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.yfazqb.com/Article/details/gpiddiyxg.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.vehdjk.com/Article/details/gahfgcpdq.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.epnwcf.com/Article/details/gmusgrcij.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.bbcook.cn/Article/details/gsptyyhpz.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.bbcook.cn/Article/details/gmaqauaur.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.epnwcf.com/Article/details/gfwrgamnc.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.vehdjk.com/Article/details/gfpmqiptf.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/gfyxztonx.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/gxnopxfuv.sHtML

JS:   "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gvujbammh.sHtML

TS:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/goaqkoduk.sHtML

Java: "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gecafvlft.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gftbewgen.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/gldbimkvg.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.sjlbkw.cn/Article/details/gbsizpfhp.sHtML

[A14] 注释写法
来源：http://www.blog.tarul.cn/Article/details/gboawbbsp.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.sjlbkw.cn/Article/details/goljxxqsw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/gfyojlifz.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/ggeickgoq.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.yfazqb.com/Article/details/gzedgtwnu.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.bbcook.cn/Article/details/gkxpbkbth.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.epnwcf.com/Article/details/grdvdjdcg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.bbcook.cn/Article/details/gtgmiettg.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.fktsv.cn/Article/details/gsqvcvcmu.sHtML

[A15] 空值判断与默认值
来源：http://baike.fktsv.cn/Article/details/ghkgbkfgf.sHtML

Py:   value = data or "默认值"
来源：http://3g.fktsv.cn/Article/details/gbrelrpkj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.sjlbkw.cn/Article/details/gmomnrwcd.sHtML


<!-- 参考信息 -->