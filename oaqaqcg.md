代发 wailian999

[U69] PHP：PDO 预处理
来源：http://3g.tarul.cn/Article/details/gsaqqsgvt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmovohoth.sHtML

[U70] PHP：PDO 事务
来源：http://wap.epnwcf.com/Article/details/gdlcynozb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.vehdjk.com/Article/details/glmtwgdkk.sHtML

[U71] PHP：抛出异常
来源：http://wap.bbcook.cn/Article/details/gdzxifnoy.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.sjlbkw.cn/Article/details/ghqcdxnzg.sHtML

[U72] PHP：写错误日志
来源：http://3g.bbcook.cn/Article/details/giosausmb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.bbcook.cn/Article/details/gbyiydgwx.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.tarul.cn/Article/details/gogxiydhg.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.bbcook.cn/Article/details/gauqdkyeh.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.vehdjk.com/Article/details/galqjboqo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.tarul.cn/Article/details/ghbhaqtlq.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.vehdjk.com/Article/details/gfajylsbf.sHtML

composer require psr/container
来源：http://blog.epnwcf.com/Article/details/gaiodhymk.sHtML

[U76] PHP：简单路由
来源：http://read.share.fktsv.cn/Article/details/gvtpxcdpo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fktsv.cn/Article/details/gwmkchaks.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fktsv.cn/Article/details/ganopkdnj.sHtML

composer require twig/twig
来源：http://m.share.bbcook.cn/Article/details/gqpzmpbgt.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhqvgjti.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.vehdjk.com/Article/details/gehppcvlt.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fktsv.cn/Article/details/gcnnrsyzo.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.sjlbkw.cn/Article/details/gccdftxzf.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.vehdjk.com/Article/details/gpgmtgmsl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.epnwcf.com/Article/details/giwunqljm.sHtML

[U81] JS：初始化项目
来源：http://mobile.vehdjk.com/Article/details/gzxfijxey.sHtML

npm init -y;  npm i express
来源：http://blog.sjlbkw.cn/Article/details/ggxehjxwd.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.epnwcf.com/Article/details/gxkhwnzju.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.yfazqb.com/Article/details/gabmabsbs.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.sjlbkw.cn/Article/details/gogxzgypt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.yfazqb.com/Article/details/gazakfipu.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.sjlbkw.cn/Article/details/gwbdeinnj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.sjlbkw.cn/Article/details/gepvvyuhh.sHtML

[U85] JS：可选链
来源：http://www.blog.bbcook.cn/Article/details/gctorfovp.sHtML

a?.b?.c
来源：http://www.share.bbcook.cn/Article/details/gpyoinett.sHtML

[U86] JS：空值合并
来源：http://blog.yfazqb.com/Article/details/gnrucvdsz.sHtML

a ?? b
来源：http://baike.fktsv.cn/Article/details/ggpehcslt.sHtML

[U87] JS：解构默认值
来源：http://www.share.sjlbkw.cn/Article/details/gwujuxovj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.epnwcf.com/Article/details/gxupvxuuk.sHtML

[U88] JS：对象展开合并
来源：http://www.share.epnwcf.com/Article/details/gtkvuvbvc.sHtML

{ ...a, ...b }
来源：http://read.share.sjlbkw.cn/Article/details/ggkfikdyt.sHtML

[U89] JS：数组去重
来源：http://blog.bbcook.cn/Article/details/gigcsmvvf.sHtML

[...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/gcaqxgohz.sHtML

[U90] JS：数字数组排序
来源：http://mobile.tarul.cn/Article/details/gozgmadzu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/ggsrvyjay.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.bbcook.cn/Article/details/galmpwgzw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.tarul.cn/Article/details/gbhlmosmg.sHtML

[U92] JS：深拷贝
来源：http://3g.bbcook.cn/Article/details/glotgtuwv.sHtML

structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gnefygigy.sHtML

[U93] JS：模板字符串
来源：http://blog.tarul.cn/Article/details/gxrvgtwcd.sHtML

`共 ${n} 条`
来源：http://3g.yfazqb.com/Article/details/gmptzxyyw.sHtML

[U94] JS：箭头函数
来源：http://3g.tarul.cn/Article/details/glrvmusow.sHtML

const double = x => x * 2;
来源：http://baike.tarul.cn/Article/details/gxwkqqrlz.sHtML

[U95] JS：Promise 包装
来源：http://3g.epnwcf.com/Article/details/gxcbfbqrs.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.vehdjk.com/Article/details/gpegqmkvw.sHtML

[U96] JS：async/await 与异常
来源：http://wap.tarul.cn/Article/details/gyfdsiwyr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/giyhtymuc.sHtML

[U97] JS：并发请求
来源：http://3g.bbcook.cn/Article/details/gpdsyltxd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gaaspdvod.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.vehdjk.com/Article/details/gxoixkjtw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.epnwcf.com/Article/details/gxtyzrqnr.sHtML

[U99] JS：事件监听
来源：http://www.m.share.vehdjk.com/Article/details/gyksibbfx.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.vehdjk.com/Article/details/gdmnvmalw.sHtML

[U100] JS：DOM 查询
来源：http://blog.epnwcf.com/Article/details/glyqdywny.sHtML

document.querySelector(".item")
来源：http://m.share.fktsv.cn/Article/details/goodbbfol.sHtML

[U101] JS：classList 操作
来源：http://wap.vehdjk.com/Article/details/gajjadtrw.sHtML

el.classList.toggle("active")
来源：http://m.share.fktsv.cn/Article/details/gexjqcaoe.sHtML

[U102] JS：本地存储
来源：http://read.share.vehdjk.com/Article/details/gwntxtshi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.epnwcf.com/Article/details/gmstdqduz.sHtML

[U103] JS：定时器
来源：http://3g.sjlbkw.cn/Article/details/ggapcxnns.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.epnwcf.com/Article/details/gjszvwkrk.sHtML

[U104] JS：防抖
来源：http://wap.bbcook.cn/Article/details/ggaiilbqd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gphzfejyr.sHtML

[U105] JS：节流
来源：http://mobile.sjlbkw.cn/Article/details/gitjzbxbj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.sjlbkw.cn/Article/details/gnswmiria.sHtML

[U106] JS：日期格式化
来源：http://baike.yfazqb.com/Article/details/gaxldxpvp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.tarul.cn/Article/details/gvujuyzbr.sHtML

[U107] JS：数字千分位
来源：http://www.share.sjlbkw.cn/Article/details/ggdqralaz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fktsv.cn/Article/details/gdmlndyny.sHtML

[U108] JS：随机整数
来源：http://baike.sjlbkw.cn/Article/details/gpxblvfbz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.sjlbkw.cn/Article/details/gfldoefdj.sHtML

[U109] JS：数组分组
来源：http://www.share.bbcook.cn/Article/details/gjoexhlbm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fktsv.cn/Article/details/gxfzonjrx.sHtML

[U110] JS：数组分块
来源：http://blog.yfazqb.com/Article/details/gfkhlnzop.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.vehdjk.com/Article/details/ghvfhctav.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.epnwcf.com/Article/details/gmsnpelms.sHtML

new Map(Object.entries(obj))
来源：http://wap.bbcook.cn/Article/details/gizvarygy.sHtML

[U112] JS：字符串补位
来源：http://3g.epnwcf.com/Article/details/ghendpksa.sHtML

"7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gyrejezok.sHtML

[U113] JS：正则替换全部
来源：http://baike.fktsv.cn/Article/details/gyhvxmhwq.sHtML

s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gkqhhfwus.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fktsv.cn/Article/details/gqrtklnck.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.bbcook.cn/Article/details/gfydgbpmh.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.tarul.cn/Article/details/gapufyrdq.sHtML

crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gemkkasvs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.tarul.cn/Article/details/gldietqdi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.yfazqb.com/Article/details/gkxeolvdh.sHtML

[U117] JS：单元测试
来源：http://www.share.yfazqb.com/Article/details/gctpyqjdn.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.vehdjk.com/Article/details/gqdcsrfvf.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fktsv.cn/Article/details/gvplpcfwo.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.sjlbkw.cn/Article/details/gyqysfwdi.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fktsv.cn/Article/details/gmrzzlflw.sHtML

npx vite build
来源：http://wap.epnwcf.com/Article/details/goriixyoe.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.tarul.cn/Article/details/gjvyhwfkv.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.tarul.cn/Article/details/gdwbqyzjf.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gbhscibqb.sHtML

统计汇总
来源：http://m.share.vehdjk.com/Article/details/gmqpxhsmf.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/grtgtzugd.sHtML

按语言统计（条）：
来源：http://3g.vehdjk.com/Article/details/ghkgcqbjw.sHtML

Python ......... 252
来源：http://m.share.yfazqb.com/Article/details/gyhuuklng.sHtML

PHP ............ 252
来源：http://m.share.bbcook.cn/Article/details/gfhcptakn.sHtML

JavaScript ..... 252
来源：http://m.share.vehdjk.com/Article/details/ggnibtdqd.sHtML

TypeScript ..... 212
来源：http://mobile.epnwcf.com/Article/details/garkcawjt.sHtML

Java ........... 212
来源：http://www.blog.sjlbkw.cn/Article/details/gjckroxid.sHtML

Go ............. 212
来源：http://m.share.bbcook.cn/Article/details/gppvrvolr.sHtML

Ruby ........... 212
来源：http://www.share.epnwcf.com/Article/details/gycqdwvne.sHtML

C# ............. 212
来源：http://blog.sjlbkw.cn/Article/details/gxxtwnmdq.sHtML

C .............. 30
来源：http://blog.vehdjk.com/Article/details/gvnqknpbs.sHtML

C++ ............ 30
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjgcdghs.sHtML

SQL ............ 90
来源：http://read.share.epnwcf.com/Article/details/gkvjvgddn.sHtML

Bash ........... 80
来源：http://3g.bbcook.cn/Article/details/gdrsgxdps.sHtML

Kotlin ......... 15
来源：http://www.m.share.epnwcf.com/Article/details/gtagtevrn.sHtML

Swift .......... 15
来源：http://www.blog.fktsv.cn/Article/details/gldzabuev.sHtML

Lua ............ 10
来源：http://www.blog.fktsv.cn/Article/details/gjawofmjb.sHtML

Perl ........... 10
来源：http://mobile.epnwcf.com/Article/details/gaipwgwpq.sHtML

Scala .......... 10
来源：http://m.share.fktsv.cn/Article/details/giapcxzxs.sHtML

------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gwyzqkjxg.sHtML

合计 ........... 2106 条
来源：http://www.blog.sjlbkw.cn/Article/details/gzhsjftqi.sHtML

按章节统计：
来源：http://www.m.share.bbcook.cn/Article/details/gnlzlvlww.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.epnwcf.com/Article/details/gtekqbvhf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.yfazqb.com/Article/details/gufypvohc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.sjlbkw.cn/Article/details/glmhtikny.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.bbcook.cn/Article/details/gddgbbbha.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fktsv.cn/Article/details/gbhesugac.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fktsv.cn/Article/details/goovxudou.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.vehdjk.com/Article/details/gmnrnidol.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.tarul.cn/Article/details/gfesbgplz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/gslptmirw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.bbcook.cn/Article/details/gmykotwtm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gzzvrnjtu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.epnwcf.com/Article/details/gtncnbmuw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gnmwnxsig.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.epnwcf.com/Article/details/gkiqcobfw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.epnwcf.com/Article/details/gzkzbtlsy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/gydjrirfs.sHtML

Q SQL 专题                              90
来源：http://www.share.bbcook.cn/Article/details/gdikppkkm.sHtML

R Bash 专题                             80
来源：http://baike.sjlbkw.cn/Article/details/ghdjnfphq.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.bbcook.cn/Article/details/gkopjidap.sHtML

T 其他语言补充                          60
来源：http://wap.vehdjk.com/Article/details/gslbvrcsv.sHtML

U 高频实用片段                         120
来源：http://mobile.sjlbkw.cn/Article/details/gttxgierw.sHtML

------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gjkoxdfrx.sHtML

合计                                  2106 条
来源：http://read.share.tarul.cn/Article/details/gmybdcxcb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/ghmpgqmeb.sHtML

使用提醒
来源：http://3g.sjlbkw.cn/Article/details/ggxthlxrb.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gamckjdoi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.yfazqb.com/Article/details/gdyvnrnai.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.sjlbkw.cn/Article/details/gewdnpjoc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.epnwcf.com/Article/details/ggccjpmfw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fktsv.cn/Article/details/gqpjpodua.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.tarul.cn/Article/details/gmqjwozlm.sHtML

—— 文件结束 ——
来源：http://mobile.tarul.cn/Article/details/gjnqkzwfh.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gppnfwnxv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.epnwcf.com/Article/details/gikzhmpgz.sHtML

Common Programming Examples Cheat Book
来源：http://blog.vehdjk.com/Article/details/ganfapgea.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/glzkfqhfn.sHtML

【收录内容】
来源：http://www.blog.epnwcf.com/Article/details/gwidmdxdo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.vehdjk.com/Article/details/gbvszaxqc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.bbcook.cn/Article/details/gjmvvzdhn.sHtML

SQL · Bash · C · C++
来源：http://www.blog.yfazqb.com/Article/details/ggworzzvd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.tarul.cn/Article/details/gxktsnyko.sHtML

【使用说明】
来源：http://m.share.bbcook.cn/Article/details/gcvgmgkwl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.epnwcf.com/Article/details/gxfruofbl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fktsv.cn/Article/details/gjrmxozaz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.bbcook.cn/Article/details/glfbbxqbx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.yfazqb.com/Article/details/gojpisvzc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.yfazqb.com/Article/details/gumxoqoie.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.bbcook.cn/Article/details/gtbiywplr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.tarul.cn/Article/details/guigcezew.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.tarul.cn/Article/details/gthejqsrl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.yfazqb.com/Article/details/gpclolyyd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.sjlbkw.cn/Article/details/graqmmjii.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fktsv.cn/Article/details/gfsfqdlxv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.vehdjk.com/Article/details/gdvjffwbn.sHtML

【文件统计】
来源：http://www.share.tarul.cn/Article/details/gvswntcaz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.bbcook.cn/Article/details/gwyvlxufa.sHtML

--------------------------------------------------------------------------------
来源：http://baike.vehdjk.com/Article/details/grkqdqhbf.sHtML

目  录
来源：http://www.share.tarul.cn/Article/details/gkdmmqcro.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gzfxfrkez.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.sjlbkw.cn/Article/details/gkegvucvn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.vehdjk.com/Article/details/gdbgpjxxq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.sjlbkw.cn/Article/details/gbxebxido.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.sjlbkw.cn/Article/details/ggbzveqth.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.sjlbkw.cn/Article/details/gnugyaelr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.bbcook.cn/Article/details/gpijhtzcw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.yfazqb.com/Article/details/gevtmkvma.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.tarul.cn/Article/details/gflpnoeyf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.yfazqb.com/Article/details/gjhraiefh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.epnwcf.com/Article/details/gmgilcjql.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.sjlbkw.cn/Article/details/gmpdzxqov.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.vehdjk.com/Article/details/gcpfkprhv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/gnvnttnys.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.tarul.cn/Article/details/grexdnhpo.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.vehdjk.com/Article/details/gkuwvkljl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.vehdjk.com/Article/details/gnadvenms.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.epnwcf.com/Article/details/gjceignqh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.bbcook.cn/Article/details/gsejglvcb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.vehdjk.com/Article/details/gqijvcuvy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.epnwcf.com/Article/details/gvnorwibo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fktsv.cn/Article/details/gigvaiyhw.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ghvwsoizl.sHtML

A. 基础语法与类型
来源：http://www.share.sjlbkw.cn/Article/details/gcoyvrsmd.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gkgumffqw.sHtML

[A01] Hello World
来源：http://3g.tarul.cn/Article/details/gviivkwbu.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fktsv.cn/Article/details/gitulzmfn.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.tarul.cn/Article/details/gdwzuggeg.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.tarul.cn/Article/details/gadjtlrjy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.sjlbkw.cn/Article/details/gkgascgph.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fktsv.cn/Article/details/ggrsrpjtn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.bbcook.cn/Article/details/gnuglvsbd.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.vehdjk.com/Article/details/gucqtbxbg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.sjlbkw.cn/Article/details/gnprqasds.sHtML

[A02] 变量声明与赋值
来源：http://mobile.epnwcf.com/Article/details/gbdvepjlg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.vehdjk.com/Article/details/ghjbnlwyf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.vehdjk.com/Article/details/gczcbzgfs.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.bbcook.cn/Article/details/gcxpavwpn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.bbcook.cn/Article/details/gwehcifng.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gfzqdbvcm.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.bbcook.cn/Article/details/gkychxmqs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.bbcook.cn/Article/details/gylwenobr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/goxjisgci.sHtML

[A03] 常量定义
来源：http://www.share.tarul.cn/Article/details/gwqlyunap.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.vehdjk.com/Article/details/gyncrkmhu.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gkubguvhj.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/ggsdqqxgo.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fktsv.cn/Article/details/gnkssqdvw.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/grsyhwduf.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.yfazqb.com/Article/details/gursnmfuk.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fktsv.cn/Article/details/gsfdoorjv.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gfjtvxpoj.sHtML

[A04] 判断变量类型
来源：http://baike.epnwcf.com/Article/details/gvleuxkec.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fktsv.cn/Article/details/giaurlcht.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.sjlbkw.cn/Article/details/gativbxyv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.sjlbkw.cn/Article/details/ggbavxkii.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.epnwcf.com/Article/details/gmdkdnlvr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.sjlbkw.cn/Article/details/gdudrqbtg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.yfazqb.com/Article/details/gfoxedeod.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.epnwcf.com/Article/details/gqxttttod.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fktsv.cn/Article/details/gcpzfdcve.sHtML

[A05] 整数除法与取模
来源：http://m.share.tarul.cn/Article/details/goshekztg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.sjlbkw.cn/Article/details/geyydydyl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.yfazqb.com/Article/details/gqruryxxu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fktsv.cn/Article/details/gpalaxury.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.sjlbkw.cn/Article/details/gacrsmczx.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.bbcook.cn/Article/details/gedoubvwu.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/gmsmljzbp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.sjlbkw.cn/Article/details/gnltfjqpw.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.yfazqb.com/Article/details/gphceesio.sHtML

[A06] 字符串转数字
来源：http://baike.tarul.cn/Article/details/gihbiqsdz.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.epnwcf.com/Article/details/gepsowqso.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.sjlbkw.cn/Article/details/gmlzikoxs.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.epnwcf.com/Article/details/gfkgcofdr.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.bbcook.cn/Article/details/grrtlrzxv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.bbcook.cn/Article/details/gvppszdyd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.epnwcf.com/Article/details/gzpjsfyqh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.tarul.cn/Article/details/gbqexkfjy.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fktsv.cn/Article/details/gyeviabgn.sHtML

[A07] 数字转字符串
来源：http://blog.fktsv.cn/Article/details/gwogbuywv.sHtML

Py:   str(42)
来源：http://www.m.share.fktsv.cn/Article/details/gmtgahwmu.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.bbcook.cn/Article/details/gmobrgiwq.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.bbcook.cn/Article/details/gendkgzug.sHtML

TS:   String(42)
来源：http://blog.yfazqb.com/Article/details/gjrzcfdxl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.yfazqb.com/Article/details/glnzknllh.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fktsv.cn/Article/details/gomegillx.sHtML

Ruby: 42.to_s
来源：http://www.share.tarul.cn/Article/details/gkfwesnfm.sHtML

C#:   42.ToString()
来源：http://read.share.sjlbkw.cn/Article/details/gmvldplsk.sHtML

[A08] 取整与四舍五入
来源：http://baike.fktsv.cn/Article/details/gkugxlfym.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.yfazqb.com/Article/details/gytndzhfu.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.epnwcf.com/Article/details/gpnubgozm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.epnwcf.com/Article/details/gioxqcozh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.epnwcf.com/Article/details/gqismxprw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.vehdjk.com/Article/details/goxoythve.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.tarul.cn/Article/details/gblegzhsp.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.tarul.cn/Article/details/gsmvaecht.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.sjlbkw.cn/Article/details/gmnsjcanb.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.yfazqb.com/Article/details/gynhrooaj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/glmbfyqys.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.bbcook.cn/Article/details/gatilmstu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gxbnzucgi.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gzjrospni.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gkecbqkcd.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.vehdjk.com/Article/details/glzepvyjs.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.yfazqb.com/Article/details/gpeirjciy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.epnwcf.com/Article/details/gyxvyxias.sHtML

[A10] 生成随机数
来源：http://blog.tarul.cn/Article/details/gwkplnvyn.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fktsv.cn/Article/details/gkunvolof.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.bbcook.cn/Article/details/gfqfsmhbn.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.vehdjk.com/Article/details/gzepfinvx.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.vehdjk.com/Article/details/grqqiljeq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.epnwcf.com/Article/details/gegsfimxl.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.sjlbkw.cn/Article/details/gcywzvubw.sHtML

Ruby: rand(1..100)
来源：http://mobile.sjlbkw.cn/Article/details/gqrlgmiee.sHtML


<!-- 参考信息 -->