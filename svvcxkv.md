代发 wailian999

[U91] JS：对象键值遍历
来源：http://m.share.tarul.cn/Article/details/gifvmllig.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.yfazqb.com/Article/details/gagbzynea.sHtML

[U92] JS：深拷贝
来源：http://wap.fktsv.cn/Article/details/gswjqgupi.sHtML

structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/ggiztoxpm.sHtML

[U93] JS：模板字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gajfetrxf.sHtML

`共 ${n} 条`
来源：http://read.share.epnwcf.com/Article/details/gdsoywofg.sHtML

[U94] JS：箭头函数
来源：http://3g.sjlbkw.cn/Article/details/gyvqrgsto.sHtML

const double = x => x * 2;
来源：http://3g.epnwcf.com/Article/details/gpamsvwzu.sHtML

[U95] JS：Promise 包装
来源：http://wap.yfazqb.com/Article/details/ggdxnoyqi.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fktsv.cn/Article/details/gtrpctoyf.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.sjlbkw.cn/Article/details/givfkwegp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/godipyhbs.sHtML

[U97] JS：并发请求
来源：http://mobile.bbcook.cn/Article/details/gshzoplae.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/ghkevqdmj.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.tarul.cn/Article/details/glwrbrwer.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.epnwcf.com/Article/details/gwkjfrvdu.sHtML

[U99] JS：事件监听
来源：http://blog.bbcook.cn/Article/details/ghlplyvoa.sHtML

el.addEventListener("click", e => {})
来源：http://baike.tarul.cn/Article/details/gezejkvuz.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.bbcook.cn/Article/details/gwrjxeljy.sHtML

document.querySelector(".item")
来源：http://www.share.bbcook.cn/Article/details/goqimkxlt.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fktsv.cn/Article/details/gfqvjkaca.sHtML

el.classList.toggle("active")
来源：http://www.m.share.yfazqb.com/Article/details/gxqwlfiae.sHtML

[U102] JS：本地存储
来源：http://www.share.fktsv.cn/Article/details/gegvkryqx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.bbcook.cn/Article/details/ggijxbekc.sHtML

[U103] JS：定时器
来源：http://blog.sjlbkw.cn/Article/details/gwogpubrf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.bbcook.cn/Article/details/gdxldkqrh.sHtML

[U104] JS：防抖
来源：http://www.m.share.fktsv.cn/Article/details/gzcgvtswj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fktsv.cn/Article/details/geqydlvlg.sHtML

[U105] JS：节流
来源：http://read.share.epnwcf.com/Article/details/gkncgopco.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.vehdjk.com/Article/details/gnxovcuah.sHtML

[U106] JS：日期格式化
来源：http://read.share.yfazqb.com/Article/details/gwkdfxqah.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.bbcook.cn/Article/details/ggaarfiqs.sHtML

[U107] JS：数字千分位
来源：http://baike.bbcook.cn/Article/details/gtldpzbva.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/gnzwmljae.sHtML

[U108] JS：随机整数
来源：http://baike.tarul.cn/Article/details/gpjztllbg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.tarul.cn/Article/details/gvifajxfj.sHtML

[U109] JS：数组分组
来源：http://www.share.epnwcf.com/Article/details/grenpjjuq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.yfazqb.com/Article/details/gokkfcync.sHtML

[U110] JS：数组分块
来源：http://www.share.sjlbkw.cn/Article/details/geagdfiid.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fktsv.cn/Article/details/gycdqowta.sHtML

[U111] JS：对象转 Map
来源：http://m.share.bbcook.cn/Article/details/glmtrczez.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fktsv.cn/Article/details/gjnjdgutq.sHtML

[U112] JS：字符串补位
来源：http://m.share.epnwcf.com/Article/details/gzgorlqpw.sHtML

"7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gthlymdqs.sHtML

[U113] JS：正则替换全部
来源：http://blog.vehdjk.com/Article/details/gziozizlr.sHtML

s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gujovjxwa.sHtML

[U114] JS：JSON 深比较
来源：http://baike.tarul.cn/Article/details/gsdvqyoap.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.bbcook.cn/Article/details/gjvkjjltx.sHtML

[U115] JS：生成 UUID
来源：http://baike.yfazqb.com/Article/details/glfilkfst.sHtML

crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gafyebjvk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.epnwcf.com/Article/details/grwgttfov.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.tarul.cn/Article/details/gqisomdgk.sHtML

[U117] JS：单元测试
来源：http://www.m.share.sjlbkw.cn/Article/details/gktiindux.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.yfazqb.com/Article/details/gstgqruvm.sHtML

[U118] JS：开发服务器
来源：http://www.share.epnwcf.com/Article/details/gubxnyjoq.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.yfazqb.com/Article/details/gcylitgrp.sHtML

[U119] JS：生产构建
来源：http://m.share.vehdjk.com/Article/details/ggifwahkb.sHtML

npx vite build
来源：http://blog.tarul.cn/Article/details/ggizafmkw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.sjlbkw.cn/Article/details/ghdddcugo.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.yfazqb.com/Article/details/ghrjgfoti.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ghtoxdrnh.sHtML

统计汇总
来源：http://mobile.epnwcf.com/Article/details/gfjmoalnl.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gomqzetpc.sHtML

按语言统计（条）：
来源：http://blog.sjlbkw.cn/Article/details/gocjtfcgq.sHtML

Python ......... 252
来源：http://mobile.sjlbkw.cn/Article/details/gfotnyxvz.sHtML

PHP ............ 252
来源：http://blog.fktsv.cn/Article/details/gansojgst.sHtML

JavaScript ..... 252
来源：http://mobile.tarul.cn/Article/details/graadcqyt.sHtML

TypeScript ..... 212
来源：http://www.share.vehdjk.com/Article/details/guptlktyz.sHtML

Java ........... 212
来源：http://baike.sjlbkw.cn/Article/details/gsaeayjtg.sHtML

Go ............. 212
来源：http://blog.fktsv.cn/Article/details/gwwsxjzxc.sHtML

Ruby ........... 212
来源：http://www.blog.tarul.cn/Article/details/gonnropwh.sHtML

C# ............. 212
来源：http://www.blog.vehdjk.com/Article/details/gozfxitxt.sHtML

C .............. 30
来源：http://www.share.sjlbkw.cn/Article/details/ghtletfhe.sHtML

C++ ............ 30
来源：http://mobile.yfazqb.com/Article/details/gddicgubm.sHtML

SQL ............ 90
来源：http://www.m.share.epnwcf.com/Article/details/gtwhuxyzp.sHtML

Bash ........... 80
来源：http://mobile.fktsv.cn/Article/details/gusxwhafb.sHtML

Kotlin ......... 15
来源：http://www.blog.vehdjk.com/Article/details/gilvqeuka.sHtML

Swift .......... 15
来源：http://blog.epnwcf.com/Article/details/ggynzwino.sHtML

Lua ............ 10
来源：http://www.m.share.tarul.cn/Article/details/gzrnocdyt.sHtML

Perl ........... 10
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzglhxex.sHtML

Scala .......... 10
来源：http://www.blog.yfazqb.com/Article/details/gzumwryhs.sHtML

------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gynedpvyw.sHtML

合计 ........... 2106 条
来源：http://mobile.tarul.cn/Article/details/gghoyhlek.sHtML

按章节统计：
来源：http://mobile.bbcook.cn/Article/details/gsatkksvm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fktsv.cn/Article/details/gbbyzyohf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.epnwcf.com/Article/details/gmtiaamlq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.bbcook.cn/Article/details/gewmyjhzz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.vehdjk.com/Article/details/gzhwxcscw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.epnwcf.com/Article/details/gunhshrnq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.yfazqb.com/Article/details/gfbtnqrkx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.vehdjk.com/Article/details/ghpwpivxu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.vehdjk.com/Article/details/ghfdemkpg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gebvkoihw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.sjlbkw.cn/Article/details/gmrickwhq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/gmvomoxhq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/gacxxebza.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/guzjiivfm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.tarul.cn/Article/details/gpbjnveil.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fktsv.cn/Article/details/gjbmvxcbr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/gnebjhgtm.sHtML

Q SQL 专题                              90
来源：http://www.blog.epnwcf.com/Article/details/goshxotbh.sHtML

R Bash 专题                             80
来源：http://3g.bbcook.cn/Article/details/gerosggpl.sHtML

S C / C++ 专题                          60
来源：http://read.share.sjlbkw.cn/Article/details/gripmnkxd.sHtML

T 其他语言补充                          60
来源：http://m.share.epnwcf.com/Article/details/gmebxjiwd.sHtML

U 高频实用片段                         120
来源：http://mobile.epnwcf.com/Article/details/gcjunxcgv.sHtML

------------------------------------
来源：http://blog.epnwcf.com/Article/details/gffsatmdw.sHtML

合计                                  2106 条
来源：http://3g.fktsv.cn/Article/details/gvoojxxga.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gxgqpgjfb.sHtML

使用提醒
来源：http://m.share.fktsv.cn/Article/details/gnprixytf.sHtML

--------------------------------------------------------------------------------
来源：http://blog.epnwcf.com/Article/details/ghjcgmabr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.sjlbkw.cn/Article/details/gtirlfhwc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.yfazqb.com/Article/details/gqgvhbchb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.bbcook.cn/Article/details/gfckkvnvr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.bbcook.cn/Article/details/grucbppud.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fktsv.cn/Article/details/gaezwyinw.sHtML

—— 文件结束 ——
来源：http://blog.epnwcf.com/Article/details/gbvnsyxry.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gjbndxcjw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fktsv.cn/Article/details/gozaylxmm.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.vehdjk.com/Article/details/gdxcaycak.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gruhwmzny.sHtML

【收录内容】
来源：http://www.blog.sjlbkw.cn/Article/details/gppmpuaqo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.yfazqb.com/Article/details/gmgqzvjkg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.vehdjk.com/Article/details/gyvzqxtey.sHtML

SQL · Bash · C · C++
来源：http://blog.yfazqb.com/Article/details/gyjtivxxj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.bbcook.cn/Article/details/gvfdlquyt.sHtML

【使用说明】
来源：http://www.blog.tarul.cn/Article/details/glswjruah.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fktsv.cn/Article/details/goigtogcp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.tarul.cn/Article/details/gxuguupgj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fktsv.cn/Article/details/gtugnhygr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.sjlbkw.cn/Article/details/guaufrrar.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.yfazqb.com/Article/details/gqdxazckk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.bbcook.cn/Article/details/grnxkgmcg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.bbcook.cn/Article/details/ghsyemmqt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.tarul.cn/Article/details/gotwjsyki.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.tarul.cn/Article/details/gkqdegxaf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.epnwcf.com/Article/details/gficlvxsx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.bbcook.cn/Article/details/ghiqnbvhx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.tarul.cn/Article/details/gzgrhgidh.sHtML

【文件统计】
来源：http://www.m.share.bbcook.cn/Article/details/gnxoukfue.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.tarul.cn/Article/details/gbpbfakit.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gsheurism.sHtML

目  录
来源：http://www.m.share.fktsv.cn/Article/details/gjppfnamg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gwjjactlr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.yfazqb.com/Article/details/gmyovghdr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.epnwcf.com/Article/details/gopoaxbxw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.sjlbkw.cn/Article/details/gzhejveqf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fktsv.cn/Article/details/gvmzieqax.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.yfazqb.com/Article/details/ggsrpmxib.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.vehdjk.com/Article/details/gccobppls.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/gbmmmgdvh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.bbcook.cn/Article/details/gejrihgzp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.epnwcf.com/Article/details/gbgzgfwpr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.sjlbkw.cn/Article/details/gkpxewavm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/gqxoeuayz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.yfazqb.com/Article/details/gwjugmmyw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/gitqzocvc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.yfazqb.com/Article/details/gdwkhykeq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.bbcook.cn/Article/details/guhkldjvk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/gqxzexvlt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.bbcook.cn/Article/details/ghvyasush.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.tarul.cn/Article/details/gwklehahf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.yfazqb.com/Article/details/gvgyhnouj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fktsv.cn/Article/details/gahavafso.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.yfazqb.com/Article/details/gobhzczto.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gjpujfrce.sHtML

A. 基础语法与类型
来源：http://mobile.epnwcf.com/Article/details/gznywwhei.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnckpznip.sHtML

[A01] Hello World
来源：http://wap.bbcook.cn/Article/details/gbztvttja.sHtML

Py:   print("Hello, World!")
来源：http://wap.vehdjk.com/Article/details/gykryrzfo.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.bbcook.cn/Article/details/gvsilbbti.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.bbcook.cn/Article/details/giosqkzrt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.sjlbkw.cn/Article/details/gsawwzybu.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.bbcook.cn/Article/details/gzsmvhnyc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.sjlbkw.cn/Article/details/gpvrywlom.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.yfazqb.com/Article/details/gpvwopzzu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.yfazqb.com/Article/details/ggsoxgyca.sHtML

[A02] 变量声明与赋值
来源：http://m.share.epnwcf.com/Article/details/gcfelxeai.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.bbcook.cn/Article/details/gzzxiosrk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fktsv.cn/Article/details/ghozhsiqv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.yfazqb.com/Article/details/gkbbrxdef.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.vehdjk.com/Article/details/gjfswqqxa.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.vehdjk.com/Article/details/gdmxljjji.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.yfazqb.com/Article/details/gydcguixq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.bbcook.cn/Article/details/gamnjzchu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.tarul.cn/Article/details/gjztmqfeu.sHtML

[A03] 常量定义
来源：http://3g.tarul.cn/Article/details/giqcipyob.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.bbcook.cn/Article/details/gaqtgojys.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/guvcttfjt.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gwywrvtfm.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gydmpocpt.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gyjjpohgj.sHtML

Go:   const PI = 3.14159
来源：http://baike.tarul.cn/Article/details/ghyrdcmln.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.bbcook.cn/Article/details/gouyenapo.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gjolncfkm.sHtML

[A04] 判断变量类型
来源：http://mobile.yfazqb.com/Article/details/gzzpctpge.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.bbcook.cn/Article/details/gpgmbwgxg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.bbcook.cn/Article/details/gxgenowoc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.bbcook.cn/Article/details/gcqkmptkp.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fktsv.cn/Article/details/gwlccnsip.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.tarul.cn/Article/details/gkkgcmctv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.yfazqb.com/Article/details/gbmiafoqf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.tarul.cn/Article/details/gfxfvjqjq.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.vehdjk.com/Article/details/glnefwfiv.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.epnwcf.com/Article/details/ganqeapbo.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.yfazqb.com/Article/details/gjsidzxnt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/gefaxocli.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gdfizkxwb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fktsv.cn/Article/details/gvprzozfr.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzhlvdmp.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fktsv.cn/Article/details/gtlbrxyxy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.vehdjk.com/Article/details/gnbqtighw.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fktsv.cn/Article/details/giogbxzrv.sHtML

[A06] 字符串转数字
来源：http://www.m.share.yfazqb.com/Article/details/gubvailfu.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.epnwcf.com/Article/details/gaesuzzhs.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.epnwcf.com/Article/details/gkchopcrz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fktsv.cn/Article/details/ghotejhuu.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.vehdjk.com/Article/details/gpyynzqtr.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.yfazqb.com/Article/details/ghlvvraio.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.tarul.cn/Article/details/gwqnzzpsy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.vehdjk.com/Article/details/gdtuovdni.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fktsv.cn/Article/details/gununpeux.sHtML

[A07] 数字转字符串
来源：http://m.share.yfazqb.com/Article/details/gpxizsejp.sHtML

Py:   str(42)
来源：http://www.blog.bbcook.cn/Article/details/gbodkxygh.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.bbcook.cn/Article/details/gmhqkymqg.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.yfazqb.com/Article/details/gbsytympj.sHtML

TS:   String(42)
来源：http://baike.vehdjk.com/Article/details/ghslfuqhe.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.yfazqb.com/Article/details/gwsqanzoo.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.bbcook.cn/Article/details/gcqvaamof.sHtML

Ruby: 42.to_s
来源：http://m.share.yfazqb.com/Article/details/guetxvfzx.sHtML

C#:   42.ToString()
来源：http://baike.bbcook.cn/Article/details/gscchtjbn.sHtML

[A08] 取整与四舍五入
来源：http://m.share.bbcook.cn/Article/details/gnsrvzysx.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.vehdjk.com/Article/details/gxebfbtne.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.sjlbkw.cn/Article/details/gohwzfsux.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.tarul.cn/Article/details/gtevyakda.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.sjlbkw.cn/Article/details/gzjbukmru.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.fktsv.cn/Article/details/gdlzhmfog.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/gahrpkxbu.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.epnwcf.com/Article/details/gpewpghko.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.fktsv.cn/Article/details/gpoundyui.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.yfazqb.com/Article/details/gzefjfpaw.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.yfazqb.com/Article/details/gixtctagx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.bbcook.cn/Article/details/grvcepxlm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.tarul.cn/Article/details/gwgalwgbn.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gnoybaqox.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gevqmyrsm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.bbcook.cn/Article/details/ghcnotnjj.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.sjlbkw.cn/Article/details/gxdsykcze.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.bbcook.cn/Article/details/ghpbbuypd.sHtML

[A10] 生成随机数
来源：http://3g.bbcook.cn/Article/details/gdtwjspif.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.bbcook.cn/Article/details/gtuneezlf.sHtML

PHP:  random_int(1, 100);
来源：http://wap.tarul.cn/Article/details/gufkokdya.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fktsv.cn/Article/details/gcenpijvp.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.bbcook.cn/Article/details/gebszwkjm.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.tarul.cn/Article/details/gcguavfjo.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.sjlbkw.cn/Article/details/gnrqdynqv.sHtML

Ruby: rand(1..100)
来源：http://read.share.bbcook.cn/Article/details/gsvfykyre.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.vehdjk.com/Article/details/gznwkznzo.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fktsv.cn/Article/details/gelgwzymh.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.yfazqb.com/Article/details/gcepdhinp.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.yfazqb.com/Article/details/gmioqnpxr.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.fktsv.cn/Article/details/gsowufqkf.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.sjlbkw.cn/Article/details/gxjphfcsv.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.sjlbkw.cn/Article/details/gzcradxmk.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.sjlbkw.cn/Article/details/gqjvfkyvh.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.bbcook.cn/Article/details/gcifyzwkr.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/gsnkzoojz.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.bbcook.cn/Article/details/gxdwdetzp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.epnwcf.com/Article/details/grnejaqkl.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fktsv.cn/Article/details/gsqyrjdaz.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.tarul.cn/Article/details/gjvoxzkwz.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.tarul.cn/Article/details/glcdecnca.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.yfazqb.com/Article/details/giyilvpeb.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.bbcook.cn/Article/details/gtprkknys.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.tarul.cn/Article/details/gttitnnma.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.vehdjk.com/Article/details/gfbtyrppc.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.tarul.cn/Article/details/gqwdqteqx.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gypfnpbwx.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/gebjfcbdn.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/gysjzfypw.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/gkuyqylbu.sHtML

Java: "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gzfivpcip.sHtML

Go:   "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/geoyssodc.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gvpyjxehp.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/gvpeudbgm.sHtML

[A14] 注释写法
来源：http://wap.fktsv.cn/Article/details/gzgvvzpmg.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.vehdjk.com/Article/details/gofmksvyb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.yfazqb.com/Article/details/gnszliqql.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.bbcook.cn/Article/details/gwomhfvse.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fktsv.cn/Article/details/gjclkxxnf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.tarul.cn/Article/details/guzcqnznb.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.tarul.cn/Article/details/ggbltkgvl.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.bbcook.cn/Article/details/gjwyiznbx.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/gzjkjepov.sHtML

[A15] 空值判断与默认值
来源：http://wap.fktsv.cn/Article/details/gpnoirwfk.sHtML

Py:   value = data or "默认值"
来源：http://3g.sjlbkw.cn/Article/details/gnllzibez.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.yfazqb.com/Article/details/gcqaylhnn.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.epnwcf.com/Article/details/gzlseiymc.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.epnwcf.com/Article/details/gyokimwfh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.vehdjk.com/Article/details/gbmddrnlr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.vehdjk.com/Article/details/gryfvmfpt.sHtML


<!-- 参考信息 -->