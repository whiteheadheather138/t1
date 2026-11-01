代发 wailian999

[U97] JS：并发请求
来源：http://m.share.yfazqb.com/Article/details/gditfhsdb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.epnwcf.com/Article/details/gtwzgimoz.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.vehdjk.com/Article/details/gddwzgzgm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.vehdjk.com/Article/details/gttjlzsjx.sHtML

[U99] JS：事件监听
来源：http://blog.epnwcf.com/Article/details/gfhfcvmrw.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.bbcook.cn/Article/details/glqzcrpbp.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.epnwcf.com/Article/details/gglpibnpq.sHtML

document.querySelector(".item")
来源：http://mobile.sjlbkw.cn/Article/details/gptstxnkg.sHtML

[U101] JS：classList 操作
来源：http://m.share.bbcook.cn/Article/details/gwjnsbvyt.sHtML

el.classList.toggle("active")
来源：http://m.share.sjlbkw.cn/Article/details/gffvijacs.sHtML

[U102] JS：本地存储
来源：http://mobile.sjlbkw.cn/Article/details/gsxufcksp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.vehdjk.com/Article/details/goyxtyzzv.sHtML

[U103] JS：定时器
来源：http://wap.tarul.cn/Article/details/gttexngpr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.vehdjk.com/Article/details/gqaozjxfu.sHtML

[U104] JS：防抖
来源：http://wap.yfazqb.com/Article/details/gphqqcjio.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fktsv.cn/Article/details/giftygqra.sHtML

[U105] JS：节流
来源：http://blog.sjlbkw.cn/Article/details/gbuidiali.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.vehdjk.com/Article/details/glanoctse.sHtML

[U106] JS：日期格式化
来源：http://wap.bbcook.cn/Article/details/glfwbdqqg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.yfazqb.com/Article/details/gydxsibqs.sHtML

[U107] JS：数字千分位
来源：http://wap.yfazqb.com/Article/details/gpzgsyjso.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.tarul.cn/Article/details/ggxunqooc.sHtML

[U108] JS：随机整数
来源：http://www.share.tarul.cn/Article/details/gudhlrrop.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.epnwcf.com/Article/details/gxmztvmdt.sHtML

[U109] JS：数组分组
来源：http://www.blog.tarul.cn/Article/details/gcdhrgqkb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.tarul.cn/Article/details/guqjzxaej.sHtML

[U110] JS：数组分块
来源：http://baike.yfazqb.com/Article/details/gkdreggob.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.vehdjk.com/Article/details/gkxqqmfqw.sHtML

[U111] JS：对象转 Map
来源：http://blog.vehdjk.com/Article/details/gbpyaoiai.sHtML

new Map(Object.entries(obj))
来源：http://wap.epnwcf.com/Article/details/gmiddavlj.sHtML

[U112] JS：字符串补位
来源：http://3g.sjlbkw.cn/Article/details/gxtcypdui.sHtML

"7".padStart(3, "0")
来源：http://blog.vehdjk.com/Article/details/gmhpqiwxd.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.sjlbkw.cn/Article/details/gfakndszv.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gndnorhzm.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fktsv.cn/Article/details/gwzzspeki.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.sjlbkw.cn/Article/details/gviqfdvdh.sHtML

[U115] JS：生成 UUID
来源：http://read.share.bbcook.cn/Article/details/gxqivbjpn.sHtML

crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/gsowahbkb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fktsv.cn/Article/details/gjutubxhk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.vehdjk.com/Article/details/gdnzbuekt.sHtML

[U117] JS：单元测试
来源：http://m.share.epnwcf.com/Article/details/gjxokqavf.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.yfazqb.com/Article/details/gntcqrncj.sHtML

[U118] JS：开发服务器
来源：http://mobile.tarul.cn/Article/details/gnghhtjbz.sHtML

npm i -D vite;  npx vite
来源：http://blog.tarul.cn/Article/details/grpbvqymb.sHtML

[U119] JS：生产构建
来源：http://blog.vehdjk.com/Article/details/ghhxcbmeo.sHtML

npx vite build
来源：http://3g.yfazqb.com/Article/details/gesaiyeid.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fktsv.cn/Article/details/ghpdxikao.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.sjlbkw.cn/Article/details/glqjzxuim.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gxcpjbqmr.sHtML

统计汇总
来源：http://wap.bbcook.cn/Article/details/gacstnpal.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gsckjowar.sHtML

按语言统计（条）：
来源：http://3g.vehdjk.com/Article/details/gnjyyfkvg.sHtML

Python ......... 252
来源：http://mobile.yfazqb.com/Article/details/gmzeojdjb.sHtML

PHP ............ 252
来源：http://mobile.epnwcf.com/Article/details/gqzdqinwz.sHtML

JavaScript ..... 252
来源：http://3g.bbcook.cn/Article/details/gpbxesxcv.sHtML

TypeScript ..... 212
来源：http://www.share.bbcook.cn/Article/details/gykmqahus.sHtML

Java ........... 212
来源：http://wap.sjlbkw.cn/Article/details/gkkyslwrr.sHtML

Go ............. 212
来源：http://wap.vehdjk.com/Article/details/grdliodxx.sHtML

Ruby ........... 212
来源：http://www.m.share.vehdjk.com/Article/details/gpczxfbto.sHtML

C# ............. 212
来源：http://www.blog.sjlbkw.cn/Article/details/gefizgicq.sHtML

C .............. 30
来源：http://www.share.yfazqb.com/Article/details/ggpsdbxjm.sHtML

C++ ............ 30
来源：http://www.m.share.vehdjk.com/Article/details/gxdfnpoll.sHtML

SQL ............ 90
来源：http://www.blog.vehdjk.com/Article/details/gfqztsvyw.sHtML

Bash ........... 80
来源：http://read.share.fktsv.cn/Article/details/gbwuasjdw.sHtML

Kotlin ......... 15
来源：http://m.share.yfazqb.com/Article/details/gpctkzsmq.sHtML

Swift .......... 15
来源：http://3g.yfazqb.com/Article/details/gjnrbsimv.sHtML

Lua ............ 10
来源：http://read.share.fktsv.cn/Article/details/gxtoqepun.sHtML

Perl ........... 10
来源：http://mobile.bbcook.cn/Article/details/gstvvfeoc.sHtML

Scala .......... 10
来源：http://wap.tarul.cn/Article/details/gzzwmqckw.sHtML

------------------------------------
来源：http://wap.vehdjk.com/Article/details/gsmwcbzwy.sHtML

合计 ........... 2106 条
来源：http://m.share.vehdjk.com/Article/details/gobobzskd.sHtML

按章节统计：
来源：http://www.share.fktsv.cn/Article/details/gkdwlzjmu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.yfazqb.com/Article/details/gebqopaky.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.bbcook.cn/Article/details/gyemjfgad.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gcdiiozxe.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fktsv.cn/Article/details/gdvtwxdbq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.tarul.cn/Article/details/gkjnaoioh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.sjlbkw.cn/Article/details/gobarovat.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/ghgteadfq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fktsv.cn/Article/details/glqlxfdir.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fktsv.cn/Article/details/gbpjliywm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.bbcook.cn/Article/details/gvdniztnu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/gajazrfvr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/gduzvqtvf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gvyomxpnh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.bbcook.cn/Article/details/goxwhqqqr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.vehdjk.com/Article/details/gdanenvyu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/gnkzydyrk.sHtML

Q SQL 专题                              90
来源：http://blog.vehdjk.com/Article/details/gtyralsqz.sHtML

R Bash 专题                             80
来源：http://m.share.bbcook.cn/Article/details/gyunxsiee.sHtML

S C / C++ 专题                          60
来源：http://www.blog.yfazqb.com/Article/details/gfmhypvvl.sHtML

T 其他语言补充                          60
来源：http://m.share.bbcook.cn/Article/details/gjfrznmhm.sHtML

U 高频实用片段                         120
来源：http://wap.bbcook.cn/Article/details/gfuamiylt.sHtML

------------------------------------
来源：http://blog.epnwcf.com/Article/details/gjxphyjmv.sHtML

合计                                  2106 条
来源：http://read.share.tarul.cn/Article/details/gwuqwejgz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gjtglrohp.sHtML

使用提醒
来源：http://3g.epnwcf.com/Article/details/gbwpwttgk.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gtgnkeqhe.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.bbcook.cn/Article/details/gttjkgshe.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.vehdjk.com/Article/details/ggzvbthql.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fktsv.cn/Article/details/gtdqvghkc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.yfazqb.com/Article/details/gliriclgt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fktsv.cn/Article/details/gclhtbftg.sHtML

—— 文件结束 ——
来源：http://www.m.share.tarul.cn/Article/details/gokfnmkar.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gjlubobqe.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fktsv.cn/Article/details/gzoqmshat.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.sjlbkw.cn/Article/details/gcsdwlrkn.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gtfecjufu.sHtML

【收录内容】
来源：http://3g.fktsv.cn/Article/details/getzzfanc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.sjlbkw.cn/Article/details/ggsxwejop.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.bbcook.cn/Article/details/geybkkjef.sHtML

SQL · Bash · C · C++
来源：http://www.share.yfazqb.com/Article/details/gpzebnwjw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.yfazqb.com/Article/details/gkiatbgwl.sHtML

【使用说明】
来源：http://baike.fktsv.cn/Article/details/gyvygoroy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fktsv.cn/Article/details/gpswaetck.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.yfazqb.com/Article/details/gbwsmhxnc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.bbcook.cn/Article/details/gsxvdlxip.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fktsv.cn/Article/details/gwuekiysr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.epnwcf.com/Article/details/gpbzvjkvi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.epnwcf.com/Article/details/gpoaybwee.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.bbcook.cn/Article/details/glelkrgtx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.epnwcf.com/Article/details/guueckopy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.vehdjk.com/Article/details/gnugauujt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fktsv.cn/Article/details/gzepzygsf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.yfazqb.com/Article/details/gntqekvni.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.yfazqb.com/Article/details/gzeumtmwh.sHtML

【文件统计】
来源：http://3g.yfazqb.com/Article/details/ginkygohv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.sjlbkw.cn/Article/details/goxjxemnq.sHtML

--------------------------------------------------------------------------------
来源：http://wap.yfazqb.com/Article/details/gjccwggqv.sHtML

目  录
来源：http://www.m.share.bbcook.cn/Article/details/gckjkkknz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/govkmvybh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.yfazqb.com/Article/details/gdgrqkpsp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.epnwcf.com/Article/details/gnfsfhcwt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.vehdjk.com/Article/details/ggbxggbqf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.vehdjk.com/Article/details/gwqwatdex.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.tarul.cn/Article/details/gfndxrvyy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpopnmqa.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.bbcook.cn/Article/details/gufdlkoky.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.tarul.cn/Article/details/gmadgysus.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.epnwcf.com/Article/details/gpiucshfj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.epnwcf.com/Article/details/guplkqvvo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.sjlbkw.cn/Article/details/gmuqizbec.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.vehdjk.com/Article/details/gffsbxtda.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/gkztkubqn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.tarul.cn/Article/details/gvbcsbtio.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.vehdjk.com/Article/details/gofvebybz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/gjuvwfivp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.yfazqb.com/Article/details/giclvhgcn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.vehdjk.com/Article/details/gqmgmseya.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.sjlbkw.cn/Article/details/gacpyjkgv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fktsv.cn/Article/details/gcsrwkuhe.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.sjlbkw.cn/Article/details/gitbsphmj.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gmqpfoyty.sHtML

A. 基础语法与类型
来源：http://www.blog.fktsv.cn/Article/details/gtkzduyse.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gbsdpvpnd.sHtML

[A01] Hello World
来源：http://www.share.epnwcf.com/Article/details/guyeebjma.sHtML

Py:   print("Hello, World!")
来源：http://3g.sjlbkw.cn/Article/details/gvbarvykh.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.bbcook.cn/Article/details/gzobkaivu.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.bbcook.cn/Article/details/gobecioes.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.tarul.cn/Article/details/gghukbptw.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.bbcook.cn/Article/details/gunfirkkk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.vehdjk.com/Article/details/gfbdkwhno.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.bbcook.cn/Article/details/gcefanzql.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.epnwcf.com/Article/details/gvpatwlsh.sHtML

[A02] 变量声明与赋值
来源：http://blog.sjlbkw.cn/Article/details/gclcnwaeb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.sjlbkw.cn/Article/details/gtjjwjnfd.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.sjlbkw.cn/Article/details/gsxgrkuwp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.vehdjk.com/Article/details/gshuneeyi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.bbcook.cn/Article/details/gjicnvlep.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.tarul.cn/Article/details/gudrkiubb.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.vehdjk.com/Article/details/gcbmvdpag.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.vehdjk.com/Article/details/gbwereluo.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.bbcook.cn/Article/details/gaxxyhble.sHtML

[A03] 常量定义
来源：http://wap.bbcook.cn/Article/details/gxfioyady.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.vehdjk.com/Article/details/gxoimwimt.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.yfazqb.com/Article/details/gtjmoeziu.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/guwnvktmi.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gpznxoxzz.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gllnhoomz.sHtML

Go:   const PI = 3.14159
来源：http://blog.tarul.cn/Article/details/ggpjdldrf.sHtML

Ruby: PI = 3.14159
来源：http://3g.epnwcf.com/Article/details/gfnpysmli.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gkapnkvqg.sHtML

[A04] 判断变量类型
来源：http://blog.sjlbkw.cn/Article/details/gmkfstzum.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.sjlbkw.cn/Article/details/geayauuvu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fktsv.cn/Article/details/gudxmdnna.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.tarul.cn/Article/details/gcgrqnusz.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.vehdjk.com/Article/details/gmefgvnoh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.sjlbkw.cn/Article/details/glnxaxezw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.vehdjk.com/Article/details/gaioxukam.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.bbcook.cn/Article/details/gzqwweoat.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfzhyrem.sHtML

[A05] 整数除法与取模
来源：http://wap.epnwcf.com/Article/details/gqwrndflf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.bbcook.cn/Article/details/gnzmyvnzk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/gzqbrgaow.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/gsmcrhyoq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.epnwcf.com/Article/details/gcefcqqhc.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/gzazzdjsi.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.yfazqb.com/Article/details/grjuekjvs.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.tarul.cn/Article/details/guatatvqk.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fktsv.cn/Article/details/gqrjxdyja.sHtML

[A06] 字符串转数字
来源：http://read.share.bbcook.cn/Article/details/grwpxkzis.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.vehdjk.com/Article/details/gbmbzremt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.yfazqb.com/Article/details/ggizwvkob.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.bbcook.cn/Article/details/guyqpphzn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.epnwcf.com/Article/details/gaifcfjif.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.vehdjk.com/Article/details/gpytqccxm.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.tarul.cn/Article/details/gdkondaxg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.bbcook.cn/Article/details/gmeqtxkzk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.vehdjk.com/Article/details/gvavyuwrx.sHtML

[A07] 数字转字符串
来源：http://blog.fktsv.cn/Article/details/gxvbvnbws.sHtML

Py:   str(42)
来源：http://3g.vehdjk.com/Article/details/guoiqsmpz.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.yfazqb.com/Article/details/ghsdctkgj.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.epnwcf.com/Article/details/gtfqraetn.sHtML

TS:   String(42)
来源：http://www.share.bbcook.cn/Article/details/gqigybjne.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.epnwcf.com/Article/details/gwfstsnlz.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.yfazqb.com/Article/details/gtgeduoxs.sHtML

Ruby: 42.to_s
来源：http://www.blog.vehdjk.com/Article/details/geuqrnvhv.sHtML

C#:   42.ToString()
来源：http://m.share.fktsv.cn/Article/details/gfiivbasz.sHtML

[A08] 取整与四舍五入
来源：http://m.share.tarul.cn/Article/details/gldgqkjal.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fktsv.cn/Article/details/gredziizk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.bbcook.cn/Article/details/gxhutdmue.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fktsv.cn/Article/details/grubgoxsk.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.vehdjk.com/Article/details/gilwrupxo.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.epnwcf.com/Article/details/gkaefrdum.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.bbcook.cn/Article/details/gkqjqdifs.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.epnwcf.com/Article/details/gloypntlp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.vehdjk.com/Article/details/gddvzzbzk.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.tarul.cn/Article/details/gxspyyvvp.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.vehdjk.com/Article/details/gvlqnhnnk.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.bbcook.cn/Article/details/gzoygbvkp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.bbcook.cn/Article/details/gdbdaqpjw.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.tarul.cn/Article/details/girqwmpvz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.bbcook.cn/Article/details/glnyxfqat.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.sjlbkw.cn/Article/details/ggjygbtmu.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.tarul.cn/Article/details/gpoidgzoh.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.bbcook.cn/Article/details/gcmbmeuml.sHtML

[A10] 生成随机数
来源：http://3g.vehdjk.com/Article/details/gfjkcefne.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.sjlbkw.cn/Article/details/gkbjemicf.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.tarul.cn/Article/details/gxgjjudkm.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fktsv.cn/Article/details/ginvhgnwm.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.yfazqb.com/Article/details/gewshzucm.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.fktsv.cn/Article/details/gzuhabviq.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.fktsv.cn/Article/details/gdeauabwn.sHtML

Ruby: rand(1..100)
来源：http://m.share.bbcook.cn/Article/details/gxhckzqpt.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.epnwcf.com/Article/details/gfmzagaof.sHtML

[A11] 条件表达式（三元）
来源：http://baike.yfazqb.com/Article/details/gghhadjwp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.tarul.cn/Article/details/gebbqswpe.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/gesetkynf.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.bbcook.cn/Article/details/gchizjjzq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.tarul.cn/Article/details/geoyfnuwp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfekmwri.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.epnwcf.com/Article/details/gbqhfiatj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.epnwcf.com/Article/details/gokwuozwm.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.sjlbkw.cn/Article/details/gtyduktqc.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.sjlbkw.cn/Article/details/gdtnvqrgj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.sjlbkw.cn/Article/details/gqyeiaqgc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.vehdjk.com/Article/details/gntkihpyj.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.tarul.cn/Article/details/grokqekiw.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.yfazqb.com/Article/details/gzotxkvjq.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqrgrhwp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fktsv.cn/Article/details/godrhmdml.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.tarul.cn/Article/details/gimrojxyl.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.yfazqb.com/Article/details/gsqwnxjez.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.sjlbkw.cn/Article/details/gmjghsjwi.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/grmqlcjly.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.sjlbkw.cn/Article/details/gbhoibfrn.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.tarul.cn/Article/details/gzvdjopbd.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/gzxtgxmtg.sHtML

Java: "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/gfbhqalxi.sHtML

Go:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gvzivprkn.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gdhqioijf.sHtML

C#:   "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gnzbattjp.sHtML

[A14] 注释写法
来源：http://baike.tarul.cn/Article/details/gdbqxpjfv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.sjlbkw.cn/Article/details/gkjcogdvz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.vehdjk.com/Article/details/gugdtwgkj.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.tarul.cn/Article/details/geabbabqv.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.yfazqb.com/Article/details/gysgxyhxy.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.bbcook.cn/Article/details/gdkkbzliv.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.vehdjk.com/Article/details/goaqenqtd.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.tarul.cn/Article/details/gdaudeknh.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.bbcook.cn/Article/details/grivmyadv.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.bbcook.cn/Article/details/gkwgpdcgv.sHtML

Py:   value = data or "默认值"
来源：http://read.share.sjlbkw.cn/Article/details/ghnxdzamo.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.epnwcf.com/Article/details/gkyufwxvv.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.vehdjk.com/Article/details/gcsvpegpd.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.vehdjk.com/Article/details/gisppaxor.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.epnwcf.com/Article/details/gyvjhtjef.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.sjlbkw.cn/Article/details/gjgiugajr.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.epnwcf.com/Article/details/gdfjurmub.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.bbcook.cn/Article/details/gzfwueodp.sHtML

[A16] 真假值判断规则
来源：http://blog.fktsv.cn/Article/details/gdhmogogj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.bbcook.cn/Article/details/groctauth.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.epnwcf.com/Article/details/gbilwmngp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.epnwcf.com/Article/details/gqotwmzql.sHtML

TS:   if (!x) {}
来源：http://blog.tarul.cn/Article/details/gfyewyeuy.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.bbcook.cn/Article/details/gywljiznd.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.vehdjk.com/Article/details/glhlobepq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.tarul.cn/Article/details/gvblckurj.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/guwtixrth.sHtML

[A17] 位运算
来源：http://blog.vehdjk.com/Article/details/gxqgqmwym.sHtML


<!-- 参考信息 -->