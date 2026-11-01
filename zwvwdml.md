代发 wailian999

[U93] JS：模板字符串
来源：http://wap.vehdjk.com/Article/details/gnavmdlzo.sHtML

`共 ${n} 条`
来源：http://wap.fktsv.cn/Article/details/gfipythyb.sHtML

[U94] JS：箭头函数
来源：http://3g.sjlbkw.cn/Article/details/gwvhwplig.sHtML

const double = x => x * 2;
来源：http://wap.fktsv.cn/Article/details/gmfwagxxd.sHtML

[U95] JS：Promise 包装
来源：http://blog.yfazqb.com/Article/details/gljilmzdg.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.vehdjk.com/Article/details/gnlcpolyg.sHtML

[U96] JS：async/await 与异常
来源：http://baike.yfazqb.com/Article/details/gwinadrqo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/gnwvyymrz.sHtML

[U97] JS：并发请求
来源：http://m.share.bbcook.cn/Article/details/gmqlskfrw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gnxvfqmvd.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.epnwcf.com/Article/details/glrwgkloj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fktsv.cn/Article/details/guonbbecq.sHtML

[U99] JS：事件监听
来源：http://mobile.sjlbkw.cn/Article/details/gaonjmizx.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.yfazqb.com/Article/details/glcjlbwpq.sHtML

[U100] JS：DOM 查询
来源：http://www.share.tarul.cn/Article/details/ghpkhyrtk.sHtML

document.querySelector(".item")
来源：http://read.share.sjlbkw.cn/Article/details/gpyolhgbr.sHtML

[U101] JS：classList 操作
来源：http://mobile.epnwcf.com/Article/details/gbbcvsrsc.sHtML

el.classList.toggle("active")
来源：http://www.share.epnwcf.com/Article/details/gvvfezevv.sHtML

[U102] JS：本地存储
来源：http://blog.vehdjk.com/Article/details/gqzcbcgpc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.tarul.cn/Article/details/gvwzknfiw.sHtML

[U103] JS：定时器
来源：http://mobile.bbcook.cn/Article/details/gavqvuqok.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.tarul.cn/Article/details/gqkzslkfa.sHtML

[U104] JS：防抖
来源：http://wap.yfazqb.com/Article/details/gemgyqxem.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/ghblsehnp.sHtML

[U105] JS：节流
来源：http://wap.fktsv.cn/Article/details/gbjtkrejy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.tarul.cn/Article/details/ggxzriiyb.sHtML

[U106] JS：日期格式化
来源：http://mobile.vehdjk.com/Article/details/golljuppr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fktsv.cn/Article/details/gptehsnbw.sHtML

[U107] JS：数字千分位
来源：http://wap.fktsv.cn/Article/details/gnidxfldu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.yfazqb.com/Article/details/gkfpasjgq.sHtML

[U108] JS：随机整数
来源：http://www.m.share.epnwcf.com/Article/details/gfxlzmapo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.vehdjk.com/Article/details/gkaiezhhc.sHtML

[U109] JS：数组分组
来源：http://read.share.vehdjk.com/Article/details/gafyeafjx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.epnwcf.com/Article/details/gtnsuphoj.sHtML

[U110] JS：数组分块
来源：http://mobile.tarul.cn/Article/details/gbtgswbch.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.epnwcf.com/Article/details/glragazff.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.epnwcf.com/Article/details/gsamyxwhu.sHtML

new Map(Object.entries(obj))
来源：http://baike.yfazqb.com/Article/details/gzmrunnox.sHtML

[U112] JS：字符串补位
来源：http://3g.sjlbkw.cn/Article/details/gaafvgtpm.sHtML

"7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gerhtsosr.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.sjlbkw.cn/Article/details/ggmsoudwi.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gqkwrapgi.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.sjlbkw.cn/Article/details/gcobgvnoo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/grvfhtjpi.sHtML

[U115] JS：生成 UUID
来源：http://baike.fktsv.cn/Article/details/gvnwcvabi.sHtML

crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/griplffvj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.tarul.cn/Article/details/guuqqwamv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.vehdjk.com/Article/details/gdzkxygpm.sHtML

[U117] JS：单元测试
来源：http://3g.sjlbkw.cn/Article/details/gzucaojre.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.sjlbkw.cn/Article/details/gbifyjsbi.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fktsv.cn/Article/details/guwxzlltv.sHtML

npm i -D vite;  npx vite
来源：http://blog.epnwcf.com/Article/details/gmrtbdboo.sHtML

[U119] JS：生产构建
来源：http://www.blog.epnwcf.com/Article/details/ghdqnpsjm.sHtML

npx vite build
来源：http://blog.yfazqb.com/Article/details/gxsehpeac.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.sjlbkw.cn/Article/details/gsbeqppbe.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.tarul.cn/Article/details/gqwafzrrr.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gschvnhau.sHtML

统计汇总
来源：http://blog.tarul.cn/Article/details/glphgqzwr.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gfbbpouce.sHtML

按语言统计（条）：
来源：http://read.share.fktsv.cn/Article/details/gomlrdgbq.sHtML

Python ......... 252
来源：http://wap.epnwcf.com/Article/details/gyiluevii.sHtML

PHP ............ 252
来源：http://3g.tarul.cn/Article/details/gxlikqowd.sHtML

JavaScript ..... 252
来源：http://baike.fktsv.cn/Article/details/gwtvshhbp.sHtML

TypeScript ..... 212
来源：http://www.m.share.bbcook.cn/Article/details/gzojfixuk.sHtML

Java ........... 212
来源：http://blog.epnwcf.com/Article/details/gnjbtbjrp.sHtML

Go ............. 212
来源：http://blog.epnwcf.com/Article/details/gcbufjatl.sHtML

Ruby ........... 212
来源：http://www.blog.vehdjk.com/Article/details/gwcsyhsph.sHtML

C# ............. 212
来源：http://baike.sjlbkw.cn/Article/details/gpnuyepex.sHtML

C .............. 30
来源：http://www.blog.epnwcf.com/Article/details/gqwtolllh.sHtML

C++ ............ 30
来源：http://read.share.epnwcf.com/Article/details/gntmzptad.sHtML

SQL ............ 90
来源：http://blog.yfazqb.com/Article/details/gnrjkngfk.sHtML

Bash ........... 80
来源：http://mobile.bbcook.cn/Article/details/gbptxngqo.sHtML

Kotlin ......... 15
来源：http://read.share.vehdjk.com/Article/details/gcelzwair.sHtML

Swift .......... 15
来源：http://blog.tarul.cn/Article/details/garrbvegh.sHtML

Lua ............ 10
来源：http://blog.vehdjk.com/Article/details/gbhmbllem.sHtML

Perl ........... 10
来源：http://baike.yfazqb.com/Article/details/gzewqseyz.sHtML

Scala .......... 10
来源：http://read.share.sjlbkw.cn/Article/details/gqcaufgeq.sHtML

------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/gwpbtfdge.sHtML

合计 ........... 2106 条
来源：http://read.share.tarul.cn/Article/details/gwkhckszo.sHtML

按章节统计：
来源：http://www.share.vehdjk.com/Article/details/gxwpmrlbr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.sjlbkw.cn/Article/details/gecrcheac.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.bbcook.cn/Article/details/gqdryivad.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fktsv.cn/Article/details/gvxbacltm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.vehdjk.com/Article/details/glltcppbo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.vehdjk.com/Article/details/gxzxiqtcr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.yfazqb.com/Article/details/grsdtsten.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.sjlbkw.cn/Article/details/gcmlzkqld.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.bbcook.cn/Article/details/gsdrtdhpr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gecgyzwfh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.yfazqb.com/Article/details/gdxhngqzr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gvgfggjre.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gtrlmrxve.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/gddkzaxdd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.tarul.cn/Article/details/gwmipqnmd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.yfazqb.com/Article/details/gtuierroy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gsfwyiday.sHtML

Q SQL 专题                              90
来源：http://m.share.epnwcf.com/Article/details/gxpgkktcv.sHtML

R Bash 专题                             80
来源：http://m.share.bbcook.cn/Article/details/gnfbojiag.sHtML

S C / C++ 专题                          60
来源：http://wap.yfazqb.com/Article/details/gxipoipej.sHtML

T 其他语言补充                          60
来源：http://blog.vehdjk.com/Article/details/gurwjosui.sHtML

U 高频实用片段                         120
来源：http://wap.yfazqb.com/Article/details/gcrwtslpk.sHtML

------------------------------------
来源：http://wap.yfazqb.com/Article/details/gvsbzuurc.sHtML

合计                                  2106 条
来源：http://baike.yfazqb.com/Article/details/gnpkhsyns.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gfdsnkxhe.sHtML

使用提醒
来源：http://mobile.yfazqb.com/Article/details/glgopkktn.sHtML

--------------------------------------------------------------------------------
来源：http://blog.bbcook.cn/Article/details/gejcssrpw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.vehdjk.com/Article/details/gezopjgiv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.yfazqb.com/Article/details/gxguwceuo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.tarul.cn/Article/details/gqhkhumhh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.bbcook.cn/Article/details/gvtuxmqhl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.sjlbkw.cn/Article/details/gyhdhocfl.sHtML

—— 文件结束 ——
来源：http://blog.epnwcf.com/Article/details/gceaouvwc.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gzwgoiifs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.bbcook.cn/Article/details/gspwpmzsq.sHtML

Common Programming Examples Cheat Book
来源：http://wap.tarul.cn/Article/details/gcyiemdoq.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gztjusmou.sHtML

【收录内容】
来源：http://mobile.yfazqb.com/Article/details/gcnokdgvq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fktsv.cn/Article/details/gbprchzbi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.epnwcf.com/Article/details/gshcbowdy.sHtML

SQL · Bash · C · C++
来源：http://wap.bbcook.cn/Article/details/gmjytuqvo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.bbcook.cn/Article/details/gbmkqzqfe.sHtML

【使用说明】
来源：http://read.share.epnwcf.com/Article/details/gafdoazsr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.epnwcf.com/Article/details/gyobxgtsx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fktsv.cn/Article/details/gkkadycue.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.bbcook.cn/Article/details/gmtshclzw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.epnwcf.com/Article/details/ghsfbjxge.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fktsv.cn/Article/details/gefwzeqqq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fktsv.cn/Article/details/guilqftuy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.tarul.cn/Article/details/guywjxxcy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.vehdjk.com/Article/details/gsljyeqin.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.bbcook.cn/Article/details/gokslkvnz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.tarul.cn/Article/details/gthyvhllm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.tarul.cn/Article/details/gxwiwranf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.yfazqb.com/Article/details/gbmkitwwy.sHtML

【文件统计】
来源：http://3g.yfazqb.com/Article/details/gpulievhx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.vehdjk.com/Article/details/gzuuzzkjt.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gpihvwhsw.sHtML

目  录
来源：http://www.m.share.yfazqb.com/Article/details/geopfqvej.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.tarul.cn/Article/details/gjoewwask.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fktsv.cn/Article/details/gtrprpmup.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/glonqbgcz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fktsv.cn/Article/details/ggoqqapqn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fktsv.cn/Article/details/gbdeuxwja.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.epnwcf.com/Article/details/gcesiqxoy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.sjlbkw.cn/Article/details/gcqxkchnr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.vehdjk.com/Article/details/gdcuwpgvo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.yfazqb.com/Article/details/gbfvsdzrr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/gqmhezvnb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.vehdjk.com/Article/details/gbmycodgn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/gymglbgzj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.epnwcf.com/Article/details/gnlvyypor.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrcsyviq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fktsv.cn/Article/details/gdjmmxteu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.bbcook.cn/Article/details/ggeieoxhx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.vehdjk.com/Article/details/gsytkpykd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.vehdjk.com/Article/details/gcvaverik.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.tarul.cn/Article/details/guzpmpbsl.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.yfazqb.com/Article/details/gldukwkwp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.tarul.cn/Article/details/gppgzbhvl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.vehdjk.com/Article/details/gcxewethm.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/grfcvtvvr.sHtML

A. 基础语法与类型
来源：http://baike.vehdjk.com/Article/details/gjwsdeltg.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gxqkwdhrp.sHtML

[A01] Hello World
来源：http://wap.epnwcf.com/Article/details/gbacylume.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fktsv.cn/Article/details/gnncivcvr.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fktsv.cn/Article/details/gbvjnbjhv.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fktsv.cn/Article/details/gkuvbsrjf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.yfazqb.com/Article/details/gufpbzrhh.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.vehdjk.com/Article/details/ghcqgjpgb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.yfazqb.com/Article/details/gpwctuttj.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.bbcook.cn/Article/details/gacayyfxd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.bbcook.cn/Article/details/grusikvkk.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fktsv.cn/Article/details/gizdtwdup.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.yfazqb.com/Article/details/gjopagguo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.tarul.cn/Article/details/gxtsirykf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fktsv.cn/Article/details/ghgibrikt.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.epnwcf.com/Article/details/gwfoivldf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/giteqjkin.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.tarul.cn/Article/details/ggjojqxgs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fktsv.cn/Article/details/gwigdcamj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.yfazqb.com/Article/details/ggkcqezlx.sHtML

[A03] 常量定义
来源：http://blog.bbcook.cn/Article/details/gjugvltgz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fktsv.cn/Article/details/gjprhpbwh.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/ghfduazjy.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gtabccrbx.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.tarul.cn/Article/details/gvneqworv.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/grakroctk.sHtML

Go:   const PI = 3.14159
来源：http://m.share.bbcook.cn/Article/details/gkbahzjmc.sHtML

Ruby: PI = 3.14159
来源：http://mobile.epnwcf.com/Article/details/gtozpbcrn.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/guuzewnaw.sHtML

[A04] 判断变量类型
来源：http://www.blog.tarul.cn/Article/details/gwgkfzldz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fktsv.cn/Article/details/giocjftpw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.yfazqb.com/Article/details/gwuegezxq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.vehdjk.com/Article/details/gvrsikxoa.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fktsv.cn/Article/details/gxqnuwwtn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fktsv.cn/Article/details/gcrmgxrwl.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.tarul.cn/Article/details/gqkugcmcs.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fktsv.cn/Article/details/gndvujkao.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.vehdjk.com/Article/details/gkkjjkrvk.sHtML

[A05] 整数除法与取模
来源：http://wap.fktsv.cn/Article/details/gwbucvobi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.yfazqb.com/Article/details/gqmemdryv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gqjrvlacv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/gxzgkwncz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.tarul.cn/Article/details/gtkngyefy.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/gqvenbyxi.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.vehdjk.com/Article/details/gksmggoiv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.epnwcf.com/Article/details/grjpgfyph.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gqcikyxpd.sHtML

[A06] 字符串转数字
来源：http://3g.fktsv.cn/Article/details/giiqvzbcx.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.sjlbkw.cn/Article/details/giwdkotyx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.tarul.cn/Article/details/gdhgumpmx.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.epnwcf.com/Article/details/gkqzfashc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.bbcook.cn/Article/details/gwzdltdts.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fktsv.cn/Article/details/gsrhhwger.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.yfazqb.com/Article/details/gqijredqc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.bbcook.cn/Article/details/gryaagvao.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.vehdjk.com/Article/details/gkbxbzylg.sHtML

[A07] 数字转字符串
来源：http://3g.bbcook.cn/Article/details/gdwebhwrl.sHtML

Py:   str(42)
来源：http://www.m.share.vehdjk.com/Article/details/gkykhlxio.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fktsv.cn/Article/details/gzuibunbe.sHtML

JS:   String(42); (42).toString()
来源：http://blog.epnwcf.com/Article/details/gjgzajnpj.sHtML

TS:   String(42)
来源：http://m.share.yfazqb.com/Article/details/gfoiqlozx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.sjlbkw.cn/Article/details/giinjugho.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.bbcook.cn/Article/details/gdmmtfqkv.sHtML

Ruby: 42.to_s
来源：http://baike.fktsv.cn/Article/details/gebvngnko.sHtML

C#:   42.ToString()
来源：http://read.share.sjlbkw.cn/Article/details/gophhwfwa.sHtML

[A08] 取整与四舍五入
来源：http://read.share.yfazqb.com/Article/details/gtrtrgwdl.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.epnwcf.com/Article/details/grkzpcroe.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fktsv.cn/Article/details/gpdghfcrs.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.tarul.cn/Article/details/gslharxba.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.yfazqb.com/Article/details/gdnshumrp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.vehdjk.com/Article/details/gtpqjoagk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.vehdjk.com/Article/details/gaudcllns.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.sjlbkw.cn/Article/details/gzswdlzlj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.bbcook.cn/Article/details/gmftlfass.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fktsv.cn/Article/details/glsphgifb.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fktsv.cn/Article/details/gmfjwqoow.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.tarul.cn/Article/details/grmgxnoru.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.vehdjk.com/Article/details/gragtmlgy.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.yfazqb.com/Article/details/gzpjxerpj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gyllscngu.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.bbcook.cn/Article/details/gxrltxeqt.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.epnwcf.com/Article/details/gzqxpsyqy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.epnwcf.com/Article/details/goikkbkgt.sHtML

[A10] 生成随机数
来源：http://read.share.fktsv.cn/Article/details/gtermsylm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.tarul.cn/Article/details/gnbvecgbo.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fktsv.cn/Article/details/gnrqdzari.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fktsv.cn/Article/details/gnktrcufk.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.vehdjk.com/Article/details/gqvujvvos.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.epnwcf.com/Article/details/gslvhjyzu.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.tarul.cn/Article/details/glvkejydg.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.bbcook.cn/Article/details/gomshbhkv.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.vehdjk.com/Article/details/gbwgwwbgw.sHtML

[A11] 条件表达式（三元）
来源：http://blog.vehdjk.com/Article/details/gvocdhaif.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.yfazqb.com/Article/details/gxnxzndql.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.vehdjk.com/Article/details/gesgahutm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.epnwcf.com/Article/details/gcirqthfh.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.sjlbkw.cn/Article/details/gnmfdnbic.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.bbcook.cn/Article/details/gcqqvvalr.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.vehdjk.com/Article/details/gatefbbro.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.epnwcf.com/Article/details/gsuvfmvlb.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.vehdjk.com/Article/details/ghqcminbl.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.yfazqb.com/Article/details/gfmztgauf.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.epnwcf.com/Article/details/gpviiwslc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.yfazqb.com/Article/details/gydotlfuc.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.sjlbkw.cn/Article/details/gcpbgtvcu.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.tarul.cn/Article/details/gnajcxpex.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.bbcook.cn/Article/details/grwynyfba.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.epnwcf.com/Article/details/gwvqvwgxo.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.yfazqb.com/Article/details/gxydsuntq.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.epnwcf.com/Article/details/gvdqxcyhi.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.vehdjk.com/Article/details/gqcaxevyu.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/gqtaqynpy.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/gtoqtbuyd.sHtML

JS:   "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/golegdhri.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/gxoakvzqk.sHtML

Java: "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gpvqocrnk.sHtML

Go:   "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gjgjwwemn.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gnqcamiji.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/gwxtnzdcr.sHtML

[A14] 注释写法
来源：http://mobile.fktsv.cn/Article/details/gfumujiwc.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.fktsv.cn/Article/details/gpwlfsjpm.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.vehdjk.com/Article/details/gyivvfrrt.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.epnwcf.com/Article/details/gkxapohus.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.sjlbkw.cn/Article/details/gqypsrzjc.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.bbcook.cn/Article/details/gpklizjre.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.bbcook.cn/Article/details/grhpnalhm.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.fktsv.cn/Article/details/gqmwtouej.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.fktsv.cn/Article/details/goepydpax.sHtML

[A15] 空值判断与默认值
来源：http://wap.epnwcf.com/Article/details/gpgsbpflw.sHtML

Py:   value = data or "默认值"
来源：http://www.share.bbcook.cn/Article/details/gwwnqwxjb.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.sjlbkw.cn/Article/details/gbikkrmdt.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.epnwcf.com/Article/details/grnzujmbz.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.bbcook.cn/Article/details/giowhcrvp.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.vehdjk.com/Article/details/gcczxlkfi.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.yfazqb.com/Article/details/ghtrradte.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.vehdjk.com/Article/details/ghcidnxgr.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fktsv.cn/Article/details/gqofzlhxa.sHtML

[A16] 真假值判断规则
来源：http://wap.fktsv.cn/Article/details/ggdydwyzd.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.yfazqb.com/Article/details/gqopubsmo.sHtML


<!-- 参考信息 -->