代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://baike.tarul.cn/Article/details/gzsvhldcx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/gspkkzxwe.sHtML

[U46] PHP：可空类型
来源：http://www.share.sjlbkw.cn/Article/details/gtddgnyjs.sHtML

?string $name = null
来源：http://www.share.sjlbkw.cn/Article/details/gjbgffcva.sHtML

[U47] PHP：联合类型
来源：http://baike.bbcook.cn/Article/details/gekbkvbbv.sHtML

int|string $id
来源：http://3g.yfazqb.com/Article/details/gxdbhwpme.sHtML

[U48] PHP：纯枚举
来源：http://3g.bbcook.cn/Article/details/gvxhmeddo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.sjlbkw.cn/Article/details/gooccbvnh.sHtML

[U49] PHP：只读属性
来源：http://baike.epnwcf.com/Article/details/gdisemizk.sHtML

public readonly string $name
来源：http://blog.tarul.cn/Article/details/glohljwjz.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.vehdjk.com/Article/details/gdpcoxesg.sHtML

public function __construct(private int $id) {}
来源：http://mobile.bbcook.cn/Article/details/gmvkvcqms.sHtML

[U51] PHP：数组解构
来源：http://wap.tarul.cn/Article/details/gftayecba.sHtML

[$a, $b] = $arr;
来源：http://m.share.sjlbkw.cn/Article/details/gzetjejpn.sHtML

[U52] PHP：箭头函数
来源：http://www.share.epnwcf.com/Article/details/gyaqxcwol.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.sjlbkw.cn/Article/details/gsyebbfsg.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.tarul.cn/Article/details/ghzwcffcs.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.vehdjk.com/Article/details/gjghskyxr.sHtML

[U54] PHP：空安全调用
来源：http://baike.fktsv.cn/Article/details/gkgkqbeco.sHtML

$obj?->method()
来源：http://www.blog.epnwcf.com/Article/details/glurfmhtk.sHtML

[U55] PHP：match 表达式
来源：http://m.share.vehdjk.com/Article/details/gjygcmihl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.sjlbkw.cn/Article/details/gtlegrotu.sHtML

[U56] PHP：命名参数
来源：http://mobile.bbcook.cn/Article/details/gslzwmcab.sHtML

f(a: 1, b: 2)
来源：http://3g.fktsv.cn/Article/details/gkqwfkatj.sHtML

[U57] PHP：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gpthuqntz.sHtML

"值: {$a}"
来源：http://www.m.share.fktsv.cn/Article/details/gmfcancbk.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.yfazqb.com/Article/details/gveaevalz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gpwbcpxpl.sHtML

[U59] PHP：自定义排序
来源：http://3g.epnwcf.com/Article/details/gzuevwjsm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.vehdjk.com/Article/details/gvikwfizw.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.tarul.cn/Article/details/gmbybdmcu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.tarul.cn/Article/details/gxzvoxiii.sHtML

[U61] PHP：正则
来源：http://blog.epnwcf.com/Article/details/grozluiry.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.vehdjk.com/Article/details/gvglvnmng.sHtML

[U62] PHP：日期对象
来源：http://wap.yfazqb.com/Article/details/gkzwrihjz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.epnwcf.com/Article/details/gnwehkncb.sHtML

[U63] PHP：文件读写
来源：http://m.share.fktsv.cn/Article/details/gmtianuom.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.sjlbkw.cn/Article/details/gighjwbnt.sHtML

[U64] PHP：目录遍历
来源：http://www.share.epnwcf.com/Article/details/gschzqlot.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fktsv.cn/Article/details/gscdtvspw.sHtML

[U65] PHP：会话
来源：http://blog.bbcook.cn/Article/details/guifqprvw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fktsv.cn/Article/details/goidppzfx.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.yfazqb.com/Article/details/gcrgysfus.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.tarul.cn/Article/details/grpygphnj.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fktsv.cn/Article/details/gcdhjplhc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fktsv.cn/Article/details/gmejdrbcw.sHtML

[U68] PHP：PDO 连接
来源：http://wap.sjlbkw.cn/Article/details/genffqbff.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.bbcook.cn/Article/details/gjhqdmdox.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.bbcook.cn/Article/details/gzkaxycwg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.tarul.cn/Article/details/gyrvldqgi.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fktsv.cn/Article/details/grjlevgmq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.tarul.cn/Article/details/gxmpvvyvh.sHtML

[U71] PHP：抛出异常
来源：http://3g.sjlbkw.cn/Article/details/grjqlxslm.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fktsv.cn/Article/details/gbyrmlqqs.sHtML

[U72] PHP：写错误日志
来源：http://read.share.bbcook.cn/Article/details/girznrwbd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.sjlbkw.cn/Article/details/gkuikonah.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fktsv.cn/Article/details/gjcbmvilz.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.tarul.cn/Article/details/gmldinwyl.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.yfazqb.com/Article/details/gxkksgzto.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.bbcook.cn/Article/details/gwblmjhzf.sHtML

[U75] PHP：依赖注入
来源：http://baike.tarul.cn/Article/details/gygywacad.sHtML

composer require psr/container
来源：http://www.blog.epnwcf.com/Article/details/gfcpghvmb.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.vehdjk.com/Article/details/gvfjscbgn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fktsv.cn/Article/details/grisxjfsy.sHtML

[U77] PHP：模板渲染
来源：http://mobile.epnwcf.com/Article/details/gkuhmprlz.sHtML

composer require twig/twig
来源：http://m.share.tarul.cn/Article/details/gpdhytmlb.sHtML

[U78] PHP：单元测试
来源：http://read.share.fktsv.cn/Article/details/gjhptaiyi.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.vehdjk.com/Article/details/gmemxtdas.sHtML

[U79] PHP：静态分析
来源：http://mobile.sjlbkw.cn/Article/details/gfsrnsgyt.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.epnwcf.com/Article/details/glbxuwtfw.sHtML

[U80] PHP：代码规范修复
来源：http://blog.sjlbkw.cn/Article/details/gqohbeaoj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.vehdjk.com/Article/details/gpyxtdgfw.sHtML

[U81] JS：初始化项目
来源：http://3g.bbcook.cn/Article/details/gloustmer.sHtML

npm init -y;  npm i express
来源：http://mobile.tarul.cn/Article/details/gtzvxdbfx.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.vehdjk.com/Article/details/gaqaqfuyi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.tarul.cn/Article/details/gluhxudtx.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.vehdjk.com/Article/details/gjxqgfdbk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.vehdjk.com/Article/details/gdppybcjl.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.tarul.cn/Article/details/gfetgfivl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fktsv.cn/Article/details/gyaizbyzj.sHtML

[U85] JS：可选链
来源：http://www.blog.bbcook.cn/Article/details/guhdmpmct.sHtML

a?.b?.c
来源：http://3g.epnwcf.com/Article/details/glzwgrjip.sHtML

[U86] JS：空值合并
来源：http://read.share.yfazqb.com/Article/details/gjvshcena.sHtML

a ?? b
来源：http://baike.epnwcf.com/Article/details/gzfqtzwhg.sHtML

[U87] JS：解构默认值
来源：http://blog.sjlbkw.cn/Article/details/giqnocabr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.epnwcf.com/Article/details/gaegyxbit.sHtML

[U88] JS：对象展开合并
来源：http://mobile.bbcook.cn/Article/details/gqtncqxrv.sHtML

{ ...a, ...b }
来源：http://m.share.tarul.cn/Article/details/gryfrgnpj.sHtML

[U89] JS：数组去重
来源：http://mobile.bbcook.cn/Article/details/gmcsoqxzl.sHtML

[...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/ghhmueyhj.sHtML

[U90] JS：数字数组排序
来源：http://blog.sjlbkw.cn/Article/details/grmjiqekm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/gczglqszk.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fktsv.cn/Article/details/gvpieaqbv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.bbcook.cn/Article/details/gvomeezzo.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.yfazqb.com/Article/details/gzxfqbfal.sHtML

structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/guyeounwi.sHtML

[U93] JS：模板字符串
来源：http://mobile.yfazqb.com/Article/details/guvimuzdg.sHtML

`共 ${n} 条`
来源：http://www.share.tarul.cn/Article/details/gtjrqzjbf.sHtML

[U94] JS：箭头函数
来源：http://www.blog.sjlbkw.cn/Article/details/guzazedvr.sHtML

const double = x => x * 2;
来源：http://www.share.tarul.cn/Article/details/gkahrahhr.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.bbcook.cn/Article/details/gsgsdoklf.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.vehdjk.com/Article/details/gmcvvcarc.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.bbcook.cn/Article/details/glwrunkec.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmkgcazn.sHtML

[U97] JS：并发请求
来源：http://www.blog.vehdjk.com/Article/details/gdfoibvjk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/gqigqfula.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fktsv.cn/Article/details/gtngdtktz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.vehdjk.com/Article/details/gplhuvbqk.sHtML

[U99] JS：事件监听
来源：http://www.share.tarul.cn/Article/details/gffeapzif.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fktsv.cn/Article/details/geifaftbe.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.tarul.cn/Article/details/ghzxbfxeu.sHtML

document.querySelector(".item")
来源：http://www.share.tarul.cn/Article/details/gkgsedybb.sHtML

[U101] JS：classList 操作
来源：http://read.share.epnwcf.com/Article/details/gvgnpgigz.sHtML

el.classList.toggle("active")
来源：http://m.share.tarul.cn/Article/details/ghgmlfftp.sHtML

[U102] JS：本地存储
来源：http://www.share.tarul.cn/Article/details/gwkqmjlxk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.tarul.cn/Article/details/gnqsiduhd.sHtML

[U103] JS：定时器
来源：http://baike.tarul.cn/Article/details/gmasiymle.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.bbcook.cn/Article/details/gwaioakry.sHtML

[U104] JS：防抖
来源：http://blog.yfazqb.com/Article/details/ggdiviajm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/giaxhzwze.sHtML

[U105] JS：节流
来源：http://www.blog.yfazqb.com/Article/details/glzqsugbm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.epnwcf.com/Article/details/grmfmcliu.sHtML

[U106] JS：日期格式化
来源：http://www.share.tarul.cn/Article/details/gqvyhqflh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.tarul.cn/Article/details/gpftyokhv.sHtML

[U107] JS：数字千分位
来源：http://blog.yfazqb.com/Article/details/gfpxfbclc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.epnwcf.com/Article/details/gldeqgyla.sHtML

[U108] JS：随机整数
来源：http://mobile.vehdjk.com/Article/details/gyetgzycr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.sjlbkw.cn/Article/details/glrqlkdpp.sHtML

[U109] JS：数组分组
来源：http://www.blog.vehdjk.com/Article/details/gzfbxeudo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.epnwcf.com/Article/details/gfycmgdcq.sHtML

[U110] JS：数组分块
来源：http://www.share.yfazqb.com/Article/details/galyehaor.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.epnwcf.com/Article/details/gamobqivh.sHtML

[U111] JS：对象转 Map
来源：http://www.share.sjlbkw.cn/Article/details/gltagntdi.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.epnwcf.com/Article/details/gdrtcgxgy.sHtML

[U112] JS：字符串补位
来源：http://baike.sjlbkw.cn/Article/details/guysdebrg.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/glkxrtfwg.sHtML

[U113] JS：正则替换全部
来源：http://blog.vehdjk.com/Article/details/gwynprfyw.sHtML

s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gcbztqrdk.sHtML

[U114] JS：JSON 深比较
来源：http://3g.bbcook.cn/Article/details/gvfvrxont.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.vehdjk.com/Article/details/gcwoquvze.sHtML

[U115] JS：生成 UUID
来源：http://blog.yfazqb.com/Article/details/gfnmpnqcf.sHtML

crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gpwsjeole.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.yfazqb.com/Article/details/gfylogima.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gvprzxgjx.sHtML

[U117] JS：单元测试
来源：http://www.blog.epnwcf.com/Article/details/gxcisbpmc.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.yfazqb.com/Article/details/gshaaljho.sHtML

[U118] JS：开发服务器
来源：http://blog.bbcook.cn/Article/details/gdskshspg.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.yfazqb.com/Article/details/gfpkyewaz.sHtML

[U119] JS：生产构建
来源：http://www.blog.fktsv.cn/Article/details/gfxhflgni.sHtML

npx vite build
来源：http://m.share.bbcook.cn/Article/details/gbwwulyla.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.yfazqb.com/Article/details/gmueqcotm.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.bbcook.cn/Article/details/gmggujtto.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gsflkmaub.sHtML

统计汇总
来源：http://www.blog.bbcook.cn/Article/details/goubkqbhs.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqtlpjqz.sHtML

按语言统计（条）：
来源：http://read.share.vehdjk.com/Article/details/gmpjlnrny.sHtML

Python ......... 252
来源：http://m.share.yfazqb.com/Article/details/gyjoogdkl.sHtML

PHP ............ 252
来源：http://m.share.bbcook.cn/Article/details/gegpnzupo.sHtML

JavaScript ..... 252
来源：http://baike.tarul.cn/Article/details/gcgncitjs.sHtML

TypeScript ..... 212
来源：http://m.share.sjlbkw.cn/Article/details/gretdekha.sHtML

Java ........... 212
来源：http://www.share.bbcook.cn/Article/details/gqqxrsxng.sHtML

Go ............. 212
来源：http://m.share.bbcook.cn/Article/details/gwuvpcasc.sHtML

Ruby ........... 212
来源：http://m.share.bbcook.cn/Article/details/gxjktwinz.sHtML

C# ............. 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gztqnfakx.sHtML

C .............. 30
来源：http://www.m.share.epnwcf.com/Article/details/giqmdffow.sHtML

C++ ............ 30
来源：http://www.share.fktsv.cn/Article/details/gjpyzzlsr.sHtML

SQL ............ 90
来源：http://blog.sjlbkw.cn/Article/details/gjmwgcqkw.sHtML

Bash ........... 80
来源：http://wap.bbcook.cn/Article/details/gnwwipbal.sHtML

Kotlin ......... 15
来源：http://www.blog.tarul.cn/Article/details/gjougqqdw.sHtML

Swift .......... 15
来源：http://www.share.bbcook.cn/Article/details/gfzimaaha.sHtML

Lua ............ 10
来源：http://www.m.share.fktsv.cn/Article/details/glwzfrrcz.sHtML

Perl ........... 10
来源：http://www.m.share.epnwcf.com/Article/details/gropifrwc.sHtML

Scala .......... 10
来源：http://3g.fktsv.cn/Article/details/gclbttcfm.sHtML

------------------------------------
来源：http://blog.fktsv.cn/Article/details/gfmfmetip.sHtML

合计 ........... 2106 条
来源：http://blog.sjlbkw.cn/Article/details/gxwimzgjc.sHtML

按章节统计：
来源：http://www.share.fktsv.cn/Article/details/gjiqzturw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.yfazqb.com/Article/details/gdfxsmlfp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.bbcook.cn/Article/details/gohqeybys.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.tarul.cn/Article/details/ghbqcyqrd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.epnwcf.com/Article/details/gblurgzud.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.epnwcf.com/Article/details/gblxxivrw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.yfazqb.com/Article/details/gazeusfpb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fktsv.cn/Article/details/gabrwikqk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.bbcook.cn/Article/details/gsdzxycim.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gvgppwpdl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fktsv.cn/Article/details/govkbzcrs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/ginhqgtca.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gryxbfwjs.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gnlafkmtn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.sjlbkw.cn/Article/details/glhsunzwk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvsculum.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gzjawfmex.sHtML

Q SQL 专题                              90
来源：http://mobile.vehdjk.com/Article/details/gnfxegmzb.sHtML

R Bash 专题                             80
来源：http://m.share.vehdjk.com/Article/details/gmxvwkxjk.sHtML

S C / C++ 专题                          60
来源：http://mobile.epnwcf.com/Article/details/gtghwwiqu.sHtML

T 其他语言补充                          60
来源：http://3g.fktsv.cn/Article/details/gkoscdlbp.sHtML

U 高频实用片段                         120
来源：http://read.share.yfazqb.com/Article/details/gyuslaerp.sHtML

------------------------------------
来源：http://3g.bbcook.cn/Article/details/gzzhcdmyy.sHtML

合计                                  2106 条
来源：http://www.share.fktsv.cn/Article/details/ghzuixfbg.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fktsv.cn/Article/details/gyvoueher.sHtML

使用提醒
来源：http://mobile.tarul.cn/Article/details/gofwycrxu.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.vehdjk.com/Article/details/gqhdnznio.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.yfazqb.com/Article/details/gfhothpqx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.sjlbkw.cn/Article/details/gfycbnvyw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.sjlbkw.cn/Article/details/gvqsqdadd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fktsv.cn/Article/details/gawzkkudz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.yfazqb.com/Article/details/gvqunoxrm.sHtML

—— 文件结束 ——
来源：http://www.share.vehdjk.com/Article/details/glhzyrdhh.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gttgaglca.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fktsv.cn/Article/details/gbcwefdix.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.epnwcf.com/Article/details/gexdxsbet.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gvkjzbgox.sHtML

【收录内容】
来源：http://mobile.vehdjk.com/Article/details/gazgcpoqx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.epnwcf.com/Article/details/gcagoiydo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.epnwcf.com/Article/details/ghebbrdaw.sHtML

SQL · Bash · C · C++
来源：http://mobile.sjlbkw.cn/Article/details/gdvegstbp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.bbcook.cn/Article/details/gnjpqnlrb.sHtML

【使用说明】
来源：http://www.m.share.vehdjk.com/Article/details/gtemexnqx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.epnwcf.com/Article/details/giscfzhdy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.sjlbkw.cn/Article/details/grurclaln.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.epnwcf.com/Article/details/gevyohqai.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.epnwcf.com/Article/details/gndchsxnx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.epnwcf.com/Article/details/grrbpsuef.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.vehdjk.com/Article/details/gdwmmrzqx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.sjlbkw.cn/Article/details/gsgfrhgdt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.vehdjk.com/Article/details/gvxyzdyba.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.vehdjk.com/Article/details/grgyowhus.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.sjlbkw.cn/Article/details/gldoaspns.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.vehdjk.com/Article/details/gimbpddvv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.bbcook.cn/Article/details/gzlvzkgfj.sHtML

【文件统计】
来源：http://baike.epnwcf.com/Article/details/gyeotpmqb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fktsv.cn/Article/details/gpfgeavih.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gfwiyvolm.sHtML

目  录
来源：http://3g.epnwcf.com/Article/details/giiwevdud.sHtML

--------------------------------------------------------------------------------
来源：http://3g.yfazqb.com/Article/details/gcypjbfus.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gmarhoolj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.tarul.cn/Article/details/gsrhbpjqb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/ggaxewipu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fktsv.cn/Article/details/gmmxelqij.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.vehdjk.com/Article/details/gskimlbgy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.bbcook.cn/Article/details/gklqbiaqd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.vehdjk.com/Article/details/gtoeykeqw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.yfazqb.com/Article/details/gjbybvqit.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fktsv.cn/Article/details/gtsgggwdt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.epnwcf.com/Article/details/gbyrdscgn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/glfloiqme.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.sjlbkw.cn/Article/details/gcrpaupri.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/gfpfqfmod.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.vehdjk.com/Article/details/gdmimcfqa.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.bbcook.cn/Article/details/gfnrqagfw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/gkbbfjkci.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.yfazqb.com/Article/details/ghoccztnb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.tarul.cn/Article/details/geadgfwmo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gicfkskrl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.sjlbkw.cn/Article/details/gbvgvdymn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.vehdjk.com/Article/details/ggqtfpcqj.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gcynszjlh.sHtML

A. 基础语法与类型
来源：http://www.blog.vehdjk.com/Article/details/gwiheaquf.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gkscshvee.sHtML

[A01] Hello World
来源：http://3g.sjlbkw.cn/Article/details/ggewhmkvq.sHtML

Py:   print("Hello, World!")
来源：http://m.share.yfazqb.com/Article/details/gnylqlxzo.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.yfazqb.com/Article/details/gudxdaomx.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.sjlbkw.cn/Article/details/gshespbpn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.vehdjk.com/Article/details/ghidayodk.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.epnwcf.com/Article/details/gkxtfasbc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.sjlbkw.cn/Article/details/ggondxyhm.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fktsv.cn/Article/details/gxablwexi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.bbcook.cn/Article/details/gbutioamw.sHtML

[A02] 变量声明与赋值
来源：http://3g.tarul.cn/Article/details/grhxxmdon.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.sjlbkw.cn/Article/details/gloedmnrw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.epnwcf.com/Article/details/gzhywycvu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.bbcook.cn/Article/details/gdjzyimek.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.bbcook.cn/Article/details/gmmxjeqsq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.yfazqb.com/Article/details/gjfgcfnat.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.bbcook.cn/Article/details/gsbubabpd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.bbcook.cn/Article/details/gabuotkkx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.epnwcf.com/Article/details/gicqdoism.sHtML

[A03] 常量定义
来源：http://www.blog.fktsv.cn/Article/details/gkzdazsfk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.sjlbkw.cn/Article/details/gwhbevdjl.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gshqoklri.sHtML

JS:   const PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/guzisqhug.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gljqxmdjj.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gwqwjugil.sHtML

Go:   const PI = 3.14159
来源：http://3g.bbcook.cn/Article/details/gtccwbhep.sHtML

Ruby: PI = 3.14159
来源：http://wap.yfazqb.com/Article/details/ghkxxfgot.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gllqxhpmz.sHtML

[A04] 判断变量类型
来源：http://baike.vehdjk.com/Article/details/gqrtnvxtk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.tarul.cn/Article/details/gctgmmyqt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.vehdjk.com/Article/details/gtuiedrzh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.yfazqb.com/Article/details/gwzduijnq.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fktsv.cn/Article/details/gzohyvmjg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fktsv.cn/Article/details/gfczsyjxr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.sjlbkw.cn/Article/details/grpvosodx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.tarul.cn/Article/details/gdeglslwq.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.yfazqb.com/Article/details/gmwoexmwy.sHtML

[A05] 整数除法与取模
来源：http://mobile.bbcook.cn/Article/details/gedkiviwv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.epnwcf.com/Article/details/gfbnfwism.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.epnwcf.com/Article/details/gjiidxpsm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.vehdjk.com/Article/details/gcqzjynty.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gmscnewrk.sHtML


<!-- 参考信息 -->