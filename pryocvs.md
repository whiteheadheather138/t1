代发 wailian999

[U47] PHP：联合类型
来源：http://www.share.bbcook.cn/Article/details/gdlzdijlu.sHtML

int|string $id
来源：http://read.share.vehdjk.com/Article/details/gttclbxch.sHtML

[U48] PHP：纯枚举
来源：http://baike.tarul.cn/Article/details/gfyzwuvdd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.tarul.cn/Article/details/gmeviqffa.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gdekfnaua.sHtML

public readonly string $name
来源：http://mobile.sjlbkw.cn/Article/details/gdeoxwrhe.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.bbcook.cn/Article/details/gvkybbitw.sHtML

public function __construct(private int $id) {}
来源：http://wap.epnwcf.com/Article/details/guqizsiit.sHtML

[U51] PHP：数组解构
来源：http://baike.vehdjk.com/Article/details/gyodkmxig.sHtML

[$a, $b] = $arr;
来源：http://www.share.tarul.cn/Article/details/gjyccpqcr.sHtML

[U52] PHP：箭头函数
来源：http://www.share.epnwcf.com/Article/details/gfzrxwhnm.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.vehdjk.com/Article/details/gscmjicys.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.tarul.cn/Article/details/gjtpfyfya.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fktsv.cn/Article/details/gerxeigfb.sHtML

[U54] PHP：空安全调用
来源：http://read.share.bbcook.cn/Article/details/gtgcinrpk.sHtML

$obj?->method()
来源：http://blog.vehdjk.com/Article/details/gneiwfoji.sHtML

[U55] PHP：match 表达式
来源：http://blog.vehdjk.com/Article/details/gufbyalxt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.vehdjk.com/Article/details/gmgdiwytn.sHtML

[U56] PHP：命名参数
来源：http://www.share.sjlbkw.cn/Article/details/gopibskrx.sHtML

f(a: 1, b: 2)
来源：http://blog.tarul.cn/Article/details/gmokrokut.sHtML

[U57] PHP：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gzajhppjm.sHtML

"值: {$a}"
来源：http://m.share.bbcook.cn/Article/details/gspsnoudv.sHtML

[U58] PHP：数组三件套
来源：http://blog.yfazqb.com/Article/details/gxfkughkz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.vehdjk.com/Article/details/gzopwqnog.sHtML

[U59] PHP：自定义排序
来源：http://3g.epnwcf.com/Article/details/geietsqpk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.sjlbkw.cn/Article/details/geekuehry.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.sjlbkw.cn/Article/details/gnzmoakqh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.epnwcf.com/Article/details/gvmviweof.sHtML

[U61] PHP：正则
来源：http://www.blog.sjlbkw.cn/Article/details/gbbbdneet.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gvgqjbqgm.sHtML

[U62] PHP：日期对象
来源：http://wap.epnwcf.com/Article/details/gayaqfbzk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.bbcook.cn/Article/details/gbxywoajs.sHtML

[U63] PHP：文件读写
来源：http://blog.vehdjk.com/Article/details/gzsbahblq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.sjlbkw.cn/Article/details/gyjyrizwa.sHtML

[U64] PHP：目录遍历
来源：http://3g.yfazqb.com/Article/details/ghuuqpvlm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.vehdjk.com/Article/details/gfcxzuxzc.sHtML

[U65] PHP：会话
来源：http://www.blog.bbcook.cn/Article/details/gqstzxbds.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.tarul.cn/Article/details/gilksvgng.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fktsv.cn/Article/details/gsysjumia.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.epnwcf.com/Article/details/gbltwrqtx.sHtML

[U67] PHP：处理文件上传
来源：http://wap.bbcook.cn/Article/details/gnazrnnth.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.epnwcf.com/Article/details/gmyxllinr.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.yfazqb.com/Article/details/ggjmizcuw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.yfazqb.com/Article/details/gloavkvhp.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.vehdjk.com/Article/details/gkwwvcvbh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.yfazqb.com/Article/details/gwexpgaus.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.bbcook.cn/Article/details/gfysjnlpq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.epnwcf.com/Article/details/gijjcmfji.sHtML

[U71] PHP：抛出异常
来源：http://mobile.epnwcf.com/Article/details/ggtfalwzr.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.vehdjk.com/Article/details/gubiyahrz.sHtML

[U72] PHP：写错误日志
来源：http://mobile.vehdjk.com/Article/details/gzgdxlxlo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.tarul.cn/Article/details/gnhfgyeus.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.bbcook.cn/Article/details/gacoxhinb.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fktsv.cn/Article/details/gnehiacsj.sHtML

[U74] PHP：读取环境变量
来源：http://blog.bbcook.cn/Article/details/gelkmhnrz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.epnwcf.com/Article/details/gvmspgsvg.sHtML

[U75] PHP：依赖注入
来源：http://3g.vehdjk.com/Article/details/gsoquylqq.sHtML

composer require psr/container
来源：http://www.m.share.sjlbkw.cn/Article/details/gqorsafne.sHtML

[U76] PHP：简单路由
来源：http://read.share.fktsv.cn/Article/details/gnadjsqwe.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.epnwcf.com/Article/details/gtxqauibh.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fktsv.cn/Article/details/gclvqdmmm.sHtML

composer require twig/twig
来源：http://www.m.share.tarul.cn/Article/details/gtuqmsbry.sHtML

[U78] PHP：单元测试
来源：http://3g.yfazqb.com/Article/details/gzpxcsrkn.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.vehdjk.com/Article/details/gkjacnctg.sHtML

[U79] PHP：静态分析
来源：http://baike.tarul.cn/Article/details/gpsmyqntb.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.yfazqb.com/Article/details/gyleygare.sHtML

[U80] PHP：代码规范修复
来源：http://blog.tarul.cn/Article/details/gewilbtft.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.bbcook.cn/Article/details/ghzrkjrsn.sHtML

[U81] JS：初始化项目
来源：http://wap.epnwcf.com/Article/details/gpxkfkoeq.sHtML

npm init -y;  npm i express
来源：http://www.blog.bbcook.cn/Article/details/gwvwsyvyn.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fktsv.cn/Article/details/ghpkrnqix.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.sjlbkw.cn/Article/details/gtlhjhdhh.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.sjlbkw.cn/Article/details/gqktqjytt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.vehdjk.com/Article/details/goejhfiyp.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.vehdjk.com/Article/details/gheuyzuzz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.yfazqb.com/Article/details/gwygnynia.sHtML

[U85] JS：可选链
来源：http://www.m.share.epnwcf.com/Article/details/gefzkasqx.sHtML

a?.b?.c
来源：http://m.share.bbcook.cn/Article/details/gcgiuspyz.sHtML

[U86] JS：空值合并
来源：http://m.share.sjlbkw.cn/Article/details/gweefimpy.sHtML

a ?? b
来源：http://read.share.bbcook.cn/Article/details/gcdfpsqgf.sHtML

[U87] JS：解构默认值
来源：http://blog.yfazqb.com/Article/details/gxwwinvkg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.epnwcf.com/Article/details/gzhxtcxyt.sHtML

[U88] JS：对象展开合并
来源：http://baike.yfazqb.com/Article/details/gbjeagphy.sHtML

{ ...a, ...b }
来源：http://baike.yfazqb.com/Article/details/gwmrsqebc.sHtML

[U89] JS：数组去重
来源：http://www.share.tarul.cn/Article/details/gmicvubef.sHtML

[...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/gzdxwvljc.sHtML

[U90] JS：数字数组排序
来源：http://3g.fktsv.cn/Article/details/gvmczfqja.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/ghnjpwqvi.sHtML

[U91] JS：对象键值遍历
来源：http://3g.tarul.cn/Article/details/gfbhkydwt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.epnwcf.com/Article/details/giafpkufu.sHtML

[U92] JS：深拷贝
来源：http://read.share.bbcook.cn/Article/details/gzxhygsld.sHtML

structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gqfynwrba.sHtML

[U93] JS：模板字符串
来源：http://blog.epnwcf.com/Article/details/gfzccgfcp.sHtML

`共 ${n} 条`
来源：http://3g.epnwcf.com/Article/details/gazaxjinl.sHtML

[U94] JS：箭头函数
来源：http://www.blog.yfazqb.com/Article/details/gacarbihg.sHtML

const double = x => x * 2;
来源：http://mobile.epnwcf.com/Article/details/gchqocevl.sHtML

[U95] JS：Promise 包装
来源：http://3g.bbcook.cn/Article/details/gzwrbaerw.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fktsv.cn/Article/details/ghzkjitug.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.epnwcf.com/Article/details/gvwcokgyj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gkbwhdexo.sHtML

[U97] JS：并发请求
来源：http://www.share.sjlbkw.cn/Article/details/grzizsnkq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/gckffikth.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.tarul.cn/Article/details/ghcjawncq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.tarul.cn/Article/details/gnasuwddl.sHtML

[U99] JS：事件监听
来源：http://mobile.vehdjk.com/Article/details/gbvydsvao.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.vehdjk.com/Article/details/gxuoqcncn.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gowcxbugy.sHtML

document.querySelector(".item")
来源：http://mobile.epnwcf.com/Article/details/gqocwbjas.sHtML

[U101] JS：classList 操作
来源：http://wap.fktsv.cn/Article/details/gyqinmjen.sHtML

el.classList.toggle("active")
来源：http://www.share.vehdjk.com/Article/details/gyitjktfx.sHtML

[U102] JS：本地存储
来源：http://read.share.tarul.cn/Article/details/goxwjdmre.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.sjlbkw.cn/Article/details/gpvtryubb.sHtML

[U103] JS：定时器
来源：http://wap.epnwcf.com/Article/details/gcokbrfvt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.vehdjk.com/Article/details/gbesfhzyp.sHtML

[U104] JS：防抖
来源：http://mobile.sjlbkw.cn/Article/details/ggyaajjnw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/gzthqixxb.sHtML

[U105] JS：节流
来源：http://read.share.fktsv.cn/Article/details/gjefqodix.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.tarul.cn/Article/details/gkizefzau.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/gjbizcbtl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.tarul.cn/Article/details/gonnebtyb.sHtML

[U107] JS：数字千分位
来源：http://read.share.sjlbkw.cn/Article/details/gugrcjwyu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.bbcook.cn/Article/details/gjqpnlwir.sHtML

[U108] JS：随机整数
来源：http://blog.vehdjk.com/Article/details/gmsmfuceg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fktsv.cn/Article/details/gkgsafnzj.sHtML

[U109] JS：数组分组
来源：http://3g.fktsv.cn/Article/details/guqeauepk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.epnwcf.com/Article/details/gelgudxxp.sHtML

[U110] JS：数组分块
来源：http://blog.tarul.cn/Article/details/gepmjiavc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.tarul.cn/Article/details/gjxavvhwf.sHtML

[U111] JS：对象转 Map
来源：http://read.share.bbcook.cn/Article/details/gcdrmowqm.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.yfazqb.com/Article/details/gabrqailf.sHtML

[U112] JS：字符串补位
来源：http://wap.sjlbkw.cn/Article/details/gfeibodwk.sHtML

"7".padStart(3, "0")
来源：http://baike.fktsv.cn/Article/details/glpwdfuyt.sHtML

[U113] JS：正则替换全部
来源：http://read.share.bbcook.cn/Article/details/ggwjwkoel.sHtML

s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gngqqrffi.sHtML

[U114] JS：JSON 深比较
来源：http://wap.epnwcf.com/Article/details/gzvppuuds.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/gyrspizlm.sHtML

[U115] JS：生成 UUID
来源：http://3g.bbcook.cn/Article/details/glozmlghj.sHtML

crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gbyodhlbq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.bbcook.cn/Article/details/ghuufzreg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.bbcook.cn/Article/details/gjkoerogd.sHtML

[U117] JS：单元测试
来源：http://www.m.share.vehdjk.com/Article/details/gsicarxje.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.tarul.cn/Article/details/ghizpdecz.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.vehdjk.com/Article/details/gwofftsoj.sHtML

npm i -D vite;  npx vite
来源：http://baike.tarul.cn/Article/details/gabytuuqa.sHtML

[U119] JS：生产构建
来源：http://3g.vehdjk.com/Article/details/gaiefvqxa.sHtML

npx vite build
来源：http://blog.epnwcf.com/Article/details/gbyzlrjnz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.yfazqb.com/Article/details/gwqsiqokn.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.tarul.cn/Article/details/gsixcudhn.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gridtghsw.sHtML

统计汇总
来源：http://baike.tarul.cn/Article/details/gkekcqzlv.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gymevlgfz.sHtML

按语言统计（条）：
来源：http://read.share.yfazqb.com/Article/details/gmpqtosrl.sHtML

Python ......... 252
来源：http://read.share.sjlbkw.cn/Article/details/gefafurtm.sHtML

PHP ............ 252
来源：http://3g.vehdjk.com/Article/details/gzyaxxsts.sHtML

JavaScript ..... 252
来源：http://blog.bbcook.cn/Article/details/gnienwcdf.sHtML

TypeScript ..... 212
来源：http://www.share.epnwcf.com/Article/details/ggxkambyp.sHtML

Java ........... 212
来源：http://mobile.vehdjk.com/Article/details/gexmrbvfj.sHtML

Go ............. 212
来源：http://www.m.share.epnwcf.com/Article/details/gfootpokd.sHtML

Ruby ........... 212
来源：http://www.m.share.tarul.cn/Article/details/gvpbypbyn.sHtML

C# ............. 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnfgantr.sHtML

C .............. 30
来源：http://m.share.vehdjk.com/Article/details/glmwubwuh.sHtML

C++ ............ 30
来源：http://www.share.tarul.cn/Article/details/gwfusshpg.sHtML

SQL ............ 90
来源：http://mobile.fktsv.cn/Article/details/ghsjgdbie.sHtML

Bash ........... 80
来源：http://www.blog.vehdjk.com/Article/details/gbjzjabys.sHtML

Kotlin ......... 15
来源：http://wap.sjlbkw.cn/Article/details/gltegiunm.sHtML

Swift .......... 15
来源：http://baike.bbcook.cn/Article/details/geqdplqsu.sHtML

Lua ............ 10
来源：http://www.share.sjlbkw.cn/Article/details/gxvbmowqc.sHtML

Perl ........... 10
来源：http://m.share.tarul.cn/Article/details/gpkwkpmvv.sHtML

Scala .......... 10
来源：http://read.share.vehdjk.com/Article/details/gqrvyomcp.sHtML

------------------------------------
来源：http://blog.epnwcf.com/Article/details/geanqedkc.sHtML

合计 ........... 2106 条
来源：http://www.m.share.epnwcf.com/Article/details/gkkvxjxwo.sHtML

按章节统计：
来源：http://wap.epnwcf.com/Article/details/gbrcwxzlo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.sjlbkw.cn/Article/details/gxqzqnjxp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.epnwcf.com/Article/details/gkjmahbbx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.vehdjk.com/Article/details/gkgregzqn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.yfazqb.com/Article/details/gthoklnax.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.bbcook.cn/Article/details/gaeefvdwg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.vehdjk.com/Article/details/gqoggyltk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.epnwcf.com/Article/details/gbyzfyyzi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.vehdjk.com/Article/details/grtnmqytz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gecclthpr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.epnwcf.com/Article/details/gfccxsmta.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/galcomkfv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/gfuvlewdl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/gzivxugxs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.bbcook.cn/Article/details/gexpewmir.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fktsv.cn/Article/details/gfcoitcnm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/gtogooejs.sHtML

Q SQL 专题                              90
来源：http://www.blog.vehdjk.com/Article/details/gtozlzsqp.sHtML

R Bash 专题                             80
来源：http://blog.epnwcf.com/Article/details/gepuqtxtb.sHtML

S C / C++ 专题                          60
来源：http://read.share.yfazqb.com/Article/details/gxlqmzwfg.sHtML

T 其他语言补充                          60
来源：http://baike.sjlbkw.cn/Article/details/gonobjtqg.sHtML

U 高频实用片段                         120
来源：http://www.share.vehdjk.com/Article/details/gjcmowkjw.sHtML

------------------------------------
来源：http://m.share.fktsv.cn/Article/details/glgevexno.sHtML

合计                                  2106 条
来源：http://www.m.share.yfazqb.com/Article/details/gnprdaexk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/grqvgdpma.sHtML

使用提醒
来源：http://blog.tarul.cn/Article/details/guwyinjpg.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/gdglwskhx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fktsv.cn/Article/details/gjbfqvspd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.vehdjk.com/Article/details/gvokobalj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.tarul.cn/Article/details/gxvjdspau.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.epnwcf.com/Article/details/gvnovjbuh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.yfazqb.com/Article/details/gzivzqsvj.sHtML

—— 文件结束 ——
来源：http://baike.tarul.cn/Article/details/gbgxyoflr.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ghphtglte.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.bbcook.cn/Article/details/gyliiyrrh.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.tarul.cn/Article/details/gjwmplkhw.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gnvesmnju.sHtML

【收录内容】
来源：http://www.blog.sjlbkw.cn/Article/details/gwwfqubuo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.tarul.cn/Article/details/gemfpxhqx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.vehdjk.com/Article/details/gwvsynmpl.sHtML

SQL · Bash · C · C++
来源：http://wap.tarul.cn/Article/details/gceiszdvt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.yfazqb.com/Article/details/guphvowho.sHtML

【使用说明】
来源：http://3g.bbcook.cn/Article/details/gczengspu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fktsv.cn/Article/details/gexxsfuta.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.yfazqb.com/Article/details/gjxbxkzdz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.sjlbkw.cn/Article/details/gxtywskml.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.tarul.cn/Article/details/gacnzilhj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.vehdjk.com/Article/details/gplfnoawt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.vehdjk.com/Article/details/gefwzudll.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fktsv.cn/Article/details/gtzxqvxdi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.sjlbkw.cn/Article/details/gsvqsquwo.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.vehdjk.com/Article/details/gxkwkolcd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.vehdjk.com/Article/details/gbnfplfro.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fktsv.cn/Article/details/grklyjfhh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.vehdjk.com/Article/details/gcawoegxr.sHtML

【文件统计】
来源：http://m.share.bbcook.cn/Article/details/ggondqiox.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.yfazqb.com/Article/details/grcmjumdp.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.tarul.cn/Article/details/gdgumpnak.sHtML

目  录
来源：http://www.blog.bbcook.cn/Article/details/gjaqkmjcn.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/grxdwnxfy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.epnwcf.com/Article/details/goflcdigk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.sjlbkw.cn/Article/details/guxbsfkbs.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.bbcook.cn/Article/details/gkbnydkjh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fktsv.cn/Article/details/gmqjlyhdn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.yfazqb.com/Article/details/goxwwfjmy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkgcvpdk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.tarul.cn/Article/details/gkudotndb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.bbcook.cn/Article/details/gwnyehwyk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.epnwcf.com/Article/details/gpybihlya.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.epnwcf.com/Article/details/gsitsdizp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtnnqsms.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/ghrcnqflu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/gzdwhdlel.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fktsv.cn/Article/details/gofugownf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fktsv.cn/Article/details/gwdoarnen.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/grzxussga.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.sjlbkw.cn/Article/details/gpjevqqad.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.vehdjk.com/Article/details/gagmucocj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.yfazqb.com/Article/details/gspknjpft.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.yfazqb.com/Article/details/guwyoejru.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.epnwcf.com/Article/details/gkbzqpbsx.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gpwxjvjzf.sHtML

A. 基础语法与类型
来源：http://www.share.tarul.cn/Article/details/gcqegppwc.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/ggjozvwqq.sHtML

[A01] Hello World
来源：http://baike.bbcook.cn/Article/details/gxelggfcn.sHtML

Py:   print("Hello, World!")
来源：http://read.share.yfazqb.com/Article/details/gsbptjpxl.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.vehdjk.com/Article/details/gatmjxvlj.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.sjlbkw.cn/Article/details/gqstbihzt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.epnwcf.com/Article/details/grahhmklz.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.sjlbkw.cn/Article/details/geaufbllp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fktsv.cn/Article/details/gmgpqahpn.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fktsv.cn/Article/details/gghsrxnok.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.sjlbkw.cn/Article/details/grdvqcjzg.sHtML

[A02] 变量声明与赋值
来源：http://3g.epnwcf.com/Article/details/gqxjwtuvy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.vehdjk.com/Article/details/gksaxivov.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.bbcook.cn/Article/details/ggpqgsfoj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.bbcook.cn/Article/details/gpxkugcfh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.vehdjk.com/Article/details/gndzydghi.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.bbcook.cn/Article/details/gtrfmmqkh.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fktsv.cn/Article/details/gxepdvwou.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.bbcook.cn/Article/details/gnffymdgc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.yfazqb.com/Article/details/gkwzomtte.sHtML

[A03] 常量定义
来源：http://3g.yfazqb.com/Article/details/gbdhqippk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.vehdjk.com/Article/details/gzkcbbyof.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gkgqcmwbt.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gvlplcvfu.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gpvisylou.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gapvlzgqx.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fktsv.cn/Article/details/gbnvipsgv.sHtML

Ruby: PI = 3.14159
来源：http://read.share.epnwcf.com/Article/details/gebhunhwc.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gtmwfbcbf.sHtML

[A04] 判断变量类型
来源：http://www.m.share.yfazqb.com/Article/details/gjgqsmenb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.sjlbkw.cn/Article/details/gpeegnfhj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.tarul.cn/Article/details/giqnulyuz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.vehdjk.com/Article/details/gxpuxicqh.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.epnwcf.com/Article/details/gcxcvgfrg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.yfazqb.com/Article/details/gtzqrgzau.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.epnwcf.com/Article/details/gjtqxhpkq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fktsv.cn/Article/details/ggvyvpxil.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.bbcook.cn/Article/details/gbctssgxf.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.bbcook.cn/Article/details/gobgwonuf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.bbcook.cn/Article/details/gwajjxrux.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.yfazqb.com/Article/details/ggwltcawo.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.epnwcf.com/Article/details/gudncjpig.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.yfazqb.com/Article/details/gwkabrwrp.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqntznrj.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.epnwcf.com/Article/details/gnqfyuscg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.epnwcf.com/Article/details/gsxzrqois.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fktsv.cn/Article/details/gsuftwfsb.sHtML


<!-- 参考信息 -->