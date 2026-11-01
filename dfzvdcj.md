代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.blog.vehdjk.com/Article/details/gbzlhvjsd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.epnwcf.com/Article/details/gtvssavtc.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.bbcook.cn/Article/details/gquxbzggw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.tarul.cn/Article/details/ggxicdarc.sHtML

[U85] JS：可选链
来源：http://mobile.yfazqb.com/Article/details/gaoavfpau.sHtML

a?.b?.c
来源：http://wap.tarul.cn/Article/details/gvzpyyspt.sHtML

[U86] JS：空值合并
来源：http://blog.sjlbkw.cn/Article/details/gcarbdqmq.sHtML

a ?? b
来源：http://3g.fktsv.cn/Article/details/gkwthdjtz.sHtML

[U87] JS：解构默认值
来源：http://baike.sjlbkw.cn/Article/details/gvlpqyall.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.sjlbkw.cn/Article/details/gemqdmvnd.sHtML

[U88] JS：对象展开合并
来源：http://baike.sjlbkw.cn/Article/details/gocxhprcb.sHtML

{ ...a, ...b }
来源：http://www.m.share.yfazqb.com/Article/details/gywvpzvzo.sHtML

[U89] JS：数组去重
来源：http://www.share.epnwcf.com/Article/details/gtywozahf.sHtML

[...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/gfrdjzwnb.sHtML

[U90] JS：数字数组排序
来源：http://3g.bbcook.cn/Article/details/gsjtwmhkn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.tarul.cn/Article/details/gpckkqosf.sHtML

[U91] JS：对象键值遍历
来源：http://blog.yfazqb.com/Article/details/gfiogvqbq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.tarul.cn/Article/details/gliftjyuu.sHtML

[U92] JS：深拷贝
来源：http://blog.vehdjk.com/Article/details/glvaomdxu.sHtML

structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gskulaibb.sHtML

[U93] JS：模板字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gmjopenfm.sHtML

`共 ${n} 条`
来源：http://www.blog.tarul.cn/Article/details/giwzymnnu.sHtML

[U94] JS：箭头函数
来源：http://read.share.tarul.cn/Article/details/gfumlvofr.sHtML

const double = x => x * 2;
来源：http://www.blog.tarul.cn/Article/details/gzdnlgoet.sHtML

[U95] JS：Promise 包装
来源：http://wap.epnwcf.com/Article/details/gruwptaff.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.tarul.cn/Article/details/gemvvxpbg.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.epnwcf.com/Article/details/gvjhgdndw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/gklfjzbyl.sHtML

[U97] JS：并发请求
来源：http://baike.vehdjk.com/Article/details/greqmgxhp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/ggxqyypmu.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fktsv.cn/Article/details/gidfgssvf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.sjlbkw.cn/Article/details/gaoawqtvl.sHtML

[U99] JS：事件监听
来源：http://mobile.vehdjk.com/Article/details/gkcjhmkon.sHtML

el.addEventListener("click", e => {})
来源：http://wap.sjlbkw.cn/Article/details/gdfkunxby.sHtML

[U100] JS：DOM 查询
来源：http://blog.bbcook.cn/Article/details/gyfoayvsi.sHtML

document.querySelector(".item")
来源：http://m.share.sjlbkw.cn/Article/details/ghvnesvzq.sHtML

[U101] JS：classList 操作
来源：http://www.blog.yfazqb.com/Article/details/gwpypyfsf.sHtML

el.classList.toggle("active")
来源：http://www.share.fktsv.cn/Article/details/gdwrokwke.sHtML

[U102] JS：本地存储
来源：http://www.share.fktsv.cn/Article/details/ghzyephax.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.yfazqb.com/Article/details/gvloglkyg.sHtML

[U103] JS：定时器
来源：http://mobile.vehdjk.com/Article/details/gdybbiwzg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.bbcook.cn/Article/details/grjrcijys.sHtML

[U104] JS：防抖
来源：http://www.m.share.epnwcf.com/Article/details/gnfughpjq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/gbgabqlfl.sHtML

[U105] JS：节流
来源：http://3g.sjlbkw.cn/Article/details/gjaqqccgb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.tarul.cn/Article/details/gcyvbkssz.sHtML

[U106] JS：日期格式化
来源：http://3g.vehdjk.com/Article/details/gliizfogk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.tarul.cn/Article/details/guxfwcudd.sHtML

[U107] JS：数字千分位
来源：http://www.blog.yfazqb.com/Article/details/gehuoiqdp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fktsv.cn/Article/details/gplrzkdvy.sHtML

[U108] JS：随机整数
来源：http://mobile.yfazqb.com/Article/details/gyyodrphi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.vehdjk.com/Article/details/gkozkgqaj.sHtML

[U109] JS：数组分组
来源：http://www.share.fktsv.cn/Article/details/giqzmsoli.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.vehdjk.com/Article/details/giefnllxo.sHtML

[U110] JS：数组分块
来源：http://wap.epnwcf.com/Article/details/gyrjkjdky.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.yfazqb.com/Article/details/ghxvpdybh.sHtML

[U111] JS：对象转 Map
来源：http://m.share.tarul.cn/Article/details/gcvvmuclv.sHtML

new Map(Object.entries(obj))
来源：http://baike.yfazqb.com/Article/details/gckrmbtpf.sHtML

[U112] JS：字符串补位
来源：http://www.blog.sjlbkw.cn/Article/details/gtykndycg.sHtML

"7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gahqjyaos.sHtML

[U113] JS：正则替换全部
来源：http://mobile.bbcook.cn/Article/details/ghtzypfdj.sHtML

s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gsnpolpai.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fktsv.cn/Article/details/gdrgyoqze.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.yfazqb.com/Article/details/gsgureafa.sHtML

[U115] JS：生成 UUID
来源：http://mobile.bbcook.cn/Article/details/gxpxlnykz.sHtML

crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/gfmcfjqof.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.epnwcf.com/Article/details/ggjgefohp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwhskzhy.sHtML

[U117] JS：单元测试
来源：http://3g.yfazqb.com/Article/details/gqylkvarq.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fktsv.cn/Article/details/gszeoudrr.sHtML

[U118] JS：开发服务器
来源：http://wap.vehdjk.com/Article/details/geqyjeida.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.sjlbkw.cn/Article/details/gdingujbt.sHtML

[U119] JS：生产构建
来源：http://m.share.tarul.cn/Article/details/gfgkvgffj.sHtML

npx vite build
来源：http://mobile.tarul.cn/Article/details/gdueikddk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.vehdjk.com/Article/details/ghmrgxhls.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.epnwcf.com/Article/details/gifvnpaxz.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/giarzfswq.sHtML

统计汇总
来源：http://mobile.sjlbkw.cn/Article/details/geotekift.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/grcrsnmjh.sHtML

按语言统计（条）：
来源：http://blog.yfazqb.com/Article/details/geqqnagow.sHtML

Python ......... 252
来源：http://mobile.fktsv.cn/Article/details/ghellleas.sHtML

PHP ............ 252
来源：http://read.share.epnwcf.com/Article/details/gflqbmslx.sHtML

JavaScript ..... 252
来源：http://www.m.share.vehdjk.com/Article/details/ggqnekwtj.sHtML

TypeScript ..... 212
来源：http://blog.vehdjk.com/Article/details/gtnubdxhi.sHtML

Java ........... 212
来源：http://3g.fktsv.cn/Article/details/gwrwtoyia.sHtML

Go ............. 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvdtnist.sHtML

Ruby ........... 212
来源：http://mobile.fktsv.cn/Article/details/gggwkfdrn.sHtML

C# ............. 212
来源：http://read.share.yfazqb.com/Article/details/gkoaepmml.sHtML

C .............. 30
来源：http://m.share.sjlbkw.cn/Article/details/guducqrne.sHtML

C++ ............ 30
来源：http://www.blog.sjlbkw.cn/Article/details/gbooppday.sHtML

SQL ............ 90
来源：http://www.blog.yfazqb.com/Article/details/gxedhtlua.sHtML

Bash ........... 80
来源：http://blog.epnwcf.com/Article/details/gzcootjeg.sHtML

Kotlin ......... 15
来源：http://read.share.fktsv.cn/Article/details/grnfnjrod.sHtML

Swift .......... 15
来源：http://www.share.epnwcf.com/Article/details/gwklzuxlu.sHtML

Lua ............ 10
来源：http://read.share.yfazqb.com/Article/details/gjbsagduq.sHtML

Perl ........... 10
来源：http://mobile.bbcook.cn/Article/details/ghomrocob.sHtML

Scala .......... 10
来源：http://baike.vehdjk.com/Article/details/gpxfqdrri.sHtML

------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gtegaxmqz.sHtML

合计 ........... 2106 条
来源：http://www.share.sjlbkw.cn/Article/details/gdwhglerq.sHtML

按章节统计：
来源：http://read.share.vehdjk.com/Article/details/gingwqinj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.tarul.cn/Article/details/gjwjmzvet.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fktsv.cn/Article/details/gtqeoxabh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.tarul.cn/Article/details/ghfxxedbg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fktsv.cn/Article/details/gfvffnntb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.epnwcf.com/Article/details/gacfftbwv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.bbcook.cn/Article/details/gntfkkayf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fktsv.cn/Article/details/gmqdojngz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.sjlbkw.cn/Article/details/gilueaupc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/gxzddqllp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.vehdjk.com/Article/details/gbaxhahyp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gyizcsjxe.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gliuiozkp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/ghhdfqpdw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.tarul.cn/Article/details/gjnjiuzja.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.tarul.cn/Article/details/gopzzestm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gaxvwtmpk.sHtML

Q SQL 专题                              90
来源：http://m.share.bbcook.cn/Article/details/gdixppkzd.sHtML

R Bash 专题                             80
来源：http://www.blog.vehdjk.com/Article/details/gerfjzlnm.sHtML

S C / C++ 专题                          60
来源：http://blog.fktsv.cn/Article/details/ghidpfzqi.sHtML

T 其他语言补充                          60
来源：http://baike.vehdjk.com/Article/details/gxrucddcn.sHtML

U 高频实用片段                         120
来源：http://wap.fktsv.cn/Article/details/guwlyranq.sHtML

------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gbqvszqlp.sHtML

合计                                  2106 条
来源：http://www.m.share.bbcook.cn/Article/details/ghrbuxcan.sHtML

--------------------------------------------------------------------------------
来源：http://baike.tarul.cn/Article/details/gkkqdinpn.sHtML

使用提醒
来源：http://mobile.sjlbkw.cn/Article/details/gzdbhqowl.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gttmowbky.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.tarul.cn/Article/details/gxvhrrrdd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.yfazqb.com/Article/details/gsfyibfag.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fktsv.cn/Article/details/gtdpewkti.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.bbcook.cn/Article/details/gpwhowydw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.sjlbkw.cn/Article/details/gljcbwmcm.sHtML

—— 文件结束 ——
来源：http://www.m.share.tarul.cn/Article/details/gvtczdsww.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gzoczohcw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.epnwcf.com/Article/details/gzhyixfwx.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.yfazqb.com/Article/details/gbkfaacga.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gepelqmuz.sHtML

【收录内容】
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvhspsbl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.sjlbkw.cn/Article/details/grdtdncbz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.bbcook.cn/Article/details/gnllznqza.sHtML

SQL · Bash · C · C++
来源：http://m.share.yfazqb.com/Article/details/gutoxkzrz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.yfazqb.com/Article/details/gqlxvjirj.sHtML

【使用说明】
来源：http://3g.epnwcf.com/Article/details/gfwykyzev.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.sjlbkw.cn/Article/details/gtwdibjpc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.bbcook.cn/Article/details/ggkazgxpr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.yfazqb.com/Article/details/gndmpvigd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.sjlbkw.cn/Article/details/goyznfltr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.epnwcf.com/Article/details/gwsgmoazv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.epnwcf.com/Article/details/gjuvjuhjr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.bbcook.cn/Article/details/gzjfissgp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.yfazqb.com/Article/details/gsftoqssf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.sjlbkw.cn/Article/details/gtaeqhlnn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.yfazqb.com/Article/details/glsvzassz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.vehdjk.com/Article/details/gvihkntps.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.yfazqb.com/Article/details/gzxsnvrtt.sHtML

【文件统计】
来源：http://baike.vehdjk.com/Article/details/gxzomuemf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.yfazqb.com/Article/details/gpwydemhe.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fktsv.cn/Article/details/gtxvusnhc.sHtML

目  录
来源：http://baike.bbcook.cn/Article/details/gudrugnql.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/goavnjser.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.vehdjk.com/Article/details/gyhoulvnw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.tarul.cn/Article/details/gvdtzarqq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.yfazqb.com/Article/details/ghjakneig.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.bbcook.cn/Article/details/ghjwvcora.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.yfazqb.com/Article/details/gniipxwwy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.sjlbkw.cn/Article/details/gdgzjnrgh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.vehdjk.com/Article/details/govpjuccs.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.yfazqb.com/Article/details/gtenwklio.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/ghqhhyexv.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.epnwcf.com/Article/details/gakyddmqu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.tarul.cn/Article/details/gcabcqinx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.epnwcf.com/Article/details/gltagviqw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/gcpjjsvxq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fktsv.cn/Article/details/gyeozaadr.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.sjlbkw.cn/Article/details/gxsodflwr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.bbcook.cn/Article/details/gzzizgmzw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.vehdjk.com/Article/details/gpdzxydkw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fktsv.cn/Article/details/gzjclmfbc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.sjlbkw.cn/Article/details/grknudgfv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.sjlbkw.cn/Article/details/gargbjrav.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.tarul.cn/Article/details/gcseagnwm.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gxvllykfj.sHtML

A. 基础语法与类型
来源：http://read.share.tarul.cn/Article/details/gjbbqyvbx.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gmwmmxrnu.sHtML

[A01] Hello World
来源：http://www.share.tarul.cn/Article/details/ggjjkshzo.sHtML

Py:   print("Hello, World!")
来源：http://read.share.sjlbkw.cn/Article/details/gyyyxmday.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.bbcook.cn/Article/details/gajygcfeu.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.sjlbkw.cn/Article/details/glmstmjkw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.yfazqb.com/Article/details/gmhyidsqv.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.vehdjk.com/Article/details/gyhlahtre.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.epnwcf.com/Article/details/ghfvcngxf.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.tarul.cn/Article/details/guljsnxto.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.tarul.cn/Article/details/gvzjrqofq.sHtML

[A02] 变量声明与赋值
来源：http://wap.fktsv.cn/Article/details/gdcrjadci.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.yfazqb.com/Article/details/gutwvavzt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.vehdjk.com/Article/details/gihusyogu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fktsv.cn/Article/details/gaknsfnaa.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.tarul.cn/Article/details/gtkgookrl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fktsv.cn/Article/details/gvtqinlce.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.tarul.cn/Article/details/gllrcrbkl.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.tarul.cn/Article/details/gvqtjxrql.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.sjlbkw.cn/Article/details/gbreqtcqa.sHtML

[A03] 常量定义
来源：http://www.blog.epnwcf.com/Article/details/gifoijgpk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.yfazqb.com/Article/details/gsjegfxns.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gilllixpm.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/ggshiwnsf.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gurocpsqu.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gjplsbowr.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.tarul.cn/Article/details/glwzyzazn.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fktsv.cn/Article/details/gnbazjxre.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gapadwbiz.sHtML

[A04] 判断变量类型
来源：http://www.share.sjlbkw.cn/Article/details/goinwherp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.tarul.cn/Article/details/gbhkhlemc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.epnwcf.com/Article/details/gkdwsheeg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fktsv.cn/Article/details/gxrvgmxcd.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.epnwcf.com/Article/details/gdvqsjsje.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.sjlbkw.cn/Article/details/gdzqtlxnw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.yfazqb.com/Article/details/gsnaexvni.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.vehdjk.com/Article/details/gvyjtxqef.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.vehdjk.com/Article/details/gtjnwpvzy.sHtML

[A05] 整数除法与取模
来源：http://m.share.yfazqb.com/Article/details/ghmcavjpz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.bbcook.cn/Article/details/glzcqkwub.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/ggrmnuqwe.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/goprnfvcq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwlzdmcy.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdlbuafp.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.vehdjk.com/Article/details/gyurtzeyg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fktsv.cn/Article/details/gvyqdgkhg.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.yfazqb.com/Article/details/gsdydvpun.sHtML

[A06] 字符串转数字
来源：http://www.m.share.yfazqb.com/Article/details/gntrowzow.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.tarul.cn/Article/details/gdzswgpxt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.vehdjk.com/Article/details/gzsuipvkl.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.tarul.cn/Article/details/gqxexbzib.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.epnwcf.com/Article/details/gonunsdlu.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.vehdjk.com/Article/details/glgioizpl.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fktsv.cn/Article/details/gpmdqdfsc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.epnwcf.com/Article/details/ggzdtwidx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fktsv.cn/Article/details/gjvjhenov.sHtML

[A07] 数字转字符串
来源：http://www.share.yfazqb.com/Article/details/gkppndoqf.sHtML

Py:   str(42)
来源：http://wap.sjlbkw.cn/Article/details/gtoewkscs.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.epnwcf.com/Article/details/gdmnkdwzf.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fktsv.cn/Article/details/gxsdijiap.sHtML

TS:   String(42)
来源：http://www.share.fktsv.cn/Article/details/gipcvbegj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.bbcook.cn/Article/details/gzbpamvuw.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.epnwcf.com/Article/details/gqxdjmyti.sHtML

Ruby: 42.to_s
来源：http://www.share.bbcook.cn/Article/details/ggqsbxujm.sHtML

C#:   42.ToString()
来源：http://wap.tarul.cn/Article/details/goasvmqcx.sHtML

[A08] 取整与四舍五入
来源：http://m.share.yfazqb.com/Article/details/gnckhnigu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.yfazqb.com/Article/details/gzataaslm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.tarul.cn/Article/details/gikwjoqjc.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.vehdjk.com/Article/details/grgfqwpce.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.bbcook.cn/Article/details/ghppsvknw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fktsv.cn/Article/details/gsmythxaw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.vehdjk.com/Article/details/gdnamdhvq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.epnwcf.com/Article/details/gprptpbzz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.fktsv.cn/Article/details/glklrftdr.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.yfazqb.com/Article/details/gxnynrfmm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.epnwcf.com/Article/details/ganadaujw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gxdpyixht.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/gkimuenid.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gzwmgclpc.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.tarul.cn/Article/details/gncsmbjxc.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.fktsv.cn/Article/details/gocqigwwv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.fktsv.cn/Article/details/gnbskgcvx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gzhzgsmso.sHtML

[A10] 生成随机数
来源：http://3g.tarul.cn/Article/details/ghnqmyioj.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.tarul.cn/Article/details/gxdorssgc.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fktsv.cn/Article/details/gxmosgmox.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.yfazqb.com/Article/details/ghvoplizt.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.sjlbkw.cn/Article/details/guafpqlyv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.sjlbkw.cn/Article/details/gpskcsavv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.tarul.cn/Article/details/gxevzyzrc.sHtML

Ruby: rand(1..100)
来源：http://blog.bbcook.cn/Article/details/gijdhanwq.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.yfazqb.com/Article/details/gxeeqdepw.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.vehdjk.com/Article/details/gdsateduz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fktsv.cn/Article/details/gevtoasgg.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.sjlbkw.cn/Article/details/gvkuouhsc.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/gpjnvriuj.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.yfazqb.com/Article/details/gmhlhmjsf.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.vehdjk.com/Article/details/gpeppdvud.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.bbcook.cn/Article/details/gpjrwalxv.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.epnwcf.com/Article/details/gixdvdwrr.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/gpeqytpft.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fktsv.cn/Article/details/gffrjepzm.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.tarul.cn/Article/details/gtuyrhplg.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.epnwcf.com/Article/details/gfsjczqpw.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.tarul.cn/Article/details/gweojakup.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.vehdjk.com/Article/details/ghwetpvly.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.bbcook.cn/Article/details/gflzidtar.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.yfazqb.com/Article/details/gmrevnqvh.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.sjlbkw.cn/Article/details/gziymkshg.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.yfazqb.com/Article/details/gjtxtwydr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fktsv.cn/Article/details/gdmldltie.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/gqtsucyog.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/ggxyouduz.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.tarul.cn/Article/details/gmgfnzwal.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/gkwzqsbnn.sHtML

Java: "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/gozzzxfzq.sHtML

Go:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gznxthlhf.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/gwsfvnqhl.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gaiupxznd.sHtML


<!-- 参考信息 -->