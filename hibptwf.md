代发 wailian999

[U87] JS：解构默认值
来源：http://3g.fktsv.cn/Article/details/gmcgkvncv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.bbcook.cn/Article/details/gggbhgech.sHtML

[U88] JS：对象展开合并
来源：http://3g.fktsv.cn/Article/details/gzmyjasdi.sHtML

{ ...a, ...b }
来源：http://www.m.share.tarul.cn/Article/details/gnpveuygs.sHtML

[U89] JS：数组去重
来源：http://baike.vehdjk.com/Article/details/gcwsljvkt.sHtML

[...new Set(arr)]
来源：http://mobile.tarul.cn/Article/details/gkzckttja.sHtML

[U90] JS：数字数组排序
来源：http://mobile.tarul.cn/Article/details/gzqipyvro.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/grefepfpa.sHtML

[U91] JS：对象键值遍历
来源：http://blog.epnwcf.com/Article/details/gfpxexzpw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.yfazqb.com/Article/details/grgkwpebo.sHtML

[U92] JS：深拷贝
来源：http://www.blog.vehdjk.com/Article/details/giyydiztq.sHtML

structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gxegwbqam.sHtML

[U93] JS：模板字符串
来源：http://read.share.tarul.cn/Article/details/guzatkbzk.sHtML

`共 ${n} 条`
来源：http://www.share.bbcook.cn/Article/details/guwxdekdx.sHtML

[U94] JS：箭头函数
来源：http://baike.epnwcf.com/Article/details/gewmsofha.sHtML

const double = x => x * 2;
来源：http://m.share.sjlbkw.cn/Article/details/ghjjtyjax.sHtML

[U95] JS：Promise 包装
来源：http://wap.vehdjk.com/Article/details/ggkkhmvgw.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fktsv.cn/Article/details/gawbcchbx.sHtML

[U96] JS：async/await 与异常
来源：http://blog.sjlbkw.cn/Article/details/glltcksaq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gnscnczdl.sHtML

[U97] JS：并发请求
来源：http://www.share.fktsv.cn/Article/details/ggumcbajo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gkfibqyya.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.yfazqb.com/Article/details/gxmroqzws.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.epnwcf.com/Article/details/gqfxogpja.sHtML

[U99] JS：事件监听
来源：http://blog.bbcook.cn/Article/details/gamsqlznz.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.bbcook.cn/Article/details/gqgxlzvon.sHtML

[U100] JS：DOM 查询
来源：http://www.share.sjlbkw.cn/Article/details/goyeitzea.sHtML

document.querySelector(".item")
来源：http://read.share.bbcook.cn/Article/details/gflwhbdqx.sHtML

[U101] JS：classList 操作
来源：http://wap.epnwcf.com/Article/details/gksdwyjxj.sHtML

el.classList.toggle("active")
来源：http://www.share.vehdjk.com/Article/details/gmgpczvts.sHtML

[U102] JS：本地存储
来源：http://mobile.fktsv.cn/Article/details/goyomllvc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.tarul.cn/Article/details/ghwbrdwhx.sHtML

[U103] JS：定时器
来源：http://baike.vehdjk.com/Article/details/gxnvludum.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.yfazqb.com/Article/details/gcgxupsrm.sHtML

[U104] JS：防抖
来源：http://read.share.yfazqb.com/Article/details/gubabimoq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/gvampwomg.sHtML

[U105] JS：节流
来源：http://www.m.share.tarul.cn/Article/details/guxkqwkuc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.bbcook.cn/Article/details/gxojfirkj.sHtML

[U106] JS：日期格式化
来源：http://www.share.tarul.cn/Article/details/gjtmszzak.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fktsv.cn/Article/details/grsybhlot.sHtML

[U107] JS：数字千分位
来源：http://3g.fktsv.cn/Article/details/gmycutisc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.epnwcf.com/Article/details/gptqofngp.sHtML

[U108] JS：随机整数
来源：http://wap.epnwcf.com/Article/details/gnggcikdd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.epnwcf.com/Article/details/gnflbiwdq.sHtML

[U109] JS：数组分组
来源：http://blog.sjlbkw.cn/Article/details/gvmuyaljt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.epnwcf.com/Article/details/gbghjfkjd.sHtML

[U110] JS：数组分块
来源：http://read.share.sjlbkw.cn/Article/details/gkuartzyg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.epnwcf.com/Article/details/gxvtrhqcr.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fktsv.cn/Article/details/gayjkdbwx.sHtML

new Map(Object.entries(obj))
来源：http://blog.bbcook.cn/Article/details/gnorfysdr.sHtML

[U112] JS：字符串补位
来源：http://wap.bbcook.cn/Article/details/gcgurokln.sHtML

"7".padStart(3, "0")
来源：http://wap.fktsv.cn/Article/details/gkhoqdqrv.sHtML

[U113] JS：正则替换全部
来源：http://blog.epnwcf.com/Article/details/gzyowkmvc.sHtML

s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gxxtzdsuy.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fktsv.cn/Article/details/gbhrevhin.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.vehdjk.com/Article/details/gzftrwvoi.sHtML

[U115] JS：生成 UUID
来源：http://baike.bbcook.cn/Article/details/gifelervu.sHtML

crypto.randomUUID()
来源：http://www.blog.vehdjk.com/Article/details/ggvfdsxbi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.sjlbkw.cn/Article/details/glounfmxi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.epnwcf.com/Article/details/gezghnbkk.sHtML

[U117] JS：单元测试
来源：http://www.m.share.tarul.cn/Article/details/gomszwcnz.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.vehdjk.com/Article/details/gihsnhmik.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.epnwcf.com/Article/details/gasphwjnc.sHtML

npm i -D vite;  npx vite
来源：http://www.share.yfazqb.com/Article/details/grqfgwrhr.sHtML

[U119] JS：生产构建
来源：http://baike.fktsv.cn/Article/details/gparfdnud.sHtML

npx vite build
来源：http://blog.sjlbkw.cn/Article/details/gihutncpk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.epnwcf.com/Article/details/gujjvhzyi.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.epnwcf.com/Article/details/grlvblmvh.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gzivlsifa.sHtML

统计汇总
来源：http://mobile.tarul.cn/Article/details/gxceyotoi.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gamggyqhn.sHtML

按语言统计（条）：
来源：http://www.blog.vehdjk.com/Article/details/gobkjzaof.sHtML

Python ......... 252
来源：http://www.m.share.epnwcf.com/Article/details/gqysxdxnr.sHtML

PHP ............ 252
来源：http://read.share.bbcook.cn/Article/details/ghthtzerx.sHtML

JavaScript ..... 252
来源：http://mobile.sjlbkw.cn/Article/details/ghlyfcpzn.sHtML

TypeScript ..... 212
来源：http://baike.epnwcf.com/Article/details/glpdhmwtw.sHtML

Java ........... 212
来源：http://blog.epnwcf.com/Article/details/gvahhqcwo.sHtML

Go ............. 212
来源：http://baike.tarul.cn/Article/details/gedbgenoh.sHtML

Ruby ........... 212
来源：http://read.share.vehdjk.com/Article/details/gdzoffxzn.sHtML

C# ............. 212
来源：http://www.blog.fktsv.cn/Article/details/gaoqohldm.sHtML

C .............. 30
来源：http://baike.yfazqb.com/Article/details/gwgfdjvbo.sHtML

C++ ............ 30
来源：http://www.share.yfazqb.com/Article/details/gfpcbpkyx.sHtML

SQL ............ 90
来源：http://read.share.sjlbkw.cn/Article/details/gmzllwfcd.sHtML

Bash ........... 80
来源：http://3g.fktsv.cn/Article/details/gthmbpmvg.sHtML

Kotlin ......... 15
来源：http://3g.sjlbkw.cn/Article/details/geqrkiyyw.sHtML

Swift .......... 15
来源：http://blog.fktsv.cn/Article/details/ghemrrqra.sHtML

Lua ............ 10
来源：http://www.blog.bbcook.cn/Article/details/gobqzltbi.sHtML

Perl ........... 10
来源：http://www.share.fktsv.cn/Article/details/gajkhwazq.sHtML

Scala .......... 10
来源：http://wap.fktsv.cn/Article/details/gozurvmam.sHtML

------------------------------------
来源：http://3g.yfazqb.com/Article/details/gafnqtjdp.sHtML

合计 ........... 2106 条
来源：http://baike.epnwcf.com/Article/details/gcdnyyoog.sHtML

按章节统计：
来源：http://mobile.epnwcf.com/Article/details/gnyqdomlc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.bbcook.cn/Article/details/giwhffsml.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.tarul.cn/Article/details/gclxcejlc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fktsv.cn/Article/details/gvvanwpxc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.yfazqb.com/Article/details/gvkppnzgt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.tarul.cn/Article/details/gimffppyz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.yfazqb.com/Article/details/gucvgmdyp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.sjlbkw.cn/Article/details/gumkkttld.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.epnwcf.com/Article/details/gezqjyvqd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.epnwcf.com/Article/details/gdbaqflxw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.sjlbkw.cn/Article/details/gogchodek.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/gxphzottm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gwyzmeirh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/gqgmqwcbf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.tarul.cn/Article/details/gokqmvpcs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.epnwcf.com/Article/details/ggnigfkji.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/guttgxzwc.sHtML

Q SQL 专题                              90
来源：http://m.share.tarul.cn/Article/details/gdkqxgtoy.sHtML

R Bash 专题                             80
来源：http://www.m.share.vehdjk.com/Article/details/gzqaesaji.sHtML

S C / C++ 专题                          60
来源：http://www.share.yfazqb.com/Article/details/gknrulwjp.sHtML

T 其他语言补充                          60
来源：http://read.share.tarul.cn/Article/details/gdlbbsqxy.sHtML

U 高频实用片段                         120
来源：http://www.share.epnwcf.com/Article/details/guyhbmlct.sHtML

------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/ggksrrblw.sHtML

合计                                  2106 条
来源：http://baike.epnwcf.com/Article/details/gfrtgniua.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gejumqenl.sHtML

使用提醒
来源：http://www.share.fktsv.cn/Article/details/gbheyddxk.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.epnwcf.com/Article/details/gwnhenhqy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.tarul.cn/Article/details/gsjsxtxsa.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.sjlbkw.cn/Article/details/guaqkrkls.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fktsv.cn/Article/details/gvgjcvugn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.sjlbkw.cn/Article/details/gyjoqanaw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.vehdjk.com/Article/details/govjcrxav.sHtML

—— 文件结束 ——
来源：http://mobile.bbcook.cn/Article/details/glmqrwbxw.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gfstzuyvp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.sjlbkw.cn/Article/details/gbudthwqw.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.bbcook.cn/Article/details/gbbknecsk.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gyfaialqm.sHtML

【收录内容】
来源：http://read.share.vehdjk.com/Article/details/grwvuppuw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.tarul.cn/Article/details/gwyndupvb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.sjlbkw.cn/Article/details/gxbvpszyg.sHtML

SQL · Bash · C · C++
来源：http://www.blog.vehdjk.com/Article/details/gtxvplasr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.epnwcf.com/Article/details/gkhszdccw.sHtML

【使用说明】
来源：http://baike.sjlbkw.cn/Article/details/gnudiyhgn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.epnwcf.com/Article/details/gvgwdfpee.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.epnwcf.com/Article/details/gnpppdlok.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.vehdjk.com/Article/details/gairduika.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.bbcook.cn/Article/details/gzdcrnleo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.epnwcf.com/Article/details/gjzntfugt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.yfazqb.com/Article/details/gdzdacmir.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.yfazqb.com/Article/details/grrlnhcjm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fktsv.cn/Article/details/gxryuyhpu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.vehdjk.com/Article/details/gocccqthk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.epnwcf.com/Article/details/gyqygiwxc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.sjlbkw.cn/Article/details/gmirnmydj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fktsv.cn/Article/details/gwqelznua.sHtML

【文件统计】
来源：http://m.share.yfazqb.com/Article/details/gjjnjvewi.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.bbcook.cn/Article/details/gghqtiram.sHtML

--------------------------------------------------------------------------------
来源：http://3g.epnwcf.com/Article/details/gqfmgpzbr.sHtML

目  录
来源：http://3g.fktsv.cn/Article/details/gzjijbzqd.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gjdqqvrsz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gcajlwcvf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.sjlbkw.cn/Article/details/grgedqorc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fktsv.cn/Article/details/ggvzmrxtu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.tarul.cn/Article/details/gvasmulmv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.bbcook.cn/Article/details/gmeqgrirj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.yfazqb.com/Article/details/goangwxgm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.yfazqb.com/Article/details/gmsawdciu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.bbcook.cn/Article/details/gtyrmxwct.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/ghoozimiq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.sjlbkw.cn/Article/details/gaqawyjpy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/gxwptqpfs.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/gjlqnwtse.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/gufxpvfzy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.epnwcf.com/Article/details/gmxyudsqj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.tarul.cn/Article/details/gajdytose.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/geiykrnhc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.yfazqb.com/Article/details/gssjifqim.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.sjlbkw.cn/Article/details/gwfatumbr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.epnwcf.com/Article/details/grjgmeqet.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.vehdjk.com/Article/details/gagpkgpnz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.vehdjk.com/Article/details/gdhvpwnwv.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gybzhmhku.sHtML

A. 基础语法与类型
来源：http://read.share.vehdjk.com/Article/details/gpbwqalls.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gcybckmgs.sHtML

[A01] Hello World
来源：http://mobile.yfazqb.com/Article/details/gevzmzsod.sHtML

Py:   print("Hello, World!")
来源：http://mobile.vehdjk.com/Article/details/gbfecnfez.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.yfazqb.com/Article/details/gytakzefc.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.bbcook.cn/Article/details/gaczauiye.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fktsv.cn/Article/details/grtqgvxht.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.epnwcf.com/Article/details/gpdleurae.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.tarul.cn/Article/details/gilulkedo.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.yfazqb.com/Article/details/gklueckho.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fktsv.cn/Article/details/gpgparivf.sHtML

[A02] 变量声明与赋值
来源：http://www.share.vehdjk.com/Article/details/giiaydfhj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fktsv.cn/Article/details/gkyyhwhsb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fktsv.cn/Article/details/gjbupnpep.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.epnwcf.com/Article/details/glmslwqmd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.yfazqb.com/Article/details/goumsbhhm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.sjlbkw.cn/Article/details/gnfwxalht.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.epnwcf.com/Article/details/gxjoistdk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.tarul.cn/Article/details/ghistdbjn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.sjlbkw.cn/Article/details/gioupuosh.sHtML

[A03] 常量定义
来源：http://blog.vehdjk.com/Article/details/gcyutrspj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.epnwcf.com/Article/details/gauvtxmvt.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gmadzvyyq.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gauimvvki.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.vehdjk.com/Article/details/giwlenopa.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/ggdkhhabs.sHtML

Go:   const PI = 3.14159
来源：http://www.share.sjlbkw.cn/Article/details/gcvgjbzjw.sHtML

Ruby: PI = 3.14159
来源：http://3g.yfazqb.com/Article/details/gmpsuwtmt.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/grcdvudqo.sHtML

[A04] 判断变量类型
来源：http://3g.yfazqb.com/Article/details/gyrgyzmip.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.tarul.cn/Article/details/gideyiquh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.tarul.cn/Article/details/gwksssgej.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.bbcook.cn/Article/details/gewpnybgh.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fktsv.cn/Article/details/gxcfqopol.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.epnwcf.com/Article/details/gctdqdytv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.sjlbkw.cn/Article/details/gbhjrirnj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.bbcook.cn/Article/details/gezjkrlva.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.tarul.cn/Article/details/geveykrje.sHtML

[A05] 整数除法与取模
来源：http://blog.sjlbkw.cn/Article/details/gcewejqvt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.vehdjk.com/Article/details/glgwbrhan.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.sjlbkw.cn/Article/details/gtgpwddfg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.yfazqb.com/Article/details/gjarpmmwo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/glgzvfros.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gfnkvtoyt.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.epnwcf.com/Article/details/goqmojpek.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.tarul.cn/Article/details/goyavaikn.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.bbcook.cn/Article/details/gzrbfxclq.sHtML

[A06] 字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gqhjiqgik.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.bbcook.cn/Article/details/gubgqllto.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.epnwcf.com/Article/details/gudfghdgl.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.bbcook.cn/Article/details/gbfelmwqm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.yfazqb.com/Article/details/gsivahuei.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fktsv.cn/Article/details/guamjegmr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.vehdjk.com/Article/details/gdhwnohcc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.sjlbkw.cn/Article/details/gtjdqowov.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.yfazqb.com/Article/details/gdgusoyqm.sHtML

[A07] 数字转字符串
来源：http://m.share.vehdjk.com/Article/details/gzcqtlvcx.sHtML

Py:   str(42)
来源：http://m.share.yfazqb.com/Article/details/gvprvekai.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.sjlbkw.cn/Article/details/gtgwaskqp.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.bbcook.cn/Article/details/gdyunpdcs.sHtML

TS:   String(42)
来源：http://mobile.bbcook.cn/Article/details/glohoiccj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.epnwcf.com/Article/details/glknlgqzl.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.bbcook.cn/Article/details/gvzyzwoni.sHtML

Ruby: 42.to_s
来源：http://3g.yfazqb.com/Article/details/gmvahuoua.sHtML

C#:   42.ToString()
来源：http://www.share.sjlbkw.cn/Article/details/gwjgbrkde.sHtML

[A08] 取整与四舍五入
来源：http://blog.bbcook.cn/Article/details/gliddaeww.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fktsv.cn/Article/details/guldeskui.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.vehdjk.com/Article/details/gjyfezzuy.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.bbcook.cn/Article/details/gopbemrgd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.tarul.cn/Article/details/gifgwslax.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fktsv.cn/Article/details/gbcctracp.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.bbcook.cn/Article/details/gwodlwxlm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.yfazqb.com/Article/details/ghxivhfwy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.tarul.cn/Article/details/gwdrplink.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.tarul.cn/Article/details/gynqyboip.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/gyltqejep.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.tarul.cn/Article/details/gcjypourz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.tarul.cn/Article/details/gsazrefzh.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gvqucoqem.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.yfazqb.com/Article/details/gpsdfzupg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.fktsv.cn/Article/details/gnvjerpbo.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.sjlbkw.cn/Article/details/gthhbisbl.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.fktsv.cn/Article/details/gkdhxgnic.sHtML

[A10] 生成随机数
来源：http://blog.fktsv.cn/Article/details/gzehcjerm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.tarul.cn/Article/details/gibvjfjdm.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.epnwcf.com/Article/details/gmeatfwbe.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.epnwcf.com/Article/details/gzusbqkyl.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fktsv.cn/Article/details/greienzsv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.yfazqb.com/Article/details/gxopqhoez.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.vehdjk.com/Article/details/gqjftdmmy.sHtML

Ruby: rand(1..100)
来源：http://mobile.fktsv.cn/Article/details/gpyiokipz.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.yfazqb.com/Article/details/grmrqqbaq.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.epnwcf.com/Article/details/glgjsnoqa.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.tarul.cn/Article/details/grbhirkmt.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fktsv.cn/Article/details/gasuplxfw.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.vehdjk.com/Article/details/gtwklsuef.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.yfazqb.com/Article/details/gtzstcrrg.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.tarul.cn/Article/details/gihbguszg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.vehdjk.com/Article/details/ggeajnzbr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.yfazqb.com/Article/details/gcddswysz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.sjlbkw.cn/Article/details/gylewfuyi.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.sjlbkw.cn/Article/details/gxeecrana.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.bbcook.cn/Article/details/gcfztvmzm.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.bbcook.cn/Article/details/glssxnmks.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.bbcook.cn/Article/details/gcmmejwrj.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.epnwcf.com/Article/details/glhyygwzw.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.bbcook.cn/Article/details/ghepoixrx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.vehdjk.com/Article/details/guaelvjbg.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.bbcook.cn/Article/details/ggtgtnqjy.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.yfazqb.com/Article/details/gnswfwwjv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fktsv.cn/Article/details/guwqldwuh.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.yfazqb.com/Article/details/gmsmosqga.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gcbbtwqai.sHtML

JS:   "第一行\n第二行"
来源：http://wap.vehdjk.com/Article/details/gtnsvpkaf.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.sjlbkw.cn/Article/details/gpvdowrif.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.bbcook.cn/Article/details/gstjilent.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/giufdcdak.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.yfazqb.com/Article/details/gchgvxuaz.sHtML

C#:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gmgmmpkql.sHtML

[A14] 注释写法
来源：http://read.share.epnwcf.com/Article/details/gkwmboqbk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fktsv.cn/Article/details/gvzzbpuib.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.bbcook.cn/Article/details/gyeronieb.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.epnwcf.com/Article/details/givdyifes.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.vehdjk.com/Article/details/gwpghbzdf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.epnwcf.com/Article/details/goeelwlcp.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fktsv.cn/Article/details/gysbwglaj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fktsv.cn/Article/details/gvehykeyi.sHtML


<!-- 参考信息 -->