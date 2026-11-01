代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://blog.tarul.cn/Article/details/ghhvevice.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.sjlbkw.cn/Article/details/gpafwmkhm.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fktsv.cn/Article/details/gyrocwils.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.tarul.cn/Article/details/gikermuao.sHtML

[U75] PHP：依赖注入
来源：http://read.share.tarul.cn/Article/details/grcbolime.sHtML

composer require psr/container
来源：http://3g.bbcook.cn/Article/details/gdgzqacfv.sHtML

[U76] PHP：简单路由
来源：http://m.share.sjlbkw.cn/Article/details/geoegdhtk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.vehdjk.com/Article/details/giqlcmqjk.sHtML

[U77] PHP：模板渲染
来源：http://blog.yfazqb.com/Article/details/gdbvgkmaw.sHtML

composer require twig/twig
来源：http://wap.sjlbkw.cn/Article/details/gvvmwgrus.sHtML

[U78] PHP：单元测试
来源：http://baike.sjlbkw.cn/Article/details/gdctczick.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.yfazqb.com/Article/details/gbrifrnaq.sHtML

[U79] PHP：静态分析
来源：http://baike.vehdjk.com/Article/details/gemszakoa.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fktsv.cn/Article/details/gpeaznioo.sHtML

[U80] PHP：代码规范修复
来源：http://3g.tarul.cn/Article/details/gxfylfwyj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.epnwcf.com/Article/details/ggugocyhf.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.vehdjk.com/Article/details/gdqxsvwfd.sHtML

npm init -y;  npm i express
来源：http://m.share.tarul.cn/Article/details/gyrjpaoct.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fktsv.cn/Article/details/gcehmmepe.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.tarul.cn/Article/details/gmpkspmsx.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.sjlbkw.cn/Article/details/ggjdddfup.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.yfazqb.com/Article/details/gdpkcjdoo.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.vehdjk.com/Article/details/gscdspvjk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fktsv.cn/Article/details/gbyluuvvg.sHtML

[U85] JS：可选链
来源：http://www.blog.epnwcf.com/Article/details/gwiwzvxjy.sHtML

a?.b?.c
来源：http://baike.tarul.cn/Article/details/gvycfvdzc.sHtML

[U86] JS：空值合并
来源：http://baike.vehdjk.com/Article/details/gbfokoclm.sHtML

a ?? b
来源：http://3g.epnwcf.com/Article/details/gwunlpryv.sHtML

[U87] JS：解构默认值
来源：http://mobile.epnwcf.com/Article/details/gwkzhzrqr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.tarul.cn/Article/details/gmrionhmk.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.epnwcf.com/Article/details/gujyffljz.sHtML

{ ...a, ...b }
来源：http://3g.sjlbkw.cn/Article/details/gogbgxjua.sHtML

[U89] JS：数组去重
来源：http://www.blog.fktsv.cn/Article/details/gsywnkklz.sHtML

[...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/ghyiozeri.sHtML

[U90] JS：数字数组排序
来源：http://3g.bbcook.cn/Article/details/gtewxrqic.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/gnjejcyjs.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.yfazqb.com/Article/details/geszjlgdp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.bbcook.cn/Article/details/gusilbyop.sHtML

[U92] JS：深拷贝
来源：http://3g.vehdjk.com/Article/details/gxuadrjja.sHtML

structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gymgsxojp.sHtML

[U93] JS：模板字符串
来源：http://blog.bbcook.cn/Article/details/glhrhoeks.sHtML

`共 ${n} 条`
来源：http://m.share.sjlbkw.cn/Article/details/gkoeevndr.sHtML

[U94] JS：箭头函数
来源：http://www.blog.vehdjk.com/Article/details/gmcwhhajn.sHtML

const double = x => x * 2;
来源：http://www.blog.vehdjk.com/Article/details/gsplfnqgk.sHtML

[U95] JS：Promise 包装
来源：http://3g.bbcook.cn/Article/details/gbvlaosro.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.bbcook.cn/Article/details/gqnuponrb.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.tarul.cn/Article/details/gyodfbkrz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.sjlbkw.cn/Article/details/gizqjzeie.sHtML

[U97] JS：并发请求
来源：http://m.share.epnwcf.com/Article/details/gfalrexnx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gscaejvio.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.yfazqb.com/Article/details/gmjknuzsw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.vehdjk.com/Article/details/gmywpywlo.sHtML

[U99] JS：事件监听
来源：http://www.share.bbcook.cn/Article/details/gpdsseskn.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fktsv.cn/Article/details/giqffmscg.sHtML

[U100] JS：DOM 查询
来源：http://3g.bbcook.cn/Article/details/gdjvzcxws.sHtML

document.querySelector(".item")
来源：http://mobile.epnwcf.com/Article/details/gujfuuypk.sHtML

[U101] JS：classList 操作
来源：http://baike.vehdjk.com/Article/details/gerwpvxvm.sHtML

el.classList.toggle("active")
来源：http://wap.vehdjk.com/Article/details/gwxzatodz.sHtML

[U102] JS：本地存储
来源：http://3g.epnwcf.com/Article/details/gyzpekhoh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.bbcook.cn/Article/details/gjonfmbbh.sHtML

[U103] JS：定时器
来源：http://read.share.yfazqb.com/Article/details/ggqlbzahv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.epnwcf.com/Article/details/gsjqudqwn.sHtML

[U104] JS：防抖
来源：http://mobile.sjlbkw.cn/Article/details/gdrbmwpqe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/gpedfmqil.sHtML

[U105] JS：节流
来源：http://www.blog.sjlbkw.cn/Article/details/ggexfcliw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.vehdjk.com/Article/details/gsbrtixal.sHtML

[U106] JS：日期格式化
来源：http://m.share.vehdjk.com/Article/details/gpphhihjf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.yfazqb.com/Article/details/ggvnvgbpw.sHtML

[U107] JS：数字千分位
来源：http://read.share.bbcook.cn/Article/details/gybcgdqli.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fktsv.cn/Article/details/ghroafawu.sHtML

[U108] JS：随机整数
来源：http://mobile.sjlbkw.cn/Article/details/gwjsekjjo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.epnwcf.com/Article/details/gagmyzabq.sHtML

[U109] JS：数组分组
来源：http://mobile.yfazqb.com/Article/details/gvohnooyv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.epnwcf.com/Article/details/godvrviqr.sHtML

[U110] JS：数组分块
来源：http://www.blog.tarul.cn/Article/details/gzkospqzk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.sjlbkw.cn/Article/details/gpnlbcqol.sHtML

[U111] JS：对象转 Map
来源：http://3g.yfazqb.com/Article/details/gvzyaxfnd.sHtML

new Map(Object.entries(obj))
来源：http://wap.yfazqb.com/Article/details/gtdoeojqv.sHtML

[U112] JS：字符串补位
来源：http://mobile.tarul.cn/Article/details/goylenewv.sHtML

"7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gfbpqtfpo.sHtML

[U113] JS：正则替换全部
来源：http://baike.bbcook.cn/Article/details/gzhndtjfl.sHtML

s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gpgaijtki.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fktsv.cn/Article/details/goqrqhqga.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.bbcook.cn/Article/details/gqpceanxe.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.vehdjk.com/Article/details/gzaxymnln.sHtML

crypto.randomUUID()
来源：http://3g.epnwcf.com/Article/details/gabbubtyc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.epnwcf.com/Article/details/gdjykbjfa.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fktsv.cn/Article/details/gthuannuc.sHtML

[U117] JS：单元测试
来源：http://m.share.bbcook.cn/Article/details/gwmckobrq.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.tarul.cn/Article/details/gecrwhwvv.sHtML

[U118] JS：开发服务器
来源：http://www.blog.epnwcf.com/Article/details/gbqzdfnyv.sHtML

npm i -D vite;  npx vite
来源：http://wap.bbcook.cn/Article/details/gohxbyxcv.sHtML

[U119] JS：生产构建
来源：http://baike.epnwcf.com/Article/details/gmsuaqref.sHtML

npx vite build
来源：http://wap.tarul.cn/Article/details/gheumjicz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.vehdjk.com/Article/details/gfmjgbvle.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.vehdjk.com/Article/details/gxaigucyo.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gzomqghpj.sHtML

统计汇总
来源：http://mobile.tarul.cn/Article/details/gzrkiyaze.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ghdnqaihr.sHtML

按语言统计（条）：
来源：http://3g.vehdjk.com/Article/details/giqlwgulf.sHtML

Python ......... 252
来源：http://baike.vehdjk.com/Article/details/gtlrjqulf.sHtML

PHP ............ 252
来源：http://www.blog.bbcook.cn/Article/details/getyxozip.sHtML

JavaScript ..... 252
来源：http://www.m.share.fktsv.cn/Article/details/gadclfiov.sHtML

TypeScript ..... 212
来源：http://3g.fktsv.cn/Article/details/gjxezqtxe.sHtML

Java ........... 212
来源：http://3g.sjlbkw.cn/Article/details/gtvmvzosn.sHtML

Go ............. 212
来源：http://mobile.sjlbkw.cn/Article/details/gtdrgkjdl.sHtML

Ruby ........... 212
来源：http://read.share.epnwcf.com/Article/details/goittxmva.sHtML

C# ............. 212
来源：http://read.share.bbcook.cn/Article/details/ggmlixchz.sHtML

C .............. 30
来源：http://blog.tarul.cn/Article/details/gvlqwbuph.sHtML

C++ ............ 30
来源：http://mobile.vehdjk.com/Article/details/gyvpchzzm.sHtML

SQL ............ 90
来源：http://www.blog.fktsv.cn/Article/details/gfbolzhqm.sHtML

Bash ........... 80
来源：http://m.share.bbcook.cn/Article/details/gvdqujmzx.sHtML

Kotlin ......... 15
来源：http://www.share.bbcook.cn/Article/details/gajchcmzs.sHtML

Swift .......... 15
来源：http://www.share.epnwcf.com/Article/details/glekmdlpa.sHtML

Lua ............ 10
来源：http://3g.epnwcf.com/Article/details/gpgdlvyhg.sHtML

Perl ........... 10
来源：http://www.share.epnwcf.com/Article/details/gihapvstq.sHtML

Scala .......... 10
来源：http://mobile.bbcook.cn/Article/details/glpvrzvan.sHtML

------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gndogdnek.sHtML

合计 ........... 2106 条
来源：http://www.m.share.vehdjk.com/Article/details/gkhdldzli.sHtML

按章节统计：
来源：http://wap.vehdjk.com/Article/details/gacjczgvw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.bbcook.cn/Article/details/gswahykzg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.sjlbkw.cn/Article/details/gbhxsgxev.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.bbcook.cn/Article/details/gzjaczlss.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.epnwcf.com/Article/details/gtwixbtse.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.tarul.cn/Article/details/gyaitzksu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.vehdjk.com/Article/details/gowoxhiku.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.sjlbkw.cn/Article/details/gwahgqtva.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.yfazqb.com/Article/details/gbamqgvjx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gdszsinfo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fktsv.cn/Article/details/gujjfgiua.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.bbcook.cn/Article/details/gjxrbgiwc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/genjidazx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/gfokvvpyk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.bbcook.cn/Article/details/gnvjtjjhb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.vehdjk.com/Article/details/gdaabymci.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/gsctqxkle.sHtML

Q SQL 专题                              90
来源：http://baike.yfazqb.com/Article/details/gfqzrwcpb.sHtML

R Bash 专题                             80
来源：http://mobile.epnwcf.com/Article/details/geuhdshcb.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.epnwcf.com/Article/details/ggzvxyynz.sHtML

T 其他语言补充                          60
来源：http://mobile.fktsv.cn/Article/details/gotmwcjxy.sHtML

U 高频实用片段                         120
来源：http://3g.vehdjk.com/Article/details/gawumqbti.sHtML

------------------------------------
来源：http://www.share.vehdjk.com/Article/details/gklflobcm.sHtML

合计                                  2106 条
来源：http://www.blog.epnwcf.com/Article/details/gnghuwlla.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.vehdjk.com/Article/details/grmllsyse.sHtML

使用提醒
来源：http://wap.vehdjk.com/Article/details/gmuxhxkkj.sHtML

--------------------------------------------------------------------------------
来源：http://wap.tarul.cn/Article/details/gyhgishfv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.yfazqb.com/Article/details/gtoqcykgh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.vehdjk.com/Article/details/gjxyjpobs.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.yfazqb.com/Article/details/gjnbaiqgf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.sjlbkw.cn/Article/details/ggdbhbijr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.tarul.cn/Article/details/gjlxwkkfm.sHtML

—— 文件结束 ——
来源：http://mobile.yfazqb.com/Article/details/gyvmaxfik.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gifbmnoxw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.tarul.cn/Article/details/gjalpcqtr.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fktsv.cn/Article/details/ghucqqkrl.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gqsfwgjuv.sHtML

【收录内容】
来源：http://baike.epnwcf.com/Article/details/gantfryue.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.vehdjk.com/Article/details/gxtvjoxsn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.yfazqb.com/Article/details/gwudakzbs.sHtML

SQL · Bash · C · C++
来源：http://baike.tarul.cn/Article/details/gwseyczxu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.yfazqb.com/Article/details/gqavhproc.sHtML

【使用说明】
来源：http://baike.vehdjk.com/Article/details/gcndvnvsg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.epnwcf.com/Article/details/gpmubpwqt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.bbcook.cn/Article/details/gvbsdvjdz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.yfazqb.com/Article/details/guknnwnha.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fktsv.cn/Article/details/ggrnoewgq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.sjlbkw.cn/Article/details/gvfobfhwc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.epnwcf.com/Article/details/gyjjkvctw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.epnwcf.com/Article/details/gmesjuzmr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fktsv.cn/Article/details/gmkyntxku.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.epnwcf.com/Article/details/gtynreseu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.bbcook.cn/Article/details/gnllhbasu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.sjlbkw.cn/Article/details/ghljvjufs.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.epnwcf.com/Article/details/gqxlhgnrp.sHtML

【文件统计】
来源：http://www.m.share.tarul.cn/Article/details/goqlvuizl.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.vehdjk.com/Article/details/gpwoxrnmo.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.tarul.cn/Article/details/gpnaegkrm.sHtML

目  录
来源：http://blog.sjlbkw.cn/Article/details/gmpyoeott.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/ggwczqpnb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.epnwcf.com/Article/details/gzxgeqzwg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.epnwcf.com/Article/details/gxlcgajgv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.yfazqb.com/Article/details/gydzgojce.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.yfazqb.com/Article/details/gcpgxljms.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.yfazqb.com/Article/details/gcpdrnzqb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fktsv.cn/Article/details/gmubshxoa.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.tarul.cn/Article/details/gzomigmnx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fktsv.cn/Article/details/gvwizbspv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.vehdjk.com/Article/details/gsiexmnng.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.tarul.cn/Article/details/gygigieff.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/gqodmaoyn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.epnwcf.com/Article/details/ggzbmmqxc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gqnxzfytc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.tarul.cn/Article/details/gzimqeqqf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.vehdjk.com/Article/details/gyfxalsrt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.tarul.cn/Article/details/gcupdgskq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.vehdjk.com/Article/details/gqpnroklt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.bbcook.cn/Article/details/gpxazsqqq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fktsv.cn/Article/details/gxvxgsevj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fktsv.cn/Article/details/grwlukuwu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.bbcook.cn/Article/details/gerctfixl.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gktbelxcb.sHtML

A. 基础语法与类型
来源：http://www.blog.tarul.cn/Article/details/gcfgayztu.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gmsobnosi.sHtML

[A01] Hello World
来源：http://wap.sjlbkw.cn/Article/details/gnphgzhtw.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.yfazqb.com/Article/details/gfybjcxss.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.vehdjk.com/Article/details/gzxaggykv.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.vehdjk.com/Article/details/gcglzkgzq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.yfazqb.com/Article/details/gtqcdnjoz.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.tarul.cn/Article/details/gntchgvxs.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.sjlbkw.cn/Article/details/gmmlmjrqg.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.vehdjk.com/Article/details/gbpfnjxak.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.bbcook.cn/Article/details/gdqrvxczr.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fktsv.cn/Article/details/geetkgwcm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.vehdjk.com/Article/details/grkwpmjty.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.bbcook.cn/Article/details/gatblsqoa.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.yfazqb.com/Article/details/gimvawbme.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fktsv.cn/Article/details/gufnboowi.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.bbcook.cn/Article/details/gfzxybolq.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.yfazqb.com/Article/details/gieabrbtn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.bbcook.cn/Article/details/gzfrakmmb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.yfazqb.com/Article/details/ghpahcofn.sHtML

[A03] 常量定义
来源：http://www.blog.sjlbkw.cn/Article/details/gfahofwlp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.epnwcf.com/Article/details/gexkuftvl.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/grnduatad.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gmtcabxke.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.bbcook.cn/Article/details/ghwlexigs.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gklbzrdvv.sHtML

Go:   const PI = 3.14159
来源：http://m.share.yfazqb.com/Article/details/gkuwlfwbv.sHtML

Ruby: PI = 3.14159
来源：http://www.share.vehdjk.com/Article/details/gxhwuppnk.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/gpgewuhfy.sHtML

[A04] 判断变量类型
来源：http://www.share.tarul.cn/Article/details/gmdgsbxjd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fktsv.cn/Article/details/gntxyfmap.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.yfazqb.com/Article/details/gbjyjaddn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.bbcook.cn/Article/details/gbxzhnapu.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.tarul.cn/Article/details/gwokosivk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.epnwcf.com/Article/details/gvgzgbmmy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fktsv.cn/Article/details/gmetjyvvu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.tarul.cn/Article/details/gyysbogxy.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.yfazqb.com/Article/details/grgyxofib.sHtML

[A05] 整数除法与取模
来源：http://blog.tarul.cn/Article/details/gampmzkks.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.epnwcf.com/Article/details/gvzxdpjcv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gceadtzzn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gdkujypww.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fktsv.cn/Article/details/gvunlfmov.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.yfazqb.com/Article/details/gxkkoflao.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.epnwcf.com/Article/details/gqrmisvpm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.yfazqb.com/Article/details/gybefgwqe.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/ghytplygc.sHtML

[A06] 字符串转数字
来源：http://www.blog.sjlbkw.cn/Article/details/gchfngndk.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.bbcook.cn/Article/details/gqcttdbth.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fktsv.cn/Article/details/glzhtzpjn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.bbcook.cn/Article/details/gmdutejeb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.epnwcf.com/Article/details/gfkythrjv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.epnwcf.com/Article/details/grnbscnrv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.tarul.cn/Article/details/gbfsntbnw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.epnwcf.com/Article/details/grhvtwism.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.epnwcf.com/Article/details/gdyhyzxgt.sHtML

[A07] 数字转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gpmaiishl.sHtML

Py:   str(42)
来源：http://wap.sjlbkw.cn/Article/details/gtcrabduu.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fktsv.cn/Article/details/gbtrfwqnk.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fktsv.cn/Article/details/gandzvsck.sHtML

TS:   String(42)
来源：http://wap.epnwcf.com/Article/details/ghdenrsnc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.bbcook.cn/Article/details/grsvwtnhf.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.sjlbkw.cn/Article/details/goqwugrja.sHtML

Ruby: 42.to_s
来源：http://wap.epnwcf.com/Article/details/gwnzdttin.sHtML

C#:   42.ToString()
来源：http://www.m.share.yfazqb.com/Article/details/ghyuvbacl.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.epnwcf.com/Article/details/gwedrrlvw.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.vehdjk.com/Article/details/gdjdsgvfj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.tarul.cn/Article/details/gvgbrzxdd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/gecmgsmha.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.tarul.cn/Article/details/greqtvcxz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.bbcook.cn/Article/details/grvaxvkws.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.sjlbkw.cn/Article/details/gafpvjtgg.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.epnwcf.com/Article/details/gjnofrokw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.tarul.cn/Article/details/gnwpjsbel.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.vehdjk.com/Article/details/gbborwvte.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gabhkgxfe.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gfrlobakw.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.vehdjk.com/Article/details/gwwembagk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gslelslfj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.epnwcf.com/Article/details/gewwwkqeb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.bbcook.cn/Article/details/gffshguud.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.vehdjk.com/Article/details/gkbvdjyzz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.yfazqb.com/Article/details/ghtajgqis.sHtML

[A10] 生成随机数
来源：http://mobile.yfazqb.com/Article/details/gojkbpwlz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.epnwcf.com/Article/details/gxphhrxmi.sHtML

PHP:  random_int(1, 100);
来源：http://wap.bbcook.cn/Article/details/gephqduab.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.yfazqb.com/Article/details/gpuifhull.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.tarul.cn/Article/details/gnzsscvrf.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.fktsv.cn/Article/details/gxncjppni.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.bbcook.cn/Article/details/gsxxhubtx.sHtML

Ruby: rand(1..100)
来源：http://read.share.yfazqb.com/Article/details/guxdlphkq.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fktsv.cn/Article/details/gvqdgopny.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.tarul.cn/Article/details/ggakavftu.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.vehdjk.com/Article/details/gexvclyhy.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.bbcook.cn/Article/details/gbmqyrtub.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.sjlbkw.cn/Article/details/getozqhhg.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.vehdjk.com/Article/details/giulwqdna.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.sjlbkw.cn/Article/details/gmteefngf.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.yfazqb.com/Article/details/gbiicixke.sHtML


<!-- 参考信息 -->