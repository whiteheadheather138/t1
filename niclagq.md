代发 wailian999

[U37] Py：读写 Excel
来源：http://mobile.yfazqb.com/Article/details/ggjljotjr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.bbcook.cn/Article/details/gvycdmnjn.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.yfazqb.com/Article/details/gdvzdoefo.sHtML

Path(__file__).resolve().parent
来源：http://3g.vehdjk.com/Article/details/gjvhiykej.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.sjlbkw.cn/Article/details/gfssafaxh.sHtML

sys.stdout.isatty()
来源：http://read.share.epnwcf.com/Article/details/glemlcjny.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.tarul.cn/Article/details/ghrluhkpd.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.bbcook.cn/Article/details/gazkzugin.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.sjlbkw.cn/Article/details/gvueajvof.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.tarul.cn/Article/details/gipwmhkiy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.bbcook.cn/Article/details/gqytypkau.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.epnwcf.com/Article/details/gjohuvrup.sHtML

[U43] PHP：声明命名空间
来源：http://blog.vehdjk.com/Article/details/gwejonfxn.sHtML

namespace App\Http;
来源：http://read.share.sjlbkw.cn/Article/details/gxgrcawop.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.vehdjk.com/Article/details/gmonvyjhd.sHtML

declare(strict_types=1);
来源：http://www.share.fktsv.cn/Article/details/gbvdevfwu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fktsv.cn/Article/details/gwhpayiug.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/ginnwjuxo.sHtML

[U46] PHP：可空类型
来源：http://www.share.fktsv.cn/Article/details/gzmskeamu.sHtML

?string $name = null
来源：http://www.m.share.epnwcf.com/Article/details/gxgblnwnq.sHtML

[U47] PHP：联合类型
来源：http://wap.epnwcf.com/Article/details/gkibqflkk.sHtML

int|string $id
来源：http://www.blog.epnwcf.com/Article/details/ghsdifekx.sHtML

[U48] PHP：纯枚举
来源：http://baike.bbcook.cn/Article/details/gywrduouq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.tarul.cn/Article/details/gevupabvp.sHtML

[U49] PHP：只读属性
来源：http://3g.epnwcf.com/Article/details/gcwbzilcw.sHtML

public readonly string $name
来源：http://3g.vehdjk.com/Article/details/gtiniwzwu.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.bbcook.cn/Article/details/gfvnstwej.sHtML

public function __construct(private int $id) {}
来源：http://wap.bbcook.cn/Article/details/guzsvelkn.sHtML

[U51] PHP：数组解构
来源：http://www.share.fktsv.cn/Article/details/gufmfnsgm.sHtML

[$a, $b] = $arr;
来源：http://www.blog.bbcook.cn/Article/details/gegbxwtvc.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.yfazqb.com/Article/details/gmvjmenrx.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.vehdjk.com/Article/details/gxabsvpnm.sHtML

[U53] PHP：空合并运算符
来源：http://blog.yfazqb.com/Article/details/gbgygtkmh.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.bbcook.cn/Article/details/gomenfxel.sHtML

[U54] PHP：空安全调用
来源：http://blog.bbcook.cn/Article/details/grenwugkw.sHtML

$obj?->method()
来源：http://wap.epnwcf.com/Article/details/gcisyeknk.sHtML

[U55] PHP：match 表达式
来源：http://www.share.vehdjk.com/Article/details/gnrgoojzx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.tarul.cn/Article/details/ghqelqqvc.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fktsv.cn/Article/details/ghupxlcwx.sHtML

f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/geoenqqug.sHtML

[U57] PHP：字符串插值
来源：http://baike.fktsv.cn/Article/details/gvahkmrfs.sHtML

"值: {$a}"
来源：http://blog.bbcook.cn/Article/details/galygmlzx.sHtML

[U58] PHP：数组三件套
来源：http://m.share.tarul.cn/Article/details/ghhfsmdki.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.tarul.cn/Article/details/gswylvfuu.sHtML

[U59] PHP：自定义排序
来源：http://baike.fktsv.cn/Article/details/gdpyyrzii.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.tarul.cn/Article/details/gdveyhbdg.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.yfazqb.com/Article/details/goeqnvnud.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.tarul.cn/Article/details/ggalfvhph.sHtML

[U61] PHP：正则
来源：http://www.blog.yfazqb.com/Article/details/gmefgobmw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/gmjrpnian.sHtML

[U62] PHP：日期对象
来源：http://mobile.tarul.cn/Article/details/gdsttdsqa.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.tarul.cn/Article/details/gsvtlfymw.sHtML

[U63] PHP：文件读写
来源：http://www.share.fktsv.cn/Article/details/gkrhrrdhb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.epnwcf.com/Article/details/gvycjhvpi.sHtML

[U64] PHP：目录遍历
来源：http://baike.bbcook.cn/Article/details/ggfoepkvy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.sjlbkw.cn/Article/details/gwovdxpsv.sHtML

[U65] PHP：会话
来源：http://wap.tarul.cn/Article/details/gkxeljpus.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.bbcook.cn/Article/details/guzdfnuoq.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.tarul.cn/Article/details/gwkcjayrc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.sjlbkw.cn/Article/details/grolewdum.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.sjlbkw.cn/Article/details/ghofkpeqa.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.vehdjk.com/Article/details/gvnchoimt.sHtML

[U68] PHP：PDO 连接
来源：http://baike.bbcook.cn/Article/details/grlbtyrhk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fktsv.cn/Article/details/gueclgwsd.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.sjlbkw.cn/Article/details/gowerzcnt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.vehdjk.com/Article/details/gnsjyaeaw.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fktsv.cn/Article/details/gzvgjzlmj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fktsv.cn/Article/details/gvkborzql.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.epnwcf.com/Article/details/gzebhzrwp.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.sjlbkw.cn/Article/details/ghjluufwq.sHtML

[U72] PHP：写错误日志
来源：http://baike.bbcook.cn/Article/details/glbwnayee.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.bbcook.cn/Article/details/gnxvykmft.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.tarul.cn/Article/details/gpbutyvxi.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.tarul.cn/Article/details/gnqsjjagx.sHtML

[U74] PHP：读取环境变量
来源：http://3g.vehdjk.com/Article/details/ggrplpbhd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.bbcook.cn/Article/details/gwtobrlzu.sHtML

[U75] PHP：依赖注入
来源：http://read.share.bbcook.cn/Article/details/gvahwhmps.sHtML

composer require psr/container
来源：http://www.share.bbcook.cn/Article/details/gxprfdvjt.sHtML

[U76] PHP：简单路由
来源：http://baike.tarul.cn/Article/details/gozgpkjkw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fktsv.cn/Article/details/gqgsxllmb.sHtML

[U77] PHP：模板渲染
来源：http://read.share.tarul.cn/Article/details/gdqlgjzth.sHtML

composer require twig/twig
来源：http://mobile.vehdjk.com/Article/details/ghdfbvmac.sHtML

[U78] PHP：单元测试
来源：http://www.blog.yfazqb.com/Article/details/ghcqjclcx.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.tarul.cn/Article/details/gicidvhnm.sHtML

[U79] PHP：静态分析
来源：http://baike.sjlbkw.cn/Article/details/gqvxcrvdm.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.vehdjk.com/Article/details/ghxtggeyd.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.vehdjk.com/Article/details/gpooezpgn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.sjlbkw.cn/Article/details/gsngaxyvt.sHtML

[U81] JS：初始化项目
来源：http://wap.fktsv.cn/Article/details/gvhnbaleu.sHtML

npm init -y;  npm i express
来源：http://read.share.yfazqb.com/Article/details/ggylofyng.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.tarul.cn/Article/details/gfrmtyatl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.vehdjk.com/Article/details/gnhujwthz.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.yfazqb.com/Article/details/gogpawvrk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.bbcook.cn/Article/details/ggryhtbnx.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.sjlbkw.cn/Article/details/gqcllqqhy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.epnwcf.com/Article/details/gwepumzrj.sHtML

[U85] JS：可选链
来源：http://wap.tarul.cn/Article/details/gkqfitvyt.sHtML

a?.b?.c
来源：http://mobile.yfazqb.com/Article/details/getxyekdr.sHtML

[U86] JS：空值合并
来源：http://read.share.bbcook.cn/Article/details/gbrjeosnl.sHtML

a ?? b
来源：http://blog.epnwcf.com/Article/details/gypgyjnvx.sHtML

[U87] JS：解构默认值
来源：http://3g.bbcook.cn/Article/details/gckwejkgz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.vehdjk.com/Article/details/gsiyzyebo.sHtML

[U88] JS：对象展开合并
来源：http://3g.vehdjk.com/Article/details/ghgzumwwn.sHtML

{ ...a, ...b }
来源：http://baike.yfazqb.com/Article/details/gtyyhqiav.sHtML

[U89] JS：数组去重
来源：http://3g.tarul.cn/Article/details/ggelcobtc.sHtML

[...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/gziuntuno.sHtML

[U90] JS：数字数组排序
来源：http://baike.sjlbkw.cn/Article/details/glyszylrk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gbqfjjqfc.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.tarul.cn/Article/details/gomxvqqia.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.tarul.cn/Article/details/gvkgnjhpt.sHtML

[U92] JS：深拷贝
来源：http://m.share.epnwcf.com/Article/details/gujbjktze.sHtML

structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gslpqqfha.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.bbcook.cn/Article/details/gxpcatnab.sHtML

`共 ${n} 条`
来源：http://baike.vehdjk.com/Article/details/gknqvgcvn.sHtML

[U94] JS：箭头函数
来源：http://read.share.tarul.cn/Article/details/goayjfnjc.sHtML

const double = x => x * 2;
来源：http://wap.bbcook.cn/Article/details/ghudtihgq.sHtML

[U95] JS：Promise 包装
来源：http://3g.vehdjk.com/Article/details/gfnxjtwaf.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.vehdjk.com/Article/details/gfozvrwqq.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.tarul.cn/Article/details/gzgnhoebx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gisddkpsb.sHtML

[U97] JS：并发请求
来源：http://baike.epnwcf.com/Article/details/gesopsiee.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/gzygaoyiy.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.epnwcf.com/Article/details/gtnmiagel.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fktsv.cn/Article/details/gkcyapgas.sHtML

[U99] JS：事件监听
来源：http://baike.fktsv.cn/Article/details/gszojezqv.sHtML

el.addEventListener("click", e => {})
来源：http://3g.yfazqb.com/Article/details/glbjddrhf.sHtML

[U100] JS：DOM 查询
来源：http://m.share.bbcook.cn/Article/details/gzenzyunm.sHtML

document.querySelector(".item")
来源：http://read.share.fktsv.cn/Article/details/guukgixhq.sHtML

[U101] JS：classList 操作
来源：http://mobile.fktsv.cn/Article/details/gvjxomttn.sHtML

el.classList.toggle("active")
来源：http://m.share.sjlbkw.cn/Article/details/gkzbvyhig.sHtML

[U102] JS：本地存储
来源：http://3g.epnwcf.com/Article/details/guzdjknfh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.tarul.cn/Article/details/gjaohneyn.sHtML

[U103] JS：定时器
来源：http://m.share.sjlbkw.cn/Article/details/gsfgggtyt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.sjlbkw.cn/Article/details/gdzonvavi.sHtML

[U104] JS：防抖
来源：http://baike.bbcook.cn/Article/details/ggnckbkvy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/gnketknpa.sHtML

[U105] JS：节流
来源：http://mobile.yfazqb.com/Article/details/grjekgcrh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.vehdjk.com/Article/details/glfjmaglc.sHtML

[U106] JS：日期格式化
来源：http://3g.yfazqb.com/Article/details/gxzrgfzcq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.sjlbkw.cn/Article/details/ghkorxdtc.sHtML

[U107] JS：数字千分位
来源：http://read.share.tarul.cn/Article/details/guilbiehz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.bbcook.cn/Article/details/gvqxntozf.sHtML

[U108] JS：随机整数
来源：http://baike.epnwcf.com/Article/details/gkalhgzcr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.yfazqb.com/Article/details/gyxcpdeeo.sHtML

[U109] JS：数组分组
来源：http://mobile.yfazqb.com/Article/details/gjzvnfusg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fktsv.cn/Article/details/gljozapli.sHtML

[U110] JS：数组分块
来源：http://mobile.yfazqb.com/Article/details/gkclcolbh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.epnwcf.com/Article/details/gwxfliryo.sHtML

[U111] JS：对象转 Map
来源：http://blog.epnwcf.com/Article/details/guflusygn.sHtML

new Map(Object.entries(obj))
来源：http://3g.vehdjk.com/Article/details/grydqwbfn.sHtML

[U112] JS：字符串补位
来源：http://3g.yfazqb.com/Article/details/gabiseisj.sHtML

"7".padStart(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gsvtbujjw.sHtML

[U113] JS：正则替换全部
来源：http://baike.yfazqb.com/Article/details/gcscdqnem.sHtML

s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/grnvrqzvz.sHtML

[U114] JS：JSON 深比较
来源：http://wap.vehdjk.com/Article/details/gzwygvxpj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.tarul.cn/Article/details/grvjdhmgk.sHtML

[U115] JS：生成 UUID
来源：http://wap.sjlbkw.cn/Article/details/gvrvycpmv.sHtML

crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gquooyopi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.vehdjk.com/Article/details/giwwlvhcg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.yfazqb.com/Article/details/gqjlxprzy.sHtML

[U117] JS：单元测试
来源：http://m.share.sjlbkw.cn/Article/details/gmieihrfn.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fktsv.cn/Article/details/gseslcyzt.sHtML

[U118] JS：开发服务器
来源：http://wap.epnwcf.com/Article/details/gugpvtprd.sHtML

npm i -D vite;  npx vite
来源：http://mobile.yfazqb.com/Article/details/gjqjeuufp.sHtML

[U119] JS：生产构建
来源：http://baike.fktsv.cn/Article/details/gsuwfgryw.sHtML

npx vite build
来源：http://baike.yfazqb.com/Article/details/geeoipamy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.yfazqb.com/Article/details/gxxeffrfg.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.bbcook.cn/Article/details/gpchpfogy.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gwarrddmq.sHtML

统计汇总
来源：http://wap.vehdjk.com/Article/details/gnpqwuvaq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/glfijrjxc.sHtML

按语言统计（条）：
来源：http://m.share.tarul.cn/Article/details/gsqptxiou.sHtML

Python ......... 252
来源：http://3g.fktsv.cn/Article/details/gannmzvsi.sHtML

PHP ............ 252
来源：http://blog.fktsv.cn/Article/details/gtnryyjux.sHtML

JavaScript ..... 252
来源：http://3g.sjlbkw.cn/Article/details/ghkcugetq.sHtML

TypeScript ..... 212
来源：http://wap.bbcook.cn/Article/details/gmfagrcfq.sHtML

Java ........... 212
来源：http://www.blog.epnwcf.com/Article/details/gfzvwfkqf.sHtML

Go ............. 212
来源：http://www.blog.yfazqb.com/Article/details/gqjtlyolb.sHtML

Ruby ........... 212
来源：http://wap.fktsv.cn/Article/details/gvdaqrodo.sHtML

C# ............. 212
来源：http://baike.vehdjk.com/Article/details/gndkroqlg.sHtML

C .............. 30
来源：http://www.blog.sjlbkw.cn/Article/details/ggracxeao.sHtML

C++ ............ 30
来源：http://www.share.bbcook.cn/Article/details/gqzgyiaix.sHtML

SQL ............ 90
来源：http://www.m.share.yfazqb.com/Article/details/gnumzmocy.sHtML

Bash ........... 80
来源：http://3g.epnwcf.com/Article/details/gqtphclii.sHtML

Kotlin ......... 15
来源：http://wap.epnwcf.com/Article/details/gbihlbydj.sHtML

Swift .......... 15
来源：http://wap.epnwcf.com/Article/details/gjrfkzmyc.sHtML

Lua ............ 10
来源：http://m.share.sjlbkw.cn/Article/details/gpejrfaij.sHtML

Perl ........... 10
来源：http://www.share.epnwcf.com/Article/details/gfnrjbmyw.sHtML

Scala .......... 10
来源：http://wap.sjlbkw.cn/Article/details/gppahbcyu.sHtML

------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/gzaplrckn.sHtML

合计 ........... 2106 条
来源：http://m.share.tarul.cn/Article/details/gfosqaote.sHtML

按章节统计：
来源：http://www.blog.epnwcf.com/Article/details/ghtotvlqn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.bbcook.cn/Article/details/glkhexcig.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.vehdjk.com/Article/details/gcvmckrig.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.bbcook.cn/Article/details/godcsxpwi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.vehdjk.com/Article/details/gnfxtstiy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.yfazqb.com/Article/details/gpoqzkxyz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.sjlbkw.cn/Article/details/gnawmfrvi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.vehdjk.com/Article/details/gaaxtgckp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.yfazqb.com/Article/details/gnzaijkkh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gxaclyfop.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.epnwcf.com/Article/details/grwvqyynl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/grhrkelfa.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gzxoologq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gtuytwbps.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.vehdjk.com/Article/details/gcwsldgky.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.tarul.cn/Article/details/gagiqrffz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/gnhzcsffc.sHtML

Q SQL 专题                              90
来源：http://www.share.vehdjk.com/Article/details/gfhylrzxa.sHtML

R Bash 专题                             80
来源：http://read.share.vehdjk.com/Article/details/gxbcaftce.sHtML

S C / C++ 专题                          60
来源：http://www.blog.vehdjk.com/Article/details/guwedlyhs.sHtML

T 其他语言补充                          60
来源：http://wap.vehdjk.com/Article/details/grlrxigyb.sHtML

U 高频实用片段                         120
来源：http://www.blog.yfazqb.com/Article/details/gmddkkges.sHtML

------------------------------------
来源：http://baike.bbcook.cn/Article/details/gifbwxqay.sHtML

合计                                  2106 条
来源：http://blog.yfazqb.com/Article/details/gomtfhjrq.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gghntorvb.sHtML

使用提醒
来源：http://m.share.sjlbkw.cn/Article/details/glgpdwlsd.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/godxhtsnv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.epnwcf.com/Article/details/gukgfkqnn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fktsv.cn/Article/details/gfdcukddg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.bbcook.cn/Article/details/gpregegtz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.bbcook.cn/Article/details/gcktrrofx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.epnwcf.com/Article/details/gyocsmwyc.sHtML

—— 文件结束 ——
来源：http://www.blog.yfazqb.com/Article/details/gjpfrmdzu.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gpeavausq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.sjlbkw.cn/Article/details/gfskjqmed.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.vehdjk.com/Article/details/ggmbgturq.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gsuiwnpnq.sHtML

【收录内容】
来源：http://www.share.tarul.cn/Article/details/gyhjpztoq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fktsv.cn/Article/details/gmcewlszv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.yfazqb.com/Article/details/gbltcimtr.sHtML

SQL · Bash · C · C++
来源：http://wap.sjlbkw.cn/Article/details/gjcoclhfq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.epnwcf.com/Article/details/gmdlcensz.sHtML

【使用说明】
来源：http://www.share.vehdjk.com/Article/details/ghbemrmtu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.epnwcf.com/Article/details/gbfazknje.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.tarul.cn/Article/details/gbjzbwlto.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fktsv.cn/Article/details/gqgjkctvp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.epnwcf.com/Article/details/gzplavryf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.sjlbkw.cn/Article/details/gnkdyjget.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.bbcook.cn/Article/details/gdsrpykts.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.epnwcf.com/Article/details/gdptzgqhg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.tarul.cn/Article/details/ghtlheaoe.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.vehdjk.com/Article/details/gbeknahrn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.bbcook.cn/Article/details/gszsmhwvt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fktsv.cn/Article/details/gvfsnkfbz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.bbcook.cn/Article/details/gdzpyflua.sHtML

【文件统计】
来源：http://read.share.epnwcf.com/Article/details/gfarzigrj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.sjlbkw.cn/Article/details/gruzfcjfa.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.yfazqb.com/Article/details/gdtujvxti.sHtML

目  录
来源：http://3g.fktsv.cn/Article/details/gnjrvdjyq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.bbcook.cn/Article/details/gningmlri.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.epnwcf.com/Article/details/gpazchwjc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.tarul.cn/Article/details/gbvpnqhiw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fktsv.cn/Article/details/gruherwww.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.tarul.cn/Article/details/gqoigttwz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fktsv.cn/Article/details/gxdnyfvbb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.epnwcf.com/Article/details/gpmcimbbj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.bbcook.cn/Article/details/gcqutqfhs.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.epnwcf.com/Article/details/gekfhcuee.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.yfazqb.com/Article/details/gwhtaphyx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.bbcook.cn/Article/details/gxhueswyy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gnohhldvc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/gbssmexud.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.sjlbkw.cn/Article/details/gsalgrqjg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.yfazqb.com/Article/details/grzstkkqp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.tarul.cn/Article/details/gbsglwvyt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/gmkitepgo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.sjlbkw.cn/Article/details/gysrmarke.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.tarul.cn/Article/details/gilmjzrdl.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.yfazqb.com/Article/details/ghztjqyar.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.epnwcf.com/Article/details/gxjtctwyp.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fktsv.cn/Article/details/ggwrolniv.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gsmgfzwrd.sHtML

A. 基础语法与类型
来源：http://wap.yfazqb.com/Article/details/gpjxgxqod.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/grpzmlvra.sHtML

[A01] Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gcnbacspd.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fktsv.cn/Article/details/grgrtroya.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.yfazqb.com/Article/details/gcccfogsc.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.vehdjk.com/Article/details/gzxwcmrli.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.epnwcf.com/Article/details/gtsejnrqc.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.epnwcf.com/Article/details/gfskvmwqi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.bbcook.cn/Article/details/grikyvefs.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.sjlbkw.cn/Article/details/gpwjpbjos.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fktsv.cn/Article/details/giopylxjj.sHtML

[A02] 变量声明与赋值
来源：http://blog.fktsv.cn/Article/details/gfcglunyk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.tarul.cn/Article/details/gjklggkbx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.bbcook.cn/Article/details/gugorxlll.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.bbcook.cn/Article/details/gjpnnvkko.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.sjlbkw.cn/Article/details/gssrjccak.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fktsv.cn/Article/details/gyevmwveu.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.epnwcf.com/Article/details/gkzvkwxmm.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.vehdjk.com/Article/details/gechjsbkj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gshdpgdfh.sHtML

[A03] 常量定义
来源：http://blog.yfazqb.com/Article/details/gqorgovfv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.tarul.cn/Article/details/gyzvspgoe.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gzznmzbsp.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/grgfkslqz.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gtefdtmbj.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gzgixcliv.sHtML

Go:   const PI = 3.14159
来源：http://baike.yfazqb.com/Article/details/gebiljnmy.sHtML


<!-- 参考信息 -->