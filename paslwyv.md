代发 wailian999

[U89] JS：数组去重
来源：http://mobile.bbcook.cn/Article/details/gtuuhwqtx.sHtML

[...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/gjtqakcas.sHtML

[U90] JS：数字数组排序
来源：http://mobile.yfazqb.com/Article/details/glurucrrv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/gmhryaght.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.sjlbkw.cn/Article/details/gsgucbtvd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.vehdjk.com/Article/details/gxzqzrtec.sHtML

[U92] JS：深拷贝
来源：http://read.share.epnwcf.com/Article/details/gditqznpu.sHtML

structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gniiyzafr.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.vehdjk.com/Article/details/gfpsdnwfh.sHtML

`共 ${n} 条`
来源：http://m.share.vehdjk.com/Article/details/gsvejutmz.sHtML

[U94] JS：箭头函数
来源：http://baike.epnwcf.com/Article/details/gmdsnedzn.sHtML

const double = x => x * 2;
来源：http://www.share.sjlbkw.cn/Article/details/gjxxfathe.sHtML

[U95] JS：Promise 包装
来源：http://mobile.bbcook.cn/Article/details/guqrrvggh.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.vehdjk.com/Article/details/gkfbkjsmg.sHtML

[U96] JS：async/await 与异常
来源：http://blog.sjlbkw.cn/Article/details/gyritgrje.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gjirxnjxk.sHtML

[U97] JS：并发请求
来源：http://baike.tarul.cn/Article/details/gmatffoxc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/gwnlwqvgl.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.tarul.cn/Article/details/gkupzgrbt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.epnwcf.com/Article/details/goertzxpp.sHtML

[U99] JS：事件监听
来源：http://m.share.yfazqb.com/Article/details/gbraxaase.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.bbcook.cn/Article/details/gcslxepsn.sHtML

[U100] JS：DOM 查询
来源：http://m.share.vehdjk.com/Article/details/gnrmpgazj.sHtML

document.querySelector(".item")
来源：http://mobile.sjlbkw.cn/Article/details/gbwvvjyzq.sHtML

[U101] JS：classList 操作
来源：http://www.share.yfazqb.com/Article/details/gqqughroj.sHtML

el.classList.toggle("active")
来源：http://mobile.yfazqb.com/Article/details/gqmfgotsm.sHtML

[U102] JS：本地存储
来源：http://www.blog.epnwcf.com/Article/details/gopgzjnsg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.sjlbkw.cn/Article/details/gacykmlaf.sHtML

[U103] JS：定时器
来源：http://3g.epnwcf.com/Article/details/gabydtcxp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.sjlbkw.cn/Article/details/gzmddvypc.sHtML

[U104] JS：防抖
来源：http://mobile.epnwcf.com/Article/details/grzjmizar.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gdcbrnqas.sHtML

[U105] JS：节流
来源：http://3g.bbcook.cn/Article/details/gshpcdsbq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fktsv.cn/Article/details/gpycllceu.sHtML

[U106] JS：日期格式化
来源：http://wap.fktsv.cn/Article/details/gfdwfcoew.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.yfazqb.com/Article/details/ghkanjehv.sHtML

[U107] JS：数字千分位
来源：http://baike.bbcook.cn/Article/details/gprnbuftk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.epnwcf.com/Article/details/gafadggks.sHtML

[U108] JS：随机整数
来源：http://mobile.fktsv.cn/Article/details/glxmbwwmx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.bbcook.cn/Article/details/girnjonqk.sHtML

[U109] JS：数组分组
来源：http://read.share.sjlbkw.cn/Article/details/gsedjexdt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.epnwcf.com/Article/details/guwojlbpr.sHtML

[U110] JS：数组分块
来源：http://m.share.epnwcf.com/Article/details/gpdtzshfr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fktsv.cn/Article/details/glgsujnrz.sHtML

[U111] JS：对象转 Map
来源：http://baike.tarul.cn/Article/details/glvhfkzpf.sHtML

new Map(Object.entries(obj))
来源：http://read.share.bbcook.cn/Article/details/gewobsxsu.sHtML

[U112] JS：字符串补位
来源：http://3g.fktsv.cn/Article/details/ghmtlbwxx.sHtML

"7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/glbmcrxqx.sHtML

[U113] JS：正则替换全部
来源：http://baike.fktsv.cn/Article/details/gohnbozej.sHtML

s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/glaanchwq.sHtML

[U114] JS：JSON 深比较
来源：http://baike.sjlbkw.cn/Article/details/gkegmhmdo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/ghwqacojh.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.tarul.cn/Article/details/ghaziivrl.sHtML

crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gbrwpkywn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.yfazqb.com/Article/details/gqgghrxrj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.vehdjk.com/Article/details/ginayawrk.sHtML

[U117] JS：单元测试
来源：http://wap.tarul.cn/Article/details/gniltkkva.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.bbcook.cn/Article/details/gqanfizgc.sHtML

[U118] JS：开发服务器
来源：http://wap.tarul.cn/Article/details/gumryqdhv.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fktsv.cn/Article/details/gmyejlnyw.sHtML

[U119] JS：生产构建
来源：http://read.share.yfazqb.com/Article/details/gdiruzjkb.sHtML

npx vite build
来源：http://3g.epnwcf.com/Article/details/geonfexrx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fktsv.cn/Article/details/gigwfkctg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.bbcook.cn/Article/details/gdsqnkfxv.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdftvgovk.sHtML

统计汇总
来源：http://mobile.fktsv.cn/Article/details/goybwznnj.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ggpzgkvjn.sHtML

按语言统计（条）：
来源：http://mobile.fktsv.cn/Article/details/guuohegrw.sHtML

Python ......... 252
来源：http://www.share.vehdjk.com/Article/details/gbjebuqph.sHtML

PHP ............ 252
来源：http://wap.sjlbkw.cn/Article/details/gthcoxkvx.sHtML

JavaScript ..... 252
来源：http://mobile.bbcook.cn/Article/details/ghkpjhebu.sHtML

TypeScript ..... 212
来源：http://baike.fktsv.cn/Article/details/gruhlzems.sHtML

Java ........... 212
来源：http://read.share.sjlbkw.cn/Article/details/gyvylvrtk.sHtML

Go ............. 212
来源：http://blog.fktsv.cn/Article/details/goatvfsfm.sHtML

Ruby ........... 212
来源：http://www.share.sjlbkw.cn/Article/details/gioeiurna.sHtML

C# ............. 212
来源：http://www.m.share.vehdjk.com/Article/details/gpowrsred.sHtML

C .............. 30
来源：http://read.share.sjlbkw.cn/Article/details/grmsrxbei.sHtML

C++ ............ 30
来源：http://read.share.tarul.cn/Article/details/gfefohlgj.sHtML

SQL ............ 90
来源：http://blog.sjlbkw.cn/Article/details/gnumiliuv.sHtML

Bash ........... 80
来源：http://wap.epnwcf.com/Article/details/gohcgboqm.sHtML

Kotlin ......... 15
来源：http://wap.sjlbkw.cn/Article/details/gpzsigqru.sHtML

Swift .......... 15
来源：http://baike.tarul.cn/Article/details/grgkkpifs.sHtML

Lua ............ 10
来源：http://3g.sjlbkw.cn/Article/details/glvrfgwvs.sHtML

Perl ........... 10
来源：http://m.share.vehdjk.com/Article/details/gdzzhdidj.sHtML

Scala .......... 10
来源：http://mobile.epnwcf.com/Article/details/gsoxitceu.sHtML

------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gjlxhzsae.sHtML

合计 ........... 2106 条
来源：http://www.share.fktsv.cn/Article/details/gsdtqspoc.sHtML

按章节统计：
来源：http://www.m.share.yfazqb.com/Article/details/gpybojxui.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.bbcook.cn/Article/details/gabelnzls.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.epnwcf.com/Article/details/gvjblklmz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.bbcook.cn/Article/details/guibytuyo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fktsv.cn/Article/details/gokitvcoo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.tarul.cn/Article/details/gswdbmsfg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.vehdjk.com/Article/details/gtzdkwwxv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.bbcook.cn/Article/details/gmffskbhv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.tarul.cn/Article/details/gipkqoziw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/gmtcxqiyx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fktsv.cn/Article/details/gclxujpns.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.tarul.cn/Article/details/gxgulznfa.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gjzpyrnlo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gexipcetv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.yfazqb.com/Article/details/gpcxtqdft.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.bbcook.cn/Article/details/gzlaspxll.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/glkqppimj.sHtML

Q SQL 专题                              90
来源：http://read.share.tarul.cn/Article/details/ggklvuzil.sHtML

R Bash 专题                             80
来源：http://blog.epnwcf.com/Article/details/gegatnyug.sHtML

S C / C++ 专题                          60
来源：http://baike.fktsv.cn/Article/details/gvlnbajhc.sHtML

T 其他语言补充                          60
来源：http://mobile.vehdjk.com/Article/details/gumqxfnos.sHtML

U 高频实用片段                         120
来源：http://mobile.epnwcf.com/Article/details/ganinzhbl.sHtML

------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gnwlhfrqb.sHtML

合计                                  2106 条
来源：http://www.share.yfazqb.com/Article/details/gvdfkgxto.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.epnwcf.com/Article/details/gxyjdtiry.sHtML

使用提醒
来源：http://wap.sjlbkw.cn/Article/details/gfjewyayh.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/gqnmwzhor.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.sjlbkw.cn/Article/details/grjjallie.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fktsv.cn/Article/details/geewrdvsh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.epnwcf.com/Article/details/gkrxoauqd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.yfazqb.com/Article/details/gqlumvpvy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.tarul.cn/Article/details/gtqvthayt.sHtML

—— 文件结束 ——
来源：http://www.m.share.fktsv.cn/Article/details/gfzhizsta.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gtilrghuc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.tarul.cn/Article/details/gkvmyfgtc.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fktsv.cn/Article/details/gddteqfih.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/guscaovoc.sHtML

【收录内容】
来源：http://blog.yfazqb.com/Article/details/gsydgyitw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.bbcook.cn/Article/details/gmrtjyzpc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.sjlbkw.cn/Article/details/gezqxhaxe.sHtML

SQL · Bash · C · C++
来源：http://www.share.yfazqb.com/Article/details/giiufeofy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.sjlbkw.cn/Article/details/gxzckzlod.sHtML

【使用说明】
来源：http://baike.vehdjk.com/Article/details/guionuvnt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.epnwcf.com/Article/details/geusssano.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.tarul.cn/Article/details/gbytylbrn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.epnwcf.com/Article/details/gqgakzyrm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.bbcook.cn/Article/details/gswnuyfcu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.tarul.cn/Article/details/gbzkagsag.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.tarul.cn/Article/details/gfrxoekgb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.yfazqb.com/Article/details/geoaxwisy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.sjlbkw.cn/Article/details/grhflubap.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.tarul.cn/Article/details/glxedcwtc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.sjlbkw.cn/Article/details/gyplvhshr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.vehdjk.com/Article/details/ghqttecap.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.tarul.cn/Article/details/gjgvqptrz.sHtML

【文件统计】
来源：http://www.m.share.sjlbkw.cn/Article/details/grwgqnfii.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.bbcook.cn/Article/details/gvzlbxcpx.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gijbmjivx.sHtML

目  录
来源：http://www.share.fktsv.cn/Article/details/gnkfhusbg.sHtML

--------------------------------------------------------------------------------
来源：http://wap.yfazqb.com/Article/details/gqempiged.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.vehdjk.com/Article/details/gjgqktlgs.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.bbcook.cn/Article/details/gyctjdzhl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gxnsibxhs.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.sjlbkw.cn/Article/details/glckaqtim.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.yfazqb.com/Article/details/gvbkfhtxk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.yfazqb.com/Article/details/grnexubwm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.tarul.cn/Article/details/gpyepzdac.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fktsv.cn/Article/details/gaiwatbmj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.vehdjk.com/Article/details/gfkopvear.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.sjlbkw.cn/Article/details/ghrasuwqg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/gbnnzgmcg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/gkfwtnibv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gowfqzetd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gjwhdwpfy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.yfazqb.com/Article/details/gnblrcgcq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/gephddyso.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.bbcook.cn/Article/details/gkfelhafa.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.tarul.cn/Article/details/ghisapevy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.tarul.cn/Article/details/gcsknpeoi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.bbcook.cn/Article/details/gzmyosyhv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.yfazqb.com/Article/details/glgjmexfp.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gkylqldma.sHtML

A. 基础语法与类型
来源：http://read.share.bbcook.cn/Article/details/guorqpnrb.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gpkktfpqv.sHtML

[A01] Hello World
来源：http://www.blog.yfazqb.com/Article/details/gzceowjsk.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.bbcook.cn/Article/details/gfkmgvkim.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.tarul.cn/Article/details/gyhdqobfu.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.yfazqb.com/Article/details/gtjdikxgj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fktsv.cn/Article/details/gqwafyxao.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.epnwcf.com/Article/details/gayauzjnx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.vehdjk.com/Article/details/gmmjxkmyp.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.yfazqb.com/Article/details/gmuyojekb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.sjlbkw.cn/Article/details/gyjenwdrv.sHtML

[A02] 变量声明与赋值
来源：http://www.share.bbcook.cn/Article/details/gnhazqijq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.vehdjk.com/Article/details/gkzwfvcou.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.bbcook.cn/Article/details/glrylefgq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.sjlbkw.cn/Article/details/gbxpeefuy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gnzntabyw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gqurffnoa.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.tarul.cn/Article/details/gsifjtjxy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.bbcook.cn/Article/details/gahpluvze.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.tarul.cn/Article/details/gewyxdctl.sHtML

[A03] 常量定义
来源：http://baike.yfazqb.com/Article/details/ghjoiuqze.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.tarul.cn/Article/details/goyzdlgoc.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gnkiqjbih.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gmkranvuk.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gsdnaltpa.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/goacedhjt.sHtML

Go:   const PI = 3.14159
来源：http://mobile.sjlbkw.cn/Article/details/gatvhprgb.sHtML

Ruby: PI = 3.14159
来源：http://blog.fktsv.cn/Article/details/guwppevjp.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/glmpbkhda.sHtML

[A04] 判断变量类型
来源：http://www.m.share.vehdjk.com/Article/details/gkodikwbf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.epnwcf.com/Article/details/gzapdpboo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.yfazqb.com/Article/details/gtzqtdanm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.tarul.cn/Article/details/gcdxiamib.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.tarul.cn/Article/details/gfdugkbmp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.vehdjk.com/Article/details/guexcvbhx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.bbcook.cn/Article/details/gyclpyeos.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fktsv.cn/Article/details/gbfzhcglz.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fktsv.cn/Article/details/gzqsvvbsn.sHtML

[A05] 整数除法与取模
来源：http://blog.bbcook.cn/Article/details/getbxjgax.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fktsv.cn/Article/details/gajshqcjd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.yfazqb.com/Article/details/gtjmtmptu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gwvlbmxvg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.sjlbkw.cn/Article/details/gnbdxjdwh.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.epnwcf.com/Article/details/geerzutts.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/gwrefwnqi.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.bbcook.cn/Article/details/gbjclkbub.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gisyyzytx.sHtML

[A06] 字符串转数字
来源：http://baike.vehdjk.com/Article/details/gueprimcy.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fktsv.cn/Article/details/gtkibpkji.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fktsv.cn/Article/details/gduxexnmb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.sjlbkw.cn/Article/details/gtelzgdou.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.bbcook.cn/Article/details/gohkmvmyr.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.bbcook.cn/Article/details/gxzciqcjd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.epnwcf.com/Article/details/gsgiwaorl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.yfazqb.com/Article/details/gfhdrcwqq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.epnwcf.com/Article/details/ggzyiblwm.sHtML

[A07] 数字转字符串
来源：http://3g.fktsv.cn/Article/details/gyulykava.sHtML

Py:   str(42)
来源：http://mobile.tarul.cn/Article/details/gxfnkhhvi.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fktsv.cn/Article/details/gvbppgnjs.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.epnwcf.com/Article/details/gabwdeveu.sHtML

TS:   String(42)
来源：http://www.share.tarul.cn/Article/details/gvyotdgde.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.epnwcf.com/Article/details/gjypogsjs.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.vehdjk.com/Article/details/grmuvuhgr.sHtML

Ruby: 42.to_s
来源：http://3g.tarul.cn/Article/details/gmxetiihw.sHtML

C#:   42.ToString()
来源：http://wap.epnwcf.com/Article/details/gwplkfbhd.sHtML

[A08] 取整与四舍五入
来源：http://blog.fktsv.cn/Article/details/gngqpptqo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.epnwcf.com/Article/details/gmaoqwjsw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.epnwcf.com/Article/details/gjyflxfgb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.tarul.cn/Article/details/gubqfpgjq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.fktsv.cn/Article/details/ggwztwqrv.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.sjlbkw.cn/Article/details/ghajmzaka.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.vehdjk.com/Article/details/gsevjzhes.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.epnwcf.com/Article/details/gbzrcnuqg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.vehdjk.com/Article/details/gaqoswzop.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.yfazqb.com/Article/details/gwfcbnuhk.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gtgxiybvj.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.epnwcf.com/Article/details/gmhdyeurw.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gcualgpwc.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.fktsv.cn/Article/details/gmufkyctc.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.yfazqb.com/Article/details/gzrsxwwup.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.bbcook.cn/Article/details/gwhkqqksl.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.tarul.cn/Article/details/gjqecjqko.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gqicskggy.sHtML

[A10] 生成随机数
来源：http://3g.fktsv.cn/Article/details/gujduacff.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.yfazqb.com/Article/details/gvzhdedhg.sHtML

PHP:  random_int(1, 100);
来源：http://blog.epnwcf.com/Article/details/gptfuomuv.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.epnwcf.com/Article/details/gjvxcvhwu.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.epnwcf.com/Article/details/gxsuhgrsr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.sjlbkw.cn/Article/details/gqeoftyay.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.fktsv.cn/Article/details/guufzzigx.sHtML

Ruby: rand(1..100)
来源：http://read.share.fktsv.cn/Article/details/gyzxlvnhl.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.vehdjk.com/Article/details/gnalhgasw.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.yfazqb.com/Article/details/gapkzjsur.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.epnwcf.com/Article/details/gizvypznr.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.bbcook.cn/Article/details/gnhswkxqp.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.epnwcf.com/Article/details/gqmaeoscn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.fktsv.cn/Article/details/gwvnbbhfr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.tarul.cn/Article/details/gndjxlhfq.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.fktsv.cn/Article/details/gevegoqrf.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.epnwcf.com/Article/details/geclncdia.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.sjlbkw.cn/Article/details/gjndlltpk.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.sjlbkw.cn/Article/details/gixwwuaak.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.fktsv.cn/Article/details/ggypxgqbz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.epnwcf.com/Article/details/gfithuilp.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.epnwcf.com/Article/details/grstfjffc.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.yfazqb.com/Article/details/glrcfspzr.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.vehdjk.com/Article/details/gnrrxwgnf.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.tarul.cn/Article/details/gzgnlfvei.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.vehdjk.com/Article/details/gugakbafh.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.yfazqb.com/Article/details/ghsffblgs.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.bbcook.cn/Article/details/gdwgswjau.sHtML

Py:   "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/guwzbfcyn.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/gsfusbbnw.sHtML

JS:   "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gcbqekzer.sHtML

TS:   "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gwmpwvbrk.sHtML

Java: "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/ghxbqoqxu.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gbwwapeii.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/ggsamyvjk.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.yfazqb.com/Article/details/grrlmxlmp.sHtML

[A14] 注释写法
来源：http://www.m.share.tarul.cn/Article/details/gdgxdsywj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.vehdjk.com/Article/details/gwypbvvke.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.epnwcf.com/Article/details/gkwxyfbko.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/ggtacwpgt.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.bbcook.cn/Article/details/gndnqbynb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.fktsv.cn/Article/details/gypigydpj.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fktsv.cn/Article/details/gyhixovtj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.sjlbkw.cn/Article/details/gbodittzl.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.vehdjk.com/Article/details/gryabmxdm.sHtML

[A15] 空值判断与默认值
来源：http://www.share.vehdjk.com/Article/details/gnkxhhnhr.sHtML

Py:   value = data or "默认值"
来源：http://mobile.vehdjk.com/Article/details/gkkybfslg.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.bbcook.cn/Article/details/gffqavkpc.sHtML


<!-- 参考信息 -->