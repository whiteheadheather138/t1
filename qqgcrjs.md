代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.yfazqb.com/Article/details/gqtkcsqpe.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.yfazqb.com/Article/details/gnhstkgvk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fktsv.cn/Article/details/gpwnqvzdg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.sjlbkw.cn/Article/details/gjjaeajbf.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.vehdjk.com/Article/details/gbwgnvdrr.sHtML

namespace App\Http;
来源：http://m.share.fktsv.cn/Article/details/gducrqdgl.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.bbcook.cn/Article/details/gbxvcxkxp.sHtML

declare(strict_types=1);
来源：http://www.blog.fktsv.cn/Article/details/gocszqlec.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.bbcook.cn/Article/details/gevfdtjcs.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gbaotrsnc.sHtML

[U46] PHP：可空类型
来源：http://wap.epnwcf.com/Article/details/gdapjmxrs.sHtML

?string $name = null
来源：http://mobile.vehdjk.com/Article/details/gjmijamrq.sHtML

[U47] PHP：联合类型
来源：http://mobile.sjlbkw.cn/Article/details/gjdsqgrvj.sHtML

int|string $id
来源：http://www.share.tarul.cn/Article/details/gsaiqiuhd.sHtML

[U48] PHP：纯枚举
来源：http://mobile.tarul.cn/Article/details/gfrtpxxzu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.vehdjk.com/Article/details/geqsrnkwz.sHtML

[U49] PHP：只读属性
来源：http://3g.yfazqb.com/Article/details/girotqork.sHtML

public readonly string $name
来源：http://www.blog.yfazqb.com/Article/details/gywakoyhl.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fktsv.cn/Article/details/givrpkkvi.sHtML

public function __construct(private int $id) {}
来源：http://read.share.yfazqb.com/Article/details/gmshbbmap.sHtML

[U51] PHP：数组解构
来源：http://www.share.sjlbkw.cn/Article/details/gemjphxsq.sHtML

[$a, $b] = $arr;
来源：http://read.share.epnwcf.com/Article/details/gddgyqzap.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fktsv.cn/Article/details/gbibpucgr.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.yfazqb.com/Article/details/gznkavomg.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.yfazqb.com/Article/details/grhcuowmu.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.sjlbkw.cn/Article/details/gnivsioxz.sHtML

[U54] PHP：空安全调用
来源：http://3g.yfazqb.com/Article/details/gnklsfrhe.sHtML

$obj?->method()
来源：http://read.share.bbcook.cn/Article/details/gikjsfgwj.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.bbcook.cn/Article/details/gtdiapayq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.sjlbkw.cn/Article/details/gqlnjdmdg.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhngmflp.sHtML

f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gtnobojet.sHtML

[U57] PHP：字符串插值
来源：http://wap.bbcook.cn/Article/details/gwindxhrn.sHtML

"值: {$a}"
来源：http://mobile.bbcook.cn/Article/details/gmwucerao.sHtML

[U58] PHP：数组三件套
来源：http://mobile.yfazqb.com/Article/details/gvusuowkw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.tarul.cn/Article/details/gnlsriwhi.sHtML

[U59] PHP：自定义排序
来源：http://www.share.vehdjk.com/Article/details/gsrakimrj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fktsv.cn/Article/details/gubibqlhx.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fktsv.cn/Article/details/gsvhcdfnl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.tarul.cn/Article/details/grfrarmiw.sHtML

[U61] PHP：正则
来源：http://m.share.fktsv.cn/Article/details/giiestozr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.vehdjk.com/Article/details/gkkmenqgr.sHtML

[U62] PHP：日期对象
来源：http://baike.tarul.cn/Article/details/gpdkrjebr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.vehdjk.com/Article/details/gwedmavmx.sHtML

[U63] PHP：文件读写
来源：http://mobile.bbcook.cn/Article/details/ghahycown.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.epnwcf.com/Article/details/gcozurcqm.sHtML

[U64] PHP：目录遍历
来源：http://m.share.sjlbkw.cn/Article/details/gmxhhcvpv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.sjlbkw.cn/Article/details/gpebbkehn.sHtML

[U65] PHP：会话
来源：http://read.share.bbcook.cn/Article/details/gdjcdsfrh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.tarul.cn/Article/details/gjretnmbz.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.tarul.cn/Article/details/goqhnushu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.vehdjk.com/Article/details/gzhqjstbq.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.tarul.cn/Article/details/gqonzcpat.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.bbcook.cn/Article/details/ggdynsvtb.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fktsv.cn/Article/details/gexvdebep.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.bbcook.cn/Article/details/gwemmrzmc.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.tarul.cn/Article/details/gtqjjhdpx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fktsv.cn/Article/details/gatjrkccp.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.vehdjk.com/Article/details/gckyzrbkm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.epnwcf.com/Article/details/gokclrqmy.sHtML

[U71] PHP：抛出异常
来源：http://m.share.yfazqb.com/Article/details/gvajmgptw.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.epnwcf.com/Article/details/gxvlfowmq.sHtML

[U72] PHP：写错误日志
来源：http://blog.tarul.cn/Article/details/gmbxrpuoc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.yfazqb.com/Article/details/giutoewkg.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.bbcook.cn/Article/details/gvrvlzvvc.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.yfazqb.com/Article/details/gwgthcdbz.sHtML

[U74] PHP：读取环境变量
来源：http://3g.vehdjk.com/Article/details/goqaxdkan.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.epnwcf.com/Article/details/gcvojqdby.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fktsv.cn/Article/details/gffahqetq.sHtML

composer require psr/container
来源：http://m.share.sjlbkw.cn/Article/details/glrtfkzsu.sHtML

[U76] PHP：简单路由
来源：http://blog.epnwcf.com/Article/details/gecwofnjt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.sjlbkw.cn/Article/details/gihimbzzw.sHtML

[U77] PHP：模板渲染
来源：http://wap.tarul.cn/Article/details/gaelxqisn.sHtML

composer require twig/twig
来源：http://baike.vehdjk.com/Article/details/gballsgzy.sHtML

[U78] PHP：单元测试
来源：http://www.blog.epnwcf.com/Article/details/gwaobrwtd.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.sjlbkw.cn/Article/details/ghdmalabo.sHtML

[U79] PHP：静态分析
来源：http://read.share.yfazqb.com/Article/details/ghglabtyz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fktsv.cn/Article/details/glcfvetxv.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fktsv.cn/Article/details/goxpitact.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.sjlbkw.cn/Article/details/gueminbhg.sHtML

[U81] JS：初始化项目
来源：http://blog.epnwcf.com/Article/details/goeziqcmv.sHtML

npm init -y;  npm i express
来源：http://mobile.tarul.cn/Article/details/gqdzuuxjx.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.tarul.cn/Article/details/gsyivqssx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.tarul.cn/Article/details/glfcjncuw.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.tarul.cn/Article/details/gshnichzo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.yfazqb.com/Article/details/ggoeonpau.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.sjlbkw.cn/Article/details/gvvpxsskb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.yfazqb.com/Article/details/ggkawbvsn.sHtML

[U85] JS：可选链
来源：http://read.share.vehdjk.com/Article/details/gnldundse.sHtML

a?.b?.c
来源：http://blog.vehdjk.com/Article/details/gvpmywejo.sHtML

[U86] JS：空值合并
来源：http://www.blog.vehdjk.com/Article/details/gamznurki.sHtML

a ?? b
来源：http://read.share.bbcook.cn/Article/details/gkroabgkl.sHtML

[U87] JS：解构默认值
来源：http://www.blog.epnwcf.com/Article/details/gnlreatyp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.tarul.cn/Article/details/gtjwmarzw.sHtML

[U88] JS：对象展开合并
来源：http://wap.bbcook.cn/Article/details/gotigfckz.sHtML

{ ...a, ...b }
来源：http://blog.sjlbkw.cn/Article/details/gttjkxdnh.sHtML

[U89] JS：数组去重
来源：http://3g.yfazqb.com/Article/details/gokteuphm.sHtML

[...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gxhdyuwhn.sHtML

[U90] JS：数字数组排序
来源：http://baike.yfazqb.com/Article/details/gomuergju.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/goncaneyi.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.tarul.cn/Article/details/gfgagxlvs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.bbcook.cn/Article/details/gxjacbnwe.sHtML

[U92] JS：深拷贝
来源：http://mobile.epnwcf.com/Article/details/ghgqutfoz.sHtML

structuredClone(obj)
来源：http://3g.fktsv.cn/Article/details/gkkstayno.sHtML

[U93] JS：模板字符串
来源：http://www.share.fktsv.cn/Article/details/gtocbmjsm.sHtML

`共 ${n} 条`
来源：http://www.share.sjlbkw.cn/Article/details/gdvomqvpi.sHtML

[U94] JS：箭头函数
来源：http://wap.bbcook.cn/Article/details/gfcihqcan.sHtML

const double = x => x * 2;
来源：http://www.blog.yfazqb.com/Article/details/gnqralbqv.sHtML

[U95] JS：Promise 包装
来源：http://mobile.sjlbkw.cn/Article/details/gxkdgyyoa.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.bbcook.cn/Article/details/gllhnzgko.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.tarul.cn/Article/details/gzhkqzbdt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/gkhkfdhsd.sHtML

[U97] JS：并发请求
来源：http://www.share.epnwcf.com/Article/details/gugrgmxqj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gjkxfrlru.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.vehdjk.com/Article/details/gfdmxtros.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.sjlbkw.cn/Article/details/gxwvxwsfp.sHtML

[U99] JS：事件监听
来源：http://mobile.bbcook.cn/Article/details/gjipmnmbe.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.bbcook.cn/Article/details/gcxswodak.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fktsv.cn/Article/details/glieovlot.sHtML

document.querySelector(".item")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjodkspko.sHtML

[U101] JS：classList 操作
来源：http://www.blog.bbcook.cn/Article/details/gonbidwhw.sHtML

el.classList.toggle("active")
来源：http://wap.sjlbkw.cn/Article/details/gbgvnvqcz.sHtML

[U102] JS：本地存储
来源：http://blog.tarul.cn/Article/details/gmeadovlq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fktsv.cn/Article/details/gyogrmdna.sHtML

[U103] JS：定时器
来源：http://www.blog.yfazqb.com/Article/details/gxwklvndq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.yfazqb.com/Article/details/gaunqhhci.sHtML

[U104] JS：防抖
来源：http://www.m.share.tarul.cn/Article/details/gellfovfi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gvrqsoggm.sHtML

[U105] JS：节流
来源：http://www.share.yfazqb.com/Article/details/gxsemtqwv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.vehdjk.com/Article/details/garxaitda.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/grdyjpsis.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.tarul.cn/Article/details/gwpydgjyh.sHtML

[U107] JS：数字千分位
来源：http://www.share.tarul.cn/Article/details/gwfujxgug.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.vehdjk.com/Article/details/gnwjryqyt.sHtML

[U108] JS：随机整数
来源：http://mobile.epnwcf.com/Article/details/gcucgtiak.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.yfazqb.com/Article/details/gggeyxwks.sHtML

[U109] JS：数组分组
来源：http://mobile.epnwcf.com/Article/details/gunzvwytn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.yfazqb.com/Article/details/gtowecoaq.sHtML

[U110] JS：数组分块
来源：http://blog.fktsv.cn/Article/details/gaqhgibey.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.epnwcf.com/Article/details/gkxzytsns.sHtML

[U111] JS：对象转 Map
来源：http://wap.yfazqb.com/Article/details/gmiukvxtl.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fktsv.cn/Article/details/gqublvbpi.sHtML

[U112] JS：字符串补位
来源：http://www.blog.bbcook.cn/Article/details/gytplsroi.sHtML

"7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/gqlqajvvc.sHtML

[U113] JS：正则替换全部
来源：http://read.share.tarul.cn/Article/details/gqjeuzryu.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gpwkjucmk.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.sjlbkw.cn/Article/details/gabjmjurt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fktsv.cn/Article/details/gzysiojix.sHtML

[U115] JS：生成 UUID
来源：http://read.share.tarul.cn/Article/details/gcbwpjftf.sHtML

crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gqhhvqfil.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fktsv.cn/Article/details/gqmpyohnr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.yfazqb.com/Article/details/geuiknzte.sHtML

[U117] JS：单元测试
来源：http://3g.fktsv.cn/Article/details/galblwqpx.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.yfazqb.com/Article/details/gksbvigwi.sHtML

[U118] JS：开发服务器
来源：http://m.share.tarul.cn/Article/details/gyxvaeelo.sHtML

npm i -D vite;  npx vite
来源：http://3g.epnwcf.com/Article/details/galptxmrk.sHtML

[U119] JS：生产构建
来源：http://wap.bbcook.cn/Article/details/gmmfywndj.sHtML

npx vite build
来源：http://read.share.epnwcf.com/Article/details/gcmbexdhn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.sjlbkw.cn/Article/details/ggyitawcs.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.epnwcf.com/Article/details/ghyjoiyqx.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gtyzqeukq.sHtML

统计汇总
来源：http://3g.yfazqb.com/Article/details/gvspfaitw.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gtirnwtdg.sHtML

按语言统计（条）：
来源：http://read.share.fktsv.cn/Article/details/gadnbyuty.sHtML

Python ......... 252
来源：http://blog.yfazqb.com/Article/details/guibyecsu.sHtML

PHP ............ 252
来源：http://blog.sjlbkw.cn/Article/details/gtotjfwcx.sHtML

JavaScript ..... 252
来源：http://www.blog.sjlbkw.cn/Article/details/gqshrngvb.sHtML

TypeScript ..... 212
来源：http://wap.bbcook.cn/Article/details/gonqnkxsm.sHtML

Java ........... 212
来源：http://mobile.tarul.cn/Article/details/gdeoalnvm.sHtML

Go ............. 212
来源：http://blog.bbcook.cn/Article/details/gqtwajxkd.sHtML

Ruby ........... 212
来源：http://3g.yfazqb.com/Article/details/guiibdhuv.sHtML

C# ............. 212
来源：http://m.share.epnwcf.com/Article/details/gtbjlpdfn.sHtML

C .............. 30
来源：http://read.share.yfazqb.com/Article/details/gavqiakxn.sHtML

C++ ............ 30
来源：http://mobile.sjlbkw.cn/Article/details/gwugppmkq.sHtML

SQL ............ 90
来源：http://blog.tarul.cn/Article/details/gdueymgqn.sHtML

Bash ........... 80
来源：http://read.share.sjlbkw.cn/Article/details/glgpwvovq.sHtML

Kotlin ......... 15
来源：http://www.m.share.vehdjk.com/Article/details/gszsjmvgz.sHtML

Swift .......... 15
来源：http://wap.sjlbkw.cn/Article/details/gqadcrxyl.sHtML

Lua ............ 10
来源：http://m.share.epnwcf.com/Article/details/grxsgohbi.sHtML

Perl ........... 10
来源：http://wap.tarul.cn/Article/details/gnwkimtmr.sHtML

Scala .......... 10
来源：http://read.share.yfazqb.com/Article/details/godrbwcsq.sHtML

------------------------------------
来源：http://blog.vehdjk.com/Article/details/glegqrehh.sHtML

合计 ........... 2106 条
来源：http://wap.epnwcf.com/Article/details/gcblyqsih.sHtML

按章节统计：
来源：http://www.share.yfazqb.com/Article/details/gijxexntb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.vehdjk.com/Article/details/gcjohugxy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fktsv.cn/Article/details/gwclxfjwq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.epnwcf.com/Article/details/gnrcvqabe.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.epnwcf.com/Article/details/gaxizjfsm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fktsv.cn/Article/details/gyeqiisaa.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.bbcook.cn/Article/details/gdmcbrgja.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.epnwcf.com/Article/details/gbyrtzxjk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.yfazqb.com/Article/details/gydkaozco.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/gxgdftqyj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.vehdjk.com/Article/details/ggfmhohgv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/gevptiech.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/gpvyblqww.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/gjneglvdh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.tarul.cn/Article/details/ggdybgoqc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.vehdjk.com/Article/details/gmrjxjsdo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gtdrqwvvl.sHtML

Q SQL 专题                              90
来源：http://www.m.share.bbcook.cn/Article/details/guknbtdhz.sHtML

R Bash 专题                             80
来源：http://3g.bbcook.cn/Article/details/grmhougkk.sHtML

S C / C++ 专题                          60
来源：http://www.share.tarul.cn/Article/details/ghgrerbiw.sHtML

T 其他语言补充                          60
来源：http://m.share.vehdjk.com/Article/details/gpvbpulgi.sHtML

U 高频实用片段                         120
来源：http://baike.yfazqb.com/Article/details/gjfyczxtw.sHtML

------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gtszmfgme.sHtML

合计                                  2106 条
来源：http://www.blog.epnwcf.com/Article/details/gtnrcttog.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fktsv.cn/Article/details/gktqnbung.sHtML

使用提醒
来源：http://www.m.share.epnwcf.com/Article/details/gcskbicab.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/gslcuziwd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.epnwcf.com/Article/details/grtemxbya.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.tarul.cn/Article/details/gcmxmpkey.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.sjlbkw.cn/Article/details/gsknmbype.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.epnwcf.com/Article/details/guhlrnopm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.epnwcf.com/Article/details/gjuxlevwq.sHtML

—— 文件结束 ——
来源：http://wap.fktsv.cn/Article/details/gikorzxzd.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gvpvxyjaw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.epnwcf.com/Article/details/gctjtgege.sHtML

Common Programming Examples Cheat Book
来源：http://wap.yfazqb.com/Article/details/gvjzxxice.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gvccthbif.sHtML

【收录内容】
来源：http://wap.fktsv.cn/Article/details/gvuhvlmfa.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.tarul.cn/Article/details/gfagoqtkb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fktsv.cn/Article/details/godrceach.sHtML

SQL · Bash · C · C++
来源：http://www.blog.vehdjk.com/Article/details/gqzimxscs.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.vehdjk.com/Article/details/gmhvrcrzw.sHtML

【使用说明】
来源：http://wap.yfazqb.com/Article/details/gyygqrqwt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.vehdjk.com/Article/details/ggpiwfkic.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.yfazqb.com/Article/details/grkvbqfla.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.yfazqb.com/Article/details/gslclsfpy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.epnwcf.com/Article/details/gwcntpaer.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.vehdjk.com/Article/details/goitwhfyd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.tarul.cn/Article/details/gtvdhjeaz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.yfazqb.com/Article/details/gbwmhnfbg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.sjlbkw.cn/Article/details/gcmzfrvwz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.yfazqb.com/Article/details/goxuubmhk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fktsv.cn/Article/details/gewyrdlzm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.tarul.cn/Article/details/grqkertab.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fktsv.cn/Article/details/gbumdyzgn.sHtML

【文件统计】
来源：http://mobile.yfazqb.com/Article/details/glfinietw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.sjlbkw.cn/Article/details/gngmtteph.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.yfazqb.com/Article/details/gbtjfeqfo.sHtML

目  录
来源：http://www.m.share.tarul.cn/Article/details/gjhbiastl.sHtML

--------------------------------------------------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gvfjusnhl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.bbcook.cn/Article/details/gvqdbuzxn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.yfazqb.com/Article/details/gyuwpfvij.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.bbcook.cn/Article/details/gyxbvkqgt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.tarul.cn/Article/details/gseonsttb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.epnwcf.com/Article/details/gqrcbtkuf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.tarul.cn/Article/details/gtjdvxneq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.vehdjk.com/Article/details/ghadouhib.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.vehdjk.com/Article/details/gxgdbjcyx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/gkrhsjeex.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fktsv.cn/Article/details/gxdplltug.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/gaklagpto.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.bbcook.cn/Article/details/grwkslgmd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fktsv.cn/Article/details/gpiaeeefn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fktsv.cn/Article/details/gamszumoi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.yfazqb.com/Article/details/glkdjhaxi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/guxmfpdom.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.vehdjk.com/Article/details/ggakxzbht.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.sjlbkw.cn/Article/details/gzhfofqib.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.vehdjk.com/Article/details/glbqhhkml.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fktsv.cn/Article/details/gmmknjhtm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.bbcook.cn/Article/details/gjrxyrlgw.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gjnmeehbl.sHtML

A. 基础语法与类型
来源：http://wap.yfazqb.com/Article/details/ggathwdil.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/guobpqbzh.sHtML

[A01] Hello World
来源：http://wap.sjlbkw.cn/Article/details/gougmuhzq.sHtML

Py:   print("Hello, World!")
来源：http://mobile.sjlbkw.cn/Article/details/gwelnerya.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.tarul.cn/Article/details/gaupdpfma.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.epnwcf.com/Article/details/gqhvkpknu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.bbcook.cn/Article/details/gijmmhxjf.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.sjlbkw.cn/Article/details/gtkqywerb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.sjlbkw.cn/Article/details/gglqlckzl.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.epnwcf.com/Article/details/gezgynfpu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.sjlbkw.cn/Article/details/grvfbapzj.sHtML

[A02] 变量声明与赋值
来源：http://read.share.sjlbkw.cn/Article/details/gnveuyeug.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.yfazqb.com/Article/details/govupyvaq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.vehdjk.com/Article/details/gahdzmnhb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.vehdjk.com/Article/details/gzqqoqnif.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fktsv.cn/Article/details/gabxvnnfo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.bbcook.cn/Article/details/gtbbwvapj.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.yfazqb.com/Article/details/gwnwrrwwg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.tarul.cn/Article/details/gaefemzlg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.yfazqb.com/Article/details/gszhwronc.sHtML

[A03] 常量定义
来源：http://www.m.share.bbcook.cn/Article/details/giqhznfua.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.sjlbkw.cn/Article/details/gtapzrfxt.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gjqoxhkzz.sHtML

JS:   const PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gutokedjm.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.tarul.cn/Article/details/giywjksoe.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gphecamkz.sHtML

Go:   const PI = 3.14159
来源：http://mobile.sjlbkw.cn/Article/details/gezausewr.sHtML

Ruby: PI = 3.14159
来源：http://read.share.tarul.cn/Article/details/ginockelg.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gghdmnzoa.sHtML

[A04] 判断变量类型
来源：http://3g.bbcook.cn/Article/details/gdfjilvbl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.bbcook.cn/Article/details/ghujtpndm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.yfazqb.com/Article/details/gfsgrwqrg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.epnwcf.com/Article/details/gicrxfxsq.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.epnwcf.com/Article/details/gpdwmysuu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.sjlbkw.cn/Article/details/gkbmthodd.sHtML


<!-- 参考信息 -->