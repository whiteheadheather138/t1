代发 wailian999

[U79] PHP：静态分析
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmmqtfxi.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.vehdjk.com/Article/details/gwneduzxp.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.epnwcf.com/Article/details/gsuczrnwx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.bbcook.cn/Article/details/gwjxbauap.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.bbcook.cn/Article/details/gcupfmdph.sHtML

npm init -y;  npm i express
来源：http://3g.yfazqb.com/Article/details/ghuimqooz.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.tarul.cn/Article/details/gxgdhisqi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.tarul.cn/Article/details/gjflxgcqc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.tarul.cn/Article/details/gevavgqul.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.epnwcf.com/Article/details/gkeinstls.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.yfazqb.com/Article/details/gpqynipnm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fktsv.cn/Article/details/gbkiockui.sHtML

[U85] JS：可选链
来源：http://blog.sjlbkw.cn/Article/details/gvsaecpic.sHtML

a?.b?.c
来源：http://wap.sjlbkw.cn/Article/details/gmtsolqwv.sHtML

[U86] JS：空值合并
来源：http://www.blog.sjlbkw.cn/Article/details/gjgdviezn.sHtML

a ?? b
来源：http://m.share.vehdjk.com/Article/details/gozgtdrcy.sHtML

[U87] JS：解构默认值
来源：http://read.share.bbcook.cn/Article/details/gfxjaeedg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fktsv.cn/Article/details/gqeeyzxzw.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.tarul.cn/Article/details/geaillrgn.sHtML

{ ...a, ...b }
来源：http://www.share.yfazqb.com/Article/details/gnlngxrxb.sHtML

[U89] JS：数组去重
来源：http://www.blog.fktsv.cn/Article/details/gqrlyfrdp.sHtML

[...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gdwslnbsy.sHtML

[U90] JS：数字数组排序
来源：http://wap.sjlbkw.cn/Article/details/gaeuiuxzy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gbpnjcpjo.sHtML

[U91] JS：对象键值遍历
来源：http://3g.yfazqb.com/Article/details/gsnkudawk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.vehdjk.com/Article/details/ghwyczolr.sHtML

[U92] JS：深拷贝
来源：http://blog.tarul.cn/Article/details/gfaoufaes.sHtML

structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/govazjdpn.sHtML

[U93] JS：模板字符串
来源：http://www.blog.bbcook.cn/Article/details/gczwembcg.sHtML

`共 ${n} 条`
来源：http://baike.vehdjk.com/Article/details/gdquvdflo.sHtML

[U94] JS：箭头函数
来源：http://baike.yfazqb.com/Article/details/gnzexgbvb.sHtML

const double = x => x * 2;
来源：http://baike.tarul.cn/Article/details/gboqmvyow.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.epnwcf.com/Article/details/gafrktbww.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.yfazqb.com/Article/details/gsrkqdegi.sHtML

[U96] JS：async/await 与异常
来源：http://wap.yfazqb.com/Article/details/genztbrxj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/geoemgohl.sHtML

[U97] JS：并发请求
来源：http://mobile.bbcook.cn/Article/details/gqzqqvrho.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gzquncslu.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.vehdjk.com/Article/details/gmrrnltfd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.sjlbkw.cn/Article/details/gnvhmqmqg.sHtML

[U99] JS：事件监听
来源：http://blog.tarul.cn/Article/details/gutbqpdyp.sHtML

el.addEventListener("click", e => {})
来源：http://baike.yfazqb.com/Article/details/gfretchsm.sHtML

[U100] JS：DOM 查询
来源：http://blog.yfazqb.com/Article/details/goymefhqj.sHtML

document.querySelector(".item")
来源：http://www.m.share.tarul.cn/Article/details/gvkjzjzqj.sHtML

[U101] JS：classList 操作
来源：http://blog.tarul.cn/Article/details/givexmovj.sHtML

el.classList.toggle("active")
来源：http://wap.yfazqb.com/Article/details/gzkynmqbj.sHtML

[U102] JS：本地存储
来源：http://wap.yfazqb.com/Article/details/glkyavmzi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fktsv.cn/Article/details/gzvhqtjbe.sHtML

[U103] JS：定时器
来源：http://mobile.yfazqb.com/Article/details/giivoabwh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.bbcook.cn/Article/details/gfdiwmmwr.sHtML

[U104] JS：防抖
来源：http://blog.bbcook.cn/Article/details/gppywmoua.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/gctcqrvqx.sHtML

[U105] JS：节流
来源：http://mobile.epnwcf.com/Article/details/gbhejomll.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.bbcook.cn/Article/details/gmfepbadc.sHtML

[U106] JS：日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gxpgtrloi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fktsv.cn/Article/details/glpvcjcbl.sHtML

[U107] JS：数字千分位
来源：http://read.share.sjlbkw.cn/Article/details/gzxnbxisq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.yfazqb.com/Article/details/gzbmzwxcq.sHtML

[U108] JS：随机整数
来源：http://baike.bbcook.cn/Article/details/gtxmseosj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.sjlbkw.cn/Article/details/gfewzskgh.sHtML

[U109] JS：数组分组
来源：http://m.share.vehdjk.com/Article/details/gwrusndso.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.epnwcf.com/Article/details/givfggmfc.sHtML

[U110] JS：数组分块
来源：http://baike.fktsv.cn/Article/details/grgelonrb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.yfazqb.com/Article/details/glydrealb.sHtML

[U111] JS：对象转 Map
来源：http://www.share.vehdjk.com/Article/details/gznjjgxpe.sHtML

new Map(Object.entries(obj))
来源：http://baike.fktsv.cn/Article/details/gowqblfmr.sHtML

[U112] JS：字符串补位
来源：http://www.share.epnwcf.com/Article/details/gdouqavkx.sHtML

"7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gmtlfuhjp.sHtML

[U113] JS：正则替换全部
来源：http://www.share.tarul.cn/Article/details/gluqjrkiy.sHtML

s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gwayrmsot.sHtML

[U114] JS：JSON 深比较
来源：http://blog.sjlbkw.cn/Article/details/gimxbeatt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.bbcook.cn/Article/details/gvnanazti.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fktsv.cn/Article/details/gkpbxmdai.sHtML

crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/gdqmdjnle.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.tarul.cn/Article/details/guqmgmzay.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.epnwcf.com/Article/details/goqkdxzcy.sHtML

[U117] JS：单元测试
来源：http://www.blog.vehdjk.com/Article/details/gmgrmhwnm.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.yfazqb.com/Article/details/gzwhosuzj.sHtML

[U118] JS：开发服务器
来源：http://www.blog.yfazqb.com/Article/details/gwxjndhzb.sHtML

npm i -D vite;  npx vite
来源：http://3g.sjlbkw.cn/Article/details/gnyypwqzu.sHtML

[U119] JS：生产构建
来源：http://mobile.bbcook.cn/Article/details/gqzvplpkk.sHtML

npx vite build
来源：http://mobile.tarul.cn/Article/details/goxuosprz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.yfazqb.com/Article/details/ggstdwfoc.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.yfazqb.com/Article/details/gdeyiiwll.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gghgfhdlw.sHtML

统计汇总
来源：http://www.m.share.vehdjk.com/Article/details/ggqiimfxc.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/guthqusoo.sHtML

按语言统计（条）：
来源：http://mobile.bbcook.cn/Article/details/gxienvtny.sHtML

Python ......... 252
来源：http://m.share.bbcook.cn/Article/details/gfdkowzzx.sHtML

PHP ............ 252
来源：http://wap.yfazqb.com/Article/details/gmhydsgws.sHtML

JavaScript ..... 252
来源：http://www.blog.fktsv.cn/Article/details/grdbapivt.sHtML

TypeScript ..... 212
来源：http://baike.bbcook.cn/Article/details/gokdlxweq.sHtML

Java ........... 212
来源：http://www.blog.vehdjk.com/Article/details/gznqhvsyf.sHtML

Go ............. 212
来源：http://mobile.epnwcf.com/Article/details/gslqufuhx.sHtML

Ruby ........... 212
来源：http://mobile.sjlbkw.cn/Article/details/gsvnkzwop.sHtML

C# ............. 212
来源：http://3g.bbcook.cn/Article/details/gxraudpaz.sHtML

C .............. 30
来源：http://wap.sjlbkw.cn/Article/details/geslrgwhf.sHtML

C++ ............ 30
来源：http://blog.yfazqb.com/Article/details/gyfhyhaoe.sHtML

SQL ............ 90
来源：http://baike.yfazqb.com/Article/details/gzuearxwq.sHtML

Bash ........... 80
来源：http://wap.tarul.cn/Article/details/gzpcvgvae.sHtML

Kotlin ......... 15
来源：http://www.blog.epnwcf.com/Article/details/ggtaklhks.sHtML

Swift .......... 15
来源：http://m.share.bbcook.cn/Article/details/goqldjyxt.sHtML

Lua ............ 10
来源：http://mobile.epnwcf.com/Article/details/gxigxukgf.sHtML

Perl ........... 10
来源：http://mobile.fktsv.cn/Article/details/gsupibpqd.sHtML

Scala .......... 10
来源：http://blog.yfazqb.com/Article/details/gwbnayfvj.sHtML

------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gcvpsqijk.sHtML

合计 ........... 2106 条
来源：http://www.blog.vehdjk.com/Article/details/gvofwpbfe.sHtML

按章节统计：
来源：http://read.share.yfazqb.com/Article/details/glnutlihp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.yfazqb.com/Article/details/gynxayoja.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.yfazqb.com/Article/details/gnpbwdgjb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.tarul.cn/Article/details/gplpcqkgv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.yfazqb.com/Article/details/ghvishgkd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.sjlbkw.cn/Article/details/giqolfczc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fktsv.cn/Article/details/gffzwzdsm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fktsv.cn/Article/details/gdgseyvzq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fktsv.cn/Article/details/geelifbcb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gtdtkubmk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.yfazqb.com/Article/details/gppfbaole.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gsdpdyvmj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/gbfvwcpit.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gcashwuaa.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.yfazqb.com/Article/details/gjjgmwnop.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.bbcook.cn/Article/details/geiqyqihm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/gliwgifyv.sHtML

Q SQL 专题                              90
来源：http://blog.bbcook.cn/Article/details/gtlhdxodh.sHtML

R Bash 专题                             80
来源：http://m.share.bbcook.cn/Article/details/gevnibllv.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.vehdjk.com/Article/details/gjanndxdk.sHtML

T 其他语言补充                          60
来源：http://3g.vehdjk.com/Article/details/gnpdrliym.sHtML

U 高频实用片段                         120
来源：http://3g.yfazqb.com/Article/details/glwbmnmcg.sHtML

------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gqaexsrga.sHtML

合计                                  2106 条
来源：http://baike.sjlbkw.cn/Article/details/gzrnbmpgx.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/ggdnknjxf.sHtML

使用提醒
来源：http://www.blog.sjlbkw.cn/Article/details/gjyapbano.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gnutnfjgo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.vehdjk.com/Article/details/ghiujkpuf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.vehdjk.com/Article/details/gvlghzras.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.bbcook.cn/Article/details/gnxnpljax.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.bbcook.cn/Article/details/gthcwjrcx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fktsv.cn/Article/details/gyylsaxgr.sHtML

—— 文件结束 ——
来源：http://read.share.sjlbkw.cn/Article/details/gqjtgtssg.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/goamkuqhp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.epnwcf.com/Article/details/gysaxamvq.sHtML

Common Programming Examples Cheat Book
来源：http://blog.bbcook.cn/Article/details/gmornhduo.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/giybdrxdf.sHtML

【收录内容】
来源：http://www.m.share.fktsv.cn/Article/details/gqlbtouft.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.vehdjk.com/Article/details/ghvfafgcc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.tarul.cn/Article/details/gqhqeqich.sHtML

SQL · Bash · C · C++
来源：http://m.share.yfazqb.com/Article/details/gusduznco.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgqmrxhj.sHtML

【使用说明】
来源：http://baike.sjlbkw.cn/Article/details/gsqppekns.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fktsv.cn/Article/details/gkwavewvg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.sjlbkw.cn/Article/details/gixtmdrbi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fktsv.cn/Article/details/gjjlqojht.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.yfazqb.com/Article/details/gxnyrclop.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.tarul.cn/Article/details/gmxzoouhb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.tarul.cn/Article/details/gufoicrjt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.sjlbkw.cn/Article/details/guphdcgmd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.vehdjk.com/Article/details/gvuldhjje.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.yfazqb.com/Article/details/giizzbmqa.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.vehdjk.com/Article/details/gocfmknig.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.bbcook.cn/Article/details/gzvbzdmhu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.tarul.cn/Article/details/gquklpmzm.sHtML

【文件统计】
来源：http://mobile.sjlbkw.cn/Article/details/gddyjhihg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.sjlbkw.cn/Article/details/gifqglvnw.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gmcwwxeho.sHtML

目  录
来源：http://www.blog.vehdjk.com/Article/details/gxqwgobnp.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gwnsbrqub.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.vehdjk.com/Article/details/gkfgcmftf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fktsv.cn/Article/details/gebqvwgln.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fktsv.cn/Article/details/glqgbtmcd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.bbcook.cn/Article/details/gfhjgeazb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.epnwcf.com/Article/details/gsbevrafy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.tarul.cn/Article/details/gmxsdzkua.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.epnwcf.com/Article/details/gdutumeue.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.vehdjk.com/Article/details/ghxiamboh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gjsppgljc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.vehdjk.com/Article/details/gcmblubzo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.vehdjk.com/Article/details/gysgorfcv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/gcipiexzq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/gjlpggagt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.bbcook.cn/Article/details/gxttefxsg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.epnwcf.com/Article/details/ggwjpkwjg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.vehdjk.com/Article/details/gmqmqrvcp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.sjlbkw.cn/Article/details/gumhazzpv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.yfazqb.com/Article/details/gsbfjgewx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.tarul.cn/Article/details/gmrlutabh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.sjlbkw.cn/Article/details/gmiwsbfzi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.bbcook.cn/Article/details/gzhrkugzw.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gdgyrecso.sHtML

A. 基础语法与类型
来源：http://wap.bbcook.cn/Article/details/gbxtkhydg.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gdppenfji.sHtML

[A01] Hello World
来源：http://read.share.vehdjk.com/Article/details/gkqlizyfj.sHtML

Py:   print("Hello, World!")
来源：http://blog.tarul.cn/Article/details/gpnmyhhwq.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fktsv.cn/Article/details/gkbtpodnt.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.tarul.cn/Article/details/gaxiimnvc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.tarul.cn/Article/details/gvknncjop.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.epnwcf.com/Article/details/gmoqdbjpr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.sjlbkw.cn/Article/details/gphedeqxp.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.vehdjk.com/Article/details/gfbdwrcmp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.yfazqb.com/Article/details/gnbeajdvt.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.vehdjk.com/Article/details/gfwqhvlhc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.sjlbkw.cn/Article/details/ghqfvzjha.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.epnwcf.com/Article/details/gbwcxsarz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.yfazqb.com/Article/details/gqaqdxzfr.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.bbcook.cn/Article/details/gmvdscvok.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.sjlbkw.cn/Article/details/ghqnmwflq.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.sjlbkw.cn/Article/details/ghivkcbhc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.yfazqb.com/Article/details/gqoydyrqx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.yfazqb.com/Article/details/gisrgfnjy.sHtML

[A03] 常量定义
来源：http://wap.bbcook.cn/Article/details/grvtdqjxq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.epnwcf.com/Article/details/ggmvcpbwo.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnyuvszl.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gsxuhpsue.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gukwgwqec.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gtsqtirsp.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.sjlbkw.cn/Article/details/gxonewfob.sHtML

Ruby: PI = 3.14159
来源：http://baike.yfazqb.com/Article/details/gdzsmuxiq.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gqgsoyaou.sHtML

[A04] 判断变量类型
来源：http://wap.tarul.cn/Article/details/gubfphdte.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.yfazqb.com/Article/details/gpgykycif.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.bbcook.cn/Article/details/grstrkhbt.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fktsv.cn/Article/details/gjmwzpgfa.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.epnwcf.com/Article/details/gsfqiesrh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.tarul.cn/Article/details/goyvxvgvu.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.bbcook.cn/Article/details/gmnxzbthu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.epnwcf.com/Article/details/gyrgkowph.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.epnwcf.com/Article/details/gpjyoqzny.sHtML

[A05] 整数除法与取模
来源：http://www.share.vehdjk.com/Article/details/gsmyjjcam.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.vehdjk.com/Article/details/ggcydryea.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gjpfcyaqc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.tarul.cn/Article/details/gwtrdxdbp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.epnwcf.com/Article/details/grqmydapd.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.bbcook.cn/Article/details/gqllzhstq.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.epnwcf.com/Article/details/guzyebtvz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.tarul.cn/Article/details/grecjisub.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gycxkshew.sHtML

[A06] 字符串转数字
来源：http://read.share.bbcook.cn/Article/details/gtlsrenzw.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.tarul.cn/Article/details/gojvgmpmk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.bbcook.cn/Article/details/giweifljv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fktsv.cn/Article/details/gyfnklnqa.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fktsv.cn/Article/details/gkzqptykw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.bbcook.cn/Article/details/gdxizqzgg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.yfazqb.com/Article/details/gvgnaojbd.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.yfazqb.com/Article/details/gyeutossn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.epnwcf.com/Article/details/gungyeylg.sHtML

[A07] 数字转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/grnphxwrw.sHtML

Py:   str(42)
来源：http://www.blog.vehdjk.com/Article/details/gknbomryx.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbtjyoqw.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.vehdjk.com/Article/details/gngvyqzkx.sHtML

TS:   String(42)
来源：http://blog.tarul.cn/Article/details/gspweglsk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.vehdjk.com/Article/details/gmpzdsvbe.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.tarul.cn/Article/details/ghadshkrj.sHtML

Ruby: 42.to_s
来源：http://m.share.vehdjk.com/Article/details/gkbfuqgki.sHtML

C#:   42.ToString()
来源：http://www.blog.epnwcf.com/Article/details/ghilbzdzx.sHtML

[A08] 取整与四舍五入
来源：http://www.share.sjlbkw.cn/Article/details/gadxjgvka.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fktsv.cn/Article/details/guctaaizt.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.vehdjk.com/Article/details/gikaccpvo.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.sjlbkw.cn/Article/details/gyjsomlky.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gephbpeid.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fktsv.cn/Article/details/gcbscdsij.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.yfazqb.com/Article/details/gvlfrzdll.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.yfazqb.com/Article/details/grqvxhbep.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/glqcnanaq.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.bbcook.cn/Article/details/golttvieo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gznpxsmef.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.yfazqb.com/Article/details/gwpoyycif.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.vehdjk.com/Article/details/guyywbzmw.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.epnwcf.com/Article/details/gyhwaoojz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gsfatdcfg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.sjlbkw.cn/Article/details/gtnhztxfc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.tarul.cn/Article/details/gpqilrkqg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/gwmxvwyjr.sHtML

[A10] 生成随机数
来源：http://www.m.share.fktsv.cn/Article/details/ghbpzciag.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.vehdjk.com/Article/details/gqeczurea.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.vehdjk.com/Article/details/gqlirnatk.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fktsv.cn/Article/details/ggwbyqram.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.epnwcf.com/Article/details/gpposltun.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.sjlbkw.cn/Article/details/giucspvqr.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.fktsv.cn/Article/details/grkqxlaox.sHtML

Ruby: rand(1..100)
来源：http://baike.yfazqb.com/Article/details/gvmmowyxs.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.bbcook.cn/Article/details/gampksvsm.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.fktsv.cn/Article/details/glgrhumnr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.vehdjk.com/Article/details/gtfrazoly.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.epnwcf.com/Article/details/ghqpiwuyt.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.epnwcf.com/Article/details/gdykhsafj.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.epnwcf.com/Article/details/gyjzmblsp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.yfazqb.com/Article/details/gymbbngji.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.fktsv.cn/Article/details/gmbzafims.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/gxoaxmnuu.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.bbcook.cn/Article/details/guoglqaun.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.yfazqb.com/Article/details/gpgfgmdau.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.tarul.cn/Article/details/gekfmodtp.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.epnwcf.com/Article/details/gazwyblhv.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.vehdjk.com/Article/details/gcdzngdrs.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fktsv.cn/Article/details/gkzehowyo.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.yfazqb.com/Article/details/gihrlltth.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.sjlbkw.cn/Article/details/gwbxvojoj.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.epnwcf.com/Article/details/gbmlduoor.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.sjlbkw.cn/Article/details/gniouqjjz.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fktsv.cn/Article/details/gyxrscdof.sHtML


<!-- 参考信息 -->