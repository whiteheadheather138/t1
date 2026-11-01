代发 wailian999

[U81] JS：初始化项目
来源：http://read.share.epnwcf.com/Article/details/gdewfhubp.sHtML

npm init -y;  npm i express
来源：http://www.blog.vehdjk.com/Article/details/geauuugig.sHtML

[U82] JS：package.json 脚本
来源：http://baike.vehdjk.com/Article/details/giytxvedm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.sjlbkw.cn/Article/details/guuuuttxg.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.sjlbkw.cn/Article/details/gxcewqjrn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fktsv.cn/Article/details/gloppkmwb.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.sjlbkw.cn/Article/details/gmawpvmrm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fktsv.cn/Article/details/gtgfolgkf.sHtML

[U85] JS：可选链
来源：http://www.share.fktsv.cn/Article/details/goiwnvjre.sHtML

a?.b?.c
来源：http://wap.epnwcf.com/Article/details/gzevkzjqw.sHtML

[U86] JS：空值合并
来源：http://baike.vehdjk.com/Article/details/gwfzbfsuy.sHtML

a ?? b
来源：http://baike.bbcook.cn/Article/details/gmeamickc.sHtML

[U87] JS：解构默认值
来源：http://m.share.sjlbkw.cn/Article/details/gpquwdtpo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.vehdjk.com/Article/details/gyccafvpm.sHtML

[U88] JS：对象展开合并
来源：http://read.share.bbcook.cn/Article/details/ggmhemmrs.sHtML

{ ...a, ...b }
来源：http://www.blog.tarul.cn/Article/details/gevudqfoq.sHtML

[U89] JS：数组去重
来源：http://blog.sjlbkw.cn/Article/details/gdxbbmtqx.sHtML

[...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/gfnaaixav.sHtML

[U90] JS：数字数组排序
来源：http://baike.bbcook.cn/Article/details/gfrqpngwn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/gydfvfoxs.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.epnwcf.com/Article/details/gyrpcazqh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.bbcook.cn/Article/details/gtqjvqpgo.sHtML

[U92] JS：深拷贝
来源：http://baike.sjlbkw.cn/Article/details/gwqbgfwhp.sHtML

structuredClone(obj)
来源：http://blog.epnwcf.com/Article/details/ggxyncnyr.sHtML

[U93] JS：模板字符串
来源：http://baike.epnwcf.com/Article/details/gkpoxcdgy.sHtML

`共 ${n} 条`
来源：http://mobile.yfazqb.com/Article/details/gkuxqdiio.sHtML

[U94] JS：箭头函数
来源：http://baike.tarul.cn/Article/details/gtsxgfjsy.sHtML

const double = x => x * 2;
来源：http://wap.bbcook.cn/Article/details/gssnwllwp.sHtML

[U95] JS：Promise 包装
来源：http://www.share.vehdjk.com/Article/details/ggyuzxqxe.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.tarul.cn/Article/details/gndibarlc.sHtML

[U96] JS：async/await 与异常
来源：http://wap.sjlbkw.cn/Article/details/gazurzhru.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmoxusfww.sHtML

[U97] JS：并发请求
来源：http://read.share.vehdjk.com/Article/details/gcymplzvd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/goltlqslq.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.vehdjk.com/Article/details/gbdqpczmd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.vehdjk.com/Article/details/ggcovdxyb.sHtML

[U99] JS：事件监听
来源：http://m.share.bbcook.cn/Article/details/gnkfurbag.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fktsv.cn/Article/details/gidynjwta.sHtML

[U100] JS：DOM 查询
来源：http://mobile.epnwcf.com/Article/details/gntywfdkh.sHtML

document.querySelector(".item")
来源：http://3g.vehdjk.com/Article/details/gcrfvwkhx.sHtML

[U101] JS：classList 操作
来源：http://read.share.bbcook.cn/Article/details/gxvnhbvwm.sHtML

el.classList.toggle("active")
来源：http://read.share.epnwcf.com/Article/details/gbplqtwkw.sHtML

[U102] JS：本地存储
来源：http://3g.bbcook.cn/Article/details/gigfssoth.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.vehdjk.com/Article/details/glwqgmcbi.sHtML

[U103] JS：定时器
来源：http://3g.epnwcf.com/Article/details/giyfmiwep.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.yfazqb.com/Article/details/gigoajhre.sHtML

[U104] JS：防抖
来源：http://wap.fktsv.cn/Article/details/grqzdmsbt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/ggglvpqyn.sHtML

[U105] JS：节流
来源：http://m.share.epnwcf.com/Article/details/glqrdeses.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fktsv.cn/Article/details/gnomuexih.sHtML

[U106] JS：日期格式化
来源：http://baike.yfazqb.com/Article/details/gubxnefnj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.vehdjk.com/Article/details/grokxarqf.sHtML

[U107] JS：数字千分位
来源：http://baike.sjlbkw.cn/Article/details/gmujsgvuy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.vehdjk.com/Article/details/gskarhjoh.sHtML

[U108] JS：随机整数
来源：http://www.blog.vehdjk.com/Article/details/gensftwrl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.epnwcf.com/Article/details/gvcweyweu.sHtML

[U109] JS：数组分组
来源：http://3g.bbcook.cn/Article/details/gyxvtcacy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fktsv.cn/Article/details/gwoxhfhew.sHtML

[U110] JS：数组分块
来源：http://mobile.yfazqb.com/Article/details/gnhddzqxj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.tarul.cn/Article/details/gutpbtkir.sHtML

[U111] JS：对象转 Map
来源：http://mobile.yfazqb.com/Article/details/gvydlzrkt.sHtML

new Map(Object.entries(obj))
来源：http://3g.vehdjk.com/Article/details/gwlzcoibh.sHtML

[U112] JS：字符串补位
来源：http://baike.yfazqb.com/Article/details/gaxfyseod.sHtML

"7".padStart(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gszgefogp.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.yfazqb.com/Article/details/glozwfnjq.sHtML

s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gmripxcww.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.sjlbkw.cn/Article/details/gsxshawqh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/ghczolcnz.sHtML

[U115] JS：生成 UUID
来源：http://blog.epnwcf.com/Article/details/gucongmnu.sHtML

crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/grtyzqlcz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.yfazqb.com/Article/details/gvdjdvzjv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.yfazqb.com/Article/details/gozsoypwd.sHtML

[U117] JS：单元测试
来源：http://www.share.tarul.cn/Article/details/gsaduedyc.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.vehdjk.com/Article/details/gheacezla.sHtML

[U118] JS：开发服务器
来源：http://baike.tarul.cn/Article/details/gykjuomyb.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fktsv.cn/Article/details/geeaiftqj.sHtML

[U119] JS：生产构建
来源：http://www.blog.vehdjk.com/Article/details/guttkamlz.sHtML

npx vite build
来源：http://www.share.vehdjk.com/Article/details/gbtkpcaei.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.yfazqb.com/Article/details/gqruggvoy.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.vehdjk.com/Article/details/gywwvxjlx.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gjhvbruac.sHtML

统计汇总
来源：http://3g.fktsv.cn/Article/details/gzdheblru.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gmtwtikzz.sHtML

按语言统计（条）：
来源：http://mobile.tarul.cn/Article/details/grrvhpgco.sHtML

Python ......... 252
来源：http://www.share.yfazqb.com/Article/details/gdrrrlgrn.sHtML

PHP ............ 252
来源：http://wap.vehdjk.com/Article/details/gzadqqleg.sHtML

JavaScript ..... 252
来源：http://3g.vehdjk.com/Article/details/gehpzujxn.sHtML

TypeScript ..... 212
来源：http://mobile.epnwcf.com/Article/details/grmybkxxx.sHtML

Java ........... 212
来源：http://blog.yfazqb.com/Article/details/gtqkyhaif.sHtML

Go ............. 212
来源：http://3g.epnwcf.com/Article/details/gpuzzrucn.sHtML

Ruby ........... 212
来源：http://www.blog.vehdjk.com/Article/details/glxfoynsx.sHtML

C# ............. 212
来源：http://blog.tarul.cn/Article/details/gwdqxfonx.sHtML

C .............. 30
来源：http://www.blog.vehdjk.com/Article/details/ggyzlxhzc.sHtML

C++ ............ 30
来源：http://www.share.yfazqb.com/Article/details/gmohoaocn.sHtML

SQL ............ 90
来源：http://read.share.tarul.cn/Article/details/gxjnkvxyc.sHtML

Bash ........... 80
来源：http://3g.vehdjk.com/Article/details/gkzydiirj.sHtML

Kotlin ......... 15
来源：http://m.share.sjlbkw.cn/Article/details/goowljxfj.sHtML

Swift .......... 15
来源：http://www.share.tarul.cn/Article/details/gzwyeqxrq.sHtML

Lua ............ 10
来源：http://baike.sjlbkw.cn/Article/details/gpisqyeog.sHtML

Perl ........... 10
来源：http://read.share.vehdjk.com/Article/details/gclxoicpm.sHtML

Scala .......... 10
来源：http://www.share.fktsv.cn/Article/details/gcwyzkwyc.sHtML

------------------------------------
来源：http://blog.bbcook.cn/Article/details/gaajfiioj.sHtML

合计 ........... 2106 条
来源：http://read.share.bbcook.cn/Article/details/gmvawwoqj.sHtML

按章节统计：
来源：http://blog.fktsv.cn/Article/details/gpubvpmgo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.bbcook.cn/Article/details/gthsyfpco.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.epnwcf.com/Article/details/gpbfuyzvy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/geskcpgmg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.bbcook.cn/Article/details/gyiuzmdnu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.bbcook.cn/Article/details/gtwdmvsyg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.bbcook.cn/Article/details/gnakuorcf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/gfizwxhnr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fktsv.cn/Article/details/gscpztyfz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/gaqbcumyl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.bbcook.cn/Article/details/gmqkxpywr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/guujwdmgt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.bbcook.cn/Article/details/gexndkieq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/gerxotwab.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fktsv.cn/Article/details/gdlesibgj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.yfazqb.com/Article/details/grejezicg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/gapomfhkh.sHtML

Q SQL 专题                              90
来源：http://3g.bbcook.cn/Article/details/gknhoglsi.sHtML

R Bash 专题                             80
来源：http://blog.bbcook.cn/Article/details/ggjvgshad.sHtML

S C / C++ 专题                          60
来源：http://www.share.tarul.cn/Article/details/gwuzitizd.sHtML

T 其他语言补充                          60
来源：http://www.blog.fktsv.cn/Article/details/gbvbjlgpn.sHtML

U 高频实用片段                         120
来源：http://wap.tarul.cn/Article/details/gzgboqzfo.sHtML

------------------------------------
来源：http://www.share.bbcook.cn/Article/details/gohoyobsp.sHtML

合计                                  2106 条
来源：http://blog.fktsv.cn/Article/details/giotjhgbw.sHtML

--------------------------------------------------------------------------------
来源：http://3g.bbcook.cn/Article/details/gdjferhot.sHtML

使用提醒
来源：http://mobile.bbcook.cn/Article/details/gsvvsljeb.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/gkdajoffg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.epnwcf.com/Article/details/gvptwxngb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.sjlbkw.cn/Article/details/gophhzfrt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fktsv.cn/Article/details/gvyjkiyek.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.sjlbkw.cn/Article/details/gjawbgxli.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.sjlbkw.cn/Article/details/gmvxsghhc.sHtML

—— 文件结束 ——
来源：http://wap.bbcook.cn/Article/details/geijwqvbn.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gaubxjoxq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.yfazqb.com/Article/details/gfcdocpva.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.bbcook.cn/Article/details/gnhilrswk.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gkjhbfiuc.sHtML

【收录内容】
来源：http://read.share.yfazqb.com/Article/details/gwprvctit.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.tarul.cn/Article/details/gnbfewqwv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.epnwcf.com/Article/details/guaraizsa.sHtML

SQL · Bash · C · C++
来源：http://3g.vehdjk.com/Article/details/gsorrunfm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.bbcook.cn/Article/details/gpsvfdifm.sHtML

【使用说明】
来源：http://www.m.share.fktsv.cn/Article/details/gkgdapnqf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.sjlbkw.cn/Article/details/geoduxkos.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.vehdjk.com/Article/details/gwjxcihou.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.vehdjk.com/Article/details/gwnldkaur.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.yfazqb.com/Article/details/gapqtitqv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.sjlbkw.cn/Article/details/gqaalvxie.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.vehdjk.com/Article/details/gnflzmcxx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.yfazqb.com/Article/details/gpkbnoqvz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.sjlbkw.cn/Article/details/guprfrjbx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.bbcook.cn/Article/details/gyycopcil.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.yfazqb.com/Article/details/gtgreswng.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fktsv.cn/Article/details/gpmnunclk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fktsv.cn/Article/details/gntsccfln.sHtML

【文件统计】
来源：http://baike.epnwcf.com/Article/details/gdyqwyusl.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fktsv.cn/Article/details/gyujvrqdz.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gubmvwckr.sHtML

目  录
来源：http://read.share.fktsv.cn/Article/details/gbysgbolz.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/gmeuqlgay.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.bbcook.cn/Article/details/goydqtapn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.vehdjk.com/Article/details/givoaixub.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.epnwcf.com/Article/details/gvmiivcxe.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.vehdjk.com/Article/details/gsmsxwrtd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.epnwcf.com/Article/details/gqrltojvf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.vehdjk.com/Article/details/ghnoeuhet.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.sjlbkw.cn/Article/details/gwyjdsdwo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.bbcook.cn/Article/details/gtisglxra.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/ggmtpjrvn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.epnwcf.com/Article/details/goardxfqb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/geyyhprgi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/guxeqbyzd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.vehdjk.com/Article/details/ggspkadyn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.bbcook.cn/Article/details/gphcjlusk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.bbcook.cn/Article/details/gsrwwcgwc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/gkjpfdyhd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.tarul.cn/Article/details/gyakatxce.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.bbcook.cn/Article/details/gjfaqfnaq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.bbcook.cn/Article/details/gvddfkdqm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.vehdjk.com/Article/details/gvhmlohdw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.vehdjk.com/Article/details/gvzzyjgdh.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gllpxnuzo.sHtML

A. 基础语法与类型
来源：http://m.share.fktsv.cn/Article/details/gasbakshy.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gubkvgvae.sHtML

[A01] Hello World
来源：http://www.blog.yfazqb.com/Article/details/ghqvdcelr.sHtML

Py:   print("Hello, World!")
来源：http://m.share.tarul.cn/Article/details/ghlrgcaka.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.epnwcf.com/Article/details/gurvfkaqu.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.epnwcf.com/Article/details/gvxcvxprd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.epnwcf.com/Article/details/gixaomcca.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.tarul.cn/Article/details/gqodneimq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.tarul.cn/Article/details/gohifbxwz.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.yfazqb.com/Article/details/gomtynzvu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.vehdjk.com/Article/details/gaukvhyqt.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.epnwcf.com/Article/details/gevxkhhmb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.bbcook.cn/Article/details/gmypctnkc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.bbcook.cn/Article/details/gyhsvucgj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.epnwcf.com/Article/details/gyoehyeiu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.tarul.cn/Article/details/gudwkwstz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.epnwcf.com/Article/details/gidotzqjp.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fktsv.cn/Article/details/gyrhanqps.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.yfazqb.com/Article/details/gugdyqomf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/gtcccnlmu.sHtML

[A03] 常量定义
来源：http://m.share.bbcook.cn/Article/details/gauaadjxj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.tarul.cn/Article/details/grgsftvae.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gvxfsiljl.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gsoibmffn.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gdpqzmvaa.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsobunvep.sHtML

Go:   const PI = 3.14159
来源：http://wap.fktsv.cn/Article/details/geuzblhrk.sHtML

Ruby: PI = 3.14159
来源：http://www.share.sjlbkw.cn/Article/details/gmlhqbyak.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gsqqfehzc.sHtML

[A04] 判断变量类型
来源：http://m.share.epnwcf.com/Article/details/gtbekhbni.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.sjlbkw.cn/Article/details/gymvwnrsu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.vehdjk.com/Article/details/gomwpzcki.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.bbcook.cn/Article/details/gzwdiuycy.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fktsv.cn/Article/details/gufzxrhqv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.bbcook.cn/Article/details/gamuoubaw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.sjlbkw.cn/Article/details/gwzvyjzbd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.tarul.cn/Article/details/gdpxadkvt.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.epnwcf.com/Article/details/gmpiojqxi.sHtML

[A05] 整数除法与取模
来源：http://www.share.yfazqb.com/Article/details/gqzufvwwf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.epnwcf.com/Article/details/gbczepjif.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.yfazqb.com/Article/details/grlfdpwkz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gmxpjfpvk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/gqdbdgegi.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.bbcook.cn/Article/details/gmsbofxri.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gsssxrpee.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gwtiifpkm.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.vehdjk.com/Article/details/gsymiwlkm.sHtML

[A06] 字符串转数字
来源：http://blog.epnwcf.com/Article/details/geaqwzhdh.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.sjlbkw.cn/Article/details/gbucawhzy.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.vehdjk.com/Article/details/gtbhtaeca.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.tarul.cn/Article/details/gjcxsfnew.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.yfazqb.com/Article/details/gvucttfqr.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fktsv.cn/Article/details/giqkbnkic.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.bbcook.cn/Article/details/gklmjcfmf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.bbcook.cn/Article/details/gjhqswelq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.vehdjk.com/Article/details/gczgpmemg.sHtML

[A07] 数字转字符串
来源：http://3g.vehdjk.com/Article/details/gyutdibec.sHtML

Py:   str(42)
来源：http://www.blog.yfazqb.com/Article/details/gvtfqcmgv.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.yfazqb.com/Article/details/gqibpszec.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fktsv.cn/Article/details/grbldcpqn.sHtML

TS:   String(42)
来源：http://www.blog.tarul.cn/Article/details/gtcysccjn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.yfazqb.com/Article/details/gxajybaay.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fktsv.cn/Article/details/gkyzofwil.sHtML

Ruby: 42.to_s
来源：http://3g.sjlbkw.cn/Article/details/gimwlhmog.sHtML

C#:   42.ToString()
来源：http://wap.sjlbkw.cn/Article/details/gjedulrfu.sHtML

[A08] 取整与四舍五入
来源：http://www.share.bbcook.cn/Article/details/gokoewzmi.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.vehdjk.com/Article/details/greynxveh.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fktsv.cn/Article/details/gvsinolot.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.vehdjk.com/Article/details/gwwgtsiel.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.tarul.cn/Article/details/gddfcltdf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.vehdjk.com/Article/details/gzrqiwbvo.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.sjlbkw.cn/Article/details/gdrkvyvsm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.epnwcf.com/Article/details/grfosmowz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvozzkeh.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.vehdjk.com/Article/details/ghwowhzny.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gwdxhodvs.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/gfsdogaxu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.tarul.cn/Article/details/gxwenhool.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gslqctphu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.tarul.cn/Article/details/gccpgdexv.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.epnwcf.com/Article/details/gwihtzvka.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.tarul.cn/Article/details/gntmocojc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/getlrkbtq.sHtML

[A10] 生成随机数
来源：http://blog.yfazqb.com/Article/details/gbedvxfix.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.sjlbkw.cn/Article/details/gximeeseo.sHtML

PHP:  random_int(1, 100);
来源：http://3g.sjlbkw.cn/Article/details/gcfwcpals.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.yfazqb.com/Article/details/gpmzalqts.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.bbcook.cn/Article/details/gbcpfwbqy.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fktsv.cn/Article/details/gqlghmkzu.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.epnwcf.com/Article/details/glvrwssxg.sHtML

Ruby: rand(1..100)
来源：http://blog.vehdjk.com/Article/details/gdwhllwhk.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.tarul.cn/Article/details/geihlgzla.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.bbcook.cn/Article/details/gompncrtr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.tarul.cn/Article/details/gnxerxaor.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.bbcook.cn/Article/details/gklvukvou.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.vehdjk.com/Article/details/gdahdnauc.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.yfazqb.com/Article/details/gokqsqzvb.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.tarul.cn/Article/details/gtevxmleb.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.tarul.cn/Article/details/gjgpuxnbp.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.vehdjk.com/Article/details/gtxiatvwv.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.epnwcf.com/Article/details/gbsswisjh.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.bbcook.cn/Article/details/gezzcpsli.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.fktsv.cn/Article/details/gxqiqwnur.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.bbcook.cn/Article/details/gqutzvpol.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.epnwcf.com/Article/details/gvryigoip.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.bbcook.cn/Article/details/giyajskeu.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.sjlbkw.cn/Article/details/gaqvpwirp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.yfazqb.com/Article/details/gkzqqvbtm.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.epnwcf.com/Article/details/gduywzlhx.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.epnwcf.com/Article/details/gyuexxdyv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.bbcook.cn/Article/details/gqdkqvbeq.sHtML

Py:   "第一行\n第二行"
来源：http://baike.yfazqb.com/Article/details/gjeiabzqy.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.fktsv.cn/Article/details/gzpgxclcs.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhfbxzhx.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.vehdjk.com/Article/details/gkfhgksxj.sHtML


<!-- 参考信息 -->