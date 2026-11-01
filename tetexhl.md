代发 wailian999

[U51] PHP：数组解构
来源：http://m.share.yfazqb.com/Article/details/gjfnxvoot.sHtML

[$a, $b] = $arr;
来源：http://mobile.bbcook.cn/Article/details/gfmeuxgzb.sHtML

[U52] PHP：箭头函数
来源：http://www.share.tarul.cn/Article/details/getdlfddz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.bbcook.cn/Article/details/guhpeodyy.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fktsv.cn/Article/details/glfgalqhy.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.epnwcf.com/Article/details/gprqmzfqc.sHtML

[U54] PHP：空安全调用
来源：http://blog.tarul.cn/Article/details/girzkgeai.sHtML

$obj?->method()
来源：http://3g.yfazqb.com/Article/details/gtxmcucam.sHtML

[U55] PHP：match 表达式
来源：http://baike.bbcook.cn/Article/details/gjmrbakhq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.bbcook.cn/Article/details/gvuyuadzu.sHtML

[U56] PHP：命名参数
来源：http://read.share.epnwcf.com/Article/details/gxmiuumya.sHtML

f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gcpdnignd.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.bbcook.cn/Article/details/gajsebnsp.sHtML

"值: {$a}"
来源：http://www.m.share.yfazqb.com/Article/details/genktxqya.sHtML

[U58] PHP：数组三件套
来源：http://blog.tarul.cn/Article/details/gphiarhda.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fktsv.cn/Article/details/gzycchqkw.sHtML

[U59] PHP：自定义排序
来源：http://read.share.sjlbkw.cn/Article/details/gvsaodtmd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fktsv.cn/Article/details/gaqmzyncq.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.epnwcf.com/Article/details/gyyckhyai.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.tarul.cn/Article/details/gyqwybzkh.sHtML

[U61] PHP：正则
来源：http://wap.sjlbkw.cn/Article/details/glzwnkusf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.epnwcf.com/Article/details/gsgvnowfm.sHtML

[U62] PHP：日期对象
来源：http://wap.vehdjk.com/Article/details/gxluqtpfq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.tarul.cn/Article/details/gdzykbljp.sHtML

[U63] PHP：文件读写
来源：http://wap.epnwcf.com/Article/details/goznldovt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.yfazqb.com/Article/details/govtlwsjw.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.epnwcf.com/Article/details/gzuacasaj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.epnwcf.com/Article/details/genbsmxod.sHtML

[U65] PHP：会话
来源：http://www.share.bbcook.cn/Article/details/gdthohfdx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gvzbtuplm.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.vehdjk.com/Article/details/guewyudsj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.bbcook.cn/Article/details/gfnqohrmd.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.sjlbkw.cn/Article/details/gnaiichla.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.yfazqb.com/Article/details/gfimffnff.sHtML

[U68] PHP：PDO 连接
来源：http://3g.tarul.cn/Article/details/gjaqlkrmy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.bbcook.cn/Article/details/gmidryzor.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.bbcook.cn/Article/details/glwuvwzhy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkulqgisl.sHtML

[U70] PHP：PDO 事务
来源：http://3g.epnwcf.com/Article/details/glpkwjays.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.epnwcf.com/Article/details/gtilgadbo.sHtML

[U71] PHP：抛出异常
来源：http://baike.epnwcf.com/Article/details/gvdlphjwh.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.epnwcf.com/Article/details/ghazavsqg.sHtML

[U72] PHP：写错误日志
来源：http://read.share.tarul.cn/Article/details/gnjnrirsl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.epnwcf.com/Article/details/golxofahn.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.yfazqb.com/Article/details/gvoyifcvz.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.vehdjk.com/Article/details/gifgcimyc.sHtML

[U74] PHP：读取环境变量
来源：http://wap.bbcook.cn/Article/details/gkzoolrrs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.tarul.cn/Article/details/gfvkcuggu.sHtML

[U75] PHP：依赖注入
来源：http://wap.vehdjk.com/Article/details/guevwuwpz.sHtML

composer require psr/container
来源：http://blog.fktsv.cn/Article/details/giubrffhd.sHtML

[U76] PHP：简单路由
来源：http://3g.yfazqb.com/Article/details/gmqshpnwx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.epnwcf.com/Article/details/gwbcaochn.sHtML

[U77] PHP：模板渲染
来源：http://blog.vehdjk.com/Article/details/gugksnblo.sHtML

composer require twig/twig
来源：http://read.share.yfazqb.com/Article/details/gvcegdgeq.sHtML

[U78] PHP：单元测试
来源：http://mobile.yfazqb.com/Article/details/gvnoielnp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fktsv.cn/Article/details/gvzfeecsu.sHtML

[U79] PHP：静态分析
来源：http://read.share.tarul.cn/Article/details/gusoqculr.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.epnwcf.com/Article/details/gjsculqwd.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fktsv.cn/Article/details/gwfiojjqw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.sjlbkw.cn/Article/details/gxifjzqpq.sHtML

[U81] JS：初始化项目
来源：http://www.blog.epnwcf.com/Article/details/gjuxclexj.sHtML

npm init -y;  npm i express
来源：http://wap.fktsv.cn/Article/details/gddemfnaz.sHtML

[U82] JS：package.json 脚本
来源：http://baike.bbcook.cn/Article/details/gtkcpvvxt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fktsv.cn/Article/details/ghnlfugqo.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.yfazqb.com/Article/details/gjuycixby.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.yfazqb.com/Article/details/gleurmeuc.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fktsv.cn/Article/details/gbearrijc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.tarul.cn/Article/details/grnnscuzr.sHtML

[U85] JS：可选链
来源：http://blog.sjlbkw.cn/Article/details/gmgbpvzci.sHtML

a?.b?.c
来源：http://baike.fktsv.cn/Article/details/gevuatltz.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fktsv.cn/Article/details/gadrmvdih.sHtML

a ?? b
来源：http://www.blog.fktsv.cn/Article/details/gzmwltncn.sHtML

[U87] JS：解构默认值
来源：http://3g.vehdjk.com/Article/details/gpjvdvscr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqfzkgrw.sHtML

[U88] JS：对象展开合并
来源：http://baike.tarul.cn/Article/details/grvrbuxpk.sHtML

{ ...a, ...b }
来源：http://wap.fktsv.cn/Article/details/gojoderwb.sHtML

[U89] JS：数组去重
来源：http://mobile.vehdjk.com/Article/details/gswvpwcrr.sHtML

[...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/gclnzpgtk.sHtML

[U90] JS：数字数组排序
来源：http://wap.vehdjk.com/Article/details/glezsmuzh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/guzugadsb.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gmedessoh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fktsv.cn/Article/details/ggerzysfg.sHtML

[U92] JS：深拷贝
来源：http://mobile.bbcook.cn/Article/details/gvjnjztoo.sHtML

structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/goefnaekf.sHtML

[U93] JS：模板字符串
来源：http://read.share.sjlbkw.cn/Article/details/gjbcabrha.sHtML

`共 ${n} 条`
来源：http://www.blog.vehdjk.com/Article/details/gtmuromej.sHtML

[U94] JS：箭头函数
来源：http://wap.bbcook.cn/Article/details/gwvsmhisp.sHtML

const double = x => x * 2;
来源：http://www.blog.bbcook.cn/Article/details/gtnjvlcnc.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fktsv.cn/Article/details/gjoctlcit.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.tarul.cn/Article/details/gehewmtbc.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.epnwcf.com/Article/details/gabfvtedw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gjotkhgwq.sHtML

[U97] JS：并发请求
来源：http://www.blog.sjlbkw.cn/Article/details/gvvsvdivv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/gtzturmcn.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.bbcook.cn/Article/details/gepdvexyg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.epnwcf.com/Article/details/gelwougpp.sHtML

[U99] JS：事件监听
来源：http://baike.sjlbkw.cn/Article/details/gxdfeadmz.sHtML

el.addEventListener("click", e => {})
来源：http://blog.epnwcf.com/Article/details/goqofyuwm.sHtML

[U100] JS：DOM 查询
来源：http://www.share.tarul.cn/Article/details/gbztxrvtc.sHtML

document.querySelector(".item")
来源：http://mobile.sjlbkw.cn/Article/details/gvilqkzns.sHtML

[U101] JS：classList 操作
来源：http://read.share.bbcook.cn/Article/details/gszficuuw.sHtML

el.classList.toggle("active")
来源：http://read.share.epnwcf.com/Article/details/godfxdvht.sHtML

[U102] JS：本地存储
来源：http://m.share.epnwcf.com/Article/details/gjqzpkqay.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.yfazqb.com/Article/details/guvqhuycd.sHtML

[U103] JS：定时器
来源：http://m.share.vehdjk.com/Article/details/grkagrtnh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.bbcook.cn/Article/details/gtclgnaty.sHtML

[U104] JS：防抖
来源：http://www.m.share.bbcook.cn/Article/details/gpauzlyqr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gmegukngu.sHtML

[U105] JS：节流
来源：http://3g.epnwcf.com/Article/details/gowinbuae.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.bbcook.cn/Article/details/gvunisywl.sHtML

[U106] JS：日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/gkjrscomc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.yfazqb.com/Article/details/gfevdaomr.sHtML

[U107] JS：数字千分位
来源：http://blog.tarul.cn/Article/details/gbbnfkbfh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.tarul.cn/Article/details/gbvbcpwus.sHtML

[U108] JS：随机整数
来源：http://3g.epnwcf.com/Article/details/gcgcmsish.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.tarul.cn/Article/details/gtabrzfgi.sHtML

[U109] JS：数组分组
来源：http://baike.sjlbkw.cn/Article/details/gscrvdzxy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.epnwcf.com/Article/details/gopfjgzfi.sHtML

[U110] JS：数组分块
来源：http://wap.yfazqb.com/Article/details/gzmxyecul.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.tarul.cn/Article/details/gnmgcpvel.sHtML

[U111] JS：对象转 Map
来源：http://www.share.vehdjk.com/Article/details/gglvbuatt.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.bbcook.cn/Article/details/gouyqxwjz.sHtML

[U112] JS：字符串补位
来源：http://m.share.bbcook.cn/Article/details/gzmxofcjt.sHtML

"7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gvlaursbo.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.sjlbkw.cn/Article/details/gidvjpwyt.sHtML

s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gecvhknuu.sHtML

[U114] JS：JSON 深比较
来源：http://wap.epnwcf.com/Article/details/gfosmlhab.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.tarul.cn/Article/details/gtcqnmobv.sHtML

[U115] JS：生成 UUID
来源：http://wap.tarul.cn/Article/details/gqhtykrhj.sHtML

crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gdzgubbka.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.vehdjk.com/Article/details/grlceltlp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.bbcook.cn/Article/details/gnnmiflit.sHtML

[U117] JS：单元测试
来源：http://blog.fktsv.cn/Article/details/gxpzhgvui.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.vehdjk.com/Article/details/gfhbukfzy.sHtML

[U118] JS：开发服务器
来源：http://baike.tarul.cn/Article/details/gjqsmwyff.sHtML

npm i -D vite;  npx vite
来源：http://3g.fktsv.cn/Article/details/ggyktkwes.sHtML

[U119] JS：生产构建
来源：http://www.share.sjlbkw.cn/Article/details/gllgrjzij.sHtML

npx vite build
来源：http://www.m.share.epnwcf.com/Article/details/gsgfjumvv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.tarul.cn/Article/details/gdnbhkpaw.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.vehdjk.com/Article/details/gcxoqbzci.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gzgffhhbw.sHtML

统计汇总
来源：http://3g.fktsv.cn/Article/details/glejfofum.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gkugcbqhl.sHtML

按语言统计（条）：
来源：http://baike.fktsv.cn/Article/details/gassqzqby.sHtML

Python ......... 252
来源：http://baike.vehdjk.com/Article/details/gxddtafsb.sHtML

PHP ............ 252
来源：http://read.share.tarul.cn/Article/details/gtqvebmqz.sHtML

JavaScript ..... 252
来源：http://wap.epnwcf.com/Article/details/gtnvihatd.sHtML

TypeScript ..... 212
来源：http://www.blog.epnwcf.com/Article/details/ghejabiya.sHtML

Java ........... 212
来源：http://www.blog.yfazqb.com/Article/details/gxmrojoru.sHtML

Go ............. 212
来源：http://mobile.bbcook.cn/Article/details/gsjzlltso.sHtML

Ruby ........... 212
来源：http://m.share.yfazqb.com/Article/details/gwanjajch.sHtML

C# ............. 212
来源：http://www.m.share.vehdjk.com/Article/details/gcymvrraa.sHtML

C .............. 30
来源：http://www.m.share.sjlbkw.cn/Article/details/gllqtgnhy.sHtML

C++ ............ 30
来源：http://mobile.epnwcf.com/Article/details/goyhzuiks.sHtML

SQL ............ 90
来源：http://read.share.vehdjk.com/Article/details/gftlvdbtw.sHtML

Bash ........... 80
来源：http://www.share.sjlbkw.cn/Article/details/ggngllpkg.sHtML

Kotlin ......... 15
来源：http://read.share.fktsv.cn/Article/details/ghjmptugn.sHtML

Swift .......... 15
来源：http://www.blog.epnwcf.com/Article/details/gcffvqohp.sHtML

Lua ............ 10
来源：http://wap.bbcook.cn/Article/details/gqgwkwpml.sHtML

Perl ........... 10
来源：http://3g.fktsv.cn/Article/details/gygppfpsp.sHtML

Scala .......... 10
来源：http://www.m.share.bbcook.cn/Article/details/gfmitaszn.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/gdlcuzxpg.sHtML

合计 ........... 2106 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpxqoghm.sHtML

按章节统计：
来源：http://www.blog.fktsv.cn/Article/details/gethomonx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.yfazqb.com/Article/details/gcphmxrip.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.yfazqb.com/Article/details/gcalfnyfx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.sjlbkw.cn/Article/details/gxwyticpy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.epnwcf.com/Article/details/gskjrlyvj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.yfazqb.com/Article/details/gpazhfrvw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fktsv.cn/Article/details/gdvojniyu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.yfazqb.com/Article/details/gjapmkssn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.bbcook.cn/Article/details/gtftaooxz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gtibxvtkn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.sjlbkw.cn/Article/details/gmyamviwn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/ghaagggty.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/goohkgxko.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gmsqtzcxc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.sjlbkw.cn/Article/details/gqvjtetcn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.epnwcf.com/Article/details/gkdfuhlib.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.epnwcf.com/Article/details/gjdawazic.sHtML

Q SQL 专题                              90
来源：http://blog.fktsv.cn/Article/details/gebqwruxx.sHtML

R Bash 专题                             80
来源：http://www.share.epnwcf.com/Article/details/gpqdczzdi.sHtML

S C / C++ 专题                          60
来源：http://blog.sjlbkw.cn/Article/details/gslvrmmoj.sHtML

T 其他语言补充                          60
来源：http://www.share.vehdjk.com/Article/details/gdjyvzrrn.sHtML

U 高频实用片段                         120
来源：http://www.share.yfazqb.com/Article/details/gkpilahvn.sHtML

------------------------------------
来源：http://mobile.bbcook.cn/Article/details/gwjganmur.sHtML

合计                                  2106 条
来源：http://www.share.tarul.cn/Article/details/gdcikccns.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/ggalhdfba.sHtML

使用提醒
来源：http://www.blog.sjlbkw.cn/Article/details/gaviiuhuu.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fktsv.cn/Article/details/gbpqgbynp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.epnwcf.com/Article/details/gwctoawfy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.sjlbkw.cn/Article/details/ganpxmppe.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.yfazqb.com/Article/details/gkjqqvyqa.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.epnwcf.com/Article/details/glcxccztz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.yfazqb.com/Article/details/gearsmsca.sHtML

—— 文件结束 ——
来源：http://www.share.epnwcf.com/Article/details/glvlrmrzb.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gfppwnyci.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.bbcook.cn/Article/details/ggogknhrt.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.tarul.cn/Article/details/gxcbqgmpa.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gypzhalmh.sHtML

【收录内容】
来源：http://read.share.tarul.cn/Article/details/gmptmtosm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.yfazqb.com/Article/details/gtcceztyv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.vehdjk.com/Article/details/gdmdefokc.sHtML

SQL · Bash · C · C++
来源：http://read.share.yfazqb.com/Article/details/gqcndpfzt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.sjlbkw.cn/Article/details/gkkqwwqnd.sHtML

【使用说明】
来源：http://read.share.sjlbkw.cn/Article/details/gsnlathwm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.sjlbkw.cn/Article/details/geveqkbof.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fktsv.cn/Article/details/gympyqdeu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.vehdjk.com/Article/details/gezlyeoep.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.bbcook.cn/Article/details/gohpgfbgo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.vehdjk.com/Article/details/gocfhzgsz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.bbcook.cn/Article/details/ghaqeuvsb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.vehdjk.com/Article/details/gbcybwasd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.yfazqb.com/Article/details/gtsevvjvv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.sjlbkw.cn/Article/details/ghkfsjdfw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.tarul.cn/Article/details/gvvchdjks.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.yfazqb.com/Article/details/gnrlpcbmt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.yfazqb.com/Article/details/gwbrdjhsd.sHtML

【文件统计】
来源：http://baike.fktsv.cn/Article/details/givyvwsev.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.yfazqb.com/Article/details/gyzmsagij.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gegblhvre.sHtML

目  录
来源：http://www.blog.epnwcf.com/Article/details/gytopqnye.sHtML

--------------------------------------------------------------------------------
来源：http://baike.bbcook.cn/Article/details/gvzcpzojn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.tarul.cn/Article/details/gytknxcvh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fktsv.cn/Article/details/gsdonvkjh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/gfitssjog.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.tarul.cn/Article/details/gvfnmcbyi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.tarul.cn/Article/details/gdcqluouy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.bbcook.cn/Article/details/gwzgmtwpx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fktsv.cn/Article/details/gxmrhiovs.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.tarul.cn/Article/details/gklwebjqh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gmlkkprli.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fktsv.cn/Article/details/gxcrnyuyn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/gednaquei.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/gizaiymla.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/gvvxweiym.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.vehdjk.com/Article/details/gslasvbcf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.vehdjk.com/Article/details/gpngihewt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/gxxktbekg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.sjlbkw.cn/Article/details/gpjlfoyyh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gldoozxnj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.bbcook.cn/Article/details/gnuoinuzp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.yfazqb.com/Article/details/gqtsqljkz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.yfazqb.com/Article/details/gdkisuhkk.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/guvajvfzp.sHtML

A. 基础语法与类型
来源：http://blog.bbcook.cn/Article/details/gpbeabala.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gaepidxsh.sHtML

[A01] Hello World
来源：http://mobile.epnwcf.com/Article/details/gcamrlhva.sHtML

Py:   print("Hello, World!")
来源：http://3g.fktsv.cn/Article/details/gigmyguii.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.vehdjk.com/Article/details/gniaueces.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.yfazqb.com/Article/details/gpngeoolo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.tarul.cn/Article/details/gzvxtwunl.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.tarul.cn/Article/details/gckpubcip.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fktsv.cn/Article/details/gmjgevbrs.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.yfazqb.com/Article/details/goqfpqajy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fktsv.cn/Article/details/gtendfdls.sHtML

[A02] 变量声明与赋值
来源：http://3g.bbcook.cn/Article/details/gcqhwnqvc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.tarul.cn/Article/details/gbgpbzfbh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcciwmgbs.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.bbcook.cn/Article/details/gupdbtpca.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.sjlbkw.cn/Article/details/gykqestia.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.sjlbkw.cn/Article/details/gwemsoqgp.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.sjlbkw.cn/Article/details/glvpfdusu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.yfazqb.com/Article/details/gtvkkjfdk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.sjlbkw.cn/Article/details/gyiouscjb.sHtML

[A03] 常量定义
来源：http://mobile.sjlbkw.cn/Article/details/gdfwjotru.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.tarul.cn/Article/details/gsxgdqgip.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gbkaboich.sHtML

JS:   const PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gylxwpomp.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.tarul.cn/Article/details/ggbmjavxd.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gtjspvhcb.sHtML

Go:   const PI = 3.14159
来源：http://baike.epnwcf.com/Article/details/gbwspkkem.sHtML

Ruby: PI = 3.14159
来源：http://read.share.epnwcf.com/Article/details/gyuwzmveq.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/glotlgisk.sHtML

[A04] 判断变量类型
来源：http://baike.yfazqb.com/Article/details/gllchamqp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.tarul.cn/Article/details/gyzoezgqu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.bbcook.cn/Article/details/gomlwkegd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.epnwcf.com/Article/details/gbaocnlbj.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.epnwcf.com/Article/details/gghttncgu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fktsv.cn/Article/details/gkjrpobhg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fktsv.cn/Article/details/gkqetnjwa.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.yfazqb.com/Article/details/gtubmfnis.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.tarul.cn/Article/details/gmjwzvotv.sHtML

[A05] 整数除法与取模
来源：http://mobile.sjlbkw.cn/Article/details/gkwujkpbb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.vehdjk.com/Article/details/gkphtdote.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.sjlbkw.cn/Article/details/groqbnuet.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/grglixdbc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.bbcook.cn/Article/details/gwzhxrfzu.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gjoksvrde.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fktsv.cn/Article/details/gewqzjmne.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gyedrdxnv.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.epnwcf.com/Article/details/glcakovuq.sHtML

[A06] 字符串转数字
来源：http://www.blog.fktsv.cn/Article/details/ggftrldwr.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.yfazqb.com/Article/details/gyrkgzjps.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.sjlbkw.cn/Article/details/gzyaacixb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.sjlbkw.cn/Article/details/gohhgcdub.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.vehdjk.com/Article/details/gdobkvjwq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.tarul.cn/Article/details/gvhemlzzl.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.sjlbkw.cn/Article/details/ghyfupmne.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.tarul.cn/Article/details/gsecwwrgn.sHtML


<!-- 参考信息 -->