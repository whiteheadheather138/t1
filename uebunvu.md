代发 wailian999

[U95] JS：Promise 包装
来源：http://blog.bbcook.cn/Article/details/geofmofsx.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.yfazqb.com/Article/details/gsokatlhz.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.bbcook.cn/Article/details/gnepqmonz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/glrhifhki.sHtML

[U97] JS：并发请求
来源：http://wap.epnwcf.com/Article/details/gttolbxdl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gfpssvjep.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fktsv.cn/Article/details/gayusnrut.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fktsv.cn/Article/details/gxemhlodt.sHtML

[U99] JS：事件监听
来源：http://read.share.sjlbkw.cn/Article/details/gyccxlwuz.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.bbcook.cn/Article/details/gytyomejm.sHtML

[U100] JS：DOM 查询
来源：http://baike.yfazqb.com/Article/details/gscnzahxn.sHtML

document.querySelector(".item")
来源：http://m.share.fktsv.cn/Article/details/guxjfiiqx.sHtML

[U101] JS：classList 操作
来源：http://read.share.vehdjk.com/Article/details/gnibyqicy.sHtML

el.classList.toggle("active")
来源：http://mobile.yfazqb.com/Article/details/grrjsmuoy.sHtML

[U102] JS：本地存储
来源：http://baike.epnwcf.com/Article/details/giklhbylc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.vehdjk.com/Article/details/gtheebwde.sHtML

[U103] JS：定时器
来源：http://m.share.fktsv.cn/Article/details/gljhuxpvx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.epnwcf.com/Article/details/ggsagyzsx.sHtML

[U104] JS：防抖
来源：http://www.share.tarul.cn/Article/details/gswomdhur.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gdcgfwjma.sHtML

[U105] JS：节流
来源：http://read.share.yfazqb.com/Article/details/gcmxgbhhw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.sjlbkw.cn/Article/details/gcorjhjpa.sHtML

[U106] JS：日期格式化
来源：http://baike.epnwcf.com/Article/details/gwkpthuiw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.sjlbkw.cn/Article/details/gwklsiykd.sHtML

[U107] JS：数字千分位
来源：http://3g.fktsv.cn/Article/details/gzgouysfr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.sjlbkw.cn/Article/details/grstocmhn.sHtML

[U108] JS：随机整数
来源：http://mobile.fktsv.cn/Article/details/gdvxfliyy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.tarul.cn/Article/details/gpnwtoslo.sHtML

[U109] JS：数组分组
来源：http://www.share.yfazqb.com/Article/details/gmgxpxmvd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.sjlbkw.cn/Article/details/gsdbclhrp.sHtML

[U110] JS：数组分块
来源：http://read.share.epnwcf.com/Article/details/guanxwrqy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.tarul.cn/Article/details/gtyyhgdzk.sHtML

[U111] JS：对象转 Map
来源：http://wap.sjlbkw.cn/Article/details/gkjxdmxnn.sHtML

new Map(Object.entries(obj))
来源：http://blog.tarul.cn/Article/details/gfxbwuhfv.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.yfazqb.com/Article/details/grdmjcmci.sHtML

"7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/grivknfqf.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.tarul.cn/Article/details/gxuoyqsgp.sHtML

s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gqjgrkbeg.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.epnwcf.com/Article/details/ghjsvxnty.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gabfrqejk.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fktsv.cn/Article/details/gobatqgef.sHtML

crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/gelecwwwx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.sjlbkw.cn/Article/details/gpoacpagu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.bbcook.cn/Article/details/gjyijvsic.sHtML

[U117] JS：单元测试
来源：http://wap.sjlbkw.cn/Article/details/gerksfevx.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.vehdjk.com/Article/details/glmrygzig.sHtML

[U118] JS：开发服务器
来源：http://wap.tarul.cn/Article/details/gwihqkomb.sHtML

npm i -D vite;  npx vite
来源：http://www.share.bbcook.cn/Article/details/gclarioal.sHtML

[U119] JS：生产构建
来源：http://www.blog.yfazqb.com/Article/details/gzbuhzkyb.sHtML

npx vite build
来源：http://baike.tarul.cn/Article/details/grkwxodwn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.epnwcf.com/Article/details/gcorpphey.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.sjlbkw.cn/Article/details/gyujfuduw.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gvleuipxr.sHtML

统计汇总
来源：http://baike.fktsv.cn/Article/details/gjfcsojup.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gngfabxom.sHtML

按语言统计（条）：
来源：http://read.share.sjlbkw.cn/Article/details/gewdmknmy.sHtML

Python ......... 252
来源：http://read.share.vehdjk.com/Article/details/guwjvfkll.sHtML

PHP ............ 252
来源：http://www.m.share.tarul.cn/Article/details/ggirtmlge.sHtML

JavaScript ..... 252
来源：http://blog.sjlbkw.cn/Article/details/gwsdowrvq.sHtML

TypeScript ..... 212
来源：http://blog.bbcook.cn/Article/details/gmdtevrut.sHtML

Java ........... 212
来源：http://baike.bbcook.cn/Article/details/gaatwicfv.sHtML

Go ............. 212
来源：http://mobile.vehdjk.com/Article/details/gfbxzmvzk.sHtML

Ruby ........... 212
来源：http://baike.sjlbkw.cn/Article/details/gzqzkmhth.sHtML

C# ............. 212
来源：http://mobile.fktsv.cn/Article/details/gpoohyaxw.sHtML

C .............. 30
来源：http://m.share.vehdjk.com/Article/details/geyfjtjsk.sHtML

C++ ............ 30
来源：http://www.m.share.bbcook.cn/Article/details/gxrxqsofo.sHtML

SQL ............ 90
来源：http://www.blog.sjlbkw.cn/Article/details/gcppluqzi.sHtML

Bash ........... 80
来源：http://mobile.fktsv.cn/Article/details/gvtdicmpx.sHtML

Kotlin ......... 15
来源：http://wap.epnwcf.com/Article/details/gtptkxyss.sHtML

Swift .......... 15
来源：http://m.share.bbcook.cn/Article/details/goubrjgey.sHtML

Lua ............ 10
来源：http://mobile.yfazqb.com/Article/details/gulyjkfpw.sHtML

Perl ........... 10
来源：http://www.share.yfazqb.com/Article/details/gggqoxvsl.sHtML

Scala .......... 10
来源：http://baike.yfazqb.com/Article/details/gpezifpdq.sHtML

------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/gzotslgdc.sHtML

合计 ........... 2106 条
来源：http://www.blog.epnwcf.com/Article/details/ggnccayyu.sHtML

按章节统计：
来源：http://3g.fktsv.cn/Article/details/grsxxkxlp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.epnwcf.com/Article/details/gqqruzkwa.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/gbpmgiedp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.bbcook.cn/Article/details/gxzsfakjw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.tarul.cn/Article/details/grzflkpvs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.tarul.cn/Article/details/gnqufqvts.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.epnwcf.com/Article/details/gotgjdixe.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.tarul.cn/Article/details/gqaxzebfy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.epnwcf.com/Article/details/gyurtwild.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.epnwcf.com/Article/details/gkrkguoww.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.sjlbkw.cn/Article/details/gufkhpufw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fktsv.cn/Article/details/gzguywumg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/gmtxdbidk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fktsv.cn/Article/details/ggswqjpjt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fktsv.cn/Article/details/gohpipeol.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.yfazqb.com/Article/details/gkomekmne.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gjuirzlut.sHtML

Q SQL 专题                              90
来源：http://baike.bbcook.cn/Article/details/gozozfddf.sHtML

R Bash 专题                             80
来源：http://www.share.fktsv.cn/Article/details/gflofgeje.sHtML

S C / C++ 专题                          60
来源：http://wap.epnwcf.com/Article/details/gwlogdpnv.sHtML

T 其他语言补充                          60
来源：http://www.share.bbcook.cn/Article/details/gozblcuzj.sHtML

U 高频实用片段                         120
来源：http://www.share.bbcook.cn/Article/details/gvtrksfic.sHtML

------------------------------------
来源：http://baike.bbcook.cn/Article/details/gzmhlqnya.sHtML

合计                                  2106 条
来源：http://www.m.share.vehdjk.com/Article/details/ghljecrar.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.tarul.cn/Article/details/gspddjjct.sHtML

使用提醒
来源：http://www.blog.vehdjk.com/Article/details/gfjbfznuy.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gdamdqubs.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fktsv.cn/Article/details/gwtyhqxdv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.yfazqb.com/Article/details/gukxkwnsl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.vehdjk.com/Article/details/gfqygsnhj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.vehdjk.com/Article/details/gunvkuchf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.vehdjk.com/Article/details/gfhoavqey.sHtML

—— 文件结束 ——
来源：http://wap.bbcook.cn/Article/details/gyioeiegy.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gmxnjzugu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.vehdjk.com/Article/details/gbtlpeacr.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.vehdjk.com/Article/details/grsnmirkr.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gwzshdbge.sHtML

【收录内容】
来源：http://3g.tarul.cn/Article/details/gpmenpoom.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.tarul.cn/Article/details/gyhxbrrzi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.tarul.cn/Article/details/golkkpdgi.sHtML

SQL · Bash · C · C++
来源：http://blog.fktsv.cn/Article/details/gircarzcc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.bbcook.cn/Article/details/gyrubqizt.sHtML

【使用说明】
来源：http://blog.tarul.cn/Article/details/gwyzqeymp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.tarul.cn/Article/details/gljjepxbt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.sjlbkw.cn/Article/details/gxynxhyfm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.epnwcf.com/Article/details/gbioahiqq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.sjlbkw.cn/Article/details/gjfepfzgy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.sjlbkw.cn/Article/details/gylsayglj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.bbcook.cn/Article/details/gqkcinvaz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.bbcook.cn/Article/details/gaednvzpb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.yfazqb.com/Article/details/gtnwppskp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.bbcook.cn/Article/details/gsxhrjvqo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.sjlbkw.cn/Article/details/gmnyvuebc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.tarul.cn/Article/details/gffohymgb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.epnwcf.com/Article/details/gbfqjepmt.sHtML

【文件统计】
来源：http://m.share.vehdjk.com/Article/details/gfxzwfopu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.tarul.cn/Article/details/gxmuosesk.sHtML

--------------------------------------------------------------------------------
来源：http://3g.bbcook.cn/Article/details/gwajkoyxu.sHtML

目  录
来源：http://wap.tarul.cn/Article/details/ggoukgeea.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gashzyoqx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.vehdjk.com/Article/details/gayhzutad.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.yfazqb.com/Article/details/gkauawccp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.bbcook.cn/Article/details/glxirmbys.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.tarul.cn/Article/details/gpndxkepm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.bbcook.cn/Article/details/gqczldmtw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.sjlbkw.cn/Article/details/gnfjaogfq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.epnwcf.com/Article/details/goqrcrrsj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.yfazqb.com/Article/details/gygxyqxvq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/gqlzlvkbz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.vehdjk.com/Article/details/gajohmhud.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.tarul.cn/Article/details/gzoelqrwh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/gsdxjhozw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.bbcook.cn/Article/details/gniqnmuuh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.bbcook.cn/Article/details/ginchulsj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fktsv.cn/Article/details/gffqmaqmz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.bbcook.cn/Article/details/gjhngyncw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.yfazqb.com/Article/details/gjkjpseux.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.epnwcf.com/Article/details/gcdccsrim.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfoboexh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.yfazqb.com/Article/details/gfrmvwwel.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.bbcook.cn/Article/details/gkmcjglkd.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gcllwjhvk.sHtML

A. 基础语法与类型
来源：http://www.blog.sjlbkw.cn/Article/details/gtvgipuja.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gzwozqtfi.sHtML

[A01] Hello World
来源：http://baike.vehdjk.com/Article/details/gfmjucagq.sHtML

Py:   print("Hello, World!")
来源：http://mobile.tarul.cn/Article/details/glsaxecvk.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.sjlbkw.cn/Article/details/glkybqixh.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.yfazqb.com/Article/details/gohunleql.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.bbcook.cn/Article/details/goesszrva.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.sjlbkw.cn/Article/details/glfqzolta.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.bbcook.cn/Article/details/gqqypcctt.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.vehdjk.com/Article/details/gluidefek.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.epnwcf.com/Article/details/ggobtjpss.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.epnwcf.com/Article/details/gutqtclsn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.sjlbkw.cn/Article/details/gxvqyiivt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.epnwcf.com/Article/details/glhcleurx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.bbcook.cn/Article/details/ghuzzvdas.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.sjlbkw.cn/Article/details/gdncdjqcg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.bbcook.cn/Article/details/gxwjxqfyn.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.epnwcf.com/Article/details/gfczsnssz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.sjlbkw.cn/Article/details/gpjawyfwn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.vehdjk.com/Article/details/gfanhgnxs.sHtML

[A03] 常量定义
来源：http://www.m.share.epnwcf.com/Article/details/gaoqmrbkd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fktsv.cn/Article/details/gudqkhzts.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gwvwtcfgy.sHtML

JS:   const PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gzuyscgvz.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gxdxujyvu.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gmqlqnrwb.sHtML

Go:   const PI = 3.14159
来源：http://blog.epnwcf.com/Article/details/geqfvvfnp.sHtML

Ruby: PI = 3.14159
来源：http://baike.bbcook.cn/Article/details/gcxyefbhf.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/grlwxxsmf.sHtML

[A04] 判断变量类型
来源：http://3g.vehdjk.com/Article/details/gpycdwmed.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fktsv.cn/Article/details/gnjjceerg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.epnwcf.com/Article/details/gaktmtmnp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.sjlbkw.cn/Article/details/gmjuufufe.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.vehdjk.com/Article/details/gkpvfxefr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.epnwcf.com/Article/details/gvpygxbje.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.yfazqb.com/Article/details/grbbbvpjd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.vehdjk.com/Article/details/gcedfzrld.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.vehdjk.com/Article/details/gczoazxol.sHtML

[A05] 整数除法与取模
来源：http://baike.fktsv.cn/Article/details/gnytxndoj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fktsv.cn/Article/details/gkqhyukyd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.yfazqb.com/Article/details/gyaocwapf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gyacotgxv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gznrqmiwk.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/gfimbuksp.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gbzhvfctn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.vehdjk.com/Article/details/glbvqmdhl.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.bbcook.cn/Article/details/gpkpxpllv.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fktsv.cn/Article/details/gldzdsokl.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.bbcook.cn/Article/details/gtsnusakg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.vehdjk.com/Article/details/ggopaxrcf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fktsv.cn/Article/details/gfklyaebf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.sjlbkw.cn/Article/details/gwputzabb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.vehdjk.com/Article/details/gxhigbens.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.tarul.cn/Article/details/grmrcvkxm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fktsv.cn/Article/details/gorzjrtya.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.bbcook.cn/Article/details/giimzofui.sHtML

[A07] 数字转字符串
来源：http://www.share.yfazqb.com/Article/details/gvvsmlpsp.sHtML

Py:   str(42)
来源：http://mobile.epnwcf.com/Article/details/gzunnafle.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.vehdjk.com/Article/details/gqqdhagpq.sHtML

JS:   String(42); (42).toString()
来源：http://3g.tarul.cn/Article/details/gcocxsfcm.sHtML

TS:   String(42)
来源：http://www.m.share.yfazqb.com/Article/details/gbouxnupu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.yfazqb.com/Article/details/gflngdoul.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.vehdjk.com/Article/details/gxwtyqald.sHtML

Ruby: 42.to_s
来源：http://www.share.tarul.cn/Article/details/giigmnkao.sHtML

C#:   42.ToString()
来源：http://www.blog.sjlbkw.cn/Article/details/gsnnusjvz.sHtML

[A08] 取整与四舍五入
来源：http://blog.tarul.cn/Article/details/gadsjtkja.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.yfazqb.com/Article/details/gdpapkbxt.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.yfazqb.com/Article/details/ghgsjcdfs.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.tarul.cn/Article/details/gygnasxsc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.tarul.cn/Article/details/gihbgdybz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.vehdjk.com/Article/details/gzdzmjafr.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.vehdjk.com/Article/details/glpufewtn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.epnwcf.com/Article/details/ggzrwmmsv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.vehdjk.com/Article/details/gsnnztyyw.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gniqprnfo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.vehdjk.com/Article/details/gsuxfsxrd.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/gtmslzwqw.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.vehdjk.com/Article/details/gvyhqwdzi.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gwhazultg.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.epnwcf.com/Article/details/grpootqea.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.fktsv.cn/Article/details/grztfzgou.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.sjlbkw.cn/Article/details/gqxhfrepq.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.vehdjk.com/Article/details/gzfzdwkrt.sHtML

[A10] 生成随机数
来源：http://m.share.sjlbkw.cn/Article/details/giphdvkyp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.vehdjk.com/Article/details/giwruxmew.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.vehdjk.com/Article/details/gdyhbhrdn.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.bbcook.cn/Article/details/gbrfmbqvv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.epnwcf.com/Article/details/gyuuxbrlv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.fktsv.cn/Article/details/gozjvudob.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.fktsv.cn/Article/details/gpzzkxgrf.sHtML

Ruby: rand(1..100)
来源：http://read.share.fktsv.cn/Article/details/gntiymxph.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.tarul.cn/Article/details/geabbvmkg.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.yfazqb.com/Article/details/gckmpqthk.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.vehdjk.com/Article/details/ggotlozbu.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.bbcook.cn/Article/details/ggukhovmd.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.epnwcf.com/Article/details/gohfcsxvv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.yfazqb.com/Article/details/gwdbuuplx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.epnwcf.com/Article/details/gxawdpxnn.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.sjlbkw.cn/Article/details/gyjcuevnp.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.fktsv.cn/Article/details/gkfsfbnhi.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gmqmgybzf.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.epnwcf.com/Article/details/gknjzviff.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.tarul.cn/Article/details/gnsdavegn.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.tarul.cn/Article/details/gyhlmiood.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.yfazqb.com/Article/details/gyauugsgp.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.yfazqb.com/Article/details/gjrfiryrq.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.yfazqb.com/Article/details/guntumigq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gszteqspg.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.vehdjk.com/Article/details/gckgouvaj.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.epnwcf.com/Article/details/gpbtaytrm.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.tarul.cn/Article/details/gynlmplrn.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.tarul.cn/Article/details/ghzemoeuw.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/guxdjqqwt.sHtML

JS:   "第一行\n第二行"
来源：http://baike.tarul.cn/Article/details/gxvjamtwn.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gpdnkkcxf.sHtML

Java: "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/guepfzyno.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.fktsv.cn/Article/details/ghvntqoyk.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gunaxlkqu.sHtML

C#:   "第一行\n第二行"
来源：http://baike.yfazqb.com/Article/details/gyvutksbu.sHtML

[A14] 注释写法
来源：http://mobile.tarul.cn/Article/details/gbufrkutb.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.vehdjk.com/Article/details/gbzntxjaq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.yfazqb.com/Article/details/gyptilcuq.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.bbcook.cn/Article/details/gchzacndg.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.sjlbkw.cn/Article/details/gpazllcsw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.epnwcf.com/Article/details/gqvvzyscv.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.vehdjk.com/Article/details/geyrlpowd.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.vehdjk.com/Article/details/gpburxevp.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.sjlbkw.cn/Article/details/gdkzmeffv.sHtML

[A15] 空值判断与默认值
来源：http://m.share.tarul.cn/Article/details/gjylukvnj.sHtML

Py:   value = data or "默认值"
来源：http://3g.yfazqb.com/Article/details/gfsmvsusq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.fktsv.cn/Article/details/ggfjxseuz.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.sjlbkw.cn/Article/details/glrduqfjd.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.fktsv.cn/Article/details/gixyivkyq.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.epnwcf.com/Article/details/gsrldfnqf.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.tarul.cn/Article/details/gvtwyzbsw.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fktsv.cn/Article/details/gngyfskic.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.epnwcf.com/Article/details/gzqjhimhd.sHtML

[A16] 真假值判断规则
来源：http://www.share.fktsv.cn/Article/details/gpevcwzbc.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.sjlbkw.cn/Article/details/gxthjzooo.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.bbcook.cn/Article/details/gxukpjgqt.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.yfazqb.com/Article/details/gbqnxkemp.sHtML

TS:   if (!x) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxujddeol.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fktsv.cn/Article/details/gpxofgtkt.sHtML


<!-- 参考信息 -->