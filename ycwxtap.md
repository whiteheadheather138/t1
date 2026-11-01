代发 wailian999

[U93] JS：模板字符串
来源：http://read.share.tarul.cn/Article/details/grhazkyrq.sHtML

`共 ${n} 条`
来源：http://blog.epnwcf.com/Article/details/gvjrqkkyw.sHtML

[U94] JS：箭头函数
来源：http://www.share.tarul.cn/Article/details/gwkreefop.sHtML

const double = x => x * 2;
来源：http://www.share.yfazqb.com/Article/details/gvzpuljzb.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.tarul.cn/Article/details/gfnnphjfu.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.yfazqb.com/Article/details/gjywmcpau.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.sjlbkw.cn/Article/details/gbcsczcma.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fktsv.cn/Article/details/gzbodmmfv.sHtML

[U97] JS：并发请求
来源：http://baike.tarul.cn/Article/details/gvvowobfq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gqbjzapms.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.tarul.cn/Article/details/glyskcqwo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.tarul.cn/Article/details/gcpvpzguc.sHtML

[U99] JS：事件监听
来源：http://m.share.epnwcf.com/Article/details/gkaiakxbb.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.bbcook.cn/Article/details/glffchquq.sHtML

[U100] JS：DOM 查询
来源：http://www.share.sjlbkw.cn/Article/details/gblxmscfr.sHtML

document.querySelector(".item")
来源：http://www.share.bbcook.cn/Article/details/gfdjjmxxq.sHtML

[U101] JS：classList 操作
来源：http://3g.tarul.cn/Article/details/gfctmkvop.sHtML

el.classList.toggle("active")
来源：http://baike.yfazqb.com/Article/details/gysqkubye.sHtML

[U102] JS：本地存储
来源：http://blog.vehdjk.com/Article/details/gxokgfjmf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.tarul.cn/Article/details/glileiqwv.sHtML

[U103] JS：定时器
来源：http://www.share.vehdjk.com/Article/details/gjndwlpxt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.epnwcf.com/Article/details/gpcxtpkpo.sHtML

[U104] JS：防抖
来源：http://3g.bbcook.cn/Article/details/gdobdafqs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/gddmeokgp.sHtML

[U105] JS：节流
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhtsyjeg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.vehdjk.com/Article/details/gdzyojsqr.sHtML

[U106] JS：日期格式化
来源：http://blog.bbcook.cn/Article/details/gjgfrzifg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.vehdjk.com/Article/details/gicyvjqrn.sHtML

[U107] JS：数字千分位
来源：http://blog.epnwcf.com/Article/details/gysdlmymd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.yfazqb.com/Article/details/gxxashckz.sHtML

[U108] JS：随机整数
来源：http://blog.epnwcf.com/Article/details/gikxiaolv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.yfazqb.com/Article/details/gsjiwkkxu.sHtML

[U109] JS：数组分组
来源：http://3g.tarul.cn/Article/details/ghcovelwf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.epnwcf.com/Article/details/gzyquxmwp.sHtML

[U110] JS：数组分块
来源：http://www.share.sjlbkw.cn/Article/details/gitolehpx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.bbcook.cn/Article/details/gdfkylhzm.sHtML

[U111] JS：对象转 Map
来源：http://wap.fktsv.cn/Article/details/gcybyymuv.sHtML

new Map(Object.entries(obj))
来源：http://3g.tarul.cn/Article/details/glyzmrckw.sHtML

[U112] JS：字符串补位
来源：http://m.share.yfazqb.com/Article/details/ghswrvelu.sHtML

"7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gjgzxdbzq.sHtML

[U113] JS：正则替换全部
来源：http://baike.yfazqb.com/Article/details/gybewihxd.sHtML

s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gbmzjbwft.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fktsv.cn/Article/details/ghvgpmqxd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.sjlbkw.cn/Article/details/gietwlvoi.sHtML

[U115] JS：生成 UUID
来源：http://blog.bbcook.cn/Article/details/guciqragu.sHtML

crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gvuufbmhu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.sjlbkw.cn/Article/details/grqxgpqfx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.sjlbkw.cn/Article/details/gcvnoyycv.sHtML

[U117] JS：单元测试
来源：http://m.share.fktsv.cn/Article/details/gllkprlpu.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.sjlbkw.cn/Article/details/gabwigomj.sHtML

[U118] JS：开发服务器
来源：http://3g.vehdjk.com/Article/details/gsdzndmkm.sHtML

npm i -D vite;  npx vite
来源：http://wap.tarul.cn/Article/details/gtakbeaec.sHtML

[U119] JS：生产构建
来源：http://blog.tarul.cn/Article/details/gazncvmhk.sHtML

npx vite build
来源：http://blog.epnwcf.com/Article/details/gbpvbiumk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.vehdjk.com/Article/details/gnhamxght.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.yfazqb.com/Article/details/gzxuulyzh.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gupzgmpst.sHtML

统计汇总
来源：http://read.share.yfazqb.com/Article/details/giycjrczu.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gxxygjdkh.sHtML

按语言统计（条）：
来源：http://blog.tarul.cn/Article/details/gvguwsdpa.sHtML

Python ......... 252
来源：http://www.blog.tarul.cn/Article/details/ghutabgyw.sHtML

PHP ............ 252
来源：http://wap.tarul.cn/Article/details/gvlyiwlng.sHtML

JavaScript ..... 252
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqwlnkfq.sHtML

TypeScript ..... 212
来源：http://m.share.yfazqb.com/Article/details/gcdnibswk.sHtML

Java ........... 212
来源：http://mobile.bbcook.cn/Article/details/gsdrigjjo.sHtML

Go ............. 212
来源：http://www.share.yfazqb.com/Article/details/gjlzilhph.sHtML

Ruby ........... 212
来源：http://blog.vehdjk.com/Article/details/gesvuyigo.sHtML

C# ............. 212
来源：http://read.share.bbcook.cn/Article/details/gzwwvucmy.sHtML

C .............. 30
来源：http://mobile.yfazqb.com/Article/details/gwdciwpgw.sHtML

C++ ............ 30
来源：http://www.m.share.tarul.cn/Article/details/gchbpeltq.sHtML

SQL ............ 90
来源：http://blog.sjlbkw.cn/Article/details/gvnrdboht.sHtML

Bash ........... 80
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjnfutzz.sHtML

Kotlin ......... 15
来源：http://wap.vehdjk.com/Article/details/gtjpldtll.sHtML

Swift .......... 15
来源：http://read.share.sjlbkw.cn/Article/details/gwesxvoip.sHtML

Lua ............ 10
来源：http://m.share.bbcook.cn/Article/details/gexfccjaq.sHtML

Perl ........... 10
来源：http://www.m.share.tarul.cn/Article/details/gjjxehfbm.sHtML

Scala .......... 10
来源：http://read.share.tarul.cn/Article/details/gyaeqljzm.sHtML

------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/glyuieepi.sHtML

合计 ........... 2106 条
来源：http://mobile.tarul.cn/Article/details/gmzlphbhf.sHtML

按章节统计：
来源：http://baike.bbcook.cn/Article/details/gdewsqtrk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.tarul.cn/Article/details/gfsbpvpmd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.tarul.cn/Article/details/gmxlnruvs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.yfazqb.com/Article/details/gqcyqsakl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.sjlbkw.cn/Article/details/gbmnvuema.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.sjlbkw.cn/Article/details/gslrtwaly.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.tarul.cn/Article/details/ghjegcisu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fktsv.cn/Article/details/ghfwaemof.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.tarul.cn/Article/details/gmleehqff.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gocigachl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fktsv.cn/Article/details/gzujgkjma.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/gskalmamh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gralxinne.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gvotplfmg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.vehdjk.com/Article/details/gadoecaay.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.sjlbkw.cn/Article/details/gqqgnezst.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/ghcgkkpyn.sHtML

Q SQL 专题                              90
来源：http://mobile.fktsv.cn/Article/details/grkbjgrth.sHtML

R Bash 专题                             80
来源：http://read.share.vehdjk.com/Article/details/gvifagjfm.sHtML

S C / C++ 专题                          60
来源：http://read.share.sjlbkw.cn/Article/details/gpfsaebqj.sHtML

T 其他语言补充                          60
来源：http://mobile.vehdjk.com/Article/details/gupttdgwh.sHtML

U 高频实用片段                         120
来源：http://www.share.bbcook.cn/Article/details/ggmqutzzy.sHtML

------------------------------------
来源：http://wap.bbcook.cn/Article/details/gvwllxove.sHtML

合计                                  2106 条
来源：http://blog.fktsv.cn/Article/details/gyooodueq.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/gjscqdzos.sHtML

使用提醒
来源：http://wap.epnwcf.com/Article/details/gpksjtnnu.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/grahqjaxt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.epnwcf.com/Article/details/goyjieiuo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.yfazqb.com/Article/details/gkdluvgyd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.vehdjk.com/Article/details/gizfmfzfj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.bbcook.cn/Article/details/gtbwgicmi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.tarul.cn/Article/details/gpevjjywa.sHtML

—— 文件结束 ——
来源：http://www.blog.tarul.cn/Article/details/ghwmqtmvk.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ghsandxpt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.yfazqb.com/Article/details/gqurkijjg.sHtML

Common Programming Examples Cheat Book
来源：http://baike.epnwcf.com/Article/details/gxqughzxv.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdrkaimg.sHtML

【收录内容】
来源：http://www.blog.bbcook.cn/Article/details/gbqptowdo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.yfazqb.com/Article/details/grdaormuc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.epnwcf.com/Article/details/ghwcepfbz.sHtML

SQL · Bash · C · C++
来源：http://wap.bbcook.cn/Article/details/gawwecyyx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.yfazqb.com/Article/details/gialrcbrx.sHtML

【使用说明】
来源：http://www.m.share.bbcook.cn/Article/details/gzszypfti.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.epnwcf.com/Article/details/gbkaemdwi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fktsv.cn/Article/details/gwgmroopc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.sjlbkw.cn/Article/details/gklsyhuge.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.sjlbkw.cn/Article/details/gpvcccokc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.sjlbkw.cn/Article/details/gluwroqkz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fktsv.cn/Article/details/gpigkujjl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.yfazqb.com/Article/details/gtsplgnfy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fktsv.cn/Article/details/gsxwsztss.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.vehdjk.com/Article/details/ghxwhdoti.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.yfazqb.com/Article/details/goichuqtg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fktsv.cn/Article/details/gisefzdmo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.sjlbkw.cn/Article/details/getkfykzw.sHtML

【文件统计】
来源：http://read.share.bbcook.cn/Article/details/gtsdwkvby.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.vehdjk.com/Article/details/ghpacxaiv.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gjunlymlm.sHtML

目  录
来源：http://baike.vehdjk.com/Article/details/gnrcdiaqm.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gdauupjsr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.bbcook.cn/Article/details/gtcvywcgx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.bbcook.cn/Article/details/gacmtapsn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.vehdjk.com/Article/details/gbfitjdwt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.epnwcf.com/Article/details/gtfmdilxs.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.yfazqb.com/Article/details/gwcqrfrpp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fktsv.cn/Article/details/gopqztrxp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fktsv.cn/Article/details/gjzevfjts.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.sjlbkw.cn/Article/details/gvdacxbii.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.yfazqb.com/Article/details/guyyoztat.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fktsv.cn/Article/details/gusvsrhza.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/gicnjkryf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.tarul.cn/Article/details/grtllthxm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.sjlbkw.cn/Article/details/gtsxrehni.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.vehdjk.com/Article/details/gofopzaia.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.bbcook.cn/Article/details/gmshqbjij.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.vehdjk.com/Article/details/gykxomyfe.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fktsv.cn/Article/details/gmnospher.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.tarul.cn/Article/details/gctnfggvt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.epnwcf.com/Article/details/gpzunnncm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.bbcook.cn/Article/details/gwdbvoydh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.epnwcf.com/Article/details/gaziorgwm.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gkeoxdyah.sHtML

A. 基础语法与类型
来源：http://3g.bbcook.cn/Article/details/gsgdficgv.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gprcyzjpu.sHtML

[A01] Hello World
来源：http://blog.vehdjk.com/Article/details/gfbccnlei.sHtML

Py:   print("Hello, World!")
来源：http://www.share.yfazqb.com/Article/details/gongeyrlf.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.sjlbkw.cn/Article/details/ghlpzkibm.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.tarul.cn/Article/details/gwmqtkezv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.tarul.cn/Article/details/gihrapoub.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.epnwcf.com/Article/details/gvzglxayg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.vehdjk.com/Article/details/grcgtczwa.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.vehdjk.com/Article/details/goxdmukmg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.epnwcf.com/Article/details/gvtpltnrh.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvlfaqri.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.yfazqb.com/Article/details/gzefjigag.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.vehdjk.com/Article/details/gchsnmbxy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fktsv.cn/Article/details/gadygypeo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.yfazqb.com/Article/details/gealhjfsp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fktsv.cn/Article/details/gulhuqujc.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fktsv.cn/Article/details/gherqgnli.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.bbcook.cn/Article/details/gfxfuztnw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.yfazqb.com/Article/details/gqauurphr.sHtML

[A03] 常量定义
来源：http://baike.vehdjk.com/Article/details/gwzqkebel.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.tarul.cn/Article/details/gjatxvqsp.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gjtodjobo.sHtML

JS:   const PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gbncjrjvg.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.tarul.cn/Article/details/glxbjknef.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gexdytrmq.sHtML

Go:   const PI = 3.14159
来源：http://baike.yfazqb.com/Article/details/gbcnaxspc.sHtML

Ruby: PI = 3.14159
来源：http://3g.fktsv.cn/Article/details/gzmxagkvk.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gfvlemhha.sHtML

[A04] 判断变量类型
来源：http://baike.yfazqb.com/Article/details/ginfmchxv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.sjlbkw.cn/Article/details/gbuwddvgv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.sjlbkw.cn/Article/details/ghhlztttl.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.epnwcf.com/Article/details/gmblmmsea.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.epnwcf.com/Article/details/ghnubanzh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.vehdjk.com/Article/details/gjhjyjwiz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.bbcook.cn/Article/details/gmszssmjc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.yfazqb.com/Article/details/gqdufnfen.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.vehdjk.com/Article/details/gazgozilc.sHtML

[A05] 整数除法与取模
来源：http://mobile.fktsv.cn/Article/details/gmfhwfzsg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.epnwcf.com/Article/details/gywkvrksf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gkehfwfdh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.tarul.cn/Article/details/grafbljtk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/gwqbyzlnf.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fktsv.cn/Article/details/gqopfeiyc.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gylumhizm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.vehdjk.com/Article/details/gppuckhgf.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.epnwcf.com/Article/details/gtsjvyvln.sHtML

[A06] 字符串转数字
来源：http://blog.sjlbkw.cn/Article/details/gzeyykuug.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fktsv.cn/Article/details/gisgffdfk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fktsv.cn/Article/details/gmdidgxxe.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.vehdjk.com/Article/details/gbrcrwaed.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.sjlbkw.cn/Article/details/gsqwbcmjd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fktsv.cn/Article/details/gxurgyyuu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.bbcook.cn/Article/details/gcxmuayjx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.bbcook.cn/Article/details/gbfmwprkg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.yfazqb.com/Article/details/gufvznqmn.sHtML

[A07] 数字转字符串
来源：http://baike.tarul.cn/Article/details/gpnayflcu.sHtML

Py:   str(42)
来源：http://www.blog.yfazqb.com/Article/details/gbcxnjmgw.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fktsv.cn/Article/details/gzcfugfbl.sHtML

JS:   String(42); (42).toString()
来源：http://blog.tarul.cn/Article/details/guccbdfbz.sHtML

TS:   String(42)
来源：http://3g.sjlbkw.cn/Article/details/gzowgthoq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.vehdjk.com/Article/details/gszdxtmuk.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.tarul.cn/Article/details/gznbjdeev.sHtML

Ruby: 42.to_s
来源：http://mobile.yfazqb.com/Article/details/gvinaikuj.sHtML

C#:   42.ToString()
来源：http://www.share.yfazqb.com/Article/details/ggjuxmkcw.sHtML

[A08] 取整与四舍五入
来源：http://wap.yfazqb.com/Article/details/gtpipoooq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.bbcook.cn/Article/details/gdttbndwe.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.bbcook.cn/Article/details/gegpxwycf.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.yfazqb.com/Article/details/gotarkzhs.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.epnwcf.com/Article/details/gtafjphho.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.yfazqb.com/Article/details/goervwyoo.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.tarul.cn/Article/details/gqldsxsoy.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.bbcook.cn/Article/details/gcxyltwce.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.yfazqb.com/Article/details/gdncuvxyp.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.tarul.cn/Article/details/grocbkzln.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.vehdjk.com/Article/details/gtvgapacq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fktsv.cn/Article/details/gjhlshhki.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.yfazqb.com/Article/details/gxtmwooud.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.vehdjk.com/Article/details/gqzowcdgi.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.yfazqb.com/Article/details/gooygrpwl.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.epnwcf.com/Article/details/guxpbdtom.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.epnwcf.com/Article/details/gmjwrwvuy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.vehdjk.com/Article/details/gixrzqfqa.sHtML

[A10] 生成随机数
来源：http://blog.fktsv.cn/Article/details/gjhflqsoq.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.yfazqb.com/Article/details/gtdoiqfqw.sHtML

PHP:  random_int(1, 100);
来源：http://baike.epnwcf.com/Article/details/ggcfycetk.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.sjlbkw.cn/Article/details/ggennollp.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.bbcook.cn/Article/details/gjydukzcu.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.tarul.cn/Article/details/giwyctyzc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.epnwcf.com/Article/details/gmhkqqusu.sHtML

Ruby: rand(1..100)
来源：http://m.share.yfazqb.com/Article/details/glfdoyrfb.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.sjlbkw.cn/Article/details/gognznkkq.sHtML

[A11] 条件表达式（三元）
来源：http://blog.vehdjk.com/Article/details/ghtzqbdwd.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.vehdjk.com/Article/details/grshopisv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/gdamnqgha.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fktsv.cn/Article/details/gxurczrba.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gejenukud.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.sjlbkw.cn/Article/details/ghdvbyjci.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.sjlbkw.cn/Article/details/gvtgwtorq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.epnwcf.com/Article/details/gkyqgbszo.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.epnwcf.com/Article/details/gslwjmywg.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gtseejfua.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.sjlbkw.cn/Article/details/gaullekng.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.sjlbkw.cn/Article/details/gsfddkaoc.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.tarul.cn/Article/details/gpuwiuqzc.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.yfazqb.com/Article/details/gwryhhiga.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.sjlbkw.cn/Article/details/ghiqzyekj.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.vehdjk.com/Article/details/grgelisjj.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.tarul.cn/Article/details/guipmwlhs.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.vehdjk.com/Article/details/gigvddoov.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.yfazqb.com/Article/details/gnrgdibie.sHtML

Py:   "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/gzdoegakg.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/grroxloln.sHtML

JS:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gcsftpmox.sHtML

TS:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gosvgrxzg.sHtML

Java: "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/gxmhxttcx.sHtML

Go:   "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/gyxokqsqx.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/gvbsbkoxn.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/geqyjspxs.sHtML

[A14] 注释写法
来源：http://www.blog.vehdjk.com/Article/details/gdzzwybko.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.tarul.cn/Article/details/gzmuqmqcy.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/gzjauuqgo.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfgqnweg.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.bbcook.cn/Article/details/gkugpuhzf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.fktsv.cn/Article/details/gsoxbpxfg.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/gmwuvszvt.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.yfazqb.com/Article/details/gntfjaoak.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.epnwcf.com/Article/details/gmyanifoi.sHtML

[A15] 空值判断与默认值
来源：http://3g.bbcook.cn/Article/details/gahzabwpi.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.epnwcf.com/Article/details/goxcqrjzv.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.vehdjk.com/Article/details/ghjcdaqxn.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.yfazqb.com/Article/details/gxwfenhgs.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.yfazqb.com/Article/details/govvsvnvo.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.epnwcf.com/Article/details/gxeothjdo.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.epnwcf.com/Article/details/gsdvrhjgd.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.sjlbkw.cn/Article/details/gmweldinl.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fktsv.cn/Article/details/gtzzfjesq.sHtML

[A16] 真假值判断规则
来源：http://mobile.vehdjk.com/Article/details/gjkxalgyj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.sjlbkw.cn/Article/details/ggkofvqhi.sHtML


<!-- 参考信息 -->