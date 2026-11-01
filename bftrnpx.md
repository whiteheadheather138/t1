代发 wailian999

[U91] JS：对象键值遍历
来源：http://baike.epnwcf.com/Article/details/giqfepgza.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fktsv.cn/Article/details/gbvqfugwj.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fktsv.cn/Article/details/gghusnwjr.sHtML

structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/gdkmufmbd.sHtML

[U93] JS：模板字符串
来源：http://mobile.bbcook.cn/Article/details/ggkdmndxz.sHtML

`共 ${n} 条`
来源：http://www.blog.vehdjk.com/Article/details/gdwyzsjdo.sHtML

[U94] JS：箭头函数
来源：http://baike.yfazqb.com/Article/details/ghrgjpaie.sHtML

const double = x => x * 2;
来源：http://m.share.tarul.cn/Article/details/gwawktnhf.sHtML

[U95] JS：Promise 包装
来源：http://baike.epnwcf.com/Article/details/ghxygdwqp.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.epnwcf.com/Article/details/gxqphppmt.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.vehdjk.com/Article/details/gwcgzbzpb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gysrjqfqo.sHtML

[U97] JS：并发请求
来源：http://read.share.sjlbkw.cn/Article/details/gpexytywj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gfujsjjlb.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.epnwcf.com/Article/details/gdmiwmywp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.epnwcf.com/Article/details/gxnftvtch.sHtML

[U99] JS：事件监听
来源：http://www.m.share.bbcook.cn/Article/details/gdpwvcqrx.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fktsv.cn/Article/details/ghwudahrg.sHtML

[U100] JS：DOM 查询
来源：http://m.share.tarul.cn/Article/details/glohpfzyk.sHtML

document.querySelector(".item")
来源：http://m.share.sjlbkw.cn/Article/details/gvgcfukpf.sHtML

[U101] JS：classList 操作
来源：http://3g.yfazqb.com/Article/details/guqkjqlny.sHtML

el.classList.toggle("active")
来源：http://3g.yfazqb.com/Article/details/gqkhqkoao.sHtML

[U102] JS：本地存储
来源：http://www.blog.fktsv.cn/Article/details/gponrkjsl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fktsv.cn/Article/details/gorzqkaij.sHtML

[U103] JS：定时器
来源：http://www.blog.bbcook.cn/Article/details/gqeoclvrj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.bbcook.cn/Article/details/gtgqktdbv.sHtML

[U104] JS：防抖
来源：http://wap.yfazqb.com/Article/details/ghvqecyag.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/gqkihicbe.sHtML

[U105] JS：节流
来源：http://read.share.fktsv.cn/Article/details/gjrrombno.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gvanhkhia.sHtML

[U106] JS：日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gcyyjuxml.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.epnwcf.com/Article/details/gxooqssgp.sHtML

[U107] JS：数字千分位
来源：http://blog.vehdjk.com/Article/details/gzcrckria.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.tarul.cn/Article/details/gumainrem.sHtML

[U108] JS：随机整数
来源：http://blog.epnwcf.com/Article/details/gmjdsdaud.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.epnwcf.com/Article/details/gsnjykofw.sHtML

[U109] JS：数组分组
来源：http://wap.vehdjk.com/Article/details/gugzqudzr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.yfazqb.com/Article/details/goddayaiu.sHtML

[U110] JS：数组分块
来源：http://read.share.vehdjk.com/Article/details/gmqctsffl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.tarul.cn/Article/details/gyegrfpsp.sHtML

[U111] JS：对象转 Map
来源：http://baike.tarul.cn/Article/details/gphdikkzh.sHtML

new Map(Object.entries(obj))
来源：http://mobile.epnwcf.com/Article/details/gqvatzprm.sHtML

[U112] JS：字符串补位
来源：http://blog.tarul.cn/Article/details/gfroovvzz.sHtML

"7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gdvntpqny.sHtML

[U113] JS：正则替换全部
来源：http://wap.yfazqb.com/Article/details/gnvjalgau.sHtML

s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gaijqyxmp.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.yfazqb.com/Article/details/gwsqkgwbg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.yfazqb.com/Article/details/gzcaxgyba.sHtML

[U115] JS：生成 UUID
来源：http://wap.epnwcf.com/Article/details/gfruqfvbd.sHtML

crypto.randomUUID()
来源：http://m.share.fktsv.cn/Article/details/gvkcqqxiu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.yfazqb.com/Article/details/gbfceswqd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.yfazqb.com/Article/details/gedsiqdjv.sHtML

[U117] JS：单元测试
来源：http://3g.sjlbkw.cn/Article/details/gmbkxwtaq.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.bbcook.cn/Article/details/gvvqhcwkh.sHtML

[U118] JS：开发服务器
来源：http://mobile.epnwcf.com/Article/details/geezklqna.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fktsv.cn/Article/details/gwcqjrgcl.sHtML

[U119] JS：生产构建
来源：http://wap.fktsv.cn/Article/details/gypehuisw.sHtML

npx vite build
来源：http://read.share.vehdjk.com/Article/details/gawzrcmnx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.epnwcf.com/Article/details/gjdftzatr.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.vehdjk.com/Article/details/ghavgtqhw.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gfhwadbry.sHtML

统计汇总
来源：http://www.share.fktsv.cn/Article/details/gysnagqmp.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ghzqjjnpg.sHtML

按语言统计（条）：
来源：http://m.share.vehdjk.com/Article/details/gowlamyon.sHtML

Python ......... 252
来源：http://m.share.epnwcf.com/Article/details/gdmtxhovh.sHtML

PHP ............ 252
来源：http://www.share.tarul.cn/Article/details/gsgvxztbt.sHtML

JavaScript ..... 252
来源：http://wap.epnwcf.com/Article/details/gtkdlhtvi.sHtML

TypeScript ..... 212
来源：http://mobile.epnwcf.com/Article/details/gpbnyxufb.sHtML

Java ........... 212
来源：http://www.blog.bbcook.cn/Article/details/gsqkcqdzx.sHtML

Go ............. 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gejpwykbs.sHtML

Ruby ........... 212
来源：http://3g.vehdjk.com/Article/details/gujrvbcus.sHtML

C# ............. 212
来源：http://www.m.share.bbcook.cn/Article/details/gjleesadz.sHtML

C .............. 30
来源：http://3g.bbcook.cn/Article/details/guytbkftc.sHtML

C++ ............ 30
来源：http://3g.vehdjk.com/Article/details/gjteyzere.sHtML

SQL ............ 90
来源：http://wap.fktsv.cn/Article/details/gdgbugynf.sHtML

Bash ........... 80
来源：http://wap.bbcook.cn/Article/details/glpmrmfwb.sHtML

Kotlin ......... 15
来源：http://blog.sjlbkw.cn/Article/details/gkwvftzhc.sHtML

Swift .......... 15
来源：http://read.share.yfazqb.com/Article/details/gisasyzce.sHtML

Lua ............ 10
来源：http://www.share.tarul.cn/Article/details/gkchspgbf.sHtML

Perl ........... 10
来源：http://3g.yfazqb.com/Article/details/gckcbkbhv.sHtML

Scala .......... 10
来源：http://wap.sjlbkw.cn/Article/details/guotxpfqb.sHtML

------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gjozsywho.sHtML

合计 ........... 2106 条
来源：http://www.blog.bbcook.cn/Article/details/goizklxwu.sHtML

按章节统计：
来源：http://www.m.share.tarul.cn/Article/details/guefxwdiy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.epnwcf.com/Article/details/gdqqmeahq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.sjlbkw.cn/Article/details/gedhwsnxa.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fktsv.cn/Article/details/gjlirbvdm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.tarul.cn/Article/details/gufebsbhv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.vehdjk.com/Article/details/gvdwzkphe.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fktsv.cn/Article/details/gmlwppasl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/gosaequhz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.epnwcf.com/Article/details/gwnzfhqnz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gpczxllvh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fktsv.cn/Article/details/gvomoofha.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/glkwhrqpn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gwwcgdoza.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/goddpbiie.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.sjlbkw.cn/Article/details/gpofpnkov.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.yfazqb.com/Article/details/gnsuzznhd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/grkornakc.sHtML

Q SQL 专题                              90
来源：http://m.share.tarul.cn/Article/details/gfiihrjae.sHtML

R Bash 专题                             80
来源：http://m.share.yfazqb.com/Article/details/gghxmxwuo.sHtML

S C / C++ 专题                          60
来源：http://read.share.yfazqb.com/Article/details/gmetfuygq.sHtML

T 其他语言补充                          60
来源：http://mobile.epnwcf.com/Article/details/grvuqpwax.sHtML

U 高频实用片段                         120
来源：http://3g.vehdjk.com/Article/details/gkgfnwoan.sHtML

------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/gexoyqjqd.sHtML

合计                                  2106 条
来源：http://mobile.tarul.cn/Article/details/gihhxwdxo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.vehdjk.com/Article/details/gvrtwtxqd.sHtML

使用提醒
来源：http://read.share.vehdjk.com/Article/details/goscqkkhi.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gpmdeekvd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.tarul.cn/Article/details/gofdjbymi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.tarul.cn/Article/details/gbajfyawo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.sjlbkw.cn/Article/details/gneovesep.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.tarul.cn/Article/details/gaxzyvktw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.vehdjk.com/Article/details/gkxrclguh.sHtML

—— 文件结束 ——
来源：http://m.share.epnwcf.com/Article/details/gdgvqyjdk.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gqegnmpts.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.bbcook.cn/Article/details/gaqwfbbxg.sHtML

Common Programming Examples Cheat Book
来源：http://wap.epnwcf.com/Article/details/gdzhtostb.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/givnyebls.sHtML

【收录内容】
来源：http://3g.epnwcf.com/Article/details/gxfwjgowb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.vehdjk.com/Article/details/gpykkqdbq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.yfazqb.com/Article/details/gdqhzglrz.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.tarul.cn/Article/details/gqdkupaoz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.bbcook.cn/Article/details/gtoxqcoif.sHtML

【使用说明】
来源：http://blog.yfazqb.com/Article/details/gzxddqfyn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.vehdjk.com/Article/details/glcsvnixu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.epnwcf.com/Article/details/gtafcaxon.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fktsv.cn/Article/details/ggzihtynq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fktsv.cn/Article/details/gqcgztimz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.tarul.cn/Article/details/gzemfacik.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.yfazqb.com/Article/details/gzgflslvl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.epnwcf.com/Article/details/gtclhwpen.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.sjlbkw.cn/Article/details/gsvwaachq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.vehdjk.com/Article/details/gpxnvrwjt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.epnwcf.com/Article/details/gezpkxnkt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.yfazqb.com/Article/details/gehwnnbww.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.tarul.cn/Article/details/gbdzaeock.sHtML

【文件统计】
来源：http://www.m.share.yfazqb.com/Article/details/glfsrvjhv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.sjlbkw.cn/Article/details/gbhkqbvfq.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gzpjznoew.sHtML

目  录
来源：http://3g.bbcook.cn/Article/details/gmmopznmw.sHtML

--------------------------------------------------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gzlzxbozz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.sjlbkw.cn/Article/details/gzitmucll.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.epnwcf.com/Article/details/gqjjbiaqq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.bbcook.cn/Article/details/gyoxlbcxr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.yfazqb.com/Article/details/gpigyvslz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.epnwcf.com/Article/details/ggztxutup.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.tarul.cn/Article/details/gfbykgnjs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.epnwcf.com/Article/details/gcosbtmvf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.sjlbkw.cn/Article/details/gedmqbmii.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.vehdjk.com/Article/details/gzafseiwc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.epnwcf.com/Article/details/grslgrdma.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/guuyjogtf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gtkpcowcl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gurvgticz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.tarul.cn/Article/details/gvshnbavw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gcyfflped.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/gmbzzhfyt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.vehdjk.com/Article/details/gdgsjbfot.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fktsv.cn/Article/details/ganuzrjkm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fktsv.cn/Article/details/gbdsemxoc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/galhqiimp.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.vehdjk.com/Article/details/gnbbdxhta.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gycjtznzm.sHtML

A. 基础语法与类型
来源：http://www.m.share.tarul.cn/Article/details/ghottdqdp.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gnoossyzh.sHtML

[A01] Hello World
来源：http://3g.epnwcf.com/Article/details/gawzaugft.sHtML

Py:   print("Hello, World!")
来源：http://m.share.tarul.cn/Article/details/gvqvxzerd.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.vehdjk.com/Article/details/gbssxefxi.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.vehdjk.com/Article/details/gtffzmeyj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.vehdjk.com/Article/details/gsigbsomq.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.tarul.cn/Article/details/gunrjpnad.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.vehdjk.com/Article/details/gbmxfjuoa.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.sjlbkw.cn/Article/details/gotezccif.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fktsv.cn/Article/details/gowgmnfyf.sHtML

[A02] 变量声明与赋值
来源：http://www.share.tarul.cn/Article/details/gluqsfjpf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.sjlbkw.cn/Article/details/gidymflbi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.sjlbkw.cn/Article/details/gftjrdbvf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.epnwcf.com/Article/details/guutsnfod.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.tarul.cn/Article/details/gyanyymka.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.yfazqb.com/Article/details/gybiuddgw.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.yfazqb.com/Article/details/gauzukkpl.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fktsv.cn/Article/details/gdqnzkcep.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.vehdjk.com/Article/details/gfpllsejm.sHtML

[A03] 常量定义
来源：http://read.share.sjlbkw.cn/Article/details/goejlruqz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.bbcook.cn/Article/details/gygghwzvz.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/ggjxwnvqf.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/govlfkqdc.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.yfazqb.com/Article/details/gnqrpcpew.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gxxdqkeuk.sHtML

Go:   const PI = 3.14159
来源：http://read.share.vehdjk.com/Article/details/gognokitj.sHtML

Ruby: PI = 3.14159
来源：http://3g.sjlbkw.cn/Article/details/ghateinkr.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gvyjsevvm.sHtML

[A04] 判断变量类型
来源：http://wap.vehdjk.com/Article/details/gozkxugki.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fktsv.cn/Article/details/giplamafz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.sjlbkw.cn/Article/details/gaxoflypv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.epnwcf.com/Article/details/gkesvavmx.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.tarul.cn/Article/details/gqgpvnloy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.sjlbkw.cn/Article/details/gzndoysxa.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.yfazqb.com/Article/details/gbmbkjzyu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.epnwcf.com/Article/details/gdwghvxlf.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fktsv.cn/Article/details/goboanesc.sHtML

[A05] 整数除法与取模
来源：http://www.share.bbcook.cn/Article/details/gajycmolr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.yfazqb.com/Article/details/gtkumzieq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.vehdjk.com/Article/details/gvadnwaer.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.vehdjk.com/Article/details/gkeppgcmx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gwruwzjme.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/gtdshdity.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.tarul.cn/Article/details/gigeaejbf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.tarul.cn/Article/details/grfxycadj.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/gsbklnwuj.sHtML

[A06] 字符串转数字
来源：http://mobile.vehdjk.com/Article/details/gusgpacyt.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.sjlbkw.cn/Article/details/grrklrsge.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fktsv.cn/Article/details/gmyuwjtmq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.bbcook.cn/Article/details/ggvypyjfq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.sjlbkw.cn/Article/details/gnhpdyrjf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.bbcook.cn/Article/details/gvbveyaif.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.epnwcf.com/Article/details/geqeaodlr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.yfazqb.com/Article/details/gaizrgvqy.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.tarul.cn/Article/details/giayzudhj.sHtML

[A07] 数字转字符串
来源：http://mobile.tarul.cn/Article/details/gauamomvr.sHtML

Py:   str(42)
来源：http://m.share.sjlbkw.cn/Article/details/gpmrcludq.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.vehdjk.com/Article/details/gfndkuvzh.sHtML

JS:   String(42); (42).toString()
来源：http://wap.yfazqb.com/Article/details/gyhyuqsfb.sHtML

TS:   String(42)
来源：http://mobile.tarul.cn/Article/details/gbrafctcx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.tarul.cn/Article/details/guxovsmsc.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.sjlbkw.cn/Article/details/ghjfuejtq.sHtML

Ruby: 42.to_s
来源：http://3g.vehdjk.com/Article/details/gunknucng.sHtML

C#:   42.ToString()
来源：http://www.m.share.bbcook.cn/Article/details/gtaoopmba.sHtML

[A08] 取整与四舍五入
来源：http://wap.tarul.cn/Article/details/gtxfsxoii.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.vehdjk.com/Article/details/ggfgmjrdp.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.epnwcf.com/Article/details/gpofnsjhf.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/gqriznvcg.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.tarul.cn/Article/details/gpjmycngz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.yfazqb.com/Article/details/gdzgzefib.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.vehdjk.com/Article/details/gilsqodaj.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.tarul.cn/Article/details/gdpsqnoyl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.sjlbkw.cn/Article/details/glfgqeycl.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.yfazqb.com/Article/details/guwoqzlbh.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.epnwcf.com/Article/details/greumjrid.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.tarul.cn/Article/details/gbudfquhb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.epnwcf.com/Article/details/glugdfpzz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gxjhytgno.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.bbcook.cn/Article/details/ggwdhgngd.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.epnwcf.com/Article/details/grhcctfzd.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.tarul.cn/Article/details/gswrofrbt.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gmvaqxejn.sHtML

[A10] 生成随机数
来源：http://wap.bbcook.cn/Article/details/gdrkmyeat.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.yfazqb.com/Article/details/gcjixpsts.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.vehdjk.com/Article/details/gkwgcbcua.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.tarul.cn/Article/details/ghfteqyoa.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.bbcook.cn/Article/details/gdaqexign.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.fktsv.cn/Article/details/gajxqkszi.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.tarul.cn/Article/details/gdigzgjkd.sHtML

Ruby: rand(1..100)
来源：http://www.share.epnwcf.com/Article/details/gmsshnnki.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.yfazqb.com/Article/details/gtwkdsioo.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.yfazqb.com/Article/details/gpfwsrqiy.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.vehdjk.com/Article/details/gwhyajpcl.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.epnwcf.com/Article/details/guhrvlypy.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.sjlbkw.cn/Article/details/gacmudmnp.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.yfazqb.com/Article/details/givffkruy.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.sjlbkw.cn/Article/details/gkmoxglgu.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fktsv.cn/Article/details/gkzyoyqhf.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.sjlbkw.cn/Article/details/ghqsqqxpn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.sjlbkw.cn/Article/details/gnupeemfr.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.yfazqb.com/Article/details/glgbhjtud.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.yfazqb.com/Article/details/gzusqioew.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.fktsv.cn/Article/details/gruhtcnlo.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.epnwcf.com/Article/details/gobarhobc.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fktsv.cn/Article/details/gnylxzemg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.epnwcf.com/Article/details/givbndxih.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.tarul.cn/Article/details/gldnkofti.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.epnwcf.com/Article/details/glqgnrxcz.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.fktsv.cn/Article/details/gzgtuouua.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.sjlbkw.cn/Article/details/gzrehqtqp.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/ghgzojwxh.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gnmcrbmoj.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/gjxtejymh.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gpaqmhekb.sHtML

Java: "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/gmtwlbxwt.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/gklvbyafd.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/ghlmjhtdp.sHtML

C#:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gcjsyznwl.sHtML

[A14] 注释写法
来源：http://3g.epnwcf.com/Article/details/gnbyjhipd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.yfazqb.com/Article/details/grivhofiy.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/gdciankat.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.epnwcf.com/Article/details/ghrqawfch.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.sjlbkw.cn/Article/details/gjtzpvvth.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.bbcook.cn/Article/details/gbdumkbvk.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.yfazqb.com/Article/details/gqofmturd.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.epnwcf.com/Article/details/gqxknxtzc.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fktsv.cn/Article/details/gltuazndu.sHtML

[A15] 空值判断与默认值
来源：http://www.share.yfazqb.com/Article/details/guenkmofh.sHtML

Py:   value = data or "默认值"
来源：http://3g.tarul.cn/Article/details/gyefsehur.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.yfazqb.com/Article/details/gjguutokm.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.vehdjk.com/Article/details/gmrdbyhza.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fktsv.cn/Article/details/gqvsnfvqp.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.yfazqb.com/Article/details/gcskkzthj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.epnwcf.com/Article/details/gtwxgjomk.sHtML


<!-- 参考信息 -->