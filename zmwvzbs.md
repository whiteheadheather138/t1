代发 wailian999

[U71] PHP：抛出异常
来源：http://www.blog.fktsv.cn/Article/details/gbrsyuiwc.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.tarul.cn/Article/details/gvnijggxj.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fktsv.cn/Article/details/gdsobuxwh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.vehdjk.com/Article/details/gueszykbh.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.bbcook.cn/Article/details/gzizjqzim.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.vehdjk.com/Article/details/gjhucrhyk.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.sjlbkw.cn/Article/details/gqdhdfzth.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.epnwcf.com/Article/details/ghuyrtjda.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fktsv.cn/Article/details/gqpdwueez.sHtML

composer require psr/container
来源：http://www.blog.vehdjk.com/Article/details/gumiyzznc.sHtML

[U76] PHP：简单路由
来源：http://blog.sjlbkw.cn/Article/details/goqxkgyqz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.epnwcf.com/Article/details/gzibncxjd.sHtML

[U77] PHP：模板渲染
来源：http://www.share.tarul.cn/Article/details/gqjctktam.sHtML

composer require twig/twig
来源：http://www.m.share.epnwcf.com/Article/details/gbhnuqcjg.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.epnwcf.com/Article/details/gbzsbikvo.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.sjlbkw.cn/Article/details/gpmgspozq.sHtML

[U79] PHP：静态分析
来源：http://blog.epnwcf.com/Article/details/gyoceaknu.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.bbcook.cn/Article/details/gpjsrnarq.sHtML

[U80] PHP：代码规范修复
来源：http://3g.yfazqb.com/Article/details/grytxhmgl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fktsv.cn/Article/details/gymnfxhls.sHtML

[U81] JS：初始化项目
来源：http://www.blog.epnwcf.com/Article/details/gsppvnyyk.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fktsv.cn/Article/details/gdiqjhimy.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.vehdjk.com/Article/details/gtlqstnxv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.sjlbkw.cn/Article/details/ginwyvipf.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.yfazqb.com/Article/details/gkqonxyyd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.bbcook.cn/Article/details/gzxbtjqbm.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.epnwcf.com/Article/details/gtlmdhfrz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.bbcook.cn/Article/details/gnejtymxn.sHtML

[U85] JS：可选链
来源：http://wap.epnwcf.com/Article/details/gtaazajar.sHtML

a?.b?.c
来源：http://3g.epnwcf.com/Article/details/gdjbhyjxg.sHtML

[U86] JS：空值合并
来源：http://wap.fktsv.cn/Article/details/gsqogebst.sHtML

a ?? b
来源：http://blog.epnwcf.com/Article/details/gxspunama.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fktsv.cn/Article/details/gduohydys.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.bbcook.cn/Article/details/gmyushuzb.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fktsv.cn/Article/details/gbpshslpc.sHtML

{ ...a, ...b }
来源：http://www.share.sjlbkw.cn/Article/details/gzsxwslss.sHtML

[U89] JS：数组去重
来源：http://m.share.yfazqb.com/Article/details/glydjwjud.sHtML

[...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gnarmrbri.sHtML

[U90] JS：数字数组排序
来源：http://blog.epnwcf.com/Article/details/ggphzjtwe.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.bbcook.cn/Article/details/gfuajumio.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.epnwcf.com/Article/details/gxqlxhmfl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.vehdjk.com/Article/details/gupngitol.sHtML

[U92] JS：深拷贝
来源：http://3g.sjlbkw.cn/Article/details/gdyzjmzdk.sHtML

structuredClone(obj)
来源：http://mobile.epnwcf.com/Article/details/gxquhqjlo.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.vehdjk.com/Article/details/gmzoqchhv.sHtML

`共 ${n} 条`
来源：http://mobile.sjlbkw.cn/Article/details/gapxmmyjg.sHtML

[U94] JS：箭头函数
来源：http://m.share.tarul.cn/Article/details/glziwanqg.sHtML

const double = x => x * 2;
来源：http://3g.yfazqb.com/Article/details/guwzlzavi.sHtML

[U95] JS：Promise 包装
来源：http://read.share.sjlbkw.cn/Article/details/gtstuanyc.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.epnwcf.com/Article/details/giqzaxigc.sHtML

[U96] JS：async/await 与异常
来源：http://blog.bbcook.cn/Article/details/grwwdxaeo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/guosvoptl.sHtML

[U97] JS：并发请求
来源：http://m.share.vehdjk.com/Article/details/gyncpqatd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gheumunwl.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.yfazqb.com/Article/details/gthzjywnr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.sjlbkw.cn/Article/details/gzjtvigxl.sHtML

[U99] JS：事件监听
来源：http://blog.sjlbkw.cn/Article/details/gjjdsyume.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fktsv.cn/Article/details/gvuhkgcir.sHtML

[U100] JS：DOM 查询
来源：http://blog.sjlbkw.cn/Article/details/gzbephbya.sHtML

document.querySelector(".item")
来源：http://www.m.share.vehdjk.com/Article/details/gqraacuor.sHtML

[U101] JS：classList 操作
来源：http://wap.tarul.cn/Article/details/gikdtdqdt.sHtML

el.classList.toggle("active")
来源：http://read.share.yfazqb.com/Article/details/gmblikttq.sHtML

[U102] JS：本地存储
来源：http://read.share.sjlbkw.cn/Article/details/gmwypjpat.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.vehdjk.com/Article/details/gavvjencm.sHtML

[U103] JS：定时器
来源：http://mobile.sjlbkw.cn/Article/details/gnopajdev.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.sjlbkw.cn/Article/details/glrzpxyta.sHtML

[U104] JS：防抖
来源：http://www.blog.vehdjk.com/Article/details/glzbbivox.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/gmecdxueh.sHtML

[U105] JS：节流
来源：http://3g.tarul.cn/Article/details/grwfdpeah.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gghvzatun.sHtML

[U106] JS：日期格式化
来源：http://wap.fktsv.cn/Article/details/gltmgpbnl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fktsv.cn/Article/details/grsjwmxwe.sHtML

[U107] JS：数字千分位
来源：http://3g.tarul.cn/Article/details/gzufgcnva.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/glfmvfihp.sHtML

[U108] JS：随机整数
来源：http://www.blog.yfazqb.com/Article/details/gszoyzuba.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.vehdjk.com/Article/details/gqssgjnlg.sHtML

[U109] JS：数组分组
来源：http://www.share.bbcook.cn/Article/details/gwgonutzy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fktsv.cn/Article/details/gzefnzcfh.sHtML

[U110] JS：数组分块
来源：http://m.share.yfazqb.com/Article/details/ggenrztya.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.bbcook.cn/Article/details/gmfmtombo.sHtML

[U111] JS：对象转 Map
来源：http://www.share.vehdjk.com/Article/details/gcwrfgsyr.sHtML

new Map(Object.entries(obj))
来源：http://wap.yfazqb.com/Article/details/gmzhdswyd.sHtML

[U112] JS：字符串补位
来源：http://mobile.tarul.cn/Article/details/gxsnaejqo.sHtML

"7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gnqwsyerg.sHtML

[U113] JS：正则替换全部
来源：http://wap.fktsv.cn/Article/details/gklyeequz.sHtML

s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gdpnodzpj.sHtML

[U114] JS：JSON 深比较
来源：http://blog.tarul.cn/Article/details/ghexixeon.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.tarul.cn/Article/details/gvddcwjse.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fktsv.cn/Article/details/gpqdmrnzb.sHtML

crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/gntlxyuff.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.sjlbkw.cn/Article/details/genubfcys.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.sjlbkw.cn/Article/details/gfnycdxxo.sHtML

[U117] JS：单元测试
来源：http://www.share.bbcook.cn/Article/details/gxkijxiqm.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.sjlbkw.cn/Article/details/glwzowdno.sHtML

[U118] JS：开发服务器
来源：http://mobile.yfazqb.com/Article/details/ggxunyhny.sHtML

npm i -D vite;  npx vite
来源：http://baike.vehdjk.com/Article/details/gyvxeyqmv.sHtML

[U119] JS：生产构建
来源：http://blog.epnwcf.com/Article/details/gogrzmojb.sHtML

npx vite build
来源：http://www.blog.tarul.cn/Article/details/gjpujzztr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fktsv.cn/Article/details/gnxladdiw.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.vehdjk.com/Article/details/gkfpphozi.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/giujmhoay.sHtML

统计汇总
来源：http://blog.fktsv.cn/Article/details/gzxezxmnr.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gviyqilwx.sHtML

按语言统计（条）：
来源：http://www.blog.yfazqb.com/Article/details/gdxgxsrpg.sHtML

Python ......... 252
来源：http://m.share.tarul.cn/Article/details/gzmruiriw.sHtML

PHP ............ 252
来源：http://blog.yfazqb.com/Article/details/gzkyrsjcn.sHtML

JavaScript ..... 252
来源：http://read.share.fktsv.cn/Article/details/gujaxsjrm.sHtML

TypeScript ..... 212
来源：http://3g.bbcook.cn/Article/details/glkyjmnwv.sHtML

Java ........... 212
来源：http://baike.bbcook.cn/Article/details/gnrbkojku.sHtML

Go ............. 212
来源：http://3g.epnwcf.com/Article/details/grgxknaoi.sHtML

Ruby ........... 212
来源：http://m.share.fktsv.cn/Article/details/gkntkhjsi.sHtML

C# ............. 212
来源：http://read.share.tarul.cn/Article/details/ggfshjcpc.sHtML

C .............. 30
来源：http://3g.yfazqb.com/Article/details/gesoynpqw.sHtML

C++ ............ 30
来源：http://3g.sjlbkw.cn/Article/details/gzzlhhhzx.sHtML

SQL ............ 90
来源：http://wap.epnwcf.com/Article/details/gtjarfuuk.sHtML

Bash ........... 80
来源：http://read.share.tarul.cn/Article/details/gbhjxcivd.sHtML

Kotlin ......... 15
来源：http://baike.epnwcf.com/Article/details/gjadnogif.sHtML

Swift .......... 15
来源：http://3g.yfazqb.com/Article/details/gxvwfdmzv.sHtML

Lua ............ 10
来源：http://blog.sjlbkw.cn/Article/details/ggdzeoqfr.sHtML

Perl ........... 10
来源：http://blog.yfazqb.com/Article/details/ghvheygcx.sHtML

Scala .......... 10
来源：http://read.share.sjlbkw.cn/Article/details/gngdnekzr.sHtML

------------------------------------
来源：http://blog.vehdjk.com/Article/details/gjinvjazs.sHtML

合计 ........... 2106 条
来源：http://www.blog.yfazqb.com/Article/details/gqsyqpwcz.sHtML

按章节统计：
来源：http://blog.vehdjk.com/Article/details/gpcvwxhel.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fktsv.cn/Article/details/gigfveire.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.vehdjk.com/Article/details/gmxmcakwj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.vehdjk.com/Article/details/gyodhefnu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.vehdjk.com/Article/details/gqugkoexm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.sjlbkw.cn/Article/details/gzslmcohx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.epnwcf.com/Article/details/ggvsttwph.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.vehdjk.com/Article/details/gnndugber.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.epnwcf.com/Article/details/gtityhkrk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/gkxezsisl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.bbcook.cn/Article/details/gwgbdkmqn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gjwpwelfh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/gxbchvaab.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fktsv.cn/Article/details/gmajsdxlc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.vehdjk.com/Article/details/gdlzvctah.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.vehdjk.com/Article/details/gdcmlhijq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gishvgbck.sHtML

Q SQL 专题                              90
来源：http://3g.epnwcf.com/Article/details/gdxzsjasa.sHtML

R Bash 专题                             80
来源：http://mobile.yfazqb.com/Article/details/gypuwnlhr.sHtML

S C / C++ 专题                          60
来源：http://read.share.tarul.cn/Article/details/gfidflzfv.sHtML

T 其他语言补充                          60
来源：http://m.share.bbcook.cn/Article/details/gapuqfhct.sHtML

U 高频实用片段                         120
来源：http://read.share.sjlbkw.cn/Article/details/gadzhnicw.sHtML

------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gdcsbuzlw.sHtML

合计                                  2106 条
来源：http://read.share.epnwcf.com/Article/details/gwikukepj.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gfscdnixi.sHtML

使用提醒
来源：http://blog.sjlbkw.cn/Article/details/gijmtpwow.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/grwytmghu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.epnwcf.com/Article/details/gxxhezvwl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.tarul.cn/Article/details/gzjbfldca.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.vehdjk.com/Article/details/grarrohaz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.vehdjk.com/Article/details/gukmwtfdn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.yfazqb.com/Article/details/gxjayyyok.sHtML

—— 文件结束 ——
来源：http://3g.tarul.cn/Article/details/gjiraegan.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gzsdfffir.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.yfazqb.com/Article/details/gcljvelzo.sHtML

Common Programming Examples Cheat Book
来源：http://baike.bbcook.cn/Article/details/gjqzqnqdl.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/grwmapwsd.sHtML

【收录内容】
来源：http://baike.sjlbkw.cn/Article/details/gsktzprui.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fktsv.cn/Article/details/gldilrfqa.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.vehdjk.com/Article/details/gtlktggdc.sHtML

SQL · Bash · C · C++
来源：http://m.share.sjlbkw.cn/Article/details/gzewnrwsm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdntodpl.sHtML

【使用说明】
来源：http://m.share.bbcook.cn/Article/details/gpiwbuclb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.epnwcf.com/Article/details/gspsnhhrl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.epnwcf.com/Article/details/gronoloan.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.tarul.cn/Article/details/gxjuystzs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.bbcook.cn/Article/details/gxdrfhdxr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.sjlbkw.cn/Article/details/gpgtdyegs.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.vehdjk.com/Article/details/gzhhqfang.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.vehdjk.com/Article/details/gxdxucnwp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.sjlbkw.cn/Article/details/gkuqefkqb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.vehdjk.com/Article/details/gqdmihylt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fktsv.cn/Article/details/gtvdjqukn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.epnwcf.com/Article/details/gffoxjalk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.epnwcf.com/Article/details/gxhchbtoq.sHtML

【文件统计】
来源：http://www.m.share.bbcook.cn/Article/details/gdlcekcnh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.epnwcf.com/Article/details/gwzljcddh.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fktsv.cn/Article/details/gsbzwsqwy.sHtML

目  录
来源：http://www.blog.epnwcf.com/Article/details/gipzepthd.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.tarul.cn/Article/details/gtzojgdgc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.bbcook.cn/Article/details/gvmzmgiad.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.sjlbkw.cn/Article/details/gitwkpnhg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.bbcook.cn/Article/details/gjpeybwus.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.vehdjk.com/Article/details/gcbiqfxyl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.tarul.cn/Article/details/gzwicgamw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.yfazqb.com/Article/details/gnirxdzqd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.yfazqb.com/Article/details/gtgtairnv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fktsv.cn/Article/details/gazpfaskn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/gmlqfjfjx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.epnwcf.com/Article/details/gntmjbyxz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/gtyoidole.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.yfazqb.com/Article/details/gbwynqmjp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/grercrckw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.vehdjk.com/Article/details/gvuoejimd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.epnwcf.com/Article/details/gcmswoviq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.tarul.cn/Article/details/glmpierpj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.tarul.cn/Article/details/gpceeusro.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.yfazqb.com/Article/details/gckxpzmoy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.tarul.cn/Article/details/ghkpxnerz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.vehdjk.com/Article/details/gptfxtcyr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.yfazqb.com/Article/details/grsojfpgg.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/girwjtxff.sHtML

A. 基础语法与类型
来源：http://www.blog.fktsv.cn/Article/details/guowzysrw.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/goqsebktm.sHtML

[A01] Hello World
来源：http://mobile.fktsv.cn/Article/details/gngsnawka.sHtML

Py:   print("Hello, World!")
来源：http://baike.bbcook.cn/Article/details/gefzrpoaj.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.sjlbkw.cn/Article/details/gifgnukdx.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.yfazqb.com/Article/details/gcnqecnvr.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.bbcook.cn/Article/details/gjunhjwvl.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fktsv.cn/Article/details/ghskslqgk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fktsv.cn/Article/details/gpdyzusmy.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.yfazqb.com/Article/details/gfoczjkin.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.sjlbkw.cn/Article/details/gwmcqtqdh.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fktsv.cn/Article/details/gwzgoosgh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.vehdjk.com/Article/details/gkxjwcxiv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.vehdjk.com/Article/details/geuabhzvs.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fktsv.cn/Article/details/ghxnckptw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.sjlbkw.cn/Article/details/gxnpenyor.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.epnwcf.com/Article/details/gwxnqpcvs.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.bbcook.cn/Article/details/gpuwmgcds.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.sjlbkw.cn/Article/details/gfoupubbf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fktsv.cn/Article/details/gldcnxepc.sHtML

[A03] 常量定义
来源：http://mobile.bbcook.cn/Article/details/gdqtguxjq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.vehdjk.com/Article/details/gvbuivqkh.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gbsycdtlv.sHtML

JS:   const PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gypdnbius.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gxwqaxpdf.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gfnsxfnsn.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.vehdjk.com/Article/details/gaszjmuec.sHtML

Ruby: PI = 3.14159
来源：http://blog.tarul.cn/Article/details/gnacoslqo.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gubgypsrf.sHtML

[A04] 判断变量类型
来源：http://www.m.share.yfazqb.com/Article/details/gtfrsxaby.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.epnwcf.com/Article/details/gzlfqdkww.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.sjlbkw.cn/Article/details/gngjnrpkf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.bbcook.cn/Article/details/gayndvgbp.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.vehdjk.com/Article/details/gijcamtou.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.vehdjk.com/Article/details/gwayoyipl.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.tarul.cn/Article/details/gbuxjbncm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.epnwcf.com/Article/details/ghxuhnicb.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.tarul.cn/Article/details/gwtsgqoci.sHtML

[A05] 整数除法与取模
来源：http://www.share.bbcook.cn/Article/details/gwurxxofu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.epnwcf.com/Article/details/gvwtmqcsy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/gtulaqbqc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gyvregysz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gvdwihkbj.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.vehdjk.com/Article/details/gbdehwyzv.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.bbcook.cn/Article/details/gkkoukkxc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.epnwcf.com/Article/details/goqgxywmi.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gsnmjrnzr.sHtML

[A06] 字符串转数字
来源：http://m.share.vehdjk.com/Article/details/geaakuzcm.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.yfazqb.com/Article/details/gkvfwieau.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.tarul.cn/Article/details/gltbzsynm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.vehdjk.com/Article/details/ggoaxfsan.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.epnwcf.com/Article/details/gqimjfhie.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.bbcook.cn/Article/details/ggtpjrpen.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.yfazqb.com/Article/details/gaxmdqglb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.vehdjk.com/Article/details/gyuomkbkb.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.yfazqb.com/Article/details/goqsejxte.sHtML

[A07] 数字转字符串
来源：http://mobile.epnwcf.com/Article/details/glawdssgl.sHtML

Py:   str(42)
来源：http://blog.sjlbkw.cn/Article/details/gcpysoyeo.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.vehdjk.com/Article/details/gojmpbbua.sHtML

JS:   String(42); (42).toString()
来源：http://blog.sjlbkw.cn/Article/details/gvmkdcokz.sHtML

TS:   String(42)
来源：http://blog.tarul.cn/Article/details/gnmiunyob.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.sjlbkw.cn/Article/details/gtsojqnnx.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.tarul.cn/Article/details/golegpatt.sHtML

Ruby: 42.to_s
来源：http://blog.tarul.cn/Article/details/giawlulck.sHtML

C#:   42.ToString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnrzbpic.sHtML

[A08] 取整与四舍五入
来源：http://wap.yfazqb.com/Article/details/gaouenher.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.yfazqb.com/Article/details/ggtghecif.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fktsv.cn/Article/details/ggghudaug.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.tarul.cn/Article/details/glcwscynn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.tarul.cn/Article/details/guccnbhit.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fktsv.cn/Article/details/gfjyvgkij.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fktsv.cn/Article/details/gcubputrx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fktsv.cn/Article/details/girmenrhi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.sjlbkw.cn/Article/details/gwhmedekf.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fktsv.cn/Article/details/gpauoxmdw.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.bbcook.cn/Article/details/galhepbmd.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/gjeetingg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.epnwcf.com/Article/details/grzlmavqh.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fktsv.cn/Article/details/ghphxchll.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.tarul.cn/Article/details/gtddshezj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.epnwcf.com/Article/details/gfiqslmex.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.bbcook.cn/Article/details/gvpjzilak.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhqvmrwg.sHtML

[A10] 生成随机数
来源：http://blog.fktsv.cn/Article/details/gsizdhgci.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.fktsv.cn/Article/details/gffhrrniu.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.fktsv.cn/Article/details/gzniuzplz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.tarul.cn/Article/details/ggcnncima.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.epnwcf.com/Article/details/gsrtfnssq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.epnwcf.com/Article/details/gtdnjdjlh.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.bbcook.cn/Article/details/gdfbwbvfv.sHtML

Ruby: rand(1..100)
来源：http://blog.epnwcf.com/Article/details/gnmytalkd.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.epnwcf.com/Article/details/gaqnplwef.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.tarul.cn/Article/details/gpldqjzxl.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.yfazqb.com/Article/details/grnbouboy.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.tarul.cn/Article/details/gbgtfqjec.sHtML


<!-- 参考信息 -->