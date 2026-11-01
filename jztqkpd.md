代发 wailian999

[U97] JS：并发请求
来源：http://www.blog.fktsv.cn/Article/details/gqpphpofp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gjvwmsxyz.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.epnwcf.com/Article/details/ghzbxjgck.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.bbcook.cn/Article/details/gpnomgxua.sHtML

[U99] JS：事件监听
来源：http://www.share.sjlbkw.cn/Article/details/ggwbddgzd.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.bbcook.cn/Article/details/gftfthwah.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.tarul.cn/Article/details/gdabqxenu.sHtML

document.querySelector(".item")
来源：http://wap.epnwcf.com/Article/details/gdtgclgqa.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.epnwcf.com/Article/details/gncjxmyqn.sHtML

el.classList.toggle("active")
来源：http://www.share.sjlbkw.cn/Article/details/gjbrdwxkd.sHtML

[U102] JS：本地存储
来源：http://www.share.fktsv.cn/Article/details/gjdigemnc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.sjlbkw.cn/Article/details/gcgkkekdp.sHtML

[U103] JS：定时器
来源：http://read.share.epnwcf.com/Article/details/giuxuenip.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.epnwcf.com/Article/details/gesklhebd.sHtML

[U104] JS：防抖
来源：http://www.blog.tarul.cn/Article/details/gqqjelebb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gvcaltijb.sHtML

[U105] JS：节流
来源：http://www.m.share.vehdjk.com/Article/details/gthnyedvw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fktsv.cn/Article/details/ggtwhzxqy.sHtML

[U106] JS：日期格式化
来源：http://wap.fktsv.cn/Article/details/gsaqdbpor.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.yfazqb.com/Article/details/gpkchoqsv.sHtML

[U107] JS：数字千分位
来源：http://mobile.bbcook.cn/Article/details/gqzgrpekp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.epnwcf.com/Article/details/gadnrjsop.sHtML

[U108] JS：随机整数
来源：http://wap.yfazqb.com/Article/details/gcvdpcygc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.bbcook.cn/Article/details/gwpfvdyor.sHtML

[U109] JS：数组分组
来源：http://mobile.sjlbkw.cn/Article/details/gwzgtanrn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.sjlbkw.cn/Article/details/gxlasklku.sHtML

[U110] JS：数组分块
来源：http://blog.epnwcf.com/Article/details/gvamulcdq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.yfazqb.com/Article/details/gzovrznlz.sHtML

[U111] JS：对象转 Map
来源：http://wap.fktsv.cn/Article/details/gmhbgroci.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.vehdjk.com/Article/details/gifdhpdet.sHtML

[U112] JS：字符串补位
来源：http://3g.epnwcf.com/Article/details/gdyuzmvko.sHtML

"7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gxwebajdo.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.bbcook.cn/Article/details/gceccpcty.sHtML

s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gejozytkl.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.tarul.cn/Article/details/gnzxwmjex.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/gmbyzzevb.sHtML

[U115] JS：生成 UUID
来源：http://baike.vehdjk.com/Article/details/gphuwrnbs.sHtML

crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gdrnbmqrf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fktsv.cn/Article/details/gjdplvouz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fktsv.cn/Article/details/gltexejxp.sHtML

[U117] JS：单元测试
来源：http://read.share.yfazqb.com/Article/details/gwiaxauxu.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.tarul.cn/Article/details/gworisrjr.sHtML

[U118] JS：开发服务器
来源：http://wap.bbcook.cn/Article/details/gfwjkbnud.sHtML

npm i -D vite;  npx vite
来源：http://3g.bbcook.cn/Article/details/gdutfyhml.sHtML

[U119] JS：生产构建
来源：http://wap.fktsv.cn/Article/details/gshfthxzn.sHtML

npx vite build
来源：http://www.blog.epnwcf.com/Article/details/gwcreoqia.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.vehdjk.com/Article/details/geqpvihhc.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.vehdjk.com/Article/details/gfpmyrgjm.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/glkllemfz.sHtML

统计汇总
来源：http://blog.bbcook.cn/Article/details/gjuvqijxv.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/goyexscyf.sHtML

按语言统计（条）：
来源：http://blog.epnwcf.com/Article/details/gvvmifziz.sHtML

Python ......... 252
来源：http://www.m.share.vehdjk.com/Article/details/gqcdpuljj.sHtML

PHP ............ 252
来源：http://www.blog.epnwcf.com/Article/details/gszpriwxr.sHtML

JavaScript ..... 252
来源：http://m.share.vehdjk.com/Article/details/gwmtkdukd.sHtML

TypeScript ..... 212
来源：http://mobile.epnwcf.com/Article/details/gjqlnkxjj.sHtML

Java ........... 212
来源：http://blog.fktsv.cn/Article/details/gynhvhxty.sHtML

Go ............. 212
来源：http://baike.tarul.cn/Article/details/gprprnzjt.sHtML

Ruby ........... 212
来源：http://blog.epnwcf.com/Article/details/gupoinist.sHtML

C# ............. 212
来源：http://m.share.sjlbkw.cn/Article/details/gcisqhmgv.sHtML

C .............. 30
来源：http://www.blog.tarul.cn/Article/details/gpgcwmmmc.sHtML

C++ ............ 30
来源：http://blog.bbcook.cn/Article/details/gpofjttdb.sHtML

SQL ............ 90
来源：http://www.m.share.bbcook.cn/Article/details/gbrkynyos.sHtML

Bash ........... 80
来源：http://3g.yfazqb.com/Article/details/ggqfdrcos.sHtML

Kotlin ......... 15
来源：http://mobile.yfazqb.com/Article/details/gtupqxtnp.sHtML

Swift .......... 15
来源：http://3g.bbcook.cn/Article/details/gozikbkmd.sHtML

Lua ............ 10
来源：http://www.blog.sjlbkw.cn/Article/details/gczbuvexg.sHtML

Perl ........... 10
来源：http://blog.epnwcf.com/Article/details/gyufimpjd.sHtML

Scala .......... 10
来源：http://3g.fktsv.cn/Article/details/greezsaux.sHtML

------------------------------------
来源：http://blog.bbcook.cn/Article/details/griyqgmop.sHtML

合计 ........... 2106 条
来源：http://www.blog.vehdjk.com/Article/details/gsgmpxvaw.sHtML

按章节统计：
来源：http://www.blog.sjlbkw.cn/Article/details/grzuubxkx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.bbcook.cn/Article/details/gtprcmrzs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.yfazqb.com/Article/details/gwinnqaqt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fktsv.cn/Article/details/gvbxalyrc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.tarul.cn/Article/details/gvshsadyq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.bbcook.cn/Article/details/gbhchxfiv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.vehdjk.com/Article/details/gnhanzsbb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.vehdjk.com/Article/details/gusafukpq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.sjlbkw.cn/Article/details/gwazmopyn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gdhlfhhta.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.tarul.cn/Article/details/gpruofgty.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gvscvmdpk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/gdjtrntmq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/ggqnrhufe.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.epnwcf.com/Article/details/ghyvatgoy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.bbcook.cn/Article/details/gxizxhsyi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/girayflum.sHtML

Q SQL 专题                              90
来源：http://wap.bbcook.cn/Article/details/gnnacluod.sHtML

R Bash 专题                             80
来源：http://3g.sjlbkw.cn/Article/details/gghvuxsbn.sHtML

S C / C++ 专题                          60
来源：http://3g.tarul.cn/Article/details/gknmfkkoc.sHtML

T 其他语言补充                          60
来源：http://3g.fktsv.cn/Article/details/ghfgiaatw.sHtML

U 高频实用片段                         120
来源：http://m.share.yfazqb.com/Article/details/gbylaeeme.sHtML

------------------------------------
来源：http://m.share.bbcook.cn/Article/details/giuszbrng.sHtML

合计                                  2106 条
来源：http://blog.yfazqb.com/Article/details/gzggluiqe.sHtML

--------------------------------------------------------------------------------
来源：http://baike.tarul.cn/Article/details/ggnqkzezc.sHtML

使用提醒
来源：http://mobile.fktsv.cn/Article/details/gcpfluetl.sHtML

--------------------------------------------------------------------------------
来源：http://wap.tarul.cn/Article/details/gqbibwtfv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.tarul.cn/Article/details/glzezhaqg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.yfazqb.com/Article/details/gqifujzjq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.tarul.cn/Article/details/gngwutjwc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.epnwcf.com/Article/details/gcdpehhtf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.yfazqb.com/Article/details/ggxawuvfb.sHtML

—— 文件结束 ——
来源：http://www.share.sjlbkw.cn/Article/details/gnhupglan.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzetplqx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.yfazqb.com/Article/details/gbkmqovla.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.tarul.cn/Article/details/gcfdtjywl.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gsctjoten.sHtML

【收录内容】
来源：http://www.m.share.tarul.cn/Article/details/gdoltddmq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.yfazqb.com/Article/details/gapsccuzx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.bbcook.cn/Article/details/gdhyulluf.sHtML

SQL · Bash · C · C++
来源：http://mobile.fktsv.cn/Article/details/gtnmdepyz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.bbcook.cn/Article/details/gmhtdacvc.sHtML

【使用说明】
来源：http://www.m.share.yfazqb.com/Article/details/gvldvhyhx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.tarul.cn/Article/details/gbfrhyick.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.vehdjk.com/Article/details/grpuutqed.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.vehdjk.com/Article/details/gzuxgzlqm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fktsv.cn/Article/details/grwonrctc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.yfazqb.com/Article/details/gqkpwjlrz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.epnwcf.com/Article/details/gcyghtyyv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.epnwcf.com/Article/details/gczsnmfuf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.bbcook.cn/Article/details/gaymcvanv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.tarul.cn/Article/details/gdsnepnqi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.tarul.cn/Article/details/gymkzxaxn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fktsv.cn/Article/details/ghldmceva.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.sjlbkw.cn/Article/details/geevnarlf.sHtML

【文件统计】
来源：http://www.m.share.tarul.cn/Article/details/gauyhhsup.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.sjlbkw.cn/Article/details/gnyfunhrp.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gvpvneawf.sHtML

目  录
来源：http://mobile.bbcook.cn/Article/details/gonfiipba.sHtML

--------------------------------------------------------------------------------
来源：http://3g.vehdjk.com/Article/details/gpjhgmhat.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.vehdjk.com/Article/details/gqvyxuhok.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/gdweglbep.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.epnwcf.com/Article/details/gqionepjp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.epnwcf.com/Article/details/gebbpocto.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.vehdjk.com/Article/details/gxwuhhfkb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.epnwcf.com/Article/details/gblndwuxu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrdhkzzr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.tarul.cn/Article/details/gbceiwomf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.bbcook.cn/Article/details/gbgevfbdj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.vehdjk.com/Article/details/gnrrdjbrx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.bbcook.cn/Article/details/gbqvkwkfr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fktsv.cn/Article/details/ghpmvzsgm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.sjlbkw.cn/Article/details/gccbtpvhx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fktsv.cn/Article/details/gtidtuhqn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fktsv.cn/Article/details/gywpgwahp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.vehdjk.com/Article/details/ganmlxbuj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.epnwcf.com/Article/details/gchcafyna.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.yfazqb.com/Article/details/gnstpdoge.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.yfazqb.com/Article/details/goeqeirmq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.epnwcf.com/Article/details/gwkekmony.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.sjlbkw.cn/Article/details/govdpqzkx.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gyqexxlof.sHtML

A. 基础语法与类型
来源：http://read.share.bbcook.cn/Article/details/grgnlvpqe.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/grvbgzfjn.sHtML

[A01] Hello World
来源：http://wap.sjlbkw.cn/Article/details/gdxuurvhx.sHtML

Py:   print("Hello, World!")
来源：http://baike.bbcook.cn/Article/details/gsvqzpycq.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.vehdjk.com/Article/details/gkzxnevlb.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.tarul.cn/Article/details/gerxwcgha.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.yfazqb.com/Article/details/gcvigbrll.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.sjlbkw.cn/Article/details/gjfscticu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.epnwcf.com/Article/details/gnmcpghss.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.tarul.cn/Article/details/ggngwelef.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fktsv.cn/Article/details/gtagorutw.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.vehdjk.com/Article/details/gaoagjlbz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.tarul.cn/Article/details/gqvrysgws.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.sjlbkw.cn/Article/details/gnhtlclac.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gugnxwlfb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtzmdiba.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.tarul.cn/Article/details/gkutyskvg.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.bbcook.cn/Article/details/gmjtsrqfy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fktsv.cn/Article/details/gbfhxcnxf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.bbcook.cn/Article/details/gldpvhhxb.sHtML

[A03] 常量定义
来源：http://blog.vehdjk.com/Article/details/gvakkxjky.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.sjlbkw.cn/Article/details/glszkctmz.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gymfnwuxn.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gbwreggwb.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/godcgjtpo.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gomvrxhdd.sHtML

Go:   const PI = 3.14159
来源：http://blog.epnwcf.com/Article/details/gsdbvyjqc.sHtML

Ruby: PI = 3.14159
来源：http://www.share.sjlbkw.cn/Article/details/grfwzkuiq.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gaenebygt.sHtML

[A04] 判断变量类型
来源：http://m.share.epnwcf.com/Article/details/ggjmpomag.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.tarul.cn/Article/details/grkcqlirf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.yfazqb.com/Article/details/gajhvqses.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.bbcook.cn/Article/details/gartnjohv.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.epnwcf.com/Article/details/gjbimvmgd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.yfazqb.com/Article/details/gchslfryz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.tarul.cn/Article/details/ginxdeqzb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.tarul.cn/Article/details/gfantdsdk.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.bbcook.cn/Article/details/gnxabrhfn.sHtML

[A05] 整数除法与取模
来源：http://baike.epnwcf.com/Article/details/grepopqtt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.vehdjk.com/Article/details/gvdvajwwl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.vehdjk.com/Article/details/ggdrbwmet.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.tarul.cn/Article/details/gmytwgtid.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gknmfggur.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/gstgdflwj.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.epnwcf.com/Article/details/gevgprdfk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.tarul.cn/Article/details/gaktovhen.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.sjlbkw.cn/Article/details/guujmtmiu.sHtML

[A06] 字符串转数字
来源：http://m.share.epnwcf.com/Article/details/gijyluvdq.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fktsv.cn/Article/details/gufnbhkfc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.yfazqb.com/Article/details/gsgiliatu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.vehdjk.com/Article/details/gudwabtzl.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.epnwcf.com/Article/details/gtjhxxnov.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.yfazqb.com/Article/details/guojvotrd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.vehdjk.com/Article/details/givdkwije.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxkzkjjw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.epnwcf.com/Article/details/gfuflyquh.sHtML

[A07] 数字转字符串
来源：http://baike.vehdjk.com/Article/details/gqcyfjses.sHtML

Py:   str(42)
来源：http://3g.yfazqb.com/Article/details/gmlfkgriu.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.bbcook.cn/Article/details/gavgzhoxl.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.vehdjk.com/Article/details/glhhnwsfl.sHtML

TS:   String(42)
来源：http://mobile.yfazqb.com/Article/details/gythcsoiq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fktsv.cn/Article/details/gylucpuha.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.yfazqb.com/Article/details/gydziimmg.sHtML

Ruby: 42.to_s
来源：http://baike.sjlbkw.cn/Article/details/gseahjrmx.sHtML

C#:   42.ToString()
来源：http://www.share.epnwcf.com/Article/details/gbxmlpgzz.sHtML

[A08] 取整与四舍五入
来源：http://m.share.epnwcf.com/Article/details/gqlvbvrkc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.epnwcf.com/Article/details/gxvwimfin.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fktsv.cn/Article/details/gtouhhqug.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.sjlbkw.cn/Article/details/gcptckvby.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.tarul.cn/Article/details/gdmrqknil.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.sjlbkw.cn/Article/details/giswkvmjq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.vehdjk.com/Article/details/ghxiosdyi.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.epnwcf.com/Article/details/gltabqtws.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/gjzifwplo.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.vehdjk.com/Article/details/gdeojsbuf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fktsv.cn/Article/details/grtvgyggu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.yfazqb.com/Article/details/greqctyrz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gplcrkegq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gnjgggvkn.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.tarul.cn/Article/details/gvybnekvx.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.fktsv.cn/Article/details/gtqjiwsst.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwjevbll.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fktsv.cn/Article/details/gsclwmdaj.sHtML

[A10] 生成随机数
来源：http://mobile.bbcook.cn/Article/details/gtsbxtcnc.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.bbcook.cn/Article/details/gmtcufkqd.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.tarul.cn/Article/details/gorkljkqy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.sjlbkw.cn/Article/details/ghvqmnmrl.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.bbcook.cn/Article/details/gvrepmlae.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.yfazqb.com/Article/details/ggllnsfos.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.vehdjk.com/Article/details/gmqnswvsj.sHtML

Ruby: rand(1..100)
来源：http://blog.yfazqb.com/Article/details/gcdeqwafq.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fktsv.cn/Article/details/gmcqoladw.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fktsv.cn/Article/details/gmoqdprfy.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.fktsv.cn/Article/details/gsldkkkqa.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.bbcook.cn/Article/details/gxeexrdqb.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.yfazqb.com/Article/details/gbdeippaw.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/gomtrgjni.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.vehdjk.com/Article/details/gcazfcjeq.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.sjlbkw.cn/Article/details/gdwmlaawb.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.sjlbkw.cn/Article/details/gpvuteolc.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/gxwslvjui.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.sjlbkw.cn/Article/details/gmnijyqkg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.bbcook.cn/Article/details/gyadvzedl.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.sjlbkw.cn/Article/details/guwjtkjpf.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.bbcook.cn/Article/details/grpaczaon.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.bbcook.cn/Article/details/gplihaakz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.sjlbkw.cn/Article/details/ghyqqypdz.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.tarul.cn/Article/details/gevntchgo.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.tarul.cn/Article/details/gbmbksrdo.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.fktsv.cn/Article/details/gftnjfxlh.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.epnwcf.com/Article/details/gzzgnjzfy.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/gbetanspt.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gvxikbbri.sHtML

JS:   "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/gxafluywx.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.vehdjk.com/Article/details/gbexajqfo.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gupnevldr.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/geypjndxb.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.tarul.cn/Article/details/gocxgjhei.sHtML

C#:   "第一行\n第二行"
来源：http://3g.bbcook.cn/Article/details/gzzgxssyl.sHtML

[A14] 注释写法
来源：http://www.m.share.yfazqb.com/Article/details/ggtujgjrz.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fktsv.cn/Article/details/glikdjtpu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.epnwcf.com/Article/details/gijfryegp.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.sjlbkw.cn/Article/details/gsprrprax.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.tarul.cn/Article/details/gegundouv.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fktsv.cn/Article/details/gdmqvfrvg.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.tarul.cn/Article/details/gwkckvzmh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fktsv.cn/Article/details/gxpxcxbld.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.bbcook.cn/Article/details/gmrejjfgl.sHtML

[A15] 空值判断与默认值
来源：http://3g.fktsv.cn/Article/details/geuutvdyz.sHtML

Py:   value = data or "默认值"
来源：http://read.share.bbcook.cn/Article/details/gxixqqfbr.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.fktsv.cn/Article/details/ghuiwvzbf.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.bbcook.cn/Article/details/gmvcgwfbh.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.yfazqb.com/Article/details/gacvrtzsi.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.bbcook.cn/Article/details/gddkemnyy.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.vehdjk.com/Article/details/goibmfqkv.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fktsv.cn/Article/details/ggtiwduvo.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.sjlbkw.cn/Article/details/gifziauii.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.yfazqb.com/Article/details/gbwyxzxzf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.epnwcf.com/Article/details/girfgumtb.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.bbcook.cn/Article/details/gjivwayri.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.vehdjk.com/Article/details/gfxrwcqaq.sHtML

TS:   if (!x) {}
来源：http://www.m.share.tarul.cn/Article/details/gfxranhux.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gkwtcvwfg.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.fktsv.cn/Article/details/gzhyeyfzp.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.epnwcf.com/Article/details/gnqjepado.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.sjlbkw.cn/Article/details/gtdnzaorp.sHtML

[A17] 位运算
来源：http://wap.sjlbkw.cn/Article/details/gahgjmsua.sHtML


<!-- 参考信息 -->