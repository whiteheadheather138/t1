代发 wailian999

[U95] JS：Promise 包装
来源：http://www.blog.fktsv.cn/Article/details/glqkutrrs.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fktsv.cn/Article/details/gdnktbcfb.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.vehdjk.com/Article/details/gzivavsbh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gprhkomke.sHtML

[U97] JS：并发请求
来源：http://baike.epnwcf.com/Article/details/gprrwwssw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/guietviao.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.vehdjk.com/Article/details/gxmkefpoe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.tarul.cn/Article/details/gfyvxiona.sHtML

[U99] JS：事件监听
来源：http://m.share.tarul.cn/Article/details/guloognbi.sHtML

el.addEventListener("click", e => {})
来源：http://wap.tarul.cn/Article/details/gksmmwrba.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fktsv.cn/Article/details/gjkrjqsnf.sHtML

document.querySelector(".item")
来源：http://wap.bbcook.cn/Article/details/gbsjhfwke.sHtML

[U101] JS：classList 操作
来源：http://baike.yfazqb.com/Article/details/gudxlovwi.sHtML

el.classList.toggle("active")
来源：http://3g.fktsv.cn/Article/details/givixvekp.sHtML

[U102] JS：本地存储
来源：http://www.blog.vehdjk.com/Article/details/gzitopvdp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fktsv.cn/Article/details/ghfuzqpfa.sHtML

[U103] JS：定时器
来源：http://wap.yfazqb.com/Article/details/gqfasiyyn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fktsv.cn/Article/details/gbxuxjibj.sHtML

[U104] JS：防抖
来源：http://mobile.sjlbkw.cn/Article/details/gkhxcqkwd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.vehdjk.com/Article/details/grlodmgdd.sHtML

[U105] JS：节流
来源：http://3g.fktsv.cn/Article/details/gmfpkupvp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gqlcbnwlo.sHtML

[U106] JS：日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gzujvaypo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fktsv.cn/Article/details/gojjslumn.sHtML

[U107] JS：数字千分位
来源：http://www.share.vehdjk.com/Article/details/gzwnzihwr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.tarul.cn/Article/details/ghxxvbgrg.sHtML

[U108] JS：随机整数
来源：http://m.share.yfazqb.com/Article/details/gtkkecrmk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.sjlbkw.cn/Article/details/gchnjulxb.sHtML

[U109] JS：数组分组
来源：http://www.m.share.vehdjk.com/Article/details/gxbfzzisc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.yfazqb.com/Article/details/guvetbxar.sHtML

[U110] JS：数组分块
来源：http://baike.vehdjk.com/Article/details/gsehvvhcf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.tarul.cn/Article/details/gsdlwoixz.sHtML

[U111] JS：对象转 Map
来源：http://mobile.sjlbkw.cn/Article/details/gtfqwafdr.sHtML

new Map(Object.entries(obj))
来源：http://mobile.tarul.cn/Article/details/grozzgdxn.sHtML

[U112] JS：字符串补位
来源：http://blog.epnwcf.com/Article/details/gzaghddeo.sHtML

"7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/gnesyjdhe.sHtML

[U113] JS：正则替换全部
来源：http://baike.yfazqb.com/Article/details/gheuzzles.sHtML

s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gntjfepal.sHtML

[U114] JS：JSON 深比较
来源：http://baike.tarul.cn/Article/details/gexxuryyu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fktsv.cn/Article/details/gqiqkjypg.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fktsv.cn/Article/details/gswlecbvj.sHtML

crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gqzemtyrq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.vehdjk.com/Article/details/gnnrxldwf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.vehdjk.com/Article/details/gzsfwoego.sHtML

[U117] JS：单元测试
来源：http://m.share.yfazqb.com/Article/details/glutotvgf.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fktsv.cn/Article/details/gisbxwvcm.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fktsv.cn/Article/details/gesdxkqbx.sHtML

npm i -D vite;  npx vite
来源：http://wap.vehdjk.com/Article/details/godlffvyi.sHtML

[U119] JS：生产构建
来源：http://m.share.sjlbkw.cn/Article/details/gmqpiarrp.sHtML

npx vite build
来源：http://3g.fktsv.cn/Article/details/gupjhvkja.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fktsv.cn/Article/details/gocrgwspk.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.sjlbkw.cn/Article/details/gwohkcmon.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gnjxdhmso.sHtML

统计汇总
来源：http://www.blog.epnwcf.com/Article/details/grypnizlo.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gebaqlpcp.sHtML

按语言统计（条）：
来源：http://3g.sjlbkw.cn/Article/details/genmkfoen.sHtML

Python ......... 252
来源：http://www.share.yfazqb.com/Article/details/gxzspvmme.sHtML

PHP ............ 252
来源：http://read.share.bbcook.cn/Article/details/gkcovkjni.sHtML

JavaScript ..... 252
来源：http://www.m.share.sjlbkw.cn/Article/details/gnoafgoir.sHtML

TypeScript ..... 212
来源：http://mobile.vehdjk.com/Article/details/gzlrdfrgr.sHtML

Java ........... 212
来源：http://www.share.tarul.cn/Article/details/gmgwhqdxh.sHtML

Go ............. 212
来源：http://read.share.yfazqb.com/Article/details/gylhtjlvq.sHtML

Ruby ........... 212
来源：http://www.share.sjlbkw.cn/Article/details/givtutyrf.sHtML

C# ............. 212
来源：http://www.blog.yfazqb.com/Article/details/gqnrplynm.sHtML

C .............. 30
来源：http://www.m.share.sjlbkw.cn/Article/details/gkehfactb.sHtML

C++ ............ 30
来源：http://www.blog.yfazqb.com/Article/details/ghdlxties.sHtML

SQL ............ 90
来源：http://wap.fktsv.cn/Article/details/gssoxszrc.sHtML

Bash ........... 80
来源：http://www.share.fktsv.cn/Article/details/gjmutzpov.sHtML

Kotlin ......... 15
来源：http://3g.vehdjk.com/Article/details/gowpcglrp.sHtML

Swift .......... 15
来源：http://read.share.fktsv.cn/Article/details/gppvuyzbd.sHtML

Lua ............ 10
来源：http://blog.sjlbkw.cn/Article/details/gxojpcpcv.sHtML

Perl ........... 10
来源：http://m.share.fktsv.cn/Article/details/goyudnaqz.sHtML

Scala .......... 10
来源：http://m.share.bbcook.cn/Article/details/gjkzioykm.sHtML

------------------------------------
来源：http://baike.epnwcf.com/Article/details/gfunrzqda.sHtML

合计 ........... 2106 条
来源：http://3g.vehdjk.com/Article/details/gpesxrxhl.sHtML

按章节统计：
来源：http://read.share.epnwcf.com/Article/details/gqtygjbwt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.tarul.cn/Article/details/gcbggfrki.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.sjlbkw.cn/Article/details/glylylojo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.bbcook.cn/Article/details/gwfrjgvsc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.epnwcf.com/Article/details/gypnwkjba.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.tarul.cn/Article/details/garfajowx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.bbcook.cn/Article/details/ganosxfcl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.bbcook.cn/Article/details/glntdqqje.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.yfazqb.com/Article/details/gznjfvzwb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gsbziadsp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fktsv.cn/Article/details/gpanbjkxn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/guobhykqc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gtmbxcprn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/ghtwtdjlz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.vehdjk.com/Article/details/gocbpoghf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fktsv.cn/Article/details/gsktvuosa.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gzfmqgtej.sHtML

Q SQL 专题                              90
来源：http://wap.fktsv.cn/Article/details/grpeapqzl.sHtML

R Bash 专题                             80
来源：http://www.share.tarul.cn/Article/details/geoveqqgg.sHtML

S C / C++ 专题                          60
来源：http://baike.epnwcf.com/Article/details/gottbpvcg.sHtML

T 其他语言补充                          60
来源：http://www.share.tarul.cn/Article/details/gpcvdafjj.sHtML

U 高频实用片段                         120
来源：http://blog.bbcook.cn/Article/details/gvfgldbhb.sHtML

------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gziifmtex.sHtML

合计                                  2106 条
来源：http://wap.bbcook.cn/Article/details/gvqgjfzlw.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gvwymlqse.sHtML

使用提醒
来源：http://www.share.yfazqb.com/Article/details/ghznvfuhg.sHtML

--------------------------------------------------------------------------------
来源：http://3g.yfazqb.com/Article/details/gikkkjzpe.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.yfazqb.com/Article/details/ghlhooxah.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fktsv.cn/Article/details/gaiehqzot.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.vehdjk.com/Article/details/geambughp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.epnwcf.com/Article/details/gzjfdqjci.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.bbcook.cn/Article/details/gjvptmtgg.sHtML

—— 文件结束 ——
来源：http://m.share.sjlbkw.cn/Article/details/gzptrxzii.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gitiknsfi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.bbcook.cn/Article/details/gzsqtrutg.sHtML

Common Programming Examples Cheat Book
来源：http://3g.epnwcf.com/Article/details/gtimuiaxv.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gzdzykxev.sHtML

【收录内容】
来源：http://www.blog.tarul.cn/Article/details/gvpduedhf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.epnwcf.com/Article/details/gsxihwbrk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.bbcook.cn/Article/details/gaxmkulrj.sHtML

SQL · Bash · C · C++
来源：http://mobile.bbcook.cn/Article/details/gdwiajyfp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.bbcook.cn/Article/details/gaycvsaqx.sHtML

【使用说明】
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdhnksro.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.bbcook.cn/Article/details/gvnjbxegt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.sjlbkw.cn/Article/details/gdkcjktqp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.bbcook.cn/Article/details/gqucjecyo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fktsv.cn/Article/details/gjvzbxslt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.vehdjk.com/Article/details/gndxoevna.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.yfazqb.com/Article/details/gvlsmkmuj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.sjlbkw.cn/Article/details/gthqqzwpn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fktsv.cn/Article/details/gyoljwwnq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fktsv.cn/Article/details/gvcutzefj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.tarul.cn/Article/details/gzvgdhyrm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.sjlbkw.cn/Article/details/gtieiumcb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fktsv.cn/Article/details/grbjulanc.sHtML

【文件统计】
来源：http://www.blog.yfazqb.com/Article/details/ghaklfhqf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.vehdjk.com/Article/details/gnaxdggrg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gclwnyusl.sHtML

目  录
来源：http://m.share.yfazqb.com/Article/details/gaagmswjy.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gqonftvjn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.bbcook.cn/Article/details/ghowufgqb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.tarul.cn/Article/details/gbsvtiira.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.yfazqb.com/Article/details/gbhetbivu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.vehdjk.com/Article/details/gxmcprqtj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.bbcook.cn/Article/details/gfdvbszav.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.yfazqb.com/Article/details/gyhzdoqbm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.tarul.cn/Article/details/gxaanumzl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.epnwcf.com/Article/details/gzrkmrgwv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.sjlbkw.cn/Article/details/ggqzeicxc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fktsv.cn/Article/details/gtwfdvfpx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/glkxtwele.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gnighsiyt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.tarul.cn/Article/details/gkrrqovqi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.epnwcf.com/Article/details/goqrcavvt.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.sjlbkw.cn/Article/details/ghuuuxtbc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/gewbludit.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.bbcook.cn/Article/details/gvjgihpzd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.sjlbkw.cn/Article/details/gglcbmenh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.bbcook.cn/Article/details/gsexponew.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.sjlbkw.cn/Article/details/gxkhwcxik.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.yfazqb.com/Article/details/gpbrezzjo.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gndswihgi.sHtML

A. 基础语法与类型
来源：http://www.m.share.yfazqb.com/Article/details/gfoohgtzs.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gafhrlxkm.sHtML

[A01] Hello World
来源：http://3g.fktsv.cn/Article/details/gtqoiuvmi.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.sjlbkw.cn/Article/details/gaiffoqxo.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.yfazqb.com/Article/details/geiunifxa.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.vehdjk.com/Article/details/ghrzgwlje.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.yfazqb.com/Article/details/gqnvejrgw.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.sjlbkw.cn/Article/details/gviwmywbd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggicstoye.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.bbcook.cn/Article/details/gznotephu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.vehdjk.com/Article/details/gxgaffobv.sHtML

[A02] 变量声明与赋值
来源：http://3g.tarul.cn/Article/details/gdmhczemz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fktsv.cn/Article/details/gwpjmzomd.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.yfazqb.com/Article/details/gyuizqyuc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.yfazqb.com/Article/details/gvzobikys.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.tarul.cn/Article/details/gszzinwcx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.sjlbkw.cn/Article/details/gibvqyqxx.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.epnwcf.com/Article/details/gaaassrhs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.yfazqb.com/Article/details/gbbeuppqn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.vehdjk.com/Article/details/grjbqdzka.sHtML

[A03] 常量定义
来源：http://wap.sjlbkw.cn/Article/details/gwqqkoyvq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.epnwcf.com/Article/details/gadpetixe.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gtedfbobr.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gabczrhhv.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gqseotlzz.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/givedhgtb.sHtML

Go:   const PI = 3.14159
来源：http://mobile.yfazqb.com/Article/details/gxyzncjpi.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.sjlbkw.cn/Article/details/gabdqdbdc.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gegwwsexk.sHtML

[A04] 判断变量类型
来源：http://blog.tarul.cn/Article/details/galcusaur.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fktsv.cn/Article/details/gqrwsuivf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.tarul.cn/Article/details/gnptaglvn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.epnwcf.com/Article/details/gmcxcjsuh.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.tarul.cn/Article/details/ggxukxcke.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fktsv.cn/Article/details/gkowihelf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.epnwcf.com/Article/details/ghzcfdmyw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.tarul.cn/Article/details/gxazlxtty.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.vehdjk.com/Article/details/gkwlxtopg.sHtML

[A05] 整数除法与取模
来源：http://mobile.yfazqb.com/Article/details/gyjvjvvmi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fktsv.cn/Article/details/ggxplbwfd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.sjlbkw.cn/Article/details/gmjyfrzxs.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.yfazqb.com/Article/details/ggjxrdvge.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/gwgbjpkoo.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.vehdjk.com/Article/details/gohwttwbo.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gtivqkako.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.yfazqb.com/Article/details/gvdwebput.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gbpcmtnxp.sHtML

[A06] 字符串转数字
来源：http://3g.yfazqb.com/Article/details/glvnzgulh.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.vehdjk.com/Article/details/gdbazhrhk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fktsv.cn/Article/details/gsifixxre.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.epnwcf.com/Article/details/gyquejrqm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.epnwcf.com/Article/details/ggcynpnry.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fktsv.cn/Article/details/glcbbirqg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.sjlbkw.cn/Article/details/glpeossqv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.sjlbkw.cn/Article/details/ghhkwtmiv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fktsv.cn/Article/details/gpfbeznyy.sHtML

[A07] 数字转字符串
来源：http://www.share.tarul.cn/Article/details/ghvdkuzbn.sHtML

Py:   str(42)
来源：http://m.share.tarul.cn/Article/details/ghcnzcfqa.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.tarul.cn/Article/details/gykbvdtwi.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.vehdjk.com/Article/details/gptoaufxz.sHtML

TS:   String(42)
来源：http://www.m.share.tarul.cn/Article/details/gihqzexub.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fktsv.cn/Article/details/gkcmnedtz.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.tarul.cn/Article/details/gngedpejc.sHtML

Ruby: 42.to_s
来源：http://wap.yfazqb.com/Article/details/gmbqtvfmc.sHtML

C#:   42.ToString()
来源：http://mobile.sjlbkw.cn/Article/details/gszxltqkv.sHtML

[A08] 取整与四舍五入
来源：http://blog.tarul.cn/Article/details/gnvkfonxz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fktsv.cn/Article/details/gtvzlwtor.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.vehdjk.com/Article/details/gxrormfoq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/gcwmzjxrq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.tarul.cn/Article/details/gkkjuqoqt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.tarul.cn/Article/details/ggrreqlzb.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.epnwcf.com/Article/details/gxauqtvzs.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.yfazqb.com/Article/details/gzakwbyii.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.vehdjk.com/Article/details/gfomtdbjp.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.sjlbkw.cn/Article/details/gxxoorqly.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gdzdhghco.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.yfazqb.com/Article/details/gnnofqlwf.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.vehdjk.com/Article/details/gmcowlsvm.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fktsv.cn/Article/details/gplrzcxve.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/gtnbluanm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.vehdjk.com/Article/details/gbmzprmlg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.sjlbkw.cn/Article/details/gvkngygtn.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.epnwcf.com/Article/details/gwmwnuahf.sHtML

[A10] 生成随机数
来源：http://3g.yfazqb.com/Article/details/gyvsigxsk.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.sjlbkw.cn/Article/details/ghdfsdvpx.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.tarul.cn/Article/details/gjtsvpxyk.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fktsv.cn/Article/details/ghhpguics.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.tarul.cn/Article/details/guvifatpm.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.tarul.cn/Article/details/gpmaupgov.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.yfazqb.com/Article/details/grqgltjdk.sHtML

Ruby: rand(1..100)
来源：http://m.share.epnwcf.com/Article/details/gadlyeteg.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.bbcook.cn/Article/details/gccitonnw.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.fktsv.cn/Article/details/gfecefoxa.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.vehdjk.com/Article/details/gkxjymzbo.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.tarul.cn/Article/details/gnhhucfez.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.epnwcf.com/Article/details/glafweqhm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/gycutlcmj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.vehdjk.com/Article/details/gqmqcnvac.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.sjlbkw.cn/Article/details/gwfxkxfyv.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.sjlbkw.cn/Article/details/gwruznsql.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fktsv.cn/Article/details/gzlcevlmo.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.tarul.cn/Article/details/gvjdsbohs.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.vehdjk.com/Article/details/gzssjxzrd.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.yfazqb.com/Article/details/goqxmgyaw.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.bbcook.cn/Article/details/gvxsngnwj.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.epnwcf.com/Article/details/gvxwdhonk.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.yfazqb.com/Article/details/gmozrvrni.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fktsv.cn/Article/details/gyxsfixyt.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.fktsv.cn/Article/details/gwjhurypd.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.tarul.cn/Article/details/gevawmjwt.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.vehdjk.com/Article/details/gzxvpwduz.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/gqreekjix.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/gljytpnlu.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/gxnpvzlkf.sHtML

TS:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gaeojrqjb.sHtML

Java: "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/grwkstchp.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.vehdjk.com/Article/details/gmbgyustr.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gjitysqdt.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/geaalzkhp.sHtML

[A14] 注释写法
来源：http://wap.epnwcf.com/Article/details/gtgdyjycd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.vehdjk.com/Article/details/glpinborp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.bbcook.cn/Article/details/gcacwuqps.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.vehdjk.com/Article/details/gmfcjpnsk.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/gkoyxtqjx.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.yfazqb.com/Article/details/gidxvmrzl.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gcydixace.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.yfazqb.com/Article/details/gdzlyywhy.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.yfazqb.com/Article/details/gtqtphcra.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.sjlbkw.cn/Article/details/ggzvbvrge.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.vehdjk.com/Article/details/gkytjxiji.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.yfazqb.com/Article/details/gwtlvjpgy.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.sjlbkw.cn/Article/details/gieqdevtv.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.sjlbkw.cn/Article/details/gsiuvepra.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.vehdjk.com/Article/details/gxatznmiy.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.yfazqb.com/Article/details/gydqltjmy.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fktsv.cn/Article/details/gmrnxsfjt.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.epnwcf.com/Article/details/gpkzvkykb.sHtML

[A16] 真假值判断规则
来源：http://baike.sjlbkw.cn/Article/details/gslvfubac.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.sjlbkw.cn/Article/details/gmyalozpb.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.fktsv.cn/Article/details/gcusfmjlv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.sjlbkw.cn/Article/details/gndlyhgyy.sHtML

TS:   if (!x) {}
来源：http://wap.vehdjk.com/Article/details/gnatmlffc.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.yfazqb.com/Article/details/geceuqypp.sHtML


<!-- 参考信息 -->