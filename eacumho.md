代发 wailian999

[U51] PHP：数组解构
来源：http://wap.sjlbkw.cn/Article/details/gjkfckxue.sHtML

[$a, $b] = $arr;
来源：http://baike.bbcook.cn/Article/details/gesotexle.sHtML

[U52] PHP：箭头函数
来源：http://baike.yfazqb.com/Article/details/gzjftmrdh.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.bbcook.cn/Article/details/gkwerdmgu.sHtML

[U53] PHP：空合并运算符
来源：http://baike.tarul.cn/Article/details/grcqcoljq.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.bbcook.cn/Article/details/gwzbashxu.sHtML

[U54] PHP：空安全调用
来源：http://baike.epnwcf.com/Article/details/gvogaawzh.sHtML

$obj?->method()
来源：http://www.share.vehdjk.com/Article/details/ghihsollr.sHtML

[U55] PHP：match 表达式
来源：http://blog.epnwcf.com/Article/details/gngygyejz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.sjlbkw.cn/Article/details/gwatyluru.sHtML

[U56] PHP：命名参数
来源：http://baike.sjlbkw.cn/Article/details/gqgwypzbd.sHtML

f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gsasifoco.sHtML

[U57] PHP：字符串插值
来源：http://3g.epnwcf.com/Article/details/ghngirxex.sHtML

"值: {$a}"
来源：http://www.blog.epnwcf.com/Article/details/gjlzyujis.sHtML

[U58] PHP：数组三件套
来源：http://read.share.vehdjk.com/Article/details/gsmyoxxag.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.epnwcf.com/Article/details/gizxbwjvu.sHtML

[U59] PHP：自定义排序
来源：http://baike.yfazqb.com/Article/details/githkydjw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.yfazqb.com/Article/details/gfrjosoej.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.bbcook.cn/Article/details/gulvevfmh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.yfazqb.com/Article/details/genndqcru.sHtML

[U61] PHP：正则
来源：http://read.share.bbcook.cn/Article/details/gfcvzbabd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.yfazqb.com/Article/details/gmpnapcsv.sHtML

[U62] PHP：日期对象
来源：http://www.share.epnwcf.com/Article/details/gtbbzjjxa.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.tarul.cn/Article/details/gqzjzpvsp.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.bbcook.cn/Article/details/gzxonmmjo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.vehdjk.com/Article/details/gkyfexxjr.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fktsv.cn/Article/details/gnhagncvm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.tarul.cn/Article/details/geninhegy.sHtML

[U65] PHP：会话
来源：http://baike.yfazqb.com/Article/details/gmooskmwx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gfiodkdap.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.yfazqb.com/Article/details/gwduztdej.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.epnwcf.com/Article/details/gwspnohgg.sHtML

[U67] PHP：处理文件上传
来源：http://blog.bbcook.cn/Article/details/gxqjynpbm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.yfazqb.com/Article/details/gezkpwgwu.sHtML

[U68] PHP：PDO 连接
来源：http://blog.vehdjk.com/Article/details/gnyrnteeo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.bbcook.cn/Article/details/gtfguzqfa.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.yfazqb.com/Article/details/gsofmlbzt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fktsv.cn/Article/details/gfjyfymxk.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.epnwcf.com/Article/details/grlkteuht.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.bbcook.cn/Article/details/gffyaymfp.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fktsv.cn/Article/details/govjppdpu.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.epnwcf.com/Article/details/gcwvpjgbz.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fktsv.cn/Article/details/gvihszagp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fktsv.cn/Article/details/gyxjcyecw.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.yfazqb.com/Article/details/ggcegnnsz.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fktsv.cn/Article/details/gvvhsodus.sHtML

[U74] PHP：读取环境变量
来源：http://blog.epnwcf.com/Article/details/gatmhhzsw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.vehdjk.com/Article/details/gqqrccxqg.sHtML

[U75] PHP：依赖注入
来源：http://mobile.yfazqb.com/Article/details/ghjgodryn.sHtML

composer require psr/container
来源：http://www.share.fktsv.cn/Article/details/gwhbpcuns.sHtML

[U76] PHP：简单路由
来源：http://baike.yfazqb.com/Article/details/gojrmasji.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fktsv.cn/Article/details/gymwrqxla.sHtML

[U77] PHP：模板渲染
来源：http://3g.fktsv.cn/Article/details/gmxinaxmp.sHtML

composer require twig/twig
来源：http://3g.sjlbkw.cn/Article/details/gmmbzkzuk.sHtML

[U78] PHP：单元测试
来源：http://m.share.bbcook.cn/Article/details/gejuwmtox.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.yfazqb.com/Article/details/gtrcyqgmt.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.vehdjk.com/Article/details/gioiwrewc.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.epnwcf.com/Article/details/gjwbmbzsp.sHtML

[U80] PHP：代码规范修复
来源：http://baike.vehdjk.com/Article/details/gqzbsmbly.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.tarul.cn/Article/details/gulgcxtvs.sHtML

[U81] JS：初始化项目
来源：http://blog.epnwcf.com/Article/details/gjissrmhv.sHtML

npm init -y;  npm i express
来源：http://mobile.yfazqb.com/Article/details/gbykiqsbo.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.epnwcf.com/Article/details/gqbhagqdu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.yfazqb.com/Article/details/gsvqmuieh.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.tarul.cn/Article/details/gribkkxse.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.yfazqb.com/Article/details/gkkxkhmxk.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.yfazqb.com/Article/details/gjrledbql.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.epnwcf.com/Article/details/gcdbhietm.sHtML

[U85] JS：可选链
来源：http://www.m.share.vehdjk.com/Article/details/gotjcwwtf.sHtML

a?.b?.c
来源：http://www.m.share.vehdjk.com/Article/details/gohpcfvvd.sHtML

[U86] JS：空值合并
来源：http://m.share.yfazqb.com/Article/details/gioxkjcbh.sHtML

a ?? b
来源：http://www.m.share.vehdjk.com/Article/details/gxzwkuzow.sHtML

[U87] JS：解构默认值
来源：http://baike.yfazqb.com/Article/details/glmvrhvri.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.bbcook.cn/Article/details/gdfzxtmwz.sHtML

[U88] JS：对象展开合并
来源：http://read.share.vehdjk.com/Article/details/gbyhdctyp.sHtML

{ ...a, ...b }
来源：http://www.blog.tarul.cn/Article/details/glioodqih.sHtML

[U89] JS：数组去重
来源：http://read.share.sjlbkw.cn/Article/details/gbgarnooa.sHtML

[...new Set(arr)]
来源：http://mobile.bbcook.cn/Article/details/giyhctlhi.sHtML

[U90] JS：数字数组排序
来源：http://baike.tarul.cn/Article/details/gnlslktma.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/gbidplumc.sHtML

[U91] JS：对象键值遍历
来源：http://wap.vehdjk.com/Article/details/goslsnpij.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.yfazqb.com/Article/details/gutfaymlm.sHtML

[U92] JS：深拷贝
来源：http://blog.bbcook.cn/Article/details/gqieegkqm.sHtML

structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gkbhlhyyz.sHtML

[U93] JS：模板字符串
来源：http://read.share.yfazqb.com/Article/details/gcljouuhz.sHtML

`共 ${n} 条`
来源：http://blog.fktsv.cn/Article/details/gukcyetie.sHtML

[U94] JS：箭头函数
来源：http://wap.bbcook.cn/Article/details/gswoncoff.sHtML

const double = x => x * 2;
来源：http://www.m.share.sjlbkw.cn/Article/details/givsxniyg.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.sjlbkw.cn/Article/details/gymqmtkyn.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.bbcook.cn/Article/details/gwsojlgzk.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.yfazqb.com/Article/details/gedbytjyd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/gcsenbusd.sHtML

[U97] JS：并发请求
来源：http://mobile.yfazqb.com/Article/details/gbjwhnidq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gxpuwvxrz.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fktsv.cn/Article/details/ghsppazom.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.sjlbkw.cn/Article/details/gpajjnipx.sHtML

[U99] JS：事件监听
来源：http://wap.sjlbkw.cn/Article/details/ggbuoyhgb.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fktsv.cn/Article/details/grggyupvy.sHtML

[U100] JS：DOM 查询
来源：http://blog.vehdjk.com/Article/details/ghjcgqusx.sHtML

document.querySelector(".item")
来源：http://www.blog.epnwcf.com/Article/details/gfalfwzwj.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.yfazqb.com/Article/details/gsihxfimx.sHtML

el.classList.toggle("active")
来源：http://read.share.bbcook.cn/Article/details/gspoczprf.sHtML

[U102] JS：本地存储
来源：http://www.share.epnwcf.com/Article/details/gcenzkfcc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.yfazqb.com/Article/details/gaekdwsnh.sHtML

[U103] JS：定时器
来源：http://m.share.epnwcf.com/Article/details/gvsogmvpc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.bbcook.cn/Article/details/gmveumlkl.sHtML

[U104] JS：防抖
来源：http://www.m.share.sjlbkw.cn/Article/details/galzajxyr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/gbijqdriq.sHtML

[U105] JS：节流
来源：http://www.share.yfazqb.com/Article/details/geetaghiy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.sjlbkw.cn/Article/details/gkvdeuxnk.sHtML

[U106] JS：日期格式化
来源：http://www.share.fktsv.cn/Article/details/ggcrguusx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.sjlbkw.cn/Article/details/gfzbepauq.sHtML

[U107] JS：数字千分位
来源：http://baike.sjlbkw.cn/Article/details/gzuyhweql.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.epnwcf.com/Article/details/gmlddxzyt.sHtML

[U108] JS：随机整数
来源：http://baike.sjlbkw.cn/Article/details/gefutjryh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.yfazqb.com/Article/details/glrlaqczs.sHtML

[U109] JS：数组分组
来源：http://www.share.tarul.cn/Article/details/grldwhxtc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.epnwcf.com/Article/details/ganhejvtq.sHtML

[U110] JS：数组分块
来源：http://3g.fktsv.cn/Article/details/gszvwtnfb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.yfazqb.com/Article/details/gnfpsopoe.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.tarul.cn/Article/details/grbjqdkkq.sHtML

new Map(Object.entries(obj))
来源：http://blog.fktsv.cn/Article/details/gepqtqvri.sHtML

[U112] JS：字符串补位
来源：http://wap.sjlbkw.cn/Article/details/gbybvngkr.sHtML

"7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gymfbaekz.sHtML

[U113] JS：正则替换全部
来源：http://read.share.yfazqb.com/Article/details/glwwwubrr.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gwyjmtupa.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fktsv.cn/Article/details/gwwqruiwp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.yfazqb.com/Article/details/glwtqeila.sHtML

[U115] JS：生成 UUID
来源：http://mobile.yfazqb.com/Article/details/gchtfykdp.sHtML

crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gcnyklmes.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fktsv.cn/Article/details/gylqiwjlx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.bbcook.cn/Article/details/gzhmqydxt.sHtML

[U117] JS：单元测试
来源：http://m.share.tarul.cn/Article/details/gzqntmvyw.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.sjlbkw.cn/Article/details/gkajvfcjg.sHtML

[U118] JS：开发服务器
来源：http://blog.fktsv.cn/Article/details/gzpdrtmjw.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fktsv.cn/Article/details/gpafzdxza.sHtML

[U119] JS：生产构建
来源：http://www.blog.bbcook.cn/Article/details/gczvcsciq.sHtML

npx vite build
来源：http://www.share.fktsv.cn/Article/details/guwfzanow.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.tarul.cn/Article/details/golukjpap.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.yfazqb.com/Article/details/gltmpzcjt.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbhbzxqmc.sHtML

统计汇总
来源：http://read.share.vehdjk.com/Article/details/gmdufddox.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gukzbmman.sHtML

按语言统计（条）：
来源：http://blog.epnwcf.com/Article/details/gyobxpsug.sHtML

Python ......... 252
来源：http://read.share.fktsv.cn/Article/details/gatprgwdv.sHtML

PHP ............ 252
来源：http://m.share.bbcook.cn/Article/details/grjpseifx.sHtML

JavaScript ..... 252
来源：http://m.share.epnwcf.com/Article/details/glwwvsboj.sHtML

TypeScript ..... 212
来源：http://m.share.epnwcf.com/Article/details/gigvcsaoc.sHtML

Java ........... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/guybyymbk.sHtML

Go ............. 212
来源：http://www.blog.tarul.cn/Article/details/gelzzairl.sHtML

Ruby ........... 212
来源：http://read.share.vehdjk.com/Article/details/gtecoxpgt.sHtML

C# ............. 212
来源：http://mobile.tarul.cn/Article/details/geusgfyaw.sHtML

C .............. 30
来源：http://blog.tarul.cn/Article/details/gulppqyma.sHtML

C++ ............ 30
来源：http://www.share.fktsv.cn/Article/details/gzrrdibam.sHtML

SQL ............ 90
来源：http://mobile.bbcook.cn/Article/details/gnnhdrslc.sHtML

Bash ........... 80
来源：http://wap.vehdjk.com/Article/details/gpohhcgjl.sHtML

Kotlin ......... 15
来源：http://m.share.epnwcf.com/Article/details/ggnmsygra.sHtML

Swift .......... 15
来源：http://www.share.tarul.cn/Article/details/gytcftbmf.sHtML

Lua ............ 10
来源：http://wap.bbcook.cn/Article/details/glyxvgptl.sHtML

Perl ........... 10
来源：http://www.share.fktsv.cn/Article/details/gpkbrgqwv.sHtML

Scala .......... 10
来源：http://m.share.vehdjk.com/Article/details/ghvlvdjip.sHtML

------------------------------------
来源：http://wap.yfazqb.com/Article/details/gyupalsqm.sHtML

合计 ........... 2106 条
来源：http://www.m.share.vehdjk.com/Article/details/geukxfejm.sHtML

按章节统计：
来源：http://www.m.share.fktsv.cn/Article/details/gkqfbctds.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.sjlbkw.cn/Article/details/glypaaakf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.yfazqb.com/Article/details/grvxvlmwh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.epnwcf.com/Article/details/gptkxhjec.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.epnwcf.com/Article/details/gujlkcfqx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.yfazqb.com/Article/details/grwedmkun.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.bbcook.cn/Article/details/gnegfrnyg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.bbcook.cn/Article/details/gwjhxtmqg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.tarul.cn/Article/details/gyjflcqbc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gqewtnase.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.epnwcf.com/Article/details/gjgwfohea.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/gzhryepfd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gzuexkhry.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.bbcook.cn/Article/details/gerstameo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.yfazqb.com/Article/details/garimnkyy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.tarul.cn/Article/details/gcsblnjac.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/giyhvahnr.sHtML

Q SQL 专题                              90
来源：http://mobile.sjlbkw.cn/Article/details/gajgmwotl.sHtML

R Bash 专题                             80
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvhgwkqt.sHtML

S C / C++ 专题                          60
来源：http://blog.epnwcf.com/Article/details/gjpzbixgk.sHtML

T 其他语言补充                          60
来源：http://3g.sjlbkw.cn/Article/details/gadzzbmyd.sHtML

U 高频实用片段                         120
来源：http://mobile.bbcook.cn/Article/details/gnltnysop.sHtML

------------------------------------
来源：http://m.share.tarul.cn/Article/details/gxodxovqm.sHtML

合计                                  2106 条
来源：http://baike.vehdjk.com/Article/details/gkwftkpmt.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fktsv.cn/Article/details/grnhibwxo.sHtML

使用提醒
来源：http://3g.bbcook.cn/Article/details/gzyhgkcns.sHtML

--------------------------------------------------------------------------------
来源：http://baike.bbcook.cn/Article/details/gtntxfyah.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.vehdjk.com/Article/details/gqgtditbm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.yfazqb.com/Article/details/gdtrcaoca.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.vehdjk.com/Article/details/guahcmhqy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.bbcook.cn/Article/details/ghzukvilm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fktsv.cn/Article/details/gzwypigie.sHtML

—— 文件结束 ——
来源：http://www.blog.epnwcf.com/Article/details/gkiyqytsq.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gtwnokjig.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.sjlbkw.cn/Article/details/gugccfkjj.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.yfazqb.com/Article/details/gcjqxtwzf.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gmnulndhm.sHtML

【收录内容】
来源：http://m.share.vehdjk.com/Article/details/guwsvtnmf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.yfazqb.com/Article/details/gntifzmly.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.sjlbkw.cn/Article/details/gysnkfcti.sHtML

SQL · Bash · C · C++
来源：http://m.share.bbcook.cn/Article/details/gploqqlvp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fktsv.cn/Article/details/gxeccoded.sHtML

【使用说明】
来源：http://www.blog.bbcook.cn/Article/details/gdvkzizku.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.epnwcf.com/Article/details/gggxnlbha.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.bbcook.cn/Article/details/gcknoqpus.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.bbcook.cn/Article/details/gnyrqiicy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.yfazqb.com/Article/details/gljhgurxp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.yfazqb.com/Article/details/gvmwgbkwk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.tarul.cn/Article/details/gvavbrmmu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.epnwcf.com/Article/details/gibomupvd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.epnwcf.com/Article/details/gucgmsgky.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.tarul.cn/Article/details/glrckfkge.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.vehdjk.com/Article/details/gkvzbekmm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.vehdjk.com/Article/details/gbnzkjxbg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.bbcook.cn/Article/details/gfvwulwhm.sHtML

【文件统计】
来源：http://3g.epnwcf.com/Article/details/gluwnxiub.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.tarul.cn/Article/details/gdfmuhnlb.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.tarul.cn/Article/details/gjhqznbum.sHtML

目  录
来源：http://mobile.vehdjk.com/Article/details/gmnzbgpwf.sHtML

--------------------------------------------------------------------------------
来源：http://3g.tarul.cn/Article/details/gfpihaqsg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fktsv.cn/Article/details/gfkueouqm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.sjlbkw.cn/Article/details/gxdnxdwpl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fktsv.cn/Article/details/gsinewlmx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.yfazqb.com/Article/details/gejnzxeea.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.vehdjk.com/Article/details/grdambzog.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.tarul.cn/Article/details/gfkhvxgzy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.vehdjk.com/Article/details/gexfkuxeo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.vehdjk.com/Article/details/gtwfwlcrv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/gehznwlvy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.epnwcf.com/Article/details/gnmfnndts.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/gtshoptcc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/ghrtfspwu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.yfazqb.com/Article/details/gpqsyzhmo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.yfazqb.com/Article/details/gekpnboem.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.tarul.cn/Article/details/gepsuhyxa.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gmsyqnzrq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.yfazqb.com/Article/details/guscvbcot.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.sjlbkw.cn/Article/details/ggvefskrc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fktsv.cn/Article/details/gwuovtkvu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.yfazqb.com/Article/details/ghbauudko.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.tarul.cn/Article/details/gfywakkcy.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gpwjmvrpn.sHtML

A. 基础语法与类型
来源：http://mobile.vehdjk.com/Article/details/gnwvazogs.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gjtrxynqr.sHtML

[A01] Hello World
来源：http://www.blog.vehdjk.com/Article/details/gcabkqjnf.sHtML

Py:   print("Hello, World!")
来源：http://read.share.epnwcf.com/Article/details/gbrgqyeiq.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.tarul.cn/Article/details/gvkusjqrg.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.vehdjk.com/Article/details/gbtewhvgv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.vehdjk.com/Article/details/gculmpjst.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.bbcook.cn/Article/details/gmsppzmrb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fktsv.cn/Article/details/glkcpjxgo.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.bbcook.cn/Article/details/gfnuqcsiw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.tarul.cn/Article/details/gqvnwiqqf.sHtML

[A02] 变量声明与赋值
来源：http://3g.sjlbkw.cn/Article/details/glglrdmcx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.epnwcf.com/Article/details/ghjszswkl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.epnwcf.com/Article/details/gwcdrgfyt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.yfazqb.com/Article/details/gtgdjshlb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.vehdjk.com/Article/details/gfujejvji.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.sjlbkw.cn/Article/details/gwrgkvglp.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.bbcook.cn/Article/details/gbwpjsolw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.epnwcf.com/Article/details/grkrcqvxy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.yfazqb.com/Article/details/gpcmprhsl.sHtML

[A03] 常量定义
来源：http://3g.tarul.cn/Article/details/gightyjkl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.bbcook.cn/Article/details/gmdtqhjpn.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gphxdwdgg.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gbpcjgjvs.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.vehdjk.com/Article/details/giymhdeen.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gdyhtmrey.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fktsv.cn/Article/details/ghmtndfej.sHtML

Ruby: PI = 3.14159
来源：http://m.share.vehdjk.com/Article/details/guytwmbdv.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gakfvejaf.sHtML

[A04] 判断变量类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzjltwtp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.vehdjk.com/Article/details/gukjllwab.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.bbcook.cn/Article/details/ggqtsybui.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.vehdjk.com/Article/details/gjphjxfyr.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.epnwcf.com/Article/details/gsknqohru.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.vehdjk.com/Article/details/gujxgpebw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.epnwcf.com/Article/details/gqezzijps.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.vehdjk.com/Article/details/gbwiswlxq.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.sjlbkw.cn/Article/details/grjjrhglf.sHtML

[A05] 整数除法与取模
来源：http://www.share.epnwcf.com/Article/details/gmguyrpkt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fktsv.cn/Article/details/ginnneocz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fktsv.cn/Article/details/gruhgyoon.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gskipvzci.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.bbcook.cn/Article/details/ggvindfjd.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.epnwcf.com/Article/details/galekdhtc.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/gvytfqxmw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/gtjewczwl.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gytsqcpja.sHtML

[A06] 字符串转数字
来源：http://read.share.yfazqb.com/Article/details/gathncerx.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.yfazqb.com/Article/details/gbounqwln.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.vehdjk.com/Article/details/ggpjfuvqv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fktsv.cn/Article/details/gvbnxbeos.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.epnwcf.com/Article/details/ghonswcpr.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fktsv.cn/Article/details/gojffhawk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.yfazqb.com/Article/details/gthdmixnk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.vehdjk.com/Article/details/gsxdgrfob.sHtML


<!-- 参考信息 -->