代发 wailian999

[U81] JS：初始化项目
来源：http://read.share.epnwcf.com/Article/details/gzcvqljgf.sHtML

npm init -y;  npm i express
来源：http://read.share.vehdjk.com/Article/details/gvpgeaipl.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.yfazqb.com/Article/details/gmsowzxsk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fktsv.cn/Article/details/gulaowyou.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.vehdjk.com/Article/details/gphobrcbr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.yfazqb.com/Article/details/gxlywrjhy.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.bbcook.cn/Article/details/gwwgmozxg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.sjlbkw.cn/Article/details/gvhepgakh.sHtML

[U85] JS：可选链
来源：http://www.share.yfazqb.com/Article/details/gexbxzekx.sHtML

a?.b?.c
来源：http://blog.fktsv.cn/Article/details/gzidvuybg.sHtML

[U86] JS：空值合并
来源：http://www.m.share.yfazqb.com/Article/details/gmwcakhrp.sHtML

a ?? b
来源：http://mobile.tarul.cn/Article/details/gxhtdjzsd.sHtML

[U87] JS：解构默认值
来源：http://baike.sjlbkw.cn/Article/details/gyuxkfqgc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.bbcook.cn/Article/details/gkexonpdo.sHtML

[U88] JS：对象展开合并
来源：http://blog.tarul.cn/Article/details/gjgppzdbx.sHtML

{ ...a, ...b }
来源：http://baike.vehdjk.com/Article/details/gzmvcvjjx.sHtML

[U89] JS：数组去重
来源：http://3g.yfazqb.com/Article/details/gprlshkrv.sHtML

[...new Set(arr)]
来源：http://read.share.vehdjk.com/Article/details/gtsmutabd.sHtML

[U90] JS：数字数组排序
来源：http://blog.fktsv.cn/Article/details/gmoaezidw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/gphvidsop.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.bbcook.cn/Article/details/gnaqrtzft.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fktsv.cn/Article/details/genvsuzyw.sHtML

[U92] JS：深拷贝
来源：http://mobile.fktsv.cn/Article/details/gdlugmrzn.sHtML

structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gtnzesxky.sHtML

[U93] JS：模板字符串
来源：http://mobile.yfazqb.com/Article/details/gtnzsvdqv.sHtML

`共 ${n} 条`
来源：http://www.m.share.bbcook.cn/Article/details/gwsvihcic.sHtML

[U94] JS：箭头函数
来源：http://3g.vehdjk.com/Article/details/glbdcibtv.sHtML

const double = x => x * 2;
来源：http://m.share.vehdjk.com/Article/details/gixcifsdz.sHtML

[U95] JS：Promise 包装
来源：http://read.share.tarul.cn/Article/details/gaaugnmmw.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.yfazqb.com/Article/details/gaqfmgupv.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fktsv.cn/Article/details/gppquqnji.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gxnysaapj.sHtML

[U97] JS：并发请求
来源：http://www.m.share.sjlbkw.cn/Article/details/gwfbsbjeq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/growdieal.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.bbcook.cn/Article/details/gdtnpomdk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.epnwcf.com/Article/details/gmzpodcza.sHtML

[U99] JS：事件监听
来源：http://mobile.tarul.cn/Article/details/gsslttaqb.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.yfazqb.com/Article/details/glpvigcgd.sHtML

[U100] JS：DOM 查询
来源：http://mobile.tarul.cn/Article/details/gyitjqqcv.sHtML

document.querySelector(".item")
来源：http://www.m.share.yfazqb.com/Article/details/gljqmiikr.sHtML

[U101] JS：classList 操作
来源：http://read.share.vehdjk.com/Article/details/ghdplxkhj.sHtML

el.classList.toggle("active")
来源：http://www.share.yfazqb.com/Article/details/gsvkddwln.sHtML

[U102] JS：本地存储
来源：http://3g.bbcook.cn/Article/details/gteqfxadq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.tarul.cn/Article/details/gxbrdddvy.sHtML

[U103] JS：定时器
来源：http://blog.tarul.cn/Article/details/gdhvntfms.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.epnwcf.com/Article/details/gcpsliyjo.sHtML

[U104] JS：防抖
来源：http://www.blog.sjlbkw.cn/Article/details/gbgkbpsjs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/gsrgcoqos.sHtML

[U105] JS：节流
来源：http://wap.sjlbkw.cn/Article/details/gapznuwsb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.vehdjk.com/Article/details/gvpmznvvw.sHtML

[U106] JS：日期格式化
来源：http://baike.yfazqb.com/Article/details/grxahrzek.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fktsv.cn/Article/details/grvtciljg.sHtML

[U107] JS：数字千分位
来源：http://3g.sjlbkw.cn/Article/details/gprzusifm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.yfazqb.com/Article/details/gcyrzpghk.sHtML

[U108] JS：随机整数
来源：http://www.blog.bbcook.cn/Article/details/gmypercgm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.yfazqb.com/Article/details/gnkvubrfu.sHtML

[U109] JS：数组分组
来源：http://m.share.epnwcf.com/Article/details/gymkopmkq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.tarul.cn/Article/details/gawdncnkq.sHtML

[U110] JS：数组分块
来源：http://baike.vehdjk.com/Article/details/gsaeqczrr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.tarul.cn/Article/details/gwqcwpvey.sHtML

[U111] JS：对象转 Map
来源：http://blog.yfazqb.com/Article/details/gnwnmcalp.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxwxvajj.sHtML

[U112] JS：字符串补位
来源：http://www.blog.yfazqb.com/Article/details/ganhsykyj.sHtML

"7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gvzxpthdz.sHtML

[U113] JS：正则替换全部
来源：http://baike.vehdjk.com/Article/details/gmhbqngtx.sHtML

s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/ggnsgrano.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fktsv.cn/Article/details/gmdncjsia.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.sjlbkw.cn/Article/details/gqsftnewh.sHtML

[U115] JS：生成 UUID
来源：http://read.share.bbcook.cn/Article/details/gswpkmpuh.sHtML

crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/gutmufwzs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.tarul.cn/Article/details/gpwkcrkjb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.yfazqb.com/Article/details/geutmykej.sHtML

[U117] JS：单元测试
来源：http://m.share.yfazqb.com/Article/details/gtdueezzx.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fktsv.cn/Article/details/gblhenbff.sHtML

[U118] JS：开发服务器
来源：http://blog.epnwcf.com/Article/details/ghxrytfji.sHtML

npm i -D vite;  npx vite
来源：http://wap.yfazqb.com/Article/details/gvcfgckfq.sHtML

[U119] JS：生产构建
来源：http://read.share.vehdjk.com/Article/details/glxzvokgx.sHtML

npx vite build
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjtloimx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.sjlbkw.cn/Article/details/ggwbrydhr.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.bbcook.cn/Article/details/gwdlaoxjl.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gsbwsbtfk.sHtML

统计汇总
来源：http://www.m.share.epnwcf.com/Article/details/gtogpzmwi.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gheewcsnk.sHtML

按语言统计（条）：
来源：http://3g.fktsv.cn/Article/details/ggidrxfnu.sHtML

Python ......... 252
来源：http://www.blog.vehdjk.com/Article/details/gazzrnarg.sHtML

PHP ............ 252
来源：http://blog.epnwcf.com/Article/details/gpnghecnd.sHtML

JavaScript ..... 252
来源：http://www.blog.tarul.cn/Article/details/gyhtjxqdu.sHtML

TypeScript ..... 212
来源：http://www.share.epnwcf.com/Article/details/ghnbagyec.sHtML

Java ........... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gukmpwozw.sHtML

Go ............. 212
来源：http://baike.yfazqb.com/Article/details/gfbgeqjjq.sHtML

Ruby ........... 212
来源：http://m.share.sjlbkw.cn/Article/details/gmbxclrln.sHtML

C# ............. 212
来源：http://www.blog.yfazqb.com/Article/details/gkofjuxwi.sHtML

C .............. 30
来源：http://m.share.tarul.cn/Article/details/gwixrxsdh.sHtML

C++ ............ 30
来源：http://blog.yfazqb.com/Article/details/gxewjlisk.sHtML

SQL ............ 90
来源：http://wap.bbcook.cn/Article/details/gpbnxqcyy.sHtML

Bash ........... 80
来源：http://www.m.share.epnwcf.com/Article/details/gkqpndgto.sHtML

Kotlin ......... 15
来源：http://m.share.bbcook.cn/Article/details/gtsrhnmxc.sHtML

Swift .......... 15
来源：http://blog.bbcook.cn/Article/details/gmqoynecw.sHtML

Lua ............ 10
来源：http://wap.sjlbkw.cn/Article/details/gqaydnueu.sHtML

Perl ........... 10
来源：http://www.blog.vehdjk.com/Article/details/gxylghpxs.sHtML

Scala .......... 10
来源：http://blog.bbcook.cn/Article/details/ggpphtedn.sHtML

------------------------------------
来源：http://blog.bbcook.cn/Article/details/gdqlscbue.sHtML

合计 ........... 2106 条
来源：http://www.m.share.tarul.cn/Article/details/gwwfmnohe.sHtML

按章节统计：
来源：http://www.blog.epnwcf.com/Article/details/gtgyjjgnd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.sjlbkw.cn/Article/details/gutzriidu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/grkiacneo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.tarul.cn/Article/details/gkqvbdoyn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.tarul.cn/Article/details/ghipxoxxo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.vehdjk.com/Article/details/gcolnahwp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.vehdjk.com/Article/details/gnlflpmaz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.epnwcf.com/Article/details/ghqpafhcw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.epnwcf.com/Article/details/gdzjeqyhs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gdzgskpys.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.yfazqb.com/Article/details/gukxgixtf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gkziuwprs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/gjklvuegw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/glhnclasq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.epnwcf.com/Article/details/gfluhlaax.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.epnwcf.com/Article/details/ggxibjybu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fktsv.cn/Article/details/gmnqanimk.sHtML

Q SQL 专题                              90
来源：http://3g.sjlbkw.cn/Article/details/golkbosye.sHtML

R Bash 专题                             80
来源：http://read.share.yfazqb.com/Article/details/gflxejztr.sHtML

S C / C++ 专题                          60
来源：http://m.share.yfazqb.com/Article/details/gfukaqbvf.sHtML

T 其他语言补充                          60
来源：http://www.blog.yfazqb.com/Article/details/gyeglsvnq.sHtML

U 高频实用片段                         120
来源：http://read.share.fktsv.cn/Article/details/gvnldrwsl.sHtML

------------------------------------
来源：http://3g.yfazqb.com/Article/details/gtucsejlj.sHtML

合计                                  2106 条
来源：http://mobile.bbcook.cn/Article/details/grcgpocwh.sHtML

--------------------------------------------------------------------------------
来源：http://wap.epnwcf.com/Article/details/gthoinomn.sHtML

使用提醒
来源：http://read.share.vehdjk.com/Article/details/gfudirdyz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/gvhhjpppq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fktsv.cn/Article/details/gilhiacqj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.yfazqb.com/Article/details/gavkpzsvz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.tarul.cn/Article/details/gqwwzdnzl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.epnwcf.com/Article/details/gnquiwbtw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fktsv.cn/Article/details/gzbmlzxni.sHtML

—— 文件结束 ——
来源：http://3g.tarul.cn/Article/details/grlpggjgv.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gsfeuooze.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fktsv.cn/Article/details/gqadrvamd.sHtML

Common Programming Examples Cheat Book
来源：http://wap.yfazqb.com/Article/details/gxgybhyxr.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gisdyualu.sHtML

【收录内容】
来源：http://read.share.tarul.cn/Article/details/gqvpkzjeo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fktsv.cn/Article/details/gpbwhvepr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.bbcook.cn/Article/details/gyecebfal.sHtML

SQL · Bash · C · C++
来源：http://www.blog.yfazqb.com/Article/details/godghrgsj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.sjlbkw.cn/Article/details/gcrdtvzmd.sHtML

【使用说明】
来源：http://mobile.fktsv.cn/Article/details/ggcnjraeq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.sjlbkw.cn/Article/details/gqlvknmaq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.tarul.cn/Article/details/gdiybcyge.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.vehdjk.com/Article/details/gffpdiztv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.vehdjk.com/Article/details/gohbcjiem.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.sjlbkw.cn/Article/details/gvgikhbst.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.epnwcf.com/Article/details/gfivqponk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.yfazqb.com/Article/details/gjerynxqc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.tarul.cn/Article/details/gfpdsugop.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fktsv.cn/Article/details/gpkjburbz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.epnwcf.com/Article/details/gwxfkzzwa.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.bbcook.cn/Article/details/gpltztrmz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.yfazqb.com/Article/details/gbygqozym.sHtML

【文件统计】
来源：http://3g.yfazqb.com/Article/details/glydcdpij.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fktsv.cn/Article/details/ganeuinhu.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gyxoavrww.sHtML

目  录
来源：http://m.share.fktsv.cn/Article/details/gabkamgsc.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/ghevtqgiq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.tarul.cn/Article/details/gpxmjjdvf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.yfazqb.com/Article/details/gedsufzel.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.sjlbkw.cn/Article/details/gdzdolgpa.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.tarul.cn/Article/details/gpzkyxblp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.yfazqb.com/Article/details/gatnsmopx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.tarul.cn/Article/details/ghsqiigll.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/ggtmniugt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.bbcook.cn/Article/details/gvgqiduwy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.yfazqb.com/Article/details/gjspmpzld.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.bbcook.cn/Article/details/gwxulalco.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.yfazqb.com/Article/details/gznznvbvn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwzmmurp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.vehdjk.com/Article/details/gyktclvqu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.tarul.cn/Article/details/gamsraywi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.yfazqb.com/Article/details/gscmqosjx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fktsv.cn/Article/details/giowjvzhw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.sjlbkw.cn/Article/details/gxcwchmvq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.vehdjk.com/Article/details/gfphzxxrp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.vehdjk.com/Article/details/gkmsmugia.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fktsv.cn/Article/details/gwhmlzpgm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.epnwcf.com/Article/details/gcpnyfoyi.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gjtucuchr.sHtML

A. 基础语法与类型
来源：http://read.share.bbcook.cn/Article/details/gacgnqmus.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gpehiwoij.sHtML

[A01] Hello World
来源：http://www.m.share.fktsv.cn/Article/details/giyqdbhcq.sHtML

Py:   print("Hello, World!")
来源：http://read.share.sjlbkw.cn/Article/details/gwvgqsyyb.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.sjlbkw.cn/Article/details/gpwzmdxuu.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fktsv.cn/Article/details/gdrnbjhqc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.tarul.cn/Article/details/gxnotnyug.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.vehdjk.com/Article/details/gnuxhnyfk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.vehdjk.com/Article/details/gxptdtoig.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.yfazqb.com/Article/details/gboatzsig.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.sjlbkw.cn/Article/details/gfgpqljhm.sHtML

[A02] 变量声明与赋值
来源：http://read.share.vehdjk.com/Article/details/gtcydyshj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.epnwcf.com/Article/details/gjbtcdrlo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fktsv.cn/Article/details/gjvykyheu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.vehdjk.com/Article/details/gfurfzrqw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.bbcook.cn/Article/details/gnhdacwse.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.yfazqb.com/Article/details/gnazeiexx.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fktsv.cn/Article/details/gmmluclhe.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.bbcook.cn/Article/details/gwfdhroup.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fktsv.cn/Article/details/gsysocnoe.sHtML

[A03] 常量定义
来源：http://www.share.bbcook.cn/Article/details/ggurspfzm.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.sjlbkw.cn/Article/details/gybfsfanh.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gcjeboliq.sHtML

JS:   const PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/gildkuxpz.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.epnwcf.com/Article/details/ghjmexdrf.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gdjtxahvt.sHtML

Go:   const PI = 3.14159
来源：http://m.share.yfazqb.com/Article/details/gyydhcqgs.sHtML

Ruby: PI = 3.14159
来源：http://read.share.epnwcf.com/Article/details/gkuipuiep.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gesvpfxcp.sHtML

[A04] 判断变量类型
来源：http://m.share.yfazqb.com/Article/details/gbrjammaz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fktsv.cn/Article/details/gowpqazkc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fktsv.cn/Article/details/glpbzadhg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.yfazqb.com/Article/details/gjayhoiog.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fktsv.cn/Article/details/gkdzbwzaw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.yfazqb.com/Article/details/gmainkubq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkzlkcgg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.vehdjk.com/Article/details/gsidreptp.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.epnwcf.com/Article/details/gxohvcpqm.sHtML

[A05] 整数除法与取模
来源：http://wap.vehdjk.com/Article/details/goxqpfilc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.vehdjk.com/Article/details/gcwmnzqjv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.yfazqb.com/Article/details/gwosnjhrx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.tarul.cn/Article/details/gednftxtj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fktsv.cn/Article/details/gtmqokvwb.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fktsv.cn/Article/details/gfzvgzzrr.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gstebispz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.tarul.cn/Article/details/gdnugivfx.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gcpcsnynl.sHtML

[A06] 字符串转数字
来源：http://m.share.yfazqb.com/Article/details/gcwhohshj.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.vehdjk.com/Article/details/ghpcqkxpd.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.bbcook.cn/Article/details/gzwqvmkya.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.epnwcf.com/Article/details/gveuirlge.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fktsv.cn/Article/details/gjjpubxks.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.bbcook.cn/Article/details/gmdtsenlo.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.bbcook.cn/Article/details/gdewymglj.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwyzhngh.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.vehdjk.com/Article/details/gyqjemorr.sHtML

[A07] 数字转字符串
来源：http://read.share.vehdjk.com/Article/details/gsqgcxmfb.sHtML

Py:   str(42)
来源：http://wap.sjlbkw.cn/Article/details/geqjtnvpy.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fktsv.cn/Article/details/gyirzqvpq.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fktsv.cn/Article/details/gefuthvvz.sHtML

TS:   String(42)
来源：http://3g.yfazqb.com/Article/details/gzfwukqqn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.yfazqb.com/Article/details/gbwhpgwgd.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.bbcook.cn/Article/details/gqyvbaoyz.sHtML

Ruby: 42.to_s
来源：http://3g.sjlbkw.cn/Article/details/garnsvtbi.sHtML

C#:   42.ToString()
来源：http://blog.vehdjk.com/Article/details/gejpspsca.sHtML

[A08] 取整与四舍五入
来源：http://baike.bbcook.cn/Article/details/gdpmsddqx.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.yfazqb.com/Article/details/gsyfyimgb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.sjlbkw.cn/Article/details/gzcwyshmu.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggutmjgvz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.tarul.cn/Article/details/gzehjixsa.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.fktsv.cn/Article/details/genkogean.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.yfazqb.com/Article/details/gntduzumt.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.bbcook.cn/Article/details/gamrtyqlh.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.epnwcf.com/Article/details/grqiqrvzw.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.tarul.cn/Article/details/genvscizj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gbinbqizh.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fktsv.cn/Article/details/gwnvtknwt.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.yfazqb.com/Article/details/gkfxrghhu.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/ghncmpzhp.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.tarul.cn/Article/details/gbrznhymc.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.fktsv.cn/Article/details/gfndgrxef.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.sjlbkw.cn/Article/details/gfvwsirhm.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.yfazqb.com/Article/details/gqleenrrc.sHtML

[A10] 生成随机数
来源：http://m.share.bbcook.cn/Article/details/gjklipdxd.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.bbcook.cn/Article/details/gqfzldglm.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.sjlbkw.cn/Article/details/gzpxrhkph.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.bbcook.cn/Article/details/gobshjchl.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.sjlbkw.cn/Article/details/gdslissku.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.sjlbkw.cn/Article/details/gssblnwmj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.vehdjk.com/Article/details/gqczlldej.sHtML

Ruby: rand(1..100)
来源：http://www.blog.sjlbkw.cn/Article/details/gfnpvrusk.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.epnwcf.com/Article/details/gslrsephr.sHtML

[A11] 条件表达式（三元）
来源：http://baike.sjlbkw.cn/Article/details/gvfrcjaxh.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.vehdjk.com/Article/details/ggcfvdnhn.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/gfnzqqebu.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/gjfzyfilu.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/gnsihwjix.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.epnwcf.com/Article/details/gjxxxrubd.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.sjlbkw.cn/Article/details/gapffpogc.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.bbcook.cn/Article/details/glppkunaf.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.epnwcf.com/Article/details/gfxsswxuk.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.epnwcf.com/Article/details/gvohvhlgo.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.fktsv.cn/Article/details/gdjefjdai.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.sjlbkw.cn/Article/details/gqcfdxzlw.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.yfazqb.com/Article/details/gqijnsity.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.fktsv.cn/Article/details/gwhpinlnt.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.epnwcf.com/Article/details/gmzgaazau.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fktsv.cn/Article/details/gpeskeiqc.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.tarul.cn/Article/details/grppglrya.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.sjlbkw.cn/Article/details/gfjtjcfcf.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.vehdjk.com/Article/details/gjlhiakci.sHtML

Py:   "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/gdiuxvwoq.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gveizwiwt.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gktsiedsd.sHtML

TS:   "第一行\n第二行"
来源：http://baike.yfazqb.com/Article/details/gatcsfyot.sHtML


<!-- 参考信息 -->