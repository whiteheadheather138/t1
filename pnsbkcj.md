代发 wailian999

[U101] JS：classList 操作
来源：http://3g.sjlbkw.cn/Article/details/gltunqtgi.sHtML

el.classList.toggle("active")
来源：http://www.share.epnwcf.com/Article/details/gfxdhgaak.sHtML

[U102] JS：本地存储
来源：http://www.blog.fktsv.cn/Article/details/gxsntxdsl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.sjlbkw.cn/Article/details/gtzaqlmdg.sHtML

[U103] JS：定时器
来源：http://www.m.share.vehdjk.com/Article/details/ghoajhswn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.yfazqb.com/Article/details/gazqpball.sHtML

[U104] JS：防抖
来源：http://wap.epnwcf.com/Article/details/gibtskduh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gdlmnlpnj.sHtML

[U105] JS：节流
来源：http://m.share.vehdjk.com/Article/details/gggfmfgoe.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.bbcook.cn/Article/details/glohnhkvx.sHtML

[U106] JS：日期格式化
来源：http://blog.tarul.cn/Article/details/gbizhtzjn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.epnwcf.com/Article/details/gvsipgzja.sHtML

[U107] JS：数字千分位
来源：http://read.share.bbcook.cn/Article/details/gayevhqhb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.vehdjk.com/Article/details/givaqkuhs.sHtML

[U108] JS：随机整数
来源：http://www.m.share.sjlbkw.cn/Article/details/gurnmrbrv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.vehdjk.com/Article/details/gemcuiyly.sHtML

[U109] JS：数组分组
来源：http://read.share.vehdjk.com/Article/details/gedjzicwv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.vehdjk.com/Article/details/gemyrbfmz.sHtML

[U110] JS：数组分块
来源：http://m.share.epnwcf.com/Article/details/gdyuwivdg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.vehdjk.com/Article/details/gdermdhtg.sHtML

[U111] JS：对象转 Map
来源：http://wap.yfazqb.com/Article/details/ghcmugguj.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.sjlbkw.cn/Article/details/gidkwzcoo.sHtML

[U112] JS：字符串补位
来源：http://www.blog.vehdjk.com/Article/details/gnawuomhj.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/giynsquwd.sHtML

[U113] JS：正则替换全部
来源：http://m.share.vehdjk.com/Article/details/gkaubfyhu.sHtML

s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gkdixvxig.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.bbcook.cn/Article/details/gwcfexvid.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.sjlbkw.cn/Article/details/glfbgdiay.sHtML

[U115] JS：生成 UUID
来源：http://m.share.yfazqb.com/Article/details/ghwxldzbw.sHtML

crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/ggbdrefhj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.vehdjk.com/Article/details/gaaxadxar.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.yfazqb.com/Article/details/gwzbfuuge.sHtML

[U117] JS：单元测试
来源：http://www.blog.vehdjk.com/Article/details/glkdcfgxi.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.tarul.cn/Article/details/gnrbptwmz.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.sjlbkw.cn/Article/details/geoyrrbzt.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.sjlbkw.cn/Article/details/gndtfisvw.sHtML

[U119] JS：生产构建
来源：http://read.share.fktsv.cn/Article/details/gizekvhyq.sHtML

npx vite build
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbvtuksd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.yfazqb.com/Article/details/gzzxbsdar.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.epnwcf.com/Article/details/glgtsoddx.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gehklgsyb.sHtML

统计汇总
来源：http://mobile.epnwcf.com/Article/details/gjfglxllx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gsgqijwnv.sHtML

按语言统计（条）：
来源：http://www.blog.tarul.cn/Article/details/gwmhqxnsh.sHtML

Python ......... 252
来源：http://blog.yfazqb.com/Article/details/geljfossk.sHtML

PHP ............ 252
来源：http://www.blog.sjlbkw.cn/Article/details/goarjjisn.sHtML

JavaScript ..... 252
来源：http://3g.fktsv.cn/Article/details/gbzpjzvkb.sHtML

TypeScript ..... 212
来源：http://www.m.share.epnwcf.com/Article/details/gzhsroldn.sHtML

Java ........... 212
来源：http://blog.yfazqb.com/Article/details/gfnovaujv.sHtML

Go ............. 212
来源：http://www.blog.tarul.cn/Article/details/gjbeutemo.sHtML

Ruby ........... 212
来源：http://mobile.sjlbkw.cn/Article/details/gyvdgfeej.sHtML

C# ............. 212
来源：http://baike.yfazqb.com/Article/details/gmiwnskrd.sHtML

C .............. 30
来源：http://www.share.yfazqb.com/Article/details/glqumcavt.sHtML

C++ ............ 30
来源：http://read.share.yfazqb.com/Article/details/gqbtgarob.sHtML

SQL ............ 90
来源：http://www.m.share.sjlbkw.cn/Article/details/glcqbtkkv.sHtML

Bash ........... 80
来源：http://wap.bbcook.cn/Article/details/gpdqiwvda.sHtML

Kotlin ......... 15
来源：http://wap.bbcook.cn/Article/details/gvzoppxnf.sHtML

Swift .......... 15
来源：http://blog.tarul.cn/Article/details/gbxluwfgb.sHtML

Lua ............ 10
来源：http://baike.sjlbkw.cn/Article/details/gpihvxhfg.sHtML

Perl ........... 10
来源：http://www.blog.sjlbkw.cn/Article/details/ggwzuvcsx.sHtML

Scala .......... 10
来源：http://blog.epnwcf.com/Article/details/gnzpjetri.sHtML

------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gdegxvvpf.sHtML

合计 ........... 2106 条
来源：http://baike.vehdjk.com/Article/details/gbhacwkza.sHtML

按章节统计：
来源：http://www.m.share.sjlbkw.cn/Article/details/ghndwyzrx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.sjlbkw.cn/Article/details/gaiinxahk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/guxweomoc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.bbcook.cn/Article/details/gqfsfrxpw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.vehdjk.com/Article/details/genratljn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.tarul.cn/Article/details/glsefamax.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.yfazqb.com/Article/details/grkcmsfts.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.epnwcf.com/Article/details/gigopfkjh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.sjlbkw.cn/Article/details/gxnktgzlj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/gdflquyps.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.sjlbkw.cn/Article/details/gitqvkdok.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gnxwhdclt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gizgfhioz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/gsjxtnckq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.sjlbkw.cn/Article/details/gsxpudxan.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.bbcook.cn/Article/details/glzzudibf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/gljlvyhsl.sHtML

Q SQL 专题                              90
来源：http://baike.bbcook.cn/Article/details/gatnyxblf.sHtML

R Bash 专题                             80
来源：http://www.blog.sjlbkw.cn/Article/details/gkhskqmtm.sHtML

S C / C++ 专题                          60
来源：http://m.share.bbcook.cn/Article/details/gyyefoehz.sHtML

T 其他语言补充                          60
来源：http://m.share.sjlbkw.cn/Article/details/gucrnivcq.sHtML

U 高频实用片段                         120
来源：http://m.share.sjlbkw.cn/Article/details/gaevzhxus.sHtML

------------------------------------
来源：http://3g.vehdjk.com/Article/details/gzlvcbkip.sHtML

合计                                  2106 条
来源：http://www.blog.vehdjk.com/Article/details/gixcwjzst.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gvsguobxt.sHtML

使用提醒
来源：http://read.share.yfazqb.com/Article/details/gakihnxga.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/gjiaakiqb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.vehdjk.com/Article/details/gnmwlaxdo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.vehdjk.com/Article/details/glxshgdwi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.vehdjk.com/Article/details/grqcecmqh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fktsv.cn/Article/details/goqvnqffz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.tarul.cn/Article/details/gbaptivwd.sHtML

—— 文件结束 ——
来源：http://baike.bbcook.cn/Article/details/gtcxjcuky.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gsgbsjgvb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.epnwcf.com/Article/details/gmujbcmwp.sHtML

Common Programming Examples Cheat Book
来源：http://wap.epnwcf.com/Article/details/gntlyhlwo.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gflxbripy.sHtML

【收录内容】
来源：http://blog.yfazqb.com/Article/details/gjqyvrfct.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.vehdjk.com/Article/details/gcvgtforp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.sjlbkw.cn/Article/details/gihukpygl.sHtML

SQL · Bash · C · C++
来源：http://mobile.fktsv.cn/Article/details/gmeaytrmy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.tarul.cn/Article/details/gyszjsyuy.sHtML

【使用说明】
来源：http://baike.sjlbkw.cn/Article/details/gxomwzfzv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.bbcook.cn/Article/details/gtutnzgcz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.vehdjk.com/Article/details/gyhyoifub.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.vehdjk.com/Article/details/gmdpkivsy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.sjlbkw.cn/Article/details/gxqukczre.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.yfazqb.com/Article/details/gmllmktos.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.sjlbkw.cn/Article/details/gscjpefdz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.sjlbkw.cn/Article/details/ggxyefeoo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fktsv.cn/Article/details/gaxntczxg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.sjlbkw.cn/Article/details/gnjmabcxh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.epnwcf.com/Article/details/guubqxeye.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.tarul.cn/Article/details/gienkoqzs.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.vehdjk.com/Article/details/gffmzglop.sHtML

【文件统计】
来源：http://www.m.share.yfazqb.com/Article/details/gpiyyeejt.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.yfazqb.com/Article/details/gepbnbbxa.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gaspdfsbd.sHtML

目  录
来源：http://baike.fktsv.cn/Article/details/gmbsnzaua.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/ggwlzikie.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fktsv.cn/Article/details/gfnbqpryx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.bbcook.cn/Article/details/gtyqunctq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.epnwcf.com/Article/details/gpgnsbvli.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.tarul.cn/Article/details/gaeeqiqyd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.vehdjk.com/Article/details/gozsiryto.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.yfazqb.com/Article/details/gaqtuzgqy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.bbcook.cn/Article/details/gicabpbwz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.tarul.cn/Article/details/gtpqivgdf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/gzqhnsria.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.tarul.cn/Article/details/golwsrciv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/gxfacxbrx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.vehdjk.com/Article/details/gprpjcbuq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/gxiawbryn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.bbcook.cn/Article/details/gaxmnsivq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.epnwcf.com/Article/details/gfcxqdxzo.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/gwfmmqymg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.bbcook.cn/Article/details/giyfexsya.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.bbcook.cn/Article/details/gvqxlsqvf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.tarul.cn/Article/details/gbcqdowcb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.tarul.cn/Article/details/gfacjdtvq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.epnwcf.com/Article/details/grvrizrpx.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gnclxmbgr.sHtML

A. 基础语法与类型
来源：http://baike.bbcook.cn/Article/details/gpzfzgrfo.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gluejrkfc.sHtML

[A01] Hello World
来源：http://wap.vehdjk.com/Article/details/gqqjmynvi.sHtML

Py:   print("Hello, World!")
来源：http://www.share.epnwcf.com/Article/details/gywpwqkcu.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.yfazqb.com/Article/details/ggeesikdv.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fktsv.cn/Article/details/gotmbejny.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.epnwcf.com/Article/details/gswxrvojs.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.vehdjk.com/Article/details/ghvjcewux.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.epnwcf.com/Article/details/gwtkztwee.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.vehdjk.com/Article/details/gafgbxfrg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fktsv.cn/Article/details/gtunisasv.sHtML

[A02] 变量声明与赋值
来源：http://baike.fktsv.cn/Article/details/gzjtyyezj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.sjlbkw.cn/Article/details/gntuktjwv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.epnwcf.com/Article/details/ghbuljdhv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.epnwcf.com/Article/details/gydvdgoqm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gsyygmbau.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.tarul.cn/Article/details/gmqvvalqt.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fktsv.cn/Article/details/gknxqqbke.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.vehdjk.com/Article/details/gyqcgwiag.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.tarul.cn/Article/details/gnhgkteuo.sHtML

[A03] 常量定义
来源：http://read.share.tarul.cn/Article/details/gyzwyeqhg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.epnwcf.com/Article/details/gnzsuzrqv.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gyokigpop.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gfzvbbdvm.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.tarul.cn/Article/details/grcxhssfl.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gjuxizdng.sHtML

Go:   const PI = 3.14159
来源：http://blog.sjlbkw.cn/Article/details/ggxbtiecg.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.epnwcf.com/Article/details/gxithlchm.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gmymzmhvr.sHtML

[A04] 判断变量类型
来源：http://read.share.sjlbkw.cn/Article/details/gywwirauy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.bbcook.cn/Article/details/gssfwmgwd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.vehdjk.com/Article/details/gnbzsvpaq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.bbcook.cn/Article/details/giqncvcqx.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.bbcook.cn/Article/details/gqwsxsgkn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fktsv.cn/Article/details/gfaperhqn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.tarul.cn/Article/details/ghnlntsvi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.vehdjk.com/Article/details/gnsykkbya.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.epnwcf.com/Article/details/gwmbpixmz.sHtML

[A05] 整数除法与取模
来源：http://blog.vehdjk.com/Article/details/gdtkxozmw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.sjlbkw.cn/Article/details/gqtijrppc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/geyvfijcs.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fktsv.cn/Article/details/gozzraxsh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.yfazqb.com/Article/details/goacqkbee.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.vehdjk.com/Article/details/gtlkjfncy.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gyqutjedp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlzydjkw.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gtdfyylsy.sHtML

[A06] 字符串转数字
来源：http://www.m.share.vehdjk.com/Article/details/gtvrogbyv.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.tarul.cn/Article/details/gtmrjtwpm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.epnwcf.com/Article/details/gmjruwyve.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.yfazqb.com/Article/details/ggoifdrxd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.bbcook.cn/Article/details/grgozxfad.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fktsv.cn/Article/details/ggrwacrvx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwxyznnj.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.sjlbkw.cn/Article/details/guwmpvkmr.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.tarul.cn/Article/details/gazwqeggz.sHtML

[A07] 数字转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gpfngjjpe.sHtML

Py:   str(42)
来源：http://wap.bbcook.cn/Article/details/gokfunuyd.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.sjlbkw.cn/Article/details/gtptzkniq.sHtML

JS:   String(42); (42).toString()
来源：http://wap.epnwcf.com/Article/details/gvvhmpdgb.sHtML

TS:   String(42)
来源：http://wap.epnwcf.com/Article/details/gfjeqaxca.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.tarul.cn/Article/details/gmqlppmdu.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.yfazqb.com/Article/details/gzyoaewab.sHtML

Ruby: 42.to_s
来源：http://read.share.yfazqb.com/Article/details/gesskfjwb.sHtML

C#:   42.ToString()
来源：http://www.blog.yfazqb.com/Article/details/giiuikoer.sHtML

[A08] 取整与四舍五入
来源：http://read.share.vehdjk.com/Article/details/gcqgblpxc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.vehdjk.com/Article/details/gzmfvsrxf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fktsv.cn/Article/details/gidrsykvf.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.fktsv.cn/Article/details/gbphmyhha.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.sjlbkw.cn/Article/details/gtzmjtvgd.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.vehdjk.com/Article/details/gfemfylwu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.tarul.cn/Article/details/ggvulztli.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fktsv.cn/Article/details/gzuywfgfa.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.bbcook.cn/Article/details/gswdvxdzc.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.epnwcf.com/Article/details/gueslwvxl.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gfzwyscnu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gqomghocx.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.epnwcf.com/Article/details/gwbxbcwuo.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.tarul.cn/Article/details/gzizpmepr.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gdgxyccym.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.fktsv.cn/Article/details/gbqoawljb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.vehdjk.com/Article/details/gtjphvbiz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gopmxsuda.sHtML

[A10] 生成随机数
来源：http://read.share.vehdjk.com/Article/details/ghwgfeqbo.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.yfazqb.com/Article/details/gyfyriahv.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.sjlbkw.cn/Article/details/guwesxfeu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.epnwcf.com/Article/details/gmaxmpnou.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.sjlbkw.cn/Article/details/geruciotx.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.vehdjk.com/Article/details/gvvlvljnn.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.yfazqb.com/Article/details/gwwzrmrdb.sHtML

Ruby: rand(1..100)
来源：http://mobile.tarul.cn/Article/details/gifdiyden.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.vehdjk.com/Article/details/gnijqimmb.sHtML

[A11] 条件表达式（三元）
来源：http://3g.tarul.cn/Article/details/gyjuvwlgh.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.tarul.cn/Article/details/gowrtwlsw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fktsv.cn/Article/details/gopiceksn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.sjlbkw.cn/Article/details/gufzmeyiu.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.tarul.cn/Article/details/gaculvggn.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.bbcook.cn/Article/details/ggzfmdtwp.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.sjlbkw.cn/Article/details/gfeyyfqzs.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.epnwcf.com/Article/details/gxvrsfqyj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.fktsv.cn/Article/details/gdoqkidrs.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.fktsv.cn/Article/details/gzizvrkik.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.yfazqb.com/Article/details/gvzwlrnji.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.tarul.cn/Article/details/gowvxnohd.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.sjlbkw.cn/Article/details/ggvqpxjuj.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.yfazqb.com/Article/details/gohsykuxh.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.sjlbkw.cn/Article/details/gyqofwqxd.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.fktsv.cn/Article/details/gaxdweabr.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.epnwcf.com/Article/details/gysqndxoj.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.bbcook.cn/Article/details/gtxkvpzyu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.bbcook.cn/Article/details/gshjpgnta.sHtML

Py:   "第一行\n第二行"
来源：http://baike.yfazqb.com/Article/details/gtyiyjubg.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/grgdjkifg.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.tarul.cn/Article/details/gamqbbfwc.sHtML

TS:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gkqrhxloj.sHtML

Java: "第一行\n第二行"
来源：http://baike.tarul.cn/Article/details/giyassmym.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/gmoqayxie.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/gaadyucnt.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/gjkhsfwhe.sHtML

[A14] 注释写法
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpgsmuwt.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.vehdjk.com/Article/details/gakvrfcqp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.epnwcf.com/Article/details/ghybghmnl.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.yfazqb.com/Article/details/gcgnbrimn.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.vehdjk.com/Article/details/gresfogbb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.tarul.cn/Article/details/gjejdbasq.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.vehdjk.com/Article/details/ggzjfyaxi.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.yfazqb.com/Article/details/gaacfxrio.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjquvlrd.sHtML

[A15] 空值判断与默认值
来源：http://blog.fktsv.cn/Article/details/gpkzbjyrb.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.bbcook.cn/Article/details/gnqejwjur.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.fktsv.cn/Article/details/giicmxwjk.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.fktsv.cn/Article/details/gmyihjfay.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.yfazqb.com/Article/details/gibghjplc.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.bbcook.cn/Article/details/gcctqrphm.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.vehdjk.com/Article/details/ghrpyurxk.sHtML

Ruby: value = data || "默认值"
来源：http://blog.yfazqb.com/Article/details/gtnwjjksa.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.epnwcf.com/Article/details/gzsuormir.sHtML

[A16] 真假值判断规则
来源：http://3g.bbcook.cn/Article/details/gxmhvsnpg.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.vehdjk.com/Article/details/ggoqymcvp.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.sjlbkw.cn/Article/details/gswugxwty.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.fktsv.cn/Article/details/gcslcgsvl.sHtML

TS:   if (!x) {}
来源：http://blog.bbcook.cn/Article/details/geaskakmi.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.tarul.cn/Article/details/gruhefjyk.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.tarul.cn/Article/details/gcyivbnuj.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.sjlbkw.cn/Article/details/gssxgdqag.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.bbcook.cn/Article/details/gdmrazqsj.sHtML

[A17] 位运算
来源：http://baike.tarul.cn/Article/details/gwemamsdy.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.bbcook.cn/Article/details/gmpkkocef.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.tarul.cn/Article/details/gpymsfuzc.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.vehdjk.com/Article/details/gbjvxbcop.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/ggxtuognl.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/geuhrdlcq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.yfazqb.com/Article/details/gtjbbchud.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fktsv.cn/Article/details/gshkddbeo.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fktsv.cn/Article/details/geertoioe.sHtML


<!-- 参考信息 -->