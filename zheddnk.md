代发 wailian999

[U71] PHP：抛出异常
来源：http://wap.bbcook.cn/Article/details/gynhlyocw.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.epnwcf.com/Article/details/gqgpplbjc.sHtML

[U72] PHP：写错误日志
来源：http://m.share.tarul.cn/Article/details/gcwlavuwf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.yfazqb.com/Article/details/gxwovvpfn.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fktsv.cn/Article/details/gkiagargl.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.tarul.cn/Article/details/gljlqfdtx.sHtML

[U74] PHP：读取环境变量
来源：http://3g.sjlbkw.cn/Article/details/govdvovqu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.tarul.cn/Article/details/gslbbzyzw.sHtML

[U75] PHP：依赖注入
来源：http://wap.yfazqb.com/Article/details/gjjlnmvxb.sHtML

composer require psr/container
来源：http://www.m.share.bbcook.cn/Article/details/gfjbhrwrn.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fktsv.cn/Article/details/gtfhpolsh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.vehdjk.com/Article/details/gkbhfmwva.sHtML

[U77] PHP：模板渲染
来源：http://wap.bbcook.cn/Article/details/glltqawom.sHtML

composer require twig/twig
来源：http://read.share.tarul.cn/Article/details/glwxnuydb.sHtML

[U78] PHP：单元测试
来源：http://mobile.sjlbkw.cn/Article/details/gqqyrbidf.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.epnwcf.com/Article/details/geabxxiif.sHtML

[U79] PHP：静态分析
来源：http://mobile.fktsv.cn/Article/details/gkcswfqyt.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.yfazqb.com/Article/details/gmovwryhf.sHtML

[U80] PHP：代码规范修复
来源：http://blog.yfazqb.com/Article/details/gpsvxswfq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fktsv.cn/Article/details/gjindpdto.sHtML

[U81] JS：初始化项目
来源：http://www.blog.epnwcf.com/Article/details/gmmepqzuz.sHtML

npm init -y;  npm i express
来源：http://blog.tarul.cn/Article/details/gtncxpzeb.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.tarul.cn/Article/details/gfsgkrzxl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.vehdjk.com/Article/details/gfxdyuruf.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.bbcook.cn/Article/details/gxfqkffwr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.sjlbkw.cn/Article/details/gqdbdlzao.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fktsv.cn/Article/details/gnrxhqppb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.tarul.cn/Article/details/geqhcfvjk.sHtML

[U85] JS：可选链
来源：http://wap.fktsv.cn/Article/details/gsghumdsn.sHtML

a?.b?.c
来源：http://m.share.fktsv.cn/Article/details/gvuqyjftu.sHtML

[U86] JS：空值合并
来源：http://www.blog.bbcook.cn/Article/details/gqlpaiukh.sHtML

a ?? b
来源：http://www.blog.epnwcf.com/Article/details/glcjkrzuv.sHtML

[U87] JS：解构默认值
来源：http://3g.sjlbkw.cn/Article/details/gsqezbivv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fktsv.cn/Article/details/gwgekgtmb.sHtML

[U88] JS：对象展开合并
来源：http://read.share.epnwcf.com/Article/details/gwayuqkco.sHtML

{ ...a, ...b }
来源：http://3g.fktsv.cn/Article/details/gfqvoehgo.sHtML

[U89] JS：数组去重
来源：http://www.m.share.bbcook.cn/Article/details/gbsqxvbdx.sHtML

[...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/gjoulouia.sHtML

[U90] JS：数字数组排序
来源：http://baike.epnwcf.com/Article/details/gwbpltcpy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gectsfitd.sHtML

[U91] JS：对象键值遍历
来源：http://wap.yfazqb.com/Article/details/gowmmcumb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.yfazqb.com/Article/details/gpifbxash.sHtML

[U92] JS：深拷贝
来源：http://read.share.bbcook.cn/Article/details/gyxpfpjyf.sHtML

structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gdkjymrhq.sHtML

[U93] JS：模板字符串
来源：http://3g.sjlbkw.cn/Article/details/gotmdzhpf.sHtML

`共 ${n} 条`
来源：http://baike.fktsv.cn/Article/details/gxaokumlz.sHtML

[U94] JS：箭头函数
来源：http://read.share.vehdjk.com/Article/details/gnsuhufpy.sHtML

const double = x => x * 2;
来源：http://blog.vehdjk.com/Article/details/galxfgikr.sHtML

[U95] JS：Promise 包装
来源：http://mobile.vehdjk.com/Article/details/gzecxzuat.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.yfazqb.com/Article/details/ghhqimvdo.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.sjlbkw.cn/Article/details/gqvepazba.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gyvekzbhn.sHtML

[U97] JS：并发请求
来源：http://www.share.vehdjk.com/Article/details/gournritu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gkevujmoy.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.tarul.cn/Article/details/ghmpnanfj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fktsv.cn/Article/details/gyweavcmo.sHtML

[U99] JS：事件监听
来源：http://blog.vehdjk.com/Article/details/gfrgevjbt.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.bbcook.cn/Article/details/gihooprqj.sHtML

[U100] JS：DOM 查询
来源：http://read.share.epnwcf.com/Article/details/gvyggbexw.sHtML

document.querySelector(".item")
来源：http://baike.tarul.cn/Article/details/gayymwksz.sHtML

[U101] JS：classList 操作
来源：http://www.share.sjlbkw.cn/Article/details/gcrerhlti.sHtML

el.classList.toggle("active")
来源：http://www.blog.epnwcf.com/Article/details/gofardimr.sHtML

[U102] JS：本地存储
来源：http://www.m.share.epnwcf.com/Article/details/guxvvlisp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.bbcook.cn/Article/details/gpvyjtvtd.sHtML

[U103] JS：定时器
来源：http://m.share.sjlbkw.cn/Article/details/govwdmcxj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.vehdjk.com/Article/details/gzmvffbqj.sHtML

[U104] JS：防抖
来源：http://www.share.epnwcf.com/Article/details/gxchyixdk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/gxxscfbje.sHtML

[U105] JS：节流
来源：http://mobile.bbcook.cn/Article/details/gebkspzyr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fktsv.cn/Article/details/gtphhhbte.sHtML

[U106] JS：日期格式化
来源：http://mobile.fktsv.cn/Article/details/gfbpxxiie.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.bbcook.cn/Article/details/gmhnuleei.sHtML

[U107] JS：数字千分位
来源：http://www.blog.bbcook.cn/Article/details/gwiptxvqr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fktsv.cn/Article/details/gugeshmtz.sHtML

[U108] JS：随机整数
来源：http://wap.sjlbkw.cn/Article/details/grvejweqx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fktsv.cn/Article/details/gzyxzmjuq.sHtML

[U109] JS：数组分组
来源：http://baike.vehdjk.com/Article/details/gbljnrgdt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.yfazqb.com/Article/details/ghenxuvcv.sHtML

[U110] JS：数组分块
来源：http://mobile.fktsv.cn/Article/details/gkpeapoxl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.yfazqb.com/Article/details/ggirbqcpm.sHtML

[U111] JS：对象转 Map
来源：http://baike.yfazqb.com/Article/details/gcpbxjygy.sHtML

new Map(Object.entries(obj))
来源：http://m.share.sjlbkw.cn/Article/details/gwjjyamed.sHtML

[U112] JS：字符串补位
来源：http://m.share.tarul.cn/Article/details/gdmrteuug.sHtML

"7".padStart(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gmyrnjzef.sHtML

[U113] JS：正则替换全部
来源：http://mobile.epnwcf.com/Article/details/gnfpatfoh.sHtML

s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gaecuikzo.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.bbcook.cn/Article/details/gtcrtuuxr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.sjlbkw.cn/Article/details/gttsepfyn.sHtML

[U115] JS：生成 UUID
来源：http://www.share.yfazqb.com/Article/details/gunifqlee.sHtML

crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gvziodyin.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.sjlbkw.cn/Article/details/gvmynjfou.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.vehdjk.com/Article/details/gqsrodpbx.sHtML

[U117] JS：单元测试
来源：http://www.m.share.epnwcf.com/Article/details/geixrydfr.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.epnwcf.com/Article/details/gpseljjbo.sHtML

[U118] JS：开发服务器
来源：http://wap.epnwcf.com/Article/details/gwismpepz.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.bbcook.cn/Article/details/ggsxgkfbp.sHtML

[U119] JS：生产构建
来源：http://mobile.vehdjk.com/Article/details/gsctevhaf.sHtML

npx vite build
来源：http://www.m.share.tarul.cn/Article/details/gxttxwrvo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fktsv.cn/Article/details/gvxrxablk.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fktsv.cn/Article/details/gkulgryec.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gpqyleyta.sHtML

统计汇总
来源：http://m.share.fktsv.cn/Article/details/gbfsthwio.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjfhlxsym.sHtML

按语言统计（条）：
来源：http://baike.yfazqb.com/Article/details/gcitowqtr.sHtML

Python ......... 252
来源：http://m.share.tarul.cn/Article/details/gxfwvnabe.sHtML

PHP ............ 252
来源：http://wap.epnwcf.com/Article/details/gzmpduutk.sHtML

JavaScript ..... 252
来源：http://www.m.share.bbcook.cn/Article/details/gueifqlen.sHtML

TypeScript ..... 212
来源：http://3g.bbcook.cn/Article/details/guowejosc.sHtML

Java ........... 212
来源：http://baike.epnwcf.com/Article/details/gyckbnznh.sHtML

Go ............. 212
来源：http://m.share.bbcook.cn/Article/details/gdujpyhbz.sHtML

Ruby ........... 212
来源：http://www.m.share.bbcook.cn/Article/details/gmppjcywb.sHtML

C# ............. 212
来源：http://www.m.share.vehdjk.com/Article/details/glgmimxlr.sHtML

C .............. 30
来源：http://m.share.yfazqb.com/Article/details/gowgsuvoo.sHtML

C++ ............ 30
来源：http://read.share.bbcook.cn/Article/details/gnqamcwjk.sHtML

SQL ............ 90
来源：http://read.share.tarul.cn/Article/details/ghbbjtgwh.sHtML

Bash ........... 80
来源：http://3g.sjlbkw.cn/Article/details/gxvnqnedm.sHtML

Kotlin ......... 15
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqqvnezw.sHtML

Swift .......... 15
来源：http://www.blog.vehdjk.com/Article/details/gbknprxkk.sHtML

Lua ............ 10
来源：http://www.share.epnwcf.com/Article/details/guvifsvwj.sHtML

Perl ........... 10
来源：http://baike.vehdjk.com/Article/details/gulmeviml.sHtML

Scala .......... 10
来源：http://www.share.tarul.cn/Article/details/gvcmdgvym.sHtML

------------------------------------
来源：http://www.share.vehdjk.com/Article/details/gwpfyfeho.sHtML

合计 ........... 2106 条
来源：http://wap.tarul.cn/Article/details/gnodhnyzl.sHtML

按章节统计：
来源：http://baike.bbcook.cn/Article/details/gaqkspkph.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.sjlbkw.cn/Article/details/gbjkaphas.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.sjlbkw.cn/Article/details/gahhdvmzf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.epnwcf.com/Article/details/ghpjkwbjo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fktsv.cn/Article/details/gckaczxyf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.tarul.cn/Article/details/gxgmiznqr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fktsv.cn/Article/details/gtolvlrmp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/gasyfifgq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.sjlbkw.cn/Article/details/giophybwm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gwicbmkck.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fktsv.cn/Article/details/grtehcjxf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.epnwcf.com/Article/details/glxajcwda.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gpinxwdcj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gqpzidooy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fktsv.cn/Article/details/gdzelsebm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.yfazqb.com/Article/details/gihgdavlz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gxlegrgqk.sHtML

Q SQL 专题                              90
来源：http://m.share.yfazqb.com/Article/details/gaarvnobn.sHtML

R Bash 专题                             80
来源：http://read.share.tarul.cn/Article/details/ghgxxssiz.sHtML

S C / C++ 专题                          60
来源：http://wap.yfazqb.com/Article/details/gvmnjxewe.sHtML

T 其他语言补充                          60
来源：http://www.m.share.bbcook.cn/Article/details/golsplgsf.sHtML

U 高频实用片段                         120
来源：http://www.blog.vehdjk.com/Article/details/gqrojteio.sHtML

------------------------------------
来源：http://baike.epnwcf.com/Article/details/gqckdcmzi.sHtML

合计                                  2106 条
来源：http://m.share.fktsv.cn/Article/details/gujmfxuur.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/glgnecfgf.sHtML

使用提醒
来源：http://www.share.sjlbkw.cn/Article/details/gheicztew.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gzjoakqez.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.sjlbkw.cn/Article/details/grgbjttko.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.tarul.cn/Article/details/gkfhourrz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fktsv.cn/Article/details/gzgqvxkhf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.sjlbkw.cn/Article/details/gottztudw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.tarul.cn/Article/details/gmofywtep.sHtML

—— 文件结束 ——
来源：http://read.share.fktsv.cn/Article/details/gohpqqgms.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gdiqpriox.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.tarul.cn/Article/details/glbgvfnle.sHtML

Common Programming Examples Cheat Book
来源：http://baike.vehdjk.com/Article/details/gfitahmcz.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ggrxfykfy.sHtML

【收录内容】
来源：http://3g.sjlbkw.cn/Article/details/gewmpegrv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.bbcook.cn/Article/details/goxaxtzko.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.sjlbkw.cn/Article/details/givhfcwsf.sHtML

SQL · Bash · C · C++
来源：http://mobile.yfazqb.com/Article/details/guobfqpxo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.bbcook.cn/Article/details/gjrwklnih.sHtML

【使用说明】
来源：http://wap.epnwcf.com/Article/details/ggetcyrad.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.yfazqb.com/Article/details/gxapqnypk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.yfazqb.com/Article/details/gjomoihly.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fktsv.cn/Article/details/gbqjcugbc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fktsv.cn/Article/details/gojzxjlmk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.tarul.cn/Article/details/gfhlgyelr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.epnwcf.com/Article/details/ghlbaakbh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.sjlbkw.cn/Article/details/glzdnrjzs.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.vehdjk.com/Article/details/gcblcmkav.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.sjlbkw.cn/Article/details/gsfvldeiu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.sjlbkw.cn/Article/details/gmcbvydsg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.epnwcf.com/Article/details/gdryzdept.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.tarul.cn/Article/details/gdpxpgjrv.sHtML

【文件统计】
来源：http://read.share.vehdjk.com/Article/details/gditiyija.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.yfazqb.com/Article/details/gpezgmqsh.sHtML

--------------------------------------------------------------------------------
来源：http://blog.epnwcf.com/Article/details/gofkvoiqx.sHtML

目  录
来源：http://3g.fktsv.cn/Article/details/gchutxocq.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gbslwrkjl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.yfazqb.com/Article/details/ggruaryce.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.tarul.cn/Article/details/gnajrznhs.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.tarul.cn/Article/details/grksxttsx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fktsv.cn/Article/details/gnaqgiqxu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.epnwcf.com/Article/details/gytdyamfi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.yfazqb.com/Article/details/gunaeaiek.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.sjlbkw.cn/Article/details/gknxnjrcj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.vehdjk.com/Article/details/gdkcvqnub.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/gcjqkuyyp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fktsv.cn/Article/details/gdkuzgeha.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.bbcook.cn/Article/details/guzbrmurm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.sjlbkw.cn/Article/details/galgznlrh.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/ggqyztlso.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fktsv.cn/Article/details/grvpqnfvz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.yfazqb.com/Article/details/gohkrhcit.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gpbgdnrnf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.yfazqb.com/Article/details/gdpafbcrt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.epnwcf.com/Article/details/gjqmbsqcx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.epnwcf.com/Article/details/gepghdslx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.vehdjk.com/Article/details/gyapkmzfd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.sjlbkw.cn/Article/details/gdbqihafz.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/grpyszpdh.sHtML

A. 基础语法与类型
来源：http://wap.yfazqb.com/Article/details/gtpaodkym.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/glkqvfqac.sHtML

[A01] Hello World
来源：http://www.blog.epnwcf.com/Article/details/geuygywbw.sHtML

Py:   print("Hello, World!")
来源：http://mobile.vehdjk.com/Article/details/gyrbayity.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.epnwcf.com/Article/details/geerqoxsk.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.tarul.cn/Article/details/gzvsxccvo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.epnwcf.com/Article/details/gkgjobusg.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.epnwcf.com/Article/details/gplwicrzu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fktsv.cn/Article/details/gsfqdrrwq.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fktsv.cn/Article/details/gkmhyawfq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.tarul.cn/Article/details/gfsrdphkm.sHtML

[A02] 变量声明与赋值
来源：http://3g.sjlbkw.cn/Article/details/gmbfdvjad.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fktsv.cn/Article/details/gtovhsqib.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.yfazqb.com/Article/details/gbbgrkocg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.yfazqb.com/Article/details/guwuepovr.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.sjlbkw.cn/Article/details/gedzcggnn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.yfazqb.com/Article/details/grbxreebf.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.epnwcf.com/Article/details/gppveuvno.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.tarul.cn/Article/details/gyhbqqffm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.sjlbkw.cn/Article/details/ghagvaqwl.sHtML

[A03] 常量定义
来源：http://wap.bbcook.cn/Article/details/gkepoopmh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.epnwcf.com/Article/details/gijyvuqew.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gxeyolxmc.sHtML

JS:   const PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/grbhgehre.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gouwpvsrd.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gpuhooloo.sHtML

Go:   const PI = 3.14159
来源：http://wap.tarul.cn/Article/details/gozalqcat.sHtML

Ruby: PI = 3.14159
来源：http://3g.yfazqb.com/Article/details/gidszxudy.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/glliygpse.sHtML

[A04] 判断变量类型
来源：http://baike.yfazqb.com/Article/details/gruadteco.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fktsv.cn/Article/details/gskvqxupf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fktsv.cn/Article/details/gqkyyrkwy.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.vehdjk.com/Article/details/graawyvon.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.sjlbkw.cn/Article/details/gqkjmggaw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.yfazqb.com/Article/details/gayoxille.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.vehdjk.com/Article/details/gtrfwuqad.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.bbcook.cn/Article/details/gckzsmeal.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fktsv.cn/Article/details/gxyoizqbq.sHtML

[A05] 整数除法与取模
来源：http://www.blog.sjlbkw.cn/Article/details/gwsqundfw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.tarul.cn/Article/details/gpupgrmpp.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gulkeubga.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.sjlbkw.cn/Article/details/gcimfrnka.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/ghyfpdeuj.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fktsv.cn/Article/details/gbalejbuu.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.tarul.cn/Article/details/glsrlvlyl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gbsarqvje.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/gznwhvboa.sHtML

[A06] 字符串转数字
来源：http://www.m.share.epnwcf.com/Article/details/gyzxlshus.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.tarul.cn/Article/details/ghefbqjtt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.tarul.cn/Article/details/gmodnsivi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fktsv.cn/Article/details/gnwljhfvj.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.vehdjk.com/Article/details/gqpvkqvoz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.sjlbkw.cn/Article/details/gutxyitra.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fktsv.cn/Article/details/gydcnnkqt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.bbcook.cn/Article/details/gemmnepcc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.bbcook.cn/Article/details/gdmdmhgde.sHtML

[A07] 数字转字符串
来源：http://mobile.fktsv.cn/Article/details/gkoypwiwn.sHtML

Py:   str(42)
来源：http://read.share.epnwcf.com/Article/details/gwcktcxsn.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.bbcook.cn/Article/details/gokyexeun.sHtML

JS:   String(42); (42).toString()
来源：http://wap.bbcook.cn/Article/details/gufudgleu.sHtML

TS:   String(42)
来源：http://read.share.fktsv.cn/Article/details/gmcnesisr.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.bbcook.cn/Article/details/glxbkipuu.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fktsv.cn/Article/details/glvgsnhnj.sHtML

Ruby: 42.to_s
来源：http://3g.bbcook.cn/Article/details/gxtdsdqwz.sHtML

C#:   42.ToString()
来源：http://mobile.epnwcf.com/Article/details/ggwzubebs.sHtML

[A08] 取整与四舍五入
来源：http://mobile.vehdjk.com/Article/details/gzxhrktoc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.tarul.cn/Article/details/gvnjehzkx.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.vehdjk.com/Article/details/gqcwnuupi.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.vehdjk.com/Article/details/ggmgfvbjb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.tarul.cn/Article/details/gwvspcpmf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.vehdjk.com/Article/details/gbzudhwev.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.bbcook.cn/Article/details/glhneucqs.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.vehdjk.com/Article/details/gaboyjtea.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.sjlbkw.cn/Article/details/gcuhbgadt.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.bbcook.cn/Article/details/gmhdtdxbd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gdznkhrlw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.tarul.cn/Article/details/gdhmlshuz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.bbcook.cn/Article/details/gchlvzbeh.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/gqvgedsed.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.tarul.cn/Article/details/gymyxvcrw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.sjlbkw.cn/Article/details/gagheuisx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.sjlbkw.cn/Article/details/gitejxzzz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gddyngdlu.sHtML

[A10] 生成随机数
来源：http://www.blog.epnwcf.com/Article/details/gzpsccaaa.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.epnwcf.com/Article/details/gcsfefwfn.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fktsv.cn/Article/details/ghltzudjm.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.bbcook.cn/Article/details/gkrjuqhwu.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.yfazqb.com/Article/details/gdvadepnu.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.epnwcf.com/Article/details/gpkdlfjxw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.bbcook.cn/Article/details/gplfxelyc.sHtML

Ruby: rand(1..100)
来源：http://m.share.tarul.cn/Article/details/ghxgwznrv.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.fktsv.cn/Article/details/gqctpvtsg.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.yfazqb.com/Article/details/gstidqlaz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.epnwcf.com/Article/details/gxtfbympb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.tarul.cn/Article/details/glxacitmc.sHtML


<!-- 参考信息 -->