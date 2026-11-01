代发 wailian999

[U99] JS：事件监听
来源：http://wap.sjlbkw.cn/Article/details/gtctxkruz.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fktsv.cn/Article/details/gddjaglpx.sHtML

[U100] JS：DOM 查询
来源：http://wap.fktsv.cn/Article/details/godvnawui.sHtML

document.querySelector(".item")
来源：http://wap.bbcook.cn/Article/details/gixuncxik.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.vehdjk.com/Article/details/gyhiecler.sHtML

el.classList.toggle("active")
来源：http://baike.sjlbkw.cn/Article/details/gqydrafor.sHtML

[U102] JS：本地存储
来源：http://wap.epnwcf.com/Article/details/gyjrybget.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.tarul.cn/Article/details/gqaqeegex.sHtML

[U103] JS：定时器
来源：http://www.m.share.tarul.cn/Article/details/guyaryjet.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.epnwcf.com/Article/details/ggetrevwg.sHtML

[U104] JS：防抖
来源：http://wap.tarul.cn/Article/details/giwzfvtsn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/gpldikbir.sHtML

[U105] JS：节流
来源：http://www.share.fktsv.cn/Article/details/gxakmidhv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.epnwcf.com/Article/details/gteiaqdwi.sHtML

[U106] JS：日期格式化
来源：http://www.share.bbcook.cn/Article/details/gyeaogwcq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fktsv.cn/Article/details/ghwuajbva.sHtML

[U107] JS：数字千分位
来源：http://3g.yfazqb.com/Article/details/goigbfele.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.epnwcf.com/Article/details/gllspqnuq.sHtML

[U108] JS：随机整数
来源：http://read.share.sjlbkw.cn/Article/details/gdhodzmms.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.vehdjk.com/Article/details/gumvbrrus.sHtML

[U109] JS：数组分组
来源：http://baike.tarul.cn/Article/details/gjyhfhzmo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.vehdjk.com/Article/details/geedlwzcs.sHtML

[U110] JS：数组分块
来源：http://www.m.share.tarul.cn/Article/details/gwtnswmgh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.sjlbkw.cn/Article/details/gxnktrzcm.sHtML

[U111] JS：对象转 Map
来源：http://www.share.yfazqb.com/Article/details/gdrtfjtfj.sHtML

new Map(Object.entries(obj))
来源：http://wap.fktsv.cn/Article/details/gxxpazqwi.sHtML

[U112] JS：字符串补位
来源：http://www.blog.tarul.cn/Article/details/gxivnuhsp.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcmnfnvp.sHtML

[U113] JS：正则替换全部
来源：http://wap.fktsv.cn/Article/details/giqsrbecg.sHtML

s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gytpwkrue.sHtML

[U114] JS：JSON 深比较
来源：http://wap.epnwcf.com/Article/details/gcylunhis.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.vehdjk.com/Article/details/gvwdphpaf.sHtML

[U115] JS：生成 UUID
来源：http://read.share.vehdjk.com/Article/details/gvclcttkj.sHtML

crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gpgqcjdau.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.epnwcf.com/Article/details/gihsjwrjy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.epnwcf.com/Article/details/gzbbfwdaj.sHtML

[U117] JS：单元测试
来源：http://www.blog.fktsv.cn/Article/details/gdjqorrnp.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.bbcook.cn/Article/details/gatwmiubn.sHtML

[U118] JS：开发服务器
来源：http://read.share.fktsv.cn/Article/details/gdkmdvwpm.sHtML

npm i -D vite;  npx vite
来源：http://read.share.yfazqb.com/Article/details/gxvkxphdo.sHtML

[U119] JS：生产构建
来源：http://www.m.share.yfazqb.com/Article/details/gmmlekttu.sHtML

npx vite build
来源：http://m.share.bbcook.cn/Article/details/gkhxbicbr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.bbcook.cn/Article/details/glsjfubut.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzjekfye.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gyufrwsra.sHtML

统计汇总
来源：http://www.m.share.tarul.cn/Article/details/gbxdzzmcd.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gbudolnwz.sHtML

按语言统计（条）：
来源：http://wap.bbcook.cn/Article/details/gkiheizqe.sHtML

Python ......... 252
来源：http://www.blog.vehdjk.com/Article/details/gaebbvnhp.sHtML

PHP ............ 252
来源：http://read.share.sjlbkw.cn/Article/details/gvbhkrpym.sHtML

JavaScript ..... 252
来源：http://baike.epnwcf.com/Article/details/gwltxjfou.sHtML

TypeScript ..... 212
来源：http://m.share.fktsv.cn/Article/details/goradwtxp.sHtML

Java ........... 212
来源：http://www.blog.vehdjk.com/Article/details/gemsxtcnd.sHtML

Go ............. 212
来源：http://3g.vehdjk.com/Article/details/gxxlgmmhz.sHtML

Ruby ........... 212
来源：http://www.blog.fktsv.cn/Article/details/gzsuwdiqy.sHtML

C# ............. 212
来源：http://blog.vehdjk.com/Article/details/gvxplxnvy.sHtML

C .............. 30
来源：http://m.share.bbcook.cn/Article/details/gkjpjsucf.sHtML

C++ ............ 30
来源：http://mobile.bbcook.cn/Article/details/guwapjmnr.sHtML

SQL ............ 90
来源：http://read.share.epnwcf.com/Article/details/gdqakdsgd.sHtML

Bash ........... 80
来源：http://baike.vehdjk.com/Article/details/giayemezx.sHtML

Kotlin ......... 15
来源：http://www.blog.tarul.cn/Article/details/gxuufmozm.sHtML

Swift .......... 15
来源：http://wap.sjlbkw.cn/Article/details/gefzqaioe.sHtML

Lua ............ 10
来源：http://www.blog.bbcook.cn/Article/details/gaauoldhj.sHtML

Perl ........... 10
来源：http://www.m.share.fktsv.cn/Article/details/gszyttrjd.sHtML

Scala .......... 10
来源：http://www.blog.tarul.cn/Article/details/ghnygdhay.sHtML

------------------------------------
来源：http://mobile.tarul.cn/Article/details/gmgclkcqm.sHtML

合计 ........... 2106 条
来源：http://3g.fktsv.cn/Article/details/gmxncecju.sHtML

按章节统计：
来源：http://m.share.yfazqb.com/Article/details/guypeghja.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fktsv.cn/Article/details/gucuwifyn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.bbcook.cn/Article/details/gaksrwfqr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fktsv.cn/Article/details/gqrblaudu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.vehdjk.com/Article/details/grpinhbio.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fktsv.cn/Article/details/gingfyval.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.bbcook.cn/Article/details/giparhzwx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.tarul.cn/Article/details/gyulfktxu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.bbcook.cn/Article/details/gqgoogqpk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/gmltgwwvt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.sjlbkw.cn/Article/details/gujufmdep.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gjjiseryi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gfscbbxan.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/ghmzfbuhg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.sjlbkw.cn/Article/details/gbnypgjou.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.bbcook.cn/Article/details/gxpnonnmf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/gjjydjhwu.sHtML

Q SQL 专题                              90
来源：http://blog.vehdjk.com/Article/details/gestryfxr.sHtML

R Bash 专题                             80
来源：http://mobile.fktsv.cn/Article/details/giwnruerp.sHtML

S C / C++ 专题                          60
来源：http://m.share.fktsv.cn/Article/details/grztwojkb.sHtML

T 其他语言补充                          60
来源：http://read.share.tarul.cn/Article/details/gkjuncrzp.sHtML

U 高频实用片段                         120
来源：http://wap.vehdjk.com/Article/details/grpazusgg.sHtML

------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/grhceogln.sHtML

合计                                  2106 条
来源：http://mobile.bbcook.cn/Article/details/gkmpbsptv.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/gexnyoekg.sHtML

使用提醒
来源：http://wap.vehdjk.com/Article/details/gstmnfbsp.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fktsv.cn/Article/details/gktvylvfc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fktsv.cn/Article/details/gmwbswoxd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.tarul.cn/Article/details/gjeyzfrnj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.bbcook.cn/Article/details/gciomexwi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.vehdjk.com/Article/details/gtbzzqmoa.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.sjlbkw.cn/Article/details/gepyjqlnz.sHtML

—— 文件结束 ——
来源：http://blog.vehdjk.com/Article/details/gdedtbsiq.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/grbcydvup.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.yfazqb.com/Article/details/gnefoxjsd.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.vehdjk.com/Article/details/govdavbdj.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gqqpyytbj.sHtML

【收录内容】
来源：http://read.share.tarul.cn/Article/details/gabqwsvtv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.yfazqb.com/Article/details/girzasjji.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.tarul.cn/Article/details/gdcsagvrq.sHtML

SQL · Bash · C · C++
来源：http://m.share.yfazqb.com/Article/details/gkzhcxwua.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fktsv.cn/Article/details/gjndqtjff.sHtML

【使用说明】
来源：http://www.blog.epnwcf.com/Article/details/gvegwjolt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fktsv.cn/Article/details/gpsjhxnam.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.bbcook.cn/Article/details/golrkwyhg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.sjlbkw.cn/Article/details/gbgifjqzj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fktsv.cn/Article/details/gpcwxveux.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.yfazqb.com/Article/details/ggnurpdhp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.tarul.cn/Article/details/gkcjuhenz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.vehdjk.com/Article/details/gydcfifrh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.bbcook.cn/Article/details/gjqmvmxlp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.vehdjk.com/Article/details/gemvpbsbz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.vehdjk.com/Article/details/graefyjob.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.sjlbkw.cn/Article/details/gwrbqiupz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.vehdjk.com/Article/details/gzuydvbsm.sHtML

【文件统计】
来源：http://www.blog.epnwcf.com/Article/details/gbqgfkdgx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.sjlbkw.cn/Article/details/gvdnwjdgb.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.bbcook.cn/Article/details/gukmkrows.sHtML

目  录
来源：http://mobile.bbcook.cn/Article/details/gidpwykio.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.bbcook.cn/Article/details/guzbkwxzh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.yfazqb.com/Article/details/gbzloqxsp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fktsv.cn/Article/details/glqenezbo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fktsv.cn/Article/details/girlpvbgf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.vehdjk.com/Article/details/gaacrajne.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.vehdjk.com/Article/details/gdrtqqcnd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.sjlbkw.cn/Article/details/gntmygvcb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.tarul.cn/Article/details/gysfbqdrx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.yfazqb.com/Article/details/gqvcjpkhc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gzeumxkxl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.vehdjk.com/Article/details/gypelhpbp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/geqlrnolv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/gqagwkijc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.tarul.cn/Article/details/gxbrnjxca.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.sjlbkw.cn/Article/details/gpzhhbupg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fktsv.cn/Article/details/gjsycthsk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/gwgmgohvv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.sjlbkw.cn/Article/details/glkljiwgr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.yfazqb.com/Article/details/gxdnowapa.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.sjlbkw.cn/Article/details/galmlxwlk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.tarul.cn/Article/details/giogfmkwb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.epnwcf.com/Article/details/givmbwojv.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gxyvqzxzs.sHtML

A. 基础语法与类型
来源：http://wap.vehdjk.com/Article/details/gtkhdsjki.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gxynyuidb.sHtML

[A01] Hello World
来源：http://3g.epnwcf.com/Article/details/garworfir.sHtML

Py:   print("Hello, World!")
来源：http://www.share.bbcook.cn/Article/details/gqlaetkqi.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.vehdjk.com/Article/details/ghksymbwm.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fktsv.cn/Article/details/gddsnlqnu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.epnwcf.com/Article/details/gjbdbcmux.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.epnwcf.com/Article/details/goujprbjs.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.sjlbkw.cn/Article/details/gikebgzjf.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.yfazqb.com/Article/details/gxscinrih.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.sjlbkw.cn/Article/details/gfoymagfm.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fktsv.cn/Article/details/giiesamhf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.yfazqb.com/Article/details/gsquipdis.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.sjlbkw.cn/Article/details/gpknqwbyo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwxerzzd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.tarul.cn/Article/details/gsfaqxyer.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fktsv.cn/Article/details/gwmgucsip.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.yfazqb.com/Article/details/gjcojhkiw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.yfazqb.com/Article/details/gwdzhbzku.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fktsv.cn/Article/details/gdgppaphi.sHtML

[A03] 常量定义
来源：http://wap.bbcook.cn/Article/details/glbmcyrrs.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.vehdjk.com/Article/details/gszdeubep.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fktsv.cn/Article/details/gvihvynkm.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gyicihaxc.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gwacszjwe.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gmlvvppee.sHtML

Go:   const PI = 3.14159
来源：http://www.share.tarul.cn/Article/details/gjphpromf.sHtML

Ruby: PI = 3.14159
来源：http://m.share.vehdjk.com/Article/details/gcecioekq.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/givbmpqyr.sHtML

[A04] 判断变量类型
来源：http://read.share.vehdjk.com/Article/details/gzoavlgns.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.bbcook.cn/Article/details/gycpaqtww.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.vehdjk.com/Article/details/gtlfosvmg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.epnwcf.com/Article/details/gngmnnvbe.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.bbcook.cn/Article/details/geilvetaq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.epnwcf.com/Article/details/gpfutlmjf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.bbcook.cn/Article/details/ggqyamgsw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.bbcook.cn/Article/details/gyotoctie.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.yfazqb.com/Article/details/gwyjdpcls.sHtML

[A05] 整数除法与取模
来源：http://www.share.epnwcf.com/Article/details/gqkxavpkb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.sjlbkw.cn/Article/details/gkzvghjdb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/gahsjbehe.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.bbcook.cn/Article/details/gewwsijof.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/gnmqtnpdc.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.yfazqb.com/Article/details/grjbvhkfa.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/gtaqxzugc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/gnhznyipl.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fktsv.cn/Article/details/gtlydggko.sHtML

[A06] 字符串转数字
来源：http://baike.tarul.cn/Article/details/ghrbkbxyz.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.yfazqb.com/Article/details/guxihnaaj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.epnwcf.com/Article/details/gdvdirotn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.yfazqb.com/Article/details/gomozrdnx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.vehdjk.com/Article/details/gmnepcicx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.tarul.cn/Article/details/geaowgyqt.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.vehdjk.com/Article/details/gxpvjujio.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.tarul.cn/Article/details/gsgixzoge.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.sjlbkw.cn/Article/details/gehslijqb.sHtML

[A07] 数字转字符串
来源：http://m.share.vehdjk.com/Article/details/gdcysmjhs.sHtML

Py:   str(42)
来源：http://read.share.fktsv.cn/Article/details/gizomrfps.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.yfazqb.com/Article/details/gueozhjql.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.epnwcf.com/Article/details/gkwxudpiw.sHtML

TS:   String(42)
来源：http://m.share.tarul.cn/Article/details/ghoszpxgl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.sjlbkw.cn/Article/details/geieduewa.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.epnwcf.com/Article/details/gwicxuslg.sHtML

Ruby: 42.to_s
来源：http://read.share.epnwcf.com/Article/details/ghsyrxtep.sHtML

C#:   42.ToString()
来源：http://www.blog.bbcook.cn/Article/details/gkwivvsbj.sHtML

[A08] 取整与四舍五入
来源：http://m.share.epnwcf.com/Article/details/gvpgqhlwt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.tarul.cn/Article/details/gijbxlius.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.epnwcf.com/Article/details/gdyuoxadd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.bbcook.cn/Article/details/ghqjqmkju.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.tarul.cn/Article/details/gfnmviijt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.yfazqb.com/Article/details/guonrfihd.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.yfazqb.com/Article/details/gfegtswdh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.bbcook.cn/Article/details/geodutiaf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.sjlbkw.cn/Article/details/gncjrupoo.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fktsv.cn/Article/details/gxrfarcqm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.yfazqb.com/Article/details/gqviulfhn.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.yfazqb.com/Article/details/gkjbchdqk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.epnwcf.com/Article/details/ghbqytiyv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.yfazqb.com/Article/details/gjhrfqboy.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.epnwcf.com/Article/details/ggorovevy.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fktsv.cn/Article/details/gmppzaoql.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.sjlbkw.cn/Article/details/ggxqskyxx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gcmlvwrrd.sHtML

[A10] 生成随机数
来源：http://baike.sjlbkw.cn/Article/details/gbtvudstp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fktsv.cn/Article/details/gmrzdqogb.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.vehdjk.com/Article/details/gapwmmpum.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.yfazqb.com/Article/details/gbcmvulmi.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.epnwcf.com/Article/details/gdektiqsf.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.bbcook.cn/Article/details/gbxgnemcs.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.tarul.cn/Article/details/gqdgnlbwk.sHtML

Ruby: rand(1..100)
来源：http://mobile.sjlbkw.cn/Article/details/gbrcbxphk.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.bbcook.cn/Article/details/gitkithdy.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.fktsv.cn/Article/details/gdiihsuta.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.bbcook.cn/Article/details/ggdehefkk.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.epnwcf.com/Article/details/gltztlaln.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.epnwcf.com/Article/details/gpazhffbz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.fktsv.cn/Article/details/gfjirremm.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.vehdjk.com/Article/details/gwdrvfctw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.bbcook.cn/Article/details/gguwbtvei.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.yfazqb.com/Article/details/gryelhbif.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.tarul.cn/Article/details/gceebbens.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.sjlbkw.cn/Article/details/grmydkapu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.yfazqb.com/Article/details/gxbkhbsid.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.bbcook.cn/Article/details/gpdjdpsol.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.bbcook.cn/Article/details/gxdmiufnv.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.vehdjk.com/Article/details/gtawnpodm.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.epnwcf.com/Article/details/gooregqwv.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.sjlbkw.cn/Article/details/ghwedmfqy.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.epnwcf.com/Article/details/gostivfnf.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.sjlbkw.cn/Article/details/gthudebal.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.vehdjk.com/Article/details/gzkhuebdx.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.vehdjk.com/Article/details/gztgxlqed.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.yfazqb.com/Article/details/gblggkpyb.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/gcbmygszv.sHtML

TS:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gtxaimrbu.sHtML

Java: "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/gpbghuojs.sHtML

Go:   "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gbqstqkky.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gxhebhhes.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.tarul.cn/Article/details/gwqzlqtrj.sHtML

[A14] 注释写法
来源：http://3g.epnwcf.com/Article/details/gotvjvwjt.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.vehdjk.com/Article/details/gqokabqsc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.yfazqb.com/Article/details/gycwawscp.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.sjlbkw.cn/Article/details/gvqfvmtzg.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.vehdjk.com/Article/details/gftdgtafa.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.tarul.cn/Article/details/gdjsbjfxl.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fktsv.cn/Article/details/glliwkudc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.tarul.cn/Article/details/glhrfwlqe.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.vehdjk.com/Article/details/guqhykhxj.sHtML

[A15] 空值判断与默认值
来源：http://3g.yfazqb.com/Article/details/gflfvciyc.sHtML

Py:   value = data or "默认值"
来源：http://3g.vehdjk.com/Article/details/gubtkaszu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.fktsv.cn/Article/details/ghtpbolyf.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.bbcook.cn/Article/details/gxzhkfsoz.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.bbcook.cn/Article/details/gbusobuxx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.sjlbkw.cn/Article/details/gutlyusyh.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.bbcook.cn/Article/details/gtztxsbcg.sHtML

Ruby: value = data || "默认值"
来源：http://wap.vehdjk.com/Article/details/gtqrgjhht.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.bbcook.cn/Article/details/gwfztanks.sHtML

[A16] 真假值判断规则
来源：http://3g.yfazqb.com/Article/details/gbawnwzta.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.epnwcf.com/Article/details/gwqdxahnn.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.sjlbkw.cn/Article/details/galpqiwpp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.tarul.cn/Article/details/gsogcpqmc.sHtML

TS:   if (!x) {}
来源：http://3g.bbcook.cn/Article/details/gwklevuat.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fktsv.cn/Article/details/gqqhyyhfe.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.fktsv.cn/Article/details/glfxehofd.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.yfazqb.com/Article/details/gbdbizlus.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.vehdjk.com/Article/details/gklesgejr.sHtML

[A17] 位运算
来源：http://blog.fktsv.cn/Article/details/gcbhscfac.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/guizqqchw.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.tarul.cn/Article/details/gxdjkxosk.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.tarul.cn/Article/details/glqllrtsx.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.bbcook.cn/Article/details/gngbzdgwt.sHtML


<!-- 参考信息 -->