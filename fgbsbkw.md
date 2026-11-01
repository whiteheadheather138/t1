代发 wailian999

[U43] PHP：声明命名空间
来源：http://m.share.tarul.cn/Article/details/geepkgcem.sHtML

namespace App\Http;
来源：http://www.blog.fktsv.cn/Article/details/gwkffpnnl.sHtML

[U44] PHP：开启严格类型
来源：http://3g.sjlbkw.cn/Article/details/gscedtwvi.sHtML

declare(strict_types=1);
来源：http://mobile.bbcook.cn/Article/details/goxakrmqs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.epnwcf.com/Article/details/gqvnzlrzk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gtcnjetre.sHtML

[U46] PHP：可空类型
来源：http://3g.epnwcf.com/Article/details/gbqcochyg.sHtML

?string $name = null
来源：http://blog.bbcook.cn/Article/details/gnppehqpk.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.bbcook.cn/Article/details/glekreyxt.sHtML

int|string $id
来源：http://mobile.bbcook.cn/Article/details/gyneutmvk.sHtML

[U48] PHP：纯枚举
来源：http://www.share.yfazqb.com/Article/details/gatarhezv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.tarul.cn/Article/details/ghkyrbwdv.sHtML

[U49] PHP：只读属性
来源：http://blog.epnwcf.com/Article/details/grbfqyigq.sHtML

public readonly string $name
来源：http://www.blog.bbcook.cn/Article/details/ganwuvnla.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.sjlbkw.cn/Article/details/gueqnipjs.sHtML

public function __construct(private int $id) {}
来源：http://blog.bbcook.cn/Article/details/gcldamiso.sHtML

[U51] PHP：数组解构
来源：http://www.share.epnwcf.com/Article/details/glrljrkcx.sHtML

[$a, $b] = $arr;
来源：http://baike.vehdjk.com/Article/details/gtumekspa.sHtML

[U52] PHP：箭头函数
来源：http://3g.epnwcf.com/Article/details/ghrmroges.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.yfazqb.com/Article/details/gewwiqchl.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.epnwcf.com/Article/details/gljiiuozt.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.sjlbkw.cn/Article/details/gkwmetklq.sHtML

[U54] PHP：空安全调用
来源：http://baike.tarul.cn/Article/details/gsnazznyw.sHtML

$obj?->method()
来源：http://www.share.bbcook.cn/Article/details/gencpuwks.sHtML

[U55] PHP：match 表达式
来源：http://mobile.bbcook.cn/Article/details/gausoxwns.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fktsv.cn/Article/details/gxcozhfmz.sHtML

[U56] PHP：命名参数
来源：http://m.share.bbcook.cn/Article/details/gidkrxyet.sHtML

f(a: 1, b: 2)
来源：http://mobile.epnwcf.com/Article/details/glazfhuqy.sHtML

[U57] PHP：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gglnsqsnk.sHtML

"值: {$a}"
来源：http://3g.fktsv.cn/Article/details/gpseqdffo.sHtML

[U58] PHP：数组三件套
来源：http://wap.vehdjk.com/Article/details/gbvajmgns.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fktsv.cn/Article/details/gbpzkmvze.sHtML

[U59] PHP：自定义排序
来源：http://www.share.epnwcf.com/Article/details/gsffpuyus.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.vehdjk.com/Article/details/gokomoigr.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.vehdjk.com/Article/details/gkxbgnxag.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.bbcook.cn/Article/details/grgqracqu.sHtML

[U61] PHP：正则
来源：http://www.blog.yfazqb.com/Article/details/gctbtmvtf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.vehdjk.com/Article/details/ghwvnaxwq.sHtML

[U62] PHP：日期对象
来源：http://www.blog.tarul.cn/Article/details/gsqqzctkz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.vehdjk.com/Article/details/gvbtusvwp.sHtML

[U63] PHP：文件读写
来源：http://www.blog.yfazqb.com/Article/details/gfujhbins.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.tarul.cn/Article/details/ggdawjabr.sHtML

[U64] PHP：目录遍历
来源：http://read.share.tarul.cn/Article/details/gbqqaelub.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.epnwcf.com/Article/details/glpbybbop.sHtML

[U65] PHP：会话
来源：http://read.share.bbcook.cn/Article/details/gqtbxjtdm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.vehdjk.com/Article/details/gjokyunsz.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.tarul.cn/Article/details/gavmykuds.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.vehdjk.com/Article/details/gttguoeyr.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fktsv.cn/Article/details/gqojnozxi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.bbcook.cn/Article/details/glmhulegx.sHtML

[U68] PHP：PDO 连接
来源：http://wap.sjlbkw.cn/Article/details/gqcpcdgpy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.yfazqb.com/Article/details/gketuqgdd.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.sjlbkw.cn/Article/details/glhvlmxgm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.yfazqb.com/Article/details/gazhuheam.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fktsv.cn/Article/details/gftmivdxd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.bbcook.cn/Article/details/gnidudrsk.sHtML

[U71] PHP：抛出异常
来源：http://read.share.sjlbkw.cn/Article/details/gchdnhjiq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.sjlbkw.cn/Article/details/gabukksto.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fktsv.cn/Article/details/gjtmjvwuy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.vehdjk.com/Article/details/gskaxyfme.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.sjlbkw.cn/Article/details/glbmjtfqy.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.vehdjk.com/Article/details/gxogooxpr.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.bbcook.cn/Article/details/gvxbjinnv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.yfazqb.com/Article/details/ghqgnxlwl.sHtML

[U75] PHP：依赖注入
来源：http://blog.yfazqb.com/Article/details/gghhhgmtq.sHtML

composer require psr/container
来源：http://www.m.share.epnwcf.com/Article/details/gbvezlvim.sHtML

[U76] PHP：简单路由
来源：http://www.share.fktsv.cn/Article/details/goqbbfdjy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.yfazqb.com/Article/details/gsqfspihp.sHtML

[U77] PHP：模板渲染
来源：http://blog.epnwcf.com/Article/details/golfepccd.sHtML

composer require twig/twig
来源：http://www.m.share.bbcook.cn/Article/details/gsfuicaeo.sHtML

[U78] PHP：单元测试
来源：http://m.share.sjlbkw.cn/Article/details/gohgvqzdm.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.epnwcf.com/Article/details/gxfyuezru.sHtML

[U79] PHP：静态分析
来源：http://mobile.fktsv.cn/Article/details/grkeylmpi.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.bbcook.cn/Article/details/gwzeixnmz.sHtML

[U80] PHP：代码规范修复
来源：http://baike.vehdjk.com/Article/details/gbwffelsh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.yfazqb.com/Article/details/ggeolgyry.sHtML

[U81] JS：初始化项目
来源：http://www.share.vehdjk.com/Article/details/gvdfptukw.sHtML

npm init -y;  npm i express
来源：http://mobile.bbcook.cn/Article/details/gzbvbyqhe.sHtML

[U82] JS：package.json 脚本
来源：http://3g.vehdjk.com/Article/details/gefsixqiy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.bbcook.cn/Article/details/gswmropgj.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.sjlbkw.cn/Article/details/gpmoftsjc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.vehdjk.com/Article/details/gejoqfufe.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fktsv.cn/Article/details/gqrvfcctd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.bbcook.cn/Article/details/gdwdrbvjw.sHtML

[U85] JS：可选链
来源：http://baike.fktsv.cn/Article/details/gqdnkvlmx.sHtML

a?.b?.c
来源：http://wap.epnwcf.com/Article/details/gebgqdncw.sHtML

[U86] JS：空值合并
来源：http://wap.yfazqb.com/Article/details/gfhkbhbur.sHtML

a ?? b
来源：http://3g.vehdjk.com/Article/details/gzjmilwec.sHtML

[U87] JS：解构默认值
来源：http://read.share.bbcook.cn/Article/details/gpkcvluyg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.tarul.cn/Article/details/ghqasjrdf.sHtML

[U88] JS：对象展开合并
来源：http://www.share.sjlbkw.cn/Article/details/ghrprfcuq.sHtML

{ ...a, ...b }
来源：http://www.share.yfazqb.com/Article/details/gpmrbsxkv.sHtML

[U89] JS：数组去重
来源：http://mobile.yfazqb.com/Article/details/gloovrkgr.sHtML

[...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/gyhizruxx.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fktsv.cn/Article/details/gnkckhwcd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gfyyxjkzs.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.bbcook.cn/Article/details/gbvjgthai.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.sjlbkw.cn/Article/details/gkinawdfp.sHtML

[U92] JS：深拷贝
来源：http://3g.tarul.cn/Article/details/gkjbwcvxx.sHtML

structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gujavhfyt.sHtML

[U93] JS：模板字符串
来源：http://www.share.tarul.cn/Article/details/gfwwsbmxi.sHtML

`共 ${n} 条`
来源：http://www.share.yfazqb.com/Article/details/gqqweixqg.sHtML

[U94] JS：箭头函数
来源：http://3g.bbcook.cn/Article/details/gdxjwtqdz.sHtML

const double = x => x * 2;
来源：http://blog.epnwcf.com/Article/details/gmuorosfy.sHtML

[U95] JS：Promise 包装
来源：http://wap.fktsv.cn/Article/details/gznvqkddh.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.sjlbkw.cn/Article/details/gpeiuiyfc.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.bbcook.cn/Article/details/gygikpjku.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gukmfrfxj.sHtML

[U97] JS：并发请求
来源：http://www.blog.tarul.cn/Article/details/gqpudvqeo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.vehdjk.com/Article/details/ginlrpkea.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fktsv.cn/Article/details/gsvrybbod.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.yfazqb.com/Article/details/gffubzqya.sHtML

[U99] JS：事件监听
来源：http://baike.tarul.cn/Article/details/gcybyukkf.sHtML

el.addEventListener("click", e => {})
来源：http://3g.yfazqb.com/Article/details/gkikpqzsj.sHtML

[U100] JS：DOM 查询
来源：http://wap.sjlbkw.cn/Article/details/gaktdaaco.sHtML

document.querySelector(".item")
来源：http://baike.fktsv.cn/Article/details/gorsnahot.sHtML

[U101] JS：classList 操作
来源：http://read.share.vehdjk.com/Article/details/ggphfzcqm.sHtML

el.classList.toggle("active")
来源：http://baike.yfazqb.com/Article/details/gavkcrnrh.sHtML

[U102] JS：本地存储
来源：http://www.m.share.bbcook.cn/Article/details/ghfkkwoow.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fktsv.cn/Article/details/gglguqxby.sHtML

[U103] JS：定时器
来源：http://blog.bbcook.cn/Article/details/gjzjunfcx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fktsv.cn/Article/details/gepbrafzn.sHtML

[U104] JS：防抖
来源：http://www.share.fktsv.cn/Article/details/gljwqkziu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gizbytxer.sHtML

[U105] JS：节流
来源：http://blog.fktsv.cn/Article/details/gchzszjdn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.epnwcf.com/Article/details/gbhkrhynl.sHtML

[U106] JS：日期格式化
来源：http://wap.yfazqb.com/Article/details/gafzcnjdy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.epnwcf.com/Article/details/gzuqolpmk.sHtML

[U107] JS：数字千分位
来源：http://blog.sjlbkw.cn/Article/details/gjqxgknnp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.yfazqb.com/Article/details/gbroagmle.sHtML

[U108] JS：随机整数
来源：http://3g.sjlbkw.cn/Article/details/gqijhorme.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.yfazqb.com/Article/details/gcrhqescb.sHtML

[U109] JS：数组分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gruseeyym.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fktsv.cn/Article/details/gmaqoneom.sHtML

[U110] JS：数组分块
来源：http://read.share.vehdjk.com/Article/details/gcldqjjqs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.vehdjk.com/Article/details/gqeihvexz.sHtML

[U111] JS：对象转 Map
来源：http://www.share.epnwcf.com/Article/details/gqpkgykqs.sHtML

new Map(Object.entries(obj))
来源：http://baike.epnwcf.com/Article/details/gbxrewhfh.sHtML

[U112] JS：字符串补位
来源：http://wap.epnwcf.com/Article/details/gntlklkdh.sHtML

"7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/gpylnkkir.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fktsv.cn/Article/details/gmnwafopp.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/giclmwuxi.sHtML

[U114] JS：JSON 深比较
来源：http://wap.bbcook.cn/Article/details/gflnfhayy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.sjlbkw.cn/Article/details/ggtccxhxe.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fktsv.cn/Article/details/goenuefwk.sHtML

crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gflhyzegz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.yfazqb.com/Article/details/gnkmbrwbu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.bbcook.cn/Article/details/gwayekdtp.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fktsv.cn/Article/details/gpjoruwtk.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.yfazqb.com/Article/details/gshsrnofn.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fktsv.cn/Article/details/gzsqsefns.sHtML

npm i -D vite;  npx vite
来源：http://blog.sjlbkw.cn/Article/details/gxbmydoew.sHtML

[U119] JS：生产构建
来源：http://read.share.bbcook.cn/Article/details/gilepywnt.sHtML

npx vite build
来源：http://www.share.fktsv.cn/Article/details/gvnabenqz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.yfazqb.com/Article/details/gawnttejv.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fktsv.cn/Article/details/gdsuctxid.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gudzoegoq.sHtML

统计汇总
来源：http://wap.epnwcf.com/Article/details/gslopxdad.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/grlhwbfpc.sHtML

按语言统计（条）：
来源：http://www.blog.bbcook.cn/Article/details/ggyosbaso.sHtML

Python ......... 252
来源：http://m.share.tarul.cn/Article/details/gowgarpqo.sHtML

PHP ............ 252
来源：http://www.share.vehdjk.com/Article/details/gdcxkvjdx.sHtML

JavaScript ..... 252
来源：http://blog.epnwcf.com/Article/details/gghfqszpp.sHtML

TypeScript ..... 212
来源：http://m.share.tarul.cn/Article/details/ghbimncna.sHtML

Java ........... 212
来源：http://blog.yfazqb.com/Article/details/gwhlynrcg.sHtML

Go ............. 212
来源：http://baike.tarul.cn/Article/details/gmiczwkjq.sHtML

Ruby ........... 212
来源：http://read.share.fktsv.cn/Article/details/gzsgdctim.sHtML

C# ............. 212
来源：http://wap.yfazqb.com/Article/details/ghjavpmwh.sHtML

C .............. 30
来源：http://www.m.share.epnwcf.com/Article/details/gpxrgqisu.sHtML

C++ ............ 30
来源：http://baike.epnwcf.com/Article/details/gavcgxulj.sHtML

SQL ............ 90
来源：http://wap.fktsv.cn/Article/details/gxmmpboze.sHtML

Bash ........... 80
来源：http://mobile.epnwcf.com/Article/details/gbjvjjcxa.sHtML

Kotlin ......... 15
来源：http://wap.tarul.cn/Article/details/gprlmhndl.sHtML

Swift .......... 15
来源：http://m.share.epnwcf.com/Article/details/gbblydxvl.sHtML

Lua ............ 10
来源：http://mobile.fktsv.cn/Article/details/gniznqlzu.sHtML

Perl ........... 10
来源：http://www.share.bbcook.cn/Article/details/gkvnigwty.sHtML

Scala .......... 10
来源：http://read.share.bbcook.cn/Article/details/gxgpxookn.sHtML

------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gcworiiqg.sHtML

合计 ........... 2106 条
来源：http://wap.fktsv.cn/Article/details/gupsdhrln.sHtML

按章节统计：
来源：http://www.share.epnwcf.com/Article/details/grcedmzqs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.tarul.cn/Article/details/gibvuywfh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.sjlbkw.cn/Article/details/gnnzmkvwp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/gkrbxxqts.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.vehdjk.com/Article/details/gyixathaq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.sjlbkw.cn/Article/details/ggroeevwr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.epnwcf.com/Article/details/gsmuxsbof.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.tarul.cn/Article/details/ggwxpfxay.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.yfazqb.com/Article/details/gkevegnuc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/giihcycix.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.epnwcf.com/Article/details/gqfwijibz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/gvdxaloiu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gerusqphx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gfopbfqnd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.yfazqb.com/Article/details/gnvecnorf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.epnwcf.com/Article/details/ghxvdkwjo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gcezfwfox.sHtML

Q SQL 专题                              90
来源：http://3g.fktsv.cn/Article/details/gftvraahc.sHtML

R Bash 专题                             80
来源：http://read.share.sjlbkw.cn/Article/details/gtegosfvx.sHtML

S C / C++ 专题                          60
来源：http://www.share.yfazqb.com/Article/details/gdffahcvs.sHtML

T 其他语言补充                          60
来源：http://3g.vehdjk.com/Article/details/gjmgoijma.sHtML

U 高频实用片段                         120
来源：http://read.share.fktsv.cn/Article/details/gjsqmsdai.sHtML

------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gifkrfvfw.sHtML

合计                                  2106 条
来源：http://m.share.fktsv.cn/Article/details/gmnkcnqie.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.bbcook.cn/Article/details/ghjihelei.sHtML

使用提醒
来源：http://www.m.share.epnwcf.com/Article/details/ggmpgeynb.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gzswfgsbx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.bbcook.cn/Article/details/gklispgee.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.yfazqb.com/Article/details/ghfzvxfcn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fktsv.cn/Article/details/gvywzceba.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.tarul.cn/Article/details/gsptosppd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.bbcook.cn/Article/details/gkfzharwb.sHtML

—— 文件结束 ——
来源：http://3g.tarul.cn/Article/details/gsumoigvb.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gwdqwnmnx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.bbcook.cn/Article/details/gpwyneqkk.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fktsv.cn/Article/details/gsqvtoqsv.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gndmcwhru.sHtML

【收录内容】
来源：http://blog.sjlbkw.cn/Article/details/giqgowsmz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.yfazqb.com/Article/details/gpzcdvewo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.vehdjk.com/Article/details/gokacmmht.sHtML

SQL · Bash · C · C++
来源：http://m.share.vehdjk.com/Article/details/gwmymtpxv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.yfazqb.com/Article/details/gafdktgia.sHtML

【使用说明】
来源：http://mobile.sjlbkw.cn/Article/details/gintenprd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.vehdjk.com/Article/details/gkvqqnrsr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.sjlbkw.cn/Article/details/gtqweknif.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.tarul.cn/Article/details/gacyhhenn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fktsv.cn/Article/details/gexmpcfqi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.yfazqb.com/Article/details/gwcjgdfzy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.tarul.cn/Article/details/gccaytvif.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.yfazqb.com/Article/details/gzgxdfqed.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fktsv.cn/Article/details/gdgvzezdm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.sjlbkw.cn/Article/details/giwcsqbxi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.tarul.cn/Article/details/gylesoisg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.yfazqb.com/Article/details/glrefqvoz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.vehdjk.com/Article/details/gnkcgzqks.sHtML

【文件统计】
来源：http://wap.epnwcf.com/Article/details/glvyzxhdu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.epnwcf.com/Article/details/gokyiqeie.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/grmyeuera.sHtML

目  录
来源：http://3g.fktsv.cn/Article/details/ggotbqfhw.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gmqbvldzg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.epnwcf.com/Article/details/gnhcnohgr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fktsv.cn/Article/details/gjhclccxz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fktsv.cn/Article/details/gajvaphxh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.epnwcf.com/Article/details/gpsjmhhtd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.sjlbkw.cn/Article/details/gibhnvgyj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.bbcook.cn/Article/details/grbyarren.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.tarul.cn/Article/details/gxrjyvnqp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.sjlbkw.cn/Article/details/gxgodmmmi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/gdvnsqwez.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fktsv.cn/Article/details/gvyapnqzw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.sjlbkw.cn/Article/details/gfwuzwtmc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/ggzecoxxb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.sjlbkw.cn/Article/details/gcpyirgca.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.sjlbkw.cn/Article/details/gbfqaqwwt.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.vehdjk.com/Article/details/gkimvlrpg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/gyhzorszd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.bbcook.cn/Article/details/gwnvqpfza.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.sjlbkw.cn/Article/details/gsyivysbg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.sjlbkw.cn/Article/details/gtosfkmiu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.yfazqb.com/Article/details/gnelbgnjt.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.sjlbkw.cn/Article/details/glprejmjc.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gttonsmer.sHtML

A. 基础语法与类型
来源：http://read.share.tarul.cn/Article/details/gamgvkwxd.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gxpwuyjsh.sHtML

[A01] Hello World
来源：http://www.share.fktsv.cn/Article/details/ggahbmvag.sHtML

Py:   print("Hello, World!")
来源：http://baike.sjlbkw.cn/Article/details/gxqvnzuvh.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.tarul.cn/Article/details/gipawzqbl.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.tarul.cn/Article/details/gkpsxvfot.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.yfazqb.com/Article/details/gdeahbquf.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.epnwcf.com/Article/details/gagqqxmby.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.tarul.cn/Article/details/gratqyhkc.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.epnwcf.com/Article/details/gifdhbogu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.tarul.cn/Article/details/gdlbcsrys.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fktsv.cn/Article/details/gtpfhcmyg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.vehdjk.com/Article/details/gwxamwdlu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.tarul.cn/Article/details/ggwyrrama.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.sjlbkw.cn/Article/details/gvrdiougn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.yfazqb.com/Article/details/gstizguqu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.tarul.cn/Article/details/gmkonzsgj.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fktsv.cn/Article/details/gszlfkqtf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.yfazqb.com/Article/details/gzzumivoi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.bbcook.cn/Article/details/gjwrboqmn.sHtML

[A03] 常量定义
来源：http://www.share.yfazqb.com/Article/details/gpceuacto.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fktsv.cn/Article/details/gplsvdhtj.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gahoyjciw.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gwjeoksmi.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gjpelbrps.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gutfkkmng.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.yfazqb.com/Article/details/gemoehyly.sHtML

Ruby: PI = 3.14159
来源：http://mobile.epnwcf.com/Article/details/gpimotqbh.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gqxxqwjbf.sHtML

[A04] 判断变量类型
来源：http://www.blog.fktsv.cn/Article/details/gnvnlsevi.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.sjlbkw.cn/Article/details/grahtupcs.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.bbcook.cn/Article/details/gnkuxzuvd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.yfazqb.com/Article/details/giexqdsut.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.epnwcf.com/Article/details/gruggrjds.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.yfazqb.com/Article/details/gzkduywwy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.vehdjk.com/Article/details/gtkouyypw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.vehdjk.com/Article/details/ggasiiabu.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.epnwcf.com/Article/details/gfwptsaqy.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.vehdjk.com/Article/details/gpanqjnqs.sHtML


<!-- 参考信息 -->