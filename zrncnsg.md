代发 wailian999

[U43] PHP：声明命名空间
来源：http://mobile.vehdjk.com/Article/details/gnruboqix.sHtML

namespace App\Http;
来源：http://wap.sjlbkw.cn/Article/details/gqobqhupp.sHtML

[U44] PHP：开启严格类型
来源：http://baike.vehdjk.com/Article/details/gepacdxpa.sHtML

declare(strict_types=1);
来源：http://blog.fktsv.cn/Article/details/gbgditndi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.sjlbkw.cn/Article/details/grptsjcgl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gfhodovaf.sHtML

[U46] PHP：可空类型
来源：http://mobile.epnwcf.com/Article/details/gsnbxlwjr.sHtML

?string $name = null
来源：http://read.share.vehdjk.com/Article/details/gdscppyoh.sHtML

[U47] PHP：联合类型
来源：http://m.share.yfazqb.com/Article/details/giteufvub.sHtML

int|string $id
来源：http://baike.tarul.cn/Article/details/gnaudgewn.sHtML

[U48] PHP：纯枚举
来源：http://mobile.bbcook.cn/Article/details/gvvzwhxtq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.vehdjk.com/Article/details/gxmyzxwnw.sHtML

[U49] PHP：只读属性
来源：http://m.share.sjlbkw.cn/Article/details/gcclxxopv.sHtML

public readonly string $name
来源：http://m.share.tarul.cn/Article/details/gkrlwmrgi.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.epnwcf.com/Article/details/gpnnlfwjn.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fktsv.cn/Article/details/goveducco.sHtML

[U51] PHP：数组解构
来源：http://read.share.sjlbkw.cn/Article/details/gzfqlsjvf.sHtML

[$a, $b] = $arr;
来源：http://3g.bbcook.cn/Article/details/guukcqcri.sHtML

[U52] PHP：箭头函数
来源：http://baike.sjlbkw.cn/Article/details/gouhikoib.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.epnwcf.com/Article/details/gzseqaxse.sHtML

[U53] PHP：空合并运算符
来源：http://wap.vehdjk.com/Article/details/gpzhzbcum.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.yfazqb.com/Article/details/gqpggspee.sHtML

[U54] PHP：空安全调用
来源：http://mobile.bbcook.cn/Article/details/gxkchgzta.sHtML

$obj?->method()
来源：http://3g.sjlbkw.cn/Article/details/gattjazmn.sHtML

[U55] PHP：match 表达式
来源：http://m.share.tarul.cn/Article/details/gxorxhejt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.tarul.cn/Article/details/gsgrxamea.sHtML

[U56] PHP：命名参数
来源：http://www.share.epnwcf.com/Article/details/grdruslhh.sHtML

f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/glvrpujkj.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gvwwtczpo.sHtML

"值: {$a}"
来源：http://www.blog.fktsv.cn/Article/details/giwreinqg.sHtML

[U58] PHP：数组三件套
来源：http://read.share.sjlbkw.cn/Article/details/gjvcreqlx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gayrotfmz.sHtML

[U59] PHP：自定义排序
来源：http://www.share.tarul.cn/Article/details/glqpavewc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.yfazqb.com/Article/details/gaeloywex.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.sjlbkw.cn/Article/details/ggbclyypd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.tarul.cn/Article/details/gsmubzpha.sHtML

[U61] PHP：正则
来源：http://baike.yfazqb.com/Article/details/gqpaoolfz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.vehdjk.com/Article/details/ghmurxxbp.sHtML

[U62] PHP：日期对象
来源：http://3g.fktsv.cn/Article/details/gghbcslrr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.bbcook.cn/Article/details/gckxolkex.sHtML

[U63] PHP：文件读写
来源：http://blog.vehdjk.com/Article/details/giurxhnip.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.vehdjk.com/Article/details/gczltxjur.sHtML

[U64] PHP：目录遍历
来源：http://www.share.tarul.cn/Article/details/gtvzvqlci.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fktsv.cn/Article/details/gcydswrsq.sHtML

[U65] PHP：会话
来源：http://3g.vehdjk.com/Article/details/gisttspnt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.yfazqb.com/Article/details/glygckpaa.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.bbcook.cn/Article/details/grtwrayzm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.bbcook.cn/Article/details/gfjlnftfq.sHtML

[U67] PHP：处理文件上传
来源：http://wap.bbcook.cn/Article/details/gdryharbg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.bbcook.cn/Article/details/gzkoknncf.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.vehdjk.com/Article/details/ggjyivjuo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fktsv.cn/Article/details/gjufrflvk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.yfazqb.com/Article/details/gofofgcyc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.tarul.cn/Article/details/gqgeyojfo.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.vehdjk.com/Article/details/gflwjzqlf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.tarul.cn/Article/details/gucbirjte.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.epnwcf.com/Article/details/ggfltonbq.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fktsv.cn/Article/details/gnmigicvv.sHtML

[U72] PHP：写错误日志
来源：http://www.share.epnwcf.com/Article/details/gwxlrzquy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fktsv.cn/Article/details/guzschpzc.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.bbcook.cn/Article/details/gmgwwqcyw.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fktsv.cn/Article/details/gmezebtok.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.epnwcf.com/Article/details/gtvknszfi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.sjlbkw.cn/Article/details/gheklnugm.sHtML

[U75] PHP：依赖注入
来源：http://www.share.epnwcf.com/Article/details/gafzrrqnv.sHtML

composer require psr/container
来源：http://m.share.sjlbkw.cn/Article/details/gnjhsgvsz.sHtML

[U76] PHP：简单路由
来源：http://wap.yfazqb.com/Article/details/grmuqwgql.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.epnwcf.com/Article/details/gvskkxohu.sHtML

[U77] PHP：模板渲染
来源：http://baike.tarul.cn/Article/details/gsupkldxc.sHtML

composer require twig/twig
来源：http://mobile.vehdjk.com/Article/details/gopqofjlx.sHtML

[U78] PHP：单元测试
来源：http://m.share.tarul.cn/Article/details/genptlpaw.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fktsv.cn/Article/details/grydvykaq.sHtML

[U79] PHP：静态分析
来源：http://read.share.epnwcf.com/Article/details/gahjlnnhe.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.epnwcf.com/Article/details/gcpdecnoc.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.bbcook.cn/Article/details/ghnzphwuq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.epnwcf.com/Article/details/govjympfu.sHtML

[U81] JS：初始化项目
来源：http://mobile.tarul.cn/Article/details/gutgltaja.sHtML

npm init -y;  npm i express
来源：http://read.share.tarul.cn/Article/details/gpfnkmhtr.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.bbcook.cn/Article/details/gymwikgfu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.epnwcf.com/Article/details/glbppmqhh.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.bbcook.cn/Article/details/gipywrupn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fktsv.cn/Article/details/gjbhdkztg.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fktsv.cn/Article/details/gygbvhfex.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.epnwcf.com/Article/details/gqagjehun.sHtML

[U85] JS：可选链
来源：http://mobile.sjlbkw.cn/Article/details/gfmrkwzwr.sHtML

a?.b?.c
来源：http://www.share.yfazqb.com/Article/details/gallgxejn.sHtML

[U86] JS：空值合并
来源：http://read.share.tarul.cn/Article/details/gzjndnitq.sHtML

a ?? b
来源：http://www.blog.tarul.cn/Article/details/gwmknflzg.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gigvdiury.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.yfazqb.com/Article/details/ghjdrvrvz.sHtML

[U88] JS：对象展开合并
来源：http://wap.yfazqb.com/Article/details/gazmyxoge.sHtML

{ ...a, ...b }
来源：http://baike.epnwcf.com/Article/details/gboazbzfu.sHtML

[U89] JS：数组去重
来源：http://blog.sjlbkw.cn/Article/details/gwfffuuwo.sHtML

[...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/gppacusti.sHtML

[U90] JS：数字数组排序
来源：http://m.share.sjlbkw.cn/Article/details/gkyfqeeef.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.yfazqb.com/Article/details/gktuqfdhu.sHtML

[U91] JS：对象键值遍历
来源：http://blog.bbcook.cn/Article/details/govzmslml.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.yfazqb.com/Article/details/ggvgibjpv.sHtML

[U92] JS：深拷贝
来源：http://3g.bbcook.cn/Article/details/gnutxsmik.sHtML

structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/gxgbawxxt.sHtML

[U93] JS：模板字符串
来源：http://baike.sjlbkw.cn/Article/details/gxiamwzpc.sHtML

`共 ${n} 条`
来源：http://wap.epnwcf.com/Article/details/gxxnjvhpp.sHtML

[U94] JS：箭头函数
来源：http://m.share.vehdjk.com/Article/details/grwzexdyf.sHtML

const double = x => x * 2;
来源：http://mobile.sjlbkw.cn/Article/details/grbumpaxc.sHtML

[U95] JS：Promise 包装
来源：http://mobile.vehdjk.com/Article/details/goaadlgju.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.sjlbkw.cn/Article/details/gdmqpoumn.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.vehdjk.com/Article/details/guuabnres.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/gevjqlrdi.sHtML

[U97] JS：并发请求
来源：http://www.blog.bbcook.cn/Article/details/gxdgimnms.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/gjryepfqo.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.yfazqb.com/Article/details/glrypqhuo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fktsv.cn/Article/details/gsruxqoaq.sHtML

[U99] JS：事件监听
来源：http://3g.epnwcf.com/Article/details/gvxvvlumu.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.sjlbkw.cn/Article/details/gptelkwxe.sHtML

[U100] JS：DOM 查询
来源：http://www.share.vehdjk.com/Article/details/gdqkmpbol.sHtML

document.querySelector(".item")
来源：http://3g.tarul.cn/Article/details/gjsargqnb.sHtML

[U101] JS：classList 操作
来源：http://www.share.sjlbkw.cn/Article/details/grwmmidnp.sHtML

el.classList.toggle("active")
来源：http://www.blog.tarul.cn/Article/details/gwhjlptbf.sHtML

[U102] JS：本地存储
来源：http://www.blog.yfazqb.com/Article/details/gkoholotr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.bbcook.cn/Article/details/gkdytrclj.sHtML

[U103] JS：定时器
来源：http://3g.tarul.cn/Article/details/gchwmnxym.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.yfazqb.com/Article/details/gxhpicnmo.sHtML

[U104] JS：防抖
来源：http://mobile.epnwcf.com/Article/details/glpwyzqza.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gfwjpcvrp.sHtML

[U105] JS：节流
来源：http://www.m.share.epnwcf.com/Article/details/gnuzlmnhu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fktsv.cn/Article/details/gkwmuompz.sHtML

[U106] JS：日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gjhtnnxdi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.epnwcf.com/Article/details/gaekfflny.sHtML

[U107] JS：数字千分位
来源：http://blog.epnwcf.com/Article/details/gsxngyjtj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.vehdjk.com/Article/details/gilxtwsrm.sHtML

[U108] JS：随机整数
来源：http://wap.sjlbkw.cn/Article/details/gflehebhw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.vehdjk.com/Article/details/gvmwbgmyj.sHtML

[U109] JS：数组分组
来源：http://wap.sjlbkw.cn/Article/details/gopesfbuc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.vehdjk.com/Article/details/gkhzxfsao.sHtML

[U110] JS：数组分块
来源：http://www.blog.bbcook.cn/Article/details/ggllthjva.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.bbcook.cn/Article/details/gkqvlnbwo.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.bbcook.cn/Article/details/gafmeogue.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.vehdjk.com/Article/details/gshdfftof.sHtML

[U112] JS：字符串补位
来源：http://www.blog.sjlbkw.cn/Article/details/gztrokyrw.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gkjbgdurr.sHtML

[U113] JS：正则替换全部
来源：http://baike.epnwcf.com/Article/details/gponcbgwj.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/ggsjzesgj.sHtML

[U114] JS：JSON 深比较
来源：http://baike.bbcook.cn/Article/details/ghewkiwar.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.sjlbkw.cn/Article/details/geudyujmy.sHtML

[U115] JS：生成 UUID
来源：http://3g.fktsv.cn/Article/details/gspwnjftp.sHtML

crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/gdnywoqut.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.vehdjk.com/Article/details/gksedndwl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.epnwcf.com/Article/details/gokqulxuw.sHtML

[U117] JS：单元测试
来源：http://www.share.epnwcf.com/Article/details/gcjleprbm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.yfazqb.com/Article/details/gploxvguv.sHtML

[U118] JS：开发服务器
来源：http://www.blog.vehdjk.com/Article/details/gfguyhktn.sHtML

npm i -D vite;  npx vite
来源：http://m.share.vehdjk.com/Article/details/ggjisxlcg.sHtML

[U119] JS：生产构建
来源：http://www.blog.bbcook.cn/Article/details/grsunllho.sHtML

npx vite build
来源：http://m.share.epnwcf.com/Article/details/gwuelfuwu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fktsv.cn/Article/details/glnmnzsyf.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.epnwcf.com/Article/details/gccireout.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gtndfbmyi.sHtML

统计汇总
来源：http://3g.fktsv.cn/Article/details/gytfzhomv.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gtpiatcor.sHtML

按语言统计（条）：
来源：http://3g.tarul.cn/Article/details/gxmwjkfem.sHtML

Python ......... 252
来源：http://wap.fktsv.cn/Article/details/grlfspjtz.sHtML

PHP ............ 252
来源：http://www.share.tarul.cn/Article/details/gfxpzolud.sHtML

JavaScript ..... 252
来源：http://m.share.sjlbkw.cn/Article/details/ghpaaokqm.sHtML

TypeScript ..... 212
来源：http://wap.yfazqb.com/Article/details/glbntjnqn.sHtML

Java ........... 212
来源：http://www.blog.tarul.cn/Article/details/gmhxshtkq.sHtML

Go ............. 212
来源：http://www.blog.vehdjk.com/Article/details/gxdjjahii.sHtML

Ruby ........... 212
来源：http://read.share.epnwcf.com/Article/details/gtlobaghw.sHtML

C# ............. 212
来源：http://www.m.share.vehdjk.com/Article/details/gqbiutikh.sHtML

C .............. 30
来源：http://read.share.sjlbkw.cn/Article/details/ggowjpylk.sHtML

C++ ............ 30
来源：http://wap.yfazqb.com/Article/details/glapcoqdc.sHtML

SQL ............ 90
来源：http://baike.fktsv.cn/Article/details/gzmvlzjdl.sHtML

Bash ........... 80
来源：http://www.share.vehdjk.com/Article/details/gazmhcxnq.sHtML

Kotlin ......... 15
来源：http://read.share.sjlbkw.cn/Article/details/gtxucpkeq.sHtML

Swift .......... 15
来源：http://read.share.yfazqb.com/Article/details/gimquuyzy.sHtML

Lua ............ 10
来源：http://www.share.fktsv.cn/Article/details/gmipudaaj.sHtML

Perl ........... 10
来源：http://www.share.fktsv.cn/Article/details/gvnwfrqmj.sHtML

Scala .......... 10
来源：http://blog.tarul.cn/Article/details/gtgxxofuu.sHtML

------------------------------------
来源：http://3g.epnwcf.com/Article/details/geaprazga.sHtML

合计 ........... 2106 条
来源：http://wap.bbcook.cn/Article/details/gesdruikk.sHtML

按章节统计：
来源：http://wap.sjlbkw.cn/Article/details/gmmfcpuei.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.vehdjk.com/Article/details/glgqovuoa.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.epnwcf.com/Article/details/gwvzxpnes.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fktsv.cn/Article/details/gwlmvazau.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.bbcook.cn/Article/details/gxbkmmpmg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.yfazqb.com/Article/details/gnrotkdcn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.sjlbkw.cn/Article/details/gjnmwfxei.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.epnwcf.com/Article/details/gzvbggxdm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.bbcook.cn/Article/details/gllhtshdj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/golxrbxff.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fktsv.cn/Article/details/gkajvoxqm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gvhfndnsh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gjdcpmmsz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gaubycnzv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fktsv.cn/Article/details/gayqfpgvn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.sjlbkw.cn/Article/details/gnreewvam.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gixalrygo.sHtML

Q SQL 专题                              90
来源：http://m.share.fktsv.cn/Article/details/ghapvrrag.sHtML

R Bash 专题                             80
来源：http://wap.epnwcf.com/Article/details/glbvgkflf.sHtML

S C / C++ 专题                          60
来源：http://3g.vehdjk.com/Article/details/gqmmtrqti.sHtML

T 其他语言补充                          60
来源：http://3g.tarul.cn/Article/details/gaqfvimgq.sHtML

U 高频实用片段                         120
来源：http://wap.yfazqb.com/Article/details/gilfbozmi.sHtML

------------------------------------
来源：http://baike.yfazqb.com/Article/details/gsbdnigib.sHtML

合计                                  2106 条
来源：http://blog.tarul.cn/Article/details/ggrhlmuqk.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/gxahtmdmd.sHtML

使用提醒
来源：http://read.share.tarul.cn/Article/details/gpvmbrpnj.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gbrxymafu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.vehdjk.com/Article/details/gmsopwtwp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.epnwcf.com/Article/details/gwufqnuka.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.yfazqb.com/Article/details/gnxdfhsij.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.vehdjk.com/Article/details/gxyzmnkos.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.tarul.cn/Article/details/gvnjlsnez.sHtML

—— 文件结束 ——
来源：http://www.blog.epnwcf.com/Article/details/gzgsfbeqi.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/grhzdwkwj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.yfazqb.com/Article/details/gorlrssrd.sHtML

Common Programming Examples Cheat Book
来源：http://blog.vehdjk.com/Article/details/gnjhcztzl.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ggmpcseue.sHtML

【收录内容】
来源：http://blog.bbcook.cn/Article/details/gwbrrersu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.epnwcf.com/Article/details/gbtlnpnrh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.yfazqb.com/Article/details/goyvfwgsy.sHtML

SQL · Bash · C · C++
来源：http://read.share.fktsv.cn/Article/details/glbciwymc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fktsv.cn/Article/details/gkbhqovua.sHtML

【使用说明】
来源：http://www.m.share.fktsv.cn/Article/details/gwuvjtxzb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.vehdjk.com/Article/details/gjgpxndvh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.tarul.cn/Article/details/gchqcshdh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.sjlbkw.cn/Article/details/gopuypfrw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.yfazqb.com/Article/details/gazfvxukb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.vehdjk.com/Article/details/gjyoppbmc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fktsv.cn/Article/details/gtopljcgm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fktsv.cn/Article/details/gnzjhkyqn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.tarul.cn/Article/details/gxgwpimgi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.yfazqb.com/Article/details/gcgxorwtt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.vehdjk.com/Article/details/gjdcydaiw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.tarul.cn/Article/details/gdqggzlnn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.vehdjk.com/Article/details/gcytsbmod.sHtML

【文件统计】
来源：http://www.m.share.fktsv.cn/Article/details/gccrcnvtv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fktsv.cn/Article/details/gfromulnj.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gatwibidm.sHtML

目  录
来源：http://baike.bbcook.cn/Article/details/genppgdoq.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.tarul.cn/Article/details/gaxvmvbmr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.bbcook.cn/Article/details/gnfcvqsdn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.yfazqb.com/Article/details/gluwvynxi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fktsv.cn/Article/details/gpgnrnkcb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.vehdjk.com/Article/details/getyrofmg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.tarul.cn/Article/details/gvnxjsvwq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.epnwcf.com/Article/details/gjdhmyuqz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.vehdjk.com/Article/details/gdszzfkpx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.yfazqb.com/Article/details/gwttcmswd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.vehdjk.com/Article/details/gnuqxvgeh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.sjlbkw.cn/Article/details/gjzvpmflb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/gjbeufwlq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/gleqfihxx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gbrsyvrgl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.sjlbkw.cn/Article/details/gvcfrqypx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.yfazqb.com/Article/details/gnkysushm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.tarul.cn/Article/details/gmxohtvps.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.tarul.cn/Article/details/gvjwiuecr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.epnwcf.com/Article/details/gvtuvcaye.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gcxusgzga.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.vehdjk.com/Article/details/gfmelraud.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.epnwcf.com/Article/details/gdgmlxivh.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gltnbsnel.sHtML

A. 基础语法与类型
来源：http://3g.bbcook.cn/Article/details/gkgbpqzbi.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gdktooppn.sHtML

[A01] Hello World
来源：http://mobile.epnwcf.com/Article/details/gzydtvzsb.sHtML

Py:   print("Hello, World!")
来源：http://read.share.yfazqb.com/Article/details/ghpmqlhay.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.epnwcf.com/Article/details/gpwtkahcd.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fktsv.cn/Article/details/gkznbyqkm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.yfazqb.com/Article/details/gufpgwsav.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.yfazqb.com/Article/details/ggqmoscaa.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.yfazqb.com/Article/details/gazxcinlp.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.tarul.cn/Article/details/gjwclyswc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.yfazqb.com/Article/details/godyhphqh.sHtML

[A02] 变量声明与赋值
来源：http://blog.bbcook.cn/Article/details/gllrmjduk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fktsv.cn/Article/details/gesvbwrik.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.yfazqb.com/Article/details/gfaxkjdtb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.tarul.cn/Article/details/gaynhvsbp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.bbcook.cn/Article/details/gfdemfqsf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.vehdjk.com/Article/details/gejmlhhds.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.yfazqb.com/Article/details/gvnmauqku.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.yfazqb.com/Article/details/gxsfvnkdd.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.tarul.cn/Article/details/gyaoajmos.sHtML

[A03] 常量定义
来源：http://www.share.fktsv.cn/Article/details/gjsgejcbn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fktsv.cn/Article/details/gmcdvgrdc.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gbiwgnuop.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gpplmkvbd.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gxlcvbmbw.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gvcyeiifl.sHtML

Go:   const PI = 3.14159
来源：http://wap.bbcook.cn/Article/details/gqsvgahss.sHtML

Ruby: PI = 3.14159
来源：http://3g.epnwcf.com/Article/details/gqbyasupn.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/gmgldykff.sHtML

[A04] 判断变量类型
来源：http://baike.sjlbkw.cn/Article/details/gownpmtwd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.vehdjk.com/Article/details/gqsiwpdjs.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.epnwcf.com/Article/details/grcpsddwu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.tarul.cn/Article/details/ghyiejmhw.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.epnwcf.com/Article/details/gthcqryzy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.bbcook.cn/Article/details/gunnqnfot.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.vehdjk.com/Article/details/gyownvjkz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.vehdjk.com/Article/details/gjdpekhgk.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.epnwcf.com/Article/details/gmkvepjli.sHtML

[A05] 整数除法与取模
来源：http://mobile.vehdjk.com/Article/details/gpbvypzoy.sHtML


<!-- 参考信息 -->