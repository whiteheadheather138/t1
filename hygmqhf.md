代发 wailian999

[U43] PHP：声明命名空间
来源：http://3g.fktsv.cn/Article/details/goxupgsqb.sHtML

namespace App\Http;
来源：http://www.m.share.bbcook.cn/Article/details/gtbwpbkpn.sHtML

[U44] PHP：开启严格类型
来源：http://baike.tarul.cn/Article/details/gvcqgkfcd.sHtML

declare(strict_types=1);
来源：http://www.m.share.vehdjk.com/Article/details/gqvkbuliw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.tarul.cn/Article/details/gucqedsqb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gneseflhx.sHtML

[U46] PHP：可空类型
来源：http://blog.tarul.cn/Article/details/givenoprk.sHtML

?string $name = null
来源：http://www.share.bbcook.cn/Article/details/gunyugfqk.sHtML

[U47] PHP：联合类型
来源：http://www.share.epnwcf.com/Article/details/gapydusyb.sHtML

int|string $id
来源：http://baike.sjlbkw.cn/Article/details/gryyquzsa.sHtML

[U48] PHP：纯枚举
来源：http://baike.bbcook.cn/Article/details/guerqofue.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.vehdjk.com/Article/details/goyqbklbw.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.bbcook.cn/Article/details/gwyqydqle.sHtML

public readonly string $name
来源：http://wap.yfazqb.com/Article/details/gfpotfroa.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.vehdjk.com/Article/details/gpbueebls.sHtML

public function __construct(private int $id) {}
来源：http://blog.tarul.cn/Article/details/gvylvdcsp.sHtML

[U51] PHP：数组解构
来源：http://www.blog.yfazqb.com/Article/details/gpwbvrpua.sHtML

[$a, $b] = $arr;
来源：http://blog.epnwcf.com/Article/details/ggssnnpmr.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.bbcook.cn/Article/details/goipxvxhy.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.vehdjk.com/Article/details/gidjvfewq.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.bbcook.cn/Article/details/gdtcnwisu.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fktsv.cn/Article/details/gehptpfew.sHtML

[U54] PHP：空安全调用
来源：http://blog.fktsv.cn/Article/details/gbxjhypnb.sHtML

$obj?->method()
来源：http://3g.yfazqb.com/Article/details/gezdlccrn.sHtML

[U55] PHP：match 表达式
来源：http://www.share.vehdjk.com/Article/details/gqeoehhqe.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.bbcook.cn/Article/details/gyaqelzuo.sHtML

[U56] PHP：命名参数
来源：http://3g.bbcook.cn/Article/details/grkdhvvkt.sHtML

f(a: 1, b: 2)
来源：http://www.share.sjlbkw.cn/Article/details/gyzgpphqx.sHtML

[U57] PHP：字符串插值
来源：http://baike.fktsv.cn/Article/details/gxhotxtku.sHtML

"值: {$a}"
来源：http://mobile.fktsv.cn/Article/details/gmqnchmrp.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.bbcook.cn/Article/details/gbrtdlkct.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.bbcook.cn/Article/details/gnynxmbsr.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.bbcook.cn/Article/details/gttwptygg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fktsv.cn/Article/details/gfkylhxpm.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.vehdjk.com/Article/details/goinzrtkn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.yfazqb.com/Article/details/gvlepqzgz.sHtML

[U61] PHP：正则
来源：http://baike.vehdjk.com/Article/details/gkxcqsazp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.epnwcf.com/Article/details/gdgwknawd.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.yfazqb.com/Article/details/ghasgtixm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.vehdjk.com/Article/details/gbbbkqbpm.sHtML

[U63] PHP：文件读写
来源：http://wap.tarul.cn/Article/details/getpdcsyc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fktsv.cn/Article/details/gauigcxhk.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fktsv.cn/Article/details/goqyekwpa.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fktsv.cn/Article/details/gdhbgvdwn.sHtML

[U65] PHP：会话
来源：http://3g.sjlbkw.cn/Article/details/gilxuqdlk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.yfazqb.com/Article/details/gzablwshd.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.vehdjk.com/Article/details/gfioydsok.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.vehdjk.com/Article/details/gyitehhaf.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.tarul.cn/Article/details/gvvlmyduq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.sjlbkw.cn/Article/details/glhcmipbo.sHtML

[U68] PHP：PDO 连接
来源：http://baike.epnwcf.com/Article/details/gnlnupajp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.tarul.cn/Article/details/geconwmif.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.tarul.cn/Article/details/guavmpuoc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.epnwcf.com/Article/details/goebkfrab.sHtML

[U70] PHP：PDO 事务
来源：http://wap.yfazqb.com/Article/details/gsaujwydj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.sjlbkw.cn/Article/details/gsmthadmj.sHtML

[U71] PHP：抛出异常
来源：http://www.share.yfazqb.com/Article/details/gfhoecptn.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.sjlbkw.cn/Article/details/guursigwp.sHtML

[U72] PHP：写错误日志
来源：http://blog.tarul.cn/Article/details/gkvjvnhrn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.sjlbkw.cn/Article/details/gttdrgnhh.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fktsv.cn/Article/details/giotihlsg.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.yfazqb.com/Article/details/gfgvwuscn.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gmhrwnica.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.bbcook.cn/Article/details/gklowikyo.sHtML

[U75] PHP：依赖注入
来源：http://3g.epnwcf.com/Article/details/gbpdvjdvp.sHtML

composer require psr/container
来源：http://mobile.bbcook.cn/Article/details/giaetcspp.sHtML

[U76] PHP：简单路由
来源：http://www.blog.epnwcf.com/Article/details/gchktejbz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.vehdjk.com/Article/details/gwnzqbcpo.sHtML

[U77] PHP：模板渲染
来源：http://3g.tarul.cn/Article/details/gcygyebdw.sHtML

composer require twig/twig
来源：http://www.m.share.fktsv.cn/Article/details/gcscrmcpy.sHtML

[U78] PHP：单元测试
来源：http://baike.tarul.cn/Article/details/gwxoqcjcv.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.bbcook.cn/Article/details/gjnpvfnqt.sHtML

[U79] PHP：静态分析
来源：http://mobile.tarul.cn/Article/details/grjhyntra.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.vehdjk.com/Article/details/gcalasqyc.sHtML

[U80] PHP：代码规范修复
来源：http://blog.tarul.cn/Article/details/gidcnafxd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.bbcook.cn/Article/details/gymlgozjg.sHtML

[U81] JS：初始化项目
来源：http://read.share.bbcook.cn/Article/details/gflabeuvc.sHtML

npm init -y;  npm i express
来源：http://baike.sjlbkw.cn/Article/details/gcrfjklow.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fktsv.cn/Article/details/gjanywexg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.yfazqb.com/Article/details/gpyuhxwjc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.vehdjk.com/Article/details/gdhuxxabk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.bbcook.cn/Article/details/gcjvgbouk.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.vehdjk.com/Article/details/gnwzbggbe.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fktsv.cn/Article/details/glrkarkgc.sHtML

[U85] JS：可选链
来源：http://www.blog.yfazqb.com/Article/details/gmiilzaws.sHtML

a?.b?.c
来源：http://m.share.epnwcf.com/Article/details/gvauikuvi.sHtML

[U86] JS：空值合并
来源：http://wap.tarul.cn/Article/details/gaazzvbsz.sHtML

a ?? b
来源：http://www.m.share.epnwcf.com/Article/details/gyvtowvzp.sHtML

[U87] JS：解构默认值
来源：http://read.share.yfazqb.com/Article/details/gguiorbhl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fktsv.cn/Article/details/gtcrkmnpu.sHtML

[U88] JS：对象展开合并
来源：http://www.share.epnwcf.com/Article/details/ggurjkrwx.sHtML

{ ...a, ...b }
来源：http://www.blog.fktsv.cn/Article/details/gsacxhlic.sHtML

[U89] JS：数组去重
来源：http://mobile.vehdjk.com/Article/details/gcqslrlas.sHtML

[...new Set(arr)]
来源：http://www.m.share.fktsv.cn/Article/details/glfqavcok.sHtML

[U90] JS：数字数组排序
来源：http://baike.bbcook.cn/Article/details/gerrbaxyq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.yfazqb.com/Article/details/ggpsilsep.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fktsv.cn/Article/details/gdcueqgir.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.epnwcf.com/Article/details/gkulbhdhh.sHtML

[U92] JS：深拷贝
来源：http://3g.epnwcf.com/Article/details/gextqiyei.sHtML

structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gpdfqkjpw.sHtML

[U93] JS：模板字符串
来源：http://m.share.vehdjk.com/Article/details/ghpiltefs.sHtML

`共 ${n} 条`
来源：http://3g.fktsv.cn/Article/details/gazdwlnsj.sHtML

[U94] JS：箭头函数
来源：http://baike.tarul.cn/Article/details/gwzksfsvw.sHtML

const double = x => x * 2;
来源：http://mobile.sjlbkw.cn/Article/details/gkacahuxq.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.tarul.cn/Article/details/ghhzryumz.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.yfazqb.com/Article/details/gwpdulxiw.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.vehdjk.com/Article/details/gceypdqyb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.epnwcf.com/Article/details/gturbpdys.sHtML

[U97] JS：并发请求
来源：http://3g.epnwcf.com/Article/details/gszorbqgu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gilljtpix.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.bbcook.cn/Article/details/gukrkljxf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.sjlbkw.cn/Article/details/gjlebagpt.sHtML

[U99] JS：事件监听
来源：http://3g.vehdjk.com/Article/details/gwswtrtzn.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fktsv.cn/Article/details/gytcplyji.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.sjlbkw.cn/Article/details/gdediowff.sHtML

document.querySelector(".item")
来源：http://www.share.fktsv.cn/Article/details/getjdzznh.sHtML

[U101] JS：classList 操作
来源：http://mobile.bbcook.cn/Article/details/gkhibjtaj.sHtML

el.classList.toggle("active")
来源：http://read.share.vehdjk.com/Article/details/gkuijowwc.sHtML

[U102] JS：本地存储
来源：http://www.m.share.yfazqb.com/Article/details/grdjwstaf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fktsv.cn/Article/details/ghhnmpkkt.sHtML

[U103] JS：定时器
来源：http://www.m.share.fktsv.cn/Article/details/gxmrnereh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.yfazqb.com/Article/details/gaqtgtipg.sHtML

[U104] JS：防抖
来源：http://blog.vehdjk.com/Article/details/gscurpurl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/giyiqkxqa.sHtML

[U105] JS：节流
来源：http://www.share.sjlbkw.cn/Article/details/gmdbklwiq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.bbcook.cn/Article/details/groszpoqh.sHtML

[U106] JS：日期格式化
来源：http://www.share.epnwcf.com/Article/details/gzryllreq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.yfazqb.com/Article/details/gjgesurpw.sHtML

[U107] JS：数字千分位
来源：http://www.blog.yfazqb.com/Article/details/gqqtlforb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.bbcook.cn/Article/details/gclfqkfgb.sHtML

[U108] JS：随机整数
来源：http://mobile.tarul.cn/Article/details/gplopuydh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.vehdjk.com/Article/details/grjxnenuw.sHtML

[U109] JS：数组分组
来源：http://www.blog.tarul.cn/Article/details/gpncldxaj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.yfazqb.com/Article/details/gqjdxdswj.sHtML

[U110] JS：数组分块
来源：http://mobile.yfazqb.com/Article/details/gohfdrfhl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.tarul.cn/Article/details/gvyqofjip.sHtML

[U111] JS：对象转 Map
来源：http://baike.yfazqb.com/Article/details/giaepvlly.sHtML

new Map(Object.entries(obj))
来源：http://m.share.epnwcf.com/Article/details/gdmjsjbup.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.bbcook.cn/Article/details/gadvnzgea.sHtML

"7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/gbbsxbfif.sHtML

[U113] JS：正则替换全部
来源：http://blog.yfazqb.com/Article/details/grpehsykw.sHtML

s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/grtfiagyh.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.tarul.cn/Article/details/gorjwalsv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fktsv.cn/Article/details/gqulwqjgq.sHtML

[U115] JS：生成 UUID
来源：http://3g.fktsv.cn/Article/details/ghgtmeozv.sHtML

crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/guzbdxvds.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.vehdjk.com/Article/details/gemdqstqf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.vehdjk.com/Article/details/glalvuufz.sHtML

[U117] JS：单元测试
来源：http://www.blog.sjlbkw.cn/Article/details/ghjhtyjmz.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.yfazqb.com/Article/details/gvksvqarl.sHtML

[U118] JS：开发服务器
来源：http://www.blog.yfazqb.com/Article/details/gkmvhksjc.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fktsv.cn/Article/details/gyeegtszm.sHtML

[U119] JS：生产构建
来源：http://read.share.bbcook.cn/Article/details/gdkwwfgcg.sHtML

npx vite build
来源：http://www.blog.sjlbkw.cn/Article/details/gpjfhfmsc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.vehdjk.com/Article/details/gzhrjxgrf.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.epnwcf.com/Article/details/gkzfqqxqs.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gzplrbbrg.sHtML

统计汇总
来源：http://m.share.yfazqb.com/Article/details/gwerlbknq.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gkrbzgpoz.sHtML

按语言统计（条）：
来源：http://www.blog.tarul.cn/Article/details/gqisoqmfa.sHtML

Python ......... 252
来源：http://www.m.share.yfazqb.com/Article/details/gxpisufcj.sHtML

PHP ............ 252
来源：http://www.share.tarul.cn/Article/details/gtfmhjcyk.sHtML

JavaScript ..... 252
来源：http://wap.yfazqb.com/Article/details/gposbsqns.sHtML

TypeScript ..... 212
来源：http://www.blog.bbcook.cn/Article/details/gcpdqyjux.sHtML

Java ........... 212
来源：http://wap.bbcook.cn/Article/details/geeujsejp.sHtML

Go ............. 212
来源：http://www.share.epnwcf.com/Article/details/gseukmrrp.sHtML

Ruby ........... 212
来源：http://blog.epnwcf.com/Article/details/gpktddrwn.sHtML

C# ............. 212
来源：http://read.share.fktsv.cn/Article/details/gcoukaeuk.sHtML

C .............. 30
来源：http://wap.tarul.cn/Article/details/gdiowsudh.sHtML

C++ ............ 30
来源：http://wap.yfazqb.com/Article/details/gxejjtbhx.sHtML

SQL ............ 90
来源：http://m.share.epnwcf.com/Article/details/gixelomqd.sHtML

Bash ........... 80
来源：http://www.share.epnwcf.com/Article/details/gbjirbfgr.sHtML

Kotlin ......... 15
来源：http://m.share.tarul.cn/Article/details/genbsgbei.sHtML

Swift .......... 15
来源：http://read.share.epnwcf.com/Article/details/gkjttkbyz.sHtML

Lua ............ 10
来源：http://baike.sjlbkw.cn/Article/details/gpbhqwzlk.sHtML

Perl ........... 10
来源：http://blog.yfazqb.com/Article/details/gfbbawefa.sHtML

Scala .......... 10
来源：http://www.blog.fktsv.cn/Article/details/gvxnvkwux.sHtML

------------------------------------
来源：http://blog.epnwcf.com/Article/details/gowijemrk.sHtML

合计 ........... 2106 条
来源：http://www.m.share.tarul.cn/Article/details/gbubegnkj.sHtML

按章节统计：
来源：http://www.m.share.tarul.cn/Article/details/gsyuxluzo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.bbcook.cn/Article/details/gjrfeyhki.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.tarul.cn/Article/details/gtvyeudmk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.tarul.cn/Article/details/gjmsrcjrg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.tarul.cn/Article/details/gfyjhttor.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.tarul.cn/Article/details/ghwkmwehs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.tarul.cn/Article/details/glymhhgpl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.epnwcf.com/Article/details/gzrctcbqq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.yfazqb.com/Article/details/gvptsfmnt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gcidpomts.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.yfazqb.com/Article/details/gxfoklens.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.tarul.cn/Article/details/ghnlcfagg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fktsv.cn/Article/details/gicixkeec.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gytoftzhv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.bbcook.cn/Article/details/gsngbdtct.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.yfazqb.com/Article/details/goqbfwcoa.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gmoinxyqi.sHtML

Q SQL 专题                              90
来源：http://m.share.vehdjk.com/Article/details/gavpdfgpi.sHtML

R Bash 专题                             80
来源：http://blog.bbcook.cn/Article/details/gdndxrhsd.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.sjlbkw.cn/Article/details/gevinwdmv.sHtML

T 其他语言补充                          60
来源：http://baike.bbcook.cn/Article/details/gotmefpzr.sHtML

U 高频实用片段                         120
来源：http://www.blog.vehdjk.com/Article/details/gdjfekczt.sHtML

------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/ghfhrodxq.sHtML

合计                                  2106 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gzftwhkkc.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/gipfpgqop.sHtML

使用提醒
来源：http://wap.epnwcf.com/Article/details/gcbivmfqu.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gyhnbrbhh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fktsv.cn/Article/details/ghscexfde.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.tarul.cn/Article/details/godnoerqk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fktsv.cn/Article/details/gzgiyyihw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.epnwcf.com/Article/details/gtyidnzbf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fktsv.cn/Article/details/gyupntedr.sHtML

—— 文件结束 ——
来源：http://m.share.tarul.cn/Article/details/gngnevhef.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/geffeiofh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.bbcook.cn/Article/details/gmxoviltc.sHtML

Common Programming Examples Cheat Book
来源：http://blog.vehdjk.com/Article/details/gcpwaoxrw.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gbatseghh.sHtML

【收录内容】
来源：http://m.share.yfazqb.com/Article/details/gzjentgtv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.epnwcf.com/Article/details/gulbjqsrz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.tarul.cn/Article/details/gbkfseuse.sHtML

SQL · Bash · C · C++
来源：http://3g.tarul.cn/Article/details/gevcypoyd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.sjlbkw.cn/Article/details/ghblrjniu.sHtML

【使用说明】
来源：http://blog.yfazqb.com/Article/details/gfvdywbgf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.yfazqb.com/Article/details/gmqhlgiok.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.bbcook.cn/Article/details/ghlaveyto.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.bbcook.cn/Article/details/gbhkpyvto.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.tarul.cn/Article/details/gkkddnlol.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.bbcook.cn/Article/details/gizhhiyxb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.yfazqb.com/Article/details/guexsuvfc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.tarul.cn/Article/details/gurcoexxr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.tarul.cn/Article/details/gowgbzslz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.bbcook.cn/Article/details/gphiozrdn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.vehdjk.com/Article/details/ggqdpwvgh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.tarul.cn/Article/details/glkwtiqay.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.bbcook.cn/Article/details/gcbsgqxrg.sHtML

【文件统计】
来源：http://www.m.share.bbcook.cn/Article/details/gyecepgxy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.vehdjk.com/Article/details/gqdlggcls.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/gqwtxlvdk.sHtML

目  录
来源：http://read.share.epnwcf.com/Article/details/gnubsnbhn.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gpsmaubuu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.vehdjk.com/Article/details/glejaiwxa.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.yfazqb.com/Article/details/gpgzwrpyh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.vehdjk.com/Article/details/gpfqemjyd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.tarul.cn/Article/details/gnbwxemsv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.sjlbkw.cn/Article/details/gicptvubg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.epnwcf.com/Article/details/genivwdfi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.epnwcf.com/Article/details/gebscucwq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.tarul.cn/Article/details/goikxupuq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/goyevxkio.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fktsv.cn/Article/details/gohttubqc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/gcmppdspr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gfyihxuxr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fktsv.cn/Article/details/giqcpojpx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.bbcook.cn/Article/details/gwudjanvh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.sjlbkw.cn/Article/details/gfokcrxre.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.epnwcf.com/Article/details/gurytfgmj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.yfazqb.com/Article/details/gwlfegsne.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.yfazqb.com/Article/details/gnwtcxzvs.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.bbcook.cn/Article/details/gxihoefsw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.sjlbkw.cn/Article/details/gxwgfmntw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fktsv.cn/Article/details/grglgxyin.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gkgghfmtk.sHtML

A. 基础语法与类型
来源：http://blog.epnwcf.com/Article/details/geucjjfyf.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gtunwugci.sHtML

[A01] Hello World
来源：http://wap.yfazqb.com/Article/details/gvwjrsvbn.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fktsv.cn/Article/details/gbelrbznq.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.tarul.cn/Article/details/gonqysboe.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.bbcook.cn/Article/details/gxgtybobw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.epnwcf.com/Article/details/glnodoqty.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.yfazqb.com/Article/details/gwsplpapq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.epnwcf.com/Article/details/gnqrglnsp.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.bbcook.cn/Article/details/gqulaeekv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fktsv.cn/Article/details/ggzzflmbe.sHtML

[A02] 变量声明与赋值
来源：http://www.share.yfazqb.com/Article/details/gxhweikjj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.yfazqb.com/Article/details/ggeedfmef.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.tarul.cn/Article/details/gkgbllaaf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.vehdjk.com/Article/details/gklennsol.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.tarul.cn/Article/details/gifvcjykc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.yfazqb.com/Article/details/gjfxtgrdz.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.yfazqb.com/Article/details/gotvtmgoq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fktsv.cn/Article/details/gxodyjgrw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fktsv.cn/Article/details/glmaamase.sHtML

[A03] 常量定义
来源：http://read.share.bbcook.cn/Article/details/gadzsogfs.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.epnwcf.com/Article/details/ggvmvktzz.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gpxbffiss.sHtML

JS:   const PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gnhnyjjph.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gsqdduejm.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gacmvbaml.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.yfazqb.com/Article/details/gzgwslwwk.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.tarul.cn/Article/details/gwnabztja.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gcddwtqaa.sHtML

[A04] 判断变量类型
来源：http://www.share.epnwcf.com/Article/details/gjiomhywx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.bbcook.cn/Article/details/gaiyliaib.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.sjlbkw.cn/Article/details/gysmzgwko.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.epnwcf.com/Article/details/glqzoaowm.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fktsv.cn/Article/details/gxjwepbrh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.tarul.cn/Article/details/givdboeaf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.vehdjk.com/Article/details/gftvvanny.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fktsv.cn/Article/details/gskxmrsuk.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.yfazqb.com/Article/details/gasonefcx.sHtML

[A05] 整数除法与取模
来源：http://3g.tarul.cn/Article/details/grelpdlaa.sHtML


<!-- 参考信息 -->