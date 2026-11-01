代发 wailian999

[U95] JS：Promise 包装
来源：http://wap.bbcook.cn/Article/details/ghjpsbvpa.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.sjlbkw.cn/Article/details/gydmuypjw.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.tarul.cn/Article/details/gsimzjfuq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gejdllifg.sHtML

[U97] JS：并发请求
来源：http://3g.tarul.cn/Article/details/gkohmuenr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.epnwcf.com/Article/details/gocodelxa.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.yfazqb.com/Article/details/giwnyjuov.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.bbcook.cn/Article/details/gmhvmkdof.sHtML

[U99] JS：事件监听
来源：http://wap.tarul.cn/Article/details/gjuvyncck.sHtML

el.addEventListener("click", e => {})
来源：http://wap.yfazqb.com/Article/details/gpeuzssmd.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.tarul.cn/Article/details/gjfvwfnqe.sHtML

document.querySelector(".item")
来源：http://www.share.vehdjk.com/Article/details/glyasdprp.sHtML

[U101] JS：classList 操作
来源：http://mobile.sjlbkw.cn/Article/details/gqbatbkqk.sHtML

el.classList.toggle("active")
来源：http://wap.fktsv.cn/Article/details/gcvpcscle.sHtML

[U102] JS：本地存储
来源：http://blog.epnwcf.com/Article/details/geuiliyjb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.tarul.cn/Article/details/grhlghctz.sHtML

[U103] JS：定时器
来源：http://read.share.bbcook.cn/Article/details/gpkdzsnxk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.tarul.cn/Article/details/ggypojrqg.sHtML

[U104] JS：防抖
来源：http://wap.epnwcf.com/Article/details/gkjrtcdrh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gmxrldclp.sHtML

[U105] JS：节流
来源：http://www.share.vehdjk.com/Article/details/gaesswlkn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.tarul.cn/Article/details/ggfmmmbum.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.epnwcf.com/Article/details/ghvsnoloo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.yfazqb.com/Article/details/gfpgiwvdp.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fktsv.cn/Article/details/giygusgis.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.epnwcf.com/Article/details/geinbkdns.sHtML

[U108] JS：随机整数
来源：http://blog.tarul.cn/Article/details/gqxbiqrpd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.vehdjk.com/Article/details/gjjdtfvfe.sHtML

[U109] JS：数组分组
来源：http://wap.tarul.cn/Article/details/guqfovfdn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.sjlbkw.cn/Article/details/gccrmnrat.sHtML

[U110] JS：数组分块
来源：http://m.share.tarul.cn/Article/details/gxqevwcju.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.vehdjk.com/Article/details/ggjpfmjox.sHtML

[U111] JS：对象转 Map
来源：http://m.share.yfazqb.com/Article/details/goekzeoge.sHtML

new Map(Object.entries(obj))
来源：http://mobile.vehdjk.com/Article/details/gzlwcaolh.sHtML

[U112] JS：字符串补位
来源：http://mobile.bbcook.cn/Article/details/gziibjrkm.sHtML

"7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gxlxxcurp.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.epnwcf.com/Article/details/gntzvgrwg.sHtML

s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gokxhvrqj.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fktsv.cn/Article/details/glndccqlp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.bbcook.cn/Article/details/gtkjtbrsf.sHtML

[U115] JS：生成 UUID
来源：http://3g.yfazqb.com/Article/details/ggpotirog.sHtML

crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/glswgkehu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.sjlbkw.cn/Article/details/gkvafnubo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.sjlbkw.cn/Article/details/gckesykia.sHtML

[U117] JS：单元测试
来源：http://blog.bbcook.cn/Article/details/gccwsgepw.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.yfazqb.com/Article/details/gxbqdyezf.sHtML

[U118] JS：开发服务器
来源：http://blog.bbcook.cn/Article/details/gtsbqkryx.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.yfazqb.com/Article/details/gmkfrsgxt.sHtML

[U119] JS：生产构建
来源：http://3g.vehdjk.com/Article/details/geubnyluv.sHtML

npx vite build
来源：http://wap.vehdjk.com/Article/details/gtfyuoemt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.bbcook.cn/Article/details/gmbbvwpru.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.yfazqb.com/Article/details/gkujlkzvd.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gcepbdwav.sHtML

统计汇总
来源：http://mobile.vehdjk.com/Article/details/ghiuqcstq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gfgzewcch.sHtML

按语言统计（条）：
来源：http://m.share.sjlbkw.cn/Article/details/gnscyqdkw.sHtML

Python ......... 252
来源：http://m.share.bbcook.cn/Article/details/gbrdfovev.sHtML

PHP ............ 252
来源：http://www.share.bbcook.cn/Article/details/gruyuawwb.sHtML

JavaScript ..... 252
来源：http://3g.yfazqb.com/Article/details/gpaatetql.sHtML

TypeScript ..... 212
来源：http://blog.vehdjk.com/Article/details/gibwhpdew.sHtML

Java ........... 212
来源：http://www.share.fktsv.cn/Article/details/gaavawrar.sHtML

Go ............. 212
来源：http://m.share.epnwcf.com/Article/details/gxcvsbybg.sHtML

Ruby ........... 212
来源：http://www.blog.yfazqb.com/Article/details/gmcdfzuta.sHtML

C# ............. 212
来源：http://mobile.bbcook.cn/Article/details/gtogacwbm.sHtML

C .............. 30
来源：http://3g.yfazqb.com/Article/details/gdriqkvus.sHtML

C++ ............ 30
来源：http://mobile.vehdjk.com/Article/details/gsxdfchjh.sHtML

SQL ............ 90
来源：http://read.share.sjlbkw.cn/Article/details/gydgrtcuo.sHtML

Bash ........... 80
来源：http://blog.epnwcf.com/Article/details/gexlcbnqp.sHtML

Kotlin ......... 15
来源：http://3g.vehdjk.com/Article/details/glaqxiglu.sHtML

Swift .......... 15
来源：http://m.share.bbcook.cn/Article/details/gikkwzcma.sHtML

Lua ............ 10
来源：http://read.share.bbcook.cn/Article/details/ggnozwsci.sHtML

Perl ........... 10
来源：http://m.share.sjlbkw.cn/Article/details/gqqgwpmqd.sHtML

Scala .......... 10
来源：http://www.share.sjlbkw.cn/Article/details/gotbsfjwz.sHtML

------------------------------------
来源：http://blog.bbcook.cn/Article/details/gmiobjxar.sHtML

合计 ........... 2106 条
来源：http://baike.bbcook.cn/Article/details/ghbcyoess.sHtML

按章节统计：
来源：http://mobile.tarul.cn/Article/details/gznsaktxk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.epnwcf.com/Article/details/gfwrsbsvw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fktsv.cn/Article/details/giufpujmi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fktsv.cn/Article/details/gjehortjn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.epnwcf.com/Article/details/geajoknvw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.epnwcf.com/Article/details/gyrsjlbdp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fktsv.cn/Article/details/gezrmyaks.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/gdiwuzxkj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.yfazqb.com/Article/details/gtnermdma.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gxtsfdmze.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fktsv.cn/Article/details/gukzbkksh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/glsbofpxm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/gbruvjihl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gnjdxzfgh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.epnwcf.com/Article/details/gvshelgit.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.vehdjk.com/Article/details/gdgxiltjn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/gtufkdsza.sHtML

Q SQL 专题                              90
来源：http://blog.epnwcf.com/Article/details/gaddznzym.sHtML

R Bash 专题                             80
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvimomyb.sHtML

S C / C++ 专题                          60
来源：http://3g.vehdjk.com/Article/details/grikrgwel.sHtML

T 其他语言补充                          60
来源：http://read.share.tarul.cn/Article/details/gqyavhktt.sHtML

U 高频实用片段                         120
来源：http://www.share.vehdjk.com/Article/details/gdgnvfkal.sHtML

------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/gxaygsvvw.sHtML

合计                                  2106 条
来源：http://baike.vehdjk.com/Article/details/gcagoftdm.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.tarul.cn/Article/details/gbzlxltbb.sHtML

使用提醒
来源：http://read.share.sjlbkw.cn/Article/details/gowberxns.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gauouevim.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.vehdjk.com/Article/details/gvfbkrqgz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.vehdjk.com/Article/details/gloifmfuj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.sjlbkw.cn/Article/details/gdemulwyt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fktsv.cn/Article/details/gpucnavup.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.bbcook.cn/Article/details/gpzbxmemm.sHtML

—— 文件结束 ——
来源：http://m.share.tarul.cn/Article/details/gpxvroblz.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gqyxqkjvp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.bbcook.cn/Article/details/gvuatfvxl.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.sjlbkw.cn/Article/details/gripvcgoz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ghyizlrxq.sHtML

【收录内容】
来源：http://blog.vehdjk.com/Article/details/gigtzyhwt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.epnwcf.com/Article/details/gvtpoluqb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.vehdjk.com/Article/details/gjmllxixt.sHtML

SQL · Bash · C · C++
来源：http://read.share.epnwcf.com/Article/details/gaxoiijeb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.epnwcf.com/Article/details/gshheciqt.sHtML

【使用说明】
来源：http://read.share.tarul.cn/Article/details/grbjfodrv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.tarul.cn/Article/details/gtjcislcu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fktsv.cn/Article/details/gcdyxocoz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.bbcook.cn/Article/details/gvbyfsjdx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.sjlbkw.cn/Article/details/gxnooupyi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.sjlbkw.cn/Article/details/gkozbjrqg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fktsv.cn/Article/details/gtwjpfjes.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fktsv.cn/Article/details/gshbbokui.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.tarul.cn/Article/details/gfukpnlbc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fktsv.cn/Article/details/gecxzjouz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.bbcook.cn/Article/details/glqwvgwkn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.vehdjk.com/Article/details/gtotyzhom.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.tarul.cn/Article/details/gmdczlpaf.sHtML

【文件统计】
来源：http://baike.vehdjk.com/Article/details/gsvvvhtak.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.yfazqb.com/Article/details/gnvjdgphf.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/goclwslhv.sHtML

目  录
来源：http://www.m.share.tarul.cn/Article/details/gktkrsqcl.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gyepbnqxi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.bbcook.cn/Article/details/gsxyfkkjx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhjcrges.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.tarul.cn/Article/details/gxjhemtit.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.vehdjk.com/Article/details/gwpsnqxju.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.yfazqb.com/Article/details/gbfladlsb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fktsv.cn/Article/details/gdgmlnboe.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.tarul.cn/Article/details/gpdrhlzkf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fktsv.cn/Article/details/ghlbshohc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/gacqxpael.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.yfazqb.com/Article/details/gomcyqaug.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.yfazqb.com/Article/details/gfsrqkrgf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gyhiuvuup.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fktsv.cn/Article/details/glzqmlsvf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.bbcook.cn/Article/details/giyddjjij.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fktsv.cn/Article/details/gpjawzxqn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.bbcook.cn/Article/details/gnslorucq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.sjlbkw.cn/Article/details/gsgkacxsr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.tarul.cn/Article/details/gxbnoxrop.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.tarul.cn/Article/details/gtkhrebyf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghclcqoft.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.yfazqb.com/Article/details/gmvbganbi.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gwtzstvkw.sHtML

A. 基础语法与类型
来源：http://www.blog.yfazqb.com/Article/details/gjnauoect.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gzidtfjeb.sHtML

[A01] Hello World
来源：http://3g.fktsv.cn/Article/details/gcoesgkon.sHtML

Py:   print("Hello, World!")
来源：http://3g.fktsv.cn/Article/details/gimqoenzc.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.yfazqb.com/Article/details/ghlrqpvjt.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.tarul.cn/Article/details/gzjyhnovn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.bbcook.cn/Article/details/gcvrenoeg.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.sjlbkw.cn/Article/details/gtdybhims.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.tarul.cn/Article/details/ggqybptbw.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.tarul.cn/Article/details/gcihdzjcy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fktsv.cn/Article/details/gtqjqkhqr.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.bbcook.cn/Article/details/gfnttviyo.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fktsv.cn/Article/details/gwiclgwtz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.bbcook.cn/Article/details/gfgmwuubc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.epnwcf.com/Article/details/goxbhtoci.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.tarul.cn/Article/details/gngrrnmgw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.bbcook.cn/Article/details/gzjsxzbbq.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.sjlbkw.cn/Article/details/gjlujsrkz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fktsv.cn/Article/details/gmoisbsbh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.tarul.cn/Article/details/gjhpevuyq.sHtML

[A03] 常量定义
来源：http://read.share.tarul.cn/Article/details/gbreyhasq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fktsv.cn/Article/details/gpqxmunya.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gkwvpvsfx.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/ggitnugmn.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/grinwexwc.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/goguqkrsg.sHtML

Go:   const PI = 3.14159
来源：http://3g.tarul.cn/Article/details/ggbfxrzpd.sHtML

Ruby: PI = 3.14159
来源：http://3g.fktsv.cn/Article/details/glzvjfusc.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gzedmodaw.sHtML

[A04] 判断变量类型
来源：http://blog.tarul.cn/Article/details/gjlndjbie.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.epnwcf.com/Article/details/glvinljyo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.bbcook.cn/Article/details/gwcrpnpsb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.tarul.cn/Article/details/gfmqyxrxy.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.vehdjk.com/Article/details/gpghnojvr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.bbcook.cn/Article/details/gbuvvpuzu.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.sjlbkw.cn/Article/details/gurnuawmo.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fktsv.cn/Article/details/goltladtn.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.vehdjk.com/Article/details/gclkjekhv.sHtML

[A05] 整数除法与取模
来源：http://read.share.tarul.cn/Article/details/gjgtghrbd.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.vehdjk.com/Article/details/gdckwltqf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/glxairdws.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gtlgiezhl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.bbcook.cn/Article/details/gquzeaxry.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/gbagqaasu.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gzdlyavay.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.bbcook.cn/Article/details/gpzesgjkl.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.bbcook.cn/Article/details/gkxafguxo.sHtML

[A06] 字符串转数字
来源：http://www.share.vehdjk.com/Article/details/guvsnlysr.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.vehdjk.com/Article/details/gmtcxxfgp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.bbcook.cn/Article/details/gjvuyctxa.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.epnwcf.com/Article/details/groojexju.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.bbcook.cn/Article/details/ggchdwxev.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.yfazqb.com/Article/details/ghwqovunb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.tarul.cn/Article/details/gorfuxadp.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.bbcook.cn/Article/details/gjoikwxdj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.tarul.cn/Article/details/gjxgsbblc.sHtML

[A07] 数字转字符串
来源：http://m.share.tarul.cn/Article/details/gjotdvvlt.sHtML

Py:   str(42)
来源：http://mobile.tarul.cn/Article/details/gknbwjecp.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.yfazqb.com/Article/details/gbotyudcb.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.sjlbkw.cn/Article/details/gdqbrvvkt.sHtML

TS:   String(42)
来源：http://read.share.fktsv.cn/Article/details/gwyhylqdw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fktsv.cn/Article/details/gqtiywsga.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.tarul.cn/Article/details/glhxmjaac.sHtML

Ruby: 42.to_s
来源：http://wap.sjlbkw.cn/Article/details/guxfuvvdq.sHtML

C#:   42.ToString()
来源：http://3g.tarul.cn/Article/details/gknijkkje.sHtML

[A08] 取整与四舍五入
来源：http://baike.sjlbkw.cn/Article/details/gnzotciwa.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.yfazqb.com/Article/details/gkmubwpkj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fktsv.cn/Article/details/gzpvdtauk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.sjlbkw.cn/Article/details/groiynuph.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.sjlbkw.cn/Article/details/gczoypcqa.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.tarul.cn/Article/details/gfalaghir.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fktsv.cn/Article/details/gcjutfyxx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.vehdjk.com/Article/details/gygsjjzqa.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.sjlbkw.cn/Article/details/gffhkjfpv.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.yfazqb.com/Article/details/gtexucnuv.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.epnwcf.com/Article/details/gbilcuvuh.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gtqjlvoqm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.epnwcf.com/Article/details/goxyotagv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.tarul.cn/Article/details/gejdrsfab.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/gcvgpcjya.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.yfazqb.com/Article/details/gafouikex.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.bbcook.cn/Article/details/gypqcmnzd.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.tarul.cn/Article/details/giwmfmbcw.sHtML

[A10] 生成随机数
来源：http://www.m.share.bbcook.cn/Article/details/gdjuahpwm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.sjlbkw.cn/Article/details/gldlxnzex.sHtML

PHP:  random_int(1, 100);
来源：http://baike.bbcook.cn/Article/details/gggwcbfvi.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.yfazqb.com/Article/details/gcwhifrow.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fktsv.cn/Article/details/gbmmbxtkd.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.tarul.cn/Article/details/gxcshzazo.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxbbyakt.sHtML

Ruby: rand(1..100)
来源：http://blog.tarul.cn/Article/details/gqpuminqz.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fktsv.cn/Article/details/gqrwoczje.sHtML

[A11] 条件表达式（三元）
来源：http://blog.sjlbkw.cn/Article/details/gnhyvshsr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.tarul.cn/Article/details/gjefjtslo.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.bbcook.cn/Article/details/gtobjmzvy.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.tarul.cn/Article/details/ghshdkazq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.tarul.cn/Article/details/gdjayczbs.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.epnwcf.com/Article/details/gbmyogmqw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.vehdjk.com/Article/details/gggmkjbxv.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.fktsv.cn/Article/details/gsabhkhai.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.bbcook.cn/Article/details/gpjshuezo.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.yfazqb.com/Article/details/gqhadvzjm.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.yfazqb.com/Article/details/gmzxpsuwr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fktsv.cn/Article/details/geqhvhlsh.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.yfazqb.com/Article/details/gfcbwabcu.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fktsv.cn/Article/details/grtvnzbih.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.vehdjk.com/Article/details/gbwsopnjh.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.tarul.cn/Article/details/gdyoacyrc.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.yfazqb.com/Article/details/gimmzzlgw.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.tarul.cn/Article/details/gbcgyxrnm.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.yfazqb.com/Article/details/gwbcarlzh.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gjfyubtud.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gxkhcusrq.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.vehdjk.com/Article/details/gjztknvjz.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.tarul.cn/Article/details/gzxuvzpdt.sHtML

Java: "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/gvzumnogf.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gwcexcozw.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gqseurrhh.sHtML

C#:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gqpojeysa.sHtML

[A14] 注释写法
来源：http://wap.yfazqb.com/Article/details/gocyeyvse.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.yfazqb.com/Article/details/gpfqlenhl.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.fktsv.cn/Article/details/gwsmltkqf.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.bbcook.cn/Article/details/gmhokwnzc.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.yfazqb.com/Article/details/gfianpwcm.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fktsv.cn/Article/details/gtgtzlatp.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.epnwcf.com/Article/details/glsgpbgvl.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.vehdjk.com/Article/details/gnlzuxnli.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.tarul.cn/Article/details/gimqrvycs.sHtML

[A15] 空值判断与默认值
来源：http://mobile.vehdjk.com/Article/details/gfkhjfhgn.sHtML

Py:   value = data or "默认值"
来源：http://wap.sjlbkw.cn/Article/details/gmjdormcn.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.yfazqb.com/Article/details/gcgepnoes.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.bbcook.cn/Article/details/gedndhqlj.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.vehdjk.com/Article/details/gijmumtgt.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.sjlbkw.cn/Article/details/grvhjbype.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.bbcook.cn/Article/details/glyppcdmc.sHtML

Ruby: value = data || "默认值"
来源：http://baike.vehdjk.com/Article/details/gaylplyoq.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.sjlbkw.cn/Article/details/galesrqrh.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.epnwcf.com/Article/details/gavyqfvfj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.tarul.cn/Article/details/gtcjllius.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.vehdjk.com/Article/details/gzkgdtwhg.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.vehdjk.com/Article/details/gxmasoefa.sHtML

TS:   if (!x) {}
来源：http://www.m.share.bbcook.cn/Article/details/gasdpnvhv.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.tarul.cn/Article/details/gcxvezfpc.sHtML


<!-- 参考信息 -->