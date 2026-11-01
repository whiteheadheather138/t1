代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://mobile.epnwcf.com/Article/details/gokyujbaa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/ghfaccsqu.sHtML

[U46] PHP：可空类型
来源：http://www.blog.tarul.cn/Article/details/gbxjbddsp.sHtML

?string $name = null
来源：http://baike.epnwcf.com/Article/details/gokruoony.sHtML

[U47] PHP：联合类型
来源：http://read.share.vehdjk.com/Article/details/gvrimwlfq.sHtML

int|string $id
来源：http://baike.epnwcf.com/Article/details/ggqagahef.sHtML

[U48] PHP：纯枚举
来源：http://www.share.vehdjk.com/Article/details/glvrtlscc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fktsv.cn/Article/details/ghkjswbxq.sHtML

[U49] PHP：只读属性
来源：http://mobile.tarul.cn/Article/details/gqxqicrwh.sHtML

public readonly string $name
来源：http://wap.yfazqb.com/Article/details/gbssfqbmj.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.epnwcf.com/Article/details/gmpxntjvq.sHtML

public function __construct(private int $id) {}
来源：http://wap.yfazqb.com/Article/details/gqxiekvft.sHtML

[U51] PHP：数组解构
来源：http://blog.epnwcf.com/Article/details/gjuwvpqlx.sHtML

[$a, $b] = $arr;
来源：http://www.share.vehdjk.com/Article/details/gchbmdiaj.sHtML

[U52] PHP：箭头函数
来源：http://wap.sjlbkw.cn/Article/details/giaohkrpy.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.sjlbkw.cn/Article/details/gftvhbwkc.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fktsv.cn/Article/details/ggpcurnhf.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.yfazqb.com/Article/details/glukjrieq.sHtML

[U54] PHP：空安全调用
来源：http://m.share.tarul.cn/Article/details/gfyhsjosu.sHtML

$obj?->method()
来源：http://www.m.share.bbcook.cn/Article/details/gruqsjuev.sHtML

[U55] PHP：match 表达式
来源：http://m.share.vehdjk.com/Article/details/gpsefkstx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.sjlbkw.cn/Article/details/gwjlzbpra.sHtML

[U56] PHP：命名参数
来源：http://3g.sjlbkw.cn/Article/details/gtkzzmqvf.sHtML

f(a: 1, b: 2)
来源：http://m.share.bbcook.cn/Article/details/galktrqhr.sHtML

[U57] PHP：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gncrcdasu.sHtML

"值: {$a}"
来源：http://wap.bbcook.cn/Article/details/gffkanbzc.sHtML

[U58] PHP：数组三件套
来源：http://wap.tarul.cn/Article/details/guayxxvdx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fktsv.cn/Article/details/gzrdwluck.sHtML

[U59] PHP：自定义排序
来源：http://www.share.sjlbkw.cn/Article/details/glixjdlwz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.tarul.cn/Article/details/gvryywhch.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fktsv.cn/Article/details/gvrpjwfjz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.bbcook.cn/Article/details/gwdowanal.sHtML

[U61] PHP：正则
来源：http://mobile.fktsv.cn/Article/details/gvhtdkjsu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.tarul.cn/Article/details/gzobhrqlr.sHtML

[U62] PHP：日期对象
来源：http://baike.bbcook.cn/Article/details/gzpxanhjn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.sjlbkw.cn/Article/details/gyvntzvug.sHtML

[U63] PHP：文件读写
来源：http://3g.sjlbkw.cn/Article/details/gzroycslb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.bbcook.cn/Article/details/gqdpktjuj.sHtML

[U64] PHP：目录遍历
来源：http://wap.bbcook.cn/Article/details/gyvcmgcky.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.tarul.cn/Article/details/gwxfmcmkc.sHtML

[U65] PHP：会话
来源：http://m.share.yfazqb.com/Article/details/gsfbqqxlb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.tarul.cn/Article/details/gpdmufvlr.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.bbcook.cn/Article/details/gvdhimkih.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.vehdjk.com/Article/details/gavbrorls.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.tarul.cn/Article/details/gxjffczst.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.vehdjk.com/Article/details/gzjisdskd.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.bbcook.cn/Article/details/gbwtgtgkv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.yfazqb.com/Article/details/gyajdcyuc.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.bbcook.cn/Article/details/gldiqouft.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.bbcook.cn/Article/details/gbmcfdxra.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.epnwcf.com/Article/details/glgnuoiys.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.vehdjk.com/Article/details/ghijmqmnd.sHtML

[U71] PHP：抛出异常
来源：http://m.share.epnwcf.com/Article/details/gcodmfhwc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.yfazqb.com/Article/details/gybppppri.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fktsv.cn/Article/details/glfvyitrj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.vehdjk.com/Article/details/ghlvpbswe.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.epnwcf.com/Article/details/ggzdydafh.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.sjlbkw.cn/Article/details/gmdalfcqn.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gdllxksje.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.epnwcf.com/Article/details/gzganzdpb.sHtML

[U75] PHP：依赖注入
来源：http://baike.tarul.cn/Article/details/gjevshkxq.sHtML

composer require psr/container
来源：http://mobile.tarul.cn/Article/details/gbllspfhi.sHtML

[U76] PHP：简单路由
来源：http://3g.vehdjk.com/Article/details/guezbdzwe.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.sjlbkw.cn/Article/details/gtonsqjnx.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fktsv.cn/Article/details/gbzxbhyft.sHtML

composer require twig/twig
来源：http://www.share.fktsv.cn/Article/details/gtjyoclmh.sHtML

[U78] PHP：单元测试
来源：http://read.share.epnwcf.com/Article/details/gbdepgvzu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.sjlbkw.cn/Article/details/givrbaada.sHtML

[U79] PHP：静态分析
来源：http://m.share.sjlbkw.cn/Article/details/gygtxxeyx.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fktsv.cn/Article/details/grvkcbyjo.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.vehdjk.com/Article/details/gpzmhbtnh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.yfazqb.com/Article/details/geyftpxuc.sHtML

[U81] JS：初始化项目
来源：http://wap.tarul.cn/Article/details/gberokmss.sHtML

npm init -y;  npm i express
来源：http://3g.yfazqb.com/Article/details/gcywngbvl.sHtML

[U82] JS：package.json 脚本
来源：http://baike.tarul.cn/Article/details/ghpsvwdsb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.bbcook.cn/Article/details/gigjxaqcc.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.tarul.cn/Article/details/gxiofrwrh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.sjlbkw.cn/Article/details/gercsruck.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fktsv.cn/Article/details/gcrmvqoim.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.vehdjk.com/Article/details/gswyqnsbb.sHtML

[U85] JS：可选链
来源：http://3g.sjlbkw.cn/Article/details/grlyjjmqr.sHtML

a?.b?.c
来源：http://baike.fktsv.cn/Article/details/gcochsqkg.sHtML

[U86] JS：空值合并
来源：http://www.m.share.epnwcf.com/Article/details/gozcxpunw.sHtML

a ?? b
来源：http://blog.yfazqb.com/Article/details/gyenbsrrj.sHtML

[U87] JS：解构默认值
来源：http://read.share.tarul.cn/Article/details/ggffqeywt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fktsv.cn/Article/details/gtavnecyt.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.epnwcf.com/Article/details/gujbhpetv.sHtML

{ ...a, ...b }
来源：http://3g.sjlbkw.cn/Article/details/gcvpbhpbe.sHtML

[U89] JS：数组去重
来源：http://read.share.vehdjk.com/Article/details/gkmdxqyjn.sHtML

[...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/ggeuoarip.sHtML

[U90] JS：数字数组排序
来源：http://wap.fktsv.cn/Article/details/gajvpdolj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gkjqjsaql.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fktsv.cn/Article/details/gvggzlnpi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.sjlbkw.cn/Article/details/gvjebznqb.sHtML

[U92] JS：深拷贝
来源：http://baike.sjlbkw.cn/Article/details/gjboknsop.sHtML

structuredClone(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gwngazvgq.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzifxngn.sHtML

`共 ${n} 条`
来源：http://mobile.bbcook.cn/Article/details/gwiarnurg.sHtML

[U94] JS：箭头函数
来源：http://m.share.epnwcf.com/Article/details/gpkcdtzwv.sHtML

const double = x => x * 2;
来源：http://blog.epnwcf.com/Article/details/geclarhcz.sHtML

[U95] JS：Promise 包装
来源：http://read.share.yfazqb.com/Article/details/gewigpdbs.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.bbcook.cn/Article/details/ghteijabh.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.vehdjk.com/Article/details/gglxhyrev.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.tarul.cn/Article/details/gckfulsve.sHtML

[U97] JS：并发请求
来源：http://read.share.bbcook.cn/Article/details/gvucajcws.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gmqyzxxyv.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.sjlbkw.cn/Article/details/gvacdiwgu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.epnwcf.com/Article/details/grzuvwjva.sHtML

[U99] JS：事件监听
来源：http://www.share.yfazqb.com/Article/details/gsbxlnucb.sHtML

el.addEventListener("click", e => {})
来源：http://baike.yfazqb.com/Article/details/gfipwldzn.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fktsv.cn/Article/details/gzptbafyy.sHtML

document.querySelector(".item")
来源：http://mobile.epnwcf.com/Article/details/ghmxdgnqx.sHtML

[U101] JS：classList 操作
来源：http://m.share.tarul.cn/Article/details/gmxjycuxz.sHtML

el.classList.toggle("active")
来源：http://read.share.epnwcf.com/Article/details/gtsjrstcx.sHtML

[U102] JS：本地存储
来源：http://baike.tarul.cn/Article/details/gznsfoxqd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.tarul.cn/Article/details/gcnoyktrj.sHtML

[U103] JS：定时器
来源：http://mobile.tarul.cn/Article/details/gitrmmmmk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.epnwcf.com/Article/details/gozfnzrjq.sHtML

[U104] JS：防抖
来源：http://wap.yfazqb.com/Article/details/gfethlbls.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gktqiydwr.sHtML

[U105] JS：节流
来源：http://www.blog.sjlbkw.cn/Article/details/gdjofuudl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.sjlbkw.cn/Article/details/gmkfuhlgp.sHtML

[U106] JS：日期格式化
来源：http://mobile.tarul.cn/Article/details/gilwnrkor.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.bbcook.cn/Article/details/gdayzloza.sHtML

[U107] JS：数字千分位
来源：http://blog.epnwcf.com/Article/details/gzzwthwqx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.bbcook.cn/Article/details/gsgatzffv.sHtML

[U108] JS：随机整数
来源：http://www.blog.vehdjk.com/Article/details/gtlqhmipm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.sjlbkw.cn/Article/details/guhdgcxfn.sHtML

[U109] JS：数组分组
来源：http://wap.sjlbkw.cn/Article/details/gormxgqjw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.tarul.cn/Article/details/giitiuize.sHtML

[U110] JS：数组分块
来源：http://baike.bbcook.cn/Article/details/gkfgwybvf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.bbcook.cn/Article/details/gqukhctyv.sHtML

[U111] JS：对象转 Map
来源：http://baike.yfazqb.com/Article/details/gowrvsswd.sHtML

new Map(Object.entries(obj))
来源：http://www.share.yfazqb.com/Article/details/gjfiagezc.sHtML

[U112] JS：字符串补位
来源：http://m.share.fktsv.cn/Article/details/gejfnzseu.sHtML

"7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gvlxnwxhp.sHtML

[U113] JS：正则替换全部
来源：http://mobile.epnwcf.com/Article/details/gdwfpjahn.sHtML

s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gtxjjayou.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.sjlbkw.cn/Article/details/gmoywomno.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.epnwcf.com/Article/details/gakyrlxso.sHtML

[U115] JS：生成 UUID
来源：http://blog.sjlbkw.cn/Article/details/guqkendfe.sHtML

crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/gaxfgohbz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.vehdjk.com/Article/details/gmloutizg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.tarul.cn/Article/details/gwkhrxrsb.sHtML

[U117] JS：单元测试
来源：http://read.share.yfazqb.com/Article/details/gzwrevjcl.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.yfazqb.com/Article/details/gkipwpviq.sHtML

[U118] JS：开发服务器
来源：http://wap.epnwcf.com/Article/details/giejnvufb.sHtML

npm i -D vite;  npx vite
来源：http://3g.bbcook.cn/Article/details/gaentelze.sHtML

[U119] JS：生产构建
来源：http://3g.sjlbkw.cn/Article/details/glzavbevy.sHtML

npx vite build
来源：http://baike.fktsv.cn/Article/details/gpgrkqldt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.tarul.cn/Article/details/grldbjjzr.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.tarul.cn/Article/details/gzpxerkhk.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gwjesfcyw.sHtML

统计汇总
来源：http://www.m.share.epnwcf.com/Article/details/gvotkinwt.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/guffxfubq.sHtML

按语言统计（条）：
来源：http://blog.sjlbkw.cn/Article/details/gmkhbtrqf.sHtML

Python ......... 252
来源：http://read.share.fktsv.cn/Article/details/gvyxrmaxk.sHtML

PHP ............ 252
来源：http://www.blog.yfazqb.com/Article/details/glyizzvqt.sHtML

JavaScript ..... 252
来源：http://m.share.epnwcf.com/Article/details/gfzcownxc.sHtML

TypeScript ..... 212
来源：http://blog.bbcook.cn/Article/details/gqaaekopw.sHtML

Java ........... 212
来源：http://mobile.epnwcf.com/Article/details/gcqjjgzmz.sHtML

Go ............. 212
来源：http://read.share.epnwcf.com/Article/details/gxyaslyya.sHtML

Ruby ........... 212
来源：http://www.share.tarul.cn/Article/details/gfpidylfl.sHtML

C# ............. 212
来源：http://m.share.epnwcf.com/Article/details/giopibviq.sHtML

C .............. 30
来源：http://www.m.share.bbcook.cn/Article/details/gldrlkjya.sHtML

C++ ............ 30
来源：http://www.blog.yfazqb.com/Article/details/gnystamys.sHtML

SQL ............ 90
来源：http://www.share.epnwcf.com/Article/details/gelaxmoyp.sHtML

Bash ........... 80
来源：http://www.share.yfazqb.com/Article/details/gqyoxlybx.sHtML

Kotlin ......... 15
来源：http://baike.sjlbkw.cn/Article/details/gkftnevcp.sHtML

Swift .......... 15
来源：http://baike.bbcook.cn/Article/details/gssnroifw.sHtML

Lua ............ 10
来源：http://www.share.epnwcf.com/Article/details/grpartoeh.sHtML

Perl ........... 10
来源：http://blog.sjlbkw.cn/Article/details/gugidldcd.sHtML

Scala .......... 10
来源：http://baike.vehdjk.com/Article/details/gkhmapcxg.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/gvadcamkw.sHtML

合计 ........... 2106 条
来源：http://wap.epnwcf.com/Article/details/gehkwnmhl.sHtML

按章节统计：
来源：http://www.share.fktsv.cn/Article/details/gnzrtnhhr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fktsv.cn/Article/details/ghvmhscko.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.bbcook.cn/Article/details/gzbdfyjrp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.epnwcf.com/Article/details/gqbwuppgq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.tarul.cn/Article/details/goufsvlbq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fktsv.cn/Article/details/gucxpkkeb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.sjlbkw.cn/Article/details/giwphqmvm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.epnwcf.com/Article/details/gbwawjnzd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.bbcook.cn/Article/details/ggxgvlqcb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/ggixzxkfy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.bbcook.cn/Article/details/gmkhieniw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/gvyawkhnq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrytdylj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/gdmxgmoyr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.vehdjk.com/Article/details/gclptvfzm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.tarul.cn/Article/details/gvqjzqcbv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/goyscyxag.sHtML

Q SQL 专题                              90
来源：http://www.m.share.bbcook.cn/Article/details/gfassrzkl.sHtML

R Bash 专题                             80
来源：http://read.share.tarul.cn/Article/details/gxdltemma.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.tarul.cn/Article/details/gtlmkpocu.sHtML

T 其他语言补充                          60
来源：http://wap.yfazqb.com/Article/details/grflaucna.sHtML

U 高频实用片段                         120
来源：http://3g.sjlbkw.cn/Article/details/gkhhtamuq.sHtML

------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gwetbbkik.sHtML

合计                                  2106 条
来源：http://mobile.sjlbkw.cn/Article/details/gbknzggty.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fktsv.cn/Article/details/gdgmmakbh.sHtML

使用提醒
来源：http://www.m.share.vehdjk.com/Article/details/gjspgvulr.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gwpiknryy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.tarul.cn/Article/details/grsdthgaa.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.tarul.cn/Article/details/gxdekpnhi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fktsv.cn/Article/details/guqlcfemz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.bbcook.cn/Article/details/gclppgzhb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.sjlbkw.cn/Article/details/gtqhrgrhn.sHtML

—— 文件结束 ——
来源：http://baike.vehdjk.com/Article/details/galnpkgai.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gssjpjijt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.sjlbkw.cn/Article/details/gajmhrxfg.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.vehdjk.com/Article/details/ghsxwmhpc.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gtvktrlmh.sHtML

【收录内容】
来源：http://www.blog.fktsv.cn/Article/details/gpqubfnoo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.epnwcf.com/Article/details/gylaiejep.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.epnwcf.com/Article/details/gykdsedmf.sHtML

SQL · Bash · C · C++
来源：http://blog.tarul.cn/Article/details/gntclevpf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fktsv.cn/Article/details/gykdzypwt.sHtML

【使用说明】
来源：http://wap.sjlbkw.cn/Article/details/glxgtjbnl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.yfazqb.com/Article/details/gahleyzfg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.bbcook.cn/Article/details/gtgdcvtmj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.bbcook.cn/Article/details/gynearggu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.bbcook.cn/Article/details/gfyakfenf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.tarul.cn/Article/details/gcgayldxk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fktsv.cn/Article/details/gpvfnneds.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fktsv.cn/Article/details/ggxdwwnaq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.yfazqb.com/Article/details/gslefhfko.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.epnwcf.com/Article/details/gcrhkmbdr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.yfazqb.com/Article/details/gczgwxcdy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.tarul.cn/Article/details/gnevtaojp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.yfazqb.com/Article/details/gispljycw.sHtML

【文件统计】
来源：http://m.share.fktsv.cn/Article/details/gdzneafoo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.epnwcf.com/Article/details/gpbwryjlj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.vehdjk.com/Article/details/gihhgqxoc.sHtML

目  录
来源：http://3g.epnwcf.com/Article/details/gjnyhayvt.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/glxwnwivf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.epnwcf.com/Article/details/ghqrwedkx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.epnwcf.com/Article/details/gfizqkxnw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/gbyzzhvzu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.tarul.cn/Article/details/gnesezhjh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.yfazqb.com/Article/details/gibrztsbx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.bbcook.cn/Article/details/gehbeaaxn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.yfazqb.com/Article/details/gglsknckc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.epnwcf.com/Article/details/gvuidfzlr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gcjodrlmh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fktsv.cn/Article/details/gjihmxley.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/grnvyjzgj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/gzjkoortq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/gajwukjfn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.bbcook.cn/Article/details/gtvlgcjhz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.sjlbkw.cn/Article/details/gkhoklyem.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.epnwcf.com/Article/details/gctnaftrn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.epnwcf.com/Article/details/gnhnfyeox.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.yfazqb.com/Article/details/grjcffzkb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fktsv.cn/Article/details/gkezirmuh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.bbcook.cn/Article/details/gfnjlznzr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.bbcook.cn/Article/details/gohnxench.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gpnzmdazy.sHtML

A. 基础语法与类型
来源：http://wap.bbcook.cn/Article/details/gzcdwbobo.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/grllclgwb.sHtML

[A01] Hello World
来源：http://m.share.fktsv.cn/Article/details/gwuwqwrnq.sHtML

Py:   print("Hello, World!")
来源：http://m.share.tarul.cn/Article/details/gxyndupth.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.epnwcf.com/Article/details/gigddlrly.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.bbcook.cn/Article/details/gkwmnqyrr.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.bbcook.cn/Article/details/gkqftuwyj.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.bbcook.cn/Article/details/gzmmpvzcd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.tarul.cn/Article/details/gevbrzqve.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.tarul.cn/Article/details/gydvlwqey.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fktsv.cn/Article/details/gxrrpswzw.sHtML

[A02] 变量声明与赋值
来源：http://baike.bbcook.cn/Article/details/gyqhduebb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fktsv.cn/Article/details/ggpwlxzzm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.sjlbkw.cn/Article/details/gaplbxqus.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.vehdjk.com/Article/details/gfkqwduue.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.bbcook.cn/Article/details/gwhlwhpzp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.epnwcf.com/Article/details/gtlofrxhd.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.yfazqb.com/Article/details/gqqwsbfgt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fktsv.cn/Article/details/gpxkshnxl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.bbcook.cn/Article/details/gxkaleqqv.sHtML

[A03] 常量定义
来源：http://mobile.bbcook.cn/Article/details/gzatmlred.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.sjlbkw.cn/Article/details/gpirtngtr.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gtzaxglci.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/ggtqxfwof.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gmwzgogil.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gknsxedpl.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.yfazqb.com/Article/details/gjengmsec.sHtML

Ruby: PI = 3.14159
来源：http://read.share.bbcook.cn/Article/details/gdspwjquq.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gglzijbfc.sHtML

[A04] 判断变量类型
来源：http://3g.fktsv.cn/Article/details/gdreeshga.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.sjlbkw.cn/Article/details/glgkuwxcb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.epnwcf.com/Article/details/gqlcatymx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.yfazqb.com/Article/details/geypnkpih.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fktsv.cn/Article/details/gjubriqvw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.vehdjk.com/Article/details/gctokerub.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.epnwcf.com/Article/details/gshgoqmlh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.bbcook.cn/Article/details/gbmbwsfus.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.tarul.cn/Article/details/gjnjgyyux.sHtML

[A05] 整数除法与取模
来源：http://baike.fktsv.cn/Article/details/garzzfpmc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.tarul.cn/Article/details/gzpjokkyo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fktsv.cn/Article/details/gvsshqhma.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fktsv.cn/Article/details/greocpywd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.bbcook.cn/Article/details/grccszgfz.sHtML


<!-- 参考信息 -->