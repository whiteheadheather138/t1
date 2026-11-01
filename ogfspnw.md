代发 wailian999

[U49] PHP：只读属性
来源：http://blog.epnwcf.com/Article/details/gkdjhbyod.sHtML

public readonly string $name
来源：http://wap.vehdjk.com/Article/details/gssgzxdab.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fktsv.cn/Article/details/gddqoeopq.sHtML

public function __construct(private int $id) {}
来源：http://www.share.bbcook.cn/Article/details/gftghvadp.sHtML

[U51] PHP：数组解构
来源：http://mobile.yfazqb.com/Article/details/gepcvvplf.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.vehdjk.com/Article/details/gbnwhkqee.sHtML

[U52] PHP：箭头函数
来源：http://m.share.tarul.cn/Article/details/gbglhbaxf.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fktsv.cn/Article/details/gwkchayiv.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.epnwcf.com/Article/details/gipzdeyrm.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.tarul.cn/Article/details/ggynxxrdm.sHtML

[U54] PHP：空安全调用
来源：http://mobile.tarul.cn/Article/details/gnjtfzqyc.sHtML

$obj?->method()
来源：http://www.m.share.epnwcf.com/Article/details/gdkvohrjm.sHtML

[U55] PHP：match 表达式
来源：http://wap.epnwcf.com/Article/details/gmvtbelqb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.bbcook.cn/Article/details/ghzgyfiua.sHtML

[U56] PHP：命名参数
来源：http://blog.vehdjk.com/Article/details/gqptipnjo.sHtML

f(a: 1, b: 2)
来源：http://wap.bbcook.cn/Article/details/gqlfukqbb.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/gqkbqlcxx.sHtML

"值: {$a}"
来源：http://www.share.sjlbkw.cn/Article/details/gkgeooosf.sHtML

[U58] PHP：数组三件套
来源：http://blog.sjlbkw.cn/Article/details/geopneoez.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.epnwcf.com/Article/details/gmhklnffd.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.yfazqb.com/Article/details/guqaltpeb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.tarul.cn/Article/details/gzjahbovh.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.vehdjk.com/Article/details/gjfqqtgse.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.tarul.cn/Article/details/ghqxquagw.sHtML

[U61] PHP：正则
来源：http://www.blog.vehdjk.com/Article/details/gxwwfyjxg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.vehdjk.com/Article/details/gtuzstebf.sHtML

[U62] PHP：日期对象
来源：http://www.blog.vehdjk.com/Article/details/gahkiipjb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.epnwcf.com/Article/details/gcomsbcfd.sHtML

[U63] PHP：文件读写
来源：http://www.blog.yfazqb.com/Article/details/gjmrkxyfs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fktsv.cn/Article/details/gqfptymcm.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.yfazqb.com/Article/details/gekksyocq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.vehdjk.com/Article/details/gsmmgrcqa.sHtML

[U65] PHP：会话
来源：http://www.share.yfazqb.com/Article/details/gqamquqcs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gkdmnmmfr.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.sjlbkw.cn/Article/details/gfeyijhfa.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.sjlbkw.cn/Article/details/gfelkjqog.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.tarul.cn/Article/details/gvawpjbzs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.vehdjk.com/Article/details/gihuhxhet.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.tarul.cn/Article/details/gknhzzdbg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.tarul.cn/Article/details/gtnrykmxd.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.yfazqb.com/Article/details/ggtdqafvd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.bbcook.cn/Article/details/grxeceqyu.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.epnwcf.com/Article/details/ggzjizqjc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fktsv.cn/Article/details/gxtrzvffe.sHtML

[U71] PHP：抛出异常
来源：http://read.share.epnwcf.com/Article/details/gkbvnfifu.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.yfazqb.com/Article/details/godqbtncv.sHtML

[U72] PHP：写错误日志
来源：http://blog.sjlbkw.cn/Article/details/gggppdtvk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.epnwcf.com/Article/details/gtxkxqyhn.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.epnwcf.com/Article/details/gxcrlebot.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.tarul.cn/Article/details/glrzdlpwt.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.bbcook.cn/Article/details/gtxrryzlw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.yfazqb.com/Article/details/gfmyvnair.sHtML

[U75] PHP：依赖注入
来源：http://baike.tarul.cn/Article/details/gqrzweavy.sHtML

composer require psr/container
来源：http://3g.epnwcf.com/Article/details/gjvecmnig.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.bbcook.cn/Article/details/gixnjotrm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.bbcook.cn/Article/details/gnvzitujv.sHtML

[U77] PHP：模板渲染
来源：http://wap.vehdjk.com/Article/details/gxjksvcps.sHtML

composer require twig/twig
来源：http://read.share.epnwcf.com/Article/details/goqcrwsrd.sHtML

[U78] PHP：单元测试
来源：http://wap.epnwcf.com/Article/details/gzjukatcv.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.vehdjk.com/Article/details/gfxfqswwf.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fktsv.cn/Article/details/gspiacatz.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.tarul.cn/Article/details/gqhzkhlhj.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.epnwcf.com/Article/details/ghkepnrct.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.tarul.cn/Article/details/gprqfhbnt.sHtML

[U81] JS：初始化项目
来源：http://blog.fktsv.cn/Article/details/gxkcmodkh.sHtML

npm init -y;  npm i express
来源：http://read.share.tarul.cn/Article/details/gdxlcypjq.sHtML

[U82] JS：package.json 脚本
来源：http://blog.yfazqb.com/Article/details/ghslfwnbn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.vehdjk.com/Article/details/gyvvoyvne.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.tarul.cn/Article/details/gvmsywdgd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.vehdjk.com/Article/details/gwmdgscla.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.sjlbkw.cn/Article/details/gzkyagivt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.yfazqb.com/Article/details/gprvuxhva.sHtML

[U85] JS：可选链
来源：http://www.blog.sjlbkw.cn/Article/details/gburmyrxq.sHtML

a?.b?.c
来源：http://www.m.share.sjlbkw.cn/Article/details/gjawferel.sHtML

[U86] JS：空值合并
来源：http://www.blog.epnwcf.com/Article/details/gzqxdkozi.sHtML

a ?? b
来源：http://www.m.share.yfazqb.com/Article/details/gvsequgoj.sHtML

[U87] JS：解构默认值
来源：http://www.share.yfazqb.com/Article/details/ggbjjypil.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.sjlbkw.cn/Article/details/giqiukqbc.sHtML

[U88] JS：对象展开合并
来源：http://blog.vehdjk.com/Article/details/gyifgerhw.sHtML

{ ...a, ...b }
来源：http://mobile.epnwcf.com/Article/details/gsjgtieup.sHtML

[U89] JS：数组去重
来源：http://read.share.tarul.cn/Article/details/gufdwtrgr.sHtML

[...new Set(arr)]
来源：http://mobile.yfazqb.com/Article/details/gronzusgc.sHtML

[U90] JS：数字数组排序
来源：http://www.share.yfazqb.com/Article/details/goptmbnnc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/geqkplyqf.sHtML

[U91] JS：对象键值遍历
来源：http://wap.sjlbkw.cn/Article/details/gxpjkwvxj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fktsv.cn/Article/details/gcfvzvasd.sHtML

[U92] JS：深拷贝
来源：http://3g.yfazqb.com/Article/details/gtfelwwbq.sHtML

structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/goudwsuxl.sHtML

[U93] JS：模板字符串
来源：http://read.share.epnwcf.com/Article/details/gmjzpdngo.sHtML

`共 ${n} 条`
来源：http://3g.vehdjk.com/Article/details/gtfqcpuwz.sHtML

[U94] JS：箭头函数
来源：http://3g.yfazqb.com/Article/details/gouijkhtb.sHtML

const double = x => x * 2;
来源：http://www.m.share.yfazqb.com/Article/details/gxvoktfos.sHtML

[U95] JS：Promise 包装
来源：http://3g.sjlbkw.cn/Article/details/gidrnlvbc.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.yfazqb.com/Article/details/gnvtuhgoo.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.epnwcf.com/Article/details/gkyrwqfbr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gzqysujcm.sHtML

[U97] JS：并发请求
来源：http://mobile.sjlbkw.cn/Article/details/gdiktqxuk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/gukeqwxas.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.bbcook.cn/Article/details/gssrhqtec.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.yfazqb.com/Article/details/gcgiofkza.sHtML

[U99] JS：事件监听
来源：http://mobile.bbcook.cn/Article/details/gyjjrvnsp.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.sjlbkw.cn/Article/details/godiosviu.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.bbcook.cn/Article/details/gyxnxgndm.sHtML

document.querySelector(".item")
来源：http://www.blog.tarul.cn/Article/details/gepqqmfuj.sHtML

[U101] JS：classList 操作
来源：http://wap.bbcook.cn/Article/details/gzrkpkwlb.sHtML

el.classList.toggle("active")
来源：http://read.share.epnwcf.com/Article/details/grlnbwfjj.sHtML

[U102] JS：本地存储
来源：http://www.blog.fktsv.cn/Article/details/guwtgyinz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.epnwcf.com/Article/details/gkmnovrxh.sHtML

[U103] JS：定时器
来源：http://mobile.fktsv.cn/Article/details/gvpuazsfi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.epnwcf.com/Article/details/grvoqxspd.sHtML

[U104] JS：防抖
来源：http://3g.epnwcf.com/Article/details/ghklndpng.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gbvlqdlwz.sHtML

[U105] JS：节流
来源：http://3g.sjlbkw.cn/Article/details/gxjjxbegp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.tarul.cn/Article/details/gxdtcwsyv.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fktsv.cn/Article/details/glsgkeaso.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.tarul.cn/Article/details/gfkqfxcsi.sHtML

[U107] JS：数字千分位
来源：http://mobile.bbcook.cn/Article/details/grsvnpets.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.tarul.cn/Article/details/gagglsteu.sHtML

[U108] JS：随机整数
来源：http://www.m.share.epnwcf.com/Article/details/gqavsqfqn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fktsv.cn/Article/details/gvufdpyzb.sHtML

[U109] JS：数组分组
来源：http://baike.sjlbkw.cn/Article/details/ghqvzlrrh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.sjlbkw.cn/Article/details/gxjcbtwyr.sHtML

[U110] JS：数组分块
来源：http://mobile.tarul.cn/Article/details/glplcoqsv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.bbcook.cn/Article/details/gmaoofkja.sHtML

[U111] JS：对象转 Map
来源：http://read.share.vehdjk.com/Article/details/gdvyjkoir.sHtML

new Map(Object.entries(obj))
来源：http://read.share.vehdjk.com/Article/details/geievkoej.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fktsv.cn/Article/details/gohrkbecm.sHtML

"7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gfqdstwuz.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.yfazqb.com/Article/details/gqjrawvrl.sHtML

s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gczpqqdsj.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.bbcook.cn/Article/details/ggrnyccdt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.tarul.cn/Article/details/glbefufhs.sHtML

[U115] JS：生成 UUID
来源：http://www.share.yfazqb.com/Article/details/gmvjlzgin.sHtML

crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gsimetoci.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.yfazqb.com/Article/details/ggziuguvo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.epnwcf.com/Article/details/guxftaiya.sHtML

[U117] JS：单元测试
来源：http://mobile.tarul.cn/Article/details/ggfuehyfm.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.epnwcf.com/Article/details/gjxjutcux.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.yfazqb.com/Article/details/gupieblge.sHtML

npm i -D vite;  npx vite
来源：http://baike.epnwcf.com/Article/details/gltmazcms.sHtML

[U119] JS：生产构建
来源：http://www.m.share.vehdjk.com/Article/details/gshhphnbx.sHtML

npx vite build
来源：http://mobile.epnwcf.com/Article/details/gknzzgjkm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.epnwcf.com/Article/details/gmfdaodgm.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.vehdjk.com/Article/details/gprbidlpi.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/goxjewwsr.sHtML

统计汇总
来源：http://m.share.epnwcf.com/Article/details/gmhgptxkz.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gmqqlaiqr.sHtML

按语言统计（条）：
来源：http://blog.yfazqb.com/Article/details/gfsegajqo.sHtML

Python ......... 252
来源：http://mobile.tarul.cn/Article/details/gwiojdhgg.sHtML

PHP ............ 252
来源：http://baike.vehdjk.com/Article/details/gnibnzoha.sHtML

JavaScript ..... 252
来源：http://www.share.fktsv.cn/Article/details/glqawxtla.sHtML

TypeScript ..... 212
来源：http://mobile.yfazqb.com/Article/details/gzkttxlpc.sHtML

Java ........... 212
来源：http://read.share.tarul.cn/Article/details/gnhkioync.sHtML

Go ............. 212
来源：http://mobile.sjlbkw.cn/Article/details/gqecycpez.sHtML

Ruby ........... 212
来源：http://www.m.share.tarul.cn/Article/details/ghqhqokyu.sHtML

C# ............. 212
来源：http://www.blog.vehdjk.com/Article/details/gdyqllvem.sHtML

C .............. 30
来源：http://www.blog.vehdjk.com/Article/details/ggpnrqthd.sHtML

C++ ............ 30
来源：http://baike.sjlbkw.cn/Article/details/gejlllbwk.sHtML

SQL ............ 90
来源：http://blog.tarul.cn/Article/details/gsbexlysv.sHtML

Bash ........... 80
来源：http://blog.sjlbkw.cn/Article/details/ghhhdufla.sHtML

Kotlin ......... 15
来源：http://3g.bbcook.cn/Article/details/giczpebfs.sHtML

Swift .......... 15
来源：http://blog.epnwcf.com/Article/details/gqkhvofun.sHtML

Lua ............ 10
来源：http://wap.epnwcf.com/Article/details/ghvavbqxw.sHtML

Perl ........... 10
来源：http://mobile.epnwcf.com/Article/details/gyzyggwfa.sHtML

Scala .......... 10
来源：http://3g.epnwcf.com/Article/details/gftkzkojp.sHtML

------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gsptcungz.sHtML

合计 ........... 2106 条
来源：http://www.blog.yfazqb.com/Article/details/gxfzjrjed.sHtML

按章节统计：
来源：http://3g.vehdjk.com/Article/details/gepwxslqz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.tarul.cn/Article/details/gwsqryewn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.yfazqb.com/Article/details/gpkgmbfmv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.bbcook.cn/Article/details/glbhwwldl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.vehdjk.com/Article/details/gmfmxheyy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.sjlbkw.cn/Article/details/gegljktpg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.bbcook.cn/Article/details/gvvcvdxiv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/gjkvdyoca.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.yfazqb.com/Article/details/giilxzudq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/gbqywftmi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.sjlbkw.cn/Article/details/gaeosducr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/gghfgtivz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/guwwkhskz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/gehaxbpvr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fktsv.cn/Article/details/gbnpsvvkm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.tarul.cn/Article/details/gunoxemse.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/gskhmivbg.sHtML

Q SQL 专题                              90
来源：http://m.share.epnwcf.com/Article/details/groefsgef.sHtML

R Bash 专题                             80
来源：http://read.share.vehdjk.com/Article/details/ggrkrfrww.sHtML

S C / C++ 专题                          60
来源：http://wap.fktsv.cn/Article/details/gltvuvyxg.sHtML

T 其他语言补充                          60
来源：http://wap.yfazqb.com/Article/details/grskdllzp.sHtML

U 高频实用片段                         120
来源：http://wap.vehdjk.com/Article/details/gyicluzkf.sHtML

------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gmhlwtqst.sHtML

合计                                  2106 条
来源：http://mobile.bbcook.cn/Article/details/goyrgtssn.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gnnhneruv.sHtML

使用提醒
来源：http://m.share.yfazqb.com/Article/details/gpvlbnimm.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gcvgpiqbz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.vehdjk.com/Article/details/georzklom.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.bbcook.cn/Article/details/gnareoyxv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.tarul.cn/Article/details/gsbdjxpun.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fktsv.cn/Article/details/gzcyltlzt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.epnwcf.com/Article/details/gzcijqqqf.sHtML

—— 文件结束 ——
来源：http://m.share.epnwcf.com/Article/details/gufcqbbfw.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gwtxxptbe.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.yfazqb.com/Article/details/gixwcaevm.sHtML

Common Programming Examples Cheat Book
来源：http://wap.bbcook.cn/Article/details/gaeypohfb.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gdtzahkdz.sHtML

【收录内容】
来源：http://www.share.bbcook.cn/Article/details/gzvksxwnb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.tarul.cn/Article/details/gfpstmfrj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.bbcook.cn/Article/details/gmbedkujf.sHtML

SQL · Bash · C · C++
来源：http://m.share.epnwcf.com/Article/details/gmnpuzdlr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.yfazqb.com/Article/details/gmnylvqxr.sHtML

【使用说明】
来源：http://baike.bbcook.cn/Article/details/ghwfjbkxu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.epnwcf.com/Article/details/ggcnalory.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.vehdjk.com/Article/details/gvwwhzmwh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.epnwcf.com/Article/details/gexqgjkuj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.yfazqb.com/Article/details/gasvhahze.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.vehdjk.com/Article/details/gjebxexve.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.vehdjk.com/Article/details/glrutheqz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.epnwcf.com/Article/details/gzuwjssyd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.sjlbkw.cn/Article/details/gyfhumgmh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.vehdjk.com/Article/details/ggizyrrxz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.epnwcf.com/Article/details/ghuupopjq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.yfazqb.com/Article/details/gifzxjzes.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.tarul.cn/Article/details/gagpccywa.sHtML

【文件统计】
来源：http://www.m.share.epnwcf.com/Article/details/gxdehjcnx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fktsv.cn/Article/details/gcvyfuvyf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/gcapkbyvx.sHtML

目  录
来源：http://www.m.share.bbcook.cn/Article/details/gettrfitu.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/ghvaslgxi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.sjlbkw.cn/Article/details/gpsnhnphx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fktsv.cn/Article/details/gyrhgbyms.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.vehdjk.com/Article/details/gcynwiduh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fktsv.cn/Article/details/gayukzzun.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.epnwcf.com/Article/details/gpphilwpm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gixbwdwpi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.vehdjk.com/Article/details/gyjfatuji.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.epnwcf.com/Article/details/ghgqvkhmq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fktsv.cn/Article/details/gsuantrpz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.bbcook.cn/Article/details/ggrzmsydc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.bbcook.cn/Article/details/gedwdylnp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gwmhxlyig.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/giyyqqnvo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fktsv.cn/Article/details/gbtihsgbl.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.bbcook.cn/Article/details/gzmfnkcgd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.yfazqb.com/Article/details/ggrmakdki.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.tarul.cn/Article/details/gjpqwiynp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.vehdjk.com/Article/details/giutcretu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fktsv.cn/Article/details/ghizyxvah.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fktsv.cn/Article/details/gxxflwekb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fktsv.cn/Article/details/gnhtqyxvu.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbdmoyqrp.sHtML

A. 基础语法与类型
来源：http://mobile.epnwcf.com/Article/details/gljtdigbw.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gjyouovfu.sHtML

[A01] Hello World
来源：http://www.share.vehdjk.com/Article/details/gnqdznkwy.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fktsv.cn/Article/details/gmsvjqcyy.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.epnwcf.com/Article/details/giprgxeei.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.yfazqb.com/Article/details/gypybqbxj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.bbcook.cn/Article/details/gcgrqqeok.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.sjlbkw.cn/Article/details/gourspubx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fktsv.cn/Article/details/gvkrcivbj.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.tarul.cn/Article/details/gerdubaoy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.yfazqb.com/Article/details/gmkvyirwn.sHtML

[A02] 变量声明与赋值
来源：http://baike.fktsv.cn/Article/details/gapfgjyaz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.epnwcf.com/Article/details/gqtlejqur.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.tarul.cn/Article/details/gtimcksgq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.bbcook.cn/Article/details/gazxqynji.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.bbcook.cn/Article/details/gclobnftv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.epnwcf.com/Article/details/gewbijiae.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.vehdjk.com/Article/details/gsksfawqp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fktsv.cn/Article/details/ghqzaenir.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.sjlbkw.cn/Article/details/gqzefgyai.sHtML

[A03] 常量定义
来源：http://read.share.epnwcf.com/Article/details/gwnkftlst.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.vehdjk.com/Article/details/glmkwmwzn.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/ggwrgerrq.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gnfjqoerw.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gnwxxrzcm.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gaabwrwio.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.vehdjk.com/Article/details/gzgellsgr.sHtML

Ruby: PI = 3.14159
来源：http://read.share.tarul.cn/Article/details/gkxbgtimo.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gqpbvodns.sHtML

[A04] 判断变量类型
来源：http://www.blog.sjlbkw.cn/Article/details/gvnuzpllx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fktsv.cn/Article/details/gyeslevnt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.epnwcf.com/Article/details/gimrwmaoc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fktsv.cn/Article/details/gbsdgpaad.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.yfazqb.com/Article/details/gsjmwijeu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.epnwcf.com/Article/details/gkfhveqsv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.tarul.cn/Article/details/gqjldpseq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.bbcook.cn/Article/details/gklpczetr.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.sjlbkw.cn/Article/details/gplhqrbtj.sHtML

[A05] 整数除法与取模
来源：http://read.share.yfazqb.com/Article/details/gcsyhztgw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.epnwcf.com/Article/details/gtogayysy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.tarul.cn/Article/details/gbzbwnezm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.epnwcf.com/Article/details/gzqyiqmcr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.tarul.cn/Article/details/gsesftusg.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/galcknbii.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/gsaolssmr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gdxdyynjz.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fktsv.cn/Article/details/ggqibbfjt.sHtML

[A06] 字符串转数字
来源：http://mobile.vehdjk.com/Article/details/gzeekstpg.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.vehdjk.com/Article/details/gizqiqykn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.epnwcf.com/Article/details/gzlztekxj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.tarul.cn/Article/details/gnkbepdkh.sHtML


<!-- 参考信息 -->