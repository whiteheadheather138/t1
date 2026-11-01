代发 wailian999

[U91] JS：对象键值遍历
来源：http://wap.yfazqb.com/Article/details/gclhhbrop.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.yfazqb.com/Article/details/gojlhxaty.sHtML

[U92] JS：深拷贝
来源：http://www.blog.tarul.cn/Article/details/gwhisjixe.sHtML

structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/guzxlkcqg.sHtML

[U93] JS：模板字符串
来源：http://www.blog.yfazqb.com/Article/details/gsfieyzog.sHtML

`共 ${n} 条`
来源：http://baike.bbcook.cn/Article/details/gdjnobroh.sHtML

[U94] JS：箭头函数
来源：http://blog.bbcook.cn/Article/details/gtfckcdyu.sHtML

const double = x => x * 2;
来源：http://3g.tarul.cn/Article/details/gwdnvzyqz.sHtML

[U95] JS：Promise 包装
来源：http://wap.sjlbkw.cn/Article/details/gfrdwqfnu.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fktsv.cn/Article/details/gljoyxaeo.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.bbcook.cn/Article/details/gwqdbliyy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gyklnfljd.sHtML

[U97] JS：并发请求
来源：http://mobile.vehdjk.com/Article/details/ggynjfzct.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gfttkokzk.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.bbcook.cn/Article/details/gszmpxpuz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.sjlbkw.cn/Article/details/gkiluvpcp.sHtML

[U99] JS：事件监听
来源：http://3g.vehdjk.com/Article/details/gkcjgeiun.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.yfazqb.com/Article/details/grelpbdfj.sHtML

[U100] JS：DOM 查询
来源：http://m.share.vehdjk.com/Article/details/gzdkpteaz.sHtML

document.querySelector(".item")
来源：http://read.share.fktsv.cn/Article/details/ghptqlirj.sHtML

[U101] JS：classList 操作
来源：http://wap.vehdjk.com/Article/details/gxegksjho.sHtML

el.classList.toggle("active")
来源：http://www.blog.tarul.cn/Article/details/gcknycqeh.sHtML

[U102] JS：本地存储
来源：http://3g.vehdjk.com/Article/details/guvylifsq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.epnwcf.com/Article/details/gzidwxrkt.sHtML

[U103] JS：定时器
来源：http://mobile.sjlbkw.cn/Article/details/gyunpxfen.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.sjlbkw.cn/Article/details/getjzucka.sHtML

[U104] JS：防抖
来源：http://m.share.epnwcf.com/Article/details/gjelvuyvr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/giawdylud.sHtML

[U105] JS：节流
来源：http://www.blog.epnwcf.com/Article/details/gneasqoeu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.bbcook.cn/Article/details/gjoxjivtg.sHtML

[U106] JS：日期格式化
来源：http://mobile.vehdjk.com/Article/details/gimbjbpjy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.epnwcf.com/Article/details/gtsxqzegh.sHtML

[U107] JS：数字千分位
来源：http://m.share.epnwcf.com/Article/details/ghlsubkwy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.bbcook.cn/Article/details/gpucogewh.sHtML

[U108] JS：随机整数
来源：http://www.m.share.epnwcf.com/Article/details/gfrwhfkds.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.sjlbkw.cn/Article/details/ghcekuhha.sHtML

[U109] JS：数组分组
来源：http://mobile.epnwcf.com/Article/details/giooymbvq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.tarul.cn/Article/details/gwjxtqeta.sHtML

[U110] JS：数组分块
来源：http://read.share.tarul.cn/Article/details/gopdloqnv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.tarul.cn/Article/details/gshxzqhbk.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fktsv.cn/Article/details/gijvrxwxj.sHtML

new Map(Object.entries(obj))
来源：http://baike.fktsv.cn/Article/details/gpiuaflnk.sHtML

[U112] JS：字符串补位
来源：http://read.share.epnwcf.com/Article/details/ggxinkhrx.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gevntemyg.sHtML

[U113] JS：正则替换全部
来源：http://mobile.yfazqb.com/Article/details/gmzfevstv.sHtML

s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/grqkrvomq.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.sjlbkw.cn/Article/details/gylwezkat.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.yfazqb.com/Article/details/guetajlab.sHtML

[U115] JS：生成 UUID
来源：http://m.share.vehdjk.com/Article/details/gjqlelyyk.sHtML

crypto.randomUUID()
来源：http://mobile.yfazqb.com/Article/details/gsqzgkvjv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fktsv.cn/Article/details/gvorkjmig.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.tarul.cn/Article/details/gpndubeyp.sHtML

[U117] JS：单元测试
来源：http://www.blog.bbcook.cn/Article/details/gqkchvugh.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.bbcook.cn/Article/details/gleiosetn.sHtML

[U118] JS：开发服务器
来源：http://wap.vehdjk.com/Article/details/gdmckdctt.sHtML

npm i -D vite;  npx vite
来源：http://3g.epnwcf.com/Article/details/gaksistnp.sHtML

[U119] JS：生产构建
来源：http://www.share.bbcook.cn/Article/details/gtrviqbdu.sHtML

npx vite build
来源：http://wap.bbcook.cn/Article/details/ghvzjypie.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.sjlbkw.cn/Article/details/gpekwkpqi.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.epnwcf.com/Article/details/gubzwnmhj.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gkqemsgjp.sHtML

统计汇总
来源：http://read.share.vehdjk.com/Article/details/gtdcdecwj.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gmsvuyxgl.sHtML

按语言统计（条）：
来源：http://www.m.share.fktsv.cn/Article/details/gnqzdgpqx.sHtML

Python ......... 252
来源：http://m.share.vehdjk.com/Article/details/gjeqszsgb.sHtML

PHP ............ 252
来源：http://read.share.fktsv.cn/Article/details/gkiixqmgp.sHtML

JavaScript ..... 252
来源：http://baike.sjlbkw.cn/Article/details/guaplfsxd.sHtML

TypeScript ..... 212
来源：http://m.share.sjlbkw.cn/Article/details/gzgfxygub.sHtML

Java ........... 212
来源：http://www.m.share.tarul.cn/Article/details/gjtvqrjcn.sHtML

Go ............. 212
来源：http://blog.tarul.cn/Article/details/gzuvzogvn.sHtML

Ruby ........... 212
来源：http://blog.yfazqb.com/Article/details/gxpqetdcs.sHtML

C# ............. 212
来源：http://www.blog.yfazqb.com/Article/details/gjjecoraw.sHtML

C .............. 30
来源：http://read.share.sjlbkw.cn/Article/details/gmhuiwhog.sHtML

C++ ............ 30
来源：http://blog.fktsv.cn/Article/details/gzsjpakkt.sHtML

SQL ............ 90
来源：http://3g.tarul.cn/Article/details/gdixzujhh.sHtML

Bash ........... 80
来源：http://www.share.tarul.cn/Article/details/gxqkhbiaz.sHtML

Kotlin ......... 15
来源：http://www.m.share.sjlbkw.cn/Article/details/gggazgsak.sHtML

Swift .......... 15
来源：http://baike.fktsv.cn/Article/details/gdlspnpqf.sHtML

Lua ............ 10
来源：http://www.m.share.vehdjk.com/Article/details/gskuancqn.sHtML

Perl ........... 10
来源：http://mobile.tarul.cn/Article/details/gpfnsbjku.sHtML

Scala .......... 10
来源：http://wap.fktsv.cn/Article/details/gwzfyxkuh.sHtML

------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gxfiyoccn.sHtML

合计 ........... 2106 条
来源：http://baike.vehdjk.com/Article/details/ghiuqafut.sHtML

按章节统计：
来源：http://blog.sjlbkw.cn/Article/details/gnldknkdi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fktsv.cn/Article/details/gambavkal.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.yfazqb.com/Article/details/gxtjnmldw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.tarul.cn/Article/details/gzhxwlcqx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.epnwcf.com/Article/details/goohdqxky.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fktsv.cn/Article/details/gtkigjzsp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.epnwcf.com/Article/details/giqndxfka.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.yfazqb.com/Article/details/gmdyefemk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fktsv.cn/Article/details/goduvadtb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gapbzchow.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.yfazqb.com/Article/details/gkvanapbo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/gurkiumoh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gkuswlwkm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gllhtiurk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.epnwcf.com/Article/details/gosprvyya.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.bbcook.cn/Article/details/gxrprmcab.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.epnwcf.com/Article/details/gbbiddvci.sHtML

Q SQL 专题                              90
来源：http://mobile.fktsv.cn/Article/details/gmqqxwuhg.sHtML

R Bash 专题                             80
来源：http://3g.epnwcf.com/Article/details/gjivzfyvx.sHtML

S C / C++ 专题                          60
来源：http://mobile.epnwcf.com/Article/details/gfxypixwy.sHtML

T 其他语言补充                          60
来源：http://3g.fktsv.cn/Article/details/gskugfxrf.sHtML

U 高频实用片段                         120
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkvksale.sHtML

------------------------------------
来源：http://3g.tarul.cn/Article/details/glblrtbqk.sHtML

合计                                  2106 条
来源：http://read.share.vehdjk.com/Article/details/gctlqtdwn.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gpojbkhsp.sHtML

使用提醒
来源：http://www.m.share.sjlbkw.cn/Article/details/gakziytpg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gakkwnnck.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.sjlbkw.cn/Article/details/gogsrgxrs.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.sjlbkw.cn/Article/details/grtsnvxtz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fktsv.cn/Article/details/gqkhemfkp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.sjlbkw.cn/Article/details/ghengquzv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.yfazqb.com/Article/details/gjolnyids.sHtML

—— 文件结束 ——
来源：http://3g.epnwcf.com/Article/details/gpfaqcvyn.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/glvrgqpgr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fktsv.cn/Article/details/gwyflbqja.sHtML

Common Programming Examples Cheat Book
来源：http://blog.sjlbkw.cn/Article/details/glfwqblzz.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gbuuqerpa.sHtML

【收录内容】
来源：http://www.blog.tarul.cn/Article/details/gkqupropx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.yfazqb.com/Article/details/gckljctag.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.bbcook.cn/Article/details/gddjrjayd.sHtML

SQL · Bash · C · C++
来源：http://3g.tarul.cn/Article/details/gkactqjhf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.yfazqb.com/Article/details/gucjxrlgh.sHtML

【使用说明】
来源：http://baike.yfazqb.com/Article/details/gastdiwuy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.tarul.cn/Article/details/gtblaaciz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fktsv.cn/Article/details/gcddgipot.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.vehdjk.com/Article/details/grmxuyqig.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.epnwcf.com/Article/details/gbbnrfsyj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fktsv.cn/Article/details/geefrgxus.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.bbcook.cn/Article/details/gobgumief.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fktsv.cn/Article/details/gnckdrhbp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.sjlbkw.cn/Article/details/gwtxolgza.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.sjlbkw.cn/Article/details/gadqhuunr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.vehdjk.com/Article/details/gohouhrph.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.bbcook.cn/Article/details/gwsypbtqo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.sjlbkw.cn/Article/details/gghxvdzwx.sHtML

【文件统计】
来源：http://blog.epnwcf.com/Article/details/godqzkhxk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.yfazqb.com/Article/details/gyjhiekfj.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/gwlrfqvki.sHtML

目  录
来源：http://www.m.share.bbcook.cn/Article/details/gwmqsssjg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gucsweuak.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.epnwcf.com/Article/details/glqhjdiuo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fktsv.cn/Article/details/gfpqyockw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.vehdjk.com/Article/details/gvilrogrx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.yfazqb.com/Article/details/gnomgzfli.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.yfazqb.com/Article/details/gzlhelekw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.vehdjk.com/Article/details/gihtnngyw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.bbcook.cn/Article/details/gvyuwuawh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.tarul.cn/Article/details/gygvlmytt.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/ghbkfxucm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.vehdjk.com/Article/details/gusrtqtqd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.vehdjk.com/Article/details/gxqrqqyrc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/gukvkimqy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/gxgqlnsnh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.sjlbkw.cn/Article/details/gvmnkjunm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fktsv.cn/Article/details/gqmajckec.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/ghqwghxet.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.yfazqb.com/Article/details/gepmzecsp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.bbcook.cn/Article/details/geqjztuqt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fktsv.cn/Article/details/gosxerxsk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.vehdjk.com/Article/details/guasredst.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.yfazqb.com/Article/details/gqsfwffpg.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gxssbbzby.sHtML

A. 基础语法与类型
来源：http://www.share.yfazqb.com/Article/details/gxgmtgdhl.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gyrvpgfer.sHtML

[A01] Hello World
来源：http://baike.vehdjk.com/Article/details/grbrphjmp.sHtML

Py:   print("Hello, World!")
来源：http://www.share.bbcook.cn/Article/details/gycnhbzqm.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.vehdjk.com/Article/details/gqzkryavk.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.sjlbkw.cn/Article/details/gqcpohrfp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.epnwcf.com/Article/details/gjcabfdpx.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.sjlbkw.cn/Article/details/gjmopiluf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fktsv.cn/Article/details/gzdsounym.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.sjlbkw.cn/Article/details/gdiwzklte.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.vehdjk.com/Article/details/gzqpwhhrj.sHtML

[A02] 变量声明与赋值
来源：http://www.share.epnwcf.com/Article/details/gqiyxneto.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fktsv.cn/Article/details/ggwnnqqdy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.tarul.cn/Article/details/gjqpfefqt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.sjlbkw.cn/Article/details/gujdopjpj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.vehdjk.com/Article/details/gvewgptnm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.sjlbkw.cn/Article/details/guilxpdro.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.bbcook.cn/Article/details/ghjanedvp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.yfazqb.com/Article/details/gxkbpbitf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.yfazqb.com/Article/details/gxxfsjips.sHtML

[A03] 常量定义
来源：http://read.share.vehdjk.com/Article/details/ghnpqlhnk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.sjlbkw.cn/Article/details/gkmazxeox.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gbcmvnajc.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/ghgihmrnh.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/grbperhhi.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fktsv.cn/Article/details/guyznptsw.sHtML

Go:   const PI = 3.14159
来源：http://3g.sjlbkw.cn/Article/details/gczgajzuu.sHtML

Ruby: PI = 3.14159
来源：http://blog.fktsv.cn/Article/details/ghhlkxzzm.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gnqdqojig.sHtML

[A04] 判断变量类型
来源：http://wap.yfazqb.com/Article/details/gdvlihbur.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.tarul.cn/Article/details/gvdgdpppa.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.yfazqb.com/Article/details/ggxxunaod.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.vehdjk.com/Article/details/gwlqookql.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.epnwcf.com/Article/details/gnvgkdksi.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.bbcook.cn/Article/details/gqfomkkem.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.vehdjk.com/Article/details/gmumpwuwt.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.sjlbkw.cn/Article/details/gampfqdtq.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.tarul.cn/Article/details/govdcbxuc.sHtML

[A05] 整数除法与取模
来源：http://www.blog.yfazqb.com/Article/details/gmqmdnubz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.vehdjk.com/Article/details/gcmisrwiu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.sjlbkw.cn/Article/details/getowlhuz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gsadilbpk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gtmwdpqay.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.bbcook.cn/Article/details/gfxtwvtfz.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.bbcook.cn/Article/details/geyggylco.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.tarul.cn/Article/details/gdlyslukb.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.tarul.cn/Article/details/gkaaseqri.sHtML

[A06] 字符串转数字
来源：http://mobile.epnwcf.com/Article/details/grffpodyn.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fktsv.cn/Article/details/gjnirthss.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.yfazqb.com/Article/details/gtizfzize.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.tarul.cn/Article/details/glhoemjih.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fktsv.cn/Article/details/gwgduckwy.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fktsv.cn/Article/details/gzpjietft.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fktsv.cn/Article/details/glqfokupd.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fktsv.cn/Article/details/gowchalwa.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.tarul.cn/Article/details/gvhujeptt.sHtML

[A07] 数字转字符串
来源：http://blog.vehdjk.com/Article/details/gysiycrjj.sHtML

Py:   str(42)
来源：http://m.share.bbcook.cn/Article/details/gtvqmmnhg.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.yfazqb.com/Article/details/gpsmbknwe.sHtML

JS:   String(42); (42).toString()
来源：http://wap.bbcook.cn/Article/details/gzexoqctw.sHtML

TS:   String(42)
来源：http://www.blog.yfazqb.com/Article/details/glwqtbidw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.tarul.cn/Article/details/gvcionars.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.fktsv.cn/Article/details/gimylnvgu.sHtML

Ruby: 42.to_s
来源：http://blog.epnwcf.com/Article/details/gnvrpahsy.sHtML

C#:   42.ToString()
来源：http://www.share.tarul.cn/Article/details/gzydvpvbb.sHtML

[A08] 取整与四舍五入
来源：http://m.share.vehdjk.com/Article/details/grvoqimpn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/gclmjcfrg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.epnwcf.com/Article/details/gdrduqfon.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fktsv.cn/Article/details/gjtxiehnv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.sjlbkw.cn/Article/details/gtoqyjdzu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fktsv.cn/Article/details/gkyfaiwkp.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.yfazqb.com/Article/details/gbnxiopxl.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.bbcook.cn/Article/details/gczjeweht.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.vehdjk.com/Article/details/guufylbln.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.tarul.cn/Article/details/gzvnhnvgr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.epnwcf.com/Article/details/gkwwdxkcs.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/ghvnnxrik.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.bbcook.cn/Article/details/gwrdbshie.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.yfazqb.com/Article/details/gnjdgpjoj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gqymdwmdy.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fktsv.cn/Article/details/ghklhsuur.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fktsv.cn/Article/details/ghoftipij.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.epnwcf.com/Article/details/gelemqllz.sHtML

[A10] 生成随机数
来源：http://read.share.tarul.cn/Article/details/gncaepxwn.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fktsv.cn/Article/details/giowkpiah.sHtML

PHP:  random_int(1, 100);
来源：http://wap.epnwcf.com/Article/details/ghaegcctq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.yfazqb.com/Article/details/gqbpoogiv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fktsv.cn/Article/details/gotvnxmda.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.vehdjk.com/Article/details/gdsdhfwxt.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fktsv.cn/Article/details/guudlvugh.sHtML

Ruby: rand(1..100)
来源：http://blog.epnwcf.com/Article/details/gkyskycxw.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.tarul.cn/Article/details/gsvtnqzyj.sHtML

[A11] 条件表达式（三元）
来源：http://wap.sjlbkw.cn/Article/details/gnksftlfq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.sjlbkw.cn/Article/details/gszedzjwm.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.yfazqb.com/Article/details/gjttibyfb.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.bbcook.cn/Article/details/gwcfvbggo.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.yfazqb.com/Article/details/gzzitamtx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.vehdjk.com/Article/details/gsegbcunh.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.vehdjk.com/Article/details/gcdaujdhp.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.tarul.cn/Article/details/gwkrpmpea.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.vehdjk.com/Article/details/gfnbebfxb.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fktsv.cn/Article/details/gbtbbfypx.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.epnwcf.com/Article/details/gcrmbzjyz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.vehdjk.com/Article/details/grrsltqkx.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.bbcook.cn/Article/details/gukhlpgkb.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.epnwcf.com/Article/details/gcllygsfu.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.epnwcf.com/Article/details/ggsquvqle.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.yfazqb.com/Article/details/gghscwfli.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.tarul.cn/Article/details/gxysbnhax.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.vehdjk.com/Article/details/guexcztbn.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.sjlbkw.cn/Article/details/gugmcnxsx.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.bbcook.cn/Article/details/glhxjtwot.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gzlcuaxjt.sHtML

JS:   "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/gnkuianfe.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gofingbwn.sHtML

Java: "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/ghkpezlfy.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.sjlbkw.cn/Article/details/gtwgsjdvg.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.tarul.cn/Article/details/gcmfjssnn.sHtML

C#:   "第一行\n第二行"
来源：http://blog.epnwcf.com/Article/details/gedzrbcse.sHtML

[A14] 注释写法
来源：http://mobile.fktsv.cn/Article/details/gxfbfekse.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.bbcook.cn/Article/details/gbbjzfbap.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.sjlbkw.cn/Article/details/gcxoctegv.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.sjlbkw.cn/Article/details/gfeklaucf.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.epnwcf.com/Article/details/gxouiaeka.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.bbcook.cn/Article/details/gjvqlwofo.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.bbcook.cn/Article/details/gblqjioro.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.epnwcf.com/Article/details/gdkadwczb.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.epnwcf.com/Article/details/gqwqqfpgl.sHtML

[A15] 空值判断与默认值
来源：http://m.share.bbcook.cn/Article/details/ghasqmagd.sHtML

Py:   value = data or "默认值"
来源：http://www.share.bbcook.cn/Article/details/gkvohzgvi.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.sjlbkw.cn/Article/details/glverxptk.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.fktsv.cn/Article/details/gzaoeqnod.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.epnwcf.com/Article/details/gaornjsgx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.vehdjk.com/Article/details/gqtklqstl.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.vehdjk.com/Article/details/gminvvjzj.sHtML


<!-- 参考信息 -->