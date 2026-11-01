代发 wailian999

[U93] JS：模板字符串
来源：http://wap.sjlbkw.cn/Article/details/gsbimhvxu.sHtML

`共 ${n} 条`
来源：http://www.m.share.bbcook.cn/Article/details/glmgnlywc.sHtML

[U94] JS：箭头函数
来源：http://blog.epnwcf.com/Article/details/gpnzaniha.sHtML

const double = x => x * 2;
来源：http://baike.fktsv.cn/Article/details/guyjjttei.sHtML

[U95] JS：Promise 包装
来源：http://blog.epnwcf.com/Article/details/geemshgbm.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.yfazqb.com/Article/details/gfkwgspil.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.yfazqb.com/Article/details/gegqhhrux.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/guzouvnpa.sHtML

[U97] JS：并发请求
来源：http://3g.sjlbkw.cn/Article/details/geyfggeqv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/ggwqcljue.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.bbcook.cn/Article/details/grmfnhkqd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.yfazqb.com/Article/details/gpmessdfx.sHtML

[U99] JS：事件监听
来源：http://m.share.bbcook.cn/Article/details/gmqpzisbc.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fktsv.cn/Article/details/gzwigqgfb.sHtML

[U100] JS：DOM 查询
来源：http://www.share.yfazqb.com/Article/details/gbphtuzql.sHtML

document.querySelector(".item")
来源：http://3g.bbcook.cn/Article/details/gilgbzevy.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxubonau.sHtML

el.classList.toggle("active")
来源：http://m.share.fktsv.cn/Article/details/gvuirhfza.sHtML

[U102] JS：本地存储
来源：http://3g.sjlbkw.cn/Article/details/ghmhtxmnp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.tarul.cn/Article/details/ggufixbkj.sHtML

[U103] JS：定时器
来源：http://www.blog.yfazqb.com/Article/details/gfcqufvdp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.sjlbkw.cn/Article/details/gzegcpehm.sHtML

[U104] JS：防抖
来源：http://3g.epnwcf.com/Article/details/gnydenyat.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gohrgkqqs.sHtML

[U105] JS：节流
来源：http://read.share.tarul.cn/Article/details/ggipokvdm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.bbcook.cn/Article/details/gbmttpymo.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fktsv.cn/Article/details/gggtagbcs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.epnwcf.com/Article/details/gdtfhbdkc.sHtML

[U107] JS：数字千分位
来源：http://3g.sjlbkw.cn/Article/details/gmvjmferz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.tarul.cn/Article/details/gvswirwlj.sHtML

[U108] JS：随机整数
来源：http://wap.vehdjk.com/Article/details/gznjsufcs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.yfazqb.com/Article/details/geymuifpz.sHtML

[U109] JS：数组分组
来源：http://mobile.fktsv.cn/Article/details/grpmzwnuz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.bbcook.cn/Article/details/gweglogiw.sHtML

[U110] JS：数组分块
来源：http://www.share.fktsv.cn/Article/details/gxvualboa.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.vehdjk.com/Article/details/gmvaemiwr.sHtML

[U111] JS：对象转 Map
来源：http://baike.epnwcf.com/Article/details/gyroeiaxw.sHtML

new Map(Object.entries(obj))
来源：http://read.share.sjlbkw.cn/Article/details/gpvbegjdr.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.sjlbkw.cn/Article/details/gguyyajzc.sHtML

"7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/ghaqsbkca.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.vehdjk.com/Article/details/goytiaukc.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/ghyadnorh.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.sjlbkw.cn/Article/details/gfyrbsdqg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fktsv.cn/Article/details/gohnmugyq.sHtML

[U115] JS：生成 UUID
来源：http://wap.epnwcf.com/Article/details/glpxpnjrf.sHtML

crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/gwgflbzes.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.tarul.cn/Article/details/gvwlrrtfu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.sjlbkw.cn/Article/details/gufuunjav.sHtML

[U117] JS：单元测试
来源：http://wap.yfazqb.com/Article/details/gpakqpovj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.epnwcf.com/Article/details/gsstokajv.sHtML

[U118] JS：开发服务器
来源：http://read.share.yfazqb.com/Article/details/gpsdqdggr.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fktsv.cn/Article/details/gpyxneoxh.sHtML

[U119] JS：生产构建
来源：http://www.share.yfazqb.com/Article/details/gtrtrgbdv.sHtML

npx vite build
来源：http://wap.epnwcf.com/Article/details/gtfwjnmfb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.bbcook.cn/Article/details/gogljqvto.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.vehdjk.com/Article/details/gqjtpxzwl.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gzuyatpew.sHtML

统计汇总
来源：http://m.share.bbcook.cn/Article/details/gskhqbhom.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gbqvkejga.sHtML

按语言统计（条）：
来源：http://www.share.yfazqb.com/Article/details/gokonmzdp.sHtML

Python ......... 252
来源：http://www.blog.tarul.cn/Article/details/glswpuddc.sHtML

PHP ............ 252
来源：http://m.share.epnwcf.com/Article/details/gieupysmg.sHtML

JavaScript ..... 252
来源：http://wap.vehdjk.com/Article/details/gfyzqymfd.sHtML

TypeScript ..... 212
来源：http://3g.epnwcf.com/Article/details/grpzgvgmk.sHtML

Java ........... 212
来源：http://www.m.share.tarul.cn/Article/details/gqmnvqpep.sHtML

Go ............. 212
来源：http://www.blog.sjlbkw.cn/Article/details/gcxgqvjim.sHtML

Ruby ........... 212
来源：http://www.blog.fktsv.cn/Article/details/guwikdfqw.sHtML

C# ............. 212
来源：http://baike.epnwcf.com/Article/details/gbeqdhaze.sHtML

C .............. 30
来源：http://mobile.sjlbkw.cn/Article/details/gmialgkiu.sHtML

C++ ............ 30
来源：http://3g.vehdjk.com/Article/details/gawjuzzse.sHtML

SQL ............ 90
来源：http://www.blog.epnwcf.com/Article/details/glmfnhvfh.sHtML

Bash ........... 80
来源：http://www.m.share.sjlbkw.cn/Article/details/gunwrjsjf.sHtML

Kotlin ......... 15
来源：http://www.share.epnwcf.com/Article/details/gvyoqsgct.sHtML

Swift .......... 15
来源：http://wap.sjlbkw.cn/Article/details/gkjrcwfrv.sHtML

Lua ............ 10
来源：http://read.share.sjlbkw.cn/Article/details/gktevadjr.sHtML

Perl ........... 10
来源：http://www.blog.epnwcf.com/Article/details/gumhakzhz.sHtML

Scala .......... 10
来源：http://blog.epnwcf.com/Article/details/gmtgpsoij.sHtML

------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gnjtmdhvf.sHtML

合计 ........... 2106 条
来源：http://mobile.sjlbkw.cn/Article/details/ghvognmxi.sHtML

按章节统计：
来源：http://m.share.sjlbkw.cn/Article/details/gqkfgvttk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.vehdjk.com/Article/details/gdlpntdou.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.sjlbkw.cn/Article/details/geblwutdk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.tarul.cn/Article/details/gdtqrruzh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.tarul.cn/Article/details/geowlepap.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.sjlbkw.cn/Article/details/gimbezlkd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fktsv.cn/Article/details/gudsdizwi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.epnwcf.com/Article/details/gzbyltwro.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.tarul.cn/Article/details/gezxnihci.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gxhkawzdg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.yfazqb.com/Article/details/gortkgjpi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gbbjxyaos.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/glmqgriqo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/gyobxwnoo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fktsv.cn/Article/details/ggaqrptpc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.vehdjk.com/Article/details/gofjzoyqq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/gerzypyxn.sHtML

Q SQL 专题                              90
来源：http://www.m.share.bbcook.cn/Article/details/gesivhctl.sHtML

R Bash 专题                             80
来源：http://www.share.vehdjk.com/Article/details/gascqzyqt.sHtML

S C / C++ 专题                          60
来源：http://wap.fktsv.cn/Article/details/gvrgpeefm.sHtML

T 其他语言补充                          60
来源：http://blog.vehdjk.com/Article/details/gqvjxsodg.sHtML

U 高频实用片段                         120
来源：http://wap.yfazqb.com/Article/details/ggsynyzxg.sHtML

------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gjbtzixsn.sHtML

合计                                  2106 条
来源：http://www.m.share.tarul.cn/Article/details/gjjbwshqn.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/gmzmwlzna.sHtML

使用提醒
来源：http://www.share.epnwcf.com/Article/details/gbdcrnnnw.sHtML

--------------------------------------------------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gwjlnjlje.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.sjlbkw.cn/Article/details/glcqmebhi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.vehdjk.com/Article/details/gcnthzaua.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.vehdjk.com/Article/details/guglutosd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.bbcook.cn/Article/details/gjdivpglv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.yfazqb.com/Article/details/gftmhcfpd.sHtML

—— 文件结束 ——
来源：http://www.share.yfazqb.com/Article/details/gyuovkumf.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gelsvexec.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fktsv.cn/Article/details/gqeteqfjz.sHtML

Common Programming Examples Cheat Book
来源：http://baike.tarul.cn/Article/details/gohjdjupo.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gpbkxxhtw.sHtML

【收录内容】
来源：http://baike.vehdjk.com/Article/details/gqkkeyrsg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.sjlbkw.cn/Article/details/gjishplgb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.tarul.cn/Article/details/glnmgqdfv.sHtML

SQL · Bash · C · C++
来源：http://3g.sjlbkw.cn/Article/details/gkwqpblgo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.yfazqb.com/Article/details/gzifxzazt.sHtML

【使用说明】
来源：http://3g.bbcook.cn/Article/details/glkmkkiue.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.sjlbkw.cn/Article/details/gospjwhtl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.tarul.cn/Article/details/gthbkdcby.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fktsv.cn/Article/details/grqvwowzh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.yfazqb.com/Article/details/geqloaaen.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.yfazqb.com/Article/details/gqlrnwmqq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.sjlbkw.cn/Article/details/ghuijmhgt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.vehdjk.com/Article/details/gffspkyiz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.yfazqb.com/Article/details/groeuvwml.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.bbcook.cn/Article/details/glcokhxpm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.bbcook.cn/Article/details/gojmynhzl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.bbcook.cn/Article/details/gkfyfpall.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fktsv.cn/Article/details/gwhbdspxt.sHtML

【文件统计】
来源：http://read.share.vehdjk.com/Article/details/guhptqkzn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.vehdjk.com/Article/details/gndzskuuh.sHtML

--------------------------------------------------------------------------------
来源：http://wap.tarul.cn/Article/details/grkxjcrgm.sHtML

目  录
来源：http://wap.bbcook.cn/Article/details/gifpvgdbc.sHtML

--------------------------------------------------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gnekuimst.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.vehdjk.com/Article/details/gxbxxcieg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.bbcook.cn/Article/details/gsshnvddn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.tarul.cn/Article/details/gskdsqjgq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.yfazqb.com/Article/details/gjuxmgree.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.bbcook.cn/Article/details/gbnoeqaey.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.tarul.cn/Article/details/gcxntkpbi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/gutwkjqfh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.vehdjk.com/Article/details/girtzijkq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gfubdcpzp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.yfazqb.com/Article/details/gldedzift.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.epnwcf.com/Article/details/ghiinmkwj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/gexzmjekh.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fktsv.cn/Article/details/gsmfcayap.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.yfazqb.com/Article/details/gecqfziwb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.tarul.cn/Article/details/gzypunaus.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/gfhcqqeal.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.tarul.cn/Article/details/gqfgfezgo.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.epnwcf.com/Article/details/gedkfmghr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.sjlbkw.cn/Article/details/gyphnfigk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.bbcook.cn/Article/details/griuwmpth.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fktsv.cn/Article/details/gzcwjsiyy.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gyrtijyjy.sHtML

A. 基础语法与类型
来源：http://www.blog.tarul.cn/Article/details/gpaztwfjp.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gzwxqtcnb.sHtML

[A01] Hello World
来源：http://www.share.fktsv.cn/Article/details/gyhptcwyu.sHtML

Py:   print("Hello, World!")
来源：http://m.share.sjlbkw.cn/Article/details/gcjonyvnl.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.vehdjk.com/Article/details/gollfgqyx.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.vehdjk.com/Article/details/gyfluulmx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.vehdjk.com/Article/details/gaehokroh.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fktsv.cn/Article/details/glwvungaz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.tarul.cn/Article/details/gtkykfpez.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fktsv.cn/Article/details/gilkdfben.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.sjlbkw.cn/Article/details/gvotkbwki.sHtML

[A02] 变量声明与赋值
来源：http://baike.tarul.cn/Article/details/gdtttorjb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.tarul.cn/Article/details/gojbrypgf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gxzzgpljr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fktsv.cn/Article/details/gomstwrbv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.vehdjk.com/Article/details/gydrcnxff.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fktsv.cn/Article/details/gouocevel.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.vehdjk.com/Article/details/giycpnrto.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.tarul.cn/Article/details/gsdlklbwk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fktsv.cn/Article/details/gqjgrzxpa.sHtML

[A03] 常量定义
来源：http://www.share.vehdjk.com/Article/details/gamsxsutu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.epnwcf.com/Article/details/gwpvpltgb.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/gbyfsbffo.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gqqcweejq.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gfonymhjv.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gmjqrqzme.sHtML

Go:   const PI = 3.14159
来源：http://blog.epnwcf.com/Article/details/glfwqyeqa.sHtML

Ruby: PI = 3.14159
来源：http://mobile.bbcook.cn/Article/details/gnljjuofr.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gogisjuku.sHtML

[A04] 判断变量类型
来源：http://wap.fktsv.cn/Article/details/gjpyjtcai.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fktsv.cn/Article/details/grgtneklt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.sjlbkw.cn/Article/details/givkaddbh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.yfazqb.com/Article/details/gyshwopee.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.epnwcf.com/Article/details/gcdkglmuu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.sjlbkw.cn/Article/details/gtzjphtve.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.epnwcf.com/Article/details/ginwiaqxm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.epnwcf.com/Article/details/gplujrclj.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.vehdjk.com/Article/details/gmtixsvrh.sHtML

[A05] 整数除法与取模
来源：http://blog.fktsv.cn/Article/details/gzfswshhk.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.bbcook.cn/Article/details/guugdobkg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.epnwcf.com/Article/details/gihsbeevr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fktsv.cn/Article/details/gukadmgzm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.sjlbkw.cn/Article/details/gihvyzkgp.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/gtszclzoi.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/gbironcux.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gzvxfswik.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fktsv.cn/Article/details/ghhfujktd.sHtML

[A06] 字符串转数字
来源：http://read.share.vehdjk.com/Article/details/gahmebwxe.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.vehdjk.com/Article/details/ggkoeabxp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.epnwcf.com/Article/details/gbpdenoci.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fktsv.cn/Article/details/gzzfurael.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.sjlbkw.cn/Article/details/gxuqtdspf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.tarul.cn/Article/details/gvispuuhs.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.sjlbkw.cn/Article/details/glibbesjd.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.yfazqb.com/Article/details/gbphpkgue.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.epnwcf.com/Article/details/gwanbzwpz.sHtML

[A07] 数字转字符串
来源：http://www.blog.yfazqb.com/Article/details/grpioutoe.sHtML

Py:   str(42)
来源：http://www.m.share.vehdjk.com/Article/details/gbbgglwsi.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.epnwcf.com/Article/details/gmhruiapm.sHtML

JS:   String(42); (42).toString()
来源：http://3g.bbcook.cn/Article/details/gxxlbvzkn.sHtML

TS:   String(42)
来源：http://blog.bbcook.cn/Article/details/grtafhzku.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.epnwcf.com/Article/details/gyqmibvef.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.bbcook.cn/Article/details/gvrsvvfgb.sHtML

Ruby: 42.to_s
来源：http://read.share.sjlbkw.cn/Article/details/gtoitdvgs.sHtML

C#:   42.ToString()
来源：http://baike.vehdjk.com/Article/details/gntovytjf.sHtML

[A08] 取整与四舍五入
来源：http://mobile.vehdjk.com/Article/details/grmifufqp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.bbcook.cn/Article/details/gvwrtvqzv.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.tarul.cn/Article/details/gyprcqnxh.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.epnwcf.com/Article/details/glbkjpmmw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.sjlbkw.cn/Article/details/gctcxjbvb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.epnwcf.com/Article/details/gdbawvuzf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.tarul.cn/Article/details/gvrvbwoui.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.vehdjk.com/Article/details/gyrtxbwtf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.sjlbkw.cn/Article/details/gqadylqcu.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.tarul.cn/Article/details/gyebvxgvw.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.bbcook.cn/Article/details/gfsddcqmc.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.epnwcf.com/Article/details/gloaewnuk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.tarul.cn/Article/details/grdzitjxt.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.vehdjk.com/Article/details/gldfaqlyq.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/ggsmexzlp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.sjlbkw.cn/Article/details/gxiwwrjyc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.vehdjk.com/Article/details/gxpckdwar.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.yfazqb.com/Article/details/gvvavfqhp.sHtML

[A10] 生成随机数
来源：http://wap.vehdjk.com/Article/details/gzelxqqgu.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.vehdjk.com/Article/details/giezjzhjq.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.yfazqb.com/Article/details/gzgskbszq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.yfazqb.com/Article/details/gsgihophh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.yfazqb.com/Article/details/ghkcpmxsz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.tarul.cn/Article/details/gfopitsuw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.epnwcf.com/Article/details/gvqygldqs.sHtML

Ruby: rand(1..100)
来源：http://read.share.epnwcf.com/Article/details/gwswywsox.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.vehdjk.com/Article/details/gywyymbry.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.epnwcf.com/Article/details/goghosrte.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.fktsv.cn/Article/details/gddssdhto.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.sjlbkw.cn/Article/details/gvxmbvmmy.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.bbcook.cn/Article/details/gsheusdsi.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.tarul.cn/Article/details/giesavoif.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.sjlbkw.cn/Article/details/gjyhpuodq.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fktsv.cn/Article/details/gjuwpmlak.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.epnwcf.com/Article/details/gcitgbuur.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.sjlbkw.cn/Article/details/gkjsyykdv.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.yfazqb.com/Article/details/gjckisnkb.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.fktsv.cn/Article/details/gywklgavd.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.tarul.cn/Article/details/glhmqgjvx.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.yfazqb.com/Article/details/gvitmlawj.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.yfazqb.com/Article/details/gwyzjtjhq.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.bbcook.cn/Article/details/ghuxfgprl.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.bbcook.cn/Article/details/ggxijubwi.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.tarul.cn/Article/details/gbqfdmxls.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.vehdjk.com/Article/details/gicacoupy.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.yfazqb.com/Article/details/gcoydnfci.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/gnvlhtesj.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gvvwolcqh.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.bbcook.cn/Article/details/gnitjgfqp.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gnntcwadi.sHtML

Java: "第一行\n第二行"
来源：http://www.share.epnwcf.com/Article/details/gqvkwdwun.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/glfxbfypo.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gvjguqjuh.sHtML

C#:   "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/gyyghtshm.sHtML

[A14] 注释写法
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwayjvgf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.bbcook.cn/Article/details/gluvmfcql.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.yfazqb.com/Article/details/gqabkrpqi.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.bbcook.cn/Article/details/gkkraueqk.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.epnwcf.com/Article/details/gehfjqlju.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.vehdjk.com/Article/details/ghigljxqj.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/gnosqrwnb.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.sjlbkw.cn/Article/details/gsjfqqazn.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.epnwcf.com/Article/details/gtjiwfymg.sHtML

[A15] 空值判断与默认值
来源：http://m.share.tarul.cn/Article/details/gxodmfyog.sHtML

Py:   value = data or "默认值"
来源：http://3g.vehdjk.com/Article/details/glximafaz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.tarul.cn/Article/details/gwbpyfbon.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.yfazqb.com/Article/details/gyoxboajf.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.fktsv.cn/Article/details/ggwumherl.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.vehdjk.com/Article/details/gkwmskpds.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.fktsv.cn/Article/details/gjdsabdsq.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.tarul.cn/Article/details/googtnezg.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.tarul.cn/Article/details/gmucbensg.sHtML

[A16] 真假值判断规则
来源：http://m.share.yfazqb.com/Article/details/gyoklafea.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.epnwcf.com/Article/details/ggppciowr.sHtML


<!-- 参考信息 -->