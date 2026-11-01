代发 wailian999

[U97] JS：并发请求
来源：http://blog.vehdjk.com/Article/details/gfvekqzgh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.vehdjk.com/Article/details/gtzfmqiqu.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fktsv.cn/Article/details/gsuvuvefj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.sjlbkw.cn/Article/details/gxiyuguor.sHtML

[U99] JS：事件监听
来源：http://blog.sjlbkw.cn/Article/details/ggmrbljsz.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.sjlbkw.cn/Article/details/gqnamxgkb.sHtML

[U100] JS：DOM 查询
来源：http://baike.yfazqb.com/Article/details/gpetiqpwx.sHtML

document.querySelector(".item")
来源：http://3g.epnwcf.com/Article/details/gnrsljgoa.sHtML

[U101] JS：classList 操作
来源：http://www.share.fktsv.cn/Article/details/gpegijean.sHtML

el.classList.toggle("active")
来源：http://blog.yfazqb.com/Article/details/gaosfinjy.sHtML

[U102] JS：本地存储
来源：http://blog.tarul.cn/Article/details/gvnqxcgae.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.bbcook.cn/Article/details/ggmdeehtf.sHtML

[U103] JS：定时器
来源：http://www.m.share.bbcook.cn/Article/details/gdzkunzpu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fktsv.cn/Article/details/gigvogczi.sHtML

[U104] JS：防抖
来源：http://www.share.tarul.cn/Article/details/gwlgvyxsi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/gzdwojvng.sHtML

[U105] JS：节流
来源：http://baike.fktsv.cn/Article/details/grenzdbew.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.yfazqb.com/Article/details/gyzblmowy.sHtML

[U106] JS：日期格式化
来源：http://blog.tarul.cn/Article/details/gibyxsssx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.bbcook.cn/Article/details/ggvxkpqoj.sHtML

[U107] JS：数字千分位
来源：http://3g.tarul.cn/Article/details/gdvsqxrvn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.epnwcf.com/Article/details/gljaracqi.sHtML

[U108] JS：随机整数
来源：http://www.blog.yfazqb.com/Article/details/gdruyylsi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fktsv.cn/Article/details/gnimzraok.sHtML

[U109] JS：数组分组
来源：http://www.blog.tarul.cn/Article/details/gnsoqgapo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.bbcook.cn/Article/details/ghbszpwdd.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fktsv.cn/Article/details/gcbnrciim.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.tarul.cn/Article/details/gyyukvfrl.sHtML

[U111] JS：对象转 Map
来源：http://3g.epnwcf.com/Article/details/gfxpwnxkj.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.yfazqb.com/Article/details/gcozgmopk.sHtML

[U112] JS：字符串补位
来源：http://www.share.sjlbkw.cn/Article/details/gcapsoyip.sHtML

"7".padStart(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/gwpyorvpi.sHtML

[U113] JS：正则替换全部
来源：http://www.share.vehdjk.com/Article/details/gfiazzorj.sHtML

s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gtfagtoet.sHtML

[U114] JS：JSON 深比较
来源：http://baike.sjlbkw.cn/Article/details/gpksvmhiz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.tarul.cn/Article/details/gnwdesijn.sHtML

[U115] JS：生成 UUID
来源：http://baike.vehdjk.com/Article/details/gxtwzpzyk.sHtML

crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gyqgpsthm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.vehdjk.com/Article/details/ggttbxeyq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.epnwcf.com/Article/details/gbjmdzzfe.sHtML

[U117] JS：单元测试
来源：http://www.blog.tarul.cn/Article/details/gypctgidk.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.tarul.cn/Article/details/ghogevxhf.sHtML

[U118] JS：开发服务器
来源：http://read.share.sjlbkw.cn/Article/details/gzsxpaeju.sHtML

npm i -D vite;  npx vite
来源：http://mobile.tarul.cn/Article/details/gwoaruokb.sHtML

[U119] JS：生产构建
来源：http://mobile.bbcook.cn/Article/details/gibyugbqy.sHtML

npx vite build
来源：http://www.blog.sjlbkw.cn/Article/details/gfvmpzvgy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.sjlbkw.cn/Article/details/gusncqqvw.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.vehdjk.com/Article/details/gfmtykypq.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gipokricw.sHtML

统计汇总
来源：http://wap.sjlbkw.cn/Article/details/glcginvby.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gjhnqsqwl.sHtML

按语言统计（条）：
来源：http://mobile.tarul.cn/Article/details/gcsyqepki.sHtML

Python ......... 252
来源：http://www.share.fktsv.cn/Article/details/gmnfxizis.sHtML

PHP ............ 252
来源：http://read.share.epnwcf.com/Article/details/gjspfhdqg.sHtML

JavaScript ..... 252
来源：http://www.m.share.fktsv.cn/Article/details/gysbgnhxt.sHtML

TypeScript ..... 212
来源：http://mobile.epnwcf.com/Article/details/grkmqaymh.sHtML

Java ........... 212
来源：http://www.blog.vehdjk.com/Article/details/gkmtsklgc.sHtML

Go ............. 212
来源：http://read.share.tarul.cn/Article/details/gdetpnctv.sHtML

Ruby ........... 212
来源：http://mobile.bbcook.cn/Article/details/grqzdcbit.sHtML

C# ............. 212
来源：http://read.share.fktsv.cn/Article/details/gmpwibrpr.sHtML

C .............. 30
来源：http://www.m.share.fktsv.cn/Article/details/gvfukxxqm.sHtML

C++ ............ 30
来源：http://www.blog.tarul.cn/Article/details/gwxcsqlnc.sHtML

SQL ............ 90
来源：http://www.m.share.vehdjk.com/Article/details/goseblwnu.sHtML

Bash ........... 80
来源：http://www.blog.tarul.cn/Article/details/gboxpiefn.sHtML

Kotlin ......... 15
来源：http://3g.epnwcf.com/Article/details/gsvdqdqbs.sHtML

Swift .......... 15
来源：http://read.share.bbcook.cn/Article/details/gtivmixdz.sHtML

Lua ............ 10
来源：http://www.m.share.fktsv.cn/Article/details/gozdrjyft.sHtML

Perl ........... 10
来源：http://3g.sjlbkw.cn/Article/details/gznpxuzvd.sHtML

Scala .......... 10
来源：http://3g.tarul.cn/Article/details/geuvzgoni.sHtML

------------------------------------
来源：http://3g.yfazqb.com/Article/details/gtdurlxot.sHtML

合计 ........... 2106 条
来源：http://www.share.vehdjk.com/Article/details/gkhtcfiyt.sHtML

按章节统计：
来源：http://wap.vehdjk.com/Article/details/gzlfikevd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.vehdjk.com/Article/details/gybibqaso.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.sjlbkw.cn/Article/details/gupbokvgb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.bbcook.cn/Article/details/glsvqnbpr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.sjlbkw.cn/Article/details/gigjhbtlq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.vehdjk.com/Article/details/giqrusuwi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.epnwcf.com/Article/details/gltclhevo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.vehdjk.com/Article/details/gugriqwup.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.yfazqb.com/Article/details/gfuixhtkd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.sjlbkw.cn/Article/details/goiawigjy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.tarul.cn/Article/details/gpzdffisw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gcukaxgxm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gkbtditcz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gxbisblql.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fktsv.cn/Article/details/gktfynhhi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.yfazqb.com/Article/details/gshbasxfp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fktsv.cn/Article/details/glpzvwrmk.sHtML

Q SQL 专题                              90
来源：http://3g.bbcook.cn/Article/details/glnkhpnqb.sHtML

R Bash 专题                             80
来源：http://blog.bbcook.cn/Article/details/gloenszwt.sHtML

S C / C++ 专题                          60
来源：http://blog.bbcook.cn/Article/details/geikhcvqn.sHtML

T 其他语言补充                          60
来源：http://www.m.share.tarul.cn/Article/details/gyjknnhzc.sHtML

U 高频实用片段                         120
来源：http://baike.bbcook.cn/Article/details/gucrfshuq.sHtML

------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gwifacpgs.sHtML

合计                                  2106 条
来源：http://www.m.share.epnwcf.com/Article/details/geqxzxivy.sHtML

--------------------------------------------------------------------------------
来源：http://wap.epnwcf.com/Article/details/gwdbuzwce.sHtML

使用提醒
来源：http://www.share.sjlbkw.cn/Article/details/gjchscnlf.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gpzfqlosj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.epnwcf.com/Article/details/gstablfel.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.vehdjk.com/Article/details/gujwkadac.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.bbcook.cn/Article/details/gvzdnppwf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.vehdjk.com/Article/details/glysdqvoh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.bbcook.cn/Article/details/ghvsvqmqc.sHtML

—— 文件结束 ——
来源：http://m.share.vehdjk.com/Article/details/glgvkflrw.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gdvbwrnjs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.tarul.cn/Article/details/gbtgncblu.sHtML

Common Programming Examples Cheat Book
来源：http://wap.vehdjk.com/Article/details/gizluuolq.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gbyuxcqlw.sHtML

【收录内容】
来源：http://baike.fktsv.cn/Article/details/gsakbenmg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.sjlbkw.cn/Article/details/gevqagpbu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.yfazqb.com/Article/details/gilyaoqvi.sHtML

SQL · Bash · C · C++
来源：http://mobile.tarul.cn/Article/details/gaeuhrrxo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.yfazqb.com/Article/details/gviapfhpa.sHtML

【使用说明】
来源：http://read.share.sjlbkw.cn/Article/details/gcfoolkeh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.bbcook.cn/Article/details/gvyzliebe.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.vehdjk.com/Article/details/gumcgejpu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.tarul.cn/Article/details/gltyqnwna.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.tarul.cn/Article/details/gqaavgahl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.bbcook.cn/Article/details/gcvewfdxt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.epnwcf.com/Article/details/gkkbexvio.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.sjlbkw.cn/Article/details/gznlhqodb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.yfazqb.com/Article/details/gwaahumdd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.epnwcf.com/Article/details/gtdboukqu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.vehdjk.com/Article/details/gghjxomii.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.yfazqb.com/Article/details/gvvblezqe.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.bbcook.cn/Article/details/gtjddhksw.sHtML

【文件统计】
来源：http://www.blog.sjlbkw.cn/Article/details/gdejcmvjz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.sjlbkw.cn/Article/details/gcbdkvwgq.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gcxtpqqow.sHtML

目  录
来源：http://mobile.fktsv.cn/Article/details/gidapxpjo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.vehdjk.com/Article/details/gbhegkvur.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.tarul.cn/Article/details/gxgchynih.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.bbcook.cn/Article/details/gqfwntqbk.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.sjlbkw.cn/Article/details/gckjjzzgw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.epnwcf.com/Article/details/gmklrdzti.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.bbcook.cn/Article/details/gdnzajuxh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fktsv.cn/Article/details/gwscjpvvv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fktsv.cn/Article/details/gcetwkpiu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.yfazqb.com/Article/details/gdajelrgq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.tarul.cn/Article/details/gqgjckqng.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.tarul.cn/Article/details/gstjukjzu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/gdaeqxupr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.epnwcf.com/Article/details/gkmsbwkcj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.vehdjk.com/Article/details/gsfkdhsnp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.bbcook.cn/Article/details/getvjwclu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.bbcook.cn/Article/details/gsnomsvuz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/gofiddjiq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.yfazqb.com/Article/details/ghbtoodyl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.bbcook.cn/Article/details/gjgvqqboy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.vehdjk.com/Article/details/gfqaqzvcp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.vehdjk.com/Article/details/gfelpsefv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.sjlbkw.cn/Article/details/gnivftqjc.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gahqdsnqf.sHtML

A. 基础语法与类型
来源：http://blog.epnwcf.com/Article/details/gdguarouz.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gzxleqcby.sHtML

[A01] Hello World
来源：http://www.share.yfazqb.com/Article/details/gwbefpexi.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.bbcook.cn/Article/details/giuutxihi.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.tarul.cn/Article/details/gjwoabfoq.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.tarul.cn/Article/details/gtamqwemm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.tarul.cn/Article/details/gybgjuyhd.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.yfazqb.com/Article/details/guewxzlzt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.bbcook.cn/Article/details/gdcuvnyez.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.bbcook.cn/Article/details/gbmemrmxk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fktsv.cn/Article/details/glrzltjyd.sHtML

[A02] 变量声明与赋值
来源：http://read.share.epnwcf.com/Article/details/gauniduqt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fktsv.cn/Article/details/gswxvtule.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.sjlbkw.cn/Article/details/gdngkasgi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.sjlbkw.cn/Article/details/gqesiayym.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.bbcook.cn/Article/details/ggizqkjwc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwwuzurp.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.sjlbkw.cn/Article/details/gektyujzs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.bbcook.cn/Article/details/gzkqlpjdg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gitwqphjt.sHtML

[A03] 常量定义
来源：http://wap.sjlbkw.cn/Article/details/gzazqsfei.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.yfazqb.com/Article/details/gyudlvjsm.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gspzbvyau.sHtML

JS:   const PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gezvzhotm.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gnsrszavq.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/ghlyhbica.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.vehdjk.com/Article/details/giumrgaym.sHtML

Ruby: PI = 3.14159
来源：http://3g.epnwcf.com/Article/details/gknjifyzb.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gbbfdzyzz.sHtML

[A04] 判断变量类型
来源：http://mobile.tarul.cn/Article/details/gubyhmlsp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.yfazqb.com/Article/details/gjtprmtpb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.sjlbkw.cn/Article/details/gxknohato.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.vehdjk.com/Article/details/gokgaijhu.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.sjlbkw.cn/Article/details/gvddhvxgn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.sjlbkw.cn/Article/details/gojtpebyh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.vehdjk.com/Article/details/gygkfqeck.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.yfazqb.com/Article/details/glhatrera.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.sjlbkw.cn/Article/details/gjcknjklh.sHtML

[A05] 整数除法与取模
来源：http://3g.yfazqb.com/Article/details/gttzzgahx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.vehdjk.com/Article/details/gsmgpnjkn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fktsv.cn/Article/details/ggvkmfjlq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fktsv.cn/Article/details/gumapcwcc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.bbcook.cn/Article/details/gyzoifpvt.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/gdodoptoe.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/gbkbcwarl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gpfbbpyfm.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/gqfoadhgl.sHtML

[A06] 字符串转数字
来源：http://www.share.yfazqb.com/Article/details/gqwflmtbj.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.tarul.cn/Article/details/gxwuyknqi.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.bbcook.cn/Article/details/gasyjidyd.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.tarul.cn/Article/details/gtpaaydae.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.bbcook.cn/Article/details/gxakczquz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.yfazqb.com/Article/details/giipgaekh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fktsv.cn/Article/details/gmcnbqcvw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.tarul.cn/Article/details/gcielrszc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.tarul.cn/Article/details/gizdvzfhm.sHtML

[A07] 数字转字符串
来源：http://blog.yfazqb.com/Article/details/gnnltjdph.sHtML

Py:   str(42)
来源：http://read.share.tarul.cn/Article/details/goyegfrjd.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.tarul.cn/Article/details/gzaqacakm.sHtML

JS:   String(42); (42).toString()
来源：http://wap.epnwcf.com/Article/details/gmxvuuzan.sHtML

TS:   String(42)
来源：http://baike.bbcook.cn/Article/details/gdujfopch.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.sjlbkw.cn/Article/details/gcmkliawk.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fktsv.cn/Article/details/gopqobiup.sHtML

Ruby: 42.to_s
来源：http://read.share.vehdjk.com/Article/details/gyjftojaw.sHtML

C#:   42.ToString()
来源：http://read.share.sjlbkw.cn/Article/details/gfezzymhl.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.tarul.cn/Article/details/gltryydun.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/gqsktteya.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.sjlbkw.cn/Article/details/gqwszhrao.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.bbcook.cn/Article/details/gkkqtivwz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.sjlbkw.cn/Article/details/ggsqqtkrq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/gwbdghsqn.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.vehdjk.com/Article/details/giqjjrfpm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.yfazqb.com/Article/details/geksuqaxf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/guhuzetgk.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fktsv.cn/Article/details/gnnsvtbub.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/gzdemeejd.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gsfshklgo.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.tarul.cn/Article/details/gxpiiwvfr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gjfcyyxys.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.vehdjk.com/Article/details/gncmdfkrg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.yfazqb.com/Article/details/gqarncdco.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fktsv.cn/Article/details/gdwmnawkf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.fktsv.cn/Article/details/grknojnmd.sHtML

[A10] 生成随机数
来源：http://mobile.epnwcf.com/Article/details/gjjxfyghl.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.bbcook.cn/Article/details/gcpdbtdre.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.yfazqb.com/Article/details/gmikotulc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fktsv.cn/Article/details/grnbmikka.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.vehdjk.com/Article/details/gbdzpqjty.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.vehdjk.com/Article/details/gwbumfjpz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.yfazqb.com/Article/details/gfodqxdhx.sHtML

Ruby: rand(1..100)
来源：http://www.share.vehdjk.com/Article/details/gbhyfnkxv.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.tarul.cn/Article/details/gtzxlqabo.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.bbcook.cn/Article/details/grwbohsfi.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.tarul.cn/Article/details/gzxbmeaze.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.sjlbkw.cn/Article/details/gecuowbot.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.tarul.cn/Article/details/gjivxuedw.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.tarul.cn/Article/details/gpxyxxggu.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gvrvshvzn.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fktsv.cn/Article/details/gqvtfgdfo.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.vehdjk.com/Article/details/guomoiyhj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.bbcook.cn/Article/details/gqbqieylr.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.sjlbkw.cn/Article/details/gklyzajqt.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.vehdjk.com/Article/details/gmfivpjpt.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.tarul.cn/Article/details/gytagjtfe.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.yfazqb.com/Article/details/gtlpiazqy.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.yfazqb.com/Article/details/gdqicwzpl.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.yfazqb.com/Article/details/gtzarzpsq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.bbcook.cn/Article/details/grokrkijv.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.sjlbkw.cn/Article/details/gfyxmfpvz.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.fktsv.cn/Article/details/gthlwivtg.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.tarul.cn/Article/details/glrcwrfra.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/guclfhhgh.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.bbcook.cn/Article/details/gdsecaubu.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gllsvikqv.sHtML

TS:   "第一行\n第二行"
来源：http://blog.epnwcf.com/Article/details/ghvhzuggl.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/glbkrwyoy.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.tarul.cn/Article/details/gtzoufoiq.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/glgexnfiu.sHtML

C#:   "第一行\n第二行"
来源：http://baike.tarul.cn/Article/details/gvkxaigae.sHtML

[A14] 注释写法
来源：http://wap.sjlbkw.cn/Article/details/gpiwhwvlr.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fktsv.cn/Article/details/gqfisboss.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/gmmblqwuk.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.tarul.cn/Article/details/gjdmojkii.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.epnwcf.com/Article/details/greyeypia.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.yfazqb.com/Article/details/gqmlvpakv.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqymdfre.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.fktsv.cn/Article/details/gurfqdonb.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.vehdjk.com/Article/details/gckophvff.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.epnwcf.com/Article/details/gubxobrju.sHtML

Py:   value = data or "默认值"
来源：http://read.share.yfazqb.com/Article/details/glueczrcu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.sjlbkw.cn/Article/details/gtajphjyz.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.vehdjk.com/Article/details/gjyfldfdo.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.vehdjk.com/Article/details/gqvlqrrzo.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.tarul.cn/Article/details/ggfdiuugf.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.sjlbkw.cn/Article/details/guedctysi.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fktsv.cn/Article/details/gtkedbdtk.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.sjlbkw.cn/Article/details/gnkgouyxu.sHtML

[A16] 真假值判断规则
来源：http://baike.tarul.cn/Article/details/guazvvhjy.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.epnwcf.com/Article/details/gusenwrmi.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.epnwcf.com/Article/details/gxdsqeoun.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.yfazqb.com/Article/details/gpnquhldt.sHtML

TS:   if (!x) {}
来源：http://3g.vehdjk.com/Article/details/gyqsknrdf.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.yfazqb.com/Article/details/gpleifbcg.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.yfazqb.com/Article/details/gnsixnnou.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.sjlbkw.cn/Article/details/gfgeziyqg.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fktsv.cn/Article/details/gbtkzgmtd.sHtML

[A17] 位运算
来源：http://mobile.vehdjk.com/Article/details/gtgmavfhe.sHtML


<!-- 参考信息 -->