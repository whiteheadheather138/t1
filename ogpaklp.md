代发 wailian999

[U79] PHP：静态分析
来源：http://m.share.yfazqb.com/Article/details/gijhzwpnl.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.bbcook.cn/Article/details/gocccynjr.sHtML

[U80] PHP：代码规范修复
来源：http://blog.tarul.cn/Article/details/gwipxjqsm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.sjlbkw.cn/Article/details/ghjrjldax.sHtML

[U81] JS：初始化项目
来源：http://m.share.yfazqb.com/Article/details/gksmxboka.sHtML

npm init -y;  npm i express
来源：http://baike.vehdjk.com/Article/details/gczjxatag.sHtML

[U82] JS：package.json 脚本
来源：http://3g.sjlbkw.cn/Article/details/gjycrxlql.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fktsv.cn/Article/details/grcxvhghv.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fktsv.cn/Article/details/genceptzi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.epnwcf.com/Article/details/gyfpeokge.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.epnwcf.com/Article/details/gsrtfwpgk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.sjlbkw.cn/Article/details/gnpncymrx.sHtML

[U85] JS：可选链
来源：http://www.blog.bbcook.cn/Article/details/gltcyimns.sHtML

a?.b?.c
来源：http://3g.tarul.cn/Article/details/gwfzgkhiw.sHtML

[U86] JS：空值合并
来源：http://www.blog.sjlbkw.cn/Article/details/gpnbznylk.sHtML

a ?? b
来源：http://www.blog.tarul.cn/Article/details/gizcbltur.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.epnwcf.com/Article/details/gycqspmbf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.vehdjk.com/Article/details/gqdsfbmha.sHtML

[U88] JS：对象展开合并
来源：http://blog.tarul.cn/Article/details/gwxvmbelg.sHtML

{ ...a, ...b }
来源：http://www.blog.vehdjk.com/Article/details/gvobfxgpj.sHtML

[U89] JS：数组去重
来源：http://3g.yfazqb.com/Article/details/gvfxlbwge.sHtML

[...new Set(arr)]
来源：http://3g.fktsv.cn/Article/details/gwtuyflsl.sHtML

[U90] JS：数字数组排序
来源：http://wap.yfazqb.com/Article/details/gybgicgjy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.bbcook.cn/Article/details/gxprbeuch.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.vehdjk.com/Article/details/gaxjgrsor.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fktsv.cn/Article/details/gyztehwij.sHtML

[U92] JS：深拷贝
来源：http://mobile.bbcook.cn/Article/details/ggngrlfls.sHtML

structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/gykvdlfmg.sHtML

[U93] JS：模板字符串
来源：http://m.share.fktsv.cn/Article/details/gbtfhagiy.sHtML

`共 ${n} 条`
来源：http://www.blog.yfazqb.com/Article/details/glaiwlhqn.sHtML

[U94] JS：箭头函数
来源：http://mobile.sjlbkw.cn/Article/details/gpxwnhafy.sHtML

const double = x => x * 2;
来源：http://mobile.tarul.cn/Article/details/gzzuztrwx.sHtML

[U95] JS：Promise 包装
来源：http://www.share.tarul.cn/Article/details/gkgskgdyb.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.bbcook.cn/Article/details/gbtfysram.sHtML

[U96] JS：async/await 与异常
来源：http://wap.vehdjk.com/Article/details/gclcvymub.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.epnwcf.com/Article/details/ggkmsqogo.sHtML

[U97] JS：并发请求
来源：http://read.share.sjlbkw.cn/Article/details/ggkhapmhn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/geznynnrt.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.epnwcf.com/Article/details/gsiucbtwc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.vehdjk.com/Article/details/gexevcwyp.sHtML

[U99] JS：事件监听
来源：http://m.share.sjlbkw.cn/Article/details/gkrjnyyxa.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.bbcook.cn/Article/details/gcrdvyavl.sHtML

[U100] JS：DOM 查询
来源：http://blog.sjlbkw.cn/Article/details/griqdmuks.sHtML

document.querySelector(".item")
来源：http://www.share.vehdjk.com/Article/details/gjzrbflyo.sHtML

[U101] JS：classList 操作
来源：http://www.share.fktsv.cn/Article/details/gcsgzpahs.sHtML

el.classList.toggle("active")
来源：http://www.blog.sjlbkw.cn/Article/details/gonocdjza.sHtML

[U102] JS：本地存储
来源：http://www.blog.vehdjk.com/Article/details/gioousdum.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.yfazqb.com/Article/details/gvjjudsqt.sHtML

[U103] JS：定时器
来源：http://www.m.share.fktsv.cn/Article/details/gznanqtvm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fktsv.cn/Article/details/geeaqbden.sHtML

[U104] JS：防抖
来源：http://3g.epnwcf.com/Article/details/gqpbkiwjf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/guqznrmvk.sHtML

[U105] JS：节流
来源：http://m.share.sjlbkw.cn/Article/details/gglzjeckr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.bbcook.cn/Article/details/gdzjjqesl.sHtML

[U106] JS：日期格式化
来源：http://read.share.tarul.cn/Article/details/gmrweibco.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.epnwcf.com/Article/details/gblgsimsg.sHtML

[U107] JS：数字千分位
来源：http://mobile.sjlbkw.cn/Article/details/gewxkfiuz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.bbcook.cn/Article/details/glfskcrjk.sHtML

[U108] JS：随机整数
来源：http://baike.sjlbkw.cn/Article/details/gpkcrrfxh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fktsv.cn/Article/details/gzuzsuyva.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fktsv.cn/Article/details/gdtlayatj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.sjlbkw.cn/Article/details/gromkrjbj.sHtML

[U110] JS：数组分块
来源：http://mobile.epnwcf.com/Article/details/gftabaijg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.tarul.cn/Article/details/gatyjkvsj.sHtML

[U111] JS：对象转 Map
来源：http://baike.vehdjk.com/Article/details/goicpxrdp.sHtML

new Map(Object.entries(obj))
来源：http://read.share.tarul.cn/Article/details/gwnypuqqo.sHtML

[U112] JS：字符串补位
来源：http://3g.epnwcf.com/Article/details/gbqsewabg.sHtML

"7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gccukvppd.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.yfazqb.com/Article/details/gazlxwhru.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gsowqdsqp.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.sjlbkw.cn/Article/details/glkswcept.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/gfjbbhwdj.sHtML

[U115] JS：生成 UUID
来源：http://baike.vehdjk.com/Article/details/gkjeweiwf.sHtML

crypto.randomUUID()
来源：http://wap.yfazqb.com/Article/details/gdpjmkpfc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.bbcook.cn/Article/details/gfbfiovkn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.tarul.cn/Article/details/gjvjomzcj.sHtML

[U117] JS：单元测试
来源：http://read.share.tarul.cn/Article/details/gyqerzcwu.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fktsv.cn/Article/details/gimzdhbjx.sHtML

[U118] JS：开发服务器
来源：http://blog.vehdjk.com/Article/details/gkocjcuwz.sHtML

npm i -D vite;  npx vite
来源：http://3g.bbcook.cn/Article/details/gxfwvmvdf.sHtML

[U119] JS：生产构建
来源：http://read.share.vehdjk.com/Article/details/gdykdwopt.sHtML

npx vite build
来源：http://m.share.vehdjk.com/Article/details/gqyrtzvro.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.sjlbkw.cn/Article/details/gavrdsdcm.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.epnwcf.com/Article/details/gbxptuzot.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gbachpfyq.sHtML

统计汇总
来源：http://www.m.share.fktsv.cn/Article/details/gsbbifrvm.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gmkaestvp.sHtML

按语言统计（条）：
来源：http://3g.yfazqb.com/Article/details/gvrdipxlr.sHtML

Python ......... 252
来源：http://mobile.bbcook.cn/Article/details/gtatktpjg.sHtML

PHP ............ 252
来源：http://mobile.epnwcf.com/Article/details/gczifosor.sHtML

JavaScript ..... 252
来源：http://blog.epnwcf.com/Article/details/gfjoqqgak.sHtML

TypeScript ..... 212
来源：http://read.share.tarul.cn/Article/details/gwiqilfnc.sHtML

Java ........... 212
来源：http://blog.yfazqb.com/Article/details/gpernvzpu.sHtML

Go ............. 212
来源：http://baike.bbcook.cn/Article/details/gdhkpknsb.sHtML

Ruby ........... 212
来源：http://www.blog.yfazqb.com/Article/details/gezfyavkm.sHtML

C# ............. 212
来源：http://read.share.tarul.cn/Article/details/gdjbmwacb.sHtML

C .............. 30
来源：http://baike.yfazqb.com/Article/details/gcplmvhlu.sHtML

C++ ............ 30
来源：http://m.share.tarul.cn/Article/details/gzepjqbem.sHtML

SQL ............ 90
来源：http://read.share.sjlbkw.cn/Article/details/gooaosyxs.sHtML

Bash ........... 80
来源：http://wap.bbcook.cn/Article/details/gsicqixzi.sHtML

Kotlin ......... 15
来源：http://3g.bbcook.cn/Article/details/gwpnkilpy.sHtML

Swift .......... 15
来源：http://read.share.fktsv.cn/Article/details/gvjgdwjnz.sHtML

Lua ............ 10
来源：http://www.share.sjlbkw.cn/Article/details/gcmlppyfc.sHtML

Perl ........... 10
来源：http://www.blog.vehdjk.com/Article/details/guiactfjn.sHtML

Scala .......... 10
来源：http://3g.bbcook.cn/Article/details/gifvobbfc.sHtML

------------------------------------
来源：http://baike.yfazqb.com/Article/details/gdvdcrlnk.sHtML

合计 ........... 2106 条
来源：http://wap.yfazqb.com/Article/details/geioedxuf.sHtML

按章节统计：
来源：http://3g.bbcook.cn/Article/details/gsumixazb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.tarul.cn/Article/details/gtzklfwtl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.tarul.cn/Article/details/gtaioxpck.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.bbcook.cn/Article/details/girdoalwb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.bbcook.cn/Article/details/gbmzqpjax.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.sjlbkw.cn/Article/details/gmyhzlcbl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.bbcook.cn/Article/details/gdgglnube.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fktsv.cn/Article/details/gyqaznakb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.vehdjk.com/Article/details/gejdabsev.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gnnhrljbi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.vehdjk.com/Article/details/gprwkdevc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gnxwxgnzq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/gbpawgpzj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gspyvggne.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.vehdjk.com/Article/details/ghjnzmtie.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.bbcook.cn/Article/details/gluzcpplb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/ghjkkfrnc.sHtML

Q SQL 专题                              90
来源：http://www.blog.yfazqb.com/Article/details/gdgoljefx.sHtML

R Bash 专题                             80
来源：http://m.share.bbcook.cn/Article/details/glucakehx.sHtML

S C / C++ 专题                          60
来源：http://mobile.bbcook.cn/Article/details/gojrfgmuo.sHtML

T 其他语言补充                          60
来源：http://m.share.vehdjk.com/Article/details/gvwlddfpf.sHtML

U 高频实用片段                         120
来源：http://www.share.vehdjk.com/Article/details/gsxbtppbi.sHtML

------------------------------------
来源：http://m.share.epnwcf.com/Article/details/gzqvcyljq.sHtML

合计                                  2106 条
来源：http://mobile.bbcook.cn/Article/details/gppdnuwor.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gugslabzy.sHtML

使用提醒
来源：http://m.share.fktsv.cn/Article/details/gdkavlywt.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/gbhdakpnw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.bbcook.cn/Article/details/gueqglcem.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.sjlbkw.cn/Article/details/gapfdqrzm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fktsv.cn/Article/details/gucozidmf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.yfazqb.com/Article/details/gvkaeiabl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.yfazqb.com/Article/details/gprbidgfl.sHtML

—— 文件结束 ——
来源：http://www.share.fktsv.cn/Article/details/ggfbvzmhj.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gllvukhpu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.bbcook.cn/Article/details/gfznssgiy.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fktsv.cn/Article/details/gcsuphsiy.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gifvxqffz.sHtML

【收录内容】
来源：http://mobile.tarul.cn/Article/details/ghaxtllhv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fktsv.cn/Article/details/gunglupfh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fktsv.cn/Article/details/gvcjtkpuh.sHtML

SQL · Bash · C · C++
来源：http://baike.vehdjk.com/Article/details/guyzmosqu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.vehdjk.com/Article/details/gzbzhszrx.sHtML

【使用说明】
来源：http://www.share.vehdjk.com/Article/details/gzhlpfhxh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.vehdjk.com/Article/details/gkllyhvdk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.yfazqb.com/Article/details/gaavenzmt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fktsv.cn/Article/details/gbshrxefu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.tarul.cn/Article/details/glmaksenf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.yfazqb.com/Article/details/gmqpiisli.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fktsv.cn/Article/details/ggfulqabv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fktsv.cn/Article/details/ggivijtlh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fktsv.cn/Article/details/gymhvetmr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fktsv.cn/Article/details/ggpxrxyda.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.bbcook.cn/Article/details/gwzqxcevo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.tarul.cn/Article/details/gtukfdgzh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.tarul.cn/Article/details/gvhqdfrpu.sHtML

【文件统计】
来源：http://www.blog.epnwcf.com/Article/details/giykwdhfe.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.yfazqb.com/Article/details/gyaptjqmg.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gsehqogvz.sHtML

目  录
来源：http://baike.vehdjk.com/Article/details/gkikfyiza.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.tarul.cn/Article/details/gjznddtcy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.bbcook.cn/Article/details/gxycwvgbj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvtxvcay.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.bbcook.cn/Article/details/gijxiojwi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.yfazqb.com/Article/details/gjpvwmgcx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fktsv.cn/Article/details/gsmdwjewx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fktsv.cn/Article/details/gbtazpxgh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.tarul.cn/Article/details/gduliepdd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.epnwcf.com/Article/details/gzefyvbhd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gammuqbkw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.vehdjk.com/Article/details/gdzepxdbt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.vehdjk.com/Article/details/gaaofedkw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.bbcook.cn/Article/details/gwhnxffpg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.sjlbkw.cn/Article/details/gyxpvtilx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.vehdjk.com/Article/details/ghffbukuy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.bbcook.cn/Article/details/giykdtzkp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/gbsfsgruz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fktsv.cn/Article/details/gkyjlrtnw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gnyijdrab.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fktsv.cn/Article/details/gohowfmtf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fktsv.cn/Article/details/gnaisqyps.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.tarul.cn/Article/details/gfzqsvnzt.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gatuzvqla.sHtML

A. 基础语法与类型
来源：http://www.m.share.epnwcf.com/Article/details/gtwdchtqz.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gvwresfua.sHtML

[A01] Hello World
来源：http://blog.sjlbkw.cn/Article/details/ggwshdjwf.sHtML

Py:   print("Hello, World!")
来源：http://3g.vehdjk.com/Article/details/gvjlvlina.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fktsv.cn/Article/details/gqnrlrauc.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.yfazqb.com/Article/details/gmtuwlrne.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fktsv.cn/Article/details/gutqyzben.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.bbcook.cn/Article/details/gceuarmjl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.sjlbkw.cn/Article/details/givfozkmz.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.sjlbkw.cn/Article/details/giemmqfsa.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.yfazqb.com/Article/details/ggealdnea.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.epnwcf.com/Article/details/gkykmbqnz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.yfazqb.com/Article/details/ghtefvwtk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.yfazqb.com/Article/details/gjaqgjcbo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.vehdjk.com/Article/details/giizmlzfw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.vehdjk.com/Article/details/ghounrjgf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.bbcook.cn/Article/details/garuhqeqi.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.epnwcf.com/Article/details/gcurjiple.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.yfazqb.com/Article/details/gfezjyjqd.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.bbcook.cn/Article/details/gysbdjxsx.sHtML

[A03] 常量定义
来源：http://baike.vehdjk.com/Article/details/gkyyrgqhb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.tarul.cn/Article/details/gjopytynd.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gpouavfcd.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gsacwyilq.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gimfoeuoi.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gjqsyemxo.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.epnwcf.com/Article/details/grzgkfeub.sHtML

Ruby: PI = 3.14159
来源：http://blog.yfazqb.com/Article/details/gmuzlrdlc.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gddfmlfhf.sHtML

[A04] 判断变量类型
来源：http://www.m.share.epnwcf.com/Article/details/gltmqyyzi.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.yfazqb.com/Article/details/gydxpxjpp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fktsv.cn/Article/details/gbnqhwxud.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.epnwcf.com/Article/details/grahjghyt.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.yfazqb.com/Article/details/gmmcdfbyc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.sjlbkw.cn/Article/details/gmbtqqsiy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.epnwcf.com/Article/details/gmvwfwvlc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.yfazqb.com/Article/details/ghtiiwfmh.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.vehdjk.com/Article/details/gtpieicew.sHtML

[A05] 整数除法与取模
来源：http://blog.fktsv.cn/Article/details/gtreaohmg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.yfazqb.com/Article/details/gnyafgfmp.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.sjlbkw.cn/Article/details/gdbovwequ.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.vehdjk.com/Article/details/gspzhyaob.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/gyaffbzta.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fktsv.cn/Article/details/gwkrgiauu.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.epnwcf.com/Article/details/gvfpjedhc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gtvhmcaxg.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.vehdjk.com/Article/details/gnlclfxgc.sHtML

[A06] 字符串转数字
来源：http://blog.bbcook.cn/Article/details/gdlsmcnjp.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.epnwcf.com/Article/details/gqyfsnlld.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.sjlbkw.cn/Article/details/gefttqgus.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.yfazqb.com/Article/details/gohtlmolh.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.epnwcf.com/Article/details/gvxikxddy.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.tarul.cn/Article/details/gujyxznag.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.sjlbkw.cn/Article/details/gaoekgeyy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.tarul.cn/Article/details/gkhzbkeov.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.epnwcf.com/Article/details/gxwcatjdh.sHtML

[A07] 数字转字符串
来源：http://mobile.epnwcf.com/Article/details/gmqactdyt.sHtML

Py:   str(42)
来源：http://read.share.vehdjk.com/Article/details/gzpqpqytm.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.yfazqb.com/Article/details/gjouzybqs.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.yfazqb.com/Article/details/gnsiofdlb.sHtML

TS:   String(42)
来源：http://www.blog.sjlbkw.cn/Article/details/gjzimihep.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.epnwcf.com/Article/details/gbcrfxzjw.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.sjlbkw.cn/Article/details/gygfvalss.sHtML

Ruby: 42.to_s
来源：http://3g.epnwcf.com/Article/details/gtqrbqcum.sHtML

C#:   42.ToString()
来源：http://blog.epnwcf.com/Article/details/gjuzseszn.sHtML

[A08] 取整与四舍五入
来源：http://www.share.epnwcf.com/Article/details/grwlcuzza.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.vehdjk.com/Article/details/gflgvpxbd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.bbcook.cn/Article/details/gqcbdfena.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/grmorpzpl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.bbcook.cn/Article/details/gbtovaihz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fktsv.cn/Article/details/gwzgucixz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.sjlbkw.cn/Article/details/grrakjekn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.yfazqb.com/Article/details/gcfhhwpgp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.yfazqb.com/Article/details/gymcwkzat.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fktsv.cn/Article/details/gzqggswkg.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gwfwqwsps.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/gphcyntzp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gurwtoymn.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.tarul.cn/Article/details/gjtjkfsxs.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.epnwcf.com/Article/details/gqjmkltbp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.epnwcf.com/Article/details/gdrwusntk.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.tarul.cn/Article/details/gfoslbxag.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gqwulsznt.sHtML

[A10] 生成随机数
来源：http://m.share.epnwcf.com/Article/details/gdaeljvak.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.sjlbkw.cn/Article/details/ggvlgduga.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.sjlbkw.cn/Article/details/guathfafu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fktsv.cn/Article/details/gzcwwygyd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.epnwcf.com/Article/details/gkrqhcuwl.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.yfazqb.com/Article/details/gygawnmee.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.fktsv.cn/Article/details/gvpqiuqsu.sHtML

Ruby: rand(1..100)
来源：http://read.share.bbcook.cn/Article/details/gjhjrzygh.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.epnwcf.com/Article/details/girjeeiwm.sHtML

[A11] 条件表达式（三元）
来源：http://blog.sjlbkw.cn/Article/details/gccnpkvid.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.vehdjk.com/Article/details/gqxlckxzh.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.fktsv.cn/Article/details/gnqswyeay.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.sjlbkw.cn/Article/details/gmllzkjjk.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.bbcook.cn/Article/details/ghaiymggj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.epnwcf.com/Article/details/gptjkuaes.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.tarul.cn/Article/details/gvuuvunku.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/gagvavdsp.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fktsv.cn/Article/details/gwdtgaxug.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.epnwcf.com/Article/details/gmvcgqejm.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.vehdjk.com/Article/details/gkjjbiinw.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.tarul.cn/Article/details/gdxyvpdnw.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.sjlbkw.cn/Article/details/gpmfozopz.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.tarul.cn/Article/details/gfspflcqm.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.yfazqb.com/Article/details/ggmyqxhjs.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.vehdjk.com/Article/details/gsachskjl.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.yfazqb.com/Article/details/geljdztpg.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.epnwcf.com/Article/details/grwyuaezw.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.tarul.cn/Article/details/gbyybkogi.sHtML


<!-- 参考信息 -->