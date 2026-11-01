代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fktsv.cn/Article/details/gakekeofd.sHtML

@contextlib.contextmanager
来源：http://wap.sjlbkw.cn/Article/details/gckazayyg.sHtML

[U22] Py：矩阵转置
来源：http://3g.sjlbkw.cn/Article/details/gstuqvvoy.sHtML

list(zip(*m))
来源：http://3g.bbcook.cn/Article/details/gcmufztnt.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.tarul.cn/Article/details/gelepikdo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.epnwcf.com/Article/details/gzktvjomn.sHtML

[U24] Py：路径操作
来源：http://www.m.share.epnwcf.com/Article/details/gijhrimul.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fktsv.cn/Article/details/ggrjiabhp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.epnwcf.com/Article/details/gltklysfs.sHtML

csv.DictReader(f)
来源：http://m.share.bbcook.cn/Article/details/gtopyjgvs.sHtML

[U26] Py：并发下载
来源：http://www.share.yfazqb.com/Article/details/ghdpsszdl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fktsv.cn/Article/details/gzqmwsejh.sHtML

[U27] Py：异步 HTTP
来源：http://wap.yfazqb.com/Article/details/gaoddmxkq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.tarul.cn/Article/details/gyusseujs.sHtML

[U28] Py：类型别名
来源：http://mobile.yfazqb.com/Article/details/gtgoileli.sHtML

UserId = int
来源：http://mobile.sjlbkw.cn/Article/details/gywaelftm.sHtML

[U29] Py：属性校验
来源：http://m.share.yfazqb.com/Article/details/gzluvxnas.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.bbcook.cn/Article/details/gjhmtgmci.sHtML

[U30] Py：数据类
来源：http://www.share.yfazqb.com/Article/details/gflvrxbnd.sHtML

@dataclass(slots=True)
来源：http://blog.vehdjk.com/Article/details/gsmxibpal.sHtML

[U31] Py：单测
来源：http://blog.yfazqb.com/Article/details/gyktlvnqk.sHtML

python -m pytest -q
来源：http://m.share.bbcook.cn/Article/details/gpnpfegef.sHtML

[U32] Py：代码格式化
来源：http://blog.tarul.cn/Article/details/gddttnlmn.sHtML

ruff format . && ruff check --fix .
来源：http://blog.bbcook.cn/Article/details/gtrvdevfc.sHtML

[U33] Py：打包发布
来源：http://www.m.share.sjlbkw.cn/Article/details/gnchudhgh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.epnwcf.com/Article/details/gjbozaimv.sHtML

[U34] Py：判断编码
来源：http://3g.yfazqb.com/Article/details/gdqntoxwb.sHtML

chardet.detect(raw)
来源：http://m.share.yfazqb.com/Article/details/gmeidrndo.sHtML

[U35] Py：发送邮件
来源：http://www.blog.epnwcf.com/Article/details/ghimankxr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.vehdjk.com/Article/details/gjvvrsdeg.sHtML

[U36] Py：定时任务
来源：http://wap.fktsv.cn/Article/details/geewemmfc.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.sjlbkw.cn/Article/details/gnyqncxvu.sHtML

[U37] Py：读写 Excel
来源：http://m.share.bbcook.cn/Article/details/gylmyqjpv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.yfazqb.com/Article/details/gdgxoussu.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.tarul.cn/Article/details/gbawvcdgk.sHtML

Path(__file__).resolve().parent
来源：http://mobile.epnwcf.com/Article/details/gphoqtydg.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.bbcook.cn/Article/details/gisiwgruo.sHtML

sys.stdout.isatty()
来源：http://www.m.share.yfazqb.com/Article/details/gigbdwill.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.epnwcf.com/Article/details/gmyxzrats.sHtML

print("err", file=sys.stderr)
来源：http://wap.fktsv.cn/Article/details/gytiryoex.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.vehdjk.com/Article/details/gyxpsntdp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.sjlbkw.cn/Article/details/gxyigkahu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.bbcook.cn/Article/details/gczxfzwtq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.bbcook.cn/Article/details/gxkurrgun.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fktsv.cn/Article/details/ghcxmlmdj.sHtML

namespace App\Http;
来源：http://www.share.bbcook.cn/Article/details/gjrqpthrj.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fktsv.cn/Article/details/gggdahzco.sHtML

declare(strict_types=1);
来源：http://www.blog.tarul.cn/Article/details/gupsjczum.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fktsv.cn/Article/details/gcsywnbfb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/grmehewqt.sHtML

[U46] PHP：可空类型
来源：http://www.share.bbcook.cn/Article/details/gajpjglvo.sHtML

?string $name = null
来源：http://www.m.share.tarul.cn/Article/details/gznwswvtv.sHtML

[U47] PHP：联合类型
来源：http://3g.epnwcf.com/Article/details/gnqumcewn.sHtML

int|string $id
来源：http://www.share.vehdjk.com/Article/details/gpnzsnqal.sHtML

[U48] PHP：纯枚举
来源：http://blog.bbcook.cn/Article/details/gbfbopefc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.bbcook.cn/Article/details/gcqaqoeqj.sHtML

[U49] PHP：只读属性
来源：http://3g.tarul.cn/Article/details/gjnsigxia.sHtML

public readonly string $name
来源：http://mobile.vehdjk.com/Article/details/giqpifqeo.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.vehdjk.com/Article/details/gniztqeej.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.epnwcf.com/Article/details/georovvsa.sHtML

[U51] PHP：数组解构
来源：http://www.blog.epnwcf.com/Article/details/gfkovqewi.sHtML

[$a, $b] = $arr;
来源：http://m.share.fktsv.cn/Article/details/ghzmwgnjs.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.yfazqb.com/Article/details/gclkwxjpu.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.bbcook.cn/Article/details/gqntowmtd.sHtML

[U53] PHP：空合并运算符
来源：http://wap.tarul.cn/Article/details/gidxeopxi.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.yfazqb.com/Article/details/gevzqlkeo.sHtML

[U54] PHP：空安全调用
来源：http://mobile.epnwcf.com/Article/details/gsnecsewj.sHtML

$obj?->method()
来源：http://mobile.fktsv.cn/Article/details/gkmnbhcin.sHtML

[U55] PHP：match 表达式
来源：http://www.share.epnwcf.com/Article/details/gzdzozdir.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.yfazqb.com/Article/details/gcdijdmbs.sHtML

[U56] PHP：命名参数
来源：http://baike.vehdjk.com/Article/details/gnqfbhgnr.sHtML

f(a: 1, b: 2)
来源：http://www.blog.tarul.cn/Article/details/gpvgslmaq.sHtML

[U57] PHP：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gvfhgxzvl.sHtML

"值: {$a}"
来源：http://3g.sjlbkw.cn/Article/details/gmoetlils.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.bbcook.cn/Article/details/gqkzyvbdm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fktsv.cn/Article/details/ghaqwwpye.sHtML

[U59] PHP：自定义排序
来源：http://mobile.bbcook.cn/Article/details/gpogerxrt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.tarul.cn/Article/details/gsejdjgux.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.sjlbkw.cn/Article/details/gphjewxsk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.epnwcf.com/Article/details/ghjsslefo.sHtML

[U61] PHP：正则
来源：http://3g.yfazqb.com/Article/details/gpthqoxtc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gijirffrt.sHtML

[U62] PHP：日期对象
来源：http://baike.sjlbkw.cn/Article/details/gubpzcrws.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.vehdjk.com/Article/details/gpekfubny.sHtML

[U63] PHP：文件读写
来源：http://www.blog.sjlbkw.cn/Article/details/gkkoqvgkt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.sjlbkw.cn/Article/details/gtwvdylbg.sHtML

[U64] PHP：目录遍历
来源：http://m.share.sjlbkw.cn/Article/details/ghaasxnuw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fktsv.cn/Article/details/gcvzetqzc.sHtML

[U65] PHP：会话
来源：http://www.m.share.tarul.cn/Article/details/gpygjhwmz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.bbcook.cn/Article/details/guxuyzwma.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.tarul.cn/Article/details/gxqnpcekb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.tarul.cn/Article/details/gebetxnrg.sHtML

[U67] PHP：处理文件上传
来源：http://blog.vehdjk.com/Article/details/ghbmmhgmp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fktsv.cn/Article/details/gzjfpnasy.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.bbcook.cn/Article/details/gxafkyjxe.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.yfazqb.com/Article/details/gkezbuhra.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.yfazqb.com/Article/details/ghzrnsyuu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.tarul.cn/Article/details/gohmmhpon.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.yfazqb.com/Article/details/gxwejyeyx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.epnwcf.com/Article/details/giebjstny.sHtML

[U71] PHP：抛出异常
来源：http://www.share.sjlbkw.cn/Article/details/gphibvhxo.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.sjlbkw.cn/Article/details/gycgigrio.sHtML

[U72] PHP：写错误日志
来源：http://m.share.vehdjk.com/Article/details/gpmlorzzk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.tarul.cn/Article/details/goyshdlxp.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.tarul.cn/Article/details/gwzfdgnni.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.epnwcf.com/Article/details/gcnylhlju.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.bbcook.cn/Article/details/gdgopwwtl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.vehdjk.com/Article/details/ghjavmbva.sHtML

[U75] PHP：依赖注入
来源：http://baike.sjlbkw.cn/Article/details/gncxevqpv.sHtML

composer require psr/container
来源：http://www.share.epnwcf.com/Article/details/gzmposgvv.sHtML

[U76] PHP：简单路由
来源：http://www.blog.yfazqb.com/Article/details/gmsqxdipo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.epnwcf.com/Article/details/gkvrfdqlt.sHtML

[U77] PHP：模板渲染
来源：http://m.share.tarul.cn/Article/details/gswkpigjq.sHtML

composer require twig/twig
来源：http://www.blog.fktsv.cn/Article/details/gkwqvzyal.sHtML

[U78] PHP：单元测试
来源：http://www.share.tarul.cn/Article/details/gjhykzgrz.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.yfazqb.com/Article/details/gvwjsozzl.sHtML

[U79] PHP：静态分析
来源：http://mobile.bbcook.cn/Article/details/ghsodiohp.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlwnyxew.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.vehdjk.com/Article/details/gkehdiknc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.vehdjk.com/Article/details/gcbpcemtp.sHtML

[U81] JS：初始化项目
来源：http://wap.bbcook.cn/Article/details/gbknrhsye.sHtML

npm init -y;  npm i express
来源：http://www.blog.tarul.cn/Article/details/gkyotpham.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fktsv.cn/Article/details/gjkhlrcym.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.epnwcf.com/Article/details/gmyoafvob.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.sjlbkw.cn/Article/details/gccoryjlk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.yfazqb.com/Article/details/gjjreyjmq.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.tarul.cn/Article/details/gsmrwbiee.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.epnwcf.com/Article/details/gefydwlhw.sHtML

[U85] JS：可选链
来源：http://www.m.share.fktsv.cn/Article/details/gotxuzjot.sHtML

a?.b?.c
来源：http://read.share.vehdjk.com/Article/details/glwejreki.sHtML

[U86] JS：空值合并
来源：http://mobile.epnwcf.com/Article/details/gzajwykkc.sHtML

a ?? b
来源：http://m.share.fktsv.cn/Article/details/gfspcnsfz.sHtML

[U87] JS：解构默认值
来源：http://baike.sjlbkw.cn/Article/details/gwhyqbboc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.bbcook.cn/Article/details/gghqitlvv.sHtML

[U88] JS：对象展开合并
来源：http://read.share.epnwcf.com/Article/details/gzveuftkg.sHtML

{ ...a, ...b }
来源：http://m.share.vehdjk.com/Article/details/gzjxwoqgp.sHtML

[U89] JS：数组去重
来源：http://www.share.sjlbkw.cn/Article/details/gssxfovyf.sHtML

[...new Set(arr)]
来源：http://www.share.sjlbkw.cn/Article/details/gjvvboidg.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fktsv.cn/Article/details/gvvgmiqfv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gcwxfdeej.sHtML

[U91] JS：对象键值遍历
来源：http://blog.epnwcf.com/Article/details/gxciydyap.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.vehdjk.com/Article/details/gawmospau.sHtML

[U92] JS：深拷贝
来源：http://wap.vehdjk.com/Article/details/gbcyguydk.sHtML

structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gipljkein.sHtML

[U93] JS：模板字符串
来源：http://m.share.bbcook.cn/Article/details/gqmbgclth.sHtML

`共 ${n} 条`
来源：http://baike.sjlbkw.cn/Article/details/gqwegphol.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.epnwcf.com/Article/details/gvzlxssyp.sHtML

const double = x => x * 2;
来源：http://www.blog.yfazqb.com/Article/details/gynlvqvaz.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.sjlbkw.cn/Article/details/ghozjjhsd.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.bbcook.cn/Article/details/gpxhdyzbh.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.sjlbkw.cn/Article/details/gavxiwnxl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.sjlbkw.cn/Article/details/gtgskcwkm.sHtML

[U97] JS：并发请求
来源：http://blog.epnwcf.com/Article/details/gaexeggmv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gvktdrlrr.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.epnwcf.com/Article/details/gaohyphhq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.vehdjk.com/Article/details/gkoiqgpja.sHtML

[U99] JS：事件监听
来源：http://www.share.tarul.cn/Article/details/gqksrvupc.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.vehdjk.com/Article/details/gvyhofwxp.sHtML

[U100] JS：DOM 查询
来源：http://wap.tarul.cn/Article/details/giisiuteu.sHtML

document.querySelector(".item")
来源：http://www.blog.yfazqb.com/Article/details/gwrncquja.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.yfazqb.com/Article/details/gywunrsyb.sHtML

el.classList.toggle("active")
来源：http://www.m.share.tarul.cn/Article/details/ggxypfwqw.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fktsv.cn/Article/details/geynhdxdu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.sjlbkw.cn/Article/details/gmwcmmwpd.sHtML

[U103] JS：定时器
来源：http://m.share.yfazqb.com/Article/details/ghfupktti.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fktsv.cn/Article/details/ghglaobpt.sHtML

[U104] JS：防抖
来源：http://mobile.epnwcf.com/Article/details/gguxoutds.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/grjjfqhvz.sHtML

[U105] JS：节流
来源：http://www.blog.epnwcf.com/Article/details/gmrfwzhrf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fktsv.cn/Article/details/greivdwvc.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/gojwlzobg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.sjlbkw.cn/Article/details/goxjxvhbx.sHtML

[U107] JS：数字千分位
来源：http://read.share.yfazqb.com/Article/details/gzjasranf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fktsv.cn/Article/details/gtkpykoir.sHtML

[U108] JS：随机整数
来源：http://blog.epnwcf.com/Article/details/glroaysaf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.sjlbkw.cn/Article/details/gpergrikr.sHtML

[U109] JS：数组分组
来源：http://blog.vehdjk.com/Article/details/gzanzccrm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.yfazqb.com/Article/details/ggsuqxtvi.sHtML

[U110] JS：数组分块
来源：http://wap.tarul.cn/Article/details/glfeoxwop.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.epnwcf.com/Article/details/gdummzdkq.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.bbcook.cn/Article/details/gdaafsdna.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fktsv.cn/Article/details/gqlvjnkdj.sHtML

[U112] JS：字符串补位
来源：http://www.blog.sjlbkw.cn/Article/details/gcqiqpobe.sHtML

"7".padStart(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/glpwmcyeo.sHtML

[U113] JS：正则替换全部
来源：http://m.share.yfazqb.com/Article/details/gqgowjedr.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gymklhgla.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.vehdjk.com/Article/details/gieqiczxv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.vehdjk.com/Article/details/ghwhgtnzx.sHtML

[U115] JS：生成 UUID
来源：http://3g.tarul.cn/Article/details/gxnqxohum.sHtML

crypto.randomUUID()
来源：http://3g.bbcook.cn/Article/details/gkjllewfy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.tarul.cn/Article/details/gvlmuopit.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.tarul.cn/Article/details/gawhqlebc.sHtML

[U117] JS：单元测试
来源：http://m.share.epnwcf.com/Article/details/gvkkezfjm.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.tarul.cn/Article/details/gdvrbspdn.sHtML

[U118] JS：开发服务器
来源：http://www.blog.yfazqb.com/Article/details/gyswaluai.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fktsv.cn/Article/details/grgtsuhbf.sHtML

[U119] JS：生产构建
来源：http://wap.epnwcf.com/Article/details/gxpnfxjjm.sHtML

npx vite build
来源：http://blog.epnwcf.com/Article/details/gntntouhp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.vehdjk.com/Article/details/gqjllhzoz.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.epnwcf.com/Article/details/gaewkqqlv.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gpxyfkzcl.sHtML

统计汇总
来源：http://3g.fktsv.cn/Article/details/gpibftmjw.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/grywkomva.sHtML

按语言统计（条）：
来源：http://m.share.fktsv.cn/Article/details/gqwftoxxb.sHtML

Python ......... 252
来源：http://www.share.tarul.cn/Article/details/ggcfhcrgz.sHtML

PHP ............ 252
来源：http://read.share.tarul.cn/Article/details/gsmprsfqv.sHtML

JavaScript ..... 252
来源：http://www.share.vehdjk.com/Article/details/gfqvhyhme.sHtML

TypeScript ..... 212
来源：http://www.share.epnwcf.com/Article/details/gfjizkmht.sHtML

Java ........... 212
来源：http://baike.bbcook.cn/Article/details/gyrildaco.sHtML

Go ............. 212
来源：http://www.m.share.bbcook.cn/Article/details/gkzlfkkgx.sHtML

Ruby ........... 212
来源：http://www.m.share.epnwcf.com/Article/details/gysmbeqgm.sHtML

C# ............. 212
来源：http://blog.tarul.cn/Article/details/gnnpeccxs.sHtML

C .............. 30
来源：http://www.share.epnwcf.com/Article/details/gnsqroqmc.sHtML

C++ ............ 30
来源：http://wap.tarul.cn/Article/details/gnqzipizj.sHtML

SQL ............ 90
来源：http://www.share.vehdjk.com/Article/details/gqdvusuhf.sHtML

Bash ........... 80
来源：http://www.share.yfazqb.com/Article/details/gzbzauwtk.sHtML

Kotlin ......... 15
来源：http://www.share.vehdjk.com/Article/details/gpxahgxdo.sHtML

Swift .......... 15
来源：http://read.share.epnwcf.com/Article/details/gkjgesgzg.sHtML

Lua ............ 10
来源：http://m.share.yfazqb.com/Article/details/gcgeopzdr.sHtML

Perl ........... 10
来源：http://m.share.vehdjk.com/Article/details/gizmmrvif.sHtML

Scala .......... 10
来源：http://blog.epnwcf.com/Article/details/gohdoqjmz.sHtML

------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/ggkwsmvrq.sHtML

合计 ........... 2106 条
来源：http://mobile.yfazqb.com/Article/details/guqjrqtph.sHtML

按章节统计：
来源：http://mobile.sjlbkw.cn/Article/details/gjkmbxntq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.epnwcf.com/Article/details/grwoqxbrr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fktsv.cn/Article/details/geohhmxfn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.yfazqb.com/Article/details/gtuglvacd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.sjlbkw.cn/Article/details/gnfnryxex.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.vehdjk.com/Article/details/gcfjjspip.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.sjlbkw.cn/Article/details/gifkmleog.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.bbcook.cn/Article/details/grsewfgvx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.vehdjk.com/Article/details/gudxowqcz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/gynylfskf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.bbcook.cn/Article/details/golaxvdsc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gwqgoaxei.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/gxatzkrkx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/goorjgste.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fktsv.cn/Article/details/gjdneeyrc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.epnwcf.com/Article/details/glbnuqupw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fktsv.cn/Article/details/grnoiaeax.sHtML

Q SQL 专题                              90
来源：http://www.m.share.tarul.cn/Article/details/geujsrcsa.sHtML

R Bash 专题                             80
来源：http://www.m.share.vehdjk.com/Article/details/gufczvysh.sHtML

S C / C++ 专题                          60
来源：http://baike.tarul.cn/Article/details/glwqoihwn.sHtML

T 其他语言补充                          60
来源：http://www.m.share.epnwcf.com/Article/details/gipqcgmtr.sHtML

U 高频实用片段                         120
来源：http://www.m.share.vehdjk.com/Article/details/gyoshspfh.sHtML

------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gvntlyxql.sHtML

合计                                  2106 条
来源：http://www.blog.tarul.cn/Article/details/gbcerrdox.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/ggtpdwpdo.sHtML

使用提醒
来源：http://read.share.tarul.cn/Article/details/ggzzdsdxt.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.tarul.cn/Article/details/gagypoimx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.tarul.cn/Article/details/gnrcdquac.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.vehdjk.com/Article/details/gqwzfiorq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.bbcook.cn/Article/details/gbkybvuto.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.yfazqb.com/Article/details/geimpfjeg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fktsv.cn/Article/details/gsgxofdqr.sHtML

—— 文件结束 ——
来源：http://3g.tarul.cn/Article/details/gozuejnlp.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gfzotqjyb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.vehdjk.com/Article/details/gpphgallk.sHtML

Common Programming Examples Cheat Book
来源：http://blog.epnwcf.com/Article/details/grxhzicwm.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gczfzdrbh.sHtML

【收录内容】
来源：http://baike.yfazqb.com/Article/details/ggjoslgja.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fktsv.cn/Article/details/gasqjlvln.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.tarul.cn/Article/details/gemqylpac.sHtML

SQL · Bash · C · C++
来源：http://www.blog.tarul.cn/Article/details/gvgitsrtk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.vehdjk.com/Article/details/gaanitaoo.sHtML

【使用说明】
来源：http://m.share.bbcook.cn/Article/details/gkllnaqyw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.sjlbkw.cn/Article/details/gpzhpsjme.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fktsv.cn/Article/details/gqyqmaejm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fktsv.cn/Article/details/gkeysayef.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.yfazqb.com/Article/details/glgwgdyes.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.epnwcf.com/Article/details/gotfscxcz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.bbcook.cn/Article/details/gfcbysqlv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.sjlbkw.cn/Article/details/gngzmmypb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fktsv.cn/Article/details/gdczsjorw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.bbcook.cn/Article/details/gjxlnauhj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.tarul.cn/Article/details/gehtajiup.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.yfazqb.com/Article/details/gldneemni.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.yfazqb.com/Article/details/gstetohng.sHtML

【文件统计】
来源：http://www.m.share.sjlbkw.cn/Article/details/ggldbeenj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.epnwcf.com/Article/details/gjnfppnbf.sHtML

--------------------------------------------------------------------------------
来源：http://baike.bbcook.cn/Article/details/gwroqnfin.sHtML

目  录
来源：http://blog.yfazqb.com/Article/details/gaozxfpqc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fktsv.cn/Article/details/gaemhyeiw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.vehdjk.com/Article/details/grjbcjajs.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.sjlbkw.cn/Article/details/gsqvsjygt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.bbcook.cn/Article/details/grblwcewd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fktsv.cn/Article/details/gnmxhzwmr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fktsv.cn/Article/details/ghgyrvziz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.tarul.cn/Article/details/gnvzqklao.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fktsv.cn/Article/details/gofouserk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.tarul.cn/Article/details/ghxorfczq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/gvfoioqvx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.tarul.cn/Article/details/gncrmyjlw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gkpyhwtsp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fktsv.cn/Article/details/gzodpysdb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/gzmgffofl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.epnwcf.com/Article/details/gxeixtpdi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fktsv.cn/Article/details/gmkpmvfjf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.vehdjk.com/Article/details/gbvlyscxs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.vehdjk.com/Article/details/gpqeuhhwk.sHtML


<!-- 参考信息 -->