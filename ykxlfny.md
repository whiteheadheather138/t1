代发 wailian999

[U79] PHP：静态分析
来源：http://www.m.share.fktsv.cn/Article/details/gxdmdqpmi.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.bbcook.cn/Article/details/gculpzhsh.sHtML

[U80] PHP：代码规范修复
来源：http://blog.bbcook.cn/Article/details/gugptfhdb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fktsv.cn/Article/details/gylyeurpm.sHtML

[U81] JS：初始化项目
来源：http://www.blog.vehdjk.com/Article/details/gqbwptlca.sHtML

npm init -y;  npm i express
来源：http://www.blog.fktsv.cn/Article/details/gshehszza.sHtML

[U82] JS：package.json 脚本
来源：http://3g.vehdjk.com/Article/details/gannvditf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.tarul.cn/Article/details/gagvsywqi.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.vehdjk.com/Article/details/gncaexjeg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.vehdjk.com/Article/details/gajgjkrrk.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.yfazqb.com/Article/details/geschdpze.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.tarul.cn/Article/details/gvsoxjuqz.sHtML

[U85] JS：可选链
来源：http://baike.tarul.cn/Article/details/gqpyxhzhw.sHtML

a?.b?.c
来源：http://mobile.bbcook.cn/Article/details/guudtvgbm.sHtML

[U86] JS：空值合并
来源：http://baike.tarul.cn/Article/details/gstrjolty.sHtML

a ?? b
来源：http://m.share.vehdjk.com/Article/details/gbedsxzfj.sHtML

[U87] JS：解构默认值
来源：http://m.share.yfazqb.com/Article/details/goombgymx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.bbcook.cn/Article/details/grahwgqvp.sHtML

[U88] JS：对象展开合并
来源：http://read.share.yfazqb.com/Article/details/goexhcrfr.sHtML

{ ...a, ...b }
来源：http://mobile.epnwcf.com/Article/details/gebzhtdvf.sHtML

[U89] JS：数组去重
来源：http://read.share.bbcook.cn/Article/details/ghauovlya.sHtML

[...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/ggsljismj.sHtML

[U90] JS：数字数组排序
来源：http://baike.epnwcf.com/Article/details/gsrdexjxm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gpmhmfhes.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.yfazqb.com/Article/details/gwfivbfbf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.epnwcf.com/Article/details/glwtulsdf.sHtML

[U92] JS：深拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gboroiwfu.sHtML

structuredClone(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gwtncfjhl.sHtML

[U93] JS：模板字符串
来源：http://wap.bbcook.cn/Article/details/gqyhgvdym.sHtML

`共 ${n} 条`
来源：http://m.share.sjlbkw.cn/Article/details/gksnopycd.sHtML

[U94] JS：箭头函数
来源：http://3g.epnwcf.com/Article/details/gudvufcqx.sHtML

const double = x => x * 2;
来源：http://www.blog.fktsv.cn/Article/details/gublxdilr.sHtML

[U95] JS：Promise 包装
来源：http://m.share.epnwcf.com/Article/details/gneucqplk.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.tarul.cn/Article/details/gglmnpepf.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.bbcook.cn/Article/details/guyaujsul.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/gektqwxpj.sHtML

[U97] JS：并发请求
来源：http://wap.epnwcf.com/Article/details/gcvisnqwf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gonpxawjl.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.sjlbkw.cn/Article/details/gfjfwuoux.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.sjlbkw.cn/Article/details/gmglxxsjh.sHtML

[U99] JS：事件监听
来源：http://mobile.epnwcf.com/Article/details/gyttrqtkt.sHtML

el.addEventListener("click", e => {})
来源：http://blog.bbcook.cn/Article/details/guoqzwwah.sHtML

[U100] JS：DOM 查询
来源：http://mobile.bbcook.cn/Article/details/gmktrtapv.sHtML

document.querySelector(".item")
来源：http://m.share.fktsv.cn/Article/details/glugjthvh.sHtML

[U101] JS：classList 操作
来源：http://wap.bbcook.cn/Article/details/gryyngsuq.sHtML

el.classList.toggle("active")
来源：http://mobile.bbcook.cn/Article/details/gxnubfrct.sHtML

[U102] JS：本地存储
来源：http://mobile.fktsv.cn/Article/details/gusvzlzvf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.bbcook.cn/Article/details/gqxdsdupg.sHtML

[U103] JS：定时器
来源：http://mobile.vehdjk.com/Article/details/gnctsbxja.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.vehdjk.com/Article/details/gmeeecuqy.sHtML

[U104] JS：防抖
来源：http://www.blog.bbcook.cn/Article/details/gyepgmuwb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/gujbgmzoa.sHtML

[U105] JS：节流
来源：http://3g.epnwcf.com/Article/details/gxxawvola.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fktsv.cn/Article/details/giqzvsuyg.sHtML

[U106] JS：日期格式化
来源：http://wap.bbcook.cn/Article/details/gurlrrdat.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fktsv.cn/Article/details/gsjbjdett.sHtML

[U107] JS：数字千分位
来源：http://wap.sjlbkw.cn/Article/details/gdhgunxkc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.epnwcf.com/Article/details/girarvlvb.sHtML

[U108] JS：随机整数
来源：http://www.share.epnwcf.com/Article/details/gtkowcoob.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.sjlbkw.cn/Article/details/gfcvpbfmz.sHtML

[U109] JS：数组分组
来源：http://www.m.share.tarul.cn/Article/details/gbwrojsrz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.bbcook.cn/Article/details/gzuppzpfq.sHtML

[U110] JS：数组分块
来源：http://www.m.share.sjlbkw.cn/Article/details/gztgytvyf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.bbcook.cn/Article/details/gemdbfwsf.sHtML

[U111] JS：对象转 Map
来源：http://wap.sjlbkw.cn/Article/details/gtiuxyhxd.sHtML

new Map(Object.entries(obj))
来源：http://read.share.epnwcf.com/Article/details/grpqygkym.sHtML

[U112] JS：字符串补位
来源：http://read.share.vehdjk.com/Article/details/gpapbxnwg.sHtML

"7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gegouzbts.sHtML

[U113] JS：正则替换全部
来源：http://blog.yfazqb.com/Article/details/ghmihlmoq.sHtML

s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gnzyzoyej.sHtML

[U114] JS：JSON 深比较
来源：http://blog.sjlbkw.cn/Article/details/gquerptgv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.epnwcf.com/Article/details/gfxybbwhk.sHtML

[U115] JS：生成 UUID
来源：http://blog.tarul.cn/Article/details/ggxylqowg.sHtML

crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gxvjignzm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.sjlbkw.cn/Article/details/guslgccsy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.vehdjk.com/Article/details/grskpjyjd.sHtML

[U117] JS：单元测试
来源：http://www.share.tarul.cn/Article/details/gcfebolvf.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.yfazqb.com/Article/details/gvfcdfuao.sHtML

[U118] JS：开发服务器
来源：http://read.share.vehdjk.com/Article/details/gssqmqkqb.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fktsv.cn/Article/details/gbroldjmo.sHtML

[U119] JS：生产构建
来源：http://3g.epnwcf.com/Article/details/gcsucupar.sHtML

npx vite build
来源：http://blog.fktsv.cn/Article/details/gfxzewxaf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.bbcook.cn/Article/details/gledchxjl.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.sjlbkw.cn/Article/details/gegrvnaxr.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gcurpryps.sHtML

统计汇总
来源：http://3g.tarul.cn/Article/details/gyxxetjro.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gvpuzrquh.sHtML

按语言统计（条）：
来源：http://www.blog.vehdjk.com/Article/details/guqifksrg.sHtML

Python ......... 252
来源：http://www.blog.vehdjk.com/Article/details/ggwqjcolw.sHtML

PHP ............ 252
来源：http://www.m.share.tarul.cn/Article/details/gaubdclkt.sHtML

JavaScript ..... 252
来源：http://mobile.yfazqb.com/Article/details/gejemqdvm.sHtML

TypeScript ..... 212
来源：http://www.m.share.yfazqb.com/Article/details/gpnxgdouo.sHtML

Java ........... 212
来源：http://m.share.yfazqb.com/Article/details/gguczjqul.sHtML

Go ............. 212
来源：http://mobile.fktsv.cn/Article/details/gjqannisa.sHtML

Ruby ........... 212
来源：http://m.share.tarul.cn/Article/details/gowbsnzzq.sHtML

C# ............. 212
来源：http://www.share.fktsv.cn/Article/details/gsnvltryf.sHtML

C .............. 30
来源：http://read.share.tarul.cn/Article/details/gnyweqckf.sHtML

C++ ............ 30
来源：http://blog.vehdjk.com/Article/details/gcmunoouy.sHtML

SQL ............ 90
来源：http://www.blog.epnwcf.com/Article/details/gwkxlytfa.sHtML

Bash ........... 80
来源：http://www.share.fktsv.cn/Article/details/guafzoqyr.sHtML

Kotlin ......... 15
来源：http://mobile.yfazqb.com/Article/details/guszjwxjr.sHtML

Swift .......... 15
来源：http://mobile.tarul.cn/Article/details/gdfbrkwhq.sHtML

Lua ............ 10
来源：http://baike.fktsv.cn/Article/details/guazuoulk.sHtML

Perl ........... 10
来源：http://blog.fktsv.cn/Article/details/gjcyxonej.sHtML

Scala .......... 10
来源：http://www.blog.sjlbkw.cn/Article/details/gvilyrlgh.sHtML

------------------------------------
来源：http://3g.tarul.cn/Article/details/gjtvczfre.sHtML

合计 ........... 2106 条
来源：http://www.m.share.tarul.cn/Article/details/gphzuvqlu.sHtML

按章节统计：
来源：http://www.m.share.yfazqb.com/Article/details/gkdgxwrfd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.bbcook.cn/Article/details/givsgwjya.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.sjlbkw.cn/Article/details/gphmbmzzz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.sjlbkw.cn/Article/details/glzzsgsne.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.vehdjk.com/Article/details/gpgdukpnm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.tarul.cn/Article/details/gcdqomdxm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.epnwcf.com/Article/details/gsxvjwapf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.epnwcf.com/Article/details/gbmigsktl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fktsv.cn/Article/details/gxggkfeuj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gkyshbjfh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.vehdjk.com/Article/details/gncyhaxbz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/gcpfambhj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/gnlphfwwv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/grqrwykps.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.tarul.cn/Article/details/gielhxeyn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.sjlbkw.cn/Article/details/gytxbwemv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gjaqsjlmu.sHtML

Q SQL 专题                              90
来源：http://blog.epnwcf.com/Article/details/gfasbmetp.sHtML

R Bash 专题                             80
来源：http://read.share.epnwcf.com/Article/details/gkqsuiviq.sHtML

S C / C++ 专题                          60
来源：http://blog.fktsv.cn/Article/details/gyeipopzl.sHtML

T 其他语言补充                          60
来源：http://m.share.fktsv.cn/Article/details/gljxihfld.sHtML

U 高频实用片段                         120
来源：http://blog.tarul.cn/Article/details/gntctiqqz.sHtML

------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gdutogqfw.sHtML

合计                                  2106 条
来源：http://www.share.bbcook.cn/Article/details/giwaozuub.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/grclyesvg.sHtML

使用提醒
来源：http://www.blog.fktsv.cn/Article/details/gqzrujyav.sHtML

--------------------------------------------------------------------------------
来源：http://wap.yfazqb.com/Article/details/gtcllazgx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.sjlbkw.cn/Article/details/gxjtbznvt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.epnwcf.com/Article/details/gauvfzneo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.epnwcf.com/Article/details/gqpewolrz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.tarul.cn/Article/details/grmtvutxo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.yfazqb.com/Article/details/gqyingofp.sHtML

—— 文件结束 ——
来源：http://mobile.fktsv.cn/Article/details/gshlngheu.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gykeujlwk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.bbcook.cn/Article/details/ghejosuad.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.tarul.cn/Article/details/guuejtzwn.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gkwpjoaxj.sHtML

【收录内容】
来源：http://wap.fktsv.cn/Article/details/gmxhqyinx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.epnwcf.com/Article/details/gkvywebsl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.sjlbkw.cn/Article/details/gydlejwux.sHtML

SQL · Bash · C · C++
来源：http://read.share.yfazqb.com/Article/details/gbxvoiajj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.tarul.cn/Article/details/gvhhdzokd.sHtML

【使用说明】
来源：http://wap.fktsv.cn/Article/details/gqnunlrdw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.tarul.cn/Article/details/gcnhluiqx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.yfazqb.com/Article/details/gyihkxtms.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.sjlbkw.cn/Article/details/gonmdizbq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fktsv.cn/Article/details/gulqektml.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.bbcook.cn/Article/details/gzggmcjda.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.tarul.cn/Article/details/grnvwyhqb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.epnwcf.com/Article/details/gewgynoxa.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.bbcook.cn/Article/details/ggxeduofw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.bbcook.cn/Article/details/gvfdkextb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.vehdjk.com/Article/details/gmwwwvufj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.sjlbkw.cn/Article/details/guikkgutd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.epnwcf.com/Article/details/gnxscdaip.sHtML

【文件统计】
来源：http://wap.yfazqb.com/Article/details/grxzkjdfn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.sjlbkw.cn/Article/details/guvhvsucr.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gkrdtimxp.sHtML

目  录
来源：http://www.m.share.epnwcf.com/Article/details/gdhhvmrdh.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/gzpruwipi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fktsv.cn/Article/details/gucwcrpjb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.bbcook.cn/Article/details/grshqlneu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.epnwcf.com/Article/details/gbmxbpdzd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.sjlbkw.cn/Article/details/gzzlqvwhq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.yfazqb.com/Article/details/genqrracb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.bbcook.cn/Article/details/gioztydyr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.vehdjk.com/Article/details/ghsmlxxvt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.vehdjk.com/Article/details/ggmkjxque.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.tarul.cn/Article/details/gqbfgyyvr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.vehdjk.com/Article/details/gqmaovmbm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/gvcetiugg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/gevaniwog.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/gawrnsobs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.vehdjk.com/Article/details/goksprdei.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.sjlbkw.cn/Article/details/gvjnfyhyr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.vehdjk.com/Article/details/gneefeuxr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.tarul.cn/Article/details/gddevzins.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.tarul.cn/Article/details/gjrwsgbmw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.epnwcf.com/Article/details/gekxklidx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.tarul.cn/Article/details/givmyeavm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.yfazqb.com/Article/details/gedajzkuc.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gvmjtnuqf.sHtML

A. 基础语法与类型
来源：http://www.blog.tarul.cn/Article/details/gzkpnidsk.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gegxvcppx.sHtML

[A01] Hello World
来源：http://wap.vehdjk.com/Article/details/gigwjrdjm.sHtML

Py:   print("Hello, World!")
来源：http://3g.vehdjk.com/Article/details/gatpveayx.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.yfazqb.com/Article/details/gxoeefbnq.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fktsv.cn/Article/details/gomstcwlu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.yfazqb.com/Article/details/gfcmilhrd.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.epnwcf.com/Article/details/gpoiuglvo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.sjlbkw.cn/Article/details/ggkfavamw.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.yfazqb.com/Article/details/gnjiwdxzc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.bbcook.cn/Article/details/gymszflfv.sHtML

[A02] 变量声明与赋值
来源：http://wap.sjlbkw.cn/Article/details/grszqhfwi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.yfazqb.com/Article/details/gmqtlmoay.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.vehdjk.com/Article/details/gsxjdynfi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.sjlbkw.cn/Article/details/gkipxstbc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.epnwcf.com/Article/details/gmxwadroh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.epnwcf.com/Article/details/gixzjytqe.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.bbcook.cn/Article/details/gijhidgwn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.sjlbkw.cn/Article/details/glaqgcfwr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.bbcook.cn/Article/details/gzsygiylq.sHtML

[A03] 常量定义
来源：http://3g.sjlbkw.cn/Article/details/gzhxyfrjg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.epnwcf.com/Article/details/gvibxnkbk.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/geoaonhdy.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gkospkjqp.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.yfazqb.com/Article/details/ghoxdpnjg.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gvbaogoat.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.yfazqb.com/Article/details/gcfvmuhuc.sHtML

Ruby: PI = 3.14159
来源：http://read.share.epnwcf.com/Article/details/gxqtqelcg.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gctehihkq.sHtML

[A04] 判断变量类型
来源：http://wap.yfazqb.com/Article/details/gocimzxel.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.tarul.cn/Article/details/gkvkopghn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.epnwcf.com/Article/details/gslaujeda.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.bbcook.cn/Article/details/gydjewopd.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.sjlbkw.cn/Article/details/gxkupzxet.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.epnwcf.com/Article/details/gzpovouwl.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.epnwcf.com/Article/details/gaazaotdi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fktsv.cn/Article/details/gqwszzpxe.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.bbcook.cn/Article/details/gwaliwjmn.sHtML

[A05] 整数除法与取模
来源：http://mobile.vehdjk.com/Article/details/gelducqsn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.bbcook.cn/Article/details/gfpvarmwd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fktsv.cn/Article/details/ggbbboiiz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.yfazqb.com/Article/details/gjvyjqrzb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.yfazqb.com/Article/details/gddlyffch.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.bbcook.cn/Article/details/gruhzmgbs.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.tarul.cn/Article/details/grkkzelfx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.vehdjk.com/Article/details/gxhghnwtw.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.bbcook.cn/Article/details/gcgihpbgd.sHtML

[A06] 字符串转数字
来源：http://wap.vehdjk.com/Article/details/giygkkyjq.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.yfazqb.com/Article/details/glziuwpfp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.bbcook.cn/Article/details/gwzpjeasv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.sjlbkw.cn/Article/details/gxqrhgjgv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.yfazqb.com/Article/details/gpjqwxurz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.bbcook.cn/Article/details/gzehkxzxo.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.epnwcf.com/Article/details/ggfdvszxo.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.yfazqb.com/Article/details/gowccxqcn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.vehdjk.com/Article/details/gexwvhfdt.sHtML

[A07] 数字转字符串
来源：http://baike.tarul.cn/Article/details/gwgltsuin.sHtML

Py:   str(42)
来源：http://www.share.yfazqb.com/Article/details/ghjcajgvm.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fktsv.cn/Article/details/gnfpsxmcp.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.bbcook.cn/Article/details/gjfvsniaz.sHtML

TS:   String(42)
来源：http://blog.fktsv.cn/Article/details/gqfaojqcy.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.bbcook.cn/Article/details/glvaucitx.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.bbcook.cn/Article/details/gdezbeykp.sHtML

Ruby: 42.to_s
来源：http://3g.bbcook.cn/Article/details/gwpygfycx.sHtML

C#:   42.ToString()
来源：http://www.share.epnwcf.com/Article/details/glfajpopd.sHtML

[A08] 取整与四舍五入
来源：http://mobile.vehdjk.com/Article/details/ghciruqdb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.epnwcf.com/Article/details/gxiqmpuij.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.vehdjk.com/Article/details/gmzetukdf.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/gaxqjxfyw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.sjlbkw.cn/Article/details/gmsbiidtf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.epnwcf.com/Article/details/gzdqcztkz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/gdvuxbzem.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.epnwcf.com/Article/details/glsycaddx.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.yfazqb.com/Article/details/gvvdvihqw.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fktsv.cn/Article/details/gmgrdodrn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.epnwcf.com/Article/details/govzrxada.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.tarul.cn/Article/details/ghnntapjc.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.epnwcf.com/Article/details/gmyexcaek.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gnhnxgyga.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.tarul.cn/Article/details/gjercrkiz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.sjlbkw.cn/Article/details/gepybzkln.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.epnwcf.com/Article/details/geuiffepf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.fktsv.cn/Article/details/gpcjilksh.sHtML

[A10] 生成随机数
来源：http://read.share.bbcook.cn/Article/details/grpmubjwe.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.yfazqb.com/Article/details/gynvlqxff.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fktsv.cn/Article/details/ggsrqdcti.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.epnwcf.com/Article/details/gvcoidykb.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.tarul.cn/Article/details/gwlkycjns.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.sjlbkw.cn/Article/details/gzgulkvtk.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.yfazqb.com/Article/details/gefebynoo.sHtML

Ruby: rand(1..100)
来源：http://mobile.epnwcf.com/Article/details/gygpufuft.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.sjlbkw.cn/Article/details/gelvfjdpu.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.yfazqb.com/Article/details/gsblvnqdt.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.vehdjk.com/Article/details/glrdfjery.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.tarul.cn/Article/details/gcyyoqvlt.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.epnwcf.com/Article/details/gdjuxmhql.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.epnwcf.com/Article/details/gvdduaoax.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.yfazqb.com/Article/details/gugpxxhrk.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.tarul.cn/Article/details/gzjfviwwv.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.sjlbkw.cn/Article/details/gszznheei.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.epnwcf.com/Article/details/grarumbvq.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.tarul.cn/Article/details/grtldzgxu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.sjlbkw.cn/Article/details/grdehiqpm.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.tarul.cn/Article/details/gftnggdmd.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.epnwcf.com/Article/details/gfehobbzh.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.yfazqb.com/Article/details/gcmzlvejv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.epnwcf.com/Article/details/gdjluujnu.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.bbcook.cn/Article/details/glohzqueh.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnwunhux.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.tarul.cn/Article/details/gxldhommr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.sjlbkw.cn/Article/details/gyqyfzxed.sHtML


<!-- 参考信息 -->