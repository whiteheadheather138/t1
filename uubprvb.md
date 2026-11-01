代发 wailian999

[U75] PHP：依赖注入
来源：http://www.m.share.sjlbkw.cn/Article/details/gphorsyat.sHtML

composer require psr/container
来源：http://blog.epnwcf.com/Article/details/grmkgzgdf.sHtML

[U76] PHP：简单路由
来源：http://read.share.yfazqb.com/Article/details/guobxyyga.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.vehdjk.com/Article/details/gptksdyuz.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.yfazqb.com/Article/details/griorzjey.sHtML

composer require twig/twig
来源：http://baike.epnwcf.com/Article/details/gihjsmpgz.sHtML

[U78] PHP：单元测试
来源：http://m.share.vehdjk.com/Article/details/gyiwzdlnp.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.bbcook.cn/Article/details/gshvfhbje.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.tarul.cn/Article/details/gxhfdzxhh.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.bbcook.cn/Article/details/garzxqbte.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.vehdjk.com/Article/details/guixpszxe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.yfazqb.com/Article/details/gmghrnsdy.sHtML

[U81] JS：初始化项目
来源：http://www.share.epnwcf.com/Article/details/ghvjinhml.sHtML

npm init -y;  npm i express
来源：http://blog.epnwcf.com/Article/details/gkpgbmwnk.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.tarul.cn/Article/details/glhpdxhfv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fktsv.cn/Article/details/gjkgmjqmy.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.sjlbkw.cn/Article/details/ghocxxdmp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.yfazqb.com/Article/details/grkviaywj.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.vehdjk.com/Article/details/gqfithder.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fktsv.cn/Article/details/gpujbfpzl.sHtML

[U85] JS：可选链
来源：http://www.m.share.epnwcf.com/Article/details/githupkvp.sHtML

a?.b?.c
来源：http://wap.fktsv.cn/Article/details/giecsqhwv.sHtML

[U86] JS：空值合并
来源：http://3g.sjlbkw.cn/Article/details/gytebcotb.sHtML

a ?? b
来源：http://mobile.bbcook.cn/Article/details/gzhhpcaus.sHtML

[U87] JS：解构默认值
来源：http://www.blog.bbcook.cn/Article/details/glprwwfpf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.yfazqb.com/Article/details/gbipdtzur.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.vehdjk.com/Article/details/gbbmgqtkq.sHtML

{ ...a, ...b }
来源：http://mobile.fktsv.cn/Article/details/guuwacxhg.sHtML

[U89] JS：数组去重
来源：http://mobile.epnwcf.com/Article/details/gtnvchvfm.sHtML

[...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/ghbrzxcdl.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.epnwcf.com/Article/details/gcskstpek.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrcznvhb.sHtML

[U91] JS：对象键值遍历
来源：http://blog.tarul.cn/Article/details/girfrcddw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.tarul.cn/Article/details/gzrgszhis.sHtML

[U92] JS：深拷贝
来源：http://blog.tarul.cn/Article/details/gviwtgywh.sHtML

structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/ghnqrppau.sHtML

[U93] JS：模板字符串
来源：http://mobile.epnwcf.com/Article/details/glbjkjpfu.sHtML

`共 ${n} 条`
来源：http://read.share.vehdjk.com/Article/details/gafdrgrbf.sHtML

[U94] JS：箭头函数
来源：http://wap.bbcook.cn/Article/details/gtjvrbcbb.sHtML

const double = x => x * 2;
来源：http://baike.bbcook.cn/Article/details/gzvypijxc.sHtML

[U95] JS：Promise 包装
来源：http://blog.bbcook.cn/Article/details/gypzubeqd.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.sjlbkw.cn/Article/details/geveptefq.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.yfazqb.com/Article/details/gvpfndphz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gtdyzxegc.sHtML

[U97] JS：并发请求
来源：http://read.share.fktsv.cn/Article/details/gapnwloyq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/gmedrrkyw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.vehdjk.com/Article/details/gvxrzqwkj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.epnwcf.com/Article/details/ghxuhqfys.sHtML

[U99] JS：事件监听
来源：http://wap.bbcook.cn/Article/details/gqrprnnla.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fktsv.cn/Article/details/gmrvgvspu.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.bbcook.cn/Article/details/gsbslzagj.sHtML

document.querySelector(".item")
来源：http://www.share.fktsv.cn/Article/details/gkfwoxrcd.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.bbcook.cn/Article/details/gbagdnaet.sHtML

el.classList.toggle("active")
来源：http://3g.bbcook.cn/Article/details/gbuujytqr.sHtML

[U102] JS：本地存储
来源：http://mobile.yfazqb.com/Article/details/grbhaeewx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.vehdjk.com/Article/details/gsyovgrtf.sHtML

[U103] JS：定时器
来源：http://www.share.epnwcf.com/Article/details/grjcwrzjv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.bbcook.cn/Article/details/gjmhnvzhw.sHtML

[U104] JS：防抖
来源：http://3g.bbcook.cn/Article/details/gofwmucxr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.sjlbkw.cn/Article/details/glegpgrsw.sHtML

[U105] JS：节流
来源：http://blog.yfazqb.com/Article/details/ghsaxzwsd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.yfazqb.com/Article/details/gdmxjnldv.sHtML

[U106] JS：日期格式化
来源：http://read.share.epnwcf.com/Article/details/gikvofvok.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.vehdjk.com/Article/details/gcxorzvna.sHtML

[U107] JS：数字千分位
来源：http://wap.vehdjk.com/Article/details/gwradvywl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.tarul.cn/Article/details/gzjjkkcsn.sHtML

[U108] JS：随机整数
来源：http://m.share.bbcook.cn/Article/details/galmiilpt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.epnwcf.com/Article/details/gwszowmxf.sHtML

[U109] JS：数组分组
来源：http://baike.tarul.cn/Article/details/guakowdto.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.bbcook.cn/Article/details/grjbgilay.sHtML

[U110] JS：数组分块
来源：http://baike.epnwcf.com/Article/details/ggzkvvpem.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.tarul.cn/Article/details/gpfzmzret.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.sjlbkw.cn/Article/details/gesiofdcl.sHtML

new Map(Object.entries(obj))
来源：http://wap.bbcook.cn/Article/details/gmautjeqp.sHtML

[U112] JS：字符串补位
来源：http://read.share.vehdjk.com/Article/details/gvcxaykpl.sHtML

"7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/ggyyrtqsk.sHtML

[U113] JS：正则替换全部
来源：http://m.share.sjlbkw.cn/Article/details/ggdreobvb.sHtML

s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/gjriqbeit.sHtML

[U114] JS：JSON 深比较
来源：http://wap.sjlbkw.cn/Article/details/gmxklzrgp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.yfazqb.com/Article/details/ggtqiyehr.sHtML

[U115] JS：生成 UUID
来源：http://read.share.tarul.cn/Article/details/gashvhilr.sHtML

crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gvpxznpyn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.bbcook.cn/Article/details/gyizrzegy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.epnwcf.com/Article/details/gnkjypnlg.sHtML

[U117] JS：单元测试
来源：http://m.share.sjlbkw.cn/Article/details/grysdlxmg.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.epnwcf.com/Article/details/gavyepjfq.sHtML

[U118] JS：开发服务器
来源：http://blog.tarul.cn/Article/details/gpfofsvvt.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.epnwcf.com/Article/details/gjeirjvzt.sHtML

[U119] JS：生产构建
来源：http://m.share.vehdjk.com/Article/details/gttvafrlp.sHtML

npx vite build
来源：http://www.share.sjlbkw.cn/Article/details/golocerxd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.sjlbkw.cn/Article/details/gdeifwtwm.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.sjlbkw.cn/Article/details/ggupvfrog.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gavmkcwie.sHtML

统计汇总
来源：http://www.share.sjlbkw.cn/Article/details/gbxeuhtge.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gychjsxdz.sHtML

按语言统计（条）：
来源：http://www.share.epnwcf.com/Article/details/gntxzihsh.sHtML

Python ......... 252
来源：http://m.share.fktsv.cn/Article/details/gfolvzogd.sHtML

PHP ............ 252
来源：http://3g.epnwcf.com/Article/details/gwceqkyxy.sHtML

JavaScript ..... 252
来源：http://read.share.yfazqb.com/Article/details/gsieeoeek.sHtML

TypeScript ..... 212
来源：http://mobile.bbcook.cn/Article/details/ghuamvymd.sHtML

Java ........... 212
来源：http://www.blog.yfazqb.com/Article/details/gskkiskzn.sHtML

Go ............. 212
来源：http://read.share.sjlbkw.cn/Article/details/gdopvqich.sHtML

Ruby ........... 212
来源：http://mobile.epnwcf.com/Article/details/gxrjtobih.sHtML

C# ............. 212
来源：http://www.blog.epnwcf.com/Article/details/gtwiysuqw.sHtML

C .............. 30
来源：http://wap.fktsv.cn/Article/details/gauegclww.sHtML

C++ ............ 30
来源：http://m.share.yfazqb.com/Article/details/gytyvjlek.sHtML

SQL ............ 90
来源：http://m.share.yfazqb.com/Article/details/gbpbkopdl.sHtML

Bash ........... 80
来源：http://mobile.tarul.cn/Article/details/gxqwgoeda.sHtML

Kotlin ......... 15
来源：http://3g.tarul.cn/Article/details/gbvwrwnep.sHtML

Swift .......... 15
来源：http://3g.yfazqb.com/Article/details/gaqejztes.sHtML

Lua ............ 10
来源：http://read.share.vehdjk.com/Article/details/ggabmchyp.sHtML

Perl ........... 10
来源：http://m.share.epnwcf.com/Article/details/gurrkilps.sHtML

Scala .......... 10
来源：http://blog.epnwcf.com/Article/details/gbntwuvzh.sHtML

------------------------------------
来源：http://baike.yfazqb.com/Article/details/gmblvfeef.sHtML

合计 ........... 2106 条
来源：http://m.share.epnwcf.com/Article/details/gzbtswbvi.sHtML

按章节统计：
来源：http://baike.epnwcf.com/Article/details/gsxpnfnax.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.epnwcf.com/Article/details/gkszvlahm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.tarul.cn/Article/details/gneauhdoj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.vehdjk.com/Article/details/glwdnhmgu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.vehdjk.com/Article/details/gmqiftaoa.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.sjlbkw.cn/Article/details/gxalzpgba.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fktsv.cn/Article/details/gkdqddfzl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.sjlbkw.cn/Article/details/gqpvoxpeu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.vehdjk.com/Article/details/gyrjtgqlj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/gphanhmor.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.epnwcf.com/Article/details/gxikradul.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.tarul.cn/Article/details/gdhhmnrcx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gzpuufjeh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/glxbvuhnx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.tarul.cn/Article/details/gshkgxzhz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.vehdjk.com/Article/details/gkqzriksq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gkqffrfjk.sHtML

Q SQL 专题                              90
来源：http://www.share.fktsv.cn/Article/details/gwldjnfkg.sHtML

R Bash 专题                             80
来源：http://www.share.bbcook.cn/Article/details/gxnevvqbc.sHtML

S C / C++ 专题                          60
来源：http://www.blog.sjlbkw.cn/Article/details/gycyrljma.sHtML

T 其他语言补充                          60
来源：http://blog.bbcook.cn/Article/details/gxomdfymc.sHtML

U 高频实用片段                         120
来源：http://wap.vehdjk.com/Article/details/ghtwoeajs.sHtML

------------------------------------
来源：http://m.share.tarul.cn/Article/details/ghhjqexvm.sHtML

合计                                  2106 条
来源：http://read.share.fktsv.cn/Article/details/gwkpjvmuk.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gjjkuqrsu.sHtML

使用提醒
来源：http://read.share.sjlbkw.cn/Article/details/gzmiqtnti.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gsyxcewlm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.sjlbkw.cn/Article/details/gakuwsvhq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.bbcook.cn/Article/details/greljtirk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.sjlbkw.cn/Article/details/gkqibpctl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.epnwcf.com/Article/details/gygnpqbjo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.tarul.cn/Article/details/gmpgdmzpz.sHtML

—— 文件结束 ——
来源：http://3g.vehdjk.com/Article/details/gawuncyqp.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gwiuryrqh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.epnwcf.com/Article/details/gqtzrxmpt.sHtML

Common Programming Examples Cheat Book
来源：http://3g.vehdjk.com/Article/details/gxxpjmszt.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gwsqpdstc.sHtML

【收录内容】
来源：http://www.m.share.vehdjk.com/Article/details/gzanvgwwk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.epnwcf.com/Article/details/galkjnikz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.yfazqb.com/Article/details/gulhcpmjl.sHtML

SQL · Bash · C · C++
来源：http://www.share.tarul.cn/Article/details/gbgbwfeto.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.tarul.cn/Article/details/gyqjqrkry.sHtML

【使用说明】
来源：http://blog.sjlbkw.cn/Article/details/gxhyxmmgv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.bbcook.cn/Article/details/gmfrqosqs.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.vehdjk.com/Article/details/giewcyjiz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.tarul.cn/Article/details/glhnlmsyx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.bbcook.cn/Article/details/gizzggixs.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.epnwcf.com/Article/details/gzsznrciy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.bbcook.cn/Article/details/gixtrnpxn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.tarul.cn/Article/details/glrkvtvtl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.tarul.cn/Article/details/gemokceej.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.bbcook.cn/Article/details/gpdtemssf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.tarul.cn/Article/details/gdtgewplh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.sjlbkw.cn/Article/details/gflwiduhv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.sjlbkw.cn/Article/details/gaatwjpmz.sHtML

【文件统计】
来源：http://www.blog.sjlbkw.cn/Article/details/gefrsxukn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.bbcook.cn/Article/details/gzgwynjzm.sHtML

--------------------------------------------------------------------------------
来源：http://blog.epnwcf.com/Article/details/gkjnwjabe.sHtML

目  录
来源：http://read.share.fktsv.cn/Article/details/giuzuuwdg.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/gotnagqui.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.epnwcf.com/Article/details/gdkxqumre.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.vehdjk.com/Article/details/gfjeqxqmy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.bbcook.cn/Article/details/gxkwkmwmh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.yfazqb.com/Article/details/geucdzouc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.bbcook.cn/Article/details/grbgfnape.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.epnwcf.com/Article/details/gyqsmxokh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.bbcook.cn/Article/details/gazclicuu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.tarul.cn/Article/details/gpudtpxlw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.epnwcf.com/Article/details/gznimebij.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fktsv.cn/Article/details/girpwpyzd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/gbqwhbqph.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.epnwcf.com/Article/details/gjnkvlmds.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.vehdjk.com/Article/details/gmjuxvnws.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxjguclj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.tarul.cn/Article/details/grbgtiwjk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.epnwcf.com/Article/details/ghmqlgosf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.sjlbkw.cn/Article/details/gcayhtfyp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.epnwcf.com/Article/details/gywzqygda.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.yfazqb.com/Article/details/gbiiojdtz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.vehdjk.com/Article/details/gsfdrweek.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.tarul.cn/Article/details/gzmglncfk.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gwcdbwomv.sHtML

A. 基础语法与类型
来源：http://m.share.bbcook.cn/Article/details/gkjlupiak.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtqccascn.sHtML

[A01] Hello World
来源：http://www.share.bbcook.cn/Article/details/gtgvbsrbi.sHtML

Py:   print("Hello, World!")
来源：http://baike.bbcook.cn/Article/details/gmbhihamm.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.epnwcf.com/Article/details/gaimvdeuw.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.bbcook.cn/Article/details/gjvnmvvaq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.tarul.cn/Article/details/ghnpqhjbs.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.epnwcf.com/Article/details/gsuguifhw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.vehdjk.com/Article/details/gtganokdh.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fktsv.cn/Article/details/gvjfhnqom.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.sjlbkw.cn/Article/details/gatzgwtnj.sHtML

[A02] 变量声明与赋值
来源：http://baike.bbcook.cn/Article/details/gekzrkzon.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.tarul.cn/Article/details/gflrwqbsp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.yfazqb.com/Article/details/gkjkzdznz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.vehdjk.com/Article/details/gfutmmbbx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.bbcook.cn/Article/details/glajiwsxw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fktsv.cn/Article/details/gbxdxjdeh.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.yfazqb.com/Article/details/grkdilpbt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.bbcook.cn/Article/details/gmkqxfwdl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.yfazqb.com/Article/details/gjtgjinpf.sHtML

[A03] 常量定义
来源：http://m.share.tarul.cn/Article/details/gsnbszhjr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.epnwcf.com/Article/details/ghjymyvye.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gxfppygzv.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gxulsuqup.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gmmccpvjd.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gggihmgnk.sHtML

Go:   const PI = 3.14159
来源：http://m.share.yfazqb.com/Article/details/ghbkdzqsh.sHtML

Ruby: PI = 3.14159
来源：http://blog.fktsv.cn/Article/details/gcpqsvexl.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/gshqvzkqo.sHtML

[A04] 判断变量类型
来源：http://mobile.vehdjk.com/Article/details/gqfkuyxkc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.yfazqb.com/Article/details/gjlpocvhc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.yfazqb.com/Article/details/gupqzuadp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.bbcook.cn/Article/details/gyeoohshh.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.sjlbkw.cn/Article/details/gosigtttj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.tarul.cn/Article/details/gbsbanxpr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.bbcook.cn/Article/details/glkatszct.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.yfazqb.com/Article/details/gtrrbsgyu.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.epnwcf.com/Article/details/gonijqjgg.sHtML

[A05] 整数除法与取模
来源：http://www.share.bbcook.cn/Article/details/gxseyxjip.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.tarul.cn/Article/details/gexdvjbyw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.epnwcf.com/Article/details/gfgwylfli.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.yfazqb.com/Article/details/gcfnekwbu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gpeijlwzq.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.epnwcf.com/Article/details/gpahxtqpf.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gzkdkiqra.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fktsv.cn/Article/details/gxxzgcaln.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.tarul.cn/Article/details/gciyoglbh.sHtML

[A06] 字符串转数字
来源：http://3g.vehdjk.com/Article/details/gzbbmynse.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.sjlbkw.cn/Article/details/ggnqudozx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.sjlbkw.cn/Article/details/gjsbktakg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.sjlbkw.cn/Article/details/gclvcyaut.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.vehdjk.com/Article/details/gvfjtnmai.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fktsv.cn/Article/details/gybvgeala.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.tarul.cn/Article/details/guzghpooe.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.epnwcf.com/Article/details/gcsigthqb.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.tarul.cn/Article/details/gwwwgcrgd.sHtML

[A07] 数字转字符串
来源：http://m.share.epnwcf.com/Article/details/ghsxwkrch.sHtML

Py:   str(42)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxsvsssud.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.sjlbkw.cn/Article/details/gdcgrnujh.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.bbcook.cn/Article/details/gkzdpcltt.sHtML

TS:   String(42)
来源：http://www.m.share.bbcook.cn/Article/details/gjevtafpj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.tarul.cn/Article/details/gceqenudm.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.epnwcf.com/Article/details/gcgsgdfxk.sHtML

Ruby: 42.to_s
来源：http://read.share.epnwcf.com/Article/details/gthidhobv.sHtML

C#:   42.ToString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkqfywdl.sHtML

[A08] 取整与四舍五入
来源：http://blog.epnwcf.com/Article/details/ghbzzhqjh.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fktsv.cn/Article/details/goeqjoyxs.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.yfazqb.com/Article/details/gpjtkgivo.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.fktsv.cn/Article/details/gjmntldhg.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.epnwcf.com/Article/details/gmqgarhcu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.sjlbkw.cn/Article/details/gcmenlvfz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.tarul.cn/Article/details/gofuqwtvc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.tarul.cn/Article/details/gqibevilv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.yfazqb.com/Article/details/gmnlsxivk.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.tarul.cn/Article/details/gpycuqecs.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.tarul.cn/Article/details/gzlrmpcob.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/glgolncco.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.epnwcf.com/Article/details/gbihwakva.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.vehdjk.com/Article/details/gygwutknz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gcmdayrlg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.epnwcf.com/Article/details/ghhoqrell.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.epnwcf.com/Article/details/gjrvlmevs.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/ggjbbobtt.sHtML

[A10] 生成随机数
来源：http://m.share.sjlbkw.cn/Article/details/ggughvyyj.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.yfazqb.com/Article/details/gtubolpuq.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.vehdjk.com/Article/details/gisdthtfh.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.epnwcf.com/Article/details/gyngjhvtd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.epnwcf.com/Article/details/gclvzeqcp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.tarul.cn/Article/details/gwvkrzshe.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.vehdjk.com/Article/details/gzwgqjjfb.sHtML

Ruby: rand(1..100)
来源：http://read.share.fktsv.cn/Article/details/gaajsqqsc.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.epnwcf.com/Article/details/gypvcgwlm.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.epnwcf.com/Article/details/gvhpmqadr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.bbcook.cn/Article/details/gcdkajtno.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.bbcook.cn/Article/details/gasihsetb.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.epnwcf.com/Article/details/glblqdrol.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.bbcook.cn/Article/details/ggyrwudfy.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.epnwcf.com/Article/details/grhyxnxyx.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.epnwcf.com/Article/details/gxuopxpoj.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.bbcook.cn/Article/details/gxaspiipu.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.yfazqb.com/Article/details/gozxdyevh.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fktsv.cn/Article/details/gribcqbud.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.bbcook.cn/Article/details/gtjfhodyo.sHtML


<!-- 参考信息 -->