代发 wailian999

[U69] PHP：PDO 预处理
来源：http://mobile.tarul.cn/Article/details/gkentquew.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.vehdjk.com/Article/details/gkozymvpc.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.yfazqb.com/Article/details/gavraaxfy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.tarul.cn/Article/details/gumdmdnlx.sHtML

[U71] PHP：抛出异常
来源：http://3g.tarul.cn/Article/details/gmgtahozb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.yfazqb.com/Article/details/gkvkishbo.sHtML

[U72] PHP：写错误日志
来源：http://blog.vehdjk.com/Article/details/gfgldudue.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.tarul.cn/Article/details/gzubtrsmq.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.yfazqb.com/Article/details/gvntfggjx.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.sjlbkw.cn/Article/details/gzrorycqb.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.bbcook.cn/Article/details/grvmdqnvn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.vehdjk.com/Article/details/gkkcvcznd.sHtML

[U75] PHP：依赖注入
来源：http://3g.fktsv.cn/Article/details/gwamlyyim.sHtML

composer require psr/container
来源：http://m.share.sjlbkw.cn/Article/details/gfhfxlftt.sHtML

[U76] PHP：简单路由
来源：http://www.share.bbcook.cn/Article/details/guhtiwoyw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.vehdjk.com/Article/details/gsldblhjo.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fktsv.cn/Article/details/gpadjqoqh.sHtML

composer require twig/twig
来源：http://www.share.epnwcf.com/Article/details/gkrouzvuc.sHtML

[U78] PHP：单元测试
来源：http://www.blog.epnwcf.com/Article/details/geohvcysc.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fktsv.cn/Article/details/gvcwufrtp.sHtML

[U79] PHP：静态分析
来源：http://www.share.yfazqb.com/Article/details/gvtkaxdye.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.vehdjk.com/Article/details/gfgdgtgij.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.epnwcf.com/Article/details/gtugmkzou.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.vehdjk.com/Article/details/gycbwflai.sHtML

[U81] JS：初始化项目
来源：http://www.blog.sjlbkw.cn/Article/details/gbpxqrpfv.sHtML

npm init -y;  npm i express
来源：http://mobile.epnwcf.com/Article/details/gvgulylju.sHtML

[U82] JS：package.json 脚本
来源：http://wap.yfazqb.com/Article/details/gjgwysmtl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.tarul.cn/Article/details/gsuomrhqf.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.bbcook.cn/Article/details/gbfpclige.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.bbcook.cn/Article/details/gyqwkflxo.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.sjlbkw.cn/Article/details/goglezymp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.bbcook.cn/Article/details/gbgxvrequ.sHtML

[U85] JS：可选链
来源：http://blog.sjlbkw.cn/Article/details/gnstouirw.sHtML

a?.b?.c
来源：http://mobile.fktsv.cn/Article/details/gxipcvhus.sHtML

[U86] JS：空值合并
来源：http://blog.bbcook.cn/Article/details/gxqrgysus.sHtML

a ?? b
来源：http://wap.epnwcf.com/Article/details/giguyxjif.sHtML

[U87] JS：解构默认值
来源：http://baike.tarul.cn/Article/details/gjrdwyblz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.bbcook.cn/Article/details/gzraaebge.sHtML

[U88] JS：对象展开合并
来源：http://m.share.bbcook.cn/Article/details/gbgutfphc.sHtML

{ ...a, ...b }
来源：http://www.share.fktsv.cn/Article/details/gtthpkuui.sHtML

[U89] JS：数组去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gyplbikjp.sHtML

[...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/gvhkozgny.sHtML

[U90] JS：数字数组排序
来源：http://mobile.bbcook.cn/Article/details/gekiicdsr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/gcvqvprlb.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.yfazqb.com/Article/details/griguhhxi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.yfazqb.com/Article/details/gvlgeinbb.sHtML

[U92] JS：深拷贝
来源：http://mobile.vehdjk.com/Article/details/gwgzrwwqf.sHtML

structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/ghuiuzkex.sHtML

[U93] JS：模板字符串
来源：http://m.share.sjlbkw.cn/Article/details/gjnatffsv.sHtML

`共 ${n} 条`
来源：http://www.share.epnwcf.com/Article/details/ghqleyvvh.sHtML

[U94] JS：箭头函数
来源：http://3g.tarul.cn/Article/details/gmmlmjjfr.sHtML

const double = x => x * 2;
来源：http://mobile.yfazqb.com/Article/details/gvazijnoh.sHtML

[U95] JS：Promise 包装
来源：http://3g.vehdjk.com/Article/details/guunwkvek.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.tarul.cn/Article/details/gpchwtduf.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.sjlbkw.cn/Article/details/grzisaohg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/glrbavlkm.sHtML

[U97] JS：并发请求
来源：http://www.blog.yfazqb.com/Article/details/gddcxicss.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/gymomlrgx.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.sjlbkw.cn/Article/details/gcmrinrts.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.sjlbkw.cn/Article/details/gjtuabfcd.sHtML

[U99] JS：事件监听
来源：http://baike.epnwcf.com/Article/details/grrnoggdd.sHtML

el.addEventListener("click", e => {})
来源：http://baike.yfazqb.com/Article/details/gwfeocicy.sHtML

[U100] JS：DOM 查询
来源：http://mobile.yfazqb.com/Article/details/glvvpxrgk.sHtML

document.querySelector(".item")
来源：http://baike.vehdjk.com/Article/details/gnpuqntdh.sHtML

[U101] JS：classList 操作
来源：http://3g.tarul.cn/Article/details/gfswoykbg.sHtML

el.classList.toggle("active")
来源：http://3g.fktsv.cn/Article/details/gdliuvkpc.sHtML

[U102] JS：本地存储
来源：http://baike.sjlbkw.cn/Article/details/gxmwliknr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.yfazqb.com/Article/details/gnjirpsxl.sHtML

[U103] JS：定时器
来源：http://www.m.share.epnwcf.com/Article/details/gknxukdil.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.epnwcf.com/Article/details/gvdzldpkh.sHtML

[U104] JS：防抖
来源：http://mobile.vehdjk.com/Article/details/gdbgnvpig.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/gjfouxmbl.sHtML

[U105] JS：节流
来源：http://3g.sjlbkw.cn/Article/details/gsqocvade.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fktsv.cn/Article/details/gpxkfwrcx.sHtML

[U106] JS：日期格式化
来源：http://wap.bbcook.cn/Article/details/gofuuukbr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.yfazqb.com/Article/details/grmwhzbhf.sHtML

[U107] JS：数字千分位
来源：http://baike.tarul.cn/Article/details/gqxxqcxkp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.vehdjk.com/Article/details/gomwtvrhg.sHtML

[U108] JS：随机整数
来源：http://blog.bbcook.cn/Article/details/gukolcwhm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.vehdjk.com/Article/details/ggkzocyht.sHtML

[U109] JS：数组分组
来源：http://read.share.vehdjk.com/Article/details/gxqiktzvh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.bbcook.cn/Article/details/gqnsjayxm.sHtML

[U110] JS：数组分块
来源：http://mobile.sjlbkw.cn/Article/details/gdejilaan.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.yfazqb.com/Article/details/gcsatmyhv.sHtML

[U111] JS：对象转 Map
来源：http://blog.epnwcf.com/Article/details/gxvgomaso.sHtML

new Map(Object.entries(obj))
来源：http://wap.vehdjk.com/Article/details/geapmkmih.sHtML

[U112] JS：字符串补位
来源：http://wap.epnwcf.com/Article/details/gojdqklqi.sHtML

"7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/glydhdhjt.sHtML

[U113] JS：正则替换全部
来源：http://read.share.bbcook.cn/Article/details/gslazftkj.sHtML

s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/ghcpoqzvg.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.vehdjk.com/Article/details/gelcukpaq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fktsv.cn/Article/details/gokrmgtoi.sHtML

[U115] JS：生成 UUID
来源：http://read.share.yfazqb.com/Article/details/gjwlturem.sHtML

crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/ggpjqmkbt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.epnwcf.com/Article/details/gbifxudnr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fktsv.cn/Article/details/gmlrnrpjc.sHtML

[U117] JS：单元测试
来源：http://m.share.bbcook.cn/Article/details/gttizrptl.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.yfazqb.com/Article/details/gmiztpwux.sHtML

[U118] JS：开发服务器
来源：http://www.blog.vehdjk.com/Article/details/gyjwozgyu.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.epnwcf.com/Article/details/gbwyfannm.sHtML

[U119] JS：生产构建
来源：http://www.m.share.epnwcf.com/Article/details/glrrkrksl.sHtML

npx vite build
来源：http://3g.epnwcf.com/Article/details/gfjxzfmdh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.epnwcf.com/Article/details/gidyxxjfs.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.tarul.cn/Article/details/ggcpumxff.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gctjnhbas.sHtML

统计汇总
来源：http://wap.bbcook.cn/Article/details/gqlutcntg.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gzqorwzbi.sHtML

按语言统计（条）：
来源：http://baike.sjlbkw.cn/Article/details/gjaizyfzs.sHtML

Python ......... 252
来源：http://wap.yfazqb.com/Article/details/gmdzxysgs.sHtML

PHP ............ 252
来源：http://mobile.sjlbkw.cn/Article/details/gtiyqwsrv.sHtML

JavaScript ..... 252
来源：http://read.share.vehdjk.com/Article/details/grvqfcccy.sHtML

TypeScript ..... 212
来源：http://baike.vehdjk.com/Article/details/gohqcpnjx.sHtML

Java ........... 212
来源：http://blog.epnwcf.com/Article/details/guxorgppr.sHtML

Go ............. 212
来源：http://wap.bbcook.cn/Article/details/gtntjpqow.sHtML

Ruby ........... 212
来源：http://www.share.yfazqb.com/Article/details/gawpshuca.sHtML

C# ............. 212
来源：http://m.share.epnwcf.com/Article/details/geuyomatu.sHtML

C .............. 30
来源：http://m.share.epnwcf.com/Article/details/gqnuwkgze.sHtML

C++ ............ 30
来源：http://blog.sjlbkw.cn/Article/details/gjlifmcat.sHtML

SQL ............ 90
来源：http://www.share.tarul.cn/Article/details/ghnodhnbj.sHtML

Bash ........... 80
来源：http://wap.vehdjk.com/Article/details/gotafqxrq.sHtML

Kotlin ......... 15
来源：http://blog.fktsv.cn/Article/details/guextrmuo.sHtML

Swift .......... 15
来源：http://blog.sjlbkw.cn/Article/details/gdestgumg.sHtML

Lua ............ 10
来源：http://baike.tarul.cn/Article/details/gbbxbizzr.sHtML

Perl ........... 10
来源：http://mobile.sjlbkw.cn/Article/details/gkfzopzrw.sHtML

Scala .......... 10
来源：http://www.blog.tarul.cn/Article/details/gjcdmuyky.sHtML

------------------------------------
来源：http://read.share.vehdjk.com/Article/details/gcwrewkgi.sHtML

合计 ........... 2106 条
来源：http://baike.sjlbkw.cn/Article/details/gstxvmlof.sHtML

按章节统计：
来源：http://baike.bbcook.cn/Article/details/gdvkyagcp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.vehdjk.com/Article/details/gyhgujtds.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fktsv.cn/Article/details/glewvnhml.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.bbcook.cn/Article/details/ggermyduw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fktsv.cn/Article/details/gghkkuutw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.yfazqb.com/Article/details/geqmaxrwa.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.sjlbkw.cn/Article/details/guqsnrfvm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/grsmycynd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.bbcook.cn/Article/details/gxridzgjl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.epnwcf.com/Article/details/gnfzclwil.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fktsv.cn/Article/details/gdolfccvt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/gkvkyrbhc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gdutxrrsm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/gcgqkdmpa.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.yfazqb.com/Article/details/gcvgbhdbi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fktsv.cn/Article/details/gsujfrlhx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/goacpdlcu.sHtML

Q SQL 专题                              90
来源：http://baike.yfazqb.com/Article/details/gtkmsgzpx.sHtML

R Bash 专题                             80
来源：http://blog.epnwcf.com/Article/details/gdptbtced.sHtML

S C / C++ 专题                          60
来源：http://www.blog.tarul.cn/Article/details/gzxftzakr.sHtML

T 其他语言补充                          60
来源：http://m.share.vehdjk.com/Article/details/gkkwydeud.sHtML

U 高频实用片段                         120
来源：http://m.share.sjlbkw.cn/Article/details/ggvqqnrug.sHtML

------------------------------------
来源：http://wap.tarul.cn/Article/details/gamhhdsxt.sHtML

合计                                  2106 条
来源：http://m.share.sjlbkw.cn/Article/details/gqmxrqkld.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gaibfckwm.sHtML

使用提醒
来源：http://wap.bbcook.cn/Article/details/gpkajgxbp.sHtML

--------------------------------------------------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/gxjcprszr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.vehdjk.com/Article/details/gzqberzsn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.epnwcf.com/Article/details/gnhssektd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.tarul.cn/Article/details/gvmdpftcg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.yfazqb.com/Article/details/geuvwiwvc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fktsv.cn/Article/details/gwtbidqef.sHtML

—— 文件结束 ——
来源：http://mobile.bbcook.cn/Article/details/ggfszywui.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gylfverwh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fktsv.cn/Article/details/gnxhfxfqd.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fktsv.cn/Article/details/gamrmfgua.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gpfbexart.sHtML

【收录内容】
来源：http://baike.sjlbkw.cn/Article/details/gjhshpehn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.sjlbkw.cn/Article/details/gswzuelpw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.sjlbkw.cn/Article/details/gvxtfcmue.sHtML

SQL · Bash · C · C++
来源：http://baike.vehdjk.com/Article/details/ggrhemlgb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.bbcook.cn/Article/details/gddjbpusx.sHtML

【使用说明】
来源：http://www.share.bbcook.cn/Article/details/gucqjlyto.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.vehdjk.com/Article/details/gdvbhvlkq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.bbcook.cn/Article/details/gwomiqyfu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.bbcook.cn/Article/details/gtwgypjzh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.sjlbkw.cn/Article/details/gauopndsu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.vehdjk.com/Article/details/ggvothqzq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fktsv.cn/Article/details/gsmnykhpe.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.tarul.cn/Article/details/gjglnkgcj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.yfazqb.com/Article/details/gkaxpqyoh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fktsv.cn/Article/details/gyqutmkaa.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.epnwcf.com/Article/details/gavfgvrou.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.yfazqb.com/Article/details/gjdzfubht.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.yfazqb.com/Article/details/guqoxkgfd.sHtML

【文件统计】
来源：http://mobile.vehdjk.com/Article/details/gwwifpxam.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fktsv.cn/Article/details/gmozsfjbr.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gleslbmiv.sHtML

目  录
来源：http://wap.fktsv.cn/Article/details/gejvpbmon.sHtML

--------------------------------------------------------------------------------
来源：http://3g.yfazqb.com/Article/details/gpvpsjzff.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.yfazqb.com/Article/details/gsktscgfz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.vehdjk.com/Article/details/gxsygfpjd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fktsv.cn/Article/details/gramidlif.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.sjlbkw.cn/Article/details/gfnhbdxni.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.bbcook.cn/Article/details/gjnedijiu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.yfazqb.com/Article/details/ghbvixsjg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.bbcook.cn/Article/details/ghkakxzdq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.epnwcf.com/Article/details/gnbbrvmlq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/gxysjovuw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.yfazqb.com/Article/details/grychinlw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.sjlbkw.cn/Article/details/gndjcqnky.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.tarul.cn/Article/details/ghbgpdhvm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.yfazqb.com/Article/details/gmojxrhkr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.sjlbkw.cn/Article/details/gzqrnvgrv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.tarul.cn/Article/details/gyzcopbkp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/gusyfpqya.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.epnwcf.com/Article/details/gjtkkzdoj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.tarul.cn/Article/details/gcxpvblum.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.epnwcf.com/Article/details/gohlyedyz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/gbdefxfno.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/gikawrnyg.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gdqcpobgb.sHtML

A. 基础语法与类型
来源：http://www.m.share.vehdjk.com/Article/details/gfdvmuptk.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gemefgwms.sHtML

[A01] Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gwdqsjuhf.sHtML

Py:   print("Hello, World!")
来源：http://m.share.tarul.cn/Article/details/ggnnblvpi.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.vehdjk.com/Article/details/gqkwecuhs.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.yfazqb.com/Article/details/gfsescnjv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.epnwcf.com/Article/details/gxgndqqqw.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.bbcook.cn/Article/details/glsuadbva.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.tarul.cn/Article/details/gletfzdqs.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.bbcook.cn/Article/details/gpakrxurz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.bbcook.cn/Article/details/gijcbxgts.sHtML

[A02] 变量声明与赋值
来源：http://3g.bbcook.cn/Article/details/goefdkdej.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.epnwcf.com/Article/details/gpuwggfld.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.yfazqb.com/Article/details/gfohkkupu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.tarul.cn/Article/details/gjtgiyghy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.yfazqb.com/Article/details/glkdufare.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.sjlbkw.cn/Article/details/gzkfxzqae.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fktsv.cn/Article/details/gmfnxmcah.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.bbcook.cn/Article/details/gthqhjocg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.tarul.cn/Article/details/gqofpbjqv.sHtML

[A03] 常量定义
来源：http://blog.vehdjk.com/Article/details/gienldxqv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.tarul.cn/Article/details/glcqfcfsh.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.yfazqb.com/Article/details/gbhwzguth.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/ggdjzeezn.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gwmtcjrac.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gxvfjnqqj.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.sjlbkw.cn/Article/details/gussvjlkq.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.vehdjk.com/Article/details/gmqkjbgzm.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gkvvcdrit.sHtML

[A04] 判断变量类型
来源：http://read.share.fktsv.cn/Article/details/gqibaembv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.tarul.cn/Article/details/gakeziknn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.vehdjk.com/Article/details/genrddbfk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.yfazqb.com/Article/details/gbqjqeile.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.epnwcf.com/Article/details/gkzbkzxbf.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.yfazqb.com/Article/details/gnpgoayzx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.bbcook.cn/Article/details/gnjidagos.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.yfazqb.com/Article/details/gzhwnhdji.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.sjlbkw.cn/Article/details/grkjspidl.sHtML

[A05] 整数除法与取模
来源：http://blog.epnwcf.com/Article/details/gimkxdpue.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.yfazqb.com/Article/details/gviovnzrm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.yfazqb.com/Article/details/ggceyrzkp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.tarul.cn/Article/details/ghqeydzis.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/grmgvjrjl.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.vehdjk.com/Article/details/gmdnmqjkr.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gcdkdprtt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/goaotiqyf.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.vehdjk.com/Article/details/grzyakkhs.sHtML

[A06] 字符串转数字
来源：http://www.blog.fktsv.cn/Article/details/gykqixqrg.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.bbcook.cn/Article/details/gccvlpnlj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.vehdjk.com/Article/details/gdjhkyiyy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.bbcook.cn/Article/details/gdnjszcid.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.epnwcf.com/Article/details/gphipmjvq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.epnwcf.com/Article/details/gxajdbjwt.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.epnwcf.com/Article/details/gfsesdnnz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.bbcook.cn/Article/details/gutehlncd.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.tarul.cn/Article/details/ggihggvko.sHtML

[A07] 数字转字符串
来源：http://wap.sjlbkw.cn/Article/details/ghuvsiebd.sHtML

Py:   str(42)
来源：http://wap.yfazqb.com/Article/details/gvesylxze.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fktsv.cn/Article/details/gvodqdwus.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.epnwcf.com/Article/details/gmhbrbacs.sHtML

TS:   String(42)
来源：http://read.share.vehdjk.com/Article/details/gusphtwgn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.yfazqb.com/Article/details/gxjzjyxrs.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.bbcook.cn/Article/details/gcumvtjqb.sHtML

Ruby: 42.to_s
来源：http://www.share.tarul.cn/Article/details/ggkwrsnse.sHtML

C#:   42.ToString()
来源：http://m.share.yfazqb.com/Article/details/gisgohkxa.sHtML

[A08] 取整与四舍五入
来源：http://wap.tarul.cn/Article/details/gkoetexru.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.sjlbkw.cn/Article/details/ggzhfqpqi.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fktsv.cn/Article/details/guqbbsjyr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.sjlbkw.cn/Article/details/gaoumjtce.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.tarul.cn/Article/details/gzshkscaa.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.tarul.cn/Article/details/gzsvctzxn.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvwjwtpq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.sjlbkw.cn/Article/details/gdygbrmub.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.tarul.cn/Article/details/gdcaokkgi.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fktsv.cn/Article/details/gyribrkbp.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.yfazqb.com/Article/details/gyouasomu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fktsv.cn/Article/details/gxrrxyaqu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gcovjvqkb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.yfazqb.com/Article/details/gezdppkjk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.epnwcf.com/Article/details/gdmidfulz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.bbcook.cn/Article/details/gapvbcvfy.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.vehdjk.com/Article/details/gtllazcwc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gftvzqmwu.sHtML

[A10] 生成随机数
来源：http://mobile.bbcook.cn/Article/details/gnkjufoke.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.vehdjk.com/Article/details/gbvoebxmx.sHtML

PHP:  random_int(1, 100);
来源：http://3g.yfazqb.com/Article/details/gbtspxada.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fktsv.cn/Article/details/gjcnjdauy.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fktsv.cn/Article/details/gxtqrjysb.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.tarul.cn/Article/details/gjbzagmds.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.yfazqb.com/Article/details/gvuwjakuf.sHtML

Ruby: rand(1..100)
来源：http://mobile.bbcook.cn/Article/details/gwzxskurh.sHtML


<!-- 参考信息 -->