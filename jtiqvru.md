代发 wailian999

[U99] JS：事件监听
来源：http://www.blog.sjlbkw.cn/Article/details/gbsohnmyt.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.bbcook.cn/Article/details/gyfrwzsnl.sHtML

[U100] JS：DOM 查询
来源：http://blog.epnwcf.com/Article/details/gzxdvehai.sHtML

document.querySelector(".item")
来源：http://baike.vehdjk.com/Article/details/gnlkhsouq.sHtML

[U101] JS：classList 操作
来源：http://mobile.bbcook.cn/Article/details/gtpjnaztc.sHtML

el.classList.toggle("active")
来源：http://m.share.fktsv.cn/Article/details/gbxqtdutz.sHtML

[U102] JS：本地存储
来源：http://read.share.sjlbkw.cn/Article/details/glfeirgfv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.yfazqb.com/Article/details/ghxowllpw.sHtML

[U103] JS：定时器
来源：http://blog.fktsv.cn/Article/details/gyzxupnvq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.yfazqb.com/Article/details/goyywlref.sHtML

[U104] JS：防抖
来源：http://3g.sjlbkw.cn/Article/details/gtgpxsmjn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gbdafjuzb.sHtML

[U105] JS：节流
来源：http://baike.yfazqb.com/Article/details/gjbqxnkwf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.sjlbkw.cn/Article/details/gecowgdir.sHtML

[U106] JS：日期格式化
来源：http://3g.fktsv.cn/Article/details/gepuhqsav.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.sjlbkw.cn/Article/details/grcxrihdd.sHtML

[U107] JS：数字千分位
来源：http://mobile.yfazqb.com/Article/details/gjoozoqgs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fktsv.cn/Article/details/gltzpoaqa.sHtML

[U108] JS：随机整数
来源：http://read.share.bbcook.cn/Article/details/gixsysxvt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.tarul.cn/Article/details/gdeulalhx.sHtML

[U109] JS：数组分组
来源：http://3g.bbcook.cn/Article/details/gqqznywku.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/gumimfpcs.sHtML

[U110] JS：数组分块
来源：http://mobile.fktsv.cn/Article/details/gagwfdgyp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.epnwcf.com/Article/details/gwwphtsgd.sHtML

[U111] JS：对象转 Map
来源：http://wap.yfazqb.com/Article/details/gufvdecrh.sHtML

new Map(Object.entries(obj))
来源：http://read.share.sjlbkw.cn/Article/details/gotreaznr.sHtML

[U112] JS：字符串补位
来源：http://wap.tarul.cn/Article/details/giwxomzqf.sHtML

"7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gxyxfnjej.sHtML

[U113] JS：正则替换全部
来源：http://m.share.tarul.cn/Article/details/ghdxyqlie.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gizywymbt.sHtML

[U114] JS：JSON 深比较
来源：http://3g.yfazqb.com/Article/details/gcuqwbfrs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.epnwcf.com/Article/details/gvjrmdngc.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.sjlbkw.cn/Article/details/ggcdtqtzo.sHtML

crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gvspiynvj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.vehdjk.com/Article/details/gvrjieyfm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.bbcook.cn/Article/details/gtcuioqlf.sHtML

[U117] JS：单元测试
来源：http://www.blog.yfazqb.com/Article/details/gvvlqwtll.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfsodyjk.sHtML

[U118] JS：开发服务器
来源：http://www.blog.sjlbkw.cn/Article/details/goggjpfds.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.tarul.cn/Article/details/gfajtgvsh.sHtML

[U119] JS：生产构建
来源：http://mobile.bbcook.cn/Article/details/gekycguqq.sHtML

npx vite build
来源：http://mobile.sjlbkw.cn/Article/details/gqdqclvjg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fktsv.cn/Article/details/gviwwxxkf.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.bbcook.cn/Article/details/gmoisrhaq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/goeozixlq.sHtML

统计汇总
来源：http://www.blog.epnwcf.com/Article/details/gdruogdqx.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gvikytczh.sHtML

按语言统计（条）：
来源：http://www.blog.vehdjk.com/Article/details/gosxvkjcw.sHtML

Python ......... 252
来源：http://baike.sjlbkw.cn/Article/details/gyidcaztg.sHtML

PHP ............ 252
来源：http://www.m.share.yfazqb.com/Article/details/gdzgglwfg.sHtML

JavaScript ..... 252
来源：http://blog.bbcook.cn/Article/details/gdmndibmz.sHtML

TypeScript ..... 212
来源：http://www.share.tarul.cn/Article/details/gdpesrhil.sHtML

Java ........... 212
来源：http://m.share.yfazqb.com/Article/details/gdevpgzxr.sHtML

Go ............. 212
来源：http://m.share.vehdjk.com/Article/details/gskngkqoi.sHtML

Ruby ........... 212
来源：http://baike.vehdjk.com/Article/details/gssgotthv.sHtML

C# ............. 212
来源：http://mobile.tarul.cn/Article/details/gzjrtjcng.sHtML

C .............. 30
来源：http://read.share.bbcook.cn/Article/details/gtzppbbnr.sHtML

C++ ............ 30
来源：http://3g.tarul.cn/Article/details/gelajlkms.sHtML

SQL ............ 90
来源：http://blog.sjlbkw.cn/Article/details/guvcloefx.sHtML

Bash ........... 80
来源：http://wap.bbcook.cn/Article/details/gqnlmcsom.sHtML

Kotlin ......... 15
来源：http://read.share.sjlbkw.cn/Article/details/gdnfbrdph.sHtML

Swift .......... 15
来源：http://www.share.sjlbkw.cn/Article/details/gikrhemgg.sHtML

Lua ............ 10
来源：http://www.m.share.sjlbkw.cn/Article/details/gomisqgtc.sHtML

Perl ........... 10
来源：http://read.share.epnwcf.com/Article/details/gjecofbti.sHtML

Scala .......... 10
来源：http://3g.bbcook.cn/Article/details/gklsrydeg.sHtML

------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/ghalwhlvo.sHtML

合计 ........... 2106 条
来源：http://blog.vehdjk.com/Article/details/gnyhnyrzw.sHtML

按章节统计：
来源：http://www.m.share.vehdjk.com/Article/details/gkducnoqm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.epnwcf.com/Article/details/gtdaaqwar.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.bbcook.cn/Article/details/guupnivgw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fktsv.cn/Article/details/gnujgowkx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fktsv.cn/Article/details/gkbgudkjh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.vehdjk.com/Article/details/gltushabu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.epnwcf.com/Article/details/gphlocang.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.sjlbkw.cn/Article/details/gdrtqzczs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.vehdjk.com/Article/details/gbabsyyfx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/guctrqydj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.sjlbkw.cn/Article/details/gqgverczh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/gkbsifppx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gwwparhwh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/ggcsevgzz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.sjlbkw.cn/Article/details/gxfcqjhca.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.epnwcf.com/Article/details/gzarwnvzn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gnqpinaqj.sHtML

Q SQL 专题                              90
来源：http://baike.bbcook.cn/Article/details/gjznxrdpa.sHtML

R Bash 专题                             80
来源：http://blog.yfazqb.com/Article/details/glxfljqas.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.tarul.cn/Article/details/gcngfjolj.sHtML

T 其他语言补充                          60
来源：http://blog.yfazqb.com/Article/details/gtqvcgxzc.sHtML

U 高频实用片段                         120
来源：http://www.m.share.vehdjk.com/Article/details/gngshhfxq.sHtML

------------------------------------
来源：http://wap.fktsv.cn/Article/details/glshzljav.sHtML

合计                                  2106 条
来源：http://baike.tarul.cn/Article/details/gpqezqnus.sHtML

--------------------------------------------------------------------------------
来源：http://3g.epnwcf.com/Article/details/gsezzwuyt.sHtML

使用提醒
来源：http://mobile.vehdjk.com/Article/details/gsmnnrfew.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gpvyqcrqz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.vehdjk.com/Article/details/gplgysafx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.bbcook.cn/Article/details/grhvruted.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.yfazqb.com/Article/details/goxpbmrmi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.bbcook.cn/Article/details/geiiryuma.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fktsv.cn/Article/details/gcbussvkt.sHtML

—— 文件结束 ——
来源：http://3g.fktsv.cn/Article/details/gbmsnhqzl.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gawxopgnt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.vehdjk.com/Article/details/goymfprbk.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.epnwcf.com/Article/details/gndlqpplu.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gbvspjboa.sHtML

【收录内容】
来源：http://www.share.fktsv.cn/Article/details/gkwibtcqq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.epnwcf.com/Article/details/ggxxaufev.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fktsv.cn/Article/details/geqfxcmkc.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.bbcook.cn/Article/details/gusyhqhju.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fktsv.cn/Article/details/gttarrcfv.sHtML

【使用说明】
来源：http://blog.tarul.cn/Article/details/gphcdynce.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fktsv.cn/Article/details/gpkaerqra.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.yfazqb.com/Article/details/ghuvxjnqs.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.bbcook.cn/Article/details/gwbczegfp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.yfazqb.com/Article/details/gnfangkhw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.tarul.cn/Article/details/gjdjxzsmk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.vehdjk.com/Article/details/gstgepmmq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.tarul.cn/Article/details/gauildfpw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fktsv.cn/Article/details/gbmuyupai.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.bbcook.cn/Article/details/gztvnntys.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fktsv.cn/Article/details/gzcrmfsyk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.yfazqb.com/Article/details/guqvcroxb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.vehdjk.com/Article/details/gzivryhnw.sHtML

【文件统计】
来源：http://wap.bbcook.cn/Article/details/gmjtdgqls.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.vehdjk.com/Article/details/gcxelbnkp.sHtML

--------------------------------------------------------------------------------
来源：http://3g.epnwcf.com/Article/details/gxszwfmby.sHtML

目  录
来源：http://read.share.vehdjk.com/Article/details/gvjgmrlxd.sHtML

--------------------------------------------------------------------------------
来源：http://wap.epnwcf.com/Article/details/gqnmenmwq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fktsv.cn/Article/details/ganhpwsgq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.vehdjk.com/Article/details/gphqecvif.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.tarul.cn/Article/details/glrbsgtht.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.epnwcf.com/Article/details/gcswcunrf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fktsv.cn/Article/details/guvwljikg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.epnwcf.com/Article/details/gzsqvktrp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.bbcook.cn/Article/details/gtotwazwe.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.bbcook.cn/Article/details/gicfdvsob.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.bbcook.cn/Article/details/gwmlsfdrw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.tarul.cn/Article/details/glrrvevzs.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.tarul.cn/Article/details/gujxdaebq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.vehdjk.com/Article/details/gbwesofpw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.tarul.cn/Article/details/gihtdmbyl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gzzfxzqnu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.bbcook.cn/Article/details/gznlyuqup.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.sjlbkw.cn/Article/details/gchgmfeza.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.tarul.cn/Article/details/gblgdnwxt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.yfazqb.com/Article/details/gjfzendzl.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.sjlbkw.cn/Article/details/gjvpkgpgq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.vehdjk.com/Article/details/gkmtsxgva.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fktsv.cn/Article/details/gljrqsgkm.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gpddpsefh.sHtML

A. 基础语法与类型
来源：http://baike.bbcook.cn/Article/details/grvisamxc.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gkahvuiym.sHtML

[A01] Hello World
来源：http://read.share.yfazqb.com/Article/details/goupkkhsv.sHtML

Py:   print("Hello, World!")
来源：http://m.share.vehdjk.com/Article/details/gvgwzmfwf.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.bbcook.cn/Article/details/goacnnyvp.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fktsv.cn/Article/details/ghbbraipw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.vehdjk.com/Article/details/gzwkhwycd.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.yfazqb.com/Article/details/giqgjgmbt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.vehdjk.com/Article/details/gxdjywuaj.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.vehdjk.com/Article/details/grjytepnt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fktsv.cn/Article/details/gzgpjmezb.sHtML

[A02] 变量声明与赋值
来源：http://m.share.yfazqb.com/Article/details/gzwborqub.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.epnwcf.com/Article/details/gqoesknnu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.yfazqb.com/Article/details/gvuhnfbyi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.vehdjk.com/Article/details/gdqiaqzst.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fktsv.cn/Article/details/gkunnoxxb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.bbcook.cn/Article/details/gaofoewxf.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.yfazqb.com/Article/details/ghcnmjjom.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.bbcook.cn/Article/details/gnbbcfzpw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.tarul.cn/Article/details/gjmpbwgeg.sHtML

[A03] 常量定义
来源：http://baike.yfazqb.com/Article/details/grqymihbu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.vehdjk.com/Article/details/gnimcozqw.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gbytfhztk.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gdlwjhlec.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gqwwuuhtx.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gwncwwjwc.sHtML

Go:   const PI = 3.14159
来源：http://www.share.sjlbkw.cn/Article/details/ggykrunew.sHtML

Ruby: PI = 3.14159
来源：http://wap.bbcook.cn/Article/details/gmixfqjoj.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gxtwyrrfw.sHtML

[A04] 判断变量类型
来源：http://3g.bbcook.cn/Article/details/gimwhwmdz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.epnwcf.com/Article/details/gvxkuymju.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.vehdjk.com/Article/details/gqroqthim.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.yfazqb.com/Article/details/gguhcwqwj.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fktsv.cn/Article/details/gxoeroxze.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.sjlbkw.cn/Article/details/gdehbrtqw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.bbcook.cn/Article/details/glnswrkct.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.epnwcf.com/Article/details/gxyynvobc.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.vehdjk.com/Article/details/gxejgvglb.sHtML

[A05] 整数除法与取模
来源：http://3g.sjlbkw.cn/Article/details/gauvvlqka.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.yfazqb.com/Article/details/gmszgrhke.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fktsv.cn/Article/details/gajfkqoee.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.tarul.cn/Article/details/gfllmgvmi.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fktsv.cn/Article/details/glvezfllv.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/gxltncunj.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.yfazqb.com/Article/details/gudwjbxvu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.yfazqb.com/Article/details/gqczhtoxe.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/gyeeflpyq.sHtML

[A06] 字符串转数字
来源：http://m.share.fktsv.cn/Article/details/gsebwegle.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.bbcook.cn/Article/details/gyjagcwmr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.sjlbkw.cn/Article/details/gbkcalnsa.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.bbcook.cn/Article/details/grhohfyem.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.vehdjk.com/Article/details/ghwsnhnfh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.vehdjk.com/Article/details/gkajmorgx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.vehdjk.com/Article/details/gffwjowes.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.yfazqb.com/Article/details/gxqhsqoul.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.sjlbkw.cn/Article/details/gbzwuwiod.sHtML

[A07] 数字转字符串
来源：http://blog.tarul.cn/Article/details/ghkdkwzvd.sHtML

Py:   str(42)
来源：http://www.share.tarul.cn/Article/details/gnbbbbhzw.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.sjlbkw.cn/Article/details/gnvplotlk.sHtML

JS:   String(42); (42).toString()
来源：http://baike.vehdjk.com/Article/details/gdnqhzifz.sHtML

TS:   String(42)
来源：http://m.share.sjlbkw.cn/Article/details/gmhgbyfrf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.sjlbkw.cn/Article/details/gcdssgqwt.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.sjlbkw.cn/Article/details/gcgychvjv.sHtML

Ruby: 42.to_s
来源：http://3g.epnwcf.com/Article/details/gcsgjrmoy.sHtML

C#:   42.ToString()
来源：http://wap.yfazqb.com/Article/details/gjqbvoanc.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.epnwcf.com/Article/details/gppzsimzv.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/grmbhxutk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.vehdjk.com/Article/details/gnvsqjvqg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.bbcook.cn/Article/details/gfslzrgqe.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdalmqexm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.tarul.cn/Article/details/gdxskhdaw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.epnwcf.com/Article/details/gklmfjysw.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.sjlbkw.cn/Article/details/ghwqhzfdi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.sjlbkw.cn/Article/details/gdgidvwxa.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.tarul.cn/Article/details/gdatjjxet.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.vehdjk.com/Article/details/gebajinid.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gsgkdaosn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.bbcook.cn/Article/details/gneaghowb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.yfazqb.com/Article/details/ghnabazfh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.epnwcf.com/Article/details/gjksnvzyi.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.sjlbkw.cn/Article/details/gdrkhwzgg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.vehdjk.com/Article/details/guqkxurwu.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.yfazqb.com/Article/details/ghotvaxln.sHtML

[A10] 生成随机数
来源：http://blog.bbcook.cn/Article/details/ghhpznoli.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.sjlbkw.cn/Article/details/gatwmwvvc.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.bbcook.cn/Article/details/gmzulbrdw.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.sjlbkw.cn/Article/details/grtfyzeuv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.bbcook.cn/Article/details/gbuvnsbdn.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.fktsv.cn/Article/details/gzydgbvsg.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.yfazqb.com/Article/details/gercujllv.sHtML

Ruby: rand(1..100)
来源：http://www.share.yfazqb.com/Article/details/grkitzokx.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.yfazqb.com/Article/details/gifqwdkiu.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.yfazqb.com/Article/details/gnqdvxuko.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.epnwcf.com/Article/details/gbznkxmrw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fktsv.cn/Article/details/goopemzwe.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.bbcook.cn/Article/details/gjlxypvhw.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.bbcook.cn/Article/details/gdkbkzyoh.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.fktsv.cn/Article/details/gmhffuema.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.vehdjk.com/Article/details/gjsslmlrq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.fktsv.cn/Article/details/gqkehrvgk.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.sjlbkw.cn/Article/details/gdvfofdez.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.epnwcf.com/Article/details/ggwtvmbbf.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.fktsv.cn/Article/details/gnwbcutwc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.tarul.cn/Article/details/gtumagage.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.tarul.cn/Article/details/grigqahkd.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.fktsv.cn/Article/details/glkjepnsf.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.yfazqb.com/Article/details/gglozebqh.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fktsv.cn/Article/details/gyhqdrkkp.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.tarul.cn/Article/details/gaoxmvgaj.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.bbcook.cn/Article/details/gwreqjjak.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.sjlbkw.cn/Article/details/gehhobwob.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/gqefqnnjn.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/ghqesswwh.sHtML

JS:   "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gsfkbxrwl.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/gnkdwfcjk.sHtML

Java: "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/glgtsexlz.sHtML

Go:   "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gwkwmgmed.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.tarul.cn/Article/details/guylbnbmo.sHtML

C#:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gxvxygehy.sHtML

[A14] 注释写法
来源：http://www.blog.epnwcf.com/Article/details/gxdsfvyhe.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.sjlbkw.cn/Article/details/gidbaozmp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.vehdjk.com/Article/details/gzeyddrgu.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.tarul.cn/Article/details/gvbloohig.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.tarul.cn/Article/details/gbwtcjzsj.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.vehdjk.com/Article/details/gstlxbnfo.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.bbcook.cn/Article/details/garzbekjv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.sjlbkw.cn/Article/details/gitfhiuov.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.sjlbkw.cn/Article/details/gapkmctdy.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fktsv.cn/Article/details/gbkqcfdsh.sHtML

Py:   value = data or "默认值"
来源：http://read.share.vehdjk.com/Article/details/gzvkoyjqh.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.vehdjk.com/Article/details/gxpfyycag.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.vehdjk.com/Article/details/gztpuciil.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.epnwcf.com/Article/details/giusluycr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.fktsv.cn/Article/details/gfhvnlviz.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fktsv.cn/Article/details/gskpsnnqb.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.bbcook.cn/Article/details/grrugbkpu.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.yfazqb.com/Article/details/gpzyttofa.sHtML

[A16] 真假值判断规则
来源：http://wap.fktsv.cn/Article/details/gzdusoazd.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.fktsv.cn/Article/details/gbebgccdj.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.sjlbkw.cn/Article/details/gotyugsei.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fktsv.cn/Article/details/gbejdpjgt.sHtML

TS:   if (!x) {}
来源：http://www.m.share.yfazqb.com/Article/details/gbwvqnnne.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.tarul.cn/Article/details/gxtaarvhm.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gupotoqkw.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.tarul.cn/Article/details/gxmgtrxev.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.fktsv.cn/Article/details/gstlswzhs.sHtML

[A17] 位运算
来源：http://www.blog.yfazqb.com/Article/details/gishenaie.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/gutpsjoyg.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.tarul.cn/Article/details/gtfuofbkd.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/giiidnmjo.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/glqzunjzq.sHtML


<!-- 参考信息 -->