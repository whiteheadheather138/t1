代发 wailian999

[U55] PHP：match 表达式
来源：http://www.blog.bbcook.cn/Article/details/ghyztxdpz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.epnwcf.com/Article/details/gooqtjguf.sHtML

[U56] PHP：命名参数
来源：http://read.share.vehdjk.com/Article/details/glmewxkft.sHtML

f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/gnffdexwg.sHtML

[U57] PHP：字符串插值
来源：http://read.share.tarul.cn/Article/details/ggnwqnyui.sHtML

"值: {$a}"
来源：http://wap.bbcook.cn/Article/details/goojiozav.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.yfazqb.com/Article/details/gpnvqanqk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fktsv.cn/Article/details/gmyhdqoyr.sHtML

[U59] PHP：自定义排序
来源：http://baike.vehdjk.com/Article/details/gzlhzvypk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.sjlbkw.cn/Article/details/gsjummaer.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.sjlbkw.cn/Article/details/gaegjijnc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.sjlbkw.cn/Article/details/gezwcnwub.sHtML

[U61] PHP：正则
来源：http://www.share.epnwcf.com/Article/details/gsyekzddy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.yfazqb.com/Article/details/giayyupjo.sHtML

[U62] PHP：日期对象
来源：http://blog.sjlbkw.cn/Article/details/gqfqqyfra.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.vehdjk.com/Article/details/gluwkzgdp.sHtML

[U63] PHP：文件读写
来源：http://m.share.yfazqb.com/Article/details/gmifzhqss.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.epnwcf.com/Article/details/ggvdgzarm.sHtML

[U64] PHP：目录遍历
来源：http://baike.yfazqb.com/Article/details/gxxqinmdi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.tarul.cn/Article/details/gxuunfunf.sHtML

[U65] PHP：会话
来源：http://3g.vehdjk.com/Article/details/gufrezemw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/ggbttsjka.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.vehdjk.com/Article/details/gmexfqzbj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.tarul.cn/Article/details/gfbsqryak.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.sjlbkw.cn/Article/details/gpzvvifla.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.tarul.cn/Article/details/gldzeniso.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.bbcook.cn/Article/details/gcsnwwzdh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.yfazqb.com/Article/details/gushzzcbk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.yfazqb.com/Article/details/gxcwnifkt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.sjlbkw.cn/Article/details/geddimkdr.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.epnwcf.com/Article/details/gkhpjcolk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fktsv.cn/Article/details/gxyncnuyy.sHtML

[U71] PHP：抛出异常
来源：http://baike.epnwcf.com/Article/details/grankinci.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.vehdjk.com/Article/details/gegrkonqg.sHtML

[U72] PHP：写错误日志
来源：http://blog.vehdjk.com/Article/details/gozgujgeq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.tarul.cn/Article/details/gyxkqddad.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.yfazqb.com/Article/details/gdmwtdodq.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.epnwcf.com/Article/details/gxojyltvg.sHtML

[U74] PHP：读取环境变量
来源：http://3g.yfazqb.com/Article/details/gsmkcimze.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.tarul.cn/Article/details/gvjzyvnaa.sHtML

[U75] PHP：依赖注入
来源：http://wap.yfazqb.com/Article/details/govjrktyz.sHtML

composer require psr/container
来源：http://read.share.tarul.cn/Article/details/gmnkwhqjm.sHtML

[U76] PHP：简单路由
来源：http://mobile.epnwcf.com/Article/details/gtdqqobwa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.epnwcf.com/Article/details/gapoqeuph.sHtML

[U77] PHP：模板渲染
来源：http://m.share.vehdjk.com/Article/details/gufhbmtqz.sHtML

composer require twig/twig
来源：http://www.m.share.vehdjk.com/Article/details/gmxpvjnvs.sHtML

[U78] PHP：单元测试
来源：http://baike.yfazqb.com/Article/details/gdqdbmtrs.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.vehdjk.com/Article/details/gpttgknvn.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fktsv.cn/Article/details/gifwciofs.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.vehdjk.com/Article/details/glogryoac.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.vehdjk.com/Article/details/gyuuwyoea.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.vehdjk.com/Article/details/gnehkxtdb.sHtML

[U81] JS：初始化项目
来源：http://blog.yfazqb.com/Article/details/gstnnfmbt.sHtML

npm init -y;  npm i express
来源：http://www.blog.epnwcf.com/Article/details/gcwddrlmh.sHtML

[U82] JS：package.json 脚本
来源：http://blog.bbcook.cn/Article/details/gggfzupns.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.epnwcf.com/Article/details/gophizbiv.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.sjlbkw.cn/Article/details/gdohhfvsg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.sjlbkw.cn/Article/details/gkwqfnozd.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.bbcook.cn/Article/details/gvhztcvdq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.bbcook.cn/Article/details/gpyknjwra.sHtML

[U85] JS：可选链
来源：http://www.blog.yfazqb.com/Article/details/ggwtwiiam.sHtML

a?.b?.c
来源：http://mobile.yfazqb.com/Article/details/gutpcuydz.sHtML

[U86] JS：空值合并
来源：http://www.blog.sjlbkw.cn/Article/details/gbawwiops.sHtML

a ?? b
来源：http://www.m.share.bbcook.cn/Article/details/galmrklzi.sHtML

[U87] JS：解构默认值
来源：http://m.share.fktsv.cn/Article/details/goouflybb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fktsv.cn/Article/details/gjignhndq.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.bbcook.cn/Article/details/gikmfceho.sHtML

{ ...a, ...b }
来源：http://baike.sjlbkw.cn/Article/details/gawvzmjmv.sHtML

[U89] JS：数组去重
来源：http://wap.tarul.cn/Article/details/guwuxlxnu.sHtML

[...new Set(arr)]
来源：http://www.blog.vehdjk.com/Article/details/gdxlutcbx.sHtML

[U90] JS：数字数组排序
来源：http://m.share.tarul.cn/Article/details/gzbeuunzy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gdkouugqe.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fktsv.cn/Article/details/gwlcyirol.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.vehdjk.com/Article/details/gyjsbbpgf.sHtML

[U92] JS：深拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/ghvvzzurq.sHtML

structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gdcybiuxl.sHtML

[U93] JS：模板字符串
来源：http://wap.tarul.cn/Article/details/gtjvrjreg.sHtML

`共 ${n} 条`
来源：http://3g.bbcook.cn/Article/details/gbjzgsvfh.sHtML

[U94] JS：箭头函数
来源：http://wap.fktsv.cn/Article/details/gtndlxfis.sHtML

const double = x => x * 2;
来源：http://wap.tarul.cn/Article/details/gpusvmokb.sHtML

[U95] JS：Promise 包装
来源：http://wap.fktsv.cn/Article/details/gtkcayqky.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.epnwcf.com/Article/details/gdskcdcyn.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.tarul.cn/Article/details/gwltzsrpr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.vehdjk.com/Article/details/gfsyzsqzh.sHtML

[U97] JS：并发请求
来源：http://blog.tarul.cn/Article/details/gikmjymdf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gvtggwllo.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.bbcook.cn/Article/details/gjgkrdwpg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.yfazqb.com/Article/details/gjtezcakg.sHtML

[U99] JS：事件监听
来源：http://baike.vehdjk.com/Article/details/gyezqrezc.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.vehdjk.com/Article/details/gansnsmpt.sHtML

[U100] JS：DOM 查询
来源：http://blog.vehdjk.com/Article/details/gyvqtwant.sHtML

document.querySelector(".item")
来源：http://www.share.yfazqb.com/Article/details/ghfpslndu.sHtML

[U101] JS：classList 操作
来源：http://read.share.fktsv.cn/Article/details/glemsquna.sHtML

el.classList.toggle("active")
来源：http://www.share.tarul.cn/Article/details/gwbfjmokr.sHtML

[U102] JS：本地存储
来源：http://read.share.bbcook.cn/Article/details/gbydrerin.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.vehdjk.com/Article/details/gmvduzndl.sHtML

[U103] JS：定时器
来源：http://www.blog.sjlbkw.cn/Article/details/grcjbxctt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.bbcook.cn/Article/details/gpvouuvqx.sHtML

[U104] JS：防抖
来源：http://3g.sjlbkw.cn/Article/details/geszxpnjc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/gobohernm.sHtML

[U105] JS：节流
来源：http://3g.yfazqb.com/Article/details/gciytfxso.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fktsv.cn/Article/details/gqoobyfhh.sHtML

[U106] JS：日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gpekknqnj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.yfazqb.com/Article/details/gcigltnuz.sHtML

[U107] JS：数字千分位
来源：http://baike.bbcook.cn/Article/details/gevrkykwc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.sjlbkw.cn/Article/details/gxmpvfwls.sHtML

[U108] JS：随机整数
来源：http://www.share.vehdjk.com/Article/details/gswsgbchl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.sjlbkw.cn/Article/details/gymraurfs.sHtML

[U109] JS：数组分组
来源：http://baike.tarul.cn/Article/details/ggvilluyg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.tarul.cn/Article/details/ghhqfhfkt.sHtML

[U110] JS：数组分块
来源：http://www.blog.sjlbkw.cn/Article/details/gbqbchrcv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.tarul.cn/Article/details/guvghggma.sHtML

[U111] JS：对象转 Map
来源：http://3g.epnwcf.com/Article/details/gdcgfgjbf.sHtML

new Map(Object.entries(obj))
来源：http://3g.epnwcf.com/Article/details/gmnqvpeba.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.epnwcf.com/Article/details/ghfmwwziw.sHtML

"7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gfsqssbsc.sHtML

[U113] JS：正则替换全部
来源：http://m.share.tarul.cn/Article/details/gexffdfcz.sHtML

s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gzaxcjesd.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.yfazqb.com/Article/details/gdcpqunuq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.sjlbkw.cn/Article/details/gykdxcyid.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fktsv.cn/Article/details/geytimnpy.sHtML

crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gouqtbqfx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.tarul.cn/Article/details/gjkabktnw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.vehdjk.com/Article/details/gxshycjig.sHtML

[U117] JS：单元测试
来源：http://blog.yfazqb.com/Article/details/grokiiwfk.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fktsv.cn/Article/details/gbjsmwzka.sHtML

[U118] JS：开发服务器
来源：http://m.share.bbcook.cn/Article/details/gzxyqmkoc.sHtML

npm i -D vite;  npx vite
来源：http://3g.vehdjk.com/Article/details/gxwnrofxv.sHtML

[U119] JS：生产构建
来源：http://wap.fktsv.cn/Article/details/glkatahmt.sHtML

npx vite build
来源：http://read.share.fktsv.cn/Article/details/gwvffjutd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.vehdjk.com/Article/details/gorsbmxyq.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.vehdjk.com/Article/details/gbazdyhkl.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gqubaftav.sHtML

统计汇总
来源：http://m.share.fktsv.cn/Article/details/gguhsobjn.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/grjjsekpb.sHtML

按语言统计（条）：
来源：http://www.m.share.tarul.cn/Article/details/gbghsjmti.sHtML

Python ......... 252
来源：http://www.share.fktsv.cn/Article/details/gpkjkzllo.sHtML

PHP ............ 252
来源：http://www.blog.vehdjk.com/Article/details/garqsoxub.sHtML

JavaScript ..... 252
来源：http://baike.vehdjk.com/Article/details/gnsejwjed.sHtML

TypeScript ..... 212
来源：http://www.m.share.epnwcf.com/Article/details/gljfafsqp.sHtML

Java ........... 212
来源：http://wap.fktsv.cn/Article/details/gquixndaj.sHtML

Go ............. 212
来源：http://m.share.tarul.cn/Article/details/gxidsqeia.sHtML

Ruby ........... 212
来源：http://m.share.fktsv.cn/Article/details/ghjlqdmqo.sHtML

C# ............. 212
来源：http://read.share.bbcook.cn/Article/details/ghgfefjbe.sHtML

C .............. 30
来源：http://wap.fktsv.cn/Article/details/gaawfkpgs.sHtML

C++ ............ 30
来源：http://read.share.vehdjk.com/Article/details/gvagbwxik.sHtML

SQL ............ 90
来源：http://www.blog.yfazqb.com/Article/details/gpmlsxdpo.sHtML

Bash ........... 80
来源：http://read.share.bbcook.cn/Article/details/gyyjhqumk.sHtML

Kotlin ......... 15
来源：http://www.share.yfazqb.com/Article/details/gtxhzqdjp.sHtML

Swift .......... 15
来源：http://3g.bbcook.cn/Article/details/gjefwgsen.sHtML

Lua ............ 10
来源：http://read.share.sjlbkw.cn/Article/details/gwsyigxeh.sHtML

Perl ........... 10
来源：http://read.share.epnwcf.com/Article/details/ggvfabqgl.sHtML

Scala .......... 10
来源：http://read.share.fktsv.cn/Article/details/gxzpvzboj.sHtML

------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gmwsgdzst.sHtML

合计 ........... 2106 条
来源：http://3g.tarul.cn/Article/details/giqlvvrcx.sHtML

按章节统计：
来源：http://www.m.share.epnwcf.com/Article/details/gajtphmsf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fktsv.cn/Article/details/gdyirkfrp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.epnwcf.com/Article/details/ggpxffgye.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.bbcook.cn/Article/details/gqsqsozdc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fktsv.cn/Article/details/gbocapmje.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.yfazqb.com/Article/details/gikrknsxl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.yfazqb.com/Article/details/gdiztynph.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.yfazqb.com/Article/details/goqwgufnc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.tarul.cn/Article/details/gdnxxxheo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gopxmpuje.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.sjlbkw.cn/Article/details/ghbpfjiry.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/ghjmtaxoh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gykdsczho.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gobuyfsbp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.epnwcf.com/Article/details/gpadfxncq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.yfazqb.com/Article/details/gndcbvghd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/goshfjmbm.sHtML

Q SQL 专题                              90
来源：http://blog.fktsv.cn/Article/details/gtmqizuvz.sHtML

R Bash 专题                             80
来源：http://baike.fktsv.cn/Article/details/gapaupfcj.sHtML

S C / C++ 专题                          60
来源：http://www.share.epnwcf.com/Article/details/gxckchajr.sHtML

T 其他语言补充                          60
来源：http://mobile.fktsv.cn/Article/details/grckzcnjp.sHtML

U 高频实用片段                         120
来源：http://3g.yfazqb.com/Article/details/gyaxrpwwf.sHtML

------------------------------------
来源：http://baike.fktsv.cn/Article/details/gsgmfsmiv.sHtML

合计                                  2106 条
来源：http://www.share.tarul.cn/Article/details/glmuijnnr.sHtML

--------------------------------------------------------------------------------
来源：http://blog.bbcook.cn/Article/details/gqzidtrmz.sHtML

使用提醒
来源：http://www.m.share.tarul.cn/Article/details/gxfkktuuh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.epnwcf.com/Article/details/grajfazip.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.bbcook.cn/Article/details/ggwkffcyx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.sjlbkw.cn/Article/details/gesiecosz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fktsv.cn/Article/details/glcynuwoc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fktsv.cn/Article/details/ghtmlxczu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.tarul.cn/Article/details/guupulypo.sHtML

—— 文件结束 ——
来源：http://www.share.sjlbkw.cn/Article/details/gdofbuxqt.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gtzxmloeb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.vehdjk.com/Article/details/geeygfszg.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fktsv.cn/Article/details/geezvmkgh.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gtpypwtxi.sHtML

【收录内容】
来源：http://read.share.vehdjk.com/Article/details/gdnmwkwhx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.vehdjk.com/Article/details/gkkbxsvhc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.yfazqb.com/Article/details/gythirczh.sHtML

SQL · Bash · C · C++
来源：http://blog.yfazqb.com/Article/details/gkelzdtrb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.bbcook.cn/Article/details/gtlpelwfc.sHtML

【使用说明】
来源：http://baike.fktsv.cn/Article/details/gazwdbogo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.tarul.cn/Article/details/gtucvcbzr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.yfazqb.com/Article/details/gcmdcsjlg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.sjlbkw.cn/Article/details/ghbaqbnvs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.sjlbkw.cn/Article/details/gyrbxhpdn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.tarul.cn/Article/details/gsaczqzpt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.sjlbkw.cn/Article/details/gkaonqsnm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.bbcook.cn/Article/details/ghpodnmkk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.bbcook.cn/Article/details/gsmhquogw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.yfazqb.com/Article/details/goegqvfck.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.vehdjk.com/Article/details/gnwcgskrn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.sjlbkw.cn/Article/details/gatjgmwtq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.yfazqb.com/Article/details/gyabaxiaa.sHtML

【文件统计】
来源：http://blog.bbcook.cn/Article/details/gvtfwmhsp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fktsv.cn/Article/details/gwktpajkz.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gmwiuszue.sHtML

目  录
来源：http://blog.tarul.cn/Article/details/gyuwvvwjl.sHtML

--------------------------------------------------------------------------------
来源：http://baike.bbcook.cn/Article/details/ggxzmgxfx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.epnwcf.com/Article/details/gkogevdcu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.sjlbkw.cn/Article/details/grlqvziji.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fktsv.cn/Article/details/gstpraeay.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.bbcook.cn/Article/details/gofwfwfur.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.bbcook.cn/Article/details/guflbnrxd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.tarul.cn/Article/details/gcyoujemc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.yfazqb.com/Article/details/gwzhubdhz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.tarul.cn/Article/details/glwlenozd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gvfaotuns.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.epnwcf.com/Article/details/gcezcfjpk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/grbfnkeuq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/gyqnumwkl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.yfazqb.com/Article/details/geiqdvbvb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.epnwcf.com/Article/details/gownmosxc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.vehdjk.com/Article/details/ghcddjfmq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.sjlbkw.cn/Article/details/gcrctgbtl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fktsv.cn/Article/details/gvckzpizy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.tarul.cn/Article/details/gfnrroxmp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.vehdjk.com/Article/details/gvuzfbczk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fktsv.cn/Article/details/gyeyowauv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.sjlbkw.cn/Article/details/gszemapud.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gkrgaxqme.sHtML

A. 基础语法与类型
来源：http://baike.bbcook.cn/Article/details/gxysxtone.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gjogopkie.sHtML

[A01] Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gcefbsfjm.sHtML

Py:   print("Hello, World!")
来源：http://mobile.sjlbkw.cn/Article/details/gvqgoyhyn.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.epnwcf.com/Article/details/gyzyaglmu.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.yfazqb.com/Article/details/gmsbpdtnu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fktsv.cn/Article/details/glefpnred.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.tarul.cn/Article/details/gmwsipgxd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.sjlbkw.cn/Article/details/gpzdahdqz.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.vehdjk.com/Article/details/ggbsaawti.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.bbcook.cn/Article/details/gjroucvkd.sHtML

[A02] 变量声明与赋值
来源：http://wap.tarul.cn/Article/details/glsyqbguw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.tarul.cn/Article/details/gvophiigy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.sjlbkw.cn/Article/details/geeuxrlvi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.sjlbkw.cn/Article/details/gbdbbmrvt.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fktsv.cn/Article/details/gclkkevka.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.tarul.cn/Article/details/gzqbsoups.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fktsv.cn/Article/details/gudbmfeic.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.vehdjk.com/Article/details/gzuvosdxu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.sjlbkw.cn/Article/details/gwltidchq.sHtML

[A03] 常量定义
来源：http://3g.fktsv.cn/Article/details/gltgtjtxw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.bbcook.cn/Article/details/gomcglfxx.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gqbversbn.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gxswonppi.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gbtjzfecz.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gbusvxklh.sHtML

Go:   const PI = 3.14159
来源：http://www.share.yfazqb.com/Article/details/gvghruoai.sHtML

Ruby: PI = 3.14159
来源：http://baike.vehdjk.com/Article/details/ghgpklwle.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gnnadtkzf.sHtML

[A04] 判断变量类型
来源：http://wap.epnwcf.com/Article/details/gjbeendpk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fktsv.cn/Article/details/gcnxrfejw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.tarul.cn/Article/details/gikvopind.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.vehdjk.com/Article/details/gydyjkkdg.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.bbcook.cn/Article/details/gcjbdjuqp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.bbcook.cn/Article/details/gushixyyb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.vehdjk.com/Article/details/gwxubqdgi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.epnwcf.com/Article/details/ghnehxtiv.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.tarul.cn/Article/details/gpbaclext.sHtML

[A05] 整数除法与取模
来源：http://www.blog.sjlbkw.cn/Article/details/gpdxgjuqv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.yfazqb.com/Article/details/ghgicgfrq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.vehdjk.com/Article/details/gmeqbouth.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gktpmxrxo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.tarul.cn/Article/details/gwevxpnjr.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gvxuzrlej.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/gieuzvztf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gpuchdhzd.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.yfazqb.com/Article/details/guttekegt.sHtML

[A06] 字符串转数字
来源：http://mobile.fktsv.cn/Article/details/gjxsiytwl.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.vehdjk.com/Article/details/geskihkxu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fktsv.cn/Article/details/gktxmipex.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.yfazqb.com/Article/details/gygfqmkpl.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.tarul.cn/Article/details/gojpnpxex.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.bbcook.cn/Article/details/gkpyggept.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.tarul.cn/Article/details/gcrobcwpc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsxtntnh.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.tarul.cn/Article/details/gixarduqa.sHtML

[A07] 数字转字符串
来源：http://www.m.share.tarul.cn/Article/details/gigrgtowq.sHtML

Py:   str(42)
来源：http://mobile.fktsv.cn/Article/details/gezpgzzhl.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.sjlbkw.cn/Article/details/goyshxgfw.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.bbcook.cn/Article/details/gzbzwnkuy.sHtML

TS:   String(42)
来源：http://3g.bbcook.cn/Article/details/grbkskisl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fktsv.cn/Article/details/gkyfntanc.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.tarul.cn/Article/details/gpigtwsbw.sHtML


<!-- 参考信息 -->