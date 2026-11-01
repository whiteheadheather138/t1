代发 wailian999

[U51] PHP：数组解构
来源：http://mobile.tarul.cn/Article/details/ggvzaubbo.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fktsv.cn/Article/details/gtzfbjyfk.sHtML

[U52] PHP：箭头函数
来源：http://www.share.vehdjk.com/Article/details/giolxfzvr.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.sjlbkw.cn/Article/details/gdfzguyxt.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.bbcook.cn/Article/details/grdreynhs.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.epnwcf.com/Article/details/gwrvdayvf.sHtML

[U54] PHP：空安全调用
来源：http://m.share.epnwcf.com/Article/details/giwienrht.sHtML

$obj?->method()
来源：http://3g.fktsv.cn/Article/details/gyjtkcyuy.sHtML

[U55] PHP：match 表达式
来源：http://m.share.tarul.cn/Article/details/gixtxavop.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.bbcook.cn/Article/details/gtlsqnmym.sHtML

[U56] PHP：命名参数
来源：http://3g.bbcook.cn/Article/details/gnlqmkzer.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/giyadlbnv.sHtML

[U57] PHP：字符串插值
来源：http://baike.vehdjk.com/Article/details/ghygoaqiy.sHtML

"值: {$a}"
来源：http://baike.bbcook.cn/Article/details/gxucxcchj.sHtML

[U58] PHP：数组三件套
来源：http://wap.sjlbkw.cn/Article/details/gyemqdnkw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gijmmrvtw.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fktsv.cn/Article/details/gceuijwmz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.vehdjk.com/Article/details/gsoegmybx.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.yfazqb.com/Article/details/gpbmnwbyh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.bbcook.cn/Article/details/gdwufygna.sHtML

[U61] PHP：正则
来源：http://baike.vehdjk.com/Article/details/gbewjrajq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.yfazqb.com/Article/details/gecwcflet.sHtML

[U62] PHP：日期对象
来源：http://baike.tarul.cn/Article/details/gkkzbwvpd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.vehdjk.com/Article/details/gjtagclxp.sHtML

[U63] PHP：文件读写
来源：http://blog.sjlbkw.cn/Article/details/gtaxtymoi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.vehdjk.com/Article/details/gicwthsoi.sHtML

[U64] PHP：目录遍历
来源：http://m.share.vehdjk.com/Article/details/gvjxmnnpr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.sjlbkw.cn/Article/details/gqugtnmqc.sHtML

[U65] PHP：会话
来源：http://wap.bbcook.cn/Article/details/gnhngzgfb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.tarul.cn/Article/details/gcspdykkh.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.epnwcf.com/Article/details/gsgqtxxlt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.sjlbkw.cn/Article/details/genzkczdm.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.yfazqb.com/Article/details/gipuiuady.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.vehdjk.com/Article/details/gjmgusuxm.sHtML

[U68] PHP：PDO 连接
来源：http://blog.bbcook.cn/Article/details/giodtpgjs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.vehdjk.com/Article/details/gygprsmjw.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.sjlbkw.cn/Article/details/gipdbycoq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.sjlbkw.cn/Article/details/gzsyfgexg.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.tarul.cn/Article/details/ghifadujx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.bbcook.cn/Article/details/gtwkwjzal.sHtML

[U71] PHP：抛出异常
来源：http://blog.fktsv.cn/Article/details/gccaafqcn.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fktsv.cn/Article/details/gldbbnbvo.sHtML

[U72] PHP：写错误日志
来源：http://mobile.bbcook.cn/Article/details/gddtfagck.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.vehdjk.com/Article/details/gmenwqjqg.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.vehdjk.com/Article/details/gcjeuzmrh.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.bbcook.cn/Article/details/grljjvzwg.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.epnwcf.com/Article/details/gkwcpehcm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.vehdjk.com/Article/details/ggpzihtob.sHtML

[U75] PHP：依赖注入
来源：http://m.share.sjlbkw.cn/Article/details/grsuntxzm.sHtML

composer require psr/container
来源：http://wap.vehdjk.com/Article/details/gxypoyrny.sHtML

[U76] PHP：简单路由
来源：http://m.share.epnwcf.com/Article/details/gavniercc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fktsv.cn/Article/details/gybmiellj.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.bbcook.cn/Article/details/gjdlgrqkd.sHtML

composer require twig/twig
来源：http://wap.fktsv.cn/Article/details/gsaxsjchs.sHtML

[U78] PHP：单元测试
来源：http://www.share.fktsv.cn/Article/details/gvxypeiml.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.sjlbkw.cn/Article/details/gbqhubmqx.sHtML

[U79] PHP：静态分析
来源：http://m.share.sjlbkw.cn/Article/details/gdgskijag.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.sjlbkw.cn/Article/details/gmclhiyln.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fktsv.cn/Article/details/gjwaaggsv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.epnwcf.com/Article/details/glwpkabum.sHtML

[U81] JS：初始化项目
来源：http://read.share.epnwcf.com/Article/details/giqoeoara.sHtML

npm init -y;  npm i express
来源：http://www.blog.tarul.cn/Article/details/gilotzlnb.sHtML

[U82] JS：package.json 脚本
来源：http://baike.bbcook.cn/Article/details/gyclfxzbs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.bbcook.cn/Article/details/gkvfmaodz.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.vehdjk.com/Article/details/gtdhacouc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.tarul.cn/Article/details/gwxyvnmps.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.sjlbkw.cn/Article/details/gfzlgpmtc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.epnwcf.com/Article/details/gxfbryhhu.sHtML

[U85] JS：可选链
来源：http://3g.sjlbkw.cn/Article/details/gvcixjiaz.sHtML

a?.b?.c
来源：http://3g.sjlbkw.cn/Article/details/guhcnuhyz.sHtML

[U86] JS：空值合并
来源：http://read.share.tarul.cn/Article/details/glmnptwwq.sHtML

a ?? b
来源：http://m.share.yfazqb.com/Article/details/gboaabgva.sHtML

[U87] JS：解构默认值
来源：http://m.share.sjlbkw.cn/Article/details/gwzrcrwvj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.sjlbkw.cn/Article/details/gwheihhwz.sHtML

[U88] JS：对象展开合并
来源：http://mobile.tarul.cn/Article/details/goanrvqhx.sHtML

{ ...a, ...b }
来源：http://mobile.sjlbkw.cn/Article/details/glniolkhg.sHtML

[U89] JS：数组去重
来源：http://3g.fktsv.cn/Article/details/gzucocsoq.sHtML

[...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/gytgclvvp.sHtML

[U90] JS：数字数组排序
来源：http://read.share.vehdjk.com/Article/details/gdvkrayow.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/guktmwfmx.sHtML

[U91] JS：对象键值遍历
来源：http://baike.vehdjk.com/Article/details/gretpzfnz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.yfazqb.com/Article/details/guqxjradm.sHtML

[U92] JS：深拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gondqjgju.sHtML

structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gyyqdwzey.sHtML

[U93] JS：模板字符串
来源：http://read.share.tarul.cn/Article/details/gxopczxap.sHtML

`共 ${n} 条`
来源：http://www.m.share.fktsv.cn/Article/details/glsysgzno.sHtML

[U94] JS：箭头函数
来源：http://www.blog.sjlbkw.cn/Article/details/gzskzcrie.sHtML

const double = x => x * 2;
来源：http://m.share.vehdjk.com/Article/details/gdqykhplz.sHtML

[U95] JS：Promise 包装
来源：http://mobile.yfazqb.com/Article/details/grvatjsoo.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.yfazqb.com/Article/details/gzamqtgdi.sHtML

[U96] JS：async/await 与异常
来源：http://blog.epnwcf.com/Article/details/ggqeivspj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.tarul.cn/Article/details/gsftxauog.sHtML

[U97] JS：并发请求
来源：http://www.m.share.vehdjk.com/Article/details/gqlkwdtij.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gnohzlvqa.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.yfazqb.com/Article/details/gegrpqhnz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.bbcook.cn/Article/details/gamxzcuii.sHtML

[U99] JS：事件监听
来源：http://www.share.sjlbkw.cn/Article/details/gyucgiapt.sHtML

el.addEventListener("click", e => {})
来源：http://wap.bbcook.cn/Article/details/gtvmhtynr.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.sjlbkw.cn/Article/details/gfsapgknb.sHtML

document.querySelector(".item")
来源：http://www.share.yfazqb.com/Article/details/gsctqrmyy.sHtML

[U101] JS：classList 操作
来源：http://baike.fktsv.cn/Article/details/gfydnuadp.sHtML

el.classList.toggle("active")
来源：http://m.share.sjlbkw.cn/Article/details/gefuyoget.sHtML

[U102] JS：本地存储
来源：http://mobile.yfazqb.com/Article/details/gwklnckyk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.bbcook.cn/Article/details/ghknqmacm.sHtML

[U103] JS：定时器
来源：http://baike.epnwcf.com/Article/details/gtgfkhecl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fktsv.cn/Article/details/gkszmylsx.sHtML

[U104] JS：防抖
来源：http://read.share.vehdjk.com/Article/details/gmjkbrira.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/geonncwkd.sHtML

[U105] JS：节流
来源：http://mobile.sjlbkw.cn/Article/details/gneehbuew.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.tarul.cn/Article/details/gzdpiytho.sHtML

[U106] JS：日期格式化
来源：http://read.share.tarul.cn/Article/details/gxmnbexub.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.tarul.cn/Article/details/gvqhicuix.sHtML

[U107] JS：数字千分位
来源：http://read.share.bbcook.cn/Article/details/grrptwmsp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.epnwcf.com/Article/details/gewfuypai.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fktsv.cn/Article/details/gzxyaqyaj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.yfazqb.com/Article/details/gnawhhyqx.sHtML

[U109] JS：数组分组
来源：http://read.share.fktsv.cn/Article/details/gztsekfvb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fktsv.cn/Article/details/ggyhafbyj.sHtML

[U110] JS：数组分块
来源：http://www.blog.bbcook.cn/Article/details/geryxsvsp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.tarul.cn/Article/details/gcelubbar.sHtML

[U111] JS：对象转 Map
来源：http://blog.sjlbkw.cn/Article/details/gohflfbeb.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.epnwcf.com/Article/details/gsiejxbak.sHtML

[U112] JS：字符串补位
来源：http://baike.bbcook.cn/Article/details/gcbtumanz.sHtML

"7".padStart(3, "0")
来源：http://wap.epnwcf.com/Article/details/gjuilymju.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.yfazqb.com/Article/details/ggprrdetd.sHtML

s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/glmdmjmpq.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.tarul.cn/Article/details/gvdldcmdr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.tarul.cn/Article/details/gtwsflwuj.sHtML

[U115] JS：生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/gtgqwpdzx.sHtML

crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/gmqtdxlbh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fktsv.cn/Article/details/gwyphmwmk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.vehdjk.com/Article/details/gkneetesq.sHtML

[U117] JS：单元测试
来源：http://read.share.fktsv.cn/Article/details/gefcbhpue.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.sjlbkw.cn/Article/details/ggczuqipn.sHtML

[U118] JS：开发服务器
来源：http://www.share.fktsv.cn/Article/details/gcyhaoxnq.sHtML

npm i -D vite;  npx vite
来源：http://blog.yfazqb.com/Article/details/gvcrprnje.sHtML

[U119] JS：生产构建
来源：http://blog.vehdjk.com/Article/details/gemengndr.sHtML

npx vite build
来源：http://mobile.yfazqb.com/Article/details/gjcjjuoul.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fktsv.cn/Article/details/gnnimivyv.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fktsv.cn/Article/details/gujwrzagg.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gukqdltcf.sHtML

统计汇总
来源：http://3g.bbcook.cn/Article/details/ggzhjaoos.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gqmlbiscq.sHtML

按语言统计（条）：
来源：http://www.blog.bbcook.cn/Article/details/gekwljdux.sHtML

Python ......... 252
来源：http://baike.sjlbkw.cn/Article/details/gtakzqmbm.sHtML

PHP ............ 252
来源：http://blog.epnwcf.com/Article/details/gvimnpygb.sHtML

JavaScript ..... 252
来源：http://mobile.vehdjk.com/Article/details/gazwyvssy.sHtML

TypeScript ..... 212
来源：http://baike.epnwcf.com/Article/details/glygbplfm.sHtML

Java ........... 212
来源：http://www.share.bbcook.cn/Article/details/grrjmmuey.sHtML

Go ............. 212
来源：http://3g.vehdjk.com/Article/details/gvsolaswa.sHtML

Ruby ........... 212
来源：http://www.share.fktsv.cn/Article/details/gwzjqieqf.sHtML

C# ............. 212
来源：http://read.share.vehdjk.com/Article/details/gkqnqcdtx.sHtML

C .............. 30
来源：http://wap.sjlbkw.cn/Article/details/grlcsfzda.sHtML

C++ ............ 30
来源：http://3g.tarul.cn/Article/details/gcoknsgvq.sHtML

SQL ............ 90
来源：http://www.m.share.sjlbkw.cn/Article/details/gsaegusmw.sHtML

Bash ........... 80
来源：http://www.m.share.bbcook.cn/Article/details/gzkkdftia.sHtML

Kotlin ......... 15
来源：http://www.share.tarul.cn/Article/details/gzieqamgp.sHtML

Swift .......... 15
来源：http://mobile.bbcook.cn/Article/details/gmuudgiae.sHtML

Lua ............ 10
来源：http://mobile.vehdjk.com/Article/details/ghlrcxdgv.sHtML

Perl ........... 10
来源：http://wap.epnwcf.com/Article/details/gbkvxquxt.sHtML

Scala .......... 10
来源：http://m.share.tarul.cn/Article/details/grsvxwwcp.sHtML

------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gtkgmtphj.sHtML

合计 ........... 2106 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgtofbok.sHtML

按章节统计：
来源：http://read.share.epnwcf.com/Article/details/gjxnfvrbp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.vehdjk.com/Article/details/gihjsetss.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.yfazqb.com/Article/details/gwtxteeol.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.epnwcf.com/Article/details/gzbyezqor.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.yfazqb.com/Article/details/gagpsyqcb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.yfazqb.com/Article/details/goxzjougg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fktsv.cn/Article/details/gzmpmixpu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.yfazqb.com/Article/details/gqoflydow.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fktsv.cn/Article/details/grxmpqzmu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/gupgoprpg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.epnwcf.com/Article/details/gntcycium.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/grzefebuq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gwfrfsrme.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gecmvoypa.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.vehdjk.com/Article/details/gsbpjpyfc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fktsv.cn/Article/details/gusrmfhge.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gpnhusjiu.sHtML

Q SQL 专题                              90
来源：http://m.share.fktsv.cn/Article/details/gkqdssqpf.sHtML

R Bash 专题                             80
来源：http://m.share.tarul.cn/Article/details/gewgxyzfo.sHtML

S C / C++ 专题                          60
来源：http://m.share.sjlbkw.cn/Article/details/gdsxmgzzi.sHtML

T 其他语言补充                          60
来源：http://www.m.share.sjlbkw.cn/Article/details/gmytithic.sHtML

U 高频实用片段                         120
来源：http://blog.epnwcf.com/Article/details/grupitper.sHtML

------------------------------------
来源：http://m.share.yfazqb.com/Article/details/glpwjxoxb.sHtML

合计                                  2106 条
来源：http://3g.tarul.cn/Article/details/gpeqcjcnk.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.epnwcf.com/Article/details/gqifnrhqt.sHtML

使用提醒
来源：http://wap.bbcook.cn/Article/details/gktohsmhy.sHtML

--------------------------------------------------------------------------------
来源：http://baike.tarul.cn/Article/details/gjzsbjues.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.bbcook.cn/Article/details/gdyxuvxka.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.bbcook.cn/Article/details/gxebvvjcr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fktsv.cn/Article/details/gooxprakd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.bbcook.cn/Article/details/gmokhawmg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrcbibji.sHtML

—— 文件结束 ——
来源：http://mobile.tarul.cn/Article/details/gsqmjtzzg.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gyfmsdjwb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.bbcook.cn/Article/details/gcarqarim.sHtML

Common Programming Examples Cheat Book
来源：http://baike.vehdjk.com/Article/details/glbfxednk.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/giwvwijxx.sHtML

【收录内容】
来源：http://blog.epnwcf.com/Article/details/goimeyeyh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fktsv.cn/Article/details/gtzkxyiko.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.yfazqb.com/Article/details/gsmyuquut.sHtML

SQL · Bash · C · C++
来源：http://m.share.epnwcf.com/Article/details/gnmyvllid.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.vehdjk.com/Article/details/gkqfopkiy.sHtML

【使用说明】
来源：http://m.share.vehdjk.com/Article/details/gqbhlwiaj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.bbcook.cn/Article/details/gzagzxgnh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.yfazqb.com/Article/details/gggmolhcg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.sjlbkw.cn/Article/details/gjmjntqzb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.yfazqb.com/Article/details/ggrslqwhp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.yfazqb.com/Article/details/gojavoada.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fktsv.cn/Article/details/gowthilwt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.vehdjk.com/Article/details/grqrlyslc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.epnwcf.com/Article/details/gwudfxkqo.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.vehdjk.com/Article/details/gwthkdmtv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.vehdjk.com/Article/details/genggehmj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fktsv.cn/Article/details/gzjaiiqqp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.yfazqb.com/Article/details/guazglucg.sHtML

【文件统计】
来源：http://www.blog.bbcook.cn/Article/details/gczxynvga.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.tarul.cn/Article/details/ggvlfenxf.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.tarul.cn/Article/details/gswfrcink.sHtML

目  录
来源：http://blog.fktsv.cn/Article/details/gugjpvhgz.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gijtuoies.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.yfazqb.com/Article/details/gadwinlmx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.tarul.cn/Article/details/gxfscqcbf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.vehdjk.com/Article/details/gowkceizy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.vehdjk.com/Article/details/ghvjmsvji.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.yfazqb.com/Article/details/guuklvyua.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.yfazqb.com/Article/details/gkjlphzom.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.yfazqb.com/Article/details/gccftchon.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.epnwcf.com/Article/details/gsclsjzbf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/gtkmirzws.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.sjlbkw.cn/Article/details/givfhjjrn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/gsqintcvu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.epnwcf.com/Article/details/groweulsq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/gxfakjrkg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fktsv.cn/Article/details/guidrtwyd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fktsv.cn/Article/details/gkdjyvnda.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fktsv.cn/Article/details/gyeabrpms.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.bbcook.cn/Article/details/gvdcptjbe.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.vehdjk.com/Article/details/gxltwwmhm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.tarul.cn/Article/details/gdufrazyt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.vehdjk.com/Article/details/gxgpmwxlb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.tarul.cn/Article/details/gpssgwbrv.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ghdwfkspo.sHtML

A. 基础语法与类型
来源：http://3g.vehdjk.com/Article/details/gtqpazhqq.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gnczprtfd.sHtML

[A01] Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gydihsubx.sHtML

Py:   print("Hello, World!")
来源：http://wap.fktsv.cn/Article/details/gfktiechc.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.yfazqb.com/Article/details/grtgpfovj.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.tarul.cn/Article/details/gnhafvnei.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.bbcook.cn/Article/details/gtulyahgh.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.bbcook.cn/Article/details/gmlrqlenx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.vehdjk.com/Article/details/ggwrrrfkx.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.sjlbkw.cn/Article/details/goykinrwe.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.epnwcf.com/Article/details/grfihtkxs.sHtML

[A02] 变量声明与赋值
来源：http://wap.yfazqb.com/Article/details/grgprumbh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.tarul.cn/Article/details/gvfpuooid.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.yfazqb.com/Article/details/gwodxoeyi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fktsv.cn/Article/details/gjhqlqywa.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.sjlbkw.cn/Article/details/gdholjbhf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.tarul.cn/Article/details/gjvfspzsr.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.tarul.cn/Article/details/gnatjtpot.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.epnwcf.com/Article/details/gwkrscwgt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.epnwcf.com/Article/details/giiypfeim.sHtML

[A03] 常量定义
来源：http://www.blog.epnwcf.com/Article/details/gotxkaxkb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.epnwcf.com/Article/details/ggnnobgnb.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/govjtkbye.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gwzhlrkof.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gsflcdkhi.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/gtpljtshe.sHtML

Go:   const PI = 3.14159
来源：http://baike.yfazqb.com/Article/details/gvsqflswd.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.yfazqb.com/Article/details/gbehnxmsl.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gacdnjrxn.sHtML

[A04] 判断变量类型
来源：http://wap.epnwcf.com/Article/details/gdktdekwv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fktsv.cn/Article/details/giytwqrry.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.epnwcf.com/Article/details/gkxvpsdjd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.sjlbkw.cn/Article/details/gdjdyrsjs.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.tarul.cn/Article/details/gpmnvwvii.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fktsv.cn/Article/details/gwjvqdfpc.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.epnwcf.com/Article/details/gpoqejmkc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.bbcook.cn/Article/details/ggiznckpc.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.yfazqb.com/Article/details/gyoinixef.sHtML

[A05] 整数除法与取模
来源：http://mobile.epnwcf.com/Article/details/gubixhaai.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.yfazqb.com/Article/details/gsircbwqw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.epnwcf.com/Article/details/gbbbwxgly.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gluekrynu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.vehdjk.com/Article/details/gyzopguvb.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.yfazqb.com/Article/details/gcymvhbxh.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.bbcook.cn/Article/details/ggmtgpxer.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gpfhjqxcs.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.yfazqb.com/Article/details/ggpbojinb.sHtML

[A06] 字符串转数字
来源：http://www.blog.fktsv.cn/Article/details/gfwiidcxm.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.tarul.cn/Article/details/gyrszlwft.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.tarul.cn/Article/details/gshnfwphn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.vehdjk.com/Article/details/gfcdlgilg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.tarul.cn/Article/details/gnjqwkxxv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.epnwcf.com/Article/details/gwqkhjlce.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.epnwcf.com/Article/details/gmnkaihbi.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.epnwcf.com/Article/details/gauabzhdp.sHtML


<!-- 参考信息 -->