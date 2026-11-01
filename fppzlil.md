代发 wailian999

[U99] JS：事件监听
来源：http://mobile.epnwcf.com/Article/details/gkkhngyth.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fktsv.cn/Article/details/gduxvxfeb.sHtML

[U100] JS：DOM 查询
来源：http://blog.epnwcf.com/Article/details/gljstwkge.sHtML

document.querySelector(".item")
来源：http://m.share.fktsv.cn/Article/details/gpswkwmnx.sHtML

[U101] JS：classList 操作
来源：http://m.share.fktsv.cn/Article/details/gfmityndb.sHtML

el.classList.toggle("active")
来源：http://www.m.share.yfazqb.com/Article/details/ggwvrdojx.sHtML

[U102] JS：本地存储
来源：http://3g.tarul.cn/Article/details/gchzpqwsx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.bbcook.cn/Article/details/gsrddtoxz.sHtML

[U103] JS：定时器
来源：http://m.share.epnwcf.com/Article/details/gevwojcml.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.tarul.cn/Article/details/gwgumxuqr.sHtML

[U104] JS：防抖
来源：http://blog.bbcook.cn/Article/details/gajbipmyp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/ghskxfjpm.sHtML

[U105] JS：节流
来源：http://www.share.tarul.cn/Article/details/gxigrdthr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.epnwcf.com/Article/details/gehpcszac.sHtML

[U106] JS：日期格式化
来源：http://read.share.tarul.cn/Article/details/gehefdeln.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.tarul.cn/Article/details/gtccgjfcz.sHtML

[U107] JS：数字千分位
来源：http://blog.bbcook.cn/Article/details/gwmnqduxq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.bbcook.cn/Article/details/gtlxqozyt.sHtML

[U108] JS：随机整数
来源：http://blog.epnwcf.com/Article/details/gmpycmluy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.epnwcf.com/Article/details/gghwtgtkw.sHtML

[U109] JS：数组分组
来源：http://mobile.bbcook.cn/Article/details/gqyrxeibg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.vehdjk.com/Article/details/gzrlfwfjn.sHtML

[U110] JS：数组分块
来源：http://wap.vehdjk.com/Article/details/gigjncfdw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.epnwcf.com/Article/details/gwafutqpm.sHtML

[U111] JS：对象转 Map
来源：http://mobile.sjlbkw.cn/Article/details/ggnqfwrih.sHtML

new Map(Object.entries(obj))
来源：http://www.share.sjlbkw.cn/Article/details/guwpqbeld.sHtML

[U112] JS：字符串补位
来源：http://www.share.bbcook.cn/Article/details/gnlbnpusp.sHtML

"7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gtzatoiqk.sHtML

[U113] JS：正则替换全部
来源：http://blog.bbcook.cn/Article/details/gohpvnwgk.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gnugfmctr.sHtML

[U114] JS：JSON 深比较
来源：http://blog.bbcook.cn/Article/details/gqrxillgb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.tarul.cn/Article/details/gzppzxemj.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.bbcook.cn/Article/details/gcwcdngdx.sHtML

crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/gldjomoek.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fktsv.cn/Article/details/gdgwvxsng.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fktsv.cn/Article/details/gdvtwzbps.sHtML

[U117] JS：单元测试
来源：http://www.m.share.tarul.cn/Article/details/gseiahznl.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.yfazqb.com/Article/details/gqpmsxvwl.sHtML

[U118] JS：开发服务器
来源：http://read.share.vehdjk.com/Article/details/gzyyvavpn.sHtML

npm i -D vite;  npx vite
来源：http://3g.fktsv.cn/Article/details/gwruxujrx.sHtML

[U119] JS：生产构建
来源：http://3g.tarul.cn/Article/details/gmjhkxdaf.sHtML

npx vite build
来源：http://baike.bbcook.cn/Article/details/gnzljlrqa.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.vehdjk.com/Article/details/gtthckbsn.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.tarul.cn/Article/details/grfemmnxa.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gaogchcpv.sHtML

统计汇总
来源：http://mobile.tarul.cn/Article/details/ghguzebnf.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gdcduaffd.sHtML

按语言统计（条）：
来源：http://www.share.epnwcf.com/Article/details/gotwmsyol.sHtML

Python ......... 252
来源：http://m.share.epnwcf.com/Article/details/ggzkipqwu.sHtML

PHP ............ 252
来源：http://baike.vehdjk.com/Article/details/gzamlwybx.sHtML

JavaScript ..... 252
来源：http://blog.epnwcf.com/Article/details/geacdsprf.sHtML

TypeScript ..... 212
来源：http://mobile.yfazqb.com/Article/details/govtbhjbb.sHtML

Java ........... 212
来源：http://3g.yfazqb.com/Article/details/gmdniuzwr.sHtML

Go ............. 212
来源：http://3g.fktsv.cn/Article/details/glmsustix.sHtML

Ruby ........... 212
来源：http://mobile.yfazqb.com/Article/details/gdqsjckqh.sHtML

C# ............. 212
来源：http://www.m.share.fktsv.cn/Article/details/gzljmyrvm.sHtML

C .............. 30
来源：http://baike.vehdjk.com/Article/details/goyppbuac.sHtML

C++ ............ 30
来源：http://read.share.sjlbkw.cn/Article/details/gbbzljqun.sHtML

SQL ............ 90
来源：http://read.share.bbcook.cn/Article/details/girfvnlur.sHtML

Bash ........... 80
来源：http://mobile.vehdjk.com/Article/details/gouttmqyx.sHtML

Kotlin ......... 15
来源：http://m.share.epnwcf.com/Article/details/gqxpnwxnq.sHtML

Swift .......... 15
来源：http://3g.epnwcf.com/Article/details/gybcvasao.sHtML

Lua ............ 10
来源：http://m.share.fktsv.cn/Article/details/guzbupawg.sHtML

Perl ........... 10
来源：http://www.share.sjlbkw.cn/Article/details/gjsngwwzo.sHtML

Scala .......... 10
来源：http://www.share.bbcook.cn/Article/details/gnruqkmdy.sHtML

------------------------------------
来源：http://baike.bbcook.cn/Article/details/gbpqhikma.sHtML

合计 ........... 2106 条
来源：http://read.share.fktsv.cn/Article/details/giyiisxuf.sHtML

按章节统计：
来源：http://m.share.yfazqb.com/Article/details/gzwoonrrm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.vehdjk.com/Article/details/gvaqiiqwh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.bbcook.cn/Article/details/gpnneqxwg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.vehdjk.com/Article/details/gftawgyav.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fktsv.cn/Article/details/ghgbxoovo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.tarul.cn/Article/details/gnokmfmyv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.vehdjk.com/Article/details/giejejzax.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.sjlbkw.cn/Article/details/ghxviajcx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.epnwcf.com/Article/details/gkqwqcukx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/ghakrpbbn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.sjlbkw.cn/Article/details/gfovdlmrb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/gqplyfhnj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/gjvvexlle.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/gkeizodxx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.tarul.cn/Article/details/ggskjghlu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.epnwcf.com/Article/details/gapvomepn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.tarul.cn/Article/details/gylqmjucc.sHtML

Q SQL 专题                              90
来源：http://mobile.fktsv.cn/Article/details/gvsosmhye.sHtML

R Bash 专题                             80
来源：http://m.share.bbcook.cn/Article/details/gbkcupmty.sHtML

S C / C++ 专题                          60
来源：http://m.share.sjlbkw.cn/Article/details/gegfnwvbt.sHtML

T 其他语言补充                          60
来源：http://baike.vehdjk.com/Article/details/gmxirbijs.sHtML

U 高频实用片段                         120
来源：http://www.m.share.tarul.cn/Article/details/gmfnmbyvk.sHtML

------------------------------------
来源：http://3g.epnwcf.com/Article/details/gkabugddz.sHtML

合计                                  2106 条
来源：http://www.blog.bbcook.cn/Article/details/gtaxicime.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gxsmrumqs.sHtML

使用提醒
来源：http://baike.fktsv.cn/Article/details/gaottvksv.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fktsv.cn/Article/details/gzwuyypkl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.bbcook.cn/Article/details/grxipiqfa.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.epnwcf.com/Article/details/gcdckllmb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.yfazqb.com/Article/details/gooktfzyf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.sjlbkw.cn/Article/details/grlkzothp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.tarul.cn/Article/details/gvuadfaxv.sHtML

—— 文件结束 ——
来源：http://m.share.vehdjk.com/Article/details/gxzyujmkc.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gvzadhnxg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.vehdjk.com/Article/details/gehuavjhp.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.epnwcf.com/Article/details/gvpfxbnwe.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gdezxjsnl.sHtML

【收录内容】
来源：http://m.share.tarul.cn/Article/details/ghzqgxhzn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.vehdjk.com/Article/details/guxomuwur.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.sjlbkw.cn/Article/details/gjgkvkhwp.sHtML

SQL · Bash · C · C++
来源：http://read.share.epnwcf.com/Article/details/gonttvfha.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.tarul.cn/Article/details/gajccurlp.sHtML

【使用说明】
来源：http://3g.yfazqb.com/Article/details/gjskuflee.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.tarul.cn/Article/details/gjxdegwfy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.bbcook.cn/Article/details/gvtrngzbk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.epnwcf.com/Article/details/guprjlsxp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.bbcook.cn/Article/details/gpbinyfth.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.sjlbkw.cn/Article/details/ghuaozpsv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.bbcook.cn/Article/details/ghddxjdvl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.vehdjk.com/Article/details/gbmywxuir.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.yfazqb.com/Article/details/gpnctqsri.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.bbcook.cn/Article/details/gtqxcomco.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.tarul.cn/Article/details/gocxyxdlh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.vehdjk.com/Article/details/gnnihrneo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.vehdjk.com/Article/details/gbviwgdnq.sHtML

【文件统计】
来源：http://3g.epnwcf.com/Article/details/gvhvaymtl.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.tarul.cn/Article/details/guxjuuvbx.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/gwdgeasls.sHtML

目  录
来源：http://www.blog.fktsv.cn/Article/details/gtpvxdlyo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/gmhtbfwym.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.tarul.cn/Article/details/gqezbzmwb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.bbcook.cn/Article/details/gcqdhifcs.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.sjlbkw.cn/Article/details/gauaippww.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.yfazqb.com/Article/details/ghvwlfeqe.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fktsv.cn/Article/details/ghnsnwsgh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.sjlbkw.cn/Article/details/gbinvdour.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/gpqrztjkp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fktsv.cn/Article/details/gszzmvidt.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.tarul.cn/Article/details/gwwgumywg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.bbcook.cn/Article/details/goibskbjo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.yfazqb.com/Article/details/grqccikqp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/gqgjxjdcl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.yfazqb.com/Article/details/gvipubnde.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gtnmxkfim.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.epnwcf.com/Article/details/gmswuxcpu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/getjhwvuq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.vehdjk.com/Article/details/gkzgdjkpb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.epnwcf.com/Article/details/ghyauthch.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fktsv.cn/Article/details/ggfuqdyjx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.sjlbkw.cn/Article/details/gbdjzdadu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.bbcook.cn/Article/details/gmhwtvjlz.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gzvjbaeoc.sHtML

A. 基础语法与类型
来源：http://wap.sjlbkw.cn/Article/details/gznzqtysl.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gefiosfil.sHtML

[A01] Hello World
来源：http://read.share.sjlbkw.cn/Article/details/ghqaaqbtt.sHtML

Py:   print("Hello, World!")
来源：http://baike.fktsv.cn/Article/details/gifavchim.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.yfazqb.com/Article/details/gwbjpsixa.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.yfazqb.com/Article/details/gebyqdrkj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fktsv.cn/Article/details/gfqaogifk.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fktsv.cn/Article/details/gazaaltgm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fktsv.cn/Article/details/gkgfcbtob.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.epnwcf.com/Article/details/gdwhblrcs.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.tarul.cn/Article/details/gqnymosyo.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.bbcook.cn/Article/details/goaxseghx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.yfazqb.com/Article/details/gfuikribt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.tarul.cn/Article/details/gsansubnx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.epnwcf.com/Article/details/gjrznxbcd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrzsfgvm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.epnwcf.com/Article/details/gszgzvybk.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.tarul.cn/Article/details/gtyoqrvii.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.sjlbkw.cn/Article/details/gwrfazknq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.bbcook.cn/Article/details/gsxrttkbv.sHtML

[A03] 常量定义
来源：http://read.share.vehdjk.com/Article/details/gbwkwwlaj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.tarul.cn/Article/details/gjusswqrp.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gkaxsclgy.sHtML

JS:   const PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gxoeyxtjf.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/goeohjecd.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/glxerkyzw.sHtML

Go:   const PI = 3.14159
来源：http://wap.tarul.cn/Article/details/gmcujqgxb.sHtML

Ruby: PI = 3.14159
来源：http://m.share.yfazqb.com/Article/details/gavuntgts.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gmpvworpa.sHtML

[A04] 判断变量类型
来源：http://wap.bbcook.cn/Article/details/guwfucdkl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.vehdjk.com/Article/details/gxthtkzly.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.epnwcf.com/Article/details/gaohjjqea.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.epnwcf.com/Article/details/gavwihten.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fktsv.cn/Article/details/gjxqejwtm.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.tarul.cn/Article/details/geisffjkz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.vehdjk.com/Article/details/grsblusna.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.tarul.cn/Article/details/gsxohkdgw.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.sjlbkw.cn/Article/details/ghsgdyxky.sHtML

[A05] 整数除法与取模
来源：http://blog.bbcook.cn/Article/details/gglhfppqq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.yfazqb.com/Article/details/gjxjgbmaj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.epnwcf.com/Article/details/gxngunirg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gosoflhgw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.yfazqb.com/Article/details/gspjyttyc.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.vehdjk.com/Article/details/gnxbcupcg.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.vehdjk.com/Article/details/gbnjfwzzt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.tarul.cn/Article/details/gsloapglz.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fktsv.cn/Article/details/gowqicnnw.sHtML

[A06] 字符串转数字
来源：http://3g.yfazqb.com/Article/details/gpmehbeht.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fktsv.cn/Article/details/gmrbredlo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.sjlbkw.cn/Article/details/gmounaxzt.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.bbcook.cn/Article/details/gkskytjcg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.bbcook.cn/Article/details/gefeplszb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.tarul.cn/Article/details/goympbkbq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.tarul.cn/Article/details/ghanpkxps.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.bbcook.cn/Article/details/gooshscgq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.yfazqb.com/Article/details/gzviuzoak.sHtML

[A07] 数字转字符串
来源：http://www.blog.fktsv.cn/Article/details/gxhvnzlwb.sHtML

Py:   str(42)
来源：http://read.share.vehdjk.com/Article/details/gykjnjgfw.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.bbcook.cn/Article/details/gcikonuhx.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.epnwcf.com/Article/details/gpkjidgxg.sHtML

TS:   String(42)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqdneipp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.bbcook.cn/Article/details/galoqdkii.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fktsv.cn/Article/details/gjxlgzbpn.sHtML

Ruby: 42.to_s
来源：http://read.share.tarul.cn/Article/details/gxyurrtki.sHtML

C#:   42.ToString()
来源：http://wap.bbcook.cn/Article/details/gubmtyvoc.sHtML

[A08] 取整与四舍五入
来源：http://blog.tarul.cn/Article/details/gxqdpyrqj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.vehdjk.com/Article/details/gbaeebohk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.sjlbkw.cn/Article/details/gnhgkeamt.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.tarul.cn/Article/details/giwolfqkp.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.yfazqb.com/Article/details/gdpruwofz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/gcacdjhjo.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.yfazqb.com/Article/details/glsuzeaek.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fktsv.cn/Article/details/gjfmpaakw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.tarul.cn/Article/details/gcevwmqju.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.bbcook.cn/Article/details/ginhovbmt.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gcoaoffdh.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fktsv.cn/Article/details/gidxjigua.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gbubbclkz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gukdwanjl.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gykcyfffb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.tarul.cn/Article/details/gldinusos.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.yfazqb.com/Article/details/grubgfrrp.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.vehdjk.com/Article/details/gepneuvtk.sHtML

[A10] 生成随机数
来源：http://www.m.share.vehdjk.com/Article/details/gjvmonyfk.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.vehdjk.com/Article/details/gmropmjif.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.yfazqb.com/Article/details/gulymqawi.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.sjlbkw.cn/Article/details/gqgfhkbhl.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fktsv.cn/Article/details/gimhmhgmo.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.vehdjk.com/Article/details/gszccjeuz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.bbcook.cn/Article/details/gtpufjxos.sHtML

Ruby: rand(1..100)
来源：http://baike.tarul.cn/Article/details/gbrotnsbd.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.tarul.cn/Article/details/gufmquhos.sHtML

[A11] 条件表达式（三元）
来源：http://3g.yfazqb.com/Article/details/gvluzuhwd.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.sjlbkw.cn/Article/details/gvuvrwwdk.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.tarul.cn/Article/details/gwghcwwju.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.vehdjk.com/Article/details/ghvtfwjjf.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.tarul.cn/Article/details/gjmebrwld.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.sjlbkw.cn/Article/details/gesfpyors.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.sjlbkw.cn/Article/details/gzjylkjaa.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.epnwcf.com/Article/details/gnvmakoil.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.tarul.cn/Article/details/gdxwreyyu.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fktsv.cn/Article/details/gzqjlnrxz.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.vehdjk.com/Article/details/guqbtiryy.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fktsv.cn/Article/details/glfmsqcoo.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.bbcook.cn/Article/details/gbmagmofm.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.bbcook.cn/Article/details/gskkzlrug.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.tarul.cn/Article/details/gdtqhzvxt.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.epnwcf.com/Article/details/gimwqvmdw.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.epnwcf.com/Article/details/gnwiigkwa.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.bbcook.cn/Article/details/gpjjjjqaa.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fktsv.cn/Article/details/guhpdiqzi.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/gjoomvyel.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.yfazqb.com/Article/details/gamepfunx.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/gzhxxvtbb.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/gtrjlnxjj.sHtML

Java: "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gnmnfvtrd.sHtML

Go:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gjzbaxnsj.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/gghjnxjwv.sHtML

C#:   "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gmfyzsvsz.sHtML

[A14] 注释写法
来源：http://www.blog.tarul.cn/Article/details/gvipljcjy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.sjlbkw.cn/Article/details/gcppqewjl.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fktsv.cn/Article/details/glujzphsa.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.epnwcf.com/Article/details/gicnlmgdx.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.sjlbkw.cn/Article/details/gmzsmvoug.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.sjlbkw.cn/Article/details/gkgeousff.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.bbcook.cn/Article/details/gthasqkfc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.tarul.cn/Article/details/gyqjuijgl.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fktsv.cn/Article/details/gljnposrz.sHtML

[A15] 空值判断与默认值
来源：http://mobile.fktsv.cn/Article/details/gukyfyqzj.sHtML

Py:   value = data or "默认值"
来源：http://mobile.epnwcf.com/Article/details/glsbyetek.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.epnwcf.com/Article/details/gewkdtyjo.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.bbcook.cn/Article/details/gjadukjdb.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.vehdjk.com/Article/details/govpsarka.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.sjlbkw.cn/Article/details/gkozynkon.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.vehdjk.com/Article/details/gnohagbbx.sHtML

Ruby: value = data || "默认值"
来源：http://3g.sjlbkw.cn/Article/details/gmajgqlzi.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.epnwcf.com/Article/details/gvzunolrm.sHtML

[A16] 真假值判断规则
来源：http://mobile.fktsv.cn/Article/details/gguhbados.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.epnwcf.com/Article/details/gcfibfadd.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.bbcook.cn/Article/details/gbptlkyox.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.epnwcf.com/Article/details/gmsqvdcek.sHtML

TS:   if (!x) {}
来源：http://wap.vehdjk.com/Article/details/grjempnrt.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.yfazqb.com/Article/details/gyqwkunjw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.sjlbkw.cn/Article/details/gvmwsljcb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.tarul.cn/Article/details/gtvjrxksb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.vehdjk.com/Article/details/gmwqmtvmt.sHtML

[A17] 位运算
来源：http://blog.sjlbkw.cn/Article/details/gnekphjvq.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/gqsvovaio.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.vehdjk.com/Article/details/gctsoqnfq.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/glqlwaozb.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/gnmjhibvt.sHtML


<!-- 参考信息 -->