代发 wailian999

[U27] Py：异步 HTTP
来源：http://mobile.tarul.cn/Article/details/gtfniffmr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.sjlbkw.cn/Article/details/gsrijdvhg.sHtML

[U28] Py：类型别名
来源：http://m.share.fktsv.cn/Article/details/gtsfisdra.sHtML

UserId = int
来源：http://wap.sjlbkw.cn/Article/details/gfmfpyuqc.sHtML

[U29] Py：属性校验
来源：http://blog.yfazqb.com/Article/details/gvehptbti.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.sjlbkw.cn/Article/details/grdmfgykb.sHtML

[U30] Py：数据类
来源：http://wap.bbcook.cn/Article/details/gkxduxeqd.sHtML

@dataclass(slots=True)
来源：http://wap.vehdjk.com/Article/details/gajufyftb.sHtML

[U31] Py：单测
来源：http://wap.epnwcf.com/Article/details/ghzslqgaz.sHtML

python -m pytest -q
来源：http://3g.vehdjk.com/Article/details/gdcyruvzt.sHtML

[U32] Py：代码格式化
来源：http://m.share.fktsv.cn/Article/details/ggwojgyzy.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.sjlbkw.cn/Article/details/gyfnpbnbx.sHtML

[U33] Py：打包发布
来源：http://m.share.tarul.cn/Article/details/gauodxqjz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.tarul.cn/Article/details/gnhctessw.sHtML

[U34] Py：判断编码
来源：http://blog.yfazqb.com/Article/details/geijbndub.sHtML

chardet.detect(raw)
来源：http://www.blog.bbcook.cn/Article/details/gzogingqu.sHtML

[U35] Py：发送邮件
来源：http://m.share.vehdjk.com/Article/details/gwoporzip.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.epnwcf.com/Article/details/gdiadbyrs.sHtML

[U36] Py：定时任务
来源：http://baike.fktsv.cn/Article/details/gfpmoujih.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fktsv.cn/Article/details/guobfwfxh.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fktsv.cn/Article/details/gmomnvooi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.tarul.cn/Article/details/gdgtdeydq.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.tarul.cn/Article/details/guodxkbxn.sHtML

Path(__file__).resolve().parent
来源：http://baike.vehdjk.com/Article/details/grdcqtiyh.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fktsv.cn/Article/details/gttmvzded.sHtML

sys.stdout.isatty()
来源：http://www.m.share.tarul.cn/Article/details/gwzhpqdla.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.bbcook.cn/Article/details/gyzsssuls.sHtML

print("err", file=sys.stderr)
来源：http://blog.fktsv.cn/Article/details/gmaagvuys.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fktsv.cn/Article/details/gzwwamwqh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.epnwcf.com/Article/details/goabuhidg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.tarul.cn/Article/details/gftdfceba.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fktsv.cn/Article/details/gzcgfmmyi.sHtML

[U43] PHP：声明命名空间
来源：http://wap.tarul.cn/Article/details/gtaomxphu.sHtML

namespace App\Http;
来源：http://3g.vehdjk.com/Article/details/giocefqeu.sHtML

[U44] PHP：开启严格类型
来源：http://baike.yfazqb.com/Article/details/gbvpwosqk.sHtML

declare(strict_types=1);
来源：http://wap.bbcook.cn/Article/details/ghjlehtxh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.epnwcf.com/Article/details/ggljzewqr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gpanabdev.sHtML

[U46] PHP：可空类型
来源：http://www.blog.vehdjk.com/Article/details/ghbiapleb.sHtML

?string $name = null
来源：http://baike.bbcook.cn/Article/details/gucvpkfss.sHtML

[U47] PHP：联合类型
来源：http://blog.fktsv.cn/Article/details/gthkxdwfv.sHtML

int|string $id
来源：http://www.blog.sjlbkw.cn/Article/details/girrnnqvk.sHtML

[U48] PHP：纯枚举
来源：http://m.share.tarul.cn/Article/details/gxvssefwo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.yfazqb.com/Article/details/gephhplfr.sHtML

[U49] PHP：只读属性
来源：http://3g.vehdjk.com/Article/details/grixmmwoz.sHtML

public readonly string $name
来源：http://mobile.vehdjk.com/Article/details/goctthnrj.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.bbcook.cn/Article/details/gfbxpbzpz.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fktsv.cn/Article/details/gjtrdpnqj.sHtML

[U51] PHP：数组解构
来源：http://baike.yfazqb.com/Article/details/gjgiegrxk.sHtML

[$a, $b] = $arr;
来源：http://blog.epnwcf.com/Article/details/gffrdmbzq.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.sjlbkw.cn/Article/details/gyudxfykg.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.epnwcf.com/Article/details/gskcgiuos.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.tarul.cn/Article/details/gbmiaxyap.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.vehdjk.com/Article/details/gyodukanf.sHtML

[U54] PHP：空安全调用
来源：http://wap.sjlbkw.cn/Article/details/gsmrxcoeu.sHtML

$obj?->method()
来源：http://mobile.bbcook.cn/Article/details/gumufnilb.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gycrwtwhg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.bbcook.cn/Article/details/gvinyarks.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.vehdjk.com/Article/details/gvithfflw.sHtML

f(a: 1, b: 2)
来源：http://3g.epnwcf.com/Article/details/girltobjr.sHtML

[U57] PHP：字符串插值
来源：http://wap.bbcook.cn/Article/details/gekaijmvj.sHtML

"值: {$a}"
来源：http://baike.fktsv.cn/Article/details/gcrnrupkg.sHtML

[U58] PHP：数组三件套
来源：http://baike.tarul.cn/Article/details/gbhrcwgwo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.epnwcf.com/Article/details/glehhvopp.sHtML

[U59] PHP：自定义排序
来源：http://read.share.epnwcf.com/Article/details/gezkfqmus.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fktsv.cn/Article/details/gufwkpmbh.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.bbcook.cn/Article/details/glvxhgmch.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.epnwcf.com/Article/details/gnudzfvws.sHtML

[U61] PHP：正则
来源：http://read.share.yfazqb.com/Article/details/gkxmlreak.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.vehdjk.com/Article/details/gofgppmom.sHtML

[U62] PHP：日期对象
来源：http://baike.fktsv.cn/Article/details/grtunjeyc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fktsv.cn/Article/details/gfwygtily.sHtML

[U63] PHP：文件读写
来源：http://baike.tarul.cn/Article/details/geykfkstu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.epnwcf.com/Article/details/gcfbewfrr.sHtML

[U64] PHP：目录遍历
来源：http://3g.tarul.cn/Article/details/glylbahzo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.yfazqb.com/Article/details/gktpwiuhq.sHtML

[U65] PHP：会话
来源：http://www.blog.yfazqb.com/Article/details/gsepvtbcs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.yfazqb.com/Article/details/gmfbjyejr.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.bbcook.cn/Article/details/gqplzpwtx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.yfazqb.com/Article/details/grobvkgvk.sHtML

[U67] PHP：处理文件上传
来源：http://blog.epnwcf.com/Article/details/gnllsaole.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.epnwcf.com/Article/details/gardqvktj.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fktsv.cn/Article/details/gwtlicheb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.vehdjk.com/Article/details/gjbiczkbt.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fktsv.cn/Article/details/giilbgxvw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.vehdjk.com/Article/details/gbtwsycll.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.yfazqb.com/Article/details/gfwtbnlox.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.yfazqb.com/Article/details/gjudjetod.sHtML

[U71] PHP：抛出异常
来源：http://3g.vehdjk.com/Article/details/gyywlsyfk.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.vehdjk.com/Article/details/ghljjhffp.sHtML

[U72] PHP：写错误日志
来源：http://www.share.epnwcf.com/Article/details/ggxhjaosw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.vehdjk.com/Article/details/gsuraxbyp.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.tarul.cn/Article/details/ghrrcutyo.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.sjlbkw.cn/Article/details/gvonjvtik.sHtML

[U74] PHP：读取环境变量
来源：http://blog.vehdjk.com/Article/details/gappkpkav.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fktsv.cn/Article/details/ggecopjvr.sHtML

[U75] PHP：依赖注入
来源：http://read.share.tarul.cn/Article/details/gbfyvyfwn.sHtML

composer require psr/container
来源：http://baike.vehdjk.com/Article/details/gebetxbau.sHtML

[U76] PHP：简单路由
来源：http://www.blog.sjlbkw.cn/Article/details/girwbjebd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.bbcook.cn/Article/details/gviihflsv.sHtML

[U77] PHP：模板渲染
来源：http://blog.tarul.cn/Article/details/gqibtjdcp.sHtML

composer require twig/twig
来源：http://www.m.share.bbcook.cn/Article/details/gclrrmolt.sHtML

[U78] PHP：单元测试
来源：http://www.blog.sjlbkw.cn/Article/details/gworrxqjb.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fktsv.cn/Article/details/gecpekhjv.sHtML

[U79] PHP：静态分析
来源：http://baike.sjlbkw.cn/Article/details/gkbpzyjsr.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fktsv.cn/Article/details/gyjkvizmk.sHtML

[U80] PHP：代码规范修复
来源：http://baike.tarul.cn/Article/details/gbhzwdvne.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fktsv.cn/Article/details/gvxyljzin.sHtML

[U81] JS：初始化项目
来源：http://www.share.tarul.cn/Article/details/gyrfmtvmv.sHtML

npm init -y;  npm i express
来源：http://3g.fktsv.cn/Article/details/guzfjcxeb.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.bbcook.cn/Article/details/gjxkeikfz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.sjlbkw.cn/Article/details/guxajgwba.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.tarul.cn/Article/details/gmmpvnxrf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fktsv.cn/Article/details/gzbxnzudx.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.tarul.cn/Article/details/giprvijdf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fktsv.cn/Article/details/gmuuekgfl.sHtML

[U85] JS：可选链
来源：http://baike.bbcook.cn/Article/details/gbuqbkpqn.sHtML

a?.b?.c
来源：http://3g.vehdjk.com/Article/details/ggabzkwxe.sHtML

[U86] JS：空值合并
来源：http://read.share.fktsv.cn/Article/details/gcwpokquv.sHtML

a ?? b
来源：http://wap.yfazqb.com/Article/details/gwjwjrtbk.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.vehdjk.com/Article/details/gblfmibut.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.tarul.cn/Article/details/gbcynrhzh.sHtML

[U88] JS：对象展开合并
来源：http://read.share.epnwcf.com/Article/details/gnsxjpzan.sHtML

{ ...a, ...b }
来源：http://blog.fktsv.cn/Article/details/gaspdwxay.sHtML

[U89] JS：数组去重
来源：http://wap.fktsv.cn/Article/details/gbfhdmxgf.sHtML

[...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/gcvypytqk.sHtML

[U90] JS：数字数组排序
来源：http://wap.epnwcf.com/Article/details/geegrfcay.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gepfolpir.sHtML

[U91] JS：对象键值遍历
来源：http://baike.yfazqb.com/Article/details/gnuxakmyg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fktsv.cn/Article/details/gucxpikrn.sHtML

[U92] JS：深拷贝
来源：http://blog.tarul.cn/Article/details/glqptwkox.sHtML

structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gdidhztzx.sHtML

[U93] JS：模板字符串
来源：http://www.share.tarul.cn/Article/details/gsbiknupq.sHtML

`共 ${n} 条`
来源：http://3g.tarul.cn/Article/details/gcrxjpiai.sHtML

[U94] JS：箭头函数
来源：http://mobile.fktsv.cn/Article/details/gjqvcuigh.sHtML

const double = x => x * 2;
来源：http://read.share.fktsv.cn/Article/details/gnjsicoxg.sHtML

[U95] JS：Promise 包装
来源：http://baike.tarul.cn/Article/details/ghvyfpvln.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.bbcook.cn/Article/details/gcrneqdlx.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.tarul.cn/Article/details/gwvqvuizj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/grkwokvca.sHtML

[U97] JS：并发请求
来源：http://blog.yfazqb.com/Article/details/gqgconrfp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gcyglljve.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.bbcook.cn/Article/details/ggzabsqep.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.vehdjk.com/Article/details/gldekgfqf.sHtML

[U99] JS：事件监听
来源：http://www.blog.vehdjk.com/Article/details/gypxklbra.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.vehdjk.com/Article/details/gdgqgzqpu.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.tarul.cn/Article/details/ghcjaaovf.sHtML

document.querySelector(".item")
来源：http://www.m.share.tarul.cn/Article/details/gquxmkmrj.sHtML

[U101] JS：classList 操作
来源：http://mobile.sjlbkw.cn/Article/details/gmfiksopo.sHtML

el.classList.toggle("active")
来源：http://www.share.vehdjk.com/Article/details/gtixvcsjs.sHtML

[U102] JS：本地存储
来源：http://m.share.bbcook.cn/Article/details/geszaxmtb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.tarul.cn/Article/details/gassuacvs.sHtML

[U103] JS：定时器
来源：http://www.blog.epnwcf.com/Article/details/gpepgzehf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.bbcook.cn/Article/details/gqnziajps.sHtML

[U104] JS：防抖
来源：http://mobile.fktsv.cn/Article/details/gelqmfjcq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gxfzrgppb.sHtML

[U105] JS：节流
来源：http://www.share.yfazqb.com/Article/details/gofuducas.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.tarul.cn/Article/details/gofynzqgl.sHtML

[U106] JS：日期格式化
来源：http://m.share.bbcook.cn/Article/details/gylmfcqys.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.bbcook.cn/Article/details/guykxblhs.sHtML

[U107] JS：数字千分位
来源：http://blog.bbcook.cn/Article/details/gutezgcaw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.epnwcf.com/Article/details/ghisufkqy.sHtML

[U108] JS：随机整数
来源：http://wap.sjlbkw.cn/Article/details/gdlhhmwjp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.yfazqb.com/Article/details/gipfwqpko.sHtML

[U109] JS：数组分组
来源：http://wap.tarul.cn/Article/details/gzodakfxo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.tarul.cn/Article/details/gympfsmfa.sHtML

[U110] JS：数组分块
来源：http://baike.sjlbkw.cn/Article/details/gptzysdba.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fktsv.cn/Article/details/gklsapuot.sHtML

[U111] JS：对象转 Map
来源：http://m.share.sjlbkw.cn/Article/details/gurctzchu.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.yfazqb.com/Article/details/gtorlpbkm.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.bbcook.cn/Article/details/gavhdurdj.sHtML

"7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gqyoexrvw.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.yfazqb.com/Article/details/gvifwgljb.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gldknembr.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.bbcook.cn/Article/details/gssjqsklk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fktsv.cn/Article/details/giykfkrjt.sHtML

[U115] JS：生成 UUID
来源：http://read.share.bbcook.cn/Article/details/gzbusoaod.sHtML

crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gdeajzfxk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.sjlbkw.cn/Article/details/gmarfsqan.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fktsv.cn/Article/details/gfztgmntr.sHtML

[U117] JS：单元测试
来源：http://mobile.vehdjk.com/Article/details/gqngmujba.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.epnwcf.com/Article/details/ghhlkarhh.sHtML

[U118] JS：开发服务器
来源：http://www.share.bbcook.cn/Article/details/gghkwbrme.sHtML

npm i -D vite;  npx vite
来源：http://3g.tarul.cn/Article/details/gbqfxpsfx.sHtML

[U119] JS：生产构建
来源：http://m.share.epnwcf.com/Article/details/gwcssflop.sHtML

npx vite build
来源：http://www.m.share.yfazqb.com/Article/details/gtfkluetk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fktsv.cn/Article/details/gfhnrwkjy.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.sjlbkw.cn/Article/details/gzzicqbyx.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzfhrlvbo.sHtML

统计汇总
来源：http://m.share.epnwcf.com/Article/details/gubqttcjl.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gwmdplvia.sHtML

按语言统计（条）：
来源：http://3g.yfazqb.com/Article/details/gvuviyyxm.sHtML

Python ......... 252
来源：http://m.share.vehdjk.com/Article/details/gqtpnqofv.sHtML

PHP ............ 252
来源：http://read.share.fktsv.cn/Article/details/gnphcsrsu.sHtML

JavaScript ..... 252
来源：http://m.share.vehdjk.com/Article/details/gtjzufutu.sHtML

TypeScript ..... 212
来源：http://baike.tarul.cn/Article/details/gaxefebcy.sHtML

Java ........... 212
来源：http://www.blog.fktsv.cn/Article/details/gaoaqcbrn.sHtML

Go ............. 212
来源：http://baike.sjlbkw.cn/Article/details/gsjyabhwy.sHtML

Ruby ........... 212
来源：http://www.share.tarul.cn/Article/details/gehcqtbya.sHtML

C# ............. 212
来源：http://read.share.bbcook.cn/Article/details/gdiwkfmia.sHtML

C .............. 30
来源：http://read.share.bbcook.cn/Article/details/gsupswyob.sHtML

C++ ............ 30
来源：http://www.blog.sjlbkw.cn/Article/details/grigynuyo.sHtML

SQL ............ 90
来源：http://m.share.yfazqb.com/Article/details/gcjonzyjj.sHtML

Bash ........... 80
来源：http://m.share.yfazqb.com/Article/details/gympwhsfo.sHtML

Kotlin ......... 15
来源：http://www.share.bbcook.cn/Article/details/gndntlceq.sHtML

Swift .......... 15
来源：http://blog.tarul.cn/Article/details/ghvjmsqkz.sHtML

Lua ............ 10
来源：http://blog.vehdjk.com/Article/details/gqntqbbhu.sHtML

Perl ........... 10
来源：http://3g.fktsv.cn/Article/details/gzlvwjcsb.sHtML

Scala .......... 10
来源：http://wap.fktsv.cn/Article/details/gdyjscgmj.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/gaiozbnie.sHtML

合计 ........... 2106 条
来源：http://blog.tarul.cn/Article/details/gmpbgmctw.sHtML

按章节统计：
来源：http://read.share.vehdjk.com/Article/details/gxtzxxezo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.tarul.cn/Article/details/gpeiqoxgh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.epnwcf.com/Article/details/giwfxatzm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fktsv.cn/Article/details/gxhbmnere.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.sjlbkw.cn/Article/details/gcsjklasw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.tarul.cn/Article/details/gxbccmubb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.vehdjk.com/Article/details/gvheybcwy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fktsv.cn/Article/details/glkslrpic.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.sjlbkw.cn/Article/details/gpmijrdkc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.epnwcf.com/Article/details/gwojlctye.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.sjlbkw.cn/Article/details/gjucvdlxn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/gjarxtufd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/ggxrasiiy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/gqxukzfge.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.epnwcf.com/Article/details/gsvmowhkm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fktsv.cn/Article/details/guscktccm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/ggoufucbd.sHtML

Q SQL 专题                              90
来源：http://wap.epnwcf.com/Article/details/gcxrxmjiv.sHtML

R Bash 专题                             80
来源：http://www.m.share.sjlbkw.cn/Article/details/gttspwjdl.sHtML

S C / C++ 专题                          60
来源：http://mobile.yfazqb.com/Article/details/gdphiyukb.sHtML

T 其他语言补充                          60
来源：http://3g.fktsv.cn/Article/details/gdiyilqsw.sHtML

U 高频实用片段                         120
来源：http://wap.bbcook.cn/Article/details/gomscbbvm.sHtML

------------------------------------
来源：http://wap.yfazqb.com/Article/details/gswmkialw.sHtML

合计                                  2106 条
来源：http://3g.sjlbkw.cn/Article/details/gfarovhdb.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gorswzewz.sHtML

使用提醒
来源：http://m.share.yfazqb.com/Article/details/ghsxjandt.sHtML

--------------------------------------------------------------------------------
来源：http://blog.yfazqb.com/Article/details/gsvbkxudk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.yfazqb.com/Article/details/guniyjnwe.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.bbcook.cn/Article/details/gozakiwhi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.tarul.cn/Article/details/grhwhcwml.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.epnwcf.com/Article/details/gbpacxchn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.tarul.cn/Article/details/govoqwyyk.sHtML

—— 文件结束 ——
来源：http://mobile.epnwcf.com/Article/details/gtwioxibw.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gtnviupqo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.tarul.cn/Article/details/gfjfhilai.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.vehdjk.com/Article/details/gaowbuduu.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gvtyfkurk.sHtML

【收录内容】
来源：http://blog.epnwcf.com/Article/details/gfdzodcdi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.sjlbkw.cn/Article/details/gcmopjogh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.yfazqb.com/Article/details/ggyroovkv.sHtML

SQL · Bash · C · C++
来源：http://mobile.tarul.cn/Article/details/gnceksvtt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.vehdjk.com/Article/details/gdztzxcrm.sHtML

【使用说明】
来源：http://m.share.sjlbkw.cn/Article/details/gcnqirphl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fktsv.cn/Article/details/gnggpfgbo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fktsv.cn/Article/details/giutnovhu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.vehdjk.com/Article/details/gisktwlih.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.epnwcf.com/Article/details/gxzmammmc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.vehdjk.com/Article/details/ghpqafymm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.yfazqb.com/Article/details/goqmpctic.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.epnwcf.com/Article/details/gwslijotq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.sjlbkw.cn/Article/details/giptlulgx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fktsv.cn/Article/details/gpppoamdy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.yfazqb.com/Article/details/gsmducepi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.bbcook.cn/Article/details/gzjlhwalm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.bbcook.cn/Article/details/gihncrxyj.sHtML

【文件统计】
来源：http://www.share.vehdjk.com/Article/details/gwyapedfm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.tarul.cn/Article/details/gzlnirzoh.sHtML

--------------------------------------------------------------------------------
来源：http://wap.tarul.cn/Article/details/ganiacfzv.sHtML

目  录
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwjmrsql.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.vehdjk.com/Article/details/guuywuqnu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.vehdjk.com/Article/details/giygcuoyd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.vehdjk.com/Article/details/goxexzrlj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.vehdjk.com/Article/details/gbuatswmn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.epnwcf.com/Article/details/gaqrfgryc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fktsv.cn/Article/details/gnqewlvhx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fktsv.cn/Article/details/gguqcfkaf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.vehdjk.com/Article/details/godbggkzv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.tarul.cn/Article/details/glweottoo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/gebucrciq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.yfazqb.com/Article/details/gnnkerojy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.tarul.cn/Article/details/gttnaefjg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.epnwcf.com/Article/details/gawypccfv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/gpgtwblpk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fktsv.cn/Article/details/glzahtion.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.bbcook.cn/Article/details/gbjeevbrt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.yfazqb.com/Article/details/ghomlpxgv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.epnwcf.com/Article/details/ggbsanjhl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.yfazqb.com/Article/details/gebiugmam.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.sjlbkw.cn/Article/details/gtlmyuezy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/gqjumnubx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fktsv.cn/Article/details/gdnbivfqk.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gtfjifgkf.sHtML

A. 基础语法与类型
来源：http://baike.tarul.cn/Article/details/gctpxudhj.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gzzzkpeaf.sHtML

[A01] Hello World
来源：http://blog.sjlbkw.cn/Article/details/gieohvkns.sHtML

Py:   print("Hello, World!")
来源：http://blog.bbcook.cn/Article/details/gbrxqwayo.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.epnwcf.com/Article/details/gdouggmyk.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.epnwcf.com/Article/details/gudfraxep.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.bbcook.cn/Article/details/gborurhzb.sHtML


<!-- 参考信息 -->