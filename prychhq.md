代发 wailian999

[U87] JS：解构默认值
来源：http://wap.bbcook.cn/Article/details/gtkvzpukb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.bbcook.cn/Article/details/gzjqxrudy.sHtML

[U88] JS：对象展开合并
来源：http://mobile.bbcook.cn/Article/details/gncgtykff.sHtML

{ ...a, ...b }
来源：http://www.blog.tarul.cn/Article/details/gtydhxbmu.sHtML

[U89] JS：数组去重
来源：http://read.share.sjlbkw.cn/Article/details/gdngxjkad.sHtML

[...new Set(arr)]
来源：http://m.share.bbcook.cn/Article/details/gowhvyqvo.sHtML

[U90] JS：数字数组排序
来源：http://blog.vehdjk.com/Article/details/glkfgfguq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/ggqezfewd.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.epnwcf.com/Article/details/gegbfgwvm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.tarul.cn/Article/details/gwuaorqws.sHtML

[U92] JS：深拷贝
来源：http://mobile.tarul.cn/Article/details/guntaopdr.sHtML

structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/gdhfniwrz.sHtML

[U93] JS：模板字符串
来源：http://www.blog.bbcook.cn/Article/details/gtpmeuxwy.sHtML

`共 ${n} 条`
来源：http://m.share.tarul.cn/Article/details/gakynyudz.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fktsv.cn/Article/details/gdqzfxukc.sHtML

const double = x => x * 2;
来源：http://www.share.bbcook.cn/Article/details/gzyvdetpd.sHtML

[U95] JS：Promise 包装
来源：http://blog.fktsv.cn/Article/details/gruesrvyk.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.vehdjk.com/Article/details/gofvgqoye.sHtML

[U96] JS：async/await 与异常
来源：http://baike.tarul.cn/Article/details/gkskfgohk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.tarul.cn/Article/details/glkbuyctn.sHtML

[U97] JS：并发请求
来源：http://read.share.vehdjk.com/Article/details/gdnolqynf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gzhgpxjgc.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.tarul.cn/Article/details/gffixfyzo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.epnwcf.com/Article/details/gdzaexydj.sHtML

[U99] JS：事件监听
来源：http://read.share.epnwcf.com/Article/details/gjpatrfzv.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.epnwcf.com/Article/details/ggulkynms.sHtML

[U100] JS：DOM 查询
来源：http://3g.sjlbkw.cn/Article/details/gknwxzmgi.sHtML

document.querySelector(".item")
来源：http://www.m.share.tarul.cn/Article/details/gvugorodj.sHtML

[U101] JS：classList 操作
来源：http://www.share.tarul.cn/Article/details/ggbfhwrml.sHtML

el.classList.toggle("active")
来源：http://read.share.fktsv.cn/Article/details/gofwbavkc.sHtML

[U102] JS：本地存储
来源：http://baike.bbcook.cn/Article/details/ggbpwzzwe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.sjlbkw.cn/Article/details/gcoeoetbg.sHtML

[U103] JS：定时器
来源：http://read.share.bbcook.cn/Article/details/gtmthdegf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.vehdjk.com/Article/details/goaldbkbg.sHtML

[U104] JS：防抖
来源：http://wap.tarul.cn/Article/details/gciqarumt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/gdnaeemvx.sHtML

[U105] JS：节流
来源：http://www.share.epnwcf.com/Article/details/gejwsfxhh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fktsv.cn/Article/details/ggigdhure.sHtML

[U106] JS：日期格式化
来源：http://baike.yfazqb.com/Article/details/grtokbdbf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.tarul.cn/Article/details/gzaqfolbw.sHtML

[U107] JS：数字千分位
来源：http://www.share.tarul.cn/Article/details/gcmortlfc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.yfazqb.com/Article/details/gbuumhxxk.sHtML

[U108] JS：随机整数
来源：http://www.blog.vehdjk.com/Article/details/gijyljakh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.vehdjk.com/Article/details/gytkgkzcb.sHtML

[U109] JS：数组分组
来源：http://baike.vehdjk.com/Article/details/ghqvcynca.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.epnwcf.com/Article/details/glyjjqtqn.sHtML

[U110] JS：数组分块
来源：http://www.share.vehdjk.com/Article/details/ghoezmpjs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.sjlbkw.cn/Article/details/gpdacyftj.sHtML

[U111] JS：对象转 Map
来源：http://3g.yfazqb.com/Article/details/gxadnvdmq.sHtML

new Map(Object.entries(obj))
来源：http://wap.bbcook.cn/Article/details/gpkyndaei.sHtML

[U112] JS：字符串补位
来源：http://blog.bbcook.cn/Article/details/gspmyienp.sHtML

"7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/gxbnxvdxl.sHtML

[U113] JS：正则替换全部
来源：http://3g.fktsv.cn/Article/details/gcsxkclul.sHtML

s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gsvyezkwz.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.yfazqb.com/Article/details/gsnsucgnw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.yfazqb.com/Article/details/glscfaojo.sHtML

[U115] JS：生成 UUID
来源：http://wap.fktsv.cn/Article/details/gpoylajpe.sHtML

crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/grokrlfnu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.epnwcf.com/Article/details/gmdbtwbxh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.tarul.cn/Article/details/ggrbksdnf.sHtML

[U117] JS：单元测试
来源：http://www.blog.bbcook.cn/Article/details/giouprkiy.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.tarul.cn/Article/details/glxrnoqyl.sHtML

[U118] JS：开发服务器
来源：http://www.blog.yfazqb.com/Article/details/gozgtiscq.sHtML

npm i -D vite;  npx vite
来源：http://blog.fktsv.cn/Article/details/gygmjnkjo.sHtML

[U119] JS：生产构建
来源：http://baike.tarul.cn/Article/details/gljsxcksc.sHtML

npx vite build
来源：http://read.share.sjlbkw.cn/Article/details/gihcnejqv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.bbcook.cn/Article/details/gutpddwle.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.vehdjk.com/Article/details/gzeegqfao.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gupfhcbvg.sHtML

统计汇总
来源：http://mobile.sjlbkw.cn/Article/details/gjwhoqppq.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gyxnygjzt.sHtML

按语言统计（条）：
来源：http://mobile.yfazqb.com/Article/details/gnxtruwtk.sHtML

Python ......... 252
来源：http://www.m.share.vehdjk.com/Article/details/gscuzxevb.sHtML

PHP ............ 252
来源：http://mobile.vehdjk.com/Article/details/gypwkchmx.sHtML

JavaScript ..... 252
来源：http://www.blog.tarul.cn/Article/details/gvyfcmckp.sHtML

TypeScript ..... 212
来源：http://wap.vehdjk.com/Article/details/gjjywioyp.sHtML

Java ........... 212
来源：http://blog.yfazqb.com/Article/details/ghgzxfexf.sHtML

Go ............. 212
来源：http://www.blog.bbcook.cn/Article/details/gjvtqbyhw.sHtML

Ruby ........... 212
来源：http://m.share.yfazqb.com/Article/details/gfzcdynkh.sHtML

C# ............. 212
来源：http://www.m.share.tarul.cn/Article/details/grgpligfo.sHtML

C .............. 30
来源：http://www.share.fktsv.cn/Article/details/gkpmvwcpp.sHtML

C++ ............ 30
来源：http://www.m.share.vehdjk.com/Article/details/gyndcifdu.sHtML

SQL ............ 90
来源：http://www.share.tarul.cn/Article/details/gutjosloy.sHtML

Bash ........... 80
来源：http://www.m.share.sjlbkw.cn/Article/details/giisawzre.sHtML

Kotlin ......... 15
来源：http://3g.sjlbkw.cn/Article/details/gwplsracp.sHtML

Swift .......... 15
来源：http://wap.epnwcf.com/Article/details/gmqefzuek.sHtML

Lua ............ 10
来源：http://3g.sjlbkw.cn/Article/details/gppwvuwry.sHtML

Perl ........... 10
来源：http://baike.epnwcf.com/Article/details/gczjfimlo.sHtML

Scala .......... 10
来源：http://read.share.bbcook.cn/Article/details/ghpqegzdn.sHtML

------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gjmomgyrn.sHtML

合计 ........... 2106 条
来源：http://3g.epnwcf.com/Article/details/gvmwbgefv.sHtML

按章节统计：
来源：http://blog.bbcook.cn/Article/details/gndlqgmkd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fktsv.cn/Article/details/gehxsffag.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.vehdjk.com/Article/details/gxtnrejwq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.sjlbkw.cn/Article/details/gdkfjdbqm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fktsv.cn/Article/details/gllujaxyh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.bbcook.cn/Article/details/gauhhcssy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.yfazqb.com/Article/details/grdsmpcuq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.vehdjk.com/Article/details/gquhrqwmh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fktsv.cn/Article/details/gguyqutea.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/grdftfqpo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.bbcook.cn/Article/details/gionnswoj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/gyqhxqcci.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/ghvqvlvye.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/groklkhiv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.sjlbkw.cn/Article/details/gkccvrvua.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.epnwcf.com/Article/details/gkgdfdnin.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gpjsalqlz.sHtML

Q SQL 专题                              90
来源：http://mobile.fktsv.cn/Article/details/gsuohvlic.sHtML

R Bash 专题                             80
来源：http://blog.epnwcf.com/Article/details/gfyokaasb.sHtML

S C / C++ 专题                          60
来源：http://blog.bbcook.cn/Article/details/gkielxurg.sHtML

T 其他语言补充                          60
来源：http://read.share.tarul.cn/Article/details/gazwaosai.sHtML

U 高频实用片段                         120
来源：http://www.share.vehdjk.com/Article/details/gwoyfrpxn.sHtML

------------------------------------
来源：http://wap.bbcook.cn/Article/details/gysddfowp.sHtML

合计                                  2106 条
来源：http://www.blog.yfazqb.com/Article/details/glcspjzla.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gkhfpauht.sHtML

使用提醒
来源：http://www.m.share.yfazqb.com/Article/details/ggraczspf.sHtML

--------------------------------------------------------------------------------
来源：http://3g.epnwcf.com/Article/details/gnqgqhkru.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.yfazqb.com/Article/details/gqlafmskx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.bbcook.cn/Article/details/gjrftfovu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.bbcook.cn/Article/details/gqehvilpu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.tarul.cn/Article/details/glcykxwcw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.epnwcf.com/Article/details/gtkbsiepc.sHtML

—— 文件结束 ——
来源：http://wap.fktsv.cn/Article/details/ggxavvddx.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gppsruzlt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.bbcook.cn/Article/details/gacicuiyg.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.vehdjk.com/Article/details/gjdliyxsh.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gcfydzqzz.sHtML

【收录内容】
来源：http://blog.fktsv.cn/Article/details/gcjrexhua.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.yfazqb.com/Article/details/gaxkmbjks.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.tarul.cn/Article/details/gwqznchhm.sHtML

SQL · Bash · C · C++
来源：http://blog.vehdjk.com/Article/details/gewscxexl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.epnwcf.com/Article/details/gieifwqdi.sHtML

【使用说明】
来源：http://www.blog.bbcook.cn/Article/details/gbvmohwjc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.bbcook.cn/Article/details/giukolqyq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.yfazqb.com/Article/details/gcummnrhe.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.epnwcf.com/Article/details/gkpsvibls.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.yfazqb.com/Article/details/gfdvxmbmp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.bbcook.cn/Article/details/gsjptbjyj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.epnwcf.com/Article/details/gayzqdxmb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.bbcook.cn/Article/details/gloqateup.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.yfazqb.com/Article/details/gzpnujwqc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.yfazqb.com/Article/details/glgzlpytj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.bbcook.cn/Article/details/ganwfxivs.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fktsv.cn/Article/details/gjdfsnhkp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.vehdjk.com/Article/details/gcbweimyw.sHtML

【文件统计】
来源：http://baike.bbcook.cn/Article/details/gsoeatiae.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.tarul.cn/Article/details/gquxvythl.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/grqgaanmc.sHtML

目  录
来源：http://www.blog.bbcook.cn/Article/details/gtdzhhrne.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/grpxoonis.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gtkabcoqu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.bbcook.cn/Article/details/gromfpyss.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fktsv.cn/Article/details/gwtkvydog.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.bbcook.cn/Article/details/gsakxmddd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fktsv.cn/Article/details/gwljpdtyu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.tarul.cn/Article/details/gvqdihgvf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.vehdjk.com/Article/details/ghwvieehv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtextcbo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.sjlbkw.cn/Article/details/gaikrpicb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.sjlbkw.cn/Article/details/gxizkwlxy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gmflymybo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/gjyhknocp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/gtyfsphjh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fktsv.cn/Article/details/gvrvcygte.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.yfazqb.com/Article/details/grslcthif.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.tarul.cn/Article/details/ggeecvipj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.bbcook.cn/Article/details/gilaghjnh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.bbcook.cn/Article/details/ginyqpfiz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.yfazqb.com/Article/details/gsugfqxpw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.tarul.cn/Article/details/gflsvgbve.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.tarul.cn/Article/details/gwjtffmpj.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gavtaegka.sHtML

A. 基础语法与类型
来源：http://read.share.fktsv.cn/Article/details/gbblrpaix.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbacurwpd.sHtML

[A01] Hello World
来源：http://blog.vehdjk.com/Article/details/gdcldwzqc.sHtML

Py:   print("Hello, World!")
来源：http://blog.yfazqb.com/Article/details/ggnscyhoi.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.epnwcf.com/Article/details/gcgebpvtl.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fktsv.cn/Article/details/gdolgkuxj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fktsv.cn/Article/details/gynkvajqw.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.bbcook.cn/Article/details/gzpwbhuvc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.yfazqb.com/Article/details/gwvfoexnb.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fktsv.cn/Article/details/gzsocjlla.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.vehdjk.com/Article/details/gkepstzam.sHtML

[A02] 变量声明与赋值
来源：http://mobile.sjlbkw.cn/Article/details/gvaomeueg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.vehdjk.com/Article/details/grgzcsqiu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.yfazqb.com/Article/details/gbqqbsssf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.bbcook.cn/Article/details/gpoooxqvt.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.bbcook.cn/Article/details/gxezedkvb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.vehdjk.com/Article/details/glgdqgqst.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.bbcook.cn/Article/details/gptecgmag.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.epnwcf.com/Article/details/gygeipowu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/gvtpapgbk.sHtML

[A03] 常量定义
来源：http://baike.epnwcf.com/Article/details/gwgusjzye.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.vehdjk.com/Article/details/gbxcqzzcp.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gsbmvhqck.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fktsv.cn/Article/details/gcyelssje.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gtollabkl.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.yfazqb.com/Article/details/gglmosnat.sHtML

Go:   const PI = 3.14159
来源：http://read.share.epnwcf.com/Article/details/gttmudnct.sHtML

Ruby: PI = 3.14159
来源：http://wap.bbcook.cn/Article/details/gaylibnmz.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/ghptntljb.sHtML

[A04] 判断变量类型
来源：http://www.share.epnwcf.com/Article/details/gbsmfkumz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.tarul.cn/Article/details/gcbkpijem.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.tarul.cn/Article/details/gyuxhwzpn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.vehdjk.com/Article/details/gfksfqqmr.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.tarul.cn/Article/details/grkpfdbiy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.epnwcf.com/Article/details/gmasxxblv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.epnwcf.com/Article/details/guzsfrkvn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.tarul.cn/Article/details/guldupcpn.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.vehdjk.com/Article/details/givbksnin.sHtML

[A05] 整数除法与取模
来源：http://mobile.tarul.cn/Article/details/gyotrtatl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.sjlbkw.cn/Article/details/ghnoydvsg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.yfazqb.com/Article/details/ghlyoqvwn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.vehdjk.com/Article/details/gsggquauk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gpizghvcj.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gkxlfujba.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gyliorbhf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gnzdjboly.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gvqgszbtr.sHtML

[A06] 字符串转数字
来源：http://mobile.epnwcf.com/Article/details/gqbgjbuwr.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.tarul.cn/Article/details/gpsvsqinz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.bbcook.cn/Article/details/gadmhckbt.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.vehdjk.com/Article/details/gpsntpqif.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.sjlbkw.cn/Article/details/giyiwigby.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.sjlbkw.cn/Article/details/glgynbptf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.epnwcf.com/Article/details/gglrtcjko.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.vehdjk.com/Article/details/gxrxyowrt.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.yfazqb.com/Article/details/gleitiygw.sHtML

[A07] 数字转字符串
来源：http://wap.vehdjk.com/Article/details/ggtkdpjha.sHtML

Py:   str(42)
来源：http://www.share.fktsv.cn/Article/details/gsgtpnloq.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fktsv.cn/Article/details/gcoyvjoav.sHtML

JS:   String(42); (42).toString()
来源：http://blog.bbcook.cn/Article/details/grunvmqid.sHtML

TS:   String(42)
来源：http://m.share.yfazqb.com/Article/details/ghfvbpujb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.yfazqb.com/Article/details/gktipfsve.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.sjlbkw.cn/Article/details/gpmheutsd.sHtML

Ruby: 42.to_s
来源：http://www.share.tarul.cn/Article/details/gpycuuzje.sHtML

C#:   42.ToString()
来源：http://read.share.fktsv.cn/Article/details/gcpubtdmq.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.epnwcf.com/Article/details/gqognbgim.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.yfazqb.com/Article/details/giwabggpg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.vehdjk.com/Article/details/gbrvdebda.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.sjlbkw.cn/Article/details/glgxuotky.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.sjlbkw.cn/Article/details/guzohhxwe.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.bbcook.cn/Article/details/gcfmwrsya.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.epnwcf.com/Article/details/gdhixcrou.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fktsv.cn/Article/details/gulnyiako.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/goazdnqro.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.sjlbkw.cn/Article/details/goqqtpnuo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gkfwmwjwx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gecjndjwf.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.tarul.cn/Article/details/ghbhhmxua.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gnolquoik.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/giblobvmm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.fktsv.cn/Article/details/ganwydzhk.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.epnwcf.com/Article/details/gfhagxmvk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.bbcook.cn/Article/details/ganceuhpg.sHtML

[A10] 生成随机数
来源：http://mobile.tarul.cn/Article/details/genzmrgfx.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.bbcook.cn/Article/details/gvovalzqg.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.vehdjk.com/Article/details/gokpvnals.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.sjlbkw.cn/Article/details/gnvbiqqhp.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.yfazqb.com/Article/details/gxispilte.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.tarul.cn/Article/details/gndqehfkq.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.epnwcf.com/Article/details/ggkfarntk.sHtML

Ruby: rand(1..100)
来源：http://wap.vehdjk.com/Article/details/gnvwejrah.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.vehdjk.com/Article/details/gvrgsgukt.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.fktsv.cn/Article/details/gylnvvmsq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.sjlbkw.cn/Article/details/ghukpjumh.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.yfazqb.com/Article/details/gpvglijcy.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/gtmrdsnsa.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.bbcook.cn/Article/details/gxugrshpi.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.fktsv.cn/Article/details/gmrwmucva.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.vehdjk.com/Article/details/gmlaebkmq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.yfazqb.com/Article/details/gfuiaesry.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fktsv.cn/Article/details/gnksjessw.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.tarul.cn/Article/details/gxcydjodg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.yfazqb.com/Article/details/gpimklxbp.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fktsv.cn/Article/details/garbgovcp.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fktsv.cn/Article/details/gkxqytxru.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.sjlbkw.cn/Article/details/gmleekwxb.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.yfazqb.com/Article/details/gqhjhflqj.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.sjlbkw.cn/Article/details/gymirbgvm.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.tarul.cn/Article/details/gmasvavml.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.fktsv.cn/Article/details/gqjblfljs.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.epnwcf.com/Article/details/gexxqorkh.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/grpqzeuwe.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/gbmrhkder.sHtML

JS:   "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gqttwkumd.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.epnwcf.com/Article/details/geiggswqn.sHtML

Java: "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/gvqrqgflr.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/guenkbyhr.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/gjbgnmtst.sHtML

C#:   "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gqvechvzu.sHtML

[A14] 注释写法
来源：http://www.share.epnwcf.com/Article/details/ggdthwzhl.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.sjlbkw.cn/Article/details/gjiwynvre.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.vehdjk.com/Article/details/gxjflzxhb.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.fktsv.cn/Article/details/gazjshggw.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.yfazqb.com/Article/details/grvqbarvr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.fktsv.cn/Article/details/gbnzgwynl.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.bbcook.cn/Article/details/gjqdwbbpa.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.bbcook.cn/Article/details/gmuchibls.sHtML


<!-- 参考信息 -->