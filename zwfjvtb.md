代发 wailian999

[U59] PHP：自定义排序
来源：http://m.share.epnwcf.com/Article/details/gumxdaagi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.bbcook.cn/Article/details/gxyknqjpw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.vehdjk.com/Article/details/gzwcdxjif.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.bbcook.cn/Article/details/gszzsqtkr.sHtML

[U61] PHP：正则
来源：http://mobile.vehdjk.com/Article/details/ggfuwmenx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.sjlbkw.cn/Article/details/gmyalvgya.sHtML

[U62] PHP：日期对象
来源：http://baike.yfazqb.com/Article/details/gixtujhqw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.sjlbkw.cn/Article/details/ghnqbfxjn.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fktsv.cn/Article/details/ggxrwnkib.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.vehdjk.com/Article/details/gjtzhezut.sHtML

[U64] PHP：目录遍历
来源：http://m.share.epnwcf.com/Article/details/gjzavyznw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.tarul.cn/Article/details/gxkuifrrm.sHtML

[U65] PHP：会话
来源：http://wap.fktsv.cn/Article/details/gwmxhclzq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gcmpkuzau.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.sjlbkw.cn/Article/details/gbcubjprt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fktsv.cn/Article/details/gjqlwhwny.sHtML

[U67] PHP：处理文件上传
来源：http://baike.vehdjk.com/Article/details/gtemoweew.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fktsv.cn/Article/details/gevdkfapw.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.bbcook.cn/Article/details/gmrobhwqt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.tarul.cn/Article/details/gvmfwtenm.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.sjlbkw.cn/Article/details/gofzbbwwi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.yfazqb.com/Article/details/gkkjumarb.sHtML

[U70] PHP：PDO 事务
来源：http://baike.yfazqb.com/Article/details/ghnknacga.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.sjlbkw.cn/Article/details/gpvixztmy.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fktsv.cn/Article/details/gqgwikmuj.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.tarul.cn/Article/details/gxaptjrfa.sHtML

[U72] PHP：写错误日志
来源：http://baike.yfazqb.com/Article/details/gdxyifhci.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.epnwcf.com/Article/details/gvngmjleo.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.epnwcf.com/Article/details/gwoqljjag.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.vehdjk.com/Article/details/gufqsqoyb.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.tarul.cn/Article/details/gmameesmd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.vehdjk.com/Article/details/gqlrcyiew.sHtML

[U75] PHP：依赖注入
来源：http://mobile.bbcook.cn/Article/details/gmfutoixg.sHtML

composer require psr/container
来源：http://wap.tarul.cn/Article/details/gxofpleob.sHtML

[U76] PHP：简单路由
来源：http://www.blog.vehdjk.com/Article/details/ggyehirkt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.bbcook.cn/Article/details/gitqmfmfz.sHtML

[U77] PHP：模板渲染
来源：http://3g.sjlbkw.cn/Article/details/gizjjwsyb.sHtML

composer require twig/twig
来源：http://www.blog.tarul.cn/Article/details/gblwmdreo.sHtML

[U78] PHP：单元测试
来源：http://www.blog.yfazqb.com/Article/details/gxtmwgboj.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.vehdjk.com/Article/details/gnkuqvmdu.sHtML

[U79] PHP：静态分析
来源：http://m.share.bbcook.cn/Article/details/goxrodgpj.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.bbcook.cn/Article/details/grbyzunin.sHtML

[U80] PHP：代码规范修复
来源：http://blog.sjlbkw.cn/Article/details/gbgiflbfd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.epnwcf.com/Article/details/gpcevgdjg.sHtML

[U81] JS：初始化项目
来源：http://m.share.tarul.cn/Article/details/gswpxlned.sHtML

npm init -y;  npm i express
来源：http://read.share.fktsv.cn/Article/details/googlsuoa.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.bbcook.cn/Article/details/gzjgbrpok.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fktsv.cn/Article/details/gkndughza.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.epnwcf.com/Article/details/gxumsrhtt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.epnwcf.com/Article/details/gbjvncvhy.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.sjlbkw.cn/Article/details/gwavuvjfz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.vehdjk.com/Article/details/gtzwcvmub.sHtML

[U85] JS：可选链
来源：http://3g.fktsv.cn/Article/details/ghtjhhszz.sHtML

a?.b?.c
来源：http://wap.fktsv.cn/Article/details/ghehksahf.sHtML

[U86] JS：空值合并
来源：http://baike.epnwcf.com/Article/details/gdxstgzts.sHtML

a ?? b
来源：http://www.share.tarul.cn/Article/details/gnsveotbi.sHtML

[U87] JS：解构默认值
来源：http://mobile.epnwcf.com/Article/details/gpafpjnkh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.vehdjk.com/Article/details/gqeugnhfw.sHtML

[U88] JS：对象展开合并
来源：http://wap.sjlbkw.cn/Article/details/gfusyopcm.sHtML

{ ...a, ...b }
来源：http://www.share.tarul.cn/Article/details/gqqibtvxx.sHtML

[U89] JS：数组去重
来源：http://blog.fktsv.cn/Article/details/grturistr.sHtML

[...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/gztbftiqt.sHtML

[U90] JS：数字数组排序
来源：http://read.share.epnwcf.com/Article/details/gsemhpjxx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fktsv.cn/Article/details/galsxvusn.sHtML

[U91] JS：对象键值遍历
来源：http://wap.sjlbkw.cn/Article/details/gzqdxxghd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.bbcook.cn/Article/details/gspftxuln.sHtML

[U92] JS：深拷贝
来源：http://blog.vehdjk.com/Article/details/gcfbunmrk.sHtML

structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/gqncviqlh.sHtML

[U93] JS：模板字符串
来源：http://read.share.fktsv.cn/Article/details/gndyeokgs.sHtML

`共 ${n} 条`
来源：http://3g.yfazqb.com/Article/details/gqetqctkq.sHtML

[U94] JS：箭头函数
来源：http://read.share.vehdjk.com/Article/details/gudtsxmza.sHtML

const double = x => x * 2;
来源：http://3g.vehdjk.com/Article/details/guxjhnnjo.sHtML

[U95] JS：Promise 包装
来源：http://www.share.epnwcf.com/Article/details/glestneur.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fktsv.cn/Article/details/glrqettkv.sHtML

[U96] JS：async/await 与异常
来源：http://blog.tarul.cn/Article/details/gpnqgmeoa.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/gnbnrgsro.sHtML

[U97] JS：并发请求
来源：http://m.share.yfazqb.com/Article/details/gszijpzxn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/govyoxrot.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.bbcook.cn/Article/details/gyddfezlx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.vehdjk.com/Article/details/gdgyihmzz.sHtML

[U99] JS：事件监听
来源：http://3g.tarul.cn/Article/details/gpiqxdukj.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.vehdjk.com/Article/details/gdqizklul.sHtML

[U100] JS：DOM 查询
来源：http://blog.sjlbkw.cn/Article/details/ggctvcrzu.sHtML

document.querySelector(".item")
来源：http://mobile.yfazqb.com/Article/details/gujhzkbjb.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.tarul.cn/Article/details/gzggrxmyh.sHtML

el.classList.toggle("active")
来源：http://www.blog.bbcook.cn/Article/details/gaooylzzt.sHtML

[U102] JS：本地存储
来源：http://mobile.epnwcf.com/Article/details/gvpnkdckx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.vehdjk.com/Article/details/gftbngmlu.sHtML

[U103] JS：定时器
来源：http://baike.bbcook.cn/Article/details/gnhzdpzbu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fktsv.cn/Article/details/gqvpfeejl.sHtML

[U104] JS：防抖
来源：http://mobile.fktsv.cn/Article/details/gfokzdwkf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/gwepoqpte.sHtML

[U105] JS：节流
来源：http://read.share.sjlbkw.cn/Article/details/gvkurmavm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.vehdjk.com/Article/details/gjvypccnz.sHtML

[U106] JS：日期格式化
来源：http://wap.vehdjk.com/Article/details/grmptgijd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.vehdjk.com/Article/details/ghyghndey.sHtML

[U107] JS：数字千分位
来源：http://wap.sjlbkw.cn/Article/details/gmnwqdkjo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.epnwcf.com/Article/details/gparkosxt.sHtML

[U108] JS：随机整数
来源：http://blog.vehdjk.com/Article/details/gvdkjvvza.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fktsv.cn/Article/details/ggfrzxuga.sHtML

[U109] JS：数组分组
来源：http://3g.tarul.cn/Article/details/gpnwwushb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.vehdjk.com/Article/details/gepycyizs.sHtML

[U110] JS：数组分块
来源：http://baike.tarul.cn/Article/details/gwzpkvrdv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.vehdjk.com/Article/details/ggvkfvltl.sHtML

[U111] JS：对象转 Map
来源：http://wap.tarul.cn/Article/details/gixbaejrz.sHtML

new Map(Object.entries(obj))
来源：http://wap.epnwcf.com/Article/details/ggygpkvwz.sHtML

[U112] JS：字符串补位
来源：http://3g.fktsv.cn/Article/details/gpognfeop.sHtML

"7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/gqfzkkloz.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.vehdjk.com/Article/details/gattbxrfg.sHtML

s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gdrzcpjau.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.tarul.cn/Article/details/giusqbqkz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fktsv.cn/Article/details/gbkzfkqlh.sHtML

[U115] JS：生成 UUID
来源：http://m.share.tarul.cn/Article/details/gaerxmxtn.sHtML

crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/geljbdsaf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.tarul.cn/Article/details/gjkbqmhtv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.bbcook.cn/Article/details/gqxrgtgnh.sHtML

[U117] JS：单元测试
来源：http://3g.fktsv.cn/Article/details/gundmbkar.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.vehdjk.com/Article/details/gtykjyixf.sHtML

[U118] JS：开发服务器
来源：http://mobile.yfazqb.com/Article/details/gdgqgcwlo.sHtML

npm i -D vite;  npx vite
来源：http://m.share.yfazqb.com/Article/details/gwxisjhkx.sHtML

[U119] JS：生产构建
来源：http://m.share.vehdjk.com/Article/details/gibwxblrc.sHtML

npx vite build
来源：http://wap.vehdjk.com/Article/details/grkjjdbmx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.yfazqb.com/Article/details/gnmzgolnb.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.bbcook.cn/Article/details/gigsfgzla.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gymdwvage.sHtML

统计汇总
来源：http://www.blog.tarul.cn/Article/details/glyqciaen.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gbvadrvls.sHtML

按语言统计（条）：
来源：http://blog.vehdjk.com/Article/details/gjtiorkrt.sHtML

Python ......... 252
来源：http://wap.fktsv.cn/Article/details/gxgquaukb.sHtML

PHP ............ 252
来源：http://m.share.sjlbkw.cn/Article/details/gcgnyufvr.sHtML

JavaScript ..... 252
来源：http://www.m.share.tarul.cn/Article/details/gnqbimomz.sHtML

TypeScript ..... 212
来源：http://mobile.bbcook.cn/Article/details/gpmyjiflo.sHtML

Java ........... 212
来源：http://read.share.yfazqb.com/Article/details/gyvrpmztb.sHtML

Go ............. 212
来源：http://www.share.tarul.cn/Article/details/gdtzfbsnz.sHtML

Ruby ........... 212
来源：http://www.blog.tarul.cn/Article/details/gypruhcfo.sHtML

C# ............. 212
来源：http://wap.yfazqb.com/Article/details/gmxwvfirl.sHtML

C .............. 30
来源：http://m.share.tarul.cn/Article/details/gztqcjnih.sHtML

C++ ............ 30
来源：http://wap.sjlbkw.cn/Article/details/gqyajzqvu.sHtML

SQL ............ 90
来源：http://www.share.vehdjk.com/Article/details/gxewjxszr.sHtML

Bash ........... 80
来源：http://3g.fktsv.cn/Article/details/gdnnkzvmj.sHtML

Kotlin ......... 15
来源：http://3g.sjlbkw.cn/Article/details/gjswrzfrp.sHtML

Swift .......... 15
来源：http://www.m.share.fktsv.cn/Article/details/gegmnfrfa.sHtML

Lua ............ 10
来源：http://www.share.sjlbkw.cn/Article/details/gzoalntzt.sHtML

Perl ........... 10
来源：http://3g.bbcook.cn/Article/details/gznoqsixm.sHtML

Scala .......... 10
来源：http://www.m.share.bbcook.cn/Article/details/gparmccvq.sHtML

------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gzlhiwjkc.sHtML

合计 ........... 2106 条
来源：http://m.share.sjlbkw.cn/Article/details/gjicadkkc.sHtML

按章节统计：
来源：http://www.blog.yfazqb.com/Article/details/gngicrzpk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fktsv.cn/Article/details/gananqzzs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fktsv.cn/Article/details/giryvaxic.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.yfazqb.com/Article/details/gfsdzibkc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.epnwcf.com/Article/details/gwvugynyu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.bbcook.cn/Article/details/gmghndwah.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.bbcook.cn/Article/details/gkdkhlvui.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.bbcook.cn/Article/details/gqnfsfkwd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.bbcook.cn/Article/details/gntmxfpse.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/giptriwqz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.tarul.cn/Article/details/gmwfewuln.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/ggmjyigub.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gqegqghfa.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/golckuwfg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fktsv.cn/Article/details/gzddknnmh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.tarul.cn/Article/details/gnjobtdra.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/glbcmgzqe.sHtML

Q SQL 专题                              90
来源：http://www.m.share.tarul.cn/Article/details/gybkqducn.sHtML

R Bash 专题                             80
来源：http://read.share.fktsv.cn/Article/details/gkkpqcgrn.sHtML

S C / C++ 专题                          60
来源：http://m.share.epnwcf.com/Article/details/gcadfnvpn.sHtML

T 其他语言补充                          60
来源：http://m.share.yfazqb.com/Article/details/glaylmicq.sHtML

U 高频实用片段                         120
来源：http://mobile.fktsv.cn/Article/details/gvchpfgef.sHtML

------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gdibnnlyl.sHtML

合计                                  2106 条
来源：http://read.share.sjlbkw.cn/Article/details/gqaflttnz.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gpkyrkgow.sHtML

使用提醒
来源：http://mobile.fktsv.cn/Article/details/gyojfzygk.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.epnwcf.com/Article/details/gnowccjqg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.epnwcf.com/Article/details/ggvfzujhv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.vehdjk.com/Article/details/gmbiyyrcu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.sjlbkw.cn/Article/details/gbpmcxuie.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.sjlbkw.cn/Article/details/gctoqpnyi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.bbcook.cn/Article/details/gmrulerxh.sHtML

—— 文件结束 ——
来源：http://read.share.bbcook.cn/Article/details/gqczqnpkv.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gyhaeajqr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.epnwcf.com/Article/details/goxqwjrlg.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.bbcook.cn/Article/details/gziyrcaru.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ghqqrqhsb.sHtML

【收录内容】
来源：http://3g.vehdjk.com/Article/details/ghxsibsfr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.vehdjk.com/Article/details/gfvkfglkk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.tarul.cn/Article/details/gssijipwg.sHtML

SQL · Bash · C · C++
来源：http://3g.yfazqb.com/Article/details/gtkjvvsyn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.yfazqb.com/Article/details/gjdnhcsaf.sHtML

【使用说明】
来源：http://wap.tarul.cn/Article/details/gcdbhttxr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.tarul.cn/Article/details/ghunaceve.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.yfazqb.com/Article/details/gidfeevjw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.bbcook.cn/Article/details/gpyhnbvte.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.vehdjk.com/Article/details/gmurokkfv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.vehdjk.com/Article/details/gsmxsurlu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.yfazqb.com/Article/details/gveamuehj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fktsv.cn/Article/details/gowhcbhde.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.vehdjk.com/Article/details/gnchgecjn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.yfazqb.com/Article/details/gfuygptkn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.sjlbkw.cn/Article/details/gdobckkhd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.yfazqb.com/Article/details/gbxdgjzuu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.yfazqb.com/Article/details/gaaddidod.sHtML

【文件统计】
来源：http://read.share.yfazqb.com/Article/details/gshxisqrj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.yfazqb.com/Article/details/gldzxivyk.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gwjgeqtlv.sHtML

目  录
来源：http://read.share.epnwcf.com/Article/details/gnussxple.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gmibpvfqh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fktsv.cn/Article/details/gtmayumpv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.sjlbkw.cn/Article/details/glpcvetjp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.epnwcf.com/Article/details/gkjqwqfqk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.yfazqb.com/Article/details/gsblsekxr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.vehdjk.com/Article/details/gxinpwlzu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.epnwcf.com/Article/details/glosmravn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.epnwcf.com/Article/details/grrmkgyhv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fktsv.cn/Article/details/gfeprmmix.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.vehdjk.com/Article/details/gpxpvhyff.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.tarul.cn/Article/details/gfrdocchc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gevlihrhw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/gzyscemjh.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.tarul.cn/Article/details/glwesoswi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fktsv.cn/Article/details/geyxjkemv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.vehdjk.com/Article/details/gsbxomqqn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/gqcrzcweq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.bbcook.cn/Article/details/goyqhnalc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.tarul.cn/Article/details/guipzcykn.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.epnwcf.com/Article/details/gtztogcic.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.vehdjk.com/Article/details/gnwswoqgm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.epnwcf.com/Article/details/gjxwbsyzd.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gkgdedzwg.sHtML

A. 基础语法与类型
来源：http://mobile.sjlbkw.cn/Article/details/gjmknctrn.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/guyavvxkw.sHtML

[A01] Hello World
来源：http://www.blog.yfazqb.com/Article/details/guobyighh.sHtML

Py:   print("Hello, World!")
来源：http://wap.fktsv.cn/Article/details/gwiimqnyw.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fktsv.cn/Article/details/ghfqpeeqv.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.tarul.cn/Article/details/gpvxvyykw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.sjlbkw.cn/Article/details/gljqxzvfg.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fktsv.cn/Article/details/gdfuucabu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.vehdjk.com/Article/details/gkdnbxbhy.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.vehdjk.com/Article/details/ggqignzpo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.bbcook.cn/Article/details/gqnkovtrf.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.bbcook.cn/Article/details/gyobzroxe.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.epnwcf.com/Article/details/giioghqok.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.bbcook.cn/Article/details/gqgfewqgy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.tarul.cn/Article/details/grbwvfpmv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.bbcook.cn/Article/details/gkovrlcyf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.epnwcf.com/Article/details/gwagkzzfx.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fktsv.cn/Article/details/gbjrfrevn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.sjlbkw.cn/Article/details/gzxampzbv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.tarul.cn/Article/details/gqufrrboj.sHtML

[A03] 常量定义
来源：http://blog.fktsv.cn/Article/details/giolaygid.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.epnwcf.com/Article/details/grbewycte.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gvkknzzgg.sHtML

JS:   const PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gufxfghnn.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gvpzgwyyb.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gtujtgfit.sHtML

Go:   const PI = 3.14159
来源：http://baike.yfazqb.com/Article/details/gtayybtki.sHtML

Ruby: PI = 3.14159
来源：http://m.share.tarul.cn/Article/details/gwewbbgoz.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gbrpmyhub.sHtML

[A04] 判断变量类型
来源：http://m.share.fktsv.cn/Article/details/gisxrorli.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.epnwcf.com/Article/details/grfnfrhuw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.tarul.cn/Article/details/gmcykpmro.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fktsv.cn/Article/details/ggocfuarq.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fktsv.cn/Article/details/ghgddcfqm.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fktsv.cn/Article/details/gywrjbzpw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.vehdjk.com/Article/details/gjmxdfqxp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.tarul.cn/Article/details/gebnbdauj.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.tarul.cn/Article/details/glsianhat.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.yfazqb.com/Article/details/gcpyluuqh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.vehdjk.com/Article/details/gbzuvzzkk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/gatxsqjdi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gfwpcforw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/gnkkmoxcd.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/gbhzjcfhs.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gwxdtalvl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.sjlbkw.cn/Article/details/gyvwctpqt.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gyamwpqux.sHtML

[A06] 字符串转数字
来源：http://baike.fktsv.cn/Article/details/gavsbhvgy.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.tarul.cn/Article/details/gyprygeqa.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.bbcook.cn/Article/details/grftplhhh.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.vehdjk.com/Article/details/glgcftznr.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.epnwcf.com/Article/details/gpsvofjvq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.epnwcf.com/Article/details/gkgnbxtyq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.sjlbkw.cn/Article/details/gifkumtjm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.yfazqb.com/Article/details/gztpmghnm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.vehdjk.com/Article/details/gqcgyjkky.sHtML

[A07] 数字转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/glcvevtsy.sHtML

Py:   str(42)
来源：http://read.share.fktsv.cn/Article/details/gllxprauk.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fktsv.cn/Article/details/gguijvxvy.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fktsv.cn/Article/details/giacqmwdv.sHtML

TS:   String(42)
来源：http://baike.bbcook.cn/Article/details/glppskodn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.yfazqb.com/Article/details/gvnxvxzmp.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.yfazqb.com/Article/details/gzouwfffo.sHtML

Ruby: 42.to_s
来源：http://m.share.epnwcf.com/Article/details/gfobdmoyv.sHtML

C#:   42.ToString()
来源：http://baike.bbcook.cn/Article/details/gzmwnuvjs.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.tarul.cn/Article/details/gzdbjkfhr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.tarul.cn/Article/details/gyyitefdi.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.bbcook.cn/Article/details/gqpoiayfo.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/ghrzhfcjt.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.bbcook.cn/Article/details/gszxvhbvn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.vehdjk.com/Article/details/grocgihne.sHtML


<!-- 参考信息 -->