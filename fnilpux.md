代发 wailian999

[U49] PHP：只读属性
来源：http://wap.vehdjk.com/Article/details/gnmduzfbi.sHtML

public readonly string $name
来源：http://wap.fktsv.cn/Article/details/gyqhtaolq.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.epnwcf.com/Article/details/giaxarlkb.sHtML

public function __construct(private int $id) {}
来源：http://read.share.tarul.cn/Article/details/gqsfsveso.sHtML

[U51] PHP：数组解构
来源：http://www.share.yfazqb.com/Article/details/gvduwnbvc.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.tarul.cn/Article/details/gdtclkrbv.sHtML

[U52] PHP：箭头函数
来源：http://blog.epnwcf.com/Article/details/gmapgiwbv.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.tarul.cn/Article/details/gyptyokaq.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fktsv.cn/Article/details/gcizsuyxy.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.bbcook.cn/Article/details/ggxbcsrmb.sHtML

[U54] PHP：空安全调用
来源：http://3g.fktsv.cn/Article/details/gefxxtznp.sHtML

$obj?->method()
来源：http://www.blog.fktsv.cn/Article/details/ggiozfhlf.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.yfazqb.com/Article/details/geiyyreox.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fktsv.cn/Article/details/gjxzlgbwk.sHtML

[U56] PHP：命名参数
来源：http://blog.vehdjk.com/Article/details/gpvezxslj.sHtML

f(a: 1, b: 2)
来源：http://3g.fktsv.cn/Article/details/gjaodjspy.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gzrvoaxoe.sHtML

"值: {$a}"
来源：http://m.share.vehdjk.com/Article/details/gmxpudveg.sHtML

[U58] PHP：数组三件套
来源：http://wap.fktsv.cn/Article/details/gvrplqpam.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fktsv.cn/Article/details/gjlcljzsh.sHtML

[U59] PHP：自定义排序
来源：http://wap.vehdjk.com/Article/details/gfaunqmbf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.vehdjk.com/Article/details/gmjbvcowk.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.yfazqb.com/Article/details/gmpbixbrw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.epnwcf.com/Article/details/gjbpyuauw.sHtML

[U61] PHP：正则
来源：http://read.share.epnwcf.com/Article/details/gjpjqdsgd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gyxyizvbb.sHtML

[U62] PHP：日期对象
来源：http://m.share.fktsv.cn/Article/details/gpjqzngph.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fktsv.cn/Article/details/gbpgjpccg.sHtML

[U63] PHP：文件读写
来源：http://mobile.vehdjk.com/Article/details/ggxywkcbd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fktsv.cn/Article/details/guianzgxa.sHtML

[U64] PHP：目录遍历
来源：http://3g.vehdjk.com/Article/details/grueerpqk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.yfazqb.com/Article/details/goubedlcx.sHtML

[U65] PHP：会话
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxgahwnk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gsuxacyzn.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fktsv.cn/Article/details/grozurmen.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.tarul.cn/Article/details/gqpyaktav.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fktsv.cn/Article/details/gqbdeonut.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.bbcook.cn/Article/details/ghmtvihtg.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.epnwcf.com/Article/details/gayhwqpnf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.bbcook.cn/Article/details/ghbxpobgw.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.vehdjk.com/Article/details/gsjvpjcct.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.epnwcf.com/Article/details/gfqiujpbs.sHtML

[U70] PHP：PDO 事务
来源：http://blog.bbcook.cn/Article/details/gufitywmq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.bbcook.cn/Article/details/gqbrlmxxk.sHtML

[U71] PHP：抛出异常
来源：http://mobile.bbcook.cn/Article/details/gnsiobqok.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.sjlbkw.cn/Article/details/gkxreyuzq.sHtML

[U72] PHP：写错误日志
来源：http://blog.fktsv.cn/Article/details/gemajkozj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.yfazqb.com/Article/details/gvcnspjhi.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.bbcook.cn/Article/details/gaphjshfe.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.bbcook.cn/Article/details/gbbnnapmj.sHtML

[U74] PHP：读取环境变量
来源：http://3g.tarul.cn/Article/details/ggnymhnxl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.vehdjk.com/Article/details/gefklrawn.sHtML

[U75] PHP：依赖注入
来源：http://wap.epnwcf.com/Article/details/glxdxsfre.sHtML

composer require psr/container
来源：http://blog.tarul.cn/Article/details/gpeydwjdn.sHtML

[U76] PHP：简单路由
来源：http://www.share.sjlbkw.cn/Article/details/ggrkujbvy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.tarul.cn/Article/details/gvhyaknsi.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.yfazqb.com/Article/details/gqgwharya.sHtML

composer require twig/twig
来源：http://wap.bbcook.cn/Article/details/gcovkypde.sHtML

[U78] PHP：单元测试
来源：http://m.share.vehdjk.com/Article/details/givrwbhzo.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fktsv.cn/Article/details/ghzrripoo.sHtML

[U79] PHP：静态分析
来源：http://baike.epnwcf.com/Article/details/giamcrgha.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.bbcook.cn/Article/details/gpmsknzxc.sHtML

[U80] PHP：代码规范修复
来源：http://blog.epnwcf.com/Article/details/gqfcqmvqb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.bbcook.cn/Article/details/gdkqqphgg.sHtML

[U81] JS：初始化项目
来源：http://mobile.fktsv.cn/Article/details/gyxkmmtlm.sHtML

npm init -y;  npm i express
来源：http://www.share.fktsv.cn/Article/details/gtcuylete.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.vehdjk.com/Article/details/ggxjsqqzr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.yfazqb.com/Article/details/gnrnxneqd.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.sjlbkw.cn/Article/details/gorgomxdi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fktsv.cn/Article/details/ggovolcyc.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.yfazqb.com/Article/details/glraoefos.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.sjlbkw.cn/Article/details/gavkkxqej.sHtML

[U85] JS：可选链
来源：http://mobile.vehdjk.com/Article/details/ghnkluztw.sHtML

a?.b?.c
来源：http://read.share.fktsv.cn/Article/details/gtgijezdn.sHtML

[U86] JS：空值合并
来源：http://baike.fktsv.cn/Article/details/ggnhzybtw.sHtML

a ?? b
来源：http://www.share.bbcook.cn/Article/details/gkcxhuclu.sHtML

[U87] JS：解构默认值
来源：http://www.blog.bbcook.cn/Article/details/ghgxucmvt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.vehdjk.com/Article/details/ggdmnyacx.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.yfazqb.com/Article/details/gkethfnij.sHtML

{ ...a, ...b }
来源：http://mobile.vehdjk.com/Article/details/gcmzgmfdv.sHtML

[U89] JS：数组去重
来源：http://www.blog.vehdjk.com/Article/details/ghczgvapt.sHtML

[...new Set(arr)]
来源：http://www.blog.epnwcf.com/Article/details/gjgksjswc.sHtML

[U90] JS：数字数组排序
来源：http://read.share.yfazqb.com/Article/details/gxjfzbzcg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fktsv.cn/Article/details/gfcmrreyw.sHtML

[U91] JS：对象键值遍历
来源：http://baike.yfazqb.com/Article/details/gxcwdqqfb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.tarul.cn/Article/details/gxqcsdwfo.sHtML

[U92] JS：深拷贝
来源：http://wap.tarul.cn/Article/details/gkhrwnrgx.sHtML

structuredClone(obj)
来源：http://3g.tarul.cn/Article/details/gwvmdyjec.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gxstpwhvq.sHtML

`共 ${n} 条`
来源：http://3g.epnwcf.com/Article/details/gluqtvdye.sHtML

[U94] JS：箭头函数
来源：http://mobile.tarul.cn/Article/details/gkjahywuf.sHtML

const double = x => x * 2;
来源：http://mobile.yfazqb.com/Article/details/gzyjafpbh.sHtML

[U95] JS：Promise 包装
来源：http://www.share.yfazqb.com/Article/details/gmjnahlwl.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.bbcook.cn/Article/details/gmaskcxjd.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fktsv.cn/Article/details/gqpobzddk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/gswvwedyn.sHtML

[U97] JS：并发请求
来源：http://read.share.epnwcf.com/Article/details/grtlxlomx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gqudyvmbj.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.bbcook.cn/Article/details/gqfffmntq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.tarul.cn/Article/details/gzskwfyxn.sHtML

[U99] JS：事件监听
来源：http://mobile.vehdjk.com/Article/details/glvacylfn.sHtML

el.addEventListener("click", e => {})
来源：http://blog.sjlbkw.cn/Article/details/gwmgkiopu.sHtML

[U100] JS：DOM 查询
来源：http://blog.fktsv.cn/Article/details/giqiwzegh.sHtML

document.querySelector(".item")
来源：http://read.share.epnwcf.com/Article/details/gtwtijpic.sHtML

[U101] JS：classList 操作
来源：http://blog.fktsv.cn/Article/details/gwarjmosg.sHtML

el.classList.toggle("active")
来源：http://blog.yfazqb.com/Article/details/gwiazufkr.sHtML

[U102] JS：本地存储
来源：http://www.share.tarul.cn/Article/details/gkneuifpz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.bbcook.cn/Article/details/gvrvpmqcg.sHtML

[U103] JS：定时器
来源：http://m.share.yfazqb.com/Article/details/ggiwggnbj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.tarul.cn/Article/details/gcbjpjdts.sHtML

[U104] JS：防抖
来源：http://www.share.sjlbkw.cn/Article/details/gldvoikkv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/gwfpcuyfy.sHtML

[U105] JS：节流
来源：http://wap.bbcook.cn/Article/details/gozxmbaok.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.tarul.cn/Article/details/gnjvsnanl.sHtML

[U106] JS：日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gkrjkrpry.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.tarul.cn/Article/details/gaedmlcrq.sHtML

[U107] JS：数字千分位
来源：http://mobile.fktsv.cn/Article/details/gdtiticdc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fktsv.cn/Article/details/gnvhqnknc.sHtML

[U108] JS：随机整数
来源：http://www.m.share.tarul.cn/Article/details/gmpwqqndi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fktsv.cn/Article/details/gycmrirvb.sHtML

[U109] JS：数组分组
来源：http://www.m.share.tarul.cn/Article/details/gssenieci.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.bbcook.cn/Article/details/gyuzyxzpt.sHtML

[U110] JS：数组分块
来源：http://3g.bbcook.cn/Article/details/gejsmlcja.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fktsv.cn/Article/details/gipizphwd.sHtML

[U111] JS：对象转 Map
来源：http://m.share.tarul.cn/Article/details/gyozfyoat.sHtML

new Map(Object.entries(obj))
来源：http://baike.fktsv.cn/Article/details/grpwyszkw.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.tarul.cn/Article/details/gllggfris.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/gppqpytrx.sHtML

[U113] JS：正则替换全部
来源：http://blog.epnwcf.com/Article/details/grkzfovct.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gzxxoerqx.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.tarul.cn/Article/details/gisobffrv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.sjlbkw.cn/Article/details/gcmbmxzfd.sHtML

[U115] JS：生成 UUID
来源：http://www.share.bbcook.cn/Article/details/gszdtyekb.sHtML

crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/gsxfiwzdl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.sjlbkw.cn/Article/details/grnthrjau.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.yfazqb.com/Article/details/gfexztmyk.sHtML

[U117] JS：单元测试
来源：http://blog.epnwcf.com/Article/details/gikjizvqv.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.sjlbkw.cn/Article/details/gavavznsm.sHtML

[U118] JS：开发服务器
来源：http://www.blog.vehdjk.com/Article/details/gknpdgjom.sHtML

npm i -D vite;  npx vite
来源：http://blog.bbcook.cn/Article/details/gyrzkbvtz.sHtML

[U119] JS：生产构建
来源：http://wap.yfazqb.com/Article/details/gmgmrzpyl.sHtML

npx vite build
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbisrdhb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.vehdjk.com/Article/details/gxdejwhdc.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.bbcook.cn/Article/details/gdkxtxpuw.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gznubpfsl.sHtML

统计汇总
来源：http://www.blog.fktsv.cn/Article/details/gwszqgfxp.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gezvagujd.sHtML

按语言统计（条）：
来源：http://baike.fktsv.cn/Article/details/gmxsjcgad.sHtML

Python ......... 252
来源：http://www.share.yfazqb.com/Article/details/gqdhgotnc.sHtML

PHP ............ 252
来源：http://m.share.yfazqb.com/Article/details/gxexevpne.sHtML

JavaScript ..... 252
来源：http://www.blog.bbcook.cn/Article/details/grdhpkejn.sHtML

TypeScript ..... 212
来源：http://baike.tarul.cn/Article/details/gcdnsfkgs.sHtML

Java ........... 212
来源：http://baike.fktsv.cn/Article/details/giyrnwphb.sHtML

Go ............. 212
来源：http://3g.sjlbkw.cn/Article/details/gmwytivvm.sHtML

Ruby ........... 212
来源：http://read.share.vehdjk.com/Article/details/gusoommng.sHtML

C# ............. 212
来源：http://www.share.yfazqb.com/Article/details/gloqvvaih.sHtML

C .............. 30
来源：http://3g.fktsv.cn/Article/details/gfnumgqsa.sHtML

C++ ............ 30
来源：http://mobile.bbcook.cn/Article/details/guuzrlito.sHtML

SQL ............ 90
来源：http://baike.sjlbkw.cn/Article/details/gnyvranmg.sHtML

Bash ........... 80
来源：http://wap.sjlbkw.cn/Article/details/gpivxtype.sHtML

Kotlin ......... 15
来源：http://3g.vehdjk.com/Article/details/gplkleoxl.sHtML

Swift .......... 15
来源：http://wap.fktsv.cn/Article/details/gngyqddax.sHtML

Lua ............ 10
来源：http://www.m.share.fktsv.cn/Article/details/gvsjcrbmi.sHtML

Perl ........... 10
来源：http://www.m.share.epnwcf.com/Article/details/geozihaqw.sHtML

Scala .......... 10
来源：http://read.share.sjlbkw.cn/Article/details/gyvlynljt.sHtML

------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gktikkstb.sHtML

合计 ........... 2106 条
来源：http://wap.tarul.cn/Article/details/geikcymut.sHtML

按章节统计：
来源：http://mobile.vehdjk.com/Article/details/gacncljns.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.tarul.cn/Article/details/glphafzds.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.sjlbkw.cn/Article/details/gojkrnctd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.epnwcf.com/Article/details/gjamyixrj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.tarul.cn/Article/details/gwymulpmj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.sjlbkw.cn/Article/details/gljahxetk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.sjlbkw.cn/Article/details/gwnhxdvvl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.tarul.cn/Article/details/ghttxydim.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.tarul.cn/Article/details/ggleuidvq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gilhbtkuq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.bbcook.cn/Article/details/gybnvmokb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/gbpynfdlh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/ggshylrld.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gfkaxsquy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.bbcook.cn/Article/details/gtqzsuyoj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fktsv.cn/Article/details/gnbyklbbj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.sjlbkw.cn/Article/details/gtswqbnim.sHtML

Q SQL 专题                              90
来源：http://blog.vehdjk.com/Article/details/glgzpplxa.sHtML

R Bash 专题                             80
来源：http://wap.bbcook.cn/Article/details/gkxhyulej.sHtML

S C / C++ 专题                          60
来源：http://3g.vehdjk.com/Article/details/ghwcnulub.sHtML

T 其他语言补充                          60
来源：http://mobile.fktsv.cn/Article/details/glcybcoje.sHtML

U 高频实用片段                         120
来源：http://www.blog.vehdjk.com/Article/details/gbqplpoew.sHtML

------------------------------------
来源：http://baike.yfazqb.com/Article/details/godausmwe.sHtML

合计                                  2106 条
来源：http://read.share.yfazqb.com/Article/details/gilibobom.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gpxjyckri.sHtML

使用提醒
来源：http://m.share.yfazqb.com/Article/details/gyggoevqv.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gnrzevuuy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.tarul.cn/Article/details/gryxbrgfz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.tarul.cn/Article/details/gghxvbqsu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.yfazqb.com/Article/details/gczycibaj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwghpyjq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.tarul.cn/Article/details/geehbdfgg.sHtML

—— 文件结束 ——
来源：http://mobile.epnwcf.com/Article/details/ggptkhsih.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gdvzhnnes.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fktsv.cn/Article/details/gqexklyqu.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.epnwcf.com/Article/details/grrfntxzz.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gjisvwqov.sHtML

【收录内容】
来源：http://www.m.share.sjlbkw.cn/Article/details/goerqckjg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.epnwcf.com/Article/details/ggujmruml.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fktsv.cn/Article/details/gbxmapogu.sHtML

SQL · Bash · C · C++
来源：http://blog.bbcook.cn/Article/details/gvcuhjpip.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.epnwcf.com/Article/details/grsngiosw.sHtML

【使用说明】
来源：http://www.blog.sjlbkw.cn/Article/details/gzushidkn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.epnwcf.com/Article/details/grvgxgais.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.sjlbkw.cn/Article/details/gprrjbmzo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.sjlbkw.cn/Article/details/gbwgsvqzk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.sjlbkw.cn/Article/details/grvzthdnp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.sjlbkw.cn/Article/details/gxezkjjlo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.yfazqb.com/Article/details/gqksadwfa.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.tarul.cn/Article/details/gtlbjrjwj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.tarul.cn/Article/details/gdgrnxzin.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.vehdjk.com/Article/details/gxwlbwvdp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.yfazqb.com/Article/details/gmeljdnlt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.yfazqb.com/Article/details/gyjiykmwn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.bbcook.cn/Article/details/gxalodgim.sHtML

【文件统计】
来源：http://baike.tarul.cn/Article/details/gaifnziuu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.epnwcf.com/Article/details/gwtgwnknl.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gynuzwkdl.sHtML

目  录
来源：http://3g.fktsv.cn/Article/details/ghtvbldur.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gxjztuztd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.tarul.cn/Article/details/gnwgvzksn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.bbcook.cn/Article/details/gitlepbvr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fktsv.cn/Article/details/gtbewqdto.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.vehdjk.com/Article/details/gdyqnslwr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fktsv.cn/Article/details/giqdmdpjg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.bbcook.cn/Article/details/grxgrurep.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fktsv.cn/Article/details/gluaqykis.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.vehdjk.com/Article/details/gqqbangvp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.tarul.cn/Article/details/ghxbionaz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.bbcook.cn/Article/details/gaatpolzt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gwdtmpzcs.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/gmiozbfqc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fktsv.cn/Article/details/gnznyyylm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.yfazqb.com/Article/details/golvogwjp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fktsv.cn/Article/details/gecthqfyf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/guxetqlam.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.sjlbkw.cn/Article/details/gatmrwmsn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.epnwcf.com/Article/details/gqwveatqx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.sjlbkw.cn/Article/details/gwsgegulz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.yfazqb.com/Article/details/gqsxpydvm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.tarul.cn/Article/details/gyjtjlnvt.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gkamjecas.sHtML

A. 基础语法与类型
来源：http://read.share.bbcook.cn/Article/details/gdtxhjoei.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gebujymxd.sHtML

[A01] Hello World
来源：http://www.blog.epnwcf.com/Article/details/ghdevmhye.sHtML

Py:   print("Hello, World!")
来源：http://read.share.sjlbkw.cn/Article/details/ggxqlowlp.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.tarul.cn/Article/details/gwfhwwxpw.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.sjlbkw.cn/Article/details/gyetbtnnr.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.epnwcf.com/Article/details/ggflhqjek.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fktsv.cn/Article/details/gmlebypzj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.yfazqb.com/Article/details/gbkfnmbev.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.sjlbkw.cn/Article/details/gzypjldro.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.vehdjk.com/Article/details/gvvevkmlq.sHtML

[A02] 变量声明与赋值
来源：http://wap.vehdjk.com/Article/details/gxvaaxdhg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.epnwcf.com/Article/details/gesssxvcr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.bbcook.cn/Article/details/gucpjesdz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.vehdjk.com/Article/details/gddrxfdxh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fktsv.cn/Article/details/gplzntvmg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gmkcylvkp.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.vehdjk.com/Article/details/gsjduwcoo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.sjlbkw.cn/Article/details/gtjrrvkse.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.sjlbkw.cn/Article/details/gtwejmlca.sHtML

[A03] 常量定义
来源：http://mobile.epnwcf.com/Article/details/gcwanapze.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fktsv.cn/Article/details/gqwzxslgf.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gakkcgvhu.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gczlupoag.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/glszwtqvh.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fktsv.cn/Article/details/gukjujazv.sHtML

Go:   const PI = 3.14159
来源：http://www.share.sjlbkw.cn/Article/details/gqsgmzxmn.sHtML

Ruby: PI = 3.14159
来源：http://m.share.vehdjk.com/Article/details/ghxagjpjy.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/ggfkatgqf.sHtML

[A04] 判断变量类型
来源：http://blog.bbcook.cn/Article/details/glxzhtbkh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.vehdjk.com/Article/details/ggbvrkozy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.vehdjk.com/Article/details/gvzyrvmet.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.epnwcf.com/Article/details/gnkklqhyd.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.sjlbkw.cn/Article/details/gipbkjqdw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.vehdjk.com/Article/details/gqbibfuxr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.vehdjk.com/Article/details/ggvhnfhnq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.tarul.cn/Article/details/gvddalwkw.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.bbcook.cn/Article/details/gwrsbmcfr.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.vehdjk.com/Article/details/gnegruosq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.bbcook.cn/Article/details/gprthyrev.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fktsv.cn/Article/details/gtbnyyepy.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/gazphxijs.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.yfazqb.com/Article/details/gennwhemj.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gtgalvrjj.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fktsv.cn/Article/details/grdxwlzrl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/guwhqjeet.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gyqqxzdxt.sHtML

[A06] 字符串转数字
来源：http://read.share.fktsv.cn/Article/details/gppvrjtwt.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.sjlbkw.cn/Article/details/gnngcajti.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.epnwcf.com/Article/details/ggbdyylaq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.tarul.cn/Article/details/gnznbwxhw.sHtML


<!-- 参考信息 -->