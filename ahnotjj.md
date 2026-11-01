代发 wailian999

[U31] Py：单测
来源：http://read.share.epnwcf.com/Article/details/geopahilu.sHtML

python -m pytest -q
来源：http://read.share.bbcook.cn/Article/details/gdukpbpum.sHtML

[U32] Py：代码格式化
来源：http://wap.bbcook.cn/Article/details/gbcwcizrs.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.epnwcf.com/Article/details/gqpbiuulj.sHtML

[U33] Py：打包发布
来源：http://mobile.yfazqb.com/Article/details/guozcmshz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.yfazqb.com/Article/details/gkhfkpbas.sHtML

[U34] Py：判断编码
来源：http://www.blog.bbcook.cn/Article/details/gqunhhcdj.sHtML

chardet.detect(raw)
来源：http://blog.sjlbkw.cn/Article/details/gqkpcggln.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.bbcook.cn/Article/details/gkyuzaovo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.bbcook.cn/Article/details/gtsdbfyus.sHtML

[U36] Py：定时任务
来源：http://3g.epnwcf.com/Article/details/gqxmyhotv.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.tarul.cn/Article/details/gehbpznqn.sHtML

[U37] Py：读写 Excel
来源：http://m.share.sjlbkw.cn/Article/details/gthoptwzm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.bbcook.cn/Article/details/gcdbeniyt.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.epnwcf.com/Article/details/gmljxfzrj.sHtML

Path(__file__).resolve().parent
来源：http://mobile.sjlbkw.cn/Article/details/gqijdtxfd.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.yfazqb.com/Article/details/gvmfizops.sHtML

sys.stdout.isatty()
来源：http://www.blog.tarul.cn/Article/details/gvgpqbrxz.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.tarul.cn/Article/details/gynkeysxd.sHtML

print("err", file=sys.stderr)
来源：http://www.share.tarul.cn/Article/details/glsafbzng.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.tarul.cn/Article/details/gdkgcbycr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.yfazqb.com/Article/details/gibpcigpy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.yfazqb.com/Article/details/gpdilwlai.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fktsv.cn/Article/details/gzsvowdcj.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.vehdjk.com/Article/details/gbzzofesm.sHtML

namespace App\Http;
来源：http://3g.fktsv.cn/Article/details/gqgmkwpqx.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fktsv.cn/Article/details/gpysplqxh.sHtML

declare(strict_types=1);
来源：http://wap.fktsv.cn/Article/details/gnvakkzls.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.vehdjk.com/Article/details/gpoyzuwgj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gcjdwocgu.sHtML

[U46] PHP：可空类型
来源：http://wap.sjlbkw.cn/Article/details/gpxuewfgx.sHtML

?string $name = null
来源：http://www.m.share.yfazqb.com/Article/details/gweyaoccd.sHtML

[U47] PHP：联合类型
来源：http://www.share.bbcook.cn/Article/details/gvhxcqjwa.sHtML

int|string $id
来源：http://m.share.sjlbkw.cn/Article/details/gjwyopyjk.sHtML

[U48] PHP：纯枚举
来源：http://wap.bbcook.cn/Article/details/gzwopevwq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.vehdjk.com/Article/details/gvvtvxpkj.sHtML

[U49] PHP：只读属性
来源：http://read.share.yfazqb.com/Article/details/gcylhvqpr.sHtML

public readonly string $name
来源：http://m.share.sjlbkw.cn/Article/details/grmcykcpu.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.epnwcf.com/Article/details/gelodhgcd.sHtML

public function __construct(private int $id) {}
来源：http://3g.epnwcf.com/Article/details/gzmvdcwja.sHtML

[U51] PHP：数组解构
来源：http://3g.yfazqb.com/Article/details/grymvkubb.sHtML

[$a, $b] = $arr;
来源：http://3g.tarul.cn/Article/details/gyfcjxmlp.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.bbcook.cn/Article/details/gjnazywgo.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.bbcook.cn/Article/details/glvlciihp.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.bbcook.cn/Article/details/gmekhhmwv.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.vehdjk.com/Article/details/ghlasyqzi.sHtML

[U54] PHP：空安全调用
来源：http://baike.epnwcf.com/Article/details/gbhtkdrub.sHtML

$obj?->method()
来源：http://www.blog.bbcook.cn/Article/details/gugumvdvs.sHtML

[U55] PHP：match 表达式
来源：http://baike.vehdjk.com/Article/details/gisvwfffa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.yfazqb.com/Article/details/ghndvczyl.sHtML

[U56] PHP：命名参数
来源：http://mobile.tarul.cn/Article/details/gllzbhlkd.sHtML

f(a: 1, b: 2)
来源：http://baike.vehdjk.com/Article/details/gpvyzopho.sHtML

[U57] PHP：字符串插值
来源：http://www.share.epnwcf.com/Article/details/gwhuxzkxu.sHtML

"值: {$a}"
来源：http://wap.fktsv.cn/Article/details/gnjyjjkcg.sHtML

[U58] PHP：数组三件套
来源：http://mobile.vehdjk.com/Article/details/gqwkwawtc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.tarul.cn/Article/details/goaolvava.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.yfazqb.com/Article/details/gphrvyuil.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.yfazqb.com/Article/details/gimcxqwmw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fktsv.cn/Article/details/gtxypsbii.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fktsv.cn/Article/details/gtttdfvod.sHtML

[U61] PHP：正则
来源：http://www.blog.vehdjk.com/Article/details/gmgtimxkw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.sjlbkw.cn/Article/details/gnqlngqoi.sHtML

[U62] PHP：日期对象
来源：http://3g.vehdjk.com/Article/details/gdemxaxfh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.bbcook.cn/Article/details/gdlomezuw.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fktsv.cn/Article/details/gciuuaaba.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.tarul.cn/Article/details/gqsuauhvq.sHtML

[U64] PHP：目录遍历
来源：http://wap.fktsv.cn/Article/details/gvnbwidxy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.vehdjk.com/Article/details/gvnbxqljz.sHtML

[U65] PHP：会话
来源：http://www.share.fktsv.cn/Article/details/gsthhgtto.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.tarul.cn/Article/details/gyrprbepj.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fktsv.cn/Article/details/gdsyrogqd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.sjlbkw.cn/Article/details/gkrzyvjhx.sHtML

[U67] PHP：处理文件上传
来源：http://baike.tarul.cn/Article/details/geodpqzab.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxdncinw.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.vehdjk.com/Article/details/guhflccbv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.vehdjk.com/Article/details/gnsnexlyr.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.epnwcf.com/Article/details/guukwgqwg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.sjlbkw.cn/Article/details/gyydcvuru.sHtML

[U70] PHP：PDO 事务
来源：http://blog.tarul.cn/Article/details/gjanbyltk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.yfazqb.com/Article/details/ghuhfjpqk.sHtML

[U71] PHP：抛出异常
来源：http://baike.yfazqb.com/Article/details/gzmzhsftc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.bbcook.cn/Article/details/gqevfqtmi.sHtML

[U72] PHP：写错误日志
来源：http://blog.epnwcf.com/Article/details/gdisegvie.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.yfazqb.com/Article/details/gqsfpmhnp.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fktsv.cn/Article/details/galfqdpta.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.epnwcf.com/Article/details/gbduuwkxi.sHtML

[U74] PHP：读取环境变量
来源：http://wap.tarul.cn/Article/details/gdvucwiap.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.sjlbkw.cn/Article/details/gtjxqzwyp.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fktsv.cn/Article/details/ggebaynfa.sHtML

composer require psr/container
来源：http://read.share.epnwcf.com/Article/details/gtudibszx.sHtML

[U76] PHP：简单路由
来源：http://read.share.epnwcf.com/Article/details/gdjyitpmp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fktsv.cn/Article/details/gquhksjfs.sHtML

[U77] PHP：模板渲染
来源：http://m.share.bbcook.cn/Article/details/gwfsjecxj.sHtML

composer require twig/twig
来源：http://3g.fktsv.cn/Article/details/gjabpufyr.sHtML

[U78] PHP：单元测试
来源：http://mobile.fktsv.cn/Article/details/gkhgvznla.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.bbcook.cn/Article/details/gnlqenvbz.sHtML

[U79] PHP：静态分析
来源：http://baike.vehdjk.com/Article/details/gkwpxhniv.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.vehdjk.com/Article/details/gzlzfarqg.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fktsv.cn/Article/details/grbijysxl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.yfazqb.com/Article/details/gmfmqubnt.sHtML

[U81] JS：初始化项目
来源：http://blog.epnwcf.com/Article/details/gqzjhvrld.sHtML

npm init -y;  npm i express
来源：http://www.share.tarul.cn/Article/details/gmzoawvtv.sHtML

[U82] JS：package.json 脚本
来源：http://wap.tarul.cn/Article/details/gxgguhibj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.yfazqb.com/Article/details/grfrjfqsh.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.tarul.cn/Article/details/gsdtnawtw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.vehdjk.com/Article/details/gkkjotixm.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.yfazqb.com/Article/details/gmikxgjvr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.epnwcf.com/Article/details/gqavvgkjj.sHtML

[U85] JS：可选链
来源：http://mobile.fktsv.cn/Article/details/geiknystn.sHtML

a?.b?.c
来源：http://blog.yfazqb.com/Article/details/gpvgkbelo.sHtML

[U86] JS：空值合并
来源：http://wap.yfazqb.com/Article/details/gzwppezuu.sHtML

a ?? b
来源：http://blog.vehdjk.com/Article/details/glmyufncs.sHtML

[U87] JS：解构默认值
来源：http://wap.tarul.cn/Article/details/gfygiejgd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.epnwcf.com/Article/details/gsgioqtng.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.tarul.cn/Article/details/gafhwmxpk.sHtML

{ ...a, ...b }
来源：http://read.share.epnwcf.com/Article/details/gclzfgkds.sHtML

[U89] JS：数组去重
来源：http://m.share.yfazqb.com/Article/details/grivreusz.sHtML

[...new Set(arr)]
来源：http://blog.sjlbkw.cn/Article/details/gzqfspsjo.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.epnwcf.com/Article/details/glemrzqkd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gdfkegatr.sHtML

[U91] JS：对象键值遍历
来源：http://wap.bbcook.cn/Article/details/gwondmdsf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.yfazqb.com/Article/details/gupvubpwd.sHtML

[U92] JS：深拷贝
来源：http://read.share.vehdjk.com/Article/details/gixwxhxem.sHtML

structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/gnlyvthjl.sHtML

[U93] JS：模板字符串
来源：http://www.share.tarul.cn/Article/details/gntrswvaa.sHtML

`共 ${n} 条`
来源：http://read.share.sjlbkw.cn/Article/details/godjcqppb.sHtML

[U94] JS：箭头函数
来源：http://wap.fktsv.cn/Article/details/gfledkgcv.sHtML

const double = x => x * 2;
来源：http://www.blog.fktsv.cn/Article/details/gugcjnlvw.sHtML

[U95] JS：Promise 包装
来源：http://www.share.epnwcf.com/Article/details/gzaeekycb.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.vehdjk.com/Article/details/gluscawaq.sHtML

[U96] JS：async/await 与异常
来源：http://3g.sjlbkw.cn/Article/details/gjhmxrrfq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gkwmyuisx.sHtML

[U97] JS：并发请求
来源：http://3g.sjlbkw.cn/Article/details/ggzncbpjp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/glawuvqhy.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.epnwcf.com/Article/details/gqwbgwkjf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.bbcook.cn/Article/details/gdajsyqap.sHtML

[U99] JS：事件监听
来源：http://mobile.sjlbkw.cn/Article/details/guzbfnocr.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.epnwcf.com/Article/details/gzgxvvutz.sHtML

[U100] JS：DOM 查询
来源：http://www.share.bbcook.cn/Article/details/gbxfbtndr.sHtML

document.querySelector(".item")
来源：http://read.share.fktsv.cn/Article/details/gqrwplfax.sHtML

[U101] JS：classList 操作
来源：http://m.share.yfazqb.com/Article/details/gtfkzyzod.sHtML

el.classList.toggle("active")
来源：http://mobile.epnwcf.com/Article/details/gvjxbmawj.sHtML

[U102] JS：本地存储
来源：http://blog.sjlbkw.cn/Article/details/gcvgnhqgv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.tarul.cn/Article/details/gihkyhgop.sHtML

[U103] JS：定时器
来源：http://www.blog.tarul.cn/Article/details/gertwqpde.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.tarul.cn/Article/details/gzcpoogat.sHtML

[U104] JS：防抖
来源：http://blog.epnwcf.com/Article/details/gjmpqvjhh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/gmvuketmb.sHtML

[U105] JS：节流
来源：http://m.share.epnwcf.com/Article/details/gpepnlwnf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.sjlbkw.cn/Article/details/ghvohtsxf.sHtML

[U106] JS：日期格式化
来源：http://mobile.vehdjk.com/Article/details/goeiiwpzm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.sjlbkw.cn/Article/details/ggcnkbecb.sHtML

[U107] JS：数字千分位
来源：http://m.share.sjlbkw.cn/Article/details/gomtyzmrw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.tarul.cn/Article/details/gzqlmymxx.sHtML

[U108] JS：随机整数
来源：http://wap.tarul.cn/Article/details/gdgotyjyp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.sjlbkw.cn/Article/details/gknbtfeof.sHtML

[U109] JS：数组分组
来源：http://m.share.tarul.cn/Article/details/gpcuxcaem.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.bbcook.cn/Article/details/gfjbcaadr.sHtML

[U110] JS：数组分块
来源：http://read.share.sjlbkw.cn/Article/details/gbefbfbtd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.bbcook.cn/Article/details/gqagyfddt.sHtML

[U111] JS：对象转 Map
来源：http://baike.vehdjk.com/Article/details/gbltaiapu.sHtML

new Map(Object.entries(obj))
来源：http://read.share.bbcook.cn/Article/details/guhfjwieo.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.yfazqb.com/Article/details/gvtninpqn.sHtML

"7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/gpnvcwhtw.sHtML

[U113] JS：正则替换全部
来源：http://3g.epnwcf.com/Article/details/gknphgdbe.sHtML

s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/grseuynan.sHtML

[U114] JS：JSON 深比较
来源：http://3g.tarul.cn/Article/details/gakptxtxu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.sjlbkw.cn/Article/details/ggpljpghg.sHtML

[U115] JS：生成 UUID
来源：http://3g.tarul.cn/Article/details/gcnchnghn.sHtML

crypto.randomUUID()
来源：http://read.share.fktsv.cn/Article/details/greclclxh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.vehdjk.com/Article/details/gfwwluabu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.tarul.cn/Article/details/gjbsitned.sHtML

[U117] JS：单元测试
来源：http://read.share.bbcook.cn/Article/details/glpyfytzv.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.tarul.cn/Article/details/gvtltotbu.sHtML

[U118] JS：开发服务器
来源：http://www.share.yfazqb.com/Article/details/gxgaunzea.sHtML

npm i -D vite;  npx vite
来源：http://blog.sjlbkw.cn/Article/details/gqafpmhwk.sHtML

[U119] JS：生产构建
来源：http://mobile.bbcook.cn/Article/details/glbbawtfs.sHtML

npx vite build
来源：http://read.share.epnwcf.com/Article/details/gpmsakqjx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.sjlbkw.cn/Article/details/goiwpguqq.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.sjlbkw.cn/Article/details/gpxsukxjz.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gjkoggtnr.sHtML

统计汇总
来源：http://m.share.epnwcf.com/Article/details/gqnyioodb.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gugreijbb.sHtML

按语言统计（条）：
来源：http://mobile.sjlbkw.cn/Article/details/gndntbdqe.sHtML

Python ......... 252
来源：http://read.share.sjlbkw.cn/Article/details/gfpyrcuku.sHtML

PHP ............ 252
来源：http://baike.epnwcf.com/Article/details/gxzcnjrpr.sHtML

JavaScript ..... 252
来源：http://www.blog.tarul.cn/Article/details/gayxsdlrc.sHtML

TypeScript ..... 212
来源：http://www.share.yfazqb.com/Article/details/gtciagyuc.sHtML

Java ........... 212
来源：http://www.m.share.bbcook.cn/Article/details/gysxbeclb.sHtML

Go ............. 212
来源：http://read.share.yfazqb.com/Article/details/gbzurjhpa.sHtML

Ruby ........... 212
来源：http://read.share.bbcook.cn/Article/details/gzzjvltju.sHtML

C# ............. 212
来源：http://wap.tarul.cn/Article/details/gdmtghnfm.sHtML

C .............. 30
来源：http://www.share.tarul.cn/Article/details/gquhdwuta.sHtML

C++ ............ 30
来源：http://www.share.vehdjk.com/Article/details/gkzfjlvrf.sHtML

SQL ............ 90
来源：http://blog.vehdjk.com/Article/details/glgnfiiep.sHtML

Bash ........... 80
来源：http://mobile.tarul.cn/Article/details/gajfuyvau.sHtML

Kotlin ......... 15
来源：http://www.share.tarul.cn/Article/details/gnhbriggp.sHtML

Swift .......... 15
来源：http://mobile.vehdjk.com/Article/details/gkclrhztn.sHtML

Lua ............ 10
来源：http://mobile.yfazqb.com/Article/details/ggxqqrbzf.sHtML

Perl ........... 10
来源：http://www.share.vehdjk.com/Article/details/gvkddgfts.sHtML

Scala .......... 10
来源：http://read.share.tarul.cn/Article/details/ghrhxfybn.sHtML

------------------------------------
来源：http://m.share.vehdjk.com/Article/details/gpumvjkog.sHtML

合计 ........... 2106 条
来源：http://www.m.share.yfazqb.com/Article/details/gsvselcst.sHtML

按章节统计：
来源：http://read.share.yfazqb.com/Article/details/gghzbktjh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.vehdjk.com/Article/details/glgqehzxi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.epnwcf.com/Article/details/ggvuuhlms.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fktsv.cn/Article/details/gctidtlha.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.epnwcf.com/Article/details/ghkcoxrnt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.bbcook.cn/Article/details/gfllekbzo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.vehdjk.com/Article/details/gtygbdtus.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.sjlbkw.cn/Article/details/ghcllucxe.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.sjlbkw.cn/Article/details/gfeqhpqqz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gvhrchsqr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fktsv.cn/Article/details/gfxongbgf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gucshoouf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gqviynmcg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/gubdgqpkp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.bbcook.cn/Article/details/gewtqlvvg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.bbcook.cn/Article/details/ghhjjeisg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/ghlhbpvsv.sHtML

Q SQL 专题                              90
来源：http://www.blog.vehdjk.com/Article/details/gxjyymzhk.sHtML

R Bash 专题                             80
来源：http://www.m.share.tarul.cn/Article/details/gjqpmjuzc.sHtML

S C / C++ 专题                          60
来源：http://mobile.yfazqb.com/Article/details/gvmjhdpwn.sHtML

T 其他语言补充                          60
来源：http://wap.vehdjk.com/Article/details/gxnlimyze.sHtML

U 高频实用片段                         120
来源：http://www.blog.epnwcf.com/Article/details/gjzwgabmd.sHtML

------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/gszeovbdt.sHtML

合计                                  2106 条
来源：http://read.share.epnwcf.com/Article/details/gpjosjkyg.sHtML

--------------------------------------------------------------------------------
来源：http://blog.bbcook.cn/Article/details/ghualyuaj.sHtML

使用提醒
来源：http://baike.yfazqb.com/Article/details/guyvxlpgo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.bbcook.cn/Article/details/goooqbezu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.yfazqb.com/Article/details/gicmiosrw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fktsv.cn/Article/details/gkhhnfhjw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fktsv.cn/Article/details/gevdvelmt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.tarul.cn/Article/details/gdvfaisjn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.epnwcf.com/Article/details/gdetulixu.sHtML

—— 文件结束 ——
来源：http://blog.vehdjk.com/Article/details/grhjubuwi.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/glbjkogvn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.vehdjk.com/Article/details/gftqxkjgk.sHtML

Common Programming Examples Cheat Book
来源：http://wap.bbcook.cn/Article/details/ggzdkkmmu.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ggyikhauy.sHtML

【收录内容】
来源：http://baike.yfazqb.com/Article/details/glsavbkpb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fktsv.cn/Article/details/gsludskdf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.yfazqb.com/Article/details/gplbyegee.sHtML

SQL · Bash · C · C++
来源：http://3g.yfazqb.com/Article/details/gndntdczn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.bbcook.cn/Article/details/gmsnnvexy.sHtML

【使用说明】
来源：http://mobile.sjlbkw.cn/Article/details/gqvnqarjw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.yfazqb.com/Article/details/gfaxgjuvu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.bbcook.cn/Article/details/guudzjomy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.yfazqb.com/Article/details/ghdoymrkf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.epnwcf.com/Article/details/gtxlgrxqu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.epnwcf.com/Article/details/gxgnbfrac.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.yfazqb.com/Article/details/gzxqwmits.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.sjlbkw.cn/Article/details/gyxhofvcr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.tarul.cn/Article/details/gcheimfeg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.bbcook.cn/Article/details/gcsrbofue.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.yfazqb.com/Article/details/gquvmurnp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.yfazqb.com/Article/details/ggjvdrupi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fktsv.cn/Article/details/gfxsfzhbl.sHtML

【文件统计】
来源：http://read.share.yfazqb.com/Article/details/gibhrvroy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.yfazqb.com/Article/details/gukzqhreq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.bbcook.cn/Article/details/gaxmsehqh.sHtML

目  录
来源：http://wap.tarul.cn/Article/details/gcishizit.sHtML

--------------------------------------------------------------------------------
来源：http://baike.tarul.cn/Article/details/gbhqummum.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.bbcook.cn/Article/details/gqmbevpyv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.sjlbkw.cn/Article/details/gpqpzbdky.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.fktsv.cn/Article/details/gztwuvfze.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.vehdjk.com/Article/details/gxmhrfubx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.tarul.cn/Article/details/gsskcsans.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fktsv.cn/Article/details/gwpuphfjn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.yfazqb.com/Article/details/gpcydriop.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.epnwcf.com/Article/details/gfgaziqji.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gtlmnbgee.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.vehdjk.com/Article/details/gewvzenoq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gyffuqhou.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/gmnbaeceq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.yfazqb.com/Article/details/gjrbznwzn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.bbcook.cn/Article/details/gaowdrmxt.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.vehdjk.com/Article/details/gomrjnktp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.bbcook.cn/Article/details/gfljghhpf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.bbcook.cn/Article/details/gxojpuxjw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fktsv.cn/Article/details/gpokbpmsf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.yfazqb.com/Article/details/gdjrxzbqq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.sjlbkw.cn/Article/details/gubnzntei.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnwapazs.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gjtfgfbzq.sHtML

A. 基础语法与类型
来源：http://wap.bbcook.cn/Article/details/gfhubowpo.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gmgmzlsxk.sHtML

[A01] Hello World
来源：http://baike.epnwcf.com/Article/details/gxkbygoke.sHtML

Py:   print("Hello, World!")
来源：http://www.share.yfazqb.com/Article/details/gvacjkhgz.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.yfazqb.com/Article/details/grvyybbam.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.bbcook.cn/Article/details/gvkpvhcgj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.epnwcf.com/Article/details/gjlnzxzmf.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.sjlbkw.cn/Article/details/godanjqqc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.yfazqb.com/Article/details/grtrxvqqo.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fktsv.cn/Article/details/geacaikih.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.yfazqb.com/Article/details/gwbkagqow.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.sjlbkw.cn/Article/details/gjnkzxynx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.bbcook.cn/Article/details/gkdbmswax.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.yfazqb.com/Article/details/gdieyqjew.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.vehdjk.com/Article/details/gtpjubmqp.sHtML


<!-- 参考信息 -->