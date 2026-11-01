代发 wailian999

[U49] PHP：只读属性
来源：http://blog.yfazqb.com/Article/details/guyakcehx.sHtML

public readonly string $name
来源：http://m.share.bbcook.cn/Article/details/gtftuffez.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fktsv.cn/Article/details/grkecszdb.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.epnwcf.com/Article/details/gpqhxjxnc.sHtML

[U51] PHP：数组解构
来源：http://baike.tarul.cn/Article/details/geffbtjru.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.sjlbkw.cn/Article/details/grmcsyoax.sHtML

[U52] PHP：箭头函数
来源：http://3g.bbcook.cn/Article/details/ghvpmydtb.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.tarul.cn/Article/details/gdsqqvxbz.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fktsv.cn/Article/details/gmobaaurw.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fktsv.cn/Article/details/gfpsmjkuy.sHtML

[U54] PHP：空安全调用
来源：http://3g.bbcook.cn/Article/details/gpvjvocol.sHtML

$obj?->method()
来源：http://www.share.fktsv.cn/Article/details/gjfxpngag.sHtML

[U55] PHP：match 表达式
来源：http://read.share.epnwcf.com/Article/details/gqbvijhrf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.tarul.cn/Article/details/gjkocqfiv.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.vehdjk.com/Article/details/gqptodwfe.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/goinpjrgg.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gjocsfttn.sHtML

"值: {$a}"
来源：http://mobile.tarul.cn/Article/details/guwfijdmf.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.epnwcf.com/Article/details/gsaxjegta.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fktsv.cn/Article/details/gwhxwrfsh.sHtML

[U59] PHP：自定义排序
来源：http://wap.tarul.cn/Article/details/gppuflewm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.epnwcf.com/Article/details/gtorlzpyg.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.yfazqb.com/Article/details/gaitudmjt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.sjlbkw.cn/Article/details/gbqgisyfh.sHtML

[U61] PHP：正则
来源：http://www.blog.epnwcf.com/Article/details/giphczngs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.tarul.cn/Article/details/gbqfgduin.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.yfazqb.com/Article/details/gskfjfecv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.sjlbkw.cn/Article/details/geuumlsto.sHtML

[U63] PHP：文件读写
来源：http://blog.bbcook.cn/Article/details/gvilneryl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fktsv.cn/Article/details/gswmakpzr.sHtML

[U64] PHP：目录遍历
来源：http://3g.yfazqb.com/Article/details/gwcwsxasp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.tarul.cn/Article/details/gfnjgulnj.sHtML

[U65] PHP：会话
来源：http://www.blog.bbcook.cn/Article/details/gdosvidaf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.bbcook.cn/Article/details/gegjdvhin.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.epnwcf.com/Article/details/gdngzyunb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.epnwcf.com/Article/details/gmchjtldr.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.vehdjk.com/Article/details/gxguwkjrk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fktsv.cn/Article/details/gltwtosjh.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fktsv.cn/Article/details/gldampuaq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fktsv.cn/Article/details/ggierctjw.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.bbcook.cn/Article/details/gnmzvxbrt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.epnwcf.com/Article/details/gvxmffcag.sHtML

[U70] PHP：PDO 事务
来源：http://baike.epnwcf.com/Article/details/guljpsuzd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.yfazqb.com/Article/details/gjqjxqmlt.sHtML

[U71] PHP：抛出异常
来源：http://read.share.epnwcf.com/Article/details/guxehpxwb.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.bbcook.cn/Article/details/gntzomwcq.sHtML

[U72] PHP：写错误日志
来源：http://blog.yfazqb.com/Article/details/gldmsefqu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.vehdjk.com/Article/details/goiggstde.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.tarul.cn/Article/details/gpvhgrdht.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.yfazqb.com/Article/details/gunrhjiut.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fktsv.cn/Article/details/gkwpglsrt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.yfazqb.com/Article/details/gsrpufpgj.sHtML

[U75] PHP：依赖注入
来源：http://read.share.sjlbkw.cn/Article/details/gmljlgncw.sHtML

composer require psr/container
来源：http://3g.sjlbkw.cn/Article/details/gnxlacwxb.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.vehdjk.com/Article/details/gtpaqevqi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.yfazqb.com/Article/details/gnkntnuub.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fktsv.cn/Article/details/gbjkqwqek.sHtML

composer require twig/twig
来源：http://www.share.fktsv.cn/Article/details/gehaptsmd.sHtML

[U78] PHP：单元测试
来源：http://blog.yfazqb.com/Article/details/gkzmsvpji.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.vehdjk.com/Article/details/gceqmamli.sHtML

[U79] PHP：静态分析
来源：http://baike.tarul.cn/Article/details/gjuyshocm.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.epnwcf.com/Article/details/gmchwqmay.sHtML

[U80] PHP：代码规范修复
来源：http://blog.yfazqb.com/Article/details/gyfwuvxyz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.sjlbkw.cn/Article/details/gadvicnsc.sHtML

[U81] JS：初始化项目
来源：http://mobile.yfazqb.com/Article/details/ghdksdktv.sHtML

npm init -y;  npm i express
来源：http://wap.vehdjk.com/Article/details/gyntpghwj.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fktsv.cn/Article/details/gboqxphqo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.bbcook.cn/Article/details/gyzalgzqx.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.tarul.cn/Article/details/gtjyndwuk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.sjlbkw.cn/Article/details/gpqjwyycc.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.bbcook.cn/Article/details/gugemgpxb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.tarul.cn/Article/details/gdpfolxyf.sHtML

[U85] JS：可选链
来源：http://baike.epnwcf.com/Article/details/gquklvxgz.sHtML

a?.b?.c
来源：http://blog.fktsv.cn/Article/details/gwmttuvmh.sHtML

[U86] JS：空值合并
来源：http://wap.tarul.cn/Article/details/gzcxmjcac.sHtML

a ?? b
来源：http://m.share.tarul.cn/Article/details/gpquyfqhh.sHtML

[U87] JS：解构默认值
来源：http://read.share.vehdjk.com/Article/details/gmffbiqel.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.tarul.cn/Article/details/grxnawvev.sHtML

[U88] JS：对象展开合并
来源：http://3g.fktsv.cn/Article/details/ghuxympfg.sHtML

{ ...a, ...b }
来源：http://read.share.sjlbkw.cn/Article/details/gufxwuqct.sHtML

[U89] JS：数组去重
来源：http://blog.yfazqb.com/Article/details/gtitqrbfv.sHtML

[...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gwtgvnxkm.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.vehdjk.com/Article/details/grchjnxml.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/gvarekrot.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fktsv.cn/Article/details/gfdwklkqq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.tarul.cn/Article/details/glbujamyk.sHtML

[U92] JS：深拷贝
来源：http://baike.yfazqb.com/Article/details/gwzxepouu.sHtML

structuredClone(obj)
来源：http://read.share.yfazqb.com/Article/details/gkltvtare.sHtML

[U93] JS：模板字符串
来源：http://wap.yfazqb.com/Article/details/gbsxmdlbo.sHtML

`共 ${n} 条`
来源：http://m.share.tarul.cn/Article/details/grbubdbit.sHtML

[U94] JS：箭头函数
来源：http://read.share.yfazqb.com/Article/details/gynrotuss.sHtML

const double = x => x * 2;
来源：http://mobile.yfazqb.com/Article/details/gftrdzrmk.sHtML

[U95] JS：Promise 包装
来源：http://mobile.sjlbkw.cn/Article/details/ghskzwrcu.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fktsv.cn/Article/details/gxvqfscfa.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.yfazqb.com/Article/details/gpymvtspb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/gqavupjpj.sHtML

[U97] JS：并发请求
来源：http://www.blog.vehdjk.com/Article/details/gnvpeeigw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/grlbgiopz.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.bbcook.cn/Article/details/gxoovodph.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.bbcook.cn/Article/details/gbmuorbji.sHtML

[U99] JS：事件监听
来源：http://wap.fktsv.cn/Article/details/gkpehibyu.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.yfazqb.com/Article/details/gycqclmod.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.yfazqb.com/Article/details/gabsgteqy.sHtML

document.querySelector(".item")
来源：http://www.blog.vehdjk.com/Article/details/grtsgdxkz.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fktsv.cn/Article/details/gynikinxy.sHtML

el.classList.toggle("active")
来源：http://wap.vehdjk.com/Article/details/gczrzohvl.sHtML

[U102] JS：本地存储
来源：http://blog.fktsv.cn/Article/details/gerfhmdeg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fktsv.cn/Article/details/gucpkoeuy.sHtML

[U103] JS：定时器
来源：http://www.share.vehdjk.com/Article/details/gmarxthoq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.vehdjk.com/Article/details/gvsorzizv.sHtML

[U104] JS：防抖
来源：http://baike.vehdjk.com/Article/details/gopbbxcow.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/gojhditxt.sHtML

[U105] JS：节流
来源：http://blog.sjlbkw.cn/Article/details/gqnrsogjq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.vehdjk.com/Article/details/geankjtsk.sHtML

[U106] JS：日期格式化
来源：http://read.share.bbcook.cn/Article/details/gwtuahqri.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fktsv.cn/Article/details/gnmctstxi.sHtML

[U107] JS：数字千分位
来源：http://wap.epnwcf.com/Article/details/gqddpjlep.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.tarul.cn/Article/details/gdmundqyu.sHtML

[U108] JS：随机整数
来源：http://blog.epnwcf.com/Article/details/gpshsfeud.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.tarul.cn/Article/details/ghqhirwzb.sHtML

[U109] JS：数组分组
来源：http://m.share.sjlbkw.cn/Article/details/gcuaidoph.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.tarul.cn/Article/details/goidanzkv.sHtML

[U110] JS：数组分块
来源：http://www.blog.bbcook.cn/Article/details/gmcvkodez.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fktsv.cn/Article/details/gcbcwbrgh.sHtML

[U111] JS：对象转 Map
来源：http://www.share.sjlbkw.cn/Article/details/gryeeqtii.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.epnwcf.com/Article/details/gwpfhybgu.sHtML

[U112] JS：字符串补位
来源：http://blog.epnwcf.com/Article/details/gzouvppyn.sHtML

"7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gqeclgxrq.sHtML

[U113] JS：正则替换全部
来源：http://mobile.epnwcf.com/Article/details/gsukvgxzq.sHtML

s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gftgpoloq.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.tarul.cn/Article/details/gqwrttoyv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.tarul.cn/Article/details/gklmaerww.sHtML

[U115] JS：生成 UUID
来源：http://wap.tarul.cn/Article/details/gbcpaqewe.sHtML

crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/gqblpbqrz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.bbcook.cn/Article/details/gghzlkqnr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.yfazqb.com/Article/details/gyrfzsahn.sHtML

[U117] JS：单元测试
来源：http://baike.epnwcf.com/Article/details/gvvzkvljx.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.bbcook.cn/Article/details/gwhqutjcw.sHtML

[U118] JS：开发服务器
来源：http://read.share.fktsv.cn/Article/details/guitfiivv.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.yfazqb.com/Article/details/gfpjsnckw.sHtML

[U119] JS：生产构建
来源：http://blog.fktsv.cn/Article/details/gnqbjnfqr.sHtML

npx vite build
来源：http://read.share.vehdjk.com/Article/details/ghqldzsjh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.epnwcf.com/Article/details/gcxqnausm.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.sjlbkw.cn/Article/details/gumkwdofs.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gpjtnqkwm.sHtML

统计汇总
来源：http://baike.epnwcf.com/Article/details/gdmsgvzib.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gxfjltofb.sHtML

按语言统计（条）：
来源：http://read.share.epnwcf.com/Article/details/gxlyjakmn.sHtML

Python ......... 252
来源：http://www.share.tarul.cn/Article/details/ggdcujsxr.sHtML

PHP ............ 252
来源：http://www.blog.tarul.cn/Article/details/gwxgplstx.sHtML

JavaScript ..... 252
来源：http://blog.sjlbkw.cn/Article/details/grbksgjta.sHtML

TypeScript ..... 212
来源：http://read.share.yfazqb.com/Article/details/grrerrtya.sHtML

Java ........... 212
来源：http://m.share.epnwcf.com/Article/details/gwnttkiib.sHtML

Go ............. 212
来源：http://blog.tarul.cn/Article/details/gmwerxsag.sHtML

Ruby ........... 212
来源：http://3g.fktsv.cn/Article/details/gtwkjeauo.sHtML

C# ............. 212
来源：http://wap.bbcook.cn/Article/details/gztuwndsi.sHtML

C .............. 30
来源：http://m.share.bbcook.cn/Article/details/giezeepiy.sHtML

C++ ............ 30
来源：http://blog.epnwcf.com/Article/details/ghaahexlo.sHtML

SQL ............ 90
来源：http://www.blog.epnwcf.com/Article/details/gussovrcn.sHtML

Bash ........... 80
来源：http://read.share.bbcook.cn/Article/details/gynevkwjo.sHtML

Kotlin ......... 15
来源：http://read.share.fktsv.cn/Article/details/gwzxqvhzq.sHtML

Swift .......... 15
来源：http://www.m.share.vehdjk.com/Article/details/gcpwvzpiw.sHtML

Lua ............ 10
来源：http://wap.tarul.cn/Article/details/gisrwwkgm.sHtML

Perl ........... 10
来源：http://www.m.share.epnwcf.com/Article/details/gbbhtmhjx.sHtML

Scala .......... 10
来源：http://baike.tarul.cn/Article/details/gbhskkinq.sHtML

------------------------------------
来源：http://www.blog.tarul.cn/Article/details/gdbipilze.sHtML

合计 ........... 2106 条
来源：http://baike.yfazqb.com/Article/details/guklzdsvu.sHtML

按章节统计：
来源：http://www.share.tarul.cn/Article/details/ggdiarkbp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fktsv.cn/Article/details/gvrekvobz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.epnwcf.com/Article/details/gleoeceml.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/gvkjnbedq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fktsv.cn/Article/details/gqpvxzlql.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.sjlbkw.cn/Article/details/gwmpogkhj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.epnwcf.com/Article/details/gsrsfdoci.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.epnwcf.com/Article/details/gxnvqpjtf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.vehdjk.com/Article/details/gzwepejoe.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/glakzcyts.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.sjlbkw.cn/Article/details/gjtfvnkjq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gexzsdyba.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/ggothfkyv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gyplsinwn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.tarul.cn/Article/details/gzghwypih.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.tarul.cn/Article/details/gnrmjjruh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/glwkqsimc.sHtML

Q SQL 专题                              90
来源：http://mobile.fktsv.cn/Article/details/gxdwkbsgo.sHtML

R Bash 专题                             80
来源：http://www.share.bbcook.cn/Article/details/gvzqixpdz.sHtML

S C / C++ 专题                          60
来源：http://baike.tarul.cn/Article/details/gpblulhws.sHtML

T 其他语言补充                          60
来源：http://3g.fktsv.cn/Article/details/gbujurivk.sHtML

U 高频实用片段                         120
来源：http://baike.fktsv.cn/Article/details/gclnaxytd.sHtML

------------------------------------
来源：http://3g.yfazqb.com/Article/details/gaiobwcdr.sHtML

合计                                  2106 条
来源：http://3g.yfazqb.com/Article/details/ganrmzipz.sHtML

--------------------------------------------------------------------------------
来源：http://3g.epnwcf.com/Article/details/gifjhuhue.sHtML

使用提醒
来源：http://www.m.share.yfazqb.com/Article/details/gbauqbnqf.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gwbilqrtb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.vehdjk.com/Article/details/gxdsnqjui.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.bbcook.cn/Article/details/ggvbwxfyb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.vehdjk.com/Article/details/gtjnzzlvn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.vehdjk.com/Article/details/gysapdsuo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.sjlbkw.cn/Article/details/gddfbmwof.sHtML

—— 文件结束 ——
来源：http://3g.sjlbkw.cn/Article/details/gozkkcmnv.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gnsefisfe.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.epnwcf.com/Article/details/gkmjiymri.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.tarul.cn/Article/details/gyyqgvuhd.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gaysyjzzh.sHtML

【收录内容】
来源：http://blog.sjlbkw.cn/Article/details/gdrujfeyi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.bbcook.cn/Article/details/gktnjticn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.epnwcf.com/Article/details/gqqqbqptn.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsvkudsb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.vehdjk.com/Article/details/gqurkowdb.sHtML

【使用说明】
来源：http://blog.bbcook.cn/Article/details/gkbfgntui.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.tarul.cn/Article/details/gvhfoholk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.vehdjk.com/Article/details/grbutjyzn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fktsv.cn/Article/details/gcxhsmyas.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.vehdjk.com/Article/details/ghdiqsxyv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.bbcook.cn/Article/details/gvwcyuafw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.vehdjk.com/Article/details/gsretfuch.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.sjlbkw.cn/Article/details/gnbaqhumv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fktsv.cn/Article/details/gefckquzl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.bbcook.cn/Article/details/gxzrshfpf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.tarul.cn/Article/details/gumlggjku.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fktsv.cn/Article/details/gvfgqqioa.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.tarul.cn/Article/details/ghfrdkjsf.sHtML

【文件统计】
来源：http://www.m.share.bbcook.cn/Article/details/gesectnir.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.bbcook.cn/Article/details/gowfptokw.sHtML

--------------------------------------------------------------------------------
来源：http://blog.yfazqb.com/Article/details/gcrmgirmg.sHtML

目  录
来源：http://wap.yfazqb.com/Article/details/gtcxhaopy.sHtML

--------------------------------------------------------------------------------
来源：http://3g.vehdjk.com/Article/details/gnjkgzmbi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.bbcook.cn/Article/details/gaydntkeq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.vehdjk.com/Article/details/gnhcwkauu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.yfazqb.com/Article/details/gjrosuaoz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.yfazqb.com/Article/details/ghonrehnp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.tarul.cn/Article/details/gyrbjxmej.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.epnwcf.com/Article/details/gkwkppqam.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.vehdjk.com/Article/details/gitbdkqdj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fktsv.cn/Article/details/gavqimxzd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/gyjqsqbrs.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.bbcook.cn/Article/details/gaaygyglv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gpkvrwmxw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/gzqinnrko.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.vehdjk.com/Article/details/gcmfvgdtf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.bbcook.cn/Article/details/gltvzjuiy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.tarul.cn/Article/details/guceifigw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.bbcook.cn/Article/details/gdsciuzjh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.epnwcf.com/Article/details/gymyrjzhs.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.epnwcf.com/Article/details/gmurfffkh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fktsv.cn/Article/details/gzuokwcvy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.sjlbkw.cn/Article/details/gtygwhger.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.vehdjk.com/Article/details/gnfhahbuw.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gprdxuqfd.sHtML

A. 基础语法与类型
来源：http://www.blog.vehdjk.com/Article/details/ggustxghi.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gtbqzloji.sHtML

[A01] Hello World
来源：http://read.share.tarul.cn/Article/details/gdfqolrlo.sHtML

Py:   print("Hello, World!")
来源：http://blog.yfazqb.com/Article/details/goeccmwxm.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.sjlbkw.cn/Article/details/gvdvxydga.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.yfazqb.com/Article/details/gvbskoqks.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.bbcook.cn/Article/details/gpcclriwo.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.yfazqb.com/Article/details/gnhbjcerv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.sjlbkw.cn/Article/details/ggjbogjjh.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fktsv.cn/Article/details/gclwdkvyx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.tarul.cn/Article/details/gwolsqtzt.sHtML

[A02] 变量声明与赋值
来源：http://baike.sjlbkw.cn/Article/details/gyrkmnsdl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.tarul.cn/Article/details/getpgmqlx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fktsv.cn/Article/details/gcpfyhmwq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.vehdjk.com/Article/details/ghfdobwss.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.tarul.cn/Article/details/gmbbeitsh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.sjlbkw.cn/Article/details/gyndedfvw.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.epnwcf.com/Article/details/gsnyjfsfq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.sjlbkw.cn/Article/details/gmfsrvkgx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.yfazqb.com/Article/details/gyktqbpdo.sHtML

[A03] 常量定义
来源：http://www.blog.sjlbkw.cn/Article/details/gjrybkfnh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.yfazqb.com/Article/details/gdlllomoh.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/getvsrnvt.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/glpticaux.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gwmfeigpn.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/grbbxltrs.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fktsv.cn/Article/details/gfxaeacam.sHtML

Ruby: PI = 3.14159
来源：http://mobile.bbcook.cn/Article/details/gxgmmjjua.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/ggnpzlzoc.sHtML

[A04] 判断变量类型
来源：http://3g.sjlbkw.cn/Article/details/gqahgvuso.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.bbcook.cn/Article/details/gowtzrtdi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.yfazqb.com/Article/details/gobupumwa.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.sjlbkw.cn/Article/details/gxurliyyh.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fktsv.cn/Article/details/gexxlapmv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fktsv.cn/Article/details/gpyxqluee.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.bbcook.cn/Article/details/gqwbyaxcz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fktsv.cn/Article/details/gtcbubxik.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.sjlbkw.cn/Article/details/glnktycpr.sHtML

[A05] 整数除法与取模
来源：http://m.share.yfazqb.com/Article/details/gfblnbljj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.tarul.cn/Article/details/gptfyncdg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.epnwcf.com/Article/details/gxrxxrsbb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/ggfkjduxl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.yfazqb.com/Article/details/gjkodybrg.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gastgjysj.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.epnwcf.com/Article/details/glyftlmbm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.tarul.cn/Article/details/grbjayzez.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.tarul.cn/Article/details/gpnagecna.sHtML

[A06] 字符串转数字
来源：http://www.m.share.tarul.cn/Article/details/guiwkwyoh.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.tarul.cn/Article/details/gybvjzuzu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.yfazqb.com/Article/details/gknhnhvkl.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.epnwcf.com/Article/details/gjmfpsiac.sHtML


<!-- 参考信息 -->