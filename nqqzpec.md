代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://3g.sjlbkw.cn/Article/details/gomwxtobo.sHtML

sys.stdout.isatty()
来源：http://blog.bbcook.cn/Article/details/gegbsitef.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.tarul.cn/Article/details/gnwentncd.sHtML

print("err", file=sys.stderr)
来源：http://3g.vehdjk.com/Article/details/gpahhcjmn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.bbcook.cn/Article/details/grozqayia.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.epnwcf.com/Article/details/gjbunzkkn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.sjlbkw.cn/Article/details/gpfzfcffo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.epnwcf.com/Article/details/gmnahduaf.sHtML

[U43] PHP：声明命名空间
来源：http://blog.epnwcf.com/Article/details/ggnuvnxqu.sHtML

namespace App\Http;
来源：http://3g.tarul.cn/Article/details/goizwnkfk.sHtML

[U44] PHP：开启严格类型
来源：http://baike.epnwcf.com/Article/details/gwvoeqvrt.sHtML

declare(strict_types=1);
来源：http://blog.fktsv.cn/Article/details/gzdhootsu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.tarul.cn/Article/details/gepymayyf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gqjfmrkgr.sHtML

[U46] PHP：可空类型
来源：http://mobile.fktsv.cn/Article/details/gsrmtwxat.sHtML

?string $name = null
来源：http://m.share.tarul.cn/Article/details/gvbcpdyjl.sHtML

[U47] PHP：联合类型
来源：http://www.share.tarul.cn/Article/details/gavugxhbq.sHtML

int|string $id
来源：http://baike.bbcook.cn/Article/details/gwzhmfevk.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.yfazqb.com/Article/details/gwvjpvwmw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fktsv.cn/Article/details/gjfabsila.sHtML

[U49] PHP：只读属性
来源：http://wap.tarul.cn/Article/details/gtiqotpop.sHtML

public readonly string $name
来源：http://m.share.yfazqb.com/Article/details/grtjahscb.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.yfazqb.com/Article/details/gfyflanvl.sHtML

public function __construct(private int $id) {}
来源：http://baike.vehdjk.com/Article/details/gejkofsiy.sHtML

[U51] PHP：数组解构
来源：http://www.share.epnwcf.com/Article/details/grcabuwou.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcasbpqfg.sHtML

[U52] PHP：箭头函数
来源：http://www.share.tarul.cn/Article/details/gztduxkad.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.epnwcf.com/Article/details/gxdrxmkvy.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.bbcook.cn/Article/details/gxevbvqiy.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.vehdjk.com/Article/details/girspefrx.sHtML

[U54] PHP：空安全调用
来源：http://blog.tarul.cn/Article/details/gotdgwapl.sHtML

$obj?->method()
来源：http://wap.vehdjk.com/Article/details/guawvuwmv.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gxyzawnvu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fktsv.cn/Article/details/golxpnxeq.sHtML

[U56] PHP：命名参数
来源：http://3g.vehdjk.com/Article/details/gtllxvizg.sHtML

f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/gvtyzyzvi.sHtML

[U57] PHP：字符串插值
来源：http://blog.tarul.cn/Article/details/ggmshghzv.sHtML

"值: {$a}"
来源：http://www.m.share.fktsv.cn/Article/details/ghxhvlmba.sHtML

[U58] PHP：数组三件套
来源：http://mobile.vehdjk.com/Article/details/gsxhfaesl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fktsv.cn/Article/details/gtcgdognn.sHtML

[U59] PHP：自定义排序
来源：http://blog.yfazqb.com/Article/details/gzpqxmpts.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fktsv.cn/Article/details/grzxkokbv.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.epnwcf.com/Article/details/glmlqvvdu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.sjlbkw.cn/Article/details/gsdkfvxgn.sHtML

[U61] PHP：正则
来源：http://blog.epnwcf.com/Article/details/gatmhbxgk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.yfazqb.com/Article/details/gfzhvgsie.sHtML

[U62] PHP：日期对象
来源：http://www.share.epnwcf.com/Article/details/gepkucuil.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.yfazqb.com/Article/details/ghujijnjz.sHtML

[U63] PHP：文件读写
来源：http://mobile.sjlbkw.cn/Article/details/gijpqeygt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.epnwcf.com/Article/details/gwixytbuv.sHtML

[U64] PHP：目录遍历
来源：http://m.share.bbcook.cn/Article/details/gsveflyed.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fktsv.cn/Article/details/gdmzkcfrp.sHtML

[U65] PHP：会话
来源：http://blog.sjlbkw.cn/Article/details/gooirzmmf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.bbcook.cn/Article/details/gksgfamqz.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fktsv.cn/Article/details/gluwhvmqi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpqedjjv.sHtML

[U67] PHP：处理文件上传
来源：http://blog.epnwcf.com/Article/details/gaazcgqpp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.sjlbkw.cn/Article/details/ggccrwmul.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.epnwcf.com/Article/details/giueuhkpc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.epnwcf.com/Article/details/geucnvvrw.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.sjlbkw.cn/Article/details/gmknsjoxu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.epnwcf.com/Article/details/gnpoagtjy.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.bbcook.cn/Article/details/guhqyuicw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fktsv.cn/Article/details/gotumzsrq.sHtML

[U71] PHP：抛出异常
来源：http://blog.epnwcf.com/Article/details/gsexewmov.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.tarul.cn/Article/details/gqyrxgfqk.sHtML

[U72] PHP：写错误日志
来源：http://wap.bbcook.cn/Article/details/gexywmchu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.tarul.cn/Article/details/gzssklsrm.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fktsv.cn/Article/details/giuvubatb.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.yfazqb.com/Article/details/gradkxexd.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.tarul.cn/Article/details/grvoqyrpj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.vehdjk.com/Article/details/giybbdjic.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.bbcook.cn/Article/details/gfaincmyw.sHtML

composer require psr/container
来源：http://3g.epnwcf.com/Article/details/gswelybjh.sHtML

[U76] PHP：简单路由
来源：http://wap.bbcook.cn/Article/details/gmqkdezhq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.vehdjk.com/Article/details/gokzvlcka.sHtML

[U77] PHP：模板渲染
来源：http://mobile.sjlbkw.cn/Article/details/gecytjtoj.sHtML

composer require twig/twig
来源：http://www.m.share.fktsv.cn/Article/details/gxptqzlbx.sHtML

[U78] PHP：单元测试
来源：http://blog.fktsv.cn/Article/details/givqxmfpy.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.epnwcf.com/Article/details/grtjonmgq.sHtML

[U79] PHP：静态分析
来源：http://m.share.epnwcf.com/Article/details/gbfbtjndg.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.tarul.cn/Article/details/gdqlfevjr.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.tarul.cn/Article/details/guvkasein.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.sjlbkw.cn/Article/details/gntbswuzc.sHtML

[U81] JS：初始化项目
来源：http://www.blog.bbcook.cn/Article/details/gxcmmajdf.sHtML

npm init -y;  npm i express
来源：http://read.share.yfazqb.com/Article/details/gpjyxized.sHtML

[U82] JS：package.json 脚本
来源：http://3g.epnwcf.com/Article/details/gagmfanmc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.epnwcf.com/Article/details/gtlgvechp.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.yfazqb.com/Article/details/gqpokkntp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.epnwcf.com/Article/details/gprmwzazf.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fktsv.cn/Article/details/gmbdskiug.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.tarul.cn/Article/details/guupvyfus.sHtML

[U85] JS：可选链
来源：http://read.share.tarul.cn/Article/details/geffxedbt.sHtML

a?.b?.c
来源：http://www.blog.tarul.cn/Article/details/gvwqctuku.sHtML

[U86] JS：空值合并
来源：http://baike.vehdjk.com/Article/details/gnjsyjuwx.sHtML

a ?? b
来源：http://blog.tarul.cn/Article/details/gahvwdrcm.sHtML

[U87] JS：解构默认值
来源：http://www.share.bbcook.cn/Article/details/gppcgbzmn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.vehdjk.com/Article/details/gifbdppxk.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.epnwcf.com/Article/details/gjetbkukv.sHtML

{ ...a, ...b }
来源：http://m.share.fktsv.cn/Article/details/gsnmolqby.sHtML

[U89] JS：数组去重
来源：http://baike.vehdjk.com/Article/details/gjjyuaqjy.sHtML

[...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gsygxqzob.sHtML

[U90] JS：数字数组排序
来源：http://wap.tarul.cn/Article/details/gjnkvenst.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gbqicdznf.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.tarul.cn/Article/details/gjtmansgc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.epnwcf.com/Article/details/gfpnqnemu.sHtML

[U92] JS：深拷贝
来源：http://blog.fktsv.cn/Article/details/guhjyjofj.sHtML

structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gzjzpxoqg.sHtML

[U93] JS：模板字符串
来源：http://wap.epnwcf.com/Article/details/giipxxgvq.sHtML

`共 ${n} 条`
来源：http://wap.yfazqb.com/Article/details/ggfitkwhi.sHtML

[U94] JS：箭头函数
来源：http://read.share.yfazqb.com/Article/details/gzeuaoyzr.sHtML

const double = x => x * 2;
来源：http://www.blog.epnwcf.com/Article/details/gtlrfwxwf.sHtML

[U95] JS：Promise 包装
来源：http://blog.epnwcf.com/Article/details/gbwagnxch.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.bbcook.cn/Article/details/gmvkzclfn.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.epnwcf.com/Article/details/ggujolhpj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/glfbxixth.sHtML

[U97] JS：并发请求
来源：http://read.share.tarul.cn/Article/details/goleyrvnj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gmlkqlgnn.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.sjlbkw.cn/Article/details/gcwgyjgbd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fktsv.cn/Article/details/gxsfnyjxi.sHtML

[U99] JS：事件监听
来源：http://blog.tarul.cn/Article/details/gxfauuhtk.sHtML

el.addEventListener("click", e => {})
来源：http://3g.sjlbkw.cn/Article/details/gyyjnhdlc.sHtML

[U100] JS：DOM 查询
来源：http://www.share.bbcook.cn/Article/details/gmytrsnta.sHtML

document.querySelector(".item")
来源：http://read.share.bbcook.cn/Article/details/geqfbcdfb.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fktsv.cn/Article/details/gzwrryxlm.sHtML

el.classList.toggle("active")
来源：http://wap.fktsv.cn/Article/details/gssabbzoa.sHtML

[U102] JS：本地存储
来源：http://baike.epnwcf.com/Article/details/gcvbgrwbu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.vehdjk.com/Article/details/gdsrrszui.sHtML

[U103] JS：定时器
来源：http://wap.epnwcf.com/Article/details/gfhvcqjrb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.vehdjk.com/Article/details/gqjtghbkj.sHtML

[U104] JS：防抖
来源：http://www.m.share.bbcook.cn/Article/details/gasgyunze.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/gmpbldkdq.sHtML

[U105] JS：节流
来源：http://www.blog.sjlbkw.cn/Article/details/ghfslzdbm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fktsv.cn/Article/details/gfafrkvqu.sHtML

[U106] JS：日期格式化
来源：http://www.share.bbcook.cn/Article/details/gqvssrrqo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.sjlbkw.cn/Article/details/grmbnqlwv.sHtML

[U107] JS：数字千分位
来源：http://read.share.tarul.cn/Article/details/grwagqkzt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.sjlbkw.cn/Article/details/gswoqfpsy.sHtML

[U108] JS：随机整数
来源：http://www.blog.tarul.cn/Article/details/gegtodrmp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.sjlbkw.cn/Article/details/gewjfipzi.sHtML

[U109] JS：数组分组
来源：http://read.share.bbcook.cn/Article/details/ggvbyhpcz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.sjlbkw.cn/Article/details/gysawxeis.sHtML

[U110] JS：数组分块
来源：http://baike.sjlbkw.cn/Article/details/greixwjtq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fktsv.cn/Article/details/gemsdhugs.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fktsv.cn/Article/details/gmeaxhrwh.sHtML

new Map(Object.entries(obj))
来源：http://3g.epnwcf.com/Article/details/guebgnwcz.sHtML

[U112] JS：字符串补位
来源：http://wap.epnwcf.com/Article/details/gjmrecyht.sHtML

"7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/ganbbhnxj.sHtML

[U113] JS：正则替换全部
来源：http://mobile.bbcook.cn/Article/details/gfhajmxmn.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/ganuwayqr.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fktsv.cn/Article/details/ghzeiehil.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.epnwcf.com/Article/details/gzxgxtivj.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fktsv.cn/Article/details/ggoexowxn.sHtML

crypto.randomUUID()
来源：http://www.m.share.fktsv.cn/Article/details/gfuznhuve.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.sjlbkw.cn/Article/details/gjmhvkkwl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fktsv.cn/Article/details/gxmxvmfoj.sHtML

[U117] JS：单元测试
来源：http://www.share.epnwcf.com/Article/details/gbdkembgf.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.yfazqb.com/Article/details/ghwhcjawf.sHtML

[U118] JS：开发服务器
来源：http://blog.epnwcf.com/Article/details/gkcuykxcs.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.bbcook.cn/Article/details/gkyinmzdp.sHtML

[U119] JS：生产构建
来源：http://mobile.bbcook.cn/Article/details/gsnjuxtha.sHtML

npx vite build
来源：http://m.share.yfazqb.com/Article/details/gpzmskbrr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.epnwcf.com/Article/details/gzsdfbtnp.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.yfazqb.com/Article/details/grovqbfxi.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gjalldjds.sHtML

统计汇总
来源：http://www.share.yfazqb.com/Article/details/gujgmwius.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gpakwydmc.sHtML

按语言统计（条）：
来源：http://www.blog.fktsv.cn/Article/details/goosgrhzk.sHtML

Python ......... 252
来源：http://www.m.share.bbcook.cn/Article/details/gcuwkfefx.sHtML

PHP ............ 252
来源：http://m.share.fktsv.cn/Article/details/ggalqjsaw.sHtML

JavaScript ..... 252
来源：http://blog.bbcook.cn/Article/details/gkfxdsoqs.sHtML

TypeScript ..... 212
来源：http://blog.yfazqb.com/Article/details/gnifrqbxg.sHtML

Java ........... 212
来源：http://read.share.yfazqb.com/Article/details/gxaaihoyz.sHtML

Go ............. 212
来源：http://www.blog.tarul.cn/Article/details/ghnnupxvr.sHtML

Ruby ........... 212
来源：http://mobile.epnwcf.com/Article/details/gudjhlhvn.sHtML

C# ............. 212
来源：http://www.blog.yfazqb.com/Article/details/glmgcktrw.sHtML

C .............. 30
来源：http://3g.epnwcf.com/Article/details/gyfnkleqc.sHtML

C++ ............ 30
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcfepljy.sHtML

SQL ............ 90
来源：http://www.m.share.sjlbkw.cn/Article/details/gvieqkknc.sHtML

Bash ........... 80
来源：http://www.share.sjlbkw.cn/Article/details/giqornsdl.sHtML

Kotlin ......... 15
来源：http://m.share.fktsv.cn/Article/details/gimsbowjh.sHtML

Swift .......... 15
来源：http://wap.vehdjk.com/Article/details/gtrwdpivb.sHtML

Lua ............ 10
来源：http://read.share.bbcook.cn/Article/details/gpppzvwma.sHtML

Perl ........... 10
来源：http://read.share.vehdjk.com/Article/details/gllwvosxt.sHtML

Scala .......... 10
来源：http://www.m.share.bbcook.cn/Article/details/gmkyvbbox.sHtML

------------------------------------
来源：http://wap.fktsv.cn/Article/details/gzigeirlz.sHtML

合计 ........... 2106 条
来源：http://wap.epnwcf.com/Article/details/gdjchvhrx.sHtML

按章节统计：
来源：http://baike.tarul.cn/Article/details/gtgwxnpsg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.yfazqb.com/Article/details/glazytssz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.vehdjk.com/Article/details/ghvmdboyi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.yfazqb.com/Article/details/gxbfxbqbm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.tarul.cn/Article/details/geotftico.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.tarul.cn/Article/details/gdkrrciql.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fktsv.cn/Article/details/gxyhnxwzz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fktsv.cn/Article/details/gvsqnhirj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.tarul.cn/Article/details/gzkunsnhh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gyrdfpssy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fktsv.cn/Article/details/gezrudykp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/guvgcvpev.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/godnomlmo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gmtpocngq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.vehdjk.com/Article/details/gvofbjoxu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.epnwcf.com/Article/details/gpxubpeqt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/gakmsftkh.sHtML

Q SQL 专题                              90
来源：http://www.blog.fktsv.cn/Article/details/gyghgxdfi.sHtML

R Bash 专题                             80
来源：http://blog.yfazqb.com/Article/details/gcdfshsis.sHtML

S C / C++ 专题                          60
来源：http://www.blog.epnwcf.com/Article/details/gxscwtkrp.sHtML

T 其他语言补充                          60
来源：http://www.m.share.bbcook.cn/Article/details/ghcolowdq.sHtML

U 高频实用片段                         120
来源：http://www.share.fktsv.cn/Article/details/gkpobfauk.sHtML

------------------------------------
来源：http://baike.fktsv.cn/Article/details/gzvjxomwz.sHtML

合计                                  2106 条
来源：http://baike.epnwcf.com/Article/details/giffkpscu.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/glrfnrzat.sHtML

使用提醒
来源：http://read.share.tarul.cn/Article/details/gejbyhvwc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/gtvfvbrak.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.sjlbkw.cn/Article/details/gwniayull.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.tarul.cn/Article/details/gbupfbmkf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.vehdjk.com/Article/details/gsqfjhknn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.yfazqb.com/Article/details/gfmnpcbsp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.tarul.cn/Article/details/glzptbito.sHtML

—— 文件结束 ——
来源：http://www.blog.vehdjk.com/Article/details/gnkbxamob.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gkblpupya.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.epnwcf.com/Article/details/gxudqhuiu.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fktsv.cn/Article/details/giuvqpite.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gintigfyj.sHtML

【收录内容】
来源：http://www.blog.bbcook.cn/Article/details/ghyubczop.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.vehdjk.com/Article/details/gnxsytyud.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fktsv.cn/Article/details/gifrhltdv.sHtML

SQL · Bash · C · C++
来源：http://baike.fktsv.cn/Article/details/gkskzkkqq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.tarul.cn/Article/details/gdoingbhk.sHtML

【使用说明】
来源：http://m.share.vehdjk.com/Article/details/givdfcufy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.bbcook.cn/Article/details/gyafvccpz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.bbcook.cn/Article/details/gtoqwxdqy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.sjlbkw.cn/Article/details/gbzioasop.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.sjlbkw.cn/Article/details/ggpairoqq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.bbcook.cn/Article/details/gozemdvdq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.yfazqb.com/Article/details/gjtzhejot.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fktsv.cn/Article/details/gwpvlpxtx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.yfazqb.com/Article/details/gnveinpwz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fktsv.cn/Article/details/gyiwdcmya.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.vehdjk.com/Article/details/gdanboajv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.sjlbkw.cn/Article/details/gavzjttxg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.vehdjk.com/Article/details/gjkqlbcmq.sHtML

【文件统计】
来源：http://3g.yfazqb.com/Article/details/gazamezbz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.bbcook.cn/Article/details/gmakppvlg.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gvugnpjlg.sHtML

目  录
来源：http://blog.fktsv.cn/Article/details/ghjkxbkxx.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/gwnpbwdva.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.tarul.cn/Article/details/gecxpfctx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fktsv.cn/Article/details/gacohpcfq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.vehdjk.com/Article/details/ggicjndwc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.vehdjk.com/Article/details/gocypdeby.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.vehdjk.com/Article/details/gunatqjqg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.sjlbkw.cn/Article/details/gfucpsppc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.sjlbkw.cn/Article/details/gtinhpggx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.tarul.cn/Article/details/gdfiizjau.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/gdyhakxkm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.yfazqb.com/Article/details/gurfdcvth.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gevburihk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.sjlbkw.cn/Article/details/gapnrpnhl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.vehdjk.com/Article/details/gegpuchwk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.vehdjk.com/Article/details/ghlfotnfs.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.sjlbkw.cn/Article/details/gfkqwqjtb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gllyoritu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.sjlbkw.cn/Article/details/gkbdzkjpp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.tarul.cn/Article/details/gcwevnohi.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fktsv.cn/Article/details/ghowtahus.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/ggdykkegj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.bbcook.cn/Article/details/gxtdldsfb.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gmqbnmnfw.sHtML

A. 基础语法与类型
来源：http://wap.epnwcf.com/Article/details/gmscyavrk.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gbwjjoxlh.sHtML

[A01] Hello World
来源：http://3g.vehdjk.com/Article/details/gozpbivld.sHtML

Py:   print("Hello, World!")
来源：http://3g.tarul.cn/Article/details/gbpmswtow.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.yfazqb.com/Article/details/gnryoombi.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.tarul.cn/Article/details/gpnjwprkz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.tarul.cn/Article/details/gamemaytl.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fktsv.cn/Article/details/gvioslnsr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.tarul.cn/Article/details/gezzwnhdb.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.tarul.cn/Article/details/gyhwehaam.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fktsv.cn/Article/details/gsvbzxuqp.sHtML

[A02] 变量声明与赋值
来源：http://www.share.epnwcf.com/Article/details/gcizqkdch.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.yfazqb.com/Article/details/gvavhqhkr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.sjlbkw.cn/Article/details/glxejhmmy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.epnwcf.com/Article/details/graupbdqq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.bbcook.cn/Article/details/gljfbhsha.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.yfazqb.com/Article/details/gtcundnlu.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fktsv.cn/Article/details/gfcduydps.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.tarul.cn/Article/details/gewfbzqma.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.vehdjk.com/Article/details/gkymuqsye.sHtML

[A03] 常量定义
来源：http://www.blog.bbcook.cn/Article/details/gqhwjmdfk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.epnwcf.com/Article/details/gqrcwyytb.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fktsv.cn/Article/details/getnyvvrc.sHtML

JS:   const PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gumysjzxb.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gugtjxlha.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gwttzasml.sHtML

Go:   const PI = 3.14159
来源：http://blog.bbcook.cn/Article/details/gezjbobxc.sHtML

Ruby: PI = 3.14159
来源：http://m.share.vehdjk.com/Article/details/gmxopkjui.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gktzldsuq.sHtML

[A04] 判断变量类型
来源：http://www.share.vehdjk.com/Article/details/gkhqfvcud.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.sjlbkw.cn/Article/details/gwwxrzljg.sHtML


<!-- 参考信息 -->