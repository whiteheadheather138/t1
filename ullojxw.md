代发 wailian999

[U47] PHP：联合类型
来源：http://mobile.sjlbkw.cn/Article/details/gxzjxtxmy.sHtML

int|string $id
来源：http://blog.vehdjk.com/Article/details/gdzuogwaf.sHtML

[U48] PHP：纯枚举
来源：http://www.share.tarul.cn/Article/details/gvhsgacvu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.vehdjk.com/Article/details/gfzffqkpb.sHtML

[U49] PHP：只读属性
来源：http://3g.bbcook.cn/Article/details/gvvuzmlpr.sHtML

public readonly string $name
来源：http://3g.yfazqb.com/Article/details/gfolehybd.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.sjlbkw.cn/Article/details/gnsimddzr.sHtML

public function __construct(private int $id) {}
来源：http://blog.fktsv.cn/Article/details/gkoglmzpz.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fktsv.cn/Article/details/glnhjwarl.sHtML

[$a, $b] = $arr;
来源：http://wap.epnwcf.com/Article/details/gmtgpjwrz.sHtML

[U52] PHP：箭头函数
来源：http://www.share.bbcook.cn/Article/details/gwgidnmki.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.sjlbkw.cn/Article/details/ghmpvfzwc.sHtML

[U53] PHP：空合并运算符
来源：http://baike.vehdjk.com/Article/details/grauwptbx.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.sjlbkw.cn/Article/details/gubonhjgu.sHtML

[U54] PHP：空安全调用
来源：http://www.share.vehdjk.com/Article/details/gyykorcdr.sHtML

$obj?->method()
来源：http://blog.yfazqb.com/Article/details/gcfgmxnqn.sHtML

[U55] PHP：match 表达式
来源：http://mobile.tarul.cn/Article/details/grcizxkat.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.sjlbkw.cn/Article/details/geoyzvtoq.sHtML

[U56] PHP：命名参数
来源：http://baike.vehdjk.com/Article/details/gmbzgdlbd.sHtML

f(a: 1, b: 2)
来源：http://blog.tarul.cn/Article/details/ggutcosno.sHtML

[U57] PHP：字符串插值
来源：http://3g.vehdjk.com/Article/details/gpoqewfqt.sHtML

"值: {$a}"
来源：http://m.share.vehdjk.com/Article/details/gzyppnnks.sHtML

[U58] PHP：数组三件套
来源：http://blog.fktsv.cn/Article/details/gbkwkawjf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.yfazqb.com/Article/details/geqsuuiej.sHtML

[U59] PHP：自定义排序
来源：http://mobile.yfazqb.com/Article/details/gwwqadxsm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.epnwcf.com/Article/details/gqysadtfs.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.yfazqb.com/Article/details/gpwxawhio.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.epnwcf.com/Article/details/gvutwylas.sHtML

[U61] PHP：正则
来源：http://blog.yfazqb.com/Article/details/gmpmbjuvq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gwyzkrdvy.sHtML

[U62] PHP：日期对象
来源：http://www.blog.tarul.cn/Article/details/gdznxindf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.tarul.cn/Article/details/gwemqgigz.sHtML

[U63] PHP：文件读写
来源：http://read.share.tarul.cn/Article/details/ghshlrzqm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.bbcook.cn/Article/details/grgaemoup.sHtML

[U64] PHP：目录遍历
来源：http://3g.yfazqb.com/Article/details/gpphajabi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.sjlbkw.cn/Article/details/ggcclqxeq.sHtML

[U65] PHP：会话
来源：http://wap.bbcook.cn/Article/details/gorllxihb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.tarul.cn/Article/details/gerebfrmc.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.epnwcf.com/Article/details/grxlifbcr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.sjlbkw.cn/Article/details/gdskniiev.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fktsv.cn/Article/details/gbylsgurn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fktsv.cn/Article/details/gptimoyni.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fktsv.cn/Article/details/gvgndmkyu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.yfazqb.com/Article/details/ggmsskgdq.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fktsv.cn/Article/details/gswrmtwio.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.bbcook.cn/Article/details/gpqafebjf.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.sjlbkw.cn/Article/details/gocdghfls.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.tarul.cn/Article/details/gseuwdamt.sHtML

[U71] PHP：抛出异常
来源：http://mobile.epnwcf.com/Article/details/gusiqzyww.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.bbcook.cn/Article/details/ggycyptdn.sHtML

[U72] PHP：写错误日志
来源：http://wap.sjlbkw.cn/Article/details/gealdaqma.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.bbcook.cn/Article/details/gmavvcpbu.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.vehdjk.com/Article/details/gricuwpao.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.sjlbkw.cn/Article/details/gezochkni.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.tarul.cn/Article/details/gftidiell.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.tarul.cn/Article/details/gfpunyfmk.sHtML

[U75] PHP：依赖注入
来源：http://mobile.epnwcf.com/Article/details/gyfjboqoi.sHtML

composer require psr/container
来源：http://www.share.epnwcf.com/Article/details/gsplxxxth.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.vehdjk.com/Article/details/gsmhgfkri.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.yfazqb.com/Article/details/gkevoqphf.sHtML

[U77] PHP：模板渲染
来源：http://m.share.bbcook.cn/Article/details/gsqxxebbg.sHtML

composer require twig/twig
来源：http://blog.tarul.cn/Article/details/gkhmbnlea.sHtML

[U78] PHP：单元测试
来源：http://blog.bbcook.cn/Article/details/gqmqeeokh.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.yfazqb.com/Article/details/gfuedvgyt.sHtML

[U79] PHP：静态分析
来源：http://m.share.bbcook.cn/Article/details/gilztdqvn.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.yfazqb.com/Article/details/genqkupoi.sHtML

[U80] PHP：代码规范修复
来源：http://wap.yfazqb.com/Article/details/gytyqhtsk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.bbcook.cn/Article/details/guxqeczyu.sHtML

[U81] JS：初始化项目
来源：http://blog.bbcook.cn/Article/details/ghrxlqvgv.sHtML

npm init -y;  npm i express
来源：http://www.m.share.yfazqb.com/Article/details/gingskkqn.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.sjlbkw.cn/Article/details/gyoeozsxc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.bbcook.cn/Article/details/glzaavfkl.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.vehdjk.com/Article/details/grvbbxkxh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.tarul.cn/Article/details/garqotvmm.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.vehdjk.com/Article/details/guoajokzv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.bbcook.cn/Article/details/gxfaortoi.sHtML

[U85] JS：可选链
来源：http://wap.bbcook.cn/Article/details/gbdjvlsjl.sHtML

a?.b?.c
来源：http://www.share.vehdjk.com/Article/details/gihcgcskk.sHtML

[U86] JS：空值合并
来源：http://wap.fktsv.cn/Article/details/gjmyyarzx.sHtML

a ?? b
来源：http://www.blog.tarul.cn/Article/details/ghutkgrpq.sHtML

[U87] JS：解构默认值
来源：http://m.share.vehdjk.com/Article/details/ggvryxdfm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.sjlbkw.cn/Article/details/gmwaufwbj.sHtML

[U88] JS：对象展开合并
来源：http://baike.bbcook.cn/Article/details/givoqrgsl.sHtML

{ ...a, ...b }
来源：http://blog.bbcook.cn/Article/details/gehmerzvu.sHtML

[U89] JS：数组去重
来源：http://3g.fktsv.cn/Article/details/grsjkiugr.sHtML

[...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/geowqtmue.sHtML

[U90] JS：数字数组排序
来源：http://blog.bbcook.cn/Article/details/guxdmsmqb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/gloqngori.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fktsv.cn/Article/details/gllmbdqwv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.tarul.cn/Article/details/govdogkce.sHtML

[U92] JS：深拷贝
来源：http://3g.tarul.cn/Article/details/gmkicrrdb.sHtML

structuredClone(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gupzpmmoq.sHtML

[U93] JS：模板字符串
来源：http://read.share.epnwcf.com/Article/details/ghnifawuy.sHtML

`共 ${n} 条`
来源：http://wap.yfazqb.com/Article/details/ghyvbjjpp.sHtML

[U94] JS：箭头函数
来源：http://blog.epnwcf.com/Article/details/gqssqcojt.sHtML

const double = x => x * 2;
来源：http://www.share.sjlbkw.cn/Article/details/grfjmwoia.sHtML

[U95] JS：Promise 包装
来源：http://read.share.sjlbkw.cn/Article/details/gbkkoruje.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.bbcook.cn/Article/details/gahymopgh.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.yfazqb.com/Article/details/gjefwbpzt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjshqksjr.sHtML

[U97] JS：并发请求
来源：http://m.share.sjlbkw.cn/Article/details/gzjjmqkkg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/getmusaec.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.tarul.cn/Article/details/gqparougb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.yfazqb.com/Article/details/gvvnjbfmh.sHtML

[U99] JS：事件监听
来源：http://3g.yfazqb.com/Article/details/grzjmovha.sHtML

el.addEventListener("click", e => {})
来源：http://blog.vehdjk.com/Article/details/gynopcdxs.sHtML

[U100] JS：DOM 查询
来源：http://3g.epnwcf.com/Article/details/gxarijpzt.sHtML

document.querySelector(".item")
来源：http://mobile.vehdjk.com/Article/details/gyvneeiaw.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gblrabhwe.sHtML

el.classList.toggle("active")
来源：http://read.share.fktsv.cn/Article/details/glzjhoeag.sHtML

[U102] JS：本地存储
来源：http://www.share.epnwcf.com/Article/details/gcgrofyaz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.epnwcf.com/Article/details/gxxpxzjaq.sHtML

[U103] JS：定时器
来源：http://baike.tarul.cn/Article/details/gcyiqaxnw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fktsv.cn/Article/details/grzfgljoh.sHtML

[U104] JS：防抖
来源：http://www.blog.vehdjk.com/Article/details/ghvtvkybx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gdnwolryo.sHtML

[U105] JS：节流
来源：http://blog.yfazqb.com/Article/details/gbthyjuwy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.tarul.cn/Article/details/ghomhfzjn.sHtML

[U106] JS：日期格式化
来源：http://mobile.fktsv.cn/Article/details/ggocukncm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.bbcook.cn/Article/details/gboezuval.sHtML

[U107] JS：数字千分位
来源：http://wap.sjlbkw.cn/Article/details/gwrryfllj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.sjlbkw.cn/Article/details/ggurulvlf.sHtML

[U108] JS：随机整数
来源：http://www.blog.epnwcf.com/Article/details/gmcbazqzr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.vehdjk.com/Article/details/gxubglruc.sHtML

[U109] JS：数组分组
来源：http://read.share.yfazqb.com/Article/details/goasmgfkd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.sjlbkw.cn/Article/details/gazhkwmjc.sHtML

[U110] JS：数组分块
来源：http://www.blog.sjlbkw.cn/Article/details/grftiixfl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.epnwcf.com/Article/details/gitzsfmua.sHtML

[U111] JS：对象转 Map
来源：http://3g.fktsv.cn/Article/details/geouactfe.sHtML

new Map(Object.entries(obj))
来源：http://3g.bbcook.cn/Article/details/gbjnwvnke.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fktsv.cn/Article/details/gmloucurn.sHtML

"7".padStart(3, "0")
来源：http://blog.vehdjk.com/Article/details/grjscimva.sHtML

[U113] JS：正则替换全部
来源：http://m.share.epnwcf.com/Article/details/gxutqhkye.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gejdacnbi.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fktsv.cn/Article/details/gycduubeg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.yfazqb.com/Article/details/geeokynsf.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxrrcmcs.sHtML

crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/gtdzuarwd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.vehdjk.com/Article/details/gmntxheec.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.epnwcf.com/Article/details/gzianhjwu.sHtML

[U117] JS：单元测试
来源：http://m.share.sjlbkw.cn/Article/details/ggwebwemz.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.tarul.cn/Article/details/gcslnvepj.sHtML

[U118] JS：开发服务器
来源：http://3g.bbcook.cn/Article/details/gmpwjkqvu.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fktsv.cn/Article/details/gtqqqnkpk.sHtML

[U119] JS：生产构建
来源：http://baike.epnwcf.com/Article/details/gxjgzhmqt.sHtML

npx vite build
来源：http://mobile.vehdjk.com/Article/details/gjisvouvy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fktsv.cn/Article/details/gzifmqnpx.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.vehdjk.com/Article/details/gzejgugbj.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gcqsuapaw.sHtML

统计汇总
来源：http://www.share.tarul.cn/Article/details/gxhrsswbs.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gexnvqzsh.sHtML

按语言统计（条）：
来源：http://3g.sjlbkw.cn/Article/details/guwvartmc.sHtML

Python ......... 252
来源：http://3g.fktsv.cn/Article/details/gkxrtlmbu.sHtML

PHP ............ 252
来源：http://wap.sjlbkw.cn/Article/details/gdxtgjwnd.sHtML

JavaScript ..... 252
来源：http://wap.yfazqb.com/Article/details/gdulxdyzj.sHtML

TypeScript ..... 212
来源：http://www.blog.epnwcf.com/Article/details/gfjlbmmjw.sHtML

Java ........... 212
来源：http://3g.tarul.cn/Article/details/gywoqjiqi.sHtML

Go ............. 212
来源：http://m.share.sjlbkw.cn/Article/details/gfihsjbrr.sHtML

Ruby ........... 212
来源：http://3g.sjlbkw.cn/Article/details/gmunrctqy.sHtML

C# ............. 212
来源：http://www.blog.sjlbkw.cn/Article/details/gaqlosldg.sHtML

C .............. 30
来源：http://www.m.share.tarul.cn/Article/details/gamyvjgcq.sHtML

C++ ............ 30
来源：http://www.m.share.yfazqb.com/Article/details/gjtnukjzf.sHtML

SQL ............ 90
来源：http://m.share.epnwcf.com/Article/details/gdygaqbhp.sHtML

Bash ........... 80
来源：http://3g.yfazqb.com/Article/details/gvaezqpfd.sHtML

Kotlin ......... 15
来源：http://www.m.share.vehdjk.com/Article/details/gziyyzoim.sHtML

Swift .......... 15
来源：http://www.blog.tarul.cn/Article/details/guvvrycro.sHtML

Lua ............ 10
来源：http://www.share.bbcook.cn/Article/details/gcqfsogaj.sHtML

Perl ........... 10
来源：http://www.blog.tarul.cn/Article/details/gsmlvsjgz.sHtML

Scala .......... 10
来源：http://read.share.sjlbkw.cn/Article/details/gcvjywhgd.sHtML

------------------------------------
来源：http://wap.vehdjk.com/Article/details/grysuakhd.sHtML

合计 ........... 2106 条
来源：http://www.share.yfazqb.com/Article/details/gmnluxjsb.sHtML

按章节统计：
来源：http://www.blog.tarul.cn/Article/details/gfwemabsj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.bbcook.cn/Article/details/gyrfdzvnl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fktsv.cn/Article/details/gsburhoas.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.epnwcf.com/Article/details/gjqrmjhdh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.sjlbkw.cn/Article/details/gmyushryr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.epnwcf.com/Article/details/gtexgaxdl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.yfazqb.com/Article/details/groeippbm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fktsv.cn/Article/details/ggvlegqtk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.vehdjk.com/Article/details/gjyejfoge.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/glpxwlnkm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.epnwcf.com/Article/details/gwuuigoaz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.tarul.cn/Article/details/grarzluru.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/glavgotzc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/gevxnqpjs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fktsv.cn/Article/details/gwppoivxx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.epnwcf.com/Article/details/gmlaaajap.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/gxrxyphtv.sHtML

Q SQL 专题                              90
来源：http://3g.epnwcf.com/Article/details/gymdrkyig.sHtML

R Bash 专题                             80
来源：http://blog.bbcook.cn/Article/details/gavzvhhrb.sHtML

S C / C++ 专题                          60
来源：http://www.blog.bbcook.cn/Article/details/gljnsnfrt.sHtML

T 其他语言补充                          60
来源：http://3g.tarul.cn/Article/details/gqccpnxat.sHtML

U 高频实用片段                         120
来源：http://wap.fktsv.cn/Article/details/gdslmlpus.sHtML

------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gnukkeejz.sHtML

合计                                  2106 条
来源：http://mobile.yfazqb.com/Article/details/gjfbscshx.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gdiyvkcmh.sHtML

使用提醒
来源：http://blog.bbcook.cn/Article/details/gtuyfzisu.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.vehdjk.com/Article/details/gwxyinxsv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.tarul.cn/Article/details/gxcftnmxh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.vehdjk.com/Article/details/grskpfktf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.epnwcf.com/Article/details/grnlqseyz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fktsv.cn/Article/details/gecuaefov.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.vehdjk.com/Article/details/gfqqdrkuv.sHtML

—— 文件结束 ——
来源：http://m.share.fktsv.cn/Article/details/gfwbpuxkz.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gobbvmyri.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.bbcook.cn/Article/details/gnjwgcxqv.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.bbcook.cn/Article/details/geyjbizfe.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gpcequcru.sHtML

【收录内容】
来源：http://m.share.vehdjk.com/Article/details/gtltpvmfm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.bbcook.cn/Article/details/ggrblpgpa.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.sjlbkw.cn/Article/details/gcjdxvqqq.sHtML

SQL · Bash · C · C++
来源：http://m.share.tarul.cn/Article/details/gxhmultcr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.bbcook.cn/Article/details/gedraxork.sHtML

【使用说明】
来源：http://read.share.yfazqb.com/Article/details/gilymabhn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.yfazqb.com/Article/details/gklqfgkoo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.sjlbkw.cn/Article/details/gcayosmlt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.vehdjk.com/Article/details/guryrlqgd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.vehdjk.com/Article/details/geejcconf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.bbcook.cn/Article/details/gapfsejrr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.tarul.cn/Article/details/gnssfxdtb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.tarul.cn/Article/details/gmphrgzpc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.tarul.cn/Article/details/gzjivmzcr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.bbcook.cn/Article/details/gwjatndyq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.tarul.cn/Article/details/glbdaquud.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.bbcook.cn/Article/details/gshufdzuq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.yfazqb.com/Article/details/gmqytknkk.sHtML

【文件统计】
来源：http://www.m.share.epnwcf.com/Article/details/glqzopslo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.sjlbkw.cn/Article/details/gatrxhejw.sHtML

--------------------------------------------------------------------------------
来源：http://wap.yfazqb.com/Article/details/gaeyoryce.sHtML

目  录
来源：http://baike.bbcook.cn/Article/details/gjhfpxgys.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/gmtltadci.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.bbcook.cn/Article/details/gudddhhxa.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.tarul.cn/Article/details/gctuftcpc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.vehdjk.com/Article/details/gbussictl.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.tarul.cn/Article/details/gogfbqjwr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.epnwcf.com/Article/details/ggtezgxmf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fktsv.cn/Article/details/gnwuyiczf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fktsv.cn/Article/details/gzhsxjuun.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.sjlbkw.cn/Article/details/gaeonuhey.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/gbyzleugd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.epnwcf.com/Article/details/gufkdxtyk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/gsoeradlm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.vehdjk.com/Article/details/gexlkvllo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fktsv.cn/Article/details/gfdthwqyr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.vehdjk.com/Article/details/ggrviyitk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.yfazqb.com/Article/details/gqakoruom.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/gothgtaav.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.bbcook.cn/Article/details/gvgdxnxfk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.vehdjk.com/Article/details/glradyexe.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.yfazqb.com/Article/details/gwesswurw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.sjlbkw.cn/Article/details/gsyuvybes.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.epnwcf.com/Article/details/gkpqnvomj.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gfnwibfnp.sHtML

A. 基础语法与类型
来源：http://wap.epnwcf.com/Article/details/genieqypz.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ghzhccwny.sHtML

[A01] Hello World
来源：http://m.share.vehdjk.com/Article/details/gifsveyhp.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.sjlbkw.cn/Article/details/gffhvejel.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.vehdjk.com/Article/details/gipkrsjcu.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fktsv.cn/Article/details/gntdctxtn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.sjlbkw.cn/Article/details/ggxvspndl.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.vehdjk.com/Article/details/gmysxxkhi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.vehdjk.com/Article/details/gpupwlxrj.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.vehdjk.com/Article/details/gejlptisk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.bbcook.cn/Article/details/glxracdwr.sHtML

[A02] 变量声明与赋值
来源：http://mobile.bbcook.cn/Article/details/gnhnwjwdo.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.epnwcf.com/Article/details/gfptsfwme.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.tarul.cn/Article/details/gubfitsmh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.bbcook.cn/Article/details/gdmuuzavv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.yfazqb.com/Article/details/ggwjwcvra.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.sjlbkw.cn/Article/details/goteperzh.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.tarul.cn/Article/details/gmwmnaavx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.epnwcf.com/Article/details/giqcryfqs.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/ghafycily.sHtML

[A03] 常量定义
来源：http://3g.yfazqb.com/Article/details/gbpjrocmx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.tarul.cn/Article/details/ghiisfktk.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gdaqsstku.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gvofkjjho.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gqzenpeyy.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gugmkhqgj.sHtML

Go:   const PI = 3.14159
来源：http://wap.epnwcf.com/Article/details/gyjltgpgn.sHtML

Ruby: PI = 3.14159
来源：http://wap.yfazqb.com/Article/details/gdayupnxg.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/gmnoxxmsp.sHtML

[A04] 判断变量类型
来源：http://www.share.bbcook.cn/Article/details/gbpmjtfnd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.bbcook.cn/Article/details/gtuupkgwo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.sjlbkw.cn/Article/details/galjqtsfm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.bbcook.cn/Article/details/gyyyupyul.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.tarul.cn/Article/details/gzjnzgkpm.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.vehdjk.com/Article/details/gurosxucy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.epnwcf.com/Article/details/gufcoxuie.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.sjlbkw.cn/Article/details/gnlvxshop.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.epnwcf.com/Article/details/ggdtgblkc.sHtML

[A05] 整数除法与取模
来源：http://read.share.sjlbkw.cn/Article/details/gmigorhrx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.vehdjk.com/Article/details/gxrjlwtes.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gghodgomq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.vehdjk.com/Article/details/geacuijvk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.bbcook.cn/Article/details/godsofozp.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.vehdjk.com/Article/details/gqubnzdfg.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.vehdjk.com/Article/details/grodaskyq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.bbcook.cn/Article/details/ghqhzvusp.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gxmaluztb.sHtML


<!-- 参考信息 -->