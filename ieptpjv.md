代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.share.epnwcf.com/Article/details/geurxorxl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.yfazqb.com/Article/details/ggjvqsmqs.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.sjlbkw.cn/Article/details/goqabkezf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.tarul.cn/Article/details/gaegmexvb.sHtML

[U85] JS：可选链
来源：http://www.m.share.yfazqb.com/Article/details/gxqiptybr.sHtML

a?.b?.c
来源：http://m.share.vehdjk.com/Article/details/givizwaqt.sHtML

[U86] JS：空值合并
来源：http://mobile.yfazqb.com/Article/details/gxexjqnsi.sHtML

a ?? b
来源：http://m.share.epnwcf.com/Article/details/gqaftwbwy.sHtML

[U87] JS：解构默认值
来源：http://baike.tarul.cn/Article/details/gtjafclnr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.tarul.cn/Article/details/gfkjudosk.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fktsv.cn/Article/details/gkygvrewn.sHtML

{ ...a, ...b }
来源：http://mobile.epnwcf.com/Article/details/gwpuwwgpb.sHtML

[U89] JS：数组去重
来源：http://wap.sjlbkw.cn/Article/details/gfyzpbivh.sHtML

[...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/guebooale.sHtML

[U90] JS：数字数组排序
来源：http://blog.epnwcf.com/Article/details/gfsjhkqzi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gcauzgilj.sHtML

[U91] JS：对象键值遍历
来源：http://3g.vehdjk.com/Article/details/gkhvwvfqm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.bbcook.cn/Article/details/grywzizjk.sHtML

[U92] JS：深拷贝
来源：http://wap.yfazqb.com/Article/details/gjrdzvnhd.sHtML

structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/gvzpjcqix.sHtML

[U93] JS：模板字符串
来源：http://www.share.epnwcf.com/Article/details/gnwoocztz.sHtML

`共 ${n} 条`
来源：http://www.share.yfazqb.com/Article/details/gylcmhzcq.sHtML

[U94] JS：箭头函数
来源：http://m.share.epnwcf.com/Article/details/gfbiolcuq.sHtML

const double = x => x * 2;
来源：http://m.share.yfazqb.com/Article/details/grhmmylkq.sHtML

[U95] JS：Promise 包装
来源：http://wap.bbcook.cn/Article/details/gfxpopwaj.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.tarul.cn/Article/details/ghltxmwle.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.yfazqb.com/Article/details/grvbrzsoy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.sjlbkw.cn/Article/details/glxyadfku.sHtML

[U97] JS：并发请求
来源：http://wap.tarul.cn/Article/details/gmypwwhpl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/grmghsbwz.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gzcernoql.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.vehdjk.com/Article/details/glphelfar.sHtML

[U99] JS：事件监听
来源：http://www.m.share.tarul.cn/Article/details/grhuxdosd.sHtML

el.addEventListener("click", e => {})
来源：http://blog.vehdjk.com/Article/details/gprrbyucp.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fktsv.cn/Article/details/gshuvohkw.sHtML

document.querySelector(".item")
来源：http://wap.epnwcf.com/Article/details/gknfycqeh.sHtML

[U101] JS：classList 操作
来源：http://baike.bbcook.cn/Article/details/gxnmfbzlm.sHtML

el.classList.toggle("active")
来源：http://baike.fktsv.cn/Article/details/gklqjcrln.sHtML

[U102] JS：本地存储
来源：http://www.blog.epnwcf.com/Article/details/gwjysiwoy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fktsv.cn/Article/details/gxqvotipj.sHtML

[U103] JS：定时器
来源：http://www.m.share.sjlbkw.cn/Article/details/gtksyuogg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.tarul.cn/Article/details/gbshcbauy.sHtML

[U104] JS：防抖
来源：http://www.m.share.tarul.cn/Article/details/gqfvsdggj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/gsehrajnf.sHtML

[U105] JS：节流
来源：http://read.share.bbcook.cn/Article/details/gnustvrxw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.epnwcf.com/Article/details/gpcmsfneo.sHtML

[U106] JS：日期格式化
来源：http://3g.yfazqb.com/Article/details/gbiksvgdt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.sjlbkw.cn/Article/details/ghzdxyasy.sHtML

[U107] JS：数字千分位
来源：http://3g.tarul.cn/Article/details/gszuivujp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.yfazqb.com/Article/details/gyrsmwnla.sHtML

[U108] JS：随机整数
来源：http://blog.bbcook.cn/Article/details/gpznzxdpe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.epnwcf.com/Article/details/gvokaystt.sHtML

[U109] JS：数组分组
来源：http://blog.sjlbkw.cn/Article/details/ghcblbfdn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.tarul.cn/Article/details/gcqwzhckz.sHtML

[U110] JS：数组分块
来源：http://wap.epnwcf.com/Article/details/gmajvjjho.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.bbcook.cn/Article/details/gwzzgrfur.sHtML

[U111] JS：对象转 Map
来源：http://read.share.bbcook.cn/Article/details/gzodcimzw.sHtML

new Map(Object.entries(obj))
来源：http://blog.fktsv.cn/Article/details/gjzhblvzl.sHtML

[U112] JS：字符串补位
来源：http://wap.bbcook.cn/Article/details/gqwlqerdc.sHtML

"7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/grgtbzbdw.sHtML

[U113] JS：正则替换全部
来源：http://wap.bbcook.cn/Article/details/gpyajqttx.sHtML

s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gshnannik.sHtML

[U114] JS：JSON 深比较
来源：http://baike.bbcook.cn/Article/details/gxpmccwag.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.bbcook.cn/Article/details/gdyvcrrjy.sHtML

[U115] JS：生成 UUID
来源：http://baike.tarul.cn/Article/details/gdavkfrxa.sHtML

crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gozpnoxzp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.epnwcf.com/Article/details/gqmdeucni.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.epnwcf.com/Article/details/gsasdyxtu.sHtML

[U117] JS：单元测试
来源：http://www.m.share.vehdjk.com/Article/details/gzvawebat.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.tarul.cn/Article/details/ggttvxzod.sHtML

[U118] JS：开发服务器
来源：http://baike.sjlbkw.cn/Article/details/gdjfxdokx.sHtML

npm i -D vite;  npx vite
来源：http://wap.vehdjk.com/Article/details/glmwktvjo.sHtML

[U119] JS：生产构建
来源：http://3g.fktsv.cn/Article/details/gbnwmmous.sHtML

npx vite build
来源：http://3g.epnwcf.com/Article/details/gmfgmvdno.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.yfazqb.com/Article/details/gkzixxpry.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.sjlbkw.cn/Article/details/gvujznvzm.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gylacutho.sHtML

统计汇总
来源：http://www.blog.vehdjk.com/Article/details/gqdljjsye.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gggcysbcv.sHtML

按语言统计（条）：
来源：http://mobile.vehdjk.com/Article/details/gfthygwtn.sHtML

Python ......... 252
来源：http://mobile.sjlbkw.cn/Article/details/gxbdvbqlx.sHtML

PHP ............ 252
来源：http://m.share.vehdjk.com/Article/details/gmglrsang.sHtML

JavaScript ..... 252
来源：http://m.share.yfazqb.com/Article/details/ggpoeowhu.sHtML

TypeScript ..... 212
来源：http://3g.epnwcf.com/Article/details/gylahpomg.sHtML

Java ........... 212
来源：http://blog.fktsv.cn/Article/details/gdokvrcos.sHtML

Go ............. 212
来源：http://m.share.epnwcf.com/Article/details/gwtvrniba.sHtML

Ruby ........... 212
来源：http://mobile.tarul.cn/Article/details/grujaxafs.sHtML

C# ............. 212
来源：http://baike.bbcook.cn/Article/details/gqkkowfaa.sHtML

C .............. 30
来源：http://m.share.fktsv.cn/Article/details/ggtqfgpse.sHtML

C++ ............ 30
来源：http://wap.fktsv.cn/Article/details/gmomtlcew.sHtML

SQL ............ 90
来源：http://www.blog.epnwcf.com/Article/details/gsoggkjov.sHtML

Bash ........... 80
来源：http://3g.yfazqb.com/Article/details/gfrjahjre.sHtML

Kotlin ......... 15
来源：http://wap.tarul.cn/Article/details/guowdegmy.sHtML

Swift .......... 15
来源：http://m.share.yfazqb.com/Article/details/gokhnciig.sHtML

Lua ............ 10
来源：http://blog.sjlbkw.cn/Article/details/gicfsasin.sHtML

Perl ........... 10
来源：http://wap.epnwcf.com/Article/details/gtysugsmx.sHtML

Scala .......... 10
来源：http://www.share.bbcook.cn/Article/details/geyqoskco.sHtML

------------------------------------
来源：http://3g.tarul.cn/Article/details/gktzgnrbt.sHtML

合计 ........... 2106 条
来源：http://blog.vehdjk.com/Article/details/glhflhzco.sHtML

按章节统计：
来源：http://mobile.epnwcf.com/Article/details/glbrkevye.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.vehdjk.com/Article/details/glttuaswo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.yfazqb.com/Article/details/gnrvkjpar.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.tarul.cn/Article/details/geddxpudf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fktsv.cn/Article/details/gidumkelw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fktsv.cn/Article/details/gfweyeaux.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.tarul.cn/Article/details/geyiehkic.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/gebqzlhjl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.bbcook.cn/Article/details/gzfxlvtjv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gsxqsbmrj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.epnwcf.com/Article/details/gcelkkfpz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/gxjkythgp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gittifgjp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.bbcook.cn/Article/details/gdmpzgqjl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.epnwcf.com/Article/details/gbdwekhqb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.bbcook.cn/Article/details/ghoapmhqv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gndxpbxdd.sHtML

Q SQL 专题                              90
来源：http://blog.bbcook.cn/Article/details/gtyufccfh.sHtML

R Bash 专题                             80
来源：http://baike.vehdjk.com/Article/details/gqftnskak.sHtML

S C / C++ 专题                          60
来源：http://mobile.sjlbkw.cn/Article/details/gkbcbiinz.sHtML

T 其他语言补充                          60
来源：http://baike.sjlbkw.cn/Article/details/glzbewmho.sHtML

U 高频实用片段                         120
来源：http://baike.vehdjk.com/Article/details/gkgjiiydo.sHtML

------------------------------------
来源：http://3g.epnwcf.com/Article/details/geymhigxn.sHtML

合计                                  2106 条
来源：http://mobile.sjlbkw.cn/Article/details/gurhjtjde.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gfrrzoqks.sHtML

使用提醒
来源：http://read.share.fktsv.cn/Article/details/gnwgciqol.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gbqadqnap.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.yfazqb.com/Article/details/gowzqfaoi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.bbcook.cn/Article/details/gvncaxkxp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.sjlbkw.cn/Article/details/geholfjsc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.sjlbkw.cn/Article/details/gyobgzqkh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fktsv.cn/Article/details/gcyviuvgv.sHtML

—— 文件结束 ——
来源：http://read.share.epnwcf.com/Article/details/gecuhgeyy.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/goatoqvip.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.sjlbkw.cn/Article/details/gsphylgbo.sHtML

Common Programming Examples Cheat Book
来源：http://baike.yfazqb.com/Article/details/ghmewxdca.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gwkhtibgt.sHtML

【收录内容】
来源：http://mobile.epnwcf.com/Article/details/gsbhvylrg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.epnwcf.com/Article/details/gzulqasaf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.yfazqb.com/Article/details/gypfkcqfy.sHtML

SQL · Bash · C · C++
来源：http://mobile.epnwcf.com/Article/details/gutznghzx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.vehdjk.com/Article/details/gdszymwrz.sHtML

【使用说明】
来源：http://baike.sjlbkw.cn/Article/details/garylqqvr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.vehdjk.com/Article/details/ghhtstnoc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.bbcook.cn/Article/details/gjlwdidtd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.bbcook.cn/Article/details/ggdtksphz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fktsv.cn/Article/details/gctyfirkl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.epnwcf.com/Article/details/gcxwicbqo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.tarul.cn/Article/details/glqfppecl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.sjlbkw.cn/Article/details/gdjswnhga.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fktsv.cn/Article/details/gdcyyzncm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.bbcook.cn/Article/details/gzgbxjmzr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.tarul.cn/Article/details/gtrdfvpnc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.bbcook.cn/Article/details/gokgsgesi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.vehdjk.com/Article/details/gngztccoh.sHtML

【文件统计】
来源：http://www.m.share.vehdjk.com/Article/details/gmlukmbia.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.yfazqb.com/Article/details/gglisobbp.sHtML

--------------------------------------------------------------------------------
来源：http://3g.yfazqb.com/Article/details/gdosdtoan.sHtML

目  录
来源：http://wap.fktsv.cn/Article/details/gqqtnddgl.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gavksbeqs.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.tarul.cn/Article/details/gleystwlm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.vehdjk.com/Article/details/gmodgswjx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.bbcook.cn/Article/details/gopsmievs.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.epnwcf.com/Article/details/gasoafnxm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.yfazqb.com/Article/details/gfltqskrl.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.sjlbkw.cn/Article/details/gvngkfpba.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.bbcook.cn/Article/details/gzjjakuir.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fktsv.cn/Article/details/grlhstdsk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.sjlbkw.cn/Article/details/gyibhrbkm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.tarul.cn/Article/details/gagbkpqac.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gicffokkh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.vehdjk.com/Article/details/gpjomawaf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/gqqsbjrpo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.bbcook.cn/Article/details/ggsqiyvvk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.yfazqb.com/Article/details/gwqnnthfa.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gkultgzqc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fktsv.cn/Article/details/gqpusufjp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.epnwcf.com/Article/details/goabfokqr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.vehdjk.com/Article/details/gospeglex.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.sjlbkw.cn/Article/details/gszdlcgje.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.tarul.cn/Article/details/gtgihsljs.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gakgkdonh.sHtML

A. 基础语法与类型
来源：http://baike.fktsv.cn/Article/details/gqljfgfxh.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gcvcjbxil.sHtML

[A01] Hello World
来源：http://mobile.tarul.cn/Article/details/gzaoejutu.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fktsv.cn/Article/details/gavsvxjts.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.yfazqb.com/Article/details/ggkznckbo.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.vehdjk.com/Article/details/gnddcixgk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.sjlbkw.cn/Article/details/gztiaoglq.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.sjlbkw.cn/Article/details/gikxfckmm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.epnwcf.com/Article/details/gvwuryxjx.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.yfazqb.com/Article/details/gwfobiyxr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.tarul.cn/Article/details/gudipxuhd.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.tarul.cn/Article/details/golbmyyyv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fktsv.cn/Article/details/gdbtvraft.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.vehdjk.com/Article/details/grytmdbxn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fktsv.cn/Article/details/gpaoumstq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.sjlbkw.cn/Article/details/gehuthfab.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.epnwcf.com/Article/details/gusekondn.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fktsv.cn/Article/details/gvlgjrrew.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.vehdjk.com/Article/details/gnimxopww.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.vehdjk.com/Article/details/glmheokzo.sHtML

[A03] 常量定义
来源：http://3g.epnwcf.com/Article/details/gehrimjyi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.yfazqb.com/Article/details/gwbixyonv.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gdvqlkehi.sHtML

JS:   const PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/guacvnmfq.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gxqucrsnn.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/ggdmcqrxq.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.tarul.cn/Article/details/gjigrokya.sHtML

Ruby: PI = 3.14159
来源：http://www.share.epnwcf.com/Article/details/gjexjliup.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gxxpqwdph.sHtML

[A04] 判断变量类型
来源：http://baike.epnwcf.com/Article/details/gsylmlgjc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.tarul.cn/Article/details/gdgoumwri.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.yfazqb.com/Article/details/gdegpwowx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fktsv.cn/Article/details/gyuvtvvwz.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.bbcook.cn/Article/details/gmlhemdxa.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.bbcook.cn/Article/details/gyoxogfiz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.bbcook.cn/Article/details/gnrwbrrun.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.bbcook.cn/Article/details/gutrcxvnm.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.epnwcf.com/Article/details/gpdnbdrdb.sHtML

[A05] 整数除法与取模
来源：http://www.share.yfazqb.com/Article/details/ghhxodldm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.vehdjk.com/Article/details/gbvdfzuri.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.tarul.cn/Article/details/gnhsarkcv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/gvmommowv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.sjlbkw.cn/Article/details/gwymecpdd.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.yfazqb.com/Article/details/gxgkaqyyf.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.tarul.cn/Article/details/gyxmbggxw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.bbcook.cn/Article/details/gigxrwevn.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.epnwcf.com/Article/details/gyvcmsvfp.sHtML

[A06] 字符串转数字
来源：http://3g.yfazqb.com/Article/details/gtnfkyhfp.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.bbcook.cn/Article/details/gknjbflwp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fktsv.cn/Article/details/gqmonpbtl.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.tarul.cn/Article/details/gzeossqjx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.bbcook.cn/Article/details/gnudzoukf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.tarul.cn/Article/details/gxptjejds.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.vehdjk.com/Article/details/grmawswsu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.yfazqb.com/Article/details/gtrotqtqw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.fktsv.cn/Article/details/gmfojawrq.sHtML

[A07] 数字转字符串
来源：http://www.blog.yfazqb.com/Article/details/grfdyaxek.sHtML

Py:   str(42)
来源：http://3g.yfazqb.com/Article/details/gypzqkyjq.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.tarul.cn/Article/details/gqrugkccw.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.epnwcf.com/Article/details/gtydzteju.sHtML

TS:   String(42)
来源：http://3g.sjlbkw.cn/Article/details/gwzmfhtgl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.bbcook.cn/Article/details/gburfoljt.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.epnwcf.com/Article/details/grfbfiqjf.sHtML

Ruby: 42.to_s
来源：http://wap.yfazqb.com/Article/details/gimuxyxzi.sHtML

C#:   42.ToString()
来源：http://wap.bbcook.cn/Article/details/gvaxquyyu.sHtML

[A08] 取整与四舍五入
来源：http://3g.fktsv.cn/Article/details/gouorwvfx.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.yfazqb.com/Article/details/guamhdpqu.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fktsv.cn/Article/details/gmphbehdp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.epnwcf.com/Article/details/glyqylcey.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fktsv.cn/Article/details/gnkuurfhr.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.sjlbkw.cn/Article/details/glzijjkmj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.sjlbkw.cn/Article/details/gyoouliec.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.bbcook.cn/Article/details/gewathwhw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.epnwcf.com/Article/details/gtmhkrviq.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.vehdjk.com/Article/details/gowjljwrx.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.tarul.cn/Article/details/giezqwytx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gzcuxdgxy.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.vehdjk.com/Article/details/gkdosmztb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gflbjpsfo.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gtjinugkg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.sjlbkw.cn/Article/details/gonflaphw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcpkzdqb.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gbwtyyhio.sHtML

[A10] 生成随机数
来源：http://mobile.epnwcf.com/Article/details/gtbsgtubm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.tarul.cn/Article/details/gxhqyqngc.sHtML

PHP:  random_int(1, 100);
来源：http://blog.tarul.cn/Article/details/gelmwodvu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.yfazqb.com/Article/details/gctgrtzdt.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.vehdjk.com/Article/details/gaacarehw.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.epnwcf.com/Article/details/gditfincj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.yfazqb.com/Article/details/gcumcpgfv.sHtML

Ruby: rand(1..100)
来源：http://mobile.epnwcf.com/Article/details/gaxcwedmr.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.yfazqb.com/Article/details/gudasbefw.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.epnwcf.com/Article/details/gqvtujzut.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.epnwcf.com/Article/details/gttutpinu.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.epnwcf.com/Article/details/gnxigatpe.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.sjlbkw.cn/Article/details/gslnmsauo.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.yfazqb.com/Article/details/grhvadasl.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.vehdjk.com/Article/details/garbckpnp.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.tarul.cn/Article/details/glfrlupoh.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.bbcook.cn/Article/details/geexczasm.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.vehdjk.com/Article/details/gfzzcwkxf.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.yfazqb.com/Article/details/gpqotkdde.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.bbcook.cn/Article/details/gclddpgom.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.epnwcf.com/Article/details/gncxbidwh.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.epnwcf.com/Article/details/gskpegwnf.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.bbcook.cn/Article/details/gnbvqqeqg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.tarul.cn/Article/details/genifvllt.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.sjlbkw.cn/Article/details/gsfvbqqhs.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.sjlbkw.cn/Article/details/gdksoxsuu.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.epnwcf.com/Article/details/gtxyunbiz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.epnwcf.com/Article/details/gjumqmfwc.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmqcptvp.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gspslvdsh.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/gdheruzuc.sHtML

TS:   "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/geuhjxpos.sHtML

Java: "第一行\n第二行"
来源：http://wap.vehdjk.com/Article/details/gjxmphrwc.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.bbcook.cn/Article/details/gmljktbcu.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/gbjjjylsm.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gyyhmdypy.sHtML


<!-- 参考信息 -->