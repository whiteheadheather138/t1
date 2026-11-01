代发 wailian999

[U47] PHP：联合类型
来源：http://www.m.share.vehdjk.com/Article/details/gkeqxvwzx.sHtML

int|string $id
来源：http://www.blog.vehdjk.com/Article/details/gwousxcom.sHtML

[U48] PHP：纯枚举
来源：http://wap.bbcook.cn/Article/details/gaxuehuxw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.tarul.cn/Article/details/girccjyom.sHtML

[U49] PHP：只读属性
来源：http://www.blog.sjlbkw.cn/Article/details/gyneprycn.sHtML

public readonly string $name
来源：http://baike.epnwcf.com/Article/details/gziyegrgp.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fktsv.cn/Article/details/gfeskpxgo.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.vehdjk.com/Article/details/gsrzktvaw.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.yfazqb.com/Article/details/gmbskitse.sHtML

[$a, $b] = $arr;
来源：http://blog.fktsv.cn/Article/details/gmfggbdjp.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.tarul.cn/Article/details/gmgpsfwux.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fktsv.cn/Article/details/gwcwsdurr.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.vehdjk.com/Article/details/gtdzyzlpo.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.bbcook.cn/Article/details/gkqjfyvaq.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.tarul.cn/Article/details/gawwrgipm.sHtML

$obj?->method()
来源：http://www.share.bbcook.cn/Article/details/gwlpgoduv.sHtML

[U55] PHP：match 表达式
来源：http://baike.vehdjk.com/Article/details/gbntcmmws.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.vehdjk.com/Article/details/gbouytvhd.sHtML

[U56] PHP：命名参数
来源：http://baike.epnwcf.com/Article/details/gmydkufww.sHtML

f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gdtaubpng.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/ghhhlpdmu.sHtML

"值: {$a}"
来源：http://m.share.epnwcf.com/Article/details/gqxnkizxr.sHtML

[U58] PHP：数组三件套
来源：http://m.share.bbcook.cn/Article/details/ggtcdbthv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.sjlbkw.cn/Article/details/glfewrfyt.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.yfazqb.com/Article/details/gkpigdccv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.vehdjk.com/Article/details/gmywjximj.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.epnwcf.com/Article/details/gkdesmkpk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fktsv.cn/Article/details/ghhbmmgtc.sHtML

[U61] PHP：正则
来源：http://m.share.sjlbkw.cn/Article/details/gudsljubd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fktsv.cn/Article/details/gmtzjxwek.sHtML

[U62] PHP：日期对象
来源：http://baike.yfazqb.com/Article/details/gkehysqvj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fktsv.cn/Article/details/gpwaydqhz.sHtML

[U63] PHP：文件读写
来源：http://www.blog.bbcook.cn/Article/details/gdvqjvczh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.vehdjk.com/Article/details/gsxazjida.sHtML

[U64] PHP：目录遍历
来源：http://www.share.sjlbkw.cn/Article/details/gtcjcjxzn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.epnwcf.com/Article/details/gjqbndipq.sHtML

[U65] PHP：会话
来源：http://mobile.tarul.cn/Article/details/gtvgmgsiy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/ghruasgwm.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fktsv.cn/Article/details/gmdzvoeui.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.sjlbkw.cn/Article/details/giaibreul.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.tarul.cn/Article/details/gqoazzbtz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.tarul.cn/Article/details/groeqdgfi.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fktsv.cn/Article/details/glfdadwve.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fktsv.cn/Article/details/gujldckfk.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.bbcook.cn/Article/details/grtppgunp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.yfazqb.com/Article/details/gipujwflp.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.epnwcf.com/Article/details/gibrfymvc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.yfazqb.com/Article/details/gsbithuju.sHtML

[U71] PHP：抛出异常
来源：http://3g.fktsv.cn/Article/details/gyjsinlkz.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fktsv.cn/Article/details/ghdahwfkk.sHtML

[U72] PHP：写错误日志
来源：http://wap.vehdjk.com/Article/details/gsaumhkju.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.tarul.cn/Article/details/gdchtymqk.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.sjlbkw.cn/Article/details/gvpnvbaji.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fktsv.cn/Article/details/gycolvaez.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.bbcook.cn/Article/details/gergzijen.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.sjlbkw.cn/Article/details/gncbyexoe.sHtML

[U75] PHP：依赖注入
来源：http://3g.vehdjk.com/Article/details/gpidwmwdx.sHtML

composer require psr/container
来源：http://www.blog.sjlbkw.cn/Article/details/gfaprrmeu.sHtML

[U76] PHP：简单路由
来源：http://blog.yfazqb.com/Article/details/gazptrunj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fktsv.cn/Article/details/gvmrhkphh.sHtML

[U77] PHP：模板渲染
来源：http://3g.fktsv.cn/Article/details/glpqxrmlw.sHtML

composer require twig/twig
来源：http://m.share.epnwcf.com/Article/details/gglkyzzip.sHtML

[U78] PHP：单元测试
来源：http://www.share.tarul.cn/Article/details/gcivqcybc.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.vehdjk.com/Article/details/gbkmubvch.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.sjlbkw.cn/Article/details/gngdqciro.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.yfazqb.com/Article/details/gqtjgnqvi.sHtML

[U80] PHP：代码规范修复
来源：http://blog.yfazqb.com/Article/details/grgqivblh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.sjlbkw.cn/Article/details/gxasejmqj.sHtML

[U81] JS：初始化项目
来源：http://3g.bbcook.cn/Article/details/gmalqcocy.sHtML

npm init -y;  npm i express
来源：http://www.m.share.yfazqb.com/Article/details/grwzjvbrk.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.tarul.cn/Article/details/gocqhwfju.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.sjlbkw.cn/Article/details/gxvwxjnel.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.bbcook.cn/Article/details/gmtgdcvwg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.epnwcf.com/Article/details/gzmpdyfep.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fktsv.cn/Article/details/gopuihbze.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.sjlbkw.cn/Article/details/gouhnoezo.sHtML

[U85] JS：可选链
来源：http://m.share.bbcook.cn/Article/details/gsnfqdvda.sHtML

a?.b?.c
来源：http://baike.tarul.cn/Article/details/gudxxujny.sHtML

[U86] JS：空值合并
来源：http://blog.epnwcf.com/Article/details/gxbievuuo.sHtML

a ?? b
来源：http://www.share.epnwcf.com/Article/details/gefecaqqy.sHtML

[U87] JS：解构默认值
来源：http://www.share.vehdjk.com/Article/details/gwzgmpkkq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fktsv.cn/Article/details/ggczcpydy.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fktsv.cn/Article/details/gldsckrhs.sHtML

{ ...a, ...b }
来源：http://blog.bbcook.cn/Article/details/gsfbodvsb.sHtML

[U89] JS：数组去重
来源：http://read.share.vehdjk.com/Article/details/goznhwmfr.sHtML

[...new Set(arr)]
来源：http://www.blog.epnwcf.com/Article/details/gkffpjdme.sHtML

[U90] JS：数字数组排序
来源：http://www.share.tarul.cn/Article/details/gnskcilqo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/gmzxaeqhs.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fktsv.cn/Article/details/gasqsylis.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.epnwcf.com/Article/details/gasveuplm.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gdhjrhuep.sHtML

structuredClone(obj)
来源：http://mobile.tarul.cn/Article/details/gkyrjousq.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.vehdjk.com/Article/details/gqctrdmie.sHtML

`共 ${n} 条`
来源：http://wap.epnwcf.com/Article/details/gbtibvosk.sHtML

[U94] JS：箭头函数
来源：http://read.share.epnwcf.com/Article/details/gcidarxmt.sHtML

const double = x => x * 2;
来源：http://www.share.sjlbkw.cn/Article/details/gscxgafed.sHtML

[U95] JS：Promise 包装
来源：http://wap.sjlbkw.cn/Article/details/gedcigshw.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.epnwcf.com/Article/details/gmlxajgqa.sHtML

[U96] JS：async/await 与异常
来源：http://baike.bbcook.cn/Article/details/gaqhbzmgq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/gtyebqvgs.sHtML

[U97] JS：并发请求
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvieffpt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gezyizfjq.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.bbcook.cn/Article/details/gmwvvfsdd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.yfazqb.com/Article/details/greojkmkm.sHtML

[U99] JS：事件监听
来源：http://mobile.epnwcf.com/Article/details/gtbnvjokc.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.bbcook.cn/Article/details/gedampklp.sHtML

[U100] JS：DOM 查询
来源：http://www.share.yfazqb.com/Article/details/gruupsqie.sHtML

document.querySelector(".item")
来源：http://blog.yfazqb.com/Article/details/gdrvrplcv.sHtML

[U101] JS：classList 操作
来源：http://www.share.fktsv.cn/Article/details/gfjcxaxvg.sHtML

el.classList.toggle("active")
来源：http://wap.sjlbkw.cn/Article/details/gzfpbhqvt.sHtML

[U102] JS：本地存储
来源：http://wap.vehdjk.com/Article/details/gccdnfwmv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.vehdjk.com/Article/details/gmoasifkx.sHtML

[U103] JS：定时器
来源：http://read.share.fktsv.cn/Article/details/gdgcejlfg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.bbcook.cn/Article/details/gwyhibywa.sHtML

[U104] JS：防抖
来源：http://baike.yfazqb.com/Article/details/gfjhzmqki.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fktsv.cn/Article/details/gtejoersd.sHtML

[U105] JS：节流
来源：http://3g.epnwcf.com/Article/details/gqjclmtkx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.vehdjk.com/Article/details/gawcbtqjg.sHtML

[U106] JS：日期格式化
来源：http://blog.tarul.cn/Article/details/gcdsbtzih.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.tarul.cn/Article/details/gkyomeapq.sHtML

[U107] JS：数字千分位
来源：http://blog.fktsv.cn/Article/details/ghrqfuwpw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.bbcook.cn/Article/details/gqspzrxhg.sHtML

[U108] JS：随机整数
来源：http://3g.fktsv.cn/Article/details/gosahdjdn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.tarul.cn/Article/details/gnvbwrddw.sHtML

[U109] JS：数组分组
来源：http://baike.yfazqb.com/Article/details/ghswoztes.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.yfazqb.com/Article/details/gtxzicspg.sHtML

[U110] JS：数组分块
来源：http://www.share.vehdjk.com/Article/details/girxwjzgn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.sjlbkw.cn/Article/details/gfzwvtrar.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.bbcook.cn/Article/details/gyntstfnt.sHtML

new Map(Object.entries(obj))
来源：http://read.share.sjlbkw.cn/Article/details/gmpwhelwh.sHtML

[U112] JS：字符串补位
来源：http://baike.epnwcf.com/Article/details/gupnpiozh.sHtML

"7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gpxprgtby.sHtML

[U113] JS：正则替换全部
来源：http://mobile.epnwcf.com/Article/details/gsdaihlqv.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gezdhuywm.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.bbcook.cn/Article/details/gilqizrsk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fktsv.cn/Article/details/gruorkugl.sHtML

[U115] JS：生成 UUID
来源：http://m.share.epnwcf.com/Article/details/gsravlbia.sHtML

crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/gpqydiqvk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.sjlbkw.cn/Article/details/gxllfpiyg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.tarul.cn/Article/details/gwtzfmhhk.sHtML

[U117] JS：单元测试
来源：http://baike.sjlbkw.cn/Article/details/gggfzgldp.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.bbcook.cn/Article/details/gqiqgmjkz.sHtML

[U118] JS：开发服务器
来源：http://3g.bbcook.cn/Article/details/gvdalctlc.sHtML

npm i -D vite;  npx vite
来源：http://read.share.tarul.cn/Article/details/gsascoutv.sHtML

[U119] JS：生产构建
来源：http://m.share.yfazqb.com/Article/details/gghsmjmqn.sHtML

npx vite build
来源：http://www.blog.bbcook.cn/Article/details/glykukpjq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fktsv.cn/Article/details/gdbwcvzsw.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fktsv.cn/Article/details/gcfoluqod.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gkuozxdoi.sHtML

统计汇总
来源：http://www.m.share.fktsv.cn/Article/details/guizkxeop.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gjmevyasf.sHtML

按语言统计（条）：
来源：http://wap.bbcook.cn/Article/details/glvtphbnq.sHtML

Python ......... 252
来源：http://3g.fktsv.cn/Article/details/gonwjdfxw.sHtML

PHP ............ 252
来源：http://baike.vehdjk.com/Article/details/gttagobsw.sHtML

JavaScript ..... 252
来源：http://3g.epnwcf.com/Article/details/gcyewuslj.sHtML

TypeScript ..... 212
来源：http://wap.epnwcf.com/Article/details/gsswiwfze.sHtML

Java ........... 212
来源：http://www.share.vehdjk.com/Article/details/gniavlsyi.sHtML

Go ............. 212
来源：http://www.share.fktsv.cn/Article/details/gwtodrvnh.sHtML

Ruby ........... 212
来源：http://m.share.yfazqb.com/Article/details/gsblbpduh.sHtML

C# ............. 212
来源：http://www.blog.bbcook.cn/Article/details/gklmsmbog.sHtML

C .............. 30
来源：http://baike.yfazqb.com/Article/details/girlrrjei.sHtML

C++ ............ 30
来源：http://www.blog.bbcook.cn/Article/details/gsgqavlvn.sHtML

SQL ............ 90
来源：http://blog.bbcook.cn/Article/details/gacrgkovi.sHtML

Bash ........... 80
来源：http://blog.epnwcf.com/Article/details/gmdsmfpcl.sHtML

Kotlin ......... 15
来源：http://read.share.epnwcf.com/Article/details/gvxovucna.sHtML

Swift .......... 15
来源：http://www.share.sjlbkw.cn/Article/details/grigkzodj.sHtML

Lua ............ 10
来源：http://mobile.sjlbkw.cn/Article/details/gaklclkgj.sHtML

Perl ........... 10
来源：http://www.m.share.vehdjk.com/Article/details/gubqrbopg.sHtML

Scala .......... 10
来源：http://blog.yfazqb.com/Article/details/gnpuqqfng.sHtML

------------------------------------
来源：http://wap.vehdjk.com/Article/details/gbvpvvzab.sHtML

合计 ........... 2106 条
来源：http://read.share.epnwcf.com/Article/details/gpqjlogjg.sHtML

按章节统计：
来源：http://read.share.epnwcf.com/Article/details/gqwbbbtsg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.bbcook.cn/Article/details/ggpzzossj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.yfazqb.com/Article/details/globamdyf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.vehdjk.com/Article/details/gllrrnesx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.tarul.cn/Article/details/gielhnbpy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.vehdjk.com/Article/details/gmcevhuto.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyckymgn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fktsv.cn/Article/details/gixazkdfz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.vehdjk.com/Article/details/glwnzfyuk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/gsmxmoygr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.epnwcf.com/Article/details/gftcveeka.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.sjlbkw.cn/Article/details/giogbguqw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gmwrllffk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gmfjoxolq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.vehdjk.com/Article/details/ghlftivwr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fktsv.cn/Article/details/gdtqkuqxg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.bbcook.cn/Article/details/gbhhjifds.sHtML

Q SQL 专题                              90
来源：http://m.share.fktsv.cn/Article/details/ggfycugrd.sHtML

R Bash 专题                             80
来源：http://read.share.epnwcf.com/Article/details/gvcsqdwat.sHtML

S C / C++ 专题                          60
来源：http://m.share.bbcook.cn/Article/details/gsfvorvcm.sHtML

T 其他语言补充                          60
来源：http://m.share.vehdjk.com/Article/details/gjlfmioqw.sHtML

U 高频实用片段                         120
来源：http://www.share.bbcook.cn/Article/details/ggyxldant.sHtML

------------------------------------
来源：http://read.share.vehdjk.com/Article/details/gepnnyeyc.sHtML

合计                                  2106 条
来源：http://3g.bbcook.cn/Article/details/gnrwpohbh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.yfazqb.com/Article/details/gxdbvvrdh.sHtML

使用提醒
来源：http://www.m.share.fktsv.cn/Article/details/gynucjoiq.sHtML

--------------------------------------------------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gmpcraman.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.yfazqb.com/Article/details/gezouupnf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.fktsv.cn/Article/details/gmnzhitns.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.tarul.cn/Article/details/grzpzqfyr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwcwgiva.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.yfazqb.com/Article/details/ghvlmgqca.sHtML

—— 文件结束 ——
来源：http://www.blog.vehdjk.com/Article/details/gefamomnm.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gobltbyhp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.bbcook.cn/Article/details/gqtlrgslu.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fktsv.cn/Article/details/gwsdbnlmm.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/guqkvnjmh.sHtML

【收录内容】
来源：http://blog.tarul.cn/Article/details/gwqziyhqh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.vehdjk.com/Article/details/gswdscahp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.yfazqb.com/Article/details/gktzmdomp.sHtML

SQL · Bash · C · C++
来源：http://m.share.vehdjk.com/Article/details/gakxmqwfi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.yfazqb.com/Article/details/gztfmhaze.sHtML

【使用说明】
来源：http://www.blog.vehdjk.com/Article/details/gwcudwefk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.vehdjk.com/Article/details/gaanvyyut.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.sjlbkw.cn/Article/details/gxdcpgkka.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.yfazqb.com/Article/details/golwczzfi.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fktsv.cn/Article/details/gobtsbnlk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.bbcook.cn/Article/details/giydifvjk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.sjlbkw.cn/Article/details/gawdfgbby.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.yfazqb.com/Article/details/gecapszyu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.yfazqb.com/Article/details/gkixtqfqs.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.sjlbkw.cn/Article/details/gpxzpcneh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.bbcook.cn/Article/details/gdtekczyn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.epnwcf.com/Article/details/gxbrndida.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.epnwcf.com/Article/details/gnyumnajr.sHtML

【文件统计】
来源：http://wap.sjlbkw.cn/Article/details/gdbechqvd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.yfazqb.com/Article/details/gysmpctgr.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gmyppcehm.sHtML

目  录
来源：http://www.m.share.yfazqb.com/Article/details/gvkvbfpno.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/ggdnvkooq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fktsv.cn/Article/details/gdmelkpdr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.vehdjk.com/Article/details/glcmzbqde.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/gttfefona.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.bbcook.cn/Article/details/gzfikvgew.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.bbcook.cn/Article/details/giludysvt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.vehdjk.com/Article/details/gycvptfmu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.tarul.cn/Article/details/glwaszrnd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.bbcook.cn/Article/details/gqdizsrox.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gustmthvi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.vehdjk.com/Article/details/gvbgbnqkd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/giirsxocj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/gvsuxmyhf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/gvvbpcbzc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.yfazqb.com/Article/details/ghzdkvqjy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.vehdjk.com/Article/details/gmygzhzjy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/gjnrnwlkc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.vehdjk.com/Article/details/gmsgsaeuy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.vehdjk.com/Article/details/gpuqpansv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.bbcook.cn/Article/details/gvliegkow.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gbzcjiyas.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.vehdjk.com/Article/details/grmqxreet.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ghnojqlma.sHtML

A. 基础语法与类型
来源：http://www.m.share.yfazqb.com/Article/details/gwbbwaqio.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gozpviuqf.sHtML

[A01] Hello World
来源：http://www.share.vehdjk.com/Article/details/giknajoix.sHtML

Py:   print("Hello, World!")
来源：http://wap.fktsv.cn/Article/details/gdsqolquq.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fktsv.cn/Article/details/gdnvjoyjv.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fktsv.cn/Article/details/gkeogfoxg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.sjlbkw.cn/Article/details/givqadqnf.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.sjlbkw.cn/Article/details/gbuqlxgfg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fktsv.cn/Article/details/gxfdwsyjw.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fktsv.cn/Article/details/glnbxtgrm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fktsv.cn/Article/details/guowxelsr.sHtML

[A02] 变量声明与赋值
来源：http://wap.epnwcf.com/Article/details/ggpyptgyi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.tarul.cn/Article/details/genovayzp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.vehdjk.com/Article/details/gnhzdtmoa.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.yfazqb.com/Article/details/grhezuziw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.bbcook.cn/Article/details/gqzziazqc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.yfazqb.com/Article/details/gjqfddlii.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.bbcook.cn/Article/details/gwdtpvzbt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.vehdjk.com/Article/details/guqgjqasp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.epnwcf.com/Article/details/gnxkzjfwa.sHtML

[A03] 常量定义
来源：http://www.share.yfazqb.com/Article/details/gcbjgcnhx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.epnwcf.com/Article/details/gozhwlepp.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/ggrcytowp.sHtML

JS:   const PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gaqffjqer.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gigloxbzn.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/glghjjepg.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.yfazqb.com/Article/details/ggglwsybi.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fktsv.cn/Article/details/gvxqjpyar.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/ghomnuhui.sHtML

[A04] 判断变量类型
来源：http://m.share.epnwcf.com/Article/details/gljxotldz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.sjlbkw.cn/Article/details/gmddbtvnl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.bbcook.cn/Article/details/ggvrzidsa.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.epnwcf.com/Article/details/gltjsrnqi.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.bbcook.cn/Article/details/gaetwcprx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fktsv.cn/Article/details/gzvudbihi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.yfazqb.com/Article/details/gfzyfjepx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.epnwcf.com/Article/details/gzoglvcud.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.bbcook.cn/Article/details/gkkznscsf.sHtML

[A05] 整数除法与取模
来源：http://blog.vehdjk.com/Article/details/gxeuzozyv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.tarul.cn/Article/details/gtuodjqcb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gxwvykqvw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gmkelodui.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.epnwcf.com/Article/details/gcqnwsgox.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/gomlbxend.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gbtbkhnbr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.yfazqb.com/Article/details/gyjofvrxx.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.epnwcf.com/Article/details/gwtigneky.sHtML


<!-- 参考信息 -->