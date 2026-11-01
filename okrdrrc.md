代发 wailian999

[U49] PHP：只读属性
来源：http://read.share.tarul.cn/Article/details/gozdgvcvp.sHtML

public readonly string $name
来源：http://www.share.bbcook.cn/Article/details/ggdwfkjum.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.yfazqb.com/Article/details/gwyeldohd.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fktsv.cn/Article/details/glsockmxw.sHtML

[U51] PHP：数组解构
来源：http://baike.sjlbkw.cn/Article/details/gasvltmdp.sHtML

[$a, $b] = $arr;
来源：http://wap.vehdjk.com/Article/details/glhlrldys.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.bbcook.cn/Article/details/gutzuzelq.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.epnwcf.com/Article/details/garxoxrgp.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.bbcook.cn/Article/details/getkqnxug.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.sjlbkw.cn/Article/details/girgaoyry.sHtML

[U54] PHP：空安全调用
来源：http://baike.tarul.cn/Article/details/gkcjtecop.sHtML

$obj?->method()
来源：http://mobile.vehdjk.com/Article/details/gambliaeb.sHtML

[U55] PHP：match 表达式
来源：http://blog.bbcook.cn/Article/details/gbxrocokx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.tarul.cn/Article/details/gbrftzpkv.sHtML

[U56] PHP：命名参数
来源：http://baike.tarul.cn/Article/details/gukhourvb.sHtML

f(a: 1, b: 2)
来源：http://baike.yfazqb.com/Article/details/gdfxptgsm.sHtML

[U57] PHP：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gpgllwlgo.sHtML

"值: {$a}"
来源：http://read.share.sjlbkw.cn/Article/details/ghvkecnoe.sHtML

[U58] PHP：数组三件套
来源：http://mobile.tarul.cn/Article/details/gasutrbcq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.bbcook.cn/Article/details/gljnjxnfe.sHtML

[U59] PHP：自定义排序
来源：http://m.share.vehdjk.com/Article/details/gjhmkkgou.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.tarul.cn/Article/details/gauycjzrr.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.tarul.cn/Article/details/glojmlngs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.bbcook.cn/Article/details/giluddgqm.sHtML

[U61] PHP：正则
来源：http://www.blog.fktsv.cn/Article/details/gcisggaco.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fktsv.cn/Article/details/gtghcpyvz.sHtML

[U62] PHP：日期对象
来源：http://read.share.sjlbkw.cn/Article/details/gqhmpmwhz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.sjlbkw.cn/Article/details/gssdlxxqq.sHtML

[U63] PHP：文件读写
来源：http://3g.yfazqb.com/Article/details/gzhzzsibf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.yfazqb.com/Article/details/gvvmvrbgb.sHtML

[U64] PHP：目录遍历
来源：http://read.share.tarul.cn/Article/details/gpwosmiot.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.bbcook.cn/Article/details/gceaushbm.sHtML

[U65] PHP：会话
来源：http://mobile.tarul.cn/Article/details/gnewnhgvy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gaejbeywr.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.bbcook.cn/Article/details/ghcemnclt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.sjlbkw.cn/Article/details/gnkdpwult.sHtML

[U67] PHP：处理文件上传
来源：http://wap.epnwcf.com/Article/details/gaujolekr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.yfazqb.com/Article/details/giizpepyn.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fktsv.cn/Article/details/guxdedjut.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.epnwcf.com/Article/details/gdnczwwea.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.yfazqb.com/Article/details/gslpkrcvd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.vehdjk.com/Article/details/gzwloxata.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.epnwcf.com/Article/details/gqbghrpjm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.vehdjk.com/Article/details/glbfqtqgf.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fktsv.cn/Article/details/grbclhejh.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.epnwcf.com/Article/details/gvczdtxvt.sHtML

[U72] PHP：写错误日志
来源：http://baike.fktsv.cn/Article/details/gyjtokhke.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.yfazqb.com/Article/details/gqsdjzexd.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.epnwcf.com/Article/details/gtwxamhrz.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.epnwcf.com/Article/details/guvizdkov.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fktsv.cn/Article/details/gkssojaev.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.epnwcf.com/Article/details/ggohawcie.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fktsv.cn/Article/details/giseidgjg.sHtML

composer require psr/container
来源：http://baike.sjlbkw.cn/Article/details/gtsaulnso.sHtML

[U76] PHP：简单路由
来源：http://read.share.epnwcf.com/Article/details/gkhdgyhjm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.yfazqb.com/Article/details/gnaiffcny.sHtML

[U77] PHP：模板渲染
来源：http://m.share.yfazqb.com/Article/details/golwjimgx.sHtML

composer require twig/twig
来源：http://www.share.tarul.cn/Article/details/ggqxvnejw.sHtML

[U78] PHP：单元测试
来源：http://wap.sjlbkw.cn/Article/details/gjgpotdfd.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.yfazqb.com/Article/details/gzvauerrv.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fktsv.cn/Article/details/grylyvfus.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.vehdjk.com/Article/details/gxggviael.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.vehdjk.com/Article/details/gjrfgsaai.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.vehdjk.com/Article/details/gzckshthi.sHtML

[U81] JS：初始化项目
来源：http://baike.tarul.cn/Article/details/gxhiuedyf.sHtML

npm init -y;  npm i express
来源：http://www.blog.epnwcf.com/Article/details/gksluksdf.sHtML

[U82] JS：package.json 脚本
来源：http://baike.tarul.cn/Article/details/gukfxjphi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.tarul.cn/Article/details/gjkushtdj.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.tarul.cn/Article/details/gvgabblvf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.epnwcf.com/Article/details/gnafjwqje.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.bbcook.cn/Article/details/ghdwyakwt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.yfazqb.com/Article/details/ghfswcqwh.sHtML

[U85] JS：可选链
来源：http://www.m.share.tarul.cn/Article/details/gckxjarry.sHtML

a?.b?.c
来源：http://wap.vehdjk.com/Article/details/gucqzappu.sHtML

[U86] JS：空值合并
来源：http://www.blog.bbcook.cn/Article/details/gffargmew.sHtML

a ?? b
来源：http://www.share.vehdjk.com/Article/details/gvjtdzndb.sHtML

[U87] JS：解构默认值
来源：http://3g.sjlbkw.cn/Article/details/gihcnnkjp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.bbcook.cn/Article/details/gpzxxfwnj.sHtML

[U88] JS：对象展开合并
来源：http://3g.epnwcf.com/Article/details/gfgsvtpld.sHtML

{ ...a, ...b }
来源：http://www.m.share.vehdjk.com/Article/details/gbnjeecya.sHtML

[U89] JS：数组去重
来源：http://www.m.share.tarul.cn/Article/details/gwajfczrp.sHtML

[...new Set(arr)]
来源：http://3g.yfazqb.com/Article/details/gcnvvbfmj.sHtML

[U90] JS：数字数组排序
来源：http://www.share.sjlbkw.cn/Article/details/gystoradq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/gxgunjkmb.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.yfazqb.com/Article/details/gjtpvwrxd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.vehdjk.com/Article/details/gfkllyncb.sHtML

[U92] JS：深拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gdakzisyi.sHtML

structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gvplfwoph.sHtML

[U93] JS：模板字符串
来源：http://wap.sjlbkw.cn/Article/details/guzuczxpu.sHtML

`共 ${n} 条`
来源：http://mobile.tarul.cn/Article/details/ghcxwsyzn.sHtML

[U94] JS：箭头函数
来源：http://www.share.epnwcf.com/Article/details/gjypfbyju.sHtML

const double = x => x * 2;
来源：http://wap.epnwcf.com/Article/details/gnbnotjvm.sHtML

[U95] JS：Promise 包装
来源：http://baike.yfazqb.com/Article/details/gfmgfpvca.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.vehdjk.com/Article/details/gmrenffxo.sHtML

[U96] JS：async/await 与异常
来源：http://wap.bbcook.cn/Article/details/gkiytufrt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gvvqakakt.sHtML

[U97] JS：并发请求
来源：http://read.share.epnwcf.com/Article/details/gaofdjvvn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/glmqjpimh.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fktsv.cn/Article/details/gmzadgvau.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.sjlbkw.cn/Article/details/gwtnqdbqe.sHtML

[U99] JS：事件监听
来源：http://baike.epnwcf.com/Article/details/gfmomghvk.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.bbcook.cn/Article/details/gcjqsvmfl.sHtML

[U100] JS：DOM 查询
来源：http://wap.fktsv.cn/Article/details/gcxcuapkz.sHtML

document.querySelector(".item")
来源：http://read.share.fktsv.cn/Article/details/gzghifurk.sHtML

[U101] JS：classList 操作
来源：http://baike.epnwcf.com/Article/details/gdeexszey.sHtML

el.classList.toggle("active")
来源：http://m.share.epnwcf.com/Article/details/gaignsywy.sHtML

[U102] JS：本地存储
来源：http://mobile.yfazqb.com/Article/details/ggfdvowrh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.yfazqb.com/Article/details/gqjyvzkqe.sHtML

[U103] JS：定时器
来源：http://wap.sjlbkw.cn/Article/details/gznreqaya.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.sjlbkw.cn/Article/details/gwahmrtyc.sHtML

[U104] JS：防抖
来源：http://www.blog.fktsv.cn/Article/details/guzozcdmb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.vehdjk.com/Article/details/gublnbltz.sHtML

[U105] JS：节流
来源：http://m.share.bbcook.cn/Article/details/gdnlysmrf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.vehdjk.com/Article/details/gyfhbxkyr.sHtML

[U106] JS：日期格式化
来源：http://3g.tarul.cn/Article/details/gjwkrfcok.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.tarul.cn/Article/details/gbfhspuci.sHtML

[U107] JS：数字千分位
来源：http://www.blog.sjlbkw.cn/Article/details/gguybhgha.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.bbcook.cn/Article/details/gppxrujrc.sHtML

[U108] JS：随机整数
来源：http://www.m.share.bbcook.cn/Article/details/gzhzwydbl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.bbcook.cn/Article/details/ghettpmql.sHtML

[U109] JS：数组分组
来源：http://m.share.tarul.cn/Article/details/gdyrtgqdp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.epnwcf.com/Article/details/gnyhedkmn.sHtML

[U110] JS：数组分块
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfyclycw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.vehdjk.com/Article/details/gmsbtqfxo.sHtML

[U111] JS：对象转 Map
来源：http://read.share.sjlbkw.cn/Article/details/gcvyvdexl.sHtML

new Map(Object.entries(obj))
来源：http://wap.fktsv.cn/Article/details/goowncgee.sHtML

[U112] JS：字符串补位
来源：http://www.blog.bbcook.cn/Article/details/gvmguodqu.sHtML

"7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gkjlrxuyv.sHtML

[U113] JS：正则替换全部
来源：http://m.share.vehdjk.com/Article/details/ghylfgvel.sHtML

s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/gtyddalwc.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.sjlbkw.cn/Article/details/glzpkftem.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.yfazqb.com/Article/details/gwvjitsuf.sHtML

[U115] JS：生成 UUID
来源：http://blog.tarul.cn/Article/details/ggywftyrr.sHtML

crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/gswdkhcbb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.bbcook.cn/Article/details/gdfpdadwm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.epnwcf.com/Article/details/gefewqaus.sHtML

[U117] JS：单元测试
来源：http://mobile.yfazqb.com/Article/details/gobabbwme.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjqbzvxc.sHtML

[U118] JS：开发服务器
来源：http://blog.vehdjk.com/Article/details/gwykxrflk.sHtML

npm i -D vite;  npx vite
来源：http://read.share.sjlbkw.cn/Article/details/gcviphoum.sHtML

[U119] JS：生产构建
来源：http://blog.tarul.cn/Article/details/giwgaosdu.sHtML

npx vite build
来源：http://www.m.share.tarul.cn/Article/details/grujqjejs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fktsv.cn/Article/details/grgbfiqip.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fktsv.cn/Article/details/ghykozryc.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gctmqmfve.sHtML

统计汇总
来源：http://www.share.fktsv.cn/Article/details/gahllkevy.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gwtmbhqxo.sHtML

按语言统计（条）：
来源：http://m.share.sjlbkw.cn/Article/details/gtaycciin.sHtML

Python ......... 252
来源：http://baike.fktsv.cn/Article/details/gugsmksid.sHtML

PHP ............ 252
来源：http://www.m.share.yfazqb.com/Article/details/glttyfalv.sHtML

JavaScript ..... 252
来源：http://www.m.share.yfazqb.com/Article/details/gqzblxxtv.sHtML

TypeScript ..... 212
来源：http://mobile.epnwcf.com/Article/details/gsqlhrsqu.sHtML

Java ........... 212
来源：http://baike.tarul.cn/Article/details/gupqgyisp.sHtML

Go ............. 212
来源：http://www.m.share.vehdjk.com/Article/details/gzsfczrkq.sHtML

Ruby ........... 212
来源：http://blog.bbcook.cn/Article/details/gmvflvtru.sHtML

C# ............. 212
来源：http://baike.sjlbkw.cn/Article/details/gluizowzk.sHtML

C .............. 30
来源：http://blog.tarul.cn/Article/details/gvompapfa.sHtML

C++ ............ 30
来源：http://www.share.yfazqb.com/Article/details/gtaadasjg.sHtML

SQL ............ 90
来源：http://wap.tarul.cn/Article/details/gbryrnjnt.sHtML

Bash ........... 80
来源：http://www.m.share.tarul.cn/Article/details/gcgwuseow.sHtML

Kotlin ......... 15
来源：http://baike.vehdjk.com/Article/details/gpagwntls.sHtML

Swift .......... 15
来源：http://www.m.share.yfazqb.com/Article/details/gngesiclx.sHtML

Lua ............ 10
来源：http://m.share.yfazqb.com/Article/details/gtwqbdfqb.sHtML

Perl ........... 10
来源：http://wap.bbcook.cn/Article/details/gadcyjcfh.sHtML

Scala .......... 10
来源：http://www.share.bbcook.cn/Article/details/gkrwbafyr.sHtML

------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gzhfkjfhi.sHtML

合计 ........... 2106 条
来源：http://baike.tarul.cn/Article/details/gszfxnusj.sHtML

按章节统计：
来源：http://mobile.vehdjk.com/Article/details/gvrtmhbad.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.bbcook.cn/Article/details/glszkgbof.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.yfazqb.com/Article/details/gjdvlccyr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.tarul.cn/Article/details/guqlfenwe.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.sjlbkw.cn/Article/details/gdqzlcutl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.vehdjk.com/Article/details/gbdstzajw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.bbcook.cn/Article/details/gyxhjwomf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fktsv.cn/Article/details/gwewgysmj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.yfazqb.com/Article/details/gvfiaehws.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/gvvxdnjpl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fktsv.cn/Article/details/ghkvgjyuu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/gggcmuxew.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gacymjsem.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/gtgvigayi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.tarul.cn/Article/details/gniiubndl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.epnwcf.com/Article/details/girtuchfv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gfammdfnq.sHtML

Q SQL 专题                              90
来源：http://blog.yfazqb.com/Article/details/ggdkqjraw.sHtML

R Bash 专题                             80
来源：http://wap.yfazqb.com/Article/details/ghgxeopuf.sHtML

S C / C++ 专题                          60
来源：http://www.share.tarul.cn/Article/details/gtnvbtudm.sHtML

T 其他语言补充                          60
来源：http://read.share.bbcook.cn/Article/details/gewquqpwq.sHtML

U 高频实用片段                         120
来源：http://www.m.share.epnwcf.com/Article/details/gpngfpcsb.sHtML

------------------------------------
来源：http://baike.vehdjk.com/Article/details/gkefmovpv.sHtML

合计                                  2106 条
来源：http://baike.vehdjk.com/Article/details/glokjtqxc.sHtML

--------------------------------------------------------------------------------
来源：http://3g.vehdjk.com/Article/details/gctnvlibs.sHtML

使用提醒
来源：http://mobile.epnwcf.com/Article/details/gmqaosjcl.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gdmacgvqf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.sjlbkw.cn/Article/details/gkttpdftd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.epnwcf.com/Article/details/giqvbywph.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.tarul.cn/Article/details/gisbpttyu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.yfazqb.com/Article/details/gcsgobopu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.vehdjk.com/Article/details/gdjafydbj.sHtML

—— 文件结束 ——
来源：http://mobile.yfazqb.com/Article/details/gyobobnhb.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gycnssdry.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.vehdjk.com/Article/details/gfbgmgflj.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.yfazqb.com/Article/details/gofxykjcn.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/glugdpqwa.sHtML

【收录内容】
来源：http://mobile.bbcook.cn/Article/details/guwdpbtdw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fktsv.cn/Article/details/gqpxmloen.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.yfazqb.com/Article/details/gazzbiavs.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.bbcook.cn/Article/details/ggektpmrj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fktsv.cn/Article/details/gindojeha.sHtML

【使用说明】
来源：http://blog.vehdjk.com/Article/details/gizocgchk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.sjlbkw.cn/Article/details/ggfvixzne.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.yfazqb.com/Article/details/gnfkqqpts.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.bbcook.cn/Article/details/gzmrplwat.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.sjlbkw.cn/Article/details/gojnwoave.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fktsv.cn/Article/details/gdmeivbzc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.epnwcf.com/Article/details/gieqcmnem.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.sjlbkw.cn/Article/details/gqiuggduj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.sjlbkw.cn/Article/details/gncuvqotb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.epnwcf.com/Article/details/gqzsyxlax.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.bbcook.cn/Article/details/geinkdzpl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fktsv.cn/Article/details/grvfwkhuz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.vehdjk.com/Article/details/gsyncgaxr.sHtML

【文件统计】
来源：http://mobile.epnwcf.com/Article/details/gcxhnykbp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.tarul.cn/Article/details/guqmzovys.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gqniiaxrd.sHtML

目  录
来源：http://3g.yfazqb.com/Article/details/gmptfxkyr.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.vehdjk.com/Article/details/ghraazavr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.yfazqb.com/Article/details/ggycbnwrb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.epnwcf.com/Article/details/gkogprayl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.bbcook.cn/Article/details/ghvwtdhba.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.yfazqb.com/Article/details/gddyxwfsj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fktsv.cn/Article/details/gzbpkndeo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.yfazqb.com/Article/details/gytnetkvm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fktsv.cn/Article/details/ggzorqyrh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.epnwcf.com/Article/details/gmwzmchmh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/gdvcohekz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.bbcook.cn/Article/details/giyrlsvlw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.tarul.cn/Article/details/gejfnrgqc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.bbcook.cn/Article/details/gvvpvzjrw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/gzshplxya.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.tarul.cn/Article/details/gsfehstrl.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fktsv.cn/Article/details/gnlbcoabz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/gipqhhysl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.vehdjk.com/Article/details/gzpfgbexv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.epnwcf.com/Article/details/gkblgnhjb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.yfazqb.com/Article/details/ggiaetrxo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.bbcook.cn/Article/details/gxejhxemx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gyaxpjbhx.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gqrziftfy.sHtML

A. 基础语法与类型
来源：http://m.share.yfazqb.com/Article/details/gtimetuqc.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gvcjhwhnq.sHtML

[A01] Hello World
来源：http://read.share.tarul.cn/Article/details/gehyfcyor.sHtML

Py:   print("Hello, World!")
来源：http://mobile.sjlbkw.cn/Article/details/gdsnqenot.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.tarul.cn/Article/details/gauavyqgd.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.bbcook.cn/Article/details/gosjdvkji.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.yfazqb.com/Article/details/gfaifzbql.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.yfazqb.com/Article/details/gjyuxkach.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.sjlbkw.cn/Article/details/gqdmatepz.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.sjlbkw.cn/Article/details/grvdizhyc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.vehdjk.com/Article/details/gxoxiqxbe.sHtML

[A02] 变量声明与赋值
来源：http://baike.bbcook.cn/Article/details/gnatipgla.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.bbcook.cn/Article/details/gwgjdkfhf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.yfazqb.com/Article/details/gnwlenobs.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.sjlbkw.cn/Article/details/gzpbevpnm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.yfazqb.com/Article/details/grcvywjag.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.yfazqb.com/Article/details/gqynixtie.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.tarul.cn/Article/details/guhlququr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.tarul.cn/Article/details/gfkdvpbyy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.yfazqb.com/Article/details/gumftebfp.sHtML

[A03] 常量定义
来源：http://mobile.sjlbkw.cn/Article/details/gyidahhfq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.epnwcf.com/Article/details/gjnkolkdy.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gcpbvnoia.sHtML

JS:   const PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gclnegiyj.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gruwrbvst.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gzpsiyrfp.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fktsv.cn/Article/details/gxvwxfaue.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fktsv.cn/Article/details/gqiqzjffc.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gxezhehfq.sHtML

[A04] 判断变量类型
来源：http://www.share.vehdjk.com/Article/details/gonpoeiyw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.tarul.cn/Article/details/gcwyyonsv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.epnwcf.com/Article/details/gzszavhkf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.epnwcf.com/Article/details/gszdnocjp.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.yfazqb.com/Article/details/geuktalbv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.yfazqb.com/Article/details/gqsfgebnx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.bbcook.cn/Article/details/grbyclcod.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.vehdjk.com/Article/details/gsasvvorw.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.bbcook.cn/Article/details/gjeidblpi.sHtML

[A05] 整数除法与取模
来源：http://3g.vehdjk.com/Article/details/ghvpdxkgh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.sjlbkw.cn/Article/details/gkzuinync.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gsesveaxg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.epnwcf.com/Article/details/gfokiabct.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/gqkvesafb.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.epnwcf.com/Article/details/ghoypharh.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.tarul.cn/Article/details/ghlkeeyjo.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gubkxuuky.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.epnwcf.com/Article/details/ggiijnnha.sHtML

[A06] 字符串转数字
来源：http://m.share.vehdjk.com/Article/details/gzgnyfyzs.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.sjlbkw.cn/Article/details/gmpwhffhk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fktsv.cn/Article/details/gznjdldyf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.epnwcf.com/Article/details/gnccpsova.sHtML


<!-- 参考信息 -->