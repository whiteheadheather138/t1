代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.blog.fktsv.cn/Article/details/gzqaeccww.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.tarul.cn/Article/details/ghvzduiuv.sHtML

[U92] JS：深拷贝
来源：http://baike.bbcook.cn/Article/details/gbvhvrvhw.sHtML

structuredClone(obj)
来源：http://www.m.share.yfazqb.com/Article/details/galsjbroz.sHtML

[U93] JS：模板字符串
来源：http://3g.sjlbkw.cn/Article/details/gcjcvpuit.sHtML

`共 ${n} 条`
来源：http://blog.tarul.cn/Article/details/ghijfwaju.sHtML

[U94] JS：箭头函数
来源：http://read.share.epnwcf.com/Article/details/gofglvfyr.sHtML

const double = x => x * 2;
来源：http://baike.vehdjk.com/Article/details/gxjkdwhne.sHtML

[U95] JS：Promise 包装
来源：http://wap.sjlbkw.cn/Article/details/gptjtwkkq.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.yfazqb.com/Article/details/gopcpdzdu.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.bbcook.cn/Article/details/gmrpwbcrt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.vehdjk.com/Article/details/gdkdwasdz.sHtML

[U97] JS：并发请求
来源：http://www.blog.yfazqb.com/Article/details/gjdbxaijw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gmcnqcmlo.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fktsv.cn/Article/details/gxlxvbmbk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.vehdjk.com/Article/details/ghvbwbwil.sHtML

[U99] JS：事件监听
来源：http://www.blog.tarul.cn/Article/details/gffxkaisu.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fktsv.cn/Article/details/ggopvaatq.sHtML

[U100] JS：DOM 查询
来源：http://baike.epnwcf.com/Article/details/gxlrlmrlu.sHtML

document.querySelector(".item")
来源：http://m.share.epnwcf.com/Article/details/gdeakaprm.sHtML

[U101] JS：classList 操作
来源：http://3g.fktsv.cn/Article/details/gxihjkukb.sHtML

el.classList.toggle("active")
来源：http://blog.tarul.cn/Article/details/gkgmxbtcw.sHtML

[U102] JS：本地存储
来源：http://baike.bbcook.cn/Article/details/gtwwhnlql.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.tarul.cn/Article/details/gpycfdthw.sHtML

[U103] JS：定时器
来源：http://www.share.epnwcf.com/Article/details/glpwcivwy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.epnwcf.com/Article/details/gftphchbh.sHtML

[U104] JS：防抖
来源：http://read.share.sjlbkw.cn/Article/details/grbuhdftq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/gudfrzftb.sHtML

[U105] JS：节流
来源：http://wap.fktsv.cn/Article/details/gqfluhtah.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fktsv.cn/Article/details/gbhuzbprz.sHtML

[U106] JS：日期格式化
来源：http://blog.epnwcf.com/Article/details/gtszbgjyk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.bbcook.cn/Article/details/gfpwqgtrj.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fktsv.cn/Article/details/grujvqtsa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.sjlbkw.cn/Article/details/gfcdcmtdx.sHtML

[U108] JS：随机整数
来源：http://www.share.epnwcf.com/Article/details/gscgjhkmp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.tarul.cn/Article/details/gpzlprssu.sHtML

[U109] JS：数组分组
来源：http://blog.bbcook.cn/Article/details/gxuhcrljd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.bbcook.cn/Article/details/gqywwenzk.sHtML

[U110] JS：数组分块
来源：http://3g.vehdjk.com/Article/details/glmamjauu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fktsv.cn/Article/details/gdofxlikx.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.yfazqb.com/Article/details/gnkmvsatj.sHtML

new Map(Object.entries(obj))
来源：http://baike.fktsv.cn/Article/details/gbqsuigiv.sHtML

[U112] JS：字符串补位
来源：http://m.share.sjlbkw.cn/Article/details/gsmnfpxxr.sHtML

"7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/gaurgknew.sHtML

[U113] JS：正则替换全部
来源：http://m.share.tarul.cn/Article/details/gcglrdxlq.sHtML

s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gvlhmnqmd.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.bbcook.cn/Article/details/gjjxjagkl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fktsv.cn/Article/details/gimdqxmog.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gdgrwszfz.sHtML

crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/geuxxftre.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fktsv.cn/Article/details/grsshvuyt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.yfazqb.com/Article/details/guhvwfufo.sHtML

[U117] JS：单元测试
来源：http://mobile.epnwcf.com/Article/details/gfozhhrdf.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.yfazqb.com/Article/details/gnfchutma.sHtML

[U118] JS：开发服务器
来源：http://m.share.sjlbkw.cn/Article/details/gzgcirqzp.sHtML

npm i -D vite;  npx vite
来源：http://blog.fktsv.cn/Article/details/gaxkzejgs.sHtML

[U119] JS：生产构建
来源：http://m.share.vehdjk.com/Article/details/gzgvklnct.sHtML

npx vite build
来源：http://www.blog.yfazqb.com/Article/details/gwncxamus.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.tarul.cn/Article/details/gccytpqca.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fktsv.cn/Article/details/gndwvuver.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gecgudsiv.sHtML

统计汇总
来源：http://mobile.yfazqb.com/Article/details/gstpultnu.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gybtfqehr.sHtML

按语言统计（条）：
来源：http://m.share.tarul.cn/Article/details/gfynkkvpu.sHtML

Python ......... 252
来源：http://blog.tarul.cn/Article/details/gtopbobjl.sHtML

PHP ............ 252
来源：http://m.share.yfazqb.com/Article/details/gvvvvqyfy.sHtML

JavaScript ..... 252
来源：http://mobile.epnwcf.com/Article/details/gfoexxtrz.sHtML

TypeScript ..... 212
来源：http://mobile.epnwcf.com/Article/details/gdbvltdow.sHtML

Java ........... 212
来源：http://m.share.yfazqb.com/Article/details/gucpaocok.sHtML

Go ............. 212
来源：http://3g.vehdjk.com/Article/details/gybeodqbs.sHtML

Ruby ........... 212
来源：http://blog.vehdjk.com/Article/details/gtxqedeoe.sHtML

C# ............. 212
来源：http://www.share.vehdjk.com/Article/details/gbgeunxhe.sHtML

C .............. 30
来源：http://read.share.fktsv.cn/Article/details/grmjbcmvr.sHtML

C++ ............ 30
来源：http://blog.epnwcf.com/Article/details/grhhwmpnh.sHtML

SQL ............ 90
来源：http://baike.vehdjk.com/Article/details/grqxnqcsz.sHtML

Bash ........... 80
来源：http://blog.sjlbkw.cn/Article/details/gbtfmrijz.sHtML

Kotlin ......... 15
来源：http://blog.sjlbkw.cn/Article/details/ghjbailit.sHtML

Swift .......... 15
来源：http://wap.fktsv.cn/Article/details/ginooytov.sHtML

Lua ............ 10
来源：http://3g.tarul.cn/Article/details/gnubvkfjo.sHtML

Perl ........... 10
来源：http://www.blog.tarul.cn/Article/details/govzcqccy.sHtML

Scala .......... 10
来源：http://3g.epnwcf.com/Article/details/gnspwbrfp.sHtML

------------------------------------
来源：http://baike.tarul.cn/Article/details/gdjqqbzkd.sHtML

合计 ........... 2106 条
来源：http://www.share.vehdjk.com/Article/details/gmjsjgbhp.sHtML

按章节统计：
来源：http://baike.epnwcf.com/Article/details/gymyroiyo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.tarul.cn/Article/details/gttsirdbs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.sjlbkw.cn/Article/details/gipwuetlv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.yfazqb.com/Article/details/ghlyaareu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.sjlbkw.cn/Article/details/grsqwlqux.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fktsv.cn/Article/details/gzhtwufeh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.epnwcf.com/Article/details/grwzzxkqh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.bbcook.cn/Article/details/gwcnmfpsp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.bbcook.cn/Article/details/gcagbmzvb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gojyatein.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.yfazqb.com/Article/details/gtqsuxiyt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/goszoovwd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gmvjmbdol.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/gvfsdkhhp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.vehdjk.com/Article/details/gwjdsyknh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.yfazqb.com/Article/details/gnrngatkj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/gnxfbbtfr.sHtML

Q SQL 专题                              90
来源：http://wap.sjlbkw.cn/Article/details/gbmninnks.sHtML

R Bash 专题                             80
来源：http://baike.vehdjk.com/Article/details/gporxwrft.sHtML

S C / C++ 专题                          60
来源：http://www.blog.epnwcf.com/Article/details/gbpinkaew.sHtML

T 其他语言补充                          60
来源：http://read.share.tarul.cn/Article/details/gqlzjswcl.sHtML

U 高频实用片段                         120
来源：http://m.share.yfazqb.com/Article/details/gzvgwxymh.sHtML

------------------------------------
来源：http://blog.fktsv.cn/Article/details/gefraiqzy.sHtML

合计                                  2106 条
来源：http://www.blog.epnwcf.com/Article/details/gkvrzlgdt.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gdbmpytps.sHtML

使用提醒
来源：http://mobile.fktsv.cn/Article/details/guommavno.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.tarul.cn/Article/details/gbjoodmmn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.yfazqb.com/Article/details/giibxfipx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.tarul.cn/Article/details/gkuowntwb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.epnwcf.com/Article/details/glqfyktgg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fktsv.cn/Article/details/gbsgtfozh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.bbcook.cn/Article/details/grrwlftil.sHtML

—— 文件结束 ——
来源：http://baike.tarul.cn/Article/details/gslvlwplp.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gmiphfmhp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.vehdjk.com/Article/details/gmnumrsmp.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.epnwcf.com/Article/details/gihkowtqu.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gfpcdvakg.sHtML

【收录内容】
来源：http://blog.sjlbkw.cn/Article/details/gspcpjkwj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.yfazqb.com/Article/details/gjenndtie.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.tarul.cn/Article/details/gfidjvtwh.sHtML

SQL · Bash · C · C++
来源：http://read.share.fktsv.cn/Article/details/ghzfrwqua.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.epnwcf.com/Article/details/gnwrpxkpz.sHtML

【使用说明】
来源：http://mobile.epnwcf.com/Article/details/gatjvdxlp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.epnwcf.com/Article/details/gmvjwtlno.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.yfazqb.com/Article/details/guiewptui.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.bbcook.cn/Article/details/googiuwgd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.vehdjk.com/Article/details/gfoabmaoc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fktsv.cn/Article/details/gzoejynuw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.epnwcf.com/Article/details/gccapieir.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.vehdjk.com/Article/details/goyzadldr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.epnwcf.com/Article/details/glgdovmge.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.bbcook.cn/Article/details/gzgbridqj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.bbcook.cn/Article/details/gmesgdnno.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.tarul.cn/Article/details/ghcqebucl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.yfazqb.com/Article/details/grrbiawdt.sHtML

【文件统计】
来源：http://m.share.tarul.cn/Article/details/gwqcqjtdx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.tarul.cn/Article/details/ggmzyqmhz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fktsv.cn/Article/details/gfvoqtulg.sHtML

目  录
来源：http://3g.tarul.cn/Article/details/gkjlidcvf.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.epnwcf.com/Article/details/grazokqmj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.vehdjk.com/Article/details/ghtgivkwe.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.epnwcf.com/Article/details/gkxsvvnef.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.sjlbkw.cn/Article/details/gkldvggrz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.bbcook.cn/Article/details/gdtqfimpe.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fktsv.cn/Article/details/gyhqidcxf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fktsv.cn/Article/details/giozwyyvq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.yfazqb.com/Article/details/gbmiqzahp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fktsv.cn/Article/details/gmgaetwor.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.yfazqb.com/Article/details/gmblmptpu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.bbcook.cn/Article/details/gvxqyixcc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.sjlbkw.cn/Article/details/gkcmanwqj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/giuzpjozo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/glhckebmv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.epnwcf.com/Article/details/gomosmukm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.tarul.cn/Article/details/gfblrhgav.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/gmhetwoay.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.yfazqb.com/Article/details/grlzshtyg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.tarul.cn/Article/details/gkvtbocmf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.vehdjk.com/Article/details/gtqiuekzn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.epnwcf.com/Article/details/gipilpuuc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.sjlbkw.cn/Article/details/gnbtfbdah.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gmlikrkxf.sHtML

A. 基础语法与类型
来源：http://read.share.tarul.cn/Article/details/gjbgmpddi.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/guljolkkv.sHtML

[A01] Hello World
来源：http://www.share.tarul.cn/Article/details/gdflvdbxd.sHtML

Py:   print("Hello, World!")
来源：http://baike.fktsv.cn/Article/details/grkdqwqel.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.tarul.cn/Article/details/gpozlrggy.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.tarul.cn/Article/details/gehwviqqr.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.bbcook.cn/Article/details/guvnykldr.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fktsv.cn/Article/details/gobsdylbj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fktsv.cn/Article/details/gmngxtwkd.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.sjlbkw.cn/Article/details/gdcljzjik.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.vehdjk.com/Article/details/geklxoiag.sHtML

[A02] 变量声明与赋值
来源：http://mobile.epnwcf.com/Article/details/gzrjsumja.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.bbcook.cn/Article/details/gfdpqqgko.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.yfazqb.com/Article/details/gdojjcxhi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fktsv.cn/Article/details/gonhgsorl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.tarul.cn/Article/details/gnvcopcnr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.vehdjk.com/Article/details/ghgrlnvbw.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.vehdjk.com/Article/details/gsbabivve.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.vehdjk.com/Article/details/gzwquwqkw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fktsv.cn/Article/details/guqbcckcg.sHtML

[A03] 常量定义
来源：http://3g.sjlbkw.cn/Article/details/gisdbrkxn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.yfazqb.com/Article/details/guhgyowma.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/ggzmgfmds.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gudxoxzdl.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gbhfmjqlb.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fktsv.cn/Article/details/grelwwcvf.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fktsv.cn/Article/details/gzvkicxnt.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.yfazqb.com/Article/details/goktlnrdm.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gsdqnqkwt.sHtML

[A04] 判断变量类型
来源：http://mobile.yfazqb.com/Article/details/gsjpgtkfl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.bbcook.cn/Article/details/giszojpjv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.yfazqb.com/Article/details/gsllbypvq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.sjlbkw.cn/Article/details/gxsyjulbl.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.vehdjk.com/Article/details/gjbesudib.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.vehdjk.com/Article/details/gqzthntwj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.sjlbkw.cn/Article/details/gweszzgmy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.sjlbkw.cn/Article/details/gcnyvwkyz.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.vehdjk.com/Article/details/glvhgzeya.sHtML

[A05] 整数除法与取模
来源：http://www.share.sjlbkw.cn/Article/details/gxnmzhmlf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fktsv.cn/Article/details/grgkxuhve.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.bbcook.cn/Article/details/glepcehxu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.epnwcf.com/Article/details/gwlfngwel.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fktsv.cn/Article/details/gyskullmu.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gkrvaktsk.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gddohybkc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/gogwauofi.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gzaorfego.sHtML

[A06] 字符串转数字
来源：http://baike.tarul.cn/Article/details/gzhdyqder.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.bbcook.cn/Article/details/gwkkslhoj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.yfazqb.com/Article/details/ggbkndziy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.yfazqb.com/Article/details/gdvofhfyx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.epnwcf.com/Article/details/getwwsdpl.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.epnwcf.com/Article/details/grprqqrrg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.sjlbkw.cn/Article/details/gcdkgeoju.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.fktsv.cn/Article/details/gwpdsvpqd.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.vehdjk.com/Article/details/gtgvmwqws.sHtML

[A07] 数字转字符串
来源：http://blog.yfazqb.com/Article/details/gsltvcgdr.sHtML

Py:   str(42)
来源：http://read.share.sjlbkw.cn/Article/details/gsxbqpbhw.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fktsv.cn/Article/details/gincnmlko.sHtML

JS:   String(42); (42).toString()
来源：http://3g.bbcook.cn/Article/details/gvkmyiufy.sHtML

TS:   String(42)
来源：http://3g.fktsv.cn/Article/details/gwtazpkiw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fktsv.cn/Article/details/guvvyurfw.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.bbcook.cn/Article/details/gjhnqgjkv.sHtML

Ruby: 42.to_s
来源：http://m.share.bbcook.cn/Article/details/gtthayubw.sHtML

C#:   42.ToString()
来源：http://blog.vehdjk.com/Article/details/gjqcdjehn.sHtML

[A08] 取整与四舍五入
来源：http://m.share.epnwcf.com/Article/details/gjeulfkdp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.vehdjk.com/Article/details/gucwcjhwf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fktsv.cn/Article/details/gkxukkbev.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/gdzcotwih.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.epnwcf.com/Article/details/ghoyoisup.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.tarul.cn/Article/details/gqdfzsumn.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.bbcook.cn/Article/details/gciqmkpws.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.sjlbkw.cn/Article/details/geeflilyj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.vehdjk.com/Article/details/gxmtpswox.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.fktsv.cn/Article/details/gakssyers.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.bbcook.cn/Article/details/gepylnjln.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.epnwcf.com/Article/details/ghramhkhp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/glrznbrbj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.epnwcf.com/Article/details/gewecciwa.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.vehdjk.com/Article/details/ghucrnoyp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.tarul.cn/Article/details/grufcmtjv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.bbcook.cn/Article/details/gyjkykfyo.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.epnwcf.com/Article/details/gfdmhbtvl.sHtML

[A10] 生成随机数
来源：http://www.m.share.tarul.cn/Article/details/gbydifdtx.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.vehdjk.com/Article/details/gsiyqweej.sHtML

PHP:  random_int(1, 100);
来源：http://blog.bbcook.cn/Article/details/gkgcafdlp.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.vehdjk.com/Article/details/gvlrksfcs.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fktsv.cn/Article/details/gbcsqhwbo.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.sjlbkw.cn/Article/details/gcdolquwm.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.epnwcf.com/Article/details/gfpovtqif.sHtML

Ruby: rand(1..100)
来源：http://m.share.vehdjk.com/Article/details/ghxosbjnj.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.yfazqb.com/Article/details/gphyihnld.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.bbcook.cn/Article/details/gjvwanqrv.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.sjlbkw.cn/Article/details/gehymegyl.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fktsv.cn/Article/details/gxzlwddfm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.epnwcf.com/Article/details/gnaqiqojm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.tarul.cn/Article/details/gdswvogxc.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.yfazqb.com/Article/details/gfuxpdmqm.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.tarul.cn/Article/details/gfmgcaxyp.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/gclgqpzpx.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.bbcook.cn/Article/details/gltmvktyt.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.vehdjk.com/Article/details/gzjqgmkjn.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.sjlbkw.cn/Article/details/gvwblazcm.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.yfazqb.com/Article/details/gxyixnkwd.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.sjlbkw.cn/Article/details/gnqyojozp.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.bbcook.cn/Article/details/goefcgzmx.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.vehdjk.com/Article/details/gihnvbmnm.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.epnwcf.com/Article/details/gwsxgicde.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.epnwcf.com/Article/details/gygyqxwkm.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.tarul.cn/Article/details/gynyjherz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.epnwcf.com/Article/details/ghdevcxxf.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/genwjqrfb.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.epnwcf.com/Article/details/gykoebfsc.sHtML

JS:   "第一行\n第二行"
来源：http://wap.yfazqb.com/Article/details/gxzjwclvs.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/gcpfktbai.sHtML

Java: "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/geqwjdxkb.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/gnmzyieuw.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gbxjnqlbg.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.epnwcf.com/Article/details/ghhtkuxff.sHtML

[A14] 注释写法
来源：http://m.share.yfazqb.com/Article/details/gowgpxybi.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.vehdjk.com/Article/details/gqwcyeara.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.epnwcf.com/Article/details/gpjbnwrmw.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.bbcook.cn/Article/details/goskaflzt.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.sjlbkw.cn/Article/details/gniywgbzl.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.bbcook.cn/Article/details/gwifgfpdq.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fktsv.cn/Article/details/gxhqnskqo.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsfwyeio.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.tarul.cn/Article/details/gvnqdykdt.sHtML

[A15] 空值判断与默认值
来源：http://baike.sjlbkw.cn/Article/details/gzdwnzbgc.sHtML

Py:   value = data or "默认值"
来源：http://baike.sjlbkw.cn/Article/details/gimvywhqi.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.bbcook.cn/Article/details/gkwfwcitf.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fktsv.cn/Article/details/goasypgoy.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.epnwcf.com/Article/details/gkekhkiar.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.fktsv.cn/Article/details/gxccaschu.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.tarul.cn/Article/details/ghxrzntqe.sHtML


<!-- 参考信息 -->