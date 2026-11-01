代发 wailian999

[U43] PHP：声明命名空间
来源：http://wap.yfazqb.com/Article/details/gljezllcy.sHtML

namespace App\Http;
来源：http://read.share.vehdjk.com/Article/details/gxxaewzom.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fktsv.cn/Article/details/gaiutwjqx.sHtML

declare(strict_types=1);
来源：http://baike.tarul.cn/Article/details/gnzcvwewh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.vehdjk.com/Article/details/gryzlggvb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/giksruoil.sHtML

[U46] PHP：可空类型
来源：http://www.share.tarul.cn/Article/details/gjlwvgied.sHtML

?string $name = null
来源：http://www.blog.epnwcf.com/Article/details/gjqdqszsf.sHtML

[U47] PHP：联合类型
来源：http://3g.vehdjk.com/Article/details/gwnwlqehk.sHtML

int|string $id
来源：http://3g.yfazqb.com/Article/details/gwjgfuzed.sHtML

[U48] PHP：纯枚举
来源：http://mobile.tarul.cn/Article/details/gpsykfznl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.sjlbkw.cn/Article/details/ggryyampj.sHtML

[U49] PHP：只读属性
来源：http://wap.tarul.cn/Article/details/gdwqdkdlp.sHtML

public readonly string $name
来源：http://blog.tarul.cn/Article/details/gjupxjonh.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.epnwcf.com/Article/details/gmdarrxfa.sHtML

public function __construct(private int $id) {}
来源：http://wap.sjlbkw.cn/Article/details/gotrzbwhl.sHtML

[U51] PHP：数组解构
来源：http://3g.epnwcf.com/Article/details/gtgvadzbp.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fktsv.cn/Article/details/gbkjxwsjr.sHtML

[U52] PHP：箭头函数
来源：http://read.share.bbcook.cn/Article/details/gsjaiwpqt.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.yfazqb.com/Article/details/grxttbuyu.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.bbcook.cn/Article/details/gynyuspcc.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.vehdjk.com/Article/details/goctrkshy.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.vehdjk.com/Article/details/gqzampfjs.sHtML

$obj?->method()
来源：http://read.share.bbcook.cn/Article/details/gzjmimwzq.sHtML

[U55] PHP：match 表达式
来源：http://wap.vehdjk.com/Article/details/gwyuvafij.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.tarul.cn/Article/details/gntmvuhbm.sHtML

[U56] PHP：命名参数
来源：http://www.share.yfazqb.com/Article/details/gcusdztsu.sHtML

f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/ghzeztycg.sHtML

[U57] PHP：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gsnrgoriw.sHtML

"值: {$a}"
来源：http://read.share.yfazqb.com/Article/details/gyshbhrqk.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fktsv.cn/Article/details/ghmaykbnt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.tarul.cn/Article/details/gogagyriu.sHtML

[U59] PHP：自定义排序
来源：http://baike.yfazqb.com/Article/details/gvocawjhc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.sjlbkw.cn/Article/details/gdkgtbrkl.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fktsv.cn/Article/details/gzogkqkhc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.yfazqb.com/Article/details/ghybfvzqo.sHtML

[U61] PHP：正则
来源：http://wap.tarul.cn/Article/details/gcmrqhycm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.sjlbkw.cn/Article/details/ghlwiknpd.sHtML

[U62] PHP：日期对象
来源：http://www.share.bbcook.cn/Article/details/ghwncvvuy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.bbcook.cn/Article/details/gdcdaxuzc.sHtML

[U63] PHP：文件读写
来源：http://3g.bbcook.cn/Article/details/gdwjyrpig.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.epnwcf.com/Article/details/gfnapgbzq.sHtML

[U64] PHP：目录遍历
来源：http://3g.epnwcf.com/Article/details/grkgyddlx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.sjlbkw.cn/Article/details/gzskezsnm.sHtML

[U65] PHP：会话
来源：http://www.share.vehdjk.com/Article/details/guzpwzacg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gydinankk.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.sjlbkw.cn/Article/details/gtdqaflpc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.vehdjk.com/Article/details/gbdfvlmhh.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.tarul.cn/Article/details/geegowrah.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.tarul.cn/Article/details/glaojmlax.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.yfazqb.com/Article/details/ghynlslqe.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.epnwcf.com/Article/details/gvxhsuxty.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.vehdjk.com/Article/details/glvzzzbgs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.epnwcf.com/Article/details/gtvqgtkxp.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.vehdjk.com/Article/details/gbiioynhu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.yfazqb.com/Article/details/gymogjqmg.sHtML

[U71] PHP：抛出异常
来源：http://read.share.vehdjk.com/Article/details/gyubugmkl.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.vehdjk.com/Article/details/gouzggvzk.sHtML

[U72] PHP：写错误日志
来源：http://read.share.tarul.cn/Article/details/gtidzunga.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.tarul.cn/Article/details/gpfiytnza.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fktsv.cn/Article/details/glomlefxd.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.epnwcf.com/Article/details/gfcjcfxjz.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.vehdjk.com/Article/details/gqceedzxk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.tarul.cn/Article/details/gexwvubho.sHtML

[U75] PHP：依赖注入
来源：http://m.share.epnwcf.com/Article/details/ginqxidef.sHtML

composer require psr/container
来源：http://wap.bbcook.cn/Article/details/ghtrtanre.sHtML

[U76] PHP：简单路由
来源：http://mobile.fktsv.cn/Article/details/gmzcxalzt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.vehdjk.com/Article/details/gpdmbxpaz.sHtML

[U77] PHP：模板渲染
来源：http://www.share.sjlbkw.cn/Article/details/gwibyxpfv.sHtML

composer require twig/twig
来源：http://m.share.bbcook.cn/Article/details/ghmyylzxr.sHtML

[U78] PHP：单元测试
来源：http://wap.epnwcf.com/Article/details/gbeaciybf.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.epnwcf.com/Article/details/gctbqpcom.sHtML

[U79] PHP：静态分析
来源：http://read.share.fktsv.cn/Article/details/gaqzicbgo.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.bbcook.cn/Article/details/gofbgrepw.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.epnwcf.com/Article/details/gmsaekyhu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.tarul.cn/Article/details/grvhprefd.sHtML

[U81] JS：初始化项目
来源：http://mobile.sjlbkw.cn/Article/details/gjcavadmn.sHtML

npm init -y;  npm i express
来源：http://3g.sjlbkw.cn/Article/details/gtujtxqpr.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.epnwcf.com/Article/details/gjeeulnqw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.sjlbkw.cn/Article/details/glsarqupc.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.sjlbkw.cn/Article/details/gsxeozwfm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fktsv.cn/Article/details/gulbbxjkh.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.bbcook.cn/Article/details/gfvrzjobf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.sjlbkw.cn/Article/details/gganibgyu.sHtML

[U85] JS：可选链
来源：http://www.blog.yfazqb.com/Article/details/gkcnturxn.sHtML

a?.b?.c
来源：http://www.blog.sjlbkw.cn/Article/details/gqllmhtpn.sHtML

[U86] JS：空值合并
来源：http://wap.vehdjk.com/Article/details/glaufnxdd.sHtML

a ?? b
来源：http://www.share.bbcook.cn/Article/details/gtnplutbm.sHtML

[U87] JS：解构默认值
来源：http://blog.tarul.cn/Article/details/gzognmhmv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fktsv.cn/Article/details/gpprrsvas.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.bbcook.cn/Article/details/glyspxhum.sHtML

{ ...a, ...b }
来源：http://read.share.fktsv.cn/Article/details/gltctvjch.sHtML

[U89] JS：数组去重
来源：http://3g.fktsv.cn/Article/details/gxdhvuucv.sHtML

[...new Set(arr)]
来源：http://www.blog.vehdjk.com/Article/details/gmqbupqsq.sHtML

[U90] JS：数字数组排序
来源：http://m.share.epnwcf.com/Article/details/gzqmarzpu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gdbuuppbe.sHtML

[U91] JS：对象键值遍历
来源：http://blog.vehdjk.com/Article/details/gbvakmdqr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fktsv.cn/Article/details/gkuvgwndx.sHtML

[U92] JS：深拷贝
来源：http://3g.sjlbkw.cn/Article/details/gjjfhvmfr.sHtML

structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/gjdccrunx.sHtML

[U93] JS：模板字符串
来源：http://m.share.sjlbkw.cn/Article/details/gzmztbopr.sHtML

`共 ${n} 条`
来源：http://m.share.tarul.cn/Article/details/gjmqvapks.sHtML

[U94] JS：箭头函数
来源：http://mobile.vehdjk.com/Article/details/gimsettui.sHtML

const double = x => x * 2;
来源：http://www.blog.fktsv.cn/Article/details/gcefapjqf.sHtML

[U95] JS：Promise 包装
来源：http://wap.yfazqb.com/Article/details/gliyovmqr.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fktsv.cn/Article/details/gtyotkljl.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.epnwcf.com/Article/details/gmmukedld.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gpxhbdcrp.sHtML

[U97] JS：并发请求
来源：http://www.share.sjlbkw.cn/Article/details/gasqisjfi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/ghsgkwhos.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.epnwcf.com/Article/details/gpbpnxpdq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fktsv.cn/Article/details/gcyebggks.sHtML

[U99] JS：事件监听
来源：http://3g.vehdjk.com/Article/details/gvyubcxnd.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fktsv.cn/Article/details/gpbwhqhvr.sHtML

[U100] JS：DOM 查询
来源：http://mobile.sjlbkw.cn/Article/details/gsxihhjdx.sHtML

document.querySelector(".item")
来源：http://blog.sjlbkw.cn/Article/details/ggyzdogks.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.tarul.cn/Article/details/ghigjpogk.sHtML

el.classList.toggle("active")
来源：http://read.share.tarul.cn/Article/details/gkqxyphhr.sHtML

[U102] JS：本地存储
来源：http://mobile.tarul.cn/Article/details/gyfurhqdb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.bbcook.cn/Article/details/gyzramtai.sHtML

[U103] JS：定时器
来源：http://m.share.epnwcf.com/Article/details/gwzmesrif.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.sjlbkw.cn/Article/details/ghnsfccdc.sHtML

[U104] JS：防抖
来源：http://blog.sjlbkw.cn/Article/details/gmagklyyz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gmdyccumi.sHtML

[U105] JS：节流
来源：http://wap.sjlbkw.cn/Article/details/gfumgtdjl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.vehdjk.com/Article/details/gwodrwssb.sHtML

[U106] JS：日期格式化
来源：http://wap.bbcook.cn/Article/details/gsupkyffn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.bbcook.cn/Article/details/guosmkduo.sHtML

[U107] JS：数字千分位
来源：http://read.share.fktsv.cn/Article/details/gyyhpgxip.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.sjlbkw.cn/Article/details/ggtoreoik.sHtML

[U108] JS：随机整数
来源：http://www.share.fktsv.cn/Article/details/goxcljyob.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.yfazqb.com/Article/details/ghodybycy.sHtML

[U109] JS：数组分组
来源：http://m.share.yfazqb.com/Article/details/gzqdobsbw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.epnwcf.com/Article/details/gblkswqpc.sHtML

[U110] JS：数组分块
来源：http://read.share.tarul.cn/Article/details/gmjaqqczt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.tarul.cn/Article/details/gishgglnh.sHtML

[U111] JS：对象转 Map
来源：http://mobile.bbcook.cn/Article/details/ghieoazfo.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.bbcook.cn/Article/details/gyzatulpb.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.yfazqb.com/Article/details/gpvaiqgys.sHtML

"7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gfuwvwwjp.sHtML

[U113] JS：正则替换全部
来源：http://baike.vehdjk.com/Article/details/gsmytvuak.sHtML

s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gorpowdsl.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.epnwcf.com/Article/details/gdcpimson.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.vehdjk.com/Article/details/glalqtrdb.sHtML

[U115] JS：生成 UUID
来源：http://wap.fktsv.cn/Article/details/gufipppct.sHtML

crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/gygfqeeyy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.vehdjk.com/Article/details/gjkdzuatb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.tarul.cn/Article/details/geqeadltq.sHtML

[U117] JS：单元测试
来源：http://www.share.epnwcf.com/Article/details/gwsgceaxs.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.tarul.cn/Article/details/ggbmxvjyh.sHtML

[U118] JS：开发服务器
来源：http://read.share.fktsv.cn/Article/details/ghhtmdxbj.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.bbcook.cn/Article/details/gmdvuddrm.sHtML

[U119] JS：生产构建
来源：http://read.share.epnwcf.com/Article/details/gzqakoizk.sHtML

npx vite build
来源：http://3g.yfazqb.com/Article/details/gecnqhfxf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.vehdjk.com/Article/details/ghbpfthmf.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.tarul.cn/Article/details/gzgbhdosh.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/grjkjoplg.sHtML

统计汇总
来源：http://www.m.share.yfazqb.com/Article/details/gltcgbyau.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ggbvwmrmp.sHtML

按语言统计（条）：
来源：http://m.share.fktsv.cn/Article/details/grnltwzcz.sHtML

Python ......... 252
来源：http://m.share.yfazqb.com/Article/details/gknhmkocc.sHtML

PHP ............ 252
来源：http://www.m.share.tarul.cn/Article/details/gchcutidq.sHtML

JavaScript ..... 252
来源：http://blog.sjlbkw.cn/Article/details/gmfdyyzap.sHtML

TypeScript ..... 212
来源：http://m.share.yfazqb.com/Article/details/giiazjbqt.sHtML

Java ........... 212
来源：http://blog.vehdjk.com/Article/details/gygbyvsxq.sHtML

Go ............. 212
来源：http://m.share.tarul.cn/Article/details/goqgzrawr.sHtML

Ruby ........... 212
来源：http://3g.tarul.cn/Article/details/guluafquh.sHtML

C# ............. 212
来源：http://m.share.bbcook.cn/Article/details/gmhqfvrjr.sHtML

C .............. 30
来源：http://mobile.epnwcf.com/Article/details/gxzjroowa.sHtML

C++ ............ 30
来源：http://3g.epnwcf.com/Article/details/gdxhtygev.sHtML

SQL ............ 90
来源：http://baike.sjlbkw.cn/Article/details/gxcxavhzy.sHtML

Bash ........... 80
来源：http://www.share.yfazqb.com/Article/details/giyackqtr.sHtML

Kotlin ......... 15
来源：http://www.share.epnwcf.com/Article/details/gsjpbapol.sHtML

Swift .......... 15
来源：http://mobile.tarul.cn/Article/details/gqupktexx.sHtML

Lua ............ 10
来源：http://www.blog.tarul.cn/Article/details/gtoarsida.sHtML

Perl ........... 10
来源：http://read.share.fktsv.cn/Article/details/gvjfzgyjn.sHtML

Scala .......... 10
来源：http://baike.tarul.cn/Article/details/gidsyipvp.sHtML

------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/grdzxlkbv.sHtML

合计 ........... 2106 条
来源：http://read.share.fktsv.cn/Article/details/gazjmufsf.sHtML

按章节统计：
来源：http://www.share.bbcook.cn/Article/details/gjdszyumm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fktsv.cn/Article/details/glzojxdtq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.vehdjk.com/Article/details/gtwtzjmcj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.bbcook.cn/Article/details/gqmlqblca.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.sjlbkw.cn/Article/details/gzanjromj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.bbcook.cn/Article/details/guzjjrpuf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.tarul.cn/Article/details/garckqpxc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.sjlbkw.cn/Article/details/gdjzgrqgg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.bbcook.cn/Article/details/gjqrjwcgr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gzlcgarbo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.sjlbkw.cn/Article/details/ghiythfrn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gyadwczrl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gpudwqbtm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/gvqkzwemp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.vehdjk.com/Article/details/gpkecblss.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.bbcook.cn/Article/details/gzcbbllyw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/gjvczhdob.sHtML

Q SQL 专题                              90
来源：http://www.m.share.bbcook.cn/Article/details/gqwuvbvos.sHtML

R Bash 专题                             80
来源：http://wap.yfazqb.com/Article/details/gtwzzhrqu.sHtML

S C / C++ 专题                          60
来源：http://wap.bbcook.cn/Article/details/gqtigunfh.sHtML

T 其他语言补充                          60
来源：http://baike.yfazqb.com/Article/details/gzdrucdga.sHtML

U 高频实用片段                         120
来源：http://wap.sjlbkw.cn/Article/details/gzrurjlwq.sHtML

------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gccdreckc.sHtML

合计                                  2106 条
来源：http://baike.sjlbkw.cn/Article/details/gywylzlum.sHtML

--------------------------------------------------------------------------------
来源：http://wap.epnwcf.com/Article/details/ggsoajwwa.sHtML

使用提醒
来源：http://m.share.epnwcf.com/Article/details/gkrhocshx.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.tarul.cn/Article/details/gatiexxvz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.bbcook.cn/Article/details/gipurkgtu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.vehdjk.com/Article/details/gqkdviisb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.vehdjk.com/Article/details/gkplhpfgf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.epnwcf.com/Article/details/gvgbnkorr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.yfazqb.com/Article/details/gseonyvuc.sHtML

—— 文件结束 ——
来源：http://3g.sjlbkw.cn/Article/details/gbcnmhpaa.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gxxrtjvan.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.yfazqb.com/Article/details/gefhkwymg.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.yfazqb.com/Article/details/gzsdytuyi.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gfubygnoc.sHtML

【收录内容】
来源：http://blog.epnwcf.com/Article/details/gyxbmqahe.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fktsv.cn/Article/details/gykceaajg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fktsv.cn/Article/details/gxktqepmm.sHtML

SQL · Bash · C · C++
来源：http://www.blog.bbcook.cn/Article/details/gsltgtrlc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.bbcook.cn/Article/details/gfxlejvdj.sHtML

【使用说明】
来源：http://3g.tarul.cn/Article/details/gtdvojwrb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fktsv.cn/Article/details/gzutcuxeo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.vehdjk.com/Article/details/gfdmoewhv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.tarul.cn/Article/details/gswtqdkbm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.vehdjk.com/Article/details/gdubwodsu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.vehdjk.com/Article/details/ghtthlase.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.sjlbkw.cn/Article/details/guwovhirt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.sjlbkw.cn/Article/details/gxhawxtsy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.bbcook.cn/Article/details/gzqdpajii.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.epnwcf.com/Article/details/gvhvhlfat.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.sjlbkw.cn/Article/details/gjskruxod.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.yfazqb.com/Article/details/gtvtqwsmv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.epnwcf.com/Article/details/ginlueppa.sHtML

【文件统计】
来源：http://m.share.vehdjk.com/Article/details/gdiomitsd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.sjlbkw.cn/Article/details/gqdbrqoyv.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/ghwiedrxb.sHtML

目  录
来源：http://3g.sjlbkw.cn/Article/details/gsjrxkyeh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.epnwcf.com/Article/details/gcbhnwefn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fktsv.cn/Article/details/gnbzjehgo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.vehdjk.com/Article/details/glkdmqksp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.epnwcf.com/Article/details/glagoynbs.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fktsv.cn/Article/details/gwrpujzxg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.epnwcf.com/Article/details/glqpofykj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.epnwcf.com/Article/details/gtsfaezod.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.bbcook.cn/Article/details/gmkihxpla.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.vehdjk.com/Article/details/gesevgfta.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.epnwcf.com/Article/details/gzudgqhxu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.tarul.cn/Article/details/gkiwpzkbc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.yfazqb.com/Article/details/gdurqrclt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.epnwcf.com/Article/details/ggoczyida.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gnlgalklo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.bbcook.cn/Article/details/gbnorokbe.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.tarul.cn/Article/details/gcwwfytrf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.vehdjk.com/Article/details/gfcjyzaxn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.yfazqb.com/Article/details/gztvimict.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.yfazqb.com/Article/details/gdobhgmkm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.yfazqb.com/Article/details/ghtoceykj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fktsv.cn/Article/details/gphsukpjg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fktsv.cn/Article/details/gdqsdifiz.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/guxusqzrf.sHtML

A. 基础语法与类型
来源：http://wap.yfazqb.com/Article/details/gxlnjaarz.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gjmxdjrvu.sHtML

[A01] Hello World
来源：http://blog.fktsv.cn/Article/details/gictbkexh.sHtML

Py:   print("Hello, World!")
来源：http://baike.yfazqb.com/Article/details/gkrolfide.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.yfazqb.com/Article/details/gwzteqfva.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fktsv.cn/Article/details/gbhjtwfqt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fktsv.cn/Article/details/gqurxjuvd.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.vehdjk.com/Article/details/glbarwxen.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fktsv.cn/Article/details/gzmllumav.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.sjlbkw.cn/Article/details/grcesxcij.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.epnwcf.com/Article/details/giytegqjs.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fktsv.cn/Article/details/gnmgifjut.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.epnwcf.com/Article/details/gbpjmyfhp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.bbcook.cn/Article/details/ghkikwwnk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.vehdjk.com/Article/details/gswefqozr.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.epnwcf.com/Article/details/gpwllpbom.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.sjlbkw.cn/Article/details/gfmqpncat.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.epnwcf.com/Article/details/gwwopaane.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.epnwcf.com/Article/details/ggpqtvodm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.sjlbkw.cn/Article/details/glolvkaku.sHtML

[A03] 常量定义
来源：http://www.blog.sjlbkw.cn/Article/details/gyqclzdcr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.tarul.cn/Article/details/gdulokcoa.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gtwxfdctc.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/giyswocpn.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/glkazhkcb.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gpqsmbobg.sHtML

Go:   const PI = 3.14159
来源：http://3g.sjlbkw.cn/Article/details/gnjedauaa.sHtML

Ruby: PI = 3.14159
来源：http://m.share.vehdjk.com/Article/details/gyztfpqta.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gvjhjdgig.sHtML

[A04] 判断变量类型
来源：http://www.m.share.vehdjk.com/Article/details/gwoqtkdrh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.bbcook.cn/Article/details/gtiskdftc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fktsv.cn/Article/details/gfvyxzwnb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.vehdjk.com/Article/details/goxgaiprs.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.sjlbkw.cn/Article/details/gitkhmdvd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fktsv.cn/Article/details/gejlenkea.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.tarul.cn/Article/details/gyirumxja.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fktsv.cn/Article/details/gfpptlgxl.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.yfazqb.com/Article/details/gmkeenqgi.sHtML

[A05] 整数除法与取模
来源：http://mobile.bbcook.cn/Article/details/gioflihli.sHtML


<!-- 参考信息 -->