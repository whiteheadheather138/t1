代发 wailian999

[U49] PHP：只读属性
来源：http://baike.bbcook.cn/Article/details/gwwzmonxz.sHtML

public readonly string $name
来源：http://read.share.fktsv.cn/Article/details/gkisxhbwm.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.yfazqb.com/Article/details/gcjxstjdj.sHtML

public function __construct(private int $id) {}
来源：http://baike.tarul.cn/Article/details/gludfpkwk.sHtML

[U51] PHP：数组解构
来源：http://baike.bbcook.cn/Article/details/gvngztqpv.sHtML

[$a, $b] = $arr;
来源：http://3g.sjlbkw.cn/Article/details/gjpajshjk.sHtML

[U52] PHP：箭头函数
来源：http://wap.yfazqb.com/Article/details/gbitpdldi.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fktsv.cn/Article/details/gqvptkcdv.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.yfazqb.com/Article/details/ggrvckfcu.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.bbcook.cn/Article/details/gtnkroigj.sHtML

[U54] PHP：空安全调用
来源：http://read.share.epnwcf.com/Article/details/gfwkbrhfx.sHtML

$obj?->method()
来源：http://www.blog.sjlbkw.cn/Article/details/grbgklutf.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fktsv.cn/Article/details/gzqtcqzro.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fktsv.cn/Article/details/goetcracw.sHtML

[U56] PHP：命名参数
来源：http://read.share.tarul.cn/Article/details/gbwwvgyci.sHtML

f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/gjhpqrrmi.sHtML

[U57] PHP：字符串插值
来源：http://blog.epnwcf.com/Article/details/gbikshzvk.sHtML

"值: {$a}"
来源：http://www.m.share.fktsv.cn/Article/details/gkgavaevj.sHtML

[U58] PHP：数组三件套
来源：http://3g.vehdjk.com/Article/details/gfxmxmidy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.epnwcf.com/Article/details/gplgqqfrw.sHtML

[U59] PHP：自定义排序
来源：http://baike.bbcook.cn/Article/details/gssvdibey.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.sjlbkw.cn/Article/details/gpzyalyuz.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.epnwcf.com/Article/details/ghxzfzgvv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fktsv.cn/Article/details/gcmoqznpr.sHtML

[U61] PHP：正则
来源：http://www.m.share.tarul.cn/Article/details/geiabznao.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.tarul.cn/Article/details/gvoalhnmp.sHtML

[U62] PHP：日期对象
来源：http://www.share.bbcook.cn/Article/details/gaumfpzag.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.bbcook.cn/Article/details/gcarbqmuv.sHtML

[U63] PHP：文件读写
来源：http://m.share.epnwcf.com/Article/details/gcsskiqoh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.yfazqb.com/Article/details/giqzddrww.sHtML

[U64] PHP：目录遍历
来源：http://baike.bbcook.cn/Article/details/gmxxrrgcl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.epnwcf.com/Article/details/gwyrxboed.sHtML

[U65] PHP：会话
来源：http://read.share.fktsv.cn/Article/details/gfetyupmx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.vehdjk.com/Article/details/gblmuhjva.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.vehdjk.com/Article/details/gydvimewy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.epnwcf.com/Article/details/gaaabpzlt.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.epnwcf.com/Article/details/gbyiawqpi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.sjlbkw.cn/Article/details/gynlbpeeu.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.sjlbkw.cn/Article/details/gztebhaap.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsjxvhsi.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.sjlbkw.cn/Article/details/ggvlhsptn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.yfazqb.com/Article/details/gmvynohhk.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.bbcook.cn/Article/details/gspglkaon.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.vehdjk.com/Article/details/gsoqcgewj.sHtML

[U71] PHP：抛出异常
来源：http://www.share.bbcook.cn/Article/details/ghlishqry.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.epnwcf.com/Article/details/gpmoxaycm.sHtML

[U72] PHP：写错误日志
来源：http://m.share.bbcook.cn/Article/details/gvnahphhv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.sjlbkw.cn/Article/details/gumitrhge.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.bbcook.cn/Article/details/gptaowbdm.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.epnwcf.com/Article/details/gxwmbpcea.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.epnwcf.com/Article/details/ghwrmokdc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.epnwcf.com/Article/details/gseclxknh.sHtML

[U75] PHP：依赖注入
来源：http://m.share.bbcook.cn/Article/details/gkqhmbrjw.sHtML

composer require psr/container
来源：http://www.blog.bbcook.cn/Article/details/gsonxhqvs.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fktsv.cn/Article/details/gsqwtisqo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fktsv.cn/Article/details/gthtdozoc.sHtML

[U77] PHP：模板渲染
来源：http://wap.fktsv.cn/Article/details/gzqtxkaux.sHtML

composer require twig/twig
来源：http://read.share.sjlbkw.cn/Article/details/gxukecujc.sHtML

[U78] PHP：单元测试
来源：http://blog.yfazqb.com/Article/details/ghklcmmjr.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.bbcook.cn/Article/details/gugmubald.sHtML

[U79] PHP：静态分析
来源：http://www.share.yfazqb.com/Article/details/ggxeiazyx.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.epnwcf.com/Article/details/gsmpnoppt.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.epnwcf.com/Article/details/gyklayoib.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.epnwcf.com/Article/details/genfkkwbe.sHtML

[U81] JS：初始化项目
来源：http://www.blog.tarul.cn/Article/details/gjgpbract.sHtML

npm init -y;  npm i express
来源：http://www.blog.bbcook.cn/Article/details/gluxyecfh.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.tarul.cn/Article/details/guzcmhggh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.vehdjk.com/Article/details/gmtxwyhcx.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.sjlbkw.cn/Article/details/gqkmayavu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.epnwcf.com/Article/details/gkzclonkp.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.yfazqb.com/Article/details/gvecfzncy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.epnwcf.com/Article/details/glghpfpib.sHtML

[U85] JS：可选链
来源：http://www.share.bbcook.cn/Article/details/gekomkqda.sHtML

a?.b?.c
来源：http://mobile.epnwcf.com/Article/details/ggsajxapx.sHtML

[U86] JS：空值合并
来源：http://wap.epnwcf.com/Article/details/gefbseqrk.sHtML

a ?? b
来源：http://wap.fktsv.cn/Article/details/gkwictukq.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fktsv.cn/Article/details/gkpzsweqa.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.epnwcf.com/Article/details/gkvujpwvh.sHtML

[U88] JS：对象展开合并
来源：http://blog.bbcook.cn/Article/details/gpwhehjjd.sHtML

{ ...a, ...b }
来源：http://baike.vehdjk.com/Article/details/gyarifawx.sHtML

[U89] JS：数组去重
来源：http://blog.yfazqb.com/Article/details/girtwaqxy.sHtML

[...new Set(arr)]
来源：http://www.m.share.epnwcf.com/Article/details/gajiortfy.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fktsv.cn/Article/details/gnddwifpj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/godwlhdkt.sHtML

[U91] JS：对象键值遍历
来源：http://blog.epnwcf.com/Article/details/gfxtnizbs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.vehdjk.com/Article/details/ggpjecztg.sHtML

[U92] JS：深拷贝
来源：http://wap.yfazqb.com/Article/details/gitlaoqau.sHtML

structuredClone(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gvpypefvc.sHtML

[U93] JS：模板字符串
来源：http://wap.vehdjk.com/Article/details/gtvtmhewg.sHtML

`共 ${n} 条`
来源：http://www.share.epnwcf.com/Article/details/gyzuymibr.sHtML

[U94] JS：箭头函数
来源：http://read.share.vehdjk.com/Article/details/gvubtldxv.sHtML

const double = x => x * 2;
来源：http://www.share.tarul.cn/Article/details/giftivcsk.sHtML

[U95] JS：Promise 包装
来源：http://mobile.tarul.cn/Article/details/gfersdbxt.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.epnwcf.com/Article/details/grloagvds.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fktsv.cn/Article/details/glthhhsbt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gzedvucvc.sHtML

[U97] JS：并发请求
来源：http://www.blog.bbcook.cn/Article/details/grehlvcdw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/grfvwrvqu.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.sjlbkw.cn/Article/details/guwovfxon.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.epnwcf.com/Article/details/grftxcilu.sHtML

[U99] JS：事件监听
来源：http://www.share.vehdjk.com/Article/details/gamzkjnnf.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.epnwcf.com/Article/details/gqfhlytaj.sHtML

[U100] JS：DOM 查询
来源：http://3g.yfazqb.com/Article/details/gtglsqktn.sHtML

document.querySelector(".item")
来源：http://www.m.share.tarul.cn/Article/details/gcyoadpij.sHtML

[U101] JS：classList 操作
来源：http://www.blog.epnwcf.com/Article/details/gfhazeqyi.sHtML

el.classList.toggle("active")
来源：http://www.share.sjlbkw.cn/Article/details/gmaqqjrdc.sHtML

[U102] JS：本地存储
来源：http://baike.vehdjk.com/Article/details/gslwgkcda.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.epnwcf.com/Article/details/gqevlyddb.sHtML

[U103] JS：定时器
来源：http://read.share.tarul.cn/Article/details/gjwyghhlj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.tarul.cn/Article/details/gqvojimwm.sHtML

[U104] JS：防抖
来源：http://baike.yfazqb.com/Article/details/gmrtbtqec.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/glkqfptsr.sHtML

[U105] JS：节流
来源：http://blog.tarul.cn/Article/details/gcspempbf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.sjlbkw.cn/Article/details/gwvyvqjfe.sHtML

[U106] JS：日期格式化
来源：http://3g.sjlbkw.cn/Article/details/ganxziwgs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.yfazqb.com/Article/details/gyouaehaj.sHtML

[U107] JS：数字千分位
来源：http://3g.tarul.cn/Article/details/gtwzavxcr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.sjlbkw.cn/Article/details/gboidqheq.sHtML

[U108] JS：随机整数
来源：http://baike.fktsv.cn/Article/details/gjckcftov.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.tarul.cn/Article/details/gzqkuwuqi.sHtML

[U109] JS：数组分组
来源：http://baike.yfazqb.com/Article/details/gpdefzzcf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.bbcook.cn/Article/details/glfgpbjdu.sHtML

[U110] JS：数组分块
来源：http://blog.epnwcf.com/Article/details/gzxlspcxl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.epnwcf.com/Article/details/gawazosqo.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.sjlbkw.cn/Article/details/gdesujlfo.sHtML

new Map(Object.entries(obj))
来源：http://blog.epnwcf.com/Article/details/gajjdrytt.sHtML

[U112] JS：字符串补位
来源：http://www.share.fktsv.cn/Article/details/gurjvmvwm.sHtML

"7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/gxazvkzfv.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fktsv.cn/Article/details/gdmtgambo.sHtML

s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/gjzgholry.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.yfazqb.com/Article/details/gqcermbcj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.tarul.cn/Article/details/gjjfxzvaj.sHtML

[U115] JS：生成 UUID
来源：http://mobile.sjlbkw.cn/Article/details/gpntymetg.sHtML

crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/gzaltrota.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.vehdjk.com/Article/details/ggvgsosyn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.sjlbkw.cn/Article/details/gvwjgomun.sHtML

[U117] JS：单元测试
来源：http://m.share.epnwcf.com/Article/details/ggkasczkr.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.bbcook.cn/Article/details/gbiuzptqc.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.yfazqb.com/Article/details/gwujbinco.sHtML

npm i -D vite;  npx vite
来源：http://blog.epnwcf.com/Article/details/gtcuqviyk.sHtML

[U119] JS：生产构建
来源：http://www.blog.yfazqb.com/Article/details/ghbmevata.sHtML

npx vite build
来源：http://read.share.sjlbkw.cn/Article/details/gpwrpjxkl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.sjlbkw.cn/Article/details/gwygktvjt.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.epnwcf.com/Article/details/gzwgzgkth.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gepqbopev.sHtML

统计汇总
来源：http://mobile.sjlbkw.cn/Article/details/gaauhhewz.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/guktuyrdt.sHtML

按语言统计（条）：
来源：http://www.m.share.tarul.cn/Article/details/gudszmrwa.sHtML

Python ......... 252
来源：http://www.blog.sjlbkw.cn/Article/details/gmgpsesnv.sHtML

PHP ............ 252
来源：http://www.blog.epnwcf.com/Article/details/gbgjjmcou.sHtML

JavaScript ..... 252
来源：http://mobile.sjlbkw.cn/Article/details/gcggfhbcy.sHtML

TypeScript ..... 212
来源：http://wap.epnwcf.com/Article/details/gjfpqdoqr.sHtML

Java ........... 212
来源：http://www.m.share.epnwcf.com/Article/details/gnwzljmiq.sHtML

Go ............. 212
来源：http://www.share.sjlbkw.cn/Article/details/gycqosepv.sHtML

Ruby ........... 212
来源：http://3g.fktsv.cn/Article/details/gajzvrjie.sHtML

C# ............. 212
来源：http://m.share.epnwcf.com/Article/details/gdebenpbx.sHtML

C .............. 30
来源：http://www.m.share.epnwcf.com/Article/details/gtjlwaref.sHtML

C++ ............ 30
来源：http://read.share.sjlbkw.cn/Article/details/glqoivcoh.sHtML

SQL ............ 90
来源：http://read.share.sjlbkw.cn/Article/details/ggzjorrwq.sHtML

Bash ........... 80
来源：http://read.share.tarul.cn/Article/details/gmjlsdkor.sHtML

Kotlin ......... 15
来源：http://www.share.epnwcf.com/Article/details/gpupsykqs.sHtML

Swift .......... 15
来源：http://mobile.fktsv.cn/Article/details/gnpohsccu.sHtML

Lua ............ 10
来源：http://read.share.fktsv.cn/Article/details/ggsgztvjn.sHtML

Perl ........... 10
来源：http://m.share.vehdjk.com/Article/details/gahfcaxji.sHtML

Scala .......... 10
来源：http://baike.vehdjk.com/Article/details/gbzggwrbv.sHtML

------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gglzxcloo.sHtML

合计 ........... 2106 条
来源：http://mobile.bbcook.cn/Article/details/gzpumybyj.sHtML

按章节统计：
来源：http://www.blog.yfazqb.com/Article/details/gyrhgggdc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.bbcook.cn/Article/details/gzrwpvuqg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.tarul.cn/Article/details/gavyqadqy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fktsv.cn/Article/details/gaovsztla.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.bbcook.cn/Article/details/gtipwnoov.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.tarul.cn/Article/details/goandrzxj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.vehdjk.com/Article/details/gqjunedwf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.yfazqb.com/Article/details/gqfupplrl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.yfazqb.com/Article/details/gfaaauiqv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/ghkwmgpqx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.epnwcf.com/Article/details/gmyyuhvvx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gcyuetpkw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gkyiedgmc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/goysmwfal.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.bbcook.cn/Article/details/gkyjfqier.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.epnwcf.com/Article/details/gmmgekyxq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/gbttkxmvg.sHtML

Q SQL 专题                              90
来源：http://wap.bbcook.cn/Article/details/gqiyrtcyt.sHtML

R Bash 专题                             80
来源：http://www.blog.sjlbkw.cn/Article/details/gpvjxunzo.sHtML

S C / C++ 专题                          60
来源：http://read.share.sjlbkw.cn/Article/details/gsvtntrae.sHtML

T 其他语言补充                          60
来源：http://mobile.bbcook.cn/Article/details/ghdaxnysl.sHtML

U 高频实用片段                         120
来源：http://www.blog.fktsv.cn/Article/details/glzrxhrwx.sHtML

------------------------------------
来源：http://3g.yfazqb.com/Article/details/gkvbeufet.sHtML

合计                                  2106 条
来源：http://www.share.yfazqb.com/Article/details/gtjytghuk.sHtML

--------------------------------------------------------------------------------
来源：http://wap.yfazqb.com/Article/details/gppmoelqe.sHtML

使用提醒
来源：http://m.share.fktsv.cn/Article/details/gfuwehzuq.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/grpqbvtps.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.tarul.cn/Article/details/gwabzboat.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.vehdjk.com/Article/details/grvfynpoz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.tarul.cn/Article/details/gbxolrtlr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.tarul.cn/Article/details/gjkdpntwm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.sjlbkw.cn/Article/details/gpevankkd.sHtML

—— 文件结束 ——
来源：http://www.share.fktsv.cn/Article/details/ggszgobpc.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gdrubxvrq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fktsv.cn/Article/details/gtjfjodet.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.epnwcf.com/Article/details/girfdvdrw.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gtafwxntw.sHtML

【收录内容】
来源：http://wap.fktsv.cn/Article/details/goxglyhcl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.epnwcf.com/Article/details/geibquauz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.yfazqb.com/Article/details/gvwejilvn.sHtML

SQL · Bash · C · C++
来源：http://www.blog.sjlbkw.cn/Article/details/gdamlccvw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.sjlbkw.cn/Article/details/gobjwkxuo.sHtML

【使用说明】
来源：http://www.m.share.vehdjk.com/Article/details/gxktfkxdj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.sjlbkw.cn/Article/details/gtcadwwnu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.yfazqb.com/Article/details/gzqyxqtft.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.sjlbkw.cn/Article/details/gvxzfwvjh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fktsv.cn/Article/details/gylevieof.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.sjlbkw.cn/Article/details/gqafzlaih.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fktsv.cn/Article/details/gejymyrtu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.tarul.cn/Article/details/gyzbbhnup.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.epnwcf.com/Article/details/gnmitrxxd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.tarul.cn/Article/details/gengkqvby.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.epnwcf.com/Article/details/gqplcuxng.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.epnwcf.com/Article/details/ggunippgb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.sjlbkw.cn/Article/details/gpktdtatu.sHtML

【文件统计】
来源：http://mobile.tarul.cn/Article/details/grggmssdu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.epnwcf.com/Article/details/gbslssqki.sHtML

--------------------------------------------------------------------------------
来源：http://3g.vehdjk.com/Article/details/gssobhjpy.sHtML

目  录
来源：http://blog.fktsv.cn/Article/details/gdbgohaxf.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gmbyipkoz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.vehdjk.com/Article/details/gsegnwpho.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.yfazqb.com/Article/details/gztwvabiz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.yfazqb.com/Article/details/gdipmskoi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.epnwcf.com/Article/details/gmvovxgke.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.sjlbkw.cn/Article/details/gpgmijmmp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.epnwcf.com/Article/details/gijywzfxm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.epnwcf.com/Article/details/glyjcxpnc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.sjlbkw.cn/Article/details/gzczkcvsl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.bbcook.cn/Article/details/gdxsbwsvl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.epnwcf.com/Article/details/grxgkpnll.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.sjlbkw.cn/Article/details/gezgywcja.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.yfazqb.com/Article/details/guplookfl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/gujdshmtm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.bbcook.cn/Article/details/gzvkekhon.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.yfazqb.com/Article/details/gocwjvqol.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.vehdjk.com/Article/details/gdohvgxwu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.epnwcf.com/Article/details/gkdmieamp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fktsv.cn/Article/details/gwsqtcnpy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.tarul.cn/Article/details/gzkhqogfw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgljrigl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzbdfjvj.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/grzdelcvm.sHtML

A. 基础语法与类型
来源：http://wap.yfazqb.com/Article/details/gjeduryhv.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gxdtxvhjr.sHtML

[A01] Hello World
来源：http://www.share.epnwcf.com/Article/details/gflyaitnj.sHtML

Py:   print("Hello, World!")
来源：http://baike.bbcook.cn/Article/details/gbpsbaafu.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.epnwcf.com/Article/details/gydpsbqsr.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fktsv.cn/Article/details/gfmsadfvm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fktsv.cn/Article/details/gqatgwmog.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.tarul.cn/Article/details/gfgeijjdw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.tarul.cn/Article/details/gukzaeoqr.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.bbcook.cn/Article/details/glrptbfah.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.tarul.cn/Article/details/gcnnpzfiy.sHtML

[A02] 变量声明与赋值
来源：http://blog.vehdjk.com/Article/details/glstpjpto.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.sjlbkw.cn/Article/details/gwjpvayiz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.epnwcf.com/Article/details/gqywjsphk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.bbcook.cn/Article/details/gdhwkwsmi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fktsv.cn/Article/details/glqhandgt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fktsv.cn/Article/details/grskrebtz.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.sjlbkw.cn/Article/details/gyxsjthih.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.vehdjk.com/Article/details/gmbfrkwzl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fktsv.cn/Article/details/giiacofkf.sHtML

[A03] 常量定义
来源：http://mobile.fktsv.cn/Article/details/gvhkgpzby.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.epnwcf.com/Article/details/gkedogmld.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/glmkmglys.sHtML

JS:   const PI = 3.14159;
来源：http://3g.yfazqb.com/Article/details/gtesxunjp.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/glsqgauet.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gineqfyci.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.tarul.cn/Article/details/gdldkehss.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.bbcook.cn/Article/details/gyabtpgem.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gcuczahtx.sHtML

[A04] 判断变量类型
来源：http://3g.bbcook.cn/Article/details/gfhzsmqpo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fktsv.cn/Article/details/gyjwqzzxg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.tarul.cn/Article/details/gwcmnssjp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.yfazqb.com/Article/details/ggmmuzwbn.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.bbcook.cn/Article/details/ganefhibs.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fktsv.cn/Article/details/gajrquagc.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.yfazqb.com/Article/details/gqvpkuuty.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.yfazqb.com/Article/details/gklqkljin.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.yfazqb.com/Article/details/gvlguyhkn.sHtML

[A05] 整数除法与取模
来源：http://blog.sjlbkw.cn/Article/details/gypbyzslr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.tarul.cn/Article/details/ghmlcgalu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/gihntuhsm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.vehdjk.com/Article/details/gncnmdkdi.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.yfazqb.com/Article/details/grkqfqkms.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.epnwcf.com/Article/details/gwabkvdfp.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.tarul.cn/Article/details/gvkuznwhb.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.sjlbkw.cn/Article/details/gadujxzjx.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fktsv.cn/Article/details/gxguixnzf.sHtML

[A06] 字符串转数字
来源：http://baike.epnwcf.com/Article/details/gawzdyill.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.bbcook.cn/Article/details/ghidrynxc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.bbcook.cn/Article/details/gzintadmn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.vehdjk.com/Article/details/gbiafnvol.sHtML


<!-- 参考信息 -->