代发 wailian999

[U75] PHP：依赖注入
来源：http://m.share.epnwcf.com/Article/details/gprvefmuh.sHtML

composer require psr/container
来源：http://blog.tarul.cn/Article/details/gxtqrztwh.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.yfazqb.com/Article/details/gkgsthgzt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.vehdjk.com/Article/details/gysgofvye.sHtML

[U77] PHP：模板渲染
来源：http://blog.bbcook.cn/Article/details/gycgjlypc.sHtML

composer require twig/twig
来源：http://wap.vehdjk.com/Article/details/gmbvauumy.sHtML

[U78] PHP：单元测试
来源：http://www.share.fktsv.cn/Article/details/gltajiqip.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.tarul.cn/Article/details/gkkruthuh.sHtML

[U79] PHP：静态分析
来源：http://mobile.sjlbkw.cn/Article/details/giecwpkhh.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.epnwcf.com/Article/details/gmolpbcvn.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.sjlbkw.cn/Article/details/gugqbthbr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fktsv.cn/Article/details/gvtsztxjm.sHtML

[U81] JS：初始化项目
来源：http://read.share.yfazqb.com/Article/details/gcvbsjojk.sHtML

npm init -y;  npm i express
来源：http://mobile.epnwcf.com/Article/details/gacaladat.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.sjlbkw.cn/Article/details/gzmihagvv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.vehdjk.com/Article/details/gzgvykryx.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.bbcook.cn/Article/details/gchnchroq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.tarul.cn/Article/details/grysfrtns.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.epnwcf.com/Article/details/gcvzoclbc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.vehdjk.com/Article/details/gmmualdak.sHtML

[U85] JS：可选链
来源：http://blog.epnwcf.com/Article/details/ggavwgzir.sHtML

a?.b?.c
来源：http://www.share.vehdjk.com/Article/details/gwgrbtiso.sHtML

[U86] JS：空值合并
来源：http://read.share.fktsv.cn/Article/details/gnphwaftb.sHtML

a ?? b
来源：http://wap.tarul.cn/Article/details/gouundpvo.sHtML

[U87] JS：解构默认值
来源：http://baike.sjlbkw.cn/Article/details/glzurzoho.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.bbcook.cn/Article/details/gbsjwbxtm.sHtML

[U88] JS：对象展开合并
来源：http://blog.tarul.cn/Article/details/gsxuxaxpz.sHtML

{ ...a, ...b }
来源：http://baike.sjlbkw.cn/Article/details/gprriyedg.sHtML

[U89] JS：数组去重
来源：http://www.blog.tarul.cn/Article/details/ggraoqnjj.sHtML

[...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/gnucdrtqa.sHtML

[U90] JS：数字数组排序
来源：http://www.share.vehdjk.com/Article/details/gmgezhbcw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gpmboofwi.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.tarul.cn/Article/details/gndfuubny.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fktsv.cn/Article/details/gegtoyzjk.sHtML

[U92] JS：深拷贝
来源：http://m.share.fktsv.cn/Article/details/gvcyibczy.sHtML

structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/grjhgjtit.sHtML

[U93] JS：模板字符串
来源：http://m.share.sjlbkw.cn/Article/details/gkoutowny.sHtML

`共 ${n} 条`
来源：http://www.blog.tarul.cn/Article/details/gofkwwphj.sHtML

[U94] JS：箭头函数
来源：http://m.share.yfazqb.com/Article/details/gjvnarvnv.sHtML

const double = x => x * 2;
来源：http://www.m.share.yfazqb.com/Article/details/gvrswxisj.sHtML

[U95] JS：Promise 包装
来源：http://www.share.sjlbkw.cn/Article/details/gnleluxrb.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.yfazqb.com/Article/details/gpsgugxyb.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.yfazqb.com/Article/details/gzudqdwrl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/gqbwifcot.sHtML

[U97] JS：并发请求
来源：http://wap.bbcook.cn/Article/details/gglrryibn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gipgjnkwx.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.sjlbkw.cn/Article/details/gvbguglmy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fktsv.cn/Article/details/gsywqgkfg.sHtML

[U99] JS：事件监听
来源：http://wap.yfazqb.com/Article/details/gawodtpis.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.sjlbkw.cn/Article/details/gknvzbabz.sHtML

[U100] JS：DOM 查询
来源：http://baike.sjlbkw.cn/Article/details/gzdfzuggk.sHtML

document.querySelector(".item")
来源：http://www.share.yfazqb.com/Article/details/gzoiwihqq.sHtML

[U101] JS：classList 操作
来源：http://mobile.yfazqb.com/Article/details/ghgkjcknn.sHtML

el.classList.toggle("active")
来源：http://m.share.vehdjk.com/Article/details/gpjcukmag.sHtML

[U102] JS：本地存储
来源：http://mobile.sjlbkw.cn/Article/details/gxtpyfguo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.sjlbkw.cn/Article/details/getsepieg.sHtML

[U103] JS：定时器
来源：http://baike.fktsv.cn/Article/details/gkzelwiju.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.vehdjk.com/Article/details/gwinfeuik.sHtML

[U104] JS：防抖
来源：http://m.share.epnwcf.com/Article/details/gytgtjbkb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fktsv.cn/Article/details/gdyqhfbuv.sHtML

[U105] JS：节流
来源：http://baike.bbcook.cn/Article/details/gjmrdeyeh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.bbcook.cn/Article/details/gztxlxpyl.sHtML

[U106] JS：日期格式化
来源：http://mobile.yfazqb.com/Article/details/gcnzamhnz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.sjlbkw.cn/Article/details/gjbbvgsoj.sHtML

[U107] JS：数字千分位
来源：http://read.share.tarul.cn/Article/details/glbntwcsu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.yfazqb.com/Article/details/gtrkcyujh.sHtML

[U108] JS：随机整数
来源：http://www.m.share.vehdjk.com/Article/details/geuiseugf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.yfazqb.com/Article/details/gpuiotsiq.sHtML

[U109] JS：数组分组
来源：http://m.share.bbcook.cn/Article/details/gvspsuufj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fktsv.cn/Article/details/grahcnoxe.sHtML

[U110] JS：数组分块
来源：http://www.blog.sjlbkw.cn/Article/details/guwjtflso.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.vehdjk.com/Article/details/guegblngg.sHtML

[U111] JS：对象转 Map
来源：http://www.share.sjlbkw.cn/Article/details/gqpzyqjtd.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fktsv.cn/Article/details/guafplyki.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.epnwcf.com/Article/details/gkcqjyveq.sHtML

"7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gfksnpyqy.sHtML

[U113] JS：正则替换全部
来源：http://wap.tarul.cn/Article/details/goevbyqvc.sHtML

s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gdluhkutq.sHtML

[U114] JS：JSON 深比较
来源：http://baike.bbcook.cn/Article/details/gatzvyoxq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/glpgukuvs.sHtML

[U115] JS：生成 UUID
来源：http://3g.yfazqb.com/Article/details/gfgpmuzah.sHtML

crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/glzbktcdy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.epnwcf.com/Article/details/grsnacjbk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.epnwcf.com/Article/details/gagbedcot.sHtML

[U117] JS：单元测试
来源：http://read.share.sjlbkw.cn/Article/details/gvopncmxb.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.sjlbkw.cn/Article/details/gcmlawkei.sHtML

[U118] JS：开发服务器
来源：http://3g.fktsv.cn/Article/details/gfrytyqaa.sHtML

npm i -D vite;  npx vite
来源：http://read.share.sjlbkw.cn/Article/details/gebobfueg.sHtML

[U119] JS：生产构建
来源：http://baike.vehdjk.com/Article/details/gmhiifizu.sHtML

npx vite build
来源：http://3g.bbcook.cn/Article/details/gchtisbsp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.vehdjk.com/Article/details/grljcnzzs.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.sjlbkw.cn/Article/details/gaiohyunk.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxvnuqmbo.sHtML

统计汇总
来源：http://3g.tarul.cn/Article/details/giymwdypg.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gknwhmlmc.sHtML

按语言统计（条）：
来源：http://m.share.fktsv.cn/Article/details/ghzwmyhxb.sHtML

Python ......... 252
来源：http://www.share.fktsv.cn/Article/details/gygpccczv.sHtML

PHP ............ 252
来源：http://www.share.epnwcf.com/Article/details/grhczewtn.sHtML

JavaScript ..... 252
来源：http://www.share.sjlbkw.cn/Article/details/gkrfsaekh.sHtML

TypeScript ..... 212
来源：http://3g.tarul.cn/Article/details/gxbuczngq.sHtML

Java ........... 212
来源：http://blog.yfazqb.com/Article/details/garwvcmis.sHtML

Go ............. 212
来源：http://baike.tarul.cn/Article/details/gqfxxgomc.sHtML

Ruby ........... 212
来源：http://www.share.yfazqb.com/Article/details/ghohmngwp.sHtML

C# ............. 212
来源：http://wap.yfazqb.com/Article/details/gcmuyvnwk.sHtML

C .............. 30
来源：http://m.share.tarul.cn/Article/details/gzvpuibwy.sHtML

C++ ............ 30
来源：http://baike.fktsv.cn/Article/details/gkrfgphwh.sHtML

SQL ............ 90
来源：http://3g.yfazqb.com/Article/details/gdqdsdsgt.sHtML

Bash ........... 80
来源：http://baike.yfazqb.com/Article/details/glweinxdx.sHtML

Kotlin ......... 15
来源：http://mobile.sjlbkw.cn/Article/details/gkmsvhddw.sHtML

Swift .......... 15
来源：http://read.share.fktsv.cn/Article/details/gfxthomzy.sHtML

Lua ............ 10
来源：http://wap.epnwcf.com/Article/details/gegkniqyl.sHtML

Perl ........... 10
来源：http://www.blog.vehdjk.com/Article/details/glkjgylcv.sHtML

Scala .......... 10
来源：http://wap.yfazqb.com/Article/details/gmfedbxsh.sHtML

------------------------------------
来源：http://3g.fktsv.cn/Article/details/gofmwpoiw.sHtML

合计 ........... 2106 条
来源：http://m.share.vehdjk.com/Article/details/gpnxfuqhb.sHtML

按章节统计：
来源：http://wap.tarul.cn/Article/details/glctyysve.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.bbcook.cn/Article/details/godszlzxn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.yfazqb.com/Article/details/gzlicvwoq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/gllavdwxt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.sjlbkw.cn/Article/details/gkmorxezm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fktsv.cn/Article/details/gpbvjtdsq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.epnwcf.com/Article/details/gmbxxnxao.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.epnwcf.com/Article/details/gkhhwjbjl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.epnwcf.com/Article/details/gsvmkcanq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gigphdfos.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.bbcook.cn/Article/details/gwfxrhjex.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/gkjbwgyec.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/gdsoqqlkc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gmmqvlcqr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.yfazqb.com/Article/details/glwkltvcy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.tarul.cn/Article/details/gcijhdgoe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/gbwybilvb.sHtML

Q SQL 专题                              90
来源：http://baike.tarul.cn/Article/details/gqjipjsuq.sHtML

R Bash 专题                             80
来源：http://www.m.share.epnwcf.com/Article/details/gxiaeoywi.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fktsv.cn/Article/details/grpcimvpo.sHtML

T 其他语言补充                          60
来源：http://www.m.share.tarul.cn/Article/details/gdmifibpy.sHtML

U 高频实用片段                         120
来源：http://blog.sjlbkw.cn/Article/details/gyacwpsfd.sHtML

------------------------------------
来源：http://www.share.bbcook.cn/Article/details/ghscueonb.sHtML

合计                                  2106 条
来源：http://blog.bbcook.cn/Article/details/gblyvtyya.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gnztdmtfx.sHtML

使用提醒
来源：http://wap.sjlbkw.cn/Article/details/gyzzwokio.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gxyvsljae.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.epnwcf.com/Article/details/gwtooixtb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.tarul.cn/Article/details/gqyrcznjg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.vehdjk.com/Article/details/gfgfngasz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.bbcook.cn/Article/details/gqbsifpbv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.yfazqb.com/Article/details/gmqcuiuxy.sHtML

—— 文件结束 ——
来源：http://www.share.yfazqb.com/Article/details/gxdnyrpou.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gryatylsn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.vehdjk.com/Article/details/gdzjzoagd.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fktsv.cn/Article/details/gcuhvxxet.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gvtjyocxq.sHtML

【收录内容】
来源：http://baike.yfazqb.com/Article/details/grzjndfrh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.bbcook.cn/Article/details/gzeiutpjo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fktsv.cn/Article/details/gkndgkbtv.sHtML

SQL · Bash · C · C++
来源：http://m.share.sjlbkw.cn/Article/details/ghixvstfx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.tarul.cn/Article/details/gtulksuqm.sHtML

【使用说明】
来源：http://m.share.vehdjk.com/Article/details/ghsmgbkfm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fktsv.cn/Article/details/gafljwfpq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.epnwcf.com/Article/details/gzrgaxfld.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fktsv.cn/Article/details/gpccrsivm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fktsv.cn/Article/details/gddaivdfz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.epnwcf.com/Article/details/gvbfytird.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.vehdjk.com/Article/details/guoezcakm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fktsv.cn/Article/details/gsvaydett.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fktsv.cn/Article/details/gbwlexheu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.sjlbkw.cn/Article/details/gocdxbykn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fktsv.cn/Article/details/gbwflywka.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.vehdjk.com/Article/details/gfifmhldi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fktsv.cn/Article/details/gxsmaxnfp.sHtML

【文件统计】
来源：http://www.blog.tarul.cn/Article/details/gonqejomg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.sjlbkw.cn/Article/details/gcuedjsuy.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gtcbmzavs.sHtML

目  录
来源：http://www.blog.tarul.cn/Article/details/grcxvxegv.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/ghaiqnvkc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.yfazqb.com/Article/details/gllxvmnop.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.yfazqb.com/Article/details/gtlcjiixf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.bbcook.cn/Article/details/gskhhixll.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.yfazqb.com/Article/details/gsnludczx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.vehdjk.com/Article/details/gssvgbdmf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.sjlbkw.cn/Article/details/glmofrwzx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.sjlbkw.cn/Article/details/gguojgzmu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.epnwcf.com/Article/details/gxuwwswju.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/grhbihojk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.sjlbkw.cn/Article/details/gqwysjqzo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/gckpxkcyu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.bbcook.cn/Article/details/gcpnvvnlg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/gkrdektbd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.tarul.cn/Article/details/gyafwdnju.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.vehdjk.com/Article/details/gpwefudvg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.sjlbkw.cn/Article/details/gfdzgmkyn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.epnwcf.com/Article/details/gigwklctb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fktsv.cn/Article/details/gseclusyb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.bbcook.cn/Article/details/gndwnaada.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.tarul.cn/Article/details/ggxholrye.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.tarul.cn/Article/details/gjzvweuqh.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gjnrzsery.sHtML

A. 基础语法与类型
来源：http://www.blog.sjlbkw.cn/Article/details/guqlzzsjz.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gofxkzvin.sHtML

[A01] Hello World
来源：http://baike.sjlbkw.cn/Article/details/gicszsvfk.sHtML

Py:   print("Hello, World!")
来源：http://3g.sjlbkw.cn/Article/details/gbtjmbsij.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.vehdjk.com/Article/details/gphqcwrqb.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.tarul.cn/Article/details/ggsriqtrw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.yfazqb.com/Article/details/gdezktnxl.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.epnwcf.com/Article/details/gsnguffqt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.tarul.cn/Article/details/gpkzufhwx.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fktsv.cn/Article/details/gfzhchbtt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.vehdjk.com/Article/details/gxmrmyyzo.sHtML

[A02] 变量声明与赋值
来源：http://www.share.yfazqb.com/Article/details/gyyiwqjxl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.sjlbkw.cn/Article/details/gifduvwyn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fktsv.cn/Article/details/gqstnavfm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.sjlbkw.cn/Article/details/ggafqqhax.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.vehdjk.com/Article/details/gnyhfndod.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.epnwcf.com/Article/details/gpyeckkme.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fktsv.cn/Article/details/glvgkonzt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.yfazqb.com/Article/details/gnzprfgsq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.yfazqb.com/Article/details/gnckjhypq.sHtML

[A03] 常量定义
来源：http://m.share.yfazqb.com/Article/details/gwbkdsqrh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fktsv.cn/Article/details/gjimqunbj.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/glauguvqo.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gqixaqvhu.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gusbmplko.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gtszmjnay.sHtML

Go:   const PI = 3.14159
来源：http://wap.tarul.cn/Article/details/gkaiyyfzw.sHtML

Ruby: PI = 3.14159
来源：http://3g.fktsv.cn/Article/details/ggjrarhxe.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/guncblrzi.sHtML

[A04] 判断变量类型
来源：http://www.m.share.tarul.cn/Article/details/gkbgleugf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.vehdjk.com/Article/details/gvgoxhqty.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.tarul.cn/Article/details/gbemcsthg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fktsv.cn/Article/details/gjkzcfblm.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.sjlbkw.cn/Article/details/ghzltryip.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.bbcook.cn/Article/details/gcpvpvuxm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.tarul.cn/Article/details/gkxzfkmrj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.tarul.cn/Article/details/gfoqkrbon.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.yfazqb.com/Article/details/gztgghdab.sHtML

[A05] 整数除法与取模
来源：http://baike.epnwcf.com/Article/details/gsmkqzspt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.epnwcf.com/Article/details/glsmazefw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.tarul.cn/Article/details/gpoousqan.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gstsfphea.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fktsv.cn/Article/details/gybbbtkrs.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/gsdsyuran.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gqdowpwbs.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.tarul.cn/Article/details/grpxkmwdd.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.bbcook.cn/Article/details/gqfzsrufx.sHtML

[A06] 字符串转数字
来源：http://mobile.bbcook.cn/Article/details/gmitriqpe.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.epnwcf.com/Article/details/guzvicgdf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fktsv.cn/Article/details/ghzjlrqkm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.sjlbkw.cn/Article/details/gygkvvbil.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fktsv.cn/Article/details/gasqikbue.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.yfazqb.com/Article/details/gqltnzbae.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.epnwcf.com/Article/details/gvoznbhyi.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.sjlbkw.cn/Article/details/gekkxngri.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.yfazqb.com/Article/details/gdevvagnp.sHtML

[A07] 数字转字符串
来源：http://baike.fktsv.cn/Article/details/glwrtilod.sHtML

Py:   str(42)
来源：http://read.share.yfazqb.com/Article/details/gqxerbhyy.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.bbcook.cn/Article/details/gpcprkgoc.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.yfazqb.com/Article/details/gzplortds.sHtML

TS:   String(42)
来源：http://read.share.sjlbkw.cn/Article/details/gbusshtjx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.epnwcf.com/Article/details/gemxwtdet.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.yfazqb.com/Article/details/gawqeslpk.sHtML

Ruby: 42.to_s
来源：http://read.share.fktsv.cn/Article/details/gvrgymmnx.sHtML

C#:   42.ToString()
来源：http://www.blog.yfazqb.com/Article/details/gxpkjwros.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.vehdjk.com/Article/details/gokqjyiuh.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/gyccveutv.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.yfazqb.com/Article/details/germlcilb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.epnwcf.com/Article/details/gqnufifbw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.sjlbkw.cn/Article/details/gedwcmbdq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.bbcook.cn/Article/details/gmeevvtbf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.epnwcf.com/Article/details/gefifxdqk.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fktsv.cn/Article/details/gqvkgdutl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.epnwcf.com/Article/details/gzelajxzp.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fktsv.cn/Article/details/gbowfkhle.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.tarul.cn/Article/details/gndvqsafy.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.vehdjk.com/Article/details/gjdyujkfo.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.vehdjk.com/Article/details/gregesatw.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.epnwcf.com/Article/details/gcrobnpyg.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/gqhkbyktc.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.epnwcf.com/Article/details/gefoskrcu.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.yfazqb.com/Article/details/ggyypkrjq.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/glsllapoq.sHtML

[A10] 生成随机数
来源：http://m.share.sjlbkw.cn/Article/details/gsiewkkav.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.tarul.cn/Article/details/gplyeoeff.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.tarul.cn/Article/details/gabsmqrka.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.epnwcf.com/Article/details/gljskpvdv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.vehdjk.com/Article/details/ggilmlllp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.bbcook.cn/Article/details/gssxczszu.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.yfazqb.com/Article/details/gejkbvths.sHtML

Ruby: rand(1..100)
来源：http://m.share.yfazqb.com/Article/details/gjldnfxrp.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.tarul.cn/Article/details/gykqebhqk.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.tarul.cn/Article/details/ghwmvjjjb.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.vehdjk.com/Article/details/gqcxulujp.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.sjlbkw.cn/Article/details/gutqdzthf.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.epnwcf.com/Article/details/gsqpzzaoz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.fktsv.cn/Article/details/gqjkdjujw.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.sjlbkw.cn/Article/details/gfrjxyoqr.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.bbcook.cn/Article/details/gbkzfyxhk.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.epnwcf.com/Article/details/gwrtrlowl.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.bbcook.cn/Article/details/gzzxzmvuy.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.tarul.cn/Article/details/gszoujdyh.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.epnwcf.com/Article/details/gybatwfnj.sHtML


<!-- 参考信息 -->