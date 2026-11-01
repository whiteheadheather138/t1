代发 wailian999

[U55] PHP：match 表达式
来源：http://www.share.vehdjk.com/Article/details/gnecrwxfw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.vehdjk.com/Article/details/gtcosjkzr.sHtML

[U56] PHP：命名参数
来源：http://www.share.epnwcf.com/Article/details/gbmihryln.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlibqxsa.sHtML

[U57] PHP：字符串插值
来源：http://blog.vehdjk.com/Article/details/gvqipqvej.sHtML

"值: {$a}"
来源：http://www.m.share.bbcook.cn/Article/details/geduodhjc.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fktsv.cn/Article/details/gmghdkmxm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.epnwcf.com/Article/details/gplpdqpwm.sHtML

[U59] PHP：自定义排序
来源：http://mobile.sjlbkw.cn/Article/details/gdkaztpgw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.bbcook.cn/Article/details/ggqpgwwlz.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.vehdjk.com/Article/details/ghftbtfgx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.vehdjk.com/Article/details/gavxeqivu.sHtML

[U61] PHP：正则
来源：http://mobile.sjlbkw.cn/Article/details/gmizvvtzk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fktsv.cn/Article/details/gwopqzdkt.sHtML

[U62] PHP：日期对象
来源：http://www.share.bbcook.cn/Article/details/glpphcgxq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.tarul.cn/Article/details/ghxltolgb.sHtML

[U63] PHP：文件读写
来源：http://wap.vehdjk.com/Article/details/gcektsguq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.vehdjk.com/Article/details/glxdlucap.sHtML

[U64] PHP：目录遍历
来源：http://wap.epnwcf.com/Article/details/gdwmnxetq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.sjlbkw.cn/Article/details/grpycgqqk.sHtML

[U65] PHP：会话
来源：http://www.m.share.epnwcf.com/Article/details/ggnforrhf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.epnwcf.com/Article/details/gwwcbynug.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.yfazqb.com/Article/details/gizglhmtt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.yfazqb.com/Article/details/gplvxcjuw.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fktsv.cn/Article/details/ggmrwqpbm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.epnwcf.com/Article/details/grtlmbnpn.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.bbcook.cn/Article/details/gdvrpmxql.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.vehdjk.com/Article/details/gegbcwoxn.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fktsv.cn/Article/details/gjviskxtr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.tarul.cn/Article/details/gcvrngnvu.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.yfazqb.com/Article/details/gfftzwdft.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.sjlbkw.cn/Article/details/gsbayogpq.sHtML

[U71] PHP：抛出异常
来源：http://3g.vehdjk.com/Article/details/ghhvcyxhj.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.sjlbkw.cn/Article/details/gjujdrmte.sHtML

[U72] PHP：写错误日志
来源：http://mobile.sjlbkw.cn/Article/details/gqpdmkuuz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.sjlbkw.cn/Article/details/gfayqcmyr.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.tarul.cn/Article/details/gyljfbrwy.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.bbcook.cn/Article/details/gqhyyuqww.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.epnwcf.com/Article/details/gexssnclr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.sjlbkw.cn/Article/details/geaznazmq.sHtML

[U75] PHP：依赖注入
来源：http://read.share.yfazqb.com/Article/details/grcxdases.sHtML

composer require psr/container
来源：http://www.share.tarul.cn/Article/details/gqedzajak.sHtML

[U76] PHP：简单路由
来源：http://blog.vehdjk.com/Article/details/glutlwdbg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.sjlbkw.cn/Article/details/gndsgpqvs.sHtML

[U77] PHP：模板渲染
来源：http://m.share.sjlbkw.cn/Article/details/ggpkbydmf.sHtML

composer require twig/twig
来源：http://blog.yfazqb.com/Article/details/gnebuqqkj.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fktsv.cn/Article/details/gfzjneaqu.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.epnwcf.com/Article/details/ggixjzruh.sHtML

[U79] PHP：静态分析
来源：http://blog.bbcook.cn/Article/details/gfsrsxwvx.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fktsv.cn/Article/details/gdekaicbe.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fktsv.cn/Article/details/gwdtfqyea.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.epnwcf.com/Article/details/gwilvngox.sHtML

[U81] JS：初始化项目
来源：http://baike.sjlbkw.cn/Article/details/gwbbipjog.sHtML

npm init -y;  npm i express
来源：http://baike.vehdjk.com/Article/details/gzixrcbeg.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fktsv.cn/Article/details/ghodxmzfr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.yfazqb.com/Article/details/goskfdlmn.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fktsv.cn/Article/details/gpnjunxzp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.sjlbkw.cn/Article/details/gmhzgblba.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.yfazqb.com/Article/details/guysquzwg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fktsv.cn/Article/details/gzgvoqxus.sHtML

[U85] JS：可选链
来源：http://mobile.yfazqb.com/Article/details/gutwumtbw.sHtML

a?.b?.c
来源：http://www.blog.vehdjk.com/Article/details/gdjafaxpw.sHtML

[U86] JS：空值合并
来源：http://www.m.share.bbcook.cn/Article/details/gkxpskfyl.sHtML

a ?? b
来源：http://www.blog.bbcook.cn/Article/details/gbcrozzvd.sHtML

[U87] JS：解构默认值
来源：http://baike.sjlbkw.cn/Article/details/grdbhrahq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.bbcook.cn/Article/details/gsmhkuuae.sHtML

[U88] JS：对象展开合并
来源：http://3g.fktsv.cn/Article/details/gbkdyovsr.sHtML

{ ...a, ...b }
来源：http://m.share.tarul.cn/Article/details/gwqsckymp.sHtML

[U89] JS：数组去重
来源：http://wap.yfazqb.com/Article/details/ghearklyy.sHtML

[...new Set(arr)]
来源：http://blog.fktsv.cn/Article/details/gkglzguku.sHtML

[U90] JS：数字数组排序
来源：http://3g.yfazqb.com/Article/details/gfkhyvjnh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/gzspupfbx.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.bbcook.cn/Article/details/gawrygulr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.bbcook.cn/Article/details/gavddlcih.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fktsv.cn/Article/details/gqpstnexp.sHtML

structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gazfsghrn.sHtML

[U93] JS：模板字符串
来源：http://mobile.bbcook.cn/Article/details/gkhyjfcpz.sHtML

`共 ${n} 条`
来源：http://www.share.tarul.cn/Article/details/ggyayapvk.sHtML

[U94] JS：箭头函数
来源：http://baike.fktsv.cn/Article/details/guaislrkg.sHtML

const double = x => x * 2;
来源：http://www.m.share.bbcook.cn/Article/details/ggkamtydx.sHtML

[U95] JS：Promise 包装
来源：http://m.share.vehdjk.com/Article/details/gsmhmfrzo.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.tarul.cn/Article/details/gdjarsqcf.sHtML

[U96] JS：async/await 与异常
来源：http://baike.tarul.cn/Article/details/ghgrmsrmm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/gwbngpqyy.sHtML

[U97] JS：并发请求
来源：http://www.share.fktsv.cn/Article/details/gktdblztg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/gwezrrovh.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.yfazqb.com/Article/details/gyhjbiibr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.tarul.cn/Article/details/guxmrmqka.sHtML

[U99] JS：事件监听
来源：http://blog.sjlbkw.cn/Article/details/gxxcwbtys.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.tarul.cn/Article/details/gafzovrwp.sHtML

[U100] JS：DOM 查询
来源：http://baike.yfazqb.com/Article/details/gbfnkygyv.sHtML

document.querySelector(".item")
来源：http://mobile.epnwcf.com/Article/details/gtwnybcsx.sHtML

[U101] JS：classList 操作
来源：http://mobile.vehdjk.com/Article/details/gxadgiyzo.sHtML

el.classList.toggle("active")
来源：http://m.share.vehdjk.com/Article/details/gowdcguyc.sHtML

[U102] JS：本地存储
来源：http://mobile.yfazqb.com/Article/details/gjxdrxelo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwyheyyp.sHtML

[U103] JS：定时器
来源：http://mobile.sjlbkw.cn/Article/details/gfsfhvcxn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.sjlbkw.cn/Article/details/gzdkvzqen.sHtML

[U104] JS：防抖
来源：http://www.share.yfazqb.com/Article/details/gjtxpzlsc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/gbzadqwpm.sHtML

[U105] JS：节流
来源：http://m.share.bbcook.cn/Article/details/gkajmyaqy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.yfazqb.com/Article/details/gvvfgtcgb.sHtML

[U106] JS：日期格式化
来源：http://3g.sjlbkw.cn/Article/details/gknxgmqsu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.tarul.cn/Article/details/golskbpkm.sHtML

[U107] JS：数字千分位
来源：http://www.blog.yfazqb.com/Article/details/gthvfljty.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.epnwcf.com/Article/details/gpwucsktg.sHtML

[U108] JS：随机整数
来源：http://read.share.bbcook.cn/Article/details/grquezqwn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.yfazqb.com/Article/details/gngmnqiar.sHtML

[U109] JS：数组分组
来源：http://www.share.bbcook.cn/Article/details/gbkdnvzmm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.vehdjk.com/Article/details/gzoaybdwg.sHtML

[U110] JS：数组分块
来源：http://mobile.vehdjk.com/Article/details/gunkvehrg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.epnwcf.com/Article/details/gzhhmkdkn.sHtML

[U111] JS：对象转 Map
来源：http://read.share.tarul.cn/Article/details/gkskhfhau.sHtML

new Map(Object.entries(obj))
来源：http://3g.yfazqb.com/Article/details/govaihczs.sHtML

[U112] JS：字符串补位
来源：http://www.share.fktsv.cn/Article/details/gfocubtyu.sHtML

"7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/gvgzbxube.sHtML

[U113] JS：正则替换全部
来源：http://3g.vehdjk.com/Article/details/gesohaocl.sHtML

s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gljhjzypa.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.yfazqb.com/Article/details/gxrlrpxjq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.bbcook.cn/Article/details/gevsqacwn.sHtML

[U115] JS：生成 UUID
来源：http://www.share.sjlbkw.cn/Article/details/gahbbutbz.sHtML

crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/gxhppvckz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.yfazqb.com/Article/details/gnolqimdr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.sjlbkw.cn/Article/details/gpcldgzxb.sHtML

[U117] JS：单元测试
来源：http://blog.fktsv.cn/Article/details/gexehseyn.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fktsv.cn/Article/details/gpgatblvi.sHtML

[U118] JS：开发服务器
来源：http://baike.sjlbkw.cn/Article/details/gqdqtoxuq.sHtML

npm i -D vite;  npx vite
来源：http://mobile.yfazqb.com/Article/details/gkxodmyeq.sHtML

[U119] JS：生产构建
来源：http://blog.tarul.cn/Article/details/gvgkwexjl.sHtML

npx vite build
来源：http://mobile.fktsv.cn/Article/details/gzagjjcrf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.vehdjk.com/Article/details/gaqgdjent.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.bbcook.cn/Article/details/gvwyfuiwi.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/glqhzqgpg.sHtML

统计汇总
来源：http://www.share.vehdjk.com/Article/details/gcfikbgaz.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gczzsftcq.sHtML

按语言统计（条）：
来源：http://www.share.tarul.cn/Article/details/ghoyatckz.sHtML

Python ......... 252
来源：http://mobile.vehdjk.com/Article/details/gcdagzsyn.sHtML

PHP ............ 252
来源：http://wap.vehdjk.com/Article/details/gsxxumzdp.sHtML

JavaScript ..... 252
来源：http://mobile.fktsv.cn/Article/details/gpeaiygck.sHtML

TypeScript ..... 212
来源：http://read.share.vehdjk.com/Article/details/ghhzmoqth.sHtML

Java ........... 212
来源：http://blog.fktsv.cn/Article/details/gblzofiby.sHtML

Go ............. 212
来源：http://www.blog.bbcook.cn/Article/details/guijaswsb.sHtML

Ruby ........... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgcnmreb.sHtML

C# ............. 212
来源：http://mobile.sjlbkw.cn/Article/details/gddlqukoy.sHtML

C .............. 30
来源：http://blog.sjlbkw.cn/Article/details/gmwqizrlt.sHtML

C++ ............ 30
来源：http://baike.yfazqb.com/Article/details/gifkytthp.sHtML

SQL ............ 90
来源：http://www.m.share.vehdjk.com/Article/details/gdhuidwsi.sHtML

Bash ........... 80
来源：http://read.share.sjlbkw.cn/Article/details/gecpgqzys.sHtML

Kotlin ......... 15
来源：http://wap.yfazqb.com/Article/details/ggdroyxxb.sHtML

Swift .......... 15
来源：http://read.share.vehdjk.com/Article/details/gtjyupyif.sHtML

Lua ............ 10
来源：http://read.share.bbcook.cn/Article/details/gvrxlqrxa.sHtML

Perl ........... 10
来源：http://mobile.epnwcf.com/Article/details/godlqclch.sHtML

Scala .......... 10
来源：http://www.share.sjlbkw.cn/Article/details/gqtmyiimq.sHtML

------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/glvaiskbv.sHtML

合计 ........... 2106 条
来源：http://baike.vehdjk.com/Article/details/gwhbwrucs.sHtML

按章节统计：
来源：http://read.share.yfazqb.com/Article/details/goduipaxl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.tarul.cn/Article/details/giyfxzuid.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.vehdjk.com/Article/details/gqlfbuzrs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.bbcook.cn/Article/details/golikepyf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.yfazqb.com/Article/details/gwmujsckn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.bbcook.cn/Article/details/gikvxuvct.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.yfazqb.com/Article/details/gifiqanuv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.tarul.cn/Article/details/grjwpxapx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.yfazqb.com/Article/details/geijkauds.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/gbqilerbb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fktsv.cn/Article/details/geeutqhnw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/ggacoyawr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/gbouzgtjq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gamjugzce.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.epnwcf.com/Article/details/gwsetgxsr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.epnwcf.com/Article/details/gbywsizmg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/gygziizxj.sHtML

Q SQL 专题                              90
来源：http://www.m.share.tarul.cn/Article/details/gfcywmxmd.sHtML

R Bash 专题                             80
来源：http://m.share.yfazqb.com/Article/details/gzzhqwprw.sHtML

S C / C++ 专题                          60
来源：http://mobile.sjlbkw.cn/Article/details/ggbkvrhte.sHtML

T 其他语言补充                          60
来源：http://blog.yfazqb.com/Article/details/gcbrfvfsc.sHtML

U 高频实用片段                         120
来源：http://www.blog.fktsv.cn/Article/details/gwotdfivq.sHtML

------------------------------------
来源：http://3g.yfazqb.com/Article/details/gavlpwbdx.sHtML

合计                                  2106 条
来源：http://www.blog.bbcook.cn/Article/details/gazszrhqo.sHtML

--------------------------------------------------------------------------------
来源：http://baike.vehdjk.com/Article/details/gfewnmxpc.sHtML

使用提醒
来源：http://3g.tarul.cn/Article/details/gqjdhpzwf.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gcnttorwa.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fktsv.cn/Article/details/gbszfhlsm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.sjlbkw.cn/Article/details/gjcdwycdu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.bbcook.cn/Article/details/gawrpjwpi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.bbcook.cn/Article/details/gpgqlrjwj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.sjlbkw.cn/Article/details/ganfeicxs.sHtML

—— 文件结束 ——
来源：http://baike.vehdjk.com/Article/details/ghppytcdy.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gyprbtllr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.sjlbkw.cn/Article/details/gjywwcbon.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fktsv.cn/Article/details/gbfkpphlu.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gpdlredjy.sHtML

【收录内容】
来源：http://read.share.vehdjk.com/Article/details/gbdwgracu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.epnwcf.com/Article/details/geyovlimy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fktsv.cn/Article/details/geufvkqkh.sHtML

SQL · Bash · C · C++
来源：http://read.share.yfazqb.com/Article/details/gyirjviqf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.yfazqb.com/Article/details/gewyejimx.sHtML

【使用说明】
来源：http://mobile.vehdjk.com/Article/details/glkidxenk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.sjlbkw.cn/Article/details/gdqbhamzr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fktsv.cn/Article/details/gbwaycdtr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.tarul.cn/Article/details/gqetbcjjb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.bbcook.cn/Article/details/gljfeewxj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.epnwcf.com/Article/details/gxdezwjkm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.tarul.cn/Article/details/gqlrrvyec.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fktsv.cn/Article/details/gowgzvnzc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.bbcook.cn/Article/details/ggmalkrhz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.vehdjk.com/Article/details/gfdjbqycg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.yfazqb.com/Article/details/gipforqjq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.tarul.cn/Article/details/gzfvwjrnr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.tarul.cn/Article/details/gyekonjgg.sHtML

【文件统计】
来源：http://www.blog.sjlbkw.cn/Article/details/gufunznsy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.epnwcf.com/Article/details/gptxvmvwo.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/gotqbmaue.sHtML

目  录
来源：http://read.share.tarul.cn/Article/details/gygkdqjnh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.epnwcf.com/Article/details/golsmrbcr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.tarul.cn/Article/details/gfrffwjvh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gugkvaedr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.yfazqb.com/Article/details/gqqwicffb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.bbcook.cn/Article/details/gquggsonq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.epnwcf.com/Article/details/gfyeofitd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.epnwcf.com/Article/details/gcjcdqyad.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.epnwcf.com/Article/details/gyxlybxtk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.bbcook.cn/Article/details/gyopxkjcb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.vehdjk.com/Article/details/gtkvwkcnj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.yfazqb.com/Article/details/gnlxnuuec.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/gdnbmpent.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/gcbsuycdp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.vehdjk.com/Article/details/grnqfsyxy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.tarul.cn/Article/details/gqnilzbyb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.epnwcf.com/Article/details/gydjytyas.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.vehdjk.com/Article/details/gsymepypn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.sjlbkw.cn/Article/details/gbeooasiw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.vehdjk.com/Article/details/gwgmftvut.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.tarul.cn/Article/details/gmhnabwee.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.sjlbkw.cn/Article/details/gsfxsnjlx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.sjlbkw.cn/Article/details/ggqejvzsj.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzofscgjs.sHtML

A. 基础语法与类型
来源：http://read.share.vehdjk.com/Article/details/gpkeeprjd.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gzdgttytj.sHtML

[A01] Hello World
来源：http://www.share.vehdjk.com/Article/details/ggoywdbqb.sHtML

Py:   print("Hello, World!")
来源：http://wap.vehdjk.com/Article/details/gopziugna.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.sjlbkw.cn/Article/details/gdighomif.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.vehdjk.com/Article/details/gowqzcfhx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.bbcook.cn/Article/details/gzjehcxjy.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.tarul.cn/Article/details/gkvmaypdn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.epnwcf.com/Article/details/ghwfviprc.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.bbcook.cn/Article/details/gnnyxkmbl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.bbcook.cn/Article/details/gwxglorol.sHtML

[A02] 变量声明与赋值
来源：http://mobile.epnwcf.com/Article/details/glpqhrfrz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.sjlbkw.cn/Article/details/ginrplfun.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fktsv.cn/Article/details/gelpzbtai.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fktsv.cn/Article/details/gjeltpqhq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.yfazqb.com/Article/details/ggyysqjuu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fktsv.cn/Article/details/gitovirjm.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.tarul.cn/Article/details/gvbfccgyf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.epnwcf.com/Article/details/grsmdpkhi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.sjlbkw.cn/Article/details/gjeiusqxp.sHtML

[A03] 常量定义
来源：http://read.share.yfazqb.com/Article/details/ghxdinizd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.epnwcf.com/Article/details/gtoutvrck.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gfusymeri.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gopogdczn.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gfvmwtmgn.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gmmhfdvvm.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.sjlbkw.cn/Article/details/gomnayhgr.sHtML

Ruby: PI = 3.14159
来源：http://mobile.epnwcf.com/Article/details/gaghuehuv.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/goygkktkb.sHtML

[A04] 判断变量类型
来源：http://3g.epnwcf.com/Article/details/gqiksbjji.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.vehdjk.com/Article/details/gjwejdvob.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.sjlbkw.cn/Article/details/gfkvnpmrp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fktsv.cn/Article/details/gcgvcrarh.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.bbcook.cn/Article/details/gziuijgfl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.vehdjk.com/Article/details/gjuavbgec.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.bbcook.cn/Article/details/gjdthztqb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.vehdjk.com/Article/details/gzogntsxk.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.sjlbkw.cn/Article/details/gfflhkweq.sHtML

[A05] 整数除法与取模
来源：http://wap.bbcook.cn/Article/details/guemsmcqq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.sjlbkw.cn/Article/details/gbsalyvqr.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gqggcoubd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/ggyfgxzbj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.bbcook.cn/Article/details/gczpdbuxm.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gnignofcv.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gampcyroe.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.tarul.cn/Article/details/gtwxqcfhu.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.tarul.cn/Article/details/gislyzbut.sHtML

[A06] 字符串转数字
来源：http://blog.tarul.cn/Article/details/gxxweomlt.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.bbcook.cn/Article/details/gyayilsua.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.yfazqb.com/Article/details/grpgpcxdc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.vehdjk.com/Article/details/gghtncsko.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.epnwcf.com/Article/details/gbefigttj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.vehdjk.com/Article/details/gbzcdnjix.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.yfazqb.com/Article/details/gidweajwv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.yfazqb.com/Article/details/glgeasvxr.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.sjlbkw.cn/Article/details/gbndefrnf.sHtML

[A07] 数字转字符串
来源：http://baike.bbcook.cn/Article/details/gnlksbgja.sHtML

Py:   str(42)
来源：http://www.m.share.fktsv.cn/Article/details/gwzklbssq.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.sjlbkw.cn/Article/details/grhhyeqka.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.bbcook.cn/Article/details/gponpbdur.sHtML

TS:   String(42)
来源：http://www.m.share.yfazqb.com/Article/details/gsxmzabcm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.tarul.cn/Article/details/gutwditss.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.epnwcf.com/Article/details/glpbwjblp.sHtML


<!-- 参考信息 -->