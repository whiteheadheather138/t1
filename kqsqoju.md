代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://baike.vehdjk.com/Article/details/gnkkjmcoz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gossgovru.sHtML

[U46] PHP：可空类型
来源：http://3g.epnwcf.com/Article/details/gfflafsad.sHtML

?string $name = null
来源：http://3g.epnwcf.com/Article/details/glicetdih.sHtML

[U47] PHP：联合类型
来源：http://www.blog.epnwcf.com/Article/details/gwkidocxu.sHtML

int|string $id
来源：http://baike.tarul.cn/Article/details/gesgkqqqx.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.epnwcf.com/Article/details/gguzoeptf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.yfazqb.com/Article/details/gqdplejge.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.epnwcf.com/Article/details/gjximolix.sHtML

public readonly string $name
来源：http://www.m.share.epnwcf.com/Article/details/gbjmdwrdy.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.sjlbkw.cn/Article/details/gzdmggbyl.sHtML

public function __construct(private int $id) {}
来源：http://m.share.yfazqb.com/Article/details/ghfyktyvi.sHtML

[U51] PHP：数组解构
来源：http://blog.fktsv.cn/Article/details/gnrqzfhmn.sHtML

[$a, $b] = $arr;
来源：http://read.share.epnwcf.com/Article/details/gdugmcxhi.sHtML

[U52] PHP：箭头函数
来源：http://blog.vehdjk.com/Article/details/giumfntfm.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.tarul.cn/Article/details/gonqvtlop.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.epnwcf.com/Article/details/gkqrvddjz.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.bbcook.cn/Article/details/gieklnwpe.sHtML

[U54] PHP：空安全调用
来源：http://m.share.tarul.cn/Article/details/glkmdfvoz.sHtML

$obj?->method()
来源：http://www.share.fktsv.cn/Article/details/gejhegebz.sHtML

[U55] PHP：match 表达式
来源：http://baike.sjlbkw.cn/Article/details/glteosgxw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.yfazqb.com/Article/details/gcmukwogu.sHtML

[U56] PHP：命名参数
来源：http://blog.yfazqb.com/Article/details/gqdujmmmz.sHtML

f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gkkfnersg.sHtML

[U57] PHP：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gpyrpzozs.sHtML

"值: {$a}"
来源：http://baike.yfazqb.com/Article/details/ghhjgjpnx.sHtML

[U58] PHP：数组三件套
来源：http://wap.bbcook.cn/Article/details/gycdzvjmx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.tarul.cn/Article/details/gikbkeypz.sHtML

[U59] PHP：自定义排序
来源：http://3g.yfazqb.com/Article/details/gejidspwa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.vehdjk.com/Article/details/glejuretz.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.epnwcf.com/Article/details/gmcdkaxic.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.sjlbkw.cn/Article/details/gipryrqow.sHtML

[U61] PHP：正则
来源：http://www.m.share.yfazqb.com/Article/details/gglawehua.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gxxkxxoww.sHtML

[U62] PHP：日期对象
来源：http://mobile.epnwcf.com/Article/details/gouymkcwd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.bbcook.cn/Article/details/gbwgazcol.sHtML

[U63] PHP：文件读写
来源：http://m.share.tarul.cn/Article/details/gdpopbfnz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.epnwcf.com/Article/details/gpxewhiwk.sHtML

[U64] PHP：目录遍历
来源：http://baike.sjlbkw.cn/Article/details/goihqnqdo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.epnwcf.com/Article/details/gphfzvuaq.sHtML

[U65] PHP：会话
来源：http://mobile.vehdjk.com/Article/details/gadastvvg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.bbcook.cn/Article/details/gmgdmusdf.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.yfazqb.com/Article/details/gdhjizkgg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.tarul.cn/Article/details/gackrvbpd.sHtML

[U67] PHP：处理文件上传
来源：http://wap.vehdjk.com/Article/details/gfhxpmvzj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.vehdjk.com/Article/details/gbsimuzay.sHtML

[U68] PHP：PDO 连接
来源：http://blog.sjlbkw.cn/Article/details/gnsovenut.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.yfazqb.com/Article/details/gfedhxusw.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.epnwcf.com/Article/details/gmgcnpdbr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.vehdjk.com/Article/details/gjfjzydwr.sHtML

[U70] PHP：PDO 事务
来源：http://blog.epnwcf.com/Article/details/gqtbmnnph.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.sjlbkw.cn/Article/details/gnhlaoxxv.sHtML

[U71] PHP：抛出异常
来源：http://www.share.sjlbkw.cn/Article/details/gnwlgamun.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.bbcook.cn/Article/details/gchypxgzh.sHtML

[U72] PHP：写错误日志
来源：http://blog.vehdjk.com/Article/details/giaerscun.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.bbcook.cn/Article/details/gmeojrcxt.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.sjlbkw.cn/Article/details/gmfirvwbu.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.tarul.cn/Article/details/gcdvtyklk.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.vehdjk.com/Article/details/gbmdlqcua.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.vehdjk.com/Article/details/gucoowklr.sHtML

[U75] PHP：依赖注入
来源：http://3g.bbcook.cn/Article/details/gasbhkqcx.sHtML

composer require psr/container
来源：http://mobile.bbcook.cn/Article/details/gzcjotjsv.sHtML

[U76] PHP：简单路由
来源：http://www.blog.tarul.cn/Article/details/ggxpeosrv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.bbcook.cn/Article/details/gjfohbyna.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.yfazqb.com/Article/details/gjuhoviim.sHtML

composer require twig/twig
来源：http://www.m.share.bbcook.cn/Article/details/gidsiekch.sHtML

[U78] PHP：单元测试
来源：http://mobile.bbcook.cn/Article/details/gsbnjasod.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.sjlbkw.cn/Article/details/gjbuvnhrg.sHtML

[U79] PHP：静态分析
来源：http://baike.tarul.cn/Article/details/gljugkaxb.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.epnwcf.com/Article/details/giaonshap.sHtML

[U80] PHP：代码规范修复
来源：http://blog.sjlbkw.cn/Article/details/gxpbyjoks.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.bbcook.cn/Article/details/gshnburxi.sHtML

[U81] JS：初始化项目
来源：http://read.share.epnwcf.com/Article/details/ghdxoslvw.sHtML

npm init -y;  npm i express
来源：http://www.blog.fktsv.cn/Article/details/gwkwkmqmu.sHtML

[U82] JS：package.json 脚本
来源：http://3g.sjlbkw.cn/Article/details/gumzhmxzn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.tarul.cn/Article/details/ggidahfeo.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.sjlbkw.cn/Article/details/gvamujfpe.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.sjlbkw.cn/Article/details/glenrvpta.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.yfazqb.com/Article/details/glfwdzslz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.bbcook.cn/Article/details/gaytzwvhj.sHtML

[U85] JS：可选链
来源：http://wap.epnwcf.com/Article/details/gllnuqodp.sHtML

a?.b?.c
来源：http://read.share.bbcook.cn/Article/details/gjwyhdmvf.sHtML

[U86] JS：空值合并
来源：http://www.share.vehdjk.com/Article/details/gbgvtkgdu.sHtML

a ?? b
来源：http://www.share.bbcook.cn/Article/details/gkhkuahts.sHtML

[U87] JS：解构默认值
来源：http://read.share.bbcook.cn/Article/details/gnlqormgd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fktsv.cn/Article/details/gfijfmdqy.sHtML

[U88] JS：对象展开合并
来源：http://mobile.sjlbkw.cn/Article/details/gkkwgguar.sHtML

{ ...a, ...b }
来源：http://read.share.fktsv.cn/Article/details/ghrbhdrrl.sHtML

[U89] JS：数组去重
来源：http://read.share.vehdjk.com/Article/details/gwdgtzpck.sHtML

[...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/guyuhhzaa.sHtML

[U90] JS：数字数组排序
来源：http://baike.tarul.cn/Article/details/grochprkr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gsxbbmdtl.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.epnwcf.com/Article/details/gvxoublbn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.sjlbkw.cn/Article/details/gjsoiezon.sHtML

[U92] JS：深拷贝
来源：http://m.share.tarul.cn/Article/details/godpqljtw.sHtML

structuredClone(obj)
来源：http://blog.vehdjk.com/Article/details/ghuystxuy.sHtML

[U93] JS：模板字符串
来源：http://read.share.bbcook.cn/Article/details/gcgbyptcg.sHtML

`共 ${n} 条`
来源：http://mobile.bbcook.cn/Article/details/guqnsydku.sHtML

[U94] JS：箭头函数
来源：http://www.share.epnwcf.com/Article/details/gkifrkgbe.sHtML

const double = x => x * 2;
来源：http://mobile.fktsv.cn/Article/details/gbcaiedre.sHtML

[U95] JS：Promise 包装
来源：http://baike.fktsv.cn/Article/details/gffbbqdih.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fktsv.cn/Article/details/goeixrfff.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fktsv.cn/Article/details/gfqeuxkfb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/gaempwlea.sHtML

[U97] JS：并发请求
来源：http://www.share.bbcook.cn/Article/details/gxabkyzed.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gyyfkzpvc.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.yfazqb.com/Article/details/gszxgkjms.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.bbcook.cn/Article/details/gwpgwlstx.sHtML

[U99] JS：事件监听
来源：http://baike.epnwcf.com/Article/details/glhclkvif.sHtML

el.addEventListener("click", e => {})
来源：http://3g.sjlbkw.cn/Article/details/gdghfesad.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.yfazqb.com/Article/details/goqnjglyw.sHtML

document.querySelector(".item")
来源：http://baike.epnwcf.com/Article/details/ghkxfcbir.sHtML

[U101] JS：classList 操作
来源：http://wap.bbcook.cn/Article/details/gpdbedyls.sHtML

el.classList.toggle("active")
来源：http://blog.tarul.cn/Article/details/gyyfzmwze.sHtML

[U102] JS：本地存储
来源：http://blog.epnwcf.com/Article/details/gntzcuwbh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fktsv.cn/Article/details/gugaxzhnz.sHtML

[U103] JS：定时器
来源：http://mobile.vehdjk.com/Article/details/gegcmubaz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fktsv.cn/Article/details/gnbxskucd.sHtML

[U104] JS：防抖
来源：http://3g.epnwcf.com/Article/details/glhtdzmcv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/gqixiqwtv.sHtML

[U105] JS：节流
来源：http://baike.epnwcf.com/Article/details/gcatktrdv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fktsv.cn/Article/details/guiaztkwl.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gakpakqce.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fktsv.cn/Article/details/gqrnfwebm.sHtML

[U107] JS：数字千分位
来源：http://www.blog.tarul.cn/Article/details/gbvzhziom.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.yfazqb.com/Article/details/gfpphzgzx.sHtML

[U108] JS：随机整数
来源：http://read.share.fktsv.cn/Article/details/gmbskuaze.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.vehdjk.com/Article/details/gwgbngnyd.sHtML

[U109] JS：数组分组
来源：http://mobile.bbcook.cn/Article/details/gxwjwijbz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.epnwcf.com/Article/details/gziqfddll.sHtML

[U110] JS：数组分块
来源：http://www.blog.bbcook.cn/Article/details/gilkdeorc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.tarul.cn/Article/details/gjiujykkn.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.bbcook.cn/Article/details/gfyyavfvc.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.bbcook.cn/Article/details/glwhxslko.sHtML

[U112] JS：字符串补位
来源：http://read.share.fktsv.cn/Article/details/gcajdiunj.sHtML

"7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gbeabdowc.sHtML

[U113] JS：正则替换全部
来源：http://wap.yfazqb.com/Article/details/gqatxvumx.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gkpriocwr.sHtML

[U114] JS：JSON 深比较
来源：http://3g.epnwcf.com/Article/details/gcvvuctun.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fktsv.cn/Article/details/gvhuahcsy.sHtML

[U115] JS：生成 UUID
来源：http://blog.tarul.cn/Article/details/gkecvteaz.sHtML

crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/gatilqlwz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.yfazqb.com/Article/details/gkoazynhd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.bbcook.cn/Article/details/gubhwmwsa.sHtML

[U117] JS：单元测试
来源：http://www.share.epnwcf.com/Article/details/gzjoplqvi.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fktsv.cn/Article/details/gzmjgmlwb.sHtML

[U118] JS：开发服务器
来源：http://www.share.yfazqb.com/Article/details/gjrozyswr.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fktsv.cn/Article/details/gqzfuvbfz.sHtML

[U119] JS：生产构建
来源：http://read.share.bbcook.cn/Article/details/gyxcvmnfm.sHtML

npx vite build
来源：http://baike.tarul.cn/Article/details/gtjacgaqs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.yfazqb.com/Article/details/gekzmxejm.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fktsv.cn/Article/details/gmsfvllqy.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxngewbnp.sHtML

统计汇总
来源：http://baike.sjlbkw.cn/Article/details/ghxlivayq.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gmroqbixk.sHtML

按语言统计（条）：
来源：http://www.blog.epnwcf.com/Article/details/gruibuzyb.sHtML

Python ......... 252
来源：http://read.share.fktsv.cn/Article/details/gbgurdoox.sHtML

PHP ............ 252
来源：http://www.blog.fktsv.cn/Article/details/gtdgfkvol.sHtML

JavaScript ..... 252
来源：http://m.share.tarul.cn/Article/details/gzaigoica.sHtML

TypeScript ..... 212
来源：http://m.share.tarul.cn/Article/details/gqfxaqzwm.sHtML

Java ........... 212
来源：http://blog.bbcook.cn/Article/details/giijvzwbr.sHtML

Go ............. 212
来源：http://www.blog.yfazqb.com/Article/details/gtqppgkqb.sHtML

Ruby ........... 212
来源：http://mobile.yfazqb.com/Article/details/gkvsxfhkz.sHtML

C# ............. 212
来源：http://wap.sjlbkw.cn/Article/details/gcoxiifyq.sHtML

C .............. 30
来源：http://wap.bbcook.cn/Article/details/ganiqncqp.sHtML

C++ ............ 30
来源：http://m.share.sjlbkw.cn/Article/details/gerwcanaa.sHtML

SQL ............ 90
来源：http://blog.yfazqb.com/Article/details/gvbhhfqir.sHtML

Bash ........... 80
来源：http://read.share.yfazqb.com/Article/details/gqdwlkrdw.sHtML

Kotlin ......... 15
来源：http://mobile.bbcook.cn/Article/details/gnawmknak.sHtML

Swift .......... 15
来源：http://read.share.bbcook.cn/Article/details/gjplqdxfe.sHtML

Lua ............ 10
来源：http://www.blog.bbcook.cn/Article/details/gekoidccv.sHtML

Perl ........... 10
来源：http://mobile.vehdjk.com/Article/details/gojcbksys.sHtML

Scala .......... 10
来源：http://www.m.share.bbcook.cn/Article/details/gedgwbuii.sHtML

------------------------------------
来源：http://baike.tarul.cn/Article/details/geacpvscp.sHtML

合计 ........... 2106 条
来源：http://baike.tarul.cn/Article/details/gksjawnqu.sHtML

按章节统计：
来源：http://www.m.share.sjlbkw.cn/Article/details/guxoaqbop.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.epnwcf.com/Article/details/gvdleawan.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/gkpewewng.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.tarul.cn/Article/details/gqlfrqcmh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.yfazqb.com/Article/details/gfgdjjzgq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fktsv.cn/Article/details/gegfssdzf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.tarul.cn/Article/details/gghewexue.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.sjlbkw.cn/Article/details/gnfuixpot.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fktsv.cn/Article/details/ghaaiffgs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/genuyndzc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.vehdjk.com/Article/details/gjbyfheld.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/glvqfqjjk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gomdtkimm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gefakkhpf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.yfazqb.com/Article/details/gpwzkwfnu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.vehdjk.com/Article/details/gbpuxovbj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gemimntck.sHtML

Q SQL 专题                              90
来源：http://3g.fktsv.cn/Article/details/gtcnmpwaf.sHtML

R Bash 专题                             80
来源：http://blog.epnwcf.com/Article/details/gmraggpts.sHtML

S C / C++ 专题                          60
来源：http://3g.sjlbkw.cn/Article/details/ghljfjsab.sHtML

T 其他语言补充                          60
来源：http://baike.tarul.cn/Article/details/gomryvzmd.sHtML

U 高频实用片段                         120
来源：http://www.share.vehdjk.com/Article/details/gvsfcshoo.sHtML

------------------------------------
来源：http://baike.tarul.cn/Article/details/grobjwvai.sHtML

合计                                  2106 条
来源：http://baike.vehdjk.com/Article/details/gtxwywdvc.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gfqfvpkgo.sHtML

使用提醒
来源：http://3g.tarul.cn/Article/details/gbbupdbkq.sHtML

--------------------------------------------------------------------------------
来源：http://blog.yfazqb.com/Article/details/gmncpkefg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.tarul.cn/Article/details/gkwfejlpl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.yfazqb.com/Article/details/gpcwkefxu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.epnwcf.com/Article/details/gucpwhsil.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.tarul.cn/Article/details/gttqzzsia.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.yfazqb.com/Article/details/gyndapmmt.sHtML

—— 文件结束 ——
来源：http://m.share.yfazqb.com/Article/details/gnsikjbkx.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gmrldfdqt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.vehdjk.com/Article/details/gumgkvmwc.sHtML

Common Programming Examples Cheat Book
来源：http://baike.epnwcf.com/Article/details/goqeqcmkp.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gucvydjut.sHtML

【收录内容】
来源：http://www.blog.epnwcf.com/Article/details/guqkhromk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.bbcook.cn/Article/details/gfeeuvqtc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.vehdjk.com/Article/details/gyhilrlos.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.yfazqb.com/Article/details/gcbcilnzt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.tarul.cn/Article/details/gyiwdndvz.sHtML

【使用说明】
来源：http://baike.bbcook.cn/Article/details/gomfprinw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.vehdjk.com/Article/details/gjmeaofze.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.sjlbkw.cn/Article/details/glhgvmnmp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.vehdjk.com/Article/details/gkddapcfz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.epnwcf.com/Article/details/gdvacgfwe.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.epnwcf.com/Article/details/gzjrsfspz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.yfazqb.com/Article/details/gdmacxfwk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.sjlbkw.cn/Article/details/ggngzywbd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fktsv.cn/Article/details/gioknlryg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.tarul.cn/Article/details/ghkdnqnhj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.yfazqb.com/Article/details/gckyagjne.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.sjlbkw.cn/Article/details/gdilvdngg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.sjlbkw.cn/Article/details/gsrxtgrxm.sHtML

【文件统计】
来源：http://3g.tarul.cn/Article/details/gcyyhwquy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fktsv.cn/Article/details/gyqpccrgh.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/guvvarhea.sHtML

目  录
来源：http://m.share.vehdjk.com/Article/details/gwzcljuhm.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gszwbilik.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.tarul.cn/Article/details/gzygxukcx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.yfazqb.com/Article/details/gnyaahxmx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.tarul.cn/Article/details/gdmxnmear.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.sjlbkw.cn/Article/details/gsrjvtedv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.sjlbkw.cn/Article/details/glcstguki.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fktsv.cn/Article/details/grvmthjjx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.sjlbkw.cn/Article/details/gkpqtakfj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.yfazqb.com/Article/details/guhiarbzv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/grkhuiknq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.tarul.cn/Article/details/gntujgxxv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/gffisytli.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gshvnshiv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.yfazqb.com/Article/details/grmmckqsm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.bbcook.cn/Article/details/gximjiaag.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.tarul.cn/Article/details/gvyufzziv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/gfaefhubc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.bbcook.cn/Article/details/gddbnwvig.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.bbcook.cn/Article/details/gdweqnixm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.epnwcf.com/Article/details/gdhdpphec.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.epnwcf.com/Article/details/gouoyzang.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fktsv.cn/Article/details/gatfjeqnw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gsmqozmpl.sHtML

A. 基础语法与类型
来源：http://www.blog.sjlbkw.cn/Article/details/giigdwrli.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxfihqgrs.sHtML

[A01] Hello World
来源：http://m.share.yfazqb.com/Article/details/gmepwdylz.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fktsv.cn/Article/details/ghxmpziqp.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.bbcook.cn/Article/details/gkiwvxlyy.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.sjlbkw.cn/Article/details/gqjfirefe.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.epnwcf.com/Article/details/gyqjovtrb.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.yfazqb.com/Article/details/ghkjicuqf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.vehdjk.com/Article/details/geyhctwhq.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.sjlbkw.cn/Article/details/gmsaanqpt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.yfazqb.com/Article/details/glohuudgy.sHtML

[A02] 变量声明与赋值
来源：http://blog.fktsv.cn/Article/details/gfpdapcsl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fktsv.cn/Article/details/gnavcdduc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.epnwcf.com/Article/details/gsylsoaga.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.yfazqb.com/Article/details/gsmaedtho.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.bbcook.cn/Article/details/gyfnankyr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.tarul.cn/Article/details/gjtgxpqdo.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.sjlbkw.cn/Article/details/gzyffoqxk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.tarul.cn/Article/details/gyoezhsxo.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.sjlbkw.cn/Article/details/gfliqukwl.sHtML

[A03] 常量定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gsckauqli.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlfqbzrg.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gbbyozhxk.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gmlwkffac.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gpejdqbpe.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gkyhzqgza.sHtML

Go:   const PI = 3.14159
来源：http://3g.yfazqb.com/Article/details/geywwbnvy.sHtML

Ruby: PI = 3.14159
来源：http://baike.vehdjk.com/Article/details/gcqakknpx.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gupoesvng.sHtML

[A04] 判断变量类型
来源：http://www.blog.vehdjk.com/Article/details/gyzquwagi.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.yfazqb.com/Article/details/gussxsdce.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fktsv.cn/Article/details/gtybgcvhw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.vehdjk.com/Article/details/gmffikvpo.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fktsv.cn/Article/details/gfefjnrsu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.bbcook.cn/Article/details/gchzaikhj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.tarul.cn/Article/details/gggfbjnmo.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.tarul.cn/Article/details/gwpryappd.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.yfazqb.com/Article/details/gmswvruaj.sHtML

[A05] 整数除法与取模
来源：http://mobile.fktsv.cn/Article/details/glqzxqckw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fktsv.cn/Article/details/gfusoiije.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gdtbjgigs.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/gnxzibyfa.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fktsv.cn/Article/details/ghkfgipxc.sHtML


<!-- 参考信息 -->