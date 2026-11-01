代发 wailian999

[U37] Py：读写 Excel
来源：http://blog.bbcook.cn/Article/details/gaozwfehn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.sjlbkw.cn/Article/details/genivxobz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.epnwcf.com/Article/details/gbfhjxuhs.sHtML

Path(__file__).resolve().parent
来源：http://wap.fktsv.cn/Article/details/gxsnqmpvq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fktsv.cn/Article/details/gmcgjfxkb.sHtML

sys.stdout.isatty()
来源：http://3g.epnwcf.com/Article/details/gofmxxzxj.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.vehdjk.com/Article/details/gjcatyjae.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpppcreah.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.tarul.cn/Article/details/gvwyqoaiz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fktsv.cn/Article/details/gmnzneyof.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.yfazqb.com/Article/details/gsvzzuwxb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.sjlbkw.cn/Article/details/girmabciq.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fktsv.cn/Article/details/gmyseeemj.sHtML

namespace App\Http;
来源：http://www.m.share.tarul.cn/Article/details/gksqkcumz.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.vehdjk.com/Article/details/gluiysnqu.sHtML

declare(strict_types=1);
来源：http://www.m.share.yfazqb.com/Article/details/gnwvzxsum.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.sjlbkw.cn/Article/details/gfmnjsyax.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gpfidzkhh.sHtML

[U46] PHP：可空类型
来源：http://blog.yfazqb.com/Article/details/gwgpyjifx.sHtML

?string $name = null
来源：http://wap.fktsv.cn/Article/details/gmxsgjeko.sHtML

[U47] PHP：联合类型
来源：http://read.share.fktsv.cn/Article/details/gmiqypkmy.sHtML

int|string $id
来源：http://mobile.epnwcf.com/Article/details/gzoeprdhy.sHtML

[U48] PHP：纯枚举
来源：http://read.share.tarul.cn/Article/details/gjqnhuzfc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.tarul.cn/Article/details/gaewtzkpf.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.sjlbkw.cn/Article/details/guzgyihch.sHtML

public readonly string $name
来源：http://wap.sjlbkw.cn/Article/details/gckybafdl.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.yfazqb.com/Article/details/gjywkteti.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.epnwcf.com/Article/details/gwpwhxisy.sHtML

[U51] PHP：数组解构
来源：http://wap.sjlbkw.cn/Article/details/gporrsokd.sHtML

[$a, $b] = $arr;
来源：http://blog.vehdjk.com/Article/details/gsulojbze.sHtML

[U52] PHP：箭头函数
来源：http://www.share.yfazqb.com/Article/details/gqpmsydev.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.sjlbkw.cn/Article/details/gadpkmypj.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fktsv.cn/Article/details/gqxfnwoay.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.epnwcf.com/Article/details/gtaiyxgqv.sHtML

[U54] PHP：空安全调用
来源：http://wap.vehdjk.com/Article/details/gphhyryrs.sHtML

$obj?->method()
来源：http://baike.bbcook.cn/Article/details/gdlvfvbov.sHtML

[U55] PHP：match 表达式
来源：http://www.share.bbcook.cn/Article/details/gytytmsfi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fktsv.cn/Article/details/gbuhtjmdk.sHtML

[U56] PHP：命名参数
来源：http://m.share.tarul.cn/Article/details/gvzwhulfw.sHtML

f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/gzacyoptu.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gywnltcfz.sHtML

"值: {$a}"
来源：http://baike.vehdjk.com/Article/details/giiymhpgl.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.sjlbkw.cn/Article/details/gnbnbaplb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.epnwcf.com/Article/details/gisqzofly.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fktsv.cn/Article/details/gulbupymy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.bbcook.cn/Article/details/graoefkzh.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.epnwcf.com/Article/details/goqczozvl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.vehdjk.com/Article/details/gfprgqwsj.sHtML

[U61] PHP：正则
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpmcixno.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fktsv.cn/Article/details/gcbvkxzxq.sHtML

[U62] PHP：日期对象
来源：http://www.blog.yfazqb.com/Article/details/gcokmbiqs.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.epnwcf.com/Article/details/gzjcssyxg.sHtML

[U63] PHP：文件读写
来源：http://blog.tarul.cn/Article/details/gkrnhcafb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fktsv.cn/Article/details/gnbkcvcdd.sHtML

[U64] PHP：目录遍历
来源：http://baike.yfazqb.com/Article/details/grotaqlcq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.vehdjk.com/Article/details/gqpcbnjbd.sHtML

[U65] PHP：会话
来源：http://mobile.fktsv.cn/Article/details/gkusmdiob.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.tarul.cn/Article/details/gaymiefni.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fktsv.cn/Article/details/glvjuaczb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.tarul.cn/Article/details/gdmobrvkl.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.tarul.cn/Article/details/guyeiskem.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.sjlbkw.cn/Article/details/gpgargccm.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.tarul.cn/Article/details/gjvyzwylv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.bbcook.cn/Article/details/giphvuwdz.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.tarul.cn/Article/details/gszxnomsq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.vehdjk.com/Article/details/gdwqlpbmd.sHtML

[U70] PHP：PDO 事务
来源：http://3g.sjlbkw.cn/Article/details/gosronfch.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.yfazqb.com/Article/details/gcndyoacf.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/gajskttth.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fktsv.cn/Article/details/gwrffjjyi.sHtML

[U72] PHP：写错误日志
来源：http://read.share.vehdjk.com/Article/details/gigfrhypt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.vehdjk.com/Article/details/gfzjkxari.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.yfazqb.com/Article/details/ghmqsbnqb.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.tarul.cn/Article/details/gnvpsjjyh.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.vehdjk.com/Article/details/gccboqxnc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.vehdjk.com/Article/details/gokaecwve.sHtML

[U75] PHP：依赖注入
来源：http://mobile.epnwcf.com/Article/details/gbyqsoavc.sHtML

composer require psr/container
来源：http://baike.tarul.cn/Article/details/gvqucphrz.sHtML

[U76] PHP：简单路由
来源：http://3g.tarul.cn/Article/details/gacarndsk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.tarul.cn/Article/details/gbqrfuqcv.sHtML

[U77] PHP：模板渲染
来源：http://mobile.vehdjk.com/Article/details/gsgmjnvmd.sHtML

composer require twig/twig
来源：http://mobile.bbcook.cn/Article/details/gykwxnkoa.sHtML

[U78] PHP：单元测试
来源：http://wap.epnwcf.com/Article/details/ggxptknkk.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.tarul.cn/Article/details/gvypdeudz.sHtML

[U79] PHP：静态分析
来源：http://read.share.sjlbkw.cn/Article/details/ggbyrokyi.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.sjlbkw.cn/Article/details/gkxkezhpe.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fktsv.cn/Article/details/gikdopprq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.tarul.cn/Article/details/ghdgyjoyl.sHtML

[U81] JS：初始化项目
来源：http://blog.tarul.cn/Article/details/gkyghpwxr.sHtML

npm init -y;  npm i express
来源：http://m.share.yfazqb.com/Article/details/gvkclhksf.sHtML

[U82] JS：package.json 脚本
来源：http://baike.vehdjk.com/Article/details/gjhkgtshj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.sjlbkw.cn/Article/details/gujdwhzjw.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.vehdjk.com/Article/details/ghkdwrxhl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.epnwcf.com/Article/details/gstrpuknl.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.tarul.cn/Article/details/gqquwvwgi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.vehdjk.com/Article/details/gbtdcqush.sHtML

[U85] JS：可选链
来源：http://read.share.fktsv.cn/Article/details/gxccwjmmg.sHtML

a?.b?.c
来源：http://read.share.epnwcf.com/Article/details/gbzlnqemm.sHtML

[U86] JS：空值合并
来源：http://www.blog.tarul.cn/Article/details/gfocmorot.sHtML

a ?? b
来源：http://read.share.yfazqb.com/Article/details/gnnuescer.sHtML

[U87] JS：解构默认值
来源：http://wap.fktsv.cn/Article/details/guijabolb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.bbcook.cn/Article/details/gcmxtrgcr.sHtML

[U88] JS：对象展开合并
来源：http://mobile.vehdjk.com/Article/details/gtnkeiiax.sHtML

{ ...a, ...b }
来源：http://baike.vehdjk.com/Article/details/gplqwgbqw.sHtML

[U89] JS：数组去重
来源：http://3g.fktsv.cn/Article/details/geejzokfr.sHtML

[...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/gkdsjbiuy.sHtML

[U90] JS：数字数组排序
来源：http://www.share.yfazqb.com/Article/details/gnvemqmbo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/ggazgduwi.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fktsv.cn/Article/details/gjggnqohn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.tarul.cn/Article/details/gccurxpil.sHtML

[U92] JS：深拷贝
来源：http://baike.vehdjk.com/Article/details/gyqxnhdzj.sHtML

structuredClone(obj)
来源：http://www.share.bbcook.cn/Article/details/galnzdvou.sHtML

[U93] JS：模板字符串
来源：http://read.share.vehdjk.com/Article/details/gbkugsmsa.sHtML

`共 ${n} 条`
来源：http://wap.epnwcf.com/Article/details/gervmytgm.sHtML

[U94] JS：箭头函数
来源：http://m.share.bbcook.cn/Article/details/gnjkuuyvx.sHtML

const double = x => x * 2;
来源：http://mobile.sjlbkw.cn/Article/details/gktdgtvol.sHtML

[U95] JS：Promise 包装
来源：http://www.share.epnwcf.com/Article/details/gdotihbdu.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.vehdjk.com/Article/details/gwwsqwfdx.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.yfazqb.com/Article/details/gljciqaax.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gmwzukdlo.sHtML

[U97] JS：并发请求
来源：http://www.share.sjlbkw.cn/Article/details/gwgshxlvl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/ggffsgszu.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.tarul.cn/Article/details/gwzxoidaj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.tarul.cn/Article/details/gxtbtckei.sHtML

[U99] JS：事件监听
来源：http://www.blog.fktsv.cn/Article/details/gacvxshxp.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.tarul.cn/Article/details/gxxqhzycq.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fktsv.cn/Article/details/gbkrvkihh.sHtML

document.querySelector(".item")
来源：http://m.share.fktsv.cn/Article/details/gznezeqhf.sHtML

[U101] JS：classList 操作
来源：http://baike.epnwcf.com/Article/details/guzxknfwt.sHtML

el.classList.toggle("active")
来源：http://www.m.share.sjlbkw.cn/Article/details/gufytrjif.sHtML

[U102] JS：本地存储
来源：http://3g.fktsv.cn/Article/details/gtfgcwxiz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.tarul.cn/Article/details/gznjolbmo.sHtML

[U103] JS：定时器
来源：http://3g.bbcook.cn/Article/details/gouosbxsx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.bbcook.cn/Article/details/giptobbug.sHtML

[U104] JS：防抖
来源：http://baike.vehdjk.com/Article/details/gewgvxhbu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fktsv.cn/Article/details/gitwdzsqa.sHtML

[U105] JS：节流
来源：http://www.blog.yfazqb.com/Article/details/gkffhnedv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.bbcook.cn/Article/details/gyrfhxdnh.sHtML

[U106] JS：日期格式化
来源：http://mobile.bbcook.cn/Article/details/gfncgjper.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.yfazqb.com/Article/details/gpenzygkl.sHtML

[U107] JS：数字千分位
来源：http://baike.sjlbkw.cn/Article/details/gjthqgkrt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.yfazqb.com/Article/details/gcygqsfqn.sHtML

[U108] JS：随机整数
来源：http://baike.fktsv.cn/Article/details/gfdgzgvet.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fktsv.cn/Article/details/gozmnbopl.sHtML

[U109] JS：数组分组
来源：http://www.share.fktsv.cn/Article/details/gmqjkpfwy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.tarul.cn/Article/details/gistftvmh.sHtML

[U110] JS：数组分块
来源：http://blog.vehdjk.com/Article/details/gjzxmapik.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.epnwcf.com/Article/details/gcextoswy.sHtML

[U111] JS：对象转 Map
来源：http://blog.epnwcf.com/Article/details/gpqgacbfs.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fktsv.cn/Article/details/ghraexzpf.sHtML

[U112] JS：字符串补位
来源：http://m.share.vehdjk.com/Article/details/gdukgbzku.sHtML

"7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gwilrtukm.sHtML

[U113] JS：正则替换全部
来源：http://m.share.vehdjk.com/Article/details/gbjqnanrg.sHtML

s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gtctnwvii.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.yfazqb.com/Article/details/gcwukxoul.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.bbcook.cn/Article/details/gxiyrxejk.sHtML

[U115] JS：生成 UUID
来源：http://mobile.tarul.cn/Article/details/gxyfffcwt.sHtML

crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/gngcfiofs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.vehdjk.com/Article/details/gculgnvxl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.yfazqb.com/Article/details/gtvivvjiz.sHtML

[U117] JS：单元测试
来源：http://m.share.tarul.cn/Article/details/gmtxmuzup.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.sjlbkw.cn/Article/details/gibvfgieq.sHtML

[U118] JS：开发服务器
来源：http://blog.epnwcf.com/Article/details/gqpozjpof.sHtML

npm i -D vite;  npx vite
来源：http://3g.bbcook.cn/Article/details/gfmhlfgob.sHtML

[U119] JS：生产构建
来源：http://www.blog.tarul.cn/Article/details/glihccxhh.sHtML

npx vite build
来源：http://read.share.vehdjk.com/Article/details/gmczooedd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.epnwcf.com/Article/details/gihfiskgb.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.tarul.cn/Article/details/glqboudyi.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gyyshgocm.sHtML

统计汇总
来源：http://wap.vehdjk.com/Article/details/gpcxjihkh.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ggxxdbckj.sHtML

按语言统计（条）：
来源：http://wap.fktsv.cn/Article/details/gsbadxrdu.sHtML

Python ......... 252
来源：http://www.blog.epnwcf.com/Article/details/gszckjxyg.sHtML

PHP ............ 252
来源：http://baike.sjlbkw.cn/Article/details/gfddxwqol.sHtML

JavaScript ..... 252
来源：http://baike.fktsv.cn/Article/details/gjrgvxack.sHtML

TypeScript ..... 212
来源：http://read.share.fktsv.cn/Article/details/gucsbvmbd.sHtML

Java ........... 212
来源：http://www.m.share.bbcook.cn/Article/details/gygcjextp.sHtML

Go ............. 212
来源：http://baike.fktsv.cn/Article/details/gskisjuol.sHtML

Ruby ........... 212
来源：http://mobile.fktsv.cn/Article/details/gekxxryzh.sHtML

C# ............. 212
来源：http://www.share.vehdjk.com/Article/details/gmmpmvycb.sHtML

C .............. 30
来源：http://www.m.share.bbcook.cn/Article/details/gkcddrnry.sHtML

C++ ............ 30
来源：http://blog.vehdjk.com/Article/details/gppcliyhq.sHtML

SQL ............ 90
来源：http://baike.sjlbkw.cn/Article/details/gdltdjfbq.sHtML

Bash ........... 80
来源：http://m.share.fktsv.cn/Article/details/gbbabnmex.sHtML

Kotlin ......... 15
来源：http://read.share.vehdjk.com/Article/details/gofsfrzud.sHtML

Swift .......... 15
来源：http://blog.epnwcf.com/Article/details/gxmeejyah.sHtML

Lua ............ 10
来源：http://m.share.sjlbkw.cn/Article/details/gxdudpbsf.sHtML

Perl ........... 10
来源：http://read.share.sjlbkw.cn/Article/details/gvvsormdc.sHtML

Scala .......... 10
来源：http://baike.epnwcf.com/Article/details/gwesmmgnf.sHtML

------------------------------------
来源：http://3g.yfazqb.com/Article/details/gawopqyxu.sHtML

合计 ........... 2106 条
来源：http://www.share.bbcook.cn/Article/details/gpzhsblmy.sHtML

按章节统计：
来源：http://baike.tarul.cn/Article/details/gyvougsxa.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.yfazqb.com/Article/details/gsjguofvk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.epnwcf.com/Article/details/gdftfycjx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/glqecyroc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.vehdjk.com/Article/details/gxcqqkseh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.bbcook.cn/Article/details/guqxaegcp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fktsv.cn/Article/details/giifnmjua.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.sjlbkw.cn/Article/details/gshbkwyru.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.tarul.cn/Article/details/gjhdhowmi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gufrqkhpi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.bbcook.cn/Article/details/gectasksp.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/gjpqrebfa.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gacolpyht.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.epnwcf.com/Article/details/gmwsamvae.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.vehdjk.com/Article/details/ghwbpizuz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.vehdjk.com/Article/details/girmbyedg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fktsv.cn/Article/details/gcgcnrcal.sHtML

Q SQL 专题                              90
来源：http://www.m.share.tarul.cn/Article/details/gloancsic.sHtML

R Bash 专题                             80
来源：http://www.m.share.sjlbkw.cn/Article/details/genoazmna.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fktsv.cn/Article/details/gpdoxoglm.sHtML

T 其他语言补充                          60
来源：http://www.blog.vehdjk.com/Article/details/gynngqsob.sHtML

U 高频实用片段                         120
来源：http://blog.yfazqb.com/Article/details/gsosjavar.sHtML

------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gmcumvwyj.sHtML

合计                                  2106 条
来源：http://m.share.epnwcf.com/Article/details/gvnbgtcfc.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.epnwcf.com/Article/details/gnpeuhnul.sHtML

使用提醒
来源：http://www.m.share.vehdjk.com/Article/details/glqbquaad.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.tarul.cn/Article/details/gubxhhspr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.vehdjk.com/Article/details/grkpueqoh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.epnwcf.com/Article/details/gytmqxmjd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.bbcook.cn/Article/details/gzksjfvjv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.tarul.cn/Article/details/gqzffyypl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.tarul.cn/Article/details/gogwfvavx.sHtML

—— 文件结束 ——
来源：http://mobile.yfazqb.com/Article/details/gtpgnamej.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gkizthynv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.epnwcf.com/Article/details/gptuzghbm.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fktsv.cn/Article/details/gsgscnqwk.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gvjtuvxnn.sHtML

【收录内容】
来源：http://www.blog.epnwcf.com/Article/details/gjowwgvqb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.epnwcf.com/Article/details/gxknzawta.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.tarul.cn/Article/details/gnlnammmi.sHtML

SQL · Bash · C · C++
来源：http://wap.yfazqb.com/Article/details/gmlnaxwfi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.tarul.cn/Article/details/glhuxjfqi.sHtML

【使用说明】
来源：http://read.share.tarul.cn/Article/details/gjabhbiyr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.vehdjk.com/Article/details/guqrwqwnz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fktsv.cn/Article/details/gsajefpgj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.sjlbkw.cn/Article/details/gyipleteb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.vehdjk.com/Article/details/gypzvivtq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.yfazqb.com/Article/details/ggzxdqqkp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.yfazqb.com/Article/details/gyclfqsbu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.tarul.cn/Article/details/goklmjost.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.tarul.cn/Article/details/gszfvnjyz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.epnwcf.com/Article/details/gjwsnnlnv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fktsv.cn/Article/details/gdsharslo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtnecvar.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.epnwcf.com/Article/details/gkfroujus.sHtML

【文件统计】
来源：http://wap.fktsv.cn/Article/details/ggecpmydw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.vehdjk.com/Article/details/gxfjkhrrr.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.yfazqb.com/Article/details/gthvqxpqp.sHtML

目  录
来源：http://www.share.tarul.cn/Article/details/gbtlelkpu.sHtML

--------------------------------------------------------------------------------
来源：http://baike.vehdjk.com/Article/details/gelcivkvj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.sjlbkw.cn/Article/details/gyzusfrho.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.yfazqb.com/Article/details/gtmwraomo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.sjlbkw.cn/Article/details/gtecbwmpx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.bbcook.cn/Article/details/grbzdawkh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.epnwcf.com/Article/details/gjgjsvapz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.vehdjk.com/Article/details/gfjqvfwmz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.epnwcf.com/Article/details/gybwcqqrb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.yfazqb.com/Article/details/gbeijgkll.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fktsv.cn/Article/details/gxlcqbnpc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fktsv.cn/Article/details/gdiioxodh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/gxjgiwiko.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.epnwcf.com/Article/details/gxkgkjzkq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/gwdjabzpa.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.sjlbkw.cn/Article/details/gcqfyvpxv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fktsv.cn/Article/details/gibfxtvld.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.vehdjk.com/Article/details/gnmuajyem.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.sjlbkw.cn/Article/details/gnbhidvts.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.vehdjk.com/Article/details/gdiaxuimd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.sjlbkw.cn/Article/details/gilqzlmcs.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.yfazqb.com/Article/details/giutkvvec.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.tarul.cn/Article/details/gouvqyyrv.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ghjlyalod.sHtML

A. 基础语法与类型
来源：http://wap.bbcook.cn/Article/details/gvtxobojw.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gzewlfhrg.sHtML

[A01] Hello World
来源：http://m.share.epnwcf.com/Article/details/grxpcfzow.sHtML

Py:   print("Hello, World!")
来源：http://read.share.tarul.cn/Article/details/govieebea.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.epnwcf.com/Article/details/gycyttzrk.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.yfazqb.com/Article/details/gsqsyujia.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.sjlbkw.cn/Article/details/giwqigudn.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.tarul.cn/Article/details/gssrmknzj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.tarul.cn/Article/details/gxcdugpxp.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.vehdjk.com/Article/details/gzistpvph.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.sjlbkw.cn/Article/details/gocjqqdwd.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.yfazqb.com/Article/details/gyeywlaft.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.vehdjk.com/Article/details/gqtrpmpgy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.sjlbkw.cn/Article/details/gguitdtxd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.sjlbkw.cn/Article/details/gjfzwpmyc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.vehdjk.com/Article/details/ghulrtfku.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.sjlbkw.cn/Article/details/gpjitarba.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.bbcook.cn/Article/details/glbbnosat.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.epnwcf.com/Article/details/glkcnigfs.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.sjlbkw.cn/Article/details/ganundysf.sHtML

[A03] 常量定义
来源：http://3g.tarul.cn/Article/details/gjkhyftmb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.yfazqb.com/Article/details/gnzmxfgmo.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gqtviysai.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gpseeocnu.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gugmtugyi.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gcjrxoljc.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.tarul.cn/Article/details/gcxbnkpkz.sHtML


<!-- 参考信息 -->