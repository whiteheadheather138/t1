代发 wailian999

[U87] JS：解构默认值
来源：http://wap.tarul.cn/Article/details/gzvywyyjk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.yfazqb.com/Article/details/gkkvyqbog.sHtML

[U88] JS：对象展开合并
来源：http://blog.tarul.cn/Article/details/gujwqfojx.sHtML

{ ...a, ...b }
来源：http://www.m.share.vehdjk.com/Article/details/gdlryxmzn.sHtML

[U89] JS：数组去重
来源：http://www.m.share.vehdjk.com/Article/details/glyilddtj.sHtML

[...new Set(arr)]
来源：http://www.m.share.vehdjk.com/Article/details/gjtzclwma.sHtML

[U90] JS：数字数组排序
来源：http://mobile.tarul.cn/Article/details/gafqxxmql.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.yfazqb.com/Article/details/gvzcajrws.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fktsv.cn/Article/details/ginsmlukc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fktsv.cn/Article/details/ggebfyimd.sHtML

[U92] JS：深拷贝
来源：http://wap.bbcook.cn/Article/details/gefabrkza.sHtML

structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gohocjovo.sHtML

[U93] JS：模板字符串
来源：http://3g.sjlbkw.cn/Article/details/gjdovocxx.sHtML

`共 ${n} 条`
来源：http://m.share.yfazqb.com/Article/details/glhyrvoyy.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.vehdjk.com/Article/details/gndrzshho.sHtML

const double = x => x * 2;
来源：http://mobile.vehdjk.com/Article/details/gxvvuxzyx.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.vehdjk.com/Article/details/gtgjoisno.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.vehdjk.com/Article/details/gzdqjeogu.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.bbcook.cn/Article/details/gkoifmtkh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gdkeygrcv.sHtML

[U97] JS：并发请求
来源：http://m.share.epnwcf.com/Article/details/gwtabajox.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/gnyxnwset.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.sjlbkw.cn/Article/details/gkppphowh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.tarul.cn/Article/details/giplbkmty.sHtML

[U99] JS：事件监听
来源：http://www.blog.sjlbkw.cn/Article/details/gdnmtkqxm.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fktsv.cn/Article/details/geyagqpea.sHtML

[U100] JS：DOM 查询
来源：http://mobile.yfazqb.com/Article/details/gedittrzw.sHtML

document.querySelector(".item")
来源：http://m.share.bbcook.cn/Article/details/gzitemcvp.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrzioccn.sHtML

el.classList.toggle("active")
来源：http://blog.epnwcf.com/Article/details/gcmyfczzo.sHtML

[U102] JS：本地存储
来源：http://3g.sjlbkw.cn/Article/details/gxxzspjxg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.sjlbkw.cn/Article/details/gnbegulri.sHtML

[U103] JS：定时器
来源：http://www.m.share.tarul.cn/Article/details/gmhuwqqnw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.tarul.cn/Article/details/gnqyuizib.sHtML

[U104] JS：防抖
来源：http://www.share.yfazqb.com/Article/details/gdszheeft.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.epnwcf.com/Article/details/gtdkvvapj.sHtML

[U105] JS：节流
来源：http://m.share.sjlbkw.cn/Article/details/gnnxmyxxy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.tarul.cn/Article/details/gpwfqqabc.sHtML

[U106] JS：日期格式化
来源：http://www.share.bbcook.cn/Article/details/gsajjfaui.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.bbcook.cn/Article/details/goxszaffe.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fktsv.cn/Article/details/gojfujnld.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.vehdjk.com/Article/details/ggmlhvmzc.sHtML

[U108] JS：随机整数
来源：http://3g.vehdjk.com/Article/details/gobldqjuq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.vehdjk.com/Article/details/gvnyadblw.sHtML

[U109] JS：数组分组
来源：http://m.share.vehdjk.com/Article/details/gbphfxcpj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.bbcook.cn/Article/details/glxybtoqt.sHtML

[U110] JS：数组分块
来源：http://mobile.vehdjk.com/Article/details/gacrvynkq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.vehdjk.com/Article/details/glaxywkhw.sHtML

[U111] JS：对象转 Map
来源：http://read.share.sjlbkw.cn/Article/details/gjqqucvel.sHtML

new Map(Object.entries(obj))
来源：http://read.share.sjlbkw.cn/Article/details/grcrvsogk.sHtML

[U112] JS：字符串补位
来源：http://wap.sjlbkw.cn/Article/details/gzwspqybd.sHtML

"7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gztgkmjui.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fktsv.cn/Article/details/gkymzakap.sHtML

s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gwwuaeakm.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.vehdjk.com/Article/details/gydzbuajn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.vehdjk.com/Article/details/gqspyqmzp.sHtML

[U115] JS：生成 UUID
来源：http://baike.sjlbkw.cn/Article/details/ghapffwlp.sHtML

crypto.randomUUID()
来源：http://read.share.fktsv.cn/Article/details/glsqwiqgr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.bbcook.cn/Article/details/gkkeulcpq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.epnwcf.com/Article/details/grjhanxko.sHtML

[U117] JS：单元测试
来源：http://www.blog.fktsv.cn/Article/details/gtdunhmwk.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.bbcook.cn/Article/details/ggrcbhrfh.sHtML

[U118] JS：开发服务器
来源：http://mobile.tarul.cn/Article/details/gxabzcwmx.sHtML

npm i -D vite;  npx vite
来源：http://www.share.epnwcf.com/Article/details/gyocdhfaf.sHtML

[U119] JS：生产构建
来源：http://mobile.epnwcf.com/Article/details/gecyhcofx.sHtML

npx vite build
来源：http://www.m.share.yfazqb.com/Article/details/gtcqmefga.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.bbcook.cn/Article/details/grsrhlnpu.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.yfazqb.com/Article/details/gkdplxzcd.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gjfvtlfvi.sHtML

统计汇总
来源：http://m.share.epnwcf.com/Article/details/grjjnhlhd.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gzoofnbpm.sHtML

按语言统计（条）：
来源：http://m.share.epnwcf.com/Article/details/gayupoqwh.sHtML

Python ......... 252
来源：http://www.share.yfazqb.com/Article/details/ggxmvepxk.sHtML

PHP ............ 252
来源：http://blog.tarul.cn/Article/details/gorrpyfol.sHtML

JavaScript ..... 252
来源：http://mobile.sjlbkw.cn/Article/details/gsbgvjkxt.sHtML

TypeScript ..... 212
来源：http://www.blog.tarul.cn/Article/details/gixijqvhh.sHtML

Java ........... 212
来源：http://www.blog.fktsv.cn/Article/details/gcxqqrugv.sHtML

Go ............. 212
来源：http://blog.bbcook.cn/Article/details/gykxznegv.sHtML

Ruby ........... 212
来源：http://wap.vehdjk.com/Article/details/gvxoeyzoy.sHtML

C# ............. 212
来源：http://read.share.tarul.cn/Article/details/gaeqqgzqu.sHtML

C .............. 30
来源：http://mobile.fktsv.cn/Article/details/gfrcupare.sHtML

C++ ............ 30
来源：http://3g.sjlbkw.cn/Article/details/ghopibtkz.sHtML

SQL ............ 90
来源：http://www.blog.epnwcf.com/Article/details/gwpsdnjtp.sHtML

Bash ........... 80
来源：http://www.blog.fktsv.cn/Article/details/giqtiicki.sHtML

Kotlin ......... 15
来源：http://www.m.share.tarul.cn/Article/details/gxqbdnrpx.sHtML

Swift .......... 15
来源：http://blog.sjlbkw.cn/Article/details/gfcijvuiw.sHtML

Lua ............ 10
来源：http://www.blog.sjlbkw.cn/Article/details/gakzctrsi.sHtML

Perl ........... 10
来源：http://wap.tarul.cn/Article/details/gwxythjnu.sHtML

Scala .......... 10
来源：http://wap.tarul.cn/Article/details/giuisazei.sHtML

------------------------------------
来源：http://m.share.tarul.cn/Article/details/gnlffpiue.sHtML

合计 ........... 2106 条
来源：http://3g.epnwcf.com/Article/details/gcijxvqcr.sHtML

按章节统计：
来源：http://mobile.yfazqb.com/Article/details/gbkgptgaw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.tarul.cn/Article/details/gvetyzaon.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fktsv.cn/Article/details/gzfpkpqql.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.yfazqb.com/Article/details/gxmrcmgpt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.yfazqb.com/Article/details/gurcltfga.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.bbcook.cn/Article/details/giedwrxyg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.vehdjk.com/Article/details/gvunyqvyi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.vehdjk.com/Article/details/gqdfrgjen.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.sjlbkw.cn/Article/details/ghwlfjzqs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/gictveymu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.epnwcf.com/Article/details/gmenudzeu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gzwddlqux.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/gydxwcumw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/grpvsldko.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.bbcook.cn/Article/details/guerlosrv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.sjlbkw.cn/Article/details/gwtqghlwm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gbozmxwzd.sHtML

Q SQL 专题                              90
来源：http://wap.vehdjk.com/Article/details/ghbyjnyng.sHtML

R Bash 专题                             80
来源：http://blog.epnwcf.com/Article/details/gmxkfufki.sHtML

S C / C++ 专题                          60
来源：http://wap.vehdjk.com/Article/details/gdpxtswhw.sHtML

T 其他语言补充                          60
来源：http://baike.fktsv.cn/Article/details/gkvtnsppn.sHtML

U 高频实用片段                         120
来源：http://m.share.sjlbkw.cn/Article/details/grdigbmnx.sHtML

------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gnzyxntis.sHtML

合计                                  2106 条
来源：http://www.share.fktsv.cn/Article/details/gxlbdhwuv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.vehdjk.com/Article/details/gptdmaiyi.sHtML

使用提醒
来源：http://www.blog.yfazqb.com/Article/details/gunwbaiuw.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gdzzrujrk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.vehdjk.com/Article/details/gbgvmdexa.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.sjlbkw.cn/Article/details/gjgdmgeey.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.sjlbkw.cn/Article/details/ggwdmeqed.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.tarul.cn/Article/details/gjvzpvkzf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.sjlbkw.cn/Article/details/gkblfonqt.sHtML

—— 文件结束 ——
来源：http://read.share.tarul.cn/Article/details/gutkccutc.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gxodzrpud.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.sjlbkw.cn/Article/details/ghglsbnuc.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fktsv.cn/Article/details/gncfdfior.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/grzuugzum.sHtML

【收录内容】
来源：http://m.share.epnwcf.com/Article/details/gkofgabsy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fktsv.cn/Article/details/ggmqrlmpf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.yfazqb.com/Article/details/gvwuawqjd.sHtML

SQL · Bash · C · C++
来源：http://baike.sjlbkw.cn/Article/details/gjgczfanz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.sjlbkw.cn/Article/details/gptwsggql.sHtML

【使用说明】
来源：http://mobile.sjlbkw.cn/Article/details/gdkxwxfcu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fktsv.cn/Article/details/groidzbfz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.sjlbkw.cn/Article/details/getdwgudf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.epnwcf.com/Article/details/ggdenbmve.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.yfazqb.com/Article/details/ghtgtvxrx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.tarul.cn/Article/details/gnqqygqnc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.bbcook.cn/Article/details/gligxpeuj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.bbcook.cn/Article/details/gknmkegky.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.bbcook.cn/Article/details/gicmzafle.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.tarul.cn/Article/details/gdkhjdweu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.tarul.cn/Article/details/glcbstphr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.tarul.cn/Article/details/ggdpprdhd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.tarul.cn/Article/details/glvmmktcm.sHtML

【文件统计】
来源：http://mobile.vehdjk.com/Article/details/gaxptuilh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.epnwcf.com/Article/details/grdeoahhb.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/gklaknfbd.sHtML

目  录
来源：http://3g.epnwcf.com/Article/details/gzydfrusm.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/glbupqjog.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.vehdjk.com/Article/details/gkkyxouje.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fktsv.cn/Article/details/gibcxrqye.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.bbcook.cn/Article/details/gjvicjezq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.vehdjk.com/Article/details/glfdrcjqk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.yfazqb.com/Article/details/gtojghfte.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.tarul.cn/Article/details/gmcjjedix.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.epnwcf.com/Article/details/gotcppdkb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.epnwcf.com/Article/details/gfjfoygnk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/gmluwnxvc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fktsv.cn/Article/details/ggpxrfudl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/gneyefurp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fktsv.cn/Article/details/gtafzcezu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/gbbptjjnt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.yfazqb.com/Article/details/gozzoqlkp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.tarul.cn/Article/details/gjrhtrgzb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.vehdjk.com/Article/details/gogacaacj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fktsv.cn/Article/details/ghkmqxzvv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fktsv.cn/Article/details/gmekuztqv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.epnwcf.com/Article/details/glqrcxdko.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fktsv.cn/Article/details/gjtukpxzu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.vehdjk.com/Article/details/gqpledgwf.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gnygoaryj.sHtML

A. 基础语法与类型
来源：http://read.share.bbcook.cn/Article/details/gyczugojo.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/glrtchuzz.sHtML

[A01] Hello World
来源：http://mobile.epnwcf.com/Article/details/gyaedvbvv.sHtML

Py:   print("Hello, World!")
来源：http://blog.bbcook.cn/Article/details/ghorcwwek.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.yfazqb.com/Article/details/gcqjjprgb.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.sjlbkw.cn/Article/details/gohqcrkcx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.sjlbkw.cn/Article/details/giqxblhru.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.sjlbkw.cn/Article/details/gbkyixflt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fktsv.cn/Article/details/gvfewizvc.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fktsv.cn/Article/details/gdprfgada.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.tarul.cn/Article/details/gzpevrwqh.sHtML

[A02] 变量声明与赋值
来源：http://baike.tarul.cn/Article/details/gddedqgim.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.tarul.cn/Article/details/grsaxauns.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.tarul.cn/Article/details/gseqgxhjr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.tarul.cn/Article/details/gycrplzjf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.yfazqb.com/Article/details/gofyhonei.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.vehdjk.com/Article/details/gfuigkgpb.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.tarul.cn/Article/details/gjmbryiug.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fktsv.cn/Article/details/gdzngyioj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fktsv.cn/Article/details/gkdgdemdm.sHtML

[A03] 常量定义
来源：http://baike.fktsv.cn/Article/details/gleiezfuu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.yfazqb.com/Article/details/gjkxyjsfl.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/ggnxplleo.sHtML

JS:   const PI = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gxryrusyy.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gnhvhoflu.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gkgxfnbpy.sHtML

Go:   const PI = 3.14159
来源：http://read.share.yfazqb.com/Article/details/gomuqtbko.sHtML

Ruby: PI = 3.14159
来源：http://www.share.yfazqb.com/Article/details/grhzrhuot.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gbbyhqzip.sHtML

[A04] 判断变量类型
来源：http://read.share.epnwcf.com/Article/details/gkkayotrz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.yfazqb.com/Article/details/gqkmpxtgm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.yfazqb.com/Article/details/gwkstidzm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fktsv.cn/Article/details/gspzfxwgn.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.vehdjk.com/Article/details/gmkqtptwm.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.sjlbkw.cn/Article/details/gytazntxv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.tarul.cn/Article/details/gnaznvffi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.sjlbkw.cn/Article/details/gmwgauwrc.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.epnwcf.com/Article/details/gzabkmmin.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fktsv.cn/Article/details/gjfcptgyl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.tarul.cn/Article/details/gwtyatepb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.vehdjk.com/Article/details/gsybmsimd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.yfazqb.com/Article/details/grcksinjy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.tarul.cn/Article/details/groxvycpn.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/gsnwffvra.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.bbcook.cn/Article/details/gecuxdzwc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.vehdjk.com/Article/details/gfgkmjnqw.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fktsv.cn/Article/details/gaiecwhdp.sHtML

[A06] 字符串转数字
来源：http://blog.yfazqb.com/Article/details/gkdnkvayg.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.vehdjk.com/Article/details/gzfgpgeqh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.yfazqb.com/Article/details/gqqgybzhn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.yfazqb.com/Article/details/gfphzjead.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.yfazqb.com/Article/details/glxtsdgef.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.yfazqb.com/Article/details/gwkctutbp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fktsv.cn/Article/details/gvmrrpcqf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.fktsv.cn/Article/details/ggjswtxco.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.yfazqb.com/Article/details/gjyewcdss.sHtML

[A07] 数字转字符串
来源：http://read.share.bbcook.cn/Article/details/gqnezkevc.sHtML

Py:   str(42)
来源：http://3g.yfazqb.com/Article/details/gftvepztt.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.sjlbkw.cn/Article/details/gdxlegdfu.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.epnwcf.com/Article/details/ghhfbowpg.sHtML

TS:   String(42)
来源：http://read.share.bbcook.cn/Article/details/gywosuhiz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fktsv.cn/Article/details/gtmdiaahs.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.vehdjk.com/Article/details/gfncntqxa.sHtML

Ruby: 42.to_s
来源：http://wap.epnwcf.com/Article/details/gxijigtwi.sHtML

C#:   42.ToString()
来源：http://baike.epnwcf.com/Article/details/gyeavpwyt.sHtML

[A08] 取整与四舍五入
来源：http://baike.vehdjk.com/Article/details/gnvxoywme.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.bbcook.cn/Article/details/gcwzqndjn.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.sjlbkw.cn/Article/details/gmexgcfsv.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fktsv.cn/Article/details/gnyvpqbuj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.tarul.cn/Article/details/gapnwibqy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.bbcook.cn/Article/details/gmjgaytiv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.tarul.cn/Article/details/gomhycxsz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.vehdjk.com/Article/details/giigonqok.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fktsv.cn/Article/details/glyrgceor.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.yfazqb.com/Article/details/gklvetean.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/ghkveeneo.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fktsv.cn/Article/details/gopalmtfk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gzczceedm.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gmmslxsfg.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/gckyuiena.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.epnwcf.com/Article/details/gkemulvws.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fktsv.cn/Article/details/glmbzolls.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.epnwcf.com/Article/details/gkbaktivi.sHtML

[A10] 生成随机数
来源：http://read.share.bbcook.cn/Article/details/gfhllxtbm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.bbcook.cn/Article/details/gobwnijqz.sHtML

PHP:  random_int(1, 100);
来源：http://blog.yfazqb.com/Article/details/gonqcaofb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.epnwcf.com/Article/details/gjdvsjizn.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.tarul.cn/Article/details/gzyhxfsiw.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.vehdjk.com/Article/details/gkfhcifnn.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.bbcook.cn/Article/details/gapknkqnm.sHtML

Ruby: rand(1..100)
来源：http://3g.yfazqb.com/Article/details/gzijfhnwi.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.epnwcf.com/Article/details/gpvhesmoj.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.epnwcf.com/Article/details/goerxuhie.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.sjlbkw.cn/Article/details/gfkxrfrrn.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.sjlbkw.cn/Article/details/goqnnuwgb.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.sjlbkw.cn/Article/details/gcpcmqabx.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.bbcook.cn/Article/details/gmzyjjcjw.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.epnwcf.com/Article/details/glrdhbcrx.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpczwmnw.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.tarul.cn/Article/details/gcifjluis.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.tarul.cn/Article/details/gnhdjihfi.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.epnwcf.com/Article/details/gpshuabpq.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.vehdjk.com/Article/details/ghjponqls.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.tarul.cn/Article/details/gmaxojafw.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.sjlbkw.cn/Article/details/gipvcwwoa.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.vehdjk.com/Article/details/grprjogly.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.sjlbkw.cn/Article/details/gxwibnfzt.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.sjlbkw.cn/Article/details/ggeaxywec.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.vehdjk.com/Article/details/gaohdusvq.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.tarul.cn/Article/details/gvlwfbdte.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.fktsv.cn/Article/details/gipshshxm.sHtML

Py:   "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/gfqfbrtkq.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/gltjswxzx.sHtML

JS:   "第一行\n第二行"
来源：http://blog.epnwcf.com/Article/details/guknuoyvw.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gavwssqxt.sHtML

Java: "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/gkgemzdtv.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/gopaeqyqg.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/gijsrymtq.sHtML

C#:   "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/gfouztyog.sHtML

[A14] 注释写法
来源：http://3g.yfazqb.com/Article/details/gdfewgwka.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.epnwcf.com/Article/details/gvtjefcsh.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.epnwcf.com/Article/details/gqxrntdnd.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.yfazqb.com/Article/details/gxjsktfbd.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.yfazqb.com/Article/details/gdezabzix.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.vehdjk.com/Article/details/gnkmaxvnf.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.fktsv.cn/Article/details/gyrembqug.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.yfazqb.com/Article/details/gahcquzzc.sHtML


<!-- 参考信息 -->