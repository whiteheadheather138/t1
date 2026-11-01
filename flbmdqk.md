代发 wailian999

[U29] Py：属性校验
来源：http://blog.sjlbkw.cn/Article/details/giutwlvsx.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fktsv.cn/Article/details/gcdkzdjia.sHtML

[U30] Py：数据类
来源：http://www.blog.sjlbkw.cn/Article/details/glsgrvbov.sHtML

@dataclass(slots=True)
来源：http://mobile.epnwcf.com/Article/details/gwixjjqhj.sHtML

[U31] Py：单测
来源：http://baike.yfazqb.com/Article/details/gowfhfjhh.sHtML

python -m pytest -q
来源：http://read.share.sjlbkw.cn/Article/details/gdoorqlzd.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.tarul.cn/Article/details/gokbiwioj.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.sjlbkw.cn/Article/details/gtfottnjo.sHtML

[U33] Py：打包发布
来源：http://read.share.epnwcf.com/Article/details/gfiinqxdf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.vehdjk.com/Article/details/gzyhtjdvz.sHtML

[U34] Py：判断编码
来源：http://blog.tarul.cn/Article/details/gsyezpfyu.sHtML

chardet.detect(raw)
来源：http://wap.epnwcf.com/Article/details/ghsaehaqq.sHtML

[U35] Py：发送邮件
来源：http://www.blog.epnwcf.com/Article/details/gmzhfiyll.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.epnwcf.com/Article/details/gyvaazade.sHtML

[U36] Py：定时任务
来源：http://m.share.bbcook.cn/Article/details/gftltiazu.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.tarul.cn/Article/details/gvhyjpobm.sHtML

[U37] Py：读写 Excel
来源：http://read.share.epnwcf.com/Article/details/gciquukil.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.tarul.cn/Article/details/gwhnfagmi.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.vehdjk.com/Article/details/gdcvzdinj.sHtML

Path(__file__).resolve().parent
来源：http://wap.yfazqb.com/Article/details/gxgfgjsax.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fktsv.cn/Article/details/gqkqqcspf.sHtML

sys.stdout.isatty()
来源：http://blog.vehdjk.com/Article/details/ghrlnyhqg.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.tarul.cn/Article/details/gcdsoyusl.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.yfazqb.com/Article/details/ghikqisjs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.epnwcf.com/Article/details/glnrpefec.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.tarul.cn/Article/details/gciocbzwm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.bbcook.cn/Article/details/gnronjpta.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.epnwcf.com/Article/details/gvmpdgdap.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fktsv.cn/Article/details/grptshidt.sHtML

namespace App\Http;
来源：http://wap.vehdjk.com/Article/details/gexheygfj.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.bbcook.cn/Article/details/gitnhjfpe.sHtML

declare(strict_types=1);
来源：http://wap.fktsv.cn/Article/details/gxtobekrj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.yfazqb.com/Article/details/goeactxjf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/giqklwmee.sHtML

[U46] PHP：可空类型
来源：http://blog.yfazqb.com/Article/details/gkepsvnst.sHtML

?string $name = null
来源：http://mobile.epnwcf.com/Article/details/gwvobhcts.sHtML

[U47] PHP：联合类型
来源：http://www.share.yfazqb.com/Article/details/gjpjbyxje.sHtML

int|string $id
来源：http://blog.epnwcf.com/Article/details/gnotvxhri.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmyatefj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fktsv.cn/Article/details/gsfxeabgg.sHtML

[U49] PHP：只读属性
来源：http://m.share.vehdjk.com/Article/details/gpryuqrem.sHtML

public readonly string $name
来源：http://mobile.fktsv.cn/Article/details/grmrxpdho.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.yfazqb.com/Article/details/grmssiyyj.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.yfazqb.com/Article/details/gcktfvfnw.sHtML

[U51] PHP：数组解构
来源：http://baike.fktsv.cn/Article/details/gmvngmbvr.sHtML

[$a, $b] = $arr;
来源：http://www.blog.tarul.cn/Article/details/gaijirwyi.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fktsv.cn/Article/details/gtrnwfovs.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.sjlbkw.cn/Article/details/gfpezoupw.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.vehdjk.com/Article/details/gawgukhkg.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fktsv.cn/Article/details/grxnczmrl.sHtML

[U54] PHP：空安全调用
来源：http://m.share.vehdjk.com/Article/details/gtbsoolxe.sHtML

$obj?->method()
来源：http://3g.bbcook.cn/Article/details/ggysjkwxr.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.epnwcf.com/Article/details/gvpmpcefh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fktsv.cn/Article/details/gedfiomuj.sHtML

[U56] PHP：命名参数
来源：http://m.share.sjlbkw.cn/Article/details/gsfuztsak.sHtML

f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/gpvzdaran.sHtML

[U57] PHP：字符串插值
来源：http://www.share.tarul.cn/Article/details/gqhjpsyfu.sHtML

"值: {$a}"
来源：http://wap.vehdjk.com/Article/details/geqkouhjx.sHtML

[U58] PHP：数组三件套
来源：http://wap.bbcook.cn/Article/details/gagnrkfnf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.vehdjk.com/Article/details/grckngruu.sHtML

[U59] PHP：自定义排序
来源：http://mobile.yfazqb.com/Article/details/gcjhzfrou.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.sjlbkw.cn/Article/details/gjpjzcuvt.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.tarul.cn/Article/details/gehjxisej.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fktsv.cn/Article/details/gpetfqeyc.sHtML

[U61] PHP：正则
来源：http://www.share.vehdjk.com/Article/details/gjkejmrei.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.yfazqb.com/Article/details/guqvojgyb.sHtML

[U62] PHP：日期对象
来源：http://m.share.yfazqb.com/Article/details/gfinlpsyu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.sjlbkw.cn/Article/details/guhehxdps.sHtML

[U63] PHP：文件读写
来源：http://mobile.fktsv.cn/Article/details/ggkwhwmgs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.yfazqb.com/Article/details/gtbzwijpc.sHtML

[U64] PHP：目录遍历
来源：http://mobile.sjlbkw.cn/Article/details/gjdtqoeho.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.tarul.cn/Article/details/gsbaqvdsy.sHtML

[U65] PHP：会话
来源：http://www.share.yfazqb.com/Article/details/gcqlofuxb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fktsv.cn/Article/details/glkvmtloh.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.vehdjk.com/Article/details/ghxlzzhkq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.vehdjk.com/Article/details/ghedtubdi.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.epnwcf.com/Article/details/gxapfypgr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.bbcook.cn/Article/details/gedgztfus.sHtML

[U68] PHP：PDO 连接
来源：http://3g.tarul.cn/Article/details/ghfqmxjed.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.vehdjk.com/Article/details/gnvvjwwwr.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.vehdjk.com/Article/details/gnewjqhdu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.epnwcf.com/Article/details/gzgoxnjwp.sHtML

[U70] PHP：PDO 事务
来源：http://baike.vehdjk.com/Article/details/gumrnzgxi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.epnwcf.com/Article/details/gquibqjaz.sHtML

[U71] PHP：抛出异常
来源：http://www.share.sjlbkw.cn/Article/details/gtmgafrjj.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.sjlbkw.cn/Article/details/geazvvyep.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.bbcook.cn/Article/details/grsgrgtvw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.vehdjk.com/Article/details/gcgyynyte.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjdbbntb.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.epnwcf.com/Article/details/giefstlex.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fktsv.cn/Article/details/gohxijkbg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.sjlbkw.cn/Article/details/gsptirbnx.sHtML

[U75] PHP：依赖注入
来源：http://3g.sjlbkw.cn/Article/details/gxwwgnlkd.sHtML

composer require psr/container
来源：http://read.share.vehdjk.com/Article/details/gzxqjrbrz.sHtML

[U76] PHP：简单路由
来源：http://baike.yfazqb.com/Article/details/gxiyjajeo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.vehdjk.com/Article/details/gcfoxrlyr.sHtML

[U77] PHP：模板渲染
来源：http://baike.bbcook.cn/Article/details/gmlaubbbc.sHtML

composer require twig/twig
来源：http://www.m.share.epnwcf.com/Article/details/gppgibwab.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.yfazqb.com/Article/details/gvtpsowof.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.sjlbkw.cn/Article/details/gsncijmuf.sHtML

[U79] PHP：静态分析
来源：http://www.blog.epnwcf.com/Article/details/gjykdfdce.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.bbcook.cn/Article/details/gfdhasefm.sHtML

[U80] PHP：代码规范修复
来源：http://3g.tarul.cn/Article/details/gbjbcodwo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.tarul.cn/Article/details/gneewwgtt.sHtML

[U81] JS：初始化项目
来源：http://www.blog.epnwcf.com/Article/details/gzhddafyu.sHtML

npm init -y;  npm i express
来源：http://www.share.epnwcf.com/Article/details/gsspsunjs.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.tarul.cn/Article/details/gkmshzqpu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.vehdjk.com/Article/details/guxkjgpli.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.epnwcf.com/Article/details/gvnlwzyxb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fktsv.cn/Article/details/gzsgythqd.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.sjlbkw.cn/Article/details/garpvnamr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.vehdjk.com/Article/details/grunieafu.sHtML

[U85] JS：可选链
来源：http://www.m.share.yfazqb.com/Article/details/ggluhkjdd.sHtML

a?.b?.c
来源：http://www.m.share.vehdjk.com/Article/details/gejkqcjfm.sHtML

[U86] JS：空值合并
来源：http://read.share.yfazqb.com/Article/details/gesrgiyax.sHtML

a ?? b
来源：http://wap.sjlbkw.cn/Article/details/gimckoerc.sHtML

[U87] JS：解构默认值
来源：http://m.share.epnwcf.com/Article/details/grsywgycz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.vehdjk.com/Article/details/guknbgarh.sHtML

[U88] JS：对象展开合并
来源：http://3g.fktsv.cn/Article/details/gyecknhrb.sHtML

{ ...a, ...b }
来源：http://3g.fktsv.cn/Article/details/gmlbrnljk.sHtML

[U89] JS：数组去重
来源：http://wap.bbcook.cn/Article/details/gfxegiryn.sHtML

[...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gmlfeltfe.sHtML

[U90] JS：数字数组排序
来源：http://wap.fktsv.cn/Article/details/gdanglmlj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/gijbovxjy.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fktsv.cn/Article/details/gqpmmwqps.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.bbcook.cn/Article/details/gzfajlkzy.sHtML

[U92] JS：深拷贝
来源：http://3g.tarul.cn/Article/details/gufmjhogw.sHtML

structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/gzoynbwgo.sHtML

[U93] JS：模板字符串
来源：http://www.share.fktsv.cn/Article/details/gyeanrven.sHtML

`共 ${n} 条`
来源：http://3g.vehdjk.com/Article/details/gjowxlyrg.sHtML

[U94] JS：箭头函数
来源：http://www.share.tarul.cn/Article/details/giiotlgoh.sHtML

const double = x => x * 2;
来源：http://baike.epnwcf.com/Article/details/gawatnuoo.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.tarul.cn/Article/details/gsjzdchqv.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.epnwcf.com/Article/details/gslbublkd.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.vehdjk.com/Article/details/gulvarscy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gtbjjwifz.sHtML

[U97] JS：并发请求
来源：http://mobile.bbcook.cn/Article/details/gyevhdpwc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/gmtonkofi.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.tarul.cn/Article/details/gltfxmlng.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.tarul.cn/Article/details/gcdjrwidx.sHtML

[U99] JS：事件监听
来源：http://baike.vehdjk.com/Article/details/gqqpegkek.sHtML

el.addEventListener("click", e => {})
来源：http://blog.vehdjk.com/Article/details/gjysextwy.sHtML

[U100] JS：DOM 查询
来源：http://read.share.tarul.cn/Article/details/gvzbjmirl.sHtML

document.querySelector(".item")
来源：http://blog.fktsv.cn/Article/details/ggwymbuup.sHtML

[U101] JS：classList 操作
来源：http://m.share.bbcook.cn/Article/details/gofargaku.sHtML

el.classList.toggle("active")
来源：http://wap.vehdjk.com/Article/details/glhfieqht.sHtML

[U102] JS：本地存储
来源：http://www.share.epnwcf.com/Article/details/gndxfjxbo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.tarul.cn/Article/details/gpwnfwdas.sHtML

[U103] JS：定时器
来源：http://wap.fktsv.cn/Article/details/gevtodaxr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.sjlbkw.cn/Article/details/gnucdncvj.sHtML

[U104] JS：防抖
来源：http://www.blog.vehdjk.com/Article/details/gqyleidbx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/gpcobmvuu.sHtML

[U105] JS：节流
来源：http://3g.tarul.cn/Article/details/gywmggrqg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.vehdjk.com/Article/details/gprgvoxbp.sHtML

[U106] JS：日期格式化
来源：http://blog.fktsv.cn/Article/details/glhhyqtiq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.epnwcf.com/Article/details/gkiigdyuq.sHtML

[U107] JS：数字千分位
来源：http://www.blog.bbcook.cn/Article/details/golvvitci.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.yfazqb.com/Article/details/gahmmnwpf.sHtML

[U108] JS：随机整数
来源：http://wap.bbcook.cn/Article/details/gbdxdpmft.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.tarul.cn/Article/details/geaykefut.sHtML

[U109] JS：数组分组
来源：http://read.share.tarul.cn/Article/details/gwwqdgjhf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.vehdjk.com/Article/details/gbpgbzaut.sHtML

[U110] JS：数组分块
来源：http://3g.vehdjk.com/Article/details/gsirdzzxg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.tarul.cn/Article/details/gkuzrikpr.sHtML

[U111] JS：对象转 Map
来源：http://wap.epnwcf.com/Article/details/gfxungvbw.sHtML

new Map(Object.entries(obj))
来源：http://baike.fktsv.cn/Article/details/giwwxcqfl.sHtML

[U112] JS：字符串补位
来源：http://mobile.epnwcf.com/Article/details/gfpcrpanl.sHtML

"7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gjgrqhfpk.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.yfazqb.com/Article/details/gauavccec.sHtML

s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/glrmppmus.sHtML

[U114] JS：JSON 深比较
来源：http://baike.epnwcf.com/Article/details/gcfgrpuwd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.tarul.cn/Article/details/gytrhhrxf.sHtML

[U115] JS：生成 UUID
来源：http://read.share.sjlbkw.cn/Article/details/glrvavvth.sHtML

crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/ggrnonswx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.vehdjk.com/Article/details/gfyronkya.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.yfazqb.com/Article/details/gnpybbnck.sHtML

[U117] JS：单元测试
来源：http://mobile.tarul.cn/Article/details/gqvgoighf.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.vehdjk.com/Article/details/goqpqqcuu.sHtML

[U118] JS：开发服务器
来源：http://3g.fktsv.cn/Article/details/gczedyryf.sHtML

npm i -D vite;  npx vite
来源：http://wap.yfazqb.com/Article/details/gqzpxntin.sHtML

[U119] JS：生产构建
来源：http://wap.sjlbkw.cn/Article/details/gpjbuhavc.sHtML

npx vite build
来源：http://blog.bbcook.cn/Article/details/gkakzivxh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.sjlbkw.cn/Article/details/gcyfpcbaq.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwctljdd.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbwsjdepr.sHtML

统计汇总
来源：http://m.share.fktsv.cn/Article/details/gesgvlivr.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gowevaoeq.sHtML

按语言统计（条）：
来源：http://m.share.sjlbkw.cn/Article/details/gqnocpmjd.sHtML

Python ......... 252
来源：http://blog.yfazqb.com/Article/details/gdjdmukpm.sHtML

PHP ............ 252
来源：http://mobile.sjlbkw.cn/Article/details/giqhihfuc.sHtML

JavaScript ..... 252
来源：http://baike.sjlbkw.cn/Article/details/gpnwoulxq.sHtML

TypeScript ..... 212
来源：http://wap.bbcook.cn/Article/details/gzxhjhzxp.sHtML

Java ........... 212
来源：http://www.blog.epnwcf.com/Article/details/ghduddtoa.sHtML

Go ............. 212
来源：http://m.share.fktsv.cn/Article/details/gnwialriq.sHtML

Ruby ........... 212
来源：http://wap.bbcook.cn/Article/details/ggiwriujn.sHtML

C# ............. 212
来源：http://www.share.sjlbkw.cn/Article/details/gglgvekox.sHtML

C .............. 30
来源：http://www.m.share.yfazqb.com/Article/details/gvmbqwmpw.sHtML

C++ ............ 30
来源：http://baike.bbcook.cn/Article/details/getrulwgk.sHtML

SQL ............ 90
来源：http://baike.sjlbkw.cn/Article/details/gomuntplo.sHtML

Bash ........... 80
来源：http://3g.fktsv.cn/Article/details/gfqmvihtu.sHtML

Kotlin ......... 15
来源：http://3g.vehdjk.com/Article/details/gzhcbbfdh.sHtML

Swift .......... 15
来源：http://www.blog.bbcook.cn/Article/details/gvbexqtdj.sHtML

Lua ............ 10
来源：http://baike.epnwcf.com/Article/details/gsplwaxrk.sHtML

Perl ........... 10
来源：http://3g.bbcook.cn/Article/details/gxvvbxxen.sHtML

Scala .......... 10
来源：http://mobile.epnwcf.com/Article/details/gbxvxdnvu.sHtML

------------------------------------
来源：http://mobile.tarul.cn/Article/details/gwsponnot.sHtML

合计 ........... 2106 条
来源：http://mobile.sjlbkw.cn/Article/details/gdpkvdjcg.sHtML

按章节统计：
来源：http://mobile.yfazqb.com/Article/details/gugebqurq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.vehdjk.com/Article/details/gzbjijucg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.yfazqb.com/Article/details/gmiikosfm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fktsv.cn/Article/details/ganrotmvd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.tarul.cn/Article/details/gtecnzvms.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.tarul.cn/Article/details/gmjqjbysr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.vehdjk.com/Article/details/gmylpvahw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.bbcook.cn/Article/details/gbxsecrgu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fktsv.cn/Article/details/ghxqgyyyl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/guffhcrgo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.vehdjk.com/Article/details/gmylqxffr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/gddrjpdxi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/golpklmxs.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gpccrrpij.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.tarul.cn/Article/details/gvrtlbiky.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.yfazqb.com/Article/details/gsgdwxljq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gzenylmve.sHtML

Q SQL 专题                              90
来源：http://blog.sjlbkw.cn/Article/details/grjyjezst.sHtML

R Bash 专题                             80
来源：http://www.share.bbcook.cn/Article/details/gjghpmhuc.sHtML

S C / C++ 专题                          60
来源：http://3g.sjlbkw.cn/Article/details/gajggzhzp.sHtML

T 其他语言补充                          60
来源：http://www.m.share.vehdjk.com/Article/details/goudbjhdx.sHtML

U 高频实用片段                         120
来源：http://blog.sjlbkw.cn/Article/details/gazrlntlx.sHtML

------------------------------------
来源：http://3g.epnwcf.com/Article/details/gvmimpytd.sHtML

合计                                  2106 条
来源：http://3g.yfazqb.com/Article/details/gudxgzngm.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gxkwzolzd.sHtML

使用提醒
来源：http://www.m.share.vehdjk.com/Article/details/gzwthaahp.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/giqjaaqch.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.sjlbkw.cn/Article/details/gqugdcvst.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.yfazqb.com/Article/details/grcizktpm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.vehdjk.com/Article/details/gtburkpnf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.epnwcf.com/Article/details/gzqgnmufd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fktsv.cn/Article/details/gxclzhkbd.sHtML

—— 文件结束 ——
来源：http://blog.fktsv.cn/Article/details/gxindcbjs.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gynacmstt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fktsv.cn/Article/details/gutugftgf.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.epnwcf.com/Article/details/gnuxjehdl.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gwljzjxed.sHtML

【收录内容】
来源：http://wap.yfazqb.com/Article/details/gwudsxgyt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.yfazqb.com/Article/details/gxdpntzjn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.bbcook.cn/Article/details/gsxxhzdka.sHtML

SQL · Bash · C · C++
来源：http://mobile.yfazqb.com/Article/details/gonyershs.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.yfazqb.com/Article/details/gtxjopgss.sHtML

【使用说明】
来源：http://wap.bbcook.cn/Article/details/glhzrtlyn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fktsv.cn/Article/details/ghrambpfy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.bbcook.cn/Article/details/ggyintxpw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.yfazqb.com/Article/details/gnhhfwgoq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.bbcook.cn/Article/details/gvxinjwrc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.epnwcf.com/Article/details/gxlmrjfsf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fktsv.cn/Article/details/gzihjjiwe.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.epnwcf.com/Article/details/gfjfguhvj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.epnwcf.com/Article/details/gerrgrear.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.bbcook.cn/Article/details/gtggtdljs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.epnwcf.com/Article/details/gstmemiou.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.bbcook.cn/Article/details/gjjxzrfcv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.epnwcf.com/Article/details/gvtmgrfzh.sHtML

【文件统计】
来源：http://m.share.vehdjk.com/Article/details/gjhqmbyef.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fktsv.cn/Article/details/gcjwjcgyt.sHtML

--------------------------------------------------------------------------------
来源：http://blog.bbcook.cn/Article/details/goxhxfugq.sHtML

目  录
来源：http://www.blog.fktsv.cn/Article/details/gjimmopfs.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fktsv.cn/Article/details/gkvitgkey.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.bbcook.cn/Article/details/gsvrgarqt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.vehdjk.com/Article/details/gtgoexzqf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/gzpahfskc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.tarul.cn/Article/details/grbzblrhp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fktsv.cn/Article/details/giowbtckn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.tarul.cn/Article/details/gzqgoipiq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.tarul.cn/Article/details/gbpnufcyq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fktsv.cn/Article/details/goewcsaqf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.tarul.cn/Article/details/gcwefebbd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.bbcook.cn/Article/details/giwycvflc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.vehdjk.com/Article/details/gtyfdywbw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.yfazqb.com/Article/details/gjbilpkcm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.sjlbkw.cn/Article/details/gdhaiobev.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.vehdjk.com/Article/details/gpxmtmdgp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fktsv.cn/Article/details/gheuhgfbh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gfapukmeb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fktsv.cn/Article/details/gclcisjsy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.tarul.cn/Article/details/gjfanubfc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.bbcook.cn/Article/details/ggrslqibk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.yfazqb.com/Article/details/gpjiycdyi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.epnwcf.com/Article/details/ggilzjctt.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gfctjcpge.sHtML

A. 基础语法与类型
来源：http://read.share.epnwcf.com/Article/details/ggyfobudj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gehedclvf.sHtML

[A01] Hello World
来源：http://www.blog.epnwcf.com/Article/details/ginpftaur.sHtML

Py:   print("Hello, World!")
来源：http://blog.vehdjk.com/Article/details/gxfqnxian.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.tarul.cn/Article/details/gfpdcecbl.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fktsv.cn/Article/details/gbxfpmtlx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.bbcook.cn/Article/details/geznmzdzq.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.epnwcf.com/Article/details/gkykimphi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.bbcook.cn/Article/details/ghbmrtqem.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.tarul.cn/Article/details/giourvmrb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fktsv.cn/Article/details/gujaljbzm.sHtML


<!-- 参考信息 -->