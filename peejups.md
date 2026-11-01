代发 wailian999

[U101] JS：classList 操作
来源：http://mobile.tarul.cn/Article/details/gvdziuufj.sHtML

el.classList.toggle("active")
来源：http://www.share.vehdjk.com/Article/details/gsbtimkyq.sHtML

[U102] JS：本地存储
来源：http://baike.vehdjk.com/Article/details/gfjaitdzf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.sjlbkw.cn/Article/details/gqwzgxdpp.sHtML

[U103] JS：定时器
来源：http://www.blog.tarul.cn/Article/details/grvbbartl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fktsv.cn/Article/details/gehzdqgkv.sHtML

[U104] JS：防抖
来源：http://m.share.bbcook.cn/Article/details/gpcdmveud.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gnhpapkmi.sHtML

[U105] JS：节流
来源：http://www.blog.vehdjk.com/Article/details/gxajewiqu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.vehdjk.com/Article/details/goaobjaeg.sHtML

[U106] JS：日期格式化
来源：http://www.share.vehdjk.com/Article/details/gufbwzzxi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.vehdjk.com/Article/details/gkqfoktrs.sHtML

[U107] JS：数字千分位
来源：http://3g.epnwcf.com/Article/details/gkarjaatl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.vehdjk.com/Article/details/gvgyidxws.sHtML

[U108] JS：随机整数
来源：http://blog.vehdjk.com/Article/details/glchrxmhs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.bbcook.cn/Article/details/gnynlzrxb.sHtML

[U109] JS：数组分组
来源：http://read.share.vehdjk.com/Article/details/gjpwedjgg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.epnwcf.com/Article/details/gawpjrozd.sHtML

[U110] JS：数组分块
来源：http://www.m.share.yfazqb.com/Article/details/gzzsdiorh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.epnwcf.com/Article/details/gjjgzcnhb.sHtML

[U111] JS：对象转 Map
来源：http://baike.bbcook.cn/Article/details/gmclcbipz.sHtML

new Map(Object.entries(obj))
来源：http://3g.bbcook.cn/Article/details/gnspvcxlv.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.vehdjk.com/Article/details/gxybmceoe.sHtML

"7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gsoqnxmeq.sHtML

[U113] JS：正则替换全部
来源：http://baike.sjlbkw.cn/Article/details/gwvqfqakb.sHtML

s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gatotfjyv.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fktsv.cn/Article/details/gairayjma.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.vehdjk.com/Article/details/gctynaoai.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gctbblfqe.sHtML

crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gdlsylukp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.bbcook.cn/Article/details/grfhixnbr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.sjlbkw.cn/Article/details/gidvffeln.sHtML

[U117] JS：单元测试
来源：http://read.share.epnwcf.com/Article/details/grrgwqmds.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.bbcook.cn/Article/details/gfyxcabgb.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.epnwcf.com/Article/details/godkwcrpp.sHtML

npm i -D vite;  npx vite
来源：http://baike.vehdjk.com/Article/details/grzqlggrm.sHtML

[U119] JS：生产构建
来源：http://read.share.fktsv.cn/Article/details/gejiaveeb.sHtML

npx vite build
来源：http://m.share.fktsv.cn/Article/details/grxndivax.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.vehdjk.com/Article/details/gszoijooo.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.sjlbkw.cn/Article/details/gwsnbbmgb.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gfrwiwwov.sHtML

统计汇总
来源：http://www.blog.fktsv.cn/Article/details/gmuftdbvl.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gfeqvpfgl.sHtML

按语言统计（条）：
来源：http://wap.yfazqb.com/Article/details/glommoamb.sHtML

Python ......... 252
来源：http://blog.fktsv.cn/Article/details/gzdteqbii.sHtML

PHP ............ 252
来源：http://blog.vehdjk.com/Article/details/gvnvfgelr.sHtML

JavaScript ..... 252
来源：http://www.blog.epnwcf.com/Article/details/gnbxymmcr.sHtML

TypeScript ..... 212
来源：http://mobile.epnwcf.com/Article/details/gpbtmzxix.sHtML

Java ........... 212
来源：http://3g.bbcook.cn/Article/details/gnctdlnzn.sHtML

Go ............. 212
来源：http://read.share.tarul.cn/Article/details/gprcgnets.sHtML

Ruby ........... 212
来源：http://www.blog.epnwcf.com/Article/details/gbzalfylo.sHtML

C# ............. 212
来源：http://www.share.fktsv.cn/Article/details/gsfkzheuo.sHtML

C .............. 30
来源：http://3g.yfazqb.com/Article/details/gzmnfkwrm.sHtML

C++ ............ 30
来源：http://www.blog.bbcook.cn/Article/details/glmbnlaio.sHtML

SQL ............ 90
来源：http://baike.bbcook.cn/Article/details/gjgeesgfd.sHtML

Bash ........... 80
来源：http://blog.sjlbkw.cn/Article/details/gffhcfhmz.sHtML

Kotlin ......... 15
来源：http://baike.fktsv.cn/Article/details/gvqrvordl.sHtML

Swift .......... 15
来源：http://3g.epnwcf.com/Article/details/gphokljwe.sHtML

Lua ............ 10
来源：http://mobile.yfazqb.com/Article/details/gdkanwyuc.sHtML

Perl ........... 10
来源：http://wap.fktsv.cn/Article/details/gjxbgmzqx.sHtML

Scala .......... 10
来源：http://baike.bbcook.cn/Article/details/gbrjnksgr.sHtML

------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gjohjixhf.sHtML

合计 ........... 2106 条
来源：http://read.share.bbcook.cn/Article/details/gqveystzf.sHtML

按章节统计：
来源：http://3g.yfazqb.com/Article/details/glxooiqni.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fktsv.cn/Article/details/giiwctqvs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.bbcook.cn/Article/details/gsyodxfkq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/gahtfspiw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.bbcook.cn/Article/details/geeunvmry.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.epnwcf.com/Article/details/govsccnqz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fktsv.cn/Article/details/goqtjbhlc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.bbcook.cn/Article/details/gkfojhzdi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.yfazqb.com/Article/details/gdfmvdmbh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/grzuzockz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.bbcook.cn/Article/details/gciuuhdgh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/gqglwmivx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.tarul.cn/Article/details/gtrrlozeq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gemftpcid.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.vehdjk.com/Article/details/gfncetiyt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.bbcook.cn/Article/details/ganvviioq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gzjxxlgjs.sHtML

Q SQL 专题                              90
来源：http://baike.yfazqb.com/Article/details/gegeehifz.sHtML

R Bash 专题                             80
来源：http://3g.yfazqb.com/Article/details/gdjvvwssc.sHtML

S C / C++ 专题                          60
来源：http://mobile.tarul.cn/Article/details/gkjscdear.sHtML

T 其他语言补充                          60
来源：http://m.share.epnwcf.com/Article/details/gengsmxps.sHtML

U 高频实用片段                         120
来源：http://www.share.bbcook.cn/Article/details/glybmdsnj.sHtML

------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gmdhbbxrp.sHtML

合计                                  2106 条
来源：http://3g.bbcook.cn/Article/details/ggxvrwlxa.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/gqbjdkyhk.sHtML

使用提醒
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvezqrxr.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gksuqrnhn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.tarul.cn/Article/details/givuzvuxr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.tarul.cn/Article/details/gqurezqzu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.sjlbkw.cn/Article/details/guzoefrid.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.sjlbkw.cn/Article/details/gbibrhkgx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.bbcook.cn/Article/details/gcdfxwkpi.sHtML

—— 文件结束 ——
来源：http://mobile.fktsv.cn/Article/details/gzcgyebms.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gdixxqttl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.sjlbkw.cn/Article/details/gainoltwa.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.sjlbkw.cn/Article/details/gmjvmlppt.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gwdgefaei.sHtML

【收录内容】
来源：http://read.share.bbcook.cn/Article/details/gbypwbqxs.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.sjlbkw.cn/Article/details/gguuniawq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.tarul.cn/Article/details/gfjgskfnj.sHtML

SQL · Bash · C · C++
来源：http://blog.vehdjk.com/Article/details/ggnycayqi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.vehdjk.com/Article/details/gtqxabosv.sHtML

【使用说明】
来源：http://www.share.tarul.cn/Article/details/ggmiwdygo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fktsv.cn/Article/details/gejhnakgz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.bbcook.cn/Article/details/gtftpveby.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.bbcook.cn/Article/details/gpyfeyxjv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fktsv.cn/Article/details/gisrvfaad.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.sjlbkw.cn/Article/details/goxhflupf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.bbcook.cn/Article/details/guiqrptfv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.vehdjk.com/Article/details/gizexrhal.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.sjlbkw.cn/Article/details/glgstublc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.vehdjk.com/Article/details/grulkpypp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.sjlbkw.cn/Article/details/gbuuezhqr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.tarul.cn/Article/details/gumkizeum.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.yfazqb.com/Article/details/gtevumlpa.sHtML

【文件统计】
来源：http://www.blog.vehdjk.com/Article/details/ggsgpofel.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.bbcook.cn/Article/details/gxwtvorak.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gpzppytxo.sHtML

目  录
来源：http://baike.vehdjk.com/Article/details/gsbrtlazy.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gpvqkiiuh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fktsv.cn/Article/details/gjncunlkz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.bbcook.cn/Article/details/gylmdwofk.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.yfazqb.com/Article/details/gerlnfktr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.epnwcf.com/Article/details/glgdvwnrn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.epnwcf.com/Article/details/gpxbubrln.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.tarul.cn/Article/details/gydkapcyx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.sjlbkw.cn/Article/details/ghpevzixf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.yfazqb.com/Article/details/gxeqgqvbd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/greisraqm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.yfazqb.com/Article/details/gfebrtcqc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/gqmfgyvfk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fktsv.cn/Article/details/gvcgoyvph.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/ggbzyuzqz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.yfazqb.com/Article/details/glujdgxqf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.yfazqb.com/Article/details/gdztwhlco.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/grbwxzmic.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.sjlbkw.cn/Article/details/gdipfegyj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.epnwcf.com/Article/details/gkortderz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.vehdjk.com/Article/details/ghoserqcb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.tarul.cn/Article/details/gknfyirup.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.tarul.cn/Article/details/gsrjkzpvk.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ghfswwwju.sHtML

A. 基础语法与类型
来源：http://www.share.fktsv.cn/Article/details/gguhmgluu.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gacniypqz.sHtML

[A01] Hello World
来源：http://blog.fktsv.cn/Article/details/gxxfgcbdw.sHtML

Py:   print("Hello, World!")
来源：http://blog.yfazqb.com/Article/details/gzycyzbti.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.tarul.cn/Article/details/grsimnwvw.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.tarul.cn/Article/details/gulcgwlsp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.yfazqb.com/Article/details/gskfdsujh.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.tarul.cn/Article/details/gknvtckro.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.yfazqb.com/Article/details/gznxyjxlk.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.epnwcf.com/Article/details/gcdtfkbqu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.yfazqb.com/Article/details/guualowqu.sHtML

[A02] 变量声明与赋值
来源：http://www.share.vehdjk.com/Article/details/gdtsutjlg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.vehdjk.com/Article/details/gmprzwpms.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.yfazqb.com/Article/details/genxqarqs.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.yfazqb.com/Article/details/ggswlqnox.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.sjlbkw.cn/Article/details/gvpzhnekb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fktsv.cn/Article/details/glhbflmpf.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fktsv.cn/Article/details/geeguvxdu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.vehdjk.com/Article/details/gvxxncclv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.epnwcf.com/Article/details/grpekddyx.sHtML

[A03] 常量定义
来源：http://blog.fktsv.cn/Article/details/gyqzithzb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.vehdjk.com/Article/details/gbbabajfq.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/goppfkckh.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/ghkcczeqx.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gkuxuicef.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gimknrwtj.sHtML

Go:   const PI = 3.14159
来源：http://read.share.bbcook.cn/Article/details/goeztmqeb.sHtML

Ruby: PI = 3.14159
来源：http://m.share.bbcook.cn/Article/details/ghukhimri.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gqhnecbex.sHtML

[A04] 判断变量类型
来源：http://wap.fktsv.cn/Article/details/gkizpmper.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.yfazqb.com/Article/details/gytldsjca.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.bbcook.cn/Article/details/gejmvceqj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fktsv.cn/Article/details/gljzksrgn.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.vehdjk.com/Article/details/gplbnlfuq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.bbcook.cn/Article/details/gogzjiwih.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.bbcook.cn/Article/details/gzjfqppcv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.bbcook.cn/Article/details/grvjbvmli.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fktsv.cn/Article/details/gqorfmqet.sHtML

[A05] 整数除法与取模
来源：http://blog.fktsv.cn/Article/details/giswsyoka.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.vehdjk.com/Article/details/grtcbfqjk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fktsv.cn/Article/details/gtqlbrlep.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.bbcook.cn/Article/details/gbessgrjf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.yfazqb.com/Article/details/grpujtoor.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.tarul.cn/Article/details/graeynxkp.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.vehdjk.com/Article/details/gmubmoeyv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/guttzmycf.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fktsv.cn/Article/details/gueqngvug.sHtML

[A06] 字符串转数字
来源：http://www.share.bbcook.cn/Article/details/gczshbaqy.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.sjlbkw.cn/Article/details/gjxjuyles.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.sjlbkw.cn/Article/details/gdbrwiglq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.vehdjk.com/Article/details/geoqdiusw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.sjlbkw.cn/Article/details/gshabfndg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.vehdjk.com/Article/details/gzoqvuvgv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.vehdjk.com/Article/details/giuvutbwr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.epnwcf.com/Article/details/gqlyzbdwe.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.epnwcf.com/Article/details/gqukbuanz.sHtML

[A07] 数字转字符串
来源：http://m.share.epnwcf.com/Article/details/geeptpbub.sHtML

Py:   str(42)
来源：http://wap.tarul.cn/Article/details/geaekmrzp.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.bbcook.cn/Article/details/gorxooohw.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fktsv.cn/Article/details/gepvdmryy.sHtML

TS:   String(42)
来源：http://mobile.yfazqb.com/Article/details/ggzeggqlk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fktsv.cn/Article/details/gcdjglbji.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.tarul.cn/Article/details/gieqwuiet.sHtML

Ruby: 42.to_s
来源：http://baike.sjlbkw.cn/Article/details/gtxkobplp.sHtML

C#:   42.ToString()
来源：http://mobile.bbcook.cn/Article/details/gmtffgijc.sHtML

[A08] 取整与四舍五入
来源：http://read.share.vehdjk.com/Article/details/gncsjahpg.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.vehdjk.com/Article/details/ghhzeoily.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.vehdjk.com/Article/details/glhpsctze.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.bbcook.cn/Article/details/gniicoiak.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fktsv.cn/Article/details/gxwmlrypt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.bbcook.cn/Article/details/ghgitbfzz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.fktsv.cn/Article/details/guytouoms.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.sjlbkw.cn/Article/details/ghuzscrpv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fktsv.cn/Article/details/gejjuhldl.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.sjlbkw.cn/Article/details/gzgvmqbta.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.tarul.cn/Article/details/gffinzpoc.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gudmhekpe.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gjbriyrbe.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.tarul.cn/Article/details/gwgyygmhp.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/ggpvapisa.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fktsv.cn/Article/details/gkbumtsjr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.tarul.cn/Article/details/gsjbxrhyr.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gakwajipe.sHtML

[A10] 生成随机数
来源：http://baike.fktsv.cn/Article/details/gykgeixzm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.tarul.cn/Article/details/gxfnyonte.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.yfazqb.com/Article/details/ghwgwfwvy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fktsv.cn/Article/details/gwlnwxzrx.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.vehdjk.com/Article/details/ghrszriui.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.sjlbkw.cn/Article/details/gnjijzccw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.tarul.cn/Article/details/ghkzqiclq.sHtML

Ruby: rand(1..100)
来源：http://m.share.yfazqb.com/Article/details/gqehggdcu.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.vehdjk.com/Article/details/gaoydgwnl.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.epnwcf.com/Article/details/gvwyxqyrw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.epnwcf.com/Article/details/gcwtmkube.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.bbcook.cn/Article/details/gtlcnhkou.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.vehdjk.com/Article/details/gxdfvimmx.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.epnwcf.com/Article/details/gblcaastp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.vehdjk.com/Article/details/gerktgmdl.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.tarul.cn/Article/details/gzhthlzcg.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbbfjxhh.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.sjlbkw.cn/Article/details/glsiypuxv.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.bbcook.cn/Article/details/gtwcitrkg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.bbcook.cn/Article/details/gtkzocatz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.sjlbkw.cn/Article/details/gxkirejbg.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.vehdjk.com/Article/details/gzucrmmqm.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.tarul.cn/Article/details/gjrwfwpks.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.tarul.cn/Article/details/gcelulhfe.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.epnwcf.com/Article/details/gdnaqcfif.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.bbcook.cn/Article/details/gvmfrjkyw.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.epnwcf.com/Article/details/galcarodp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.tarul.cn/Article/details/ggkkmxbon.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/gqujdiwon.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.yfazqb.com/Article/details/gpuggwyhu.sHtML

JS:   "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/gaucsdayj.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/gpwuzumun.sHtML

Java: "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gwuhvopop.sHtML

Go:   "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gvnnnalcq.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/guldalaxu.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/ghbpreolk.sHtML

[A14] 注释写法
来源：http://mobile.tarul.cn/Article/details/gedvyysif.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.epnwcf.com/Article/details/gfwyikdta.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.bbcook.cn/Article/details/gjergbinw.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.vehdjk.com/Article/details/gpeebwvez.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.bbcook.cn/Article/details/gypumluip.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.epnwcf.com/Article/details/gbbosmudj.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.bbcook.cn/Article/details/gxrqjupui.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.vehdjk.com/Article/details/gyemitzfe.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.bbcook.cn/Article/details/gwiflpdgx.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.bbcook.cn/Article/details/ghrmxkmuh.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.yfazqb.com/Article/details/gzfygtkkt.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.bbcook.cn/Article/details/gtqrswrxo.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.vehdjk.com/Article/details/gispvwlbl.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.vehdjk.com/Article/details/gehsfsozt.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.vehdjk.com/Article/details/gygwvdzgj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.epnwcf.com/Article/details/gngrcjhej.sHtML

Ruby: value = data || "默认值"
来源：http://blog.yfazqb.com/Article/details/gyxqeoscq.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.bbcook.cn/Article/details/gbcsmevcu.sHtML

[A16] 真假值判断规则
来源：http://baike.fktsv.cn/Article/details/ghyoyvjtw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.fktsv.cn/Article/details/gveuizlfn.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.yfazqb.com/Article/details/gfddatwms.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fktsv.cn/Article/details/gekvdifnp.sHtML

TS:   if (!x) {}
来源：http://www.share.tarul.cn/Article/details/gzrcqnilm.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.yfazqb.com/Article/details/gxkaguqis.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.bbcook.cn/Article/details/glmenedds.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.bbcook.cn/Article/details/gvzicrqob.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.yfazqb.com/Article/details/gwxjmnyag.sHtML

[A17] 位运算
来源：http://www.m.share.yfazqb.com/Article/details/gbfjejhyh.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gfgqmxsrd.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.vehdjk.com/Article/details/gyrudtuva.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.bbcook.cn/Article/details/gwykwwxly.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.epnwcf.com/Article/details/gyppcjdqf.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/gxnyzhdya.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/gigsddusn.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.vehdjk.com/Article/details/gpdhwfgfc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.sjlbkw.cn/Article/details/gxcnniobo.sHtML


<!-- 参考信息 -->