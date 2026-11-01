代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.m.share.vehdjk.com/Article/details/gzmmfvxcx.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.epnwcf.com/Article/details/guwyxeong.sHtML

[U54] PHP：空安全调用
来源：http://read.share.epnwcf.com/Article/details/gqeaifehj.sHtML

$obj?->method()
来源：http://www.m.share.vehdjk.com/Article/details/gclprarzn.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fktsv.cn/Article/details/gkmvhcdme.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.vehdjk.com/Article/details/gliianigo.sHtML

[U56] PHP：命名参数
来源：http://3g.yfazqb.com/Article/details/gqnbbnzui.sHtML

f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/grquokyoe.sHtML

[U57] PHP：字符串插值
来源：http://wap.epnwcf.com/Article/details/gnrucsnvp.sHtML

"值: {$a}"
来源：http://www.share.fktsv.cn/Article/details/gmwhtbefj.sHtML

[U58] PHP：数组三件套
来源：http://baike.bbcook.cn/Article/details/gmjhrmuea.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.vehdjk.com/Article/details/ghhfnkcti.sHtML

[U59] PHP：自定义排序
来源：http://wap.fktsv.cn/Article/details/gonunjcyh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.sjlbkw.cn/Article/details/gdjxpiaeb.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.epnwcf.com/Article/details/gceelvqju.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.yfazqb.com/Article/details/guzgpmuni.sHtML

[U61] PHP：正则
来源：http://www.share.yfazqb.com/Article/details/gbcodvajk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.yfazqb.com/Article/details/gujlwikeu.sHtML

[U62] PHP：日期对象
来源：http://baike.epnwcf.com/Article/details/gwwoznirh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.yfazqb.com/Article/details/gdpdurfhu.sHtML

[U63] PHP：文件读写
来源：http://www.share.tarul.cn/Article/details/gdtvvwylj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fktsv.cn/Article/details/gcoagxhpn.sHtML

[U64] PHP：目录遍历
来源：http://3g.fktsv.cn/Article/details/gjjqqrfsa.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.sjlbkw.cn/Article/details/gvlvsckkt.sHtML

[U65] PHP：会话
来源：http://3g.fktsv.cn/Article/details/gcgxevlrp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gjlbnwwee.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fktsv.cn/Article/details/gkadoxhci.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.epnwcf.com/Article/details/gupocisoh.sHtML

[U67] PHP：处理文件上传
来源：http://wap.yfazqb.com/Article/details/gqjflckqh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fktsv.cn/Article/details/grwkcfkfd.sHtML

[U68] PHP：PDO 连接
来源：http://wap.epnwcf.com/Article/details/guoqfdowg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.sjlbkw.cn/Article/details/gntkbhvev.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.vehdjk.com/Article/details/gmmyrsagg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fktsv.cn/Article/details/gpvaxkkdi.sHtML

[U70] PHP：PDO 事务
来源：http://baike.tarul.cn/Article/details/gwxxnuywr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.yfazqb.com/Article/details/gaisglqlq.sHtML

[U71] PHP：抛出异常
来源：http://baike.vehdjk.com/Article/details/gmspcacjg.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fktsv.cn/Article/details/gzxgjulsz.sHtML

[U72] PHP：写错误日志
来源：http://www.share.bbcook.cn/Article/details/gwvlcnfcp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.vehdjk.com/Article/details/gtpafpnnh.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fktsv.cn/Article/details/grymvmnrl.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.epnwcf.com/Article/details/glscraaac.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.bbcook.cn/Article/details/guxzweahz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fktsv.cn/Article/details/gegmrrohe.sHtML

[U75] PHP：依赖注入
来源：http://www.share.vehdjk.com/Article/details/gdmxevski.sHtML

composer require psr/container
来源：http://mobile.sjlbkw.cn/Article/details/gbjsqpbll.sHtML

[U76] PHP：简单路由
来源：http://www.share.tarul.cn/Article/details/gqpegothn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.vehdjk.com/Article/details/ggakafsoi.sHtML

[U77] PHP：模板渲染
来源：http://mobile.sjlbkw.cn/Article/details/grayvxdyl.sHtML

composer require twig/twig
来源：http://www.blog.fktsv.cn/Article/details/gkjufhqgv.sHtML

[U78] PHP：单元测试
来源：http://www.share.sjlbkw.cn/Article/details/grvfiisef.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.tarul.cn/Article/details/ggqyuwqtf.sHtML

[U79] PHP：静态分析
来源：http://blog.yfazqb.com/Article/details/gsnclmhor.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.sjlbkw.cn/Article/details/ggprllfmm.sHtML

[U80] PHP：代码规范修复
来源：http://baike.tarul.cn/Article/details/gdfcpnmqt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.tarul.cn/Article/details/gvcjystye.sHtML

[U81] JS：初始化项目
来源：http://baike.epnwcf.com/Article/details/gtpyrrmtt.sHtML

npm init -y;  npm i express
来源：http://mobile.yfazqb.com/Article/details/gsgbvxzzt.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.sjlbkw.cn/Article/details/gnsfxzmnj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.epnwcf.com/Article/details/gqhmgkgte.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.yfazqb.com/Article/details/gkcnvmxdx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.vehdjk.com/Article/details/gciyxvsvk.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtonfjgn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.yfazqb.com/Article/details/gwihrxwli.sHtML

[U85] JS：可选链
来源：http://3g.yfazqb.com/Article/details/gvsxoqrkv.sHtML

a?.b?.c
来源：http://wap.fktsv.cn/Article/details/gxfgqosmf.sHtML

[U86] JS：空值合并
来源：http://wap.vehdjk.com/Article/details/gnpqldrlq.sHtML

a ?? b
来源：http://3g.epnwcf.com/Article/details/gmjvmdztw.sHtML

[U87] JS：解构默认值
来源：http://m.share.vehdjk.com/Article/details/gnuxvkukj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.yfazqb.com/Article/details/gtqjfvrbk.sHtML

[U88] JS：对象展开合并
来源：http://wap.epnwcf.com/Article/details/gspedddie.sHtML

{ ...a, ...b }
来源：http://baike.yfazqb.com/Article/details/gjhwaxumy.sHtML

[U89] JS：数组去重
来源：http://www.m.share.bbcook.cn/Article/details/gjtkyfqfn.sHtML

[...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/gnhdkoyzk.sHtML

[U90] JS：数字数组排序
来源：http://3g.yfazqb.com/Article/details/ghfwncgtu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/gbqagpymm.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.tarul.cn/Article/details/gruxyfhwa.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.vehdjk.com/Article/details/gbqtheygo.sHtML

[U92] JS：深拷贝
来源：http://www.blog.bbcook.cn/Article/details/gmdhvjttn.sHtML

structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/ggqsxzyof.sHtML

[U93] JS：模板字符串
来源：http://mobile.vehdjk.com/Article/details/gckitearx.sHtML

`共 ${n} 条`
来源：http://www.m.share.tarul.cn/Article/details/ghmbborrx.sHtML

[U94] JS：箭头函数
来源：http://m.share.bbcook.cn/Article/details/gatpdiwsg.sHtML

const double = x => x * 2;
来源：http://blog.epnwcf.com/Article/details/gbubfsslr.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.sjlbkw.cn/Article/details/gsvgaeoth.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.epnwcf.com/Article/details/gtgcgoprn.sHtML

[U96] JS：async/await 与异常
来源：http://wap.bbcook.cn/Article/details/gtuhxzstj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/gntlkugim.sHtML

[U97] JS：并发请求
来源：http://mobile.fktsv.cn/Article/details/gfornagql.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/gdkjniyqv.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.tarul.cn/Article/details/gsdznslvd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fktsv.cn/Article/details/guybsalra.sHtML

[U99] JS：事件监听
来源：http://www.share.bbcook.cn/Article/details/gjkszqymv.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.bbcook.cn/Article/details/gzazmnjnx.sHtML

[U100] JS：DOM 查询
来源：http://wap.sjlbkw.cn/Article/details/gfofquuvs.sHtML

document.querySelector(".item")
来源：http://read.share.yfazqb.com/Article/details/gjgoiykdc.sHtML

[U101] JS：classList 操作
来源：http://wap.epnwcf.com/Article/details/gsejpkjlm.sHtML

el.classList.toggle("active")
来源：http://baike.fktsv.cn/Article/details/getdlvxsz.sHtML

[U102] JS：本地存储
来源：http://mobile.yfazqb.com/Article/details/gjymqalga.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.bbcook.cn/Article/details/gdurtlojj.sHtML

[U103] JS：定时器
来源：http://baike.vehdjk.com/Article/details/gttgkwmef.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.epnwcf.com/Article/details/gnsjhnmrf.sHtML

[U104] JS：防抖
来源：http://wap.tarul.cn/Article/details/gaploncxp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.tarul.cn/Article/details/gwjspznzy.sHtML

[U105] JS：节流
来源：http://www.blog.vehdjk.com/Article/details/gwgeoeubv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnrmwkfs.sHtML

[U106] JS：日期格式化
来源：http://wap.yfazqb.com/Article/details/gofydaoih.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.bbcook.cn/Article/details/gekehsnxi.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.vehdjk.com/Article/details/gyvysqoqy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.yfazqb.com/Article/details/gbdpkdulo.sHtML

[U108] JS：随机整数
来源：http://3g.vehdjk.com/Article/details/gehqxzceq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.vehdjk.com/Article/details/gqfxacgoa.sHtML

[U109] JS：数组分组
来源：http://mobile.fktsv.cn/Article/details/gsbgebvif.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.epnwcf.com/Article/details/gyysgivjy.sHtML

[U110] JS：数组分块
来源：http://blog.fktsv.cn/Article/details/gdoeedaze.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.epnwcf.com/Article/details/gpujoggju.sHtML

[U111] JS：对象转 Map
来源：http://wap.vehdjk.com/Article/details/gslonppiz.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.bbcook.cn/Article/details/gkzabdarh.sHtML

[U112] JS：字符串补位
来源：http://wap.epnwcf.com/Article/details/getmoufns.sHtML

"7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gexyxuhei.sHtML

[U113] JS：正则替换全部
来源：http://baike.epnwcf.com/Article/details/grruagcvn.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/grhlzmwiy.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.sjlbkw.cn/Article/details/gnfiaqlbx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.epnwcf.com/Article/details/gmwdqzcgt.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.yfazqb.com/Article/details/gpgynftec.sHtML

crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gnefrwddb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.tarul.cn/Article/details/gsguaafxa.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.epnwcf.com/Article/details/grevaqnal.sHtML

[U117] JS：单元测试
来源：http://read.share.bbcook.cn/Article/details/gujuoowde.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fktsv.cn/Article/details/gmopjvkwb.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fktsv.cn/Article/details/gkpzdeupv.sHtML

npm i -D vite;  npx vite
来源：http://mobile.yfazqb.com/Article/details/gfhkfsxyt.sHtML

[U119] JS：生产构建
来源：http://blog.bbcook.cn/Article/details/goglcdysl.sHtML

npx vite build
来源：http://baike.bbcook.cn/Article/details/gskpojiir.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.tarul.cn/Article/details/gifhngedq.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.sjlbkw.cn/Article/details/galsgoqyx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gmhxiscdb.sHtML

统计汇总
来源：http://m.share.bbcook.cn/Article/details/gnvwzjjsr.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gurkreazc.sHtML

按语言统计（条）：
来源：http://read.share.vehdjk.com/Article/details/gtwketrfd.sHtML

Python ......... 252
来源：http://blog.epnwcf.com/Article/details/giyxefkkx.sHtML

PHP ............ 252
来源：http://mobile.sjlbkw.cn/Article/details/gvjfpzhgz.sHtML

JavaScript ..... 252
来源：http://baike.fktsv.cn/Article/details/gioishtvp.sHtML

TypeScript ..... 212
来源：http://blog.vehdjk.com/Article/details/gmzueknyn.sHtML

Java ........... 212
来源：http://www.share.sjlbkw.cn/Article/details/gsdpywvwo.sHtML

Go ............. 212
来源：http://blog.vehdjk.com/Article/details/ghbdzrcxz.sHtML

Ruby ........... 212
来源：http://mobile.vehdjk.com/Article/details/gbjzgexjo.sHtML

C# ............. 212
来源：http://mobile.bbcook.cn/Article/details/grdadsjzv.sHtML

C .............. 30
来源：http://3g.bbcook.cn/Article/details/gowtbqpnt.sHtML

C++ ............ 30
来源：http://wap.epnwcf.com/Article/details/gqulfpmcf.sHtML

SQL ............ 90
来源：http://www.m.share.vehdjk.com/Article/details/gvikdigdp.sHtML

Bash ........... 80
来源：http://www.blog.vehdjk.com/Article/details/guameyryb.sHtML

Kotlin ......... 15
来源：http://3g.epnwcf.com/Article/details/gorpmcswt.sHtML

Swift .......... 15
来源：http://baike.vehdjk.com/Article/details/glbpwhjbz.sHtML

Lua ............ 10
来源：http://mobile.bbcook.cn/Article/details/gelvkejkw.sHtML

Perl ........... 10
来源：http://m.share.epnwcf.com/Article/details/gwnjqatrs.sHtML

Scala .......... 10
来源：http://m.share.yfazqb.com/Article/details/gcbvcivvc.sHtML

------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/guqlzbsmp.sHtML

合计 ........... 2106 条
来源：http://read.share.bbcook.cn/Article/details/glnudcdhn.sHtML

按章节统计：
来源：http://www.m.share.fktsv.cn/Article/details/gspdzppfj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.vehdjk.com/Article/details/gvvamzwvd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fktsv.cn/Article/details/gtwmopdew.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/gnsolzfol.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.vehdjk.com/Article/details/gtpdhphhz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.yfazqb.com/Article/details/gccovoxhs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.bbcook.cn/Article/details/gzdzakvik.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.tarul.cn/Article/details/gctoajmcw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fktsv.cn/Article/details/gouxsbxnz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/gixalauaw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.sjlbkw.cn/Article/details/gqwbwcbez.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/grefgonnb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gglfocuni.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/ghfaqhsdk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.bbcook.cn/Article/details/gkjzlrekh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.tarul.cn/Article/details/gzlzpaoqm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/goysnxtfi.sHtML

Q SQL 专题                              90
来源：http://baike.epnwcf.com/Article/details/gzjkcoyec.sHtML

R Bash 专题                             80
来源：http://blog.vehdjk.com/Article/details/gvyvlmvrv.sHtML

S C / C++ 专题                          60
来源：http://baike.vehdjk.com/Article/details/gzvmxhvzs.sHtML

T 其他语言补充                          60
来源：http://wap.sjlbkw.cn/Article/details/gbdyesbbe.sHtML

U 高频实用片段                         120
来源：http://mobile.sjlbkw.cn/Article/details/glatidjbs.sHtML

------------------------------------
来源：http://3g.yfazqb.com/Article/details/gdrqdywux.sHtML

合计                                  2106 条
来源：http://www.m.share.epnwcf.com/Article/details/gyhtkiwjk.sHtML

--------------------------------------------------------------------------------
来源：http://3g.epnwcf.com/Article/details/gencrqfnl.sHtML

使用提醒
来源：http://wap.yfazqb.com/Article/details/gwydlejqr.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gjqbkbywk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fktsv.cn/Article/details/gvvwqgbra.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.bbcook.cn/Article/details/gfxiemelt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.bbcook.cn/Article/details/gvqsucmdp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.vehdjk.com/Article/details/gyoxhmxpf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fktsv.cn/Article/details/glawleigu.sHtML

—— 文件结束 ——
来源：http://www.m.share.tarul.cn/Article/details/glbrpxfqo.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/guhkhqgvl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fktsv.cn/Article/details/gyugxkagx.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.tarul.cn/Article/details/gywcyrfni.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gbpjnvrop.sHtML

【收录内容】
来源：http://mobile.fktsv.cn/Article/details/gvchcrldq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.vehdjk.com/Article/details/gcunxymzk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.epnwcf.com/Article/details/gwkkpqhtp.sHtML

SQL · Bash · C · C++
来源：http://mobile.bbcook.cn/Article/details/gqenitjvb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.yfazqb.com/Article/details/gelhsyhpa.sHtML

【使用说明】
来源：http://www.m.share.tarul.cn/Article/details/gcnxwoqcw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.bbcook.cn/Article/details/gnbxxlpcp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.tarul.cn/Article/details/gmkrfylyh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.sjlbkw.cn/Article/details/gcerromiz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.sjlbkw.cn/Article/details/gdcswnedq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.yfazqb.com/Article/details/gsnqotffv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.sjlbkw.cn/Article/details/golxtlxii.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.epnwcf.com/Article/details/gzdlgzrpe.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.bbcook.cn/Article/details/gksgzirtb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.tarul.cn/Article/details/gordnlymc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.yfazqb.com/Article/details/gdtiubbcp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.bbcook.cn/Article/details/gtwbududm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.epnwcf.com/Article/details/gypxsspuz.sHtML

【文件统计】
来源：http://3g.yfazqb.com/Article/details/gtatyplrs.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fktsv.cn/Article/details/gnidshtvi.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/guxncaqfg.sHtML

目  录
来源：http://3g.tarul.cn/Article/details/grpzosodq.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/glcraobni.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.tarul.cn/Article/details/glufukgsm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.bbcook.cn/Article/details/gmjdemsek.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.vehdjk.com/Article/details/gfnaytvbm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.sjlbkw.cn/Article/details/ghusuwjng.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.yfazqb.com/Article/details/gsbxcvryq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.epnwcf.com/Article/details/gprxozbbk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.bbcook.cn/Article/details/glbclrsnl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.vehdjk.com/Article/details/gawrtgrkg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/gtxgxmmjp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.sjlbkw.cn/Article/details/gjcemjvmz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.vehdjk.com/Article/details/ghefvqqdh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/gdbcuuyzj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/ggaugtnjf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.epnwcf.com/Article/details/gicdnackg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.vehdjk.com/Article/details/griecaory.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/gvnkrzgjd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.bbcook.cn/Article/details/gbvoqjzlx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.tarul.cn/Article/details/gvfabvcos.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.vehdjk.com/Article/details/gwkprfznc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.bbcook.cn/Article/details/gvzljhlnm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.bbcook.cn/Article/details/grrcywyij.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gglpiqobc.sHtML

A. 基础语法与类型
来源：http://baike.vehdjk.com/Article/details/grbsqoeic.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gahavacdj.sHtML

[A01] Hello World
来源：http://read.share.yfazqb.com/Article/details/gchfoikyc.sHtML

Py:   print("Hello, World!")
来源：http://mobile.sjlbkw.cn/Article/details/gkrsxzicf.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.yfazqb.com/Article/details/gubdjxbsl.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.vehdjk.com/Article/details/ghvjjmbsw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.vehdjk.com/Article/details/gzfcvibbd.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fktsv.cn/Article/details/gjpinbhkk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fktsv.cn/Article/details/gfirwopca.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fktsv.cn/Article/details/ghdurjpsx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.bbcook.cn/Article/details/gssmadezt.sHtML

[A02] 变量声明与赋值
来源：http://www.share.sjlbkw.cn/Article/details/gthsythns.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.vehdjk.com/Article/details/gzjemjlml.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.epnwcf.com/Article/details/gqhqhrawr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.sjlbkw.cn/Article/details/gbdxzwbbk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.bbcook.cn/Article/details/gwvevfrba.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fktsv.cn/Article/details/gbbsqfhqb.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.bbcook.cn/Article/details/gyslbpxli.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.bbcook.cn/Article/details/giihskxeo.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fktsv.cn/Article/details/gkjiwjuqv.sHtML

[A03] 常量定义
来源：http://www.blog.epnwcf.com/Article/details/gylcdexsy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.yfazqb.com/Article/details/gekctxxzx.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gcdtcaxxl.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gckdpnusq.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/guegszzoo.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gpktafjfn.sHtML

Go:   const PI = 3.14159
来源：http://wap.sjlbkw.cn/Article/details/gjyinqrrx.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.tarul.cn/Article/details/gurjcitsh.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fktsv.cn/Article/details/gjdfefxvt.sHtML

[A04] 判断变量类型
来源：http://m.share.yfazqb.com/Article/details/gpaqxfooy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.epnwcf.com/Article/details/gjoalasle.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.bbcook.cn/Article/details/gtjfkcbcr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.vehdjk.com/Article/details/gilrpsvlr.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.tarul.cn/Article/details/gncqgtjje.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.yfazqb.com/Article/details/gzddyutrk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.vehdjk.com/Article/details/glolyopvd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.sjlbkw.cn/Article/details/gleiqzxfw.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.epnwcf.com/Article/details/guhfktwav.sHtML

[A05] 整数除法与取模
来源：http://baike.bbcook.cn/Article/details/gdkuugqll.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.yfazqb.com/Article/details/gduuistdk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gxjtvjqdo.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.vehdjk.com/Article/details/giwvrtonj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.tarul.cn/Article/details/gtgbkwauw.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.tarul.cn/Article/details/grxwmhrfg.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.epnwcf.com/Article/details/gsfwplgpi.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.tarul.cn/Article/details/gsqdbkmyb.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.yfazqb.com/Article/details/gjqvqiqzs.sHtML

[A06] 字符串转数字
来源：http://blog.tarul.cn/Article/details/gkbjvuucj.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.epnwcf.com/Article/details/grpdpkttq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.yfazqb.com/Article/details/gcnkgeglj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.yfazqb.com/Article/details/gccozxhoo.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.bbcook.cn/Article/details/gojuqmtrz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.epnwcf.com/Article/details/gicvngmty.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fktsv.cn/Article/details/gozdtlugf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.bbcook.cn/Article/details/gkyokfmkn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.yfazqb.com/Article/details/gijjabbmw.sHtML

[A07] 数字转字符串
来源：http://wap.vehdjk.com/Article/details/gcuazsenu.sHtML

Py:   str(42)
来源：http://baike.sjlbkw.cn/Article/details/gjrallzbc.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.epnwcf.com/Article/details/gdxvnndbj.sHtML


<!-- 参考信息 -->