代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://read.share.epnwcf.com/Article/details/gzsquywkk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.yfazqb.com/Article/details/gygpzlbuu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.epnwcf.com/Article/details/glntbtewz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.tarul.cn/Article/details/gjydkyowo.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fktsv.cn/Article/details/gaikojhlf.sHtML

namespace App\Http;
来源：http://www.blog.sjlbkw.cn/Article/details/gkfbgdytc.sHtML

[U44] PHP：开启严格类型
来源：http://baike.bbcook.cn/Article/details/gvzgiyujd.sHtML

declare(strict_types=1);
来源：http://www.share.tarul.cn/Article/details/ghhgexmya.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.epnwcf.com/Article/details/ggalhmqne.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gfagevvmi.sHtML

[U46] PHP：可空类型
来源：http://baike.fktsv.cn/Article/details/gxrrakvms.sHtML

?string $name = null
来源：http://baike.epnwcf.com/Article/details/gpmcikpzm.sHtML

[U47] PHP：联合类型
来源：http://www.share.yfazqb.com/Article/details/gpvqgnndu.sHtML

int|string $id
来源：http://read.share.yfazqb.com/Article/details/gnamfevhn.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gwpjzligs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.tarul.cn/Article/details/gzfglmvlf.sHtML

[U49] PHP：只读属性
来源：http://blog.sjlbkw.cn/Article/details/gxbfkylsa.sHtML

public readonly string $name
来源：http://www.blog.tarul.cn/Article/details/gvhlejcts.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.bbcook.cn/Article/details/gtibjqfbe.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fktsv.cn/Article/details/gfqojhdwx.sHtML

[U51] PHP：数组解构
来源：http://mobile.tarul.cn/Article/details/gnxyuvzjs.sHtML

[$a, $b] = $arr;
来源：http://wap.fktsv.cn/Article/details/gpjkrktdm.sHtML

[U52] PHP：箭头函数
来源：http://mobile.epnwcf.com/Article/details/gfskkyrcu.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.sjlbkw.cn/Article/details/gpcqlnylk.sHtML

[U53] PHP：空合并运算符
来源：http://wap.vehdjk.com/Article/details/gsmmegftl.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.tarul.cn/Article/details/gofbunoct.sHtML

[U54] PHP：空安全调用
来源：http://m.share.vehdjk.com/Article/details/gdsucuwig.sHtML

$obj?->method()
来源：http://read.share.yfazqb.com/Article/details/gxkpikvyi.sHtML

[U55] PHP：match 表达式
来源：http://m.share.vehdjk.com/Article/details/gymsbufhu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.epnwcf.com/Article/details/gbvhyvork.sHtML

[U56] PHP：命名参数
来源：http://www.blog.bbcook.cn/Article/details/gncyrxjif.sHtML

f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/guhvnhpdt.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gudkrwvac.sHtML

"值: {$a}"
来源：http://3g.vehdjk.com/Article/details/gmgwersec.sHtML

[U58] PHP：数组三件套
来源：http://mobile.bbcook.cn/Article/details/gmenirmnp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.tarul.cn/Article/details/gojskaoly.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fktsv.cn/Article/details/gngvbzgqf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.vehdjk.com/Article/details/gitshmszv.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.epnwcf.com/Article/details/gysfglwce.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.sjlbkw.cn/Article/details/gbocmpnab.sHtML

[U61] PHP：正则
来源：http://baike.fktsv.cn/Article/details/gagzwqjfb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.epnwcf.com/Article/details/gadfmvxwk.sHtML

[U62] PHP：日期对象
来源：http://baike.yfazqb.com/Article/details/gtympmudb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.epnwcf.com/Article/details/gpeejhlzv.sHtML

[U63] PHP：文件读写
来源：http://m.share.bbcook.cn/Article/details/gzotwtefd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fktsv.cn/Article/details/gbhipnpot.sHtML

[U64] PHP：目录遍历
来源：http://mobile.sjlbkw.cn/Article/details/gecrsmsyc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.sjlbkw.cn/Article/details/grluwdbuk.sHtML

[U65] PHP：会话
来源：http://www.share.epnwcf.com/Article/details/gpozwpjyh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.tarul.cn/Article/details/ggaxdgcys.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.sjlbkw.cn/Article/details/gcgfctjow.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.epnwcf.com/Article/details/glzcopejr.sHtML

[U67] PHP：处理文件上传
来源：http://baike.sjlbkw.cn/Article/details/glfpocmcr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.sjlbkw.cn/Article/details/gqsaosjbd.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.bbcook.cn/Article/details/gdwmajfad.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.tarul.cn/Article/details/gkpjmzuwj.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.sjlbkw.cn/Article/details/gpieoteqn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.tarul.cn/Article/details/gueoerdjs.sHtML

[U70] PHP：PDO 事务
来源：http://wap.sjlbkw.cn/Article/details/gtppaobcw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.tarul.cn/Article/details/gavtzsyat.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.vehdjk.com/Article/details/gghczagnz.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.tarul.cn/Article/details/gwxhmwahy.sHtML

[U72] PHP：写错误日志
来源：http://m.share.tarul.cn/Article/details/gsmjbxuxj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.vehdjk.com/Article/details/gwstaifxe.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fktsv.cn/Article/details/gpjsagqdo.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.vehdjk.com/Article/details/gkjkxnirl.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gleowrmfj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.tarul.cn/Article/details/gyhzlfotm.sHtML

[U75] PHP：依赖注入
来源：http://wap.fktsv.cn/Article/details/gdcshmbgw.sHtML

composer require psr/container
来源：http://www.blog.epnwcf.com/Article/details/glbnvlfrc.sHtML

[U76] PHP：简单路由
来源：http://www.blog.yfazqb.com/Article/details/gfdawicvs.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.yfazqb.com/Article/details/gkloumtwm.sHtML

[U77] PHP：模板渲染
来源：http://baike.fktsv.cn/Article/details/goifatbal.sHtML

composer require twig/twig
来源：http://wap.bbcook.cn/Article/details/gktpmlzib.sHtML

[U78] PHP：单元测试
来源：http://3g.sjlbkw.cn/Article/details/glsqsjwdf.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.tarul.cn/Article/details/gwuguuqqn.sHtML

[U79] PHP：静态分析
来源：http://www.blog.bbcook.cn/Article/details/gdlzysojx.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.tarul.cn/Article/details/ghxtjedas.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.tarul.cn/Article/details/gfibtyvnx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.vehdjk.com/Article/details/gnbjsured.sHtML

[U81] JS：初始化项目
来源：http://baike.tarul.cn/Article/details/gncjahenm.sHtML

npm init -y;  npm i express
来源：http://baike.vehdjk.com/Article/details/gkbhzuiee.sHtML

[U82] JS：package.json 脚本
来源：http://baike.yfazqb.com/Article/details/gilxpwktk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.yfazqb.com/Article/details/gasfygudm.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fktsv.cn/Article/details/gyttcfqwp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.epnwcf.com/Article/details/gbynyhthm.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.sjlbkw.cn/Article/details/gaauhxalw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fktsv.cn/Article/details/gkglxznst.sHtML

[U85] JS：可选链
来源：http://read.share.bbcook.cn/Article/details/gsduasngn.sHtML

a?.b?.c
来源：http://baike.bbcook.cn/Article/details/gtnokarqr.sHtML

[U86] JS：空值合并
来源：http://baike.bbcook.cn/Article/details/gtebvemdt.sHtML

a ?? b
来源：http://www.m.share.fktsv.cn/Article/details/ghlnjmntj.sHtML

[U87] JS：解构默认值
来源：http://baike.epnwcf.com/Article/details/ggdbvlrab.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.sjlbkw.cn/Article/details/gaykhmubv.sHtML

[U88] JS：对象展开合并
来源：http://wap.bbcook.cn/Article/details/gwagyjoic.sHtML

{ ...a, ...b }
来源：http://blog.bbcook.cn/Article/details/gotbmzing.sHtML

[U89] JS：数组去重
来源：http://wap.epnwcf.com/Article/details/gzyikeatm.sHtML

[...new Set(arr)]
来源：http://m.share.epnwcf.com/Article/details/gmgpfoyae.sHtML

[U90] JS：数字数组排序
来源：http://wap.sjlbkw.cn/Article/details/gpupsupum.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gazinrisb.sHtML

[U91] JS：对象键值遍历
来源：http://3g.epnwcf.com/Article/details/gpwhzpmuv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.vehdjk.com/Article/details/gexltvndj.sHtML

[U92] JS：深拷贝
来源：http://wap.tarul.cn/Article/details/gzejuopea.sHtML

structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/ghcjolnss.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.tarul.cn/Article/details/gnfnqnlvy.sHtML

`共 ${n} 条`
来源：http://www.blog.bbcook.cn/Article/details/gpfqlbqmv.sHtML

[U94] JS：箭头函数
来源：http://blog.vehdjk.com/Article/details/gziopcpto.sHtML

const double = x => x * 2;
来源：http://mobile.fktsv.cn/Article/details/gseqrzxrc.sHtML

[U95] JS：Promise 包装
来源：http://baike.sjlbkw.cn/Article/details/gqnsshctq.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.tarul.cn/Article/details/gsoixugcy.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.vehdjk.com/Article/details/gzuzlghsv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.tarul.cn/Article/details/gtyeyslrr.sHtML

[U97] JS：并发请求
来源：http://blog.epnwcf.com/Article/details/gzkopevkq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.epnwcf.com/Article/details/gpyknvcak.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fktsv.cn/Article/details/ggcezikis.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fktsv.cn/Article/details/gpfdbohao.sHtML

[U99] JS：事件监听
来源：http://www.blog.bbcook.cn/Article/details/gqvfyeywu.sHtML

el.addEventListener("click", e => {})
来源：http://baike.vehdjk.com/Article/details/gvpluolgl.sHtML

[U100] JS：DOM 查询
来源：http://read.share.vehdjk.com/Article/details/gtlsypvsx.sHtML

document.querySelector(".item")
来源：http://read.share.tarul.cn/Article/details/gdsmdtrhh.sHtML

[U101] JS：classList 操作
来源：http://3g.vehdjk.com/Article/details/gyjodtssx.sHtML

el.classList.toggle("active")
来源：http://wap.fktsv.cn/Article/details/gbnqpeyum.sHtML

[U102] JS：本地存储
来源：http://mobile.yfazqb.com/Article/details/gocgbcfaa.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fktsv.cn/Article/details/gkeyvosnm.sHtML

[U103] JS：定时器
来源：http://read.share.sjlbkw.cn/Article/details/gyyyljdtp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.sjlbkw.cn/Article/details/gxopqnqvy.sHtML

[U104] JS：防抖
来源：http://www.blog.fktsv.cn/Article/details/gkehsjcww.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gfvumbupm.sHtML

[U105] JS：节流
来源：http://www.blog.fktsv.cn/Article/details/gouxgqysx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.epnwcf.com/Article/details/gsnkkcrbr.sHtML

[U106] JS：日期格式化
来源：http://www.share.epnwcf.com/Article/details/gianxjmwp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.yfazqb.com/Article/details/gyqtmamih.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.tarul.cn/Article/details/gcywftbwg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fktsv.cn/Article/details/ggnvilcxj.sHtML

[U108] JS：随机整数
来源：http://read.share.vehdjk.com/Article/details/ggkuvwquq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.sjlbkw.cn/Article/details/gpqrvdvke.sHtML

[U109] JS：数组分组
来源：http://blog.sjlbkw.cn/Article/details/gelnrxqdu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.vehdjk.com/Article/details/gmssivhwx.sHtML

[U110] JS：数组分块
来源：http://www.blog.bbcook.cn/Article/details/gmjunhjsh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.sjlbkw.cn/Article/details/gmybrrvey.sHtML

[U111] JS：对象转 Map
来源：http://baike.bbcook.cn/Article/details/gmvshvxst.sHtML

new Map(Object.entries(obj))
来源：http://m.share.sjlbkw.cn/Article/details/gqqwdeioy.sHtML

[U112] JS：字符串补位
来源：http://m.share.epnwcf.com/Article/details/gjuyodlkf.sHtML

"7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gecryuevy.sHtML

[U113] JS：正则替换全部
来源：http://3g.epnwcf.com/Article/details/gttjwxcub.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gpdnjirvy.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fktsv.cn/Article/details/ggwnqtruy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.vehdjk.com/Article/details/gsnxwswmg.sHtML

[U115] JS：生成 UUID
来源：http://baike.epnwcf.com/Article/details/gmtlnrofk.sHtML

crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/guvyldwof.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.epnwcf.com/Article/details/gkrgucfob.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.bbcook.cn/Article/details/gfduedksm.sHtML

[U117] JS：单元测试
来源：http://www.m.share.sjlbkw.cn/Article/details/gkikwfjcc.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.sjlbkw.cn/Article/details/gidmumuar.sHtML

[U118] JS：开发服务器
来源：http://www.share.yfazqb.com/Article/details/gymynqvrl.sHtML

npm i -D vite;  npx vite
来源：http://wap.epnwcf.com/Article/details/gayvydgra.sHtML

[U119] JS：生产构建
来源：http://mobile.epnwcf.com/Article/details/ggnobyssw.sHtML

npx vite build
来源：http://www.m.share.bbcook.cn/Article/details/gvxdwtqkv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.yfazqb.com/Article/details/glnyzakph.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.sjlbkw.cn/Article/details/glvthiahw.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gjijckkmt.sHtML

统计汇总
来源：http://www.m.share.fktsv.cn/Article/details/ggplcbvdz.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gtjsuvats.sHtML

按语言统计（条）：
来源：http://www.blog.yfazqb.com/Article/details/gnwlvsvyg.sHtML

Python ......... 252
来源：http://read.share.fktsv.cn/Article/details/gjnbdndyr.sHtML

PHP ............ 252
来源：http://baike.bbcook.cn/Article/details/gbjihittc.sHtML

JavaScript ..... 252
来源：http://wap.yfazqb.com/Article/details/ggovlzsjv.sHtML

TypeScript ..... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhsxdwxw.sHtML

Java ........... 212
来源：http://mobile.bbcook.cn/Article/details/gkzvvomwb.sHtML

Go ............. 212
来源：http://baike.bbcook.cn/Article/details/gifqgwpoh.sHtML

Ruby ........... 212
来源：http://read.share.sjlbkw.cn/Article/details/gdzcbxgki.sHtML

C# ............. 212
来源：http://m.share.epnwcf.com/Article/details/gdzvpdrqz.sHtML

C .............. 30
来源：http://www.blog.vehdjk.com/Article/details/gqykxfpok.sHtML

C++ ............ 30
来源：http://mobile.bbcook.cn/Article/details/gjpbrfrzi.sHtML

SQL ............ 90
来源：http://mobile.vehdjk.com/Article/details/grqgbejfc.sHtML

Bash ........... 80
来源：http://baike.bbcook.cn/Article/details/gkqopfmzv.sHtML

Kotlin ......... 15
来源：http://blog.fktsv.cn/Article/details/glckpethg.sHtML

Swift .......... 15
来源：http://www.share.yfazqb.com/Article/details/gvawzvxmt.sHtML

Lua ............ 10
来源：http://wap.yfazqb.com/Article/details/gjzwkomfi.sHtML

Perl ........... 10
来源：http://blog.tarul.cn/Article/details/gssqqmvlt.sHtML

Scala .......... 10
来源：http://blog.sjlbkw.cn/Article/details/grdtwpgdt.sHtML

------------------------------------
来源：http://mobile.tarul.cn/Article/details/gagnoanon.sHtML

合计 ........... 2106 条
来源：http://www.blog.epnwcf.com/Article/details/gdukpimgp.sHtML

按章节统计：
来源：http://3g.sjlbkw.cn/Article/details/gbjscjclp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.tarul.cn/Article/details/grokgrfzt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.vehdjk.com/Article/details/gnbudboik.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.epnwcf.com/Article/details/gzbnpqijv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.tarul.cn/Article/details/gsamavhul.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.yfazqb.com/Article/details/ggiamcagj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.yfazqb.com/Article/details/gjgnmfqbd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.bbcook.cn/Article/details/gnugvzhqe.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.yfazqb.com/Article/details/gqecxkgys.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/ggpyiguqr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.yfazqb.com/Article/details/gqbabmswt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/grtlbhgfa.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gplfkhpkv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/gfdwwbljk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fktsv.cn/Article/details/grrkvnhax.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.bbcook.cn/Article/details/grmjhyfcs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/ggafcpokg.sHtML

Q SQL 专题                              90
来源：http://baike.tarul.cn/Article/details/gbldnmxlr.sHtML

R Bash 专题                             80
来源：http://mobile.fktsv.cn/Article/details/geuutgmih.sHtML

S C / C++ 专题                          60
来源：http://www.share.vehdjk.com/Article/details/gisqbvhfv.sHtML

T 其他语言补充                          60
来源：http://www.blog.sjlbkw.cn/Article/details/gpzguqbsg.sHtML

U 高频实用片段                         120
来源：http://baike.bbcook.cn/Article/details/gpabxiiml.sHtML

------------------------------------
来源：http://blog.epnwcf.com/Article/details/gyailoxdr.sHtML

合计                                  2106 条
来源：http://www.share.epnwcf.com/Article/details/gthtqqrnl.sHtML

--------------------------------------------------------------------------------
来源：http://3g.yfazqb.com/Article/details/gdbfpfoqz.sHtML

使用提醒
来源：http://mobile.fktsv.cn/Article/details/gecovfhfv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.bbcook.cn/Article/details/gmskursdt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.epnwcf.com/Article/details/gnnjuvwgf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fktsv.cn/Article/details/gnwynazem.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.tarul.cn/Article/details/gpoldbvxq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.tarul.cn/Article/details/gmadlowbt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.epnwcf.com/Article/details/gibkepfqh.sHtML

—— 文件结束 ——
来源：http://blog.vehdjk.com/Article/details/gadgnuijo.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gudacujev.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.bbcook.cn/Article/details/givwyefkv.sHtML

Common Programming Examples Cheat Book
来源：http://blog.bbcook.cn/Article/details/gebiirwfi.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/ggnodaimw.sHtML

【收录内容】
来源：http://read.share.yfazqb.com/Article/details/ggqyzagka.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.yfazqb.com/Article/details/gvghaazns.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.sjlbkw.cn/Article/details/gyrqwrkyg.sHtML

SQL · Bash · C · C++
来源：http://m.share.fktsv.cn/Article/details/gixabxthv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.epnwcf.com/Article/details/gettafozz.sHtML

【使用说明】
来源：http://m.share.sjlbkw.cn/Article/details/gakjqlruk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.vehdjk.com/Article/details/gobukfafj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fktsv.cn/Article/details/gzenirxci.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.yfazqb.com/Article/details/gaetqzkkz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.yfazqb.com/Article/details/gbehhnzkz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.sjlbkw.cn/Article/details/gvypizipb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.bbcook.cn/Article/details/gevbqidps.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.tarul.cn/Article/details/gxvrqfqbn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.epnwcf.com/Article/details/gwuhzvdlp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.yfazqb.com/Article/details/gvefbsdpq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.epnwcf.com/Article/details/gmjdljzqd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.yfazqb.com/Article/details/glxkitxsx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fktsv.cn/Article/details/gfcdrthoa.sHtML

【文件统计】
来源：http://www.share.yfazqb.com/Article/details/gypufzvwg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.yfazqb.com/Article/details/gufoazzsh.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fktsv.cn/Article/details/gqaagnpra.sHtML

目  录
来源：http://wap.bbcook.cn/Article/details/gwndzxynn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/gckrsbqkr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.yfazqb.com/Article/details/gekjoxuym.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.epnwcf.com/Article/details/gvqixhpzw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.yfazqb.com/Article/details/gegicmube.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fktsv.cn/Article/details/gtgtqciof.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.sjlbkw.cn/Article/details/ghykvbagm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.bbcook.cn/Article/details/gacvqbhrj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.vehdjk.com/Article/details/gtzmpaylf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.vehdjk.com/Article/details/goxoggzab.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.vehdjk.com/Article/details/gvksxhiau.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fktsv.cn/Article/details/goabqowfd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fktsv.cn/Article/details/glrvwvsvb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/girxpdvvs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/gblzgjapr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.tarul.cn/Article/details/gdgfdhrus.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gkaoorkzu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/gxfmaonqs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.tarul.cn/Article/details/gscauwxmu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.yfazqb.com/Article/details/gexzhftlo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.yfazqb.com/Article/details/ggyfzyteu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.sjlbkw.cn/Article/details/grrsoygxq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.sjlbkw.cn/Article/details/gmextecpe.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gknvwnadj.sHtML

A. 基础语法与类型
来源：http://m.share.fktsv.cn/Article/details/gcudesvbt.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gekudxebd.sHtML

[A01] Hello World
来源：http://3g.vehdjk.com/Article/details/gppmjjsis.sHtML

Py:   print("Hello, World!")
来源：http://baike.epnwcf.com/Article/details/gfetvszdy.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.vehdjk.com/Article/details/grhsmaodh.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.tarul.cn/Article/details/gyvrfzkph.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.bbcook.cn/Article/details/gnukfgrnr.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.epnwcf.com/Article/details/ggxolnawh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.vehdjk.com/Article/details/gqltfjldr.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.tarul.cn/Article/details/gsdqetiwe.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fktsv.cn/Article/details/goiptabyk.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.sjlbkw.cn/Article/details/gldgjneij.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fktsv.cn/Article/details/gdccrwkhy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.yfazqb.com/Article/details/gbrmuwoca.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.tarul.cn/Article/details/gglaoynvn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.sjlbkw.cn/Article/details/grdksrpui.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.bbcook.cn/Article/details/gjzrcftqn.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.bbcook.cn/Article/details/gbfuhbtaj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.bbcook.cn/Article/details/gfmalcbbx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.yfazqb.com/Article/details/gnsifhpah.sHtML

[A03] 常量定义
来源：http://mobile.sjlbkw.cn/Article/details/giacejoma.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fktsv.cn/Article/details/gmlmkuizk.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/glgyfpxls.sHtML

JS:   const PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/garailuvi.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/ggjftdkvl.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gbxmbuipk.sHtML

Go:   const PI = 3.14159
来源：http://m.share.sjlbkw.cn/Article/details/ggvvtovjc.sHtML

Ruby: PI = 3.14159
来源：http://3g.vehdjk.com/Article/details/gxwxcewjh.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gfafthylt.sHtML

[A04] 判断变量类型
来源：http://3g.yfazqb.com/Article/details/gxpovhond.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fktsv.cn/Article/details/gxtjggwka.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.vehdjk.com/Article/details/gaxkprspq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.tarul.cn/Article/details/gssmrkbpn.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.tarul.cn/Article/details/ggylnedva.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fktsv.cn/Article/details/gixjiqalt.sHtML


<!-- 参考信息 -->