代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.blog.epnwcf.com/Article/details/gpfnjglqh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.vehdjk.com/Article/details/godbzcsha.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.vehdjk.com/Article/details/gleqqefqu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.epnwcf.com/Article/details/gqcxwmqjn.sHtML

[U71] PHP：抛出异常
来源：http://wap.epnwcf.com/Article/details/guxfljuoc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.tarul.cn/Article/details/gqlocdkok.sHtML

[U72] PHP：写错误日志
来源：http://read.share.epnwcf.com/Article/details/ghtmeobok.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.bbcook.cn/Article/details/gzcpsqonj.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fktsv.cn/Article/details/grkgwvrzs.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.yfazqb.com/Article/details/gdjigmbqh.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.epnwcf.com/Article/details/guwekjfga.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.sjlbkw.cn/Article/details/gqutgreks.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fktsv.cn/Article/details/gwxaxjhpv.sHtML

composer require psr/container
来源：http://www.blog.sjlbkw.cn/Article/details/gfdkzilnl.sHtML

[U76] PHP：简单路由
来源：http://baike.tarul.cn/Article/details/gwwvysurb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.yfazqb.com/Article/details/gztljmvld.sHtML

[U77] PHP：模板渲染
来源：http://baike.vehdjk.com/Article/details/gmfsonalt.sHtML

composer require twig/twig
来源：http://3g.sjlbkw.cn/Article/details/gluxcjlef.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fktsv.cn/Article/details/gxzjvghpz.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.vehdjk.com/Article/details/gtzecdubv.sHtML

[U79] PHP：静态分析
来源：http://3g.tarul.cn/Article/details/gvedhxpwc.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.tarul.cn/Article/details/gnjoqwadt.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.epnwcf.com/Article/details/gxkvpzfzn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.yfazqb.com/Article/details/gprlxjzve.sHtML

[U81] JS：初始化项目
来源：http://www.blog.tarul.cn/Article/details/glsuhhovy.sHtML

npm init -y;  npm i express
来源：http://baike.yfazqb.com/Article/details/gusxamzdy.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.tarul.cn/Article/details/gvfondpda.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.tarul.cn/Article/details/gssijrass.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.tarul.cn/Article/details/grmffwupc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.bbcook.cn/Article/details/gafcvcklh.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fktsv.cn/Article/details/gcmklfrqm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.yfazqb.com/Article/details/gvzebythl.sHtML

[U85] JS：可选链
来源：http://3g.vehdjk.com/Article/details/girvhlkgd.sHtML

a?.b?.c
来源：http://m.share.vehdjk.com/Article/details/gdwelwdaw.sHtML

[U86] JS：空值合并
来源：http://baike.bbcook.cn/Article/details/gwiwrfyll.sHtML

a ?? b
来源：http://www.m.share.epnwcf.com/Article/details/gdagpzqny.sHtML

[U87] JS：解构默认值
来源：http://3g.vehdjk.com/Article/details/gqrkkwszd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fktsv.cn/Article/details/grdpndbjb.sHtML

[U88] JS：对象展开合并
来源：http://mobile.tarul.cn/Article/details/giwugrgxf.sHtML

{ ...a, ...b }
来源：http://wap.sjlbkw.cn/Article/details/gopcpbbry.sHtML

[U89] JS：数组去重
来源：http://read.share.vehdjk.com/Article/details/gawvgczln.sHtML

[...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/gtvqqjhab.sHtML

[U90] JS：数字数组排序
来源：http://wap.yfazqb.com/Article/details/gttosurtx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gxcodeijo.sHtML

[U91] JS：对象键值遍历
来源：http://blog.bbcook.cn/Article/details/gtetstmov.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.epnwcf.com/Article/details/gwbvkbziz.sHtML

[U92] JS：深拷贝
来源：http://www.blog.tarul.cn/Article/details/grevsiquf.sHtML

structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/gfmyugbcv.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.vehdjk.com/Article/details/gtnfxwhve.sHtML

`共 ${n} 条`
来源：http://read.share.vehdjk.com/Article/details/ghypvuhoz.sHtML

[U94] JS：箭头函数
来源：http://www.share.tarul.cn/Article/details/gjugbekzf.sHtML

const double = x => x * 2;
来源：http://wap.fktsv.cn/Article/details/gsbzdlbhz.sHtML

[U95] JS：Promise 包装
来源：http://read.share.sjlbkw.cn/Article/details/geptelmmp.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.tarul.cn/Article/details/gcwedutsr.sHtML

[U96] JS：async/await 与异常
来源：http://blog.tarul.cn/Article/details/gbsokemeq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gzeauqqob.sHtML

[U97] JS：并发请求
来源：http://www.share.bbcook.cn/Article/details/gpgoatukx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/guzqwnrak.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.bbcook.cn/Article/details/gfrzdpyfx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.epnwcf.com/Article/details/gqxyqshkb.sHtML

[U99] JS：事件监听
来源：http://www.blog.yfazqb.com/Article/details/gokognrez.sHtML

el.addEventListener("click", e => {})
来源：http://blog.epnwcf.com/Article/details/gtikedpsc.sHtML

[U100] JS：DOM 查询
来源：http://mobile.bbcook.cn/Article/details/gjkflljzj.sHtML

document.querySelector(".item")
来源：http://www.m.share.epnwcf.com/Article/details/gzuyrwatv.sHtML

[U101] JS：classList 操作
来源：http://mobile.sjlbkw.cn/Article/details/gotrocdof.sHtML

el.classList.toggle("active")
来源：http://www.m.share.bbcook.cn/Article/details/gtnylarzz.sHtML

[U102] JS：本地存储
来源：http://3g.sjlbkw.cn/Article/details/gtavawhoa.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.epnwcf.com/Article/details/gknnblvuo.sHtML

[U103] JS：定时器
来源：http://www.m.share.fktsv.cn/Article/details/gjmkxmimt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.yfazqb.com/Article/details/ggsjkhwqd.sHtML

[U104] JS：防抖
来源：http://baike.bbcook.cn/Article/details/grqdpezju.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/gemukvlsy.sHtML

[U105] JS：节流
来源：http://baike.vehdjk.com/Article/details/gynwouhhw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.epnwcf.com/Article/details/gxhmwsrxn.sHtML

[U106] JS：日期格式化
来源：http://m.share.vehdjk.com/Article/details/gwifgchig.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.vehdjk.com/Article/details/gqmotzqfr.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.epnwcf.com/Article/details/gpnyzsrge.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fktsv.cn/Article/details/gkwblkssh.sHtML

[U108] JS：随机整数
来源：http://m.share.bbcook.cn/Article/details/glwhbphmp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fktsv.cn/Article/details/gtshcfmlq.sHtML

[U109] JS：数组分组
来源：http://mobile.sjlbkw.cn/Article/details/ggphrotge.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.tarul.cn/Article/details/gacpgwlxq.sHtML

[U110] JS：数组分块
来源：http://read.share.bbcook.cn/Article/details/gzyrplodf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.epnwcf.com/Article/details/gzbwscqau.sHtML

[U111] JS：对象转 Map
来源：http://3g.yfazqb.com/Article/details/gkbnjhuek.sHtML

new Map(Object.entries(obj))
来源：http://read.share.vehdjk.com/Article/details/gthfztfrh.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.sjlbkw.cn/Article/details/ghccrwnxv.sHtML

"7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gsijfihza.sHtML

[U113] JS：正则替换全部
来源：http://3g.epnwcf.com/Article/details/gdyivutxf.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gmsounkkr.sHtML

[U114] JS：JSON 深比较
来源：http://3g.yfazqb.com/Article/details/godcguixz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.tarul.cn/Article/details/gxkdqirer.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.sjlbkw.cn/Article/details/gzijitihb.sHtML

crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/gppjuyqzz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.bbcook.cn/Article/details/gcxlkyqai.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.tarul.cn/Article/details/gkhbsgaiz.sHtML

[U117] JS：单元测试
来源：http://3g.tarul.cn/Article/details/gyrrirhpy.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.bbcook.cn/Article/details/gomiteqpu.sHtML

[U118] JS：开发服务器
来源：http://wap.tarul.cn/Article/details/gkbzkmaqq.sHtML

npm i -D vite;  npx vite
来源：http://mobile.yfazqb.com/Article/details/gdywusuef.sHtML

[U119] JS：生产构建
来源：http://blog.yfazqb.com/Article/details/guyissmbw.sHtML

npx vite build
来源：http://www.blog.epnwcf.com/Article/details/gbrnobjhn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjtypmmw.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fktsv.cn/Article/details/gxfqvhcju.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/guypzaaef.sHtML

统计汇总
来源：http://m.share.vehdjk.com/Article/details/gzmoavkwo.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gbimyiibh.sHtML

按语言统计（条）：
来源：http://m.share.epnwcf.com/Article/details/gklqtgtzu.sHtML

Python ......... 252
来源：http://read.share.sjlbkw.cn/Article/details/gunvnzyhf.sHtML

PHP ............ 252
来源：http://m.share.fktsv.cn/Article/details/gsleszjea.sHtML

JavaScript ..... 252
来源：http://mobile.vehdjk.com/Article/details/gbvihfojw.sHtML

TypeScript ..... 212
来源：http://m.share.sjlbkw.cn/Article/details/gfdnmfyyf.sHtML

Java ........... 212
来源：http://www.share.vehdjk.com/Article/details/gomgwoqoc.sHtML

Go ............. 212
来源：http://www.blog.sjlbkw.cn/Article/details/gncshukyc.sHtML

Ruby ........... 212
来源：http://www.m.share.tarul.cn/Article/details/gdiifhfdf.sHtML

C# ............. 212
来源：http://www.blog.epnwcf.com/Article/details/guobmiefs.sHtML

C .............. 30
来源：http://www.share.sjlbkw.cn/Article/details/glsopcaaf.sHtML

C++ ............ 30
来源：http://read.share.epnwcf.com/Article/details/glvzdtyjw.sHtML

SQL ............ 90
来源：http://www.share.yfazqb.com/Article/details/guidyvizd.sHtML

Bash ........... 80
来源：http://read.share.vehdjk.com/Article/details/gkhprwftu.sHtML

Kotlin ......... 15
来源：http://www.blog.fktsv.cn/Article/details/gcavhcrno.sHtML

Swift .......... 15
来源：http://baike.vehdjk.com/Article/details/gicakkxyc.sHtML

Lua ............ 10
来源：http://blog.bbcook.cn/Article/details/gkbgtawlm.sHtML

Perl ........... 10
来源：http://baike.epnwcf.com/Article/details/ghdvrcgjr.sHtML

Scala .......... 10
来源：http://blog.sjlbkw.cn/Article/details/grwaxfbqe.sHtML

------------------------------------
来源：http://mobile.fktsv.cn/Article/details/guyplahdc.sHtML

合计 ........... 2106 条
来源：http://3g.fktsv.cn/Article/details/gyulsknie.sHtML

按章节统计：
来源：http://baike.tarul.cn/Article/details/gtbyagilg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fktsv.cn/Article/details/grqxaogdb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.yfazqb.com/Article/details/gcsllwmzo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.tarul.cn/Article/details/gtcdoeedm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.yfazqb.com/Article/details/gsooacswp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.bbcook.cn/Article/details/ghmxjxfhj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.epnwcf.com/Article/details/gfbrldqma.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.bbcook.cn/Article/details/gsuljasuz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.tarul.cn/Article/details/gyzigdmoh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gptlfhrfu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.vehdjk.com/Article/details/gunbauoyg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/gtjkvznoi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/gocqkgohz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/giwcvhiny.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.vehdjk.com/Article/details/gvkqmqmgo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fktsv.cn/Article/details/guoftietm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/gmccoanco.sHtML

Q SQL 专题                              90
来源：http://blog.yfazqb.com/Article/details/gqvlvexpp.sHtML

R Bash 专题                             80
来源：http://www.m.share.tarul.cn/Article/details/gpdswvsjo.sHtML

S C / C++ 专题                          60
来源：http://www.blog.epnwcf.com/Article/details/gddyxvupm.sHtML

T 其他语言补充                          60
来源：http://baike.tarul.cn/Article/details/guroispun.sHtML

U 高频实用片段                         120
来源：http://wap.epnwcf.com/Article/details/gvpbuylef.sHtML

------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/gaswipkbq.sHtML

合计                                  2106 条
来源：http://mobile.epnwcf.com/Article/details/gtnnrucaa.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gnhtkvmat.sHtML

使用提醒
来源：http://www.blog.tarul.cn/Article/details/gwqrmsfbi.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gudpsbblb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.epnwcf.com/Article/details/goeqfqnbw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.tarul.cn/Article/details/guokvulmn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.tarul.cn/Article/details/gigxcupts.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fktsv.cn/Article/details/gzeqmmifn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.epnwcf.com/Article/details/gtsksupje.sHtML

—— 文件结束 ——
来源：http://read.share.bbcook.cn/Article/details/gitctgjbm.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/grmnzstvg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fktsv.cn/Article/details/gkquoqqli.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.yfazqb.com/Article/details/glavivvwo.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gtlmmxjno.sHtML

【收录内容】
来源：http://baike.vehdjk.com/Article/details/gdvusgfrf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.tarul.cn/Article/details/geazptjlh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.sjlbkw.cn/Article/details/ggmvnfqdk.sHtML

SQL · Bash · C · C++
来源：http://wap.epnwcf.com/Article/details/gfkvzvgjr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.epnwcf.com/Article/details/gsppcihlz.sHtML

【使用说明】
来源：http://baike.bbcook.cn/Article/details/gneflybny.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.bbcook.cn/Article/details/gqkjtpyrv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.epnwcf.com/Article/details/gtorrvbhb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.epnwcf.com/Article/details/gfgoryauc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.epnwcf.com/Article/details/grqgisazh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fktsv.cn/Article/details/gcixewbbd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.epnwcf.com/Article/details/gdaxtuehb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.yfazqb.com/Article/details/gqgrbnuwg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.vehdjk.com/Article/details/gkfnkyhhj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.sjlbkw.cn/Article/details/gdsyejdna.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.vehdjk.com/Article/details/ghatldowp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.vehdjk.com/Article/details/gpaadekdj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.bbcook.cn/Article/details/gyxwpswdd.sHtML

【文件统计】
来源：http://www.blog.epnwcf.com/Article/details/gdejcpxnf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.bbcook.cn/Article/details/gqzjdkuwh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gdmusovrg.sHtML

目  录
来源：http://www.m.share.vehdjk.com/Article/details/gwjljwguf.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.tarul.cn/Article/details/gxugpwikx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwmlmkap.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.vehdjk.com/Article/details/gdbfiqhcp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.epnwcf.com/Article/details/gpqoakwqd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fktsv.cn/Article/details/gdqrwjahe.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.epnwcf.com/Article/details/gequzdxxs.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.vehdjk.com/Article/details/gycaroxil.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/gmgblmhrp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.yfazqb.com/Article/details/gzfjmpclw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/gvnqdhgnw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.tarul.cn/Article/details/gynxgopjd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/gmcotbzkl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.vehdjk.com/Article/details/gafvgezjs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.yfazqb.com/Article/details/gkhtlmbxn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.vehdjk.com/Article/details/grcydcomz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.sjlbkw.cn/Article/details/gmbaoyzqq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/gjtgwpjzn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.tarul.cn/Article/details/gtpoeazmp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.sjlbkw.cn/Article/details/gahspvwcd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.epnwcf.com/Article/details/gfcptngoi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.vehdjk.com/Article/details/gyulspqkb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.yfazqb.com/Article/details/gdwyiomqz.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gjllmmddr.sHtML

A. 基础语法与类型
来源：http://m.share.sjlbkw.cn/Article/details/gsfprzjdo.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gacwpguyw.sHtML

[A01] Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gzrdatohc.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.tarul.cn/Article/details/ghetqczmq.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.vehdjk.com/Article/details/giwhbpdis.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.bbcook.cn/Article/details/gazcbmdgb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.bbcook.cn/Article/details/gcbitpdca.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.tarul.cn/Article/details/guoohyglh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.sjlbkw.cn/Article/details/gmkzeampl.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.vehdjk.com/Article/details/gdydbwvvl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.epnwcf.com/Article/details/gvqnnepgl.sHtML

[A02] 变量声明与赋值
来源：http://baike.epnwcf.com/Article/details/galgmiyjz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.yfazqb.com/Article/details/gufzpklda.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.epnwcf.com/Article/details/gdkqfcrzt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.yfazqb.com/Article/details/gaywpltnx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fktsv.cn/Article/details/gfxxlcasx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.tarul.cn/Article/details/gqidbmcoj.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.epnwcf.com/Article/details/gjiyvkzby.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.tarul.cn/Article/details/gixzmsrub.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.bbcook.cn/Article/details/gjcdxyifl.sHtML

[A03] 常量定义
来源：http://m.share.fktsv.cn/Article/details/gchtvmair.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.yfazqb.com/Article/details/gllkpxgiy.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gfypkvgqr.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gpxquatyx.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gvnlsxpui.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/guzjsnehf.sHtML

Go:   const PI = 3.14159
来源：http://blog.tarul.cn/Article/details/gmgorpmld.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.vehdjk.com/Article/details/ghtnkgwki.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/grnrtrzkr.sHtML

[A04] 判断变量类型
来源：http://www.m.share.epnwcf.com/Article/details/gkxtufiqc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.yfazqb.com/Article/details/gofuzifag.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.tarul.cn/Article/details/gxxrnealu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.bbcook.cn/Article/details/goaicisgc.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.tarul.cn/Article/details/gdulnsmwb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.vehdjk.com/Article/details/gemqhllau.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.epnwcf.com/Article/details/geptkakxk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.vehdjk.com/Article/details/gzkgmfyrg.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.epnwcf.com/Article/details/gnxleohxt.sHtML

[A05] 整数除法与取模
来源：http://blog.vehdjk.com/Article/details/glkwjqchm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.vehdjk.com/Article/details/gprcokeeh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.epnwcf.com/Article/details/gtnfshdap.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.tarul.cn/Article/details/gpjlpluhq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/gunxvdcug.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.bbcook.cn/Article/details/gtajbyqqz.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.bbcook.cn/Article/details/gyzecvztc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.bbcook.cn/Article/details/gbluetxic.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/gnebppszv.sHtML

[A06] 字符串转数字
来源：http://mobile.vehdjk.com/Article/details/gbtwtnuaj.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fktsv.cn/Article/details/gcgqcsgnx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.sjlbkw.cn/Article/details/ggjvksmyw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.epnwcf.com/Article/details/gnetubcwr.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.yfazqb.com/Article/details/gyovtdrgl.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.epnwcf.com/Article/details/gnjxmoqfi.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.epnwcf.com/Article/details/gkontohwf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fktsv.cn/Article/details/grbtqzrnx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.vehdjk.com/Article/details/gcruffref.sHtML

[A07] 数字转字符串
来源：http://baike.vehdjk.com/Article/details/guwqahrka.sHtML

Py:   str(42)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnoolkqb.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.yfazqb.com/Article/details/gsirnxjtp.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.bbcook.cn/Article/details/gliywzzni.sHtML

TS:   String(42)
来源：http://wap.sjlbkw.cn/Article/details/gzyuuiysb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.vehdjk.com/Article/details/gybjirrbd.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.epnwcf.com/Article/details/gzvakywei.sHtML

Ruby: 42.to_s
来源：http://mobile.fktsv.cn/Article/details/gmuigftwq.sHtML

C#:   42.ToString()
来源：http://www.blog.epnwcf.com/Article/details/geokxqyph.sHtML

[A08] 取整与四舍五入
来源：http://3g.yfazqb.com/Article/details/gznyawesx.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.epnwcf.com/Article/details/gaotqvjky.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.sjlbkw.cn/Article/details/gcfdchnew.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/grinolpvb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.yfazqb.com/Article/details/gnmjpvbxi.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.bbcook.cn/Article/details/ghzbsxhzu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/gxlmavujm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fktsv.cn/Article/details/gmomvtznd.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.yfazqb.com/Article/details/gwgtmnagw.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.bbcook.cn/Article/details/gtrhhwiwd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.yfazqb.com/Article/details/gltjvtsyx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.epnwcf.com/Article/details/grehkxzqs.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gufwyunkx.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gsefpjacm.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gitxonxuq.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.fktsv.cn/Article/details/gyngtclkh.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.yfazqb.com/Article/details/gvbmqaazy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.vehdjk.com/Article/details/gedqbpqlj.sHtML

[A10] 生成随机数
来源：http://www.blog.bbcook.cn/Article/details/gdwlyawkv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.epnwcf.com/Article/details/gmuwsocve.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.vehdjk.com/Article/details/geoimrhjd.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.tarul.cn/Article/details/ginaghsjq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.tarul.cn/Article/details/gxvjmrqxg.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.fktsv.cn/Article/details/gbuarmijq.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.epnwcf.com/Article/details/gucrypxga.sHtML

Ruby: rand(1..100)
来源：http://wap.vehdjk.com/Article/details/gzbtoobht.sHtML


<!-- 参考信息 -->