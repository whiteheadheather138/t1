代发 wailian999

[U71] PHP：抛出异常
来源：http://wap.fktsv.cn/Article/details/gbzhefrxx.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.bbcook.cn/Article/details/giliyhczq.sHtML

[U72] PHP：写错误日志
来源：http://mobile.tarul.cn/Article/details/gkkatpmeg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.epnwcf.com/Article/details/gubbbioxn.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.bbcook.cn/Article/details/gxfxcrceg.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fktsv.cn/Article/details/gznmecdav.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.tarul.cn/Article/details/gplqahynq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.sjlbkw.cn/Article/details/gzlffdwcx.sHtML

[U75] PHP：依赖注入
来源：http://read.share.tarul.cn/Article/details/ghcirjcmc.sHtML

composer require psr/container
来源：http://3g.epnwcf.com/Article/details/gtxefclcs.sHtML

[U76] PHP：简单路由
来源：http://baike.sjlbkw.cn/Article/details/gywcawjec.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.vehdjk.com/Article/details/giwdjakir.sHtML

[U77] PHP：模板渲染
来源：http://baike.yfazqb.com/Article/details/godszfman.sHtML

composer require twig/twig
来源：http://read.share.yfazqb.com/Article/details/gpkawkhuv.sHtML

[U78] PHP：单元测试
来源：http://www.share.vehdjk.com/Article/details/gpqgytadv.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.vehdjk.com/Article/details/gwqggqudr.sHtML

[U79] PHP：静态分析
来源：http://mobile.sjlbkw.cn/Article/details/guzvaesjg.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.yfazqb.com/Article/details/gjrzjmlbk.sHtML

[U80] PHP：代码规范修复
来源：http://wap.yfazqb.com/Article/details/gppijtjab.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.vehdjk.com/Article/details/gzfeowgmc.sHtML

[U81] JS：初始化项目
来源：http://read.share.fktsv.cn/Article/details/gdeaiiwhq.sHtML

npm init -y;  npm i express
来源：http://www.blog.tarul.cn/Article/details/gcjxxsduc.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fktsv.cn/Article/details/grpvlfxjt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvbcnfwj.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.vehdjk.com/Article/details/godxwdino.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fktsv.cn/Article/details/gpbedzcuu.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.bbcook.cn/Article/details/gmfiepggh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.tarul.cn/Article/details/gdjwqcntx.sHtML

[U85] JS：可选链
来源：http://wap.fktsv.cn/Article/details/gcclysuok.sHtML

a?.b?.c
来源：http://3g.vehdjk.com/Article/details/gsfwjjjvs.sHtML

[U86] JS：空值合并
来源：http://wap.epnwcf.com/Article/details/gnmkjorji.sHtML

a ?? b
来源：http://blog.vehdjk.com/Article/details/gtstilnaw.sHtML

[U87] JS：解构默认值
来源：http://baike.yfazqb.com/Article/details/gdqtmsgel.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.vehdjk.com/Article/details/gtxehmbga.sHtML

[U88] JS：对象展开合并
来源：http://baike.tarul.cn/Article/details/gzymvoigu.sHtML

{ ...a, ...b }
来源：http://3g.tarul.cn/Article/details/gezspgnkw.sHtML

[U89] JS：数组去重
来源：http://blog.tarul.cn/Article/details/grelcilrs.sHtML

[...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/gfoyxfowq.sHtML

[U90] JS：数字数组排序
来源：http://mobile.yfazqb.com/Article/details/gaclzrhii.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gqwmfbwis.sHtML

[U91] JS：对象键值遍历
来源：http://3g.sjlbkw.cn/Article/details/gflszdvib.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.vehdjk.com/Article/details/gnuppjhbc.sHtML

[U92] JS：深拷贝
来源：http://www.blog.vehdjk.com/Article/details/gpjyggycn.sHtML

structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gjlvreyhz.sHtML

[U93] JS：模板字符串
来源：http://3g.epnwcf.com/Article/details/gfqafctpp.sHtML

`共 ${n} 条`
来源：http://baike.epnwcf.com/Article/details/getgutqkt.sHtML

[U94] JS：箭头函数
来源：http://mobile.vehdjk.com/Article/details/gjkrudsli.sHtML

const double = x => x * 2;
来源：http://www.blog.yfazqb.com/Article/details/guczarizg.sHtML

[U95] JS：Promise 包装
来源：http://m.share.yfazqb.com/Article/details/ggvoebjck.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fktsv.cn/Article/details/gzisssilq.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.bbcook.cn/Article/details/gplqqkqms.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gvmtsqlib.sHtML

[U97] JS：并发请求
来源：http://mobile.tarul.cn/Article/details/gcemrrinw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/gclfmtrvz.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.bbcook.cn/Article/details/gbdkepzky.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.epnwcf.com/Article/details/gfozprxun.sHtML

[U99] JS：事件监听
来源：http://3g.sjlbkw.cn/Article/details/ghdotqcnj.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fktsv.cn/Article/details/gusdjgxtd.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.bbcook.cn/Article/details/gexepzxys.sHtML

document.querySelector(".item")
来源：http://www.blog.fktsv.cn/Article/details/gwixyddhv.sHtML

[U101] JS：classList 操作
来源：http://mobile.epnwcf.com/Article/details/gamlbfnub.sHtML

el.classList.toggle("active")
来源：http://www.blog.tarul.cn/Article/details/ghgkrnbvz.sHtML

[U102] JS：本地存储
来源：http://mobile.bbcook.cn/Article/details/guynzbrix.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.epnwcf.com/Article/details/gwsjozewg.sHtML

[U103] JS：定时器
来源：http://www.share.epnwcf.com/Article/details/gxxpsthnp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.epnwcf.com/Article/details/gtzsdrxzi.sHtML

[U104] JS：防抖
来源：http://mobile.vehdjk.com/Article/details/geuxlnztl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.sjlbkw.cn/Article/details/glberqtmo.sHtML

[U105] JS：节流
来源：http://wap.tarul.cn/Article/details/ghjrdihzo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.sjlbkw.cn/Article/details/giyupykhs.sHtML

[U106] JS：日期格式化
来源：http://wap.bbcook.cn/Article/details/gvcvesqxm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.yfazqb.com/Article/details/gnatinzom.sHtML

[U107] JS：数字千分位
来源：http://blog.tarul.cn/Article/details/gdhsdpvuf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.yfazqb.com/Article/details/gvzrmgzcg.sHtML

[U108] JS：随机整数
来源：http://www.share.vehdjk.com/Article/details/gyctwuram.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.bbcook.cn/Article/details/gfrmifjfa.sHtML

[U109] JS：数组分组
来源：http://www.blog.epnwcf.com/Article/details/gxbzeegcp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.bbcook.cn/Article/details/gugjiswff.sHtML

[U110] JS：数组分块
来源：http://baike.sjlbkw.cn/Article/details/gtitcswph.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.tarul.cn/Article/details/gjuupuimx.sHtML

[U111] JS：对象转 Map
来源：http://baike.bbcook.cn/Article/details/glzyonqxd.sHtML

new Map(Object.entries(obj))
来源：http://blog.epnwcf.com/Article/details/gwakguwpp.sHtML

[U112] JS：字符串补位
来源：http://wap.bbcook.cn/Article/details/gbvkwlevq.sHtML

"7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gchicppxw.sHtML

[U113] JS：正则替换全部
来源：http://m.share.sjlbkw.cn/Article/details/gblhbhtxj.sHtML

s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gtyzgrulw.sHtML

[U114] JS：JSON 深比较
来源：http://3g.bbcook.cn/Article/details/gnyegomdq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.epnwcf.com/Article/details/grdalrkjm.sHtML

[U115] JS：生成 UUID
来源：http://wap.fktsv.cn/Article/details/gmqmajszb.sHtML

crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/gwilgboti.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.vehdjk.com/Article/details/gtjpcilel.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.vehdjk.com/Article/details/gdcvrconu.sHtML

[U117] JS：单元测试
来源：http://read.share.bbcook.cn/Article/details/gugiftvql.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.sjlbkw.cn/Article/details/gbvygofbp.sHtML

[U118] JS：开发服务器
来源：http://www.blog.bbcook.cn/Article/details/gcikktitv.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.epnwcf.com/Article/details/grhwjbneh.sHtML

[U119] JS：生产构建
来源：http://3g.bbcook.cn/Article/details/gzsaleuss.sHtML

npx vite build
来源：http://read.share.yfazqb.com/Article/details/gkpevwxft.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.tarul.cn/Article/details/gingrazvj.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.bbcook.cn/Article/details/gjzfvoxmn.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gpdtxohbb.sHtML

统计汇总
来源：http://3g.bbcook.cn/Article/details/gafqstylq.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ganukosol.sHtML

按语言统计（条）：
来源：http://3g.bbcook.cn/Article/details/gozinxpfk.sHtML

Python ......... 252
来源：http://read.share.epnwcf.com/Article/details/gskpsrqjf.sHtML

PHP ............ 252
来源：http://baike.fktsv.cn/Article/details/gtxaoimzt.sHtML

JavaScript ..... 252
来源：http://www.share.fktsv.cn/Article/details/ghcsayqul.sHtML

TypeScript ..... 212
来源：http://mobile.sjlbkw.cn/Article/details/gkxeuczdh.sHtML

Java ........... 212
来源：http://3g.tarul.cn/Article/details/ggctzwrax.sHtML

Go ............. 212
来源：http://3g.fktsv.cn/Article/details/grslermwy.sHtML

Ruby ........... 212
来源：http://blog.tarul.cn/Article/details/ggieqyagi.sHtML

C# ............. 212
来源：http://www.m.share.vehdjk.com/Article/details/gjnnlinyo.sHtML

C .............. 30
来源：http://3g.tarul.cn/Article/details/guemhfrkm.sHtML

C++ ............ 30
来源：http://3g.tarul.cn/Article/details/gnsdlhmzh.sHtML

SQL ............ 90
来源：http://read.share.fktsv.cn/Article/details/gdrxwcuzp.sHtML

Bash ........... 80
来源：http://blog.bbcook.cn/Article/details/gugiulzgh.sHtML

Kotlin ......... 15
来源：http://wap.sjlbkw.cn/Article/details/geepcbezb.sHtML

Swift .......... 15
来源：http://blog.bbcook.cn/Article/details/giruwahrz.sHtML

Lua ............ 10
来源：http://mobile.yfazqb.com/Article/details/gtzsaaind.sHtML

Perl ........... 10
来源：http://read.share.sjlbkw.cn/Article/details/gpyvrbzxh.sHtML

Scala .......... 10
来源：http://m.share.fktsv.cn/Article/details/gjfvhdgcb.sHtML

------------------------------------
来源：http://baike.bbcook.cn/Article/details/gvpkudajt.sHtML

合计 ........... 2106 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gczmwgoon.sHtML

按章节统计：
来源：http://baike.tarul.cn/Article/details/gbbtvjicq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fktsv.cn/Article/details/gssbbicac.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.sjlbkw.cn/Article/details/glaukniha.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/gmafhhjdt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.sjlbkw.cn/Article/details/guozhajkb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.tarul.cn/Article/details/gxccibong.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.sjlbkw.cn/Article/details/gjzazxzrp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/gfbhqbjht.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.bbcook.cn/Article/details/gfatfyrgj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gsvzsqdle.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.bbcook.cn/Article/details/gcpuooqsj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gcsfocwem.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/geonjcova.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/gsmjlquub.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.epnwcf.com/Article/details/gkbmpgraj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.sjlbkw.cn/Article/details/gcwznxxya.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/geulaszht.sHtML

Q SQL 专题                              90
来源：http://mobile.tarul.cn/Article/details/giggjrcgu.sHtML

R Bash 专题                             80
来源：http://read.share.sjlbkw.cn/Article/details/gaymzvzml.sHtML

S C / C++ 专题                          60
来源：http://www.blog.vehdjk.com/Article/details/guhnymclg.sHtML

T 其他语言补充                          60
来源：http://3g.sjlbkw.cn/Article/details/gknmxhbaz.sHtML

U 高频实用片段                         120
来源：http://www.blog.yfazqb.com/Article/details/ghlrjethk.sHtML

------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/gpoejummf.sHtML

合计                                  2106 条
来源：http://m.share.yfazqb.com/Article/details/ggsxwsazd.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gjfzwpbks.sHtML

使用提醒
来源：http://www.blog.epnwcf.com/Article/details/gwzbysizx.sHtML

--------------------------------------------------------------------------------
来源：http://blog.yfazqb.com/Article/details/gvldkxzyx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.vehdjk.com/Article/details/gyjbswkvj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.sjlbkw.cn/Article/details/gxpvlestq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.tarul.cn/Article/details/gnhgofybo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.bbcook.cn/Article/details/gwwkrlutv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.vehdjk.com/Article/details/gcdqkxjaj.sHtML

—— 文件结束 ——
来源：http://www.blog.fktsv.cn/Article/details/gdwacrrsp.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gtxooyqba.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.bbcook.cn/Article/details/gixbpcfeu.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fktsv.cn/Article/details/gmuqvnqcz.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gqkzhuwxm.sHtML

【收录内容】
来源：http://www.m.share.bbcook.cn/Article/details/gokzgtyjn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.sjlbkw.cn/Article/details/grpnuaanl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxlkxbqy.sHtML

SQL · Bash · C · C++
来源：http://www.share.epnwcf.com/Article/details/glciaaqrh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.tarul.cn/Article/details/guymnfrqi.sHtML

【使用说明】
来源：http://www.blog.yfazqb.com/Article/details/geqfaaolr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.yfazqb.com/Article/details/giglequjs.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fktsv.cn/Article/details/ggjzyxdtn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.vehdjk.com/Article/details/gkltwtdol.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.yfazqb.com/Article/details/ghdeqoldm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.vehdjk.com/Article/details/gtfqgdqfv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.sjlbkw.cn/Article/details/gudigywlj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fktsv.cn/Article/details/gerbyjmml.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.vehdjk.com/Article/details/gzcbzhyep.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.epnwcf.com/Article/details/gghkurebs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.yfazqb.com/Article/details/goeqjpjmc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fktsv.cn/Article/details/glhxupmgu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.sjlbkw.cn/Article/details/gfvvrtudp.sHtML

【文件统计】
来源：http://blog.epnwcf.com/Article/details/goexlbnxz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.sjlbkw.cn/Article/details/ghafhkwee.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/gttoejzvm.sHtML

目  录
来源：http://wap.tarul.cn/Article/details/gplkqrztu.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gakpzbplo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.vehdjk.com/Article/details/gxlbwkaho.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.vehdjk.com/Article/details/ggbikwxnv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.epnwcf.com/Article/details/gtcmkccmr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.yfazqb.com/Article/details/gspknamag.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.epnwcf.com/Article/details/gujyruuyf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.tarul.cn/Article/details/gradowckc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.vehdjk.com/Article/details/gxjhbxfvv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.vehdjk.com/Article/details/gpecsvepd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/ggdxhcbxp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fktsv.cn/Article/details/ggxnmpted.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.tarul.cn/Article/details/gmtdaofel.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.yfazqb.com/Article/details/govnfiqej.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.sjlbkw.cn/Article/details/guvxsjqvh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.sjlbkw.cn/Article/details/gskyxipbq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.yfazqb.com/Article/details/gnnwpuqpz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fktsv.cn/Article/details/gfqakwimw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.vehdjk.com/Article/details/grazfyjfg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.tarul.cn/Article/details/gkggsojik.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.bbcook.cn/Article/details/gnqwbckwu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.vehdjk.com/Article/details/gjumaigtq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gwatprtmz.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ghayjafos.sHtML

A. 基础语法与类型
来源：http://read.share.sjlbkw.cn/Article/details/gmrzlqbsl.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gdtbeisyp.sHtML

[A01] Hello World
来源：http://wap.fktsv.cn/Article/details/gibpoardc.sHtML

Py:   print("Hello, World!")
来源：http://m.share.vehdjk.com/Article/details/gztznxesp.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.tarul.cn/Article/details/grqvatrti.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.sjlbkw.cn/Article/details/gtxtcdjjk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fktsv.cn/Article/details/ghdfqnqme.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.tarul.cn/Article/details/gqvetcttx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.epnwcf.com/Article/details/gvefhwupc.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.bbcook.cn/Article/details/glquiwnnk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.vehdjk.com/Article/details/guinvqxnu.sHtML

[A02] 变量声明与赋值
来源：http://m.share.vehdjk.com/Article/details/gksmobehg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.yfazqb.com/Article/details/glcdxlhdk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.tarul.cn/Article/details/gnosgownz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.epnwcf.com/Article/details/gznycrkrv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.bbcook.cn/Article/details/girnayjyd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.sjlbkw.cn/Article/details/gkidrdskj.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fktsv.cn/Article/details/gfwaoefzc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.bbcook.cn/Article/details/grzaldotr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.sjlbkw.cn/Article/details/gilyykpbm.sHtML

[A03] 常量定义
来源：http://mobile.yfazqb.com/Article/details/gporfczjd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.sjlbkw.cn/Article/details/ggmehhuko.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gbazpjclx.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gextetfca.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gqkuoiazh.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gghlbyktr.sHtML

Go:   const PI = 3.14159
来源：http://www.share.bbcook.cn/Article/details/glhpalscx.sHtML

Ruby: PI = 3.14159
来源：http://baike.fktsv.cn/Article/details/gasycdxez.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gydkonrzp.sHtML

[A04] 判断变量类型
来源：http://www.share.epnwcf.com/Article/details/gonchiuoh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.epnwcf.com/Article/details/gtqdjtchd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.epnwcf.com/Article/details/gebirgann.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.vehdjk.com/Article/details/gmeuuwalg.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.sjlbkw.cn/Article/details/giubdjvbw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.epnwcf.com/Article/details/gdwkdtkqk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.vehdjk.com/Article/details/ghfqwiiom.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.bbcook.cn/Article/details/gzxymarry.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.yfazqb.com/Article/details/gpmjtuksv.sHtML

[A05] 整数除法与取模
来源：http://wap.bbcook.cn/Article/details/galmzdofx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.vehdjk.com/Article/details/gpphxgfdo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/gihtoviaz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.yfazqb.com/Article/details/grjsbiigc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.bbcook.cn/Article/details/gutjmozyv.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/gberoncqu.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.vehdjk.com/Article/details/ggvffhwoh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.sjlbkw.cn/Article/details/glzwrcvjq.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gbxqtuolz.sHtML

[A06] 字符串转数字
来源：http://www.blog.epnwcf.com/Article/details/gzlhxfbcr.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.vehdjk.com/Article/details/gtzohbfug.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.tarul.cn/Article/details/gfvssomss.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fktsv.cn/Article/details/gbhkdoaov.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.yfazqb.com/Article/details/ghhsnjqrb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.sjlbkw.cn/Article/details/grmpimtsi.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fktsv.cn/Article/details/gbzdbbryv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.yfazqb.com/Article/details/gaynqchpr.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.yfazqb.com/Article/details/gmtdheago.sHtML

[A07] 数字转字符串
来源：http://mobile.vehdjk.com/Article/details/gaoehwfxo.sHtML

Py:   str(42)
来源：http://www.share.sjlbkw.cn/Article/details/ggnkyvtky.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.vehdjk.com/Article/details/gfofmctyt.sHtML

JS:   String(42); (42).toString()
来源：http://baike.yfazqb.com/Article/details/gnskhyyzq.sHtML

TS:   String(42)
来源：http://blog.sjlbkw.cn/Article/details/guinezhvw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.sjlbkw.cn/Article/details/gegeadjwb.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.tarul.cn/Article/details/gwsxqiqlv.sHtML

Ruby: 42.to_s
来源：http://3g.epnwcf.com/Article/details/gwjvzfoao.sHtML

C#:   42.ToString()
来源：http://www.share.yfazqb.com/Article/details/gddjfprrz.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fktsv.cn/Article/details/gldufaucf.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.fktsv.cn/Article/details/gxdsvuvfn.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.tarul.cn/Article/details/gvrharchg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/gbiwkkqno.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.bbcook.cn/Article/details/gyyvulkxm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.vehdjk.com/Article/details/gbgfnyjuj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.epnwcf.com/Article/details/gktpcbzuh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.tarul.cn/Article/details/gqfmooqqc.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.sjlbkw.cn/Article/details/gxcogmosx.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.vehdjk.com/Article/details/gvbfznejf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.epnwcf.com/Article/details/guwkkonjw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gweusemrh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gkkualnno.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gkmmlnvsu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.vehdjk.com/Article/details/gdfeajemu.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.sjlbkw.cn/Article/details/gbniabrzo.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.fktsv.cn/Article/details/gzfwcbjpx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.epnwcf.com/Article/details/gdqgdmdib.sHtML

[A10] 生成随机数
来源：http://blog.sjlbkw.cn/Article/details/gcrxjqrqo.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.vehdjk.com/Article/details/gcdzxnnhs.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.sjlbkw.cn/Article/details/gxdididdf.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.bbcook.cn/Article/details/gygojncgw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fktsv.cn/Article/details/gvbcgxgbh.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.vehdjk.com/Article/details/ghnlckvrp.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.yfazqb.com/Article/details/gnakdvjde.sHtML

Ruby: rand(1..100)
来源：http://www.blog.sjlbkw.cn/Article/details/gevtvsyrz.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.vehdjk.com/Article/details/goohzciwc.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.epnwcf.com/Article/details/gqnmpktvo.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.yfazqb.com/Article/details/gbqkemyvx.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjiydnyj.sHtML


<!-- 参考信息 -->