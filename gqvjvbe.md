代发 wailian999

[U95] JS：Promise 包装
来源：http://www.share.fktsv.cn/Article/details/gjxzkngzw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.yfazqb.com/Article/details/gigfkbvdd.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.vehdjk.com/Article/details/gxotuxiqy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gygocmvks.sHtML

[U97] JS：并发请求
来源：http://www.share.fktsv.cn/Article/details/gbgxjurjz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gzpppzuro.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.sjlbkw.cn/Article/details/gtrquogeg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.bbcook.cn/Article/details/guqyfjldg.sHtML

[U99] JS：事件监听
来源：http://mobile.sjlbkw.cn/Article/details/ggtdvjypm.sHtML

el.addEventListener("click", e => {})
来源：http://blog.yfazqb.com/Article/details/gbjppefqg.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fktsv.cn/Article/details/giosvwmbg.sHtML

document.querySelector(".item")
来源：http://www.m.share.yfazqb.com/Article/details/gfztedrje.sHtML

[U101] JS：classList 操作
来源：http://baike.epnwcf.com/Article/details/gsuibsysp.sHtML

el.classList.toggle("active")
来源：http://read.share.sjlbkw.cn/Article/details/gyvvvdewi.sHtML

[U102] JS：本地存储
来源：http://blog.tarul.cn/Article/details/gutmkroxq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.yfazqb.com/Article/details/glvlwdher.sHtML

[U103] JS：定时器
来源：http://3g.epnwcf.com/Article/details/gslopvjce.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.tarul.cn/Article/details/gkprpagpe.sHtML

[U104] JS：防抖
来源：http://wap.sjlbkw.cn/Article/details/gqmkvguit.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/gkettyhhu.sHtML

[U105] JS：节流
来源：http://m.share.bbcook.cn/Article/details/gugokjrdd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.yfazqb.com/Article/details/gyufnsilb.sHtML

[U106] JS：日期格式化
来源：http://wap.bbcook.cn/Article/details/gjlljjprg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.yfazqb.com/Article/details/gzexxwims.sHtML

[U107] JS：数字千分位
来源：http://read.share.fktsv.cn/Article/details/ghugyxgwp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fktsv.cn/Article/details/ghqreuloc.sHtML

[U108] JS：随机整数
来源：http://read.share.tarul.cn/Article/details/gkkgszjss.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.tarul.cn/Article/details/gmuatqnfx.sHtML

[U109] JS：数组分组
来源：http://m.share.bbcook.cn/Article/details/garbvggpv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.sjlbkw.cn/Article/details/grvatyuof.sHtML

[U110] JS：数组分块
来源：http://blog.tarul.cn/Article/details/gcoswfbxc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.vehdjk.com/Article/details/guwhiqbkb.sHtML

[U111] JS：对象转 Map
来源：http://blog.bbcook.cn/Article/details/gpeaqtebk.sHtML

new Map(Object.entries(obj))
来源：http://3g.sjlbkw.cn/Article/details/gvwcsrrfo.sHtML

[U112] JS：字符串补位
来源：http://mobile.yfazqb.com/Article/details/gfztejmrg.sHtML

"7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gktbxrwan.sHtML

[U113] JS：正则替换全部
来源：http://read.share.epnwcf.com/Article/details/glrbrccxt.sHtML

s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gpijoxjas.sHtML

[U114] JS：JSON 深比较
来源：http://baike.yfazqb.com/Article/details/ggguorbjl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.bbcook.cn/Article/details/goomkuvbj.sHtML

[U115] JS：生成 UUID
来源：http://wap.bbcook.cn/Article/details/gdrnvukdb.sHtML

crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gzbgysnpp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.vehdjk.com/Article/details/gnxrlmyhb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.sjlbkw.cn/Article/details/grjxnducn.sHtML

[U117] JS：单元测试
来源：http://blog.fktsv.cn/Article/details/gwdhellpt.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.bbcook.cn/Article/details/gcxzfsgfc.sHtML

[U118] JS：开发服务器
来源：http://www.share.yfazqb.com/Article/details/gvycyqwxh.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.vehdjk.com/Article/details/gsdyztjme.sHtML

[U119] JS：生产构建
来源：http://mobile.yfazqb.com/Article/details/ganmmdjau.sHtML

npx vite build
来源：http://read.share.yfazqb.com/Article/details/ggtvbneht.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.sjlbkw.cn/Article/details/gcovjhzot.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.epnwcf.com/Article/details/gxreluurg.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gsauldqpd.sHtML

统计汇总
来源：http://baike.bbcook.cn/Article/details/gzykbmalx.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gficvhpyu.sHtML

按语言统计（条）：
来源：http://3g.sjlbkw.cn/Article/details/gcggtuuig.sHtML

Python ......... 252
来源：http://www.share.yfazqb.com/Article/details/gzyfdyene.sHtML

PHP ............ 252
来源：http://www.m.share.vehdjk.com/Article/details/gbgtmomfr.sHtML

JavaScript ..... 252
来源：http://www.blog.yfazqb.com/Article/details/gdfryswtt.sHtML

TypeScript ..... 212
来源：http://m.share.vehdjk.com/Article/details/gkrqeqrkk.sHtML

Java ........... 212
来源：http://blog.yfazqb.com/Article/details/ghbkwpqol.sHtML

Go ............. 212
来源：http://blog.epnwcf.com/Article/details/gzywofwey.sHtML

Ruby ........... 212
来源：http://mobile.sjlbkw.cn/Article/details/ggjknkobx.sHtML

C# ............. 212
来源：http://baike.fktsv.cn/Article/details/gflizoegn.sHtML

C .............. 30
来源：http://www.blog.epnwcf.com/Article/details/gluawbxhg.sHtML

C++ ............ 30
来源：http://m.share.vehdjk.com/Article/details/guyeregjl.sHtML

SQL ............ 90
来源：http://www.m.share.epnwcf.com/Article/details/gyylueghj.sHtML

Bash ........... 80
来源：http://www.m.share.tarul.cn/Article/details/gjlgwmdaq.sHtML

Kotlin ......... 15
来源：http://m.share.fktsv.cn/Article/details/gmevjwqpc.sHtML

Swift .......... 15
来源：http://blog.vehdjk.com/Article/details/gpmneqwnz.sHtML

Lua ............ 10
来源：http://www.share.fktsv.cn/Article/details/grxoiuyzz.sHtML

Perl ........... 10
来源：http://blog.bbcook.cn/Article/details/geejnqbpq.sHtML

Scala .......... 10
来源：http://read.share.vehdjk.com/Article/details/giembmgix.sHtML

------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gjtchswvc.sHtML

合计 ........... 2106 条
来源：http://baike.tarul.cn/Article/details/gpwwtqggw.sHtML

按章节统计：
来源：http://read.share.epnwcf.com/Article/details/gmexrxazc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fktsv.cn/Article/details/gepkyqerq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.bbcook.cn/Article/details/gyjjpzqkb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.tarul.cn/Article/details/gldlqyfzc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.tarul.cn/Article/details/ghzlqpvxy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.vehdjk.com/Article/details/gciycsusr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.vehdjk.com/Article/details/gicvqatel.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/gxlauyyrw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.tarul.cn/Article/details/gffsqjbov.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gvpaekstl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fktsv.cn/Article/details/gwlkclper.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gmkmudfyd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvfhavyh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/guolsiccl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.vehdjk.com/Article/details/gltjsgltg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.bbcook.cn/Article/details/gprtcbekv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/ghdywgeav.sHtML

Q SQL 专题                              90
来源：http://www.blog.fktsv.cn/Article/details/gjssvwbcy.sHtML

R Bash 专题                             80
来源：http://mobile.fktsv.cn/Article/details/gtbjrcvaa.sHtML

S C / C++ 专题                          60
来源：http://mobile.sjlbkw.cn/Article/details/gfvgfzfgd.sHtML

T 其他语言补充                          60
来源：http://read.share.yfazqb.com/Article/details/gimmmztfn.sHtML

U 高频实用片段                         120
来源：http://www.blog.epnwcf.com/Article/details/gdeldgtbt.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/griagzxpy.sHtML

合计                                  2106 条
来源：http://blog.tarul.cn/Article/details/gwlncmewn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.vehdjk.com/Article/details/gegxygtpd.sHtML

使用提醒
来源：http://www.blog.yfazqb.com/Article/details/gthvzuhzx.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gnsqwnadc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.yfazqb.com/Article/details/gpjklnyyf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fktsv.cn/Article/details/gafcfafnj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.tarul.cn/Article/details/gsdbdxphu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.bbcook.cn/Article/details/gpfnaiqeg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.sjlbkw.cn/Article/details/guusjyhkq.sHtML

—— 文件结束 ——
来源：http://www.m.share.sjlbkw.cn/Article/details/genukgbip.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gfiffwyjv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.sjlbkw.cn/Article/details/ggxqvfvts.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.epnwcf.com/Article/details/givvhrmpn.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/glagimlhk.sHtML

【收录内容】
来源：http://www.blog.fktsv.cn/Article/details/gwhovlvff.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.epnwcf.com/Article/details/gxbchjamh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fktsv.cn/Article/details/gtlvhrfws.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fktsv.cn/Article/details/gfnmnxble.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.epnwcf.com/Article/details/gafenpqqy.sHtML

【使用说明】
来源：http://wap.epnwcf.com/Article/details/gqqqwmoyk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.sjlbkw.cn/Article/details/gqrdxpqxa.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.vehdjk.com/Article/details/ggofprilr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.yfazqb.com/Article/details/gvlmhbave.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.bbcook.cn/Article/details/gziihcnpc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.vehdjk.com/Article/details/grkjzkrrj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.yfazqb.com/Article/details/gmpemguna.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.vehdjk.com/Article/details/gckdvvzit.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.vehdjk.com/Article/details/giumhtlni.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.yfazqb.com/Article/details/gjcxbwozt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.vehdjk.com/Article/details/guwteiumd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.tarul.cn/Article/details/gctmkigcp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.epnwcf.com/Article/details/gfhzcurag.sHtML

【文件统计】
来源：http://baike.sjlbkw.cn/Article/details/gfwhfwauk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.bbcook.cn/Article/details/gwsloareb.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fktsv.cn/Article/details/gyvevvuhn.sHtML

目  录
来源：http://baike.epnwcf.com/Article/details/gepgeekqt.sHtML

--------------------------------------------------------------------------------
来源：http://baike.bbcook.cn/Article/details/gnikjlcfb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.tarul.cn/Article/details/giusfmcow.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.bbcook.cn/Article/details/gskelmclr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/goeqifmvn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.tarul.cn/Article/details/gcoiblxms.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.tarul.cn/Article/details/ghcddlpmj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.vehdjk.com/Article/details/gznnacsfw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.bbcook.cn/Article/details/gbqptcmbi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.sjlbkw.cn/Article/details/gkgpxhfjg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/gtflwhcid.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.vehdjk.com/Article/details/gdqojscmw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fktsv.cn/Article/details/gbymijcgc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/glzcoizxl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.epnwcf.com/Article/details/gyavwkjia.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.epnwcf.com/Article/details/grjdcsglg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.tarul.cn/Article/details/gcclviyvg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.epnwcf.com/Article/details/gbmkvrkul.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.tarul.cn/Article/details/griqgisjd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.bbcook.cn/Article/details/gkowaixov.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.tarul.cn/Article/details/geuhrjacy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gyhtwztbi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.tarul.cn/Article/details/gbngmxpuz.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gmdppprhn.sHtML

A. 基础语法与类型
来源：http://www.share.tarul.cn/Article/details/gojzvkbyo.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ghvzkikre.sHtML

[A01] Hello World
来源：http://www.blog.vehdjk.com/Article/details/grskaffeh.sHtML

Py:   print("Hello, World!")
来源：http://m.share.vehdjk.com/Article/details/glkpdzoax.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.epnwcf.com/Article/details/gtfsifbxw.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.epnwcf.com/Article/details/goonfytlr.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fktsv.cn/Article/details/guccelhyu.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.vehdjk.com/Article/details/gkysvuamj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.epnwcf.com/Article/details/gaaadjudo.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.vehdjk.com/Article/details/ghiphqvbp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.tarul.cn/Article/details/gazjnfuxt.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fktsv.cn/Article/details/gptnkfmxd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.yfazqb.com/Article/details/gxkrlhyra.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.vehdjk.com/Article/details/gmeijkzfj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.bbcook.cn/Article/details/gidmmvxmp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.vehdjk.com/Article/details/ggqfywszi.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.bbcook.cn/Article/details/giornmtwh.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fktsv.cn/Article/details/gsxesghip.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fktsv.cn/Article/details/gpilkrpkr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.bbcook.cn/Article/details/gqflhpzpx.sHtML

[A03] 常量定义
来源：http://m.share.yfazqb.com/Article/details/gbvonlckb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.vehdjk.com/Article/details/gzbqzduxp.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gwgdtxnje.sHtML

JS:   const PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/ghfylskhb.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.vehdjk.com/Article/details/grumfwada.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fktsv.cn/Article/details/gmtyotpht.sHtML

Go:   const PI = 3.14159
来源：http://3g.epnwcf.com/Article/details/gtfiqoqwy.sHtML

Ruby: PI = 3.14159
来源：http://read.share.epnwcf.com/Article/details/gmnazwyxu.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/getfwefli.sHtML

[A04] 判断变量类型
来源：http://m.share.epnwcf.com/Article/details/gardboojf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.yfazqb.com/Article/details/gzecearkz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fktsv.cn/Article/details/gjrglouso.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.sjlbkw.cn/Article/details/grlxovwks.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.tarul.cn/Article/details/ghmljzcjj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.yfazqb.com/Article/details/gugfofckh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.vehdjk.com/Article/details/gyobswnys.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fktsv.cn/Article/details/gzotlcrod.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.vehdjk.com/Article/details/gusknpprn.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fktsv.cn/Article/details/gdwudbqik.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.bbcook.cn/Article/details/gxlnkhwng.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.tarul.cn/Article/details/guefquhyf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.epnwcf.com/Article/details/gvabviznv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.sjlbkw.cn/Article/details/gddiwpjtc.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gifgtzqec.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fktsv.cn/Article/details/gtjwmaary.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/ggjcryfte.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.epnwcf.com/Article/details/gdxulbxxq.sHtML

[A06] 字符串转数字
来源：http://www.m.share.yfazqb.com/Article/details/ghbboxtqc.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.vehdjk.com/Article/details/gqdhmrusg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.vehdjk.com/Article/details/gsbmvsiax.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.bbcook.cn/Article/details/gqomgefmn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.bbcook.cn/Article/details/gsmrlkeyh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.vehdjk.com/Article/details/ggbvdkoyz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.vehdjk.com/Article/details/gxleqjnfp.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.vehdjk.com/Article/details/gsprhgvox.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.sjlbkw.cn/Article/details/gwescmmmz.sHtML

[A07] 数字转字符串
来源：http://www.blog.epnwcf.com/Article/details/gzciiltub.sHtML

Py:   str(42)
来源：http://blog.fktsv.cn/Article/details/grlmfapow.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.bbcook.cn/Article/details/gnaivokdy.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fktsv.cn/Article/details/gcggyddor.sHtML

TS:   String(42)
来源：http://3g.fktsv.cn/Article/details/gkrvhtufc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.bbcook.cn/Article/details/gwoeehqfw.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fktsv.cn/Article/details/gasyaubla.sHtML

Ruby: 42.to_s
来源：http://www.m.share.epnwcf.com/Article/details/gjbipltph.sHtML

C#:   42.ToString()
来源：http://wap.fktsv.cn/Article/details/gucdqciib.sHtML

[A08] 取整与四舍五入
来源：http://m.share.sjlbkw.cn/Article/details/gsyqpbyqt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.sjlbkw.cn/Article/details/goopwttyk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.tarul.cn/Article/details/guiedohcr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.bbcook.cn/Article/details/gbfxwezof.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.yfazqb.com/Article/details/gpsuutglv.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.sjlbkw.cn/Article/details/ghcrkqans.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.epnwcf.com/Article/details/gnylammzu.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.bbcook.cn/Article/details/gvgkwhrfr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/gexelyeao.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.yfazqb.com/Article/details/glyyujatd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.epnwcf.com/Article/details/gsgohndid.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gwqgcfnkr.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.vehdjk.com/Article/details/gaxdokoxt.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/guokmqdmh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.yfazqb.com/Article/details/gbuaewxoc.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.vehdjk.com/Article/details/gvlofyswk.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.bbcook.cn/Article/details/gmdtvklrl.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.yfazqb.com/Article/details/gfwcfmwlh.sHtML

[A10] 生成随机数
来源：http://blog.bbcook.cn/Article/details/gbsygvxgn.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fktsv.cn/Article/details/guhhmanfe.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.bbcook.cn/Article/details/gzumneihy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.sjlbkw.cn/Article/details/gtgivclhm.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.sjlbkw.cn/Article/details/ghcfcnkaz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.sjlbkw.cn/Article/details/gpqpfcqxf.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.bbcook.cn/Article/details/gzyfzuztg.sHtML

Ruby: rand(1..100)
来源：http://mobile.epnwcf.com/Article/details/gsdspuwjy.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.tarul.cn/Article/details/gxeijzztp.sHtML

[A11] 条件表达式（三元）
来源：http://wap.bbcook.cn/Article/details/ghufrnrmw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.bbcook.cn/Article/details/glxiqkbid.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.epnwcf.com/Article/details/gumhcjxfk.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.vehdjk.com/Article/details/gmfznvnan.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.vehdjk.com/Article/details/gfgbjgghs.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.sjlbkw.cn/Article/details/ggltrmquk.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.vehdjk.com/Article/details/gnalezvtj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.fktsv.cn/Article/details/gbdmgipmq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.epnwcf.com/Article/details/gjxgjfwkd.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.fktsv.cn/Article/details/goxnwucii.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.epnwcf.com/Article/details/gwjwmfsxm.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.epnwcf.com/Article/details/gwqjvrztk.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fktsv.cn/Article/details/ggukhfphu.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.yfazqb.com/Article/details/gwtnsnkvg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.vehdjk.com/Article/details/gwrdantqk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.yfazqb.com/Article/details/gbdjahagi.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.yfazqb.com/Article/details/gkvhopwzt.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.tarul.cn/Article/details/gtyxvfdff.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fktsv.cn/Article/details/grsonhkln.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/gwwjaairr.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/gogvwgfdz.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/gzvxzpsfz.sHtML

TS:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gsduxoxmq.sHtML

Java: "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/gykqcazuu.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.epnwcf.com/Article/details/gkrjdwvhw.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/gbkusgwkm.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/gstzcsyju.sHtML

[A14] 注释写法
来源：http://wap.fktsv.cn/Article/details/gqcsxippi.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.bbcook.cn/Article/details/gdszgktde.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.yfazqb.com/Article/details/grjcmmkbg.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/gvhtwdvnl.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.tarul.cn/Article/details/gucwjdupp.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.tarul.cn/Article/details/gxjdnujtm.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.tarul.cn/Article/details/gadbjrqjk.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.yfazqb.com/Article/details/gbvyhrirn.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.vehdjk.com/Article/details/gmonwkjcy.sHtML

[A15] 空值判断与默认值
来源：http://read.share.yfazqb.com/Article/details/giqdlotha.sHtML

Py:   value = data or "默认值"
来源：http://m.share.epnwcf.com/Article/details/gpvpmajwd.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.vehdjk.com/Article/details/gclfxtnyp.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.sjlbkw.cn/Article/details/gvwvlidwt.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.sjlbkw.cn/Article/details/geeaoylhz.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.vehdjk.com/Article/details/gimuhlvui.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.tarul.cn/Article/details/ghoqsmapo.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.sjlbkw.cn/Article/details/gxnactwev.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.epnwcf.com/Article/details/gzxthkzdr.sHtML

[A16] 真假值判断规则
来源：http://blog.yfazqb.com/Article/details/gkoxlubah.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fktsv.cn/Article/details/grluregif.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.sjlbkw.cn/Article/details/gwhvqvbzb.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.bbcook.cn/Article/details/gkqeadzda.sHtML

TS:   if (!x) {}
来源：http://www.blog.yfazqb.com/Article/details/gwxmsysab.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.bbcook.cn/Article/details/ggfxixbak.sHtML


<!-- 参考信息 -->