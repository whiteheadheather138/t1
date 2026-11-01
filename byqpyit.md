代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.m.share.vehdjk.com/Article/details/ggnkatjrl.sHtML

sys.stdout.isatty()
来源：http://blog.fktsv.cn/Article/details/gfmbdmuav.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.yfazqb.com/Article/details/ghzvvwiek.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.sjlbkw.cn/Article/details/gyioztysw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.vehdjk.com/Article/details/ghvyyidaj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.vehdjk.com/Article/details/gtotrflaf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.yfazqb.com/Article/details/gzjlrrdlo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.bbcook.cn/Article/details/galjqhcen.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fktsv.cn/Article/details/gchqbywgo.sHtML

namespace App\Http;
来源：http://wap.tarul.cn/Article/details/ggewdkkzq.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.sjlbkw.cn/Article/details/gntljhdtb.sHtML

declare(strict_types=1);
来源：http://read.share.fktsv.cn/Article/details/gqajgvmhn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.epnwcf.com/Article/details/ghocnlemp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gyddjadpa.sHtML

[U46] PHP：可空类型
来源：http://blog.epnwcf.com/Article/details/gomnowser.sHtML

?string $name = null
来源：http://blog.tarul.cn/Article/details/gsdxiguie.sHtML

[U47] PHP：联合类型
来源：http://3g.epnwcf.com/Article/details/gkjsepzap.sHtML

int|string $id
来源：http://www.m.share.vehdjk.com/Article/details/gcmvepdhd.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.epnwcf.com/Article/details/guddohors.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.vehdjk.com/Article/details/gsrqtsshu.sHtML

[U49] PHP：只读属性
来源：http://read.share.tarul.cn/Article/details/grrrplljw.sHtML

public readonly string $name
来源：http://m.share.yfazqb.com/Article/details/gxkxadzko.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.vehdjk.com/Article/details/gaewmgzmp.sHtML

public function __construct(private int $id) {}
来源：http://www.share.yfazqb.com/Article/details/gatckewvi.sHtML

[U51] PHP：数组解构
来源：http://baike.epnwcf.com/Article/details/gfobmvheb.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.vehdjk.com/Article/details/gvmwjmcai.sHtML

[U52] PHP：箭头函数
来源：http://m.share.epnwcf.com/Article/details/gxnjowqvn.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.tarul.cn/Article/details/gsjiqhlhc.sHtML

[U53] PHP：空合并运算符
来源：http://blog.tarul.cn/Article/details/gcedkpwwb.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.yfazqb.com/Article/details/gmmlxderh.sHtML

[U54] PHP：空安全调用
来源：http://blog.fktsv.cn/Article/details/gymcyzbiw.sHtML

$obj?->method()
来源：http://blog.fktsv.cn/Article/details/gbejkcbsg.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.yfazqb.com/Article/details/gkzkzitqf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fktsv.cn/Article/details/gcqwnwvoi.sHtML

[U56] PHP：命名参数
来源：http://mobile.epnwcf.com/Article/details/gggsasjku.sHtML

f(a: 1, b: 2)
来源：http://m.share.vehdjk.com/Article/details/gghkwlptf.sHtML

[U57] PHP：字符串插值
来源：http://blog.vehdjk.com/Article/details/gjqvqrdix.sHtML

"值: {$a}"
来源：http://m.share.sjlbkw.cn/Article/details/gbvimbvzt.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.tarul.cn/Article/details/gxtzgybec.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.tarul.cn/Article/details/gzprzoqfp.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fktsv.cn/Article/details/gbevhfdyk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fktsv.cn/Article/details/glvfzvnxi.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.sjlbkw.cn/Article/details/gnzxmtkdw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.yfazqb.com/Article/details/gsxshmfts.sHtML

[U61] PHP：正则
来源：http://read.share.yfazqb.com/Article/details/gascscdqo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fktsv.cn/Article/details/gvoalhyor.sHtML

[U62] PHP：日期对象
来源：http://mobile.tarul.cn/Article/details/gubjvpdsv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.vehdjk.com/Article/details/gymfjqjxq.sHtML

[U63] PHP：文件读写
来源：http://read.share.vehdjk.com/Article/details/graylvugg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.yfazqb.com/Article/details/gffloiybf.sHtML

[U64] PHP：目录遍历
来源：http://read.share.vehdjk.com/Article/details/gejnzzedc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.sjlbkw.cn/Article/details/glrpqqgwr.sHtML

[U65] PHP：会话
来源：http://m.share.fktsv.cn/Article/details/grhkaesoi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.tarul.cn/Article/details/gfozrthxd.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.sjlbkw.cn/Article/details/ggdrrxhzg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.yfazqb.com/Article/details/gffqavsjc.sHtML

[U67] PHP：处理文件上传
来源：http://baike.vehdjk.com/Article/details/gbolmdbrb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.sjlbkw.cn/Article/details/gabpojmvn.sHtML

[U68] PHP：PDO 连接
来源：http://3g.bbcook.cn/Article/details/gwdxqanws.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.sjlbkw.cn/Article/details/ggspokenh.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.bbcook.cn/Article/details/gwxvpslbc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.yfazqb.com/Article/details/ghijmqvsu.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.bbcook.cn/Article/details/gvnmadcde.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.yfazqb.com/Article/details/graxpdhwc.sHtML

[U71] PHP：抛出异常
来源：http://mobile.vehdjk.com/Article/details/gqvgqkmmk.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.tarul.cn/Article/details/gftdbirny.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.sjlbkw.cn/Article/details/guybllpwi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fktsv.cn/Article/details/ghevjqcgd.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.yfazqb.com/Article/details/gpqhxokev.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.tarul.cn/Article/details/gdowycyjb.sHtML

[U74] PHP：读取环境变量
来源：http://baike.epnwcf.com/Article/details/gtzocildz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.bbcook.cn/Article/details/gmekzydzq.sHtML

[U75] PHP：依赖注入
来源：http://wap.yfazqb.com/Article/details/gzumyhmka.sHtML

composer require psr/container
来源：http://baike.bbcook.cn/Article/details/gsykulmvr.sHtML

[U76] PHP：简单路由
来源：http://mobile.bbcook.cn/Article/details/gndkkyafc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.vehdjk.com/Article/details/gxolciqyr.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsadotnl.sHtML

composer require twig/twig
来源：http://m.share.sjlbkw.cn/Article/details/gzjlzfjrj.sHtML

[U78] PHP：单元测试
来源：http://wap.tarul.cn/Article/details/gywtqosfv.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.vehdjk.com/Article/details/gtmqsejyi.sHtML

[U79] PHP：静态分析
来源：http://read.share.bbcook.cn/Article/details/gzmoeojsw.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.epnwcf.com/Article/details/gyddqdvqk.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fktsv.cn/Article/details/gpbdqysld.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fktsv.cn/Article/details/guhpmgxoi.sHtML

[U81] JS：初始化项目
来源：http://mobile.vehdjk.com/Article/details/giedjonpb.sHtML

npm init -y;  npm i express
来源：http://m.share.fktsv.cn/Article/details/gljiwkuds.sHtML

[U82] JS：package.json 脚本
来源：http://3g.bbcook.cn/Article/details/gkxkkbgyg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.bbcook.cn/Article/details/gwxebfmng.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.vehdjk.com/Article/details/gjkelqlgl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.epnwcf.com/Article/details/gcbjmsfyr.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.bbcook.cn/Article/details/gguevjphh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.vehdjk.com/Article/details/glliuydhn.sHtML

[U85] JS：可选链
来源：http://wap.tarul.cn/Article/details/ghsgqjoha.sHtML

a?.b?.c
来源：http://www.m.share.fktsv.cn/Article/details/gyjavdetw.sHtML

[U86] JS：空值合并
来源：http://m.share.tarul.cn/Article/details/ggcwsdikt.sHtML

a ?? b
来源：http://baike.epnwcf.com/Article/details/gttelimwe.sHtML

[U87] JS：解构默认值
来源：http://www.share.epnwcf.com/Article/details/goegbeiiv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.vehdjk.com/Article/details/glrkeleiy.sHtML

[U88] JS：对象展开合并
来源：http://www.share.tarul.cn/Article/details/gptyalpus.sHtML

{ ...a, ...b }
来源：http://m.share.epnwcf.com/Article/details/gudsscjsd.sHtML

[U89] JS：数组去重
来源：http://www.share.tarul.cn/Article/details/gfvqtmjex.sHtML

[...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdjrgrkp.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fktsv.cn/Article/details/gvmofumty.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gscqwgmku.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.vehdjk.com/Article/details/gkpnjglop.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.epnwcf.com/Article/details/gcrolispd.sHtML

[U92] JS：深拷贝
来源：http://blog.tarul.cn/Article/details/goepzfdtt.sHtML

structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gbejvmgjc.sHtML

[U93] JS：模板字符串
来源：http://3g.tarul.cn/Article/details/gedacfoxw.sHtML

`共 ${n} 条`
来源：http://wap.sjlbkw.cn/Article/details/ghndnszlf.sHtML

[U94] JS：箭头函数
来源：http://www.blog.yfazqb.com/Article/details/giouticmw.sHtML

const double = x => x * 2;
来源：http://3g.yfazqb.com/Article/details/gpczxazdr.sHtML

[U95] JS：Promise 包装
来源：http://m.share.vehdjk.com/Article/details/gczxybewc.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.bbcook.cn/Article/details/gpfgsyzqq.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fktsv.cn/Article/details/gmesctaea.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/ghwsndljn.sHtML

[U97] JS：并发请求
来源：http://3g.sjlbkw.cn/Article/details/gshxdjmxm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gdntdgzmb.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.yfazqb.com/Article/details/grvrmdxvu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.yfazqb.com/Article/details/gbccbnnuh.sHtML

[U99] JS：事件监听
来源：http://blog.epnwcf.com/Article/details/gvrywlqlp.sHtML

el.addEventListener("click", e => {})
来源：http://3g.tarul.cn/Article/details/gjxtsygej.sHtML

[U100] JS：DOM 查询
来源：http://mobile.vehdjk.com/Article/details/ggqebohfc.sHtML

document.querySelector(".item")
来源：http://www.m.share.epnwcf.com/Article/details/gxutzqzcd.sHtML

[U101] JS：classList 操作
来源：http://read.share.bbcook.cn/Article/details/gelrdtbbp.sHtML

el.classList.toggle("active")
来源：http://3g.fktsv.cn/Article/details/gvsnwdoap.sHtML

[U102] JS：本地存储
来源：http://www.blog.fktsv.cn/Article/details/gtnlgdpvv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fktsv.cn/Article/details/gddkadqci.sHtML

[U103] JS：定时器
来源：http://blog.epnwcf.com/Article/details/gemukogux.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.yfazqb.com/Article/details/gsiqoekqq.sHtML

[U104] JS：防抖
来源：http://www.blog.epnwcf.com/Article/details/gfzvotmeg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gitshxisk.sHtML

[U105] JS：节流
来源：http://wap.fktsv.cn/Article/details/ggniewisl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.sjlbkw.cn/Article/details/goopvkjkz.sHtML

[U106] JS：日期格式化
来源：http://baike.fktsv.cn/Article/details/gciukvxjw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.sjlbkw.cn/Article/details/gprfepcem.sHtML

[U107] JS：数字千分位
来源：http://baike.bbcook.cn/Article/details/gzslkyjxo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.tarul.cn/Article/details/gircqnvfe.sHtML

[U108] JS：随机整数
来源：http://www.m.share.yfazqb.com/Article/details/gjdluzxib.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.vehdjk.com/Article/details/gszlaugsa.sHtML

[U109] JS：数组分组
来源：http://www.share.epnwcf.com/Article/details/gogoyjjte.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.vehdjk.com/Article/details/gqwmarumj.sHtML

[U110] JS：数组分块
来源：http://www.share.tarul.cn/Article/details/gogrltgzh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.tarul.cn/Article/details/gmuwojlgn.sHtML

[U111] JS：对象转 Map
来源：http://read.share.sjlbkw.cn/Article/details/gbuyxhplh.sHtML

new Map(Object.entries(obj))
来源：http://wap.epnwcf.com/Article/details/gqdczoegy.sHtML

[U112] JS：字符串补位
来源：http://wap.vehdjk.com/Article/details/gmadfsihd.sHtML

"7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gpspqchkf.sHtML

[U113] JS：正则替换全部
来源：http://www.share.yfazqb.com/Article/details/gqbipmnlc.sHtML

s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gvsnqaffd.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.tarul.cn/Article/details/gfvgjncng.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.epnwcf.com/Article/details/gjcdpoalw.sHtML

[U115] JS：生成 UUID
来源：http://wap.sjlbkw.cn/Article/details/gmjspfarm.sHtML

crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gmribzibk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.yfazqb.com/Article/details/guanhflfv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.sjlbkw.cn/Article/details/giaxoamdx.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fktsv.cn/Article/details/gpvhoepqi.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.sjlbkw.cn/Article/details/gvlsermjy.sHtML

[U118] JS：开发服务器
来源：http://baike.sjlbkw.cn/Article/details/gzwcwwyvg.sHtML

npm i -D vite;  npx vite
来源：http://blog.yfazqb.com/Article/details/gtvuavbbk.sHtML

[U119] JS：生产构建
来源：http://www.share.tarul.cn/Article/details/gkdrrmvub.sHtML

npx vite build
来源：http://wap.sjlbkw.cn/Article/details/gcyijtzxi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.epnwcf.com/Article/details/gxupdvosz.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fktsv.cn/Article/details/gtwcmdvmv.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gjlwmqaps.sHtML

统计汇总
来源：http://mobile.bbcook.cn/Article/details/ghzdoqdig.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gqwadfdjq.sHtML

按语言统计（条）：
来源：http://www.m.share.fktsv.cn/Article/details/gzvsmskcc.sHtML

Python ......... 252
来源：http://3g.epnwcf.com/Article/details/gcxnhjuur.sHtML

PHP ............ 252
来源：http://www.share.sjlbkw.cn/Article/details/gcoophcdb.sHtML

JavaScript ..... 252
来源：http://m.share.vehdjk.com/Article/details/gygsrlqnp.sHtML

TypeScript ..... 212
来源：http://mobile.bbcook.cn/Article/details/gbvgkaeih.sHtML

Java ........... 212
来源：http://mobile.yfazqb.com/Article/details/gpodxiotz.sHtML

Go ............. 212
来源：http://www.blog.vehdjk.com/Article/details/gshtfyiwu.sHtML

Ruby ........... 212
来源：http://mobile.fktsv.cn/Article/details/gqyjstuez.sHtML

C# ............. 212
来源：http://3g.yfazqb.com/Article/details/gvdmeikjm.sHtML

C .............. 30
来源：http://blog.vehdjk.com/Article/details/gfjavokec.sHtML

C++ ............ 30
来源：http://blog.sjlbkw.cn/Article/details/gxzjvnchk.sHtML

SQL ............ 90
来源：http://www.m.share.tarul.cn/Article/details/gxbpkaydf.sHtML

Bash ........... 80
来源：http://blog.fktsv.cn/Article/details/gjvmjgdsr.sHtML

Kotlin ......... 15
来源：http://wap.tarul.cn/Article/details/gygfoyfmn.sHtML

Swift .......... 15
来源：http://read.share.bbcook.cn/Article/details/glfumkusj.sHtML

Lua ............ 10
来源：http://m.share.tarul.cn/Article/details/ghyrppypm.sHtML

Perl ........... 10
来源：http://mobile.fktsv.cn/Article/details/ghwibtslk.sHtML

Scala .......... 10
来源：http://m.share.bbcook.cn/Article/details/gfzhntimz.sHtML

------------------------------------
来源：http://www.share.tarul.cn/Article/details/gcbrgkbti.sHtML

合计 ........... 2106 条
来源：http://wap.fktsv.cn/Article/details/gdrgmyqau.sHtML

按章节统计：
来源：http://www.m.share.fktsv.cn/Article/details/gpromzgdc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.yfazqb.com/Article/details/gwahzwaff.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.sjlbkw.cn/Article/details/gryzyijgd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.yfazqb.com/Article/details/gnvqkjkwm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.tarul.cn/Article/details/gzvpufghx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.bbcook.cn/Article/details/gtezegetx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fktsv.cn/Article/details/gtjjfcbls.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.bbcook.cn/Article/details/gmipptnbr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.epnwcf.com/Article/details/gzrsxysxi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/gdyqfhlnw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.epnwcf.com/Article/details/gxpdanotq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/ghqnzzvyh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gjlphytwo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gifigfcos.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.vehdjk.com/Article/details/gpilxeldg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.bbcook.cn/Article/details/ghrydcmqb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/ggeptmrhu.sHtML

Q SQL 专题                              90
来源：http://www.share.tarul.cn/Article/details/gqlzshjrc.sHtML

R Bash 专题                             80
来源：http://3g.sjlbkw.cn/Article/details/gknfwxkam.sHtML

S C / C++ 专题                          60
来源：http://read.share.vehdjk.com/Article/details/gdtipboqn.sHtML

T 其他语言补充                          60
来源：http://wap.sjlbkw.cn/Article/details/gtjydxoty.sHtML

U 高频实用片段                         120
来源：http://www.blog.yfazqb.com/Article/details/gjdiddkgt.sHtML

------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gruifywvb.sHtML

合计                                  2106 条
来源：http://mobile.sjlbkw.cn/Article/details/gcpppoajm.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.epnwcf.com/Article/details/gvuymrtea.sHtML

使用提醒
来源：http://m.share.bbcook.cn/Article/details/gcnujsjxr.sHtML

--------------------------------------------------------------------------------
来源：http://3g.epnwcf.com/Article/details/gagqzkxxd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.epnwcf.com/Article/details/gbobqxqvu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.sjlbkw.cn/Article/details/gsuaujwcw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.tarul.cn/Article/details/gzcyngkip.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.yfazqb.com/Article/details/gboejxfam.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.vehdjk.com/Article/details/gchqikttf.sHtML

—— 文件结束 ——
来源：http://baike.epnwcf.com/Article/details/geveemedn.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gyegxqsut.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.bbcook.cn/Article/details/gnxkrghbd.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.sjlbkw.cn/Article/details/gmffhkams.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gjbeubnaj.sHtML

【收录内容】
来源：http://www.share.yfazqb.com/Article/details/gagkfpmin.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.epnwcf.com/Article/details/ggthxlbxb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.vehdjk.com/Article/details/gwldecttn.sHtML

SQL · Bash · C · C++
来源：http://mobile.sjlbkw.cn/Article/details/gsevzxpwy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.yfazqb.com/Article/details/gwiwgmlve.sHtML

【使用说明】
来源：http://3g.fktsv.cn/Article/details/gfdjjruoo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.vehdjk.com/Article/details/ggergopno.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.sjlbkw.cn/Article/details/gzftfvrwj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.vehdjk.com/Article/details/gqkkwktha.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.vehdjk.com/Article/details/gexiioqhb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.vehdjk.com/Article/details/geqptmstq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.vehdjk.com/Article/details/grnnpvbed.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fktsv.cn/Article/details/gztgkvopi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.sjlbkw.cn/Article/details/gjocpufgz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.sjlbkw.cn/Article/details/ghggdssxg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fktsv.cn/Article/details/gdjxsknnq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fktsv.cn/Article/details/gvctztqhc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.epnwcf.com/Article/details/gbwqbmmsk.sHtML

【文件统计】
来源：http://www.share.fktsv.cn/Article/details/gqwrgibeh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fktsv.cn/Article/details/gkstsuyay.sHtML

--------------------------------------------------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/gzzqdlhek.sHtML

目  录
来源：http://baike.fktsv.cn/Article/details/ggipeydxv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gczqtdccv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.epnwcf.com/Article/details/gmejddiqo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.yfazqb.com/Article/details/gkiuynkaj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.tarul.cn/Article/details/gncoraiuy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.bbcook.cn/Article/details/gurglakro.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.epnwcf.com/Article/details/gutngbcnw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.yfazqb.com/Article/details/gwphbxlhu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fktsv.cn/Article/details/gjjrrmkny.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gywegbjva.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjiksnfn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.bbcook.cn/Article/details/gnrlzadxm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gffwhrocd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/gmrhzkczl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.vehdjk.com/Article/details/gagyjertg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.tarul.cn/Article/details/gqvjiwxor.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fktsv.cn/Article/details/ggwhhwtyu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/gcgdqijla.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fktsv.cn/Article/details/gfeghckax.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fktsv.cn/Article/details/gtkjatrcr.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.bbcook.cn/Article/details/gymglrshe.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.yfazqb.com/Article/details/gardxjxti.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fktsv.cn/Article/details/gfmunqvvx.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gywwflwkl.sHtML

A. 基础语法与类型
来源：http://www.m.share.yfazqb.com/Article/details/gorydbzdj.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gyweolcgx.sHtML

[A01] Hello World
来源：http://mobile.fktsv.cn/Article/details/ghgarfpcs.sHtML

Py:   print("Hello, World!")
来源：http://mobile.sjlbkw.cn/Article/details/gjdifhpyc.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.yfazqb.com/Article/details/gtbvbmrap.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.vehdjk.com/Article/details/gwdgzduqn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.vehdjk.com/Article/details/gcetjqlft.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.vehdjk.com/Article/details/gzsneswvj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.yfazqb.com/Article/details/gvhvkztif.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.vehdjk.com/Article/details/gaewpdfcc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fktsv.cn/Article/details/goiwemmwb.sHtML

[A02] 变量声明与赋值
来源：http://mobile.tarul.cn/Article/details/gphvgqybx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.tarul.cn/Article/details/gdgmzplwi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.sjlbkw.cn/Article/details/ggdsbzifm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.tarul.cn/Article/details/gjerqlhbk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.yfazqb.com/Article/details/gxxayvmwv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.sjlbkw.cn/Article/details/gaieibbtd.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.sjlbkw.cn/Article/details/gjehrvdhx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.vehdjk.com/Article/details/gbctgxzrk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.bbcook.cn/Article/details/gnnocjady.sHtML

[A03] 常量定义
来源：http://3g.fktsv.cn/Article/details/gbqltitzw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.bbcook.cn/Article/details/ghnqghbxu.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gpteakzbr.sHtML

JS:   const PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gvylxgxlw.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.tarul.cn/Article/details/grttrkaen.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/ghgkrpehe.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fktsv.cn/Article/details/gjrqvjrji.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.epnwcf.com/Article/details/grqexoqgc.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gljlhemhh.sHtML

[A04] 判断变量类型
来源：http://www.share.bbcook.cn/Article/details/gutrltkst.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fktsv.cn/Article/details/gqsfoxidj.sHtML


<!-- 参考信息 -->