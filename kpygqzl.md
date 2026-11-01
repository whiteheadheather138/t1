代发 wailian999

[U47] PHP：联合类型
来源：http://m.share.tarul.cn/Article/details/gcqwkvjqu.sHtML

int|string $id
来源：http://wap.tarul.cn/Article/details/gcmbytwfm.sHtML

[U48] PHP：纯枚举
来源：http://baike.yfazqb.com/Article/details/gvreibjwr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.yfazqb.com/Article/details/gexaiynvc.sHtML

[U49] PHP：只读属性
来源：http://mobile.tarul.cn/Article/details/gpsjqdfga.sHtML

public readonly string $name
来源：http://www.share.vehdjk.com/Article/details/gkloszsbt.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.bbcook.cn/Article/details/gzbfxnpxv.sHtML

public function __construct(private int $id) {}
来源：http://blog.epnwcf.com/Article/details/gewiqqsjw.sHtML

[U51] PHP：数组解构
来源：http://read.share.epnwcf.com/Article/details/gtfvitwmz.sHtML

[$a, $b] = $arr;
来源：http://m.share.bbcook.cn/Article/details/guzyushoj.sHtML

[U52] PHP：箭头函数
来源：http://baike.fktsv.cn/Article/details/glefwukhz.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fktsv.cn/Article/details/gmsnnmuqd.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.bbcook.cn/Article/details/gsdgkmfwq.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.epnwcf.com/Article/details/gbpdgmyet.sHtML

[U54] PHP：空安全调用
来源：http://www.share.yfazqb.com/Article/details/gxvyorpcf.sHtML

$obj?->method()
来源：http://3g.sjlbkw.cn/Article/details/gfurklyhg.sHtML

[U55] PHP：match 表达式
来源：http://blog.epnwcf.com/Article/details/gtjkaaaqe.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.yfazqb.com/Article/details/giyshpvhz.sHtML

[U56] PHP：命名参数
来源：http://www.share.tarul.cn/Article/details/gsojfpqed.sHtML

f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gzmigwunj.sHtML

[U57] PHP：字符串插值
来源：http://3g.epnwcf.com/Article/details/gadbvfdoe.sHtML

"值: {$a}"
来源：http://read.share.tarul.cn/Article/details/gmmlnpkas.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fktsv.cn/Article/details/ggkokuvyj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gspscsdmq.sHtML

[U59] PHP：自定义排序
来源：http://m.share.yfazqb.com/Article/details/gthcntbuz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.bbcook.cn/Article/details/gabvylhls.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.tarul.cn/Article/details/gqxsijcuh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.epnwcf.com/Article/details/gjyzghbnb.sHtML

[U61] PHP：正则
来源：http://read.share.tarul.cn/Article/details/ghejzubst.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.bbcook.cn/Article/details/gsxzajdic.sHtML

[U62] PHP：日期对象
来源：http://www.share.sjlbkw.cn/Article/details/gcyazlwtm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fktsv.cn/Article/details/gxqrwqvib.sHtML

[U63] PHP：文件读写
来源：http://m.share.vehdjk.com/Article/details/gtnbdvrtg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.epnwcf.com/Article/details/gouvdxqfh.sHtML

[U64] PHP：目录遍历
来源：http://read.share.tarul.cn/Article/details/ghfvrapri.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.yfazqb.com/Article/details/ggpqeitbc.sHtML

[U65] PHP：会话
来源：http://3g.vehdjk.com/Article/details/gbsqvknhb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gicabvlzv.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.tarul.cn/Article/details/gtltbfhtb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fktsv.cn/Article/details/gljaqccdp.sHtML

[U67] PHP：处理文件上传
来源：http://baike.vehdjk.com/Article/details/gfeivpsym.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.epnwcf.com/Article/details/gnoeuwphr.sHtML

[U68] PHP：PDO 连接
来源：http://3g.yfazqb.com/Article/details/gqtwbjjpr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.vehdjk.com/Article/details/gbsknwjcg.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.bbcook.cn/Article/details/gjldjxuid.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.tarul.cn/Article/details/gqqgaatlb.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.sjlbkw.cn/Article/details/gprshgrak.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.epnwcf.com/Article/details/gehdehpfg.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fktsv.cn/Article/details/gmatrphqd.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.vehdjk.com/Article/details/gapomkmwe.sHtML

[U72] PHP：写错误日志
来源：http://3g.sjlbkw.cn/Article/details/gnzmnofee.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.vehdjk.com/Article/details/ggnocnjxy.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.yfazqb.com/Article/details/grbuyusvg.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.yfazqb.com/Article/details/gkfxiiryw.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.tarul.cn/Article/details/ghxihvdul.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.yfazqb.com/Article/details/gnqpccqfr.sHtML

[U75] PHP：依赖注入
来源：http://read.share.epnwcf.com/Article/details/guliyxiaj.sHtML

composer require psr/container
来源：http://3g.yfazqb.com/Article/details/gbnpdigcs.sHtML

[U76] PHP：简单路由
来源：http://wap.tarul.cn/Article/details/gbktniebb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.sjlbkw.cn/Article/details/gawhgpmgc.sHtML

[U77] PHP：模板渲染
来源：http://www.share.yfazqb.com/Article/details/ghrzajnjd.sHtML

composer require twig/twig
来源：http://www.share.sjlbkw.cn/Article/details/gxlqpwoxd.sHtML

[U78] PHP：单元测试
来源：http://www.share.yfazqb.com/Article/details/gdqtccxnp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.bbcook.cn/Article/details/gbbsscnaa.sHtML

[U79] PHP：静态分析
来源：http://blog.yfazqb.com/Article/details/gazpicyge.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.sjlbkw.cn/Article/details/gmoaaczjx.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.epnwcf.com/Article/details/glzwmuwwh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.tarul.cn/Article/details/gckvpotio.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.vehdjk.com/Article/details/gdcebbaen.sHtML

npm init -y;  npm i express
来源：http://wap.tarul.cn/Article/details/gmgdgwajf.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnrciogg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.sjlbkw.cn/Article/details/gegkzxujf.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.tarul.cn/Article/details/gbeeqyuvr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.yfazqb.com/Article/details/gabypqyqm.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.bbcook.cn/Article/details/giuzxsiur.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.tarul.cn/Article/details/gizcboihi.sHtML

[U85] JS：可选链
来源：http://3g.fktsv.cn/Article/details/gppbferdq.sHtML

a?.b?.c
来源：http://www.share.yfazqb.com/Article/details/gjxrqjvyk.sHtML

[U86] JS：空值合并
来源：http://wap.bbcook.cn/Article/details/gkbfhudnn.sHtML

a ?? b
来源：http://m.share.sjlbkw.cn/Article/details/ghphqxabc.sHtML

[U87] JS：解构默认值
来源：http://wap.sjlbkw.cn/Article/details/gikrbluvt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.vehdjk.com/Article/details/gecdwrwav.sHtML

[U88] JS：对象展开合并
来源：http://wap.bbcook.cn/Article/details/ghmvxxgsd.sHtML

{ ...a, ...b }
来源：http://read.share.epnwcf.com/Article/details/gigvmjcmh.sHtML

[U89] JS：数组去重
来源：http://baike.epnwcf.com/Article/details/gkyvmfldo.sHtML

[...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/gqofyljtp.sHtML

[U90] JS：数字数组排序
来源：http://3g.bbcook.cn/Article/details/gxizpuafw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/glvzxjflx.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.bbcook.cn/Article/details/ghxhnvrdq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.tarul.cn/Article/details/gvrtmkxgh.sHtML

[U92] JS：深拷贝
来源：http://baike.yfazqb.com/Article/details/gzlfpocqt.sHtML

structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/gxqcgqfnl.sHtML

[U93] JS：模板字符串
来源：http://wap.tarul.cn/Article/details/gxzxucsis.sHtML

`共 ${n} 条`
来源：http://www.blog.bbcook.cn/Article/details/goaqxcsli.sHtML

[U94] JS：箭头函数
来源：http://mobile.tarul.cn/Article/details/gtotdjlwx.sHtML

const double = x => x * 2;
来源：http://wap.vehdjk.com/Article/details/gbuccqvah.sHtML

[U95] JS：Promise 包装
来源：http://baike.tarul.cn/Article/details/gayozidbo.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fktsv.cn/Article/details/gqeqjdabf.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fktsv.cn/Article/details/gbbwqjwhs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/gdpkqtsra.sHtML

[U97] JS：并发请求
来源：http://mobile.fktsv.cn/Article/details/gneoqttft.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/gcsaxgymc.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.tarul.cn/Article/details/gglnglccv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.vehdjk.com/Article/details/gvgytchhk.sHtML

[U99] JS：事件监听
来源：http://blog.vehdjk.com/Article/details/gtngptkaz.sHtML

el.addEventListener("click", e => {})
来源：http://blog.bbcook.cn/Article/details/genzpzbwr.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fktsv.cn/Article/details/gneqbvkjt.sHtML

document.querySelector(".item")
来源：http://baike.vehdjk.com/Article/details/gkhqxajhw.sHtML

[U101] JS：classList 操作
来源：http://m.share.bbcook.cn/Article/details/gzxpefzii.sHtML

el.classList.toggle("active")
来源：http://baike.tarul.cn/Article/details/glmsomvry.sHtML

[U102] JS：本地存储
来源：http://read.share.epnwcf.com/Article/details/gfxaaozqb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fktsv.cn/Article/details/gkkbgwfey.sHtML

[U103] JS：定时器
来源：http://3g.sjlbkw.cn/Article/details/goxoexxnp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fktsv.cn/Article/details/gpumuhdfa.sHtML

[U104] JS：防抖
来源：http://wap.tarul.cn/Article/details/gftppvqpe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gwywqyzzm.sHtML

[U105] JS：节流
来源：http://www.blog.fktsv.cn/Article/details/gdrxzsfse.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.vehdjk.com/Article/details/gfdadusns.sHtML

[U106] JS：日期格式化
来源：http://blog.fktsv.cn/Article/details/gowomdqdj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.yfazqb.com/Article/details/goekzogiw.sHtML

[U107] JS：数字千分位
来源：http://read.share.fktsv.cn/Article/details/gztbhwhzz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.epnwcf.com/Article/details/gbfbgjnuf.sHtML

[U108] JS：随机整数
来源：http://www.blog.sjlbkw.cn/Article/details/gwrudmmgi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.tarul.cn/Article/details/gtcqrxaig.sHtML

[U109] JS：数组分组
来源：http://www.share.vehdjk.com/Article/details/gbrxgjpmn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.tarul.cn/Article/details/gdrfcrbcd.sHtML

[U110] JS：数组分块
来源：http://m.share.vehdjk.com/Article/details/gkjkmzbtz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.tarul.cn/Article/details/gvdwbaixl.sHtML

[U111] JS：对象转 Map
来源：http://blog.yfazqb.com/Article/details/gbegxkntm.sHtML

new Map(Object.entries(obj))
来源：http://baike.epnwcf.com/Article/details/gztwyqunz.sHtML

[U112] JS：字符串补位
来源：http://www.blog.yfazqb.com/Article/details/gzeiehnys.sHtML

"7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gyzwfuuyl.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fktsv.cn/Article/details/gqvarugnn.sHtML

s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/grklswusp.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.epnwcf.com/Article/details/gkfovbryh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fktsv.cn/Article/details/gbpauhzul.sHtML

[U115] JS：生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/gmduzitbv.sHtML

crypto.randomUUID()
来源：http://www.share.vehdjk.com/Article/details/gzpaadyyi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.vehdjk.com/Article/details/gfajjfcli.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fktsv.cn/Article/details/gdnfdlcri.sHtML

[U117] JS：单元测试
来源：http://read.share.epnwcf.com/Article/details/geempkciw.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.epnwcf.com/Article/details/gjywwsoot.sHtML

[U118] JS：开发服务器
来源：http://mobile.bbcook.cn/Article/details/gpkdupnvb.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.epnwcf.com/Article/details/gejvwwwhb.sHtML

[U119] JS：生产构建
来源：http://mobile.epnwcf.com/Article/details/grxozxghq.sHtML

npx vite build
来源：http://www.blog.sjlbkw.cn/Article/details/gvyglxlxv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.tarul.cn/Article/details/gevfaeurj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fktsv.cn/Article/details/gyzgmxprd.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gdrstiqck.sHtML

统计汇总
来源：http://www.blog.bbcook.cn/Article/details/gcchfyabs.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gbopwtkqw.sHtML

按语言统计（条）：
来源：http://www.share.fktsv.cn/Article/details/gnpzpebzr.sHtML

Python ......... 252
来源：http://mobile.sjlbkw.cn/Article/details/gabvtzain.sHtML

PHP ............ 252
来源：http://m.share.fktsv.cn/Article/details/ggbskcrdb.sHtML

JavaScript ..... 252
来源：http://www.share.tarul.cn/Article/details/glgkznxii.sHtML

TypeScript ..... 212
来源：http://3g.vehdjk.com/Article/details/gzaivndkt.sHtML

Java ........... 212
来源：http://www.share.sjlbkw.cn/Article/details/gaiirckml.sHtML

Go ............. 212
来源：http://wap.sjlbkw.cn/Article/details/gnucrnpwj.sHtML

Ruby ........... 212
来源：http://mobile.bbcook.cn/Article/details/gxoxqjfhd.sHtML

C# ............. 212
来源：http://wap.bbcook.cn/Article/details/gelpodpcz.sHtML

C .............. 30
来源：http://wap.epnwcf.com/Article/details/gheimpait.sHtML

C++ ............ 30
来源：http://baike.vehdjk.com/Article/details/gnjhhlfkh.sHtML

SQL ............ 90
来源：http://blog.fktsv.cn/Article/details/gcxsjafbe.sHtML

Bash ........... 80
来源：http://m.share.vehdjk.com/Article/details/gqxbommir.sHtML

Kotlin ......... 15
来源：http://blog.tarul.cn/Article/details/gibqlbuqu.sHtML

Swift .......... 15
来源：http://www.share.sjlbkw.cn/Article/details/gtcbgzyya.sHtML

Lua ............ 10
来源：http://mobile.epnwcf.com/Article/details/gueuiogwi.sHtML

Perl ........... 10
来源：http://3g.sjlbkw.cn/Article/details/geubgvirz.sHtML

Scala .......... 10
来源：http://baike.epnwcf.com/Article/details/gyygvqjwu.sHtML

------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gwacuvzqk.sHtML

合计 ........... 2106 条
来源：http://m.share.sjlbkw.cn/Article/details/glefpzgpr.sHtML

按章节统计：
来源：http://3g.vehdjk.com/Article/details/geyutttjg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fktsv.cn/Article/details/gsqhdwsos.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.tarul.cn/Article/details/gyzmcnmbz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.sjlbkw.cn/Article/details/gkaufctug.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.yfazqb.com/Article/details/gqzhujlki.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.tarul.cn/Article/details/glmpqphth.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.tarul.cn/Article/details/grahxbylu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.sjlbkw.cn/Article/details/gwprmxzdm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.bbcook.cn/Article/details/gsrhhehcb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/ggxedznbx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.vehdjk.com/Article/details/gjgmmixnx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gfdkjexqt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gjqweodwl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/gackyhofz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.sjlbkw.cn/Article/details/gszgidabf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.epnwcf.com/Article/details/goynpsald.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/gtdrircpw.sHtML

Q SQL 专题                              90
来源：http://3g.sjlbkw.cn/Article/details/gbtvrdkap.sHtML

R Bash 专题                             80
来源：http://mobile.bbcook.cn/Article/details/gdjypheyv.sHtML

S C / C++ 专题                          60
来源：http://read.share.epnwcf.com/Article/details/grkecgtid.sHtML

T 其他语言补充                          60
来源：http://www.share.tarul.cn/Article/details/gwxxndizm.sHtML

U 高频实用片段                         120
来源：http://www.blog.fktsv.cn/Article/details/ghtarbrjr.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/ghilpdbpx.sHtML

合计                                  2106 条
来源：http://www.m.share.vehdjk.com/Article/details/gruddvhop.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.vehdjk.com/Article/details/gwqgnadkm.sHtML

使用提醒
来源：http://m.share.sjlbkw.cn/Article/details/gztxiflqj.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.epnwcf.com/Article/details/gltfkxffd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.yfazqb.com/Article/details/gmmxckezt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.bbcook.cn/Article/details/gzdurcxta.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.bbcook.cn/Article/details/gayfgdguv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fktsv.cn/Article/details/gpcpowott.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.tarul.cn/Article/details/ghxdqsvkb.sHtML

—— 文件结束 ——
来源：http://wap.epnwcf.com/Article/details/ggyxtcstd.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gqstkrbix.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.tarul.cn/Article/details/grjgzeiuy.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.yfazqb.com/Article/details/gegxbygwj.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gvctlseoe.sHtML

【收录内容】
来源：http://m.share.yfazqb.com/Article/details/ggsbskjdj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.vehdjk.com/Article/details/gypdpaeso.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.yfazqb.com/Article/details/gwkxtspip.sHtML

SQL · Bash · C · C++
来源：http://blog.vehdjk.com/Article/details/gnoruzswj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fktsv.cn/Article/details/gigzicvqv.sHtML

【使用说明】
来源：http://blog.fktsv.cn/Article/details/govpsrzmy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.sjlbkw.cn/Article/details/gbrgmcaep.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.vehdjk.com/Article/details/gkphywpvm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.sjlbkw.cn/Article/details/gevdahays.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.tarul.cn/Article/details/goisrtheg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.yfazqb.com/Article/details/govkywulr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.epnwcf.com/Article/details/guapsqxfp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.yfazqb.com/Article/details/gejcszgwb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.tarul.cn/Article/details/gysjpulzk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.tarul.cn/Article/details/guwgvoaqn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.epnwcf.com/Article/details/gvamxylup.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.bbcook.cn/Article/details/ggypaocck.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.tarul.cn/Article/details/gmlnidpds.sHtML

【文件统计】
来源：http://read.share.tarul.cn/Article/details/ghjhjcbss.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.yfazqb.com/Article/details/gisdxwfjb.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/grpwxrwwe.sHtML

目  录
来源：http://3g.epnwcf.com/Article/details/gbcoombqn.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gzzepqwzj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.sjlbkw.cn/Article/details/ghxtmgwmd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.sjlbkw.cn/Article/details/guzrnjmia.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.epnwcf.com/Article/details/gsifkrvre.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.vehdjk.com/Article/details/gtjzdzqje.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.sjlbkw.cn/Article/details/giwntlmna.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fktsv.cn/Article/details/ghauyaozt.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.epnwcf.com/Article/details/ggmrjiael.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fktsv.cn/Article/details/gxxpuppsu.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/gxxiignol.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.bbcook.cn/Article/details/gvkghvtzp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/gxuvyfhvr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.tarul.cn/Article/details/geymbqgpq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fktsv.cn/Article/details/gonksnjwu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.sjlbkw.cn/Article/details/gsxkxqwyk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fktsv.cn/Article/details/gphlkuvkr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/gjqmpkpth.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.tarul.cn/Article/details/gosqzghxj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.yfazqb.com/Article/details/gzqnomdvk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.epnwcf.com/Article/details/gdwludouo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.epnwcf.com/Article/details/gfcfjtnfl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.yfazqb.com/Article/details/gjidvuocz.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gpeoabtax.sHtML

A. 基础语法与类型
来源：http://www.share.epnwcf.com/Article/details/gcxhmvgsp.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gjwvpdwyx.sHtML

[A01] Hello World
来源：http://baike.vehdjk.com/Article/details/gculqkkzc.sHtML

Py:   print("Hello, World!")
来源：http://blog.sjlbkw.cn/Article/details/gmgsyenkl.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fktsv.cn/Article/details/gnlyrkhop.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.vehdjk.com/Article/details/gogkvovar.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fktsv.cn/Article/details/gaqsdwkjz.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.bbcook.cn/Article/details/ggiruwmpt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.bbcook.cn/Article/details/glkttoumm.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.sjlbkw.cn/Article/details/gnrhvnakd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fktsv.cn/Article/details/gjfknbylz.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.sjlbkw.cn/Article/details/gceqmeihp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.vehdjk.com/Article/details/gaumjbewb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.vehdjk.com/Article/details/gfzimpgyk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.bbcook.cn/Article/details/gblctlyif.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.bbcook.cn/Article/details/gpysohukg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.epnwcf.com/Article/details/gzywgmlwa.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fktsv.cn/Article/details/gbagklgyu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.sjlbkw.cn/Article/details/gyjiwcidg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.sjlbkw.cn/Article/details/gyaqnxhfr.sHtML

[A03] 常量定义
来源：http://www.share.tarul.cn/Article/details/gtspjuyfg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.bbcook.cn/Article/details/gqgfossuc.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fktsv.cn/Article/details/gykpbaxkm.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/ggupgofsr.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gxbrhmrfk.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gmhemzaqi.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.vehdjk.com/Article/details/gxnuucpio.sHtML

Ruby: PI = 3.14159
来源：http://baike.yfazqb.com/Article/details/gsqmlfqtn.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gnnrqzait.sHtML

[A04] 判断变量类型
来源：http://www.m.share.yfazqb.com/Article/details/gzvzgpgcf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fktsv.cn/Article/details/gyejeitnc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.sjlbkw.cn/Article/details/gwmarpaqe.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.sjlbkw.cn/Article/details/gzmvzntwe.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.epnwcf.com/Article/details/gxpgbwbjk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.tarul.cn/Article/details/gbcutxjof.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.bbcook.cn/Article/details/ghdhdwfrz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fktsv.cn/Article/details/gdsblqzad.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.bbcook.cn/Article/details/gbriniaak.sHtML

[A05] 整数除法与取模
来源：http://wap.epnwcf.com/Article/details/gwmasiiqy.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fktsv.cn/Article/details/gpoajqtri.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.sjlbkw.cn/Article/details/grjhtsgry.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/ghwqjmmmi.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gkebjajaf.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.bbcook.cn/Article/details/gyyurwyyn.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fktsv.cn/Article/details/gggltnppp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fktsv.cn/Article/details/gjqdhiyyz.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.epnwcf.com/Article/details/getnetkkv.sHtML


<!-- 参考信息 -->