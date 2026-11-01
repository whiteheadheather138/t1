代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://read.share.vehdjk.com/Article/details/ghzlhpgfd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.vehdjk.com/Article/details/gxjtjlysm.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.epnwcf.com/Article/details/grsumhmts.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.epnwcf.com/Article/details/gssgygdvu.sHtML

[U85] JS：可选链
来源：http://www.share.bbcook.cn/Article/details/gdbtyztba.sHtML

a?.b?.c
来源：http://wap.yfazqb.com/Article/details/gzaeagrij.sHtML

[U86] JS：空值合并
来源：http://wap.fktsv.cn/Article/details/gjdmiafct.sHtML

a ?? b
来源：http://mobile.vehdjk.com/Article/details/gyxdilzxv.sHtML

[U87] JS：解构默认值
来源：http://read.share.tarul.cn/Article/details/ghcjqdbzb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fktsv.cn/Article/details/gudcecyog.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fktsv.cn/Article/details/gunjmustq.sHtML

{ ...a, ...b }
来源：http://blog.sjlbkw.cn/Article/details/gdxhlecke.sHtML

[U89] JS：数组去重
来源：http://baike.sjlbkw.cn/Article/details/gljdbxsre.sHtML

[...new Set(arr)]
来源：http://3g.sjlbkw.cn/Article/details/genglqwxx.sHtML

[U90] JS：数字数组排序
来源：http://3g.sjlbkw.cn/Article/details/gamvusmid.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbeeuliqk.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gjlshuvsb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.bbcook.cn/Article/details/ghsapvtaj.sHtML

[U92] JS：深拷贝
来源：http://read.share.epnwcf.com/Article/details/gdtwdodzm.sHtML

structuredClone(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gdsdqcbnr.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gldcipppl.sHtML

`共 ${n} 条`
来源：http://3g.fktsv.cn/Article/details/gzygqwvmj.sHtML

[U94] JS：箭头函数
来源：http://www.blog.sjlbkw.cn/Article/details/gjtbiqahe.sHtML

const double = x => x * 2;
来源：http://m.share.fktsv.cn/Article/details/gmsiqabvn.sHtML

[U95] JS：Promise 包装
来源：http://read.share.epnwcf.com/Article/details/gjfbocxgg.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.epnwcf.com/Article/details/gwwyovzqd.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.tarul.cn/Article/details/gixwryfyq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gbhhjevna.sHtML

[U97] JS：并发请求
来源：http://www.m.share.yfazqb.com/Article/details/goszhycer.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/gdocunxcc.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.bbcook.cn/Article/details/gzfqionqo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fktsv.cn/Article/details/gtkrinkbc.sHtML

[U99] JS：事件监听
来源：http://baike.vehdjk.com/Article/details/gikfglgfk.sHtML

el.addEventListener("click", e => {})
来源：http://blog.bbcook.cn/Article/details/gkrnehefi.sHtML

[U100] JS：DOM 查询
来源：http://blog.yfazqb.com/Article/details/gzyhrtxvs.sHtML

document.querySelector(".item")
来源：http://www.blog.epnwcf.com/Article/details/gcdpkcduv.sHtML

[U101] JS：classList 操作
来源：http://wap.sjlbkw.cn/Article/details/gyxkhktxb.sHtML

el.classList.toggle("active")
来源：http://wap.epnwcf.com/Article/details/gkasfixdn.sHtML

[U102] JS：本地存储
来源：http://m.share.sjlbkw.cn/Article/details/gskiopwmm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.yfazqb.com/Article/details/gtdjhwbnz.sHtML

[U103] JS：定时器
来源：http://www.blog.epnwcf.com/Article/details/grdfyvpvj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.sjlbkw.cn/Article/details/gsgeybazx.sHtML

[U104] JS：防抖
来源：http://www.blog.fktsv.cn/Article/details/goarcpchm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gjyhwqhlx.sHtML

[U105] JS：节流
来源：http://3g.tarul.cn/Article/details/gnvdprxce.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.tarul.cn/Article/details/geuopjyhp.sHtML

[U106] JS：日期格式化
来源：http://m.share.sjlbkw.cn/Article/details/gmaxzurcx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.bbcook.cn/Article/details/goihtacug.sHtML

[U107] JS：数字千分位
来源：http://wap.sjlbkw.cn/Article/details/gaavqqcxz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.yfazqb.com/Article/details/gcrjhwjyy.sHtML

[U108] JS：随机整数
来源：http://blog.vehdjk.com/Article/details/gisemoexi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.vehdjk.com/Article/details/gidlqzbii.sHtML

[U109] JS：数组分组
来源：http://3g.vehdjk.com/Article/details/gtclfkmyk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.vehdjk.com/Article/details/gqpokrrcl.sHtML

[U110] JS：数组分块
来源：http://blog.tarul.cn/Article/details/ggotwpxja.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.vehdjk.com/Article/details/gvslbossn.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.epnwcf.com/Article/details/gwvuyexgo.sHtML

new Map(Object.entries(obj))
来源：http://baike.tarul.cn/Article/details/gpnpipzzt.sHtML

[U112] JS：字符串补位
来源：http://baike.bbcook.cn/Article/details/gensuidgd.sHtML

"7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/glncjmvkd.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.epnwcf.com/Article/details/gsyppexll.sHtML

s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gqvpcosrx.sHtML

[U114] JS：JSON 深比较
来源：http://blog.tarul.cn/Article/details/gzlqwewrm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/geiobeejk.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.sjlbkw.cn/Article/details/gmrqghtkf.sHtML

crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/ghpggaxct.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.vehdjk.com/Article/details/glvphigmu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.bbcook.cn/Article/details/gzmyprhbb.sHtML

[U117] JS：单元测试
来源：http://read.share.tarul.cn/Article/details/giljalyum.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.epnwcf.com/Article/details/gtwswmblg.sHtML

[U118] JS：开发服务器
来源：http://baike.sjlbkw.cn/Article/details/glxqrqvzb.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.vehdjk.com/Article/details/gcvxnixyi.sHtML

[U119] JS：生产构建
来源：http://3g.fktsv.cn/Article/details/gxmuycoin.sHtML

npx vite build
来源：http://m.share.fktsv.cn/Article/details/gmbvnzape.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fktsv.cn/Article/details/glnqyhtru.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.tarul.cn/Article/details/gnedkmtvg.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ggsyvuyml.sHtML

统计汇总
来源：http://www.share.bbcook.cn/Article/details/gohxvllpw.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gulkqzgsb.sHtML

按语言统计（条）：
来源：http://m.share.fktsv.cn/Article/details/gukiddhtc.sHtML

Python ......... 252
来源：http://m.share.fktsv.cn/Article/details/gwycgbdkz.sHtML

PHP ............ 252
来源：http://read.share.epnwcf.com/Article/details/gwqlnacxb.sHtML

JavaScript ..... 252
来源：http://baike.sjlbkw.cn/Article/details/gvufitctr.sHtML

TypeScript ..... 212
来源：http://www.share.epnwcf.com/Article/details/gvzxuyupw.sHtML

Java ........... 212
来源：http://baike.fktsv.cn/Article/details/gudytfuof.sHtML

Go ............. 212
来源：http://www.share.yfazqb.com/Article/details/gxdsqqaux.sHtML

Ruby ........... 212
来源：http://mobile.bbcook.cn/Article/details/ghoxxqdfz.sHtML

C# ............. 212
来源：http://baike.yfazqb.com/Article/details/gmukipyoc.sHtML

C .............. 30
来源：http://wap.tarul.cn/Article/details/gqzalktnd.sHtML

C++ ............ 30
来源：http://m.share.epnwcf.com/Article/details/gfwuoezfo.sHtML

SQL ............ 90
来源：http://mobile.sjlbkw.cn/Article/details/gvqgyllsi.sHtML

Bash ........... 80
来源：http://mobile.tarul.cn/Article/details/gjesyslen.sHtML

Kotlin ......... 15
来源：http://mobile.sjlbkw.cn/Article/details/gksulcujm.sHtML

Swift .......... 15
来源：http://www.share.epnwcf.com/Article/details/gtjskojvk.sHtML

Lua ............ 10
来源：http://blog.fktsv.cn/Article/details/gptqpjgsb.sHtML

Perl ........... 10
来源：http://www.share.vehdjk.com/Article/details/gurcsuwjd.sHtML

Scala .......... 10
来源：http://www.blog.epnwcf.com/Article/details/gfpkesxra.sHtML

------------------------------------
来源：http://blog.vehdjk.com/Article/details/gpgdrsyii.sHtML

合计 ........... 2106 条
来源：http://www.share.bbcook.cn/Article/details/gjfzwyzgn.sHtML

按章节统计：
来源：http://read.share.yfazqb.com/Article/details/gjgfmubin.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fktsv.cn/Article/details/gptlpwzwk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.sjlbkw.cn/Article/details/ggkshkxzc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fktsv.cn/Article/details/gazqmcrfz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.bbcook.cn/Article/details/gildkgwls.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fktsv.cn/Article/details/gyhkbjcqw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.epnwcf.com/Article/details/geiyobudl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.tarul.cn/Article/details/ghtsvrmcc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.sjlbkw.cn/Article/details/gfzrsrbaz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/grtddjwkm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fktsv.cn/Article/details/gtfgzkmll.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/gezgmcfgc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gnhieqlap.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gbnbaawkf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.sjlbkw.cn/Article/details/gqjniefsy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.bbcook.cn/Article/details/ghmgnsept.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/gtjbosdsm.sHtML

Q SQL 专题                              90
来源：http://www.blog.bbcook.cn/Article/details/ggirvgwse.sHtML

R Bash 专题                             80
来源：http://blog.tarul.cn/Article/details/gvofubuwa.sHtML

S C / C++ 专题                          60
来源：http://baike.sjlbkw.cn/Article/details/gdvjxiuvi.sHtML

T 其他语言补充                          60
来源：http://www.m.share.vehdjk.com/Article/details/gfqqfudas.sHtML

U 高频实用片段                         120
来源：http://www.share.sjlbkw.cn/Article/details/gsiawfrky.sHtML

------------------------------------
来源：http://blog.vehdjk.com/Article/details/gfegqkydn.sHtML

合计                                  2106 条
来源：http://3g.tarul.cn/Article/details/grausvfss.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fktsv.cn/Article/details/gmhipokyq.sHtML

使用提醒
来源：http://baike.epnwcf.com/Article/details/gntwnejte.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.yfazqb.com/Article/details/glvmtrakh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.tarul.cn/Article/details/gkhfnftqu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.bbcook.cn/Article/details/guuovatlo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.epnwcf.com/Article/details/gaulnfqio.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.bbcook.cn/Article/details/gdjnncuxr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.yfazqb.com/Article/details/gasmgetli.sHtML

—— 文件结束 ——
来源：http://blog.epnwcf.com/Article/details/gtzyezjdt.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/glxwkxlhh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.yfazqb.com/Article/details/gyderjvbf.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.epnwcf.com/Article/details/gauiihmzy.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gzzrsvpak.sHtML

【收录内容】
来源：http://mobile.tarul.cn/Article/details/gaehzxxhm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.bbcook.cn/Article/details/gcpajsxac.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fktsv.cn/Article/details/gkqoxkwfz.sHtML

SQL · Bash · C · C++
来源：http://mobile.sjlbkw.cn/Article/details/gfhqxebuq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.epnwcf.com/Article/details/gnffmlguk.sHtML

【使用说明】
来源：http://baike.vehdjk.com/Article/details/gioavpraj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fktsv.cn/Article/details/gdhtprrgv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.yfazqb.com/Article/details/gowabcwbq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.epnwcf.com/Article/details/gbwzheqxv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.epnwcf.com/Article/details/giqmkmpxi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.vehdjk.com/Article/details/gegbyjuvj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.tarul.cn/Article/details/gksoppwgb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.epnwcf.com/Article/details/gmfntdywj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.vehdjk.com/Article/details/gjgxfpcny.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.vehdjk.com/Article/details/geivpmirs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.sjlbkw.cn/Article/details/ghfbsioxr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.epnwcf.com/Article/details/gwqybnsdk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.sjlbkw.cn/Article/details/ghzvvoouf.sHtML

【文件统计】
来源：http://3g.fktsv.cn/Article/details/ghkljtmqv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.yfazqb.com/Article/details/gqegfcjez.sHtML

--------------------------------------------------------------------------------
来源：http://wap.epnwcf.com/Article/details/gojjjusfv.sHtML

目  录
来源：http://m.share.sjlbkw.cn/Article/details/gopbqjhiw.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/grssxibyd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.tarul.cn/Article/details/gwffqprbp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.vehdjk.com/Article/details/gpmkbhxap.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fktsv.cn/Article/details/geuvcoirr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.yfazqb.com/Article/details/ghlxsmfdm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.epnwcf.com/Article/details/gkjnzpywj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.bbcook.cn/Article/details/gtaatbqkz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.yfazqb.com/Article/details/ghztepmuo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.tarul.cn/Article/details/gptacpiep.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/gvcmctpnm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.tarul.cn/Article/details/gdqeucbnb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/gdilxsxud.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.tarul.cn/Article/details/gxussxftk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gtmwpkaok.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.epnwcf.com/Article/details/gfnccszbv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.bbcook.cn/Article/details/gdosowgmn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.sjlbkw.cn/Article/details/gyjyvyjtb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.sjlbkw.cn/Article/details/gduteugei.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.tarul.cn/Article/details/gruodaxpr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.yfazqb.com/Article/details/glkydpczs.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.tarul.cn/Article/details/gyxlbttba.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.vehdjk.com/Article/details/gzplbokkp.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/glirktiyu.sHtML

A. 基础语法与类型
来源：http://wap.vehdjk.com/Article/details/gatdqutid.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gmhrafjnj.sHtML

[A01] Hello World
来源：http://wap.epnwcf.com/Article/details/grifajema.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.vehdjk.com/Article/details/giwxlrjzd.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.sjlbkw.cn/Article/details/grnxfcqcc.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.yfazqb.com/Article/details/gvkhokcdd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.bbcook.cn/Article/details/gwjbtctxb.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.tarul.cn/Article/details/gvkcwsiia.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.bbcook.cn/Article/details/gkmnrblkk.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.sjlbkw.cn/Article/details/girlxetru.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fktsv.cn/Article/details/gmvdlgbua.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fktsv.cn/Article/details/gwoejyhjt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.sjlbkw.cn/Article/details/glrmogibf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fktsv.cn/Article/details/gihjzxezj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.epnwcf.com/Article/details/gyopmdroh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.sjlbkw.cn/Article/details/gcsfylijp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.epnwcf.com/Article/details/gixjvowjt.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.tarul.cn/Article/details/grytuvbfs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fktsv.cn/Article/details/gwfuoxsil.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.vehdjk.com/Article/details/gvggszdxm.sHtML

[A03] 常量定义
来源：http://www.blog.epnwcf.com/Article/details/gsuuwwszq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.yfazqb.com/Article/details/glrdhtlwj.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/godfecdbv.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gsfdfjneq.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gkbwaruxu.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gzpjmatna.sHtML

Go:   const PI = 3.14159
来源：http://read.share.vehdjk.com/Article/details/gwmmifgzq.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fktsv.cn/Article/details/gpjpukjlq.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gdkuzsvof.sHtML

[A04] 判断变量类型
来源：http://3g.yfazqb.com/Article/details/gcyovcuph.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fktsv.cn/Article/details/geofspjux.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.tarul.cn/Article/details/gakszpbro.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.sjlbkw.cn/Article/details/gglskqgpj.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.vehdjk.com/Article/details/gakxyynkw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fktsv.cn/Article/details/gyirbklyk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fktsv.cn/Article/details/gdguvqyrc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.yfazqb.com/Article/details/girjtpnuw.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.bbcook.cn/Article/details/gkuvykibx.sHtML

[A05] 整数除法与取模
来源：http://mobile.vehdjk.com/Article/details/gxpxtsusm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fktsv.cn/Article/details/gkkxliiao.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gfroabzfn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gayykgsqg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.yfazqb.com/Article/details/gurcwjcwq.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gztvwaces.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/gqlohezbb.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.fktsv.cn/Article/details/gvxgenovd.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gybzvdwmd.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fktsv.cn/Article/details/gzikmzjsa.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.vehdjk.com/Article/details/gllceqdlw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fktsv.cn/Article/details/grgxugtfu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fktsv.cn/Article/details/gekjyyofa.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.yfazqb.com/Article/details/gfpcepnig.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.epnwcf.com/Article/details/gspbutvvy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.tarul.cn/Article/details/gxygzxpqc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.bbcook.cn/Article/details/gnmlzcatf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.vehdjk.com/Article/details/gqsfortoh.sHtML

[A07] 数字转字符串
来源：http://www.share.tarul.cn/Article/details/gebbvgtaw.sHtML

Py:   str(42)
来源：http://mobile.tarul.cn/Article/details/ggjjkbmdv.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.epnwcf.com/Article/details/gifciggce.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.yfazqb.com/Article/details/gczgjqkui.sHtML

TS:   String(42)
来源：http://wap.tarul.cn/Article/details/gzacxhdcf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.yfazqb.com/Article/details/gjejvlfbl.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.sjlbkw.cn/Article/details/gkrtogzwo.sHtML

Ruby: 42.to_s
来源：http://www.blog.fktsv.cn/Article/details/gvtvyfdnn.sHtML

C#:   42.ToString()
来源：http://wap.tarul.cn/Article/details/gibxyiwiz.sHtML

[A08] 取整与四舍五入
来源：http://baike.fktsv.cn/Article/details/gsupqwytb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.bbcook.cn/Article/details/ghssihmiw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fktsv.cn/Article/details/gimugifmw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.epnwcf.com/Article/details/gotmrhvjl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.yfazqb.com/Article/details/glqmvgtwq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.sjlbkw.cn/Article/details/guyfnaqcy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.sjlbkw.cn/Article/details/gzmhjogfq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.bbcook.cn/Article/details/gjcwjshig.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.epnwcf.com/Article/details/gjniytmeb.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.epnwcf.com/Article/details/gmvgwifoh.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gqudhtglt.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.epnwcf.com/Article/details/gahefbeec.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gxmemmjjh.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gzwksbbgh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.fktsv.cn/Article/details/gnfqlhcjp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.sjlbkw.cn/Article/details/glvaxwamq.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.epnwcf.com/Article/details/gfgmpfefu.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gzzxqlexy.sHtML

[A10] 生成随机数
来源：http://www.share.bbcook.cn/Article/details/gcekozakn.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.bbcook.cn/Article/details/gxhxxqxxf.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.tarul.cn/Article/details/gzxgnhagm.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.bbcook.cn/Article/details/grfmlejxq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.tarul.cn/Article/details/gviqueykb.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.epnwcf.com/Article/details/gdgyylupn.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.vehdjk.com/Article/details/gwgoerufx.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgxongxp.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.fktsv.cn/Article/details/glulrlhde.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.bbcook.cn/Article/details/gzwtbezxx.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.tarul.cn/Article/details/gikbptrrv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.tarul.cn/Article/details/gxwbnlvpl.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/gijpobzvv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.sjlbkw.cn/Article/details/gxrtfwyko.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.bbcook.cn/Article/details/glnvsgqsd.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.bbcook.cn/Article/details/gvhifjxhj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.sjlbkw.cn/Article/details/gjzkgsufq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gtujfpfeo.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.vehdjk.com/Article/details/gstouyhmd.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.vehdjk.com/Article/details/gtrxdtvjw.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.vehdjk.com/Article/details/gsclmegvw.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.yfazqb.com/Article/details/ggpizzcik.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.bbcook.cn/Article/details/gpmlipqge.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.bbcook.cn/Article/details/gshhhruxx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.sjlbkw.cn/Article/details/grgogughh.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.vehdjk.com/Article/details/gnqjdalue.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.yfazqb.com/Article/details/gcixxwray.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.tarul.cn/Article/details/gecuyuhnl.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.vehdjk.com/Article/details/gqspneyxq.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.tarul.cn/Article/details/ghbxnupmw.sHtML

JS:   "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/ghpvkeywi.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gqretymos.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.bbcook.cn/Article/details/gxcctbebu.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/gytspebrt.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gyxbhzhcv.sHtML

C#:   "第一行\n第二行"
来源：http://wap.yfazqb.com/Article/details/gwrbuezdg.sHtML


<!-- 参考信息 -->