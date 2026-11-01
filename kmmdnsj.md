代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.share.epnwcf.com/Article/details/gtthxkujg.sHtML

namespace App\Http;
来源：http://baike.fktsv.cn/Article/details/gtpefamwy.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.epnwcf.com/Article/details/ghvkvrqoq.sHtML

declare(strict_types=1);
来源：http://blog.fktsv.cn/Article/details/gtqsklzpo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fktsv.cn/Article/details/geqwtdqww.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/ggkwctkid.sHtML

[U46] PHP：可空类型
来源：http://baike.yfazqb.com/Article/details/gqshshswy.sHtML

?string $name = null
来源：http://wap.tarul.cn/Article/details/gsqgaokzq.sHtML

[U47] PHP：联合类型
来源：http://baike.bbcook.cn/Article/details/gpynnuegr.sHtML

int|string $id
来源：http://mobile.sjlbkw.cn/Article/details/gujoovgqt.sHtML

[U48] PHP：纯枚举
来源：http://3g.bbcook.cn/Article/details/glbxtovkx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.tarul.cn/Article/details/gztettxql.sHtML

[U49] PHP：只读属性
来源：http://blog.yfazqb.com/Article/details/gaoesugxe.sHtML

public readonly string $name
来源：http://www.blog.yfazqb.com/Article/details/ghuzdjrul.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.sjlbkw.cn/Article/details/gcjoidzim.sHtML

public function __construct(private int $id) {}
来源：http://read.share.bbcook.cn/Article/details/gzprzihbg.sHtML

[U51] PHP：数组解构
来源：http://3g.tarul.cn/Article/details/gmgsgjptu.sHtML

[$a, $b] = $arr;
来源：http://mobile.fktsv.cn/Article/details/gmhkuhita.sHtML

[U52] PHP：箭头函数
来源：http://blog.yfazqb.com/Article/details/gsgcsmtbh.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.yfazqb.com/Article/details/gxmbwcczg.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.vehdjk.com/Article/details/gualdxdiy.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.sjlbkw.cn/Article/details/gdojjykqb.sHtML

[U54] PHP：空安全调用
来源：http://baike.vehdjk.com/Article/details/gtsjetyip.sHtML

$obj?->method()
来源：http://www.m.share.yfazqb.com/Article/details/gdpvszuao.sHtML

[U55] PHP：match 表达式
来源：http://blog.fktsv.cn/Article/details/gzjrmrzpo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.tarul.cn/Article/details/gnnuhqtuv.sHtML

[U56] PHP：命名参数
来源：http://read.share.fktsv.cn/Article/details/ghucwoywf.sHtML

f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gqotxyfmx.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/grjcurxjc.sHtML

"值: {$a}"
来源：http://www.share.sjlbkw.cn/Article/details/gbmvjngrv.sHtML

[U58] PHP：数组三件套
来源：http://3g.bbcook.cn/Article/details/gocfbsqzw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.bbcook.cn/Article/details/gfvpdtzam.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fktsv.cn/Article/details/gfcdktspe.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.vehdjk.com/Article/details/gwavgjdjq.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.sjlbkw.cn/Article/details/goidhhhwo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fktsv.cn/Article/details/gupiipgiy.sHtML

[U61] PHP：正则
来源：http://www.share.bbcook.cn/Article/details/gqmiqurft.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.epnwcf.com/Article/details/geqjcdasr.sHtML

[U62] PHP：日期对象
来源：http://wap.yfazqb.com/Article/details/gqfknyucx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.yfazqb.com/Article/details/gztalrnkr.sHtML

[U63] PHP：文件读写
来源：http://m.share.tarul.cn/Article/details/gjnxminfo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.yfazqb.com/Article/details/gvqodwtqu.sHtML

[U64] PHP：目录遍历
来源：http://m.share.yfazqb.com/Article/details/gekeatrev.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.vehdjk.com/Article/details/gfnbfmori.sHtML

[U65] PHP：会话
来源：http://m.share.fktsv.cn/Article/details/gjtkfgtuu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.tarul.cn/Article/details/gqgubbgia.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.vehdjk.com/Article/details/glgnzkjhq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqianogs.sHtML

[U67] PHP：处理文件上传
来源：http://baike.epnwcf.com/Article/details/gnhxgjxur.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.sjlbkw.cn/Article/details/gitlrqglk.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.epnwcf.com/Article/details/gbxygqcnw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.sjlbkw.cn/Article/details/gsykrzlpo.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fktsv.cn/Article/details/gpucgdnsd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.bbcook.cn/Article/details/glhdfnwxw.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.tarul.cn/Article/details/gvavpvknr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.sjlbkw.cn/Article/details/gnwditcmx.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.bbcook.cn/Article/details/gvtljfgog.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.epnwcf.com/Article/details/gjcwukatz.sHtML

[U72] PHP：写错误日志
来源：http://m.share.tarul.cn/Article/details/gfjoofqdq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.yfazqb.com/Article/details/ghrtuzudj.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.tarul.cn/Article/details/gszuncrql.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.epnwcf.com/Article/details/gwgczaxye.sHtML

[U74] PHP：读取环境变量
来源：http://blog.bbcook.cn/Article/details/gmqsbmmpo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.epnwcf.com/Article/details/gphpoffwz.sHtML

[U75] PHP：依赖注入
来源：http://m.share.bbcook.cn/Article/details/gilrxkoum.sHtML

composer require psr/container
来源：http://blog.tarul.cn/Article/details/gvllagecz.sHtML

[U76] PHP：简单路由
来源：http://www.blog.bbcook.cn/Article/details/gdhsxruci.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.yfazqb.com/Article/details/gedzkrrrh.sHtML

[U77] PHP：模板渲染
来源：http://mobile.sjlbkw.cn/Article/details/gggndqmmg.sHtML

composer require twig/twig
来源：http://blog.epnwcf.com/Article/details/gwtimrfgl.sHtML

[U78] PHP：单元测试
来源：http://blog.bbcook.cn/Article/details/gxqyynupt.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.yfazqb.com/Article/details/gkunoivzs.sHtML

[U79] PHP：静态分析
来源：http://blog.vehdjk.com/Article/details/gslswfbry.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.tarul.cn/Article/details/gqisduofc.sHtML

[U80] PHP：代码规范修复
来源：http://3g.epnwcf.com/Article/details/geaiclxfj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.bbcook.cn/Article/details/gcqhnelay.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.yfazqb.com/Article/details/gyjdwfkqo.sHtML

npm init -y;  npm i express
来源：http://3g.bbcook.cn/Article/details/gcszhfghj.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.sjlbkw.cn/Article/details/gsphipsze.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.epnwcf.com/Article/details/gvwvmypcw.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.yfazqb.com/Article/details/gtpesbtep.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.tarul.cn/Article/details/gauowmatr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.yfazqb.com/Article/details/gjeekguko.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.tarul.cn/Article/details/gkuaovgtj.sHtML

[U85] JS：可选链
来源：http://read.share.tarul.cn/Article/details/gspiadwsv.sHtML

a?.b?.c
来源：http://www.m.share.epnwcf.com/Article/details/gwhuxfzew.sHtML

[U86] JS：空值合并
来源：http://www.m.share.yfazqb.com/Article/details/gtmuenwxh.sHtML

a ?? b
来源：http://www.m.share.epnwcf.com/Article/details/gqcfremjr.sHtML

[U87] JS：解构默认值
来源：http://m.share.epnwcf.com/Article/details/gccdtjott.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.bbcook.cn/Article/details/gdvskbklf.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.tarul.cn/Article/details/ggpdrytsz.sHtML

{ ...a, ...b }
来源：http://www.m.share.fktsv.cn/Article/details/gqzvlazva.sHtML

[U89] JS：数组去重
来源：http://mobile.bbcook.cn/Article/details/gtueljzfg.sHtML

[...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gglbqcvhm.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fktsv.cn/Article/details/gvjmnqrvv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/gztqnoqxe.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.yfazqb.com/Article/details/gsozqlbii.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.yfazqb.com/Article/details/gghomnlow.sHtML

[U92] JS：深拷贝
来源：http://www.share.vehdjk.com/Article/details/gfsnimuoh.sHtML

structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/gslxadqdo.sHtML

[U93] JS：模板字符串
来源：http://mobile.fktsv.cn/Article/details/gyyhossvg.sHtML

`共 ${n} 条`
来源：http://baike.yfazqb.com/Article/details/gkcmewssc.sHtML

[U94] JS：箭头函数
来源：http://baike.bbcook.cn/Article/details/gnsayexeu.sHtML

const double = x => x * 2;
来源：http://wap.vehdjk.com/Article/details/geqonayih.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.sjlbkw.cn/Article/details/grfashqfj.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.bbcook.cn/Article/details/gcirtkxok.sHtML

[U96] JS：async/await 与异常
来源：http://3g.epnwcf.com/Article/details/gegrbcdyk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/grudkfamz.sHtML

[U97] JS：并发请求
来源：http://read.share.yfazqb.com/Article/details/gzjcxuthj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/gypkmsojp.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.yfazqb.com/Article/details/gpcxginun.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fktsv.cn/Article/details/ghslditrz.sHtML

[U99] JS：事件监听
来源：http://www.share.vehdjk.com/Article/details/gtnprcpkm.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.vehdjk.com/Article/details/goexwdadn.sHtML

[U100] JS：DOM 查询
来源：http://mobile.vehdjk.com/Article/details/goxyargug.sHtML

document.querySelector(".item")
来源：http://www.share.vehdjk.com/Article/details/gypitnssy.sHtML

[U101] JS：classList 操作
来源：http://read.share.vehdjk.com/Article/details/gysvijzdv.sHtML

el.classList.toggle("active")
来源：http://www.m.share.tarul.cn/Article/details/godyvbaeu.sHtML

[U102] JS：本地存储
来源：http://3g.bbcook.cn/Article/details/gdyswigeb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.yfazqb.com/Article/details/gitbgktyk.sHtML

[U103] JS：定时器
来源：http://mobile.fktsv.cn/Article/details/gbgfwbrie.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fktsv.cn/Article/details/glmhefokd.sHtML

[U104] JS：防抖
来源：http://wap.bbcook.cn/Article/details/gawyxcmyz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gzynzcvjm.sHtML

[U105] JS：节流
来源：http://m.share.bbcook.cn/Article/details/gacickwei.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.bbcook.cn/Article/details/gfhfmcjbt.sHtML

[U106] JS：日期格式化
来源：http://www.blog.bbcook.cn/Article/details/ghtbhnkpq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.epnwcf.com/Article/details/gzdgpwzth.sHtML

[U107] JS：数字千分位
来源：http://www.share.tarul.cn/Article/details/grxdsucgv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.yfazqb.com/Article/details/gyronhgkx.sHtML

[U108] JS：随机整数
来源：http://www.share.epnwcf.com/Article/details/ggqlytyks.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.sjlbkw.cn/Article/details/gtcihjilr.sHtML

[U109] JS：数组分组
来源：http://mobile.epnwcf.com/Article/details/gpemhqysy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.epnwcf.com/Article/details/gxpnhlgaf.sHtML

[U110] JS：数组分块
来源：http://blog.bbcook.cn/Article/details/gculeptoh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.tarul.cn/Article/details/gnnoppwgv.sHtML

[U111] JS：对象转 Map
来源：http://wap.sjlbkw.cn/Article/details/ghkrwghsj.sHtML

new Map(Object.entries(obj))
来源：http://wap.bbcook.cn/Article/details/gphvbiidj.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.vehdjk.com/Article/details/goykhcqfq.sHtML

"7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gllqyylvf.sHtML

[U113] JS：正则替换全部
来源：http://read.share.bbcook.cn/Article/details/ghebhjphs.sHtML

s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/ghlkpcrlf.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.tarul.cn/Article/details/getpxacfh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.sjlbkw.cn/Article/details/gsnfifcan.sHtML

[U115] JS：生成 UUID
来源：http://baike.tarul.cn/Article/details/giunmsnnd.sHtML

crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/gedyzfzaa.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.yfazqb.com/Article/details/ggfjnvnhd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.bbcook.cn/Article/details/ghfqeeypt.sHtML

[U117] JS：单元测试
来源：http://wap.fktsv.cn/Article/details/gorwbmjfb.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.epnwcf.com/Article/details/gsggdlcpe.sHtML

[U118] JS：开发服务器
来源：http://baike.bbcook.cn/Article/details/grxvrofnr.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fktsv.cn/Article/details/ggoorvqvd.sHtML

[U119] JS：生产构建
来源：http://3g.fktsv.cn/Article/details/gmxhzurrn.sHtML

npx vite build
来源：http://www.blog.fktsv.cn/Article/details/gidjgnlbt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fktsv.cn/Article/details/gesovtcts.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.epnwcf.com/Article/details/gejwqznoc.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gofsulyep.sHtML

统计汇总
来源：http://m.share.bbcook.cn/Article/details/gxzpbewyt.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gsqpmfobb.sHtML

按语言统计（条）：
来源：http://read.share.fktsv.cn/Article/details/gpxuhfzyv.sHtML

Python ......... 252
来源：http://m.share.fktsv.cn/Article/details/gboxosscu.sHtML

PHP ............ 252
来源：http://3g.vehdjk.com/Article/details/gueshrxlz.sHtML

JavaScript ..... 252
来源：http://mobile.vehdjk.com/Article/details/groqgolar.sHtML

TypeScript ..... 212
来源：http://www.m.share.yfazqb.com/Article/details/gsfxjwube.sHtML

Java ........... 212
来源：http://3g.vehdjk.com/Article/details/gnfzlpzyw.sHtML

Go ............. 212
来源：http://www.m.share.tarul.cn/Article/details/gvetbrhxp.sHtML

Ruby ........... 212
来源：http://blog.vehdjk.com/Article/details/gqmsxirqu.sHtML

C# ............. 212
来源：http://www.blog.fktsv.cn/Article/details/gksgjnjjc.sHtML

C .............. 30
来源：http://baike.bbcook.cn/Article/details/gtcydudva.sHtML

C++ ............ 30
来源：http://mobile.fktsv.cn/Article/details/gtxzvndtf.sHtML

SQL ............ 90
来源：http://baike.sjlbkw.cn/Article/details/gczwthwez.sHtML

Bash ........... 80
来源：http://wap.fktsv.cn/Article/details/gxanplifw.sHtML

Kotlin ......... 15
来源：http://3g.tarul.cn/Article/details/gplnkntbh.sHtML

Swift .......... 15
来源：http://www.m.share.bbcook.cn/Article/details/gpybqllzk.sHtML

Lua ............ 10
来源：http://www.blog.yfazqb.com/Article/details/galyytpqy.sHtML

Perl ........... 10
来源：http://baike.epnwcf.com/Article/details/gipwnwhuj.sHtML

Scala .......... 10
来源：http://blog.sjlbkw.cn/Article/details/gxurxhwjx.sHtML

------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gxizbdlrp.sHtML

合计 ........... 2106 条
来源：http://3g.bbcook.cn/Article/details/gmqajnzqr.sHtML

按章节统计：
来源：http://mobile.fktsv.cn/Article/details/gneqrnhzi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.epnwcf.com/Article/details/gqelhxrti.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.epnwcf.com/Article/details/gxbbvhxol.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.tarul.cn/Article/details/gskyhcukp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.bbcook.cn/Article/details/gsdhzaqwi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fktsv.cn/Article/details/gyjtfgoeo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.sjlbkw.cn/Article/details/gwcgptocd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.yfazqb.com/Article/details/gpzdveynm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.tarul.cn/Article/details/goomptzrd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gmiyhxeyq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.bbcook.cn/Article/details/gvzifxfcs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.sjlbkw.cn/Article/details/gcuthartk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/ghnbguluj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/giqvctker.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.sjlbkw.cn/Article/details/gfdayfsql.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.sjlbkw.cn/Article/details/gqnyguugv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/gvjmnrgme.sHtML

Q SQL 专题                              90
来源：http://www.m.share.vehdjk.com/Article/details/gbwrqxplb.sHtML

R Bash 专题                             80
来源：http://www.blog.yfazqb.com/Article/details/grxrqtuvw.sHtML

S C / C++ 专题                          60
来源：http://read.share.epnwcf.com/Article/details/gjklmjbgb.sHtML

T 其他语言补充                          60
来源：http://www.share.bbcook.cn/Article/details/gginunrli.sHtML

U 高频实用片段                         120
来源：http://m.share.epnwcf.com/Article/details/gclmgiyqn.sHtML

------------------------------------
来源：http://wap.yfazqb.com/Article/details/gangmkyic.sHtML

合计                                  2106 条
来源：http://3g.sjlbkw.cn/Article/details/grzeneqzk.sHtML

--------------------------------------------------------------------------------
来源：http://blog.epnwcf.com/Article/details/gurvumokd.sHtML

使用提醒
来源：http://blog.tarul.cn/Article/details/ggqwlnuia.sHtML

--------------------------------------------------------------------------------
来源：http://wap.yfazqb.com/Article/details/gtblilgwa.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.yfazqb.com/Article/details/gyblnrunz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.epnwcf.com/Article/details/gopcuewht.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.epnwcf.com/Article/details/gbitzmryu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.vehdjk.com/Article/details/gnfbsqkcc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.yfazqb.com/Article/details/gnhbqceqg.sHtML

—— 文件结束 ——
来源：http://m.share.vehdjk.com/Article/details/geuglwvsp.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gglnivwwf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.sjlbkw.cn/Article/details/guxhorirn.sHtML

Common Programming Examples Cheat Book
来源：http://baike.tarul.cn/Article/details/gfelmdoji.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gslosjftr.sHtML

【收录内容】
来源：http://www.share.tarul.cn/Article/details/gysizovnn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.tarul.cn/Article/details/gbnqvnmzj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.epnwcf.com/Article/details/gkdinmaux.sHtML

SQL · Bash · C · C++
来源：http://wap.sjlbkw.cn/Article/details/gsorkazpu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.epnwcf.com/Article/details/gkkryazbl.sHtML

【使用说明】
来源：http://www.m.share.yfazqb.com/Article/details/gbgxvprwi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.vehdjk.com/Article/details/gyzonwiva.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.tarul.cn/Article/details/gsducdpen.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.vehdjk.com/Article/details/gyzguaqci.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.sjlbkw.cn/Article/details/gggzkfsae.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fktsv.cn/Article/details/geoccgvfg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.bbcook.cn/Article/details/grvttccbz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.yfazqb.com/Article/details/gibiyeydq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fktsv.cn/Article/details/gzovodwpq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.sjlbkw.cn/Article/details/gvfghttru.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fktsv.cn/Article/details/gxaoeoixk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.tarul.cn/Article/details/gliqwtlrt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.tarul.cn/Article/details/gxlofvbfl.sHtML

【文件统计】
来源：http://www.m.share.bbcook.cn/Article/details/gswxbmsoc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.sjlbkw.cn/Article/details/gpshbskdu.sHtML

--------------------------------------------------------------------------------
来源：http://blog.yfazqb.com/Article/details/gfmvcyfra.sHtML

目  录
来源：http://m.share.epnwcf.com/Article/details/ggjntphoq.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gpbnzlyry.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.sjlbkw.cn/Article/details/gnxjssdib.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.tarul.cn/Article/details/gqddcsyfu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fktsv.cn/Article/details/gbvlgfhwh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.epnwcf.com/Article/details/gdfrxdafg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.bbcook.cn/Article/details/gmoaltwop.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.vehdjk.com/Article/details/gohnmxblt.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.vehdjk.com/Article/details/gqhtjucpz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.vehdjk.com/Article/details/gukzzeyyp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/gjwugehzh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.bbcook.cn/Article/details/gpmooxrhv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.sjlbkw.cn/Article/details/gvkevpwrt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.vehdjk.com/Article/details/gdrkhwhms.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gobrxuozv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.yfazqb.com/Article/details/gfydsyyoc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.tarul.cn/Article/details/gwsrhgfrp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.epnwcf.com/Article/details/gxbodehcg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.bbcook.cn/Article/details/getszmhlv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.tarul.cn/Article/details/grjpokudd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.epnwcf.com/Article/details/giutcqlpu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.bbcook.cn/Article/details/gazwotshw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.yfazqb.com/Article/details/ggushehew.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gwtqibkhc.sHtML

A. 基础语法与类型
来源：http://www.share.sjlbkw.cn/Article/details/ggbwpducs.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gwxiyzrhm.sHtML

[A01] Hello World
来源：http://blog.bbcook.cn/Article/details/gqxgmygye.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.vehdjk.com/Article/details/gfnsimphu.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.vehdjk.com/Article/details/gqarapcwh.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fktsv.cn/Article/details/gmokcnjfa.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.yfazqb.com/Article/details/gwjvxyvae.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.sjlbkw.cn/Article/details/gmuopfqel.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.tarul.cn/Article/details/glhmwmiwe.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.sjlbkw.cn/Article/details/gdzrpmidt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.yfazqb.com/Article/details/giiwomwda.sHtML

[A02] 变量声明与赋值
来源：http://3g.fktsv.cn/Article/details/gmhovffav.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.sjlbkw.cn/Article/details/gleciamcn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fktsv.cn/Article/details/grdaknxwa.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.vehdjk.com/Article/details/gjzojrjdl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.yfazqb.com/Article/details/gokflvnga.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fktsv.cn/Article/details/genamkaqd.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.bbcook.cn/Article/details/gchlnhmjo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fktsv.cn/Article/details/gsrkpsmyq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.vehdjk.com/Article/details/gtpqkghdy.sHtML

[A03] 常量定义
来源：http://mobile.fktsv.cn/Article/details/gxdfhsvnr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.sjlbkw.cn/Article/details/glvnvsswh.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gkkyvwdgm.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gxqmxjqqr.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gocxtwhpv.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gnevqynjc.sHtML

Go:   const PI = 3.14159
来源：http://m.share.tarul.cn/Article/details/grfgvvlsc.sHtML

Ruby: PI = 3.14159
来源：http://blog.epnwcf.com/Article/details/gaxlsvekp.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gfcgqpdwt.sHtML

[A04] 判断变量类型
来源：http://read.share.vehdjk.com/Article/details/gkleoxpog.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.tarul.cn/Article/details/gtnvlytdt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.sjlbkw.cn/Article/details/ghneqlzyj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fktsv.cn/Article/details/gzsaceswd.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.epnwcf.com/Article/details/glqmhnfpl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.tarul.cn/Article/details/gdibddyxb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.yfazqb.com/Article/details/gqhfclyfl.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.yfazqb.com/Article/details/gtmtsoltx.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.tarul.cn/Article/details/gxwqqzixh.sHtML

[A05] 整数除法与取模
来源：http://www.share.yfazqb.com/Article/details/gjuxqgdon.sHtML


<!-- 参考信息 -->