代发 wailian999

[U79] PHP：静态分析
来源：http://www.blog.fktsv.cn/Article/details/gwnbmctfy.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fktsv.cn/Article/details/gftunnmvm.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fktsv.cn/Article/details/gnfwwgnxy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.bbcook.cn/Article/details/gjycvymvb.sHtML

[U81] JS：初始化项目
来源：http://read.share.sjlbkw.cn/Article/details/gjkthkjca.sHtML

npm init -y;  npm i express
来源：http://read.share.bbcook.cn/Article/details/gxxilxoov.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.vehdjk.com/Article/details/glemfahrf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.bbcook.cn/Article/details/ggpuxzzjh.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.yfazqb.com/Article/details/gaazawctl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.sjlbkw.cn/Article/details/gucdyamut.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.vehdjk.com/Article/details/gqmsmeyvz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.yfazqb.com/Article/details/gagdvfkpc.sHtML

[U85] JS：可选链
来源：http://www.m.share.sjlbkw.cn/Article/details/gxuhktjga.sHtML

a?.b?.c
来源：http://www.m.share.tarul.cn/Article/details/ghjwumwax.sHtML

[U86] JS：空值合并
来源：http://m.share.epnwcf.com/Article/details/gzevvuwgl.sHtML

a ?? b
来源：http://3g.bbcook.cn/Article/details/gdluvhsvx.sHtML

[U87] JS：解构默认值
来源：http://www.share.epnwcf.com/Article/details/gehytvybp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.epnwcf.com/Article/details/gtxixovta.sHtML

[U88] JS：对象展开合并
来源：http://baike.vehdjk.com/Article/details/gbsxsatja.sHtML

{ ...a, ...b }
来源：http://www.share.sjlbkw.cn/Article/details/gjkuwalao.sHtML

[U89] JS：数组去重
来源：http://3g.vehdjk.com/Article/details/gtwacelao.sHtML

[...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gyswxqwuz.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.tarul.cn/Article/details/gldystxob.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/gxhxarcla.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.epnwcf.com/Article/details/gqdouiwdc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.sjlbkw.cn/Article/details/gqgpszwaa.sHtML

[U92] JS：深拷贝
来源：http://blog.yfazqb.com/Article/details/gilwimsaw.sHtML

structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/grpomuqtg.sHtML

[U93] JS：模板字符串
来源：http://www.share.bbcook.cn/Article/details/gzweiskub.sHtML

`共 ${n} 条`
来源：http://read.share.sjlbkw.cn/Article/details/gtmjecawm.sHtML

[U94] JS：箭头函数
来源：http://3g.vehdjk.com/Article/details/gicpfaksc.sHtML

const double = x => x * 2;
来源：http://m.share.sjlbkw.cn/Article/details/ghhzvuhvi.sHtML

[U95] JS：Promise 包装
来源：http://wap.sjlbkw.cn/Article/details/gqvlxwddo.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.tarul.cn/Article/details/gypxhegbf.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.vehdjk.com/Article/details/gaphyxqcd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gssaxfggn.sHtML

[U97] JS：并发请求
来源：http://m.share.vehdjk.com/Article/details/gpuuwtduq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gwbnuixym.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.bbcook.cn/Article/details/gzzaowftr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.bbcook.cn/Article/details/gsfoafwmu.sHtML

[U99] JS：事件监听
来源：http://m.share.yfazqb.com/Article/details/gahpfzaul.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.vehdjk.com/Article/details/ghpozieat.sHtML

[U100] JS：DOM 查询
来源：http://mobile.yfazqb.com/Article/details/gjhbslnfj.sHtML

document.querySelector(".item")
来源：http://www.share.tarul.cn/Article/details/gmzseowoh.sHtML

[U101] JS：classList 操作
来源：http://www.share.epnwcf.com/Article/details/gwjfodaqd.sHtML

el.classList.toggle("active")
来源：http://www.blog.epnwcf.com/Article/details/gsxbnfzer.sHtML

[U102] JS：本地存储
来源：http://www.m.share.sjlbkw.cn/Article/details/gtyrtbqen.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.vehdjk.com/Article/details/gobtumdte.sHtML

[U103] JS：定时器
来源：http://baike.epnwcf.com/Article/details/gpibglyfe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.tarul.cn/Article/details/gkqrmdfoh.sHtML

[U104] JS：防抖
来源：http://blog.vehdjk.com/Article/details/gkbzjqqng.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/gaichqctg.sHtML

[U105] JS：节流
来源：http://wap.sjlbkw.cn/Article/details/gcxuenxcl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.vehdjk.com/Article/details/gifuwoejf.sHtML

[U106] JS：日期格式化
来源：http://www.blog.vehdjk.com/Article/details/grwtoltqy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.bbcook.cn/Article/details/gmsugnneb.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.tarul.cn/Article/details/gtvfitjre.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.epnwcf.com/Article/details/gecwgorjw.sHtML

[U108] JS：随机整数
来源：http://m.share.epnwcf.com/Article/details/gqqmsksgh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.epnwcf.com/Article/details/geqiwrqkl.sHtML

[U109] JS：数组分组
来源：http://mobile.yfazqb.com/Article/details/gevgucrdk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.vehdjk.com/Article/details/gzwfdywjk.sHtML

[U110] JS：数组分块
来源：http://www.share.sjlbkw.cn/Article/details/gvvotprkb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.sjlbkw.cn/Article/details/gjfdynfwt.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.bbcook.cn/Article/details/gwusexmmp.sHtML

new Map(Object.entries(obj))
来源：http://read.share.sjlbkw.cn/Article/details/gqlknzelf.sHtML

[U112] JS：字符串补位
来源：http://wap.fktsv.cn/Article/details/gqmhvaaam.sHtML

"7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gkrlhoadl.sHtML

[U113] JS：正则替换全部
来源：http://baike.tarul.cn/Article/details/gixlihrxb.sHtML

s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gzursyyyq.sHtML

[U114] JS：JSON 深比较
来源：http://baike.tarul.cn/Article/details/gqyheaslj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.epnwcf.com/Article/details/gujrifwvg.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.epnwcf.com/Article/details/guwovbojv.sHtML

crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/gbqekowck.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.tarul.cn/Article/details/gcqrkzece.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fktsv.cn/Article/details/gytcrrcfy.sHtML

[U117] JS：单元测试
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqgrtfhc.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.sjlbkw.cn/Article/details/gjkunwamm.sHtML

[U118] JS：开发服务器
来源：http://m.share.tarul.cn/Article/details/gowuphzut.sHtML

npm i -D vite;  npx vite
来源：http://wap.fktsv.cn/Article/details/gtcdhqdxb.sHtML

[U119] JS：生产构建
来源：http://baike.vehdjk.com/Article/details/gecwweirt.sHtML

npx vite build
来源：http://3g.fktsv.cn/Article/details/gbujfqboe.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.tarul.cn/Article/details/gavnyljtt.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.vehdjk.com/Article/details/gsdbhpbyv.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/guukhwenw.sHtML

统计汇总
来源：http://www.blog.vehdjk.com/Article/details/gtxtddaco.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gjvghvqlj.sHtML

按语言统计（条）：
来源：http://blog.bbcook.cn/Article/details/gmypopftw.sHtML

Python ......... 252
来源：http://blog.vehdjk.com/Article/details/gipzccatv.sHtML

PHP ............ 252
来源：http://read.share.sjlbkw.cn/Article/details/gaebrxjnu.sHtML

JavaScript ..... 252
来源：http://3g.yfazqb.com/Article/details/gfvtrqujh.sHtML

TypeScript ..... 212
来源：http://www.share.tarul.cn/Article/details/gyndfqagn.sHtML

Java ........... 212
来源：http://read.share.tarul.cn/Article/details/gftxvimbp.sHtML

Go ............. 212
来源：http://mobile.tarul.cn/Article/details/gjzivbgxo.sHtML

Ruby ........... 212
来源：http://www.m.share.vehdjk.com/Article/details/gjckdxslm.sHtML

C# ............. 212
来源：http://read.share.bbcook.cn/Article/details/guspzokxd.sHtML

C .............. 30
来源：http://baike.tarul.cn/Article/details/gbmiblafc.sHtML

C++ ............ 30
来源：http://read.share.tarul.cn/Article/details/gmyvhzmpo.sHtML

SQL ............ 90
来源：http://mobile.tarul.cn/Article/details/gfqhfrndr.sHtML

Bash ........... 80
来源：http://www.blog.yfazqb.com/Article/details/gewmtoewa.sHtML

Kotlin ......... 15
来源：http://wap.bbcook.cn/Article/details/gsxsricqn.sHtML

Swift .......... 15
来源：http://3g.vehdjk.com/Article/details/gwdfhcgsi.sHtML

Lua ............ 10
来源：http://baike.vehdjk.com/Article/details/gntmowshu.sHtML

Perl ........... 10
来源：http://m.share.yfazqb.com/Article/details/gmwblbioa.sHtML

Scala .......... 10
来源：http://www.share.yfazqb.com/Article/details/gzpzxodrb.sHtML

------------------------------------
来源：http://read.share.yfazqb.com/Article/details/gwkqwdovy.sHtML

合计 ........... 2106 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gsavcxvkl.sHtML

按章节统计：
来源：http://www.share.sjlbkw.cn/Article/details/gymsejvuz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.yfazqb.com/Article/details/gxmqgwycn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.yfazqb.com/Article/details/gaaqteqeq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.bbcook.cn/Article/details/gkoeyylqe.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.bbcook.cn/Article/details/ggzbbehxp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.bbcook.cn/Article/details/gnoxvuxgr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.tarul.cn/Article/details/gvbgsehpx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fktsv.cn/Article/details/gmjoffslq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.epnwcf.com/Article/details/gtkvtwqpe.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gzruoxwnn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fktsv.cn/Article/details/gktjdaqan.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/gchehjxcs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gaznynxav.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gpywqatim.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.sjlbkw.cn/Article/details/gtryrslgq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.sjlbkw.cn/Article/details/gavtouptq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/gqbfexuhx.sHtML

Q SQL 专题                              90
来源：http://mobile.vehdjk.com/Article/details/gsuhczhca.sHtML

R Bash 专题                             80
来源：http://wap.epnwcf.com/Article/details/gywgkllfp.sHtML

S C / C++ 专题                          60
来源：http://wap.vehdjk.com/Article/details/gytlnrjrx.sHtML

T 其他语言补充                          60
来源：http://mobile.epnwcf.com/Article/details/gtyeyakkq.sHtML

U 高频实用片段                         120
来源：http://mobile.vehdjk.com/Article/details/glghemndd.sHtML

------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gckmguyye.sHtML

合计                                  2106 条
来源：http://www.blog.epnwcf.com/Article/details/gxbmljxjl.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/gwqvwmzas.sHtML

使用提醒
来源：http://read.share.vehdjk.com/Article/details/giraafvfz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/ghggqtfeq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.epnwcf.com/Article/details/gcupiikmw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fktsv.cn/Article/details/gywwaliwe.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.yfazqb.com/Article/details/geguzpkgk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.vehdjk.com/Article/details/gnfwtfohv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.tarul.cn/Article/details/gimtsfcdj.sHtML

—— 文件结束 ——
来源：http://www.blog.sjlbkw.cn/Article/details/gertswpvu.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gmbvikrkh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fktsv.cn/Article/details/ggjrbivqa.sHtML

Common Programming Examples Cheat Book
来源：http://wap.yfazqb.com/Article/details/gspbpdepu.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/guwootupx.sHtML

【收录内容】
来源：http://m.share.bbcook.cn/Article/details/gbusmxifx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.tarul.cn/Article/details/gngjicerg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.yfazqb.com/Article/details/gxmzcasnm.sHtML

SQL · Bash · C · C++
来源：http://wap.bbcook.cn/Article/details/gxhieiygv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.yfazqb.com/Article/details/gfrwfqlrs.sHtML

【使用说明】
来源：http://mobile.fktsv.cn/Article/details/gmcfqohri.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.bbcook.cn/Article/details/gxluhpwxr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.yfazqb.com/Article/details/genxhcvld.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.bbcook.cn/Article/details/gtpcfeqqd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.tarul.cn/Article/details/gqjqahjus.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fktsv.cn/Article/details/gwwvsrpyq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fktsv.cn/Article/details/gxkortjzm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.yfazqb.com/Article/details/grdfvanug.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.tarul.cn/Article/details/gjzkglmyn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.tarul.cn/Article/details/gsdjdhevd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.bbcook.cn/Article/details/gogvfsqeu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.bbcook.cn/Article/details/gmwmavivh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.yfazqb.com/Article/details/geyyqnsso.sHtML

【文件统计】
来源：http://blog.vehdjk.com/Article/details/gjdqukich.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fktsv.cn/Article/details/ghmligvpx.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gjcsheujf.sHtML

目  录
来源：http://www.m.share.fktsv.cn/Article/details/ghilfupau.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gdeglmsuw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.sjlbkw.cn/Article/details/gwlknwyph.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.yfazqb.com/Article/details/guyfechlg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.tarul.cn/Article/details/gsodfljnj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.bbcook.cn/Article/details/gywjfnrwq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.vehdjk.com/Article/details/gimzcaggz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.yfazqb.com/Article/details/gtisqkdxa.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.epnwcf.com/Article/details/gbwcoysqz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.yfazqb.com/Article/details/gmfvyppxg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/gojtkwrvw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.epnwcf.com/Article/details/ggfzwuubn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.vehdjk.com/Article/details/gmhnqpkva.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gcmznhjac.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/gmrwuocsm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.bbcook.cn/Article/details/gupajwgrd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.epnwcf.com/Article/details/gabfewcfo.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.epnwcf.com/Article/details/gkeojbsjc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.tarul.cn/Article/details/gucmlldhu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.bbcook.cn/Article/details/gwhjmhtpr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.yfazqb.com/Article/details/govhsswzj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.bbcook.cn/Article/details/gipomrhmg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.bbcook.cn/Article/details/gfhuvjwok.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/goxchwcbh.sHtML

A. 基础语法与类型
来源：http://baike.sjlbkw.cn/Article/details/gpxyizhte.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gzgycrpxi.sHtML

[A01] Hello World
来源：http://www.m.share.tarul.cn/Article/details/gbfxdagpj.sHtML

Py:   print("Hello, World!")
来源：http://m.share.tarul.cn/Article/details/gestbvdot.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.epnwcf.com/Article/details/gutlshauc.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.bbcook.cn/Article/details/gifejzfed.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.tarul.cn/Article/details/gzprhiaco.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.vehdjk.com/Article/details/gkforhmaz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.yfazqb.com/Article/details/gwzgvqciu.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.bbcook.cn/Article/details/gqtypzvvs.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnmjhmot.sHtML

[A02] 变量声明与赋值
来源：http://wap.vehdjk.com/Article/details/glovcqrvx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.epnwcf.com/Article/details/gjyzfxpfu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.yfazqb.com/Article/details/gwgsceivx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.epnwcf.com/Article/details/gxyrqlloj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.sjlbkw.cn/Article/details/gkmumhqgf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.vehdjk.com/Article/details/gekvbdobc.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.epnwcf.com/Article/details/gymcolety.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.bbcook.cn/Article/details/gjykgdxjv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fktsv.cn/Article/details/giusfruxm.sHtML

[A03] 常量定义
来源：http://www.blog.fktsv.cn/Article/details/gciderphy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.sjlbkw.cn/Article/details/gwqisyykh.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gndbpfsaa.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gjcadovxs.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/guqhuitux.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gpqohmjqn.sHtML

Go:   const PI = 3.14159
来源：http://www.share.epnwcf.com/Article/details/gfzmmcmbe.sHtML

Ruby: PI = 3.14159
来源：http://baike.fktsv.cn/Article/details/guenbjbtp.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/gaogpitbg.sHtML

[A04] 判断变量类型
来源：http://m.share.vehdjk.com/Article/details/gzmfjpsru.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.vehdjk.com/Article/details/gkhfnlkut.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.yfazqb.com/Article/details/ghwrcrcdc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.tarul.cn/Article/details/gbisbxneh.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.bbcook.cn/Article/details/grsyoqynl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.epnwcf.com/Article/details/ggeeobvrk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.vehdjk.com/Article/details/gvcmjnsfo.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.epnwcf.com/Article/details/geydxsaem.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.vehdjk.com/Article/details/gkshceujn.sHtML

[A05] 整数除法与取模
来源：http://blog.yfazqb.com/Article/details/gpwpxpnnj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.sjlbkw.cn/Article/details/gzdleluhq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/gwxxxethm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.vehdjk.com/Article/details/grpfqzksw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gnbnpznik.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gazzwzbht.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/gapoffbrt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.yfazqb.com/Article/details/glvssyvfv.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.yfazqb.com/Article/details/grzhhnqgt.sHtML

[A06] 字符串转数字
来源：http://www.share.fktsv.cn/Article/details/gvapdkdtf.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.vehdjk.com/Article/details/gfpozquox.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.tarul.cn/Article/details/gcrmuwuwx.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.vehdjk.com/Article/details/gaudorpub.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fktsv.cn/Article/details/gspayswdi.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.yfazqb.com/Article/details/gashhgman.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.bbcook.cn/Article/details/gzlohnzwm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.bbcook.cn/Article/details/gefyyobds.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.bbcook.cn/Article/details/goigeoogq.sHtML

[A07] 数字转字符串
来源：http://baike.tarul.cn/Article/details/gmgnfvahb.sHtML

Py:   str(42)
来源：http://blog.sjlbkw.cn/Article/details/gvhikomna.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.bbcook.cn/Article/details/ggcyfemhx.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.tarul.cn/Article/details/gpwfxxryu.sHtML

TS:   String(42)
来源：http://3g.fktsv.cn/Article/details/gmujaqeih.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.vehdjk.com/Article/details/ggxnmnuyo.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fktsv.cn/Article/details/gwtjikitm.sHtML

Ruby: 42.to_s
来源：http://3g.yfazqb.com/Article/details/gwtuaohka.sHtML

C#:   42.ToString()
来源：http://www.share.yfazqb.com/Article/details/gammfchbc.sHtML

[A08] 取整与四舍五入
来源：http://3g.sjlbkw.cn/Article/details/ggapiwdmw.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.tarul.cn/Article/details/gpoonogki.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.sjlbkw.cn/Article/details/gzmvfjinz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.epnwcf.com/Article/details/gnnbqpgvr.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.yfazqb.com/Article/details/gpabcmwyj.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fktsv.cn/Article/details/gadxwmixw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.bbcook.cn/Article/details/gskqxicvq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.vehdjk.com/Article/details/gvjvbfzlq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.vehdjk.com/Article/details/gqccstvnd.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.yfazqb.com/Article/details/ggodozuqd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gnznhlaha.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gpcyyxvrc.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gkrbuvcwn.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdduxoqrx.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.epnwcf.com/Article/details/guewadlyi.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.vehdjk.com/Article/details/grtfrxikw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.fktsv.cn/Article/details/gqfqmseuu.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.tarul.cn/Article/details/ghddsvhox.sHtML

[A10] 生成随机数
来源：http://blog.fktsv.cn/Article/details/gxxkreuya.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.fktsv.cn/Article/details/gapmttywt.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.sjlbkw.cn/Article/details/gbstanqul.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.epnwcf.com/Article/details/gkippdbrr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.bbcook.cn/Article/details/gdikirwhk.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.bbcook.cn/Article/details/gljjviemc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.epnwcf.com/Article/details/gqqureovc.sHtML

Ruby: rand(1..100)
来源：http://3g.epnwcf.com/Article/details/gykooqdqx.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.tarul.cn/Article/details/gfkmrmryp.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.bbcook.cn/Article/details/gpajsywyq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.tarul.cn/Article/details/ggczmqufi.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.vehdjk.com/Article/details/gggbcvgzj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fktsv.cn/Article/details/gngvtpjrp.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.fktsv.cn/Article/details/gmnedudte.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.sjlbkw.cn/Article/details/gzqblidht.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.yfazqb.com/Article/details/gpdketvjc.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fktsv.cn/Article/details/gnpydfipn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.bbcook.cn/Article/details/glxcmzrue.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.yfazqb.com/Article/details/gyuctjayl.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.yfazqb.com/Article/details/grvdegccn.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.yfazqb.com/Article/details/girehmyti.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fktsv.cn/Article/details/gfqticqhg.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.vehdjk.com/Article/details/gbxmgzdsd.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.yfazqb.com/Article/details/gkjinughz.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.vehdjk.com/Article/details/gqxxselbd.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.sjlbkw.cn/Article/details/gluypooqc.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.vehdjk.com/Article/details/gkyinkkch.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.sjlbkw.cn/Article/details/gszcufhxo.sHtML


<!-- 参考信息 -->