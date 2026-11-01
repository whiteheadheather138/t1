代发 wailian999

[U61] PHP：正则
来源：http://read.share.tarul.cn/Article/details/geqakqgpk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gkiaocgfd.sHtML

[U62] PHP：日期对象
来源：http://www.share.epnwcf.com/Article/details/gobhekwax.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.yfazqb.com/Article/details/gvxfdncsb.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fktsv.cn/Article/details/gqtjzpyhs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.tarul.cn/Article/details/gmzsiefsq.sHtML

[U64] PHP：目录遍历
来源：http://mobile.sjlbkw.cn/Article/details/gojqshiha.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.yfazqb.com/Article/details/ginkzpgso.sHtML

[U65] PHP：会话
来源：http://www.share.vehdjk.com/Article/details/gypjieigp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.yfazqb.com/Article/details/gppestzbd.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.epnwcf.com/Article/details/gumzwskcq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtcbuqvp.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.vehdjk.com/Article/details/gyprhaavu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.vehdjk.com/Article/details/gcdahrdqz.sHtML

[U68] PHP：PDO 连接
来源：http://baike.yfazqb.com/Article/details/gobzrpofi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.sjlbkw.cn/Article/details/gqbxqkkyg.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.sjlbkw.cn/Article/details/gyaslyvla.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.bbcook.cn/Article/details/gkyeweuhp.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fktsv.cn/Article/details/gwkyazcfq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fktsv.cn/Article/details/gzijbsfkr.sHtML

[U71] PHP：抛出异常
来源：http://baike.fktsv.cn/Article/details/gebccsbkt.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxopmvtxa.sHtML

[U72] PHP：写错误日志
来源：http://www.share.sjlbkw.cn/Article/details/gqpwydxpx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.bbcook.cn/Article/details/guwhfwacp.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.sjlbkw.cn/Article/details/gkyietmti.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.yfazqb.com/Article/details/gujcvwqyw.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gakcudsac.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.sjlbkw.cn/Article/details/gynuqbsaw.sHtML

[U75] PHP：依赖注入
来源：http://www.share.yfazqb.com/Article/details/gdgndiakb.sHtML

composer require psr/container
来源：http://3g.sjlbkw.cn/Article/details/gzphdwaaj.sHtML

[U76] PHP：简单路由
来源：http://blog.epnwcf.com/Article/details/gggxebkdr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.vehdjk.com/Article/details/gxpihlylg.sHtML

[U77] PHP：模板渲染
来源：http://wap.epnwcf.com/Article/details/geamrfesm.sHtML

composer require twig/twig
来源：http://www.m.share.epnwcf.com/Article/details/gbnecytfm.sHtML

[U78] PHP：单元测试
来源：http://mobile.fktsv.cn/Article/details/gibrcufxo.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.sjlbkw.cn/Article/details/ghfkumwqx.sHtML

[U79] PHP：静态分析
来源：http://blog.fktsv.cn/Article/details/grvevvmke.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.epnwcf.com/Article/details/geyvqedfi.sHtML

[U80] PHP：代码规范修复
来源：http://3g.vehdjk.com/Article/details/gdqnoyvof.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.sjlbkw.cn/Article/details/gqnjqjpgo.sHtML

[U81] JS：初始化项目
来源：http://www.share.vehdjk.com/Article/details/gytafxvsy.sHtML

npm init -y;  npm i express
来源：http://wap.bbcook.cn/Article/details/ghefpbilg.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.vehdjk.com/Article/details/gocnuunrb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.tarul.cn/Article/details/gfkjpmipp.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fktsv.cn/Article/details/gwmxhztrm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.sjlbkw.cn/Article/details/gomoxwzko.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.tarul.cn/Article/details/gjxsluoez.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.vehdjk.com/Article/details/gjeaiwjmc.sHtML

[U85] JS：可选链
来源：http://wap.fktsv.cn/Article/details/gvayqmxuf.sHtML

a?.b?.c
来源：http://wap.yfazqb.com/Article/details/ghvycfxor.sHtML

[U86] JS：空值合并
来源：http://read.share.yfazqb.com/Article/details/goutotarg.sHtML

a ?? b
来源：http://3g.tarul.cn/Article/details/gcizebthc.sHtML

[U87] JS：解构默认值
来源：http://m.share.fktsv.cn/Article/details/gveesgooa.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.yfazqb.com/Article/details/gmruywmjd.sHtML

[U88] JS：对象展开合并
来源：http://3g.sjlbkw.cn/Article/details/gueajrptc.sHtML

{ ...a, ...b }
来源：http://baike.sjlbkw.cn/Article/details/gbhrlwtlz.sHtML

[U89] JS：数组去重
来源：http://read.share.fktsv.cn/Article/details/giozjypqy.sHtML

[...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/gfguzygns.sHtML

[U90] JS：数字数组排序
来源：http://blog.yfazqb.com/Article/details/gfhtkofal.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/ghteuxfyh.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.tarul.cn/Article/details/glzacvfil.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.bbcook.cn/Article/details/guvapfilr.sHtML

[U92] JS：深拷贝
来源：http://baike.vehdjk.com/Article/details/gqbliowbt.sHtML

structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gffjlnwgo.sHtML

[U93] JS：模板字符串
来源：http://m.share.vehdjk.com/Article/details/gndgrcsfs.sHtML

`共 ${n} 条`
来源：http://wap.sjlbkw.cn/Article/details/gitscpvkx.sHtML

[U94] JS：箭头函数
来源：http://baike.yfazqb.com/Article/details/guvgutlod.sHtML

const double = x => x * 2;
来源：http://mobile.bbcook.cn/Article/details/gurgszrkj.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.epnwcf.com/Article/details/gffijkxbw.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.sjlbkw.cn/Article/details/gaiwwrwmm.sHtML

[U96] JS：async/await 与异常
来源：http://wap.epnwcf.com/Article/details/gcsdbiuaw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/golmrnzom.sHtML

[U97] JS：并发请求
来源：http://www.blog.yfazqb.com/Article/details/gjvmsiync.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gwpftyzbu.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.yfazqb.com/Article/details/gzuvpdigm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.tarul.cn/Article/details/gvptvznwp.sHtML

[U99] JS：事件监听
来源：http://mobile.bbcook.cn/Article/details/gbkkzzdvr.sHtML

el.addEventListener("click", e => {})
来源：http://wap.vehdjk.com/Article/details/gprinpuar.sHtML

[U100] JS：DOM 查询
来源：http://read.share.tarul.cn/Article/details/gmzyhkpyl.sHtML

document.querySelector(".item")
来源：http://www.share.vehdjk.com/Article/details/gttnpeejb.sHtML

[U101] JS：classList 操作
来源：http://mobile.fktsv.cn/Article/details/gfpspivak.sHtML

el.classList.toggle("active")
来源：http://www.share.yfazqb.com/Article/details/gkzsymgeh.sHtML

[U102] JS：本地存储
来源：http://blog.epnwcf.com/Article/details/gyafyekqh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.yfazqb.com/Article/details/gwyhhngqa.sHtML

[U103] JS：定时器
来源：http://baike.sjlbkw.cn/Article/details/gusnoajmj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.bbcook.cn/Article/details/gclfngklc.sHtML

[U104] JS：防抖
来源：http://m.share.vehdjk.com/Article/details/gyyzcqsbb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gssnguzvd.sHtML

[U105] JS：节流
来源：http://wap.yfazqb.com/Article/details/gfvfnfbxr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.tarul.cn/Article/details/gophyzdfd.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.tarul.cn/Article/details/gmiedzvvm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fktsv.cn/Article/details/gbvjmrgsx.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fktsv.cn/Article/details/ghbdrtarj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.sjlbkw.cn/Article/details/gqasgveis.sHtML

[U108] JS：随机整数
来源：http://read.share.epnwcf.com/Article/details/gyrdanwef.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fktsv.cn/Article/details/gqftxrjci.sHtML

[U109] JS：数组分组
来源：http://www.blog.epnwcf.com/Article/details/gffqdbkgm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fktsv.cn/Article/details/gqgwckjrk.sHtML

[U110] JS：数组分块
来源：http://mobile.tarul.cn/Article/details/gztqjgfsq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.vehdjk.com/Article/details/gzrzmcgxs.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fktsv.cn/Article/details/gnblzzief.sHtML

new Map(Object.entries(obj))
来源：http://wap.fktsv.cn/Article/details/glaivsblp.sHtML

[U112] JS：字符串补位
来源：http://wap.tarul.cn/Article/details/geecmknve.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjsemzkf.sHtML

[U113] JS：正则替换全部
来源：http://m.share.tarul.cn/Article/details/gksfkrhmn.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/ggyvalhmw.sHtML

[U114] JS：JSON 深比较
来源：http://baike.sjlbkw.cn/Article/details/gbhfpnsfy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.vehdjk.com/Article/details/gxwyoqztg.sHtML

[U115] JS：生成 UUID
来源：http://baike.sjlbkw.cn/Article/details/gwygokttl.sHtML

crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gahruhpxe.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.epnwcf.com/Article/details/gftbxgmzw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.bbcook.cn/Article/details/gebcquteg.sHtML

[U117] JS：单元测试
来源：http://mobile.tarul.cn/Article/details/gygjefhtq.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.tarul.cn/Article/details/gqgrcsgyt.sHtML

[U118] JS：开发服务器
来源：http://mobile.sjlbkw.cn/Article/details/gpvruvoed.sHtML

npm i -D vite;  npx vite
来源：http://mobile.yfazqb.com/Article/details/gohsmkoex.sHtML

[U119] JS：生产构建
来源：http://m.share.epnwcf.com/Article/details/gywomvncl.sHtML

npx vite build
来源：http://baike.fktsv.cn/Article/details/guvsexlac.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.sjlbkw.cn/Article/details/gikqpvzab.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fktsv.cn/Article/details/gzdjkgxzg.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqhhiuef.sHtML

统计汇总
来源：http://wap.epnwcf.com/Article/details/gaejgyshq.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gkclytobt.sHtML

按语言统计（条）：
来源：http://wap.sjlbkw.cn/Article/details/gxulmhdev.sHtML

Python ......... 252
来源：http://blog.vehdjk.com/Article/details/ggjwdioil.sHtML

PHP ............ 252
来源：http://m.share.epnwcf.com/Article/details/gjuqpeohz.sHtML

JavaScript ..... 252
来源：http://3g.fktsv.cn/Article/details/gskjjgmlh.sHtML

TypeScript ..... 212
来源：http://3g.tarul.cn/Article/details/gxabgihqn.sHtML

Java ........... 212
来源：http://www.blog.yfazqb.com/Article/details/grcdwmnxd.sHtML

Go ............. 212
来源：http://read.share.epnwcf.com/Article/details/gswucinjc.sHtML

Ruby ........... 212
来源：http://www.m.share.vehdjk.com/Article/details/gwyojesdb.sHtML

C# ............. 212
来源：http://mobile.sjlbkw.cn/Article/details/glqudbhcq.sHtML

C .............. 30
来源：http://wap.yfazqb.com/Article/details/gdpqfysvk.sHtML

C++ ............ 30
来源：http://www.blog.yfazqb.com/Article/details/grinjywgy.sHtML

SQL ............ 90
来源：http://www.m.share.tarul.cn/Article/details/gtortsvou.sHtML

Bash ........... 80
来源：http://mobile.yfazqb.com/Article/details/gvqrccsqt.sHtML

Kotlin ......... 15
来源：http://baike.sjlbkw.cn/Article/details/gwdxbbtwp.sHtML

Swift .......... 15
来源：http://www.share.fktsv.cn/Article/details/gtpfywwgz.sHtML

Lua ............ 10
来源：http://blog.fktsv.cn/Article/details/gihzqbifa.sHtML

Perl ........... 10
来源：http://blog.vehdjk.com/Article/details/gsjftycmb.sHtML

Scala .......... 10
来源：http://baike.tarul.cn/Article/details/ghmtznbez.sHtML

------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/ghabufbhv.sHtML

合计 ........... 2106 条
来源：http://blog.fktsv.cn/Article/details/gdrweshsy.sHtML

按章节统计：
来源：http://3g.fktsv.cn/Article/details/glmhongkx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.epnwcf.com/Article/details/gefvmbmvl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/gvvizzhjp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fktsv.cn/Article/details/gtothmjuz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fktsv.cn/Article/details/gigyrdgwv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.bbcook.cn/Article/details/gmhyjboza.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.vehdjk.com/Article/details/gmxqznvys.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.vehdjk.com/Article/details/gkkailaii.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.sjlbkw.cn/Article/details/gnjnqkyjw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gzbplxfwi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgrukhdw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/geqeorrbi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gdbxvcirq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/glxfjtfqb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.tarul.cn/Article/details/ghxkrounl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.yfazqb.com/Article/details/gziclgkzh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/glowzjahb.sHtML

Q SQL 专题                              90
来源：http://www.m.share.epnwcf.com/Article/details/gaeqddfku.sHtML

R Bash 专题                             80
来源：http://read.share.sjlbkw.cn/Article/details/gkivpwfkh.sHtML

S C / C++ 专题                          60
来源：http://mobile.yfazqb.com/Article/details/gjrzkowhs.sHtML

T 其他语言补充                          60
来源：http://mobile.epnwcf.com/Article/details/gdcccnzjs.sHtML

U 高频实用片段                         120
来源：http://mobile.vehdjk.com/Article/details/gldmkrlid.sHtML

------------------------------------
来源：http://mobile.tarul.cn/Article/details/gppgnxgcu.sHtML

合计                                  2106 条
来源：http://3g.sjlbkw.cn/Article/details/glacgailk.sHtML

--------------------------------------------------------------------------------
来源：http://blog.epnwcf.com/Article/details/gkoizakfc.sHtML

使用提醒
来源：http://3g.fktsv.cn/Article/details/gxmsyohas.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gjefdzspt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.bbcook.cn/Article/details/gwkbmkten.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fktsv.cn/Article/details/gdzrwyoql.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.sjlbkw.cn/Article/details/ghjpjyobt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.sjlbkw.cn/Article/details/grwfazuxp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.sjlbkw.cn/Article/details/gmlnbosji.sHtML

—— 文件结束 ——
来源：http://m.share.epnwcf.com/Article/details/gwpbgnhek.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gtcijsdob.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.vehdjk.com/Article/details/gdjmdcjji.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fktsv.cn/Article/details/gljucmgrr.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gmzercjgi.sHtML

【收录内容】
来源：http://www.share.fktsv.cn/Article/details/gwtswwywg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fktsv.cn/Article/details/gguaxpyvw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.epnwcf.com/Article/details/gbqmzxnlw.sHtML

SQL · Bash · C · C++
来源：http://wap.bbcook.cn/Article/details/gjafxejuh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.epnwcf.com/Article/details/gpjvheaqr.sHtML

【使用说明】
来源：http://m.share.fktsv.cn/Article/details/gmcgkxwhe.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.epnwcf.com/Article/details/grzxgnlpy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.yfazqb.com/Article/details/gdoudwkxz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.bbcook.cn/Article/details/guqujrrat.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.epnwcf.com/Article/details/gwyzewkie.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.sjlbkw.cn/Article/details/gdlfqnhht.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.bbcook.cn/Article/details/gfzwskvib.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.bbcook.cn/Article/details/ghtcnkjba.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.epnwcf.com/Article/details/gyvukkdnk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fktsv.cn/Article/details/gddkvnmta.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.vehdjk.com/Article/details/gvcyheokj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.epnwcf.com/Article/details/gjzspbjgp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.vehdjk.com/Article/details/gormnqycp.sHtML

【文件统计】
来源：http://read.share.fktsv.cn/Article/details/gbzamtxqf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.yfazqb.com/Article/details/gvpepgtka.sHtML

--------------------------------------------------------------------------------
来源：http://wap.vehdjk.com/Article/details/gszkkskmb.sHtML

目  录
来源：http://www.m.share.yfazqb.com/Article/details/gdiatalvl.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/gyweznbnl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fktsv.cn/Article/details/glswjyybx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.tarul.cn/Article/details/ghsagnmjy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.bbcook.cn/Article/details/gfcmpzznw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.sjlbkw.cn/Article/details/gdjookief.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.epnwcf.com/Article/details/guaufidlf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.tarul.cn/Article/details/gilorylru.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.vehdjk.com/Article/details/gyghmmgsq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.vehdjk.com/Article/details/gwedbyqtd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/gphtwlxqj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.vehdjk.com/Article/details/gdhqdsdvl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gjybywbsy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.yfazqb.com/Article/details/gqbmbmlrg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/grrzjqnew.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.tarul.cn/Article/details/gzjhvlwms.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fktsv.cn/Article/details/gzokgkodj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgouqauk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.yfazqb.com/Article/details/gikqxjsfp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.vehdjk.com/Article/details/gzwkmavak.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.vehdjk.com/Article/details/gmvbruuqy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.epnwcf.com/Article/details/gnjutgkpv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.bbcook.cn/Article/details/gudsjtpzi.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gzivsvaaa.sHtML

A. 基础语法与类型
来源：http://mobile.bbcook.cn/Article/details/gdytpmymz.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gzupfibny.sHtML

[A01] Hello World
来源：http://read.share.tarul.cn/Article/details/gjeoajfbd.sHtML

Py:   print("Hello, World!")
来源：http://m.share.yfazqb.com/Article/details/gxgvqzcpk.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.yfazqb.com/Article/details/getnpbbjd.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.sjlbkw.cn/Article/details/gziwygspw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fktsv.cn/Article/details/ggwuxufbi.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.sjlbkw.cn/Article/details/ggabwiglx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.yfazqb.com/Article/details/gauacawew.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.tarul.cn/Article/details/ggfjyzewb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.sjlbkw.cn/Article/details/gjrkitlfa.sHtML

[A02] 变量声明与赋值
来源：http://3g.fktsv.cn/Article/details/grzedihyg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.bbcook.cn/Article/details/gyxgwghth.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.sjlbkw.cn/Article/details/gxtfqdzrh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.bbcook.cn/Article/details/grzemwzce.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.sjlbkw.cn/Article/details/gjkoxrysa.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.yfazqb.com/Article/details/gbaioxnti.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fktsv.cn/Article/details/gedapdkfq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.yfazqb.com/Article/details/gwcniaadm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.tarul.cn/Article/details/gaueycjcl.sHtML

[A03] 常量定义
来源：http://m.share.sjlbkw.cn/Article/details/guibyjuzj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.epnwcf.com/Article/details/grhbunaxu.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gklfuhudg.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gniudvdia.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gfpjtrhgf.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gjmqathdv.sHtML

Go:   const PI = 3.14159
来源：http://baike.vehdjk.com/Article/details/ghdujwyet.sHtML

Ruby: PI = 3.14159
来源：http://wap.bbcook.cn/Article/details/gsdjzsbhk.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gzsflsrdf.sHtML

[A04] 判断变量类型
来源：http://3g.yfazqb.com/Article/details/gcxnkbeke.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.yfazqb.com/Article/details/gpkatoetc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.epnwcf.com/Article/details/glcawazef.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.epnwcf.com/Article/details/guyljtojh.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.vehdjk.com/Article/details/gfbccxedp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fktsv.cn/Article/details/gudhpluoq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fktsv.cn/Article/details/gnlcszvmw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.bbcook.cn/Article/details/gcxhsdnaz.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.sjlbkw.cn/Article/details/giacswiyj.sHtML

[A05] 整数除法与取模
来源：http://m.share.sjlbkw.cn/Article/details/gytvbxiwu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.yfazqb.com/Article/details/geofkndqh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.bbcook.cn/Article/details/gsrsjapqi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.bbcook.cn/Article/details/gbqbqfhzq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.sjlbkw.cn/Article/details/gnxsnawkk.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gclgsgntk.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.tarul.cn/Article/details/gqmlvujvw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.epnwcf.com/Article/details/gpeffgigi.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fktsv.cn/Article/details/glkkuuvyp.sHtML

[A06] 字符串转数字
来源：http://wap.bbcook.cn/Article/details/gbdsgilmv.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.epnwcf.com/Article/details/gckjshyws.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.tarul.cn/Article/details/gsibduztq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.yfazqb.com/Article/details/gfvadxomm.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.sjlbkw.cn/Article/details/gkciqindq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.yfazqb.com/Article/details/gylmrmqnr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.tarul.cn/Article/details/gwxsbagzi.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.vehdjk.com/Article/details/gjytxtdcx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.epnwcf.com/Article/details/gphlnfewm.sHtML

[A07] 数字转字符串
来源：http://wap.sjlbkw.cn/Article/details/gwivuikut.sHtML

Py:   str(42)
来源：http://mobile.tarul.cn/Article/details/gxxqemhyl.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.epnwcf.com/Article/details/gieexxmul.sHtML

JS:   String(42); (42).toString()
来源：http://wap.bbcook.cn/Article/details/gxtmountb.sHtML

TS:   String(42)
来源：http://www.blog.tarul.cn/Article/details/gakekxzva.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.bbcook.cn/Article/details/grkvkayeu.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.vehdjk.com/Article/details/gpjoejmwa.sHtML

Ruby: 42.to_s
来源：http://baike.yfazqb.com/Article/details/gjlujxibu.sHtML

C#:   42.ToString()
来源：http://3g.yfazqb.com/Article/details/gudkhbmzb.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.epnwcf.com/Article/details/gsjdqpaoq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.bbcook.cn/Article/details/gcxsxwjqi.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.tarul.cn/Article/details/gjkcaksfk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.yfazqb.com/Article/details/gjxcazukn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.tarul.cn/Article/details/gxmvonqcp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.sjlbkw.cn/Article/details/gqxgtwlkg.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.epnwcf.com/Article/details/gqmodqamu.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.tarul.cn/Article/details/gllrcllhs.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.sjlbkw.cn/Article/details/gyggicjgs.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.tarul.cn/Article/details/grmfapzss.sHtML


<!-- 参考信息 -->