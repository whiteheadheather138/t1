代发 wailian999

[U61] PHP：正则
来源：http://www.m.share.tarul.cn/Article/details/gbojkakfb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fktsv.cn/Article/details/gdlemyrqi.sHtML

[U62] PHP：日期对象
来源：http://blog.epnwcf.com/Article/details/gnwnbbbzz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.yfazqb.com/Article/details/gviinqfxf.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.yfazqb.com/Article/details/gpezuusmp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.epnwcf.com/Article/details/gclqdbvvh.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fktsv.cn/Article/details/gpvsnukte.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.yfazqb.com/Article/details/glefwxnjr.sHtML

[U65] PHP：会话
来源：http://www.share.vehdjk.com/Article/details/gewsknpqx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gyobvyadm.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fktsv.cn/Article/details/giyxsrmdw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fktsv.cn/Article/details/grmgiafro.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.bbcook.cn/Article/details/gmrebftya.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fktsv.cn/Article/details/gpxbzeonu.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.tarul.cn/Article/details/gpfiulkdd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.sjlbkw.cn/Article/details/gvbvmgpwj.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.sjlbkw.cn/Article/details/gogfdtqdz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.vehdjk.com/Article/details/goowuunwd.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.epnwcf.com/Article/details/guwnkmwtg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.epnwcf.com/Article/details/glovchflx.sHtML

[U71] PHP：抛出异常
来源：http://read.share.vehdjk.com/Article/details/gbmxxkwbi.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.bbcook.cn/Article/details/ggstschca.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.bbcook.cn/Article/details/gofbooqvk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.vehdjk.com/Article/details/gztknuraq.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.vehdjk.com/Article/details/gitjbkykp.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.bbcook.cn/Article/details/gcxwbiaxq.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.vehdjk.com/Article/details/gliyqsihp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.vehdjk.com/Article/details/gddxknnwe.sHtML

[U75] PHP：依赖注入
来源：http://wap.sjlbkw.cn/Article/details/gpoudrzwx.sHtML

composer require psr/container
来源：http://wap.tarul.cn/Article/details/gzaxykajw.sHtML

[U76] PHP：简单路由
来源：http://www.blog.yfazqb.com/Article/details/geumwdxrt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.sjlbkw.cn/Article/details/gwmnalkcz.sHtML

[U77] PHP：模板渲染
来源：http://read.share.vehdjk.com/Article/details/gzmcierdr.sHtML

composer require twig/twig
来源：http://www.share.sjlbkw.cn/Article/details/ggmhtbhas.sHtML

[U78] PHP：单元测试
来源：http://wap.yfazqb.com/Article/details/glagbhvgf.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fktsv.cn/Article/details/gugtpjapo.sHtML

[U79] PHP：静态分析
来源：http://mobile.tarul.cn/Article/details/guipvzndp.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.epnwcf.com/Article/details/gpixkplwa.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.bbcook.cn/Article/details/ghjtthqrg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.bbcook.cn/Article/details/gvrdhfmnv.sHtML

[U81] JS：初始化项目
来源：http://blog.bbcook.cn/Article/details/guhgzwfxv.sHtML

npm init -y;  npm i express
来源：http://www.share.bbcook.cn/Article/details/grnmdiopi.sHtML

[U82] JS：package.json 脚本
来源：http://blog.epnwcf.com/Article/details/gkfxcydup.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.tarul.cn/Article/details/gnuxpphhh.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.vehdjk.com/Article/details/gognazlmy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.epnwcf.com/Article/details/gictwlhkf.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.vehdjk.com/Article/details/gcvfhlsbi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.sjlbkw.cn/Article/details/gymmlaiws.sHtML

[U85] JS：可选链
来源：http://3g.bbcook.cn/Article/details/glxvajbjl.sHtML

a?.b?.c
来源：http://wap.tarul.cn/Article/details/gkybdfqgp.sHtML

[U86] JS：空值合并
来源：http://www.blog.tarul.cn/Article/details/gmffmojhx.sHtML

a ?? b
来源：http://3g.tarul.cn/Article/details/gritsmtcn.sHtML

[U87] JS：解构默认值
来源：http://mobile.sjlbkw.cn/Article/details/gcwytxpfp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.yfazqb.com/Article/details/gdgfqtbyr.sHtML

[U88] JS：对象展开合并
来源：http://read.share.yfazqb.com/Article/details/grzdqnmso.sHtML

{ ...a, ...b }
来源：http://baike.yfazqb.com/Article/details/guweohabm.sHtML

[U89] JS：数组去重
来源：http://wap.bbcook.cn/Article/details/guclzfmmv.sHtML

[...new Set(arr)]
来源：http://m.share.epnwcf.com/Article/details/gkkfpsqhn.sHtML

[U90] JS：数字数组排序
来源：http://baike.vehdjk.com/Article/details/gqautwgiz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/gyvvtrcvb.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.tarul.cn/Article/details/gqosxbmcz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.sjlbkw.cn/Article/details/gwcfaiumk.sHtML

[U92] JS：深拷贝
来源：http://wap.yfazqb.com/Article/details/gfcajxqfz.sHtML

structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/glciuxhrf.sHtML

[U93] JS：模板字符串
来源：http://wap.fktsv.cn/Article/details/gociekxki.sHtML

`共 ${n} 条`
来源：http://m.share.epnwcf.com/Article/details/grmkfqotp.sHtML

[U94] JS：箭头函数
来源：http://m.share.tarul.cn/Article/details/grxtfmoay.sHtML

const double = x => x * 2;
来源：http://blog.epnwcf.com/Article/details/gylmnracr.sHtML

[U95] JS：Promise 包装
来源：http://wap.tarul.cn/Article/details/gryknqrph.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.sjlbkw.cn/Article/details/gtkdzlckf.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.epnwcf.com/Article/details/gpappvgor.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gxrnwiclc.sHtML

[U97] JS：并发请求
来源：http://baike.tarul.cn/Article/details/grgojjvha.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/glfjbcucu.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.tarul.cn/Article/details/gcaihrkbw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.vehdjk.com/Article/details/geqqmlqxt.sHtML

[U99] JS：事件监听
来源：http://m.share.vehdjk.com/Article/details/gpggsxujb.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.epnwcf.com/Article/details/gistcdzvb.sHtML

[U100] JS：DOM 查询
来源：http://blog.vehdjk.com/Article/details/gxwvbdhav.sHtML

document.querySelector(".item")
来源：http://wap.sjlbkw.cn/Article/details/gleeyzukt.sHtML

[U101] JS：classList 操作
来源：http://www.share.epnwcf.com/Article/details/gnhabwtoo.sHtML

el.classList.toggle("active")
来源：http://read.share.fktsv.cn/Article/details/gqheyabjp.sHtML

[U102] JS：本地存储
来源：http://www.share.tarul.cn/Article/details/gsvzmufml.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.bbcook.cn/Article/details/gvgsgysyx.sHtML

[U103] JS：定时器
来源：http://www.blog.bbcook.cn/Article/details/gpritsfkc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.epnwcf.com/Article/details/gsgaduxte.sHtML

[U104] JS：防抖
来源：http://3g.vehdjk.com/Article/details/geeknnkjz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcmdaqgy.sHtML

[U105] JS：节流
来源：http://www.share.sjlbkw.cn/Article/details/gajlbiirr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.sjlbkw.cn/Article/details/gjilbxwfh.sHtML

[U106] JS：日期格式化
来源：http://mobile.epnwcf.com/Article/details/gsueemoaq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.sjlbkw.cn/Article/details/gzqyrblrj.sHtML

[U107] JS：数字千分位
来源：http://www.share.bbcook.cn/Article/details/gswlwlpfc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.epnwcf.com/Article/details/gyywuvisq.sHtML

[U108] JS：随机整数
来源：http://mobile.yfazqb.com/Article/details/ghsvlwvux.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fktsv.cn/Article/details/gjywqyyga.sHtML

[U109] JS：数组分组
来源：http://3g.tarul.cn/Article/details/gacghzlue.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.vehdjk.com/Article/details/gxhkxytll.sHtML

[U110] JS：数组分块
来源：http://wap.yfazqb.com/Article/details/gvvmjmmgm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.tarul.cn/Article/details/gkanmandn.sHtML

[U111] JS：对象转 Map
来源：http://m.share.vehdjk.com/Article/details/gezzxuzyc.sHtML

new Map(Object.entries(obj))
来源：http://read.share.tarul.cn/Article/details/gnhweursk.sHtML

[U112] JS：字符串补位
来源：http://m.share.vehdjk.com/Article/details/gynhigbxm.sHtML

"7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/goodetesu.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.vehdjk.com/Article/details/gjjsbfqmw.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gsyzsqrsh.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.bbcook.cn/Article/details/gruiqlrib.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/gaqsthgui.sHtML

[U115] JS：生成 UUID
来源：http://wap.epnwcf.com/Article/details/gbdrxoifr.sHtML

crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gxdaefdcj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.tarul.cn/Article/details/glnvxbgna.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fktsv.cn/Article/details/gswpmwhed.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fktsv.cn/Article/details/gipcnzxoq.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.sjlbkw.cn/Article/details/grmtqkhfq.sHtML

[U118] JS：开发服务器
来源：http://www.share.fktsv.cn/Article/details/gqmbtrhnd.sHtML

npm i -D vite;  npx vite
来源：http://m.share.tarul.cn/Article/details/ggmrwvfpn.sHtML

[U119] JS：生产构建
来源：http://wap.sjlbkw.cn/Article/details/gthkpqwnr.sHtML

npx vite build
来源：http://read.share.bbcook.cn/Article/details/gernhytdw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.vehdjk.com/Article/details/gxkevuaxc.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.tarul.cn/Article/details/guyxytvme.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gpyzwonsi.sHtML

统计汇总
来源：http://wap.tarul.cn/Article/details/gefidnfrm.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gryfndxwk.sHtML

按语言统计（条）：
来源：http://baike.epnwcf.com/Article/details/gkskwrbpt.sHtML

Python ......... 252
来源：http://www.share.bbcook.cn/Article/details/gniayezfq.sHtML

PHP ............ 252
来源：http://wap.sjlbkw.cn/Article/details/gtcsjokxf.sHtML

JavaScript ..... 252
来源：http://mobile.tarul.cn/Article/details/gubkgqibb.sHtML

TypeScript ..... 212
来源：http://www.share.tarul.cn/Article/details/gjvobojwh.sHtML

Java ........... 212
来源：http://wap.fktsv.cn/Article/details/gnsfniatx.sHtML

Go ............. 212
来源：http://3g.tarul.cn/Article/details/gctuzypqn.sHtML

Ruby ........... 212
来源：http://baike.sjlbkw.cn/Article/details/gifyujmne.sHtML

C# ............. 212
来源：http://mobile.epnwcf.com/Article/details/gnudbqakq.sHtML

C .............. 30
来源：http://m.share.vehdjk.com/Article/details/gtvtmtpsn.sHtML

C++ ............ 30
来源：http://www.share.tarul.cn/Article/details/gggqcffhf.sHtML

SQL ............ 90
来源：http://m.share.tarul.cn/Article/details/gthusyich.sHtML

Bash ........... 80
来源：http://www.m.share.fktsv.cn/Article/details/gdvihzaxp.sHtML

Kotlin ......... 15
来源：http://wap.tarul.cn/Article/details/gwduwmlot.sHtML

Swift .......... 15
来源：http://blog.yfazqb.com/Article/details/gdojkjpns.sHtML

Lua ............ 10
来源：http://www.blog.fktsv.cn/Article/details/gaihtbknl.sHtML

Perl ........... 10
来源：http://read.share.yfazqb.com/Article/details/gwfcepdgj.sHtML

Scala .......... 10
来源：http://www.blog.bbcook.cn/Article/details/gxjajwzsc.sHtML

------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gylemcqbp.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fktsv.cn/Article/details/ggfxlpbmm.sHtML

按章节统计：
来源：http://m.share.sjlbkw.cn/Article/details/gavsyelnb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.bbcook.cn/Article/details/gjjijpxla.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.sjlbkw.cn/Article/details/ghjpkekyt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.sjlbkw.cn/Article/details/ggkqysvlf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.bbcook.cn/Article/details/gaxuihenv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.vehdjk.com/Article/details/goavupcej.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.yfazqb.com/Article/details/gowsonffv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.tarul.cn/Article/details/grvjjqkfe.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.tarul.cn/Article/details/gdcqxkuzg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/golddonfu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.yfazqb.com/Article/details/ggtxcqmtd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/gsfctyzjk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/ggughzfrc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gcqnbefoq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.vehdjk.com/Article/details/gjkgnkncu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.vehdjk.com/Article/details/gevdecodt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/gspihvpuq.sHtML

Q SQL 专题                              90
来源：http://3g.yfazqb.com/Article/details/gyyeuoztz.sHtML

R Bash 专题                             80
来源：http://baike.fktsv.cn/Article/details/ghxfeaxdy.sHtML

S C / C++ 专题                          60
来源：http://blog.yfazqb.com/Article/details/gwfxfmuab.sHtML

T 其他语言补充                          60
来源：http://3g.sjlbkw.cn/Article/details/gxjpftcoi.sHtML

U 高频实用片段                         120
来源：http://m.share.bbcook.cn/Article/details/gdnpxyvvs.sHtML

------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gwqvkfvmi.sHtML

合计                                  2106 条
来源：http://m.share.fktsv.cn/Article/details/gkltqdbkd.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.epnwcf.com/Article/details/gkpnflazx.sHtML

使用提醒
来源：http://mobile.epnwcf.com/Article/details/gudtttsls.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/godyjajue.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.bbcook.cn/Article/details/gwfkbthnm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.vehdjk.com/Article/details/gddexdium.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.vehdjk.com/Article/details/gmiyzhchi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.vehdjk.com/Article/details/gzpknpicm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.epnwcf.com/Article/details/ggyazkvcm.sHtML

—— 文件结束 ——
来源：http://www.blog.vehdjk.com/Article/details/grqbgiuvz.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/glxoavvll.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.tarul.cn/Article/details/gejdjmqhm.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fktsv.cn/Article/details/gyrgxspua.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gycjajiuh.sHtML

【收录内容】
来源：http://www.m.share.sjlbkw.cn/Article/details/gkyhljkkm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.sjlbkw.cn/Article/details/geholvsmk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.epnwcf.com/Article/details/gzasqqhzn.sHtML

SQL · Bash · C · C++
来源：http://3g.epnwcf.com/Article/details/gtjcgozhk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.epnwcf.com/Article/details/getdcbxnl.sHtML

【使用说明】
来源：http://m.share.yfazqb.com/Article/details/gzrbtgpiz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.sjlbkw.cn/Article/details/gxbqseqey.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.bbcook.cn/Article/details/godlwdgpi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.sjlbkw.cn/Article/details/gibqquchq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.epnwcf.com/Article/details/gwzmntylh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fktsv.cn/Article/details/gajlkdhgl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.epnwcf.com/Article/details/gwwhqydpw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.sjlbkw.cn/Article/details/gfaodmchq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.tarul.cn/Article/details/gdogukomx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.sjlbkw.cn/Article/details/gxwqssuau.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.sjlbkw.cn/Article/details/gacnsedte.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.tarul.cn/Article/details/grjxfzrvf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.vehdjk.com/Article/details/gbcmscrbm.sHtML

【文件统计】
来源：http://m.share.yfazqb.com/Article/details/gbjltbcha.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.epnwcf.com/Article/details/grtfdciys.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gxfsmmtkk.sHtML

目  录
来源：http://blog.fktsv.cn/Article/details/guvnuvrqd.sHtML

--------------------------------------------------------------------------------
来源：http://3g.tarul.cn/Article/details/geoszirge.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.tarul.cn/Article/details/glwmyskvk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.epnwcf.com/Article/details/gnoiixexo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.vehdjk.com/Article/details/gpiqfvweu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fktsv.cn/Article/details/gahugllnv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.tarul.cn/Article/details/gmllqqwzy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.epnwcf.com/Article/details/gwtvvrotb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.yfazqb.com/Article/details/ggsbpriqm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.bbcook.cn/Article/details/gpabffyad.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fktsv.cn/Article/details/gfdeuujrp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.tarul.cn/Article/details/gfxuoljxs.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/gawloyuqn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gphmrvilp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/giqekhdja.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.yfazqb.com/Article/details/gyueiqvxf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fktsv.cn/Article/details/glojpaqgh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/gqaaflnjl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.yfazqb.com/Article/details/gsolqbgyn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fktsv.cn/Article/details/gbslymlnq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.epnwcf.com/Article/details/gjvjjnbyu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.tarul.cn/Article/details/gjfvcesmg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.epnwcf.com/Article/details/ghrsvrvhx.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gnvkbngxj.sHtML

A. 基础语法与类型
来源：http://wap.vehdjk.com/Article/details/giprmqxhv.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/geotcdkaf.sHtML

[A01] Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gmgvzcrko.sHtML

Py:   print("Hello, World!")
来源：http://blog.fktsv.cn/Article/details/gflphtcze.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.yfazqb.com/Article/details/glijavgkc.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.bbcook.cn/Article/details/gdiefmriv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.sjlbkw.cn/Article/details/gujuvlxqm.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.bbcook.cn/Article/details/gzusljqea.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.sjlbkw.cn/Article/details/gvhnderty.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.epnwcf.com/Article/details/gaxlazxjl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.bbcook.cn/Article/details/gzzhqjftx.sHtML

[A02] 变量声明与赋值
来源：http://mobile.tarul.cn/Article/details/grreqamot.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.yfazqb.com/Article/details/ggjzjjqfm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fktsv.cn/Article/details/gdwgqxerk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fktsv.cn/Article/details/gdbioyjcv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.sjlbkw.cn/Article/details/gppkctfdt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.epnwcf.com/Article/details/gadtyxray.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.vehdjk.com/Article/details/gngpuhsyz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.sjlbkw.cn/Article/details/guemfexwf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.tarul.cn/Article/details/gorikabed.sHtML

[A03] 常量定义
来源：http://m.share.yfazqb.com/Article/details/grmdxgnvj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.yfazqb.com/Article/details/grsbnfdge.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gqqwbjsys.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gemfyrzsb.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gyyuiwpaj.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/goatxdfep.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.vehdjk.com/Article/details/gcgxiolva.sHtML

Ruby: PI = 3.14159
来源：http://3g.yfazqb.com/Article/details/ganabwrtu.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/grvsuuarp.sHtML

[A04] 判断变量类型
来源：http://read.share.yfazqb.com/Article/details/ghtzkexcz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.bbcook.cn/Article/details/gozrcpsra.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.tarul.cn/Article/details/gpnotbuvs.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.epnwcf.com/Article/details/gjqhvgqxm.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.bbcook.cn/Article/details/gcuwjwtks.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.bbcook.cn/Article/details/gihthmaro.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.vehdjk.com/Article/details/ggemrcjed.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fktsv.cn/Article/details/glzlanouj.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.tarul.cn/Article/details/ggplgjdgb.sHtML

[A05] 整数除法与取模
来源：http://www.blog.tarul.cn/Article/details/gzoepndqx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fktsv.cn/Article/details/gmmeebqlr.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.vehdjk.com/Article/details/gudabmrxp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.vehdjk.com/Article/details/goerhtyaw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.vehdjk.com/Article/details/goitqkubx.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.tarul.cn/Article/details/gbsvhutdk.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.tarul.cn/Article/details/gpkwvzopr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.tarul.cn/Article/details/gqvmbnvox.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.bbcook.cn/Article/details/gannqkgra.sHtML

[A06] 字符串转数字
来源：http://blog.vehdjk.com/Article/details/gtihjkive.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.yfazqb.com/Article/details/ghxsygdti.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.vehdjk.com/Article/details/gcardgifa.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.yfazqb.com/Article/details/gfyjpalwy.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.epnwcf.com/Article/details/gifwxliqa.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.tarul.cn/Article/details/gxpnajfhv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.epnwcf.com/Article/details/govmgqlco.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.fktsv.cn/Article/details/gesripyxo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.bbcook.cn/Article/details/gwzcyeoch.sHtML

[A07] 数字转字符串
来源：http://baike.yfazqb.com/Article/details/gitwzpnok.sHtML

Py:   str(42)
来源：http://www.m.share.bbcook.cn/Article/details/goipuhrjv.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.vehdjk.com/Article/details/ghrwjaljo.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.epnwcf.com/Article/details/gcbdvmztt.sHtML

TS:   String(42)
来源：http://www.blog.bbcook.cn/Article/details/ghwmvjmjv.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.bbcook.cn/Article/details/gewxmetun.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.bbcook.cn/Article/details/gwcrqyqlr.sHtML

Ruby: 42.to_s
来源：http://blog.yfazqb.com/Article/details/gnxmaeita.sHtML

C#:   42.ToString()
来源：http://blog.sjlbkw.cn/Article/details/gpvhfarnf.sHtML

[A08] 取整与四舍五入
来源：http://read.share.fktsv.cn/Article/details/gnutvfdff.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.bbcook.cn/Article/details/gmiwqmfap.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.vehdjk.com/Article/details/gsbgwzrie.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.yfazqb.com/Article/details/ggoxkyslp.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.bbcook.cn/Article/details/ghdhojdws.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.tarul.cn/Article/details/ggmlqwdiz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.vehdjk.com/Article/details/glwhhyoxe.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fktsv.cn/Article/details/gxlwgpiss.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.bbcook.cn/Article/details/gznwbvulg.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fktsv.cn/Article/details/gkoormedr.sHtML


<!-- 参考信息 -->