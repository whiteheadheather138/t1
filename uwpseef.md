代发 wailian999

[U63] PHP：文件读写
来源：http://www.m.share.epnwcf.com/Article/details/gqtayohtz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.vehdjk.com/Article/details/gashergoe.sHtML

[U64] PHP：目录遍历
来源：http://www.share.bbcook.cn/Article/details/ghcjklvuo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.yfazqb.com/Article/details/gsdbncjqr.sHtML

[U65] PHP：会话
来源：http://3g.yfazqb.com/Article/details/gcidmkrgk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gmsuxsvev.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.sjlbkw.cn/Article/details/gjokxegex.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.epnwcf.com/Article/details/ghdhqbffp.sHtML

[U67] PHP：处理文件上传
来源：http://baike.bbcook.cn/Article/details/gfjkorcmk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.epnwcf.com/Article/details/gkmpqprzf.sHtML

[U68] PHP：PDO 连接
来源：http://wap.vehdjk.com/Article/details/gfgpzztob.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.sjlbkw.cn/Article/details/gbwomtexx.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.epnwcf.com/Article/details/gpzwyfdpn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.tarul.cn/Article/details/gzwrwmups.sHtML

[U70] PHP：PDO 事务
来源：http://3g.tarul.cn/Article/details/glhftesqc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.vehdjk.com/Article/details/gqxchupcl.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.yfazqb.com/Article/details/gpueuhhhb.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.vehdjk.com/Article/details/gwqokanww.sHtML

[U72] PHP：写错误日志
来源：http://read.share.vehdjk.com/Article/details/gexjgtxfg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.tarul.cn/Article/details/gqigexmjx.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.sjlbkw.cn/Article/details/gauspgfaw.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.bbcook.cn/Article/details/gehdxyrzy.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.epnwcf.com/Article/details/gxeocdvhw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.sjlbkw.cn/Article/details/gizlykxmw.sHtML

[U75] PHP：依赖注入
来源：http://3g.sjlbkw.cn/Article/details/geskberkp.sHtML

composer require psr/container
来源：http://baike.yfazqb.com/Article/details/gxhojqdkn.sHtML

[U76] PHP：简单路由
来源：http://m.share.bbcook.cn/Article/details/grdapnhdd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.yfazqb.com/Article/details/gdeznvhjx.sHtML

[U77] PHP：模板渲染
来源：http://www.share.vehdjk.com/Article/details/gxplavkxh.sHtML

composer require twig/twig
来源：http://read.share.tarul.cn/Article/details/gsfykpnhb.sHtML

[U78] PHP：单元测试
来源：http://m.share.tarul.cn/Article/details/gnxtolqav.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.sjlbkw.cn/Article/details/gmyghealy.sHtML

[U79] PHP：静态分析
来源：http://mobile.epnwcf.com/Article/details/glaszipra.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.tarul.cn/Article/details/gudkppsui.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.tarul.cn/Article/details/gyzzqhiin.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.vehdjk.com/Article/details/gntwbntep.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fktsv.cn/Article/details/gnrwzsrcu.sHtML

npm init -y;  npm i express
来源：http://mobile.tarul.cn/Article/details/ggnugajpo.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.vehdjk.com/Article/details/gvsckywyi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.tarul.cn/Article/details/gsuigozjo.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fktsv.cn/Article/details/gdxhprpmb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.epnwcf.com/Article/details/gnhzzncqu.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.bbcook.cn/Article/details/gjnmyebgx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fktsv.cn/Article/details/gmvlmmkqk.sHtML

[U85] JS：可选链
来源：http://www.m.share.tarul.cn/Article/details/giwghywgc.sHtML

a?.b?.c
来源：http://m.share.tarul.cn/Article/details/genereaju.sHtML

[U86] JS：空值合并
来源：http://read.share.bbcook.cn/Article/details/gurbmrwwx.sHtML

a ?? b
来源：http://www.m.share.fktsv.cn/Article/details/gphjycmjt.sHtML

[U87] JS：解构默认值
来源：http://blog.epnwcf.com/Article/details/gbwvoqtqw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.bbcook.cn/Article/details/gbpvxeixq.sHtML

[U88] JS：对象展开合并
来源：http://baike.fktsv.cn/Article/details/gnqcwiezv.sHtML

{ ...a, ...b }
来源：http://www.share.yfazqb.com/Article/details/gtxeztlan.sHtML

[U89] JS：数组去重
来源：http://www.share.bbcook.cn/Article/details/grrkeiibk.sHtML

[...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/ggscjlzus.sHtML

[U90] JS：数字数组排序
来源：http://www.share.epnwcf.com/Article/details/gineksrjw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gkykpunrj.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.epnwcf.com/Article/details/gvtdippcv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.tarul.cn/Article/details/grrtbxaic.sHtML

[U92] JS：深拷贝
来源：http://baike.vehdjk.com/Article/details/gaeycvzzd.sHtML

structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/gyzpnrrem.sHtML

[U93] JS：模板字符串
来源：http://read.share.fktsv.cn/Article/details/glyqgidbq.sHtML

`共 ${n} 条`
来源：http://www.m.share.tarul.cn/Article/details/gjtjyejna.sHtML

[U94] JS：箭头函数
来源：http://read.share.bbcook.cn/Article/details/guzvjulkt.sHtML

const double = x => x * 2;
来源：http://read.share.yfazqb.com/Article/details/gsamowmqw.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.yfazqb.com/Article/details/gcflbutri.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.bbcook.cn/Article/details/gfufejqpj.sHtML

[U96] JS：async/await 与异常
来源：http://wap.tarul.cn/Article/details/glcdkkplv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gdwfbeigq.sHtML

[U97] JS：并发请求
来源：http://www.blog.bbcook.cn/Article/details/gozeiuxkh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/gpvwgtaym.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.epnwcf.com/Article/details/gwmrgqgbd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fktsv.cn/Article/details/gcscgdfzn.sHtML

[U99] JS：事件监听
来源：http://read.share.fktsv.cn/Article/details/geibzjxqx.sHtML

el.addEventListener("click", e => {})
来源：http://wap.tarul.cn/Article/details/gupskqczt.sHtML

[U100] JS：DOM 查询
来源：http://baike.epnwcf.com/Article/details/gdteroslm.sHtML

document.querySelector(".item")
来源：http://www.blog.vehdjk.com/Article/details/gsqzmandk.sHtML

[U101] JS：classList 操作
来源：http://read.share.bbcook.cn/Article/details/gqvphtcqk.sHtML

el.classList.toggle("active")
来源：http://baike.yfazqb.com/Article/details/gzvirslzo.sHtML

[U102] JS：本地存储
来源：http://www.m.share.bbcook.cn/Article/details/gfddonith.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.epnwcf.com/Article/details/gpdxgfknt.sHtML

[U103] JS：定时器
来源：http://wap.sjlbkw.cn/Article/details/gfoggpsvx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.sjlbkw.cn/Article/details/gtqtfdmth.sHtML

[U104] JS：防抖
来源：http://baike.yfazqb.com/Article/details/gxqedurwl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gvdlcjpvl.sHtML

[U105] JS：节流
来源：http://www.share.tarul.cn/Article/details/gnduodknx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.epnwcf.com/Article/details/grdfsmwbt.sHtML

[U106] JS：日期格式化
来源：http://wap.epnwcf.com/Article/details/gwdtfkaoi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fktsv.cn/Article/details/gbkblkpkh.sHtML

[U107] JS：数字千分位
来源：http://3g.yfazqb.com/Article/details/gjvcvsdzs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fktsv.cn/Article/details/gniflncqz.sHtML

[U108] JS：随机整数
来源：http://read.share.tarul.cn/Article/details/gtkrgspho.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fktsv.cn/Article/details/guhpbvlzz.sHtML

[U109] JS：数组分组
来源：http://blog.epnwcf.com/Article/details/gbrfiatye.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.vehdjk.com/Article/details/gwunkxuic.sHtML

[U110] JS：数组分块
来源：http://www.m.share.bbcook.cn/Article/details/guciqtwje.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.vehdjk.com/Article/details/gaknenazp.sHtML

[U111] JS：对象转 Map
来源：http://blog.vehdjk.com/Article/details/gaprpqutl.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.sjlbkw.cn/Article/details/gazpgqxed.sHtML

[U112] JS：字符串补位
来源：http://mobile.bbcook.cn/Article/details/gieomsbsa.sHtML

"7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gnfuqoyzg.sHtML

[U113] JS：正则替换全部
来源：http://wap.vehdjk.com/Article/details/gzanhgjiw.sHtML

s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gplenpzev.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fktsv.cn/Article/details/gdrcxjatd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/gaopmoeju.sHtML

[U115] JS：生成 UUID
来源：http://read.share.sjlbkw.cn/Article/details/ggowypnle.sHtML

crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/ggjtvujqt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fktsv.cn/Article/details/gdtewfgqo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.tarul.cn/Article/details/ggsgvmzuw.sHtML

[U117] JS：单元测试
来源：http://www.share.bbcook.cn/Article/details/gghwaqvfs.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fktsv.cn/Article/details/gyfpizghx.sHtML

[U118] JS：开发服务器
来源：http://baike.sjlbkw.cn/Article/details/gtzilszmt.sHtML

npm i -D vite;  npx vite
来源：http://read.share.bbcook.cn/Article/details/gisaowqqj.sHtML

[U119] JS：生产构建
来源：http://blog.bbcook.cn/Article/details/gorvcydmh.sHtML

npx vite build
来源：http://blog.fktsv.cn/Article/details/gdapsgwsp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.epnwcf.com/Article/details/gpewiidoh.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.tarul.cn/Article/details/gbbepwhyi.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gvaifcjhy.sHtML

统计汇总
来源：http://read.share.vehdjk.com/Article/details/gurpjvgqe.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gnlnvsxir.sHtML

按语言统计（条）：
来源：http://www.share.fktsv.cn/Article/details/gtfhegupy.sHtML

Python ......... 252
来源：http://mobile.bbcook.cn/Article/details/gnuxzasyz.sHtML

PHP ............ 252
来源：http://wap.epnwcf.com/Article/details/gwguehrch.sHtML

JavaScript ..... 252
来源：http://www.share.sjlbkw.cn/Article/details/gpzdkxycc.sHtML

TypeScript ..... 212
来源：http://m.share.yfazqb.com/Article/details/gmmiunssf.sHtML

Java ........... 212
来源：http://www.share.vehdjk.com/Article/details/gbsbbfohq.sHtML

Go ............. 212
来源：http://mobile.vehdjk.com/Article/details/ghtwwocay.sHtML

Ruby ........... 212
来源：http://mobile.yfazqb.com/Article/details/gajrqrgyf.sHtML

C# ............. 212
来源：http://blog.fktsv.cn/Article/details/gugmcwcoc.sHtML

C .............. 30
来源：http://blog.tarul.cn/Article/details/gaqtfwmpf.sHtML

C++ ............ 30
来源：http://m.share.epnwcf.com/Article/details/gwlsfjbqt.sHtML

SQL ............ 90
来源：http://www.share.yfazqb.com/Article/details/gvknxcubi.sHtML

Bash ........... 80
来源：http://read.share.vehdjk.com/Article/details/gaqexpndj.sHtML

Kotlin ......... 15
来源：http://m.share.sjlbkw.cn/Article/details/gmwlfdhvv.sHtML

Swift .......... 15
来源：http://3g.tarul.cn/Article/details/gbxyqaout.sHtML

Lua ............ 10
来源：http://www.blog.yfazqb.com/Article/details/gafxonvxc.sHtML

Perl ........... 10
来源：http://m.share.yfazqb.com/Article/details/gtiepqwxg.sHtML

Scala .......... 10
来源：http://www.blog.vehdjk.com/Article/details/gnextlnih.sHtML

------------------------------------
来源：http://baike.fktsv.cn/Article/details/gdzzmhkfn.sHtML

合计 ........... 2106 条
来源：http://baike.bbcook.cn/Article/details/gmplbfxyq.sHtML

按章节统计：
来源：http://read.share.yfazqb.com/Article/details/gpwtqqsbv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwdzdxzt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fktsv.cn/Article/details/ghdryqrrg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/gkaqkgklo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.sjlbkw.cn/Article/details/ggeppljsg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.tarul.cn/Article/details/gkglncacv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.yfazqb.com/Article/details/gnwbuhrhw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fktsv.cn/Article/details/glqjpcabr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.vehdjk.com/Article/details/gvegzbhsy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gurqbwcvr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.bbcook.cn/Article/details/gurqjdxed.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gmbweagrt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gwntcoitz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/gslaqozkn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.epnwcf.com/Article/details/gpbfskkzf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fktsv.cn/Article/details/gwynsoapv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.tarul.cn/Article/details/gpmmttdjb.sHtML

Q SQL 专题                              90
来源：http://read.share.fktsv.cn/Article/details/gicksssho.sHtML

R Bash 专题                             80
来源：http://3g.fktsv.cn/Article/details/gypqnmjos.sHtML

S C / C++ 专题                          60
来源：http://read.share.fktsv.cn/Article/details/gtjtatsqu.sHtML

T 其他语言补充                          60
来源：http://m.share.bbcook.cn/Article/details/gladlclsq.sHtML

U 高频实用片段                         120
来源：http://www.share.bbcook.cn/Article/details/ghwmhougt.sHtML

------------------------------------
来源：http://wap.fktsv.cn/Article/details/gxcerjtfm.sHtML

合计                                  2106 条
来源：http://wap.tarul.cn/Article/details/gjdynpued.sHtML

--------------------------------------------------------------------------------
来源：http://wap.tarul.cn/Article/details/gxxisoffo.sHtML

使用提醒
来源：http://wap.fktsv.cn/Article/details/gjhzbibbd.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gccvqwxkx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.bbcook.cn/Article/details/gwnclmcbo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.vehdjk.com/Article/details/ghocsaokz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.bbcook.cn/Article/details/glbggqjgs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.sjlbkw.cn/Article/details/gbbrxlgxf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.yfazqb.com/Article/details/gwaejixxt.sHtML

—— 文件结束 ——
来源：http://baike.sjlbkw.cn/Article/details/gjjuplbcl.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gyupfurqy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fktsv.cn/Article/details/gcvgucggh.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.tarul.cn/Article/details/ggpxugfye.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gwkaojdbt.sHtML

【收录内容】
来源：http://blog.sjlbkw.cn/Article/details/gqkhnrcfw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.epnwcf.com/Article/details/ghvhsavbg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.yfazqb.com/Article/details/gbvcsqftz.sHtML

SQL · Bash · C · C++
来源：http://mobile.epnwcf.com/Article/details/gguagtkqz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.vehdjk.com/Article/details/gsnxaxxop.sHtML

【使用说明】
来源：http://mobile.tarul.cn/Article/details/gowzyinne.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.epnwcf.com/Article/details/gsyzzsfzl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.tarul.cn/Article/details/glzwckiwd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.sjlbkw.cn/Article/details/ghycoctda.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.tarul.cn/Article/details/ggcmtjxda.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fktsv.cn/Article/details/glhldhydh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.bbcook.cn/Article/details/gurtygzdf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fktsv.cn/Article/details/gdvtolrjn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.epnwcf.com/Article/details/gxrsgexdd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fktsv.cn/Article/details/gjrsbauar.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.sjlbkw.cn/Article/details/gnguqostv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.epnwcf.com/Article/details/gebczcxqy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fktsv.cn/Article/details/glpieiuea.sHtML

【文件统计】
来源：http://3g.epnwcf.com/Article/details/goodchxmo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.sjlbkw.cn/Article/details/gmcipklfy.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gpybtqgaz.sHtML

目  录
来源：http://mobile.sjlbkw.cn/Article/details/gtgmgcqlh.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gdkjomarp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.vehdjk.com/Article/details/gkcpppjlf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.vehdjk.com/Article/details/goouynwhp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.bbcook.cn/Article/details/gvamljboy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fktsv.cn/Article/details/gxhvcsycx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.yfazqb.com/Article/details/giblrkdid.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.vehdjk.com/Article/details/gigihgtyz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.epnwcf.com/Article/details/gwbnxlkjr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.bbcook.cn/Article/details/gdmnpflzg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.vehdjk.com/Article/details/ggnxqubnp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.epnwcf.com/Article/details/gcwbutpco.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.tarul.cn/Article/details/gnfvylhkm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.vehdjk.com/Article/details/gigkvzwlb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.yfazqb.com/Article/details/gmuwqjgix.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.tarul.cn/Article/details/gfefoouhx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fktsv.cn/Article/details/ghkctyymr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbfucibx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.yfazqb.com/Article/details/gutlrecbi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.bbcook.cn/Article/details/gympwmnsd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fktsv.cn/Article/details/gfscwcgar.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.yfazqb.com/Article/details/geotzuidk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fktsv.cn/Article/details/gkbztmckl.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/godkdwlrg.sHtML

A. 基础语法与类型
来源：http://3g.epnwcf.com/Article/details/gumugkxfj.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/guljdylhf.sHtML

[A01] Hello World
来源：http://baike.bbcook.cn/Article/details/gyggtlqde.sHtML

Py:   print("Hello, World!")
来源：http://3g.epnwcf.com/Article/details/gwhptuqtr.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.tarul.cn/Article/details/gzmlhazjd.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fktsv.cn/Article/details/gzfopogyd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.yfazqb.com/Article/details/gxsnxfgia.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.vehdjk.com/Article/details/gffcbmjou.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.yfazqb.com/Article/details/gukikfhlu.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.tarul.cn/Article/details/gzurqzkmi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.yfazqb.com/Article/details/gdcstdruq.sHtML

[A02] 变量声明与赋值
来源：http://3g.epnwcf.com/Article/details/gkalckcgl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fktsv.cn/Article/details/gdewxcekw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.epnwcf.com/Article/details/gycyimnuh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.sjlbkw.cn/Article/details/gmvixaghd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.vehdjk.com/Article/details/gqbmiapze.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.epnwcf.com/Article/details/gevmcalqc.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.vehdjk.com/Article/details/gxgqawddn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.sjlbkw.cn/Article/details/gnitxwqsq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.yfazqb.com/Article/details/gmrkjalkj.sHtML

[A03] 常量定义
来源：http://www.m.share.fktsv.cn/Article/details/gmtjletzx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.tarul.cn/Article/details/gcxrpwvhy.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gxgcrgycn.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gcrgiamjy.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gqwlvpoyl.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gnpnnqcki.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.vehdjk.com/Article/details/gxoisdhfz.sHtML

Ruby: PI = 3.14159
来源：http://mobile.tarul.cn/Article/details/gocqmtqmq.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gkcuegifv.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fktsv.cn/Article/details/gfyugdduo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.vehdjk.com/Article/details/gimpuvomp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fktsv.cn/Article/details/gbdqynbmr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fktsv.cn/Article/details/gwzmyvwhi.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.bbcook.cn/Article/details/geypheujs.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fktsv.cn/Article/details/gqjfyhkwt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.yfazqb.com/Article/details/gdxfgndau.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.sjlbkw.cn/Article/details/gkltmwott.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.vehdjk.com/Article/details/gjqnbwsop.sHtML

[A05] 整数除法与取模
来源：http://blog.yfazqb.com/Article/details/gagognufi.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.sjlbkw.cn/Article/details/gejgfkjza.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.tarul.cn/Article/details/gbdpgwtya.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gbawcbnfn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gbnjluwyj.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/gtxdmnkoa.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gmbcknwsm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.vehdjk.com/Article/details/ggcgfmfwo.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.yfazqb.com/Article/details/gvkslmbeg.sHtML

[A06] 字符串转数字
来源：http://www.share.yfazqb.com/Article/details/gqzzqshvi.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.sjlbkw.cn/Article/details/gmiqdboxm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.tarul.cn/Article/details/gsmzbdvan.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.epnwcf.com/Article/details/gbhtrmwyq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.yfazqb.com/Article/details/gevitdjrp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.vehdjk.com/Article/details/gcbeknrge.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.epnwcf.com/Article/details/gybkemtyt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.sjlbkw.cn/Article/details/gaxllogff.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.epnwcf.com/Article/details/gfyryatso.sHtML

[A07] 数字转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gljgotvbb.sHtML

Py:   str(42)
来源：http://baike.yfazqb.com/Article/details/gbxoqnpdb.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.yfazqb.com/Article/details/gpbiwuhxs.sHtML

JS:   String(42); (42).toString()
来源：http://wap.sjlbkw.cn/Article/details/gtyoehexn.sHtML

TS:   String(42)
来源：http://www.blog.yfazqb.com/Article/details/gjjxqmald.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.sjlbkw.cn/Article/details/ggrncpvva.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.yfazqb.com/Article/details/gkupsrjcl.sHtML

Ruby: 42.to_s
来源：http://wap.fktsv.cn/Article/details/gxsjjxyjj.sHtML

C#:   42.ToString()
来源：http://www.m.share.bbcook.cn/Article/details/gweheawss.sHtML

[A08] 取整与四舍五入
来源：http://read.share.tarul.cn/Article/details/gpedlpgwk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.tarul.cn/Article/details/gtuybfczi.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.yfazqb.com/Article/details/ganwhhuoe.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.bbcook.cn/Article/details/gobhwnlfz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.tarul.cn/Article/details/giiyvevjo.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.yfazqb.com/Article/details/ghcuyddhv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.sjlbkw.cn/Article/details/gfjtgsjhn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fktsv.cn/Article/details/gkhpoxgus.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fktsv.cn/Article/details/gtmweazqm.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.vehdjk.com/Article/details/gdfmdluhv.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.epnwcf.com/Article/details/gfroyhdyo.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.bbcook.cn/Article/details/gqvwsbitn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/grdqqfspl.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gfzvfaonw.sHtML


<!-- 参考信息 -->