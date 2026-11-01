代发 wailian999

[U43] PHP：声明命名空间
来源：http://blog.bbcook.cn/Article/details/guaxxflqk.sHtML

namespace App\Http;
来源：http://blog.vehdjk.com/Article/details/gfwsmrevs.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fktsv.cn/Article/details/gcatgpvxo.sHtML

declare(strict_types=1);
来源：http://3g.epnwcf.com/Article/details/gegsqmoqz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.bbcook.cn/Article/details/gmvjrhwhy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/gmcqzsqfv.sHtML

[U46] PHP：可空类型
来源：http://www.blog.tarul.cn/Article/details/ghudfbiyy.sHtML

?string $name = null
来源：http://www.m.share.epnwcf.com/Article/details/gkjbrkimr.sHtML

[U47] PHP：联合类型
来源：http://m.share.epnwcf.com/Article/details/gvoptxxum.sHtML

int|string $id
来源：http://m.share.bbcook.cn/Article/details/gxjwmmzic.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.vehdjk.com/Article/details/gwhmjourj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.yfazqb.com/Article/details/gmxwmxney.sHtML

[U49] PHP：只读属性
来源：http://www.blog.epnwcf.com/Article/details/gaicocair.sHtML

public readonly string $name
来源：http://baike.tarul.cn/Article/details/gdyhacdtz.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.tarul.cn/Article/details/gdxhgzhni.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fktsv.cn/Article/details/gotegjdew.sHtML

[U51] PHP：数组解构
来源：http://3g.vehdjk.com/Article/details/gjzlmpxeu.sHtML

[$a, $b] = $arr;
来源：http://baike.yfazqb.com/Article/details/ghrwtikku.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.sjlbkw.cn/Article/details/gampbborq.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fktsv.cn/Article/details/gmdgjeeyk.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.vehdjk.com/Article/details/gicpksmfy.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.sjlbkw.cn/Article/details/gthurcxsw.sHtML

[U54] PHP：空安全调用
来源：http://baike.tarul.cn/Article/details/gsowqktle.sHtML

$obj?->method()
来源：http://www.blog.tarul.cn/Article/details/gwmiddtlf.sHtML

[U55] PHP：match 表达式
来源：http://blog.vehdjk.com/Article/details/gdxdfduun.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.tarul.cn/Article/details/gddyvisnp.sHtML

[U56] PHP：命名参数
来源：http://m.share.yfazqb.com/Article/details/gybyrzcqa.sHtML

f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gzgoeanpb.sHtML

[U57] PHP：字符串插值
来源：http://blog.vehdjk.com/Article/details/glfejntha.sHtML

"值: {$a}"
来源：http://mobile.vehdjk.com/Article/details/gnyajtier.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fktsv.cn/Article/details/gzrmszwlz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.yfazqb.com/Article/details/gygozthjv.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.epnwcf.com/Article/details/glrbpunjb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fktsv.cn/Article/details/gesxmgqfl.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.vehdjk.com/Article/details/gzswjuiga.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.vehdjk.com/Article/details/gnbtxyjkh.sHtML

[U61] PHP：正则
来源：http://www.blog.epnwcf.com/Article/details/gdugutwag.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gwpfhkhsz.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.bbcook.cn/Article/details/gxtubpimx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fktsv.cn/Article/details/gefebvxmq.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.tarul.cn/Article/details/gdzeyurpz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.sjlbkw.cn/Article/details/gsqldloik.sHtML

[U64] PHP：目录遍历
来源：http://m.share.sjlbkw.cn/Article/details/grikygjuq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.tarul.cn/Article/details/ghplzplte.sHtML

[U65] PHP：会话
来源：http://www.blog.sjlbkw.cn/Article/details/gedsgpzlu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvxkcqhg.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.sjlbkw.cn/Article/details/gwigvrusm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.bbcook.cn/Article/details/gqyrexpnq.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.yfazqb.com/Article/details/gmougwsqk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.bbcook.cn/Article/details/gbkyoqvbu.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.epnwcf.com/Article/details/gjxrscfao.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.sjlbkw.cn/Article/details/gwiwizhiz.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.yfazqb.com/Article/details/geoneasvx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.tarul.cn/Article/details/gwzndsyqk.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fktsv.cn/Article/details/ggkwmddst.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.vehdjk.com/Article/details/gscvahngf.sHtML

[U71] PHP：抛出异常
来源：http://3g.epnwcf.com/Article/details/gtbrexzkw.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.vehdjk.com/Article/details/ghuzglvax.sHtML

[U72] PHP：写错误日志
来源：http://mobile.tarul.cn/Article/details/gartrggic.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.bbcook.cn/Article/details/gcfuwwbhm.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.epnwcf.com/Article/details/gppijtdtk.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.yfazqb.com/Article/details/ggtvcfqua.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/ghyjbtyua.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.epnwcf.com/Article/details/gbuybhske.sHtML

[U75] PHP：依赖注入
来源：http://mobile.sjlbkw.cn/Article/details/gvtbpwusa.sHtML

composer require psr/container
来源：http://blog.tarul.cn/Article/details/gyxwcwycz.sHtML

[U76] PHP：简单路由
来源：http://mobile.sjlbkw.cn/Article/details/giaaitflw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fktsv.cn/Article/details/gwlktsjpn.sHtML

[U77] PHP：模板渲染
来源：http://blog.epnwcf.com/Article/details/geersrixy.sHtML

composer require twig/twig
来源：http://wap.bbcook.cn/Article/details/gelcaqspc.sHtML

[U78] PHP：单元测试
来源：http://www.share.vehdjk.com/Article/details/grxzfkxmk.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.bbcook.cn/Article/details/glhdjpucb.sHtML

[U79] PHP：静态分析
来源：http://read.share.yfazqb.com/Article/details/glqatqmvh.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.epnwcf.com/Article/details/glpybjppu.sHtML

[U80] PHP：代码规范修复
来源：http://baike.tarul.cn/Article/details/gklharruj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.yfazqb.com/Article/details/gcinomwwe.sHtML

[U81] JS：初始化项目
来源：http://read.share.tarul.cn/Article/details/grquoknfy.sHtML

npm init -y;  npm i express
来源：http://wap.sjlbkw.cn/Article/details/gcqrswcgo.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.tarul.cn/Article/details/gzrhwajki.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.vehdjk.com/Article/details/gvymzwohp.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.vehdjk.com/Article/details/gblatpmly.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.vehdjk.com/Article/details/gfitzvfbw.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.vehdjk.com/Article/details/gvgkbfhaw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.epnwcf.com/Article/details/gnpnbjrxw.sHtML

[U85] JS：可选链
来源：http://read.share.yfazqb.com/Article/details/gwmabmzkx.sHtML

a?.b?.c
来源：http://baike.bbcook.cn/Article/details/gtiavdela.sHtML

[U86] JS：空值合并
来源：http://www.blog.epnwcf.com/Article/details/gcowkxpya.sHtML

a ?? b
来源：http://baike.yfazqb.com/Article/details/gefcujcvl.sHtML

[U87] JS：解构默认值
来源：http://baike.epnwcf.com/Article/details/gcjmjzhil.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.bbcook.cn/Article/details/gveltpcpt.sHtML

[U88] JS：对象展开合并
来源：http://baike.epnwcf.com/Article/details/gggdhemvo.sHtML

{ ...a, ...b }
来源：http://read.share.yfazqb.com/Article/details/ghwrcbkeo.sHtML

[U89] JS：数组去重
来源：http://read.share.tarul.cn/Article/details/gelmmtokw.sHtML

[...new Set(arr)]
来源：http://www.m.share.fktsv.cn/Article/details/gndbtgucf.sHtML

[U90] JS：数字数组排序
来源：http://mobile.bbcook.cn/Article/details/ggalhclmd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fktsv.cn/Article/details/gbqyvrczr.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.bbcook.cn/Article/details/gnovujtmi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.epnwcf.com/Article/details/gqdzfkmwv.sHtML

[U92] JS：深拷贝
来源：http://www.blog.bbcook.cn/Article/details/gmyrzlzmb.sHtML

structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gbammciti.sHtML

[U93] JS：模板字符串
来源：http://wap.tarul.cn/Article/details/gjbhesnuk.sHtML

`共 ${n} 条`
来源：http://blog.yfazqb.com/Article/details/gtvemuclf.sHtML

[U94] JS：箭头函数
来源：http://blog.sjlbkw.cn/Article/details/gbwdudfzb.sHtML

const double = x => x * 2;
来源：http://mobile.tarul.cn/Article/details/gyzvjfvrs.sHtML

[U95] JS：Promise 包装
来源：http://baike.vehdjk.com/Article/details/gacvodmnz.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fktsv.cn/Article/details/glmwuxevv.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.epnwcf.com/Article/details/gaisbgdeh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gkfcqcynx.sHtML

[U97] JS：并发请求
来源：http://mobile.fktsv.cn/Article/details/gyjdfwnyc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/gaecppkbe.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.epnwcf.com/Article/details/geuajtqya.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.vehdjk.com/Article/details/gdjnmxoor.sHtML

[U99] JS：事件监听
来源：http://3g.sjlbkw.cn/Article/details/guttbjcfq.sHtML

el.addEventListener("click", e => {})
来源：http://baike.bbcook.cn/Article/details/gjskftqix.sHtML

[U100] JS：DOM 查询
来源：http://m.share.yfazqb.com/Article/details/gusrwtofo.sHtML

document.querySelector(".item")
来源：http://wap.epnwcf.com/Article/details/gshqlfdwb.sHtML

[U101] JS：classList 操作
来源：http://mobile.sjlbkw.cn/Article/details/gvhbivcal.sHtML

el.classList.toggle("active")
来源：http://mobile.fktsv.cn/Article/details/ggutvksdj.sHtML

[U102] JS：本地存储
来源：http://www.blog.tarul.cn/Article/details/gvwguybny.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.bbcook.cn/Article/details/grdvtbrja.sHtML

[U103] JS：定时器
来源：http://wap.tarul.cn/Article/details/gxzbyesoy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.vehdjk.com/Article/details/gnppqdxju.sHtML

[U104] JS：防抖
来源：http://m.share.sjlbkw.cn/Article/details/geqhjuglx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.bbcook.cn/Article/details/gabxucwov.sHtML

[U105] JS：节流
来源：http://www.blog.bbcook.cn/Article/details/gsrjgzryt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.epnwcf.com/Article/details/gfsbtyqat.sHtML

[U106] JS：日期格式化
来源：http://www.blog.bbcook.cn/Article/details/gdnmiqvvz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.sjlbkw.cn/Article/details/glcvbljeh.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.tarul.cn/Article/details/glemkzerm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.sjlbkw.cn/Article/details/gdfbkdufh.sHtML

[U108] JS：随机整数
来源：http://wap.vehdjk.com/Article/details/gslrebcxw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.sjlbkw.cn/Article/details/gpgepwakh.sHtML

[U109] JS：数组分组
来源：http://www.blog.bbcook.cn/Article/details/gqqtitmit.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.tarul.cn/Article/details/gzbeuqycy.sHtML

[U110] JS：数组分块
来源：http://mobile.vehdjk.com/Article/details/gkkdlsxeq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.tarul.cn/Article/details/gwmitmlib.sHtML

[U111] JS：对象转 Map
来源：http://blog.yfazqb.com/Article/details/gwcebqxpn.sHtML

new Map(Object.entries(obj))
来源：http://blog.tarul.cn/Article/details/gdnybfcth.sHtML

[U112] JS：字符串补位
来源：http://baike.vehdjk.com/Article/details/gqsyfszdz.sHtML

"7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gbybedhpw.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.bbcook.cn/Article/details/ghmomsrfd.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gwcojacqs.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fktsv.cn/Article/details/gifrjfhql.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.vehdjk.com/Article/details/gcloimwft.sHtML

[U115] JS：生成 UUID
来源：http://baike.vehdjk.com/Article/details/gihqdtfma.sHtML

crypto.randomUUID()
来源：http://mobile.yfazqb.com/Article/details/gksrtauho.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.bbcook.cn/Article/details/gepwsupdz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.bbcook.cn/Article/details/gejojkpej.sHtML

[U117] JS：单元测试
来源：http://blog.fktsv.cn/Article/details/gsdenexwe.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.epnwcf.com/Article/details/gopxgmknc.sHtML

[U118] JS：开发服务器
来源：http://read.share.sjlbkw.cn/Article/details/gsajdxeud.sHtML

npm i -D vite;  npx vite
来源：http://baike.tarul.cn/Article/details/gguqxmddr.sHtML

[U119] JS：生产构建
来源：http://m.share.tarul.cn/Article/details/gagmynwib.sHtML

npx vite build
来源：http://www.m.share.vehdjk.com/Article/details/grwlqupoc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.yfazqb.com/Article/details/gushzlvmt.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.tarul.cn/Article/details/gsdnnkvyn.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/geobidxas.sHtML

统计汇总
来源：http://blog.bbcook.cn/Article/details/gaxvxuadj.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gmtysgcvo.sHtML

按语言统计（条）：
来源：http://www.blog.vehdjk.com/Article/details/gkdduadyz.sHtML

Python ......... 252
来源：http://baike.tarul.cn/Article/details/gotqzhabz.sHtML

PHP ............ 252
来源：http://www.blog.fktsv.cn/Article/details/giywbkmln.sHtML

JavaScript ..... 252
来源：http://www.share.epnwcf.com/Article/details/grszcqobw.sHtML

TypeScript ..... 212
来源：http://www.share.tarul.cn/Article/details/giskduage.sHtML

Java ........... 212
来源：http://www.m.share.tarul.cn/Article/details/gmofopwvr.sHtML

Go ............. 212
来源：http://wap.vehdjk.com/Article/details/gkissdddo.sHtML

Ruby ........... 212
来源：http://3g.tarul.cn/Article/details/gqlbszeum.sHtML

C# ............. 212
来源：http://wap.yfazqb.com/Article/details/ggnuquobv.sHtML

C .............. 30
来源：http://m.share.vehdjk.com/Article/details/gxhekivsl.sHtML

C++ ............ 30
来源：http://www.blog.vehdjk.com/Article/details/gufravlss.sHtML

SQL ............ 90
来源：http://read.share.yfazqb.com/Article/details/gysupuvph.sHtML

Bash ........... 80
来源：http://www.blog.yfazqb.com/Article/details/gedliihdo.sHtML

Kotlin ......... 15
来源：http://www.m.share.epnwcf.com/Article/details/gryjepckh.sHtML

Swift .......... 15
来源：http://www.share.bbcook.cn/Article/details/ganyddtce.sHtML

Lua ............ 10
来源：http://www.m.share.sjlbkw.cn/Article/details/gerlfemit.sHtML

Perl ........... 10
来源：http://m.share.tarul.cn/Article/details/gxitbzzmw.sHtML

Scala .......... 10
来源：http://www.share.tarul.cn/Article/details/gykowjldt.sHtML

------------------------------------
来源：http://baike.bbcook.cn/Article/details/glvpwfyzc.sHtML

合计 ........... 2106 条
来源：http://read.share.fktsv.cn/Article/details/gqgrxdxop.sHtML

按章节统计：
来源：http://www.share.yfazqb.com/Article/details/glaqijfso.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.epnwcf.com/Article/details/goennvfvw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.tarul.cn/Article/details/gfcicdzgv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.epnwcf.com/Article/details/gakzdwmqh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.yfazqb.com/Article/details/gvltidwlp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.epnwcf.com/Article/details/gcdpsjqpv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.yfazqb.com/Article/details/gqalsrbld.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.vehdjk.com/Article/details/ghxphhkin.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.sjlbkw.cn/Article/details/gfpyscwhb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gglfqqcou.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fktsv.cn/Article/details/gwxczhfdc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/geanmpkpz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gctyybdgj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gsnpblcld.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.vehdjk.com/Article/details/gufrugljb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.tarul.cn/Article/details/gfdmcbqrg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/gjmlhtcob.sHtML

Q SQL 专题                              90
来源：http://baike.tarul.cn/Article/details/gnigyfjvv.sHtML

R Bash 专题                             80
来源：http://3g.tarul.cn/Article/details/gmmtmjoeo.sHtML

S C / C++ 专题                          60
来源：http://www.blog.epnwcf.com/Article/details/gzikqeaau.sHtML

T 其他语言补充                          60
来源：http://wap.bbcook.cn/Article/details/gjcoysvhh.sHtML

U 高频实用片段                         120
来源：http://3g.tarul.cn/Article/details/gmbwnldip.sHtML

------------------------------------
来源：http://baike.vehdjk.com/Article/details/gxqncbyka.sHtML

合计                                  2106 条
来源：http://baike.epnwcf.com/Article/details/ggkkywxhr.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/gkxorbnwx.sHtML

使用提醒
来源：http://baike.sjlbkw.cn/Article/details/gnrdcytxk.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.epnwcf.com/Article/details/gsxvsttwj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.sjlbkw.cn/Article/details/gppbaaznk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.sjlbkw.cn/Article/details/grnzdjlig.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.sjlbkw.cn/Article/details/gmqbupdyy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.sjlbkw.cn/Article/details/gabbdicml.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.sjlbkw.cn/Article/details/gigffxcxh.sHtML

—— 文件结束 ——
来源：http://m.share.tarul.cn/Article/details/gbhpusuif.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gckgdyvhb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.bbcook.cn/Article/details/gzrcudwwp.sHtML

Common Programming Examples Cheat Book
来源：http://wap.epnwcf.com/Article/details/gplyjxkbl.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gbmqyumkp.sHtML

【收录内容】
来源：http://www.share.yfazqb.com/Article/details/ghzqwfdhd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fktsv.cn/Article/details/guzuishli.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.sjlbkw.cn/Article/details/gsdzcygus.sHtML

SQL · Bash · C · C++
来源：http://read.share.yfazqb.com/Article/details/gofghrbre.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.sjlbkw.cn/Article/details/gearunduo.sHtML

【使用说明】
来源：http://www.share.sjlbkw.cn/Article/details/glvgkwzfh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.tarul.cn/Article/details/gpbdgqbhj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fktsv.cn/Article/details/gjaczfagu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.epnwcf.com/Article/details/gznajhqez.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.vehdjk.com/Article/details/gixwpabyp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.yfazqb.com/Article/details/ggedylerj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.bbcook.cn/Article/details/gohvkonyp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.sjlbkw.cn/Article/details/ghvruakvp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.epnwcf.com/Article/details/gvuehjpcl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.bbcook.cn/Article/details/gkxytnvfd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.yfazqb.com/Article/details/gulirtidy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.vehdjk.com/Article/details/gwelvtyqb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fktsv.cn/Article/details/ghcjbnqte.sHtML

【文件统计】
来源：http://mobile.fktsv.cn/Article/details/gsgiyhmqn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.yfazqb.com/Article/details/gxrlhlado.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/guhbxfppp.sHtML

目  录
来源：http://www.blog.fktsv.cn/Article/details/gbjxzucgv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gilhhlvsu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.tarul.cn/Article/details/gqnbmllub.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fktsv.cn/Article/details/gpcalxcmz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.epnwcf.com/Article/details/gpecpaume.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.tarul.cn/Article/details/ghsmhtzql.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.bbcook.cn/Article/details/gdfvymstu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.epnwcf.com/Article/details/gnoacrxqg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.sjlbkw.cn/Article/details/gmjrwezhv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fktsv.cn/Article/details/gdmvpjosp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gtkfmtmgl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.vehdjk.com/Article/details/gsjsmozmc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/gigufuran.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.bbcook.cn/Article/details/gwnkzayfc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.bbcook.cn/Article/details/gbumhbgeg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.bbcook.cn/Article/details/gfpqogvay.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fktsv.cn/Article/details/gmnfdhond.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.vehdjk.com/Article/details/gvavatuxj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.bbcook.cn/Article/details/gsflybpzv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.epnwcf.com/Article/details/ggvnjxwjg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.bbcook.cn/Article/details/gqdgosuqa.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.bbcook.cn/Article/details/guspcofzc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.yfazqb.com/Article/details/glewlslmb.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzmnppgsf.sHtML

A. 基础语法与类型
来源：http://www.blog.epnwcf.com/Article/details/gduoywjhy.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gwqjybjbb.sHtML

[A01] Hello World
来源：http://m.share.epnwcf.com/Article/details/gkogicrgn.sHtML

Py:   print("Hello, World!")
来源：http://m.share.yfazqb.com/Article/details/gddrubeeo.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.bbcook.cn/Article/details/gskwjsodk.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fktsv.cn/Article/details/gyiwdqlzc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.sjlbkw.cn/Article/details/gwqdktpvy.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.tarul.cn/Article/details/gpigjzbtn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.yfazqb.com/Article/details/gdaagjvqm.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.bbcook.cn/Article/details/gzutxoles.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.bbcook.cn/Article/details/gguthrmiq.sHtML

[A02] 变量声明与赋值
来源：http://www.share.bbcook.cn/Article/details/gdwmzejoj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.sjlbkw.cn/Article/details/gielkvnht.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.yfazqb.com/Article/details/gtuhbktnm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.sjlbkw.cn/Article/details/ggidfjiqc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.epnwcf.com/Article/details/gzmyfersa.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.tarul.cn/Article/details/gxteneshj.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.vehdjk.com/Article/details/gkxpztlhm.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.epnwcf.com/Article/details/gwrisxoop.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.sjlbkw.cn/Article/details/gdgmmrmaq.sHtML

[A03] 常量定义
来源：http://read.share.fktsv.cn/Article/details/gzkapawdk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.bbcook.cn/Article/details/genubrybc.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gcllnfioh.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/ghiicrhdw.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gkflwddil.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gvctldwbv.sHtML

Go:   const PI = 3.14159
来源：http://baike.epnwcf.com/Article/details/gfwsxeogl.sHtML

Ruby: PI = 3.14159
来源：http://baike.sjlbkw.cn/Article/details/gmtgyfhta.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gskbymigm.sHtML

[A04] 判断变量类型
来源：http://3g.yfazqb.com/Article/details/gkruoyept.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fktsv.cn/Article/details/gfbefwzoj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.tarul.cn/Article/details/gqbqafrcb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.vehdjk.com/Article/details/ghwuuvvak.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fktsv.cn/Article/details/gfuggtrzc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fktsv.cn/Article/details/gvvtpoxzn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.yfazqb.com/Article/details/gqizlcarg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.tarul.cn/Article/details/ghcwmlyqy.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.epnwcf.com/Article/details/ghooddnsj.sHtML

[A05] 整数除法与取模
来源：http://blog.yfazqb.com/Article/details/gqvszrrxs.sHtML


<!-- 参考信息 -->