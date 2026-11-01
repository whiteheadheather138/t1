代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://baike.tarul.cn/Article/details/gupyqutvy.sHtML

sys.stdout.isatty()
来源：http://baike.epnwcf.com/Article/details/gkjjljvnv.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.bbcook.cn/Article/details/gwdflrplj.sHtML

print("err", file=sys.stderr)
来源：http://baike.sjlbkw.cn/Article/details/gsuwkyjxf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.vehdjk.com/Article/details/getudcnpb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.sjlbkw.cn/Article/details/ggerdzcxy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.bbcook.cn/Article/details/gdnrodlae.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.sjlbkw.cn/Article/details/gfrczrqug.sHtML

[U43] PHP：声明命名空间
来源：http://baike.vehdjk.com/Article/details/gngsdcqxt.sHtML

namespace App\Http;
来源：http://read.share.tarul.cn/Article/details/gfpqgqqzx.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.bbcook.cn/Article/details/gogwkcwym.sHtML

declare(strict_types=1);
来源：http://read.share.tarul.cn/Article/details/ghpwgnszz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.sjlbkw.cn/Article/details/gcpkuxjop.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gtwoszwji.sHtML

[U46] PHP：可空类型
来源：http://blog.bbcook.cn/Article/details/gdbwqtyto.sHtML

?string $name = null
来源：http://blog.epnwcf.com/Article/details/gayqvlzpw.sHtML

[U47] PHP：联合类型
来源：http://mobile.bbcook.cn/Article/details/grihizfuv.sHtML

int|string $id
来源：http://mobile.vehdjk.com/Article/details/gemiqbckt.sHtML

[U48] PHP：纯枚举
来源：http://wap.vehdjk.com/Article/details/guzhxmlxp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.yfazqb.com/Article/details/gmiqpkwnr.sHtML

[U49] PHP：只读属性
来源：http://wap.yfazqb.com/Article/details/gzzpvbgdt.sHtML

public readonly string $name
来源：http://3g.yfazqb.com/Article/details/gyeqxaysz.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.vehdjk.com/Article/details/ghsbptaqi.sHtML

public function __construct(private int $id) {}
来源：http://www.share.bbcook.cn/Article/details/gvexmapzr.sHtML

[U51] PHP：数组解构
来源：http://wap.tarul.cn/Article/details/gdtomxtfr.sHtML

[$a, $b] = $arr;
来源：http://blog.bbcook.cn/Article/details/ggkmujktm.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.tarul.cn/Article/details/gsspobhos.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.epnwcf.com/Article/details/gtrriatjd.sHtML

[U53] PHP：空合并运算符
来源：http://baike.epnwcf.com/Article/details/gzaaxrfog.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.yfazqb.com/Article/details/gmqtiedsz.sHtML

[U54] PHP：空安全调用
来源：http://read.share.tarul.cn/Article/details/gqpcpnloy.sHtML

$obj?->method()
来源：http://www.m.share.epnwcf.com/Article/details/gjbuftiub.sHtML

[U55] PHP：match 表达式
来源：http://3g.tarul.cn/Article/details/gzhesjecr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.epnwcf.com/Article/details/gdpdaqxqy.sHtML

[U56] PHP：命名参数
来源：http://blog.vehdjk.com/Article/details/gpzlncmlk.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/gjtosptpr.sHtML

[U57] PHP：字符串插值
来源：http://www.share.epnwcf.com/Article/details/gqojiillk.sHtML

"值: {$a}"
来源：http://baike.epnwcf.com/Article/details/gjjwrimdi.sHtML

[U58] PHP：数组三件套
来源：http://blog.yfazqb.com/Article/details/gozlmmdzg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.epnwcf.com/Article/details/gjzjtdqfb.sHtML

[U59] PHP：自定义排序
来源：http://baike.yfazqb.com/Article/details/gmeeormjy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.yfazqb.com/Article/details/glkryiune.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fktsv.cn/Article/details/gsvgcybsk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.yfazqb.com/Article/details/gxxcywrma.sHtML

[U61] PHP：正则
来源：http://www.m.share.bbcook.cn/Article/details/grijfnqdq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gswrntmcl.sHtML

[U62] PHP：日期对象
来源：http://mobile.tarul.cn/Article/details/gvezkhicm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.sjlbkw.cn/Article/details/gijovdxql.sHtML

[U63] PHP：文件读写
来源：http://www.share.tarul.cn/Article/details/guhnhjayr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.bbcook.cn/Article/details/gyfrblkqt.sHtML

[U64] PHP：目录遍历
来源：http://m.share.sjlbkw.cn/Article/details/gkjvhteaj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.yfazqb.com/Article/details/gexyxbfbf.sHtML

[U65] PHP：会话
来源：http://www.blog.bbcook.cn/Article/details/gwfqbchgx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.yfazqb.com/Article/details/ghbcetbte.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fktsv.cn/Article/details/gyknkfzsx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.bbcook.cn/Article/details/gloqordym.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.yfazqb.com/Article/details/glhabjuav.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.epnwcf.com/Article/details/gjirawkoq.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.sjlbkw.cn/Article/details/gmtganawo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.vehdjk.com/Article/details/gtgfhxkjg.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.yfazqb.com/Article/details/gviwdfwnb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.vehdjk.com/Article/details/gjatrazeg.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.sjlbkw.cn/Article/details/gvhwiyvlz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.sjlbkw.cn/Article/details/gcivcyfbq.sHtML

[U71] PHP：抛出异常
来源：http://wap.sjlbkw.cn/Article/details/grwfkonlb.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.bbcook.cn/Article/details/gvjkdkovx.sHtML

[U72] PHP：写错误日志
来源：http://m.share.yfazqb.com/Article/details/gcvkrwwnm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.tarul.cn/Article/details/gkbxyencg.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.vehdjk.com/Article/details/ghowwdobd.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.bbcook.cn/Article/details/gfoylqssi.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.tarul.cn/Article/details/gemlosjnz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fktsv.cn/Article/details/gkzapyulj.sHtML

[U75] PHP：依赖注入
来源：http://blog.tarul.cn/Article/details/gqekoqthl.sHtML

composer require psr/container
来源：http://wap.bbcook.cn/Article/details/gzaqehqpd.sHtML

[U76] PHP：简单路由
来源：http://blog.vehdjk.com/Article/details/grpzjpclz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.tarul.cn/Article/details/grmfcxxch.sHtML

[U77] PHP：模板渲染
来源：http://read.share.vehdjk.com/Article/details/grdmclxkj.sHtML

composer require twig/twig
来源：http://wap.tarul.cn/Article/details/gpiltxthu.sHtML

[U78] PHP：单元测试
来源：http://3g.sjlbkw.cn/Article/details/geuejlzrv.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.sjlbkw.cn/Article/details/gdoistxet.sHtML

[U79] PHP：静态分析
来源：http://3g.sjlbkw.cn/Article/details/gggfjzuit.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fktsv.cn/Article/details/gnwbugxrx.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.bbcook.cn/Article/details/gpduyghtt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.bbcook.cn/Article/details/gaeeuyslc.sHtML

[U81] JS：初始化项目
来源：http://mobile.tarul.cn/Article/details/ghfcmoett.sHtML

npm init -y;  npm i express
来源：http://read.share.sjlbkw.cn/Article/details/glpwypkks.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.vehdjk.com/Article/details/gzquholkn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.epnwcf.com/Article/details/gpolmahgt.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.bbcook.cn/Article/details/gmzpfaoop.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.bbcook.cn/Article/details/gxziovnlx.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.epnwcf.com/Article/details/gpbrdxjhu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.tarul.cn/Article/details/gquxilnoi.sHtML

[U85] JS：可选链
来源：http://www.m.share.epnwcf.com/Article/details/guntyoqtn.sHtML

a?.b?.c
来源：http://m.share.bbcook.cn/Article/details/gpacgreon.sHtML

[U86] JS：空值合并
来源：http://www.m.share.bbcook.cn/Article/details/giptlddos.sHtML

a ?? b
来源：http://read.share.fktsv.cn/Article/details/gumidjrjd.sHtML

[U87] JS：解构默认值
来源：http://m.share.fktsv.cn/Article/details/gayrtxnxj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fktsv.cn/Article/details/gcyhbwtwk.sHtML

[U88] JS：对象展开合并
来源：http://www.share.yfazqb.com/Article/details/gkrmqijzd.sHtML

{ ...a, ...b }
来源：http://www.m.share.yfazqb.com/Article/details/gnwxvayyp.sHtML

[U89] JS：数组去重
来源：http://blog.fktsv.cn/Article/details/gqqfilhax.sHtML

[...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gibefpzpb.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.yfazqb.com/Article/details/gwfutqxii.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gwrwvtzhz.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.bbcook.cn/Article/details/gujukfoha.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.tarul.cn/Article/details/guarptpce.sHtML

[U92] JS：深拷贝
来源：http://wap.vehdjk.com/Article/details/gwdtxqzlv.sHtML

structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/gnquiqorp.sHtML

[U93] JS：模板字符串
来源：http://www.share.sjlbkw.cn/Article/details/gfhdhahkh.sHtML

`共 ${n} 条`
来源：http://mobile.yfazqb.com/Article/details/grcfoaxju.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.bbcook.cn/Article/details/gjmbvvjfv.sHtML

const double = x => x * 2;
来源：http://3g.yfazqb.com/Article/details/gkdsxdkng.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.yfazqb.com/Article/details/gupltfjxn.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.bbcook.cn/Article/details/ghyqttody.sHtML

[U96] JS：async/await 与异常
来源：http://blog.epnwcf.com/Article/details/gdfzsxuae.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/gioiexvfd.sHtML

[U97] JS：并发请求
来源：http://mobile.bbcook.cn/Article/details/gpedblilt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/ggxtazjkw.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.tarul.cn/Article/details/gmdweacjb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.bbcook.cn/Article/details/gfyjlsepi.sHtML

[U99] JS：事件监听
来源：http://blog.vehdjk.com/Article/details/gklqzisrf.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.tarul.cn/Article/details/gnqzugclk.sHtML

[U100] JS：DOM 查询
来源：http://mobile.yfazqb.com/Article/details/gqwicinws.sHtML

document.querySelector(".item")
来源：http://m.share.fktsv.cn/Article/details/glggwewbs.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.yfazqb.com/Article/details/gzazgsyut.sHtML

el.classList.toggle("active")
来源：http://blog.fktsv.cn/Article/details/gjfbjtpdy.sHtML

[U102] JS：本地存储
来源：http://www.blog.sjlbkw.cn/Article/details/gsdmuzpmi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fktsv.cn/Article/details/gviatcxqc.sHtML

[U103] JS：定时器
来源：http://www.m.share.bbcook.cn/Article/details/ghqxilyyq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.yfazqb.com/Article/details/ghmdjnssv.sHtML

[U104] JS：防抖
来源：http://baike.yfazqb.com/Article/details/gyiifoukn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/gddmntwja.sHtML

[U105] JS：节流
来源：http://read.share.sjlbkw.cn/Article/details/gselancne.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.tarul.cn/Article/details/ganeaucpt.sHtML

[U106] JS：日期格式化
来源：http://read.share.bbcook.cn/Article/details/gojwbpanu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.vehdjk.com/Article/details/gylkwhmcd.sHtML

[U107] JS：数字千分位
来源：http://blog.sjlbkw.cn/Article/details/gzlavmlve.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.bbcook.cn/Article/details/givexwpkm.sHtML

[U108] JS：随机整数
来源：http://www.share.yfazqb.com/Article/details/gojxqpmjw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fktsv.cn/Article/details/guzrzhykn.sHtML

[U109] JS：数组分组
来源：http://www.m.share.tarul.cn/Article/details/gajdxxbcg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.yfazqb.com/Article/details/gqsvaofqc.sHtML

[U110] JS：数组分块
来源：http://www.m.share.yfazqb.com/Article/details/gkjdapcfu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.yfazqb.com/Article/details/gjnyxorpl.sHtML

[U111] JS：对象转 Map
来源：http://3g.bbcook.cn/Article/details/glkcinvgh.sHtML

new Map(Object.entries(obj))
来源：http://3g.epnwcf.com/Article/details/gnmnveewh.sHtML

[U112] JS：字符串补位
来源：http://3g.sjlbkw.cn/Article/details/gghczvmea.sHtML

"7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/grspwrset.sHtML

[U113] JS：正则替换全部
来源：http://baike.sjlbkw.cn/Article/details/gmpzkinzb.sHtML

s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gedbuleer.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.yfazqb.com/Article/details/ggcrrayzv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.epnwcf.com/Article/details/gbfaltnuj.sHtML

[U115] JS：生成 UUID
来源：http://mobile.bbcook.cn/Article/details/gvejkplcd.sHtML

crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/gglfsgsuh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.epnwcf.com/Article/details/gniopkwan.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.tarul.cn/Article/details/gsbaparfx.sHtML

[U117] JS：单元测试
来源：http://baike.sjlbkw.cn/Article/details/gjryciinm.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.epnwcf.com/Article/details/gwggsagtu.sHtML

[U118] JS：开发服务器
来源：http://read.share.vehdjk.com/Article/details/giwltdhbo.sHtML

npm i -D vite;  npx vite
来源：http://mobile.epnwcf.com/Article/details/gghjvlhkw.sHtML

[U119] JS：生产构建
来源：http://m.share.tarul.cn/Article/details/gkqybkewa.sHtML

npx vite build
来源：http://www.m.share.vehdjk.com/Article/details/gcfxgycma.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.yfazqb.com/Article/details/gareixzix.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.bbcook.cn/Article/details/gyetsujti.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/glkmmnjmr.sHtML

统计汇总
来源：http://mobile.epnwcf.com/Article/details/ghaiaedeo.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gclgqlfcs.sHtML

按语言统计（条）：
来源：http://read.share.tarul.cn/Article/details/gbhfyzxkn.sHtML

Python ......... 252
来源：http://www.share.bbcook.cn/Article/details/gdnkvjyok.sHtML

PHP ............ 252
来源：http://baike.fktsv.cn/Article/details/gidntvlwe.sHtML

JavaScript ..... 252
来源：http://3g.vehdjk.com/Article/details/gscwiskhl.sHtML

TypeScript ..... 212
来源：http://baike.fktsv.cn/Article/details/glkotrusw.sHtML

Java ........... 212
来源：http://www.share.vehdjk.com/Article/details/gcdyepfom.sHtML

Go ............. 212
来源：http://read.share.fktsv.cn/Article/details/gltcxbiyk.sHtML

Ruby ........... 212
来源：http://www.blog.bbcook.cn/Article/details/gzdevjlif.sHtML

C# ............. 212
来源：http://mobile.fktsv.cn/Article/details/gnuhohnir.sHtML

C .............. 30
来源：http://3g.tarul.cn/Article/details/gzziwhyml.sHtML

C++ ............ 30
来源：http://mobile.epnwcf.com/Article/details/gcrlulcfp.sHtML

SQL ............ 90
来源：http://blog.epnwcf.com/Article/details/gazqztytz.sHtML

Bash ........... 80
来源：http://baike.bbcook.cn/Article/details/giagwmgvn.sHtML

Kotlin ......... 15
来源：http://m.share.bbcook.cn/Article/details/gvrxsqpns.sHtML

Swift .......... 15
来源：http://www.m.share.epnwcf.com/Article/details/gyqmqoplt.sHtML

Lua ............ 10
来源：http://baike.sjlbkw.cn/Article/details/gzaqsywcz.sHtML

Perl ........... 10
来源：http://mobile.fktsv.cn/Article/details/gxdryrcnf.sHtML

Scala .......... 10
来源：http://wap.epnwcf.com/Article/details/gzndsvuxe.sHtML

------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gvdtkqzry.sHtML

合计 ........... 2106 条
来源：http://wap.bbcook.cn/Article/details/gijifgang.sHtML

按章节统计：
来源：http://read.share.sjlbkw.cn/Article/details/gnqnbqjyt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.tarul.cn/Article/details/gzxykzcuc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.epnwcf.com/Article/details/ghgpxipsi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.yfazqb.com/Article/details/gclohiwdt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fktsv.cn/Article/details/grfcfyzqq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.epnwcf.com/Article/details/gwlpjbcwk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.vehdjk.com/Article/details/gwkjzzgfd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.bbcook.cn/Article/details/gslnlalnp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.vehdjk.com/Article/details/gvjajqxlt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/gctohzdeg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.bbcook.cn/Article/details/gksmgnyeq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gkhnowwwu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gndoezemc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gwbhjtlbf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.epnwcf.com/Article/details/grzgxvrtp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.sjlbkw.cn/Article/details/gzhewxgsr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gtsvcrlpb.sHtML

Q SQL 专题                              90
来源：http://www.m.share.yfazqb.com/Article/details/gpondvgap.sHtML

R Bash 专题                             80
来源：http://baike.tarul.cn/Article/details/gpdqzqbjx.sHtML

S C / C++ 专题                          60
来源：http://baike.sjlbkw.cn/Article/details/gliyghyyx.sHtML

T 其他语言补充                          60
来源：http://www.share.epnwcf.com/Article/details/gpegpodxz.sHtML

U 高频实用片段                         120
来源：http://baike.epnwcf.com/Article/details/gdkandxsg.sHtML

------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/grabaauhe.sHtML

合计                                  2106 条
来源：http://blog.tarul.cn/Article/details/gjldanepz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fktsv.cn/Article/details/gfeswmrly.sHtML

使用提醒
来源：http://read.share.yfazqb.com/Article/details/gihykphky.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/ggutmvxiw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.vehdjk.com/Article/details/gvyqczimu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.yfazqb.com/Article/details/gcbmnvgxj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.tarul.cn/Article/details/gnqwsexph.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgfsfaoi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fktsv.cn/Article/details/goucxosip.sHtML

—— 文件结束 ——
来源：http://3g.sjlbkw.cn/Article/details/gpbaxpkij.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ghzkjtxqy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fktsv.cn/Article/details/gsepseigm.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fktsv.cn/Article/details/gwaloirpk.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gkfnthojs.sHtML

【收录内容】
来源：http://www.share.fktsv.cn/Article/details/grvjdczwr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.tarul.cn/Article/details/ggexsmikp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrkxzbhu.sHtML

SQL · Bash · C · C++
来源：http://3g.fktsv.cn/Article/details/gwefbjfjg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.sjlbkw.cn/Article/details/grbkssoda.sHtML

【使用说明】
来源：http://baike.epnwcf.com/Article/details/glsykdhbh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.epnwcf.com/Article/details/gnofiiysv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.bbcook.cn/Article/details/grvhfbfhh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fktsv.cn/Article/details/gmawwxojg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fktsv.cn/Article/details/gpzumuytl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.epnwcf.com/Article/details/gthzxmulk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fktsv.cn/Article/details/gexinjfaf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.tarul.cn/Article/details/gnubencrs.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.bbcook.cn/Article/details/gmsbpzvkp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fktsv.cn/Article/details/gvjtzifmj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.tarul.cn/Article/details/gnnkwxpzu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.vehdjk.com/Article/details/gnmlflxtm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.epnwcf.com/Article/details/gnluwkamh.sHtML

【文件统计】
来源：http://wap.fktsv.cn/Article/details/gisygwmhm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.bbcook.cn/Article/details/grashtzzq.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gmxxgqlgw.sHtML

目  录
来源：http://www.share.yfazqb.com/Article/details/gvmvduboq.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/gkrdrrzwm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.bbcook.cn/Article/details/gcupseprn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.vehdjk.com/Article/details/ggioqdzpr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.yfazqb.com/Article/details/gdoxqacce.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.epnwcf.com/Article/details/gcgbmjsly.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.tarul.cn/Article/details/gqcbuhjti.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.yfazqb.com/Article/details/ggiaozwii.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.tarul.cn/Article/details/govmbzxdo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.vehdjk.com/Article/details/gaicvyegl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/guuknclnz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.epnwcf.com/Article/details/gibqfdikt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/gkxezpkna.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/ganhgdqdt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/gmbqhulwa.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.sjlbkw.cn/Article/details/gfritfsgi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.vehdjk.com/Article/details/gjgvinpxx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.yfazqb.com/Article/details/gnjrbtvwv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fktsv.cn/Article/details/gnggzktti.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.sjlbkw.cn/Article/details/gufzaopzr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.vehdjk.com/Article/details/gsibsrvsl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.tarul.cn/Article/details/gljtazihg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.epnwcf.com/Article/details/ggdsoeskd.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gdlmomagj.sHtML

A. 基础语法与类型
来源：http://3g.epnwcf.com/Article/details/glqtgicqm.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gegcjyqui.sHtML

[A01] Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gxqmwvqhx.sHtML

Py:   print("Hello, World!")
来源：http://wap.yfazqb.com/Article/details/gsbndtuia.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.yfazqb.com/Article/details/ganoczfvy.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.tarul.cn/Article/details/gyoupbuon.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.bbcook.cn/Article/details/gjlschlcs.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.sjlbkw.cn/Article/details/gchwuzcph.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.tarul.cn/Article/details/gdashxmeb.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.yfazqb.com/Article/details/ghedusais.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.bbcook.cn/Article/details/gmhuzdrpn.sHtML

[A02] 变量声明与赋值
来源：http://blog.yfazqb.com/Article/details/gstuddwci.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.vehdjk.com/Article/details/gzpnbqdnp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.epnwcf.com/Article/details/gdlsasxbf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.epnwcf.com/Article/details/gclailzmu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.tarul.cn/Article/details/gldzamjcy.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gkemkgrzr.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.sjlbkw.cn/Article/details/gttpisnij.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.sjlbkw.cn/Article/details/gchijefci.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.epnwcf.com/Article/details/gzefkqcwd.sHtML

[A03] 常量定义
来源：http://read.share.bbcook.cn/Article/details/gngclrvhb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fktsv.cn/Article/details/gbgvrqkse.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gehkhkxqs.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gbksrhkfm.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gvtjypwut.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gjoaubkpu.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.vehdjk.com/Article/details/gdotcwkhh.sHtML

Ruby: PI = 3.14159
来源：http://m.share.yfazqb.com/Article/details/gpvbwxptp.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/ggpqiysui.sHtML

[A04] 判断变量类型
来源：http://3g.yfazqb.com/Article/details/gvvpomspx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.sjlbkw.cn/Article/details/ghkzihuzu.sHtML


<!-- 参考信息 -->