代发 wailian999

[U47] PHP：联合类型
来源：http://www.blog.bbcook.cn/Article/details/gjsixuggz.sHtML

int|string $id
来源：http://blog.bbcook.cn/Article/details/gerytyioy.sHtML

[U48] PHP：纯枚举
来源：http://m.share.epnwcf.com/Article/details/gkxpczyvb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.tarul.cn/Article/details/gwttoygzu.sHtML

[U49] PHP：只读属性
来源：http://read.share.vehdjk.com/Article/details/gazmgmykt.sHtML

public readonly string $name
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwultkzw.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fktsv.cn/Article/details/goezhblht.sHtML

public function __construct(private int $id) {}
来源：http://wap.tarul.cn/Article/details/gyqoysxql.sHtML

[U51] PHP：数组解构
来源：http://read.share.bbcook.cn/Article/details/gworqaimj.sHtML

[$a, $b] = $arr;
来源：http://wap.vehdjk.com/Article/details/gluflbnuw.sHtML

[U52] PHP：箭头函数
来源：http://wap.yfazqb.com/Article/details/gxnjnuvqu.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fktsv.cn/Article/details/gadbcfojy.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.tarul.cn/Article/details/gtzedjooc.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.vehdjk.com/Article/details/gtscgiyoq.sHtML

[U54] PHP：空安全调用
来源：http://m.share.yfazqb.com/Article/details/gcwcmgawo.sHtML

$obj?->method()
来源：http://3g.vehdjk.com/Article/details/gfirnqodt.sHtML

[U55] PHP：match 表达式
来源：http://3g.sjlbkw.cn/Article/details/geaglabye.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.bbcook.cn/Article/details/gfofqxncf.sHtML

[U56] PHP：命名参数
来源：http://read.share.bbcook.cn/Article/details/gmjfwlvgh.sHtML

f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/gpuxhtgli.sHtML

[U57] PHP：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gsekzggln.sHtML

"值: {$a}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gyygfuhzl.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.bbcook.cn/Article/details/gmapaobxa.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.yfazqb.com/Article/details/gcbnlueev.sHtML

[U59] PHP：自定义排序
来源：http://3g.yfazqb.com/Article/details/glnottaqb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.bbcook.cn/Article/details/grpabqzgo.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fktsv.cn/Article/details/gwcrsehtb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.yfazqb.com/Article/details/gbaimzbgp.sHtML

[U61] PHP：正则
来源：http://baike.sjlbkw.cn/Article/details/gxgxewscg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.bbcook.cn/Article/details/grzjofidz.sHtML

[U62] PHP：日期对象
来源：http://www.share.tarul.cn/Article/details/gvugvwmvc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.vehdjk.com/Article/details/ghbvrzosz.sHtML

[U63] PHP：文件读写
来源：http://wap.vehdjk.com/Article/details/ghqwicbwm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.vehdjk.com/Article/details/giuztagau.sHtML

[U64] PHP：目录遍历
来源：http://wap.tarul.cn/Article/details/gxeircwtl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.yfazqb.com/Article/details/giobbynbu.sHtML

[U65] PHP：会话
来源：http://www.blog.tarul.cn/Article/details/gjiwridoj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.yfazqb.com/Article/details/ghgwyzige.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.yfazqb.com/Article/details/ghkhlrrdb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.yfazqb.com/Article/details/gzrdguyfh.sHtML

[U67] PHP：处理文件上传
来源：http://wap.yfazqb.com/Article/details/gcaamgtaw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.epnwcf.com/Article/details/gnuwadzjp.sHtML

[U68] PHP：PDO 连接
来源：http://baike.tarul.cn/Article/details/gulhqloum.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.vehdjk.com/Article/details/guvlbtqzr.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.epnwcf.com/Article/details/gdbptmfgm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fktsv.cn/Article/details/gcuzuakfx.sHtML

[U70] PHP：PDO 事务
来源：http://baike.vehdjk.com/Article/details/gbrccsvtq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.sjlbkw.cn/Article/details/gncnlelft.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fktsv.cn/Article/details/gmjlgivvi.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.yfazqb.com/Article/details/gchrndxjc.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.epnwcf.com/Article/details/gkhrzcwwr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fktsv.cn/Article/details/galwcaylh.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.bbcook.cn/Article/details/gbtqhnomz.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.bbcook.cn/Article/details/gnlgbfxwm.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.yfazqb.com/Article/details/gphinzdwc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.vehdjk.com/Article/details/gjhamxqix.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.yfazqb.com/Article/details/gogivljvx.sHtML

composer require psr/container
来源：http://mobile.fktsv.cn/Article/details/gwudgolws.sHtML

[U76] PHP：简单路由
来源：http://www.share.fktsv.cn/Article/details/grqpqfofg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fktsv.cn/Article/details/gfyjztkjv.sHtML

[U77] PHP：模板渲染
来源：http://mobile.yfazqb.com/Article/details/ggevnhinm.sHtML

composer require twig/twig
来源：http://3g.tarul.cn/Article/details/gzadhibgx.sHtML

[U78] PHP：单元测试
来源：http://3g.vehdjk.com/Article/details/grwcwgead.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fktsv.cn/Article/details/glgoteruv.sHtML

[U79] PHP：静态分析
来源：http://m.share.sjlbkw.cn/Article/details/gzcxuwdrf.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.epnwcf.com/Article/details/gsjofswqk.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fktsv.cn/Article/details/geqhlqksw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.bbcook.cn/Article/details/gsldonfep.sHtML

[U81] JS：初始化项目
来源：http://www.share.tarul.cn/Article/details/gqhdapfrf.sHtML

npm init -y;  npm i express
来源：http://mobile.fktsv.cn/Article/details/gwmrjqvog.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fktsv.cn/Article/details/gdpqcuxda.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.tarul.cn/Article/details/gwkegidzp.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.tarul.cn/Article/details/geuskqkkw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.yfazqb.com/Article/details/guevypweb.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.tarul.cn/Article/details/gnvhbdmbq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.sjlbkw.cn/Article/details/gczbufrzk.sHtML

[U85] JS：可选链
来源：http://www.blog.bbcook.cn/Article/details/gpmfmlipm.sHtML

a?.b?.c
来源：http://blog.tarul.cn/Article/details/gndzvnjbe.sHtML

[U86] JS：空值合并
来源：http://blog.bbcook.cn/Article/details/guesqatwp.sHtML

a ?? b
来源：http://www.m.share.bbcook.cn/Article/details/gfhgzblbb.sHtML

[U87] JS：解构默认值
来源：http://blog.bbcook.cn/Article/details/gissioywc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fktsv.cn/Article/details/gcgulzulm.sHtML

[U88] JS：对象展开合并
来源：http://wap.tarul.cn/Article/details/ganelaths.sHtML

{ ...a, ...b }
来源：http://read.share.sjlbkw.cn/Article/details/gpamviqmi.sHtML

[U89] JS：数组去重
来源：http://www.blog.yfazqb.com/Article/details/grsmefcxr.sHtML

[...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/ghfrqhtpu.sHtML

[U90] JS：数字数组排序
来源：http://m.share.epnwcf.com/Article/details/ganhfwkyh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gryrzsbbg.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.epnwcf.com/Article/details/gclhcdenm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.bbcook.cn/Article/details/gwcmjpiqo.sHtML

[U92] JS：深拷贝
来源：http://wap.epnwcf.com/Article/details/gfwwtbxar.sHtML

structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/grvxuelxp.sHtML

[U93] JS：模板字符串
来源：http://m.share.tarul.cn/Article/details/gnqiodgok.sHtML

`共 ${n} 条`
来源：http://mobile.epnwcf.com/Article/details/gjckixxsz.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.bbcook.cn/Article/details/geigyilul.sHtML

const double = x => x * 2;
来源：http://www.share.bbcook.cn/Article/details/gomoliilk.sHtML

[U95] JS：Promise 包装
来源：http://read.share.sjlbkw.cn/Article/details/geuxlotoo.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.bbcook.cn/Article/details/gvviaoyyt.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fktsv.cn/Article/details/gckxsgbyw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gezzlwbkd.sHtML

[U97] JS：并发请求
来源：http://m.share.tarul.cn/Article/details/gfulmyjzc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gzojlskcv.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fktsv.cn/Article/details/gaclfzckt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.yfazqb.com/Article/details/gkwbybfql.sHtML

[U99] JS：事件监听
来源：http://www.blog.fktsv.cn/Article/details/gnatvealb.sHtML

el.addEventListener("click", e => {})
来源：http://wap.vehdjk.com/Article/details/gafbppdam.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.yfazqb.com/Article/details/gjkgnqyet.sHtML

document.querySelector(".item")
来源：http://blog.sjlbkw.cn/Article/details/grbkvrkqt.sHtML

[U101] JS：classList 操作
来源：http://read.share.epnwcf.com/Article/details/ggpejykhe.sHtML

el.classList.toggle("active")
来源：http://www.m.share.yfazqb.com/Article/details/gjmpiuolq.sHtML

[U102] JS：本地存储
来源：http://wap.vehdjk.com/Article/details/gkscklknk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.yfazqb.com/Article/details/girdiidki.sHtML

[U103] JS：定时器
来源：http://m.share.epnwcf.com/Article/details/ghehvsvch.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.tarul.cn/Article/details/gsysjsdup.sHtML

[U104] JS：防抖
来源：http://m.share.yfazqb.com/Article/details/ggfbqlhjl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gyiglpgco.sHtML

[U105] JS：节流
来源：http://wap.yfazqb.com/Article/details/gdwpjnsjl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.epnwcf.com/Article/details/gtihbeham.sHtML

[U106] JS：日期格式化
来源：http://3g.epnwcf.com/Article/details/gaxkpiizt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.yfazqb.com/Article/details/gfxjbohxg.sHtML

[U107] JS：数字千分位
来源：http://m.share.bbcook.cn/Article/details/gztoequtl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.vehdjk.com/Article/details/ggxffyqfe.sHtML

[U108] JS：随机整数
来源：http://mobile.yfazqb.com/Article/details/gnjjzuetg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.vehdjk.com/Article/details/gwumtakyb.sHtML

[U109] JS：数组分组
来源：http://m.share.yfazqb.com/Article/details/ghqgujliz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fktsv.cn/Article/details/goruulhdd.sHtML

[U110] JS：数组分块
来源：http://3g.fktsv.cn/Article/details/gwxajdfhb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.yfazqb.com/Article/details/gkkurxezz.sHtML

[U111] JS：对象转 Map
来源：http://baike.sjlbkw.cn/Article/details/ghltntzot.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.sjlbkw.cn/Article/details/gabbeugiw.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsxipvrc.sHtML

"7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gbvkqqsbl.sHtML

[U113] JS：正则替换全部
来源：http://mobile.epnwcf.com/Article/details/gbdnqjkqs.sHtML

s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gvtcgezaa.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.yfazqb.com/Article/details/gpnbpebeh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.epnwcf.com/Article/details/gjmcfgixv.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.bbcook.cn/Article/details/gufllpgje.sHtML

crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/gcrloykwn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fktsv.cn/Article/details/gpartnfoc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.yfazqb.com/Article/details/guhwvehci.sHtML

[U117] JS：单元测试
来源：http://baike.epnwcf.com/Article/details/gcqeicayd.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.tarul.cn/Article/details/gtqlzdehu.sHtML

[U118] JS：开发服务器
来源：http://www.blog.vehdjk.com/Article/details/gjrgeurhh.sHtML

npm i -D vite;  npx vite
来源：http://3g.vehdjk.com/Article/details/gadfwxsyl.sHtML

[U119] JS：生产构建
来源：http://3g.vehdjk.com/Article/details/gsxunxgre.sHtML

npx vite build
来源：http://www.blog.bbcook.cn/Article/details/giaacjmju.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.yfazqb.com/Article/details/gbfgyjqdy.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.bbcook.cn/Article/details/gxfvrljqr.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/goqldfzep.sHtML

统计汇总
来源：http://www.m.share.fktsv.cn/Article/details/gurdgbcya.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gjzefovtz.sHtML

按语言统计（条）：
来源：http://www.blog.yfazqb.com/Article/details/grpdpxnjp.sHtML

Python ......... 252
来源：http://wap.vehdjk.com/Article/details/gnzhjycrp.sHtML

PHP ............ 252
来源：http://www.share.bbcook.cn/Article/details/grciiwhpk.sHtML

JavaScript ..... 252
来源：http://www.share.fktsv.cn/Article/details/gngjgfytn.sHtML

TypeScript ..... 212
来源：http://www.share.bbcook.cn/Article/details/gqgpzikcm.sHtML

Java ........... 212
来源：http://www.share.yfazqb.com/Article/details/ginjbsnbd.sHtML

Go ............. 212
来源：http://blog.bbcook.cn/Article/details/glmcfkufi.sHtML

Ruby ........... 212
来源：http://www.blog.bbcook.cn/Article/details/gslcnmvyz.sHtML

C# ............. 212
来源：http://mobile.tarul.cn/Article/details/gafnbeodt.sHtML

C .............. 30
来源：http://www.blog.yfazqb.com/Article/details/gqozsfmcs.sHtML

C++ ............ 30
来源：http://www.share.epnwcf.com/Article/details/gmnnkfjyx.sHtML

SQL ............ 90
来源：http://blog.vehdjk.com/Article/details/gduoiyxiy.sHtML

Bash ........... 80
来源：http://mobile.yfazqb.com/Article/details/gmaorarxt.sHtML

Kotlin ......... 15
来源：http://www.share.tarul.cn/Article/details/glqxrpemp.sHtML

Swift .......... 15
来源：http://3g.vehdjk.com/Article/details/ghgidafyx.sHtML

Lua ............ 10
来源：http://mobile.fktsv.cn/Article/details/gqqvhdwqy.sHtML

Perl ........... 10
来源：http://blog.sjlbkw.cn/Article/details/gbuoyecfu.sHtML

Scala .......... 10
来源：http://wap.tarul.cn/Article/details/gsbjzzmla.sHtML

------------------------------------
来源：http://baike.bbcook.cn/Article/details/goimnqhkd.sHtML

合计 ........... 2106 条
来源：http://mobile.epnwcf.com/Article/details/gvwqkafci.sHtML

按章节统计：
来源：http://wap.sjlbkw.cn/Article/details/gazevqxsc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.bbcook.cn/Article/details/gnxevjrkr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fktsv.cn/Article/details/gtavhypny.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.bbcook.cn/Article/details/gkwwswvqf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.bbcook.cn/Article/details/gtgsyoaew.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.yfazqb.com/Article/details/gnizngusf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.tarul.cn/Article/details/gevutgwxo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.epnwcf.com/Article/details/gcucdcajr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.sjlbkw.cn/Article/details/gwgasrinc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gipguuoqm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fktsv.cn/Article/details/gqpabpzpw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gvngbqvhb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.tarul.cn/Article/details/gwhgmwsud.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/gkuqxugay.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.epnwcf.com/Article/details/gwijnrkwn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.epnwcf.com/Article/details/grluxflsy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/glwzctghd.sHtML

Q SQL 专题                              90
来源：http://read.share.bbcook.cn/Article/details/gcqmsanql.sHtML

R Bash 专题                             80
来源：http://m.share.bbcook.cn/Article/details/gmipdqsqq.sHtML

S C / C++ 专题                          60
来源：http://wap.bbcook.cn/Article/details/gjikqcnzt.sHtML

T 其他语言补充                          60
来源：http://wap.yfazqb.com/Article/details/gnzkxuxpe.sHtML

U 高频实用片段                         120
来源：http://blog.yfazqb.com/Article/details/gboxnkbxc.sHtML

------------------------------------
来源：http://wap.epnwcf.com/Article/details/gixwmkzbk.sHtML

合计                                  2106 条
来源：http://www.share.bbcook.cn/Article/details/gkippztex.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gpxownruj.sHtML

使用提醒
来源：http://www.blog.epnwcf.com/Article/details/gyirouuqw.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/gwezhhhvk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fktsv.cn/Article/details/gytdvsklf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.bbcook.cn/Article/details/gvfuayoeu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.bbcook.cn/Article/details/gqqsllfqt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.vehdjk.com/Article/details/gwmlzwkot.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fktsv.cn/Article/details/gmqkdxsye.sHtML

—— 文件结束 ——
来源：http://www.m.share.epnwcf.com/Article/details/gxtbeymuo.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gflxckwxu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.epnwcf.com/Article/details/guaupdpqp.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.yfazqb.com/Article/details/gxusqgzvd.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ghhnbgilm.sHtML

【收录内容】
来源：http://baike.tarul.cn/Article/details/gueizhplu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.tarul.cn/Article/details/gppmtfeej.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.sjlbkw.cn/Article/details/gcozdgsty.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.epnwcf.com/Article/details/gnghcmfml.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.epnwcf.com/Article/details/gkdrlakuw.sHtML

【使用说明】
来源：http://blog.fktsv.cn/Article/details/gsfitmgck.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.yfazqb.com/Article/details/gwjuhtlio.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.vehdjk.com/Article/details/gndycbjnp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.yfazqb.com/Article/details/gzbwqpsgb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.vehdjk.com/Article/details/gysjptpfw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.vehdjk.com/Article/details/gsfsttarx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fktsv.cn/Article/details/gwalkhkyb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.sjlbkw.cn/Article/details/gbsjjbfle.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.bbcook.cn/Article/details/gwfwohazh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.yfazqb.com/Article/details/gbdjpnypd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.epnwcf.com/Article/details/geeyedoal.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fktsv.cn/Article/details/gzvbfqzkk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fktsv.cn/Article/details/gmvcahwvl.sHtML

【文件统计】
来源：http://www.share.sjlbkw.cn/Article/details/gqugqeggv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.sjlbkw.cn/Article/details/ggiypaowr.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gunzmfpjh.sHtML

目  录
来源：http://www.blog.vehdjk.com/Article/details/gletgwvrn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gjmpvhaqd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.sjlbkw.cn/Article/details/gqxnhmbri.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.yfazqb.com/Article/details/gtdvtpsbn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.yfazqb.com/Article/details/gjhehpjmy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.vehdjk.com/Article/details/gcxshlnwz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fktsv.cn/Article/details/ggxazqcay.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.tarul.cn/Article/details/gkhoikwes.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.tarul.cn/Article/details/gkcabzymh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.sjlbkw.cn/Article/details/gdxpvcejf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/grjtygvrc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.vehdjk.com/Article/details/geldvpqjm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fktsv.cn/Article/details/ggrufpjxt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gjuagyzzy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.sjlbkw.cn/Article/details/gpugglhhz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.vehdjk.com/Article/details/ghgbfbclc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.epnwcf.com/Article/details/gfuorcvwp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.yfazqb.com/Article/details/gqjsugcqz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fktsv.cn/Article/details/gthqhztce.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.yfazqb.com/Article/details/gxlemjcby.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.tarul.cn/Article/details/gnqdppuvj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.sjlbkw.cn/Article/details/gzzygesbz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.bbcook.cn/Article/details/gqyvaenho.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gksdxpmzd.sHtML

A. 基础语法与类型
来源：http://read.share.vehdjk.com/Article/details/gmqwooipo.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gxedkvcql.sHtML

[A01] Hello World
来源：http://baike.bbcook.cn/Article/details/gknjxvaag.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.epnwcf.com/Article/details/gtfkcwnym.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.yfazqb.com/Article/details/gbtyzrgps.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.bbcook.cn/Article/details/geoibxjrp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fktsv.cn/Article/details/gaypjwfkd.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.epnwcf.com/Article/details/gznbxudcp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.tarul.cn/Article/details/gogoxqrka.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.epnwcf.com/Article/details/gfxmdftlx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.yfazqb.com/Article/details/gdllalgnn.sHtML

[A02] 变量声明与赋值
来源：http://3g.tarul.cn/Article/details/gtofhyiib.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.tarul.cn/Article/details/gtlaxiytl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.epnwcf.com/Article/details/gwrkqjcgd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fktsv.cn/Article/details/gpaihlhhe.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.vehdjk.com/Article/details/gphfodbnh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.yfazqb.com/Article/details/gvrvfmsny.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.vehdjk.com/Article/details/gsygwjxgs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.bbcook.cn/Article/details/ggjsaadlz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.tarul.cn/Article/details/ghivjrfxx.sHtML

[A03] 常量定义
来源：http://mobile.yfazqb.com/Article/details/gsmjxoyzy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.yfazqb.com/Article/details/gholofsba.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gpuyoygpi.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fktsv.cn/Article/details/goctzfidq.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.sjlbkw.cn/Article/details/gniaejhof.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gskktkrri.sHtML

Go:   const PI = 3.14159
来源：http://baike.bbcook.cn/Article/details/gatbvnauy.sHtML

Ruby: PI = 3.14159
来源：http://m.share.epnwcf.com/Article/details/gplqouqic.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnegyjana.sHtML

[A04] 判断变量类型
来源：http://www.m.share.epnwcf.com/Article/details/gwocnrvsj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.bbcook.cn/Article/details/gbyeiqiob.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fktsv.cn/Article/details/gyohhlrot.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.epnwcf.com/Article/details/guafxfjsb.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.bbcook.cn/Article/details/grgtneids.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.sjlbkw.cn/Article/details/guadgwzzk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.sjlbkw.cn/Article/details/guhyfiubh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.yfazqb.com/Article/details/gstztjqvy.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.yfazqb.com/Article/details/gjtprifce.sHtML

[A05] 整数除法与取模
来源：http://wap.tarul.cn/Article/details/gmfmaueqb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.epnwcf.com/Article/details/gbwqqfuym.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.epnwcf.com/Article/details/gbrgmexyv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/ghqwjvtzx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.vehdjk.com/Article/details/gmczgfqia.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.bbcook.cn/Article/details/gthrpluaz.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.vehdjk.com/Article/details/gzsnoxhgx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.vehdjk.com/Article/details/gyarezrtm.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/gatguejay.sHtML


<!-- 参考信息 -->