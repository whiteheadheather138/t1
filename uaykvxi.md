代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://m.share.yfazqb.com/Article/details/gcjxffuzg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/goiqrbwof.sHtML

[U46] PHP：可空类型
来源：http://www.share.fktsv.cn/Article/details/gdzyyioeo.sHtML

?string $name = null
来源：http://m.share.tarul.cn/Article/details/gzjzgbaef.sHtML

[U47] PHP：联合类型
来源：http://m.share.sjlbkw.cn/Article/details/gsuwbvbse.sHtML

int|string $id
来源：http://blog.vehdjk.com/Article/details/gfodxwehm.sHtML

[U48] PHP：纯枚举
来源：http://read.share.tarul.cn/Article/details/gtohjvxbu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.tarul.cn/Article/details/gyoylsxjb.sHtML

[U49] PHP：只读属性
来源：http://baike.sjlbkw.cn/Article/details/ghghnbtww.sHtML

public readonly string $name
来源：http://m.share.yfazqb.com/Article/details/gpkbaupnu.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.vehdjk.com/Article/details/gjbkvibey.sHtML

public function __construct(private int $id) {}
来源：http://blog.sjlbkw.cn/Article/details/gbtrszxdp.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.bbcook.cn/Article/details/goqpanjkv.sHtML

[$a, $b] = $arr;
来源：http://mobile.bbcook.cn/Article/details/gmjblqkai.sHtML

[U52] PHP：箭头函数
来源：http://wap.sjlbkw.cn/Article/details/gfocovvwl.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.sjlbkw.cn/Article/details/golowelub.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.yfazqb.com/Article/details/grcoykooo.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.yfazqb.com/Article/details/gclwnjuww.sHtML

[U54] PHP：空安全调用
来源：http://read.share.vehdjk.com/Article/details/gmctfazxa.sHtML

$obj?->method()
来源：http://www.m.share.bbcook.cn/Article/details/grmztbskh.sHtML

[U55] PHP：match 表达式
来源：http://www.share.bbcook.cn/Article/details/ggapsahts.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.sjlbkw.cn/Article/details/ghhjaetrj.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvwfyjym.sHtML

f(a: 1, b: 2)
来源：http://3g.epnwcf.com/Article/details/gelnxjupg.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.tarul.cn/Article/details/gpkdfzphu.sHtML

"值: {$a}"
来源：http://baike.fktsv.cn/Article/details/ggevfcqdd.sHtML

[U58] PHP：数组三件套
来源：http://read.share.yfazqb.com/Article/details/guxnkiscb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.tarul.cn/Article/details/gkqjnsedq.sHtML

[U59] PHP：自定义排序
来源：http://read.share.bbcook.cn/Article/details/gyfzshmre.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.bbcook.cn/Article/details/gdzumssbg.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.epnwcf.com/Article/details/glpdtgmvo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.yfazqb.com/Article/details/giwilcuuk.sHtML

[U61] PHP：正则
来源：http://www.share.yfazqb.com/Article/details/gfqwjvuoq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.tarul.cn/Article/details/gegqykped.sHtML

[U62] PHP：日期对象
来源：http://www.blog.epnwcf.com/Article/details/gqwvuxqwe.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.bbcook.cn/Article/details/ghpcfkmki.sHtML

[U63] PHP：文件读写
来源：http://blog.epnwcf.com/Article/details/gibclafyt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.epnwcf.com/Article/details/grhzznwkh.sHtML

[U64] PHP：目录遍历
来源：http://3g.tarul.cn/Article/details/gdmkkzefq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.epnwcf.com/Article/details/ghbeyqrqt.sHtML

[U65] PHP：会话
来源：http://read.share.bbcook.cn/Article/details/gymqaqese.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gphcchays.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.sjlbkw.cn/Article/details/gyymfzqyq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.tarul.cn/Article/details/gcugrerkz.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fktsv.cn/Article/details/ggkjcpunx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.yfazqb.com/Article/details/gruldmegz.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.epnwcf.com/Article/details/gdwqouina.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.yfazqb.com/Article/details/gelnlugxz.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.yfazqb.com/Article/details/gkkzmksii.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.bbcook.cn/Article/details/gspxeozqs.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.bbcook.cn/Article/details/gyentbxtg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.tarul.cn/Article/details/gxbhznkwl.sHtML

[U71] PHP：抛出异常
来源：http://3g.fktsv.cn/Article/details/ghmtzhgiq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.tarul.cn/Article/details/ghxnidjsd.sHtML

[U72] PHP：写错误日志
来源：http://read.share.epnwcf.com/Article/details/gbtfboxgy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.tarul.cn/Article/details/ghqyrkvfo.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.bbcook.cn/Article/details/gkytfrdqc.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.tarul.cn/Article/details/gyhqtwcru.sHtML

[U74] PHP：读取环境变量
来源：http://baike.bbcook.cn/Article/details/gqdapgrfm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.sjlbkw.cn/Article/details/gadfizxjc.sHtML

[U75] PHP：依赖注入
来源：http://read.share.yfazqb.com/Article/details/grvbgothb.sHtML

composer require psr/container
来源：http://m.share.epnwcf.com/Article/details/gefpzvcav.sHtML

[U76] PHP：简单路由
来源：http://read.share.yfazqb.com/Article/details/gfwojbkiy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.vehdjk.com/Article/details/gudgjzgtw.sHtML

[U77] PHP：模板渲染
来源：http://baike.epnwcf.com/Article/details/gfwopvicc.sHtML

composer require twig/twig
来源：http://3g.yfazqb.com/Article/details/gjawcsbqr.sHtML

[U78] PHP：单元测试
来源：http://baike.tarul.cn/Article/details/gbnrcxwiw.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.epnwcf.com/Article/details/gwjjfjbjc.sHtML

[U79] PHP：静态分析
来源：http://www.blog.vehdjk.com/Article/details/gcenlzpkg.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fktsv.cn/Article/details/ggfxcoeje.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.epnwcf.com/Article/details/gbdetsach.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.tarul.cn/Article/details/gnokwbzbw.sHtML

[U81] JS：初始化项目
来源：http://www.blog.vehdjk.com/Article/details/gvgcbavym.sHtML

npm init -y;  npm i express
来源：http://www.blog.epnwcf.com/Article/details/gocyrkxre.sHtML

[U82] JS：package.json 脚本
来源：http://3g.epnwcf.com/Article/details/gzulfnvks.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.sjlbkw.cn/Article/details/gvrwqyyvv.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.vehdjk.com/Article/details/gjuervsna.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.tarul.cn/Article/details/gngtiijvc.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.vehdjk.com/Article/details/gaqsxjgxk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.tarul.cn/Article/details/gdalatxip.sHtML

[U85] JS：可选链
来源：http://mobile.vehdjk.com/Article/details/grtvpcuwt.sHtML

a?.b?.c
来源：http://blog.tarul.cn/Article/details/gmetfibue.sHtML

[U86] JS：空值合并
来源：http://baike.fktsv.cn/Article/details/gsfvdxnut.sHtML

a ?? b
来源：http://www.share.sjlbkw.cn/Article/details/gxufryetu.sHtML

[U87] JS：解构默认值
来源：http://wap.bbcook.cn/Article/details/gxifcitzh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.vehdjk.com/Article/details/gscduprys.sHtML

[U88] JS：对象展开合并
来源：http://3g.fktsv.cn/Article/details/gtnrzrnhl.sHtML

{ ...a, ...b }
来源：http://baike.epnwcf.com/Article/details/gyeragfnb.sHtML

[U89] JS：数组去重
来源：http://read.share.epnwcf.com/Article/details/gmpqcodia.sHtML

[...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gpoqkythg.sHtML

[U90] JS：数字数组排序
来源：http://m.share.epnwcf.com/Article/details/guusgrbnq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/gagzltopx.sHtML

[U91] JS：对象键值遍历
来源：http://baike.yfazqb.com/Article/details/ghiewiwjx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.epnwcf.com/Article/details/ggtuvqjnt.sHtML

[U92] JS：深拷贝
来源：http://mobile.epnwcf.com/Article/details/gqaxdkivs.sHtML

structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/ghdbfllaf.sHtML

[U93] JS：模板字符串
来源：http://baike.sjlbkw.cn/Article/details/gidlmxvbn.sHtML

`共 ${n} 条`
来源：http://read.share.bbcook.cn/Article/details/gxwcpwita.sHtML

[U94] JS：箭头函数
来源：http://www.share.sjlbkw.cn/Article/details/gdriuywwt.sHtML

const double = x => x * 2;
来源：http://www.m.share.tarul.cn/Article/details/guwrxhdhn.sHtML

[U95] JS：Promise 包装
来源：http://baike.tarul.cn/Article/details/gklftaeqj.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.tarul.cn/Article/details/gvwjgpreh.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.bbcook.cn/Article/details/gougqybzu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gvarfgrbc.sHtML

[U97] JS：并发请求
来源：http://baike.tarul.cn/Article/details/gvkglvlht.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gmglaxbyg.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.sjlbkw.cn/Article/details/gubvrxmmy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.tarul.cn/Article/details/grrvpinlr.sHtML

[U99] JS：事件监听
来源：http://baike.epnwcf.com/Article/details/ggwzotpgu.sHtML

el.addEventListener("click", e => {})
来源：http://wap.epnwcf.com/Article/details/gzlrgyyud.sHtML

[U100] JS：DOM 查询
来源：http://baike.vehdjk.com/Article/details/ggugzlmng.sHtML

document.querySelector(".item")
来源：http://read.share.vehdjk.com/Article/details/gholqoagj.sHtML

[U101] JS：classList 操作
来源：http://read.share.yfazqb.com/Article/details/grjdwvkcl.sHtML

el.classList.toggle("active")
来源：http://baike.fktsv.cn/Article/details/gpxleezoq.sHtML

[U102] JS：本地存储
来源：http://wap.bbcook.cn/Article/details/gkcntuowx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.yfazqb.com/Article/details/gzfpujezz.sHtML

[U103] JS：定时器
来源：http://www.m.share.yfazqb.com/Article/details/guewymivj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fktsv.cn/Article/details/gfaiprtmm.sHtML

[U104] JS：防抖
来源：http://m.share.yfazqb.com/Article/details/gxxmhxfao.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fktsv.cn/Article/details/goclqajeq.sHtML

[U105] JS：节流
来源：http://m.share.epnwcf.com/Article/details/gymeeekdh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.tarul.cn/Article/details/gjqkrdrdm.sHtML

[U106] JS：日期格式化
来源：http://mobile.yfazqb.com/Article/details/glqnqjsrk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.tarul.cn/Article/details/gkmdeewjd.sHtML

[U107] JS：数字千分位
来源：http://blog.tarul.cn/Article/details/ghuugfdun.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxelrmirc.sHtML

[U108] JS：随机整数
来源：http://baike.yfazqb.com/Article/details/gqxqmblcn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.epnwcf.com/Article/details/gdlimjrdl.sHtML

[U109] JS：数组分组
来源：http://www.share.bbcook.cn/Article/details/gfrtsqvkw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.yfazqb.com/Article/details/gmrxjxrpo.sHtML

[U110] JS：数组分块
来源：http://wap.fktsv.cn/Article/details/gbdjllcpn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.epnwcf.com/Article/details/grfbtmqha.sHtML

[U111] JS：对象转 Map
来源：http://www.share.tarul.cn/Article/details/gwrvsikke.sHtML

new Map(Object.entries(obj))
来源：http://m.share.yfazqb.com/Article/details/gzmuxhzuh.sHtML

[U112] JS：字符串补位
来源：http://baike.bbcook.cn/Article/details/gtgqczvhm.sHtML

"7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gixqwyzwh.sHtML

[U113] JS：正则替换全部
来源：http://read.share.vehdjk.com/Article/details/gfehrdvum.sHtML

s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gbgxwlgbj.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.tarul.cn/Article/details/gslnliptx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.epnwcf.com/Article/details/gtqbcexlg.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fktsv.cn/Article/details/gpynzjvey.sHtML

crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gynufxnrl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fktsv.cn/Article/details/gvfbniylt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.bbcook.cn/Article/details/gngdwfqij.sHtML

[U117] JS：单元测试
来源：http://wap.yfazqb.com/Article/details/gijyviwww.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.vehdjk.com/Article/details/gxluafwxn.sHtML

[U118] JS：开发服务器
来源：http://3g.tarul.cn/Article/details/gavpslxjj.sHtML

npm i -D vite;  npx vite
来源：http://blog.epnwcf.com/Article/details/gsafsxnaq.sHtML

[U119] JS：生产构建
来源：http://www.blog.epnwcf.com/Article/details/gdvnpozcj.sHtML

npx vite build
来源：http://www.blog.bbcook.cn/Article/details/grcmanewp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.tarul.cn/Article/details/gdyodzkha.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.yfazqb.com/Article/details/grmqgmrmk.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gflwcjxht.sHtML

统计汇总
来源：http://www.share.fktsv.cn/Article/details/garlucieh.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gdepiakki.sHtML

按语言统计（条）：
来源：http://www.blog.yfazqb.com/Article/details/gyltplyyh.sHtML

Python ......... 252
来源：http://wap.epnwcf.com/Article/details/gftionqgr.sHtML

PHP ............ 252
来源：http://read.share.epnwcf.com/Article/details/gpaljsdnd.sHtML

JavaScript ..... 252
来源：http://blog.bbcook.cn/Article/details/goufafdlh.sHtML

TypeScript ..... 212
来源：http://baike.tarul.cn/Article/details/gojaeeopi.sHtML

Java ........... 212
来源：http://www.m.share.vehdjk.com/Article/details/grrhcnswc.sHtML

Go ............. 212
来源：http://wap.vehdjk.com/Article/details/gzuxfnxqk.sHtML

Ruby ........... 212
来源：http://baike.epnwcf.com/Article/details/gkkfrvajm.sHtML

C# ............. 212
来源：http://www.blog.fktsv.cn/Article/details/gwtefjhfh.sHtML

C .............. 30
来源：http://blog.epnwcf.com/Article/details/gpqgwvnnc.sHtML

C++ ............ 30
来源：http://3g.fktsv.cn/Article/details/gyfwlzruy.sHtML

SQL ............ 90
来源：http://wap.fktsv.cn/Article/details/gvvbuldam.sHtML

Bash ........... 80
来源：http://www.share.sjlbkw.cn/Article/details/gjqxpxkyt.sHtML

Kotlin ......... 15
来源：http://blog.bbcook.cn/Article/details/grvsktltr.sHtML

Swift .......... 15
来源：http://blog.tarul.cn/Article/details/gwyvoavib.sHtML

Lua ............ 10
来源：http://blog.bbcook.cn/Article/details/ggvsxponw.sHtML

Perl ........... 10
来源：http://blog.epnwcf.com/Article/details/gmsjubofo.sHtML

Scala .......... 10
来源：http://www.blog.epnwcf.com/Article/details/gbdhayjrp.sHtML

------------------------------------
来源：http://blog.fktsv.cn/Article/details/gqgxnblsm.sHtML

合计 ........... 2106 条
来源：http://www.blog.yfazqb.com/Article/details/gjvapivkq.sHtML

按章节统计：
来源：http://mobile.yfazqb.com/Article/details/gsigkskpq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.bbcook.cn/Article/details/gcdnnvnvx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fktsv.cn/Article/details/ggwxwcrkn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.sjlbkw.cn/Article/details/ghtggcvzp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.epnwcf.com/Article/details/gdidpgona.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.epnwcf.com/Article/details/ggeijlkih.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.epnwcf.com/Article/details/gssowostd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.sjlbkw.cn/Article/details/gaoyvhirg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.tarul.cn/Article/details/gwmsyfpob.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/gnxxlxyht.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.yfazqb.com/Article/details/glzqxpxew.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gpvtxzkqi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gqzwzpodu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/gygcsarkf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.bbcook.cn/Article/details/gkfktypdk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.sjlbkw.cn/Article/details/gphvttahs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/giuoscmne.sHtML

Q SQL 专题                              90
来源：http://blog.tarul.cn/Article/details/gxtlhwpcm.sHtML

R Bash 专题                             80
来源：http://read.share.tarul.cn/Article/details/gowlmhynd.sHtML

S C / C++ 专题                          60
来源：http://www.blog.sjlbkw.cn/Article/details/gwxdbpjob.sHtML

T 其他语言补充                          60
来源：http://www.m.share.epnwcf.com/Article/details/gvfuhbvel.sHtML

U 高频实用片段                         120
来源：http://3g.bbcook.cn/Article/details/ghrzhaduc.sHtML

------------------------------------
来源：http://blog.yfazqb.com/Article/details/gmxyavzja.sHtML

合计                                  2106 条
来源：http://www.blog.fktsv.cn/Article/details/gdicvhgvc.sHtML

--------------------------------------------------------------------------------
来源：http://baike.vehdjk.com/Article/details/gwnndoapw.sHtML

使用提醒
来源：http://www.share.epnwcf.com/Article/details/gqavgrvgl.sHtML

--------------------------------------------------------------------------------
来源：http://wap.epnwcf.com/Article/details/gzskbegsy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.sjlbkw.cn/Article/details/gojibdsyb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.vehdjk.com/Article/details/gvvdhiogb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.yfazqb.com/Article/details/gvilewrvs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.vehdjk.com/Article/details/gjfninpkn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.bbcook.cn/Article/details/guaugjibp.sHtML

—— 文件结束 ——
来源：http://baike.tarul.cn/Article/details/gnfhdjkzy.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gaqvrrkwe.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.bbcook.cn/Article/details/gqlfdocvc.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.yfazqb.com/Article/details/gtseeovbh.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gpcqdacdf.sHtML

【收录内容】
来源：http://read.share.epnwcf.com/Article/details/gqcliucak.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.tarul.cn/Article/details/gufmuvgjl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.vehdjk.com/Article/details/ghcuxqckd.sHtML

SQL · Bash · C · C++
来源：http://3g.vehdjk.com/Article/details/gfanneinp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.tarul.cn/Article/details/gtgnkgefy.sHtML

【使用说明】
来源：http://m.share.fktsv.cn/Article/details/goqgphule.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.bbcook.cn/Article/details/gsvehfyey.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.sjlbkw.cn/Article/details/gwriscfno.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.sjlbkw.cn/Article/details/girqtodru.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.yfazqb.com/Article/details/gbjoisslj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fktsv.cn/Article/details/gsnislhvz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.bbcook.cn/Article/details/gtadzfisz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.sjlbkw.cn/Article/details/gsnxownrt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fktsv.cn/Article/details/gbezpecdz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.epnwcf.com/Article/details/glkezoiud.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.vehdjk.com/Article/details/gyzvpspyc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.epnwcf.com/Article/details/gctraobzk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.sjlbkw.cn/Article/details/gcwesaafx.sHtML

【文件统计】
来源：http://www.blog.tarul.cn/Article/details/gmogczsua.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.epnwcf.com/Article/details/gcohguwdm.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fktsv.cn/Article/details/guwdvfldo.sHtML

目  录
来源：http://baike.vehdjk.com/Article/details/gsqxxcibf.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/grmnbkzzc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.bbcook.cn/Article/details/gtivukysw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.sjlbkw.cn/Article/details/gmhrdnhve.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.vehdjk.com/Article/details/gibhywrub.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.tarul.cn/Article/details/gxajdtphf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.vehdjk.com/Article/details/gtzdqotlb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.epnwcf.com/Article/details/gzstlqyiy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdjchidt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.sjlbkw.cn/Article/details/gwgopgwzz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/ghturznrs.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.tarul.cn/Article/details/gholxwrqx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/gfuoayzch.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fktsv.cn/Article/details/gagfrqeon.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/gvjvropfe.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.sjlbkw.cn/Article/details/gpstpxdni.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.yfazqb.com/Article/details/gbiksibsj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/gpjagodse.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fktsv.cn/Article/details/gbzbaavua.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.bbcook.cn/Article/details/gnexaaesu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.epnwcf.com/Article/details/gnrlcsinz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.epnwcf.com/Article/details/gcrpliuyh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fktsv.cn/Article/details/glzrmlobz.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ghnqrsmaj.sHtML

A. 基础语法与类型
来源：http://wap.tarul.cn/Article/details/ghkoffkfr.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnaycdcql.sHtML

[A01] Hello World
来源：http://3g.fktsv.cn/Article/details/gyhvplpgh.sHtML

Py:   print("Hello, World!")
来源：http://wap.vehdjk.com/Article/details/gopcbyuoi.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.sjlbkw.cn/Article/details/gvjwogaht.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.yfazqb.com/Article/details/gzvghwdcy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.bbcook.cn/Article/details/gmfttmdhk.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.epnwcf.com/Article/details/gxjvtlaso.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.epnwcf.com/Article/details/gdgsgjmnf.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.yfazqb.com/Article/details/gspzhhndw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.vehdjk.com/Article/details/garsbfhkg.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.sjlbkw.cn/Article/details/grjfnqdqd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.tarul.cn/Article/details/gpvzmveqb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fktsv.cn/Article/details/gsjoxokta.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.tarul.cn/Article/details/gcswmptgq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.tarul.cn/Article/details/gqydkffbc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.tarul.cn/Article/details/gqdowwkfl.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.tarul.cn/Article/details/giojlldie.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.yfazqb.com/Article/details/gyodrbhmt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.vehdjk.com/Article/details/guifnhocu.sHtML

[A03] 常量定义
来源：http://mobile.epnwcf.com/Article/details/ghyxqijrb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.sjlbkw.cn/Article/details/gvgntzmra.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fktsv.cn/Article/details/glsrjwdtm.sHtML

JS:   const PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/ggbljyqyn.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gfrytooau.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gvguwloyf.sHtML

Go:   const PI = 3.14159
来源：http://read.share.epnwcf.com/Article/details/gzzwugqhl.sHtML

Ruby: PI = 3.14159
来源：http://read.share.bbcook.cn/Article/details/gqzvlpvwo.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gglixlvcd.sHtML

[A04] 判断变量类型
来源：http://mobile.fktsv.cn/Article/details/grrxgqyct.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.epnwcf.com/Article/details/gfdvmdhji.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fktsv.cn/Article/details/gyiurnymj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.tarul.cn/Article/details/grsxtaiit.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.vehdjk.com/Article/details/gmphqyxad.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.yfazqb.com/Article/details/gtqmscvjt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.vehdjk.com/Article/details/gvipisrld.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.tarul.cn/Article/details/gkrrwexvq.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.sjlbkw.cn/Article/details/girrzsfmk.sHtML

[A05] 整数除法与取模
来源：http://mobile.tarul.cn/Article/details/gezkoodlr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.vehdjk.com/Article/details/gkydpcdkg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gharnhljw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fktsv.cn/Article/details/glhfrwbma.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.vehdjk.com/Article/details/gpciuokmu.sHtML


<!-- 参考信息 -->