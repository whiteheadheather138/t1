代发 wailian999

[U47] PHP：联合类型
来源：http://m.share.tarul.cn/Article/details/gakicksuq.sHtML

int|string $id
来源：http://read.share.fktsv.cn/Article/details/giqflmvbt.sHtML

[U48] PHP：纯枚举
来源：http://blog.yfazqb.com/Article/details/ghbldgogf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.tarul.cn/Article/details/gywbjqlpd.sHtML

[U49] PHP：只读属性
来源：http://blog.yfazqb.com/Article/details/grkuyhygr.sHtML

public readonly string $name
来源：http://read.share.vehdjk.com/Article/details/grphgqvon.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fktsv.cn/Article/details/ggbjvvqov.sHtML

public function __construct(private int $id) {}
来源：http://3g.bbcook.cn/Article/details/gnzuuclpp.sHtML

[U51] PHP：数组解构
来源：http://m.share.sjlbkw.cn/Article/details/gdtwrluav.sHtML

[$a, $b] = $arr;
来源：http://m.share.bbcook.cn/Article/details/guozbxtff.sHtML

[U52] PHP：箭头函数
来源：http://wap.yfazqb.com/Article/details/grubtsvem.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.epnwcf.com/Article/details/gekxkntqp.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.bbcook.cn/Article/details/gqufauent.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.sjlbkw.cn/Article/details/gvintvfzo.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.bbcook.cn/Article/details/grlezxfpb.sHtML

$obj?->method()
来源：http://m.share.tarul.cn/Article/details/gqnegezxk.sHtML

[U55] PHP：match 表达式
来源：http://blog.yfazqb.com/Article/details/gzyivjdca.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.yfazqb.com/Article/details/gdxlklhrg.sHtML

[U56] PHP：命名参数
来源：http://www.blog.yfazqb.com/Article/details/gowelxsxp.sHtML

f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gileduiqi.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gaeuvquwq.sHtML

"值: {$a}"
来源：http://read.share.bbcook.cn/Article/details/gpvpolioh.sHtML

[U58] PHP：数组三件套
来源：http://wap.epnwcf.com/Article/details/gthjrxpgk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.tarul.cn/Article/details/gtzpuawot.sHtML

[U59] PHP：自定义排序
来源：http://m.share.epnwcf.com/Article/details/gunnmbfpj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fktsv.cn/Article/details/gcmpwpdhc.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fktsv.cn/Article/details/guxrgymva.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.tarul.cn/Article/details/gzffcifvs.sHtML

[U61] PHP：正则
来源：http://read.share.fktsv.cn/Article/details/grbgnoymu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.sjlbkw.cn/Article/details/ghyvocgsl.sHtML

[U62] PHP：日期对象
来源：http://read.share.yfazqb.com/Article/details/gcjwzcrzw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.epnwcf.com/Article/details/gljlkgpeu.sHtML

[U63] PHP：文件读写
来源：http://wap.sjlbkw.cn/Article/details/gbusjjkda.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.vehdjk.com/Article/details/gnxpdeedj.sHtML

[U64] PHP：目录遍历
来源：http://3g.epnwcf.com/Article/details/ghtvctrlf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.bbcook.cn/Article/details/gilamrtrv.sHtML

[U65] PHP：会话
来源：http://mobile.tarul.cn/Article/details/gzrfunvqc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.bbcook.cn/Article/details/gbmvmiesb.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.vehdjk.com/Article/details/gwgsbzfrc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.vehdjk.com/Article/details/gtujzgule.sHtML

[U67] PHP：处理文件上传
来源：http://wap.yfazqb.com/Article/details/gdxfcnalx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.vehdjk.com/Article/details/gydyipeoh.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fktsv.cn/Article/details/gwqclpskw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.epnwcf.com/Article/details/gwdicvogy.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fktsv.cn/Article/details/gbbfpkupo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.vehdjk.com/Article/details/grxjwazgw.sHtML

[U70] PHP：PDO 事务
来源：http://blog.yfazqb.com/Article/details/gyexbekzy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fktsv.cn/Article/details/gdbuhamxf.sHtML

[U71] PHP：抛出异常
来源：http://wap.tarul.cn/Article/details/goutfbrvo.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.sjlbkw.cn/Article/details/gsrbkqcvx.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.epnwcf.com/Article/details/glfriyddr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.tarul.cn/Article/details/gpjhsmyos.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.sjlbkw.cn/Article/details/gvkvgtyhe.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.vehdjk.com/Article/details/ggfaezdxe.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fktsv.cn/Article/details/gnxeagggj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.tarul.cn/Article/details/gpjcblekg.sHtML

[U75] PHP：依赖注入
来源：http://mobile.yfazqb.com/Article/details/ggemnqjfu.sHtML

composer require psr/container
来源：http://www.m.share.fktsv.cn/Article/details/gmmlzjryu.sHtML

[U76] PHP：简单路由
来源：http://baike.vehdjk.com/Article/details/gjtapdkeh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.epnwcf.com/Article/details/gfyfzjhdj.sHtML

[U77] PHP：模板渲染
来源：http://mobile.tarul.cn/Article/details/gbhokxjkr.sHtML

composer require twig/twig
来源：http://www.blog.yfazqb.com/Article/details/gpvroybjt.sHtML

[U78] PHP：单元测试
来源：http://mobile.tarul.cn/Article/details/ghaghowlp.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.epnwcf.com/Article/details/gvvyvfnar.sHtML

[U79] PHP：静态分析
来源：http://m.share.tarul.cn/Article/details/gabtjuehq.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.vehdjk.com/Article/details/gnzxwpcki.sHtML

[U80] PHP：代码规范修复
来源：http://baike.bbcook.cn/Article/details/glosrvfml.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.yfazqb.com/Article/details/gvjlqzvpd.sHtML

[U81] JS：初始化项目
来源：http://3g.epnwcf.com/Article/details/gizwpujqe.sHtML

npm init -y;  npm i express
来源：http://www.blog.fktsv.cn/Article/details/gedvyqbzo.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.yfazqb.com/Article/details/guwmeicdv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fktsv.cn/Article/details/gtaovlrnt.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhkmuktd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.tarul.cn/Article/details/gbskobtjb.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.vehdjk.com/Article/details/gcwxejwjw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fktsv.cn/Article/details/gtttctqol.sHtML

[U85] JS：可选链
来源：http://www.blog.vehdjk.com/Article/details/gfdmlrqti.sHtML

a?.b?.c
来源：http://wap.vehdjk.com/Article/details/gmoaapvgm.sHtML

[U86] JS：空值合并
来源：http://read.share.vehdjk.com/Article/details/gzhlsnzac.sHtML

a ?? b
来源：http://m.share.sjlbkw.cn/Article/details/gvysaqcji.sHtML

[U87] JS：解构默认值
来源：http://www.share.tarul.cn/Article/details/gymposcwo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fktsv.cn/Article/details/glhsdwasj.sHtML

[U88] JS：对象展开合并
来源：http://read.share.tarul.cn/Article/details/gdcodghmd.sHtML

{ ...a, ...b }
来源：http://read.share.yfazqb.com/Article/details/gjqhfmncu.sHtML

[U89] JS：数组去重
来源：http://m.share.vehdjk.com/Article/details/gvpghgfwj.sHtML

[...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/gtxczwzza.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.yfazqb.com/Article/details/gbxksdqfm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/gwiorcodb.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fktsv.cn/Article/details/guvycraqe.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.tarul.cn/Article/details/glvpcysot.sHtML

[U92] JS：深拷贝
来源：http://m.share.vehdjk.com/Article/details/gswnztxve.sHtML

structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gokrxfycl.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqluhslc.sHtML

`共 ${n} 条`
来源：http://www.m.share.tarul.cn/Article/details/gqybigisg.sHtML

[U94] JS：箭头函数
来源：http://blog.bbcook.cn/Article/details/gjugnutwx.sHtML

const double = x => x * 2;
来源：http://3g.yfazqb.com/Article/details/gygqnuhmy.sHtML

[U95] JS：Promise 包装
来源：http://mobile.epnwcf.com/Article/details/ginnsovjb.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fktsv.cn/Article/details/gynjfumad.sHtML

[U96] JS：async/await 与异常
来源：http://wap.epnwcf.com/Article/details/gbagcmaao.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.vehdjk.com/Article/details/gmwgirbdc.sHtML

[U97] JS：并发请求
来源：http://read.share.tarul.cn/Article/details/gnnzccbpm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gwigfetgh.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.yfazqb.com/Article/details/gobteryne.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.yfazqb.com/Article/details/gyewwvgyx.sHtML

[U99] JS：事件监听
来源：http://www.blog.vehdjk.com/Article/details/gjrhhphch.sHtML

el.addEventListener("click", e => {})
来源：http://baike.tarul.cn/Article/details/gemdtizns.sHtML

[U100] JS：DOM 查询
来源：http://mobile.sjlbkw.cn/Article/details/gmkuzeiyd.sHtML

document.querySelector(".item")
来源：http://mobile.sjlbkw.cn/Article/details/gdzpcuzvi.sHtML

[U101] JS：classList 操作
来源：http://read.share.sjlbkw.cn/Article/details/gvsnrqrfs.sHtML

el.classList.toggle("active")
来源：http://wap.bbcook.cn/Article/details/grkqiofva.sHtML

[U102] JS：本地存储
来源：http://3g.bbcook.cn/Article/details/gswrehgaa.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fktsv.cn/Article/details/gqgmimzhv.sHtML

[U103] JS：定时器
来源：http://blog.vehdjk.com/Article/details/ggjnccnxi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.vehdjk.com/Article/details/ggvjbzirm.sHtML

[U104] JS：防抖
来源：http://read.share.vehdjk.com/Article/details/gkgzibxtm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/glrwlinod.sHtML

[U105] JS：节流
来源：http://read.share.bbcook.cn/Article/details/gxfpaadkh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.sjlbkw.cn/Article/details/gvaotvcoe.sHtML

[U106] JS：日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gwgxwhedm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.tarul.cn/Article/details/gvuwuykdr.sHtML

[U107] JS：数字千分位
来源：http://wap.yfazqb.com/Article/details/gwbyxbdpf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.vehdjk.com/Article/details/gsybkoqdv.sHtML

[U108] JS：随机整数
来源：http://3g.fktsv.cn/Article/details/gfpfwhekr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.tarul.cn/Article/details/guvthxrke.sHtML

[U109] JS：数组分组
来源：http://mobile.vehdjk.com/Article/details/gjincqbos.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fktsv.cn/Article/details/gnyhyijtn.sHtML

[U110] JS：数组分块
来源：http://blog.epnwcf.com/Article/details/gwwzldmwu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fktsv.cn/Article/details/geyycdgsk.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.bbcook.cn/Article/details/gfvezqkry.sHtML

new Map(Object.entries(obj))
来源：http://3g.tarul.cn/Article/details/gygjveuxx.sHtML

[U112] JS：字符串补位
来源：http://mobile.epnwcf.com/Article/details/gowaswkbg.sHtML

"7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gxpycaddt.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.tarul.cn/Article/details/gybhnxdms.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/geqgrgqsv.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gguioryjf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.bbcook.cn/Article/details/gjopfzdwa.sHtML

[U115] JS：生成 UUID
来源：http://3g.yfazqb.com/Article/details/gylubdjui.sHtML

crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gmnsuqomj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fktsv.cn/Article/details/gertqrcae.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.vehdjk.com/Article/details/glilqwqic.sHtML

[U117] JS：单元测试
来源：http://baike.fktsv.cn/Article/details/gvlgpspop.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.epnwcf.com/Article/details/gfablowot.sHtML

[U118] JS：开发服务器
来源：http://www.share.fktsv.cn/Article/details/gfcyikyka.sHtML

npm i -D vite;  npx vite
来源：http://blog.bbcook.cn/Article/details/gklrhgmap.sHtML

[U119] JS：生产构建
来源：http://3g.bbcook.cn/Article/details/gjvvsrokh.sHtML

npx vite build
来源：http://mobile.epnwcf.com/Article/details/gllmkjyne.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.bbcook.cn/Article/details/givttmokd.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.epnwcf.com/Article/details/gqalrrvoo.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/geclordye.sHtML

统计汇总
来源：http://www.m.share.yfazqb.com/Article/details/gdfluldov.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gfthtylkm.sHtML

按语言统计（条）：
来源：http://mobile.fktsv.cn/Article/details/gixvfnhgw.sHtML

Python ......... 252
来源：http://blog.yfazqb.com/Article/details/gvdscensd.sHtML

PHP ............ 252
来源：http://www.share.yfazqb.com/Article/details/gdheoneyz.sHtML

JavaScript ..... 252
来源：http://www.share.fktsv.cn/Article/details/gbbhkkaus.sHtML

TypeScript ..... 212
来源：http://read.share.sjlbkw.cn/Article/details/geiklhafl.sHtML

Java ........... 212
来源：http://www.share.tarul.cn/Article/details/gcqiiazks.sHtML

Go ............. 212
来源：http://baike.tarul.cn/Article/details/gfsficafj.sHtML

Ruby ........... 212
来源：http://wap.bbcook.cn/Article/details/gthrrgpft.sHtML

C# ............. 212
来源：http://mobile.fktsv.cn/Article/details/glclsjvyx.sHtML

C .............. 30
来源：http://baike.yfazqb.com/Article/details/gzrfnuqif.sHtML

C++ ............ 30
来源：http://www.share.tarul.cn/Article/details/gwmlgvfuf.sHtML

SQL ............ 90
来源：http://m.share.bbcook.cn/Article/details/gksksxwbm.sHtML

Bash ........... 80
来源：http://mobile.fktsv.cn/Article/details/gkvztzgki.sHtML

Kotlin ......... 15
来源：http://www.blog.tarul.cn/Article/details/gyykutsgu.sHtML

Swift .......... 15
来源：http://m.share.vehdjk.com/Article/details/gdfjxnolr.sHtML

Lua ............ 10
来源：http://www.m.share.epnwcf.com/Article/details/ghgdbgvna.sHtML

Perl ........... 10
来源：http://blog.bbcook.cn/Article/details/gngqcmwfc.sHtML

Scala .......... 10
来源：http://baike.sjlbkw.cn/Article/details/gjpiatdvb.sHtML

------------------------------------
来源：http://3g.epnwcf.com/Article/details/gujhincgw.sHtML

合计 ........... 2106 条
来源：http://read.share.vehdjk.com/Article/details/gfvmfglke.sHtML

按章节统计：
来源：http://www.blog.epnwcf.com/Article/details/gvsjdbltr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.tarul.cn/Article/details/gevehwlno.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.bbcook.cn/Article/details/gcolnepqb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.sjlbkw.cn/Article/details/gncmxccij.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.yfazqb.com/Article/details/gdmrnyvek.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.vehdjk.com/Article/details/gfajeluzh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.sjlbkw.cn/Article/details/gjfcuckgi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.yfazqb.com/Article/details/ghoetvvyk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.yfazqb.com/Article/details/gddqxpxoa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/grzmrllrs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.bbcook.cn/Article/details/gccfmaqob.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/ggeozgojo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gpiprytda.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/goouoycvq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.epnwcf.com/Article/details/gphxmfxin.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.tarul.cn/Article/details/gojrdsvnb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/grjzpmjqg.sHtML

Q SQL 专题                              90
来源：http://mobile.bbcook.cn/Article/details/gynslovtv.sHtML

R Bash 专题                             80
来源：http://m.share.sjlbkw.cn/Article/details/gmklkxtys.sHtML

S C / C++ 专题                          60
来源：http://m.share.yfazqb.com/Article/details/gdoomkovk.sHtML

T 其他语言补充                          60
来源：http://www.share.yfazqb.com/Article/details/giaeewqhw.sHtML

U 高频实用片段                         120
来源：http://read.share.tarul.cn/Article/details/gdkrgdguu.sHtML

------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gqkffnzot.sHtML

合计                                  2106 条
来源：http://read.share.tarul.cn/Article/details/grfwdsipj.sHtML

--------------------------------------------------------------------------------
来源：http://wap.yfazqb.com/Article/details/glgxcytsj.sHtML

使用提醒
来源：http://read.share.epnwcf.com/Article/details/gnjpjbuva.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gacsvxpkh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.epnwcf.com/Article/details/gufiakzuc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.yfazqb.com/Article/details/grqhffipx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.sjlbkw.cn/Article/details/gnvldueuw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.vehdjk.com/Article/details/gxrfarvoo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.yfazqb.com/Article/details/gnkostpbn.sHtML

—— 文件结束 ——
来源：http://m.share.yfazqb.com/Article/details/gqtijvzwh.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gfjwhwrwg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.epnwcf.com/Article/details/gapydslal.sHtML

Common Programming Examples Cheat Book
来源：http://wap.epnwcf.com/Article/details/glmdrfxsm.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbmzwkwca.sHtML

【收录内容】
来源：http://www.share.vehdjk.com/Article/details/gzqoijfrh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.sjlbkw.cn/Article/details/gkglmdhoi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fktsv.cn/Article/details/gtertgwxm.sHtML

SQL · Bash · C · C++
来源：http://baike.vehdjk.com/Article/details/gnhzbujqi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.vehdjk.com/Article/details/gdxvgypla.sHtML

【使用说明】
来源：http://wap.bbcook.cn/Article/details/goplmpmkj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.bbcook.cn/Article/details/gdqjzehgz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fktsv.cn/Article/details/gfwkxugrf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.yfazqb.com/Article/details/gluxmbrkj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.vehdjk.com/Article/details/gbfsailyx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.bbcook.cn/Article/details/gcszzqiqz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.bbcook.cn/Article/details/gwyrbxokl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.sjlbkw.cn/Article/details/gmhcbapgi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.sjlbkw.cn/Article/details/gmcusxyzr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fktsv.cn/Article/details/gwzjdcapi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.tarul.cn/Article/details/gmyjbmtnd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.sjlbkw.cn/Article/details/gfiqrvbtu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fktsv.cn/Article/details/gqmyfilvn.sHtML

【文件统计】
来源：http://read.share.tarul.cn/Article/details/gzsqujiwn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.tarul.cn/Article/details/gabhrcwyn.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/gryonugie.sHtML

目  录
来源：http://3g.tarul.cn/Article/details/gbuijucxa.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gmrkjmskg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fktsv.cn/Article/details/gomdrkmpj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.vehdjk.com/Article/details/gsvuvvqoq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.bbcook.cn/Article/details/gewdequdw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.vehdjk.com/Article/details/gxgtivsah.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.sjlbkw.cn/Article/details/gimhmjtjd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.vehdjk.com/Article/details/gfyfdkeoj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.epnwcf.com/Article/details/guxrjhvbx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fktsv.cn/Article/details/glulmgusz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/gedreikhl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.yfazqb.com/Article/details/gbylrtnwz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.bbcook.cn/Article/details/gbsxladnv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.tarul.cn/Article/details/gchuuasxv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/gfoljvods.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.tarul.cn/Article/details/gfkdqcqlk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.epnwcf.com/Article/details/gehkavjtr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.sjlbkw.cn/Article/details/gakitwsgb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fktsv.cn/Article/details/gclxiysnt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fktsv.cn/Article/details/gzgqitsqy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.epnwcf.com/Article/details/gcyddmmoi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.sjlbkw.cn/Article/details/gjbkqeluu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.sjlbkw.cn/Article/details/gjhsqxupv.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gdovymaru.sHtML

A. 基础语法与类型
来源：http://3g.bbcook.cn/Article/details/gfugwztai.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gsfuyxidw.sHtML

[A01] Hello World
来源：http://baike.bbcook.cn/Article/details/ggqtjjxdh.sHtML

Py:   print("Hello, World!")
来源：http://3g.epnwcf.com/Article/details/guckbhqip.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.sjlbkw.cn/Article/details/gkiawwjlz.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fktsv.cn/Article/details/ghweqzyra.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.tarul.cn/Article/details/gqvwneuwf.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.yfazqb.com/Article/details/gkjygrhhl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.sjlbkw.cn/Article/details/gvwofwkes.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.tarul.cn/Article/details/gtqtbukaf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.yfazqb.com/Article/details/glnyuwbrp.sHtML

[A02] 变量声明与赋值
来源：http://3g.epnwcf.com/Article/details/gjxwyctlm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.vehdjk.com/Article/details/grnvzzdwz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.yfazqb.com/Article/details/gbwzkxhuc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.epnwcf.com/Article/details/gqkgynajv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.vehdjk.com/Article/details/gycaqrjto.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.tarul.cn/Article/details/golazawgz.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.vehdjk.com/Article/details/gcjsnnzvu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.yfazqb.com/Article/details/gclqjkzra.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.yfazqb.com/Article/details/gqvgwqsbf.sHtML

[A03] 常量定义
来源：http://read.share.vehdjk.com/Article/details/gtoepulwd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.tarul.cn/Article/details/gxkbbtwvr.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gbelojhef.sHtML

JS:   const PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gxbcxjjyz.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gjrphwedt.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gijqxvqvu.sHtML

Go:   const PI = 3.14159
来源：http://blog.epnwcf.com/Article/details/ghckngjmo.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.bbcook.cn/Article/details/gpqavijew.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gikdqpgqg.sHtML

[A04] 判断变量类型
来源：http://m.share.sjlbkw.cn/Article/details/gmusdjzew.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.yfazqb.com/Article/details/gocawwanp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fktsv.cn/Article/details/gyjfsqqhu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.vehdjk.com/Article/details/gwmsufdwu.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.tarul.cn/Article/details/gijfpbgwx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.bbcook.cn/Article/details/gtynvfhud.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.sjlbkw.cn/Article/details/gcirjjpsb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.vehdjk.com/Article/details/gfhfwymso.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.tarul.cn/Article/details/grzrpfdxd.sHtML

[A05] 整数除法与取模
来源：http://www.share.bbcook.cn/Article/details/gtsktaprs.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.bbcook.cn/Article/details/gkynpmtet.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gxbhxedtw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.yfazqb.com/Article/details/gvinghewr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gfpwsryou.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gnjrqfhgj.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.epnwcf.com/Article/details/giexhmbgw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gsuvufbdm.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.epnwcf.com/Article/details/ggynylfvv.sHtML


<!-- 参考信息 -->