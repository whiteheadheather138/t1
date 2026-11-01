代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://3g.tarul.cn/Article/details/gputsudnr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.epnwcf.com/Article/details/gtuwiiikg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fktsv.cn/Article/details/gsxbkkgxz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.epnwcf.com/Article/details/gpfbayivl.sHtML

[U43] PHP：声明命名空间
来源：http://wap.vehdjk.com/Article/details/gakkbjbpv.sHtML

namespace App\Http;
来源：http://read.share.bbcook.cn/Article/details/ghnkkshuc.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.tarul.cn/Article/details/gudhgpfjf.sHtML

declare(strict_types=1);
来源：http://baike.epnwcf.com/Article/details/gpgbtrmoy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.bbcook.cn/Article/details/gqqopewwr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/geayftbxr.sHtML

[U46] PHP：可空类型
来源：http://read.share.sjlbkw.cn/Article/details/gxdzkvzat.sHtML

?string $name = null
来源：http://www.m.share.epnwcf.com/Article/details/gbamaeara.sHtML

[U47] PHP：联合类型
来源：http://baike.sjlbkw.cn/Article/details/gntssxnff.sHtML

int|string $id
来源：http://www.blog.epnwcf.com/Article/details/gvyvkuwep.sHtML

[U48] PHP：纯枚举
来源：http://www.share.tarul.cn/Article/details/gxwpdudym.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.bbcook.cn/Article/details/gsnhjrrxu.sHtML

[U49] PHP：只读属性
来源：http://www.share.vehdjk.com/Article/details/gkrtsvhcq.sHtML

public readonly string $name
来源：http://www.blog.tarul.cn/Article/details/gyrtnumko.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.epnwcf.com/Article/details/glwftxhea.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.yfazqb.com/Article/details/gfenvpxhn.sHtML

[U51] PHP：数组解构
来源：http://mobile.yfazqb.com/Article/details/gqaxryykl.sHtML

[$a, $b] = $arr;
来源：http://baike.vehdjk.com/Article/details/giecfsvti.sHtML

[U52] PHP：箭头函数
来源：http://www.share.sjlbkw.cn/Article/details/ghycuxzrt.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.tarul.cn/Article/details/gdfuevefl.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fktsv.cn/Article/details/gymvnnquy.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.epnwcf.com/Article/details/gmgcaowpz.sHtML

[U54] PHP：空安全调用
来源：http://3g.epnwcf.com/Article/details/gxghoaqqd.sHtML

$obj?->method()
来源：http://3g.epnwcf.com/Article/details/ghowpsnbn.sHtML

[U55] PHP：match 表达式
来源：http://baike.bbcook.cn/Article/details/gbmqgofwj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.yfazqb.com/Article/details/golvycsbp.sHtML

[U56] PHP：命名参数
来源：http://mobile.tarul.cn/Article/details/gywbabliu.sHtML

f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/gbvtyanyy.sHtML

[U57] PHP：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gqaapzajj.sHtML

"值: {$a}"
来源：http://www.share.bbcook.cn/Article/details/gjncewcwk.sHtML

[U58] PHP：数组三件套
来源：http://blog.sjlbkw.cn/Article/details/gwekwhctr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.epnwcf.com/Article/details/gglkuqwbv.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fktsv.cn/Article/details/gmtletlvd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.sjlbkw.cn/Article/details/gtpnulwic.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.tarul.cn/Article/details/gzyzabuga.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.bbcook.cn/Article/details/gozbvogmh.sHtML

[U61] PHP：正则
来源：http://www.blog.vehdjk.com/Article/details/gpgzbgbwf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fktsv.cn/Article/details/gfjruuvoq.sHtML

[U62] PHP：日期对象
来源：http://mobile.bbcook.cn/Article/details/gqtfzskgv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.sjlbkw.cn/Article/details/gdgxhcrgt.sHtML

[U63] PHP：文件读写
来源：http://www.blog.yfazqb.com/Article/details/gckzqfvtw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.bbcook.cn/Article/details/gwhvsiclm.sHtML

[U64] PHP：目录遍历
来源：http://blog.bbcook.cn/Article/details/gszsiqwal.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.bbcook.cn/Article/details/ghuzopefv.sHtML

[U65] PHP：会话
来源：http://m.share.fktsv.cn/Article/details/gqqjunuxx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.tarul.cn/Article/details/groonmqaf.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fktsv.cn/Article/details/gotweuoll.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.yfazqb.com/Article/details/gxijrdwma.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.yfazqb.com/Article/details/glpqlcfjq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.yfazqb.com/Article/details/gwqrsdwte.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fktsv.cn/Article/details/gyeipdpxh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.epnwcf.com/Article/details/gbwbzskjj.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fktsv.cn/Article/details/guwuozkls.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.vehdjk.com/Article/details/gologqpkb.sHtML

[U70] PHP：PDO 事务
来源：http://3g.yfazqb.com/Article/details/ggeqcwqef.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.yfazqb.com/Article/details/gqbtnrhak.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fktsv.cn/Article/details/gigrhwdpe.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.tarul.cn/Article/details/gnoutwvtd.sHtML

[U72] PHP：写错误日志
来源：http://www.share.bbcook.cn/Article/details/gowyphqtr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.epnwcf.com/Article/details/gikqyoceg.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.tarul.cn/Article/details/gykvyqqmu.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fktsv.cn/Article/details/gujomrnji.sHtML

[U74] PHP：读取环境变量
来源：http://baike.bbcook.cn/Article/details/grjzxpgcx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.sjlbkw.cn/Article/details/ggdcxsqhb.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fktsv.cn/Article/details/gcchprvib.sHtML

composer require psr/container
来源：http://www.share.epnwcf.com/Article/details/gdcjdggnj.sHtML

[U76] PHP：简单路由
来源：http://3g.tarul.cn/Article/details/gehpealeg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.yfazqb.com/Article/details/gdihvxueo.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fktsv.cn/Article/details/gtgfhnoqn.sHtML

composer require twig/twig
来源：http://wap.tarul.cn/Article/details/gxktzirkd.sHtML

[U78] PHP：单元测试
来源：http://blog.sjlbkw.cn/Article/details/gxcumonax.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.epnwcf.com/Article/details/guzcklnly.sHtML

[U79] PHP：静态分析
来源：http://blog.yfazqb.com/Article/details/gacdhkabl.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fktsv.cn/Article/details/gavxcehyk.sHtML

[U80] PHP：代码规范修复
来源：http://wap.epnwcf.com/Article/details/gejfxzeje.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.epnwcf.com/Article/details/gyeclvsdf.sHtML

[U81] JS：初始化项目
来源：http://3g.tarul.cn/Article/details/gmgooxldp.sHtML

npm init -y;  npm i express
来源：http://www.share.bbcook.cn/Article/details/gedlpascb.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.tarul.cn/Article/details/gnxkqmndy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.vehdjk.com/Article/details/grzqnjqlo.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.bbcook.cn/Article/details/gaidjnfky.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.vehdjk.com/Article/details/gaptjxgka.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.sjlbkw.cn/Article/details/glbpjaoel.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.yfazqb.com/Article/details/gemnsqple.sHtML

[U85] JS：可选链
来源：http://3g.epnwcf.com/Article/details/grbetvldm.sHtML

a?.b?.c
来源：http://baike.epnwcf.com/Article/details/guttpnogx.sHtML

[U86] JS：空值合并
来源：http://www.share.tarul.cn/Article/details/gzlnuhzhv.sHtML

a ?? b
来源：http://www.m.share.tarul.cn/Article/details/gvlhvhuib.sHtML

[U87] JS：解构默认值
来源：http://blog.bbcook.cn/Article/details/gkmmlkfma.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.yfazqb.com/Article/details/gqjgmizml.sHtML

[U88] JS：对象展开合并
来源：http://blog.yfazqb.com/Article/details/gdoioqudy.sHtML

{ ...a, ...b }
来源：http://blog.epnwcf.com/Article/details/gxnhzmgkt.sHtML

[U89] JS：数组去重
来源：http://read.share.tarul.cn/Article/details/gkstngtnj.sHtML

[...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gscwgykjb.sHtML

[U90] JS：数字数组排序
来源：http://mobile.epnwcf.com/Article/details/grsoywjbo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gcgvnnmpq.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.epnwcf.com/Article/details/gaeoxalzn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.tarul.cn/Article/details/gmxowwcxy.sHtML

[U92] JS：深拷贝
来源：http://read.share.epnwcf.com/Article/details/gojamuiwl.sHtML

structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/gfnfsehtf.sHtML

[U93] JS：模板字符串
来源：http://www.share.fktsv.cn/Article/details/gahtagwjr.sHtML

`共 ${n} 条`
来源：http://wap.bbcook.cn/Article/details/gnafkfzgt.sHtML

[U94] JS：箭头函数
来源：http://3g.bbcook.cn/Article/details/gcnvfgihc.sHtML

const double = x => x * 2;
来源：http://blog.tarul.cn/Article/details/gbyuvngps.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.bbcook.cn/Article/details/gdjplzoqp.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.yfazqb.com/Article/details/gjgogzmkd.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.epnwcf.com/Article/details/gvgpokxbx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/glwmohyfb.sHtML

[U97] JS：并发请求
来源：http://baike.fktsv.cn/Article/details/gccqwcuzi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/gseaywjxd.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.sjlbkw.cn/Article/details/gjwkqgtqj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.bbcook.cn/Article/details/ggtrcxppl.sHtML

[U99] JS：事件监听
来源：http://read.share.epnwcf.com/Article/details/glsspuhds.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.tarul.cn/Article/details/gervxpwcj.sHtML

[U100] JS：DOM 查询
来源：http://m.share.epnwcf.com/Article/details/gopooqzno.sHtML

document.querySelector(".item")
来源：http://baike.yfazqb.com/Article/details/ggnkvlnfz.sHtML

[U101] JS：classList 操作
来源：http://3g.epnwcf.com/Article/details/gfnihzvwh.sHtML

el.classList.toggle("active")
来源：http://www.share.vehdjk.com/Article/details/gyrbeijvh.sHtML

[U102] JS：本地存储
来源：http://m.share.tarul.cn/Article/details/gyeyhdjtd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fktsv.cn/Article/details/gjvjheett.sHtML

[U103] JS：定时器
来源：http://mobile.yfazqb.com/Article/details/gmvxxjfbb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.sjlbkw.cn/Article/details/gufhqtczs.sHtML

[U104] JS：防抖
来源：http://www.blog.bbcook.cn/Article/details/gqhgrnomz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/gahexdmha.sHtML

[U105] JS：节流
来源：http://blog.sjlbkw.cn/Article/details/gglgfvraa.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.bbcook.cn/Article/details/gsngglsfh.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.tarul.cn/Article/details/gbjwkvxdh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.bbcook.cn/Article/details/gyeaeogbj.sHtML

[U107] JS：数字千分位
来源：http://read.share.vehdjk.com/Article/details/gfgagqmhj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.bbcook.cn/Article/details/gubsftabt.sHtML

[U108] JS：随机整数
来源：http://read.share.tarul.cn/Article/details/giqlidwqq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.sjlbkw.cn/Article/details/glumolzmx.sHtML

[U109] JS：数组分组
来源：http://www.blog.vehdjk.com/Article/details/ggljuvzht.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.bbcook.cn/Article/details/gubmhhjnn.sHtML

[U110] JS：数组分块
来源：http://read.share.vehdjk.com/Article/details/gdadxiuvy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fktsv.cn/Article/details/gjuvebspv.sHtML

[U111] JS：对象转 Map
来源：http://read.share.sjlbkw.cn/Article/details/gpqebheze.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fktsv.cn/Article/details/gxeggqive.sHtML

[U112] JS：字符串补位
来源：http://m.share.tarul.cn/Article/details/gsozfickg.sHtML

"7".padStart(3, "0")
来源：http://m.share.bbcook.cn/Article/details/gqlkashuu.sHtML

[U113] JS：正则替换全部
来源：http://mobile.bbcook.cn/Article/details/ghqseccst.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gsvkymtoo.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.yfazqb.com/Article/details/gmnamxlxv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.tarul.cn/Article/details/ggroosphw.sHtML

[U115] JS：生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/gvcnmmkch.sHtML

crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/grybrpigh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.bbcook.cn/Article/details/gwryjrasx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.sjlbkw.cn/Article/details/gytupcnat.sHtML

[U117] JS：单元测试
来源：http://m.share.epnwcf.com/Article/details/gltqoassm.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.sjlbkw.cn/Article/details/gvinfalkn.sHtML

[U118] JS：开发服务器
来源：http://m.share.epnwcf.com/Article/details/gybusnlyk.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.tarul.cn/Article/details/gulqybbit.sHtML

[U119] JS：生产构建
来源：http://m.share.fktsv.cn/Article/details/gmokksaya.sHtML

npx vite build
来源：http://www.m.share.fktsv.cn/Article/details/gzfxiaoln.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.epnwcf.com/Article/details/gdacocwzm.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.sjlbkw.cn/Article/details/gtstbbahl.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gbwnqxtfj.sHtML

统计汇总
来源：http://www.blog.bbcook.cn/Article/details/gzognasgb.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gssgmxhat.sHtML

按语言统计（条）：
来源：http://blog.sjlbkw.cn/Article/details/glatbfkjt.sHtML

Python ......... 252
来源：http://www.blog.bbcook.cn/Article/details/glwtwnffy.sHtML

PHP ............ 252
来源：http://www.blog.tarul.cn/Article/details/grmzzpdqu.sHtML

JavaScript ..... 252
来源：http://mobile.epnwcf.com/Article/details/gkhlipuib.sHtML

TypeScript ..... 212
来源：http://www.share.sjlbkw.cn/Article/details/gxomaebhs.sHtML

Java ........... 212
来源：http://baike.bbcook.cn/Article/details/giuyytyqs.sHtML

Go ............. 212
来源：http://blog.vehdjk.com/Article/details/gixuaafdo.sHtML

Ruby ........... 212
来源：http://read.share.yfazqb.com/Article/details/gosgvgtxu.sHtML

C# ............. 212
来源：http://blog.yfazqb.com/Article/details/gsqvsuvnj.sHtML

C .............. 30
来源：http://read.share.yfazqb.com/Article/details/gdouqofxo.sHtML

C++ ............ 30
来源：http://read.share.tarul.cn/Article/details/ghkywwmox.sHtML

SQL ............ 90
来源：http://baike.fktsv.cn/Article/details/gbbddbebh.sHtML

Bash ........... 80
来源：http://www.share.yfazqb.com/Article/details/gfdenlkrw.sHtML

Kotlin ......... 15
来源：http://read.share.bbcook.cn/Article/details/gqraoeqay.sHtML

Swift .......... 15
来源：http://www.blog.sjlbkw.cn/Article/details/gkpqumfku.sHtML

Lua ............ 10
来源：http://baike.fktsv.cn/Article/details/gnqwpxydo.sHtML

Perl ........... 10
来源：http://www.blog.epnwcf.com/Article/details/gazchkdnn.sHtML

Scala .......... 10
来源：http://www.m.share.vehdjk.com/Article/details/gmyvdwqtj.sHtML

------------------------------------
来源：http://3g.epnwcf.com/Article/details/gpkmyrlrv.sHtML

合计 ........... 2106 条
来源：http://m.share.epnwcf.com/Article/details/ggvdhxyfj.sHtML

按章节统计：
来源：http://www.blog.yfazqb.com/Article/details/gywvedhah.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.epnwcf.com/Article/details/gtpcgqvtk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.vehdjk.com/Article/details/gkbmqeihk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.bbcook.cn/Article/details/gdciizjlb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.yfazqb.com/Article/details/gaclgssul.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fktsv.cn/Article/details/gvaylrglw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.epnwcf.com/Article/details/gibonpzly.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.bbcook.cn/Article/details/gixkizmhs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.tarul.cn/Article/details/ggpfheprd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/gqafqpwin.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.tarul.cn/Article/details/gplecluju.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gcqjrpqev.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/geggorskc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gtrbttvkf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.vehdjk.com/Article/details/ggiwlmabt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.yfazqb.com/Article/details/gqvrtravt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/gmfixufqx.sHtML

Q SQL 专题                              90
来源：http://3g.epnwcf.com/Article/details/gqhltzbrf.sHtML

R Bash 专题                             80
来源：http://www.m.share.yfazqb.com/Article/details/gdsokyjkl.sHtML

S C / C++ 专题                          60
来源：http://blog.sjlbkw.cn/Article/details/gqfjsfeei.sHtML

T 其他语言补充                          60
来源：http://3g.tarul.cn/Article/details/gyaksxagi.sHtML

U 高频实用片段                         120
来源：http://www.blog.fktsv.cn/Article/details/gfkoktbad.sHtML

------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gvmdohhof.sHtML

合计                                  2106 条
来源：http://3g.vehdjk.com/Article/details/gzkioware.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/gejvvljzf.sHtML

使用提醒
来源：http://m.share.yfazqb.com/Article/details/gjepkbvir.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/glzhlogvi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.vehdjk.com/Article/details/ghqaxbwbk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.yfazqb.com/Article/details/gkhopszue.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.tarul.cn/Article/details/gitxfbxvb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.tarul.cn/Article/details/gjqxlabdp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.epnwcf.com/Article/details/gydocbqvr.sHtML

—— 文件结束 ——
来源：http://blog.yfazqb.com/Article/details/gfhskdvsh.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/grpfipchi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.bbcook.cn/Article/details/gpifojuxw.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.yfazqb.com/Article/details/ggwuwkmtz.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gekhgxuwa.sHtML

【收录内容】
来源：http://www.blog.yfazqb.com/Article/details/ghdxgrcnw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.sjlbkw.cn/Article/details/ggwgzgpaz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.sjlbkw.cn/Article/details/gvnguoies.sHtML

SQL · Bash · C · C++
来源：http://blog.vehdjk.com/Article/details/gumfimbuu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.vehdjk.com/Article/details/gdedhkfrd.sHtML

【使用说明】
来源：http://blog.bbcook.cn/Article/details/gtbqkthmj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.sjlbkw.cn/Article/details/gsbkmlgwd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.vehdjk.com/Article/details/gmcncbvbk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.bbcook.cn/Article/details/gsipigoza.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.yfazqb.com/Article/details/gtjxxvogy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.vehdjk.com/Article/details/gihrsdria.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.epnwcf.com/Article/details/gftcphzrf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.tarul.cn/Article/details/gmxwvqnbj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.tarul.cn/Article/details/goyqvpcds.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fktsv.cn/Article/details/gatbazvyh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.vehdjk.com/Article/details/gzmgztxjo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.sjlbkw.cn/Article/details/gkesebues.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.bbcook.cn/Article/details/gtfzqvqyu.sHtML

【文件统计】
来源：http://www.blog.tarul.cn/Article/details/gmaawgocg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.yfazqb.com/Article/details/gyhythkaf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/gxpvmbsis.sHtML

目  录
来源：http://mobile.sjlbkw.cn/Article/details/gdxrtssaf.sHtML

--------------------------------------------------------------------------------
来源：http://baike.bbcook.cn/Article/details/gzeposfrj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.tarul.cn/Article/details/gndnatpuq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.epnwcf.com/Article/details/gvgfclwom.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.tarul.cn/Article/details/gevwmhuqo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fktsv.cn/Article/details/gigjmqqiv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.vehdjk.com/Article/details/gqqnlaeki.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.vehdjk.com/Article/details/ghkowumes.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.bbcook.cn/Article/details/gvehwkqpl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.bbcook.cn/Article/details/gmglekmjg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/gyxxvjtby.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fktsv.cn/Article/details/grvzkixpb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/golwebdgl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/gdxlcwxhx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/gabgyukbg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.tarul.cn/Article/details/gqkftswkt.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.vehdjk.com/Article/details/gfzayfzmk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gcpnnotxl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.yfazqb.com/Article/details/gjldlgzjz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.vehdjk.com/Article/details/gfcnpvqqn.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.bbcook.cn/Article/details/gitfjqlhk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.tarul.cn/Article/details/gyavsjblz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fktsv.cn/Article/details/gozaaygbb.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gnbthmxyz.sHtML

A. 基础语法与类型
来源：http://mobile.bbcook.cn/Article/details/gslkoozgd.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gyhnvzpkf.sHtML

[A01] Hello World
来源：http://baike.vehdjk.com/Article/details/ghjpybmoc.sHtML

Py:   print("Hello, World!")
来源：http://mobile.bbcook.cn/Article/details/gubmanruq.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.bbcook.cn/Article/details/gcquenseo.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.tarul.cn/Article/details/gbofcsxqx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.sjlbkw.cn/Article/details/gizpqtxjp.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.tarul.cn/Article/details/gpqmsedoc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.yfazqb.com/Article/details/ggurvquci.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.tarul.cn/Article/details/garbncgvu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.yfazqb.com/Article/details/gbbobudeo.sHtML

[A02] 变量声明与赋值
来源：http://www.share.yfazqb.com/Article/details/gyfjdzhqo.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.tarul.cn/Article/details/grchlncqq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fktsv.cn/Article/details/gsjwcszlw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.tarul.cn/Article/details/guyzsrewg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.bbcook.cn/Article/details/gwjtcipgb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.bbcook.cn/Article/details/giihgmtmf.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fktsv.cn/Article/details/gjjtvkdly.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.bbcook.cn/Article/details/gyaodmuag.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.vehdjk.com/Article/details/gghiuqxsw.sHtML

[A03] 常量定义
来源：http://www.m.share.bbcook.cn/Article/details/gmnrnhzbt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.epnwcf.com/Article/details/gylssiobk.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gpyslqbsj.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gqxdbxfet.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gfnuzbwmt.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gxsgnumrw.sHtML

Go:   const PI = 3.14159
来源：http://read.share.tarul.cn/Article/details/gfkbeaopz.sHtML

Ruby: PI = 3.14159
来源：http://read.share.sjlbkw.cn/Article/details/gfiolxchv.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gayovinpz.sHtML

[A04] 判断变量类型
来源：http://3g.sjlbkw.cn/Article/details/gxkjghxqi.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.vehdjk.com/Article/details/gmiavlukt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.vehdjk.com/Article/details/gqwzwghpt.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.vehdjk.com/Article/details/gzzcglrhm.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fktsv.cn/Article/details/ghwdnifpi.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.bbcook.cn/Article/details/gsidqxfxh.sHtML


<!-- 参考信息 -->