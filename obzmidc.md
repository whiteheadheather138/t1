代发 wailian999

[U65] PHP：会话
来源：http://read.share.vehdjk.com/Article/details/ggxwbwsvp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.yfazqb.com/Article/details/gkwkezlpz.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.tarul.cn/Article/details/gezfxvoil.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.bbcook.cn/Article/details/gicvvitkw.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.epnwcf.com/Article/details/gunwmiweq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.sjlbkw.cn/Article/details/gztcuadti.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.epnwcf.com/Article/details/gvziasbjs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.tarul.cn/Article/details/gwoegtnvu.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.vehdjk.com/Article/details/gztnahati.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.yfazqb.com/Article/details/gpcbgywzs.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fktsv.cn/Article/details/gkbbwjxlg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.vehdjk.com/Article/details/gyhzeeygn.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fktsv.cn/Article/details/gawvbjkkw.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.tarul.cn/Article/details/gyxcqophg.sHtML

[U72] PHP：写错误日志
来源：http://wap.epnwcf.com/Article/details/gwpzvzcke.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fktsv.cn/Article/details/guazwuizn.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqbjatdo.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.yfazqb.com/Article/details/goacshjkz.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.epnwcf.com/Article/details/graqusamz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fktsv.cn/Article/details/gejweeufd.sHtML

[U75] PHP：依赖注入
来源：http://m.share.sjlbkw.cn/Article/details/gvxmtgybb.sHtML

composer require psr/container
来源：http://blog.vehdjk.com/Article/details/gkfmxrwej.sHtML

[U76] PHP：简单路由
来源：http://3g.yfazqb.com/Article/details/gsmxpqfza.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.vehdjk.com/Article/details/gyeldrshw.sHtML

[U77] PHP：模板渲染
来源：http://baike.fktsv.cn/Article/details/gddwntzux.sHtML

composer require twig/twig
来源：http://mobile.yfazqb.com/Article/details/glfhfktsp.sHtML

[U78] PHP：单元测试
来源：http://read.share.tarul.cn/Article/details/gofnkrqip.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.tarul.cn/Article/details/gbiwcspjm.sHtML

[U79] PHP：静态分析
来源：http://baike.yfazqb.com/Article/details/gyfjjxnto.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.tarul.cn/Article/details/gfzcvozlc.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.sjlbkw.cn/Article/details/gwkmekfju.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.sjlbkw.cn/Article/details/gxhyqloqn.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fktsv.cn/Article/details/gnwkvzrfm.sHtML

npm init -y;  npm i express
来源：http://baike.yfazqb.com/Article/details/gjefchmtp.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.epnwcf.com/Article/details/gbaepbqsw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.vehdjk.com/Article/details/gqxefxwbf.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.vehdjk.com/Article/details/gyoshlkjz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.bbcook.cn/Article/details/gsgabjygi.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.epnwcf.com/Article/details/gpjxumdwn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.vehdjk.com/Article/details/gmltvmggz.sHtML

[U85] JS：可选链
来源：http://www.m.share.yfazqb.com/Article/details/gcxosljdi.sHtML

a?.b?.c
来源：http://wap.fktsv.cn/Article/details/gtwqpbspy.sHtML

[U86] JS：空值合并
来源：http://blog.epnwcf.com/Article/details/gfvquoosv.sHtML

a ?? b
来源：http://baike.epnwcf.com/Article/details/gwloxnryk.sHtML

[U87] JS：解构默认值
来源：http://m.share.fktsv.cn/Article/details/gilbcyucc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.yfazqb.com/Article/details/gtnuxkduc.sHtML

[U88] JS：对象展开合并
来源：http://baike.tarul.cn/Article/details/gxplwhsal.sHtML

{ ...a, ...b }
来源：http://m.share.tarul.cn/Article/details/gqyxgwats.sHtML

[U89] JS：数组去重
来源：http://www.blog.epnwcf.com/Article/details/gbnlckalh.sHtML

[...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gxsdytpaf.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.vehdjk.com/Article/details/gfmmqlohv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gluskzcua.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.sjlbkw.cn/Article/details/gufjgbhxc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.sjlbkw.cn/Article/details/gkttmhbrw.sHtML

[U92] JS：深拷贝
来源：http://read.share.sjlbkw.cn/Article/details/gfqdskwfa.sHtML

structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/guyttkthi.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrxwyvup.sHtML

`共 ${n} 条`
来源：http://m.share.sjlbkw.cn/Article/details/gefkqcluc.sHtML

[U94] JS：箭头函数
来源：http://blog.sjlbkw.cn/Article/details/gpmszdcuz.sHtML

const double = x => x * 2;
来源：http://blog.yfazqb.com/Article/details/gkvopjxpr.sHtML

[U95] JS：Promise 包装
来源：http://baike.yfazqb.com/Article/details/gstfhsotl.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fktsv.cn/Article/details/gbsbpbwfm.sHtML

[U96] JS：async/await 与异常
来源：http://wap.epnwcf.com/Article/details/giqbripyg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/goxhomviy.sHtML

[U97] JS：并发请求
来源：http://read.share.vehdjk.com/Article/details/gasxiebcu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gblswiflk.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.epnwcf.com/Article/details/gqxyuccka.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.tarul.cn/Article/details/gnpnnyljy.sHtML

[U99] JS：事件监听
来源：http://www.m.share.epnwcf.com/Article/details/gocsmnmrm.sHtML

el.addEventListener("click", e => {})
来源：http://wap.sjlbkw.cn/Article/details/gkxzmdncw.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.yfazqb.com/Article/details/ggbqmwzoi.sHtML

document.querySelector(".item")
来源：http://mobile.fktsv.cn/Article/details/gkclxanqv.sHtML

[U101] JS：classList 操作
来源：http://www.share.vehdjk.com/Article/details/gskskzlao.sHtML

el.classList.toggle("active")
来源：http://read.share.bbcook.cn/Article/details/gxrlgfple.sHtML

[U102] JS：本地存储
来源：http://www.blog.fktsv.cn/Article/details/gfyyjavlq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.yfazqb.com/Article/details/ggxumultk.sHtML

[U103] JS：定时器
来源：http://blog.bbcook.cn/Article/details/ghvuohtsx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.yfazqb.com/Article/details/gihfqdekj.sHtML

[U104] JS：防抖
来源：http://baike.sjlbkw.cn/Article/details/gvmcabuuo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gztfztqdd.sHtML

[U105] JS：节流
来源：http://m.share.epnwcf.com/Article/details/gpkeebrrv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.tarul.cn/Article/details/ggfpxnqqw.sHtML

[U106] JS：日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/ggxaerjre.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.yfazqb.com/Article/details/gxkznbpqk.sHtML

[U107] JS：数字千分位
来源：http://baike.vehdjk.com/Article/details/gcdzmvaor.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.tarul.cn/Article/details/gkedurukr.sHtML

[U108] JS：随机整数
来源：http://mobile.bbcook.cn/Article/details/gvbeyyibu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.yfazqb.com/Article/details/gvznqhzch.sHtML

[U109] JS：数组分组
来源：http://www.m.share.bbcook.cn/Article/details/grixninxq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/gjoqnirvn.sHtML

[U110] JS：数组分块
来源：http://mobile.fktsv.cn/Article/details/gzcxajfrg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.yfazqb.com/Article/details/gnjspclvo.sHtML

[U111] JS：对象转 Map
来源：http://blog.epnwcf.com/Article/details/gjtftjxxt.sHtML

new Map(Object.entries(obj))
来源：http://m.share.tarul.cn/Article/details/ggjhoekan.sHtML

[U112] JS：字符串补位
来源：http://wap.bbcook.cn/Article/details/gbjkdbrzi.sHtML

"7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gccsugbit.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.epnwcf.com/Article/details/gdbfreryg.sHtML

s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/gwtqhrynd.sHtML

[U114] JS：JSON 深比较
来源：http://blog.vehdjk.com/Article/details/gaecuuswc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.yfazqb.com/Article/details/gqsmodhas.sHtML

[U115] JS：生成 UUID
来源：http://www.share.bbcook.cn/Article/details/grmiuxkce.sHtML

crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/gfidvwemi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.vehdjk.com/Article/details/gkgdzpmhi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.tarul.cn/Article/details/gernrnqiz.sHtML

[U117] JS：单元测试
来源：http://m.share.fktsv.cn/Article/details/geckrdlhf.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.bbcook.cn/Article/details/gzfwxcyfm.sHtML

[U118] JS：开发服务器
来源：http://3g.fktsv.cn/Article/details/grggaplzj.sHtML

npm i -D vite;  npx vite
来源：http://baike.epnwcf.com/Article/details/gvmjdcwgv.sHtML

[U119] JS：生产构建
来源：http://www.share.bbcook.cn/Article/details/gucpgadvj.sHtML

npx vite build
来源：http://m.share.fktsv.cn/Article/details/gtzokxyvf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.vehdjk.com/Article/details/goovtsaxy.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fktsv.cn/Article/details/gpjpciatj.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gehzanpbx.sHtML

统计汇总
来源：http://www.blog.fktsv.cn/Article/details/gkzvywprz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gnzcgttxx.sHtML

按语言统计（条）：
来源：http://www.blog.sjlbkw.cn/Article/details/gkedpopvx.sHtML

Python ......... 252
来源：http://mobile.bbcook.cn/Article/details/gogzbckri.sHtML

PHP ............ 252
来源：http://baike.fktsv.cn/Article/details/glmnrxvbj.sHtML

JavaScript ..... 252
来源：http://baike.sjlbkw.cn/Article/details/gdxvfevuy.sHtML

TypeScript ..... 212
来源：http://read.share.sjlbkw.cn/Article/details/gfkowqemg.sHtML

Java ........... 212
来源：http://wap.epnwcf.com/Article/details/gplamwewh.sHtML

Go ............. 212
来源：http://3g.bbcook.cn/Article/details/gemywkeru.sHtML

Ruby ........... 212
来源：http://www.share.fktsv.cn/Article/details/groqtdwzk.sHtML

C# ............. 212
来源：http://www.blog.vehdjk.com/Article/details/gwbmizkes.sHtML

C .............. 30
来源：http://blog.fktsv.cn/Article/details/gvylpetep.sHtML

C++ ............ 30
来源：http://read.share.vehdjk.com/Article/details/greqbgbml.sHtML

SQL ............ 90
来源：http://www.blog.sjlbkw.cn/Article/details/gwlgjpzec.sHtML

Bash ........... 80
来源：http://baike.yfazqb.com/Article/details/gydptbiyq.sHtML

Kotlin ......... 15
来源：http://mobile.bbcook.cn/Article/details/gvdorjgcw.sHtML

Swift .......... 15
来源：http://wap.fktsv.cn/Article/details/gbzwtqyla.sHtML

Lua ............ 10
来源：http://m.share.tarul.cn/Article/details/gwdkfzcdo.sHtML

Perl ........... 10
来源：http://www.blog.bbcook.cn/Article/details/gfzbpmmez.sHtML

Scala .......... 10
来源：http://wap.epnwcf.com/Article/details/gdnxfesye.sHtML

------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gebbmszxn.sHtML

合计 ........... 2106 条
来源：http://mobile.bbcook.cn/Article/details/geshtttvs.sHtML

按章节统计：
来源：http://3g.fktsv.cn/Article/details/gwwvsipoq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.vehdjk.com/Article/details/gwpirzdyg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.tarul.cn/Article/details/gcutuylhr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.vehdjk.com/Article/details/gygujimvc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.vehdjk.com/Article/details/grqefjvmy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fktsv.cn/Article/details/gcnrjrezq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.tarul.cn/Article/details/gqenqdjqf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.vehdjk.com/Article/details/gfzvrupen.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.tarul.cn/Article/details/ggsiajtvn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gkbvoegej.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.epnwcf.com/Article/details/gzsuwaaru.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/goojjxzzn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/gxytligzo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.epnwcf.com/Article/details/gqcnhwfkk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.yfazqb.com/Article/details/gglidhoas.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.epnwcf.com/Article/details/gtrjcpjiw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/girlsenlc.sHtML

Q SQL 专题                              90
来源：http://m.share.epnwcf.com/Article/details/gplfixchr.sHtML

R Bash 专题                             80
来源：http://blog.yfazqb.com/Article/details/gfwadbjtv.sHtML

S C / C++ 专题                          60
来源：http://www.share.bbcook.cn/Article/details/gsefoekyn.sHtML

T 其他语言补充                          60
来源：http://read.share.epnwcf.com/Article/details/ggtowevcs.sHtML

U 高频实用片段                         120
来源：http://3g.vehdjk.com/Article/details/gcgvsrndq.sHtML

------------------------------------
来源：http://www.share.bbcook.cn/Article/details/goramxudx.sHtML

合计                                  2106 条
来源：http://read.share.epnwcf.com/Article/details/gcufuypru.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gggaaaaio.sHtML

使用提醒
来源：http://www.share.yfazqb.com/Article/details/gvpsdkelg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gjeiwqcbs.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.tarul.cn/Article/details/greontrsg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.bbcook.cn/Article/details/gyloeyphy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.sjlbkw.cn/Article/details/gwloiwnjc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.epnwcf.com/Article/details/gdlivcxaf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.tarul.cn/Article/details/gqezifydo.sHtML

—— 文件结束 ——
来源：http://mobile.yfazqb.com/Article/details/gmlgopfqs.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/glragvqye.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.yfazqb.com/Article/details/gfiughhfh.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.vehdjk.com/Article/details/gwojncxnm.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gtxwmjqjk.sHtML

【收录内容】
来源：http://www.share.tarul.cn/Article/details/giukydgmp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.sjlbkw.cn/Article/details/gkotxqmmu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.yfazqb.com/Article/details/gdcpvhguz.sHtML

SQL · Bash · C · C++
来源：http://3g.bbcook.cn/Article/details/gaaaqtanc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fktsv.cn/Article/details/glllkidud.sHtML

【使用说明】
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxvvebss.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.epnwcf.com/Article/details/ghltyjwft.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.vehdjk.com/Article/details/gceohwkwa.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.sjlbkw.cn/Article/details/gszcvhvcx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.vehdjk.com/Article/details/gzzvkofrq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.yfazqb.com/Article/details/gyyznkphf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.vehdjk.com/Article/details/gzybmkmxa.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.vehdjk.com/Article/details/gslchfipn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.tarul.cn/Article/details/gvwdlxxaf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.sjlbkw.cn/Article/details/gcwyjgbir.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.tarul.cn/Article/details/gzanjalto.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.yfazqb.com/Article/details/geyphzmwo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.yfazqb.com/Article/details/gnhprgnko.sHtML

【文件统计】
来源：http://www.m.share.epnwcf.com/Article/details/gqttfmkcz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.vehdjk.com/Article/details/gbmvmbffg.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gmgdgzdka.sHtML

目  录
来源：http://mobile.vehdjk.com/Article/details/gcymfmjdg.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/guzgqvspf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.yfazqb.com/Article/details/gmxgfelwn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.vehdjk.com/Article/details/ggpfnkprv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fktsv.cn/Article/details/gperrtycm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.bbcook.cn/Article/details/gbjsfknpa.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.sjlbkw.cn/Article/details/gedkxrtfd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.epnwcf.com/Article/details/golouulzx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fktsv.cn/Article/details/grrfuccsm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.sjlbkw.cn/Article/details/gidczmtcf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/gjwvwgzhn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.yfazqb.com/Article/details/gmwabdpnn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/gtuijrdtl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gniqgshih.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/gttzvndfq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.epnwcf.com/Article/details/gzyjuutti.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.bbcook.cn/Article/details/ggnfflefg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/guixlkncg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.yfazqb.com/Article/details/gdjmalkwl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.tarul.cn/Article/details/ggechdnbn.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.sjlbkw.cn/Article/details/gzelmwtjz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjwoziuh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.sjlbkw.cn/Article/details/gpaoshnye.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gtqfhnhxu.sHtML

A. 基础语法与类型
来源：http://mobile.tarul.cn/Article/details/gihkcnodf.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gdemghesm.sHtML

[A01] Hello World
来源：http://wap.tarul.cn/Article/details/gtrteqqmg.sHtML

Py:   print("Hello, World!")
来源：http://read.share.vehdjk.com/Article/details/ghmzlytia.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fktsv.cn/Article/details/guthdynaa.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.sjlbkw.cn/Article/details/gjjnodske.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fktsv.cn/Article/details/gdirkbvir.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fktsv.cn/Article/details/ghdrgmuhq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fktsv.cn/Article/details/gqyruvopf.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.bbcook.cn/Article/details/ghinyzzar.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.sjlbkw.cn/Article/details/gtbxskvkl.sHtML

[A02] 变量声明与赋值
来源：http://3g.epnwcf.com/Article/details/gguurvndu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fktsv.cn/Article/details/gemkvdgqj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.vehdjk.com/Article/details/gqjninucv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.epnwcf.com/Article/details/gsxjxqcse.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.yfazqb.com/Article/details/gcrromlyl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.epnwcf.com/Article/details/gogrfypby.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.yfazqb.com/Article/details/gdmaibvcr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.epnwcf.com/Article/details/ghbxlhhln.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.epnwcf.com/Article/details/glebqmwtu.sHtML

[A03] 常量定义
来源：http://read.share.fktsv.cn/Article/details/gneipsbmo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.vehdjk.com/Article/details/grzlaudva.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gxqogioph.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gmudrmbdt.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gsroivyil.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gxqqaawxo.sHtML

Go:   const PI = 3.14159
来源：http://mobile.sjlbkw.cn/Article/details/goovphhdb.sHtML

Ruby: PI = 3.14159
来源：http://baike.bbcook.cn/Article/details/gnfqykwsf.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/guxjozxhp.sHtML

[A04] 判断变量类型
来源：http://www.m.share.tarul.cn/Article/details/gmqhhparm.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.bbcook.cn/Article/details/gocncpjgk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.epnwcf.com/Article/details/gtmgxckng.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fktsv.cn/Article/details/gmfxjwteg.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.epnwcf.com/Article/details/guauvgrys.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fktsv.cn/Article/details/gainbbknt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.bbcook.cn/Article/details/gihrllxnh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.tarul.cn/Article/details/ghrfcufkw.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.vehdjk.com/Article/details/gymdvbghw.sHtML

[A05] 整数除法与取模
来源：http://m.share.fktsv.cn/Article/details/gkclokndh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.tarul.cn/Article/details/glazlhmlv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.epnwcf.com/Article/details/gjgwpoltx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gmkhjefzy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.sjlbkw.cn/Article/details/gjklrujag.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.bbcook.cn/Article/details/glhiqcdqj.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/gdcvdfvpw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.epnwcf.com/Article/details/gzkoepwpn.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.tarul.cn/Article/details/grhapsdnl.sHtML

[A06] 字符串转数字
来源：http://www.blog.yfazqb.com/Article/details/gygyzpvqy.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.epnwcf.com/Article/details/gdmuvcucz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fktsv.cn/Article/details/gzlmrfqkc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.epnwcf.com/Article/details/grshwgwzs.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.bbcook.cn/Article/details/gwvchkocp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.sjlbkw.cn/Article/details/giwdckeeo.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.yfazqb.com/Article/details/gtosgcjxd.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.epnwcf.com/Article/details/gecukaoam.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.bbcook.cn/Article/details/giuzfrfkl.sHtML

[A07] 数字转字符串
来源：http://read.share.yfazqb.com/Article/details/gvgwiwifa.sHtML

Py:   str(42)
来源：http://read.share.sjlbkw.cn/Article/details/gzsflwrzn.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.sjlbkw.cn/Article/details/gksguiksb.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.epnwcf.com/Article/details/gtvfdqfud.sHtML

TS:   String(42)
来源：http://mobile.sjlbkw.cn/Article/details/gdhckihce.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.yfazqb.com/Article/details/gumyilaaf.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.epnwcf.com/Article/details/gagnxhivu.sHtML

Ruby: 42.to_s
来源：http://3g.fktsv.cn/Article/details/gyeugntzq.sHtML

C#:   42.ToString()
来源：http://3g.yfazqb.com/Article/details/gdojduadb.sHtML

[A08] 取整与四舍五入
来源：http://blog.yfazqb.com/Article/details/gtknkytka.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/gyjvynsgx.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.tarul.cn/Article/details/gjvtdglpt.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/gsbzkydhu.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.vehdjk.com/Article/details/ghbdygfjv.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.epnwcf.com/Article/details/ghcdbgqhb.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.tarul.cn/Article/details/goprrnova.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.sjlbkw.cn/Article/details/gboastzdt.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fktsv.cn/Article/details/gjsoynjry.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.sjlbkw.cn/Article/details/gmoartajt.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.vehdjk.com/Article/details/gcgszrzaj.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gypflvfou.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gqawptfyj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.vehdjk.com/Article/details/ggzczifex.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.sjlbkw.cn/Article/details/gkojjfwyr.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.bbcook.cn/Article/details/gkqofuaww.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.vehdjk.com/Article/details/ghxmwozfp.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gzdnjuawo.sHtML


<!-- 参考信息 -->