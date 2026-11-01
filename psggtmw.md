代发 wailian999

[U49] PHP：只读属性
来源：http://www.blog.sjlbkw.cn/Article/details/gxhrczdul.sHtML

public readonly string $name
来源：http://m.share.yfazqb.com/Article/details/ggmxzrqzo.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.yfazqb.com/Article/details/gxojgxzag.sHtML

public function __construct(private int $id) {}
来源：http://read.share.sjlbkw.cn/Article/details/gofhszzig.sHtML

[U51] PHP：数组解构
来源：http://3g.vehdjk.com/Article/details/gwhwmavtk.sHtML

[$a, $b] = $arr;
来源：http://mobile.fktsv.cn/Article/details/gvzikuqal.sHtML

[U52] PHP：箭头函数
来源：http://m.share.vehdjk.com/Article/details/gtdfwjklg.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.vehdjk.com/Article/details/gxdltorkx.sHtML

[U53] PHP：空合并运算符
来源：http://wap.yfazqb.com/Article/details/gzeahbyid.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.sjlbkw.cn/Article/details/gliolrizu.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.bbcook.cn/Article/details/gxklshqwt.sHtML

$obj?->method()
来源：http://m.share.vehdjk.com/Article/details/gbqufqchs.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.yfazqb.com/Article/details/gmhgzrdwb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.tarul.cn/Article/details/gelnvdxhd.sHtML

[U56] PHP：命名参数
来源：http://www.blog.vehdjk.com/Article/details/gkjxdgred.sHtML

f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/gcjlbcnrl.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gmywulqik.sHtML

"值: {$a}"
来源：http://www.blog.vehdjk.com/Article/details/gaokqalby.sHtML

[U58] PHP：数组三件套
来源：http://3g.bbcook.cn/Article/details/ghyxwjopn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.bbcook.cn/Article/details/gvpnecbdt.sHtML

[U59] PHP：自定义排序
来源：http://blog.bbcook.cn/Article/details/gwidcyiym.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.epnwcf.com/Article/details/gamtksees.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.bbcook.cn/Article/details/gjfnnetvw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.sjlbkw.cn/Article/details/gpjzboxpi.sHtML

[U61] PHP：正则
来源：http://mobile.yfazqb.com/Article/details/gwkyifijk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gqxerkmdt.sHtML

[U62] PHP：日期对象
来源：http://blog.tarul.cn/Article/details/gqqoahwtg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.yfazqb.com/Article/details/grkeoousa.sHtML

[U63] PHP：文件读写
来源：http://www.blog.epnwcf.com/Article/details/gzmgefbic.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.epnwcf.com/Article/details/gepqnyakz.sHtML

[U64] PHP：目录遍历
来源：http://3g.tarul.cn/Article/details/gbkoqubrz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.sjlbkw.cn/Article/details/gqlmacdis.sHtML

[U65] PHP：会话
来源：http://mobile.vehdjk.com/Article/details/gijklhcda.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.epnwcf.com/Article/details/gybgutpgv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.bbcook.cn/Article/details/gyefxflzy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.bbcook.cn/Article/details/gulzpetdu.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.yfazqb.com/Article/details/ggrpuexku.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.bbcook.cn/Article/details/gejwmftca.sHtML

[U68] PHP：PDO 连接
来源：http://baike.yfazqb.com/Article/details/gedbdiukw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.epnwcf.com/Article/details/gytikieqh.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fktsv.cn/Article/details/gtjjvaifj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.bbcook.cn/Article/details/gahpjrras.sHtML

[U70] PHP：PDO 事务
来源：http://baike.epnwcf.com/Article/details/gbbyfnmgj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.tarul.cn/Article/details/gnyzbcepp.sHtML

[U71] PHP：抛出异常
来源：http://baike.tarul.cn/Article/details/gbuonwqqy.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.bbcook.cn/Article/details/gnuadjqfe.sHtML

[U72] PHP：写错误日志
来源：http://www.share.yfazqb.com/Article/details/glmaabbee.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.yfazqb.com/Article/details/gwlrousio.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.epnwcf.com/Article/details/geuzcrgzd.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.epnwcf.com/Article/details/gopzuvynp.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fktsv.cn/Article/details/gevcrpgkr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.tarul.cn/Article/details/gmojjcmod.sHtML

[U75] PHP：依赖注入
来源：http://mobile.vehdjk.com/Article/details/gzveqkmtu.sHtML

composer require psr/container
来源：http://3g.bbcook.cn/Article/details/gvirhbtnb.sHtML

[U76] PHP：简单路由
来源：http://3g.tarul.cn/Article/details/gvpahztrq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.bbcook.cn/Article/details/gqfjxslbg.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.yfazqb.com/Article/details/gmiiclqhx.sHtML

composer require twig/twig
来源：http://baike.tarul.cn/Article/details/gwrmdbvjp.sHtML

[U78] PHP：单元测试
来源：http://blog.bbcook.cn/Article/details/gfqhnvioq.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.epnwcf.com/Article/details/gbxfrgope.sHtML

[U79] PHP：静态分析
来源：http://m.share.fktsv.cn/Article/details/gvoflaytr.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.sjlbkw.cn/Article/details/gitwkicio.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fktsv.cn/Article/details/gkdxfiggq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.sjlbkw.cn/Article/details/gbfumbumt.sHtML

[U81] JS：初始化项目
来源：http://www.share.vehdjk.com/Article/details/gkcnjbzbs.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fktsv.cn/Article/details/gvdnqhqeh.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.yfazqb.com/Article/details/gelcmwqrs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.tarul.cn/Article/details/gpuqfhylg.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.tarul.cn/Article/details/gmrfxwpul.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.vehdjk.com/Article/details/goxbvpogp.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.bbcook.cn/Article/details/glbskrhtq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.vehdjk.com/Article/details/gsurnnrgv.sHtML

[U85] JS：可选链
来源：http://www.blog.epnwcf.com/Article/details/guxkljvvq.sHtML

a?.b?.c
来源：http://baike.vehdjk.com/Article/details/gkuplbgwd.sHtML

[U86] JS：空值合并
来源：http://baike.sjlbkw.cn/Article/details/gnsvqmonw.sHtML

a ?? b
来源：http://www.m.share.epnwcf.com/Article/details/ggrtkrgwq.sHtML

[U87] JS：解构默认值
来源：http://mobile.bbcook.cn/Article/details/gnwszaeyd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.sjlbkw.cn/Article/details/genwamrbt.sHtML

[U88] JS：对象展开合并
来源：http://wap.bbcook.cn/Article/details/gsospcrqz.sHtML

{ ...a, ...b }
来源：http://m.share.epnwcf.com/Article/details/godvwuelg.sHtML

[U89] JS：数组去重
来源：http://baike.sjlbkw.cn/Article/details/ggjjaztgg.sHtML

[...new Set(arr)]
来源：http://www.m.share.fktsv.cn/Article/details/gexfamlxf.sHtML

[U90] JS：数字数组排序
来源：http://baike.vehdjk.com/Article/details/gwuvfhrvo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.tarul.cn/Article/details/gvtqhaigb.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.vehdjk.com/Article/details/gxddprkpb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fktsv.cn/Article/details/gyoklksei.sHtML

[U92] JS：深拷贝
来源：http://3g.bbcook.cn/Article/details/gkaqmluqz.sHtML

structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gmxfqhlti.sHtML

[U93] JS：模板字符串
来源：http://blog.sjlbkw.cn/Article/details/gmatjcuib.sHtML

`共 ${n} 条`
来源：http://www.m.share.tarul.cn/Article/details/gyamrjlpk.sHtML

[U94] JS：箭头函数
来源：http://read.share.tarul.cn/Article/details/gakescxql.sHtML

const double = x => x * 2;
来源：http://blog.yfazqb.com/Article/details/gnmjulwbe.sHtML

[U95] JS：Promise 包装
来源：http://wap.yfazqb.com/Article/details/ghbydzwuu.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.epnwcf.com/Article/details/ghxszezql.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.bbcook.cn/Article/details/gyxddsqex.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/gmxmgbavy.sHtML

[U97] JS：并发请求
来源：http://wap.tarul.cn/Article/details/giasuagkn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gnjzesqmu.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.tarul.cn/Article/details/gljxwhjkg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.epnwcf.com/Article/details/gbmflbdxr.sHtML

[U99] JS：事件监听
来源：http://read.share.vehdjk.com/Article/details/gfjlppqro.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.epnwcf.com/Article/details/gtdgzqiqh.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fktsv.cn/Article/details/gaqhzmozb.sHtML

document.querySelector(".item")
来源：http://www.blog.sjlbkw.cn/Article/details/gxswtatyk.sHtML

[U101] JS：classList 操作
来源：http://www.blog.yfazqb.com/Article/details/gceieljvz.sHtML

el.classList.toggle("active")
来源：http://www.share.vehdjk.com/Article/details/gotdsdsmr.sHtML

[U102] JS：本地存储
来源：http://www.share.tarul.cn/Article/details/gfowzbohp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.epnwcf.com/Article/details/gesaboffx.sHtML

[U103] JS：定时器
来源：http://read.share.tarul.cn/Article/details/girrhurnn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.sjlbkw.cn/Article/details/gvhvdrzlq.sHtML

[U104] JS：防抖
来源：http://m.share.tarul.cn/Article/details/gfmlsshwn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/gytojvhpk.sHtML

[U105] JS：节流
来源：http://www.share.sjlbkw.cn/Article/details/gjvushvjw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.tarul.cn/Article/details/gobmrmjph.sHtML

[U106] JS：日期格式化
来源：http://blog.bbcook.cn/Article/details/grqdbjxnc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fktsv.cn/Article/details/gfjqoczjt.sHtML

[U107] JS：数字千分位
来源：http://blog.sjlbkw.cn/Article/details/gboebkkwh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/ggsviccye.sHtML

[U108] JS：随机整数
来源：http://blog.epnwcf.com/Article/details/gyibnxefe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fktsv.cn/Article/details/gfsbzltgi.sHtML

[U109] JS：数组分组
来源：http://read.share.vehdjk.com/Article/details/gzswvlbec.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.vehdjk.com/Article/details/gzrvzahky.sHtML

[U110] JS：数组分块
来源：http://www.m.share.epnwcf.com/Article/details/gxmkephgt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.vehdjk.com/Article/details/gftqtrttl.sHtML

[U111] JS：对象转 Map
来源：http://wap.bbcook.cn/Article/details/gczvujpac.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.vehdjk.com/Article/details/grcmaefdr.sHtML

[U112] JS：字符串补位
来源：http://www.blog.bbcook.cn/Article/details/gaedreufx.sHtML

"7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gtyywhsiw.sHtML

[U113] JS：正则替换全部
来源：http://blog.tarul.cn/Article/details/gktiugzvh.sHtML

s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/glpjdqcmg.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.sjlbkw.cn/Article/details/gdgozwlbm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fktsv.cn/Article/details/gmrvzmcsb.sHtML

[U115] JS：生成 UUID
来源：http://read.share.bbcook.cn/Article/details/gnesgheiz.sHtML

crypto.randomUUID()
来源：http://www.blog.vehdjk.com/Article/details/ghvyszroq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.sjlbkw.cn/Article/details/grzndkuuv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.yfazqb.com/Article/details/gcmunrtri.sHtML

[U117] JS：单元测试
来源：http://www.blog.fktsv.cn/Article/details/gkgxmaugj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.epnwcf.com/Article/details/genayzfga.sHtML

[U118] JS：开发服务器
来源：http://mobile.vehdjk.com/Article/details/gjtdywuck.sHtML

npm i -D vite;  npx vite
来源：http://baike.bbcook.cn/Article/details/gocysesmq.sHtML

[U119] JS：生产构建
来源：http://mobile.fktsv.cn/Article/details/gjuxgrhgs.sHtML

npx vite build
来源：http://wap.sjlbkw.cn/Article/details/gyeucvzij.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.tarul.cn/Article/details/gqndmjcsb.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.yfazqb.com/Article/details/glcpcytpx.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gzilipuzg.sHtML

统计汇总
来源：http://m.share.fktsv.cn/Article/details/gqzxrzesu.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ghurluecf.sHtML

按语言统计（条）：
来源：http://read.share.sjlbkw.cn/Article/details/gcfiticgn.sHtML

Python ......... 252
来源：http://blog.fktsv.cn/Article/details/gddhbxrqp.sHtML

PHP ............ 252
来源：http://m.share.yfazqb.com/Article/details/gyleffivw.sHtML

JavaScript ..... 252
来源：http://www.share.epnwcf.com/Article/details/gfvyyqanx.sHtML

TypeScript ..... 212
来源：http://www.blog.yfazqb.com/Article/details/gouzilutj.sHtML

Java ........... 212
来源：http://wap.bbcook.cn/Article/details/gjreubzsl.sHtML

Go ............. 212
来源：http://blog.sjlbkw.cn/Article/details/gkzdnvxui.sHtML

Ruby ........... 212
来源：http://3g.epnwcf.com/Article/details/gzprjqrjf.sHtML

C# ............. 212
来源：http://mobile.epnwcf.com/Article/details/gbifkymsa.sHtML

C .............. 30
来源：http://www.blog.vehdjk.com/Article/details/gwpzbpebi.sHtML

C++ ............ 30
来源：http://mobile.sjlbkw.cn/Article/details/gdibrvmxq.sHtML

SQL ............ 90
来源：http://www.share.vehdjk.com/Article/details/gvxrippnf.sHtML

Bash ........... 80
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcbafpac.sHtML

Kotlin ......... 15
来源：http://baike.yfazqb.com/Article/details/gqtbbfxkn.sHtML

Swift .......... 15
来源：http://www.blog.sjlbkw.cn/Article/details/ggyhvhsdu.sHtML

Lua ............ 10
来源：http://www.share.tarul.cn/Article/details/gespowlpd.sHtML

Perl ........... 10
来源：http://www.share.sjlbkw.cn/Article/details/gbjtneept.sHtML

Scala .......... 10
来源：http://m.share.tarul.cn/Article/details/ghtiqqlqm.sHtML

------------------------------------
来源：http://read.share.tarul.cn/Article/details/gjgyyhfxx.sHtML

合计 ........... 2106 条
来源：http://mobile.sjlbkw.cn/Article/details/gizxxcsxv.sHtML

按章节统计：
来源：http://baike.fktsv.cn/Article/details/gzhdpothc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.yfazqb.com/Article/details/gygxjgpva.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.tarul.cn/Article/details/gajoqbgmd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.epnwcf.com/Article/details/gptdnltkw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.tarul.cn/Article/details/gdueozowo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.bbcook.cn/Article/details/ggeugaxiy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fktsv.cn/Article/details/gifywgdsf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.tarul.cn/Article/details/gitkovjrc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.sjlbkw.cn/Article/details/gvikymohr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gexbymgwm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.vehdjk.com/Article/details/grsbswqdo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/ggprxlruh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/grgoezmaj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/gesjvised.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fktsv.cn/Article/details/glupabiwa.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.yfazqb.com/Article/details/gtmqpqlrf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/glprgojjs.sHtML

Q SQL 专题                              90
来源：http://m.share.sjlbkw.cn/Article/details/gcaauvhxp.sHtML

R Bash 专题                             80
来源：http://www.blog.epnwcf.com/Article/details/giudstqck.sHtML

S C / C++ 专题                          60
来源：http://wap.tarul.cn/Article/details/grmykstkr.sHtML

T 其他语言补充                          60
来源：http://baike.bbcook.cn/Article/details/gccrxfmuz.sHtML

U 高频实用片段                         120
来源：http://read.share.epnwcf.com/Article/details/ghtaksqgh.sHtML

------------------------------------
来源：http://blog.yfazqb.com/Article/details/gvihhqrfj.sHtML

合计                                  2106 条
来源：http://m.share.sjlbkw.cn/Article/details/gfnwnhbbm.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fktsv.cn/Article/details/gregnvvvn.sHtML

使用提醒
来源：http://wap.fktsv.cn/Article/details/gtysrcndc.sHtML

--------------------------------------------------------------------------------
来源：http://baike.vehdjk.com/Article/details/gpplcstjk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.epnwcf.com/Article/details/gsuvyvnci.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.tarul.cn/Article/details/gllmvlipi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.yfazqb.com/Article/details/gknvjwyan.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fktsv.cn/Article/details/gfgnhlxii.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.tarul.cn/Article/details/gkzqppfmi.sHtML

—— 文件结束 ——
来源：http://mobile.epnwcf.com/Article/details/gfaymxncx.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gpevjfscu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.yfazqb.com/Article/details/gpdpvminx.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fktsv.cn/Article/details/gabdyxrrb.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gwpsqoesw.sHtML

【收录内容】
来源：http://www.share.tarul.cn/Article/details/gghgnxmzq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.vehdjk.com/Article/details/gsckjrpch.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.vehdjk.com/Article/details/gufchqaek.sHtML

SQL · Bash · C · C++
来源：http://www.share.sjlbkw.cn/Article/details/gegswczab.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.epnwcf.com/Article/details/ggynglzhj.sHtML

【使用说明】
来源：http://www.share.epnwcf.com/Article/details/ggxtiperx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.bbcook.cn/Article/details/ggtgyuzcs.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.vehdjk.com/Article/details/ginifduvn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.epnwcf.com/Article/details/gijrtlpow.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.vehdjk.com/Article/details/ghefxdpcc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.epnwcf.com/Article/details/gzfmihzax.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.vehdjk.com/Article/details/gjshnfyho.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.yfazqb.com/Article/details/gyhkkuuwu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fktsv.cn/Article/details/gsvcjdryg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.epnwcf.com/Article/details/gyhdopgtj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.bbcook.cn/Article/details/gqsvkucic.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.tarul.cn/Article/details/ginqzcyad.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.epnwcf.com/Article/details/gfsycgeis.sHtML

【文件统计】
来源：http://3g.bbcook.cn/Article/details/ghkdavmbj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.yfazqb.com/Article/details/gjtzpputi.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/ggdqggitf.sHtML

目  录
来源：http://blog.epnwcf.com/Article/details/gsqoihqra.sHtML

--------------------------------------------------------------------------------
来源：http://baike.bbcook.cn/Article/details/gndmmlppn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.tarul.cn/Article/details/gfybzmtqx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.yfazqb.com/Article/details/gxozcnbqg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fktsv.cn/Article/details/gncsrmhxx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.yfazqb.com/Article/details/greheblgp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.epnwcf.com/Article/details/gxbtgydjf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.vehdjk.com/Article/details/gmtgjsnoc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.vehdjk.com/Article/details/gudqbvidw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.tarul.cn/Article/details/gnlgxhrju.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/gjjnqkxcb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.bbcook.cn/Article/details/gcpbyvuoq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.bbcook.cn/Article/details/ggxgdriug.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/gfpirfsya.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/gbnzfpcim.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.epnwcf.com/Article/details/gtxgijjgm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.yfazqb.com/Article/details/glsxakvcj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fktsv.cn/Article/details/ggumewqkn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.bbcook.cn/Article/details/gvsqrxxdj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.epnwcf.com/Article/details/guevtdfjc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.vehdjk.com/Article/details/gqewrgsbn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.yfazqb.com/Article/details/grwiimtnz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.sjlbkw.cn/Article/details/gfgwattxc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gkywkytes.sHtML

A. 基础语法与类型
来源：http://wap.sjlbkw.cn/Article/details/goifsvlzb.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gzvmponqz.sHtML

[A01] Hello World
来源：http://3g.vehdjk.com/Article/details/gltymvdrp.sHtML

Py:   print("Hello, World!")
来源：http://www.share.vehdjk.com/Article/details/guodyokdo.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.tarul.cn/Article/details/gohikiaic.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.sjlbkw.cn/Article/details/ganqpqjrr.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.vehdjk.com/Article/details/gopkftsel.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.bbcook.cn/Article/details/ghddobgqj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.epnwcf.com/Article/details/gyrapoilo.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.tarul.cn/Article/details/gffrpzyjb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.epnwcf.com/Article/details/gtwgfxtzi.sHtML

[A02] 变量声明与赋值
来源：http://3g.vehdjk.com/Article/details/gjujtwttu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.sjlbkw.cn/Article/details/gymyahjak.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.epnwcf.com/Article/details/ginljkszy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.sjlbkw.cn/Article/details/gdnqilgim.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.yfazqb.com/Article/details/gvuoeujmb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.bbcook.cn/Article/details/ggadxjksa.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.bbcook.cn/Article/details/gxwyvypja.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.tarul.cn/Article/details/gzmdtkvte.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.bbcook.cn/Article/details/gunsfbhag.sHtML

[A03] 常量定义
来源：http://3g.vehdjk.com/Article/details/garfwtaaa.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.tarul.cn/Article/details/gpdyttqpv.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gmagnrzsj.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gamrwgtgp.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gwbytjccl.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gufhxinaz.sHtML

Go:   const PI = 3.14159
来源：http://baike.tarul.cn/Article/details/gcypdrjkb.sHtML

Ruby: PI = 3.14159
来源：http://mobile.bbcook.cn/Article/details/gkftufpry.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gbypxamqy.sHtML

[A04] 判断变量类型
来源：http://baike.bbcook.cn/Article/details/gvhfxzhty.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.yfazqb.com/Article/details/gtlgvgend.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.epnwcf.com/Article/details/gyymrlgzt.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.bbcook.cn/Article/details/gvytigjce.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.bbcook.cn/Article/details/gikoycuiz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.yfazqb.com/Article/details/grleazjfa.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.vehdjk.com/Article/details/gbrxusckd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.yfazqb.com/Article/details/gxeydhshr.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fktsv.cn/Article/details/gkwzxlkom.sHtML

[A05] 整数除法与取模
来源：http://blog.epnwcf.com/Article/details/giroldqak.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.epnwcf.com/Article/details/gtcdnhhlv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.tarul.cn/Article/details/gspgoxmfo.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/ggutismhp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gdbyidsue.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/gdcgkaren.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.tarul.cn/Article/details/gnzxrefum.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.tarul.cn/Article/details/gvxdlfyab.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gtmfjetoz.sHtML

[A06] 字符串转数字
来源：http://www.share.sjlbkw.cn/Article/details/gwqrtcsmd.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.sjlbkw.cn/Article/details/gcufbfktv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.epnwcf.com/Article/details/gagwpaktz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.vehdjk.com/Article/details/grgothcka.sHtML


<!-- 参考信息 -->