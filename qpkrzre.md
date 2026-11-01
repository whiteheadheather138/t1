代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://wap.sjlbkw.cn/Article/details/gufmikmuh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.tarul.cn/Article/details/gcnjryjvc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.yfazqb.com/Article/details/gsrjjrrbp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.yfazqb.com/Article/details/gokrhfvjb.sHtML

[U43] PHP：声明命名空间
来源：http://baike.bbcook.cn/Article/details/gjolewkay.sHtML

namespace App\Http;
来源：http://3g.yfazqb.com/Article/details/gvckegtbn.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.vehdjk.com/Article/details/gispiftbj.sHtML

declare(strict_types=1);
来源：http://www.blog.tarul.cn/Article/details/gjstjtnxj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.yfazqb.com/Article/details/ggraduyep.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gltonwstm.sHtML

[U46] PHP：可空类型
来源：http://www.blog.epnwcf.com/Article/details/gykdmjruo.sHtML

?string $name = null
来源：http://baike.epnwcf.com/Article/details/ggjnkobqj.sHtML

[U47] PHP：联合类型
来源：http://read.share.sjlbkw.cn/Article/details/gpihfjemg.sHtML

int|string $id
来源：http://m.share.fktsv.cn/Article/details/gdmckxdgx.sHtML

[U48] PHP：纯枚举
来源：http://read.share.tarul.cn/Article/details/ggzimxild.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.bbcook.cn/Article/details/gkprjlqup.sHtML

[U49] PHP：只读属性
来源：http://read.share.vehdjk.com/Article/details/gfkaptifs.sHtML

public readonly string $name
来源：http://wap.yfazqb.com/Article/details/gtganpufv.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fktsv.cn/Article/details/grsmpziuh.sHtML

public function __construct(private int $id) {}
来源：http://3g.yfazqb.com/Article/details/gerkoixnm.sHtML

[U51] PHP：数组解构
来源：http://wap.tarul.cn/Article/details/gtjjgklon.sHtML

[$a, $b] = $arr;
来源：http://wap.yfazqb.com/Article/details/gwsfjxxal.sHtML

[U52] PHP：箭头函数
来源：http://read.share.bbcook.cn/Article/details/glmxjqyib.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.vehdjk.com/Article/details/gmlzpdqau.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fktsv.cn/Article/details/ghrvnwftd.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.vehdjk.com/Article/details/gvrwvqvhv.sHtML

[U54] PHP：空安全调用
来源：http://3g.yfazqb.com/Article/details/gesxdzacd.sHtML

$obj?->method()
来源：http://www.blog.bbcook.cn/Article/details/gfypuixgz.sHtML

[U55] PHP：match 表达式
来源：http://3g.sjlbkw.cn/Article/details/gvdkkxtrf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.epnwcf.com/Article/details/guuamoujt.sHtML

[U56] PHP：命名参数
来源：http://www.blog.yfazqb.com/Article/details/gwmafxhwf.sHtML

f(a: 1, b: 2)
来源：http://m.share.fktsv.cn/Article/details/ggtkhhgqj.sHtML

[U57] PHP：字符串插值
来源：http://blog.fktsv.cn/Article/details/giodcumwm.sHtML

"值: {$a}"
来源：http://blog.fktsv.cn/Article/details/glptrotkf.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.epnwcf.com/Article/details/gmirygsho.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gozyudmqq.sHtML

[U59] PHP：自定义排序
来源：http://wap.yfazqb.com/Article/details/gdpgmobtm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.sjlbkw.cn/Article/details/gtgeaefxk.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.bbcook.cn/Article/details/gsbdwxbpq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.bbcook.cn/Article/details/ggwnktves.sHtML

[U61] PHP：正则
来源：http://www.m.share.tarul.cn/Article/details/grpbclxax.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.epnwcf.com/Article/details/gtxzpbshg.sHtML

[U62] PHP：日期对象
来源：http://baike.bbcook.cn/Article/details/guuoaxptt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.yfazqb.com/Article/details/ghyzcixel.sHtML

[U63] PHP：文件读写
来源：http://blog.sjlbkw.cn/Article/details/gfrtcsppe.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.vehdjk.com/Article/details/gorpzvnkz.sHtML

[U64] PHP：目录遍历
来源：http://wap.fktsv.cn/Article/details/gtwnfonlt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.epnwcf.com/Article/details/genonxjly.sHtML

[U65] PHP：会话
来源：http://3g.vehdjk.com/Article/details/gvrmoswth.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.epnwcf.com/Article/details/gadrboqxc.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fktsv.cn/Article/details/gqxpculqu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.bbcook.cn/Article/details/gspamxchd.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.tarul.cn/Article/details/golpxszjw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.bbcook.cn/Article/details/glkpgizhq.sHtML

[U68] PHP：PDO 连接
来源：http://blog.bbcook.cn/Article/details/gpbsotrwv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.vehdjk.com/Article/details/gpeayggjf.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.yfazqb.com/Article/details/ggylmsvng.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.tarul.cn/Article/details/gltaoswkx.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.bbcook.cn/Article/details/gfiazxbkl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.epnwcf.com/Article/details/gxckxjsfj.sHtML

[U71] PHP：抛出异常
来源：http://blog.sjlbkw.cn/Article/details/gwzwtpwid.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.tarul.cn/Article/details/gjplancoj.sHtML

[U72] PHP：写错误日志
来源：http://wap.sjlbkw.cn/Article/details/gtifckubt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.epnwcf.com/Article/details/gfkkrvtgw.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fktsv.cn/Article/details/gzjnahbwo.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fktsv.cn/Article/details/ganiaovsw.sHtML

[U74] PHP：读取环境变量
来源：http://wap.sjlbkw.cn/Article/details/guffnmzdo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.vehdjk.com/Article/details/gmfjdzjzt.sHtML

[U75] PHP：依赖注入
来源：http://m.share.sjlbkw.cn/Article/details/gxgrncops.sHtML

composer require psr/container
来源：http://www.share.fktsv.cn/Article/details/gjqbabanh.sHtML

[U76] PHP：简单路由
来源：http://baike.tarul.cn/Article/details/gyrdtrwfh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.tarul.cn/Article/details/grccbczax.sHtML

[U77] PHP：模板渲染
来源：http://read.share.epnwcf.com/Article/details/gfgkjjwms.sHtML

composer require twig/twig
来源：http://www.share.sjlbkw.cn/Article/details/gseaveczj.sHtML

[U78] PHP：单元测试
来源：http://3g.fktsv.cn/Article/details/gkttatpkr.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.sjlbkw.cn/Article/details/giqvlmgdc.sHtML

[U79] PHP：静态分析
来源：http://wap.epnwcf.com/Article/details/gdofmwnvv.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.yfazqb.com/Article/details/gjoxahmvc.sHtML

[U80] PHP：代码规范修复
来源：http://blog.vehdjk.com/Article/details/gpqqzlwvs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.vehdjk.com/Article/details/gzqfmalkr.sHtML

[U81] JS：初始化项目
来源：http://wap.tarul.cn/Article/details/grozuccmm.sHtML

npm init -y;  npm i express
来源：http://mobile.fktsv.cn/Article/details/gtwddloqo.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.tarul.cn/Article/details/gxudfzzpm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.bbcook.cn/Article/details/ggwgbudge.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.vehdjk.com/Article/details/glorpdgzm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.vehdjk.com/Article/details/gkrpfaiiv.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.tarul.cn/Article/details/gqmhuexcl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.tarul.cn/Article/details/gmjytginb.sHtML

[U85] JS：可选链
来源：http://wap.vehdjk.com/Article/details/gelauftne.sHtML

a?.b?.c
来源：http://www.blog.yfazqb.com/Article/details/gbgaeyvku.sHtML

[U86] JS：空值合并
来源：http://wap.fktsv.cn/Article/details/gsyrvusgk.sHtML

a ?? b
来源：http://3g.bbcook.cn/Article/details/gidocgsws.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.tarul.cn/Article/details/gbeixycji.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.sjlbkw.cn/Article/details/gqkbgyney.sHtML

[U88] JS：对象展开合并
来源：http://mobile.tarul.cn/Article/details/gotpxitvr.sHtML

{ ...a, ...b }
来源：http://3g.sjlbkw.cn/Article/details/globofaub.sHtML

[U89] JS：数组去重
来源：http://blog.bbcook.cn/Article/details/gncyzjrim.sHtML

[...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/goigordjz.sHtML

[U90] JS：数字数组排序
来源：http://read.share.bbcook.cn/Article/details/gageniopv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/gdzfotmfn.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.epnwcf.com/Article/details/gpkebgowt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fktsv.cn/Article/details/gxmssjuqt.sHtML

[U92] JS：深拷贝
来源：http://blog.fktsv.cn/Article/details/ggvosgykd.sHtML

structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gcregrntp.sHtML

[U93] JS：模板字符串
来源：http://www.blog.yfazqb.com/Article/details/gppnycwlw.sHtML

`共 ${n} 条`
来源：http://read.share.vehdjk.com/Article/details/gidxoefxz.sHtML

[U94] JS：箭头函数
来源：http://m.share.yfazqb.com/Article/details/gensehxrf.sHtML

const double = x => x * 2;
来源：http://blog.sjlbkw.cn/Article/details/ghaobymmu.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.yfazqb.com/Article/details/gbfelmlqw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.bbcook.cn/Article/details/gvvoiawih.sHtML

[U96] JS：async/await 与异常
来源：http://blog.vehdjk.com/Article/details/gwjzlktxe.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/gnaxqzyaf.sHtML

[U97] JS：并发请求
来源：http://www.blog.tarul.cn/Article/details/gauthqyzn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.epnwcf.com/Article/details/gbvyexnvw.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.vehdjk.com/Article/details/gizprhkti.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.tarul.cn/Article/details/gzlreesbl.sHtML

[U99] JS：事件监听
来源：http://www.share.yfazqb.com/Article/details/gleivaoud.sHtML

el.addEventListener("click", e => {})
来源：http://3g.tarul.cn/Article/details/gurypjjqj.sHtML

[U100] JS：DOM 查询
来源：http://read.share.yfazqb.com/Article/details/gxcwqfrkb.sHtML

document.querySelector(".item")
来源：http://baike.tarul.cn/Article/details/gtvmcijoq.sHtML

[U101] JS：classList 操作
来源：http://www.blog.sjlbkw.cn/Article/details/gjjjbhjcz.sHtML

el.classList.toggle("active")
来源：http://m.share.bbcook.cn/Article/details/gwhilmldr.sHtML

[U102] JS：本地存储
来源：http://www.blog.bbcook.cn/Article/details/ghatyvccs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.yfazqb.com/Article/details/gourjwaxn.sHtML

[U103] JS：定时器
来源：http://blog.fktsv.cn/Article/details/gvxbpcqcx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fktsv.cn/Article/details/gfmvsdrga.sHtML

[U104] JS：防抖
来源：http://blog.fktsv.cn/Article/details/glppzonjp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/gazssdybb.sHtML

[U105] JS：节流
来源：http://www.m.share.yfazqb.com/Article/details/ggcpjgivf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.yfazqb.com/Article/details/gayrbqvph.sHtML

[U106] JS：日期格式化
来源：http://3g.epnwcf.com/Article/details/gmzfebync.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fktsv.cn/Article/details/gjdrkyimx.sHtML

[U107] JS：数字千分位
来源：http://3g.fktsv.cn/Article/details/guncclgfm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.bbcook.cn/Article/details/gwujoibro.sHtML

[U108] JS：随机整数
来源：http://blog.yfazqb.com/Article/details/gngdvctrv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.tarul.cn/Article/details/gpmgukmmv.sHtML

[U109] JS：数组分组
来源：http://www.blog.yfazqb.com/Article/details/gfpwnszkd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.vehdjk.com/Article/details/gpuxckurs.sHtML

[U110] JS：数组分块
来源：http://baike.sjlbkw.cn/Article/details/gleuesvjc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.yfazqb.com/Article/details/gktnzqtle.sHtML

[U111] JS：对象转 Map
来源：http://m.share.epnwcf.com/Article/details/grmwepham.sHtML

new Map(Object.entries(obj))
来源：http://baike.yfazqb.com/Article/details/gdawrfbnd.sHtML

[U112] JS：字符串补位
来源：http://blog.fktsv.cn/Article/details/gmvfzzdyx.sHtML

"7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gbupazjja.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fktsv.cn/Article/details/glqifclnx.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gdynjvuwp.sHtML

[U114] JS：JSON 深比较
来源：http://3g.tarul.cn/Article/details/grokhukyo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fktsv.cn/Article/details/gqyhufbxi.sHtML

[U115] JS：生成 UUID
来源：http://wap.fktsv.cn/Article/details/gamgqydyi.sHtML

crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/gzytawgnu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.sjlbkw.cn/Article/details/gpuqvvkex.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.sjlbkw.cn/Article/details/gyuxgncfp.sHtML

[U117] JS：单元测试
来源：http://m.share.tarul.cn/Article/details/gdgkkqhrn.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fktsv.cn/Article/details/gzxrfjfqg.sHtML

[U118] JS：开发服务器
来源：http://read.share.bbcook.cn/Article/details/gsxpvjghm.sHtML

npm i -D vite;  npx vite
来源：http://blog.tarul.cn/Article/details/gnlcpqfip.sHtML

[U119] JS：生产构建
来源：http://www.blog.sjlbkw.cn/Article/details/gtjqrkmkd.sHtML

npx vite build
来源：http://blog.epnwcf.com/Article/details/guigudbrv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.sjlbkw.cn/Article/details/gelszytnk.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.bbcook.cn/Article/details/gpliajqwv.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gdmoonvlu.sHtML

统计汇总
来源：http://m.share.tarul.cn/Article/details/gdmszgnuj.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gsugkcfei.sHtML

按语言统计（条）：
来源：http://m.share.vehdjk.com/Article/details/govysprfx.sHtML

Python ......... 252
来源：http://baike.sjlbkw.cn/Article/details/gkhbuboon.sHtML

PHP ............ 252
来源：http://m.share.tarul.cn/Article/details/gdwkjanck.sHtML

JavaScript ..... 252
来源：http://m.share.fktsv.cn/Article/details/gptpxqvad.sHtML

TypeScript ..... 212
来源：http://read.share.vehdjk.com/Article/details/gvgdhpgek.sHtML

Java ........... 212
来源：http://www.blog.yfazqb.com/Article/details/gfhruqrsu.sHtML

Go ............. 212
来源：http://3g.fktsv.cn/Article/details/gasxbgfwv.sHtML

Ruby ........... 212
来源：http://wap.vehdjk.com/Article/details/gaaqysmzp.sHtML

C# ............. 212
来源：http://baike.yfazqb.com/Article/details/guwkmxlhq.sHtML

C .............. 30
来源：http://read.share.vehdjk.com/Article/details/gvypubqeh.sHtML

C++ ............ 30
来源：http://www.m.share.vehdjk.com/Article/details/gsuzqbvzu.sHtML

SQL ............ 90
来源：http://read.share.bbcook.cn/Article/details/ggtqcvzfx.sHtML

Bash ........... 80
来源：http://baike.tarul.cn/Article/details/gbcvvjwoa.sHtML

Kotlin ......... 15
来源：http://baike.fktsv.cn/Article/details/gndehhcvg.sHtML

Swift .......... 15
来源：http://www.share.fktsv.cn/Article/details/guwgkoxni.sHtML

Lua ............ 10
来源：http://www.share.vehdjk.com/Article/details/gphhsdvdf.sHtML

Perl ........... 10
来源：http://baike.yfazqb.com/Article/details/gexgyxwjl.sHtML

Scala .......... 10
来源：http://wap.sjlbkw.cn/Article/details/ghljjjwmk.sHtML

------------------------------------
来源：http://blog.yfazqb.com/Article/details/golpmcbfl.sHtML

合计 ........... 2106 条
来源：http://baike.fktsv.cn/Article/details/gorrijdwz.sHtML

按章节统计：
来源：http://www.blog.vehdjk.com/Article/details/gzmfhvogt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmsnccrk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.bbcook.cn/Article/details/gdydnopdi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.epnwcf.com/Article/details/gappbbsic.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.vehdjk.com/Article/details/gtignrttg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.yfazqb.com/Article/details/gzwhmylpa.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fktsv.cn/Article/details/gzzcvuwse.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.tarul.cn/Article/details/gwazvjbtn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.tarul.cn/Article/details/gadyopnup.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gyxcjfmdu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.bbcook.cn/Article/details/gfhqrgorc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gtkejkdvz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/gcvurqciv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fktsv.cn/Article/details/gnbppmoxi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.yfazqb.com/Article/details/grzxalrqt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.yfazqb.com/Article/details/gvoifdyfh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/grbtorlvr.sHtML

Q SQL 专题                              90
来源：http://www.blog.epnwcf.com/Article/details/gwscnfrio.sHtML

R Bash 专题                             80
来源：http://baike.yfazqb.com/Article/details/grbvwpwok.sHtML

S C / C++ 专题                          60
来源：http://mobile.sjlbkw.cn/Article/details/glohmpylm.sHtML

T 其他语言补充                          60
来源：http://m.share.bbcook.cn/Article/details/glsphvust.sHtML

U 高频实用片段                         120
来源：http://www.m.share.sjlbkw.cn/Article/details/gcuyeyrvs.sHtML

------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkgntunv.sHtML

合计                                  2106 条
来源：http://3g.fktsv.cn/Article/details/gdztqskau.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fktsv.cn/Article/details/gbeeyscvv.sHtML

使用提醒
来源：http://wap.fktsv.cn/Article/details/gjaqtalsk.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gmlzulzgd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.tarul.cn/Article/details/gjvhmtdsa.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.epnwcf.com/Article/details/grhdvdpfl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.yfazqb.com/Article/details/gireljmsf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.sjlbkw.cn/Article/details/gkqmqqkfd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.bbcook.cn/Article/details/gsexiwscb.sHtML

—— 文件结束 ——
来源：http://baike.epnwcf.com/Article/details/gjfqzrbri.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gxxgevhue.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.bbcook.cn/Article/details/gkpmgesrh.sHtML

Common Programming Examples Cheat Book
来源：http://3g.sjlbkw.cn/Article/details/gpnsbbmrn.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/grsprgbrp.sHtML

【收录内容】
来源：http://blog.epnwcf.com/Article/details/grlejyvxr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.bbcook.cn/Article/details/gweykqkec.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.bbcook.cn/Article/details/gkdeukkdk.sHtML

SQL · Bash · C · C++
来源：http://www.share.tarul.cn/Article/details/gefjrzcgu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.vehdjk.com/Article/details/gsucoltab.sHtML

【使用说明】
来源：http://mobile.tarul.cn/Article/details/gtwcvbqjn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.bbcook.cn/Article/details/gazlcsgxi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.vehdjk.com/Article/details/gchibvspx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fktsv.cn/Article/details/glzznaoha.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fktsv.cn/Article/details/gjzkeuzvh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.vehdjk.com/Article/details/gdulmgmcj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.vehdjk.com/Article/details/gjngvsupl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.epnwcf.com/Article/details/glbrohjkr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fktsv.cn/Article/details/gpgdsemtf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.yfazqb.com/Article/details/gxvvhnlwv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.vehdjk.com/Article/details/gdsgrasxl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.bbcook.cn/Article/details/grrajnwtd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.bbcook.cn/Article/details/gyyxbwtba.sHtML

【文件统计】
来源：http://3g.bbcook.cn/Article/details/gduhpdsay.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.bbcook.cn/Article/details/grhqeoheu.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/glvkopdxi.sHtML

目  录
来源：http://mobile.bbcook.cn/Article/details/gtlwsuqfh.sHtML

--------------------------------------------------------------------------------
来源：http://wap.tarul.cn/Article/details/gmiuwtwtd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.vehdjk.com/Article/details/gxapucmsa.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.yfazqb.com/Article/details/gkpxgpaqd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.yfazqb.com/Article/details/glmabrrrs.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.yfazqb.com/Article/details/gnbykwald.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.yfazqb.com/Article/details/geauojwhh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.epnwcf.com/Article/details/gyoingkwi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.tarul.cn/Article/details/gjgoornwb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.yfazqb.com/Article/details/gwmlsjdlo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/gdmhndkve.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.vehdjk.com/Article/details/gfpuclgni.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gabdggiik.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.epnwcf.com/Article/details/geavzbsvr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/gxiwxozpx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.yfazqb.com/Article/details/gruagtqff.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.epnwcf.com/Article/details/gridxvduq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/gchclmmep.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.tarul.cn/Article/details/gsmjioqwj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.sjlbkw.cn/Article/details/gjahxkcjo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gainfyyqp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.yfazqb.com/Article/details/gzehzkwkj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.sjlbkw.cn/Article/details/gewbunlfe.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gxozanrqt.sHtML

A. 基础语法与类型
来源：http://www.m.share.fktsv.cn/Article/details/gkkokvhtz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gwrsukbak.sHtML

[A01] Hello World
来源：http://mobile.tarul.cn/Article/details/gqxhyhxxx.sHtML

Py:   print("Hello, World!")
来源：http://3g.epnwcf.com/Article/details/gibjiteqw.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.tarul.cn/Article/details/gfyatzrar.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.sjlbkw.cn/Article/details/ghvdcfhmn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.vehdjk.com/Article/details/gtmraftfn.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.tarul.cn/Article/details/gjqvxyooz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.epnwcf.com/Article/details/gqisywqnj.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.epnwcf.com/Article/details/gzholjhlk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.tarul.cn/Article/details/gfxicmypz.sHtML

[A02] 变量声明与赋值
来源：http://m.share.epnwcf.com/Article/details/gnphxjroa.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.tarul.cn/Article/details/gxqoefoup.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gxiwkhorx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.vehdjk.com/Article/details/gboxweuig.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.tarul.cn/Article/details/glzmfgegn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.vehdjk.com/Article/details/gaasrgqah.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.epnwcf.com/Article/details/genoqramv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.bbcook.cn/Article/details/gyekttrfx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fktsv.cn/Article/details/govzvhnms.sHtML

[A03] 常量定义
来源：http://blog.epnwcf.com/Article/details/gxczmqdvj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.tarul.cn/Article/details/gnzbclgwm.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gycytejwz.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gdhcsxwpz.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gjayyfcxm.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gykeumylm.sHtML

Go:   const PI = 3.14159
来源：http://baike.tarul.cn/Article/details/gfjjyqouo.sHtML

Ruby: PI = 3.14159
来源：http://mobile.vehdjk.com/Article/details/gbnnepcfn.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gsmhpyhgg.sHtML

[A04] 判断变量类型
来源：http://m.share.epnwcf.com/Article/details/gvfwjqhty.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.bbcook.cn/Article/details/gopxhzgwo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.sjlbkw.cn/Article/details/gdxbtiokb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.sjlbkw.cn/Article/details/gcbmsiayd.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.epnwcf.com/Article/details/gtugyqkeb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.vehdjk.com/Article/details/gbnwzlbeh.sHtML


<!-- 参考信息 -->