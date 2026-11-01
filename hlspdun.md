代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://baike.vehdjk.com/Article/details/ghxjffhez.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/ggkjznaie.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.bbcook.cn/Article/details/gvcvlgwqx.sHtML

?string $name = null
来源：http://www.blog.vehdjk.com/Article/details/gstdgeoot.sHtML

[U47] PHP：联合类型
来源：http://mobile.sjlbkw.cn/Article/details/gwxubemrv.sHtML

int|string $id
来源：http://read.share.yfazqb.com/Article/details/gbpbwdevy.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fktsv.cn/Article/details/gsyuxesvz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.yfazqb.com/Article/details/gqhmijayh.sHtML

[U49] PHP：只读属性
来源：http://wap.fktsv.cn/Article/details/gwsbxuyrz.sHtML

public readonly string $name
来源：http://wap.epnwcf.com/Article/details/gemcfsunt.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.yfazqb.com/Article/details/gnywqelyo.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.bbcook.cn/Article/details/gjvftjvsf.sHtML

[U51] PHP：数组解构
来源：http://blog.fktsv.cn/Article/details/gllajgodz.sHtML

[$a, $b] = $arr;
来源：http://www.blog.vehdjk.com/Article/details/gfudceika.sHtML

[U52] PHP：箭头函数
来源：http://www.share.epnwcf.com/Article/details/gyldevnil.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fktsv.cn/Article/details/gfyowozed.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.epnwcf.com/Article/details/ghdbdxzcg.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.yfazqb.com/Article/details/ggcphtmdk.sHtML

[U54] PHP：空安全调用
来源：http://m.share.epnwcf.com/Article/details/grjqmfjzg.sHtML

$obj?->method()
来源：http://3g.tarul.cn/Article/details/gtogydhcl.sHtML

[U55] PHP：match 表达式
来源：http://m.share.tarul.cn/Article/details/gtcwutqfd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.tarul.cn/Article/details/grxkqceri.sHtML

[U56] PHP：命名参数
来源：http://baike.fktsv.cn/Article/details/gsselkcpp.sHtML

f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/gjnoakafq.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/grqeyasly.sHtML

"值: {$a}"
来源：http://wap.tarul.cn/Article/details/gcbrmostx.sHtML

[U58] PHP：数组三件套
来源：http://3g.fktsv.cn/Article/details/gxwxxjabd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fktsv.cn/Article/details/gqwbndetl.sHtML

[U59] PHP：自定义排序
来源：http://blog.bbcook.cn/Article/details/gmrmjkrtc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.bbcook.cn/Article/details/gpuhhiwux.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.sjlbkw.cn/Article/details/gedboaqhy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.epnwcf.com/Article/details/gjqssnyvt.sHtML

[U61] PHP：正则
来源：http://read.share.bbcook.cn/Article/details/grwakxkyx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.tarul.cn/Article/details/gbiveqdew.sHtML

[U62] PHP：日期对象
来源：http://www.blog.sjlbkw.cn/Article/details/gwvswqbxa.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.vehdjk.com/Article/details/gkcftmsus.sHtML

[U63] PHP：文件读写
来源：http://m.share.tarul.cn/Article/details/gbjxfxkwo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwjuwxnn.sHtML

[U64] PHP：目录遍历
来源：http://mobile.vehdjk.com/Article/details/gczrcgumg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.sjlbkw.cn/Article/details/gqkmdztcx.sHtML

[U65] PHP：会话
来源：http://baike.yfazqb.com/Article/details/gvqdrffus.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/ggxssvssx.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.vehdjk.com/Article/details/guzfkcsjc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.vehdjk.com/Article/details/gjnzlowyz.sHtML

[U67] PHP：处理文件上传
来源：http://3g.epnwcf.com/Article/details/gegwdevhd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.yfazqb.com/Article/details/gdmmitjyr.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fktsv.cn/Article/details/gepgbbext.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.epnwcf.com/Article/details/gmmlycaza.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.sjlbkw.cn/Article/details/gisqjxkjm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.bbcook.cn/Article/details/glfwxhccq.sHtML

[U70] PHP：PDO 事务
来源：http://blog.bbcook.cn/Article/details/grweiowes.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.yfazqb.com/Article/details/gtftilyud.sHtML

[U71] PHP：抛出异常
来源：http://www.share.bbcook.cn/Article/details/gbfxfllsk.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.sjlbkw.cn/Article/details/gjlvkjgmu.sHtML

[U72] PHP：写错误日志
来源：http://baike.sjlbkw.cn/Article/details/gqrdnybgi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.yfazqb.com/Article/details/greuchklq.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.sjlbkw.cn/Article/details/ghricztna.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.bbcook.cn/Article/details/gxfrrqbzv.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gsfkiyizi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.bbcook.cn/Article/details/gwqxlompk.sHtML

[U75] PHP：依赖注入
来源：http://m.share.sjlbkw.cn/Article/details/gijyjtaqg.sHtML

composer require psr/container
来源：http://www.blog.fktsv.cn/Article/details/ghjptmwtq.sHtML

[U76] PHP：简单路由
来源：http://wap.vehdjk.com/Article/details/ggtrzckdv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.yfazqb.com/Article/details/gihodijkt.sHtML

[U77] PHP：模板渲染
来源：http://blog.tarul.cn/Article/details/gkscfflub.sHtML

composer require twig/twig
来源：http://baike.yfazqb.com/Article/details/gqpyjbpmk.sHtML

[U78] PHP：单元测试
来源：http://mobile.tarul.cn/Article/details/godwmykpu.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.epnwcf.com/Article/details/guqrpcxel.sHtML

[U79] PHP：静态分析
来源：http://www.blog.vehdjk.com/Article/details/gxesrcdum.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.yfazqb.com/Article/details/gfogpvmme.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.tarul.cn/Article/details/gygjdztgs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.bbcook.cn/Article/details/gtdwvquck.sHtML

[U81] JS：初始化项目
来源：http://read.share.yfazqb.com/Article/details/gxeaoeucv.sHtML

npm init -y;  npm i express
来源：http://3g.vehdjk.com/Article/details/gxrvzwhyz.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.bbcook.cn/Article/details/gwdarixid.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.vehdjk.com/Article/details/gldxarkrl.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.sjlbkw.cn/Article/details/gyvpuiffu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.vehdjk.com/Article/details/ggkabridz.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.bbcook.cn/Article/details/gujbszmxe.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.yfazqb.com/Article/details/gwgdxvllz.sHtML

[U85] JS：可选链
来源：http://www.m.share.vehdjk.com/Article/details/gfcvmumfs.sHtML

a?.b?.c
来源：http://www.m.share.bbcook.cn/Article/details/gkcxhjypv.sHtML

[U86] JS：空值合并
来源：http://www.m.share.sjlbkw.cn/Article/details/gqltudqzz.sHtML

a ?? b
来源：http://read.share.vehdjk.com/Article/details/gcltinevc.sHtML

[U87] JS：解构默认值
来源：http://wap.bbcook.cn/Article/details/guyrljroh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.bbcook.cn/Article/details/guwxjqayk.sHtML

[U88] JS：对象展开合并
来源：http://www.share.vehdjk.com/Article/details/gsnnuhpcr.sHtML

{ ...a, ...b }
来源：http://read.share.sjlbkw.cn/Article/details/gjhbnqinn.sHtML

[U89] JS：数组去重
来源：http://www.share.yfazqb.com/Article/details/gpqfzjhcg.sHtML

[...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gupwjmpdd.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.tarul.cn/Article/details/ghqekopaw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/gbzymxwyp.sHtML

[U91] JS：对象键值遍历
来源：http://3g.sjlbkw.cn/Article/details/gildxytyu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fktsv.cn/Article/details/gqvlzytia.sHtML

[U92] JS：深拷贝
来源：http://wap.vehdjk.com/Article/details/gynwrccyn.sHtML

structuredClone(obj)
来源：http://blog.vehdjk.com/Article/details/gcutakmgr.sHtML

[U93] JS：模板字符串
来源：http://baike.tarul.cn/Article/details/grxjheixb.sHtML

`共 ${n} 条`
来源：http://wap.vehdjk.com/Article/details/glxwuwwne.sHtML

[U94] JS：箭头函数
来源：http://www.share.yfazqb.com/Article/details/ghnqskgwe.sHtML

const double = x => x * 2;
来源：http://www.share.epnwcf.com/Article/details/gmkwmxwnt.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.sjlbkw.cn/Article/details/gasgwyhpv.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.vehdjk.com/Article/details/gnmyhostj.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fktsv.cn/Article/details/gtmeeobus.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gffkeecem.sHtML

[U97] JS：并发请求
来源：http://mobile.bbcook.cn/Article/details/gckjllzre.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gerlqbbsd.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.sjlbkw.cn/Article/details/guezvbtvw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.yfazqb.com/Article/details/gooplicfb.sHtML

[U99] JS：事件监听
来源：http://baike.sjlbkw.cn/Article/details/gjirqaewk.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.bbcook.cn/Article/details/gwitjmftb.sHtML

[U100] JS：DOM 查询
来源：http://blog.yfazqb.com/Article/details/gjbnqgfqn.sHtML

document.querySelector(".item")
来源：http://3g.bbcook.cn/Article/details/gpbmpmbxe.sHtML

[U101] JS：classList 操作
来源：http://mobile.fktsv.cn/Article/details/glnglwexh.sHtML

el.classList.toggle("active")
来源：http://www.m.share.epnwcf.com/Article/details/gvkgqmezd.sHtML

[U102] JS：本地存储
来源：http://blog.vehdjk.com/Article/details/gyehchcrg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.epnwcf.com/Article/details/gxnqcxuvn.sHtML

[U103] JS：定时器
来源：http://read.share.fktsv.cn/Article/details/gcyglzzwa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.tarul.cn/Article/details/gryupyhuf.sHtML

[U104] JS：防抖
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdtyoerm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gwrmeudaj.sHtML

[U105] JS：节流
来源：http://www.blog.vehdjk.com/Article/details/gjdxzmbkk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.tarul.cn/Article/details/grjtedeza.sHtML

[U106] JS：日期格式化
来源：http://mobile.vehdjk.com/Article/details/gptycykbw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.bbcook.cn/Article/details/gcilwswti.sHtML

[U107] JS：数字千分位
来源：http://wap.tarul.cn/Article/details/guieshnor.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.vehdjk.com/Article/details/gurclusqi.sHtML

[U108] JS：随机整数
来源：http://wap.vehdjk.com/Article/details/gyzjnangs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.bbcook.cn/Article/details/gzbbchuce.sHtML

[U109] JS：数组分组
来源：http://www.share.epnwcf.com/Article/details/gbojoydnc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.tarul.cn/Article/details/gsoaecznd.sHtML

[U110] JS：数组分块
来源：http://blog.yfazqb.com/Article/details/gsyqoclcc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.vehdjk.com/Article/details/gyxracatk.sHtML

[U111] JS：对象转 Map
来源：http://wap.fktsv.cn/Article/details/gnbhbpjjg.sHtML

new Map(Object.entries(obj))
来源：http://read.share.yfazqb.com/Article/details/glcowtsln.sHtML

[U112] JS：字符串补位
来源：http://3g.vehdjk.com/Article/details/gaasaoxlx.sHtML

"7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gigsmteke.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.bbcook.cn/Article/details/ghntkceum.sHtML

s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gpfikgefa.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.vehdjk.com/Article/details/gbklxynre.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fktsv.cn/Article/details/gjokqxrmg.sHtML

[U115] JS：生成 UUID
来源：http://baike.tarul.cn/Article/details/gdxwieeij.sHtML

crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/gxtvuyryk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.bbcook.cn/Article/details/gpzzfcmkj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.yfazqb.com/Article/details/gygnrdvpk.sHtML

[U117] JS：单元测试
来源：http://wap.fktsv.cn/Article/details/gkctbnfvu.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.sjlbkw.cn/Article/details/guflzbrwt.sHtML

[U118] JS：开发服务器
来源：http://m.share.vehdjk.com/Article/details/gngyryyvr.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fktsv.cn/Article/details/gdgoieezt.sHtML

[U119] JS：生产构建
来源：http://mobile.sjlbkw.cn/Article/details/gpwjsrgnn.sHtML

npx vite build
来源：http://baike.yfazqb.com/Article/details/gmntosxan.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.vehdjk.com/Article/details/glyqjukvk.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.bbcook.cn/Article/details/gvoagkqem.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gorcqncfu.sHtML

统计汇总
来源：http://mobile.epnwcf.com/Article/details/gvaefgrib.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gjrvsksji.sHtML

按语言统计（条）：
来源：http://m.share.yfazqb.com/Article/details/gxmpxydcb.sHtML

Python ......... 252
来源：http://www.m.share.yfazqb.com/Article/details/gnucunhgm.sHtML

PHP ............ 252
来源：http://baike.vehdjk.com/Article/details/gtwafvwpo.sHtML

JavaScript ..... 252
来源：http://www.m.share.fktsv.cn/Article/details/gyicdfwzp.sHtML

TypeScript ..... 212
来源：http://m.share.sjlbkw.cn/Article/details/grqhqqlpx.sHtML

Java ........... 212
来源：http://baike.sjlbkw.cn/Article/details/gxabxynyn.sHtML

Go ............. 212
来源：http://read.share.fktsv.cn/Article/details/gxgekibbu.sHtML

Ruby ........... 212
来源：http://www.blog.bbcook.cn/Article/details/gtdairxje.sHtML

C# ............. 212
来源：http://wap.epnwcf.com/Article/details/gwinhypxc.sHtML

C .............. 30
来源：http://read.share.tarul.cn/Article/details/gbiararkv.sHtML

C++ ............ 30
来源：http://mobile.epnwcf.com/Article/details/gmoijkroo.sHtML

SQL ............ 90
来源：http://read.share.tarul.cn/Article/details/gkzitaoth.sHtML

Bash ........... 80
来源：http://3g.yfazqb.com/Article/details/gfobqvzvk.sHtML

Kotlin ......... 15
来源：http://mobile.tarul.cn/Article/details/gwjszmowf.sHtML

Swift .......... 15
来源：http://www.m.share.yfazqb.com/Article/details/goyfkavza.sHtML

Lua ............ 10
来源：http://www.m.share.tarul.cn/Article/details/gxjnandjd.sHtML

Perl ........... 10
来源：http://www.blog.epnwcf.com/Article/details/gavxzhcja.sHtML

Scala .......... 10
来源：http://3g.bbcook.cn/Article/details/gerzkuzfg.sHtML

------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/ghtxxrsau.sHtML

合计 ........... 2106 条
来源：http://blog.fktsv.cn/Article/details/gynqgjyjz.sHtML

按章节统计：
来源：http://www.blog.vehdjk.com/Article/details/gsufbhixo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.tarul.cn/Article/details/gjwxdxstj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.tarul.cn/Article/details/gezbnceqq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.tarul.cn/Article/details/gwtpiegyg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.tarul.cn/Article/details/gyvnmcciz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.vehdjk.com/Article/details/gwfqtmbib.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.epnwcf.com/Article/details/gqtzuhedn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/galnvgnuo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.tarul.cn/Article/details/gikmgqwdo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/gptpgunzi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.vehdjk.com/Article/details/glendthig.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gsvzbxupc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.sjlbkw.cn/Article/details/gubairnsp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/gxyfaggcj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.tarul.cn/Article/details/gbwhqpovr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.yfazqb.com/Article/details/gkuicaxpj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/geksxabia.sHtML

Q SQL 专题                              90
来源：http://baike.epnwcf.com/Article/details/gdulittnv.sHtML

R Bash 专题                             80
来源：http://www.share.fktsv.cn/Article/details/gyetrjblf.sHtML

S C / C++ 专题                          60
来源：http://mobile.sjlbkw.cn/Article/details/gsxtkvuke.sHtML

T 其他语言补充                          60
来源：http://read.share.sjlbkw.cn/Article/details/gntjhzact.sHtML

U 高频实用片段                         120
来源：http://wap.fktsv.cn/Article/details/gzqxsaizi.sHtML

------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gnixbbcpo.sHtML

合计                                  2106 条
来源：http://blog.yfazqb.com/Article/details/gohwfkuvh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.epnwcf.com/Article/details/gealtbjyu.sHtML

使用提醒
来源：http://m.share.tarul.cn/Article/details/gnmptybbt.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/gwekxumpo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.bbcook.cn/Article/details/ghwceypxi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.yfazqb.com/Article/details/grobvspzd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.bbcook.cn/Article/details/gjyvzkrrb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fktsv.cn/Article/details/guzajwxyw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.yfazqb.com/Article/details/gxnbzlcwu.sHtML

—— 文件结束 ——
来源：http://wap.epnwcf.com/Article/details/gpxtvcofv.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gammcamnu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fktsv.cn/Article/details/gwrgppote.sHtML

Common Programming Examples Cheat Book
来源：http://baike.tarul.cn/Article/details/gpajxneov.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gjumnhhxz.sHtML

【收录内容】
来源：http://read.share.bbcook.cn/Article/details/gfxsyqlev.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.bbcook.cn/Article/details/gzaalgnua.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.sjlbkw.cn/Article/details/gkunwaarr.sHtML

SQL · Bash · C · C++
来源：http://wap.vehdjk.com/Article/details/glfkchugs.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.tarul.cn/Article/details/gnwvkmxzg.sHtML

【使用说明】
来源：http://m.share.vehdjk.com/Article/details/gwcixgvtf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.bbcook.cn/Article/details/ggdvwjoyx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.yfazqb.com/Article/details/ggmgzwgpv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.epnwcf.com/Article/details/gdiwlwpdm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.yfazqb.com/Article/details/gpwzodpps.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.tarul.cn/Article/details/gmnwjjodd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.sjlbkw.cn/Article/details/gptcamaqf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.bbcook.cn/Article/details/gfaegnoln.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.bbcook.cn/Article/details/ggvvmgfer.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.epnwcf.com/Article/details/gxuzntmic.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.sjlbkw.cn/Article/details/geudodaoh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.yfazqb.com/Article/details/goacrynio.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.bbcook.cn/Article/details/gnyosgdgi.sHtML

【文件统计】
来源：http://mobile.tarul.cn/Article/details/gwheapgdl.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.epnwcf.com/Article/details/gjscbwvoj.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gsuzamcwk.sHtML

目  录
来源：http://www.m.share.vehdjk.com/Article/details/gtawckiyz.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/grmmryajg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.bbcook.cn/Article/details/gpsoztkhu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/gfbohasxj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.vehdjk.com/Article/details/gbylxrxec.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.bbcook.cn/Article/details/gacvfrfmo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.vehdjk.com/Article/details/gpbykuvog.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.tarul.cn/Article/details/ghqekxarx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fktsv.cn/Article/details/gyixfkgdg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.bbcook.cn/Article/details/gigoykloj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gqxrshedp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.sjlbkw.cn/Article/details/gyrszntpd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.bbcook.cn/Article/details/ghuwufqmq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/gnhlmxbnw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gikqdttfo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fktsv.cn/Article/details/grussxiku.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.bbcook.cn/Article/details/gkpnbhpda.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.sjlbkw.cn/Article/details/gapmtrffa.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.vehdjk.com/Article/details/gxjbprgxd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjxorhvq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.tarul.cn/Article/details/ghvqyolbi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.tarul.cn/Article/details/gevsxjqvm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.bbcook.cn/Article/details/gjfgrgpus.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gultoifmf.sHtML

A. 基础语法与类型
来源：http://baike.vehdjk.com/Article/details/ggedmfqui.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gjrscqvkq.sHtML

[A01] Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gomtvwznm.sHtML

Py:   print("Hello, World!")
来源：http://www.share.bbcook.cn/Article/details/gpbsajiva.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fktsv.cn/Article/details/gslmtcudv.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.sjlbkw.cn/Article/details/gyqcoinhu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.vehdjk.com/Article/details/gnalwhyka.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.sjlbkw.cn/Article/details/gvazchhvo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.tarul.cn/Article/details/giqtdfbmn.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.vehdjk.com/Article/details/gzhbiheqm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.tarul.cn/Article/details/ghwnkulut.sHtML

[A02] 变量声明与赋值
来源：http://read.share.yfazqb.com/Article/details/gvwsyeufr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.yfazqb.com/Article/details/gxrjclyjj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.yfazqb.com/Article/details/guqnykkra.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.vehdjk.com/Article/details/gbgoafpym.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.yfazqb.com/Article/details/grtgzortw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.sjlbkw.cn/Article/details/gzluxzmdw.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.bbcook.cn/Article/details/gkanroeci.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.vehdjk.com/Article/details/ggpaveylw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fktsv.cn/Article/details/gkemjictn.sHtML

[A03] 常量定义
来源：http://read.share.bbcook.cn/Article/details/gpqgfxewn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.epnwcf.com/Article/details/gkjplydeo.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gnwcewyld.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/glhlktwac.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gmvhyyyht.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gmuowwdnu.sHtML

Go:   const PI = 3.14159
来源：http://3g.bbcook.cn/Article/details/guzvavrzy.sHtML

Ruby: PI = 3.14159
来源：http://3g.bbcook.cn/Article/details/gxylmhivh.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gljybsjsr.sHtML

[A04] 判断变量类型
来源：http://baike.tarul.cn/Article/details/gzpzwqkpr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.epnwcf.com/Article/details/gngyojmqq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.sjlbkw.cn/Article/details/gusftbzgg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.epnwcf.com/Article/details/gportzqbt.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.epnwcf.com/Article/details/gqkmtjcsw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fktsv.cn/Article/details/grrikhthy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.sjlbkw.cn/Article/details/gknmxjrpo.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.vehdjk.com/Article/details/gnyrgtrym.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.yfazqb.com/Article/details/gdinfvnac.sHtML

[A05] 整数除法与取模
来源：http://3g.fktsv.cn/Article/details/gmmgnedii.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.bbcook.cn/Article/details/gtsxjsadc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fktsv.cn/Article/details/gtpfvuors.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.yfazqb.com/Article/details/gsawgtdeb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gfogjydrl.sHtML


<!-- 参考信息 -->