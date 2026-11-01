代发 wailian999

[U79] PHP：静态分析
来源：http://m.share.epnwcf.com/Article/details/gtaaircka.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.bbcook.cn/Article/details/gfducyvec.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.tarul.cn/Article/details/gnqkmedsh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.tarul.cn/Article/details/gnjyuvfng.sHtML

[U81] JS：初始化项目
来源：http://www.share.vehdjk.com/Article/details/gdslovnmk.sHtML

npm init -y;  npm i express
来源：http://baike.fktsv.cn/Article/details/gpahprtfi.sHtML

[U82] JS：package.json 脚本
来源：http://blog.epnwcf.com/Article/details/ghqkapxfa.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.tarul.cn/Article/details/grcyjkjhf.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.vehdjk.com/Article/details/gmsjjpajm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.vehdjk.com/Article/details/gpvjaecrq.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.tarul.cn/Article/details/gawjlrhoz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.sjlbkw.cn/Article/details/ghtxlxjqm.sHtML

[U85] JS：可选链
来源：http://blog.yfazqb.com/Article/details/ggebytaze.sHtML

a?.b?.c
来源：http://wap.fktsv.cn/Article/details/geartjhic.sHtML

[U86] JS：空值合并
来源：http://3g.epnwcf.com/Article/details/gqmgzydwi.sHtML

a ?? b
来源：http://www.blog.vehdjk.com/Article/details/gsjwxhyyy.sHtML

[U87] JS：解构默认值
来源：http://read.share.fktsv.cn/Article/details/gdakgosiq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.tarul.cn/Article/details/ghxqtcitk.sHtML

[U88] JS：对象展开合并
来源：http://www.share.bbcook.cn/Article/details/gbkeqziho.sHtML

{ ...a, ...b }
来源：http://www.blog.bbcook.cn/Article/details/gezonodzs.sHtML

[U89] JS：数组去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gpddbeusu.sHtML

[...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/ggzhnxqus.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.epnwcf.com/Article/details/gkyhgbdqw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gwchhmoai.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gltsipjxc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.vehdjk.com/Article/details/gxgbuuzac.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fktsv.cn/Article/details/gjvvhzcxd.sHtML

structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/gxahyyikx.sHtML

[U93] JS：模板字符串
来源：http://www.share.vehdjk.com/Article/details/gmevqasxh.sHtML

`共 ${n} 条`
来源：http://read.share.sjlbkw.cn/Article/details/gkcasitlx.sHtML

[U94] JS：箭头函数
来源：http://m.share.tarul.cn/Article/details/gvsofokrq.sHtML

const double = x => x * 2;
来源：http://mobile.vehdjk.com/Article/details/ghxgmcinf.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.yfazqb.com/Article/details/gsldsfgkj.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.sjlbkw.cn/Article/details/gpqfefrqb.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fktsv.cn/Article/details/gcimykcjo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/gaomadvum.sHtML

[U97] JS：并发请求
来源：http://www.m.share.bbcook.cn/Article/details/gphlzqpzh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/giplraymb.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.yfazqb.com/Article/details/gsyjccgmz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fktsv.cn/Article/details/glqefxziv.sHtML

[U99] JS：事件监听
来源：http://3g.bbcook.cn/Article/details/grepfjzmg.sHtML

el.addEventListener("click", e => {})
来源：http://wap.bbcook.cn/Article/details/galmebbko.sHtML

[U100] JS：DOM 查询
来源：http://wap.yfazqb.com/Article/details/gvnahinqk.sHtML

document.querySelector(".item")
来源：http://read.share.vehdjk.com/Article/details/gossdjbzz.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fktsv.cn/Article/details/gnwblptqk.sHtML

el.classList.toggle("active")
来源：http://3g.sjlbkw.cn/Article/details/gjeexxqqo.sHtML

[U102] JS：本地存储
来源：http://read.share.sjlbkw.cn/Article/details/gjlgquhhg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.yfazqb.com/Article/details/gnjgvyfkd.sHtML

[U103] JS：定时器
来源：http://www.m.share.bbcook.cn/Article/details/gvipiurdv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.bbcook.cn/Article/details/gjamrmrpv.sHtML

[U104] JS：防抖
来源：http://www.blog.yfazqb.com/Article/details/gazhmdtrn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/gsackwdlo.sHtML

[U105] JS：节流
来源：http://3g.bbcook.cn/Article/details/ggwslbmbp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fktsv.cn/Article/details/gcykkhpor.sHtML

[U106] JS：日期格式化
来源：http://baike.tarul.cn/Article/details/gzmgurwnz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.sjlbkw.cn/Article/details/gqcufpxvy.sHtML

[U107] JS：数字千分位
来源：http://mobile.vehdjk.com/Article/details/gjjceqnpk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.vehdjk.com/Article/details/gxtgrlmgc.sHtML

[U108] JS：随机整数
来源：http://3g.sjlbkw.cn/Article/details/gmidegiki.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fktsv.cn/Article/details/gtnygbcoa.sHtML

[U109] JS：数组分组
来源：http://read.share.bbcook.cn/Article/details/gkxotiydu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.bbcook.cn/Article/details/gbpokxatw.sHtML

[U110] JS：数组分块
来源：http://blog.epnwcf.com/Article/details/gasivhglx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.vehdjk.com/Article/details/gccpmivnk.sHtML

[U111] JS：对象转 Map
来源：http://blog.vehdjk.com/Article/details/gfsoyhaea.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.bbcook.cn/Article/details/gbokcicxs.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fktsv.cn/Article/details/gfcfobkrx.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gduurzqgg.sHtML

[U113] JS：正则替换全部
来源：http://m.share.sjlbkw.cn/Article/details/gnhpadoii.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gbvjkbomh.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.vehdjk.com/Article/details/gqsgshjoh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.tarul.cn/Article/details/givegkjmn.sHtML

[U115] JS：生成 UUID
来源：http://3g.yfazqb.com/Article/details/glsloxcrz.sHtML

crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gotodqtpp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fktsv.cn/Article/details/gkuwinmdt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.yfazqb.com/Article/details/gbyhdgmnn.sHtML

[U117] JS：单元测试
来源：http://read.share.tarul.cn/Article/details/gxlsqqurb.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.vehdjk.com/Article/details/gahhyqljr.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.bbcook.cn/Article/details/ghtvqhbct.sHtML

npm i -D vite;  npx vite
来源：http://read.share.sjlbkw.cn/Article/details/gjgkywamz.sHtML

[U119] JS：生产构建
来源：http://www.share.yfazqb.com/Article/details/gbxxhllxz.sHtML

npx vite build
来源：http://www.blog.epnwcf.com/Article/details/gwvqdqlro.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fktsv.cn/Article/details/ggnuvygcd.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.epnwcf.com/Article/details/gvnghxlui.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gbgatndtc.sHtML

统计汇总
来源：http://3g.bbcook.cn/Article/details/guabfqcww.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/giwhhaohu.sHtML

按语言统计（条）：
来源：http://read.share.fktsv.cn/Article/details/gvoyllpdl.sHtML

Python ......... 252
来源：http://m.share.yfazqb.com/Article/details/gggodwbxu.sHtML

PHP ............ 252
来源：http://www.share.sjlbkw.cn/Article/details/ggwhrbmse.sHtML

JavaScript ..... 252
来源：http://www.m.share.vehdjk.com/Article/details/ggwelguzz.sHtML

TypeScript ..... 212
来源：http://wap.sjlbkw.cn/Article/details/gsldplzxl.sHtML

Java ........... 212
来源：http://www.share.yfazqb.com/Article/details/gsuoculli.sHtML

Go ............. 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgkswpxk.sHtML

Ruby ........... 212
来源：http://www.blog.fktsv.cn/Article/details/gruyhgtsz.sHtML

C# ............. 212
来源：http://baike.epnwcf.com/Article/details/gglnsioie.sHtML

C .............. 30
来源：http://m.share.epnwcf.com/Article/details/gmtiklrws.sHtML

C++ ............ 30
来源：http://m.share.vehdjk.com/Article/details/gyveplrwt.sHtML

SQL ............ 90
来源：http://read.share.epnwcf.com/Article/details/gtkljbztr.sHtML

Bash ........... 80
来源：http://blog.tarul.cn/Article/details/goxptxsma.sHtML

Kotlin ......... 15
来源：http://3g.vehdjk.com/Article/details/gxsolbkec.sHtML

Swift .......... 15
来源：http://mobile.tarul.cn/Article/details/gzicvoxya.sHtML

Lua ............ 10
来源：http://www.m.share.fktsv.cn/Article/details/gvxusvfzm.sHtML

Perl ........... 10
来源：http://baike.epnwcf.com/Article/details/gqjxcppue.sHtML

Scala .......... 10
来源：http://read.share.yfazqb.com/Article/details/gujuljqih.sHtML

------------------------------------
来源：http://www.share.vehdjk.com/Article/details/gkryjxugt.sHtML

合计 ........... 2106 条
来源：http://mobile.bbcook.cn/Article/details/gnlgzsbqh.sHtML

按章节统计：
来源：http://mobile.fktsv.cn/Article/details/glilcrlkq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.tarul.cn/Article/details/ggutjljok.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.tarul.cn/Article/details/ghpykojcv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.sjlbkw.cn/Article/details/grvciahjx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.sjlbkw.cn/Article/details/ghqudzdsk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.epnwcf.com/Article/details/gzunpbwfa.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.epnwcf.com/Article/details/grhmgddpy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.tarul.cn/Article/details/gnqzygcqv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.epnwcf.com/Article/details/gmdxxjhcp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gltlfhccg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.tarul.cn/Article/details/gbtknwpvp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gnxhiefgu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gextawhby.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gbuwxwrxl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fktsv.cn/Article/details/gcwubymjx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fktsv.cn/Article/details/gogbvfndw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/ghtstitqv.sHtML

Q SQL 专题                              90
来源：http://3g.vehdjk.com/Article/details/guiqcdgjm.sHtML

R Bash 专题                             80
来源：http://blog.vehdjk.com/Article/details/gfjrbjmmz.sHtML

S C / C++ 专题                          60
来源：http://wap.epnwcf.com/Article/details/golnndedr.sHtML

T 其他语言补充                          60
来源：http://www.share.fktsv.cn/Article/details/gmowucnic.sHtML

U 高频实用片段                         120
来源：http://blog.vehdjk.com/Article/details/gncuuthnm.sHtML

------------------------------------
来源：http://read.share.tarul.cn/Article/details/gvzjrdjkz.sHtML

合计                                  2106 条
来源：http://read.share.yfazqb.com/Article/details/gzwsjinfd.sHtML

--------------------------------------------------------------------------------
来源：http://baike.tarul.cn/Article/details/gnawaxgdj.sHtML

使用提醒
来源：http://www.blog.tarul.cn/Article/details/gmaeynoga.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gdelvfwqv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.vehdjk.com/Article/details/goyrblpyg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.bbcook.cn/Article/details/gqinplwfa.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.yfazqb.com/Article/details/gjywsrfaw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.yfazqb.com/Article/details/giflwwjrt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.epnwcf.com/Article/details/ggxvwpdgp.sHtML

—— 文件结束 ——
来源：http://www.share.fktsv.cn/Article/details/gnvykoyjn.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/getddenet.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.vehdjk.com/Article/details/gbvswqmtl.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fktsv.cn/Article/details/gwxxgknbw.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gdiooirmi.sHtML

【收录内容】
来源：http://blog.tarul.cn/Article/details/gjrfsavjl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fktsv.cn/Article/details/glnjqrmok.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fktsv.cn/Article/details/gvppnqaxx.sHtML

SQL · Bash · C · C++
来源：http://wap.epnwcf.com/Article/details/gkfxpuxxy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.bbcook.cn/Article/details/grcivkvei.sHtML

【使用说明】
来源：http://m.share.epnwcf.com/Article/details/gsocbfick.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.bbcook.cn/Article/details/gunchynzl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.yfazqb.com/Article/details/gabfshrqb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.yfazqb.com/Article/details/gklwrlhlt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.vehdjk.com/Article/details/gvusehyal.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.tarul.cn/Article/details/gmfbdqrys.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.epnwcf.com/Article/details/ggaalmyhf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.tarul.cn/Article/details/gvowjhtju.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.bbcook.cn/Article/details/gfcojbivt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.bbcook.cn/Article/details/gejvvrfsz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.bbcook.cn/Article/details/gdyzcuqld.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.epnwcf.com/Article/details/gccmuahex.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.vehdjk.com/Article/details/gslivxpzg.sHtML

【文件统计】
来源：http://blog.tarul.cn/Article/details/gigwbmhdi.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.sjlbkw.cn/Article/details/gbykmncom.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.bbcook.cn/Article/details/geqkdzczr.sHtML

目  录
来源：http://baike.sjlbkw.cn/Article/details/gsjwlkmob.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gqwigogwh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.bbcook.cn/Article/details/giqfqcgly.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fktsv.cn/Article/details/goudndljo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.yfazqb.com/Article/details/geyrgdczp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.bbcook.cn/Article/details/gsaspxtsv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fktsv.cn/Article/details/gohfibvml.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.epnwcf.com/Article/details/glreqxnei.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.bbcook.cn/Article/details/giqjcwctj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.epnwcf.com/Article/details/gwvsxbskn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/gacuitsti.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.vehdjk.com/Article/details/gjrigmjwg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/gfltuzuwl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/glylgegaf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fktsv.cn/Article/details/gtpxcbnfi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.sjlbkw.cn/Article/details/gijwpfked.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.vehdjk.com/Article/details/gsofbdpte.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fktsv.cn/Article/details/gxaveytzp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fktsv.cn/Article/details/gomtgscbf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.vehdjk.com/Article/details/gqteumdmt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.tarul.cn/Article/details/gctqiibqc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.vehdjk.com/Article/details/gxswzifjw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.epnwcf.com/Article/details/gseotgggz.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gdhpuiwou.sHtML

A. 基础语法与类型
来源：http://www.share.epnwcf.com/Article/details/gqpjfsvas.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gdwqhdjvq.sHtML

[A01] Hello World
来源：http://wap.fktsv.cn/Article/details/gjixucpid.sHtML

Py:   print("Hello, World!")
来源：http://mobile.sjlbkw.cn/Article/details/gupcwrttw.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.sjlbkw.cn/Article/details/gcdjwllrk.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.vehdjk.com/Article/details/gihvgfsop.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.yfazqb.com/Article/details/gmsdbvqvf.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fktsv.cn/Article/details/gscwfhuqg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.tarul.cn/Article/details/gvcqezeae.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.bbcook.cn/Article/details/gvjmuysnd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.sjlbkw.cn/Article/details/gvgfsdyva.sHtML

[A02] 变量声明与赋值
来源：http://3g.sjlbkw.cn/Article/details/gygkreamb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.yfazqb.com/Article/details/gswerksmj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.bbcook.cn/Article/details/gimesnnjt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.epnwcf.com/Article/details/grrlhphot.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.vehdjk.com/Article/details/gemnvsvfp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.sjlbkw.cn/Article/details/gvedovcck.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.sjlbkw.cn/Article/details/gixycyxkj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.bbcook.cn/Article/details/gxaiqyzab.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.vehdjk.com/Article/details/gkwzmcbhu.sHtML

[A03] 常量定义
来源：http://m.share.fktsv.cn/Article/details/gnxmtfknr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.sjlbkw.cn/Article/details/gysvlgpnv.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gwqqikurf.sHtML

JS:   const PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gpjmizcel.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gbvwewzsq.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gcizeukmb.sHtML

Go:   const PI = 3.14159
来源：http://baike.vehdjk.com/Article/details/gvloblwhl.sHtML

Ruby: PI = 3.14159
来源：http://mobile.bbcook.cn/Article/details/guqrvstpu.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gemxtxwje.sHtML

[A04] 判断变量类型
来源：http://3g.vehdjk.com/Article/details/ghhpohhve.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.sjlbkw.cn/Article/details/ghoziggni.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.vehdjk.com/Article/details/gqjfnehey.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fktsv.cn/Article/details/ggnijsdpk.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.yfazqb.com/Article/details/gqfqmyxxl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.sjlbkw.cn/Article/details/gsftdohxp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.epnwcf.com/Article/details/gitgmtsrp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.sjlbkw.cn/Article/details/gxqvexwkv.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.epnwcf.com/Article/details/ghgtqglvl.sHtML

[A05] 整数除法与取模
来源：http://mobile.yfazqb.com/Article/details/gdssqqlbu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.epnwcf.com/Article/details/gxmhsjgzk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.epnwcf.com/Article/details/graaudimq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gqxetefok.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gliginqbr.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.tarul.cn/Article/details/gtguqpnrm.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.bbcook.cn/Article/details/grvbapjbt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.fktsv.cn/Article/details/gujciwngj.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gdldhfozc.sHtML

[A06] 字符串转数字
来源：http://mobile.vehdjk.com/Article/details/gqzckakqn.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.vehdjk.com/Article/details/gjznnqakl.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fktsv.cn/Article/details/gudsbpzeb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.yfazqb.com/Article/details/gpzgyzzyp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fktsv.cn/Article/details/goxiwunqg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.epnwcf.com/Article/details/gwyhpmvta.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.yfazqb.com/Article/details/gyarufflt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.vehdjk.com/Article/details/gyzzvsztr.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fktsv.cn/Article/details/glvymagpg.sHtML

[A07] 数字转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gfuyorsez.sHtML

Py:   str(42)
来源：http://read.share.yfazqb.com/Article/details/gzgagpvlr.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.bbcook.cn/Article/details/gwuourggx.sHtML

JS:   String(42); (42).toString()
来源：http://wap.tarul.cn/Article/details/ghsvuwvgw.sHtML

TS:   String(42)
来源：http://3g.yfazqb.com/Article/details/gbecwgcki.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.sjlbkw.cn/Article/details/gfuatqjfl.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.epnwcf.com/Article/details/glwsccmyz.sHtML

Ruby: 42.to_s
来源：http://baike.yfazqb.com/Article/details/gbmojgblv.sHtML

C#:   42.ToString()
来源：http://3g.yfazqb.com/Article/details/grlqyceou.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwfrpwud.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.bbcook.cn/Article/details/gzvsmrfbs.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.vehdjk.com/Article/details/gppeshjiv.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.epnwcf.com/Article/details/gpnkfrzpu.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.epnwcf.com/Article/details/gfjrdugag.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.sjlbkw.cn/Article/details/gqnrfbklc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.epnwcf.com/Article/details/gnybzcxtp.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.tarul.cn/Article/details/gmksdokip.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.sjlbkw.cn/Article/details/gouhidkrt.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.yfazqb.com/Article/details/gajcqqhez.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.tarul.cn/Article/details/gwfleylui.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gvxcvqyju.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gcprqcbxc.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gdnxpymyq.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fktsv.cn/Article/details/ggldmojcj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjccxogb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmxlwkwc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gmlyavnxp.sHtML

[A10] 生成随机数
来源：http://wap.fktsv.cn/Article/details/gqbcslbox.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.sjlbkw.cn/Article/details/ghgwrwnix.sHtML

PHP:  random_int(1, 100);
来源：http://wap.tarul.cn/Article/details/ghnzxwpvu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.bbcook.cn/Article/details/gyxwwtfey.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.epnwcf.com/Article/details/gozmvxbrp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.sjlbkw.cn/Article/details/ghfuoutbj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.sjlbkw.cn/Article/details/guhcndikm.sHtML

Ruby: rand(1..100)
来源：http://3g.tarul.cn/Article/details/getoaqbkl.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.vehdjk.com/Article/details/guhohsbmv.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.yfazqb.com/Article/details/gtyymvsqu.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.vehdjk.com/Article/details/glycgbtgx.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.yfazqb.com/Article/details/gglowvttz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.vehdjk.com/Article/details/govqqkyfu.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.sjlbkw.cn/Article/details/gehfrzbkk.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.epnwcf.com/Article/details/gsofrdxpn.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.fktsv.cn/Article/details/ggudgaoom.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.bbcook.cn/Article/details/gkskxvweu.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.sjlbkw.cn/Article/details/gxjivahxc.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.vehdjk.com/Article/details/gibqigoja.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.vehdjk.com/Article/details/gbevhndjo.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.tarul.cn/Article/details/gmbbxpfht.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.tarul.cn/Article/details/gopeubepc.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.epnwcf.com/Article/details/gnofhzncy.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.yfazqb.com/Article/details/gevynydqb.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.tarul.cn/Article/details/gswgsecrj.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fktsv.cn/Article/details/gfzetsbun.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fktsv.cn/Article/details/gbholeoyl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.epnwcf.com/Article/details/gnsbdatph.sHtML


<!-- 参考信息 -->