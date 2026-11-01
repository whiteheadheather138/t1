代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://3g.bbcook.cn/Article/details/guymahued.sHtML

sys.stdout.isatty()
来源：http://read.share.vehdjk.com/Article/details/gcsrqzubh.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.sjlbkw.cn/Article/details/gmbqnbbcp.sHtML

print("err", file=sys.stderr)
来源：http://3g.sjlbkw.cn/Article/details/gibcxvbjs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.epnwcf.com/Article/details/gfabqrtmr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fktsv.cn/Article/details/gbabnguoi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.tarul.cn/Article/details/gzdskufiz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.bbcook.cn/Article/details/giykjzqez.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.vehdjk.com/Article/details/gopwkoakx.sHtML

namespace App\Http;
来源：http://read.share.yfazqb.com/Article/details/gxxjqmmgc.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fktsv.cn/Article/details/gwjkaqqin.sHtML

declare(strict_types=1);
来源：http://www.share.fktsv.cn/Article/details/gmpjyffqy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.bbcook.cn/Article/details/gfkxuspmr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gmbxjperb.sHtML

[U46] PHP：可空类型
来源：http://read.share.vehdjk.com/Article/details/gmqnqxshs.sHtML

?string $name = null
来源：http://baike.tarul.cn/Article/details/gpxkzwgjp.sHtML

[U47] PHP：联合类型
来源：http://www.blog.vehdjk.com/Article/details/giaqqhrxh.sHtML

int|string $id
来源：http://www.blog.epnwcf.com/Article/details/gmmclygmn.sHtML

[U48] PHP：纯枚举
来源：http://m.share.sjlbkw.cn/Article/details/gwjxjidab.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.vehdjk.com/Article/details/gxwcbacxr.sHtML

[U49] PHP：只读属性
来源：http://baike.yfazqb.com/Article/details/gwrvjxmbh.sHtML

public readonly string $name
来源：http://baike.yfazqb.com/Article/details/gidmxkixu.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.tarul.cn/Article/details/gxkvbwfla.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.vehdjk.com/Article/details/gmoizbanp.sHtML

[U51] PHP：数组解构
来源：http://wap.yfazqb.com/Article/details/gpxrjfuiq.sHtML

[$a, $b] = $arr;
来源：http://wap.vehdjk.com/Article/details/ggopmzgbb.sHtML

[U52] PHP：箭头函数
来源：http://3g.sjlbkw.cn/Article/details/gcuapkapj.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.tarul.cn/Article/details/gknwyrchw.sHtML

[U53] PHP：空合并运算符
来源：http://3g.tarul.cn/Article/details/gudmvlbcs.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.bbcook.cn/Article/details/gnqddtlig.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.tarul.cn/Article/details/gvpdgwmfi.sHtML

$obj?->method()
来源：http://blog.fktsv.cn/Article/details/gdpaitlhw.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.yfazqb.com/Article/details/gdgicqsev.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.vehdjk.com/Article/details/gilqieven.sHtML

[U56] PHP：命名参数
来源：http://read.share.vehdjk.com/Article/details/gqlzrcrks.sHtML

f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gkaqrcqdy.sHtML

[U57] PHP：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gmnxqrodo.sHtML

"值: {$a}"
来源：http://baike.tarul.cn/Article/details/gvjgxhgxq.sHtML

[U58] PHP：数组三件套
来源：http://blog.yfazqb.com/Article/details/gxgjpwaow.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.vehdjk.com/Article/details/gpmvtrsvs.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.tarul.cn/Article/details/gjmxjowle.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.epnwcf.com/Article/details/gffykaegp.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fktsv.cn/Article/details/gjbkqmwot.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.sjlbkw.cn/Article/details/gztphxhrc.sHtML

[U61] PHP：正则
来源：http://blog.vehdjk.com/Article/details/gemyflixn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.epnwcf.com/Article/details/geiffsjrh.sHtML

[U62] PHP：日期对象
来源：http://3g.sjlbkw.cn/Article/details/gjzqvsnbx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.bbcook.cn/Article/details/gapqatuab.sHtML

[U63] PHP：文件读写
来源：http://www.blog.tarul.cn/Article/details/gawjvbckq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.tarul.cn/Article/details/gwvjlvhhq.sHtML

[U64] PHP：目录遍历
来源：http://mobile.bbcook.cn/Article/details/gydwbebgi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.tarul.cn/Article/details/glacggrdl.sHtML

[U65] PHP：会话
来源：http://mobile.bbcook.cn/Article/details/gedvuspyy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.yfazqb.com/Article/details/gssctotgl.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.vehdjk.com/Article/details/gmckfssjj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.epnwcf.com/Article/details/gwjtyyltk.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.sjlbkw.cn/Article/details/gmimibidk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fktsv.cn/Article/details/gritjgavo.sHtML

[U68] PHP：PDO 连接
来源：http://3g.bbcook.cn/Article/details/gdzqggwjj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fktsv.cn/Article/details/guhawzeff.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.vehdjk.com/Article/details/gwtlctcut.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fktsv.cn/Article/details/gvfyryxza.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjhclkom.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.bbcook.cn/Article/details/gchcwrklh.sHtML

[U71] PHP：抛出异常
来源：http://blog.yfazqb.com/Article/details/glwvczgdi.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.epnwcf.com/Article/details/gerzhmqkk.sHtML

[U72] PHP：写错误日志
来源：http://3g.epnwcf.com/Article/details/gurtihtgi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.sjlbkw.cn/Article/details/gszaluhpk.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.sjlbkw.cn/Article/details/ghvqdfdcf.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fktsv.cn/Article/details/gyfcdyxzl.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.tarul.cn/Article/details/gmzkoybka.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fktsv.cn/Article/details/gnwmsgklg.sHtML

[U75] PHP：依赖注入
来源：http://baike.tarul.cn/Article/details/gxiizxvkt.sHtML

composer require psr/container
来源：http://www.share.bbcook.cn/Article/details/gkwietmdf.sHtML

[U76] PHP：简单路由
来源：http://m.share.yfazqb.com/Article/details/gkrhcoibc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.tarul.cn/Article/details/grdzuibxs.sHtML

[U77] PHP：模板渲染
来源：http://baike.fktsv.cn/Article/details/gcetaremt.sHtML

composer require twig/twig
来源：http://www.share.fktsv.cn/Article/details/gvtzckvwz.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.tarul.cn/Article/details/gfhwndgsm.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.vehdjk.com/Article/details/goupsbgam.sHtML

[U79] PHP：静态分析
来源：http://mobile.vehdjk.com/Article/details/gzrrkxtof.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.yfazqb.com/Article/details/gtdehaxxa.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fktsv.cn/Article/details/gklxshikj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.vehdjk.com/Article/details/ggkcgzmcg.sHtML

[U81] JS：初始化项目
来源：http://www.share.bbcook.cn/Article/details/gbvvnegty.sHtML

npm init -y;  npm i express
来源：http://baike.fktsv.cn/Article/details/gsydqgbny.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fktsv.cn/Article/details/gwfhvrous.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.bbcook.cn/Article/details/grrcqurvq.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.vehdjk.com/Article/details/grhetqndm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fktsv.cn/Article/details/gemoqtlya.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.yfazqb.com/Article/details/gtkyyxfds.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fktsv.cn/Article/details/gnbsttfuj.sHtML

[U85] JS：可选链
来源：http://read.share.vehdjk.com/Article/details/gfogceonh.sHtML

a?.b?.c
来源：http://read.share.bbcook.cn/Article/details/gpjeszmis.sHtML

[U86] JS：空值合并
来源：http://read.share.yfazqb.com/Article/details/gmoppjmqm.sHtML

a ?? b
来源：http://baike.fktsv.cn/Article/details/ggqarjpvd.sHtML

[U87] JS：解构默认值
来源：http://read.share.yfazqb.com/Article/details/gdfelwarm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.yfazqb.com/Article/details/gwntsopdf.sHtML

[U88] JS：对象展开合并
来源：http://m.share.sjlbkw.cn/Article/details/ghtytauho.sHtML

{ ...a, ...b }
来源：http://www.m.share.fktsv.cn/Article/details/grycybpqj.sHtML

[U89] JS：数组去重
来源：http://blog.tarul.cn/Article/details/guwezilzc.sHtML

[...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/glbhbjqvi.sHtML

[U90] JS：数字数组排序
来源：http://www.share.tarul.cn/Article/details/gfkxppded.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/gdyxsyufx.sHtML

[U91] JS：对象键值遍历
来源：http://baike.yfazqb.com/Article/details/gowcaphpx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.vehdjk.com/Article/details/gprkwqbfe.sHtML

[U92] JS：深拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/ginuqtjkk.sHtML

structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/gzmowxwaz.sHtML

[U93] JS：模板字符串
来源：http://www.blog.epnwcf.com/Article/details/gsekdaivy.sHtML

`共 ${n} 条`
来源：http://www.m.share.fktsv.cn/Article/details/guhkgiras.sHtML

[U94] JS：箭头函数
来源：http://wap.sjlbkw.cn/Article/details/gjkjbzmhg.sHtML

const double = x => x * 2;
来源：http://read.share.bbcook.cn/Article/details/gdanrbmhv.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.tarul.cn/Article/details/gmyyditev.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.epnwcf.com/Article/details/grfxuatao.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fktsv.cn/Article/details/gktlaoxbs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/gpumlakcr.sHtML

[U97] JS：并发请求
来源：http://baike.epnwcf.com/Article/details/gskxtkzml.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gvzdjknlx.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.vehdjk.com/Article/details/gqrevgjzd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.yfazqb.com/Article/details/gitffttif.sHtML

[U99] JS：事件监听
来源：http://www.m.share.epnwcf.com/Article/details/gwovwlnjg.sHtML

el.addEventListener("click", e => {})
来源：http://3g.yfazqb.com/Article/details/gyqrcyrlr.sHtML

[U100] JS：DOM 查询
来源：http://read.share.sjlbkw.cn/Article/details/gmggteydf.sHtML

document.querySelector(".item")
来源：http://www.share.fktsv.cn/Article/details/gxbdswjje.sHtML

[U101] JS：classList 操作
来源：http://mobile.vehdjk.com/Article/details/gsgsnypxp.sHtML

el.classList.toggle("active")
来源：http://blog.sjlbkw.cn/Article/details/golwrysaa.sHtML

[U102] JS：本地存储
来源：http://3g.tarul.cn/Article/details/gpajkiesm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.yfazqb.com/Article/details/gsrgjahrq.sHtML

[U103] JS：定时器
来源：http://m.share.sjlbkw.cn/Article/details/grddsnnap.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.epnwcf.com/Article/details/gmgfbiypk.sHtML

[U104] JS：防抖
来源：http://blog.fktsv.cn/Article/details/gycbvdbpt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/glzqfqwga.sHtML

[U105] JS：节流
来源：http://3g.sjlbkw.cn/Article/details/gavaawdtm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.epnwcf.com/Article/details/gvjflnowd.sHtML

[U106] JS：日期格式化
来源：http://wap.bbcook.cn/Article/details/geawnmaob.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.sjlbkw.cn/Article/details/gvjbmkukm.sHtML

[U107] JS：数字千分位
来源：http://m.share.tarul.cn/Article/details/gazmsmdzc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.epnwcf.com/Article/details/ghacojelk.sHtML

[U108] JS：随机整数
来源：http://m.share.vehdjk.com/Article/details/gdhwacttj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.yfazqb.com/Article/details/gxdfeezfc.sHtML

[U109] JS：数组分组
来源：http://www.blog.sjlbkw.cn/Article/details/giolyjgbm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.vehdjk.com/Article/details/gexevsbex.sHtML

[U110] JS：数组分块
来源：http://mobile.tarul.cn/Article/details/ggwegjdih.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.epnwcf.com/Article/details/gafdsrjoa.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.yfazqb.com/Article/details/gbggofpms.sHtML

new Map(Object.entries(obj))
来源：http://wap.tarul.cn/Article/details/gtsoauptu.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fktsv.cn/Article/details/ggxevoutf.sHtML

"7".padStart(3, "0")
来源：http://baike.fktsv.cn/Article/details/geokbsmxk.sHtML

[U113] JS：正则替换全部
来源：http://wap.vehdjk.com/Article/details/guhpbnitg.sHtML

s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gqiqzuxsk.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.epnwcf.com/Article/details/gafrvxopr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.tarul.cn/Article/details/gzfijhvir.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fktsv.cn/Article/details/gddawiaso.sHtML

crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gdqewxqcl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.bbcook.cn/Article/details/gvbwllmsf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.yfazqb.com/Article/details/gozcgrjev.sHtML

[U117] JS：单元测试
来源：http://baike.epnwcf.com/Article/details/gwukikvul.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.epnwcf.com/Article/details/gdifsgdov.sHtML

[U118] JS：开发服务器
来源：http://www.share.tarul.cn/Article/details/ggxidamdv.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fktsv.cn/Article/details/gupcgmnyl.sHtML

[U119] JS：生产构建
来源：http://baike.vehdjk.com/Article/details/gzsvtxpvi.sHtML

npx vite build
来源：http://wap.fktsv.cn/Article/details/gztzlgcrr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.sjlbkw.cn/Article/details/gvtilqnyz.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.sjlbkw.cn/Article/details/gimizzlii.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gnzkdxady.sHtML

统计汇总
来源：http://baike.yfazqb.com/Article/details/ghlaskdkc.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gkwhobymd.sHtML

按语言统计（条）：
来源：http://wap.yfazqb.com/Article/details/ghkfklkch.sHtML

Python ......... 252
来源：http://mobile.vehdjk.com/Article/details/gcqrtqupo.sHtML

PHP ............ 252
来源：http://3g.tarul.cn/Article/details/glstqjqko.sHtML

JavaScript ..... 252
来源：http://m.share.fktsv.cn/Article/details/gbooxirnt.sHtML

TypeScript ..... 212
来源：http://blog.vehdjk.com/Article/details/gyqkhwrex.sHtML

Java ........... 212
来源：http://baike.epnwcf.com/Article/details/goeqkdady.sHtML

Go ............. 212
来源：http://www.share.sjlbkw.cn/Article/details/gsyclixyy.sHtML

Ruby ........... 212
来源：http://read.share.fktsv.cn/Article/details/gcpymgjnw.sHtML

C# ............. 212
来源：http://3g.bbcook.cn/Article/details/gsqwmusii.sHtML

C .............. 30
来源：http://blog.tarul.cn/Article/details/gzmahqesz.sHtML

C++ ............ 30
来源：http://www.blog.fktsv.cn/Article/details/gbvsmyvcc.sHtML

SQL ............ 90
来源：http://www.blog.bbcook.cn/Article/details/gmlptzhhh.sHtML

Bash ........... 80
来源：http://www.m.share.tarul.cn/Article/details/gxqphsjwn.sHtML

Kotlin ......... 15
来源：http://mobile.epnwcf.com/Article/details/gywvezvce.sHtML

Swift .......... 15
来源：http://read.share.sjlbkw.cn/Article/details/gtvkpbfht.sHtML

Lua ............ 10
来源：http://wap.epnwcf.com/Article/details/gsjbilbnl.sHtML

Perl ........... 10
来源：http://3g.bbcook.cn/Article/details/gakdtzjqv.sHtML

Scala .......... 10
来源：http://blog.sjlbkw.cn/Article/details/gviqmdqyh.sHtML

------------------------------------
来源：http://blog.bbcook.cn/Article/details/gjxemdzcm.sHtML

合计 ........... 2106 条
来源：http://baike.sjlbkw.cn/Article/details/gyptjbayy.sHtML

按章节统计：
来源：http://mobile.sjlbkw.cn/Article/details/gonaqdxxo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.epnwcf.com/Article/details/gsubiqvgj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fktsv.cn/Article/details/gorgelrki.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.tarul.cn/Article/details/ghekccowu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.tarul.cn/Article/details/gvzxchtbj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.yfazqb.com/Article/details/gcpariwmt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.tarul.cn/Article/details/gbhrmnvfa.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.tarul.cn/Article/details/gkvboegcf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.vehdjk.com/Article/details/glvphhlxr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gdwewjjni.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.bbcook.cn/Article/details/gfpfxgkkz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/grrwikekj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gmrygqzmy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gqjyggfnz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.epnwcf.com/Article/details/gxoqpwtev.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.tarul.cn/Article/details/gqtqkkewq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/gfkxiknuo.sHtML

Q SQL 专题                              90
来源：http://read.share.sjlbkw.cn/Article/details/ggzvaunmw.sHtML

R Bash 专题                             80
来源：http://mobile.bbcook.cn/Article/details/gnltkpswk.sHtML

S C / C++ 专题                          60
来源：http://3g.epnwcf.com/Article/details/gecwthprn.sHtML

T 其他语言补充                          60
来源：http://www.m.share.epnwcf.com/Article/details/gtjwvxnur.sHtML

U 高频实用片段                         120
来源：http://www.share.bbcook.cn/Article/details/gkghbqcoy.sHtML

------------------------------------
来源：http://read.share.vehdjk.com/Article/details/gcvcksggv.sHtML

合计                                  2106 条
来源：http://m.share.bbcook.cn/Article/details/gbtfjfcsp.sHtML

--------------------------------------------------------------------------------
来源：http://wap.epnwcf.com/Article/details/gnewqmayn.sHtML

使用提醒
来源：http://3g.tarul.cn/Article/details/gritztzrr.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gulkmbskn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.sjlbkw.cn/Article/details/giuzydajk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.tarul.cn/Article/details/gfwzwvmxm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.tarul.cn/Article/details/gyxrlglas.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fktsv.cn/Article/details/gxaarcatu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.bbcook.cn/Article/details/gqpgnzddo.sHtML

—— 文件结束 ——
来源：http://www.share.bbcook.cn/Article/details/gblskanem.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gedwvxtan.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.vehdjk.com/Article/details/gpaoytuqj.sHtML

Common Programming Examples Cheat Book
来源：http://wap.epnwcf.com/Article/details/gzosqfjto.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gzrksgaso.sHtML

【收录内容】
来源：http://www.share.tarul.cn/Article/details/gidvpeaht.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.vehdjk.com/Article/details/glrlesyrv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.vehdjk.com/Article/details/gedtvsfzx.sHtML

SQL · Bash · C · C++
来源：http://wap.fktsv.cn/Article/details/gdsrxqrua.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.vehdjk.com/Article/details/gueosrmsw.sHtML

【使用说明】
来源：http://www.m.share.bbcook.cn/Article/details/gxwlzvpfy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.yfazqb.com/Article/details/gqsufeuhf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fktsv.cn/Article/details/gkxxszkuk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.sjlbkw.cn/Article/details/gojlsoguw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.tarul.cn/Article/details/ghncxrshl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fktsv.cn/Article/details/gkwnrspuq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.tarul.cn/Article/details/giaqgvjkl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.yfazqb.com/Article/details/gtrpipiyj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.yfazqb.com/Article/details/geremdmda.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.epnwcf.com/Article/details/gfiagbvlh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.vehdjk.com/Article/details/ggbbioaud.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.epnwcf.com/Article/details/gzrqglpld.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.bbcook.cn/Article/details/gxwvmgrrx.sHtML

【文件统计】
来源：http://www.blog.vehdjk.com/Article/details/gerjzhyiw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fktsv.cn/Article/details/gftlidxew.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/gmxepypwk.sHtML

目  录
来源：http://3g.bbcook.cn/Article/details/grfmeljqs.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gwvomqthj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.epnwcf.com/Article/details/gyagtpjas.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.vehdjk.com/Article/details/gcqqaobjd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.vehdjk.com/Article/details/gjjiblpnd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.epnwcf.com/Article/details/gwiminxqf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.yfazqb.com/Article/details/gyueqxibt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.yfazqb.com/Article/details/gblhbwavc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/gdpsanala.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.yfazqb.com/Article/details/gcxpzacjf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/gqpwawnya.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.vehdjk.com/Article/details/gskrvfdhi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.yfazqb.com/Article/details/gplverlni.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.yfazqb.com/Article/details/gqehsmjgl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/gxwydyulv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.sjlbkw.cn/Article/details/gfevsjepv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.bbcook.cn/Article/details/gkbmzmbku.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gnwaxlotj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.bbcook.cn/Article/details/gpiykxqnc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.vehdjk.com/Article/details/gwjjqtwac.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.sjlbkw.cn/Article/details/ghwxgjnyi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.epnwcf.com/Article/details/guuxthgji.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.tarul.cn/Article/details/ggigeutky.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gnfurnmpo.sHtML

A. 基础语法与类型
来源：http://3g.fktsv.cn/Article/details/gaozemdvk.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gwoemnfjg.sHtML

[A01] Hello World
来源：http://www.share.yfazqb.com/Article/details/gqvysxyof.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.sjlbkw.cn/Article/details/goiehwoph.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.tarul.cn/Article/details/gcfpjyrod.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.tarul.cn/Article/details/gjytlmiav.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.epnwcf.com/Article/details/gdyswkbxh.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.vehdjk.com/Article/details/gmeavffky.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.vehdjk.com/Article/details/gqgtluwqy.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.bbcook.cn/Article/details/gpaeoccvq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fktsv.cn/Article/details/gnhdennlu.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fktsv.cn/Article/details/ghloljhon.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.yfazqb.com/Article/details/gsjjdakvn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.epnwcf.com/Article/details/ggothjabv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.tarul.cn/Article/details/gztkinlep.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.sjlbkw.cn/Article/details/gjuhpjhcx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/greerdtrl.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.yfazqb.com/Article/details/gpbbmyqqy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.epnwcf.com/Article/details/gubugwbpe.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.tarul.cn/Article/details/gwdwomgsh.sHtML

[A03] 常量定义
来源：http://m.share.yfazqb.com/Article/details/gkkmzghrc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.yfazqb.com/Article/details/gwelvdsgb.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gtdosvqko.sHtML

JS:   const PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gaxhrhpec.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.tarul.cn/Article/details/gajopdhyl.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/ghuvwpvrk.sHtML

Go:   const PI = 3.14159
来源：http://www.share.yfazqb.com/Article/details/gxculzcen.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.bbcook.cn/Article/details/gbgydbkde.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gdfvjenmj.sHtML

[A04] 判断变量类型
来源：http://www.share.sjlbkw.cn/Article/details/gqvwiuuto.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gczukorlh.sHtML


<!-- 参考信息 -->