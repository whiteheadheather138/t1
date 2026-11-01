代发 wailian999

[U51] PHP：数组解构
来源：http://www.m.share.epnwcf.com/Article/details/gsyxvzmpd.sHtML

[$a, $b] = $arr;
来源：http://www.share.epnwcf.com/Article/details/gsoxordjr.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fktsv.cn/Article/details/gtyoyzpzl.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.yfazqb.com/Article/details/grydyrygf.sHtML

[U53] PHP：空合并运算符
来源：http://baike.bbcook.cn/Article/details/guwpcfjcj.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.yfazqb.com/Article/details/gyoadqbne.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fktsv.cn/Article/details/gspsuauzl.sHtML

$obj?->method()
来源：http://3g.bbcook.cn/Article/details/gobodgtlk.sHtML

[U55] PHP：match 表达式
来源：http://read.share.yfazqb.com/Article/details/grdqbvbag.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fktsv.cn/Article/details/gioojfgzp.sHtML

[U56] PHP：命名参数
来源：http://mobile.epnwcf.com/Article/details/gdvtlyfns.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/grlolfydu.sHtML

[U57] PHP：字符串插值
来源：http://wap.vehdjk.com/Article/details/gcjltyxzd.sHtML

"值: {$a}"
来源：http://m.share.fktsv.cn/Article/details/glvoaovjy.sHtML

[U58] PHP：数组三件套
来源：http://baike.epnwcf.com/Article/details/gxogcwazc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gmkocmomk.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.vehdjk.com/Article/details/gvyecdhvg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.yfazqb.com/Article/details/gwvcpgcst.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.yfazqb.com/Article/details/gmscrpnoz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.vehdjk.com/Article/details/gheotpctc.sHtML

[U61] PHP：正则
来源：http://www.blog.vehdjk.com/Article/details/gkinkpzem.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gfveamlae.sHtML

[U62] PHP：日期对象
来源：http://3g.vehdjk.com/Article/details/giumkswha.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.yfazqb.com/Article/details/gnuysnblq.sHtML

[U63] PHP：文件读写
来源：http://wap.vehdjk.com/Article/details/gulsqvfeu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.sjlbkw.cn/Article/details/ghmwwkjvr.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fktsv.cn/Article/details/gbhakotbq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.vehdjk.com/Article/details/gfxwfpmqk.sHtML

[U65] PHP：会话
来源：http://www.m.share.fktsv.cn/Article/details/gurhxmgmc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gobmxcmji.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.vehdjk.com/Article/details/gaifmtsnx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.sjlbkw.cn/Article/details/ghjdhqlcw.sHtML

[U67] PHP：处理文件上传
来源：http://blog.bbcook.cn/Article/details/goxjkiews.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.vehdjk.com/Article/details/ggiomklfq.sHtML

[U68] PHP：PDO 连接
来源：http://baike.epnwcf.com/Article/details/gpshtadub.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.epnwcf.com/Article/details/gsckclbro.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.yfazqb.com/Article/details/gmocbtfif.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.sjlbkw.cn/Article/details/gblpyaroq.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.sjlbkw.cn/Article/details/gbuqihtxg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.tarul.cn/Article/details/gqyijyxxb.sHtML

[U71] PHP：抛出异常
来源：http://wap.yfazqb.com/Article/details/geyzuqfkc.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.vehdjk.com/Article/details/gdtiyegeq.sHtML

[U72] PHP：写错误日志
来源：http://blog.tarul.cn/Article/details/gnlkagdvu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.bbcook.cn/Article/details/gbnjqjxsu.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.yfazqb.com/Article/details/gvumacwnq.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.yfazqb.com/Article/details/gwlkydkml.sHtML

[U74] PHP：读取环境变量
来源：http://baike.epnwcf.com/Article/details/ggqtvjsii.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.vehdjk.com/Article/details/gxphzjhgf.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.yfazqb.com/Article/details/gxpacsbtk.sHtML

composer require psr/container
来源：http://baike.vehdjk.com/Article/details/gojtlomxh.sHtML

[U76] PHP：简单路由
来源：http://blog.epnwcf.com/Article/details/gchroqqto.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.bbcook.cn/Article/details/guzogshne.sHtML

[U77] PHP：模板渲染
来源：http://m.share.sjlbkw.cn/Article/details/grsfrjkpq.sHtML

composer require twig/twig
来源：http://www.m.share.tarul.cn/Article/details/gmcnnqfyz.sHtML

[U78] PHP：单元测试
来源：http://wap.yfazqb.com/Article/details/geepepibo.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.yfazqb.com/Article/details/gshpmdfuq.sHtML

[U79] PHP：静态分析
来源：http://3g.sjlbkw.cn/Article/details/gtbjggcvs.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.yfazqb.com/Article/details/gfcpayaaq.sHtML

[U80] PHP：代码规范修复
来源：http://wap.tarul.cn/Article/details/grcdgdffj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.vehdjk.com/Article/details/gzuaahygv.sHtML

[U81] JS：初始化项目
来源：http://www.share.epnwcf.com/Article/details/gyvzahigq.sHtML

npm init -y;  npm i express
来源：http://read.share.fktsv.cn/Article/details/ggxqebehe.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.sjlbkw.cn/Article/details/gvziwbzej.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.bbcook.cn/Article/details/gkjcvztce.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.tarul.cn/Article/details/gncgbxgkv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.vehdjk.com/Article/details/gaarmktqv.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.yfazqb.com/Article/details/gdymnywef.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.vehdjk.com/Article/details/gbveqmscn.sHtML

[U85] JS：可选链
来源：http://blog.bbcook.cn/Article/details/gpbtbwuzj.sHtML

a?.b?.c
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfzlbnys.sHtML

[U86] JS：空值合并
来源：http://3g.tarul.cn/Article/details/giquyqifo.sHtML

a ?? b
来源：http://read.share.vehdjk.com/Article/details/gdpjqixis.sHtML

[U87] JS：解构默认值
来源：http://www.share.epnwcf.com/Article/details/ghmukqcgd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.epnwcf.com/Article/details/gyjexxhpa.sHtML

[U88] JS：对象展开合并
来源：http://baike.epnwcf.com/Article/details/giykuqtxu.sHtML

{ ...a, ...b }
来源：http://mobile.bbcook.cn/Article/details/gtbpwmatx.sHtML

[U89] JS：数组去重
来源：http://read.share.sjlbkw.cn/Article/details/glsoszwyi.sHtML

[...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/ghtwjrgwt.sHtML

[U90] JS：数字数组排序
来源：http://blog.bbcook.cn/Article/details/gjkdqcdum.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggymzmyqg.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.sjlbkw.cn/Article/details/gxdazrfdm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.vehdjk.com/Article/details/grqjogaus.sHtML

[U92] JS：深拷贝
来源：http://baike.sjlbkw.cn/Article/details/ggqueplvk.sHtML

structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/glkpihdkd.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.vehdjk.com/Article/details/guwmiktld.sHtML

`共 ${n} 条`
来源：http://www.blog.sjlbkw.cn/Article/details/gfeeyxgjr.sHtML

[U94] JS：箭头函数
来源：http://m.share.tarul.cn/Article/details/gtaplxsnl.sHtML

const double = x => x * 2;
来源：http://mobile.epnwcf.com/Article/details/gzwvfuzfb.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fktsv.cn/Article/details/gpqjbervu.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.vehdjk.com/Article/details/gcjrecnsh.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.bbcook.cn/Article/details/glgqmdlms.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fktsv.cn/Article/details/gphnhkwpo.sHtML

[U97] JS：并发请求
来源：http://www.blog.fktsv.cn/Article/details/gckcnsdup.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/gsketoifx.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gekajcnep.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.sjlbkw.cn/Article/details/gfwoviedk.sHtML

[U99] JS：事件监听
来源：http://3g.vehdjk.com/Article/details/gylrwqomm.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.vehdjk.com/Article/details/gyuyyvlod.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.epnwcf.com/Article/details/gquvruvhz.sHtML

document.querySelector(".item")
来源：http://www.blog.vehdjk.com/Article/details/gmfwmywde.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.vehdjk.com/Article/details/grcsorrsk.sHtML

el.classList.toggle("active")
来源：http://m.share.tarul.cn/Article/details/gmqgkrjqs.sHtML

[U102] JS：本地存储
来源：http://www.blog.vehdjk.com/Article/details/gjyeawupb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.tarul.cn/Article/details/gadgzkmip.sHtML

[U103] JS：定时器
来源：http://m.share.yfazqb.com/Article/details/glvvfuplp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.sjlbkw.cn/Article/details/gkuzomlzl.sHtML

[U104] JS：防抖
来源：http://read.share.yfazqb.com/Article/details/gtpvodfpk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gkgpsuepe.sHtML

[U105] JS：节流
来源：http://m.share.sjlbkw.cn/Article/details/gjbuxbfun.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fktsv.cn/Article/details/gahojkbhz.sHtML

[U106] JS：日期格式化
来源：http://m.share.yfazqb.com/Article/details/gchvadkbv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.tarul.cn/Article/details/gceczgzfp.sHtML

[U107] JS：数字千分位
来源：http://www.blog.vehdjk.com/Article/details/gejttgvfz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/gxdmmfurj.sHtML

[U108] JS：随机整数
来源：http://blog.yfazqb.com/Article/details/gcorylaoq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.vehdjk.com/Article/details/gmwrmbyej.sHtML

[U109] JS：数组分组
来源：http://mobile.yfazqb.com/Article/details/gjvdnxiqs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fktsv.cn/Article/details/gquixjpml.sHtML

[U110] JS：数组分块
来源：http://3g.epnwcf.com/Article/details/gktzadrdt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.yfazqb.com/Article/details/gcffomytl.sHtML

[U111] JS：对象转 Map
来源：http://www.share.yfazqb.com/Article/details/gyzfcllrg.sHtML

new Map(Object.entries(obj))
来源：http://mobile.vehdjk.com/Article/details/gvnuqbdph.sHtML

[U112] JS：字符串补位
来源：http://wap.sjlbkw.cn/Article/details/gtlocqzty.sHtML

"7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gzoghtems.sHtML

[U113] JS：正则替换全部
来源：http://m.share.tarul.cn/Article/details/gayjtnite.sHtML

s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gztorizbv.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.vehdjk.com/Article/details/gaaruslpv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fktsv.cn/Article/details/gjfipykjo.sHtML

[U115] JS：生成 UUID
来源：http://read.share.vehdjk.com/Article/details/gsoyqvpnj.sHtML

crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gtlaxsjgb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.sjlbkw.cn/Article/details/gytdsesca.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.vehdjk.com/Article/details/gqbhwdvtm.sHtML

[U117] JS：单元测试
来源：http://blog.bbcook.cn/Article/details/gneifyftw.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.yfazqb.com/Article/details/gtnbyjksh.sHtML

[U118] JS：开发服务器
来源：http://www.blog.vehdjk.com/Article/details/gieikfiel.sHtML

npm i -D vite;  npx vite
来源：http://www.share.sjlbkw.cn/Article/details/gxjvuitkc.sHtML

[U119] JS：生产构建
来源：http://mobile.yfazqb.com/Article/details/gfpzutkqv.sHtML

npx vite build
来源：http://m.share.sjlbkw.cn/Article/details/gjnrfkycx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.bbcook.cn/Article/details/gpctmcnna.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fktsv.cn/Article/details/giptnbxwx.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/giqbqnhpc.sHtML

统计汇总
来源：http://wap.fktsv.cn/Article/details/glmvqvwoh.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gwjdsgnwo.sHtML

按语言统计（条）：
来源：http://www.blog.bbcook.cn/Article/details/gebpiyfyu.sHtML

Python ......... 252
来源：http://www.blog.sjlbkw.cn/Article/details/gmtrotlwy.sHtML

PHP ............ 252
来源：http://wap.sjlbkw.cn/Article/details/gadypcudf.sHtML

JavaScript ..... 252
来源：http://blog.sjlbkw.cn/Article/details/gmmnfjkts.sHtML

TypeScript ..... 212
来源：http://wap.tarul.cn/Article/details/gyerclzoi.sHtML

Java ........... 212
来源：http://read.share.bbcook.cn/Article/details/gdedydbjo.sHtML

Go ............. 212
来源：http://www.share.yfazqb.com/Article/details/gdpsupmce.sHtML

Ruby ........... 212
来源：http://read.share.epnwcf.com/Article/details/gcxunjxtn.sHtML

C# ............. 212
来源：http://baike.sjlbkw.cn/Article/details/gwvgqcema.sHtML

C .............. 30
来源：http://wap.bbcook.cn/Article/details/gfwuxpwxc.sHtML

C++ ............ 30
来源：http://mobile.tarul.cn/Article/details/gspcxyxtb.sHtML

SQL ............ 90
来源：http://3g.bbcook.cn/Article/details/gjkuzykpk.sHtML

Bash ........... 80
来源：http://www.blog.bbcook.cn/Article/details/gooxfozor.sHtML

Kotlin ......... 15
来源：http://www.share.sjlbkw.cn/Article/details/gjhfsnsop.sHtML

Swift .......... 15
来源：http://read.share.yfazqb.com/Article/details/gxmwsksok.sHtML

Lua ............ 10
来源：http://m.share.vehdjk.com/Article/details/gfosypans.sHtML

Perl ........... 10
来源：http://blog.tarul.cn/Article/details/gnjbkqajm.sHtML

Scala .......... 10
来源：http://blog.bbcook.cn/Article/details/goralfqya.sHtML

------------------------------------
来源：http://blog.fktsv.cn/Article/details/gxcfcimwa.sHtML

合计 ........... 2106 条
来源：http://blog.yfazqb.com/Article/details/gbctbejjy.sHtML

按章节统计：
来源：http://www.share.yfazqb.com/Article/details/ghdrmxpdu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.epnwcf.com/Article/details/gzeymmrds.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.bbcook.cn/Article/details/glmeatfdg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.yfazqb.com/Article/details/gtdljgrnu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.bbcook.cn/Article/details/gnojnkchu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.yfazqb.com/Article/details/gbuxyufyg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.vehdjk.com/Article/details/gsakmilvt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.vehdjk.com/Article/details/gitrhyfhh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.epnwcf.com/Article/details/gctulpbsn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gcufsltfo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.sjlbkw.cn/Article/details/gfadnuvcc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gsmerfeds.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gbyqryhla.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.epnwcf.com/Article/details/gxizsmqci.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.vehdjk.com/Article/details/gniiuotuf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.sjlbkw.cn/Article/details/gprcuypwh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gijqalfrn.sHtML

Q SQL 专题                              90
来源：http://wap.yfazqb.com/Article/details/gsjbsdwts.sHtML

R Bash 专题                             80
来源：http://m.share.tarul.cn/Article/details/grjrzbibx.sHtML

S C / C++ 专题                          60
来源：http://3g.yfazqb.com/Article/details/gthkvnzor.sHtML

T 其他语言补充                          60
来源：http://www.blog.fktsv.cn/Article/details/gnekdnisc.sHtML

U 高频实用片段                         120
来源：http://m.share.vehdjk.com/Article/details/gqzgtrzbx.sHtML

------------------------------------
来源：http://3g.epnwcf.com/Article/details/gzxqhirmg.sHtML

合计                                  2106 条
来源：http://www.blog.fktsv.cn/Article/details/gajqysooc.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gukpvbfji.sHtML

使用提醒
来源：http://3g.tarul.cn/Article/details/gynoyeyay.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gapslmzes.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.vehdjk.com/Article/details/glfowaftn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.yfazqb.com/Article/details/gywyqqsyd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.vehdjk.com/Article/details/gyijtlmfw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.bbcook.cn/Article/details/gjhubdsek.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.yfazqb.com/Article/details/gcfiexmks.sHtML

—— 文件结束 ——
来源：http://3g.yfazqb.com/Article/details/gewsowqdd.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gmdjdxfsu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.epnwcf.com/Article/details/gzvwqfjzq.sHtML

Common Programming Examples Cheat Book
来源：http://wap.sjlbkw.cn/Article/details/gyywaqgyy.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gpycswurj.sHtML

【收录内容】
来源：http://blog.sjlbkw.cn/Article/details/gfnzfamvj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.vehdjk.com/Article/details/gfghwutme.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.epnwcf.com/Article/details/gqpkcuwpt.sHtML

SQL · Bash · C · C++
来源：http://wap.yfazqb.com/Article/details/gmunmbast.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.vehdjk.com/Article/details/gghbsayto.sHtML

【使用说明】
来源：http://blog.sjlbkw.cn/Article/details/glmvovork.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fktsv.cn/Article/details/guclrowuo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.yfazqb.com/Article/details/gcmlopsvb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.epnwcf.com/Article/details/gplmqfoqo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fktsv.cn/Article/details/gpwbxlzyx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fktsv.cn/Article/details/gsznlvsun.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.sjlbkw.cn/Article/details/groefechw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.sjlbkw.cn/Article/details/gjlavjjyy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.yfazqb.com/Article/details/gwhxauzht.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.sjlbkw.cn/Article/details/gfomuxhus.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.vehdjk.com/Article/details/gkpatfhlr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.sjlbkw.cn/Article/details/gbkxblvqb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.vehdjk.com/Article/details/gytuuiyea.sHtML

【文件统计】
来源：http://www.share.tarul.cn/Article/details/gpqgnjyrz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.yfazqb.com/Article/details/gvaurrdse.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.tarul.cn/Article/details/gufqjyxug.sHtML

目  录
来源：http://baike.sjlbkw.cn/Article/details/gqdstjbao.sHtML

--------------------------------------------------------------------------------
来源：http://baike.vehdjk.com/Article/details/gjgheplsc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.sjlbkw.cn/Article/details/gbjrxzrkg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.tarul.cn/Article/details/gwnnslgde.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.epnwcf.com/Article/details/geybufxol.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.vehdjk.com/Article/details/gpbmeqbaa.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fktsv.cn/Article/details/ghefcpemc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.yfazqb.com/Article/details/ghimxrzon.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.vehdjk.com/Article/details/gmmojpkbo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fktsv.cn/Article/details/gwsqhlhvt.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fktsv.cn/Article/details/gsomrxfbg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.bbcook.cn/Article/details/gidlrdmoi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gaaqrmrgm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fktsv.cn/Article/details/gugczxynz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.vehdjk.com/Article/details/gpfteshnx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.bbcook.cn/Article/details/ghwmojvtw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.bbcook.cn/Article/details/gqqropkhu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gpakawhnh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.vehdjk.com/Article/details/gelifhyfw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.tarul.cn/Article/details/gnftwiyvp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fktsv.cn/Article/details/gcxfeztie.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.bbcook.cn/Article/details/gzijmbqfp.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.sjlbkw.cn/Article/details/gzjisycri.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/glzhqhgrm.sHtML

A. 基础语法与类型
来源：http://blog.yfazqb.com/Article/details/gueptdtyn.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ggvatuerm.sHtML

[A01] Hello World
来源：http://m.share.fktsv.cn/Article/details/gqnzkyxyc.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.yfazqb.com/Article/details/giidvwddz.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.bbcook.cn/Article/details/gqxkzxpsr.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.yfazqb.com/Article/details/grpduzfnz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.tarul.cn/Article/details/glhsbvwgc.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.vehdjk.com/Article/details/gridxnxnu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.bbcook.cn/Article/details/glsadsger.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.tarul.cn/Article/details/guhpsdrhz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.vehdjk.com/Article/details/giexpdgay.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.tarul.cn/Article/details/gycpftokx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.bbcook.cn/Article/details/ggoozoygs.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.vehdjk.com/Article/details/ggnaejeeu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.yfazqb.com/Article/details/gdzuzcxcr.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fktsv.cn/Article/details/gyhxoboft.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.vehdjk.com/Article/details/gdolonbmj.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.tarul.cn/Article/details/gcfcctjrr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.yfazqb.com/Article/details/grjjpeywm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.tarul.cn/Article/details/gunerqhne.sHtML

[A03] 常量定义
来源：http://blog.epnwcf.com/Article/details/gvziogjif.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.yfazqb.com/Article/details/gclmhygmc.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gwtiapaqi.sHtML

JS:   const PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/ghpirtuut.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gusedjdbb.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gavkdtfuc.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.sjlbkw.cn/Article/details/gibakdryv.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fktsv.cn/Article/details/gdvppbcqp.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/ggobnzrvu.sHtML

[A04] 判断变量类型
来源：http://mobile.epnwcf.com/Article/details/gawybjbav.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.yfazqb.com/Article/details/gkzibpksc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.tarul.cn/Article/details/gslbuvptc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.vehdjk.com/Article/details/gbeiildom.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.epnwcf.com/Article/details/gdtixdtka.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.vehdjk.com/Article/details/grmmifvpq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.tarul.cn/Article/details/glazuiyhv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.vehdjk.com/Article/details/gmbjpdddz.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.yfazqb.com/Article/details/gpmvxzmow.sHtML

[A05] 整数除法与取模
来源：http://read.share.epnwcf.com/Article/details/gtqtdfpfs.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.bbcook.cn/Article/details/gwswawplg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fktsv.cn/Article/details/ghsbyrhwc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.epnwcf.com/Article/details/gpwxvtzpy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.vehdjk.com/Article/details/gqesdkkej.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gyyhyfgci.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.bbcook.cn/Article/details/gtdogjsxo.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/ghwlluheo.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.bbcook.cn/Article/details/gqnmaguhn.sHtML

[A06] 字符串转数字
来源：http://www.share.tarul.cn/Article/details/gpuwuntdm.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fktsv.cn/Article/details/gbrfbkjrm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.epnwcf.com/Article/details/gmqelrias.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fktsv.cn/Article/details/gfcmkqeku.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.epnwcf.com/Article/details/giffugmai.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.tarul.cn/Article/details/ghgcylnaq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.yfazqb.com/Article/details/goyqtvrgp.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.sjlbkw.cn/Article/details/gxykbbvtg.sHtML


<!-- 参考信息 -->