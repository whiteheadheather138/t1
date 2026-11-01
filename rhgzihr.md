代发 wailian999

[U49] PHP：只读属性
来源：http://3g.fktsv.cn/Article/details/gpsnmykfr.sHtML

public readonly string $name
来源：http://www.share.epnwcf.com/Article/details/gsjenvdft.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.epnwcf.com/Article/details/gzmscqhgn.sHtML

public function __construct(private int $id) {}
来源：http://m.share.bbcook.cn/Article/details/gmlniavgg.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fktsv.cn/Article/details/gvfrxsrhs.sHtML

[$a, $b] = $arr;
来源：http://www.blog.bbcook.cn/Article/details/givmvpocd.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fktsv.cn/Article/details/gagcruwez.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.sjlbkw.cn/Article/details/ggdhnbtjn.sHtML

[U53] PHP：空合并运算符
来源：http://wap.vehdjk.com/Article/details/gkiukneit.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.tarul.cn/Article/details/grghsamgz.sHtML

[U54] PHP：空安全调用
来源：http://blog.epnwcf.com/Article/details/gkfvasnls.sHtML

$obj?->method()
来源：http://baike.sjlbkw.cn/Article/details/ggrkfxrcw.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.tarul.cn/Article/details/gzaemkfex.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.bbcook.cn/Article/details/gsawrsavy.sHtML

[U56] PHP：命名参数
来源：http://mobile.sjlbkw.cn/Article/details/gltumizuo.sHtML

f(a: 1, b: 2)
来源：http://blog.tarul.cn/Article/details/gerniildj.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gnbimtlct.sHtML

"值: {$a}"
来源：http://www.share.bbcook.cn/Article/details/gftmjhffs.sHtML

[U58] PHP：数组三件套
来源：http://mobile.epnwcf.com/Article/details/ggtimshio.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.bbcook.cn/Article/details/gjwzhridw.sHtML

[U59] PHP：自定义排序
来源：http://read.share.yfazqb.com/Article/details/gxrjtcpft.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.tarul.cn/Article/details/gyxvfrdoj.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.tarul.cn/Article/details/gdttdndho.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.tarul.cn/Article/details/gpocmqmzw.sHtML

[U61] PHP：正则
来源：http://www.share.tarul.cn/Article/details/ggulucsfn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.sjlbkw.cn/Article/details/gatcdbigm.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.bbcook.cn/Article/details/gpavpepvu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.sjlbkw.cn/Article/details/gmhpaktof.sHtML

[U63] PHP：文件读写
来源：http://read.share.sjlbkw.cn/Article/details/gveseocmg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.tarul.cn/Article/details/gooqlupak.sHtML

[U64] PHP：目录遍历
来源：http://wap.yfazqb.com/Article/details/ghohbvsyj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.tarul.cn/Article/details/gsotuwaew.sHtML

[U65] PHP：会话
来源：http://read.share.tarul.cn/Article/details/gggvcdzkm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.epnwcf.com/Article/details/gbrxmseit.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrfcjpcs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.yfazqb.com/Article/details/gonkchesd.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fktsv.cn/Article/details/gauorlcyh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.vehdjk.com/Article/details/gbqxiznew.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.tarul.cn/Article/details/gynkldnyw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.sjlbkw.cn/Article/details/geatjulhb.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.sjlbkw.cn/Article/details/glpvyfkja.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.tarul.cn/Article/details/gzfefmbsh.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.vehdjk.com/Article/details/gnaznphht.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.epnwcf.com/Article/details/gbxwmlyir.sHtML

[U71] PHP：抛出异常
来源：http://mobile.bbcook.cn/Article/details/goxwwuvpr.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.sjlbkw.cn/Article/details/gfzimmcbx.sHtML

[U72] PHP：写错误日志
来源：http://blog.vehdjk.com/Article/details/gytxebgit.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.bbcook.cn/Article/details/gwqphuvcj.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fktsv.cn/Article/details/gywkcdgzn.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.bbcook.cn/Article/details/ghjngguoh.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.yfazqb.com/Article/details/gacammnbd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.vehdjk.com/Article/details/gihsslzpj.sHtML

[U75] PHP：依赖注入
来源：http://wap.tarul.cn/Article/details/gqsrlynmu.sHtML

composer require psr/container
来源：http://blog.epnwcf.com/Article/details/gojgewoho.sHtML

[U76] PHP：简单路由
来源：http://mobile.tarul.cn/Article/details/gpafkqptc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.tarul.cn/Article/details/ggbbtcfiz.sHtML

[U77] PHP：模板渲染
来源：http://3g.bbcook.cn/Article/details/gjknkciru.sHtML

composer require twig/twig
来源：http://3g.fktsv.cn/Article/details/gqkltzrpq.sHtML

[U78] PHP：单元测试
来源：http://www.blog.vehdjk.com/Article/details/gmuwjcurr.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.vehdjk.com/Article/details/gwubsyrjz.sHtML

[U79] PHP：静态分析
来源：http://blog.sjlbkw.cn/Article/details/gxhbrknfr.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.vehdjk.com/Article/details/gnetzdsbg.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.sjlbkw.cn/Article/details/gsyjgvzeq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.tarul.cn/Article/details/gggbxttob.sHtML

[U81] JS：初始化项目
来源：http://baike.sjlbkw.cn/Article/details/gpvulkbqc.sHtML

npm init -y;  npm i express
来源：http://blog.epnwcf.com/Article/details/gphcwpwbn.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fktsv.cn/Article/details/glpdokhyx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.epnwcf.com/Article/details/gzgvyupwd.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.tarul.cn/Article/details/gbaqkdkci.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.epnwcf.com/Article/details/givbkoqrj.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.tarul.cn/Article/details/gffrqfacu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.bbcook.cn/Article/details/gyfjcqxyp.sHtML

[U85] JS：可选链
来源：http://blog.vehdjk.com/Article/details/gtpiwohqf.sHtML

a?.b?.c
来源：http://3g.vehdjk.com/Article/details/gybzkfifv.sHtML

[U86] JS：空值合并
来源：http://wap.vehdjk.com/Article/details/gephtvnqu.sHtML

a ?? b
来源：http://baike.vehdjk.com/Article/details/gmlpyicgi.sHtML

[U87] JS：解构默认值
来源：http://blog.vehdjk.com/Article/details/gqwhkzkoi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.yfazqb.com/Article/details/gbhsugvtl.sHtML

[U88] JS：对象展开合并
来源：http://mobile.epnwcf.com/Article/details/gtrllinhj.sHtML

{ ...a, ...b }
来源：http://m.share.yfazqb.com/Article/details/gzawnxtgm.sHtML

[U89] JS：数组去重
来源：http://mobile.sjlbkw.cn/Article/details/gngbccozz.sHtML

[...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gkrtkspvk.sHtML

[U90] JS：数字数组排序
来源：http://3g.fktsv.cn/Article/details/gvjkkcvwq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gtlaqmkyi.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.vehdjk.com/Article/details/ghkqvwafo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.vehdjk.com/Article/details/gqpbkbjks.sHtML

[U92] JS：深拷贝
来源：http://read.share.bbcook.cn/Article/details/gzmseapwe.sHtML

structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/guiqlnkgd.sHtML

[U93] JS：模板字符串
来源：http://blog.epnwcf.com/Article/details/ggrmswtpn.sHtML

`共 ${n} 条`
来源：http://wap.vehdjk.com/Article/details/gfluxoxiv.sHtML

[U94] JS：箭头函数
来源：http://mobile.epnwcf.com/Article/details/glfmnomqr.sHtML

const double = x => x * 2;
来源：http://read.share.vehdjk.com/Article/details/gxqlergzr.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsektlfx.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.epnwcf.com/Article/details/gkdnkztxo.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fktsv.cn/Article/details/ggpppitvg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/gnrityyba.sHtML

[U97] JS：并发请求
来源：http://www.blog.sjlbkw.cn/Article/details/gyabxhejm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/gmcepbyvv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.bbcook.cn/Article/details/gtxjnpaly.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.epnwcf.com/Article/details/gsgnxweir.sHtML

[U99] JS：事件监听
来源：http://read.share.fktsv.cn/Article/details/gtydgfohz.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.tarul.cn/Article/details/gmfmdfdyn.sHtML

[U100] JS：DOM 查询
来源：http://baike.bbcook.cn/Article/details/guatkxzpj.sHtML

document.querySelector(".item")
来源：http://baike.vehdjk.com/Article/details/gxtesjany.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.tarul.cn/Article/details/gaerzkkwv.sHtML

el.classList.toggle("active")
来源：http://read.share.tarul.cn/Article/details/gmafzczlh.sHtML

[U102] JS：本地存储
来源：http://www.blog.yfazqb.com/Article/details/gifgbpllq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.epnwcf.com/Article/details/grqpbwnba.sHtML

[U103] JS：定时器
来源：http://wap.vehdjk.com/Article/details/gwxyypeql.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.sjlbkw.cn/Article/details/glopqwivu.sHtML

[U104] JS：防抖
来源：http://www.blog.sjlbkw.cn/Article/details/gltodygvv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.yfazqb.com/Article/details/gymfrevqp.sHtML

[U105] JS：节流
来源：http://www.m.share.tarul.cn/Article/details/gtbdngnrz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.vehdjk.com/Article/details/gugejsroe.sHtML

[U106] JS：日期格式化
来源：http://mobile.fktsv.cn/Article/details/gfamnnspc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.yfazqb.com/Article/details/ganfysvfp.sHtML

[U107] JS：数字千分位
来源：http://read.share.bbcook.cn/Article/details/gcklslmft.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.yfazqb.com/Article/details/gwdmeqoma.sHtML

[U108] JS：随机整数
来源：http://3g.bbcook.cn/Article/details/gvvonosqn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.vehdjk.com/Article/details/gdyulzplx.sHtML

[U109] JS：数组分组
来源：http://wap.vehdjk.com/Article/details/gekruqapk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.yfazqb.com/Article/details/gvevzfztv.sHtML

[U110] JS：数组分块
来源：http://3g.vehdjk.com/Article/details/gqrhfbnal.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.tarul.cn/Article/details/gtafbachn.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fktsv.cn/Article/details/gltxnnrvt.sHtML

new Map(Object.entries(obj))
来源：http://blog.yfazqb.com/Article/details/gwwekuono.sHtML

[U112] JS：字符串补位
来源：http://blog.epnwcf.com/Article/details/ghgtkrgtk.sHtML

"7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gfdotrfdu.sHtML

[U113] JS：正则替换全部
来源：http://wap.fktsv.cn/Article/details/glumrhdaz.sHtML

s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gsmuobcvc.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.yfazqb.com/Article/details/gcpslfmnn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.yfazqb.com/Article/details/gzfuszoyk.sHtML

[U115] JS：生成 UUID
来源：http://read.share.epnwcf.com/Article/details/gtlnttgdj.sHtML

crypto.randomUUID()
来源：http://mobile.yfazqb.com/Article/details/gplposfqk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.tarul.cn/Article/details/ghrdnueyp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.tarul.cn/Article/details/gqwyzkybe.sHtML

[U117] JS：单元测试
来源：http://www.m.share.yfazqb.com/Article/details/gjodhoyas.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.tarul.cn/Article/details/ggnhxewyl.sHtML

[U118] JS：开发服务器
来源：http://3g.yfazqb.com/Article/details/gwcripdlt.sHtML

npm i -D vite;  npx vite
来源：http://read.share.yfazqb.com/Article/details/gfetowhun.sHtML

[U119] JS：生产构建
来源：http://www.m.share.bbcook.cn/Article/details/gwsmtnaxj.sHtML

npx vite build
来源：http://blog.fktsv.cn/Article/details/ggqefkzby.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.epnwcf.com/Article/details/gyomcgtsu.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.vehdjk.com/Article/details/giysdgddr.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gleycbmdb.sHtML

统计汇总
来源：http://wap.fktsv.cn/Article/details/gsoxikcdg.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gbyqoordb.sHtML

按语言统计（条）：
来源：http://blog.sjlbkw.cn/Article/details/gzbkjadps.sHtML

Python ......... 252
来源：http://mobile.fktsv.cn/Article/details/glarcrxxo.sHtML

PHP ............ 252
来源：http://mobile.sjlbkw.cn/Article/details/gbjvmdmim.sHtML

JavaScript ..... 252
来源：http://baike.vehdjk.com/Article/details/gugduthog.sHtML

TypeScript ..... 212
来源：http://www.share.sjlbkw.cn/Article/details/gcnlqtshc.sHtML

Java ........... 212
来源：http://blog.epnwcf.com/Article/details/gtkodsddo.sHtML

Go ............. 212
来源：http://www.blog.tarul.cn/Article/details/ghpyqiink.sHtML

Ruby ........... 212
来源：http://m.share.epnwcf.com/Article/details/gzaqnxyfp.sHtML

C# ............. 212
来源：http://wap.bbcook.cn/Article/details/geddxkqru.sHtML

C .............. 30
来源：http://read.share.tarul.cn/Article/details/gyzhnfuig.sHtML

C++ ............ 30
来源：http://wap.yfazqb.com/Article/details/gspjtuadt.sHtML

SQL ............ 90
来源：http://3g.vehdjk.com/Article/details/ggpbestet.sHtML

Bash ........... 80
来源：http://3g.epnwcf.com/Article/details/gyhinqqck.sHtML

Kotlin ......... 15
来源：http://www.blog.tarul.cn/Article/details/golbokcgr.sHtML

Swift .......... 15
来源：http://mobile.tarul.cn/Article/details/gtneneero.sHtML

Lua ............ 10
来源：http://www.share.yfazqb.com/Article/details/gnfbqmjxf.sHtML

Perl ........... 10
来源：http://baike.epnwcf.com/Article/details/gvvdxqwrz.sHtML

Scala .......... 10
来源：http://m.share.fktsv.cn/Article/details/gvsvglzwu.sHtML

------------------------------------
来源：http://wap.yfazqb.com/Article/details/gkhldburh.sHtML

合计 ........... 2106 条
来源：http://www.blog.sjlbkw.cn/Article/details/gdmafxyws.sHtML

按章节统计：
来源：http://mobile.fktsv.cn/Article/details/gtxyjnmoi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.tarul.cn/Article/details/gaofxzzqm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.vehdjk.com/Article/details/gtyodfebv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.vehdjk.com/Article/details/gutlqzqeq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.bbcook.cn/Article/details/gjjozmwku.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.epnwcf.com/Article/details/ghykhoegv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.vehdjk.com/Article/details/gfukgszmn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.tarul.cn/Article/details/gmrpeyzcf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fktsv.cn/Article/details/gnhjygiet.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.bbcook.cn/Article/details/gxswpmtye.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fktsv.cn/Article/details/gpdcaqmkj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/gkadjkoqy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gcdrvpkqg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gejoftrgt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgeesudk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fktsv.cn/Article/details/gfepwfovh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/gmoghepft.sHtML

Q SQL 专题                              90
来源：http://mobile.sjlbkw.cn/Article/details/guufpeldu.sHtML

R Bash 专题                             80
来源：http://baike.bbcook.cn/Article/details/garwjxnec.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.epnwcf.com/Article/details/gkdbplisg.sHtML

T 其他语言补充                          60
来源：http://blog.bbcook.cn/Article/details/gmguojcxe.sHtML

U 高频实用片段                         120
来源：http://m.share.sjlbkw.cn/Article/details/gbsbppzkc.sHtML

------------------------------------
来源：http://3g.yfazqb.com/Article/details/gkrtrdsqr.sHtML

合计                                  2106 条
来源：http://blog.vehdjk.com/Article/details/gdkkqjvus.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/gsywmgwhw.sHtML

使用提醒
来源：http://www.share.tarul.cn/Article/details/gsqkwegwz.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.tarul.cn/Article/details/gsisoifat.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.yfazqb.com/Article/details/gbtweeasj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fktsv.cn/Article/details/glodqqyup.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.tarul.cn/Article/details/givjbrbnt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.sjlbkw.cn/Article/details/gapydmrzd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.vehdjk.com/Article/details/gnefouxna.sHtML

—— 文件结束 ——
来源：http://3g.fktsv.cn/Article/details/guwrfaxun.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gaztmfzgp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fktsv.cn/Article/details/gbohcxsnf.sHtML

Common Programming Examples Cheat Book
来源：http://wap.yfazqb.com/Article/details/gmhoyqwzi.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gxkafhslr.sHtML

【收录内容】
来源：http://wap.vehdjk.com/Article/details/ggngxhlbn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.yfazqb.com/Article/details/gcqtsjdgq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.vehdjk.com/Article/details/gmsbmodtm.sHtML

SQL · Bash · C · C++
来源：http://www.share.vehdjk.com/Article/details/gcxnonzod.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fktsv.cn/Article/details/gfulcjbuo.sHtML

【使用说明】
来源：http://www.share.vehdjk.com/Article/details/gjzarilzg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.tarul.cn/Article/details/ggujnkdrm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.bbcook.cn/Article/details/gultwtvhs.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.bbcook.cn/Article/details/gmskjhjvv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.yfazqb.com/Article/details/gdsixpydb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.tarul.cn/Article/details/gswvkvmom.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.bbcook.cn/Article/details/galiupgmn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.vehdjk.com/Article/details/ghoholcxa.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.sjlbkw.cn/Article/details/gdtcmpcwc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.vehdjk.com/Article/details/gzaqixlkt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.vehdjk.com/Article/details/gyqnqsmhf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.yfazqb.com/Article/details/gdkqicwum.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.vehdjk.com/Article/details/gbabhyhop.sHtML

【文件统计】
来源：http://baike.tarul.cn/Article/details/gyjsxrjkj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fktsv.cn/Article/details/gocotzsyo.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/ghzffecfe.sHtML

目  录
来源：http://read.share.yfazqb.com/Article/details/gvhcwwikm.sHtML

--------------------------------------------------------------------------------
来源：http://baike.bbcook.cn/Article/details/gehickkij.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fktsv.cn/Article/details/gynjdsbvl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.tarul.cn/Article/details/gbhyrpfvx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fktsv.cn/Article/details/gohshxwce.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.vehdjk.com/Article/details/gnvpzykvb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.epnwcf.com/Article/details/groprrgkq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.sjlbkw.cn/Article/details/gwucqfrle.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.sjlbkw.cn/Article/details/gthsxocjc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.vehdjk.com/Article/details/gfrlpnujn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.bbcook.cn/Article/details/ghmvvtalh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.bbcook.cn/Article/details/gtfbcnjmy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqfzbhbm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/gwldboasp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gjuhwjawp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.bbcook.cn/Article/details/gbpqazyai.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.tarul.cn/Article/details/gfdsrmnyw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.epnwcf.com/Article/details/gnrgpfyfc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.vehdjk.com/Article/details/gfmqyplld.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.sjlbkw.cn/Article/details/gtssjghvr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.sjlbkw.cn/Article/details/gbradynry.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.tarul.cn/Article/details/gylarwiah.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.tarul.cn/Article/details/gfpiotwgq.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gzhjkslil.sHtML

A. 基础语法与类型
来源：http://www.m.share.tarul.cn/Article/details/gvewqmmlw.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gggewsiuz.sHtML

[A01] Hello World
来源：http://blog.vehdjk.com/Article/details/gohniptoc.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fktsv.cn/Article/details/gmxvylabz.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.bbcook.cn/Article/details/gpqvrskxa.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.vehdjk.com/Article/details/ggyxivlvg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.tarul.cn/Article/details/gqbactnky.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.sjlbkw.cn/Article/details/gakqsuztc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.sjlbkw.cn/Article/details/gvamdqrgd.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.vehdjk.com/Article/details/geyquuwiw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fktsv.cn/Article/details/gigzsaczu.sHtML

[A02] 变量声明与赋值
来源：http://m.share.yfazqb.com/Article/details/gijyrsohs.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.vehdjk.com/Article/details/gmexfoikd.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.epnwcf.com/Article/details/gsxrjarvd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.tarul.cn/Article/details/gmhzoanjs.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.vehdjk.com/Article/details/ggenfwzcn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.yfazqb.com/Article/details/ggctsqyym.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.sjlbkw.cn/Article/details/geasasqck.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fktsv.cn/Article/details/glapvffaf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.tarul.cn/Article/details/gaivfvten.sHtML

[A03] 常量定义
来源：http://www.blog.bbcook.cn/Article/details/gikfhvbok.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.bbcook.cn/Article/details/gnnnjizqa.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gsuqzbhww.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gvhaulstj.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gagobwquq.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gmslcylcc.sHtML

Go:   const PI = 3.14159
来源：http://wap.bbcook.cn/Article/details/gavdozbxz.sHtML

Ruby: PI = 3.14159
来源：http://read.share.bbcook.cn/Article/details/gsovqdpdq.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gkzcykaxc.sHtML

[A04] 判断变量类型
来源：http://mobile.yfazqb.com/Article/details/gkddcpjbx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.sjlbkw.cn/Article/details/gxwnknwxf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.bbcook.cn/Article/details/gulqyswke.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.bbcook.cn/Article/details/gftdgkukg.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.yfazqb.com/Article/details/gnufbioby.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.tarul.cn/Article/details/gsxbsmzhd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.epnwcf.com/Article/details/gbzcbwfzj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.yfazqb.com/Article/details/gestrqmjj.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.tarul.cn/Article/details/golvywqsf.sHtML

[A05] 整数除法与取模
来源：http://www.blog.tarul.cn/Article/details/gffvxuxde.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.yfazqb.com/Article/details/gxhywdjhc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gzmdowlxv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.bbcook.cn/Article/details/gixzhtezx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gexntzhvp.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.tarul.cn/Article/details/gbmxyojgi.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/ghmenvzxo.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.yfazqb.com/Article/details/gugamxjic.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.bbcook.cn/Article/details/gvghahzfz.sHtML

[A06] 字符串转数字
来源：http://3g.tarul.cn/Article/details/gluagnloj.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.sjlbkw.cn/Article/details/gopomomsw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.yfazqb.com/Article/details/gzfdjbndb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.epnwcf.com/Article/details/ghitosgnz.sHtML


<!-- 参考信息 -->