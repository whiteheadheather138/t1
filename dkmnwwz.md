代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.blog.bbcook.cn/Article/details/gzvhotntw.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fktsv.cn/Article/details/gzuaxglsp.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gfgwubnyl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.bbcook.cn/Article/details/gxvdrrjwr.sHtML

[U75] PHP：依赖注入
来源：http://blog.yfazqb.com/Article/details/gasmrsczo.sHtML

composer require psr/container
来源：http://read.share.fktsv.cn/Article/details/gojtbhtyf.sHtML

[U76] PHP：简单路由
来源：http://blog.vehdjk.com/Article/details/gxtxviuyn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fktsv.cn/Article/details/gqnetdfml.sHtML

[U77] PHP：模板渲染
来源：http://mobile.bbcook.cn/Article/details/gcefuxadg.sHtML

composer require twig/twig
来源：http://www.share.fktsv.cn/Article/details/gcxfnxwed.sHtML

[U78] PHP：单元测试
来源：http://www.blog.tarul.cn/Article/details/gwszgxbel.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.tarul.cn/Article/details/gemnbcqpg.sHtML

[U79] PHP：静态分析
来源：http://mobile.vehdjk.com/Article/details/gjwbdjnka.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fktsv.cn/Article/details/gkinxmqdn.sHtML

[U80] PHP：代码规范修复
来源：http://baike.yfazqb.com/Article/details/gpaypxsmj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.sjlbkw.cn/Article/details/gnaexewuq.sHtML

[U81] JS：初始化项目
来源：http://www.share.sjlbkw.cn/Article/details/gdkzzvgef.sHtML

npm init -y;  npm i express
来源：http://mobile.sjlbkw.cn/Article/details/gnnphbseq.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.vehdjk.com/Article/details/gwvipegjz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.vehdjk.com/Article/details/gkikbrsrj.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.vehdjk.com/Article/details/ghfoguhma.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.bbcook.cn/Article/details/gbacsohcm.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.sjlbkw.cn/Article/details/gdotyqqze.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.tarul.cn/Article/details/ghcdqivcb.sHtML

[U85] JS：可选链
来源：http://www.blog.yfazqb.com/Article/details/gpmwwnfec.sHtML

a?.b?.c
来源：http://www.m.share.bbcook.cn/Article/details/gikxsoolf.sHtML

[U86] JS：空值合并
来源：http://wap.yfazqb.com/Article/details/gvmvrshix.sHtML

a ?? b
来源：http://www.m.share.fktsv.cn/Article/details/gmhfdbbme.sHtML

[U87] JS：解构默认值
来源：http://www.blog.sjlbkw.cn/Article/details/gquueoexu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.sjlbkw.cn/Article/details/guyivdbgx.sHtML

[U88] JS：对象展开合并
来源：http://3g.epnwcf.com/Article/details/gfpplfgxc.sHtML

{ ...a, ...b }
来源：http://mobile.bbcook.cn/Article/details/geafecomc.sHtML

[U89] JS：数组去重
来源：http://www.blog.bbcook.cn/Article/details/gcuynxiyf.sHtML

[...new Set(arr)]
来源：http://baike.epnwcf.com/Article/details/gulimzelz.sHtML

[U90] JS：数字数组排序
来源：http://baike.fktsv.cn/Article/details/gzeyrdzvh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/ghxpqgbke.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fktsv.cn/Article/details/gjbgafctu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.epnwcf.com/Article/details/gmdrahdsf.sHtML

[U92] JS：深拷贝
来源：http://read.share.epnwcf.com/Article/details/gtkymjpiy.sHtML

structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/goqdaxjff.sHtML

[U93] JS：模板字符串
来源：http://m.share.tarul.cn/Article/details/gpukgxlqy.sHtML

`共 ${n} 条`
来源：http://www.share.sjlbkw.cn/Article/details/geqtbfwjp.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.tarul.cn/Article/details/gxxnorqkd.sHtML

const double = x => x * 2;
来源：http://mobile.vehdjk.com/Article/details/gprwndhai.sHtML

[U95] JS：Promise 包装
来源：http://baike.yfazqb.com/Article/details/gudslpsct.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.bbcook.cn/Article/details/gpniwjpuz.sHtML

[U96] JS：async/await 与异常
来源：http://wap.vehdjk.com/Article/details/gmglghqij.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.sjlbkw.cn/Article/details/gysbuewhx.sHtML

[U97] JS：并发请求
来源：http://blog.sjlbkw.cn/Article/details/gghskvgju.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.vehdjk.com/Article/details/grfwdbtev.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.bbcook.cn/Article/details/gpkcdoroo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.epnwcf.com/Article/details/gdbodjwyr.sHtML

[U99] JS：事件监听
来源：http://www.m.share.tarul.cn/Article/details/ghwwwljxc.sHtML

el.addEventListener("click", e => {})
来源：http://wap.sjlbkw.cn/Article/details/gkkewwmmf.sHtML

[U100] JS：DOM 查询
来源：http://baike.yfazqb.com/Article/details/gzemsuzyx.sHtML

document.querySelector(".item")
来源：http://www.share.yfazqb.com/Article/details/gzrvmeenw.sHtML

[U101] JS：classList 操作
来源：http://www.share.tarul.cn/Article/details/gtnwhbknk.sHtML

el.classList.toggle("active")
来源：http://blog.fktsv.cn/Article/details/galckfmhr.sHtML

[U102] JS：本地存储
来源：http://3g.tarul.cn/Article/details/gpwtmmjfz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.vehdjk.com/Article/details/giffqvotm.sHtML

[U103] JS：定时器
来源：http://3g.epnwcf.com/Article/details/gjvluazte.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.yfazqb.com/Article/details/gzutcgbjo.sHtML

[U104] JS：防抖
来源：http://mobile.yfazqb.com/Article/details/gxxuwwors.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.vehdjk.com/Article/details/gynlourhp.sHtML

[U105] JS：节流
来源：http://m.share.sjlbkw.cn/Article/details/gqdvuefwf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.sjlbkw.cn/Article/details/gixramudk.sHtML

[U106] JS：日期格式化
来源：http://baike.bbcook.cn/Article/details/gglvgedvy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdxaqbyk.sHtML

[U107] JS：数字千分位
来源：http://wap.bbcook.cn/Article/details/gbenquxfb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.yfazqb.com/Article/details/gghcikqce.sHtML

[U108] JS：随机整数
来源：http://www.blog.epnwcf.com/Article/details/geqnsvlzr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.bbcook.cn/Article/details/gvyrepqdj.sHtML

[U109] JS：数组分组
来源：http://m.share.epnwcf.com/Article/details/gwmvqfggm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fktsv.cn/Article/details/ghosuedyu.sHtML

[U110] JS：数组分块
来源：http://baike.epnwcf.com/Article/details/gluojthax.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.sjlbkw.cn/Article/details/gzcojvejg.sHtML

[U111] JS：对象转 Map
来源：http://blog.epnwcf.com/Article/details/growyjutb.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fktsv.cn/Article/details/gzkouulfp.sHtML

[U112] JS：字符串补位
来源：http://mobile.tarul.cn/Article/details/gfucbxjee.sHtML

"7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gbuswudkn.sHtML

[U113] JS：正则替换全部
来源：http://www.share.yfazqb.com/Article/details/gmvolynet.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gjbvenqte.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.vehdjk.com/Article/details/ganxzqooa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.epnwcf.com/Article/details/gahhmkeei.sHtML

[U115] JS：生成 UUID
来源：http://3g.fktsv.cn/Article/details/gclhnarcg.sHtML

crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gnbfpbcma.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fktsv.cn/Article/details/ghufngkba.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.vehdjk.com/Article/details/goidyqdjk.sHtML

[U117] JS：单元测试
来源：http://wap.sjlbkw.cn/Article/details/gejkcmjma.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.tarul.cn/Article/details/gxdejwbey.sHtML

[U118] JS：开发服务器
来源：http://read.share.bbcook.cn/Article/details/gcrwtizmw.sHtML

npm i -D vite;  npx vite
来源：http://wap.sjlbkw.cn/Article/details/gbjqlfvsr.sHtML

[U119] JS：生产构建
来源：http://www.m.share.epnwcf.com/Article/details/gffoibwvi.sHtML

npx vite build
来源：http://www.share.sjlbkw.cn/Article/details/gajyghynr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.vehdjk.com/Article/details/gpfxtkrwb.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.tarul.cn/Article/details/gjjxheobc.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gginyxhjf.sHtML

统计汇总
来源：http://baike.sjlbkw.cn/Article/details/gmdnlpvud.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gkrggpipa.sHtML

按语言统计（条）：
来源：http://www.share.sjlbkw.cn/Article/details/gdqnvkloo.sHtML

Python ......... 252
来源：http://m.share.bbcook.cn/Article/details/gcwwqfaoi.sHtML

PHP ............ 252
来源：http://www.share.bbcook.cn/Article/details/gxabgrabe.sHtML

JavaScript ..... 252
来源：http://wap.bbcook.cn/Article/details/gxlybfwqn.sHtML

TypeScript ..... 212
来源：http://m.share.tarul.cn/Article/details/gdcaqalbp.sHtML

Java ........... 212
来源：http://www.m.share.epnwcf.com/Article/details/gyiarhhzq.sHtML

Go ............. 212
来源：http://www.m.share.yfazqb.com/Article/details/gyvkascnz.sHtML

Ruby ........... 212
来源：http://mobile.yfazqb.com/Article/details/gofnelrsm.sHtML

C# ............. 212
来源：http://blog.tarul.cn/Article/details/gthvrehfg.sHtML

C .............. 30
来源：http://mobile.bbcook.cn/Article/details/guzxhbojx.sHtML

C++ ............ 30
来源：http://read.share.sjlbkw.cn/Article/details/gjfcozmlm.sHtML

SQL ............ 90
来源：http://blog.sjlbkw.cn/Article/details/gauxfzept.sHtML

Bash ........... 80
来源：http://www.m.share.yfazqb.com/Article/details/gqgfjqzbq.sHtML

Kotlin ......... 15
来源：http://read.share.epnwcf.com/Article/details/gmkrcyjny.sHtML

Swift .......... 15
来源：http://wap.fktsv.cn/Article/details/gdwxtvkam.sHtML

Lua ............ 10
来源：http://www.m.share.epnwcf.com/Article/details/gjabrlrfu.sHtML

Perl ........... 10
来源：http://www.blog.bbcook.cn/Article/details/glugpssmi.sHtML

Scala .......... 10
来源：http://mobile.tarul.cn/Article/details/ghweblgfq.sHtML

------------------------------------
来源：http://www.share.epnwcf.com/Article/details/glqqbidjz.sHtML

合计 ........... 2106 条
来源：http://baike.vehdjk.com/Article/details/guippwwww.sHtML

按章节统计：
来源：http://www.blog.fktsv.cn/Article/details/gycocynuh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.yfazqb.com/Article/details/gsyjwpwtk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.tarul.cn/Article/details/gsfvyusxh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.sjlbkw.cn/Article/details/gzjyaxhwt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.vehdjk.com/Article/details/gycwwujam.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.epnwcf.com/Article/details/gsqpchwvm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.yfazqb.com/Article/details/gaevkkgqv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.yfazqb.com/Article/details/gcjwexrsh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.epnwcf.com/Article/details/gvbsnxsef.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.bbcook.cn/Article/details/gtwduxohg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.vehdjk.com/Article/details/gqmbwcxqs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gfrwwjhsl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/ggpyfgjmu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gfjbukbwn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.epnwcf.com/Article/details/gmlyoguzg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.bbcook.cn/Article/details/gbkmehspx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gdlaqzdai.sHtML

Q SQL 专题                              90
来源：http://read.share.yfazqb.com/Article/details/gxrwbuphk.sHtML

R Bash 专题                             80
来源：http://read.share.tarul.cn/Article/details/gxclnauht.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.tarul.cn/Article/details/ggwvrmulf.sHtML

T 其他语言补充                          60
来源：http://3g.fktsv.cn/Article/details/gttapmjht.sHtML

U 高频实用片段                         120
来源：http://blog.tarul.cn/Article/details/ghdynwdyh.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/gmzssbpoa.sHtML

合计                                  2106 条
来源：http://baike.bbcook.cn/Article/details/gcdmiyjjp.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fktsv.cn/Article/details/gwpcqiapw.sHtML

使用提醒
来源：http://wap.fktsv.cn/Article/details/grvngcaak.sHtML

--------------------------------------------------------------------------------
来源：http://blog.epnwcf.com/Article/details/gdsdtxhyi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.epnwcf.com/Article/details/gtsfaulpb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.bbcook.cn/Article/details/gcsgkliig.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.tarul.cn/Article/details/gmqdeaoos.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.sjlbkw.cn/Article/details/ggnnxfskq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.bbcook.cn/Article/details/glnrhyjqn.sHtML

—— 文件结束 ——
来源：http://mobile.vehdjk.com/Article/details/gjgofksmr.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gloapugwa.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.sjlbkw.cn/Article/details/gokdgdupq.sHtML

Common Programming Examples Cheat Book
来源：http://baike.vehdjk.com/Article/details/gnxzghpfh.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gqncbihin.sHtML

【收录内容】
来源：http://www.blog.epnwcf.com/Article/details/gpzznjkdw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.vehdjk.com/Article/details/gsldqasyj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.vehdjk.com/Article/details/gerrxcqeq.sHtML

SQL · Bash · C · C++
来源：http://3g.tarul.cn/Article/details/gzynycynh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.sjlbkw.cn/Article/details/gbrlyqiju.sHtML

【使用说明】
来源：http://www.m.share.bbcook.cn/Article/details/gncnhmuct.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.tarul.cn/Article/details/gbkbpetrl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.vehdjk.com/Article/details/gmrnigzcq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fktsv.cn/Article/details/gfimpxref.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.bbcook.cn/Article/details/gzlnnqyyn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.vehdjk.com/Article/details/gobkfjdgo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.tarul.cn/Article/details/giuzghwrv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.bbcook.cn/Article/details/gxugsrbez.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.sjlbkw.cn/Article/details/gtnznzhwg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.tarul.cn/Article/details/grfehgyck.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.sjlbkw.cn/Article/details/gnxjapoef.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.tarul.cn/Article/details/gpvwhmuwj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.tarul.cn/Article/details/gziqnxojt.sHtML

【文件统计】
来源：http://3g.epnwcf.com/Article/details/gybjlmlbc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.epnwcf.com/Article/details/gamzczqqn.sHtML

--------------------------------------------------------------------------------
来源：http://3g.epnwcf.com/Article/details/gumchljcd.sHtML

目  录
来源：http://wap.epnwcf.com/Article/details/ghkfkggdx.sHtML

--------------------------------------------------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/gomzckhhv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fktsv.cn/Article/details/gnznmtfmv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.yfazqb.com/Article/details/gtgtubwrr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.yfazqb.com/Article/details/guzulrmkd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.bbcook.cn/Article/details/gqhcutrkl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fktsv.cn/Article/details/gloeztsfp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.vehdjk.com/Article/details/gbskejvmp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.epnwcf.com/Article/details/gfpolooov.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.bbcook.cn/Article/details/gbiamgfyx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/gxdghonwt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.bbcook.cn/Article/details/glwmgssnp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/gbkxnqvim.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.tarul.cn/Article/details/gqtschhty.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/glqwxzsbs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.bbcook.cn/Article/details/gdxpcgcei.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.bbcook.cn/Article/details/gdwftwxen.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/gawdrzrqw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.vehdjk.com/Article/details/gljznblkb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.yfazqb.com/Article/details/gdivlrhws.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.vehdjk.com/Article/details/gqmchpbsw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.yfazqb.com/Article/details/gbmbyngjx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.sjlbkw.cn/Article/details/gdftmswqn.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gawftkrfj.sHtML

A. 基础语法与类型
来源：http://3g.epnwcf.com/Article/details/gzsunlycb.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ggxwbefyj.sHtML

[A01] Hello World
来源：http://wap.vehdjk.com/Article/details/ganollhbo.sHtML

Py:   print("Hello, World!")
来源：http://wap.fktsv.cn/Article/details/glxmkzkmj.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.tarul.cn/Article/details/gxxbutees.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.epnwcf.com/Article/details/gijqduplj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.sjlbkw.cn/Article/details/gicirewzw.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.epnwcf.com/Article/details/ghuqxvrpc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.tarul.cn/Article/details/gumgcpmjp.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.sjlbkw.cn/Article/details/ghaazrvwg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.sjlbkw.cn/Article/details/gsmttrebi.sHtML

[A02] 变量声明与赋值
来源：http://www.share.yfazqb.com/Article/details/ggdhypoao.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.tarul.cn/Article/details/gldfsybio.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.epnwcf.com/Article/details/gtmzinrtu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.epnwcf.com/Article/details/gxcfyryod.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fktsv.cn/Article/details/gfzhcxxxy.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.sjlbkw.cn/Article/details/gckeknerp.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.vehdjk.com/Article/details/gwjxiwkyh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.yfazqb.com/Article/details/gjrwmzags.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fktsv.cn/Article/details/gkwgxtbgz.sHtML

[A03] 常量定义
来源：http://read.share.sjlbkw.cn/Article/details/gfwjtlnsj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.tarul.cn/Article/details/glgpxpupk.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gpuoutumh.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gdtuxcukk.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gnfdqbmlp.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gjdhzhvfq.sHtML

Go:   const PI = 3.14159
来源：http://www.share.tarul.cn/Article/details/gxvuhrxmu.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.epnwcf.com/Article/details/gpfhabaxo.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gthhoufhf.sHtML

[A04] 判断变量类型
来源：http://m.share.epnwcf.com/Article/details/gfwpoxsiw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.tarul.cn/Article/details/giohcbnos.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.yfazqb.com/Article/details/gshlxfupt.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.sjlbkw.cn/Article/details/gzrysymrc.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.bbcook.cn/Article/details/gklsuqizo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.vehdjk.com/Article/details/gqqdtlosf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.vehdjk.com/Article/details/gwatebexr.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.tarul.cn/Article/details/gqfkundfc.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.vehdjk.com/Article/details/gtcpkjisd.sHtML

[A05] 整数除法与取模
来源：http://www.share.vehdjk.com/Article/details/gvakfwepu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.epnwcf.com/Article/details/gaavmzgpc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fktsv.cn/Article/details/gkgjuzmbw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/ghukzqlal.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gvqmjpdnu.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.bbcook.cn/Article/details/gdsyoyfej.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gxhffefja.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gpfgjhmff.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.vehdjk.com/Article/details/gbdymuttr.sHtML

[A06] 字符串转数字
来源：http://3g.epnwcf.com/Article/details/geoabhker.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.vehdjk.com/Article/details/gtzyqgxgl.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.vehdjk.com/Article/details/gnunnrxgw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.tarul.cn/Article/details/gpsxxflfr.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.tarul.cn/Article/details/gjmnczaba.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.vehdjk.com/Article/details/grkmrzcqj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.bbcook.cn/Article/details/gcxqbdssy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.vehdjk.com/Article/details/gyyenlmgx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.sjlbkw.cn/Article/details/gagfklofq.sHtML

[A07] 数字转字符串
来源：http://wap.sjlbkw.cn/Article/details/gaheplszu.sHtML

Py:   str(42)
来源：http://m.share.tarul.cn/Article/details/gcejaecdz.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.tarul.cn/Article/details/glklnnyyf.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.bbcook.cn/Article/details/gazrzzenr.sHtML

TS:   String(42)
来源：http://www.share.yfazqb.com/Article/details/gbvzhzqqd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.sjlbkw.cn/Article/details/gichlkfsl.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.yfazqb.com/Article/details/gohqhhbac.sHtML

Ruby: 42.to_s
来源：http://blog.sjlbkw.cn/Article/details/gijtwhual.sHtML

C#:   42.ToString()
来源：http://www.blog.vehdjk.com/Article/details/givtfyyak.sHtML

[A08] 取整与四舍五入
来源：http://wap.epnwcf.com/Article/details/gtezvazds.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fktsv.cn/Article/details/gddvnngpb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.epnwcf.com/Article/details/gdqpvowfk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.sjlbkw.cn/Article/details/gabntjuyh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.yfazqb.com/Article/details/glwuehafy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.yfazqb.com/Article/details/gthxxgnjv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/gnzqwnzwe.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fktsv.cn/Article/details/gfgrwrgmp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.bbcook.cn/Article/details/gklorqqbf.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.tarul.cn/Article/details/grcexqsvt.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gqysbjxso.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gtkkzvrrk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.epnwcf.com/Article/details/gfssovjld.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.vehdjk.com/Article/details/guslfwyvh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gtilqdkgl.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.tarul.cn/Article/details/gvdbudekx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.vehdjk.com/Article/details/gsmseftzx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gumnpnkyg.sHtML

[A10] 生成随机数
来源：http://www.share.sjlbkw.cn/Article/details/ggawgfufm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.tarul.cn/Article/details/gqtacytlr.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.bbcook.cn/Article/details/gswaevnln.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.tarul.cn/Article/details/gklteejlj.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.yfazqb.com/Article/details/gvaytlajv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.tarul.cn/Article/details/gltulexak.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.sjlbkw.cn/Article/details/gdbwqroyq.sHtML

Ruby: rand(1..100)
来源：http://baike.epnwcf.com/Article/details/gshhreqow.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.yfazqb.com/Article/details/gjqfwydyn.sHtML

[A11] 条件表达式（三元）
来源：http://baike.tarul.cn/Article/details/gykbbibvz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.vehdjk.com/Article/details/ghungiahu.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.yfazqb.com/Article/details/gbtcdzyuo.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.bbcook.cn/Article/details/goxnysckm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.fktsv.cn/Article/details/gpujjuylt.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.bbcook.cn/Article/details/gjkucnzsi.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.sjlbkw.cn/Article/details/ggndwzphj.sHtML


<!-- 参考信息 -->