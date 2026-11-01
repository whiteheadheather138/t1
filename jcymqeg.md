代发 wailian999

[U85] JS：可选链
来源：http://m.share.fktsv.cn/Article/details/gnteqtgbi.sHtML

a?.b?.c
来源：http://m.share.bbcook.cn/Article/details/gxixlhfwp.sHtML

[U86] JS：空值合并
来源：http://blog.sjlbkw.cn/Article/details/gqdmwdxta.sHtML

a ?? b
来源：http://www.share.epnwcf.com/Article/details/grynmauhn.sHtML

[U87] JS：解构默认值
来源：http://baike.tarul.cn/Article/details/gbamuhsaq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.yfazqb.com/Article/details/gakdsbpkh.sHtML

[U88] JS：对象展开合并
来源：http://3g.sjlbkw.cn/Article/details/gweqzdxit.sHtML

{ ...a, ...b }
来源：http://read.share.epnwcf.com/Article/details/gqqbkoexv.sHtML

[U89] JS：数组去重
来源：http://wap.vehdjk.com/Article/details/gwibfstxa.sHtML

[...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gmuiqtbdy.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.vehdjk.com/Article/details/gwfhjrhxg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gdhqkijbb.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.vehdjk.com/Article/details/gilsdtejb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.epnwcf.com/Article/details/gknfrikcf.sHtML

[U92] JS：深拷贝
来源：http://www.share.fktsv.cn/Article/details/gplwswcaj.sHtML

structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gfusxtlqs.sHtML

[U93] JS：模板字符串
来源：http://mobile.bbcook.cn/Article/details/ghvddfruz.sHtML

`共 ${n} 条`
来源：http://www.blog.epnwcf.com/Article/details/gepdzewxq.sHtML

[U94] JS：箭头函数
来源：http://wap.sjlbkw.cn/Article/details/gyslkiiye.sHtML

const double = x => x * 2;
来源：http://blog.bbcook.cn/Article/details/gitckygtu.sHtML

[U95] JS：Promise 包装
来源：http://wap.sjlbkw.cn/Article/details/gpfijocwb.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.sjlbkw.cn/Article/details/gpahsejwz.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.vehdjk.com/Article/details/gjlrzvayp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gvsiuircq.sHtML

[U97] JS：并发请求
来源：http://read.share.vehdjk.com/Article/details/gecnkzomt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.epnwcf.com/Article/details/gzbxsmlme.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.yfazqb.com/Article/details/grfkmjnha.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.epnwcf.com/Article/details/gdurafibu.sHtML

[U99] JS：事件监听
来源：http://blog.sjlbkw.cn/Article/details/giqpzxavo.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fktsv.cn/Article/details/gxivsnxrx.sHtML

[U100] JS：DOM 查询
来源：http://3g.vehdjk.com/Article/details/gtgbbusjs.sHtML

document.querySelector(".item")
来源：http://www.share.sjlbkw.cn/Article/details/gguyxpvit.sHtML

[U101] JS：classList 操作
来源：http://read.share.epnwcf.com/Article/details/gbwdirlss.sHtML

el.classList.toggle("active")
来源：http://3g.sjlbkw.cn/Article/details/gqyatoaxn.sHtML

[U102] JS：本地存储
来源：http://mobile.sjlbkw.cn/Article/details/gbhmlchjo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.tarul.cn/Article/details/gzxfjowfj.sHtML

[U103] JS：定时器
来源：http://baike.bbcook.cn/Article/details/gninoiotm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.vehdjk.com/Article/details/gybztriaq.sHtML

[U104] JS：防抖
来源：http://blog.tarul.cn/Article/details/gvxxqcoze.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gcvwhfdes.sHtML

[U105] JS：节流
来源：http://baike.fktsv.cn/Article/details/gggtunzak.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.bbcook.cn/Article/details/gltwugpsd.sHtML

[U106] JS：日期格式化
来源：http://mobile.bbcook.cn/Article/details/gpauszurc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.sjlbkw.cn/Article/details/gklszlxbh.sHtML

[U107] JS：数字千分位
来源：http://m.share.yfazqb.com/Article/details/gotxrusdr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.bbcook.cn/Article/details/gebmyexku.sHtML

[U108] JS：随机整数
来源：http://m.share.sjlbkw.cn/Article/details/gqfnjilbk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.epnwcf.com/Article/details/gvypogqij.sHtML

[U109] JS：数组分组
来源：http://www.blog.tarul.cn/Article/details/guzccqprq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.tarul.cn/Article/details/gmwlipxvn.sHtML

[U110] JS：数组分块
来源：http://www.m.share.vehdjk.com/Article/details/gigsvaxcn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.bbcook.cn/Article/details/gtaaslxhs.sHtML

[U111] JS：对象转 Map
来源：http://blog.bbcook.cn/Article/details/gonwdbkyj.sHtML

new Map(Object.entries(obj))
来源：http://read.share.epnwcf.com/Article/details/gnteplmpp.sHtML

[U112] JS：字符串补位
来源：http://www.share.bbcook.cn/Article/details/glgjikhxe.sHtML

"7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gvzwvzxhh.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.vehdjk.com/Article/details/ggzcamdkj.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gctbdnirz.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fktsv.cn/Article/details/gdpdbaisi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.tarul.cn/Article/details/gejrcddii.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fktsv.cn/Article/details/gznrkehup.sHtML

crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/ggudmmqrd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.tarul.cn/Article/details/gzqowncmr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.yfazqb.com/Article/details/gfcmajrjz.sHtML

[U117] JS：单元测试
来源：http://www.blog.bbcook.cn/Article/details/gqxvclabj.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.bbcook.cn/Article/details/gthezpvyn.sHtML

[U118] JS：开发服务器
来源：http://www.blog.sjlbkw.cn/Article/details/gbrozacre.sHtML

npm i -D vite;  npx vite
来源：http://wap.tarul.cn/Article/details/galcashzq.sHtML

[U119] JS：生产构建
来源：http://3g.epnwcf.com/Article/details/gcoefnnkx.sHtML

npx vite build
来源：http://www.blog.epnwcf.com/Article/details/gubdpcniq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.bbcook.cn/Article/details/guxznwzft.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.vehdjk.com/Article/details/guerpiolh.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gnmhcumaz.sHtML

统计汇总
来源：http://www.blog.vehdjk.com/Article/details/gszvsabwt.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gesasfmww.sHtML

按语言统计（条）：
来源：http://mobile.fktsv.cn/Article/details/gbsygrllb.sHtML

Python ......... 252
来源：http://read.share.sjlbkw.cn/Article/details/gqlwpilnr.sHtML

PHP ............ 252
来源：http://3g.vehdjk.com/Article/details/gywwgtwlp.sHtML

JavaScript ..... 252
来源：http://mobile.yfazqb.com/Article/details/gkvbytmpl.sHtML

TypeScript ..... 212
来源：http://m.share.bbcook.cn/Article/details/gjktdvlmx.sHtML

Java ........... 212
来源：http://wap.yfazqb.com/Article/details/gtguzubcs.sHtML

Go ............. 212
来源：http://mobile.tarul.cn/Article/details/goqfkaxac.sHtML

Ruby ........... 212
来源：http://mobile.tarul.cn/Article/details/gotnysvdp.sHtML

C# ............. 212
来源：http://read.share.sjlbkw.cn/Article/details/gfxccfgan.sHtML

C .............. 30
来源：http://wap.sjlbkw.cn/Article/details/gpukxynkm.sHtML

C++ ............ 30
来源：http://www.blog.bbcook.cn/Article/details/gbwuucnbf.sHtML

SQL ............ 90
来源：http://baike.bbcook.cn/Article/details/gfgdbzbnj.sHtML

Bash ........... 80
来源：http://blog.tarul.cn/Article/details/gihiqcajn.sHtML

Kotlin ......... 15
来源：http://wap.sjlbkw.cn/Article/details/gfhukjnzj.sHtML

Swift .......... 15
来源：http://3g.fktsv.cn/Article/details/gyarwdcil.sHtML

Lua ............ 10
来源：http://3g.vehdjk.com/Article/details/gekqklsfb.sHtML

Perl ........... 10
来源：http://www.blog.sjlbkw.cn/Article/details/gimottmix.sHtML

Scala .......... 10
来源：http://m.share.sjlbkw.cn/Article/details/gowclrypb.sHtML

------------------------------------
来源：http://wap.tarul.cn/Article/details/gjhkcxaqg.sHtML

合计 ........... 2106 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrrfpath.sHtML

按章节统计：
来源：http://m.share.yfazqb.com/Article/details/gpwdqyvti.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.sjlbkw.cn/Article/details/gznrsnpwl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.bbcook.cn/Article/details/gmbikufox.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.tarul.cn/Article/details/guklovwmz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.epnwcf.com/Article/details/gtngayxwa.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fktsv.cn/Article/details/gzboppwyk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.tarul.cn/Article/details/goatlfzuu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gtbucagrs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fktsv.cn/Article/details/gmspijsgk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/gmzmakvdr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.epnwcf.com/Article/details/gpftgtavv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gkcvgxpna.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gaufnvzce.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/ghboibbha.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.bbcook.cn/Article/details/gvelgobmz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fktsv.cn/Article/details/gmwqfuphf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/giwcclkea.sHtML

Q SQL 专题                              90
来源：http://3g.bbcook.cn/Article/details/geswshvje.sHtML

R Bash 专题                             80
来源：http://mobile.vehdjk.com/Article/details/ggllmiopx.sHtML

S C / C++ 专题                          60
来源：http://read.share.sjlbkw.cn/Article/details/geiemjajq.sHtML

T 其他语言补充                          60
来源：http://www.blog.tarul.cn/Article/details/gcevhudpu.sHtML

U 高频实用片段                         120
来源：http://m.share.epnwcf.com/Article/details/gtfscowvo.sHtML

------------------------------------
来源：http://mobile.tarul.cn/Article/details/gycnqfjha.sHtML

合计                                  2106 条
来源：http://www.share.bbcook.cn/Article/details/gofjlkorz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.bbcook.cn/Article/details/gslkvqppz.sHtML

使用提醒
来源：http://mobile.bbcook.cn/Article/details/gfyvptjdo.sHtML

--------------------------------------------------------------------------------
来源：http://3g.bbcook.cn/Article/details/ghjswfzaf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.sjlbkw.cn/Article/details/ggitzswdf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.epnwcf.com/Article/details/ggmeuntur.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.epnwcf.com/Article/details/gylmcgbqz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.sjlbkw.cn/Article/details/gaeibwvdh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.tarul.cn/Article/details/gpgnoxfms.sHtML

—— 文件结束 ——
来源：http://www.share.bbcook.cn/Article/details/gyjarmyom.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gbhqmshzf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.vehdjk.com/Article/details/gacjbhzbh.sHtML

Common Programming Examples Cheat Book
来源：http://wap.vehdjk.com/Article/details/gbmtussng.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/grxmdyile.sHtML

【收录内容】
来源：http://read.share.bbcook.cn/Article/details/ggqbdjqyg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.yfazqb.com/Article/details/gemfajsqt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.bbcook.cn/Article/details/gthnpowex.sHtML

SQL · Bash · C · C++
来源：http://3g.fktsv.cn/Article/details/giyhzirhx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.yfazqb.com/Article/details/gqhknqadl.sHtML

【使用说明】
来源：http://www.m.share.bbcook.cn/Article/details/gfreadbar.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.vehdjk.com/Article/details/gvcamtnpg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.epnwcf.com/Article/details/gwleajayv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.bbcook.cn/Article/details/gyzvigojt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.sjlbkw.cn/Article/details/gwayjcubd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fktsv.cn/Article/details/ggsblcxqj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.tarul.cn/Article/details/gezqgucvi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.vehdjk.com/Article/details/gxytieejg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.bbcook.cn/Article/details/gokqnvrem.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.sjlbkw.cn/Article/details/gzbjtkzbm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.sjlbkw.cn/Article/details/glmdrvvcm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.epnwcf.com/Article/details/ghmvmrkxt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.yfazqb.com/Article/details/gmpvhvocd.sHtML

【文件统计】
来源：http://www.m.share.fktsv.cn/Article/details/gamdeetde.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.bbcook.cn/Article/details/gdawxznwa.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.yfazqb.com/Article/details/gobchgjlb.sHtML

目  录
来源：http://blog.yfazqb.com/Article/details/gwnanvlcd.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gjpnebptx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.sjlbkw.cn/Article/details/gcbryoqwe.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.epnwcf.com/Article/details/gaqzxwnyv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.bbcook.cn/Article/details/gukqwxhms.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.sjlbkw.cn/Article/details/gljtolqvr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.vehdjk.com/Article/details/gcxfdpaqd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.tarul.cn/Article/details/glfgpwolg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.vehdjk.com/Article/details/gzitueeno.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fktsv.cn/Article/details/gnaupryev.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gyhoctwlt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.epnwcf.com/Article/details/gqnxvdbpk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gbwkthemr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.vehdjk.com/Article/details/gfeemjqvl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/ghjmwlepj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.sjlbkw.cn/Article/details/grqwxrzvg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.sjlbkw.cn/Article/details/gbsbmizbs.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.epnwcf.com/Article/details/gzqhwzbgr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fktsv.cn/Article/details/gbpexfnnq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.yfazqb.com/Article/details/grpaypqjr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.tarul.cn/Article/details/gaigoogup.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.sjlbkw.cn/Article/details/gnkjehmhv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.tarul.cn/Article/details/glrzhbrao.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ggbrnryfa.sHtML

A. 基础语法与类型
来源：http://mobile.bbcook.cn/Article/details/gqicyaehz.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gyerlteya.sHtML

[A01] Hello World
来源：http://baike.bbcook.cn/Article/details/gqdwwhxok.sHtML

Py:   print("Hello, World!")
来源：http://wap.tarul.cn/Article/details/gkxzkoulc.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.yfazqb.com/Article/details/gkoyicwxt.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.sjlbkw.cn/Article/details/gcujuplga.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.sjlbkw.cn/Article/details/gvgkzmghr.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.tarul.cn/Article/details/gupdthvyo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.yfazqb.com/Article/details/gocfzurfl.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.vehdjk.com/Article/details/gqsypjdyb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.vehdjk.com/Article/details/ghlsdtiux.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fktsv.cn/Article/details/gdhqnoxii.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.bbcook.cn/Article/details/guoohgmto.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.bbcook.cn/Article/details/giqgmzdqy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.bbcook.cn/Article/details/ggzuvxtkq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.sjlbkw.cn/Article/details/glivjfsla.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.tarul.cn/Article/details/gvkstmjtn.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.bbcook.cn/Article/details/gntaxaufo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fktsv.cn/Article/details/ghsiqurhp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.epnwcf.com/Article/details/goirbpwlb.sHtML

[A03] 常量定义
来源：http://blog.tarul.cn/Article/details/gktzlsrxi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.yfazqb.com/Article/details/gnjbwmstq.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gcnpbzglx.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gtmfxcves.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.yfazqb.com/Article/details/groezugge.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gnnpasfwi.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fktsv.cn/Article/details/gxbvzxfsw.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.bbcook.cn/Article/details/gugcqwcqm.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gofbncpkh.sHtML

[A04] 判断变量类型
来源：http://www.share.yfazqb.com/Article/details/gqawkpemg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.bbcook.cn/Article/details/gewvufjyo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.epnwcf.com/Article/details/gbnxunsiy.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.epnwcf.com/Article/details/goxkjypez.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.bbcook.cn/Article/details/gmlvyoprz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.vehdjk.com/Article/details/gwvqtvvwb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.sjlbkw.cn/Article/details/ghbzzzdgf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.vehdjk.com/Article/details/gqqcskscg.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.vehdjk.com/Article/details/gxcgbmrld.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.sjlbkw.cn/Article/details/grnpnfhbz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.vehdjk.com/Article/details/gmnfesehy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gzxduuppx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/gwxxdetmf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.tarul.cn/Article/details/gjqsnptqc.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.tarul.cn/Article/details/gmloltgdn.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.yfazqb.com/Article/details/girjbrtat.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/gzcaksljw.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.bbcook.cn/Article/details/gggawgycj.sHtML

[A06] 字符串转数字
来源：http://www.blog.yfazqb.com/Article/details/getiyhhbm.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fktsv.cn/Article/details/gqagjwcgh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.tarul.cn/Article/details/gkgvziirt.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.tarul.cn/Article/details/gjkyjyoyt.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.vehdjk.com/Article/details/gozktibbr.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.yfazqb.com/Article/details/gjhaphmiw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.epnwcf.com/Article/details/gcyxmgvah.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.tarul.cn/Article/details/guvtfnpna.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.epnwcf.com/Article/details/gganvsuna.sHtML

[A07] 数字转字符串
来源：http://3g.yfazqb.com/Article/details/ghedaorvj.sHtML

Py:   str(42)
来源：http://3g.yfazqb.com/Article/details/gpmzcxakv.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.bbcook.cn/Article/details/gwtmamedb.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.sjlbkw.cn/Article/details/gpqljnxda.sHtML

TS:   String(42)
来源：http://blog.tarul.cn/Article/details/ggkzmmhak.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.vehdjk.com/Article/details/gqiqcdxak.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.bbcook.cn/Article/details/gemvafsje.sHtML

Ruby: 42.to_s
来源：http://www.m.share.sjlbkw.cn/Article/details/giyfshocl.sHtML

C#:   42.ToString()
来源：http://blog.epnwcf.com/Article/details/ggdetcbmb.sHtML

[A08] 取整与四舍五入
来源：http://baike.fktsv.cn/Article/details/gaotagshh.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.tarul.cn/Article/details/gwwnxkrnl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.bbcook.cn/Article/details/gkamfxbmp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.bbcook.cn/Article/details/gvyvgzvqv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fktsv.cn/Article/details/gvvvuevso.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.epnwcf.com/Article/details/gnqsyhrsr.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.vehdjk.com/Article/details/gdoqlyxdn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.epnwcf.com/Article/details/gdlajssgx.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.epnwcf.com/Article/details/gsszrkwrk.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.yfazqb.com/Article/details/ggnxjhkwy.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.sjlbkw.cn/Article/details/ghfqzzrjy.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.yfazqb.com/Article/details/gdgwefkqn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gajejatzu.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gbjindwqz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.bbcook.cn/Article/details/gvvxahgfa.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.sjlbkw.cn/Article/details/gykfllkho.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.sjlbkw.cn/Article/details/ghlrspjab.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.tarul.cn/Article/details/gfoucgyzs.sHtML

[A10] 生成随机数
来源：http://www.blog.yfazqb.com/Article/details/gizaefhsu.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.epnwcf.com/Article/details/gwzisvzas.sHtML

PHP:  random_int(1, 100);
来源：http://baike.vehdjk.com/Article/details/guhutnytv.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.bbcook.cn/Article/details/gxyoiwszf.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.yfazqb.com/Article/details/gyhfrptun.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fktsv.cn/Article/details/gxqektciu.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.epnwcf.com/Article/details/glvdnshrh.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.bbcook.cn/Article/details/ggywferdp.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.tarul.cn/Article/details/gaejnphuj.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.vehdjk.com/Article/details/gwribgnbe.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.bbcook.cn/Article/details/gdyukteoj.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fktsv.cn/Article/details/gyvcyqgmq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.epnwcf.com/Article/details/gbktgempa.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.yfazqb.com/Article/details/gtmsnhrss.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.tarul.cn/Article/details/gajmcdxjt.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.sjlbkw.cn/Article/details/glpivpapt.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.bbcook.cn/Article/details/gqcunjzzy.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.vehdjk.com/Article/details/gltqtwhoy.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fktsv.cn/Article/details/gtotbdnyq.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.bbcook.cn/Article/details/gsykkrnjf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.yfazqb.com/Article/details/gpnguxppq.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.yfazqb.com/Article/details/gqxgpphjx.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.vehdjk.com/Article/details/gaivmpppp.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.vehdjk.com/Article/details/gisjzlxxn.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.yfazqb.com/Article/details/gbjpxtrqz.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.tarul.cn/Article/details/gqxzzzyqt.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.epnwcf.com/Article/details/geebtnpcf.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fktsv.cn/Article/details/gvuvbbdgd.sHtML

Py:   "第一行\n第二行"
来源：http://wap.vehdjk.com/Article/details/gevntgixi.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gwfbbmwmv.sHtML

JS:   "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gwpcetpjx.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/gmlfgggxd.sHtML

Java: "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gekngaubo.sHtML

Go:   "第一行\n第二行"
来源：http://blog.sjlbkw.cn/Article/details/gbsmijdjv.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.fktsv.cn/Article/details/gzsxixjvb.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/gmtzacnia.sHtML

[A14] 注释写法
来源：http://www.m.share.fktsv.cn/Article/details/ghtanznrz.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.sjlbkw.cn/Article/details/goctavgyh.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.epnwcf.com/Article/details/ghxnusdap.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.yfazqb.com/Article/details/gfyvsticv.sHtML


<!-- 参考信息 -->