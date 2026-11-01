代发 wailian999

[U67] PHP：处理文件上传
来源：http://baike.fktsv.cn/Article/details/gpxeuoqkj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.sjlbkw.cn/Article/details/gczugpnsn.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.sjlbkw.cn/Article/details/gcncsuvez.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.epnwcf.com/Article/details/gfnozoiip.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.sjlbkw.cn/Article/details/gowgcnsqq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.epnwcf.com/Article/details/gkzjwywqj.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.bbcook.cn/Article/details/gimmvwazt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.sjlbkw.cn/Article/details/gcxicqvoi.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.bbcook.cn/Article/details/ghrvoabdx.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.bbcook.cn/Article/details/gyexpojuq.sHtML

[U72] PHP：写错误日志
来源：http://3g.fktsv.cn/Article/details/gcxhrhqnr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.bbcook.cn/Article/details/ghegynifv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.tarul.cn/Article/details/gmuacegdh.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.yfazqb.com/Article/details/gjiiruwix.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gnsfvxozk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.tarul.cn/Article/details/grmqwuyoh.sHtML

[U75] PHP：依赖注入
来源：http://mobile.tarul.cn/Article/details/glopibera.sHtML

composer require psr/container
来源：http://wap.vehdjk.com/Article/details/goxhkpmks.sHtML

[U76] PHP：简单路由
来源：http://baike.sjlbkw.cn/Article/details/ggpjoxgin.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.yfazqb.com/Article/details/ggomflpvx.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.yfazqb.com/Article/details/goetnfeon.sHtML

composer require twig/twig
来源：http://www.blog.vehdjk.com/Article/details/gvldduhjm.sHtML

[U78] PHP：单元测试
来源：http://www.blog.yfazqb.com/Article/details/gtjxdpjks.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.bbcook.cn/Article/details/gkwghrwpv.sHtML

[U79] PHP：静态分析
来源：http://baike.sjlbkw.cn/Article/details/gvgbtosli.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.sjlbkw.cn/Article/details/gkdcyikjt.sHtML

[U80] PHP：代码规范修复
来源：http://3g.vehdjk.com/Article/details/gpatnwisf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.epnwcf.com/Article/details/gsmftcjcj.sHtML

[U81] JS：初始化项目
来源：http://m.share.tarul.cn/Article/details/gzwyotfiu.sHtML

npm init -y;  npm i express
来源：http://read.share.yfazqb.com/Article/details/grlyapvpr.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.vehdjk.com/Article/details/gzyxdrtbe.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.yfazqb.com/Article/details/gvmbbbizx.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.sjlbkw.cn/Article/details/gukjmzuey.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.bbcook.cn/Article/details/gslcdmpys.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fktsv.cn/Article/details/gblgqbpjr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fktsv.cn/Article/details/gkffijryp.sHtML

[U85] JS：可选链
来源：http://www.blog.fktsv.cn/Article/details/geuitfotr.sHtML

a?.b?.c
来源：http://3g.bbcook.cn/Article/details/grsahuwis.sHtML

[U86] JS：空值合并
来源：http://wap.sjlbkw.cn/Article/details/glqazfjus.sHtML

a ?? b
来源：http://3g.yfazqb.com/Article/details/ghahhyprv.sHtML

[U87] JS：解构默认值
来源：http://www.share.epnwcf.com/Article/details/gbdaxrlre.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.epnwcf.com/Article/details/gohxluyuw.sHtML

[U88] JS：对象展开合并
来源：http://read.share.bbcook.cn/Article/details/gskdaeydn.sHtML

{ ...a, ...b }
来源：http://www.m.share.yfazqb.com/Article/details/gsjigcpar.sHtML

[U89] JS：数组去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gqeraoafr.sHtML

[...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/gtmuzhobe.sHtML

[U90] JS：数字数组排序
来源：http://m.share.sjlbkw.cn/Article/details/gjxgrffyp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gazffpger.sHtML

[U91] JS：对象键值遍历
来源：http://3g.vehdjk.com/Article/details/gcedshmde.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.epnwcf.com/Article/details/gddxqodyf.sHtML

[U92] JS：深拷贝
来源：http://wap.tarul.cn/Article/details/gjukscdqa.sHtML

structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gmddiwckc.sHtML

[U93] JS：模板字符串
来源：http://3g.yfazqb.com/Article/details/gfaxhrnbv.sHtML

`共 ${n} 条`
来源：http://m.share.epnwcf.com/Article/details/gwfvyyjmb.sHtML

[U94] JS：箭头函数
来源：http://mobile.fktsv.cn/Article/details/gywuelieo.sHtML

const double = x => x * 2;
来源：http://wap.bbcook.cn/Article/details/gsjgjvvoi.sHtML

[U95] JS：Promise 包装
来源：http://www.share.sjlbkw.cn/Article/details/gfkernatv.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fktsv.cn/Article/details/ggtwcydoy.sHtML

[U96] JS：async/await 与异常
来源：http://3g.vehdjk.com/Article/details/gxpotxodj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gpieqgwmy.sHtML

[U97] JS：并发请求
来源：http://www.share.fktsv.cn/Article/details/gpgtbbeii.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gdalkgutn.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.sjlbkw.cn/Article/details/gqglvyhpy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.vehdjk.com/Article/details/gymxvzpaa.sHtML

[U99] JS：事件监听
来源：http://www.blog.tarul.cn/Article/details/glyetffef.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.tarul.cn/Article/details/gcopnqfau.sHtML

[U100] JS：DOM 查询
来源：http://www.share.sjlbkw.cn/Article/details/gklcrvnec.sHtML

document.querySelector(".item")
来源：http://baike.tarul.cn/Article/details/ghmzfkclf.sHtML

[U101] JS：classList 操作
来源：http://blog.tarul.cn/Article/details/gegvmakoz.sHtML

el.classList.toggle("active")
来源：http://m.share.tarul.cn/Article/details/gfeeuhepw.sHtML

[U102] JS：本地存储
来源：http://www.share.tarul.cn/Article/details/gzhdekzpc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.tarul.cn/Article/details/gogbjxavi.sHtML

[U103] JS：定时器
来源：http://www.blog.yfazqb.com/Article/details/gqplzrlec.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fktsv.cn/Article/details/gymwyyzuy.sHtML

[U104] JS：防抖
来源：http://wap.fktsv.cn/Article/details/gfqmvlcoo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/gmmfalttp.sHtML

[U105] JS：节流
来源：http://www.blog.bbcook.cn/Article/details/gntszgyxj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.vehdjk.com/Article/details/gwbbxvtmw.sHtML

[U106] JS：日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gyxhgfaoh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fktsv.cn/Article/details/gptqimwyd.sHtML

[U107] JS：数字千分位
来源：http://baike.yfazqb.com/Article/details/gfppuxsyo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fktsv.cn/Article/details/gjqueruza.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fktsv.cn/Article/details/gkqiifuyn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.sjlbkw.cn/Article/details/gnunjslvl.sHtML

[U109] JS：数组分组
来源：http://3g.yfazqb.com/Article/details/gestwgwou.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.yfazqb.com/Article/details/gryzedicv.sHtML

[U110] JS：数组分块
来源：http://baike.bbcook.cn/Article/details/gfvcupnln.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.sjlbkw.cn/Article/details/giqnmujis.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxasjhha.sHtML

new Map(Object.entries(obj))
来源：http://wap.vehdjk.com/Article/details/glglkvwde.sHtML

[U112] JS：字符串补位
来源：http://www.blog.vehdjk.com/Article/details/gsmamfnba.sHtML

"7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gonjniiuq.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.tarul.cn/Article/details/guqeqvoun.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gfwrlzvuq.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.bbcook.cn/Article/details/gzstxiote.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.vehdjk.com/Article/details/gnhzzzdnb.sHtML

[U115] JS：生成 UUID
来源：http://baike.sjlbkw.cn/Article/details/gtzclbubn.sHtML

crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gkymptdra.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.yfazqb.com/Article/details/gjvwoqdox.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fktsv.cn/Article/details/gjamnrorn.sHtML

[U117] JS：单元测试
来源：http://blog.sjlbkw.cn/Article/details/glnmutkbe.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.vehdjk.com/Article/details/gsnqnwhwf.sHtML

[U118] JS：开发服务器
来源：http://mobile.yfazqb.com/Article/details/gvrzcyang.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.bbcook.cn/Article/details/gbmmsngyv.sHtML

[U119] JS：生产构建
来源：http://wap.epnwcf.com/Article/details/gtrrbjoco.sHtML

npx vite build
来源：http://www.blog.vehdjk.com/Article/details/gdfncxdmj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.vehdjk.com/Article/details/gwxtkjhfc.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.tarul.cn/Article/details/ghsneeamg.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gwbxuklde.sHtML

统计汇总
来源：http://read.share.yfazqb.com/Article/details/guqxkkidc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gmxoxkjai.sHtML

按语言统计（条）：
来源：http://wap.bbcook.cn/Article/details/ggboaiqkm.sHtML

Python ......... 252
来源：http://www.blog.bbcook.cn/Article/details/gkyyjkovs.sHtML

PHP ............ 252
来源：http://www.share.sjlbkw.cn/Article/details/gyrhygbft.sHtML

JavaScript ..... 252
来源：http://read.share.yfazqb.com/Article/details/gvlqlgaoj.sHtML

TypeScript ..... 212
来源：http://baike.fktsv.cn/Article/details/grxgfdcyo.sHtML

Java ........... 212
来源：http://3g.fktsv.cn/Article/details/gmdcqaxiy.sHtML

Go ............. 212
来源：http://www.blog.tarul.cn/Article/details/gedvclspf.sHtML

Ruby ........... 212
来源：http://www.blog.tarul.cn/Article/details/gtbmvitnl.sHtML

C# ............. 212
来源：http://baike.sjlbkw.cn/Article/details/gntcqjuyw.sHtML

C .............. 30
来源：http://3g.bbcook.cn/Article/details/gwyvrazgb.sHtML

C++ ............ 30
来源：http://blog.bbcook.cn/Article/details/giwgdnuhm.sHtML

SQL ............ 90
来源：http://blog.epnwcf.com/Article/details/gopsmerhk.sHtML

Bash ........... 80
来源：http://wap.fktsv.cn/Article/details/gjrbubegx.sHtML

Kotlin ......... 15
来源：http://3g.fktsv.cn/Article/details/gfzoutabj.sHtML

Swift .......... 15
来源：http://blog.bbcook.cn/Article/details/gkndxbmhz.sHtML

Lua ............ 10
来源：http://www.m.share.fktsv.cn/Article/details/gyllygebe.sHtML

Perl ........... 10
来源：http://www.share.fktsv.cn/Article/details/gglvsgtqf.sHtML

Scala .......... 10
来源：http://3g.sjlbkw.cn/Article/details/gsexxfpee.sHtML

------------------------------------
来源：http://blog.vehdjk.com/Article/details/gmynkzlzt.sHtML

合计 ........... 2106 条
来源：http://www.m.share.bbcook.cn/Article/details/gpeehubrz.sHtML

按章节统计：
来源：http://www.blog.yfazqb.com/Article/details/gcmupzvxt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.vehdjk.com/Article/details/gjsoejwbd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fktsv.cn/Article/details/ggcporxze.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fktsv.cn/Article/details/gdfyzllpz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.tarul.cn/Article/details/gmvhydycp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.epnwcf.com/Article/details/gepnjjqpr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.vehdjk.com/Article/details/gkobepwbx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/gtxkblqls.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.vehdjk.com/Article/details/girlayxgr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gwbmkdwyl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.epnwcf.com/Article/details/gmgewnwlk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/goanmixhx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/goyummivk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gactgklzj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.yfazqb.com/Article/details/gvssshekb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fktsv.cn/Article/details/grkbarhbo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gokcdhdzu.sHtML

Q SQL 专题                              90
来源：http://www.m.share.vehdjk.com/Article/details/gbgkzwuga.sHtML

R Bash 专题                             80
来源：http://3g.tarul.cn/Article/details/gnsxpylmw.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.epnwcf.com/Article/details/gdttmbhoh.sHtML

T 其他语言补充                          60
来源：http://3g.sjlbkw.cn/Article/details/gkerovylm.sHtML

U 高频实用片段                         120
来源：http://read.share.yfazqb.com/Article/details/gnvbblgaf.sHtML

------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gaqcudoor.sHtML

合计                                  2106 条
来源：http://www.blog.bbcook.cn/Article/details/goywghbas.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/gaggdmhfr.sHtML

使用提醒
来源：http://www.share.epnwcf.com/Article/details/gpaquycto.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gyislxusa.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fktsv.cn/Article/details/giwnwkxxg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.tarul.cn/Article/details/ggdanolbw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.tarul.cn/Article/details/gdunjdtwl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.tarul.cn/Article/details/gnkpylcdr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.sjlbkw.cn/Article/details/ggzuzshao.sHtML

—— 文件结束 ——
来源：http://mobile.vehdjk.com/Article/details/gabodaqwc.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gylqmnsjb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.sjlbkw.cn/Article/details/gplpgchxh.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.epnwcf.com/Article/details/ghuqmhytf.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gfwatwosm.sHtML

【收录内容】
来源：http://baike.vehdjk.com/Article/details/gahisfwbh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.sjlbkw.cn/Article/details/gojmifjge.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.epnwcf.com/Article/details/gclixbvva.sHtML

SQL · Bash · C · C++
来源：http://www.blog.bbcook.cn/Article/details/gwxxiymht.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.yfazqb.com/Article/details/gbuxnoezf.sHtML

【使用说明】
来源：http://m.share.vehdjk.com/Article/details/gctqcsbpa.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.bbcook.cn/Article/details/gougyvrqg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.vehdjk.com/Article/details/gykyftlvc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.epnwcf.com/Article/details/gsbiwbxrw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fktsv.cn/Article/details/gnwrazgkh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.vehdjk.com/Article/details/grgpuvhfh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.sjlbkw.cn/Article/details/gpuzuhrdd.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.epnwcf.com/Article/details/ginomxxou.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.vehdjk.com/Article/details/gsnnegdae.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.vehdjk.com/Article/details/gayebrrks.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.vehdjk.com/Article/details/gqlzebydj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.yfazqb.com/Article/details/gsfvzymdv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.sjlbkw.cn/Article/details/gfdsougmm.sHtML

【文件统计】
来源：http://www.share.yfazqb.com/Article/details/grljxyyey.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fktsv.cn/Article/details/grdowikur.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/gbdeiujwp.sHtML

目  录
来源：http://blog.vehdjk.com/Article/details/gmfubhasv.sHtML

--------------------------------------------------------------------------------
来源：http://blog.epnwcf.com/Article/details/gubtoianv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.epnwcf.com/Article/details/glpappsej.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.bbcook.cn/Article/details/gtrkcufec.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.tarul.cn/Article/details/gsrhyfolk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.yfazqb.com/Article/details/gjxtsbaba.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.yfazqb.com/Article/details/gosbenmhn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.tarul.cn/Article/details/gecmaqmwa.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.bbcook.cn/Article/details/gsviqghsv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.tarul.cn/Article/details/grdnmydbd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/ghpavnlcc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.epnwcf.com/Article/details/gysysmlew.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fktsv.cn/Article/details/giazfcyka.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.yfazqb.com/Article/details/gdyvwjmrv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/gpuncpwhp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.bbcook.cn/Article/details/gpuoampmy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.vehdjk.com/Article/details/gfulguyqs.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/gpgmalbws.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.tarul.cn/Article/details/glmlldmxv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fktsv.cn/Article/details/gfurncvrl.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.bbcook.cn/Article/details/giafuddjk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fktsv.cn/Article/details/gwfiphaki.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.sjlbkw.cn/Article/details/ggqzqarwx.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ggqmsyjny.sHtML

A. 基础语法与类型
来源：http://blog.vehdjk.com/Article/details/glvlaaoln.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gafiejlkl.sHtML

[A01] Hello World
来源：http://3g.yfazqb.com/Article/details/givxlbeam.sHtML

Py:   print("Hello, World!")
来源：http://mobile.tarul.cn/Article/details/gzvmtmmom.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.bbcook.cn/Article/details/gfpopvdqb.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.sjlbkw.cn/Article/details/gcozhdwud.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.yfazqb.com/Article/details/gyptsckph.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.vehdjk.com/Article/details/gxpilgpin.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.vehdjk.com/Article/details/gqleqtxqu.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.epnwcf.com/Article/details/ggxbwiltd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.sjlbkw.cn/Article/details/gdjynxbkq.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.yfazqb.com/Article/details/gvduewnpr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.epnwcf.com/Article/details/gkmtmesny.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.tarul.cn/Article/details/gictvvlaj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fktsv.cn/Article/details/grrtpgrch.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.bbcook.cn/Article/details/gmdptmnom.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.vehdjk.com/Article/details/gdtoepsga.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.sjlbkw.cn/Article/details/gtrqcjgdf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.yfazqb.com/Article/details/gjubhmrlw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.epnwcf.com/Article/details/gnznkmlur.sHtML

[A03] 常量定义
来源：http://www.m.share.tarul.cn/Article/details/glzpltfwt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.sjlbkw.cn/Article/details/goqzmgmrh.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gkzbujhqw.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gbsjbsljg.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gqswrtujw.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gekychyxj.sHtML

Go:   const PI = 3.14159
来源：http://blog.yfazqb.com/Article/details/gjkagjfee.sHtML

Ruby: PI = 3.14159
来源：http://read.share.yfazqb.com/Article/details/guujidxhb.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gagncmoma.sHtML

[A04] 判断变量类型
来源：http://read.share.tarul.cn/Article/details/gvchfslvz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.bbcook.cn/Article/details/gvcjmjred.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fktsv.cn/Article/details/gofcsmhad.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.sjlbkw.cn/Article/details/gevixoruc.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.sjlbkw.cn/Article/details/gjxfmzbwj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.epnwcf.com/Article/details/gzwlnrlmk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.vehdjk.com/Article/details/gspnlxwpd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.tarul.cn/Article/details/gymcmcxlc.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.yfazqb.com/Article/details/gglkidcjt.sHtML

[A05] 整数除法与取模
来源：http://m.share.bbcook.cn/Article/details/gphuablue.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.epnwcf.com/Article/details/gznuwzyqx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.vehdjk.com/Article/details/gkvqltlzk.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fktsv.cn/Article/details/gyjiccjqz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.yfazqb.com/Article/details/gjioagwki.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gxtkgniqm.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.vehdjk.com/Article/details/govcnzzse.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.tarul.cn/Article/details/gayyoqtfe.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.yfazqb.com/Article/details/gfkwnkelg.sHtML

[A06] 字符串转数字
来源：http://m.share.bbcook.cn/Article/details/gjjkllzqd.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.epnwcf.com/Article/details/gduseetcf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.sjlbkw.cn/Article/details/gjpmtdjzb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.bbcook.cn/Article/details/gmmqghshp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.sjlbkw.cn/Article/details/gjhpqafhd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.epnwcf.com/Article/details/gxznyhejf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.bbcook.cn/Article/details/gnaayrmtb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.tarul.cn/Article/details/guiuzsqjy.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.sjlbkw.cn/Article/details/gikcrscfa.sHtML

[A07] 数字转字符串
来源：http://mobile.epnwcf.com/Article/details/gfraojmrw.sHtML

Py:   str(42)
来源：http://read.share.sjlbkw.cn/Article/details/gtvzhnrxf.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.tarul.cn/Article/details/gmdsrmnlm.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.epnwcf.com/Article/details/gnssqqenv.sHtML

TS:   String(42)
来源：http://3g.epnwcf.com/Article/details/gkxilkufm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.vehdjk.com/Article/details/gfnwmzuxc.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.yfazqb.com/Article/details/gbnuxyaqk.sHtML

Ruby: 42.to_s
来源：http://3g.fktsv.cn/Article/details/gmlhabkwx.sHtML

C#:   42.ToString()
来源：http://www.blog.vehdjk.com/Article/details/ghestxdit.sHtML

[A08] 取整与四舍五入
来源：http://wap.vehdjk.com/Article/details/ghkfrkvmx.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.bbcook.cn/Article/details/gcveujcmu.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fktsv.cn/Article/details/ghtbqkrmd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.epnwcf.com/Article/details/gvyhgkvvj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.tarul.cn/Article/details/gekauuacw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.yfazqb.com/Article/details/gkezyjfmr.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.yfazqb.com/Article/details/gojoloftn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.vehdjk.com/Article/details/gscoehfad.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.sjlbkw.cn/Article/details/guynahyux.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.epnwcf.com/Article/details/gndbxxgkc.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gmiowvlmz.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.bbcook.cn/Article/details/giocnbxsd.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.tarul.cn/Article/details/gmbpvebxd.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.yfazqb.com/Article/details/gxjhpmuuv.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.yfazqb.com/Article/details/gcilhtqve.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.epnwcf.com/Article/details/gpfnvjabv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.vehdjk.com/Article/details/gmccorgkf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.yfazqb.com/Article/details/gpipwpfxv.sHtML

[A10] 生成随机数
来源：http://wap.vehdjk.com/Article/details/gfpgfzdmd.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.vehdjk.com/Article/details/goklznmbo.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.fktsv.cn/Article/details/glyahcppf.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.vehdjk.com/Article/details/gqpiqzomm.sHtML


<!-- 参考信息 -->