代发 wailian999

[U53] PHP：空合并运算符
来源：http://blog.bbcook.cn/Article/details/gglrniglw.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.epnwcf.com/Article/details/gieohghbb.sHtML

[U54] PHP：空安全调用
来源：http://3g.vehdjk.com/Article/details/gugirztnc.sHtML

$obj?->method()
来源：http://www.m.share.sjlbkw.cn/Article/details/grafqtohj.sHtML

[U55] PHP：match 表达式
来源：http://mobile.sjlbkw.cn/Article/details/ggogokocr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.bbcook.cn/Article/details/gewwgemcl.sHtML

[U56] PHP：命名参数
来源：http://read.share.fktsv.cn/Article/details/gmuycoegj.sHtML

f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gqpnwnpcz.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gasbogvpi.sHtML

"值: {$a}"
来源：http://3g.epnwcf.com/Article/details/gmvlhqgya.sHtML

[U58] PHP：数组三件套
来源：http://read.share.tarul.cn/Article/details/gxcapkeht.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fktsv.cn/Article/details/gagzyiqkt.sHtML

[U59] PHP：自定义排序
来源：http://wap.sjlbkw.cn/Article/details/gcbpaozez.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.epnwcf.com/Article/details/ggugxkfjk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.tarul.cn/Article/details/giodeskxg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.bbcook.cn/Article/details/glnmtoxgd.sHtML

[U61] PHP：正则
来源：http://baike.vehdjk.com/Article/details/gymtkaati.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.epnwcf.com/Article/details/godwcpnxg.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.bbcook.cn/Article/details/gvjrmnsat.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.vehdjk.com/Article/details/guhreabtc.sHtML

[U63] PHP：文件读写
来源：http://read.share.vehdjk.com/Article/details/ghvtidhei.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.yfazqb.com/Article/details/gqpbjcmny.sHtML

[U64] PHP：目录遍历
来源：http://read.share.vehdjk.com/Article/details/gjvqbhtzz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.tarul.cn/Article/details/glnophjbe.sHtML

[U65] PHP：会话
来源：http://m.share.sjlbkw.cn/Article/details/gxujmdsic.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gnyyelmye.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fktsv.cn/Article/details/gifktgnbm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.yfazqb.com/Article/details/gghnwnwgc.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.bbcook.cn/Article/details/gasvfebvf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.bbcook.cn/Article/details/gtqnxbwxt.sHtML

[U68] PHP：PDO 连接
来源：http://blog.bbcook.cn/Article/details/gfcygggfc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.sjlbkw.cn/Article/details/gbbafcowh.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.sjlbkw.cn/Article/details/gbmwuvadl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.bbcook.cn/Article/details/gcsbuyhug.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fktsv.cn/Article/details/giutmpump.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.bbcook.cn/Article/details/ghwunndfb.sHtML

[U71] PHP：抛出异常
来源：http://www.share.sjlbkw.cn/Article/details/gcaowienx.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.yfazqb.com/Article/details/gdjjpihmw.sHtML

[U72] PHP：写错误日志
来源：http://3g.sjlbkw.cn/Article/details/gzouwrnmn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.tarul.cn/Article/details/gqkgyfkzc.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.bbcook.cn/Article/details/gounsvetw.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.epnwcf.com/Article/details/gyprowsdl.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gvmqsujxr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.sjlbkw.cn/Article/details/gwmachyhz.sHtML

[U75] PHP：依赖注入
来源：http://mobile.vehdjk.com/Article/details/goivxzgfs.sHtML

composer require psr/container
来源：http://blog.yfazqb.com/Article/details/gtvojyumg.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.epnwcf.com/Article/details/geccdkyco.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.vehdjk.com/Article/details/gsmdpavvm.sHtML

[U77] PHP：模板渲染
来源：http://3g.sjlbkw.cn/Article/details/gypalsdlk.sHtML

composer require twig/twig
来源：http://wap.tarul.cn/Article/details/gqmymcglo.sHtML

[U78] PHP：单元测试
来源：http://baike.yfazqb.com/Article/details/gsalflftc.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.bbcook.cn/Article/details/gffpcvulh.sHtML

[U79] PHP：静态分析
来源：http://mobile.sjlbkw.cn/Article/details/glokgrbbk.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.sjlbkw.cn/Article/details/gwucvwzhd.sHtML

[U80] PHP：代码规范修复
来源：http://blog.vehdjk.com/Article/details/ginsmohnv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.epnwcf.com/Article/details/gudnrchix.sHtML

[U81] JS：初始化项目
来源：http://3g.yfazqb.com/Article/details/gyyyoavkd.sHtML

npm init -y;  npm i express
来源：http://3g.bbcook.cn/Article/details/ghfzvsgwt.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.vehdjk.com/Article/details/gnuqtwlpc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.sjlbkw.cn/Article/details/gqazuxnbv.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fktsv.cn/Article/details/gmgeognlj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.sjlbkw.cn/Article/details/gbqcxpamj.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.tarul.cn/Article/details/gaqumuthx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.bbcook.cn/Article/details/gvdojmabh.sHtML

[U85] JS：可选链
来源：http://baike.tarul.cn/Article/details/gayzaxlvn.sHtML

a?.b?.c
来源：http://blog.bbcook.cn/Article/details/gbukeceae.sHtML

[U86] JS：空值合并
来源：http://www.share.tarul.cn/Article/details/gmsqhuvkt.sHtML

a ?? b
来源：http://blog.yfazqb.com/Article/details/ghcaapsav.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gtounlwme.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fktsv.cn/Article/details/gevzzvwbw.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.bbcook.cn/Article/details/gnmzdnmfw.sHtML

{ ...a, ...b }
来源：http://baike.bbcook.cn/Article/details/ghifsnpqr.sHtML

[U89] JS：数组去重
来源：http://mobile.yfazqb.com/Article/details/gawwsuqnp.sHtML

[...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gsfevwcdu.sHtML

[U90] JS：数字数组排序
来源：http://m.share.bbcook.cn/Article/details/gyvnwvgyy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/gmrymqpbm.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fktsv.cn/Article/details/gpekzgszs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.sjlbkw.cn/Article/details/ghfbezwxg.sHtML

[U92] JS：深拷贝
来源：http://3g.sjlbkw.cn/Article/details/gzryzpktb.sHtML

structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/gywqjnzwe.sHtML

[U93] JS：模板字符串
来源：http://read.share.yfazqb.com/Article/details/gyozqyanq.sHtML

`共 ${n} 条`
来源：http://www.m.share.yfazqb.com/Article/details/gsljvdsbu.sHtML

[U94] JS：箭头函数
来源：http://www.blog.vehdjk.com/Article/details/gqwdhpzok.sHtML

const double = x => x * 2;
来源：http://wap.tarul.cn/Article/details/ghrftbxzd.sHtML

[U95] JS：Promise 包装
来源：http://baike.tarul.cn/Article/details/gnzusdbkm.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.yfazqb.com/Article/details/gjxmfcdpr.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.yfazqb.com/Article/details/ghtdpnkco.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/guepfaips.sHtML

[U97] JS：并发请求
来源：http://baike.sjlbkw.cn/Article/details/gmpumolws.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/grngutwix.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.epnwcf.com/Article/details/ggydimrsk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.epnwcf.com/Article/details/gyorjyhmh.sHtML

[U99] JS：事件监听
来源：http://www.share.bbcook.cn/Article/details/gehkvwmek.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.tarul.cn/Article/details/gyxehjqog.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.epnwcf.com/Article/details/gtfxqarvf.sHtML

document.querySelector(".item")
来源：http://3g.bbcook.cn/Article/details/gsombkofw.sHtML

[U101] JS：classList 操作
来源：http://baike.epnwcf.com/Article/details/gqadlpjfc.sHtML

el.classList.toggle("active")
来源：http://blog.yfazqb.com/Article/details/ghbquczbu.sHtML

[U102] JS：本地存储
来源：http://3g.sjlbkw.cn/Article/details/ggmxznlti.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.sjlbkw.cn/Article/details/gwpaslfug.sHtML

[U103] JS：定时器
来源：http://3g.yfazqb.com/Article/details/gkecbphll.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.sjlbkw.cn/Article/details/glfeqinwb.sHtML

[U104] JS：防抖
来源：http://blog.tarul.cn/Article/details/gnaphrnmd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/gjbrbvqba.sHtML

[U105] JS：节流
来源：http://wap.tarul.cn/Article/details/guuiwsppr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.sjlbkw.cn/Article/details/giyvozqlr.sHtML

[U106] JS：日期格式化
来源：http://mobile.fktsv.cn/Article/details/gapcdijwo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvwitenb.sHtML

[U107] JS：数字千分位
来源：http://blog.sjlbkw.cn/Article/details/gbqcptplr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fktsv.cn/Article/details/gosdcjjck.sHtML

[U108] JS：随机整数
来源：http://mobile.tarul.cn/Article/details/gyzqpolhy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.epnwcf.com/Article/details/gqhrawotk.sHtML

[U109] JS：数组分组
来源：http://m.share.vehdjk.com/Article/details/ghlooffxx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.bbcook.cn/Article/details/gckoepazu.sHtML

[U110] JS：数组分块
来源：http://baike.tarul.cn/Article/details/gdalypsqc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.epnwcf.com/Article/details/gfsbussfx.sHtML

[U111] JS：对象转 Map
来源：http://blog.epnwcf.com/Article/details/gqnlcporo.sHtML

new Map(Object.entries(obj))
来源：http://3g.yfazqb.com/Article/details/gwajpdnyz.sHtML

[U112] JS：字符串补位
来源：http://wap.bbcook.cn/Article/details/gyncjbffs.sHtML

"7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gjpbvogza.sHtML

[U113] JS：正则替换全部
来源：http://3g.vehdjk.com/Article/details/ggnaifwde.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gerubtzuj.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.sjlbkw.cn/Article/details/gaochueis.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.bbcook.cn/Article/details/gxmyxpemr.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.tarul.cn/Article/details/ggsrezzvo.sHtML

crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/gkjawujad.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.bbcook.cn/Article/details/gzluptmly.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.tarul.cn/Article/details/gohtsdonz.sHtML

[U117] JS：单元测试
来源：http://mobile.bbcook.cn/Article/details/gffysvewo.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.bbcook.cn/Article/details/guhsafxax.sHtML

[U118] JS：开发服务器
来源：http://3g.vehdjk.com/Article/details/gypmxnqck.sHtML

npm i -D vite;  npx vite
来源：http://mobile.yfazqb.com/Article/details/geqafpyog.sHtML

[U119] JS：生产构建
来源：http://www.m.share.tarul.cn/Article/details/gxqbioixr.sHtML

npx vite build
来源：http://www.m.share.yfazqb.com/Article/details/gdttfojuk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.vehdjk.com/Article/details/gpsoiubwj.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.vehdjk.com/Article/details/grfwagqwz.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gbkgorxfb.sHtML

统计汇总
来源：http://blog.vehdjk.com/Article/details/glkkrfxom.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gegswxoam.sHtML

按语言统计（条）：
来源：http://www.m.share.fktsv.cn/Article/details/gspvxqpqa.sHtML

Python ......... 252
来源：http://m.share.sjlbkw.cn/Article/details/ggjqvshvm.sHtML

PHP ............ 252
来源：http://www.m.share.tarul.cn/Article/details/ggzrmqenr.sHtML

JavaScript ..... 252
来源：http://m.share.sjlbkw.cn/Article/details/gscfogjnj.sHtML

TypeScript ..... 212
来源：http://blog.tarul.cn/Article/details/gmndzalix.sHtML

Java ........... 212
来源：http://m.share.fktsv.cn/Article/details/ghewvtbaz.sHtML

Go ............. 212
来源：http://read.share.fktsv.cn/Article/details/gojjebogn.sHtML

Ruby ........... 212
来源：http://m.share.fktsv.cn/Article/details/gczolhjsn.sHtML

C# ............. 212
来源：http://www.m.share.tarul.cn/Article/details/gvcllmkpz.sHtML

C .............. 30
来源：http://blog.fktsv.cn/Article/details/gjfuabkzg.sHtML

C++ ............ 30
来源：http://read.share.vehdjk.com/Article/details/gqjaeubqs.sHtML

SQL ............ 90
来源：http://www.share.fktsv.cn/Article/details/gqaigxnty.sHtML

Bash ........... 80
来源：http://www.share.bbcook.cn/Article/details/guymnhfzf.sHtML

Kotlin ......... 15
来源：http://read.share.bbcook.cn/Article/details/gaapsdukn.sHtML

Swift .......... 15
来源：http://www.m.share.yfazqb.com/Article/details/grozlqync.sHtML

Lua ............ 10
来源：http://www.m.share.epnwcf.com/Article/details/gpmxtkrms.sHtML

Perl ........... 10
来源：http://baike.vehdjk.com/Article/details/gsuyaihmd.sHtML

Scala .......... 10
来源：http://www.blog.yfazqb.com/Article/details/gqihroobq.sHtML

------------------------------------
来源：http://3g.yfazqb.com/Article/details/gaxqwizln.sHtML

合计 ........... 2106 条
来源：http://3g.sjlbkw.cn/Article/details/gzpcwjkcq.sHtML

按章节统计：
来源：http://wap.bbcook.cn/Article/details/glbiexwmb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.epnwcf.com/Article/details/ganhmpsfj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.sjlbkw.cn/Article/details/gkjsnqplk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/goksvlddw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.tarul.cn/Article/details/gbajnuajc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.tarul.cn/Article/details/gcvfufqej.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.bbcook.cn/Article/details/gjthufldi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.bbcook.cn/Article/details/gnoawncin.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.epnwcf.com/Article/details/geulmdybx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/gliknawbl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.epnwcf.com/Article/details/gbqwwfxnk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gvuugvliv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gitqvdksf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/goxrxjbqb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.bbcook.cn/Article/details/gtwlwtfpt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.yfazqb.com/Article/details/gfddizoxg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gbuyemrwh.sHtML

Q SQL 专题                              90
来源：http://m.share.tarul.cn/Article/details/gbyspsehr.sHtML

R Bash 专题                             80
来源：http://read.share.tarul.cn/Article/details/gcdshzrwk.sHtML

S C / C++ 专题                          60
来源：http://www.share.sjlbkw.cn/Article/details/grtgcjddt.sHtML

T 其他语言补充                          60
来源：http://read.share.epnwcf.com/Article/details/gtgtktaqp.sHtML

U 高频实用片段                         120
来源：http://www.m.share.epnwcf.com/Article/details/gcgvngedq.sHtML

------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gkrtlknrk.sHtML

合计                                  2106 条
来源：http://read.share.yfazqb.com/Article/details/gswazthku.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.vehdjk.com/Article/details/ggffptthv.sHtML

使用提醒
来源：http://m.share.fktsv.cn/Article/details/gfcxmrexh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gfjxdleti.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.epnwcf.com/Article/details/gaocfbgtl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.vehdjk.com/Article/details/gzphgxapc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.yfazqb.com/Article/details/godnvjzux.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fktsv.cn/Article/details/gxsqkbbfw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.vehdjk.com/Article/details/gicbtkfdj.sHtML

—— 文件结束 ——
来源：http://wap.yfazqb.com/Article/details/gzfyzbwpw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gtwcipzvs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.epnwcf.com/Article/details/gkncuxlvm.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.epnwcf.com/Article/details/gjkkankyv.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gwzespqcp.sHtML

【收录内容】
来源：http://3g.epnwcf.com/Article/details/gathtkjom.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.epnwcf.com/Article/details/gjrweexnh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.bbcook.cn/Article/details/gbfdxlkld.sHtML

SQL · Bash · C · C++
来源：http://www.blog.tarul.cn/Article/details/gqqctjjty.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.yfazqb.com/Article/details/gmdztuecs.sHtML

【使用说明】
来源：http://www.share.sjlbkw.cn/Article/details/gjflqzkgl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.epnwcf.com/Article/details/gtocnxosv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fktsv.cn/Article/details/gpqzrmxtx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.vehdjk.com/Article/details/gshvejhxr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.vehdjk.com/Article/details/gxfpkbtwj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.tarul.cn/Article/details/gkfmzqfdu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.sjlbkw.cn/Article/details/ggbxzjhan.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.vehdjk.com/Article/details/gynzuompj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.bbcook.cn/Article/details/gzvmacmjy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.yfazqb.com/Article/details/gmqbunxyc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.vehdjk.com/Article/details/gyizvbdnw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.sjlbkw.cn/Article/details/goufqtnhh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.tarul.cn/Article/details/gvbzbffvw.sHtML

【文件统计】
来源：http://blog.vehdjk.com/Article/details/gzrcbtrpf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.epnwcf.com/Article/details/glwuxsvwq.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/grunuwttk.sHtML

目  录
来源：http://www.m.share.fktsv.cn/Article/details/gntdbaucj.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.bbcook.cn/Article/details/ghnrcofwj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.yfazqb.com/Article/details/gyifsftmf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.yfazqb.com/Article/details/gltkyawfd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.bbcook.cn/Article/details/gzjhnkyuu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.yfazqb.com/Article/details/ghnbizego.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.vehdjk.com/Article/details/gfmgygazi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.yfazqb.com/Article/details/giogrhmrx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.tarul.cn/Article/details/gbdpylehm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.vehdjk.com/Article/details/gyfaymfay.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/gpelcubqb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.yfazqb.com/Article/details/gxkzvtfza.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.yfazqb.com/Article/details/glqhppzrx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gyiovfgaz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/gziisrwpg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.sjlbkw.cn/Article/details/gtojqotvz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fktsv.cn/Article/details/gbsjlddeo.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/gbqzprbez.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.bbcook.cn/Article/details/gupnuyehw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.yfazqb.com/Article/details/gimftdzco.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.vehdjk.com/Article/details/gydsxlfej.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fktsv.cn/Article/details/gjzghlhos.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.yfazqb.com/Article/details/gkxegdfre.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gnhkiqhnb.sHtML

A. 基础语法与类型
来源：http://www.m.share.fktsv.cn/Article/details/gidaybfir.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gqbyqpula.sHtML

[A01] Hello World
来源：http://www.share.bbcook.cn/Article/details/gsxtiubep.sHtML

Py:   print("Hello, World!")
来源：http://3g.epnwcf.com/Article/details/gcxngpsbi.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.vehdjk.com/Article/details/gxjnjacjs.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.bbcook.cn/Article/details/gpiquzezi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.epnwcf.com/Article/details/gmfzpxpcw.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.tarul.cn/Article/details/gjzarqimt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.tarul.cn/Article/details/gantwzcfz.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.epnwcf.com/Article/details/glcjopvpr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.yfazqb.com/Article/details/gtkkhjqvy.sHtML

[A02] 变量声明与赋值
来源：http://mobile.tarul.cn/Article/details/gprbtelwo.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.yfazqb.com/Article/details/grcggmhlf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.sjlbkw.cn/Article/details/gfecahzeb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.epnwcf.com/Article/details/ghmmebkxr.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.yfazqb.com/Article/details/gfytgdsgj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.yfazqb.com/Article/details/gkgvdminz.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.vehdjk.com/Article/details/gkvpciynj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.tarul.cn/Article/details/grzxvfvyv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.epnwcf.com/Article/details/gcvhaukrj.sHtML

[A03] 常量定义
来源：http://www.share.tarul.cn/Article/details/gcxfscdru.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.vehdjk.com/Article/details/gtphkdtby.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gtwxrwzpc.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gdgrymflg.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gntdgoruy.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gyuaindsf.sHtML

Go:   const PI = 3.14159
来源：http://blog.fktsv.cn/Article/details/gewkpgiwa.sHtML

Ruby: PI = 3.14159
来源：http://m.share.tarul.cn/Article/details/garypfziy.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gowdgbtez.sHtML

[A04] 判断变量类型
来源：http://read.share.sjlbkw.cn/Article/details/glwtqkkmt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.vehdjk.com/Article/details/gscsfjpmj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.sjlbkw.cn/Article/details/gvwxwnstd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.epnwcf.com/Article/details/gsdaefkia.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.bbcook.cn/Article/details/gnjjmldsz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fktsv.cn/Article/details/glakrgxjo.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.yfazqb.com/Article/details/gurygxtlo.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.epnwcf.com/Article/details/gyxsatawg.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.sjlbkw.cn/Article/details/gvvhznbyf.sHtML

[A05] 整数除法与取模
来源：http://mobile.fktsv.cn/Article/details/gttnbazxm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.bbcook.cn/Article/details/gskbixbcr.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gwihbxdtp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gieobanhr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.bbcook.cn/Article/details/gkkonrgqb.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/gmayetlax.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gjvbsmpbx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.epnwcf.com/Article/details/gkmadddjt.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.bbcook.cn/Article/details/gcmeoeibg.sHtML

[A06] 字符串转数字
来源：http://www.blog.tarul.cn/Article/details/gnacjoean.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.sjlbkw.cn/Article/details/ggyfsczny.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.bbcook.cn/Article/details/gobqeqiwb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzzgfhfn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.sjlbkw.cn/Article/details/grqaszcjb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.bbcook.cn/Article/details/gflxvxkss.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.epnwcf.com/Article/details/gzzgpgfsx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fktsv.cn/Article/details/gsyegpluv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.epnwcf.com/Article/details/gtorgfjzq.sHtML

[A07] 数字转字符串
来源：http://m.share.fktsv.cn/Article/details/gxxbtcioz.sHtML

Py:   str(42)
来源：http://blog.fktsv.cn/Article/details/gocwoilrr.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.epnwcf.com/Article/details/glhcelyjy.sHtML


<!-- 参考信息 -->