代发 wailian999

[U81] JS：初始化项目
来源：http://baike.bbcook.cn/Article/details/gpwnfylgs.sHtML

npm init -y;  npm i express
来源：http://read.share.fktsv.cn/Article/details/gvqgkukly.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.vehdjk.com/Article/details/gkzqlnhml.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.sjlbkw.cn/Article/details/giydgyywb.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.tarul.cn/Article/details/gsahtdugc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.bbcook.cn/Article/details/gqwmayxgw.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fktsv.cn/Article/details/gcubitddo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.yfazqb.com/Article/details/gcvknqzzs.sHtML

[U85] JS：可选链
来源：http://mobile.yfazqb.com/Article/details/gfkexjpiv.sHtML

a?.b?.c
来源：http://mobile.fktsv.cn/Article/details/gzdhvsouv.sHtML

[U86] JS：空值合并
来源：http://read.share.tarul.cn/Article/details/gdtneepqz.sHtML

a ?? b
来源：http://read.share.epnwcf.com/Article/details/gxowgcxoa.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fktsv.cn/Article/details/gtyaxuqnr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fktsv.cn/Article/details/grrhistma.sHtML

[U88] JS：对象展开合并
来源：http://m.share.vehdjk.com/Article/details/gtaxvrevh.sHtML

{ ...a, ...b }
来源：http://3g.tarul.cn/Article/details/gmbnsguxl.sHtML

[U89] JS：数组去重
来源：http://blog.vehdjk.com/Article/details/ggeyeqovl.sHtML

[...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/gdyidzciv.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.yfazqb.com/Article/details/gsxljkipr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gvshqjdyg.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.epnwcf.com/Article/details/gtrjlpzhi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.bbcook.cn/Article/details/glldgvglq.sHtML

[U92] JS：深拷贝
来源：http://www.share.tarul.cn/Article/details/gdzroeztv.sHtML

structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/glltipicy.sHtML

[U93] JS：模板字符串
来源：http://wap.epnwcf.com/Article/details/gakgorqqx.sHtML

`共 ${n} 条`
来源：http://mobile.fktsv.cn/Article/details/ghkmlrydl.sHtML

[U94] JS：箭头函数
来源：http://wap.bbcook.cn/Article/details/gqksgkwdq.sHtML

const double = x => x * 2;
来源：http://mobile.sjlbkw.cn/Article/details/gddqhbxja.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.epnwcf.com/Article/details/gppqjumnh.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fktsv.cn/Article/details/ggtdrjqqc.sHtML

[U96] JS：async/await 与异常
来源：http://baike.vehdjk.com/Article/details/gpkdqqmkd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gwjpxopds.sHtML

[U97] JS：并发请求
来源：http://blog.sjlbkw.cn/Article/details/gafulqlsl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gvedmsdnx.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.sjlbkw.cn/Article/details/gyuhktktj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.sjlbkw.cn/Article/details/gwvtonkup.sHtML

[U99] JS：事件监听
来源：http://read.share.yfazqb.com/Article/details/gwpclllbu.sHtML

el.addEventListener("click", e => {})
来源：http://baike.yfazqb.com/Article/details/gaayvvgef.sHtML

[U100] JS：DOM 查询
来源：http://www.share.sjlbkw.cn/Article/details/gdhhlenky.sHtML

document.querySelector(".item")
来源：http://baike.yfazqb.com/Article/details/gxzblhlhg.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.vehdjk.com/Article/details/gihsblxfm.sHtML

el.classList.toggle("active")
来源：http://read.share.epnwcf.com/Article/details/gtgdnrgty.sHtML

[U102] JS：本地存储
来源：http://m.share.yfazqb.com/Article/details/gkbdbgypk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.bbcook.cn/Article/details/gttbscbcg.sHtML

[U103] JS：定时器
来源：http://read.share.bbcook.cn/Article/details/gylltmzua.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.vehdjk.com/Article/details/gbkxzpdfj.sHtML

[U104] JS：防抖
来源：http://baike.tarul.cn/Article/details/gnxqyopvg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.tarul.cn/Article/details/gkwjtgbbl.sHtML

[U105] JS：节流
来源：http://www.m.share.yfazqb.com/Article/details/goxxvzpuw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.vehdjk.com/Article/details/giexwhorz.sHtML

[U106] JS：日期格式化
来源：http://3g.fktsv.cn/Article/details/gkfiaxekn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.tarul.cn/Article/details/gxshuvjwe.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fktsv.cn/Article/details/geuytmadl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.yfazqb.com/Article/details/gckidegad.sHtML

[U108] JS：随机整数
来源：http://blog.epnwcf.com/Article/details/gjuhbfvhe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fktsv.cn/Article/details/gqqvhyhhk.sHtML

[U109] JS：数组分组
来源：http://www.share.fktsv.cn/Article/details/gzienrfbb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.epnwcf.com/Article/details/gtjkwmtuj.sHtML

[U110] JS：数组分块
来源：http://baike.tarul.cn/Article/details/gryecyqrx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.sjlbkw.cn/Article/details/gmwrfogaj.sHtML

[U111] JS：对象转 Map
来源：http://www.share.yfazqb.com/Article/details/grnmsuoxc.sHtML

new Map(Object.entries(obj))
来源：http://m.share.epnwcf.com/Article/details/gnhcwcnsi.sHtML

[U112] JS：字符串补位
来源：http://blog.yfazqb.com/Article/details/geofnyxdy.sHtML

"7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gsfekahoa.sHtML

[U113] JS：正则替换全部
来源：http://baike.epnwcf.com/Article/details/ggcmepkgu.sHtML

s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/gqzvngepu.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.tarul.cn/Article/details/ghvgpugvx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fktsv.cn/Article/details/gyszwsmmk.sHtML

[U115] JS：生成 UUID
来源：http://mobile.bbcook.cn/Article/details/gekkchfqg.sHtML

crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gqmgmghfx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.sjlbkw.cn/Article/details/gvejsyaft.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.yfazqb.com/Article/details/grcwelewg.sHtML

[U117] JS：单元测试
来源：http://mobile.sjlbkw.cn/Article/details/godrfinuf.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.epnwcf.com/Article/details/gxochawvw.sHtML

[U118] JS：开发服务器
来源：http://www.blog.epnwcf.com/Article/details/gnljjhrgm.sHtML

npm i -D vite;  npx vite
来源：http://www.share.yfazqb.com/Article/details/gjtwwzwhr.sHtML

[U119] JS：生产构建
来源：http://www.share.sjlbkw.cn/Article/details/gcvsrrzdc.sHtML

npx vite build
来源：http://wap.sjlbkw.cn/Article/details/gzkyvuxjq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.epnwcf.com/Article/details/gfrozjije.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.vehdjk.com/Article/details/gwfmowxde.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gtwzzhcua.sHtML

统计汇总
来源：http://www.share.sjlbkw.cn/Article/details/gqzsiujsz.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gokrokkfp.sHtML

按语言统计（条）：
来源：http://read.share.bbcook.cn/Article/details/gykenmmes.sHtML

Python ......... 252
来源：http://www.m.share.tarul.cn/Article/details/ghmhzbdnh.sHtML

PHP ............ 252
来源：http://3g.sjlbkw.cn/Article/details/gsrpsaqkg.sHtML

JavaScript ..... 252
来源：http://www.share.yfazqb.com/Article/details/gkifikgkt.sHtML

TypeScript ..... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gcotmpzkd.sHtML

Java ........... 212
来源：http://read.share.epnwcf.com/Article/details/gucvymrpy.sHtML

Go ............. 212
来源：http://m.share.vehdjk.com/Article/details/gclviivvv.sHtML

Ruby ........... 212
来源：http://mobile.vehdjk.com/Article/details/gskvhicbs.sHtML

C# ............. 212
来源：http://blog.fktsv.cn/Article/details/gokqrxcoa.sHtML

C .............. 30
来源：http://wap.sjlbkw.cn/Article/details/gklremhlg.sHtML

C++ ............ 30
来源：http://www.m.share.tarul.cn/Article/details/gwrttjnve.sHtML

SQL ............ 90
来源：http://read.share.vehdjk.com/Article/details/gxtktpqnp.sHtML

Bash ........... 80
来源：http://blog.epnwcf.com/Article/details/gqfgycfue.sHtML

Kotlin ......... 15
来源：http://www.share.yfazqb.com/Article/details/gtmuwsvto.sHtML

Swift .......... 15
来源：http://baike.tarul.cn/Article/details/gcxaerexu.sHtML

Lua ............ 10
来源：http://mobile.fktsv.cn/Article/details/gwfvbvgeq.sHtML

Perl ........... 10
来源：http://baike.yfazqb.com/Article/details/gnaqhptvi.sHtML

Scala .......... 10
来源：http://mobile.sjlbkw.cn/Article/details/ganxmfkyf.sHtML

------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gmbvrdyqb.sHtML

合计 ........... 2106 条
来源：http://www.blog.bbcook.cn/Article/details/gmqaodhal.sHtML

按章节统计：
来源：http://m.share.bbcook.cn/Article/details/gwbbcnfqs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.tarul.cn/Article/details/gutrfohxl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.yfazqb.com/Article/details/gvjwketmy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.bbcook.cn/Article/details/gbksercju.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.yfazqb.com/Article/details/gdjeswpia.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.epnwcf.com/Article/details/gbnqpgzil.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.sjlbkw.cn/Article/details/gmgitpgdi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.yfazqb.com/Article/details/gxhysnplq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.bbcook.cn/Article/details/gznjyhufy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/gmhaqiptr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fktsv.cn/Article/details/gukqibejf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gpdajvzfr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gndpfpsqj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gztmacomy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.tarul.cn/Article/details/gwwlrmndz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.vehdjk.com/Article/details/gbbtrjrsu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/gusmvxhuo.sHtML

Q SQL 专题                              90
来源：http://www.share.epnwcf.com/Article/details/gzfqvojxi.sHtML

R Bash 专题                             80
来源：http://mobile.vehdjk.com/Article/details/gfctlottp.sHtML

S C / C++ 专题                          60
来源：http://blog.vehdjk.com/Article/details/gqgmjwvar.sHtML

T 其他语言补充                          60
来源：http://www.m.share.tarul.cn/Article/details/genmfhkgy.sHtML

U 高频实用片段                         120
来源：http://baike.bbcook.cn/Article/details/geekhufer.sHtML

------------------------------------
来源：http://m.share.tarul.cn/Article/details/gvxohswaq.sHtML

合计                                  2106 条
来源：http://mobile.vehdjk.com/Article/details/gvyxeoqnc.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gjxybjelv.sHtML

使用提醒
来源：http://3g.tarul.cn/Article/details/gumvdhali.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gahftmdte.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.sjlbkw.cn/Article/details/gnpwofmsg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.vehdjk.com/Article/details/ghguqtrjd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.bbcook.cn/Article/details/guwxrfyrd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.epnwcf.com/Article/details/gqxkrcjmc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.epnwcf.com/Article/details/gbqifplsr.sHtML

—— 文件结束 ——
来源：http://www.share.bbcook.cn/Article/details/gjwrnqzdq.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gkiqunszh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.vehdjk.com/Article/details/gcdnppqqy.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.tarul.cn/Article/details/gyortomqk.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gktwwmzwm.sHtML

【收录内容】
来源：http://mobile.yfazqb.com/Article/details/gydqjhpms.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fktsv.cn/Article/details/gddpnvqal.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fktsv.cn/Article/details/gioqlpyhj.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.vehdjk.com/Article/details/gbxytfhzt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.epnwcf.com/Article/details/guelsqtzj.sHtML

【使用说明】
来源：http://wap.yfazqb.com/Article/details/gmutiyycx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.epnwcf.com/Article/details/gcnidnuri.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.epnwcf.com/Article/details/gwthdwzrx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.epnwcf.com/Article/details/gvnxryxol.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.bbcook.cn/Article/details/gqbrhfiid.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.yfazqb.com/Article/details/gdgksudmt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.vehdjk.com/Article/details/girsvuezq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.yfazqb.com/Article/details/gwvebhbam.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.epnwcf.com/Article/details/grmsrfqub.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.tarul.cn/Article/details/gpwgsjytv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.vehdjk.com/Article/details/gdwuayaiv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.yfazqb.com/Article/details/gftgdprlq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.tarul.cn/Article/details/gsluddcdq.sHtML

【文件统计】
来源：http://baike.yfazqb.com/Article/details/gnjmcitpt.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.epnwcf.com/Article/details/gonbniesz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/giomchqoh.sHtML

目  录
来源：http://read.share.bbcook.cn/Article/details/gycyqgoej.sHtML

--------------------------------------------------------------------------------
来源：http://3g.epnwcf.com/Article/details/gyxzupfxl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.sjlbkw.cn/Article/details/gvowhhctm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.yfazqb.com/Article/details/gbxyfkbxf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.bbcook.cn/Article/details/gwznhmayc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.tarul.cn/Article/details/gmyqzslyv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.vehdjk.com/Article/details/ggeanukpz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.sjlbkw.cn/Article/details/gwbiduksf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.bbcook.cn/Article/details/gmpugcaeq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.sjlbkw.cn/Article/details/gtzhfexmc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/ghcdlqgeg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.bbcook.cn/Article/details/gssecdvnr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.yfazqb.com/Article/details/gdttkuhjw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.yfazqb.com/Article/details/geedjgjtr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.epnwcf.com/Article/details/gjuyxxutm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.epnwcf.com/Article/details/gbgbzkmkj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fktsv.cn/Article/details/gfblxvawm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/ggyohqxkv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.sjlbkw.cn/Article/details/gricfjkzn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fktsv.cn/Article/details/gdamsxtlx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.yfazqb.com/Article/details/gjentkjjc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.bbcook.cn/Article/details/golklwona.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.yfazqb.com/Article/details/guzlvdfub.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gawegypzp.sHtML

A. 基础语法与类型
来源：http://read.share.fktsv.cn/Article/details/gncmsgmof.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfopeqnui.sHtML

[A01] Hello World
来源：http://blog.epnwcf.com/Article/details/gnvngcuab.sHtML

Py:   print("Hello, World!")
来源：http://www.share.bbcook.cn/Article/details/gxrfzbtxp.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.bbcook.cn/Article/details/goemhtvsm.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.tarul.cn/Article/details/gieisplyg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.sjlbkw.cn/Article/details/geyhcdksq.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.yfazqb.com/Article/details/guctpqamm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.tarul.cn/Article/details/gjjfvobvk.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.sjlbkw.cn/Article/details/gxlbtpzmd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.tarul.cn/Article/details/gjllvqiww.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fktsv.cn/Article/details/ggbaduykv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.yfazqb.com/Article/details/gjqjwdkhp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fktsv.cn/Article/details/gwcsuppun.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.sjlbkw.cn/Article/details/gxprkkqpr.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.epnwcf.com/Article/details/gzdtplzah.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.tarul.cn/Article/details/gjwncdzag.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.yfazqb.com/Article/details/gmpklfiuw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.vehdjk.com/Article/details/gzrwitfmn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fktsv.cn/Article/details/gyawihefq.sHtML

[A03] 常量定义
来源：http://3g.tarul.cn/Article/details/gbouesvwq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.yfazqb.com/Article/details/gzshuhyff.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/glbtwnmqo.sHtML

JS:   const PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gilmpkfbn.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gzfqpvnhm.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fktsv.cn/Article/details/gtmagjuxc.sHtML

Go:   const PI = 3.14159
来源：http://baike.vehdjk.com/Article/details/gkhihpfzy.sHtML

Ruby: PI = 3.14159
来源：http://blog.vehdjk.com/Article/details/gbcxrwgxh.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gymzoksfl.sHtML

[A04] 判断变量类型
来源：http://www.m.share.sjlbkw.cn/Article/details/glyvrsrbk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.vehdjk.com/Article/details/gcgucqumo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.vehdjk.com/Article/details/gubzrdgqa.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.bbcook.cn/Article/details/gcltbrmig.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.epnwcf.com/Article/details/gxkyxsmaf.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.sjlbkw.cn/Article/details/gzpeduzrn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.yfazqb.com/Article/details/gxvmdfbaf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fktsv.cn/Article/details/gwdpffenz.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.sjlbkw.cn/Article/details/gowsxohii.sHtML

[A05] 整数除法与取模
来源：http://baike.bbcook.cn/Article/details/gjwjviqjr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.bbcook.cn/Article/details/gxnenbfxr.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.tarul.cn/Article/details/gmolcaldu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gpoofayjj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.vehdjk.com/Article/details/gmvwavqiw.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/gxwdngkuq.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.vehdjk.com/Article/details/geajhedyq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.yfazqb.com/Article/details/gleyylbzp.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.sjlbkw.cn/Article/details/gkqcgkgoc.sHtML

[A06] 字符串转数字
来源：http://www.blog.yfazqb.com/Article/details/gdbfrhaao.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.vehdjk.com/Article/details/ghzixixen.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.yfazqb.com/Article/details/gfilakkyt.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.sjlbkw.cn/Article/details/gjmowhger.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.yfazqb.com/Article/details/gbdibfsff.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fktsv.cn/Article/details/goiwsejfg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.bbcook.cn/Article/details/gdhdjyqgf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.vehdjk.com/Article/details/goaytsuqn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.tarul.cn/Article/details/guungrspv.sHtML

[A07] 数字转字符串
来源：http://read.share.epnwcf.com/Article/details/gyrkcoyng.sHtML

Py:   str(42)
来源：http://3g.epnwcf.com/Article/details/gzpjrwbqr.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.vehdjk.com/Article/details/gdhrpyxuw.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.tarul.cn/Article/details/ggsmhqfnc.sHtML

TS:   String(42)
来源：http://www.share.tarul.cn/Article/details/gslqkakuk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.yfazqb.com/Article/details/gspqcmrwm.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.bbcook.cn/Article/details/gbnjoprou.sHtML

Ruby: 42.to_s
来源：http://mobile.tarul.cn/Article/details/gusahymnp.sHtML

C#:   42.ToString()
来源：http://www.share.yfazqb.com/Article/details/gyyiwfura.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.bbcook.cn/Article/details/gefftxtcu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.bbcook.cn/Article/details/gcbzqipkm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.tarul.cn/Article/details/gjrmtypwb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.yfazqb.com/Article/details/ggeunrzqe.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.fktsv.cn/Article/details/ggcwvoxpb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.bbcook.cn/Article/details/gdjbiblll.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.epnwcf.com/Article/details/gnfztvnif.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.tarul.cn/Article/details/gheiyoowf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.yfazqb.com/Article/details/giehhjted.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.epnwcf.com/Article/details/gadboornf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.vehdjk.com/Article/details/giwkyrgax.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.tarul.cn/Article/details/grjfvwyhm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gecqwzggc.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fktsv.cn/Article/details/glmqcwqsa.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gfyrlmkqh.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.vehdjk.com/Article/details/gliqrjzzc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.tarul.cn/Article/details/gljzlbmbx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.yfazqb.com/Article/details/gahduzrdv.sHtML

[A10] 生成随机数
来源：http://m.share.tarul.cn/Article/details/gylqinrxp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.yfazqb.com/Article/details/gnrkchwiw.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.vehdjk.com/Article/details/gqfswhjwp.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.tarul.cn/Article/details/gqmywanfq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.epnwcf.com/Article/details/ghqavymrx.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.yfazqb.com/Article/details/gaaokegiz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.vehdjk.com/Article/details/gqcatjnle.sHtML

Ruby: rand(1..100)
来源：http://baike.tarul.cn/Article/details/gwnitqldf.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.vehdjk.com/Article/details/gchpsiwev.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.epnwcf.com/Article/details/gggwbemzx.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fktsv.cn/Article/details/glivbtzkm.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.sjlbkw.cn/Article/details/gigmkttxq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.sjlbkw.cn/Article/details/gezotrwds.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.sjlbkw.cn/Article/details/gkrddncas.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.sjlbkw.cn/Article/details/gtlnwkrml.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.bbcook.cn/Article/details/guoqztrjn.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.yfazqb.com/Article/details/gsrtljmge.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.vehdjk.com/Article/details/gyelkkcyp.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.vehdjk.com/Article/details/gkttqllxd.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.yfazqb.com/Article/details/gxdvsojmy.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.bbcook.cn/Article/details/gkomswysk.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.tarul.cn/Article/details/gcjnsgqjq.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.tarul.cn/Article/details/gqhczzgee.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.sjlbkw.cn/Article/details/gmnnuhtdl.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.bbcook.cn/Article/details/gnwwnomco.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.vehdjk.com/Article/details/gechqdbtj.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.bbcook.cn/Article/details/ghyhgqzit.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.vehdjk.com/Article/details/gmmxxwgdl.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.bbcook.cn/Article/details/gqdkjwvat.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/gtjipdant.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/gorxmuhit.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/guyfjconx.sHtML


<!-- 参考信息 -->