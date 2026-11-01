代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fktsv.cn/Article/details/gizwdgpic.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.bbcook.cn/Article/details/ggbsqwdlc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.bbcook.cn/Article/details/gauskroyj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fktsv.cn/Article/details/gheqioxxg.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.yfazqb.com/Article/details/ghkhcixdk.sHtML

namespace App\Http;
来源：http://www.blog.fktsv.cn/Article/details/gbxxzohsw.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.yfazqb.com/Article/details/gvbkxeugp.sHtML

declare(strict_types=1);
来源：http://m.share.epnwcf.com/Article/details/grqqnkrsb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.epnwcf.com/Article/details/gruvlelgf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gmlzskctd.sHtML

[U46] PHP：可空类型
来源：http://mobile.sjlbkw.cn/Article/details/gjfzijvfl.sHtML

?string $name = null
来源：http://mobile.tarul.cn/Article/details/gwzaoexjx.sHtML

[U47] PHP：联合类型
来源：http://blog.bbcook.cn/Article/details/gebbpejrj.sHtML

int|string $id
来源：http://m.share.epnwcf.com/Article/details/gmnxfujzq.sHtML

[U48] PHP：纯枚举
来源：http://www.share.epnwcf.com/Article/details/gstbpocoi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.bbcook.cn/Article/details/gidnwxwfh.sHtML

[U49] PHP：只读属性
来源：http://baike.yfazqb.com/Article/details/gfkputxfo.sHtML

public readonly string $name
来源：http://3g.sjlbkw.cn/Article/details/ganijdseg.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.tarul.cn/Article/details/gtpplwamb.sHtML

public function __construct(private int $id) {}
来源：http://www.share.sjlbkw.cn/Article/details/gmztglvfa.sHtML

[U51] PHP：数组解构
来源：http://www.share.bbcook.cn/Article/details/glxvruesq.sHtML

[$a, $b] = $arr;
来源：http://mobile.yfazqb.com/Article/details/gnoceolnz.sHtML

[U52] PHP：箭头函数
来源：http://read.share.vehdjk.com/Article/details/gefjtvmeo.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fktsv.cn/Article/details/gnspmgfky.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.yfazqb.com/Article/details/gixljerwk.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.yfazqb.com/Article/details/gxuajtvih.sHtML

[U54] PHP：空安全调用
来源：http://baike.yfazqb.com/Article/details/gqzwvnqvh.sHtML

$obj?->method()
来源：http://m.share.tarul.cn/Article/details/gqeqdqarc.sHtML

[U55] PHP：match 表达式
来源：http://read.share.vehdjk.com/Article/details/gjizzpcgp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fktsv.cn/Article/details/gqzbkvjaw.sHtML

[U56] PHP：命名参数
来源：http://mobile.tarul.cn/Article/details/gkgoosuil.sHtML

f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/gvzvqsbey.sHtML

[U57] PHP：字符串插值
来源：http://3g.bbcook.cn/Article/details/grqbfncok.sHtML

"值: {$a}"
来源：http://www.m.share.tarul.cn/Article/details/gljmeirlz.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.sjlbkw.cn/Article/details/gsgozvhzy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fktsv.cn/Article/details/gxxsfyhou.sHtML

[U59] PHP：自定义排序
来源：http://baike.epnwcf.com/Article/details/gflncsncu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.tarul.cn/Article/details/gidnbxcue.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.tarul.cn/Article/details/grkrvzhyq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.yfazqb.com/Article/details/gfmuypavm.sHtML

[U61] PHP：正则
来源：http://www.share.fktsv.cn/Article/details/gkekczwnd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gdoyxtnmf.sHtML

[U62] PHP：日期对象
来源：http://m.share.fktsv.cn/Article/details/gphusrqkk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.yfazqb.com/Article/details/gcbhhyzle.sHtML

[U63] PHP：文件读写
来源：http://www.blog.vehdjk.com/Article/details/ghwlxkjxx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.tarul.cn/Article/details/gsgllawyj.sHtML

[U64] PHP：目录遍历
来源：http://m.share.epnwcf.com/Article/details/gospptnrs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.epnwcf.com/Article/details/gahsoykou.sHtML

[U65] PHP：会话
来源：http://www.share.sjlbkw.cn/Article/details/glsygjlxx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.yfazqb.com/Article/details/gpxqjojtr.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.sjlbkw.cn/Article/details/ghdrisfvq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.vehdjk.com/Article/details/ggvintzie.sHtML

[U67] PHP：处理文件上传
来源：http://3g.bbcook.cn/Article/details/geppidfas.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.vehdjk.com/Article/details/gwnuzlxyq.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.epnwcf.com/Article/details/ghsyaaiio.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.epnwcf.com/Article/details/gpwmoavms.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.yfazqb.com/Article/details/gqvwpcpsk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.epnwcf.com/Article/details/gqxvrfnwf.sHtML

[U70] PHP：PDO 事务
来源：http://3g.epnwcf.com/Article/details/grhlqypxj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.yfazqb.com/Article/details/gtpegzcjq.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.yfazqb.com/Article/details/gqtsuzwiq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.yfazqb.com/Article/details/gfgpmjwrl.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.yfazqb.com/Article/details/geryytqft.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.epnwcf.com/Article/details/gnsqwawel.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.vehdjk.com/Article/details/gkcrfduox.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.yfazqb.com/Article/details/gemtehwgn.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fktsv.cn/Article/details/gamvcwpsa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.vehdjk.com/Article/details/gnxapyenq.sHtML

[U75] PHP：依赖注入
来源：http://baike.fktsv.cn/Article/details/grnsmbhrv.sHtML

composer require psr/container
来源：http://wap.sjlbkw.cn/Article/details/gdnkceqzt.sHtML

[U76] PHP：简单路由
来源：http://mobile.tarul.cn/Article/details/gbbektfzd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.bbcook.cn/Article/details/gbrsxqnuj.sHtML

[U77] PHP：模板渲染
来源：http://baike.fktsv.cn/Article/details/gkveafraa.sHtML

composer require twig/twig
来源：http://www.blog.tarul.cn/Article/details/gfzfcbqqz.sHtML

[U78] PHP：单元测试
来源：http://m.share.tarul.cn/Article/details/gboxvtjcd.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fktsv.cn/Article/details/gziineubw.sHtML

[U79] PHP：静态分析
来源：http://mobile.epnwcf.com/Article/details/giyictiqx.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.sjlbkw.cn/Article/details/gdnqwkkha.sHtML

[U80] PHP：代码规范修复
来源：http://baike.epnwcf.com/Article/details/gczledukb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fktsv.cn/Article/details/giksckewo.sHtML

[U81] JS：初始化项目
来源：http://read.share.yfazqb.com/Article/details/gtmrddgbl.sHtML

npm init -y;  npm i express
来源：http://m.share.vehdjk.com/Article/details/gqnuetugo.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.sjlbkw.cn/Article/details/gsrvbwzrp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.tarul.cn/Article/details/ghfalcpyv.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.yfazqb.com/Article/details/ghoobsqsn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fktsv.cn/Article/details/gpsspkzza.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.epnwcf.com/Article/details/gdaeddiad.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.yfazqb.com/Article/details/gatuoauec.sHtML

[U85] JS：可选链
来源：http://blog.epnwcf.com/Article/details/gsbvqsynx.sHtML

a?.b?.c
来源：http://mobile.vehdjk.com/Article/details/gzgcuxmgu.sHtML

[U86] JS：空值合并
来源：http://read.share.bbcook.cn/Article/details/gwebpkwav.sHtML

a ?? b
来源：http://wap.fktsv.cn/Article/details/gjxsekrmy.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gehmvrhxt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.bbcook.cn/Article/details/glhabvgwo.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.bbcook.cn/Article/details/gzbtomspc.sHtML

{ ...a, ...b }
来源：http://baike.yfazqb.com/Article/details/glgoxkctd.sHtML

[U89] JS：数组去重
来源：http://baike.vehdjk.com/Article/details/gtwuccyvm.sHtML

[...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/glhsijauc.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.vehdjk.com/Article/details/gdqwptfmw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/gkhjjyadd.sHtML

[U91] JS：对象键值遍历
来源：http://3g.tarul.cn/Article/details/gnchcnhqc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.epnwcf.com/Article/details/gnhowpszs.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.vehdjk.com/Article/details/glnrfcqjp.sHtML

structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/gjoxxekvx.sHtML

[U93] JS：模板字符串
来源：http://www.blog.yfazqb.com/Article/details/gcgjojivt.sHtML

`共 ${n} 条`
来源：http://baike.tarul.cn/Article/details/gjsanvxzt.sHtML

[U94] JS：箭头函数
来源：http://www.blog.tarul.cn/Article/details/gzfqqxujw.sHtML

const double = x => x * 2;
来源：http://mobile.sjlbkw.cn/Article/details/gxsllacfn.sHtML

[U95] JS：Promise 包装
来源：http://mobile.yfazqb.com/Article/details/gmqfqhwsq.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.sjlbkw.cn/Article/details/goztphgdn.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fktsv.cn/Article/details/gyklhurzg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/goghtbknw.sHtML

[U97] JS：并发请求
来源：http://baike.epnwcf.com/Article/details/gnqrmxpca.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gdwbrnbun.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fktsv.cn/Article/details/gjrljmrjp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fktsv.cn/Article/details/gihtrwkmm.sHtML

[U99] JS：事件监听
来源：http://read.share.sjlbkw.cn/Article/details/gjjjwvgfd.sHtML

el.addEventListener("click", e => {})
来源：http://wap.yfazqb.com/Article/details/gwyxczrcm.sHtML

[U100] JS：DOM 查询
来源：http://baike.yfazqb.com/Article/details/gvyklzxdt.sHtML

document.querySelector(".item")
来源：http://read.share.epnwcf.com/Article/details/gyefbjxjw.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gglhuvkid.sHtML

el.classList.toggle("active")
来源：http://read.share.epnwcf.com/Article/details/gttdrbczt.sHtML

[U102] JS：本地存储
来源：http://read.share.epnwcf.com/Article/details/gzjhyspeq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.epnwcf.com/Article/details/ggrptesdo.sHtML

[U103] JS：定时器
来源：http://3g.yfazqb.com/Article/details/gagzktyrg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.vehdjk.com/Article/details/gannyoksp.sHtML

[U104] JS：防抖
来源：http://mobile.sjlbkw.cn/Article/details/grdwmzcbh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gqftnymmf.sHtML

[U105] JS：节流
来源：http://3g.tarul.cn/Article/details/gxcnpjovj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fktsv.cn/Article/details/gwjzfzcfo.sHtML

[U106] JS：日期格式化
来源：http://mobile.tarul.cn/Article/details/goiutwbkr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fktsv.cn/Article/details/gqdcpyyrf.sHtML

[U107] JS：数字千分位
来源：http://m.share.bbcook.cn/Article/details/gvgbnjnud.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gertyexys.sHtML

[U108] JS：随机整数
来源：http://wap.sjlbkw.cn/Article/details/gdfplbedv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.vehdjk.com/Article/details/gezovdlfs.sHtML

[U109] JS：数组分组
来源：http://www.share.sjlbkw.cn/Article/details/gjarkuyux.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fktsv.cn/Article/details/gjqqqbzya.sHtML

[U110] JS：数组分块
来源：http://www.share.bbcook.cn/Article/details/gczlhfegm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.yfazqb.com/Article/details/gzjkwmbty.sHtML

[U111] JS：对象转 Map
来源：http://mobile.tarul.cn/Article/details/gjllqdslm.sHtML

new Map(Object.entries(obj))
来源：http://3g.vehdjk.com/Article/details/gvibhrdqy.sHtML

[U112] JS：字符串补位
来源：http://read.share.sjlbkw.cn/Article/details/gllyljhow.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gkgfjpeps.sHtML

[U113] JS：正则替换全部
来源：http://baike.yfazqb.com/Article/details/gagfbedlr.sHtML

s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/givolglbp.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.yfazqb.com/Article/details/gurygzjzu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.tarul.cn/Article/details/gilyzhkqm.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fktsv.cn/Article/details/gvselihpl.sHtML

crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gmhghaaeh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fktsv.cn/Article/details/gbaorknrk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.tarul.cn/Article/details/ggfavijsm.sHtML

[U117] JS：单元测试
来源：http://wap.tarul.cn/Article/details/gbxieqsfy.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.sjlbkw.cn/Article/details/gtmmegyyh.sHtML

[U118] JS：开发服务器
来源：http://wap.yfazqb.com/Article/details/gzxytwnxp.sHtML

npm i -D vite;  npx vite
来源：http://www.share.sjlbkw.cn/Article/details/gzifuhdbe.sHtML

[U119] JS：生产构建
来源：http://mobile.bbcook.cn/Article/details/gxpitntnz.sHtML

npx vite build
来源：http://wap.bbcook.cn/Article/details/gkhpasroh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.bbcook.cn/Article/details/gptpoqzss.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.epnwcf.com/Article/details/gwyfnsgpn.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gniiypjqk.sHtML

统计汇总
来源：http://m.share.yfazqb.com/Article/details/gilkoutjq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/goxlmzbec.sHtML

按语言统计（条）：
来源：http://3g.tarul.cn/Article/details/gqpqgxmln.sHtML

Python ......... 252
来源：http://www.m.share.epnwcf.com/Article/details/gscrrknbn.sHtML

PHP ............ 252
来源：http://wap.bbcook.cn/Article/details/gxvnjtbfq.sHtML

JavaScript ..... 252
来源：http://www.share.epnwcf.com/Article/details/guxpjbovj.sHtML

TypeScript ..... 212
来源：http://m.share.epnwcf.com/Article/details/gpydwypjg.sHtML

Java ........... 212
来源：http://blog.yfazqb.com/Article/details/glmevodas.sHtML

Go ............. 212
来源：http://blog.fktsv.cn/Article/details/gjzuirhfj.sHtML

Ruby ........... 212
来源：http://m.share.fktsv.cn/Article/details/gcfbzwpbq.sHtML

C# ............. 212
来源：http://www.share.tarul.cn/Article/details/gkpnhwheg.sHtML

C .............. 30
来源：http://baike.vehdjk.com/Article/details/gpgzpzojx.sHtML

C++ ............ 30
来源：http://m.share.epnwcf.com/Article/details/gnhtdsflp.sHtML

SQL ............ 90
来源：http://www.m.share.bbcook.cn/Article/details/gvbddocbh.sHtML

Bash ........... 80
来源：http://baike.yfazqb.com/Article/details/gfcsgjqxc.sHtML

Kotlin ......... 15
来源：http://www.m.share.sjlbkw.cn/Article/details/gngjbkowv.sHtML

Swift .......... 15
来源：http://m.share.fktsv.cn/Article/details/groqzohlp.sHtML

Lua ............ 10
来源：http://baike.sjlbkw.cn/Article/details/ggvurouts.sHtML

Perl ........... 10
来源：http://m.share.vehdjk.com/Article/details/gymcpwixh.sHtML

Scala .......... 10
来源：http://read.share.bbcook.cn/Article/details/gonyitchr.sHtML

------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gxqvxamkg.sHtML

合计 ........... 2106 条
来源：http://3g.sjlbkw.cn/Article/details/gnwlmnhss.sHtML

按章节统计：
来源：http://www.blog.tarul.cn/Article/details/gxkltnmwx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.sjlbkw.cn/Article/details/gbpajfxku.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.tarul.cn/Article/details/geyzxftdk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fktsv.cn/Article/details/gjgnxoiju.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.sjlbkw.cn/Article/details/gzaobbsdo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.epnwcf.com/Article/details/gzkfldwqf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.epnwcf.com/Article/details/gmlfktnir.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.vehdjk.com/Article/details/ghyxkdtgw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.bbcook.cn/Article/details/gurmglwid.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.epnwcf.com/Article/details/ggvcrtwre.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.vehdjk.com/Article/details/gipmzhkpr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gxubsyxvy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gcjsvtkzo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gewtuuusy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.tarul.cn/Article/details/gdnykrfox.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.bbcook.cn/Article/details/ghdejyexl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/gcyshgcxt.sHtML

Q SQL 专题                              90
来源：http://wap.bbcook.cn/Article/details/gfkefiuel.sHtML

R Bash 专题                             80
来源：http://read.share.tarul.cn/Article/details/gekgqybqj.sHtML

S C / C++ 专题                          60
来源：http://mobile.yfazqb.com/Article/details/gsdcpslsv.sHtML

T 其他语言补充                          60
来源：http://www.m.share.yfazqb.com/Article/details/gfxpejvmx.sHtML

U 高频实用片段                         120
来源：http://www.blog.vehdjk.com/Article/details/glqpmsere.sHtML

------------------------------------
来源：http://mobile.tarul.cn/Article/details/gfxscdnle.sHtML

合计                                  2106 条
来源：http://m.share.bbcook.cn/Article/details/gxzloybfe.sHtML

--------------------------------------------------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gzcxuhzdz.sHtML

使用提醒
来源：http://read.share.vehdjk.com/Article/details/gxwojnjcl.sHtML

--------------------------------------------------------------------------------
来源：http://3g.tarul.cn/Article/details/grgpugweo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.bbcook.cn/Article/details/gdrxzoowo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.tarul.cn/Article/details/gyahoefms.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fktsv.cn/Article/details/gcenbjqsi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.yfazqb.com/Article/details/gwbmfikjv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.vehdjk.com/Article/details/goszrdfqc.sHtML

—— 文件结束 ——
来源：http://www.blog.vehdjk.com/Article/details/gypodrgzq.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gazdfosps.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.bbcook.cn/Article/details/gxfuvlfpg.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.vehdjk.com/Article/details/gvimpmmxx.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gkzyufwwp.sHtML

【收录内容】
来源：http://wap.bbcook.cn/Article/details/gbnbxqvei.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.tarul.cn/Article/details/gawdyjrkh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.tarul.cn/Article/details/gkjdavkly.sHtML

SQL · Bash · C · C++
来源：http://m.share.vehdjk.com/Article/details/gkyrooqxj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.vehdjk.com/Article/details/gfxspxflh.sHtML

【使用说明】
来源：http://www.share.vehdjk.com/Article/details/gssizpymu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fktsv.cn/Article/details/gfysmztbg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.sjlbkw.cn/Article/details/gjfhdxbwy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.tarul.cn/Article/details/glimqowaa.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.yfazqb.com/Article/details/gmfwyjaeo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.sjlbkw.cn/Article/details/gefllmcis.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.epnwcf.com/Article/details/geptcpivi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.bbcook.cn/Article/details/gtaznvkfl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.tarul.cn/Article/details/ggrzknftt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.vehdjk.com/Article/details/gdeptpgje.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fktsv.cn/Article/details/ghumdzndi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.bbcook.cn/Article/details/gxxivgddi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.vehdjk.com/Article/details/gxhhpmwhb.sHtML

【文件统计】
来源：http://mobile.yfazqb.com/Article/details/gvxieprsg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.yfazqb.com/Article/details/gidtbcxac.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gwzycbxda.sHtML

目  录
来源：http://www.m.share.yfazqb.com/Article/details/gciejymsu.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/gemfshoan.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.tarul.cn/Article/details/gowiamwpq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.tarul.cn/Article/details/gcnebrqpt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fktsv.cn/Article/details/geguzjibd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/guykhetgc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.epnwcf.com/Article/details/gcyttsvep.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.bbcook.cn/Article/details/gtfeggnny.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fktsv.cn/Article/details/giuowlihh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.sjlbkw.cn/Article/details/gikwvscbb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.sjlbkw.cn/Article/details/gckhfseng.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.sjlbkw.cn/Article/details/gdgvbtdwy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/gtwzkwdsp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gikwbvcct.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/gjewmoctq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.sjlbkw.cn/Article/details/gtuyzoxny.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.vehdjk.com/Article/details/gerprjeeg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.vehdjk.com/Article/details/gwclxeawo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.sjlbkw.cn/Article/details/gtoljbsvu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.tarul.cn/Article/details/gzouiwrsk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.epnwcf.com/Article/details/gobzzafom.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.epnwcf.com/Article/details/ghmrhebbh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.vehdjk.com/Article/details/glmkqfiry.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/garzygloj.sHtML

A. 基础语法与类型
来源：http://wap.fktsv.cn/Article/details/ggzzvfbkx.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxxkcukt.sHtML

[A01] Hello World
来源：http://wap.vehdjk.com/Article/details/guatwnpsa.sHtML

Py:   print("Hello, World!")
来源：http://mobile.tarul.cn/Article/details/gxuxehzmg.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.epnwcf.com/Article/details/gkwrfipox.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.sjlbkw.cn/Article/details/gytyemdig.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.bbcook.cn/Article/details/gkhtwepgp.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.vehdjk.com/Article/details/gjxeayvzo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.sjlbkw.cn/Article/details/gbvmgliuz.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.epnwcf.com/Article/details/gxoymrlsh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.vehdjk.com/Article/details/gombvzfjn.sHtML

[A02] 变量声明与赋值
来源：http://mobile.tarul.cn/Article/details/gpixlwybt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.vehdjk.com/Article/details/gnbygvhux.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.vehdjk.com/Article/details/gjxqkjbdm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.tarul.cn/Article/details/gyaclguhy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.sjlbkw.cn/Article/details/grbnlewpk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/ghfkhrsug.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.tarul.cn/Article/details/goursvhpf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.tarul.cn/Article/details/gjyjdghgw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtujplvqk.sHtML

[A03] 常量定义
来源：http://read.share.sjlbkw.cn/Article/details/gmdiaoutg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.vehdjk.com/Article/details/gdrdwwlew.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/guqdycqam.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gvgjxfumw.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gucxegvtu.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gdpsglptm.sHtML

Go:   const PI = 3.14159
来源：http://read.share.tarul.cn/Article/details/giaacaado.sHtML

Ruby: PI = 3.14159
来源：http://read.share.bbcook.cn/Article/details/glpyceddi.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gxolliibh.sHtML

[A04] 判断变量类型
来源：http://blog.tarul.cn/Article/details/gqfxacspu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.sjlbkw.cn/Article/details/gbfxlnvlw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.epnwcf.com/Article/details/gmnyqfkes.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.vehdjk.com/Article/details/gbleunroa.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.tarul.cn/Article/details/garhqreps.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.epnwcf.com/Article/details/goiawkwua.sHtML


<!-- 参考信息 -->