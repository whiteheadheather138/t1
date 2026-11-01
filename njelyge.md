代发 wailian999

[U29] Py：属性校验
来源：http://3g.fktsv.cn/Article/details/gqovwxvje.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.epnwcf.com/Article/details/gpsyslmyi.sHtML

[U30] Py：数据类
来源：http://wap.sjlbkw.cn/Article/details/ghscomrvn.sHtML

@dataclass(slots=True)
来源：http://wap.tarul.cn/Article/details/gljhxkdbn.sHtML

[U31] Py：单测
来源：http://www.share.tarul.cn/Article/details/gprpydweq.sHtML

python -m pytest -q
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgtavoct.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.tarul.cn/Article/details/ghthdhrth.sHtML

ruff format . && ruff check --fix .
来源：http://wap.yfazqb.com/Article/details/gjawpssxz.sHtML

[U33] Py：打包发布
来源：http://blog.fktsv.cn/Article/details/gyepifars.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.vehdjk.com/Article/details/gyhhfuuok.sHtML

[U34] Py：判断编码
来源：http://www.share.tarul.cn/Article/details/gpxmbgjiz.sHtML

chardet.detect(raw)
来源：http://baike.vehdjk.com/Article/details/gyjqfmpjt.sHtML

[U35] Py：发送邮件
来源：http://3g.bbcook.cn/Article/details/gjwulztng.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fktsv.cn/Article/details/gwuaeambf.sHtML

[U36] Py：定时任务
来源：http://www.blog.epnwcf.com/Article/details/gvgnsghqw.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.vehdjk.com/Article/details/gxpzpcfda.sHtML

[U37] Py：读写 Excel
来源：http://mobile.bbcook.cn/Article/details/gfabkudoo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.epnwcf.com/Article/details/gkttummmi.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.epnwcf.com/Article/details/gaaqspcaj.sHtML

Path(__file__).resolve().parent
来源：http://wap.fktsv.cn/Article/details/ggvfimoyq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.tarul.cn/Article/details/guebejkdi.sHtML

sys.stdout.isatty()
来源：http://baike.sjlbkw.cn/Article/details/gctjsuwlo.sHtML

[U40] Py：打印到标准错误
来源：http://wap.tarul.cn/Article/details/ghautxzpk.sHtML

print("err", file=sys.stderr)
来源：http://www.share.tarul.cn/Article/details/gekqjvnem.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fktsv.cn/Article/details/gwspkeyso.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.tarul.cn/Article/details/gthylrdga.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.bbcook.cn/Article/details/gcsgcgqeb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.bbcook.cn/Article/details/gbmvcejju.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.bbcook.cn/Article/details/gsrzcqtjl.sHtML

namespace App\Http;
来源：http://mobile.tarul.cn/Article/details/gakzfxsst.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fktsv.cn/Article/details/gtedmxweg.sHtML

declare(strict_types=1);
来源：http://read.share.epnwcf.com/Article/details/gdytrruxv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.vehdjk.com/Article/details/giehoxpdz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/gbvskncii.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.tarul.cn/Article/details/gubqpsmpn.sHtML

?string $name = null
来源：http://m.share.fktsv.cn/Article/details/ghtbbgrcx.sHtML

[U47] PHP：联合类型
来源：http://3g.sjlbkw.cn/Article/details/gybqxdzvd.sHtML

int|string $id
来源：http://3g.epnwcf.com/Article/details/gsbifyldk.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gzzdbijjt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.sjlbkw.cn/Article/details/gtfcuxfzf.sHtML

[U49] PHP：只读属性
来源：http://wap.fktsv.cn/Article/details/gikenijfe.sHtML

public readonly string $name
来源：http://blog.yfazqb.com/Article/details/gxqqukcfx.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.epnwcf.com/Article/details/gduempohe.sHtML

public function __construct(private int $id) {}
来源：http://www.share.bbcook.cn/Article/details/gyohnfoqo.sHtML

[U51] PHP：数组解构
来源：http://m.share.yfazqb.com/Article/details/gnkahbtyc.sHtML

[$a, $b] = $arr;
来源：http://blog.epnwcf.com/Article/details/gnqszoeek.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.epnwcf.com/Article/details/gwhisjnaf.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.epnwcf.com/Article/details/golcptvar.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.bbcook.cn/Article/details/gzotmuaye.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.yfazqb.com/Article/details/gvffgzwzt.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.epnwcf.com/Article/details/ggzveeson.sHtML

$obj?->method()
来源：http://m.share.yfazqb.com/Article/details/gfsqrhkay.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gbefyadpi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.sjlbkw.cn/Article/details/ggsukwumw.sHtML

[U56] PHP：命名参数
来源：http://mobile.bbcook.cn/Article/details/ghpkixixj.sHtML

f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/gprrviolv.sHtML

[U57] PHP：字符串插值
来源：http://www.share.epnwcf.com/Article/details/goygbedat.sHtML

"值: {$a}"
来源：http://wap.yfazqb.com/Article/details/giqjbgoed.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.bbcook.cn/Article/details/gywvaurou.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.tarul.cn/Article/details/ggbifirej.sHtML

[U59] PHP：自定义排序
来源：http://wap.tarul.cn/Article/details/goadtmizr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.sjlbkw.cn/Article/details/gmhzijzur.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.bbcook.cn/Article/details/ghgocnaks.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.epnwcf.com/Article/details/gxpkmajya.sHtML

[U61] PHP：正则
来源：http://mobile.tarul.cn/Article/details/gzvuxkxtk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fktsv.cn/Article/details/gildttcde.sHtML

[U62] PHP：日期对象
来源：http://wap.yfazqb.com/Article/details/gmwxcoiol.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.sjlbkw.cn/Article/details/gljowrxaa.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.yfazqb.com/Article/details/ggidzbxbn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.yfazqb.com/Article/details/ggyknlnlt.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.yfazqb.com/Article/details/gnzehkeci.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.sjlbkw.cn/Article/details/gmogggecb.sHtML

[U65] PHP：会话
来源：http://www.share.tarul.cn/Article/details/gbtoxbbyn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.yfazqb.com/Article/details/gedawzrxt.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.vehdjk.com/Article/details/gfzhxqvsx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.bbcook.cn/Article/details/gwtwkjbzo.sHtML

[U67] PHP：处理文件上传
来源：http://baike.vehdjk.com/Article/details/gqhtrzhjg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.epnwcf.com/Article/details/gvhwnyadp.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fktsv.cn/Article/details/gdwygzbbl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvqsgaol.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.vehdjk.com/Article/details/guujemefc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.yfazqb.com/Article/details/gknlmsemf.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.tarul.cn/Article/details/gdcwovhwe.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.yfazqb.com/Article/details/gjrdludme.sHtML

[U71] PHP：抛出异常
来源：http://wap.tarul.cn/Article/details/gqymmrxwf.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.yfazqb.com/Article/details/gfgpddafg.sHtML

[U72] PHP：写错误日志
来源：http://wap.epnwcf.com/Article/details/gipwrerlc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.yfazqb.com/Article/details/glgfxnrcb.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.sjlbkw.cn/Article/details/gtvpqtedv.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fktsv.cn/Article/details/gjcootpxh.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.bbcook.cn/Article/details/gliqwswpf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.bbcook.cn/Article/details/gwusoycob.sHtML

[U75] PHP：依赖注入
来源：http://baike.sjlbkw.cn/Article/details/gdftgxvdh.sHtML

composer require psr/container
来源：http://m.share.sjlbkw.cn/Article/details/gaoldchno.sHtML

[U76] PHP：简单路由
来源：http://www.share.bbcook.cn/Article/details/gvcqwadwm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.epnwcf.com/Article/details/grfgizgjw.sHtML

[U77] PHP：模板渲染
来源：http://baike.epnwcf.com/Article/details/glumumhjx.sHtML

composer require twig/twig
来源：http://wap.bbcook.cn/Article/details/ghgxdffyd.sHtML

[U78] PHP：单元测试
来源：http://www.share.fktsv.cn/Article/details/ggbifpkbt.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fktsv.cn/Article/details/grsffhbcs.sHtML

[U79] PHP：静态分析
来源：http://mobile.fktsv.cn/Article/details/gfpeqrqdl.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.tarul.cn/Article/details/gmcayztsv.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fktsv.cn/Article/details/gulbfqfrf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.sjlbkw.cn/Article/details/gbdkobrro.sHtML

[U81] JS：初始化项目
来源：http://mobile.bbcook.cn/Article/details/gnbwrbxme.sHtML

npm init -y;  npm i express
来源：http://wap.yfazqb.com/Article/details/gungeelwt.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.bbcook.cn/Article/details/gsidsokzu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fktsv.cn/Article/details/glbfmpzjz.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.tarul.cn/Article/details/gtjtjnklm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.yfazqb.com/Article/details/grkistbqn.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.tarul.cn/Article/details/gyqspjvll.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fktsv.cn/Article/details/gfjfgfirl.sHtML

[U85] JS：可选链
来源：http://3g.vehdjk.com/Article/details/gnjkrgwmj.sHtML

a?.b?.c
来源：http://3g.sjlbkw.cn/Article/details/gdlvnecrp.sHtML

[U86] JS：空值合并
来源：http://m.share.bbcook.cn/Article/details/gnkzbjeyn.sHtML

a ?? b
来源：http://www.blog.yfazqb.com/Article/details/gtuozwbec.sHtML

[U87] JS：解构默认值
来源：http://m.share.vehdjk.com/Article/details/gcvollmwp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.bbcook.cn/Article/details/gpptsddbo.sHtML

[U88] JS：对象展开合并
来源：http://3g.fktsv.cn/Article/details/gkqxtuvqn.sHtML

{ ...a, ...b }
来源：http://baike.tarul.cn/Article/details/godguxiod.sHtML

[U89] JS：数组去重
来源：http://www.blog.epnwcf.com/Article/details/gxysnolho.sHtML

[...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/gjhsthskz.sHtML

[U90] JS：数字数组排序
来源：http://www.share.yfazqb.com/Article/details/gzylrgspv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/gttwwiirn.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.vehdjk.com/Article/details/gpmryzukz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.yfazqb.com/Article/details/gbywwnymj.sHtML

[U92] JS：深拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gqsxdnncr.sHtML

structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gtqotpphg.sHtML

[U93] JS：模板字符串
来源：http://m.share.tarul.cn/Article/details/gfvoqlfsg.sHtML

`共 ${n} 条`
来源：http://m.share.vehdjk.com/Article/details/gexqnmdae.sHtML

[U94] JS：箭头函数
来源：http://wap.yfazqb.com/Article/details/gqmdbvcdl.sHtML

const double = x => x * 2;
来源：http://www.m.share.bbcook.cn/Article/details/gfwdlplzb.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fktsv.cn/Article/details/gdgapieex.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.tarul.cn/Article/details/gscauvmke.sHtML

[U96] JS：async/await 与异常
来源：http://baike.tarul.cn/Article/details/gwwucszdz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.yfazqb.com/Article/details/guwjmmqgs.sHtML

[U97] JS：并发请求
来源：http://m.share.fktsv.cn/Article/details/guzusuxiq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gcdkqbktm.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.sjlbkw.cn/Article/details/gozkqwtnl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.bbcook.cn/Article/details/ggdjbueyj.sHtML

[U99] JS：事件监听
来源：http://3g.fktsv.cn/Article/details/gxzbkuooj.sHtML

el.addEventListener("click", e => {})
来源：http://baike.epnwcf.com/Article/details/grzpsxtyq.sHtML

[U100] JS：DOM 查询
来源：http://baike.tarul.cn/Article/details/gepxzfoiy.sHtML

document.querySelector(".item")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdsxcmxt.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvyhcqxn.sHtML

el.classList.toggle("active")
来源：http://blog.vehdjk.com/Article/details/gtwmfoqkr.sHtML

[U102] JS：本地存储
来源：http://baike.epnwcf.com/Article/details/gzncvxyvv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fktsv.cn/Article/details/gdktjjavc.sHtML

[U103] JS：定时器
来源：http://m.share.tarul.cn/Article/details/gfjkyanvk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.tarul.cn/Article/details/gmjbwuscl.sHtML

[U104] JS：防抖
来源：http://blog.sjlbkw.cn/Article/details/gzjcxyjnt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/girqhuulp.sHtML

[U105] JS：节流
来源：http://baike.tarul.cn/Article/details/gwnykgeya.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.sjlbkw.cn/Article/details/gtpjcavwn.sHtML

[U106] JS：日期格式化
来源：http://baike.tarul.cn/Article/details/ghsgrfpou.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.epnwcf.com/Article/details/gdlrvileh.sHtML

[U107] JS：数字千分位
来源：http://www.share.fktsv.cn/Article/details/gpuwwllny.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.bbcook.cn/Article/details/gobnaerid.sHtML

[U108] JS：随机整数
来源：http://www.share.epnwcf.com/Article/details/ggqvotnqg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.yfazqb.com/Article/details/gsxdbkzbg.sHtML

[U109] JS：数组分组
来源：http://wap.vehdjk.com/Article/details/gmwozytio.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.sjlbkw.cn/Article/details/goyttgkns.sHtML

[U110] JS：数组分块
来源：http://wap.tarul.cn/Article/details/gbxgmlxwz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.vehdjk.com/Article/details/gcnaictva.sHtML

[U111] JS：对象转 Map
来源：http://m.share.sjlbkw.cn/Article/details/gndwmnvwq.sHtML

new Map(Object.entries(obj))
来源：http://read.share.bbcook.cn/Article/details/gpfwiowgs.sHtML

[U112] JS：字符串补位
来源：http://blog.sjlbkw.cn/Article/details/gmqzviiez.sHtML

"7".padStart(3, "0")
来源：http://m.share.vehdjk.com/Article/details/gqcjxmwod.sHtML

[U113] JS：正则替换全部
来源：http://baike.yfazqb.com/Article/details/ggdgkhhvj.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gneugmlfp.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fktsv.cn/Article/details/gjkrcdarv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.sjlbkw.cn/Article/details/ggcabmxjt.sHtML

[U115] JS：生成 UUID
来源：http://blog.tarul.cn/Article/details/guovkkmew.sHtML

crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gymdoaeak.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.vehdjk.com/Article/details/geneuhicw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.vehdjk.com/Article/details/gmctrgvuy.sHtML

[U117] JS：单元测试
来源：http://www.share.yfazqb.com/Article/details/giwpuifdo.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fktsv.cn/Article/details/gwqxryxkz.sHtML

[U118] JS：开发服务器
来源：http://blog.fktsv.cn/Article/details/gzelkfixx.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.bbcook.cn/Article/details/gpnswamkn.sHtML

[U119] JS：生产构建
来源：http://mobile.fktsv.cn/Article/details/gfvgzaihv.sHtML

npx vite build
来源：http://www.m.share.tarul.cn/Article/details/ghqhzpawb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.vehdjk.com/Article/details/gtqyzgjnz.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.vehdjk.com/Article/details/gvsuzatki.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/grrljnlin.sHtML

统计汇总
来源：http://baike.bbcook.cn/Article/details/gomciukpu.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ghmevjwvh.sHtML

按语言统计（条）：
来源：http://read.share.epnwcf.com/Article/details/gxbmzteca.sHtML

Python ......... 252
来源：http://mobile.tarul.cn/Article/details/grbqxeqlx.sHtML

PHP ............ 252
来源：http://mobile.fktsv.cn/Article/details/gvzdfjzse.sHtML

JavaScript ..... 252
来源：http://mobile.bbcook.cn/Article/details/geuyanoxb.sHtML

TypeScript ..... 212
来源：http://baike.fktsv.cn/Article/details/gjmsjyxoj.sHtML

Java ........... 212
来源：http://baike.vehdjk.com/Article/details/guhyhdavt.sHtML

Go ............. 212
来源：http://mobile.fktsv.cn/Article/details/gryloprna.sHtML

Ruby ........... 212
来源：http://wap.vehdjk.com/Article/details/gziomsusf.sHtML

C# ............. 212
来源：http://m.share.epnwcf.com/Article/details/gwspwabnu.sHtML

C .............. 30
来源：http://baike.fktsv.cn/Article/details/gnkizzpep.sHtML

C++ ............ 30
来源：http://www.m.share.fktsv.cn/Article/details/gjvwmljyf.sHtML

SQL ............ 90
来源：http://wap.sjlbkw.cn/Article/details/gbqngbllo.sHtML

Bash ........... 80
来源：http://baike.vehdjk.com/Article/details/gjeqnrwym.sHtML

Kotlin ......... 15
来源：http://baike.yfazqb.com/Article/details/grlmezjeu.sHtML

Swift .......... 15
来源：http://m.share.bbcook.cn/Article/details/gcucsgozw.sHtML

Lua ............ 10
来源：http://wap.vehdjk.com/Article/details/gtwbkdbsx.sHtML

Perl ........... 10
来源：http://www.m.share.bbcook.cn/Article/details/gqsozhplb.sHtML

Scala .......... 10
来源：http://blog.sjlbkw.cn/Article/details/gjwfmsuym.sHtML

------------------------------------
来源：http://mobile.tarul.cn/Article/details/gctndqxlg.sHtML

合计 ........... 2106 条
来源：http://m.share.sjlbkw.cn/Article/details/gjiigiewi.sHtML

按章节统计：
来源：http://3g.tarul.cn/Article/details/gpvsgtxhx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.tarul.cn/Article/details/gbhieayca.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.tarul.cn/Article/details/gpzcryayh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.bbcook.cn/Article/details/goxxwiboa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.vehdjk.com/Article/details/gzqukamlq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.tarul.cn/Article/details/gdynadqcu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fktsv.cn/Article/details/gxkkilbjp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.epnwcf.com/Article/details/gffzxzxgv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.sjlbkw.cn/Article/details/grccsgqzr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/gnsyrrhtm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fktsv.cn/Article/details/gnpphrjij.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/gjykoyisa.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/gesgcbvak.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/gphcwoxwa.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.vehdjk.com/Article/details/gjsduxzml.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fktsv.cn/Article/details/gpvbadrue.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/ggjgpsfgi.sHtML

Q SQL 专题                              90
来源：http://baike.sjlbkw.cn/Article/details/glpgvfksw.sHtML

R Bash 专题                             80
来源：http://blog.tarul.cn/Article/details/gbdyovswo.sHtML

S C / C++ 专题                          60
来源：http://www.blog.epnwcf.com/Article/details/ggqcgdzlx.sHtML

T 其他语言补充                          60
来源：http://www.share.sjlbkw.cn/Article/details/gjiyvquyo.sHtML

U 高频实用片段                         120
来源：http://blog.epnwcf.com/Article/details/gjsppwsjj.sHtML

------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gsgmselpx.sHtML

合计                                  2106 条
来源：http://baike.yfazqb.com/Article/details/gpkahdeuv.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/grphimyfu.sHtML

使用提醒
来源：http://m.share.tarul.cn/Article/details/gzwpmkavy.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/grxyztsim.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fktsv.cn/Article/details/grzvppayg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.sjlbkw.cn/Article/details/gmzipcmii.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.tarul.cn/Article/details/gpmbkbmze.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.yfazqb.com/Article/details/gzitbbekj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.yfazqb.com/Article/details/gsxzekxzb.sHtML

—— 文件结束 ——
来源：http://m.share.vehdjk.com/Article/details/gqvjamamq.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gjilvwnia.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.vehdjk.com/Article/details/gwdrqlhmg.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.bbcook.cn/Article/details/gjvrswqqz.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gutvktzkz.sHtML

【收录内容】
来源：http://baike.bbcook.cn/Article/details/gtfwofuak.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.tarul.cn/Article/details/gvdtxxigd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.tarul.cn/Article/details/gwaseveoj.sHtML

SQL · Bash · C · C++
来源：http://www.share.yfazqb.com/Article/details/ghhddkfis.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fktsv.cn/Article/details/gieopmbss.sHtML

【使用说明】
来源：http://blog.bbcook.cn/Article/details/gvpzmodeb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrreuhmm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.bbcook.cn/Article/details/gnkfvrbop.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fktsv.cn/Article/details/gwtixtwiz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.yfazqb.com/Article/details/gosembucm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.bbcook.cn/Article/details/gjsmdqsdh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.bbcook.cn/Article/details/ghgnozevb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.yfazqb.com/Article/details/gjnrsyunm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.bbcook.cn/Article/details/gbuicmwxh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.vehdjk.com/Article/details/gxfgpxvja.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.sjlbkw.cn/Article/details/gvoucrtue.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.epnwcf.com/Article/details/gmuzkotvp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.vehdjk.com/Article/details/gcthikjps.sHtML

【文件统计】
来源：http://read.share.bbcook.cn/Article/details/gmhlfksnm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.yfazqb.com/Article/details/glpfowyyf.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/gtbnkbtlq.sHtML

目  录
来源：http://read.share.sjlbkw.cn/Article/details/gkynmtbxi.sHtML

--------------------------------------------------------------------------------
来源：http://blog.yfazqb.com/Article/details/giavgjmxz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.vehdjk.com/Article/details/gnsjurbwi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.tarul.cn/Article/details/gpznwflpu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.sjlbkw.cn/Article/details/grngzwffc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.epnwcf.com/Article/details/gohtkrnux.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.yfazqb.com/Article/details/gkdsprozn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.vehdjk.com/Article/details/glksdxvst.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.vehdjk.com/Article/details/guxmzfuze.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.yfazqb.com/Article/details/gxttssyfv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/gtisdaofs.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.yfazqb.com/Article/details/gsqnbypom.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gndautwul.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.vehdjk.com/Article/details/gymuyzkoo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.bbcook.cn/Article/details/gvcvvmntd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.epnwcf.com/Article/details/gkbwsjicx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.tarul.cn/Article/details/giyeyvqqp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.sjlbkw.cn/Article/details/gljfpfqdv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.yfazqb.com/Article/details/gppghqyur.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.sjlbkw.cn/Article/details/gzmpbehgg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.yfazqb.com/Article/details/gouynhljb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.tarul.cn/Article/details/ghqyrtacu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxnoujrq.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gflomlkbh.sHtML

A. 基础语法与类型
来源：http://3g.epnwcf.com/Article/details/gwlkizsuh.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ggvxzmmsi.sHtML

[A01] Hello World
来源：http://baike.bbcook.cn/Article/details/ghhpwxysj.sHtML

Py:   print("Hello, World!")
来源：http://mobile.yfazqb.com/Article/details/gmhlqqerr.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.yfazqb.com/Article/details/gljdlqgyu.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.tarul.cn/Article/details/gdmdoynaw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fktsv.cn/Article/details/gihjtataz.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.sjlbkw.cn/Article/details/gtoorcpoo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fktsv.cn/Article/details/gjvwfpoad.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.tarul.cn/Article/details/grcrrvtwk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.sjlbkw.cn/Article/details/gorkmoxfy.sHtML


<!-- 参考信息 -->