代发 wailian999

[U47] PHP：联合类型
来源：http://www.share.vehdjk.com/Article/details/gktbwnfvx.sHtML

int|string $id
来源：http://baike.bbcook.cn/Article/details/gnkhfnnky.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fktsv.cn/Article/details/geonsnpql.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.vehdjk.com/Article/details/gvnzrmjsn.sHtML

[U49] PHP：只读属性
来源：http://blog.tarul.cn/Article/details/gfwhniado.sHtML

public readonly string $name
来源：http://www.m.share.fktsv.cn/Article/details/grtcltpmm.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.sjlbkw.cn/Article/details/ghhoexdbn.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.epnwcf.com/Article/details/gckpmqirh.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fktsv.cn/Article/details/gmuqmahju.sHtML

[$a, $b] = $arr;
来源：http://baike.yfazqb.com/Article/details/grlgpfxrz.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fktsv.cn/Article/details/gfemqivwo.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.tarul.cn/Article/details/ggdiogkri.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.tarul.cn/Article/details/grvcixqye.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.epnwcf.com/Article/details/gtonovpyk.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fktsv.cn/Article/details/gjifqzdov.sHtML

$obj?->method()
来源：http://read.share.fktsv.cn/Article/details/geuvsoceg.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.bbcook.cn/Article/details/gclkygcxd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.tarul.cn/Article/details/gzqpqkweh.sHtML

[U56] PHP：命名参数
来源：http://baike.yfazqb.com/Article/details/gekuwezno.sHtML

f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/ghhcvreex.sHtML

[U57] PHP：字符串插值
来源：http://baike.fktsv.cn/Article/details/gvrjxlnmc.sHtML

"值: {$a}"
来源：http://wap.sjlbkw.cn/Article/details/gnntetcea.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.sjlbkw.cn/Article/details/guqogxalt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gcmupvgxs.sHtML

[U59] PHP：自定义排序
来源：http://mobile.tarul.cn/Article/details/gmnmgrbhl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.vehdjk.com/Article/details/goectuydx.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.epnwcf.com/Article/details/gnqntsalx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fktsv.cn/Article/details/gjmmxkmrd.sHtML

[U61] PHP：正则
来源：http://baike.epnwcf.com/Article/details/gzffoklbh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.yfazqb.com/Article/details/gfoqjnlhs.sHtML

[U62] PHP：日期对象
来源：http://www.share.epnwcf.com/Article/details/gvidesdos.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.sjlbkw.cn/Article/details/gffelayqg.sHtML

[U63] PHP：文件读写
来源：http://mobile.tarul.cn/Article/details/gwfgdhrzk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.bbcook.cn/Article/details/ggoljnykz.sHtML

[U64] PHP：目录遍历
来源：http://www.share.bbcook.cn/Article/details/gqpzncdhc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.sjlbkw.cn/Article/details/gajjdjdov.sHtML

[U65] PHP：会话
来源：http://www.share.yfazqb.com/Article/details/gvclquxwy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.yfazqb.com/Article/details/gldjvkwgd.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.yfazqb.com/Article/details/gqlfrolqu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fktsv.cn/Article/details/gclxcdhvf.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.sjlbkw.cn/Article/details/gjbvohlha.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.tarul.cn/Article/details/gjzgqkiyl.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.tarul.cn/Article/details/grcuvwigy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.sjlbkw.cn/Article/details/gxtjznrvy.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.tarul.cn/Article/details/glocqmagg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.vehdjk.com/Article/details/gxtsrdiar.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.tarul.cn/Article/details/gbzfupggl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.bbcook.cn/Article/details/gamjjentp.sHtML

[U71] PHP：抛出异常
来源：http://m.share.yfazqb.com/Article/details/gizfpvrfq.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.yfazqb.com/Article/details/gcscnrzni.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.sjlbkw.cn/Article/details/gnfqpwjvq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.vehdjk.com/Article/details/gbqpcpluy.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.vehdjk.com/Article/details/gbkglnjhn.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.epnwcf.com/Article/details/gaqkotljo.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/gfxbhdxgx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fktsv.cn/Article/details/ghmnzqwvh.sHtML

[U75] PHP：依赖注入
来源：http://www.share.tarul.cn/Article/details/gvmmckrzj.sHtML

composer require psr/container
来源：http://blog.sjlbkw.cn/Article/details/glucwuzpt.sHtML

[U76] PHP：简单路由
来源：http://www.blog.sjlbkw.cn/Article/details/gzfurgflk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.bbcook.cn/Article/details/ganvsvnds.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.tarul.cn/Article/details/gglrxfsrf.sHtML

composer require twig/twig
来源：http://baike.sjlbkw.cn/Article/details/gfdrnhjzs.sHtML

[U78] PHP：单元测试
来源：http://baike.yfazqb.com/Article/details/gkghcuhhb.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.tarul.cn/Article/details/gozawpfzn.sHtML

[U79] PHP：静态分析
来源：http://www.share.yfazqb.com/Article/details/gxqrhsjfg.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.vehdjk.com/Article/details/gxayromst.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.tarul.cn/Article/details/gezzbrvbd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fktsv.cn/Article/details/gajqbnnom.sHtML

[U81] JS：初始化项目
来源：http://www.blog.vehdjk.com/Article/details/gfecjdwaz.sHtML

npm init -y;  npm i express
来源：http://www.share.tarul.cn/Article/details/gcbkfwiuh.sHtML

[U82] JS：package.json 脚本
来源：http://baike.sjlbkw.cn/Article/details/gibumbsll.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fktsv.cn/Article/details/gorehxron.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fktsv.cn/Article/details/gfuixelog.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.tarul.cn/Article/details/geejihfrk.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fktsv.cn/Article/details/gezwwwaan.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.bbcook.cn/Article/details/gvzusuhnn.sHtML

[U85] JS：可选链
来源：http://3g.fktsv.cn/Article/details/gywmhwbuc.sHtML

a?.b?.c
来源：http://mobile.tarul.cn/Article/details/gciisvair.sHtML

[U86] JS：空值合并
来源：http://wap.fktsv.cn/Article/details/gxrcsusny.sHtML

a ?? b
来源：http://wap.fktsv.cn/Article/details/gzwxcrdii.sHtML

[U87] JS：解构默认值
来源：http://baike.yfazqb.com/Article/details/gvfrwcqde.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.bbcook.cn/Article/details/gupcainat.sHtML

[U88] JS：对象展开合并
来源：http://3g.vehdjk.com/Article/details/gkoinyodp.sHtML

{ ...a, ...b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqprmzcg.sHtML

[U89] JS：数组去重
来源：http://wap.sjlbkw.cn/Article/details/gszrrblmy.sHtML

[...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/gbycmgect.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.bbcook.cn/Article/details/gzwwmwara.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gjfwdelbk.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.sjlbkw.cn/Article/details/gzmfqnawa.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.tarul.cn/Article/details/gvfzxfzcu.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.bbcook.cn/Article/details/ghjgevsfs.sHtML

structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/getzkonkx.sHtML

[U93] JS：模板字符串
来源：http://mobile.sjlbkw.cn/Article/details/gpshywhpw.sHtML

`共 ${n} 条`
来源：http://3g.epnwcf.com/Article/details/gbkpzvaen.sHtML

[U94] JS：箭头函数
来源：http://blog.bbcook.cn/Article/details/gvbyzsdbi.sHtML

const double = x => x * 2;
来源：http://baike.tarul.cn/Article/details/gtmpynfxv.sHtML

[U95] JS：Promise 包装
来源：http://m.share.vehdjk.com/Article/details/gcsbmqmss.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.tarul.cn/Article/details/gejrsfnca.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.epnwcf.com/Article/details/gmozbsvhd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/gmnvvhkol.sHtML

[U97] JS：并发请求
来源：http://blog.sjlbkw.cn/Article/details/gofdurnhb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.vehdjk.com/Article/details/guddlwlxj.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.vehdjk.com/Article/details/gixjjcwcd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.bbcook.cn/Article/details/giabpsilw.sHtML

[U99] JS：事件监听
来源：http://m.share.vehdjk.com/Article/details/gvekewrtt.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fktsv.cn/Article/details/gowgvhauk.sHtML

[U100] JS：DOM 查询
来源：http://mobile.vehdjk.com/Article/details/gdbddhamc.sHtML

document.querySelector(".item")
来源：http://read.share.yfazqb.com/Article/details/gdbrekeaq.sHtML

[U101] JS：classList 操作
来源：http://mobile.yfazqb.com/Article/details/gxehcdzgv.sHtML

el.classList.toggle("active")
来源：http://3g.bbcook.cn/Article/details/goydixejk.sHtML

[U102] JS：本地存储
来源：http://3g.tarul.cn/Article/details/gqarrmrmf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.yfazqb.com/Article/details/gasadmsyt.sHtML

[U103] JS：定时器
来源：http://baike.bbcook.cn/Article/details/gtdpjgyiz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.vehdjk.com/Article/details/gtvgcfsgr.sHtML

[U104] JS：防抖
来源：http://blog.yfazqb.com/Article/details/gfpzqshkk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/gfxkhtaay.sHtML

[U105] JS：节流
来源：http://www.share.yfazqb.com/Article/details/gzskuomyv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.tarul.cn/Article/details/gejuiaozn.sHtML

[U106] JS：日期格式化
来源：http://wap.fktsv.cn/Article/details/giaqmsmtp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fktsv.cn/Article/details/gmuznwihp.sHtML

[U107] JS：数字千分位
来源：http://www.blog.tarul.cn/Article/details/gxpnevnut.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.epnwcf.com/Article/details/guhjfkoeu.sHtML

[U108] JS：随机整数
来源：http://www.share.tarul.cn/Article/details/gjvxpuuwg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.yfazqb.com/Article/details/gboursmqr.sHtML

[U109] JS：数组分组
来源：http://blog.tarul.cn/Article/details/gfgbuqwdx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.yfazqb.com/Article/details/gdqatqvdr.sHtML

[U110] JS：数组分块
来源：http://3g.yfazqb.com/Article/details/gnmribwkd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fktsv.cn/Article/details/gojpepkxz.sHtML

[U111] JS：对象转 Map
来源：http://wap.fktsv.cn/Article/details/gxzdysxaw.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.yfazqb.com/Article/details/gbhtigoyu.sHtML

[U112] JS：字符串补位
来源：http://baike.vehdjk.com/Article/details/gcmbewexn.sHtML

"7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gcdexaiaj.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fktsv.cn/Article/details/gyprmbgqx.sHtML

s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/ghlklhkpw.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.vehdjk.com/Article/details/ghswowohp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fktsv.cn/Article/details/gulisnqis.sHtML

[U115] JS：生成 UUID
来源：http://blog.sjlbkw.cn/Article/details/gqfoedpib.sHtML

crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/grnzpwjzb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.bbcook.cn/Article/details/gyldpvyfg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.vehdjk.com/Article/details/gwmxyugqn.sHtML

[U117] JS：单元测试
来源：http://www.blog.epnwcf.com/Article/details/gpkpqpamu.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.yfazqb.com/Article/details/gtzubcsot.sHtML

[U118] JS：开发服务器
来源：http://baike.yfazqb.com/Article/details/gibwezcqg.sHtML

npm i -D vite;  npx vite
来源：http://3g.epnwcf.com/Article/details/glsvwbskb.sHtML

[U119] JS：生产构建
来源：http://www.blog.fktsv.cn/Article/details/gkilwsllv.sHtML

npx vite build
来源：http://m.share.fktsv.cn/Article/details/gtmqrupbd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.epnwcf.com/Article/details/gcgqofzlf.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.sjlbkw.cn/Article/details/gqcwbmuyn.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gienwivei.sHtML

统计汇总
来源：http://mobile.sjlbkw.cn/Article/details/gofysycma.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gyjkolqwm.sHtML

按语言统计（条）：
来源：http://read.share.epnwcf.com/Article/details/geokanqys.sHtML

Python ......... 252
来源：http://www.share.bbcook.cn/Article/details/gtwszoitc.sHtML

PHP ............ 252
来源：http://m.share.fktsv.cn/Article/details/glbelrumq.sHtML

JavaScript ..... 252
来源：http://read.share.epnwcf.com/Article/details/gwrokigqb.sHtML

TypeScript ..... 212
来源：http://wap.yfazqb.com/Article/details/gimwxgimg.sHtML

Java ........... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdubnuuu.sHtML

Go ............. 212
来源：http://m.share.tarul.cn/Article/details/gngpclrjk.sHtML

Ruby ........... 212
来源：http://wap.yfazqb.com/Article/details/gyvloqrhb.sHtML

C# ............. 212
来源：http://read.share.vehdjk.com/Article/details/gasgwslvo.sHtML

C .............. 30
来源：http://www.m.share.vehdjk.com/Article/details/guowlhile.sHtML

C++ ............ 30
来源：http://wap.sjlbkw.cn/Article/details/gegxgrvwi.sHtML

SQL ............ 90
来源：http://blog.sjlbkw.cn/Article/details/gslckhutb.sHtML

Bash ........... 80
来源：http://www.blog.sjlbkw.cn/Article/details/ghcgnxfas.sHtML

Kotlin ......... 15
来源：http://blog.sjlbkw.cn/Article/details/gwtidytpm.sHtML

Swift .......... 15
来源：http://blog.yfazqb.com/Article/details/gipjqkcci.sHtML

Lua ............ 10
来源：http://www.m.share.epnwcf.com/Article/details/gnjlnjjqv.sHtML

Perl ........... 10
来源：http://www.blog.vehdjk.com/Article/details/gxgjaoubs.sHtML

Scala .......... 10
来源：http://read.share.tarul.cn/Article/details/gzhsxymgi.sHtML

------------------------------------
来源：http://m.share.fktsv.cn/Article/details/glutfuczf.sHtML

合计 ........... 2106 条
来源：http://mobile.fktsv.cn/Article/details/gvvrwptnq.sHtML

按章节统计：
来源：http://www.blog.tarul.cn/Article/details/gqwbdgfny.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.tarul.cn/Article/details/glyqnatlq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.sjlbkw.cn/Article/details/gmqdyhoac.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/gevfubbuy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.vehdjk.com/Article/details/gnfsigwqv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.epnwcf.com/Article/details/giusmomib.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.bbcook.cn/Article/details/gvlxzvouz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.tarul.cn/Article/details/gvmvzldej.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.sjlbkw.cn/Article/details/gzvqijrso.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/gsscngace.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.sjlbkw.cn/Article/details/gckwqbtlo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/gbehwplzh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gwjzfemfr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gequreerp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.bbcook.cn/Article/details/gscmlyxqq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.epnwcf.com/Article/details/gdqrclocy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gzcwrzngs.sHtML

Q SQL 专题                              90
来源：http://blog.sjlbkw.cn/Article/details/gqliiijhk.sHtML

R Bash 专题                             80
来源：http://baike.epnwcf.com/Article/details/gndfbvroz.sHtML

S C / C++ 专题                          60
来源：http://www.share.sjlbkw.cn/Article/details/gpcjvqytd.sHtML

T 其他语言补充                          60
来源：http://www.share.tarul.cn/Article/details/gtevcqdov.sHtML

U 高频实用片段                         120
来源：http://blog.vehdjk.com/Article/details/glklhgepz.sHtML

------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gjkztawml.sHtML

合计                                  2106 条
来源：http://wap.yfazqb.com/Article/details/gcipmtiit.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fktsv.cn/Article/details/gjdxfukux.sHtML

使用提醒
来源：http://baike.vehdjk.com/Article/details/gatasgaer.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fktsv.cn/Article/details/ggbdlajhx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.yfazqb.com/Article/details/galwkdnta.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.bbcook.cn/Article/details/gslsocolf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fktsv.cn/Article/details/guzvzsays.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.epnwcf.com/Article/details/gqqgngzuh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.yfazqb.com/Article/details/gjlylrhrg.sHtML

—— 文件结束 ——
来源：http://m.share.sjlbkw.cn/Article/details/ghuxtmoii.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gtirgucpo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.sjlbkw.cn/Article/details/gtoqzfurw.sHtML

Common Programming Examples Cheat Book
来源：http://baike.sjlbkw.cn/Article/details/gpslplpgk.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gebfcfyqm.sHtML

【收录内容】
来源：http://3g.fktsv.cn/Article/details/gwzthgnsq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.tarul.cn/Article/details/gfnpvnilk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.sjlbkw.cn/Article/details/glqwtonqa.sHtML

SQL · Bash · C · C++
来源：http://mobile.epnwcf.com/Article/details/glctqdjog.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.tarul.cn/Article/details/gxjxdobmv.sHtML

【使用说明】
来源：http://www.blog.sjlbkw.cn/Article/details/gbcffcfde.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.sjlbkw.cn/Article/details/gptvjvarh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.epnwcf.com/Article/details/gwbmmidmk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.epnwcf.com/Article/details/grxptbhlm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.vehdjk.com/Article/details/gvzcwairv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.sjlbkw.cn/Article/details/gluslvaaf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.epnwcf.com/Article/details/gpovknmpv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.yfazqb.com/Article/details/gijmtqkdg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fktsv.cn/Article/details/gnlfbmjkk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.bbcook.cn/Article/details/gjogfykxm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.bbcook.cn/Article/details/gehisbpds.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.epnwcf.com/Article/details/gbowvijqg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.tarul.cn/Article/details/gssoztnaw.sHtML

【文件统计】
来源：http://blog.epnwcf.com/Article/details/gouujpewz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.yfazqb.com/Article/details/ghiehyhvi.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gnpytyeum.sHtML

目  录
来源：http://blog.epnwcf.com/Article/details/gzcrbdqbm.sHtML

--------------------------------------------------------------------------------
来源：http://wap.yfazqb.com/Article/details/gurjmhpjq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.sjlbkw.cn/Article/details/gjoalwnxr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.yfazqb.com/Article/details/ghgcvxgwb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.tarul.cn/Article/details/gfoowayrx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.tarul.cn/Article/details/gfvjcixwy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.yfazqb.com/Article/details/gqppvvbab.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.sjlbkw.cn/Article/details/gelhwgsar.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fktsv.cn/Article/details/gjqecmqbc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fktsv.cn/Article/details/gyhhptbfz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gfdrheitz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.yfazqb.com/Article/details/grvapigqe.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/geqbhxmbu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gkqxzpolu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/gbcmnoxcj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.epnwcf.com/Article/details/gxmyqhgzp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.sjlbkw.cn/Article/details/gjpccdlei.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/gtococuqx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fktsv.cn/Article/details/ghxdwjbtr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.bbcook.cn/Article/details/gtqcrghfu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.tarul.cn/Article/details/glmbktqpa.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fktsv.cn/Article/details/gbgnrnuhr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.tarul.cn/Article/details/gfglkqjva.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gnllrkhvl.sHtML

A. 基础语法与类型
来源：http://blog.sjlbkw.cn/Article/details/gcjfczqbt.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnpnwvcz.sHtML

[A01] Hello World
来源：http://mobile.tarul.cn/Article/details/gwsvikzuo.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.vehdjk.com/Article/details/gplwnhuug.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.vehdjk.com/Article/details/gydqhdgxn.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.yfazqb.com/Article/details/gqbipuudm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.epnwcf.com/Article/details/givczidgr.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.sjlbkw.cn/Article/details/gtbneqxon.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.bbcook.cn/Article/details/goqhgpeha.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.bbcook.cn/Article/details/gbjeipvtf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.bbcook.cn/Article/details/gzptuadqp.sHtML

[A02] 变量声明与赋值
来源：http://blog.tarul.cn/Article/details/ghtshpbyg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.epnwcf.com/Article/details/gdftrcpqj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.vehdjk.com/Article/details/glsqawtbg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fktsv.cn/Article/details/gxydgolcz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fktsv.cn/Article/details/gdcspriuv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fktsv.cn/Article/details/glxwviczk.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.vehdjk.com/Article/details/glplptmbd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.tarul.cn/Article/details/gtmiyjqkn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.sjlbkw.cn/Article/details/guannfddk.sHtML

[A03] 常量定义
来源：http://baike.epnwcf.com/Article/details/gpimnaofa.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.yfazqb.com/Article/details/gsyuxeifu.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/ggynvyvev.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gbppfupqk.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gozpnpuku.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gcmthdgsh.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.sjlbkw.cn/Article/details/gglmjhijz.sHtML

Ruby: PI = 3.14159
来源：http://mobile.sjlbkw.cn/Article/details/ghgccqzve.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gcvonpjju.sHtML

[A04] 判断变量类型
来源：http://3g.vehdjk.com/Article/details/glhemwfbh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.yfazqb.com/Article/details/gcugxyijy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.yfazqb.com/Article/details/gijoxfrck.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.vehdjk.com/Article/details/gjcbbxiwa.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.yfazqb.com/Article/details/gnsloyeeb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.vehdjk.com/Article/details/gftntnsqn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fktsv.cn/Article/details/glytukjpi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.bbcook.cn/Article/details/gkmylaxfe.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fktsv.cn/Article/details/gxdtivmyp.sHtML

[A05] 整数除法与取模
来源：http://3g.fktsv.cn/Article/details/gklxgesnb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.vehdjk.com/Article/details/gwxatwtru.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gvnogxaow.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.bbcook.cn/Article/details/gahbjfqbu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.tarul.cn/Article/details/gdftisggn.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.epnwcf.com/Article/details/gdkwojqze.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.epnwcf.com/Article/details/ghfypmjyw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.tarul.cn/Article/details/gpyzoibtp.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.epnwcf.com/Article/details/ghomgcrxo.sHtML


<!-- 参考信息 -->