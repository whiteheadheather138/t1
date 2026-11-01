代发 wailian999

[U95] JS：Promise 包装
来源：http://read.share.sjlbkw.cn/Article/details/gnruyfvjd.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.bbcook.cn/Article/details/gkithugcd.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.tarul.cn/Article/details/ghhhxfsmd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gxhhoymqk.sHtML

[U97] JS：并发请求
来源：http://www.blog.fktsv.cn/Article/details/gmgspdbvy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gcsfeucuk.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.bbcook.cn/Article/details/gphvxqshp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.tarul.cn/Article/details/gjnwrtlcz.sHtML

[U99] JS：事件监听
来源：http://blog.fktsv.cn/Article/details/gmrlwvgrb.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.bbcook.cn/Article/details/gctatbvoc.sHtML

[U100] JS：DOM 查询
来源：http://3g.sjlbkw.cn/Article/details/grjnnkcce.sHtML

document.querySelector(".item")
来源：http://baike.sjlbkw.cn/Article/details/gndiicskx.sHtML

[U101] JS：classList 操作
来源：http://wap.tarul.cn/Article/details/gbaoyovxc.sHtML

el.classList.toggle("active")
来源：http://m.share.tarul.cn/Article/details/geoswposq.sHtML

[U102] JS：本地存储
来源：http://blog.epnwcf.com/Article/details/grfflzzmv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.bbcook.cn/Article/details/gqdxrbvgg.sHtML

[U103] JS：定时器
来源：http://wap.epnwcf.com/Article/details/gequydtdl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.bbcook.cn/Article/details/gkdypmvym.sHtML

[U104] JS：防抖
来源：http://baike.bbcook.cn/Article/details/gbilelaxn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.bbcook.cn/Article/details/geaekgbif.sHtML

[U105] JS：节流
来源：http://3g.epnwcf.com/Article/details/gkxzjslbq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.yfazqb.com/Article/details/gseagxpcv.sHtML

[U106] JS：日期格式化
来源：http://wap.epnwcf.com/Article/details/gzmkxnqos.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.sjlbkw.cn/Article/details/gxvudrurs.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.tarul.cn/Article/details/gpvotixpg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.epnwcf.com/Article/details/gilhpymww.sHtML

[U108] JS：随机整数
来源：http://wap.fktsv.cn/Article/details/gujdtuljn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.tarul.cn/Article/details/gediidull.sHtML

[U109] JS：数组分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gumxxsvfa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.sjlbkw.cn/Article/details/ghccmbkck.sHtML

[U110] JS：数组分块
来源：http://read.share.bbcook.cn/Article/details/ggtzvhorp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.tarul.cn/Article/details/gkpybwyxm.sHtML

[U111] JS：对象转 Map
来源：http://baike.fktsv.cn/Article/details/geumlfmhw.sHtML

new Map(Object.entries(obj))
来源：http://www.share.bbcook.cn/Article/details/gxbdgxbfp.sHtML

[U112] JS：字符串补位
来源：http://baike.yfazqb.com/Article/details/ghwizzjik.sHtML

"7".padStart(3, "0")
来源：http://wap.fktsv.cn/Article/details/gfvklzbpl.sHtML

[U113] JS：正则替换全部
来源：http://read.share.yfazqb.com/Article/details/gxarsrenf.sHtML

s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gjnldqtnt.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.sjlbkw.cn/Article/details/gbevqyxqi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gljamywvw.sHtML

[U115] JS：生成 UUID
来源：http://blog.sjlbkw.cn/Article/details/gzcwqbpwh.sHtML

crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/gnvpeortr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.bbcook.cn/Article/details/gtteearqy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.sjlbkw.cn/Article/details/gkeviwbrq.sHtML

[U117] JS：单元测试
来源：http://blog.bbcook.cn/Article/details/guhvkaoyo.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.tarul.cn/Article/details/gyppxaszb.sHtML

[U118] JS：开发服务器
来源：http://baike.fktsv.cn/Article/details/gjmswetpu.sHtML

npm i -D vite;  npx vite
来源：http://mobile.tarul.cn/Article/details/gdksboezv.sHtML

[U119] JS：生产构建
来源：http://m.share.epnwcf.com/Article/details/grycmkgpj.sHtML

npx vite build
来源：http://www.share.epnwcf.com/Article/details/gdgjjuekf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.vehdjk.com/Article/details/gndumeeet.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.vehdjk.com/Article/details/gjnowdgdq.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ggfqnwhiq.sHtML

统计汇总
来源：http://3g.epnwcf.com/Article/details/gmtcwrbtb.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/giodtpejz.sHtML

按语言统计（条）：
来源：http://www.m.share.yfazqb.com/Article/details/gdcdhvnuw.sHtML

Python ......... 252
来源：http://wap.yfazqb.com/Article/details/gsvprfnfx.sHtML

PHP ............ 252
来源：http://www.m.share.vehdjk.com/Article/details/gehbgyxhl.sHtML

JavaScript ..... 252
来源：http://wap.yfazqb.com/Article/details/gpkldgluw.sHtML

TypeScript ..... 212
来源：http://3g.tarul.cn/Article/details/gnmxcahun.sHtML

Java ........... 212
来源：http://m.share.bbcook.cn/Article/details/gbcelqzfm.sHtML

Go ............. 212
来源：http://read.share.bbcook.cn/Article/details/gvwuqfplk.sHtML

Ruby ........... 212
来源：http://mobile.bbcook.cn/Article/details/gzkpnvzle.sHtML

C# ............. 212
来源：http://www.blog.tarul.cn/Article/details/gucxgmvrb.sHtML

C .............. 30
来源：http://blog.vehdjk.com/Article/details/gedghkmnk.sHtML

C++ ............ 30
来源：http://www.share.vehdjk.com/Article/details/gvektxwhl.sHtML

SQL ............ 90
来源：http://wap.yfazqb.com/Article/details/ggvcsyhzm.sHtML

Bash ........... 80
来源：http://www.share.yfazqb.com/Article/details/gyqmykfic.sHtML

Kotlin ......... 15
来源：http://blog.epnwcf.com/Article/details/gzsojkcym.sHtML

Swift .......... 15
来源：http://read.share.vehdjk.com/Article/details/gvklkdabg.sHtML

Lua ............ 10
来源：http://m.share.tarul.cn/Article/details/gynudjdld.sHtML

Perl ........... 10
来源：http://www.share.vehdjk.com/Article/details/gumumjtrb.sHtML

Scala .......... 10
来源：http://m.share.bbcook.cn/Article/details/gadgetwlk.sHtML

------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gtntpjkex.sHtML

合计 ........... 2106 条
来源：http://mobile.epnwcf.com/Article/details/gzxsraktr.sHtML

按章节统计：
来源：http://3g.epnwcf.com/Article/details/gtiewfcxo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.bbcook.cn/Article/details/grvgfggxl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.yfazqb.com/Article/details/gvpfsofxr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.tarul.cn/Article/details/gipsltpfj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.vehdjk.com/Article/details/gicfgocrn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.tarul.cn/Article/details/ggzhpqwgj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.vehdjk.com/Article/details/gpgsmyufe.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.epnwcf.com/Article/details/gzdiamyal.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fktsv.cn/Article/details/gtkgppfng.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gospsicjm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.epnwcf.com/Article/details/ghbjazdqp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/goybybita.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gztnirsks.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/gtngtpzwc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fktsv.cn/Article/details/gsbtisfns.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.bbcook.cn/Article/details/grpoopdkx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gubeejnhm.sHtML

Q SQL 专题                              90
来源：http://3g.bbcook.cn/Article/details/gpefwadsw.sHtML

R Bash 专题                             80
来源：http://blog.epnwcf.com/Article/details/gyoudszrh.sHtML

S C / C++ 专题                          60
来源：http://mobile.bbcook.cn/Article/details/gypfgcpsv.sHtML

T 其他语言补充                          60
来源：http://3g.vehdjk.com/Article/details/gqwoqkyjc.sHtML

U 高频实用片段                         120
来源：http://www.share.bbcook.cn/Article/details/gbblfalvr.sHtML

------------------------------------
来源：http://blog.vehdjk.com/Article/details/gzjkxvlao.sHtML

合计                                  2106 条
来源：http://read.share.bbcook.cn/Article/details/gobnhpohv.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.yfazqb.com/Article/details/ggmobrrca.sHtML

使用提醒
来源：http://www.blog.vehdjk.com/Article/details/gpmygdpzt.sHtML

--------------------------------------------------------------------------------
来源：http://baike.bbcook.cn/Article/details/gsibykvth.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.yfazqb.com/Article/details/gikzkitye.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.bbcook.cn/Article/details/gvetouwvj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.vehdjk.com/Article/details/gffmtqokq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.yfazqb.com/Article/details/giodetwig.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.yfazqb.com/Article/details/gsqojsaqp.sHtML

—— 文件结束 ——
来源：http://www.blog.fktsv.cn/Article/details/gkpxonvol.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gneltpyaf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.bbcook.cn/Article/details/gophicuuf.sHtML

Common Programming Examples Cheat Book
来源：http://baike.sjlbkw.cn/Article/details/ghndkdvmj.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gnbmthtmj.sHtML

【收录内容】
来源：http://read.share.tarul.cn/Article/details/gejaswgam.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.vehdjk.com/Article/details/gzroodngs.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.vehdjk.com/Article/details/goqfsfwkg.sHtML

SQL · Bash · C · C++
来源：http://read.share.vehdjk.com/Article/details/gntermdcc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.bbcook.cn/Article/details/gzslejnar.sHtML

【使用说明】
来源：http://www.share.sjlbkw.cn/Article/details/gocodfdne.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.tarul.cn/Article/details/gqxopmbxu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.yfazqb.com/Article/details/gawnmdgez.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.bbcook.cn/Article/details/gpmumxsta.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.epnwcf.com/Article/details/giycfvjhl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrfpmgic.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.tarul.cn/Article/details/gsziigfls.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.yfazqb.com/Article/details/gatnwpmvt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.bbcook.cn/Article/details/gqwglbpnp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.yfazqb.com/Article/details/gqvxzktvh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.epnwcf.com/Article/details/ghpsqcgsn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fktsv.cn/Article/details/gajsssycb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fktsv.cn/Article/details/gljcxoobq.sHtML

【文件统计】
来源：http://www.m.share.yfazqb.com/Article/details/gjqywyfqx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.tarul.cn/Article/details/grvictevf.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/gpeqpqokk.sHtML

目  录
来源：http://mobile.yfazqb.com/Article/details/gczmtgryw.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/glhdycsqc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.epnwcf.com/Article/details/gfeggtlqr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.bbcook.cn/Article/details/gjssjdpyi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.tarul.cn/Article/details/gcnypgrwk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.vehdjk.com/Article/details/gmluarfdj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fktsv.cn/Article/details/gpvexxojp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.bbcook.cn/Article/details/gaeixjups.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.vehdjk.com/Article/details/gecivcsat.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fktsv.cn/Article/details/goscabrjp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.sjlbkw.cn/Article/details/gjwmozoud.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.tarul.cn/Article/details/grpgmlfta.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/getlqobpr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/gobyufbuo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.sjlbkw.cn/Article/details/glnpqqqea.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.tarul.cn/Article/details/gmzzrzwsf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.epnwcf.com/Article/details/glfcgpiwa.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.vehdjk.com/Article/details/gsyuindlq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.sjlbkw.cn/Article/details/gjsamtijl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.tarul.cn/Article/details/gycruzuju.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.bbcook.cn/Article/details/gvkxvkswi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/gcuhagjui.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.vehdjk.com/Article/details/gtpamtwfj.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gtpffmxii.sHtML

A. 基础语法与类型
来源：http://m.share.sjlbkw.cn/Article/details/gcysjvsoe.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/geqftenek.sHtML

[A01] Hello World
来源：http://blog.sjlbkw.cn/Article/details/gacsgzkqu.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fktsv.cn/Article/details/ghvvfmuqf.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fktsv.cn/Article/details/gienywrmd.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fktsv.cn/Article/details/ghdfbuerk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fktsv.cn/Article/details/gwyxkuigu.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.yfazqb.com/Article/details/grgjufywg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.vehdjk.com/Article/details/gcpnhnzfp.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.sjlbkw.cn/Article/details/ghyxznvie.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.sjlbkw.cn/Article/details/grznrewpg.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.bbcook.cn/Article/details/grpcmadcx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.yfazqb.com/Article/details/govyxaarv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.epnwcf.com/Article/details/gzrifqttd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.bbcook.cn/Article/details/gximtgouw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.epnwcf.com/Article/details/gvoxtaqjk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.tarul.cn/Article/details/gjuhgrsga.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.tarul.cn/Article/details/gtqnhflsc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.sjlbkw.cn/Article/details/goacaasgm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.sjlbkw.cn/Article/details/glubmufun.sHtML

[A03] 常量定义
来源：http://baike.vehdjk.com/Article/details/ghtlmawiw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.yfazqb.com/Article/details/gsgbcqsui.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/grqidunzk.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/glqrojthj.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gnlrgodmx.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gvxhbazif.sHtML

Go:   const PI = 3.14159
来源：http://m.share.sjlbkw.cn/Article/details/guoyfnsgt.sHtML

Ruby: PI = 3.14159
来源：http://3g.epnwcf.com/Article/details/gdeghlcvw.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gbuhrgfwj.sHtML

[A04] 判断变量类型
来源：http://wap.vehdjk.com/Article/details/gcxozxtab.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.vehdjk.com/Article/details/gqkdgwdxm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.epnwcf.com/Article/details/glpaehozu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.tarul.cn/Article/details/gfattdbhx.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.yfazqb.com/Article/details/grwyihduu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.tarul.cn/Article/details/gkrujvfbx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.tarul.cn/Article/details/gyyvnkifd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.tarul.cn/Article/details/gjvbovppr.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fktsv.cn/Article/details/ggtwijxlj.sHtML

[A05] 整数除法与取模
来源：http://read.share.bbcook.cn/Article/details/gynbxaqiv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.epnwcf.com/Article/details/groxxtlat.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.yfazqb.com/Article/details/gvffkpljv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.bbcook.cn/Article/details/gclgnpcfq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.bbcook.cn/Article/details/ghzudzbus.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/gkxnutnki.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gfpvmiymi.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/gmsjsfwyq.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.epnwcf.com/Article/details/gigloprhu.sHtML

[A06] 字符串转数字
来源：http://read.share.tarul.cn/Article/details/gmumyzmij.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.yfazqb.com/Article/details/gxfisitwm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fktsv.cn/Article/details/gxwrthzvw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.vehdjk.com/Article/details/gjftgtaat.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.epnwcf.com/Article/details/gbhhhwsyt.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fktsv.cn/Article/details/giqkugknu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.yfazqb.com/Article/details/glibgadcb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.yfazqb.com/Article/details/gqhmadjce.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.tarul.cn/Article/details/gcahsnfef.sHtML

[A07] 数字转字符串
来源：http://www.blog.epnwcf.com/Article/details/grwrszymw.sHtML

Py:   str(42)
来源：http://www.share.fktsv.cn/Article/details/gharmubsj.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.yfazqb.com/Article/details/giliwuqpk.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.yfazqb.com/Article/details/ghlrlghgo.sHtML

TS:   String(42)
来源：http://www.share.epnwcf.com/Article/details/gfyjynygh.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.vehdjk.com/Article/details/gjyhbtpdy.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.epnwcf.com/Article/details/gfrjtvsbx.sHtML

Ruby: 42.to_s
来源：http://read.share.tarul.cn/Article/details/goiwsmaiz.sHtML

C#:   42.ToString()
来源：http://m.share.epnwcf.com/Article/details/guardywkz.sHtML

[A08] 取整与四舍五入
来源：http://www.share.tarul.cn/Article/details/gnsovccex.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/gqgogwntc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.vehdjk.com/Article/details/gsjexufke.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.epnwcf.com/Article/details/gfxwghqgq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.epnwcf.com/Article/details/gpecdwtjd.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.tarul.cn/Article/details/gawkvreoa.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.epnwcf.com/Article/details/grhhrihwa.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.sjlbkw.cn/Article/details/gvcqsrjxw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.yfazqb.com/Article/details/gozojvufz.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.yfazqb.com/Article/details/gtxbamcwa.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.vehdjk.com/Article/details/guqagzqzr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gjlbgqjzc.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.yfazqb.com/Article/details/ghqgwiqgm.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gdfciffhj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.fktsv.cn/Article/details/ggcymuyrz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.vehdjk.com/Article/details/gpsvwehyl.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.tarul.cn/Article/details/gtqazalup.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.tarul.cn/Article/details/gdrhpcydu.sHtML

[A10] 生成随机数
来源：http://baike.epnwcf.com/Article/details/gjzstduek.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.sjlbkw.cn/Article/details/gxtswhbzw.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.bbcook.cn/Article/details/gevnkgeuz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.bbcook.cn/Article/details/gmazdyiow.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fktsv.cn/Article/details/gkvjpfjjd.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.bbcook.cn/Article/details/girasivcg.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.sjlbkw.cn/Article/details/gksdiunfh.sHtML

Ruby: rand(1..100)
来源：http://blog.sjlbkw.cn/Article/details/gkmyyuliv.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.sjlbkw.cn/Article/details/gthgapsmw.sHtML

[A11] 条件表达式（三元）
来源：http://wap.tarul.cn/Article/details/gwrmuqavv.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.sjlbkw.cn/Article/details/gjzdfopzz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.bbcook.cn/Article/details/gfjyopfho.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.yfazqb.com/Article/details/gpvvdufhr.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.sjlbkw.cn/Article/details/ghsrsqeqb.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.bbcook.cn/Article/details/gfqekybgf.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.bbcook.cn/Article/details/gnhshxiee.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.sjlbkw.cn/Article/details/gmybnmdqs.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fktsv.cn/Article/details/gwjvgngdd.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.sjlbkw.cn/Article/details/gazlwmcwu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.fktsv.cn/Article/details/gjkhsgfgo.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.bbcook.cn/Article/details/govvllumv.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.tarul.cn/Article/details/gcrqedrer.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.fktsv.cn/Article/details/gmiardurn.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.vehdjk.com/Article/details/giupxpelx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.fktsv.cn/Article/details/gnevqkzlo.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.vehdjk.com/Article/details/gtmjidyce.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.fktsv.cn/Article/details/gwwfcilwe.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.fktsv.cn/Article/details/grurbqzoo.sHtML

Py:   "第一行\n第二行"
来源：http://baike.tarul.cn/Article/details/gsfkkuhfu.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/geogzyklg.sHtML

JS:   "第一行\n第二行"
来源：http://baike.tarul.cn/Article/details/gwemexzpy.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/ggoflwmoj.sHtML

Java: "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/guyijlwjk.sHtML

Go:   "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gketjlmyj.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/gxmnjbzdj.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gvgjndhfy.sHtML

[A14] 注释写法
来源：http://m.share.sjlbkw.cn/Article/details/gdglvkkpt.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.sjlbkw.cn/Article/details/gwkifqztk.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.epnwcf.com/Article/details/gjxztijgm.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.bbcook.cn/Article/details/gaoonchzm.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.yfazqb.com/Article/details/grrpguvpd.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gvoskliox.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/gxhxzlene.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.yfazqb.com/Article/details/gxecnahzy.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.yfazqb.com/Article/details/gtuabizkc.sHtML

[A15] 空值判断与默认值
来源：http://mobile.epnwcf.com/Article/details/gputjgcmh.sHtML

Py:   value = data or "默认值"
来源：http://blog.sjlbkw.cn/Article/details/gucqtkfap.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.sjlbkw.cn/Article/details/gyfseutiz.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.tarul.cn/Article/details/gfudjnkcg.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.bbcook.cn/Article/details/gmqhfahfn.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.vehdjk.com/Article/details/gmeryzbgq.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.vehdjk.com/Article/details/gstunhltp.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.bbcook.cn/Article/details/ggdshgcbo.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.yfazqb.com/Article/details/gvumurekw.sHtML

[A16] 真假值判断规则
来源：http://baike.yfazqb.com/Article/details/gzofxcxra.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.fktsv.cn/Article/details/gphlnvzqk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.epnwcf.com/Article/details/gjpaogmgs.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.fktsv.cn/Article/details/gmvaeftpk.sHtML

TS:   if (!x) {}
来源：http://blog.vehdjk.com/Article/details/gxcnpxmoo.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.sjlbkw.cn/Article/details/gbupwnave.sHtML


<!-- 参考信息 -->