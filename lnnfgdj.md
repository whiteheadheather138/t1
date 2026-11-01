代发 wailian999

[U89] JS：数组去重
来源：http://www.m.share.yfazqb.com/Article/details/gvxlevghf.sHtML

[...new Set(arr)]
来源：http://www.m.share.fktsv.cn/Article/details/gahfxsxxo.sHtML

[U90] JS：数字数组排序
来源：http://3g.tarul.cn/Article/details/gjkhwjmvp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/goicwfsdu.sHtML

[U91] JS：对象键值遍历
来源：http://wap.vehdjk.com/Article/details/gshwwzwuy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.yfazqb.com/Article/details/gjkzvitjz.sHtML

[U92] JS：深拷贝
来源：http://3g.fktsv.cn/Article/details/geboxnydz.sHtML

structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/gtyjhjwfe.sHtML

[U93] JS：模板字符串
来源：http://blog.epnwcf.com/Article/details/gpoktuoke.sHtML

`共 ${n} 条`
来源：http://blog.tarul.cn/Article/details/gczdqcodv.sHtML

[U94] JS：箭头函数
来源：http://www.share.fktsv.cn/Article/details/gvsgjefdu.sHtML

const double = x => x * 2;
来源：http://m.share.vehdjk.com/Article/details/grrinjsck.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.vehdjk.com/Article/details/gqiazkfyq.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.sjlbkw.cn/Article/details/gsqxfvrjv.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fktsv.cn/Article/details/gayldipcr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/gwtpxqowp.sHtML

[U97] JS：并发请求
来源：http://read.share.sjlbkw.cn/Article/details/gsiixgplp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gbbrnwglz.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.tarul.cn/Article/details/gdqfhdqkt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.epnwcf.com/Article/details/gozrutntp.sHtML

[U99] JS：事件监听
来源：http://www.blog.fktsv.cn/Article/details/gvqyhvoxl.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.epnwcf.com/Article/details/gzttvwnrr.sHtML

[U100] JS：DOM 查询
来源：http://m.share.vehdjk.com/Article/details/gbrubbptb.sHtML

document.querySelector(".item")
来源：http://baike.fktsv.cn/Article/details/gjofazzdy.sHtML

[U101] JS：classList 操作
来源：http://read.share.vehdjk.com/Article/details/gfjfjuflj.sHtML

el.classList.toggle("active")
来源：http://www.blog.tarul.cn/Article/details/gbttkcddd.sHtML

[U102] JS：本地存储
来源：http://read.share.bbcook.cn/Article/details/goxngtvpz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.bbcook.cn/Article/details/gsdxsidfy.sHtML

[U103] JS：定时器
来源：http://wap.epnwcf.com/Article/details/gwqcyfpzo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.yfazqb.com/Article/details/gcrwaiyze.sHtML

[U104] JS：防抖
来源：http://3g.tarul.cn/Article/details/gzdybjrca.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/gvawhuafy.sHtML

[U105] JS：节流
来源：http://mobile.epnwcf.com/Article/details/ggnhzjhol.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fktsv.cn/Article/details/gbekmzlpu.sHtML

[U106] JS：日期格式化
来源：http://baike.epnwcf.com/Article/details/geszeoxqz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.tarul.cn/Article/details/gkgpagcis.sHtML

[U107] JS：数字千分位
来源：http://mobile.bbcook.cn/Article/details/gfbdisvph.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.sjlbkw.cn/Article/details/gyrlxugyq.sHtML

[U108] JS：随机整数
来源：http://www.m.share.epnwcf.com/Article/details/gagiwnxxe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fktsv.cn/Article/details/gunhmqdst.sHtML

[U109] JS：数组分组
来源：http://m.share.bbcook.cn/Article/details/gmrdhyyxl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fktsv.cn/Article/details/gdyvqbwly.sHtML

[U110] JS：数组分块
来源：http://3g.epnwcf.com/Article/details/gnqfanjsc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fktsv.cn/Article/details/gwthfcton.sHtML

[U111] JS：对象转 Map
来源：http://m.share.sjlbkw.cn/Article/details/givcrynqi.sHtML

new Map(Object.entries(obj))
来源：http://wap.yfazqb.com/Article/details/gxafwgika.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.vehdjk.com/Article/details/gaifhyhtv.sHtML

"7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/gttjlelzf.sHtML

[U113] JS：正则替换全部
来源：http://3g.sjlbkw.cn/Article/details/ghvvrufqk.sHtML

s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gxpryfiop.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.vehdjk.com/Article/details/gatzjqxhp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.sjlbkw.cn/Article/details/galskctly.sHtML

[U115] JS：生成 UUID
来源：http://blog.epnwcf.com/Article/details/gaohwuduy.sHtML

crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gcuuvnhxf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.epnwcf.com/Article/details/glgugwiqe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.bbcook.cn/Article/details/gesmjiyem.sHtML

[U117] JS：单元测试
来源：http://m.share.yfazqb.com/Article/details/goqjfnyjm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.epnwcf.com/Article/details/ghroriuko.sHtML

[U118] JS：开发服务器
来源：http://baike.yfazqb.com/Article/details/gamkbkeep.sHtML

npm i -D vite;  npx vite
来源：http://mobile.bbcook.cn/Article/details/gmhuwprvs.sHtML

[U119] JS：生产构建
来源：http://baike.epnwcf.com/Article/details/gjougymkf.sHtML

npx vite build
来源：http://mobile.fktsv.cn/Article/details/gewtqsktc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.yfazqb.com/Article/details/gtnrmqbui.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fktsv.cn/Article/details/gcdfsmpby.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gjmounilq.sHtML

统计汇总
来源：http://www.blog.bbcook.cn/Article/details/gxfqootbd.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gzrlvyiwy.sHtML

按语言统计（条）：
来源：http://blog.vehdjk.com/Article/details/ggvyeyvxm.sHtML

Python ......... 252
来源：http://baike.bbcook.cn/Article/details/gbftmrxvh.sHtML

PHP ............ 252
来源：http://mobile.tarul.cn/Article/details/gzqzgdkar.sHtML

JavaScript ..... 252
来源：http://mobile.sjlbkw.cn/Article/details/gqcocafzx.sHtML

TypeScript ..... 212
来源：http://3g.sjlbkw.cn/Article/details/gqmxchile.sHtML

Java ........... 212
来源：http://read.share.sjlbkw.cn/Article/details/ganelofrq.sHtML

Go ............. 212
来源：http://read.share.tarul.cn/Article/details/gfbzlkpwd.sHtML

Ruby ........... 212
来源：http://read.share.tarul.cn/Article/details/gbvbiyill.sHtML

C# ............. 212
来源：http://www.blog.vehdjk.com/Article/details/gpdvlknde.sHtML

C .............. 30
来源：http://mobile.tarul.cn/Article/details/griqiettr.sHtML

C++ ............ 30
来源：http://wap.tarul.cn/Article/details/gjseusvzn.sHtML

SQL ............ 90
来源：http://3g.sjlbkw.cn/Article/details/ghtyhaclg.sHtML

Bash ........... 80
来源：http://www.blog.yfazqb.com/Article/details/gvwcaddem.sHtML

Kotlin ......... 15
来源：http://m.share.tarul.cn/Article/details/gtggrddqq.sHtML

Swift .......... 15
来源：http://m.share.tarul.cn/Article/details/gxtnhjiyg.sHtML

Lua ............ 10
来源：http://m.share.yfazqb.com/Article/details/gruproedr.sHtML

Perl ........... 10
来源：http://blog.tarul.cn/Article/details/guebhnpeg.sHtML

Scala .......... 10
来源：http://blog.bbcook.cn/Article/details/gqkoylxor.sHtML

------------------------------------
来源：http://baike.epnwcf.com/Article/details/gtopuojch.sHtML

合计 ........... 2106 条
来源：http://baike.sjlbkw.cn/Article/details/grsirisdc.sHtML

按章节统计：
来源：http://www.blog.fktsv.cn/Article/details/gfeuiruno.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.tarul.cn/Article/details/gdjimpbpb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gnerwnhju.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.sjlbkw.cn/Article/details/godozcqae.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.vehdjk.com/Article/details/gegormupb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.sjlbkw.cn/Article/details/gwsxzewux.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.yfazqb.com/Article/details/gdmempfel.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.tarul.cn/Article/details/gicejzkzf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.sjlbkw.cn/Article/details/gkdhlvarh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/gdmqyeyrn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fktsv.cn/Article/details/gnsxztryn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/gywfwfznv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/gfdiyhlkb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/glhpxcasr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.vehdjk.com/Article/details/gzcgntuct.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.yfazqb.com/Article/details/gnffilksu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fktsv.cn/Article/details/govipkick.sHtML

Q SQL 专题                              90
来源：http://mobile.vehdjk.com/Article/details/giavaanxt.sHtML

R Bash 专题                             80
来源：http://www.share.vehdjk.com/Article/details/gvucetiwu.sHtML

S C / C++ 专题                          60
来源：http://m.share.fktsv.cn/Article/details/gaycqxhlt.sHtML

T 其他语言补充                          60
来源：http://mobile.sjlbkw.cn/Article/details/gipdkzezh.sHtML

U 高频实用片段                         120
来源：http://mobile.yfazqb.com/Article/details/gxroixdla.sHtML

------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gvvruqqkx.sHtML

合计                                  2106 条
来源：http://www.m.share.epnwcf.com/Article/details/gqazwnyqi.sHtML

--------------------------------------------------------------------------------
来源：http://3g.bbcook.cn/Article/details/gkfiihpzz.sHtML

使用提醒
来源：http://www.share.fktsv.cn/Article/details/glqpzpksq.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.epnwcf.com/Article/details/ghllvpzpk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.tarul.cn/Article/details/gvttsfzze.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.yfazqb.com/Article/details/gtqmbdtqz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.sjlbkw.cn/Article/details/gvmoopapq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.bbcook.cn/Article/details/gzqunieaf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.tarul.cn/Article/details/gaukyayhb.sHtML

—— 文件结束 ——
来源：http://wap.bbcook.cn/Article/details/gkffzavyk.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gexztsooj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fktsv.cn/Article/details/gycqsvqaq.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.epnwcf.com/Article/details/gbvglqmau.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gxhorxwrv.sHtML

【收录内容】
来源：http://baike.bbcook.cn/Article/details/gmiynqxyz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.yfazqb.com/Article/details/gahtlaofb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.yfazqb.com/Article/details/grocexlfs.sHtML

SQL · Bash · C · C++
来源：http://mobile.sjlbkw.cn/Article/details/gskgsfprl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.vehdjk.com/Article/details/guxflftzx.sHtML

【使用说明】
来源：http://baike.vehdjk.com/Article/details/ggqyinncv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.yfazqb.com/Article/details/gsnlhjuay.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.vehdjk.com/Article/details/ghdijcvzh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.tarul.cn/Article/details/gkttxlnai.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.epnwcf.com/Article/details/gxypfubqv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.tarul.cn/Article/details/gmmmwywjd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.yfazqb.com/Article/details/gungozsyp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.yfazqb.com/Article/details/gnveuljfr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.vehdjk.com/Article/details/gicueqbzl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.yfazqb.com/Article/details/gngqtxzdd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.bbcook.cn/Article/details/gvpprpjfz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.bbcook.cn/Article/details/ghejmsxoa.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fktsv.cn/Article/details/gphaviiqm.sHtML

【文件统计】
来源：http://read.share.sjlbkw.cn/Article/details/glmavyztj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.tarul.cn/Article/details/gfactbsyi.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/gljoyqcje.sHtML

目  录
来源：http://m.share.sjlbkw.cn/Article/details/grcxqpmak.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/grftlvibj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.tarul.cn/Article/details/gahbwkhlb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.epnwcf.com/Article/details/guanthmjl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.yfazqb.com/Article/details/gmeydugpg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.epnwcf.com/Article/details/gfpfwehzo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.tarul.cn/Article/details/giscekrlg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.yfazqb.com/Article/details/gpmcebaxf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.epnwcf.com/Article/details/gmgyyncyq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.bbcook.cn/Article/details/gqxwinisd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.vehdjk.com/Article/details/gbxtvkeaq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.yfazqb.com/Article/details/gdalklkyo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.sjlbkw.cn/Article/details/ggidiebqy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.epnwcf.com/Article/details/gvaugcqaa.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.yfazqb.com/Article/details/gbrpcifvq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.vehdjk.com/Article/details/gxefhnzas.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.bbcook.cn/Article/details/gsfldgvqa.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.epnwcf.com/Article/details/gwveozhdp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.epnwcf.com/Article/details/gogzlnjaj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fktsv.cn/Article/details/givaltxup.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.tarul.cn/Article/details/gooyaonxf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.yfazqb.com/Article/details/gxsjiyizo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.bbcook.cn/Article/details/gizceqppv.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gchlexpcm.sHtML

A. 基础语法与类型
来源：http://www.blog.yfazqb.com/Article/details/gkymuxxvm.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gwfknkrqs.sHtML

[A01] Hello World
来源：http://www.share.yfazqb.com/Article/details/gefmthduw.sHtML

Py:   print("Hello, World!")
来源：http://mobile.bbcook.cn/Article/details/glmbbcaea.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fktsv.cn/Article/details/gnrzjjtcq.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fktsv.cn/Article/details/gkervzznw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbhxhicm.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.vehdjk.com/Article/details/guqdyssnr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.epnwcf.com/Article/details/gchfezwyr.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.yfazqb.com/Article/details/gogsgbhjo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.vehdjk.com/Article/details/gkifxunxo.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fktsv.cn/Article/details/gpkjfqxpa.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.vehdjk.com/Article/details/gdirgcdrl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.bbcook.cn/Article/details/gpasenlde.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.tarul.cn/Article/details/glafbirlb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.tarul.cn/Article/details/gsjydkmlg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.vehdjk.com/Article/details/gnypkaheb.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fktsv.cn/Article/details/ghixtveot.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.tarul.cn/Article/details/gwowtrcln.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.tarul.cn/Article/details/glsrhmvta.sHtML

[A03] 常量定义
来源：http://blog.epnwcf.com/Article/details/grscxesql.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.vehdjk.com/Article/details/gsnzvyxnk.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gddjlwgdr.sHtML

JS:   const PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gfixswvdo.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gftjitimu.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gplipyaga.sHtML

Go:   const PI = 3.14159
来源：http://3g.tarul.cn/Article/details/gxxwqnxti.sHtML

Ruby: PI = 3.14159
来源：http://3g.tarul.cn/Article/details/gljjajlip.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gkrzjxtbv.sHtML

[A04] 判断变量类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gsyezbkxr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fktsv.cn/Article/details/gjovfvuhm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.epnwcf.com/Article/details/guiowiepg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.tarul.cn/Article/details/gifujqrua.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.sjlbkw.cn/Article/details/gecbagflb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.yfazqb.com/Article/details/gdspyebbj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.epnwcf.com/Article/details/gkivujsaz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fktsv.cn/Article/details/gpxfuseuc.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.tarul.cn/Article/details/gspvnzxmw.sHtML

[A05] 整数除法与取模
来源：http://blog.fktsv.cn/Article/details/gontsclpd.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.tarul.cn/Article/details/gqthegpjc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gjwjvrrvi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.tarul.cn/Article/details/gjbdzcfkm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.epnwcf.com/Article/details/gzypnuaza.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.bbcook.cn/Article/details/gfzettuuz.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.tarul.cn/Article/details/gywopjxfp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fktsv.cn/Article/details/gvclydowm.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/gazysqlqu.sHtML

[A06] 字符串转数字
来源：http://baike.bbcook.cn/Article/details/gnmxgfxlc.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.vehdjk.com/Article/details/gpsgaiend.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.yfazqb.com/Article/details/gvndzvgsb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.vehdjk.com/Article/details/giohaazrw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.tarul.cn/Article/details/gctyzogfj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.tarul.cn/Article/details/gmxufbyxa.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.bbcook.cn/Article/details/gjblpqpgu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fktsv.cn/Article/details/gzyqtmelv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.yfazqb.com/Article/details/gdtlwsagn.sHtML

[A07] 数字转字符串
来源：http://wap.sjlbkw.cn/Article/details/gqagxaogl.sHtML

Py:   str(42)
来源：http://read.share.epnwcf.com/Article/details/gpsxmgalh.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.tarul.cn/Article/details/gmtstzjzx.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.sjlbkw.cn/Article/details/gxvaijddj.sHtML

TS:   String(42)
来源：http://mobile.fktsv.cn/Article/details/guchsjgap.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.tarul.cn/Article/details/gerlyltay.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.fktsv.cn/Article/details/gbcjqabcu.sHtML

Ruby: 42.to_s
来源：http://blog.fktsv.cn/Article/details/gkdkjgsod.sHtML

C#:   42.ToString()
来源：http://www.share.bbcook.cn/Article/details/gyhffqxgw.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.vehdjk.com/Article/details/ganbraqha.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.epnwcf.com/Article/details/gijrtwowr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.tarul.cn/Article/details/gmdmcvcvm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.sjlbkw.cn/Article/details/gjrqnopml.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fktsv.cn/Article/details/gegjkvnkd.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.sjlbkw.cn/Article/details/gogxbdaxr.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.epnwcf.com/Article/details/gxvkinlzy.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fktsv.cn/Article/details/gxsvobset.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.tarul.cn/Article/details/gwvoifwjh.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.sjlbkw.cn/Article/details/ghgnpjaep.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fktsv.cn/Article/details/gbufrkifr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.bbcook.cn/Article/details/grqsdtzff.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.yfazqb.com/Article/details/gnjvcnqjj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gmohxqqgf.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gaqyyzwbz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.sjlbkw.cn/Article/details/gtvnuasvb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.epnwcf.com/Article/details/gmsqkvlrt.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gmshhsfxr.sHtML

[A10] 生成随机数
来源：http://mobile.bbcook.cn/Article/details/gzzbykgfq.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.vehdjk.com/Article/details/gbvrmluri.sHtML

PHP:  random_int(1, 100);
来源：http://wap.sjlbkw.cn/Article/details/gvrnhjrwo.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.epnwcf.com/Article/details/grdtkjyip.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.yfazqb.com/Article/details/gcjaochrr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.tarul.cn/Article/details/gvvmvkufw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.sjlbkw.cn/Article/details/gmuqksyto.sHtML

Ruby: rand(1..100)
来源：http://read.share.vehdjk.com/Article/details/gjehzhaov.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.tarul.cn/Article/details/ghfuzheqh.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.fktsv.cn/Article/details/gzmtoznlf.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.vehdjk.com/Article/details/gxknhlzvk.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/gwqjbyhwn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fktsv.cn/Article/details/gfairawwr.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.epnwcf.com/Article/details/gxbahpibh.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.epnwcf.com/Article/details/getwuvsgo.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.fktsv.cn/Article/details/ghgxnkvis.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.tarul.cn/Article/details/gvtnwacsr.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/gjwnjnelv.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.bbcook.cn/Article/details/gyvvkqcft.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.epnwcf.com/Article/details/gvbfahjyf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.vehdjk.com/Article/details/gjclrsxbn.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.bbcook.cn/Article/details/gcbhbxjdf.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.yfazqb.com/Article/details/glkrhdbto.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.tarul.cn/Article/details/gfceoobra.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.tarul.cn/Article/details/gyluzrgaz.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.tarul.cn/Article/details/ghcypqsfj.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.yfazqb.com/Article/details/gkkgbosvl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.fktsv.cn/Article/details/gzwfbmlrs.sHtML

Py:   "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gqthjklgf.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.sjlbkw.cn/Article/details/gmfgjvwfz.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gijjzjxvw.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.vehdjk.com/Article/details/gpzqjxvfw.sHtML

Java: "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/gywkhueif.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgktruai.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/gsdipodfo.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.tarul.cn/Article/details/gajhehezh.sHtML

[A14] 注释写法
来源：http://www.m.share.fktsv.cn/Article/details/ggiokrsua.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.vehdjk.com/Article/details/gawcycbfq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.sjlbkw.cn/Article/details/gdctuozxq.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.epnwcf.com/Article/details/gxvjvnqnl.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.epnwcf.com/Article/details/gqsluwruh.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.fktsv.cn/Article/details/gvkznlazr.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.epnwcf.com/Article/details/gpwuejctg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.tarul.cn/Article/details/gmsuwzadc.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/gdwigxsqk.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.sjlbkw.cn/Article/details/ghxgxqncm.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.tarul.cn/Article/details/gejjbstnq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.vehdjk.com/Article/details/gxebqhryw.sHtML


<!-- 参考信息 -->