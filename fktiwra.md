代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.blog.epnwcf.com/Article/details/gzerezdis.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.yfazqb.com/Article/details/gaepnsoxc.sHtML

[U46] PHP：可空类型
来源：http://read.share.bbcook.cn/Article/details/gbaubaqbi.sHtML

?string $name = null
来源：http://read.share.yfazqb.com/Article/details/glhlshtcd.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fktsv.cn/Article/details/gmnhfnnvx.sHtML

int|string $id
来源：http://baike.vehdjk.com/Article/details/gxoysykoc.sHtML

[U48] PHP：纯枚举
来源：http://read.share.yfazqb.com/Article/details/grpprcaoo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.epnwcf.com/Article/details/gjxijxoxu.sHtML

[U49] PHP：只读属性
来源：http://baike.yfazqb.com/Article/details/gnhelvjhg.sHtML

public readonly string $name
来源：http://baike.yfazqb.com/Article/details/gqbjdtlsq.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fktsv.cn/Article/details/gzxykezbz.sHtML

public function __construct(private int $id) {}
来源：http://3g.vehdjk.com/Article/details/gdwhbbavv.sHtML

[U51] PHP：数组解构
来源：http://3g.tarul.cn/Article/details/gdvxgslot.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.bbcook.cn/Article/details/gwkvlfpeo.sHtML

[U52] PHP：箭头函数
来源：http://3g.yfazqb.com/Article/details/gjohbqpta.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.epnwcf.com/Article/details/gajlpkbue.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.bbcook.cn/Article/details/gjgicaqgh.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.yfazqb.com/Article/details/gwwmerbry.sHtML

[U54] PHP：空安全调用
来源：http://m.share.sjlbkw.cn/Article/details/grcjilpll.sHtML

$obj?->method()
来源：http://3g.yfazqb.com/Article/details/gkhtanmqg.sHtML

[U55] PHP：match 表达式
来源：http://blog.vehdjk.com/Article/details/ghgalnmbh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.vehdjk.com/Article/details/gysaorkxs.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gavjclrot.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/gumvqjlxc.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gmhpwafdr.sHtML

"值: {$a}"
来源：http://www.m.share.tarul.cn/Article/details/ggtqnjtaj.sHtML

[U58] PHP：数组三件套
来源：http://read.share.bbcook.cn/Article/details/gerxyuxhg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gpkboecqb.sHtML

[U59] PHP：自定义排序
来源：http://mobile.sjlbkw.cn/Article/details/gjjnauhvc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.tarul.cn/Article/details/gvtyviqyh.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.bbcook.cn/Article/details/gaztoqbdi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.bbcook.cn/Article/details/gloepkgbj.sHtML

[U61] PHP：正则
来源：http://mobile.epnwcf.com/Article/details/gsjnzinnx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.epnwcf.com/Article/details/gupyosdxt.sHtML

[U62] PHP：日期对象
来源：http://www.share.fktsv.cn/Article/details/gywwvbqyq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fktsv.cn/Article/details/gyblmpcqa.sHtML

[U63] PHP：文件读写
来源：http://www.blog.epnwcf.com/Article/details/glinjyosq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.epnwcf.com/Article/details/gkgwkhihl.sHtML

[U64] PHP：目录遍历
来源：http://m.share.epnwcf.com/Article/details/gqiopukgy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.vehdjk.com/Article/details/gcwtcoajj.sHtML

[U65] PHP：会话
来源：http://www.m.share.epnwcf.com/Article/details/gxhlwfiov.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gzervztds.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.vehdjk.com/Article/details/goetovodx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.vehdjk.com/Article/details/gscjgtvtm.sHtML

[U67] PHP：处理文件上传
来源：http://blog.vehdjk.com/Article/details/glhtsknbo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.yfazqb.com/Article/details/gdwlmyiql.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.sjlbkw.cn/Article/details/gkzbpwqep.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.bbcook.cn/Article/details/gvrbqiiax.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.vehdjk.com/Article/details/grjmeujpo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.bbcook.cn/Article/details/gibrkrcjs.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.bbcook.cn/Article/details/gubgnvmfm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.vehdjk.com/Article/details/gguovgtge.sHtML

[U71] PHP：抛出异常
来源：http://www.share.tarul.cn/Article/details/gzbldqtcb.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.epnwcf.com/Article/details/gzhbytfys.sHtML

[U72] PHP：写错误日志
来源：http://3g.tarul.cn/Article/details/gwhsvpoqr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.tarul.cn/Article/details/gxlevccwh.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.epnwcf.com/Article/details/gphsghwfy.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.epnwcf.com/Article/details/ggmfhzfug.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gskhiessm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.tarul.cn/Article/details/gteofxtqt.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.bbcook.cn/Article/details/gkaahyiky.sHtML

composer require psr/container
来源：http://baike.sjlbkw.cn/Article/details/gxdwwuefk.sHtML

[U76] PHP：简单路由
来源：http://m.share.tarul.cn/Article/details/gctqrrfwz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.vehdjk.com/Article/details/gpyboqjbh.sHtML

[U77] PHP：模板渲染
来源：http://3g.yfazqb.com/Article/details/gcmygchvz.sHtML

composer require twig/twig
来源：http://baike.vehdjk.com/Article/details/gvugyowle.sHtML

[U78] PHP：单元测试
来源：http://www.share.tarul.cn/Article/details/gscvccqht.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.yfazqb.com/Article/details/gpanwjexz.sHtML

[U79] PHP：静态分析
来源：http://blog.fktsv.cn/Article/details/gyjlikkbi.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.sjlbkw.cn/Article/details/gqfgraoxu.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.vehdjk.com/Article/details/gxijootwa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.yfazqb.com/Article/details/giroczphk.sHtML

[U81] JS：初始化项目
来源：http://wap.yfazqb.com/Article/details/gtcywwpiw.sHtML

npm init -y;  npm i express
来源：http://3g.yfazqb.com/Article/details/gizammned.sHtML

[U82] JS：package.json 脚本
来源：http://baike.bbcook.cn/Article/details/ggcwpgnnq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.sjlbkw.cn/Article/details/govrmsncc.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.bbcook.cn/Article/details/gkrjdodxs.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.yfazqb.com/Article/details/gefpglpye.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.tarul.cn/Article/details/gyqgxdvqm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.epnwcf.com/Article/details/gtolmfggb.sHtML

[U85] JS：可选链
来源：http://www.blog.epnwcf.com/Article/details/ggieaejxh.sHtML

a?.b?.c
来源：http://3g.yfazqb.com/Article/details/gkeeylyli.sHtML

[U86] JS：空值合并
来源：http://blog.epnwcf.com/Article/details/gmzmovcbe.sHtML

a ?? b
来源：http://wap.yfazqb.com/Article/details/grmojadav.sHtML

[U87] JS：解构默认值
来源：http://www.share.bbcook.cn/Article/details/gmnokillw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.bbcook.cn/Article/details/gwgihacgq.sHtML

[U88] JS：对象展开合并
来源：http://read.share.epnwcf.com/Article/details/gezkuzfua.sHtML

{ ...a, ...b }
来源：http://read.share.yfazqb.com/Article/details/guukiensx.sHtML

[U89] JS：数组去重
来源：http://www.share.bbcook.cn/Article/details/gavteyini.sHtML

[...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/ggajuidpq.sHtML

[U90] JS：数字数组排序
来源：http://read.share.epnwcf.com/Article/details/gblnjlnlu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/ggxbdwfzs.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fktsv.cn/Article/details/gktwheeet.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmmnnmwm.sHtML

[U92] JS：深拷贝
来源：http://wap.epnwcf.com/Article/details/gkgrtyvvm.sHtML

structuredClone(obj)
来源：http://mobile.tarul.cn/Article/details/gpdiufosh.sHtML

[U93] JS：模板字符串
来源：http://mobile.yfazqb.com/Article/details/gqqojjjrj.sHtML

`共 ${n} 条`
来源：http://wap.bbcook.cn/Article/details/gxwhnnhrw.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.tarul.cn/Article/details/gkqsitmwb.sHtML

const double = x => x * 2;
来源：http://www.m.share.epnwcf.com/Article/details/gqgxyajrh.sHtML

[U95] JS：Promise 包装
来源：http://baike.bbcook.cn/Article/details/gkidblegh.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.yfazqb.com/Article/details/gveuurzdk.sHtML

[U96] JS：async/await 与异常
来源：http://3g.bbcook.cn/Article/details/gitzmbgpd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/ggfxoarug.sHtML

[U97] JS：并发请求
来源：http://www.share.vehdjk.com/Article/details/gklytqvak.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/gcwslshbx.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.tarul.cn/Article/details/goqgploez.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.bbcook.cn/Article/details/gpdkxajib.sHtML

[U99] JS：事件监听
来源：http://blog.epnwcf.com/Article/details/gbzsvqfms.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.yfazqb.com/Article/details/gmobjtnvg.sHtML

[U100] JS：DOM 查询
来源：http://3g.tarul.cn/Article/details/gqhzygmkl.sHtML

document.querySelector(".item")
来源：http://mobile.bbcook.cn/Article/details/gsmwemjkh.sHtML

[U101] JS：classList 操作
来源：http://mobile.vehdjk.com/Article/details/gfavwjzxp.sHtML

el.classList.toggle("active")
来源：http://wap.epnwcf.com/Article/details/gijubtmgl.sHtML

[U102] JS：本地存储
来源：http://www.blog.sjlbkw.cn/Article/details/gcatstmlv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.sjlbkw.cn/Article/details/gxhefqlpp.sHtML

[U103] JS：定时器
来源：http://wap.epnwcf.com/Article/details/gtbmarqwt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.sjlbkw.cn/Article/details/ggzdceaxc.sHtML

[U104] JS：防抖
来源：http://mobile.epnwcf.com/Article/details/gxmifuzin.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/grazeorzr.sHtML

[U105] JS：节流
来源：http://3g.fktsv.cn/Article/details/ggvsskuof.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.vehdjk.com/Article/details/gfwgghbrc.sHtML

[U106] JS：日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/gfadmdvof.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.yfazqb.com/Article/details/gcbxjrdzl.sHtML

[U107] JS：数字千分位
来源：http://blog.bbcook.cn/Article/details/geqmkdnur.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.vehdjk.com/Article/details/gytzwpwff.sHtML

[U108] JS：随机整数
来源：http://wap.tarul.cn/Article/details/gccpasjbi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.epnwcf.com/Article/details/gmfwhkvpw.sHtML

[U109] JS：数组分组
来源：http://read.share.epnwcf.com/Article/details/gkspobbax.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.yfazqb.com/Article/details/grywrsatk.sHtML

[U110] JS：数组分块
来源：http://3g.tarul.cn/Article/details/gdwlsjxrw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.sjlbkw.cn/Article/details/gcljrntil.sHtML

[U111] JS：对象转 Map
来源：http://baike.sjlbkw.cn/Article/details/gkpkqgoyt.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fktsv.cn/Article/details/gxnnjuvtf.sHtML

[U112] JS：字符串补位
来源：http://blog.epnwcf.com/Article/details/gcfnijcxj.sHtML

"7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/glhfkvlnb.sHtML

[U113] JS：正则替换全部
来源：http://read.share.sjlbkw.cn/Article/details/gpurqngeh.sHtML

s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gjduvckft.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fktsv.cn/Article/details/gfxlgisqh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.vehdjk.com/Article/details/ggycpxbxm.sHtML

[U115] JS：生成 UUID
来源：http://wap.tarul.cn/Article/details/gpexbnnfs.sHtML

crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gyimpaczg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.sjlbkw.cn/Article/details/gvhdlgrlf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/glowvijld.sHtML

[U117] JS：单元测试
来源：http://3g.sjlbkw.cn/Article/details/gjcyfmjte.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.vehdjk.com/Article/details/gaegvlgid.sHtML

[U118] JS：开发服务器
来源：http://read.share.yfazqb.com/Article/details/gntoilfvr.sHtML

npm i -D vite;  npx vite
来源：http://blog.sjlbkw.cn/Article/details/gngnlriwp.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fktsv.cn/Article/details/gghnrhewm.sHtML

npx vite build
来源：http://wap.fktsv.cn/Article/details/gjhitdqyc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.bbcook.cn/Article/details/gkvggahip.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.tarul.cn/Article/details/gvysnjpvy.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gqicmhrtc.sHtML

统计汇总
来源：http://mobile.tarul.cn/Article/details/ggtzfvrfo.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gydznhbbw.sHtML

按语言统计（条）：
来源：http://m.share.tarul.cn/Article/details/gqwzjammi.sHtML

Python ......... 252
来源：http://baike.vehdjk.com/Article/details/guutudbwm.sHtML

PHP ............ 252
来源：http://baike.epnwcf.com/Article/details/gvqrxbskw.sHtML

JavaScript ..... 252
来源：http://m.share.vehdjk.com/Article/details/ghdlwykfl.sHtML

TypeScript ..... 212
来源：http://www.share.bbcook.cn/Article/details/gaimeqoqe.sHtML

Java ........... 212
来源：http://www.share.sjlbkw.cn/Article/details/gurprxnys.sHtML

Go ............. 212
来源：http://mobile.epnwcf.com/Article/details/gjjejbbfu.sHtML

Ruby ........... 212
来源：http://www.blog.sjlbkw.cn/Article/details/gfxgmdyht.sHtML

C# ............. 212
来源：http://3g.vehdjk.com/Article/details/gxkdrikko.sHtML

C .............. 30
来源：http://read.share.sjlbkw.cn/Article/details/gceukrsxd.sHtML

C++ ............ 30
来源：http://mobile.tarul.cn/Article/details/gkdoanaua.sHtML

SQL ............ 90
来源：http://m.share.epnwcf.com/Article/details/gjwnwekml.sHtML

Bash ........... 80
来源：http://wap.yfazqb.com/Article/details/gdohxumdm.sHtML

Kotlin ......... 15
来源：http://mobile.epnwcf.com/Article/details/gtsdsiiho.sHtML

Swift .......... 15
来源：http://m.share.epnwcf.com/Article/details/gqdxlxmcd.sHtML

Lua ............ 10
来源：http://mobile.bbcook.cn/Article/details/gdnmfsejz.sHtML

Perl ........... 10
来源：http://www.blog.fktsv.cn/Article/details/gbdtskdsq.sHtML

Scala .......... 10
来源：http://www.m.share.yfazqb.com/Article/details/gfvotyijo.sHtML

------------------------------------
来源：http://baike.fktsv.cn/Article/details/ghtfbvauz.sHtML

合计 ........... 2106 条
来源：http://3g.vehdjk.com/Article/details/gahujkbop.sHtML

按章节统计：
来源：http://read.share.bbcook.cn/Article/details/groocakqo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.tarul.cn/Article/details/girbxskcc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/gvzkcuvzh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fktsv.cn/Article/details/guwltsnwj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.tarul.cn/Article/details/gjvbaemme.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.yfazqb.com/Article/details/gnslugngz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.vehdjk.com/Article/details/gttrqtxlr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fktsv.cn/Article/details/glexnrurv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.vehdjk.com/Article/details/gyqycgnky.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gzhicsume.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.epnwcf.com/Article/details/gklztlrrh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gmuhzslrn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/geuscpawy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/gyaxsiwhs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.yfazqb.com/Article/details/grtpukeif.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.tarul.cn/Article/details/gnuiykfsd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/gygqvwfen.sHtML

Q SQL 专题                              90
来源：http://3g.sjlbkw.cn/Article/details/gisnnaqut.sHtML

R Bash 专题                             80
来源：http://mobile.sjlbkw.cn/Article/details/gzdrumcag.sHtML

S C / C++ 专题                          60
来源：http://baike.epnwcf.com/Article/details/gbtxmomkw.sHtML

T 其他语言补充                          60
来源：http://3g.vehdjk.com/Article/details/gxhtboacj.sHtML

U 高频实用片段                         120
来源：http://m.share.bbcook.cn/Article/details/grzmkolwu.sHtML

------------------------------------
来源：http://read.share.vehdjk.com/Article/details/griaewvuy.sHtML

合计                                  2106 条
来源：http://blog.tarul.cn/Article/details/guixoztky.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.yfazqb.com/Article/details/gucdcmdih.sHtML

使用提醒
来源：http://www.blog.tarul.cn/Article/details/ggbtcilcf.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.tarul.cn/Article/details/gpfggezsv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.epnwcf.com/Article/details/gqnkqqvif.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.yfazqb.com/Article/details/ghdfiywtg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.vehdjk.com/Article/details/gecxftzps.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.yfazqb.com/Article/details/gypydrjed.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.vehdjk.com/Article/details/gffvnmyum.sHtML

—— 文件结束 ——
来源：http://blog.bbcook.cn/Article/details/gyhzdekol.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gjmoyviph.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.vehdjk.com/Article/details/gmigjaewn.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.vehdjk.com/Article/details/goazhfllw.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gbemufsmd.sHtML

【收录内容】
来源：http://www.blog.fktsv.cn/Article/details/gmulymiic.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.bbcook.cn/Article/details/gryfocyzn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.sjlbkw.cn/Article/details/gvwajwjmz.sHtML

SQL · Bash · C · C++
来源：http://wap.vehdjk.com/Article/details/gwwtsqgvc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fktsv.cn/Article/details/gbsyzvotr.sHtML

【使用说明】
来源：http://wap.yfazqb.com/Article/details/gnklfdscw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.vehdjk.com/Article/details/gakskfqjg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.epnwcf.com/Article/details/guawyoeah.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.yfazqb.com/Article/details/gnmuisohk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.bbcook.cn/Article/details/gvpnlpmzt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.tarul.cn/Article/details/gwqzngsbz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.epnwcf.com/Article/details/gjcbpuhgh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.sjlbkw.cn/Article/details/gzocdnjma.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.sjlbkw.cn/Article/details/gbymyoqlp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.yfazqb.com/Article/details/gjsrcejaz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fktsv.cn/Article/details/gxsnddazq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fktsv.cn/Article/details/gryavyvaf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.tarul.cn/Article/details/gzctbfaxu.sHtML

【文件统计】
来源：http://read.share.yfazqb.com/Article/details/glpfkseck.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.yfazqb.com/Article/details/ggqlmgcpj.sHtML

--------------------------------------------------------------------------------
来源：http://3g.bbcook.cn/Article/details/gxkogqhdf.sHtML

目  录
来源：http://3g.bbcook.cn/Article/details/gpakfxpdn.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gcrhwcqbi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.bbcook.cn/Article/details/gsfbjxbfx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.vehdjk.com/Article/details/gqlttlwmg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/gtlyffevh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gedirtpgo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.sjlbkw.cn/Article/details/guzsdlxzr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.yfazqb.com/Article/details/gbdkgfitk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.bbcook.cn/Article/details/gbqtizvjs.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.yfazqb.com/Article/details/gjmukihga.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/gvwgbatww.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.sjlbkw.cn/Article/details/gvrvbzktr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/gdynyvjpm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.yfazqb.com/Article/details/gwmfwskgs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gmoltqvjj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.bbcook.cn/Article/details/gmdjoxxnp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.yfazqb.com/Article/details/gpnrtpjgo.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/ghumhqyuo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fktsv.cn/Article/details/gvqrgqbog.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.vehdjk.com/Article/details/galjcjcqa.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fktsv.cn/Article/details/gvxqftorp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/gunlmjhgl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbvzcxtw.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gqwzhypiu.sHtML

A. 基础语法与类型
来源：http://read.share.tarul.cn/Article/details/gusguyjuo.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ggipkpqgr.sHtML

[A01] Hello World
来源：http://baike.fktsv.cn/Article/details/gzvgzujfa.sHtML

Py:   print("Hello, World!")
来源：http://www.share.yfazqb.com/Article/details/gchiwwguj.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.tarul.cn/Article/details/gcpkhcfor.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.epnwcf.com/Article/details/gjlammxbw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.vehdjk.com/Article/details/gevyseppi.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.sjlbkw.cn/Article/details/gfvunqbzv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.tarul.cn/Article/details/gkubkejjr.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.sjlbkw.cn/Article/details/gbdqxzlgb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.sjlbkw.cn/Article/details/garmhvtyk.sHtML

[A02] 变量声明与赋值
来源：http://3g.tarul.cn/Article/details/geduwcxqt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.bbcook.cn/Article/details/gypvtgmic.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.sjlbkw.cn/Article/details/gzvgsdjwx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.bbcook.cn/Article/details/gcyackcbp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.tarul.cn/Article/details/gxzouztmg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.sjlbkw.cn/Article/details/gylwrpima.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.yfazqb.com/Article/details/gurrnvhgs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.bbcook.cn/Article/details/gbxygqrhx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fktsv.cn/Article/details/gcsrulnng.sHtML

[A03] 常量定义
来源：http://www.m.share.tarul.cn/Article/details/gibktvzfr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.vehdjk.com/Article/details/ghhfgnanw.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gcryfsmlf.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gugicbliu.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gahbshtok.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gdlcahjld.sHtML

Go:   const PI = 3.14159
来源：http://read.share.bbcook.cn/Article/details/gjmhehbgo.sHtML

Ruby: PI = 3.14159
来源：http://baike.sjlbkw.cn/Article/details/gbmmgmyru.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gcyjlcobr.sHtML

[A04] 判断变量类型
来源：http://wap.bbcook.cn/Article/details/gcbeuejtp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.yfazqb.com/Article/details/goqatndds.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.tarul.cn/Article/details/gqdkvgzjv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.vehdjk.com/Article/details/glnmzhosv.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.yfazqb.com/Article/details/guygtbrvt.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.sjlbkw.cn/Article/details/glvtcmtqu.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.tarul.cn/Article/details/gmnpbdviw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.yfazqb.com/Article/details/grjxxevaq.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.vehdjk.com/Article/details/gtsexljxi.sHtML

[A05] 整数除法与取模
来源：http://www.blog.vehdjk.com/Article/details/gcozwhqbr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.sjlbkw.cn/Article/details/gahvrcbez.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.vehdjk.com/Article/details/gjygfzkyr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/goyyckfda.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.vehdjk.com/Article/details/gsrggvweh.sHtML


<!-- 参考信息 -->