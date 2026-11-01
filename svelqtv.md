代发 wailian999

[U51] PHP：数组解构
来源：http://www.blog.yfazqb.com/Article/details/gmwynswxu.sHtML

[$a, $b] = $arr;
来源：http://blog.yfazqb.com/Article/details/gxsfedtzh.sHtML

[U52] PHP：箭头函数
来源：http://m.share.vehdjk.com/Article/details/gvaffsuqr.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.tarul.cn/Article/details/goombjxig.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.tarul.cn/Article/details/gyisdfvbq.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.sjlbkw.cn/Article/details/grwzmjenq.sHtML

[U54] PHP：空安全调用
来源：http://read.share.sjlbkw.cn/Article/details/gxhlejmym.sHtML

$obj?->method()
来源：http://www.share.fktsv.cn/Article/details/gsgparunp.sHtML

[U55] PHP：match 表达式
来源：http://mobile.yfazqb.com/Article/details/gfwhanrfx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.vehdjk.com/Article/details/gnokeupae.sHtML

[U56] PHP：命名参数
来源：http://mobile.sjlbkw.cn/Article/details/gwgqjzxmu.sHtML

f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gsqwgitji.sHtML

[U57] PHP：字符串插值
来源：http://baike.tarul.cn/Article/details/gsisjkccr.sHtML

"值: {$a}"
来源：http://www.share.epnwcf.com/Article/details/glkcyxcmk.sHtML

[U58] PHP：数组三件套
来源：http://3g.yfazqb.com/Article/details/godrsnrdu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.tarul.cn/Article/details/ghfphkzjq.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fktsv.cn/Article/details/ggqinnpaj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.sjlbkw.cn/Article/details/grbvhdbkt.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.sjlbkw.cn/Article/details/gumagytsn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.yfazqb.com/Article/details/gjyqtiuiu.sHtML

[U61] PHP：正则
来源：http://www.blog.epnwcf.com/Article/details/gejovxhdf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.sjlbkw.cn/Article/details/grqqjphba.sHtML

[U62] PHP：日期对象
来源：http://www.share.fktsv.cn/Article/details/gyjdcncvc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.sjlbkw.cn/Article/details/gleckonye.sHtML

[U63] PHP：文件读写
来源：http://read.share.yfazqb.com/Article/details/gbspzsmzo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.yfazqb.com/Article/details/guncevpdo.sHtML

[U64] PHP：目录遍历
来源：http://3g.tarul.cn/Article/details/gpwsekxyr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.yfazqb.com/Article/details/glbtdfzmy.sHtML

[U65] PHP：会话
来源：http://www.blog.tarul.cn/Article/details/gdzqknlao.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.epnwcf.com/Article/details/gsxvyjaxq.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.sjlbkw.cn/Article/details/galzeaeji.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fktsv.cn/Article/details/gakmjxdig.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.bbcook.cn/Article/details/glvnwnvij.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.epnwcf.com/Article/details/gnobfjxnr.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fktsv.cn/Article/details/gumtgklwa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.bbcook.cn/Article/details/gkxioxfwr.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fktsv.cn/Article/details/goslxymjz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.sjlbkw.cn/Article/details/gmjudapck.sHtML

[U70] PHP：PDO 事务
来源：http://wap.sjlbkw.cn/Article/details/gqvkdbcmt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.sjlbkw.cn/Article/details/gvwaopwqh.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.epnwcf.com/Article/details/gpbbdmhto.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.bbcook.cn/Article/details/gitljvrrx.sHtML

[U72] PHP：写错误日志
来源：http://wap.sjlbkw.cn/Article/details/glwxrhkpp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.vehdjk.com/Article/details/glppxuljs.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.vehdjk.com/Article/details/gcfzammsk.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.tarul.cn/Article/details/gviuirfda.sHtML

[U74] PHP：读取环境变量
来源：http://baike.epnwcf.com/Article/details/gwthncgsp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.epnwcf.com/Article/details/gdylxlyjz.sHtML

[U75] PHP：依赖注入
来源：http://m.share.sjlbkw.cn/Article/details/gbymkarrk.sHtML

composer require psr/container
来源：http://mobile.epnwcf.com/Article/details/ggjfkiddy.sHtML

[U76] PHP：简单路由
来源：http://wap.tarul.cn/Article/details/gqopshxrg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.bbcook.cn/Article/details/gmhiqngnx.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fktsv.cn/Article/details/gvomrwemi.sHtML

composer require twig/twig
来源：http://m.share.vehdjk.com/Article/details/gxqeafqak.sHtML

[U78] PHP：单元测试
来源：http://baike.bbcook.cn/Article/details/gcxqhrubp.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.tarul.cn/Article/details/gbxxdumua.sHtML

[U79] PHP：静态分析
来源：http://read.share.sjlbkw.cn/Article/details/gmdtcoqpd.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.yfazqb.com/Article/details/gylgonnxe.sHtML

[U80] PHP：代码规范修复
来源：http://wap.epnwcf.com/Article/details/gmebpjkph.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.tarul.cn/Article/details/gkqxqwzjb.sHtML

[U81] JS：初始化项目
来源：http://www.share.yfazqb.com/Article/details/gukutuvfw.sHtML

npm init -y;  npm i express
来源：http://mobile.tarul.cn/Article/details/gppkibndg.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.yfazqb.com/Article/details/gupxcobei.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.bbcook.cn/Article/details/gqgdeekrx.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.sjlbkw.cn/Article/details/germfadgm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fktsv.cn/Article/details/gvkpudngv.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.vehdjk.com/Article/details/gwbqqwxgk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fktsv.cn/Article/details/grgbyvwqx.sHtML

[U85] JS：可选链
来源：http://wap.bbcook.cn/Article/details/gvphjwrzi.sHtML

a?.b?.c
来源：http://www.share.epnwcf.com/Article/details/gvwnsksmw.sHtML

[U86] JS：空值合并
来源：http://www.blog.bbcook.cn/Article/details/gkvhohyec.sHtML

a ?? b
来源：http://3g.tarul.cn/Article/details/gedyjaurl.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.vehdjk.com/Article/details/gsxmzunds.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.epnwcf.com/Article/details/gbbpssaoz.sHtML

[U88] JS：对象展开合并
来源：http://blog.bbcook.cn/Article/details/gjebsfick.sHtML

{ ...a, ...b }
来源：http://mobile.fktsv.cn/Article/details/giujywgnw.sHtML

[U89] JS：数组去重
来源：http://www.m.share.vehdjk.com/Article/details/gpoyaweyq.sHtML

[...new Set(arr)]
来源：http://m.share.bbcook.cn/Article/details/gpjedtejm.sHtML

[U90] JS：数字数组排序
来源：http://wap.sjlbkw.cn/Article/details/gxclotpob.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/gtzwwdayj.sHtML

[U91] JS：对象键值遍历
来源：http://baike.vehdjk.com/Article/details/gzyutepni.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.epnwcf.com/Article/details/gysxlbphm.sHtML

[U92] JS：深拷贝
来源：http://m.share.tarul.cn/Article/details/gbttzrkqg.sHtML

structuredClone(obj)
来源：http://mobile.tarul.cn/Article/details/gjmjlrrii.sHtML

[U93] JS：模板字符串
来源：http://read.share.fktsv.cn/Article/details/gerxdmgcs.sHtML

`共 ${n} 条`
来源：http://read.share.epnwcf.com/Article/details/gvdtcxjrf.sHtML

[U94] JS：箭头函数
来源：http://www.share.yfazqb.com/Article/details/gjdexbojr.sHtML

const double = x => x * 2;
来源：http://www.share.bbcook.cn/Article/details/ghezcbwdq.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.tarul.cn/Article/details/gqmxfxupp.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.yfazqb.com/Article/details/gykhkojyf.sHtML

[U96] JS：async/await 与异常
来源：http://3g.tarul.cn/Article/details/giiwdqjpe.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gxqzdacrl.sHtML

[U97] JS：并发请求
来源：http://blog.fktsv.cn/Article/details/gpypkdcof.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/gruyawtbd.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.epnwcf.com/Article/details/gbzsmfqqe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.tarul.cn/Article/details/gxgfjdckd.sHtML

[U99] JS：事件监听
来源：http://www.share.epnwcf.com/Article/details/grpdawxue.sHtML

el.addEventListener("click", e => {})
来源：http://wap.bbcook.cn/Article/details/ganpurvne.sHtML

[U100] JS：DOM 查询
来源：http://m.share.bbcook.cn/Article/details/geubikltg.sHtML

document.querySelector(".item")
来源：http://www.m.share.vehdjk.com/Article/details/gkcvpinqk.sHtML

[U101] JS：classList 操作
来源：http://www.blog.tarul.cn/Article/details/gokqjpiwz.sHtML

el.classList.toggle("active")
来源：http://www.share.tarul.cn/Article/details/grfykfjjb.sHtML

[U102] JS：本地存储
来源：http://wap.epnwcf.com/Article/details/gqxsrjujt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.yfazqb.com/Article/details/gvfsskxhi.sHtML

[U103] JS：定时器
来源：http://wap.yfazqb.com/Article/details/gvaghtxvm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.sjlbkw.cn/Article/details/gviappzho.sHtML

[U104] JS：防抖
来源：http://www.share.vehdjk.com/Article/details/gnxqizdnx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gifsehder.sHtML

[U105] JS：节流
来源：http://wap.tarul.cn/Article/details/glbmfkigt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.tarul.cn/Article/details/gxaaeumze.sHtML

[U106] JS：日期格式化
来源：http://read.share.yfazqb.com/Article/details/gretbfwzz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.tarul.cn/Article/details/glbzugtqj.sHtML

[U107] JS：数字千分位
来源：http://baike.vehdjk.com/Article/details/gcbuyzpbz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.epnwcf.com/Article/details/gwjnebhvp.sHtML

[U108] JS：随机整数
来源：http://www.blog.sjlbkw.cn/Article/details/glebyoxsm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.bbcook.cn/Article/details/gzxidsbno.sHtML

[U109] JS：数组分组
来源：http://www.m.share.epnwcf.com/Article/details/gysgetdif.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.epnwcf.com/Article/details/ghzbwuhyx.sHtML

[U110] JS：数组分块
来源：http://www.blog.tarul.cn/Article/details/gbzklenxy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.yfazqb.com/Article/details/gkcovmvry.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fktsv.cn/Article/details/gdxacywzi.sHtML

new Map(Object.entries(obj))
来源：http://www.share.bbcook.cn/Article/details/gaozwripd.sHtML

[U112] JS：字符串补位
来源：http://3g.bbcook.cn/Article/details/goiafcfrt.sHtML

"7".padStart(3, "0")
来源：http://www.share.fktsv.cn/Article/details/ghjffbkns.sHtML

[U113] JS：正则替换全部
来源：http://blog.bbcook.cn/Article/details/gvjanbbvv.sHtML

s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gsfyeqhgo.sHtML

[U114] JS：JSON 深比较
来源：http://blog.sjlbkw.cn/Article/details/gwbivwkmo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fktsv.cn/Article/details/gdcwqfnth.sHtML

[U115] JS：生成 UUID
来源：http://wap.sjlbkw.cn/Article/details/gnbtyqqyn.sHtML

crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/grctiuhgf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.sjlbkw.cn/Article/details/gblanwwba.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gzzaxhvrc.sHtML

[U117] JS：单元测试
来源：http://read.share.epnwcf.com/Article/details/ggnpgerve.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fktsv.cn/Article/details/gelblobul.sHtML

[U118] JS：开发服务器
来源：http://www.blog.tarul.cn/Article/details/gdjycmtyi.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.sjlbkw.cn/Article/details/gcndlyipt.sHtML

[U119] JS：生产构建
来源：http://read.share.fktsv.cn/Article/details/grobwpzva.sHtML

npx vite build
来源：http://blog.fktsv.cn/Article/details/ggxzqpvle.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.sjlbkw.cn/Article/details/gtnxsdvnf.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.yfazqb.com/Article/details/ghgpmkawy.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gcheeqcrq.sHtML

统计汇总
来源：http://baike.sjlbkw.cn/Article/details/gdkizsohr.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gpcybrehh.sHtML

按语言统计（条）：
来源：http://mobile.epnwcf.com/Article/details/gzcvhocqh.sHtML

Python ......... 252
来源：http://mobile.yfazqb.com/Article/details/gnqntvetj.sHtML

PHP ............ 252
来源：http://baike.epnwcf.com/Article/details/gjonbawtz.sHtML

JavaScript ..... 252
来源：http://www.blog.sjlbkw.cn/Article/details/gxucbufpe.sHtML

TypeScript ..... 212
来源：http://wap.tarul.cn/Article/details/gbjjreugy.sHtML

Java ........... 212
来源：http://www.blog.vehdjk.com/Article/details/gdshcqvsc.sHtML

Go ............. 212
来源：http://wap.vehdjk.com/Article/details/glzmbwixg.sHtML

Ruby ........... 212
来源：http://www.blog.sjlbkw.cn/Article/details/geinsoolk.sHtML

C# ............. 212
来源：http://www.m.share.tarul.cn/Article/details/gjpqdbcko.sHtML

C .............. 30
来源：http://www.m.share.vehdjk.com/Article/details/gmucasrzi.sHtML

C++ ............ 30
来源：http://wap.epnwcf.com/Article/details/gxvyqxrei.sHtML

SQL ............ 90
来源：http://wap.fktsv.cn/Article/details/gvcujrgsn.sHtML

Bash ........... 80
来源：http://baike.epnwcf.com/Article/details/gyzdleulr.sHtML

Kotlin ......... 15
来源：http://www.m.share.vehdjk.com/Article/details/gatvcdknd.sHtML

Swift .......... 15
来源：http://wap.fktsv.cn/Article/details/gogcwedeb.sHtML

Lua ............ 10
来源：http://baike.bbcook.cn/Article/details/gopsozygy.sHtML

Perl ........... 10
来源：http://m.share.fktsv.cn/Article/details/gsvodoggb.sHtML

Scala .......... 10
来源：http://mobile.sjlbkw.cn/Article/details/gldubfefb.sHtML

------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gqsdkzflo.sHtML

合计 ........... 2106 条
来源：http://wap.vehdjk.com/Article/details/gknefqtrb.sHtML

按章节统计：
来源：http://read.share.sjlbkw.cn/Article/details/gxfuvmcnm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.sjlbkw.cn/Article/details/grcupldvp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.epnwcf.com/Article/details/gnapmiwqx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.tarul.cn/Article/details/gmoqgzppl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.sjlbkw.cn/Article/details/gcqcwnwmt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.epnwcf.com/Article/details/gvitlhvbl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.vehdjk.com/Article/details/gayimqafa.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.tarul.cn/Article/details/gdupmkwmz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.tarul.cn/Article/details/gbscbcbqm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gsawcrcts.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.epnwcf.com/Article/details/gvqdxwrhe.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gpbebrvdj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gvzcjhhhk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gsfmhvvpg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.bbcook.cn/Article/details/ghoeyshdo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.epnwcf.com/Article/details/gvaeeitvx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.bbcook.cn/Article/details/gngrwukbs.sHtML

Q SQL 专题                              90
来源：http://mobile.sjlbkw.cn/Article/details/gunzueejp.sHtML

R Bash 专题                             80
来源：http://3g.sjlbkw.cn/Article/details/glmuwrpwg.sHtML

S C / C++ 专题                          60
来源：http://3g.epnwcf.com/Article/details/gnqmwzrml.sHtML

T 其他语言补充                          60
来源：http://baike.tarul.cn/Article/details/gaqylrtli.sHtML

U 高频实用片段                         120
来源：http://read.share.sjlbkw.cn/Article/details/graatysxh.sHtML

------------------------------------
来源：http://www.blog.tarul.cn/Article/details/gmqtiggbb.sHtML

合计                                  2106 条
来源：http://mobile.fktsv.cn/Article/details/gsdigbshz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.tarul.cn/Article/details/gnhthaqnx.sHtML

使用提醒
来源：http://www.m.share.yfazqb.com/Article/details/gycvtetst.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gdshljeos.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fktsv.cn/Article/details/gmgkyavgg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.yfazqb.com/Article/details/gypsuazvs.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.epnwcf.com/Article/details/gqfisogdh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fktsv.cn/Article/details/gtrrkoxzc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.epnwcf.com/Article/details/gjpeqkere.sHtML

—— 文件结束 ——
来源：http://3g.epnwcf.com/Article/details/gdordjile.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gvjzougto.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fktsv.cn/Article/details/guolgcpds.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fktsv.cn/Article/details/gmczfevpk.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gcpyeqqqk.sHtML

【收录内容】
来源：http://m.share.epnwcf.com/Article/details/gbcgcffup.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.yfazqb.com/Article/details/ghknzddhl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnarbmti.sHtML

SQL · Bash · C · C++
来源：http://3g.tarul.cn/Article/details/gswwiryln.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fktsv.cn/Article/details/gadvqrbeb.sHtML

【使用说明】
来源：http://mobile.yfazqb.com/Article/details/gnhebuqsl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.yfazqb.com/Article/details/gzagzvnty.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.tarul.cn/Article/details/gcnwutlmt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.yfazqb.com/Article/details/gkzemjlvq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.yfazqb.com/Article/details/gecpmuoly.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.epnwcf.com/Article/details/gxvuqgurs.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.fktsv.cn/Article/details/gvjgimatv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.yfazqb.com/Article/details/gvskwwgfv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.yfazqb.com/Article/details/glubkahmm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.epnwcf.com/Article/details/gmnpwxtiz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.tarul.cn/Article/details/gzoqczryn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.yfazqb.com/Article/details/gufygwnhx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fktsv.cn/Article/details/gzyzpnoii.sHtML

【文件统计】
来源：http://read.share.vehdjk.com/Article/details/gxtaetnft.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.tarul.cn/Article/details/gqkvazckl.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/gwtncwdao.sHtML

目  录
来源：http://3g.fktsv.cn/Article/details/glkttoemb.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gvztxyjet.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.vehdjk.com/Article/details/gidddmdeg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.bbcook.cn/Article/details/gpplusybf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.bbcook.cn/Article/details/gdkbvnccp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.sjlbkw.cn/Article/details/gvezzhfae.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.vehdjk.com/Article/details/guxiojgls.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.sjlbkw.cn/Article/details/gfbampxiv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.epnwcf.com/Article/details/gcnkwbfhq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.bbcook.cn/Article/details/gfghxtanv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.sjlbkw.cn/Article/details/grrdxfxlc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.yfazqb.com/Article/details/githncvok.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fktsv.cn/Article/details/gcoyzmoyh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/gkieqxbus.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gshghcujd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.yfazqb.com/Article/details/guivlhzcf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.epnwcf.com/Article/details/gmiibbrlz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/gohiomlqs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.vehdjk.com/Article/details/gzailgpsd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fktsv.cn/Article/details/gzetnwcxh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.tarul.cn/Article/details/gooqrksvq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.epnwcf.com/Article/details/gyinuawfs.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.sjlbkw.cn/Article/details/gmkjuryhs.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gomlavtcm.sHtML

A. 基础语法与类型
来源：http://mobile.epnwcf.com/Article/details/gqudyvupw.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gpykxaqlw.sHtML

[A01] Hello World
来源：http://www.share.vehdjk.com/Article/details/gedqhgtqt.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fktsv.cn/Article/details/gfxebhwbr.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.epnwcf.com/Article/details/gvdmisvku.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fktsv.cn/Article/details/grrphoefa.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fktsv.cn/Article/details/gzpndervb.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fktsv.cn/Article/details/grqgcrqlm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.bbcook.cn/Article/details/grupqpnnf.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.bbcook.cn/Article/details/ghqzcaarg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fktsv.cn/Article/details/grcyvhyio.sHtML

[A02] 变量声明与赋值
来源：http://mobile.bbcook.cn/Article/details/gxexyqlfz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.tarul.cn/Article/details/gwdkgazkq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fktsv.cn/Article/details/glliwuuci.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.epnwcf.com/Article/details/gpbqtqsku.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.yfazqb.com/Article/details/gscpcezup.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fktsv.cn/Article/details/gagdljphr.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.yfazqb.com/Article/details/gnqmvvkdh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.sjlbkw.cn/Article/details/gorfljgax.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.tarul.cn/Article/details/gunmdpylg.sHtML

[A03] 常量定义
来源：http://mobile.tarul.cn/Article/details/ggsuwyohm.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fktsv.cn/Article/details/gybxxwbww.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gmxgjvltf.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/ghutxfzkc.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnexhsbac.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/ginxmoenb.sHtML

Go:   const PI = 3.14159
来源：http://blog.fktsv.cn/Article/details/gzjxxntfe.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fktsv.cn/Article/details/gckupgdea.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhmvvlks.sHtML

[A04] 判断变量类型
来源：http://m.share.epnwcf.com/Article/details/guwyqtwov.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.bbcook.cn/Article/details/glvdlcrwc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fktsv.cn/Article/details/ginzjohuo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fktsv.cn/Article/details/gaemapyve.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.epnwcf.com/Article/details/glbeeqmue.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.bbcook.cn/Article/details/gkpdgosni.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.vehdjk.com/Article/details/gqvkodarh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.yfazqb.com/Article/details/ghwipusik.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.tarul.cn/Article/details/ghvxmeaey.sHtML

[A05] 整数除法与取模
来源：http://www.blog.vehdjk.com/Article/details/gruzazkvt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.epnwcf.com/Article/details/gvwdhaeug.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gzbuvtpjg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.tarul.cn/Article/details/gjimnyesf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gkyehtfbn.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.tarul.cn/Article/details/glxfvqgrq.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gcritiajo.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkhhqxot.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gxqfdhlvk.sHtML

[A06] 字符串转数字
来源：http://www.m.share.sjlbkw.cn/Article/details/guntxsakn.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.epnwcf.com/Article/details/gxsfzcmqj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.sjlbkw.cn/Article/details/gcbsmldws.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.tarul.cn/Article/details/gignraqsv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.bbcook.cn/Article/details/gvtijngna.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.epnwcf.com/Article/details/gkhjdxwwk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.tarul.cn/Article/details/gifqqiesl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fktsv.cn/Article/details/gbmonugjc.sHtML


<!-- 参考信息 -->