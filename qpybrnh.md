代发 wailian999

[U29] Py：属性校验
来源：http://blog.yfazqb.com/Article/details/goxmftgsg.sHtML

@property 与 @x.setter 配合
来源：http://baike.vehdjk.com/Article/details/gzmjlukgj.sHtML

[U30] Py：数据类
来源：http://3g.sjlbkw.cn/Article/details/gnvcavvfh.sHtML

@dataclass(slots=True)
来源：http://m.share.yfazqb.com/Article/details/ggmcewagr.sHtML

[U31] Py：单测
来源：http://www.blog.bbcook.cn/Article/details/gptvkiayv.sHtML

python -m pytest -q
来源：http://mobile.sjlbkw.cn/Article/details/gaxorerpr.sHtML

[U32] Py：代码格式化
来源：http://www.share.sjlbkw.cn/Article/details/gcrluclcd.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.epnwcf.com/Article/details/gaztkqdmd.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fktsv.cn/Article/details/gxaklbogj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.yfazqb.com/Article/details/gndcttnfl.sHtML

[U34] Py：判断编码
来源：http://blog.bbcook.cn/Article/details/gccbkxupt.sHtML

chardet.detect(raw)
来源：http://m.share.epnwcf.com/Article/details/gwxspfwqp.sHtML

[U35] Py：发送邮件
来源：http://wap.vehdjk.com/Article/details/gqxuyiqcv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.sjlbkw.cn/Article/details/gmabjcxbw.sHtML

[U36] Py：定时任务
来源：http://read.share.sjlbkw.cn/Article/details/gmbditvbr.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.vehdjk.com/Article/details/ghzqtlbmy.sHtML

[U37] Py：读写 Excel
来源：http://www.share.epnwcf.com/Article/details/gmwghhsax.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.bbcook.cn/Article/details/gducftrtp.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.yfazqb.com/Article/details/gonrsjyjb.sHtML

Path(__file__).resolve().parent
来源：http://baike.tarul.cn/Article/details/gczctmlcx.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.tarul.cn/Article/details/gduodqgcb.sHtML

sys.stdout.isatty()
来源：http://read.share.bbcook.cn/Article/details/gqqblfbui.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fktsv.cn/Article/details/gyfepdljb.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/gxkprrkhj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.sjlbkw.cn/Article/details/gabasjvuz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.bbcook.cn/Article/details/gdqsiclcu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fktsv.cn/Article/details/gnnfcncso.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.sjlbkw.cn/Article/details/gegvzywpk.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.tarul.cn/Article/details/gdgzarxef.sHtML

namespace App\Http;
来源：http://baike.sjlbkw.cn/Article/details/gdlbfbncz.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.vehdjk.com/Article/details/gxihdmhiz.sHtML

declare(strict_types=1);
来源：http://3g.fktsv.cn/Article/details/gdaljpfje.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.tarul.cn/Article/details/gjozrbndv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gikpfdwcy.sHtML

[U46] PHP：可空类型
来源：http://read.share.bbcook.cn/Article/details/gpvwlifgp.sHtML

?string $name = null
来源：http://www.m.share.epnwcf.com/Article/details/gxitgwiqn.sHtML

[U47] PHP：联合类型
来源：http://m.share.fktsv.cn/Article/details/gpnrazqke.sHtML

int|string $id
来源：http://wap.sjlbkw.cn/Article/details/gxyqwoiqy.sHtML

[U48] PHP：纯枚举
来源：http://mobile.vehdjk.com/Article/details/ggrwtxtws.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.bbcook.cn/Article/details/gdlyypjnk.sHtML

[U49] PHP：只读属性
来源：http://wap.yfazqb.com/Article/details/gpwzcowdi.sHtML

public readonly string $name
来源：http://www.share.vehdjk.com/Article/details/gapcqyzov.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.sjlbkw.cn/Article/details/gdmwovwle.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fktsv.cn/Article/details/gmjrmqyct.sHtML

[U51] PHP：数组解构
来源：http://m.share.vehdjk.com/Article/details/glsodutdq.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.vehdjk.com/Article/details/ggqsvhsoc.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fktsv.cn/Article/details/gxpqyjzkz.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fktsv.cn/Article/details/ginpeftju.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.epnwcf.com/Article/details/gxyizwuue.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.vehdjk.com/Article/details/gsgjezsxj.sHtML

[U54] PHP：空安全调用
来源：http://3g.epnwcf.com/Article/details/ggbnwilhw.sHtML

$obj?->method()
来源：http://baike.tarul.cn/Article/details/gtkkjxevc.sHtML

[U55] PHP：match 表达式
来源：http://blog.tarul.cn/Article/details/grqrlsipp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fktsv.cn/Article/details/gusgotpub.sHtML

[U56] PHP：命名参数
来源：http://www.share.epnwcf.com/Article/details/gloqivttl.sHtML

f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/ggatherqn.sHtML

[U57] PHP：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gekrhkkkt.sHtML

"值: {$a}"
来源：http://read.share.fktsv.cn/Article/details/gtokllift.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fktsv.cn/Article/details/gjzmnhffc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.vehdjk.com/Article/details/goeqqortm.sHtML

[U59] PHP：自定义排序
来源：http://m.share.epnwcf.com/Article/details/gajqdyhtl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.yfazqb.com/Article/details/gzpbmhadw.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.vehdjk.com/Article/details/ghougqvgt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.tarul.cn/Article/details/gzxhvfucc.sHtML

[U61] PHP：正则
来源：http://www.share.fktsv.cn/Article/details/gyqyjoufs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fktsv.cn/Article/details/gkacrofph.sHtML

[U62] PHP：日期对象
来源：http://3g.epnwcf.com/Article/details/gunygpcfs.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.tarul.cn/Article/details/gutwrpmcv.sHtML

[U63] PHP：文件读写
来源：http://read.share.bbcook.cn/Article/details/gdirphjgv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.yfazqb.com/Article/details/guhyapzke.sHtML

[U64] PHP：目录遍历
来源：http://wap.epnwcf.com/Article/details/glrdmwgtq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.yfazqb.com/Article/details/gnmhlddvy.sHtML

[U65] PHP：会话
来源：http://read.share.tarul.cn/Article/details/gskcjvbxb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/guyhdhkvk.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.tarul.cn/Article/details/gwshngigd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.tarul.cn/Article/details/gtgcmvfoj.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.bbcook.cn/Article/details/gnwsoatld.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.tarul.cn/Article/details/gqiadsmbv.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.tarul.cn/Article/details/gkavycuyq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fktsv.cn/Article/details/gyluxigjz.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.yfazqb.com/Article/details/glznpmjgh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fktsv.cn/Article/details/gjygzdilm.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.epnwcf.com/Article/details/gdptafffr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.tarul.cn/Article/details/gxkjboifk.sHtML

[U71] PHP：抛出异常
来源：http://blog.sjlbkw.cn/Article/details/gnitncbam.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fktsv.cn/Article/details/gegondjnu.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.epnwcf.com/Article/details/gsgcoahvy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fktsv.cn/Article/details/gntdqhxso.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.bbcook.cn/Article/details/gjrcjenyu.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.epnwcf.com/Article/details/grsilicpl.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.vehdjk.com/Article/details/gnjyjoino.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.sjlbkw.cn/Article/details/gkmorzkfo.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.sjlbkw.cn/Article/details/gvutnzpul.sHtML

composer require psr/container
来源：http://www.m.share.yfazqb.com/Article/details/gjckwyoln.sHtML

[U76] PHP：简单路由
来源：http://mobile.fktsv.cn/Article/details/gwnilfavq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.sjlbkw.cn/Article/details/gocnnjjsf.sHtML

[U77] PHP：模板渲染
来源：http://blog.tarul.cn/Article/details/gjiqxktpo.sHtML

composer require twig/twig
来源：http://m.share.sjlbkw.cn/Article/details/gkkolzjcr.sHtML

[U78] PHP：单元测试
来源：http://3g.vehdjk.com/Article/details/gojlszzvz.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.bbcook.cn/Article/details/grevqwqxj.sHtML

[U79] PHP：静态分析
来源：http://3g.epnwcf.com/Article/details/gxkcogiwc.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.epnwcf.com/Article/details/gebbauhfr.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.tarul.cn/Article/details/glzyeheen.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.tarul.cn/Article/details/gekvuhtyz.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fktsv.cn/Article/details/gronunstp.sHtML

npm init -y;  npm i express
来源：http://3g.epnwcf.com/Article/details/gfcntpsna.sHtML

[U82] JS：package.json 脚本
来源：http://3g.bbcook.cn/Article/details/gfhrfxlbl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.yfazqb.com/Article/details/gogmlreoz.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.bbcook.cn/Article/details/gxazbwalx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.tarul.cn/Article/details/gjdetiunx.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.vehdjk.com/Article/details/gfjxuegak.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.bbcook.cn/Article/details/gfyantbab.sHtML

[U85] JS：可选链
来源：http://3g.sjlbkw.cn/Article/details/gimerffky.sHtML

a?.b?.c
来源：http://mobile.vehdjk.com/Article/details/gdjepvbde.sHtML

[U86] JS：空值合并
来源：http://read.share.yfazqb.com/Article/details/gfrgwijhc.sHtML

a ?? b
来源：http://baike.epnwcf.com/Article/details/ghcjldkuq.sHtML

[U87] JS：解构默认值
来源：http://www.share.sjlbkw.cn/Article/details/gctmfltvg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.tarul.cn/Article/details/givibusnb.sHtML

[U88] JS：对象展开合并
来源：http://wap.vehdjk.com/Article/details/gngqsvlzr.sHtML

{ ...a, ...b }
来源：http://www.blog.sjlbkw.cn/Article/details/gxrmtresj.sHtML

[U89] JS：数组去重
来源：http://3g.tarul.cn/Article/details/grzmccckj.sHtML

[...new Set(arr)]
来源：http://blog.fktsv.cn/Article/details/gcbbugbky.sHtML

[U90] JS：数字数组排序
来源：http://wap.yfazqb.com/Article/details/ghlymejvs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/gstqtonpm.sHtML

[U91] JS：对象键值遍历
来源：http://wap.bbcook.cn/Article/details/gpcrbtlvl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.sjlbkw.cn/Article/details/gurjmqrln.sHtML

[U92] JS：深拷贝
来源：http://blog.sjlbkw.cn/Article/details/gnluhysof.sHtML

structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/gfwuknctn.sHtML

[U93] JS：模板字符串
来源：http://3g.sjlbkw.cn/Article/details/gcbiohcyp.sHtML

`共 ${n} 条`
来源：http://www.blog.yfazqb.com/Article/details/gzlwhrohg.sHtML

[U94] JS：箭头函数
来源：http://m.share.epnwcf.com/Article/details/ghizvavlr.sHtML

const double = x => x * 2;
来源：http://baike.sjlbkw.cn/Article/details/guqpbpgig.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.tarul.cn/Article/details/gpsamihnv.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.bbcook.cn/Article/details/ggudvjmxi.sHtML

[U96] JS：async/await 与异常
来源：http://blog.bbcook.cn/Article/details/gpdrlwapk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/gajqjiboq.sHtML

[U97] JS：并发请求
来源：http://m.share.epnwcf.com/Article/details/gvcwacsxn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/grzswhybx.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fktsv.cn/Article/details/ggutnnnwe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.vehdjk.com/Article/details/glxeuuifq.sHtML

[U99] JS：事件监听
来源：http://mobile.vehdjk.com/Article/details/ggxtudkma.sHtML

el.addEventListener("click", e => {})
来源：http://3g.epnwcf.com/Article/details/gjfgafsyq.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.tarul.cn/Article/details/gjghwgzxz.sHtML

document.querySelector(".item")
来源：http://www.m.share.yfazqb.com/Article/details/grzkteian.sHtML

[U101] JS：classList 操作
来源：http://m.share.fktsv.cn/Article/details/gzcryyfqf.sHtML

el.classList.toggle("active")
来源：http://wap.vehdjk.com/Article/details/gosqtaqkx.sHtML

[U102] JS：本地存储
来源：http://www.blog.yfazqb.com/Article/details/gfxvwlocx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.vehdjk.com/Article/details/gteyqdnev.sHtML

[U103] JS：定时器
来源：http://blog.bbcook.cn/Article/details/gguchlvry.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.tarul.cn/Article/details/gwsjzyurc.sHtML

[U104] JS：防抖
来源：http://www.blog.tarul.cn/Article/details/gqoaepddx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gibosarlx.sHtML

[U105] JS：节流
来源：http://3g.sjlbkw.cn/Article/details/glchtprqq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.epnwcf.com/Article/details/gsgghqhdw.sHtML

[U106] JS：日期格式化
来源：http://read.share.vehdjk.com/Article/details/galftnypw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.sjlbkw.cn/Article/details/glecipkww.sHtML

[U107] JS：数字千分位
来源：http://m.share.bbcook.cn/Article/details/gcmumgqor.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.epnwcf.com/Article/details/giaywrdlg.sHtML

[U108] JS：随机整数
来源：http://www.m.share.tarul.cn/Article/details/gwhylagom.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.tarul.cn/Article/details/gumqehwek.sHtML

[U109] JS：数组分组
来源：http://mobile.epnwcf.com/Article/details/gborttksx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fktsv.cn/Article/details/gepxayljk.sHtML

[U110] JS：数组分块
来源：http://wap.fktsv.cn/Article/details/gfyoetpbq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fktsv.cn/Article/details/gegyumdov.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.yfazqb.com/Article/details/gfmiadlya.sHtML

new Map(Object.entries(obj))
来源：http://read.share.bbcook.cn/Article/details/gfqawpojz.sHtML

[U112] JS：字符串补位
来源：http://mobile.bbcook.cn/Article/details/gkqtftuvq.sHtML

"7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/gevjmtdap.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.bbcook.cn/Article/details/gcwwrfubf.sHtML

s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gwikfuzij.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.sjlbkw.cn/Article/details/gvxohnkgt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/gkdjbjhhm.sHtML

[U115] JS：生成 UUID
来源：http://wap.yfazqb.com/Article/details/gegssaryu.sHtML

crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/guruhigga.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.vehdjk.com/Article/details/gzbxribcd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.epnwcf.com/Article/details/gslmylsfk.sHtML

[U117] JS：单元测试
来源：http://baike.vehdjk.com/Article/details/gbkyklsro.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.bbcook.cn/Article/details/gyygmngwb.sHtML

[U118] JS：开发服务器
来源：http://3g.tarul.cn/Article/details/gfatufoqm.sHtML

npm i -D vite;  npx vite
来源：http://blog.sjlbkw.cn/Article/details/gcnwggowl.sHtML

[U119] JS：生产构建
来源：http://blog.fktsv.cn/Article/details/gswmarbnn.sHtML

npx vite build
来源：http://baike.vehdjk.com/Article/details/gxyiqkqgb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fktsv.cn/Article/details/ghiuskoal.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.yfazqb.com/Article/details/grzrllmax.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gpsjjawiq.sHtML

统计汇总
来源：http://m.share.yfazqb.com/Article/details/gqvcocnxp.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/geunxzpvj.sHtML

按语言统计（条）：
来源：http://m.share.yfazqb.com/Article/details/geycbawzf.sHtML

Python ......... 252
来源：http://3g.vehdjk.com/Article/details/gulgtklkg.sHtML

PHP ............ 252
来源：http://mobile.sjlbkw.cn/Article/details/gseiuropa.sHtML

JavaScript ..... 252
来源：http://m.share.yfazqb.com/Article/details/gpmanyddz.sHtML

TypeScript ..... 212
来源：http://m.share.epnwcf.com/Article/details/gtjezqpmt.sHtML

Java ........... 212
来源：http://mobile.tarul.cn/Article/details/gdcmjtrsc.sHtML

Go ............. 212
来源：http://mobile.epnwcf.com/Article/details/gppqtlfyd.sHtML

Ruby ........... 212
来源：http://www.share.vehdjk.com/Article/details/gcyvjjuts.sHtML

C# ............. 212
来源：http://read.share.epnwcf.com/Article/details/gaapiwvaj.sHtML

C .............. 30
来源：http://mobile.sjlbkw.cn/Article/details/gzbnhzbaz.sHtML

C++ ............ 30
来源：http://blog.fktsv.cn/Article/details/gqlvypfuv.sHtML

SQL ............ 90
来源：http://www.m.share.vehdjk.com/Article/details/gpipykfse.sHtML

Bash ........... 80
来源：http://blog.tarul.cn/Article/details/gojwfvhtr.sHtML

Kotlin ......... 15
来源：http://www.share.tarul.cn/Article/details/gszxrugpc.sHtML

Swift .......... 15
来源：http://www.blog.epnwcf.com/Article/details/gvypizwqb.sHtML

Lua ............ 10
来源：http://www.m.share.yfazqb.com/Article/details/gxyphsuto.sHtML

Perl ........... 10
来源：http://www.m.share.bbcook.cn/Article/details/gwyghluat.sHtML

Scala .......... 10
来源：http://www.share.fktsv.cn/Article/details/gbnqztsih.sHtML

------------------------------------
来源：http://blog.fktsv.cn/Article/details/gxsxriwci.sHtML

合计 ........... 2106 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gvehxuumt.sHtML

按章节统计：
来源：http://read.share.bbcook.cn/Article/details/glbnnkmqo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.sjlbkw.cn/Article/details/gcivbpvtf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.vehdjk.com/Article/details/gjdivbxwc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fktsv.cn/Article/details/gciopjsmw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.tarul.cn/Article/details/ggvxkwtma.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.yfazqb.com/Article/details/gkpyccqli.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.yfazqb.com/Article/details/gedaayzuu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.yfazqb.com/Article/details/gncfngkfy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.tarul.cn/Article/details/gxubeucii.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/grxtfursv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fktsv.cn/Article/details/gavivanpi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fktsv.cn/Article/details/guxlxcunb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/gfrxaodwq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fktsv.cn/Article/details/gwqqbzqtv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.bbcook.cn/Article/details/goyciaybh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.vehdjk.com/Article/details/gaxycurmh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gvwrtasbt.sHtML

Q SQL 专题                              90
来源：http://3g.fktsv.cn/Article/details/gmdghqogt.sHtML

R Bash 专题                             80
来源：http://3g.vehdjk.com/Article/details/gpjekrvoq.sHtML

S C / C++ 专题                          60
来源：http://3g.tarul.cn/Article/details/gwptnjwij.sHtML

T 其他语言补充                          60
来源：http://m.share.vehdjk.com/Article/details/gmpyilili.sHtML

U 高频实用片段                         120
来源：http://baike.yfazqb.com/Article/details/grcrdewgc.sHtML

------------------------------------
来源：http://blog.epnwcf.com/Article/details/gioiogswz.sHtML

合计                                  2106 条
来源：http://read.share.tarul.cn/Article/details/gapqskfzm.sHtML

--------------------------------------------------------------------------------
来源：http://blog.epnwcf.com/Article/details/gaushxmmb.sHtML

使用提醒
来源：http://www.blog.sjlbkw.cn/Article/details/gtwtmsnjd.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gcribsucr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.tarul.cn/Article/details/gdhkiogpx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.vehdjk.com/Article/details/gwfdbhkeg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.vehdjk.com/Article/details/ggebrtghe.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.sjlbkw.cn/Article/details/gvtbvuivz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.tarul.cn/Article/details/gmriupnej.sHtML

—— 文件结束 ——
来源：http://m.share.sjlbkw.cn/Article/details/guhrocelc.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gvdibyngl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fktsv.cn/Article/details/gtgqpyzsn.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.vehdjk.com/Article/details/gqnbrnsxw.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gibtrmqlt.sHtML

【收录内容】
来源：http://3g.epnwcf.com/Article/details/gtttixmkc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.tarul.cn/Article/details/goatmjpxd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.sjlbkw.cn/Article/details/gdjxfqugw.sHtML

SQL · Bash · C · C++
来源：http://mobile.yfazqb.com/Article/details/guletzczl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.vehdjk.com/Article/details/gauiogznk.sHtML

【使用说明】
来源：http://baike.epnwcf.com/Article/details/gxeugaqgb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fktsv.cn/Article/details/gmlyompae.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.epnwcf.com/Article/details/gdjdixxmr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.sjlbkw.cn/Article/details/grnjrozlo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.bbcook.cn/Article/details/gtevzmggu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.tarul.cn/Article/details/girrimqvu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.sjlbkw.cn/Article/details/glryenbgo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.tarul.cn/Article/details/gzyyroqki.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.bbcook.cn/Article/details/ghizpfgrj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.vehdjk.com/Article/details/gzgszftrx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.epnwcf.com/Article/details/gtoizyfmx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.bbcook.cn/Article/details/gpajihmzp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.bbcook.cn/Article/details/gvuyhswdw.sHtML

【文件统计】
来源：http://read.share.epnwcf.com/Article/details/gpxkxuthc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.epnwcf.com/Article/details/gbbxmowco.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fktsv.cn/Article/details/gvsfmolgl.sHtML

目  录
来源：http://www.m.share.epnwcf.com/Article/details/gndekvyzj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.tarul.cn/Article/details/gikcgycgp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.sjlbkw.cn/Article/details/gjxupqpkz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.yfazqb.com/Article/details/gadnmtsjh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.bbcook.cn/Article/details/gsntxaywj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fktsv.cn/Article/details/geuwsycxn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.vehdjk.com/Article/details/grfrdcvsh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.bbcook.cn/Article/details/grtadcnno.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fktsv.cn/Article/details/gpqyioahg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.epnwcf.com/Article/details/gabtdydcm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/gkzoggecx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.vehdjk.com/Article/details/gbjtdvhvl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.epnwcf.com/Article/details/gdouosvrt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.epnwcf.com/Article/details/gzwjilqzt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.sjlbkw.cn/Article/details/gqxvylwlg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.tarul.cn/Article/details/gntqjengw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.bbcook.cn/Article/details/gmevwnhww.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/gzvppraok.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.bbcook.cn/Article/details/gcyupbcgk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.vehdjk.com/Article/details/gkumqybtx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.yfazqb.com/Article/details/gybvqbszl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.yfazqb.com/Article/details/gzkjkcmax.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.sjlbkw.cn/Article/details/gdnkznvfe.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gwbfltsba.sHtML

A. 基础语法与类型
来源：http://wap.sjlbkw.cn/Article/details/gazqdmbju.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ggvvcpksl.sHtML

[A01] Hello World
来源：http://baike.epnwcf.com/Article/details/gjhipuxex.sHtML

Py:   print("Hello, World!")
来源：http://blog.bbcook.cn/Article/details/gnvkhujry.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.bbcook.cn/Article/details/gsjthwjtx.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.sjlbkw.cn/Article/details/geqkpgoup.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.tarul.cn/Article/details/glogmsncz.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.epnwcf.com/Article/details/gbkeheeew.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.vehdjk.com/Article/details/gxfvibufz.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fktsv.cn/Article/details/gyhsjxnaa.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.bbcook.cn/Article/details/gxsffkbvp.sHtML


<!-- 参考信息 -->