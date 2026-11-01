代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.share.tarul.cn/Article/details/gvsqpikgp.sHtML

sys.stdout.isatty()
来源：http://3g.bbcook.cn/Article/details/gmztmbtwt.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.vehdjk.com/Article/details/gzfxzghyj.sHtML

print("err", file=sys.stderr)
来源：http://baike.sjlbkw.cn/Article/details/grnrymokh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.yfazqb.com/Article/details/gtspfhhdr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fktsv.cn/Article/details/gxjqqzkau.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.tarul.cn/Article/details/gtzqybunl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.tarul.cn/Article/details/gaohlmfee.sHtML

[U43] PHP：声明命名空间
来源：http://wap.vehdjk.com/Article/details/gjhfykrpp.sHtML

namespace App\Http;
来源：http://m.share.vehdjk.com/Article/details/gsbytmiez.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fktsv.cn/Article/details/gzdziiwrl.sHtML

declare(strict_types=1);
来源：http://mobile.yfazqb.com/Article/details/gxalkctxp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.epnwcf.com/Article/details/gyggccesc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gkozzeeqq.sHtML

[U46] PHP：可空类型
来源：http://www.share.sjlbkw.cn/Article/details/gyibqfyxt.sHtML

?string $name = null
来源：http://www.m.share.fktsv.cn/Article/details/gwkrqvgfh.sHtML

[U47] PHP：联合类型
来源：http://mobile.epnwcf.com/Article/details/ghjwkufiv.sHtML

int|string $id
来源：http://m.share.vehdjk.com/Article/details/gyvwbkpkw.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gkeagnrfr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fktsv.cn/Article/details/gqajtbujn.sHtML

[U49] PHP：只读属性
来源：http://www.blog.sjlbkw.cn/Article/details/garimkqid.sHtML

public readonly string $name
来源：http://read.share.bbcook.cn/Article/details/gwghqruzj.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fktsv.cn/Article/details/gyhaahojz.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fktsv.cn/Article/details/gfyjpjvhs.sHtML

[U51] PHP：数组解构
来源：http://wap.epnwcf.com/Article/details/gjcjqhhun.sHtML

[$a, $b] = $arr;
来源：http://www.share.fktsv.cn/Article/details/gfiozzwez.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.epnwcf.com/Article/details/gonorydwd.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.tarul.cn/Article/details/geyxbamcz.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.vehdjk.com/Article/details/gtegldaro.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.vehdjk.com/Article/details/gucmrmmvb.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.tarul.cn/Article/details/gthpcpxel.sHtML

$obj?->method()
来源：http://blog.yfazqb.com/Article/details/gjhjameyk.sHtML

[U55] PHP：match 表达式
来源：http://m.share.tarul.cn/Article/details/gwlusxnvr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fktsv.cn/Article/details/gcdivmrdr.sHtML

[U56] PHP：命名参数
来源：http://wap.tarul.cn/Article/details/gixpureor.sHtML

f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/gugnpvbho.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.tarul.cn/Article/details/gguwmblts.sHtML

"值: {$a}"
来源：http://mobile.fktsv.cn/Article/details/gjbhevlwi.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.epnwcf.com/Article/details/geavebdtu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.vehdjk.com/Article/details/grqpclvcw.sHtML

[U59] PHP：自定义排序
来源：http://blog.fktsv.cn/Article/details/gmlkdauzs.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fktsv.cn/Article/details/guhmarbdq.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.bbcook.cn/Article/details/gokboveyg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.epnwcf.com/Article/details/gqudvcyfs.sHtML

[U61] PHP：正则
来源：http://3g.fktsv.cn/Article/details/gqkfctjbk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.yfazqb.com/Article/details/gxeuszcoz.sHtML

[U62] PHP：日期对象
来源：http://m.share.yfazqb.com/Article/details/ggaszknfr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.bbcook.cn/Article/details/gmgueepnn.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fktsv.cn/Article/details/gmtwiwrcl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.epnwcf.com/Article/details/gztobbsjd.sHtML

[U64] PHP：目录遍历
来源：http://3g.vehdjk.com/Article/details/gfhryadsa.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.tarul.cn/Article/details/gtreuvfdt.sHtML

[U65] PHP：会话
来源：http://baike.yfazqb.com/Article/details/gyfztrxqg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.bbcook.cn/Article/details/gzdqwyuah.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.vehdjk.com/Article/details/gaengqban.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.vehdjk.com/Article/details/glmomsspp.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.tarul.cn/Article/details/gxoelopnn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.vehdjk.com/Article/details/gfulbkyhq.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.tarul.cn/Article/details/gvgyfgxgl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.sjlbkw.cn/Article/details/gnbdrhjqn.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.vehdjk.com/Article/details/gwyuvpuqo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.vehdjk.com/Article/details/gpyhuygzv.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fktsv.cn/Article/details/gxjmxbrhb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.tarul.cn/Article/details/gvolgptow.sHtML

[U71] PHP：抛出异常
来源：http://blog.yfazqb.com/Article/details/gieznbhfn.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.sjlbkw.cn/Article/details/gcoopknqe.sHtML

[U72] PHP：写错误日志
来源：http://m.share.sjlbkw.cn/Article/details/gmkjzlqdt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.vehdjk.com/Article/details/gnzpfmtev.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.tarul.cn/Article/details/gejpekmzu.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.tarul.cn/Article/details/gafuelpzi.sHtML

[U74] PHP：读取环境变量
来源：http://wap.epnwcf.com/Article/details/grmlpkdkv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.sjlbkw.cn/Article/details/gjvydklqz.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.bbcook.cn/Article/details/goxnaflyq.sHtML

composer require psr/container
来源：http://wap.tarul.cn/Article/details/gvkdnbtdd.sHtML

[U76] PHP：简单路由
来源：http://3g.fktsv.cn/Article/details/ghrxajjxg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.yfazqb.com/Article/details/gqtarkycn.sHtML

[U77] PHP：模板渲染
来源：http://m.share.tarul.cn/Article/details/gtnearsfp.sHtML

composer require twig/twig
来源：http://www.share.fktsv.cn/Article/details/gwretgzca.sHtML

[U78] PHP：单元测试
来源：http://read.share.yfazqb.com/Article/details/gsqxrlzvm.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.yfazqb.com/Article/details/goaafgpkr.sHtML

[U79] PHP：静态分析
来源：http://baike.bbcook.cn/Article/details/ggjpclfut.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fktsv.cn/Article/details/gvrqgbbwn.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.bbcook.cn/Article/details/gjuoaqhrk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fktsv.cn/Article/details/gtlcyqwgm.sHtML

[U81] JS：初始化项目
来源：http://read.share.fktsv.cn/Article/details/gfpkefroq.sHtML

npm init -y;  npm i express
来源：http://baike.fktsv.cn/Article/details/gikhiaods.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.tarul.cn/Article/details/geupfwmpt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.sjlbkw.cn/Article/details/gkajovitk.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.vehdjk.com/Article/details/gcetnlnym.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.sjlbkw.cn/Article/details/gjrcfckgc.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.vehdjk.com/Article/details/gryhfjpjl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.epnwcf.com/Article/details/gixswcgqy.sHtML

[U85] JS：可选链
来源：http://m.share.sjlbkw.cn/Article/details/grewnxgyj.sHtML

a?.b?.c
来源：http://3g.epnwcf.com/Article/details/gherngcxv.sHtML

[U86] JS：空值合并
来源：http://blog.fktsv.cn/Article/details/gxkgqhxee.sHtML

a ?? b
来源：http://read.share.vehdjk.com/Article/details/grpazdxyc.sHtML

[U87] JS：解构默认值
来源：http://baike.vehdjk.com/Article/details/gjbnqytil.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.sjlbkw.cn/Article/details/gzxpxzwhj.sHtML

[U88] JS：对象展开合并
来源：http://3g.yfazqb.com/Article/details/gblslrwcb.sHtML

{ ...a, ...b }
来源：http://wap.sjlbkw.cn/Article/details/gdkvywiqt.sHtML

[U89] JS：数组去重
来源：http://3g.sjlbkw.cn/Article/details/gckackhdf.sHtML

[...new Set(arr)]
来源：http://3g.fktsv.cn/Article/details/gkgpsewmv.sHtML

[U90] JS：数字数组排序
来源：http://3g.yfazqb.com/Article/details/guwaoebih.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/grrerszlt.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.bbcook.cn/Article/details/gvoorpmxr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.sjlbkw.cn/Article/details/givkupwsl.sHtML

[U92] JS：深拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gxslvccje.sHtML

structuredClone(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gwyldyucc.sHtML

[U93] JS：模板字符串
来源：http://wap.yfazqb.com/Article/details/gnhwxrbmu.sHtML

`共 ${n} 条`
来源：http://m.share.bbcook.cn/Article/details/gptyfkgga.sHtML

[U94] JS：箭头函数
来源：http://mobile.bbcook.cn/Article/details/gjrujrsla.sHtML

const double = x => x * 2;
来源：http://www.share.bbcook.cn/Article/details/gjskwpgvt.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.tarul.cn/Article/details/gchftcftw.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.vehdjk.com/Article/details/gobnajtnl.sHtML

[U96] JS：async/await 与异常
来源：http://wap.vehdjk.com/Article/details/gbfgjsalt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gvludvawo.sHtML

[U97] JS：并发请求
来源：http://wap.tarul.cn/Article/details/gzuxjpiyh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gvmzxkfef.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.sjlbkw.cn/Article/details/gtyycbpyn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.bbcook.cn/Article/details/gsmygwlfj.sHtML

[U99] JS：事件监听
来源：http://m.share.yfazqb.com/Article/details/gkcchdvts.sHtML

el.addEventListener("click", e => {})
来源：http://baike.tarul.cn/Article/details/gmjtkkqfe.sHtML

[U100] JS：DOM 查询
来源：http://mobile.tarul.cn/Article/details/gftipzdvh.sHtML

document.querySelector(".item")
来源：http://3g.vehdjk.com/Article/details/gzlsrnqiu.sHtML

[U101] JS：classList 操作
来源：http://read.share.yfazqb.com/Article/details/gcfnnlkxo.sHtML

el.classList.toggle("active")
来源：http://3g.tarul.cn/Article/details/gufchulue.sHtML

[U102] JS：本地存储
来源：http://3g.tarul.cn/Article/details/gkakyvvpt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.sjlbkw.cn/Article/details/gthrinuoi.sHtML

[U103] JS：定时器
来源：http://blog.bbcook.cn/Article/details/gonlimfuc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.vehdjk.com/Article/details/gnkxifflo.sHtML

[U104] JS：防抖
来源：http://www.share.bbcook.cn/Article/details/gzjsmvmpd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gaxedgozu.sHtML

[U105] JS：节流
来源：http://wap.fktsv.cn/Article/details/gfcctpqpu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.tarul.cn/Article/details/gbwzccrbc.sHtML

[U106] JS：日期格式化
来源：http://www.share.vehdjk.com/Article/details/gdxoejdix.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.vehdjk.com/Article/details/ghwgvjlfs.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.epnwcf.com/Article/details/gvfkwehwd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.bbcook.cn/Article/details/gtvbfyqan.sHtML

[U108] JS：随机整数
来源：http://www.blog.fktsv.cn/Article/details/gjgienolc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.vehdjk.com/Article/details/gigtdjbgp.sHtML

[U109] JS：数组分组
来源：http://mobile.vehdjk.com/Article/details/gkytkrvfa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.bbcook.cn/Article/details/gctozwdsa.sHtML

[U110] JS：数组分块
来源：http://www.m.share.vehdjk.com/Article/details/gjdqziixc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.yfazqb.com/Article/details/gtfcwonre.sHtML

[U111] JS：对象转 Map
来源：http://read.share.bbcook.cn/Article/details/gwuotvwok.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.vehdjk.com/Article/details/guxgrkkrg.sHtML

[U112] JS：字符串补位
来源：http://baike.bbcook.cn/Article/details/grisbovad.sHtML

"7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gsrijzziv.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.tarul.cn/Article/details/gvfawudno.sHtML

s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/ggetnwzji.sHtML

[U114] JS：JSON 深比较
来源：http://blog.yfazqb.com/Article/details/gnsidjgjz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.yfazqb.com/Article/details/govrygngc.sHtML

[U115] JS：生成 UUID
来源：http://3g.bbcook.cn/Article/details/ggwacsfob.sHtML

crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/gxiyoyycy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.tarul.cn/Article/details/gkcfzeniv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.yfazqb.com/Article/details/gcrmsarkp.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fktsv.cn/Article/details/gufmxxeqr.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.epnwcf.com/Article/details/grygrgqch.sHtML

[U118] JS：开发服务器
来源：http://m.share.sjlbkw.cn/Article/details/gireiapsu.sHtML

npm i -D vite;  npx vite
来源：http://www.share.yfazqb.com/Article/details/gmpmkjbeg.sHtML

[U119] JS：生产构建
来源：http://www.share.yfazqb.com/Article/details/gxhkooedn.sHtML

npx vite build
来源：http://read.share.sjlbkw.cn/Article/details/gzqerkrsx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fktsv.cn/Article/details/ggbavmhxw.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.yfazqb.com/Article/details/gzxsgbnyg.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gjatnwcss.sHtML

统计汇总
来源：http://blog.tarul.cn/Article/details/gmuzszjws.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gpxmduxwh.sHtML

按语言统计（条）：
来源：http://www.share.fktsv.cn/Article/details/geboqjoue.sHtML

Python ......... 252
来源：http://read.share.sjlbkw.cn/Article/details/gpjtngfik.sHtML

PHP ............ 252
来源：http://read.share.vehdjk.com/Article/details/gbasakddh.sHtML

JavaScript ..... 252
来源：http://3g.tarul.cn/Article/details/gkfdlggqp.sHtML

TypeScript ..... 212
来源：http://www.blog.bbcook.cn/Article/details/gxurciugm.sHtML

Java ........... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gljlpktwt.sHtML

Go ............. 212
来源：http://3g.yfazqb.com/Article/details/gnxaddyev.sHtML

Ruby ........... 212
来源：http://wap.fktsv.cn/Article/details/guuxmiiht.sHtML

C# ............. 212
来源：http://blog.epnwcf.com/Article/details/gzmmyziie.sHtML

C .............. 30
来源：http://www.share.epnwcf.com/Article/details/glfxjkdad.sHtML

C++ ............ 30
来源：http://blog.tarul.cn/Article/details/gdyxeocgo.sHtML

SQL ............ 90
来源：http://wap.tarul.cn/Article/details/ggjshcmxu.sHtML

Bash ........... 80
来源：http://www.share.sjlbkw.cn/Article/details/gkqclepmb.sHtML

Kotlin ......... 15
来源：http://m.share.fktsv.cn/Article/details/gbxjcpuik.sHtML

Swift .......... 15
来源：http://www.m.share.fktsv.cn/Article/details/goxjikayr.sHtML

Lua ............ 10
来源：http://m.share.fktsv.cn/Article/details/gvubtdqjs.sHtML

Perl ........... 10
来源：http://www.share.yfazqb.com/Article/details/glsgvsmob.sHtML

Scala .......... 10
来源：http://read.share.bbcook.cn/Article/details/gehhoiikl.sHtML

------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gxlrfwcja.sHtML

合计 ........... 2106 条
来源：http://m.share.epnwcf.com/Article/details/gidpcjnhr.sHtML

按章节统计：
来源：http://read.share.yfazqb.com/Article/details/gnutahxqm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.sjlbkw.cn/Article/details/gekbapynl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.epnwcf.com/Article/details/gvrmvchrw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.vehdjk.com/Article/details/gjukzlxye.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fktsv.cn/Article/details/gmdlsljkb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.tarul.cn/Article/details/gxpkrdjcs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.vehdjk.com/Article/details/gedvnwghv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.vehdjk.com/Article/details/gpztrvlyc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.tarul.cn/Article/details/guoptfbdc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gxfrbniog.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fktsv.cn/Article/details/ganwwukbd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gdmuiimyp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gxomjhmrw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/geqjubqkf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.bbcook.cn/Article/details/gpnznbkhs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.vehdjk.com/Article/details/gnrlfsttv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/gmajlsjap.sHtML

Q SQL 专题                              90
来源：http://m.share.vehdjk.com/Article/details/gwjqgnihf.sHtML

R Bash 专题                             80
来源：http://www.blog.tarul.cn/Article/details/galgffxjh.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.vehdjk.com/Article/details/ggsswiere.sHtML

T 其他语言补充                          60
来源：http://read.share.tarul.cn/Article/details/gbndtblfp.sHtML

U 高频实用片段                         120
来源：http://blog.bbcook.cn/Article/details/gvckssxvv.sHtML

------------------------------------
来源：http://wap.fktsv.cn/Article/details/gvafwkkmy.sHtML

合计                                  2106 条
来源：http://www.share.epnwcf.com/Article/details/ghtclitfv.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.tarul.cn/Article/details/gvryvhkxw.sHtML

使用提醒
来源：http://www.blog.fktsv.cn/Article/details/gzmrhadfv.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gedkbqyyd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.yfazqb.com/Article/details/gnhtvwcim.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.bbcook.cn/Article/details/gnkohvkhg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.epnwcf.com/Article/details/gdzsicfca.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.bbcook.cn/Article/details/grztwcrtt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.vehdjk.com/Article/details/ggtuhkbdy.sHtML

—— 文件结束 ——
来源：http://blog.vehdjk.com/Article/details/giucxapez.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gypivvitv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.yfazqb.com/Article/details/ghvtrnkwv.sHtML

Common Programming Examples Cheat Book
来源：http://3g.bbcook.cn/Article/details/gawdwigwd.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/guporojet.sHtML

【收录内容】
来源：http://3g.bbcook.cn/Article/details/gxleeuogf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fktsv.cn/Article/details/guggtaefz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fktsv.cn/Article/details/ghvtdmfbr.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fktsv.cn/Article/details/gqcwqqfin.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.sjlbkw.cn/Article/details/gyflkdbml.sHtML

【使用说明】
来源：http://baike.yfazqb.com/Article/details/gifprzisv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.vehdjk.com/Article/details/gkyspknmc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.epnwcf.com/Article/details/goywlwgeo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.vehdjk.com/Article/details/gcvuavusc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.sjlbkw.cn/Article/details/gbxyhnaze.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.yfazqb.com/Article/details/gxetzdmvg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.epnwcf.com/Article/details/ghvoqjqmh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.bbcook.cn/Article/details/ghjkvekwu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.tarul.cn/Article/details/ghelwngwd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.yfazqb.com/Article/details/gjurtjuyu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.sjlbkw.cn/Article/details/gfqulwqij.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.vehdjk.com/Article/details/guyxybmag.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fktsv.cn/Article/details/gomshosjr.sHtML

【文件统计】
来源：http://blog.bbcook.cn/Article/details/gngoncriw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.epnwcf.com/Article/details/grgofokad.sHtML

--------------------------------------------------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/glszfurib.sHtML

目  录
来源：http://blog.vehdjk.com/Article/details/gxskjxkej.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gfupwqvyk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.yfazqb.com/Article/details/gxfblsklc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.vehdjk.com/Article/details/gyowvjjrq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.yfazqb.com/Article/details/gnhdrpaem.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.sjlbkw.cn/Article/details/gyqedtljx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.sjlbkw.cn/Article/details/gysordkue.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmhcmggg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.yfazqb.com/Article/details/grjjhkabl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.yfazqb.com/Article/details/gjmnaifzg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/gtoijjpjq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.tarul.cn/Article/details/gppnrtqzr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.sjlbkw.cn/Article/details/geslpnxbm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.sjlbkw.cn/Article/details/glrjujzqs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.tarul.cn/Article/details/ghgppwcjr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.bbcook.cn/Article/details/glyvoxljj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.vehdjk.com/Article/details/gtwyesbxe.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/gfhfogzyg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.bbcook.cn/Article/details/gwllooodw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.vehdjk.com/Article/details/gahernrvv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.vehdjk.com/Article/details/gfbqmzqsa.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.epnwcf.com/Article/details/ggnlxkrxq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.epnwcf.com/Article/details/gjioqgvip.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gioqfaudx.sHtML

A. 基础语法与类型
来源：http://baike.bbcook.cn/Article/details/gqtjceyjl.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gtztkuhef.sHtML

[A01] Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzvwqrws.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fktsv.cn/Article/details/gcsheucjv.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.sjlbkw.cn/Article/details/guqpygftb.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.tarul.cn/Article/details/gfccwzhbt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.tarul.cn/Article/details/gmpidzaeh.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.tarul.cn/Article/details/gblxmgfvv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.sjlbkw.cn/Article/details/gkttuioxp.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.bbcook.cn/Article/details/gleqlfrss.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.bbcook.cn/Article/details/gspiutdjs.sHtML

[A02] 变量声明与赋值
来源：http://wap.vehdjk.com/Article/details/ggfzyzpfi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.yfazqb.com/Article/details/gwdqatfuz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.bbcook.cn/Article/details/gybtpnllf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/glqachkmx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fktsv.cn/Article/details/gslskojjx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.sjlbkw.cn/Article/details/gsjemsmvp.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.tarul.cn/Article/details/goxurxbnx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.epnwcf.com/Article/details/gmeoxjfwi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.yfazqb.com/Article/details/gfcjyvuzd.sHtML

[A03] 常量定义
来源：http://baike.epnwcf.com/Article/details/gshfetzbr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.vehdjk.com/Article/details/gsabuhzmo.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/gzoavaoqi.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gpqivwheh.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gfiikikjl.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gcpwvaprt.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.epnwcf.com/Article/details/gwzyzxdpe.sHtML

Ruby: PI = 3.14159
来源：http://mobile.tarul.cn/Article/details/gtcfvgxnj.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gevsyrocu.sHtML

[A04] 判断变量类型
来源：http://wap.vehdjk.com/Article/details/gspkvdanw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.sjlbkw.cn/Article/details/gorpodugn.sHtML


<!-- 参考信息 -->