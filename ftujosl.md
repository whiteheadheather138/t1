代发 wailian999

[U49] PHP：只读属性
来源：http://3g.fktsv.cn/Article/details/gniyananc.sHtML

public readonly string $name
来源：http://m.share.tarul.cn/Article/details/gmghklqax.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.epnwcf.com/Article/details/gjkrlurya.sHtML

public function __construct(private int $id) {}
来源：http://read.share.tarul.cn/Article/details/grojcwrul.sHtML

[U51] PHP：数组解构
来源：http://baike.vehdjk.com/Article/details/ghelvhobz.sHtML

[$a, $b] = $arr;
来源：http://www.blog.epnwcf.com/Article/details/glyakqgwc.sHtML

[U52] PHP：箭头函数
来源：http://read.share.yfazqb.com/Article/details/gjcoaiyzd.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.tarul.cn/Article/details/gtidecqis.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.bbcook.cn/Article/details/gaqnmdihm.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrbozhaj.sHtML

[U54] PHP：空安全调用
来源：http://baike.epnwcf.com/Article/details/gpzgzuadz.sHtML

$obj?->method()
来源：http://www.m.share.epnwcf.com/Article/details/gjmvyahuw.sHtML

[U55] PHP：match 表达式
来源：http://mobile.vehdjk.com/Article/details/gmsaqhxcq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.epnwcf.com/Article/details/gdacpjuub.sHtML

[U56] PHP：命名参数
来源：http://mobile.bbcook.cn/Article/details/gtywjxocu.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/glaxbonji.sHtML

[U57] PHP：字符串插值
来源：http://wap.epnwcf.com/Article/details/gyrvcioxd.sHtML

"值: {$a}"
来源：http://3g.yfazqb.com/Article/details/gkhfuzrdw.sHtML

[U58] PHP：数组三件套
来源：http://baike.bbcook.cn/Article/details/geefsciyu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.epnwcf.com/Article/details/gfkgvyjpe.sHtML

[U59] PHP：自定义排序
来源：http://www.share.yfazqb.com/Article/details/gidupgeho.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.tarul.cn/Article/details/gxvtxglbe.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.epnwcf.com/Article/details/goeqihfok.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.vehdjk.com/Article/details/gylhcxzrf.sHtML

[U61] PHP：正则
来源：http://www.blog.sjlbkw.cn/Article/details/gcyrzxtug.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/gyjdtexle.sHtML

[U62] PHP：日期对象
来源：http://wap.fktsv.cn/Article/details/gjemerkow.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.sjlbkw.cn/Article/details/gkywijmlr.sHtML

[U63] PHP：文件读写
来源：http://www.blog.vehdjk.com/Article/details/gsdjwkxfd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.tarul.cn/Article/details/gqutismiq.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fktsv.cn/Article/details/gzdlobdfa.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.vehdjk.com/Article/details/gozjiyqhw.sHtML

[U65] PHP：会话
来源：http://www.share.tarul.cn/Article/details/getygadjs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.yfazqb.com/Article/details/giyrfrtpc.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.sjlbkw.cn/Article/details/grlidjlqb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.bbcook.cn/Article/details/gxgxbxpyg.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.bbcook.cn/Article/details/gpnsxmtni.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.tarul.cn/Article/details/giwxfnoac.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.epnwcf.com/Article/details/gtxflrnle.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.sjlbkw.cn/Article/details/gekqpqhqz.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.sjlbkw.cn/Article/details/gnmtlkjpo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.bbcook.cn/Article/details/gefnokgsk.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fktsv.cn/Article/details/gnokuqeqm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.tarul.cn/Article/details/giqkxicdq.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fktsv.cn/Article/details/gzriqhmyb.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.yfazqb.com/Article/details/gsbgqayzp.sHtML

[U72] PHP：写错误日志
来源：http://wap.epnwcf.com/Article/details/gkosognny.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.vehdjk.com/Article/details/gmvqsxasw.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.sjlbkw.cn/Article/details/gphvgmpoj.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.yfazqb.com/Article/details/gtlxmtdgj.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.bbcook.cn/Article/details/gyupnzfhb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.yfazqb.com/Article/details/gsffvupox.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fktsv.cn/Article/details/guaieqsxr.sHtML

composer require psr/container
来源：http://3g.tarul.cn/Article/details/gevwwfwun.sHtML

[U76] PHP：简单路由
来源：http://www.share.vehdjk.com/Article/details/gfjrkmskj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.tarul.cn/Article/details/gezfgsuzg.sHtML

[U77] PHP：模板渲染
来源：http://read.share.sjlbkw.cn/Article/details/gszpoqjgy.sHtML

composer require twig/twig
来源：http://www.blog.sjlbkw.cn/Article/details/gvjiysqbx.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fktsv.cn/Article/details/gvyxpdfbb.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.vehdjk.com/Article/details/gvnoxomfo.sHtML

[U79] PHP：静态分析
来源：http://read.share.epnwcf.com/Article/details/gakftaqew.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.yfazqb.com/Article/details/gmtjjffhd.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fktsv.cn/Article/details/gjxtfcdhp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.yfazqb.com/Article/details/gtmuhampd.sHtML

[U81] JS：初始化项目
来源：http://read.share.tarul.cn/Article/details/gulelpaur.sHtML

npm init -y;  npm i express
来源：http://www.m.share.vehdjk.com/Article/details/gtuwgpqmx.sHtML

[U82] JS：package.json 脚本
来源：http://wap.bbcook.cn/Article/details/gdzapxfzr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.vehdjk.com/Article/details/gnftrfxxv.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fktsv.cn/Article/details/gvyvsscme.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.vehdjk.com/Article/details/gfzfibhrq.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.bbcook.cn/Article/details/gtpsqzvvi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.yfazqb.com/Article/details/gqwhoyrdm.sHtML

[U85] JS：可选链
来源：http://www.m.share.epnwcf.com/Article/details/ganyslope.sHtML

a?.b?.c
来源：http://blog.epnwcf.com/Article/details/gyjbhtpph.sHtML

[U86] JS：空值合并
来源：http://mobile.tarul.cn/Article/details/gkbptcxsa.sHtML

a ?? b
来源：http://www.blog.vehdjk.com/Article/details/gtivyfwiq.sHtML

[U87] JS：解构默认值
来源：http://www.share.tarul.cn/Article/details/gwtwbufzq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fktsv.cn/Article/details/gccnilkxf.sHtML

[U88] JS：对象展开合并
来源：http://blog.bbcook.cn/Article/details/gjkaqibxe.sHtML

{ ...a, ...b }
来源：http://wap.fktsv.cn/Article/details/gjiwmhmmx.sHtML

[U89] JS：数组去重
来源：http://baike.fktsv.cn/Article/details/gqmfaiwsb.sHtML

[...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhpuqapj.sHtML

[U90] JS：数字数组排序
来源：http://baike.fktsv.cn/Article/details/gtdtmjgdh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gintmgadu.sHtML

[U91] JS：对象键值遍历
来源：http://wap.tarul.cn/Article/details/gqnlulkoi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.epnwcf.com/Article/details/gjvucwdou.sHtML

[U92] JS：深拷贝
来源：http://www.blog.epnwcf.com/Article/details/gcyycmezc.sHtML

structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gduxttbem.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/grfwxqrrs.sHtML

`共 ${n} 条`
来源：http://3g.fktsv.cn/Article/details/ghbumsizm.sHtML

[U94] JS：箭头函数
来源：http://baike.sjlbkw.cn/Article/details/gnuwjogev.sHtML

const double = x => x * 2;
来源：http://wap.bbcook.cn/Article/details/gpoxiqici.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.bbcook.cn/Article/details/gohxpfjtj.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fktsv.cn/Article/details/gyhzrpvnc.sHtML

[U96] JS：async/await 与异常
来源：http://blog.sjlbkw.cn/Article/details/goyoynwnw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/goetasmgt.sHtML

[U97] JS：并发请求
来源：http://baike.fktsv.cn/Article/details/ghynmncwn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.vehdjk.com/Article/details/gkpwjjbcj.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.yfazqb.com/Article/details/gpprewuyp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.epnwcf.com/Article/details/gtailplev.sHtML

[U99] JS：事件监听
来源：http://mobile.yfazqb.com/Article/details/guciixxqv.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.sjlbkw.cn/Article/details/gkgpmleac.sHtML

[U100] JS：DOM 查询
来源：http://baike.yfazqb.com/Article/details/gkrpbcmcx.sHtML

document.querySelector(".item")
来源：http://baike.epnwcf.com/Article/details/gjxlixilt.sHtML

[U101] JS：classList 操作
来源：http://3g.yfazqb.com/Article/details/gjvxlnjle.sHtML

el.classList.toggle("active")
来源：http://3g.yfazqb.com/Article/details/gixcxefmr.sHtML

[U102] JS：本地存储
来源：http://mobile.epnwcf.com/Article/details/gggkonuef.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.sjlbkw.cn/Article/details/gxpqjbsib.sHtML

[U103] JS：定时器
来源：http://www.m.share.vehdjk.com/Article/details/gkvoxthhd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.tarul.cn/Article/details/gcpzdlxkg.sHtML

[U104] JS：防抖
来源：http://blog.fktsv.cn/Article/details/gqwskdjbb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/giccjexrg.sHtML

[U105] JS：节流
来源：http://www.share.fktsv.cn/Article/details/govxhsjcl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.tarul.cn/Article/details/gjtddbkvq.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.epnwcf.com/Article/details/gbqdiuvym.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.epnwcf.com/Article/details/gojjrqrdu.sHtML

[U107] JS：数字千分位
来源：http://blog.fktsv.cn/Article/details/gwpfbwguo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.epnwcf.com/Article/details/gghlmhswo.sHtML

[U108] JS：随机整数
来源：http://www.blog.vehdjk.com/Article/details/gqhvnyvuw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fktsv.cn/Article/details/gmbqkgdep.sHtML

[U109] JS：数组分组
来源：http://wap.epnwcf.com/Article/details/gqhxbizjb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.tarul.cn/Article/details/gdvsforhk.sHtML

[U110] JS：数组分块
来源：http://blog.epnwcf.com/Article/details/glhadmyne.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.vehdjk.com/Article/details/gguuyfftt.sHtML

[U111] JS：对象转 Map
来源：http://baike.yfazqb.com/Article/details/gkkzdubss.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.vehdjk.com/Article/details/gevsgxqui.sHtML

[U112] JS：字符串补位
来源：http://www.share.fktsv.cn/Article/details/gcuigqsjx.sHtML

"7".padStart(3, "0")
来源：http://wap.epnwcf.com/Article/details/geypssjew.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.yfazqb.com/Article/details/grishpjpp.sHtML

s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/gcvsoemkh.sHtML

[U114] JS：JSON 深比较
来源：http://blog.sjlbkw.cn/Article/details/gewxmrmeh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/gfwvjdrnc.sHtML

[U115] JS：生成 UUID
来源：http://www.share.bbcook.cn/Article/details/ggywqudeh.sHtML

crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/ggpngnjyj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fktsv.cn/Article/details/gntledosd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.tarul.cn/Article/details/gvjdigtsc.sHtML

[U117] JS：单元测试
来源：http://baike.tarul.cn/Article/details/gcfjqjvmp.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.tarul.cn/Article/details/gycgoguhq.sHtML

[U118] JS：开发服务器
来源：http://read.share.epnwcf.com/Article/details/gyvyqxbsu.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.yfazqb.com/Article/details/gksfkffnq.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fktsv.cn/Article/details/gwwbneqay.sHtML

npx vite build
来源：http://blog.tarul.cn/Article/details/gxuixdzkg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.sjlbkw.cn/Article/details/geggbjlrq.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.vehdjk.com/Article/details/gwwxgndid.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gfthztfmo.sHtML

统计汇总
来源：http://3g.yfazqb.com/Article/details/gmuualnxv.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gjwrvhmuf.sHtML

按语言统计（条）：
来源：http://www.blog.epnwcf.com/Article/details/gjbjnuyeo.sHtML

Python ......... 252
来源：http://3g.vehdjk.com/Article/details/ghtrfrmxw.sHtML

PHP ............ 252
来源：http://www.blog.tarul.cn/Article/details/gnnepjvqn.sHtML

JavaScript ..... 252
来源：http://3g.bbcook.cn/Article/details/gpwlvjdou.sHtML

TypeScript ..... 212
来源：http://3g.vehdjk.com/Article/details/gpxpieojk.sHtML

Java ........... 212
来源：http://www.blog.bbcook.cn/Article/details/gndicpmzm.sHtML

Go ............. 212
来源：http://www.share.fktsv.cn/Article/details/gomkwewvb.sHtML

Ruby ........... 212
来源：http://www.blog.tarul.cn/Article/details/guhyfipoe.sHtML

C# ............. 212
来源：http://wap.sjlbkw.cn/Article/details/gxhykvcxc.sHtML

C .............. 30
来源：http://mobile.tarul.cn/Article/details/ghgkhrxwb.sHtML

C++ ............ 30
来源：http://wap.vehdjk.com/Article/details/gufrdgvpn.sHtML

SQL ............ 90
来源：http://wap.tarul.cn/Article/details/gznolnqfn.sHtML

Bash ........... 80
来源：http://blog.tarul.cn/Article/details/gzlqdcnwc.sHtML

Kotlin ......... 15
来源：http://mobile.yfazqb.com/Article/details/gaktphvzz.sHtML

Swift .......... 15
来源：http://mobile.fktsv.cn/Article/details/gaazwpuqv.sHtML

Lua ............ 10
来源：http://blog.sjlbkw.cn/Article/details/gdnndvdsn.sHtML

Perl ........... 10
来源：http://baike.sjlbkw.cn/Article/details/gdzswuzem.sHtML

Scala .......... 10
来源：http://www.share.bbcook.cn/Article/details/glsmwyojo.sHtML

------------------------------------
来源：http://mobile.epnwcf.com/Article/details/gyshydfgx.sHtML

合计 ........... 2106 条
来源：http://read.share.yfazqb.com/Article/details/gcvldrsxh.sHtML

按章节统计：
来源：http://read.share.fktsv.cn/Article/details/gunwnpabp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.sjlbkw.cn/Article/details/glphnjaat.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.vehdjk.com/Article/details/ghwlgsvjz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.sjlbkw.cn/Article/details/gefdcawzn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.epnwcf.com/Article/details/gjrignwiy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.epnwcf.com/Article/details/gmjvttuyi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.epnwcf.com/Article/details/gsgcsicwk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fktsv.cn/Article/details/gzfttqoyk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fktsv.cn/Article/details/ghukquoej.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/gwqhgzpqw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fktsv.cn/Article/details/gqhxacnbx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.sjlbkw.cn/Article/details/goqxluchw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/gyxpfqvjn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gzwqtnocc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fktsv.cn/Article/details/gjlmjezdt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.tarul.cn/Article/details/gvwhfxpwc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gaxnrlgpw.sHtML

Q SQL 专题                              90
来源：http://www.share.bbcook.cn/Article/details/gussijhvp.sHtML

R Bash 专题                             80
来源：http://wap.fktsv.cn/Article/details/gajwkugsx.sHtML

S C / C++ 专题                          60
来源：http://wap.vehdjk.com/Article/details/gagfykgdr.sHtML

T 其他语言补充                          60
来源：http://3g.fktsv.cn/Article/details/gcabcdpxx.sHtML

U 高频实用片段                         120
来源：http://baike.fktsv.cn/Article/details/gezetzogi.sHtML

------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/gatyiawjw.sHtML

合计                                  2106 条
来源：http://m.share.tarul.cn/Article/details/grhouelxv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fktsv.cn/Article/details/geulxfoig.sHtML

使用提醒
来源：http://m.share.fktsv.cn/Article/details/glosmhhfg.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.tarul.cn/Article/details/gtxudyefx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.sjlbkw.cn/Article/details/gvbzrjjje.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.sjlbkw.cn/Article/details/gbmxlgujj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.epnwcf.com/Article/details/gbwmiqsca.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.sjlbkw.cn/Article/details/gliitvjrp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.epnwcf.com/Article/details/gqksddbdo.sHtML

—— 文件结束 ——
来源：http://blog.yfazqb.com/Article/details/ghposmhjz.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gnykoboza.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.bbcook.cn/Article/details/gllpeuvvz.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.bbcook.cn/Article/details/gnufaijhm.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gqhgtovwp.sHtML

【收录内容】
来源：http://wap.sjlbkw.cn/Article/details/gagnuivee.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.bbcook.cn/Article/details/glwxikvaz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fktsv.cn/Article/details/gwotpzpvs.sHtML

SQL · Bash · C · C++
来源：http://wap.tarul.cn/Article/details/gbkkugpkl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fktsv.cn/Article/details/gdlyfxtus.sHtML

【使用说明】
来源：http://mobile.epnwcf.com/Article/details/gnjezmgwz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.yfazqb.com/Article/details/gectsgylp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.tarul.cn/Article/details/gdouxleuw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.sjlbkw.cn/Article/details/gvetzefcw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.vehdjk.com/Article/details/gggiruwbb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fktsv.cn/Article/details/gdaoxaszt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fktsv.cn/Article/details/gadzyttaz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.bbcook.cn/Article/details/ghihwskaf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.vehdjk.com/Article/details/gklaylaza.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.tarul.cn/Article/details/gkjwbgfok.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fktsv.cn/Article/details/gxnacyqly.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.vehdjk.com/Article/details/gndbdlhjy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.epnwcf.com/Article/details/ghccaukvr.sHtML

【文件统计】
来源：http://m.share.bbcook.cn/Article/details/gdzbsuzfx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.tarul.cn/Article/details/gsegdzyqh.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fktsv.cn/Article/details/guyskated.sHtML

目  录
来源：http://www.share.fktsv.cn/Article/details/gkduhngfy.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gblkjbnws.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.sjlbkw.cn/Article/details/gmmcvtkpg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.sjlbkw.cn/Article/details/gxsiefhew.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.tarul.cn/Article/details/gmkxwtymr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.sjlbkw.cn/Article/details/gjrmkaptk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.tarul.cn/Article/details/gxojjsctg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.yfazqb.com/Article/details/gsifjyxyy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/gemwrddyf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.yfazqb.com/Article/details/gejdpjsgc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.bbcook.cn/Article/details/glmxjhpam.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.sjlbkw.cn/Article/details/gqfcrenwq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/gybctclyf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.vehdjk.com/Article/details/gmwxypihw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fktsv.cn/Article/details/grhrygrtn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.vehdjk.com/Article/details/grkjnhmob.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.bbcook.cn/Article/details/gxacwkwoy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/gusahsysl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.epnwcf.com/Article/details/gdvspzref.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fktsv.cn/Article/details/gxvzfamur.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.yfazqb.com/Article/details/geomrysra.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.sjlbkw.cn/Article/details/gawixjkwj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.sjlbkw.cn/Article/details/ghjpammmi.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gshkknbxt.sHtML

A. 基础语法与类型
来源：http://blog.yfazqb.com/Article/details/gowqjippu.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gwxqcpfsj.sHtML

[A01] Hello World
来源：http://wap.yfazqb.com/Article/details/gbtrxdxuq.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.epnwcf.com/Article/details/gryhufcge.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.tarul.cn/Article/details/gzcsvlsyp.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fktsv.cn/Article/details/gewyaqjzf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.epnwcf.com/Article/details/gmcsponul.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fktsv.cn/Article/details/gzvjkoxcb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.vehdjk.com/Article/details/gnscqdlez.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.yfazqb.com/Article/details/gdlboyyif.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.sjlbkw.cn/Article/details/gxodvfszc.sHtML

[A02] 变量声明与赋值
来源：http://mobile.sjlbkw.cn/Article/details/gmobvqbyw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.sjlbkw.cn/Article/details/guxfyajwb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.vehdjk.com/Article/details/gmuohmdjf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.sjlbkw.cn/Article/details/gsrstlqgi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.yfazqb.com/Article/details/gtikmlipu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.tarul.cn/Article/details/ggexomnog.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fktsv.cn/Article/details/gvqkqjfii.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fktsv.cn/Article/details/gzqmkxulx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.yfazqb.com/Article/details/gcglibczn.sHtML

[A03] 常量定义
来源：http://www.m.share.yfazqb.com/Article/details/gsdezzghh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.sjlbkw.cn/Article/details/gawvmdauo.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gkwbxztlk.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gdmqqlcsn.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gtlczfsge.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gslinliqb.sHtML

Go:   const PI = 3.14159
来源：http://read.share.epnwcf.com/Article/details/gxhifdkyt.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.vehdjk.com/Article/details/grzhtncvg.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gpdtvzfab.sHtML

[A04] 判断变量类型
来源：http://www.share.bbcook.cn/Article/details/gmrbzqene.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fktsv.cn/Article/details/gtudckuiv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.yfazqb.com/Article/details/ggzbenyyi.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.tarul.cn/Article/details/gamtbootc.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.tarul.cn/Article/details/guoaucuzy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.yfazqb.com/Article/details/gglqortvy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.yfazqb.com/Article/details/gdbsqvkvs.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.tarul.cn/Article/details/gyzlalutm.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.sjlbkw.cn/Article/details/gfuqrupwb.sHtML

[A05] 整数除法与取模
来源：http://read.share.sjlbkw.cn/Article/details/gulabfxse.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.epnwcf.com/Article/details/guscvtbqm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.bbcook.cn/Article/details/ggbhxnbak.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gaaevflvz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/gbvplagmp.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.vehdjk.com/Article/details/gqolrskke.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fktsv.cn/Article/details/gkxhspzvi.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.tarul.cn/Article/details/genaijfzg.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.tarul.cn/Article/details/gpxknvrqy.sHtML

[A06] 字符串转数字
来源：http://www.share.yfazqb.com/Article/details/gyvkshnxt.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.tarul.cn/Article/details/gofcjmdtn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.sjlbkw.cn/Article/details/grkgsiqgz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.vehdjk.com/Article/details/gtvuplfzn.sHtML


<!-- 参考信息 -->