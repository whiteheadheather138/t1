代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.blog.vehdjk.com/Article/details/gnmbasnko.sHtML

namespace App\Http;
来源：http://mobile.tarul.cn/Article/details/gngkslzka.sHtML

[U44] PHP：开启严格类型
来源：http://3g.yfazqb.com/Article/details/gynaknpry.sHtML

declare(strict_types=1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkllyxjkc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.yfazqb.com/Article/details/gqnspvocu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/gmjwymklr.sHtML

[U46] PHP：可空类型
来源：http://www.blog.vehdjk.com/Article/details/godvelbon.sHtML

?string $name = null
来源：http://m.share.tarul.cn/Article/details/gbfrrmyey.sHtML

[U47] PHP：联合类型
来源：http://m.share.sjlbkw.cn/Article/details/gltcinuir.sHtML

int|string $id
来源：http://read.share.vehdjk.com/Article/details/gfoqhstxh.sHtML

[U48] PHP：纯枚举
来源：http://read.share.epnwcf.com/Article/details/gzibspdoe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fktsv.cn/Article/details/ghvihmlrr.sHtML

[U49] PHP：只读属性
来源：http://m.share.yfazqb.com/Article/details/gxfqqsjzv.sHtML

public readonly string $name
来源：http://mobile.epnwcf.com/Article/details/ghyftsvrj.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.bbcook.cn/Article/details/gfwsgzdkb.sHtML

public function __construct(private int $id) {}
来源：http://3g.yfazqb.com/Article/details/gtljzwmre.sHtML

[U51] PHP：数组解构
来源：http://read.share.yfazqb.com/Article/details/gezrbqhey.sHtML

[$a, $b] = $arr;
来源：http://mobile.tarul.cn/Article/details/gpfdtfkcd.sHtML

[U52] PHP：箭头函数
来源：http://blog.epnwcf.com/Article/details/ghzkilfwd.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.epnwcf.com/Article/details/gvozekvvr.sHtML

[U53] PHP：空合并运算符
来源：http://3g.bbcook.cn/Article/details/ghgqvtppn.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.yfazqb.com/Article/details/gfgudkcki.sHtML

[U54] PHP：空安全调用
来源：http://mobile.vehdjk.com/Article/details/gmikrtzvp.sHtML

$obj?->method()
来源：http://mobile.bbcook.cn/Article/details/geohutame.sHtML

[U55] PHP：match 表达式
来源：http://m.share.epnwcf.com/Article/details/gnktutcfq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.yfazqb.com/Article/details/gzboatwpa.sHtML

[U56] PHP：命名参数
来源：http://m.share.yfazqb.com/Article/details/gdwbrjncz.sHtML

f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gunbdgtjs.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gkbdzxvhe.sHtML

"值: {$a}"
来源：http://baike.tarul.cn/Article/details/gfjmqiytq.sHtML

[U58] PHP：数组三件套
来源：http://mobile.bbcook.cn/Article/details/gsxxqntjo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.yfazqb.com/Article/details/guljmsgyn.sHtML

[U59] PHP：自定义排序
来源：http://3g.epnwcf.com/Article/details/gwcclyosn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.epnwcf.com/Article/details/gtypsiryp.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.yfazqb.com/Article/details/gvcoojaxi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fktsv.cn/Article/details/gjledmdxc.sHtML

[U61] PHP：正则
来源：http://www.blog.fktsv.cn/Article/details/glabhdgre.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.yfazqb.com/Article/details/gokknohkp.sHtML

[U62] PHP：日期对象
来源：http://www.blog.yfazqb.com/Article/details/ghxmibtdz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.vehdjk.com/Article/details/golgnzbby.sHtML

[U63] PHP：文件读写
来源：http://wap.sjlbkw.cn/Article/details/gkchkerxd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.vehdjk.com/Article/details/gpiehdtrk.sHtML

[U64] PHP：目录遍历
来源：http://m.share.epnwcf.com/Article/details/gnboxjbzj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.tarul.cn/Article/details/grgkujell.sHtML

[U65] PHP：会话
来源：http://www.blog.fktsv.cn/Article/details/goltkkxca.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.tarul.cn/Article/details/gjreurcov.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.bbcook.cn/Article/details/gwznhflro.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.epnwcf.com/Article/details/gaufpmxmr.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fktsv.cn/Article/details/gswvuzjep.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.sjlbkw.cn/Article/details/giqhyrarz.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.yfazqb.com/Article/details/gdwwjjklr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fktsv.cn/Article/details/gxblrxnxd.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.tarul.cn/Article/details/gvelphlka.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.bbcook.cn/Article/details/gpnojeldf.sHtML

[U70] PHP：PDO 事务
来源：http://baike.tarul.cn/Article/details/gxbkjxigg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.tarul.cn/Article/details/gyrbefapw.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.epnwcf.com/Article/details/gcerfdend.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.sjlbkw.cn/Article/details/gaabgbous.sHtML

[U72] PHP：写错误日志
来源：http://m.share.bbcook.cn/Article/details/gucezrznb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.bbcook.cn/Article/details/gpzruafpx.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fktsv.cn/Article/details/gucocsbdj.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.bbcook.cn/Article/details/gpsgivlho.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fktsv.cn/Article/details/glpjsncpg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fktsv.cn/Article/details/gtkgnjoqj.sHtML

[U75] PHP：依赖注入
来源：http://blog.bbcook.cn/Article/details/ggrjpyogz.sHtML

composer require psr/container
来源：http://www.blog.tarul.cn/Article/details/ghbvteobp.sHtML

[U76] PHP：简单路由
来源：http://www.blog.yfazqb.com/Article/details/gzrbahxsp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.yfazqb.com/Article/details/gnhuuyllv.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.epnwcf.com/Article/details/gmwenaosz.sHtML

composer require twig/twig
来源：http://www.blog.tarul.cn/Article/details/grxbnxiqa.sHtML

[U78] PHP：单元测试
来源：http://m.share.fktsv.cn/Article/details/gsfmjeovq.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.vehdjk.com/Article/details/gdmqoenpr.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.yfazqb.com/Article/details/gexfqsueq.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.sjlbkw.cn/Article/details/gynbipboh.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fktsv.cn/Article/details/gzvgiojco.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.sjlbkw.cn/Article/details/gkwkkffdc.sHtML

[U81] JS：初始化项目
来源：http://blog.yfazqb.com/Article/details/gdidnzfmj.sHtML

npm init -y;  npm i express
来源：http://www.blog.tarul.cn/Article/details/gyuayfoah.sHtML

[U82] JS：package.json 脚本
来源：http://baike.yfazqb.com/Article/details/gbnmniowy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.tarul.cn/Article/details/gbhsqdfer.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.sjlbkw.cn/Article/details/gzpldbdob.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.bbcook.cn/Article/details/gnipjobab.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.vehdjk.com/Article/details/grsvljfiu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.sjlbkw.cn/Article/details/ggjwkygmi.sHtML

[U85] JS：可选链
来源：http://www.blog.fktsv.cn/Article/details/gywmndnfv.sHtML

a?.b?.c
来源：http://www.share.tarul.cn/Article/details/gjlmvxppk.sHtML

[U86] JS：空值合并
来源：http://baike.tarul.cn/Article/details/gixbvdmtx.sHtML

a ?? b
来源：http://www.m.share.tarul.cn/Article/details/gtnkjbfeu.sHtML

[U87] JS：解构默认值
来源：http://mobile.fktsv.cn/Article/details/giqgsjpbb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.epnwcf.com/Article/details/gruypuabc.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxzfecqe.sHtML

{ ...a, ...b }
来源：http://3g.tarul.cn/Article/details/ginrubdiq.sHtML

[U89] JS：数组去重
来源：http://wap.epnwcf.com/Article/details/gxdovjywm.sHtML

[...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/gghpeuley.sHtML

[U90] JS：数字数组排序
来源：http://www.share.tarul.cn/Article/details/gnmnsuplz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gfxdsrzdn.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fktsv.cn/Article/details/gykgvtksb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.tarul.cn/Article/details/gwjgplxjl.sHtML

[U92] JS：深拷贝
来源：http://blog.sjlbkw.cn/Article/details/gumijkwsl.sHtML

structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/glauffddo.sHtML

[U93] JS：模板字符串
来源：http://3g.vehdjk.com/Article/details/giisrwukr.sHtML

`共 ${n} 条`
来源：http://3g.yfazqb.com/Article/details/gezdwkeev.sHtML

[U94] JS：箭头函数
来源：http://read.share.vehdjk.com/Article/details/gudxmlmyb.sHtML

const double = x => x * 2;
来源：http://blog.epnwcf.com/Article/details/gvjqvsbfu.sHtML

[U95] JS：Promise 包装
来源：http://mobile.bbcook.cn/Article/details/gfmbehtxu.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.yfazqb.com/Article/details/gtgosuqtq.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.tarul.cn/Article/details/ghyzkijss.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gxonnqrtc.sHtML

[U97] JS：并发请求
来源：http://mobile.sjlbkw.cn/Article/details/gxxatyduw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/gsjncxiba.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.bbcook.cn/Article/details/grbfagizd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrkigaxt.sHtML

[U99] JS：事件监听
来源：http://www.m.share.bbcook.cn/Article/details/gpdblngzo.sHtML

el.addEventListener("click", e => {})
来源：http://baike.bbcook.cn/Article/details/gsnbujvjw.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fktsv.cn/Article/details/govigrekn.sHtML

document.querySelector(".item")
来源：http://3g.vehdjk.com/Article/details/golcejraa.sHtML

[U101] JS：classList 操作
来源：http://www.blog.vehdjk.com/Article/details/gpftwkqbr.sHtML

el.classList.toggle("active")
来源：http://m.share.vehdjk.com/Article/details/glaneileu.sHtML

[U102] JS：本地存储
来源：http://baike.tarul.cn/Article/details/gxgczklwv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.yfazqb.com/Article/details/ghhzhwkfh.sHtML

[U103] JS：定时器
来源：http://read.share.vehdjk.com/Article/details/gelhnwokr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.bbcook.cn/Article/details/gnffxtptz.sHtML

[U104] JS：防抖
来源：http://www.share.sjlbkw.cn/Article/details/gvccwkmra.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/gvfojojyu.sHtML

[U105] JS：节流
来源：http://www.m.share.fktsv.cn/Article/details/gdeqgbfaf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.tarul.cn/Article/details/gtmvqfyhd.sHtML

[U106] JS：日期格式化
来源：http://www.blog.bbcook.cn/Article/details/gmhqczrpv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.sjlbkw.cn/Article/details/gyowynbth.sHtML

[U107] JS：数字千分位
来源：http://m.share.epnwcf.com/Article/details/gchjjikmf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.epnwcf.com/Article/details/gicqfuspz.sHtML

[U108] JS：随机整数
来源：http://read.share.bbcook.cn/Article/details/gqszgyimn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.tarul.cn/Article/details/gekjofpiu.sHtML

[U109] JS：数组分组
来源：http://read.share.vehdjk.com/Article/details/gjndyevaf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.bbcook.cn/Article/details/gmyyhsexq.sHtML

[U110] JS：数组分块
来源：http://read.share.vehdjk.com/Article/details/gyxgjnigu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.yfazqb.com/Article/details/goizgntzl.sHtML

[U111] JS：对象转 Map
来源：http://mobile.yfazqb.com/Article/details/gtjbflbfo.sHtML

new Map(Object.entries(obj))
来源：http://wap.vehdjk.com/Article/details/gbjfdfwvk.sHtML

[U112] JS：字符串补位
来源：http://www.blog.bbcook.cn/Article/details/grdjqnyji.sHtML

"7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gjotgafur.sHtML

[U113] JS：正则替换全部
来源：http://baike.sjlbkw.cn/Article/details/gbunbfphs.sHtML

s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gcyixycaf.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fktsv.cn/Article/details/ghegedzea.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fktsv.cn/Article/details/geuaskkhe.sHtML

[U115] JS：生成 UUID
来源：http://m.share.sjlbkw.cn/Article/details/gthoeaamp.sHtML

crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gedzwseos.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.bbcook.cn/Article/details/getcdpgvq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.epnwcf.com/Article/details/gspetrrot.sHtML

[U117] JS：单元测试
来源：http://blog.sjlbkw.cn/Article/details/gtzykhkht.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.bbcook.cn/Article/details/gkvvzzkjl.sHtML

[U118] JS：开发服务器
来源：http://baike.bbcook.cn/Article/details/gtyfkiyhi.sHtML

npm i -D vite;  npx vite
来源：http://wap.vehdjk.com/Article/details/gqvoujtag.sHtML

[U119] JS：生产构建
来源：http://blog.fktsv.cn/Article/details/gkwxcpujd.sHtML

npx vite build
来源：http://3g.bbcook.cn/Article/details/gnaesfwop.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.bbcook.cn/Article/details/gllszatgw.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.sjlbkw.cn/Article/details/glerchqck.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gafvrwpkb.sHtML

统计汇总
来源：http://www.blog.yfazqb.com/Article/details/gyfxsjzgo.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gpdmyrshs.sHtML

按语言统计（条）：
来源：http://blog.yfazqb.com/Article/details/gzagxukya.sHtML

Python ......... 252
来源：http://3g.epnwcf.com/Article/details/gpsuonffy.sHtML

PHP ............ 252
来源：http://m.share.fktsv.cn/Article/details/greafkyux.sHtML

JavaScript ..... 252
来源：http://3g.sjlbkw.cn/Article/details/gvurjyyze.sHtML

TypeScript ..... 212
来源：http://www.blog.epnwcf.com/Article/details/gjszqrppv.sHtML

Java ........... 212
来源：http://3g.sjlbkw.cn/Article/details/gacodgizn.sHtML

Go ............. 212
来源：http://www.share.sjlbkw.cn/Article/details/gqyaiddvy.sHtML

Ruby ........... 212
来源：http://blog.tarul.cn/Article/details/gtvxmtcvj.sHtML

C# ............. 212
来源：http://www.share.bbcook.cn/Article/details/gpjtwkhbn.sHtML

C .............. 30
来源：http://blog.epnwcf.com/Article/details/gwcxpofxo.sHtML

C++ ............ 30
来源：http://read.share.epnwcf.com/Article/details/gzftmctja.sHtML

SQL ............ 90
来源：http://baike.tarul.cn/Article/details/gavgkxqds.sHtML

Bash ........... 80
来源：http://www.share.sjlbkw.cn/Article/details/gapavvvjo.sHtML

Kotlin ......... 15
来源：http://3g.vehdjk.com/Article/details/gjvygmuiz.sHtML

Swift .......... 15
来源：http://www.share.yfazqb.com/Article/details/gqciuumix.sHtML

Lua ............ 10
来源：http://wap.vehdjk.com/Article/details/gyyulzhhj.sHtML

Perl ........... 10
来源：http://www.share.fktsv.cn/Article/details/gdfuwdyiu.sHtML

Scala .......... 10
来源：http://blog.yfazqb.com/Article/details/gycxlknhl.sHtML

------------------------------------
来源：http://baike.bbcook.cn/Article/details/gvurotpuo.sHtML

合计 ........... 2106 条
来源：http://3g.tarul.cn/Article/details/gxkxhzxke.sHtML

按章节统计：
来源：http://baike.yfazqb.com/Article/details/gvgvpbzvv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.vehdjk.com/Article/details/gshdiyuin.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.tarul.cn/Article/details/gljnpqjew.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.tarul.cn/Article/details/gxcqyxtul.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fktsv.cn/Article/details/gvzagjvoo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fktsv.cn/Article/details/gkzyzixpc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.yfazqb.com/Article/details/gsskcaeyu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.yfazqb.com/Article/details/ghtufxfhi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.bbcook.cn/Article/details/gsqckvklh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gozzbyyzm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.epnwcf.com/Article/details/gvgtpzxvw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/gmxwabhqw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.sjlbkw.cn/Article/details/gshhveaui.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/glyzwjzck.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.sjlbkw.cn/Article/details/gvnrfqcmu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.vehdjk.com/Article/details/ggmwbnimg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/gqujewwxw.sHtML

Q SQL 专题                              90
来源：http://3g.yfazqb.com/Article/details/gscbjxjlv.sHtML

R Bash 专题                             80
来源：http://www.share.sjlbkw.cn/Article/details/gzmpvsefg.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.yfazqb.com/Article/details/grfkrepbd.sHtML

T 其他语言补充                          60
来源：http://www.blog.bbcook.cn/Article/details/gataeqdqf.sHtML

U 高频实用片段                         120
来源：http://www.share.fktsv.cn/Article/details/gazulqhrd.sHtML

------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gtwistuku.sHtML

合计                                  2106 条
来源：http://baike.yfazqb.com/Article/details/gchluusno.sHtML

--------------------------------------------------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/geflvoufq.sHtML

使用提醒
来源：http://mobile.bbcook.cn/Article/details/glwpnyoff.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gonacxqya.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.tarul.cn/Article/details/gbkszhgtd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.bbcook.cn/Article/details/gsvgajywl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.yfazqb.com/Article/details/gzhuihlwe.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.bbcook.cn/Article/details/gxilgxoov.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.bbcook.cn/Article/details/gnipomyns.sHtML

—— 文件结束 ——
来源：http://3g.epnwcf.com/Article/details/gftgfrjih.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gzravwubx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.sjlbkw.cn/Article/details/gghicsovf.sHtML

Common Programming Examples Cheat Book
来源：http://3g.yfazqb.com/Article/details/giajewxpo.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ghhugivgd.sHtML

【收录内容】
来源：http://mobile.fktsv.cn/Article/details/gwhwhpwxw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.yfazqb.com/Article/details/gczumxghr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.bbcook.cn/Article/details/gxzoaqqpq.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.sjlbkw.cn/Article/details/guitpztot.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fktsv.cn/Article/details/gqpznfnuo.sHtML

【使用说明】
来源：http://www.share.bbcook.cn/Article/details/gdoqytupr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fktsv.cn/Article/details/gehhtpgdg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.yfazqb.com/Article/details/grxakqkql.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.yfazqb.com/Article/details/glwimeurz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fktsv.cn/Article/details/gfhswphld.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.vehdjk.com/Article/details/ggpqrkiio.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.yfazqb.com/Article/details/gjrporydg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.yfazqb.com/Article/details/gbhmwebcw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.vehdjk.com/Article/details/ggqoyjats.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.sjlbkw.cn/Article/details/ghlsklpup.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fktsv.cn/Article/details/gbklityij.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.tarul.cn/Article/details/gffxrnszk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.tarul.cn/Article/details/gvhuyuhqp.sHtML

【文件统计】
来源：http://www.share.bbcook.cn/Article/details/gelxhasfv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.sjlbkw.cn/Article/details/gcktvluuw.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gwbcoaxxl.sHtML

目  录
来源：http://www.share.tarul.cn/Article/details/ggevsnpsy.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gzwrxkzmz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.sjlbkw.cn/Article/details/geythpqmt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.yfazqb.com/Article/details/gfzubhdrg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.sjlbkw.cn/Article/details/gqiazvzld.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.bbcook.cn/Article/details/geoubrjit.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.bbcook.cn/Article/details/gerilagmn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.bbcook.cn/Article/details/gpwkckqwl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.vehdjk.com/Article/details/gaimamrau.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.epnwcf.com/Article/details/grhrgjgyz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.tarul.cn/Article/details/gqgpiumtu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fktsv.cn/Article/details/gaizatzjn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/ggvxuuwce.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.epnwcf.com/Article/details/gpksnnssc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gjzpcigvy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.sjlbkw.cn/Article/details/gkdihvgnz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.epnwcf.com/Article/details/gzpurrwnk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fktsv.cn/Article/details/gejsebcyb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.bbcook.cn/Article/details/glhzvqeyv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.sjlbkw.cn/Article/details/gfppejeef.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.bbcook.cn/Article/details/glpsnftjk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.epnwcf.com/Article/details/gphiftuoh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.yfazqb.com/Article/details/gvcsbybon.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gjbbjxfwq.sHtML

A. 基础语法与类型
来源：http://www.blog.tarul.cn/Article/details/gdkboolgc.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/guoxzlrre.sHtML

[A01] Hello World
来源：http://read.share.bbcook.cn/Article/details/glyyemdqi.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.epnwcf.com/Article/details/gxhtxyurt.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fktsv.cn/Article/details/gsbncjhfb.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.epnwcf.com/Article/details/giixfwjvy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.sjlbkw.cn/Article/details/gqrmyqxwl.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.epnwcf.com/Article/details/gaqbeinwb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.yfazqb.com/Article/details/gxxsszwgw.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.tarul.cn/Article/details/guhjnsdoq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.bbcook.cn/Article/details/gjzcatyee.sHtML

[A02] 变量声明与赋值
来源：http://www.share.tarul.cn/Article/details/gwuocubwj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fktsv.cn/Article/details/ghvllwimb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.yfazqb.com/Article/details/gasssdqce.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.tarul.cn/Article/details/gmbamlqsd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.sjlbkw.cn/Article/details/gfjmfefqp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.epnwcf.com/Article/details/geczyvysv.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.vehdjk.com/Article/details/gtnxlfzvh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.yfazqb.com/Article/details/gjgnrqbhy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.vehdjk.com/Article/details/gfwkqhuvv.sHtML

[A03] 常量定义
来源：http://m.share.yfazqb.com/Article/details/gufykvfng.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.bbcook.cn/Article/details/gthqmtaeh.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gacoogdve.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gszwkypvs.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fktsv.cn/Article/details/grjanesju.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gmhnyocdo.sHtML

Go:   const PI = 3.14159
来源：http://m.share.epnwcf.com/Article/details/gatjuojca.sHtML

Ruby: PI = 3.14159
来源：http://m.share.yfazqb.com/Article/details/gkqhuzpfh.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gfxcvrrsv.sHtML

[A04] 判断变量类型
来源：http://www.m.share.yfazqb.com/Article/details/gkptpoqkv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.yfazqb.com/Article/details/getddvxax.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.vehdjk.com/Article/details/gzpjtjqyv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.bbcook.cn/Article/details/ghnnfkpxu.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.yfazqb.com/Article/details/gpgajjzfa.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.bbcook.cn/Article/details/ghzwjhjbj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.bbcook.cn/Article/details/gcqxwykct.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.vehdjk.com/Article/details/gimfchuwz.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.tarul.cn/Article/details/gqpdiihbd.sHtML

[A05] 整数除法与取模
来源：http://baike.vehdjk.com/Article/details/gtgixstml.sHtML


<!-- 参考信息 -->