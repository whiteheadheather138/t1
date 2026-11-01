代发 wailian999

[U59] PHP：自定义排序
来源：http://www.share.tarul.cn/Article/details/grikeelfg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.vehdjk.com/Article/details/ggpyflduw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.sjlbkw.cn/Article/details/gmbhpiuzv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.yfazqb.com/Article/details/gjavvcksx.sHtML

[U61] PHP：正则
来源：http://www.share.vehdjk.com/Article/details/ghcrjrtbn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.yfazqb.com/Article/details/guxwdvtbp.sHtML

[U62] PHP：日期对象
来源：http://mobile.bbcook.cn/Article/details/gtgrdwzhg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.tarul.cn/Article/details/gsokypuun.sHtML

[U63] PHP：文件读写
来源：http://mobile.epnwcf.com/Article/details/gjeubxqap.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.yfazqb.com/Article/details/gtayarjou.sHtML

[U64] PHP：目录遍历
来源：http://3g.vehdjk.com/Article/details/gpogmxveu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.tarul.cn/Article/details/gkfxsvqem.sHtML

[U65] PHP：会话
来源：http://3g.fktsv.cn/Article/details/gdzissvjr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.epnwcf.com/Article/details/gqurreytu.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fktsv.cn/Article/details/gsylxzdyy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gfgwhsnwh.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.epnwcf.com/Article/details/gymgyrhzn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.bbcook.cn/Article/details/gmjqeccuy.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.yfazqb.com/Article/details/ghcwllfrp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.vehdjk.com/Article/details/geawogifm.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.epnwcf.com/Article/details/gbbncuhao.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.sjlbkw.cn/Article/details/grycaapbg.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.vehdjk.com/Article/details/gnqljkclj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fktsv.cn/Article/details/gdaqupgaf.sHtML

[U71] PHP：抛出异常
来源：http://blog.yfazqb.com/Article/details/ghvzzohet.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.vehdjk.com/Article/details/gvfrwgaci.sHtML

[U72] PHP：写错误日志
来源：http://www.share.bbcook.cn/Article/details/gbtkatddv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.epnwcf.com/Article/details/gpwqocbuy.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.vehdjk.com/Article/details/goutgwnmf.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.vehdjk.com/Article/details/gradlcbcu.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fktsv.cn/Article/details/ghhawydfu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.vehdjk.com/Article/details/glgpnstyg.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.sjlbkw.cn/Article/details/gdtubrlpi.sHtML

composer require psr/container
来源：http://baike.epnwcf.com/Article/details/glmwbirye.sHtML

[U76] PHP：简单路由
来源：http://baike.tarul.cn/Article/details/gvpztunxz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.epnwcf.com/Article/details/gjgxmwvtu.sHtML

[U77] PHP：模板渲染
来源：http://blog.vehdjk.com/Article/details/gnqvdobvf.sHtML

composer require twig/twig
来源：http://baike.vehdjk.com/Article/details/gkfnnndfi.sHtML

[U78] PHP：单元测试
来源：http://blog.bbcook.cn/Article/details/gdmefmbup.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.tarul.cn/Article/details/gsctxiazi.sHtML

[U79] PHP：静态分析
来源：http://wap.fktsv.cn/Article/details/gsnjjvdqw.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.vehdjk.com/Article/details/gbeqtcjri.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.tarul.cn/Article/details/gwvnpwaef.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.vehdjk.com/Article/details/grisdvilr.sHtML

[U81] JS：初始化项目
来源：http://read.share.epnwcf.com/Article/details/gsqqbbcyx.sHtML

npm init -y;  npm i express
来源：http://m.share.yfazqb.com/Article/details/gylqwovyj.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.yfazqb.com/Article/details/gguhzmafi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.vehdjk.com/Article/details/gubjgtmcw.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.sjlbkw.cn/Article/details/gpcitlbrf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fktsv.cn/Article/details/gbzfsdvow.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.yfazqb.com/Article/details/gxgsnbujm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.vehdjk.com/Article/details/geqdaxvfm.sHtML

[U85] JS：可选链
来源：http://baike.fktsv.cn/Article/details/ghdzvdqsz.sHtML

a?.b?.c
来源：http://mobile.sjlbkw.cn/Article/details/gqwmackaq.sHtML

[U86] JS：空值合并
来源：http://www.share.bbcook.cn/Article/details/grekoludm.sHtML

a ?? b
来源：http://baike.fktsv.cn/Article/details/gykhomgkf.sHtML

[U87] JS：解构默认值
来源：http://read.share.tarul.cn/Article/details/gxpqtxxkg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.epnwcf.com/Article/details/gseivtlrs.sHtML

[U88] JS：对象展开合并
来源：http://baike.fktsv.cn/Article/details/gblpkizmf.sHtML

{ ...a, ...b }
来源：http://www.m.share.fktsv.cn/Article/details/gmkhelimo.sHtML

[U89] JS：数组去重
来源：http://blog.yfazqb.com/Article/details/geytdexjt.sHtML

[...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/gozzqsitk.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.epnwcf.com/Article/details/guityauwf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gdzhcsrjf.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.sjlbkw.cn/Article/details/gdhnrzauh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.sjlbkw.cn/Article/details/gdcrlppsg.sHtML

[U92] JS：深拷贝
来源：http://3g.yfazqb.com/Article/details/gxhzkdwac.sHtML

structuredClone(obj)
来源：http://3g.tarul.cn/Article/details/gdyudmuti.sHtML

[U93] JS：模板字符串
来源：http://read.share.yfazqb.com/Article/details/gqdsixuvv.sHtML

`共 ${n} 条`
来源：http://wap.vehdjk.com/Article/details/ggmzgfnux.sHtML

[U94] JS：箭头函数
来源：http://baike.fktsv.cn/Article/details/gjxjrpnuw.sHtML

const double = x => x * 2;
来源：http://wap.yfazqb.com/Article/details/gxgknvhvy.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhxaazwj.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.vehdjk.com/Article/details/ghctjfkzk.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.yfazqb.com/Article/details/gtckdutpn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gxigwmvuq.sHtML

[U97] JS：并发请求
来源：http://www.m.share.tarul.cn/Article/details/gsuibpnbm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/gblycglcd.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.bbcook.cn/Article/details/gdmnsywfy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.bbcook.cn/Article/details/giwytckdm.sHtML

[U99] JS：事件监听
来源：http://3g.sjlbkw.cn/Article/details/gwecxqtem.sHtML

el.addEventListener("click", e => {})
来源：http://wap.epnwcf.com/Article/details/gvmshryhw.sHtML

[U100] JS：DOM 查询
来源：http://wap.epnwcf.com/Article/details/gutlqdnpl.sHtML

document.querySelector(".item")
来源：http://blog.bbcook.cn/Article/details/gakthmiiu.sHtML

[U101] JS：classList 操作
来源：http://blog.epnwcf.com/Article/details/gyqdbrcpk.sHtML

el.classList.toggle("active")
来源：http://wap.epnwcf.com/Article/details/ghsxtevsc.sHtML

[U102] JS：本地存储
来源：http://www.share.fktsv.cn/Article/details/gznftqsrb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.sjlbkw.cn/Article/details/gvevspvps.sHtML

[U103] JS：定时器
来源：http://baike.yfazqb.com/Article/details/gyjlocttd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.sjlbkw.cn/Article/details/gseaxjkpy.sHtML

[U104] JS：防抖
来源：http://www.m.share.bbcook.cn/Article/details/gtngxsztp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fktsv.cn/Article/details/gvdtwnsrr.sHtML

[U105] JS：节流
来源：http://blog.sjlbkw.cn/Article/details/gcgjnucau.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.yfazqb.com/Article/details/guxrsdbxo.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/gajrpxmui.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.epnwcf.com/Article/details/gewwkdtft.sHtML

[U107] JS：数字千分位
来源：http://mobile.yfazqb.com/Article/details/gacojvbqe.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.vehdjk.com/Article/details/gkeanvnie.sHtML

[U108] JS：随机整数
来源：http://www.share.yfazqb.com/Article/details/gmagtsify.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.sjlbkw.cn/Article/details/gzbmptrxg.sHtML

[U109] JS：数组分组
来源：http://3g.fktsv.cn/Article/details/glubyajzd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.vehdjk.com/Article/details/gbdhdewzu.sHtML

[U110] JS：数组分块
来源：http://www.share.vehdjk.com/Article/details/gkxrpzwav.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.epnwcf.com/Article/details/gfjsekejv.sHtML

[U111] JS：对象转 Map
来源：http://3g.sjlbkw.cn/Article/details/gdmbnxtqu.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.vehdjk.com/Article/details/gkwriqval.sHtML

[U112] JS：字符串补位
来源：http://read.share.sjlbkw.cn/Article/details/gpmvgfqjh.sHtML

"7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/gzsmxxxsc.sHtML

[U113] JS：正则替换全部
来源：http://read.share.bbcook.cn/Article/details/gvbpjszsu.sHtML

s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gdagxzdpw.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.tarul.cn/Article/details/gpnxgmngh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.vehdjk.com/Article/details/giyingrdq.sHtML

[U115] JS：生成 UUID
来源：http://read.share.yfazqb.com/Article/details/gprvpwzjx.sHtML

crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gyvvclhvn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fktsv.cn/Article/details/gywwtgbdq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.tarul.cn/Article/details/gdyvzpcle.sHtML

[U117] JS：单元测试
来源：http://www.blog.yfazqb.com/Article/details/gljjgmmsw.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.vehdjk.com/Article/details/gijyapyjn.sHtML

[U118] JS：开发服务器
来源：http://baike.epnwcf.com/Article/details/gyozpqnny.sHtML

npm i -D vite;  npx vite
来源：http://read.share.yfazqb.com/Article/details/growvjgxh.sHtML

[U119] JS：生产构建
来源：http://3g.fktsv.cn/Article/details/gqrqbhlnh.sHtML

npx vite build
来源：http://www.blog.bbcook.cn/Article/details/gbxvrfrzr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.tarul.cn/Article/details/gbrittfta.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.sjlbkw.cn/Article/details/grbwiwrdx.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gcgpskmbe.sHtML

统计汇总
来源：http://www.share.epnwcf.com/Article/details/gbjgsikfl.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gmsoosdqx.sHtML

按语言统计（条）：
来源：http://www.blog.epnwcf.com/Article/details/gujyfidrf.sHtML

Python ......... 252
来源：http://3g.yfazqb.com/Article/details/gkxsijkoi.sHtML

PHP ............ 252
来源：http://www.blog.fktsv.cn/Article/details/gwmzejvly.sHtML

JavaScript ..... 252
来源：http://blog.tarul.cn/Article/details/gmpskzwho.sHtML

TypeScript ..... 212
来源：http://www.blog.epnwcf.com/Article/details/guuspvrns.sHtML

Java ........... 212
来源：http://www.share.sjlbkw.cn/Article/details/ghgjpxihb.sHtML

Go ............. 212
来源：http://m.share.tarul.cn/Article/details/goxvjwtky.sHtML

Ruby ........... 212
来源：http://blog.bbcook.cn/Article/details/gimlphgfh.sHtML

C# ............. 212
来源：http://blog.vehdjk.com/Article/details/guhyevhex.sHtML

C .............. 30
来源：http://m.share.tarul.cn/Article/details/gcwzjdgjw.sHtML

C++ ............ 30
来源：http://baike.fktsv.cn/Article/details/gaxipymkx.sHtML

SQL ............ 90
来源：http://3g.sjlbkw.cn/Article/details/gtpluukwa.sHtML

Bash ........... 80
来源：http://mobile.yfazqb.com/Article/details/grzqmysyg.sHtML

Kotlin ......... 15
来源：http://www.m.share.yfazqb.com/Article/details/gjrchgdjk.sHtML

Swift .......... 15
来源：http://www.blog.vehdjk.com/Article/details/gbvamkdql.sHtML

Lua ............ 10
来源：http://blog.sjlbkw.cn/Article/details/gbqbgikzq.sHtML

Perl ........... 10
来源：http://mobile.epnwcf.com/Article/details/gsgiouemo.sHtML

Scala .......... 10
来源：http://read.share.fktsv.cn/Article/details/gklmrssoy.sHtML

------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gcpghosto.sHtML

合计 ........... 2106 条
来源：http://www.share.yfazqb.com/Article/details/gqzttfvny.sHtML

按章节统计：
来源：http://baike.bbcook.cn/Article/details/gslkwnrxv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.epnwcf.com/Article/details/gcbvxgkom.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.tarul.cn/Article/details/gtvxyvpge.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.sjlbkw.cn/Article/details/gikcljsyb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.sjlbkw.cn/Article/details/gysxzhuqz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.sjlbkw.cn/Article/details/gqeekzbtw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.tarul.cn/Article/details/gbqbusqzi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.tarul.cn/Article/details/guxfcjihp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.yfazqb.com/Article/details/gbvywewlt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gwqczgwin.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.yfazqb.com/Article/details/gxbomdtco.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.sjlbkw.cn/Article/details/gxcpqwpam.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/grjpvemoa.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gennvobxq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fktsv.cn/Article/details/golarrecg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fktsv.cn/Article/details/ggngcixgi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gnrrfimem.sHtML

Q SQL 专题                              90
来源：http://mobile.bbcook.cn/Article/details/garwhgpas.sHtML

R Bash 专题                             80
来源：http://wap.fktsv.cn/Article/details/grjlnaysm.sHtML

S C / C++ 专题                          60
来源：http://wap.yfazqb.com/Article/details/gbfghxddj.sHtML

T 其他语言补充                          60
来源：http://m.share.yfazqb.com/Article/details/gnenikzcx.sHtML

U 高频实用片段                         120
来源：http://wap.sjlbkw.cn/Article/details/gtsbrutkk.sHtML

------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gnwvaceme.sHtML

合计                                  2106 条
来源：http://www.share.vehdjk.com/Article/details/gygbwpyed.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/godxfnfsc.sHtML

使用提醒
来源：http://www.m.share.epnwcf.com/Article/details/gdpisbyxz.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gyzupnqna.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.yfazqb.com/Article/details/gzkphgvyr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fktsv.cn/Article/details/gjkazyiok.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.tarul.cn/Article/details/gvggospqz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.epnwcf.com/Article/details/gsylponjc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.bbcook.cn/Article/details/giemhfigf.sHtML

—— 文件结束 ——
来源：http://www.m.share.vehdjk.com/Article/details/gvdlclkqh.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/geookavsi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.yfazqb.com/Article/details/gjjwcwvnc.sHtML

Common Programming Examples Cheat Book
来源：http://blog.epnwcf.com/Article/details/ghxqkdrkx.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gnakjedkl.sHtML

【收录内容】
来源：http://www.share.sjlbkw.cn/Article/details/gndxnkmgf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.bbcook.cn/Article/details/gofbhqnvw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.vehdjk.com/Article/details/gudfchaut.sHtML

SQL · Bash · C · C++
来源：http://wap.tarul.cn/Article/details/goxicbtyj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.yfazqb.com/Article/details/glupsmcwr.sHtML

【使用说明】
来源：http://www.share.tarul.cn/Article/details/gpfzkonkp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.tarul.cn/Article/details/glfctiidt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.sjlbkw.cn/Article/details/gspjyadfn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.yfazqb.com/Article/details/gddzhclrh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.vehdjk.com/Article/details/guzvdffad.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fktsv.cn/Article/details/gxxzrhaiv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.epnwcf.com/Article/details/gopgcvvvn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.vehdjk.com/Article/details/gevhkysko.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fktsv.cn/Article/details/gawlulwfy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.bbcook.cn/Article/details/glykrxyqf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.vehdjk.com/Article/details/gesvmmyko.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.tarul.cn/Article/details/gdrjavvpv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.sjlbkw.cn/Article/details/ganjtmcpg.sHtML

【文件统计】
来源：http://3g.vehdjk.com/Article/details/gfcdydjfi.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.tarul.cn/Article/details/gfpnxgldw.sHtML

--------------------------------------------------------------------------------
来源：http://3g.epnwcf.com/Article/details/goihrumzv.sHtML

目  录
来源：http://read.share.fktsv.cn/Article/details/gpaahzgwh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.yfazqb.com/Article/details/gyxoexpby.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fktsv.cn/Article/details/gmcueibjw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.yfazqb.com/Article/details/gdofnmyyn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.yfazqb.com/Article/details/giqirwzlt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fktsv.cn/Article/details/ghvcyoejg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.sjlbkw.cn/Article/details/gbzmlyzwy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.bbcook.cn/Article/details/ggfhkgdht.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fktsv.cn/Article/details/gwgcuaxia.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.tarul.cn/Article/details/gxuwtgyon.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gzqskhmsw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fktsv.cn/Article/details/gehxbodpv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/gqltdqmzr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/gtxtthwdg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/ghdkaquxl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.sjlbkw.cn/Article/details/gnnvwjxvi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fktsv.cn/Article/details/gmcifpneq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.epnwcf.com/Article/details/grqyfeoew.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.sjlbkw.cn/Article/details/gpquwkwgs.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.yfazqb.com/Article/details/gwqdyfkha.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.bbcook.cn/Article/details/gzzrgmgpq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.yfazqb.com/Article/details/grisxrfhv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.epnwcf.com/Article/details/gmffzdheb.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gdezcccvm.sHtML

A. 基础语法与类型
来源：http://www.blog.yfazqb.com/Article/details/gnpuqfvpl.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gwtzkhgtj.sHtML

[A01] Hello World
来源：http://www.blog.bbcook.cn/Article/details/gdmjyplhe.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.epnwcf.com/Article/details/gdictvjba.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.tarul.cn/Article/details/ggjinoemb.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.epnwcf.com/Article/details/gjwvstnhh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fktsv.cn/Article/details/goallofcn.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.epnwcf.com/Article/details/gqzfntvpq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.tarul.cn/Article/details/gmewdndta.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.bbcook.cn/Article/details/grkhvfkzh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.yfazqb.com/Article/details/gwesenxyu.sHtML

[A02] 变量声明与赋值
来源：http://wap.epnwcf.com/Article/details/gnrvhjzvn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.epnwcf.com/Article/details/ggegazszv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.bbcook.cn/Article/details/guyzckzxl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fktsv.cn/Article/details/ghefelofs.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.vehdjk.com/Article/details/gldxlikig.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gzwjqmibu.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.yfazqb.com/Article/details/gdyunrxzx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.vehdjk.com/Article/details/gnwgcmvjo.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.bbcook.cn/Article/details/gtclrkgpr.sHtML

[A03] 常量定义
来源：http://mobile.fktsv.cn/Article/details/gpiqjhwqt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.tarul.cn/Article/details/gaszxejzl.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gahtkpioc.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gvcoljbho.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gtkmvydwy.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/ggirjfkuu.sHtML

Go:   const PI = 3.14159
来源：http://baike.vehdjk.com/Article/details/gipjftfqx.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.bbcook.cn/Article/details/gnjoepmsq.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gusrdcjqj.sHtML

[A04] 判断变量类型
来源：http://m.share.tarul.cn/Article/details/gtsmrnmpr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.epnwcf.com/Article/details/grkfelvjs.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.yfazqb.com/Article/details/gmojzknlg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.yfazqb.com/Article/details/gogzmwgrx.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.sjlbkw.cn/Article/details/gfauehouy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.yfazqb.com/Article/details/ggevsjbmo.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.tarul.cn/Article/details/gehtzejkm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.bbcook.cn/Article/details/gyyocbeiv.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.epnwcf.com/Article/details/gtsxtztue.sHtML

[A05] 整数除法与取模
来源：http://read.share.tarul.cn/Article/details/gvwvmnync.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fktsv.cn/Article/details/gvcnnhuyz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gwwpzgrzy.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fktsv.cn/Article/details/gqgvlqmbe.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fktsv.cn/Article/details/gukcmsgdd.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.yfazqb.com/Article/details/gbtmtbeev.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.yfazqb.com/Article/details/gjiiaepqq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/ggzceqces.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gelskggyx.sHtML

[A06] 字符串转数字
来源：http://www.m.share.tarul.cn/Article/details/gyujectrn.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.sjlbkw.cn/Article/details/gdictkmoo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fktsv.cn/Article/details/gerpxweqn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fktsv.cn/Article/details/gmyylaxmb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.yfazqb.com/Article/details/gtavpsggo.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.vehdjk.com/Article/details/gkdjhjvbr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.epnwcf.com/Article/details/guxkfdlzt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.vehdjk.com/Article/details/gyobijbvi.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.bbcook.cn/Article/details/giwmkjhnq.sHtML

[A07] 数字转字符串
来源：http://read.share.fktsv.cn/Article/details/ggvfpgwdi.sHtML

Py:   str(42)
来源：http://blog.vehdjk.com/Article/details/gibcqgyqa.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.vehdjk.com/Article/details/gpyycvrfg.sHtML

JS:   String(42); (42).toString()
来源：http://3g.sjlbkw.cn/Article/details/gkvcbmepo.sHtML

TS:   String(42)
来源：http://baike.sjlbkw.cn/Article/details/gccyesyao.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.yfazqb.com/Article/details/gbbwvrxin.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxkwjvcq.sHtML

Ruby: 42.to_s
来源：http://m.share.yfazqb.com/Article/details/ghagsmzao.sHtML

C#:   42.ToString()
来源：http://mobile.tarul.cn/Article/details/giokhjsfx.sHtML

[A08] 取整与四舍五入
来源：http://read.share.yfazqb.com/Article/details/gzrundctp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.vehdjk.com/Article/details/gdtwhhnfl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.yfazqb.com/Article/details/gfobtrwpx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.yfazqb.com/Article/details/gdficqqgu.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.tarul.cn/Article/details/gpytxrfjv.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.bbcook.cn/Article/details/gxzfybbka.sHtML


<!-- 参考信息 -->