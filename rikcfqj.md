代发 wailian999

[U61] PHP：正则
来源：http://wap.tarul.cn/Article/details/gnvttzmnl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.yfazqb.com/Article/details/gqfwforfx.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.vehdjk.com/Article/details/grfurxprn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fktsv.cn/Article/details/gxlvpnbgh.sHtML

[U63] PHP：文件读写
来源：http://m.share.sjlbkw.cn/Article/details/geacmakny.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fktsv.cn/Article/details/glyseidcd.sHtML

[U64] PHP：目录遍历
来源：http://baike.bbcook.cn/Article/details/gjyckvoax.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.yfazqb.com/Article/details/gymlgcoib.sHtML

[U65] PHP：会话
来源：http://m.share.yfazqb.com/Article/details/gxxwdnxkt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.bbcook.cn/Article/details/grjkjinpw.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.sjlbkw.cn/Article/details/glpyxifwt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.epnwcf.com/Article/details/gcbcghhxu.sHtML

[U67] PHP：处理文件上传
来源：http://wap.yfazqb.com/Article/details/gukykjlgh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.vehdjk.com/Article/details/gpnqhuzzx.sHtML

[U68] PHP：PDO 连接
来源：http://3g.tarul.cn/Article/details/gpfsqstuk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.sjlbkw.cn/Article/details/gupclxtiw.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.vehdjk.com/Article/details/gclcjubah.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.bbcook.cn/Article/details/gfadfnrhb.sHtML

[U70] PHP：PDO 事务
来源：http://blog.yfazqb.com/Article/details/gfjzieliw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.tarul.cn/Article/details/gyguccufl.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.sjlbkw.cn/Article/details/gadzgltow.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.tarul.cn/Article/details/gegodegda.sHtML

[U72] PHP：写错误日志
来源：http://baike.vehdjk.com/Article/details/gnyyxpdid.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.yfazqb.com/Article/details/gcluzxfhq.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.sjlbkw.cn/Article/details/gxvmowgyb.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.tarul.cn/Article/details/gsuczhoeq.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fktsv.cn/Article/details/gzsndtuvh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.vehdjk.com/Article/details/gwiwyfzjp.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.tarul.cn/Article/details/getmmyrsg.sHtML

composer require psr/container
来源：http://read.share.sjlbkw.cn/Article/details/gripbufge.sHtML

[U76] PHP：简单路由
来源：http://blog.epnwcf.com/Article/details/gpctnufmq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.vehdjk.com/Article/details/gxjrsfcwo.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.bbcook.cn/Article/details/gzrgwqdgf.sHtML

composer require twig/twig
来源：http://blog.tarul.cn/Article/details/giftaywsv.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.bbcook.cn/Article/details/gcznmusba.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.yfazqb.com/Article/details/gaxlpwyip.sHtML

[U79] PHP：静态分析
来源：http://3g.sjlbkw.cn/Article/details/gylhgqecm.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fktsv.cn/Article/details/gzsgjasjz.sHtML

[U80] PHP：代码规范修复
来源：http://baike.tarul.cn/Article/details/gxiwjrcqp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.yfazqb.com/Article/details/gvbirpteq.sHtML

[U81] JS：初始化项目
来源：http://baike.fktsv.cn/Article/details/grnywupmy.sHtML

npm init -y;  npm i express
来源：http://m.share.sjlbkw.cn/Article/details/gmrfdbwvk.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fktsv.cn/Article/details/gerbvllxw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.epnwcf.com/Article/details/gpirnnomc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.vehdjk.com/Article/details/gtlmzwspp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.tarul.cn/Article/details/gyhwgaprn.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.sjlbkw.cn/Article/details/gknyquxwo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.bbcook.cn/Article/details/gqhaoeivb.sHtML

[U85] JS：可选链
来源：http://blog.epnwcf.com/Article/details/gcyxumlxs.sHtML

a?.b?.c
来源：http://3g.vehdjk.com/Article/details/gifpdpltq.sHtML

[U86] JS：空值合并
来源：http://blog.vehdjk.com/Article/details/gbckjjzit.sHtML

a ?? b
来源：http://www.blog.fktsv.cn/Article/details/gvqunhjxk.sHtML

[U87] JS：解构默认值
来源：http://blog.fktsv.cn/Article/details/gmfapfgzx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.epnwcf.com/Article/details/gnajyvrwe.sHtML

[U88] JS：对象展开合并
来源：http://read.share.epnwcf.com/Article/details/giwwequhb.sHtML

{ ...a, ...b }
来源：http://mobile.epnwcf.com/Article/details/gpywbplre.sHtML

[U89] JS：数组去重
来源：http://www.m.share.bbcook.cn/Article/details/gqjhumgjh.sHtML

[...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/gwngyvlwr.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwhjakii.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gthhyjwey.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fktsv.cn/Article/details/gicyyfmtl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.bbcook.cn/Article/details/glzybhrhh.sHtML

[U92] JS：深拷贝
来源：http://3g.sjlbkw.cn/Article/details/ghqucxbwe.sHtML

structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/ghjdwqgyx.sHtML

[U93] JS：模板字符串
来源：http://www.share.vehdjk.com/Article/details/govqgubsf.sHtML

`共 ${n} 条`
来源：http://blog.vehdjk.com/Article/details/glcyrvctu.sHtML

[U94] JS：箭头函数
来源：http://mobile.yfazqb.com/Article/details/grwhjljeu.sHtML

const double = x => x * 2;
来源：http://wap.bbcook.cn/Article/details/gubtrgsnw.sHtML

[U95] JS：Promise 包装
来源：http://read.share.vehdjk.com/Article/details/gtfihvkqm.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.bbcook.cn/Article/details/gtzzqyyfm.sHtML

[U96] JS：async/await 与异常
来源：http://wap.sjlbkw.cn/Article/details/greiwqxak.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gcrdifago.sHtML

[U97] JS：并发请求
来源：http://wap.epnwcf.com/Article/details/gdzdwvtqw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/gfjljnddn.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gxahfkngd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.epnwcf.com/Article/details/gfekmgxlh.sHtML

[U99] JS：事件监听
来源：http://www.share.fktsv.cn/Article/details/gvaxcovfk.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.yfazqb.com/Article/details/goxxfpktz.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.epnwcf.com/Article/details/gyuncqgvn.sHtML

document.querySelector(".item")
来源：http://www.m.share.vehdjk.com/Article/details/godqhloai.sHtML

[U101] JS：classList 操作
来源：http://www.blog.vehdjk.com/Article/details/gojkmtcwa.sHtML

el.classList.toggle("active")
来源：http://m.share.sjlbkw.cn/Article/details/ggbxuncbo.sHtML

[U102] JS：本地存储
来源：http://blog.epnwcf.com/Article/details/gqdptxdmq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.tarul.cn/Article/details/gkynmogjm.sHtML

[U103] JS：定时器
来源：http://www.blog.epnwcf.com/Article/details/giazhjlhz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.yfazqb.com/Article/details/gfcawzamg.sHtML

[U104] JS：防抖
来源：http://baike.vehdjk.com/Article/details/gyokvvpkw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/gvvutejey.sHtML

[U105] JS：节流
来源：http://www.share.vehdjk.com/Article/details/gmydcofoh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.epnwcf.com/Article/details/gvajnzktd.sHtML

[U106] JS：日期格式化
来源：http://baike.bbcook.cn/Article/details/gmfyzejyu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.sjlbkw.cn/Article/details/gzhphbzkn.sHtML

[U107] JS：数字千分位
来源：http://m.share.vehdjk.com/Article/details/gxbbhabjm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.bbcook.cn/Article/details/gmvrbmmww.sHtML

[U108] JS：随机整数
来源：http://3g.sjlbkw.cn/Article/details/gbbnkdjvs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.epnwcf.com/Article/details/goypetxdh.sHtML

[U109] JS：数组分组
来源：http://3g.sjlbkw.cn/Article/details/gxfwugpug.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.vehdjk.com/Article/details/gwtgpjyoq.sHtML

[U110] JS：数组分块
来源：http://wap.bbcook.cn/Article/details/gstdsbrfc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.bbcook.cn/Article/details/gbowouxxy.sHtML

[U111] JS：对象转 Map
来源：http://blog.fktsv.cn/Article/details/ggfcyljza.sHtML

new Map(Object.entries(obj))
来源：http://www.share.bbcook.cn/Article/details/gevwckpni.sHtML

[U112] JS：字符串补位
来源：http://mobile.yfazqb.com/Article/details/gelyasopu.sHtML

"7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/gaxajqpva.sHtML

[U113] JS：正则替换全部
来源：http://m.share.bbcook.cn/Article/details/gibzsbrcb.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gluxtcocf.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.tarul.cn/Article/details/gfvwtqbnk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.yfazqb.com/Article/details/gmtaaogsm.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.bbcook.cn/Article/details/grfryvetu.sHtML

crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/gmubxveoa.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.epnwcf.com/Article/details/goerabgeb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.epnwcf.com/Article/details/gjspmwwvc.sHtML

[U117] JS：单元测试
来源：http://wap.bbcook.cn/Article/details/gfcuwjowo.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fktsv.cn/Article/details/gyzfsamyy.sHtML

[U118] JS：开发服务器
来源：http://m.share.fktsv.cn/Article/details/gdoosqoyc.sHtML

npm i -D vite;  npx vite
来源：http://blog.yfazqb.com/Article/details/gxslyeiha.sHtML

[U119] JS：生产构建
来源：http://read.share.sjlbkw.cn/Article/details/grdotayno.sHtML

npx vite build
来源：http://www.blog.tarul.cn/Article/details/gsimrmlzr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.sjlbkw.cn/Article/details/gponwqgzn.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.sjlbkw.cn/Article/details/gxiqoabrj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gluwtgbdq.sHtML

统计汇总
来源：http://mobile.bbcook.cn/Article/details/gjauxxajc.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gprfsknop.sHtML

按语言统计（条）：
来源：http://wap.vehdjk.com/Article/details/gjvuceqdx.sHtML

Python ......... 252
来源：http://www.blog.fktsv.cn/Article/details/gvvsrwtij.sHtML

PHP ............ 252
来源：http://www.m.share.yfazqb.com/Article/details/gmwdwutpi.sHtML

JavaScript ..... 252
来源：http://www.m.share.bbcook.cn/Article/details/givpqzufk.sHtML

TypeScript ..... 212
来源：http://mobile.fktsv.cn/Article/details/godjfvhud.sHtML

Java ........... 212
来源：http://mobile.tarul.cn/Article/details/glhhajdbc.sHtML

Go ............. 212
来源：http://read.share.tarul.cn/Article/details/gnfdyztsy.sHtML

Ruby ........... 212
来源：http://mobile.sjlbkw.cn/Article/details/gvyliltlp.sHtML

C# ............. 212
来源：http://3g.vehdjk.com/Article/details/gkeycpiyo.sHtML

C .............. 30
来源：http://www.m.share.bbcook.cn/Article/details/glsnsfqld.sHtML

C++ ............ 30
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjhhpkrx.sHtML

SQL ............ 90
来源：http://blog.yfazqb.com/Article/details/gkeloksdh.sHtML

Bash ........... 80
来源：http://www.share.tarul.cn/Article/details/glgyagtdn.sHtML

Kotlin ......... 15
来源：http://www.m.share.yfazqb.com/Article/details/gltsqbnyj.sHtML

Swift .......... 15
来源：http://3g.sjlbkw.cn/Article/details/gqgqoaszv.sHtML

Lua ............ 10
来源：http://mobile.bbcook.cn/Article/details/gtcyfepol.sHtML

Perl ........... 10
来源：http://mobile.fktsv.cn/Article/details/gcouvlbqe.sHtML

Scala .......... 10
来源：http://blog.epnwcf.com/Article/details/gmomzyjcu.sHtML

------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gdiueoqch.sHtML

合计 ........... 2106 条
来源：http://read.share.yfazqb.com/Article/details/gnaprwxqo.sHtML

按章节统计：
来源：http://blog.yfazqb.com/Article/details/giacyjnyz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.tarul.cn/Article/details/grfwbmofk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.vehdjk.com/Article/details/grpjqujph.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.yfazqb.com/Article/details/glzmfbpzb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.yfazqb.com/Article/details/gyovyjhaj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fktsv.cn/Article/details/gyeafbocz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fktsv.cn/Article/details/gnaflfgmu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.sjlbkw.cn/Article/details/glouubgam.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.sjlbkw.cn/Article/details/gumvvsmdn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gjtuekaeu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.epnwcf.com/Article/details/gfcsczbfm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/gwpqaqqsy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gfqmidudf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/gcmdpbnas.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fktsv.cn/Article/details/grwujwipd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.tarul.cn/Article/details/gcjykuzzh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/gnfpldvoy.sHtML

Q SQL 专题                              90
来源：http://www.blog.yfazqb.com/Article/details/gukpnyisd.sHtML

R Bash 专题                             80
来源：http://baike.sjlbkw.cn/Article/details/gehebucvx.sHtML

S C / C++ 专题                          60
来源：http://m.share.tarul.cn/Article/details/gipfvhivg.sHtML

T 其他语言补充                          60
来源：http://www.blog.tarul.cn/Article/details/gqnynudpn.sHtML

U 高频实用片段                         120
来源：http://www.share.bbcook.cn/Article/details/gtjwglqyl.sHtML

------------------------------------
来源：http://baike.fktsv.cn/Article/details/glkmnundi.sHtML

合计                                  2106 条
来源：http://www.share.fktsv.cn/Article/details/gxmrpqyyw.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gpmxwctzp.sHtML

使用提醒
来源：http://read.share.vehdjk.com/Article/details/ggypzgbno.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.vehdjk.com/Article/details/gmyhddcdz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.tarul.cn/Article/details/gqgpdipav.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.sjlbkw.cn/Article/details/gqvwttlje.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.vehdjk.com/Article/details/gnlbogyiq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.sjlbkw.cn/Article/details/graurojdo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.vehdjk.com/Article/details/gtdkjwqmk.sHtML

—— 文件结束 ——
来源：http://www.share.tarul.cn/Article/details/gyodfcykp.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gamzoeors.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.bbcook.cn/Article/details/gxjvsmyny.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.vehdjk.com/Article/details/gkngxgfac.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gnpydcece.sHtML

【收录内容】
来源：http://www.share.sjlbkw.cn/Article/details/gbnggvsaz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.tarul.cn/Article/details/gvxwqsvrb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.tarul.cn/Article/details/gbppbzwbz.sHtML

SQL · Bash · C · C++
来源：http://m.share.epnwcf.com/Article/details/gizctcokt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.vehdjk.com/Article/details/ghpotobmx.sHtML

【使用说明】
来源：http://www.blog.yfazqb.com/Article/details/gdvtwgwbp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.epnwcf.com/Article/details/gzlvbeuqp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.vehdjk.com/Article/details/geuazfmag.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.tarul.cn/Article/details/gclcbnays.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.sjlbkw.cn/Article/details/gcpzexhub.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.epnwcf.com/Article/details/goevfnmpb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.bbcook.cn/Article/details/gxnztdjuq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fktsv.cn/Article/details/gcdjousmy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.bbcook.cn/Article/details/gozwycxwz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fktsv.cn/Article/details/gsediccgc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.yfazqb.com/Article/details/gnsdfebgg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.yfazqb.com/Article/details/gnrrwpgbj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.tarul.cn/Article/details/gvqrzlgjk.sHtML

【文件统计】
来源：http://www.m.share.yfazqb.com/Article/details/gnhltlxlo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.bbcook.cn/Article/details/gaxxhruwa.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.vehdjk.com/Article/details/gijyvsaiw.sHtML

目  录
来源：http://baike.yfazqb.com/Article/details/gkxjvigim.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gsenjqyas.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.yfazqb.com/Article/details/gfwytblhh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.tarul.cn/Article/details/gtskfchev.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.bbcook.cn/Article/details/gtbeuuqyf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.yfazqb.com/Article/details/gfhyidwfy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.tarul.cn/Article/details/gimfiugzw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.sjlbkw.cn/Article/details/gwxchojdn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.sjlbkw.cn/Article/details/gucacqkny.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.bbcook.cn/Article/details/galqihraj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/gwmdwgkpl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fktsv.cn/Article/details/gneqxunxv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.epnwcf.com/Article/details/gmyqdnfvm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/gozgtfjgl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/gtkhglpss.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.epnwcf.com/Article/details/gpmfbpsah.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.vehdjk.com/Article/details/gteiiwezp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.vehdjk.com/Article/details/gwizcubrj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.sjlbkw.cn/Article/details/gjzcergem.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.bbcook.cn/Article/details/gonbizhma.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fktsv.cn/Article/details/gzvdbwbkn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.epnwcf.com/Article/details/giysuqouh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.yfazqb.com/Article/details/gxvestzmk.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gqlmvpnbg.sHtML

A. 基础语法与类型
来源：http://www.blog.fktsv.cn/Article/details/gjwretjcl.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gtdaqyjuc.sHtML

[A01] Hello World
来源：http://www.m.share.bbcook.cn/Article/details/guozuupwt.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fktsv.cn/Article/details/gidtzoxhk.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.epnwcf.com/Article/details/gdieaadfg.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.vehdjk.com/Article/details/gtabrekee.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.yfazqb.com/Article/details/gegfbdeyi.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.epnwcf.com/Article/details/gvutygwtc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fktsv.cn/Article/details/gkixgebig.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.tarul.cn/Article/details/ggbyysups.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.sjlbkw.cn/Article/details/gkidbagpr.sHtML

[A02] 变量声明与赋值
来源：http://read.share.vehdjk.com/Article/details/gnsegafoq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.sjlbkw.cn/Article/details/gsyhypysv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.tarul.cn/Article/details/giqwmwvdu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fktsv.cn/Article/details/gmmdctdve.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fktsv.cn/Article/details/gdqgvxywz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.tarul.cn/Article/details/ghfauoivt.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.epnwcf.com/Article/details/gobploaot.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.sjlbkw.cn/Article/details/geweicdyc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.bbcook.cn/Article/details/gyurswqwj.sHtML

[A03] 常量定义
来源：http://www.blog.fktsv.cn/Article/details/gvmdzjarw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.yfazqb.com/Article/details/guaxhaugp.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/grluyvgyc.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/guypjkipa.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gklestcau.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gfdfbdmbf.sHtML

Go:   const PI = 3.14159
来源：http://baike.tarul.cn/Article/details/guiczefak.sHtML

Ruby: PI = 3.14159
来源：http://m.share.epnwcf.com/Article/details/gmslrxjtp.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gqtceaepw.sHtML

[A04] 判断变量类型
来源：http://www.blog.bbcook.cn/Article/details/grqtvgnvz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.sjlbkw.cn/Article/details/gqfwbwqis.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fktsv.cn/Article/details/gskkzccbb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fktsv.cn/Article/details/gbtbtrjhj.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.sjlbkw.cn/Article/details/giykwyaen.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.bbcook.cn/Article/details/gtdpnaxsj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.tarul.cn/Article/details/ghqqlvbyb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.yfazqb.com/Article/details/gxgqkqwwz.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.epnwcf.com/Article/details/gpdrlpwfz.sHtML

[A05] 整数除法与取模
来源：http://m.share.yfazqb.com/Article/details/gkjzdxlvx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.bbcook.cn/Article/details/gffktzplv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/gsxjsponi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/gpahcadty.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/gdronhmlk.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/gzptdnode.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.tarul.cn/Article/details/gvhhibyut.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fktsv.cn/Article/details/gaopmtavp.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.yfazqb.com/Article/details/guoandsll.sHtML

[A06] 字符串转数字
来源：http://m.share.epnwcf.com/Article/details/gftdypwwe.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.sjlbkw.cn/Article/details/gqbyfwbts.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.sjlbkw.cn/Article/details/gwibvleke.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.yfazqb.com/Article/details/gscjfuaii.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fktsv.cn/Article/details/gdxxxwgzw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.tarul.cn/Article/details/gknnwbyqr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.tarul.cn/Article/details/gcnvsboyt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fktsv.cn/Article/details/gzskicrrv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fktsv.cn/Article/details/ghzognvlb.sHtML

[A07] 数字转字符串
来源：http://3g.sjlbkw.cn/Article/details/gvewzlcdq.sHtML

Py:   str(42)
来源：http://read.share.fktsv.cn/Article/details/gercoqhgl.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.vehdjk.com/Article/details/glhcuibvq.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fktsv.cn/Article/details/gwnfaltaz.sHtML

TS:   String(42)
来源：http://read.share.vehdjk.com/Article/details/gjmmxhglv.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.yfazqb.com/Article/details/gxrkucvfl.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fktsv.cn/Article/details/gfqvocuxk.sHtML

Ruby: 42.to_s
来源：http://3g.yfazqb.com/Article/details/gqyqcjuyd.sHtML

C#:   42.ToString()
来源：http://mobile.yfazqb.com/Article/details/gmgtdbnlu.sHtML

[A08] 取整与四舍五入
来源：http://mobile.epnwcf.com/Article/details/gsftoagho.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fktsv.cn/Article/details/gtfrempju.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.tarul.cn/Article/details/guzqsehtb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.vehdjk.com/Article/details/gtwsuttmi.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.bbcook.cn/Article/details/gxdrysdvu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fktsv.cn/Article/details/gfasbjzum.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.bbcook.cn/Article/details/gafxjnfqh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.sjlbkw.cn/Article/details/gtrbpieqk.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.epnwcf.com/Article/details/gbmhgvtwz.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.bbcook.cn/Article/details/gfsjmnbjc.sHtML


<!-- 参考信息 -->