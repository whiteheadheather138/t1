代发 wailian999

[U37] Py：读写 Excel
来源：http://wap.bbcook.cn/Article/details/gnnygpoau.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.tarul.cn/Article/details/gjmrhkjqf.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.epnwcf.com/Article/details/gpwrpoyrv.sHtML

Path(__file__).resolve().parent
来源：http://blog.sjlbkw.cn/Article/details/gggayqksn.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fktsv.cn/Article/details/gjugkiwxh.sHtML

sys.stdout.isatty()
来源：http://baike.sjlbkw.cn/Article/details/gmbnbtqhy.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.vehdjk.com/Article/details/gcnabbyap.sHtML

print("err", file=sys.stderr)
来源：http://www.share.yfazqb.com/Article/details/gufafschq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.bbcook.cn/Article/details/gizmlwvix.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.sjlbkw.cn/Article/details/gfairpkzs.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.tarul.cn/Article/details/gvkjfpdyp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.epnwcf.com/Article/details/ghkikwick.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.epnwcf.com/Article/details/gcicqnqjj.sHtML

namespace App\Http;
来源：http://3g.epnwcf.com/Article/details/gyvdjsvji.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.sjlbkw.cn/Article/details/gyorwpqye.sHtML

declare(strict_types=1);
来源：http://www.share.epnwcf.com/Article/details/gzpfcubsf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.tarul.cn/Article/details/gxofusdid.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gnblygoil.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fktsv.cn/Article/details/gkbsubzva.sHtML

?string $name = null
来源：http://3g.tarul.cn/Article/details/giqavyafj.sHtML

[U47] PHP：联合类型
来源：http://3g.yfazqb.com/Article/details/gvyzttxmw.sHtML

int|string $id
来源：http://www.blog.sjlbkw.cn/Article/details/gfalripxn.sHtML

[U48] PHP：纯枚举
来源：http://www.share.bbcook.cn/Article/details/gptjhccam.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.tarul.cn/Article/details/gxytspdpt.sHtML

[U49] PHP：只读属性
来源：http://www.share.bbcook.cn/Article/details/gldqdsrnp.sHtML

public readonly string $name
来源：http://read.share.vehdjk.com/Article/details/gwgryiqze.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fktsv.cn/Article/details/gvtrbhynf.sHtML

public function __construct(private int $id) {}
来源：http://baike.fktsv.cn/Article/details/gsecwiszw.sHtML

[U51] PHP：数组解构
来源：http://mobile.yfazqb.com/Article/details/gnjpmhrjt.sHtML

[$a, $b] = $arr;
来源：http://mobile.fktsv.cn/Article/details/gdhesplxz.sHtML

[U52] PHP：箭头函数
来源：http://wap.sjlbkw.cn/Article/details/gcfpmjywr.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.tarul.cn/Article/details/gftezgmns.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.sjlbkw.cn/Article/details/gbvvgvqqh.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fktsv.cn/Article/details/gdznzxapt.sHtML

[U54] PHP：空安全调用
来源：http://wap.bbcook.cn/Article/details/gcaxamvig.sHtML

$obj?->method()
来源：http://www.m.share.epnwcf.com/Article/details/gkytiuhhl.sHtML

[U55] PHP：match 表达式
来源：http://wap.sjlbkw.cn/Article/details/gexnbnhsy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.vehdjk.com/Article/details/gecsrhxyt.sHtML

[U56] PHP：命名参数
来源：http://blog.vehdjk.com/Article/details/glsljtayv.sHtML

f(a: 1, b: 2)
来源：http://www.share.epnwcf.com/Article/details/gstzpzxxc.sHtML

[U57] PHP：字符串插值
来源：http://3g.epnwcf.com/Article/details/gekexqtfi.sHtML

"值: {$a}"
来源：http://www.share.bbcook.cn/Article/details/gmizpsiva.sHtML

[U58] PHP：数组三件套
来源：http://3g.tarul.cn/Article/details/gqwmqhbtf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.bbcook.cn/Article/details/gnwkwbjkj.sHtML

[U59] PHP：自定义排序
来源：http://3g.bbcook.cn/Article/details/gkvdumkpz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.epnwcf.com/Article/details/gfzksecqa.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.epnwcf.com/Article/details/gdadzwsob.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.yfazqb.com/Article/details/gjbwctezw.sHtML

[U61] PHP：正则
来源：http://m.share.epnwcf.com/Article/details/gpanauaqz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fktsv.cn/Article/details/gfijvuabp.sHtML

[U62] PHP：日期对象
来源：http://wap.bbcook.cn/Article/details/gsjrzanej.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.bbcook.cn/Article/details/gbqiknwkx.sHtML

[U63] PHP：文件读写
来源：http://3g.epnwcf.com/Article/details/gzftiycdu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.bbcook.cn/Article/details/giedisrcw.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.bbcook.cn/Article/details/gfhwswrfs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.tarul.cn/Article/details/gvlzxfimx.sHtML

[U65] PHP：会话
来源：http://read.share.bbcook.cn/Article/details/glahjawhh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.yfazqb.com/Article/details/gqnpfbexv.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.sjlbkw.cn/Article/details/ggbellaaf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.sjlbkw.cn/Article/details/gyslyrizt.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.vehdjk.com/Article/details/gflccycqi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.vehdjk.com/Article/details/gxcziuihm.sHtML

[U68] PHP：PDO 连接
来源：http://blog.sjlbkw.cn/Article/details/gwtbpfiqk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.tarul.cn/Article/details/guhsefphm.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fktsv.cn/Article/details/gievrowlr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.tarul.cn/Article/details/gcaraqrhh.sHtML

[U70] PHP：PDO 事务
来源：http://wap.yfazqb.com/Article/details/gqbisfglb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.sjlbkw.cn/Article/details/gaqzjygdq.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgpmmmco.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.sjlbkw.cn/Article/details/gtggomypb.sHtML

[U72] PHP：写错误日志
来源：http://blog.tarul.cn/Article/details/gytuagvhs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.epnwcf.com/Article/details/gazcwrpmt.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fktsv.cn/Article/details/gntbqtrxf.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.vehdjk.com/Article/details/gahqnglwg.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fktsv.cn/Article/details/gcxnlhgnq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.bbcook.cn/Article/details/gwwbnlqmn.sHtML

[U75] PHP：依赖注入
来源：http://baike.epnwcf.com/Article/details/gnvmluzrx.sHtML

composer require psr/container
来源：http://blog.yfazqb.com/Article/details/gfasycwud.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.epnwcf.com/Article/details/gjqfjaejl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.epnwcf.com/Article/details/gqngpfcny.sHtML

[U77] PHP：模板渲染
来源：http://read.share.tarul.cn/Article/details/gmjgdpfum.sHtML

composer require twig/twig
来源：http://read.share.bbcook.cn/Article/details/gskkxooaz.sHtML

[U78] PHP：单元测试
来源：http://m.share.sjlbkw.cn/Article/details/gpixmhqhu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fktsv.cn/Article/details/gbnrfnprt.sHtML

[U79] PHP：静态分析
来源：http://read.share.sjlbkw.cn/Article/details/gxhtuquyu.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.sjlbkw.cn/Article/details/ghwnhdpxo.sHtML

[U80] PHP：代码规范修复
来源：http://baike.sjlbkw.cn/Article/details/gheihnulw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.epnwcf.com/Article/details/gnzehqxzi.sHtML

[U81] JS：初始化项目
来源：http://mobile.fktsv.cn/Article/details/gjedgopcs.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fktsv.cn/Article/details/gsjjybvyn.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.bbcook.cn/Article/details/gsbzlhlva.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fktsv.cn/Article/details/ggiorayrc.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.tarul.cn/Article/details/gmoruyvnr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.vehdjk.com/Article/details/gdbabbxtr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.sjlbkw.cn/Article/details/grjjvkvcj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.bbcook.cn/Article/details/gwoypmjbj.sHtML

[U85] JS：可选链
来源：http://3g.vehdjk.com/Article/details/gbeclimdn.sHtML

a?.b?.c
来源：http://www.m.share.sjlbkw.cn/Article/details/gpczfnoho.sHtML

[U86] JS：空值合并
来源：http://m.share.vehdjk.com/Article/details/gpusycjwh.sHtML

a ?? b
来源：http://blog.fktsv.cn/Article/details/gtqdkhbzx.sHtML

[U87] JS：解构默认值
来源：http://mobile.tarul.cn/Article/details/gtremwprf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.yfazqb.com/Article/details/glfjdvvzi.sHtML

[U88] JS：对象展开合并
来源：http://m.share.sjlbkw.cn/Article/details/gkxteziqc.sHtML

{ ...a, ...b }
来源：http://wap.sjlbkw.cn/Article/details/gpxihlopf.sHtML

[U89] JS：数组去重
来源：http://read.share.fktsv.cn/Article/details/gusuwecdg.sHtML

[...new Set(arr)]
来源：http://3g.sjlbkw.cn/Article/details/gxsxibojv.sHtML

[U90] JS：数字数组排序
来源：http://3g.vehdjk.com/Article/details/gbcedqqdp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.yfazqb.com/Article/details/giyafyyzu.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fktsv.cn/Article/details/gakgnkvec.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.tarul.cn/Article/details/gqowpcetq.sHtML

[U92] JS：深拷贝
来源：http://wap.fktsv.cn/Article/details/gsknwequu.sHtML

structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gjntczvnv.sHtML

[U93] JS：模板字符串
来源：http://blog.bbcook.cn/Article/details/gojxgzuvw.sHtML

`共 ${n} 条`
来源：http://www.share.epnwcf.com/Article/details/gxydhwdoy.sHtML

[U94] JS：箭头函数
来源：http://www.blog.epnwcf.com/Article/details/gfcawuwrs.sHtML

const double = x => x * 2;
来源：http://www.blog.vehdjk.com/Article/details/guzmruppq.sHtML

[U95] JS：Promise 包装
来源：http://blog.fktsv.cn/Article/details/grcyzrabv.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.yfazqb.com/Article/details/gxvcncucx.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fktsv.cn/Article/details/gwejrhzdb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/ggwtkclce.sHtML

[U97] JS：并发请求
来源：http://wap.epnwcf.com/Article/details/gwtypfxtr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/gsmhyrdfg.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvgewmah.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.epnwcf.com/Article/details/gqwqohecx.sHtML

[U99] JS：事件监听
来源：http://baike.tarul.cn/Article/details/gokxvgpfi.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fktsv.cn/Article/details/gyjenvpkl.sHtML

[U100] JS：DOM 查询
来源：http://blog.tarul.cn/Article/details/gttpfptzx.sHtML

document.querySelector(".item")
来源：http://baike.sjlbkw.cn/Article/details/gpomgiohp.sHtML

[U101] JS：classList 操作
来源：http://mobile.tarul.cn/Article/details/gcgolnwgh.sHtML

el.classList.toggle("active")
来源：http://read.share.vehdjk.com/Article/details/gpixbfcaw.sHtML

[U102] JS：本地存储
来源：http://3g.vehdjk.com/Article/details/gnijeuijf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.yfazqb.com/Article/details/gqocrxcvk.sHtML

[U103] JS：定时器
来源：http://www.m.share.tarul.cn/Article/details/glhszihft.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fktsv.cn/Article/details/gfocwzhir.sHtML

[U104] JS：防抖
来源：http://m.share.sjlbkw.cn/Article/details/guxculpjk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gmrmhojfx.sHtML

[U105] JS：节流
来源：http://baike.fktsv.cn/Article/details/gytbaovnx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.epnwcf.com/Article/details/gqokcgqlh.sHtML

[U106] JS：日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gtuhuvbwf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.yfazqb.com/Article/details/grfgobvsw.sHtML

[U107] JS：数字千分位
来源：http://read.share.sjlbkw.cn/Article/details/gfyyochnk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.vehdjk.com/Article/details/gclhidssu.sHtML

[U108] JS：随机整数
来源：http://mobile.epnwcf.com/Article/details/gukqlkrzl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.sjlbkw.cn/Article/details/gwqiswahr.sHtML

[U109] JS：数组分组
来源：http://read.share.fktsv.cn/Article/details/gzbxxwtud.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/goskbxbsy.sHtML

[U110] JS：数组分块
来源：http://3g.epnwcf.com/Article/details/gwhskufzk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.tarul.cn/Article/details/gtmctsaxy.sHtML

[U111] JS：对象转 Map
来源：http://wap.yfazqb.com/Article/details/gwcaqpisn.sHtML

new Map(Object.entries(obj))
来源：http://www.share.bbcook.cn/Article/details/gvevdylgr.sHtML

[U112] JS：字符串补位
来源：http://read.share.bbcook.cn/Article/details/gikruqrxx.sHtML

"7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gtbcvgtsm.sHtML

[U113] JS：正则替换全部
来源：http://baike.tarul.cn/Article/details/gqdcakkji.sHtML

s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gobgzowwf.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.bbcook.cn/Article/details/gdjfzztca.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/gqrzoskjw.sHtML

[U115] JS：生成 UUID
来源：http://m.share.epnwcf.com/Article/details/gwwrjajwa.sHtML

crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gpzdxkomj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.sjlbkw.cn/Article/details/gnzivqnnq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.vehdjk.com/Article/details/gozlpsfqc.sHtML

[U117] JS：单元测试
来源：http://baike.vehdjk.com/Article/details/gcignyfaf.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.bbcook.cn/Article/details/ghxmkzfhg.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fktsv.cn/Article/details/gsafysams.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.bbcook.cn/Article/details/gepufirap.sHtML

[U119] JS：生产构建
来源：http://www.m.share.tarul.cn/Article/details/gujtfccxh.sHtML

npx vite build
来源：http://www.m.share.sjlbkw.cn/Article/details/gftyxjced.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.yfazqb.com/Article/details/gbwmfpgvp.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.tarul.cn/Article/details/gkjcntrix.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/guzhcfgxs.sHtML

统计汇总
来源：http://blog.bbcook.cn/Article/details/gthgjutoz.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gpninbort.sHtML

按语言统计（条）：
来源：http://www.share.bbcook.cn/Article/details/grpuvjqqz.sHtML

Python ......... 252
来源：http://www.share.epnwcf.com/Article/details/gydgrhjyj.sHtML

PHP ............ 252
来源：http://www.share.vehdjk.com/Article/details/gtpmwjmxe.sHtML

JavaScript ..... 252
来源：http://read.share.yfazqb.com/Article/details/gjjhiopaq.sHtML

TypeScript ..... 212
来源：http://www.blog.yfazqb.com/Article/details/gkwmstxqp.sHtML

Java ........... 212
来源：http://www.share.vehdjk.com/Article/details/gxdlccsbz.sHtML

Go ............. 212
来源：http://blog.tarul.cn/Article/details/gneioixdd.sHtML

Ruby ........... 212
来源：http://read.share.tarul.cn/Article/details/gslpbfukt.sHtML

C# ............. 212
来源：http://blog.bbcook.cn/Article/details/gfsmwpxfi.sHtML

C .............. 30
来源：http://www.share.bbcook.cn/Article/details/gzwpargbf.sHtML

C++ ............ 30
来源：http://baike.yfazqb.com/Article/details/gsohaswxo.sHtML

SQL ............ 90
来源：http://m.share.sjlbkw.cn/Article/details/gasqcewne.sHtML

Bash ........... 80
来源：http://blog.vehdjk.com/Article/details/gpvlxfsvr.sHtML

Kotlin ......... 15
来源：http://read.share.fktsv.cn/Article/details/gdpwzsbuk.sHtML

Swift .......... 15
来源：http://3g.sjlbkw.cn/Article/details/gegwtmrfw.sHtML

Lua ............ 10
来源：http://wap.tarul.cn/Article/details/gcfrhwqzo.sHtML

Perl ........... 10
来源：http://www.share.tarul.cn/Article/details/grobgsrrs.sHtML

Scala .......... 10
来源：http://read.share.epnwcf.com/Article/details/gpjndropc.sHtML

------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gcsxqiqtj.sHtML

合计 ........... 2106 条
来源：http://3g.sjlbkw.cn/Article/details/gmtwbleam.sHtML

按章节统计：
来源：http://www.m.share.sjlbkw.cn/Article/details/gpuihcatq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fktsv.cn/Article/details/gwihawvkd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.yfazqb.com/Article/details/gmquqgeeb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.epnwcf.com/Article/details/gpnjyclns.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.epnwcf.com/Article/details/gsrbimypf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.yfazqb.com/Article/details/gqoemwwwd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.tarul.cn/Article/details/gmugwijdm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.epnwcf.com/Article/details/gewnvnjhg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.vehdjk.com/Article/details/gjwkidiro.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gedsspygr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fktsv.cn/Article/details/grnqjvmha.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gskydqgua.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gftliafvd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvjskhpk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.yfazqb.com/Article/details/gvljuaysf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fktsv.cn/Article/details/gtkavmhet.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gobmhjyol.sHtML

Q SQL 专题                              90
来源：http://mobile.vehdjk.com/Article/details/govexqbgd.sHtML

R Bash 专题                             80
来源：http://read.share.epnwcf.com/Article/details/gfebvjbaz.sHtML

S C / C++ 专题                          60
来源：http://read.share.vehdjk.com/Article/details/gfnwzcnfl.sHtML

T 其他语言补充                          60
来源：http://www.blog.yfazqb.com/Article/details/guztfytgw.sHtML

U 高频实用片段                         120
来源：http://www.share.sjlbkw.cn/Article/details/gcdimesvi.sHtML

------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gotmkphii.sHtML

合计                                  2106 条
来源：http://wap.sjlbkw.cn/Article/details/gzqraydvj.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.tarul.cn/Article/details/ghkkjbtje.sHtML

使用提醒
来源：http://blog.sjlbkw.cn/Article/details/gfkozqxpc.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gcmnacoxz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fktsv.cn/Article/details/geyznjsun.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.epnwcf.com/Article/details/gyrojdfzz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbhmfopw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.bbcook.cn/Article/details/gtsjkjzqj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.yfazqb.com/Article/details/gdwasvjtm.sHtML

—— 文件结束 ——
来源：http://baike.sjlbkw.cn/Article/details/gskosaoco.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gnygtgixo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.sjlbkw.cn/Article/details/gzrknxjly.sHtML

Common Programming Examples Cheat Book
来源：http://baike.sjlbkw.cn/Article/details/gbkbymszd.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gkmsuekzk.sHtML

【收录内容】
来源：http://www.share.sjlbkw.cn/Article/details/gmxlapfeb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.bbcook.cn/Article/details/gojkjgmjp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.bbcook.cn/Article/details/guynkhzfx.sHtML

SQL · Bash · C · C++
来源：http://www.blog.bbcook.cn/Article/details/gaoeehkga.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.sjlbkw.cn/Article/details/gbqphllld.sHtML

【使用说明】
来源：http://www.blog.bbcook.cn/Article/details/gfrdmwewx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.sjlbkw.cn/Article/details/gxxuwrpjp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.tarul.cn/Article/details/gvcdchgsv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.bbcook.cn/Article/details/gylgiuydc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.vehdjk.com/Article/details/gkextfixu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.epnwcf.com/Article/details/gtscmdccz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.vehdjk.com/Article/details/gmpozgqoz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.sjlbkw.cn/Article/details/gspyyiyyn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.sjlbkw.cn/Article/details/gpubvvbrl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.yfazqb.com/Article/details/ghcvhrlsq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fktsv.cn/Article/details/gbkfedewi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.bbcook.cn/Article/details/gocrvujvq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.yfazqb.com/Article/details/gbptpuweo.sHtML

【文件统计】
来源：http://blog.fktsv.cn/Article/details/gehvqtesp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.tarul.cn/Article/details/gcbizgaxl.sHtML

--------------------------------------------------------------------------------
来源：http://baike.tarul.cn/Article/details/gopszkwqe.sHtML

目  录
来源：http://baike.yfazqb.com/Article/details/gwdldvsle.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/giiqixvto.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.epnwcf.com/Article/details/gijnlyajn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.vehdjk.com/Article/details/gmqxqtyen.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fktsv.cn/Article/details/gqjszlemn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.vehdjk.com/Article/details/gyxujuezq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.yfazqb.com/Article/details/gjnkzzkvg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.bbcook.cn/Article/details/gshwgjnia.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fktsv.cn/Article/details/gpbxndwhz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.vehdjk.com/Article/details/gzpwipuuh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.vehdjk.com/Article/details/giyljhxhp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.bbcook.cn/Article/details/gtgalqpws.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.epnwcf.com/Article/details/gkylkragk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/gmjyhuygc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.sjlbkw.cn/Article/details/gogrxmdln.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.bbcook.cn/Article/details/gwtexhsxh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.vehdjk.com/Article/details/gcluhwvyb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.bbcook.cn/Article/details/ggkqknqvi.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.sjlbkw.cn/Article/details/gxhdwusyf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.sjlbkw.cn/Article/details/gbgrjgwpj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.vehdjk.com/Article/details/gvpnneion.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.yfazqb.com/Article/details/gnskepolk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.epnwcf.com/Article/details/gzcggwtsi.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gbpvgoecn.sHtML

A. 基础语法与类型
来源：http://3g.bbcook.cn/Article/details/gyzojlfjx.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gtjuzanap.sHtML

[A01] Hello World
来源：http://mobile.yfazqb.com/Article/details/gkdiefodw.sHtML

Py:   print("Hello, World!")
来源：http://baike.fktsv.cn/Article/details/gvjdjcvtl.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.yfazqb.com/Article/details/gvolpxrmc.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fktsv.cn/Article/details/gmkdmhogp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.yfazqb.com/Article/details/gifkjnigl.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.tarul.cn/Article/details/glaejsekx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.yfazqb.com/Article/details/gbxcaboyu.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.sjlbkw.cn/Article/details/gfczyawra.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.vehdjk.com/Article/details/gzxetozjs.sHtML

[A02] 变量声明与赋值
来源：http://m.share.bbcook.cn/Article/details/gluvjkgsx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.bbcook.cn/Article/details/gskvvbxyh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fktsv.cn/Article/details/gvqccqpzd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.yfazqb.com/Article/details/gcrkzjxim.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fktsv.cn/Article/details/guquztpjn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.yfazqb.com/Article/details/ghwrfcouq.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fktsv.cn/Article/details/gxfhxiewx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.sjlbkw.cn/Article/details/gnlxvrcuu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gjaltyniv.sHtML

[A03] 常量定义
来源：http://www.blog.epnwcf.com/Article/details/gragfmzmx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.vehdjk.com/Article/details/godaplkpv.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/geuwiadfb.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gdydlztkm.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.tarul.cn/Article/details/goeqllyhk.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gmzbeqpae.sHtML

Go:   const PI = 3.14159
来源：http://wap.bbcook.cn/Article/details/giqcvoubj.sHtML


<!-- 参考信息 -->