代发 wailian999

[U85] JS：可选链
来源：http://read.share.yfazqb.com/Article/details/ggcpdqmhv.sHtML

a?.b?.c
来源：http://mobile.fktsv.cn/Article/details/gohfkxdvk.sHtML

[U86] JS：空值合并
来源：http://read.share.fktsv.cn/Article/details/grbmvrgvq.sHtML

a ?? b
来源：http://www.m.share.bbcook.cn/Article/details/gvctxcwtj.sHtML

[U87] JS：解构默认值
来源：http://m.share.fktsv.cn/Article/details/grlchkzhs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fktsv.cn/Article/details/gcwlbgiat.sHtML

[U88] JS：对象展开合并
来源：http://blog.sjlbkw.cn/Article/details/gtyvclzxu.sHtML

{ ...a, ...b }
来源：http://3g.yfazqb.com/Article/details/gitmzcqxj.sHtML

[U89] JS：数组去重
来源：http://read.share.epnwcf.com/Article/details/ggwnrcaio.sHtML

[...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/grhvmbixs.sHtML

[U90] JS：数字数组排序
来源：http://wap.epnwcf.com/Article/details/gppaqpteg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gfghqvyxm.sHtML

[U91] JS：对象键值遍历
来源：http://blog.sjlbkw.cn/Article/details/greoezeku.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.sjlbkw.cn/Article/details/gbqlubhdr.sHtML

[U92] JS：深拷贝
来源：http://www.blog.epnwcf.com/Article/details/gggesfawo.sHtML

structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gfambuurj.sHtML

[U93] JS：模板字符串
来源：http://read.share.sjlbkw.cn/Article/details/gfipquieh.sHtML

`共 ${n} 条`
来源：http://mobile.tarul.cn/Article/details/gugtzasfc.sHtML

[U94] JS：箭头函数
来源：http://wap.tarul.cn/Article/details/gdlrsdfbv.sHtML

const double = x => x * 2;
来源：http://read.share.epnwcf.com/Article/details/gsrxhttbm.sHtML

[U95] JS：Promise 包装
来源：http://baike.vehdjk.com/Article/details/gjqeotmsc.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.tarul.cn/Article/details/glsjkjkgr.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.bbcook.cn/Article/details/gfjqlnpwy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gbknrbwyv.sHtML

[U97] JS：并发请求
来源：http://www.share.bbcook.cn/Article/details/godprqtiz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gzarpazkj.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.bbcook.cn/Article/details/ginxynzqs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.bbcook.cn/Article/details/gprnijoia.sHtML

[U99] JS：事件监听
来源：http://baike.sjlbkw.cn/Article/details/gukibdsnz.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.sjlbkw.cn/Article/details/gdizzxqag.sHtML

[U100] JS：DOM 查询
来源：http://wap.yfazqb.com/Article/details/glyqbrbfd.sHtML

document.querySelector(".item")
来源：http://www.blog.yfazqb.com/Article/details/gpxgnrghd.sHtML

[U101] JS：classList 操作
来源：http://mobile.fktsv.cn/Article/details/gyquvzrbl.sHtML

el.classList.toggle("active")
来源：http://m.share.epnwcf.com/Article/details/gzyuanssg.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fktsv.cn/Article/details/gjdregzdk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.sjlbkw.cn/Article/details/gxzlkqoki.sHtML

[U103] JS：定时器
来源：http://www.blog.vehdjk.com/Article/details/gmxwuvlaw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.epnwcf.com/Article/details/gdkcslrjz.sHtML

[U104] JS：防抖
来源：http://baike.bbcook.cn/Article/details/gkuryxtnu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/glhkszcie.sHtML

[U105] JS：节流
来源：http://blog.tarul.cn/Article/details/goxhmzwkm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.yfazqb.com/Article/details/gtmojoxkw.sHtML

[U106] JS：日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/gkdztrtdl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.vehdjk.com/Article/details/gxazlnwsu.sHtML

[U107] JS：数字千分位
来源：http://wap.fktsv.cn/Article/details/gapakwtqw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.bbcook.cn/Article/details/gjrctnxkd.sHtML

[U108] JS：随机整数
来源：http://3g.epnwcf.com/Article/details/gjulhmxhf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fktsv.cn/Article/details/grpkqdwtl.sHtML

[U109] JS：数组分组
来源：http://mobile.epnwcf.com/Article/details/gowrtemxb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.sjlbkw.cn/Article/details/gnoldfymq.sHtML

[U110] JS：数组分块
来源：http://www.blog.fktsv.cn/Article/details/gzfksrmee.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.epnwcf.com/Article/details/gyczspbyt.sHtML

[U111] JS：对象转 Map
来源：http://wap.bbcook.cn/Article/details/gcukakwvm.sHtML

new Map(Object.entries(obj))
来源：http://www.share.vehdjk.com/Article/details/gdnlejeyv.sHtML

[U112] JS：字符串补位
来源：http://mobile.epnwcf.com/Article/details/grvxohuzv.sHtML

"7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gonicgaln.sHtML

[U113] JS：正则替换全部
来源：http://blog.tarul.cn/Article/details/gbcxtcush.sHtML

s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gzvldlmua.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.vehdjk.com/Article/details/golwqwehe.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.bbcook.cn/Article/details/gcgbffiue.sHtML

[U115] JS：生成 UUID
来源：http://baike.sjlbkw.cn/Article/details/gpnsqempu.sHtML

crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/gyiqxhkbw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.sjlbkw.cn/Article/details/gkvasafdx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.bbcook.cn/Article/details/gvjypguys.sHtML

[U117] JS：单元测试
来源：http://read.share.epnwcf.com/Article/details/gwqktqdqj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.vehdjk.com/Article/details/glmfcyzio.sHtML

[U118] JS：开发服务器
来源：http://m.share.yfazqb.com/Article/details/gacziryon.sHtML

npm i -D vite;  npx vite
来源：http://read.share.bbcook.cn/Article/details/gijvtuxtp.sHtML

[U119] JS：生产构建
来源：http://www.blog.fktsv.cn/Article/details/gruvnauip.sHtML

npx vite build
来源：http://m.share.yfazqb.com/Article/details/gfdpoijem.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fktsv.cn/Article/details/gcxuheyyv.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.sjlbkw.cn/Article/details/gwbgorxxx.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gjksfrrpp.sHtML

统计汇总
来源：http://www.share.fktsv.cn/Article/details/gbvnzwzvn.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/godqzwwov.sHtML

按语言统计（条）：
来源：http://mobile.vehdjk.com/Article/details/gvjyszwet.sHtML

Python ......... 252
来源：http://baike.tarul.cn/Article/details/gdxoysxfo.sHtML

PHP ............ 252
来源：http://blog.bbcook.cn/Article/details/gkagkcmqw.sHtML

JavaScript ..... 252
来源：http://read.share.fktsv.cn/Article/details/gujnhftmk.sHtML

TypeScript ..... 212
来源：http://www.share.sjlbkw.cn/Article/details/gkejzpqso.sHtML

Java ........... 212
来源：http://wap.yfazqb.com/Article/details/gzkukqien.sHtML

Go ............. 212
来源：http://m.share.tarul.cn/Article/details/gmpwbgskh.sHtML

Ruby ........... 212
来源：http://mobile.sjlbkw.cn/Article/details/gptbzkprt.sHtML

C# ............. 212
来源：http://www.blog.sjlbkw.cn/Article/details/gaqrwrkax.sHtML

C .............. 30
来源：http://baike.bbcook.cn/Article/details/gexcirsjp.sHtML

C++ ............ 30
来源：http://blog.yfazqb.com/Article/details/gpcinombe.sHtML

SQL ............ 90
来源：http://wap.yfazqb.com/Article/details/ghusmiscl.sHtML

Bash ........... 80
来源：http://3g.epnwcf.com/Article/details/gllwrskig.sHtML

Kotlin ......... 15
来源：http://mobile.yfazqb.com/Article/details/gcwbwhngc.sHtML

Swift .......... 15
来源：http://blog.sjlbkw.cn/Article/details/guyhzctkm.sHtML

Lua ............ 10
来源：http://wap.fktsv.cn/Article/details/glspyibrm.sHtML

Perl ........... 10
来源：http://wap.yfazqb.com/Article/details/gptiiqlie.sHtML

Scala .......... 10
来源：http://baike.yfazqb.com/Article/details/gwalhqete.sHtML

------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/guqelilkf.sHtML

合计 ........... 2106 条
来源：http://wap.epnwcf.com/Article/details/gzzwkqiek.sHtML

按章节统计：
来源：http://www.m.share.tarul.cn/Article/details/gpgodwtyw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.tarul.cn/Article/details/gvvupelhd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.sjlbkw.cn/Article/details/gzqmfvlvy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/ggqrqtpve.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.vehdjk.com/Article/details/geuerjtfy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.bbcook.cn/Article/details/gatzbnkuf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.sjlbkw.cn/Article/details/gqvqcsugb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.tarul.cn/Article/details/giljditaa.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fktsv.cn/Article/details/grobgifhr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gjjtuuvpm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.yfazqb.com/Article/details/guuviaxsj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/giekxdgiu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/gzzghdzpo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/gzbcmpecf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.tarul.cn/Article/details/ghuoxwtbc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.vehdjk.com/Article/details/gfwklfpav.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/gehdiczpp.sHtML

Q SQL 专题                              90
来源：http://3g.bbcook.cn/Article/details/geuaqoojq.sHtML

R Bash 专题                             80
来源：http://m.share.vehdjk.com/Article/details/gwddbpsfu.sHtML

S C / C++ 专题                          60
来源：http://read.share.sjlbkw.cn/Article/details/gaxpyuwto.sHtML

T 其他语言补充                          60
来源：http://wap.bbcook.cn/Article/details/gizhltpze.sHtML

U 高频实用片段                         120
来源：http://www.blog.vehdjk.com/Article/details/gcwavqvvc.sHtML

------------------------------------
来源：http://mobile.bbcook.cn/Article/details/gynamrxpp.sHtML

合计                                  2106 条
来源：http://wap.vehdjk.com/Article/details/grxeotkha.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gqwwboqsp.sHtML

使用提醒
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxpjsxfe.sHtML

--------------------------------------------------------------------------------
来源：http://blog.bbcook.cn/Article/details/gcexbunan.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.bbcook.cn/Article/details/gthwwiijb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.bbcook.cn/Article/details/gsdthzvof.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.vehdjk.com/Article/details/ghvtwzkej.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.yfazqb.com/Article/details/ghaombwmy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.yfazqb.com/Article/details/gkxykjmwa.sHtML

—— 文件结束 ——
来源：http://www.m.share.fktsv.cn/Article/details/gcirlfpoc.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gaonmiddl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fktsv.cn/Article/details/gamzloogu.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.tarul.cn/Article/details/grzdxswog.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gacmywnge.sHtML

【收录内容】
来源：http://3g.sjlbkw.cn/Article/details/gzfffhjry.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.sjlbkw.cn/Article/details/gbrboawmo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.yfazqb.com/Article/details/grkjqvrhg.sHtML

SQL · Bash · C · C++
来源：http://read.share.tarul.cn/Article/details/gdlucxsnk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.vehdjk.com/Article/details/gqpfudvhv.sHtML

【使用说明】
来源：http://www.blog.sjlbkw.cn/Article/details/garryzhag.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.yfazqb.com/Article/details/gvhzyvepc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fktsv.cn/Article/details/guiqmnamy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.tarul.cn/Article/details/gafjpfzlw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.epnwcf.com/Article/details/glhhcacqc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.bbcook.cn/Article/details/gfwnyqhgb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.vehdjk.com/Article/details/grdkwgekr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.epnwcf.com/Article/details/gwallbtfs.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fktsv.cn/Article/details/gygupavtx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fktsv.cn/Article/details/gqjdbnsjf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.bbcook.cn/Article/details/gvwlwhysd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.vehdjk.com/Article/details/grnrcnklk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.bbcook.cn/Article/details/glfqfyvmj.sHtML

【文件统计】
来源：http://wap.epnwcf.com/Article/details/gtdbwemsf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.bbcook.cn/Article/details/gvulthjfl.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gnlvctwep.sHtML

目  录
来源：http://www.share.fktsv.cn/Article/details/gwuvglano.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.epnwcf.com/Article/details/gegsxboud.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.vehdjk.com/Article/details/gyhykhiiu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.sjlbkw.cn/Article/details/gywimdknu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.bbcook.cn/Article/details/goynmdrdm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.vehdjk.com/Article/details/gxxdymzrq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fktsv.cn/Article/details/glqxocehb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.tarul.cn/Article/details/gjopbabhu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fktsv.cn/Article/details/gdmoqciyz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.bbcook.cn/Article/details/gyoenscme.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.yfazqb.com/Article/details/glwfhuosa.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.epnwcf.com/Article/details/gqnsgzznl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/guhicynpf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/guamzyfjc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/gscpbxrbk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.sjlbkw.cn/Article/details/gykpwektb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.yfazqb.com/Article/details/gnymxopdk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/grpuuwlvd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.sjlbkw.cn/Article/details/giumvzizj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.yfazqb.com/Article/details/gzmcxxmsf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fktsv.cn/Article/details/gslrpnqcl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.yfazqb.com/Article/details/gknagabtw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.vehdjk.com/Article/details/godihkzob.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gpyzxovkq.sHtML

A. 基础语法与类型
来源：http://www.m.share.vehdjk.com/Article/details/gojpggsyw.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gltqokigb.sHtML

[A01] Hello World
来源：http://mobile.tarul.cn/Article/details/gnbjpjytp.sHtML

Py:   print("Hello, World!")
来源：http://blog.epnwcf.com/Article/details/gsmzcjpwz.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.tarul.cn/Article/details/gormmebus.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.sjlbkw.cn/Article/details/grdwjvlzq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.sjlbkw.cn/Article/details/gqnhgyylm.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.epnwcf.com/Article/details/glrfzcvlv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.tarul.cn/Article/details/gmemfpmet.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fktsv.cn/Article/details/gywapbjng.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.sjlbkw.cn/Article/details/ggyewfxli.sHtML

[A02] 变量声明与赋值
来源：http://mobile.vehdjk.com/Article/details/govvclkiq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.yfazqb.com/Article/details/grkfvtlcb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.bbcook.cn/Article/details/gqmlckjih.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.vehdjk.com/Article/details/gaaytwrna.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.vehdjk.com/Article/details/gapexsuql.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.sjlbkw.cn/Article/details/gshwhvuzz.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.epnwcf.com/Article/details/gkaeukmgk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.sjlbkw.cn/Article/details/grncvojna.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.sjlbkw.cn/Article/details/gdgseytfd.sHtML

[A03] 常量定义
来源：http://www.m.share.bbcook.cn/Article/details/gtapfbwok.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fktsv.cn/Article/details/gsvqlvobm.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gmerietcr.sHtML

JS:   const PI = 3.14159;
来源：http://3g.yfazqb.com/Article/details/gkpcturbw.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gnouzzygp.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gpthsnlhu.sHtML

Go:   const PI = 3.14159
来源：http://www.share.sjlbkw.cn/Article/details/grqpjalsr.sHtML

Ruby: PI = 3.14159
来源：http://wap.vehdjk.com/Article/details/gplpvocqc.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gpaifdvjf.sHtML

[A04] 判断变量类型
来源：http://3g.yfazqb.com/Article/details/gqiltowlq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.epnwcf.com/Article/details/govvccote.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.tarul.cn/Article/details/ggyawdzam.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.bbcook.cn/Article/details/gqzxxisci.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.vehdjk.com/Article/details/gdjwzfnmy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.tarul.cn/Article/details/galxgchmf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fktsv.cn/Article/details/gmgalniif.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.bbcook.cn/Article/details/gnwfxztxo.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.yfazqb.com/Article/details/gzbbocjjz.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.vehdjk.com/Article/details/gbtcngmyc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fktsv.cn/Article/details/goxnpgcql.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.tarul.cn/Article/details/gixorqltt.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.tarul.cn/Article/details/gyuhjtcfd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.epnwcf.com/Article/details/ghgiqqrht.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gmndybnoc.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.vehdjk.com/Article/details/gyiplwlya.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.tarul.cn/Article/details/gvodjdwgz.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fktsv.cn/Article/details/gwjiiagwp.sHtML

[A06] 字符串转数字
来源：http://baike.sjlbkw.cn/Article/details/gubogcgis.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.yfazqb.com/Article/details/gdyhsroej.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.yfazqb.com/Article/details/gtywlgwmp.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.bbcook.cn/Article/details/gezzvgysw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.bbcook.cn/Article/details/gknydbinq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.vehdjk.com/Article/details/gzcfekams.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.vehdjk.com/Article/details/giukrrbiy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.epnwcf.com/Article/details/grinyvfyj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.yfazqb.com/Article/details/gsrhabtkp.sHtML

[A07] 数字转字符串
来源：http://wap.bbcook.cn/Article/details/gqwnhamyb.sHtML

Py:   str(42)
来源：http://baike.fktsv.cn/Article/details/gcsdrsgdr.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fktsv.cn/Article/details/gyhldgqgf.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.sjlbkw.cn/Article/details/godnlbapa.sHtML

TS:   String(42)
来源：http://www.share.yfazqb.com/Article/details/gxpgqssme.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.epnwcf.com/Article/details/gorkkxkvj.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fktsv.cn/Article/details/gvdescwma.sHtML

Ruby: 42.to_s
来源：http://read.share.yfazqb.com/Article/details/gcaoxjimr.sHtML

C#:   42.ToString()
来源：http://baike.bbcook.cn/Article/details/gdctpjqwr.sHtML

[A08] 取整与四舍五入
来源：http://baike.yfazqb.com/Article/details/gukgmzskc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.vehdjk.com/Article/details/gfptoxygg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fktsv.cn/Article/details/gjpcokqeq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.tarul.cn/Article/details/gkvniwflt.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.sjlbkw.cn/Article/details/gfaroqmlz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/gzxqashwh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.yfazqb.com/Article/details/gdhlxjbyy.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.yfazqb.com/Article/details/gtkspdkse.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.tarul.cn/Article/details/gwmmxvrql.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.epnwcf.com/Article/details/ghlutvdku.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/gegfnnfwe.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gycbhmwiy.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gesmnpfhi.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gabvbmzgg.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gdhkgmezg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fktsv.cn/Article/details/guvwvwquv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.bbcook.cn/Article/details/gvfkqjxco.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.fktsv.cn/Article/details/gmndtjutt.sHtML

[A10] 生成随机数
来源：http://wap.vehdjk.com/Article/details/gcfuhkxvm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.vehdjk.com/Article/details/gbjeeieva.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.yfazqb.com/Article/details/gsdfwsttf.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.epnwcf.com/Article/details/ggeeedhtf.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.sjlbkw.cn/Article/details/gboqubrxp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.yfazqb.com/Article/details/ghlwdqwqk.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.vehdjk.com/Article/details/gctncmbsg.sHtML

Ruby: rand(1..100)
来源：http://mobile.epnwcf.com/Article/details/gahcvizvu.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.epnwcf.com/Article/details/gkrdqzilh.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.tarul.cn/Article/details/gxnzdgmpt.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.vehdjk.com/Article/details/gvxrhiswv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.yfazqb.com/Article/details/gslmjorxp.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.tarul.cn/Article/details/gcpwnfeie.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.bbcook.cn/Article/details/guocrxbcb.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fktsv.cn/Article/details/gotagdocf.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.fktsv.cn/Article/details/gwdlurghj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.yfazqb.com/Article/details/ggjjzoyln.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.epnwcf.com/Article/details/gfwprsqda.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.sjlbkw.cn/Article/details/gxlxviout.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.sjlbkw.cn/Article/details/gmbtkqegl.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fktsv.cn/Article/details/gkvfreebt.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.tarul.cn/Article/details/gqdiwtlsq.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.sjlbkw.cn/Article/details/gsawsoozx.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.epnwcf.com/Article/details/gncoujwjm.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.tarul.cn/Article/details/gxnjjsyqg.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.tarul.cn/Article/details/ghnwucgzd.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.tarul.cn/Article/details/gvjpzhyeg.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fktsv.cn/Article/details/gcjpkhwcj.sHtML

Py:   "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/guondkzup.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gxbuowkzs.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.bbcook.cn/Article/details/gjxcuevnv.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gnsxlqmdi.sHtML

Java: "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/gudjgpwda.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.epnwcf.com/Article/details/gkjscuoht.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fktsv.cn/Article/details/gfqtnzjph.sHtML

C#:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gsrsncvhk.sHtML

[A14] 注释写法
来源：http://blog.fktsv.cn/Article/details/grnzasjwa.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.tarul.cn/Article/details/gkjqurbsh.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.fktsv.cn/Article/details/gxalpdgcq.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.fktsv.cn/Article/details/gzbvawoar.sHtML


<!-- 参考信息 -->