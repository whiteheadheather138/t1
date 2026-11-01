代发 wailian999

[U71] PHP：抛出异常
来源：http://read.share.tarul.cn/Article/details/goqmimoau.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.sjlbkw.cn/Article/details/goktoaovd.sHtML

[U72] PHP：写错误日志
来源：http://mobile.vehdjk.com/Article/details/guubrwyiy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fktsv.cn/Article/details/gdknbrsuy.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.yfazqb.com/Article/details/gfwlxrfph.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.vehdjk.com/Article/details/ghvkzjxgj.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.tarul.cn/Article/details/grnoouwig.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.yfazqb.com/Article/details/gmfplynjl.sHtML

[U75] PHP：依赖注入
来源：http://mobile.tarul.cn/Article/details/gtszdndfn.sHtML

composer require psr/container
来源：http://blog.sjlbkw.cn/Article/details/gcipoixow.sHtML

[U76] PHP：简单路由
来源：http://mobile.sjlbkw.cn/Article/details/gmzkbmuur.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.yfazqb.com/Article/details/gptgyyneb.sHtML

[U77] PHP：模板渲染
来源：http://baike.fktsv.cn/Article/details/gupdvzuwj.sHtML

composer require twig/twig
来源：http://3g.bbcook.cn/Article/details/gxnglpegj.sHtML

[U78] PHP：单元测试
来源：http://www.share.bbcook.cn/Article/details/grynglkye.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.tarul.cn/Article/details/gpjqehxhl.sHtML

[U79] PHP：静态分析
来源：http://wap.bbcook.cn/Article/details/gualhbxcg.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.epnwcf.com/Article/details/gygwbmacm.sHtML

[U80] PHP：代码规范修复
来源：http://blog.bbcook.cn/Article/details/gowzsihcw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fktsv.cn/Article/details/gwkwlyuwm.sHtML

[U81] JS：初始化项目
来源：http://wap.sjlbkw.cn/Article/details/ghkwwxjzg.sHtML

npm init -y;  npm i express
来源：http://m.share.epnwcf.com/Article/details/gbmjpxudh.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.yfazqb.com/Article/details/gffwnonip.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fktsv.cn/Article/details/gggalvvue.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.yfazqb.com/Article/details/gyskcwxzw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.yfazqb.com/Article/details/golhsjrfu.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.tarul.cn/Article/details/gafwiples.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.sjlbkw.cn/Article/details/gylqfbfep.sHtML

[U85] JS：可选链
来源：http://mobile.tarul.cn/Article/details/ggmysesoj.sHtML

a?.b?.c
来源：http://read.share.sjlbkw.cn/Article/details/gxjylwcns.sHtML

[U86] JS：空值合并
来源：http://www.blog.fktsv.cn/Article/details/gwohkjgwe.sHtML

a ?? b
来源：http://www.m.share.bbcook.cn/Article/details/gqfqirvwf.sHtML

[U87] JS：解构默认值
来源：http://baike.yfazqb.com/Article/details/gjefaicly.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.sjlbkw.cn/Article/details/gnszaajip.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fktsv.cn/Article/details/gctswtscs.sHtML

{ ...a, ...b }
来源：http://www.blog.tarul.cn/Article/details/gcerpvnyz.sHtML

[U89] JS：数组去重
来源：http://mobile.epnwcf.com/Article/details/gpvwlwpge.sHtML

[...new Set(arr)]
来源：http://wap.bbcook.cn/Article/details/gyworpjnt.sHtML

[U90] JS：数字数组排序
来源：http://blog.yfazqb.com/Article/details/gojfujiom.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gmsnigjzw.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.epnwcf.com/Article/details/gckdgqjkd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.vehdjk.com/Article/details/gguesivtx.sHtML

[U92] JS：深拷贝
来源：http://read.share.epnwcf.com/Article/details/ggefcxewh.sHtML

structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/gfxwoluya.sHtML

[U93] JS：模板字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gqnkopscr.sHtML

`共 ${n} 条`
来源：http://read.share.fktsv.cn/Article/details/ggbvxjxoc.sHtML

[U94] JS：箭头函数
来源：http://wap.tarul.cn/Article/details/ggtyqbuxd.sHtML

const double = x => x * 2;
来源：http://read.share.sjlbkw.cn/Article/details/gmspzsbeu.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fktsv.cn/Article/details/gcwvwfkci.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.bbcook.cn/Article/details/gousadihg.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.yfazqb.com/Article/details/gxkdfzfel.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/glpcdursn.sHtML

[U97] JS：并发请求
来源：http://baike.bbcook.cn/Article/details/gukxqadjp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gefkrswhf.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.vehdjk.com/Article/details/ghyrrbxfv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.sjlbkw.cn/Article/details/gddtzogxc.sHtML

[U99] JS：事件监听
来源：http://read.share.sjlbkw.cn/Article/details/gnhfbcgwx.sHtML

el.addEventListener("click", e => {})
来源：http://baike.vehdjk.com/Article/details/gtnatyesa.sHtML

[U100] JS：DOM 查询
来源：http://baike.tarul.cn/Article/details/gpoipfqyg.sHtML

document.querySelector(".item")
来源：http://wap.vehdjk.com/Article/details/gmxjoivlq.sHtML

[U101] JS：classList 操作
来源：http://blog.sjlbkw.cn/Article/details/ggmgiueky.sHtML

el.classList.toggle("active")
来源：http://blog.yfazqb.com/Article/details/grnllgfjp.sHtML

[U102] JS：本地存储
来源：http://mobile.vehdjk.com/Article/details/gluotoyif.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fktsv.cn/Article/details/gibqimrnv.sHtML

[U103] JS：定时器
来源：http://www.m.share.fktsv.cn/Article/details/gewkxhdbx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.epnwcf.com/Article/details/gylfdrvdv.sHtML

[U104] JS：防抖
来源：http://mobile.sjlbkw.cn/Article/details/gnniioglk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/ggzdwkrqi.sHtML

[U105] JS：节流
来源：http://read.share.tarul.cn/Article/details/gzvkoehil.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.sjlbkw.cn/Article/details/gpgbsebrz.sHtML

[U106] JS：日期格式化
来源：http://blog.bbcook.cn/Article/details/gcrkargwd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.sjlbkw.cn/Article/details/gxifoaofm.sHtML

[U107] JS：数字千分位
来源：http://blog.bbcook.cn/Article/details/gcefvymel.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.bbcook.cn/Article/details/gzeuqxhdf.sHtML

[U108] JS：随机整数
来源：http://www.share.vehdjk.com/Article/details/grhexhepa.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fktsv.cn/Article/details/goetbinbb.sHtML

[U109] JS：数组分组
来源：http://m.share.yfazqb.com/Article/details/gaunesklu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.vehdjk.com/Article/details/gyehalmnt.sHtML

[U110] JS：数组分块
来源：http://m.share.yfazqb.com/Article/details/gjhqlanlz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.sjlbkw.cn/Article/details/gjxbnrpyy.sHtML

[U111] JS：对象转 Map
来源：http://blog.tarul.cn/Article/details/gywanddgq.sHtML

new Map(Object.entries(obj))
来源：http://read.share.yfazqb.com/Article/details/gbjnxouij.sHtML

[U112] JS：字符串补位
来源：http://blog.vehdjk.com/Article/details/gyrgpdnvn.sHtML

"7".padStart(3, "0")
来源：http://3g.vehdjk.com/Article/details/gxqjgxeut.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.vehdjk.com/Article/details/gadkcqvwl.sHtML

s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gnvkwozmf.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.epnwcf.com/Article/details/gccmiqzxh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.bbcook.cn/Article/details/gkrcdcqaj.sHtML

[U115] JS：生成 UUID
来源：http://baike.fktsv.cn/Article/details/goofjafte.sHtML

crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/glclsjdso.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.bbcook.cn/Article/details/gtxuvplgk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.bbcook.cn/Article/details/gfqrbpewy.sHtML

[U117] JS：单元测试
来源：http://www.blog.fktsv.cn/Article/details/gevdxiyhv.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.bbcook.cn/Article/details/gqjmrioiq.sHtML

[U118] JS：开发服务器
来源：http://mobile.fktsv.cn/Article/details/gtlvgtymv.sHtML

npm i -D vite;  npx vite
来源：http://baike.vehdjk.com/Article/details/ggdctgbhn.sHtML

[U119] JS：生产构建
来源：http://read.share.bbcook.cn/Article/details/ghjekmwch.sHtML

npx vite build
来源：http://m.share.epnwcf.com/Article/details/gmclvxeee.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fktsv.cn/Article/details/gfxuirfbp.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.yfazqb.com/Article/details/gvgfhrmfa.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/girapbltd.sHtML

统计汇总
来源：http://m.share.yfazqb.com/Article/details/gadxojeux.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/goddzfxwm.sHtML

按语言统计（条）：
来源：http://read.share.tarul.cn/Article/details/gfkmmzcvz.sHtML

Python ......... 252
来源：http://www.m.share.sjlbkw.cn/Article/details/glibzxblt.sHtML

PHP ............ 252
来源：http://wap.epnwcf.com/Article/details/gxamxpfhy.sHtML

JavaScript ..... 252
来源：http://mobile.vehdjk.com/Article/details/glvlxzkqx.sHtML

TypeScript ..... 212
来源：http://blog.fktsv.cn/Article/details/gdixyaycr.sHtML

Java ........... 212
来源：http://read.share.yfazqb.com/Article/details/gsbdygrgh.sHtML

Go ............. 212
来源：http://read.share.sjlbkw.cn/Article/details/ggcpqhsrc.sHtML

Ruby ........... 212
来源：http://baike.bbcook.cn/Article/details/gwgfzpccy.sHtML

C# ............. 212
来源：http://blog.epnwcf.com/Article/details/gchpovmod.sHtML

C .............. 30
来源：http://www.m.share.epnwcf.com/Article/details/gjjxnvayt.sHtML

C++ ............ 30
来源：http://baike.yfazqb.com/Article/details/glfmvoygq.sHtML

SQL ............ 90
来源：http://www.share.sjlbkw.cn/Article/details/goikzdaut.sHtML

Bash ........... 80
来源：http://www.m.share.tarul.cn/Article/details/gqbxnwxxe.sHtML

Kotlin ......... 15
来源：http://www.blog.sjlbkw.cn/Article/details/gustavszf.sHtML

Swift .......... 15
来源：http://baike.tarul.cn/Article/details/gerzywxad.sHtML

Lua ............ 10
来源：http://baike.tarul.cn/Article/details/gratzwqvo.sHtML

Perl ........... 10
来源：http://m.share.bbcook.cn/Article/details/ghagkkrhq.sHtML

Scala .......... 10
来源：http://blog.epnwcf.com/Article/details/gevyifbxh.sHtML

------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/giifleexi.sHtML

合计 ........... 2106 条
来源：http://wap.fktsv.cn/Article/details/gutcydehm.sHtML

按章节统计：
来源：http://blog.fktsv.cn/Article/details/gpraktfyh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.bbcook.cn/Article/details/gpfkacazq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.tarul.cn/Article/details/gzkdhpdhh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.sjlbkw.cn/Article/details/gyotbrnhv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fktsv.cn/Article/details/gyqahottc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.epnwcf.com/Article/details/gqtpjpiiu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.vehdjk.com/Article/details/gtwthjvyn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.yfazqb.com/Article/details/glroquibf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.vehdjk.com/Article/details/gayviooih.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/gmjxztczw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.epnwcf.com/Article/details/gsfwnspoa.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gssxwwlge.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/gikzgwmki.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gysaoppjx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.tarul.cn/Article/details/gdxjtqgcn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.vehdjk.com/Article/details/gxjesujmi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gemqjnhyb.sHtML

Q SQL 专题                              90
来源：http://baike.yfazqb.com/Article/details/gdwholngr.sHtML

R Bash 专题                             80
来源：http://baike.vehdjk.com/Article/details/gmaejkypg.sHtML

S C / C++ 专题                          60
来源：http://m.share.tarul.cn/Article/details/guklkyyfl.sHtML

T 其他语言补充                          60
来源：http://m.share.fktsv.cn/Article/details/gqsdzbxcs.sHtML

U 高频实用片段                         120
来源：http://m.share.epnwcf.com/Article/details/gygsvfdsm.sHtML

------------------------------------
来源：http://www.blog.tarul.cn/Article/details/ghosjuevg.sHtML

合计                                  2106 条
来源：http://www.blog.vehdjk.com/Article/details/gjzorrpff.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/ghnivcpgk.sHtML

使用提醒
来源：http://www.share.epnwcf.com/Article/details/gukshxusc.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/ggxtpuccc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.sjlbkw.cn/Article/details/gmuforqqo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.bbcook.cn/Article/details/gocmdqxzu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.bbcook.cn/Article/details/gfjepogdz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.vehdjk.com/Article/details/gnqasjqsx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.epnwcf.com/Article/details/gdvzmfioh.sHtML

—— 文件结束 ——
来源：http://www.share.bbcook.cn/Article/details/gmpiedwzr.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/graalpivn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fktsv.cn/Article/details/ghxnrifjf.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fktsv.cn/Article/details/gabynlajf.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gnzrpanjr.sHtML

【收录内容】
来源：http://www.share.tarul.cn/Article/details/gndchtcxa.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.vehdjk.com/Article/details/gvmtuzxcl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.epnwcf.com/Article/details/gkyskibyz.sHtML

SQL · Bash · C · C++
来源：http://mobile.vehdjk.com/Article/details/gpxhjxsqw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fktsv.cn/Article/details/gfdzkeogc.sHtML

【使用说明】
来源：http://www.m.share.bbcook.cn/Article/details/gdyuhvnkc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.epnwcf.com/Article/details/gfayxrcuk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.sjlbkw.cn/Article/details/gvbxqvwiu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.bbcook.cn/Article/details/gttnsspcb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.epnwcf.com/Article/details/gopcwypdv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fktsv.cn/Article/details/gvmlskwir.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.bbcook.cn/Article/details/gyoutpsti.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.bbcook.cn/Article/details/gwoacjkze.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fktsv.cn/Article/details/gpnjdnrah.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.bbcook.cn/Article/details/gllehhbtv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.bbcook.cn/Article/details/ghmrbrmdk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.sjlbkw.cn/Article/details/gttnwgwje.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.yfazqb.com/Article/details/gafrakxik.sHtML

【文件统计】
来源：http://www.share.fktsv.cn/Article/details/griyjwowi.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.yfazqb.com/Article/details/grneuoxlj.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gklsjtvnm.sHtML

目  录
来源：http://3g.tarul.cn/Article/details/gxznirlgm.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gxmehdhcw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.yfazqb.com/Article/details/gyaelbazt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.tarul.cn/Article/details/gleroivcv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.sjlbkw.cn/Article/details/gmiazqtzd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.epnwcf.com/Article/details/gdffxvmgv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.tarul.cn/Article/details/gqqxlpkoi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.bbcook.cn/Article/details/gfuvxxhry.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fktsv.cn/Article/details/ggkyasgcq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.yfazqb.com/Article/details/gvksaytox.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gvxvzjlhq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.epnwcf.com/Article/details/gmgftzbug.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.tarul.cn/Article/details/gvnfrtslg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.sjlbkw.cn/Article/details/gzkcihahe.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/gueldsiah.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.sjlbkw.cn/Article/details/gucehdkvb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.sjlbkw.cn/Article/details/gahbewovy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.vehdjk.com/Article/details/gsddvywzk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.bbcook.cn/Article/details/gxhmormlx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.sjlbkw.cn/Article/details/geemevhdg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fktsv.cn/Article/details/gpkxkjish.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.sjlbkw.cn/Article/details/gbaxwtkaf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.sjlbkw.cn/Article/details/gzyrmydwp.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gijpzqhxd.sHtML

A. 基础语法与类型
来源：http://m.share.fktsv.cn/Article/details/gmobhfmyl.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gfrjpjexb.sHtML

[A01] Hello World
来源：http://wap.bbcook.cn/Article/details/gwjhlojxk.sHtML

Py:   print("Hello, World!")
来源：http://baike.yfazqb.com/Article/details/goetylafz.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fktsv.cn/Article/details/gjtycgtmu.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.sjlbkw.cn/Article/details/gepdvlxyh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.yfazqb.com/Article/details/gyqybgndl.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fktsv.cn/Article/details/gcgmpputl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.yfazqb.com/Article/details/gxjkuglkr.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.bbcook.cn/Article/details/gauwubljd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.tarul.cn/Article/details/gkqayyyop.sHtML

[A02] 变量声明与赋值
来源：http://mobile.vehdjk.com/Article/details/gumagzclx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fktsv.cn/Article/details/gnxmqwblj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.bbcook.cn/Article/details/gctxivkbh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.bbcook.cn/Article/details/gabhtiert.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.yfazqb.com/Article/details/gtxlelvsq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.epnwcf.com/Article/details/gionkooys.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.yfazqb.com/Article/details/gdlybbouy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.sjlbkw.cn/Article/details/gxzmbkpty.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.vehdjk.com/Article/details/gdmwpeavt.sHtML

[A03] 常量定义
来源：http://m.share.fktsv.cn/Article/details/gqxfuidtq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.vehdjk.com/Article/details/gppzmklks.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gufetoqjg.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gvcjofbtf.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gstgmhaxr.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/guqaptfuv.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fktsv.cn/Article/details/gkkkhpjqb.sHtML

Ruby: PI = 3.14159
来源：http://www.share.tarul.cn/Article/details/goyzqkaoe.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gbocqqiwr.sHtML

[A04] 判断变量类型
来源：http://read.share.tarul.cn/Article/details/gzasyyzyr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fktsv.cn/Article/details/gfvrirpnk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.tarul.cn/Article/details/ghhbichbd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.vehdjk.com/Article/details/guannnjii.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.tarul.cn/Article/details/gmfsrpors.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.bbcook.cn/Article/details/gajzebozi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fktsv.cn/Article/details/giilaiefd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.vehdjk.com/Article/details/gqnugqlme.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fktsv.cn/Article/details/glggeguto.sHtML

[A05] 整数除法与取模
来源：http://www.blog.sjlbkw.cn/Article/details/gzjmyvyph.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.tarul.cn/Article/details/gzahgpcmy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/gfebshxhs.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.bbcook.cn/Article/details/gcxdbcohj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fktsv.cn/Article/details/gendgjjwi.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/grkgzouok.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gfcmqdrym.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gcvmvcqsl.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.bbcook.cn/Article/details/gaosfjrep.sHtML

[A06] 字符串转数字
来源：http://baike.tarul.cn/Article/details/gfamlpfbv.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fktsv.cn/Article/details/gotqdxzon.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.sjlbkw.cn/Article/details/gffikmwkl.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.yfazqb.com/Article/details/gfelqovbv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.yfazqb.com/Article/details/gjehhtlka.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.vehdjk.com/Article/details/gipbfkcsx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.vehdjk.com/Article/details/gqxkdcfbe.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.bbcook.cn/Article/details/gtkobbuak.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.sjlbkw.cn/Article/details/grchfnbls.sHtML

[A07] 数字转字符串
来源：http://wap.bbcook.cn/Article/details/gwuvuunsq.sHtML

Py:   str(42)
来源：http://wap.vehdjk.com/Article/details/gnobinoay.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fktsv.cn/Article/details/gtsizqxkb.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.sjlbkw.cn/Article/details/gxduhgfgg.sHtML

TS:   String(42)
来源：http://read.share.yfazqb.com/Article/details/gdclcmeds.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.vehdjk.com/Article/details/gwxwbsjug.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.sjlbkw.cn/Article/details/gyvixpebn.sHtML

Ruby: 42.to_s
来源：http://m.share.sjlbkw.cn/Article/details/gvcfuvvfc.sHtML

C#:   42.ToString()
来源：http://www.share.epnwcf.com/Article/details/gosjiekzl.sHtML

[A08] 取整与四舍五入
来源：http://baike.bbcook.cn/Article/details/gfpsalmzt.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fktsv.cn/Article/details/gfywrylhw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.vehdjk.com/Article/details/gresfayom.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.vehdjk.com/Article/details/ggoxirtda.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.bbcook.cn/Article/details/gbnxvavxc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.yfazqb.com/Article/details/gcxbhczxk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/gmxzrxszi.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.bbcook.cn/Article/details/gjztybsuo.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.tarul.cn/Article/details/gnxdeqczl.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.epnwcf.com/Article/details/ggocopghr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.vehdjk.com/Article/details/gsssbtqqh.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/ghipqinci.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.yfazqb.com/Article/details/ggulxhxka.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.fktsv.cn/Article/details/gdxzspqts.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gxtvnhgnv.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.sjlbkw.cn/Article/details/gzivjebiw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.yfazqb.com/Article/details/gmrpqkciy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.tarul.cn/Article/details/gpgrsvzqv.sHtML

[A10] 生成随机数
来源：http://baike.yfazqb.com/Article/details/gitenmaoe.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.yfazqb.com/Article/details/gddtkkjmt.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.bbcook.cn/Article/details/gdoqnqhip.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.vehdjk.com/Article/details/gxjunytwn.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.vehdjk.com/Article/details/gdphsbexu.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.vehdjk.com/Article/details/gholkrich.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.vehdjk.com/Article/details/ggtuwjaye.sHtML

Ruby: rand(1..100)
来源：http://www.blog.epnwcf.com/Article/details/gtbegmksy.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.yfazqb.com/Article/details/grskoqkre.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.fktsv.cn/Article/details/gzjcykvbz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fktsv.cn/Article/details/gbqdmpksz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.yfazqb.com/Article/details/gtewcsdsa.sHtML


<!-- 参考信息 -->