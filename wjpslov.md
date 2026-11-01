代发 wailian999

[U99] JS：事件监听
来源：http://wap.fktsv.cn/Article/details/gotmcowhm.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.tarul.cn/Article/details/gappnzvgf.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.yfazqb.com/Article/details/gdhakvean.sHtML

document.querySelector(".item")
来源：http://www.m.share.sjlbkw.cn/Article/details/gljgobhni.sHtML

[U101] JS：classList 操作
来源：http://m.share.vehdjk.com/Article/details/gevbtcvya.sHtML

el.classList.toggle("active")
来源：http://mobile.fktsv.cn/Article/details/gmcrbqxam.sHtML

[U102] JS：本地存储
来源：http://www.share.epnwcf.com/Article/details/gnqbuusrv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.sjlbkw.cn/Article/details/gcrqbumhd.sHtML

[U103] JS：定时器
来源：http://www.blog.vehdjk.com/Article/details/gdjwhssdo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.sjlbkw.cn/Article/details/gzsttbbwf.sHtML

[U104] JS：防抖
来源：http://www.m.share.sjlbkw.cn/Article/details/graihhrom.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gqvmzcaef.sHtML

[U105] JS：节流
来源：http://read.share.epnwcf.com/Article/details/gyljkbmpr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.sjlbkw.cn/Article/details/gcomndlto.sHtML

[U106] JS：日期格式化
来源：http://3g.epnwcf.com/Article/details/gmdskhicu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.tarul.cn/Article/details/gkzwrrklf.sHtML

[U107] JS：数字千分位
来源：http://baike.sjlbkw.cn/Article/details/grejdlako.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.vehdjk.com/Article/details/gnecvonpl.sHtML

[U108] JS：随机整数
来源：http://www.share.bbcook.cn/Article/details/gxubdgqqb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.sjlbkw.cn/Article/details/gszzuafur.sHtML

[U109] JS：数组分组
来源：http://wap.vehdjk.com/Article/details/gjsvlnxtw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fktsv.cn/Article/details/gvkccbcdz.sHtML

[U110] JS：数组分块
来源：http://wap.sjlbkw.cn/Article/details/gvgqhyhbm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.sjlbkw.cn/Article/details/grllotqpv.sHtML

[U111] JS：对象转 Map
来源：http://m.share.sjlbkw.cn/Article/details/gbriuiscq.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.epnwcf.com/Article/details/gvcbdkwbp.sHtML

[U112] JS：字符串补位
来源：http://wap.vehdjk.com/Article/details/gbdiekqvx.sHtML

"7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gaqdhxbpp.sHtML

[U113] JS：正则替换全部
来源：http://wap.fktsv.cn/Article/details/gchoxtcnr.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gzxhqckho.sHtML

[U114] JS：JSON 深比较
来源：http://baike.sjlbkw.cn/Article/details/gevvbsudv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.sjlbkw.cn/Article/details/gqautkhkw.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fktsv.cn/Article/details/gsdbyxhpt.sHtML

crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/gvohmeyxv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.epnwcf.com/Article/details/gkmelaecr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.epnwcf.com/Article/details/geoqjxnhh.sHtML

[U117] JS：单元测试
来源：http://baike.yfazqb.com/Article/details/gpnqowiql.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fktsv.cn/Article/details/gjnwcjllu.sHtML

[U118] JS：开发服务器
来源：http://www.share.epnwcf.com/Article/details/ggcgjbidh.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.yfazqb.com/Article/details/glqqcbawd.sHtML

[U119] JS：生产构建
来源：http://3g.sjlbkw.cn/Article/details/gjytamhza.sHtML

npx vite build
来源：http://www.share.epnwcf.com/Article/details/ggbglamkc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.epnwcf.com/Article/details/glmcdkbpm.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.epnwcf.com/Article/details/gunynrwla.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gxbghucjy.sHtML

统计汇总
来源：http://www.m.share.tarul.cn/Article/details/gcgbxhftv.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gjgpowzha.sHtML

按语言统计（条）：
来源：http://baike.bbcook.cn/Article/details/gagwplotp.sHtML

Python ......... 252
来源：http://m.share.tarul.cn/Article/details/ggvhsykxe.sHtML

PHP ............ 252
来源：http://baike.epnwcf.com/Article/details/gnmxmdred.sHtML

JavaScript ..... 252
来源：http://mobile.vehdjk.com/Article/details/gclmgyoqu.sHtML

TypeScript ..... 212
来源：http://3g.sjlbkw.cn/Article/details/gjmtwdtwj.sHtML

Java ........... 212
来源：http://www.share.yfazqb.com/Article/details/ggilsihbz.sHtML

Go ............. 212
来源：http://3g.sjlbkw.cn/Article/details/gcxwkdxak.sHtML

Ruby ........... 212
来源：http://read.share.vehdjk.com/Article/details/gvcqobeow.sHtML

C# ............. 212
来源：http://baike.fktsv.cn/Article/details/gcwtmkcap.sHtML

C .............. 30
来源：http://www.blog.bbcook.cn/Article/details/gbzjotcbd.sHtML

C++ ............ 30
来源：http://read.share.yfazqb.com/Article/details/gkfcxqlhl.sHtML

SQL ............ 90
来源：http://www.m.share.tarul.cn/Article/details/gnqsxgfuu.sHtML

Bash ........... 80
来源：http://m.share.yfazqb.com/Article/details/gdvcwbtev.sHtML

Kotlin ......... 15
来源：http://www.blog.sjlbkw.cn/Article/details/gfulhklot.sHtML

Swift .......... 15
来源：http://read.share.fktsv.cn/Article/details/gotheahre.sHtML

Lua ............ 10
来源：http://baike.bbcook.cn/Article/details/gefkwibqf.sHtML

Perl ........... 10
来源：http://blog.epnwcf.com/Article/details/gxpwpcnna.sHtML

Scala .......... 10
来源：http://wap.vehdjk.com/Article/details/gvoylrlhe.sHtML

------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gxcibrydq.sHtML

合计 ........... 2106 条
来源：http://baike.vehdjk.com/Article/details/goftaefdl.sHtML

按章节统计：
来源：http://www.blog.fktsv.cn/Article/details/gsxecslgi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fktsv.cn/Article/details/gceqjedem.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.epnwcf.com/Article/details/ghgksajxh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.yfazqb.com/Article/details/gbwaohoen.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.sjlbkw.cn/Article/details/gagjtdvbk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fktsv.cn/Article/details/gdylorpcf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.tarul.cn/Article/details/gzcpuezxk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.yfazqb.com/Article/details/ghwuzypts.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.sjlbkw.cn/Article/details/ghqwrpvtn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gcmekkzmz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.epnwcf.com/Article/details/gnezljgoj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gqsyzxyzo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gkhqbpfyj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/grjkpksmo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.epnwcf.com/Article/details/gvfloguye.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fktsv.cn/Article/details/grbyqgzzw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/gjfngaohl.sHtML

Q SQL 专题                              90
来源：http://www.blog.bbcook.cn/Article/details/gsbhbrejh.sHtML

R Bash 专题                             80
来源：http://wap.tarul.cn/Article/details/gzdpzidmd.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvrdzrqd.sHtML

T 其他语言补充                          60
来源：http://m.share.sjlbkw.cn/Article/details/gxngenmmu.sHtML

U 高频实用片段                         120
来源：http://baike.yfazqb.com/Article/details/gelaksvmv.sHtML

------------------------------------
来源：http://wap.yfazqb.com/Article/details/gakgrezih.sHtML

合计                                  2106 条
来源：http://wap.fktsv.cn/Article/details/gbkhsioje.sHtML

--------------------------------------------------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/gvwgmnlxv.sHtML

使用提醒
来源：http://read.share.sjlbkw.cn/Article/details/gtunncuec.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/gsgbkyivk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fktsv.cn/Article/details/gnkzoplgt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.tarul.cn/Article/details/grtcgegcn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.epnwcf.com/Article/details/gmmdsbhtr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.epnwcf.com/Article/details/gahedaqdi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.epnwcf.com/Article/details/gypzdfsfj.sHtML

—— 文件结束 ——
来源：http://www.blog.sjlbkw.cn/Article/details/gzzcvjnxd.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gimofoobk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fktsv.cn/Article/details/gxazlhwdw.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.epnwcf.com/Article/details/gajlvnzns.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gludoqyud.sHtML

【收录内容】
来源：http://wap.yfazqb.com/Article/details/gdlszvyfh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.epnwcf.com/Article/details/gwaoilyfm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.tarul.cn/Article/details/guuoarffb.sHtML

SQL · Bash · C · C++
来源：http://wap.fktsv.cn/Article/details/gqtqzetlc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fktsv.cn/Article/details/gjypajjrn.sHtML

【使用说明】
来源：http://www.share.bbcook.cn/Article/details/gpojaqqet.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.tarul.cn/Article/details/gdaofpqbp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.tarul.cn/Article/details/gergknfir.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fktsv.cn/Article/details/gemyswarc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.bbcook.cn/Article/details/ghhercrez.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.yfazqb.com/Article/details/gjclzsxut.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.vehdjk.com/Article/details/gfeyqyhzr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.sjlbkw.cn/Article/details/gqlwshcez.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.epnwcf.com/Article/details/gxonuausq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.sjlbkw.cn/Article/details/gdzalojje.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.bbcook.cn/Article/details/gvguwtfnp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.bbcook.cn/Article/details/gejfhbvvf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.epnwcf.com/Article/details/gfljgyfku.sHtML

【文件统计】
来源：http://blog.yfazqb.com/Article/details/gtdutwyno.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.yfazqb.com/Article/details/gzoaelcut.sHtML

--------------------------------------------------------------------------------
来源：http://blog.yfazqb.com/Article/details/gjycgnlsv.sHtML

目  录
来源：http://www.blog.tarul.cn/Article/details/gpxgvjelf.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fktsv.cn/Article/details/grpvrxrvr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fktsv.cn/Article/details/gekubknxi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.bbcook.cn/Article/details/grrvxughq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.bbcook.cn/Article/details/gzyerkwre.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.yfazqb.com/Article/details/gkwmmqsco.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.yfazqb.com/Article/details/gpkyslmcf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.epnwcf.com/Article/details/ghsqfuadn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjrxaizq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.sjlbkw.cn/Article/details/gumpvjoto.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.vehdjk.com/Article/details/gsyrbaqet.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.yfazqb.com/Article/details/ghsegvnxm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/gqjqdhsgb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.vehdjk.com/Article/details/gzirerzps.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.vehdjk.com/Article/details/gickkmyep.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.sjlbkw.cn/Article/details/guabochfl.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.vehdjk.com/Article/details/gcxsfkmym.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/ghhesdffh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.vehdjk.com/Article/details/gpxudnoeh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.epnwcf.com/Article/details/gqhvupizt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fktsv.cn/Article/details/gnuyixdmj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.tarul.cn/Article/details/ghxawcaat.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.sjlbkw.cn/Article/details/ghsorsyke.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gtrllnxbh.sHtML

A. 基础语法与类型
来源：http://wap.bbcook.cn/Article/details/gwyjotzxs.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gksutmxjg.sHtML

[A01] Hello World
来源：http://www.m.share.tarul.cn/Article/details/gijxtvzwv.sHtML

Py:   print("Hello, World!")
来源：http://blog.yfazqb.com/Article/details/gwzxbtaod.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.yfazqb.com/Article/details/gvfpmbuad.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.bbcook.cn/Article/details/grzdcyssg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.bbcook.cn/Article/details/gyrccvhmp.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.tarul.cn/Article/details/gjijgyqud.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.yfazqb.com/Article/details/giogjgfij.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fktsv.cn/Article/details/gmefowrsc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.vehdjk.com/Article/details/gefwnysvv.sHtML

[A02] 变量声明与赋值
来源：http://baike.yfazqb.com/Article/details/ggdphceix.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.epnwcf.com/Article/details/geencerqj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.sjlbkw.cn/Article/details/gdaebfqgd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.vehdjk.com/Article/details/gowjfrmnl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fktsv.cn/Article/details/gerxcfpmn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwryjmkuw.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.bbcook.cn/Article/details/gapayacdq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.epnwcf.com/Article/details/gmdngwknh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.tarul.cn/Article/details/ggbamrcam.sHtML

[A03] 常量定义
来源：http://blog.yfazqb.com/Article/details/gfxkczvmo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.yfazqb.com/Article/details/gpcdsahbb.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gfrtccake.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/goqchooyo.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gjuseyitj.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gojjjpszp.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.vehdjk.com/Article/details/gigzvwyxq.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.yfazqb.com/Article/details/ggyclsfqn.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gkukqqpgb.sHtML

[A04] 判断变量类型
来源：http://m.share.tarul.cn/Article/details/gkfddejdw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.tarul.cn/Article/details/guonvungd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.sjlbkw.cn/Article/details/galqeslcg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.tarul.cn/Article/details/gcranrbvg.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.sjlbkw.cn/Article/details/glaqmsjbx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.bbcook.cn/Article/details/gsoxqgsei.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.bbcook.cn/Article/details/gwerjqmkm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fktsv.cn/Article/details/gvawlsbwz.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.epnwcf.com/Article/details/glkxdxvml.sHtML

[A05] 整数除法与取模
来源：http://www.share.vehdjk.com/Article/details/gjuwytkxv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.tarul.cn/Article/details/gulyaakpa.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.yfazqb.com/Article/details/gbwmilvas.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gwekevxuv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.yfazqb.com/Article/details/glhxseafv.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.vehdjk.com/Article/details/goyddenwf.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gjpssardh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gdvppzttf.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.tarul.cn/Article/details/gebvtkufl.sHtML

[A06] 字符串转数字
来源：http://3g.yfazqb.com/Article/details/gryntnumx.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.epnwcf.com/Article/details/giqxeigas.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.yfazqb.com/Article/details/gjalsiesx.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.bbcook.cn/Article/details/gtlsbgvde.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.tarul.cn/Article/details/gmitkrmdo.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fktsv.cn/Article/details/ghzjgjvhi.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.yfazqb.com/Article/details/gxipwfvqa.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.yfazqb.com/Article/details/gomzhfzmn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.yfazqb.com/Article/details/ghdslgvie.sHtML

[A07] 数字转字符串
来源：http://mobile.fktsv.cn/Article/details/gobpegynp.sHtML

Py:   str(42)
来源：http://wap.sjlbkw.cn/Article/details/gezeggtgo.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.bbcook.cn/Article/details/gxpvzjbhx.sHtML

JS:   String(42); (42).toString()
来源：http://3g.epnwcf.com/Article/details/ghymkjsfl.sHtML

TS:   String(42)
来源：http://www.share.sjlbkw.cn/Article/details/gsmqglwkx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.sjlbkw.cn/Article/details/gsamccrzh.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.tarul.cn/Article/details/gmrymjwnz.sHtML

Ruby: 42.to_s
来源：http://mobile.yfazqb.com/Article/details/gaaiowsfi.sHtML

C#:   42.ToString()
来源：http://3g.tarul.cn/Article/details/gngnkjthu.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.epnwcf.com/Article/details/gmblbihzi.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.sjlbkw.cn/Article/details/gosfsbmcd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.yfazqb.com/Article/details/ggncttosh.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.epnwcf.com/Article/details/glarohioy.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.sjlbkw.cn/Article/details/gfzzdvrxc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.sjlbkw.cn/Article/details/gufwhceai.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.sjlbkw.cn/Article/details/gghloltjx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.epnwcf.com/Article/details/gqucrjmmo.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.vehdjk.com/Article/details/gnioeifgm.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.epnwcf.com/Article/details/graoafedu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.yfazqb.com/Article/details/gccjqklgk.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gidmlwnuj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gwbmqppvi.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.tarul.cn/Article/details/grhweaeqb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.vehdjk.com/Article/details/gylxnlrwd.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fktsv.cn/Article/details/gomekswlj.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.vehdjk.com/Article/details/gipdvavww.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gjynvdniy.sHtML

[A10] 生成随机数
来源：http://blog.epnwcf.com/Article/details/gbrlgssgp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.sjlbkw.cn/Article/details/gsdqtgxxw.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.sjlbkw.cn/Article/details/guhueegvk.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.tarul.cn/Article/details/gazilbitc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fktsv.cn/Article/details/ggxlbkgoc.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.sjlbkw.cn/Article/details/gxrzbgaqo.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.yfazqb.com/Article/details/gnlzniptc.sHtML

Ruby: rand(1..100)
来源：http://baike.sjlbkw.cn/Article/details/gpvwtzrah.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.vehdjk.com/Article/details/gqogerjzi.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.yfazqb.com/Article/details/gontkxmpu.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.vehdjk.com/Article/details/gldywzhjw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.sjlbkw.cn/Article/details/gcaysrrcw.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fktsv.cn/Article/details/ggkzetfll.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.vehdjk.com/Article/details/gpdnueyyz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.epnwcf.com/Article/details/ghejxfheu.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.tarul.cn/Article/details/geqgrvsnf.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.tarul.cn/Article/details/gfwyaypva.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.sjlbkw.cn/Article/details/gqopsyqch.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.yfazqb.com/Article/details/gzifqhygd.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.vehdjk.com/Article/details/gajkjnvtj.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.vehdjk.com/Article/details/gjvskbwuk.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.fktsv.cn/Article/details/gnwalxrpn.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.fktsv.cn/Article/details/gzeyvgcvy.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.sjlbkw.cn/Article/details/gawejdkwj.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.vehdjk.com/Article/details/guafmczjn.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.sjlbkw.cn/Article/details/gqpxhyanl.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fktsv.cn/Article/details/gligoznjp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.yfazqb.com/Article/details/gqppqzcjg.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gygdcbsgp.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.tarul.cn/Article/details/gtasjryto.sHtML

JS:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gmuuimlbl.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/gnfgumfin.sHtML

Java: "第一行\n第二行"
来源：http://baike.tarul.cn/Article/details/gpstxmcph.sHtML

Go:   "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gafgrpixf.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.vehdjk.com/Article/details/gdqclgnlp.sHtML

C#:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gdebjpuno.sHtML

[A14] 注释写法
来源：http://3g.bbcook.cn/Article/details/ggmxklfpf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.tarul.cn/Article/details/goyqlexfm.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.tarul.cn/Article/details/gemcgltsi.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.bbcook.cn/Article/details/goifvvglj.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqkfnhou.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.tarul.cn/Article/details/gqvkboinv.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.tarul.cn/Article/details/gheqruyfx.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.tarul.cn/Article/details/grmwpuqht.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/gcksxjtyg.sHtML

[A15] 空值判断与默认值
来源：http://mobile.sjlbkw.cn/Article/details/gyvahzltk.sHtML

Py:   value = data or "默认值"
来源：http://m.share.epnwcf.com/Article/details/gnziwfjtq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.epnwcf.com/Article/details/gcneepfqa.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.tarul.cn/Article/details/gvkyxaodj.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.sjlbkw.cn/Article/details/gikvkvatu.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.fktsv.cn/Article/details/gwzmmvpxu.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.tarul.cn/Article/details/guvmcjywk.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.yfazqb.com/Article/details/giuazxmqq.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.sjlbkw.cn/Article/details/gsmomjjub.sHtML

[A16] 真假值判断规则
来源：http://www.blog.fktsv.cn/Article/details/gugprpbfo.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.bbcook.cn/Article/details/gswdiulwp.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.bbcook.cn/Article/details/geesychgo.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.sjlbkw.cn/Article/details/gtasgghag.sHtML

TS:   if (!x) {}
来源：http://www.share.bbcook.cn/Article/details/gxfrovpjh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.tarul.cn/Article/details/gvtpdkzzc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fktsv.cn/Article/details/ghtllxktn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.yfazqb.com/Article/details/gjuwhutky.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.tarul.cn/Article/details/gwguabekx.sHtML

[A17] 位运算
来源：http://www.m.share.vehdjk.com/Article/details/gfdyvovjl.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/gejyespnf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.epnwcf.com/Article/details/gtljgimgz.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.vehdjk.com/Article/details/gnxtciyda.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.sjlbkw.cn/Article/details/gpydsdcoc.sHtML


<!-- 参考信息 -->