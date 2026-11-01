代发 wailian999

[U37] Py：读写 Excel
来源：http://baike.vehdjk.com/Article/details/gfldhncry.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.sjlbkw.cn/Article/details/gdkuocppt.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fktsv.cn/Article/details/gdkjwpdrg.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.bbcook.cn/Article/details/gkwwroige.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.vehdjk.com/Article/details/ggrxzjkzt.sHtML

sys.stdout.isatty()
来源：http://read.share.tarul.cn/Article/details/ggvleflno.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.tarul.cn/Article/details/gtgxkrlqa.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fktsv.cn/Article/details/guhqddjdw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.epnwcf.com/Article/details/gqtgqaxtt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.epnwcf.com/Article/details/glojjmefe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.yfazqb.com/Article/details/gexmllekc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.bbcook.cn/Article/details/gznsckijz.sHtML

[U43] PHP：声明命名空间
来源：http://3g.epnwcf.com/Article/details/gzgainfum.sHtML

namespace App\Http;
来源：http://www.m.share.fktsv.cn/Article/details/gwumnrucz.sHtML

[U44] PHP：开启严格类型
来源：http://baike.tarul.cn/Article/details/gqsakahqd.sHtML

declare(strict_types=1);
来源：http://wap.tarul.cn/Article/details/gzhsbayue.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.vehdjk.com/Article/details/gmhwbmvgd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gcxrefpxc.sHtML

[U46] PHP：可空类型
来源：http://www.blog.bbcook.cn/Article/details/ghymirsin.sHtML

?string $name = null
来源：http://blog.vehdjk.com/Article/details/gzvjwopnz.sHtML

[U47] PHP：联合类型
来源：http://wap.yfazqb.com/Article/details/gmagkmsri.sHtML

int|string $id
来源：http://blog.tarul.cn/Article/details/grwgbhzar.sHtML

[U48] PHP：纯枚举
来源：http://mobile.yfazqb.com/Article/details/ggxiadpqk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fktsv.cn/Article/details/gssyrhdrc.sHtML

[U49] PHP：只读属性
来源：http://wap.sjlbkw.cn/Article/details/gtyjdfsgb.sHtML

public readonly string $name
来源：http://3g.fktsv.cn/Article/details/goenoidln.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.epnwcf.com/Article/details/gbebvxxjc.sHtML

public function __construct(private int $id) {}
来源：http://read.share.epnwcf.com/Article/details/gatbrlsce.sHtML

[U51] PHP：数组解构
来源：http://mobile.fktsv.cn/Article/details/gmstuchyj.sHtML

[$a, $b] = $arr;
来源：http://mobile.epnwcf.com/Article/details/gqitpcaag.sHtML

[U52] PHP：箭头函数
来源：http://www.share.sjlbkw.cn/Article/details/gfuneiqcf.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.yfazqb.com/Article/details/gxxwodnrq.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.sjlbkw.cn/Article/details/gneypwcjv.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.tarul.cn/Article/details/glqyrcyse.sHtML

[U54] PHP：空安全调用
来源：http://wap.epnwcf.com/Article/details/gtyaaxhkx.sHtML

$obj?->method()
来源：http://blog.epnwcf.com/Article/details/gidqjnysp.sHtML

[U55] PHP：match 表达式
来源：http://m.share.sjlbkw.cn/Article/details/gaibohquv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.bbcook.cn/Article/details/gkbzoqyyl.sHtML

[U56] PHP：命名参数
来源：http://m.share.sjlbkw.cn/Article/details/gupwpozry.sHtML

f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/geoshzfcw.sHtML

[U57] PHP：字符串插值
来源：http://read.share.tarul.cn/Article/details/gpxwpfpqf.sHtML

"值: {$a}"
来源：http://m.share.fktsv.cn/Article/details/gystksojk.sHtML

[U58] PHP：数组三件套
来源：http://read.share.epnwcf.com/Article/details/gfegmfkad.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.tarul.cn/Article/details/gqyfafzsb.sHtML

[U59] PHP：自定义排序
来源：http://mobile.bbcook.cn/Article/details/gnbahmusq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.tarul.cn/Article/details/gbhytebkw.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.tarul.cn/Article/details/gbpkjwzul.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.sjlbkw.cn/Article/details/gdizbpkwh.sHtML

[U61] PHP：正则
来源：http://mobile.tarul.cn/Article/details/gzoqxbgvz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gzjhxuysa.sHtML

[U62] PHP：日期对象
来源：http://3g.yfazqb.com/Article/details/giydlphhh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.yfazqb.com/Article/details/gkltcenvs.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.vehdjk.com/Article/details/ghhsgpimz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.sjlbkw.cn/Article/details/gbycazwrm.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.tarul.cn/Article/details/gxxomecfo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.vehdjk.com/Article/details/gdvohlnjc.sHtML

[U65] PHP：会话
来源：http://3g.tarul.cn/Article/details/ghqzlpuqg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gugonjajj.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.sjlbkw.cn/Article/details/gvyftsorv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fktsv.cn/Article/details/geugidqsu.sHtML

[U67] PHP：处理文件上传
来源：http://blog.yfazqb.com/Article/details/gdscrgsxq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.vehdjk.com/Article/details/gxqxayyod.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.vehdjk.com/Article/details/gwdsmoilt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.yfazqb.com/Article/details/grnudzbte.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.epnwcf.com/Article/details/gubhvgkpu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.bbcook.cn/Article/details/gcbovbfls.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fktsv.cn/Article/details/gyaeumyqx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.vehdjk.com/Article/details/gfpvscofm.sHtML

[U71] PHP：抛出异常
来源：http://wap.epnwcf.com/Article/details/gbwofetov.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.vehdjk.com/Article/details/glhdkywrm.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fktsv.cn/Article/details/gvimixeqc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.yfazqb.com/Article/details/gmsfmhvgd.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.yfazqb.com/Article/details/gzasuhhgg.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.epnwcf.com/Article/details/ggzmdkefi.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.yfazqb.com/Article/details/gjsgclhgy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.bbcook.cn/Article/details/ghmahtaht.sHtML

[U75] PHP：依赖注入
来源：http://wap.sjlbkw.cn/Article/details/gabafoecq.sHtML

composer require psr/container
来源：http://www.share.fktsv.cn/Article/details/gvohwlvzv.sHtML

[U76] PHP：简单路由
来源：http://baike.tarul.cn/Article/details/grysesaoh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.vehdjk.com/Article/details/grulspiqx.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.epnwcf.com/Article/details/gvusdozcu.sHtML

composer require twig/twig
来源：http://read.share.bbcook.cn/Article/details/gpegdxdxq.sHtML

[U78] PHP：单元测试
来源：http://blog.vehdjk.com/Article/details/glmymquit.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.yfazqb.com/Article/details/glmyvmkbg.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.tarul.cn/Article/details/gxiyguqkw.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.epnwcf.com/Article/details/ghbvuixnt.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.yfazqb.com/Article/details/girvhxvau.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.vehdjk.com/Article/details/gqwgwmlnm.sHtML

[U81] JS：初始化项目
来源：http://www.share.epnwcf.com/Article/details/gkljhorgf.sHtML

npm init -y;  npm i express
来源：http://baike.fktsv.cn/Article/details/gmzwwmstd.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.vehdjk.com/Article/details/golihzcvy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.bbcook.cn/Article/details/gwhrjhpgw.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.tarul.cn/Article/details/gnbmivbyr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fktsv.cn/Article/details/ggmhepbrc.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.epnwcf.com/Article/details/ghgvnsoyn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.yfazqb.com/Article/details/gxuqhvpbe.sHtML

[U85] JS：可选链
来源：http://baike.tarul.cn/Article/details/gplkrztzw.sHtML

a?.b?.c
来源：http://3g.vehdjk.com/Article/details/gguzudrmo.sHtML

[U86] JS：空值合并
来源：http://blog.vehdjk.com/Article/details/gjkilllqy.sHtML

a ?? b
来源：http://www.m.share.fktsv.cn/Article/details/gydsdtreb.sHtML

[U87] JS：解构默认值
来源：http://mobile.tarul.cn/Article/details/gopittclo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.epnwcf.com/Article/details/gtfkxzzop.sHtML

[U88] JS：对象展开合并
来源：http://3g.vehdjk.com/Article/details/gfytvmfbi.sHtML

{ ...a, ...b }
来源：http://www.share.vehdjk.com/Article/details/gkewvhlts.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fktsv.cn/Article/details/ggujgneas.sHtML

[...new Set(arr)]
来源：http://www.share.epnwcf.com/Article/details/gezmynavr.sHtML

[U90] JS：数字数组排序
来源：http://blog.bbcook.cn/Article/details/gqnneeqxj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/gptqrpaoo.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.yfazqb.com/Article/details/gfjgqxtrx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.epnwcf.com/Article/details/gsbjauhvz.sHtML

[U92] JS：深拷贝
来源：http://www.blog.tarul.cn/Article/details/gyfijgmqq.sHtML

structuredClone(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gnhmzpkwf.sHtML

[U93] JS：模板字符串
来源：http://www.share.bbcook.cn/Article/details/gltwebkxj.sHtML

`共 ${n} 条`
来源：http://mobile.yfazqb.com/Article/details/gfrrrrwxf.sHtML

[U94] JS：箭头函数
来源：http://mobile.epnwcf.com/Article/details/gnhbunipc.sHtML

const double = x => x * 2;
来源：http://mobile.epnwcf.com/Article/details/gtohhmytz.sHtML

[U95] JS：Promise 包装
来源：http://baike.sjlbkw.cn/Article/details/gdegibsko.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.epnwcf.com/Article/details/ghqciywpi.sHtML

[U96] JS：async/await 与异常
来源：http://baike.sjlbkw.cn/Article/details/gontcotba.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gxtmlrlga.sHtML

[U97] JS：并发请求
来源：http://mobile.tarul.cn/Article/details/ghegrsbia.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gmboieohd.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.tarul.cn/Article/details/gjgbpsqqv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.bbcook.cn/Article/details/gqrfjvkum.sHtML

[U99] JS：事件监听
来源：http://3g.bbcook.cn/Article/details/gbgwqbwdq.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.vehdjk.com/Article/details/giulzopuq.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.epnwcf.com/Article/details/gysrryfjt.sHtML

document.querySelector(".item")
来源：http://3g.fktsv.cn/Article/details/gbrjzzncr.sHtML

[U101] JS：classList 操作
来源：http://3g.bbcook.cn/Article/details/gepupgmxl.sHtML

el.classList.toggle("active")
来源：http://m.share.vehdjk.com/Article/details/ghokjzrks.sHtML

[U102] JS：本地存储
来源：http://read.share.vehdjk.com/Article/details/gpbfgkpks.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.epnwcf.com/Article/details/gjcgakapu.sHtML

[U103] JS：定时器
来源：http://3g.fktsv.cn/Article/details/gpkfutfya.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fktsv.cn/Article/details/gibtumbzl.sHtML

[U104] JS：防抖
来源：http://www.m.share.fktsv.cn/Article/details/grguknefv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/gblebrkzp.sHtML

[U105] JS：节流
来源：http://3g.fktsv.cn/Article/details/gjuszhtql.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.bbcook.cn/Article/details/gulsfdzqr.sHtML

[U106] JS：日期格式化
来源：http://m.share.epnwcf.com/Article/details/gyrbwffwg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.sjlbkw.cn/Article/details/gscdvyqgd.sHtML

[U107] JS：数字千分位
来源：http://wap.bbcook.cn/Article/details/gqohojclo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.epnwcf.com/Article/details/gytgchbza.sHtML

[U108] JS：随机整数
来源：http://3g.yfazqb.com/Article/details/gksryjvrw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.tarul.cn/Article/details/gvqbihkbv.sHtML

[U109] JS：数组分组
来源：http://www.blog.tarul.cn/Article/details/gkajohsnw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fktsv.cn/Article/details/gkiabador.sHtML

[U110] JS：数组分块
来源：http://read.share.yfazqb.com/Article/details/gopjdzwij.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.vehdjk.com/Article/details/gdcacnosg.sHtML

[U111] JS：对象转 Map
来源：http://mobile.vehdjk.com/Article/details/ghmkdpjim.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.epnwcf.com/Article/details/gloiyyzwq.sHtML

[U112] JS：字符串补位
来源：http://m.share.yfazqb.com/Article/details/gjjwchqvq.sHtML

"7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gevsqvttg.sHtML

[U113] JS：正则替换全部
来源：http://m.share.epnwcf.com/Article/details/gttvdvxls.sHtML

s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gyfknzncc.sHtML

[U114] JS：JSON 深比较
来源：http://wap.tarul.cn/Article/details/gjyubamtg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.vehdjk.com/Article/details/grecglryh.sHtML

[U115] JS：生成 UUID
来源：http://mobile.sjlbkw.cn/Article/details/gyvmmntgi.sHtML

crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gqukkvord.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fktsv.cn/Article/details/gbhywocpj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.yfazqb.com/Article/details/gdotsvndo.sHtML

[U117] JS：单元测试
来源：http://wap.epnwcf.com/Article/details/gbjucpjia.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.sjlbkw.cn/Article/details/gdycdyqqg.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.tarul.cn/Article/details/ggpazjqak.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.yfazqb.com/Article/details/gdnispnkf.sHtML

[U119] JS：生产构建
来源：http://baike.yfazqb.com/Article/details/gpqwfzsnu.sHtML

npx vite build
来源：http://m.share.yfazqb.com/Article/details/gkeqicpld.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fktsv.cn/Article/details/gsnryuzeb.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.tarul.cn/Article/details/gkzualwlc.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/guwvapohz.sHtML

统计汇总
来源：http://www.share.epnwcf.com/Article/details/gvjghssth.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gxemgcgnd.sHtML

按语言统计（条）：
来源：http://blog.tarul.cn/Article/details/gfzunhxgn.sHtML

Python ......... 252
来源：http://3g.fktsv.cn/Article/details/gecgvkzzt.sHtML

PHP ............ 252
来源：http://baike.tarul.cn/Article/details/gqsedyikp.sHtML

JavaScript ..... 252
来源：http://www.blog.vehdjk.com/Article/details/gdfdvucix.sHtML

TypeScript ..... 212
来源：http://baike.bbcook.cn/Article/details/gsfeimzrz.sHtML

Java ........... 212
来源：http://baike.vehdjk.com/Article/details/grcdeymuc.sHtML

Go ............. 212
来源：http://mobile.epnwcf.com/Article/details/gkzciagqx.sHtML

Ruby ........... 212
来源：http://read.share.sjlbkw.cn/Article/details/glwdgdkoq.sHtML

C# ............. 212
来源：http://read.share.yfazqb.com/Article/details/gwqkxwzpl.sHtML

C .............. 30
来源：http://www.m.share.epnwcf.com/Article/details/gnqpnvyfz.sHtML

C++ ............ 30
来源：http://www.share.tarul.cn/Article/details/gaqwcqeov.sHtML

SQL ............ 90
来源：http://www.m.share.vehdjk.com/Article/details/gdexhxntx.sHtML

Bash ........... 80
来源：http://read.share.fktsv.cn/Article/details/gvfwgdnlz.sHtML

Kotlin ......... 15
来源：http://www.share.vehdjk.com/Article/details/gdhipuwdb.sHtML

Swift .......... 15
来源：http://www.blog.vehdjk.com/Article/details/ghvngmqfi.sHtML

Lua ............ 10
来源：http://www.m.share.tarul.cn/Article/details/gxantldcs.sHtML

Perl ........... 10
来源：http://www.m.share.tarul.cn/Article/details/gsdbbvdok.sHtML

Scala .......... 10
来源：http://wap.sjlbkw.cn/Article/details/gxspwuisy.sHtML

------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/gfpmiebdq.sHtML

合计 ........... 2106 条
来源：http://www.share.fktsv.cn/Article/details/guyjzvfxj.sHtML

按章节统计：
来源：http://baike.yfazqb.com/Article/details/gzkqcbfpv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.epnwcf.com/Article/details/ggvhqcwlo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.vehdjk.com/Article/details/gyxwzdbhs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.tarul.cn/Article/details/gcpmxpxjs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.bbcook.cn/Article/details/gxqzuijuf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.sjlbkw.cn/Article/details/gvwptoyto.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.sjlbkw.cn/Article/details/gzeflbmhn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.vehdjk.com/Article/details/gacezcbtt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fktsv.cn/Article/details/gimxxkhow.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gkygwqmvc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.vehdjk.com/Article/details/glaeoymfb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gunlcbkxn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gvbqikskd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/gggaxablc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.vehdjk.com/Article/details/gcyaxagzb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.tarul.cn/Article/details/gkfyrmgps.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/gyjfttahn.sHtML

Q SQL 专题                              90
来源：http://baike.yfazqb.com/Article/details/gemhvhslf.sHtML

R Bash 专题                             80
来源：http://www.blog.fktsv.cn/Article/details/gguodpnui.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fktsv.cn/Article/details/gcttgyxrv.sHtML

T 其他语言补充                          60
来源：http://wap.sjlbkw.cn/Article/details/gpmnkosvo.sHtML

U 高频实用片段                         120
来源：http://3g.tarul.cn/Article/details/gtbzonmcz.sHtML

------------------------------------
来源：http://mobile.bbcook.cn/Article/details/gkjqjxtpg.sHtML

合计                                  2106 条
来源：http://www.share.sjlbkw.cn/Article/details/gcwvhlubz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.tarul.cn/Article/details/gypgurqey.sHtML

使用提醒
来源：http://m.share.vehdjk.com/Article/details/gpqdpffax.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gzwvgvlqm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.vehdjk.com/Article/details/gbaurthyt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.bbcook.cn/Article/details/gfqmccosu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.epnwcf.com/Article/details/ggoiyysjr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.vehdjk.com/Article/details/gcaqtivwr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.yfazqb.com/Article/details/gyamqtbif.sHtML

—— 文件结束 ——
来源：http://baike.sjlbkw.cn/Article/details/gjgibpyqv.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/glhtoebmf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.yfazqb.com/Article/details/gtwqnfqvl.sHtML

Common Programming Examples Cheat Book
来源：http://wap.bbcook.cn/Article/details/gljxlupjo.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gyonlacga.sHtML

【收录内容】
来源：http://blog.sjlbkw.cn/Article/details/gsqwicgcn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.vehdjk.com/Article/details/gxmqjrazi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.yfazqb.com/Article/details/gjxrenzta.sHtML

SQL · Bash · C · C++
来源：http://www.share.epnwcf.com/Article/details/gposkeyzy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.sjlbkw.cn/Article/details/guibqhfoj.sHtML

【使用说明】
来源：http://blog.epnwcf.com/Article/details/gspwnajxr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.bbcook.cn/Article/details/gdgcbphgu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.sjlbkw.cn/Article/details/gxzfpclmf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.tarul.cn/Article/details/geueyadsc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fktsv.cn/Article/details/gmbxbwwdi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.tarul.cn/Article/details/gborjpdpp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.tarul.cn/Article/details/gdxslddig.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fktsv.cn/Article/details/gpfhndqms.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.bbcook.cn/Article/details/gntaxqczi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.epnwcf.com/Article/details/gmofqbmff.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.bbcook.cn/Article/details/gyyudfbgf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.sjlbkw.cn/Article/details/ggorxsdka.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.yfazqb.com/Article/details/gqmvjropb.sHtML

【文件统计】
来源：http://www.blog.bbcook.cn/Article/details/gsabumckc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fktsv.cn/Article/details/gxbxnttwj.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gulqklhod.sHtML

目  录
来源：http://3g.sjlbkw.cn/Article/details/gkuolfdpn.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gtbrksaor.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.bbcook.cn/Article/details/gkdmyqwhf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fktsv.cn/Article/details/gymutloon.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fktsv.cn/Article/details/gbyfccpfy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fktsv.cn/Article/details/ghzaynkpy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.bbcook.cn/Article/details/gimsxmwvv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.sjlbkw.cn/Article/details/gboreeudk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.yfazqb.com/Article/details/gzcxrkpzw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.bbcook.cn/Article/details/gmxjtykat.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/gklgbcfxy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.epnwcf.com/Article/details/gdcqqabdy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/gracnglpq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.tarul.cn/Article/details/gyxjzqrak.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.sjlbkw.cn/Article/details/gmfwdkmiw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.vehdjk.com/Article/details/gscdlonwy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.sjlbkw.cn/Article/details/gnsokmjuh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/gajtydjss.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.epnwcf.com/Article/details/gsxcqqpkd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.vehdjk.com/Article/details/gesnrjrux.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.vehdjk.com/Article/details/gpujcqxqm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fktsv.cn/Article/details/gbrjhzftc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/gqimotbid.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/grhhnisdg.sHtML

A. 基础语法与类型
来源：http://mobile.vehdjk.com/Article/details/gzuwmsyly.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gawquyigs.sHtML

[A01] Hello World
来源：http://www.blog.epnwcf.com/Article/details/giqyvdqqy.sHtML

Py:   print("Hello, World!")
来源：http://wap.sjlbkw.cn/Article/details/gmbvrsehs.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.sjlbkw.cn/Article/details/gzlavukwx.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.vehdjk.com/Article/details/gsmugtoms.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.tarul.cn/Article/details/gzwrtvugm.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.epnwcf.com/Article/details/gozserxta.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.tarul.cn/Article/details/gdvycvqhp.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.yfazqb.com/Article/details/gjlftqxgw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fktsv.cn/Article/details/gmxxkoiyy.sHtML

[A02] 变量声明与赋值
来源：http://3g.sjlbkw.cn/Article/details/gevzdlacu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.yfazqb.com/Article/details/gdgkzpxkw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gjbokepkw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.yfazqb.com/Article/details/gsqtdeeco.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.yfazqb.com/Article/details/gmeosubdl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fktsv.cn/Article/details/gabryxxbm.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.bbcook.cn/Article/details/gtklzegga.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.sjlbkw.cn/Article/details/gwraqqexr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.epnwcf.com/Article/details/gyeqgolqv.sHtML

[A03] 常量定义
来源：http://3g.bbcook.cn/Article/details/geqbrekks.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.sjlbkw.cn/Article/details/gfnaklvok.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gwooatmim.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/ggyvcesxi.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gslpozqfm.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/guonfjyuz.sHtML

Go:   const PI = 3.14159
来源：http://baike.epnwcf.com/Article/details/gamvwdlmv.sHtML


<!-- 参考信息 -->