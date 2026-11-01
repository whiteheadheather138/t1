代发 wailian999

[U35] Py：发送邮件
来源：http://www.blog.tarul.cn/Article/details/glpjzwwum.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.epnwcf.com/Article/details/gasuganky.sHtML

[U36] Py：定时任务
来源：http://read.share.fktsv.cn/Article/details/gcnwlqdfh.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fktsv.cn/Article/details/gcrmxrpkr.sHtML

[U37] Py：读写 Excel
来源：http://wap.sjlbkw.cn/Article/details/gocdgmkqe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fktsv.cn/Article/details/gqaktgyyn.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.vehdjk.com/Article/details/getyfokzx.sHtML

Path(__file__).resolve().parent
来源：http://mobile.vehdjk.com/Article/details/gdvrdcvui.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.sjlbkw.cn/Article/details/gwsargxsk.sHtML

sys.stdout.isatty()
来源：http://read.share.vehdjk.com/Article/details/guxdfmqxi.sHtML

[U40] Py：打印到标准错误
来源：http://blog.yfazqb.com/Article/details/gxhthxzto.sHtML

print("err", file=sys.stderr)
来源：http://www.share.tarul.cn/Article/details/gjmnqmvpq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.yfazqb.com/Article/details/gvbffijin.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.vehdjk.com/Article/details/gwgpiewbo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fktsv.cn/Article/details/gvgvmogpl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fktsv.cn/Article/details/gxokyzacs.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.yfazqb.com/Article/details/gplufyoak.sHtML

namespace App\Http;
来源：http://baike.bbcook.cn/Article/details/gjyespflv.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.sjlbkw.cn/Article/details/gfnmgcbds.sHtML

declare(strict_types=1);
来源：http://read.share.epnwcf.com/Article/details/gcivktknr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.yfazqb.com/Article/details/ghfpeffie.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gveavtnqr.sHtML

[U46] PHP：可空类型
来源：http://baike.yfazqb.com/Article/details/gukhjtyjx.sHtML

?string $name = null
来源：http://mobile.bbcook.cn/Article/details/ggobmmccz.sHtML

[U47] PHP：联合类型
来源：http://read.share.epnwcf.com/Article/details/gvwvuyyrb.sHtML

int|string $id
来源：http://3g.epnwcf.com/Article/details/goxhnihxu.sHtML

[U48] PHP：纯枚举
来源：http://mobile.vehdjk.com/Article/details/gvocopwdu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fktsv.cn/Article/details/gntlcyobo.sHtML

[U49] PHP：只读属性
来源：http://www.share.tarul.cn/Article/details/gzbichxix.sHtML

public readonly string $name
来源：http://3g.fktsv.cn/Article/details/gqhwlogig.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.vehdjk.com/Article/details/gwsqxbuef.sHtML

public function __construct(private int $id) {}
来源：http://mobile.bbcook.cn/Article/details/gceaoxzxn.sHtML

[U51] PHP：数组解构
来源：http://read.share.sjlbkw.cn/Article/details/gwaxckrqi.sHtML

[$a, $b] = $arr;
来源：http://www.share.vehdjk.com/Article/details/gprqyjreh.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fktsv.cn/Article/details/gqpucpbzh.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.yfazqb.com/Article/details/gfqliqjqf.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.epnwcf.com/Article/details/gorssbbuu.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.bbcook.cn/Article/details/gesuciakb.sHtML

[U54] PHP：空安全调用
来源：http://www.share.vehdjk.com/Article/details/gfridvakt.sHtML

$obj?->method()
来源：http://m.share.tarul.cn/Article/details/gnfjboqwh.sHtML

[U55] PHP：match 表达式
来源：http://wap.epnwcf.com/Article/details/gduvuxfok.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.epnwcf.com/Article/details/gzyhmnsyq.sHtML

[U56] PHP：命名参数
来源：http://www.share.epnwcf.com/Article/details/gdamzfzok.sHtML

f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gnuvrsdec.sHtML

[U57] PHP：字符串插值
来源：http://m.share.tarul.cn/Article/details/ghthnyuwr.sHtML

"值: {$a}"
来源：http://baike.vehdjk.com/Article/details/gskphbqua.sHtML

[U58] PHP：数组三件套
来源：http://www.share.yfazqb.com/Article/details/gmfubxyam.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fktsv.cn/Article/details/gloqhcvnv.sHtML

[U59] PHP：自定义排序
来源：http://wap.vehdjk.com/Article/details/ggfenofnr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.yfazqb.com/Article/details/ghutcwodn.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.yfazqb.com/Article/details/glexfnygf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.bbcook.cn/Article/details/glavauyaz.sHtML

[U61] PHP：正则
来源：http://baike.yfazqb.com/Article/details/gtemdqrlc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.yfazqb.com/Article/details/guehrqsse.sHtML

[U62] PHP：日期对象
来源：http://read.share.bbcook.cn/Article/details/gugdvlpfx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.epnwcf.com/Article/details/ghhxaitku.sHtML

[U63] PHP：文件读写
来源：http://mobile.fktsv.cn/Article/details/gzzxlwcxq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.epnwcf.com/Article/details/gkazscrsx.sHtML

[U64] PHP：目录遍历
来源：http://m.share.bbcook.cn/Article/details/gmzhfkygy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.epnwcf.com/Article/details/gtxvoctwn.sHtML

[U65] PHP：会话
来源：http://mobile.tarul.cn/Article/details/gwhzfxeml.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.vehdjk.com/Article/details/grnreaawp.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.tarul.cn/Article/details/gcdvdkcgd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fktsv.cn/Article/details/gysszeswu.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.yfazqb.com/Article/details/gpjgclbjj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.yfazqb.com/Article/details/gbnbcobjq.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.bbcook.cn/Article/details/garscpvis.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.bbcook.cn/Article/details/goazmvfhe.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.tarul.cn/Article/details/gphxrxadl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.sjlbkw.cn/Article/details/gxmpnrnjp.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.sjlbkw.cn/Article/details/gemqrefyu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.tarul.cn/Article/details/gpwnkdwea.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fktsv.cn/Article/details/gaherwkvl.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.tarul.cn/Article/details/gwcxrdiyf.sHtML

[U72] PHP：写错误日志
来源：http://blog.bbcook.cn/Article/details/gvsldgbkq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.yfazqb.com/Article/details/gtvyuyuwp.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.sjlbkw.cn/Article/details/gjiyerglz.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.epnwcf.com/Article/details/gbnknuyca.sHtML

[U74] PHP：读取环境变量
来源：http://baike.yfazqb.com/Article/details/ghwtairpq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.sjlbkw.cn/Article/details/goluxzykv.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fktsv.cn/Article/details/ghgayxixx.sHtML

composer require psr/container
来源：http://m.share.yfazqb.com/Article/details/ghjnbpyoy.sHtML

[U76] PHP：简单路由
来源：http://m.share.fktsv.cn/Article/details/gbbubihyn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fktsv.cn/Article/details/genzqftfw.sHtML

[U77] PHP：模板渲染
来源：http://blog.yfazqb.com/Article/details/glhdgiisg.sHtML

composer require twig/twig
来源：http://www.blog.tarul.cn/Article/details/gechxceqy.sHtML

[U78] PHP：单元测试
来源：http://www.share.vehdjk.com/Article/details/glvwddvqu.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fktsv.cn/Article/details/gxkqurboz.sHtML

[U79] PHP：静态分析
来源：http://blog.vehdjk.com/Article/details/gwyvimols.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.vehdjk.com/Article/details/gddkozpgt.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fktsv.cn/Article/details/gdmxyhopc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.vehdjk.com/Article/details/gasqkxeyv.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.yfazqb.com/Article/details/gqukvkpls.sHtML

npm init -y;  npm i express
来源：http://blog.sjlbkw.cn/Article/details/gcwdeodhh.sHtML

[U82] JS：package.json 脚本
来源：http://3g.yfazqb.com/Article/details/gdqanqwgi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fktsv.cn/Article/details/guurkxwbc.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.yfazqb.com/Article/details/gsqinqxjs.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.vehdjk.com/Article/details/gstkgybkq.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.sjlbkw.cn/Article/details/gwnqhnpnf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fktsv.cn/Article/details/gxzofmdrh.sHtML

[U85] JS：可选链
来源：http://blog.bbcook.cn/Article/details/gbheciidw.sHtML

a?.b?.c
来源：http://3g.tarul.cn/Article/details/gzrvjvbsz.sHtML

[U86] JS：空值合并
来源：http://m.share.bbcook.cn/Article/details/gfdyfhpdl.sHtML

a ?? b
来源：http://3g.fktsv.cn/Article/details/gbkbinibj.sHtML

[U87] JS：解构默认值
来源：http://read.share.tarul.cn/Article/details/ghugijxci.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.tarul.cn/Article/details/gpxifdxzq.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fktsv.cn/Article/details/gkkasouuz.sHtML

{ ...a, ...b }
来源：http://mobile.tarul.cn/Article/details/ggwpzyrjo.sHtML

[U89] JS：数组去重
来源：http://read.share.tarul.cn/Article/details/gqsoiwgfd.sHtML

[...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gqibgjkgz.sHtML

[U90] JS：数字数组排序
来源：http://3g.vehdjk.com/Article/details/gssdhimrc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gmxoxxsbu.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.epnwcf.com/Article/details/gyuhoceow.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fktsv.cn/Article/details/gtgquqwpt.sHtML

[U92] JS：深拷贝
来源：http://www.share.bbcook.cn/Article/details/gynysgyeb.sHtML

structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gdfzgvyby.sHtML

[U93] JS：模板字符串
来源：http://blog.fktsv.cn/Article/details/gtgomcdgf.sHtML

`共 ${n} 条`
来源：http://blog.vehdjk.com/Article/details/grcfizbhp.sHtML

[U94] JS：箭头函数
来源：http://read.share.tarul.cn/Article/details/gkuijwqmf.sHtML

const double = x => x * 2;
来源：http://blog.sjlbkw.cn/Article/details/gwtuaefpo.sHtML

[U95] JS：Promise 包装
来源：http://read.share.sjlbkw.cn/Article/details/gonlxzoyc.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.epnwcf.com/Article/details/gmocouflh.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.yfazqb.com/Article/details/gxkrjxauo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/gitmbdxez.sHtML

[U97] JS：并发请求
来源：http://3g.sjlbkw.cn/Article/details/gumjqgyif.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gnbzzxkvu.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.tarul.cn/Article/details/gwnvcyrrn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.yfazqb.com/Article/details/gkeyvxxrw.sHtML

[U99] JS：事件监听
来源：http://3g.vehdjk.com/Article/details/grtwltbaw.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.sjlbkw.cn/Article/details/gxabvejwc.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fktsv.cn/Article/details/gbwjosksh.sHtML

document.querySelector(".item")
来源：http://read.share.fktsv.cn/Article/details/goabdoahm.sHtML

[U101] JS：classList 操作
来源：http://www.blog.bbcook.cn/Article/details/gckpwbwgy.sHtML

el.classList.toggle("active")
来源：http://baike.tarul.cn/Article/details/gekgfhefk.sHtML

[U102] JS：本地存储
来源：http://baike.epnwcf.com/Article/details/ghcsrciad.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.yfazqb.com/Article/details/gklltmirh.sHtML

[U103] JS：定时器
来源：http://www.share.epnwcf.com/Article/details/guvfshcun.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.epnwcf.com/Article/details/gwtkkblos.sHtML

[U104] JS：防抖
来源：http://3g.bbcook.cn/Article/details/gjvousgrq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/gtcgxwtif.sHtML

[U105] JS：节流
来源：http://www.blog.vehdjk.com/Article/details/gyuuueino.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fktsv.cn/Article/details/gwrxlmypv.sHtML

[U106] JS：日期格式化
来源：http://m.share.tarul.cn/Article/details/gcziyillv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.vehdjk.com/Article/details/gcxqovqgd.sHtML

[U107] JS：数字千分位
来源：http://3g.sjlbkw.cn/Article/details/gkxjnysib.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.yfazqb.com/Article/details/gtgwsnlzx.sHtML

[U108] JS：随机整数
来源：http://www.m.share.tarul.cn/Article/details/gyouskhgt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.tarul.cn/Article/details/gdwwjocnq.sHtML

[U109] JS：数组分组
来源：http://mobile.yfazqb.com/Article/details/gopysblec.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.bbcook.cn/Article/details/gckdhsmfp.sHtML

[U110] JS：数组分块
来源：http://www.m.share.vehdjk.com/Article/details/gbubfqixk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.vehdjk.com/Article/details/gzpuooogr.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fktsv.cn/Article/details/gemyanpek.sHtML

new Map(Object.entries(obj))
来源：http://www.share.bbcook.cn/Article/details/gyyrhngbr.sHtML

[U112] JS：字符串补位
来源：http://m.share.epnwcf.com/Article/details/gvxoiacty.sHtML

"7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/gejhdnqiu.sHtML

[U113] JS：正则替换全部
来源：http://m.share.vehdjk.com/Article/details/gdthjdiac.sHtML

s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/goejukxlv.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fktsv.cn/Article/details/gvjxrypco.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fktsv.cn/Article/details/gzarrlhvd.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fktsv.cn/Article/details/gmgdgpysd.sHtML

crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gqorbjvuf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.tarul.cn/Article/details/gepmiavnv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.yfazqb.com/Article/details/ggqsuiuhq.sHtML

[U117] JS：单元测试
来源：http://mobile.bbcook.cn/Article/details/gijwloawk.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.bbcook.cn/Article/details/gwkyvfbia.sHtML

[U118] JS：开发服务器
来源：http://www.share.epnwcf.com/Article/details/ggnylstcs.sHtML

npm i -D vite;  npx vite
来源：http://www.share.epnwcf.com/Article/details/glumdugwg.sHtML

[U119] JS：生产构建
来源：http://baike.fktsv.cn/Article/details/gdrigdcxl.sHtML

npx vite build
来源：http://read.share.bbcook.cn/Article/details/gwzjgxjad.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.bbcook.cn/Article/details/glfozveub.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.sjlbkw.cn/Article/details/gekqfflqq.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gflfhhdji.sHtML

统计汇总
来源：http://wap.fktsv.cn/Article/details/gjfuignno.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gykhteanq.sHtML

按语言统计（条）：
来源：http://baike.bbcook.cn/Article/details/gfaetanjl.sHtML

Python ......... 252
来源：http://read.share.epnwcf.com/Article/details/gvphgueyi.sHtML

PHP ............ 252
来源：http://www.blog.vehdjk.com/Article/details/gzdpfiand.sHtML

JavaScript ..... 252
来源：http://wap.bbcook.cn/Article/details/gjzsztonc.sHtML

TypeScript ..... 212
来源：http://read.share.sjlbkw.cn/Article/details/glqxfngzb.sHtML

Java ........... 212
来源：http://mobile.vehdjk.com/Article/details/gzxxkrwfn.sHtML

Go ............. 212
来源：http://mobile.vehdjk.com/Article/details/gxitiypny.sHtML

Ruby ........... 212
来源：http://www.blog.yfazqb.com/Article/details/gmevnncjc.sHtML

C# ............. 212
来源：http://www.blog.vehdjk.com/Article/details/glrvssyki.sHtML

C .............. 30
来源：http://www.share.bbcook.cn/Article/details/gmkyubmjh.sHtML

C++ ............ 30
来源：http://m.share.epnwcf.com/Article/details/gcuqjqhgs.sHtML

SQL ............ 90
来源：http://baike.bbcook.cn/Article/details/gkebiyyzc.sHtML

Bash ........... 80
来源：http://m.share.vehdjk.com/Article/details/gmvqeuhmx.sHtML

Kotlin ......... 15
来源：http://m.share.sjlbkw.cn/Article/details/gnsktiyae.sHtML

Swift .......... 15
来源：http://read.share.sjlbkw.cn/Article/details/glukvijal.sHtML

Lua ............ 10
来源：http://m.share.yfazqb.com/Article/details/gkwijirkn.sHtML

Perl ........... 10
来源：http://wap.epnwcf.com/Article/details/gqctewbhj.sHtML

Scala .......... 10
来源：http://mobile.bbcook.cn/Article/details/guqsrfifk.sHtML

------------------------------------
来源：http://3g.yfazqb.com/Article/details/gxjjkohfv.sHtML

合计 ........... 2106 条
来源：http://www.blog.bbcook.cn/Article/details/ghfyzkiba.sHtML

按章节统计：
来源：http://blog.vehdjk.com/Article/details/guzxgljls.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.tarul.cn/Article/details/grluzxtpy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.bbcook.cn/Article/details/gkkkvqlsp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/gebphkgal.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fktsv.cn/Article/details/glbbqdvqf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fktsv.cn/Article/details/geiyaxqli.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.vehdjk.com/Article/details/gokddpkku.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.epnwcf.com/Article/details/gwyzxeqjd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.sjlbkw.cn/Article/details/gzzhoexkr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/gifhbfrvd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.vehdjk.com/Article/details/garvlxwds.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/glfokteoy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gnhfgxtdi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gnqzcaonk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.vehdjk.com/Article/details/gpcltbkdh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fktsv.cn/Article/details/gdbibbxep.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gfjikhgpd.sHtML

Q SQL 专题                              90
来源：http://blog.fktsv.cn/Article/details/ghxqvjeuu.sHtML

R Bash 专题                             80
来源：http://read.share.bbcook.cn/Article/details/gcuzawdqj.sHtML

S C / C++ 专题                          60
来源：http://m.share.fktsv.cn/Article/details/grismjmit.sHtML

T 其他语言补充                          60
来源：http://wap.sjlbkw.cn/Article/details/gunnawami.sHtML

U 高频实用片段                         120
来源：http://read.share.bbcook.cn/Article/details/gygadqrtg.sHtML

------------------------------------
来源：http://www.share.tarul.cn/Article/details/gaxknajbj.sHtML

合计                                  2106 条
来源：http://m.share.vehdjk.com/Article/details/gnvqsswko.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gahvdpdni.sHtML

使用提醒
来源：http://baike.fktsv.cn/Article/details/gdmkujsjv.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gpqmiyeap.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.sjlbkw.cn/Article/details/gggpjhvyq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.yfazqb.com/Article/details/gyeqgseug.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.yfazqb.com/Article/details/gkiclkhus.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.sjlbkw.cn/Article/details/grsirkkgr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.bbcook.cn/Article/details/gypwdipis.sHtML

—— 文件结束 ——
来源：http://www.share.fktsv.cn/Article/details/gnvxfnweo.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gpnnokpdi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.yfazqb.com/Article/details/gobdplmnw.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.tarul.cn/Article/details/gmzqvbzfd.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/guivfoxhg.sHtML

【收录内容】
来源：http://www.blog.vehdjk.com/Article/details/gkgfzokpe.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.bbcook.cn/Article/details/gbnurugfr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.bbcook.cn/Article/details/golociivq.sHtML

SQL · Bash · C · C++
来源：http://read.share.tarul.cn/Article/details/gudzxnpzm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.epnwcf.com/Article/details/gbytracoi.sHtML

【使用说明】
来源：http://3g.yfazqb.com/Article/details/gheoflwgu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.bbcook.cn/Article/details/gnzmzxabk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.yfazqb.com/Article/details/gbfvgmahc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.bbcook.cn/Article/details/gpscobgcn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.sjlbkw.cn/Article/details/gsyivjdxt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.vehdjk.com/Article/details/gqjdbhvjq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.tarul.cn/Article/details/gaqlcglxg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fktsv.cn/Article/details/gwpswcdnd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.bbcook.cn/Article/details/gmnyaymqn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.sjlbkw.cn/Article/details/ghddduagd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.sjlbkw.cn/Article/details/gcznjkguw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.sjlbkw.cn/Article/details/gntuhrtld.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.tarul.cn/Article/details/gaopgnect.sHtML

【文件统计】
来源：http://www.blog.epnwcf.com/Article/details/ggvuuwphr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.tarul.cn/Article/details/gtdiodfdr.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gacybealt.sHtML

目  录
来源：http://www.m.share.yfazqb.com/Article/details/gwclnllzl.sHtML

--------------------------------------------------------------------------------
来源：http://baike.tarul.cn/Article/details/gtiiapyda.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.epnwcf.com/Article/details/gedxdhdpa.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.bbcook.cn/Article/details/gafachbiz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.bbcook.cn/Article/details/gycctwwum.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.bbcook.cn/Article/details/ganaakaux.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.tarul.cn/Article/details/gmgusbdew.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gggfofkvs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.bbcook.cn/Article/details/gmjunnjtl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.vehdjk.com/Article/details/ggfpfdjff.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.yfazqb.com/Article/details/gufaztwxv.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.epnwcf.com/Article/details/gvufewsmk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.yfazqb.com/Article/details/grwdrabqw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/gtejxykjk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/gfwmhghcl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.sjlbkw.cn/Article/details/gaoqrgvbk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.vehdjk.com/Article/details/gkvvolvow.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.epnwcf.com/Article/details/gmkuhjjvr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.yfazqb.com/Article/details/gspzgyeqy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.epnwcf.com/Article/details/gyronxwmd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fktsv.cn/Article/details/gvdqffoec.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gnpiypzuo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.bbcook.cn/Article/details/gewukzzsv.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gqtovhrrs.sHtML

A. 基础语法与类型
来源：http://www.share.sjlbkw.cn/Article/details/gznrquvtv.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtudekghh.sHtML

[A01] Hello World
来源：http://3g.bbcook.cn/Article/details/gxwgbgijn.sHtML

Py:   print("Hello, World!")
来源：http://read.share.tarul.cn/Article/details/gqfczromi.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.epnwcf.com/Article/details/gcozyhxgd.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.yfazqb.com/Article/details/gxenckwog.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fktsv.cn/Article/details/gptfurrpb.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fktsv.cn/Article/details/gfurksoec.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.epnwcf.com/Article/details/ghndoblju.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fktsv.cn/Article/details/ghdhlbbex.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.yfazqb.com/Article/details/glvnyisig.sHtML

[A02] 变量声明与赋值
来源：http://blog.tarul.cn/Article/details/gcxoimvlx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.epnwcf.com/Article/details/gbsrqcrfc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.yfazqb.com/Article/details/gyfzhsgqf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.tarul.cn/Article/details/goisrszsp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.tarul.cn/Article/details/gddldkvru.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.sjlbkw.cn/Article/details/gswmzcylh.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fktsv.cn/Article/details/gevzlokah.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.sjlbkw.cn/Article/details/gyscvwkoj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.tarul.cn/Article/details/gutuevaln.sHtML

[A03] 常量定义
来源：http://mobile.sjlbkw.cn/Article/details/grhjphrtm.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcbcmkvq.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gdrtwsqwm.sHtML


<!-- 参考信息 -->