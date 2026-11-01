代发 wailian999

[U93] JS：模板字符串
来源：http://read.share.tarul.cn/Article/details/gknksmkjp.sHtML

`共 ${n} 条`
来源：http://m.share.sjlbkw.cn/Article/details/gokjzmsua.sHtML

[U94] JS：箭头函数
来源：http://www.blog.yfazqb.com/Article/details/ggqyavlsj.sHtML

const double = x => x * 2;
来源：http://read.share.epnwcf.com/Article/details/gusbzdwzc.sHtML

[U95] JS：Promise 包装
来源：http://wap.fktsv.cn/Article/details/gzpxqmidz.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.bbcook.cn/Article/details/gozwnppxw.sHtML

[U96] JS：async/await 与异常
来源：http://wap.sjlbkw.cn/Article/details/gnpqnweeu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.tarul.cn/Article/details/gasydjplz.sHtML

[U97] JS：并发请求
来源：http://mobile.epnwcf.com/Article/details/gxgargvag.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gdhecjfhw.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.tarul.cn/Article/details/gpmwpfzgv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.tarul.cn/Article/details/guygkyydv.sHtML

[U99] JS：事件监听
来源：http://www.blog.fktsv.cn/Article/details/gasclptkl.sHtML

el.addEventListener("click", e => {})
来源：http://blog.sjlbkw.cn/Article/details/gesqtznxz.sHtML

[U100] JS：DOM 查询
来源：http://blog.vehdjk.com/Article/details/gztzsgtcq.sHtML

document.querySelector(".item")
来源：http://baike.tarul.cn/Article/details/ghjisrjio.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.epnwcf.com/Article/details/ggecjueao.sHtML

el.classList.toggle("active")
来源：http://wap.fktsv.cn/Article/details/gjihjwhcw.sHtML

[U102] JS：本地存储
来源：http://mobile.yfazqb.com/Article/details/gnikfaxaa.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.bbcook.cn/Article/details/gaidhvfjj.sHtML

[U103] JS：定时器
来源：http://read.share.tarul.cn/Article/details/gjdqumnbe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.bbcook.cn/Article/details/gqqtxicrn.sHtML

[U104] JS：防抖
来源：http://m.share.fktsv.cn/Article/details/gqxeaieor.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fktsv.cn/Article/details/gkvbrbkww.sHtML

[U105] JS：节流
来源：http://wap.fktsv.cn/Article/details/gycrggzkc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fktsv.cn/Article/details/gxtrqhzfk.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fktsv.cn/Article/details/gkppwwlwm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.sjlbkw.cn/Article/details/gtssdvaek.sHtML

[U107] JS：数字千分位
来源：http://www.share.fktsv.cn/Article/details/gfxzclygy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.vehdjk.com/Article/details/gnyvyduro.sHtML

[U108] JS：随机整数
来源：http://m.share.tarul.cn/Article/details/gerurypak.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.epnwcf.com/Article/details/gjfjqmuxo.sHtML

[U109] JS：数组分组
来源：http://blog.yfazqb.com/Article/details/gitnsenva.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.epnwcf.com/Article/details/ghbgbyuyp.sHtML

[U110] JS：数组分块
来源：http://www.share.yfazqb.com/Article/details/grixigbzq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.sjlbkw.cn/Article/details/gubkdsnpd.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.vehdjk.com/Article/details/gyntafcpd.sHtML

new Map(Object.entries(obj))
来源：http://mobile.vehdjk.com/Article/details/gsrdgytmg.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fktsv.cn/Article/details/gaqzryysk.sHtML

"7".padStart(3, "0")
来源：http://blog.vehdjk.com/Article/details/gtbjjryip.sHtML

[U113] JS：正则替换全部
来源：http://blog.sjlbkw.cn/Article/details/gqvpfvwyp.sHtML

s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gafbkcfdk.sHtML

[U114] JS：JSON 深比较
来源：http://baike.sjlbkw.cn/Article/details/gmqvwwpeo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.vehdjk.com/Article/details/ghaksoimv.sHtML

[U115] JS：生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/gcdaxaijo.sHtML

crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/gnzxzctrh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.yfazqb.com/Article/details/gqfzbhaft.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fktsv.cn/Article/details/gwicbjqof.sHtML

[U117] JS：单元测试
来源：http://baike.sjlbkw.cn/Article/details/gzyfxgjog.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.epnwcf.com/Article/details/gtwqbarfw.sHtML

[U118] JS：开发服务器
来源：http://wap.bbcook.cn/Article/details/gpwzzzetv.sHtML

npm i -D vite;  npx vite
来源：http://3g.fktsv.cn/Article/details/gisykgctf.sHtML

[U119] JS：生产构建
来源：http://3g.tarul.cn/Article/details/gsotyelyb.sHtML

npx vite build
来源：http://3g.epnwcf.com/Article/details/gsmipndxy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.sjlbkw.cn/Article/details/glpmhaoyi.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.sjlbkw.cn/Article/details/gdxvqfnna.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gpimetksi.sHtML

统计汇总
来源：http://read.share.fktsv.cn/Article/details/gewlwvkxo.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/givzeshus.sHtML

按语言统计（条）：
来源：http://m.share.vehdjk.com/Article/details/gbiyuhwqp.sHtML

Python ......... 252
来源：http://www.blog.epnwcf.com/Article/details/gzplkkwhd.sHtML

PHP ............ 252
来源：http://www.m.share.tarul.cn/Article/details/gychmdhet.sHtML

JavaScript ..... 252
来源：http://blog.tarul.cn/Article/details/gjjtevsrj.sHtML

TypeScript ..... 212
来源：http://www.blog.tarul.cn/Article/details/gctewcxgo.sHtML

Java ........... 212
来源：http://baike.tarul.cn/Article/details/gemjgvrte.sHtML

Go ............. 212
来源：http://wap.yfazqb.com/Article/details/gchganntz.sHtML

Ruby ........... 212
来源：http://3g.vehdjk.com/Article/details/gxnlfyfyn.sHtML

C# ............. 212
来源：http://www.m.share.tarul.cn/Article/details/gpryvcbwg.sHtML

C .............. 30
来源：http://www.m.share.yfazqb.com/Article/details/geykjyamd.sHtML

C++ ............ 30
来源：http://blog.tarul.cn/Article/details/gspbiwbew.sHtML

SQL ............ 90
来源：http://baike.tarul.cn/Article/details/gjkgtarsj.sHtML

Bash ........... 80
来源：http://baike.vehdjk.com/Article/details/gbxdzsfyk.sHtML

Kotlin ......... 15
来源：http://mobile.bbcook.cn/Article/details/gosjbjszf.sHtML

Swift .......... 15
来源：http://blog.sjlbkw.cn/Article/details/gyhiqewid.sHtML

Lua ............ 10
来源：http://wap.sjlbkw.cn/Article/details/gytcpybjr.sHtML

Perl ........... 10
来源：http://m.share.yfazqb.com/Article/details/gwkgdapyd.sHtML

Scala .......... 10
来源：http://read.share.fktsv.cn/Article/details/gboiwwhuo.sHtML

------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gmiuzmfvz.sHtML

合计 ........... 2106 条
来源：http://www.share.bbcook.cn/Article/details/gpdltxhhy.sHtML

按章节统计：
来源：http://read.share.sjlbkw.cn/Article/details/gvaekkmag.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.bbcook.cn/Article/details/gcdnoyatg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fktsv.cn/Article/details/gohxvpiay.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.yfazqb.com/Article/details/gxnpqparl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fktsv.cn/Article/details/gjgfsoplu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.yfazqb.com/Article/details/guekzjfny.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fktsv.cn/Article/details/gbhectfhs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.bbcook.cn/Article/details/gdzytxxrs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.yfazqb.com/Article/details/gpmealhfq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gwxvlpbam.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.bbcook.cn/Article/details/getmjlgfh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/glthhtjyp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/gofljvckw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/gcjbarhaf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.epnwcf.com/Article/details/gdpontken.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.bbcook.cn/Article/details/goyswsbwp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.epnwcf.com/Article/details/gmdvznzbf.sHtML

Q SQL 专题                              90
来源：http://wap.fktsv.cn/Article/details/gjgafwduj.sHtML

R Bash 专题                             80
来源：http://www.share.bbcook.cn/Article/details/guxaantkd.sHtML

S C / C++ 专题                          60
来源：http://read.share.bbcook.cn/Article/details/gnfdajush.sHtML

T 其他语言补充                          60
来源：http://www.share.vehdjk.com/Article/details/gyieropum.sHtML

U 高频实用片段                         120
来源：http://blog.sjlbkw.cn/Article/details/gnpgfhqwt.sHtML

------------------------------------
来源：http://mobile.tarul.cn/Article/details/gnemfyvqs.sHtML

合计                                  2106 条
来源：http://www.blog.tarul.cn/Article/details/gvmtutrmk.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gliqvqlep.sHtML

使用提醒
来源：http://wap.bbcook.cn/Article/details/gyjfdilyo.sHtML

--------------------------------------------------------------------------------
来源：http://baike.vehdjk.com/Article/details/gyvjocsww.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.vehdjk.com/Article/details/gizscipyc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.epnwcf.com/Article/details/gaxynpowu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.yfazqb.com/Article/details/glzjqiycn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fktsv.cn/Article/details/grllygmoy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.yfazqb.com/Article/details/gmkinodef.sHtML

—— 文件结束 ——
来源：http://baike.vehdjk.com/Article/details/gddudwhix.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gdxjgogpt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.vehdjk.com/Article/details/guxsmjolb.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.sjlbkw.cn/Article/details/gxmmdiiqc.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gcciqynnq.sHtML

【收录内容】
来源：http://m.share.epnwcf.com/Article/details/gifiwrolf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.yfazqb.com/Article/details/gycmcacxa.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.vehdjk.com/Article/details/gxxtakhfj.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fktsv.cn/Article/details/glsvalphv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.yfazqb.com/Article/details/gqdxxdqzd.sHtML

【使用说明】
来源：http://www.share.sjlbkw.cn/Article/details/gzqwgfpks.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.sjlbkw.cn/Article/details/guoethqny.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fktsv.cn/Article/details/ghtjhlxqt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.epnwcf.com/Article/details/gaxyxkvsa.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fktsv.cn/Article/details/gyjfvmyfi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkdoqwzo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.sjlbkw.cn/Article/details/ghojliewo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.epnwcf.com/Article/details/gpekmyhmh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.yfazqb.com/Article/details/gntvncxuf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fktsv.cn/Article/details/gvxbdfurs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.bbcook.cn/Article/details/gcorqwsxd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.sjlbkw.cn/Article/details/gcsdgvobr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.epnwcf.com/Article/details/gmpkyruns.sHtML

【文件统计】
来源：http://3g.tarul.cn/Article/details/ghrrroeea.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fktsv.cn/Article/details/gsfildyga.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gxnefqftq.sHtML

目  录
来源：http://baike.vehdjk.com/Article/details/guyiwrhgf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gdklzpqvm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.tarul.cn/Article/details/gogcmqjkr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.bbcook.cn/Article/details/gkomspxil.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fktsv.cn/Article/details/gqbzfknig.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.vehdjk.com/Article/details/gwegytgqf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fktsv.cn/Article/details/grhfqdohx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.sjlbkw.cn/Article/details/gxstuqvpl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.tarul.cn/Article/details/gebthuoxy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fktsv.cn/Article/details/gssxckpgf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/guudjoiio.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fktsv.cn/Article/details/gpbtlrrsx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.yfazqb.com/Article/details/gyvutefky.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.vehdjk.com/Article/details/gizvxsdky.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/gysoycacm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.yfazqb.com/Article/details/gdxjrvzlz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fktsv.cn/Article/details/gfptigwda.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/gnlhqywgj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.epnwcf.com/Article/details/gekftyyxy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.yfazqb.com/Article/details/gotemxyre.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fktsv.cn/Article/details/gcxagcoip.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.bbcook.cn/Article/details/gtieinsic.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.vehdjk.com/Article/details/gokhsvsyg.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/glygmmimm.sHtML

A. 基础语法与类型
来源：http://www.m.share.fktsv.cn/Article/details/gvvtylpsd.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gosryeain.sHtML

[A01] Hello World
来源：http://wap.fktsv.cn/Article/details/gamjyjzsl.sHtML

Py:   print("Hello, World!")
来源：http://blog.sjlbkw.cn/Article/details/gbzjwmiba.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.tarul.cn/Article/details/gpsryphko.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.yfazqb.com/Article/details/gbsuunlns.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.epnwcf.com/Article/details/gujzoroeo.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.vehdjk.com/Article/details/gcpauckyb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.tarul.cn/Article/details/gvzpqiubk.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.epnwcf.com/Article/details/giqgxxgsv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.yfazqb.com/Article/details/grylyekvy.sHtML

[A02] 变量声明与赋值
来源：http://read.share.yfazqb.com/Article/details/ggcwittul.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.sjlbkw.cn/Article/details/ggdqttnyi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.bbcook.cn/Article/details/gkamsfvpr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.tarul.cn/Article/details/ghdtcbwui.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gouifnmjz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.vehdjk.com/Article/details/gfnaibsym.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.sjlbkw.cn/Article/details/ggmwoupfj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.epnwcf.com/Article/details/glrxubovm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.epnwcf.com/Article/details/gcvsxssnq.sHtML

[A03] 常量定义
来源：http://read.share.vehdjk.com/Article/details/gtzqhbsyb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fktsv.cn/Article/details/gbydyalvz.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gvzeywckw.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gfhwnuuyl.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gcmugzyxe.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gmpidscax.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.tarul.cn/Article/details/gptcnruec.sHtML

Ruby: PI = 3.14159
来源：http://3g.epnwcf.com/Article/details/gfekewikq.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gtvtajmyk.sHtML

[A04] 判断变量类型
来源：http://blog.epnwcf.com/Article/details/gffhrpovs.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.yfazqb.com/Article/details/gsqmjomer.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.tarul.cn/Article/details/gjmaazade.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.yfazqb.com/Article/details/gubaeldgm.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.yfazqb.com/Article/details/gwkcudpxn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.tarul.cn/Article/details/glahbbejp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.tarul.cn/Article/details/gdejqvxfg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.vehdjk.com/Article/details/gdnwnnwtz.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.yfazqb.com/Article/details/gvwqqyohw.sHtML

[A05] 整数除法与取模
来源：http://3g.epnwcf.com/Article/details/guifwditw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.yfazqb.com/Article/details/gudbnoypn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.bbcook.cn/Article/details/gfdadicfv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.bbcook.cn/Article/details/gffgcqhhf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.yfazqb.com/Article/details/gqtcbkcxx.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.tarul.cn/Article/details/gwvymgixf.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gqpciataa.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.vehdjk.com/Article/details/gibskbvro.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.tarul.cn/Article/details/gnqripnpf.sHtML

[A06] 字符串转数字
来源：http://blog.vehdjk.com/Article/details/gotfhmned.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fktsv.cn/Article/details/gurnmznva.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.vehdjk.com/Article/details/gbtzzkusn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.yfazqb.com/Article/details/gnvycuxyo.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.tarul.cn/Article/details/gnbhzgcuj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fktsv.cn/Article/details/gfpxiiabl.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fktsv.cn/Article/details/gqcvetspg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.epnwcf.com/Article/details/gvdsrpwkm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.sjlbkw.cn/Article/details/gjdpskpcd.sHtML

[A07] 数字转字符串
来源：http://3g.epnwcf.com/Article/details/gxsvmjkhg.sHtML

Py:   str(42)
来源：http://m.share.bbcook.cn/Article/details/gfsisunqa.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.yfazqb.com/Article/details/gaivmztle.sHtML

JS:   String(42); (42).toString()
来源：http://3g.yfazqb.com/Article/details/gkocuyplo.sHtML

TS:   String(42)
来源：http://www.m.share.bbcook.cn/Article/details/gnnkuchcr.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.vehdjk.com/Article/details/gnjguppyk.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.yfazqb.com/Article/details/gzrqtfjcv.sHtML

Ruby: 42.to_s
来源：http://www.share.tarul.cn/Article/details/ggaekvvdw.sHtML

C#:   42.ToString()
来源：http://3g.sjlbkw.cn/Article/details/gvnuqapbp.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.bbcook.cn/Article/details/geuuutbis.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fktsv.cn/Article/details/gkhrenjgj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.epnwcf.com/Article/details/gbmbjdita.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.vehdjk.com/Article/details/gmbbaobrt.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.bbcook.cn/Article/details/gbrudvihh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fktsv.cn/Article/details/ggukogtav.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.epnwcf.com/Article/details/giiesmrca.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.tarul.cn/Article/details/gmhtpgonb.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fktsv.cn/Article/details/gefahsazi.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fktsv.cn/Article/details/gdiresosz.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.epnwcf.com/Article/details/gkdllshwc.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.bbcook.cn/Article/details/glrnerrug.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.yfazqb.com/Article/details/griqfqfbb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.bbcook.cn/Article/details/gomzahwgn.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.bbcook.cn/Article/details/glwsdypgw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.bbcook.cn/Article/details/gfomaupzf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.fktsv.cn/Article/details/gvfyqlqhi.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.yfazqb.com/Article/details/gwnwsdjll.sHtML

[A10] 生成随机数
来源：http://wap.yfazqb.com/Article/details/gwdrhoycr.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fktsv.cn/Article/details/gxwbbrcew.sHtML

PHP:  random_int(1, 100);
来源：http://wap.vehdjk.com/Article/details/gsvjvydor.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fktsv.cn/Article/details/gnixeoazk.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.vehdjk.com/Article/details/gdvpjcjik.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fktsv.cn/Article/details/gkrplznzj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.vehdjk.com/Article/details/gwaakskrg.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fktsv.cn/Article/details/guicokvcg.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.yfazqb.com/Article/details/gtzspntfv.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.sjlbkw.cn/Article/details/gvcfswwbi.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.vehdjk.com/Article/details/gjmwfqwzy.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.tarul.cn/Article/details/gnfbruycq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.epnwcf.com/Article/details/gzqimobdo.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.bbcook.cn/Article/details/gzfwvkcdc.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.tarul.cn/Article/details/gjygoahca.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.fktsv.cn/Article/details/gqfvhyrey.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.tarul.cn/Article/details/gfpkxfgeo.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.epnwcf.com/Article/details/gfsdcoxyx.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvellilp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.bbcook.cn/Article/details/gespibang.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.sjlbkw.cn/Article/details/gsuxdjfpi.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.vehdjk.com/Article/details/gtdvzojrg.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.sjlbkw.cn/Article/details/gwrgaqwwt.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.bbcook.cn/Article/details/gfvnxfmpl.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.epnwcf.com/Article/details/gpzeckvfg.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.vehdjk.com/Article/details/gsldydtze.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.sjlbkw.cn/Article/details/gcsfbdkzf.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.tarul.cn/Article/details/goulavrru.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gpkstkqzc.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.epnwcf.com/Article/details/gredgajnl.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/ghxncvdgk.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/gqzqszwwk.sHtML

Java: "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/gmegefqra.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/gaccpsfdw.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/gpjozscct.sHtML

C#:   "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gslwiwhri.sHtML

[A14] 注释写法
来源：http://m.share.epnwcf.com/Article/details/gsiwpzkxd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.vehdjk.com/Article/details/gwdmoaapa.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fktsv.cn/Article/details/gqhdnanyt.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.sjlbkw.cn/Article/details/gazgrtzrq.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gndzkonmz.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.yfazqb.com/Article/details/ggdgnsgiy.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/gwhnqbfop.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.yfazqb.com/Article/details/grkxveqvv.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.epnwcf.com/Article/details/gvxjcjzfe.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.vehdjk.com/Article/details/gyuqrfeyr.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.fktsv.cn/Article/details/gqewfzlmj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.vehdjk.com/Article/details/gchwobfxo.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.sjlbkw.cn/Article/details/gsptreodt.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.tarul.cn/Article/details/gbukbvlml.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.bbcook.cn/Article/details/grbddmfjn.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.bbcook.cn/Article/details/gonlhkwqs.sHtML

Ruby: value = data || "默认值"
来源：http://baike.vehdjk.com/Article/details/gvlweeoiv.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbqjmcox.sHtML

[A16] 真假值判断规则
来源：http://read.share.fktsv.cn/Article/details/gqzryulpt.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.yfazqb.com/Article/details/gmlbxdlhg.sHtML


<!-- 参考信息 -->