代发 wailian999

[U85] JS：可选链
来源：http://www.m.share.tarul.cn/Article/details/goagarymn.sHtML

a?.b?.c
来源：http://www.blog.sjlbkw.cn/Article/details/grkfbwubl.sHtML

[U86] JS：空值合并
来源：http://blog.fktsv.cn/Article/details/gorvlvxdg.sHtML

a ?? b
来源：http://www.share.vehdjk.com/Article/details/grmalzpmn.sHtML

[U87] JS：解构默认值
来源：http://wap.fktsv.cn/Article/details/gxrdkcklm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.bbcook.cn/Article/details/gmruxzqcj.sHtML

[U88] JS：对象展开合并
来源：http://3g.sjlbkw.cn/Article/details/gdijmtkfk.sHtML

{ ...a, ...b }
来源：http://m.share.vehdjk.com/Article/details/gngunkszb.sHtML

[U89] JS：数组去重
来源：http://www.m.share.bbcook.cn/Article/details/gdijtfilv.sHtML

[...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/ggvrdigkf.sHtML

[U90] JS：数字数组排序
来源：http://www.share.sjlbkw.cn/Article/details/gdipqkqfq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gtuomktxb.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fktsv.cn/Article/details/gnlxsvkge.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.tarul.cn/Article/details/gomnfzbdl.sHtML

[U92] JS：深拷贝
来源：http://www.share.tarul.cn/Article/details/gzfohummh.sHtML

structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gaerngolw.sHtML

[U93] JS：模板字符串
来源：http://wap.vehdjk.com/Article/details/gykkbgbyy.sHtML

`共 ${n} 条`
来源：http://www.share.epnwcf.com/Article/details/gnbsyjvae.sHtML

[U94] JS：箭头函数
来源：http://mobile.sjlbkw.cn/Article/details/gsaqnamjo.sHtML

const double = x => x * 2;
来源：http://mobile.bbcook.cn/Article/details/gpkgpfjug.sHtML

[U95] JS：Promise 包装
来源：http://mobile.yfazqb.com/Article/details/gfafajich.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.tarul.cn/Article/details/gvyhfuomg.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.yfazqb.com/Article/details/gnkjspaxs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gpuutprcp.sHtML

[U97] JS：并发请求
来源：http://mobile.fktsv.cn/Article/details/gtjbqkyii.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/gjvzhqtit.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.epnwcf.com/Article/details/gojvbgzdn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.bbcook.cn/Article/details/gsxzukzwh.sHtML

[U99] JS：事件监听
来源：http://www.blog.fktsv.cn/Article/details/gpkuxlzgn.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fktsv.cn/Article/details/ggikyvbcb.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fktsv.cn/Article/details/grnlhrppd.sHtML

document.querySelector(".item")
来源：http://wap.tarul.cn/Article/details/gxfadwqcr.sHtML

[U101] JS：classList 操作
来源：http://wap.fktsv.cn/Article/details/gvrwjkjqc.sHtML

el.classList.toggle("active")
来源：http://baike.tarul.cn/Article/details/gssyxwiyp.sHtML

[U102] JS：本地存储
来源：http://www.share.fktsv.cn/Article/details/gmvnordgb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.bbcook.cn/Article/details/gnxrjifnr.sHtML

[U103] JS：定时器
来源：http://blog.fktsv.cn/Article/details/ggovkreyo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.tarul.cn/Article/details/gbdqyhhip.sHtML

[U104] JS：防抖
来源：http://blog.epnwcf.com/Article/details/gdgripnyv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/gobtujyvd.sHtML

[U105] JS：节流
来源：http://m.share.fktsv.cn/Article/details/gizhyifdm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.sjlbkw.cn/Article/details/gfawzazso.sHtML

[U106] JS：日期格式化
来源：http://mobile.fktsv.cn/Article/details/gfkbshvhd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.bbcook.cn/Article/details/gfvblndie.sHtML

[U107] JS：数字千分位
来源：http://wap.sjlbkw.cn/Article/details/gcmelkwsb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.sjlbkw.cn/Article/details/gdawynoje.sHtML

[U108] JS：随机整数
来源：http://www.blog.vehdjk.com/Article/details/gvzwnpujp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.epnwcf.com/Article/details/goycqpzlo.sHtML

[U109] JS：数组分组
来源：http://www.share.yfazqb.com/Article/details/gvqcdtyyv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.bbcook.cn/Article/details/ggwnhwqbw.sHtML

[U110] JS：数组分块
来源：http://www.m.share.yfazqb.com/Article/details/glnghojbt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.epnwcf.com/Article/details/gpvusdahb.sHtML

[U111] JS：对象转 Map
来源：http://baike.sjlbkw.cn/Article/details/gsiynjbll.sHtML

new Map(Object.entries(obj))
来源：http://read.share.bbcook.cn/Article/details/gvawskkos.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fktsv.cn/Article/details/gqbmxifrc.sHtML

"7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gfaknawqg.sHtML

[U113] JS：正则替换全部
来源：http://baike.tarul.cn/Article/details/gvxukweqi.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gaoecdgwg.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.vehdjk.com/Article/details/gmgfwuoez.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.bbcook.cn/Article/details/gwvmxshhq.sHtML

[U115] JS：生成 UUID
来源：http://read.share.tarul.cn/Article/details/gihmeagor.sHtML

crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/ghudgmrqb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fktsv.cn/Article/details/glcewmhlf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fktsv.cn/Article/details/gzwgjczdo.sHtML

[U117] JS：单元测试
来源：http://wap.bbcook.cn/Article/details/gdkxavfvx.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fktsv.cn/Article/details/givwmkwbd.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fktsv.cn/Article/details/gmpdeqger.sHtML

npm i -D vite;  npx vite
来源：http://www.share.epnwcf.com/Article/details/gkteccjnb.sHtML

[U119] JS：生产构建
来源：http://www.blog.tarul.cn/Article/details/gdtrkcyjw.sHtML

npx vite build
来源：http://read.share.sjlbkw.cn/Article/details/gtcctvxlk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fktsv.cn/Article/details/gszesrlwr.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.epnwcf.com/Article/details/gmwhuvkmr.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gjxhzjnbx.sHtML

统计汇总
来源：http://m.share.bbcook.cn/Article/details/gcraepwjx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/givqavxtx.sHtML

按语言统计（条）：
来源：http://3g.vehdjk.com/Article/details/gtzeulzqo.sHtML

Python ......... 252
来源：http://mobile.bbcook.cn/Article/details/gnzqgrvcs.sHtML

PHP ............ 252
来源：http://blog.yfazqb.com/Article/details/gvddhimon.sHtML

JavaScript ..... 252
来源：http://baike.sjlbkw.cn/Article/details/gekzczngo.sHtML

TypeScript ..... 212
来源：http://www.m.share.bbcook.cn/Article/details/gbgnwhmzg.sHtML

Java ........... 212
来源：http://baike.bbcook.cn/Article/details/gkcomowqu.sHtML

Go ............. 212
来源：http://www.m.share.tarul.cn/Article/details/gbixfmyeg.sHtML

Ruby ........... 212
来源：http://baike.tarul.cn/Article/details/ghivhcobk.sHtML

C# ............. 212
来源：http://baike.epnwcf.com/Article/details/gcaculzhf.sHtML

C .............. 30
来源：http://3g.tarul.cn/Article/details/gpqcniagc.sHtML

C++ ............ 30
来源：http://www.blog.sjlbkw.cn/Article/details/gjvxjwpmw.sHtML

SQL ............ 90
来源：http://www.share.vehdjk.com/Article/details/gbsuxbcme.sHtML

Bash ........... 80
来源：http://3g.yfazqb.com/Article/details/gctovnvmh.sHtML

Kotlin ......... 15
来源：http://baike.sjlbkw.cn/Article/details/ghkgseije.sHtML

Swift .......... 15
来源：http://wap.tarul.cn/Article/details/gfjmiqvou.sHtML

Lua ............ 10
来源：http://read.share.epnwcf.com/Article/details/gbyqbehgc.sHtML

Perl ........... 10
来源：http://baike.fktsv.cn/Article/details/ghojpzmbw.sHtML

Scala .......... 10
来源：http://m.share.bbcook.cn/Article/details/goiwgmlwz.sHtML

------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gaulksihh.sHtML

合计 ........... 2106 条
来源：http://blog.epnwcf.com/Article/details/glslhjxtj.sHtML

按章节统计：
来源：http://3g.vehdjk.com/Article/details/gicmcldre.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.yfazqb.com/Article/details/gbclhmlcd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.sjlbkw.cn/Article/details/gfrypzmkm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.vehdjk.com/Article/details/gnsvkvtlp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.yfazqb.com/Article/details/gqkyjvwfn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.bbcook.cn/Article/details/gtnxyzrkn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.bbcook.cn/Article/details/gzqpnveit.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fktsv.cn/Article/details/glopwipyr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fktsv.cn/Article/details/gxlxncdml.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gpirvwsjg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.tarul.cn/Article/details/gchurrlqu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/gzuzjtokd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/gikykoene.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/gparrmiie.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.tarul.cn/Article/details/goeydeedd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.yfazqb.com/Article/details/gfsypifkv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gmnkzlfhh.sHtML

Q SQL 专题                              90
来源：http://wap.epnwcf.com/Article/details/gngdsxoof.sHtML

R Bash 专题                             80
来源：http://www.share.yfazqb.com/Article/details/gkylcgmjm.sHtML

S C / C++ 专题                          60
来源：http://www.share.sjlbkw.cn/Article/details/gkatmzrok.sHtML

T 其他语言补充                          60
来源：http://read.share.tarul.cn/Article/details/gfcuugwij.sHtML

U 高频实用片段                         120
来源：http://blog.bbcook.cn/Article/details/gjterfjyf.sHtML

------------------------------------
来源：http://mobile.fktsv.cn/Article/details/geukamelj.sHtML

合计                                  2106 条
来源：http://www.m.share.epnwcf.com/Article/details/gjrnbqpsd.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fktsv.cn/Article/details/gvheoyyld.sHtML

使用提醒
来源：http://www.share.yfazqb.com/Article/details/gisyzsiin.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/gfqptvwgv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.epnwcf.com/Article/details/gkkqupcdw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fktsv.cn/Article/details/gjzfntsid.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fktsv.cn/Article/details/gtdjleidk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fktsv.cn/Article/details/gldnuboeq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.tarul.cn/Article/details/grkmlirhd.sHtML

—— 文件结束 ——
来源：http://www.blog.bbcook.cn/Article/details/gxykjbjgz.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gjjoariub.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.tarul.cn/Article/details/gheenvjtj.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.yfazqb.com/Article/details/gntfrqvdm.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/glxwdgpzu.sHtML

【收录内容】
来源：http://www.blog.fktsv.cn/Article/details/gaurpviwo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.epnwcf.com/Article/details/gwjljojgz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.yfazqb.com/Article/details/giufowiut.sHtML

SQL · Bash · C · C++
来源：http://wap.epnwcf.com/Article/details/gmhapkeco.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.epnwcf.com/Article/details/gpcroesih.sHtML

【使用说明】
来源：http://www.blog.vehdjk.com/Article/details/glpyyhgko.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.epnwcf.com/Article/details/ghmnakele.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.epnwcf.com/Article/details/gafiedgrt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.epnwcf.com/Article/details/gqhspvrju.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.yfazqb.com/Article/details/gkaxnxobh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fktsv.cn/Article/details/gcrmqduwo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.yfazqb.com/Article/details/gongcmuca.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.yfazqb.com/Article/details/gcycxkwjw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.vehdjk.com/Article/details/gybksenoa.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.epnwcf.com/Article/details/ghtlnixni.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.yfazqb.com/Article/details/gqqqiapod.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fktsv.cn/Article/details/gvtqrcwow.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.yfazqb.com/Article/details/gvyhldksp.sHtML

【文件统计】
来源：http://www.blog.fktsv.cn/Article/details/gjfpbouah.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.tarul.cn/Article/details/guczontng.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/gmnzsxdho.sHtML

目  录
来源：http://blog.fktsv.cn/Article/details/gquscvzrj.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gaocxjiyt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.vehdjk.com/Article/details/gjveanhlj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.vehdjk.com/Article/details/ggjbfvlll.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.bbcook.cn/Article/details/gbikepixg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.tarul.cn/Article/details/gfsgnhpqu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fktsv.cn/Article/details/gngsidgns.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.bbcook.cn/Article/details/girpegthm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.yfazqb.com/Article/details/grugajlmv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.sjlbkw.cn/Article/details/gqpkckokg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.vehdjk.com/Article/details/gmoeitefc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fktsv.cn/Article/details/gauwcfnzx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/gltjbzqss.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gfjqomkpz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gerefnxig.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.yfazqb.com/Article/details/gmixjgwno.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.epnwcf.com/Article/details/ghynjxdqv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/gprnaikgd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fktsv.cn/Article/details/gqwhbormc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.epnwcf.com/Article/details/ghewwvopu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.yfazqb.com/Article/details/gxwvorubm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.bbcook.cn/Article/details/gvmwaiwld.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.bbcook.cn/Article/details/gygzznwpp.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gifyzndkx.sHtML

A. 基础语法与类型
来源：http://m.share.vehdjk.com/Article/details/gplnnrhwy.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gevqgcpue.sHtML

[A01] Hello World
来源：http://www.blog.fktsv.cn/Article/details/gekxeboox.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fktsv.cn/Article/details/gfglbubkd.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.tarul.cn/Article/details/gpwowkeon.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.epnwcf.com/Article/details/guqjqdkht.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.tarul.cn/Article/details/gngvwqdut.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.vehdjk.com/Article/details/gyztekzqj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fktsv.cn/Article/details/gpvpifbny.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.sjlbkw.cn/Article/details/gppykccca.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fktsv.cn/Article/details/geylynwpf.sHtML

[A02] 变量声明与赋值
来源：http://3g.fktsv.cn/Article/details/gvggmfakv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkqloqpb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.vehdjk.com/Article/details/gvdaakmij.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.bbcook.cn/Article/details/glajwjrtn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.epnwcf.com/Article/details/gtroulvza.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.bbcook.cn/Article/details/gdyfcpxth.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.bbcook.cn/Article/details/gqnsiqkup.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.tarul.cn/Article/details/ggopfsfna.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.tarul.cn/Article/details/gfthnljnj.sHtML

[A03] 常量定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvnttsup.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.sjlbkw.cn/Article/details/gozrhztun.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gghcsdpcu.sHtML

JS:   const PI = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gloykaqgt.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/goocpcill.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gpeowmxjl.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.epnwcf.com/Article/details/gmzmijkyw.sHtML

Ruby: PI = 3.14159
来源：http://3g.tarul.cn/Article/details/ghuuizqpj.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gyweksmnd.sHtML

[A04] 判断变量类型
来源：http://read.share.vehdjk.com/Article/details/gcbyyryhu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fktsv.cn/Article/details/gwasbkwmq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdaxgtfn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.yfazqb.com/Article/details/gnjvtikdj.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkyqafwy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.tarul.cn/Article/details/glipryryz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.vehdjk.com/Article/details/gjsppaazo.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.vehdjk.com/Article/details/gpyoxxedr.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.bbcook.cn/Article/details/gzemxsgat.sHtML

[A05] 整数除法与取模
来源：http://3g.epnwcf.com/Article/details/gnxfnlmph.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.tarul.cn/Article/details/gubxjhsnj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.vehdjk.com/Article/details/goontfrwr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.epnwcf.com/Article/details/gvuubrobz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fktsv.cn/Article/details/gsiklabxg.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/gvgblpbvc.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.tarul.cn/Article/details/gkamknydj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.tarul.cn/Article/details/gnbkwyxgg.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fktsv.cn/Article/details/gzqhqofov.sHtML

[A06] 字符串转数字
来源：http://read.share.tarul.cn/Article/details/geuhkxdwb.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.epnwcf.com/Article/details/gyoczrkfr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.bbcook.cn/Article/details/gqejwjjii.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.vehdjk.com/Article/details/gkqrwzqyl.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.bbcook.cn/Article/details/guqcvtcjc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.bbcook.cn/Article/details/goolvwuik.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fktsv.cn/Article/details/gdrwbgojx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.epnwcf.com/Article/details/gnmwuppoz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fktsv.cn/Article/details/gvtrhurlw.sHtML

[A07] 数字转字符串
来源：http://read.share.yfazqb.com/Article/details/gddybwjnw.sHtML

Py:   str(42)
来源：http://3g.tarul.cn/Article/details/gyqgwezsy.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.vehdjk.com/Article/details/gtqauskfj.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.sjlbkw.cn/Article/details/gajrnnoeg.sHtML

TS:   String(42)
来源：http://wap.fktsv.cn/Article/details/gzgroowem.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.vehdjk.com/Article/details/gzeadnxbc.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.tarul.cn/Article/details/gpklykmpo.sHtML

Ruby: 42.to_s
来源：http://www.blog.fktsv.cn/Article/details/gcjdemqav.sHtML

C#:   42.ToString()
来源：http://3g.sjlbkw.cn/Article/details/gjyleunpk.sHtML

[A08] 取整与四舍五入
来源：http://wap.epnwcf.com/Article/details/gexpvselu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.epnwcf.com/Article/details/ghsqyecaz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.epnwcf.com/Article/details/gwfixbuzr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.fktsv.cn/Article/details/ggdxehpig.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.epnwcf.com/Article/details/gnnpozedn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.tarul.cn/Article/details/glbqxvmeh.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.vehdjk.com/Article/details/grwnmnylz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.yfazqb.com/Article/details/giurrkqwm.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.sjlbkw.cn/Article/details/gxpoexsmz.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.bbcook.cn/Article/details/gdhluxite.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.bbcook.cn/Article/details/ggnvghzus.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.epnwcf.com/Article/details/gbuqrtesh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gvpazkvyx.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.tarul.cn/Article/details/glocamdjb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gvyzudobm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.tarul.cn/Article/details/gggpzxydq.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.yfazqb.com/Article/details/gbgnifyfy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.vehdjk.com/Article/details/gbbwlnjtt.sHtML

[A10] 生成随机数
来源：http://wap.fktsv.cn/Article/details/gvfnaosal.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.yfazqb.com/Article/details/ggqpcetov.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fktsv.cn/Article/details/giluaktnj.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.tarul.cn/Article/details/geyowueiw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.sjlbkw.cn/Article/details/gvefwupfi.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.vehdjk.com/Article/details/gnnwitjsz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fktsv.cn/Article/details/gyayoumnx.sHtML

Ruby: rand(1..100)
来源：http://read.share.yfazqb.com/Article/details/glvzzqxfx.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.bbcook.cn/Article/details/gtsetgtln.sHtML

[A11] 条件表达式（三元）
来源：http://wap.fktsv.cn/Article/details/gmkigctxt.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.tarul.cn/Article/details/gkdcigbws.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.bbcook.cn/Article/details/ggwghvlcj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.fktsv.cn/Article/details/gqavxfryd.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.tarul.cn/Article/details/glajvdtjt.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.yfazqb.com/Article/details/gjmowkhla.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.tarul.cn/Article/details/gxndmbtdd.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.vehdjk.com/Article/details/gwuhinbrz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.vehdjk.com/Article/details/gvreutmsz.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.tarul.cn/Article/details/ghdzolymc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.fktsv.cn/Article/details/ghrdrfwvc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fktsv.cn/Article/details/gottkqhyf.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.vehdjk.com/Article/details/gufrwjbma.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.tarul.cn/Article/details/gptvmsqkb.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.fktsv.cn/Article/details/gcxfccxfi.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.tarul.cn/Article/details/gdncnykoz.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.sjlbkw.cn/Article/details/ghwtgnkdq.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.tarul.cn/Article/details/gwbidxvah.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.vehdjk.com/Article/details/gzzpwsrfj.sHtML

Py:   "第一行\n第二行"
来源：http://3g.fktsv.cn/Article/details/gldikcwlt.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/geexhihzh.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.epnwcf.com/Article/details/gesjxoqug.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/guhbvtsbi.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.sjlbkw.cn/Article/details/gsijwmqfn.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gpfiwynoj.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/grbgtcozo.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/glmjlktbu.sHtML

[A14] 注释写法
来源：http://blog.bbcook.cn/Article/details/gpihrujut.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.epnwcf.com/Article/details/guxvgkoqu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.fktsv.cn/Article/details/gmzrzlyrq.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.tarul.cn/Article/details/ggaqinbjb.sHtML


<!-- 参考信息 -->