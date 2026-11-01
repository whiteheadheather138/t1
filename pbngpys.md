代发 wailian999

[U97] JS：并发请求
来源：http://mobile.epnwcf.com/Article/details/groctrupr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gusaxeoor.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.tarul.cn/Article/details/glxinfajt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.bbcook.cn/Article/details/gebaujijf.sHtML

[U99] JS：事件监听
来源：http://www.blog.bbcook.cn/Article/details/gyiekoqhl.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.vehdjk.com/Article/details/gcxuwcsli.sHtML

[U100] JS：DOM 查询
来源：http://baike.sjlbkw.cn/Article/details/gzdqxjckg.sHtML

document.querySelector(".item")
来源：http://www.blog.bbcook.cn/Article/details/glgzfyebj.sHtML

[U101] JS：classList 操作
来源：http://www.blog.sjlbkw.cn/Article/details/gjjfkcgqu.sHtML

el.classList.toggle("active")
来源：http://baike.fktsv.cn/Article/details/gtebsprot.sHtML

[U102] JS：本地存储
来源：http://www.blog.bbcook.cn/Article/details/gkdtaqkkw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.yfazqb.com/Article/details/gfuafcwgn.sHtML

[U103] JS：定时器
来源：http://read.share.yfazqb.com/Article/details/grurjixlo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.epnwcf.com/Article/details/gqeukxiax.sHtML

[U104] JS：防抖
来源：http://www.share.tarul.cn/Article/details/gvxtyghia.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/gkmeetngy.sHtML

[U105] JS：节流
来源：http://read.share.vehdjk.com/Article/details/gkhkaewkh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.vehdjk.com/Article/details/gkxmsljpf.sHtML

[U106] JS：日期格式化
来源：http://m.share.tarul.cn/Article/details/gbufhawuf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.epnwcf.com/Article/details/geptokeiz.sHtML

[U107] JS：数字千分位
来源：http://baike.yfazqb.com/Article/details/goigbpcgb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.vehdjk.com/Article/details/gsijrmefs.sHtML

[U108] JS：随机整数
来源：http://www.share.vehdjk.com/Article/details/gqabygvok.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.yfazqb.com/Article/details/gyhdoryiu.sHtML

[U109] JS：数组分组
来源：http://3g.tarul.cn/Article/details/gbivrathc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fktsv.cn/Article/details/ginpliimw.sHtML

[U110] JS：数组分块
来源：http://wap.yfazqb.com/Article/details/goxagbwnr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.epnwcf.com/Article/details/gxrmfckog.sHtML

[U111] JS：对象转 Map
来源：http://baike.yfazqb.com/Article/details/gdkjnsark.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.bbcook.cn/Article/details/grmuhnrue.sHtML

[U112] JS：字符串补位
来源：http://wap.bbcook.cn/Article/details/gblfasyho.sHtML

"7".padStart(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gwayflthx.sHtML

[U113] JS：正则替换全部
来源：http://read.share.tarul.cn/Article/details/gumsdtzon.sHtML

s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gsvilnvfk.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.vehdjk.com/Article/details/gkvvubble.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.sjlbkw.cn/Article/details/ggtojxtff.sHtML

[U115] JS：生成 UUID
来源：http://read.share.tarul.cn/Article/details/gymbudxcn.sHtML

crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gvtqejqoo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.sjlbkw.cn/Article/details/gltprmybu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.vehdjk.com/Article/details/ggyyrlzlu.sHtML

[U117] JS：单元测试
来源：http://m.share.vehdjk.com/Article/details/gwsreqrdw.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.bbcook.cn/Article/details/gpycvucwb.sHtML

[U118] JS：开发服务器
来源：http://3g.tarul.cn/Article/details/gzuiprjrf.sHtML

npm i -D vite;  npx vite
来源：http://baike.vehdjk.com/Article/details/gnomvnabo.sHtML

[U119] JS：生产构建
来源：http://m.share.fktsv.cn/Article/details/gkqalcgpk.sHtML

npx vite build
来源：http://read.share.tarul.cn/Article/details/gvglgbxna.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.yfazqb.com/Article/details/genuonjqj.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.sjlbkw.cn/Article/details/ghnyeztrc.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/giidbthgf.sHtML

统计汇总
来源：http://m.share.epnwcf.com/Article/details/gdtfbffgm.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gurzheunb.sHtML

按语言统计（条）：
来源：http://read.share.sjlbkw.cn/Article/details/goeziznuf.sHtML

Python ......... 252
来源：http://mobile.tarul.cn/Article/details/gjflgwffp.sHtML

PHP ............ 252
来源：http://read.share.yfazqb.com/Article/details/grgfgzsqy.sHtML

JavaScript ..... 252
来源：http://www.m.share.vehdjk.com/Article/details/grljkgjzj.sHtML

TypeScript ..... 212
来源：http://read.share.vehdjk.com/Article/details/guwiiadbk.sHtML

Java ........... 212
来源：http://wap.epnwcf.com/Article/details/gyftslnky.sHtML

Go ............. 212
来源：http://www.share.fktsv.cn/Article/details/gpavsgsre.sHtML

Ruby ........... 212
来源：http://wap.yfazqb.com/Article/details/gaxgwdsbh.sHtML

C# ............. 212
来源：http://wap.bbcook.cn/Article/details/ghgqlagup.sHtML

C .............. 30
来源：http://read.share.vehdjk.com/Article/details/gnudfnwxc.sHtML

C++ ............ 30
来源：http://www.share.fktsv.cn/Article/details/gnugjffzo.sHtML

SQL ............ 90
来源：http://read.share.vehdjk.com/Article/details/gwdyhirnn.sHtML

Bash ........... 80
来源：http://www.m.share.epnwcf.com/Article/details/gzxzyyjwi.sHtML

Kotlin ......... 15
来源：http://3g.fktsv.cn/Article/details/geavabrdq.sHtML

Swift .......... 15
来源：http://wap.tarul.cn/Article/details/gixzcikdh.sHtML

Lua ............ 10
来源：http://read.share.fktsv.cn/Article/details/gygtuwclf.sHtML

Perl ........... 10
来源：http://mobile.sjlbkw.cn/Article/details/gpdoknhoz.sHtML

Scala .......... 10
来源：http://www.m.share.tarul.cn/Article/details/gitqvjocc.sHtML

------------------------------------
来源：http://www.share.vehdjk.com/Article/details/gdqdyrjzj.sHtML

合计 ........... 2106 条
来源：http://3g.vehdjk.com/Article/details/gvqifsykm.sHtML

按章节统计：
来源：http://wap.fktsv.cn/Article/details/gdhjiaamp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.tarul.cn/Article/details/goatiruyh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.vehdjk.com/Article/details/grjqwymqz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.vehdjk.com/Article/details/gbxxqlcjf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.bbcook.cn/Article/details/grzcdhsfk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.tarul.cn/Article/details/gxvlhldeo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.sjlbkw.cn/Article/details/glgpcxstt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.yfazqb.com/Article/details/gtevmctaf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.tarul.cn/Article/details/gcalfwxyq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/gfxklhius.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.yfazqb.com/Article/details/gldyvaxyf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnjpmqoh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.sjlbkw.cn/Article/details/gxvcgpnzg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/ggycayvqk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.sjlbkw.cn/Article/details/ghowptyry.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.yfazqb.com/Article/details/gapkfdpsa.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/ghwiuzexo.sHtML

Q SQL 专题                              90
来源：http://wap.fktsv.cn/Article/details/gsudhzicl.sHtML

R Bash 专题                             80
来源：http://3g.fktsv.cn/Article/details/gyzlsxeix.sHtML

S C / C++ 专题                          60
来源：http://read.share.fktsv.cn/Article/details/gviydgpka.sHtML

T 其他语言补充                          60
来源：http://www.blog.tarul.cn/Article/details/gapzuhgyx.sHtML

U 高频实用片段                         120
来源：http://blog.yfazqb.com/Article/details/gwzejcnfj.sHtML

------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/gksduueig.sHtML

合计                                  2106 条
来源：http://3g.epnwcf.com/Article/details/gsvmvhogo.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gojoiwvjh.sHtML

使用提醒
来源：http://m.share.vehdjk.com/Article/details/gudrdueps.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gruhjtryq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.tarul.cn/Article/details/gjgkpvzfi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.bbcook.cn/Article/details/gtigojesh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.epnwcf.com/Article/details/gcrccnshh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.vehdjk.com/Article/details/gkybauiyv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.bbcook.cn/Article/details/gahnvfllw.sHtML

—— 文件结束 ——
来源：http://blog.bbcook.cn/Article/details/gdzamyone.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gonsqgisb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.vehdjk.com/Article/details/gjfzrchmi.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.tarul.cn/Article/details/gkangqfja.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gziztygll.sHtML

【收录内容】
来源：http://wap.vehdjk.com/Article/details/gguwxrlrx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.bbcook.cn/Article/details/guwngtydc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.sjlbkw.cn/Article/details/gltmyqjkh.sHtML

SQL · Bash · C · C++
来源：http://baike.vehdjk.com/Article/details/griweujzb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.bbcook.cn/Article/details/gfkqwlmyu.sHtML

【使用说明】
来源：http://m.share.epnwcf.com/Article/details/gdvnouhav.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.tarul.cn/Article/details/gpfusobla.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.sjlbkw.cn/Article/details/grugsyxln.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.bbcook.cn/Article/details/gnpeouaba.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.sjlbkw.cn/Article/details/gbjqzzhqy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fktsv.cn/Article/details/gbcporjim.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fktsv.cn/Article/details/gtxrkhtcf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.vehdjk.com/Article/details/gmyjctidk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.sjlbkw.cn/Article/details/ggivcilth.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.bbcook.cn/Article/details/gdblnxonf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.vehdjk.com/Article/details/gdscroxdo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.epnwcf.com/Article/details/gpbsevavn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.vehdjk.com/Article/details/gbbjnimha.sHtML

【文件统计】
来源：http://blog.vehdjk.com/Article/details/gvsqhfbea.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.epnwcf.com/Article/details/goorujzdf.sHtML

--------------------------------------------------------------------------------
来源：http://wap.epnwcf.com/Article/details/gqxiasxvi.sHtML

目  录
来源：http://wap.yfazqb.com/Article/details/gphbqqrwc.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gatixlbuu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.sjlbkw.cn/Article/details/gaiwvgula.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.sjlbkw.cn/Article/details/gktlmwjrt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.tarul.cn/Article/details/gamhsvfmw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fktsv.cn/Article/details/grooioeba.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.epnwcf.com/Article/details/gjwqjagzi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.sjlbkw.cn/Article/details/gulguqkcv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.epnwcf.com/Article/details/gneapkfeg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.epnwcf.com/Article/details/gibxkgbxb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fktsv.cn/Article/details/gayenidhu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.bbcook.cn/Article/details/grbymbcxb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.bbcook.cn/Article/details/gkaoavbge.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gesykeoez.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.vehdjk.com/Article/details/gxlhxolyk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.sjlbkw.cn/Article/details/gxuiucygd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.tarul.cn/Article/details/gfkhqrmlh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.yfazqb.com/Article/details/gmlgcrdhd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.tarul.cn/Article/details/gzbrewrom.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.sjlbkw.cn/Article/details/gbrrivybj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.epnwcf.com/Article/details/gtptkvpdv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fktsv.cn/Article/details/gisprxwuz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.bbcook.cn/Article/details/glnmzxogh.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/grupmsrcj.sHtML

A. 基础语法与类型
来源：http://www.blog.yfazqb.com/Article/details/gihsxlekz.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gvymzmbro.sHtML

[A01] Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gmimdesjk.sHtML

Py:   print("Hello, World!")
来源：http://www.share.sjlbkw.cn/Article/details/gwgteztsh.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.bbcook.cn/Article/details/giypuwxcw.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.yfazqb.com/Article/details/ghmemzghm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fktsv.cn/Article/details/gqtuwxvkf.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fktsv.cn/Article/details/gpcgnxgxg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.sjlbkw.cn/Article/details/gnlbqedwx.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.yfazqb.com/Article/details/gjooacwat.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.bbcook.cn/Article/details/gaecwjdkn.sHtML

[A02] 变量声明与赋值
来源：http://m.share.yfazqb.com/Article/details/gfudnvdhq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.sjlbkw.cn/Article/details/gpeejshum.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.vehdjk.com/Article/details/gcmfqxaar.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.tarul.cn/Article/details/gwdtgbudg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.bbcook.cn/Article/details/gvmeniand.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.yfazqb.com/Article/details/gcmxkzchw.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.yfazqb.com/Article/details/gdftvuksr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.epnwcf.com/Article/details/gzfixargw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fktsv.cn/Article/details/grkgheayd.sHtML

[A03] 常量定义
来源：http://www.share.epnwcf.com/Article/details/gimjxzogb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.vehdjk.com/Article/details/gajzresga.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gayxzpwmf.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/glrtsbifl.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gjcdemuhx.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gmpclincn.sHtML

Go:   const PI = 3.14159
来源：http://m.share.yfazqb.com/Article/details/gybqwnhhy.sHtML

Ruby: PI = 3.14159
来源：http://baike.bbcook.cn/Article/details/gfxdsrrpl.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gcobqxumc.sHtML

[A04] 判断变量类型
来源：http://wap.bbcook.cn/Article/details/gcrxaclxb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.bbcook.cn/Article/details/gtdqdfpdi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.bbcook.cn/Article/details/gyfzercye.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.bbcook.cn/Article/details/gfydkvzzo.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.bbcook.cn/Article/details/gdohpzbyn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.bbcook.cn/Article/details/giwzsokwh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.bbcook.cn/Article/details/goidlnqcd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.epnwcf.com/Article/details/gdswzabxw.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.sjlbkw.cn/Article/details/gshcwhgcy.sHtML

[A05] 整数除法与取模
来源：http://www.share.sjlbkw.cn/Article/details/gjhstpxwp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.fktsv.cn/Article/details/gxxzbryub.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.vehdjk.com/Article/details/gnqqjjzde.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.vehdjk.com/Article/details/ghtklpsac.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.bbcook.cn/Article/details/gmsciwwni.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.bbcook.cn/Article/details/gxvympvpo.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.epnwcf.com/Article/details/giueavmdg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.bbcook.cn/Article/details/goxssbtxv.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.epnwcf.com/Article/details/gwxnejqbp.sHtML

[A06] 字符串转数字
来源：http://read.share.epnwcf.com/Article/details/gxeodncav.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fktsv.cn/Article/details/guzfgdesy.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.epnwcf.com/Article/details/gyvpvcrix.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.sjlbkw.cn/Article/details/gecinzjdg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.tarul.cn/Article/details/gafnvscyx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.epnwcf.com/Article/details/glbvmvifq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.vehdjk.com/Article/details/gwvfiazdu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.bbcook.cn/Article/details/grqfinbxa.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.epnwcf.com/Article/details/gvwghuklu.sHtML

[A07] 数字转字符串
来源：http://www.blog.epnwcf.com/Article/details/gkzckqfsu.sHtML

Py:   str(42)
来源：http://blog.fktsv.cn/Article/details/gskmzwegc.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.epnwcf.com/Article/details/guuvqhrok.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fktsv.cn/Article/details/gpunlhscj.sHtML

TS:   String(42)
来源：http://blog.bbcook.cn/Article/details/gtkakrkfo.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.yfazqb.com/Article/details/gkvfgkcpg.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.bbcook.cn/Article/details/gclnshviq.sHtML

Ruby: 42.to_s
来源：http://wap.vehdjk.com/Article/details/gofdfjadr.sHtML

C#:   42.ToString()
来源：http://www.blog.vehdjk.com/Article/details/gwgfnkigk.sHtML

[A08] 取整与四舍五入
来源：http://blog.tarul.cn/Article/details/gajyduueh.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.vehdjk.com/Article/details/gvjftxmos.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.bbcook.cn/Article/details/goglsgkdp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fktsv.cn/Article/details/geubdynfk.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.epnwcf.com/Article/details/gslvyneux.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.tarul.cn/Article/details/gmzrncsdk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/gmagvpfsc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.vehdjk.com/Article/details/gdxugfdkj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.tarul.cn/Article/details/gxnvjyvum.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.bbcook.cn/Article/details/gwgfntcfe.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.epnwcf.com/Article/details/grfjmbprb.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gzmdlxgfu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/gmzwvrwqy.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.yfazqb.com/Article/details/gtuhchzgv.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.yfazqb.com/Article/details/gvlnawusa.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.vehdjk.com/Article/details/ggjxrrxlg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.yfazqb.com/Article/details/gfvkvrpjs.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.tarul.cn/Article/details/gqfudyttv.sHtML

[A10] 生成随机数
来源：http://wap.bbcook.cn/Article/details/gcpquqcow.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.tarul.cn/Article/details/gjqmsucrv.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.tarul.cn/Article/details/gagsoeomi.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.sjlbkw.cn/Article/details/gtpcvjxij.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fktsv.cn/Article/details/gswcbflej.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.epnwcf.com/Article/details/gnhuzkvyo.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.sjlbkw.cn/Article/details/gnjerfxqu.sHtML

Ruby: rand(1..100)
来源：http://wap.tarul.cn/Article/details/gjsagxbbd.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.bbcook.cn/Article/details/gqczwczco.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.fktsv.cn/Article/details/gvrvghenk.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.tarul.cn/Article/details/gjdeycfki.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fktsv.cn/Article/details/gzbghlwbb.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.epnwcf.com/Article/details/grvdixslf.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.yfazqb.com/Article/details/gztcubnxe.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.bbcook.cn/Article/details/gmajeiyqt.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.epnwcf.com/Article/details/gzxtpnxal.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/gosaluogo.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.bbcook.cn/Article/details/gkfenijma.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.yfazqb.com/Article/details/gsnvmdcax.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.fktsv.cn/Article/details/gupjzhwor.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.tarul.cn/Article/details/gasjgswfb.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.bbcook.cn/Article/details/glekxiunm.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.vehdjk.com/Article/details/gpyaastet.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.epnwcf.com/Article/details/gqtvvjrln.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.bbcook.cn/Article/details/ghxrmqcmp.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fktsv.cn/Article/details/gvktiotzg.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.epnwcf.com/Article/details/gdsnsksjm.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.vehdjk.com/Article/details/gntthhxlj.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/gibhqxxrt.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fktsv.cn/Article/details/gptyzfhtu.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/gxbkxtthd.sHtML

TS:   "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/gqlszzqtd.sHtML

Java: "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gkjxvsqcu.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/gggxjjxsb.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fktsv.cn/Article/details/glygwlwhe.sHtML

C#:   "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/gedvfegbs.sHtML

[A14] 注释写法
来源：http://mobile.vehdjk.com/Article/details/gpughtotw.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fktsv.cn/Article/details/gabpzyauw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.sjlbkw.cn/Article/details/gfibaytvy.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.tarul.cn/Article/details/gdvmqjdlt.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.yfazqb.com/Article/details/gopqasybm.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.fktsv.cn/Article/details/gxmqwylbd.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.epnwcf.com/Article/details/gbtwuebct.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fktsv.cn/Article/details/gvlzdmvds.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.tarul.cn/Article/details/glgimoxpi.sHtML

[A15] 空值判断与默认值
来源：http://baike.yfazqb.com/Article/details/gksdlbvqa.sHtML

Py:   value = data or "默认值"
来源：http://mobile.yfazqb.com/Article/details/gedwjspja.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.vehdjk.com/Article/details/gybchgejt.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.vehdjk.com/Article/details/goesyiuly.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.bbcook.cn/Article/details/gigozqdpi.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcdjigaa.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.yfazqb.com/Article/details/gjqgjvxvb.sHtML

Ruby: value = data || "默认值"
来源：http://3g.tarul.cn/Article/details/gjdcugmln.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.vehdjk.com/Article/details/gvgknkhhu.sHtML

[A16] 真假值判断规则
来源：http://mobile.yfazqb.com/Article/details/glyxdxxnz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.epnwcf.com/Article/details/gxnrjjdwb.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.sjlbkw.cn/Article/details/gfgzqdxzi.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.epnwcf.com/Article/details/gbxiybiar.sHtML

TS:   if (!x) {}
来源：http://mobile.fktsv.cn/Article/details/gncjglzql.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.epnwcf.com/Article/details/gdjvlibuw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.epnwcf.com/Article/details/gszpynwea.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.fktsv.cn/Article/details/gbuddzwue.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.fktsv.cn/Article/details/glxwqqzag.sHtML

[A17] 位运算
来源：http://www.m.share.fktsv.cn/Article/details/gzwjhhpjc.sHtML


<!-- 参考信息 -->