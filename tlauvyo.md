代发 wailian999

[U97] JS：并发请求
来源：http://read.share.tarul.cn/Article/details/gxgaflbsw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gaiwwxeos.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.epnwcf.com/Article/details/glszglvky.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.yfazqb.com/Article/details/gfcxvvllx.sHtML

[U99] JS：事件监听
来源：http://www.blog.vehdjk.com/Article/details/gkmqockxx.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.bbcook.cn/Article/details/gnkgzlmal.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.epnwcf.com/Article/details/grzqwtpjc.sHtML

document.querySelector(".item")
来源：http://wap.vehdjk.com/Article/details/gugeatgye.sHtML

[U101] JS：classList 操作
来源：http://wap.sjlbkw.cn/Article/details/gymxzvncy.sHtML

el.classList.toggle("active")
来源：http://www.share.tarul.cn/Article/details/glaeyjmng.sHtML

[U102] JS：本地存储
来源：http://www.share.fktsv.cn/Article/details/gvmeiprxk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.yfazqb.com/Article/details/ggeuhvyqj.sHtML

[U103] JS：定时器
来源：http://read.share.vehdjk.com/Article/details/gwopwrxte.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.vehdjk.com/Article/details/gwroyomgn.sHtML

[U104] JS：防抖
来源：http://read.share.epnwcf.com/Article/details/gdneootqf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/gvwtaxnrz.sHtML

[U105] JS：节流
来源：http://3g.yfazqb.com/Article/details/gahkspysc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.bbcook.cn/Article/details/gtjgkmndo.sHtML

[U106] JS：日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/gqxatyxih.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.sjlbkw.cn/Article/details/gnnfezjag.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.yfazqb.com/Article/details/gonjrglkj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gdalnjrrf.sHtML

[U108] JS：随机整数
来源：http://baike.epnwcf.com/Article/details/ghussxicr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.epnwcf.com/Article/details/ghpdpuhro.sHtML

[U109] JS：数组分组
来源：http://www.blog.tarul.cn/Article/details/gyscdozqf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fktsv.cn/Article/details/gdyfassne.sHtML

[U110] JS：数组分块
来源：http://www.m.share.epnwcf.com/Article/details/gngbnalxz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.tarul.cn/Article/details/gvqlblopo.sHtML

[U111] JS：对象转 Map
来源：http://mobile.sjlbkw.cn/Article/details/gzoqhhcrp.sHtML

new Map(Object.entries(obj))
来源：http://wap.fktsv.cn/Article/details/gilrubyyv.sHtML

[U112] JS：字符串补位
来源：http://www.share.fktsv.cn/Article/details/grfnihzpp.sHtML

"7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gvibhvvsy.sHtML

[U113] JS：正则替换全部
来源：http://blog.tarul.cn/Article/details/gvvmxflgl.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gtuckdqza.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.tarul.cn/Article/details/gndprnlxo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.tarul.cn/Article/details/gtpxwaefu.sHtML

[U115] JS：生成 UUID
来源：http://read.share.epnwcf.com/Article/details/gbpougstk.sHtML

crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/gjkjxwarn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.tarul.cn/Article/details/gsoysyeus.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.tarul.cn/Article/details/gugllbjjl.sHtML

[U117] JS：单元测试
来源：http://blog.bbcook.cn/Article/details/gxuebmtmy.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.vehdjk.com/Article/details/gsmiayvkf.sHtML

[U118] JS：开发服务器
来源：http://baike.epnwcf.com/Article/details/gnfrshrsw.sHtML

npm i -D vite;  npx vite
来源：http://wap.sjlbkw.cn/Article/details/gsrjshkim.sHtML

[U119] JS：生产构建
来源：http://read.share.sjlbkw.cn/Article/details/gramevbxb.sHtML

npx vite build
来源：http://www.share.vehdjk.com/Article/details/gjlkandxv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fktsv.cn/Article/details/gdynchsuh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.bbcook.cn/Article/details/gqmpplsbj.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gxetodbsp.sHtML

统计汇总
来源：http://wap.tarul.cn/Article/details/gubvykwxz.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gilqjmshh.sHtML

按语言统计（条）：
来源：http://www.share.fktsv.cn/Article/details/gytphcbno.sHtML

Python ......... 252
来源：http://3g.yfazqb.com/Article/details/gminofnby.sHtML

PHP ............ 252
来源：http://blog.sjlbkw.cn/Article/details/gogsojxrw.sHtML

JavaScript ..... 252
来源：http://www.blog.vehdjk.com/Article/details/gwmxubkqi.sHtML

TypeScript ..... 212
来源：http://baike.yfazqb.com/Article/details/gloiqimld.sHtML

Java ........... 212
来源：http://baike.fktsv.cn/Article/details/gpkwmmegr.sHtML

Go ............. 212
来源：http://www.blog.epnwcf.com/Article/details/gpveizrvk.sHtML

Ruby ........... 212
来源：http://www.blog.fktsv.cn/Article/details/grvsljnkv.sHtML

C# ............. 212
来源：http://blog.yfazqb.com/Article/details/gnmriogpi.sHtML

C .............. 30
来源：http://mobile.bbcook.cn/Article/details/gsxxygupv.sHtML

C++ ............ 30
来源：http://blog.epnwcf.com/Article/details/goytuabcq.sHtML

SQL ............ 90
来源：http://3g.bbcook.cn/Article/details/gpekpuwcw.sHtML

Bash ........... 80
来源：http://baike.fktsv.cn/Article/details/gzacxtdal.sHtML

Kotlin ......... 15
来源：http://read.share.yfazqb.com/Article/details/gnjtmuxhe.sHtML

Swift .......... 15
来源：http://www.m.share.vehdjk.com/Article/details/gfikhlsmn.sHtML

Lua ............ 10
来源：http://www.share.bbcook.cn/Article/details/gufekghbw.sHtML

Perl ........... 10
来源：http://3g.vehdjk.com/Article/details/gpwirkzad.sHtML

Scala .......... 10
来源：http://baike.bbcook.cn/Article/details/gwqhyzhnx.sHtML

------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gfzqfywue.sHtML

合计 ........... 2106 条
来源：http://3g.vehdjk.com/Article/details/gjptizcgn.sHtML

按章节统计：
来源：http://m.share.tarul.cn/Article/details/gxckkwmdk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.epnwcf.com/Article/details/gcdklfzhd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.vehdjk.com/Article/details/gekhhougx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.vehdjk.com/Article/details/gtoudhbcj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.sjlbkw.cn/Article/details/gqzwboyes.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.tarul.cn/Article/details/gzftksxvj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.sjlbkw.cn/Article/details/goqachaxi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.epnwcf.com/Article/details/gbdtfaheh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.epnwcf.com/Article/details/ghioufvxl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/grgzhnlwr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fktsv.cn/Article/details/gzeescoig.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/ganxjogvg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/gxtsfdmip.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gknesxghd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fktsv.cn/Article/details/gmedbhdyp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.yfazqb.com/Article/details/grwezhvrb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/glsgcqryh.sHtML

Q SQL 专题                              90
来源：http://blog.sjlbkw.cn/Article/details/gsrbxzhpj.sHtML

R Bash 专题                             80
来源：http://mobile.vehdjk.com/Article/details/gxspikpgb.sHtML

S C / C++ 专题                          60
来源：http://3g.bbcook.cn/Article/details/gjqbsevak.sHtML

T 其他语言补充                          60
来源：http://wap.fktsv.cn/Article/details/gajzahynx.sHtML

U 高频实用片段                         120
来源：http://www.blog.epnwcf.com/Article/details/gwtfgngfd.sHtML

------------------------------------
来源：http://m.share.fktsv.cn/Article/details/glaupwdjn.sHtML

合计                                  2106 条
来源：http://read.share.fktsv.cn/Article/details/gwuwnmynm.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gojwvfneq.sHtML

使用提醒
来源：http://www.m.share.bbcook.cn/Article/details/giycbuqhe.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.tarul.cn/Article/details/gwiocdtty.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.epnwcf.com/Article/details/glmrgzixr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.yfazqb.com/Article/details/glirjweqw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.epnwcf.com/Article/details/gnulavrve.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.vehdjk.com/Article/details/gtmdnqfry.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.sjlbkw.cn/Article/details/gqqojhbiz.sHtML

—— 文件结束 ——
来源：http://read.share.vehdjk.com/Article/details/gwcelkkkg.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gvzffhkly.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fktsv.cn/Article/details/gpvcluwfw.sHtML

Common Programming Examples Cheat Book
来源：http://blog.epnwcf.com/Article/details/gdxnevdde.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gjgjgyhkr.sHtML

【收录内容】
来源：http://wap.epnwcf.com/Article/details/gaftgqljt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.yfazqb.com/Article/details/ginrkmsgv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.epnwcf.com/Article/details/gmhryaend.sHtML

SQL · Bash · C · C++
来源：http://read.share.sjlbkw.cn/Article/details/gxmpmpjfm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.epnwcf.com/Article/details/gotyijblz.sHtML

【使用说明】
来源：http://read.share.vehdjk.com/Article/details/gdehzrirq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.sjlbkw.cn/Article/details/gpdjfobxv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.yfazqb.com/Article/details/gkccglcpf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.bbcook.cn/Article/details/giiaynrev.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.yfazqb.com/Article/details/gcneivuer.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.vehdjk.com/Article/details/gdmrezeha.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.tarul.cn/Article/details/gptfwsgcz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.vehdjk.com/Article/details/gxrpkrpdf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.yfazqb.com/Article/details/gkfgvzriu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.bbcook.cn/Article/details/gxuhmussg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnufmwga.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.tarul.cn/Article/details/goctcvuxw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.vehdjk.com/Article/details/gpcabtcsq.sHtML

【文件统计】
来源：http://m.share.fktsv.cn/Article/details/gcupukbda.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fktsv.cn/Article/details/gwnicjknt.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gtnliobvr.sHtML

目  录
来源：http://blog.vehdjk.com/Article/details/gdktvpirg.sHtML

--------------------------------------------------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gaacpytgz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.epnwcf.com/Article/details/ghajnpzsv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/gjlrblabn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.epnwcf.com/Article/details/glenhhxgw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.tarul.cn/Article/details/ggmocspip.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.sjlbkw.cn/Article/details/glexgmgzi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.vehdjk.com/Article/details/gthbodyzk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.yfazqb.com/Article/details/girrgnecu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.epnwcf.com/Article/details/ghzacwckb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/gqavjwnep.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.bbcook.cn/Article/details/gwioocsnm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/gkbbtmqfv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/gimalfqsu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/gwvysrtek.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.vehdjk.com/Article/details/gbmvxmkdg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.tarul.cn/Article/details/golxprarp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gezjoapaa.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.vehdjk.com/Article/details/gqmubdptw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.tarul.cn/Article/details/ghmnepftz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fktsv.cn/Article/details/gwntszbpk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.bbcook.cn/Article/details/glbacvjfy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.vehdjk.com/Article/details/gwvxevhmc.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gisyerhcx.sHtML

A. 基础语法与类型
来源：http://mobile.epnwcf.com/Article/details/gfupgbjay.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gnwwlefce.sHtML

[A01] Hello World
来源：http://wap.bbcook.cn/Article/details/gekaengsg.sHtML

Py:   print("Hello, World!")
来源：http://m.share.epnwcf.com/Article/details/gvlvwhalq.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.sjlbkw.cn/Article/details/ggvuaqtxw.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.sjlbkw.cn/Article/details/goshqtzyi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.vehdjk.com/Article/details/gmnyulsja.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.bbcook.cn/Article/details/gasknmpow.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fktsv.cn/Article/details/geepwowiz.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.vehdjk.com/Article/details/gbhjqxxgt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.yfazqb.com/Article/details/gckhcszqu.sHtML

[A02] 变量声明与赋值
来源：http://blog.epnwcf.com/Article/details/ghkzfujsz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.yfazqb.com/Article/details/ggrodyntg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fktsv.cn/Article/details/guehrbnjs.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fktsv.cn/Article/details/gyeqxcxms.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.vehdjk.com/Article/details/gluneqfck.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gkyuamypr.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fktsv.cn/Article/details/gqfynxiyk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.bbcook.cn/Article/details/gkwowfqnv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gpxxqplck.sHtML

[A03] 常量定义
来源：http://read.share.fktsv.cn/Article/details/gcfyhbvij.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.yfazqb.com/Article/details/grfkzvjmu.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gglsuwmki.sHtML

JS:   const PI = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gfreudcfh.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gyetyldja.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/glpyrfzsg.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fktsv.cn/Article/details/gsmdfkgge.sHtML

Ruby: PI = 3.14159
来源：http://read.share.epnwcf.com/Article/details/gytpbepsi.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gvvqtatjg.sHtML

[A04] 判断变量类型
来源：http://m.share.vehdjk.com/Article/details/gvcdtpnnt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fktsv.cn/Article/details/guggnqlad.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.sjlbkw.cn/Article/details/gswioxnkb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.sjlbkw.cn/Article/details/gjeeekymb.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fktsv.cn/Article/details/gyhzuyhnw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.vehdjk.com/Article/details/gpkvvvgcc.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.tarul.cn/Article/details/grkrvrgti.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfjltycd.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.vehdjk.com/Article/details/gbahpesbg.sHtML

[A05] 整数除法与取模
来源：http://wap.sjlbkw.cn/Article/details/glccctjjk.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.yfazqb.com/Article/details/gmyzutebq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gujbajgtd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/glgsjnfec.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gqmipuuew.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gzbwhkeeh.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gkovistiu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.epnwcf.com/Article/details/gbyrutjdf.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fktsv.cn/Article/details/gbfjxqvhx.sHtML

[A06] 字符串转数字
来源：http://www.share.fktsv.cn/Article/details/geeqfmdhj.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.sjlbkw.cn/Article/details/gkkkcujpm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.tarul.cn/Article/details/gkcuzgjjr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.bbcook.cn/Article/details/grbdnheib.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.tarul.cn/Article/details/gaxtcnxhe.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.bbcook.cn/Article/details/geaakxhjw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.tarul.cn/Article/details/gsbltehxe.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.sjlbkw.cn/Article/details/gucgorxku.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.bbcook.cn/Article/details/gwsmxoxdx.sHtML

[A07] 数字转字符串
来源：http://mobile.bbcook.cn/Article/details/gqrhvojiq.sHtML

Py:   str(42)
来源：http://m.share.fktsv.cn/Article/details/gdnhjuvpx.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.epnwcf.com/Article/details/glwugyadv.sHtML

JS:   String(42); (42).toString()
来源：http://baike.tarul.cn/Article/details/goquznlqv.sHtML

TS:   String(42)
来源：http://www.blog.bbcook.cn/Article/details/gevsokgve.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.bbcook.cn/Article/details/giswkgssy.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.sjlbkw.cn/Article/details/gyusvfdqq.sHtML

Ruby: 42.to_s
来源：http://www.m.share.yfazqb.com/Article/details/glzqqdhww.sHtML

C#:   42.ToString()
来源：http://baike.bbcook.cn/Article/details/godqusnem.sHtML

[A08] 取整与四舍五入
来源：http://read.share.epnwcf.com/Article/details/gzlepbekq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/gcjxtzakw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fktsv.cn/Article/details/gzybgkksg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.sjlbkw.cn/Article/details/gsnmmrxti.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.tarul.cn/Article/details/gvsyhegbb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.vehdjk.com/Article/details/gjtvbhkez.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.vehdjk.com/Article/details/guxvepkod.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.vehdjk.com/Article/details/gschowzin.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.yfazqb.com/Article/details/gehxnepxo.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.bbcook.cn/Article/details/gxossxjji.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.vehdjk.com/Article/details/guphsorhy.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gjklxvuly.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.tarul.cn/Article/details/gmrsxczro.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.yfazqb.com/Article/details/gwmgqearb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gspdeydxm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.vehdjk.com/Article/details/gjgqxzknc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.yfazqb.com/Article/details/gatidfssx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.tarul.cn/Article/details/gaqwafmug.sHtML

[A10] 生成随机数
来源：http://baike.tarul.cn/Article/details/ggidrjmhq.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.fktsv.cn/Article/details/gwsqilreo.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyxzywtt.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.epnwcf.com/Article/details/grnnuwoxx.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.yfazqb.com/Article/details/gvmehpgvf.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.tarul.cn/Article/details/gjolhsbqj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.yfazqb.com/Article/details/gckavjbrq.sHtML

Ruby: rand(1..100)
来源：http://read.share.vehdjk.com/Article/details/gcfqsfjbz.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.tarul.cn/Article/details/gtuhwulbt.sHtML

[A11] 条件表达式（三元）
来源：http://baike.vehdjk.com/Article/details/gmscrnpay.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.sjlbkw.cn/Article/details/gsvduxsum.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/gldmbmwso.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.fktsv.cn/Article/details/geamnnujv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.epnwcf.com/Article/details/gdkscwmvc.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.yfazqb.com/Article/details/gnubjpluw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.tarul.cn/Article/details/gcpzzmbap.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.vehdjk.com/Article/details/geikpjhxm.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/gcqodttkv.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.tarul.cn/Article/details/ggxvisovb.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.sjlbkw.cn/Article/details/gouqxiqho.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.vehdjk.com/Article/details/gzpzhkkcj.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.epnwcf.com/Article/details/gwgaotlpa.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.tarul.cn/Article/details/gshekndrd.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.vehdjk.com/Article/details/gyujezqev.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.bbcook.cn/Article/details/gkspcjquj.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.sjlbkw.cn/Article/details/gxbphntie.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.tarul.cn/Article/details/goslrwdwf.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.bbcook.cn/Article/details/gefluankp.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/gsyflzblh.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gdeyjvqfb.sHtML

JS:   "第一行\n第二行"
来源：http://wap.yfazqb.com/Article/details/gyfhozbab.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gmemizzst.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.bbcook.cn/Article/details/gvlpurwno.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fktsv.cn/Article/details/gjvarjtmb.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/gnfsvaknq.sHtML

C#:   "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/gljbpdctw.sHtML

[A14] 注释写法
来源：http://3g.tarul.cn/Article/details/gpnclinuv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.bbcook.cn/Article/details/gzbndidhb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fktsv.cn/Article/details/gsofcxfjg.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.tarul.cn/Article/details/gqkknrqrl.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.epnwcf.com/Article/details/gvkieknha.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.sjlbkw.cn/Article/details/gfazmeyki.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.tarul.cn/Article/details/gckbrkabj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.fktsv.cn/Article/details/glblatktm.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.yfazqb.com/Article/details/gbkhrkkfd.sHtML

[A15] 空值判断与默认值
来源：http://mobile.bbcook.cn/Article/details/gtqywnhbb.sHtML

Py:   value = data or "默认值"
来源：http://mobile.fktsv.cn/Article/details/gcskvqpzf.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.epnwcf.com/Article/details/gnefjriyh.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.fktsv.cn/Article/details/gbmkfxhsi.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.bbcook.cn/Article/details/gfjdmhiyl.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.bbcook.cn/Article/details/gmaxxlpop.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.tarul.cn/Article/details/gcnkbibol.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.vehdjk.com/Article/details/gpjfjaplh.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.bbcook.cn/Article/details/gnlzigiiw.sHtML

[A16] 真假值判断规则
来源：http://www.share.bbcook.cn/Article/details/gmxqqntrv.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.vehdjk.com/Article/details/gnhbfezxf.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fktsv.cn/Article/details/gtocgnwqh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.epnwcf.com/Article/details/gxweyrvim.sHtML

TS:   if (!x) {}
来源：http://blog.yfazqb.com/Article/details/gfbqsmiyl.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.yfazqb.com/Article/details/gqatwsejc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.bbcook.cn/Article/details/gsurerkwi.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fktsv.cn/Article/details/giuyqqmxn.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.yfazqb.com/Article/details/grdguuurj.sHtML

[A17] 位运算
来源：http://read.share.yfazqb.com/Article/details/gkaihvwxw.sHtML


<!-- 参考信息 -->