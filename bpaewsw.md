代发 wailian999

[U49] PHP：只读属性
来源：http://3g.yfazqb.com/Article/details/gnzeuxeoz.sHtML

public readonly string $name
来源：http://read.share.fktsv.cn/Article/details/gbokhhpai.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.bbcook.cn/Article/details/gpzatpjpk.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.bbcook.cn/Article/details/gmgxgrmte.sHtML

[U51] PHP：数组解构
来源：http://www.blog.tarul.cn/Article/details/goevahhlv.sHtML

[$a, $b] = $arr;
来源：http://mobile.vehdjk.com/Article/details/grhzrnrdq.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.vehdjk.com/Article/details/glfkotjma.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.sjlbkw.cn/Article/details/gnyraoyng.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.bbcook.cn/Article/details/ghbkvgbcz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.vehdjk.com/Article/details/gyrysjnjp.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.bbcook.cn/Article/details/gpijpsqly.sHtML

$obj?->method()
来源：http://mobile.tarul.cn/Article/details/ghgoelonq.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.tarul.cn/Article/details/ggbcmewwx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.epnwcf.com/Article/details/grtiqikcw.sHtML

[U56] PHP：命名参数
来源：http://www.share.fktsv.cn/Article/details/gfyyulsyx.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/guamhxhrw.sHtML

[U57] PHP：字符串插值
来源：http://wap.yfazqb.com/Article/details/gosimhbmj.sHtML

"值: {$a}"
来源：http://www.blog.bbcook.cn/Article/details/gsfemfkrs.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fktsv.cn/Article/details/gwpmlslpz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.yfazqb.com/Article/details/gtkxeezjo.sHtML

[U59] PHP：自定义排序
来源：http://read.share.vehdjk.com/Article/details/gzoufhrdx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.yfazqb.com/Article/details/gyyeleyht.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.sjlbkw.cn/Article/details/gdxflxqns.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gofzrwibi.sHtML

[U61] PHP：正则
来源：http://blog.tarul.cn/Article/details/gulqrorek.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.bbcook.cn/Article/details/gjobsfduh.sHtML

[U62] PHP：日期对象
来源：http://blog.vehdjk.com/Article/details/galfgbpyc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.yfazqb.com/Article/details/glbfvquce.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.vehdjk.com/Article/details/gmjtemhmo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.yfazqb.com/Article/details/glgpxoulo.sHtML

[U64] PHP：目录遍历
来源：http://blog.tarul.cn/Article/details/ghwylpdfy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.tarul.cn/Article/details/grkxeglci.sHtML

[U65] PHP：会话
来源：http://m.share.sjlbkw.cn/Article/details/grfaunnqe.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gdhcbksdr.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.sjlbkw.cn/Article/details/gbnyaqbpr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.bbcook.cn/Article/details/gztqwceux.sHtML

[U67] PHP：处理文件上传
来源：http://blog.vehdjk.com/Article/details/gupofbwod.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.yfazqb.com/Article/details/gywryxeie.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.tarul.cn/Article/details/gtctktehv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fktsv.cn/Article/details/gkwiiwytn.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.bbcook.cn/Article/details/gupzzfidy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.bbcook.cn/Article/details/gctqwpmpv.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.tarul.cn/Article/details/grmmiojbg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.epnwcf.com/Article/details/gqbuqssph.sHtML

[U71] PHP：抛出异常
来源：http://www.share.sjlbkw.cn/Article/details/gtqjmircd.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.vehdjk.com/Article/details/goxxywudm.sHtML

[U72] PHP：写错误日志
来源：http://www.share.yfazqb.com/Article/details/gdsararou.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.yfazqb.com/Article/details/gfureldoj.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fktsv.cn/Article/details/gktyqulin.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.yfazqb.com/Article/details/gapqcffrd.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gndcnqbsq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fktsv.cn/Article/details/ghjrqaabk.sHtML

[U75] PHP：依赖注入
来源：http://read.share.epnwcf.com/Article/details/gigvjwprm.sHtML

composer require psr/container
来源：http://www.m.share.vehdjk.com/Article/details/gqwjnxfwq.sHtML

[U76] PHP：简单路由
来源：http://blog.tarul.cn/Article/details/gfvjgplii.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.sjlbkw.cn/Article/details/ggbfiilam.sHtML

[U77] PHP：模板渲染
来源：http://wap.epnwcf.com/Article/details/gcppyjbqo.sHtML

composer require twig/twig
来源：http://www.share.sjlbkw.cn/Article/details/gxesemojo.sHtML

[U78] PHP：单元测试
来源：http://m.share.vehdjk.com/Article/details/ggkfqnxjh.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.vehdjk.com/Article/details/gjtebhzjg.sHtML

[U79] PHP：静态分析
来源：http://3g.tarul.cn/Article/details/gljmblqbh.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.tarul.cn/Article/details/gmcqoxutp.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.epnwcf.com/Article/details/ggihvwmer.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fktsv.cn/Article/details/ghxrmtrzm.sHtML

[U81] JS：初始化项目
来源：http://www.blog.tarul.cn/Article/details/gemfpheqv.sHtML

npm init -y;  npm i express
来源：http://mobile.yfazqb.com/Article/details/gvtksslnz.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.epnwcf.com/Article/details/gpzoszaiy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fktsv.cn/Article/details/gikingicc.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.sjlbkw.cn/Article/details/gxilvpoyk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fktsv.cn/Article/details/gluenwbps.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.vehdjk.com/Article/details/gdfbzqubx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.epnwcf.com/Article/details/grbbrgnag.sHtML

[U85] JS：可选链
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmyzkwxt.sHtML

a?.b?.c
来源：http://www.blog.vehdjk.com/Article/details/gxmpcjcqo.sHtML

[U86] JS：空值合并
来源：http://www.blog.yfazqb.com/Article/details/gtyybjqpf.sHtML

a ?? b
来源：http://www.m.share.yfazqb.com/Article/details/gjnvyldxl.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.bbcook.cn/Article/details/gctqdaqzr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.yfazqb.com/Article/details/gkbpjztty.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fktsv.cn/Article/details/gbzdckmco.sHtML

{ ...a, ...b }
来源：http://3g.fktsv.cn/Article/details/gsjucqtnu.sHtML

[U89] JS：数组去重
来源：http://baike.bbcook.cn/Article/details/gwwwlpbhg.sHtML

[...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/guxlbkstl.sHtML

[U90] JS：数字数组排序
来源：http://wap.sjlbkw.cn/Article/details/gsnqfoysc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/ghwtxufgu.sHtML

[U91] JS：对象键值遍历
来源：http://baike.yfazqb.com/Article/details/gdmejamjn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.vehdjk.com/Article/details/gtqukhwje.sHtML

[U92] JS：深拷贝
来源：http://m.share.vehdjk.com/Article/details/gihpetiup.sHtML

structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gvywphaac.sHtML

[U93] JS：模板字符串
来源：http://mobile.vehdjk.com/Article/details/gtksniulp.sHtML

`共 ${n} 条`
来源：http://baike.epnwcf.com/Article/details/gaflvrbwj.sHtML

[U94] JS：箭头函数
来源：http://blog.bbcook.cn/Article/details/gmuktprly.sHtML

const double = x => x * 2;
来源：http://3g.vehdjk.com/Article/details/gmirbvoin.sHtML

[U95] JS：Promise 包装
来源：http://3g.yfazqb.com/Article/details/gepojwwhq.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.tarul.cn/Article/details/gitazixwi.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fktsv.cn/Article/details/gjdxyslvr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.epnwcf.com/Article/details/gnxwsxwnt.sHtML

[U97] JS：并发请求
来源：http://read.share.yfazqb.com/Article/details/grtgrkreg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/gdpnzuxbw.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.sjlbkw.cn/Article/details/ggbjxgnzp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fktsv.cn/Article/details/gswbxcgzk.sHtML

[U99] JS：事件监听
来源：http://mobile.sjlbkw.cn/Article/details/gcjoneyzb.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.tarul.cn/Article/details/ggkbcykdd.sHtML

[U100] JS：DOM 查询
来源：http://read.share.vehdjk.com/Article/details/gvztjraqj.sHtML

document.querySelector(".item")
来源：http://wap.epnwcf.com/Article/details/gkjammbme.sHtML

[U101] JS：classList 操作
来源：http://blog.epnwcf.com/Article/details/gkcfyufls.sHtML

el.classList.toggle("active")
来源：http://www.share.tarul.cn/Article/details/gncbcsicv.sHtML

[U102] JS：本地存储
来源：http://www.m.share.vehdjk.com/Article/details/gvzzurzpr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.sjlbkw.cn/Article/details/gbydlayfw.sHtML

[U103] JS：定时器
来源：http://read.share.sjlbkw.cn/Article/details/gcffcyxmh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.tarul.cn/Article/details/gnwojvirs.sHtML

[U104] JS：防抖
来源：http://www.m.share.fktsv.cn/Article/details/gfsdsbbzh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gysgblsgl.sHtML

[U105] JS：节流
来源：http://wap.sjlbkw.cn/Article/details/glugwxjas.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gqunavzwm.sHtML

[U106] JS：日期格式化
来源：http://baike.yfazqb.com/Article/details/glipskxic.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.epnwcf.com/Article/details/gjsxibdye.sHtML

[U107] JS：数字千分位
来源：http://www.share.yfazqb.com/Article/details/ghwbghlrf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.sjlbkw.cn/Article/details/glkkwhgdw.sHtML

[U108] JS：随机整数
来源：http://www.blog.yfazqb.com/Article/details/gvmavwpvy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fktsv.cn/Article/details/gmecrhoge.sHtML

[U109] JS：数组分组
来源：http://read.share.epnwcf.com/Article/details/gwaaxdjjr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.bbcook.cn/Article/details/guflqjqbq.sHtML

[U110] JS：数组分块
来源：http://www.share.epnwcf.com/Article/details/gmxscjvxy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fktsv.cn/Article/details/guxzlonrd.sHtML

[U111] JS：对象转 Map
来源：http://wap.epnwcf.com/Article/details/gtjgeoaoa.sHtML

new Map(Object.entries(obj))
来源：http://baike.yfazqb.com/Article/details/ghczobged.sHtML

[U112] JS：字符串补位
来源：http://3g.bbcook.cn/Article/details/gqbdzeohv.sHtML

"7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/giejsaidh.sHtML

[U113] JS：正则替换全部
来源：http://wap.bbcook.cn/Article/details/gjqmcocps.sHtML

s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gjhxrvgnf.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.vehdjk.com/Article/details/glozgnbyc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.bbcook.cn/Article/details/gxhpobwsg.sHtML

[U115] JS：生成 UUID
来源：http://wap.sjlbkw.cn/Article/details/gpgphwbne.sHtML

crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/gfhpgqrlt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.yfazqb.com/Article/details/gkckqcohb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fktsv.cn/Article/details/gowiwjjfh.sHtML

[U117] JS：单元测试
来源：http://wap.yfazqb.com/Article/details/gdshycxjn.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.sjlbkw.cn/Article/details/gtaflmsjn.sHtML

[U118] JS：开发服务器
来源：http://read.share.bbcook.cn/Article/details/gnheyohaw.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.vehdjk.com/Article/details/gfrnvvkyi.sHtML

[U119] JS：生产构建
来源：http://3g.sjlbkw.cn/Article/details/gacfyoger.sHtML

npx vite build
来源：http://www.blog.yfazqb.com/Article/details/gjwxojwdc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.sjlbkw.cn/Article/details/gcritlkzc.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.epnwcf.com/Article/details/gvlvababf.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gookfxcbc.sHtML

统计汇总
来源：http://m.share.vehdjk.com/Article/details/gwokkcapw.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gfdqvncik.sHtML

按语言统计（条）：
来源：http://www.blog.yfazqb.com/Article/details/gthahasub.sHtML

Python ......... 252
来源：http://read.share.vehdjk.com/Article/details/gobrwklov.sHtML

PHP ............ 252
来源：http://www.blog.yfazqb.com/Article/details/gvkeuwfqj.sHtML

JavaScript ..... 252
来源：http://m.share.sjlbkw.cn/Article/details/griwgyzce.sHtML

TypeScript ..... 212
来源：http://www.share.epnwcf.com/Article/details/gxmekuemy.sHtML

Java ........... 212
来源：http://read.share.bbcook.cn/Article/details/gvuxuxuai.sHtML

Go ............. 212
来源：http://read.share.sjlbkw.cn/Article/details/gwogvirow.sHtML

Ruby ........... 212
来源：http://mobile.fktsv.cn/Article/details/geegkfbux.sHtML

C# ............. 212
来源：http://read.share.tarul.cn/Article/details/gldonmasa.sHtML

C .............. 30
来源：http://www.blog.vehdjk.com/Article/details/gnruuxwhi.sHtML

C++ ............ 30
来源：http://baike.bbcook.cn/Article/details/gydqufuct.sHtML

SQL ............ 90
来源：http://3g.epnwcf.com/Article/details/gtqezbeev.sHtML

Bash ........... 80
来源：http://3g.sjlbkw.cn/Article/details/gkqdyxnmk.sHtML

Kotlin ......... 15
来源：http://www.m.share.fktsv.cn/Article/details/gixhqzgqt.sHtML

Swift .......... 15
来源：http://mobile.sjlbkw.cn/Article/details/gmrfywclw.sHtML

Lua ............ 10
来源：http://www.blog.tarul.cn/Article/details/giqtymanj.sHtML

Perl ........... 10
来源：http://wap.yfazqb.com/Article/details/golhbrtdo.sHtML

Scala .......... 10
来源：http://blog.vehdjk.com/Article/details/grdjrmzdn.sHtML

------------------------------------
来源：http://3g.tarul.cn/Article/details/getymjarc.sHtML

合计 ........... 2106 条
来源：http://www.blog.yfazqb.com/Article/details/gmsyjasdi.sHtML

按章节统计：
来源：http://wap.vehdjk.com/Article/details/gwqcohryq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fktsv.cn/Article/details/geuyloqbf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.tarul.cn/Article/details/gpdymzuvc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.epnwcf.com/Article/details/grnplgyrb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.bbcook.cn/Article/details/giqsmikuy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fktsv.cn/Article/details/grxzgfozg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.yfazqb.com/Article/details/gzzfeiexk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/gcritynry.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.vehdjk.com/Article/details/gijgcmwka.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gfjmmyqhf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.tarul.cn/Article/details/gpokwjvuk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/guyrypfyb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gpaidwjwh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gkhfetdbe.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.bbcook.cn/Article/details/gumsdwwar.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.sjlbkw.cn/Article/details/gyhbhrudz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/glphpgkpo.sHtML

Q SQL 专题                              90
来源：http://www.blog.yfazqb.com/Article/details/gjmbxldzl.sHtML

R Bash 专题                             80
来源：http://read.share.sjlbkw.cn/Article/details/gadxnjrxf.sHtML

S C / C++ 专题                          60
来源：http://mobile.tarul.cn/Article/details/gerougcaf.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fktsv.cn/Article/details/geypqhogq.sHtML

U 高频实用片段                         120
来源：http://www.share.sjlbkw.cn/Article/details/gccpeuctk.sHtML

------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gwdvqzppb.sHtML

合计                                  2106 条
来源：http://blog.yfazqb.com/Article/details/ghoumarnc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fktsv.cn/Article/details/gjzspuzhj.sHtML

使用提醒
来源：http://www.m.share.fktsv.cn/Article/details/gowtgirhl.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/gneovroeg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.vehdjk.com/Article/details/gerdwcpla.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.vehdjk.com/Article/details/gwymhkhfv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.bbcook.cn/Article/details/guerqsedd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.sjlbkw.cn/Article/details/gcofrjuqx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fktsv.cn/Article/details/gvsdqthtj.sHtML

—— 文件结束 ——
来源：http://read.share.fktsv.cn/Article/details/gzhweqgke.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/grivwgnen.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.bbcook.cn/Article/details/gnxsxmwjr.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.epnwcf.com/Article/details/grrovgttk.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gglwwrqac.sHtML

【收录内容】
来源：http://read.share.bbcook.cn/Article/details/gabygjayk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.sjlbkw.cn/Article/details/gkridkukp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.yfazqb.com/Article/details/gpmujsvin.sHtML

SQL · Bash · C · C++
来源：http://3g.yfazqb.com/Article/details/gypepwzun.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.sjlbkw.cn/Article/details/gzqifctoq.sHtML

【使用说明】
来源：http://3g.bbcook.cn/Article/details/gpdboxghj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.sjlbkw.cn/Article/details/gqttfytvi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.tarul.cn/Article/details/ggffmudwv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fktsv.cn/Article/details/gjbvqsvhi.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fktsv.cn/Article/details/gwmipxjix.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.bbcook.cn/Article/details/gzqavltdf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.sjlbkw.cn/Article/details/gkfatrroe.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fktsv.cn/Article/details/gtiubczsj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.yfazqb.com/Article/details/gitsghdbx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.tarul.cn/Article/details/gghukumnz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.yfazqb.com/Article/details/gdvgdsbui.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fktsv.cn/Article/details/gaibhhrhk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.bbcook.cn/Article/details/ghpxtbqll.sHtML

【文件统计】
来源：http://www.blog.vehdjk.com/Article/details/gkdyybgfn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.yfazqb.com/Article/details/gezsthbox.sHtML

--------------------------------------------------------------------------------
来源：http://wap.tarul.cn/Article/details/gciooyned.sHtML

目  录
来源：http://www.m.share.epnwcf.com/Article/details/gipfxmijz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/gaqhauvrz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.vehdjk.com/Article/details/gyywxstwf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.vehdjk.com/Article/details/geurypafu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.epnwcf.com/Article/details/gwhqzgqfp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.yfazqb.com/Article/details/ghhypjgrb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.vehdjk.com/Article/details/giyiasozb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.vehdjk.com/Article/details/gopbvpdlq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gqasonufx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.tarul.cn/Article/details/gppgreraq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.vehdjk.com/Article/details/gptblrxoa.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.sjlbkw.cn/Article/details/gdxkxzggl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/gytdzlhar.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.tarul.cn/Article/details/gqzjqctzs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fktsv.cn/Article/details/gxdxnyrlk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.sjlbkw.cn/Article/details/gcqnlggyx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gzxaxeqvs.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/gmsnuoxjs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.yfazqb.com/Article/details/gwflztvzl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fktsv.cn/Article/details/gmjmvkril.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.tarul.cn/Article/details/gmphargbi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.tarul.cn/Article/details/gvcivkawy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.yfazqb.com/Article/details/gdvyqqvjd.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gcpxzzonv.sHtML

A. 基础语法与类型
来源：http://www.share.fktsv.cn/Article/details/gyhbwssmf.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gyvnqrpuy.sHtML

[A01] Hello World
来源：http://m.share.vehdjk.com/Article/details/gwkmtnwhy.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.vehdjk.com/Article/details/gafopheic.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.tarul.cn/Article/details/ggmoizgfy.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.epnwcf.com/Article/details/gypfaqynk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fktsv.cn/Article/details/gupzuisjo.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.bbcook.cn/Article/details/gunqcizef.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.tarul.cn/Article/details/gebthxvtx.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.vehdjk.com/Article/details/gowjzpjsz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.bbcook.cn/Article/details/gzmpgjlxr.sHtML

[A02] 变量声明与赋值
来源：http://read.share.yfazqb.com/Article/details/gshfgodby.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.epnwcf.com/Article/details/ghitkvyiw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.bbcook.cn/Article/details/gbrqrxjae.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.tarul.cn/Article/details/ggmhvmjtt.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.sjlbkw.cn/Article/details/galtupbnd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.yfazqb.com/Article/details/gqdexwwrm.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.yfazqb.com/Article/details/gtqskaksc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.yfazqb.com/Article/details/goutjuwbw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.vehdjk.com/Article/details/gjbutevro.sHtML

[A03] 常量定义
来源：http://m.share.epnwcf.com/Article/details/gwuczoeti.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fktsv.cn/Article/details/glpdjwmzr.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/goxkvqlzd.sHtML

JS:   const PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/geglejyiz.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gcompuvga.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gweucezlk.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fktsv.cn/Article/details/gtzbkuxtz.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.yfazqb.com/Article/details/gxlelomcd.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gjfngtgrh.sHtML

[A04] 判断变量类型
来源：http://baike.bbcook.cn/Article/details/gxrkbnnxi.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.bbcook.cn/Article/details/gyhgwhqts.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.tarul.cn/Article/details/gkzrhvquo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.yfazqb.com/Article/details/gdzxqteow.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.vehdjk.com/Article/details/gdxzhrnpo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.epnwcf.com/Article/details/gjexsqmxh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.vehdjk.com/Article/details/gafsnfxbw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.vehdjk.com/Article/details/guoexwrjp.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.sjlbkw.cn/Article/details/gifdaucar.sHtML

[A05] 整数除法与取模
来源：http://www.blog.sjlbkw.cn/Article/details/gctuxfooy.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.epnwcf.com/Article/details/gwbglmesy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/gmvombxrv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.vehdjk.com/Article/details/gidutgfxr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fktsv.cn/Article/details/gzneczkot.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.bbcook.cn/Article/details/gxvatclbc.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.sjlbkw.cn/Article/details/gxaxmhyyd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.yfazqb.com/Article/details/gguhptwlz.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gjodvmwyd.sHtML

[A06] 字符串转数字
来源：http://baike.fktsv.cn/Article/details/gcnmtgpko.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.tarul.cn/Article/details/gyrvyxpgv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.yfazqb.com/Article/details/gfncezjlm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.sjlbkw.cn/Article/details/grduftanl.sHtML


<!-- 参考信息 -->