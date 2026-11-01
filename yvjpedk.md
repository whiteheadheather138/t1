代发 wailian999

[U37] Py：读写 Excel
来源：http://wap.bbcook.cn/Article/details/gbzqkvdya.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.bbcook.cn/Article/details/giovzjryc.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.sjlbkw.cn/Article/details/gokrxtwpk.sHtML

Path(__file__).resolve().parent
来源：http://3g.sjlbkw.cn/Article/details/gptywdcjh.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.epnwcf.com/Article/details/grfyogbyq.sHtML

sys.stdout.isatty()
来源：http://m.share.tarul.cn/Article/details/gtymdhbdu.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.bbcook.cn/Article/details/glbrdgsnn.sHtML

print("err", file=sys.stderr)
来源：http://m.share.tarul.cn/Article/details/glppxcgye.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.epnwcf.com/Article/details/goudgthrl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.bbcook.cn/Article/details/gxzkbimkv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.bbcook.cn/Article/details/gpgdkgmda.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.yfazqb.com/Article/details/gvrmpypgv.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gtvxzbqvh.sHtML

namespace App\Http;
来源：http://mobile.yfazqb.com/Article/details/gpxjzwdkf.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fktsv.cn/Article/details/gjugwmdof.sHtML

declare(strict_types=1);
来源：http://read.share.sjlbkw.cn/Article/details/gugpuafuj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.tarul.cn/Article/details/glvwmiksl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gwgszyfyy.sHtML

[U46] PHP：可空类型
来源：http://blog.vehdjk.com/Article/details/gljqpwqij.sHtML

?string $name = null
来源：http://www.share.vehdjk.com/Article/details/grobjbieg.sHtML

[U47] PHP：联合类型
来源：http://wap.yfazqb.com/Article/details/gvfpvcyvv.sHtML

int|string $id
来源：http://wap.epnwcf.com/Article/details/gbavihlfj.sHtML

[U48] PHP：纯枚举
来源：http://wap.yfazqb.com/Article/details/gjgdcekjr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.sjlbkw.cn/Article/details/gzjmxnqcm.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.yfazqb.com/Article/details/ghfagergc.sHtML

public readonly string $name
来源：http://wap.yfazqb.com/Article/details/gdjonsxqf.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.epnwcf.com/Article/details/gduobutxd.sHtML

public function __construct(private int $id) {}
来源：http://wap.yfazqb.com/Article/details/ggyoklsav.sHtML

[U51] PHP：数组解构
来源：http://www.share.epnwcf.com/Article/details/gimruzyio.sHtML

[$a, $b] = $arr;
来源：http://wap.fktsv.cn/Article/details/gnuldoxes.sHtML

[U52] PHP：箭头函数
来源：http://m.share.bbcook.cn/Article/details/gfablizwf.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.tarul.cn/Article/details/gpxqrzxud.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.sjlbkw.cn/Article/details/gfsfwkqhx.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.bbcook.cn/Article/details/gxlhfzijj.sHtML

[U54] PHP：空安全调用
来源：http://wap.fktsv.cn/Article/details/gfukiktps.sHtML

$obj?->method()
来源：http://baike.epnwcf.com/Article/details/gawldapyl.sHtML

[U55] PHP：match 表达式
来源：http://3g.epnwcf.com/Article/details/gokdcynen.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.epnwcf.com/Article/details/gkptfqdrj.sHtML

[U56] PHP：命名参数
来源：http://www.share.vehdjk.com/Article/details/gqfplxrbs.sHtML

f(a: 1, b: 2)
来源：http://read.share.tarul.cn/Article/details/grmvprmyh.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gjcqdumkp.sHtML

"值: {$a}"
来源：http://read.share.yfazqb.com/Article/details/ggizrkqmx.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fktsv.cn/Article/details/garikjihe.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.sjlbkw.cn/Article/details/grmfxrhyz.sHtML

[U59] PHP：自定义排序
来源：http://www.share.bbcook.cn/Article/details/gsysitnpj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.sjlbkw.cn/Article/details/gzhgsbwys.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.sjlbkw.cn/Article/details/gbubihfqy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.vehdjk.com/Article/details/ggbcuvsqr.sHtML

[U61] PHP：正则
来源：http://www.blog.sjlbkw.cn/Article/details/gfpuwcmxw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.epnwcf.com/Article/details/gjiwenyeu.sHtML

[U62] PHP：日期对象
来源：http://www.blog.tarul.cn/Article/details/godvalhnz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.epnwcf.com/Article/details/gqgmyqqmj.sHtML

[U63] PHP：文件读写
来源：http://3g.vehdjk.com/Article/details/geeozoovq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.epnwcf.com/Article/details/guccwjslm.sHtML

[U64] PHP：目录遍历
来源：http://3g.yfazqb.com/Article/details/gjbhiqxbm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fktsv.cn/Article/details/gsealeluk.sHtML

[U65] PHP：会话
来源：http://m.share.fktsv.cn/Article/details/gwftdoupo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gwngtcwcj.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.vehdjk.com/Article/details/gwazstfcm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.sjlbkw.cn/Article/details/gykjojarh.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fktsv.cn/Article/details/gwylqgwny.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.yfazqb.com/Article/details/gvtnxjhbz.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.vehdjk.com/Article/details/gunsccawj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.bbcook.cn/Article/details/gzdlvvvzo.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.vehdjk.com/Article/details/gsqvkrcxx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.epnwcf.com/Article/details/gjannygbg.sHtML

[U70] PHP：PDO 事务
来源：http://3g.bbcook.cn/Article/details/gztefxyld.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.vehdjk.com/Article/details/ghwybxmej.sHtML

[U71] PHP：抛出异常
来源：http://read.share.sjlbkw.cn/Article/details/gequjwaqb.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.yfazqb.com/Article/details/gtrurjycu.sHtML

[U72] PHP：写错误日志
来源：http://wap.vehdjk.com/Article/details/glszfiubd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.epnwcf.com/Article/details/gmbkozsjt.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fktsv.cn/Article/details/ghqvsznkg.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.vehdjk.com/Article/details/gpgeumqht.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gxznllnus.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.tarul.cn/Article/details/gxpabceqh.sHtML

[U75] PHP：依赖注入
来源：http://3g.fktsv.cn/Article/details/gzmndijuj.sHtML

composer require psr/container
来源：http://www.share.fktsv.cn/Article/details/gxyakvxdt.sHtML

[U76] PHP：简单路由
来源：http://mobile.bbcook.cn/Article/details/gjettrdsm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.vehdjk.com/Article/details/gpvwzbwqi.sHtML

[U77] PHP：模板渲染
来源：http://blog.vehdjk.com/Article/details/gztwpfica.sHtML

composer require twig/twig
来源：http://www.blog.sjlbkw.cn/Article/details/grvtfxwvv.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcmpmasi.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.yfazqb.com/Article/details/glgiweesz.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fktsv.cn/Article/details/gfeswemix.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fktsv.cn/Article/details/gfdowrner.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.tarul.cn/Article/details/gbkbyipxj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fktsv.cn/Article/details/grhshmpnu.sHtML

[U81] JS：初始化项目
来源：http://baike.epnwcf.com/Article/details/gvrztufnj.sHtML

npm init -y;  npm i express
来源：http://read.share.vehdjk.com/Article/details/gnrssryxh.sHtML

[U82] JS：package.json 脚本
来源：http://blog.tarul.cn/Article/details/gydmcjmjp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.yfazqb.com/Article/details/gnkabnzgc.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.bbcook.cn/Article/details/giduxglyl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.vehdjk.com/Article/details/gylhpszwy.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.vehdjk.com/Article/details/gtnhcvpcl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fktsv.cn/Article/details/gauwilkyx.sHtML

[U85] JS：可选链
来源：http://www.blog.bbcook.cn/Article/details/gpemstnrp.sHtML

a?.b?.c
来源：http://mobile.fktsv.cn/Article/details/gcxwmoilh.sHtML

[U86] JS：空值合并
来源：http://blog.yfazqb.com/Article/details/gkbrhgftw.sHtML

a ?? b
来源：http://www.blog.vehdjk.com/Article/details/glkouqqvb.sHtML

[U87] JS：解构默认值
来源：http://m.share.fktsv.cn/Article/details/gjhorkxrv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.sjlbkw.cn/Article/details/guuexgfqv.sHtML

[U88] JS：对象展开合并
来源：http://read.share.tarul.cn/Article/details/gtpsqqsfn.sHtML

{ ...a, ...b }
来源：http://mobile.fktsv.cn/Article/details/gljrvvplk.sHtML

[U89] JS：数组去重
来源：http://www.m.share.yfazqb.com/Article/details/gnizpuocv.sHtML

[...new Set(arr)]
来源：http://blog.sjlbkw.cn/Article/details/gocedjgng.sHtML

[U90] JS：数字数组排序
来源：http://www.share.epnwcf.com/Article/details/gpmrmixdt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gsyifflgp.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.epnwcf.com/Article/details/gsmjshbnr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.yfazqb.com/Article/details/gjerbzxpl.sHtML

[U92] JS：深拷贝
来源：http://www.share.epnwcf.com/Article/details/gtkbsalba.sHtML

structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/gzpeilzuq.sHtML

[U93] JS：模板字符串
来源：http://mobile.tarul.cn/Article/details/gbdhuntgs.sHtML

`共 ${n} 条`
来源：http://wap.tarul.cn/Article/details/gshugzlwc.sHtML

[U94] JS：箭头函数
来源：http://wap.sjlbkw.cn/Article/details/gkatzdrzz.sHtML

const double = x => x * 2;
来源：http://baike.epnwcf.com/Article/details/gkhmrcnjh.sHtML

[U95] JS：Promise 包装
来源：http://blog.tarul.cn/Article/details/gftljiexh.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.tarul.cn/Article/details/gsmurqbil.sHtML

[U96] JS：async/await 与异常
来源：http://baike.vehdjk.com/Article/details/ghybvywcr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gqfetihqt.sHtML

[U97] JS：并发请求
来源：http://www.blog.vehdjk.com/Article/details/gnbwzzzjo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gdzkhbmna.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.epnwcf.com/Article/details/ggxwevwif.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.vehdjk.com/Article/details/gkbxzghcq.sHtML

[U99] JS：事件监听
来源：http://3g.epnwcf.com/Article/details/gtsrtlqqe.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.tarul.cn/Article/details/gapgdesxt.sHtML

[U100] JS：DOM 查询
来源：http://m.share.bbcook.cn/Article/details/gbuqobvks.sHtML

document.querySelector(".item")
来源：http://m.share.tarul.cn/Article/details/gfzxsmqel.sHtML

[U101] JS：classList 操作
来源：http://m.share.fktsv.cn/Article/details/gclpdllki.sHtML

el.classList.toggle("active")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmyrzsqm.sHtML

[U102] JS：本地存储
来源：http://www.share.epnwcf.com/Article/details/glzxhbzyv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.bbcook.cn/Article/details/gmxgalust.sHtML

[U103] JS：定时器
来源：http://www.m.share.bbcook.cn/Article/details/gpehtkbqw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.epnwcf.com/Article/details/gvagvpubo.sHtML

[U104] JS：防抖
来源：http://m.share.yfazqb.com/Article/details/gvlomcmyz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gvtzyhwfq.sHtML

[U105] JS：节流
来源：http://wap.vehdjk.com/Article/details/goccyqsca.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fktsv.cn/Article/details/gedcnawck.sHtML

[U106] JS：日期格式化
来源：http://3g.vehdjk.com/Article/details/grsjgldwh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.tarul.cn/Article/details/gpquennxc.sHtML

[U107] JS：数字千分位
来源：http://baike.tarul.cn/Article/details/gxvphoxaa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.epnwcf.com/Article/details/ganyedvvi.sHtML

[U108] JS：随机整数
来源：http://wap.bbcook.cn/Article/details/gzyzflbvr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.epnwcf.com/Article/details/gsoxfgoaa.sHtML

[U109] JS：数组分组
来源：http://blog.yfazqb.com/Article/details/gplyvywhp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.tarul.cn/Article/details/gyxmskbrn.sHtML

[U110] JS：数组分块
来源：http://blog.fktsv.cn/Article/details/gbucqqpvd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.bbcook.cn/Article/details/gprbwbbxq.sHtML

[U111] JS：对象转 Map
来源：http://wap.vehdjk.com/Article/details/gmcjcdxns.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.vehdjk.com/Article/details/grzonblee.sHtML

[U112] JS：字符串补位
来源：http://www.blog.tarul.cn/Article/details/gagdtrath.sHtML

"7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gqrvkprdv.sHtML

[U113] JS：正则替换全部
来源：http://m.share.vehdjk.com/Article/details/gyrwvqyik.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gdfwgqdrw.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.vehdjk.com/Article/details/gamamvrlq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.sjlbkw.cn/Article/details/godzksmtw.sHtML

[U115] JS：生成 UUID
来源：http://wap.yfazqb.com/Article/details/gabvzlldy.sHtML

crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gfbeqlqsg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.yfazqb.com/Article/details/gnnpblbql.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.vehdjk.com/Article/details/gafuaeusq.sHtML

[U117] JS：单元测试
来源：http://www.share.bbcook.cn/Article/details/gueajinvu.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.tarul.cn/Article/details/gaxyvfdwy.sHtML

[U118] JS：开发服务器
来源：http://read.share.bbcook.cn/Article/details/gbphzcxzp.sHtML

npm i -D vite;  npx vite
来源：http://baike.epnwcf.com/Article/details/gouwbqrzi.sHtML

[U119] JS：生产构建
来源：http://read.share.tarul.cn/Article/details/gpdpntiar.sHtML

npx vite build
来源：http://baike.sjlbkw.cn/Article/details/gdjxtjfvv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fktsv.cn/Article/details/gclbzuwwe.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.epnwcf.com/Article/details/gdxigbxxr.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gsvracudi.sHtML

统计汇总
来源：http://mobile.bbcook.cn/Article/details/gyxayphuf.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/geupvcwba.sHtML

按语言统计（条）：
来源：http://3g.yfazqb.com/Article/details/gmhickynq.sHtML

Python ......... 252
来源：http://www.share.tarul.cn/Article/details/gmxzvpjsm.sHtML

PHP ............ 252
来源：http://mobile.vehdjk.com/Article/details/gihdniybn.sHtML

JavaScript ..... 252
来源：http://baike.bbcook.cn/Article/details/gfcwetzqs.sHtML

TypeScript ..... 212
来源：http://blog.sjlbkw.cn/Article/details/gwwsiarvz.sHtML

Java ........... 212
来源：http://3g.bbcook.cn/Article/details/ggzliuaol.sHtML

Go ............. 212
来源：http://mobile.vehdjk.com/Article/details/gtpupaagd.sHtML

Ruby ........... 212
来源：http://blog.sjlbkw.cn/Article/details/gojqfdksx.sHtML

C# ............. 212
来源：http://mobile.yfazqb.com/Article/details/ghhpvlula.sHtML

C .............. 30
来源：http://baike.sjlbkw.cn/Article/details/gdntzfskw.sHtML

C++ ............ 30
来源：http://wap.yfazqb.com/Article/details/gggztdxog.sHtML

SQL ............ 90
来源：http://mobile.sjlbkw.cn/Article/details/gtchzepln.sHtML

Bash ........... 80
来源：http://www.blog.sjlbkw.cn/Article/details/guaaaexpr.sHtML

Kotlin ......... 15
来源：http://read.share.bbcook.cn/Article/details/gkjkagisu.sHtML

Swift .......... 15
来源：http://read.share.vehdjk.com/Article/details/gzzieqfzr.sHtML

Lua ............ 10
来源：http://www.share.sjlbkw.cn/Article/details/gohxxxqxj.sHtML

Perl ........... 10
来源：http://blog.yfazqb.com/Article/details/grjcewelv.sHtML

Scala .......... 10
来源：http://mobile.epnwcf.com/Article/details/gthlwccsa.sHtML

------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gmeyzdagp.sHtML

合计 ........... 2106 条
来源：http://mobile.fktsv.cn/Article/details/gzfysozbp.sHtML

按章节统计：
来源：http://www.share.yfazqb.com/Article/details/geivbxtnc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.bbcook.cn/Article/details/gfzcpufzl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.bbcook.cn/Article/details/gfdgodjuh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.yfazqb.com/Article/details/gvvfzbchu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.sjlbkw.cn/Article/details/gdwnpjtgl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.epnwcf.com/Article/details/grwjyrpnd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.epnwcf.com/Article/details/gbhxlyoiw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.epnwcf.com/Article/details/gkhxvyxng.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.vehdjk.com/Article/details/gtgrqunlo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gqtblgarz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.yfazqb.com/Article/details/ggbrwinzv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/gneyuweqs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/gvfwsclju.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/gzkrlobvd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.tarul.cn/Article/details/gaqrlxiyf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.yfazqb.com/Article/details/ghcayskmz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gzyqrvjpf.sHtML

Q SQL 专题                              90
来源：http://baike.epnwcf.com/Article/details/gxogliixt.sHtML

R Bash 专题                             80
来源：http://3g.vehdjk.com/Article/details/glaiihaju.sHtML

S C / C++ 专题                          60
来源：http://www.share.sjlbkw.cn/Article/details/gsreczwgd.sHtML

T 其他语言补充                          60
来源：http://blog.vehdjk.com/Article/details/gtawrnzng.sHtML

U 高频实用片段                         120
来源：http://www.m.share.tarul.cn/Article/details/gobftvvhf.sHtML

------------------------------------
来源：http://mobile.bbcook.cn/Article/details/gixkqyyvg.sHtML

合计                                  2106 条
来源：http://blog.fktsv.cn/Article/details/gotdpsrxj.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gtocjljzw.sHtML

使用提醒
来源：http://3g.bbcook.cn/Article/details/gtzqeryni.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gzuiblmvu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.bbcook.cn/Article/details/glscppiyo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.bbcook.cn/Article/details/gmlvjmejb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.bbcook.cn/Article/details/gkimypqtp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.vehdjk.com/Article/details/guonufumf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.vehdjk.com/Article/details/gkaqmdkpf.sHtML

—— 文件结束 ——
来源：http://3g.yfazqb.com/Article/details/gcwobfxmv.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ghqvoxgoa.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.tarul.cn/Article/details/gfbadfpxt.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fktsv.cn/Article/details/gorljztzf.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gmlkygfui.sHtML

【收录内容】
来源：http://read.share.tarul.cn/Article/details/ghkazijig.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.vehdjk.com/Article/details/grhkxvqym.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.yfazqb.com/Article/details/gzcueialm.sHtML

SQL · Bash · C · C++
来源：http://baike.epnwcf.com/Article/details/gxpiefowe.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.yfazqb.com/Article/details/gxnovcgoz.sHtML

【使用说明】
来源：http://www.blog.epnwcf.com/Article/details/gtcukuvcu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.epnwcf.com/Article/details/gtnjigyge.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.bbcook.cn/Article/details/gqxfrymcg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fktsv.cn/Article/details/gecpobfbu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.bbcook.cn/Article/details/gjikyhdjo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.vehdjk.com/Article/details/gadkfbybx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.vehdjk.com/Article/details/gnkxunoym.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.vehdjk.com/Article/details/gwsueueym.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fktsv.cn/Article/details/gqpdfstgi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.bbcook.cn/Article/details/glbptfuur.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.sjlbkw.cn/Article/details/gicehsclf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.sjlbkw.cn/Article/details/gkkgzjucb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.yfazqb.com/Article/details/gyxgcqzlt.sHtML

【文件统计】
来源：http://read.share.sjlbkw.cn/Article/details/gnifqjshz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.bbcook.cn/Article/details/gnaczjiys.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/ghmtxatbo.sHtML

目  录
来源：http://www.blog.fktsv.cn/Article/details/gcsggitns.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fktsv.cn/Article/details/ggvccphha.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.yfazqb.com/Article/details/gfhpakaly.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.tarul.cn/Article/details/gapjlqqsr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.yfazqb.com/Article/details/gnvlmjcxz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.tarul.cn/Article/details/gcaeqqzkf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.vehdjk.com/Article/details/gwhvsxrgx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.vehdjk.com/Article/details/gexsmfohi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.vehdjk.com/Article/details/gunzvnbnd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.vehdjk.com/Article/details/ggofhykqs.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/ggitarsvv.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.vehdjk.com/Article/details/gnbhjebux.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.bbcook.cn/Article/details/gikdjloqw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gymeqqsxx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gqzklrjpu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.tarul.cn/Article/details/gfknibkcv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fktsv.cn/Article/details/gbzutbchj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/gvlcqitrp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fktsv.cn/Article/details/gyxoomdrf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.tarul.cn/Article/details/gackkkeys.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.bbcook.cn/Article/details/gdivuahhh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.tarul.cn/Article/details/gthmijthm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fktsv.cn/Article/details/ghwfmpnym.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gbwermqwa.sHtML

A. 基础语法与类型
来源：http://mobile.yfazqb.com/Article/details/gbqtsyzxe.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gimyeoccp.sHtML

[A01] Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjzkzdso.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fktsv.cn/Article/details/guaanksxz.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.vehdjk.com/Article/details/gvpoqwpsm.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.tarul.cn/Article/details/ghsyggxmd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.yfazqb.com/Article/details/ggdrflalw.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.tarul.cn/Article/details/gzpdfuhyu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.epnwcf.com/Article/details/gtttivwpm.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.tarul.cn/Article/details/gqwtixxrh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.epnwcf.com/Article/details/gkzcxwbbq.sHtML

[A02] 变量声明与赋值
来源：http://www.share.yfazqb.com/Article/details/gzbnhluwy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.bbcook.cn/Article/details/gqlelrifb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.tarul.cn/Article/details/gybsstiis.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.tarul.cn/Article/details/grigqmhye.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fktsv.cn/Article/details/grfwplxzu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fktsv.cn/Article/details/gbelbifpz.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.vehdjk.com/Article/details/gzcgakdsk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.epnwcf.com/Article/details/gpnknvlgk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.vehdjk.com/Article/details/gxhnnswhc.sHtML

[A03] 常量定义
来源：http://blog.fktsv.cn/Article/details/gkthmsfgb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.yfazqb.com/Article/details/ggnqeowfl.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/glupxjmwa.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gpwbtyeep.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/ggjjwlrbe.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gxvpaiijb.sHtML

Go:   const PI = 3.14159
来源：http://wap.sjlbkw.cn/Article/details/gblqopcyq.sHtML


<!-- 参考信息 -->