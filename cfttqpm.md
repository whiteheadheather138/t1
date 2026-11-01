代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.share.tarul.cn/Article/details/guedylmkm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.vehdjk.com/Article/details/gcmtygkcm.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.bbcook.cn/Article/details/gnarbaixg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.tarul.cn/Article/details/gnvfqmmdn.sHtML

[U85] JS：可选链
来源：http://read.share.sjlbkw.cn/Article/details/gaszyonci.sHtML

a?.b?.c
来源：http://www.share.sjlbkw.cn/Article/details/gigpmcutf.sHtML

[U86] JS：空值合并
来源：http://3g.vehdjk.com/Article/details/gghaxuajb.sHtML

a ?? b
来源：http://baike.epnwcf.com/Article/details/godilfcks.sHtML

[U87] JS：解构默认值
来源：http://read.share.epnwcf.com/Article/details/gkgbztvdq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.tarul.cn/Article/details/gnrhydyin.sHtML

[U88] JS：对象展开合并
来源：http://blog.epnwcf.com/Article/details/gridarvnd.sHtML

{ ...a, ...b }
来源：http://mobile.vehdjk.com/Article/details/ghswgjsdb.sHtML

[U89] JS：数组去重
来源：http://www.share.epnwcf.com/Article/details/gdgejgoda.sHtML

[...new Set(arr)]
来源：http://www.blog.vehdjk.com/Article/details/gsxoobpnu.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.vehdjk.com/Article/details/gdtzuhjcd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/giylihbsi.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.yfazqb.com/Article/details/gismfxoac.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.vehdjk.com/Article/details/gmatlqefp.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.vehdjk.com/Article/details/goqutvwyw.sHtML

structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gzdmyvhnm.sHtML

[U93] JS：模板字符串
来源：http://www.share.fktsv.cn/Article/details/gazjmetus.sHtML

`共 ${n} 条`
来源：http://wap.sjlbkw.cn/Article/details/gxqkcmbkd.sHtML

[U94] JS：箭头函数
来源：http://blog.yfazqb.com/Article/details/gzanczvpu.sHtML

const double = x => x * 2;
来源：http://mobile.fktsv.cn/Article/details/gokziaxjf.sHtML

[U95] JS：Promise 包装
来源：http://3g.bbcook.cn/Article/details/gownleszg.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.tarul.cn/Article/details/gmrwgfjav.sHtML

[U96] JS：async/await 与异常
来源：http://wap.yfazqb.com/Article/details/gofldcvdi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gzyzkiukj.sHtML

[U97] JS：并发请求
来源：http://www.m.share.epnwcf.com/Article/details/grroebvzb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/gaiyxhilx.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.bbcook.cn/Article/details/gnzjfrwwp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.bbcook.cn/Article/details/ggoddixib.sHtML

[U99] JS：事件监听
来源：http://www.blog.fktsv.cn/Article/details/gkhbnqljb.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.vehdjk.com/Article/details/gwyrodhdl.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.tarul.cn/Article/details/gwumrxnky.sHtML

document.querySelector(".item")
来源：http://www.blog.yfazqb.com/Article/details/grpbusnlz.sHtML

[U101] JS：classList 操作
来源：http://m.share.sjlbkw.cn/Article/details/gmoiimpxg.sHtML

el.classList.toggle("active")
来源：http://wap.yfazqb.com/Article/details/gfmqwyicb.sHtML

[U102] JS：本地存储
来源：http://www.m.share.tarul.cn/Article/details/grbquistq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.sjlbkw.cn/Article/details/gacrmslba.sHtML

[U103] JS：定时器
来源：http://blog.yfazqb.com/Article/details/glxgdpgzu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.tarul.cn/Article/details/gyyqxevug.sHtML

[U104] JS：防抖
来源：http://m.share.bbcook.cn/Article/details/gdxkndbbh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gamzuwnai.sHtML

[U105] JS：节流
来源：http://www.blog.yfazqb.com/Article/details/gwpvmxcbl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.bbcook.cn/Article/details/gcajxlskw.sHtML

[U106] JS：日期格式化
来源：http://www.blog.tarul.cn/Article/details/gvleottcq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.bbcook.cn/Article/details/geqoxkxnh.sHtML

[U107] JS：数字千分位
来源：http://baike.tarul.cn/Article/details/gfxlkpyzc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/gpfjvhnvy.sHtML

[U108] JS：随机整数
来源：http://www.share.fktsv.cn/Article/details/gtmlfkbxf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.tarul.cn/Article/details/gnlfvjvmf.sHtML

[U109] JS：数组分组
来源：http://www.share.sjlbkw.cn/Article/details/gghctuphz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.sjlbkw.cn/Article/details/gqslfxvqi.sHtML

[U110] JS：数组分块
来源：http://mobile.tarul.cn/Article/details/gmuvshitl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fktsv.cn/Article/details/ggzvghskd.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fktsv.cn/Article/details/gpucsxovs.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.epnwcf.com/Article/details/gxqqekadf.sHtML

[U112] JS：字符串补位
来源：http://m.share.epnwcf.com/Article/details/gukhpikkb.sHtML

"7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gokocxqeq.sHtML

[U113] JS：正则替换全部
来源：http://wap.fktsv.cn/Article/details/geawnsxtm.sHtML

s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/grecxbyyz.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fktsv.cn/Article/details/glgmxvkec.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.epnwcf.com/Article/details/gzpwzhmeg.sHtML

[U115] JS：生成 UUID
来源：http://m.share.bbcook.cn/Article/details/ggktocdtk.sHtML

crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/glenjdttf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fktsv.cn/Article/details/gdzluccae.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.vehdjk.com/Article/details/gmjweodan.sHtML

[U117] JS：单元测试
来源：http://m.share.fktsv.cn/Article/details/gouooaflj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fktsv.cn/Article/details/grrummhut.sHtML

[U118] JS：开发服务器
来源：http://mobile.bbcook.cn/Article/details/gvezosjhc.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.sjlbkw.cn/Article/details/gnyrthgfx.sHtML

[U119] JS：生产构建
来源：http://mobile.sjlbkw.cn/Article/details/gnjnkuudy.sHtML

npx vite build
来源：http://www.share.vehdjk.com/Article/details/gfcinibmh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fktsv.cn/Article/details/gkzszrcsu.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.sjlbkw.cn/Article/details/gwzhgcufk.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gtouogocq.sHtML

统计汇总
来源：http://m.share.sjlbkw.cn/Article/details/gcufhdjwv.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gafrqnozb.sHtML

按语言统计（条）：
来源：http://blog.yfazqb.com/Article/details/ghnnzhmkk.sHtML

Python ......... 252
来源：http://www.blog.tarul.cn/Article/details/gnxmcqpiz.sHtML

PHP ............ 252
来源：http://mobile.bbcook.cn/Article/details/gsjyxpmxr.sHtML

JavaScript ..... 252
来源：http://mobile.tarul.cn/Article/details/gwlbviyns.sHtML

TypeScript ..... 212
来源：http://www.m.share.tarul.cn/Article/details/gquyfvovm.sHtML

Java ........... 212
来源：http://3g.tarul.cn/Article/details/gqnvywtwf.sHtML

Go ............. 212
来源：http://blog.yfazqb.com/Article/details/gnvnrapsx.sHtML

Ruby ........... 212
来源：http://m.share.bbcook.cn/Article/details/gwceqiaat.sHtML

C# ............. 212
来源：http://www.m.share.epnwcf.com/Article/details/gpldeeynh.sHtML

C .............. 30
来源：http://mobile.bbcook.cn/Article/details/gsbzzdxas.sHtML

C++ ............ 30
来源：http://blog.sjlbkw.cn/Article/details/gpwmykftw.sHtML

SQL ............ 90
来源：http://blog.fktsv.cn/Article/details/gnbxyrals.sHtML

Bash ........... 80
来源：http://www.m.share.epnwcf.com/Article/details/gubnvfufl.sHtML

Kotlin ......... 15
来源：http://blog.fktsv.cn/Article/details/gauliudkt.sHtML

Swift .......... 15
来源：http://mobile.fktsv.cn/Article/details/gkqkrskek.sHtML

Lua ............ 10
来源：http://m.share.vehdjk.com/Article/details/gnkxhwzpe.sHtML

Perl ........... 10
来源：http://blog.vehdjk.com/Article/details/gwcibfdad.sHtML

Scala .......... 10
来源：http://m.share.bbcook.cn/Article/details/glflriwqn.sHtML

------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gsmqabpiq.sHtML

合计 ........... 2106 条
来源：http://wap.bbcook.cn/Article/details/gbxfidmzt.sHtML

按章节统计：
来源：http://www.m.share.tarul.cn/Article/details/gkhqyqgsj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.bbcook.cn/Article/details/ghgvcwcfa.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fktsv.cn/Article/details/gzjhqqgcs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.sjlbkw.cn/Article/details/gpgxeunwl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.sjlbkw.cn/Article/details/gwlrskoja.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.tarul.cn/Article/details/gmznbvkss.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.epnwcf.com/Article/details/gkxzsdkeh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.sjlbkw.cn/Article/details/gisfcfrxd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.vehdjk.com/Article/details/gidfgrlss.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/gqixoggfw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.sjlbkw.cn/Article/details/gjvsvejpy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/grwqwwdbq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/gaxfmoyuj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/ghckbktfh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.yfazqb.com/Article/details/gegpcpcbs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.tarul.cn/Article/details/goagnekxe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/gfcpnykvn.sHtML

Q SQL 专题                              90
来源：http://www.share.sjlbkw.cn/Article/details/gsqxjtdiw.sHtML

R Bash 专题                             80
来源：http://wap.sjlbkw.cn/Article/details/gpukakctx.sHtML

S C / C++ 专题                          60
来源：http://blog.fktsv.cn/Article/details/gqezbvtza.sHtML

T 其他语言补充                          60
来源：http://mobile.sjlbkw.cn/Article/details/gijvxhhur.sHtML

U 高频实用片段                         120
来源：http://www.share.yfazqb.com/Article/details/glhlytylj.sHtML

------------------------------------
来源：http://3g.tarul.cn/Article/details/goojnoewk.sHtML

合计                                  2106 条
来源：http://mobile.epnwcf.com/Article/details/guhnswjjp.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.tarul.cn/Article/details/gxuppleyu.sHtML

使用提醒
来源：http://baike.vehdjk.com/Article/details/gymzrljfk.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gcozvmxhg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.yfazqb.com/Article/details/gkjsegxdd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.yfazqb.com/Article/details/gaokyynxe.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.epnwcf.com/Article/details/gjjdovkcy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.tarul.cn/Article/details/grmurgrxg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.tarul.cn/Article/details/gcbinlpnj.sHtML

—— 文件结束 ——
来源：http://mobile.tarul.cn/Article/details/gxhbbiwvc.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gltdueakq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.epnwcf.com/Article/details/gougmoend.sHtML

Common Programming Examples Cheat Book
来源：http://wap.sjlbkw.cn/Article/details/grlspfvna.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gaxaigxbf.sHtML

【收录内容】
来源：http://mobile.sjlbkw.cn/Article/details/gaauqjevf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.vehdjk.com/Article/details/gjtujhcku.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.sjlbkw.cn/Article/details/gbiamkquh.sHtML

SQL · Bash · C · C++
来源：http://3g.fktsv.cn/Article/details/gxovwmaiv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.sjlbkw.cn/Article/details/galojkezc.sHtML

【使用说明】
来源：http://wap.bbcook.cn/Article/details/gyggbjgee.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.epnwcf.com/Article/details/ggrsrwhic.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.tarul.cn/Article/details/gegxlgbeb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.epnwcf.com/Article/details/gllsvmwix.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.epnwcf.com/Article/details/gdtqdoltc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.bbcook.cn/Article/details/gbjxhtavh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.sjlbkw.cn/Article/details/gdlylivmm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.vehdjk.com/Article/details/gdxkdgpkv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.bbcook.cn/Article/details/gfzprjmly.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.epnwcf.com/Article/details/gzadzazuw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fktsv.cn/Article/details/gkadhtnck.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.bbcook.cn/Article/details/giyzpiesb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.yfazqb.com/Article/details/gjkvgpwvl.sHtML

【文件统计】
来源：http://wap.fktsv.cn/Article/details/gjvhnxelc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fktsv.cn/Article/details/gagvglocn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/gjbgulrtx.sHtML

目  录
来源：http://mobile.fktsv.cn/Article/details/gquhpgwzc.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.tarul.cn/Article/details/gftvdszyo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.tarul.cn/Article/details/gknejdmal.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.vehdjk.com/Article/details/gxtqqpjjl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.tarul.cn/Article/details/gurniagez.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fktsv.cn/Article/details/glymszaeg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.vehdjk.com/Article/details/goxdllakn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdnlbjjk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.yfazqb.com/Article/details/gsgibqann.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.sjlbkw.cn/Article/details/gvnszmhnf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.epnwcf.com/Article/details/gzaiqipeh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.sjlbkw.cn/Article/details/giofwlpnm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gyvxcemzn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.bbcook.cn/Article/details/gbnnvcdmq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.bbcook.cn/Article/details/getphrtgs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.vehdjk.com/Article/details/gamgfxrly.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.vehdjk.com/Article/details/gpqgomugw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/gzvozwyjt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.yfazqb.com/Article/details/gjbujppwj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.epnwcf.com/Article/details/gxprfovtk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.yfazqb.com/Article/details/gceqhkmie.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.vehdjk.com/Article/details/gifpgrbyr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.yfazqb.com/Article/details/gpojghslw.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gvplhadtd.sHtML

A. 基础语法与类型
来源：http://www.blog.tarul.cn/Article/details/gtuxzmime.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gtbqzsxlg.sHtML

[A01] Hello World
来源：http://www.blog.vehdjk.com/Article/details/garpicyik.sHtML

Py:   print("Hello, World!")
来源：http://wap.fktsv.cn/Article/details/gonhvvvlp.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.epnwcf.com/Article/details/gquyxasgd.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.tarul.cn/Article/details/geypmhswx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fktsv.cn/Article/details/glvwxvpmy.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.tarul.cn/Article/details/gzzkdwwcc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.tarul.cn/Article/details/ggrhpwuex.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.tarul.cn/Article/details/gslpkdvkz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fktsv.cn/Article/details/ggxyfdmkj.sHtML

[A02] 变量声明与赋值
来源：http://baike.epnwcf.com/Article/details/ggfpgbpqt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.yfazqb.com/Article/details/gtoyylhnn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.bbcook.cn/Article/details/gbysehjvz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fktsv.cn/Article/details/ggyrsklzz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fktsv.cn/Article/details/geadfqdpn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fktsv.cn/Article/details/gguybexri.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.epnwcf.com/Article/details/gxnujfyiz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fktsv.cn/Article/details/gavbcgbud.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.yfazqb.com/Article/details/gvtlidmno.sHtML

[A03] 常量定义
来源：http://baike.yfazqb.com/Article/details/gcowzfwha.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.vehdjk.com/Article/details/gcqupvvos.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/geinsdsno.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/givuwwozf.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gznfeomqd.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gxwyfdshj.sHtML

Go:   const PI = 3.14159
来源：http://3g.vehdjk.com/Article/details/gcaslaijw.sHtML

Ruby: PI = 3.14159
来源：http://blog.yfazqb.com/Article/details/gqhxpiruu.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gyppgxnzi.sHtML

[A04] 判断变量类型
来源：http://blog.fktsv.cn/Article/details/gziqoqcfq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.tarul.cn/Article/details/gwliuwlre.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.tarul.cn/Article/details/ggtnwdcxx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.bbcook.cn/Article/details/gdpicjvbz.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.vehdjk.com/Article/details/grwvtjild.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.bbcook.cn/Article/details/gkvivwmsg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.epnwcf.com/Article/details/gwtwcoqqa.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.yfazqb.com/Article/details/gwdonvome.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.tarul.cn/Article/details/gvkvveusd.sHtML

[A05] 整数除法与取模
来源：http://baike.tarul.cn/Article/details/gpoqrnont.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.tarul.cn/Article/details/ggbpcfwmw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fktsv.cn/Article/details/ggprlwccp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.epnwcf.com/Article/details/glgvokyex.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.bbcook.cn/Article/details/gydphukha.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gmaxgfdol.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.yfazqb.com/Article/details/gqqsjwmtp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gciwfbtjo.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fktsv.cn/Article/details/gyquwlate.sHtML

[A06] 字符串转数字
来源：http://www.share.epnwcf.com/Article/details/ggvncwavx.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fktsv.cn/Article/details/gystmdvsu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.tarul.cn/Article/details/ggmphzjjn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.epnwcf.com/Article/details/guymxwsvs.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.yfazqb.com/Article/details/gqccdykye.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.bbcook.cn/Article/details/gbqfbuwwk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.yfazqb.com/Article/details/giuhlfife.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.vehdjk.com/Article/details/gtrlbwhlx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.yfazqb.com/Article/details/gwzcwbkdh.sHtML

[A07] 数字转字符串
来源：http://m.share.epnwcf.com/Article/details/gkuholyla.sHtML

Py:   str(42)
来源：http://read.share.fktsv.cn/Article/details/gilwslnai.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.vehdjk.com/Article/details/grxefjndb.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.bbcook.cn/Article/details/gtxvetrmo.sHtML

TS:   String(42)
来源：http://www.share.bbcook.cn/Article/details/gxhgtpnwd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.sjlbkw.cn/Article/details/gcenrvqnf.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.vehdjk.com/Article/details/ghjhadwdy.sHtML

Ruby: 42.to_s
来源：http://baike.fktsv.cn/Article/details/gulhqszwi.sHtML

C#:   42.ToString()
来源：http://blog.fktsv.cn/Article/details/gbsruecdb.sHtML

[A08] 取整与四舍五入
来源：http://mobile.yfazqb.com/Article/details/guwazmxvj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.epnwcf.com/Article/details/gehjlvzje.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.yfazqb.com/Article/details/gwyrjohma.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.vehdjk.com/Article/details/gamgfqayj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.tarul.cn/Article/details/grhznzzzz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.yfazqb.com/Article/details/gemqnmapo.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.vehdjk.com/Article/details/ghjliftnz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.fktsv.cn/Article/details/gqedoplzy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.bbcook.cn/Article/details/gbenfeodu.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fktsv.cn/Article/details/gyttzldft.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.tarul.cn/Article/details/gtvhxgjsj.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.vehdjk.com/Article/details/gcwplqrav.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.epnwcf.com/Article/details/gengcjdca.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gzsulvztv.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.fktsv.cn/Article/details/gsmhdvuyl.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.tarul.cn/Article/details/givsanbuy.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.yfazqb.com/Article/details/gazjxexgv.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gajnmivsy.sHtML

[A10] 生成随机数
来源：http://wap.bbcook.cn/Article/details/ghytamrjn.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.fktsv.cn/Article/details/gcepouczt.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fktsv.cn/Article/details/glmnbrrjb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.epnwcf.com/Article/details/gtcuskgfh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.sjlbkw.cn/Article/details/gujmyqjxh.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.epnwcf.com/Article/details/gwgawtzcc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.epnwcf.com/Article/details/gpobkqfod.sHtML

Ruby: rand(1..100)
来源：http://wap.fktsv.cn/Article/details/glnvsjzac.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.epnwcf.com/Article/details/gvisojeeu.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.bbcook.cn/Article/details/gqbechncf.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.epnwcf.com/Article/details/gglgvnqax.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.bbcook.cn/Article/details/gksarxewj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.vehdjk.com/Article/details/gmxfxhcqc.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.epnwcf.com/Article/details/gvrskvmxi.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/gosjkdolr.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.yfazqb.com/Article/details/gjvkjnkql.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.vehdjk.com/Article/details/goiuvqlmz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gekqbotht.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.tarul.cn/Article/details/glnylweps.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.bbcook.cn/Article/details/gwwhussck.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.epnwcf.com/Article/details/gsbhzvrea.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.epnwcf.com/Article/details/grndftpeu.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.sjlbkw.cn/Article/details/gjixypgoj.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.epnwcf.com/Article/details/gdrdksfwq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fktsv.cn/Article/details/gkqivflvx.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.tarul.cn/Article/details/gjzdymxiu.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.tarul.cn/Article/details/gwnovqtkb.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.fktsv.cn/Article/details/gnfueecgn.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/gsacbjhfh.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/gwxvinfnd.sHtML

JS:   "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/gfqldejkl.sHtML

TS:   "第一行\n第二行"
来源：http://wap.vehdjk.com/Article/details/gnuhbfqbd.sHtML

Java: "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gwvlqoxqu.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.tarul.cn/Article/details/gdiltrpxl.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/gnphqbaor.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/gbmnxbrbw.sHtML


<!-- 参考信息 -->