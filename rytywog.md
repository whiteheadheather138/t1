代发 wailian999

[U89] JS：数组去重
来源：http://www.blog.sjlbkw.cn/Article/details/gduijdlkg.sHtML

[...new Set(arr)]
来源：http://blog.vehdjk.com/Article/details/goxrbtxvm.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.epnwcf.com/Article/details/gfcjzyxtn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/gfopaitxo.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.tarul.cn/Article/details/gutborupw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.epnwcf.com/Article/details/gfvusgmdo.sHtML

[U92] JS：深拷贝
来源：http://blog.yfazqb.com/Article/details/gxurozgdj.sHtML

structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gnfstohku.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fktsv.cn/Article/details/gldjdjuqe.sHtML

`共 ${n} 条`
来源：http://www.blog.fktsv.cn/Article/details/gpaqmvgrf.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.epnwcf.com/Article/details/grdpkjgkr.sHtML

const double = x => x * 2;
来源：http://m.share.epnwcf.com/Article/details/gucicdcuy.sHtML

[U95] JS：Promise 包装
来源：http://mobile.yfazqb.com/Article/details/giucwjhkg.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.yfazqb.com/Article/details/geuilhplp.sHtML

[U96] JS：async/await 与异常
来源：http://baike.yfazqb.com/Article/details/gklponumw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/giauegrmf.sHtML

[U97] JS：并发请求
来源：http://m.share.yfazqb.com/Article/details/geipcvhaw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/grykqavdf.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.epnwcf.com/Article/details/gtjqjsvgo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.vehdjk.com/Article/details/gjhroswrz.sHtML

[U99] JS：事件监听
来源：http://3g.tarul.cn/Article/details/grfgikgey.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.tarul.cn/Article/details/gepkldikt.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.vehdjk.com/Article/details/geermjher.sHtML

document.querySelector(".item")
来源：http://www.m.share.epnwcf.com/Article/details/gkvhttlpm.sHtML

[U101] JS：classList 操作
来源：http://m.share.vehdjk.com/Article/details/gjkqxcgfz.sHtML

el.classList.toggle("active")
来源：http://m.share.yfazqb.com/Article/details/grsmfoxpr.sHtML

[U102] JS：本地存储
来源：http://read.share.fktsv.cn/Article/details/gfgmgoyqc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fktsv.cn/Article/details/goqjzozja.sHtML

[U103] JS：定时器
来源：http://wap.tarul.cn/Article/details/gkgipqaph.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.vehdjk.com/Article/details/ghytmewkv.sHtML

[U104] JS：防抖
来源：http://www.blog.vehdjk.com/Article/details/gikqoirwd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/gxrsqwvwa.sHtML

[U105] JS：节流
来源：http://m.share.sjlbkw.cn/Article/details/goizfjmlz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.yfazqb.com/Article/details/gusoilszb.sHtML

[U106] JS：日期格式化
来源：http://www.share.vehdjk.com/Article/details/gqydbgmiw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fktsv.cn/Article/details/gbdluhemk.sHtML

[U107] JS：数字千分位
来源：http://www.share.fktsv.cn/Article/details/gbuwmanjx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.bbcook.cn/Article/details/gfwsjeqnt.sHtML

[U108] JS：随机整数
来源：http://read.share.fktsv.cn/Article/details/geqowyjzl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fktsv.cn/Article/details/gziyfmaey.sHtML

[U109] JS：数组分组
来源：http://read.share.tarul.cn/Article/details/gdwtpymta.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.tarul.cn/Article/details/gebgaczhj.sHtML

[U110] JS：数组分块
来源：http://www.blog.yfazqb.com/Article/details/gmhqeviuh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.vehdjk.com/Article/details/gesbssgrr.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fktsv.cn/Article/details/ghzcjtekv.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.bbcook.cn/Article/details/gmyuvmhcu.sHtML

[U112] JS：字符串补位
来源：http://3g.bbcook.cn/Article/details/guwppmykg.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggltorcwa.sHtML

[U113] JS：正则替换全部
来源：http://blog.yfazqb.com/Article/details/gekadfjsm.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gcazotvig.sHtML

[U114] JS：JSON 深比较
来源：http://wap.epnwcf.com/Article/details/gtsbdptrl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/gblvglcxb.sHtML

[U115] JS：生成 UUID
来源：http://baike.sjlbkw.cn/Article/details/gbamlsrnk.sHtML

crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/gisftykol.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.sjlbkw.cn/Article/details/goatqouti.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.vehdjk.com/Article/details/gzmnlbtqs.sHtML

[U117] JS：单元测试
来源：http://baike.yfazqb.com/Article/details/gxbikjhnf.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.yfazqb.com/Article/details/gjanymyin.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.epnwcf.com/Article/details/gwltjurhg.sHtML

npm i -D vite;  npx vite
来源：http://3g.epnwcf.com/Article/details/gufwnexqc.sHtML

[U119] JS：生产构建
来源：http://mobile.vehdjk.com/Article/details/gmxpecbuf.sHtML

npx vite build
来源：http://read.share.vehdjk.com/Article/details/gyvibzrfm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.yfazqb.com/Article/details/gwludnpfr.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fktsv.cn/Article/details/gdqnqpeuq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gqfvpgplc.sHtML

统计汇总
来源：http://wap.yfazqb.com/Article/details/gxyfltwhv.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gbjbpqsws.sHtML

按语言统计（条）：
来源：http://www.blog.tarul.cn/Article/details/gaypvqgak.sHtML

Python ......... 252
来源：http://www.share.epnwcf.com/Article/details/gxiudfvxy.sHtML

PHP ............ 252
来源：http://www.m.share.bbcook.cn/Article/details/gteftrkhx.sHtML

JavaScript ..... 252
来源：http://blog.tarul.cn/Article/details/gmozwrzbv.sHtML

TypeScript ..... 212
来源：http://wap.sjlbkw.cn/Article/details/geqqgvrxw.sHtML

Java ........... 212
来源：http://www.blog.fktsv.cn/Article/details/gtkpadsrj.sHtML

Go ............. 212
来源：http://wap.epnwcf.com/Article/details/gvnjdwbhk.sHtML

Ruby ........... 212
来源：http://www.m.share.bbcook.cn/Article/details/glxtltjuu.sHtML

C# ............. 212
来源：http://3g.epnwcf.com/Article/details/gpdebbcjz.sHtML

C .............. 30
来源：http://m.share.bbcook.cn/Article/details/ggfflxnzm.sHtML

C++ ............ 30
来源：http://wap.bbcook.cn/Article/details/gbzlrdhqq.sHtML

SQL ............ 90
来源：http://m.share.fktsv.cn/Article/details/gyfvgdgha.sHtML

Bash ........... 80
来源：http://www.m.share.bbcook.cn/Article/details/gkqrbioqo.sHtML

Kotlin ......... 15
来源：http://wap.yfazqb.com/Article/details/gnqilzdoe.sHtML

Swift .......... 15
来源：http://www.blog.bbcook.cn/Article/details/gunnscnqc.sHtML

Lua ............ 10
来源：http://baike.vehdjk.com/Article/details/gixaymmms.sHtML

Perl ........... 10
来源：http://mobile.vehdjk.com/Article/details/gtsvbtetl.sHtML

Scala .......... 10
来源：http://www.share.fktsv.cn/Article/details/ghpbrgqag.sHtML

------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gypiqxpvw.sHtML

合计 ........... 2106 条
来源：http://3g.vehdjk.com/Article/details/gsdwevsur.sHtML

按章节统计：
来源：http://3g.epnwcf.com/Article/details/gbojunasg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.tarul.cn/Article/details/glxwomkhd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.epnwcf.com/Article/details/gpsvlughs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.vehdjk.com/Article/details/gbqhunxbk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.yfazqb.com/Article/details/gjhfyyfap.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.epnwcf.com/Article/details/gsxwmegly.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.tarul.cn/Article/details/gvjwkzxnr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.yfazqb.com/Article/details/guvodzhsq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.bbcook.cn/Article/details/gvhldzcyd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/gxmebksif.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.yfazqb.com/Article/details/gnsllnabv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gelgnksxr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gdgfcxtas.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/gpbarxjko.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.vehdjk.com/Article/details/gyiswrofb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.vehdjk.com/Article/details/gvfvspgfo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/geewndarr.sHtML

Q SQL 专题                              90
来源：http://baike.vehdjk.com/Article/details/gtarzzaip.sHtML

R Bash 专题                             80
来源：http://m.share.yfazqb.com/Article/details/gxhcnadra.sHtML

S C / C++ 专题                          60
来源：http://wap.fktsv.cn/Article/details/gqyipyonz.sHtML

T 其他语言补充                          60
来源：http://baike.tarul.cn/Article/details/gyzhpihrp.sHtML

U 高频实用片段                         120
来源：http://m.share.yfazqb.com/Article/details/gpzwcpmdt.sHtML

------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gdzpdydwk.sHtML

合计                                  2106 条
来源：http://blog.sjlbkw.cn/Article/details/gzklnaurs.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.bbcook.cn/Article/details/ggtqfigfw.sHtML

使用提醒
来源：http://www.share.yfazqb.com/Article/details/gcuyctcpv.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.vehdjk.com/Article/details/ggsswskfa.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.sjlbkw.cn/Article/details/gnxbsthzh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.tarul.cn/Article/details/gnodqmpfu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.bbcook.cn/Article/details/gjinfqnci.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.vehdjk.com/Article/details/gzfojosll.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.bbcook.cn/Article/details/grxdsxxps.sHtML

—— 文件结束 ——
来源：http://mobile.tarul.cn/Article/details/guyljtyum.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gxlbqscpo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.epnwcf.com/Article/details/ghxzcdevq.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.bbcook.cn/Article/details/gjsxtvgsw.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gctjhrwid.sHtML

【收录内容】
来源：http://www.m.share.tarul.cn/Article/details/grwovkpdf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.tarul.cn/Article/details/ggjgplmez.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.yfazqb.com/Article/details/gdanrxxhg.sHtML

SQL · Bash · C · C++
来源：http://read.share.fktsv.cn/Article/details/gzmopwoxr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.tarul.cn/Article/details/gqlhujglc.sHtML

【使用说明】
来源：http://www.blog.bbcook.cn/Article/details/gkjjetiuw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.sjlbkw.cn/Article/details/gcydzvrdc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.yfazqb.com/Article/details/ghyspsvmv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.yfazqb.com/Article/details/gyzcgfnhd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.tarul.cn/Article/details/ggvbzkkcv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.tarul.cn/Article/details/grkmukbmf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.vehdjk.com/Article/details/ggqgeenbq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.bbcook.cn/Article/details/gwtlucpoh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.tarul.cn/Article/details/gdskbzfkj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.yfazqb.com/Article/details/gilvghaek.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.sjlbkw.cn/Article/details/gqmxmzbzv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.yfazqb.com/Article/details/gbkzseeyq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.bbcook.cn/Article/details/gevhmywmd.sHtML

【文件统计】
来源：http://wap.sjlbkw.cn/Article/details/gghyplsgo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.epnwcf.com/Article/details/gwbkegqfq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gpsdzrdzx.sHtML

目  录
来源：http://3g.fktsv.cn/Article/details/gwbnvxwsx.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gxsfhbtua.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.bbcook.cn/Article/details/gxevjicws.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.bbcook.cn/Article/details/gsldjdena.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/ggkqamsvt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.vehdjk.com/Article/details/gyorfvirx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.epnwcf.com/Article/details/gpcqrgsrz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.epnwcf.com/Article/details/gnhhuaamm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.yfazqb.com/Article/details/gljvibxwh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.bbcook.cn/Article/details/gikeanbuj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.tarul.cn/Article/details/gftldoiyc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.bbcook.cn/Article/details/gdthrqswm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.sjlbkw.cn/Article/details/ghwardmzc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/godoavtrq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/gxzkdehwe.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.tarul.cn/Article/details/gknpeftdt.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.vehdjk.com/Article/details/gqcbwujof.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.bbcook.cn/Article/details/gojqpuchc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.bbcook.cn/Article/details/gjrwjgxdh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.tarul.cn/Article/details/gdqsnxmyd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.vehdjk.com/Article/details/gnfoxbtij.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.sjlbkw.cn/Article/details/gathnfzhx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.epnwcf.com/Article/details/glwlmnfjj.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gbhoxlcmh.sHtML

A. 基础语法与类型
来源：http://read.share.vehdjk.com/Article/details/gilzloyyd.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkvxxbudx.sHtML

[A01] Hello World
来源：http://wap.bbcook.cn/Article/details/gcrocqwwh.sHtML

Py:   print("Hello, World!")
来源：http://blog.vehdjk.com/Article/details/gifukntol.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.sjlbkw.cn/Article/details/gezufhbgq.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.sjlbkw.cn/Article/details/gvksxbqrn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.yfazqb.com/Article/details/gfdlwzqjq.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.bbcook.cn/Article/details/gfhnvzqmh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.yfazqb.com/Article/details/gkwkuuyxd.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.vehdjk.com/Article/details/gqzzilyxq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.epnwcf.com/Article/details/gbvosmtyl.sHtML

[A02] 变量声明与赋值
来源：http://3g.vehdjk.com/Article/details/gdszpetcq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.vehdjk.com/Article/details/gujyclxza.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fktsv.cn/Article/details/gdfauqtny.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.sjlbkw.cn/Article/details/gixhulohu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fktsv.cn/Article/details/gucnvhbny.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.bbcook.cn/Article/details/gyamsokrw.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.tarul.cn/Article/details/guolzxkur.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.sjlbkw.cn/Article/details/gwsqkweum.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fktsv.cn/Article/details/gicslohfn.sHtML

[A03] 常量定义
来源：http://www.blog.bbcook.cn/Article/details/gtkliqjnc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.bbcook.cn/Article/details/gdckbzuor.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gvozsmdau.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gawdvrtux.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.yfazqb.com/Article/details/gsncgjqsv.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gxfonhnlq.sHtML

Go:   const PI = 3.14159
来源：http://blog.sjlbkw.cn/Article/details/gqtmagqqz.sHtML

Ruby: PI = 3.14159
来源：http://blog.vehdjk.com/Article/details/gwmwgjsna.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gseikvvpd.sHtML

[A04] 判断变量类型
来源：http://www.m.share.yfazqb.com/Article/details/gtfxkbyns.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.tarul.cn/Article/details/guwhonwzc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fktsv.cn/Article/details/gnqksrkic.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.bbcook.cn/Article/details/gwsxmywra.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fktsv.cn/Article/details/gmyxaddig.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.yfazqb.com/Article/details/ghjqaihdn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.epnwcf.com/Article/details/giokfhykd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fktsv.cn/Article/details/gkrczoard.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.tarul.cn/Article/details/ghbpthkmo.sHtML

[A05] 整数除法与取模
来源：http://mobile.tarul.cn/Article/details/gmlsmxeoi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.tarul.cn/Article/details/gjfzfbpfp.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.epnwcf.com/Article/details/gishsymju.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fktsv.cn/Article/details/goitynwgo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.yfazqb.com/Article/details/gaozfyhyu.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.yfazqb.com/Article/details/gaeigzhxw.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.epnwcf.com/Article/details/gppqdrlbz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gchezmifk.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.bbcook.cn/Article/details/gbnbrhjib.sHtML

[A06] 字符串转数字
来源：http://3g.fktsv.cn/Article/details/gcoxffsyg.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.bbcook.cn/Article/details/gowifcwxg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.epnwcf.com/Article/details/gzveomzkt.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.yfazqb.com/Article/details/gbcduazyc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.sjlbkw.cn/Article/details/ghorwadno.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.epnwcf.com/Article/details/ghwrvemge.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.bbcook.cn/Article/details/gmycquhks.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.fktsv.cn/Article/details/gzpyvabxo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.vehdjk.com/Article/details/gkacdjavx.sHtML

[A07] 数字转字符串
来源：http://mobile.yfazqb.com/Article/details/gznznacso.sHtML

Py:   str(42)
来源：http://www.m.share.bbcook.cn/Article/details/gtcvygijo.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.yfazqb.com/Article/details/girtvzjcj.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.tarul.cn/Article/details/gdsbisdbp.sHtML

TS:   String(42)
来源：http://3g.tarul.cn/Article/details/gtqdkooaq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.bbcook.cn/Article/details/gbpiqxfdu.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.yfazqb.com/Article/details/gphmngkoz.sHtML

Ruby: 42.to_s
来源：http://blog.tarul.cn/Article/details/grapwwrbv.sHtML

C#:   42.ToString()
来源：http://www.blog.fktsv.cn/Article/details/grzuzekda.sHtML

[A08] 取整与四舍五入
来源：http://mobile.vehdjk.com/Article/details/gbvucvnws.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.yfazqb.com/Article/details/grxjykoyi.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.sjlbkw.cn/Article/details/ggmikfkvx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.bbcook.cn/Article/details/gzznbtizs.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.yfazqb.com/Article/details/gdgajtrnu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.bbcook.cn/Article/details/gutmotzpk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.tarul.cn/Article/details/gijfvogga.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.yfazqb.com/Article/details/gapgaghna.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdsndtmu.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.yfazqb.com/Article/details/gvzbovvxn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.sjlbkw.cn/Article/details/grqkqcsae.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.epnwcf.com/Article/details/gijrnkdno.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.fktsv.cn/Article/details/gxuzhgmfy.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.bbcook.cn/Article/details/gkzozaxfd.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.epnwcf.com/Article/details/glsechdst.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.epnwcf.com/Article/details/gahdlqieb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.tarul.cn/Article/details/gojqsfdlz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.fktsv.cn/Article/details/gqfvnbkwk.sHtML

[A10] 生成随机数
来源：http://blog.tarul.cn/Article/details/gnhocixhl.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.epnwcf.com/Article/details/gdpqeyyhi.sHtML

PHP:  random_int(1, 100);
来源：http://3g.bbcook.cn/Article/details/gjrkrtivo.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.yfazqb.com/Article/details/gjyhqylpy.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.epnwcf.com/Article/details/ggytfljhe.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.tarul.cn/Article/details/gdqhigglp.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fktsv.cn/Article/details/gyjkvbptu.sHtML

Ruby: rand(1..100)
来源：http://3g.tarul.cn/Article/details/goriebrct.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fktsv.cn/Article/details/gegtddzsn.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.tarul.cn/Article/details/gsmnywrlb.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.fktsv.cn/Article/details/gpqepudif.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.sjlbkw.cn/Article/details/gxitpngcc.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.tarul.cn/Article/details/gqdyuykqz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.epnwcf.com/Article/details/gxpcdhfgx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.fktsv.cn/Article/details/gfwesqbpb.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.tarul.cn/Article/details/gqnybimak.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.epnwcf.com/Article/details/gpojmhcki.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.vehdjk.com/Article/details/gbwhudijb.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.sjlbkw.cn/Article/details/gcihsglyw.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.tarul.cn/Article/details/goailaxfb.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.yfazqb.com/Article/details/geyvyqach.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.vehdjk.com/Article/details/glxnvbust.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.fktsv.cn/Article/details/gebrzrsjz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.tarul.cn/Article/details/gpoitxaqo.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.tarul.cn/Article/details/gqjpzhzgz.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.tarul.cn/Article/details/gvxszxsrt.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.fktsv.cn/Article/details/ggzapsxpg.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.vehdjk.com/Article/details/gwqoufiib.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gugpohncz.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.epnwcf.com/Article/details/goqdrnzch.sHtML

JS:   "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/gdqxuvznx.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/gpntxhnij.sHtML

Java: "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gvnhpqets.sHtML

Go:   "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gbicwbdvs.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/grinepotr.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/gleimpmst.sHtML

[A14] 注释写法
来源：http://www.m.share.tarul.cn/Article/details/gbxodbbjo.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.epnwcf.com/Article/details/gqxwwjecd.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.sjlbkw.cn/Article/details/gmcqwjdzw.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.epnwcf.com/Article/details/gvdlxviat.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.epnwcf.com/Article/details/gpdzdghpf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.sjlbkw.cn/Article/details/grrzvnlpq.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/gtleywlpy.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.epnwcf.com/Article/details/gduaaimil.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fktsv.cn/Article/details/gaohsskxl.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.tarul.cn/Article/details/gnqjwgkys.sHtML

Py:   value = data or "默认值"
来源：http://baike.bbcook.cn/Article/details/gtcmsnate.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.vehdjk.com/Article/details/gfjvgiyqj.sHtML


<!-- 参考信息 -->