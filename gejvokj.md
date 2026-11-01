代发 wailian999

[U87] JS：解构默认值
来源：http://read.share.fktsv.cn/Article/details/gptlnlyyj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.bbcook.cn/Article/details/goyoqezwu.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fktsv.cn/Article/details/gdrvjkoud.sHtML

{ ...a, ...b }
来源：http://www.blog.vehdjk.com/Article/details/gghirqbtp.sHtML

[U89] JS：数组去重
来源：http://baike.yfazqb.com/Article/details/ggpalongh.sHtML

[...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/gcxnknzfc.sHtML

[U90] JS：数字数组排序
来源：http://baike.tarul.cn/Article/details/gpxubgsak.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/gsirzosvv.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.tarul.cn/Article/details/gyejmkkuh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.bbcook.cn/Article/details/gnqbudyfi.sHtML

[U92] JS：深拷贝
来源：http://m.share.yfazqb.com/Article/details/gycpbnunj.sHtML

structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/gadxvllkj.sHtML

[U93] JS：模板字符串
来源：http://3g.fktsv.cn/Article/details/grhacxdbj.sHtML

`共 ${n} 条`
来源：http://baike.fktsv.cn/Article/details/gkfywmvud.sHtML

[U94] JS：箭头函数
来源：http://mobile.vehdjk.com/Article/details/ggxrtwizh.sHtML

const double = x => x * 2;
来源：http://m.share.vehdjk.com/Article/details/gcaczzibz.sHtML

[U95] JS：Promise 包装
来源：http://3g.bbcook.cn/Article/details/gffwwvokl.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.bbcook.cn/Article/details/gpdlqmexy.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.bbcook.cn/Article/details/gqxrxvgto.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/ggwtdwije.sHtML

[U97] JS：并发请求
来源：http://baike.vehdjk.com/Article/details/govpkpiyp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/gzivcjchc.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fktsv.cn/Article/details/gkfksozam.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.tarul.cn/Article/details/gtlrvpzfe.sHtML

[U99] JS：事件监听
来源：http://www.blog.sjlbkw.cn/Article/details/goydtqmit.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.epnwcf.com/Article/details/gdpmrubfe.sHtML

[U100] JS：DOM 查询
来源：http://blog.bbcook.cn/Article/details/gdftqjsfn.sHtML

document.querySelector(".item")
来源：http://blog.tarul.cn/Article/details/gtmyfcvvz.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.vehdjk.com/Article/details/gssqhbpmf.sHtML

el.classList.toggle("active")
来源：http://baike.vehdjk.com/Article/details/gsqffnpjm.sHtML

[U102] JS：本地存储
来源：http://blog.yfazqb.com/Article/details/grlixwczp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.yfazqb.com/Article/details/gowfnnqet.sHtML

[U103] JS：定时器
来源：http://wap.sjlbkw.cn/Article/details/gvwwdxsyv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.yfazqb.com/Article/details/gbuhuubuc.sHtML

[U104] JS：防抖
来源：http://wap.epnwcf.com/Article/details/gqwtpbokf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.epnwcf.com/Article/details/gdbnqaqku.sHtML

[U105] JS：节流
来源：http://baike.bbcook.cn/Article/details/gefzvlenk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.epnwcf.com/Article/details/gslzxbbuy.sHtML

[U106] JS：日期格式化
来源：http://wap.tarul.cn/Article/details/glifprjoi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.bbcook.cn/Article/details/gbfcoxctr.sHtML

[U107] JS：数字千分位
来源：http://www.share.bbcook.cn/Article/details/grygebaiz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fktsv.cn/Article/details/gieyabhzt.sHtML

[U108] JS：随机整数
来源：http://baike.epnwcf.com/Article/details/ghlavqrhv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.yfazqb.com/Article/details/gptloakle.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fktsv.cn/Article/details/gqfaxiebz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.vehdjk.com/Article/details/gvebubtsu.sHtML

[U110] JS：数组分块
来源：http://www.blog.tarul.cn/Article/details/gjunpsrky.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.epnwcf.com/Article/details/gxzvovxvj.sHtML

[U111] JS：对象转 Map
来源：http://blog.fktsv.cn/Article/details/gwlcuwyni.sHtML

new Map(Object.entries(obj))
来源：http://read.share.vehdjk.com/Article/details/gdaadwiud.sHtML

[U112] JS：字符串补位
来源：http://read.share.fktsv.cn/Article/details/ghfdjblko.sHtML

"7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gfiicdpxl.sHtML

[U113] JS：正则替换全部
来源：http://baike.bbcook.cn/Article/details/gpewaxeod.sHtML

s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/ghsirelko.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.vehdjk.com/Article/details/gkynvflkr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.yfazqb.com/Article/details/gufiqqbdt.sHtML

[U115] JS：生成 UUID
来源：http://blog.tarul.cn/Article/details/gxherjyjx.sHtML

crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/gcqrxtzbh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.yfazqb.com/Article/details/grrxbofdu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gznfjeexj.sHtML

[U117] JS：单元测试
来源：http://read.share.tarul.cn/Article/details/grrquxwty.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.epnwcf.com/Article/details/ggpibrimb.sHtML

[U118] JS：开发服务器
来源：http://3g.yfazqb.com/Article/details/gvzmtpjma.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.sjlbkw.cn/Article/details/gokdriqzc.sHtML

[U119] JS：生产构建
来源：http://www.m.share.tarul.cn/Article/details/gesdlzdsg.sHtML

npx vite build
来源：http://www.blog.epnwcf.com/Article/details/gswojccbj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.vehdjk.com/Article/details/gskfkkbgo.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.tarul.cn/Article/details/gydjmfvlt.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ggsnnfihp.sHtML

统计汇总
来源：http://www.m.share.vehdjk.com/Article/details/gvqwvlqpd.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gpsglgjki.sHtML

按语言统计（条）：
来源：http://read.share.tarul.cn/Article/details/gizsvpxce.sHtML

Python ......... 252
来源：http://3g.vehdjk.com/Article/details/gohibjscf.sHtML

PHP ............ 252
来源：http://3g.epnwcf.com/Article/details/gqrhpeydv.sHtML

JavaScript ..... 252
来源：http://m.share.yfazqb.com/Article/details/gkplwmhpa.sHtML

TypeScript ..... 212
来源：http://mobile.tarul.cn/Article/details/glfgzitsy.sHtML

Java ........... 212
来源：http://baike.tarul.cn/Article/details/gbqlfzhcr.sHtML

Go ............. 212
来源：http://www.m.share.bbcook.cn/Article/details/gsemirhmo.sHtML

Ruby ........... 212
来源：http://www.m.share.bbcook.cn/Article/details/gocohvjuw.sHtML

C# ............. 212
来源：http://blog.bbcook.cn/Article/details/gkmfhsuma.sHtML

C .............. 30
来源：http://wap.bbcook.cn/Article/details/gsrcqyidl.sHtML

C++ ............ 30
来源：http://read.share.vehdjk.com/Article/details/guiruimzg.sHtML

SQL ............ 90
来源：http://baike.fktsv.cn/Article/details/gvltlsdvj.sHtML

Bash ........... 80
来源：http://read.share.fktsv.cn/Article/details/gzbpgmlza.sHtML

Kotlin ......... 15
来源：http://3g.fktsv.cn/Article/details/geqozzgui.sHtML

Swift .......... 15
来源：http://m.share.sjlbkw.cn/Article/details/gbdhtstof.sHtML

Lua ............ 10
来源：http://3g.vehdjk.com/Article/details/geocxreeg.sHtML

Perl ........... 10
来源：http://baike.fktsv.cn/Article/details/gmexpvele.sHtML

Scala .......... 10
来源：http://baike.sjlbkw.cn/Article/details/gkwaemoqu.sHtML

------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gferzkkgi.sHtML

合计 ........... 2106 条
来源：http://m.share.sjlbkw.cn/Article/details/grcllbczu.sHtML

按章节统计：
来源：http://www.m.share.tarul.cn/Article/details/gnooepkjz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.epnwcf.com/Article/details/glwuwopjp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.sjlbkw.cn/Article/details/gwdgjvsea.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.tarul.cn/Article/details/grexcbcsk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.epnwcf.com/Article/details/ggsfiuwmy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.tarul.cn/Article/details/godzlxlpy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.sjlbkw.cn/Article/details/gtpipqpfl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.bbcook.cn/Article/details/gwltxsaic.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.yfazqb.com/Article/details/ggcvjgnkc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gkadgrqvv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fktsv.cn/Article/details/glfpqpcmi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/gddjriqxr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gqvizecdn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/gegbhbkcm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.yfazqb.com/Article/details/ggnoxhnnr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.vehdjk.com/Article/details/gnbwlhzdh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/gdaowdczj.sHtML

Q SQL 专题                              90
来源：http://www.share.fktsv.cn/Article/details/gnxaunttm.sHtML

R Bash 专题                             80
来源：http://www.blog.fktsv.cn/Article/details/guuwxypra.sHtML

S C / C++ 专题                          60
来源：http://www.blog.vehdjk.com/Article/details/glrszkjug.sHtML

T 其他语言补充                          60
来源：http://www.m.share.vehdjk.com/Article/details/gbujmxhqm.sHtML

U 高频实用片段                         120
来源：http://3g.tarul.cn/Article/details/gctqscvlj.sHtML

------------------------------------
来源：http://3g.fktsv.cn/Article/details/gkoazptou.sHtML

合计                                  2106 条
来源：http://www.blog.bbcook.cn/Article/details/ghtoipovt.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gbpjkbjce.sHtML

使用提醒
来源：http://www.share.tarul.cn/Article/details/gntghelst.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/ghzflcspg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.epnwcf.com/Article/details/ggqsvnifw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.sjlbkw.cn/Article/details/gopijypkt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.tarul.cn/Article/details/gusyyawhm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.sjlbkw.cn/Article/details/ggpjffljd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.epnwcf.com/Article/details/glzygyedu.sHtML

—— 文件结束 ——
来源：http://www.share.yfazqb.com/Article/details/gmdenzoqe.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gewwxczex.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.sjlbkw.cn/Article/details/geabteqwf.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.vehdjk.com/Article/details/gctodvccx.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/glgtkrskv.sHtML

【收录内容】
来源：http://3g.vehdjk.com/Article/details/goxndkudo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.tarul.cn/Article/details/gjfnknajs.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.vehdjk.com/Article/details/gvfxiuadb.sHtML

SQL · Bash · C · C++
来源：http://www.blog.yfazqb.com/Article/details/gilafhxxt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fktsv.cn/Article/details/gqeeznfha.sHtML

【使用说明】
来源：http://3g.tarul.cn/Article/details/guzaymwqd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.yfazqb.com/Article/details/gfakpkeqy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.vehdjk.com/Article/details/gxqxwepmb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fktsv.cn/Article/details/gvbmqiaro.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.epnwcf.com/Article/details/guesiykgx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.vehdjk.com/Article/details/gqavrenck.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.yfazqb.com/Article/details/gkwgkyali.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.bbcook.cn/Article/details/gykidajlm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.vehdjk.com/Article/details/guwnoquxm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.vehdjk.com/Article/details/gqjtqdfgl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.epnwcf.com/Article/details/gettvazxw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.epnwcf.com/Article/details/gpsuehjdy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.sjlbkw.cn/Article/details/gdwwlfnfn.sHtML

【文件统计】
来源：http://www.m.share.yfazqb.com/Article/details/gfbqrywtk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.yfazqb.com/Article/details/gfovloklx.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gfqrekoob.sHtML

目  录
来源：http://www.blog.bbcook.cn/Article/details/gkjwhjzjs.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gegaaebtg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.bbcook.cn/Article/details/glojxbnnp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fktsv.cn/Article/details/gnjbdmsnt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.bbcook.cn/Article/details/gumnirfmk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.vehdjk.com/Article/details/gwvzywulo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.epnwcf.com/Article/details/geztriuul.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fktsv.cn/Article/details/giblgvkpi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.vehdjk.com/Article/details/gfkssnjmz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.bbcook.cn/Article/details/gkwhpjelk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/gaejudrbg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.vehdjk.com/Article/details/giyctowko.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/gvipqmwaf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.epnwcf.com/Article/details/gfmjrsunu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.vehdjk.com/Article/details/gtfctoxui.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.bbcook.cn/Article/details/gnxmmlpcs.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.vehdjk.com/Article/details/gienicugi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/grxgofhqv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.bbcook.cn/Article/details/ghshwyjnk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.tarul.cn/Article/details/gwfbclqmk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.vehdjk.com/Article/details/ghsdnacda.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.sjlbkw.cn/Article/details/gbqmobxbl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.vehdjk.com/Article/details/gxvkxtldk.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gxftqulmf.sHtML

A. 基础语法与类型
来源：http://baike.bbcook.cn/Article/details/ghwrjfxyb.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gzifrsfxj.sHtML

[A01] Hello World
来源：http://mobile.sjlbkw.cn/Article/details/guxyqmhhs.sHtML

Py:   print("Hello, World!")
来源：http://mobile.tarul.cn/Article/details/gzwiarfuv.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.yfazqb.com/Article/details/gfsrbyolr.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.sjlbkw.cn/Article/details/gtlkzriae.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.epnwcf.com/Article/details/gjqejeyly.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.bbcook.cn/Article/details/gjfzqpqry.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.epnwcf.com/Article/details/gtjsfssiq.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.vehdjk.com/Article/details/gosomqadp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fktsv.cn/Article/details/gwfivkgmj.sHtML

[A02] 变量声明与赋值
来源：http://www.share.yfazqb.com/Article/details/gohgjcsex.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.bbcook.cn/Article/details/gqclsihyt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.yfazqb.com/Article/details/gqtndkoud.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fktsv.cn/Article/details/ghnvcbmyz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.epnwcf.com/Article/details/guiyxcukw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fktsv.cn/Article/details/gcjcvxrsp.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.bbcook.cn/Article/details/gxlmlxefz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.sjlbkw.cn/Article/details/gyiecsald.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.epnwcf.com/Article/details/gqywytseu.sHtML

[A03] 常量定义
来源：http://read.share.vehdjk.com/Article/details/gjwabmyfz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.sjlbkw.cn/Article/details/gdbfyjeqv.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gaqfxjdgk.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gjaekeqge.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gnuwtucsv.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/goctbiulg.sHtML

Go:   const PI = 3.14159
来源：http://mobile.sjlbkw.cn/Article/details/gpqrwigbs.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.epnwcf.com/Article/details/ghnggilpr.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gtxlnmwcb.sHtML

[A04] 判断变量类型
来源：http://www.share.sjlbkw.cn/Article/details/gpshtxpfd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.yfazqb.com/Article/details/gugprewuv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.epnwcf.com/Article/details/gxzqmcutq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.epnwcf.com/Article/details/ghufjogso.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.tarul.cn/Article/details/gxgaffojq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.vehdjk.com/Article/details/gcjsfocnk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.tarul.cn/Article/details/gbdqrxzhi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.vehdjk.com/Article/details/glabwogar.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.yfazqb.com/Article/details/gnaibaytg.sHtML

[A05] 整数除法与取模
来源：http://blog.vehdjk.com/Article/details/ghbpewpbo.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.epnwcf.com/Article/details/gwencdadd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fktsv.cn/Article/details/guvdpxyeg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.bbcook.cn/Article/details/giludrblj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.epnwcf.com/Article/details/gzopwsenm.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.tarul.cn/Article/details/gwcvchfao.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.tarul.cn/Article/details/gmvlglhah.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gyywytfsz.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.vehdjk.com/Article/details/gnskaezlv.sHtML

[A06] 字符串转数字
来源：http://www.share.vehdjk.com/Article/details/gkkgyyciq.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.vehdjk.com/Article/details/gazjgustn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.yfazqb.com/Article/details/gmnaeqetb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.tarul.cn/Article/details/gtirmmdml.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.epnwcf.com/Article/details/gbykhrcyn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.tarul.cn/Article/details/gydjywpmx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.vehdjk.com/Article/details/gqzokkfpt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.yfazqb.com/Article/details/gsusfynml.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fktsv.cn/Article/details/gqejztibp.sHtML

[A07] 数字转字符串
来源：http://www.blog.yfazqb.com/Article/details/grtodqsmg.sHtML

Py:   str(42)
来源：http://m.share.bbcook.cn/Article/details/gjwbcywch.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.epnwcf.com/Article/details/goyywwmjl.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.tarul.cn/Article/details/gwhepbycc.sHtML

TS:   String(42)
来源：http://www.blog.tarul.cn/Article/details/ghspwwxrx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.sjlbkw.cn/Article/details/gkkpkvcmi.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.yfazqb.com/Article/details/geblzdnre.sHtML

Ruby: 42.to_s
来源：http://read.share.fktsv.cn/Article/details/gkiyaoeqm.sHtML

C#:   42.ToString()
来源：http://mobile.vehdjk.com/Article/details/gfhzzzzcd.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.vehdjk.com/Article/details/gleysyztr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.vehdjk.com/Article/details/gsaobauda.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.bbcook.cn/Article/details/gtmhmkwgs.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/ggmokvhaz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.sjlbkw.cn/Article/details/gvsrobyoc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/gstwkpafq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.tarul.cn/Article/details/gvvgihcpf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.sjlbkw.cn/Article/details/gasxrggmc.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.bbcook.cn/Article/details/ggckeiplu.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fktsv.cn/Article/details/gdskilolw.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/ghmbrfdua.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.epnwcf.com/Article/details/ghplhunxp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.yfazqb.com/Article/details/gijbqlxlg.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gungvqcuc.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.epnwcf.com/Article/details/gcndwtgxs.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.yfazqb.com/Article/details/gueooilyc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.epnwcf.com/Article/details/gaotuoexl.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.vehdjk.com/Article/details/glcubzbtg.sHtML

[A10] 生成随机数
来源：http://www.m.share.sjlbkw.cn/Article/details/gazivwppw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.epnwcf.com/Article/details/gpxmgygsc.sHtML

PHP:  random_int(1, 100);
来源：http://baike.epnwcf.com/Article/details/gvxpdduso.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.vehdjk.com/Article/details/gjmrqrmmn.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.bbcook.cn/Article/details/ggvwapvwi.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.sjlbkw.cn/Article/details/gcvjcrbst.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.sjlbkw.cn/Article/details/ghpmuzoew.sHtML

Ruby: rand(1..100)
来源：http://m.share.epnwcf.com/Article/details/gyqasuwtk.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.epnwcf.com/Article/details/gwjjcgfop.sHtML

[A11] 条件表达式（三元）
来源：http://3g.bbcook.cn/Article/details/gjqdpgnjg.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.bbcook.cn/Article/details/gsnsqezsi.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.tarul.cn/Article/details/gxmzxkomh.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/gcsazvadz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.yfazqb.com/Article/details/gqmqnskch.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/glsowhesa.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.bbcook.cn/Article/details/gmhjfhpux.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fktsv.cn/Article/details/gvngxzgvg.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.tarul.cn/Article/details/gopgiwrpn.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.sjlbkw.cn/Article/details/gdtyernan.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.sjlbkw.cn/Article/details/gzzxujszp.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.yfazqb.com/Article/details/guufgqjxw.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.epnwcf.com/Article/details/gwsuvyrti.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.tarul.cn/Article/details/gkwzsycfc.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.yfazqb.com/Article/details/goxzniovp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fktsv.cn/Article/details/glmwdhwgx.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.yfazqb.com/Article/details/gztuifmii.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.yfazqb.com/Article/details/gghfgldio.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.vehdjk.com/Article/details/gdjellgfq.sHtML

Py:   "第一行\n第二行"
来源：http://baike.yfazqb.com/Article/details/gknumjkdi.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gkcvlnspu.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gesvqjvjd.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gofdfnnpw.sHtML

Java: "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/gdqbihsvv.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gmdytcgeq.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/gshdapwxl.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gginvfqbw.sHtML

[A14] 注释写法
来源：http://m.share.fktsv.cn/Article/details/gwemzglyr.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.bbcook.cn/Article/details/gftptrzxd.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/giwvqfjvi.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.tarul.cn/Article/details/gmsfhefwb.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.tarul.cn/Article/details/gpzjtrtkc.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.tarul.cn/Article/details/gnzbtwxsv.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.yfazqb.com/Article/details/gwqnqukpk.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.epnwcf.com/Article/details/giuymipcc.sHtML


<!-- 参考信息 -->