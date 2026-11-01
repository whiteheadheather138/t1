代发 wailian999

[U99] JS：事件监听
来源：http://www.share.sjlbkw.cn/Article/details/gqcowkmle.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.epnwcf.com/Article/details/gdmgvyurq.sHtML

[U100] JS：DOM 查询
来源：http://mobile.bbcook.cn/Article/details/gkqrwqouk.sHtML

document.querySelector(".item")
来源：http://baike.epnwcf.com/Article/details/gadrwlrms.sHtML

[U101] JS：classList 操作
来源：http://baike.sjlbkw.cn/Article/details/gjmqvftmu.sHtML

el.classList.toggle("active")
来源：http://read.share.tarul.cn/Article/details/gubkgizxa.sHtML

[U102] JS：本地存储
来源：http://blog.vehdjk.com/Article/details/gujmjjpdw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.bbcook.cn/Article/details/gwbfgdbqr.sHtML

[U103] JS：定时器
来源：http://www.m.share.tarul.cn/Article/details/glvzkgenu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.yfazqb.com/Article/details/gvoukxbvd.sHtML

[U104] JS：防抖
来源：http://mobile.yfazqb.com/Article/details/gcuxpditj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gzhxtpftk.sHtML

[U105] JS：节流
来源：http://www.m.share.bbcook.cn/Article/details/gvkmpilmr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fktsv.cn/Article/details/gmohtchas.sHtML

[U106] JS：日期格式化
来源：http://mobile.fktsv.cn/Article/details/gcwqawaie.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.vehdjk.com/Article/details/gvpgvcmdg.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fktsv.cn/Article/details/gesquciww.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.epnwcf.com/Article/details/gcqnrzszj.sHtML

[U108] JS：随机整数
来源：http://www.m.share.yfazqb.com/Article/details/gvfspdmso.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.yfazqb.com/Article/details/gemeewwdr.sHtML

[U109] JS：数组分组
来源：http://read.share.bbcook.cn/Article/details/gabdnyeui.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fktsv.cn/Article/details/giefbesaw.sHtML

[U110] JS：数组分块
来源：http://m.share.yfazqb.com/Article/details/gtegivnnf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.epnwcf.com/Article/details/gqiftfabl.sHtML

[U111] JS：对象转 Map
来源：http://www.share.epnwcf.com/Article/details/gbvmrperl.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.vehdjk.com/Article/details/gqekamqcb.sHtML

[U112] JS：字符串补位
来源：http://m.share.yfazqb.com/Article/details/gdoleebdq.sHtML

"7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/grldwpfqc.sHtML

[U113] JS：正则替换全部
来源：http://read.share.yfazqb.com/Article/details/gidslpilc.sHtML

s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/grednpwgk.sHtML

[U114] JS：JSON 深比较
来源：http://3g.vehdjk.com/Article/details/gowubkurp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.yfazqb.com/Article/details/gcmsdivau.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.yfazqb.com/Article/details/gumkflixy.sHtML

crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/gqvlyfoto.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fktsv.cn/Article/details/gtdroqisx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.tarul.cn/Article/details/gjdgnbjyh.sHtML

[U117] JS：单元测试
来源：http://www.blog.sjlbkw.cn/Article/details/gpvgkxqsr.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.bbcook.cn/Article/details/gwivtdsci.sHtML

[U118] JS：开发服务器
来源：http://www.share.epnwcf.com/Article/details/gdvjydofk.sHtML

npm i -D vite;  npx vite
来源：http://mobile.yfazqb.com/Article/details/gzkvswyre.sHtML

[U119] JS：生产构建
来源：http://m.share.sjlbkw.cn/Article/details/gommvjtef.sHtML

npx vite build
来源：http://www.blog.epnwcf.com/Article/details/gwmttzfrb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.sjlbkw.cn/Article/details/grnmgexww.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.tarul.cn/Article/details/gwhjrntoh.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/guhbwhedt.sHtML

统计汇总
来源：http://www.m.share.epnwcf.com/Article/details/ghitgzuli.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkhctzvkq.sHtML

按语言统计（条）：
来源：http://baike.yfazqb.com/Article/details/gjsclnyem.sHtML

Python ......... 252
来源：http://baike.yfazqb.com/Article/details/gzryeruan.sHtML

PHP ............ 252
来源：http://www.blog.epnwcf.com/Article/details/gyadcgixu.sHtML

JavaScript ..... 252
来源：http://m.share.yfazqb.com/Article/details/gbazxtfuv.sHtML

TypeScript ..... 212
来源：http://read.share.tarul.cn/Article/details/gpdgnksqv.sHtML

Java ........... 212
来源：http://3g.vehdjk.com/Article/details/gedjdhbri.sHtML

Go ............. 212
来源：http://www.blog.vehdjk.com/Article/details/gopvrctwf.sHtML

Ruby ........... 212
来源：http://wap.vehdjk.com/Article/details/gfnipaojj.sHtML

C# ............. 212
来源：http://read.share.fktsv.cn/Article/details/gcyxohlbw.sHtML

C .............. 30
来源：http://mobile.fktsv.cn/Article/details/gurmwuvrr.sHtML

C++ ............ 30
来源：http://read.share.fktsv.cn/Article/details/gxtoiuekf.sHtML

SQL ............ 90
来源：http://www.m.share.sjlbkw.cn/Article/details/gasujvjos.sHtML

Bash ........... 80
来源：http://3g.sjlbkw.cn/Article/details/gczmsubwj.sHtML

Kotlin ......... 15
来源：http://m.share.fktsv.cn/Article/details/ggemekkkl.sHtML

Swift .......... 15
来源：http://www.blog.sjlbkw.cn/Article/details/gmegftfej.sHtML

Lua ............ 10
来源：http://blog.epnwcf.com/Article/details/gwnczebca.sHtML

Perl ........... 10
来源：http://baike.fktsv.cn/Article/details/gestnqcrz.sHtML

Scala .......... 10
来源：http://baike.epnwcf.com/Article/details/gbhrgfqjb.sHtML

------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/gkhnnqlov.sHtML

合计 ........... 2106 条
来源：http://mobile.sjlbkw.cn/Article/details/ggpsvbegn.sHtML

按章节统计：
来源：http://baike.epnwcf.com/Article/details/ghgexmxaj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.sjlbkw.cn/Article/details/gomfjyoxh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gxjzsxooi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.bbcook.cn/Article/details/gonklpovg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.epnwcf.com/Article/details/gsfbcpuze.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.sjlbkw.cn/Article/details/gajwjoajc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.vehdjk.com/Article/details/gswlgnqma.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.yfazqb.com/Article/details/guqjhjrwu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.sjlbkw.cn/Article/details/gqesjebox.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gdmwgybcq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.vehdjk.com/Article/details/gliuisgbx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.bbcook.cn/Article/details/geaegzien.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/gedsumzzz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/gflibjfwj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fktsv.cn/Article/details/glufgvohh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.tarul.cn/Article/details/geakosctr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gbqctpmpu.sHtML

Q SQL 专题                              90
来源：http://wap.vehdjk.com/Article/details/gtxszjhmk.sHtML

R Bash 专题                             80
来源：http://3g.vehdjk.com/Article/details/gqqtmankh.sHtML

S C / C++ 专题                          60
来源：http://www.share.fktsv.cn/Article/details/gqnwoanig.sHtML

T 其他语言补充                          60
来源：http://read.share.fktsv.cn/Article/details/gxbpcinko.sHtML

U 高频实用片段                         120
来源：http://m.share.epnwcf.com/Article/details/gvyblsifc.sHtML

------------------------------------
来源：http://read.share.vehdjk.com/Article/details/gfsuadhxc.sHtML

合计                                  2106 条
来源：http://www.blog.tarul.cn/Article/details/gqlvgqizd.sHtML

--------------------------------------------------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gcvehcvnv.sHtML

使用提醒
来源：http://mobile.vehdjk.com/Article/details/gobpcmgmu.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gbkgpkltp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.vehdjk.com/Article/details/gkxsbvqyx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.vehdjk.com/Article/details/guordatqc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.sjlbkw.cn/Article/details/gekxloopq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.epnwcf.com/Article/details/gmzyuznbw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fktsv.cn/Article/details/gwvkjaakp.sHtML

—— 文件结束 ——
来源：http://www.m.share.bbcook.cn/Article/details/gngkxqtxh.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gweinvxse.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.vehdjk.com/Article/details/gqgitfbmu.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.bbcook.cn/Article/details/ggdgobcjx.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gsottitzz.sHtML

【收录内容】
来源：http://3g.epnwcf.com/Article/details/gwxgqhibs.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.tarul.cn/Article/details/gqrknaygc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.yfazqb.com/Article/details/ghvljmwqv.sHtML

SQL · Bash · C · C++
来源：http://mobile.epnwcf.com/Article/details/gusuicjvp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.bbcook.cn/Article/details/gnqqtbmva.sHtML

【使用说明】
来源：http://www.share.fktsv.cn/Article/details/gcqdhejkz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.vehdjk.com/Article/details/gohpwumlo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.sjlbkw.cn/Article/details/giwwoqccy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.epnwcf.com/Article/details/gvjgoaufj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.bbcook.cn/Article/details/gnnvahmce.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.epnwcf.com/Article/details/ggfkgcupe.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.sjlbkw.cn/Article/details/gmyfxukef.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.sjlbkw.cn/Article/details/geubcptlw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.sjlbkw.cn/Article/details/gwwnffmsv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.yfazqb.com/Article/details/gqugwiasm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.epnwcf.com/Article/details/gweaxknqa.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.sjlbkw.cn/Article/details/gcwsnykei.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.sjlbkw.cn/Article/details/ggivrlbdu.sHtML

【文件统计】
来源：http://blog.fktsv.cn/Article/details/gnlphsaxz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.yfazqb.com/Article/details/guvaooatn.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/giobsuvsz.sHtML

目  录
来源：http://read.share.bbcook.cn/Article/details/gjnrlckgd.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.tarul.cn/Article/details/ghcoekldn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.tarul.cn/Article/details/gqbckxebb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.bbcook.cn/Article/details/gfszjfxdr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.bbcook.cn/Article/details/gyjswkhvj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.yfazqb.com/Article/details/gkfqgbjlu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.tarul.cn/Article/details/grdawvpks.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.tarul.cn/Article/details/gbctjxgkm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.tarul.cn/Article/details/gziskujjk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.yfazqb.com/Article/details/grwgxqmpv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/gudxjkunv.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.yfazqb.com/Article/details/gxativcor.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/gnljrctfx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.bbcook.cn/Article/details/gyybvftvt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.bbcook.cn/Article/details/ggbwichwc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.vehdjk.com/Article/details/glkjwofbn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.sjlbkw.cn/Article/details/gvqeyceyx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.bbcook.cn/Article/details/ggocxeiao.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.sjlbkw.cn/Article/details/gzjxsotxg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.yfazqb.com/Article/details/gedcjjhcg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.bbcook.cn/Article/details/gkbrtnsmy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.vehdjk.com/Article/details/gpkhtbieg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.vehdjk.com/Article/details/gibcglism.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gftctyreq.sHtML

A. 基础语法与类型
来源：http://www.share.epnwcf.com/Article/details/grznrdscx.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gahygtllh.sHtML

[A01] Hello World
来源：http://wap.epnwcf.com/Article/details/ggfuncmuy.sHtML

Py:   print("Hello, World!")
来源：http://mobile.yfazqb.com/Article/details/gsnzhyevd.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.tarul.cn/Article/details/gerjqbfog.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.tarul.cn/Article/details/gtxnvsxpb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.epnwcf.com/Article/details/gadpidjjx.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.vehdjk.com/Article/details/gihglyexu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fktsv.cn/Article/details/gogqlakis.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.yfazqb.com/Article/details/gazqrtcxr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.vehdjk.com/Article/details/gsmdkznpa.sHtML

[A02] 变量声明与赋值
来源：http://wap.fktsv.cn/Article/details/gietpftwa.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.sjlbkw.cn/Article/details/gmxucfige.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fktsv.cn/Article/details/gkvpiwslv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.yfazqb.com/Article/details/gumxiqztn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.bbcook.cn/Article/details/glhxskzil.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.bbcook.cn/Article/details/ggjrikblp.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.vehdjk.com/Article/details/gqrfrysxt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.epnwcf.com/Article/details/gjjsojxax.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fktsv.cn/Article/details/gmcuxapbm.sHtML

[A03] 常量定义
来源：http://www.blog.fktsv.cn/Article/details/gxwmmvvro.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.epnwcf.com/Article/details/gulxkqmlz.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gdyqnayor.sHtML

JS:   const PI = 3.14159;
来源：http://3g.yfazqb.com/Article/details/gwhwnzxxo.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gikhtfuha.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gsduobnzr.sHtML

Go:   const PI = 3.14159
来源：http://wap.yfazqb.com/Article/details/gfqzirwef.sHtML

Ruby: PI = 3.14159
来源：http://mobile.yfazqb.com/Article/details/gvlslkxmk.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gsrabodyn.sHtML

[A04] 判断变量类型
来源：http://blog.yfazqb.com/Article/details/gmwnhiyxk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.bbcook.cn/Article/details/gulyabsgs.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.tarul.cn/Article/details/gwxpktwmr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.bbcook.cn/Article/details/gpslsudhw.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.sjlbkw.cn/Article/details/giythhdhk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.bbcook.cn/Article/details/gykgozfqw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.sjlbkw.cn/Article/details/gqknhdrjo.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.epnwcf.com/Article/details/gbtjszfap.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.tarul.cn/Article/details/grtsbxewu.sHtML

[A05] 整数除法与取模
来源：http://wap.fktsv.cn/Article/details/ggrbeiegi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fktsv.cn/Article/details/gfvxhxwdx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gniozhcfx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.epnwcf.com/Article/details/grugrpnue.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.vehdjk.com/Article/details/grmyhwxzf.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.yfazqb.com/Article/details/gvmwalzva.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gykfcyzbk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gzzafmqne.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.tarul.cn/Article/details/gewmrdnzf.sHtML

[A06] 字符串转数字
来源：http://m.share.fktsv.cn/Article/details/gaoomdlwy.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fktsv.cn/Article/details/glbtevsds.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.bbcook.cn/Article/details/gurobhssg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.bbcook.cn/Article/details/gwontljcf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.sjlbkw.cn/Article/details/gylkggywy.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.yfazqb.com/Article/details/grxrhezuk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fktsv.cn/Article/details/gtssdbkne.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.sjlbkw.cn/Article/details/gwrabavyu.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fktsv.cn/Article/details/gtnicpvet.sHtML

[A07] 数字转字符串
来源：http://blog.fktsv.cn/Article/details/gpicyaqkw.sHtML

Py:   str(42)
来源：http://www.share.sjlbkw.cn/Article/details/gpshzgqac.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.vehdjk.com/Article/details/gzhwmpxcr.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.vehdjk.com/Article/details/gwpefjfrh.sHtML

TS:   String(42)
来源：http://3g.bbcook.cn/Article/details/gzhvvpfsr.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.vehdjk.com/Article/details/gmgxvaggx.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.sjlbkw.cn/Article/details/gelyehgxa.sHtML

Ruby: 42.to_s
来源：http://www.blog.bbcook.cn/Article/details/gzpniojhq.sHtML

C#:   42.ToString()
来源：http://read.share.yfazqb.com/Article/details/gdjqdkkss.sHtML

[A08] 取整与四舍五入
来源：http://baike.epnwcf.com/Article/details/gvjbnnwil.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.tarul.cn/Article/details/gjjhazwhm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.epnwcf.com/Article/details/gwiduakbq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.fktsv.cn/Article/details/gfkijolyn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbsqorqt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.sjlbkw.cn/Article/details/gfcbptshe.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.bbcook.cn/Article/details/gtiijmepb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.tarul.cn/Article/details/gouklepbm.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.yfazqb.com/Article/details/gljnhijmu.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gighragec.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.bbcook.cn/Article/details/gqomahvsr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gavpsufnt.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gsqjagfic.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gtbjuwyms.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.yfazqb.com/Article/details/gzcehxpli.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fktsv.cn/Article/details/gddeiemuv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.vehdjk.com/Article/details/gpdeuktdk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.vehdjk.com/Article/details/gxbkkngiz.sHtML

[A10] 生成随机数
来源：http://wap.vehdjk.com/Article/details/glecelmsc.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.bbcook.cn/Article/details/grqgayfby.sHtML

PHP:  random_int(1, 100);
来源：http://blog.vehdjk.com/Article/details/gdokvgjyw.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.tarul.cn/Article/details/gpqmpmwsd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.tarul.cn/Article/details/gnbddjgdx.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.sjlbkw.cn/Article/details/gyxwupxlv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.tarul.cn/Article/details/gifycevdb.sHtML

Ruby: rand(1..100)
来源：http://m.share.yfazqb.com/Article/details/gljfqnjhz.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.yfazqb.com/Article/details/gdefwahsm.sHtML

[A11] 条件表达式（三元）
来源：http://wap.fktsv.cn/Article/details/gjtygqrsf.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.tarul.cn/Article/details/grobpzyoi.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/gqcgnjupd.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.vehdjk.com/Article/details/ggdlkbttg.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.epnwcf.com/Article/details/goabhrdkt.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.epnwcf.com/Article/details/gvccofxhx.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.sjlbkw.cn/Article/details/giobzvlfa.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.epnwcf.com/Article/details/genfygwnm.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.epnwcf.com/Article/details/gtuzgqflt.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.yfazqb.com/Article/details/gxabfqjxn.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.bbcook.cn/Article/details/ggnutrzcg.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.bbcook.cn/Article/details/gajgmtfzo.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.tarul.cn/Article/details/ghbwzpgko.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.epnwcf.com/Article/details/gixlpdoih.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.tarul.cn/Article/details/gfkzyrpmz.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.tarul.cn/Article/details/gsmpxuyqr.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.bbcook.cn/Article/details/gwjujqcwf.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.epnwcf.com/Article/details/grljrcfvx.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.vehdjk.com/Article/details/gplzkzfuj.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/ghlxahcey.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/glsqcecip.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gusxccjxw.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.vehdjk.com/Article/details/gayyfvsir.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.vehdjk.com/Article/details/gifetacwv.sHtML

Go:   "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gyjrkykhg.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gtacyvtlq.sHtML

C#:   "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/gkklxsgtx.sHtML

[A14] 注释写法
来源：http://read.share.epnwcf.com/Article/details/gudyakeay.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.tarul.cn/Article/details/gxfwotygg.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.tarul.cn/Article/details/ggxkvzccw.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.sjlbkw.cn/Article/details/gkujnvyco.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/gabrqhjod.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.sjlbkw.cn/Article/details/gymvbwxsb.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.epnwcf.com/Article/details/giafjbmgy.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.sjlbkw.cn/Article/details/gsymrdohb.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.yfazqb.com/Article/details/gvdufzvcu.sHtML

[A15] 空值判断与默认值
来源：http://blog.epnwcf.com/Article/details/gitqbszvs.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.bbcook.cn/Article/details/gulirgtra.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.tarul.cn/Article/details/gkrexyxky.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.vehdjk.com/Article/details/gonxmdujl.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.sjlbkw.cn/Article/details/gwwqtguss.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.tarul.cn/Article/details/ghtciuhtj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.yfazqb.com/Article/details/gqkwagpht.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.tarul.cn/Article/details/gyyafwixl.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.bbcook.cn/Article/details/gwvtxtayy.sHtML

[A16] 真假值判断规则
来源：http://mobile.bbcook.cn/Article/details/gzrkgzbax.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.sjlbkw.cn/Article/details/gqjyaazzi.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.vehdjk.com/Article/details/grunzssbd.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.vehdjk.com/Article/details/gjokzfktf.sHtML

TS:   if (!x) {}
来源：http://read.share.epnwcf.com/Article/details/gqsyleref.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gqcjehebh.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.yfazqb.com/Article/details/gjnzovyzx.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.epnwcf.com/Article/details/giuzynvsq.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.yfazqb.com/Article/details/gzuustqcb.sHtML

[A17] 位运算
来源：http://www.share.sjlbkw.cn/Article/details/glivvtfya.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/gwebhryom.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.vehdjk.com/Article/details/guwzuqtsl.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.sjlbkw.cn/Article/details/grigpoupm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gcoyprxut.sHtML


<!-- 参考信息 -->