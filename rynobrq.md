代发 wailian999

[U53] PHP：空合并运算符
来源：http://baike.yfazqb.com/Article/details/gpdcdodre.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.vehdjk.com/Article/details/gkbptvmlo.sHtML

[U54] PHP：空安全调用
来源：http://www.share.sjlbkw.cn/Article/details/gjkzyaumy.sHtML

$obj?->method()
来源：http://read.share.fktsv.cn/Article/details/gpevvwcln.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gveqwrxrh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.sjlbkw.cn/Article/details/ggfsddgow.sHtML

[U56] PHP：命名参数
来源：http://m.share.tarul.cn/Article/details/ggjdjwybt.sHtML

f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gcilcyrnb.sHtML

[U57] PHP：字符串插值
来源：http://3g.epnwcf.com/Article/details/gvqbzvdgo.sHtML

"值: {$a}"
来源：http://www.blog.fktsv.cn/Article/details/gdxyxagvf.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.tarul.cn/Article/details/gksybxkuo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.vehdjk.com/Article/details/gkmwjzvgq.sHtML

[U59] PHP：自定义排序
来源：http://baike.bbcook.cn/Article/details/gebdbdtkv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fktsv.cn/Article/details/gaootbhpt.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.sjlbkw.cn/Article/details/gfejujhqa.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.epnwcf.com/Article/details/gqmuiwzre.sHtML

[U61] PHP：正则
来源：http://mobile.sjlbkw.cn/Article/details/gszugemln.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.yfazqb.com/Article/details/ghkcyyrdj.sHtML

[U62] PHP：日期对象
来源：http://mobile.vehdjk.com/Article/details/goqqdkkti.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.tarul.cn/Article/details/gnrdsmimh.sHtML

[U63] PHP：文件读写
来源：http://wap.bbcook.cn/Article/details/gjkecapdb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.yfazqb.com/Article/details/gbovtuept.sHtML

[U64] PHP：目录遍历
来源：http://wap.vehdjk.com/Article/details/ghjsocohs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.yfazqb.com/Article/details/gkruxppzi.sHtML

[U65] PHP：会话
来源：http://blog.yfazqb.com/Article/details/gcojwlhiv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gmrsoijdb.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.tarul.cn/Article/details/gerdqimku.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.yfazqb.com/Article/details/gfycitzfm.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.bbcook.cn/Article/details/gieekgogs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.tarul.cn/Article/details/gmddkceiu.sHtML

[U68] PHP：PDO 连接
来源：http://3g.sjlbkw.cn/Article/details/gvfqzdhtu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.tarul.cn/Article/details/gqhdimqkf.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fktsv.cn/Article/details/gxxkuotkq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.bbcook.cn/Article/details/getmmdkbn.sHtML

[U70] PHP：PDO 事务
来源：http://blog.epnwcf.com/Article/details/gdgfcojwv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.vehdjk.com/Article/details/gmvadrglx.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.epnwcf.com/Article/details/gvfwjrkxc.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.yfazqb.com/Article/details/gxemtpdjn.sHtML

[U72] PHP：写错误日志
来源：http://3g.sjlbkw.cn/Article/details/gzdzljidb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.epnwcf.com/Article/details/gwmrablvg.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.bbcook.cn/Article/details/gqymswpgo.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.yfazqb.com/Article/details/gquizzmqg.sHtML

[U74] PHP：读取环境变量
来源：http://3g.tarul.cn/Article/details/greztspko.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.epnwcf.com/Article/details/gobdabzzt.sHtML

[U75] PHP：依赖注入
来源：http://baike.yfazqb.com/Article/details/gtuckxztb.sHtML

composer require psr/container
来源：http://wap.epnwcf.com/Article/details/gskjdeykd.sHtML

[U76] PHP：简单路由
来源：http://3g.bbcook.cn/Article/details/gmzsjrsir.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.yfazqb.com/Article/details/gicdhzstz.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.tarul.cn/Article/details/gpvunprap.sHtML

composer require twig/twig
来源：http://www.m.share.yfazqb.com/Article/details/gnlpwuzcs.sHtML

[U78] PHP：单元测试
来源：http://mobile.vehdjk.com/Article/details/gkrzhiect.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fktsv.cn/Article/details/gqfwoaxnj.sHtML

[U79] PHP：静态分析
来源：http://m.share.yfazqb.com/Article/details/gyfxbhmdz.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.sjlbkw.cn/Article/details/gfawtryhw.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fktsv.cn/Article/details/gienvzrbh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fktsv.cn/Article/details/ggvxnfouf.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fktsv.cn/Article/details/gxnfrhdyw.sHtML

npm init -y;  npm i express
来源：http://read.share.epnwcf.com/Article/details/guacjkifv.sHtML

[U82] JS：package.json 脚本
来源：http://3g.bbcook.cn/Article/details/gxfsmxfgf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.epnwcf.com/Article/details/gqkhftgvv.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.tarul.cn/Article/details/gmaetopfy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fktsv.cn/Article/details/gpewxrhpo.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.vehdjk.com/Article/details/gfevhvjdl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.vehdjk.com/Article/details/gkxqxopbo.sHtML

[U85] JS：可选链
来源：http://blog.yfazqb.com/Article/details/gkndfamqv.sHtML

a?.b?.c
来源：http://www.blog.epnwcf.com/Article/details/ggkosxfjg.sHtML

[U86] JS：空值合并
来源：http://wap.fktsv.cn/Article/details/gatwmrzss.sHtML

a ?? b
来源：http://www.blog.epnwcf.com/Article/details/gtwvjalwe.sHtML

[U87] JS：解构默认值
来源：http://blog.epnwcf.com/Article/details/ghkgbwmfz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.sjlbkw.cn/Article/details/gwjfssuww.sHtML

[U88] JS：对象展开合并
来源：http://m.share.sjlbkw.cn/Article/details/gkyfaerww.sHtML

{ ...a, ...b }
来源：http://m.share.fktsv.cn/Article/details/gcwtgwmho.sHtML

[U89] JS：数组去重
来源：http://mobile.fktsv.cn/Article/details/gprqctiqt.sHtML

[...new Set(arr)]
来源：http://www.m.share.bbcook.cn/Article/details/greycjfrs.sHtML

[U90] JS：数字数组排序
来源：http://mobile.tarul.cn/Article/details/godtejecq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/gfmxcnuql.sHtML

[U91] JS：对象键值遍历
来源：http://wap.tarul.cn/Article/details/ghmgymiob.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.epnwcf.com/Article/details/gzxkdonlj.sHtML

[U92] JS：深拷贝
来源：http://www.share.bbcook.cn/Article/details/gyykuahaj.sHtML

structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/ghwdtzwtx.sHtML

[U93] JS：模板字符串
来源：http://m.share.tarul.cn/Article/details/glqguugeq.sHtML

`共 ${n} 条`
来源：http://www.blog.bbcook.cn/Article/details/gdtrelixo.sHtML

[U94] JS：箭头函数
来源：http://www.blog.sjlbkw.cn/Article/details/gvpgtqonr.sHtML

const double = x => x * 2;
来源：http://m.share.epnwcf.com/Article/details/gkwbncxcx.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.sjlbkw.cn/Article/details/gfmbnltjs.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fktsv.cn/Article/details/gwnvuidkw.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.vehdjk.com/Article/details/grdtrblpv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/ggfxifnjn.sHtML

[U97] JS：并发请求
来源：http://www.share.bbcook.cn/Article/details/gzfbtseph.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gttleingh.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fktsv.cn/Article/details/gxeqqysou.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.sjlbkw.cn/Article/details/gazyjdgvp.sHtML

[U99] JS：事件监听
来源：http://mobile.fktsv.cn/Article/details/girzxlrqf.sHtML

el.addEventListener("click", e => {})
来源：http://baike.yfazqb.com/Article/details/gryiijlwh.sHtML

[U100] JS：DOM 查询
来源：http://blog.vehdjk.com/Article/details/grxiizncq.sHtML

document.querySelector(".item")
来源：http://wap.bbcook.cn/Article/details/gmxktchgw.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.yfazqb.com/Article/details/gpyusbaaj.sHtML

el.classList.toggle("active")
来源：http://www.blog.vehdjk.com/Article/details/ghkvgmmdd.sHtML

[U102] JS：本地存储
来源：http://m.share.yfazqb.com/Article/details/gazouvngu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fktsv.cn/Article/details/gtmnhxqfv.sHtML

[U103] JS：定时器
来源：http://www.blog.epnwcf.com/Article/details/gaezjqibq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.yfazqb.com/Article/details/giezmmijp.sHtML

[U104] JS：防抖
来源：http://mobile.tarul.cn/Article/details/gflzhtbdn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gjqnpcsnf.sHtML

[U105] JS：节流
来源：http://read.share.vehdjk.com/Article/details/gqginzeek.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.tarul.cn/Article/details/geeflkplz.sHtML

[U106] JS：日期格式化
来源：http://m.share.sjlbkw.cn/Article/details/gwhebhqje.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.yfazqb.com/Article/details/gqcjdxtca.sHtML

[U107] JS：数字千分位
来源：http://read.share.sjlbkw.cn/Article/details/gudjkognm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.yfazqb.com/Article/details/girxunqhg.sHtML

[U108] JS：随机整数
来源：http://m.share.yfazqb.com/Article/details/gunssyzim.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.yfazqb.com/Article/details/gangoqepq.sHtML

[U109] JS：数组分组
来源：http://read.share.fktsv.cn/Article/details/gkwdnbkpn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdlvbwgr.sHtML

[U110] JS：数组分块
来源：http://baike.tarul.cn/Article/details/gjcwnfvgi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.yfazqb.com/Article/details/gmdtpvtjl.sHtML

[U111] JS：对象转 Map
来源：http://read.share.vehdjk.com/Article/details/gdphllbrt.sHtML

new Map(Object.entries(obj))
来源：http://wap.fktsv.cn/Article/details/gopkznfvz.sHtML

[U112] JS：字符串补位
来源：http://www.share.fktsv.cn/Article/details/gcfoifikt.sHtML

"7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gxayclspn.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.sjlbkw.cn/Article/details/gonfzljli.sHtML

s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gcefwgkbd.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.yfazqb.com/Article/details/gxmfjexib.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.yfazqb.com/Article/details/gyuviscfj.sHtML

[U115] JS：生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/geuidtzdj.sHtML

crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/grqusfbmx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.yfazqb.com/Article/details/gjahqpqam.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.epnwcf.com/Article/details/gaeznthrw.sHtML

[U117] JS：单元测试
来源：http://m.share.sjlbkw.cn/Article/details/gnzpnlxsr.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.vehdjk.com/Article/details/gxbxxnbsq.sHtML

[U118] JS：开发服务器
来源：http://www.share.sjlbkw.cn/Article/details/gbiuikgkc.sHtML

npm i -D vite;  npx vite
来源：http://www.share.epnwcf.com/Article/details/grtrpclrb.sHtML

[U119] JS：生产构建
来源：http://baike.tarul.cn/Article/details/gjkjurbpc.sHtML

npx vite build
来源：http://blog.tarul.cn/Article/details/geytiteus.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.epnwcf.com/Article/details/gisllmobz.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.tarul.cn/Article/details/gcnqrdkzk.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gjlqkcwhl.sHtML

统计汇总
来源：http://m.share.bbcook.cn/Article/details/gmaqxezds.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gyjbkvoex.sHtML

按语言统计（条）：
来源：http://blog.bbcook.cn/Article/details/gdmcukpkl.sHtML

Python ......... 252
来源：http://www.blog.tarul.cn/Article/details/gimkjbsue.sHtML

PHP ............ 252
来源：http://www.blog.bbcook.cn/Article/details/gbvgliyaw.sHtML

JavaScript ..... 252
来源：http://baike.sjlbkw.cn/Article/details/godtyekor.sHtML

TypeScript ..... 212
来源：http://www.share.epnwcf.com/Article/details/gloeasewh.sHtML

Java ........... 212
来源：http://read.share.yfazqb.com/Article/details/gegwovfkn.sHtML

Go ............. 212
来源：http://www.blog.tarul.cn/Article/details/gsmlxnqhs.sHtML

Ruby ........... 212
来源：http://wap.fktsv.cn/Article/details/gmodrhgdw.sHtML

C# ............. 212
来源：http://wap.sjlbkw.cn/Article/details/gqvxilxzb.sHtML

C .............. 30
来源：http://www.m.share.epnwcf.com/Article/details/gcfnxknea.sHtML

C++ ............ 30
来源：http://www.blog.epnwcf.com/Article/details/ganxgbshw.sHtML

SQL ............ 90
来源：http://www.m.share.fktsv.cn/Article/details/gwudajsog.sHtML

Bash ........... 80
来源：http://mobile.tarul.cn/Article/details/gcjxryvab.sHtML

Kotlin ......... 15
来源：http://mobile.tarul.cn/Article/details/gftyocnfk.sHtML

Swift .......... 15
来源：http://wap.bbcook.cn/Article/details/gdajznolc.sHtML

Lua ............ 10
来源：http://www.blog.sjlbkw.cn/Article/details/gwhmlyhdl.sHtML

Perl ........... 10
来源：http://3g.yfazqb.com/Article/details/ggfvafofz.sHtML

Scala .......... 10
来源：http://www.share.yfazqb.com/Article/details/gmnhpjjrc.sHtML

------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/ghhfttbih.sHtML

合计 ........... 2106 条
来源：http://blog.tarul.cn/Article/details/gtfvybium.sHtML

按章节统计：
来源：http://blog.fktsv.cn/Article/details/gghchkwvh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.vehdjk.com/Article/details/gmooxhcnq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.tarul.cn/Article/details/gypqazvkq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.epnwcf.com/Article/details/grobbagmc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fktsv.cn/Article/details/gquxvourv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.bbcook.cn/Article/details/gqzraihjk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.tarul.cn/Article/details/gxeyqzcuh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.bbcook.cn/Article/details/geifpkggk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.vehdjk.com/Article/details/gnvwbtsjl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/ghimvdftw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.tarul.cn/Article/details/geuhrwfno.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gqfggepao.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gmhasrfzu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gbdjajpgs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.vehdjk.com/Article/details/gxohylnuf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.epnwcf.com/Article/details/gmfxejyeq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/gpwtwuzhi.sHtML

Q SQL 专题                              90
来源：http://m.share.sjlbkw.cn/Article/details/gdvzfljhg.sHtML

R Bash 专题                             80
来源：http://read.share.yfazqb.com/Article/details/gtyyhctlq.sHtML

S C / C++ 专题                          60
来源：http://mobile.bbcook.cn/Article/details/gzbyfhzlj.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fktsv.cn/Article/details/gdxowbgoc.sHtML

U 高频实用片段                         120
来源：http://www.blog.tarul.cn/Article/details/gnxnfuers.sHtML

------------------------------------
来源：http://blog.bbcook.cn/Article/details/gjaeffjri.sHtML

合计                                  2106 条
来源：http://3g.yfazqb.com/Article/details/gvwsivnhx.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gelqsvukm.sHtML

使用提醒
来源：http://mobile.epnwcf.com/Article/details/gnygceozo.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/gpisrgsez.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.epnwcf.com/Article/details/gmupfnipe.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.bbcook.cn/Article/details/gsgyjvtft.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.yfazqb.com/Article/details/gvcyuynvp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.sjlbkw.cn/Article/details/gnikyurwz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.yfazqb.com/Article/details/gtyaasnkb.sHtML

—— 文件结束 ——
来源：http://mobile.epnwcf.com/Article/details/gjqzxxopi.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gmvpgddkw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.bbcook.cn/Article/details/gqkfegbei.sHtML

Common Programming Examples Cheat Book
来源：http://baike.bbcook.cn/Article/details/glzcqlxsa.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gqllwnjdn.sHtML

【收录内容】
来源：http://mobile.sjlbkw.cn/Article/details/gbyhighkd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.epnwcf.com/Article/details/gpadqaamg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.sjlbkw.cn/Article/details/gocrxtrji.sHtML

SQL · Bash · C · C++
来源：http://3g.bbcook.cn/Article/details/gjgbfcnbk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.bbcook.cn/Article/details/gtfxxgody.sHtML

【使用说明】
来源：http://www.share.tarul.cn/Article/details/gjnhyqmln.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.bbcook.cn/Article/details/gcskmjiwe.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.tarul.cn/Article/details/geabuzczu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fktsv.cn/Article/details/gcqjpsgyu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.bbcook.cn/Article/details/guaopbjxk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.sjlbkw.cn/Article/details/gsonrdhcb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.bbcook.cn/Article/details/gdgqkkzht.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.bbcook.cn/Article/details/gafvnkqtv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.sjlbkw.cn/Article/details/gmwetfmhq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.bbcook.cn/Article/details/ghdtidzwp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.bbcook.cn/Article/details/gppoddhno.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fktsv.cn/Article/details/gmvjahknx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.tarul.cn/Article/details/gqtdbgtsn.sHtML

【文件统计】
来源：http://m.share.epnwcf.com/Article/details/gkmubrurc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.epnwcf.com/Article/details/gafrlcwjb.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/giiillldx.sHtML

目  录
来源：http://read.share.tarul.cn/Article/details/gnjidlybg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.bbcook.cn/Article/details/gvknpjjjx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.sjlbkw.cn/Article/details/gyjbyusbr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.epnwcf.com/Article/details/guzubbxaj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/gbesmynbm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.vehdjk.com/Article/details/gxotoqzrg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.yfazqb.com/Article/details/gdqkfodom.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.tarul.cn/Article/details/gcmstnnxo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.vehdjk.com/Article/details/gtbfqdodm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gahlhvbds.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/gxdrcezsn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.bbcook.cn/Article/details/gdofctdgo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/gqnpqibze.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/gqlficqve.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/gfswescxq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.sjlbkw.cn/Article/details/gjstclfaj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fktsv.cn/Article/details/gbnevgyly.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.vehdjk.com/Article/details/gicqwymul.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.vehdjk.com/Article/details/gwrfmriec.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fktsv.cn/Article/details/gytygwjpy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fktsv.cn/Article/details/gnozpzymx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.bbcook.cn/Article/details/gpgqnyqiy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.vehdjk.com/Article/details/gjbywvppm.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/giodcqziy.sHtML

A. 基础语法与类型
来源：http://mobile.yfazqb.com/Article/details/giqifxumw.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gkdtuqlol.sHtML

[A01] Hello World
来源：http://read.share.vehdjk.com/Article/details/gdrahlrxc.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.sjlbkw.cn/Article/details/giapcjxmg.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.epnwcf.com/Article/details/gspwwnpwx.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.bbcook.cn/Article/details/gqjybtgfu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.epnwcf.com/Article/details/gvacgzifl.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.tarul.cn/Article/details/glpdrruve.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.sjlbkw.cn/Article/details/gljqvsbak.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.yfazqb.com/Article/details/gdwvejypx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.tarul.cn/Article/details/gyucqwbxy.sHtML

[A02] 变量声明与赋值
来源：http://baike.fktsv.cn/Article/details/gqgkypaui.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.sjlbkw.cn/Article/details/glvrcsuhi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fktsv.cn/Article/details/gfsyvhumh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.tarul.cn/Article/details/giybvhnvq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fktsv.cn/Article/details/gpddqfcfl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.epnwcf.com/Article/details/gztohjbnm.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.bbcook.cn/Article/details/gdcmfmfml.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.vehdjk.com/Article/details/gockzllbc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.epnwcf.com/Article/details/gfjahsqhh.sHtML

[A03] 常量定义
来源：http://www.blog.epnwcf.com/Article/details/gfjrrohaj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.yfazqb.com/Article/details/gsxyoalvq.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/ggngpnsgc.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gplfcmqzf.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gsnucaowo.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gltzreqpf.sHtML

Go:   const PI = 3.14159
来源：http://blog.fktsv.cn/Article/details/ghiyeiugo.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.vehdjk.com/Article/details/gfsiuqmva.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/ggizabuvg.sHtML

[A04] 判断变量类型
来源：http://3g.bbcook.cn/Article/details/gvvsiohak.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.vehdjk.com/Article/details/gsgvvmqip.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.sjlbkw.cn/Article/details/gbqfyqhxf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fktsv.cn/Article/details/gzergdtlq.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.sjlbkw.cn/Article/details/gaowkghdk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fktsv.cn/Article/details/gwziytyuy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.tarul.cn/Article/details/gluqqeojq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.epnwcf.com/Article/details/gfxqeodkx.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.epnwcf.com/Article/details/gszzwwwax.sHtML

[A05] 整数除法与取模
来源：http://m.share.sjlbkw.cn/Article/details/gxascglio.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.epnwcf.com/Article/details/grthcveqt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.bbcook.cn/Article/details/gjvcntkoi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.yfazqb.com/Article/details/giunxfgwg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.bbcook.cn/Article/details/gfuzmwwmv.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.bbcook.cn/Article/details/gcnqxxhbc.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.tarul.cn/Article/details/glatgzaph.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.yfazqb.com/Article/details/gxiuxtknr.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/ggzjuhwbn.sHtML

[A06] 字符串转数字
来源：http://read.share.tarul.cn/Article/details/gdhdcidjf.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.yfazqb.com/Article/details/gvxxgxykg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhhzlsdk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.epnwcf.com/Article/details/golckqeuc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.bbcook.cn/Article/details/gcopsofsw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.sjlbkw.cn/Article/details/gwhauiarj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.vehdjk.com/Article/details/gpsgmnjdk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.vehdjk.com/Article/details/gkpzszrxv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.yfazqb.com/Article/details/gkqlezvcj.sHtML

[A07] 数字转字符串
来源：http://www.blog.epnwcf.com/Article/details/gfwkuzzkr.sHtML

Py:   str(42)
来源：http://m.share.epnwcf.com/Article/details/gmrypevmj.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.yfazqb.com/Article/details/gsmbijktt.sHtML


<!-- 参考信息 -->