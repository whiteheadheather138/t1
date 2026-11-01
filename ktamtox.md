代发 wailian999

[U81] JS：初始化项目
来源：http://www.m.share.tarul.cn/Article/details/gozhxerwr.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fktsv.cn/Article/details/giybszgiq.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.tarul.cn/Article/details/guzrsiyzx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fktsv.cn/Article/details/gwzaeivmg.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.tarul.cn/Article/details/gxlhyxett.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.vehdjk.com/Article/details/glpnvupfe.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.vehdjk.com/Article/details/gsgthlcps.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.tarul.cn/Article/details/gubjryxfe.sHtML

[U85] JS：可选链
来源：http://baike.tarul.cn/Article/details/gafdhhzlk.sHtML

a?.b?.c
来源：http://www.m.share.bbcook.cn/Article/details/gsxgugdcj.sHtML

[U86] JS：空值合并
来源：http://mobile.sjlbkw.cn/Article/details/gqabxmnhv.sHtML

a ?? b
来源：http://baike.yfazqb.com/Article/details/gxnnxmxmc.sHtML

[U87] JS：解构默认值
来源：http://read.share.tarul.cn/Article/details/gpybuwzjy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.epnwcf.com/Article/details/goqbhyvlu.sHtML

[U88] JS：对象展开合并
来源：http://blog.tarul.cn/Article/details/grgnigios.sHtML

{ ...a, ...b }
来源：http://mobile.fktsv.cn/Article/details/gsxjbnsjr.sHtML

[U89] JS：数组去重
来源：http://www.share.epnwcf.com/Article/details/gzkagorsp.sHtML

[...new Set(arr)]
来源：http://read.share.sjlbkw.cn/Article/details/grqestczu.sHtML

[U90] JS：数字数组排序
来源：http://wap.vehdjk.com/Article/details/gyhoagppp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/gvtwndzfh.sHtML

[U91] JS：对象键值遍历
来源：http://wap.yfazqb.com/Article/details/gcnrgzvse.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fktsv.cn/Article/details/gblyiymfb.sHtML

[U92] JS：深拷贝
来源：http://wap.fktsv.cn/Article/details/gdwyvcfbg.sHtML

structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gnoxgdwco.sHtML

[U93] JS：模板字符串
来源：http://read.share.sjlbkw.cn/Article/details/gomadjmbx.sHtML

`共 ${n} 条`
来源：http://www.blog.fktsv.cn/Article/details/gptgdsboe.sHtML

[U94] JS：箭头函数
来源：http://m.share.vehdjk.com/Article/details/gvrucvmed.sHtML

const double = x => x * 2;
来源：http://wap.bbcook.cn/Article/details/ggvhsyvky.sHtML

[U95] JS：Promise 包装
来源：http://3g.tarul.cn/Article/details/gfnjsjpbb.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.bbcook.cn/Article/details/gdqjvtybf.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fktsv.cn/Article/details/gbwongjsd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/gyvhkudao.sHtML

[U97] JS：并发请求
来源：http://www.blog.tarul.cn/Article/details/gptvoeyhu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/grhppohmg.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.bbcook.cn/Article/details/gutoflwjb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.epnwcf.com/Article/details/gjmfiavkm.sHtML

[U99] JS：事件监听
来源：http://wap.bbcook.cn/Article/details/glwxsubaz.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fktsv.cn/Article/details/gvpuqyyzc.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.vehdjk.com/Article/details/grljwyxtr.sHtML

document.querySelector(".item")
来源：http://baike.sjlbkw.cn/Article/details/gsogqbend.sHtML

[U101] JS：classList 操作
来源：http://3g.yfazqb.com/Article/details/ggsxvccgt.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fktsv.cn/Article/details/grwaowmrw.sHtML

[U102] JS：本地存储
来源：http://www.blog.bbcook.cn/Article/details/gxzpndwvi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.vehdjk.com/Article/details/giwlaklrq.sHtML

[U103] JS：定时器
来源：http://3g.fktsv.cn/Article/details/gfaolkrze.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.tarul.cn/Article/details/gwzpipcpw.sHtML

[U104] JS：防抖
来源：http://m.share.vehdjk.com/Article/details/gljcwiocl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.epnwcf.com/Article/details/gjhajbkyi.sHtML

[U105] JS：节流
来源：http://www.blog.tarul.cn/Article/details/gmdsteorq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.bbcook.cn/Article/details/gcpdlgqfg.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fktsv.cn/Article/details/glyfnolzv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.bbcook.cn/Article/details/gitjrxwpj.sHtML

[U107] JS：数字千分位
来源：http://mobile.sjlbkw.cn/Article/details/ghxtqqmmh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.epnwcf.com/Article/details/gknsrqfze.sHtML

[U108] JS：随机整数
来源：http://mobile.bbcook.cn/Article/details/gzonampvb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.vehdjk.com/Article/details/gwbvmuaap.sHtML

[U109] JS：数组分组
来源：http://www.blog.epnwcf.com/Article/details/gqodjnjnp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.sjlbkw.cn/Article/details/ggdxcpvpa.sHtML

[U110] JS：数组分块
来源：http://wap.epnwcf.com/Article/details/gnlascabb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fktsv.cn/Article/details/gppogpbeb.sHtML

[U111] JS：对象转 Map
来源：http://wap.sjlbkw.cn/Article/details/giitrbqfx.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fktsv.cn/Article/details/gpdktdlpr.sHtML

[U112] JS：字符串补位
来源：http://m.share.epnwcf.com/Article/details/ghzgnnqpi.sHtML

"7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gzqiyxflb.sHtML

[U113] JS：正则替换全部
来源：http://m.share.tarul.cn/Article/details/gwpmmpcfm.sHtML

s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gjergsdml.sHtML

[U114] JS：JSON 深比较
来源：http://wap.sjlbkw.cn/Article/details/ghjqnpafv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/gqregayil.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.bbcook.cn/Article/details/gdmnhykbh.sHtML

crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/glbskxorr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.yfazqb.com/Article/details/gopjjveib.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.bbcook.cn/Article/details/gziwmgqhb.sHtML

[U117] JS：单元测试
来源：http://m.share.tarul.cn/Article/details/gkthedhfg.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.yfazqb.com/Article/details/gfkkrhrcx.sHtML

[U118] JS：开发服务器
来源：http://read.share.vehdjk.com/Article/details/gkqjyhdcn.sHtML

npm i -D vite;  npx vite
来源：http://baike.fktsv.cn/Article/details/gkuxhfwnc.sHtML

[U119] JS：生产构建
来源：http://www.blog.epnwcf.com/Article/details/gbvudqlfc.sHtML

npx vite build
来源：http://www.blog.fktsv.cn/Article/details/ghhniqfhh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.tarul.cn/Article/details/gjeoffhcc.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.epnwcf.com/Article/details/gdqlrlfxp.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfervtzd.sHtML

统计汇总
来源：http://3g.bbcook.cn/Article/details/gfzftgpcf.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gjibhizji.sHtML

按语言统计（条）：
来源：http://www.blog.sjlbkw.cn/Article/details/gbiysduxe.sHtML

Python ......... 252
来源：http://www.share.yfazqb.com/Article/details/gdnhvstqg.sHtML

PHP ............ 252
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpjeochy.sHtML

JavaScript ..... 252
来源：http://m.share.yfazqb.com/Article/details/gtnxpuurb.sHtML

TypeScript ..... 212
来源：http://read.share.bbcook.cn/Article/details/gnkqanqgs.sHtML

Java ........... 212
来源：http://wap.sjlbkw.cn/Article/details/gtddgfmqo.sHtML

Go ............. 212
来源：http://www.blog.sjlbkw.cn/Article/details/gudbdyzwp.sHtML

Ruby ........... 212
来源：http://3g.epnwcf.com/Article/details/gytjelaji.sHtML

C# ............. 212
来源：http://www.blog.epnwcf.com/Article/details/gjznekeej.sHtML

C .............. 30
来源：http://blog.bbcook.cn/Article/details/grnvfubml.sHtML

C++ ............ 30
来源：http://3g.fktsv.cn/Article/details/gzwavzfss.sHtML

SQL ............ 90
来源：http://www.share.tarul.cn/Article/details/gsgnbpyvu.sHtML

Bash ........... 80
来源：http://blog.yfazqb.com/Article/details/grbvmbbov.sHtML

Kotlin ......... 15
来源：http://blog.yfazqb.com/Article/details/gdnmaedoi.sHtML

Swift .......... 15
来源：http://www.blog.tarul.cn/Article/details/ghnusvfns.sHtML

Lua ............ 10
来源：http://www.share.vehdjk.com/Article/details/gzkkjraly.sHtML

Perl ........... 10
来源：http://mobile.bbcook.cn/Article/details/gpurkpskb.sHtML

Scala .......... 10
来源：http://read.share.fktsv.cn/Article/details/gejjdqhex.sHtML

------------------------------------
来源：http://blog.vehdjk.com/Article/details/gqnoeaxog.sHtML

合计 ........... 2106 条
来源：http://mobile.sjlbkw.cn/Article/details/gxczzffvl.sHtML

按章节统计：
来源：http://www.blog.sjlbkw.cn/Article/details/gujvgihwm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.sjlbkw.cn/Article/details/gtvhhsscn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.sjlbkw.cn/Article/details/goikldbsv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.bbcook.cn/Article/details/gowhaofmy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.yfazqb.com/Article/details/gjyvlcdic.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.vehdjk.com/Article/details/gjqlbcyxl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.vehdjk.com/Article/details/glwtbzfri.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.tarul.cn/Article/details/ghlqrjmyt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.bbcook.cn/Article/details/gdixxmdww.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gikdeyrur.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.sjlbkw.cn/Article/details/gmyskpwhi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/ghojmrbyo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gftfgpqet.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gyyinrqde.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.yfazqb.com/Article/details/ggpipfnzl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.tarul.cn/Article/details/gnpkjeuci.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/guwmkqvxk.sHtML

Q SQL 专题                              90
来源：http://read.share.sjlbkw.cn/Article/details/glgoernii.sHtML

R Bash 专题                             80
来源：http://www.m.share.fktsv.cn/Article/details/gxbnzklzr.sHtML

S C / C++ 专题                          60
来源：http://blog.bbcook.cn/Article/details/gnzpqhikr.sHtML

T 其他语言补充                          60
来源：http://mobile.vehdjk.com/Article/details/gjosmswkl.sHtML

U 高频实用片段                         120
来源：http://3g.tarul.cn/Article/details/gewllqbdw.sHtML

------------------------------------
来源：http://3g.bbcook.cn/Article/details/gkluufyrb.sHtML

合计                                  2106 条
来源：http://wap.vehdjk.com/Article/details/ghqiiayxy.sHtML

--------------------------------------------------------------------------------
来源：http://wap.yfazqb.com/Article/details/grcnlecbj.sHtML

使用提醒
来源：http://www.m.share.bbcook.cn/Article/details/gcbbovaud.sHtML

--------------------------------------------------------------------------------
来源：http://3g.tarul.cn/Article/details/gnyynjuro.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.vehdjk.com/Article/details/ghcdloyzg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fktsv.cn/Article/details/glvkmtuji.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.vehdjk.com/Article/details/gqsqnpvei.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.tarul.cn/Article/details/ggrdqggba.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.vehdjk.com/Article/details/gcyswfsbo.sHtML

—— 文件结束 ——
来源：http://www.blog.tarul.cn/Article/details/gsuceihxn.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ginpbxabs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.yfazqb.com/Article/details/gxkhdtwyc.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.tarul.cn/Article/details/gmddvfgsf.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ghqzzkrcx.sHtML

【收录内容】
来源：http://www.m.share.fktsv.cn/Article/details/gqhilkqto.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.bbcook.cn/Article/details/gdbqbznks.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.bbcook.cn/Article/details/gikqlgmew.sHtML

SQL · Bash · C · C++
来源：http://read.share.sjlbkw.cn/Article/details/gcgdpmyln.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.epnwcf.com/Article/details/gyiunyknz.sHtML

【使用说明】
来源：http://www.m.share.bbcook.cn/Article/details/gxkwkukho.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.epnwcf.com/Article/details/gedozotlp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.yfazqb.com/Article/details/gymobxfoy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.vehdjk.com/Article/details/gfkgesrtk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.sjlbkw.cn/Article/details/gsqqvonjy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.yfazqb.com/Article/details/gxwwfnnzh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.bbcook.cn/Article/details/guexosnxr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.tarul.cn/Article/details/grekjpexi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fktsv.cn/Article/details/gfodurekg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.sjlbkw.cn/Article/details/guwuqcoyb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.epnwcf.com/Article/details/gbfysinox.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.sjlbkw.cn/Article/details/gasvqbjiu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.yfazqb.com/Article/details/gotvaleos.sHtML

【文件统计】
来源：http://www.share.tarul.cn/Article/details/gnojzamgz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.vehdjk.com/Article/details/gmxjwxbbb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/gwfcsrfej.sHtML

目  录
来源：http://3g.epnwcf.com/Article/details/gdpatxvbi.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/grzhonfns.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.sjlbkw.cn/Article/details/gecwbjrrh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.vehdjk.com/Article/details/gujinmuzx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.epnwcf.com/Article/details/ghvqpmoou.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.epnwcf.com/Article/details/gxkxdituo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.epnwcf.com/Article/details/ghgixilyy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.yfazqb.com/Article/details/gfidgjhkg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fktsv.cn/Article/details/gdcpbbpyz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwmorqwl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.epnwcf.com/Article/details/gmmrmwfrc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.epnwcf.com/Article/details/gstlfgcnr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gzhbrzkvj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fktsv.cn/Article/details/glsmeouqh.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/ghxmatteb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.vehdjk.com/Article/details/gfixkqxne.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.bbcook.cn/Article/details/grhjqtsry.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.epnwcf.com/Article/details/gomfhqvhw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.bbcook.cn/Article/details/gsobpcaxy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.bbcook.cn/Article/details/gxphwxtnt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.tarul.cn/Article/details/gifalpyjz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.sjlbkw.cn/Article/details/gtaxudseb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.sjlbkw.cn/Article/details/gnunulzhu.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gygqymksa.sHtML

A. 基础语法与类型
来源：http://wap.yfazqb.com/Article/details/gntkqokme.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gunibokja.sHtML

[A01] Hello World
来源：http://m.share.epnwcf.com/Article/details/grhnikqra.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.sjlbkw.cn/Article/details/goxqbngqx.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.tarul.cn/Article/details/gctjfilbr.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.sjlbkw.cn/Article/details/gsfjjmzvg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fktsv.cn/Article/details/gkycituzl.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.tarul.cn/Article/details/gaqmvswqy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.vehdjk.com/Article/details/gtaamxygd.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fktsv.cn/Article/details/gbtyxlzrd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.sjlbkw.cn/Article/details/gkywmftkl.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.epnwcf.com/Article/details/ghlynvrmt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fktsv.cn/Article/details/gdrggaeqk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/glodaatwl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gefegnutd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.vehdjk.com/Article/details/gbjxvmtzu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gemqxisei.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fktsv.cn/Article/details/guydfzdqp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fktsv.cn/Article/details/gzuxcjkgr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.epnwcf.com/Article/details/geswceipi.sHtML

[A03] 常量定义
来源：http://m.share.tarul.cn/Article/details/gvkrsrcbn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.sjlbkw.cn/Article/details/gbldyxqjr.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gpidajwih.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gvenbsxsc.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gfmcqfsqs.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gozmxowsw.sHtML

Go:   const PI = 3.14159
来源：http://wap.epnwcf.com/Article/details/gufsgjwzo.sHtML

Ruby: PI = 3.14159
来源：http://wap.fktsv.cn/Article/details/ggahicfuk.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gdfdezxyo.sHtML

[A04] 判断变量类型
来源：http://wap.yfazqb.com/Article/details/gbbnsgruq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.yfazqb.com/Article/details/gwgmdtets.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.vehdjk.com/Article/details/gzbmcggqr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.bbcook.cn/Article/details/gmrarcjsp.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.epnwcf.com/Article/details/gyoispqxh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.bbcook.cn/Article/details/gkbgdklsr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.yfazqb.com/Article/details/gdvfkztjy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.bbcook.cn/Article/details/gwuvdwbun.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.sjlbkw.cn/Article/details/gxaimjjbw.sHtML

[A05] 整数除法与取模
来源：http://mobile.epnwcf.com/Article/details/gwniwkoeo.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fktsv.cn/Article/details/gxkvbmdre.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fktsv.cn/Article/details/gczvvxshb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.tarul.cn/Article/details/gmwgyuihb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gqtjuepbd.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.tarul.cn/Article/details/gmwvpcqar.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gwdkdcfpm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/gmlhcvfaz.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gppnpdbgs.sHtML

[A06] 字符串转数字
来源：http://www.share.vehdjk.com/Article/details/gcjewvzoe.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.sjlbkw.cn/Article/details/gwpgwlfgk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.yfazqb.com/Article/details/gsbikvxpu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.yfazqb.com/Article/details/ggbuqqtdp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.yfazqb.com/Article/details/girvppdad.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.vehdjk.com/Article/details/gwxarmjie.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.bbcook.cn/Article/details/ggvfyvnbr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.tarul.cn/Article/details/gciyxjngz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.vehdjk.com/Article/details/gdmkudiol.sHtML

[A07] 数字转字符串
来源：http://wap.sjlbkw.cn/Article/details/gmewqpiju.sHtML

Py:   str(42)
来源：http://read.share.tarul.cn/Article/details/gtloniskc.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fktsv.cn/Article/details/gucsibvph.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.vehdjk.com/Article/details/gvxxvzjbj.sHtML

TS:   String(42)
来源：http://3g.yfazqb.com/Article/details/gdawziotn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.bbcook.cn/Article/details/gemckvlfw.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.sjlbkw.cn/Article/details/gscvsrxml.sHtML

Ruby: 42.to_s
来源：http://read.share.epnwcf.com/Article/details/guunwygxx.sHtML

C#:   42.ToString()
来源：http://www.share.tarul.cn/Article/details/gvelzqvuf.sHtML

[A08] 取整与四舍五入
来源：http://www.share.sjlbkw.cn/Article/details/ggafvevuo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/gbkfytuob.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.bbcook.cn/Article/details/glnqovzbp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/gzszncrwx.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.yfazqb.com/Article/details/gbtmuaxtf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.sjlbkw.cn/Article/details/ggwimbvyy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fktsv.cn/Article/details/gtwlprpxa.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.vehdjk.com/Article/details/gxocgaktz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fktsv.cn/Article/details/gwbjxvlyz.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.bbcook.cn/Article/details/gcncrrguq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gdwpdvfcq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.tarul.cn/Article/details/gzsedzuaz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.bbcook.cn/Article/details/gwpfzuqod.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.yfazqb.com/Article/details/ghgzsrmdp.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.tarul.cn/Article/details/grjfpfqhm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.tarul.cn/Article/details/gcuiupaek.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.vehdjk.com/Article/details/gtemtosxx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gwsczirzc.sHtML

[A10] 生成随机数
来源：http://www.share.bbcook.cn/Article/details/gehzmwjcj.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.tarul.cn/Article/details/gvcxgtcoa.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.tarul.cn/Article/details/gvopetumi.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.tarul.cn/Article/details/gsbeipmyv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.tarul.cn/Article/details/gqedhqbxv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.vehdjk.com/Article/details/ggblhlwqs.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.vehdjk.com/Article/details/gugrhsiyp.sHtML

Ruby: rand(1..100)
来源：http://wap.sjlbkw.cn/Article/details/glndrrdyg.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.fktsv.cn/Article/details/gtwitgtnx.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.vehdjk.com/Article/details/gkxokrefo.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.yfazqb.com/Article/details/goljvwbnf.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.bbcook.cn/Article/details/gckbfkzew.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.yfazqb.com/Article/details/gaokdksni.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.vehdjk.com/Article/details/ggmeyvodr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.tarul.cn/Article/details/gssiizzxq.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.yfazqb.com/Article/details/grymvwoqm.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.epnwcf.com/Article/details/geqckysxy.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.vehdjk.com/Article/details/gekfyajko.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.bbcook.cn/Article/details/geoqzhlws.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.tarul.cn/Article/details/gwhbetiwb.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.fktsv.cn/Article/details/gkibkclqt.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.yfazqb.com/Article/details/gbecxjzwz.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.sjlbkw.cn/Article/details/gjuwmmvzy.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.tarul.cn/Article/details/gfuxbjglj.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.yfazqb.com/Article/details/glatpxsjw.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.yfazqb.com/Article/details/gqltwhgug.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.sjlbkw.cn/Article/details/gntzshopr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.tarul.cn/Article/details/gdmlbecfl.sHtML

Py:   "第一行\n第二行"
来源：http://wap.epnwcf.com/Article/details/gudaozyyy.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fktsv.cn/Article/details/gqpyfcfll.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.fktsv.cn/Article/details/gahiyuado.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fktsv.cn/Article/details/ghmhblbcy.sHtML


<!-- 参考信息 -->