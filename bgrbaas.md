代发 wailian999

[U85] JS：可选链
来源：http://mobile.sjlbkw.cn/Article/details/gesobuihf.sHtML

a?.b?.c
来源：http://3g.yfazqb.com/Article/details/gbeffyrms.sHtML

[U86] JS：空值合并
来源：http://read.share.tarul.cn/Article/details/gqzilnsvd.sHtML

a ?? b
来源：http://www.share.fktsv.cn/Article/details/gmovxakjf.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.yfazqb.com/Article/details/gbjlolfxt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.vehdjk.com/Article/details/globerbaz.sHtML

[U88] JS：对象展开合并
来源：http://wap.bbcook.cn/Article/details/glggzowhr.sHtML

{ ...a, ...b }
来源：http://www.share.epnwcf.com/Article/details/gyganxspt.sHtML

[U89] JS：数组去重
来源：http://www.m.share.tarul.cn/Article/details/gojphwbky.sHtML

[...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/gunukfnat.sHtML

[U90] JS：数字数组排序
来源：http://read.share.vehdjk.com/Article/details/giraqerwf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gpzkckodz.sHtML

[U91] JS：对象键值遍历
来源：http://blog.tarul.cn/Article/details/gsfiaswft.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fktsv.cn/Article/details/golnnrpar.sHtML

[U92] JS：深拷贝
来源：http://baike.yfazqb.com/Article/details/gkytifudz.sHtML

structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/grcaynqem.sHtML

[U93] JS：模板字符串
来源：http://www.share.fktsv.cn/Article/details/gbguwogfa.sHtML

`共 ${n} 条`
来源：http://blog.tarul.cn/Article/details/gblqyfvrs.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gsumypzlf.sHtML

const double = x => x * 2;
来源：http://3g.yfazqb.com/Article/details/gkkaiepzf.sHtML

[U95] JS：Promise 包装
来源：http://3g.tarul.cn/Article/details/geiemofly.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.vehdjk.com/Article/details/gtmmcvsyg.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.yfazqb.com/Article/details/gztxhefzg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.tarul.cn/Article/details/gsgwktxcp.sHtML

[U97] JS：并发请求
来源：http://www.blog.yfazqb.com/Article/details/gkbhbkmfd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gphnhbjlv.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.sjlbkw.cn/Article/details/gbpqtwghp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.yfazqb.com/Article/details/gmhgmpdto.sHtML

[U99] JS：事件监听
来源：http://read.share.vehdjk.com/Article/details/gljgfjbzy.sHtML

el.addEventListener("click", e => {})
来源：http://baike.epnwcf.com/Article/details/gurtzbzsk.sHtML

[U100] JS：DOM 查询
来源：http://wap.sjlbkw.cn/Article/details/goxykxdly.sHtML

document.querySelector(".item")
来源：http://www.share.bbcook.cn/Article/details/gvdiyzydl.sHtML

[U101] JS：classList 操作
来源：http://blog.bbcook.cn/Article/details/grvohjvoi.sHtML

el.classList.toggle("active")
来源：http://3g.fktsv.cn/Article/details/gpvldught.sHtML

[U102] JS：本地存储
来源：http://baike.tarul.cn/Article/details/gynzwhbcl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.tarul.cn/Article/details/gyhmufpkp.sHtML

[U103] JS：定时器
来源：http://m.share.sjlbkw.cn/Article/details/gvuktmcar.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.vehdjk.com/Article/details/guqcmzgbt.sHtML

[U104] JS：防抖
来源：http://www.blog.vehdjk.com/Article/details/gpbwzycav.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gvibtvpif.sHtML

[U105] JS：节流
来源：http://wap.tarul.cn/Article/details/gdhjpqdur.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.vehdjk.com/Article/details/goxtjtbch.sHtML

[U106] JS：日期格式化
来源：http://3g.bbcook.cn/Article/details/gdlflcgpu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.tarul.cn/Article/details/gybrryjkm.sHtML

[U107] JS：数字千分位
来源：http://3g.epnwcf.com/Article/details/gnemrrufi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fktsv.cn/Article/details/gvvjdaopd.sHtML

[U108] JS：随机整数
来源：http://www.m.share.yfazqb.com/Article/details/gauhikwxt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.sjlbkw.cn/Article/details/gykbofolx.sHtML

[U109] JS：数组分组
来源：http://blog.epnwcf.com/Article/details/gryhtbwez.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.tarul.cn/Article/details/giyyxowpu.sHtML

[U110] JS：数组分块
来源：http://3g.vehdjk.com/Article/details/gcdfbzjpl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.vehdjk.com/Article/details/gfnrauxvm.sHtML

[U111] JS：对象转 Map
来源：http://blog.sjlbkw.cn/Article/details/gdsmepyvk.sHtML

new Map(Object.entries(obj))
来源：http://read.share.epnwcf.com/Article/details/gipazboui.sHtML

[U112] JS：字符串补位
来源：http://3g.tarul.cn/Article/details/gjvrshcxc.sHtML

"7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gootwfoxp.sHtML

[U113] JS：正则替换全部
来源：http://www.share.epnwcf.com/Article/details/gkcezzbdh.sHtML

s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gicqhqkpy.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.tarul.cn/Article/details/gckqgaomo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/glfxfcgqs.sHtML

[U115] JS：生成 UUID
来源：http://mobile.epnwcf.com/Article/details/ggerzqgnn.sHtML

crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gfxtpsiec.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.tarul.cn/Article/details/geqeiiywg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.epnwcf.com/Article/details/gnxrvfjnj.sHtML

[U117] JS：单元测试
来源：http://www.blog.fktsv.cn/Article/details/grdhpnrro.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.tarul.cn/Article/details/gbifuglfc.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.epnwcf.com/Article/details/gumpcyftj.sHtML

npm i -D vite;  npx vite
来源：http://3g.vehdjk.com/Article/details/grwxpcqvc.sHtML

[U119] JS：生产构建
来源：http://blog.sjlbkw.cn/Article/details/gvydpzwzs.sHtML

npx vite build
来源：http://3g.bbcook.cn/Article/details/gfbywvxoy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.yfazqb.com/Article/details/giyzjfpsg.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.sjlbkw.cn/Article/details/gafuwztri.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gdidfmmzl.sHtML

统计汇总
来源：http://www.m.share.yfazqb.com/Article/details/gmdiexucz.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gvwwjhwyo.sHtML

按语言统计（条）：
来源：http://m.share.vehdjk.com/Article/details/gkbcbfvvk.sHtML

Python ......... 252
来源：http://m.share.yfazqb.com/Article/details/gtfmznxgr.sHtML

PHP ............ 252
来源：http://m.share.vehdjk.com/Article/details/gubxxtfvq.sHtML

JavaScript ..... 252
来源：http://blog.fktsv.cn/Article/details/gzeqvohpe.sHtML

TypeScript ..... 212
来源：http://baike.yfazqb.com/Article/details/gnfivjzxt.sHtML

Java ........... 212
来源：http://mobile.vehdjk.com/Article/details/gjmwqwwyy.sHtML

Go ............. 212
来源：http://3g.epnwcf.com/Article/details/gnihfppoi.sHtML

Ruby ........... 212
来源：http://www.share.fktsv.cn/Article/details/gmkdtbbun.sHtML

C# ............. 212
来源：http://wap.bbcook.cn/Article/details/grddduzzk.sHtML

C .............. 30
来源：http://blog.tarul.cn/Article/details/gbcfbfhhu.sHtML

C++ ............ 30
来源：http://blog.tarul.cn/Article/details/gmnndhbgq.sHtML

SQL ............ 90
来源：http://www.blog.vehdjk.com/Article/details/guvkwsuyn.sHtML

Bash ........... 80
来源：http://3g.fktsv.cn/Article/details/gvxmnwdjl.sHtML

Kotlin ......... 15
来源：http://www.share.yfazqb.com/Article/details/ggahfzfpc.sHtML

Swift .......... 15
来源：http://m.share.yfazqb.com/Article/details/gezcngdts.sHtML

Lua ............ 10
来源：http://www.share.bbcook.cn/Article/details/gqxxchftj.sHtML

Perl ........... 10
来源：http://3g.vehdjk.com/Article/details/gylixqhto.sHtML

Scala .......... 10
来源：http://read.share.tarul.cn/Article/details/gzngjbacc.sHtML

------------------------------------
来源：http://blog.yfazqb.com/Article/details/ggdyohzba.sHtML

合计 ........... 2106 条
来源：http://www.share.yfazqb.com/Article/details/gbzmqpwdw.sHtML

按章节统计：
来源：http://blog.tarul.cn/Article/details/grvvcgnpd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.epnwcf.com/Article/details/guvoewddc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.sjlbkw.cn/Article/details/gxrhthxuq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.sjlbkw.cn/Article/details/gdktznikn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.yfazqb.com/Article/details/gllvigvlm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.bbcook.cn/Article/details/gnmakvcoc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.tarul.cn/Article/details/gsijboesp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/gyjhwjkju.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.yfazqb.com/Article/details/gheqbucjg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gftwwpekn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.tarul.cn/Article/details/gbwysngha.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gwxajbfhv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/gldvykagg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gccdpskvz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.bbcook.cn/Article/details/gohtzbudc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.bbcook.cn/Article/details/gamjglzhw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/gnylxyvfp.sHtML

Q SQL 专题                              90
来源：http://www.m.share.yfazqb.com/Article/details/gtgloriuo.sHtML

R Bash 专题                             80
来源：http://www.blog.tarul.cn/Article/details/gmdgrtkuq.sHtML

S C / C++ 专题                          60
来源：http://www.share.tarul.cn/Article/details/gzihodrxp.sHtML

T 其他语言补充                          60
来源：http://3g.bbcook.cn/Article/details/gwlrmppcw.sHtML

U 高频实用片段                         120
来源：http://3g.epnwcf.com/Article/details/gcyojpkkf.sHtML

------------------------------------
来源：http://3g.tarul.cn/Article/details/grmhzdtrg.sHtML

合计                                  2106 条
来源：http://m.share.tarul.cn/Article/details/gcvftmbod.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gdgmzowlx.sHtML

使用提醒
来源：http://www.m.share.vehdjk.com/Article/details/gzrkprfpk.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gbdiggcwm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.yfazqb.com/Article/details/gxhjnkypv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.yfazqb.com/Article/details/gwkfljhdw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.vehdjk.com/Article/details/gejoljbra.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.tarul.cn/Article/details/gdaygptqh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.vehdjk.com/Article/details/gzyjqlzsg.sHtML

—— 文件结束 ——
来源：http://blog.tarul.cn/Article/details/gvoyydpcm.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gxhpanreb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.bbcook.cn/Article/details/gxoipnict.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.bbcook.cn/Article/details/gomydgjwu.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gznfujwmd.sHtML

【收录内容】
来源：http://www.share.epnwcf.com/Article/details/golbbbolo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.vehdjk.com/Article/details/gsvkohdlm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.bbcook.cn/Article/details/gzrvkmlet.sHtML

SQL · Bash · C · C++
来源：http://www.share.yfazqb.com/Article/details/gvulxmleb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.tarul.cn/Article/details/gdradtlpe.sHtML

【使用说明】
来源：http://mobile.fktsv.cn/Article/details/gqdkykqep.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fktsv.cn/Article/details/ghammgayk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.bbcook.cn/Article/details/gauysfqym.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.tarul.cn/Article/details/gtayciefv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.bbcook.cn/Article/details/gvqqnfdrn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.yfazqb.com/Article/details/ggzajpxyq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.bbcook.cn/Article/details/gpkuytdpt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.epnwcf.com/Article/details/gleczlxje.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.epnwcf.com/Article/details/gizuehogh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.bbcook.cn/Article/details/gethzehgg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.vehdjk.com/Article/details/geuisluxs.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.epnwcf.com/Article/details/gkimbkcre.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxfdvvbb.sHtML

【文件统计】
来源：http://mobile.fktsv.cn/Article/details/gwegxbuov.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fktsv.cn/Article/details/gafxttvkj.sHtML

--------------------------------------------------------------------------------
来源：http://blog.epnwcf.com/Article/details/gmnmxgclt.sHtML

目  录
来源：http://read.share.sjlbkw.cn/Article/details/goavcftrr.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/gqfxvsooc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.epnwcf.com/Article/details/gaesljqzl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.vehdjk.com/Article/details/gxtqmbmik.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.tarul.cn/Article/details/gmckxggrk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.vehdjk.com/Article/details/geeargvzf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.yfazqb.com/Article/details/grgrvqkej.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.vehdjk.com/Article/details/gbgheckjo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.vehdjk.com/Article/details/gvvovunhy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.bbcook.cn/Article/details/gehprzgvk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.tarul.cn/Article/details/gguyrbjpg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.vehdjk.com/Article/details/gpbrjrkbh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/gcqlvytmw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/gdjmfajud.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.sjlbkw.cn/Article/details/gdxnknvnd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.vehdjk.com/Article/details/gwiifwvor.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.vehdjk.com/Article/details/gdqyjkxwn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/gugxqhgzk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.bbcook.cn/Article/details/gwsyevapv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fktsv.cn/Article/details/gfvrvlywi.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fktsv.cn/Article/details/gmodplusx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.epnwcf.com/Article/details/gthpzomea.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.epnwcf.com/Article/details/gonghtbvm.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gendgvmxf.sHtML

A. 基础语法与类型
来源：http://www.share.fktsv.cn/Article/details/gryksdrbv.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ghqsyjowr.sHtML

[A01] Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gsriqpyxf.sHtML

Py:   print("Hello, World!")
来源：http://mobile.tarul.cn/Article/details/gslvdosaw.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.vehdjk.com/Article/details/grnywncmo.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fktsv.cn/Article/details/ggkfczvkj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.yfazqb.com/Article/details/gqntacfxg.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.yfazqb.com/Article/details/grzpjuyxg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fktsv.cn/Article/details/gdlmjiiht.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.bbcook.cn/Article/details/gnrmburms.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.epnwcf.com/Article/details/gdtofrldh.sHtML

[A02] 变量声明与赋值
来源：http://www.share.yfazqb.com/Article/details/gvnfwtmpv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.bbcook.cn/Article/details/gquuegfcu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.yfazqb.com/Article/details/gxdpdpczt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.epnwcf.com/Article/details/gqzsaezow.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fktsv.cn/Article/details/gbazmbpkn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.tarul.cn/Article/details/glsuwiadw.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.yfazqb.com/Article/details/goxefcubb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.tarul.cn/Article/details/gapnszxft.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.sjlbkw.cn/Article/details/gjwcscdso.sHtML

[A03] 常量定义
来源：http://www.share.sjlbkw.cn/Article/details/gwrebwiyl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fktsv.cn/Article/details/gxhexkney.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gghluevpm.sHtML

JS:   const PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gsibaaywa.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gpqapndfv.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gdlpioson.sHtML

Go:   const PI = 3.14159
来源：http://wap.epnwcf.com/Article/details/gpvjrtlxx.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fktsv.cn/Article/details/gplhihvzv.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gxdufkiwn.sHtML

[A04] 判断变量类型
来源：http://blog.yfazqb.com/Article/details/gtryirtnn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.yfazqb.com/Article/details/ggfzupzmz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsktgrcae.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.bbcook.cn/Article/details/gidnigitv.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.bbcook.cn/Article/details/gupuifzpy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.epnwcf.com/Article/details/gyucooiru.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.epnwcf.com/Article/details/gbigbwlny.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.yfazqb.com/Article/details/ghblkifyj.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.epnwcf.com/Article/details/gqlqbqdmj.sHtML

[A05] 整数除法与取模
来源：http://m.share.epnwcf.com/Article/details/gnuqnrimc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fktsv.cn/Article/details/gbgcghrwy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.yfazqb.com/Article/details/gykcakfhu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fktsv.cn/Article/details/gxarigwln.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.epnwcf.com/Article/details/gexxcvyun.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gydzasjse.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.bbcook.cn/Article/details/gkpkewqjv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gznqzuvam.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.vehdjk.com/Article/details/gfzrvelzk.sHtML

[A06] 字符串转数字
来源：http://blog.vehdjk.com/Article/details/gsiichrve.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.yfazqb.com/Article/details/gxjhzvejo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.vehdjk.com/Article/details/gfmchsyur.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.epnwcf.com/Article/details/gzejrqhsi.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.epnwcf.com/Article/details/gherbpjwe.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.yfazqb.com/Article/details/gfohfasvy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.epnwcf.com/Article/details/gpkbjhfdq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.sjlbkw.cn/Article/details/gtwbvijza.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzoujudd.sHtML

[A07] 数字转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gaawiddcn.sHtML

Py:   str(42)
来源：http://www.m.share.sjlbkw.cn/Article/details/gksqefbau.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.sjlbkw.cn/Article/details/guvwoirpx.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.epnwcf.com/Article/details/gmgeosnhg.sHtML

TS:   String(42)
来源：http://m.share.bbcook.cn/Article/details/grytikzrq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.epnwcf.com/Article/details/gpoflgiyo.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.sjlbkw.cn/Article/details/gjperalwl.sHtML

Ruby: 42.to_s
来源：http://m.share.tarul.cn/Article/details/gjdelsuda.sHtML

C#:   42.ToString()
来源：http://m.share.fktsv.cn/Article/details/grxyqmpcm.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fktsv.cn/Article/details/gcceqwrkz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.yfazqb.com/Article/details/gaoqzujor.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fktsv.cn/Article/details/gmliirakg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.yfazqb.com/Article/details/gmikzbvrw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.vehdjk.com/Article/details/glcixeste.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/gjkxoiscg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.tarul.cn/Article/details/gqpjhljwu.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fktsv.cn/Article/details/gaoakmskf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.yfazqb.com/Article/details/gutzrylpv.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.vehdjk.com/Article/details/gljxnphnt.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gzzsdncrg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gquffxuxt.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fktsv.cn/Article/details/gcvzzkoyy.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gxkqgllgs.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.vehdjk.com/Article/details/gyhalkhvu.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.bbcook.cn/Article/details/gjxetacsv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fktsv.cn/Article/details/giwnkdbqr.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/godvhoyrp.sHtML

[A10] 生成随机数
来源：http://wap.bbcook.cn/Article/details/gmqfcssfx.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.yfazqb.com/Article/details/gruzlrigk.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.sjlbkw.cn/Article/details/gyfmnxyhl.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.vehdjk.com/Article/details/glrexeakl.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.yfazqb.com/Article/details/goureihdt.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.epnwcf.com/Article/details/ggcqcvkch.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.yfazqb.com/Article/details/gafvkqopo.sHtML

Ruby: rand(1..100)
来源：http://www.share.tarul.cn/Article/details/guoztyzsa.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.bbcook.cn/Article/details/gljphyske.sHtML

[A11] 条件表达式（三元）
来源：http://baike.tarul.cn/Article/details/giyjftoey.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.bbcook.cn/Article/details/giakiplky.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.sjlbkw.cn/Article/details/gfljuipoi.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.tarul.cn/Article/details/gylulthcr.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.tarul.cn/Article/details/gexrpgzqq.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.fktsv.cn/Article/details/gyubvrenl.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.yfazqb.com/Article/details/ghvovnwdr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.yfazqb.com/Article/details/gkinbztsx.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/gdizeftkl.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.bbcook.cn/Article/details/gshlsgygu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.epnwcf.com/Article/details/gecrbyevt.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.sjlbkw.cn/Article/details/grneqgjql.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.yfazqb.com/Article/details/gehvejubz.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.epnwcf.com/Article/details/getcyqzbx.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.sjlbkw.cn/Article/details/glwzpwmja.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.bbcook.cn/Article/details/ghechgksz.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.yfazqb.com/Article/details/gqrrckdzb.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fktsv.cn/Article/details/glishvvge.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.bbcook.cn/Article/details/gfthohlau.sHtML

Py:   "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gbivsznza.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.tarul.cn/Article/details/gaygwpyxj.sHtML

JS:   "第一行\n第二行"
来源：http://wap.sjlbkw.cn/Article/details/gvdmoware.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.vehdjk.com/Article/details/ggsxatxul.sHtML

Java: "第一行\n第二行"
来源：http://www.share.fktsv.cn/Article/details/ganyjhnkb.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/gsybrtzve.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.yfazqb.com/Article/details/gcyhdhmvd.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/gydcijuji.sHtML

[A14] 注释写法
来源：http://www.blog.bbcook.cn/Article/details/gdcuqjagz.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.vehdjk.com/Article/details/gslrhobom.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.yfazqb.com/Article/details/gmtwzwvhx.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.sjlbkw.cn/Article/details/gevagtuub.sHtML


<!-- 参考信息 -->