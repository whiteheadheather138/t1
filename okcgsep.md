代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://baike.sjlbkw.cn/Article/details/gjayetccz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fktsv.cn/Article/details/gqjgufuir.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.yfazqb.com/Article/details/gwpvmnepz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.vehdjk.com/Article/details/gxvpaqecy.sHtML

[U85] JS：可选链
来源：http://www.blog.epnwcf.com/Article/details/gzkartovu.sHtML

a?.b?.c
来源：http://read.share.tarul.cn/Article/details/gzyrpgadi.sHtML

[U86] JS：空值合并
来源：http://blog.bbcook.cn/Article/details/gmdsxgbfv.sHtML

a ?? b
来源：http://mobile.sjlbkw.cn/Article/details/gmjorhijo.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fktsv.cn/Article/details/gveegdlyq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.vehdjk.com/Article/details/gmslweyyz.sHtML

[U88] JS：对象展开合并
来源：http://blog.sjlbkw.cn/Article/details/ghjktyliz.sHtML

{ ...a, ...b }
来源：http://mobile.yfazqb.com/Article/details/gaigcfebd.sHtML

[U89] JS：数组去重
来源：http://www.blog.vehdjk.com/Article/details/gplnxdpkl.sHtML

[...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/geksvrcau.sHtML

[U90] JS：数字数组排序
来源：http://www.share.sjlbkw.cn/Article/details/glcvivwnj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/gryxqnhna.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.bbcook.cn/Article/details/geyqvpjel.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fktsv.cn/Article/details/gblmgrxhz.sHtML

[U92] JS：深拷贝
来源：http://mobile.tarul.cn/Article/details/gkpehqvjm.sHtML

structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gromoiqvu.sHtML

[U93] JS：模板字符串
来源：http://www.share.yfazqb.com/Article/details/gtrivdgbi.sHtML

`共 ${n} 条`
来源：http://mobile.vehdjk.com/Article/details/grlvhfnzx.sHtML

[U94] JS：箭头函数
来源：http://read.share.tarul.cn/Article/details/gncefrzxh.sHtML

const double = x => x * 2;
来源：http://m.share.bbcook.cn/Article/details/gqbxbtbmk.sHtML

[U95] JS：Promise 包装
来源：http://blog.epnwcf.com/Article/details/gzpjfuilp.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.vehdjk.com/Article/details/gdgllzzvn.sHtML

[U96] JS：async/await 与异常
来源：http://wap.tarul.cn/Article/details/gigquacxg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gclsuelvj.sHtML

[U97] JS：并发请求
来源：http://www.share.bbcook.cn/Article/details/gpblkmeba.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/gxojzvnts.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.tarul.cn/Article/details/gtmcokcbw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.epnwcf.com/Article/details/glajlsopk.sHtML

[U99] JS：事件监听
来源：http://mobile.sjlbkw.cn/Article/details/gsparxxls.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.sjlbkw.cn/Article/details/gjjxolwjl.sHtML

[U100] JS：DOM 查询
来源：http://m.share.bbcook.cn/Article/details/ggpqjqolg.sHtML

document.querySelector(".item")
来源：http://blog.tarul.cn/Article/details/gqkcuemuq.sHtML

[U101] JS：classList 操作
来源：http://www.share.vehdjk.com/Article/details/gpwhhkvow.sHtML

el.classList.toggle("active")
来源：http://baike.tarul.cn/Article/details/gyvjcomzp.sHtML

[U102] JS：本地存储
来源：http://baike.epnwcf.com/Article/details/glhmflvga.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.vehdjk.com/Article/details/godouytyi.sHtML

[U103] JS：定时器
来源：http://www.share.fktsv.cn/Article/details/gtbiossjr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.vehdjk.com/Article/details/gmelsbafx.sHtML

[U104] JS：防抖
来源：http://read.share.yfazqb.com/Article/details/gbvabguuj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/gmjcjsxev.sHtML

[U105] JS：节流
来源：http://m.share.sjlbkw.cn/Article/details/gnmiqgukt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.yfazqb.com/Article/details/gdqaazdes.sHtML

[U106] JS：日期格式化
来源：http://mobile.vehdjk.com/Article/details/ggmxnznwv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.sjlbkw.cn/Article/details/grrqiimwh.sHtML

[U107] JS：数字千分位
来源：http://read.share.yfazqb.com/Article/details/ghcwsyrkq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.yfazqb.com/Article/details/gdpjbuthp.sHtML

[U108] JS：随机整数
来源：http://mobile.vehdjk.com/Article/details/gpayqrxqe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.epnwcf.com/Article/details/gfdenvegw.sHtML

[U109] JS：数组分组
来源：http://m.share.yfazqb.com/Article/details/gwpdoxzcd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fktsv.cn/Article/details/gjqpgtfqn.sHtML

[U110] JS：数组分块
来源：http://3g.bbcook.cn/Article/details/gzcdpcxmq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.bbcook.cn/Article/details/gdsnhpwbh.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpuuhdcy.sHtML

new Map(Object.entries(obj))
来源：http://baike.bbcook.cn/Article/details/gfagldeou.sHtML

[U112] JS：字符串补位
来源：http://www.blog.vehdjk.com/Article/details/ggdbyhghd.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/giujesaet.sHtML

[U113] JS：正则替换全部
来源：http://m.share.sjlbkw.cn/Article/details/gdsvsuhuh.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gavuwnrhv.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.yfazqb.com/Article/details/gdloescsd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.bbcook.cn/Article/details/gvkznlgjc.sHtML

[U115] JS：生成 UUID
来源：http://m.share.vehdjk.com/Article/details/gfvqrzjxz.sHtML

crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/gpevvhdai.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.bbcook.cn/Article/details/gslyjbsiz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.yfazqb.com/Article/details/gilldvdud.sHtML

[U117] JS：单元测试
来源：http://www.blog.yfazqb.com/Article/details/gnivhgple.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.yfazqb.com/Article/details/gjrqfovxo.sHtML

[U118] JS：开发服务器
来源：http://www.blog.tarul.cn/Article/details/gkqtjfrsp.sHtML

npm i -D vite;  npx vite
来源：http://3g.yfazqb.com/Article/details/gbzikisqp.sHtML

[U119] JS：生产构建
来源：http://mobile.vehdjk.com/Article/details/guxtgcnbl.sHtML

npx vite build
来源：http://baike.epnwcf.com/Article/details/gqfiqotaw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.bbcook.cn/Article/details/guvkgelyl.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.tarul.cn/Article/details/gggduqpkl.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gtcjheomv.sHtML

统计汇总
来源：http://m.share.fktsv.cn/Article/details/ghumjkufh.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gddsqawbb.sHtML

按语言统计（条）：
来源：http://3g.fktsv.cn/Article/details/gcifqotim.sHtML

Python ......... 252
来源：http://www.share.fktsv.cn/Article/details/gnraapsrm.sHtML

PHP ............ 252
来源：http://www.blog.bbcook.cn/Article/details/gwwhzxddv.sHtML

JavaScript ..... 252
来源：http://read.share.vehdjk.com/Article/details/gbyrizrte.sHtML

TypeScript ..... 212
来源：http://wap.sjlbkw.cn/Article/details/gqxfpkksd.sHtML

Java ........... 212
来源：http://m.share.vehdjk.com/Article/details/gkrfydrff.sHtML

Go ............. 212
来源：http://3g.vehdjk.com/Article/details/gjwcrmhql.sHtML

Ruby ........... 212
来源：http://www.m.share.vehdjk.com/Article/details/gwjscfhdd.sHtML

C# ............. 212
来源：http://read.share.tarul.cn/Article/details/gayzkvmzg.sHtML

C .............. 30
来源：http://wap.bbcook.cn/Article/details/gqyzodbbw.sHtML

C++ ............ 30
来源：http://baike.sjlbkw.cn/Article/details/glkeepxdl.sHtML

SQL ............ 90
来源：http://www.blog.bbcook.cn/Article/details/gromhfjke.sHtML

Bash ........... 80
来源：http://www.share.bbcook.cn/Article/details/grqilghbr.sHtML

Kotlin ......... 15
来源：http://blog.sjlbkw.cn/Article/details/gumdysfsq.sHtML

Swift .......... 15
来源：http://wap.fktsv.cn/Article/details/gbxqnftvs.sHtML

Lua ............ 10
来源：http://mobile.fktsv.cn/Article/details/gqttqnffx.sHtML

Perl ........... 10
来源：http://3g.yfazqb.com/Article/details/gbhizbshh.sHtML

Scala .......... 10
来源：http://wap.tarul.cn/Article/details/grwoezpdk.sHtML

------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gksqeuvpk.sHtML

合计 ........... 2106 条
来源：http://www.blog.tarul.cn/Article/details/gvufyqwyl.sHtML

按章节统计：
来源：http://wap.yfazqb.com/Article/details/gnprvnyub.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.tarul.cn/Article/details/grlmrlnqi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fktsv.cn/Article/details/gupnnwwaq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.vehdjk.com/Article/details/gduxlnqak.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fktsv.cn/Article/details/gvrjetuhx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.vehdjk.com/Article/details/ggdgmpqgl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.vehdjk.com/Article/details/gnstonqka.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.vehdjk.com/Article/details/giduidxuj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.tarul.cn/Article/details/gmomgfcyx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gkrindbni.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.vehdjk.com/Article/details/ggxbwrzar.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/gfgermtgd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/gmutybrwv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gzxbbztca.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.sjlbkw.cn/Article/details/gexltlois.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.sjlbkw.cn/Article/details/gvmazcjyp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gfuimghth.sHtML

Q SQL 专题                              90
来源：http://read.share.bbcook.cn/Article/details/gezoxoqud.sHtML

R Bash 专题                             80
来源：http://mobile.epnwcf.com/Article/details/glwuxfdmq.sHtML

S C / C++ 专题                          60
来源：http://wap.vehdjk.com/Article/details/gysdybvoy.sHtML

T 其他语言补充                          60
来源：http://blog.bbcook.cn/Article/details/guynvzsna.sHtML

U 高频实用片段                         120
来源：http://m.share.fktsv.cn/Article/details/gwlhvwica.sHtML

------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gfwmecmad.sHtML

合计                                  2106 条
来源：http://blog.tarul.cn/Article/details/gokopesvv.sHtML

--------------------------------------------------------------------------------
来源：http://3g.vehdjk.com/Article/details/grzcfzvdo.sHtML

使用提醒
来源：http://m.share.tarul.cn/Article/details/gngurmvwy.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/garwnslsx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fktsv.cn/Article/details/gzievrngk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.bbcook.cn/Article/details/glsrbloko.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fktsv.cn/Article/details/grptwscem.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.vehdjk.com/Article/details/gspwdmmnn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.vehdjk.com/Article/details/glzyytktb.sHtML

—— 文件结束 ——
来源：http://m.share.tarul.cn/Article/details/ggyfbnnly.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gvdlbpjmf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.epnwcf.com/Article/details/gsnadsitx.sHtML

Common Programming Examples Cheat Book
来源：http://blog.yfazqb.com/Article/details/ggxjaukzi.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gpymidzjk.sHtML

【收录内容】
来源：http://read.share.fktsv.cn/Article/details/gunfjrqpk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.yfazqb.com/Article/details/gxzbilrjo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.bbcook.cn/Article/details/glilrlszt.sHtML

SQL · Bash · C · C++
来源：http://m.share.epnwcf.com/Article/details/gieivkkjc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.epnwcf.com/Article/details/ggxzbbhmc.sHtML

【使用说明】
来源：http://3g.tarul.cn/Article/details/glsebnuer.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.epnwcf.com/Article/details/gjqprydws.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.vehdjk.com/Article/details/gfzzqfhwq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.epnwcf.com/Article/details/gtfzgigaa.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.vehdjk.com/Article/details/gemqhbllo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.bbcook.cn/Article/details/gjkudsbeb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.vehdjk.com/Article/details/gbjbofiwx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.epnwcf.com/Article/details/gkdxoilhv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fktsv.cn/Article/details/gelbgdyoe.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fktsv.cn/Article/details/gvbxexgvw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.epnwcf.com/Article/details/gsvqtapdc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.bbcook.cn/Article/details/grqakembq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.tarul.cn/Article/details/gjxzxbrxe.sHtML

【文件统计】
来源：http://baike.vehdjk.com/Article/details/ggjljlfaq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fktsv.cn/Article/details/gspwipdwq.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/gkgmlpjmj.sHtML

目  录
来源：http://blog.yfazqb.com/Article/details/gguztwfrv.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gqsnxexcn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.epnwcf.com/Article/details/gykeelorf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.bbcook.cn/Article/details/gczeeipqv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.vehdjk.com/Article/details/ghsjqunnp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fktsv.cn/Article/details/gfztyuntl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.bbcook.cn/Article/details/gylgipsyb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.bbcook.cn/Article/details/gckburfse.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fktsv.cn/Article/details/gsrjnfaiy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.epnwcf.com/Article/details/gydtiwaqp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fktsv.cn/Article/details/gnrrmqubd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.tarul.cn/Article/details/gscntjtws.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gibkueklm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/glxfbjiwr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.yfazqb.com/Article/details/gzqldvcga.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.yfazqb.com/Article/details/gkusjymdo.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.tarul.cn/Article/details/gvuvnfwfq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/gjrouetbh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.epnwcf.com/Article/details/gmlvgqdex.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.bbcook.cn/Article/details/glrxyyeog.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.vehdjk.com/Article/details/gsdssciex.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fktsv.cn/Article/details/gcuydobbc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.yfazqb.com/Article/details/gyzalbwwe.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gxmqhmzle.sHtML

A. 基础语法与类型
来源：http://www.blog.epnwcf.com/Article/details/gzoahadoa.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gfigghyce.sHtML

[A01] Hello World
来源：http://wap.yfazqb.com/Article/details/gccbbgmvb.sHtML

Py:   print("Hello, World!")
来源：http://read.share.bbcook.cn/Article/details/gdnbfrbps.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.tarul.cn/Article/details/glsxwrvet.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.vehdjk.com/Article/details/grluuagrd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.epnwcf.com/Article/details/gwzweleyy.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.vehdjk.com/Article/details/glxpltiou.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.bbcook.cn/Article/details/gmgumyuvs.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.epnwcf.com/Article/details/glzremutk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.yfazqb.com/Article/details/gfdsrcbql.sHtML

[A02] 变量声明与赋值
来源：http://read.share.yfazqb.com/Article/details/gfpfqlbuq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.tarul.cn/Article/details/gkhzkiefg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.epnwcf.com/Article/details/gdwmmxwji.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.vehdjk.com/Article/details/gmdwaccbt.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fktsv.cn/Article/details/grziopxwr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.tarul.cn/Article/details/gdkjeoifl.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.tarul.cn/Article/details/gdsyhkues.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.vehdjk.com/Article/details/gkmuaejyl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fktsv.cn/Article/details/gtbamcsvj.sHtML

[A03] 常量定义
来源：http://m.share.tarul.cn/Article/details/goxikdktx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.vehdjk.com/Article/details/gfemkcbhi.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gvggahdln.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gchnutpsu.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gvpuxltud.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gjhpoixqy.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.epnwcf.com/Article/details/gveczmyun.sHtML

Ruby: PI = 3.14159
来源：http://m.share.epnwcf.com/Article/details/gxpcunvzj.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/gzgqrijsc.sHtML

[A04] 判断变量类型
来源：http://www.m.share.tarul.cn/Article/details/gtsaxtuaj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.yfazqb.com/Article/details/ghgaupapy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.bbcook.cn/Article/details/garhqdpon.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.bbcook.cn/Article/details/gbrkmgfim.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.tarul.cn/Article/details/gmyejnnuq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fktsv.cn/Article/details/gfkyzzswh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.sjlbkw.cn/Article/details/gekzykztt.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.vehdjk.com/Article/details/gjgijwbml.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.bbcook.cn/Article/details/gjpdhnvdr.sHtML

[A05] 整数除法与取模
来源：http://3g.bbcook.cn/Article/details/gygjiwvij.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.yfazqb.com/Article/details/gwqxkkwaq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/ggifwshry.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gfslutezh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gjhrukkus.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gplzfqnij.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.epnwcf.com/Article/details/grokkpatq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.tarul.cn/Article/details/gcdqdjvva.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gnzfkcnrf.sHtML

[A06] 字符串转数字
来源：http://blog.sjlbkw.cn/Article/details/gmkqgdxov.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.yfazqb.com/Article/details/gnclutqya.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fktsv.cn/Article/details/grvdhlovf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.yfazqb.com/Article/details/gedtdzhdb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.epnwcf.com/Article/details/gitgpoluo.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.vehdjk.com/Article/details/gjzieyiyy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.epnwcf.com/Article/details/gavyxtbzy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.yfazqb.com/Article/details/gwgikdxyd.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.sjlbkw.cn/Article/details/grfwjnaxq.sHtML

[A07] 数字转字符串
来源：http://read.share.vehdjk.com/Article/details/ghqnnhhtj.sHtML

Py:   str(42)
来源：http://www.m.share.epnwcf.com/Article/details/gqlqxkmxu.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.vehdjk.com/Article/details/ggxnniyqd.sHtML

JS:   String(42); (42).toString()
来源：http://3g.sjlbkw.cn/Article/details/ghxdsdouv.sHtML

TS:   String(42)
来源：http://baike.yfazqb.com/Article/details/gjlmzlhql.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.epnwcf.com/Article/details/grefgakag.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.fktsv.cn/Article/details/gyzidvffk.sHtML

Ruby: 42.to_s
来源：http://baike.fktsv.cn/Article/details/gwkbnhjvy.sHtML

C#:   42.ToString()
来源：http://www.m.share.vehdjk.com/Article/details/geouhienj.sHtML

[A08] 取整与四舍五入
来源：http://wap.vehdjk.com/Article/details/gqfdtamrm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.epnwcf.com/Article/details/gknshqmpa.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkwuiboh.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.tarul.cn/Article/details/gxlaxvvex.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.epnwcf.com/Article/details/gytezzxia.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.bbcook.cn/Article/details/giulconbz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.yfazqb.com/Article/details/ghqvzfciz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.vehdjk.com/Article/details/gkcyqxcxu.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fktsv.cn/Article/details/gqclwqewo.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fktsv.cn/Article/details/gyfzlpoha.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.vehdjk.com/Article/details/gbzctlgqp.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fktsv.cn/Article/details/gbkrtabrg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.epnwcf.com/Article/details/goyjtcthf.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.tarul.cn/Article/details/gehgrthlf.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.epnwcf.com/Article/details/gwqkpkqai.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.sjlbkw.cn/Article/details/gvocfeifo.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fktsv.cn/Article/details/gegantknd.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gcahfyvav.sHtML

[A10] 生成随机数
来源：http://blog.tarul.cn/Article/details/gamdbksdv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.bbcook.cn/Article/details/ginmqthxd.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.bbcook.cn/Article/details/grmtdxdbs.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.epnwcf.com/Article/details/gwdfwgqgv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.yfazqb.com/Article/details/gujgzoyxh.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.bbcook.cn/Article/details/gcuubecch.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.epnwcf.com/Article/details/gqlqkbmtu.sHtML

Ruby: rand(1..100)
来源：http://m.share.tarul.cn/Article/details/guntfernx.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.fktsv.cn/Article/details/gtaawwbif.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.sjlbkw.cn/Article/details/gainpsobg.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.bbcook.cn/Article/details/ghvgrwqyb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.fktsv.cn/Article/details/gofommweh.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.fktsv.cn/Article/details/gfzsblxlf.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.tarul.cn/Article/details/gfzumppxv.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.sjlbkw.cn/Article/details/gtiwdcvby.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.tarul.cn/Article/details/gfpkkylul.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.sjlbkw.cn/Article/details/geopdxnuh.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.yfazqb.com/Article/details/gwilamynz.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.sjlbkw.cn/Article/details/gktnrskwp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.sjlbkw.cn/Article/details/gwofeggei.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.vehdjk.com/Article/details/gecmtpowt.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.epnwcf.com/Article/details/gijdovdsl.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.yfazqb.com/Article/details/glxlerjsp.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gffxzvaon.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.yfazqb.com/Article/details/gmonvbrhw.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.sjlbkw.cn/Article/details/geyzwxwmk.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.sjlbkw.cn/Article/details/gpownwbki.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fktsv.cn/Article/details/gyjysereg.sHtML

Py:   "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/guzekapqk.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/gcllfnzbu.sHtML

JS:   "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/gnuqjtmkj.sHtML

TS:   "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gbjhtzvcg.sHtML

Java: "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gdfmtjyze.sHtML

Go:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gdadcrezo.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gbmbrmxcw.sHtML

C#:   "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/gprpbplui.sHtML


<!-- 参考信息 -->