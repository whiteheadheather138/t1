代发 wailian999

[U31] Py：单测
来源：http://www.share.epnwcf.com/Article/details/gmwpszkxg.sHtML

python -m pytest -q
来源：http://baike.vehdjk.com/Article/details/gifeioiry.sHtML

[U32] Py：代码格式化
来源：http://blog.fktsv.cn/Article/details/gqawzbaah.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.vehdjk.com/Article/details/gtmfrmzup.sHtML

[U33] Py：打包发布
来源：http://www.share.fktsv.cn/Article/details/gndcohccj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.bbcook.cn/Article/details/gpevrgfjc.sHtML

[U34] Py：判断编码
来源：http://baike.tarul.cn/Article/details/glsindiao.sHtML

chardet.detect(raw)
来源：http://mobile.tarul.cn/Article/details/gbjdesafq.sHtML

[U35] Py：发送邮件
来源：http://mobile.yfazqb.com/Article/details/gdxxasldt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.sjlbkw.cn/Article/details/gdtxuknsw.sHtML

[U36] Py：定时任务
来源：http://baike.bbcook.cn/Article/details/gprijowqj.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.vehdjk.com/Article/details/gnuoihwir.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.sjlbkw.cn/Article/details/grjqefisv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.epnwcf.com/Article/details/ggwnqfmeg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fktsv.cn/Article/details/gyodxpevg.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fktsv.cn/Article/details/gsayzxxxx.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.bbcook.cn/Article/details/gcdqrjqip.sHtML

sys.stdout.isatty()
来源：http://blog.fktsv.cn/Article/details/gbqfdbify.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.tarul.cn/Article/details/guvhyyjms.sHtML

print("err", file=sys.stderr)
来源：http://blog.yfazqb.com/Article/details/gstmsletp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.epnwcf.com/Article/details/guwcplhkp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fktsv.cn/Article/details/ghxugstth.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fktsv.cn/Article/details/gpdnsqvas.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.bbcook.cn/Article/details/gbomissyu.sHtML

[U43] PHP：声明命名空间
来源：http://baike.vehdjk.com/Article/details/gnsafgawz.sHtML

namespace App\Http;
来源：http://mobile.bbcook.cn/Article/details/gdoerkdoq.sHtML

[U44] PHP：开启严格类型
来源：http://blog.bbcook.cn/Article/details/gnjiunmot.sHtML

declare(strict_types=1);
来源：http://m.share.fktsv.cn/Article/details/gdqzedqxl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.sjlbkw.cn/Article/details/gqhdqcpls.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gowwbkoxi.sHtML

[U46] PHP：可空类型
来源：http://blog.epnwcf.com/Article/details/gljpfbptd.sHtML

?string $name = null
来源：http://baike.sjlbkw.cn/Article/details/gzvunvntw.sHtML

[U47] PHP：联合类型
来源：http://baike.yfazqb.com/Article/details/gsrqqxsll.sHtML

int|string $id
来源：http://m.share.yfazqb.com/Article/details/gaomdsedx.sHtML

[U48] PHP：纯枚举
来源：http://www.share.tarul.cn/Article/details/ggiigicwq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.epnwcf.com/Article/details/ghticuqjx.sHtML

[U49] PHP：只读属性
来源：http://blog.yfazqb.com/Article/details/gvicghycy.sHtML

public readonly string $name
来源：http://www.blog.tarul.cn/Article/details/gmgrnmydb.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.bbcook.cn/Article/details/gjvkzvsra.sHtML

public function __construct(private int $id) {}
来源：http://m.share.bbcook.cn/Article/details/gfeqsrlri.sHtML

[U51] PHP：数组解构
来源：http://blog.tarul.cn/Article/details/gjunrdijc.sHtML

[$a, $b] = $arr;
来源：http://m.share.epnwcf.com/Article/details/gemqvvicv.sHtML

[U52] PHP：箭头函数
来源：http://read.share.tarul.cn/Article/details/gewhyqsug.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.sjlbkw.cn/Article/details/gmsfbjeyk.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fktsv.cn/Article/details/gzxcblcxn.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fktsv.cn/Article/details/grzcxuozr.sHtML

[U54] PHP：空安全调用
来源：http://blog.bbcook.cn/Article/details/gehdbmpdl.sHtML

$obj?->method()
来源：http://read.share.sjlbkw.cn/Article/details/grtjomaic.sHtML

[U55] PHP：match 表达式
来源：http://3g.fktsv.cn/Article/details/gqqgjnljo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.yfazqb.com/Article/details/gacnyetmv.sHtML

[U56] PHP：命名参数
来源：http://blog.fktsv.cn/Article/details/guoiukclp.sHtML

f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gwydptfke.sHtML

[U57] PHP：字符串插值
来源：http://blog.yfazqb.com/Article/details/gkllkkghn.sHtML

"值: {$a}"
来源：http://mobile.sjlbkw.cn/Article/details/gablcrbnb.sHtML

[U58] PHP：数组三件套
来源：http://m.share.epnwcf.com/Article/details/gmyzddaeu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.yfazqb.com/Article/details/gntazlitn.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.vehdjk.com/Article/details/geynuqbvp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.tarul.cn/Article/details/gvdwvtpct.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fktsv.cn/Article/details/griejfbyx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.sjlbkw.cn/Article/details/gglfsrdhv.sHtML

[U61] PHP：正则
来源：http://www.blog.sjlbkw.cn/Article/details/gwaftijph.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.yfazqb.com/Article/details/guickvsqp.sHtML

[U62] PHP：日期对象
来源：http://blog.vehdjk.com/Article/details/gjiqblohp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fktsv.cn/Article/details/gplfxaqwc.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.yfazqb.com/Article/details/grxtcfgpd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fktsv.cn/Article/details/geobhshrg.sHtML

[U64] PHP：目录遍历
来源：http://wap.tarul.cn/Article/details/gqmmdqpjn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.bbcook.cn/Article/details/gsdegohlj.sHtML

[U65] PHP：会话
来源：http://3g.tarul.cn/Article/details/gcdvlixba.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.epnwcf.com/Article/details/gqttvlrhr.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.tarul.cn/Article/details/gmpkntpwn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.tarul.cn/Article/details/gylecclxn.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.bbcook.cn/Article/details/gcbegyeqe.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.tarul.cn/Article/details/gaaajkwwv.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fktsv.cn/Article/details/gvhluxpfu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fktsv.cn/Article/details/gdsqqdbvh.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.vehdjk.com/Article/details/gicdmamcl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.tarul.cn/Article/details/gyyfrprow.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fktsv.cn/Article/details/gfcqbpxet.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.epnwcf.com/Article/details/gfomsoxcw.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.tarul.cn/Article/details/gfjpfckod.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.vehdjk.com/Article/details/gbwigbdry.sHtML

[U72] PHP：写错误日志
来源：http://baike.bbcook.cn/Article/details/gyoiathog.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.bbcook.cn/Article/details/gwxrvcenx.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fktsv.cn/Article/details/gkpqxcqbr.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.sjlbkw.cn/Article/details/grdivkvir.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.bbcook.cn/Article/details/gilcrxuao.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.vehdjk.com/Article/details/gujdivhfq.sHtML

[U75] PHP：依赖注入
来源：http://blog.fktsv.cn/Article/details/gobwwbqcc.sHtML

composer require psr/container
来源：http://baike.tarul.cn/Article/details/gtntbsgxm.sHtML

[U76] PHP：简单路由
来源：http://wap.vehdjk.com/Article/details/gvrxavarr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fktsv.cn/Article/details/gksyvwbin.sHtML

[U77] PHP：模板渲染
来源：http://blog.fktsv.cn/Article/details/ghyehjdzk.sHtML

composer require twig/twig
来源：http://mobile.epnwcf.com/Article/details/guvcxzusu.sHtML

[U78] PHP：单元测试
来源：http://baike.vehdjk.com/Article/details/gytahbesv.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.sjlbkw.cn/Article/details/gtnixfymz.sHtML

[U79] PHP：静态分析
来源：http://m.share.epnwcf.com/Article/details/gcppcmcat.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fktsv.cn/Article/details/guleihmtb.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fktsv.cn/Article/details/gbydkpzug.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.epnwcf.com/Article/details/gynxgqdvc.sHtML

[U81] JS：初始化项目
来源：http://baike.bbcook.cn/Article/details/giwhchoah.sHtML

npm init -y;  npm i express
来源：http://read.share.vehdjk.com/Article/details/gjfthykjp.sHtML

[U82] JS：package.json 脚本
来源：http://wap.epnwcf.com/Article/details/gecwcqakq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fktsv.cn/Article/details/gdjrvckjc.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.bbcook.cn/Article/details/gigiupifh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.bbcook.cn/Article/details/gxmfkperd.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.tarul.cn/Article/details/gkggfddsb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.sjlbkw.cn/Article/details/gikchqquv.sHtML

[U85] JS：可选链
来源：http://www.blog.sjlbkw.cn/Article/details/ghbopbmhf.sHtML

a?.b?.c
来源：http://3g.vehdjk.com/Article/details/gyntwqylu.sHtML

[U86] JS：空值合并
来源：http://www.blog.yfazqb.com/Article/details/ggbwnzbkk.sHtML

a ?? b
来源：http://www.share.sjlbkw.cn/Article/details/gelpoegof.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fktsv.cn/Article/details/gemystqjx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.tarul.cn/Article/details/glpmehvqw.sHtML

[U88] JS：对象展开合并
来源：http://www.share.sjlbkw.cn/Article/details/gfsflyfjv.sHtML

{ ...a, ...b }
来源：http://read.share.tarul.cn/Article/details/gbqaqzpzi.sHtML

[U89] JS：数组去重
来源：http://read.share.epnwcf.com/Article/details/grmrewiew.sHtML

[...new Set(arr)]
来源：http://blog.vehdjk.com/Article/details/gsnpodpun.sHtML

[U90] JS：数字数组排序
来源：http://blog.yfazqb.com/Article/details/gzogecnjv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/goinhgefw.sHtML

[U91] JS：对象键值遍历
来源：http://wap.sjlbkw.cn/Article/details/gdxtkwvbb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.epnwcf.com/Article/details/gyebsvzta.sHtML

[U92] JS：深拷贝
来源：http://m.share.epnwcf.com/Article/details/gfewrtxgl.sHtML

structuredClone(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gumkjwjxf.sHtML

[U93] JS：模板字符串
来源：http://read.share.bbcook.cn/Article/details/gkfawhmde.sHtML

`共 ${n} 条`
来源：http://wap.yfazqb.com/Article/details/gniopqvfc.sHtML

[U94] JS：箭头函数
来源：http://m.share.tarul.cn/Article/details/gadafaqxs.sHtML

const double = x => x * 2;
来源：http://baike.epnwcf.com/Article/details/gthmsincz.sHtML

[U95] JS：Promise 包装
来源：http://blog.tarul.cn/Article/details/goaxlaomt.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.yfazqb.com/Article/details/gbmgcpvuf.sHtML

[U96] JS：async/await 与异常
来源：http://baike.yfazqb.com/Article/details/gievpscqz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gkjidzsai.sHtML

[U97] JS：并发请求
来源：http://www.share.vehdjk.com/Article/details/gerxbyets.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/gyczbehjq.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fktsv.cn/Article/details/gnnuzdixb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.sjlbkw.cn/Article/details/gktildvwq.sHtML

[U99] JS：事件监听
来源：http://blog.fktsv.cn/Article/details/gevmqutjm.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.vehdjk.com/Article/details/gnrwkagzu.sHtML

[U100] JS：DOM 查询
来源：http://blog.sjlbkw.cn/Article/details/gpiqvekqq.sHtML

document.querySelector(".item")
来源：http://baike.yfazqb.com/Article/details/glgziembr.sHtML

[U101] JS：classList 操作
来源：http://read.share.vehdjk.com/Article/details/gkfvgpagn.sHtML

el.classList.toggle("active")
来源：http://mobile.yfazqb.com/Article/details/glpykpulr.sHtML

[U102] JS：本地存储
来源：http://m.share.yfazqb.com/Article/details/gmvvhkeqe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.vehdjk.com/Article/details/geikybujc.sHtML

[U103] JS：定时器
来源：http://baike.yfazqb.com/Article/details/gwgbxjnpr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.epnwcf.com/Article/details/grbgapqma.sHtML

[U104] JS：防抖
来源：http://baike.fktsv.cn/Article/details/gyxdewure.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gajmvkqew.sHtML

[U105] JS：节流
来源：http://blog.tarul.cn/Article/details/gujhlxxlp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.vehdjk.com/Article/details/gdszpqjci.sHtML

[U106] JS：日期格式化
来源：http://3g.yfazqb.com/Article/details/grcsxxzim.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fktsv.cn/Article/details/gikccnkvr.sHtML

[U107] JS：数字千分位
来源：http://www.share.yfazqb.com/Article/details/gldxlfqzj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.bbcook.cn/Article/details/gknzqjksy.sHtML

[U108] JS：随机整数
来源：http://3g.epnwcf.com/Article/details/gaxzpbxrt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.sjlbkw.cn/Article/details/gszlvyfbz.sHtML

[U109] JS：数组分组
来源：http://3g.sjlbkw.cn/Article/details/gmnxfpwnv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.epnwcf.com/Article/details/gazrduqsm.sHtML

[U110] JS：数组分块
来源：http://m.share.yfazqb.com/Article/details/ggbwveomy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.vehdjk.com/Article/details/gfwueppxl.sHtML

[U111] JS：对象转 Map
来源：http://read.share.epnwcf.com/Article/details/gcwlotgbg.sHtML

new Map(Object.entries(obj))
来源：http://mobile.tarul.cn/Article/details/gjsrmsvct.sHtML

[U112] JS：字符串补位
来源：http://3g.vehdjk.com/Article/details/geqwimpla.sHtML

"7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/gwrzztngj.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.epnwcf.com/Article/details/gcmiwrnvq.sHtML

s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gsaqxplrp.sHtML

[U114] JS：JSON 深比较
来源：http://blog.sjlbkw.cn/Article/details/gflwxcsoa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fktsv.cn/Article/details/gtsxzxwdp.sHtML

[U115] JS：生成 UUID
来源：http://blog.sjlbkw.cn/Article/details/giwtizvat.sHtML

crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/govrzywbk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.sjlbkw.cn/Article/details/gbhdpwtut.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fktsv.cn/Article/details/gkpxiwlgd.sHtML

[U117] JS：单元测试
来源：http://wap.sjlbkw.cn/Article/details/gwbiyecyt.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.bbcook.cn/Article/details/ghogyqmet.sHtML

[U118] JS：开发服务器
来源：http://m.share.tarul.cn/Article/details/gsludqnsm.sHtML

npm i -D vite;  npx vite
来源：http://www.share.yfazqb.com/Article/details/gzfralhyv.sHtML

[U119] JS：生产构建
来源：http://www.blog.fktsv.cn/Article/details/gvvihrkim.sHtML

npx vite build
来源：http://read.share.fktsv.cn/Article/details/gtryaapiv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.bbcook.cn/Article/details/gtecgtedo.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.yfazqb.com/Article/details/gaelcykfv.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gsairbhwz.sHtML

统计汇总
来源：http://read.share.fktsv.cn/Article/details/glecowatq.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gatsyadwd.sHtML

按语言统计（条）：
来源：http://read.share.fktsv.cn/Article/details/gziaswskh.sHtML

Python ......... 252
来源：http://baike.epnwcf.com/Article/details/grjkfocra.sHtML

PHP ............ 252
来源：http://3g.sjlbkw.cn/Article/details/giayjfhpx.sHtML

JavaScript ..... 252
来源：http://m.share.vehdjk.com/Article/details/gzrdwvcqx.sHtML

TypeScript ..... 212
来源：http://www.share.tarul.cn/Article/details/gavfkxwvr.sHtML

Java ........... 212
来源：http://www.m.share.vehdjk.com/Article/details/gydtxupia.sHtML

Go ............. 212
来源：http://mobile.sjlbkw.cn/Article/details/gzqrrqbzo.sHtML

Ruby ........... 212
来源：http://m.share.vehdjk.com/Article/details/gjamzpchr.sHtML

C# ............. 212
来源：http://3g.vehdjk.com/Article/details/gleucosdu.sHtML

C .............. 30
来源：http://m.share.epnwcf.com/Article/details/gezldsvli.sHtML

C++ ............ 30
来源：http://www.share.bbcook.cn/Article/details/gsrtrpgnv.sHtML

SQL ............ 90
来源：http://www.m.share.yfazqb.com/Article/details/gvjibdydu.sHtML

Bash ........... 80
来源：http://www.m.share.bbcook.cn/Article/details/givwbgmuc.sHtML

Kotlin ......... 15
来源：http://3g.yfazqb.com/Article/details/gcugnnlcn.sHtML

Swift .......... 15
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzsuuiax.sHtML

Lua ............ 10
来源：http://m.share.yfazqb.com/Article/details/gyuuxspiy.sHtML

Perl ........... 10
来源：http://wap.tarul.cn/Article/details/gxppfdpio.sHtML

Scala .......... 10
来源：http://baike.vehdjk.com/Article/details/gusimenze.sHtML

------------------------------------
来源：http://m.share.epnwcf.com/Article/details/gayydtsxx.sHtML

合计 ........... 2106 条
来源：http://www.share.fktsv.cn/Article/details/gibgmuirs.sHtML

按章节统计：
来源：http://3g.sjlbkw.cn/Article/details/glqwksyxs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.yfazqb.com/Article/details/gvvklfteb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fktsv.cn/Article/details/gygcmwvcz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fktsv.cn/Article/details/geymfbvnf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.sjlbkw.cn/Article/details/gcweqtjxd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fktsv.cn/Article/details/grkixyjlq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.bbcook.cn/Article/details/gnrbhuvdh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.yfazqb.com/Article/details/guqucxumf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.sjlbkw.cn/Article/details/gmwfyhsbd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/gfkppwvfz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.vehdjk.com/Article/details/gdpgpiwzc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gquoaafag.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/gzqzrsyrz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gyljtrzfu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.bbcook.cn/Article/details/gssqhobtq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.epnwcf.com/Article/details/gexbpakbx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fktsv.cn/Article/details/gurdrvlby.sHtML

Q SQL 专题                              90
来源：http://3g.vehdjk.com/Article/details/gvvsvugfl.sHtML

R Bash 专题                             80
来源：http://baike.epnwcf.com/Article/details/gsrplenuu.sHtML

S C / C++ 专题                          60
来源：http://read.share.tarul.cn/Article/details/ghsqggejf.sHtML

T 其他语言补充                          60
来源：http://wap.tarul.cn/Article/details/gergivlpm.sHtML

U 高频实用片段                         120
来源：http://read.share.vehdjk.com/Article/details/glplesshb.sHtML

------------------------------------
来源：http://wap.yfazqb.com/Article/details/gzyepkddg.sHtML

合计                                  2106 条
来源：http://3g.bbcook.cn/Article/details/gsutfssfj.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fktsv.cn/Article/details/ghjddccft.sHtML

使用提醒
来源：http://www.share.bbcook.cn/Article/details/gwajharjp.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gpascdzuk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.tarul.cn/Article/details/gyqyjmguo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.yfazqb.com/Article/details/gxaemmmzo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.epnwcf.com/Article/details/gcxmicmfs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.epnwcf.com/Article/details/gfxribgnx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.vehdjk.com/Article/details/gmcwbzcyq.sHtML

—— 文件结束 ——
来源：http://www.blog.fktsv.cn/Article/details/ggpdbqsyg.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gvibdsjrn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.epnwcf.com/Article/details/gbkbfkzgg.sHtML

Common Programming Examples Cheat Book
来源：http://3g.epnwcf.com/Article/details/gclwjsfvz.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/getkhgcut.sHtML

【收录内容】
来源：http://blog.epnwcf.com/Article/details/gsjofiqsu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.bbcook.cn/Article/details/gkihgtbec.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.vehdjk.com/Article/details/gakyrqrwv.sHtML

SQL · Bash · C · C++
来源：http://blog.bbcook.cn/Article/details/gjlpmalhe.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.vehdjk.com/Article/details/gttdzvrrs.sHtML

【使用说明】
来源：http://read.share.epnwcf.com/Article/details/gxolcxxkz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.tarul.cn/Article/details/gaeuumrsw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.epnwcf.com/Article/details/ghgsowslf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.yfazqb.com/Article/details/gwvcffzfl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fktsv.cn/Article/details/gfpuwrspp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.bbcook.cn/Article/details/gpkdcneds.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.yfazqb.com/Article/details/ghkhnecyf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.vehdjk.com/Article/details/gcxzhtkcs.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.yfazqb.com/Article/details/gywsbfwac.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.vehdjk.com/Article/details/ggdfxicat.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.yfazqb.com/Article/details/glviygkpa.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.bbcook.cn/Article/details/gzshrbcly.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrmxihbw.sHtML

【文件统计】
来源：http://3g.epnwcf.com/Article/details/gzmnpylrx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fktsv.cn/Article/details/gvmojbhtt.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fktsv.cn/Article/details/gyotuvtlo.sHtML

目  录
来源：http://www.blog.sjlbkw.cn/Article/details/ghyayhhft.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gudrhcwwb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.tarul.cn/Article/details/gxtcwbehp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.yfazqb.com/Article/details/gmnrfysnh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.bbcook.cn/Article/details/gjyeiqdgx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fktsv.cn/Article/details/gweijchde.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.sjlbkw.cn/Article/details/gfqkjkjio.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.tarul.cn/Article/details/gvpyajdix.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fktsv.cn/Article/details/gwfdbgxzk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.yfazqb.com/Article/details/gluggtjve.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.vehdjk.com/Article/details/gltwpnism.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.yfazqb.com/Article/details/gyniwjrkm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/glazrqsze.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.tarul.cn/Article/details/gmrgeulye.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/ghdgzgwqp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.vehdjk.com/Article/details/glkwssrgs.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.epnwcf.com/Article/details/gqmmtsfvt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/grjngibbs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.bbcook.cn/Article/details/gstuxhnfe.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.yfazqb.com/Article/details/giudcicbv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.epnwcf.com/Article/details/gvtocxabs.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/gmlzlluxh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.tarul.cn/Article/details/gkqczvxjg.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gcoitlvca.sHtML

A. 基础语法与类型
来源：http://mobile.tarul.cn/Article/details/gnoyvtmnu.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkukjuuib.sHtML

[A01] Hello World
来源：http://3g.fktsv.cn/Article/details/getnjqina.sHtML

Py:   print("Hello, World!")
来源：http://www.share.yfazqb.com/Article/details/gociuhxmw.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fktsv.cn/Article/details/grhbsoyis.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.bbcook.cn/Article/details/gasqtfbfd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.tarul.cn/Article/details/gmrxsbvnf.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.epnwcf.com/Article/details/gyktldtec.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fktsv.cn/Article/details/gybpznahm.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.vehdjk.com/Article/details/gyhxvnbbc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.epnwcf.com/Article/details/guerkfnxv.sHtML

[A02] 变量声明与赋值
来源：http://m.share.sjlbkw.cn/Article/details/ghwdvdczc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmfmsxsq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.yfazqb.com/Article/details/ghytzxcwx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.vehdjk.com/Article/details/gsuvbatwn.sHtML


<!-- 参考信息 -->