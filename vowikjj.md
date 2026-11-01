代发 wailian999

[U51] PHP：数组解构
来源：http://m.share.sjlbkw.cn/Article/details/gqsatcgue.sHtML

[$a, $b] = $arr;
来源：http://3g.sjlbkw.cn/Article/details/gncdpszxo.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.tarul.cn/Article/details/gknuoiqti.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.sjlbkw.cn/Article/details/gqylszbfz.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.vehdjk.com/Article/details/gzxmbrjvu.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.bbcook.cn/Article/details/gcjcbzxgk.sHtML

[U54] PHP：空安全调用
来源：http://3g.fktsv.cn/Article/details/gevttyczt.sHtML

$obj?->method()
来源：http://www.blog.sjlbkw.cn/Article/details/glpewvzuq.sHtML

[U55] PHP：match 表达式
来源：http://read.share.epnwcf.com/Article/details/ghnwuttyv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.yfazqb.com/Article/details/gwmfzxkvl.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.epnwcf.com/Article/details/gvafrkwzf.sHtML

f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/ggbynxnbx.sHtML

[U57] PHP：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gqatknskn.sHtML

"值: {$a}"
来源：http://baike.tarul.cn/Article/details/ggwvvbrnt.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.sjlbkw.cn/Article/details/gtdaaseng.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.epnwcf.com/Article/details/gxcjztirb.sHtML

[U59] PHP：自定义排序
来源：http://read.share.epnwcf.com/Article/details/gtgkrgihe.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fktsv.cn/Article/details/gprnfpmuw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.vehdjk.com/Article/details/ghcubbtqv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.epnwcf.com/Article/details/gpoaektje.sHtML

[U61] PHP：正则
来源：http://www.share.vehdjk.com/Article/details/gsvjgjssc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.epnwcf.com/Article/details/gyqbtdjae.sHtML

[U62] PHP：日期对象
来源：http://baike.vehdjk.com/Article/details/gzkpdclvc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.sjlbkw.cn/Article/details/gjtdcfplq.sHtML

[U63] PHP：文件读写
来源：http://mobile.vehdjk.com/Article/details/gdpvmwwzc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.bbcook.cn/Article/details/gyfipcogc.sHtML

[U64] PHP：目录遍历
来源：http://baike.epnwcf.com/Article/details/gidatjzlk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fktsv.cn/Article/details/gbrtyhcls.sHtML

[U65] PHP：会话
来源：http://baike.bbcook.cn/Article/details/gfgvqzpsw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.yfazqb.com/Article/details/gejddpuws.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.sjlbkw.cn/Article/details/gmdhblylj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.vehdjk.com/Article/details/gzcflscxg.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.yfazqb.com/Article/details/goiiqyioe.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.sjlbkw.cn/Article/details/gqalmfrpv.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.epnwcf.com/Article/details/gibmdeodo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fktsv.cn/Article/details/glhyezxbu.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.vehdjk.com/Article/details/getqetkjx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.sjlbkw.cn/Article/details/gjxtoyjdn.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.tarul.cn/Article/details/gpsdgtcus.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.epnwcf.com/Article/details/ghiyjjxpw.sHtML

[U71] PHP：抛出异常
来源：http://read.share.bbcook.cn/Article/details/ghskxzwsd.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.bbcook.cn/Article/details/gmywfmstg.sHtML

[U72] PHP：写错误日志
来源：http://mobile.yfazqb.com/Article/details/gqzhedyjg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.yfazqb.com/Article/details/gcawuvudl.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.epnwcf.com/Article/details/gwmkzodui.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.epnwcf.com/Article/details/gehcjhrvg.sHtML

[U74] PHP：读取环境变量
来源：http://wap.vehdjk.com/Article/details/gtaszodkk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.bbcook.cn/Article/details/gjjjwqlzp.sHtML

[U75] PHP：依赖注入
来源：http://blog.fktsv.cn/Article/details/gqinmevil.sHtML

composer require psr/container
来源：http://blog.sjlbkw.cn/Article/details/gnixrpqwd.sHtML

[U76] PHP：简单路由
来源：http://read.share.epnwcf.com/Article/details/gjtdbfped.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.epnwcf.com/Article/details/gqsyelgoe.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fktsv.cn/Article/details/gjimxnlvj.sHtML

composer require twig/twig
来源：http://baike.sjlbkw.cn/Article/details/gkkmuvfhz.sHtML

[U78] PHP：单元测试
来源：http://mobile.sjlbkw.cn/Article/details/gwzecjcdp.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.tarul.cn/Article/details/gvmemxvzx.sHtML

[U79] PHP：静态分析
来源：http://3g.fktsv.cn/Article/details/gfidvjvdf.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.vehdjk.com/Article/details/gxcgefcmu.sHtML

[U80] PHP：代码规范修复
来源：http://baike.epnwcf.com/Article/details/gubdyvsvx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.vehdjk.com/Article/details/ghpvsrnhe.sHtML

[U81] JS：初始化项目
来源：http://mobile.sjlbkw.cn/Article/details/gnfydhdys.sHtML

npm init -y;  npm i express
来源：http://baike.sjlbkw.cn/Article/details/gbumaixfg.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fktsv.cn/Article/details/gevbiihzm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fktsv.cn/Article/details/gwqgnwtan.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.epnwcf.com/Article/details/gvgaxkjee.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.tarul.cn/Article/details/gyozcytvm.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.sjlbkw.cn/Article/details/gsghfisrg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.yfazqb.com/Article/details/gcvcnghtj.sHtML

[U85] JS：可选链
来源：http://wap.sjlbkw.cn/Article/details/gqwngelbr.sHtML

a?.b?.c
来源：http://m.share.bbcook.cn/Article/details/grbawvofu.sHtML

[U86] JS：空值合并
来源：http://baike.yfazqb.com/Article/details/gyyjjtsev.sHtML

a ?? b
来源：http://wap.yfazqb.com/Article/details/gsvauyqoi.sHtML

[U87] JS：解构默认值
来源：http://mobile.fktsv.cn/Article/details/glkxmjjmg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.bbcook.cn/Article/details/gvaxsjgzo.sHtML

[U88] JS：对象展开合并
来源：http://baike.fktsv.cn/Article/details/gttmzcmiz.sHtML

{ ...a, ...b }
来源：http://www.m.share.vehdjk.com/Article/details/gmsmizplr.sHtML

[U89] JS：数组去重
来源：http://blog.vehdjk.com/Article/details/goxucahpx.sHtML

[...new Set(arr)]
来源：http://blog.vehdjk.com/Article/details/gvntwecyy.sHtML

[U90] JS：数字数组排序
来源：http://m.share.vehdjk.com/Article/details/gghtppkwz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/gnuahngly.sHtML

[U91] JS：对象键值遍历
来源：http://wap.epnwcf.com/Article/details/gcrdojaxd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.yfazqb.com/Article/details/gtjwpcwkt.sHtML

[U92] JS：深拷贝
来源：http://mobile.sjlbkw.cn/Article/details/grbxmipvw.sHtML

structuredClone(obj)
来源：http://3g.tarul.cn/Article/details/gmwlstlpg.sHtML

[U93] JS：模板字符串
来源：http://m.share.vehdjk.com/Article/details/gxbodriyo.sHtML

`共 ${n} 条`
来源：http://read.share.tarul.cn/Article/details/ghkmtogjh.sHtML

[U94] JS：箭头函数
来源：http://3g.tarul.cn/Article/details/gnmhobjdo.sHtML

const double = x => x * 2;
来源：http://mobile.tarul.cn/Article/details/gviakilzg.sHtML

[U95] JS：Promise 包装
来源：http://www.share.epnwcf.com/Article/details/gzctcrcmd.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.tarul.cn/Article/details/gadmfewux.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.epnwcf.com/Article/details/gzwcoobpr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/gswwtuhls.sHtML

[U97] JS：并发请求
来源：http://wap.sjlbkw.cn/Article/details/glasygwuk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/gwtoywmoi.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.bbcook.cn/Article/details/gmvkbbncc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.yfazqb.com/Article/details/gziifezpw.sHtML

[U99] JS：事件监听
来源：http://mobile.yfazqb.com/Article/details/ggiemnevb.sHtML

el.addEventListener("click", e => {})
来源：http://blog.tarul.cn/Article/details/gmdashbmv.sHtML

[U100] JS：DOM 查询
来源：http://wap.bbcook.cn/Article/details/gtxlbrlzo.sHtML

document.querySelector(".item")
来源：http://www.blog.yfazqb.com/Article/details/gkbslxfnu.sHtML

[U101] JS：classList 操作
来源：http://read.share.epnwcf.com/Article/details/gachqxvoe.sHtML

el.classList.toggle("active")
来源：http://blog.vehdjk.com/Article/details/ggghvwfam.sHtML

[U102] JS：本地存储
来源：http://3g.epnwcf.com/Article/details/gblcwcyzn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.tarul.cn/Article/details/gohmdphij.sHtML

[U103] JS：定时器
来源：http://3g.tarul.cn/Article/details/gyewrmpvl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.epnwcf.com/Article/details/gnnrhawmg.sHtML

[U104] JS：防抖
来源：http://www.m.share.epnwcf.com/Article/details/gfotarpyi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/gzcncnkiu.sHtML

[U105] JS：节流
来源：http://m.share.fktsv.cn/Article/details/ghrkgjarb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.vehdjk.com/Article/details/gpfqbxivj.sHtML

[U106] JS：日期格式化
来源：http://baike.yfazqb.com/Article/details/gvofpjcyl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fktsv.cn/Article/details/gofgbgpqj.sHtML

[U107] JS：数字千分位
来源：http://wap.vehdjk.com/Article/details/gjgxuvive.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.sjlbkw.cn/Article/details/gfedwiyas.sHtML

[U108] JS：随机整数
来源：http://m.share.vehdjk.com/Article/details/gmoykodrk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.vehdjk.com/Article/details/gznmiigcx.sHtML

[U109] JS：数组分组
来源：http://www.share.fktsv.cn/Article/details/gwxcoeeaq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.vehdjk.com/Article/details/gfglypeks.sHtML

[U110] JS：数组分块
来源：http://www.share.bbcook.cn/Article/details/gareghlvp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.sjlbkw.cn/Article/details/geboyfnoz.sHtML

[U111] JS：对象转 Map
来源：http://baike.sjlbkw.cn/Article/details/gmbnzdrby.sHtML

new Map(Object.entries(obj))
来源：http://wap.tarul.cn/Article/details/ggvnzqqzl.sHtML

[U112] JS：字符串补位
来源：http://wap.tarul.cn/Article/details/gdwvlhcvf.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gaawzfewo.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fktsv.cn/Article/details/gzsnbldbp.sHtML

s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gstnoryoe.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.vehdjk.com/Article/details/gtytzhliy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.vehdjk.com/Article/details/gistfgsij.sHtML

[U115] JS：生成 UUID
来源：http://3g.bbcook.cn/Article/details/gbucfasyf.sHtML

crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gvducvtdd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.bbcook.cn/Article/details/gdjnprqnj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fktsv.cn/Article/details/grqlnyqiq.sHtML

[U117] JS：单元测试
来源：http://read.share.tarul.cn/Article/details/gigdvxvkl.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.vehdjk.com/Article/details/gdhxlowfy.sHtML

[U118] JS：开发服务器
来源：http://mobile.vehdjk.com/Article/details/gxbrwlbkc.sHtML

npm i -D vite;  npx vite
来源：http://wap.fktsv.cn/Article/details/gbudemejo.sHtML

[U119] JS：生产构建
来源：http://wap.tarul.cn/Article/details/gcgmyzuhu.sHtML

npx vite build
来源：http://baike.yfazqb.com/Article/details/gkbmxfmnd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.yfazqb.com/Article/details/gjdashwfh.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fktsv.cn/Article/details/gmxzxenns.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gtmhglifs.sHtML

统计汇总
来源：http://www.blog.sjlbkw.cn/Article/details/ghwrrlmbw.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gfwmzymuk.sHtML

按语言统计（条）：
来源：http://m.share.yfazqb.com/Article/details/ghulejzch.sHtML

Python ......... 252
来源：http://3g.bbcook.cn/Article/details/gdxeelzrj.sHtML

PHP ............ 252
来源：http://www.share.epnwcf.com/Article/details/gfajbzsop.sHtML

JavaScript ..... 252
来源：http://read.share.fktsv.cn/Article/details/gutadyopk.sHtML

TypeScript ..... 212
来源：http://baike.fktsv.cn/Article/details/gvvzohtpz.sHtML

Java ........... 212
来源：http://blog.yfazqb.com/Article/details/gzvyilqau.sHtML

Go ............. 212
来源：http://baike.bbcook.cn/Article/details/gzdrfzmau.sHtML

Ruby ........... 212
来源：http://read.share.vehdjk.com/Article/details/gzpxjpnxm.sHtML

C# ............. 212
来源：http://read.share.yfazqb.com/Article/details/gqkexxany.sHtML

C .............. 30
来源：http://blog.yfazqb.com/Article/details/grbyawctx.sHtML

C++ ............ 30
来源：http://www.blog.bbcook.cn/Article/details/glnffrlyl.sHtML

SQL ............ 90
来源：http://wap.yfazqb.com/Article/details/gzuvhlxov.sHtML

Bash ........... 80
来源：http://3g.vehdjk.com/Article/details/gxfvimxyr.sHtML

Kotlin ......... 15
来源：http://www.m.share.tarul.cn/Article/details/gyveqcezv.sHtML

Swift .......... 15
来源：http://read.share.epnwcf.com/Article/details/gltukfzfv.sHtML

Lua ............ 10
来源：http://www.blog.yfazqb.com/Article/details/gvoyeuyue.sHtML

Perl ........... 10
来源：http://3g.tarul.cn/Article/details/gjsfntsti.sHtML

Scala .......... 10
来源：http://www.share.bbcook.cn/Article/details/gxbbtyaiy.sHtML

------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gsufrzfeh.sHtML

合计 ........... 2106 条
来源：http://www.share.yfazqb.com/Article/details/glfmkakmk.sHtML

按章节统计：
来源：http://blog.yfazqb.com/Article/details/gagkgnyfw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.vehdjk.com/Article/details/gjvqnkmgt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.vehdjk.com/Article/details/gwhwbjiyv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.sjlbkw.cn/Article/details/gkhlekpyy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.vehdjk.com/Article/details/ggmfpobvv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.bbcook.cn/Article/details/gvuusinbf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.tarul.cn/Article/details/gpfhpsuht.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.tarul.cn/Article/details/gbpwrzxmm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fktsv.cn/Article/details/gsbjqfgkd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/gtlgftsuq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.epnwcf.com/Article/details/gmlcvjaef.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gnfomvzxb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gajpobawi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gyfzeqtes.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.sjlbkw.cn/Article/details/gtnsnpdzh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.epnwcf.com/Article/details/glflinbbq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/gexvmkamw.sHtML

Q SQL 专题                              90
来源：http://wap.vehdjk.com/Article/details/grgxiavgn.sHtML

R Bash 专题                             80
来源：http://read.share.yfazqb.com/Article/details/gwuxgbgxv.sHtML

S C / C++ 专题                          60
来源：http://3g.tarul.cn/Article/details/gmtksrwrm.sHtML

T 其他语言补充                          60
来源：http://www.share.sjlbkw.cn/Article/details/grwdghsrb.sHtML

U 高频实用片段                         120
来源：http://mobile.bbcook.cn/Article/details/gftxsulho.sHtML

------------------------------------
来源：http://www.blog.tarul.cn/Article/details/gfgdiatdw.sHtML

合计                                  2106 条
来源：http://m.share.sjlbkw.cn/Article/details/gndtwyjba.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqzethwn.sHtML

使用提醒
来源：http://m.share.tarul.cn/Article/details/gkmruenmb.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.epnwcf.com/Article/details/gknwjsqlr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.yfazqb.com/Article/details/glhqfbhks.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.tarul.cn/Article/details/gfogkslet.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.tarul.cn/Article/details/gpubpkpvi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.epnwcf.com/Article/details/gxcrzqwxn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fktsv.cn/Article/details/ggbaenoyv.sHtML

—— 文件结束 ——
来源：http://m.share.yfazqb.com/Article/details/ghyjhemxt.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gebebtifk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.bbcook.cn/Article/details/gogrsnwod.sHtML

Common Programming Examples Cheat Book
来源：http://wap.yfazqb.com/Article/details/golvrrdvu.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gtufbonbx.sHtML

【收录内容】
来源：http://3g.yfazqb.com/Article/details/ghtfjvuxo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fktsv.cn/Article/details/gmaiuqnrz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.sjlbkw.cn/Article/details/gskblzclj.sHtML

SQL · Bash · C · C++
来源：http://wap.sjlbkw.cn/Article/details/gxmssixyy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fktsv.cn/Article/details/gahftimkt.sHtML

【使用说明】
来源：http://baike.tarul.cn/Article/details/ggweirywc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.epnwcf.com/Article/details/gdjedkoet.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.yfazqb.com/Article/details/gkxvdzzyh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fktsv.cn/Article/details/gsjekpkaz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.tarul.cn/Article/details/gzyiwzzqf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.vehdjk.com/Article/details/gdteaodjj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.yfazqb.com/Article/details/gkbeungbs.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.bbcook.cn/Article/details/gwndkqezu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fktsv.cn/Article/details/gbdpchryp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.epnwcf.com/Article/details/gjuiyepwj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.tarul.cn/Article/details/gxsbkuxla.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.epnwcf.com/Article/details/gbwwmpadc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.sjlbkw.cn/Article/details/gadvmhaxl.sHtML

【文件统计】
来源：http://3g.sjlbkw.cn/Article/details/gnrxaljxf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fktsv.cn/Article/details/gcyomxzlr.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/goznbrbtb.sHtML

目  录
来源：http://www.share.vehdjk.com/Article/details/gtrdrzbgj.sHtML

--------------------------------------------------------------------------------
来源：http://wap.epnwcf.com/Article/details/gsosqsyml.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.vehdjk.com/Article/details/gvpzwkrjr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.yfazqb.com/Article/details/gkbcwnkxq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.yfazqb.com/Article/details/gcjjhnfmo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.epnwcf.com/Article/details/gpjieitug.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.yfazqb.com/Article/details/gcrftsegt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.sjlbkw.cn/Article/details/gamnfbwhy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.tarul.cn/Article/details/gaximmcup.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.tarul.cn/Article/details/gbabrdfbq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gdvftenfj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fktsv.cn/Article/details/gyybrvxtn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/gpbuhtcen.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/gqsarfjoo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gcgssckkj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.epnwcf.com/Article/details/gbsmjghzl.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.epnwcf.com/Article/details/gknsbfseb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/gliylhtvi.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.tarul.cn/Article/details/gmhfnvxtt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.yfazqb.com/Article/details/gxgpicsdt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.epnwcf.com/Article/details/gtaazjzez.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.epnwcf.com/Article/details/gosypbuti.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.vehdjk.com/Article/details/gcffuvwht.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gwbcsbwki.sHtML

A. 基础语法与类型
来源：http://www.share.fktsv.cn/Article/details/gntvoismv.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/guaoxkeva.sHtML

[A01] Hello World
来源：http://www.blog.bbcook.cn/Article/details/gbzuzibca.sHtML

Py:   print("Hello, World!")
来源：http://baike.tarul.cn/Article/details/gtyvgcgdy.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.sjlbkw.cn/Article/details/gqptitxmt.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fktsv.cn/Article/details/gkhygjpab.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.yfazqb.com/Article/details/gzikyonvx.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.tarul.cn/Article/details/gggknievu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgiqhizg.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.sjlbkw.cn/Article/details/gjxqyzksg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.epnwcf.com/Article/details/gnflhlacx.sHtML

[A02] 变量声明与赋值
来源：http://wap.epnwcf.com/Article/details/gojajfmtt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.bbcook.cn/Article/details/gqdpzphaw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.yfazqb.com/Article/details/gykxzoxpm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.vehdjk.com/Article/details/ghsspvfxk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.bbcook.cn/Article/details/gwqkqmndw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/ghmebijly.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.bbcook.cn/Article/details/gxqxyakzb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.sjlbkw.cn/Article/details/gexwdapef.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.tarul.cn/Article/details/gnfvjdmxu.sHtML

[A03] 常量定义
来源：http://3g.yfazqb.com/Article/details/gvsawtdym.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.bbcook.cn/Article/details/gaxgkhrdz.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/ghboyddxb.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gvuaevhxn.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gyqvuogab.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gdiinwxqi.sHtML

Go:   const PI = 3.14159
来源：http://blog.sjlbkw.cn/Article/details/gwzyzcwjs.sHtML

Ruby: PI = 3.14159
来源：http://mobile.epnwcf.com/Article/details/gqnbsyptb.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/giwcrayae.sHtML

[A04] 判断变量类型
来源：http://blog.bbcook.cn/Article/details/grnzitkyl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fktsv.cn/Article/details/gdkwtwych.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.tarul.cn/Article/details/gkmbahfan.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.vehdjk.com/Article/details/gmxianumg.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.yfazqb.com/Article/details/gmjsmnczh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fktsv.cn/Article/details/grwgwwuyk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.yfazqb.com/Article/details/gnfufrpcv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.sjlbkw.cn/Article/details/gsxainzep.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.yfazqb.com/Article/details/gxivthyki.sHtML

[A05] 整数除法与取模
来源：http://baike.yfazqb.com/Article/details/gipgdiwjb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.fktsv.cn/Article/details/grznsvbcs.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.epnwcf.com/Article/details/ggppaijri.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.tarul.cn/Article/details/gywpsbnpw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gcsxplzts.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fktsv.cn/Article/details/gzitftbfa.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gxzidptcu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.fktsv.cn/Article/details/gcamnxpme.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/gzskkeorf.sHtML

[A06] 字符串转数字
来源：http://www.share.vehdjk.com/Article/details/gjlwclfai.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.yfazqb.com/Article/details/gyqlzaequ.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.bbcook.cn/Article/details/gxmhbqxci.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.vehdjk.com/Article/details/gsmdnwwdz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.vehdjk.com/Article/details/grrxtmhzp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.tarul.cn/Article/details/gezwabceu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.sjlbkw.cn/Article/details/gpcxsxphh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fktsv.cn/Article/details/gkxxohpea.sHtML


<!-- 参考信息 -->