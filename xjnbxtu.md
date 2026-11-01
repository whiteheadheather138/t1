代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmijyiff.sHtML

namespace App\Http;
来源：http://mobile.sjlbkw.cn/Article/details/glvkaasdy.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.yfazqb.com/Article/details/gofnlxoso.sHtML

declare(strict_types=1);
来源：http://www.m.share.epnwcf.com/Article/details/gbbicjrho.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.vehdjk.com/Article/details/glmbldyjn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gawdzevzr.sHtML

[U46] PHP：可空类型
来源：http://read.share.tarul.cn/Article/details/gdbaqookg.sHtML

?string $name = null
来源：http://wap.yfazqb.com/Article/details/gohdjauyu.sHtML

[U47] PHP：联合类型
来源：http://3g.vehdjk.com/Article/details/gwszfgdvq.sHtML

int|string $id
来源：http://3g.bbcook.cn/Article/details/gzedxwlnh.sHtML

[U48] PHP：纯枚举
来源：http://m.share.epnwcf.com/Article/details/gashxchpq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.vehdjk.com/Article/details/gkgkvikuc.sHtML

[U49] PHP：只读属性
来源：http://mobile.yfazqb.com/Article/details/gexukaflm.sHtML

public readonly string $name
来源：http://read.share.vehdjk.com/Article/details/gkqrahhub.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.vehdjk.com/Article/details/gdtvrcoia.sHtML

public function __construct(private int $id) {}
来源：http://3g.fktsv.cn/Article/details/gjfrvfcvt.sHtML

[U51] PHP：数组解构
来源：http://3g.sjlbkw.cn/Article/details/gppdyuubt.sHtML

[$a, $b] = $arr;
来源：http://wap.vehdjk.com/Article/details/gccrcbdsb.sHtML

[U52] PHP：箭头函数
来源：http://baike.vehdjk.com/Article/details/giiscpevv.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.vehdjk.com/Article/details/gpmocetjt.sHtML

[U53] PHP：空合并运算符
来源：http://3g.tarul.cn/Article/details/gsnudkdcc.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fktsv.cn/Article/details/gwehpakca.sHtML

[U54] PHP：空安全调用
来源：http://blog.fktsv.cn/Article/details/guagnjels.sHtML

$obj?->method()
来源：http://3g.epnwcf.com/Article/details/gkboccftd.sHtML

[U55] PHP：match 表达式
来源：http://blog.tarul.cn/Article/details/ggvvttpko.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.yfazqb.com/Article/details/gxrdaklxd.sHtML

[U56] PHP：命名参数
来源：http://baike.vehdjk.com/Article/details/gyuttwihc.sHtML

f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gdbaoesqi.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/gmhiynnru.sHtML

"值: {$a}"
来源：http://3g.vehdjk.com/Article/details/gngepirly.sHtML

[U58] PHP：数组三件套
来源：http://3g.epnwcf.com/Article/details/gxxhlzvew.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.yfazqb.com/Article/details/guffsmzvg.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fktsv.cn/Article/details/gxbmigkos.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.bbcook.cn/Article/details/gliutqegn.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.bbcook.cn/Article/details/giqdibwov.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.vehdjk.com/Article/details/gdboudjvg.sHtML

[U61] PHP：正则
来源：http://www.share.tarul.cn/Article/details/gsvyhqihu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/gvzlydshd.sHtML

[U62] PHP：日期对象
来源：http://www.share.vehdjk.com/Article/details/gyssnkkhy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.epnwcf.com/Article/details/gijyoommr.sHtML

[U63] PHP：文件读写
来源：http://www.share.fktsv.cn/Article/details/gutzndlwi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fktsv.cn/Article/details/guernsjtt.sHtML

[U64] PHP：目录遍历
来源：http://mobile.yfazqb.com/Article/details/gorwpfxfw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.vehdjk.com/Article/details/giplyjsvg.sHtML

[U65] PHP：会话
来源：http://www.blog.sjlbkw.cn/Article/details/gllviegba.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.epnwcf.com/Article/details/gidquvpvm.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.yfazqb.com/Article/details/grhtjkamz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.bbcook.cn/Article/details/gdgxotwbf.sHtML

[U67] PHP：处理文件上传
来源：http://3g.yfazqb.com/Article/details/ghifxquai.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.tarul.cn/Article/details/gweerlncp.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.vehdjk.com/Article/details/gropymwhh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fktsv.cn/Article/details/glwqhdukp.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.yfazqb.com/Article/details/gfokumtgd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.epnwcf.com/Article/details/gqoqpaqhi.sHtML

[U70] PHP：PDO 事务
来源：http://3g.sjlbkw.cn/Article/details/gfyjdhjkc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.vehdjk.com/Article/details/gmusyvkjs.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fktsv.cn/Article/details/gcoapvfsh.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.tarul.cn/Article/details/gdaytuojl.sHtML

[U72] PHP：写错误日志
来源：http://baike.bbcook.cn/Article/details/gmgwdcusg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.tarul.cn/Article/details/gasobvriv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.sjlbkw.cn/Article/details/gipfivdzg.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.sjlbkw.cn/Article/details/giiyabhki.sHtML

[U74] PHP：读取环境变量
来源：http://baike.yfazqb.com/Article/details/gjxgiezoo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.vehdjk.com/Article/details/gxzyjypif.sHtML

[U75] PHP：依赖注入
来源：http://wap.vehdjk.com/Article/details/ggzguskpz.sHtML

composer require psr/container
来源：http://read.share.vehdjk.com/Article/details/gcoocqaeh.sHtML

[U76] PHP：简单路由
来源：http://m.share.epnwcf.com/Article/details/gkbqdfely.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.tarul.cn/Article/details/gmyqxjpaf.sHtML

[U77] PHP：模板渲染
来源：http://wap.fktsv.cn/Article/details/grfzukyrq.sHtML

composer require twig/twig
来源：http://read.share.vehdjk.com/Article/details/gaiernsxg.sHtML

[U78] PHP：单元测试
来源：http://mobile.fktsv.cn/Article/details/gmemyqzza.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.yfazqb.com/Article/details/ggxcazwof.sHtML

[U79] PHP：静态分析
来源：http://read.share.bbcook.cn/Article/details/gnzahxurn.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.epnwcf.com/Article/details/gdcwtwedw.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fktsv.cn/Article/details/genyieuac.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fktsv.cn/Article/details/gdjxlajdc.sHtML

[U81] JS：初始化项目
来源：http://www.share.bbcook.cn/Article/details/gbfbildjs.sHtML

npm init -y;  npm i express
来源：http://baike.vehdjk.com/Article/details/gynrodsvl.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.vehdjk.com/Article/details/gpbjtneuq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.vehdjk.com/Article/details/gezpumnmo.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.bbcook.cn/Article/details/gegzrldth.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.sjlbkw.cn/Article/details/gywdxjslb.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fktsv.cn/Article/details/gbpooanxo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.tarul.cn/Article/details/gktxhmoiv.sHtML

[U85] JS：可选链
来源：http://wap.fktsv.cn/Article/details/gzbkcocpd.sHtML

a?.b?.c
来源：http://wap.tarul.cn/Article/details/ghvlmtuqs.sHtML

[U86] JS：空值合并
来源：http://www.blog.tarul.cn/Article/details/gzxhoubcd.sHtML

a ?? b
来源：http://read.share.tarul.cn/Article/details/gncbdofnm.sHtML

[U87] JS：解构默认值
来源：http://baike.tarul.cn/Article/details/geldikpht.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.sjlbkw.cn/Article/details/gcbpklvam.sHtML

[U88] JS：对象展开合并
来源：http://3g.sjlbkw.cn/Article/details/gwtafcwsz.sHtML

{ ...a, ...b }
来源：http://mobile.sjlbkw.cn/Article/details/gzlkwxymy.sHtML

[U89] JS：数组去重
来源：http://www.blog.sjlbkw.cn/Article/details/gmeylxuki.sHtML

[...new Set(arr)]
来源：http://baike.epnwcf.com/Article/details/geizdppww.sHtML

[U90] JS：数字数组排序
来源：http://m.share.bbcook.cn/Article/details/gizdptfcj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/gjdkskflp.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.bbcook.cn/Article/details/golzbflhz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fktsv.cn/Article/details/glxpynwua.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gotulhdte.sHtML

structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gxckjtrut.sHtML

[U93] JS：模板字符串
来源：http://wap.vehdjk.com/Article/details/ggsrufenq.sHtML

`共 ${n} 条`
来源：http://www.m.share.bbcook.cn/Article/details/gagsfxajf.sHtML

[U94] JS：箭头函数
来源：http://mobile.tarul.cn/Article/details/gukiffgyw.sHtML

const double = x => x * 2;
来源：http://wap.vehdjk.com/Article/details/ggxltkejc.sHtML

[U95] JS：Promise 包装
来源：http://read.share.epnwcf.com/Article/details/gmnmfeyhb.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.yfazqb.com/Article/details/gtpnyfwyp.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.bbcook.cn/Article/details/gygbxtrds.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsydowncl.sHtML

[U97] JS：并发请求
来源：http://3g.yfazqb.com/Article/details/gkjryuwpl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.vehdjk.com/Article/details/gkvojyroj.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhcepaiy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.yfazqb.com/Article/details/gqiouggxl.sHtML

[U99] JS：事件监听
来源：http://baike.tarul.cn/Article/details/gylysfiep.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.bbcook.cn/Article/details/gpvlqrgin.sHtML

[U100] JS：DOM 查询
来源：http://baike.sjlbkw.cn/Article/details/giqlkxjhf.sHtML

document.querySelector(".item")
来源：http://www.share.tarul.cn/Article/details/gspwdivsp.sHtML

[U101] JS：classList 操作
来源：http://baike.tarul.cn/Article/details/gmhvckghs.sHtML

el.classList.toggle("active")
来源：http://wap.vehdjk.com/Article/details/gnbqpalrl.sHtML

[U102] JS：本地存储
来源：http://read.share.vehdjk.com/Article/details/guanyddlu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.yfazqb.com/Article/details/gqxyqwcsc.sHtML

[U103] JS：定时器
来源：http://read.share.yfazqb.com/Article/details/gqztalgfo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.tarul.cn/Article/details/gallgkkeg.sHtML

[U104] JS：防抖
来源：http://3g.epnwcf.com/Article/details/gfsfrkxbq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/ghykfjvch.sHtML

[U105] JS：节流
来源：http://baike.bbcook.cn/Article/details/glrbhfsan.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fktsv.cn/Article/details/ghtvkuyqb.sHtML

[U106] JS：日期格式化
来源：http://baike.tarul.cn/Article/details/gdxnceggl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.tarul.cn/Article/details/gbmxsyozt.sHtML

[U107] JS：数字千分位
来源：http://3g.epnwcf.com/Article/details/grmiwclbn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.yfazqb.com/Article/details/gagzoovir.sHtML

[U108] JS：随机整数
来源：http://blog.bbcook.cn/Article/details/gtmfrwwzw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.vehdjk.com/Article/details/gxokkzxxm.sHtML

[U109] JS：数组分组
来源：http://www.blog.fktsv.cn/Article/details/gvsztdyjl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.bbcook.cn/Article/details/gpvhmrcsn.sHtML

[U110] JS：数组分块
来源：http://baike.sjlbkw.cn/Article/details/gpbtizcuq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fktsv.cn/Article/details/gqoociakn.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.tarul.cn/Article/details/gxflzbwep.sHtML

new Map(Object.entries(obj))
来源：http://3g.fktsv.cn/Article/details/gexwlgoye.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fktsv.cn/Article/details/gpujdxqhe.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gplhsqyps.sHtML

[U113] JS：正则替换全部
来源：http://baike.bbcook.cn/Article/details/guhhatqff.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gykdjilav.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fktsv.cn/Article/details/gykplobmx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.epnwcf.com/Article/details/gkwipdwow.sHtML

[U115] JS：生成 UUID
来源：http://wap.sjlbkw.cn/Article/details/ghzuuqppx.sHtML

crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/geeugjmcr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.bbcook.cn/Article/details/gdbeqxavr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.yfazqb.com/Article/details/gqjkwmmzq.sHtML

[U117] JS：单元测试
来源：http://3g.tarul.cn/Article/details/gvkhnrdic.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.tarul.cn/Article/details/gprrwwxvr.sHtML

[U118] JS：开发服务器
来源：http://www.share.sjlbkw.cn/Article/details/gdzgnxcir.sHtML

npm i -D vite;  npx vite
来源：http://m.share.tarul.cn/Article/details/giblaruxu.sHtML

[U119] JS：生产构建
来源：http://3g.sjlbkw.cn/Article/details/gbrcnwgrd.sHtML

npx vite build
来源：http://www.share.bbcook.cn/Article/details/gxutaxqte.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.epnwcf.com/Article/details/gqzkpyisa.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.tarul.cn/Article/details/ggkhllaxo.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gxrlhhekn.sHtML

统计汇总
来源：http://www.share.tarul.cn/Article/details/gunrtgspg.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/guehucjlb.sHtML

按语言统计（条）：
来源：http://read.share.sjlbkw.cn/Article/details/gnjzwzaab.sHtML

Python ......... 252
来源：http://www.blog.fktsv.cn/Article/details/gphvaepgc.sHtML

PHP ............ 252
来源：http://wap.epnwcf.com/Article/details/geueiynrp.sHtML

JavaScript ..... 252
来源：http://read.share.fktsv.cn/Article/details/ggjwxnjkc.sHtML

TypeScript ..... 212
来源：http://3g.fktsv.cn/Article/details/gsgchjikt.sHtML

Java ........... 212
来源：http://baike.sjlbkw.cn/Article/details/gairczcil.sHtML

Go ............. 212
来源：http://baike.sjlbkw.cn/Article/details/gfrrsjekv.sHtML

Ruby ........... 212
来源：http://mobile.epnwcf.com/Article/details/gqevghcrh.sHtML

C# ............. 212
来源：http://www.blog.epnwcf.com/Article/details/glhmpcxyc.sHtML

C .............. 30
来源：http://www.blog.yfazqb.com/Article/details/gpjvyhrqh.sHtML

C++ ............ 30
来源：http://baike.sjlbkw.cn/Article/details/gerxpqgbi.sHtML

SQL ............ 90
来源：http://baike.vehdjk.com/Article/details/gwipdjfvl.sHtML

Bash ........... 80
来源：http://blog.fktsv.cn/Article/details/gkrkjiqzw.sHtML

Kotlin ......... 15
来源：http://read.share.yfazqb.com/Article/details/gkpxrvgdh.sHtML

Swift .......... 15
来源：http://www.share.sjlbkw.cn/Article/details/gyjigeldv.sHtML

Lua ............ 10
来源：http://www.m.share.bbcook.cn/Article/details/ghcwutxca.sHtML

Perl ........... 10
来源：http://mobile.yfazqb.com/Article/details/ghekknvfv.sHtML

Scala .......... 10
来源：http://www.m.share.bbcook.cn/Article/details/gngfkqwln.sHtML

------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gyxotptik.sHtML

合计 ........... 2106 条
来源：http://www.m.share.vehdjk.com/Article/details/gqnchzgbt.sHtML

按章节统计：
来源：http://3g.vehdjk.com/Article/details/gtnpfdabm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.vehdjk.com/Article/details/gpqvmency.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.bbcook.cn/Article/details/glejdazfb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.sjlbkw.cn/Article/details/gxochlqms.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.sjlbkw.cn/Article/details/gknwpiajv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.vehdjk.com/Article/details/gzxnrigxv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.epnwcf.com/Article/details/gkjffyrjs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.bbcook.cn/Article/details/gosxpvtdo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.vehdjk.com/Article/details/gguekjktd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gzwffwjmr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.vehdjk.com/Article/details/gtyxxuubf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gyzsyshjv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gsvjabova.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gfebqgllc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.sjlbkw.cn/Article/details/gkcjpssos.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.sjlbkw.cn/Article/details/gkuvbbbrn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/gntnqbhri.sHtML

Q SQL 专题                              90
来源：http://m.share.bbcook.cn/Article/details/gyyvvknth.sHtML

R Bash 专题                             80
来源：http://www.share.yfazqb.com/Article/details/gypdsnfvk.sHtML

S C / C++ 专题                          60
来源：http://3g.epnwcf.com/Article/details/gfhezhkmo.sHtML

T 其他语言补充                          60
来源：http://mobile.vehdjk.com/Article/details/gwepcpthf.sHtML

U 高频实用片段                         120
来源：http://baike.yfazqb.com/Article/details/gxaldlfyw.sHtML

------------------------------------
来源：http://3g.bbcook.cn/Article/details/gglirkouh.sHtML

合计                                  2106 条
来源：http://blog.sjlbkw.cn/Article/details/gvhsbcloo.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.tarul.cn/Article/details/gcsagglqt.sHtML

使用提醒
来源：http://www.share.yfazqb.com/Article/details/gkygmezqq.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/ghwzyhehx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.tarul.cn/Article/details/gkatweehx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fktsv.cn/Article/details/gjylvwepc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.bbcook.cn/Article/details/geuqhveoy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.yfazqb.com/Article/details/gczbmcdzu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.epnwcf.com/Article/details/gthntvbik.sHtML

—— 文件结束 ——
来源：http://mobile.bbcook.cn/Article/details/gwjurnvbg.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gdanzsfmx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.bbcook.cn/Article/details/gcdcgajux.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fktsv.cn/Article/details/gmodyuqgm.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/grdezdohg.sHtML

【收录内容】
来源：http://www.blog.tarul.cn/Article/details/gmgeqbkmf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fktsv.cn/Article/details/gpckdfwwv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.tarul.cn/Article/details/gdxyovrkz.sHtML

SQL · Bash · C · C++
来源：http://read.share.yfazqb.com/Article/details/gtfryacik.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.epnwcf.com/Article/details/gomzxceeb.sHtML

【使用说明】
来源：http://baike.bbcook.cn/Article/details/gjcmknjiw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmszssdk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.yfazqb.com/Article/details/gvmbouqwj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.bbcook.cn/Article/details/gyimaldbs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.epnwcf.com/Article/details/gwhoeeumj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.tarul.cn/Article/details/gleaeacod.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.bbcook.cn/Article/details/gtlnajecq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.yfazqb.com/Article/details/gwqhzwdvj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.tarul.cn/Article/details/guyzoanis.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.epnwcf.com/Article/details/giprupkpe.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fktsv.cn/Article/details/geamqgewl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.vehdjk.com/Article/details/gfsxupkfc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.yfazqb.com/Article/details/goioqovjc.sHtML

【文件统计】
来源：http://baike.epnwcf.com/Article/details/gkqyeyvpb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fktsv.cn/Article/details/geofxdzmn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/ggjpmwsmj.sHtML

目  录
来源：http://3g.tarul.cn/Article/details/ghnfcrkyi.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.tarul.cn/Article/details/gscpwmobs.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.bbcook.cn/Article/details/gvtfievsy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.bbcook.cn/Article/details/gftuifngt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.sjlbkw.cn/Article/details/gtqhkhvim.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.tarul.cn/Article/details/gxffmvpeo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.sjlbkw.cn/Article/details/giujesyhl.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.bbcook.cn/Article/details/gwtxlphfh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.tarul.cn/Article/details/gbqoicffg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.tarul.cn/Article/details/gbpnacnwk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/gmjcxtzhy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.epnwcf.com/Article/details/gexzzlvkw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.vehdjk.com/Article/details/gshxthpjo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/gnmxrbwua.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.bbcook.cn/Article/details/grvdxokqj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.vehdjk.com/Article/details/gkqzgijnf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.epnwcf.com/Article/details/gnyiunfvd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/golzbjfba.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.bbcook.cn/Article/details/gtfookgyo.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.yfazqb.com/Article/details/givmngctr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.vehdjk.com/Article/details/gsyhbgndv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.yfazqb.com/Article/details/gvaacfrte.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.vehdjk.com/Article/details/gkhjfpfil.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gfbtawlqu.sHtML

A. 基础语法与类型
来源：http://blog.tarul.cn/Article/details/gmlyeptid.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ghzypvsvk.sHtML

[A01] Hello World
来源：http://m.share.bbcook.cn/Article/details/gewbumztm.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.epnwcf.com/Article/details/gtgicjyly.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.yfazqb.com/Article/details/gojdvfvgv.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.epnwcf.com/Article/details/gmrxxuvgo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.vehdjk.com/Article/details/gmacxarmy.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.vehdjk.com/Article/details/gyuntnwci.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.epnwcf.com/Article/details/gofqcqnop.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.epnwcf.com/Article/details/gjsrsssdw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.epnwcf.com/Article/details/gzwzdoxxl.sHtML

[A02] 变量声明与赋值
来源：http://read.share.epnwcf.com/Article/details/gtubtzbdr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.sjlbkw.cn/Article/details/ggsedevlj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.epnwcf.com/Article/details/gqlvdxvnc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpunzolhs.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.vehdjk.com/Article/details/gkcdoyopi.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.yfazqb.com/Article/details/gwosoxpew.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.vehdjk.com/Article/details/gmjpmudjz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.yfazqb.com/Article/details/guyedupdg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.bbcook.cn/Article/details/gomlolmxl.sHtML

[A03] 常量定义
来源：http://m.share.tarul.cn/Article/details/gzhhyaazv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.bbcook.cn/Article/details/gbyvvdlef.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gbkgfbqqg.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gfwxayvby.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.yfazqb.com/Article/details/guggveldf.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gpmihlwtt.sHtML

Go:   const PI = 3.14159
来源：http://www.share.yfazqb.com/Article/details/goxblhvbl.sHtML

Ruby: PI = 3.14159
来源：http://wap.tarul.cn/Article/details/gwanllvoc.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gmehkupws.sHtML

[A04] 判断变量类型
来源：http://www.blog.fktsv.cn/Article/details/gmhhgxvbu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.epnwcf.com/Article/details/gybwxcoqm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.tarul.cn/Article/details/geurbqlhp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.sjlbkw.cn/Article/details/gcpssycjl.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.sjlbkw.cn/Article/details/gnnphsjfq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.tarul.cn/Article/details/garksaoko.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.yfazqb.com/Article/details/ggbfacudw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.bbcook.cn/Article/details/glzmmsgot.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fktsv.cn/Article/details/grgfdkpei.sHtML

[A05] 整数除法与取模
来源：http://wap.yfazqb.com/Article/details/gqjpffxfk.sHtML


<!-- 参考信息 -->