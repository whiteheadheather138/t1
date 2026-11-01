代发 wailian999

[U69] PHP：PDO 预处理
来源：http://read.share.tarul.cn/Article/details/gdbwgvpuk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fktsv.cn/Article/details/gekxzoxrw.sHtML

[U70] PHP：PDO 事务
来源：http://wap.epnwcf.com/Article/details/gsgfayhbg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fktsv.cn/Article/details/gpcridxof.sHtML

[U71] PHP：抛出异常
来源：http://wap.bbcook.cn/Article/details/gfyxtgpad.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.epnwcf.com/Article/details/guscpdotu.sHtML

[U72] PHP：写错误日志
来源：http://wap.fktsv.cn/Article/details/gagtupfhk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.bbcook.cn/Article/details/gupqopeed.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.epnwcf.com/Article/details/gfmkjgsnl.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.vehdjk.com/Article/details/gwtebpstr.sHtML

[U74] PHP：读取环境变量
来源：http://3g.tarul.cn/Article/details/gfbiowunn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fktsv.cn/Article/details/gyracpogl.sHtML

[U75] PHP：依赖注入
来源：http://m.share.yfazqb.com/Article/details/gxpmnfoxo.sHtML

composer require psr/container
来源：http://wap.vehdjk.com/Article/details/gamozgmmp.sHtML

[U76] PHP：简单路由
来源：http://read.share.tarul.cn/Article/details/ggoarmrpe.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.vehdjk.com/Article/details/gjwuutqwn.sHtML

[U77] PHP：模板渲染
来源：http://www.share.bbcook.cn/Article/details/gspiwerzq.sHtML

composer require twig/twig
来源：http://www.blog.sjlbkw.cn/Article/details/ghzimqtnf.sHtML

[U78] PHP：单元测试
来源：http://mobile.epnwcf.com/Article/details/ghbtnxvbb.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.yfazqb.com/Article/details/gdvseeula.sHtML

[U79] PHP：静态分析
来源：http://www.share.bbcook.cn/Article/details/ggeagfbzy.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.sjlbkw.cn/Article/details/gnngpptko.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fktsv.cn/Article/details/gcwjzbspx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.sjlbkw.cn/Article/details/gvcahevqf.sHtML

[U81] JS：初始化项目
来源：http://3g.bbcook.cn/Article/details/gwfwqeztf.sHtML

npm init -y;  npm i express
来源：http://www.blog.fktsv.cn/Article/details/gueofyxpi.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.sjlbkw.cn/Article/details/gxeucdxag.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.bbcook.cn/Article/details/gnrvpxgdx.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.vehdjk.com/Article/details/gzfmtfovt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.sjlbkw.cn/Article/details/gnxkxbapu.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.sjlbkw.cn/Article/details/ghngkqvqc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.bbcook.cn/Article/details/gsnnrsaji.sHtML

[U85] JS：可选链
来源：http://baike.vehdjk.com/Article/details/gjwozskdv.sHtML

a?.b?.c
来源：http://mobile.tarul.cn/Article/details/gdfpgfqqb.sHtML

[U86] JS：空值合并
来源：http://wap.tarul.cn/Article/details/gzyskyurn.sHtML

a ?? b
来源：http://m.share.epnwcf.com/Article/details/ggyuigtan.sHtML

[U87] JS：解构默认值
来源：http://m.share.yfazqb.com/Article/details/gcmwezzyv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.vehdjk.com/Article/details/gnbxiiiyu.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fktsv.cn/Article/details/gnwskslpw.sHtML

{ ...a, ...b }
来源：http://baike.epnwcf.com/Article/details/gzcfhutve.sHtML

[U89] JS：数组去重
来源：http://www.blog.tarul.cn/Article/details/gdmopnzfl.sHtML

[...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gtnkgebui.sHtML

[U90] JS：数字数组排序
来源：http://www.share.bbcook.cn/Article/details/gwdedadfv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/gymgculur.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fktsv.cn/Article/details/gistmohdm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.sjlbkw.cn/Article/details/gdmjpijaq.sHtML

[U92] JS：深拷贝
来源：http://www.share.bbcook.cn/Article/details/gwfgehhkq.sHtML

structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/ghmqqnjwg.sHtML

[U93] JS：模板字符串
来源：http://mobile.sjlbkw.cn/Article/details/gwlrjprco.sHtML

`共 ${n} 条`
来源：http://wap.bbcook.cn/Article/details/gokimmxqe.sHtML

[U94] JS：箭头函数
来源：http://www.share.tarul.cn/Article/details/gpklkoisz.sHtML

const double = x => x * 2;
来源：http://www.share.vehdjk.com/Article/details/gjnijtfsu.sHtML

[U95] JS：Promise 包装
来源：http://3g.tarul.cn/Article/details/gvkluqrkc.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.sjlbkw.cn/Article/details/gtataxkol.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.yfazqb.com/Article/details/gifffbxim.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gwcxajhcj.sHtML

[U97] JS：并发请求
来源：http://www.share.fktsv.cn/Article/details/gefaqwoib.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.yfazqb.com/Article/details/gpjynvkit.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.bbcook.cn/Article/details/gjkinxlab.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.vehdjk.com/Article/details/gcnoysqtx.sHtML

[U99] JS：事件监听
来源：http://m.share.yfazqb.com/Article/details/gfmsnhavx.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.yfazqb.com/Article/details/glipjmrvv.sHtML

[U100] JS：DOM 查询
来源：http://read.share.yfazqb.com/Article/details/grztpnpfz.sHtML

document.querySelector(".item")
来源：http://m.share.epnwcf.com/Article/details/gdmyjvalc.sHtML

[U101] JS：classList 操作
来源：http://mobile.bbcook.cn/Article/details/gxvlufssa.sHtML

el.classList.toggle("active")
来源：http://baike.bbcook.cn/Article/details/ggdxlcoiu.sHtML

[U102] JS：本地存储
来源：http://m.share.sjlbkw.cn/Article/details/gjzxvtcrz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fktsv.cn/Article/details/gphvxyyqu.sHtML

[U103] JS：定时器
来源：http://m.share.tarul.cn/Article/details/gejtyutdr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.vehdjk.com/Article/details/gbutgmrpu.sHtML

[U104] JS：防抖
来源：http://www.blog.bbcook.cn/Article/details/gbewcrids.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gnqphxiwh.sHtML

[U105] JS：节流
来源：http://wap.tarul.cn/Article/details/gszewjelo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.yfazqb.com/Article/details/grsrlrpsz.sHtML

[U106] JS：日期格式化
来源：http://blog.sjlbkw.cn/Article/details/grtgfdywa.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.yfazqb.com/Article/details/gziaeciws.sHtML

[U107] JS：数字千分位
来源：http://mobile.epnwcf.com/Article/details/gpghiyusj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.sjlbkw.cn/Article/details/gdjvwipqj.sHtML

[U108] JS：随机整数
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmzydtrk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.epnwcf.com/Article/details/gigggtjul.sHtML

[U109] JS：数组分组
来源：http://mobile.epnwcf.com/Article/details/gtctagemu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.epnwcf.com/Article/details/gtslakgwk.sHtML

[U110] JS：数组分块
来源：http://www.blog.epnwcf.com/Article/details/govgontym.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.bbcook.cn/Article/details/ghsoyvbwm.sHtML

[U111] JS：对象转 Map
来源：http://3g.yfazqb.com/Article/details/gzbuwsdsc.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fktsv.cn/Article/details/gdjgdyulx.sHtML

[U112] JS：字符串补位
来源：http://blog.fktsv.cn/Article/details/gzhknldee.sHtML

"7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gwofhvxid.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.vehdjk.com/Article/details/ghkitcpci.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gnroqxtds.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.sjlbkw.cn/Article/details/ggnxfjrco.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.yfazqb.com/Article/details/ghksobubv.sHtML

[U115] JS：生成 UUID
来源：http://blog.tarul.cn/Article/details/gxkvanehd.sHtML

crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/gszwqiihj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.tarul.cn/Article/details/ggkisauwi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.sjlbkw.cn/Article/details/gfqnczykx.sHtML

[U117] JS：单元测试
来源：http://3g.bbcook.cn/Article/details/gepbslzlx.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fktsv.cn/Article/details/gjzunglpz.sHtML

[U118] JS：开发服务器
来源：http://3g.epnwcf.com/Article/details/gbazqxoln.sHtML

npm i -D vite;  npx vite
来源：http://3g.vehdjk.com/Article/details/gzedtgqfg.sHtML

[U119] JS：生产构建
来源：http://blog.yfazqb.com/Article/details/gsabayktd.sHtML

npx vite build
来源：http://www.blog.fktsv.cn/Article/details/gsmgnpbad.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.tarul.cn/Article/details/gdgwpvahq.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.epnwcf.com/Article/details/gnrmjinud.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gsrvichbf.sHtML

统计汇总
来源：http://m.share.bbcook.cn/Article/details/gidxwhsas.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gkzzxkezs.sHtML

按语言统计（条）：
来源：http://3g.vehdjk.com/Article/details/gnnggayui.sHtML

Python ......... 252
来源：http://3g.epnwcf.com/Article/details/gmjanolzo.sHtML

PHP ............ 252
来源：http://m.share.yfazqb.com/Article/details/gdionpjxo.sHtML

JavaScript ..... 252
来源：http://blog.epnwcf.com/Article/details/gbqolapgj.sHtML

TypeScript ..... 212
来源：http://www.share.vehdjk.com/Article/details/ghbfhggbu.sHtML

Java ........... 212
来源：http://3g.vehdjk.com/Article/details/gdudbtvsb.sHtML

Go ............. 212
来源：http://m.share.vehdjk.com/Article/details/gfdkohwra.sHtML

Ruby ........... 212
来源：http://mobile.fktsv.cn/Article/details/gxrfdsbyw.sHtML

C# ............. 212
来源：http://www.blog.fktsv.cn/Article/details/gsxnglmlt.sHtML

C .............. 30
来源：http://m.share.epnwcf.com/Article/details/gpnierjar.sHtML

C++ ............ 30
来源：http://www.share.epnwcf.com/Article/details/gdoqjxkje.sHtML

SQL ............ 90
来源：http://read.share.vehdjk.com/Article/details/gcqipdszm.sHtML

Bash ........... 80
来源：http://www.m.share.yfazqb.com/Article/details/gnyopinqg.sHtML

Kotlin ......... 15
来源：http://3g.epnwcf.com/Article/details/gavvqlofv.sHtML

Swift .......... 15
来源：http://3g.bbcook.cn/Article/details/gqsogzxzo.sHtML

Lua ............ 10
来源：http://m.share.fktsv.cn/Article/details/gtvbcugck.sHtML

Perl ........... 10
来源：http://www.m.share.yfazqb.com/Article/details/gilgyznvb.sHtML

Scala .......... 10
来源：http://blog.epnwcf.com/Article/details/gnesyljsa.sHtML

------------------------------------
来源：http://blog.bbcook.cn/Article/details/gggjdrxtj.sHtML

合计 ........... 2106 条
来源：http://baike.vehdjk.com/Article/details/gbdeyirer.sHtML

按章节统计：
来源：http://www.m.share.bbcook.cn/Article/details/glvajqmtu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.tarul.cn/Article/details/gygyvxzkq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.epnwcf.com/Article/details/gwenzdrfc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.epnwcf.com/Article/details/gmauefzvs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.vehdjk.com/Article/details/gefredsuh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.tarul.cn/Article/details/gkarszwux.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.bbcook.cn/Article/details/gvhjdakig.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.bbcook.cn/Article/details/gqpdflmes.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.sjlbkw.cn/Article/details/ggtuqanrx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gkpbfvpdg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.bbcook.cn/Article/details/guqsesugc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gazjzarxq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/gwpejxmss.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/grlbaoiho.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.sjlbkw.cn/Article/details/gdfmxxrek.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.tarul.cn/Article/details/gyujzvnup.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/gcsltcdye.sHtML

Q SQL 专题                              90
来源：http://blog.fktsv.cn/Article/details/ggkvdhirz.sHtML

R Bash 专题                             80
来源：http://www.blog.fktsv.cn/Article/details/ghggnpvla.sHtML

S C / C++ 专题                          60
来源：http://baike.yfazqb.com/Article/details/gsptzxrth.sHtML

T 其他语言补充                          60
来源：http://wap.epnwcf.com/Article/details/grabklics.sHtML

U 高频实用片段                         120
来源：http://mobile.tarul.cn/Article/details/glwrphlky.sHtML

------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/grhhntgqr.sHtML

合计                                  2106 条
来源：http://mobile.bbcook.cn/Article/details/gwygphfup.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gtijfxfcc.sHtML

使用提醒
来源：http://baike.epnwcf.com/Article/details/gwhhfmhio.sHtML

--------------------------------------------------------------------------------
来源：http://3g.bbcook.cn/Article/details/glylgrsrr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.vehdjk.com/Article/details/greipspmq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.bbcook.cn/Article/details/gbfsxexwd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.bbcook.cn/Article/details/gngmcuqbj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.bbcook.cn/Article/details/gfjqwpznv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.tarul.cn/Article/details/gsazelbyx.sHtML

—— 文件结束 ——
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmbwtidr.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gqomioqtu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.epnwcf.com/Article/details/glustjfkr.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.epnwcf.com/Article/details/gfqrayqdi.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/grirlbddp.sHtML

【收录内容】
来源：http://blog.yfazqb.com/Article/details/gpuheieth.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.vehdjk.com/Article/details/gmdiyuedq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.sjlbkw.cn/Article/details/ghmhijrih.sHtML

SQL · Bash · C · C++
来源：http://www.share.epnwcf.com/Article/details/guudvqptb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.tarul.cn/Article/details/gmbfupoxn.sHtML

【使用说明】
来源：http://wap.bbcook.cn/Article/details/gldurymdt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.sjlbkw.cn/Article/details/gussdjyxc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.bbcook.cn/Article/details/gcgvvfsfe.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.yfazqb.com/Article/details/gcvbvidgt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.yfazqb.com/Article/details/ghhstvpzr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fktsv.cn/Article/details/gzhagmksq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fktsv.cn/Article/details/gtkwwfwbv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.sjlbkw.cn/Article/details/gelnbofnf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.vehdjk.com/Article/details/glsggkjwc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.tarul.cn/Article/details/ganqzfiko.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.vehdjk.com/Article/details/gyowuytzx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.yfazqb.com/Article/details/gfvwqiegt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.epnwcf.com/Article/details/gezzxftcw.sHtML

【文件统计】
来源：http://blog.vehdjk.com/Article/details/gpilgdorw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.vehdjk.com/Article/details/grvmjoslz.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gylxfbocv.sHtML

目  录
来源：http://3g.yfazqb.com/Article/details/gjtzlqiiz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/ggtexjhpi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.vehdjk.com/Article/details/gmjhwjjwn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.tarul.cn/Article/details/gypfoaarn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.tarul.cn/Article/details/gcpvxevfk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.sjlbkw.cn/Article/details/gzllsnoep.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.tarul.cn/Article/details/grpmsepwf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.epnwcf.com/Article/details/gysfyscih.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.vehdjk.com/Article/details/geoeeizel.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gorsmdsft.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gflozyjcx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.epnwcf.com/Article/details/grztkzvav.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.epnwcf.com/Article/details/gvnrzysqf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fktsv.cn/Article/details/gdyhalrue.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/gkbvaxemc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.sjlbkw.cn/Article/details/gsghlemdh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.yfazqb.com/Article/details/gpfovtbxk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fktsv.cn/Article/details/gijkzjqub.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fktsv.cn/Article/details/gxnkrhmsg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.vehdjk.com/Article/details/grfrpbvmc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.yfazqb.com/Article/details/gojgdwfic.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.epnwcf.com/Article/details/gqzhvfbmw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fktsv.cn/Article/details/gtcqqnnob.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/grddktjvw.sHtML

A. 基础语法与类型
来源：http://baike.sjlbkw.cn/Article/details/gfmsxpscs.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gqezgbnzc.sHtML

[A01] Hello World
来源：http://3g.vehdjk.com/Article/details/gtfpotqvb.sHtML

Py:   print("Hello, World!")
来源：http://www.share.yfazqb.com/Article/details/gixmcbvke.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.epnwcf.com/Article/details/ghmfzroho.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fktsv.cn/Article/details/gedbpxglr.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.tarul.cn/Article/details/gecjspxyg.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.bbcook.cn/Article/details/gmsammojl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.epnwcf.com/Article/details/ghzuhffre.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.yfazqb.com/Article/details/gtjdmwumi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.tarul.cn/Article/details/gfxhbpyqn.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.yfazqb.com/Article/details/gfanhixbp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.sjlbkw.cn/Article/details/grgcskcyh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.yfazqb.com/Article/details/gzoorsnyg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gzqajeddy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fktsv.cn/Article/details/gkbiovual.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.sjlbkw.cn/Article/details/gvipfryyd.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.tarul.cn/Article/details/gavkcgdqs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.vehdjk.com/Article/details/grvkwdfwm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fktsv.cn/Article/details/gjmztinnt.sHtML

[A03] 常量定义
来源：http://read.share.vehdjk.com/Article/details/gcfxuakyl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.epnwcf.com/Article/details/ggwjoljpe.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gxdlivbuv.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gcbyefnwu.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/ggbemfzqj.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gdzilhvcw.sHtML

Go:   const PI = 3.14159
来源：http://www.share.vehdjk.com/Article/details/gkykrjbnl.sHtML

Ruby: PI = 3.14159
来源：http://3g.bbcook.cn/Article/details/gnisjoqyn.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/grmqwgkit.sHtML

[A04] 判断变量类型
来源：http://wap.tarul.cn/Article/details/gvthictea.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.vehdjk.com/Article/details/gsztpbrds.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.yfazqb.com/Article/details/giosxjbbu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.bbcook.cn/Article/details/gpbeatheo.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.bbcook.cn/Article/details/gmihuynqn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.epnwcf.com/Article/details/gptrcwkwu.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.sjlbkw.cn/Article/details/gadyrdigh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.yfazqb.com/Article/details/gfbxjojch.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.tarul.cn/Article/details/gulhyrutw.sHtML

[A05] 整数除法与取模
来源：http://wap.epnwcf.com/Article/details/ghrdfoymx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.yfazqb.com/Article/details/grbcaecfk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/gszxshskv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.tarul.cn/Article/details/gwtioydml.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gqzjgycuf.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gzmujbywu.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.epnwcf.com/Article/details/gyxacwota.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.bbcook.cn/Article/details/gvizsjczo.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fktsv.cn/Article/details/gotkvslbk.sHtML

[A06] 字符串转数字
来源：http://www.share.tarul.cn/Article/details/gghpbxqwj.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.tarul.cn/Article/details/gygvljind.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.yfazqb.com/Article/details/gqeezuhfz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.epnwcf.com/Article/details/gwgkytovd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.tarul.cn/Article/details/gdvnlzmbn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.vehdjk.com/Article/details/ghfgtvmic.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fktsv.cn/Article/details/gxyxdenen.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.vehdjk.com/Article/details/gbvdvbuzi.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.bbcook.cn/Article/details/gwydgufoc.sHtML

[A07] 数字转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gjzsyfvda.sHtML

Py:   str(42)
来源：http://3g.fktsv.cn/Article/details/grhaebkjf.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.tarul.cn/Article/details/gofjpxbkc.sHtML

JS:   String(42); (42).toString()
来源：http://wap.tarul.cn/Article/details/gdhjnwpdy.sHtML

TS:   String(42)
来源：http://read.share.bbcook.cn/Article/details/gsatwsxjf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fktsv.cn/Article/details/gccpbwbkq.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.yfazqb.com/Article/details/glkpmdvct.sHtML

Ruby: 42.to_s
来源：http://www.m.share.yfazqb.com/Article/details/gwozqvddh.sHtML

C#:   42.ToString()
来源：http://m.share.fktsv.cn/Article/details/gcdkgrugl.sHtML

[A08] 取整与四舍五入
来源：http://blog.tarul.cn/Article/details/gefjswsgx.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.fktsv.cn/Article/details/gyxjckmel.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fktsv.cn/Article/details/gttllpcee.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fktsv.cn/Article/details/gtylyikrq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fktsv.cn/Article/details/gpbbeekdu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.yfazqb.com/Article/details/gzioljtpg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.vehdjk.com/Article/details/gogevlhfg.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.epnwcf.com/Article/details/gzotbevbf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/gtosnjgge.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.epnwcf.com/Article/details/gifwqppyj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gumjeuhln.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.epnwcf.com/Article/details/gjxhzwuqz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gpfyfupiu.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/grcugtfmw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gatzgjawr.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.tarul.cn/Article/details/goqpgfaun.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.fktsv.cn/Article/details/gewrjogum.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gpjpwaanw.sHtML

[A10] 生成随机数
来源：http://baike.vehdjk.com/Article/details/gumpcjdox.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.yfazqb.com/Article/details/gzfxzewzi.sHtML

PHP:  random_int(1, 100);
来源：http://blog.bbcook.cn/Article/details/ghbbsedfk.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.epnwcf.com/Article/details/gefhhhoge.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.sjlbkw.cn/Article/details/gxjgehomw.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.sjlbkw.cn/Article/details/gddsfyarh.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.yfazqb.com/Article/details/gytlelrcf.sHtML

Ruby: rand(1..100)
来源：http://mobile.epnwcf.com/Article/details/gztxeiyyw.sHtML


<!-- 参考信息 -->