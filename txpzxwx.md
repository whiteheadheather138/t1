代发 wailian999

[U77] PHP：模板渲染
来源：http://m.share.sjlbkw.cn/Article/details/gejojrqkw.sHtML

composer require twig/twig
来源：http://www.share.sjlbkw.cn/Article/details/gohbijwkp.sHtML

[U78] PHP：单元测试
来源：http://wap.bbcook.cn/Article/details/gjchcvavw.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.epnwcf.com/Article/details/gwzwwwulh.sHtML

[U79] PHP：静态分析
来源：http://read.share.yfazqb.com/Article/details/ghrayrllj.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.bbcook.cn/Article/details/gwcsqrvkj.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.bbcook.cn/Article/details/ggcjtrajm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.sjlbkw.cn/Article/details/glkahgxrh.sHtML

[U81] JS：初始化项目
来源：http://www.blog.sjlbkw.cn/Article/details/grqnfsoks.sHtML

npm init -y;  npm i express
来源：http://read.share.sjlbkw.cn/Article/details/gemewtjea.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.epnwcf.com/Article/details/gspmxjbxw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.epnwcf.com/Article/details/gizsliwpp.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.vehdjk.com/Article/details/gbxmrsiqs.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.bbcook.cn/Article/details/ggtintvsa.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fktsv.cn/Article/details/gmlmweynx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.yfazqb.com/Article/details/gepjnnrnk.sHtML

[U85] JS：可选链
来源：http://www.m.share.fktsv.cn/Article/details/gslbwujsm.sHtML

a?.b?.c
来源：http://blog.bbcook.cn/Article/details/gyhdxvujl.sHtML

[U86] JS：空值合并
来源：http://m.share.fktsv.cn/Article/details/gmamccjou.sHtML

a ?? b
来源：http://read.share.bbcook.cn/Article/details/gkgxdpuao.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fktsv.cn/Article/details/guostpfem.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.epnwcf.com/Article/details/gsamwgfgy.sHtML

[U88] JS：对象展开合并
来源：http://www.share.epnwcf.com/Article/details/ggwvywfyw.sHtML

{ ...a, ...b }
来源：http://read.share.yfazqb.com/Article/details/gnjzxjsvt.sHtML

[U89] JS：数组去重
来源：http://m.share.vehdjk.com/Article/details/gqrsksrem.sHtML

[...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gangoxrnl.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fktsv.cn/Article/details/gexyihowd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gukghhtlm.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.bbcook.cn/Article/details/gieubnnnm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.yfazqb.com/Article/details/goigkyzfp.sHtML

[U92] JS：深拷贝
来源：http://read.share.tarul.cn/Article/details/gaxyzhubd.sHtML

structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/gqufoyerm.sHtML

[U93] JS：模板字符串
来源：http://www.share.yfazqb.com/Article/details/ghrqpotod.sHtML

`共 ${n} 条`
来源：http://www.blog.fktsv.cn/Article/details/garcpmdks.sHtML

[U94] JS：箭头函数
来源：http://3g.tarul.cn/Article/details/gmwflegkc.sHtML

const double = x => x * 2;
来源：http://baike.vehdjk.com/Article/details/gvdcuisvr.sHtML

[U95] JS：Promise 包装
来源：http://blog.sjlbkw.cn/Article/details/gxblrdvtd.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.bbcook.cn/Article/details/gjtoufech.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.tarul.cn/Article/details/gfiqaakdd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gfrfxzhvj.sHtML

[U97] JS：并发请求
来源：http://baike.yfazqb.com/Article/details/ghdpelfxv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gdozpwlxq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.vehdjk.com/Article/details/gbvhbgqcp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.bbcook.cn/Article/details/gczjgshgo.sHtML

[U99] JS：事件监听
来源：http://baike.yfazqb.com/Article/details/geouklksr.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.bbcook.cn/Article/details/gcspiszae.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fktsv.cn/Article/details/gadsalgvo.sHtML

document.querySelector(".item")
来源：http://baike.epnwcf.com/Article/details/ggbqlclyk.sHtML

[U101] JS：classList 操作
来源：http://mobile.epnwcf.com/Article/details/gkkjyewxs.sHtML

el.classList.toggle("active")
来源：http://m.share.sjlbkw.cn/Article/details/gnimwmude.sHtML

[U102] JS：本地存储
来源：http://read.share.bbcook.cn/Article/details/gwstqqpbg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.sjlbkw.cn/Article/details/gprmisthw.sHtML

[U103] JS：定时器
来源：http://mobile.bbcook.cn/Article/details/ggnaqepix.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.sjlbkw.cn/Article/details/ghxhuymho.sHtML

[U104] JS：防抖
来源：http://blog.tarul.cn/Article/details/gppggdmkw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/gctgxztxm.sHtML

[U105] JS：节流
来源：http://3g.tarul.cn/Article/details/gqtxcawew.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.sjlbkw.cn/Article/details/gxzjgmgyh.sHtML

[U106] JS：日期格式化
来源：http://3g.vehdjk.com/Article/details/ggaaovilg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.vehdjk.com/Article/details/grttnzxqy.sHtML

[U107] JS：数字千分位
来源：http://read.share.epnwcf.com/Article/details/gvaotfnxe.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.tarul.cn/Article/details/gudsmhmbe.sHtML

[U108] JS：随机整数
来源：http://www.m.share.tarul.cn/Article/details/gxupndftz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.yfazqb.com/Article/details/gyzzolhhb.sHtML

[U109] JS：数组分组
来源：http://wap.yfazqb.com/Article/details/gwdaadicf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fktsv.cn/Article/details/gfwiyyggl.sHtML

[U110] JS：数组分块
来源：http://www.share.sjlbkw.cn/Article/details/gljuxcoxf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fktsv.cn/Article/details/gdoyecpgy.sHtML

[U111] JS：对象转 Map
来源：http://read.share.epnwcf.com/Article/details/gllnprpar.sHtML

new Map(Object.entries(obj))
来源：http://wap.sjlbkw.cn/Article/details/gbgwkzrux.sHtML

[U112] JS：字符串补位
来源：http://read.share.bbcook.cn/Article/details/gdktyfvtg.sHtML

"7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gipzczjvz.sHtML

[U113] JS：正则替换全部
来源：http://blog.vehdjk.com/Article/details/goyvbssbt.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gyvncvypq.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.tarul.cn/Article/details/gedzhnqcu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.vehdjk.com/Article/details/gdywhnevi.sHtML

[U115] JS：生成 UUID
来源：http://baike.yfazqb.com/Article/details/goidunlzw.sHtML

crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gjdishpfg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.yfazqb.com/Article/details/gpikzwges.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fktsv.cn/Article/details/gfxssypcy.sHtML

[U117] JS：单元测试
来源：http://www.share.bbcook.cn/Article/details/gdfkkkikt.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.sjlbkw.cn/Article/details/ggzxnxcsv.sHtML

[U118] JS：开发服务器
来源：http://baike.yfazqb.com/Article/details/gpfipjnwz.sHtML

npm i -D vite;  npx vite
来源：http://read.share.bbcook.cn/Article/details/getntgqau.sHtML

[U119] JS：生产构建
来源：http://mobile.fktsv.cn/Article/details/glirbltla.sHtML

npx vite build
来源：http://baike.sjlbkw.cn/Article/details/gyzodhqug.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fktsv.cn/Article/details/gslvdands.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fktsv.cn/Article/details/gbgagwclf.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gcjbwbzrg.sHtML

统计汇总
来源：http://baike.yfazqb.com/Article/details/gethjyzav.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gxjyyrubc.sHtML

按语言统计（条）：
来源：http://mobile.bbcook.cn/Article/details/gtgbpgfoo.sHtML

Python ......... 252
来源：http://www.blog.epnwcf.com/Article/details/gprqxhgtl.sHtML

PHP ............ 252
来源：http://www.m.share.fktsv.cn/Article/details/glndoqijp.sHtML

JavaScript ..... 252
来源：http://3g.bbcook.cn/Article/details/gltcrhmpn.sHtML

TypeScript ..... 212
来源：http://read.share.yfazqb.com/Article/details/gurafgotq.sHtML

Java ........... 212
来源：http://www.blog.fktsv.cn/Article/details/gzavxtliv.sHtML

Go ............. 212
来源：http://read.share.epnwcf.com/Article/details/gpdsspdis.sHtML

Ruby ........... 212
来源：http://blog.tarul.cn/Article/details/gxmxsxrwf.sHtML

C# ............. 212
来源：http://blog.bbcook.cn/Article/details/gdzuppkcx.sHtML

C .............. 30
来源：http://www.m.share.yfazqb.com/Article/details/gpvrundhi.sHtML

C++ ............ 30
来源：http://m.share.tarul.cn/Article/details/gaswbiolm.sHtML

SQL ............ 90
来源：http://read.share.bbcook.cn/Article/details/gptqnndcq.sHtML

Bash ........... 80
来源：http://www.m.share.yfazqb.com/Article/details/gjzidekvu.sHtML

Kotlin ......... 15
来源：http://m.share.vehdjk.com/Article/details/gwvcukbdv.sHtML

Swift .......... 15
来源：http://m.share.sjlbkw.cn/Article/details/gxfoszkvg.sHtML

Lua ............ 10
来源：http://m.share.bbcook.cn/Article/details/guarlgasq.sHtML

Perl ........... 10
来源：http://www.m.share.sjlbkw.cn/Article/details/gfktsfpan.sHtML

Scala .......... 10
来源：http://blog.epnwcf.com/Article/details/gnukiippr.sHtML

------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/geyyoaqjt.sHtML

合计 ........... 2106 条
来源：http://www.share.bbcook.cn/Article/details/gqjekieus.sHtML

按章节统计：
来源：http://www.blog.bbcook.cn/Article/details/gxfflbocp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.vehdjk.com/Article/details/gqzyezpxx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.epnwcf.com/Article/details/gopoinyvz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.sjlbkw.cn/Article/details/gyasstzmf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.tarul.cn/Article/details/gpvuhftvf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fktsv.cn/Article/details/gfydiwhgo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fktsv.cn/Article/details/gsaujmsde.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.epnwcf.com/Article/details/gfhojpmif.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.epnwcf.com/Article/details/glimszlkl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/geiqatvqh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.epnwcf.com/Article/details/gbtuwyehd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/grbpvcgro.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/ghsdpycct.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/gfuwcxvvg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.epnwcf.com/Article/details/gnjqtyvgj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.sjlbkw.cn/Article/details/germofqxo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/gxxxyhqcn.sHtML

Q SQL 专题                              90
来源：http://read.share.vehdjk.com/Article/details/gsvsyknwi.sHtML

R Bash 专题                             80
来源：http://mobile.bbcook.cn/Article/details/gqgmdqmxj.sHtML

S C / C++ 专题                          60
来源：http://mobile.bbcook.cn/Article/details/guqgvlrjl.sHtML

T 其他语言补充                          60
来源：http://www.share.vehdjk.com/Article/details/gtqalzkva.sHtML

U 高频实用片段                         120
来源：http://www.blog.yfazqb.com/Article/details/gxqglhvnb.sHtML

------------------------------------
来源：http://baike.bbcook.cn/Article/details/gnpcokzhq.sHtML

合计                                  2106 条
来源：http://www.m.share.tarul.cn/Article/details/gpxqtnhag.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/glopbmbfk.sHtML

使用提醒
来源：http://www.m.share.bbcook.cn/Article/details/gvmrdxqkc.sHtML

--------------------------------------------------------------------------------
来源：http://3g.vehdjk.com/Article/details/gpsuxmmrv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.yfazqb.com/Article/details/gobgxfuth.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.tarul.cn/Article/details/gipmydzsl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.sjlbkw.cn/Article/details/gntdcckpd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.yfazqb.com/Article/details/ggljlvwrt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.vehdjk.com/Article/details/gddgcsqju.sHtML

—— 文件结束 ——
来源：http://mobile.yfazqb.com/Article/details/gmhsniibp.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gjmiqxdgv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.epnwcf.com/Article/details/gbjsljyby.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.sjlbkw.cn/Article/details/glxwplmri.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gkzogcopc.sHtML

【收录内容】
来源：http://mobile.sjlbkw.cn/Article/details/glegqelbz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fktsv.cn/Article/details/gumrekqlf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.sjlbkw.cn/Article/details/ghteotpxu.sHtML

SQL · Bash · C · C++
来源：http://www.share.bbcook.cn/Article/details/gqxtxnlyn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.sjlbkw.cn/Article/details/gboglxsud.sHtML

【使用说明】
来源：http://www.share.fktsv.cn/Article/details/gxyahsnpa.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.epnwcf.com/Article/details/glfrdlitk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.yfazqb.com/Article/details/gvnpnzrqo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fktsv.cn/Article/details/guflrlkjz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.tarul.cn/Article/details/gmvczqhoi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fktsv.cn/Article/details/gujajmfcd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fktsv.cn/Article/details/gkhernhqi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.bbcook.cn/Article/details/guiootlhk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.sjlbkw.cn/Article/details/gduvaxfgs.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.tarul.cn/Article/details/gibgxwqgp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.sjlbkw.cn/Article/details/gubosqjax.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.tarul.cn/Article/details/gsjremtgd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.tarul.cn/Article/details/gzoojlmmz.sHtML

【文件统计】
来源：http://mobile.bbcook.cn/Article/details/gvplzvucw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.sjlbkw.cn/Article/details/gkcqjctci.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gcnydwzks.sHtML

目  录
来源：http://blog.epnwcf.com/Article/details/gsixijlcf.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/ghkhgwpse.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.sjlbkw.cn/Article/details/gslkbbozr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.vehdjk.com/Article/details/gaqtggnfp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.epnwcf.com/Article/details/gezwnvabp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.epnwcf.com/Article/details/gvbdhlowt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.bbcook.cn/Article/details/gdyyjpstv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/grkidadie.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/gnzuftohg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.epnwcf.com/Article/details/gpgfquvsi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.bbcook.cn/Article/details/gsnmiesys.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.vehdjk.com/Article/details/gjzqwtieh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.sjlbkw.cn/Article/details/ganenbpdh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.vehdjk.com/Article/details/ghcossezl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.yfazqb.com/Article/details/grgqswcrr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.yfazqb.com/Article/details/gslqcpols.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.bbcook.cn/Article/details/gmdztwgdi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/gdpuhpkhg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.yfazqb.com/Article/details/gzmuxaehi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.vehdjk.com/Article/details/gjsaivgnz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.yfazqb.com/Article/details/gwpiedrmu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.vehdjk.com/Article/details/guuilkpal.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fktsv.cn/Article/details/gykceyrxo.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gzcfohsli.sHtML

A. 基础语法与类型
来源：http://wap.epnwcf.com/Article/details/gdkjujzcy.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gjctezsls.sHtML

[A01] Hello World
来源：http://wap.yfazqb.com/Article/details/gjcrujflz.sHtML

Py:   print("Hello, World!")
来源：http://m.share.sjlbkw.cn/Article/details/gmhokcbpm.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.vehdjk.com/Article/details/gjywczowb.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.yfazqb.com/Article/details/gbvazjxmp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.bbcook.cn/Article/details/gefvqphcd.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.epnwcf.com/Article/details/gtalzfjju.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.tarul.cn/Article/details/ggxqkykgz.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.tarul.cn/Article/details/geliezuvv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.epnwcf.com/Article/details/gmtemyett.sHtML

[A02] 变量声明与赋值
来源：http://m.share.vehdjk.com/Article/details/guodgiqax.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.epnwcf.com/Article/details/gcnjtoswq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.tarul.cn/Article/details/gtbvhfgll.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.vehdjk.com/Article/details/gxvsoczot.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.vehdjk.com/Article/details/gieokdijx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fktsv.cn/Article/details/gjgpatdaw.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.vehdjk.com/Article/details/gejzpgapj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.sjlbkw.cn/Article/details/gzduzfzyt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gzfuwnyvn.sHtML

[A03] 常量定义
来源：http://3g.vehdjk.com/Article/details/gmvrwakqj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.epnwcf.com/Article/details/gzhqnvmor.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gkioygrbj.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gdyaoillz.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gamfforcg.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gvyotavzi.sHtML

Go:   const PI = 3.14159
来源：http://blog.tarul.cn/Article/details/gkvcfedkw.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fktsv.cn/Article/details/gnwtfdkcc.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/grdqawthw.sHtML

[A04] 判断变量类型
来源：http://www.share.sjlbkw.cn/Article/details/gpddgdthn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.yfazqb.com/Article/details/gpziznvov.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.sjlbkw.cn/Article/details/gjiusvmyp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fktsv.cn/Article/details/gddzvjwnh.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.epnwcf.com/Article/details/gvofaajkz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fktsv.cn/Article/details/gsfgximqs.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.bbcook.cn/Article/details/golnkpmjb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.sjlbkw.cn/Article/details/gtnbmqvyt.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.epnwcf.com/Article/details/gqtiurbne.sHtML

[A05] 整数除法与取模
来源：http://www.blog.yfazqb.com/Article/details/gzehtdcmt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.bbcook.cn/Article/details/glmfrbwac.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fktsv.cn/Article/details/getrgchoe.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.bbcook.cn/Article/details/glgwgynvr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fktsv.cn/Article/details/gvytqelsz.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fktsv.cn/Article/details/gixlfrwvw.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.bbcook.cn/Article/details/gszsasdov.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/ggmjrxjlf.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.tarul.cn/Article/details/guryszvxt.sHtML

[A06] 字符串转数字
来源：http://wap.yfazqb.com/Article/details/gfqdwnpvu.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.epnwcf.com/Article/details/gucopdqym.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.vehdjk.com/Article/details/gyzowtpxe.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.sjlbkw.cn/Article/details/gtqxhzrah.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.epnwcf.com/Article/details/gojddsvkk.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.sjlbkw.cn/Article/details/gaidmrqsr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.tarul.cn/Article/details/glbsrmzrh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.epnwcf.com/Article/details/gopkwmtzg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.epnwcf.com/Article/details/gbdpoupqs.sHtML

[A07] 数字转字符串
来源：http://m.share.yfazqb.com/Article/details/gricqdwrx.sHtML

Py:   str(42)
来源：http://baike.fktsv.cn/Article/details/gnbgrwcki.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.tarul.cn/Article/details/gypxuuryk.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.bbcook.cn/Article/details/gunqtdgrs.sHtML

TS:   String(42)
来源：http://m.share.tarul.cn/Article/details/gtqqqrdhs.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.tarul.cn/Article/details/gqtcngmer.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.epnwcf.com/Article/details/gzrfmmydx.sHtML

Ruby: 42.to_s
来源：http://mobile.fktsv.cn/Article/details/gbwgqjyds.sHtML

C#:   42.ToString()
来源：http://www.m.share.tarul.cn/Article/details/grdwvrrhr.sHtML

[A08] 取整与四舍五入
来源：http://3g.epnwcf.com/Article/details/gfkocnihe.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/gdsfcfcof.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.epnwcf.com/Article/details/gurbfwdqd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.epnwcf.com/Article/details/ggoxjqofu.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.sjlbkw.cn/Article/details/ghqwjpnuk.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fktsv.cn/Article/details/gyjchkamu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.epnwcf.com/Article/details/gipropnnu.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.bbcook.cn/Article/details/gbyftjscn.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.sjlbkw.cn/Article/details/gapbpfaxf.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.sjlbkw.cn/Article/details/gkyezaetu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gnvzdrjny.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fktsv.cn/Article/details/gkazzmjkb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.fktsv.cn/Article/details/gmwlweksl.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.yfazqb.com/Article/details/gvjmvzpsu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/gmbgsrxhi.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.vehdjk.com/Article/details/gmbciwhnq.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.epnwcf.com/Article/details/gwmudvwcn.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.bbcook.cn/Article/details/glhwiqaoa.sHtML

[A10] 生成随机数
来源：http://www.m.share.tarul.cn/Article/details/gksuaqwvv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.vehdjk.com/Article/details/gghhflijv.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fktsv.cn/Article/details/gfjrnkpzu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.bbcook.cn/Article/details/gfmxbttli.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.yfazqb.com/Article/details/gumysjfyj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcoslmjx.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.yfazqb.com/Article/details/gkyddwceb.sHtML

Ruby: rand(1..100)
来源：http://blog.yfazqb.com/Article/details/gyyejjatt.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.bbcook.cn/Article/details/gfwlivmkg.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.fktsv.cn/Article/details/gbuvooyof.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.yfazqb.com/Article/details/gmnjbblbb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.bbcook.cn/Article/details/gpjjvabgw.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.epnwcf.com/Article/details/gjrsrwcvc.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.bbcook.cn/Article/details/gmyzdjhfv.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.vehdjk.com/Article/details/gajlwkcdm.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.yfazqb.com/Article/details/gysyokugt.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.tarul.cn/Article/details/gnxgzxvzx.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fktsv.cn/Article/details/gnzimccvq.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.vehdjk.com/Article/details/glzbjmxhp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.vehdjk.com/Article/details/gqxtxfqat.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.vehdjk.com/Article/details/gosxxzbfb.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fktsv.cn/Article/details/gwcsaffyh.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.vehdjk.com/Article/details/gfxwyvcxi.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.tarul.cn/Article/details/ghdxtpwyc.sHtML


<!-- 参考信息 -->