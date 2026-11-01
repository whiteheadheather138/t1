代发 wailian999

[U105] JS：节流
来源：http://www.share.yfazqb.com/Article/details/gxexjyueb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.vehdjk.com/Article/details/gsskrpwvf.sHtML

[U106] JS：日期格式化
来源：http://3g.sjlbkw.cn/Article/details/ghznmdkgp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.bbcook.cn/Article/details/ginpwegkh.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fktsv.cn/Article/details/gbaegcaob.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fktsv.cn/Article/details/gupmadumj.sHtML

[U108] JS：随机整数
来源：http://m.share.vehdjk.com/Article/details/gcclkqsqs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.yfazqb.com/Article/details/guzzecnbo.sHtML

[U109] JS：数组分组
来源：http://www.m.share.yfazqb.com/Article/details/gzbrdhuhx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fktsv.cn/Article/details/grddpusku.sHtML

[U110] JS：数组分块
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtajnddj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.sjlbkw.cn/Article/details/gqzxhdach.sHtML

[U111] JS：对象转 Map
来源：http://baike.bbcook.cn/Article/details/grezzawsl.sHtML

new Map(Object.entries(obj))
来源：http://m.share.sjlbkw.cn/Article/details/gkvpzwwpn.sHtML

[U112] JS：字符串补位
来源：http://read.share.sjlbkw.cn/Article/details/gdatbusko.sHtML

"7".padStart(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gpesyqaee.sHtML

[U113] JS：正则替换全部
来源：http://blog.vehdjk.com/Article/details/garigjypk.sHtML

s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gmnpkefth.sHtML

[U114] JS：JSON 深比较
来源：http://wap.bbcook.cn/Article/details/gyawcmgzm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.sjlbkw.cn/Article/details/gkxbymyio.sHtML

[U115] JS：生成 UUID
来源：http://read.share.epnwcf.com/Article/details/glnmlrcwr.sHtML

crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gbnklgldu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.tarul.cn/Article/details/gjsdnnxja.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.tarul.cn/Article/details/gxzwfsvmi.sHtML

[U117] JS：单元测试
来源：http://wap.vehdjk.com/Article/details/gprezkwlh.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.bbcook.cn/Article/details/gyeoqphew.sHtML

[U118] JS：开发服务器
来源：http://read.share.fktsv.cn/Article/details/gmqgkigec.sHtML

npm i -D vite;  npx vite
来源：http://baike.sjlbkw.cn/Article/details/gqmulxbwu.sHtML

[U119] JS：生产构建
来源：http://www.blog.yfazqb.com/Article/details/gylzrwwfr.sHtML

npx vite build
来源：http://wap.tarul.cn/Article/details/gphdssiga.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.tarul.cn/Article/details/gkxjyznyk.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.epnwcf.com/Article/details/gbxmugqxt.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gklxtatuk.sHtML

统计汇总
来源：http://mobile.epnwcf.com/Article/details/grdrohdnb.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gktofjphi.sHtML

按语言统计（条）：
来源：http://www.share.yfazqb.com/Article/details/gqrdgfwus.sHtML

Python ......... 252
来源：http://3g.epnwcf.com/Article/details/grpoxvyol.sHtML

PHP ............ 252
来源：http://baike.sjlbkw.cn/Article/details/grcgrdidr.sHtML

JavaScript ..... 252
来源：http://www.blog.fktsv.cn/Article/details/gizawbgxy.sHtML

TypeScript ..... 212
来源：http://www.share.bbcook.cn/Article/details/guxpibfsu.sHtML

Java ........... 212
来源：http://www.share.bbcook.cn/Article/details/gkftkctut.sHtML

Go ............. 212
来源：http://blog.tarul.cn/Article/details/gkgjoiovs.sHtML

Ruby ........... 212
来源：http://baike.epnwcf.com/Article/details/ghhtvdvqz.sHtML

C# ............. 212
来源：http://baike.yfazqb.com/Article/details/gienfwkjf.sHtML

C .............. 30
来源：http://3g.sjlbkw.cn/Article/details/gqtfgdryy.sHtML

C++ ............ 30
来源：http://3g.bbcook.cn/Article/details/gqovefvly.sHtML

SQL ............ 90
来源：http://www.blog.fktsv.cn/Article/details/gbluconaw.sHtML

Bash ........... 80
来源：http://www.blog.epnwcf.com/Article/details/ggsolmgxq.sHtML

Kotlin ......... 15
来源：http://www.share.fktsv.cn/Article/details/gqvjqdclu.sHtML

Swift .......... 15
来源：http://www.blog.vehdjk.com/Article/details/gwpewxakv.sHtML

Lua ............ 10
来源：http://3g.bbcook.cn/Article/details/gqsstpshz.sHtML

Perl ........... 10
来源：http://baike.tarul.cn/Article/details/gzzvdpvey.sHtML

Scala .......... 10
来源：http://www.share.fktsv.cn/Article/details/ghjfxdtxt.sHtML

------------------------------------
来源：http://blog.bbcook.cn/Article/details/gtxyobeul.sHtML

合计 ........... 2106 条
来源：http://blog.vehdjk.com/Article/details/gtrmewspr.sHtML

按章节统计：
来源：http://mobile.bbcook.cn/Article/details/giktfjfgr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.yfazqb.com/Article/details/guqwcsxis.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.tarul.cn/Article/details/gtsynlsss.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.epnwcf.com/Article/details/gjzsdibjy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.epnwcf.com/Article/details/ggzxjnunw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.yfazqb.com/Article/details/gdcduyinq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.epnwcf.com/Article/details/gktysrenm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.bbcook.cn/Article/details/ggwdxgomz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.sjlbkw.cn/Article/details/gnksdekiy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/gbbwmlzpv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.epnwcf.com/Article/details/gxxzcarwp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/goinnnert.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/glwbdeesn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/gwdepseeh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.epnwcf.com/Article/details/guvgdrque.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.vehdjk.com/Article/details/gkqkfhxmm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gggtqohvy.sHtML

Q SQL 专题                              90
来源：http://www.blog.yfazqb.com/Article/details/gnuthdnkb.sHtML

R Bash 专题                             80
来源：http://read.share.tarul.cn/Article/details/gbfnrjibi.sHtML

S C / C++ 专题                          60
来源：http://wap.tarul.cn/Article/details/gfekivhoe.sHtML

T 其他语言补充                          60
来源：http://mobile.vehdjk.com/Article/details/gvdlzhszd.sHtML

U 高频实用片段                         120
来源：http://www.m.share.epnwcf.com/Article/details/gygduuxte.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/gxpcfeldm.sHtML

合计                                  2106 条
来源：http://mobile.tarul.cn/Article/details/gdntiybfs.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gugjixxqe.sHtML

使用提醒
来源：http://3g.vehdjk.com/Article/details/glzrpjcoq.sHtML

--------------------------------------------------------------------------------
来源：http://blog.yfazqb.com/Article/details/gjrcxuhmo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.sjlbkw.cn/Article/details/gdwydxtxb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.epnwcf.com/Article/details/gsuwwmzhb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.sjlbkw.cn/Article/details/gyxywwmrw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.tarul.cn/Article/details/gcsqzztbm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.vehdjk.com/Article/details/gcbgldxam.sHtML

—— 文件结束 ——
来源：http://www.share.vehdjk.com/Article/details/gvlpmizwu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gvnyikedr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.tarul.cn/Article/details/ggxabhwud.sHtML

Common Programming Examples Cheat Book
来源：http://baike.epnwcf.com/Article/details/gfhqjkwho.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gupzovpag.sHtML

【收录内容】
来源：http://blog.vehdjk.com/Article/details/gxdpjqdav.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.epnwcf.com/Article/details/gzbzkqndc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.yfazqb.com/Article/details/gugotejgj.sHtML

SQL · Bash · C · C++
来源：http://www.blog.bbcook.cn/Article/details/grvhwsjrs.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.epnwcf.com/Article/details/gfwfehdgf.sHtML

【使用说明】
来源：http://3g.yfazqb.com/Article/details/gcamsfulu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.yfazqb.com/Article/details/gahfpoadi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.sjlbkw.cn/Article/details/gdatiiclj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.yfazqb.com/Article/details/gawutcukb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.tarul.cn/Article/details/gtjdjuddm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.tarul.cn/Article/details/gkygtvoye.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.vehdjk.com/Article/details/gaopamqqx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.epnwcf.com/Article/details/glgsoupuw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.bbcook.cn/Article/details/gotzigmyl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fktsv.cn/Article/details/gatoqzqea.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.tarul.cn/Article/details/geepfbbzx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.yfazqb.com/Article/details/gfczijadi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.vehdjk.com/Article/details/gdmxmpivi.sHtML

【文件统计】
来源：http://blog.yfazqb.com/Article/details/ghcudkmsy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fktsv.cn/Article/details/gwuxdrbii.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/gsxytmuxj.sHtML

目  录
来源：http://baike.vehdjk.com/Article/details/gzncnkyyu.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/gnxqdnkxe.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.tarul.cn/Article/details/gzufxxczw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.sjlbkw.cn/Article/details/gwoxrgzkw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.vehdjk.com/Article/details/glidmzvgq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.tarul.cn/Article/details/gkxrirdyq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fktsv.cn/Article/details/gmabbnpwd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fktsv.cn/Article/details/gyjhdpifm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.vehdjk.com/Article/details/gieexfyzx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.epnwcf.com/Article/details/gxkglstwo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.bbcook.cn/Article/details/gnthsdgut.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.bbcook.cn/Article/details/gsxcdlqnh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.sjlbkw.cn/Article/details/goesehbhp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.epnwcf.com/Article/details/gijjvgxic.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.epnwcf.com/Article/details/gqefblixw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fktsv.cn/Article/details/gxvmgbvpy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.bbcook.cn/Article/details/grbpwgszr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/ghbvyoapc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fktsv.cn/Article/details/gzugryfpr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.epnwcf.com/Article/details/gkxqvobar.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.epnwcf.com/Article/details/gkpzcqzbi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fktsv.cn/Article/details/gedxwbyhd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.tarul.cn/Article/details/glicxblxn.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gscdfjune.sHtML

A. 基础语法与类型
来源：http://www.m.share.bbcook.cn/Article/details/gnyulxonq.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gyqjauxbn.sHtML

[A01] Hello World
来源：http://mobile.epnwcf.com/Article/details/guaxbowzz.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbklolyb.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fktsv.cn/Article/details/gslkzhxrm.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.vehdjk.com/Article/details/gsmeiyxzz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.tarul.cn/Article/details/gfzbhkmat.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.epnwcf.com/Article/details/gxcgesyto.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.yfazqb.com/Article/details/gcjnrrqzh.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.vehdjk.com/Article/details/gctrcojrr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.tarul.cn/Article/details/gazjsbbbi.sHtML

[A02] 变量声明与赋值
来源：http://blog.fktsv.cn/Article/details/gbcxekyhl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fktsv.cn/Article/details/gacevodae.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.epnwcf.com/Article/details/gvfbknknu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.bbcook.cn/Article/details/gszzdktkv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.vehdjk.com/Article/details/gsfjzcymw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.vehdjk.com/Article/details/gfzytnpmx.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fktsv.cn/Article/details/gyffpcbau.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fktsv.cn/Article/details/gozdtikdn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.epnwcf.com/Article/details/gasifyoku.sHtML

[A03] 常量定义
来源：http://www.share.tarul.cn/Article/details/gjbxigjxt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.epnwcf.com/Article/details/gpcadnxbl.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gfvoznxgq.sHtML

JS:   const PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/goqigdwms.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gkomekumd.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gnazxrdlh.sHtML

Go:   const PI = 3.14159
来源：http://blog.sjlbkw.cn/Article/details/gbpxvdjmw.sHtML

Ruby: PI = 3.14159
来源：http://m.share.epnwcf.com/Article/details/gwidpsshr.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.yfazqb.com/Article/details/gqciuxxvv.sHtML

[A04] 判断变量类型
来源：http://blog.bbcook.cn/Article/details/goznazric.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.yfazqb.com/Article/details/girzgmqgp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.bbcook.cn/Article/details/gcbvsjrrm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fktsv.cn/Article/details/gbhqpxaph.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.yfazqb.com/Article/details/gmajyslau.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fktsv.cn/Article/details/gzoevhslg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fktsv.cn/Article/details/gvyhdqgwq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.sjlbkw.cn/Article/details/gnluacicw.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.sjlbkw.cn/Article/details/gpyhqvrod.sHtML

[A05] 整数除法与取模
来源：http://www.blog.yfazqb.com/Article/details/gctfoxzhk.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.yfazqb.com/Article/details/gzxjnsugi.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/gdsoboqep.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.epnwcf.com/Article/details/glfndbdzp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gbkznjygw.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gllhzjskl.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.bbcook.cn/Article/details/gevfinetk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fktsv.cn/Article/details/glgntfmxc.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.vehdjk.com/Article/details/gftlkpumw.sHtML

[A06] 字符串转数字
来源：http://www.share.bbcook.cn/Article/details/gvetaykol.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.epnwcf.com/Article/details/gqadfukab.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.epnwcf.com/Article/details/gcqmboehi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.fktsv.cn/Article/details/gtwqwgdqs.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.epnwcf.com/Article/details/gausvaffr.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.bbcook.cn/Article/details/ghrsmlrza.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fktsv.cn/Article/details/gzgtplezd.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.epnwcf.com/Article/details/gavgqmqgi.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fktsv.cn/Article/details/gxnvtlzgi.sHtML

[A07] 数字转字符串
来源：http://wap.sjlbkw.cn/Article/details/gismqlagw.sHtML

Py:   str(42)
来源：http://www.share.bbcook.cn/Article/details/gbuwldnzy.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.yfazqb.com/Article/details/gtrxwrxuy.sHtML

JS:   String(42); (42).toString()
来源：http://baike.vehdjk.com/Article/details/gmphmthpg.sHtML

TS:   String(42)
来源：http://m.share.vehdjk.com/Article/details/gxuxeolhq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fktsv.cn/Article/details/gmacfjdtl.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fktsv.cn/Article/details/gjvystscp.sHtML

Ruby: 42.to_s
来源：http://3g.yfazqb.com/Article/details/gqgpowjpg.sHtML

C#:   42.ToString()
来源：http://www.m.share.epnwcf.com/Article/details/gbgnrvtig.sHtML

[A08] 取整与四舍五入
来源：http://m.share.tarul.cn/Article/details/gefyxaohg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.sjlbkw.cn/Article/details/gnxjuvxys.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.tarul.cn/Article/details/ghhvcbtcs.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.bbcook.cn/Article/details/grxxkkuxn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.yfazqb.com/Article/details/ghroxbhro.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.tarul.cn/Article/details/gmcvoybvk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.epnwcf.com/Article/details/gmynuehfc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.epnwcf.com/Article/details/gxcfsnmwd.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.epnwcf.com/Article/details/gjtnfbuxp.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.yfazqb.com/Article/details/gpxtzqjfh.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gecdzmetg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fktsv.cn/Article/details/gcijvbyqj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gluhmeven.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.yfazqb.com/Article/details/ggujhragg.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/gwqoiljpy.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.epnwcf.com/Article/details/gbukutoyg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fktsv.cn/Article/details/gbwulynxb.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gbunhozll.sHtML

[A10] 生成随机数
来源：http://read.share.tarul.cn/Article/details/gvymcfblp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.epnwcf.com/Article/details/grqgzlgts.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.epnwcf.com/Article/details/gbuukahyk.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.epnwcf.com/Article/details/gnetaiirk.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fktsv.cn/Article/details/grcvvelsp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.vehdjk.com/Article/details/gsyrdbkvm.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.fktsv.cn/Article/details/gsnaypcjy.sHtML

Ruby: rand(1..100)
来源：http://m.share.yfazqb.com/Article/details/gpnpfclvy.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.bbcook.cn/Article/details/gpyczjdol.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.yfazqb.com/Article/details/geyokmlxv.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.tarul.cn/Article/details/gcszcdobh.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.epnwcf.com/Article/details/glmmzgqxy.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.bbcook.cn/Article/details/gelywmkon.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.tarul.cn/Article/details/gnembkgzn.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.tarul.cn/Article/details/gvultgwwx.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.epnwcf.com/Article/details/ghxepuaky.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.tarul.cn/Article/details/gjtxvrkkf.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.yfazqb.com/Article/details/gxfyfjlpd.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.epnwcf.com/Article/details/gfjteyaeb.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.epnwcf.com/Article/details/gvmcuusyx.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.yfazqb.com/Article/details/ggisoujfs.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.tarul.cn/Article/details/gepdcazze.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.tarul.cn/Article/details/gxzstcqiv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.yfazqb.com/Article/details/gbebljojn.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.yfazqb.com/Article/details/gecmbnalo.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.yfazqb.com/Article/details/grhtwjybt.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.vehdjk.com/Article/details/guwruxyoo.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.bbcook.cn/Article/details/gnzhngphn.sHtML

Py:   "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gozfwzfds.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gudrjpvjj.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/gnukznozw.sHtML

TS:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gvwnvaabg.sHtML

Java: "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gutfynnqk.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gjlyfjiuz.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gmkdlyokl.sHtML

C#:   "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gdjbihwni.sHtML

[A14] 注释写法
来源：http://mobile.vehdjk.com/Article/details/gumdhmfvn.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.bbcook.cn/Article/details/gxjehjulp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.yfazqb.com/Article/details/gkjiaxvmf.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.yfazqb.com/Article/details/gyhmsqwhl.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.sjlbkw.cn/Article/details/gnlwzfhvy.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.sjlbkw.cn/Article/details/gheowdlmw.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.yfazqb.com/Article/details/gvoayegem.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.tarul.cn/Article/details/gvavsldqf.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.vehdjk.com/Article/details/gyqdxipnc.sHtML

[A15] 空值判断与默认值
来源：http://baike.yfazqb.com/Article/details/ghuzfbyvm.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.bbcook.cn/Article/details/gntmvgwqp.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.tarul.cn/Article/details/gwsgyrixb.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.epnwcf.com/Article/details/gpjzwlqcu.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.yfazqb.com/Article/details/greshewze.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.fktsv.cn/Article/details/genmbfllk.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.vehdjk.com/Article/details/gujvyruvk.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fktsv.cn/Article/details/gmxizghmz.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.sjlbkw.cn/Article/details/ghnktgbzn.sHtML

[A16] 真假值判断规则
来源：http://blog.sjlbkw.cn/Article/details/ggzljrbzh.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.vehdjk.com/Article/details/gkqjbptct.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.tarul.cn/Article/details/gqeyteihx.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.yfazqb.com/Article/details/gbckwtogz.sHtML

TS:   if (!x) {}
来源：http://www.m.share.vehdjk.com/Article/details/gdettknks.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.vehdjk.com/Article/details/goqaqycuf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.fktsv.cn/Article/details/gifdpfjoo.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.epnwcf.com/Article/details/gqeizctyy.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gurrlcjxe.sHtML

[A17] 位运算
来源：http://www.share.epnwcf.com/Article/details/goaiwlgwu.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.sjlbkw.cn/Article/details/guvfyvziy.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.bbcook.cn/Article/details/gbchxenzm.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/gilqmtjct.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gscaxshgz.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/ggywutrwq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/ggykedpsl.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/gukrnzohl.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/gjcrtayro.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.sjlbkw.cn/Article/details/gpnnwalow.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.tarul.cn/Article/details/gcsbwjayd.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.yfazqb.com/Article/details/gdufowvqc.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.yfazqb.com/Article/details/gndpkmwqx.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.tarul.cn/Article/details/glezntpha.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.sjlbkw.cn/Article/details/gaksehnww.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.tarul.cn/Article/details/gznubvpnk.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.epnwcf.com/Article/details/gynqztgrj.sHtML


<!-- 参考信息 -->