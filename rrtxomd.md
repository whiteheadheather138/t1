代发 wailian999

[U47] PHP：联合类型
来源：http://wap.yfazqb.com/Article/details/gciyoagci.sHtML

int|string $id
来源：http://www.share.yfazqb.com/Article/details/gorejeeoj.sHtML

[U48] PHP：纯枚举
来源：http://blog.fktsv.cn/Article/details/ggvbwvtjm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.yfazqb.com/Article/details/glzudukjf.sHtML

[U49] PHP：只读属性
来源：http://baike.yfazqb.com/Article/details/guuutamzv.sHtML

public readonly string $name
来源：http://3g.sjlbkw.cn/Article/details/grxgfhrnh.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.yfazqb.com/Article/details/gfjaqccqc.sHtML

public function __construct(private int $id) {}
来源：http://www.share.sjlbkw.cn/Article/details/gmfabpglw.sHtML

[U51] PHP：数组解构
来源：http://blog.tarul.cn/Article/details/gboptmhyk.sHtML

[$a, $b] = $arr;
来源：http://www.share.epnwcf.com/Article/details/gtdgwqzok.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.epnwcf.com/Article/details/gvhfiwttc.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fktsv.cn/Article/details/gfcjbmaxx.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fktsv.cn/Article/details/gbtbdvadi.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.bbcook.cn/Article/details/gyxqxqocg.sHtML

[U54] PHP：空安全调用
来源：http://blog.epnwcf.com/Article/details/gtlttsiuh.sHtML

$obj?->method()
来源：http://3g.tarul.cn/Article/details/gxltrytop.sHtML

[U55] PHP：match 表达式
来源：http://baike.vehdjk.com/Article/details/gkapholvf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.vehdjk.com/Article/details/ghkrpxgcx.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.yfazqb.com/Article/details/gyhfetxnn.sHtML

f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gobzjwtjf.sHtML

[U57] PHP：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gfgifbuai.sHtML

"值: {$a}"
来源：http://www.blog.tarul.cn/Article/details/gjxzcoftr.sHtML

[U58] PHP：数组三件套
来源：http://m.share.tarul.cn/Article/details/gxwhhxyse.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.tarul.cn/Article/details/grouncodl.sHtML

[U59] PHP：自定义排序
来源：http://blog.bbcook.cn/Article/details/gyrgllbbl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.tarul.cn/Article/details/gievbbvyx.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.sjlbkw.cn/Article/details/ghfrpxbkd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.sjlbkw.cn/Article/details/geajrtebj.sHtML

[U61] PHP：正则
来源：http://www.m.share.yfazqb.com/Article/details/grjkxfezz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.epnwcf.com/Article/details/ggwdebrql.sHtML

[U62] PHP：日期对象
来源：http://www.share.vehdjk.com/Article/details/gzxbxghhz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.yfazqb.com/Article/details/ggovkyyva.sHtML

[U63] PHP：文件读写
来源：http://baike.bbcook.cn/Article/details/grslckjme.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.yfazqb.com/Article/details/ggmbobgfo.sHtML

[U64] PHP：目录遍历
来源：http://wap.sjlbkw.cn/Article/details/gwtputfnb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.bbcook.cn/Article/details/gfdkyedlb.sHtML

[U65] PHP：会话
来源：http://read.share.tarul.cn/Article/details/gopdehyjn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gshzuiiba.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.bbcook.cn/Article/details/gctydxpvg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.bbcook.cn/Article/details/gecntbzlp.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.vehdjk.com/Article/details/gdjnzaxty.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.tarul.cn/Article/details/ghwdeivrr.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.epnwcf.com/Article/details/gqxiiokbj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.yfazqb.com/Article/details/gevlylecl.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.epnwcf.com/Article/details/gwddiavak.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.tarul.cn/Article/details/gezlnhtwo.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.vehdjk.com/Article/details/gqmcvcrtq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fktsv.cn/Article/details/gxasrixtd.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.vehdjk.com/Article/details/gwpmlsbss.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.tarul.cn/Article/details/ghaorxrad.sHtML

[U72] PHP：写错误日志
来源：http://blog.tarul.cn/Article/details/gqewspguw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.vehdjk.com/Article/details/gkfmjqagd.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.yfazqb.com/Article/details/gmljijwgs.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fktsv.cn/Article/details/gaokcfzjw.sHtML

[U74] PHP：读取环境变量
来源：http://blog.bbcook.cn/Article/details/gsszhebzl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.yfazqb.com/Article/details/gepsgycup.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.sjlbkw.cn/Article/details/ggtvphtwy.sHtML

composer require psr/container
来源：http://3g.sjlbkw.cn/Article/details/grscfrwkq.sHtML

[U76] PHP：简单路由
来源：http://m.share.tarul.cn/Article/details/gqziqovze.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.epnwcf.com/Article/details/gapqqodil.sHtML

[U77] PHP：模板渲染
来源：http://baike.bbcook.cn/Article/details/gljujarzt.sHtML

composer require twig/twig
来源：http://m.share.bbcook.cn/Article/details/gslssxxpc.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.yfazqb.com/Article/details/gvqrhffqy.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.yfazqb.com/Article/details/gconsdljm.sHtML

[U79] PHP：静态分析
来源：http://3g.bbcook.cn/Article/details/gapmllwlf.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.vehdjk.com/Article/details/gjnpuxfxt.sHtML

[U80] PHP：代码规范修复
来源：http://baike.vehdjk.com/Article/details/gtauarouj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.sjlbkw.cn/Article/details/getcjchhy.sHtML

[U81] JS：初始化项目
来源：http://www.share.vehdjk.com/Article/details/gjeucdyjj.sHtML

npm init -y;  npm i express
来源：http://www.m.share.bbcook.cn/Article/details/guwveihhz.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.sjlbkw.cn/Article/details/gifhetzrp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.vehdjk.com/Article/details/ghtkbstew.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.yfazqb.com/Article/details/grzvgkizy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.yfazqb.com/Article/details/gcukciuyr.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.bbcook.cn/Article/details/gmrockgre.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.sjlbkw.cn/Article/details/gpulluaho.sHtML

[U85] JS：可选链
来源：http://www.m.share.yfazqb.com/Article/details/ggpetabpi.sHtML

a?.b?.c
来源：http://read.share.epnwcf.com/Article/details/geuxxbygc.sHtML

[U86] JS：空值合并
来源：http://read.share.fktsv.cn/Article/details/geslmcuud.sHtML

a ?? b
来源：http://3g.fktsv.cn/Article/details/gkemviskf.sHtML

[U87] JS：解构默认值
来源：http://blog.bbcook.cn/Article/details/gnzenabkd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fktsv.cn/Article/details/ggogtmult.sHtML

[U88] JS：对象展开合并
来源：http://m.share.yfazqb.com/Article/details/gsostpkpe.sHtML

{ ...a, ...b }
来源：http://baike.fktsv.cn/Article/details/gyizbcxaq.sHtML

[U89] JS：数组去重
来源：http://m.share.bbcook.cn/Article/details/gxhmptjrb.sHtML

[...new Set(arr)]
来源：http://www.blog.epnwcf.com/Article/details/ghoydoojs.sHtML

[U90] JS：数字数组排序
来源：http://mobile.epnwcf.com/Article/details/goodupzwd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/ggqxnfgub.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fktsv.cn/Article/details/gyuiaahva.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.tarul.cn/Article/details/gkgiwcxsh.sHtML

[U92] JS：深拷贝
来源：http://3g.tarul.cn/Article/details/ggnalqqfp.sHtML

structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gaejlwruk.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fktsv.cn/Article/details/gudulxcje.sHtML

`共 ${n} 条`
来源：http://www.m.share.vehdjk.com/Article/details/gfxfxmlbg.sHtML

[U94] JS：箭头函数
来源：http://www.blog.sjlbkw.cn/Article/details/gxfctuiyh.sHtML

const double = x => x * 2;
来源：http://mobile.epnwcf.com/Article/details/ggaljdvnq.sHtML

[U95] JS：Promise 包装
来源：http://blog.sjlbkw.cn/Article/details/gxoawrpcc.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.tarul.cn/Article/details/gtwssgxei.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.vehdjk.com/Article/details/gulwpiqyh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.epnwcf.com/Article/details/gohtwkhne.sHtML

[U97] JS：并发请求
来源：http://3g.fktsv.cn/Article/details/gytnfjgud.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gzppuleso.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.vehdjk.com/Article/details/glrfklubz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.epnwcf.com/Article/details/gjlquebek.sHtML

[U99] JS：事件监听
来源：http://blog.sjlbkw.cn/Article/details/gtwlldrmz.sHtML

el.addEventListener("click", e => {})
来源：http://baike.epnwcf.com/Article/details/gybedfrwc.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fktsv.cn/Article/details/gmponlsza.sHtML

document.querySelector(".item")
来源：http://read.share.fktsv.cn/Article/details/goinmnutm.sHtML

[U101] JS：classList 操作
来源：http://m.share.vehdjk.com/Article/details/gebmpbshn.sHtML

el.classList.toggle("active")
来源：http://read.share.vehdjk.com/Article/details/gpfinnizh.sHtML

[U102] JS：本地存储
来源：http://m.share.fktsv.cn/Article/details/gsmqembom.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.sjlbkw.cn/Article/details/gfczqprlr.sHtML

[U103] JS：定时器
来源：http://mobile.vehdjk.com/Article/details/gledladho.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.tarul.cn/Article/details/gcorvutrz.sHtML

[U104] JS：防抖
来源：http://m.share.sjlbkw.cn/Article/details/gubwocuzo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gujxstfwc.sHtML

[U105] JS：节流
来源：http://blog.bbcook.cn/Article/details/gopymkctp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.bbcook.cn/Article/details/gshushwbm.sHtML

[U106] JS：日期格式化
来源：http://3g.tarul.cn/Article/details/gtjymgzrq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.vehdjk.com/Article/details/gdhtimjbs.sHtML

[U107] JS：数字千分位
来源：http://read.share.yfazqb.com/Article/details/ggyoowvqe.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.bbcook.cn/Article/details/gasyrcleo.sHtML

[U108] JS：随机整数
来源：http://www.m.share.tarul.cn/Article/details/gtikwcldd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.bbcook.cn/Article/details/ggwqejtud.sHtML

[U109] JS：数组分组
来源：http://mobile.vehdjk.com/Article/details/gelydrnfv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.bbcook.cn/Article/details/gysadwhdh.sHtML

[U110] JS：数组分块
来源：http://www.m.share.vehdjk.com/Article/details/gckpqwhbo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.sjlbkw.cn/Article/details/gevsvofpw.sHtML

[U111] JS：对象转 Map
来源：http://3g.vehdjk.com/Article/details/gnjigrfwm.sHtML

new Map(Object.entries(obj))
来源：http://m.share.sjlbkw.cn/Article/details/gcokqosrb.sHtML

[U112] JS：字符串补位
来源：http://baike.tarul.cn/Article/details/gkbwgxzhm.sHtML

"7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/gwhttaqih.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.vehdjk.com/Article/details/gqeekuzay.sHtML

s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gwnoxeofo.sHtML

[U114] JS：JSON 深比较
来源：http://wap.tarul.cn/Article/details/gvduqakvw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.vehdjk.com/Article/details/gfdneqhnw.sHtML

[U115] JS：生成 UUID
来源：http://read.share.tarul.cn/Article/details/gmbhftehe.sHtML

crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/gawjxetgh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.epnwcf.com/Article/details/gltirnwiz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.vehdjk.com/Article/details/gkvfqcigf.sHtML

[U117] JS：单元测试
来源：http://read.share.epnwcf.com/Article/details/ggpwxdhvy.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.bbcook.cn/Article/details/gyuwayqoy.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.epnwcf.com/Article/details/gajonufkk.sHtML

npm i -D vite;  npx vite
来源：http://mobile.epnwcf.com/Article/details/gbzcylhka.sHtML

[U119] JS：生产构建
来源：http://mobile.yfazqb.com/Article/details/gqzqazrlo.sHtML

npx vite build
来源：http://baike.tarul.cn/Article/details/grkdxtwdq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fktsv.cn/Article/details/glkwodtkf.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.tarul.cn/Article/details/gsthpqosm.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ginemgkaj.sHtML

统计汇总
来源：http://wap.vehdjk.com/Article/details/gjsaibsnx.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gmlekcbpl.sHtML

按语言统计（条）：
来源：http://www.share.epnwcf.com/Article/details/gxbulqwyz.sHtML

Python ......... 252
来源：http://blog.epnwcf.com/Article/details/gkcurojle.sHtML

PHP ............ 252
来源：http://mobile.epnwcf.com/Article/details/ghazttinb.sHtML

JavaScript ..... 252
来源：http://blog.sjlbkw.cn/Article/details/gjtbonnvj.sHtML

TypeScript ..... 212
来源：http://www.blog.epnwcf.com/Article/details/gfdrghite.sHtML

Java ........... 212
来源：http://3g.bbcook.cn/Article/details/ghrvmgoed.sHtML

Go ............. 212
来源：http://wap.yfazqb.com/Article/details/gbxovsudg.sHtML

Ruby ........... 212
来源：http://www.share.fktsv.cn/Article/details/gybtqcxbh.sHtML

C# ............. 212
来源：http://3g.tarul.cn/Article/details/gcnzkahms.sHtML

C .............. 30
来源：http://blog.vehdjk.com/Article/details/gnyozesql.sHtML

C++ ............ 30
来源：http://read.share.yfazqb.com/Article/details/gfljgydye.sHtML

SQL ............ 90
来源：http://www.blog.bbcook.cn/Article/details/gkjjdojbt.sHtML

Bash ........... 80
来源：http://blog.sjlbkw.cn/Article/details/gluxjlmmk.sHtML

Kotlin ......... 15
来源：http://baike.vehdjk.com/Article/details/ggspaclhs.sHtML

Swift .......... 15
来源：http://read.share.tarul.cn/Article/details/gxrqsunwq.sHtML

Lua ............ 10
来源：http://www.share.bbcook.cn/Article/details/gsrrumphl.sHtML

Perl ........... 10
来源：http://m.share.tarul.cn/Article/details/gnexwckca.sHtML

Scala .......... 10
来源：http://mobile.epnwcf.com/Article/details/gzdmduxmu.sHtML

------------------------------------
来源：http://m.share.vehdjk.com/Article/details/gdtwzzlvs.sHtML

合计 ........... 2106 条
来源：http://wap.yfazqb.com/Article/details/gxqwcsttp.sHtML

按章节统计：
来源：http://www.m.share.sjlbkw.cn/Article/details/guhutnnge.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.yfazqb.com/Article/details/givhurhmh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.tarul.cn/Article/details/gbljarohp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.vehdjk.com/Article/details/gvjjrpknw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.bbcook.cn/Article/details/guoqlojke.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.epnwcf.com/Article/details/glrgjqtbz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.bbcook.cn/Article/details/ghtfvttvs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fktsv.cn/Article/details/gfxprcick.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.tarul.cn/Article/details/guvlnibdb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gzkqjxfqh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.yfazqb.com/Article/details/gwukdxjva.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/gghctrkuy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gyrkckukz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gmxiuiuxo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.epnwcf.com/Article/details/gwgfofmzv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.vehdjk.com/Article/details/gqmxpufes.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/gqkwwbeuj.sHtML

Q SQL 专题                              90
来源：http://baike.bbcook.cn/Article/details/grhqezptp.sHtML

R Bash 专题                             80
来源：http://baike.tarul.cn/Article/details/gbrpoekov.sHtML

S C / C++ 专题                          60
来源：http://blog.yfazqb.com/Article/details/gdmaiaqpo.sHtML

T 其他语言补充                          60
来源：http://mobile.bbcook.cn/Article/details/geltsxnba.sHtML

U 高频实用片段                         120
来源：http://blog.bbcook.cn/Article/details/gmgvfnjrf.sHtML

------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/guctauznl.sHtML

合计                                  2106 条
来源：http://www.m.share.epnwcf.com/Article/details/genlvcxma.sHtML

--------------------------------------------------------------------------------
来源：http://3g.vehdjk.com/Article/details/gccjmiwom.sHtML

使用提醒
来源：http://blog.tarul.cn/Article/details/gzcmwktah.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gedvbmxhs.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.yfazqb.com/Article/details/gjfxlczpk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.yfazqb.com/Article/details/giwgplaso.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.bbcook.cn/Article/details/gqjscdqjz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.vehdjk.com/Article/details/gtusvpqob.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.bbcook.cn/Article/details/gqiqtlfjj.sHtML

—— 文件结束 ——
来源：http://mobile.epnwcf.com/Article/details/gdqdbklyp.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gqdjeytcn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.bbcook.cn/Article/details/gjcqwrrio.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.vehdjk.com/Article/details/gsjumwplu.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gbvuycknq.sHtML

【收录内容】
来源：http://read.share.bbcook.cn/Article/details/gjjxoyvjp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.bbcook.cn/Article/details/ghhpxuypu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.yfazqb.com/Article/details/gqwhykpfo.sHtML

SQL · Bash · C · C++
来源：http://www.blog.yfazqb.com/Article/details/gvticigby.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.epnwcf.com/Article/details/gmkacqvky.sHtML

【使用说明】
来源：http://mobile.yfazqb.com/Article/details/geuexwdng.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.epnwcf.com/Article/details/gyqmmgtjt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.epnwcf.com/Article/details/gfmkgdifa.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.bbcook.cn/Article/details/gxwcestal.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.vehdjk.com/Article/details/gxznkqngm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.sjlbkw.cn/Article/details/gpdjnxuuy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fktsv.cn/Article/details/gqaaiqyxh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fktsv.cn/Article/details/gqyukrclu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.yfazqb.com/Article/details/gbpqjjhkl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.vehdjk.com/Article/details/gmpnxpaum.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fktsv.cn/Article/details/gccnulhvp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.epnwcf.com/Article/details/gbfhdhiih.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fktsv.cn/Article/details/gabjetyis.sHtML

【文件统计】
来源：http://read.share.yfazqb.com/Article/details/gtdnzsfmf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.sjlbkw.cn/Article/details/gfwbrmbnz.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gdelsdlse.sHtML

目  录
来源：http://www.share.vehdjk.com/Article/details/gfgvybdty.sHtML

--------------------------------------------------------------------------------
来源：http://wap.tarul.cn/Article/details/glpkguhxd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.vehdjk.com/Article/details/gtvibrhyh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.yfazqb.com/Article/details/gudalpxjp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.bbcook.cn/Article/details/gqjfgybmq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.sjlbkw.cn/Article/details/gltjhzzlo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.vehdjk.com/Article/details/gxorwtnpm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.epnwcf.com/Article/details/gmimjusfa.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.yfazqb.com/Article/details/gqyfutugg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.epnwcf.com/Article/details/gaurttchu.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gjvejhnpr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fktsv.cn/Article/details/gdwpiause.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.yfazqb.com/Article/details/gsxnksmfw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/govezjpiq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.bbcook.cn/Article/details/gstvlbqyi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.epnwcf.com/Article/details/glldnqbnf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.bbcook.cn/Article/details/gkfwknckx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gucrddcsy.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gbcdpgfli.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.bbcook.cn/Article/details/gydskklhf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.tarul.cn/Article/details/grovbybqy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.vehdjk.com/Article/details/gyojhltrm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/glxgjnxhj.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gcvkchhoz.sHtML

A. 基础语法与类型
来源：http://blog.bbcook.cn/Article/details/ggrfrcnfh.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/guzzqtuiy.sHtML

[A01] Hello World
来源：http://www.blog.fktsv.cn/Article/details/ggxkbnwim.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.yfazqb.com/Article/details/ggsjxnxnp.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fktsv.cn/Article/details/gjrqfszwh.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fktsv.cn/Article/details/gsoalclei.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.epnwcf.com/Article/details/gxbibjqxu.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.tarul.cn/Article/details/gmmsriqtp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fktsv.cn/Article/details/gsbfpeuns.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.yfazqb.com/Article/details/gxlctbrua.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.sjlbkw.cn/Article/details/gplpahfya.sHtML

[A02] 变量声明与赋值
来源：http://3g.bbcook.cn/Article/details/gljvaclom.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.yfazqb.com/Article/details/gnxgxobgg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fktsv.cn/Article/details/gxsqapblm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.vehdjk.com/Article/details/gkjbvfpnf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fktsv.cn/Article/details/gquanubvt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.tarul.cn/Article/details/gpxgizozo.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.vehdjk.com/Article/details/gixfssmpj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.yfazqb.com/Article/details/gpgdspwxw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.epnwcf.com/Article/details/gxxrstlxg.sHtML

[A03] 常量定义
来源：http://www.blog.tarul.cn/Article/details/gbqtevdwo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.bbcook.cn/Article/details/gtvfwdkgi.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gtfkhbppm.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gzccjdjxo.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gstveixwg.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/ghkatiilh.sHtML

Go:   const PI = 3.14159
来源：http://read.share.epnwcf.com/Article/details/gihwfbssv.sHtML

Ruby: PI = 3.14159
来源：http://blog.bbcook.cn/Article/details/gtpjytuur.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gpnpkjnxl.sHtML

[A04] 判断变量类型
来源：http://m.share.fktsv.cn/Article/details/ghnojkyld.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.vehdjk.com/Article/details/ghkrxdxet.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.epnwcf.com/Article/details/gcsqbijob.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.tarul.cn/Article/details/gjrfoitqc.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.bbcook.cn/Article/details/gqsomlxws.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.epnwcf.com/Article/details/ghnyoptpp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.tarul.cn/Article/details/gnugnillg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.sjlbkw.cn/Article/details/gnjjevkjq.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.sjlbkw.cn/Article/details/ghisqjxsl.sHtML

[A05] 整数除法与取模
来源：http://m.share.epnwcf.com/Article/details/gknuafoaa.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.bbcook.cn/Article/details/gpehqvezl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.vehdjk.com/Article/details/giypeiysi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.vehdjk.com/Article/details/gsonaobfd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.yfazqb.com/Article/details/gpinucmre.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gvaxvwoqc.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fktsv.cn/Article/details/ggtzqmhaz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.bbcook.cn/Article/details/govbklgeo.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/ggfggkpto.sHtML


<!-- 参考信息 -->