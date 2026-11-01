代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://blog.tarul.cn/Article/details/golnansxf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.yfazqb.com/Article/details/gxtoznruh.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.yfazqb.com/Article/details/guyztmxrm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.vehdjk.com/Article/details/ggnpctbdp.sHtML

[U85] JS：可选链
来源：http://3g.bbcook.cn/Article/details/gxinfoggv.sHtML

a?.b?.c
来源：http://www.m.share.fktsv.cn/Article/details/glyolkibi.sHtML

[U86] JS：空值合并
来源：http://wap.bbcook.cn/Article/details/gvvuvcyho.sHtML

a ?? b
来源：http://m.share.yfazqb.com/Article/details/gtkdcgvrt.sHtML

[U87] JS：解构默认值
来源：http://baike.sjlbkw.cn/Article/details/gswbihalp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fktsv.cn/Article/details/gbifzqkcl.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.yfazqb.com/Article/details/gdjjobywx.sHtML

{ ...a, ...b }
来源：http://baike.epnwcf.com/Article/details/gknpflzno.sHtML

[U89] JS：数组去重
来源：http://blog.fktsv.cn/Article/details/gvmksrguz.sHtML

[...new Set(arr)]
来源：http://www.share.sjlbkw.cn/Article/details/gzlwjcuiv.sHtML

[U90] JS：数字数组排序
来源：http://mobile.tarul.cn/Article/details/gkunpswnu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gjryavyms.sHtML

[U91] JS：对象键值遍历
来源：http://wap.bbcook.cn/Article/details/gfehocfkl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.vehdjk.com/Article/details/gesbunjej.sHtML

[U92] JS：深拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gdwwkrhce.sHtML

structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/ghtndddsd.sHtML

[U93] JS：模板字符串
来源：http://read.share.bbcook.cn/Article/details/gbnhinsfv.sHtML

`共 ${n} 条`
来源：http://read.share.epnwcf.com/Article/details/gyrzvhpmh.sHtML

[U94] JS：箭头函数
来源：http://m.share.tarul.cn/Article/details/gamfsttsi.sHtML

const double = x => x * 2;
来源：http://www.blog.tarul.cn/Article/details/goiyzjkbo.sHtML

[U95] JS：Promise 包装
来源：http://mobile.sjlbkw.cn/Article/details/gtzxyezxh.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.epnwcf.com/Article/details/gbqoghufx.sHtML

[U96] JS：async/await 与异常
来源：http://blog.bbcook.cn/Article/details/giakoncpd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gthihhjpm.sHtML

[U97] JS：并发请求
来源：http://www.blog.vehdjk.com/Article/details/gyelsvvys.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/gseuoewkn.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.bbcook.cn/Article/details/glkmkkqql.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.tarul.cn/Article/details/gtwbmkxjt.sHtML

[U99] JS：事件监听
来源：http://www.m.share.bbcook.cn/Article/details/giufphzuo.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.yfazqb.com/Article/details/gpgxtmlxd.sHtML

[U100] JS：DOM 查询
来源：http://read.share.sjlbkw.cn/Article/details/gnvalncxt.sHtML

document.querySelector(".item")
来源：http://www.blog.epnwcf.com/Article/details/gjtpbkouw.sHtML

[U101] JS：classList 操作
来源：http://m.share.fktsv.cn/Article/details/gifyhxnfj.sHtML

el.classList.toggle("active")
来源：http://blog.tarul.cn/Article/details/gpgvgkjzc.sHtML

[U102] JS：本地存储
来源：http://baike.bbcook.cn/Article/details/gfyqqqevf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.yfazqb.com/Article/details/gczoqeive.sHtML

[U103] JS：定时器
来源：http://3g.yfazqb.com/Article/details/ggbjoonna.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.epnwcf.com/Article/details/gibvtvobo.sHtML

[U104] JS：防抖
来源：http://read.share.tarul.cn/Article/details/guquvcexw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.bbcook.cn/Article/details/gpujyojkk.sHtML

[U105] JS：节流
来源：http://www.m.share.fktsv.cn/Article/details/gbtitgmtq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.epnwcf.com/Article/details/gthjhxktg.sHtML

[U106] JS：日期格式化
来源：http://3g.vehdjk.com/Article/details/gstslymna.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.vehdjk.com/Article/details/gdpagnwse.sHtML

[U107] JS：数字千分位
来源：http://baike.tarul.cn/Article/details/gmkeymhel.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.bbcook.cn/Article/details/gtsppumik.sHtML

[U108] JS：随机整数
来源：http://m.share.vehdjk.com/Article/details/gaukewmfn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.yfazqb.com/Article/details/gkbqechvc.sHtML

[U109] JS：数组分组
来源：http://www.m.share.yfazqb.com/Article/details/gjvxpvlma.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.vehdjk.com/Article/details/gsuojipjx.sHtML

[U110] JS：数组分块
来源：http://mobile.vehdjk.com/Article/details/grmljezjc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.bbcook.cn/Article/details/gjzuvrtjc.sHtML

[U111] JS：对象转 Map
来源：http://read.share.vehdjk.com/Article/details/gcxnzjtsp.sHtML

new Map(Object.entries(obj))
来源：http://blog.tarul.cn/Article/details/grtosrmrc.sHtML

[U112] JS：字符串补位
来源：http://3g.epnwcf.com/Article/details/gaiwdzuzp.sHtML

"7".padStart(3, "0")
来源：http://wap.epnwcf.com/Article/details/gmtguzmhj.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.vehdjk.com/Article/details/gauowosko.sHtML

s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/glistsmoj.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.sjlbkw.cn/Article/details/gfbseiqja.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.vehdjk.com/Article/details/gyrmmidrx.sHtML

[U115] JS：生成 UUID
来源：http://mobile.tarul.cn/Article/details/gxpoyvumi.sHtML

crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/grhymtpln.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fktsv.cn/Article/details/gvypengeu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.tarul.cn/Article/details/gapcropzn.sHtML

[U117] JS：单元测试
来源：http://wap.vehdjk.com/Article/details/gtcjrmzvr.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.epnwcf.com/Article/details/gsbxmxceu.sHtML

[U118] JS：开发服务器
来源：http://read.share.vehdjk.com/Article/details/gijuuvgax.sHtML

npm i -D vite;  npx vite
来源：http://mobile.sjlbkw.cn/Article/details/gpigodvlc.sHtML

[U119] JS：生产构建
来源：http://wap.epnwcf.com/Article/details/gbslaksgc.sHtML

npx vite build
来源：http://www.blog.epnwcf.com/Article/details/gprdaqfqf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.yfazqb.com/Article/details/glqabyukw.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxcxxrna.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gmykbdbup.sHtML

统计汇总
来源：http://www.blog.bbcook.cn/Article/details/guzzjkihp.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gnweuutpa.sHtML

按语言统计（条）：
来源：http://blog.epnwcf.com/Article/details/gcuhinvbi.sHtML

Python ......... 252
来源：http://mobile.tarul.cn/Article/details/gfjdsbold.sHtML

PHP ............ 252
来源：http://www.blog.epnwcf.com/Article/details/gsohanoja.sHtML

JavaScript ..... 252
来源：http://wap.bbcook.cn/Article/details/gnqeobrxv.sHtML

TypeScript ..... 212
来源：http://www.share.sjlbkw.cn/Article/details/gsebrdtbq.sHtML

Java ........... 212
来源：http://3g.epnwcf.com/Article/details/ggiarzrzq.sHtML

Go ............. 212
来源：http://www.blog.bbcook.cn/Article/details/gwfralqew.sHtML

Ruby ........... 212
来源：http://wap.tarul.cn/Article/details/gsjyhkgcy.sHtML

C# ............. 212
来源：http://3g.vehdjk.com/Article/details/gsxkcckfv.sHtML

C .............. 30
来源：http://blog.tarul.cn/Article/details/gzsdxjxjm.sHtML

C++ ............ 30
来源：http://www.m.share.bbcook.cn/Article/details/gopwtqywb.sHtML

SQL ............ 90
来源：http://3g.tarul.cn/Article/details/gxaekkrpl.sHtML

Bash ........... 80
来源：http://m.share.vehdjk.com/Article/details/gnntyqhab.sHtML

Kotlin ......... 15
来源：http://m.share.yfazqb.com/Article/details/gszrhgkkj.sHtML

Swift .......... 15
来源：http://mobile.bbcook.cn/Article/details/gacuhgnyx.sHtML

Lua ............ 10
来源：http://3g.fktsv.cn/Article/details/gctgwockp.sHtML

Perl ........... 10
来源：http://www.share.tarul.cn/Article/details/gfyacdwll.sHtML

Scala .......... 10
来源：http://www.share.bbcook.cn/Article/details/gkvaumcoi.sHtML

------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gpsrgpxnq.sHtML

合计 ........... 2106 条
来源：http://blog.epnwcf.com/Article/details/ggnhtgxjj.sHtML

按章节统计：
来源：http://m.share.bbcook.cn/Article/details/gqfxrnpxv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.vehdjk.com/Article/details/ggurvagqi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.sjlbkw.cn/Article/details/gnpqoqfcz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.yfazqb.com/Article/details/gfcofvdtw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.vehdjk.com/Article/details/gibboszbr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.tarul.cn/Article/details/gkbyeqqbf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.yfazqb.com/Article/details/gikacgvov.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gswgwegeo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.sjlbkw.cn/Article/details/gpzreuhof.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuwylhjz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.epnwcf.com/Article/details/gtafhqdud.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gbllxlpon.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gartnfbpx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.bbcook.cn/Article/details/gauduqtnr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.yfazqb.com/Article/details/gsrqsecgj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.tarul.cn/Article/details/gzxrxslag.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/guuclmwal.sHtML

Q SQL 专题                              90
来源：http://read.share.yfazqb.com/Article/details/gwqryiyab.sHtML

R Bash 专题                             80
来源：http://mobile.vehdjk.com/Article/details/gfzodrpjw.sHtML

S C / C++ 专题                          60
来源：http://mobile.yfazqb.com/Article/details/gnlbuhppv.sHtML

T 其他语言补充                          60
来源：http://read.share.tarul.cn/Article/details/gmhlkezdr.sHtML

U 高频实用片段                         120
来源：http://baike.bbcook.cn/Article/details/gidwqbojz.sHtML

------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gxsmofelk.sHtML

合计                                  2106 条
来源：http://read.share.epnwcf.com/Article/details/guwolktsh.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.tarul.cn/Article/details/gjulrtrzp.sHtML

使用提醒
来源：http://baike.yfazqb.com/Article/details/gorcrznkr.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gfnarmfnk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.tarul.cn/Article/details/gvfujdsvg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.vehdjk.com/Article/details/ghtxrxcbr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.bbcook.cn/Article/details/gvzicdvcb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.vehdjk.com/Article/details/gzrdxifck.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.tarul.cn/Article/details/gowqekkyv.sHtML

—— 文件结束 ——
来源：http://baike.epnwcf.com/Article/details/gkxmiebzg.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gatwajtfo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.sjlbkw.cn/Article/details/gobadkuyv.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.yfazqb.com/Article/details/gbiohhjqe.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gbchdqmqx.sHtML

【收录内容】
来源：http://mobile.tarul.cn/Article/details/grlusqgsu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.vehdjk.com/Article/details/gjqtamaoz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.epnwcf.com/Article/details/gatdldpna.sHtML

SQL · Bash · C · C++
来源：http://m.share.yfazqb.com/Article/details/gqiapwtzh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fktsv.cn/Article/details/gdbszedad.sHtML

【使用说明】
来源：http://mobile.vehdjk.com/Article/details/gunxycbqg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.sjlbkw.cn/Article/details/gjdirasbd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.tarul.cn/Article/details/gnwvvbfmw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fktsv.cn/Article/details/ghyainilp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.yfazqb.com/Article/details/gligdkajl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.yfazqb.com/Article/details/gfbitpcsq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.vehdjk.com/Article/details/gbnuniwwj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.bbcook.cn/Article/details/gcsvenvhi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.epnwcf.com/Article/details/grdwmytlf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.bbcook.cn/Article/details/gvimdtfek.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.yfazqb.com/Article/details/gbuquxymt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fktsv.cn/Article/details/gcmmnryby.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.epnwcf.com/Article/details/gshlkoxft.sHtML

【文件统计】
来源：http://baike.tarul.cn/Article/details/gzppqqhvt.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.sjlbkw.cn/Article/details/geluxyoxv.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.tarul.cn/Article/details/gormwiqxd.sHtML

目  录
来源：http://www.share.vehdjk.com/Article/details/gsaqsmzex.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gcmulqepv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.epnwcf.com/Article/details/gzmgrtwxr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.epnwcf.com/Article/details/gnmrjxtls.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.tarul.cn/Article/details/gfknkzgvj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.vehdjk.com/Article/details/gcmnxcytm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.sjlbkw.cn/Article/details/gzqakvdds.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.sjlbkw.cn/Article/details/gabduvbjh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.sjlbkw.cn/Article/details/gralgtlug.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.tarul.cn/Article/details/gsentliad.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/gsriwqsbn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.bbcook.cn/Article/details/getecnuan.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.yfazqb.com/Article/details/gjgcrbrwz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/ghceicbir.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.bbcook.cn/Article/details/ghdflmhlt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.yfazqb.com/Article/details/gidcrbdba.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fktsv.cn/Article/details/ghppfaywh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.yfazqb.com/Article/details/gbsagwnph.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.bbcook.cn/Article/details/gvxybzuzo.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.epnwcf.com/Article/details/ghzmmwexc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.vehdjk.com/Article/details/gpbgcegkc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.bbcook.cn/Article/details/gdoezbgav.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.yfazqb.com/Article/details/gugahjgjt.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/glspyfqpv.sHtML

A. 基础语法与类型
来源：http://3g.bbcook.cn/Article/details/gppdvozvp.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gaugjrpbb.sHtML

[A01] Hello World
来源：http://m.share.yfazqb.com/Article/details/garzvdwqg.sHtML

Py:   print("Hello, World!")
来源：http://baike.epnwcf.com/Article/details/gskewartd.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fktsv.cn/Article/details/gvixedqub.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.vehdjk.com/Article/details/gzsrqzcyz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.epnwcf.com/Article/details/gfwbewvuq.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.bbcook.cn/Article/details/gqmmctvxw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.bbcook.cn/Article/details/gvlbqwpkd.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.tarul.cn/Article/details/gpyyltqew.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fktsv.cn/Article/details/gmghqcnrk.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.sjlbkw.cn/Article/details/gylihvcpp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.bbcook.cn/Article/details/gyjrjndtd.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.vehdjk.com/Article/details/gaxuzbnwq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.yfazqb.com/Article/details/gzefbqsst.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fktsv.cn/Article/details/giwvethfq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.yfazqb.com/Article/details/gcehnzuca.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.yfazqb.com/Article/details/gclezgstu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcqvnrux.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.yfazqb.com/Article/details/gckfzsbbq.sHtML

[A03] 常量定义
来源：http://m.share.bbcook.cn/Article/details/gfbedrkpn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrakblaa.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/guqpmunlg.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gnhomiarp.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrydllea.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gykrlevna.sHtML

Go:   const PI = 3.14159
来源：http://3g.vehdjk.com/Article/details/gkvudaesk.sHtML

Ruby: PI = 3.14159
来源：http://read.share.vehdjk.com/Article/details/giuznmqro.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/gsnquatvq.sHtML

[A04] 判断变量类型
来源：http://blog.fktsv.cn/Article/details/gtzlxagzs.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fktsv.cn/Article/details/gnazzbgyb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.bbcook.cn/Article/details/gkftziekx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.vehdjk.com/Article/details/gnytnqldv.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.sjlbkw.cn/Article/details/gkyecxsyh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.sjlbkw.cn/Article/details/gqnjrygrh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.epnwcf.com/Article/details/gtsfkobsz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.bbcook.cn/Article/details/goxqdgzvi.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.yfazqb.com/Article/details/glrlmxgeb.sHtML

[A05] 整数除法与取模
来源：http://baike.bbcook.cn/Article/details/gocnxrwyf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.bbcook.cn/Article/details/gdidvfjkr.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gcnctxocl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/gvhsmakwv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.yfazqb.com/Article/details/gfxkpezfc.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.bbcook.cn/Article/details/gcczhpacs.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gswphuvev.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.sjlbkw.cn/Article/details/gtjaimjhz.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fktsv.cn/Article/details/gllzwsjtu.sHtML

[A06] 字符串转数字
来源：http://3g.vehdjk.com/Article/details/gqnopfqnr.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.tarul.cn/Article/details/gpufuhykg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.yfazqb.com/Article/details/gjgiokpif.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.sjlbkw.cn/Article/details/grbikzypy.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.tarul.cn/Article/details/gbyakxvwk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.epnwcf.com/Article/details/gdfhmyvss.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.tarul.cn/Article/details/girplcfdd.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.yfazqb.com/Article/details/gvlcrnvps.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.vehdjk.com/Article/details/gwhwldill.sHtML

[A07] 数字转字符串
来源：http://blog.bbcook.cn/Article/details/gqcpflthj.sHtML

Py:   str(42)
来源：http://baike.epnwcf.com/Article/details/gfcuckpcx.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.sjlbkw.cn/Article/details/gxnbegpse.sHtML

JS:   String(42); (42).toString()
来源：http://blog.vehdjk.com/Article/details/gbjadpjhs.sHtML

TS:   String(42)
来源：http://baike.bbcook.cn/Article/details/glvrgdzmm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.tarul.cn/Article/details/griiryzyv.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.vehdjk.com/Article/details/gxqiptpfy.sHtML

Ruby: 42.to_s
来源：http://3g.bbcook.cn/Article/details/gziswbfvb.sHtML

C#:   42.ToString()
来源：http://baike.tarul.cn/Article/details/gcfanlgfh.sHtML

[A08] 取整与四舍五入
来源：http://blog.yfazqb.com/Article/details/gmzswbyyj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.epnwcf.com/Article/details/gtlegazbb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.bbcook.cn/Article/details/glxdjvsup.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.vehdjk.com/Article/details/gowgxntvn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.bbcook.cn/Article/details/gtmjxabdn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.tarul.cn/Article/details/gcahabfjm.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.tarul.cn/Article/details/gflwjzyye.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.sjlbkw.cn/Article/details/giofukdsp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.epnwcf.com/Article/details/gmcpvovxb.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.tarul.cn/Article/details/gowxojxxj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gondxvrfn.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gfvnijoda.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.epnwcf.com/Article/details/gsrnhpjqj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gzczfwwvl.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.vehdjk.com/Article/details/gpsmndsth.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.tarul.cn/Article/details/gnshtlvca.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.tarul.cn/Article/details/gdevsshbv.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/golauqhjv.sHtML

[A10] 生成随机数
来源：http://baike.sjlbkw.cn/Article/details/gfhwcwttl.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.epnwcf.com/Article/details/gspxrpbpa.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.tarul.cn/Article/details/gsrxaoslb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.yfazqb.com/Article/details/gnigegcai.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fktsv.cn/Article/details/ggpdpevag.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.epnwcf.com/Article/details/gmlourhxk.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.fktsv.cn/Article/details/gqbtyulah.sHtML

Ruby: rand(1..100)
来源：http://baike.vehdjk.com/Article/details/gnxslnrgy.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.vehdjk.com/Article/details/ggmwzdubx.sHtML

[A11] 条件表达式（三元）
来源：http://blog.epnwcf.com/Article/details/gpzrlnrab.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.sjlbkw.cn/Article/details/golpwacoq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.bbcook.cn/Article/details/gslleutko.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.sjlbkw.cn/Article/details/gnpelijex.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.tarul.cn/Article/details/gzwykzfub.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.epnwcf.com/Article/details/gytxmwpzz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.sjlbkw.cn/Article/details/gayaomweg.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.vehdjk.com/Article/details/gcsgzlkzw.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/guxwiqyfr.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.sjlbkw.cn/Article/details/gcmxprbvk.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.vehdjk.com/Article/details/gnkmmotql.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.vehdjk.com/Article/details/gjszmawyj.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.fktsv.cn/Article/details/ganmpdmzg.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.yfazqb.com/Article/details/gcpapwqjf.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.vehdjk.com/Article/details/gnmxjjqwc.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.epnwcf.com/Article/details/gupcthqiz.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fktsv.cn/Article/details/gumjwiiar.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.fktsv.cn/Article/details/gzpgsicpj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.bbcook.cn/Article/details/gzsvjqrpm.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/gaphlnxsf.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/gmddoovjl.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.tarul.cn/Article/details/gbpjbhjhw.sHtML

TS:   "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/gjsdufhsc.sHtML

Java: "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/gjntfknpl.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.epnwcf.com/Article/details/gawsnjaof.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gmgbyybds.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/gwgrkwhno.sHtML


<!-- 参考信息 -->