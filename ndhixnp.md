代发 wailian999

[U87] JS：解构默认值
来源：http://www.blog.bbcook.cn/Article/details/guburiszh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.vehdjk.com/Article/details/gjuhnnjic.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fktsv.cn/Article/details/gkwfvgkaq.sHtML

{ ...a, ...b }
来源：http://read.share.epnwcf.com/Article/details/gstvhuiqk.sHtML

[U89] JS：数组去重
来源：http://blog.yfazqb.com/Article/details/gzpeqmrge.sHtML

[...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gmozbmtxl.sHtML

[U90] JS：数字数组排序
来源：http://mobile.tarul.cn/Article/details/ggjxdkwnd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/ggobyawuo.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fktsv.cn/Article/details/goztxrsob.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.epnwcf.com/Article/details/gmxnddoze.sHtML

[U92] JS：深拷贝
来源：http://read.share.fktsv.cn/Article/details/gxpjhdgif.sHtML

structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gohgnauvk.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gktcpjuel.sHtML

`共 ${n} 条`
来源：http://3g.epnwcf.com/Article/details/galjpijzd.sHtML

[U94] JS：箭头函数
来源：http://3g.tarul.cn/Article/details/glprzmvyk.sHtML

const double = x => x * 2;
来源：http://www.blog.sjlbkw.cn/Article/details/gdhvwjfzf.sHtML

[U95] JS：Promise 包装
来源：http://wap.epnwcf.com/Article/details/golquatte.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.tarul.cn/Article/details/gcknrfkht.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fktsv.cn/Article/details/geclloqtf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.epnwcf.com/Article/details/gonuuezzf.sHtML

[U97] JS：并发请求
来源：http://baike.bbcook.cn/Article/details/gzgaojmwc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gesqppyra.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fktsv.cn/Article/details/gciwkjwzn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fktsv.cn/Article/details/gwqegxztt.sHtML

[U99] JS：事件监听
来源：http://www.blog.vehdjk.com/Article/details/gzctoxvyt.sHtML

el.addEventListener("click", e => {})
来源：http://blog.yfazqb.com/Article/details/gjyomcolb.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fktsv.cn/Article/details/gxjtiropl.sHtML

document.querySelector(".item")
来源：http://m.share.fktsv.cn/Article/details/gahvxdsid.sHtML

[U101] JS：classList 操作
来源：http://www.share.sjlbkw.cn/Article/details/gmjejypzw.sHtML

el.classList.toggle("active")
来源：http://mobile.sjlbkw.cn/Article/details/grjsikpae.sHtML

[U102] JS：本地存储
来源：http://mobile.epnwcf.com/Article/details/gjqoqrvly.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.epnwcf.com/Article/details/gydjuhizf.sHtML

[U103] JS：定时器
来源：http://www.share.fktsv.cn/Article/details/gubheyjrt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.tarul.cn/Article/details/gzzywoirm.sHtML

[U104] JS：防抖
来源：http://www.share.bbcook.cn/Article/details/gciaeprfm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gfjwkdhdv.sHtML

[U105] JS：节流
来源：http://www.share.bbcook.cn/Article/details/gndewbljg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.bbcook.cn/Article/details/gkkovcbrn.sHtML

[U106] JS：日期格式化
来源：http://baike.bbcook.cn/Article/details/gsoxcuuld.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.yfazqb.com/Article/details/gqslrvdiv.sHtML

[U107] JS：数字千分位
来源：http://read.share.vehdjk.com/Article/details/gczojfvum.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.vehdjk.com/Article/details/glsszhxrl.sHtML

[U108] JS：随机整数
来源：http://www.blog.epnwcf.com/Article/details/gfcckjfxl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.vehdjk.com/Article/details/gecxwinln.sHtML

[U109] JS：数组分组
来源：http://baike.bbcook.cn/Article/details/glmpvdrzt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.vehdjk.com/Article/details/gjmwrabeb.sHtML

[U110] JS：数组分块
来源：http://www.share.fktsv.cn/Article/details/gksvyoagy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.vehdjk.com/Article/details/guiroaqou.sHtML

[U111] JS：对象转 Map
来源：http://blog.fktsv.cn/Article/details/gfnwdiqzm.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzpcrgfa.sHtML

[U112] JS：字符串补位
来源：http://read.share.tarul.cn/Article/details/gbzprwudz.sHtML

"7".padStart(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gnjdtetky.sHtML

[U113] JS：正则替换全部
来源：http://read.share.vehdjk.com/Article/details/gkkkkzuop.sHtML

s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/gefdjxdvh.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.yfazqb.com/Article/details/gdbyneawn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.sjlbkw.cn/Article/details/getqicaho.sHtML

[U115] JS：生成 UUID
来源：http://3g.yfazqb.com/Article/details/gtqmwvjfy.sHtML

crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/gigssugwl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.bbcook.cn/Article/details/gbxmyqymx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.vehdjk.com/Article/details/gundtxlud.sHtML

[U117] JS：单元测试
来源：http://wap.vehdjk.com/Article/details/gcuqsietf.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.sjlbkw.cn/Article/details/gihfroypp.sHtML

[U118] JS：开发服务器
来源：http://baike.yfazqb.com/Article/details/gvckxztqi.sHtML

npm i -D vite;  npx vite
来源：http://wap.epnwcf.com/Article/details/guqaugloc.sHtML

[U119] JS：生产构建
来源：http://mobile.tarul.cn/Article/details/gxzybjskq.sHtML

npx vite build
来源：http://mobile.fktsv.cn/Article/details/gbignaesf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.tarul.cn/Article/details/ggvrgbuev.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.epnwcf.com/Article/details/gqxrlkkil.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gyeeuolaf.sHtML

统计汇总
来源：http://blog.epnwcf.com/Article/details/ggoqoqggd.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gcigjzfrl.sHtML

按语言统计（条）：
来源：http://3g.epnwcf.com/Article/details/gupaehbrx.sHtML

Python ......... 252
来源：http://3g.epnwcf.com/Article/details/gzedicbnt.sHtML

PHP ............ 252
来源：http://baike.yfazqb.com/Article/details/gheppcdld.sHtML

JavaScript ..... 252
来源：http://www.share.fktsv.cn/Article/details/gngfdyntb.sHtML

TypeScript ..... 212
来源：http://wap.vehdjk.com/Article/details/gtvhnqnhs.sHtML

Java ........... 212
来源：http://www.m.share.tarul.cn/Article/details/gujvnifws.sHtML

Go ............. 212
来源：http://www.share.epnwcf.com/Article/details/gslcjdokg.sHtML

Ruby ........... 212
来源：http://blog.tarul.cn/Article/details/gevwskcox.sHtML

C# ............. 212
来源：http://www.share.fktsv.cn/Article/details/gzdcqvkmk.sHtML

C .............. 30
来源：http://read.share.tarul.cn/Article/details/ghcrkmnow.sHtML

C++ ............ 30
来源：http://3g.bbcook.cn/Article/details/grzgbxrza.sHtML

SQL ............ 90
来源：http://m.share.epnwcf.com/Article/details/gqhmkutqu.sHtML

Bash ........... 80
来源：http://mobile.vehdjk.com/Article/details/gpbrsfqqy.sHtML

Kotlin ......... 15
来源：http://blog.vehdjk.com/Article/details/gahiybtba.sHtML

Swift .......... 15
来源：http://www.share.sjlbkw.cn/Article/details/gigacgdku.sHtML

Lua ............ 10
来源：http://blog.epnwcf.com/Article/details/gijghjzjr.sHtML

Perl ........... 10
来源：http://www.m.share.fktsv.cn/Article/details/gukrtfrze.sHtML

Scala .......... 10
来源：http://wap.yfazqb.com/Article/details/gfjbgwpee.sHtML

------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/grvzrdjrs.sHtML

合计 ........... 2106 条
来源：http://3g.yfazqb.com/Article/details/gutkzhyxi.sHtML

按章节统计：
来源：http://wap.vehdjk.com/Article/details/gznulkntb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.bbcook.cn/Article/details/gcpzsmwez.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fktsv.cn/Article/details/gpmiqrbcx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/ggloauhqh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fktsv.cn/Article/details/gtniflazm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.sjlbkw.cn/Article/details/gangqxlcr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.epnwcf.com/Article/details/gdnlrqbyv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.epnwcf.com/Article/details/gjjqcrjxc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fktsv.cn/Article/details/gksdnekns.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gltfltdwj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fktsv.cn/Article/details/gvizlyceo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/goxjuhyte.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gxidtkvkt.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/gfchmvxlv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.yfazqb.com/Article/details/gtmlwsdei.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fktsv.cn/Article/details/ghpnwqepm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/grjiylrqn.sHtML

Q SQL 专题                              90
来源：http://blog.sjlbkw.cn/Article/details/gawutrggz.sHtML

R Bash 专题                             80
来源：http://www.share.epnwcf.com/Article/details/gojcenose.sHtML

S C / C++ 专题                          60
来源：http://wap.vehdjk.com/Article/details/gojamtwjw.sHtML

T 其他语言补充                          60
来源：http://baike.fktsv.cn/Article/details/gawktszwg.sHtML

U 高频实用片段                         120
来源：http://3g.yfazqb.com/Article/details/gryubvffc.sHtML

------------------------------------
来源：http://blog.yfazqb.com/Article/details/gxabkctna.sHtML

合计                                  2106 条
来源：http://wap.epnwcf.com/Article/details/gbalqvfbp.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gmkqledup.sHtML

使用提醒
来源：http://wap.vehdjk.com/Article/details/ghwgdhhnb.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.yfazqb.com/Article/details/gcmmsowqh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fktsv.cn/Article/details/gtysfrqbn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.vehdjk.com/Article/details/guzwsqwap.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.sjlbkw.cn/Article/details/gjumgrkxa.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.epnwcf.com/Article/details/gdasiamux.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.epnwcf.com/Article/details/gwstyurne.sHtML

—— 文件结束 ——
来源：http://wap.bbcook.cn/Article/details/gvneimgrf.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gnrcybkhg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.sjlbkw.cn/Article/details/gncplhlfp.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.bbcook.cn/Article/details/gvgprvewi.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gfmvtqdxf.sHtML

【收录内容】
来源：http://www.m.share.yfazqb.com/Article/details/gwxseahvt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.epnwcf.com/Article/details/gnmvvybsi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.vehdjk.com/Article/details/ghixfqksx.sHtML

SQL · Bash · C · C++
来源：http://blog.fktsv.cn/Article/details/goivwdoed.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.yfazqb.com/Article/details/gokbwllvo.sHtML

【使用说明】
来源：http://blog.bbcook.cn/Article/details/gwrgawcaz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.epnwcf.com/Article/details/guwetzshi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fktsv.cn/Article/details/gespcgjld.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fktsv.cn/Article/details/glznadwla.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.epnwcf.com/Article/details/gqlzajqwx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.yfazqb.com/Article/details/gwqgzdrtn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.epnwcf.com/Article/details/gvrgtorvc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.sjlbkw.cn/Article/details/gfxpzpwhd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.bbcook.cn/Article/details/ghcnwelbw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.bbcook.cn/Article/details/gqlsdpxng.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.tarul.cn/Article/details/geidqnzox.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.bbcook.cn/Article/details/gnmhpskzj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.yfazqb.com/Article/details/gmtjgmstm.sHtML

【文件统计】
来源：http://baike.bbcook.cn/Article/details/gwhxquyya.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.epnwcf.com/Article/details/gcnjuxrpc.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/ghdstypot.sHtML

目  录
来源：http://baike.vehdjk.com/Article/details/gvtwbdhcm.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gztfcsrmt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.sjlbkw.cn/Article/details/gijukqrqa.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.yfazqb.com/Article/details/gnyrjyspw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.tarul.cn/Article/details/gbxqwwcpj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.sjlbkw.cn/Article/details/gibzfzagj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.sjlbkw.cn/Article/details/gcvexmwno.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gyagdvkxg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.yfazqb.com/Article/details/ggycjgueo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.vehdjk.com/Article/details/gqamkgbmr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/gzkygdott.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.sjlbkw.cn/Article/details/gidtbbfyz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/gluyxtiuw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gosutumuz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gooyvwgel.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fktsv.cn/Article/details/gpfzimlel.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.sjlbkw.cn/Article/details/gkfvwivrm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fktsv.cn/Article/details/gqmckdbje.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.tarul.cn/Article/details/gokyhwmmm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.vehdjk.com/Article/details/gveehdjkp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.vehdjk.com/Article/details/gglraakeu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/gcvzmcryp.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.epnwcf.com/Article/details/gddupakkx.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gwpimtxtw.sHtML

A. 基础语法与类型
来源：http://www.m.share.bbcook.cn/Article/details/gcsvektzw.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gppqufsmk.sHtML

[A01] Hello World
来源：http://baike.yfazqb.com/Article/details/ghmsarrmu.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.epnwcf.com/Article/details/goolpgpsx.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.tarul.cn/Article/details/gbmqyozbx.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.epnwcf.com/Article/details/gjpsbnizu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.tarul.cn/Article/details/gmjjyjduh.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.yfazqb.com/Article/details/gcoooexqn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.vehdjk.com/Article/details/gvdccivka.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fktsv.cn/Article/details/gqqwloctl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.epnwcf.com/Article/details/gutqakark.sHtML

[A02] 变量声明与赋值
来源：http://baike.epnwcf.com/Article/details/ghqlwggnx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.epnwcf.com/Article/details/gicaucgze.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.bbcook.cn/Article/details/gqmmuhtsq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.yfazqb.com/Article/details/gckkphfat.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.sjlbkw.cn/Article/details/glpbpzsut.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.tarul.cn/Article/details/gdsuxuvyw.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.yfazqb.com/Article/details/gmqonhsbo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.tarul.cn/Article/details/goenaaoin.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.tarul.cn/Article/details/gurwkpchk.sHtML

[A03] 常量定义
来源：http://baike.sjlbkw.cn/Article/details/gnshvofdf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.tarul.cn/Article/details/gogbvfbyt.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gylbjzzuf.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gocqjpfcq.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gkoanidzg.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gotzllwvw.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.yfazqb.com/Article/details/ggupzvzfw.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fktsv.cn/Article/details/gbjkyhpcl.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/godiqdkmr.sHtML

[A04] 判断变量类型
来源：http://baike.tarul.cn/Article/details/ghlzpyypv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnylvrwii.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.vehdjk.com/Article/details/gjylvxgus.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.yfazqb.com/Article/details/gcpsldsdv.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.vehdjk.com/Article/details/gwniujeyg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.bbcook.cn/Article/details/gugsoggwv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fktsv.cn/Article/details/goqflwpza.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.sjlbkw.cn/Article/details/glksktebs.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.tarul.cn/Article/details/gdtbhuewq.sHtML

[A05] 整数除法与取模
来源：http://read.share.bbcook.cn/Article/details/gwgwfpdec.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.bbcook.cn/Article/details/gioywxqgg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gdozyjevw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gorzohuye.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gbeqtntgv.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/gvpgntuaj.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.epnwcf.com/Article/details/gfgicfnwy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gvfgmhjje.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fktsv.cn/Article/details/gbzsepykk.sHtML

[A06] 字符串转数字
来源：http://www.share.bbcook.cn/Article/details/gzxjfdtlg.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.epnwcf.com/Article/details/gqvfvpbbt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.epnwcf.com/Article/details/gagpnnxlv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.vehdjk.com/Article/details/ghojthqlp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.epnwcf.com/Article/details/gvcimtexx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.bbcook.cn/Article/details/gyovtzpgw.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.tarul.cn/Article/details/goskebaba.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.sjlbkw.cn/Article/details/gnjqvdjjb.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.vehdjk.com/Article/details/gpifqqkcg.sHtML

[A07] 数字转字符串
来源：http://www.blog.epnwcf.com/Article/details/gcwzwgqsn.sHtML

Py:   str(42)
来源：http://www.share.bbcook.cn/Article/details/gpfzyhrzq.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.sjlbkw.cn/Article/details/gechrcmgz.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.sjlbkw.cn/Article/details/gqhzxnxrd.sHtML

TS:   String(42)
来源：http://read.share.epnwcf.com/Article/details/ghabbbxao.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.yfazqb.com/Article/details/gfmpszmfp.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.vehdjk.com/Article/details/gzuvtxows.sHtML

Ruby: 42.to_s
来源：http://m.share.bbcook.cn/Article/details/ganvcneid.sHtML

C#:   42.ToString()
来源：http://wap.fktsv.cn/Article/details/gsragdilg.sHtML

[A08] 取整与四舍五入
来源：http://wap.fktsv.cn/Article/details/gzeeuwpsn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.tarul.cn/Article/details/gdneldjhr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.tarul.cn/Article/details/gwihdwuxw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.sjlbkw.cn/Article/details/gkaffhfhd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.sjlbkw.cn/Article/details/gseoeupnl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.yfazqb.com/Article/details/ghjquaviw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.fktsv.cn/Article/details/gexjwftlh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fktsv.cn/Article/details/giuragpxj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.sjlbkw.cn/Article/details/gzulrbbbj.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.vehdjk.com/Article/details/gknwsrxwc.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gazegpddr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.epnwcf.com/Article/details/gngzuiyde.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.vehdjk.com/Article/details/gprlbcaav.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gogvtnlpy.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.tarul.cn/Article/details/gknxdqgle.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.vehdjk.com/Article/details/gijlhwwqf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.epnwcf.com/Article/details/gieaxgrrw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fktsv.cn/Article/details/gdtltvkfq.sHtML

[A10] 生成随机数
来源：http://www.m.share.epnwcf.com/Article/details/gwldczchh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.vehdjk.com/Article/details/gfontsyif.sHtML

PHP:  random_int(1, 100);
来源：http://wap.sjlbkw.cn/Article/details/gfwydiihc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.yfazqb.com/Article/details/gqaaljncd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.epnwcf.com/Article/details/gclnhxpfs.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.fktsv.cn/Article/details/gikbzbqwk.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.tarul.cn/Article/details/gnordjffx.sHtML

Ruby: rand(1..100)
来源：http://mobile.fktsv.cn/Article/details/gucxcgisq.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.sjlbkw.cn/Article/details/gsghokgxl.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.bbcook.cn/Article/details/gfoebgfac.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.sjlbkw.cn/Article/details/gykqsekyb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.tarul.cn/Article/details/gdilsazhl.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.yfazqb.com/Article/details/gyznmqcfm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/gwrfkmemz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.yfazqb.com/Article/details/gklmaipxz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.yfazqb.com/Article/details/gmnbgqcck.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.epnwcf.com/Article/details/gwlapywkw.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/gymmgozpv.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.tarul.cn/Article/details/gecwwrhjl.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.sjlbkw.cn/Article/details/gccdrmyom.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.epnwcf.com/Article/details/givjrflix.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.epnwcf.com/Article/details/genqhcnkn.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.yfazqb.com/Article/details/geaovypip.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.sjlbkw.cn/Article/details/gtoauedjf.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzaiotdam.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.vehdjk.com/Article/details/gdoelqbsm.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.bbcook.cn/Article/details/gbzkkxjrt.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.bbcook.cn/Article/details/gbpivvcde.sHtML

Py:   "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gzqmbhwha.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.yfazqb.com/Article/details/glxsylgpx.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/grbngodym.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.fktsv.cn/Article/details/gyujkhawx.sHtML

Java: "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gzegzvkuw.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.fktsv.cn/Article/details/gcucvpylv.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.epnwcf.com/Article/details/gcehqezuh.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gahqpjgkt.sHtML

[A14] 注释写法
来源：http://baike.fktsv.cn/Article/details/goinidmjx.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.sjlbkw.cn/Article/details/grredzskv.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.vehdjk.com/Article/details/glavojbze.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/gzgpargov.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.fktsv.cn/Article/details/grrgfelro.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.tarul.cn/Article/details/gptshklkc.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.vehdjk.com/Article/details/grujnjdnc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.tarul.cn/Article/details/gqmkqdhct.sHtML


<!-- 参考信息 -->