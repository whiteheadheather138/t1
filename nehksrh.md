代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.m.share.tarul.cn/Article/details/gkssuvamz.sHtML

sys.stdout.isatty()
来源：http://www.m.share.tarul.cn/Article/details/gmtifunze.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fktsv.cn/Article/details/glszpyxow.sHtML

print("err", file=sys.stderr)
来源：http://m.share.yfazqb.com/Article/details/gmwpvbczr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.bbcook.cn/Article/details/gpzezeyrq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fktsv.cn/Article/details/gehtwlykn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.tarul.cn/Article/details/gxqwnemdd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.epnwcf.com/Article/details/gwmgeysyu.sHtML

[U43] PHP：声明命名空间
来源：http://3g.yfazqb.com/Article/details/gvbcdwosd.sHtML

namespace App\Http;
来源：http://mobile.vehdjk.com/Article/details/ghtbaoafq.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.tarul.cn/Article/details/gwuvhryhb.sHtML

declare(strict_types=1);
来源：http://www.blog.epnwcf.com/Article/details/ghrgdlpqi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.vehdjk.com/Article/details/gztgckywb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqfkxsafq.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.bbcook.cn/Article/details/gqsaclyjb.sHtML

?string $name = null
来源：http://mobile.sjlbkw.cn/Article/details/gpzmgnsul.sHtML

[U47] PHP：联合类型
来源：http://m.share.epnwcf.com/Article/details/gzvymzqth.sHtML

int|string $id
来源：http://m.share.fktsv.cn/Article/details/gguimkwts.sHtML

[U48] PHP：纯枚举
来源：http://mobile.vehdjk.com/Article/details/glpqwwmtq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.epnwcf.com/Article/details/gkdzivsed.sHtML

[U49] PHP：只读属性
来源：http://www.share.tarul.cn/Article/details/ggwutxouh.sHtML

public readonly string $name
来源：http://3g.vehdjk.com/Article/details/gcpwtjcfy.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fktsv.cn/Article/details/gulouorhf.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.vehdjk.com/Article/details/gjlnzzqta.sHtML

[U51] PHP：数组解构
来源：http://read.share.tarul.cn/Article/details/gdtjbgoja.sHtML

[$a, $b] = $arr;
来源：http://www.blog.sjlbkw.cn/Article/details/gpqvvhgwb.sHtML

[U52] PHP：箭头函数
来源：http://baike.yfazqb.com/Article/details/gwhehngiv.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fktsv.cn/Article/details/gcqgmfiuh.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fktsv.cn/Article/details/gkrlrcrgv.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fktsv.cn/Article/details/gghxinbjz.sHtML

[U54] PHP：空安全调用
来源：http://mobile.tarul.cn/Article/details/gdzqkjmgh.sHtML

$obj?->method()
来源：http://3g.sjlbkw.cn/Article/details/gnhdjvnqr.sHtML

[U55] PHP：match 表达式
来源：http://www.share.sjlbkw.cn/Article/details/gtgnnzvfh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.bbcook.cn/Article/details/ghugpahcb.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.vehdjk.com/Article/details/gizsbhjfj.sHtML

f(a: 1, b: 2)
来源：http://m.share.vehdjk.com/Article/details/goddyrsxd.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.tarul.cn/Article/details/grsbhqjtq.sHtML

"值: {$a}"
来源：http://baike.yfazqb.com/Article/details/gdiidjzgj.sHtML

[U58] PHP：数组三件套
来源：http://blog.epnwcf.com/Article/details/gjjmoqtnn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fktsv.cn/Article/details/gejjfmesd.sHtML

[U59] PHP：自定义排序
来源：http://m.share.epnwcf.com/Article/details/gblgqjdlk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.epnwcf.com/Article/details/gtaocfnjc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.epnwcf.com/Article/details/grzivpuau.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.vehdjk.com/Article/details/gxootzrcc.sHtML

[U61] PHP：正则
来源：http://read.share.sjlbkw.cn/Article/details/gczrpykvt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.yfazqb.com/Article/details/gnhpmnqbh.sHtML

[U62] PHP：日期对象
来源：http://baike.tarul.cn/Article/details/gmcvrtzwk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.bbcook.cn/Article/details/gssgxhuir.sHtML

[U63] PHP：文件读写
来源：http://www.blog.yfazqb.com/Article/details/gyuzbqkgn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.sjlbkw.cn/Article/details/gfovuufth.sHtML

[U64] PHP：目录遍历
来源：http://baike.fktsv.cn/Article/details/gwitvplsw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fktsv.cn/Article/details/giynymlxf.sHtML

[U65] PHP：会话
来源：http://read.share.epnwcf.com/Article/details/gjfdlzoag.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/ggtynbfwk.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.bbcook.cn/Article/details/gohqqsult.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.bbcook.cn/Article/details/gzpajthjw.sHtML

[U67] PHP：处理文件上传
来源：http://blog.tarul.cn/Article/details/ghfqqkzjr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.vehdjk.com/Article/details/gzoddzooi.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.sjlbkw.cn/Article/details/gxtkyqaib.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.epnwcf.com/Article/details/gghjxmbnc.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fktsv.cn/Article/details/gybtkqmwh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.bbcook.cn/Article/details/gesgvtath.sHtML

[U70] PHP：PDO 事务
来源：http://baike.tarul.cn/Article/details/gowpywwwd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.sjlbkw.cn/Article/details/goaebqqwd.sHtML

[U71] PHP：抛出异常
来源：http://m.share.yfazqb.com/Article/details/gyjskxoko.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.epnwcf.com/Article/details/gwhiufcxm.sHtML

[U72] PHP：写错误日志
来源：http://baike.yfazqb.com/Article/details/gpurzzibb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fktsv.cn/Article/details/gdyhizmbz.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.bbcook.cn/Article/details/gzpffwhuf.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.bbcook.cn/Article/details/gpzigseih.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.bbcook.cn/Article/details/grxnjssnh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.sjlbkw.cn/Article/details/gxvoqzmtd.sHtML

[U75] PHP：依赖注入
来源：http://baike.vehdjk.com/Article/details/glwdtgsro.sHtML

composer require psr/container
来源：http://baike.epnwcf.com/Article/details/gggbinrly.sHtML

[U76] PHP：简单路由
来源：http://mobile.tarul.cn/Article/details/ghaezmxkz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fktsv.cn/Article/details/gttklmntf.sHtML

[U77] PHP：模板渲染
来源：http://wap.sjlbkw.cn/Article/details/giblzrzax.sHtML

composer require twig/twig
来源：http://wap.yfazqb.com/Article/details/gwbpqhzzo.sHtML

[U78] PHP：单元测试
来源：http://blog.yfazqb.com/Article/details/gfjxnotdf.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.tarul.cn/Article/details/glzwyqgrv.sHtML

[U79] PHP：静态分析
来源：http://blog.epnwcf.com/Article/details/gewlqcjam.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.yfazqb.com/Article/details/ghhrptxca.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.vehdjk.com/Article/details/gobgrvrbq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.epnwcf.com/Article/details/glburzeub.sHtML

[U81] JS：初始化项目
来源：http://wap.tarul.cn/Article/details/gtdaopghq.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fktsv.cn/Article/details/gesnuyyiq.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.epnwcf.com/Article/details/guameuliz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.epnwcf.com/Article/details/gujdylclm.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fktsv.cn/Article/details/ggpundusg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.vehdjk.com/Article/details/gsnqphepl.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.bbcook.cn/Article/details/gxuvrwiwg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.tarul.cn/Article/details/gpxunkodz.sHtML

[U85] JS：可选链
来源：http://3g.tarul.cn/Article/details/gmwtobpsz.sHtML

a?.b?.c
来源：http://www.share.tarul.cn/Article/details/gttmwozrc.sHtML

[U86] JS：空值合并
来源：http://www.m.share.bbcook.cn/Article/details/gxeapgich.sHtML

a ?? b
来源：http://3g.sjlbkw.cn/Article/details/gmuoylxjq.sHtML

[U87] JS：解构默认值
来源：http://read.share.epnwcf.com/Article/details/ghxakqvfc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.epnwcf.com/Article/details/grtcljyyp.sHtML

[U88] JS：对象展开合并
来源：http://3g.bbcook.cn/Article/details/gltngdmpg.sHtML

{ ...a, ...b }
来源：http://wap.bbcook.cn/Article/details/gmtwqoaoi.sHtML

[U89] JS：数组去重
来源：http://www.m.share.bbcook.cn/Article/details/gbdehkxqo.sHtML

[...new Set(arr)]
来源：http://blog.yfazqb.com/Article/details/ggiiwmyei.sHtML

[U90] JS：数字数组排序
来源：http://baike.tarul.cn/Article/details/gvbtiojng.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gnqospmop.sHtML

[U91] JS：对象键值遍历
来源：http://blog.bbcook.cn/Article/details/grckuncik.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.sjlbkw.cn/Article/details/gemboxxsb.sHtML

[U92] JS：深拷贝
来源：http://3g.fktsv.cn/Article/details/goemmtchu.sHtML

structuredClone(obj)
来源：http://blog.epnwcf.com/Article/details/gkqzdpwhp.sHtML

[U93] JS：模板字符串
来源：http://m.share.fktsv.cn/Article/details/gojydsxnt.sHtML

`共 ${n} 条`
来源：http://baike.sjlbkw.cn/Article/details/ghlhvjbqt.sHtML

[U94] JS：箭头函数
来源：http://3g.yfazqb.com/Article/details/ggemrmfco.sHtML

const double = x => x * 2;
来源：http://baike.epnwcf.com/Article/details/gbqqtqwxx.sHtML

[U95] JS：Promise 包装
来源：http://baike.vehdjk.com/Article/details/gnxogjnky.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.sjlbkw.cn/Article/details/gabqoalxa.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.epnwcf.com/Article/details/gepvqqprn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/gisiykqoy.sHtML

[U97] JS：并发请求
来源：http://wap.epnwcf.com/Article/details/gvhqpbynd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/gpaqlyqwy.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.yfazqb.com/Article/details/grlxvweje.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.epnwcf.com/Article/details/glfvoheex.sHtML

[U99] JS：事件监听
来源：http://blog.vehdjk.com/Article/details/gyqdvnktt.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.yfazqb.com/Article/details/ghdjmjatn.sHtML

[U100] JS：DOM 查询
来源：http://baike.fktsv.cn/Article/details/goagathdo.sHtML

document.querySelector(".item")
来源：http://baike.tarul.cn/Article/details/ghtveahxo.sHtML

[U101] JS：classList 操作
来源：http://m.share.fktsv.cn/Article/details/gfzulydhh.sHtML

el.classList.toggle("active")
来源：http://baike.fktsv.cn/Article/details/gblgdlfwi.sHtML

[U102] JS：本地存储
来源：http://www.share.bbcook.cn/Article/details/gqhbkgmtr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.epnwcf.com/Article/details/gjcutsvix.sHtML

[U103] JS：定时器
来源：http://wap.yfazqb.com/Article/details/gemnzlbul.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhdupgrb.sHtML

[U104] JS：防抖
来源：http://3g.tarul.cn/Article/details/gmrrulljt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.epnwcf.com/Article/details/gtvbasyui.sHtML

[U105] JS：节流
来源：http://baike.sjlbkw.cn/Article/details/gpobysvts.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.yfazqb.com/Article/details/gwsejymom.sHtML

[U106] JS：日期格式化
来源：http://m.share.fktsv.cn/Article/details/guywlwwgx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fktsv.cn/Article/details/gfmbcxrlb.sHtML

[U107] JS：数字千分位
来源：http://www.share.yfazqb.com/Article/details/gzdddmwdr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.tarul.cn/Article/details/gcjjscpek.sHtML

[U108] JS：随机整数
来源：http://read.share.epnwcf.com/Article/details/gicierljo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fktsv.cn/Article/details/gnpxkatci.sHtML

[U109] JS：数组分组
来源：http://baike.bbcook.cn/Article/details/gnqndxvpw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.vehdjk.com/Article/details/gxrjfhroh.sHtML

[U110] JS：数组分块
来源：http://wap.tarul.cn/Article/details/gogadtolz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.yfazqb.com/Article/details/gysdzmzyf.sHtML

[U111] JS：对象转 Map
来源：http://3g.bbcook.cn/Article/details/gwunzfcry.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.epnwcf.com/Article/details/gyalvkyqf.sHtML

[U112] JS：字符串补位
来源：http://m.share.yfazqb.com/Article/details/galpneolc.sHtML

"7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/geagbyyxg.sHtML

[U113] JS：正则替换全部
来源：http://baike.bbcook.cn/Article/details/gynodhbxh.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/ghlbviefb.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.tarul.cn/Article/details/gsawybfdk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fktsv.cn/Article/details/gebfxyjez.sHtML

[U115] JS：生成 UUID
来源：http://blog.fktsv.cn/Article/details/gjkeiwhem.sHtML

crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/gxpwxwusu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.epnwcf.com/Article/details/gzigkvmxz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.yfazqb.com/Article/details/gwjfrkkia.sHtML

[U117] JS：单元测试
来源：http://read.share.bbcook.cn/Article/details/gfnrlkicq.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.sjlbkw.cn/Article/details/gpucpilqw.sHtML

[U118] JS：开发服务器
来源：http://www.blog.bbcook.cn/Article/details/gldomsltw.sHtML

npm i -D vite;  npx vite
来源：http://blog.fktsv.cn/Article/details/gcfslkrsg.sHtML

[U119] JS：生产构建
来源：http://read.share.bbcook.cn/Article/details/gkgicjhig.sHtML

npx vite build
来源：http://m.share.tarul.cn/Article/details/gqzjsnrps.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.yfazqb.com/Article/details/gksmlopdi.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fktsv.cn/Article/details/gftcclzjz.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gcdyldrwr.sHtML

统计汇总
来源：http://www.m.share.vehdjk.com/Article/details/gbskehfwu.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/guzblystz.sHtML

按语言统计（条）：
来源：http://wap.fktsv.cn/Article/details/gsfrfjwxu.sHtML

Python ......... 252
来源：http://blog.tarul.cn/Article/details/giosdeiin.sHtML

PHP ............ 252
来源：http://www.share.yfazqb.com/Article/details/gwgszsrnk.sHtML

JavaScript ..... 252
来源：http://www.blog.vehdjk.com/Article/details/ghlzqnmhb.sHtML

TypeScript ..... 212
来源：http://3g.sjlbkw.cn/Article/details/gdusfajwz.sHtML

Java ........... 212
来源：http://3g.vehdjk.com/Article/details/ghqbzcvpw.sHtML

Go ............. 212
来源：http://www.blog.fktsv.cn/Article/details/gpbozbwmj.sHtML

Ruby ........... 212
来源：http://read.share.sjlbkw.cn/Article/details/gnyedhfpu.sHtML

C# ............. 212
来源：http://blog.fktsv.cn/Article/details/ggahircfm.sHtML

C .............. 30
来源：http://blog.tarul.cn/Article/details/gegasjuzp.sHtML

C++ ............ 30
来源：http://blog.tarul.cn/Article/details/gtibfvutv.sHtML

SQL ............ 90
来源：http://m.share.bbcook.cn/Article/details/gzpisqzkp.sHtML

Bash ........... 80
来源：http://baike.epnwcf.com/Article/details/gcalsuphd.sHtML

Kotlin ......... 15
来源：http://www.blog.fktsv.cn/Article/details/gwniktfeh.sHtML

Swift .......... 15
来源：http://baike.yfazqb.com/Article/details/gauyzeeef.sHtML

Lua ............ 10
来源：http://www.blog.sjlbkw.cn/Article/details/gpkzhshqw.sHtML

Perl ........... 10
来源：http://blog.epnwcf.com/Article/details/gfxwgnlcy.sHtML

Scala .......... 10
来源：http://www.share.tarul.cn/Article/details/gyidlgzwb.sHtML

------------------------------------
来源：http://read.share.epnwcf.com/Article/details/ghwljbyss.sHtML

合计 ........... 2106 条
来源：http://www.m.share.vehdjk.com/Article/details/gwuhxgqiz.sHtML

按章节统计：
来源：http://blog.sjlbkw.cn/Article/details/guzxsfkab.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.tarul.cn/Article/details/gqemxmpxb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.vehdjk.com/Article/details/gfslxpumr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.vehdjk.com/Article/details/gstyguggg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.tarul.cn/Article/details/gvonozdjx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.epnwcf.com/Article/details/gvnbafych.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.tarul.cn/Article/details/gxyarxucu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.yfazqb.com/Article/details/ggttyoome.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.tarul.cn/Article/details/gdrbewnkk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.epnwcf.com/Article/details/gktpiroli.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.tarul.cn/Article/details/grcrpcenj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gvsrtqroy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/ggszzogal.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gfelcqhss.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.epnwcf.com/Article/details/gcdjhbogf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.vehdjk.com/Article/details/gimwpxckt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gsegcvmyl.sHtML

Q SQL 专题                              90
来源：http://wap.tarul.cn/Article/details/gkptstyhy.sHtML

R Bash 专题                             80
来源：http://www.m.share.epnwcf.com/Article/details/guoxwzuhk.sHtML

S C / C++ 专题                          60
来源：http://read.share.yfazqb.com/Article/details/gljkyoiqd.sHtML

T 其他语言补充                          60
来源：http://baike.vehdjk.com/Article/details/gbaawdgew.sHtML

U 高频实用片段                         120
来源：http://www.share.yfazqb.com/Article/details/gikxktwxi.sHtML

------------------------------------
来源：http://3g.vehdjk.com/Article/details/gphanmphl.sHtML

合计                                  2106 条
来源：http://www.m.share.bbcook.cn/Article/details/gvucgpgrq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gadumiock.sHtML

使用提醒
来源：http://m.share.sjlbkw.cn/Article/details/gahamzsgn.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjgbujok.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.yfazqb.com/Article/details/gskwsxamv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fktsv.cn/Article/details/gkkmphsiy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.epnwcf.com/Article/details/gzslhtyha.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.vehdjk.com/Article/details/gqtwhrmyv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.yfazqb.com/Article/details/gqpbfzjhc.sHtML

—— 文件结束 ——
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmfyckiu.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gdsglkevs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.sjlbkw.cn/Article/details/gbftqzjjl.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.epnwcf.com/Article/details/gzsgbwlbz.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gripmwxsj.sHtML

【收录内容】
来源：http://wap.bbcook.cn/Article/details/gsxadqvxl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fktsv.cn/Article/details/gmwixfqav.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.sjlbkw.cn/Article/details/gllfqjzox.sHtML

SQL · Bash · C · C++
来源：http://www.share.epnwcf.com/Article/details/gvrmqveax.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.tarul.cn/Article/details/geiemeagh.sHtML

【使用说明】
来源：http://www.m.share.bbcook.cn/Article/details/gccabyszs.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.tarul.cn/Article/details/gxnlrbwwf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fktsv.cn/Article/details/gsnfifymd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.vehdjk.com/Article/details/gqtyzuhgf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.sjlbkw.cn/Article/details/guwolkeku.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.tarul.cn/Article/details/glsyzhwpp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.bbcook.cn/Article/details/geeskkckt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwvxbcmf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.sjlbkw.cn/Article/details/gmmvhfsly.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.sjlbkw.cn/Article/details/giqzouihi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.yfazqb.com/Article/details/gliuugfnv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.vehdjk.com/Article/details/gozagmkul.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxupfvry.sHtML

【文件统计】
来源：http://3g.bbcook.cn/Article/details/gagnomtlx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fktsv.cn/Article/details/gsbnhecwr.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gexgwthwd.sHtML

目  录
来源：http://read.share.epnwcf.com/Article/details/gynujutyr.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.yfazqb.com/Article/details/gdwukhbon.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.tarul.cn/Article/details/gkosidfng.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.bbcook.cn/Article/details/gjfirfmkr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.vehdjk.com/Article/details/gymygccez.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.bbcook.cn/Article/details/gnrrdlrzw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.yfazqb.com/Article/details/gwdqjotrc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.tarul.cn/Article/details/gthrtdjss.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.bbcook.cn/Article/details/gfiyrxrnq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.yfazqb.com/Article/details/gwxuveawv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/gvkjgavlo.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.bbcook.cn/Article/details/gorpuavoy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/ghuoqmrcw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/gcjasdxet.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/gnabfkgna.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.tarul.cn/Article/details/gzaxajuzh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fktsv.cn/Article/details/gjrztaoqe.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/gxdpocihk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.bbcook.cn/Article/details/gseokbvhp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.vehdjk.com/Article/details/gpmmsdzhm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.tarul.cn/Article/details/gzxbmldhi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.bbcook.cn/Article/details/gokoglakx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.sjlbkw.cn/Article/details/gyvytyhvs.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gvniiocbx.sHtML

A. 基础语法与类型
来源：http://www.blog.yfazqb.com/Article/details/gswnkelyc.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gsiyrodfx.sHtML

[A01] Hello World
来源：http://www.share.yfazqb.com/Article/details/grgpdafgf.sHtML

Py:   print("Hello, World!")
来源：http://baike.tarul.cn/Article/details/gedaiyrph.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.yfazqb.com/Article/details/grfklgtof.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.sjlbkw.cn/Article/details/gwissiveo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fktsv.cn/Article/details/gyiyffdon.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.epnwcf.com/Article/details/gkhjesmar.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.bbcook.cn/Article/details/gjppwmqgg.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.sjlbkw.cn/Article/details/gckkpcrbe.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fktsv.cn/Article/details/gokjzggry.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.sjlbkw.cn/Article/details/grxnhiemk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.yfazqb.com/Article/details/gwgztvksb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.bbcook.cn/Article/details/gqdzbixre.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.yfazqb.com/Article/details/gybsmkuba.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.sjlbkw.cn/Article/details/gsrnewisg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.yfazqb.com/Article/details/gcddmqyhc.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.vehdjk.com/Article/details/gjeziiytb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.tarul.cn/Article/details/gfpsaknug.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.epnwcf.com/Article/details/goxytfbop.sHtML

[A03] 常量定义
来源：http://baike.yfazqb.com/Article/details/gvytmwizh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.epnwcf.com/Article/details/gyvktcmtb.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gkmaiablx.sHtML

JS:   const PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gfjbpgsof.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gnchcuupq.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gzcqltwdk.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.tarul.cn/Article/details/glogczxhr.sHtML

Ruby: PI = 3.14159
来源：http://mobile.yfazqb.com/Article/details/gmibbwmgk.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gemjstqit.sHtML

[A04] 判断变量类型
来源：http://wap.tarul.cn/Article/details/gcwzwqzyi.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.bbcook.cn/Article/details/gshixawxc.sHtML


<!-- 参考信息 -->