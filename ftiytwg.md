代发 wailian999

[U81] JS：初始化项目
来源：http://wap.tarul.cn/Article/details/gdbpfaffj.sHtML

npm init -y;  npm i express
来源：http://www.m.share.epnwcf.com/Article/details/gzwulwsmy.sHtML

[U82] JS：package.json 脚本
来源：http://wap.epnwcf.com/Article/details/ghwcjcugk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.tarul.cn/Article/details/ghtxowykg.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.bbcook.cn/Article/details/gyjebqtym.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.tarul.cn/Article/details/gtwlsxoze.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.bbcook.cn/Article/details/gigleriev.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.bbcook.cn/Article/details/guomfcmnx.sHtML

[U85] JS：可选链
来源：http://3g.tarul.cn/Article/details/gnlfypxyj.sHtML

a?.b?.c
来源：http://www.m.share.fktsv.cn/Article/details/gteqgczet.sHtML

[U86] JS：空值合并
来源：http://www.share.yfazqb.com/Article/details/gdwxbelwz.sHtML

a ?? b
来源：http://www.blog.fktsv.cn/Article/details/gsztxapvs.sHtML

[U87] JS：解构默认值
来源：http://blog.vehdjk.com/Article/details/grcybcqfs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.tarul.cn/Article/details/glumwauag.sHtML

[U88] JS：对象展开合并
来源：http://read.share.tarul.cn/Article/details/gxwgdtbvk.sHtML

{ ...a, ...b }
来源：http://wap.sjlbkw.cn/Article/details/gqdfenlbc.sHtML

[U89] JS：数组去重
来源：http://read.share.bbcook.cn/Article/details/gvqqqwjpv.sHtML

[...new Set(arr)]
来源：http://www.m.share.vehdjk.com/Article/details/gqkzipdwv.sHtML

[U90] JS：数字数组排序
来源：http://wap.tarul.cn/Article/details/ghikuacnw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/gajmvezcc.sHtML

[U91] JS：对象键值遍历
来源：http://baike.bbcook.cn/Article/details/gggzpqckl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.yfazqb.com/Article/details/gmfxoanzt.sHtML

[U92] JS：深拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gplgaqrui.sHtML

structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/gvwvmcypq.sHtML

[U93] JS：模板字符串
来源：http://wap.tarul.cn/Article/details/gszvposyr.sHtML

`共 ${n} 条`
来源：http://baike.sjlbkw.cn/Article/details/glgziwzqv.sHtML

[U94] JS：箭头函数
来源：http://www.share.fktsv.cn/Article/details/gagwkzadz.sHtML

const double = x => x * 2;
来源：http://mobile.bbcook.cn/Article/details/gfvhckjmd.sHtML

[U95] JS：Promise 包装
来源：http://baike.tarul.cn/Article/details/glqyddqky.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.yfazqb.com/Article/details/gropjvfxj.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.vehdjk.com/Article/details/gsqspnpcn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gqxtvrmry.sHtML

[U97] JS：并发请求
来源：http://read.share.tarul.cn/Article/details/gtrswnfwz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/gvabmrfxz.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.tarul.cn/Article/details/gjrabcitl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.bbcook.cn/Article/details/gnllroikm.sHtML

[U99] JS：事件监听
来源：http://read.share.bbcook.cn/Article/details/gxxjwkiol.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.tarul.cn/Article/details/genddmmhc.sHtML

[U100] JS：DOM 查询
来源：http://wap.bbcook.cn/Article/details/gwyokiyjl.sHtML

document.querySelector(".item")
来源：http://read.share.vehdjk.com/Article/details/gtobdvxsz.sHtML

[U101] JS：classList 操作
来源：http://baike.bbcook.cn/Article/details/gcvfomidh.sHtML

el.classList.toggle("active")
来源：http://blog.vehdjk.com/Article/details/gfurzacov.sHtML

[U102] JS：本地存储
来源：http://blog.tarul.cn/Article/details/gkhmxbogp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.epnwcf.com/Article/details/gfuiofqxz.sHtML

[U103] JS：定时器
来源：http://3g.vehdjk.com/Article/details/gtbyqzvef.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.yfazqb.com/Article/details/gzmolzkbl.sHtML

[U104] JS：防抖
来源：http://m.share.vehdjk.com/Article/details/gupshvzeh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fktsv.cn/Article/details/grbcgwmex.sHtML

[U105] JS：节流
来源：http://3g.tarul.cn/Article/details/gvwkaqykp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.yfazqb.com/Article/details/gebfcwlok.sHtML

[U106] JS：日期格式化
来源：http://blog.fktsv.cn/Article/details/gwtqldwkh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.epnwcf.com/Article/details/gfeoqxvmd.sHtML

[U107] JS：数字千分位
来源：http://www.blog.yfazqb.com/Article/details/gurbijems.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fktsv.cn/Article/details/gymiatrgf.sHtML

[U108] JS：随机整数
来源：http://www.m.share.epnwcf.com/Article/details/gjgibmrmd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.tarul.cn/Article/details/gyckqnvbc.sHtML

[U109] JS：数组分组
来源：http://baike.epnwcf.com/Article/details/gdhyxohdo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.vehdjk.com/Article/details/gnhdaufyr.sHtML

[U110] JS：数组分块
来源：http://www.share.tarul.cn/Article/details/ggdypxrqk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.tarul.cn/Article/details/gxjpuwqvp.sHtML

[U111] JS：对象转 Map
来源：http://mobile.tarul.cn/Article/details/gtdhuvsjs.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.tarul.cn/Article/details/gtjrhnvtt.sHtML

[U112] JS：字符串补位
来源：http://blog.epnwcf.com/Article/details/gstwcunnw.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gkcdetvkz.sHtML

[U113] JS：正则替换全部
来源：http://baike.epnwcf.com/Article/details/gwexulome.sHtML

s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gvwrbbtfm.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.yfazqb.com/Article/details/gnvkeqeuz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.bbcook.cn/Article/details/gmbfgvfjr.sHtML

[U115] JS：生成 UUID
来源：http://www.share.bbcook.cn/Article/details/gcfktfike.sHtML

crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/gybuhdobg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.sjlbkw.cn/Article/details/gowhorwzq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.vehdjk.com/Article/details/gznseipfd.sHtML

[U117] JS：单元测试
来源：http://wap.tarul.cn/Article/details/gwfdgjbdv.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.bbcook.cn/Article/details/gkuhxmaoc.sHtML

[U118] JS：开发服务器
来源：http://www.blog.sjlbkw.cn/Article/details/gmcgxsqbo.sHtML

npm i -D vite;  npx vite
来源：http://m.share.epnwcf.com/Article/details/gyguwgxxl.sHtML

[U119] JS：生产构建
来源：http://read.share.sjlbkw.cn/Article/details/gyyrhyidg.sHtML

npx vite build
来源：http://baike.yfazqb.com/Article/details/gubkvmuij.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghllmqvkc.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.epnwcf.com/Article/details/gzsfoxrjh.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gldgutfhq.sHtML

统计汇总
来源：http://3g.fktsv.cn/Article/details/gnbfhlmac.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/geyiekzam.sHtML

按语言统计（条）：
来源：http://3g.epnwcf.com/Article/details/gczgwlfwn.sHtML

Python ......... 252
来源：http://3g.bbcook.cn/Article/details/gwgfyeqge.sHtML

PHP ............ 252
来源：http://m.share.yfazqb.com/Article/details/gimyqsckw.sHtML

JavaScript ..... 252
来源：http://mobile.bbcook.cn/Article/details/gnlygqvec.sHtML

TypeScript ..... 212
来源：http://blog.epnwcf.com/Article/details/gwnydinpk.sHtML

Java ........... 212
来源：http://wap.sjlbkw.cn/Article/details/gxwdcyxce.sHtML

Go ............. 212
来源：http://mobile.epnwcf.com/Article/details/gioynokgb.sHtML

Ruby ........... 212
来源：http://blog.bbcook.cn/Article/details/gvanzflwj.sHtML

C# ............. 212
来源：http://mobile.vehdjk.com/Article/details/gwwpqixyg.sHtML

C .............. 30
来源：http://3g.bbcook.cn/Article/details/gktibjbyi.sHtML

C++ ............ 30
来源：http://www.m.share.vehdjk.com/Article/details/gidtxsekz.sHtML

SQL ............ 90
来源：http://read.share.tarul.cn/Article/details/gmmezwuaf.sHtML

Bash ........... 80
来源：http://wap.epnwcf.com/Article/details/grkurzrnq.sHtML

Kotlin ......... 15
来源：http://wap.fktsv.cn/Article/details/gvdydznlr.sHtML

Swift .......... 15
来源：http://read.share.fktsv.cn/Article/details/gunfzndah.sHtML

Lua ............ 10
来源：http://baike.bbcook.cn/Article/details/ghrxqsrnu.sHtML

Perl ........... 10
来源：http://www.blog.tarul.cn/Article/details/ghyytqjqi.sHtML

Scala .......... 10
来源：http://3g.fktsv.cn/Article/details/giifyktet.sHtML

------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/ghelbqadl.sHtML

合计 ........... 2106 条
来源：http://wap.vehdjk.com/Article/details/gpuumlimx.sHtML

按章节统计：
来源：http://www.blog.vehdjk.com/Article/details/gtltobqre.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.yfazqb.com/Article/details/gjglsyhrk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fktsv.cn/Article/details/gcxulwoga.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.sjlbkw.cn/Article/details/gzilqpbpn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.epnwcf.com/Article/details/gtjrrcsmt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.vehdjk.com/Article/details/gxmaqbstj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.yfazqb.com/Article/details/gefjxecnw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.yfazqb.com/Article/details/gezpzrukz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.sjlbkw.cn/Article/details/gnfshzhhn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/guyjclxnd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fktsv.cn/Article/details/gyjimehgf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/guhedhfzf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/gumscfdbb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gozjcbkio.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.bbcook.cn/Article/details/ghbgyrybh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.bbcook.cn/Article/details/gphoqobsr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gaiiircug.sHtML

Q SQL 专题                              90
来源：http://baike.bbcook.cn/Article/details/ghixgzrej.sHtML

R Bash 专题                             80
来源：http://www.share.vehdjk.com/Article/details/gexwgybng.sHtML

S C / C++ 专题                          60
来源：http://blog.yfazqb.com/Article/details/gguzukvpz.sHtML

T 其他语言补充                          60
来源：http://mobile.yfazqb.com/Article/details/gzlhqnsqb.sHtML

U 高频实用片段                         120
来源：http://m.share.fktsv.cn/Article/details/gwykrgngx.sHtML

------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/grjcdhzkw.sHtML

合计                                  2106 条
来源：http://www.share.bbcook.cn/Article/details/gwbasrrxm.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.tarul.cn/Article/details/gtpimsxvg.sHtML

使用提醒
来源：http://www.blog.vehdjk.com/Article/details/gcnrdppeq.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/grhjthaoc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fktsv.cn/Article/details/gqmoeprat.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.sjlbkw.cn/Article/details/glovozbfh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.tarul.cn/Article/details/gksxirnpe.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.sjlbkw.cn/Article/details/ggssyfuqt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.tarul.cn/Article/details/gkfuxyxcb.sHtML

—— 文件结束 ——
来源：http://3g.sjlbkw.cn/Article/details/gkmczqlqt.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gzkanrpnq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.tarul.cn/Article/details/gqwkzzuiq.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fktsv.cn/Article/details/gwmgputmc.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gpkdpjhmp.sHtML

【收录内容】
来源：http://mobile.tarul.cn/Article/details/gxamagjbn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.epnwcf.com/Article/details/girsiigyh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.vehdjk.com/Article/details/gecgkwlan.sHtML

SQL · Bash · C · C++
来源：http://www.share.bbcook.cn/Article/details/ghgeewftj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.epnwcf.com/Article/details/gbaxbsiyq.sHtML

【使用说明】
来源：http://wap.bbcook.cn/Article/details/gxjwwypbj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.sjlbkw.cn/Article/details/gxbihoqdd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fktsv.cn/Article/details/gcqgpwxzi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.sjlbkw.cn/Article/details/gsqllwuwz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.bbcook.cn/Article/details/gxmoydkhp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.sjlbkw.cn/Article/details/ghkybjndg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.yfazqb.com/Article/details/griyevhae.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.epnwcf.com/Article/details/gnsbjajbj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqpbovta.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.epnwcf.com/Article/details/gnnuzvabj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.bbcook.cn/Article/details/gcmuhdxqn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.sjlbkw.cn/Article/details/gezdnwxjo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.sjlbkw.cn/Article/details/gpvmelzmh.sHtML

【文件统计】
来源：http://wap.bbcook.cn/Article/details/gfrrwavxc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.yfazqb.com/Article/details/geeggwtwe.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/gjdnjosmt.sHtML

目  录
来源：http://www.blog.fktsv.cn/Article/details/gwiiiyqjr.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gnhjczetk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.yfazqb.com/Article/details/gzbzyonem.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fktsv.cn/Article/details/gerjftlem.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.vehdjk.com/Article/details/garhydvst.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fktsv.cn/Article/details/gdepisonh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.epnwcf.com/Article/details/gztybirxy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.epnwcf.com/Article/details/gzprodxle.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.yfazqb.com/Article/details/gpaeerrvb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.epnwcf.com/Article/details/gxsuhrxsx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/gsjskwauo.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.epnwcf.com/Article/details/gwdlcqase.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/ggafywfev.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.yfazqb.com/Article/details/gswolfadu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/geffkdozb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.bbcook.cn/Article/details/gnnjdtbwz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.vehdjk.com/Article/details/gllmlzrhq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.sjlbkw.cn/Article/details/giohstgbk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.yfazqb.com/Article/details/gpoiwvonn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.sjlbkw.cn/Article/details/ggnzscmvg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.yfazqb.com/Article/details/gruarwhwo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.epnwcf.com/Article/details/gfhynzedw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fktsv.cn/Article/details/gsgnzlcaw.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gwuwpcuux.sHtML

A. 基础语法与类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gomvlgick.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gtsqqfkck.sHtML

[A01] Hello World
来源：http://baike.bbcook.cn/Article/details/ggwxjqbzn.sHtML

Py:   print("Hello, World!")
来源：http://wap.sjlbkw.cn/Article/details/gcvpftnez.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.bbcook.cn/Article/details/gbpshohuc.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.bbcook.cn/Article/details/gilzlbcyn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fktsv.cn/Article/details/ghskwjslc.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.yfazqb.com/Article/details/gxwcxxeuy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fktsv.cn/Article/details/gtzrodcjm.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.epnwcf.com/Article/details/gatzspfrt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.sjlbkw.cn/Article/details/grbigushf.sHtML

[A02] 变量声明与赋值
来源：http://read.share.sjlbkw.cn/Article/details/gfrncfjqt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.bbcook.cn/Article/details/gdzvnvppo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.sjlbkw.cn/Article/details/ghxjghokd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.epnwcf.com/Article/details/gjvtyjwqh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.yfazqb.com/Article/details/ggfliiccw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.yfazqb.com/Article/details/gioduvriy.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.epnwcf.com/Article/details/ggxtukfib.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.yfazqb.com/Article/details/gvbroupep.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.yfazqb.com/Article/details/gexkhiygw.sHtML

[A03] 常量定义
来源：http://3g.epnwcf.com/Article/details/gsoxuiwum.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.yfazqb.com/Article/details/grrxqgoxh.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gavviadnl.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gfislipfc.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gilvzjhqp.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/ghdykorhu.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fktsv.cn/Article/details/gcflbkszv.sHtML

Ruby: PI = 3.14159
来源：http://mobile.vehdjk.com/Article/details/gzkmlpyyr.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gzvxneufc.sHtML

[A04] 判断变量类型
来源：http://3g.epnwcf.com/Article/details/gsfcatvql.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fktsv.cn/Article/details/gydfemyvi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.yfazqb.com/Article/details/gntgubtap.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.yfazqb.com/Article/details/gwfhxdedw.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.sjlbkw.cn/Article/details/gvgjojjat.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.bbcook.cn/Article/details/gvffccvuv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.vehdjk.com/Article/details/gswghdqzc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.bbcook.cn/Article/details/gwhieqbth.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.sjlbkw.cn/Article/details/gskwmgler.sHtML

[A05] 整数除法与取模
来源：http://3g.bbcook.cn/Article/details/gauelklqy.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.bbcook.cn/Article/details/gyjfkurum.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.vehdjk.com/Article/details/girhkkrrx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.bbcook.cn/Article/details/gtkbvgvun.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.epnwcf.com/Article/details/ghuflqfxv.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.bbcook.cn/Article/details/ghhjmftsg.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.bbcook.cn/Article/details/gemtzmxei.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gjyjhvsvt.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.yfazqb.com/Article/details/gvnubytbd.sHtML

[A06] 字符串转数字
来源：http://www.blog.vehdjk.com/Article/details/gdmbczwll.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.sjlbkw.cn/Article/details/gompckbnz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.tarul.cn/Article/details/gpgncimad.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.bbcook.cn/Article/details/grfwtuxdk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fktsv.cn/Article/details/gazezmpvi.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fktsv.cn/Article/details/gkjehnjhw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.tarul.cn/Article/details/gjkfwmdfx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.sjlbkw.cn/Article/details/gkpodjdmh.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.tarul.cn/Article/details/gttviubdh.sHtML

[A07] 数字转字符串
来源：http://www.share.bbcook.cn/Article/details/gwxxtiscf.sHtML

Py:   str(42)
来源：http://wap.fktsv.cn/Article/details/gyzwaxfal.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.yfazqb.com/Article/details/gmuhqldnr.sHtML

JS:   String(42); (42).toString()
来源：http://baike.bbcook.cn/Article/details/gcasnoyjj.sHtML

TS:   String(42)
来源：http://wap.tarul.cn/Article/details/gfhfsilxj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.epnwcf.com/Article/details/gktvnohir.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.tarul.cn/Article/details/gflyzyvyq.sHtML

Ruby: 42.to_s
来源：http://m.share.bbcook.cn/Article/details/gcnkwjkoy.sHtML

C#:   42.ToString()
来源：http://3g.bbcook.cn/Article/details/gmumwqcrw.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.sjlbkw.cn/Article/details/grxloswcg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.bbcook.cn/Article/details/gilcuekfz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.vehdjk.com/Article/details/gfqxzgvjp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.yfazqb.com/Article/details/gtzdkvdtv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.tarul.cn/Article/details/gybnwcpey.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.sjlbkw.cn/Article/details/gxwvsxrrx.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.bbcook.cn/Article/details/gyedjghcn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.epnwcf.com/Article/details/gnqrgzwvf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.tarul.cn/Article/details/giwebmyaz.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.vehdjk.com/Article/details/gjvbnitai.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gfvqzqbna.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gqltfbgdf.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/givtgipmt.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.yfazqb.com/Article/details/gffcezxig.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.tarul.cn/Article/details/ghxytogfe.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.bbcook.cn/Article/details/gciymrupm.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.vehdjk.com/Article/details/gpsiuhvjc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.vehdjk.com/Article/details/gulzaqzqu.sHtML

[A10] 生成随机数
来源：http://mobile.fktsv.cn/Article/details/gnskvsyff.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.bbcook.cn/Article/details/gcishjwir.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.vehdjk.com/Article/details/gdssyboiy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.epnwcf.com/Article/details/gzkuiwufe.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.sjlbkw.cn/Article/details/gvmdxnbvy.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.epnwcf.com/Article/details/gvnlizirb.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.fktsv.cn/Article/details/gfgjtestj.sHtML

Ruby: rand(1..100)
来源：http://wap.vehdjk.com/Article/details/gnfcqwkze.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.epnwcf.com/Article/details/gfwzmhlzy.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.fktsv.cn/Article/details/gxrpivktq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.vehdjk.com/Article/details/gwyuknago.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.bbcook.cn/Article/details/gbsgzkuoz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/grwhqhewx.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.yfazqb.com/Article/details/gajkxbnle.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gsvtkjzcl.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.yfazqb.com/Article/details/gljpbtjqp.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.yfazqb.com/Article/details/gjtedgjwq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.vehdjk.com/Article/details/gnlwoujmx.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.epnwcf.com/Article/details/gheycfcng.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.bbcook.cn/Article/details/ggrntnsyg.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.tarul.cn/Article/details/gtfsukvuz.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.yfazqb.com/Article/details/gujusldmu.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.epnwcf.com/Article/details/gcrokucdi.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.bbcook.cn/Article/details/gyragoyun.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fktsv.cn/Article/details/gqkgjxdpx.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.bbcook.cn/Article/details/gkcwzghzx.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.epnwcf.com/Article/details/gcjjisjwl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fktsv.cn/Article/details/gnehogmfk.sHtML

Py:   "第一行\n第二行"
来源：http://baike.tarul.cn/Article/details/gacfesevy.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.epnwcf.com/Article/details/gswuvznzm.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/giydfgyqo.sHtML

TS:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/gefnrlkkq.sHtML


<!-- 参考信息 -->