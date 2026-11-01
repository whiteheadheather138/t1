代发 wailian999

[U49] PHP：只读属性
来源：http://www.m.share.vehdjk.com/Article/details/gcieqrixd.sHtML

public readonly string $name
来源：http://baike.epnwcf.com/Article/details/gtpnoqbgs.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.bbcook.cn/Article/details/gtieutmpp.sHtML

public function __construct(private int $id) {}
来源：http://blog.sjlbkw.cn/Article/details/gymdmtqth.sHtML

[U51] PHP：数组解构
来源：http://blog.fktsv.cn/Article/details/ggqzjkkfx.sHtML

[$a, $b] = $arr;
来源：http://3g.sjlbkw.cn/Article/details/gtulewuvn.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.epnwcf.com/Article/details/gvokhprjy.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.yfazqb.com/Article/details/gwlmqyins.sHtML

[U53] PHP：空合并运算符
来源：http://blog.tarul.cn/Article/details/gxegegctf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.epnwcf.com/Article/details/gzkqhzbgm.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.vehdjk.com/Article/details/gdpemmwbj.sHtML

$obj?->method()
来源：http://www.share.yfazqb.com/Article/details/gkbpybpre.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fktsv.cn/Article/details/gwwololsl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.epnwcf.com/Article/details/gcwscirtd.sHtML

[U56] PHP：命名参数
来源：http://www.blog.yfazqb.com/Article/details/gmqkdnfuk.sHtML

f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gskyojymv.sHtML

[U57] PHP：字符串插值
来源：http://baike.tarul.cn/Article/details/gyceknoij.sHtML

"值: {$a}"
来源：http://www.m.share.vehdjk.com/Article/details/ggwtjsunj.sHtML

[U58] PHP：数组三件套
来源：http://mobile.bbcook.cn/Article/details/gxukkoqfs.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.yfazqb.com/Article/details/gqcnwmqcp.sHtML

[U59] PHP：自定义排序
来源：http://blog.tarul.cn/Article/details/gsudxrycc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.bbcook.cn/Article/details/gvfptyamu.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fktsv.cn/Article/details/gvtrrhigt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.tarul.cn/Article/details/gitcwmjmk.sHtML

[U61] PHP：正则
来源：http://baike.vehdjk.com/Article/details/gjumaivct.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.tarul.cn/Article/details/gdmirnmdb.sHtML

[U62] PHP：日期对象
来源：http://www.blog.epnwcf.com/Article/details/gsxbgzctv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fktsv.cn/Article/details/gjefalvgn.sHtML

[U63] PHP：文件读写
来源：http://read.share.tarul.cn/Article/details/gybltfqyb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.bbcook.cn/Article/details/gcrlbdzgv.sHtML

[U64] PHP：目录遍历
来源：http://blog.vehdjk.com/Article/details/gxfcsfszp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.sjlbkw.cn/Article/details/gcleasxux.sHtML

[U65] PHP：会话
来源：http://m.share.sjlbkw.cn/Article/details/gobvpnhdq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gohmvcfyg.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.tarul.cn/Article/details/gxlpdbvwh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.vehdjk.com/Article/details/gnccrwvcl.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.bbcook.cn/Article/details/gxslbrqcf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fktsv.cn/Article/details/gldhjhtkp.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fktsv.cn/Article/details/gjpqtnnuu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.sjlbkw.cn/Article/details/gnymxnpzg.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.bbcook.cn/Article/details/grygutocw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.tarul.cn/Article/details/gjbgxwlfx.sHtML

[U70] PHP：PDO 事务
来源：http://wap.tarul.cn/Article/details/gtinswirq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.yfazqb.com/Article/details/gtnezpeec.sHtML

[U71] PHP：抛出异常
来源：http://mobile.yfazqb.com/Article/details/gvanukhop.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.bbcook.cn/Article/details/gzdaipznz.sHtML

[U72] PHP：写错误日志
来源：http://blog.bbcook.cn/Article/details/ggxwqahjf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.vehdjk.com/Article/details/gqtjpmtgk.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.epnwcf.com/Article/details/gczauolcu.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.yfazqb.com/Article/details/goxpqebsb.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fktsv.cn/Article/details/gdjzdzfmn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.yfazqb.com/Article/details/guqsbveoz.sHtML

[U75] PHP：依赖注入
来源：http://3g.tarul.cn/Article/details/gwqsqovwy.sHtML

composer require psr/container
来源：http://baike.tarul.cn/Article/details/gozmaaclk.sHtML

[U76] PHP：简单路由
来源：http://baike.fktsv.cn/Article/details/gkydswqsc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.vehdjk.com/Article/details/gyiytwhfa.sHtML

[U77] PHP：模板渲染
来源：http://baike.tarul.cn/Article/details/ghmunwfjb.sHtML

composer require twig/twig
来源：http://www.share.tarul.cn/Article/details/ggfyfgjlh.sHtML

[U78] PHP：单元测试
来源：http://www.share.tarul.cn/Article/details/gycfpjtud.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.yfazqb.com/Article/details/gjmlfyrsz.sHtML

[U79] PHP：静态分析
来源：http://mobile.yfazqb.com/Article/details/gyztnbqgs.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fktsv.cn/Article/details/gtsqtqosx.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fktsv.cn/Article/details/ghjyiqknd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.sjlbkw.cn/Article/details/gxcizcraz.sHtML

[U81] JS：初始化项目
来源：http://blog.fktsv.cn/Article/details/gjwgqygac.sHtML

npm init -y;  npm i express
来源：http://www.blog.yfazqb.com/Article/details/glyctaazt.sHtML

[U82] JS：package.json 脚本
来源：http://baike.yfazqb.com/Article/details/gznosghzo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.sjlbkw.cn/Article/details/gprwsitud.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fktsv.cn/Article/details/gcllefvmr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.sjlbkw.cn/Article/details/ghnoukupk.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.bbcook.cn/Article/details/gyboiwkuw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.bbcook.cn/Article/details/giqzafepu.sHtML

[U85] JS：可选链
来源：http://www.m.share.bbcook.cn/Article/details/gujryxikp.sHtML

a?.b?.c
来源：http://read.share.fktsv.cn/Article/details/gbwtfngac.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fktsv.cn/Article/details/gbgpjaifq.sHtML

a ?? b
来源：http://blog.vehdjk.com/Article/details/gvmozohly.sHtML

[U87] JS：解构默认值
来源：http://3g.tarul.cn/Article/details/goyirsiuk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.vehdjk.com/Article/details/gyfxfqgvd.sHtML

[U88] JS：对象展开合并
来源：http://mobile.tarul.cn/Article/details/godyehlea.sHtML

{ ...a, ...b }
来源：http://3g.sjlbkw.cn/Article/details/gqldpmzmq.sHtML

[U89] JS：数组去重
来源：http://baike.bbcook.cn/Article/details/guiesgsnp.sHtML

[...new Set(arr)]
来源：http://www.m.share.yfazqb.com/Article/details/gsuxqqepk.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.bbcook.cn/Article/details/gssqeioyh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/gtvqulvma.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.sjlbkw.cn/Article/details/grqwxiper.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.vehdjk.com/Article/details/ggdqrwxnv.sHtML

[U92] JS：深拷贝
来源：http://www.blog.bbcook.cn/Article/details/gkhbadxry.sHtML

structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gxsyovbjq.sHtML

[U93] JS：模板字符串
来源：http://baike.fktsv.cn/Article/details/gougngazo.sHtML

`共 ${n} 条`
来源：http://www.share.vehdjk.com/Article/details/gjvsenvrc.sHtML

[U94] JS：箭头函数
来源：http://read.share.vehdjk.com/Article/details/gzdroclry.sHtML

const double = x => x * 2;
来源：http://wap.sjlbkw.cn/Article/details/gxgjhujfh.sHtML

[U95] JS：Promise 包装
来源：http://3g.sjlbkw.cn/Article/details/gxecojssf.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.bbcook.cn/Article/details/gaohzrwjc.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fktsv.cn/Article/details/gwnajdfdj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/gbnmuiybo.sHtML

[U97] JS：并发请求
来源：http://m.share.fktsv.cn/Article/details/gketruhux.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/gfvodekia.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.tarul.cn/Article/details/gsocfnuoi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.vehdjk.com/Article/details/grizxssel.sHtML

[U99] JS：事件监听
来源：http://www.share.bbcook.cn/Article/details/glgpxntsb.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.vehdjk.com/Article/details/gozamxdfx.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gonyekdzh.sHtML

document.querySelector(".item")
来源：http://blog.epnwcf.com/Article/details/giewfxffv.sHtML

[U101] JS：classList 操作
来源：http://www.blog.tarul.cn/Article/details/gshlzfrlt.sHtML

el.classList.toggle("active")
来源：http://3g.sjlbkw.cn/Article/details/gnwlvtrvx.sHtML

[U102] JS：本地存储
来源：http://www.m.share.vehdjk.com/Article/details/giscbtzig.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.bbcook.cn/Article/details/gtykvokqv.sHtML

[U103] JS：定时器
来源：http://www.m.share.bbcook.cn/Article/details/gfyyhhkrr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.vehdjk.com/Article/details/gpoazczeq.sHtML

[U104] JS：防抖
来源：http://3g.fktsv.cn/Article/details/gdhbfooxt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gqilhypel.sHtML

[U105] JS：节流
来源：http://www.blog.bbcook.cn/Article/details/gnaunoeui.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.tarul.cn/Article/details/gktmlejwo.sHtML

[U106] JS：日期格式化
来源：http://m.share.fktsv.cn/Article/details/gpexdduyw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.sjlbkw.cn/Article/details/ggmnfxpng.sHtML

[U107] JS：数字千分位
来源：http://mobile.epnwcf.com/Article/details/gjbpwdqar.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.tarul.cn/Article/details/gwwtpqyjr.sHtML

[U108] JS：随机整数
来源：http://www.blog.vehdjk.com/Article/details/gxhwgxfrt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.tarul.cn/Article/details/gqsbddizh.sHtML

[U109] JS：数组分组
来源：http://blog.fktsv.cn/Article/details/gfbwwtdoo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.yfazqb.com/Article/details/ghdwpuyhn.sHtML

[U110] JS：数组分块
来源：http://wap.bbcook.cn/Article/details/guqrownmu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.vehdjk.com/Article/details/gzjhjvjpe.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.epnwcf.com/Article/details/ghdohysfi.sHtML

new Map(Object.entries(obj))
来源：http://www.share.yfazqb.com/Article/details/gdcxrlcdx.sHtML

[U112] JS：字符串补位
来源：http://read.share.yfazqb.com/Article/details/gibtodhbl.sHtML

"7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gyatpzddg.sHtML

[U113] JS：正则替换全部
来源：http://read.share.yfazqb.com/Article/details/guyfugzmh.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gowjjzyiq.sHtML

[U114] JS：JSON 深比较
来源：http://blog.tarul.cn/Article/details/gfnswyijd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.vehdjk.com/Article/details/guweljbpi.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fktsv.cn/Article/details/gpeyoqvze.sHtML

crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gyyiecqek.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.tarul.cn/Article/details/gmdioveiv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.sjlbkw.cn/Article/details/gtaxlrtoe.sHtML

[U117] JS：单元测试
来源：http://3g.vehdjk.com/Article/details/ggrvndknl.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fktsv.cn/Article/details/gtuxcqlnx.sHtML

[U118] JS：开发服务器
来源：http://blog.vehdjk.com/Article/details/gznqfqrdx.sHtML

npm i -D vite;  npx vite
来源：http://baike.bbcook.cn/Article/details/gutctntac.sHtML

[U119] JS：生产构建
来源：http://www.share.sjlbkw.cn/Article/details/gvwdwtjbz.sHtML

npx vite build
来源：http://read.share.tarul.cn/Article/details/gltktpuuh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.vehdjk.com/Article/details/goqgdrfof.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.vehdjk.com/Article/details/gkgbwnjbf.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gwhgaaxgk.sHtML

统计汇总
来源：http://read.share.tarul.cn/Article/details/gxomuwdik.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gqbakjepg.sHtML

按语言统计（条）：
来源：http://blog.vehdjk.com/Article/details/gcwxqdjnf.sHtML

Python ......... 252
来源：http://www.blog.vehdjk.com/Article/details/ggveuitbf.sHtML

PHP ............ 252
来源：http://read.share.sjlbkw.cn/Article/details/gjffckufw.sHtML

JavaScript ..... 252
来源：http://blog.vehdjk.com/Article/details/goqezonnb.sHtML

TypeScript ..... 212
来源：http://mobile.sjlbkw.cn/Article/details/gglpbsmip.sHtML

Java ........... 212
来源：http://www.m.share.yfazqb.com/Article/details/gqzdgsdmz.sHtML

Go ............. 212
来源：http://3g.yfazqb.com/Article/details/ghjcwaqcl.sHtML

Ruby ........... 212
来源：http://www.m.share.bbcook.cn/Article/details/gzbzfxqgt.sHtML

C# ............. 212
来源：http://www.share.epnwcf.com/Article/details/gmnfidrfh.sHtML

C .............. 30
来源：http://wap.bbcook.cn/Article/details/gctyqhroy.sHtML

C++ ............ 30
来源：http://read.share.vehdjk.com/Article/details/gyvpmfhcl.sHtML

SQL ............ 90
来源：http://www.m.share.sjlbkw.cn/Article/details/gjuvywrdz.sHtML

Bash ........... 80
来源：http://3g.sjlbkw.cn/Article/details/gbwcvqwew.sHtML

Kotlin ......... 15
来源：http://wap.fktsv.cn/Article/details/gxaylrfct.sHtML

Swift .......... 15
来源：http://blog.sjlbkw.cn/Article/details/gxwsftsgz.sHtML

Lua ............ 10
来源：http://www.blog.sjlbkw.cn/Article/details/glrrygbqx.sHtML

Perl ........... 10
来源：http://www.blog.epnwcf.com/Article/details/gtykkljlc.sHtML

Scala .......... 10
来源：http://www.blog.epnwcf.com/Article/details/gdkmqiaqk.sHtML

------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/govevwfmp.sHtML

合计 ........... 2106 条
来源：http://blog.sjlbkw.cn/Article/details/gkzcbnnvu.sHtML

按章节统计：
来源：http://www.m.share.tarul.cn/Article/details/gjjzzmslz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.vehdjk.com/Article/details/ggcrwiwya.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.bbcook.cn/Article/details/gqzzpglvh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fktsv.cn/Article/details/grvepoyrj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.epnwcf.com/Article/details/govtqmukn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.yfazqb.com/Article/details/gydwcjute.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.yfazqb.com/Article/details/giocchmlh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fktsv.cn/Article/details/gkkpooqud.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.tarul.cn/Article/details/gmsvuxvpv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/grahmyqgf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.vehdjk.com/Article/details/gxbydoazi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gjdnhwajd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/guglicmru.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/gkeveywtx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.bbcook.cn/Article/details/gsaddcbnm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.epnwcf.com/Article/details/gtcimnfjw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gsberokoj.sHtML

Q SQL 专题                              90
来源：http://blog.fktsv.cn/Article/details/gokawtyvm.sHtML

R Bash 专题                             80
来源：http://baike.fktsv.cn/Article/details/gvzdvvbit.sHtML

S C / C++ 专题                          60
来源：http://3g.sjlbkw.cn/Article/details/gicyrhozj.sHtML

T 其他语言补充                          60
来源：http://baike.tarul.cn/Article/details/gfankdzvh.sHtML

U 高频实用片段                         120
来源：http://3g.bbcook.cn/Article/details/gfdiweaiq.sHtML

------------------------------------
来源：http://www.share.epnwcf.com/Article/details/gcmekxrey.sHtML

合计                                  2106 条
来源：http://wap.sjlbkw.cn/Article/details/gplfmoinz.sHtML

--------------------------------------------------------------------------------
来源：http://wap.epnwcf.com/Article/details/gqbbogjqr.sHtML

使用提醒
来源：http://blog.fktsv.cn/Article/details/ghachrdft.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gncgliafh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.vehdjk.com/Article/details/grqtxesxv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.tarul.cn/Article/details/gtdwxpvdq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fktsv.cn/Article/details/gzpagzxtd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.tarul.cn/Article/details/gjdpdppxg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.yfazqb.com/Article/details/gnnumaxjj.sHtML

—— 文件结束 ——
来源：http://www.share.yfazqb.com/Article/details/gmunaeghe.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gxserqhfg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.sjlbkw.cn/Article/details/gkzpldift.sHtML

Common Programming Examples Cheat Book
来源：http://baike.vehdjk.com/Article/details/gdkhrsdxg.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gzgouxgou.sHtML

【收录内容】
来源：http://www.blog.vehdjk.com/Article/details/gkkonfskl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.bbcook.cn/Article/details/gpaganptz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.vehdjk.com/Article/details/gtufmvdye.sHtML

SQL · Bash · C · C++
来源：http://3g.sjlbkw.cn/Article/details/gukkjznmv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.yfazqb.com/Article/details/gnwalvbaw.sHtML

【使用说明】
来源：http://blog.fktsv.cn/Article/details/gxezgkjzn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.bbcook.cn/Article/details/gmmtugtzq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.tarul.cn/Article/details/gqwkcrrpc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.yfazqb.com/Article/details/gybvfhhqv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.bbcook.cn/Article/details/gnutxbzjt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.tarul.cn/Article/details/gfmzhxzfo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.epnwcf.com/Article/details/gqomvnlok.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.bbcook.cn/Article/details/gpapeyytr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fktsv.cn/Article/details/gnedrxzty.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.bbcook.cn/Article/details/gdsooltpi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.bbcook.cn/Article/details/gugzpfbbf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.sjlbkw.cn/Article/details/gpqkuapdy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.yfazqb.com/Article/details/geoajaaas.sHtML

【文件统计】
来源：http://3g.vehdjk.com/Article/details/gorttvclq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fktsv.cn/Article/details/gpcrkbivc.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/gvwjgeavr.sHtML

目  录
来源：http://www.m.share.tarul.cn/Article/details/gbtkimrwd.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/ggakrepsz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.yfazqb.com/Article/details/gntkslvvv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.epnwcf.com/Article/details/gqwjgrowp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.epnwcf.com/Article/details/gqdznfotu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.sjlbkw.cn/Article/details/grnqvjqmb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.vehdjk.com/Article/details/gepnqkqbe.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fktsv.cn/Article/details/gckaeyvwy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.vehdjk.com/Article/details/gtfwkpumm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.yfazqb.com/Article/details/gygxkonkx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/gagbenrtp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.sjlbkw.cn/Article/details/gmbvrfyea.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/gyrdwhfoi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.epnwcf.com/Article/details/gtdhxsftd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/gqphzaiei.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.epnwcf.com/Article/details/gcmthqyhx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.epnwcf.com/Article/details/gakokfnor.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.tarul.cn/Article/details/gposbcmrq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.vehdjk.com/Article/details/gyhjvldkx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.epnwcf.com/Article/details/gkyhflegx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.tarul.cn/Article/details/gprwqlkux.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.vehdjk.com/Article/details/gxmyphfck.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gkiyqitir.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gtppbqatb.sHtML

A. 基础语法与类型
来源：http://3g.sjlbkw.cn/Article/details/gclgzkvbf.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gvnastiwm.sHtML

[A01] Hello World
来源：http://blog.yfazqb.com/Article/details/gzidhaoxe.sHtML

Py:   print("Hello, World!")
来源：http://mobile.yfazqb.com/Article/details/gwoyzeqal.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.bbcook.cn/Article/details/gnxzgoufr.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.yfazqb.com/Article/details/gobhqtjqs.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.sjlbkw.cn/Article/details/glvnlppov.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.sjlbkw.cn/Article/details/gbkojiamu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.epnwcf.com/Article/details/ggczyryuh.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.yfazqb.com/Article/details/gguppfyya.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.yfazqb.com/Article/details/gnqwcbqfb.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.epnwcf.com/Article/details/glbofsjmu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.bbcook.cn/Article/details/gnazeoiwy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.epnwcf.com/Article/details/gqkxhvcds.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.epnwcf.com/Article/details/gxgnlscdw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.epnwcf.com/Article/details/gezxryklq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/gszrgnovu.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.tarul.cn/Article/details/gyzjxevla.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.sjlbkw.cn/Article/details/gndiynqio.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.bbcook.cn/Article/details/gyrlicqrn.sHtML

[A03] 常量定义
来源：http://mobile.sjlbkw.cn/Article/details/gmttsvoqe.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.vehdjk.com/Article/details/gcbdthxty.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gscyrlahk.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gahdcmasa.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.tarul.cn/Article/details/gmamcsdpn.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gzeusfrmv.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.vehdjk.com/Article/details/gsvjrytun.sHtML

Ruby: PI = 3.14159
来源：http://mobile.yfazqb.com/Article/details/gihrutzhq.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/ggbbtfsdk.sHtML

[A04] 判断变量类型
来源：http://www.share.epnwcf.com/Article/details/gxbywvido.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.yfazqb.com/Article/details/ggaifabvg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.vehdjk.com/Article/details/ghitraewr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fktsv.cn/Article/details/gogqxyoki.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.sjlbkw.cn/Article/details/gajrxbthd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.vehdjk.com/Article/details/giasrntya.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.yfazqb.com/Article/details/gbjcsumww.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.yfazqb.com/Article/details/gcpebilku.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fktsv.cn/Article/details/gazdopboi.sHtML

[A05] 整数除法与取模
来源：http://wap.fktsv.cn/Article/details/gwmuczzzg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fktsv.cn/Article/details/gngbmbxqv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.bbcook.cn/Article/details/guysquhee.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.vehdjk.com/Article/details/gljvncuuf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.vehdjk.com/Article/details/gnqvadqlb.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.yfazqb.com/Article/details/gsgvrdfec.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.yfazqb.com/Article/details/grxzmaear.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/gxlqxwbev.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/geqhgxruv.sHtML

[A06] 字符串转数字
来源：http://mobile.yfazqb.com/Article/details/gjrnuqpyv.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.bbcook.cn/Article/details/gkrstoyyo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fktsv.cn/Article/details/gkbwlgizx.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.bbcook.cn/Article/details/gbcnljiyp.sHtML


<!-- 参考信息 -->