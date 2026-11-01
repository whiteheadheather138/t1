代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.epnwcf.com/Article/details/gnyxcglad.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.vehdjk.com/Article/details/gdodaskxb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.epnwcf.com/Article/details/glzbxsgli.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fktsv.cn/Article/details/gcdeczczr.sHtML

[U43] PHP：声明命名空间
来源：http://3g.bbcook.cn/Article/details/gcutotqcs.sHtML

namespace App\Http;
来源：http://www.share.sjlbkw.cn/Article/details/gnizgpjyq.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.tarul.cn/Article/details/gdxpgcssk.sHtML

declare(strict_types=1);
来源：http://www.share.yfazqb.com/Article/details/geovaokbz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.bbcook.cn/Article/details/gjuauhovl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.tarul.cn/Article/details/gfdmsqgdo.sHtML

[U46] PHP：可空类型
来源：http://www.blog.tarul.cn/Article/details/gzlyqitxv.sHtML

?string $name = null
来源：http://blog.sjlbkw.cn/Article/details/gqcxhvheq.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fktsv.cn/Article/details/gxriuqmoj.sHtML

int|string $id
来源：http://wap.yfazqb.com/Article/details/gofsnomzq.sHtML

[U48] PHP：纯枚举
来源：http://www.share.bbcook.cn/Article/details/gaukgqwpw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.yfazqb.com/Article/details/gfxubncta.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.vehdjk.com/Article/details/gpufuvksm.sHtML

public readonly string $name
来源：http://m.share.fktsv.cn/Article/details/gfzmisojn.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fktsv.cn/Article/details/gytcndbek.sHtML

public function __construct(private int $id) {}
来源：http://mobile.sjlbkw.cn/Article/details/gryfqtqjd.sHtML

[U51] PHP：数组解构
来源：http://wap.fktsv.cn/Article/details/gjblssitq.sHtML

[$a, $b] = $arr;
来源：http://mobile.bbcook.cn/Article/details/gnydrjtgo.sHtML

[U52] PHP：箭头函数
来源：http://baike.sjlbkw.cn/Article/details/gystpuduw.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.epnwcf.com/Article/details/gjtnfrrkd.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.sjlbkw.cn/Article/details/goqydnvuw.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.yfazqb.com/Article/details/gapdhebpu.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fktsv.cn/Article/details/gngubzkfv.sHtML

$obj?->method()
来源：http://baike.epnwcf.com/Article/details/gymtmambu.sHtML

[U55] PHP：match 表达式
来源：http://wap.vehdjk.com/Article/details/gjfasgnxm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.yfazqb.com/Article/details/gtnkvliav.sHtML

[U56] PHP：命名参数
来源：http://blog.yfazqb.com/Article/details/gdxtifsbv.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/gwbziwwrf.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gyacdanbl.sHtML

"值: {$a}"
来源：http://m.share.bbcook.cn/Article/details/gcnygrtaq.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.bbcook.cn/Article/details/gfrteblby.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.sjlbkw.cn/Article/details/grmncwici.sHtML

[U59] PHP：自定义排序
来源：http://baike.tarul.cn/Article/details/gliojpvbw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fktsv.cn/Article/details/gbwbxbilq.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.yfazqb.com/Article/details/grsxlmcgh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.yfazqb.com/Article/details/gzqrdnnpv.sHtML

[U61] PHP：正则
来源：http://3g.bbcook.cn/Article/details/gyvfdlyoi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.bbcook.cn/Article/details/gycsxcfeu.sHtML

[U62] PHP：日期对象
来源：http://mobile.epnwcf.com/Article/details/gkzejvify.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.bbcook.cn/Article/details/gzzzgovii.sHtML

[U63] PHP：文件读写
来源：http://www.share.fktsv.cn/Article/details/gokqkdhbl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.epnwcf.com/Article/details/gbrkwmpuv.sHtML

[U64] PHP：目录遍历
来源：http://wap.sjlbkw.cn/Article/details/gvdamlagv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.epnwcf.com/Article/details/gbvebrexw.sHtML

[U65] PHP：会话
来源：http://baike.bbcook.cn/Article/details/gzwfxvhar.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gcdejnvyl.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.sjlbkw.cn/Article/details/glcvpufrp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.tarul.cn/Article/details/gzsdvwxuq.sHtML

[U67] PHP：处理文件上传
来源：http://baike.vehdjk.com/Article/details/guvrhtraf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.tarul.cn/Article/details/gucujvzcs.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.epnwcf.com/Article/details/grqgdgppg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.bbcook.cn/Article/details/gdlgiumjz.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.yfazqb.com/Article/details/guewaobxu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fktsv.cn/Article/details/gxybupanm.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gffopyxou.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.bbcook.cn/Article/details/gbhvvieno.sHtML

[U71] PHP：抛出异常
来源：http://3g.yfazqb.com/Article/details/gupzxvnwq.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.tarul.cn/Article/details/grjwmmzpa.sHtML

[U72] PHP：写错误日志
来源：http://baike.vehdjk.com/Article/details/gueltdloy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.sjlbkw.cn/Article/details/ggvmdifqb.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.epnwcf.com/Article/details/gusrujcxf.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.tarul.cn/Article/details/gwjpktuky.sHtML

[U74] PHP：读取环境变量
来源：http://wap.epnwcf.com/Article/details/gwpnpyflt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fktsv.cn/Article/details/gdezmguut.sHtML

[U75] PHP：依赖注入
来源：http://read.share.bbcook.cn/Article/details/gsdkrfory.sHtML

composer require psr/container
来源：http://www.blog.vehdjk.com/Article/details/gebnkocoy.sHtML

[U76] PHP：简单路由
来源：http://baike.fktsv.cn/Article/details/gthgmbmtt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.tarul.cn/Article/details/gjqbaydmv.sHtML

[U77] PHP：模板渲染
来源：http://read.share.bbcook.cn/Article/details/goibcozfb.sHtML

composer require twig/twig
来源：http://mobile.sjlbkw.cn/Article/details/gqlsomarw.sHtML

[U78] PHP：单元测试
来源：http://m.share.yfazqb.com/Article/details/glscrocey.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.bbcook.cn/Article/details/gjfkmkevc.sHtML

[U79] PHP：静态分析
来源：http://www.share.epnwcf.com/Article/details/gdosigmsj.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fktsv.cn/Article/details/grnprximf.sHtML

[U80] PHP：代码规范修复
来源：http://3g.epnwcf.com/Article/details/gvufyvmub.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.epnwcf.com/Article/details/gssiqmhtr.sHtML

[U81] JS：初始化项目
来源：http://wap.bbcook.cn/Article/details/gcyrvwjpu.sHtML

npm init -y;  npm i express
来源：http://wap.yfazqb.com/Article/details/gnbowwvxz.sHtML

[U82] JS：package.json 脚本
来源：http://wap.epnwcf.com/Article/details/giyqejqwd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.bbcook.cn/Article/details/gcegtjavy.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.bbcook.cn/Article/details/gozfyphho.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.bbcook.cn/Article/details/gmcgiisch.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.vehdjk.com/Article/details/gxiexntrn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.epnwcf.com/Article/details/gohfmesip.sHtML

[U85] JS：可选链
来源：http://www.blog.fktsv.cn/Article/details/gusynxtrp.sHtML

a?.b?.c
来源：http://blog.vehdjk.com/Article/details/gcpoquqwl.sHtML

[U86] JS：空值合并
来源：http://3g.vehdjk.com/Article/details/gkahryfux.sHtML

a ?? b
来源：http://www.blog.epnwcf.com/Article/details/gikaiegmq.sHtML

[U87] JS：解构默认值
来源：http://www.blog.sjlbkw.cn/Article/details/gieoywrmm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.vehdjk.com/Article/details/gnykfpmwc.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fktsv.cn/Article/details/gvxuplvsp.sHtML

{ ...a, ...b }
来源：http://www.blog.tarul.cn/Article/details/gboquvweg.sHtML

[U89] JS：数组去重
来源：http://www.m.share.epnwcf.com/Article/details/gzzuvseew.sHtML

[...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/ghhnieeeu.sHtML

[U90] JS：数字数组排序
来源：http://wap.epnwcf.com/Article/details/gndhfwqhl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gumzvlxuz.sHtML

[U91] JS：对象键值遍历
来源：http://baike.yfazqb.com/Article/details/gtochfxqn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fktsv.cn/Article/details/gjwasnuno.sHtML

[U92] JS：深拷贝
来源：http://baike.epnwcf.com/Article/details/gzfnrefcl.sHtML

structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/gehspjhyk.sHtML

[U93] JS：模板字符串
来源：http://blog.bbcook.cn/Article/details/grwqlqttr.sHtML

`共 ${n} 条`
来源：http://www.blog.sjlbkw.cn/Article/details/grcvktilt.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.epnwcf.com/Article/details/gezowysre.sHtML

const double = x => x * 2;
来源：http://mobile.yfazqb.com/Article/details/gnzmmgwgr.sHtML

[U95] JS：Promise 包装
来源：http://blog.sjlbkw.cn/Article/details/gpcqowgdb.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjpnyduu.sHtML

[U96] JS：async/await 与异常
来源：http://3g.bbcook.cn/Article/details/gomiqncgh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/gyeogfjlg.sHtML

[U97] JS：并发请求
来源：http://3g.tarul.cn/Article/details/gglqkivin.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gntigpiwj.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.sjlbkw.cn/Article/details/gpwbesfdb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.vehdjk.com/Article/details/gatikwhkb.sHtML

[U99] JS：事件监听
来源：http://mobile.vehdjk.com/Article/details/gwifyviud.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.tarul.cn/Article/details/glxpyunax.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.tarul.cn/Article/details/glhmacauq.sHtML

document.querySelector(".item")
来源：http://www.blog.tarul.cn/Article/details/ghtswrhbl.sHtML

[U101] JS：classList 操作
来源：http://3g.yfazqb.com/Article/details/gqmxewsje.sHtML

el.classList.toggle("active")
来源：http://www.blog.bbcook.cn/Article/details/glzchibzl.sHtML

[U102] JS：本地存储
来源：http://mobile.bbcook.cn/Article/details/ghlvvgfbv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.tarul.cn/Article/details/gkifffdoc.sHtML

[U103] JS：定时器
来源：http://mobile.yfazqb.com/Article/details/gakzrnnlj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.bbcook.cn/Article/details/gkdyqgpoj.sHtML

[U104] JS：防抖
来源：http://www.share.yfazqb.com/Article/details/gaonzanym.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gvbqnwmym.sHtML

[U105] JS：节流
来源：http://baike.bbcook.cn/Article/details/gafgdwnqh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.sjlbkw.cn/Article/details/gaoniwwjb.sHtML

[U106] JS：日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/gifcxowim.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.epnwcf.com/Article/details/gdfbircah.sHtML

[U107] JS：数字千分位
来源：http://read.share.vehdjk.com/Article/details/gchdlcqig.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fktsv.cn/Article/details/glcbivahx.sHtML

[U108] JS：随机整数
来源：http://www.share.sjlbkw.cn/Article/details/ggtoerahq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fktsv.cn/Article/details/glxanzwbt.sHtML

[U109] JS：数组分组
来源：http://read.share.epnwcf.com/Article/details/gjcgqjwew.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.vehdjk.com/Article/details/glgohjxti.sHtML

[U110] JS：数组分块
来源：http://read.share.bbcook.cn/Article/details/gzjmclzeb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.tarul.cn/Article/details/gxtejfdar.sHtML

[U111] JS：对象转 Map
来源：http://blog.yfazqb.com/Article/details/gdlasiynl.sHtML

new Map(Object.entries(obj))
来源：http://m.share.bbcook.cn/Article/details/gpfngcpac.sHtML

[U112] JS：字符串补位
来源：http://wap.yfazqb.com/Article/details/gmrzqqofk.sHtML

"7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gzblgxnwx.sHtML

[U113] JS：正则替换全部
来源：http://wap.sjlbkw.cn/Article/details/gorjeriip.sHtML

s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gdquvcwfr.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.yfazqb.com/Article/details/gxbugbzvj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.tarul.cn/Article/details/gcfcfymlq.sHtML

[U115] JS：生成 UUID
来源：http://wap.sjlbkw.cn/Article/details/goifjuvcu.sHtML

crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/gcxmuadzy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.epnwcf.com/Article/details/gzjrzedjm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gzaaeydpy.sHtML

[U117] JS：单元测试
来源：http://blog.epnwcf.com/Article/details/gnbuihpdm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.bbcook.cn/Article/details/ghusvqdsz.sHtML

[U118] JS：开发服务器
来源：http://www.share.yfazqb.com/Article/details/gjkvsqoml.sHtML

npm i -D vite;  npx vite
来源：http://baike.vehdjk.com/Article/details/gjhnvmxbf.sHtML

[U119] JS：生产构建
来源：http://read.share.tarul.cn/Article/details/gbcipwjbg.sHtML

npx vite build
来源：http://www.m.share.bbcook.cn/Article/details/gpagjjgcm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.bbcook.cn/Article/details/ggmvsirzw.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.epnwcf.com/Article/details/grsdumled.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gpfmqamtn.sHtML

统计汇总
来源：http://blog.yfazqb.com/Article/details/gcmmyxkxz.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gtqcybpzo.sHtML

按语言统计（条）：
来源：http://mobile.vehdjk.com/Article/details/glsrlciwn.sHtML

Python ......... 252
来源：http://3g.sjlbkw.cn/Article/details/gxkvkmmgl.sHtML

PHP ............ 252
来源：http://blog.tarul.cn/Article/details/gsilpdgrs.sHtML

JavaScript ..... 252
来源：http://wap.epnwcf.com/Article/details/ggylfjtmt.sHtML

TypeScript ..... 212
来源：http://read.share.sjlbkw.cn/Article/details/gybbziygd.sHtML

Java ........... 212
来源：http://wap.bbcook.cn/Article/details/ggpcrkmlf.sHtML

Go ............. 212
来源：http://www.m.share.fktsv.cn/Article/details/gwdqzgebt.sHtML

Ruby ........... 212
来源：http://baike.bbcook.cn/Article/details/gqkejpbcz.sHtML

C# ............. 212
来源：http://m.share.fktsv.cn/Article/details/gtvysrfrj.sHtML

C .............. 30
来源：http://mobile.fktsv.cn/Article/details/gqfejinxi.sHtML

C++ ............ 30
来源：http://baike.yfazqb.com/Article/details/gxjkdgrsb.sHtML

SQL ............ 90
来源：http://m.share.vehdjk.com/Article/details/geuklypfs.sHtML

Bash ........... 80
来源：http://read.share.epnwcf.com/Article/details/grukajjtx.sHtML

Kotlin ......... 15
来源：http://baike.yfazqb.com/Article/details/ganvsocah.sHtML

Swift .......... 15
来源：http://www.blog.epnwcf.com/Article/details/gfnxwrczl.sHtML

Lua ............ 10
来源：http://www.m.share.epnwcf.com/Article/details/gqwcepytl.sHtML

Perl ........... 10
来源：http://www.blog.fktsv.cn/Article/details/grsyzqmft.sHtML

Scala .......... 10
来源：http://3g.epnwcf.com/Article/details/gdptkekrb.sHtML

------------------------------------
来源：http://wap.tarul.cn/Article/details/ggddkwbfd.sHtML

合计 ........... 2106 条
来源：http://m.share.fktsv.cn/Article/details/goguwsiig.sHtML

按章节统计：
来源：http://mobile.tarul.cn/Article/details/ggiiuuyjq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.bbcook.cn/Article/details/ggcqbbnpn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.bbcook.cn/Article/details/gjtkwqktp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fktsv.cn/Article/details/gljafpuvc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.epnwcf.com/Article/details/gcpyitnti.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.yfazqb.com/Article/details/gccofaoqm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.yfazqb.com/Article/details/gzdzanjay.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.yfazqb.com/Article/details/gxocceouw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.vehdjk.com/Article/details/gvfhiutox.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/gpblazkxh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.epnwcf.com/Article/details/gtjnymspi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/gbsypxxuu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gnoozvwaa.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/gnozeoryj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fktsv.cn/Article/details/gcdkxcxhf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.bbcook.cn/Article/details/gegwqzpck.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gnwherrku.sHtML

Q SQL 专题                              90
来源：http://mobile.sjlbkw.cn/Article/details/gwtwcnrhw.sHtML

R Bash 专题                             80
来源：http://3g.fktsv.cn/Article/details/gczkybzfv.sHtML

S C / C++ 专题                          60
来源：http://baike.sjlbkw.cn/Article/details/gnloirrxm.sHtML

T 其他语言补充                          60
来源：http://baike.yfazqb.com/Article/details/ganvpgsnb.sHtML

U 高频实用片段                         120
来源：http://m.share.vehdjk.com/Article/details/ghwcwufbc.sHtML

------------------------------------
来源：http://wap.yfazqb.com/Article/details/gmzmuhvzp.sHtML

合计                                  2106 条
来源：http://wap.epnwcf.com/Article/details/gevzlsawc.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.yfazqb.com/Article/details/gzpnnwfat.sHtML

使用提醒
来源：http://mobile.bbcook.cn/Article/details/goqafcjgn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.vehdjk.com/Article/details/gngxmtfin.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.vehdjk.com/Article/details/gprncjfqq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.vehdjk.com/Article/details/gnrqvbhyf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.yfazqb.com/Article/details/gnsfwnlxn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.bbcook.cn/Article/details/gxrrneowy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.sjlbkw.cn/Article/details/gitrylpnh.sHtML

—— 文件结束 ——
来源：http://m.share.yfazqb.com/Article/details/gfbdmsjyi.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/goovqvdfg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.bbcook.cn/Article/details/gbolkzthe.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fktsv.cn/Article/details/grgngjgpx.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ggygtarig.sHtML

【收录内容】
来源：http://www.blog.epnwcf.com/Article/details/gxndpzfcz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.epnwcf.com/Article/details/gdujzcbgf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.yfazqb.com/Article/details/gdsjqzwhm.sHtML

SQL · Bash · C · C++
来源：http://3g.yfazqb.com/Article/details/geplrjwfk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fktsv.cn/Article/details/gtcbliayi.sHtML

【使用说明】
来源：http://blog.fktsv.cn/Article/details/gkephzwez.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.epnwcf.com/Article/details/gjyqeozrj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.epnwcf.com/Article/details/gmyqsseua.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.epnwcf.com/Article/details/ghtzlukuv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.tarul.cn/Article/details/gcqbxddnk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.vehdjk.com/Article/details/gwzhhfhjs.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.yfazqb.com/Article/details/gxrrrlnjm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.yfazqb.com/Article/details/gmvswwdzn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fktsv.cn/Article/details/gvyihiwvx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.bbcook.cn/Article/details/gxlznwmjr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.bbcook.cn/Article/details/glpsgrhnk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.tarul.cn/Article/details/gegrzapfw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.bbcook.cn/Article/details/gljqhxyao.sHtML

【文件统计】
来源：http://3g.tarul.cn/Article/details/gkbfaqipa.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.sjlbkw.cn/Article/details/gblowzwin.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/grpevdmrg.sHtML

目  录
来源：http://3g.epnwcf.com/Article/details/guivmtmyz.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/gzkehnrxo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.tarul.cn/Article/details/gxlgxvxmu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.tarul.cn/Article/details/gugzeuaha.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.epnwcf.com/Article/details/gfzgscqrt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.epnwcf.com/Article/details/gsntwcqvq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.yfazqb.com/Article/details/guvubgivg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.epnwcf.com/Article/details/gyojhabao.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.bbcook.cn/Article/details/gwgrattzz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.bbcook.cn/Article/details/gtvsgyagi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/gzcdbuebp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.vehdjk.com/Article/details/gduvcldrj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.vehdjk.com/Article/details/gcpgvvuiz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/gfnaltilh.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.epnwcf.com/Article/details/gjjdoqdmw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.yfazqb.com/Article/details/gatcvmwxk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fktsv.cn/Article/details/guglmcwys.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/gppuwprft.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fktsv.cn/Article/details/gknanozhg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.sjlbkw.cn/Article/details/goovymjix.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.bbcook.cn/Article/details/glwbwnukp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.tarul.cn/Article/details/gqfcbyyqc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.epnwcf.com/Article/details/gcpjbvgav.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ggqangfma.sHtML

A. 基础语法与类型
来源：http://3g.vehdjk.com/Article/details/gukpjuiki.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gpbcbamil.sHtML

[A01] Hello World
来源：http://www.m.share.bbcook.cn/Article/details/girnojftd.sHtML

Py:   print("Hello, World!")
来源：http://wap.tarul.cn/Article/details/gcegmrgfg.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.epnwcf.com/Article/details/gbivujsyr.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.tarul.cn/Article/details/gszuwatlh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.yfazqb.com/Article/details/gknmbzrxs.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.yfazqb.com/Article/details/gkunmyrfo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.epnwcf.com/Article/details/gwblzdali.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.bbcook.cn/Article/details/gvxstrfex.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.yfazqb.com/Article/details/gpjrzldlv.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fktsv.cn/Article/details/gzcburply.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.bbcook.cn/Article/details/grodmgcxi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.sjlbkw.cn/Article/details/gkzxovzvh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.yfazqb.com/Article/details/gkosofete.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.vehdjk.com/Article/details/gfexvxujx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.epnwcf.com/Article/details/gqlmvgimf.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.bbcook.cn/Article/details/gnfjnmpvb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.yfazqb.com/Article/details/gsjsajxvp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fktsv.cn/Article/details/gbtcgfijq.sHtML

[A03] 常量定义
来源：http://blog.bbcook.cn/Article/details/ggbykizwn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.bbcook.cn/Article/details/gwunojtff.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gpvtjhakm.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gjmgxczvl.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gejfymijm.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gfexywrki.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fktsv.cn/Article/details/gnfbvcate.sHtML

Ruby: PI = 3.14159
来源：http://blog.epnwcf.com/Article/details/gdpbodqkq.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gmbrxsaej.sHtML

[A04] 判断变量类型
来源：http://www.blog.bbcook.cn/Article/details/givxgpejw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.yfazqb.com/Article/details/ghffymlah.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fktsv.cn/Article/details/gafpqmpav.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.sjlbkw.cn/Article/details/gbfrceikz.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.epnwcf.com/Article/details/goefinsdx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgdmtbld.sHtML


<!-- 参考信息 -->