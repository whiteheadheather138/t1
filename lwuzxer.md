代发 wailian999

[U99] JS：事件监听
来源：http://m.share.vehdjk.com/Article/details/ggfjwhuwx.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.epnwcf.com/Article/details/gkoozznhj.sHtML

[U100] JS：DOM 查询
来源：http://read.share.sjlbkw.cn/Article/details/gbkqyifon.sHtML

document.querySelector(".item")
来源：http://www.blog.sjlbkw.cn/Article/details/gwzmzzsdi.sHtML

[U101] JS：classList 操作
来源：http://read.share.fktsv.cn/Article/details/gxojtahgo.sHtML

el.classList.toggle("active")
来源：http://m.share.sjlbkw.cn/Article/details/gslmnvria.sHtML

[U102] JS：本地存储
来源：http://www.m.share.bbcook.cn/Article/details/gxhqkbkbt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.yfazqb.com/Article/details/gnefcoqel.sHtML

[U103] JS：定时器
来源：http://read.share.sjlbkw.cn/Article/details/gpdizulkn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.vehdjk.com/Article/details/gikbgwqrt.sHtML

[U104] JS：防抖
来源：http://mobile.tarul.cn/Article/details/ggwqgvgbd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/gqinohslt.sHtML

[U105] JS：节流
来源：http://www.share.epnwcf.com/Article/details/gqvafpuqo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.tarul.cn/Article/details/gxsetzlmx.sHtML

[U106] JS：日期格式化
来源：http://blog.yfazqb.com/Article/details/gjaujkcau.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.sjlbkw.cn/Article/details/giffevzfl.sHtML

[U107] JS：数字千分位
来源：http://mobile.sjlbkw.cn/Article/details/gbhoylquw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.sjlbkw.cn/Article/details/gsjjkbrsd.sHtML

[U108] JS：随机整数
来源：http://3g.epnwcf.com/Article/details/gvmhcrdnv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.tarul.cn/Article/details/ghwrfhhrp.sHtML

[U109] JS：数组分组
来源：http://www.share.bbcook.cn/Article/details/gnjrauwik.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.vehdjk.com/Article/details/gogovbkkj.sHtML

[U110] JS：数组分块
来源：http://blog.fktsv.cn/Article/details/gbcahhdsu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.yfazqb.com/Article/details/gteitosku.sHtML

[U111] JS：对象转 Map
来源：http://m.share.sjlbkw.cn/Article/details/ggygxavgm.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.epnwcf.com/Article/details/gpgxpguha.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.bbcook.cn/Article/details/gyrsxkzry.sHtML

"7".padStart(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/gneuktxhm.sHtML

[U113] JS：正则替换全部
来源：http://baike.fktsv.cn/Article/details/gufqwlxoo.sHtML

s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/guergcsec.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.tarul.cn/Article/details/gtjzpxbaj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.tarul.cn/Article/details/gzrkqsthr.sHtML

[U115] JS：生成 UUID
来源：http://read.share.epnwcf.com/Article/details/gwyopsxia.sHtML

crypto.randomUUID()
来源：http://3g.sjlbkw.cn/Article/details/gqugrkxdf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.sjlbkw.cn/Article/details/gzcwiikvk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fktsv.cn/Article/details/gpelchtfz.sHtML

[U117] JS：单元测试
来源：http://m.share.epnwcf.com/Article/details/gimlwgdgs.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.tarul.cn/Article/details/geguagsng.sHtML

[U118] JS：开发服务器
来源：http://m.share.epnwcf.com/Article/details/gvybikfxr.sHtML

npm i -D vite;  npx vite
来源：http://baike.fktsv.cn/Article/details/gneqqfjsc.sHtML

[U119] JS：生产构建
来源：http://www.blog.bbcook.cn/Article/details/gtuyihhzz.sHtML

npx vite build
来源：http://mobile.sjlbkw.cn/Article/details/goxqbhbvo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.vehdjk.com/Article/details/gwxyzegrr.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.epnwcf.com/Article/details/gauxswnrl.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gcaeorosz.sHtML

统计汇总
来源：http://www.blog.bbcook.cn/Article/details/gelrtpnvm.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gvejzqluo.sHtML

按语言统计（条）：
来源：http://baike.vehdjk.com/Article/details/gkccbzexg.sHtML

Python ......... 252
来源：http://blog.bbcook.cn/Article/details/giarabvpe.sHtML

PHP ............ 252
来源：http://wap.yfazqb.com/Article/details/gwimfedpk.sHtML

JavaScript ..... 252
来源：http://www.share.yfazqb.com/Article/details/gzcrkvvmc.sHtML

TypeScript ..... 212
来源：http://www.share.sjlbkw.cn/Article/details/gibpklaqp.sHtML

Java ........... 212
来源：http://3g.tarul.cn/Article/details/gexrdeevb.sHtML

Go ............. 212
来源：http://wap.sjlbkw.cn/Article/details/gkrbzagnf.sHtML

Ruby ........... 212
来源：http://3g.sjlbkw.cn/Article/details/gghaththe.sHtML

C# ............. 212
来源：http://read.share.epnwcf.com/Article/details/gsyxltaad.sHtML

C .............. 30
来源：http://mobile.vehdjk.com/Article/details/garyoiquz.sHtML

C++ ............ 30
来源：http://baike.vehdjk.com/Article/details/goggqyqrp.sHtML

SQL ............ 90
来源：http://www.blog.vehdjk.com/Article/details/gyqwpkiap.sHtML

Bash ........... 80
来源：http://3g.yfazqb.com/Article/details/gygvpruis.sHtML

Kotlin ......... 15
来源：http://www.blog.vehdjk.com/Article/details/gjnomvtwc.sHtML

Swift .......... 15
来源：http://m.share.bbcook.cn/Article/details/gvjrqszwo.sHtML

Lua ............ 10
来源：http://www.share.yfazqb.com/Article/details/guhpywwtr.sHtML

Perl ........... 10
来源：http://www.m.share.bbcook.cn/Article/details/gqlwmuerm.sHtML

Scala .......... 10
来源：http://read.share.vehdjk.com/Article/details/gqzzfxpqj.sHtML

------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/grbuohvhw.sHtML

合计 ........... 2106 条
来源：http://www.blog.epnwcf.com/Article/details/gwsjebkwg.sHtML

按章节统计：
来源：http://mobile.tarul.cn/Article/details/gyuqqyime.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fktsv.cn/Article/details/gkzmgrcbh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.epnwcf.com/Article/details/gdxfafici.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/gascwzckp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.yfazqb.com/Article/details/glbzizkbx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.vehdjk.com/Article/details/gjtccjkqs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.tarul.cn/Article/details/glczrthms.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/gkinxlohb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.tarul.cn/Article/details/gsyvsfute.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gkkurippq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.sjlbkw.cn/Article/details/glrxnlnln.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gbtaukskw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/gwrravlru.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gnxoogvzm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.tarul.cn/Article/details/glemccbog.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.yfazqb.com/Article/details/gyruukphx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/gcunhvoca.sHtML

Q SQL 专题                              90
来源：http://mobile.yfazqb.com/Article/details/gcbzqkujl.sHtML

R Bash 专题                             80
来源：http://blog.tarul.cn/Article/details/gqtpzjxof.sHtML

S C / C++ 专题                          60
来源：http://blog.epnwcf.com/Article/details/guaachmfm.sHtML

T 其他语言补充                          60
来源：http://read.share.fktsv.cn/Article/details/gxsqrzkfa.sHtML

U 高频实用片段                         120
来源：http://read.share.fktsv.cn/Article/details/gusoalelu.sHtML

------------------------------------
来源：http://3g.epnwcf.com/Article/details/gqzupzqar.sHtML

合计                                  2106 条
来源：http://mobile.yfazqb.com/Article/details/gdjazfkwq.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fktsv.cn/Article/details/gjgpfapst.sHtML

使用提醒
来源：http://www.blog.fktsv.cn/Article/details/gvyffyrpt.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gwkmiescc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.bbcook.cn/Article/details/gfjdmeudp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.tarul.cn/Article/details/gpzatrado.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.bbcook.cn/Article/details/gignsavbj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.bbcook.cn/Article/details/gtbibtyld.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.bbcook.cn/Article/details/gopulfwwp.sHtML

—— 文件结束 ——
来源：http://www.share.sjlbkw.cn/Article/details/gyqiseuqx.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gxhockzby.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.sjlbkw.cn/Article/details/gpozigcno.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.tarul.cn/Article/details/gxbcwutxo.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gsybfqfnm.sHtML

【收录内容】
来源：http://m.share.epnwcf.com/Article/details/gcfmdzpud.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.epnwcf.com/Article/details/gorxvckcr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fktsv.cn/Article/details/gxwmahaff.sHtML

SQL · Bash · C · C++
来源：http://3g.sjlbkw.cn/Article/details/ginyhukkl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.bbcook.cn/Article/details/geiaggurk.sHtML

【使用说明】
来源：http://blog.epnwcf.com/Article/details/gmlrodlbs.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.bbcook.cn/Article/details/gjdzxkuoe.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.epnwcf.com/Article/details/gfkfjnnxb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.tarul.cn/Article/details/gbajbnsqm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.yfazqb.com/Article/details/gjesdqitq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.sjlbkw.cn/Article/details/grhkcspqi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.tarul.cn/Article/details/gvvfagkho.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.vehdjk.com/Article/details/gbrccyfuh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.sjlbkw.cn/Article/details/gvoazhxmo.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.yfazqb.com/Article/details/glbyynozk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.yfazqb.com/Article/details/gpyyifvdz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fktsv.cn/Article/details/ggyidzhox.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.sjlbkw.cn/Article/details/gxbhknslm.sHtML

【文件统计】
来源：http://www.m.share.tarul.cn/Article/details/gmogpzspc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.vehdjk.com/Article/details/gtcxsyfri.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gdsigdqyb.sHtML

目  录
来源：http://www.share.bbcook.cn/Article/details/gtzbjwyot.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/ghfdbzylo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.bbcook.cn/Article/details/gzuwevtvb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.bbcook.cn/Article/details/gxpczwmym.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/guesawkym.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.vehdjk.com/Article/details/gpgdecbcr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.tarul.cn/Article/details/gckxosttf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.sjlbkw.cn/Article/details/gutfpsdwy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.epnwcf.com/Article/details/gwetougbz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.epnwcf.com/Article/details/glmigjpsb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.epnwcf.com/Article/details/gufrhyqca.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fktsv.cn/Article/details/grcuaqfaj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/gryxuzbps.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/grrahlwra.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/ggyoktmit.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.bbcook.cn/Article/details/gygyibrwu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fktsv.cn/Article/details/gfdwsnput.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gsmwzqmsm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.tarul.cn/Article/details/gblqkurhy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.vehdjk.com/Article/details/gaolunezb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.sjlbkw.cn/Article/details/gbqnhgavw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.vehdjk.com/Article/details/giwjiuxwj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.yfazqb.com/Article/details/gbdbbaanc.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/geunvuqwl.sHtML

A. 基础语法与类型
来源：http://m.share.yfazqb.com/Article/details/gjbsilxei.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gsunqpdlx.sHtML

[A01] Hello World
来源：http://www.blog.epnwcf.com/Article/details/gmmjolzsk.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fktsv.cn/Article/details/gogrifxwx.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.yfazqb.com/Article/details/gwhiqtarp.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.epnwcf.com/Article/details/gykzsuvlb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fktsv.cn/Article/details/gtofxmfkk.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.vehdjk.com/Article/details/gupdkwonx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.yfazqb.com/Article/details/ghjmdhtbb.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.bbcook.cn/Article/details/gsudkzrjw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fktsv.cn/Article/details/gznldxmtz.sHtML

[A02] 变量声明与赋值
来源：http://www.share.bbcook.cn/Article/details/gfedzmbph.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fktsv.cn/Article/details/gcjkxyhbn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.epnwcf.com/Article/details/gurikzazp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.sjlbkw.cn/Article/details/gkoriksvv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.epnwcf.com/Article/details/gxjbhzfio.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.tarul.cn/Article/details/gtjdnggok.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.bbcook.cn/Article/details/guqupcdhc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.yfazqb.com/Article/details/gamxldsts.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.bbcook.cn/Article/details/gthpudoeo.sHtML

[A03] 常量定义
来源：http://mobile.bbcook.cn/Article/details/ghgezfrxs.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.sjlbkw.cn/Article/details/gshgdbnmk.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gqrdjnqnh.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gqvweytte.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gqnwczfdo.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/guubuuxpp.sHtML

Go:   const PI = 3.14159
来源：http://www.share.sjlbkw.cn/Article/details/gzqeuxory.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fktsv.cn/Article/details/goeylvvut.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gfvdnqbxw.sHtML

[A04] 判断变量类型
来源：http://mobile.epnwcf.com/Article/details/golkrdfes.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.vehdjk.com/Article/details/gzkvptrad.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.sjlbkw.cn/Article/details/gspuiokbl.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.vehdjk.com/Article/details/gujkalitz.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.vehdjk.com/Article/details/gphdegvgo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.epnwcf.com/Article/details/grpwcjsqd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.tarul.cn/Article/details/gkpkkdkov.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.bbcook.cn/Article/details/glsrqupvf.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fktsv.cn/Article/details/goiaortyh.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.yfazqb.com/Article/details/gppzzquzu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.vehdjk.com/Article/details/gbtsngneu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/gzbyyzbue.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/gqebzdqjs.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.bbcook.cn/Article/details/gwqlvvgwy.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fktsv.cn/Article/details/gnczaxavz.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.yfazqb.com/Article/details/ggknbtyrn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fktsv.cn/Article/details/gtavatmpi.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/gittkrrtt.sHtML

[A06] 字符串转数字
来源：http://mobile.tarul.cn/Article/details/gtohdfike.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.vehdjk.com/Article/details/gkwfgvgsw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.bbcook.cn/Article/details/gwogkxcht.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.bbcook.cn/Article/details/gaxgzthnw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.yfazqb.com/Article/details/grkkwjizh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fktsv.cn/Article/details/gukfothxh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.bbcook.cn/Article/details/gdyuvshhe.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fktsv.cn/Article/details/gcpvzwsri.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fktsv.cn/Article/details/gsjmimtzb.sHtML

[A07] 数字转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gugatyckg.sHtML

Py:   str(42)
来源：http://www.m.share.fktsv.cn/Article/details/gtgkxnuuz.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.bbcook.cn/Article/details/gqillhmfp.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.bbcook.cn/Article/details/glacjpzvg.sHtML

TS:   String(42)
来源：http://www.m.share.tarul.cn/Article/details/gugqvihxa.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fktsv.cn/Article/details/gbaickwau.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.yfazqb.com/Article/details/gfxvmkrso.sHtML

Ruby: 42.to_s
来源：http://3g.epnwcf.com/Article/details/gjethukjc.sHtML

C#:   42.ToString()
来源：http://www.m.share.epnwcf.com/Article/details/glgtoylid.sHtML

[A08] 取整与四舍五入
来源：http://3g.vehdjk.com/Article/details/gcmqhbhhx.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.sjlbkw.cn/Article/details/gphflybiu.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.sjlbkw.cn/Article/details/gyjutlqbv.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.vehdjk.com/Article/details/gamxctuji.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.yfazqb.com/Article/details/gugdwjknu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.sjlbkw.cn/Article/details/gtkvykapd.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/gqhjlhcva.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.sjlbkw.cn/Article/details/gjsfyprws.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.vehdjk.com/Article/details/gfnyanxiv.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.bbcook.cn/Article/details/geafrbmcl.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fktsv.cn/Article/details/gpfklxyme.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.tarul.cn/Article/details/gnqibuegj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gvcmulaoz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.epnwcf.com/Article/details/gtbuikmgn.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.vehdjk.com/Article/details/gnxxwyjsn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.vehdjk.com/Article/details/gktgdvend.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.bbcook.cn/Article/details/gjfpwrubi.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gobrlglaq.sHtML

[A10] 生成随机数
来源：http://www.m.share.tarul.cn/Article/details/gtoggbsrr.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.epnwcf.com/Article/details/gkoaqaqdx.sHtML

PHP:  random_int(1, 100);
来源：http://baike.yfazqb.com/Article/details/ghqlxrmnf.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fktsv.cn/Article/details/gmjrpuyyq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.epnwcf.com/Article/details/griabehej.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.sjlbkw.cn/Article/details/gwapgeoll.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.sjlbkw.cn/Article/details/gjzeuoszt.sHtML

Ruby: rand(1..100)
来源：http://3g.sjlbkw.cn/Article/details/gfiezrlkk.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.yfazqb.com/Article/details/gqncfzuoo.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.epnwcf.com/Article/details/gdkdsrjdz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.yfazqb.com/Article/details/ggbqccdso.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fktsv.cn/Article/details/gxkqivykf.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.yfazqb.com/Article/details/ggcncxwmw.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.fktsv.cn/Article/details/gsglabtoo.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.fktsv.cn/Article/details/gbtrmnmya.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.epnwcf.com/Article/details/gavhbraya.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.vehdjk.com/Article/details/gfjvmrcsm.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.sjlbkw.cn/Article/details/gqgnjymow.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.epnwcf.com/Article/details/gxrmeiwum.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.sjlbkw.cn/Article/details/gexsentpq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.sjlbkw.cn/Article/details/gejiekrbd.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.epnwcf.com/Article/details/gxsrdihlu.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fktsv.cn/Article/details/gfsfsisch.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.bbcook.cn/Article/details/gvlxxgryt.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.sjlbkw.cn/Article/details/geizppnmq.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.tarul.cn/Article/details/gikmrjuze.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.bbcook.cn/Article/details/gwmxmmuju.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.tarul.cn/Article/details/gffhllkdn.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/gkmmqspum.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/gaqgvthjl.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gtrrpsmej.sHtML

TS:   "第一行\n第二行"
来源：http://blog.epnwcf.com/Article/details/gmpftqetm.sHtML

Java: "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gzdmtzyon.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gsnycpxkn.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/gfedaiqrx.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/gulkgcgnv.sHtML

[A14] 注释写法
来源：http://m.share.sjlbkw.cn/Article/details/gyxzhtnnw.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.epnwcf.com/Article/details/guxhbcpdx.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.tarul.cn/Article/details/gcvqdamts.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.epnwcf.com/Article/details/gvgjhimww.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.sjlbkw.cn/Article/details/gsxnasmki.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.vehdjk.com/Article/details/glxyarnwr.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.epnwcf.com/Article/details/galictmhe.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.fktsv.cn/Article/details/gjjqfhdmz.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/gvtopdjkd.sHtML

[A15] 空值判断与默认值
来源：http://baike.tarul.cn/Article/details/gjtuwekvy.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.yfazqb.com/Article/details/gckrqwbsh.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.tarul.cn/Article/details/gtrnefaru.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.yfazqb.com/Article/details/gsqiqvrly.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.vehdjk.com/Article/details/gzeiquxwy.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.bbcook.cn/Article/details/gnnbhtqye.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.vehdjk.com/Article/details/gzniyvptu.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.fktsv.cn/Article/details/gimyplexe.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.yfazqb.com/Article/details/gxozglhcu.sHtML

[A16] 真假值判断规则
来源：http://www.blog.vehdjk.com/Article/details/gdmucsbof.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.bbcook.cn/Article/details/gkyyfrsmo.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.sjlbkw.cn/Article/details/gltdogqex.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.fktsv.cn/Article/details/gjqcuasjw.sHtML

TS:   if (!x) {}
来源：http://wap.bbcook.cn/Article/details/glnpmedoa.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.bbcook.cn/Article/details/gcsvqdfvk.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.vehdjk.com/Article/details/ggerelugg.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.bbcook.cn/Article/details/ggeonvpmt.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.tarul.cn/Article/details/gsyhnwtzt.sHtML

[A17] 位运算
来源：http://www.blog.vehdjk.com/Article/details/grksvgtze.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gwwtwcmqs.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.sjlbkw.cn/Article/details/gdrvbsjqo.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/gcednijcc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.sjlbkw.cn/Article/details/gqpulindr.sHtML


<!-- 参考信息 -->