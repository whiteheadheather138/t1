代发 wailian999

[U93] JS：模板字符串
来源：http://www.m.share.epnwcf.com/Article/details/glsckjczz.sHtML

`共 ${n} 条`
来源：http://www.share.sjlbkw.cn/Article/details/gsvenomrm.sHtML

[U94] JS：箭头函数
来源：http://mobile.tarul.cn/Article/details/gakczwodw.sHtML

const double = x => x * 2;
来源：http://wap.vehdjk.com/Article/details/gbfglacxd.sHtML

[U95] JS：Promise 包装
来源：http://read.share.epnwcf.com/Article/details/gallombtj.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.epnwcf.com/Article/details/gvqdvimih.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fktsv.cn/Article/details/gzaxqfjgg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gjsvwarha.sHtML

[U97] JS：并发请求
来源：http://mobile.yfazqb.com/Article/details/gzhujrgfz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gstvxgbxe.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.sjlbkw.cn/Article/details/gthyzcryq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.vehdjk.com/Article/details/gqtsroonq.sHtML

[U99] JS：事件监听
来源：http://www.share.vehdjk.com/Article/details/gzktlyylp.sHtML

el.addEventListener("click", e => {})
来源：http://wap.tarul.cn/Article/details/geutruura.sHtML

[U100] JS：DOM 查询
来源：http://m.share.bbcook.cn/Article/details/gipnwktfh.sHtML

document.querySelector(".item")
来源：http://mobile.fktsv.cn/Article/details/ggieuixjk.sHtML

[U101] JS：classList 操作
来源：http://m.share.bbcook.cn/Article/details/gskpdyooy.sHtML

el.classList.toggle("active")
来源：http://www.share.fktsv.cn/Article/details/gzwwcmajq.sHtML

[U102] JS：本地存储
来源：http://wap.vehdjk.com/Article/details/gmoevqpky.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.bbcook.cn/Article/details/ghplxflds.sHtML

[U103] JS：定时器
来源：http://mobile.epnwcf.com/Article/details/gppdzrsop.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.vehdjk.com/Article/details/gnednczze.sHtML

[U104] JS：防抖
来源：http://www.m.share.bbcook.cn/Article/details/gahdnncim.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.bbcook.cn/Article/details/geibdfdea.sHtML

[U105] JS：节流
来源：http://baike.yfazqb.com/Article/details/gghwtktzl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.yfazqb.com/Article/details/gvlrevlfd.sHtML

[U106] JS：日期格式化
来源：http://wap.sjlbkw.cn/Article/details/gwqyfxmmk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.bbcook.cn/Article/details/gcadlufgh.sHtML

[U107] JS：数字千分位
来源：http://m.share.yfazqb.com/Article/details/grfetpdwz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.yfazqb.com/Article/details/gjdytgrzw.sHtML

[U108] JS：随机整数
来源：http://mobile.sjlbkw.cn/Article/details/gwxwxgepv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.tarul.cn/Article/details/gsvpehbna.sHtML

[U109] JS：数组分组
来源：http://read.share.bbcook.cn/Article/details/ghhiynpro.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.bbcook.cn/Article/details/gmikfnaej.sHtML

[U110] JS：数组分块
来源：http://baike.tarul.cn/Article/details/gkujzzhrs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fktsv.cn/Article/details/gjfyyvefi.sHtML

[U111] JS：对象转 Map
来源：http://mobile.vehdjk.com/Article/details/gsvzalube.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.yfazqb.com/Article/details/gptnfuoco.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.tarul.cn/Article/details/gbezduxdg.sHtML

"7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gmjviarbe.sHtML

[U113] JS：正则替换全部
来源：http://blog.fktsv.cn/Article/details/grlrvfsdj.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gwkwoerul.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.bbcook.cn/Article/details/gyfghqlmr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.bbcook.cn/Article/details/geldjsthc.sHtML

[U115] JS：生成 UUID
来源：http://www.share.sjlbkw.cn/Article/details/grkqqljts.sHtML

crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gwjvfgtzw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.tarul.cn/Article/details/gvgletlwg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fktsv.cn/Article/details/gcboaocbi.sHtML

[U117] JS：单元测试
来源：http://blog.bbcook.cn/Article/details/gygsahsga.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.sjlbkw.cn/Article/details/gsljmcpie.sHtML

[U118] JS：开发服务器
来源：http://blog.epnwcf.com/Article/details/gphkoexhl.sHtML

npm i -D vite;  npx vite
来源：http://wap.sjlbkw.cn/Article/details/gvkjdyprk.sHtML

[U119] JS：生产构建
来源：http://blog.yfazqb.com/Article/details/gqulrxfxh.sHtML

npx vite build
来源：http://www.blog.yfazqb.com/Article/details/glneythjm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.yfazqb.com/Article/details/gmgpsztpw.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.bbcook.cn/Article/details/gounnvyri.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gsxvpbgpd.sHtML

统计汇总
来源：http://www.blog.yfazqb.com/Article/details/glmotuiod.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gucgocdhh.sHtML

按语言统计（条）：
来源：http://www.m.share.yfazqb.com/Article/details/gvympmlpn.sHtML

Python ......... 252
来源：http://www.blog.vehdjk.com/Article/details/grmruhtbh.sHtML

PHP ............ 252
来源：http://www.m.share.tarul.cn/Article/details/gkqanavmy.sHtML

JavaScript ..... 252
来源：http://www.blog.epnwcf.com/Article/details/gbmhabdyi.sHtML

TypeScript ..... 212
来源：http://www.m.share.tarul.cn/Article/details/getpzzqbo.sHtML

Java ........... 212
来源：http://www.blog.vehdjk.com/Article/details/gnwokznip.sHtML

Go ............. 212
来源：http://3g.bbcook.cn/Article/details/gibchbbrd.sHtML

Ruby ........... 212
来源：http://www.m.share.yfazqb.com/Article/details/gmzgrmdul.sHtML

C# ............. 212
来源：http://www.share.vehdjk.com/Article/details/gnntsdbpb.sHtML

C .............. 30
来源：http://wap.fktsv.cn/Article/details/grhuofogw.sHtML

C++ ............ 30
来源：http://www.share.sjlbkw.cn/Article/details/gtupauyde.sHtML

SQL ............ 90
来源：http://www.m.share.sjlbkw.cn/Article/details/gyczxdeec.sHtML

Bash ........... 80
来源：http://www.m.share.sjlbkw.cn/Article/details/guvxxypvh.sHtML

Kotlin ......... 15
来源：http://baike.yfazqb.com/Article/details/ghxchxhps.sHtML

Swift .......... 15
来源：http://www.blog.bbcook.cn/Article/details/gxdwxlbpy.sHtML

Lua ............ 10
来源：http://mobile.vehdjk.com/Article/details/gwtremhwv.sHtML

Perl ........... 10
来源：http://blog.fktsv.cn/Article/details/gicyhdnvc.sHtML

Scala .......... 10
来源：http://www.blog.vehdjk.com/Article/details/gcacovnju.sHtML

------------------------------------
来源：http://blog.epnwcf.com/Article/details/ghljysngj.sHtML

合计 ........... 2106 条
来源：http://www.m.share.vehdjk.com/Article/details/gmaytejyy.sHtML

按章节统计：
来源：http://read.share.epnwcf.com/Article/details/guhmtjvwb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.epnwcf.com/Article/details/gsbqqviox.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.vehdjk.com/Article/details/gebgtccyt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.tarul.cn/Article/details/gzejqwakc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.vehdjk.com/Article/details/gozaqolap.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.tarul.cn/Article/details/gefjzjdfu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.epnwcf.com/Article/details/gevigffmu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.vehdjk.com/Article/details/glhqjfsdv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.bbcook.cn/Article/details/gdzautlsd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fktsv.cn/Article/details/gxeiygtpp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.sjlbkw.cn/Article/details/gebtpzngd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gfmdyjxdo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/gbeujxbmp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/gnrhaclcm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.tarul.cn/Article/details/gkzchyggy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.tarul.cn/Article/details/gstdgknje.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gdqgoaagb.sHtML

Q SQL 专题                              90
来源：http://baike.epnwcf.com/Article/details/gbokymsov.sHtML

R Bash 专题                             80
来源：http://wap.tarul.cn/Article/details/gxxvslvky.sHtML

S C / C++ 专题                          60
来源：http://blog.yfazqb.com/Article/details/gxvvyguyb.sHtML

T 其他语言补充                          60
来源：http://www.share.bbcook.cn/Article/details/glbaankiv.sHtML

U 高频实用片段                         120
来源：http://read.share.tarul.cn/Article/details/glzjviooq.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/gdnpbgakf.sHtML

合计                                  2106 条
来源：http://www.m.share.fktsv.cn/Article/details/gzzoxexqc.sHtML

--------------------------------------------------------------------------------
来源：http://baike.tarul.cn/Article/details/gtiezvzos.sHtML

使用提醒
来源：http://3g.fktsv.cn/Article/details/gkwqpwuao.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/gknoqkewc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.fktsv.cn/Article/details/gzeqcfqiz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.yfazqb.com/Article/details/gsracloxg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fktsv.cn/Article/details/gmzuftujo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.vehdjk.com/Article/details/gayrfblko.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.tarul.cn/Article/details/gcoaxuvzn.sHtML

—— 文件结束 ——
来源：http://m.share.fktsv.cn/Article/details/ghysldftm.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gqnozgtcb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fktsv.cn/Article/details/guyedbohb.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.tarul.cn/Article/details/grldeqarr.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gyadbqnvf.sHtML

【收录内容】
来源：http://mobile.yfazqb.com/Article/details/gtlzmnmdi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fktsv.cn/Article/details/gaoyxznjn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.epnwcf.com/Article/details/gghgmrgzc.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fktsv.cn/Article/details/gzlofuaod.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.tarul.cn/Article/details/gfgosqjlv.sHtML

【使用说明】
来源：http://www.blog.epnwcf.com/Article/details/gxvtvzagp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.vehdjk.com/Article/details/ggqlqlydw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.epnwcf.com/Article/details/googhiavm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.epnwcf.com/Article/details/ggrjfdxxe.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.sjlbkw.cn/Article/details/gfxhgqale.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.yfazqb.com/Article/details/gtpnihpoq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.sjlbkw.cn/Article/details/ghvkgrnzi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.sjlbkw.cn/Article/details/guamlrorg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.bbcook.cn/Article/details/gnqskilpw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fktsv.cn/Article/details/gkhyecvfy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fktsv.cn/Article/details/gfigenhfz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.epnwcf.com/Article/details/gkdgxuclm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.yfazqb.com/Article/details/gqcdnicnv.sHtML

【文件统计】
来源：http://3g.bbcook.cn/Article/details/gnnztwbwf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.bbcook.cn/Article/details/gqhzdqngi.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gspwooflw.sHtML

目  录
来源：http://www.m.share.vehdjk.com/Article/details/gszyoqztg.sHtML

--------------------------------------------------------------------------------
来源：http://baike.vehdjk.com/Article/details/gbqaovvbg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.bbcook.cn/Article/details/gvjbcvbqt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.epnwcf.com/Article/details/glkevwtiv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.yfazqb.com/Article/details/gdnhcmnpp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.tarul.cn/Article/details/gpzlfqsbg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.epnwcf.com/Article/details/gezqvjeea.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fktsv.cn/Article/details/gqazygtoi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.yfazqb.com/Article/details/giwuiisfv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.vehdjk.com/Article/details/glncpddya.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.yfazqb.com/Article/details/goxpqbogr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.sjlbkw.cn/Article/details/gepdqqypo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/gyecmtujk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gcnyafjie.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/gbwrllmnc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fktsv.cn/Article/details/grkeubvmt.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.yfazqb.com/Article/details/gzuurknsu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.vehdjk.com/Article/details/ggcaykguh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fktsv.cn/Article/details/gtezjpaah.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.tarul.cn/Article/details/gztispxjg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.sjlbkw.cn/Article/details/gynbkiimt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/gcexkkshc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.yfazqb.com/Article/details/gqmvebdew.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gljcdbucj.sHtML

A. 基础语法与类型
来源：http://www.m.share.fktsv.cn/Article/details/gtrpklwdk.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gjkickedb.sHtML

[A01] Hello World
来源：http://wap.yfazqb.com/Article/details/goebaglvl.sHtML

Py:   print("Hello, World!")
来源：http://blog.epnwcf.com/Article/details/gnaswoilg.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.epnwcf.com/Article/details/gillrjcfa.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.bbcook.cn/Article/details/gctctzxhv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.sjlbkw.cn/Article/details/gocxrvtdz.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.bbcook.cn/Article/details/gsegepnox.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.epnwcf.com/Article/details/ghreetzjb.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.tarul.cn/Article/details/giljglmhd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.tarul.cn/Article/details/gvawqcwxb.sHtML

[A02] 变量声明与赋值
来源：http://www.share.epnwcf.com/Article/details/geqhoqqch.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.epnwcf.com/Article/details/grhzdzrtu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fktsv.cn/Article/details/goamqsejx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fktsv.cn/Article/details/gdxyzichc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.vehdjk.com/Article/details/gdognyjbu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fktsv.cn/Article/details/gbeqxmajq.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.yfazqb.com/Article/details/gqcwzbpdh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.sjlbkw.cn/Article/details/ggjxzqaor.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.bbcook.cn/Article/details/gyhfqwcni.sHtML

[A03] 常量定义
来源：http://baike.bbcook.cn/Article/details/gavpodbvs.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fktsv.cn/Article/details/gtzgedxfp.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gqgadycgr.sHtML

JS:   const PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/gcjaaqhpw.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gnxfvbnuz.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/grlthflxr.sHtML

Go:   const PI = 3.14159
来源：http://m.share.tarul.cn/Article/details/gphxztumv.sHtML

Ruby: PI = 3.14159
来源：http://baike.tarul.cn/Article/details/gnkthunlk.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gmnzjvqbi.sHtML

[A04] 判断变量类型
来源：http://www.share.yfazqb.com/Article/details/gzeqznthz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.sjlbkw.cn/Article/details/gvunobdmz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.bbcook.cn/Article/details/gnoxgupqz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.vehdjk.com/Article/details/gdbebwycv.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.tarul.cn/Article/details/gqbsdmrzn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.yfazqb.com/Article/details/gqjyftiye.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.bbcook.cn/Article/details/gkxvgtfbc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.epnwcf.com/Article/details/gxdvoqpfs.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.epnwcf.com/Article/details/gfankdcdi.sHtML

[A05] 整数除法与取模
来源：http://blog.bbcook.cn/Article/details/gnkmleqsk.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fktsv.cn/Article/details/glmalfwhy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgvjwnni.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.tarul.cn/Article/details/gckmzmjyd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.yfazqb.com/Article/details/gvcdysnal.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gvlipakva.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.epnwcf.com/Article/details/gbuluyvzs.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fktsv.cn/Article/details/glozdwhuz.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.vehdjk.com/Article/details/gkilfcfqp.sHtML

[A06] 字符串转数字
来源：http://blog.bbcook.cn/Article/details/ghfdpddkj.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.sjlbkw.cn/Article/details/gkzzjtfrb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.bbcook.cn/Article/details/gcywhqtnf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.fktsv.cn/Article/details/gkuagmfmr.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.bbcook.cn/Article/details/gcctcqjhh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.bbcook.cn/Article/details/glmxaqnaf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.tarul.cn/Article/details/gljcjumqx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.bbcook.cn/Article/details/gzqofiitl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fktsv.cn/Article/details/gnjpdklye.sHtML

[A07] 数字转字符串
来源：http://www.share.tarul.cn/Article/details/gyzpjtesh.sHtML

Py:   str(42)
来源：http://wap.tarul.cn/Article/details/gtotatemo.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.vehdjk.com/Article/details/gtlbvbmyo.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.yfazqb.com/Article/details/galteqnrc.sHtML

TS:   String(42)
来源：http://m.share.vehdjk.com/Article/details/goovhwvef.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.epnwcf.com/Article/details/gotunbkiy.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.bbcook.cn/Article/details/gfmvlbbvj.sHtML

Ruby: 42.to_s
来源：http://mobile.vehdjk.com/Article/details/gcapfdrmw.sHtML

C#:   42.ToString()
来源：http://m.share.yfazqb.com/Article/details/grfhzphyr.sHtML

[A08] 取整与四舍五入
来源：http://blog.bbcook.cn/Article/details/ghpabajwh.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/gmsmcfqrj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.sjlbkw.cn/Article/details/gcburulow.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.vehdjk.com/Article/details/gxskkpxhx.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.vehdjk.com/Article/details/glpcjgicm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.epnwcf.com/Article/details/gddmvaimi.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.epnwcf.com/Article/details/gsjwdsltv.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.vehdjk.com/Article/details/gusexznab.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.tarul.cn/Article/details/grpoealzk.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.yfazqb.com/Article/details/gwdmuzkzg.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.bbcook.cn/Article/details/gjbxxgyzu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gshfcakdu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.yfazqb.com/Article/details/gaegkcmxc.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gwslewycp.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.tarul.cn/Article/details/geuntcgob.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.tarul.cn/Article/details/grjzzmorx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.vehdjk.com/Article/details/gmrsaxaha.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.tarul.cn/Article/details/grdduedov.sHtML

[A10] 生成随机数
来源：http://read.share.vehdjk.com/Article/details/gtytbvfky.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.tarul.cn/Article/details/gfvpldzat.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.yfazqb.com/Article/details/gtwdseoha.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.yfazqb.com/Article/details/gxoxwfhay.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.epnwcf.com/Article/details/gcswuyswh.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.vehdjk.com/Article/details/gwrmpkmpq.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.epnwcf.com/Article/details/gdpfxajsu.sHtML

Ruby: rand(1..100)
来源：http://mobile.epnwcf.com/Article/details/ghevmfcen.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.epnwcf.com/Article/details/gmadxckok.sHtML

[A11] 条件表达式（三元）
来源：http://baike.yfazqb.com/Article/details/gtllrmqwz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.yfazqb.com/Article/details/gbaijcioq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/gccnclori.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.epnwcf.com/Article/details/gpwtebkeh.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.epnwcf.com/Article/details/gjzlhzzxn.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.bbcook.cn/Article/details/gukpvwthr.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.epnwcf.com/Article/details/gjtaptwjo.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.sjlbkw.cn/Article/details/gjimabcdw.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.bbcook.cn/Article/details/gshyaregz.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.epnwcf.com/Article/details/gtxipulyd.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.fktsv.cn/Article/details/gmkmgdqmo.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.vehdjk.com/Article/details/gwbidthhv.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fktsv.cn/Article/details/gnophqgbo.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.yfazqb.com/Article/details/gcwfroagv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.bbcook.cn/Article/details/gcqydprhq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.vehdjk.com/Article/details/gzxanreuz.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.epnwcf.com/Article/details/gapfqtpxo.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.bbcook.cn/Article/details/gbqhttyai.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.tarul.cn/Article/details/gnjvwcbfo.sHtML

Py:   "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/gmjuinylo.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.vehdjk.com/Article/details/gwayejife.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gybykzfrt.sHtML

TS:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/gamikolfa.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/gqkfrbhda.sHtML

Go:   "第一行\n第二行"
来源：http://baike.yfazqb.com/Article/details/gbpkmgdrm.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.vehdjk.com/Article/details/ghorivfum.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/gmkcqzuzo.sHtML

[A14] 注释写法
来源：http://blog.epnwcf.com/Article/details/gqjqtfsop.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.yfazqb.com/Article/details/grtxkpmfm.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/ghuvdgqyd.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.vehdjk.com/Article/details/gvjbhakct.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.yfazqb.com/Article/details/guqpjmsvp.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.yfazqb.com/Article/details/gvwbptheg.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.vehdjk.com/Article/details/gbhzaahkv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.epnwcf.com/Article/details/gnrymvjlc.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.sjlbkw.cn/Article/details/gisanfhzg.sHtML

[A15] 空值判断与默认值
来源：http://blog.yfazqb.com/Article/details/gfrjdffas.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.bbcook.cn/Article/details/gubaliroj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.tarul.cn/Article/details/gswixhuag.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.sjlbkw.cn/Article/details/gcnyyhjlj.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.tarul.cn/Article/details/gcogwuikp.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.fktsv.cn/Article/details/gvbcpeykn.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.vehdjk.com/Article/details/gqeuyddtj.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.bbcook.cn/Article/details/gejarrntr.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.vehdjk.com/Article/details/ghlrwhlqy.sHtML

[A16] 真假值判断规则
来源：http://3g.sjlbkw.cn/Article/details/gclzfwumo.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.bbcook.cn/Article/details/gbecdyuhk.sHtML


<!-- 参考信息 -->