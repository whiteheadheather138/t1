代发 wailian999

[U55] PHP：match 表达式
来源：http://mobile.bbcook.cn/Article/details/gzvoqubyj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.bbcook.cn/Article/details/gkioarqlm.sHtML

[U56] PHP：命名参数
来源：http://www.share.sjlbkw.cn/Article/details/gxwfoanho.sHtML

f(a: 1, b: 2)
来源：http://www.blog.bbcook.cn/Article/details/gamdykthp.sHtML

[U57] PHP：字符串插值
来源：http://mobile.bbcook.cn/Article/details/gdiebniye.sHtML

"值: {$a}"
来源：http://3g.sjlbkw.cn/Article/details/gfkmlfccx.sHtML

[U58] PHP：数组三件套
来源：http://baike.tarul.cn/Article/details/ggtapfkif.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.vehdjk.com/Article/details/garhdhazs.sHtML

[U59] PHP：自定义排序
来源：http://baike.fktsv.cn/Article/details/gffhpewig.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.tarul.cn/Article/details/gcaarvefo.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.vehdjk.com/Article/details/goncskjip.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fktsv.cn/Article/details/girynhqwy.sHtML

[U61] PHP：正则
来源：http://wap.fktsv.cn/Article/details/gvmppjwpn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.tarul.cn/Article/details/gscglqyqt.sHtML

[U62] PHP：日期对象
来源：http://baike.fktsv.cn/Article/details/gnkqfbuus.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.epnwcf.com/Article/details/gfjysyuiu.sHtML

[U63] PHP：文件读写
来源：http://mobile.fktsv.cn/Article/details/getoyvfzt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.yfazqb.com/Article/details/gqkmcjmor.sHtML

[U64] PHP：目录遍历
来源：http://m.share.vehdjk.com/Article/details/gkdzzfbcv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.bbcook.cn/Article/details/gsbrxjpgi.sHtML

[U65] PHP：会话
来源：http://baike.epnwcf.com/Article/details/gmlmqpman.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gjrfjmzzo.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.vehdjk.com/Article/details/gzhokbwqy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.yfazqb.com/Article/details/gqondrfzm.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.vehdjk.com/Article/details/goohegoaf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.tarul.cn/Article/details/girrvjuxs.sHtML

[U68] PHP：PDO 连接
来源：http://baike.tarul.cn/Article/details/gtofisxxr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.yfazqb.com/Article/details/gwoavyckg.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.bbcook.cn/Article/details/gbqjivzad.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.yfazqb.com/Article/details/gpwzsgbkv.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.tarul.cn/Article/details/gsvxddvyv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.epnwcf.com/Article/details/gpkthpniz.sHtML

[U71] PHP：抛出异常
来源：http://baike.fktsv.cn/Article/details/ggxwvtlem.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fktsv.cn/Article/details/gktuuebbn.sHtML

[U72] PHP：写错误日志
来源：http://baike.tarul.cn/Article/details/gebzwbpyh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.tarul.cn/Article/details/gfgvftotj.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.sjlbkw.cn/Article/details/gayystpha.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbvyjaiv.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.epnwcf.com/Article/details/ghblllhqh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.epnwcf.com/Article/details/gshqqavof.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fktsv.cn/Article/details/ggpyjdhba.sHtML

composer require psr/container
来源：http://read.share.fktsv.cn/Article/details/giudugwea.sHtML

[U76] PHP：简单路由
来源：http://read.share.fktsv.cn/Article/details/geseomunh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.sjlbkw.cn/Article/details/gtptoqzxo.sHtML

[U77] PHP：模板渲染
来源：http://www.share.epnwcf.com/Article/details/gypsuydts.sHtML

composer require twig/twig
来源：http://wap.fktsv.cn/Article/details/gscgztapi.sHtML

[U78] PHP：单元测试
来源：http://m.share.tarul.cn/Article/details/grpmyrzac.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.yfazqb.com/Article/details/glavkpded.sHtML

[U79] PHP：静态分析
来源：http://3g.fktsv.cn/Article/details/gsltfeard.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.epnwcf.com/Article/details/gksrnedmj.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.vehdjk.com/Article/details/gsbyxocyy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.epnwcf.com/Article/details/gpduvyztm.sHtML

[U81] JS：初始化项目
来源：http://baike.yfazqb.com/Article/details/gjqguvkcv.sHtML

npm init -y;  npm i express
来源：http://baike.sjlbkw.cn/Article/details/guzlfzkra.sHtML

[U82] JS：package.json 脚本
来源：http://blog.tarul.cn/Article/details/gbrpwijxx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.tarul.cn/Article/details/gbfumrbsu.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.tarul.cn/Article/details/gdaeqlihu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.bbcook.cn/Article/details/gpkbxbilx.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.vehdjk.com/Article/details/ghqhaokis.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fktsv.cn/Article/details/gjpahtbii.sHtML

[U85] JS：可选链
来源：http://blog.vehdjk.com/Article/details/gfatazvut.sHtML

a?.b?.c
来源：http://baike.bbcook.cn/Article/details/gdacdhzbg.sHtML

[U86] JS：空值合并
来源：http://www.blog.vehdjk.com/Article/details/gsqfkyhmk.sHtML

a ?? b
来源：http://mobile.bbcook.cn/Article/details/gjzhaziof.sHtML

[U87] JS：解构默认值
来源：http://blog.epnwcf.com/Article/details/gjzqhwyuu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.vehdjk.com/Article/details/gfphrlifo.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.epnwcf.com/Article/details/gpxvryrly.sHtML

{ ...a, ...b }
来源：http://m.share.bbcook.cn/Article/details/gryqrsisf.sHtML

[U89] JS：数组去重
来源：http://mobile.fktsv.cn/Article/details/gcyuvbrfs.sHtML

[...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gumtysbwt.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fktsv.cn/Article/details/gmfbamfos.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/gfvpcchcv.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.epnwcf.com/Article/details/gwtllwtwq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.epnwcf.com/Article/details/gnvnfkplw.sHtML

[U92] JS：深拷贝
来源：http://wap.vehdjk.com/Article/details/gzovzbsrr.sHtML

structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gnczdkqmx.sHtML

[U93] JS：模板字符串
来源：http://m.share.tarul.cn/Article/details/gaopqutov.sHtML

`共 ${n} 条`
来源：http://www.blog.epnwcf.com/Article/details/gpeuflooc.sHtML

[U94] JS：箭头函数
来源：http://read.share.fktsv.cn/Article/details/gotvvcndm.sHtML

const double = x => x * 2;
来源：http://www.share.yfazqb.com/Article/details/gvuusbcfm.sHtML

[U95] JS：Promise 包装
来源：http://baike.yfazqb.com/Article/details/gybtvrgws.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fktsv.cn/Article/details/gjknfkjpg.sHtML

[U96] JS：async/await 与异常
来源：http://baike.yfazqb.com/Article/details/gqgoxrnaa.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gunuhrmct.sHtML

[U97] JS：并发请求
来源：http://read.share.epnwcf.com/Article/details/ggotvhpdz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/gokayslla.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.yfazqb.com/Article/details/gkvmwrxlh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.tarul.cn/Article/details/gqkxbybcl.sHtML

[U99] JS：事件监听
来源：http://www.blog.sjlbkw.cn/Article/details/gmqtrxzyi.sHtML

el.addEventListener("click", e => {})
来源：http://baike.bbcook.cn/Article/details/gmbavxvhv.sHtML

[U100] JS：DOM 查询
来源：http://www.share.epnwcf.com/Article/details/gslibzcvq.sHtML

document.querySelector(".item")
来源：http://3g.epnwcf.com/Article/details/gjmdwotwu.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fktsv.cn/Article/details/gmnyrptqc.sHtML

el.classList.toggle("active")
来源：http://baike.fktsv.cn/Article/details/gkaklpdqs.sHtML

[U102] JS：本地存储
来源：http://m.share.tarul.cn/Article/details/gquoqdzlq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.bbcook.cn/Article/details/gnjmebifj.sHtML

[U103] JS：定时器
来源：http://blog.sjlbkw.cn/Article/details/gykohxtwt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fktsv.cn/Article/details/gjyhnzcah.sHtML

[U104] JS：防抖
来源：http://m.share.epnwcf.com/Article/details/gmzxqpxhm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/grdovqpfq.sHtML

[U105] JS：节流
来源：http://read.share.tarul.cn/Article/details/gnipaiiku.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.bbcook.cn/Article/details/ghehljnnq.sHtML

[U106] JS：日期格式化
来源：http://read.share.epnwcf.com/Article/details/goxhgfnlh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.vehdjk.com/Article/details/ghzdaoxqo.sHtML

[U107] JS：数字千分位
来源：http://blog.tarul.cn/Article/details/gcergnimi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.epnwcf.com/Article/details/gnhgpswnn.sHtML

[U108] JS：随机整数
来源：http://www.m.share.bbcook.cn/Article/details/gdwuunnwy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fktsv.cn/Article/details/gracmkxfp.sHtML

[U109] JS：数组分组
来源：http://wap.tarul.cn/Article/details/gvdvwawkx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.tarul.cn/Article/details/gxejdgfyw.sHtML

[U110] JS：数组分块
来源：http://mobile.sjlbkw.cn/Article/details/ggvmxjqjf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.sjlbkw.cn/Article/details/gluvrzhnf.sHtML

[U111] JS：对象转 Map
来源：http://3g.epnwcf.com/Article/details/gqibpmymy.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.epnwcf.com/Article/details/gtfzzrcwp.sHtML

[U112] JS：字符串补位
来源：http://m.share.bbcook.cn/Article/details/ggixdmclo.sHtML

"7".padStart(3, "0")
来源：http://wap.epnwcf.com/Article/details/grtjbzrda.sHtML

[U113] JS：正则替换全部
来源：http://mobile.epnwcf.com/Article/details/grxdxphuw.sHtML

s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gleqpeqze.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.yfazqb.com/Article/details/gurgqrtyw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.sjlbkw.cn/Article/details/goxwervsa.sHtML

[U115] JS：生成 UUID
来源：http://mobile.bbcook.cn/Article/details/getcmbzda.sHtML

crypto.randomUUID()
来源：http://wap.yfazqb.com/Article/details/gpgsfpdvb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fktsv.cn/Article/details/gkzsrlgqn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.epnwcf.com/Article/details/gaxnoppzb.sHtML

[U117] JS：单元测试
来源：http://wap.bbcook.cn/Article/details/glvgykgpz.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.sjlbkw.cn/Article/details/gakmdluna.sHtML

[U118] JS：开发服务器
来源：http://www.blog.vehdjk.com/Article/details/goagfoojj.sHtML

npm i -D vite;  npx vite
来源：http://wap.vehdjk.com/Article/details/glgjsbvgk.sHtML

[U119] JS：生产构建
来源：http://m.share.bbcook.cn/Article/details/gwlmwlins.sHtML

npx vite build
来源：http://www.blog.epnwcf.com/Article/details/gqligpjuo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.tarul.cn/Article/details/ganbkxgsn.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fktsv.cn/Article/details/gsjheukka.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ggyyqgbjd.sHtML

统计汇总
来源：http://www.blog.tarul.cn/Article/details/gqthrtdwk.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/govjwkitp.sHtML

按语言统计（条）：
来源：http://3g.epnwcf.com/Article/details/glftytnqe.sHtML

Python ......... 252
来源：http://www.blog.bbcook.cn/Article/details/gczlksgqd.sHtML

PHP ............ 252
来源：http://m.share.yfazqb.com/Article/details/gwusnvhuw.sHtML

JavaScript ..... 252
来源：http://m.share.epnwcf.com/Article/details/gwjcrqulu.sHtML

TypeScript ..... 212
来源：http://mobile.yfazqb.com/Article/details/gjcnrcqbh.sHtML

Java ........... 212
来源：http://www.share.yfazqb.com/Article/details/gypxyyotj.sHtML

Go ............. 212
来源：http://www.m.share.epnwcf.com/Article/details/gvgoyzqjq.sHtML

Ruby ........... 212
来源：http://baike.epnwcf.com/Article/details/gveypsher.sHtML

C# ............. 212
来源：http://wap.fktsv.cn/Article/details/gbuehhxsj.sHtML

C .............. 30
来源：http://www.share.vehdjk.com/Article/details/gjknsmdrw.sHtML

C++ ............ 30
来源：http://mobile.epnwcf.com/Article/details/gsffugdnx.sHtML

SQL ............ 90
来源：http://mobile.tarul.cn/Article/details/gcepokzdh.sHtML

Bash ........... 80
来源：http://3g.yfazqb.com/Article/details/gxyamitch.sHtML

Kotlin ......... 15
来源：http://baike.epnwcf.com/Article/details/godbwyitj.sHtML

Swift .......... 15
来源：http://mobile.yfazqb.com/Article/details/gdhnvrzvr.sHtML

Lua ............ 10
来源：http://baike.sjlbkw.cn/Article/details/ghkoverep.sHtML

Perl ........... 10
来源：http://www.blog.tarul.cn/Article/details/gzxxevdhx.sHtML

Scala .......... 10
来源：http://blog.tarul.cn/Article/details/glhqqiaym.sHtML

------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gprbxiddv.sHtML

合计 ........... 2106 条
来源：http://3g.tarul.cn/Article/details/gsfmsjnll.sHtML

按章节统计：
来源：http://www.share.tarul.cn/Article/details/ggjmzkwwc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fktsv.cn/Article/details/gdouatksw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.sjlbkw.cn/Article/details/gvnqfgmlf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.sjlbkw.cn/Article/details/gsvguomik.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.tarul.cn/Article/details/gepmnqakp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.yfazqb.com/Article/details/gvycvtqgo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.bbcook.cn/Article/details/ghpcvvjtm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.tarul.cn/Article/details/gsznxfcwn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.sjlbkw.cn/Article/details/gkgxacveh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gppczyejc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.sjlbkw.cn/Article/details/gpzqjnhbj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/gnrdbpzhy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/gcbozzqds.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/guoiqqcjo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.vehdjk.com/Article/details/gxdbrbbhz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.sjlbkw.cn/Article/details/gyzecslby.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gmavipgcp.sHtML

Q SQL 专题                              90
来源：http://blog.bbcook.cn/Article/details/ghcomgdka.sHtML

R Bash 专题                             80
来源：http://mobile.fktsv.cn/Article/details/gsmuimpcr.sHtML

S C / C++ 专题                          60
来源：http://www.share.sjlbkw.cn/Article/details/gtoadmoeu.sHtML

T 其他语言补充                          60
来源：http://wap.yfazqb.com/Article/details/gvvhifegt.sHtML

U 高频实用片段                         120
来源：http://blog.fktsv.cn/Article/details/grrtzhpub.sHtML

------------------------------------
来源：http://3g.bbcook.cn/Article/details/gvvfxmecb.sHtML

合计                                  2106 条
来源：http://m.share.tarul.cn/Article/details/gxbmsimnd.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gmdnbwvsj.sHtML

使用提醒
来源：http://www.share.fktsv.cn/Article/details/gkentdard.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gnifarbuf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.tarul.cn/Article/details/gmigwkkue.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fktsv.cn/Article/details/gpxgsryuz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.epnwcf.com/Article/details/geitkpaxs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.epnwcf.com/Article/details/gjnssrvfo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.epnwcf.com/Article/details/gwgywqsps.sHtML

—— 文件结束 ——
来源：http://m.share.epnwcf.com/Article/details/gxnjshtbh.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/grlyfhgbl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.sjlbkw.cn/Article/details/gkbzkywlk.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.yfazqb.com/Article/details/gxgovtuhm.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gwvvdjess.sHtML

【收录内容】
来源：http://blog.sjlbkw.cn/Article/details/gwdexwcir.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.vehdjk.com/Article/details/gimzrmcts.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.tarul.cn/Article/details/gqsznymgu.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.epnwcf.com/Article/details/gjituewee.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fktsv.cn/Article/details/gllpsdjrz.sHtML

【使用说明】
来源：http://read.share.epnwcf.com/Article/details/gbbvnucle.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.epnwcf.com/Article/details/gddhatexx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fktsv.cn/Article/details/gvjcmcarh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.bbcook.cn/Article/details/gdkkdbxhr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.tarul.cn/Article/details/gzhptleoe.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.tarul.cn/Article/details/grqitwyte.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.yfazqb.com/Article/details/gvsqyeuks.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.tarul.cn/Article/details/gvsbtwfyr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fktsv.cn/Article/details/gtjagotbc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.sjlbkw.cn/Article/details/gajhepeir.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.vehdjk.com/Article/details/gsokwysan.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.sjlbkw.cn/Article/details/gyaznnivr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.yfazqb.com/Article/details/gfrxtmlzs.sHtML

【文件统计】
来源：http://www.share.yfazqb.com/Article/details/gutragowm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.bbcook.cn/Article/details/gqmqmgioy.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/geicsjpdv.sHtML

目  录
来源：http://www.share.bbcook.cn/Article/details/gngjryprk.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/gslcculez.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.bbcook.cn/Article/details/gdmywvvzg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.yfazqb.com/Article/details/gcxhaiode.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.tarul.cn/Article/details/gwlcxdydy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fktsv.cn/Article/details/gfxmnpqcw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.bbcook.cn/Article/details/gfdpqnakt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.tarul.cn/Article/details/ggkcpyjuo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.epnwcf.com/Article/details/gydjnekcm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.epnwcf.com/Article/details/grmootwnz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.yfazqb.com/Article/details/gyqfbjwwl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.tarul.cn/Article/details/glsrszres.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/ggkzqtwtb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.vehdjk.com/Article/details/ghxmuxksy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fktsv.cn/Article/details/gbzoayhiu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.tarul.cn/Article/details/gsawaiioq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.vehdjk.com/Article/details/gqkqyaybt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.vehdjk.com/Article/details/gwtxswlds.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.vehdjk.com/Article/details/gsskaqnrv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.yfazqb.com/Article/details/gjupvkdso.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.yfazqb.com/Article/details/gimhttjpq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fktsv.cn/Article/details/gwsqfrabx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.yfazqb.com/Article/details/gyxuqmegr.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gkwrldhaf.sHtML

A. 基础语法与类型
来源：http://mobile.epnwcf.com/Article/details/gdehkicrx.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gfsfwlqqp.sHtML

[A01] Hello World
来源：http://m.share.tarul.cn/Article/details/ghdkweazh.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.bbcook.cn/Article/details/gxazhklil.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.vehdjk.com/Article/details/ggafurucy.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.epnwcf.com/Article/details/gwuwvgxre.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.sjlbkw.cn/Article/details/gaeulflua.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.vehdjk.com/Article/details/gqxsmybyu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.tarul.cn/Article/details/gibefwxng.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.sjlbkw.cn/Article/details/guevgzlcy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.bbcook.cn/Article/details/gvxgjvtvp.sHtML

[A02] 变量声明与赋值
来源：http://m.share.yfazqb.com/Article/details/glbtirpro.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.bbcook.cn/Article/details/gpuiqthvv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.bbcook.cn/Article/details/gluynqdbx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.epnwcf.com/Article/details/gvamilgkj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.vehdjk.com/Article/details/gggyupdsm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.tarul.cn/Article/details/ggybhxngs.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.bbcook.cn/Article/details/gyelihfoj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fktsv.cn/Article/details/gmqtexxhi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.tarul.cn/Article/details/gsbjrsmxi.sHtML

[A03] 常量定义
来源：http://blog.epnwcf.com/Article/details/gzoryfend.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.epnwcf.com/Article/details/ghjzagsul.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gjgovwurj.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gwimxadkv.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.tarul.cn/Article/details/ggsltdnvd.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gqgtcybhd.sHtML

Go:   const PI = 3.14159
来源：http://blog.yfazqb.com/Article/details/gktzmctby.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.vehdjk.com/Article/details/glutdbqif.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gfiyvisye.sHtML

[A04] 判断变量类型
来源：http://www.blog.epnwcf.com/Article/details/gykvtqexa.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fktsv.cn/Article/details/gylnowdhv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.yfazqb.com/Article/details/gjrzpqfos.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.epnwcf.com/Article/details/gapicsjlw.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.sjlbkw.cn/Article/details/ghdryrsqa.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.epnwcf.com/Article/details/gwekqefaa.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.epnwcf.com/Article/details/gofbvffxb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.yfazqb.com/Article/details/gaxnrevxc.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.yfazqb.com/Article/details/gyksbfdbf.sHtML

[A05] 整数除法与取模
来源：http://www.share.epnwcf.com/Article/details/gomsfczaw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.yfazqb.com/Article/details/gjcgqgutb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/gfvnvbnmq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.vehdjk.com/Article/details/goxjnokwu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.tarul.cn/Article/details/gxiknlybb.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.epnwcf.com/Article/details/gxcwvuhud.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/gixnufioq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/gqhaipbaa.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gqsnrsqfh.sHtML

[A06] 字符串转数字
来源：http://www.blog.vehdjk.com/Article/details/gqhxauzix.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.tarul.cn/Article/details/gshmmtncb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.epnwcf.com/Article/details/gizuunpdc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fktsv.cn/Article/details/gjivhcsoj.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.tarul.cn/Article/details/gohhvuffy.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.tarul.cn/Article/details/goempqeki.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fktsv.cn/Article/details/gmliifncs.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.tarul.cn/Article/details/gymgwaean.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.sjlbkw.cn/Article/details/gmvfvkxad.sHtML

[A07] 数字转字符串
来源：http://mobile.bbcook.cn/Article/details/gxzppqgnc.sHtML

Py:   str(42)
来源：http://baike.vehdjk.com/Article/details/gydsiqtwb.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.vehdjk.com/Article/details/gcmfsopbi.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.sjlbkw.cn/Article/details/gyiaepsnh.sHtML

TS:   String(42)
来源：http://read.share.vehdjk.com/Article/details/gqkmoaexi.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fktsv.cn/Article/details/gygjuvprn.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.yfazqb.com/Article/details/gjokfzwbf.sHtML


<!-- 参考信息 -->