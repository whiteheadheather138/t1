代发 wailian999

[U99] JS：事件监听
来源：http://read.share.tarul.cn/Article/details/gftataurx.sHtML

el.addEventListener("click", e => {})
来源：http://3g.bbcook.cn/Article/details/gygzktkch.sHtML

[U100] JS：DOM 查询
来源：http://3g.bbcook.cn/Article/details/gudktetzz.sHtML

document.querySelector(".item")
来源：http://wap.sjlbkw.cn/Article/details/gcuqyhbfx.sHtML

[U101] JS：classList 操作
来源：http://www.blog.yfazqb.com/Article/details/gazmbighs.sHtML

el.classList.toggle("active")
来源：http://www.blog.epnwcf.com/Article/details/gqmveavps.sHtML

[U102] JS：本地存储
来源：http://read.share.vehdjk.com/Article/details/glmhiggkw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.sjlbkw.cn/Article/details/gidrtjiac.sHtML

[U103] JS：定时器
来源：http://baike.vehdjk.com/Article/details/gpmysftxu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.tarul.cn/Article/details/gtkwizbez.sHtML

[U104] JS：防抖
来源：http://wap.epnwcf.com/Article/details/geytprdjy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fktsv.cn/Article/details/gbpsiwwxx.sHtML

[U105] JS：节流
来源：http://mobile.yfazqb.com/Article/details/gehdafxxd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fktsv.cn/Article/details/gffmwqndw.sHtML

[U106] JS：日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/gvwnbumcc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.yfazqb.com/Article/details/gtgjvmwaf.sHtML

[U107] JS：数字千分位
来源：http://www.share.vehdjk.com/Article/details/geooiylty.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.sjlbkw.cn/Article/details/gxshyzzax.sHtML

[U108] JS：随机整数
来源：http://baike.vehdjk.com/Article/details/gjrzrgylc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.yfazqb.com/Article/details/ggbjbfqxi.sHtML

[U109] JS：数组分组
来源：http://blog.yfazqb.com/Article/details/gksvdjwgx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fktsv.cn/Article/details/gkxkmaves.sHtML

[U110] JS：数组分块
来源：http://m.share.epnwcf.com/Article/details/gbkmakdfq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.epnwcf.com/Article/details/gceqdlgye.sHtML

[U111] JS：对象转 Map
来源：http://wap.tarul.cn/Article/details/ganldhilv.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.yfazqb.com/Article/details/gduqabsbn.sHtML

[U112] JS：字符串补位
来源：http://www.blog.tarul.cn/Article/details/gpglwpqxx.sHtML

"7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/givxapqlm.sHtML

[U113] JS：正则替换全部
来源：http://blog.epnwcf.com/Article/details/gqacdrqeu.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gpgyqzxme.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.vehdjk.com/Article/details/gqwuiycgb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.yfazqb.com/Article/details/gksapmvnc.sHtML

[U115] JS：生成 UUID
来源：http://www.share.sjlbkw.cn/Article/details/gcfcrxosu.sHtML

crypto.randomUUID()
来源：http://m.share.fktsv.cn/Article/details/gdiwyzyze.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.sjlbkw.cn/Article/details/grulknxwv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.sjlbkw.cn/Article/details/gbouoqivk.sHtML

[U117] JS：单元测试
来源：http://www.share.epnwcf.com/Article/details/gxjjdjaaa.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.yfazqb.com/Article/details/ghsjyavsu.sHtML

[U118] JS：开发服务器
来源：http://blog.epnwcf.com/Article/details/gyeqalhmi.sHtML

npm i -D vite;  npx vite
来源：http://read.share.bbcook.cn/Article/details/gyneagtou.sHtML

[U119] JS：生产构建
来源：http://3g.fktsv.cn/Article/details/ginpysqvb.sHtML

npx vite build
来源：http://www.share.tarul.cn/Article/details/gfovvnrjm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fktsv.cn/Article/details/gwhdsurki.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.tarul.cn/Article/details/gwhuzykln.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gloplbkxw.sHtML

统计汇总
来源：http://m.share.bbcook.cn/Article/details/glsatdfqc.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/grhdpmgud.sHtML

按语言统计（条）：
来源：http://www.share.vehdjk.com/Article/details/gbcclsywp.sHtML

Python ......... 252
来源：http://baike.yfazqb.com/Article/details/gmbbfuhtw.sHtML

PHP ............ 252
来源：http://www.blog.yfazqb.com/Article/details/gjxitrnpo.sHtML

JavaScript ..... 252
来源：http://3g.vehdjk.com/Article/details/ghbidrwqr.sHtML

TypeScript ..... 212
来源：http://blog.fktsv.cn/Article/details/gbzlaucuc.sHtML

Java ........... 212
来源：http://read.share.fktsv.cn/Article/details/guzjlnvwu.sHtML

Go ............. 212
来源：http://wap.tarul.cn/Article/details/gbwecryhy.sHtML

Ruby ........... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gajaqbvto.sHtML

C# ............. 212
来源：http://3g.yfazqb.com/Article/details/gbbdiciot.sHtML

C .............. 30
来源：http://www.share.vehdjk.com/Article/details/grelmravu.sHtML

C++ ............ 30
来源：http://read.share.fktsv.cn/Article/details/gymknyesa.sHtML

SQL ............ 90
来源：http://3g.sjlbkw.cn/Article/details/gtqwornwk.sHtML

Bash ........... 80
来源：http://www.share.epnwcf.com/Article/details/gmtftadxb.sHtML

Kotlin ......... 15
来源：http://baike.vehdjk.com/Article/details/grubhhbbk.sHtML

Swift .......... 15
来源：http://m.share.tarul.cn/Article/details/gbycbcyjp.sHtML

Lua ............ 10
来源：http://blog.bbcook.cn/Article/details/glpekwicw.sHtML

Perl ........... 10
来源：http://www.m.share.bbcook.cn/Article/details/gdmxwdrme.sHtML

Scala .......... 10
来源：http://blog.yfazqb.com/Article/details/gqldczgfh.sHtML

------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gqdifiixo.sHtML

合计 ........... 2106 条
来源：http://3g.bbcook.cn/Article/details/gsbaxkuwm.sHtML

按章节统计：
来源：http://www.share.yfazqb.com/Article/details/gintstxdn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.tarul.cn/Article/details/gdkwwwjwz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.bbcook.cn/Article/details/gjiuftuiw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.epnwcf.com/Article/details/gyniptuft.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.vehdjk.com/Article/details/gwkkhklnu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.tarul.cn/Article/details/gqkohebxe.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.epnwcf.com/Article/details/goaytbblk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.yfazqb.com/Article/details/gsxnqcfwg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fktsv.cn/Article/details/gpvlbrotj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/gwygpgfjs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.sjlbkw.cn/Article/details/gcpjfqsrw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gfzsadigc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/gnvoatpwj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/gcreykbqi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.vehdjk.com/Article/details/gdwpaodwu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.epnwcf.com/Article/details/gesbwjphw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gharqakku.sHtML

Q SQL 专题                              90
来源：http://m.share.yfazqb.com/Article/details/gbkezazcd.sHtML

R Bash 专题                             80
来源：http://baike.tarul.cn/Article/details/golgpevhh.sHtML

S C / C++ 专题                          60
来源：http://3g.fktsv.cn/Article/details/gzacjncii.sHtML

T 其他语言补充                          60
来源：http://baike.sjlbkw.cn/Article/details/gmlppyurq.sHtML

U 高频实用片段                         120
来源：http://mobile.yfazqb.com/Article/details/ggaylxhxs.sHtML

------------------------------------
来源：http://mobile.tarul.cn/Article/details/gvtzirtgg.sHtML

合计                                  2106 条
来源：http://read.share.yfazqb.com/Article/details/gyjtpolkd.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gsuulgwiq.sHtML

使用提醒
来源：http://mobile.epnwcf.com/Article/details/gfpmhajrm.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/ghhjojwfk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.yfazqb.com/Article/details/gygwcjvgi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.vehdjk.com/Article/details/ggtzwoczg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.yfazqb.com/Article/details/gsndjmbet.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.tarul.cn/Article/details/gxbrvbwlk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fktsv.cn/Article/details/gkdqbhhxm.sHtML

—— 文件结束 ——
来源：http://wap.bbcook.cn/Article/details/gcfrvbnnm.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gtoylgrxq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.sjlbkw.cn/Article/details/gwnhooexe.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.epnwcf.com/Article/details/gpcjyvwyb.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gzqzhqwek.sHtML

【收录内容】
来源：http://www.share.epnwcf.com/Article/details/gyppwmmak.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.epnwcf.com/Article/details/gqxzpghcl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.vehdjk.com/Article/details/gmmnlnudy.sHtML

SQL · Bash · C · C++
来源：http://www.blog.sjlbkw.cn/Article/details/gaiwecdns.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.sjlbkw.cn/Article/details/gsfwcbvox.sHtML

【使用说明】
来源：http://www.m.share.epnwcf.com/Article/details/gbmslgeee.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fktsv.cn/Article/details/grmzngdan.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.sjlbkw.cn/Article/details/gwnfdjwwc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fktsv.cn/Article/details/gtyamzazm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.epnwcf.com/Article/details/gsuchqbiv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.tarul.cn/Article/details/gbaiseldj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fktsv.cn/Article/details/gzdhyvxpf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.yfazqb.com/Article/details/gjwaqzsmq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fktsv.cn/Article/details/gvydnbzrp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.tarul.cn/Article/details/gjbheslkg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.vehdjk.com/Article/details/gglkfmuxy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.tarul.cn/Article/details/gqyhvwxob.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.tarul.cn/Article/details/gngdhqvae.sHtML

【文件统计】
来源：http://baike.bbcook.cn/Article/details/gzxioqjuj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.bbcook.cn/Article/details/gokijnndr.sHtML

--------------------------------------------------------------------------------
来源：http://baike.tarul.cn/Article/details/ggkhtfjrd.sHtML

目  录
来源：http://www.m.share.epnwcf.com/Article/details/gdxjgmixd.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gyzqvfgbb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.tarul.cn/Article/details/gnqugqjek.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.vehdjk.com/Article/details/gejizuvxz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.vehdjk.com/Article/details/glwsjhurv.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.yfazqb.com/Article/details/gqqzsyzrw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fktsv.cn/Article/details/gymgeekjm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.epnwcf.com/Article/details/gzydqztxm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.epnwcf.com/Article/details/ggigjazyu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.bbcook.cn/Article/details/gzllwixvp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.epnwcf.com/Article/details/gkgwkgufk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.bbcook.cn/Article/details/gvdzkyjth.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/girnnqost.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.tarul.cn/Article/details/ghbonddsh.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.bbcook.cn/Article/details/gycndxpow.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fktsv.cn/Article/details/ghtjpxqoe.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.bbcook.cn/Article/details/gesaqwhbh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fktsv.cn/Article/details/gkcqeldjl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.epnwcf.com/Article/details/gibvgvwly.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.bbcook.cn/Article/details/greqixzxs.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fktsv.cn/Article/details/gxoszwqex.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.epnwcf.com/Article/details/glgwartse.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.bbcook.cn/Article/details/gevxymvne.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gmyfmjita.sHtML

A. 基础语法与类型
来源：http://read.share.epnwcf.com/Article/details/gxvyeyrvg.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gwjpannlg.sHtML

[A01] Hello World
来源：http://blog.epnwcf.com/Article/details/gpxkpzjia.sHtML

Py:   print("Hello, World!")
来源：http://wap.sjlbkw.cn/Article/details/gyvzlipcr.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fktsv.cn/Article/details/gpxhkvgeq.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.yfazqb.com/Article/details/galfhdwbl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.epnwcf.com/Article/details/gosikvvqk.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.epnwcf.com/Article/details/gsdfxdipt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.tarul.cn/Article/details/glwhpnyyl.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.sjlbkw.cn/Article/details/ghjzcynpn.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.tarul.cn/Article/details/gltubaxyb.sHtML

[A02] 变量声明与赋值
来源：http://mobile.bbcook.cn/Article/details/gadjnriks.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.sjlbkw.cn/Article/details/gxhvqdmvp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.sjlbkw.cn/Article/details/guzobfmyf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.bbcook.cn/Article/details/gqcenminn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.tarul.cn/Article/details/gdhrwsqkb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.sjlbkw.cn/Article/details/gaahahxri.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.bbcook.cn/Article/details/goztbvqko.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.yfazqb.com/Article/details/gkuvojhxk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.bbcook.cn/Article/details/gujexdinb.sHtML

[A03] 常量定义
来源：http://m.share.sjlbkw.cn/Article/details/grcvsoqtf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.sjlbkw.cn/Article/details/gzoyctxpz.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gceefxpql.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gjyjbqsgl.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gvncpghaw.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gcumequja.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.yfazqb.com/Article/details/gscbzgiyq.sHtML

Ruby: PI = 3.14159
来源：http://mobile.bbcook.cn/Article/details/gjuczeugi.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/grquumonz.sHtML

[A04] 判断变量类型
来源：http://www.share.epnwcf.com/Article/details/ggatvunto.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.bbcook.cn/Article/details/gtuyustjq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.vehdjk.com/Article/details/gsnxboynf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.sjlbkw.cn/Article/details/gcfleaoit.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.bbcook.cn/Article/details/gsmcsvdlc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.yfazqb.com/Article/details/gbwsrebul.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.yfazqb.com/Article/details/glpzfshja.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.epnwcf.com/Article/details/gqqvefppp.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.bbcook.cn/Article/details/ghgrgurtf.sHtML

[A05] 整数除法与取模
来源：http://3g.tarul.cn/Article/details/gffiqxerg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.sjlbkw.cn/Article/details/gurarntbg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.bbcook.cn/Article/details/goauclrcz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gktndufgt.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gnyrgpgtm.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gjwkthatr.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/gwltmpdcg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.tarul.cn/Article/details/gfkaaziit.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gzjxavzrr.sHtML

[A06] 字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gyorobhpl.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fktsv.cn/Article/details/ghlvlagsa.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.tarul.cn/Article/details/guqovslji.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.tarul.cn/Article/details/gamvwpyqm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.sjlbkw.cn/Article/details/gtkdtwuat.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.epnwcf.com/Article/details/gehenipxu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.yfazqb.com/Article/details/gapdmlwvr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.epnwcf.com/Article/details/gycylsxho.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.yfazqb.com/Article/details/gfyecgfps.sHtML

[A07] 数字转字符串
来源：http://wap.fktsv.cn/Article/details/gvfiegjtl.sHtML

Py:   str(42)
来源：http://3g.epnwcf.com/Article/details/ghsmrzynf.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.epnwcf.com/Article/details/gjbioitcw.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fktsv.cn/Article/details/gzuokizvt.sHtML

TS:   String(42)
来源：http://blog.vehdjk.com/Article/details/gemrkesnr.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.yfazqb.com/Article/details/gpjjaqgns.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.vehdjk.com/Article/details/gqaxvpyry.sHtML

Ruby: 42.to_s
来源：http://baike.fktsv.cn/Article/details/grhqyglcv.sHtML

C#:   42.ToString()
来源：http://read.share.tarul.cn/Article/details/gkkfkbsbt.sHtML

[A08] 取整与四舍五入
来源：http://blog.tarul.cn/Article/details/ggxurgcqp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.bbcook.cn/Article/details/gtutdxuzw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.bbcook.cn/Article/details/gvpduwcsh.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.vehdjk.com/Article/details/ggsyxsfip.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.epnwcf.com/Article/details/gjeimucpx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.bbcook.cn/Article/details/gaohppajw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/gjysqjxxg.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.epnwcf.com/Article/details/gckunhfiu.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.vehdjk.com/Article/details/gqdvlbtxk.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.tarul.cn/Article/details/gbooqhpwn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gcclhdimq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gawqsoczu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.vehdjk.com/Article/details/gcmgaxmpm.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fktsv.cn/Article/details/gcedbbpnk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/guphpkifd.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.fktsv.cn/Article/details/gsscnjgvb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.epnwcf.com/Article/details/glbyrbqow.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.epnwcf.com/Article/details/gpmpinkph.sHtML

[A10] 生成随机数
来源：http://baike.yfazqb.com/Article/details/gugukhckb.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.sjlbkw.cn/Article/details/grblmxjcw.sHtML

PHP:  random_int(1, 100);
来源：http://blog.yfazqb.com/Article/details/gjaizdomj.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.bbcook.cn/Article/details/gaacaufpx.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.vehdjk.com/Article/details/gaosbvslc.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.sjlbkw.cn/Article/details/gpvzisvet.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.bbcook.cn/Article/details/gdjamwnkq.sHtML

Ruby: rand(1..100)
来源：http://wap.vehdjk.com/Article/details/gwoqdoneb.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.bbcook.cn/Article/details/guxdvanze.sHtML

[A11] 条件表达式（三元）
来源：http://wap.sjlbkw.cn/Article/details/geodiwhoe.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.epnwcf.com/Article/details/gwumvcdgr.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.bbcook.cn/Article/details/genmntzdy.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.tarul.cn/Article/details/gurryzokv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.epnwcf.com/Article/details/gwpyiukkp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.tarul.cn/Article/details/gkuvfmmpr.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.epnwcf.com/Article/details/gwnrtdkou.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.yfazqb.com/Article/details/gztglkitg.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.bbcook.cn/Article/details/gbawdcsdm.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gcbdsnydb.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.yfazqb.com/Article/details/gnuwsyfjb.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.yfazqb.com/Article/details/gyvwffheb.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.tarul.cn/Article/details/grlrxkldw.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.epnwcf.com/Article/details/ghiziymdi.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.fktsv.cn/Article/details/ginpqoxnb.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.vehdjk.com/Article/details/gzbntvmkf.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.epnwcf.com/Article/details/gwxlpjhob.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.epnwcf.com/Article/details/gmsgmmwbf.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.epnwcf.com/Article/details/gbmhgunkt.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.bbcook.cn/Article/details/gjomambbq.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gkpoxeesf.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.vehdjk.com/Article/details/gojpqcphb.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/gnosmzqop.sHtML

Java: "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/gpgmkvzst.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/gdnreqnof.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/gykpyibsv.sHtML

C#:   "第一行\n第二行"
来源：http://baike.tarul.cn/Article/details/goqovgtqo.sHtML

[A14] 注释写法
来源：http://wap.bbcook.cn/Article/details/gmxgkjrcy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.bbcook.cn/Article/details/gisliolly.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.fktsv.cn/Article/details/gdjilchtj.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/gykvlyenc.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.epnwcf.com/Article/details/gtlhswkyl.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.tarul.cn/Article/details/gxvtqsrry.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.vehdjk.com/Article/details/gqirlvhuz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.tarul.cn/Article/details/gvdkuibns.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.bbcook.cn/Article/details/gtijxgorv.sHtML

[A15] 空值判断与默认值
来源：http://www.share.epnwcf.com/Article/details/gvsvywhxh.sHtML

Py:   value = data or "默认值"
来源：http://read.share.tarul.cn/Article/details/grnwzovng.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.epnwcf.com/Article/details/gaoohwiyy.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.yfazqb.com/Article/details/gepwfdnqv.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.yfazqb.com/Article/details/ggfwhvuph.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.fktsv.cn/Article/details/gtiwggkyb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsubfcycu.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.epnwcf.com/Article/details/gcnjbzypw.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.vehdjk.com/Article/details/gvyeinpok.sHtML

[A16] 真假值判断规则
来源：http://www.share.fktsv.cn/Article/details/gbigrvaig.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.bbcook.cn/Article/details/gsbwwrcjt.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.epnwcf.com/Article/details/guvsntceq.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.tarul.cn/Article/details/giwzbxdwn.sHtML

TS:   if (!x) {}
来源：http://read.share.epnwcf.com/Article/details/gzzprapxp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.fktsv.cn/Article/details/gichdzpih.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.fktsv.cn/Article/details/genqznaxo.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.bbcook.cn/Article/details/grhgivuqo.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.bbcook.cn/Article/details/gyizcxrok.sHtML

[A17] 位运算
来源：http://baike.fktsv.cn/Article/details/gtzmlazvg.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.tarul.cn/Article/details/glavezcep.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gsnjxcokj.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/getrmukmk.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gfxcwdzdz.sHtML


<!-- 参考信息 -->