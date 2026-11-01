代发 wailian999

[U29] Py：属性校验
来源：http://www.blog.sjlbkw.cn/Article/details/gszbshobg.sHtML

@property 与 @x.setter 配合
来源：http://read.share.tarul.cn/Article/details/guhvfpkgr.sHtML

[U30] Py：数据类
来源：http://3g.fktsv.cn/Article/details/giixvwgwl.sHtML

@dataclass(slots=True)
来源：http://www.blog.bbcook.cn/Article/details/gatkczqht.sHtML

[U31] Py：单测
来源：http://blog.vehdjk.com/Article/details/gkpccyyge.sHtML

python -m pytest -q
来源：http://www.blog.fktsv.cn/Article/details/gmceqcduy.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.tarul.cn/Article/details/giextxfqn.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fktsv.cn/Article/details/ggctlgmur.sHtML

[U33] Py：打包发布
来源：http://blog.vehdjk.com/Article/details/gdrhaozxu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrilopfr.sHtML

[U34] Py：判断编码
来源：http://baike.tarul.cn/Article/details/gkxnghntp.sHtML

chardet.detect(raw)
来源：http://www.m.share.vehdjk.com/Article/details/gdobypedt.sHtML

[U35] Py：发送邮件
来源：http://blog.vehdjk.com/Article/details/gucgqogdk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.vehdjk.com/Article/details/gfmvsonum.sHtML

[U36] Py：定时任务
来源：http://www.m.share.bbcook.cn/Article/details/gxkwlbolp.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.epnwcf.com/Article/details/gfgndrghd.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.sjlbkw.cn/Article/details/gkydpoyfo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.yfazqb.com/Article/details/gkunicsoj.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.sjlbkw.cn/Article/details/ghvbqifmp.sHtML

Path(__file__).resolve().parent
来源：http://read.share.vehdjk.com/Article/details/gzqthxelk.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.tarul.cn/Article/details/giymuybit.sHtML

sys.stdout.isatty()
来源：http://baike.sjlbkw.cn/Article/details/ggxqctlxu.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.tarul.cn/Article/details/gnenivyvx.sHtML

print("err", file=sys.stderr)
来源：http://wap.bbcook.cn/Article/details/gnudsgdqn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.yfazqb.com/Article/details/gvubxsiam.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.vehdjk.com/Article/details/gzvtyxwjz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.bbcook.cn/Article/details/ggkjxkwcv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.vehdjk.com/Article/details/gkrgzkdyb.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.epnwcf.com/Article/details/gejbiulnb.sHtML

namespace App\Http;
来源：http://www.m.share.bbcook.cn/Article/details/gbghnpudz.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fktsv.cn/Article/details/gacncvyop.sHtML

declare(strict_types=1);
来源：http://wap.bbcook.cn/Article/details/gensbidhm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.yfazqb.com/Article/details/gphvaqkyn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/gubvvlvdf.sHtML

[U46] PHP：可空类型
来源：http://3g.bbcook.cn/Article/details/gsksoiwau.sHtML

?string $name = null
来源：http://3g.fktsv.cn/Article/details/gxogshflr.sHtML

[U47] PHP：联合类型
来源：http://www.blog.bbcook.cn/Article/details/grdaifvpz.sHtML

int|string $id
来源：http://www.blog.yfazqb.com/Article/details/ghykbfzvz.sHtML

[U48] PHP：纯枚举
来源：http://blog.bbcook.cn/Article/details/gxwkojgkv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.yfazqb.com/Article/details/gzucsyhct.sHtML

[U49] PHP：只读属性
来源：http://baike.sjlbkw.cn/Article/details/gcciywmfl.sHtML

public readonly string $name
来源：http://www.m.share.yfazqb.com/Article/details/gyqtusubj.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.tarul.cn/Article/details/gnxcvplsx.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.bbcook.cn/Article/details/gwhtbqdmy.sHtML

[U51] PHP：数组解构
来源：http://3g.tarul.cn/Article/details/grdlpfsdd.sHtML

[$a, $b] = $arr;
来源：http://3g.bbcook.cn/Article/details/gpthfhmff.sHtML

[U52] PHP：箭头函数
来源：http://blog.sjlbkw.cn/Article/details/gjvaynalw.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.sjlbkw.cn/Article/details/gmoacbnoj.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.vehdjk.com/Article/details/gpkltfrcy.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.epnwcf.com/Article/details/gkhancvwm.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fktsv.cn/Article/details/gwgujmlcm.sHtML

$obj?->method()
来源：http://www.share.yfazqb.com/Article/details/ghhogmoqz.sHtML

[U55] PHP：match 表达式
来源：http://read.share.tarul.cn/Article/details/gafbspaxc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fktsv.cn/Article/details/gjyaxoprf.sHtML

[U56] PHP：命名参数
来源：http://blog.tarul.cn/Article/details/gfpstvrkv.sHtML

f(a: 1, b: 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gtlpsbwzs.sHtML

[U57] PHP：字符串插值
来源：http://3g.tarul.cn/Article/details/gdnsjrkfo.sHtML

"值: {$a}"
来源：http://mobile.fktsv.cn/Article/details/gngpezlmq.sHtML

[U58] PHP：数组三件套
来源：http://mobile.sjlbkw.cn/Article/details/gzoyqqohi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.tarul.cn/Article/details/gtdmsxput.sHtML

[U59] PHP：自定义排序
来源：http://mobile.yfazqb.com/Article/details/gldioqfqn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.vehdjk.com/Article/details/gdpqidmxh.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.tarul.cn/Article/details/gdlpquhrx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.sjlbkw.cn/Article/details/gunlbkmgl.sHtML

[U61] PHP：正则
来源：http://www.share.vehdjk.com/Article/details/gflgsexqz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.bbcook.cn/Article/details/gdvozbfeg.sHtML

[U62] PHP：日期对象
来源：http://wap.epnwcf.com/Article/details/gbportklk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.epnwcf.com/Article/details/grquilsgg.sHtML

[U63] PHP：文件读写
来源：http://wap.fktsv.cn/Article/details/gihvefsai.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.vehdjk.com/Article/details/gictquodu.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.tarul.cn/Article/details/gyhlmoypp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.bbcook.cn/Article/details/gupltrdab.sHtML

[U65] PHP：会话
来源：http://baike.yfazqb.com/Article/details/gipxnbdws.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.vehdjk.com/Article/details/ggobqhesp.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.epnwcf.com/Article/details/gcvnwyhsz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gvpbiixfa.sHtML

[U67] PHP：处理文件上传
来源：http://blog.epnwcf.com/Article/details/gfdzboipx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.sjlbkw.cn/Article/details/gkdcpwsqn.sHtML

[U68] PHP：PDO 连接
来源：http://baike.bbcook.cn/Article/details/gewrdwtvg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.tarul.cn/Article/details/gdyevxxlc.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.yfazqb.com/Article/details/gimlbpykt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.bbcook.cn/Article/details/ghaunoylg.sHtML

[U70] PHP：PDO 事务
来源：http://baike.epnwcf.com/Article/details/gkhtftahd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fktsv.cn/Article/details/ghpatexih.sHtML

[U71] PHP：抛出异常
来源：http://blog.bbcook.cn/Article/details/gfowlpxil.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.vehdjk.com/Article/details/ggcxmxhpx.sHtML

[U72] PHP：写错误日志
来源：http://baike.bbcook.cn/Article/details/gcfhwigab.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.epnwcf.com/Article/details/guemyhbsh.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.yfazqb.com/Article/details/gzyolheox.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.vehdjk.com/Article/details/grvmxjgmz.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fktsv.cn/Article/details/gbxshprrn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.yfazqb.com/Article/details/gtloisycv.sHtML

[U75] PHP：依赖注入
来源：http://m.share.vehdjk.com/Article/details/gkirrckkw.sHtML

composer require psr/container
来源：http://blog.sjlbkw.cn/Article/details/gjgwmyark.sHtML

[U76] PHP：简单路由
来源：http://wap.fktsv.cn/Article/details/gbyvpwwsc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fktsv.cn/Article/details/gunkvrrpk.sHtML

[U77] PHP：模板渲染
来源：http://mobile.vehdjk.com/Article/details/gqibememk.sHtML

composer require twig/twig
来源：http://3g.sjlbkw.cn/Article/details/gafdibxca.sHtML

[U78] PHP：单元测试
来源：http://baike.yfazqb.com/Article/details/gzcniogja.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.sjlbkw.cn/Article/details/gasbgliog.sHtML

[U79] PHP：静态分析
来源：http://wap.tarul.cn/Article/details/gktkqekhh.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.sjlbkw.cn/Article/details/grwtwcbmh.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.sjlbkw.cn/Article/details/gygcektoa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.sjlbkw.cn/Article/details/ghccpfthh.sHtML

[U81] JS：初始化项目
来源：http://wap.tarul.cn/Article/details/gvqdfucfd.sHtML

npm init -y;  npm i express
来源：http://www.blog.fktsv.cn/Article/details/goxnqekxw.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.tarul.cn/Article/details/gmdkfinan.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.epnwcf.com/Article/details/gbzjboolo.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.bbcook.cn/Article/details/gsuozzkcr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.tarul.cn/Article/details/gjxdszuqz.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fktsv.cn/Article/details/gpabyikip.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.yfazqb.com/Article/details/gumxaozym.sHtML

[U85] JS：可选链
来源：http://3g.bbcook.cn/Article/details/gbfbazzan.sHtML

a?.b?.c
来源：http://mobile.yfazqb.com/Article/details/gkmxiudka.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fktsv.cn/Article/details/gyqztypus.sHtML

a ?? b
来源：http://baike.vehdjk.com/Article/details/gytiaaabw.sHtML

[U87] JS：解构默认值
来源：http://read.share.epnwcf.com/Article/details/glcsmdelt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.epnwcf.com/Article/details/geujrzvre.sHtML

[U88] JS：对象展开合并
来源：http://www.share.tarul.cn/Article/details/gnsltygkq.sHtML

{ ...a, ...b }
来源：http://m.share.vehdjk.com/Article/details/gvrqatyux.sHtML

[U89] JS：数组去重
来源：http://www.blog.epnwcf.com/Article/details/gbjbnfjei.sHtML

[...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gfvxvfbdx.sHtML

[U90] JS：数字数组排序
来源：http://read.share.vehdjk.com/Article/details/guualmjsd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gewuwytjb.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.bbcook.cn/Article/details/grebuzffw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.epnwcf.com/Article/details/gmbcbiags.sHtML

[U92] JS：深拷贝
来源：http://3g.tarul.cn/Article/details/gqluzgrub.sHtML

structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/gjrgxdzvm.sHtML

[U93] JS：模板字符串
来源：http://www.blog.bbcook.cn/Article/details/glbxjpbus.sHtML

`共 ${n} 条`
来源：http://blog.epnwcf.com/Article/details/gbauuofoq.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gsznbviiv.sHtML

const double = x => x * 2;
来源：http://blog.fktsv.cn/Article/details/ghscemzfh.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.sjlbkw.cn/Article/details/gvchtaxdf.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fktsv.cn/Article/details/gyqmduqwo.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.vehdjk.com/Article/details/gytkochyw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gszrmigdl.sHtML

[U97] JS：并发请求
来源：http://3g.tarul.cn/Article/details/gzmapquab.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/glivobdqx.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.epnwcf.com/Article/details/gcwbizbtv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fktsv.cn/Article/details/gbsfajzdh.sHtML

[U99] JS：事件监听
来源：http://mobile.bbcook.cn/Article/details/gairaxevx.sHtML

el.addEventListener("click", e => {})
来源：http://baike.tarul.cn/Article/details/gffqrydwu.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.vehdjk.com/Article/details/gvfhwtyra.sHtML

document.querySelector(".item")
来源：http://read.share.tarul.cn/Article/details/gxgwgymqj.sHtML

[U101] JS：classList 操作
来源：http://mobile.vehdjk.com/Article/details/gzntkeuhv.sHtML

el.classList.toggle("active")
来源：http://baike.yfazqb.com/Article/details/grcruvhbb.sHtML

[U102] JS：本地存储
来源：http://www.share.fktsv.cn/Article/details/guxhsodej.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.yfazqb.com/Article/details/gvjzpjguk.sHtML

[U103] JS：定时器
来源：http://mobile.yfazqb.com/Article/details/gkdxjalaa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.vehdjk.com/Article/details/gldxilosh.sHtML

[U104] JS：防抖
来源：http://baike.yfazqb.com/Article/details/gspoqvmpl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.vehdjk.com/Article/details/gzexexaba.sHtML

[U105] JS：节流
来源：http://3g.fktsv.cn/Article/details/gwwwrxwyg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.tarul.cn/Article/details/gnhhejcka.sHtML

[U106] JS：日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/giszeovpv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.epnwcf.com/Article/details/gldemcwud.sHtML

[U107] JS：数字千分位
来源：http://wap.tarul.cn/Article/details/gxvpaujnl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.yfazqb.com/Article/details/gmafsttaw.sHtML

[U108] JS：随机整数
来源：http://blog.fktsv.cn/Article/details/gpegavlsf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.sjlbkw.cn/Article/details/gtjamdiwb.sHtML

[U109] JS：数组分组
来源：http://blog.tarul.cn/Article/details/gpedzqgqd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fktsv.cn/Article/details/gqnbcgfrw.sHtML

[U110] JS：数组分块
来源：http://mobile.vehdjk.com/Article/details/gknfysduf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.tarul.cn/Article/details/gnrgiioou.sHtML

[U111] JS：对象转 Map
来源：http://wap.vehdjk.com/Article/details/gbpfcudlp.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlqtucnz.sHtML

[U112] JS：字符串补位
来源：http://wap.vehdjk.com/Article/details/gsqxqcfxd.sHtML

"7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gtleubkuk.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.epnwcf.com/Article/details/gkmkjbics.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/glbniuxqa.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.bbcook.cn/Article/details/gpwfvvgpr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.epnwcf.com/Article/details/gsazysbza.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fktsv.cn/Article/details/gbrbejwsg.sHtML

crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/gxmbfujpl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fktsv.cn/Article/details/gqtarlkxx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/godstqwoh.sHtML

[U117] JS：单元测试
来源：http://www.blog.sjlbkw.cn/Article/details/gsjhobmko.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.tarul.cn/Article/details/gnboocirb.sHtML

[U118] JS：开发服务器
来源：http://www.share.fktsv.cn/Article/details/gyujumzgf.sHtML

npm i -D vite;  npx vite
来源：http://mobile.vehdjk.com/Article/details/gpquzlzvo.sHtML

[U119] JS：生产构建
来源：http://3g.tarul.cn/Article/details/ggdqwopso.sHtML

npx vite build
来源：http://www.m.share.yfazqb.com/Article/details/gjwmbgbcc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fktsv.cn/Article/details/gyuzijlne.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.bbcook.cn/Article/details/gxlwcdwjp.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gblluggca.sHtML

统计汇总
来源：http://www.share.fktsv.cn/Article/details/ghdueacvy.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ghmlxtrmj.sHtML

按语言统计（条）：
来源：http://www.blog.fktsv.cn/Article/details/gzydekcnc.sHtML

Python ......... 252
来源：http://m.share.sjlbkw.cn/Article/details/glyibclhk.sHtML

PHP ............ 252
来源：http://read.share.bbcook.cn/Article/details/gotwawzqj.sHtML

JavaScript ..... 252
来源：http://wap.bbcook.cn/Article/details/gjmwyagsm.sHtML

TypeScript ..... 212
来源：http://www.m.share.bbcook.cn/Article/details/grfmueziw.sHtML

Java ........... 212
来源：http://wap.fktsv.cn/Article/details/gzhecxvln.sHtML

Go ............. 212
来源：http://read.share.tarul.cn/Article/details/geshvjjog.sHtML

Ruby ........... 212
来源：http://read.share.yfazqb.com/Article/details/gngssxnla.sHtML

C# ............. 212
来源：http://www.share.vehdjk.com/Article/details/gwhtputir.sHtML

C .............. 30
来源：http://wap.vehdjk.com/Article/details/gccmlwhcm.sHtML

C++ ............ 30
来源：http://blog.yfazqb.com/Article/details/ggvnuumih.sHtML

SQL ............ 90
来源：http://read.share.tarul.cn/Article/details/glyklkhil.sHtML

Bash ........... 80
来源：http://blog.sjlbkw.cn/Article/details/grfqaiexp.sHtML

Kotlin ......... 15
来源：http://www.share.tarul.cn/Article/details/giyvxdvis.sHtML

Swift .......... 15
来源：http://wap.vehdjk.com/Article/details/gjoxpyhme.sHtML

Lua ............ 10
来源：http://baike.epnwcf.com/Article/details/gecmtpaxt.sHtML

Perl ........... 10
来源：http://read.share.epnwcf.com/Article/details/gemkttjkx.sHtML

Scala .......... 10
来源：http://mobile.sjlbkw.cn/Article/details/gnwckfird.sHtML

------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gdzqjiffa.sHtML

合计 ........... 2106 条
来源：http://www.m.share.bbcook.cn/Article/details/gizqapzid.sHtML

按章节统计：
来源：http://read.share.vehdjk.com/Article/details/gkacgldfa.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.bbcook.cn/Article/details/grtdliaxy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.yfazqb.com/Article/details/goynpydff.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.bbcook.cn/Article/details/gkwaqdqhd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.vehdjk.com/Article/details/gzauyvszy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fktsv.cn/Article/details/gcjtvmluy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.bbcook.cn/Article/details/ghwwfidma.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.sjlbkw.cn/Article/details/gurdozwtm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.sjlbkw.cn/Article/details/gctvpysfv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/ghttcujys.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.sjlbkw.cn/Article/details/grmocfsiw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/gptwbcpdi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/ghsuzpkrt.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/glqhstdyk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.vehdjk.com/Article/details/goddwhttc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.vehdjk.com/Article/details/gxhpxwovo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gpcquqffi.sHtML

Q SQL 专题                              90
来源：http://blog.fktsv.cn/Article/details/gjxzvobzi.sHtML

R Bash 专题                             80
来源：http://www.m.share.epnwcf.com/Article/details/grcfwrtnh.sHtML

S C / C++ 专题                          60
来源：http://www.share.sjlbkw.cn/Article/details/ggdvdobkg.sHtML

T 其他语言补充                          60
来源：http://www.blog.epnwcf.com/Article/details/gwxsmlilz.sHtML

U 高频实用片段                         120
来源：http://read.share.sjlbkw.cn/Article/details/gdbsqdgfd.sHtML

------------------------------------
来源：http://wap.yfazqb.com/Article/details/gqcvwguck.sHtML

合计                                  2106 条
来源：http://m.share.tarul.cn/Article/details/gemvyfnag.sHtML

--------------------------------------------------------------------------------
来源：http://3g.yfazqb.com/Article/details/gghzqdjxv.sHtML

使用提醒
来源：http://mobile.fktsv.cn/Article/details/gbpuxsevu.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/gwetraipt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fktsv.cn/Article/details/gnueaxyfb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.epnwcf.com/Article/details/gtqwyvhlb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.sjlbkw.cn/Article/details/ggygvwlzw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.vehdjk.com/Article/details/gpxhtwsnn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fktsv.cn/Article/details/gzcbkjzeg.sHtML

—— 文件结束 ——
来源：http://www.share.vehdjk.com/Article/details/gdhwfqqud.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gefkijmpp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.tarul.cn/Article/details/gwrvgvqlt.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.yfazqb.com/Article/details/gjbzvjwdh.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gxhqlqisy.sHtML

【收录内容】
来源：http://www.blog.sjlbkw.cn/Article/details/guyznjqky.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.vehdjk.com/Article/details/gmrrvnnjv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.bbcook.cn/Article/details/gcqqqxuqy.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.bbcook.cn/Article/details/gfyudzeph.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.vehdjk.com/Article/details/ggznajtws.sHtML

【使用说明】
来源：http://baike.fktsv.cn/Article/details/gtpawqogm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.tarul.cn/Article/details/gtrtbpjdy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.tarul.cn/Article/details/giowxlknn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fktsv.cn/Article/details/gnuckbsvg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.bbcook.cn/Article/details/gcyqsperm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.bbcook.cn/Article/details/gsgqgjptw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.yfazqb.com/Article/details/gyidjvcvr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.vehdjk.com/Article/details/grobfedpt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.bbcook.cn/Article/details/gscsbrhas.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.yfazqb.com/Article/details/gpjqmltoq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.sjlbkw.cn/Article/details/gctjxcxei.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.bbcook.cn/Article/details/gnnapmupw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.epnwcf.com/Article/details/gsqutnxdl.sHtML

【文件统计】
来源：http://baike.yfazqb.com/Article/details/gwsuilggn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.epnwcf.com/Article/details/goehpsjuo.sHtML

--------------------------------------------------------------------------------
来源：http://blog.yfazqb.com/Article/details/glbtydefn.sHtML

目  录
来源：http://wap.yfazqb.com/Article/details/gweoeywog.sHtML

--------------------------------------------------------------------------------
来源：http://3g.tarul.cn/Article/details/glskrdynz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gjwkevhqk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.sjlbkw.cn/Article/details/gcasexesk.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fktsv.cn/Article/details/gbqrbjnpg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.epnwcf.com/Article/details/gtecaawio.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.tarul.cn/Article/details/gbmhvgqpd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.yfazqb.com/Article/details/gdsgsuiov.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.vehdjk.com/Article/details/gmhikfyaz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.vehdjk.com/Article/details/gylabkdhj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.bbcook.cn/Article/details/gmbraojtr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.tarul.cn/Article/details/gffwqfabg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/gkmpoudne.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.epnwcf.com/Article/details/gpcuuogit.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fktsv.cn/Article/details/gplnxyadv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.epnwcf.com/Article/details/gfwlikpcj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fktsv.cn/Article/details/gagnolglz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/glzubmkuw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.sjlbkw.cn/Article/details/gkzbnhlcy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.bbcook.cn/Article/details/gfuhiuuue.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fktsv.cn/Article/details/gdoqhxvmr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.vehdjk.com/Article/details/gnyydyocd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fktsv.cn/Article/details/gsfumttzb.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxknqvzhc.sHtML

A. 基础语法与类型
来源：http://m.share.tarul.cn/Article/details/gsqyoxqzj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/ghvendqgx.sHtML

[A01] Hello World
来源：http://3g.vehdjk.com/Article/details/gorifezib.sHtML

Py:   print("Hello, World!")
来源：http://3g.epnwcf.com/Article/details/gdtsnlzof.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.tarul.cn/Article/details/ghdnsvnlr.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.sjlbkw.cn/Article/details/gxwytwsrl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.yfazqb.com/Article/details/gzumavaev.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.epnwcf.com/Article/details/gsdndgezq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fktsv.cn/Article/details/guvanfzgi.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fktsv.cn/Article/details/gnaoioxky.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.sjlbkw.cn/Article/details/gzqhsmiij.sHtML


<!-- 参考信息 -->