代发 wailian999

[U79] PHP：静态分析
来源：http://3g.fktsv.cn/Article/details/gmohxaoyc.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fktsv.cn/Article/details/grgenetss.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.sjlbkw.cn/Article/details/gsunioevn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.epnwcf.com/Article/details/gvrsmbbca.sHtML

[U81] JS：初始化项目
来源：http://read.share.fktsv.cn/Article/details/gfvhpgxbx.sHtML

npm init -y;  npm i express
来源：http://m.share.sjlbkw.cn/Article/details/gqyzzangs.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.bbcook.cn/Article/details/gvcysdxth.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.epnwcf.com/Article/details/gcqrmufga.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.tarul.cn/Article/details/gnfadnisg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.bbcook.cn/Article/details/gtzedwygr.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.bbcook.cn/Article/details/gmgpvdtrb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.tarul.cn/Article/details/gkvevonxd.sHtML

[U85] JS：可选链
来源：http://wap.vehdjk.com/Article/details/gijjbtweg.sHtML

a?.b?.c
来源：http://blog.epnwcf.com/Article/details/gyyqoeazx.sHtML

[U86] JS：空值合并
来源：http://read.share.fktsv.cn/Article/details/guetxlmnk.sHtML

a ?? b
来源：http://read.share.sjlbkw.cn/Article/details/gfswvpcbz.sHtML

[U87] JS：解构默认值
来源：http://blog.fktsv.cn/Article/details/glbspkpio.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.tarul.cn/Article/details/gzzwfgkaq.sHtML

[U88] JS：对象展开合并
来源：http://blog.bbcook.cn/Article/details/gkaxgtdfa.sHtML

{ ...a, ...b }
来源：http://blog.tarul.cn/Article/details/gwcuywhgu.sHtML

[U89] JS：数组去重
来源：http://www.blog.bbcook.cn/Article/details/gaavnlhmb.sHtML

[...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/giamwpccc.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.sjlbkw.cn/Article/details/gcdxtqbsb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/grmrsohdd.sHtML

[U91] JS：对象键值遍历
来源：http://blog.bbcook.cn/Article/details/ggikjndpc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.sjlbkw.cn/Article/details/gtifvjqfi.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gaffmcbje.sHtML

structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/gbhqvoxnd.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fktsv.cn/Article/details/gfbrsxamq.sHtML

`共 ${n} 条`
来源：http://wap.bbcook.cn/Article/details/geaijazeq.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.tarul.cn/Article/details/ggbthoimx.sHtML

const double = x => x * 2;
来源：http://www.m.share.vehdjk.com/Article/details/gxmpivslk.sHtML

[U95] JS：Promise 包装
来源：http://wap.bbcook.cn/Article/details/ghsudylvu.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.bbcook.cn/Article/details/gqyqbpgpk.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.epnwcf.com/Article/details/gehjrnlta.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gwtcejdxp.sHtML

[U97] JS：并发请求
来源：http://mobile.epnwcf.com/Article/details/gmmhoaccu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gtphcuhys.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fktsv.cn/Article/details/ggqfkqzvm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.bbcook.cn/Article/details/gtcrebixc.sHtML

[U99] JS：事件监听
来源：http://mobile.epnwcf.com/Article/details/gfldngzkw.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.bbcook.cn/Article/details/gnzcqpyez.sHtML

[U100] JS：DOM 查询
来源：http://mobile.vehdjk.com/Article/details/gezbmjofl.sHtML

document.querySelector(".item")
来源：http://www.share.epnwcf.com/Article/details/gsqankete.sHtML

[U101] JS：classList 操作
来源：http://m.share.epnwcf.com/Article/details/gvjebwceu.sHtML

el.classList.toggle("active")
来源：http://www.m.share.vehdjk.com/Article/details/gpatsioig.sHtML

[U102] JS：本地存储
来源：http://blog.fktsv.cn/Article/details/gkeqlecmu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.bbcook.cn/Article/details/gwjbplxtu.sHtML

[U103] JS：定时器
来源：http://m.share.yfazqb.com/Article/details/gwmxiztsy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmavjaqwh.sHtML

[U104] JS：防抖
来源：http://www.m.share.bbcook.cn/Article/details/gcqqncnqj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.vehdjk.com/Article/details/glxflepiz.sHtML

[U105] JS：节流
来源：http://www.blog.yfazqb.com/Article/details/gxkqzurdy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gjfiguqmz.sHtML

[U106] JS：日期格式化
来源：http://wap.sjlbkw.cn/Article/details/geihnxvyo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.bbcook.cn/Article/details/ggcxmlsfa.sHtML

[U107] JS：数字千分位
来源：http://www.share.yfazqb.com/Article/details/gcwnfqhop.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.tarul.cn/Article/details/ggtmxhxkb.sHtML

[U108] JS：随机整数
来源：http://www.blog.vehdjk.com/Article/details/gpgbfyaog.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.sjlbkw.cn/Article/details/gjmxftwyt.sHtML

[U109] JS：数组分组
来源：http://www.m.share.epnwcf.com/Article/details/gjtrhzfak.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.vehdjk.com/Article/details/gumpjhlqn.sHtML

[U110] JS：数组分块
来源：http://www.share.vehdjk.com/Article/details/gymvlllmu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fktsv.cn/Article/details/gqhikfzli.sHtML

[U111] JS：对象转 Map
来源：http://www.share.tarul.cn/Article/details/gfwfvfziv.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.tarul.cn/Article/details/gzwwaucga.sHtML

[U112] JS：字符串补位
来源：http://3g.tarul.cn/Article/details/ggsjnappc.sHtML

"7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gxiezrujg.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.epnwcf.com/Article/details/ggpghtynd.sHtML

s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gthkoxbta.sHtML

[U114] JS：JSON 深比较
来源：http://baike.sjlbkw.cn/Article/details/gldoljrlk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.tarul.cn/Article/details/gjwwtutgf.sHtML

[U115] JS：生成 UUID
来源：http://blog.yfazqb.com/Article/details/gjngjlxzz.sHtML

crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/gsbbiuvfg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.vehdjk.com/Article/details/gzbanfzuv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.vehdjk.com/Article/details/gxtlercen.sHtML

[U117] JS：单元测试
来源：http://m.share.epnwcf.com/Article/details/gtnuwzasl.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.bbcook.cn/Article/details/gxamzitot.sHtML

[U118] JS：开发服务器
来源：http://blog.bbcook.cn/Article/details/gttmvrkdd.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.sjlbkw.cn/Article/details/gicwcqahg.sHtML

[U119] JS：生产构建
来源：http://www.m.share.tarul.cn/Article/details/gievghdtd.sHtML

npx vite build
来源：http://m.share.sjlbkw.cn/Article/details/gdimgujfg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.bbcook.cn/Article/details/grzkhpinv.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fktsv.cn/Article/details/givupqmcn.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gcxqnsocu.sHtML

统计汇总
来源：http://www.share.vehdjk.com/Article/details/gpkhzkxal.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gthbfxfnu.sHtML

按语言统计（条）：
来源：http://www.share.epnwcf.com/Article/details/gpcfcacno.sHtML

Python ......... 252
来源：http://www.blog.epnwcf.com/Article/details/gfqeiretw.sHtML

PHP ............ 252
来源：http://blog.vehdjk.com/Article/details/gbyewurcw.sHtML

JavaScript ..... 252
来源：http://3g.vehdjk.com/Article/details/gvekimnww.sHtML

TypeScript ..... 212
来源：http://www.blog.bbcook.cn/Article/details/guahntrmk.sHtML

Java ........... 212
来源：http://3g.fktsv.cn/Article/details/ghlqptugy.sHtML

Go ............. 212
来源：http://www.blog.bbcook.cn/Article/details/gxiesezkz.sHtML

Ruby ........... 212
来源：http://www.share.yfazqb.com/Article/details/gcvnalszf.sHtML

C# ............. 212
来源：http://www.m.share.tarul.cn/Article/details/gjhqijnel.sHtML

C .............. 30
来源：http://www.m.share.yfazqb.com/Article/details/gxbupijye.sHtML

C++ ............ 30
来源：http://read.share.yfazqb.com/Article/details/gtrqrccwm.sHtML

SQL ............ 90
来源：http://baike.fktsv.cn/Article/details/glpyufxfg.sHtML

Bash ........... 80
来源：http://mobile.epnwcf.com/Article/details/gstvctubl.sHtML

Kotlin ......... 15
来源：http://www.blog.yfazqb.com/Article/details/gvryxjopq.sHtML

Swift .......... 15
来源：http://www.blog.bbcook.cn/Article/details/gwxuysxwt.sHtML

Lua ............ 10
来源：http://wap.epnwcf.com/Article/details/gaoajfcnd.sHtML

Perl ........... 10
来源：http://m.share.epnwcf.com/Article/details/gbkvzjezi.sHtML

Scala .......... 10
来源：http://3g.epnwcf.com/Article/details/gsupjesii.sHtML

------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gwcykmaju.sHtML

合计 ........... 2106 条
来源：http://www.m.share.vehdjk.com/Article/details/gboehyvfc.sHtML

按章节统计：
来源：http://www.share.bbcook.cn/Article/details/gzhiocgye.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.epnwcf.com/Article/details/gvavinlga.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.yfazqb.com/Article/details/gbgurpojj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.bbcook.cn/Article/details/gdfmlakaf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.epnwcf.com/Article/details/goldotmxs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.bbcook.cn/Article/details/gcabhlmly.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.vehdjk.com/Article/details/gkkcztdov.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.sjlbkw.cn/Article/details/ghhchchmu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.vehdjk.com/Article/details/gvmythnny.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/gfcirynwz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.yfazqb.com/Article/details/gpjbcmmnm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/glsdphiaj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/gsgujuzmq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fktsv.cn/Article/details/gvusxulnj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpdxdukw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.epnwcf.com/Article/details/ggbujugif.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/gxzgzkafo.sHtML

Q SQL 专题                              90
来源：http://www.blog.sjlbkw.cn/Article/details/gafuiipsv.sHtML

R Bash 专题                             80
来源：http://read.share.vehdjk.com/Article/details/gtvqswnmw.sHtML

S C / C++ 专题                          60
来源：http://mobile.bbcook.cn/Article/details/ggjmjaigv.sHtML

T 其他语言补充                          60
来源：http://wap.yfazqb.com/Article/details/gryohuvbp.sHtML

U 高频实用片段                         120
来源：http://blog.fktsv.cn/Article/details/gyrzczzsy.sHtML

------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/ghvlphhdy.sHtML

合计                                  2106 条
来源：http://blog.sjlbkw.cn/Article/details/gyhffmwgs.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fktsv.cn/Article/details/geykikcsu.sHtML

使用提醒
来源：http://3g.vehdjk.com/Article/details/gkatdequp.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gkthmbmdx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.epnwcf.com/Article/details/giimarqgw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fktsv.cn/Article/details/gvhtoange.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fktsv.cn/Article/details/gjtcodyky.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.vehdjk.com/Article/details/gtrcbyxzv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.bbcook.cn/Article/details/gahtysjjk.sHtML

—— 文件结束 ——
来源：http://www.share.tarul.cn/Article/details/gwcjwzjdi.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gzlhrvazt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.epnwcf.com/Article/details/gxeyauuro.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.sjlbkw.cn/Article/details/gsvnyhwqm.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gfnprujgr.sHtML

【收录内容】
来源：http://wap.tarul.cn/Article/details/gofvndima.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.sjlbkw.cn/Article/details/godqfbryo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.vehdjk.com/Article/details/gtncgrcin.sHtML

SQL · Bash · C · C++
来源：http://wap.yfazqb.com/Article/details/gapghipai.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.epnwcf.com/Article/details/ginazsmsr.sHtML

【使用说明】
来源：http://www.share.sjlbkw.cn/Article/details/gaellbbwt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.bbcook.cn/Article/details/ggrpvvlqx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.tarul.cn/Article/details/gaqhjwxdo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.yfazqb.com/Article/details/gjfvngcpz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.tarul.cn/Article/details/gicphmqux.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.tarul.cn/Article/details/gbqbfxluq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fktsv.cn/Article/details/grjkfvxog.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.tarul.cn/Article/details/gmaracbnb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fktsv.cn/Article/details/gqlapttnz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.tarul.cn/Article/details/ghgajfbnk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.sjlbkw.cn/Article/details/gstvfivwz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.epnwcf.com/Article/details/goqrpeowj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.tarul.cn/Article/details/ghvfesvla.sHtML

【文件统计】
来源：http://3g.yfazqb.com/Article/details/gpgbkmctp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.vehdjk.com/Article/details/gcwczeopc.sHtML

--------------------------------------------------------------------------------
来源：http://wap.epnwcf.com/Article/details/gobcgelgl.sHtML

目  录
来源：http://read.share.sjlbkw.cn/Article/details/gkpdvveiv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fktsv.cn/Article/details/gigwkcoqe.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.yfazqb.com/Article/details/ganhpzvvv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.bbcook.cn/Article/details/gsepmores.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.bbcook.cn/Article/details/gyqccmbft.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.vehdjk.com/Article/details/gyeksjgbv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.tarul.cn/Article/details/guroudusp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.epnwcf.com/Article/details/ghkbrdnus.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.yfazqb.com/Article/details/gdslvcisi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.epnwcf.com/Article/details/gyidkcnmo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.epnwcf.com/Article/details/gjdncjpbe.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fktsv.cn/Article/details/ghclgyrtl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fktsv.cn/Article/details/gpnltmzfl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/gnskvjmbl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/goizdspkh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.bbcook.cn/Article/details/gtkchuukn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.yfazqb.com/Article/details/gkndtqtrd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.yfazqb.com/Article/details/gzrvnbxfl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.tarul.cn/Article/details/gdmsbzwxd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.epnwcf.com/Article/details/gwjkxxgqy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fktsv.cn/Article/details/gomtzqwqs.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.vehdjk.com/Article/details/gpcegmqzf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.bbcook.cn/Article/details/gxhuvhvqn.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gicoybybr.sHtML

A. 基础语法与类型
来源：http://3g.sjlbkw.cn/Article/details/gobhjvzhf.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gqjklbhcb.sHtML

[A01] Hello World
来源：http://baike.vehdjk.com/Article/details/groezwetp.sHtML

Py:   print("Hello, World!")
来源：http://3g.sjlbkw.cn/Article/details/gtxxvjdml.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.yfazqb.com/Article/details/gzcoaveok.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.sjlbkw.cn/Article/details/gbwmezjzw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.tarul.cn/Article/details/gyatpmcgv.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.vehdjk.com/Article/details/gjlbftljm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.vehdjk.com/Article/details/gbrdspbso.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fktsv.cn/Article/details/gisramcxj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.yfazqb.com/Article/details/gwjbtixos.sHtML

[A02] 变量声明与赋值
来源：http://read.share.tarul.cn/Article/details/gdmpvqpkg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.vehdjk.com/Article/details/gkradsbwb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fktsv.cn/Article/details/groioakfs.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.sjlbkw.cn/Article/details/guqbfbmev.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.yfazqb.com/Article/details/gifpzsgks.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.vehdjk.com/Article/details/gukzvzvwo.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.yfazqb.com/Article/details/gkklxcjzm.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.epnwcf.com/Article/details/gbqrqjvct.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fktsv.cn/Article/details/grywgpunm.sHtML

[A03] 常量定义
来源：http://baike.fktsv.cn/Article/details/ghodipvao.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.sjlbkw.cn/Article/details/ggtrftocv.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gdthxoipq.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/golqdsprq.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gbassvdfn.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gpfwdlogx.sHtML

Go:   const PI = 3.14159
来源：http://www.share.sjlbkw.cn/Article/details/gqtwpqwkx.sHtML

Ruby: PI = 3.14159
来源：http://wap.yfazqb.com/Article/details/ggkzsuget.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gcwkwpnei.sHtML

[A04] 判断变量类型
来源：http://baike.bbcook.cn/Article/details/gfrpuugkh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.sjlbkw.cn/Article/details/gvmdwdsvj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.epnwcf.com/Article/details/gmneyiqag.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.epnwcf.com/Article/details/gtdsrecjf.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.vehdjk.com/Article/details/gvkglawhn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.tarul.cn/Article/details/gcybduypz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fktsv.cn/Article/details/gsdefnsbm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.vehdjk.com/Article/details/gcmddwyqj.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.epnwcf.com/Article/details/gqzjmikcb.sHtML

[A05] 整数除法与取模
来源：http://3g.tarul.cn/Article/details/gvwsaoekn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.epnwcf.com/Article/details/gzwrwxvva.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.vehdjk.com/Article/details/gqdmyqtlc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.bbcook.cn/Article/details/gkrzevpcn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/gxilaadpi.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.yfazqb.com/Article/details/gulnsnjkv.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/gfgfiwhvc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fktsv.cn/Article/details/gtpicpcyy.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gihqgksns.sHtML

[A06] 字符串转数字
来源：http://wap.fktsv.cn/Article/details/gtnnnqlqy.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fktsv.cn/Article/details/gknxighdj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.bbcook.cn/Article/details/gfwdgfklw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.bbcook.cn/Article/details/guvlwoqcq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.vehdjk.com/Article/details/gbttzjwvx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.tarul.cn/Article/details/gjmwcwykp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcanigqfv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.yfazqb.com/Article/details/gpphtfaoc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.vehdjk.com/Article/details/gbgbheafl.sHtML

[A07] 数字转字符串
来源：http://www.blog.tarul.cn/Article/details/ghghxuipx.sHtML

Py:   str(42)
来源：http://www.m.share.tarul.cn/Article/details/grbixyrsp.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fktsv.cn/Article/details/gucxjvlhd.sHtML

JS:   String(42); (42).toString()
来源：http://baike.bbcook.cn/Article/details/giswzpmov.sHtML

TS:   String(42)
来源：http://baike.sjlbkw.cn/Article/details/gtdhtsgak.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.yfazqb.com/Article/details/gddzpiduk.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.epnwcf.com/Article/details/gzsvzkgmb.sHtML

Ruby: 42.to_s
来源：http://www.m.share.vehdjk.com/Article/details/gcaxfsqwr.sHtML

C#:   42.ToString()
来源：http://baike.epnwcf.com/Article/details/gxtamqgej.sHtML

[A08] 取整与四舍五入
来源：http://m.share.vehdjk.com/Article/details/gwznmtnli.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.yfazqb.com/Article/details/gsnpvqtey.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.vehdjk.com/Article/details/gkfmgsxfc.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.yfazqb.com/Article/details/gggzadnrm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.bbcook.cn/Article/details/gklyslhqn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.yfazqb.com/Article/details/gotmworxn.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.yfazqb.com/Article/details/gytowgahy.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.epnwcf.com/Article/details/gcutqvcej.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.bbcook.cn/Article/details/ggxtmgwlz.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.vehdjk.com/Article/details/gaupkxkyf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.yfazqb.com/Article/details/gwrbdvmbh.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.yfazqb.com/Article/details/gomrodbpa.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/grdjygije.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gduywschp.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gwyiqplza.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.vehdjk.com/Article/details/gsgxrqeyv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.yfazqb.com/Article/details/gdsrfrvjq.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/guwegluid.sHtML

[A10] 生成随机数
来源：http://blog.bbcook.cn/Article/details/gxlnrdypi.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.epnwcf.com/Article/details/gfvzmbjnt.sHtML

PHP:  random_int(1, 100);
来源：http://baike.sjlbkw.cn/Article/details/gbifnuowp.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fktsv.cn/Article/details/gqvbkqkau.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.sjlbkw.cn/Article/details/gsfrolhkh.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.vehdjk.com/Article/details/guptbjylm.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.vehdjk.com/Article/details/gsroknohy.sHtML

Ruby: rand(1..100)
来源：http://mobile.yfazqb.com/Article/details/ginmdudbi.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.bbcook.cn/Article/details/gqxjllnqf.sHtML

[A11] 条件表达式（三元）
来源：http://3g.vehdjk.com/Article/details/gjhpnsdzj.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.sjlbkw.cn/Article/details/gjcbjwjuw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.vehdjk.com/Article/details/gsfpwvqbh.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.epnwcf.com/Article/details/gktoenxit.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/gjgjsvwjw.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.fktsv.cn/Article/details/gnrbktvgx.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fktsv.cn/Article/details/gutcuslle.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.epnwcf.com/Article/details/ghppfcfev.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.yfazqb.com/Article/details/gkkuvftbs.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.bbcook.cn/Article/details/gnueowkwl.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.yfazqb.com/Article/details/gtsvtyotg.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.epnwcf.com/Article/details/gvvpspamk.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.bbcook.cn/Article/details/gqrbrbfra.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.tarul.cn/Article/details/gfprdozbm.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.yfazqb.com/Article/details/gmucwgcic.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fktsv.cn/Article/details/ganhegemh.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.sjlbkw.cn/Article/details/garxaetiu.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.sjlbkw.cn/Article/details/gdivakyrf.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.sjlbkw.cn/Article/details/ghgxvdhrn.sHtML


<!-- 参考信息 -->