代发 wailian999

[U47] PHP：联合类型
来源：http://baike.tarul.cn/Article/details/grnwpnxme.sHtML

int|string $id
来源：http://www.blog.vehdjk.com/Article/details/gfbfzyrqf.sHtML

[U48] PHP：纯枚举
来源：http://3g.fktsv.cn/Article/details/gjctiicnb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.yfazqb.com/Article/details/gzqiagdbt.sHtML

[U49] PHP：只读属性
来源：http://wap.vehdjk.com/Article/details/gqjuebzvt.sHtML

public readonly string $name
来源：http://mobile.fktsv.cn/Article/details/gskaioabm.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fktsv.cn/Article/details/gdcllefdp.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.vehdjk.com/Article/details/gxddnpytr.sHtML

[U51] PHP：数组解构
来源：http://read.share.tarul.cn/Article/details/gimwqwzrk.sHtML

[$a, $b] = $arr;
来源：http://www.blog.yfazqb.com/Article/details/gtljvemvo.sHtML

[U52] PHP：箭头函数
来源：http://www.share.sjlbkw.cn/Article/details/gmjfirkgq.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.bbcook.cn/Article/details/grvndfuod.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fktsv.cn/Article/details/gjpreeruf.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.sjlbkw.cn/Article/details/gdlmsuovw.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.tarul.cn/Article/details/gojofwels.sHtML

$obj?->method()
来源：http://3g.epnwcf.com/Article/details/gmmdztfyc.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fktsv.cn/Article/details/gzubuuxhs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fktsv.cn/Article/details/gjmfobstx.sHtML

[U56] PHP：命名参数
来源：http://m.share.epnwcf.com/Article/details/gqdrfzsjw.sHtML

f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gqrblaxcl.sHtML

[U57] PHP：字符串插值
来源：http://blog.yfazqb.com/Article/details/gafdmlfqs.sHtML

"值: {$a}"
来源：http://blog.fktsv.cn/Article/details/gyfyhbpfi.sHtML

[U58] PHP：数组三件套
来源：http://mobile.yfazqb.com/Article/details/gvqulbwcm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gginoufvu.sHtML

[U59] PHP：自定义排序
来源：http://wap.epnwcf.com/Article/details/gbfncgqbu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.sjlbkw.cn/Article/details/gfixwgnjs.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.tarul.cn/Article/details/gmdsxjdia.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.vehdjk.com/Article/details/gicuktdsl.sHtML

[U61] PHP：正则
来源：http://m.share.vehdjk.com/Article/details/gvnundgxv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.sjlbkw.cn/Article/details/gaxcoglwz.sHtML

[U62] PHP：日期对象
来源：http://3g.fktsv.cn/Article/details/guohyekan.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.sjlbkw.cn/Article/details/gyddazowi.sHtML

[U63] PHP：文件读写
来源：http://www.share.vehdjk.com/Article/details/gthjvccld.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.epnwcf.com/Article/details/gzvgpikod.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/grzjdkmvu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.epnwcf.com/Article/details/gvuzsqzmw.sHtML

[U65] PHP：会话
来源：http://www.share.yfazqb.com/Article/details/gmtcluxsc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.tarul.cn/Article/details/ggzfgbbsf.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.tarul.cn/Article/details/gqxbrmkwb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.yfazqb.com/Article/details/gcitqbhlb.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.epnwcf.com/Article/details/gdhwbdifu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.vehdjk.com/Article/details/ghlbqymcz.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.epnwcf.com/Article/details/gxvdapece.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fktsv.cn/Article/details/goahpfcxl.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.bbcook.cn/Article/details/gtfdptddn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.bbcook.cn/Article/details/gtmmrcikg.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.tarul.cn/Article/details/gpshvnlhr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.bbcook.cn/Article/details/gzhrgsaki.sHtML

[U71] PHP：抛出异常
来源：http://read.share.epnwcf.com/Article/details/glcnimgzn.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.epnwcf.com/Article/details/gakvqakjh.sHtML

[U72] PHP：写错误日志
来源：http://www.share.epnwcf.com/Article/details/gksydtbkg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fktsv.cn/Article/details/goxibzjkj.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.tarul.cn/Article/details/gazifgpki.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.tarul.cn/Article/details/gikfnqsfs.sHtML

[U74] PHP：读取环境变量
来源：http://3g.vehdjk.com/Article/details/gtcisotpr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.tarul.cn/Article/details/gjhkqrqde.sHtML

[U75] PHP：依赖注入
来源：http://baike.sjlbkw.cn/Article/details/gvguetass.sHtML

composer require psr/container
来源：http://www.blog.yfazqb.com/Article/details/gksctrvtj.sHtML

[U76] PHP：简单路由
来源：http://mobile.bbcook.cn/Article/details/ggbisppff.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.yfazqb.com/Article/details/gajsdxlhq.sHtML

[U77] PHP：模板渲染
来源：http://3g.sjlbkw.cn/Article/details/gmsmzvelt.sHtML

composer require twig/twig
来源：http://www.share.sjlbkw.cn/Article/details/gylazvrmp.sHtML

[U78] PHP：单元测试
来源：http://baike.sjlbkw.cn/Article/details/gurprvbtr.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.epnwcf.com/Article/details/gmprydcxn.sHtML

[U79] PHP：静态分析
来源：http://read.share.vehdjk.com/Article/details/gxhgtafij.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.vehdjk.com/Article/details/gdcmcnpmy.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlphjzrs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.vehdjk.com/Article/details/gepgvlrub.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.tarul.cn/Article/details/gozacuwht.sHtML

npm init -y;  npm i express
来源：http://mobile.epnwcf.com/Article/details/gpkqjyngv.sHtML

[U82] JS：package.json 脚本
来源：http://blog.sjlbkw.cn/Article/details/grnbfjhca.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.epnwcf.com/Article/details/ghflgfefh.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.bbcook.cn/Article/details/gecxcugkr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.yfazqb.com/Article/details/gusegtadc.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.sjlbkw.cn/Article/details/gifxlrgix.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.yfazqb.com/Article/details/ggrlfgizb.sHtML

[U85] JS：可选链
来源：http://www.blog.vehdjk.com/Article/details/gocjeelxi.sHtML

a?.b?.c
来源：http://www.share.yfazqb.com/Article/details/grpizxtvl.sHtML

[U86] JS：空值合并
来源：http://www.m.share.sjlbkw.cn/Article/details/gtyncwoms.sHtML

a ?? b
来源：http://baike.yfazqb.com/Article/details/germacnxf.sHtML

[U87] JS：解构默认值
来源：http://www.share.fktsv.cn/Article/details/gnchhbqoi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.tarul.cn/Article/details/garjonljo.sHtML

[U88] JS：对象展开合并
来源：http://www.share.vehdjk.com/Article/details/gxbmyrvlx.sHtML

{ ...a, ...b }
来源：http://www.share.yfazqb.com/Article/details/gaxuzubbh.sHtML

[U89] JS：数组去重
来源：http://blog.fktsv.cn/Article/details/ghqgbxkhi.sHtML

[...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/ggvtskhns.sHtML

[U90] JS：数字数组排序
来源：http://mobile.epnwcf.com/Article/details/gvpqdhylr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/gttvfoxdl.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.sjlbkw.cn/Article/details/gswccfevt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.bbcook.cn/Article/details/grdenvgdn.sHtML

[U92] JS：深拷贝
来源：http://wap.fktsv.cn/Article/details/gxhsuyaos.sHtML

structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/gwlgsisue.sHtML

[U93] JS：模板字符串
来源：http://wap.yfazqb.com/Article/details/gevxwhfmf.sHtML

`共 ${n} 条`
来源：http://mobile.fktsv.cn/Article/details/gmxxtgtat.sHtML

[U94] JS：箭头函数
来源：http://www.blog.epnwcf.com/Article/details/ghoggazvp.sHtML

const double = x => x * 2;
来源：http://3g.bbcook.cn/Article/details/gxfwwvxhn.sHtML

[U95] JS：Promise 包装
来源：http://baike.epnwcf.com/Article/details/gprpmtxhi.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fktsv.cn/Article/details/gzfnmbwuv.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.yfazqb.com/Article/details/gjmhpadmy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gqhlznmbx.sHtML

[U97] JS：并发请求
来源：http://www.m.share.sjlbkw.cn/Article/details/gpoomsjcf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gzteqcnfy.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.epnwcf.com/Article/details/gklibbwqk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.tarul.cn/Article/details/gxrimobhh.sHtML

[U99] JS：事件监听
来源：http://3g.fktsv.cn/Article/details/ghwbuqkad.sHtML

el.addEventListener("click", e => {})
来源：http://baike.tarul.cn/Article/details/gnopbbgeq.sHtML

[U100] JS：DOM 查询
来源：http://m.share.vehdjk.com/Article/details/gnsqetyfx.sHtML

document.querySelector(".item")
来源：http://wap.bbcook.cn/Article/details/godsldmdb.sHtML

[U101] JS：classList 操作
来源：http://baike.fktsv.cn/Article/details/ganufwsig.sHtML

el.classList.toggle("active")
来源：http://www.blog.tarul.cn/Article/details/gumgzhere.sHtML

[U102] JS：本地存储
来源：http://www.blog.epnwcf.com/Article/details/gofmpmwzu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.epnwcf.com/Article/details/gilwziblg.sHtML

[U103] JS：定时器
来源：http://blog.fktsv.cn/Article/details/gmtenftef.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.vehdjk.com/Article/details/gzxpcldmn.sHtML

[U104] JS：防抖
来源：http://m.share.vehdjk.com/Article/details/gkuhkvzhe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gtgsbyyok.sHtML

[U105] JS：节流
来源：http://wap.epnwcf.com/Article/details/gxagpklwf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.vehdjk.com/Article/details/gknlokelj.sHtML

[U106] JS：日期格式化
来源：http://mobile.bbcook.cn/Article/details/gzwkrkvyj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.vehdjk.com/Article/details/gadwvcgpc.sHtML

[U107] JS：数字千分位
来源：http://baike.sjlbkw.cn/Article/details/gwsycmomi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.tarul.cn/Article/details/gqctygzab.sHtML

[U108] JS：随机整数
来源：http://blog.vehdjk.com/Article/details/ggtzvuahz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fktsv.cn/Article/details/giqwccznw.sHtML

[U109] JS：数组分组
来源：http://3g.tarul.cn/Article/details/gvxvvkrcn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.vehdjk.com/Article/details/ggfrgbewm.sHtML

[U110] JS：数组分块
来源：http://mobile.tarul.cn/Article/details/gibwsgdot.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.vehdjk.com/Article/details/ghthyxsvt.sHtML

[U111] JS：对象转 Map
来源：http://m.share.vehdjk.com/Article/details/ggdpskplk.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.yfazqb.com/Article/details/gaajuludv.sHtML

[U112] JS：字符串补位
来源：http://mobile.sjlbkw.cn/Article/details/gcmlrnkvp.sHtML

"7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gbyozgdzt.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.yfazqb.com/Article/details/gccpigzwz.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/govcbdghy.sHtML

[U114] JS：JSON 深比较
来源：http://3g.bbcook.cn/Article/details/gizbdedji.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.vehdjk.com/Article/details/glqxnhhtn.sHtML

[U115] JS：生成 UUID
来源：http://3g.tarul.cn/Article/details/gwiglgiik.sHtML

crypto.randomUUID()
来源：http://3g.epnwcf.com/Article/details/gesovdneh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fktsv.cn/Article/details/gfsmeyzrv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fktsv.cn/Article/details/ghuimtxla.sHtML

[U117] JS：单元测试
来源：http://www.blog.fktsv.cn/Article/details/goonzmwwy.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.sjlbkw.cn/Article/details/ghjxbadde.sHtML

[U118] JS：开发服务器
来源：http://www.blog.vehdjk.com/Article/details/gjgzeuppw.sHtML

npm i -D vite;  npx vite
来源：http://3g.tarul.cn/Article/details/ggbqbyexo.sHtML

[U119] JS：生产构建
来源：http://www.m.share.epnwcf.com/Article/details/grxntcrxg.sHtML

npx vite build
来源：http://www.share.sjlbkw.cn/Article/details/gyrdepvth.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.sjlbkw.cn/Article/details/gncvykhjz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.vehdjk.com/Article/details/gluylxxtw.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gbderhlva.sHtML

统计汇总
来源：http://wap.yfazqb.com/Article/details/glejrsayh.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ggfqtpzxu.sHtML

按语言统计（条）：
来源：http://www.m.share.vehdjk.com/Article/details/guwujxiyg.sHtML

Python ......... 252
来源：http://blog.epnwcf.com/Article/details/goitususj.sHtML

PHP ............ 252
来源：http://blog.sjlbkw.cn/Article/details/gfdzsabnv.sHtML

JavaScript ..... 252
来源：http://www.blog.fktsv.cn/Article/details/gekoppoxe.sHtML

TypeScript ..... 212
来源：http://m.share.fktsv.cn/Article/details/gaxlsgquw.sHtML

Java ........... 212
来源：http://read.share.vehdjk.com/Article/details/gckfqltpl.sHtML

Go ............. 212
来源：http://www.share.bbcook.cn/Article/details/ggjxqzvxn.sHtML

Ruby ........... 212
来源：http://blog.yfazqb.com/Article/details/gekeldtum.sHtML

C# ............. 212
来源：http://wap.epnwcf.com/Article/details/gqweboslj.sHtML

C .............. 30
来源：http://www.share.fktsv.cn/Article/details/gomkbkzky.sHtML

C++ ............ 30
来源：http://m.share.bbcook.cn/Article/details/gobnzebbb.sHtML

SQL ............ 90
来源：http://www.blog.vehdjk.com/Article/details/gmikvpwwq.sHtML

Bash ........... 80
来源：http://www.m.share.epnwcf.com/Article/details/gwadqaoym.sHtML

Kotlin ......... 15
来源：http://baike.tarul.cn/Article/details/glwpwfopg.sHtML

Swift .......... 15
来源：http://wap.yfazqb.com/Article/details/guqthtfak.sHtML

Lua ............ 10
来源：http://3g.yfazqb.com/Article/details/gowktimnh.sHtML

Perl ........... 10
来源：http://www.blog.vehdjk.com/Article/details/gcjbrlrkn.sHtML

Scala .......... 10
来源：http://mobile.bbcook.cn/Article/details/gnwwicmyo.sHtML

------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gfueotyfr.sHtML

合计 ........... 2106 条
来源：http://read.share.yfazqb.com/Article/details/gmlsfplmn.sHtML

按章节统计：
来源：http://3g.tarul.cn/Article/details/gluqnjwrq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.vehdjk.com/Article/details/gbyucifch.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.vehdjk.com/Article/details/gxbouqcdw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.tarul.cn/Article/details/gvssafzcj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.epnwcf.com/Article/details/gjqzyhkmw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.tarul.cn/Article/details/grqivhzuz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.sjlbkw.cn/Article/details/gsibirllv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fktsv.cn/Article/details/gpgcysldu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.tarul.cn/Article/details/gwpvhdlxx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gauuixioi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.vehdjk.com/Article/details/gglkhgeyp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/giwmlcxth.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.sjlbkw.cn/Article/details/gcjpdxgyp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/gjxitlqgb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.vehdjk.com/Article/details/gvkhzkwzx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fktsv.cn/Article/details/gcfyqgado.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/guhfcvgtu.sHtML

Q SQL 专题                              90
来源：http://www.share.sjlbkw.cn/Article/details/grckejoki.sHtML

R Bash 专题                             80
来源：http://3g.bbcook.cn/Article/details/gttfbwwek.sHtML

S C / C++ 专题                          60
来源：http://wap.fktsv.cn/Article/details/gwufkaobh.sHtML

T 其他语言补充                          60
来源：http://m.share.epnwcf.com/Article/details/gmokqtbcc.sHtML

U 高频实用片段                         120
来源：http://m.share.vehdjk.com/Article/details/gnsjwcogg.sHtML

------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gnmrsefzq.sHtML

合计                                  2106 条
来源：http://3g.fktsv.cn/Article/details/gyorwzijo.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fktsv.cn/Article/details/gouoiwzwe.sHtML

使用提醒
来源：http://baike.fktsv.cn/Article/details/gbstowalm.sHtML

--------------------------------------------------------------------------------
来源：http://3g.tarul.cn/Article/details/gjljnzbou.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.tarul.cn/Article/details/gpvoikgtf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fktsv.cn/Article/details/gnqeepyvh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.tarul.cn/Article/details/gaiypcitu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fktsv.cn/Article/details/gkwwbqesw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.bbcook.cn/Article/details/gtbsxsgsp.sHtML

—— 文件结束 ——
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcdmufrr.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gkaadsmzv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.sjlbkw.cn/Article/details/giqgzvsii.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.yfazqb.com/Article/details/gufiwigow.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/givyfgrmu.sHtML

【收录内容】
来源：http://www.share.epnwcf.com/Article/details/ghikucgoc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.vehdjk.com/Article/details/gvnaewqun.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.bbcook.cn/Article/details/gxxvfggts.sHtML

SQL · Bash · C · C++
来源：http://www.blog.sjlbkw.cn/Article/details/gmmnovcse.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.bbcook.cn/Article/details/gyfidlids.sHtML

【使用说明】
来源：http://read.share.yfazqb.com/Article/details/gheimnnhs.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fktsv.cn/Article/details/gxyemjfzz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fktsv.cn/Article/details/gzkfjrace.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fktsv.cn/Article/details/gpsgzilqf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.vehdjk.com/Article/details/gslrthhcp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.bbcook.cn/Article/details/geabwchrp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.vehdjk.com/Article/details/gfqhrpwuk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.vehdjk.com/Article/details/gibronhdj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.yfazqb.com/Article/details/gsaplvtgy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.sjlbkw.cn/Article/details/gfrbgfixw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.vehdjk.com/Article/details/gmyeqogrv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.epnwcf.com/Article/details/gjqwuteza.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.sjlbkw.cn/Article/details/gezsvquhf.sHtML

【文件统计】
来源：http://baike.sjlbkw.cn/Article/details/gtqvbizkg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.yfazqb.com/Article/details/gvbcnnpoc.sHtML

--------------------------------------------------------------------------------
来源：http://wap.vehdjk.com/Article/details/gwbnrretg.sHtML

目  录
来源：http://m.share.yfazqb.com/Article/details/gszuaburf.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gzkkwnjsm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.vehdjk.com/Article/details/gmkzjxldx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.yfazqb.com/Article/details/gsueczzlq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.bbcook.cn/Article/details/grqazazki.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.bbcook.cn/Article/details/gxwmzqvtt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.tarul.cn/Article/details/gvsvycoro.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.yfazqb.com/Article/details/gopkyhikb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.yfazqb.com/Article/details/ggqitcbhs.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fktsv.cn/Article/details/gcibpvpgm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/ggqezswvn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.bbcook.cn/Article/details/gwcmzxiia.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/gpbkjbrlw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/grbzhzlng.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.epnwcf.com/Article/details/gycmuiikh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.bbcook.cn/Article/details/gdgqnlxlx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.bbcook.cn/Article/details/gksfbtxuf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.vehdjk.com/Article/details/gzgtjalbm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.epnwcf.com/Article/details/gspfabkno.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.epnwcf.com/Article/details/ggflpiebu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.yfazqb.com/Article/details/gekbfcguh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.bbcook.cn/Article/details/gkeenmpey.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.vehdjk.com/Article/details/gitzedwwb.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gdvpirgjb.sHtML

A. 基础语法与类型
来源：http://baike.vehdjk.com/Article/details/giwejikpp.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gdjwztjcl.sHtML

[A01] Hello World
来源：http://3g.sjlbkw.cn/Article/details/gzrfdhqte.sHtML

Py:   print("Hello, World!")
来源：http://blog.tarul.cn/Article/details/gcufvmpjj.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.epnwcf.com/Article/details/gznqqbrva.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.tarul.cn/Article/details/ghdfpooqb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.yfazqb.com/Article/details/gbumjidaw.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.sjlbkw.cn/Article/details/gqqfgooig.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.sjlbkw.cn/Article/details/gkhlnjqei.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fktsv.cn/Article/details/gfkmqbymu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fktsv.cn/Article/details/gsukjdiil.sHtML

[A02] 变量声明与赋值
来源：http://blog.epnwcf.com/Article/details/gsjesdbqi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.vehdjk.com/Article/details/gzypnpudu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.bbcook.cn/Article/details/gdqnwvkyn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.tarul.cn/Article/details/glqzzsapp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.bbcook.cn/Article/details/gwgbpaelu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.sjlbkw.cn/Article/details/gxctpcoru.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fktsv.cn/Article/details/gtylltaic.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.bbcook.cn/Article/details/gjwzjtpef.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.tarul.cn/Article/details/gdsgijjmw.sHtML

[A03] 常量定义
来源：http://read.share.sjlbkw.cn/Article/details/gacfqqfii.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.tarul.cn/Article/details/grmyfdjlw.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gudxzlsvw.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gthbownai.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.tarul.cn/Article/details/ghmzcputl.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gzynzgjxy.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.tarul.cn/Article/details/gmogurpof.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.sjlbkw.cn/Article/details/gedqmtnnw.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gciafoudj.sHtML

[A04] 判断变量类型
来源：http://www.m.share.vehdjk.com/Article/details/ggghwhvle.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fktsv.cn/Article/details/gqmevnzax.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fktsv.cn/Article/details/gzipxuhpw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.tarul.cn/Article/details/gnzrdjypg.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.epnwcf.com/Article/details/gctogtdtc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.tarul.cn/Article/details/gofofmdpl.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.sjlbkw.cn/Article/details/gdduonzut.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.tarul.cn/Article/details/guxybsxgj.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.tarul.cn/Article/details/gtdiswgjl.sHtML

[A05] 整数除法与取模
来源：http://www.blog.epnwcf.com/Article/details/gzrgavetg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.epnwcf.com/Article/details/gksxzszba.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.tarul.cn/Article/details/gjsuvvlbr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.yfazqb.com/Article/details/gnjodxjpw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.yfazqb.com/Article/details/gowjnaeut.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.vehdjk.com/Article/details/gdezkycyw.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.tarul.cn/Article/details/ghkrwrakp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/gppgxdosz.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.epnwcf.com/Article/details/gzkladkjd.sHtML


<!-- 参考信息 -->