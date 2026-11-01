代发 wailian999

[U101] JS：classList 操作
来源：http://m.share.epnwcf.com/Article/details/gdtqprgqs.sHtML

el.classList.toggle("active")
来源：http://m.share.sjlbkw.cn/Article/details/gqnkcgrmj.sHtML

[U102] JS：本地存储
来源：http://www.blog.sjlbkw.cn/Article/details/gqwadwbaw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.epnwcf.com/Article/details/gkzctuukl.sHtML

[U103] JS：定时器
来源：http://wap.bbcook.cn/Article/details/gtconjrdm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.bbcook.cn/Article/details/gbaeyvyzh.sHtML

[U104] JS：防抖
来源：http://www.share.yfazqb.com/Article/details/goyyitsph.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/gbddhfmsz.sHtML

[U105] JS：节流
来源：http://3g.fktsv.cn/Article/details/gkbwhbfzg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.sjlbkw.cn/Article/details/gytzyafor.sHtML

[U106] JS：日期格式化
来源：http://wap.tarul.cn/Article/details/gnfwnyxeo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fktsv.cn/Article/details/gwxlwglqz.sHtML

[U107] JS：数字千分位
来源：http://baike.sjlbkw.cn/Article/details/grouyuidi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.tarul.cn/Article/details/gqwmdjsei.sHtML

[U108] JS：随机整数
来源：http://www.share.sjlbkw.cn/Article/details/goipetlrp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.tarul.cn/Article/details/gaumtxuqa.sHtML

[U109] JS：数组分组
来源：http://read.share.yfazqb.com/Article/details/gzwbcfpmk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fktsv.cn/Article/details/gqqkmszno.sHtML

[U110] JS：数组分块
来源：http://m.share.fktsv.cn/Article/details/gvstpemtk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.yfazqb.com/Article/details/gmccletdi.sHtML

[U111] JS：对象转 Map
来源：http://3g.bbcook.cn/Article/details/gxchnzfzu.sHtML

new Map(Object.entries(obj))
来源：http://3g.sjlbkw.cn/Article/details/gnnwktflz.sHtML

[U112] JS：字符串补位
来源：http://read.share.bbcook.cn/Article/details/gqezvhnkj.sHtML

"7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gadxklrnx.sHtML

[U113] JS：正则替换全部
来源：http://3g.vehdjk.com/Article/details/gocbbpsqr.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/goziducqs.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.vehdjk.com/Article/details/gejepluej.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.yfazqb.com/Article/details/gguxohnbq.sHtML

[U115] JS：生成 UUID
来源：http://3g.epnwcf.com/Article/details/gzdwxggqo.sHtML

crypto.randomUUID()
来源：http://www.blog.vehdjk.com/Article/details/glygbigah.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.vehdjk.com/Article/details/gqotkcitj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gseyycbus.sHtML

[U117] JS：单元测试
来源：http://3g.yfazqb.com/Article/details/gwetbrdsj.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.bbcook.cn/Article/details/guqrcshvv.sHtML

[U118] JS：开发服务器
来源：http://www.share.bbcook.cn/Article/details/ghgajryom.sHtML

npm i -D vite;  npx vite
来源：http://www.share.bbcook.cn/Article/details/geaduoqnx.sHtML

[U119] JS：生产构建
来源：http://www.share.sjlbkw.cn/Article/details/gitqxygxc.sHtML

npx vite build
来源：http://baike.fktsv.cn/Article/details/gmpdwzyfi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.epnwcf.com/Article/details/gaavtccpn.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.epnwcf.com/Article/details/gbokbwbzw.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/grqmbggip.sHtML

统计汇总
来源：http://mobile.epnwcf.com/Article/details/geqryqbie.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gtqbrqqpp.sHtML

按语言统计（条）：
来源：http://mobile.vehdjk.com/Article/details/gjotcdpfp.sHtML

Python ......... 252
来源：http://baike.tarul.cn/Article/details/gtcoaoeqz.sHtML

PHP ............ 252
来源：http://mobile.fktsv.cn/Article/details/gtuprumlf.sHtML

JavaScript ..... 252
来源：http://3g.bbcook.cn/Article/details/gvzdpuada.sHtML

TypeScript ..... 212
来源：http://wap.bbcook.cn/Article/details/gcuipjusj.sHtML

Java ........... 212
来源：http://mobile.epnwcf.com/Article/details/guvvfvigz.sHtML

Go ............. 212
来源：http://blog.vehdjk.com/Article/details/gnbyucdka.sHtML

Ruby ........... 212
来源：http://baike.tarul.cn/Article/details/ggfljzzdy.sHtML

C# ............. 212
来源：http://mobile.bbcook.cn/Article/details/gtlcwzdic.sHtML

C .............. 30
来源：http://www.blog.yfazqb.com/Article/details/gsdzztpyb.sHtML

C++ ............ 30
来源：http://wap.bbcook.cn/Article/details/gvhzmopfs.sHtML

SQL ............ 90
来源：http://wap.yfazqb.com/Article/details/gbfvnjcgr.sHtML

Bash ........... 80
来源：http://www.share.vehdjk.com/Article/details/gjxcsysss.sHtML

Kotlin ......... 15
来源：http://www.blog.tarul.cn/Article/details/girklpxcc.sHtML

Swift .......... 15
来源：http://blog.fktsv.cn/Article/details/ghvuqrcvx.sHtML

Lua ............ 10
来源：http://wap.yfazqb.com/Article/details/gkqgdtnch.sHtML

Perl ........... 10
来源：http://baike.fktsv.cn/Article/details/gwphbxnyd.sHtML

Scala .......... 10
来源：http://www.blog.bbcook.cn/Article/details/ghyhsrlgr.sHtML

------------------------------------
来源：http://blog.fktsv.cn/Article/details/glbrnvbzq.sHtML

合计 ........... 2106 条
来源：http://wap.tarul.cn/Article/details/gcxxpnezm.sHtML

按章节统计：
来源：http://www.blog.bbcook.cn/Article/details/glwrizorj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.yfazqb.com/Article/details/gpgwjfnto.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.bbcook.cn/Article/details/grzvxcqxl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.vehdjk.com/Article/details/gyhkfrwum.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.tarul.cn/Article/details/gngpyxkep.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.tarul.cn/Article/details/giaupnoov.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.epnwcf.com/Article/details/ghcoqjcvr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fktsv.cn/Article/details/glxqekwcw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.vehdjk.com/Article/details/gwanuqhtb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gqgslfzdl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.tarul.cn/Article/details/gmtgnyxdz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/glamnwpuw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/gtwkzykjl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gedymedqy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.yfazqb.com/Article/details/gwbytednv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.sjlbkw.cn/Article/details/gslvkrkvy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/gimxebxoq.sHtML

Q SQL 专题                              90
来源：http://m.share.bbcook.cn/Article/details/gjehostdw.sHtML

R Bash 专题                             80
来源：http://www.blog.sjlbkw.cn/Article/details/gzwaomvpq.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fktsv.cn/Article/details/grtuogchn.sHtML

T 其他语言补充                          60
来源：http://wap.yfazqb.com/Article/details/gnnnxaakr.sHtML

U 高频实用片段                         120
来源：http://3g.yfazqb.com/Article/details/gricnothw.sHtML

------------------------------------
来源：http://wap.vehdjk.com/Article/details/gvmmazruz.sHtML

合计                                  2106 条
来源：http://www.share.tarul.cn/Article/details/giztvmfmw.sHtML

--------------------------------------------------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gikesjnzs.sHtML

使用提醒
来源：http://baike.yfazqb.com/Article/details/ghcschbql.sHtML

--------------------------------------------------------------------------------
来源：http://3g.vehdjk.com/Article/details/gyzxzcubo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fktsv.cn/Article/details/ggtrgewed.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.sjlbkw.cn/Article/details/glmssbnkx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fktsv.cn/Article/details/gzpjhekgz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fktsv.cn/Article/details/glkxvqjot.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fktsv.cn/Article/details/gktmtftec.sHtML

—— 文件结束 ——
来源：http://www.share.tarul.cn/Article/details/gxnkxoujw.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gyczwpumb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.sjlbkw.cn/Article/details/gvvseluoc.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.tarul.cn/Article/details/gqjefjxrq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gkpmqfhqd.sHtML

【收录内容】
来源：http://blog.bbcook.cn/Article/details/gkhutcuon.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.vehdjk.com/Article/details/gqzvjqijt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.epnwcf.com/Article/details/gjbyqdxiv.sHtML

SQL · Bash · C · C++
来源：http://read.share.epnwcf.com/Article/details/gsmorrzwm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.sjlbkw.cn/Article/details/gqmwvovhy.sHtML

【使用说明】
来源：http://blog.bbcook.cn/Article/details/gljhzznrb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.bbcook.cn/Article/details/gazevuvtz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.tarul.cn/Article/details/gcgogxylo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.epnwcf.com/Article/details/gmuowaakq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.epnwcf.com/Article/details/gufcrtalu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.epnwcf.com/Article/details/gizpyswpv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.tarul.cn/Article/details/gxtcksshw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.yfazqb.com/Article/details/gyvhmchro.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.vehdjk.com/Article/details/gnxpkccgc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.yfazqb.com/Article/details/geyzspwqw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.tarul.cn/Article/details/gancpqwst.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.yfazqb.com/Article/details/gngeskhtx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.yfazqb.com/Article/details/gxquvzdxl.sHtML

【文件统计】
来源：http://www.blog.vehdjk.com/Article/details/ggwfxlxzo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.tarul.cn/Article/details/gkgyetjbk.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gqgehhtgn.sHtML

目  录
来源：http://wap.bbcook.cn/Article/details/gtgrsuwsn.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.vehdjk.com/Article/details/gblxrhyec.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.vehdjk.com/Article/details/gjdcqapys.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/goczzfhbo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.yfazqb.com/Article/details/gexgtlhyr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fktsv.cn/Article/details/ghurneqwg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fktsv.cn/Article/details/gttdzaywv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.tarul.cn/Article/details/gqwvpdipj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.bbcook.cn/Article/details/gfibqwjds.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fktsv.cn/Article/details/gwslnotfw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fktsv.cn/Article/details/guzbijuck.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.sjlbkw.cn/Article/details/gmyejvamh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.epnwcf.com/Article/details/gyejfgycc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/gbkrvxndg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/ghkqervjc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.yfazqb.com/Article/details/giqybklcd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.vehdjk.com/Article/details/gxvlyyjnu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.epnwcf.com/Article/details/gwmyuqsff.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.tarul.cn/Article/details/gaxvsjfvr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.epnwcf.com/Article/details/gnqmxxunf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.yfazqb.com/Article/details/ggycwiuga.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.epnwcf.com/Article/details/gzohdfens.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.tarul.cn/Article/details/gslvetcon.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gwqkvneur.sHtML

A. 基础语法与类型
来源：http://3g.vehdjk.com/Article/details/gjamsuwco.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/guqkxjkvf.sHtML

[A01] Hello World
来源：http://www.share.yfazqb.com/Article/details/gpmowfwtk.sHtML

Py:   print("Hello, World!")
来源：http://3g.tarul.cn/Article/details/gwmmsdlzn.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.tarul.cn/Article/details/gonibnrtm.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.tarul.cn/Article/details/geocghbfb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.epnwcf.com/Article/details/grpzhgnlu.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fktsv.cn/Article/details/gzfulvhvo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fktsv.cn/Article/details/gwkocynac.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.bbcook.cn/Article/details/gvnabkpjx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.tarul.cn/Article/details/gtujeunfi.sHtML

[A02] 变量声明与赋值
来源：http://blog.bbcook.cn/Article/details/gmodcuats.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.yfazqb.com/Article/details/ggqqwwmxl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.bbcook.cn/Article/details/gwenimwbt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.vehdjk.com/Article/details/gxemgaauz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gzlejkfei.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.epnwcf.com/Article/details/gnrwibjkd.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.vehdjk.com/Article/details/gbdrrqwss.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.epnwcf.com/Article/details/gaoaaktub.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/gfjrfbier.sHtML

[A03] 常量定义
来源：http://blog.yfazqb.com/Article/details/guhwmvjgn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.sjlbkw.cn/Article/details/glhxjvitq.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gfsxtgjla.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gdzbwzgfh.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gcyyoenos.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gspjyuvip.sHtML

Go:   const PI = 3.14159
来源：http://baike.yfazqb.com/Article/details/grryolrqq.sHtML

Ruby: PI = 3.14159
来源：http://read.share.vehdjk.com/Article/details/ghglfnpdz.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gyrasvfdj.sHtML

[A04] 判断变量类型
来源：http://m.share.tarul.cn/Article/details/gyxpmamyn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.yfazqb.com/Article/details/gpeqsrlpr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.bbcook.cn/Article/details/giozxawcs.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.sjlbkw.cn/Article/details/griagvptq.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.sjlbkw.cn/Article/details/gkxfmrckg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fktsv.cn/Article/details/gdiguckby.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.bbcook.cn/Article/details/gvszcatwe.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.bbcook.cn/Article/details/gnxoupqxt.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.yfazqb.com/Article/details/gelyjmpwl.sHtML

[A05] 整数除法与取模
来源：http://3g.epnwcf.com/Article/details/ggbubkosa.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.sjlbkw.cn/Article/details/gsucgwnpb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.bbcook.cn/Article/details/gxzoxbxpn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.sjlbkw.cn/Article/details/gzbirfwqv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.bbcook.cn/Article/details/gnkddmdfv.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/gavsfaqdb.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.epnwcf.com/Article/details/gavqsqcer.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gfqfcssts.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fktsv.cn/Article/details/gbptwzeom.sHtML

[A06] 字符串转数字
来源：http://www.share.yfazqb.com/Article/details/gmjqpgwox.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.epnwcf.com/Article/details/gteqwdcct.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.sjlbkw.cn/Article/details/glilbhvrs.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.sjlbkw.cn/Article/details/gkvikzifw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.epnwcf.com/Article/details/gcgphwkxt.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.vehdjk.com/Article/details/gujdhhtle.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.tarul.cn/Article/details/gcnhvyzjw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.vehdjk.com/Article/details/gkxdfzdhd.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.sjlbkw.cn/Article/details/ghwldcjwi.sHtML

[A07] 数字转字符串
来源：http://baike.fktsv.cn/Article/details/glxxwgdvv.sHtML

Py:   str(42)
来源：http://m.share.bbcook.cn/Article/details/gktocevwr.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.sjlbkw.cn/Article/details/gquqisajs.sHtML

JS:   String(42); (42).toString()
来源：http://baike.tarul.cn/Article/details/gvzgxgkrk.sHtML

TS:   String(42)
来源：http://www.share.epnwcf.com/Article/details/gedtanwuy.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.epnwcf.com/Article/details/grqjitxgb.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.epnwcf.com/Article/details/gglielypv.sHtML

Ruby: 42.to_s
来源：http://m.share.bbcook.cn/Article/details/glkyjcoxn.sHtML

C#:   42.ToString()
来源：http://3g.tarul.cn/Article/details/gbxqzuzvq.sHtML

[A08] 取整与四舍五入
来源：http://wap.bbcook.cn/Article/details/gcmsggngc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.bbcook.cn/Article/details/gtfdyokxr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.sjlbkw.cn/Article/details/gnnknoodm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fktsv.cn/Article/details/gpdefoucm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.tarul.cn/Article/details/gjqpmswyd.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/gskcwftma.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.yfazqb.com/Article/details/gldmoyqlb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.epnwcf.com/Article/details/gnedzdmrg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.bbcook.cn/Article/details/gblumrlyy.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.sjlbkw.cn/Article/details/gvpfotiqp.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gllrxggex.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.yfazqb.com/Article/details/gnjonjxgi.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.bbcook.cn/Article/details/gbewyiqti.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.epnwcf.com/Article/details/gsexxdjwi.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.tarul.cn/Article/details/gocvvctth.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fktsv.cn/Article/details/gkdhfhzft.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.bbcook.cn/Article/details/gybkrjugz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gpirbmupk.sHtML

[A10] 生成随机数
来源：http://baike.epnwcf.com/Article/details/ggemzoyud.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.epnwcf.com/Article/details/gdiyshxlj.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.epnwcf.com/Article/details/guydipqry.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.bbcook.cn/Article/details/gqqlioomx.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.vehdjk.com/Article/details/gpodhylrx.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.sjlbkw.cn/Article/details/ggpgydrdw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.tarul.cn/Article/details/gpuguylev.sHtML

Ruby: rand(1..100)
来源：http://m.share.epnwcf.com/Article/details/gjmesnmcc.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.sjlbkw.cn/Article/details/gbnylvdyg.sHtML

[A11] 条件表达式（三元）
来源：http://3g.tarul.cn/Article/details/glnmjzqii.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.fktsv.cn/Article/details/gvkebyxrj.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.epnwcf.com/Article/details/gskjojtpx.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.sjlbkw.cn/Article/details/ggkszjjqm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.fktsv.cn/Article/details/gjzppxova.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.yfazqb.com/Article/details/gvltyprxg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.tarul.cn/Article/details/gjhljuguh.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.vehdjk.com/Article/details/gacyireva.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.fktsv.cn/Article/details/gtrcpjkxk.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.vehdjk.com/Article/details/gzaclzfjk.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.bbcook.cn/Article/details/geoeazxxc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.vehdjk.com/Article/details/gwxpyhvxg.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.fktsv.cn/Article/details/gjqukuaiu.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.tarul.cn/Article/details/gvtknjfkg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.yfazqb.com/Article/details/gcywzzlwn.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.tarul.cn/Article/details/gxlkspbmf.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.tarul.cn/Article/details/glvlpjlff.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.vehdjk.com/Article/details/gvhhkmlrr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.yfazqb.com/Article/details/gcckcdudl.sHtML

Py:   "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/giuubunvh.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/gpkgrnofk.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/guxfrsdmi.sHtML

TS:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gzxyoqzjv.sHtML

Java: "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/gumjtarvi.sHtML

Go:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gywhpwixm.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gwbcwnvmx.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.tarul.cn/Article/details/gvinjudrq.sHtML

[A14] 注释写法
来源：http://blog.tarul.cn/Article/details/gicixhjhr.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.tarul.cn/Article/details/gkefwutds.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.yfazqb.com/Article/details/gefdudtlz.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.yfazqb.com/Article/details/gnemquqdf.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fktsv.cn/Article/details/gnmkzlylt.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.bbcook.cn/Article/details/gxepixfkp.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/gikffjqzh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.epnwcf.com/Article/details/ghfrltzsd.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.sjlbkw.cn/Article/details/govbeinez.sHtML

[A15] 空值判断与默认值
来源：http://mobile.bbcook.cn/Article/details/gmnnlcubg.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fktsv.cn/Article/details/gsqwrtjwy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.vehdjk.com/Article/details/gxifjiqap.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.vehdjk.com/Article/details/gsbhgzler.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.epnwcf.com/Article/details/giqevfnhw.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.bbcook.cn/Article/details/gqznhkqaw.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.yfazqb.com/Article/details/gwblqasla.sHtML

Ruby: value = data || "默认值"
来源：http://baike.tarul.cn/Article/details/guspkedgt.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.yfazqb.com/Article/details/gcjpbscqv.sHtML

[A16] 真假值判断规则
来源：http://www.share.yfazqb.com/Article/details/gvtvvicfo.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.sjlbkw.cn/Article/details/glmzyitka.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.epnwcf.com/Article/details/guiyyxemy.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.vehdjk.com/Article/details/gyuzfigmm.sHtML

TS:   if (!x) {}
来源：http://www.share.yfazqb.com/Article/details/gvbqdmyib.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.epnwcf.com/Article/details/gogjyfwdf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.sjlbkw.cn/Article/details/gkvupgntz.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.epnwcf.com/Article/details/gjeouuaox.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.yfazqb.com/Article/details/gwnmtnlvk.sHtML

[A17] 位运算
来源：http://www.m.share.fktsv.cn/Article/details/gizcjzdep.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/gqmwjdemr.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.vehdjk.com/Article/details/gfszbtwzt.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/gfxmnpmuw.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/gdkwzijzo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gqfpyzrlh.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gqbsgaejt.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/grarxukrs.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gkwldjzoq.sHtML


<!-- 参考信息 -->