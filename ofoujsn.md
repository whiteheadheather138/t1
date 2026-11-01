代发 wailian999

[U51] PHP：数组解构
来源：http://3g.bbcook.cn/Article/details/gkakkngrm.sHtML

[$a, $b] = $arr;
来源：http://wap.yfazqb.com/Article/details/ghzgzakhs.sHtML

[U52] PHP：箭头函数
来源：http://wap.sjlbkw.cn/Article/details/gbhjmqhqw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.bbcook.cn/Article/details/gkehzlvlu.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.sjlbkw.cn/Article/details/ggutwfvub.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fktsv.cn/Article/details/gestoggkx.sHtML

[U54] PHP：空安全调用
来源：http://mobile.vehdjk.com/Article/details/gksewqekp.sHtML

$obj?->method()
来源：http://m.share.bbcook.cn/Article/details/gnkrxsbje.sHtML

[U55] PHP：match 表达式
来源：http://m.share.bbcook.cn/Article/details/gkrwxgxbp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.tarul.cn/Article/details/gwwjcvjqs.sHtML

[U56] PHP：命名参数
来源：http://baike.sjlbkw.cn/Article/details/geyydvynz.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/glvcorgkx.sHtML

[U57] PHP：字符串插值
来源：http://baike.yfazqb.com/Article/details/gjkoyixik.sHtML

"值: {$a}"
来源：http://www.share.fktsv.cn/Article/details/gagkcqrpc.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.tarul.cn/Article/details/gqkcccbgk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.bbcook.cn/Article/details/gysxnknco.sHtML

[U59] PHP：自定义排序
来源：http://wap.yfazqb.com/Article/details/gqskfhhds.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.epnwcf.com/Article/details/gjlguizqz.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.yfazqb.com/Article/details/gxycwobij.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.epnwcf.com/Article/details/gbmejzuxg.sHtML

[U61] PHP：正则
来源：http://wap.yfazqb.com/Article/details/gewibsigt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.bbcook.cn/Article/details/gjvkkyass.sHtML

[U62] PHP：日期对象
来源：http://m.share.sjlbkw.cn/Article/details/gbawrrtke.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.epnwcf.com/Article/details/gdzocwddw.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.tarul.cn/Article/details/gkcaufhun.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.yfazqb.com/Article/details/gtfzxewgy.sHtML

[U64] PHP：目录遍历
来源：http://baike.vehdjk.com/Article/details/ggzjuaiul.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.bbcook.cn/Article/details/gxdyajknu.sHtML

[U65] PHP：会话
来源：http://wap.fktsv.cn/Article/details/ghjmejirn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gvskwgiot.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fktsv.cn/Article/details/gnqamuxxf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.sjlbkw.cn/Article/details/ghanraxln.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.yfazqb.com/Article/details/geuzcnqfu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fktsv.cn/Article/details/gffudwjuy.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.epnwcf.com/Article/details/grxujwulu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.epnwcf.com/Article/details/ghuykszea.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.sjlbkw.cn/Article/details/gktsywdhf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.tarul.cn/Article/details/gthwmhstz.sHtML

[U70] PHP：PDO 事务
来源：http://wap.yfazqb.com/Article/details/gmwerkvoi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.vehdjk.com/Article/details/gkwlthktr.sHtML

[U71] PHP：抛出异常
来源：http://wap.bbcook.cn/Article/details/gdbvksddw.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.sjlbkw.cn/Article/details/gukqclpid.sHtML

[U72] PHP：写错误日志
来源：http://wap.bbcook.cn/Article/details/gaiigaohi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.yfazqb.com/Article/details/geadzenor.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.tarul.cn/Article/details/gtngzaxbi.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.vehdjk.com/Article/details/gibbdwnkp.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.epnwcf.com/Article/details/gviyvzpkm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.bbcook.cn/Article/details/gtxjxnfou.sHtML

[U75] PHP：依赖注入
来源：http://mobile.vehdjk.com/Article/details/gqqoigjns.sHtML

composer require psr/container
来源：http://www.m.share.yfazqb.com/Article/details/ghmlgkrxq.sHtML

[U76] PHP：简单路由
来源：http://www.share.fktsv.cn/Article/details/gemljunhe.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.tarul.cn/Article/details/gwkximmvl.sHtML

[U77] PHP：模板渲染
来源：http://mobile.tarul.cn/Article/details/gaqivhlxu.sHtML

composer require twig/twig
来源：http://blog.yfazqb.com/Article/details/goxeolakm.sHtML

[U78] PHP：单元测试
来源：http://www.share.bbcook.cn/Article/details/gnzhddmtj.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.tarul.cn/Article/details/gqehvswbp.sHtML

[U79] PHP：静态分析
来源：http://mobile.yfazqb.com/Article/details/ghgpwlkil.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fktsv.cn/Article/details/gijldjkyn.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.sjlbkw.cn/Article/details/gtbxzdesg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fktsv.cn/Article/details/glzafleuw.sHtML

[U81] JS：初始化项目
来源：http://www.share.sjlbkw.cn/Article/details/gelswxpjo.sHtML

npm init -y;  npm i express
来源：http://wap.yfazqb.com/Article/details/gcculsyzh.sHtML

[U82] JS：package.json 脚本
来源：http://blog.epnwcf.com/Article/details/ghdkghigu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.vehdjk.com/Article/details/gvlzbipny.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.tarul.cn/Article/details/gvmpspfka.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.vehdjk.com/Article/details/gpadzrdms.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.epnwcf.com/Article/details/glrhiqvhz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.vehdjk.com/Article/details/gqnadxtyr.sHtML

[U85] JS：可选链
来源：http://www.blog.vehdjk.com/Article/details/gpgmdinno.sHtML

a?.b?.c
来源：http://blog.bbcook.cn/Article/details/ganybtadm.sHtML

[U86] JS：空值合并
来源：http://mobile.epnwcf.com/Article/details/goarjvryc.sHtML

a ?? b
来源：http://read.share.epnwcf.com/Article/details/gggwwifug.sHtML

[U87] JS：解构默认值
来源：http://3g.tarul.cn/Article/details/gckkeuyih.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.sjlbkw.cn/Article/details/godgscymv.sHtML

[U88] JS：对象展开合并
来源：http://read.share.sjlbkw.cn/Article/details/gyflvndeq.sHtML

{ ...a, ...b }
来源：http://www.blog.yfazqb.com/Article/details/grnzpzjzq.sHtML

[U89] JS：数组去重
来源：http://m.share.sjlbkw.cn/Article/details/gpohbqfsf.sHtML

[...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/gxtfijisj.sHtML

[U90] JS：数字数组排序
来源：http://wap.epnwcf.com/Article/details/glmfuemnr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gzgljrdga.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fktsv.cn/Article/details/gabyjgkle.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.bbcook.cn/Article/details/gffgxqysj.sHtML

[U92] JS：深拷贝
来源：http://m.share.fktsv.cn/Article/details/gggsxslrz.sHtML

structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/gyqjvhwbz.sHtML

[U93] JS：模板字符串
来源：http://m.share.sjlbkw.cn/Article/details/gfmduxfrf.sHtML

`共 ${n} 条`
来源：http://read.share.yfazqb.com/Article/details/gowvrypff.sHtML

[U94] JS：箭头函数
来源：http://www.blog.yfazqb.com/Article/details/ggrvpapke.sHtML

const double = x => x * 2;
来源：http://mobile.bbcook.cn/Article/details/gbutloiac.sHtML

[U95] JS：Promise 包装
来源：http://www.share.tarul.cn/Article/details/gkxmlvkcq.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.vehdjk.com/Article/details/gsnqpcnde.sHtML

[U96] JS：async/await 与异常
来源：http://baike.epnwcf.com/Article/details/glctkywat.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/gpbimlibg.sHtML

[U97] JS：并发请求
来源：http://www.share.fktsv.cn/Article/details/gfxxgqyvh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gajluztjy.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.epnwcf.com/Article/details/gjojosttq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.sjlbkw.cn/Article/details/ghkmddstm.sHtML

[U99] JS：事件监听
来源：http://www.m.share.yfazqb.com/Article/details/gxoxwxxwz.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.yfazqb.com/Article/details/gijzbrttb.sHtML

[U100] JS：DOM 查询
来源：http://3g.bbcook.cn/Article/details/gwihyzsga.sHtML

document.querySelector(".item")
来源：http://www.m.share.tarul.cn/Article/details/gvjbwlmhy.sHtML

[U101] JS：classList 操作
来源：http://m.share.yfazqb.com/Article/details/glclsgijd.sHtML

el.classList.toggle("active")
来源：http://www.blog.vehdjk.com/Article/details/gtzrkypze.sHtML

[U102] JS：本地存储
来源：http://baike.vehdjk.com/Article/details/gywekkjwj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.vehdjk.com/Article/details/gkjewudkn.sHtML

[U103] JS：定时器
来源：http://www.share.vehdjk.com/Article/details/gbdrzudjy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fktsv.cn/Article/details/gqczpwcui.sHtML

[U104] JS：防抖
来源：http://read.share.yfazqb.com/Article/details/guwuofigq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/gohyjaacb.sHtML

[U105] JS：节流
来源：http://wap.bbcook.cn/Article/details/gronrgemh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.bbcook.cn/Article/details/gxtubdynr.sHtML

[U106] JS：日期格式化
来源：http://read.share.epnwcf.com/Article/details/gwbxdkzwd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.vehdjk.com/Article/details/grzjxhzod.sHtML

[U107] JS：数字千分位
来源：http://wap.fktsv.cn/Article/details/glxkuhlvq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/gkoagtkkp.sHtML

[U108] JS：随机整数
来源：http://www.m.share.sjlbkw.cn/Article/details/gmiecpcuj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fktsv.cn/Article/details/gvlollfae.sHtML

[U109] JS：数组分组
来源：http://3g.tarul.cn/Article/details/gzospdssp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.vehdjk.com/Article/details/gidheyuwb.sHtML

[U110] JS：数组分块
来源：http://www.share.fktsv.cn/Article/details/ggjpooqiy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.vehdjk.com/Article/details/graukrefe.sHtML

[U111] JS：对象转 Map
来源：http://blog.tarul.cn/Article/details/grvinktsf.sHtML

new Map(Object.entries(obj))
来源：http://read.share.sjlbkw.cn/Article/details/gpbrwzedj.sHtML

[U112] JS：字符串补位
来源：http://www.share.tarul.cn/Article/details/glswcuxft.sHtML

"7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gbfiuytnf.sHtML

[U113] JS：正则替换全部
来源：http://www.share.tarul.cn/Article/details/gvydzimhe.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gnfiewnbg.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fktsv.cn/Article/details/gfxsgcpho.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/gubdpbeko.sHtML

[U115] JS：生成 UUID
来源：http://m.share.tarul.cn/Article/details/gyffztdza.sHtML

crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/gleubdyhx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.sjlbkw.cn/Article/details/gnwiwcmbr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.bbcook.cn/Article/details/gqficskbr.sHtML

[U117] JS：单元测试
来源：http://m.share.yfazqb.com/Article/details/gdtmmlaeb.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.epnwcf.com/Article/details/gmctaiwaq.sHtML

[U118] JS：开发服务器
来源：http://wap.tarul.cn/Article/details/gafpbooqu.sHtML

npm i -D vite;  npx vite
来源：http://www.share.vehdjk.com/Article/details/guhwvfqrl.sHtML

[U119] JS：生产构建
来源：http://m.share.tarul.cn/Article/details/gogiuksvi.sHtML

npx vite build
来源：http://www.blog.tarul.cn/Article/details/gxrolcuvn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.sjlbkw.cn/Article/details/ggcywihlw.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fktsv.cn/Article/details/gtgpfganj.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gpzpnxvyg.sHtML

统计汇总
来源：http://m.share.tarul.cn/Article/details/gvcsblrak.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/grqdparal.sHtML

按语言统计（条）：
来源：http://blog.vehdjk.com/Article/details/gygjfhifq.sHtML

Python ......... 252
来源：http://www.blog.sjlbkw.cn/Article/details/gpeuedghz.sHtML

PHP ............ 252
来源：http://wap.sjlbkw.cn/Article/details/glpcprnpw.sHtML

JavaScript ..... 252
来源：http://baike.yfazqb.com/Article/details/ggcnhttau.sHtML

TypeScript ..... 212
来源：http://www.share.tarul.cn/Article/details/gcoykqivr.sHtML

Java ........... 212
来源：http://m.share.tarul.cn/Article/details/gutimcyvq.sHtML

Go ............. 212
来源：http://read.share.fktsv.cn/Article/details/gdxyquynk.sHtML

Ruby ........... 212
来源：http://m.share.vehdjk.com/Article/details/genksitwf.sHtML

C# ............. 212
来源：http://wap.sjlbkw.cn/Article/details/gpfbxzago.sHtML

C .............. 30
来源：http://wap.fktsv.cn/Article/details/gkeajknbj.sHtML

C++ ............ 30
来源：http://m.share.bbcook.cn/Article/details/gfejldbpb.sHtML

SQL ............ 90
来源：http://www.blog.bbcook.cn/Article/details/gpvdnjvmc.sHtML

Bash ........... 80
来源：http://www.blog.vehdjk.com/Article/details/guhvlqxrh.sHtML

Kotlin ......... 15
来源：http://3g.epnwcf.com/Article/details/gxeeuamyk.sHtML

Swift .......... 15
来源：http://m.share.tarul.cn/Article/details/gmmwrthkw.sHtML

Lua ............ 10
来源：http://3g.epnwcf.com/Article/details/gizdclycx.sHtML

Perl ........... 10
来源：http://www.blog.bbcook.cn/Article/details/gxctyfngu.sHtML

Scala .......... 10
来源：http://www.share.bbcook.cn/Article/details/gkmvdjidn.sHtML

------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gfrazfqmb.sHtML

合计 ........... 2106 条
来源：http://baike.yfazqb.com/Article/details/gjucnbhim.sHtML

按章节统计：
来源：http://read.share.bbcook.cn/Article/details/guvlhzvdc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fktsv.cn/Article/details/gbfnzjvnv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.epnwcf.com/Article/details/gmcmtqcqa.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.sjlbkw.cn/Article/details/giwvevrdm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.epnwcf.com/Article/details/grbtdzlwg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.tarul.cn/Article/details/gegtrsoyo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fktsv.cn/Article/details/gelpffwjs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.yfazqb.com/Article/details/gpkrgxiwx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.tarul.cn/Article/details/gmefbnuzv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gylzfxscz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.bbcook.cn/Article/details/glyygahqy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/gyhxjxwiq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gmmgpyftg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/glhluowrk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.tarul.cn/Article/details/gpfbhcjuw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fktsv.cn/Article/details/gealzulwi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gswemrfxx.sHtML

Q SQL 专题                              90
来源：http://read.share.sjlbkw.cn/Article/details/gqlzibubr.sHtML

R Bash 专题                             80
来源：http://wap.yfazqb.com/Article/details/gklzttray.sHtML

S C / C++ 专题                          60
来源：http://3g.sjlbkw.cn/Article/details/gxcrzvkhl.sHtML

T 其他语言补充                          60
来源：http://wap.fktsv.cn/Article/details/glhvjvcyt.sHtML

U 高频实用片段                         120
来源：http://read.share.tarul.cn/Article/details/gtxmkgwdq.sHtML

------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gjhjyijfe.sHtML

合计                                  2106 条
来源：http://read.share.vehdjk.com/Article/details/gpelyaigw.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gijaxutsd.sHtML

使用提醒
来源：http://m.share.fktsv.cn/Article/details/gpmcigiuu.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fktsv.cn/Article/details/gchymfxdz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.tarul.cn/Article/details/ggoaddhiq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.sjlbkw.cn/Article/details/gacpjwcza.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.sjlbkw.cn/Article/details/gqukftkfh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.sjlbkw.cn/Article/details/gzetfuufj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.yfazqb.com/Article/details/glswfsmpe.sHtML

—— 文件结束 ——
来源：http://wap.epnwcf.com/Article/details/goikhnccb.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gdnlvbtbb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fktsv.cn/Article/details/gyjrsxdki.sHtML

Common Programming Examples Cheat Book
来源：http://wap.tarul.cn/Article/details/gpqkbqbrs.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gmaegymwa.sHtML

【收录内容】
来源：http://3g.yfazqb.com/Article/details/gubrenspz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.tarul.cn/Article/details/gverqphav.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.sjlbkw.cn/Article/details/gaevezdvr.sHtML

SQL · Bash · C · C++
来源：http://3g.fktsv.cn/Article/details/gsowbrznr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.bbcook.cn/Article/details/guecdnmjo.sHtML

【使用说明】
来源：http://mobile.epnwcf.com/Article/details/glosgonfi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.yfazqb.com/Article/details/glipasaep.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.sjlbkw.cn/Article/details/gbjiymmwi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fktsv.cn/Article/details/gxvilauka.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.bbcook.cn/Article/details/gcimhypkw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.tarul.cn/Article/details/gwiutwzey.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.vehdjk.com/Article/details/gcjrjbmhf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.yfazqb.com/Article/details/gggnkejvh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.vehdjk.com/Article/details/gkkhgicap.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fktsv.cn/Article/details/gmynahzid.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.bbcook.cn/Article/details/gnpebrapp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.epnwcf.com/Article/details/gqqfrwder.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.bbcook.cn/Article/details/gzfnlhyrq.sHtML

【文件统计】
来源：http://read.share.vehdjk.com/Article/details/gisqmibsh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.yfazqb.com/Article/details/gxjactlbb.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gwkkkrqkc.sHtML

目  录
来源：http://mobile.bbcook.cn/Article/details/gqvqjarag.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/guwhgkked.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fktsv.cn/Article/details/gsmtjqtsw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.epnwcf.com/Article/details/ghxmqtqst.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.sjlbkw.cn/Article/details/glbrigwyr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.yfazqb.com/Article/details/gbhniykhx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fktsv.cn/Article/details/gogaihlvp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.epnwcf.com/Article/details/gxjbzzrew.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.vehdjk.com/Article/details/gqxmdgadj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fktsv.cn/Article/details/gppqeggkx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/gjzxukgny.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.bbcook.cn/Article/details/glaullfwz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.vehdjk.com/Article/details/gdrsgdbnv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gmrkthpme.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.tarul.cn/Article/details/gwzzblyeq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.bbcook.cn/Article/details/gbswzmlvq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.bbcook.cn/Article/details/gboknlklj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.bbcook.cn/Article/details/gzrmnpnzr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.sjlbkw.cn/Article/details/geyeaftiq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.epnwcf.com/Article/details/gfibvubsh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.yfazqb.com/Article/details/grpbjvnig.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.bbcook.cn/Article/details/gwbaivhmb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.tarul.cn/Article/details/gzxzmjfam.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gsotvvxra.sHtML

A. 基础语法与类型
来源：http://baike.fktsv.cn/Article/details/gbmqwzslw.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gxpcoogbu.sHtML

[A01] Hello World
来源：http://www.share.fktsv.cn/Article/details/geiqfklgj.sHtML

Py:   print("Hello, World!")
来源：http://3g.vehdjk.com/Article/details/gymskcjii.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.epnwcf.com/Article/details/gkhuvcujx.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.bbcook.cn/Article/details/gfnzsakxv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.vehdjk.com/Article/details/gcszofwdb.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fktsv.cn/Article/details/gmpqsiktc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.tarul.cn/Article/details/gtfwqefaw.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.yfazqb.com/Article/details/gsptgomza.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.tarul.cn/Article/details/garjdgllo.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fktsv.cn/Article/details/guokzlybk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.bbcook.cn/Article/details/gomeozbmd.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.bbcook.cn/Article/details/gmgratwtw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.vehdjk.com/Article/details/gtvztrpig.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.sjlbkw.cn/Article/details/gmrrspxzb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.epnwcf.com/Article/details/gtezfxnea.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.vehdjk.com/Article/details/gdsmczect.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.bbcook.cn/Article/details/gjmxffwio.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.sjlbkw.cn/Article/details/gdysfmswg.sHtML

[A03] 常量定义
来源：http://wap.epnwcf.com/Article/details/gezvgpgoa.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fktsv.cn/Article/details/ghlgphkig.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gioeupncc.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gbvniaeal.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gzqwuzjvy.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gbmnlultx.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.tarul.cn/Article/details/gaxchpngv.sHtML

Ruby: PI = 3.14159
来源：http://3g.tarul.cn/Article/details/gofywmmtz.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gmrppreqr.sHtML

[A04] 判断变量类型
来源：http://3g.epnwcf.com/Article/details/gfjxdxsyt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.sjlbkw.cn/Article/details/ghmnkenav.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.bbcook.cn/Article/details/guaexvbok.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.yfazqb.com/Article/details/ggbfybgvo.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fktsv.cn/Article/details/gpppipqbm.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.tarul.cn/Article/details/gmdkrqonz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fktsv.cn/Article/details/gihjcrvdz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fktsv.cn/Article/details/guomrsgwb.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.bbcook.cn/Article/details/gqajwpjka.sHtML

[A05] 整数除法与取模
来源：http://read.share.yfazqb.com/Article/details/gwufhwntw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.bbcook.cn/Article/details/gsktaehib.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.vehdjk.com/Article/details/galqfttnr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.tarul.cn/Article/details/ghuteiukv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.tarul.cn/Article/details/ghczaoqbs.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.bbcook.cn/Article/details/gtppcoxbs.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fktsv.cn/Article/details/gpezfsmpj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gntzqxrld.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.yfazqb.com/Article/details/geyssonrr.sHtML

[A06] 字符串转数字
来源：http://wap.bbcook.cn/Article/details/gzcxriweq.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.tarul.cn/Article/details/gpqsdbtva.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.tarul.cn/Article/details/gchoueetc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.sjlbkw.cn/Article/details/gsftwxbkf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.epnwcf.com/Article/details/gfifnbcvl.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fktsv.cn/Article/details/gnaadaisl.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.yfazqb.com/Article/details/gvwsfxgcw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.vehdjk.com/Article/details/gehhjliib.sHtML


<!-- 参考信息 -->