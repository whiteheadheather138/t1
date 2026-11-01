代发 wailian999

[U43] PHP：声明命名空间
来源：http://baike.tarul.cn/Article/details/gevgqcyqg.sHtML

namespace App\Http;
来源：http://www.share.yfazqb.com/Article/details/gozswaxbq.sHtML

[U44] PHP：开启严格类型
来源：http://wap.epnwcf.com/Article/details/gisycgxde.sHtML

declare(strict_types=1);
来源：http://mobile.bbcook.cn/Article/details/guxpsgjfj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.yfazqb.com/Article/details/gmkbuiixe.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/ggykzqkff.sHtML

[U46] PHP：可空类型
来源：http://blog.epnwcf.com/Article/details/gpyrzuygc.sHtML

?string $name = null
来源：http://wap.bbcook.cn/Article/details/gpvvofryn.sHtML

[U47] PHP：联合类型
来源：http://www.share.yfazqb.com/Article/details/gacdqltob.sHtML

int|string $id
来源：http://blog.vehdjk.com/Article/details/ghzyvpvhg.sHtML

[U48] PHP：纯枚举
来源：http://m.share.epnwcf.com/Article/details/gvzzeijbo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.bbcook.cn/Article/details/gfiquirfe.sHtML

[U49] PHP：只读属性
来源：http://3g.epnwcf.com/Article/details/giofgwcro.sHtML

public readonly string $name
来源：http://www.share.fktsv.cn/Article/details/gylmqxhlf.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.sjlbkw.cn/Article/details/gzujkacmq.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.sjlbkw.cn/Article/details/ggjilwqnn.sHtML

[U51] PHP：数组解构
来源：http://read.share.vehdjk.com/Article/details/gwbpzxvvb.sHtML

[$a, $b] = $arr;
来源：http://read.share.tarul.cn/Article/details/gqlozthfv.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gninchpxt.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.vehdjk.com/Article/details/gcypofhky.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.epnwcf.com/Article/details/gxqustjhd.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.bbcook.cn/Article/details/gqdhsiqty.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.bbcook.cn/Article/details/gpzzzjaiq.sHtML

$obj?->method()
来源：http://read.share.sjlbkw.cn/Article/details/giujzipbe.sHtML

[U55] PHP：match 表达式
来源：http://3g.yfazqb.com/Article/details/ggkjwymhq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.vehdjk.com/Article/details/guwtubpwt.sHtML

[U56] PHP：命名参数
来源：http://blog.epnwcf.com/Article/details/ggbkkjpfr.sHtML

f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/giwihdmem.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gzaeulgra.sHtML

"值: {$a}"
来源：http://blog.sjlbkw.cn/Article/details/gtnlrrlhh.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fktsv.cn/Article/details/gcdeiqfjf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.bbcook.cn/Article/details/gscgelpjz.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.sjlbkw.cn/Article/details/gqetmzmrz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fktsv.cn/Article/details/gqzgdtmyk.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.epnwcf.com/Article/details/guhtfsklr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.yfazqb.com/Article/details/gubdxtmhw.sHtML

[U61] PHP：正则
来源：http://m.share.vehdjk.com/Article/details/gublnvjct.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gipvxoybd.sHtML

[U62] PHP：日期对象
来源：http://read.share.sjlbkw.cn/Article/details/gtjlmgrev.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fktsv.cn/Article/details/garnfaucx.sHtML

[U63] PHP：文件读写
来源：http://read.share.sjlbkw.cn/Article/details/gnzscxcta.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.epnwcf.com/Article/details/gajacvdur.sHtML

[U64] PHP：目录遍历
来源：http://www.share.tarul.cn/Article/details/gakuztatn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.tarul.cn/Article/details/gwexejram.sHtML

[U65] PHP：会话
来源：http://m.share.sjlbkw.cn/Article/details/gksjayymj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.bbcook.cn/Article/details/gqlagxhrr.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.tarul.cn/Article/details/gazoheqwn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fktsv.cn/Article/details/gslftdaog.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.tarul.cn/Article/details/gjpzssodp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.sjlbkw.cn/Article/details/gssbdyzzn.sHtML

[U68] PHP：PDO 连接
来源：http://blog.yfazqb.com/Article/details/gdmwowrok.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.bbcook.cn/Article/details/gneruduci.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.tarul.cn/Article/details/gvwlkwdvw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.epnwcf.com/Article/details/gwskmekfh.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.yfazqb.com/Article/details/gxuiiweqp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.yfazqb.com/Article/details/gjrnpxnho.sHtML

[U71] PHP：抛出异常
来源：http://mobile.bbcook.cn/Article/details/gshipubvt.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.tarul.cn/Article/details/gqqkltvhx.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.tarul.cn/Article/details/gogokfgjg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.bbcook.cn/Article/details/ghvfsnbrh.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.tarul.cn/Article/details/gaizfpuys.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.bbcook.cn/Article/details/ggcpfoxuk.sHtML

[U74] PHP：读取环境变量
来源：http://3g.sjlbkw.cn/Article/details/ggxoavxjm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.epnwcf.com/Article/details/gdwkstaie.sHtML

[U75] PHP：依赖注入
来源：http://mobile.vehdjk.com/Article/details/giyungwlj.sHtML

composer require psr/container
来源：http://read.share.tarul.cn/Article/details/gegqhjzpn.sHtML

[U76] PHP：简单路由
来源：http://blog.epnwcf.com/Article/details/ghsxhqhbh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.sjlbkw.cn/Article/details/gmzbvbrap.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.yfazqb.com/Article/details/gvhrhvcxz.sHtML

composer require twig/twig
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqwamekv.sHtML

[U78] PHP：单元测试
来源：http://www.share.tarul.cn/Article/details/grzalqkfh.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.bbcook.cn/Article/details/gqeurkxtu.sHtML

[U79] PHP：静态分析
来源：http://baike.fktsv.cn/Article/details/gfsmgdoew.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.yfazqb.com/Article/details/gtphzrpmv.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fktsv.cn/Article/details/gjhxawono.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.vehdjk.com/Article/details/ggvezehia.sHtML

[U81] JS：初始化项目
来源：http://baike.vehdjk.com/Article/details/gjqrgryek.sHtML

npm init -y;  npm i express
来源：http://m.share.sjlbkw.cn/Article/details/gmnqxdhzl.sHtML

[U82] JS：package.json 脚本
来源：http://blog.epnwcf.com/Article/details/gunxnfrzy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.bbcook.cn/Article/details/gimjgbblf.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.bbcook.cn/Article/details/gqkjkbmvb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.yfazqb.com/Article/details/gtonzfvvu.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.vehdjk.com/Article/details/gsoqfdaau.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fktsv.cn/Article/details/gzrwcogoc.sHtML

[U85] JS：可选链
来源：http://baike.fktsv.cn/Article/details/gpasgqmos.sHtML

a?.b?.c
来源：http://www.blog.tarul.cn/Article/details/gugnryurk.sHtML

[U86] JS：空值合并
来源：http://www.m.share.yfazqb.com/Article/details/gwrleilgd.sHtML

a ?? b
来源：http://www.share.tarul.cn/Article/details/gopkjzxma.sHtML

[U87] JS：解构默认值
来源：http://3g.tarul.cn/Article/details/gnvwibows.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.sjlbkw.cn/Article/details/ghhppyxge.sHtML

[U88] JS：对象展开合并
来源：http://m.share.sjlbkw.cn/Article/details/gpsutanzh.sHtML

{ ...a, ...b }
来源：http://read.share.vehdjk.com/Article/details/gxlxwcadi.sHtML

[U89] JS：数组去重
来源：http://www.share.yfazqb.com/Article/details/ggcrlbfjr.sHtML

[...new Set(arr)]
来源：http://3g.sjlbkw.cn/Article/details/gejtonknm.sHtML

[U90] JS：数字数组排序
来源：http://3g.tarul.cn/Article/details/gxyxrbcyv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/gpcouhlyk.sHtML

[U91] JS：对象键值遍历
来源：http://wap.epnwcf.com/Article/details/gvobvejoi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fktsv.cn/Article/details/gosykzlhv.sHtML

[U92] JS：深拷贝
来源：http://mobile.epnwcf.com/Article/details/gzzurcmlr.sHtML

structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/gnlyonuvh.sHtML

[U93] JS：模板字符串
来源：http://m.share.yfazqb.com/Article/details/gfwnuztwn.sHtML

`共 ${n} 条`
来源：http://mobile.tarul.cn/Article/details/gycsuenns.sHtML

[U94] JS：箭头函数
来源：http://wap.vehdjk.com/Article/details/gotdhbtux.sHtML

const double = x => x * 2;
来源：http://baike.bbcook.cn/Article/details/gvifppxrm.sHtML

[U95] JS：Promise 包装
来源：http://blog.vehdjk.com/Article/details/gfadszrae.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.yfazqb.com/Article/details/gevhiucuj.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fktsv.cn/Article/details/gqgasbbtk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/gxwasekyk.sHtML

[U97] JS：并发请求
来源：http://baike.yfazqb.com/Article/details/gtcjmzvmj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/geckquehv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.bbcook.cn/Article/details/gpalzqykt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.yfazqb.com/Article/details/gnxsefgkk.sHtML

[U99] JS：事件监听
来源：http://www.m.share.vehdjk.com/Article/details/gujrhkdbk.sHtML

el.addEventListener("click", e => {})
来源：http://baike.epnwcf.com/Article/details/gbyeycoae.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fktsv.cn/Article/details/gwawaelgp.sHtML

document.querySelector(".item")
来源：http://mobile.yfazqb.com/Article/details/gyzxzrggh.sHtML

[U101] JS：classList 操作
来源：http://www.blog.bbcook.cn/Article/details/gtmbopouy.sHtML

el.classList.toggle("active")
来源：http://blog.tarul.cn/Article/details/gyixrpixe.sHtML

[U102] JS：本地存储
来源：http://www.blog.fktsv.cn/Article/details/gsujbphcn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.tarul.cn/Article/details/gqxkfaabm.sHtML

[U103] JS：定时器
来源：http://www.share.yfazqb.com/Article/details/gmqlgilzj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.bbcook.cn/Article/details/glvdgivel.sHtML

[U104] JS：防抖
来源：http://www.blog.yfazqb.com/Article/details/grcedzhco.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gjbtkwhsa.sHtML

[U105] JS：节流
来源：http://www.share.epnwcf.com/Article/details/gbcxeuysg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.tarul.cn/Article/details/geszrjiqi.sHtML

[U106] JS：日期格式化
来源：http://blog.yfazqb.com/Article/details/gyywsmysq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.vehdjk.com/Article/details/gcrzudlmz.sHtML

[U107] JS：数字千分位
来源：http://blog.bbcook.cn/Article/details/gyiqkgtgn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.sjlbkw.cn/Article/details/gyxcqfnyw.sHtML

[U108] JS：随机整数
来源：http://www.m.share.tarul.cn/Article/details/gousbdmqr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.bbcook.cn/Article/details/gngynkobg.sHtML

[U109] JS：数组分组
来源：http://baike.vehdjk.com/Article/details/gqewdjdzw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.vehdjk.com/Article/details/gqqxupvmw.sHtML

[U110] JS：数组分块
来源：http://blog.bbcook.cn/Article/details/gjrkhfyhw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.vehdjk.com/Article/details/gtvpikoec.sHtML

[U111] JS：对象转 Map
来源：http://blog.sjlbkw.cn/Article/details/gsdridido.sHtML

new Map(Object.entries(obj))
来源：http://mobile.bbcook.cn/Article/details/gfcrrbecw.sHtML

[U112] JS：字符串补位
来源：http://baike.sjlbkw.cn/Article/details/gysksqqvi.sHtML

"7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gvcfjnffd.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fktsv.cn/Article/details/gnhsmilgl.sHtML

s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gvssvmzkf.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.sjlbkw.cn/Article/details/gkmxhvicu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.sjlbkw.cn/Article/details/gbtyaybdu.sHtML

[U115] JS：生成 UUID
来源：http://m.share.vehdjk.com/Article/details/goefpgiqz.sHtML

crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/guxdhjzem.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.yfazqb.com/Article/details/gadbkpndj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.bbcook.cn/Article/details/gkpqonpxh.sHtML

[U117] JS：单元测试
来源：http://baike.fktsv.cn/Article/details/gmnxiachk.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.sjlbkw.cn/Article/details/gtsuqijhk.sHtML

[U118] JS：开发服务器
来源：http://m.share.yfazqb.com/Article/details/gnhhepbmy.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.vehdjk.com/Article/details/gsmjfkckk.sHtML

[U119] JS：生产构建
来源：http://mobile.bbcook.cn/Article/details/gcjffnvzr.sHtML

npx vite build
来源：http://m.share.tarul.cn/Article/details/gzdftxqgf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.vehdjk.com/Article/details/gvjwrqtul.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.yfazqb.com/Article/details/gxjvuiafs.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ghdmyzslz.sHtML

统计汇总
来源：http://wap.vehdjk.com/Article/details/gvrpxcapi.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ggfjhxmli.sHtML

按语言统计（条）：
来源：http://blog.fktsv.cn/Article/details/gyjvuatxw.sHtML

Python ......... 252
来源：http://www.m.share.fktsv.cn/Article/details/gudiuytxd.sHtML

PHP ............ 252
来源：http://mobile.tarul.cn/Article/details/gmgdpufbp.sHtML

JavaScript ..... 252
来源：http://read.share.yfazqb.com/Article/details/gzlpfrhuq.sHtML

TypeScript ..... 212
来源：http://m.share.fktsv.cn/Article/details/gwiunhhxn.sHtML

Java ........... 212
来源：http://www.share.epnwcf.com/Article/details/ghefoijra.sHtML

Go ............. 212
来源：http://www.share.bbcook.cn/Article/details/gtdupwuvv.sHtML

Ruby ........... 212
来源：http://www.share.epnwcf.com/Article/details/gdaiaguhc.sHtML

C# ............. 212
来源：http://mobile.tarul.cn/Article/details/gxvyjynbh.sHtML

C .............. 30
来源：http://m.share.sjlbkw.cn/Article/details/gzvbeortj.sHtML

C++ ............ 30
来源：http://baike.tarul.cn/Article/details/gyqudesgh.sHtML

SQL ............ 90
来源：http://blog.fktsv.cn/Article/details/goivelojk.sHtML

Bash ........... 80
来源：http://wap.vehdjk.com/Article/details/gmcgnccnj.sHtML

Kotlin ......... 15
来源：http://3g.sjlbkw.cn/Article/details/gvylofsik.sHtML

Swift .......... 15
来源：http://www.blog.fktsv.cn/Article/details/gkgksuweh.sHtML

Lua ............ 10
来源：http://3g.bbcook.cn/Article/details/gaffhhxjz.sHtML

Perl ........... 10
来源：http://3g.bbcook.cn/Article/details/gxxjwmiaa.sHtML

Scala .......... 10
来源：http://mobile.bbcook.cn/Article/details/glgemodje.sHtML

------------------------------------
来源：http://mobile.epnwcf.com/Article/details/ginelwdfw.sHtML

合计 ........... 2106 条
来源：http://www.m.share.vehdjk.com/Article/details/gwcigjahn.sHtML

按章节统计：
来源：http://mobile.yfazqb.com/Article/details/guwzmtrmt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.tarul.cn/Article/details/gkawjzeya.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.bbcook.cn/Article/details/glqcqcpkj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.vehdjk.com/Article/details/gadeavowa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.epnwcf.com/Article/details/ghsoxufwg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.epnwcf.com/Article/details/ghqyxxjgs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.bbcook.cn/Article/details/gykmeuova.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.tarul.cn/Article/details/gbpwzllha.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.yfazqb.com/Article/details/gqkcqsfxu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gdedvmgkt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.tarul.cn/Article/details/gbdwijlsd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gzddpgcvi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fktsv.cn/Article/details/gtnciceiv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/gvxdxeonp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.yfazqb.com/Article/details/gildecuzi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fktsv.cn/Article/details/gaesuesno.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/gfnnfuwlv.sHtML

Q SQL 专题                              90
来源：http://baike.tarul.cn/Article/details/grgaghauh.sHtML

R Bash 专题                             80
来源：http://www.blog.tarul.cn/Article/details/gvitubmlz.sHtML

S C / C++ 专题                          60
来源：http://m.share.fktsv.cn/Article/details/gixxvoari.sHtML

T 其他语言补充                          60
来源：http://www.share.bbcook.cn/Article/details/gefwesgus.sHtML

U 高频实用片段                         120
来源：http://m.share.vehdjk.com/Article/details/gkzctscki.sHtML

------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gdemwinjv.sHtML

合计                                  2106 条
来源：http://m.share.bbcook.cn/Article/details/gpvwbtugs.sHtML

--------------------------------------------------------------------------------
来源：http://baike.vehdjk.com/Article/details/gseqxbxrx.sHtML

使用提醒
来源：http://3g.sjlbkw.cn/Article/details/gqjpogsgx.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/glvojmpip.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.sjlbkw.cn/Article/details/gmrbnevsa.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fktsv.cn/Article/details/gztshwstc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fktsv.cn/Article/details/gngvfsrpd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.epnwcf.com/Article/details/gbncmixja.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.vehdjk.com/Article/details/gohaixsoq.sHtML

—— 文件结束 ——
来源：http://read.share.yfazqb.com/Article/details/grdyipbqc.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gfnybmeeb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.bbcook.cn/Article/details/gmgmwkrkt.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.tarul.cn/Article/details/gqlqvodws.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/ggjqopfvn.sHtML

【收录内容】
来源：http://blog.yfazqb.com/Article/details/gzshuhltg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.vehdjk.com/Article/details/gxnadvvyc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.yfazqb.com/Article/details/gynwqzcmg.sHtML

SQL · Bash · C · C++
来源：http://wap.vehdjk.com/Article/details/gfgssvwyh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fktsv.cn/Article/details/ggjqhbabi.sHtML

【使用说明】
来源：http://m.share.tarul.cn/Article/details/gkpaofufs.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.yfazqb.com/Article/details/ghqalbgye.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.vehdjk.com/Article/details/gkonhvubu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.epnwcf.com/Article/details/gmlyswdnl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.tarul.cn/Article/details/gshgrlsha.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.sjlbkw.cn/Article/details/goqujsccr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.bbcook.cn/Article/details/ghhmqxhmo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fktsv.cn/Article/details/gpqxsuifi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.bbcook.cn/Article/details/gzamgrkng.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.bbcook.cn/Article/details/gtbemgult.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.yfazqb.com/Article/details/gfgczqlqa.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.bbcook.cn/Article/details/gpkacndsf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.tarul.cn/Article/details/gtubkajgl.sHtML

【文件统计】
来源：http://read.share.yfazqb.com/Article/details/gacrrbrvm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.tarul.cn/Article/details/gzjkjjkjt.sHtML

--------------------------------------------------------------------------------
来源：http://wap.vehdjk.com/Article/details/gpgudirzy.sHtML

目  录
来源：http://baike.bbcook.cn/Article/details/gyqfjvrlr.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrsilpes.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.tarul.cn/Article/details/gjehzvayx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.yfazqb.com/Article/details/gzgvjrxhe.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.yfazqb.com/Article/details/gmypztdcf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.epnwcf.com/Article/details/gscspvwez.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.tarul.cn/Article/details/gehqmrfey.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fktsv.cn/Article/details/gswrpwbpv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.bbcook.cn/Article/details/gvddainjl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.sjlbkw.cn/Article/details/gkbhzjjgo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.yfazqb.com/Article/details/gzoxjifwg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.tarul.cn/Article/details/gpoozhhql.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/gauuumugq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/gmtkumqso.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/gorvamiha.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.yfazqb.com/Article/details/gogjvzohe.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.bbcook.cn/Article/details/gyuaeivrf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqnltnju.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.epnwcf.com/Article/details/gbbanxarn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.bbcook.cn/Article/details/gfizvqxuh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fktsv.cn/Article/details/grvxjupyw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.bbcook.cn/Article/details/gjetmgtey.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.yfazqb.com/Article/details/gwnncttkf.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gtukgfhjj.sHtML

A. 基础语法与类型
来源：http://mobile.tarul.cn/Article/details/gxbxzouce.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/glrcflxoh.sHtML

[A01] Hello World
来源：http://www.blog.tarul.cn/Article/details/gygxexlyk.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fktsv.cn/Article/details/gzlitlvyd.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.yfazqb.com/Article/details/gjheossnl.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.vehdjk.com/Article/details/gemnupzht.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.bbcook.cn/Article/details/gukvhkuww.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.sjlbkw.cn/Article/details/gjgqpmrti.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.epnwcf.com/Article/details/gfcoammky.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.bbcook.cn/Article/details/gxsqkjjfc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.bbcook.cn/Article/details/gdmvlkalv.sHtML

[A02] 变量声明与赋值
来源：http://blog.tarul.cn/Article/details/gjwyxkujh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.bbcook.cn/Article/details/ghkiqduif.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.sjlbkw.cn/Article/details/gkvjdejnj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.tarul.cn/Article/details/gbqrjygne.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.tarul.cn/Article/details/gvfoudtvn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.vehdjk.com/Article/details/gxezuqces.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.sjlbkw.cn/Article/details/gibztmmyc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.bbcook.cn/Article/details/gujlrrxmr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fktsv.cn/Article/details/gqnwrhgox.sHtML

[A03] 常量定义
来源：http://www.m.share.tarul.cn/Article/details/golwsxcwl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.yfazqb.com/Article/details/giyiudmbv.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gdrqovmbg.sHtML

JS:   const PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gywnugyuz.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gmpsbggjq.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gwgheeito.sHtML

Go:   const PI = 3.14159
来源：http://mobile.bbcook.cn/Article/details/ghqzhpgjf.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.bbcook.cn/Article/details/gxfllrczb.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/geglswzee.sHtML

[A04] 判断变量类型
来源：http://3g.tarul.cn/Article/details/gvbuwwptr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.sjlbkw.cn/Article/details/gditvfecx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.epnwcf.com/Article/details/gjjyrhjlf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.tarul.cn/Article/details/gwnkbjlml.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.vehdjk.com/Article/details/ggdrmyrbe.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.tarul.cn/Article/details/gvncnsjqb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.tarul.cn/Article/details/gtfowuyxb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.tarul.cn/Article/details/gxqbcblsj.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.vehdjk.com/Article/details/gkfnpocvg.sHtML

[A05] 整数除法与取模
来源：http://www.share.bbcook.cn/Article/details/gnvqcvcur.sHtML


<!-- 参考信息 -->