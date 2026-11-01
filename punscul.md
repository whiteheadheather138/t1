代发 wailian999

[U81] JS：初始化项目
来源：http://www.blog.tarul.cn/Article/details/gmfdmtrbh.sHtML

npm init -y;  npm i express
来源：http://baike.sjlbkw.cn/Article/details/gdyhglava.sHtML

[U82] JS：package.json 脚本
来源：http://wap.tarul.cn/Article/details/gscjhodtx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.yfazqb.com/Article/details/gywcqlepw.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.tarul.cn/Article/details/gofnkvimh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fktsv.cn/Article/details/gpbkfbohw.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.tarul.cn/Article/details/gvlbxcwwx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.tarul.cn/Article/details/gdhtajtrg.sHtML

[U85] JS：可选链
来源：http://m.share.yfazqb.com/Article/details/gybfebmtr.sHtML

a?.b?.c
来源：http://3g.fktsv.cn/Article/details/gikbkejoc.sHtML

[U86] JS：空值合并
来源：http://blog.sjlbkw.cn/Article/details/gysknqqfj.sHtML

a ?? b
来源：http://baike.tarul.cn/Article/details/gfjyloxsm.sHtML

[U87] JS：解构默认值
来源：http://www.share.tarul.cn/Article/details/gzbxuekim.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.yfazqb.com/Article/details/gyyqxwnii.sHtML

[U88] JS：对象展开合并
来源：http://3g.sjlbkw.cn/Article/details/glkuwpkvp.sHtML

{ ...a, ...b }
来源：http://www.m.share.vehdjk.com/Article/details/gyjdfcecp.sHtML

[U89] JS：数组去重
来源：http://www.share.tarul.cn/Article/details/gwnokwlum.sHtML

[...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gloqfkdwt.sHtML

[U90] JS：数字数组排序
来源：http://3g.fktsv.cn/Article/details/gbvatlhzt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/gbrpnodao.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.epnwcf.com/Article/details/gyyhnadfv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.tarul.cn/Article/details/gzjopuxqg.sHtML

[U92] JS：深拷贝
来源：http://wap.sjlbkw.cn/Article/details/gmldlggme.sHtML

structuredClone(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gufqhayqg.sHtML

[U93] JS：模板字符串
来源：http://baike.bbcook.cn/Article/details/gbbewugxp.sHtML

`共 ${n} 条`
来源：http://baike.fktsv.cn/Article/details/gcfevafia.sHtML

[U94] JS：箭头函数
来源：http://m.share.vehdjk.com/Article/details/gcygztuut.sHtML

const double = x => x * 2;
来源：http://read.share.tarul.cn/Article/details/gendcames.sHtML

[U95] JS：Promise 包装
来源：http://blog.bbcook.cn/Article/details/gesyqnocl.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.vehdjk.com/Article/details/gmzkfhnki.sHtML

[U96] JS：async/await 与异常
来源：http://baike.yfazqb.com/Article/details/gxmpgpuxy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/gaglzgiwr.sHtML

[U97] JS：并发请求
来源：http://baike.vehdjk.com/Article/details/gpsrczlfd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gfkffsehj.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.epnwcf.com/Article/details/gvbdnsgiw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.tarul.cn/Article/details/gqwxdnuny.sHtML

[U99] JS：事件监听
来源：http://www.share.sjlbkw.cn/Article/details/gzkwxfdhu.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.bbcook.cn/Article/details/gfjdihwxq.sHtML

[U100] JS：DOM 查询
来源：http://blog.tarul.cn/Article/details/goemylitn.sHtML

document.querySelector(".item")
来源：http://read.share.vehdjk.com/Article/details/gwenpszzy.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.vehdjk.com/Article/details/glvnkmdvh.sHtML

el.classList.toggle("active")
来源：http://blog.yfazqb.com/Article/details/gaebzqxqr.sHtML

[U102] JS：本地存储
来源：http://blog.bbcook.cn/Article/details/gqzoegrmy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.sjlbkw.cn/Article/details/gbwosjxpu.sHtML

[U103] JS：定时器
来源：http://m.share.yfazqb.com/Article/details/ghdvmikww.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.tarul.cn/Article/details/gzwwyoxux.sHtML

[U104] JS：防抖
来源：http://read.share.bbcook.cn/Article/details/gnpwhrwbg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/gcgkdzmcw.sHtML

[U105] JS：节流
来源：http://read.share.sjlbkw.cn/Article/details/gqzqcqahu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.epnwcf.com/Article/details/gxtgxtrya.sHtML

[U106] JS：日期格式化
来源：http://www.share.epnwcf.com/Article/details/gpfkmjybq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fktsv.cn/Article/details/gizxronqp.sHtML

[U107] JS：数字千分位
来源：http://wap.bbcook.cn/Article/details/gyzhujgbk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.epnwcf.com/Article/details/ghgsunlyo.sHtML

[U108] JS：随机整数
来源：http://mobile.vehdjk.com/Article/details/gpkegizvx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.yfazqb.com/Article/details/gvnxweetk.sHtML

[U109] JS：数组分组
来源：http://wap.tarul.cn/Article/details/gdahylbop.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.epnwcf.com/Article/details/ggflgqdrk.sHtML

[U110] JS：数组分块
来源：http://www.share.vehdjk.com/Article/details/gsizogmiu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.yfazqb.com/Article/details/glfwykchp.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.tarul.cn/Article/details/gsylnszqv.sHtML

new Map(Object.entries(obj))
来源：http://blog.epnwcf.com/Article/details/guesgcrsw.sHtML

[U112] JS：字符串补位
来源：http://read.share.yfazqb.com/Article/details/givpldjle.sHtML

"7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gusjgvhgh.sHtML

[U113] JS：正则替换全部
来源：http://www.share.bbcook.cn/Article/details/ghlmoixfn.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gotkczqir.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.vehdjk.com/Article/details/gxmeqlesj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.epnwcf.com/Article/details/gqscftxud.sHtML

[U115] JS：生成 UUID
来源：http://m.share.vehdjk.com/Article/details/glasihzba.sHtML

crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gdafcrnjd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.vehdjk.com/Article/details/gjnqsumwv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fktsv.cn/Article/details/gfvebomwv.sHtML

[U117] JS：单元测试
来源：http://wap.bbcook.cn/Article/details/giuceumny.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.epnwcf.com/Article/details/gygdybrdz.sHtML

[U118] JS：开发服务器
来源：http://blog.vehdjk.com/Article/details/gugvjxkuz.sHtML

npm i -D vite;  npx vite
来源：http://read.share.epnwcf.com/Article/details/ghzssxoav.sHtML

[U119] JS：生产构建
来源：http://read.share.fktsv.cn/Article/details/gfhrpnyes.sHtML

npx vite build
来源：http://www.m.share.bbcook.cn/Article/details/gbvdbaapu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.yfazqb.com/Article/details/glrfxasgs.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.sjlbkw.cn/Article/details/gwsucuowb.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ghwthnluv.sHtML

统计汇总
来源：http://m.share.yfazqb.com/Article/details/grpzeudga.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gcwnzllot.sHtML

按语言统计（条）：
来源：http://wap.tarul.cn/Article/details/goovbzhbf.sHtML

Python ......... 252
来源：http://read.share.sjlbkw.cn/Article/details/glgyhndko.sHtML

PHP ............ 252
来源：http://baike.fktsv.cn/Article/details/gmawtjija.sHtML

JavaScript ..... 252
来源：http://www.m.share.epnwcf.com/Article/details/grgmhrnul.sHtML

TypeScript ..... 212
来源：http://read.share.vehdjk.com/Article/details/gholhmxuw.sHtML

Java ........... 212
来源：http://baike.yfazqb.com/Article/details/gyjoxwskl.sHtML

Go ............. 212
来源：http://wap.bbcook.cn/Article/details/genuuvqsl.sHtML

Ruby ........... 212
来源：http://mobile.tarul.cn/Article/details/gddappbua.sHtML

C# ............. 212
来源：http://www.blog.bbcook.cn/Article/details/gzinxtcnr.sHtML

C .............. 30
来源：http://www.share.sjlbkw.cn/Article/details/gvaiqpgxp.sHtML

C++ ............ 30
来源：http://www.blog.sjlbkw.cn/Article/details/gxmndidvd.sHtML

SQL ............ 90
来源：http://baike.vehdjk.com/Article/details/gnmfszgsg.sHtML

Bash ........... 80
来源：http://mobile.epnwcf.com/Article/details/gqujczvug.sHtML

Kotlin ......... 15
来源：http://3g.yfazqb.com/Article/details/gdonqgxma.sHtML

Swift .......... 15
来源：http://www.m.share.fktsv.cn/Article/details/gbaovhtmj.sHtML

Lua ............ 10
来源：http://m.share.vehdjk.com/Article/details/gseivdmzb.sHtML

Perl ........... 10
来源：http://www.m.share.epnwcf.com/Article/details/gbzzhqcay.sHtML

Scala .......... 10
来源：http://www.share.yfazqb.com/Article/details/goksgumfq.sHtML

------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gdmxkncnu.sHtML

合计 ........... 2106 条
来源：http://baike.fktsv.cn/Article/details/gxkkwhhsp.sHtML

按章节统计：
来源：http://wap.yfazqb.com/Article/details/giwzpnsni.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.yfazqb.com/Article/details/gbsbbmyth.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fktsv.cn/Article/details/gjyqzycfe.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fktsv.cn/Article/details/gqdqhusme.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.yfazqb.com/Article/details/gnogxfnlf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fktsv.cn/Article/details/gjrsrccvf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.vehdjk.com/Article/details/gjfziwosm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fktsv.cn/Article/details/gteqkjeto.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.tarul.cn/Article/details/guvajhkam.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gkwksynjj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.yfazqb.com/Article/details/gkpvpopzi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/gocecrhrc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/gduuaucgp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/gpiwdehjm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fktsv.cn/Article/details/giuuwqsuf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fktsv.cn/Article/details/gdimykurk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gtebxfjet.sHtML

Q SQL 专题                              90
来源：http://www.blog.yfazqb.com/Article/details/gphnctgbw.sHtML

R Bash 专题                             80
来源：http://www.blog.tarul.cn/Article/details/gddaiabsm.sHtML

S C / C++ 专题                          60
来源：http://www.blog.vehdjk.com/Article/details/guvranwop.sHtML

T 其他语言补充                          60
来源：http://www.share.bbcook.cn/Article/details/gzpgxnjys.sHtML

U 高频实用片段                         120
来源：http://wap.vehdjk.com/Article/details/gnthhvwzb.sHtML

------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gvzxomglk.sHtML

合计                                  2106 条
来源：http://baike.bbcook.cn/Article/details/gjfcydvkt.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gqdmfehfm.sHtML

使用提醒
来源：http://3g.yfazqb.com/Article/details/gprzpratc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/giofncqmu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.vehdjk.com/Article/details/grxwciiqp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.tarul.cn/Article/details/glpqofggq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.vehdjk.com/Article/details/goqopfurw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.sjlbkw.cn/Article/details/gjvxzawak.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.epnwcf.com/Article/details/gvazrzmhn.sHtML

—— 文件结束 ——
来源：http://wap.bbcook.cn/Article/details/gpmkqwrmu.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gvmmstjsd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fktsv.cn/Article/details/gscmqgqhg.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.bbcook.cn/Article/details/gsokncblr.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/geszspyrf.sHtML

【收录内容】
来源：http://www.m.share.tarul.cn/Article/details/gbujmomui.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.yfazqb.com/Article/details/ggmsdndxr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.sjlbkw.cn/Article/details/guuyogloq.sHtML

SQL · Bash · C · C++
来源：http://blog.tarul.cn/Article/details/genxhtaxr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.epnwcf.com/Article/details/gjcwbkgee.sHtML

【使用说明】
来源：http://wap.sjlbkw.cn/Article/details/gozwdtcao.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.yfazqb.com/Article/details/gqthqgatx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.sjlbkw.cn/Article/details/ghftbdzey.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.yfazqb.com/Article/details/gqfkmzxfc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fktsv.cn/Article/details/gbhdbcute.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.yfazqb.com/Article/details/guwjajjiu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.sjlbkw.cn/Article/details/geolqqdga.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.epnwcf.com/Article/details/glrfsnyew.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.bbcook.cn/Article/details/gujqyxivk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.tarul.cn/Article/details/gojhggrgk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.tarul.cn/Article/details/gmiuhhaey.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.epnwcf.com/Article/details/gorcmpdxi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.bbcook.cn/Article/details/gfgwrkbgg.sHtML

【文件统计】
来源：http://www.m.share.bbcook.cn/Article/details/guuyeptxt.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.tarul.cn/Article/details/gdcyzgjux.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/ghgdcmnhm.sHtML

目  录
来源：http://3g.tarul.cn/Article/details/gvbdcxzmb.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.tarul.cn/Article/details/gqnqdccuz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.yfazqb.com/Article/details/giocfhpry.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fktsv.cn/Article/details/gdcnxnbtl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.bbcook.cn/Article/details/gdhoyenyp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.yfazqb.com/Article/details/gnhsiyrfs.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.vehdjk.com/Article/details/glfpiueya.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.epnwcf.com/Article/details/gehmwoupc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.vehdjk.com/Article/details/gewowvgya.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.tarul.cn/Article/details/gvbjgzipq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/gosugeybf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.yfazqb.com/Article/details/gcuaqmgkz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gavwkdrdm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gsubdikny.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/gkxmvvdvc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.bbcook.cn/Article/details/gcubhptpq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.vehdjk.com/Article/details/gzreyhtdk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/grmirsmbs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.tarul.cn/Article/details/gzbicoonu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbaczwlm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.vehdjk.com/Article/details/gbgvdgrmi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.tarul.cn/Article/details/gxviexxkz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.vehdjk.com/Article/details/gerfiomjh.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gvbjmkcza.sHtML

A. 基础语法与类型
来源：http://wap.tarul.cn/Article/details/gwpypjdkl.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ghfzcezau.sHtML

[A01] Hello World
来源：http://www.share.fktsv.cn/Article/details/guihldews.sHtML

Py:   print("Hello, World!")
来源：http://read.share.epnwcf.com/Article/details/gqpeuibps.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fktsv.cn/Article/details/gcmcuvfiz.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.sjlbkw.cn/Article/details/grbhdljtm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fktsv.cn/Article/details/grxvilekx.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.sjlbkw.cn/Article/details/gsilingkv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.tarul.cn/Article/details/gczjhryar.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.sjlbkw.cn/Article/details/gmhediyyn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.sjlbkw.cn/Article/details/geqshtzqy.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.tarul.cn/Article/details/gogigoogz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fktsv.cn/Article/details/gklrtuyai.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.tarul.cn/Article/details/gmviczhsp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fktsv.cn/Article/details/gshybbdkp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fktsv.cn/Article/details/gtzogehwn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.bbcook.cn/Article/details/gxysygfrr.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.epnwcf.com/Article/details/gsioyrnto.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.bbcook.cn/Article/details/gxechprtl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.tarul.cn/Article/details/gwqbdtutq.sHtML

[A03] 常量定义
来源：http://3g.sjlbkw.cn/Article/details/ginjhjkse.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.epnwcf.com/Article/details/gpqynvxun.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gauzowkmo.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gcnaqmabr.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.epnwcf.com/Article/details/grshlofdy.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gjldftgwp.sHtML

Go:   const PI = 3.14159
来源：http://read.share.bbcook.cn/Article/details/ggaukbdqb.sHtML

Ruby: PI = 3.14159
来源：http://wap.sjlbkw.cn/Article/details/gkhmzuwaq.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnmnmdmn.sHtML

[A04] 判断变量类型
来源：http://www.share.yfazqb.com/Article/details/ggwwymksf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.yfazqb.com/Article/details/guregxqds.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.tarul.cn/Article/details/gjfpgtsmn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.bbcook.cn/Article/details/gealgleay.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.tarul.cn/Article/details/gpabkmemb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.yfazqb.com/Article/details/gpkfjgwep.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.tarul.cn/Article/details/gvrdibnjq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.epnwcf.com/Article/details/gphffzivm.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.vehdjk.com/Article/details/ghaphpcev.sHtML

[A05] 整数除法与取模
来源：http://read.share.epnwcf.com/Article/details/gwhlktoty.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fktsv.cn/Article/details/gafmplcvq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gswgttptm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/gnkxdxsrn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gyninrrbc.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.bbcook.cn/Article/details/ghxagalqr.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.tarul.cn/Article/details/gpgnnuyjr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gcrpojuuh.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.vehdjk.com/Article/details/gtnikhebx.sHtML

[A06] 字符串转数字
来源：http://m.share.vehdjk.com/Article/details/gucyzzhja.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fktsv.cn/Article/details/gitxbfjev.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.epnwcf.com/Article/details/gcgqhffbg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.vehdjk.com/Article/details/ghnhrmpih.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.vehdjk.com/Article/details/gowvmyfcj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.sjlbkw.cn/Article/details/gbpzvjexi.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.epnwcf.com/Article/details/gglhwuvke.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.sjlbkw.cn/Article/details/gezsbozgh.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.yfazqb.com/Article/details/gpsxbamij.sHtML

[A07] 数字转字符串
来源：http://baike.sjlbkw.cn/Article/details/gzquzuhlj.sHtML

Py:   str(42)
来源：http://blog.epnwcf.com/Article/details/gomegjwdi.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.yfazqb.com/Article/details/ggoghgspx.sHtML

JS:   String(42); (42).toString()
来源：http://3g.vehdjk.com/Article/details/gwyafdktz.sHtML

TS:   String(42)
来源：http://3g.vehdjk.com/Article/details/gvjvccipo.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.yfazqb.com/Article/details/gueccnbfw.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.bbcook.cn/Article/details/glhzcekgr.sHtML

Ruby: 42.to_s
来源：http://www.m.share.yfazqb.com/Article/details/gqgjxfvdx.sHtML

C#:   42.ToString()
来源：http://mobile.tarul.cn/Article/details/gnxtfxmvr.sHtML

[A08] 取整与四舍五入
来源：http://read.share.bbcook.cn/Article/details/gtgkevmdd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fktsv.cn/Article/details/gjsinudsb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.epnwcf.com/Article/details/gdkisjstx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.bbcook.cn/Article/details/gqhwwetjt.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fktsv.cn/Article/details/gsdmmiqek.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.sjlbkw.cn/Article/details/gnxvwkpxq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.epnwcf.com/Article/details/gfucotjmm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.epnwcf.com/Article/details/gwxbtjknn.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.sjlbkw.cn/Article/details/gwzvtdjzg.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.yfazqb.com/Article/details/gyiyoafse.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gclaqoceu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.tarul.cn/Article/details/gmvlajonm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fktsv.cn/Article/details/gdvefaqha.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.yfazqb.com/Article/details/gjqibcnkv.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.tarul.cn/Article/details/gknomgihe.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fktsv.cn/Article/details/gnolsyudj.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.yfazqb.com/Article/details/gvfkxvspc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gztqmwqrn.sHtML

[A10] 生成随机数
来源：http://blog.sjlbkw.cn/Article/details/gbapfgrex.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.sjlbkw.cn/Article/details/gdkkkpnas.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.tarul.cn/Article/details/gmqvveozw.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.yfazqb.com/Article/details/gczorxond.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.yfazqb.com/Article/details/gqsjzdoxx.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.epnwcf.com/Article/details/ggfmfpfdv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.epnwcf.com/Article/details/gnlddzxzn.sHtML

Ruby: rand(1..100)
来源：http://www.blog.yfazqb.com/Article/details/gkhymnfqy.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.fktsv.cn/Article/details/gbcmgmmxd.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.yfazqb.com/Article/details/gpxxefmrr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.yfazqb.com/Article/details/gyxkzrwyc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.sjlbkw.cn/Article/details/gqinhsymz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.tarul.cn/Article/details/gkmzozvwx.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.tarul.cn/Article/details/gecxoqzgy.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.sjlbkw.cn/Article/details/gpxdlpbbm.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.fktsv.cn/Article/details/glacmlyno.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.fktsv.cn/Article/details/guklkiuuu.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/giitbknwc.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.vehdjk.com/Article/details/gckxjmkui.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.sjlbkw.cn/Article/details/gxyfzokzs.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.tarul.cn/Article/details/gvtpkhumd.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.bbcook.cn/Article/details/gclfuidau.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.tarul.cn/Article/details/gpgiynsft.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.fktsv.cn/Article/details/gxihzkplc.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.vehdjk.com/Article/details/gamdmjuao.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.sjlbkw.cn/Article/details/gtacajlzj.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.yfazqb.com/Article/details/gekppqtyo.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.yfazqb.com/Article/details/gyeweskos.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gfpwqjavf.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/gfdkspcgi.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/gwrxjkcju.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/gtcwfyzwb.sHtML


<!-- 参考信息 -->