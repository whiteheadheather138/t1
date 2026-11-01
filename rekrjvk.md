代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.blog.tarul.cn/Article/details/gfhysgrup.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.yfazqb.com/Article/details/gxwgzswmt.sHtML

[U92] JS：深拷贝
来源：http://www.share.bbcook.cn/Article/details/ghrtpcymi.sHtML

structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gisbrefua.sHtML

[U93] JS：模板字符串
来源：http://m.share.fktsv.cn/Article/details/gxawjhpeo.sHtML

`共 ${n} 条`
来源：http://mobile.sjlbkw.cn/Article/details/grazyvahw.sHtML

[U94] JS：箭头函数
来源：http://mobile.bbcook.cn/Article/details/gplgpezxh.sHtML

const double = x => x * 2;
来源：http://wap.fktsv.cn/Article/details/gfkudguax.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.tarul.cn/Article/details/gkaebvdfr.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjetvqsm.sHtML

[U96] JS：async/await 与异常
来源：http://baike.bbcook.cn/Article/details/gslkniyot.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/geugmvwld.sHtML

[U97] JS：并发请求
来源：http://read.share.epnwcf.com/Article/details/gfujjwhpt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/giufbotsa.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.bbcook.cn/Article/details/gdlethlrm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.sjlbkw.cn/Article/details/gtgnlwcnz.sHtML

[U99] JS：事件监听
来源：http://www.m.share.vehdjk.com/Article/details/gsghzzmzf.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fktsv.cn/Article/details/gfuujwqtu.sHtML

[U100] JS：DOM 查询
来源：http://3g.sjlbkw.cn/Article/details/gkkpqzivf.sHtML

document.querySelector(".item")
来源：http://blog.tarul.cn/Article/details/gaogokpdn.sHtML

[U101] JS：classList 操作
来源：http://www.blog.bbcook.cn/Article/details/gaajexjxi.sHtML

el.classList.toggle("active")
来源：http://www.m.share.sjlbkw.cn/Article/details/glwqgjytn.sHtML

[U102] JS：本地存储
来源：http://baike.tarul.cn/Article/details/glybqkzzq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.epnwcf.com/Article/details/gpvoxxugt.sHtML

[U103] JS：定时器
来源：http://www.share.yfazqb.com/Article/details/gfunfeuwa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fktsv.cn/Article/details/gaybktlih.sHtML

[U104] JS：防抖
来源：http://www.share.tarul.cn/Article/details/ggrekcuep.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gnvauspcy.sHtML

[U105] JS：节流
来源：http://m.share.bbcook.cn/Article/details/gjgvbzvxm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.yfazqb.com/Article/details/gpeyjqzdg.sHtML

[U106] JS：日期格式化
来源：http://www.share.yfazqb.com/Article/details/gvqexjtoq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.sjlbkw.cn/Article/details/gcijgigqq.sHtML

[U107] JS：数字千分位
来源：http://wap.bbcook.cn/Article/details/gvbxmnhfx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.vehdjk.com/Article/details/glpzpzfuz.sHtML

[U108] JS：随机整数
来源：http://m.share.sjlbkw.cn/Article/details/gfkxpiexh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.yfazqb.com/Article/details/gzgxgwtfj.sHtML

[U109] JS：数组分组
来源：http://www.share.tarul.cn/Article/details/gkcowiljh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.epnwcf.com/Article/details/grvkyxhqi.sHtML

[U110] JS：数组分块
来源：http://m.share.tarul.cn/Article/details/gfajrgbtn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.bbcook.cn/Article/details/gfpjkupjr.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fktsv.cn/Article/details/gxquujrwr.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.bbcook.cn/Article/details/gdogdglyv.sHtML

[U112] JS：字符串补位
来源：http://read.share.fktsv.cn/Article/details/gtttaswdy.sHtML

"7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/gylibgftb.sHtML

[U113] JS：正则替换全部
来源：http://read.share.epnwcf.com/Article/details/gzshbszgs.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gjsjqsmtc.sHtML

[U114] JS：JSON 深比较
来源：http://3g.vehdjk.com/Article/details/glcgfuzfk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.tarul.cn/Article/details/gwcphyhgp.sHtML

[U115] JS：生成 UUID
来源：http://read.share.epnwcf.com/Article/details/gzzyapuqv.sHtML

crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/gcnwphshu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.vehdjk.com/Article/details/glbuweunr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.vehdjk.com/Article/details/gsretunwe.sHtML

[U117] JS：单元测试
来源：http://www.blog.bbcook.cn/Article/details/gvxcelcaf.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.tarul.cn/Article/details/gqqjvhcwx.sHtML

[U118] JS：开发服务器
来源：http://read.share.tarul.cn/Article/details/gdtlcssyj.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fktsv.cn/Article/details/gclwnatth.sHtML

[U119] JS：生产构建
来源：http://3g.epnwcf.com/Article/details/gqqihkwyg.sHtML

npx vite build
来源：http://blog.yfazqb.com/Article/details/gsopghpqu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.epnwcf.com/Article/details/gcgmljvuf.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.tarul.cn/Article/details/ganiqejrh.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gkdjvtmwk.sHtML

统计汇总
来源：http://baike.bbcook.cn/Article/details/gzqceqeyb.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ghdwsokzw.sHtML

按语言统计（条）：
来源：http://wap.sjlbkw.cn/Article/details/gmjblfvzi.sHtML

Python ......... 252
来源：http://read.share.sjlbkw.cn/Article/details/ggxausioz.sHtML

PHP ............ 252
来源：http://baike.fktsv.cn/Article/details/gjrqvcinb.sHtML

JavaScript ..... 252
来源：http://www.share.epnwcf.com/Article/details/gtkndjoes.sHtML

TypeScript ..... 212
来源：http://wap.epnwcf.com/Article/details/gvqugkqkz.sHtML

Java ........... 212
来源：http://www.m.share.fktsv.cn/Article/details/ggnfccmyp.sHtML

Go ............. 212
来源：http://3g.yfazqb.com/Article/details/gbqkzdpgw.sHtML

Ruby ........... 212
来源：http://baike.yfazqb.com/Article/details/gmiroryke.sHtML

C# ............. 212
来源：http://www.share.sjlbkw.cn/Article/details/gbzpoucap.sHtML

C .............. 30
来源：http://www.share.yfazqb.com/Article/details/ghfpfjwzi.sHtML

C++ ............ 30
来源：http://www.blog.yfazqb.com/Article/details/gnwcazcjc.sHtML

SQL ............ 90
来源：http://3g.bbcook.cn/Article/details/grhmulcni.sHtML

Bash ........... 80
来源：http://wap.fktsv.cn/Article/details/guboamppu.sHtML

Kotlin ......... 15
来源：http://wap.bbcook.cn/Article/details/gttulgysg.sHtML

Swift .......... 15
来源：http://www.share.epnwcf.com/Article/details/gvkpjtidr.sHtML

Lua ............ 10
来源：http://www.blog.bbcook.cn/Article/details/gfwaconqg.sHtML

Perl ........... 10
来源：http://www.share.yfazqb.com/Article/details/gmwottckr.sHtML

Scala .......... 10
来源：http://www.share.yfazqb.com/Article/details/gfwkgknwc.sHtML

------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gylmuehss.sHtML

合计 ........... 2106 条
来源：http://m.share.vehdjk.com/Article/details/gndhybbej.sHtML

按章节统计：
来源：http://blog.bbcook.cn/Article/details/gajjniaqk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.sjlbkw.cn/Article/details/ghuxppyvu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fktsv.cn/Article/details/gijbejkgk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fktsv.cn/Article/details/gpmyxczey.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.sjlbkw.cn/Article/details/gafdtiaqd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.sjlbkw.cn/Article/details/gmyvlfbse.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.sjlbkw.cn/Article/details/gqqimivel.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.bbcook.cn/Article/details/gqngoonfz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.vehdjk.com/Article/details/gdqlahtjl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/geuiaonen.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.tarul.cn/Article/details/gtlikgchc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fktsv.cn/Article/details/gmspquiqf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gifwwbdkr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/gvroedvpu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.bbcook.cn/Article/details/gppnsknda.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.sjlbkw.cn/Article/details/gisulnyum.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gcwybvwrz.sHtML

Q SQL 专题                              90
来源：http://blog.tarul.cn/Article/details/glotsnhxw.sHtML

R Bash 专题                             80
来源：http://www.blog.vehdjk.com/Article/details/glryguvjl.sHtML

S C / C++ 专题                          60
来源：http://m.share.epnwcf.com/Article/details/guvznyfbh.sHtML

T 其他语言补充                          60
来源：http://3g.sjlbkw.cn/Article/details/ggqqfcgvi.sHtML

U 高频实用片段                         120
来源：http://3g.yfazqb.com/Article/details/guktgwtyu.sHtML

------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gxajyhdjf.sHtML

合计                                  2106 条
来源：http://read.share.bbcook.cn/Article/details/gawojbfet.sHtML

--------------------------------------------------------------------------------
来源：http://3g.vehdjk.com/Article/details/gdsuurtee.sHtML

使用提醒
来源：http://www.share.fktsv.cn/Article/details/gtmpqtbfl.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gexqazlky.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.epnwcf.com/Article/details/gnjkuwctm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.sjlbkw.cn/Article/details/gcasensge.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.yfazqb.com/Article/details/gqlufitmy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.epnwcf.com/Article/details/ghvqgpigu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fktsv.cn/Article/details/gytvptsqa.sHtML

—— 文件结束 ——
来源：http://baike.vehdjk.com/Article/details/gxmnefata.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/giemenvjt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fktsv.cn/Article/details/gwggsmnnb.sHtML

Common Programming Examples Cheat Book
来源：http://3g.sjlbkw.cn/Article/details/ggcfxzlwz.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gmmnwonjn.sHtML

【收录内容】
来源：http://www.blog.sjlbkw.cn/Article/details/gatvtktyi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.sjlbkw.cn/Article/details/gapunpdgb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.sjlbkw.cn/Article/details/galfbcqsz.sHtML

SQL · Bash · C · C++
来源：http://www.blog.yfazqb.com/Article/details/gslgtjiws.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.epnwcf.com/Article/details/gpuxxyayp.sHtML

【使用说明】
来源：http://wap.vehdjk.com/Article/details/gkwvkspzn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fktsv.cn/Article/details/giubyittl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fktsv.cn/Article/details/gaabsvhll.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.sjlbkw.cn/Article/details/glnjtlhzo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.sjlbkw.cn/Article/details/gskoepqez.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.sjlbkw.cn/Article/details/gkcldljqb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.tarul.cn/Article/details/gsqjvclcd.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.bbcook.cn/Article/details/gkzsehuhd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.sjlbkw.cn/Article/details/guxeoktqy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.bbcook.cn/Article/details/gqxvwypws.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.bbcook.cn/Article/details/guyzwfdsb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.tarul.cn/Article/details/gmjldmtpr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.sjlbkw.cn/Article/details/gujfzleeu.sHtML

【文件统计】
来源：http://baike.vehdjk.com/Article/details/gvnaxiwwt.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fktsv.cn/Article/details/gphwcykqq.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.epnwcf.com/Article/details/gaqkmqvqz.sHtML

目  录
来源：http://mobile.sjlbkw.cn/Article/details/gvpxwkuoh.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.bbcook.cn/Article/details/gxaumjtic.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.bbcook.cn/Article/details/grmjdyvuv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.epnwcf.com/Article/details/gkahyonxo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.vehdjk.com/Article/details/gyadrojyx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.yfazqb.com/Article/details/gwxplofyr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.yfazqb.com/Article/details/gijoyblcn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.epnwcf.com/Article/details/gjiptwxga.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.vehdjk.com/Article/details/gcxiwilmn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fktsv.cn/Article/details/gstqltnng.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gyprcprwo.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.bbcook.cn/Article/details/gakbmmsbf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.yfazqb.com/Article/details/gdsvfflpf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.sjlbkw.cn/Article/details/gmiioghav.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.vehdjk.com/Article/details/gvdjjscbq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.epnwcf.com/Article/details/gvsbxzqmi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.vehdjk.com/Article/details/gnoofnyen.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/gpaktevzx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.vehdjk.com/Article/details/ggfhxkwal.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.tarul.cn/Article/details/gcjvrmetz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fktsv.cn/Article/details/ggmhavkce.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.tarul.cn/Article/details/gczvfgzvs.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.yfazqb.com/Article/details/grgfshxbi.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gkpvkdogg.sHtML

A. 基础语法与类型
来源：http://m.share.fktsv.cn/Article/details/gxlviihfi.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gqjrlcazk.sHtML

[A01] Hello World
来源：http://3g.vehdjk.com/Article/details/gtitmcfxc.sHtML

Py:   print("Hello, World!")
来源：http://read.share.tarul.cn/Article/details/gzxowgfrs.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.yfazqb.com/Article/details/gefbaeevx.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.tarul.cn/Article/details/guzhpvfcf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.vehdjk.com/Article/details/gxtudoubg.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.epnwcf.com/Article/details/gfpwyiyca.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.yfazqb.com/Article/details/gaigasdec.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fktsv.cn/Article/details/gsodflufz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.bbcook.cn/Article/details/goqlojntx.sHtML

[A02] 变量声明与赋值
来源：http://baike.epnwcf.com/Article/details/gjaqxejag.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.epnwcf.com/Article/details/gqcijgjqf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.bbcook.cn/Article/details/geffjvosp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.tarul.cn/Article/details/giogaeghs.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.sjlbkw.cn/Article/details/gjmtpeyal.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.bbcook.cn/Article/details/glvjewkpz.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.tarul.cn/Article/details/gfmowhjvi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.yfazqb.com/Article/details/ghuwiamwf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.vehdjk.com/Article/details/gtqebioaq.sHtML

[A03] 常量定义
来源：http://www.m.share.vehdjk.com/Article/details/gzqmyktbt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.vehdjk.com/Article/details/gzidjvmax.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/ghjxmnpgn.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gktoqgakj.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.tarul.cn/Article/details/gzeombkaq.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gumgwxrto.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlxqdjcc.sHtML

Ruby: PI = 3.14159
来源：http://wap.tarul.cn/Article/details/gyvlpsbok.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fktsv.cn/Article/details/gwgrnkxwf.sHtML

[A04] 判断变量类型
来源：http://blog.yfazqb.com/Article/details/gokfcvsjx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.epnwcf.com/Article/details/gywvviwqy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.vehdjk.com/Article/details/gowlpwfmd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.epnwcf.com/Article/details/gxzkuvpvj.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.yfazqb.com/Article/details/gupblfksg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fktsv.cn/Article/details/gpaeawyre.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.vehdjk.com/Article/details/gqvuqytkd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.sjlbkw.cn/Article/details/gsvzwemuo.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.yfazqb.com/Article/details/gurgnqbjr.sHtML

[A05] 整数除法与取模
来源：http://www.blog.yfazqb.com/Article/details/gairfxtzi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.sjlbkw.cn/Article/details/ghztidzhd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.tarul.cn/Article/details/gfmfmohqv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/gxlwggpcx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.epnwcf.com/Article/details/grbpocwum.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/gkalioeeb.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/gniqvnluc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/gtmlyyrbi.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.tarul.cn/Article/details/gwvfmzjxt.sHtML

[A06] 字符串转数字
来源：http://blog.bbcook.cn/Article/details/gvloopvvk.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.epnwcf.com/Article/details/gnihbxvdw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.vehdjk.com/Article/details/gazzsicjj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fktsv.cn/Article/details/gzvcjstor.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.tarul.cn/Article/details/gxqwhwqvj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.bbcook.cn/Article/details/gyjzdlrqw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.vehdjk.com/Article/details/grvpmubhh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fktsv.cn/Article/details/gxcckfhze.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.tarul.cn/Article/details/gjogppsce.sHtML

[A07] 数字转字符串
来源：http://baike.bbcook.cn/Article/details/gyptdvzri.sHtML

Py:   str(42)
来源：http://wap.epnwcf.com/Article/details/gplqhfezo.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.vehdjk.com/Article/details/goyqcopjs.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gmgzpzoho.sHtML

TS:   String(42)
来源：http://www.m.share.vehdjk.com/Article/details/gsklfqqzo.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.yfazqb.com/Article/details/gtrlsbyfi.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.epnwcf.com/Article/details/gurphakkp.sHtML

Ruby: 42.to_s
来源：http://baike.tarul.cn/Article/details/gsjhpcuiu.sHtML

C#:   42.ToString()
来源：http://3g.yfazqb.com/Article/details/gmexpsang.sHtML

[A08] 取整与四舍五入
来源：http://baike.epnwcf.com/Article/details/gjnnftjbk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.vehdjk.com/Article/details/gwrdulldz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fktsv.cn/Article/details/gdvhnubca.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/gtszlomuo.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.yfazqb.com/Article/details/grhsiyaxw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.epnwcf.com/Article/details/gisjemdvi.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.epnwcf.com/Article/details/gdwgiyyqp.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.sjlbkw.cn/Article/details/gjixrarwi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.tarul.cn/Article/details/gbsnebmia.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.tarul.cn/Article/details/gbrgoztsg.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.vehdjk.com/Article/details/gvtciustd.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fktsv.cn/Article/details/gpqghssie.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.bbcook.cn/Article/details/ggklcxwml.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gvypraqcm.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.yfazqb.com/Article/details/gpxwoofym.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.tarul.cn/Article/details/gvvtubswp.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.vehdjk.com/Article/details/gjygmjkew.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gbtqczhol.sHtML

[A10] 生成随机数
来源：http://mobile.tarul.cn/Article/details/gmptkvsgp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.tarul.cn/Article/details/gwmdvqlvc.sHtML

PHP:  random_int(1, 100);
来源：http://3g.yfazqb.com/Article/details/gwniwfpxd.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.bbcook.cn/Article/details/gbgjyeusd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.yfazqb.com/Article/details/gmqhiutfg.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.sjlbkw.cn/Article/details/gdgdevwnv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.epnwcf.com/Article/details/gittmuuko.sHtML

Ruby: rand(1..100)
来源：http://3g.tarul.cn/Article/details/gskzdxnfe.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.bbcook.cn/Article/details/grkqnswqz.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.epnwcf.com/Article/details/gxnrcrmss.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.sjlbkw.cn/Article/details/gwhsqyxcg.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fktsv.cn/Article/details/gtbmltlfv.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.fktsv.cn/Article/details/gjonykhuv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.yfazqb.com/Article/details/grlzdmtnc.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.yfazqb.com/Article/details/gwiwnnuwu.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.vehdjk.com/Article/details/gjpgycyra.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.tarul.cn/Article/details/gwhnhwasj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.tarul.cn/Article/details/gtaknmmtn.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.fktsv.cn/Article/details/gecupqefc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.yfazqb.com/Article/details/gexatdrsc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.sjlbkw.cn/Article/details/gwwqetaik.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fktsv.cn/Article/details/gczouvqfa.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.fktsv.cn/Article/details/gmjifjprw.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.vehdjk.com/Article/details/gssvdfado.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.bbcook.cn/Article/details/gtoyvxqsk.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.epnwcf.com/Article/details/gwmukhyjz.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.bbcook.cn/Article/details/gmvadmdal.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.vehdjk.com/Article/details/gocjwgxwg.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/gbryqcnny.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/gyzepfklm.sHtML

JS:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/givkzatka.sHtML

TS:   "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/gyloxmjsa.sHtML

Java: "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gokjjkdev.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.epnwcf.com/Article/details/gstckamlj.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/gwxusvrfd.sHtML

C#:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/gspxxznjm.sHtML

[A14] 注释写法
来源：http://mobile.tarul.cn/Article/details/gilzxazds.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fktsv.cn/Article/details/gstbpdqgb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.yfazqb.com/Article/details/gqeituyld.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.tarul.cn/Article/details/gzeqjuvdn.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.sjlbkw.cn/Article/details/gejctcfcr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.sjlbkw.cn/Article/details/grdpltbxv.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/gbvzimesw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.epnwcf.com/Article/details/goeyezxml.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.bbcook.cn/Article/details/gkqvgouwg.sHtML

[A15] 空值判断与默认值
来源：http://baike.tarul.cn/Article/details/gjnckzhlc.sHtML

Py:   value = data or "默认值"
来源：http://blog.tarul.cn/Article/details/gyilvdrfq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.tarul.cn/Article/details/genymlpse.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.yfazqb.com/Article/details/giyufexvr.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.tarul.cn/Article/details/gupaeswgc.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.yfazqb.com/Article/details/gwyxlbsza.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.sjlbkw.cn/Article/details/gahavaatb.sHtML


<!-- 参考信息 -->