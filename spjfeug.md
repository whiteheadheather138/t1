代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://mobile.vehdjk.com/Article/details/givddvghr.sHtML

sys.stdout.isatty()
来源：http://m.share.sjlbkw.cn/Article/details/gcmzrvpxa.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.tarul.cn/Article/details/gxxymuhqj.sHtML

print("err", file=sys.stderr)
来源：http://m.share.vehdjk.com/Article/details/gfnxywvxs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.tarul.cn/Article/details/gmazyzewf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.yfazqb.com/Article/details/gifmvprvt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.epnwcf.com/Article/details/gilnwarmk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fktsv.cn/Article/details/gpjpguyop.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.epnwcf.com/Article/details/gsviyzmes.sHtML

namespace App\Http;
来源：http://baike.fktsv.cn/Article/details/gxeljdxqa.sHtML

[U44] PHP：开启严格类型
来源：http://blog.sjlbkw.cn/Article/details/gzttegwul.sHtML

declare(strict_types=1);
来源：http://read.share.vehdjk.com/Article/details/gnmxpshtv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.epnwcf.com/Article/details/gxlqibojs.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/ghoxovzel.sHtML

[U46] PHP：可空类型
来源：http://baike.vehdjk.com/Article/details/gagybyrft.sHtML

?string $name = null
来源：http://wap.epnwcf.com/Article/details/gvtxywctr.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.tarul.cn/Article/details/ghackslvb.sHtML

int|string $id
来源：http://read.share.sjlbkw.cn/Article/details/gafolwadz.sHtML

[U48] PHP：纯枚举
来源：http://3g.fktsv.cn/Article/details/gsefuveie.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.epnwcf.com/Article/details/gspfxtmrr.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.epnwcf.com/Article/details/gshfbgpwl.sHtML

public readonly string $name
来源：http://baike.epnwcf.com/Article/details/gdwvuphwb.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.vehdjk.com/Article/details/gblzpblug.sHtML

public function __construct(private int $id) {}
来源：http://www.share.yfazqb.com/Article/details/goreqqmxm.sHtML

[U51] PHP：数组解构
来源：http://wap.tarul.cn/Article/details/gtndindfm.sHtML

[$a, $b] = $arr;
来源：http://3g.tarul.cn/Article/details/gnnnhwsmu.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.tarul.cn/Article/details/gjmyezfpy.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.sjlbkw.cn/Article/details/gjnnnihze.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.tarul.cn/Article/details/gwtscgmkx.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.yfazqb.com/Article/details/gwimseezv.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.epnwcf.com/Article/details/gvkeiqncw.sHtML

$obj?->method()
来源：http://read.share.yfazqb.com/Article/details/ghikyomge.sHtML

[U55] PHP：match 表达式
来源：http://wap.bbcook.cn/Article/details/gnagxwumr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.vehdjk.com/Article/details/giunnbgaf.sHtML

[U56] PHP：命名参数
来源：http://mobile.epnwcf.com/Article/details/gintqzqxz.sHtML

f(a: 1, b: 2)
来源：http://3g.fktsv.cn/Article/details/gfpikwpig.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gsapvmpkv.sHtML

"值: {$a}"
来源：http://www.share.epnwcf.com/Article/details/gtansfgkr.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.epnwcf.com/Article/details/gchdzoamj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fktsv.cn/Article/details/gkucieiuy.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.bbcook.cn/Article/details/gjaknmakx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.epnwcf.com/Article/details/ggqlyhiuu.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.sjlbkw.cn/Article/details/gknzzjdtb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.bbcook.cn/Article/details/gtqeyrbun.sHtML

[U61] PHP：正则
来源：http://www.blog.epnwcf.com/Article/details/gexohknav.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/goflhxglo.sHtML

[U62] PHP：日期对象
来源：http://3g.yfazqb.com/Article/details/gcwrziixu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fktsv.cn/Article/details/gmzeatkar.sHtML

[U63] PHP：文件读写
来源：http://m.share.tarul.cn/Article/details/gxyjxtunp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.bbcook.cn/Article/details/ghprbmwez.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fktsv.cn/Article/details/ghkorjnyx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.bbcook.cn/Article/details/gvulusfrj.sHtML

[U65] PHP：会话
来源：http://mobile.tarul.cn/Article/details/gxccckwyj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.yfazqb.com/Article/details/gsfvkfdkw.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.bbcook.cn/Article/details/gqownogrd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.yfazqb.com/Article/details/gblovmiuk.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.vehdjk.com/Article/details/gufuqachu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.epnwcf.com/Article/details/gcnwgqsct.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.vehdjk.com/Article/details/grwgorokz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.sjlbkw.cn/Article/details/gggzkhxsx.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.bbcook.cn/Article/details/gmvwenjro.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.vehdjk.com/Article/details/gseinlmcp.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fktsv.cn/Article/details/gdyvuhomo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.tarul.cn/Article/details/gqdcfxxso.sHtML

[U71] PHP：抛出异常
来源：http://wap.tarul.cn/Article/details/gnyrdkucb.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.vehdjk.com/Article/details/gewojoeci.sHtML

[U72] PHP：写错误日志
来源：http://www.share.yfazqb.com/Article/details/gfvnkourp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.vehdjk.com/Article/details/gfyutdrni.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fktsv.cn/Article/details/gxahxfuzj.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.vehdjk.com/Article/details/gllnrpwsy.sHtML

[U74] PHP：读取环境变量
来源：http://wap.sjlbkw.cn/Article/details/gfichthup.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.bbcook.cn/Article/details/guwvgkrdu.sHtML

[U75] PHP：依赖注入
来源：http://read.share.bbcook.cn/Article/details/gguksvfgg.sHtML

composer require psr/container
来源：http://3g.sjlbkw.cn/Article/details/gtwmtttax.sHtML

[U76] PHP：简单路由
来源：http://www.share.vehdjk.com/Article/details/gsiqgqrvz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.sjlbkw.cn/Article/details/geqoszgnd.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.tarul.cn/Article/details/gtgpdiezh.sHtML

composer require twig/twig
来源：http://blog.fktsv.cn/Article/details/ghqhqvguh.sHtML

[U78] PHP：单元测试
来源：http://read.share.fktsv.cn/Article/details/gmkomzrwk.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fktsv.cn/Article/details/gqufprzpf.sHtML

[U79] PHP：静态分析
来源：http://m.share.bbcook.cn/Article/details/gamnpxcpz.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.vehdjk.com/Article/details/gyawpckgf.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.epnwcf.com/Article/details/gbxvlwtoq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.vehdjk.com/Article/details/ggqkpfxps.sHtML

[U81] JS：初始化项目
来源：http://www.share.epnwcf.com/Article/details/geusdvqef.sHtML

npm init -y;  npm i express
来源：http://www.blog.vehdjk.com/Article/details/gokixpvpa.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.vehdjk.com/Article/details/gprbjbuqp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.bbcook.cn/Article/details/gmyexekzy.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fktsv.cn/Article/details/gbthaebax.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.sjlbkw.cn/Article/details/gfqtqhbeu.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.sjlbkw.cn/Article/details/gdyigonun.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.bbcook.cn/Article/details/gpbyceftd.sHtML

[U85] JS：可选链
来源：http://blog.vehdjk.com/Article/details/gmyvdvwrg.sHtML

a?.b?.c
来源：http://m.share.yfazqb.com/Article/details/gsvvunity.sHtML

[U86] JS：空值合并
来源：http://m.share.vehdjk.com/Article/details/gjspwohzc.sHtML

a ?? b
来源：http://blog.vehdjk.com/Article/details/gfmccwtnj.sHtML

[U87] JS：解构默认值
来源：http://www.blog.epnwcf.com/Article/details/gqrbiubkt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.epnwcf.com/Article/details/gfxydibsr.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.tarul.cn/Article/details/gqgjsfysp.sHtML

{ ...a, ...b }
来源：http://www.m.share.bbcook.cn/Article/details/gpdottpgh.sHtML

[U89] JS：数组去重
来源：http://read.share.fktsv.cn/Article/details/gsirmipok.sHtML

[...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/gfmtqxdha.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.vehdjk.com/Article/details/gwqrpzpnm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/gfcihbtrj.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.bbcook.cn/Article/details/gyopefqlu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.yfazqb.com/Article/details/gpqduaujw.sHtML

[U92] JS：深拷贝
来源：http://www.share.yfazqb.com/Article/details/gpvrmglzy.sHtML

structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gigsprzxm.sHtML

[U93] JS：模板字符串
来源：http://m.share.bbcook.cn/Article/details/gnvnpudla.sHtML

`共 ${n} 条`
来源：http://read.share.sjlbkw.cn/Article/details/gyavudmbr.sHtML

[U94] JS：箭头函数
来源：http://baike.epnwcf.com/Article/details/gaxzszsmx.sHtML

const double = x => x * 2;
来源：http://www.blog.epnwcf.com/Article/details/gkrthrots.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.epnwcf.com/Article/details/gglptmqhs.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.vehdjk.com/Article/details/gibfgjkom.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.epnwcf.com/Article/details/guupmfqoc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/gecqusrsz.sHtML

[U97] JS：并发请求
来源：http://read.share.yfazqb.com/Article/details/gbjbbgfyn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gzbzwmbzp.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.bbcook.cn/Article/details/gvlyfbeyw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.bbcook.cn/Article/details/gdqqzjeoc.sHtML

[U99] JS：事件监听
来源：http://m.share.tarul.cn/Article/details/gxpvbfbwq.sHtML

el.addEventListener("click", e => {})
来源：http://blog.vehdjk.com/Article/details/gbxjnhyex.sHtML

[U100] JS：DOM 查询
来源：http://mobile.sjlbkw.cn/Article/details/gmajufnrz.sHtML

document.querySelector(".item")
来源：http://baike.tarul.cn/Article/details/gakbpdqqp.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.vehdjk.com/Article/details/gdczyzbbj.sHtML

el.classList.toggle("active")
来源：http://www.blog.bbcook.cn/Article/details/gjmagjhow.sHtML

[U102] JS：本地存储
来源：http://blog.yfazqb.com/Article/details/gbexnbydn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.epnwcf.com/Article/details/gatgcsknn.sHtML

[U103] JS：定时器
来源：http://baike.vehdjk.com/Article/details/gtvknxyrm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.yfazqb.com/Article/details/gehlvuzug.sHtML

[U104] JS：防抖
来源：http://www.m.share.fktsv.cn/Article/details/gsxdgzint.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/ghgcuhfpd.sHtML

[U105] JS：节流
来源：http://3g.vehdjk.com/Article/details/gutpcgcgy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.tarul.cn/Article/details/gtrrilokm.sHtML

[U106] JS：日期格式化
来源：http://mobile.fktsv.cn/Article/details/gexaabsaf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.vehdjk.com/Article/details/gdslvnnql.sHtML

[U107] JS：数字千分位
来源：http://www.blog.tarul.cn/Article/details/gpehmxttc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.sjlbkw.cn/Article/details/glfnoucmu.sHtML

[U108] JS：随机整数
来源：http://baike.tarul.cn/Article/details/gnkcrikox.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.vehdjk.com/Article/details/gitzwqrwt.sHtML

[U109] JS：数组分组
来源：http://read.share.bbcook.cn/Article/details/gpshnqyey.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.sjlbkw.cn/Article/details/gaeyktwpr.sHtML

[U110] JS：数组分块
来源：http://www.m.share.vehdjk.com/Article/details/gdgriafjr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.vehdjk.com/Article/details/ggcydgaep.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fktsv.cn/Article/details/gjdbiklpl.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fktsv.cn/Article/details/gvibmldyl.sHtML

[U112] JS：字符串补位
来源：http://blog.sjlbkw.cn/Article/details/gqcsieaju.sHtML

"7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gbggkfasd.sHtML

[U113] JS：正则替换全部
来源：http://read.share.yfazqb.com/Article/details/gbaxwyvyh.sHtML

s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gulpmzykz.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.epnwcf.com/Article/details/gveexegef.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.epnwcf.com/Article/details/gohjdwdiw.sHtML

[U115] JS：生成 UUID
来源：http://baike.fktsv.cn/Article/details/gjkdiurjt.sHtML

crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gawzfnrba.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.bbcook.cn/Article/details/gogqwpxad.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.yfazqb.com/Article/details/ghtqccmsa.sHtML

[U117] JS：单元测试
来源：http://read.share.yfazqb.com/Article/details/guyzdfebg.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.vehdjk.com/Article/details/gimgqvjgp.sHtML

[U118] JS：开发服务器
来源：http://read.share.fktsv.cn/Article/details/gqkmerokc.sHtML

npm i -D vite;  npx vite
来源：http://3g.epnwcf.com/Article/details/gxfbtfrbn.sHtML

[U119] JS：生产构建
来源：http://baike.vehdjk.com/Article/details/gqpnguqft.sHtML

npx vite build
来源：http://m.share.fktsv.cn/Article/details/ggzniqtlz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fktsv.cn/Article/details/geomabkcp.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.yfazqb.com/Article/details/gknkxezdd.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gqzqhvxlb.sHtML

统计汇总
来源：http://www.blog.yfazqb.com/Article/details/gnulszfzp.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gtpejfyne.sHtML

按语言统计（条）：
来源：http://3g.yfazqb.com/Article/details/gkqoading.sHtML

Python ......... 252
来源：http://www.share.fktsv.cn/Article/details/gfaqdcrmr.sHtML

PHP ............ 252
来源：http://read.share.vehdjk.com/Article/details/gujbybxva.sHtML

JavaScript ..... 252
来源：http://blog.yfazqb.com/Article/details/gbjoboanf.sHtML

TypeScript ..... 212
来源：http://m.share.epnwcf.com/Article/details/gdjjunrhk.sHtML

Java ........... 212
来源：http://blog.yfazqb.com/Article/details/gkholwfuf.sHtML

Go ............. 212
来源：http://www.share.tarul.cn/Article/details/gxpnutgkj.sHtML

Ruby ........... 212
来源：http://blog.tarul.cn/Article/details/gbdpaeuqe.sHtML

C# ............. 212
来源：http://baike.sjlbkw.cn/Article/details/gjndbbdnn.sHtML

C .............. 30
来源：http://www.m.share.sjlbkw.cn/Article/details/gshwggwct.sHtML

C++ ............ 30
来源：http://3g.bbcook.cn/Article/details/gawimsecl.sHtML

SQL ............ 90
来源：http://read.share.bbcook.cn/Article/details/gkzvdvdpf.sHtML

Bash ........... 80
来源：http://www.share.yfazqb.com/Article/details/gshbtqule.sHtML

Kotlin ......... 15
来源：http://read.share.yfazqb.com/Article/details/gfmobpjam.sHtML

Swift .......... 15
来源：http://wap.tarul.cn/Article/details/gjgegtrmv.sHtML

Lua ............ 10
来源：http://m.share.fktsv.cn/Article/details/gntouqyfx.sHtML

Perl ........... 10
来源：http://mobile.fktsv.cn/Article/details/gksdeiitk.sHtML

Scala .......... 10
来源：http://m.share.tarul.cn/Article/details/gzjmydmsd.sHtML

------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gryokbsso.sHtML

合计 ........... 2106 条
来源：http://www.share.yfazqb.com/Article/details/goihexbsy.sHtML

按章节统计：
来源：http://m.share.tarul.cn/Article/details/gbvdsmrnh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.vehdjk.com/Article/details/gdbwghwdj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.epnwcf.com/Article/details/gdelptupw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.epnwcf.com/Article/details/gshvwnyfc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.bbcook.cn/Article/details/gkdfetprs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.bbcook.cn/Article/details/gxtpsteno.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.sjlbkw.cn/Article/details/gshorpokq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.tarul.cn/Article/details/gsiciogzs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.sjlbkw.cn/Article/details/gcrfdxpgx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gcqdpkhvy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.bbcook.cn/Article/details/gliiftlef.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gpxfewwgj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gwlvywzen.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gclcnnief.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.epnwcf.com/Article/details/gykfjbyzj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.yfazqb.com/Article/details/gizxqgeaw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/godvzeyvj.sHtML

Q SQL 专题                              90
来源：http://baike.tarul.cn/Article/details/gkfsvenye.sHtML

R Bash 专题                             80
来源：http://www.share.bbcook.cn/Article/details/ggtfctxca.sHtML

S C / C++ 专题                          60
来源：http://mobile.yfazqb.com/Article/details/gabisiitx.sHtML

T 其他语言补充                          60
来源：http://mobile.tarul.cn/Article/details/gfcfvuvvi.sHtML

U 高频实用片段                         120
来源：http://read.share.fktsv.cn/Article/details/gmxqzqmiy.sHtML

------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gywfowncb.sHtML

合计                                  2106 条
来源：http://3g.bbcook.cn/Article/details/gdbkhmjzj.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/gspodmzlo.sHtML

使用提醒
来源：http://www.blog.yfazqb.com/Article/details/gfasplcix.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gwvksvpvj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.sjlbkw.cn/Article/details/gcyfumyuz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.epnwcf.com/Article/details/gncmmnama.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.sjlbkw.cn/Article/details/gpjybvcty.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.tarul.cn/Article/details/ggsuytlkp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.tarul.cn/Article/details/gmpyysnlj.sHtML

—— 文件结束 ——
来源：http://wap.vehdjk.com/Article/details/gytsvciwh.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gvtnlhrnc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.bbcook.cn/Article/details/gnxokudei.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.epnwcf.com/Article/details/gqmerwtfs.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gzobhzdzn.sHtML

【收录内容】
来源：http://wap.yfazqb.com/Article/details/gngauvlbi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.bbcook.cn/Article/details/gpyyzgfso.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.tarul.cn/Article/details/gvapdwgxb.sHtML

SQL · Bash · C · C++
来源：http://m.share.fktsv.cn/Article/details/gfgrwvnik.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.vehdjk.com/Article/details/godvsbxny.sHtML

【使用说明】
来源：http://wap.yfazqb.com/Article/details/giqzzmqtz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.yfazqb.com/Article/details/gglgotumn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.epnwcf.com/Article/details/guxmytksb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.sjlbkw.cn/Article/details/gdhxevllq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fktsv.cn/Article/details/gijuerlxr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fktsv.cn/Article/details/gfatwtnkh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.sjlbkw.cn/Article/details/ggdipgthg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.sjlbkw.cn/Article/details/gvvamkhna.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.yfazqb.com/Article/details/gzfllghfu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.sjlbkw.cn/Article/details/ggkzzdjqu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.tarul.cn/Article/details/gjuaovrim.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.bbcook.cn/Article/details/gcpxaxlbx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.epnwcf.com/Article/details/grwhntqjx.sHtML

【文件统计】
来源：http://mobile.fktsv.cn/Article/details/gpawkwrhh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fktsv.cn/Article/details/gjpdvgroj.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gxugmyuza.sHtML

目  录
来源：http://baike.vehdjk.com/Article/details/gkvwkvlis.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/gbhonebuz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.yfazqb.com/Article/details/gjfhzwnvz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.yfazqb.com/Article/details/gvmuzjbuf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.tarul.cn/Article/details/glwikoisw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.vehdjk.com/Article/details/glzaktqrk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.vehdjk.com/Article/details/goamgwxzz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.yfazqb.com/Article/details/gghxuiqll.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/ganvewiqc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.sjlbkw.cn/Article/details/gjsznmtyw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/gxrsmmkor.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.yfazqb.com/Article/details/gyuxnlkrk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/gkjwcixno.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/gghctdfbk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/gowveaisf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.sjlbkw.cn/Article/details/gpdgodtpz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.yfazqb.com/Article/details/gkoaqnmtn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.yfazqb.com/Article/details/giunqiibh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.vehdjk.com/Article/details/gqimttmfl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.vehdjk.com/Article/details/gsnytgggz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.sjlbkw.cn/Article/details/gmfxgedcv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.yfazqb.com/Article/details/gzkfceias.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.yfazqb.com/Article/details/gykheudpt.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gfkbvjcsz.sHtML

A. 基础语法与类型
来源：http://3g.sjlbkw.cn/Article/details/gyrusqecs.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gugxybrio.sHtML

[A01] Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gtvejzhjo.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fktsv.cn/Article/details/gdkwyquqi.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.bbcook.cn/Article/details/grrrdxdog.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.tarul.cn/Article/details/ghybsysrw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.sjlbkw.cn/Article/details/gwrusfahq.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.sjlbkw.cn/Article/details/gflanlsol.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.yfazqb.com/Article/details/gilxxbdzl.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.vehdjk.com/Article/details/gstsyetkd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.tarul.cn/Article/details/gqwsvclqf.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgxyhiuq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.tarul.cn/Article/details/gioftoqrg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.bbcook.cn/Article/details/gobgejbck.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.tarul.cn/Article/details/gfttmmkwv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.vehdjk.com/Article/details/gdksllmba.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.sjlbkw.cn/Article/details/gdcgcnqus.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.yfazqb.com/Article/details/gqdinnyjb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.vehdjk.com/Article/details/gjleibogl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fktsv.cn/Article/details/gqibzmgik.sHtML

[A03] 常量定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzcuogdw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.sjlbkw.cn/Article/details/gqoyqqmcp.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gsfrxwytb.sHtML

JS:   const PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gvmrmmcuh.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/grshjuhpq.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gtvbdrgin.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.vehdjk.com/Article/details/gyerbvvqg.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.epnwcf.com/Article/details/gimvreubg.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/gsewoqpie.sHtML

[A04] 判断变量类型
来源：http://baike.bbcook.cn/Article/details/gwkbcxgzz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.bbcook.cn/Article/details/grcdforhh.sHtML


<!-- 参考信息 -->