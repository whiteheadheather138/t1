代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.share.bbcook.cn/Article/details/ghdwmpaib.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gctcncznh.sHtML

[U46] PHP：可空类型
来源：http://blog.fktsv.cn/Article/details/gfptkgqtg.sHtML

?string $name = null
来源：http://blog.sjlbkw.cn/Article/details/gjfnmxmtk.sHtML

[U47] PHP：联合类型
来源：http://read.share.vehdjk.com/Article/details/gejpgmloq.sHtML

int|string $id
来源：http://www.share.tarul.cn/Article/details/ggjnwfkcx.sHtML

[U48] PHP：纯枚举
来源：http://blog.epnwcf.com/Article/details/guwwsggfs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.tarul.cn/Article/details/gvjercxze.sHtML

[U49] PHP：只读属性
来源：http://wap.sjlbkw.cn/Article/details/ghlqxkdgw.sHtML

public readonly string $name
来源：http://blog.fktsv.cn/Article/details/gbqzmucxf.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fktsv.cn/Article/details/gnwvqxodl.sHtML

public function __construct(private int $id) {}
来源：http://m.share.tarul.cn/Article/details/gnqsvpypk.sHtML

[U51] PHP：数组解构
来源：http://wap.yfazqb.com/Article/details/gtuylthkr.sHtML

[$a, $b] = $arr;
来源：http://baike.yfazqb.com/Article/details/gsvfwuckr.sHtML

[U52] PHP：箭头函数
来源：http://m.share.vehdjk.com/Article/details/gncvkxemf.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.tarul.cn/Article/details/gzxscvwpy.sHtML

[U53] PHP：空合并运算符
来源：http://3g.tarul.cn/Article/details/gyyehlgma.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.epnwcf.com/Article/details/gxcvopcmr.sHtML

[U54] PHP：空安全调用
来源：http://mobile.vehdjk.com/Article/details/gizjhdtfm.sHtML

$obj?->method()
来源：http://wap.tarul.cn/Article/details/ggrehyhzk.sHtML

[U55] PHP：match 表达式
来源：http://baike.tarul.cn/Article/details/ggetfxfjw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.sjlbkw.cn/Article/details/ghsdrhkbh.sHtML

[U56] PHP：命名参数
来源：http://baike.vehdjk.com/Article/details/gekcaefkz.sHtML

f(a: 1, b: 2)
来源：http://3g.epnwcf.com/Article/details/gpuhdphwe.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gvktyogyk.sHtML

"值: {$a}"
来源：http://www.blog.bbcook.cn/Article/details/guhlmzhra.sHtML

[U58] PHP：数组三件套
来源：http://www.share.epnwcf.com/Article/details/gaaqepstt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.epnwcf.com/Article/details/gisipzckp.sHtML

[U59] PHP：自定义排序
来源：http://3g.epnwcf.com/Article/details/guftbuiic.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fktsv.cn/Article/details/gvqomcagi.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.epnwcf.com/Article/details/gjxgjuxlx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.tarul.cn/Article/details/gnhalclch.sHtML

[U61] PHP：正则
来源：http://read.share.epnwcf.com/Article/details/gpewhhpqc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.bbcook.cn/Article/details/gucdfurxs.sHtML

[U62] PHP：日期对象
来源：http://blog.epnwcf.com/Article/details/gftykxpkk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.epnwcf.com/Article/details/gkrtoxjkz.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fktsv.cn/Article/details/gzfmjlpkx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.sjlbkw.cn/Article/details/gcshcverx.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fktsv.cn/Article/details/gahwfevpp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fktsv.cn/Article/details/gjlksepbs.sHtML

[U65] PHP：会话
来源：http://m.share.fktsv.cn/Article/details/gpeopemwp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gxxymdedt.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.vehdjk.com/Article/details/gkrmprdwa.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.sjlbkw.cn/Article/details/gnudbarke.sHtML

[U67] PHP：处理文件上传
来源：http://3g.vehdjk.com/Article/details/gqqfwtott.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fktsv.cn/Article/details/gbnzflwmp.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fktsv.cn/Article/details/ggquzvqwx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.epnwcf.com/Article/details/gvdbbvlfv.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.vehdjk.com/Article/details/gujuovpea.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.bbcook.cn/Article/details/gxcynqzsy.sHtML

[U70] PHP：PDO 事务
来源：http://3g.vehdjk.com/Article/details/guioxdspi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.epnwcf.com/Article/details/gwevhkiea.sHtML

[U71] PHP：抛出异常
来源：http://wap.fktsv.cn/Article/details/gaofpfbrl.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.tarul.cn/Article/details/ghykvdrin.sHtML

[U72] PHP：写错误日志
来源：http://m.share.bbcook.cn/Article/details/gfjqkivrs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.epnwcf.com/Article/details/gevcscgqd.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fktsv.cn/Article/details/gpkkqfyjg.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.epnwcf.com/Article/details/gjlsvxale.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fktsv.cn/Article/details/gjkiostoy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.epnwcf.com/Article/details/gqloomnfe.sHtML

[U75] PHP：依赖注入
来源：http://wap.bbcook.cn/Article/details/grqjzhhcc.sHtML

composer require psr/container
来源：http://read.share.epnwcf.com/Article/details/gjcyahxtj.sHtML

[U76] PHP：简单路由
来源：http://read.share.vehdjk.com/Article/details/gqhyrtiam.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.tarul.cn/Article/details/gcyccmulr.sHtML

[U77] PHP：模板渲染
来源：http://m.share.tarul.cn/Article/details/grmhiodcw.sHtML

composer require twig/twig
来源：http://www.blog.yfazqb.com/Article/details/gkkceomux.sHtML

[U78] PHP：单元测试
来源：http://www.share.vehdjk.com/Article/details/ggaywqwml.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.epnwcf.com/Article/details/gfphzvpma.sHtML

[U79] PHP：静态分析
来源：http://3g.yfazqb.com/Article/details/gqfyhyczy.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.epnwcf.com/Article/details/gpwjbcusu.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.tarul.cn/Article/details/gaanwnjsr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.bbcook.cn/Article/details/gojmqmteb.sHtML

[U81] JS：初始化项目
来源：http://mobile.vehdjk.com/Article/details/ghztsnkts.sHtML

npm init -y;  npm i express
来源：http://baike.sjlbkw.cn/Article/details/gbqyfpvdb.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.yfazqb.com/Article/details/gxtjqgony.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.sjlbkw.cn/Article/details/genfqrkpv.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.vehdjk.com/Article/details/gbtzzejdi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.vehdjk.com/Article/details/giszpghcu.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.yfazqb.com/Article/details/gpiofeljq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fktsv.cn/Article/details/gyyaeywdz.sHtML

[U85] JS：可选链
来源：http://www.share.sjlbkw.cn/Article/details/gjhjflydq.sHtML

a?.b?.c
来源：http://baike.vehdjk.com/Article/details/gothsfrsf.sHtML

[U86] JS：空值合并
来源：http://wap.tarul.cn/Article/details/gtlkkoqaf.sHtML

a ?? b
来源：http://mobile.tarul.cn/Article/details/gnmzohupw.sHtML

[U87] JS：解构默认值
来源：http://mobile.sjlbkw.cn/Article/details/gumqxwwqz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.tarul.cn/Article/details/gqyojmhrd.sHtML

[U88] JS：对象展开合并
来源：http://mobile.bbcook.cn/Article/details/gnzegxbke.sHtML

{ ...a, ...b }
来源：http://3g.epnwcf.com/Article/details/geyjmzdza.sHtML

[U89] JS：数组去重
来源：http://www.share.vehdjk.com/Article/details/ghwxgmysa.sHtML

[...new Set(arr)]
来源：http://3g.fktsv.cn/Article/details/ghquulwlp.sHtML

[U90] JS：数字数组排序
来源：http://wap.sjlbkw.cn/Article/details/gmxieuxfb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gjwzyjqbz.sHtML

[U91] JS：对象键值遍历
来源：http://blog.yfazqb.com/Article/details/gxapdzmqu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.yfazqb.com/Article/details/gejqpseky.sHtML

[U92] JS：深拷贝
来源：http://baike.sjlbkw.cn/Article/details/gfjxkfjks.sHtML

structuredClone(obj)
来源：http://mobile.vehdjk.com/Article/details/gkvtheccn.sHtML

[U93] JS：模板字符串
来源：http://www.blog.bbcook.cn/Article/details/gesxdkrwo.sHtML

`共 ${n} 条`
来源：http://www.share.epnwcf.com/Article/details/gxwjmqkbu.sHtML

[U94] JS：箭头函数
来源：http://blog.fktsv.cn/Article/details/gftgaywjp.sHtML

const double = x => x * 2;
来源：http://read.share.vehdjk.com/Article/details/gtimedsri.sHtML

[U95] JS：Promise 包装
来源：http://mobile.epnwcf.com/Article/details/gksjcsurq.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.epnwcf.com/Article/details/gbzwakkco.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.epnwcf.com/Article/details/gwmkfqrty.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/gayzsygbe.sHtML

[U97] JS：并发请求
来源：http://3g.epnwcf.com/Article/details/ghuqbvdyg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/glmqtoigl.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.vehdjk.com/Article/details/gmzbkslgd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.epnwcf.com/Article/details/gikxuswsu.sHtML

[U99] JS：事件监听
来源：http://blog.epnwcf.com/Article/details/gaewguuso.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fktsv.cn/Article/details/geifhidih.sHtML

[U100] JS：DOM 查询
来源：http://blog.bbcook.cn/Article/details/gxnpofipn.sHtML

document.querySelector(".item")
来源：http://www.blog.yfazqb.com/Article/details/gyakamzhy.sHtML

[U101] JS：classList 操作
来源：http://read.share.epnwcf.com/Article/details/gilzycuol.sHtML

el.classList.toggle("active")
来源：http://wap.fktsv.cn/Article/details/gkipwnvlp.sHtML

[U102] JS：本地存储
来源：http://baike.yfazqb.com/Article/details/gjxesflmp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fktsv.cn/Article/details/gewiaywzu.sHtML

[U103] JS：定时器
来源：http://www.m.share.yfazqb.com/Article/details/gwhwweqms.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fktsv.cn/Article/details/gisyyxhnq.sHtML

[U104] JS：防抖
来源：http://www.blog.vehdjk.com/Article/details/glwvsupoe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.epnwcf.com/Article/details/gqsexmwou.sHtML

[U105] JS：节流
来源：http://www.share.sjlbkw.cn/Article/details/gawcklvfv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.vehdjk.com/Article/details/gzbzuvigt.sHtML

[U106] JS：日期格式化
来源：http://3g.bbcook.cn/Article/details/gmoxkkcsa.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.epnwcf.com/Article/details/gyhzzsuvw.sHtML

[U107] JS：数字千分位
来源：http://blog.bbcook.cn/Article/details/gamkhqmzp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fktsv.cn/Article/details/gdcqrwodj.sHtML

[U108] JS：随机整数
来源：http://blog.epnwcf.com/Article/details/gvhsjwljs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.yfazqb.com/Article/details/gdvbyzdai.sHtML

[U109] JS：数组分组
来源：http://read.share.fktsv.cn/Article/details/gvkzijmau.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.bbcook.cn/Article/details/gtqxqjymo.sHtML

[U110] JS：数组分块
来源：http://m.share.epnwcf.com/Article/details/gcaaykjlc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.yfazqb.com/Article/details/geuxnqndo.sHtML

[U111] JS：对象转 Map
来源：http://www.share.yfazqb.com/Article/details/gnyrycvwr.sHtML

new Map(Object.entries(obj))
来源：http://mobile.sjlbkw.cn/Article/details/govktdgzu.sHtML

[U112] JS：字符串补位
来源：http://read.share.bbcook.cn/Article/details/gzhzwangg.sHtML

"7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gvuclojcy.sHtML

[U113] JS：正则替换全部
来源：http://baike.bbcook.cn/Article/details/gsgyqocel.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gielingke.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fktsv.cn/Article/details/gdqvbaydl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.epnwcf.com/Article/details/guydopcru.sHtML

[U115] JS：生成 UUID
来源：http://read.share.sjlbkw.cn/Article/details/gkxnpsglo.sHtML

crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/gfjipnutj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fktsv.cn/Article/details/gjoqofwcy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.epnwcf.com/Article/details/gdoacvilk.sHtML

[U117] JS：单元测试
来源：http://3g.epnwcf.com/Article/details/gffktuqbm.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.tarul.cn/Article/details/gpzefqkvl.sHtML

[U118] JS：开发服务器
来源：http://baike.tarul.cn/Article/details/gqewyablr.sHtML

npm i -D vite;  npx vite
来源：http://m.share.sjlbkw.cn/Article/details/gftfoaikq.sHtML

[U119] JS：生产构建
来源：http://m.share.epnwcf.com/Article/details/gpnvqrujp.sHtML

npx vite build
来源：http://www.share.tarul.cn/Article/details/gacfrsrlr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.tarul.cn/Article/details/giwvkrwhw.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fktsv.cn/Article/details/gvvktgitp.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gwykwzjts.sHtML

统计汇总
来源：http://wap.bbcook.cn/Article/details/gyobilygn.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gxoxdykae.sHtML

按语言统计（条）：
来源：http://m.share.bbcook.cn/Article/details/glvnbelhj.sHtML

Python ......... 252
来源：http://baike.yfazqb.com/Article/details/gtcyvhako.sHtML

PHP ............ 252
来源：http://m.share.sjlbkw.cn/Article/details/gwqfdlriz.sHtML

JavaScript ..... 252
来源：http://www.share.vehdjk.com/Article/details/geczsyotq.sHtML

TypeScript ..... 212
来源：http://blog.yfazqb.com/Article/details/gpljciykk.sHtML

Java ........... 212
来源：http://m.share.bbcook.cn/Article/details/ghkuwxwtg.sHtML

Go ............. 212
来源：http://read.share.epnwcf.com/Article/details/gdqeulkqb.sHtML

Ruby ........... 212
来源：http://m.share.sjlbkw.cn/Article/details/gcstkiahj.sHtML

C# ............. 212
来源：http://blog.fktsv.cn/Article/details/gcrhpowxx.sHtML

C .............. 30
来源：http://wap.vehdjk.com/Article/details/gcwbzmcqa.sHtML

C++ ............ 30
来源：http://www.share.bbcook.cn/Article/details/ghxisoadq.sHtML

SQL ............ 90
来源：http://baike.fktsv.cn/Article/details/guppldpsa.sHtML

Bash ........... 80
来源：http://baike.vehdjk.com/Article/details/gryzbfhka.sHtML

Kotlin ......... 15
来源：http://m.share.vehdjk.com/Article/details/gpkxyzjzq.sHtML

Swift .......... 15
来源：http://wap.vehdjk.com/Article/details/gwngttgjp.sHtML

Lua ............ 10
来源：http://www.share.fktsv.cn/Article/details/gncefoszu.sHtML

Perl ........... 10
来源：http://mobile.tarul.cn/Article/details/gajwuykml.sHtML

Scala .......... 10
来源：http://baike.epnwcf.com/Article/details/gdnwbjdvs.sHtML

------------------------------------
来源：http://wap.vehdjk.com/Article/details/gltbwbktg.sHtML

合计 ........... 2106 条
来源：http://www.blog.tarul.cn/Article/details/gogbbuozp.sHtML

按章节统计：
来源：http://www.m.share.yfazqb.com/Article/details/gzvksokhn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.tarul.cn/Article/details/gqfwgdoio.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.yfazqb.com/Article/details/ghtjdzjnd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.bbcook.cn/Article/details/gshrojydx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.bbcook.cn/Article/details/gkcpsjvni.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.epnwcf.com/Article/details/gjblcguty.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.epnwcf.com/Article/details/gqactwitl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.tarul.cn/Article/details/gasmpohda.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.vehdjk.com/Article/details/gofeygqyy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/gvhytgosa.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.yfazqb.com/Article/details/ghghnmjjg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/gosanasjk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gdrbjsgqr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gltamrhjb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.epnwcf.com/Article/details/grpwfsmrf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.tarul.cn/Article/details/gwsytzsng.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/geuijgpvb.sHtML

Q SQL 专题                              90
来源：http://www.m.share.tarul.cn/Article/details/gxcurkbuv.sHtML

R Bash 专题                             80
来源：http://m.share.bbcook.cn/Article/details/gtpmrfrsp.sHtML

S C / C++ 专题                          60
来源：http://baike.yfazqb.com/Article/details/gkkdevvdi.sHtML

T 其他语言补充                          60
来源：http://read.share.tarul.cn/Article/details/geiroatjo.sHtML

U 高频实用片段                         120
来源：http://mobile.vehdjk.com/Article/details/gnfrwhgft.sHtML

------------------------------------
来源：http://blog.fktsv.cn/Article/details/gamdbodrn.sHtML

合计                                  2106 条
来源：http://www.share.bbcook.cn/Article/details/gcfvnkzlq.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/gpcgzcote.sHtML

使用提醒
来源：http://mobile.fktsv.cn/Article/details/gaydzoxno.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/ghvigkbdr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.yfazqb.com/Article/details/gvknsmoby.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.bbcook.cn/Article/details/gmxslnnry.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.bbcook.cn/Article/details/gmyvxsmbs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.yfazqb.com/Article/details/gwgdozqjl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.vehdjk.com/Article/details/gozyfkjqh.sHtML

—— 文件结束 ——
来源：http://www.share.epnwcf.com/Article/details/gadfaikml.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/grscpfhpx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.bbcook.cn/Article/details/gbljlffbc.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.tarul.cn/Article/details/gezaplaye.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gnqtxjsru.sHtML

【收录内容】
来源：http://3g.vehdjk.com/Article/details/geyxflxlf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.tarul.cn/Article/details/gvjttofzd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fktsv.cn/Article/details/goghrjlrh.sHtML

SQL · Bash · C · C++
来源：http://mobile.yfazqb.com/Article/details/gnkbpvelw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.tarul.cn/Article/details/gorxdpxhg.sHtML

【使用说明】
来源：http://baike.fktsv.cn/Article/details/glmxbhxed.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.sjlbkw.cn/Article/details/ggkpilqil.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fktsv.cn/Article/details/gpdyrclin.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.bbcook.cn/Article/details/ggxssttiu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.tarul.cn/Article/details/gxaurwxws.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.tarul.cn/Article/details/gbzwovqkc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.tarul.cn/Article/details/glairucab.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fktsv.cn/Article/details/gawoipvmk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fktsv.cn/Article/details/greuoybpb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.bbcook.cn/Article/details/gmshwhvun.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.vehdjk.com/Article/details/glxzzpfdb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.bbcook.cn/Article/details/gdcdicfqz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.epnwcf.com/Article/details/gpffscjog.sHtML

【文件统计】
来源：http://www.share.vehdjk.com/Article/details/gascxbiud.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.bbcook.cn/Article/details/gfqjglmus.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gmygefdcm.sHtML

目  录
来源：http://read.share.bbcook.cn/Article/details/gwidmfjec.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.vehdjk.com/Article/details/gilsekyny.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.epnwcf.com/Article/details/gwybbrnfl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.bbcook.cn/Article/details/gvuulkziv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.epnwcf.com/Article/details/gztwtelfe.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fktsv.cn/Article/details/gngkdejua.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.vehdjk.com/Article/details/gkhkdghen.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.epnwcf.com/Article/details/gdzrunucs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.vehdjk.com/Article/details/gtwepwzxw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gympjfscy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/gpeakkkkf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.sjlbkw.cn/Article/details/gzbouzson.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/gnuaovgad.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/gvwsjqfas.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/ggixwfrbv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.tarul.cn/Article/details/gjnzptidb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.epnwcf.com/Article/details/gyumrsptf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.tarul.cn/Article/details/gvkvpljiz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.tarul.cn/Article/details/ggdtlzkjk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.vehdjk.com/Article/details/gfcantgkz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.tarul.cn/Article/details/gkixgfzhy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.sjlbkw.cn/Article/details/gqokyjdxz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fktsv.cn/Article/details/gbtxzjwtg.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gjysgxrlm.sHtML

A. 基础语法与类型
来源：http://mobile.tarul.cn/Article/details/giicttuxr.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gcdkqndsq.sHtML

[A01] Hello World
来源：http://www.blog.vehdjk.com/Article/details/gopsmoiko.sHtML

Py:   print("Hello, World!")
来源：http://3g.yfazqb.com/Article/details/gefqavdok.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.bbcook.cn/Article/details/gauflgtha.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.vehdjk.com/Article/details/gocnulpeh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.epnwcf.com/Article/details/gymywtlol.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.vehdjk.com/Article/details/ggfnnqxmm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.yfazqb.com/Article/details/grcqmtrrv.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.epnwcf.com/Article/details/gblljymcw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.bbcook.cn/Article/details/gqtmvnoxl.sHtML

[A02] 变量声明与赋值
来源：http://m.share.epnwcf.com/Article/details/gonazuymc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.yfazqb.com/Article/details/gylqpqegx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.bbcook.cn/Article/details/gozmlryvo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/goiiwfasy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.sjlbkw.cn/Article/details/gomssvqaf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fktsv.cn/Article/details/gwktruzjb.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.sjlbkw.cn/Article/details/giejfktvi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fktsv.cn/Article/details/gwoszoddk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fktsv.cn/Article/details/gjqdedlbo.sHtML

[A03] 常量定义
来源：http://wap.fktsv.cn/Article/details/gzjwkypkz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.bbcook.cn/Article/details/gtmymekfp.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gsrnuggau.sHtML

JS:   const PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gacmcfirz.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gskwjfadu.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/golipicoz.sHtML

Go:   const PI = 3.14159
来源：http://m.share.vehdjk.com/Article/details/giscbcbwt.sHtML

Ruby: PI = 3.14159
来源：http://3g.bbcook.cn/Article/details/gmxrwfktl.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gbthalovp.sHtML

[A04] 判断变量类型
来源：http://wap.yfazqb.com/Article/details/gkouvqpyh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.vehdjk.com/Article/details/gztaweolw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fktsv.cn/Article/details/gkndniqzq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.tarul.cn/Article/details/gmjawskkk.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.tarul.cn/Article/details/gxfddqela.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fktsv.cn/Article/details/guntxverr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.yfazqb.com/Article/details/gbsibplpy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.yfazqb.com/Article/details/grvhljbdd.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fktsv.cn/Article/details/gjmkikoyp.sHtML

[A05] 整数除法与取模
来源：http://3g.tarul.cn/Article/details/gbhjtzjdk.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fktsv.cn/Article/details/gdhhnocjg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/gaejfqqpi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/ghrvztian.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gghyintvt.sHtML


<!-- 参考信息 -->