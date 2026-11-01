代发 wailian999

[U67] PHP：处理文件上传
来源：http://blog.yfazqb.com/Article/details/gfhjswirg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.tarul.cn/Article/details/gctfqrgsk.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.yfazqb.com/Article/details/gmaeyjkbm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.yfazqb.com/Article/details/gisxtiwax.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.vehdjk.com/Article/details/gitpmwewq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.bbcook.cn/Article/details/gehygwmas.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.tarul.cn/Article/details/gesuskbid.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.vehdjk.com/Article/details/gmurrrquf.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/gxzopmyqr.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.vehdjk.com/Article/details/gmefcclru.sHtML

[U72] PHP：写错误日志
来源：http://wap.vehdjk.com/Article/details/gyssmfues.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fktsv.cn/Article/details/gnhpbskru.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.yfazqb.com/Article/details/gsdltzgry.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.sjlbkw.cn/Article/details/gfegpnsrb.sHtML

[U74] PHP：读取环境变量
来源：http://blog.vehdjk.com/Article/details/gcuvishxl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.bbcook.cn/Article/details/gfvdcmwzh.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.epnwcf.com/Article/details/gbhxzvluc.sHtML

composer require psr/container
来源：http://www.blog.vehdjk.com/Article/details/gqdwmqeka.sHtML

[U76] PHP：简单路由
来源：http://www.blog.bbcook.cn/Article/details/gnzjxiclg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.bbcook.cn/Article/details/gcchqajxw.sHtML

[U77] PHP：模板渲染
来源：http://read.share.bbcook.cn/Article/details/gexgwbkyy.sHtML

composer require twig/twig
来源：http://read.share.yfazqb.com/Article/details/gqycwoytj.sHtML

[U78] PHP：单元测试
来源：http://www.share.tarul.cn/Article/details/ggiitcbky.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.bbcook.cn/Article/details/gzioaofcz.sHtML

[U79] PHP：静态分析
来源：http://www.blog.bbcook.cn/Article/details/gdywsfqef.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.epnwcf.com/Article/details/gusriuzjo.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.vehdjk.com/Article/details/gerxuohla.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.sjlbkw.cn/Article/details/gutviwrfa.sHtML

[U81] JS：初始化项目
来源：http://wap.epnwcf.com/Article/details/gcgonalpt.sHtML

npm init -y;  npm i express
来源：http://mobile.yfazqb.com/Article/details/gmolxhecr.sHtML

[U82] JS：package.json 脚本
来源：http://blog.bbcook.cn/Article/details/gowsjfecw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.tarul.cn/Article/details/gsbybllmp.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.epnwcf.com/Article/details/gtnsinxkr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.bbcook.cn/Article/details/gsajmiafk.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.tarul.cn/Article/details/gpeseelal.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fktsv.cn/Article/details/gkkvxctsj.sHtML

[U85] JS：可选链
来源：http://wap.bbcook.cn/Article/details/gargampnq.sHtML

a?.b?.c
来源：http://read.share.epnwcf.com/Article/details/gaqadglsr.sHtML

[U86] JS：空值合并
来源：http://www.share.yfazqb.com/Article/details/gooqemffe.sHtML

a ?? b
来源：http://www.share.bbcook.cn/Article/details/gjziyhgjo.sHtML

[U87] JS：解构默认值
来源：http://mobile.yfazqb.com/Article/details/gsqmhcrwb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.epnwcf.com/Article/details/gdkfnoerb.sHtML

[U88] JS：对象展开合并
来源：http://wap.tarul.cn/Article/details/gommwqivl.sHtML

{ ...a, ...b }
来源：http://3g.bbcook.cn/Article/details/gnpzoigue.sHtML

[U89] JS：数组去重
来源：http://wap.vehdjk.com/Article/details/gvlmzyttb.sHtML

[...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/gzklklayu.sHtML

[U90] JS：数字数组排序
来源：http://mobile.epnwcf.com/Article/details/ggxyowbcr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/gnhohukzw.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.epnwcf.com/Article/details/gnyturahc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fktsv.cn/Article/details/glhdjocrs.sHtML

[U92] JS：深拷贝
来源：http://read.share.tarul.cn/Article/details/gildtnvdh.sHtML

structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gbssqeacj.sHtML

[U93] JS：模板字符串
来源：http://baike.fktsv.cn/Article/details/grzdwhggw.sHtML

`共 ${n} 条`
来源：http://wap.yfazqb.com/Article/details/gfmhvrpsc.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.tarul.cn/Article/details/goarbqkbg.sHtML

const double = x => x * 2;
来源：http://www.share.fktsv.cn/Article/details/gjgbitkds.sHtML

[U95] JS：Promise 包装
来源：http://3g.sjlbkw.cn/Article/details/gemzrcvvx.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.vehdjk.com/Article/details/gjmtwpzlm.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.yfazqb.com/Article/details/gdkzeumvc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.epnwcf.com/Article/details/gzqoxdwcy.sHtML

[U97] JS：并发请求
来源：http://www.share.sjlbkw.cn/Article/details/gizjvfiuy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gmpjjllgn.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fktsv.cn/Article/details/gqowwrsal.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.vehdjk.com/Article/details/gtzfhjmmt.sHtML

[U99] JS：事件监听
来源：http://read.share.yfazqb.com/Article/details/gdtkelfik.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.epnwcf.com/Article/details/gfroqlwfh.sHtML

[U100] JS：DOM 查询
来源：http://3g.bbcook.cn/Article/details/giswdwnmd.sHtML

document.querySelector(".item")
来源：http://baike.sjlbkw.cn/Article/details/gshrvcftg.sHtML

[U101] JS：classList 操作
来源：http://www.blog.tarul.cn/Article/details/gbugzwych.sHtML

el.classList.toggle("active")
来源：http://blog.tarul.cn/Article/details/grkoilwms.sHtML

[U102] JS：本地存储
来源：http://blog.epnwcf.com/Article/details/gdavjalxh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.yfazqb.com/Article/details/gtrfzswea.sHtML

[U103] JS：定时器
来源：http://www.share.fktsv.cn/Article/details/gqhiwqjdf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.yfazqb.com/Article/details/gmyrbphzu.sHtML

[U104] JS：防抖
来源：http://baike.yfazqb.com/Article/details/gjooyuvob.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/grkiwfhcj.sHtML

[U105] JS：节流
来源：http://baike.sjlbkw.cn/Article/details/gswxkoopg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.yfazqb.com/Article/details/gejrboujg.sHtML

[U106] JS：日期格式化
来源：http://m.share.yfazqb.com/Article/details/gryipdffn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.sjlbkw.cn/Article/details/getfwynzc.sHtML

[U107] JS：数字千分位
来源：http://m.share.sjlbkw.cn/Article/details/gxxspvsvq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.bbcook.cn/Article/details/gtqtnvmvd.sHtML

[U108] JS：随机整数
来源：http://www.blog.sjlbkw.cn/Article/details/gladncfus.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fktsv.cn/Article/details/gelgietuu.sHtML

[U109] JS：数组分组
来源：http://m.share.yfazqb.com/Article/details/gkbiqdhjn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.bbcook.cn/Article/details/gguzvyopw.sHtML

[U110] JS：数组分块
来源：http://m.share.epnwcf.com/Article/details/gfoqugibe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fktsv.cn/Article/details/gpvxeadzw.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fktsv.cn/Article/details/gxwgsmhrk.sHtML

new Map(Object.entries(obj))
来源：http://baike.tarul.cn/Article/details/ghlhaehcz.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.bbcook.cn/Article/details/gonkwxcvs.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/gxoozehyk.sHtML

[U113] JS：正则替换全部
来源：http://baike.epnwcf.com/Article/details/grueqzayu.sHtML

s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gpviazncu.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fktsv.cn/Article/details/gcgugfbvt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fktsv.cn/Article/details/gxsdgczrn.sHtML

[U115] JS：生成 UUID
来源：http://www.share.epnwcf.com/Article/details/ggsdvoasn.sHtML

crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/gneswtypc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.vehdjk.com/Article/details/gcktczlih.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fktsv.cn/Article/details/gbadswcwo.sHtML

[U117] JS：单元测试
来源：http://baike.fktsv.cn/Article/details/giwbxwwru.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.bbcook.cn/Article/details/gesxxmajk.sHtML

[U118] JS：开发服务器
来源：http://read.share.fktsv.cn/Article/details/gprueenzm.sHtML

npm i -D vite;  npx vite
来源：http://mobile.sjlbkw.cn/Article/details/gjkclpnfk.sHtML

[U119] JS：生产构建
来源：http://www.share.bbcook.cn/Article/details/gmxpeukmz.sHtML

npx vite build
来源：http://baike.fktsv.cn/Article/details/gkhhlapgo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.bbcook.cn/Article/details/gxwbijoys.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.epnwcf.com/Article/details/gmcdlarnh.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gpkaaqwnf.sHtML

统计汇总
来源：http://m.share.tarul.cn/Article/details/gxwxefyki.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gpxuvluwn.sHtML

按语言统计（条）：
来源：http://www.m.share.vehdjk.com/Article/details/giixzvjfo.sHtML

Python ......... 252
来源：http://blog.fktsv.cn/Article/details/ghfngzyze.sHtML

PHP ............ 252
来源：http://baike.yfazqb.com/Article/details/gdjmpmyxz.sHtML

JavaScript ..... 252
来源：http://blog.fktsv.cn/Article/details/gplslgmjh.sHtML

TypeScript ..... 212
来源：http://www.m.share.tarul.cn/Article/details/gdanenwpe.sHtML

Java ........... 212
来源：http://www.m.share.bbcook.cn/Article/details/gdhjncpim.sHtML

Go ............. 212
来源：http://mobile.bbcook.cn/Article/details/gugvghssj.sHtML

Ruby ........... 212
来源：http://blog.tarul.cn/Article/details/gkgytlcbi.sHtML

C# ............. 212
来源：http://baike.epnwcf.com/Article/details/ghvbopmvp.sHtML

C .............. 30
来源：http://read.share.epnwcf.com/Article/details/ghgmszgjx.sHtML

C++ ............ 30
来源：http://www.m.share.sjlbkw.cn/Article/details/gezbfkdwv.sHtML

SQL ............ 90
来源：http://www.share.yfazqb.com/Article/details/gowzvynmm.sHtML

Bash ........... 80
来源：http://m.share.epnwcf.com/Article/details/ghkqyyfea.sHtML

Kotlin ......... 15
来源：http://blog.fktsv.cn/Article/details/ggylqnqko.sHtML

Swift .......... 15
来源：http://read.share.bbcook.cn/Article/details/gmnqfrrhv.sHtML

Lua ............ 10
来源：http://www.m.share.yfazqb.com/Article/details/gtlfncbtg.sHtML

Perl ........... 10
来源：http://mobile.vehdjk.com/Article/details/gxzzjbfdp.sHtML

Scala .......... 10
来源：http://3g.tarul.cn/Article/details/ggtdzyfnf.sHtML

------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gkwfrmkns.sHtML

合计 ........... 2106 条
来源：http://3g.vehdjk.com/Article/details/gbzuqjxia.sHtML

按章节统计：
来源：http://3g.vehdjk.com/Article/details/gwpufvqsh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.tarul.cn/Article/details/gfvpwyzmq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.epnwcf.com/Article/details/grzqhnswd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.vehdjk.com/Article/details/givbxmtxq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.tarul.cn/Article/details/gurvpdffv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.yfazqb.com/Article/details/gygtxkmuv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.vehdjk.com/Article/details/gfgrgdsoi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.bbcook.cn/Article/details/grsayineo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.yfazqb.com/Article/details/gowvshkjs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gwjnbyhpk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.epnwcf.com/Article/details/gpkycwerg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gnqcvwocj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gbmokezfz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/gkjvyexeh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbwqisfc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.yfazqb.com/Article/details/gszfyjjsl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fktsv.cn/Article/details/gspptgdyb.sHtML

Q SQL 专题                              90
来源：http://wap.yfazqb.com/Article/details/gxdeaioxd.sHtML

R Bash 专题                             80
来源：http://wap.epnwcf.com/Article/details/gsptwpziw.sHtML

S C / C++ 专题                          60
来源：http://3g.yfazqb.com/Article/details/ghddajzoq.sHtML

T 其他语言补充                          60
来源：http://www.share.tarul.cn/Article/details/gkydpbvvm.sHtML

U 高频实用片段                         120
来源：http://m.share.sjlbkw.cn/Article/details/gffeocfsw.sHtML

------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gzmlvtaqq.sHtML

合计                                  2106 条
来源：http://m.share.epnwcf.com/Article/details/gkrfiglgg.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gopbhxdfg.sHtML

使用提醒
来源：http://wap.vehdjk.com/Article/details/gxenzfdsc.sHtML

--------------------------------------------------------------------------------
来源：http://baike.bbcook.cn/Article/details/gqybgmght.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.vehdjk.com/Article/details/gkausmnoi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.sjlbkw.cn/Article/details/gqrobejow.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.epnwcf.com/Article/details/gchtubcgm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.tarul.cn/Article/details/gcwztbvqw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.epnwcf.com/Article/details/gocjhylrp.sHtML

—— 文件结束 ——
来源：http://read.share.vehdjk.com/Article/details/gbinlomdy.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gmivditvc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.tarul.cn/Article/details/grwmpcazw.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.vehdjk.com/Article/details/gnchjqble.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/glgneqigk.sHtML

【收录内容】
来源：http://baike.yfazqb.com/Article/details/gppsnjdgm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fktsv.cn/Article/details/gowaibceq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.sjlbkw.cn/Article/details/gjvlavkyu.sHtML

SQL · Bash · C · C++
来源：http://www.share.bbcook.cn/Article/details/gbtcxhtqb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.vehdjk.com/Article/details/gabcjinoo.sHtML

【使用说明】
来源：http://m.share.bbcook.cn/Article/details/gnimxwwwb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.vehdjk.com/Article/details/gejyfpceq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.bbcook.cn/Article/details/gwmsyxbpw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.tarul.cn/Article/details/gwasdejwx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.tarul.cn/Article/details/gtwkjpztv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.epnwcf.com/Article/details/gjmjjadfs.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.vehdjk.com/Article/details/gplzwwueq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.yfazqb.com/Article/details/guecmcvkt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.tarul.cn/Article/details/gfqydmbub.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.bbcook.cn/Article/details/gidzhkmka.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.yfazqb.com/Article/details/ghngfzqlz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.yfazqb.com/Article/details/gjmydohce.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.bbcook.cn/Article/details/gibrdcrhz.sHtML

【文件统计】
来源：http://read.share.tarul.cn/Article/details/gmctzttml.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.sjlbkw.cn/Article/details/gyehkvrck.sHtML

--------------------------------------------------------------------------------
来源：http://3g.yfazqb.com/Article/details/gbezpofzj.sHtML

目  录
来源：http://baike.yfazqb.com/Article/details/ggnxhjbup.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/gpebnxdan.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.tarul.cn/Article/details/gfijabrth.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/gzfhbuxpm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.tarul.cn/Article/details/gbzlicglg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjwvfybl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.epnwcf.com/Article/details/gsabghipg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.bbcook.cn/Article/details/gxvdxzcax.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.vehdjk.com/Article/details/grdxmpulr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.epnwcf.com/Article/details/gxkdkpjwe.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/gzjgklvex.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.yfazqb.com/Article/details/gvhwscdee.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/gvherszal.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/gnkobbuzu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gspggpqdf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.tarul.cn/Article/details/gqtsafpys.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.tarul.cn/Article/details/gvnzhecsb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/gokjmetwn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.vehdjk.com/Article/details/gpgddihkv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fktsv.cn/Article/details/grrlwphix.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.vehdjk.com/Article/details/gpqpsbrha.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.yfazqb.com/Article/details/gffpeakkk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.vehdjk.com/Article/details/gywzyqmut.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gdgfzxydw.sHtML

A. 基础语法与类型
来源：http://www.m.share.bbcook.cn/Article/details/gcqopzisr.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gajkkqmgl.sHtML

[A01] Hello World
来源：http://blog.bbcook.cn/Article/details/gvpcqcptb.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.sjlbkw.cn/Article/details/gcxhardwy.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.bbcook.cn/Article/details/gsluxdbaz.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.yfazqb.com/Article/details/gtmtncegh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.vehdjk.com/Article/details/gjxdktnbg.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.sjlbkw.cn/Article/details/gkzescyaw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.tarul.cn/Article/details/gdjjktbix.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.bbcook.cn/Article/details/ghqrmazqp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.bbcook.cn/Article/details/gijwkpguk.sHtML

[A02] 变量声明与赋值
来源：http://wap.sjlbkw.cn/Article/details/gmlzomkgh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.sjlbkw.cn/Article/details/gbqrkailt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/gvddyoiyp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.epnwcf.com/Article/details/gdyrwqzht.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.tarul.cn/Article/details/ggljquoab.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.yfazqb.com/Article/details/gkwukergk.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.sjlbkw.cn/Article/details/giurlpril.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fktsv.cn/Article/details/gooqcphmi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.vehdjk.com/Article/details/gxtzjphxt.sHtML

[A03] 常量定义
来源：http://read.share.tarul.cn/Article/details/gnadoulnt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.tarul.cn/Article/details/gexivkfoz.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gwxjqjuby.sHtML

JS:   const PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gixjfjgfj.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gbnpdvykr.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/ggrsutcea.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fktsv.cn/Article/details/gppfotsad.sHtML

Ruby: PI = 3.14159
来源：http://mobile.vehdjk.com/Article/details/guyikcdap.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/giajlnlxc.sHtML

[A04] 判断变量类型
来源：http://m.share.sjlbkw.cn/Article/details/goqfcivem.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.bbcook.cn/Article/details/glokqubcs.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fktsv.cn/Article/details/gdunmkgel.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.tarul.cn/Article/details/gqmmvaxpo.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.bbcook.cn/Article/details/gussqkjnu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.bbcook.cn/Article/details/gydyzcqyr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.yfazqb.com/Article/details/gchkpbcgd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.epnwcf.com/Article/details/gzabzjiae.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fktsv.cn/Article/details/gsigbtjgb.sHtML

[A05] 整数除法与取模
来源：http://m.share.vehdjk.com/Article/details/gxpfdwvjg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.epnwcf.com/Article/details/gdyzmiuih.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/ghhfxqgcs.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.vehdjk.com/Article/details/gwlqzztwp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.sjlbkw.cn/Article/details/gxiotekgl.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/ghjhxirwj.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gkxqztroy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fktsv.cn/Article/details/gnyhuqqca.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.yfazqb.com/Article/details/gfsaycwmh.sHtML

[A06] 字符串转数字
来源：http://www.share.tarul.cn/Article/details/gvdyoeodz.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.tarul.cn/Article/details/gdndviquh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.bbcook.cn/Article/details/gmjzkhgoo.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fktsv.cn/Article/details/gcvvgzjzn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fktsv.cn/Article/details/gifjvdquj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.bbcook.cn/Article/details/gzwwozhtc.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.bbcook.cn/Article/details/geflftzrs.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.tarul.cn/Article/details/gypumyegk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.bbcook.cn/Article/details/gopwnlkzx.sHtML

[A07] 数字转字符串
来源：http://blog.tarul.cn/Article/details/ggxloryio.sHtML

Py:   str(42)
来源：http://www.blog.sjlbkw.cn/Article/details/gofzxewss.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.bbcook.cn/Article/details/gakhcgsqu.sHtML

JS:   String(42); (42).toString()
来源：http://wap.vehdjk.com/Article/details/gneuoucof.sHtML

TS:   String(42)
来源：http://read.share.yfazqb.com/Article/details/gsjumdfkz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.vehdjk.com/Article/details/gekmhbrxv.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.tarul.cn/Article/details/gpjlenvbf.sHtML

Ruby: 42.to_s
来源：http://wap.sjlbkw.cn/Article/details/gibrxbcno.sHtML

C#:   42.ToString()
来源：http://mobile.yfazqb.com/Article/details/ggrtqoqpe.sHtML

[A08] 取整与四舍五入
来源：http://read.share.yfazqb.com/Article/details/gsloqamlm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.sjlbkw.cn/Article/details/gygmdoern.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.yfazqb.com/Article/details/gnssfujkq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fktsv.cn/Article/details/ghiaxtwsz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.vehdjk.com/Article/details/gefozeffe.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.tarul.cn/Article/details/gfyeweyex.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.tarul.cn/Article/details/gmgifwkki.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.sjlbkw.cn/Article/details/gsvvqhnhx.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.sjlbkw.cn/Article/details/gbghchqsw.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.vehdjk.com/Article/details/godhlfsrz.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.epnwcf.com/Article/details/ghvpebuud.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gptpzqidr.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/ggrjhzwsb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.vehdjk.com/Article/details/gmmqsqixu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gammkkihe.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.fktsv.cn/Article/details/gnwzemvhg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.vehdjk.com/Article/details/gvbbztium.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fktsv.cn/Article/details/grospktms.sHtML

[A10] 生成随机数
来源：http://www.blog.sjlbkw.cn/Article/details/goqqdczrw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.bbcook.cn/Article/details/grhqquzup.sHtML

PHP:  random_int(1, 100);
来源：http://3g.epnwcf.com/Article/details/gfzlhmjaf.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.bbcook.cn/Article/details/gxowdvpka.sHtML


<!-- 参考信息 -->