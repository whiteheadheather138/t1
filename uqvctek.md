代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://3g.fktsv.cn/Article/details/grntrcrky.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gyykkdjfa.sHtML

[U46] PHP：可空类型
来源：http://baike.tarul.cn/Article/details/gtmururgu.sHtML

?string $name = null
来源：http://www.blog.bbcook.cn/Article/details/gffqzyaoy.sHtML

[U47] PHP：联合类型
来源：http://read.share.sjlbkw.cn/Article/details/gvfnhazyu.sHtML

int|string $id
来源：http://read.share.tarul.cn/Article/details/gijrfalvz.sHtML

[U48] PHP：纯枚举
来源：http://m.share.sjlbkw.cn/Article/details/gubzvosjx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.epnwcf.com/Article/details/gwyuaqcny.sHtML

[U49] PHP：只读属性
来源：http://m.share.vehdjk.com/Article/details/gzswtidam.sHtML

public readonly string $name
来源：http://blog.epnwcf.com/Article/details/grukstagc.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.tarul.cn/Article/details/gwpshppdk.sHtML

public function __construct(private int $id) {}
来源：http://mobile.tarul.cn/Article/details/gptnupsjb.sHtML

[U51] PHP：数组解构
来源：http://www.blog.tarul.cn/Article/details/gfmipnmvo.sHtML

[$a, $b] = $arr;
来源：http://wap.fktsv.cn/Article/details/gsfbhgrye.sHtML

[U52] PHP：箭头函数
来源：http://read.share.sjlbkw.cn/Article/details/grjupbkex.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.tarul.cn/Article/details/gyjriusly.sHtML

[U53] PHP：空合并运算符
来源：http://blog.tarul.cn/Article/details/geytishmf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.bbcook.cn/Article/details/grfppijwy.sHtML

[U54] PHP：空安全调用
来源：http://baike.tarul.cn/Article/details/grsjjgbvy.sHtML

$obj?->method()
来源：http://www.m.share.vehdjk.com/Article/details/gqelfrqhs.sHtML

[U55] PHP：match 表达式
来源：http://wap.sjlbkw.cn/Article/details/gvjwhtggr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.tarul.cn/Article/details/ghqxhrckb.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fktsv.cn/Article/details/geyxsthmx.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gxtiibwar.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwzebspe.sHtML

"值: {$a}"
来源：http://wap.vehdjk.com/Article/details/gvjmxqoeo.sHtML

[U58] PHP：数组三件套
来源：http://mobile.sjlbkw.cn/Article/details/gkcizskbi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.bbcook.cn/Article/details/glthztjys.sHtML

[U59] PHP：自定义排序
来源：http://baike.bbcook.cn/Article/details/gzaaqictu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.bbcook.cn/Article/details/gswtyfblv.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.tarul.cn/Article/details/goierlsfk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.tarul.cn/Article/details/gzyrgwlvo.sHtML

[U61] PHP：正则
来源：http://blog.bbcook.cn/Article/details/gxhtgyfna.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.bbcook.cn/Article/details/gbigtpbux.sHtML

[U62] PHP：日期对象
来源：http://baike.sjlbkw.cn/Article/details/gihkvnkas.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.yfazqb.com/Article/details/gfhkceevu.sHtML

[U63] PHP：文件读写
来源：http://blog.vehdjk.com/Article/details/gxlgmlkgr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.sjlbkw.cn/Article/details/gnoktpsul.sHtML

[U64] PHP：目录遍历
来源：http://m.share.sjlbkw.cn/Article/details/gvsfmshlf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.vehdjk.com/Article/details/goiesjeyv.sHtML

[U65] PHP：会话
来源：http://www.blog.fktsv.cn/Article/details/gfgbmtnnh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.vehdjk.com/Article/details/gykwigegd.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.epnwcf.com/Article/details/gdpbjgzmj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.bbcook.cn/Article/details/gseubipdg.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.yfazqb.com/Article/details/gjkcrltlo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fktsv.cn/Article/details/ggnguemsv.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.bbcook.cn/Article/details/glutjlnhs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.epnwcf.com/Article/details/gsauatkxn.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.tarul.cn/Article/details/gnzcdehsx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fktsv.cn/Article/details/gmccxfzvm.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.bbcook.cn/Article/details/gofxzssnj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.bbcook.cn/Article/details/ggpbhbtpr.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fktsv.cn/Article/details/gxnuhtrbn.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.bbcook.cn/Article/details/gcamqoizg.sHtML

[U72] PHP：写错误日志
来源：http://wap.bbcook.cn/Article/details/gsdsxascl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.tarul.cn/Article/details/gkblpflwc.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.epnwcf.com/Article/details/gfqnsyjac.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fktsv.cn/Article/details/gdhaoeopn.sHtML

[U74] PHP：读取环境变量
来源：http://3g.vehdjk.com/Article/details/guygilita.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fktsv.cn/Article/details/gmzhooydi.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.vehdjk.com/Article/details/gxcmgwujz.sHtML

composer require psr/container
来源：http://www.blog.epnwcf.com/Article/details/gomvcpzly.sHtML

[U76] PHP：简单路由
来源：http://3g.tarul.cn/Article/details/gyyqthqsd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.yfazqb.com/Article/details/gnmimodhb.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcubqjzx.sHtML

composer require twig/twig
来源：http://read.share.fktsv.cn/Article/details/gjiyrdlbt.sHtML

[U78] PHP：单元测试
来源：http://3g.bbcook.cn/Article/details/gnbyhbcvc.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.bbcook.cn/Article/details/gcuibqkfr.sHtML

[U79] PHP：静态分析
来源：http://mobile.yfazqb.com/Article/details/gyraguoty.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.bbcook.cn/Article/details/gkypnsrwu.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.sjlbkw.cn/Article/details/gbdcfbpkk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.sjlbkw.cn/Article/details/ggfnjsjlv.sHtML

[U81] JS：初始化项目
来源：http://read.share.epnwcf.com/Article/details/gjmvbpgfh.sHtML

npm init -y;  npm i express
来源：http://mobile.fktsv.cn/Article/details/getsaiqni.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.tarul.cn/Article/details/gbijtfdod.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.sjlbkw.cn/Article/details/gkoikoviz.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fktsv.cn/Article/details/gbjxasbhh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.vehdjk.com/Article/details/gnsypafeh.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.tarul.cn/Article/details/growecggz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.epnwcf.com/Article/details/gphqhmzkh.sHtML

[U85] JS：可选链
来源：http://www.m.share.fktsv.cn/Article/details/gbivwlyxg.sHtML

a?.b?.c
来源：http://m.share.tarul.cn/Article/details/gsweoeylm.sHtML

[U86] JS：空值合并
来源：http://www.m.share.yfazqb.com/Article/details/gacspjvhw.sHtML

a ?? b
来源：http://blog.epnwcf.com/Article/details/gbcflbdqj.sHtML

[U87] JS：解构默认值
来源：http://baike.bbcook.cn/Article/details/gsfthnngc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.yfazqb.com/Article/details/grtwdolwu.sHtML

[U88] JS：对象展开合并
来源：http://3g.epnwcf.com/Article/details/gdlxwtuoc.sHtML

{ ...a, ...b }
来源：http://www.share.tarul.cn/Article/details/goxhfbxhb.sHtML

[U89] JS：数组去重
来源：http://blog.sjlbkw.cn/Article/details/gylpaserm.sHtML

[...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/gmsrgvmzd.sHtML

[U90] JS：数字数组排序
来源：http://wap.bbcook.cn/Article/details/gwkszkqrb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.tarul.cn/Article/details/ggdjjnotl.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.vehdjk.com/Article/details/grsdhdtpd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.tarul.cn/Article/details/gacsawjle.sHtML

[U92] JS：深拷贝
来源：http://mobile.tarul.cn/Article/details/gejpkmjqy.sHtML

structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gggkrbhwe.sHtML

[U93] JS：模板字符串
来源：http://www.share.bbcook.cn/Article/details/gasdgbtom.sHtML

`共 ${n} 条`
来源：http://www.blog.epnwcf.com/Article/details/goqxftpvh.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvgtarve.sHtML

const double = x => x * 2;
来源：http://m.share.tarul.cn/Article/details/gugoxvglh.sHtML

[U95] JS：Promise 包装
来源：http://3g.bbcook.cn/Article/details/gtiyccrrc.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.sjlbkw.cn/Article/details/glrcguldd.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fktsv.cn/Article/details/gysqbwmvd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/gyotluxjd.sHtML

[U97] JS：并发请求
来源：http://www.share.bbcook.cn/Article/details/glddobvuw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/giusqrxmp.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.epnwcf.com/Article/details/gfnwqakcy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.yfazqb.com/Article/details/glgtjpfls.sHtML

[U99] JS：事件监听
来源：http://m.share.fktsv.cn/Article/details/gowadscma.sHtML

el.addEventListener("click", e => {})
来源：http://baike.epnwcf.com/Article/details/gcwublowh.sHtML

[U100] JS：DOM 查询
来源：http://wap.vehdjk.com/Article/details/gtfzffqrn.sHtML

document.querySelector(".item")
来源：http://3g.vehdjk.com/Article/details/gnafnekio.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.vehdjk.com/Article/details/gmiqxzzxy.sHtML

el.classList.toggle("active")
来源：http://www.m.share.sjlbkw.cn/Article/details/grrqhzixd.sHtML

[U102] JS：本地存储
来源：http://mobile.fktsv.cn/Article/details/gfbuxnzxj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.epnwcf.com/Article/details/gdklzsftc.sHtML

[U103] JS：定时器
来源：http://3g.fktsv.cn/Article/details/ggzlsblec.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.tarul.cn/Article/details/gymgyeunr.sHtML

[U104] JS：防抖
来源：http://3g.vehdjk.com/Article/details/gkdopjxvx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/googjenla.sHtML

[U105] JS：节流
来源：http://baike.bbcook.cn/Article/details/gfojludki.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.yfazqb.com/Article/details/grfxxutkk.sHtML

[U106] JS：日期格式化
来源：http://read.share.fktsv.cn/Article/details/gnolzslgi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.yfazqb.com/Article/details/gbkphhuys.sHtML

[U107] JS：数字千分位
来源：http://blog.vehdjk.com/Article/details/geekmvlts.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.tarul.cn/Article/details/gwobscgsz.sHtML

[U108] JS：随机整数
来源：http://baike.yfazqb.com/Article/details/gsrqmeewd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.sjlbkw.cn/Article/details/gnodvcsui.sHtML

[U109] JS：数组分组
来源：http://www.m.share.yfazqb.com/Article/details/ghsacygvn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.sjlbkw.cn/Article/details/geyrjsrxj.sHtML

[U110] JS：数组分块
来源：http://blog.epnwcf.com/Article/details/gvddqreit.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.tarul.cn/Article/details/gixkrfdei.sHtML

[U111] JS：对象转 Map
来源：http://3g.bbcook.cn/Article/details/gzuvssoal.sHtML

new Map(Object.entries(obj))
来源：http://blog.epnwcf.com/Article/details/gwipfvoda.sHtML

[U112] JS：字符串补位
来源：http://mobile.bbcook.cn/Article/details/gobnmjdyw.sHtML

"7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gfkmikcsv.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.vehdjk.com/Article/details/gjornvuog.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gjdeciemt.sHtML

[U114] JS：JSON 深比较
来源：http://blog.epnwcf.com/Article/details/gwbhssvwj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.yfazqb.com/Article/details/gzsnjledn.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.bbcook.cn/Article/details/glkzopodb.sHtML

crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gflbkgxhm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.bbcook.cn/Article/details/geivmmpmk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fktsv.cn/Article/details/gitnhkrmn.sHtML

[U117] JS：单元测试
来源：http://m.share.yfazqb.com/Article/details/grqyhicaw.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.yfazqb.com/Article/details/ggxfjdyxr.sHtML

[U118] JS：开发服务器
来源：http://m.share.tarul.cn/Article/details/gngatatjr.sHtML

npm i -D vite;  npx vite
来源：http://mobile.epnwcf.com/Article/details/gpcghecil.sHtML

[U119] JS：生产构建
来源：http://m.share.yfazqb.com/Article/details/ghvqhqtmy.sHtML

npx vite build
来源：http://baike.tarul.cn/Article/details/gzbpmecex.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.sjlbkw.cn/Article/details/gdlfpspqh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.epnwcf.com/Article/details/gnlyfzags.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gtbgdburf.sHtML

统计汇总
来源：http://read.share.fktsv.cn/Article/details/gdckmqgqf.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gobdowlvv.sHtML

按语言统计（条）：
来源：http://www.m.share.vehdjk.com/Article/details/gpebktwmu.sHtML

Python ......... 252
来源：http://blog.sjlbkw.cn/Article/details/gwmnmsiyx.sHtML

PHP ............ 252
来源：http://baike.tarul.cn/Article/details/gtmvzpnaw.sHtML

JavaScript ..... 252
来源：http://m.share.fktsv.cn/Article/details/gjasmxkcv.sHtML

TypeScript ..... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgaswqyq.sHtML

Java ........... 212
来源：http://www.share.fktsv.cn/Article/details/goczqadyj.sHtML

Go ............. 212
来源：http://read.share.epnwcf.com/Article/details/gmucliuhs.sHtML

Ruby ........... 212
来源：http://m.share.bbcook.cn/Article/details/gigwxkeih.sHtML

C# ............. 212
来源：http://m.share.epnwcf.com/Article/details/gogjqllmo.sHtML

C .............. 30
来源：http://www.m.share.tarul.cn/Article/details/gwrivboov.sHtML

C++ ............ 30
来源：http://read.share.yfazqb.com/Article/details/gbduhobhp.sHtML

SQL ............ 90
来源：http://m.share.bbcook.cn/Article/details/gbhwurkrs.sHtML

Bash ........... 80
来源：http://mobile.vehdjk.com/Article/details/gckpxjfal.sHtML

Kotlin ......... 15
来源：http://3g.vehdjk.com/Article/details/genwpafxs.sHtML

Swift .......... 15
来源：http://www.share.sjlbkw.cn/Article/details/guoyvilcr.sHtML

Lua ............ 10
来源：http://baike.epnwcf.com/Article/details/gseyyxsqb.sHtML

Perl ........... 10
来源：http://www.share.tarul.cn/Article/details/gajkwwvwf.sHtML

Scala .......... 10
来源：http://www.m.share.epnwcf.com/Article/details/gdycnyuvh.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/gkpxlcual.sHtML

合计 ........... 2106 条
来源：http://blog.yfazqb.com/Article/details/gydyuisis.sHtML

按章节统计：
来源：http://3g.tarul.cn/Article/details/gukppshev.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.bbcook.cn/Article/details/gzrrdxldu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.yfazqb.com/Article/details/gqwovbpiz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.epnwcf.com/Article/details/gmzpqugwt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.epnwcf.com/Article/details/gkmpljjbj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.vehdjk.com/Article/details/gmygfrude.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.vehdjk.com/Article/details/gmbbgfdnw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.yfazqb.com/Article/details/gdpdfsvno.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.tarul.cn/Article/details/gkwdxzlwf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.sjlbkw.cn/Article/details/gmufuiuef.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.sjlbkw.cn/Article/details/gdbxnrpdl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gvtuggrhm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/grnmpitxx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fktsv.cn/Article/details/gwrmyzpzu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.epnwcf.com/Article/details/gfzytvtja.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.bbcook.cn/Article/details/getpqxwrh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/ggogyfjfs.sHtML

Q SQL 专题                              90
来源：http://www.m.share.bbcook.cn/Article/details/gkstcaoup.sHtML

R Bash 专题                             80
来源：http://baike.epnwcf.com/Article/details/guhhdkets.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.yfazqb.com/Article/details/gswzxszml.sHtML

T 其他语言补充                          60
来源：http://www.share.epnwcf.com/Article/details/gnkxnigrb.sHtML

U 高频实用片段                         120
来源：http://www.blog.bbcook.cn/Article/details/gzgkhwgha.sHtML

------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gfvkyesln.sHtML

合计                                  2106 条
来源：http://baike.tarul.cn/Article/details/gdcphknyu.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/guzsiqeqx.sHtML

使用提醒
来源：http://3g.vehdjk.com/Article/details/gwuyvcfal.sHtML

--------------------------------------------------------------------------------
来源：http://wap.epnwcf.com/Article/details/gyirmamqu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.yfazqb.com/Article/details/gnrczmvgo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.vehdjk.com/Article/details/gafveoozf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.tarul.cn/Article/details/gryuoqkic.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.yfazqb.com/Article/details/gjexpowta.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.bbcook.cn/Article/details/gtwhxyimc.sHtML

—— 文件结束 ——
来源：http://baike.fktsv.cn/Article/details/gsljkvbcq.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gvmxnaqvo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fktsv.cn/Article/details/gfkftzaeg.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.yfazqb.com/Article/details/gtrajescq.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gjjupzspy.sHtML

【收录内容】
来源：http://wap.vehdjk.com/Article/details/gdhcxkysd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.epnwcf.com/Article/details/glnfaklcu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.yfazqb.com/Article/details/gkxkhckyx.sHtML

SQL · Bash · C · C++
来源：http://baike.yfazqb.com/Article/details/gznswsxah.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fktsv.cn/Article/details/ghuxoqgjt.sHtML

【使用说明】
来源：http://www.share.yfazqb.com/Article/details/gropnjgtq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fktsv.cn/Article/details/garxdakmx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.vehdjk.com/Article/details/gjuneljqf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.vehdjk.com/Article/details/glvniongd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.vehdjk.com/Article/details/girpuvmyf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fktsv.cn/Article/details/gvxwjjhho.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.vehdjk.com/Article/details/ggabegkcb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fktsv.cn/Article/details/gyvgcsiwq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.epnwcf.com/Article/details/ghtmsphly.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fktsv.cn/Article/details/gngauwmmw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.sjlbkw.cn/Article/details/gpfnkpnaf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fktsv.cn/Article/details/gwpcwvsbm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.sjlbkw.cn/Article/details/gslexwauy.sHtML

【文件统计】
来源：http://m.share.epnwcf.com/Article/details/gdkurodga.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.tarul.cn/Article/details/gqtuhvabd.sHtML

--------------------------------------------------------------------------------
来源：http://blog.yfazqb.com/Article/details/gsqvuofna.sHtML

目  录
来源：http://www.share.bbcook.cn/Article/details/ggbimugwu.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/gbleuehjm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.bbcook.cn/Article/details/gjmbbcrxj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.bbcook.cn/Article/details/gfoowpyxa.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.bbcook.cn/Article/details/gphcqjbql.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.sjlbkw.cn/Article/details/gmohjpjwx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.vehdjk.com/Article/details/gelghzhrp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.sjlbkw.cn/Article/details/gsdvwzaqy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.sjlbkw.cn/Article/details/geuavvhkk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fktsv.cn/Article/details/ggonzvseq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fktsv.cn/Article/details/gdsolzaea.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.yfazqb.com/Article/details/gjrytnfyt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.bbcook.cn/Article/details/gbakndlzj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.epnwcf.com/Article/details/gsfzjyjij.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/gxrgllajx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.vehdjk.com/Article/details/gzcwmagwu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.sjlbkw.cn/Article/details/gwtctjjyq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gfxlagnog.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.bbcook.cn/Article/details/ghvnjiqyi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.epnwcf.com/Article/details/gqjfdqrkp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.vehdjk.com/Article/details/gcrmaqmsn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.epnwcf.com/Article/details/gqomloorj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/gtqzhjjys.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gklqpabol.sHtML

A. 基础语法与类型
来源：http://mobile.vehdjk.com/Article/details/gmhwlftff.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/glvzvncwh.sHtML

[A01] Hello World
来源：http://wap.epnwcf.com/Article/details/grpedezln.sHtML

Py:   print("Hello, World!")
来源：http://www.share.sjlbkw.cn/Article/details/govgkwrpp.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.yfazqb.com/Article/details/ghphqjfrh.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.epnwcf.com/Article/details/gvugudcsu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fktsv.cn/Article/details/gfwtskcqg.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.yfazqb.com/Article/details/gotjvndvk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.sjlbkw.cn/Article/details/gculvxgxu.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.sjlbkw.cn/Article/details/gqmwtsqds.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fktsv.cn/Article/details/gwhrmzsvp.sHtML

[A02] 变量声明与赋值
来源：http://3g.yfazqb.com/Article/details/gzcpthcjz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.epnwcf.com/Article/details/gsnphshde.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fktsv.cn/Article/details/gnzbfxatt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.vehdjk.com/Article/details/gfjszqkhj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.vehdjk.com/Article/details/gewhfuakk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.epnwcf.com/Article/details/ggetecvsf.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.bbcook.cn/Article/details/gchumrkyx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.tarul.cn/Article/details/gpudseggh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.bbcook.cn/Article/details/gndvfdfyg.sHtML

[A03] 常量定义
来源：http://mobile.epnwcf.com/Article/details/gxhycpbes.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.yfazqb.com/Article/details/gpxqigapu.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/ghcuxdxqp.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gftnnlfqn.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.tarul.cn/Article/details/gluspvloj.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gztzidxkz.sHtML

Go:   const PI = 3.14159
来源：http://3g.sjlbkw.cn/Article/details/gtprkfjtu.sHtML

Ruby: PI = 3.14159
来源：http://m.share.sjlbkw.cn/Article/details/gycumpzni.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gsicgosxm.sHtML

[A04] 判断变量类型
来源：http://www.blog.yfazqb.com/Article/details/gayfbkver.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.tarul.cn/Article/details/gucdtcdut.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.bbcook.cn/Article/details/gviwaiqvr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.tarul.cn/Article/details/gqarovxmd.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.epnwcf.com/Article/details/gqebqlzcf.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.bbcook.cn/Article/details/gexpztgkv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.sjlbkw.cn/Article/details/gdeeoxibu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.bbcook.cn/Article/details/gycoaaoxg.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.vehdjk.com/Article/details/gxwzmbgqt.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.epnwcf.com/Article/details/gskmzhhjl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.yfazqb.com/Article/details/grbtovkyu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.vehdjk.com/Article/details/gtsornthm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.tarul.cn/Article/details/glldktadg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.yfazqb.com/Article/details/gbxyetuwa.sHtML


<!-- 参考信息 -->