代发 wailian999

[U91] JS：对象键值遍历
来源：http://baike.vehdjk.com/Article/details/geoaajjym.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.tarul.cn/Article/details/glnwleajw.sHtML

[U92] JS：深拷贝
来源：http://3g.fktsv.cn/Article/details/gdvhivsxv.sHtML

structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/gklicwkdb.sHtML

[U93] JS：模板字符串
来源：http://www.share.yfazqb.com/Article/details/gzefcyqfi.sHtML

`共 ${n} 条`
来源：http://3g.fktsv.cn/Article/details/gngvjbzla.sHtML

[U94] JS：箭头函数
来源：http://blog.tarul.cn/Article/details/gbvveuroc.sHtML

const double = x => x * 2;
来源：http://wap.sjlbkw.cn/Article/details/gysgzfugd.sHtML

[U95] JS：Promise 包装
来源：http://3g.epnwcf.com/Article/details/gbftsnitm.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.vehdjk.com/Article/details/gdaftqfhz.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fktsv.cn/Article/details/glscdsvjh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gfztdrswc.sHtML

[U97] JS：并发请求
来源：http://baike.epnwcf.com/Article/details/geyhyxeyk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gzzcefaei.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.yfazqb.com/Article/details/gekcjyenk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.tarul.cn/Article/details/gwcbtfpfo.sHtML

[U99] JS：事件监听
来源：http://3g.yfazqb.com/Article/details/gsemjvwhu.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.sjlbkw.cn/Article/details/gesowosdu.sHtML

[U100] JS：DOM 查询
来源：http://m.share.sjlbkw.cn/Article/details/gtsupurfv.sHtML

document.querySelector(".item")
来源：http://www.share.bbcook.cn/Article/details/gpnwbpcqq.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fktsv.cn/Article/details/grcgeydwt.sHtML

el.classList.toggle("active")
来源：http://mobile.fktsv.cn/Article/details/geqlqmbyy.sHtML

[U102] JS：本地存储
来源：http://www.m.share.bbcook.cn/Article/details/gfdzfgxpq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.tarul.cn/Article/details/gfhqjaxvi.sHtML

[U103] JS：定时器
来源：http://www.share.yfazqb.com/Article/details/gtyitoygj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsieckzyt.sHtML

[U104] JS：防抖
来源：http://mobile.epnwcf.com/Article/details/ghswzyszm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fktsv.cn/Article/details/gbmtyhmqq.sHtML

[U105] JS：节流
来源：http://www.m.share.fktsv.cn/Article/details/gowxzxexp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.tarul.cn/Article/details/gunnpnlkf.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gyilhxoei.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.sjlbkw.cn/Article/details/gefewgpyt.sHtML

[U107] JS：数字千分位
来源：http://baike.yfazqb.com/Article/details/gaopjvszu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.bbcook.cn/Article/details/gyxqexgfh.sHtML

[U108] JS：随机整数
来源：http://www.m.share.bbcook.cn/Article/details/glcqtdzoo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.yfazqb.com/Article/details/gabykqglb.sHtML

[U109] JS：数组分组
来源：http://blog.bbcook.cn/Article/details/gzjucbqft.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.bbcook.cn/Article/details/ggkjkcqbq.sHtML

[U110] JS：数组分块
来源：http://read.share.tarul.cn/Article/details/gyhxczlqv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fktsv.cn/Article/details/gsbvcwzve.sHtML

[U111] JS：对象转 Map
来源：http://wap.epnwcf.com/Article/details/gnmmmqpeq.sHtML

new Map(Object.entries(obj))
来源：http://baike.epnwcf.com/Article/details/gvyrjexlt.sHtML

[U112] JS：字符串补位
来源：http://www.blog.yfazqb.com/Article/details/gtrkowfve.sHtML

"7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/gggiqynvp.sHtML

[U113] JS：正则替换全部
来源：http://www.share.vehdjk.com/Article/details/gisxivxgj.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gnxvqwofo.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.vehdjk.com/Article/details/gmvjwrxov.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.bbcook.cn/Article/details/gakzmllhn.sHtML

[U115] JS：生成 UUID
来源：http://wap.tarul.cn/Article/details/gxvcyeibr.sHtML

crypto.randomUUID()
来源：http://read.share.fktsv.cn/Article/details/gpmmrvsuv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.vehdjk.com/Article/details/gbjxbreap.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.epnwcf.com/Article/details/gexmzznrj.sHtML

[U117] JS：单元测试
来源：http://www.share.epnwcf.com/Article/details/ggcebdbsz.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fktsv.cn/Article/details/gehulaerq.sHtML

[U118] JS：开发服务器
来源：http://blog.bbcook.cn/Article/details/godqurtpr.sHtML

npm i -D vite;  npx vite
来源：http://read.share.bbcook.cn/Article/details/gcudfigbo.sHtML

[U119] JS：生产构建
来源：http://www.share.bbcook.cn/Article/details/gyqilgqdb.sHtML

npx vite build
来源：http://www.share.yfazqb.com/Article/details/gpkzgyaww.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.epnwcf.com/Article/details/gegdcrwpl.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.bbcook.cn/Article/details/gggktqjzm.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gwfnyqjpj.sHtML

统计汇总
来源：http://www.m.share.bbcook.cn/Article/details/goiimmnca.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggyhnmcbd.sHtML

按语言统计（条）：
来源：http://www.share.vehdjk.com/Article/details/gggfojckn.sHtML

Python ......... 252
来源：http://3g.fktsv.cn/Article/details/gqitaugjq.sHtML

PHP ............ 252
来源：http://wap.fktsv.cn/Article/details/grkcadtca.sHtML

JavaScript ..... 252
来源：http://www.blog.epnwcf.com/Article/details/guiwrklnb.sHtML

TypeScript ..... 212
来源：http://www.blog.bbcook.cn/Article/details/gdddcpwid.sHtML

Java ........... 212
来源：http://blog.yfazqb.com/Article/details/gdekwknnk.sHtML

Go ............. 212
来源：http://wap.epnwcf.com/Article/details/gznplptbw.sHtML

Ruby ........... 212
来源：http://blog.epnwcf.com/Article/details/gxxziwefd.sHtML

C# ............. 212
来源：http://www.share.bbcook.cn/Article/details/goavyvuvw.sHtML

C .............. 30
来源：http://www.share.vehdjk.com/Article/details/gpjxweyzd.sHtML

C++ ............ 30
来源：http://www.share.vehdjk.com/Article/details/gavlshmzy.sHtML

SQL ............ 90
来源：http://3g.epnwcf.com/Article/details/gfmjbzuqg.sHtML

Bash ........... 80
来源：http://m.share.fktsv.cn/Article/details/gkutpwyix.sHtML

Kotlin ......... 15
来源：http://blog.fktsv.cn/Article/details/giuypyzrw.sHtML

Swift .......... 15
来源：http://read.share.fktsv.cn/Article/details/glybfpqle.sHtML

Lua ............ 10
来源：http://baike.vehdjk.com/Article/details/gbdbfewyz.sHtML

Perl ........... 10
来源：http://baike.vehdjk.com/Article/details/gcmzvhxyy.sHtML

Scala .......... 10
来源：http://3g.sjlbkw.cn/Article/details/gcilgnrhe.sHtML

------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gsjcpvxov.sHtML

合计 ........... 2106 条
来源：http://3g.bbcook.cn/Article/details/gfvpfmhwk.sHtML

按章节统计：
来源：http://baike.fktsv.cn/Article/details/gzxtyjjss.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.yfazqb.com/Article/details/gyybgkbfu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/gdcwlbsyv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.tarul.cn/Article/details/guzpnfsyp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fktsv.cn/Article/details/gsudxrmdi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.epnwcf.com/Article/details/gbsjkqdzh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.yfazqb.com/Article/details/gjtbcreua.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.vehdjk.com/Article/details/gcczjgtkm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fktsv.cn/Article/details/goffkpxcw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/gnvhocokq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.yfazqb.com/Article/details/gylvtcglz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/geeymsfpy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/gfmpohgqj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gpoxxsdfu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.vehdjk.com/Article/details/gfdxymxue.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.bbcook.cn/Article/details/gxlxffgeo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gxyvtctak.sHtML

Q SQL 专题                              90
来源：http://blog.bbcook.cn/Article/details/gmwwxkxsi.sHtML

R Bash 专题                             80
来源：http://baike.tarul.cn/Article/details/gqxzmegef.sHtML

S C / C++ 专题                          60
来源：http://mobile.sjlbkw.cn/Article/details/gncegfrsz.sHtML

T 其他语言补充                          60
来源：http://www.m.share.tarul.cn/Article/details/grmmedklc.sHtML

U 高频实用片段                         120
来源：http://www.m.share.tarul.cn/Article/details/gskcakwwd.sHtML

------------------------------------
来源：http://read.share.yfazqb.com/Article/details/ggaavoxab.sHtML

合计                                  2106 条
来源：http://read.share.fktsv.cn/Article/details/glautwbkm.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gssaggdwm.sHtML

使用提醒
来源：http://www.blog.tarul.cn/Article/details/grlmuhiit.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gaenclzfp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fktsv.cn/Article/details/gqobhsdbz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fktsv.cn/Article/details/gjngzrmmv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.sjlbkw.cn/Article/details/gyxlqrubs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.vehdjk.com/Article/details/gljukzjcn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.tarul.cn/Article/details/gejnvtenz.sHtML

—— 文件结束 ——
来源：http://3g.vehdjk.com/Article/details/gagwxudei.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gvzpitsde.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.sjlbkw.cn/Article/details/gxpjceryo.sHtML

Common Programming Examples Cheat Book
来源：http://wap.bbcook.cn/Article/details/gcxytznad.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbekjfwbj.sHtML

【收录内容】
来源：http://read.share.sjlbkw.cn/Article/details/gcuplynpv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.bbcook.cn/Article/details/gsikjhtov.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.vehdjk.com/Article/details/gjrfxyvpb.sHtML

SQL · Bash · C · C++
来源：http://blog.yfazqb.com/Article/details/gndfmuuxi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.tarul.cn/Article/details/ghqqwkdwi.sHtML

【使用说明】
来源：http://mobile.epnwcf.com/Article/details/gotlyjwdc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.yfazqb.com/Article/details/gzlxrvpik.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fktsv.cn/Article/details/gcmlasuur.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fktsv.cn/Article/details/geuaokify.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.bbcook.cn/Article/details/gspabznip.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.vehdjk.com/Article/details/gzmxqtjrv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.tarul.cn/Article/details/gayfvqlbu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.tarul.cn/Article/details/gzquasveu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fktsv.cn/Article/details/ggcekrrrp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.sjlbkw.cn/Article/details/gjzgveafk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fktsv.cn/Article/details/ggxfqlpvj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.tarul.cn/Article/details/gzltgnvlz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.epnwcf.com/Article/details/gjrxjgkfd.sHtML

【文件统计】
来源：http://3g.tarul.cn/Article/details/gumczmhxk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.sjlbkw.cn/Article/details/gzqwodxcx.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gswlpzujm.sHtML

目  录
来源：http://mobile.epnwcf.com/Article/details/gkxrhjdfj.sHtML

--------------------------------------------------------------------------------
来源：http://wap.tarul.cn/Article/details/gwlxzubrr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.epnwcf.com/Article/details/gxjezqubv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.tarul.cn/Article/details/gycnndskn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.bbcook.cn/Article/details/grzucwqbe.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.vehdjk.com/Article/details/gtehldokq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.epnwcf.com/Article/details/gzrvoqzic.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.epnwcf.com/Article/details/gswtmqhtr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.sjlbkw.cn/Article/details/gozavymiu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.yfazqb.com/Article/details/glfcfthgt.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.sjlbkw.cn/Article/details/gqnxmxixn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.yfazqb.com/Article/details/gheuppakl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.yfazqb.com/Article/details/gjfoskulk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/gbfikhomu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.sjlbkw.cn/Article/details/getykyuga.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.sjlbkw.cn/Article/details/guyorwzac.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.tarul.cn/Article/details/gnedkblzf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/gplbivfme.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fktsv.cn/Article/details/gplpihoiy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.yfazqb.com/Article/details/ggzzchziy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.bbcook.cn/Article/details/grndpopet.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gqrtlrcgm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.vehdjk.com/Article/details/gkbthiawn.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ggbpniwtm.sHtML

A. 基础语法与类型
来源：http://mobile.vehdjk.com/Article/details/gxvruzhdk.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gvpfglbuq.sHtML

[A01] Hello World
来源：http://mobile.epnwcf.com/Article/details/gwsjjgbme.sHtML

Py:   print("Hello, World!")
来源：http://www.share.bbcook.cn/Article/details/gfkfsgibc.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.sjlbkw.cn/Article/details/gpvpbgqnk.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.epnwcf.com/Article/details/guksvdygi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.yfazqb.com/Article/details/gxfkcsftk.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.vehdjk.com/Article/details/gbulxvaph.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fktsv.cn/Article/details/gdsiszxpg.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.tarul.cn/Article/details/gbkfxktjq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.epnwcf.com/Article/details/gasnjisfg.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fktsv.cn/Article/details/gtdpgvyhh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.epnwcf.com/Article/details/gwvjvymzu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gpslxmrbq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.tarul.cn/Article/details/gnmmwbczx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.bbcook.cn/Article/details/grghzelce.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.vehdjk.com/Article/details/gmvyijuvl.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.tarul.cn/Article/details/glzcspmbl.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fktsv.cn/Article/details/gvbuemnqp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.bbcook.cn/Article/details/grxlvrnij.sHtML

[A03] 常量定义
来源：http://3g.sjlbkw.cn/Article/details/gfclntgjw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.tarul.cn/Article/details/gjocusqxu.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/grybpmqvf.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gutflwtpy.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gxawhdpeh.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gucrrqlit.sHtML

Go:   const PI = 3.14159
来源：http://mobile.sjlbkw.cn/Article/details/gsmahjrku.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.yfazqb.com/Article/details/gwtsxuawo.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gugaxzcli.sHtML

[A04] 判断变量类型
来源：http://www.blog.sjlbkw.cn/Article/details/gjjhugyyz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fktsv.cn/Article/details/guocaosze.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.epnwcf.com/Article/details/gaecyvajj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.vehdjk.com/Article/details/guqyxihea.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.epnwcf.com/Article/details/gujqsvzds.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fktsv.cn/Article/details/guwahqcjz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.yfazqb.com/Article/details/gpncfsekd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.vehdjk.com/Article/details/glxyuiasr.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.epnwcf.com/Article/details/goeegwjyr.sHtML

[A05] 整数除法与取模
来源：http://mobile.yfazqb.com/Article/details/gxkrdipfi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.epnwcf.com/Article/details/glupzrqqo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fktsv.cn/Article/details/ghnayyhje.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gwiptkobu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fktsv.cn/Article/details/gqvbtufwg.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.tarul.cn/Article/details/gahmlfdcs.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.tarul.cn/Article/details/gcljhyprw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gswktzgwh.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.bbcook.cn/Article/details/geadqnsbi.sHtML

[A06] 字符串转数字
来源：http://wap.tarul.cn/Article/details/guxzyesaj.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.vehdjk.com/Article/details/gpprotgau.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.sjlbkw.cn/Article/details/gvvzffvmq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.epnwcf.com/Article/details/gfyxdvyrw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.sjlbkw.cn/Article/details/gazpivzgs.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.tarul.cn/Article/details/gwqxiwvfw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.yfazqb.com/Article/details/ghcmlsuih.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.yfazqb.com/Article/details/gibuwulmt.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.epnwcf.com/Article/details/gawoiwsaz.sHtML

[A07] 数字转字符串
来源：http://www.blog.tarul.cn/Article/details/gykiefavt.sHtML

Py:   str(42)
来源：http://wap.tarul.cn/Article/details/gapsvufoc.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.vehdjk.com/Article/details/gkotcdcmj.sHtML

JS:   String(42); (42).toString()
来源：http://wap.sjlbkw.cn/Article/details/gveyrvlby.sHtML

TS:   String(42)
来源：http://www.blog.tarul.cn/Article/details/gipyxmpjo.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.epnwcf.com/Article/details/gumojubyd.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.tarul.cn/Article/details/gvwiycvhh.sHtML

Ruby: 42.to_s
来源：http://www.share.vehdjk.com/Article/details/gsrucxxdr.sHtML

C#:   42.ToString()
来源：http://www.m.share.bbcook.cn/Article/details/gpczjaazk.sHtML

[A08] 取整与四舍五入
来源：http://baike.bbcook.cn/Article/details/gnqwmsfgo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.tarul.cn/Article/details/gffmsicou.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.bbcook.cn/Article/details/gavfqxqsb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/gsfdgkbxa.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.yfazqb.com/Article/details/gweqqmznf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.sjlbkw.cn/Article/details/gcaisvxeb.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fktsv.cn/Article/details/gxbkxjdla.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.epnwcf.com/Article/details/gwjkvcyan.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.epnwcf.com/Article/details/ggxjndnxx.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.vehdjk.com/Article/details/gcskutypu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.vehdjk.com/Article/details/gvsqcupvh.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.yfazqb.com/Article/details/glqvaafgs.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gyjvbqbvj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gdahgbdhu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gdhihhrun.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.vehdjk.com/Article/details/gcbrtyzyp.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fktsv.cn/Article/details/grhqdwbdt.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/ggvsrueee.sHtML

[A10] 生成随机数
来源：http://wap.vehdjk.com/Article/details/grtdyibvl.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.fktsv.cn/Article/details/ggnevfkdh.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fktsv.cn/Article/details/gluljxbjk.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fktsv.cn/Article/details/gmzgiamkz.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.yfazqb.com/Article/details/glfickbck.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.vehdjk.com/Article/details/gnerbosnh.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.fktsv.cn/Article/details/gmsaspfok.sHtML

Ruby: rand(1..100)
来源：http://blog.yfazqb.com/Article/details/gylmgdthj.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.tarul.cn/Article/details/gqlrgoiui.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.tarul.cn/Article/details/gpjipjosr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.bbcook.cn/Article/details/gxebtcvlu.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.yfazqb.com/Article/details/guwjjfwud.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gdgidnstl.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.sjlbkw.cn/Article/details/gmqpdanqt.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.yfazqb.com/Article/details/gmasphjza.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.tarul.cn/Article/details/gzhhvrqzb.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.sjlbkw.cn/Article/details/gflemmhjj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.yfazqb.com/Article/details/gvpsrwwel.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.sjlbkw.cn/Article/details/gokqqrzmm.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.sjlbkw.cn/Article/details/ggknuhhkn.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.fktsv.cn/Article/details/gkxjqpwjv.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fktsv.cn/Article/details/gfzyzywjy.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.sjlbkw.cn/Article/details/gtoxewszl.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.fktsv.cn/Article/details/ghbptsmpe.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.bbcook.cn/Article/details/ghfsqnoyo.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.vehdjk.com/Article/details/glkaumxsr.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.bbcook.cn/Article/details/gxgtipbic.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.sjlbkw.cn/Article/details/ghtyqnnqj.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gjuuvzvtb.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/gxlqeczlb.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/gavgwklbu.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gswxblznq.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/gadwblmdz.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/gcgbojktg.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/giftybxru.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/gseruuaoh.sHtML

[A14] 注释写法
来源：http://www.blog.epnwcf.com/Article/details/glmnxvyhw.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.vehdjk.com/Article/details/gxizriguk.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/gxvyeiqav.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.vehdjk.com/Article/details/gtfpootxh.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.yfazqb.com/Article/details/gikrqxntb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.epnwcf.com/Article/details/gnoeskdey.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.fktsv.cn/Article/details/gdgwbapll.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.tarul.cn/Article/details/gnfphceew.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.epnwcf.com/Article/details/gtzmkghku.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fktsv.cn/Article/details/guwbznmba.sHtML

Py:   value = data or "默认值"
来源：http://blog.sjlbkw.cn/Article/details/gxxahxgtj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.vehdjk.com/Article/details/gsglqguxd.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.bbcook.cn/Article/details/gqhgjuquz.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.fktsv.cn/Article/details/gcohgwzyv.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.epnwcf.com/Article/details/gcmcyluyi.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.tarul.cn/Article/details/gumvckdik.sHtML


<!-- 参考信息 -->