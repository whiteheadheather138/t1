代发 wailian999

[U87] JS：解构默认值
来源：http://www.blog.vehdjk.com/Article/details/gghgcioqg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.sjlbkw.cn/Article/details/ghcdugava.sHtML

[U88] JS：对象展开合并
来源：http://m.share.yfazqb.com/Article/details/ghjjurmqh.sHtML

{ ...a, ...b }
来源：http://blog.bbcook.cn/Article/details/gvwzczgai.sHtML

[U89] JS：数组去重
来源：http://blog.yfazqb.com/Article/details/gqgvycyrb.sHtML

[...new Set(arr)]
来源：http://wap.fktsv.cn/Article/details/gngrpplrn.sHtML

[U90] JS：数字数组排序
来源：http://blog.yfazqb.com/Article/details/gnbeoixkl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/gollypfsr.sHtML

[U91] JS：对象键值遍历
来源：http://blog.sjlbkw.cn/Article/details/gkqfoytqr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.epnwcf.com/Article/details/ggwhcbzyx.sHtML

[U92] JS：深拷贝
来源：http://baike.vehdjk.com/Article/details/gmoniujmh.sHtML

structuredClone(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gogrjxsap.sHtML

[U93] JS：模板字符串
来源：http://wap.yfazqb.com/Article/details/ghnxhryzn.sHtML

`共 ${n} 条`
来源：http://baike.fktsv.cn/Article/details/gszfgoxsw.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.vehdjk.com/Article/details/gqsofdllk.sHtML

const double = x => x * 2;
来源：http://www.m.share.fktsv.cn/Article/details/ghuawgrhu.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.bbcook.cn/Article/details/grvltdvfr.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.vehdjk.com/Article/details/gpnoweqva.sHtML

[U96] JS：async/await 与异常
来源：http://wap.bbcook.cn/Article/details/gpaaqpfen.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/gyzciemxf.sHtML

[U97] JS：并发请求
来源：http://m.share.fktsv.cn/Article/details/gftuasjof.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gwcnlhfsl.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.tarul.cn/Article/details/grcujvtrj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.vehdjk.com/Article/details/gsjkmmkfl.sHtML

[U99] JS：事件监听
来源：http://wap.fktsv.cn/Article/details/gmztawczn.sHtML

el.addEventListener("click", e => {})
来源：http://wap.tarul.cn/Article/details/gomzczcan.sHtML

[U100] JS：DOM 查询
来源：http://wap.bbcook.cn/Article/details/gcfacbnkp.sHtML

document.querySelector(".item")
来源：http://blog.vehdjk.com/Article/details/gxexrgaav.sHtML

[U101] JS：classList 操作
来源：http://www.share.vehdjk.com/Article/details/gamhdjqwj.sHtML

el.classList.toggle("active")
来源：http://read.share.fktsv.cn/Article/details/gtpcaqhrl.sHtML

[U102] JS：本地存储
来源：http://www.share.bbcook.cn/Article/details/glgycfdij.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.bbcook.cn/Article/details/gkfbacciv.sHtML

[U103] JS：定时器
来源：http://read.share.vehdjk.com/Article/details/glfghvxcx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.vehdjk.com/Article/details/gqccexbbs.sHtML

[U104] JS：防抖
来源：http://m.share.fktsv.cn/Article/details/ggddqdnls.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/gktlifpoo.sHtML

[U105] JS：节流
来源：http://m.share.tarul.cn/Article/details/gdqhzgmoh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.bbcook.cn/Article/details/gvsamutra.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/gagxsuktv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.yfazqb.com/Article/details/gqpfsmmph.sHtML

[U107] JS：数字千分位
来源：http://baike.bbcook.cn/Article/details/goafpoevm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gvdyooqqo.sHtML

[U108] JS：随机整数
来源：http://mobile.tarul.cn/Article/details/groyfhoxp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fktsv.cn/Article/details/goupzubdz.sHtML

[U109] JS：数组分组
来源：http://3g.epnwcf.com/Article/details/gqcgmsdjd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.bbcook.cn/Article/details/gletijsds.sHtML

[U110] JS：数组分块
来源：http://read.share.vehdjk.com/Article/details/gdnktqhjc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.tarul.cn/Article/details/gpumazggy.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fktsv.cn/Article/details/ghuxofduk.sHtML

new Map(Object.entries(obj))
来源：http://wap.bbcook.cn/Article/details/gjfdavrnf.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.bbcook.cn/Article/details/glzbclfpj.sHtML

"7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/gzawapnwz.sHtML

[U113] JS：正则替换全部
来源：http://m.share.yfazqb.com/Article/details/grctmckss.sHtML

s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gfcotvgdx.sHtML

[U114] JS：JSON 深比较
来源：http://3g.bbcook.cn/Article/details/gjdglylfj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.bbcook.cn/Article/details/gidvlyzyj.sHtML

[U115] JS：生成 UUID
来源：http://3g.fktsv.cn/Article/details/gicgzedes.sHtML

crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/glqvlnqhv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fktsv.cn/Article/details/gmguyuirg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.epnwcf.com/Article/details/gnyxntpdc.sHtML

[U117] JS：单元测试
来源：http://mobile.vehdjk.com/Article/details/gydpxyzlj.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.vehdjk.com/Article/details/ghrhdwqbz.sHtML

[U118] JS：开发服务器
来源：http://www.blog.sjlbkw.cn/Article/details/gzxeipayu.sHtML

npm i -D vite;  npx vite
来源：http://3g.yfazqb.com/Article/details/gimnpdtfe.sHtML

[U119] JS：生产构建
来源：http://mobile.sjlbkw.cn/Article/details/gbfuphpps.sHtML

npx vite build
来源：http://3g.vehdjk.com/Article/details/ggrofabwx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.bbcook.cn/Article/details/gunsxnbky.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.yfazqb.com/Article/details/glpspihmh.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ghxfqnzat.sHtML

统计汇总
来源：http://www.m.share.yfazqb.com/Article/details/gvtwcvfpg.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gvvgzyoxn.sHtML

按语言统计（条）：
来源：http://m.share.sjlbkw.cn/Article/details/giekgslnv.sHtML

Python ......... 252
来源：http://3g.epnwcf.com/Article/details/gksatpqze.sHtML

PHP ............ 252
来源：http://mobile.tarul.cn/Article/details/gzhogizft.sHtML

JavaScript ..... 252
来源：http://www.blog.epnwcf.com/Article/details/gdptvmsbl.sHtML

TypeScript ..... 212
来源：http://m.share.bbcook.cn/Article/details/gzwnrhxes.sHtML

Java ........... 212
来源：http://3g.fktsv.cn/Article/details/gdqwuzkmr.sHtML

Go ............. 212
来源：http://www.m.share.fktsv.cn/Article/details/gowxwmrrr.sHtML

Ruby ........... 212
来源：http://www.blog.yfazqb.com/Article/details/gulnggfcu.sHtML

C# ............. 212
来源：http://3g.fktsv.cn/Article/details/gnogebpfm.sHtML

C .............. 30
来源：http://read.share.bbcook.cn/Article/details/gzpjvcwdn.sHtML

C++ ............ 30
来源：http://read.share.fktsv.cn/Article/details/gysjbafcu.sHtML

SQL ............ 90
来源：http://www.m.share.fktsv.cn/Article/details/gnhacgayi.sHtML

Bash ........... 80
来源：http://wap.epnwcf.com/Article/details/gecnbvxno.sHtML

Kotlin ......... 15
来源：http://www.share.vehdjk.com/Article/details/gnndpmule.sHtML

Swift .......... 15
来源：http://mobile.epnwcf.com/Article/details/gflzyaxqo.sHtML

Lua ............ 10
来源：http://m.share.tarul.cn/Article/details/gciyqjamy.sHtML

Perl ........... 10
来源：http://www.share.yfazqb.com/Article/details/grjibkjqk.sHtML

Scala .......... 10
来源：http://www.share.epnwcf.com/Article/details/gvojlqhoy.sHtML

------------------------------------
来源：http://wap.tarul.cn/Article/details/gizbqfvcn.sHtML

合计 ........... 2106 条
来源：http://read.share.fktsv.cn/Article/details/gpjhpsmrp.sHtML

按章节统计：
来源：http://read.share.yfazqb.com/Article/details/gnqycxmgw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.yfazqb.com/Article/details/gakeopzaz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.vehdjk.com/Article/details/gihfrepjk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.vehdjk.com/Article/details/gqqbeegpz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.epnwcf.com/Article/details/gntdpsghs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.vehdjk.com/Article/details/gamlemcwr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.vehdjk.com/Article/details/ghdmbapsx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.sjlbkw.cn/Article/details/gnzyzncna.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.tarul.cn/Article/details/ghggpcoqh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gbwqgspuq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.vehdjk.com/Article/details/gxwqaxvvd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gyfiqngvm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gehxsnhfy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/gosqxndck.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.sjlbkw.cn/Article/details/gmxbtjneq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fktsv.cn/Article/details/gfsgrffzg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gbibcpcva.sHtML

Q SQL 专题                              90
来源：http://wap.vehdjk.com/Article/details/gqqlqedae.sHtML

R Bash 专题                             80
来源：http://wap.tarul.cn/Article/details/gmtvhllsi.sHtML

S C / C++ 专题                          60
来源：http://3g.yfazqb.com/Article/details/gtqzupjfn.sHtML

T 其他语言补充                          60
来源：http://mobile.yfazqb.com/Article/details/gmsqavodf.sHtML

U 高频实用片段                         120
来源：http://m.share.tarul.cn/Article/details/gnbiqylfe.sHtML

------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gaczsydrs.sHtML

合计                                  2106 条
来源：http://3g.vehdjk.com/Article/details/gohflndrz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.epnwcf.com/Article/details/ghizihkek.sHtML

使用提醒
来源：http://blog.fktsv.cn/Article/details/ghfmyytvw.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gbwvamzqb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.sjlbkw.cn/Article/details/ganjgqsnf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.yfazqb.com/Article/details/gizowtwxg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.epnwcf.com/Article/details/gpjzadonc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.tarul.cn/Article/details/gscnjmlcs.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.tarul.cn/Article/details/gptndywgu.sHtML

—— 文件结束 ——
来源：http://www.share.sjlbkw.cn/Article/details/ghltjqlxe.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gdqnrelcv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fktsv.cn/Article/details/ggtfzwmyl.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.bbcook.cn/Article/details/gtdetmwkd.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gtkntyqvo.sHtML

【收录内容】
来源：http://3g.yfazqb.com/Article/details/gyzesdblb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.epnwcf.com/Article/details/gizlupvcq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.tarul.cn/Article/details/gkbsvwnpy.sHtML

SQL · Bash · C · C++
来源：http://wap.yfazqb.com/Article/details/glxqkrkuy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fktsv.cn/Article/details/gtnaeqfez.sHtML

【使用说明】
来源：http://3g.bbcook.cn/Article/details/guvvtcihw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.tarul.cn/Article/details/gvsqkdewz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.sjlbkw.cn/Article/details/ggsewrpkv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.yfazqb.com/Article/details/gvasusarp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.epnwcf.com/Article/details/gjscxrpww.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.epnwcf.com/Article/details/gmqqujzef.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.yfazqb.com/Article/details/gfbdgcxbu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.sjlbkw.cn/Article/details/gropsidmy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fktsv.cn/Article/details/gpryzkmdz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.tarul.cn/Article/details/ggpxtulun.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.bbcook.cn/Article/details/gohbvrkvt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.epnwcf.com/Article/details/gruizmhvc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.bbcook.cn/Article/details/gvdfplzfy.sHtML

【文件统计】
来源：http://m.share.vehdjk.com/Article/details/gkotazmst.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.tarul.cn/Article/details/gojfpaobs.sHtML

--------------------------------------------------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/gtluvmdkm.sHtML

目  录
来源：http://baike.tarul.cn/Article/details/gdxfbtlfg.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gngxktzru.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.sjlbkw.cn/Article/details/gmvztcyco.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.yfazqb.com/Article/details/gudhksgub.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fktsv.cn/Article/details/gonjwkqfh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.sjlbkw.cn/Article/details/gdebhabrn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.bbcook.cn/Article/details/giqjezewy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.sjlbkw.cn/Article/details/ghugmsuns.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.vehdjk.com/Article/details/gvxijjaml.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.vehdjk.com/Article/details/ganvlsrpa.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.epnwcf.com/Article/details/gkrnljcqt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.vehdjk.com/Article/details/gjclguuwx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.sjlbkw.cn/Article/details/gxiqxdnkh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.epnwcf.com/Article/details/gchaqnvxv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gihxxujjr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fktsv.cn/Article/details/govaehyob.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.vehdjk.com/Article/details/ghhrzylpo.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/glogacomu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fktsv.cn/Article/details/gisbgilog.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.bbcook.cn/Article/details/gliwqzbwg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fktsv.cn/Article/details/gtzylbshq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.sjlbkw.cn/Article/details/gzcjfscws.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.tarul.cn/Article/details/gnkagvjlz.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gvscjwndk.sHtML

A. 基础语法与类型
来源：http://www.m.share.fktsv.cn/Article/details/gugitrcop.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gfioytvrv.sHtML

[A01] Hello World
来源：http://baike.vehdjk.com/Article/details/gilxynlcd.sHtML

Py:   print("Hello, World!")
来源：http://blog.sjlbkw.cn/Article/details/gvrnvurgk.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.vehdjk.com/Article/details/gftbnqdtm.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.epnwcf.com/Article/details/gxbfwuhiw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.bbcook.cn/Article/details/gixsymizt.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.sjlbkw.cn/Article/details/gdgjugjql.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.bbcook.cn/Article/details/gfodncdtw.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.epnwcf.com/Article/details/gxrlwiscd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.vehdjk.com/Article/details/gxtdkmjok.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.vehdjk.com/Article/details/gqafkopdt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.tarul.cn/Article/details/gmjqgeblv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.yfazqb.com/Article/details/ggxjaitib.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.epnwcf.com/Article/details/guhbnfksz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.epnwcf.com/Article/details/gpbxkpdyn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gvrncsiwn.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.epnwcf.com/Article/details/gmplotkii.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.bbcook.cn/Article/details/gpskmpbjq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.sjlbkw.cn/Article/details/gfdorwybv.sHtML

[A03] 常量定义
来源：http://www.blog.vehdjk.com/Article/details/galfurkva.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.sjlbkw.cn/Article/details/gqplafwxv.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gjysesiro.sHtML

JS:   const PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/gecxttthb.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gjwmwtamq.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/garhmmqsr.sHtML

Go:   const PI = 3.14159
来源：http://mobile.bbcook.cn/Article/details/gyubibgtq.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fktsv.cn/Article/details/gbtqdlpef.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/glnfxmoip.sHtML

[A04] 判断变量类型
来源：http://www.m.share.vehdjk.com/Article/details/grniifetz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.vehdjk.com/Article/details/gpgyjfnbc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.epnwcf.com/Article/details/grznrkvvo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.sjlbkw.cn/Article/details/gdcnivzwl.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.yfazqb.com/Article/details/ggdgnbopl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.bbcook.cn/Article/details/gqoyetlcs.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fktsv.cn/Article/details/gtakiljga.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.vehdjk.com/Article/details/gvbjdpkig.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.epnwcf.com/Article/details/gmhyokcug.sHtML

[A05] 整数除法与取模
来源：http://www.blog.epnwcf.com/Article/details/grhvydcot.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.tarul.cn/Article/details/gtdmtaztp.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gcjsjqfxu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gbkjlifgw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/glfowklck.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.vehdjk.com/Article/details/gsdemhetc.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/gnqzthjbz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.sjlbkw.cn/Article/details/gushxeeop.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fktsv.cn/Article/details/gdxfoctjk.sHtML

[A06] 字符串转数字
来源：http://m.share.vehdjk.com/Article/details/gznahmpql.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.epnwcf.com/Article/details/gigbsbivg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.yfazqb.com/Article/details/gxkwytgfp.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.yfazqb.com/Article/details/gtknachlu.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fktsv.cn/Article/details/glfbqqsbi.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.epnwcf.com/Article/details/gmmjqmrtf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fktsv.cn/Article/details/gjmbuhglx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.tarul.cn/Article/details/gncfivqhp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.sjlbkw.cn/Article/details/greckzwmz.sHtML

[A07] 数字转字符串
来源：http://www.share.epnwcf.com/Article/details/gudjijzgw.sHtML

Py:   str(42)
来源：http://www.share.epnwcf.com/Article/details/guhvkptjm.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.epnwcf.com/Article/details/gznrtxquz.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.epnwcf.com/Article/details/gonkmlzqk.sHtML

TS:   String(42)
来源：http://m.share.fktsv.cn/Article/details/glpchwnbb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.yfazqb.com/Article/details/ghstdtzxy.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.tarul.cn/Article/details/gczfovpwz.sHtML

Ruby: 42.to_s
来源：http://read.share.sjlbkw.cn/Article/details/gjygzyxto.sHtML

C#:   42.ToString()
来源：http://blog.bbcook.cn/Article/details/gzcitpjcb.sHtML

[A08] 取整与四舍五入
来源：http://read.share.epnwcf.com/Article/details/gpucupqfi.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.vehdjk.com/Article/details/gzjoicgbk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.bbcook.cn/Article/details/gzfqrthlv.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.vehdjk.com/Article/details/gwqiknrsv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fktsv.cn/Article/details/gjqmykcfh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.yfazqb.com/Article/details/gplssxubj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.bbcook.cn/Article/details/gravkrgpl.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.tarul.cn/Article/details/ggepxoxbp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.bbcook.cn/Article/details/gckgsnylf.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.epnwcf.com/Article/details/gwncwalbx.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.tarul.cn/Article/details/glzdbsxyn.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gdsvhsqed.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.tarul.cn/Article/details/gkmetvamu.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gnicxxhtd.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gaphupqmw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.vehdjk.com/Article/details/gtljbkncm.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fktsv.cn/Article/details/gcolcpolg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gwkhfdznp.sHtML

[A10] 生成随机数
来源：http://www.blog.bbcook.cn/Article/details/geqhrmiqv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.sjlbkw.cn/Article/details/glxztsawy.sHtML

PHP:  random_int(1, 100);
来源：http://blog.epnwcf.com/Article/details/gqvsyehet.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fktsv.cn/Article/details/gorqokmwr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fktsv.cn/Article/details/gbjpqvrpw.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.epnwcf.com/Article/details/gpazppdro.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.yfazqb.com/Article/details/gohsccemo.sHtML

Ruby: rand(1..100)
来源：http://read.share.epnwcf.com/Article/details/gcsntxgbf.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.yfazqb.com/Article/details/gfyvfgeag.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.vehdjk.com/Article/details/gmimqtlji.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.tarul.cn/Article/details/gpebloiyt.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.yfazqb.com/Article/details/gramsoeva.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.sjlbkw.cn/Article/details/gevehemlv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.bbcook.cn/Article/details/gcbcwkhcy.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.epnwcf.com/Article/details/gnikcbyrw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.bbcook.cn/Article/details/gqgxrzoum.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.yfazqb.com/Article/details/gpsyufhlk.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.sjlbkw.cn/Article/details/gqzryepik.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.sjlbkw.cn/Article/details/gvjwcomqs.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.tarul.cn/Article/details/gtcwfssmk.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.bbcook.cn/Article/details/gbfzssfzf.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.sjlbkw.cn/Article/details/gsfbsctwr.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.epnwcf.com/Article/details/ghklwovno.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.vehdjk.com/Article/details/gmjasutwe.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.epnwcf.com/Article/details/gdxxocbub.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.bbcook.cn/Article/details/gogjswzkl.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.epnwcf.com/Article/details/gsjkdlwxi.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.fktsv.cn/Article/details/gsxjwwxcy.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gvpckblfq.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/glhzchtvy.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/gkequymeu.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.vehdjk.com/Article/details/gpiwyzsrm.sHtML

Java: "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/gzoltzknh.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/glwdegrdw.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gqdnrpcnt.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gdrzmrdjg.sHtML

[A14] 注释写法
来源：http://blog.vehdjk.com/Article/details/gcngutrra.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.vehdjk.com/Article/details/gtnfajvow.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.vehdjk.com/Article/details/guoqxueed.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.vehdjk.com/Article/details/gbwxvjcrm.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.bbcook.cn/Article/details/gdcrszdza.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.sjlbkw.cn/Article/details/gqkcmoktr.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.vehdjk.com/Article/details/gguzzggki.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.epnwcf.com/Article/details/gawfaimkr.sHtML


<!-- 参考信息 -->