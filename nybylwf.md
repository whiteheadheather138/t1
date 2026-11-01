代发 wailian999

[U97] JS：并发请求
来源：http://www.m.share.yfazqb.com/Article/details/guzwwyxqn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gcbscnmeg.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.sjlbkw.cn/Article/details/goebouuzr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.epnwcf.com/Article/details/gfflmtryz.sHtML

[U99] JS：事件监听
来源：http://wap.sjlbkw.cn/Article/details/gxqlcxkpl.sHtML

el.addEventListener("click", e => {})
来源：http://baike.vehdjk.com/Article/details/golwzhcty.sHtML

[U100] JS：DOM 查询
来源：http://baike.vehdjk.com/Article/details/gkfwnsjmf.sHtML

document.querySelector(".item")
来源：http://mobile.vehdjk.com/Article/details/gbxzpsbqe.sHtML

[U101] JS：classList 操作
来源：http://m.share.bbcook.cn/Article/details/gtudzllfx.sHtML

el.classList.toggle("active")
来源：http://www.blog.yfazqb.com/Article/details/gtswyqeub.sHtML

[U102] JS：本地存储
来源：http://3g.bbcook.cn/Article/details/gkfbtnkhg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.epnwcf.com/Article/details/ghafqazpe.sHtML

[U103] JS：定时器
来源：http://wap.yfazqb.com/Article/details/glhyuvzwc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.vehdjk.com/Article/details/gfnmeoanv.sHtML

[U104] JS：防抖
来源：http://www.blog.bbcook.cn/Article/details/gzhwamvuy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/ggszuyfzu.sHtML

[U105] JS：节流
来源：http://baike.epnwcf.com/Article/details/glagkgrue.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.tarul.cn/Article/details/gbyrgsdom.sHtML

[U106] JS：日期格式化
来源：http://baike.bbcook.cn/Article/details/gzhpktdbn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fktsv.cn/Article/details/gijykexwf.sHtML

[U107] JS：数字千分位
来源：http://baike.vehdjk.com/Article/details/gnahbeqpg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.bbcook.cn/Article/details/gxavaddfk.sHtML

[U108] JS：随机整数
来源：http://read.share.epnwcf.com/Article/details/gexblujdd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.yfazqb.com/Article/details/gqtoeorxv.sHtML

[U109] JS：数组分组
来源：http://www.share.tarul.cn/Article/details/gqfuneedy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fktsv.cn/Article/details/gzzqclodn.sHtML

[U110] JS：数组分块
来源：http://read.share.epnwcf.com/Article/details/gglpibeib.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.sjlbkw.cn/Article/details/gjqqhoamu.sHtML

[U111] JS：对象转 Map
来源：http://wap.vehdjk.com/Article/details/geshewzfu.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fktsv.cn/Article/details/glshmhtxd.sHtML

[U112] JS：字符串补位
来源：http://m.share.yfazqb.com/Article/details/glxoxdmpv.sHtML

"7".padStart(3, "0")
来源：http://3g.fktsv.cn/Article/details/grdetohms.sHtML

[U113] JS：正则替换全部
来源：http://wap.epnwcf.com/Article/details/gcfikbtnk.sHtML

s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gtjkxwnes.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.bbcook.cn/Article/details/glwpgjfna.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.vehdjk.com/Article/details/gyodqtumd.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/ghznjkpre.sHtML

crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/gsplxbrup.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.epnwcf.com/Article/details/gpajddfut.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.bbcook.cn/Article/details/gqogoxwbg.sHtML

[U117] JS：单元测试
来源：http://www.blog.tarul.cn/Article/details/gfjpchabq.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.tarul.cn/Article/details/gdpdiicoq.sHtML

[U118] JS：开发服务器
来源：http://blog.epnwcf.com/Article/details/gqrxbxwoq.sHtML

npm i -D vite;  npx vite
来源：http://3g.bbcook.cn/Article/details/gavkprfke.sHtML

[U119] JS：生产构建
来源：http://www.m.share.bbcook.cn/Article/details/gbhufaucr.sHtML

npx vite build
来源：http://baike.sjlbkw.cn/Article/details/gljoaspkg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fktsv.cn/Article/details/gechzfdxo.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.sjlbkw.cn/Article/details/gvhskzxmt.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gurncbdrn.sHtML

统计汇总
来源：http://3g.fktsv.cn/Article/details/glnehdfem.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gnlnemjci.sHtML

按语言统计（条）：
来源：http://mobile.sjlbkw.cn/Article/details/gijfegqpn.sHtML

Python ......... 252
来源：http://www.share.bbcook.cn/Article/details/grmsfxizu.sHtML

PHP ............ 252
来源：http://m.share.yfazqb.com/Article/details/gyplrmgla.sHtML

JavaScript ..... 252
来源：http://wap.vehdjk.com/Article/details/gweddkgcb.sHtML

TypeScript ..... 212
来源：http://www.share.fktsv.cn/Article/details/gexkcgxrd.sHtML

Java ........... 212
来源：http://wap.sjlbkw.cn/Article/details/gwdgmxxoy.sHtML

Go ............. 212
来源：http://3g.yfazqb.com/Article/details/glmcvymdm.sHtML

Ruby ........... 212
来源：http://3g.tarul.cn/Article/details/gjqgbnvpl.sHtML

C# ............. 212
来源：http://mobile.epnwcf.com/Article/details/gazubckly.sHtML

C .............. 30
来源：http://3g.vehdjk.com/Article/details/gheonztmm.sHtML

C++ ............ 30
来源：http://3g.vehdjk.com/Article/details/gvumyeshl.sHtML

SQL ............ 90
来源：http://www.share.sjlbkw.cn/Article/details/gaxaphjzr.sHtML

Bash ........... 80
来源：http://www.m.share.vehdjk.com/Article/details/gjcfpngci.sHtML

Kotlin ......... 15
来源：http://m.share.yfazqb.com/Article/details/gfdmavfok.sHtML

Swift .......... 15
来源：http://wap.fktsv.cn/Article/details/ghpqmjcei.sHtML

Lua ............ 10
来源：http://www.share.tarul.cn/Article/details/gxpjwxcsb.sHtML

Perl ........... 10
来源：http://read.share.bbcook.cn/Article/details/gxzjdkhik.sHtML

Scala .......... 10
来源：http://baike.yfazqb.com/Article/details/gkwbjyjkc.sHtML

------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gjgkzwvbu.sHtML

合计 ........... 2106 条
来源：http://www.share.sjlbkw.cn/Article/details/gyxrecywd.sHtML

按章节统计：
来源：http://wap.yfazqb.com/Article/details/gvfjloryj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.vehdjk.com/Article/details/gnnalafug.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.epnwcf.com/Article/details/goxvhwrmo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.sjlbkw.cn/Article/details/gcugrmfqa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.tarul.cn/Article/details/ggavcvilc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.yfazqb.com/Article/details/guukjqoxc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.sjlbkw.cn/Article/details/gtuhswdng.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.tarul.cn/Article/details/gcpkonrts.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.bbcook.cn/Article/details/gitpbzatn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/glcjzzkcp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.tarul.cn/Article/details/giofxuvsj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/gjmjdkkkj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gmvyssqto.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/glmeydrpf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fktsv.cn/Article/details/ggejuwjna.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.sjlbkw.cn/Article/details/gvnmatxsx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/goljkftat.sHtML

Q SQL 专题                              90
来源：http://blog.epnwcf.com/Article/details/gokxfungh.sHtML

R Bash 专题                             80
来源：http://www.blog.tarul.cn/Article/details/gtgfcexox.sHtML

S C / C++ 专题                          60
来源：http://mobile.fktsv.cn/Article/details/griqdfpod.sHtML

T 其他语言补充                          60
来源：http://wap.sjlbkw.cn/Article/details/gvtkrjwyi.sHtML

U 高频实用片段                         120
来源：http://mobile.bbcook.cn/Article/details/gcibueity.sHtML

------------------------------------
来源：http://wap.yfazqb.com/Article/details/gbngfszlc.sHtML

合计                                  2106 条
来源：http://mobile.fktsv.cn/Article/details/grngoomva.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.tarul.cn/Article/details/gmpukildq.sHtML

使用提醒
来源：http://m.share.tarul.cn/Article/details/gtdpefems.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gynvwxuwe.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.vehdjk.com/Article/details/gbtcnjgii.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.epnwcf.com/Article/details/gdxaxacil.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.epnwcf.com/Article/details/gmnfcoehy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.epnwcf.com/Article/details/gmcmjxzyh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.epnwcf.com/Article/details/gxxntuctl.sHtML

—— 文件结束 ——
来源：http://mobile.tarul.cn/Article/details/goczskqyv.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gahavrsyo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.tarul.cn/Article/details/gznkfoeap.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.epnwcf.com/Article/details/gkvdhwtqe.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ggxdbmybo.sHtML

【收录内容】
来源：http://www.share.epnwcf.com/Article/details/gntvvdyrm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.yfazqb.com/Article/details/gziqrkyrn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.vehdjk.com/Article/details/glnoqxgea.sHtML

SQL · Bash · C · C++
来源：http://baike.fktsv.cn/Article/details/gkpecwslh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.tarul.cn/Article/details/gfkcqucoq.sHtML

【使用说明】
来源：http://baike.sjlbkw.cn/Article/details/gsziijmhc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.vehdjk.com/Article/details/gczwbrgex.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.epnwcf.com/Article/details/gdfbbslyc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.tarul.cn/Article/details/golnjspxy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.yfazqb.com/Article/details/gooxnmckw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.yfazqb.com/Article/details/gsyvxsyqm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.sjlbkw.cn/Article/details/ggbmigmky.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.epnwcf.com/Article/details/gnnhlsujd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.sjlbkw.cn/Article/details/guxnhoowd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.epnwcf.com/Article/details/grsqqovjs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fktsv.cn/Article/details/gwmpfuere.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.vehdjk.com/Article/details/gfyfulrgg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fktsv.cn/Article/details/gusnlviun.sHtML

【文件统计】
来源：http://m.share.bbcook.cn/Article/details/gxbxkmbyc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fktsv.cn/Article/details/gnkfrylmp.sHtML

--------------------------------------------------------------------------------
来源：http://baike.tarul.cn/Article/details/gacdmgpeg.sHtML

目  录
来源：http://3g.fktsv.cn/Article/details/gkmrrytmt.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/ggezneudz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.yfazqb.com/Article/details/gillaksgb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.sjlbkw.cn/Article/details/gxhdkbtfo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxzvwzjh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.epnwcf.com/Article/details/gckevntyy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.epnwcf.com/Article/details/gpfjmeyzt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.bbcook.cn/Article/details/guiteyimb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/gznblyqhv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.yfazqb.com/Article/details/grkwkgfot.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.bbcook.cn/Article/details/gsswkvnnm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fktsv.cn/Article/details/gsjdaulte.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.vehdjk.com/Article/details/gnefzxdds.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.sjlbkw.cn/Article/details/gnlimqujz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/gaqrvbmdp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.yfazqb.com/Article/details/gsxfumuax.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtugbcuz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.vehdjk.com/Article/details/gkicvnayb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.vehdjk.com/Article/details/gggffujtd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnilukgi.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.bbcook.cn/Article/details/ggahxjtrh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmrhkqir.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.sjlbkw.cn/Article/details/glarpvsmf.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gjfsabyak.sHtML

A. 基础语法与类型
来源：http://read.share.sjlbkw.cn/Article/details/gflzbmdca.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gauhyqavi.sHtML

[A01] Hello World
来源：http://m.share.sjlbkw.cn/Article/details/glzavtbcm.sHtML

Py:   print("Hello, World!")
来源：http://wap.yfazqb.com/Article/details/gfciaybfg.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.sjlbkw.cn/Article/details/ggfplksbx.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.sjlbkw.cn/Article/details/glvdhxbcz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.sjlbkw.cn/Article/details/gjqpbqjcn.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.tarul.cn/Article/details/geifdgfzr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.sjlbkw.cn/Article/details/gbxgmjacc.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.sjlbkw.cn/Article/details/gltwyhcmo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.sjlbkw.cn/Article/details/griowertr.sHtML

[A02] 变量声明与赋值
来源：http://m.share.yfazqb.com/Article/details/gkzwxfsjc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.bbcook.cn/Article/details/gbdddiyjm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.epnwcf.com/Article/details/gfghggypb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.epnwcf.com/Article/details/gzxxujxiy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.epnwcf.com/Article/details/gtejciojs.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fktsv.cn/Article/details/ginkthqdt.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.vehdjk.com/Article/details/gklsmwdky.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.bbcook.cn/Article/details/girwfgeup.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.yfazqb.com/Article/details/gxxtwlnwi.sHtML

[A03] 常量定义
来源：http://www.blog.tarul.cn/Article/details/gwutbwomo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fktsv.cn/Article/details/gzuzaqqyh.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gmztkxxez.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gozgvpoml.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gmcqbqtkg.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gpryaovsr.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.epnwcf.com/Article/details/gvztdcawx.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.sjlbkw.cn/Article/details/gleelljfg.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gnxyviewr.sHtML

[A04] 判断变量类型
来源：http://m.share.tarul.cn/Article/details/gheadbkpb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.bbcook.cn/Article/details/gxtkydksh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.epnwcf.com/Article/details/gffjsuist.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.epnwcf.com/Article/details/ganvdweip.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.sjlbkw.cn/Article/details/gzyzogtup.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.vehdjk.com/Article/details/gpsdntzru.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.sjlbkw.cn/Article/details/gkbrljvpp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.epnwcf.com/Article/details/gxdvoencb.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.sjlbkw.cn/Article/details/ggeestwbe.sHtML

[A05] 整数除法与取模
来源：http://www.share.bbcook.cn/Article/details/gtqieuzoc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.vehdjk.com/Article/details/gnvojcmyu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fktsv.cn/Article/details/gszehwzdg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.sjlbkw.cn/Article/details/gwolwcxin.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.bbcook.cn/Article/details/gbdhzwrhj.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fktsv.cn/Article/details/gbnuetvxe.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.tarul.cn/Article/details/glaxvmbuk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fktsv.cn/Article/details/gocanukff.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.tarul.cn/Article/details/gtmfdhknm.sHtML

[A06] 字符串转数字
来源：http://read.share.tarul.cn/Article/details/gvyhqpeij.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.vehdjk.com/Article/details/gihscpekc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.sjlbkw.cn/Article/details/gkxtixtpl.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.sjlbkw.cn/Article/details/gwpieehdc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.epnwcf.com/Article/details/ghadojgmp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.yfazqb.com/Article/details/gcqqtzqol.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.tarul.cn/Article/details/gthroqvjt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.vehdjk.com/Article/details/gnlfzlqfp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.bbcook.cn/Article/details/gvximmhgp.sHtML

[A07] 数字转字符串
来源：http://read.share.epnwcf.com/Article/details/gtorrzxuq.sHtML

Py:   str(42)
来源：http://www.share.bbcook.cn/Article/details/gqqspcpwz.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.yfazqb.com/Article/details/gijjvotyp.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.yfazqb.com/Article/details/gdwjghjbh.sHtML

TS:   String(42)
来源：http://mobile.vehdjk.com/Article/details/gcdrltmax.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.sjlbkw.cn/Article/details/gnvcygmny.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.fktsv.cn/Article/details/gqahyteft.sHtML

Ruby: 42.to_s
来源：http://www.m.share.yfazqb.com/Article/details/gbdskchxu.sHtML

C#:   42.ToString()
来源：http://3g.sjlbkw.cn/Article/details/gxkgxuoqk.sHtML

[A08] 取整与四舍五入
来源：http://m.share.yfazqb.com/Article/details/gzzzppknl.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.tarul.cn/Article/details/gswtqujlx.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fktsv.cn/Article/details/gtnsqouzj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.sjlbkw.cn/Article/details/gfvwkyhbz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.sjlbkw.cn/Article/details/gpnswzznl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.sjlbkw.cn/Article/details/ggwuyqpra.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.bbcook.cn/Article/details/glkupvopg.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.sjlbkw.cn/Article/details/gcqemtloh.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.tarul.cn/Article/details/gdtirqhhr.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.yfazqb.com/Article/details/gmejkbhma.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.tarul.cn/Article/details/glhzldjzt.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/gsxedxauo.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.epnwcf.com/Article/details/gibzytqgn.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.vehdjk.com/Article/details/gljvkkrpe.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.bbcook.cn/Article/details/gbcjkxmvk.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.tarul.cn/Article/details/gbjawapta.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.bbcook.cn/Article/details/gxxzbycpd.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/gdddpxcdk.sHtML

[A10] 生成随机数
来源：http://read.share.epnwcf.com/Article/details/gdhctqhiw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fktsv.cn/Article/details/gruauxbqg.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.epnwcf.com/Article/details/gqicefflq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.vehdjk.com/Article/details/giheefllw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.tarul.cn/Article/details/gwrkozfmr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fktsv.cn/Article/details/gygpjojxx.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.yfazqb.com/Article/details/gmltfzyog.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.vehdjk.com/Article/details/gfuvjnjnj.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.epnwcf.com/Article/details/ggxtayqfs.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fktsv.cn/Article/details/gpzlzqvfi.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.tarul.cn/Article/details/gbdhgbwqh.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.bbcook.cn/Article/details/gfxstuipn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.sjlbkw.cn/Article/details/gzmxkyeud.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.fktsv.cn/Article/details/gmrywbesu.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.yfazqb.com/Article/details/gdtrxgeos.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.sjlbkw.cn/Article/details/gyqvptxtw.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.tarul.cn/Article/details/ggsorbsde.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.yfazqb.com/Article/details/gskpvfmps.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.vehdjk.com/Article/details/gmporvgsj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.epnwcf.com/Article/details/gqdckpeil.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.tarul.cn/Article/details/gzkipoewi.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.tarul.cn/Article/details/gmmqsegls.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.bbcook.cn/Article/details/gbnrprcvx.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.yfazqb.com/Article/details/gmtujftzl.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.vehdjk.com/Article/details/gvkeytukh.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcrdeorv.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.bbcook.cn/Article/details/gerdxqtvo.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.vehdjk.com/Article/details/gvzkuzvaz.sHtML

Py:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/glacngyjb.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gkbgfupph.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.epnwcf.com/Article/details/ghdqaxxnd.sHtML

TS:   "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/gohaybkat.sHtML

Java: "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/glnylndek.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gygmtentj.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gpnfkivjm.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.bbcook.cn/Article/details/gudhbjdru.sHtML

[A14] 注释写法
来源：http://3g.tarul.cn/Article/details/gdnvcrbrk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.yfazqb.com/Article/details/gddrksngz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.epnwcf.com/Article/details/glvljkroz.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.sjlbkw.cn/Article/details/gedqvvhjt.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.tarul.cn/Article/details/ghnxlynlc.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.yfazqb.com/Article/details/gjkgohppg.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.vehdjk.com/Article/details/gxcwqvwcd.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.sjlbkw.cn/Article/details/gzhdwnluq.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fktsv.cn/Article/details/ghgwigpgb.sHtML

[A15] 空值判断与默认值
来源：http://read.share.bbcook.cn/Article/details/gepcalnqx.sHtML

Py:   value = data or "默认值"
来源：http://3g.sjlbkw.cn/Article/details/gucgkcjwh.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.bbcook.cn/Article/details/gkyqwzfoe.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.tarul.cn/Article/details/gbfbyfacw.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.fktsv.cn/Article/details/gaxmnsvwp.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.sjlbkw.cn/Article/details/gqvyyrhga.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fktsv.cn/Article/details/gsrtgmkik.sHtML

Ruby: value = data || "默认值"
来源：http://3g.yfazqb.com/Article/details/gncbwijee.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.vehdjk.com/Article/details/gayopjsay.sHtML

[A16] 真假值判断规则
来源：http://3g.sjlbkw.cn/Article/details/gtcehmwhw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.vehdjk.com/Article/details/gxiuzfxiv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.yfazqb.com/Article/details/gamdirxiy.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.sjlbkw.cn/Article/details/gvghgcsqn.sHtML

TS:   if (!x) {}
来源：http://www.m.share.fktsv.cn/Article/details/gaplxkqux.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.yfazqb.com/Article/details/gjhxtbzzd.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.bbcook.cn/Article/details/goaqgcszt.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.bbcook.cn/Article/details/ginoelgho.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.tarul.cn/Article/details/gxjdjunev.sHtML

[A17] 位运算
来源：http://m.share.sjlbkw.cn/Article/details/gjvkdvhym.sHtML


<!-- 参考信息 -->