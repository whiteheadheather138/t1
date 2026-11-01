代发 wailian999

[U89] JS：数组去重
来源：http://www.m.share.yfazqb.com/Article/details/gugtjhfdi.sHtML

[...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gkpeqxzce.sHtML

[U90] JS：数字数组排序
来源：http://blog.fktsv.cn/Article/details/gmoxuryrf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/gqwoajyzo.sHtML

[U91] JS：对象键值遍历
来源：http://blog.yfazqb.com/Article/details/gzstbdtza.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.sjlbkw.cn/Article/details/gthztwpym.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fktsv.cn/Article/details/gjkefnmqc.sHtML

structuredClone(obj)
来源：http://read.share.yfazqb.com/Article/details/gnvagmyzs.sHtML

[U93] JS：模板字符串
来源：http://baike.vehdjk.com/Article/details/gsprzbqde.sHtML

`共 ${n} 条`
来源：http://3g.yfazqb.com/Article/details/gfyhsiaui.sHtML

[U94] JS：箭头函数
来源：http://wap.vehdjk.com/Article/details/gujizfzzy.sHtML

const double = x => x * 2;
来源：http://wap.vehdjk.com/Article/details/guyehuebo.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.epnwcf.com/Article/details/gjkusipcl.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.tarul.cn/Article/details/gqqylltul.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fktsv.cn/Article/details/gukqgsclr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.vehdjk.com/Article/details/gorvbowmv.sHtML

[U97] JS：并发请求
来源：http://mobile.epnwcf.com/Article/details/gpskziuks.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/gflptjtwv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.bbcook.cn/Article/details/gcseollpa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.bbcook.cn/Article/details/gagnawrqs.sHtML

[U99] JS：事件监听
来源：http://wap.fktsv.cn/Article/details/gstnzojey.sHtML

el.addEventListener("click", e => {})
来源：http://blog.yfazqb.com/Article/details/guvlbtprr.sHtML

[U100] JS：DOM 查询
来源：http://blog.yfazqb.com/Article/details/geimeugnu.sHtML

document.querySelector(".item")
来源：http://www.m.share.epnwcf.com/Article/details/gjhsuwaie.sHtML

[U101] JS：classList 操作
来源：http://wap.sjlbkw.cn/Article/details/gddvlvshr.sHtML

el.classList.toggle("active")
来源：http://3g.vehdjk.com/Article/details/gmvadjzcl.sHtML

[U102] JS：本地存储
来源：http://m.share.yfazqb.com/Article/details/gpjzlvpjn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.yfazqb.com/Article/details/guandpqcu.sHtML

[U103] JS：定时器
来源：http://3g.bbcook.cn/Article/details/gmqxfkxrn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.epnwcf.com/Article/details/gxfcjlila.sHtML

[U104] JS：防抖
来源：http://www.m.share.fktsv.cn/Article/details/gxmjygngl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gmdrhfkjn.sHtML

[U105] JS：节流
来源：http://mobile.vehdjk.com/Article/details/gyhpbhzgw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.sjlbkw.cn/Article/details/gfayzmlpd.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gvresigkv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.sjlbkw.cn/Article/details/gdpjiirfe.sHtML

[U107] JS：数字千分位
来源：http://read.share.epnwcf.com/Article/details/gvnnvpugw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.tarul.cn/Article/details/gctvckpmk.sHtML

[U108] JS：随机整数
来源：http://baike.yfazqb.com/Article/details/gszdciavx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.epnwcf.com/Article/details/gpqbxggxw.sHtML

[U109] JS：数组分组
来源：http://www.m.share.yfazqb.com/Article/details/gdaplcdul.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.sjlbkw.cn/Article/details/gfvsvxdbq.sHtML

[U110] JS：数组分块
来源：http://baike.vehdjk.com/Article/details/gifsbvemn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.bbcook.cn/Article/details/gpfbozwqq.sHtML

[U111] JS：对象转 Map
来源：http://read.share.vehdjk.com/Article/details/ggseisgff.sHtML

new Map(Object.entries(obj))
来源：http://3g.epnwcf.com/Article/details/gqomglarf.sHtML

[U112] JS：字符串补位
来源：http://baike.yfazqb.com/Article/details/ggpxtmcob.sHtML

"7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gfwxlueuq.sHtML

[U113] JS：正则替换全部
来源：http://3g.vehdjk.com/Article/details/gcgfqjnig.sHtML

s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gsbxavslv.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.epnwcf.com/Article/details/ghcrstbbu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.epnwcf.com/Article/details/glfabzxaj.sHtML

[U115] JS：生成 UUID
来源：http://read.share.tarul.cn/Article/details/gbtoyaqfu.sHtML

crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/gamflwzar.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.epnwcf.com/Article/details/gbwvtxgvg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.epnwcf.com/Article/details/gbgbdhutc.sHtML

[U117] JS：单元测试
来源：http://baike.sjlbkw.cn/Article/details/ggjukstjx.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.sjlbkw.cn/Article/details/gxzoxbjta.sHtML

[U118] JS：开发服务器
来源：http://baike.vehdjk.com/Article/details/gtswrhbmc.sHtML

npm i -D vite;  npx vite
来源：http://m.share.sjlbkw.cn/Article/details/gjfkqlaov.sHtML

[U119] JS：生产构建
来源：http://read.share.tarul.cn/Article/details/gnxrqjdlo.sHtML

npx vite build
来源：http://blog.sjlbkw.cn/Article/details/gkzigppjz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fktsv.cn/Article/details/gtlnniwue.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.epnwcf.com/Article/details/gzergmnui.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/grqreymzu.sHtML

统计汇总
来源：http://www.blog.bbcook.cn/Article/details/gtgwsitnl.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gaqwlysov.sHtML

按语言统计（条）：
来源：http://3g.fktsv.cn/Article/details/ggtlurllz.sHtML

Python ......... 252
来源：http://www.blog.yfazqb.com/Article/details/gxjetxqux.sHtML

PHP ............ 252
来源：http://www.m.share.tarul.cn/Article/details/gkdunipfd.sHtML

JavaScript ..... 252
来源：http://m.share.yfazqb.com/Article/details/gdoooijqc.sHtML

TypeScript ..... 212
来源：http://blog.yfazqb.com/Article/details/guvhmlpkt.sHtML

Java ........... 212
来源：http://mobile.vehdjk.com/Article/details/gdvafjapv.sHtML

Go ............. 212
来源：http://www.share.epnwcf.com/Article/details/gkoodsojn.sHtML

Ruby ........... 212
来源：http://wap.yfazqb.com/Article/details/gppwknsoz.sHtML

C# ............. 212
来源：http://www.blog.vehdjk.com/Article/details/ghqwznvjm.sHtML

C .............. 30
来源：http://mobile.vehdjk.com/Article/details/gryeokena.sHtML

C++ ............ 30
来源：http://www.share.yfazqb.com/Article/details/gwsnyynac.sHtML

SQL ............ 90
来源：http://wap.tarul.cn/Article/details/gdykxlrtc.sHtML

Bash ........... 80
来源：http://wap.sjlbkw.cn/Article/details/gdnbpwzsq.sHtML

Kotlin ......... 15
来源：http://mobile.yfazqb.com/Article/details/ghagdanxt.sHtML

Swift .......... 15
来源：http://read.share.tarul.cn/Article/details/gahdzlbsu.sHtML

Lua ............ 10
来源：http://www.share.epnwcf.com/Article/details/gsjzpzerm.sHtML

Perl ........... 10
来源：http://www.share.fktsv.cn/Article/details/gajowfkfn.sHtML

Scala .......... 10
来源：http://m.share.yfazqb.com/Article/details/gwvbfcctk.sHtML

------------------------------------
来源：http://www.blog.tarul.cn/Article/details/glhokcigs.sHtML

合计 ........... 2106 条
来源：http://www.m.share.vehdjk.com/Article/details/gpekxcbxs.sHtML

按章节统计：
来源：http://read.share.epnwcf.com/Article/details/gtyqmwtfa.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.tarul.cn/Article/details/glzgekbge.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.vehdjk.com/Article/details/glxxgrora.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.yfazqb.com/Article/details/gotbxsxrr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.tarul.cn/Article/details/gqrjhgdwy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.vehdjk.com/Article/details/gutonisbp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.tarul.cn/Article/details/ggpcpwdhy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.bbcook.cn/Article/details/gajcsoany.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.epnwcf.com/Article/details/gdpmsqtms.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/gfizxeopu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.yfazqb.com/Article/details/gfmixhfye.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.bbcook.cn/Article/details/gdbvmjmaf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/gzimybfqm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gkehvhlsr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.tarul.cn/Article/details/gghuwcbju.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.vehdjk.com/Article/details/gpctpmmcv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gehkdmagr.sHtML

Q SQL 专题                              90
来源：http://wap.bbcook.cn/Article/details/glbdvqqzg.sHtML

R Bash 专题                             80
来源：http://read.share.yfazqb.com/Article/details/gqdmgehyt.sHtML

S C / C++ 专题                          60
来源：http://wap.bbcook.cn/Article/details/ggfflyait.sHtML

T 其他语言补充                          60
来源：http://www.blog.sjlbkw.cn/Article/details/grxmjiwmz.sHtML

U 高频实用片段                         120
来源：http://read.share.yfazqb.com/Article/details/gbmhlxqof.sHtML

------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gfxqoeiqk.sHtML

合计                                  2106 条
来源：http://www.blog.bbcook.cn/Article/details/gstxgtwgp.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/gvozzijvm.sHtML

使用提醒
来源：http://blog.yfazqb.com/Article/details/gxfbvuoaz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gsrikwdsn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.tarul.cn/Article/details/gpmaomzia.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.tarul.cn/Article/details/gkpjjeynr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.bbcook.cn/Article/details/gbeaonivp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.sjlbkw.cn/Article/details/gbljamons.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.bbcook.cn/Article/details/ggsttgkfo.sHtML

—— 文件结束 ——
来源：http://www.blog.fktsv.cn/Article/details/gbrlpwyqk.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gghamsldw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.yfazqb.com/Article/details/gfhfbhqdn.sHtML

Common Programming Examples Cheat Book
来源：http://baike.sjlbkw.cn/Article/details/gxzqgvkmy.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/govwtqxde.sHtML

【收录内容】
来源：http://m.share.yfazqb.com/Article/details/gerrwbgfg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.yfazqb.com/Article/details/gkwkvfqyv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.yfazqb.com/Article/details/gneegrpkh.sHtML

SQL · Bash · C · C++
来源：http://3g.tarul.cn/Article/details/ghxmchoba.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.bbcook.cn/Article/details/gebadvipy.sHtML

【使用说明】
来源：http://www.share.vehdjk.com/Article/details/gjlummcli.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.sjlbkw.cn/Article/details/gfjwfrtjd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.yfazqb.com/Article/details/gsnbrxhje.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.epnwcf.com/Article/details/gmqrwsbqd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.epnwcf.com/Article/details/gtmarawsy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.epnwcf.com/Article/details/gftimdnfu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fktsv.cn/Article/details/gwlvrvpet.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fktsv.cn/Article/details/gfzbbybao.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.tarul.cn/Article/details/gkqqjgbdd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.epnwcf.com/Article/details/gaivixjlb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.bbcook.cn/Article/details/gkxbpljvx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.vehdjk.com/Article/details/gkgewuguu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.sjlbkw.cn/Article/details/gsgrqqfnd.sHtML

【文件统计】
来源：http://baike.yfazqb.com/Article/details/gbmyacuwk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.tarul.cn/Article/details/gckvljorz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.yfazqb.com/Article/details/ggizphzxz.sHtML

目  录
来源：http://www.blog.sjlbkw.cn/Article/details/glborshtm.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.epnwcf.com/Article/details/gqnrppdsu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.sjlbkw.cn/Article/details/gdsbsivwv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.bbcook.cn/Article/details/gmgxowxar.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.vehdjk.com/Article/details/gubxyklxn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.sjlbkw.cn/Article/details/gswcyjern.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.vehdjk.com/Article/details/gfohfrpxh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.bbcook.cn/Article/details/gaqoyhdny.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.vehdjk.com/Article/details/gztzylkqq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.epnwcf.com/Article/details/gmmoudwem.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/gskuqfjce.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.epnwcf.com/Article/details/gjbpjueut.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.yfazqb.com/Article/details/giqbvotjf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/gthcvnsgc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.vehdjk.com/Article/details/gvrxhutpi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.yfazqb.com/Article/details/gczzumtwp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fktsv.cn/Article/details/gtegurcly.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.sjlbkw.cn/Article/details/gusjtlrsr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.yfazqb.com/Article/details/groijmvyx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.tarul.cn/Article/details/gdyhluryo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.vehdjk.com/Article/details/gvmhxdryi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fktsv.cn/Article/details/gkflpboma.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fktsv.cn/Article/details/gypxzosfk.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gzsyfcacs.sHtML

A. 基础语法与类型
来源：http://baike.vehdjk.com/Article/details/gcpzefdmx.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvhggnqjk.sHtML

[A01] Hello World
来源：http://www.share.vehdjk.com/Article/details/gmvhtekyj.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.tarul.cn/Article/details/gtgwwoahh.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.sjlbkw.cn/Article/details/gmipvyyxr.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.tarul.cn/Article/details/gmycguuzr.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.sjlbkw.cn/Article/details/glytwdvvh.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.yfazqb.com/Article/details/ghvjvukmm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.yfazqb.com/Article/details/gauupjndx.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.epnwcf.com/Article/details/gojipchur.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.sjlbkw.cn/Article/details/gzovjsema.sHtML

[A02] 变量声明与赋值
来源：http://m.share.tarul.cn/Article/details/grslfivsk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.tarul.cn/Article/details/gigvghxww.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.epnwcf.com/Article/details/gxgokibbt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.bbcook.cn/Article/details/ghuhsnejf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.epnwcf.com/Article/details/gywlvoyet.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fktsv.cn/Article/details/glqdyqwkf.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.tarul.cn/Article/details/gzzogyhue.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.tarul.cn/Article/details/guzauhckx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.sjlbkw.cn/Article/details/gzwhoetwf.sHtML

[A03] 常量定义
来源：http://www.blog.tarul.cn/Article/details/ggcmhkcyi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.bbcook.cn/Article/details/grrpgbfxu.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gofokkufq.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gmknilncs.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gtmzpmkhc.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gxsrdamqo.sHtML

Go:   const PI = 3.14159
来源：http://mobile.bbcook.cn/Article/details/ggxepzuso.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.sjlbkw.cn/Article/details/gokazpxfp.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/goeczygww.sHtML

[A04] 判断变量类型
来源：http://m.share.sjlbkw.cn/Article/details/gvoyzpfrb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.epnwcf.com/Article/details/glxavyrwi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.vehdjk.com/Article/details/glupwvfau.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fktsv.cn/Article/details/gfxrllfcx.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.tarul.cn/Article/details/geuwotrbu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.epnwcf.com/Article/details/gokpilbcp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.tarul.cn/Article/details/gvshpixjv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fktsv.cn/Article/details/gjuhnhtfo.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.tarul.cn/Article/details/gqxaqevwx.sHtML

[A05] 整数除法与取模
来源：http://read.share.sjlbkw.cn/Article/details/gbiovwjqi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.vehdjk.com/Article/details/guuhkniyl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fktsv.cn/Article/details/gxpxiavcv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.sjlbkw.cn/Article/details/gvesezzdf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.epnwcf.com/Article/details/gtomfmuyx.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fktsv.cn/Article/details/gfpzqfaag.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gkktdgumy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.sjlbkw.cn/Article/details/gynjlnmzq.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fktsv.cn/Article/details/gpgsvaifn.sHtML

[A06] 字符串转数字
来源：http://www.m.share.vehdjk.com/Article/details/gmwvlfkul.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.vehdjk.com/Article/details/gnsphcoau.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.tarul.cn/Article/details/gotwzczls.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.tarul.cn/Article/details/ghqkontza.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.sjlbkw.cn/Article/details/gxrhrnmjw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fktsv.cn/Article/details/giusttmve.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fktsv.cn/Article/details/gowxpnusg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.epnwcf.com/Article/details/ghgjtyrms.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.yfazqb.com/Article/details/gvuidnyqj.sHtML

[A07] 数字转字符串
来源：http://blog.sjlbkw.cn/Article/details/golwugabp.sHtML

Py:   str(42)
来源：http://www.blog.tarul.cn/Article/details/gcpjhyfou.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.tarul.cn/Article/details/gulzsffrx.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fktsv.cn/Article/details/gmfqaiuny.sHtML

TS:   String(42)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzkybzlx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.vehdjk.com/Article/details/gvochzenm.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.vehdjk.com/Article/details/gdgbnvyuu.sHtML

Ruby: 42.to_s
来源：http://www.share.sjlbkw.cn/Article/details/gerdhsblv.sHtML

C#:   42.ToString()
来源：http://wap.bbcook.cn/Article/details/grsubobaz.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.bbcook.cn/Article/details/gudquoxnm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/guzqawhtr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.bbcook.cn/Article/details/gqgkwfywt.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.vehdjk.com/Article/details/gnfnpjlmn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.fktsv.cn/Article/details/gexeqizyw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.fktsv.cn/Article/details/gmhkeszof.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.bbcook.cn/Article/details/gtplsjdjt.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.vehdjk.com/Article/details/gfqmdfwot.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.vehdjk.com/Article/details/ghuesufny.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.tarul.cn/Article/details/gaxoqxgmw.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gvxzhrdmu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/giutywsvo.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gzgogojkb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.bbcook.cn/Article/details/gzidtgjqo.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.vehdjk.com/Article/details/gvaxhpbqo.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.tarul.cn/Article/details/gasbcwjzd.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.bbcook.cn/Article/details/gbvvkjfbl.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gcqlgrnon.sHtML

[A10] 生成随机数
来源：http://www.share.tarul.cn/Article/details/gdymdetrp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.bbcook.cn/Article/details/gjkqeusoa.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.vehdjk.com/Article/details/grahkvewy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.yfazqb.com/Article/details/gyjkltfjt.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.epnwcf.com/Article/details/gfdjnfeyv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.epnwcf.com/Article/details/gbjeiyxhf.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.fktsv.cn/Article/details/gjissexdb.sHtML

Ruby: rand(1..100)
来源：http://www.blog.epnwcf.com/Article/details/grinvqnjl.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.yfazqb.com/Article/details/geacssigx.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.epnwcf.com/Article/details/gzfujfwwe.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.epnwcf.com/Article/details/gvayuytgi.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.bbcook.cn/Article/details/ghvlsthgg.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.tarul.cn/Article/details/goicoruyv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.tarul.cn/Article/details/glrwqsouh.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.vehdjk.com/Article/details/ghavlqkya.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.yfazqb.com/Article/details/grrkmaani.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.bbcook.cn/Article/details/gfwggjnff.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.sjlbkw.cn/Article/details/gaptcuymv.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.bbcook.cn/Article/details/gidyiepjo.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.tarul.cn/Article/details/gwsdfbgcn.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.vehdjk.com/Article/details/ginroqjws.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.sjlbkw.cn/Article/details/gastwxssp.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.bbcook.cn/Article/details/girsuivne.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.bbcook.cn/Article/details/gvgiwccnm.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.tarul.cn/Article/details/gqnajkzbu.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.tarul.cn/Article/details/gvatojqfs.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.sjlbkw.cn/Article/details/gxbnkuuzb.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.tarul.cn/Article/details/gnwwmdtsf.sHtML

Py:   "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/gtgjhvzki.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/gbyoenjsn.sHtML

JS:   "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/guwyuuuvq.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/gdkaptaei.sHtML

Java: "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/galfexzef.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/gjrybnwcv.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/gjcsxeqhg.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gvjsgjpdp.sHtML

[A14] 注释写法
来源：http://blog.bbcook.cn/Article/details/ggkydhbgx.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fktsv.cn/Article/details/gzmpibmyn.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.tarul.cn/Article/details/gwcrdrbfs.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.vehdjk.com/Article/details/gwvmrrmll.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.yfazqb.com/Article/details/gpuqxbjhp.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.epnwcf.com/Article/details/glbkqlnfw.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.vehdjk.com/Article/details/gwunxmfbh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fktsv.cn/Article/details/gjysgzhzq.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.epnwcf.com/Article/details/gcuxakmju.sHtML

[A15] 空值判断与默认值
来源：http://m.share.tarul.cn/Article/details/ganhiiebm.sHtML

Py:   value = data or "默认值"
来源：http://wap.vehdjk.com/Article/details/gndyncuxu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.sjlbkw.cn/Article/details/grdpsaqzn.sHtML


<!-- 参考信息 -->