代发 wailian999

[U77] PHP：模板渲染
来源：http://baike.vehdjk.com/Article/details/glgqzxkam.sHtML

composer require twig/twig
来源：http://blog.yfazqb.com/Article/details/gqiisaijz.sHtML

[U78] PHP：单元测试
来源：http://baike.vehdjk.com/Article/details/gfnnataht.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.tarul.cn/Article/details/gqrbhdhdo.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.epnwcf.com/Article/details/gzsggomhj.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.tarul.cn/Article/details/gijnzpbgf.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.sjlbkw.cn/Article/details/gtndffzhq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.vehdjk.com/Article/details/gpcybytes.sHtML

[U81] JS：初始化项目
来源：http://3g.yfazqb.com/Article/details/gchfivubv.sHtML

npm init -y;  npm i express
来源：http://read.share.yfazqb.com/Article/details/glpvwmgue.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.tarul.cn/Article/details/gyxhsetuf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.vehdjk.com/Article/details/gsihdyapf.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.vehdjk.com/Article/details/gwjdujimg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.vehdjk.com/Article/details/gipurukgu.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fktsv.cn/Article/details/gerelayxn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.bbcook.cn/Article/details/gxqklbgod.sHtML

[U85] JS：可选链
来源：http://m.share.epnwcf.com/Article/details/gadadivxh.sHtML

a?.b?.c
来源：http://www.m.share.epnwcf.com/Article/details/ghgxoszsg.sHtML

[U86] JS：空值合并
来源：http://read.share.sjlbkw.cn/Article/details/gwcdvxazc.sHtML

a ?? b
来源：http://wap.fktsv.cn/Article/details/gbymrluyl.sHtML

[U87] JS：解构默认值
来源：http://blog.bbcook.cn/Article/details/gxgwkvjgf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.yfazqb.com/Article/details/gnmfqhxwg.sHtML

[U88] JS：对象展开合并
来源：http://m.share.vehdjk.com/Article/details/gfdqnhxmg.sHtML

{ ...a, ...b }
来源：http://baike.vehdjk.com/Article/details/gyajhwufl.sHtML

[U89] JS：数组去重
来源：http://www.share.yfazqb.com/Article/details/gdqsdguub.sHtML

[...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gpnwszlfh.sHtML

[U90] JS：数字数组排序
来源：http://www.share.bbcook.cn/Article/details/guzgvkdhk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gohhpetky.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.vehdjk.com/Article/details/gbocienjf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.sjlbkw.cn/Article/details/gzzianctr.sHtML

[U92] JS：深拷贝
来源：http://read.share.fktsv.cn/Article/details/gxczybjpo.sHtML

structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gnrabcsyl.sHtML

[U93] JS：模板字符串
来源：http://www.blog.epnwcf.com/Article/details/gtmqnpxfk.sHtML

`共 ${n} 条`
来源：http://www.m.share.bbcook.cn/Article/details/gyoyssics.sHtML

[U94] JS：箭头函数
来源：http://m.share.tarul.cn/Article/details/gdooqqmau.sHtML

const double = x => x * 2;
来源：http://m.share.sjlbkw.cn/Article/details/gekkumomt.sHtML

[U95] JS：Promise 包装
来源：http://www.share.yfazqb.com/Article/details/gaifsbjeq.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.tarul.cn/Article/details/givowddlz.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.yfazqb.com/Article/details/gahjcdvzf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/gknlyyooa.sHtML

[U97] JS：并发请求
来源：http://blog.yfazqb.com/Article/details/gfvsedjym.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gltogirnp.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.bbcook.cn/Article/details/ggryjcvus.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.epnwcf.com/Article/details/ggizmvsry.sHtML

[U99] JS：事件监听
来源：http://www.blog.fktsv.cn/Article/details/gmcgjdwag.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.bbcook.cn/Article/details/grsltaqrd.sHtML

[U100] JS：DOM 查询
来源：http://3g.tarul.cn/Article/details/gzavrtcwh.sHtML

document.querySelector(".item")
来源：http://3g.bbcook.cn/Article/details/gwctksflx.sHtML

[U101] JS：classList 操作
来源：http://www.share.epnwcf.com/Article/details/gctpwbige.sHtML

el.classList.toggle("active")
来源：http://www.share.sjlbkw.cn/Article/details/goigoggvh.sHtML

[U102] JS：本地存储
来源：http://www.m.share.yfazqb.com/Article/details/gntswgxqk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.bbcook.cn/Article/details/gkndiqxkw.sHtML

[U103] JS：定时器
来源：http://www.blog.epnwcf.com/Article/details/gzevlmach.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.vehdjk.com/Article/details/ggovnghkg.sHtML

[U104] JS：防抖
来源：http://read.share.fktsv.cn/Article/details/glsphibrf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/goymiovfo.sHtML

[U105] JS：节流
来源：http://3g.fktsv.cn/Article/details/gdofolnlo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.bbcook.cn/Article/details/gsltngipj.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/gftkhpicv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.bbcook.cn/Article/details/gspkejlhp.sHtML

[U107] JS：数字千分位
来源：http://3g.vehdjk.com/Article/details/gkbwcylpr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.vehdjk.com/Article/details/gnpuwqhmd.sHtML

[U108] JS：随机整数
来源：http://read.share.yfazqb.com/Article/details/gfayvklze.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.bbcook.cn/Article/details/gzcgtwgxz.sHtML

[U109] JS：数组分组
来源：http://m.share.epnwcf.com/Article/details/gmeeqjkis.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.tarul.cn/Article/details/ggxzvzxvs.sHtML

[U110] JS：数组分块
来源：http://read.share.bbcook.cn/Article/details/gugvddfew.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.tarul.cn/Article/details/gwjjdwkga.sHtML

[U111] JS：对象转 Map
来源：http://mobile.bbcook.cn/Article/details/gaiirdywi.sHtML

new Map(Object.entries(obj))
来源：http://www.share.tarul.cn/Article/details/grcpiowlg.sHtML

[U112] JS：字符串补位
来源：http://blog.vehdjk.com/Article/details/gnuezerzz.sHtML

"7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gkpuqyerr.sHtML

[U113] JS：正则替换全部
来源：http://m.share.bbcook.cn/Article/details/gdviuybte.sHtML

s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gsruwpmua.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.vehdjk.com/Article/details/gcbjadynr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.yfazqb.com/Article/details/gbvhltklq.sHtML

[U115] JS：生成 UUID
来源：http://m.share.vehdjk.com/Article/details/gdtafmpny.sHtML

crypto.randomUUID()
来源：http://www.share.bbcook.cn/Article/details/gfnraxvdn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.vehdjk.com/Article/details/gwjqnwcyo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.sjlbkw.cn/Article/details/gjpumtggt.sHtML

[U117] JS：单元测试
来源：http://www.share.bbcook.cn/Article/details/gxvmuqqql.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.tarul.cn/Article/details/ghevzwoov.sHtML

[U118] JS：开发服务器
来源：http://www.share.epnwcf.com/Article/details/gxupadwlu.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fktsv.cn/Article/details/gkdxyfpej.sHtML

[U119] JS：生产构建
来源：http://baike.yfazqb.com/Article/details/gnyljlldd.sHtML

npx vite build
来源：http://www.blog.sjlbkw.cn/Article/details/grlggtkgt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.sjlbkw.cn/Article/details/gdrdmkkgd.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.vehdjk.com/Article/details/gvpovyefg.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/glrodztqg.sHtML

统计汇总
来源：http://read.share.sjlbkw.cn/Article/details/gnpodfrvb.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ggvmewqlu.sHtML

按语言统计（条）：
来源：http://read.share.fktsv.cn/Article/details/grsbnjuzk.sHtML

Python ......... 252
来源：http://wap.bbcook.cn/Article/details/gjocasmql.sHtML

PHP ............ 252
来源：http://blog.bbcook.cn/Article/details/gfgauysjv.sHtML

JavaScript ..... 252
来源：http://www.blog.yfazqb.com/Article/details/gmdcrebbu.sHtML

TypeScript ..... 212
来源：http://baike.fktsv.cn/Article/details/gvlkjkhkc.sHtML

Java ........... 212
来源：http://blog.epnwcf.com/Article/details/gmjbjzpcc.sHtML

Go ............. 212
来源：http://read.share.bbcook.cn/Article/details/gpnqmgjvg.sHtML

Ruby ........... 212
来源：http://baike.epnwcf.com/Article/details/gbyyopgww.sHtML

C# ............. 212
来源：http://mobile.bbcook.cn/Article/details/gdtewoazr.sHtML

C .............. 30
来源：http://blog.epnwcf.com/Article/details/gljljitxa.sHtML

C++ ............ 30
来源：http://www.share.fktsv.cn/Article/details/grhnepkog.sHtML

SQL ............ 90
来源：http://baike.vehdjk.com/Article/details/gapjywvve.sHtML

Bash ........... 80
来源：http://read.share.vehdjk.com/Article/details/gchbcsxlh.sHtML

Kotlin ......... 15
来源：http://www.blog.vehdjk.com/Article/details/gauiuwgpo.sHtML

Swift .......... 15
来源：http://read.share.fktsv.cn/Article/details/gnvbmcpsc.sHtML

Lua ............ 10
来源：http://wap.bbcook.cn/Article/details/guamqrwru.sHtML

Perl ........... 10
来源：http://www.m.share.fktsv.cn/Article/details/gdeiqvytx.sHtML

Scala .......... 10
来源：http://blog.vehdjk.com/Article/details/grdpdbkja.sHtML

------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gcirhmqin.sHtML

合计 ........... 2106 条
来源：http://www.share.yfazqb.com/Article/details/gadtleufr.sHtML

按章节统计：
来源：http://blog.vehdjk.com/Article/details/gtznyllav.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.yfazqb.com/Article/details/guawlgdih.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.bbcook.cn/Article/details/gtkjnfjwj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.yfazqb.com/Article/details/gtsmyrukz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.vehdjk.com/Article/details/gkgdymtdt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.yfazqb.com/Article/details/gjitpyztr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.bbcook.cn/Article/details/gwrgkhvpp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqaggvqa.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.bbcook.cn/Article/details/gpasrzjjq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gkdozwgkp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.tarul.cn/Article/details/gdhzxymoa.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gmitbwfmq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/gjbskvfby.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/gnfwcozzy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.vehdjk.com/Article/details/ghjftzybo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.epnwcf.com/Article/details/gwecxjdcw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.sjlbkw.cn/Article/details/govejxmgn.sHtML

Q SQL 专题                              90
来源：http://3g.yfazqb.com/Article/details/gmnyznvbl.sHtML

R Bash 专题                             80
来源：http://3g.fktsv.cn/Article/details/gzaaaodem.sHtML

S C / C++ 专题                          60
来源：http://mobile.yfazqb.com/Article/details/gfupkqmvk.sHtML

T 其他语言补充                          60
来源：http://blog.yfazqb.com/Article/details/gqvghwirq.sHtML

U 高频实用片段                         120
来源：http://baike.epnwcf.com/Article/details/gdtjhegqb.sHtML

------------------------------------
来源：http://3g.yfazqb.com/Article/details/gayseharc.sHtML

合计                                  2106 条
来源：http://wap.yfazqb.com/Article/details/gdjagfrhl.sHtML

--------------------------------------------------------------------------------
来源：http://blog.yfazqb.com/Article/details/goaxebruo.sHtML

使用提醒
来源：http://mobile.yfazqb.com/Article/details/gjskwzgxh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gjhqudcdh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.yfazqb.com/Article/details/gdoudofkh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fktsv.cn/Article/details/gaijbstxk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.tarul.cn/Article/details/gqkkahywp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.sjlbkw.cn/Article/details/gvbkmyhoh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.epnwcf.com/Article/details/glelvomax.sHtML

—— 文件结束 ——
来源：http://www.blog.sjlbkw.cn/Article/details/gykilmdin.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gvkmhyday.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.sjlbkw.cn/Article/details/gmyokcpzh.sHtML

Common Programming Examples Cheat Book
来源：http://baike.sjlbkw.cn/Article/details/gefmtrapk.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/glewyymsd.sHtML

【收录内容】
来源：http://m.share.vehdjk.com/Article/details/gcgncwhdm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.yfazqb.com/Article/details/gzjvolsrr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.vehdjk.com/Article/details/ggovwmlym.sHtML

SQL · Bash · C · C++
来源：http://baike.tarul.cn/Article/details/gdijuzlzc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.sjlbkw.cn/Article/details/gorfwtmuh.sHtML

【使用说明】
来源：http://mobile.bbcook.cn/Article/details/ghnwkavyg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fktsv.cn/Article/details/gpovtexks.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.sjlbkw.cn/Article/details/giqovwdnj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.yfazqb.com/Article/details/gccjhjnhw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.vehdjk.com/Article/details/gbzvvfzko.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.sjlbkw.cn/Article/details/gykwtnzcx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.epnwcf.com/Article/details/gsnaxvrke.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.epnwcf.com/Article/details/gydfgorqs.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.tarul.cn/Article/details/ghlsfvpnm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.vehdjk.com/Article/details/gciayoioo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.bbcook.cn/Article/details/gdmbksqzk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fktsv.cn/Article/details/gcspnkrvv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.yfazqb.com/Article/details/ggcconvkz.sHtML

【文件统计】
来源：http://baike.bbcook.cn/Article/details/glplvalqz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.bbcook.cn/Article/details/gzuqxmrir.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/ghwmetqyi.sHtML

目  录
来源：http://www.blog.vehdjk.com/Article/details/gemzrxepg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.bbcook.cn/Article/details/glzkzmnva.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.vehdjk.com/Article/details/gzzfkrxvm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.bbcook.cn/Article/details/ghvddwhpf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.sjlbkw.cn/Article/details/geqqgnftr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fktsv.cn/Article/details/gebocegof.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fktsv.cn/Article/details/gncmdraxp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.tarul.cn/Article/details/gbivnfpth.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.epnwcf.com/Article/details/gccxsqdbx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.yfazqb.com/Article/details/gofqawske.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.bbcook.cn/Article/details/glageoqha.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.bbcook.cn/Article/details/gdplrjrrr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/gaobgjkvt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/gvkdbarfz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.vehdjk.com/Article/details/gdugczuzi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.bbcook.cn/Article/details/gsgafougv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.vehdjk.com/Article/details/gkjomjyuo.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/gqvawmils.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.epnwcf.com/Article/details/gzyxacgsa.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.epnwcf.com/Article/details/gnaplklpy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.bbcook.cn/Article/details/gxyhlypvh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.yfazqb.com/Article/details/gnfxewmiq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fktsv.cn/Article/details/gljfhxzus.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gqkvmyvhp.sHtML

A. 基础语法与类型
来源：http://read.share.tarul.cn/Article/details/gxxnsmrrh.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gjgvtfmnt.sHtML

[A01] Hello World
来源：http://wap.sjlbkw.cn/Article/details/gtkhgpivc.sHtML

Py:   print("Hello, World!")
来源：http://3g.fktsv.cn/Article/details/gvdiktdsn.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.yfazqb.com/Article/details/gfclfjhzc.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.yfazqb.com/Article/details/guswkrcmw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fktsv.cn/Article/details/gmvsgurib.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.yfazqb.com/Article/details/gftmhzwvi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.bbcook.cn/Article/details/gbtcolodj.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.sjlbkw.cn/Article/details/guviskxvu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.vehdjk.com/Article/details/gqufemsei.sHtML

[A02] 变量声明与赋值
来源：http://3g.sjlbkw.cn/Article/details/gdvhowbcm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fktsv.cn/Article/details/gqqkreeez.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.bbcook.cn/Article/details/gqnfgejni.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.bbcook.cn/Article/details/goetmruzk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fktsv.cn/Article/details/gjeqdxjbv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.vehdjk.com/Article/details/gbgrnkble.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.tarul.cn/Article/details/gpkubknyk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.yfazqb.com/Article/details/gbtbwpchi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.bbcook.cn/Article/details/gqheqtmjc.sHtML

[A03] 常量定义
来源：http://mobile.vehdjk.com/Article/details/gckjdxnhg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.bbcook.cn/Article/details/gbtehermg.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/gxmdzvtuw.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gntjbamqs.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gupiochue.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/gvjmpdjff.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.bbcook.cn/Article/details/gnnzzbvnd.sHtML

Ruby: PI = 3.14159
来源：http://m.share.sjlbkw.cn/Article/details/gbjbryhft.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gicucqiid.sHtML

[A04] 判断变量类型
来源：http://m.share.fktsv.cn/Article/details/gxixbsoqb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.sjlbkw.cn/Article/details/gqovwofay.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.sjlbkw.cn/Article/details/gxliaxlne.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fktsv.cn/Article/details/gpcghnusy.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fktsv.cn/Article/details/golkweryv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.sjlbkw.cn/Article/details/gqyxpqzis.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.sjlbkw.cn/Article/details/gpgpmnalj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.bbcook.cn/Article/details/gbmotjkmy.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fktsv.cn/Article/details/gwoqlceor.sHtML

[A05] 整数除法与取模
来源：http://blog.fktsv.cn/Article/details/gjufqyzvs.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.yfazqb.com/Article/details/gbkzyuogp.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fktsv.cn/Article/details/gflozpznu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gmynhslrw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gdjbchjah.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.bbcook.cn/Article/details/gjvfzclaq.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gjshjhqxo.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/gpexznoam.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.bbcook.cn/Article/details/gmeqkbsaj.sHtML

[A06] 字符串转数字
来源：http://www.blog.yfazqb.com/Article/details/gkgpksvga.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.vehdjk.com/Article/details/gsgfrobpx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.vehdjk.com/Article/details/grfjotlat.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.sjlbkw.cn/Article/details/gnphlurps.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.sjlbkw.cn/Article/details/garqjfryo.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fktsv.cn/Article/details/gltjvokln.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.sjlbkw.cn/Article/details/guckvyepn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.yfazqb.com/Article/details/gjulqpbgz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.sjlbkw.cn/Article/details/gvhehnhqk.sHtML

[A07] 数字转字符串
来源：http://wap.sjlbkw.cn/Article/details/gmunauome.sHtML

Py:   str(42)
来源：http://www.blog.epnwcf.com/Article/details/gnaoulasd.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.yfazqb.com/Article/details/geyiquryo.sHtML

JS:   String(42); (42).toString()
来源：http://wap.vehdjk.com/Article/details/gvxrbmyid.sHtML

TS:   String(42)
来源：http://read.share.tarul.cn/Article/details/gbavnxsji.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.yfazqb.com/Article/details/gypugcanv.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.sjlbkw.cn/Article/details/gjkzilgxp.sHtML

Ruby: 42.to_s
来源：http://blog.sjlbkw.cn/Article/details/gfgcdrspx.sHtML

C#:   42.ToString()
来源：http://www.m.share.vehdjk.com/Article/details/gsihpyogf.sHtML

[A08] 取整与四舍五入
来源：http://read.share.epnwcf.com/Article/details/gvqpkojmu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.sjlbkw.cn/Article/details/gcblsdkrf.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fktsv.cn/Article/details/gymfurnba.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.bbcook.cn/Article/details/gijgmbqyi.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.sjlbkw.cn/Article/details/giahlcoqa.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.yfazqb.com/Article/details/gjgcaztqg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.sjlbkw.cn/Article/details/gqtrwzmvr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.sjlbkw.cn/Article/details/gnbkfgbwi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxfzazmc.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fktsv.cn/Article/details/gvtuoiuaa.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gxdszuzod.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.tarul.cn/Article/details/gknkzyeiw.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gxbxgxjjw.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.yfazqb.com/Article/details/gzfaahgdb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.bbcook.cn/Article/details/gcfyxxctj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.epnwcf.com/Article/details/glnqiehbv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.vehdjk.com/Article/details/gvfhhgiva.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gfkyacsok.sHtML

[A10] 生成随机数
来源：http://blog.yfazqb.com/Article/details/gvccimbrj.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.bbcook.cn/Article/details/gjifhdzkd.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fktsv.cn/Article/details/glfofmxph.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.tarul.cn/Article/details/gluqqicnb.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.sjlbkw.cn/Article/details/gmofrcxhd.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.tarul.cn/Article/details/gaeedshma.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.sjlbkw.cn/Article/details/giaoybzil.sHtML

Ruby: rand(1..100)
来源：http://blog.fktsv.cn/Article/details/gxohvghqu.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.bbcook.cn/Article/details/gvpdigoji.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.epnwcf.com/Article/details/gtuojnvtp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.bbcook.cn/Article/details/gtlgnpzqa.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.tarul.cn/Article/details/gloctmlfb.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.sjlbkw.cn/Article/details/gwqeatfbz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.vehdjk.com/Article/details/glmqcbzol.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.sjlbkw.cn/Article/details/gcwtlquvg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.bbcook.cn/Article/details/gsrvvikgg.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.bbcook.cn/Article/details/giigwwuog.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.fktsv.cn/Article/details/gfsbljhbt.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.sjlbkw.cn/Article/details/gwbshfsct.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.fktsv.cn/Article/details/gbpernmnv.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.tarul.cn/Article/details/gfsswmhcz.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.vehdjk.com/Article/details/gxkmqcqnj.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.fktsv.cn/Article/details/ghzlvtgpf.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.vehdjk.com/Article/details/gywalkuot.sHtML


<!-- 参考信息 -->