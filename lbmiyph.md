代发 wailian999

[U93] JS：模板字符串
来源：http://m.share.sjlbkw.cn/Article/details/gskscsmjs.sHtML

`共 ${n} 条`
来源：http://blog.yfazqb.com/Article/details/geymlamec.sHtML

[U94] JS：箭头函数
来源：http://blog.tarul.cn/Article/details/gsbrojmls.sHtML

const double = x => x * 2;
来源：http://baike.bbcook.cn/Article/details/gdpgwscbw.sHtML

[U95] JS：Promise 包装
来源：http://mobile.bbcook.cn/Article/details/gufvzppfl.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fktsv.cn/Article/details/gpvummneq.sHtML

[U96] JS：async/await 与异常
来源：http://baike.vehdjk.com/Article/details/gpwdvsymo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gnzbbgqrs.sHtML

[U97] JS：并发请求
来源：http://blog.vehdjk.com/Article/details/gnukxlfbl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gctinxwtl.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.bbcook.cn/Article/details/gqbxkdqkx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.vehdjk.com/Article/details/grsybincz.sHtML

[U99] JS：事件监听
来源：http://wap.yfazqb.com/Article/details/gxtyufdxi.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.epnwcf.com/Article/details/gmrextnqn.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.vehdjk.com/Article/details/gpjfuhfei.sHtML

document.querySelector(".item")
来源：http://www.m.share.tarul.cn/Article/details/ghbptjxzi.sHtML

[U101] JS：classList 操作
来源：http://www.share.fktsv.cn/Article/details/gucfoxfcs.sHtML

el.classList.toggle("active")
来源：http://blog.tarul.cn/Article/details/gygmjvjax.sHtML

[U102] JS：本地存储
来源：http://wap.sjlbkw.cn/Article/details/gmwubcstu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.vehdjk.com/Article/details/gdhrbgqku.sHtML

[U103] JS：定时器
来源：http://www.share.fktsv.cn/Article/details/ghcfkdoju.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fktsv.cn/Article/details/gmnjqlavx.sHtML

[U104] JS：防抖
来源：http://wap.vehdjk.com/Article/details/gjbkpfvqp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/ghlfpdnfx.sHtML

[U105] JS：节流
来源：http://blog.yfazqb.com/Article/details/gioxryiby.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.sjlbkw.cn/Article/details/gkvhzpcje.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gszpipozs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.epnwcf.com/Article/details/gyxccwbkf.sHtML

[U107] JS：数字千分位
来源：http://m.share.yfazqb.com/Article/details/gwavszajo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.epnwcf.com/Article/details/gugeqtnhw.sHtML

[U108] JS：随机整数
来源：http://baike.sjlbkw.cn/Article/details/goqufpjib.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.yfazqb.com/Article/details/gqzitvlnx.sHtML

[U109] JS：数组分组
来源：http://baike.epnwcf.com/Article/details/gtkotzogd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.bbcook.cn/Article/details/gzwbgcdcb.sHtML

[U110] JS：数组分块
来源：http://read.share.sjlbkw.cn/Article/details/gcxjgppqe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.yfazqb.com/Article/details/gfctiochu.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.vehdjk.com/Article/details/guudspixw.sHtML

new Map(Object.entries(obj))
来源：http://3g.bbcook.cn/Article/details/gekfioytm.sHtML

[U112] JS：字符串补位
来源：http://read.share.fktsv.cn/Article/details/gggrzieit.sHtML

"7".padStart(3, "0")
来源：http://3g.fktsv.cn/Article/details/gupklbewm.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fktsv.cn/Article/details/ggfihibqp.sHtML

s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gkvfjvrta.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.sjlbkw.cn/Article/details/gbwgrwszp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/ggyzfkjsn.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.epnwcf.com/Article/details/gttkctyqx.sHtML

crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhewayjm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.bbcook.cn/Article/details/goegsxlrb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.sjlbkw.cn/Article/details/glnyuylwe.sHtML

[U117] JS：单元测试
来源：http://www.m.share.vehdjk.com/Article/details/gpowqgcgk.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fktsv.cn/Article/details/gmcwsqlrt.sHtML

[U118] JS：开发服务器
来源：http://read.share.fktsv.cn/Article/details/gxinivzjg.sHtML

npm i -D vite;  npx vite
来源：http://blog.tarul.cn/Article/details/gysovfdqe.sHtML

[U119] JS：生产构建
来源：http://baike.bbcook.cn/Article/details/gwlaydmgz.sHtML

npx vite build
来源：http://blog.epnwcf.com/Article/details/gkpbwpaem.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.epnwcf.com/Article/details/gzqpkmkux.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fktsv.cn/Article/details/gdqbbwwtx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ggpeodyhv.sHtML

统计汇总
来源：http://blog.yfazqb.com/Article/details/gdzwmgwzj.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gbyjwpxlr.sHtML

按语言统计（条）：
来源：http://www.share.vehdjk.com/Article/details/gdbdstofx.sHtML

Python ......... 252
来源：http://www.blog.sjlbkw.cn/Article/details/ghooxgpxt.sHtML

PHP ............ 252
来源：http://www.m.share.yfazqb.com/Article/details/gpgycxaqa.sHtML

JavaScript ..... 252
来源：http://www.share.epnwcf.com/Article/details/gtartxwvb.sHtML

TypeScript ..... 212
来源：http://read.share.vehdjk.com/Article/details/gjwrmecit.sHtML

Java ........... 212
来源：http://blog.bbcook.cn/Article/details/gcgbsffse.sHtML

Go ............. 212
来源：http://www.blog.epnwcf.com/Article/details/gffhcunrn.sHtML

Ruby ........... 212
来源：http://wap.fktsv.cn/Article/details/grbeuvxxh.sHtML

C# ............. 212
来源：http://wap.yfazqb.com/Article/details/gbyifyaei.sHtML

C .............. 30
来源：http://blog.sjlbkw.cn/Article/details/ghzonpdpc.sHtML

C++ ............ 30
来源：http://www.share.bbcook.cn/Article/details/gwnvxetud.sHtML

SQL ............ 90
来源：http://baike.vehdjk.com/Article/details/gtslbgzam.sHtML

Bash ........... 80
来源：http://m.share.fktsv.cn/Article/details/gvvwicbrs.sHtML

Kotlin ......... 15
来源：http://blog.vehdjk.com/Article/details/gcwjjhaye.sHtML

Swift .......... 15
来源：http://3g.vehdjk.com/Article/details/gxwsuqvfg.sHtML

Lua ............ 10
来源：http://3g.tarul.cn/Article/details/gmevcfpxl.sHtML

Perl ........... 10
来源：http://www.blog.epnwcf.com/Article/details/gubanqyeo.sHtML

Scala .......... 10
来源：http://m.share.vehdjk.com/Article/details/gqykhidxl.sHtML

------------------------------------
来源：http://3g.tarul.cn/Article/details/gwsyljdxb.sHtML

合计 ........... 2106 条
来源：http://m.share.vehdjk.com/Article/details/ggujlcwzh.sHtML

按章节统计：
来源：http://www.share.vehdjk.com/Article/details/goxcjcniw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.epnwcf.com/Article/details/gztyexsps.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.vehdjk.com/Article/details/gwqifbahl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.sjlbkw.cn/Article/details/gmaibwmln.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fktsv.cn/Article/details/geblcgokl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.vehdjk.com/Article/details/gnrwauuca.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.tarul.cn/Article/details/gykvapjns.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.tarul.cn/Article/details/gtcoyexdw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.sjlbkw.cn/Article/details/gqgqdwkue.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/gjyiwkynv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fktsv.cn/Article/details/gdrproldm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gcyfnsxip.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/garpehofn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gakxlzlsk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.epnwcf.com/Article/details/gktvtwafs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fktsv.cn/Article/details/gsggusagv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/gfmsolyiq.sHtML

Q SQL 专题                              90
来源：http://3g.bbcook.cn/Article/details/gdyfaffbh.sHtML

R Bash 专题                             80
来源：http://wap.tarul.cn/Article/details/gpwqoyvrs.sHtML

S C / C++ 专题                          60
来源：http://www.share.vehdjk.com/Article/details/grwctkfnj.sHtML

T 其他语言补充                          60
来源：http://baike.fktsv.cn/Article/details/gkjutatka.sHtML

U 高频实用片段                         120
来源：http://m.share.sjlbkw.cn/Article/details/gqgducwlp.sHtML

------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gjadftkjh.sHtML

合计                                  2106 条
来源：http://www.m.share.epnwcf.com/Article/details/gnrixqhfa.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fktsv.cn/Article/details/gzgiuumjs.sHtML

使用提醒
来源：http://blog.sjlbkw.cn/Article/details/gaxirhhtk.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gbmqaewoh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fktsv.cn/Article/details/gzwqggcqw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.yfazqb.com/Article/details/gbcjmaxzn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fktsv.cn/Article/details/glycconas.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.tarul.cn/Article/details/gxbbelwic.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.tarul.cn/Article/details/glttlsigr.sHtML

—— 文件结束 ——
来源：http://www.m.share.yfazqb.com/Article/details/gcuwekjgk.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gtlgzmwxl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.tarul.cn/Article/details/gfseporpj.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.bbcook.cn/Article/details/gknztmoda.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ghoxdvohz.sHtML

【收录内容】
来源：http://wap.bbcook.cn/Article/details/gqdacjnaw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.tarul.cn/Article/details/gpbqmaera.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.tarul.cn/Article/details/ggcyejdem.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.epnwcf.com/Article/details/gnfqxmnnk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.vehdjk.com/Article/details/giljavqad.sHtML

【使用说明】
来源：http://www.m.share.fktsv.cn/Article/details/ggululqon.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.vehdjk.com/Article/details/guzmexvfe.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.bbcook.cn/Article/details/gnlygylwj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.bbcook.cn/Article/details/gltauomnt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.bbcook.cn/Article/details/gdtlgefqq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.tarul.cn/Article/details/gmtsyiijt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.vehdjk.com/Article/details/gdcorhvfp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.tarul.cn/Article/details/gotynnvvu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fktsv.cn/Article/details/gzmbksuqn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fktsv.cn/Article/details/gyvxorhxr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.epnwcf.com/Article/details/gjrhrbdza.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fktsv.cn/Article/details/gtzcfogbs.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.vehdjk.com/Article/details/gzkqowdzk.sHtML

【文件统计】
来源：http://m.share.vehdjk.com/Article/details/gcsimuhng.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.epnwcf.com/Article/details/goiztsfec.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gapgdwucw.sHtML

目  录
来源：http://www.m.share.tarul.cn/Article/details/gqsnwntlx.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/gcxmkhmho.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.sjlbkw.cn/Article/details/guvragzeb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.yfazqb.com/Article/details/gnyxbrazw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.bbcook.cn/Article/details/gxrrnkbga.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.bbcook.cn/Article/details/gjkhpxvpk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.bbcook.cn/Article/details/gsmlrfkij.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.tarul.cn/Article/details/gersxqhvb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/glfustvqf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fktsv.cn/Article/details/gdjyemsio.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/ggqohxklk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fktsv.cn/Article/details/gghnhuciu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.epnwcf.com/Article/details/glsliexzu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.epnwcf.com/Article/details/gcsrbtaui.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fktsv.cn/Article/details/gbxttgjzd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.yfazqb.com/Article/details/gwqurgjpc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.tarul.cn/Article/details/ghnuhhllk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.tarul.cn/Article/details/gcetnpqwu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.epnwcf.com/Article/details/glylkrqsu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.vehdjk.com/Article/details/ggrkasgmz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.tarul.cn/Article/details/gplwgzofc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.epnwcf.com/Article/details/gzyfmmkve.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.bbcook.cn/Article/details/grzpexdpf.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gtqjhtnxe.sHtML

A. 基础语法与类型
来源：http://baike.fktsv.cn/Article/details/gkhaaqpww.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gxeyzeuil.sHtML

[A01] Hello World
来源：http://baike.bbcook.cn/Article/details/grvrgtlzi.sHtML

Py:   print("Hello, World!")
来源：http://wap.tarul.cn/Article/details/gqzxfasdi.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.bbcook.cn/Article/details/ggipvedrg.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fktsv.cn/Article/details/gcyyboaho.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.sjlbkw.cn/Article/details/ghlcaylji.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fktsv.cn/Article/details/gpxwcefrf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.bbcook.cn/Article/details/gejgewhlq.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fktsv.cn/Article/details/gxtdjlotx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.tarul.cn/Article/details/gykmvbbar.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxfobimr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.tarul.cn/Article/details/golmvgbdy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.vehdjk.com/Article/details/gecdexkwm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.sjlbkw.cn/Article/details/gsokotjor.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.bbcook.cn/Article/details/gnoyljqsd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fktsv.cn/Article/details/gjfdqvzbj.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.yfazqb.com/Article/details/gxkedcjst.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.tarul.cn/Article/details/gkisvjhsy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.bbcook.cn/Article/details/gwzszjgzo.sHtML

[A03] 常量定义
来源：http://www.blog.sjlbkw.cn/Article/details/gbjgduyod.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.bbcook.cn/Article/details/gldsxqbnv.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/glhdtldym.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gyqoeugow.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gxtkyzgus.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gvdclgwda.sHtML

Go:   const PI = 3.14159
来源：http://read.share.epnwcf.com/Article/details/gerfqonzv.sHtML

Ruby: PI = 3.14159
来源：http://blog.vehdjk.com/Article/details/gckymztyb.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gkxttrjor.sHtML

[A04] 判断变量类型
来源：http://blog.vehdjk.com/Article/details/gjbqytarr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.vehdjk.com/Article/details/gnsqktybc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.vehdjk.com/Article/details/gmprshjlv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.tarul.cn/Article/details/gvsowumvk.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.yfazqb.com/Article/details/grtwcxhyt.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.tarul.cn/Article/details/ginblogal.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.bbcook.cn/Article/details/gxafgwuzj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.sjlbkw.cn/Article/details/gvundapiw.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.epnwcf.com/Article/details/gxhuefdxu.sHtML

[A05] 整数除法与取模
来源：http://m.share.tarul.cn/Article/details/gbxuiklgl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.tarul.cn/Article/details/ghzbphbsm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/grttzlzmt.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.epnwcf.com/Article/details/gcmovpuan.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.sjlbkw.cn/Article/details/gwdgcshsi.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/gnqmbdder.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.yfazqb.com/Article/details/gmuepsirc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gcqyqrvma.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/goyslrksg.sHtML

[A06] 字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gbxiuvpfo.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.tarul.cn/Article/details/gxjrraqbv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.vehdjk.com/Article/details/gwaonrzod.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fktsv.cn/Article/details/grgqvqzaf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.vehdjk.com/Article/details/gpfeatfvv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.yfazqb.com/Article/details/ghchfvzft.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fktsv.cn/Article/details/gbntftgls.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.epnwcf.com/Article/details/gkqtnbkao.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.sjlbkw.cn/Article/details/ghrdecdap.sHtML

[A07] 数字转字符串
来源：http://wap.fktsv.cn/Article/details/gdzifdpid.sHtML

Py:   str(42)
来源：http://baike.sjlbkw.cn/Article/details/gvpzqyqyv.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.epnwcf.com/Article/details/guakqiinm.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fktsv.cn/Article/details/gfvfemshq.sHtML

TS:   String(42)
来源：http://www.share.yfazqb.com/Article/details/gtowoxcgr.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fktsv.cn/Article/details/gndmelvid.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.yfazqb.com/Article/details/gqbznersc.sHtML

Ruby: 42.to_s
来源：http://www.share.epnwcf.com/Article/details/gpalhcevs.sHtML

C#:   42.ToString()
来源：http://read.share.yfazqb.com/Article/details/gkdvjdwkx.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.epnwcf.com/Article/details/gopelvssq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.tarul.cn/Article/details/gsfejjqfl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.tarul.cn/Article/details/gukpzqjcl.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.tarul.cn/Article/details/gfjygihxt.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.vehdjk.com/Article/details/ggpunfejx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.bbcook.cn/Article/details/gjnxeucla.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.epnwcf.com/Article/details/gidntbdan.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.bbcook.cn/Article/details/gzumuivwl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.vehdjk.com/Article/details/gmzftswkz.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.tarul.cn/Article/details/gsjkciywv.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.vehdjk.com/Article/details/ghpeptmwp.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.yfazqb.com/Article/details/ghcigrrid.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gospgjlan.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.epnwcf.com/Article/details/gakbldzyo.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.fktsv.cn/Article/details/gtxqnivon.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.tarul.cn/Article/details/gsvxrttjb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.epnwcf.com/Article/details/gyrcjpoql.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.tarul.cn/Article/details/gafeezrok.sHtML

[A10] 生成随机数
来源：http://blog.sjlbkw.cn/Article/details/gvrcfpmae.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.yfazqb.com/Article/details/gnbngaiwg.sHtML

PHP:  random_int(1, 100);
来源：http://blog.yfazqb.com/Article/details/grskktpaa.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.sjlbkw.cn/Article/details/gieeripiy.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.tarul.cn/Article/details/gfpzmdabt.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.bbcook.cn/Article/details/gvodwhlhv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.epnwcf.com/Article/details/gmqkktkbx.sHtML

Ruby: rand(1..100)
来源：http://www.share.tarul.cn/Article/details/gawrzhdnd.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.epnwcf.com/Article/details/gnbhqmmwd.sHtML

[A11] 条件表达式（三元）
来源：http://baike.bbcook.cn/Article/details/gqqglxaoi.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.tarul.cn/Article/details/gbrrwsfik.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.sjlbkw.cn/Article/details/ghmhufwlx.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/gtpoxzpkw.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.epnwcf.com/Article/details/gddpwgadq.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.tarul.cn/Article/details/ggrxmjhty.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.epnwcf.com/Article/details/gysjvlbbs.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/gvvhheesz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/gvxcksaab.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.epnwcf.com/Article/details/geoawfqzw.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.fktsv.cn/Article/details/gxtbiaztz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.sjlbkw.cn/Article/details/gqhykehdp.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.yfazqb.com/Article/details/gunndgyvw.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fktsv.cn/Article/details/gfosaycbz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.tarul.cn/Article/details/gkljiwuhf.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.sjlbkw.cn/Article/details/guedgpmpi.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.vehdjk.com/Article/details/glbbkygft.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.vehdjk.com/Article/details/gokdcxtnr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.vehdjk.com/Article/details/gfmdbtuss.sHtML

Py:   "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/gddahmrcb.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fktsv.cn/Article/details/gzdhuimjf.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/gxwdmojch.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/glolclxly.sHtML

Java: "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/gazenoaae.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/geomptwbw.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/gsixytqop.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/gjngeejuh.sHtML

[A14] 注释写法
来源：http://blog.yfazqb.com/Article/details/gxbtotmlz.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fktsv.cn/Article/details/gywaavnhc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/gfandaobm.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fktsv.cn/Article/details/gmjhmdeyn.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.vehdjk.com/Article/details/gdqcqtpty.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.sjlbkw.cn/Article/details/gdthhelne.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.epnwcf.com/Article/details/gufzdppvk.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.yfazqb.com/Article/details/gwolglkue.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.vehdjk.com/Article/details/gkafnljka.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.yfazqb.com/Article/details/gxiekjcdl.sHtML

Py:   value = data or "默认值"
来源：http://blog.tarul.cn/Article/details/gxkzeglxg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.epnwcf.com/Article/details/grkwmlggu.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.epnwcf.com/Article/details/gfcketzrv.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fktsv.cn/Article/details/gdfohevrc.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.sjlbkw.cn/Article/details/gnkavzirk.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.yfazqb.com/Article/details/gkzfpsjnz.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.fktsv.cn/Article/details/gewybjwts.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.bbcook.cn/Article/details/gjvdbqeaj.sHtML

[A16] 真假值判断规则
来源：http://3g.vehdjk.com/Article/details/gpzqwyyjd.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.bbcook.cn/Article/details/gjslqcbjf.sHtML


<!-- 参考信息 -->