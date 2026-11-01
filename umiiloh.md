代发 wailian999

[U19] Py：正则替换带回调
来源：http://read.share.epnwcf.com/Article/details/gwhtrdpvg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fktsv.cn/Article/details/gmuuapfaj.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.tarul.cn/Article/details/gzmtobqas.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fktsv.cn/Article/details/gcgzsouqp.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.yfazqb.com/Article/details/gornphpjz.sHtML

@contextlib.contextmanager
来源：http://baike.vehdjk.com/Article/details/gksjyqxvr.sHtML

[U22] Py：矩阵转置
来源：http://m.share.vehdjk.com/Article/details/gnfdkdmea.sHtML

list(zip(*m))
来源：http://m.share.yfazqb.com/Article/details/gxanvtzdl.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.epnwcf.com/Article/details/geuszdxzh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.epnwcf.com/Article/details/gijrqduqt.sHtML

[U24] Py：路径操作
来源：http://3g.epnwcf.com/Article/details/giyjcbvzb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/gnjwmswky.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.vehdjk.com/Article/details/guynofqfh.sHtML

csv.DictReader(f)
来源：http://3g.yfazqb.com/Article/details/gnydmpqnn.sHtML

[U26] Py：并发下载
来源：http://www.share.vehdjk.com/Article/details/gxvktfxik.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.epnwcf.com/Article/details/gywboelsg.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.epnwcf.com/Article/details/guobiaetz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.yfazqb.com/Article/details/gosnombsc.sHtML

[U28] Py：类型别名
来源：http://www.share.sjlbkw.cn/Article/details/ggiyqlhzu.sHtML

UserId = int
来源：http://m.share.epnwcf.com/Article/details/gnynkxvmt.sHtML

[U29] Py：属性校验
来源：http://www.blog.sjlbkw.cn/Article/details/gbmpvomex.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.vehdjk.com/Article/details/gjbweaujz.sHtML

[U30] Py：数据类
来源：http://www.blog.yfazqb.com/Article/details/gioffihub.sHtML

@dataclass(slots=True)
来源：http://wap.bbcook.cn/Article/details/gugpotlwd.sHtML

[U31] Py：单测
来源：http://3g.yfazqb.com/Article/details/gkuzdlddm.sHtML

python -m pytest -q
来源：http://read.share.sjlbkw.cn/Article/details/ghvvobwbu.sHtML

[U32] Py：代码格式化
来源：http://www.share.epnwcf.com/Article/details/guwssxwqq.sHtML

ruff format . && ruff check --fix .
来源：http://blog.sjlbkw.cn/Article/details/gkbbxtysl.sHtML

[U33] Py：打包发布
来源：http://baike.sjlbkw.cn/Article/details/gqymqfidc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.tarul.cn/Article/details/gphczrxlp.sHtML

[U34] Py：判断编码
来源：http://wap.bbcook.cn/Article/details/gftxnquum.sHtML

chardet.detect(raw)
来源：http://wap.sjlbkw.cn/Article/details/gcsxurcqh.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.tarul.cn/Article/details/glhfdjxhu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.sjlbkw.cn/Article/details/giflqqwtx.sHtML

[U36] Py：定时任务
来源：http://read.share.vehdjk.com/Article/details/grcmccxwh.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.tarul.cn/Article/details/gyvcjzpsi.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.sjlbkw.cn/Article/details/gcborugmu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.bbcook.cn/Article/details/gkzbtljxx.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.bbcook.cn/Article/details/gijlhtmhw.sHtML

Path(__file__).resolve().parent
来源：http://read.share.sjlbkw.cn/Article/details/gxjhovoqz.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.yfazqb.com/Article/details/gtjsupnao.sHtML

sys.stdout.isatty()
来源：http://baike.tarul.cn/Article/details/gsrfalbbt.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.yfazqb.com/Article/details/gijpobvui.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.bbcook.cn/Article/details/gpjnjzfcc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.yfazqb.com/Article/details/gdhwqwuop.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fktsv.cn/Article/details/gloxsmogw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.vehdjk.com/Article/details/gryqqnfyd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.yfazqb.com/Article/details/gfrygbyji.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.sjlbkw.cn/Article/details/gzurzhgad.sHtML

namespace App\Http;
来源：http://wap.fktsv.cn/Article/details/gihbuznic.sHtML

[U44] PHP：开启严格类型
来源：http://baike.epnwcf.com/Article/details/gdxpkregk.sHtML

declare(strict_types=1);
来源：http://read.share.yfazqb.com/Article/details/gsuascynx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fktsv.cn/Article/details/gurswopdw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/gpvbvaadv.sHtML

[U46] PHP：可空类型
来源：http://baike.yfazqb.com/Article/details/gsyldfagb.sHtML

?string $name = null
来源：http://3g.vehdjk.com/Article/details/gsyirgdah.sHtML

[U47] PHP：联合类型
来源：http://wap.epnwcf.com/Article/details/guozrrjwo.sHtML

int|string $id
来源：http://3g.fktsv.cn/Article/details/gpuplpzwi.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.bbcook.cn/Article/details/gdmejspsk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.sjlbkw.cn/Article/details/gikvgqmvs.sHtML

[U49] PHP：只读属性
来源：http://mobile.epnwcf.com/Article/details/gcrfrcbwd.sHtML

public readonly string $name
来源：http://baike.tarul.cn/Article/details/ghlqeqspk.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.vehdjk.com/Article/details/gexhbsoux.sHtML

public function __construct(private int $id) {}
来源：http://mobile.sjlbkw.cn/Article/details/gqplqfzlq.sHtML

[U51] PHP：数组解构
来源：http://www.share.bbcook.cn/Article/details/glbsgquqj.sHtML

[$a, $b] = $arr;
来源：http://m.share.fktsv.cn/Article/details/gnbkfoonp.sHtML

[U52] PHP：箭头函数
来源：http://wap.yfazqb.com/Article/details/gljptzwto.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.bbcook.cn/Article/details/gjacuckkr.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.epnwcf.com/Article/details/giqjppvva.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.vehdjk.com/Article/details/gskcrgnyt.sHtML

[U54] PHP：空安全调用
来源：http://m.share.yfazqb.com/Article/details/gogfxzydw.sHtML

$obj?->method()
来源：http://baike.tarul.cn/Article/details/getvhkivj.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fktsv.cn/Article/details/gajiwtczd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.epnwcf.com/Article/details/ggvflhuvb.sHtML

[U56] PHP：命名参数
来源：http://m.share.epnwcf.com/Article/details/gmffdpanx.sHtML

f(a: 1, b: 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gvesjljud.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.yfazqb.com/Article/details/geeygonny.sHtML

"值: {$a}"
来源：http://m.share.tarul.cn/Article/details/geyfdnhaw.sHtML

[U58] PHP：数组三件套
来源：http://read.share.sjlbkw.cn/Article/details/gippfzsvg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gheimdgjd.sHtML

[U59] PHP：自定义排序
来源：http://3g.tarul.cn/Article/details/ghoetqysa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.yfazqb.com/Article/details/goywkwtvs.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.epnwcf.com/Article/details/gzhzyfqib.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.sjlbkw.cn/Article/details/gikxzjyyp.sHtML

[U61] PHP：正则
来源：http://wap.fktsv.cn/Article/details/gqplarmdd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.tarul.cn/Article/details/gkxqkmxnq.sHtML

[U62] PHP：日期对象
来源：http://www.share.bbcook.cn/Article/details/gtqkzwyfn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.yfazqb.com/Article/details/gwrxssmek.sHtML

[U63] PHP：文件读写
来源：http://blog.fktsv.cn/Article/details/ghucausns.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fktsv.cn/Article/details/grtfvmbbi.sHtML

[U64] PHP：目录遍历
来源：http://mobile.yfazqb.com/Article/details/ghjfwxfib.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.tarul.cn/Article/details/gpvrcxuyw.sHtML

[U65] PHP：会话
来源：http://mobile.vehdjk.com/Article/details/gppmchmjr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.tarul.cn/Article/details/gvmmehkcx.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.bbcook.cn/Article/details/guhoxtzyo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fktsv.cn/Article/details/gmtoqkukl.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.vehdjk.com/Article/details/gwcclhkum.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.epnwcf.com/Article/details/gyomsbnbe.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.vehdjk.com/Article/details/gixzhubba.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.bbcook.cn/Article/details/gfkneonkd.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.epnwcf.com/Article/details/gzbfmlhac.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.vehdjk.com/Article/details/gzkrxxqqn.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.yfazqb.com/Article/details/gcxosvtpz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.vehdjk.com/Article/details/gjcydqvhb.sHtML

[U71] PHP：抛出异常
来源：http://wap.yfazqb.com/Article/details/gjducxhtt.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.bbcook.cn/Article/details/gzavhrmcj.sHtML

[U72] PHP：写错误日志
来源：http://3g.bbcook.cn/Article/details/gitbomccb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.tarul.cn/Article/details/ghykbexde.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.epnwcf.com/Article/details/gxlfhvypm.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.bbcook.cn/Article/details/gwmlmslou.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.tarul.cn/Article/details/gefryfaai.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.vehdjk.com/Article/details/gvsbvewtu.sHtML

[U75] PHP：依赖注入
来源：http://blog.fktsv.cn/Article/details/gqsbvcrdr.sHtML

composer require psr/container
来源：http://www.m.share.yfazqb.com/Article/details/guzksgcrj.sHtML

[U76] PHP：简单路由
来源：http://baike.yfazqb.com/Article/details/gdqmzmunw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.epnwcf.com/Article/details/gduqgmfsq.sHtML

[U77] PHP：模板渲染
来源：http://blog.sjlbkw.cn/Article/details/glixpxory.sHtML

composer require twig/twig
来源：http://3g.yfazqb.com/Article/details/gprgdbezg.sHtML

[U78] PHP：单元测试
来源：http://mobile.fktsv.cn/Article/details/gqeobhxlc.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.sjlbkw.cn/Article/details/girhnfumb.sHtML

[U79] PHP：静态分析
来源：http://blog.vehdjk.com/Article/details/gfkknwwrz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.yfazqb.com/Article/details/gexxsewwr.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.epnwcf.com/Article/details/gxcmgsyyt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.vehdjk.com/Article/details/gqutoooym.sHtML

[U81] JS：初始化项目
来源：http://mobile.epnwcf.com/Article/details/gpzkgpvov.sHtML

npm init -y;  npm i express
来源：http://www.m.share.epnwcf.com/Article/details/gnpethnph.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.sjlbkw.cn/Article/details/gppcdcdfw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.vehdjk.com/Article/details/gyyjnzsfw.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.yfazqb.com/Article/details/gvjgxooau.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fktsv.cn/Article/details/gaevmrosq.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.yfazqb.com/Article/details/gyryafcyg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.bbcook.cn/Article/details/garnyzmcm.sHtML

[U85] JS：可选链
来源：http://mobile.tarul.cn/Article/details/gmqfkcroj.sHtML

a?.b?.c
来源：http://wap.vehdjk.com/Article/details/gydcvewyi.sHtML

[U86] JS：空值合并
来源：http://read.share.tarul.cn/Article/details/gulphrlcz.sHtML

a ?? b
来源：http://read.share.epnwcf.com/Article/details/gcpcgsvoe.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fktsv.cn/Article/details/grzajvuix.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.yfazqb.com/Article/details/ghapvzsuz.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.tarul.cn/Article/details/gpxratggb.sHtML

{ ...a, ...b }
来源：http://m.share.fktsv.cn/Article/details/gbygmhzmk.sHtML

[U89] JS：数组去重
来源：http://baike.yfazqb.com/Article/details/gmfhvqdxy.sHtML

[...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/gzwnthnvh.sHtML

[U90] JS：数字数组排序
来源：http://3g.vehdjk.com/Article/details/guwomknrd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gwgoaoqwb.sHtML

[U91] JS：对象键值遍历
来源：http://3g.sjlbkw.cn/Article/details/gelkshlpe.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.epnwcf.com/Article/details/gifbpbcoq.sHtML

[U92] JS：深拷贝
来源：http://blog.vehdjk.com/Article/details/gknyqnnbq.sHtML

structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/gzvdfhtjt.sHtML

[U93] JS：模板字符串
来源：http://m.share.epnwcf.com/Article/details/giqpwucna.sHtML

`共 ${n} 条`
来源：http://www.blog.bbcook.cn/Article/details/gfkeexhxv.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fktsv.cn/Article/details/gnwaeykbq.sHtML

const double = x => x * 2;
来源：http://m.share.fktsv.cn/Article/details/gfkfkmomk.sHtML

[U95] JS：Promise 包装
来源：http://www.share.sjlbkw.cn/Article/details/gjmxzhgan.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.yfazqb.com/Article/details/gqvmneqpu.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.epnwcf.com/Article/details/gvzmkoasn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gyndiqsur.sHtML

[U97] JS：并发请求
来源：http://www.share.fktsv.cn/Article/details/gtarqurdx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/gfzyuvkky.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.sjlbkw.cn/Article/details/gmxoxizko.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.vehdjk.com/Article/details/ghixcakfn.sHtML

[U99] JS：事件监听
来源：http://www.share.tarul.cn/Article/details/gxtqswpyz.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fktsv.cn/Article/details/gmrcafnji.sHtML

[U100] JS：DOM 查询
来源：http://blog.yfazqb.com/Article/details/geikzbudp.sHtML

document.querySelector(".item")
来源：http://read.share.sjlbkw.cn/Article/details/gxatjfoon.sHtML

[U101] JS：classList 操作
来源：http://m.share.bbcook.cn/Article/details/gogrhdsme.sHtML

el.classList.toggle("active")
来源：http://3g.fktsv.cn/Article/details/gygndfvkc.sHtML

[U102] JS：本地存储
来源：http://read.share.bbcook.cn/Article/details/gfykqwdas.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fktsv.cn/Article/details/gnbigzzbm.sHtML

[U103] JS：定时器
来源：http://wap.bbcook.cn/Article/details/gztwnqxnn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fktsv.cn/Article/details/ghtblhwlt.sHtML

[U104] JS：防抖
来源：http://www.share.fktsv.cn/Article/details/ghiiiujbt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gtcvztxdc.sHtML

[U105] JS：节流
来源：http://blog.yfazqb.com/Article/details/gunqhscmu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.vehdjk.com/Article/details/gokwatnpk.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fktsv.cn/Article/details/gkmeapahl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.epnwcf.com/Article/details/gbkwqimss.sHtML

[U107] JS：数字千分位
来源：http://www.blog.vehdjk.com/Article/details/glisrbbna.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.epnwcf.com/Article/details/gnknlxcaj.sHtML

[U108] JS：随机整数
来源：http://m.share.yfazqb.com/Article/details/gnpshdsoo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fktsv.cn/Article/details/goxtjlegh.sHtML

[U109] JS：数组分组
来源：http://read.share.yfazqb.com/Article/details/gmzvroafz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fktsv.cn/Article/details/gpuerijsy.sHtML

[U110] JS：数组分块
来源：http://www.blog.vehdjk.com/Article/details/gwmgddyuy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fktsv.cn/Article/details/gwmebsvoj.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.vehdjk.com/Article/details/gkvyndher.sHtML

new Map(Object.entries(obj))
来源：http://3g.fktsv.cn/Article/details/ghicrijhk.sHtML

[U112] JS：字符串补位
来源：http://read.share.fktsv.cn/Article/details/gmrgonday.sHtML

"7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/grxdeydpb.sHtML

[U113] JS：正则替换全部
来源：http://wap.yfazqb.com/Article/details/goosowswa.sHtML

s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gtkxoabvb.sHtML

[U114] JS：JSON 深比较
来源：http://blog.sjlbkw.cn/Article/details/ggsluohts.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.yfazqb.com/Article/details/gpyjpxtoo.sHtML

[U115] JS：生成 UUID
来源：http://read.share.epnwcf.com/Article/details/gzslldwsl.sHtML

crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/ggnhrhbwr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.yfazqb.com/Article/details/gdgxzsjra.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.tarul.cn/Article/details/gpfkjeusr.sHtML

[U117] JS：单元测试
来源：http://www.blog.bbcook.cn/Article/details/gytykuumt.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.tarul.cn/Article/details/gveavwpzi.sHtML

[U118] JS：开发服务器
来源：http://www.blog.bbcook.cn/Article/details/gsuqjetkb.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fktsv.cn/Article/details/gltjfaqvw.sHtML

[U119] JS：生产构建
来源：http://read.share.fktsv.cn/Article/details/gqwyvdxua.sHtML

npx vite build
来源：http://wap.yfazqb.com/Article/details/gnsvihdgk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.vehdjk.com/Article/details/gxmvvjpkp.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.epnwcf.com/Article/details/goiwfmbud.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gktoxfvct.sHtML

统计汇总
来源：http://blog.vehdjk.com/Article/details/gudzfhilt.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gatugsqns.sHtML

按语言统计（条）：
来源：http://www.blog.sjlbkw.cn/Article/details/gwrwtweci.sHtML

Python ......... 252
来源：http://www.blog.fktsv.cn/Article/details/gtrqdszoc.sHtML

PHP ............ 252
来源：http://m.share.sjlbkw.cn/Article/details/gfxgmnlol.sHtML

JavaScript ..... 252
来源：http://www.share.vehdjk.com/Article/details/gkwxsgazt.sHtML

TypeScript ..... 212
来源：http://blog.bbcook.cn/Article/details/gwrhscnlz.sHtML

Java ........... 212
来源：http://www.blog.sjlbkw.cn/Article/details/gnwojfodw.sHtML

Go ............. 212
来源：http://3g.vehdjk.com/Article/details/gmbtrqkuo.sHtML

Ruby ........... 212
来源：http://www.m.share.yfazqb.com/Article/details/gtnefkddk.sHtML

C# ............. 212
来源：http://3g.tarul.cn/Article/details/gojpkqewg.sHtML

C .............. 30
来源：http://www.m.share.yfazqb.com/Article/details/gbkmabvjf.sHtML

C++ ............ 30
来源：http://3g.yfazqb.com/Article/details/ghdcwxteu.sHtML

SQL ............ 90
来源：http://www.blog.fktsv.cn/Article/details/gnnwchazg.sHtML

Bash ........... 80
来源：http://www.blog.yfazqb.com/Article/details/gywskgbxw.sHtML

Kotlin ......... 15
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrcukhbs.sHtML

Swift .......... 15
来源：http://baike.yfazqb.com/Article/details/gbdxsblyg.sHtML

Lua ............ 10
来源：http://www.share.fktsv.cn/Article/details/ghrvipiok.sHtML

Perl ........... 10
来源：http://mobile.tarul.cn/Article/details/gqmxrjevv.sHtML

Scala .......... 10
来源：http://read.share.yfazqb.com/Article/details/gomqaxpeu.sHtML

------------------------------------
来源：http://3g.tarul.cn/Article/details/gfubqxkdm.sHtML

合计 ........... 2106 条
来源：http://www.share.sjlbkw.cn/Article/details/gxwmmfbje.sHtML

按章节统计：
来源：http://read.share.tarul.cn/Article/details/gyjbaxdmq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.yfazqb.com/Article/details/gqbvnguvh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.tarul.cn/Article/details/gayqjymko.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.epnwcf.com/Article/details/ggvcusvyt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.vehdjk.com/Article/details/gzxzfiqrv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.yfazqb.com/Article/details/guebqhcxz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.bbcook.cn/Article/details/gatzhaipe.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnfmvdxy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.yfazqb.com/Article/details/gkdqgxhwj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gsbdsxrid.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.vehdjk.com/Article/details/gvernvvev.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/ggxntpshn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/gygpgmtvd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/gzushrjwh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fktsv.cn/Article/details/gjxauwaop.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.bbcook.cn/Article/details/gezjbyffg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/getqjgmqu.sHtML

Q SQL 专题                              90
来源：http://www.share.sjlbkw.cn/Article/details/gkwnphawd.sHtML

R Bash 专题                             80
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgxcoqxw.sHtML

S C / C++ 专题                          60
来源：http://m.share.epnwcf.com/Article/details/gpurhcini.sHtML

T 其他语言补充                          60
来源：http://3g.bbcook.cn/Article/details/giosdtxvh.sHtML

U 高频实用片段                         120
来源：http://www.share.yfazqb.com/Article/details/gqrhggykd.sHtML

------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gplwikdbr.sHtML

合计                                  2106 条
来源：http://www.blog.bbcook.cn/Article/details/gviwmlsdn.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/gluktjyft.sHtML

使用提醒
来源：http://www.share.fktsv.cn/Article/details/gbbjrywoa.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gszzpunme.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.bbcook.cn/Article/details/gsgamftvt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.sjlbkw.cn/Article/details/guwmxugfi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.vehdjk.com/Article/details/ghdholavb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fktsv.cn/Article/details/gbustwnlh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.sjlbkw.cn/Article/details/gwsohjrcp.sHtML

—— 文件结束 ——
来源：http://wap.sjlbkw.cn/Article/details/gnksodbhv.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gmgqqiyvb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fktsv.cn/Article/details/gxvvrvjhr.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.vehdjk.com/Article/details/gsovkbmhb.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gojtxoxco.sHtML

【收录内容】
来源：http://www.blog.epnwcf.com/Article/details/gylyxtpcm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.bbcook.cn/Article/details/gemtwywmu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fktsv.cn/Article/details/ghvlpysmz.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.vehdjk.com/Article/details/glcgmwiub.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.tarul.cn/Article/details/guqecnnvg.sHtML

【使用说明】
来源：http://www.blog.sjlbkw.cn/Article/details/gwmyifyok.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fktsv.cn/Article/details/gsxmkqqag.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fktsv.cn/Article/details/gkkcoaiba.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.bbcook.cn/Article/details/gvgkixnqy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.epnwcf.com/Article/details/grwyqsrct.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.epnwcf.com/Article/details/ggdfxuimh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fktsv.cn/Article/details/gkknlexsc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.tarul.cn/Article/details/gwadiiexl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.bbcook.cn/Article/details/gwcwnntbg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.tarul.cn/Article/details/gfgtjzwhj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.vehdjk.com/Article/details/gzrakfynz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.epnwcf.com/Article/details/gkgltlyzi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.yfazqb.com/Article/details/gjkomoysv.sHtML

【文件统计】
来源：http://mobile.vehdjk.com/Article/details/geepypqho.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.sjlbkw.cn/Article/details/gtmxhjobm.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gwgxedrzz.sHtML

目  录
来源：http://baike.sjlbkw.cn/Article/details/guszxizae.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fktsv.cn/Article/details/gdpcjnvct.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.sjlbkw.cn/Article/details/geqsqgqoi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.bbcook.cn/Article/details/gakvciorf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.epnwcf.com/Article/details/gjhhrhxdj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.tarul.cn/Article/details/gdiqxuloe.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.vehdjk.com/Article/details/gnnwrxfea.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.epnwcf.com/Article/details/globshzfx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.epnwcf.com/Article/details/gsxzudorl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.epnwcf.com/Article/details/gfasyzygm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/gpqjmdfpy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.tarul.cn/Article/details/gmgpzenqx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/gboxcfdqy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.sjlbkw.cn/Article/details/gvoypzpnx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fktsv.cn/Article/details/gounszszi.sHtML


<!-- 参考信息 -->