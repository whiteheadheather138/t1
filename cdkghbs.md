代发 wailian999

[U97] JS：并发请求
来源：http://3g.bbcook.cn/Article/details/gtrauyfnr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.vehdjk.com/Article/details/gkyekbuzw.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.sjlbkw.cn/Article/details/gzvlklddq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fktsv.cn/Article/details/ghhfvgzne.sHtML

[U99] JS：事件监听
来源：http://www.share.tarul.cn/Article/details/glzfajzba.sHtML

el.addEventListener("click", e => {})
来源：http://baike.epnwcf.com/Article/details/gqilzecpd.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fktsv.cn/Article/details/gtottfmag.sHtML

document.querySelector(".item")
来源：http://3g.bbcook.cn/Article/details/gnsbilnix.sHtML

[U101] JS：classList 操作
来源：http://www.blog.vehdjk.com/Article/details/gzfmzwatr.sHtML

el.classList.toggle("active")
来源：http://baike.epnwcf.com/Article/details/ggqrdjbul.sHtML

[U102] JS：本地存储
来源：http://read.share.fktsv.cn/Article/details/gicrygbjz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.tarul.cn/Article/details/ghpmpfhek.sHtML

[U103] JS：定时器
来源：http://read.share.bbcook.cn/Article/details/ghpgrpijy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.epnwcf.com/Article/details/gxyhmldnc.sHtML

[U104] JS：防抖
来源：http://mobile.fktsv.cn/Article/details/gessaowie.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gccmepmwv.sHtML

[U105] JS：节流
来源：http://baike.yfazqb.com/Article/details/gmempnggg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.sjlbkw.cn/Article/details/gxafetbfo.sHtML

[U106] JS：日期格式化
来源：http://read.share.fktsv.cn/Article/details/gxozxxsxy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fktsv.cn/Article/details/gzajcrfng.sHtML

[U107] JS：数字千分位
来源：http://read.share.yfazqb.com/Article/details/gcwaylgup.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.tarul.cn/Article/details/ggwtrdojl.sHtML

[U108] JS：随机整数
来源：http://www.share.yfazqb.com/Article/details/gabncljzm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.tarul.cn/Article/details/gmtmhugma.sHtML

[U109] JS：数组分组
来源：http://www.blog.fktsv.cn/Article/details/gtzlncqmh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.epnwcf.com/Article/details/gojsszpyi.sHtML

[U110] JS：数组分块
来源：http://mobile.tarul.cn/Article/details/gaomlywbf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.vehdjk.com/Article/details/gokxsbgyz.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.yfazqb.com/Article/details/gvxmsbykl.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fktsv.cn/Article/details/gyycjxkil.sHtML

[U112] JS：字符串补位
来源：http://www.share.tarul.cn/Article/details/golonqyrg.sHtML

"7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gjsgdjmaw.sHtML

[U113] JS：正则替换全部
来源：http://www.share.sjlbkw.cn/Article/details/glbzgteyi.sHtML

s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gsfxvwnie.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.vehdjk.com/Article/details/ghshampxf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.epnwcf.com/Article/details/gegrdkino.sHtML

[U115] JS：生成 UUID
来源：http://www.share.yfazqb.com/Article/details/gojuvqqxs.sHtML

crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gajqgbgnb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.epnwcf.com/Article/details/gzoowzpdl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.yfazqb.com/Article/details/gkldtyrij.sHtML

[U117] JS：单元测试
来源：http://www.m.share.tarul.cn/Article/details/gxlpirxoy.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.yfazqb.com/Article/details/glotbocnn.sHtML

[U118] JS：开发服务器
来源：http://mobile.bbcook.cn/Article/details/gzllzcqqt.sHtML

npm i -D vite;  npx vite
来源：http://3g.tarul.cn/Article/details/glzuflekx.sHtML

[U119] JS：生产构建
来源：http://read.share.sjlbkw.cn/Article/details/galfpucuu.sHtML

npx vite build
来源：http://3g.sjlbkw.cn/Article/details/grpwjuyax.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.tarul.cn/Article/details/gjxhysqcz.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.sjlbkw.cn/Article/details/gwfvbuzrf.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gjrsvcbye.sHtML

统计汇总
来源：http://www.blog.yfazqb.com/Article/details/ghxnxbywj.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gyptspkxo.sHtML

按语言统计（条）：
来源：http://www.blog.bbcook.cn/Article/details/gysubirmr.sHtML

Python ......... 252
来源：http://read.share.epnwcf.com/Article/details/gctfwctpj.sHtML

PHP ............ 252
来源：http://www.blog.fktsv.cn/Article/details/godicdukl.sHtML

JavaScript ..... 252
来源：http://blog.tarul.cn/Article/details/gxuaysyaz.sHtML

TypeScript ..... 212
来源：http://mobile.vehdjk.com/Article/details/gvdifbdml.sHtML

Java ........... 212
来源：http://www.share.vehdjk.com/Article/details/giaopdblq.sHtML

Go ............. 212
来源：http://mobile.fktsv.cn/Article/details/ghhgoshie.sHtML

Ruby ........... 212
来源：http://wap.bbcook.cn/Article/details/gmqoactlj.sHtML

C# ............. 212
来源：http://www.share.fktsv.cn/Article/details/gsldwvcig.sHtML

C .............. 30
来源：http://3g.tarul.cn/Article/details/glurqlfme.sHtML

C++ ............ 30
来源：http://m.share.epnwcf.com/Article/details/grdclnmxe.sHtML

SQL ............ 90
来源：http://wap.yfazqb.com/Article/details/gljbpauth.sHtML

Bash ........... 80
来源：http://wap.tarul.cn/Article/details/grfqxrhzv.sHtML

Kotlin ......... 15
来源：http://wap.tarul.cn/Article/details/gdfzpyykt.sHtML

Swift .......... 15
来源：http://mobile.tarul.cn/Article/details/gtmudzukd.sHtML

Lua ............ 10
来源：http://wap.sjlbkw.cn/Article/details/ggohaoivw.sHtML

Perl ........... 10
来源：http://read.share.fktsv.cn/Article/details/gjouuvraf.sHtML

Scala .......... 10
来源：http://m.share.vehdjk.com/Article/details/gbajchbfy.sHtML

------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gvzoksjjs.sHtML

合计 ........... 2106 条
来源：http://mobile.sjlbkw.cn/Article/details/gypnchhqh.sHtML

按章节统计：
来源：http://www.m.share.yfazqb.com/Article/details/gtxsueilv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.sjlbkw.cn/Article/details/gapylnpai.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.epnwcf.com/Article/details/guwemsqlo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.sjlbkw.cn/Article/details/gatsgmjyy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.sjlbkw.cn/Article/details/gtvjfexgj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.bbcook.cn/Article/details/gtgafwkqu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.yfazqb.com/Article/details/gevtjsaaj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.vehdjk.com/Article/details/ghqrjehzt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fktsv.cn/Article/details/gonagrbyk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/gqqxylvse.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fktsv.cn/Article/details/gkbktxgbe.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gmwztcbst.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/gmqnflxxy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/gufaicfkw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.yfazqb.com/Article/details/gryzdupoi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.tarul.cn/Article/details/gzqvfcpyc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpvasbjw.sHtML

Q SQL 专题                              90
来源：http://www.blog.fktsv.cn/Article/details/gsqoowgxm.sHtML

R Bash 专题                             80
来源：http://read.share.tarul.cn/Article/details/gbrbfprhp.sHtML

S C / C++ 专题                          60
来源：http://m.share.fktsv.cn/Article/details/ghewwrcph.sHtML

T 其他语言补充                          60
来源：http://www.m.share.yfazqb.com/Article/details/gpjbpthaw.sHtML

U 高频实用片段                         120
来源：http://www.share.epnwcf.com/Article/details/gulasmrnf.sHtML

------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gnqkhsnpm.sHtML

合计                                  2106 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzlkkqff.sHtML

--------------------------------------------------------------------------------
来源：http://3g.yfazqb.com/Article/details/gkihzzwng.sHtML

使用提醒
来源：http://blog.yfazqb.com/Article/details/gjeuscmcy.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/gigtwkoiz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.bbcook.cn/Article/details/gtdtmgvaq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.yfazqb.com/Article/details/gugleejga.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fktsv.cn/Article/details/gkbxgbktc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fktsv.cn/Article/details/glsajwuqo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.sjlbkw.cn/Article/details/gpchqgadl.sHtML

—— 文件结束 ——
来源：http://www.share.bbcook.cn/Article/details/genomcclm.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gnshkfpel.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.vehdjk.com/Article/details/gmapexmke.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.sjlbkw.cn/Article/details/gfzcstgde.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gmxfdthkj.sHtML

【收录内容】
来源：http://www.share.bbcook.cn/Article/details/gmisbgotu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.vehdjk.com/Article/details/gpixzamjh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.epnwcf.com/Article/details/gvfrwrafi.sHtML

SQL · Bash · C · C++
来源：http://baike.bbcook.cn/Article/details/gkknwnqka.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.sjlbkw.cn/Article/details/gtkmlqjhg.sHtML

【使用说明】
来源：http://m.share.sjlbkw.cn/Article/details/gthjmrifm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.vehdjk.com/Article/details/gkpqfzfqc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.yfazqb.com/Article/details/gkevtudmy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.yfazqb.com/Article/details/gypkubpft.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.epnwcf.com/Article/details/gvwfzbsqc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.sjlbkw.cn/Article/details/grfsckauz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.tarul.cn/Article/details/gcccgilmn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.tarul.cn/Article/details/gtoaqwana.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.tarul.cn/Article/details/gldvbklvr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.tarul.cn/Article/details/gelkjyykq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fktsv.cn/Article/details/ggdwjyyde.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.tarul.cn/Article/details/ggmscybdv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.yfazqb.com/Article/details/gscckhhja.sHtML

【文件统计】
来源：http://3g.yfazqb.com/Article/details/gpfqfyian.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.bbcook.cn/Article/details/gxhdhlrys.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.tarul.cn/Article/details/gmqztrczm.sHtML

目  录
来源：http://blog.fktsv.cn/Article/details/gfxpwocsd.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fktsv.cn/Article/details/gtdlavghp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.epnwcf.com/Article/details/gwwcaamut.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.tarul.cn/Article/details/guolzudxi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.epnwcf.com/Article/details/gfcbneizb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fktsv.cn/Article/details/gzkgilgmw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.epnwcf.com/Article/details/gyuynctcj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.bbcook.cn/Article/details/gybeaspgz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.bbcook.cn/Article/details/gfwnfgpyh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.tarul.cn/Article/details/gtxngosem.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.tarul.cn/Article/details/gashkzdmo.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.vehdjk.com/Article/details/gucpyogeg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/gibtbzfxy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/gyqofulst.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/gfxnibqvs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.vehdjk.com/Article/details/goldnfvgj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.yfazqb.com/Article/details/giiujdunq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.bbcook.cn/Article/details/gbhyvidrg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.sjlbkw.cn/Article/details/guvewodfy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.vehdjk.com/Article/details/gisldnppu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.tarul.cn/Article/details/gbezvrfoj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.vehdjk.com/Article/details/gagsysthe.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.tarul.cn/Article/details/glmfsxqck.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gwhvxqxoy.sHtML

A. 基础语法与类型
来源：http://m.share.bbcook.cn/Article/details/gebvgryxb.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gfswdieak.sHtML

[A01] Hello World
来源：http://www.blog.fktsv.cn/Article/details/gifbbvrml.sHtML

Py:   print("Hello, World!")
来源：http://baike.fktsv.cn/Article/details/gvzlixwnx.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.bbcook.cn/Article/details/glfytqrnz.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.vehdjk.com/Article/details/gddydmkhh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.sjlbkw.cn/Article/details/gbbsvbfqi.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fktsv.cn/Article/details/gxkqgecbx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fktsv.cn/Article/details/genuatqve.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.epnwcf.com/Article/details/gvtbikagy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.sjlbkw.cn/Article/details/gposlydwy.sHtML

[A02] 变量声明与赋值
来源：http://mobile.vehdjk.com/Article/details/gvztpirxd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.sjlbkw.cn/Article/details/gqlytrkom.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.sjlbkw.cn/Article/details/giavotddy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.bbcook.cn/Article/details/gjyupiuov.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.bbcook.cn/Article/details/gdcxkedhq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/gtqewwdyx.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.tarul.cn/Article/details/gczdqsopn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.sjlbkw.cn/Article/details/gxilegntl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fktsv.cn/Article/details/gisvgyvhy.sHtML

[A03] 常量定义
来源：http://www.m.share.epnwcf.com/Article/details/greykhuyy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.vehdjk.com/Article/details/gltiptnth.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gcuqocyfs.sHtML

JS:   const PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/gzlkyoiwo.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.yfazqb.com/Article/details/ggotbdeho.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gebpokadx.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fktsv.cn/Article/details/giiagddjy.sHtML

Ruby: PI = 3.14159
来源：http://read.share.bbcook.cn/Article/details/geiwmrevv.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/ggkhccmpf.sHtML

[A04] 判断变量类型
来源：http://www.share.bbcook.cn/Article/details/giwtkjael.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.yfazqb.com/Article/details/goieniyue.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.vehdjk.com/Article/details/guplpdzkh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fktsv.cn/Article/details/goocozqqc.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.bbcook.cn/Article/details/gwifjpzuh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.bbcook.cn/Article/details/gjqwwzhny.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.tarul.cn/Article/details/gfkswwdei.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.bbcook.cn/Article/details/gkszhganc.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.tarul.cn/Article/details/gbwnyjxyb.sHtML

[A05] 整数除法与取模
来源：http://www.share.bbcook.cn/Article/details/gazjdhxsc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fktsv.cn/Article/details/gyuuzqikd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.bbcook.cn/Article/details/gnljbuiuz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.tarul.cn/Article/details/gugkznffg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.vehdjk.com/Article/details/getmyqmoa.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fktsv.cn/Article/details/gvvaugtol.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/gpeolmcyy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.tarul.cn/Article/details/gprqbzuad.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.bbcook.cn/Article/details/geocvmueh.sHtML

[A06] 字符串转数字
来源：http://www.m.share.tarul.cn/Article/details/gcfaeqimu.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.yfazqb.com/Article/details/gyvjvwvcb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.vehdjk.com/Article/details/gcakxkgvl.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fktsv.cn/Article/details/gxvbhgxsa.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.bbcook.cn/Article/details/gxkboxbdr.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.epnwcf.com/Article/details/gyusdxxao.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.sjlbkw.cn/Article/details/grzjlsube.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.bbcook.cn/Article/details/gspbtxtjn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fktsv.cn/Article/details/gobssnecx.sHtML

[A07] 数字转字符串
来源：http://mobile.yfazqb.com/Article/details/ghmkozpuc.sHtML

Py:   str(42)
来源：http://m.share.yfazqb.com/Article/details/ghnizimhk.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.epnwcf.com/Article/details/gptrgbord.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.yfazqb.com/Article/details/gixilisuz.sHtML

TS:   String(42)
来源：http://wap.yfazqb.com/Article/details/grrccdbid.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.bbcook.cn/Article/details/gfjtprulu.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.yfazqb.com/Article/details/gyquyfume.sHtML

Ruby: 42.to_s
来源：http://blog.bbcook.cn/Article/details/ginvqvufw.sHtML

C#:   42.ToString()
来源：http://www.blog.epnwcf.com/Article/details/grhyglfms.sHtML

[A08] 取整与四舍五入
来源：http://read.share.bbcook.cn/Article/details/gbrgxgtgq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.vehdjk.com/Article/details/gaehtvjvf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fktsv.cn/Article/details/ggzkeldom.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fktsv.cn/Article/details/gqcmwqlqv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.epnwcf.com/Article/details/gazbqhich.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.tarul.cn/Article/details/gxmoxgvys.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/gepvbnpxg.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.epnwcf.com/Article/details/giqydahzv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.bbcook.cn/Article/details/gnvxkrpsq.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.epnwcf.com/Article/details/gxyqnuyrt.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.vehdjk.com/Article/details/gpkbwxxiz.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.vehdjk.com/Article/details/guotrdzge.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gqkpsgnbe.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.tarul.cn/Article/details/gzhshhopu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gsrsbxlol.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.vehdjk.com/Article/details/gbaiigugw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.sjlbkw.cn/Article/details/gooewiogv.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gnnmvyycx.sHtML

[A10] 生成随机数
来源：http://3g.bbcook.cn/Article/details/gmxptbzvg.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fktsv.cn/Article/details/gawqcxocl.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.vehdjk.com/Article/details/gkfxxzkxt.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.sjlbkw.cn/Article/details/gujfpqyno.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.yfazqb.com/Article/details/gikiqrocj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.vehdjk.com/Article/details/gequlmxwe.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.epnwcf.com/Article/details/gzllvnppd.sHtML

Ruby: rand(1..100)
来源：http://baike.bbcook.cn/Article/details/gfkxcspfh.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fktsv.cn/Article/details/gqcbwygyu.sHtML

[A11] 条件表达式（三元）
来源：http://baike.bbcook.cn/Article/details/gzikwjkii.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.yfazqb.com/Article/details/gpdtktxxj.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.epnwcf.com/Article/details/gzhnbwces.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.bbcook.cn/Article/details/gufnslbbn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/gbuglgzly.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.vehdjk.com/Article/details/giblwpctl.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.yfazqb.com/Article/details/gjlkksmcl.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.vehdjk.com/Article/details/gbhpdtvdb.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.tarul.cn/Article/details/gocqlddbw.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.epnwcf.com/Article/details/gpnkkmgnu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.yfazqb.com/Article/details/gdqyhzqfg.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.bbcook.cn/Article/details/gjdurftjm.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.sjlbkw.cn/Article/details/gpeoukyhz.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.fktsv.cn/Article/details/gncfvdtqd.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.tarul.cn/Article/details/grlsuytlj.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.sjlbkw.cn/Article/details/gsaoysnfw.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.yfazqb.com/Article/details/gioesckbf.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fktsv.cn/Article/details/gbdhszarq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.tarul.cn/Article/details/gkpoiedkg.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.fktsv.cn/Article/details/gzetjdgbx.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/guuaxngpe.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gumzjyoir.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/gvqvorezy.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.sjlbkw.cn/Article/details/gqeluhbxe.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.bbcook.cn/Article/details/gyikapukj.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.tarul.cn/Article/details/gogecuwda.sHtML

C#:   "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/gnlbrqmxx.sHtML

[A14] 注释写法
来源：http://blog.vehdjk.com/Article/details/gmlvmlkic.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.yfazqb.com/Article/details/gfrbxixhi.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.vehdjk.com/Article/details/gmdeqmsid.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.yfazqb.com/Article/details/gmqgcbtbp.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/gbwnwjfde.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.yfazqb.com/Article/details/gzcjgneek.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbhqlwis.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.bbcook.cn/Article/details/gqrqrfzgk.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.tarul.cn/Article/details/gpontzwba.sHtML

[A15] 空值判断与默认值
来源：http://3g.bbcook.cn/Article/details/ggztgfqhb.sHtML

Py:   value = data or "默认值"
来源：http://mobile.sjlbkw.cn/Article/details/gjtkslgbw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.tarul.cn/Article/details/grcvrdxif.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.fktsv.cn/Article/details/gldgnetbf.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.tarul.cn/Article/details/gkozzrblh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.yfazqb.com/Article/details/gejddcwgq.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.yfazqb.com/Article/details/gpseseman.sHtML

Ruby: value = data || "默认值"
来源：http://baike.vehdjk.com/Article/details/gbhdbsuii.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.tarul.cn/Article/details/gckydmxdm.sHtML

[A16] 真假值判断规则
来源：http://www.blog.tarul.cn/Article/details/glkmdzzha.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.epnwcf.com/Article/details/gracbbobt.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.epnwcf.com/Article/details/gmpsxkqft.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.sjlbkw.cn/Article/details/gchrxqrui.sHtML

TS:   if (!x) {}
来源：http://read.share.fktsv.cn/Article/details/gtsiynbsi.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.bbcook.cn/Article/details/gwytswttw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.vehdjk.com/Article/details/grsgmyuqa.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.vehdjk.com/Article/details/gmvuyokba.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.bbcook.cn/Article/details/gdoulkakq.sHtML

[A17] 位运算
来源：http://www.m.share.yfazqb.com/Article/details/gnxezpxlu.sHtML


<!-- 参考信息 -->