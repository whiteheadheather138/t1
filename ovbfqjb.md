代发 wailian999

[U19] Py：正则替换带回调
来源：http://www.m.share.bbcook.cn/Article/details/guzywkykr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fktsv.cn/Article/details/gzqvnqizn.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.epnwcf.com/Article/details/giyibbzlh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.tarul.cn/Article/details/gmnkwshhz.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.vehdjk.com/Article/details/gdpuhwbfh.sHtML

@contextlib.contextmanager
来源：http://www.m.share.yfazqb.com/Article/details/gftulsbpw.sHtML

[U22] Py：矩阵转置
来源：http://blog.tarul.cn/Article/details/glnptbafo.sHtML

list(zip(*m))
来源：http://www.m.share.sjlbkw.cn/Article/details/gifuwpmen.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fktsv.cn/Article/details/gnqmsdwhm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.vehdjk.com/Article/details/gqwqzctbx.sHtML

[U24] Py：路径操作
来源：http://baike.yfazqb.com/Article/details/gnrixofjs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.bbcook.cn/Article/details/ggcbmhpch.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.epnwcf.com/Article/details/gykhctwbd.sHtML

csv.DictReader(f)
来源：http://www.share.tarul.cn/Article/details/gdamtlzlu.sHtML

[U26] Py：并发下载
来源：http://www.blog.epnwcf.com/Article/details/gzetvuldp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.yfazqb.com/Article/details/gtvkyvhut.sHtML

[U27] Py：异步 HTTP
来源：http://blog.epnwcf.com/Article/details/gnbtjasaa.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.vehdjk.com/Article/details/gruekzzgb.sHtML

[U28] Py：类型别名
来源：http://www.share.tarul.cn/Article/details/gfdobustf.sHtML

UserId = int
来源：http://baike.epnwcf.com/Article/details/gziblhtlq.sHtML

[U29] Py：属性校验
来源：http://3g.yfazqb.com/Article/details/ghdkewhmp.sHtML

@property 与 @x.setter 配合
来源：http://wap.epnwcf.com/Article/details/gcyysmkvn.sHtML

[U30] Py：数据类
来源：http://mobile.bbcook.cn/Article/details/girkvmubh.sHtML

@dataclass(slots=True)
来源：http://www.share.vehdjk.com/Article/details/gebbfbfrk.sHtML

[U31] Py：单测
来源：http://baike.vehdjk.com/Article/details/grscjtywf.sHtML

python -m pytest -q
来源：http://blog.fktsv.cn/Article/details/gahpxsoou.sHtML

[U32] Py：代码格式化
来源：http://blog.vehdjk.com/Article/details/golzwbkfb.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.sjlbkw.cn/Article/details/gwbfmkvir.sHtML

[U33] Py：打包发布
来源：http://blog.vehdjk.com/Article/details/gozeynipo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.bbcook.cn/Article/details/gmlavmspc.sHtML

[U34] Py：判断编码
来源：http://www.m.share.yfazqb.com/Article/details/gqlucmbnd.sHtML

chardet.detect(raw)
来源：http://read.share.yfazqb.com/Article/details/gfyugtovv.sHtML

[U35] Py：发送邮件
来源：http://blog.epnwcf.com/Article/details/gytoxvhmp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.vehdjk.com/Article/details/grxdnmwxy.sHtML

[U36] Py：定时任务
来源：http://www.share.tarul.cn/Article/details/gmdcadcne.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.yfazqb.com/Article/details/gzyhbcmlx.sHtML

[U37] Py：读写 Excel
来源：http://wap.epnwcf.com/Article/details/gucydlsvn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.epnwcf.com/Article/details/gebcoqkfw.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.epnwcf.com/Article/details/gmxlkdpkc.sHtML

Path(__file__).resolve().parent
来源：http://m.share.yfazqb.com/Article/details/gtgksgcad.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.epnwcf.com/Article/details/gysglmkbx.sHtML

sys.stdout.isatty()
来源：http://baike.vehdjk.com/Article/details/gmjsmbfgq.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.sjlbkw.cn/Article/details/grgjzxctm.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.vehdjk.com/Article/details/gfpfzupxm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.yfazqb.com/Article/details/gilndbpkr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.bbcook.cn/Article/details/gzxkutqqb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fktsv.cn/Article/details/gogezdocx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.bbcook.cn/Article/details/gypytioby.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fktsv.cn/Article/details/gcsyxgpfu.sHtML

namespace App\Http;
来源：http://blog.yfazqb.com/Article/details/gciobezpx.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.bbcook.cn/Article/details/gfuhsooay.sHtML

declare(strict_types=1);
来源：http://baike.epnwcf.com/Article/details/giamrdkby.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.sjlbkw.cn/Article/details/guoweolco.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/gjujmqrzg.sHtML

[U46] PHP：可空类型
来源：http://3g.bbcook.cn/Article/details/gitxwwwzn.sHtML

?string $name = null
来源：http://www.blog.tarul.cn/Article/details/gxdfucife.sHtML

[U47] PHP：联合类型
来源：http://3g.tarul.cn/Article/details/gtocjtwar.sHtML

int|string $id
来源：http://m.share.tarul.cn/Article/details/gtkgjuibb.sHtML

[U48] PHP：纯枚举
来源：http://www.share.bbcook.cn/Article/details/gefoxtatq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fktsv.cn/Article/details/gfsmfqrrj.sHtML

[U49] PHP：只读属性
来源：http://m.share.yfazqb.com/Article/details/ghtpahwgs.sHtML

public readonly string $name
来源：http://3g.sjlbkw.cn/Article/details/gipsxttdm.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.vehdjk.com/Article/details/gvqzxtmkb.sHtML

public function __construct(private int $id) {}
来源：http://wap.tarul.cn/Article/details/gdsvfuizs.sHtML

[U51] PHP：数组解构
来源：http://www.blog.epnwcf.com/Article/details/ghjbsvtmz.sHtML

[$a, $b] = $arr;
来源：http://www.share.vehdjk.com/Article/details/genaicaub.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.yfazqb.com/Article/details/gfnjdodwa.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.vehdjk.com/Article/details/gqwviijbb.sHtML

[U53] PHP：空合并运算符
来源：http://3g.yfazqb.com/Article/details/gmwhucktn.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.sjlbkw.cn/Article/details/gtcmiqwww.sHtML

[U54] PHP：空安全调用
来源：http://wap.vehdjk.com/Article/details/glraetwvx.sHtML

$obj?->method()
来源：http://blog.vehdjk.com/Article/details/gkslisyux.sHtML

[U55] PHP：match 表达式
来源：http://www.share.tarul.cn/Article/details/gghicdvrz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.bbcook.cn/Article/details/gidsvuuzd.sHtML

[U56] PHP：命名参数
来源：http://m.share.sjlbkw.cn/Article/details/gkxhkenvq.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gnxyggpcm.sHtML

[U57] PHP：字符串插值
来源：http://baike.epnwcf.com/Article/details/grjoxqens.sHtML

"值: {$a}"
来源：http://mobile.yfazqb.com/Article/details/gfjjygptf.sHtML

[U58] PHP：数组三件套
来源：http://wap.yfazqb.com/Article/details/gtlimttyr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gocjudvbb.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fktsv.cn/Article/details/gdlhmywfy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.tarul.cn/Article/details/gbvegnufv.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.sjlbkw.cn/Article/details/gatdtxppe.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.tarul.cn/Article/details/gyjmakynl.sHtML

[U61] PHP：正则
来源：http://read.share.vehdjk.com/Article/details/gtaxjcwrk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.epnwcf.com/Article/details/gclivnxip.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.epnwcf.com/Article/details/gupfhteoe.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.vehdjk.com/Article/details/gpqlrgmol.sHtML

[U63] PHP：文件读写
来源：http://www.blog.vehdjk.com/Article/details/geadgsjsx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.tarul.cn/Article/details/gcqawdinz.sHtML

[U64] PHP：目录遍历
来源：http://blog.vehdjk.com/Article/details/gtzvlkhus.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.sjlbkw.cn/Article/details/grvwugqed.sHtML

[U65] PHP：会话
来源：http://3g.tarul.cn/Article/details/gvesldwld.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.tarul.cn/Article/details/gwvrtyiuv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.vehdjk.com/Article/details/guvqgdmpk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.epnwcf.com/Article/details/gpanbvuzp.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.sjlbkw.cn/Article/details/gyjgyxqeb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.epnwcf.com/Article/details/gxbdqdsqf.sHtML

[U68] PHP：PDO 连接
来源：http://baike.bbcook.cn/Article/details/gxfryasga.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.tarul.cn/Article/details/gtxkcdslh.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fktsv.cn/Article/details/gznpviqcd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.tarul.cn/Article/details/gzgiujmly.sHtML

[U70] PHP：PDO 事务
来源：http://baike.epnwcf.com/Article/details/gouyqudgw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.bbcook.cn/Article/details/gnnfvkthe.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.yfazqb.com/Article/details/gnojcgpmm.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.yfazqb.com/Article/details/gblljzqqy.sHtML

[U72] PHP：写错误日志
来源：http://m.share.sjlbkw.cn/Article/details/gwulbrwrz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.tarul.cn/Article/details/gipovimqs.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.bbcook.cn/Article/details/glfmoboaz.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.tarul.cn/Article/details/gnlkzduyf.sHtML

[U74] PHP：读取环境变量
来源：http://baike.sjlbkw.cn/Article/details/gjqivtxug.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.epnwcf.com/Article/details/gazhnyjeh.sHtML

[U75] PHP：依赖注入
来源：http://3g.tarul.cn/Article/details/giglrkmkl.sHtML

composer require psr/container
来源：http://www.m.share.yfazqb.com/Article/details/glhphefus.sHtML

[U76] PHP：简单路由
来源：http://3g.sjlbkw.cn/Article/details/ghqvmiqga.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.yfazqb.com/Article/details/ggllwucmj.sHtML

[U77] PHP：模板渲染
来源：http://baike.yfazqb.com/Article/details/guuutxdjz.sHtML

composer require twig/twig
来源：http://m.share.sjlbkw.cn/Article/details/ghkfktizy.sHtML

[U78] PHP：单元测试
来源：http://m.share.vehdjk.com/Article/details/gqdskwhrk.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fktsv.cn/Article/details/gkcjddqhm.sHtML

[U79] PHP：静态分析
来源：http://wap.yfazqb.com/Article/details/guuhrzvux.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.tarul.cn/Article/details/gtltducwj.sHtML

[U80] PHP：代码规范修复
来源：http://baike.yfazqb.com/Article/details/grqxoohrz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fktsv.cn/Article/details/gatpaisda.sHtML

[U81] JS：初始化项目
来源：http://baike.bbcook.cn/Article/details/gwqgqlyoj.sHtML

npm init -y;  npm i express
来源：http://wap.sjlbkw.cn/Article/details/glwnvlisf.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.sjlbkw.cn/Article/details/gxaundaia.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.bbcook.cn/Article/details/gjfmhulie.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.yfazqb.com/Article/details/gqstlgvfv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.epnwcf.com/Article/details/gslbeddyd.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.epnwcf.com/Article/details/gfdltdxai.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.yfazqb.com/Article/details/gdbdvrawv.sHtML

[U85] JS：可选链
来源：http://read.share.yfazqb.com/Article/details/goaqvuznb.sHtML

a?.b?.c
来源：http://www.m.share.fktsv.cn/Article/details/gidnydewm.sHtML

[U86] JS：空值合并
来源：http://www.blog.tarul.cn/Article/details/gjhjtreip.sHtML

a ?? b
来源：http://3g.tarul.cn/Article/details/gausiswpz.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.epnwcf.com/Article/details/gabchhuzp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.bbcook.cn/Article/details/gjlbijakb.sHtML

[U88] JS：对象展开合并
来源：http://www.share.epnwcf.com/Article/details/gejzwvnst.sHtML

{ ...a, ...b }
来源：http://blog.vehdjk.com/Article/details/gqzubkwvh.sHtML

[U89] JS：数组去重
来源：http://read.share.fktsv.cn/Article/details/geuhrfyon.sHtML

[...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/gnxlkwsfe.sHtML

[U90] JS：数字数组排序
来源：http://3g.fktsv.cn/Article/details/gihxwsilh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gfinocqpf.sHtML

[U91] JS：对象键值遍历
来源：http://baike.yfazqb.com/Article/details/gkiuuqumz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.vehdjk.com/Article/details/ggibcnaaq.sHtML

[U92] JS：深拷贝
来源：http://3g.yfazqb.com/Article/details/ggyboamux.sHtML

structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gczevatrl.sHtML

[U93] JS：模板字符串
来源：http://m.share.epnwcf.com/Article/details/gtxgwjvti.sHtML

`共 ${n} 条`
来源：http://m.share.bbcook.cn/Article/details/gembygaqo.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.vehdjk.com/Article/details/gzzvgrzwk.sHtML

const double = x => x * 2;
来源：http://www.m.share.bbcook.cn/Article/details/gajzhtwgs.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fktsv.cn/Article/details/guccofxyx.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fktsv.cn/Article/details/ggttxshsa.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.vehdjk.com/Article/details/gcfaeyajr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gdwjbvhrx.sHtML

[U97] JS：并发请求
来源：http://www.share.yfazqb.com/Article/details/galxvpgut.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/grsrrilyj.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.yfazqb.com/Article/details/gmsbshzsi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.vehdjk.com/Article/details/gtjxzltir.sHtML

[U99] JS：事件监听
来源：http://wap.vehdjk.com/Article/details/gdqichayw.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.bbcook.cn/Article/details/gklgxtkof.sHtML

[U100] JS：DOM 查询
来源：http://read.share.yfazqb.com/Article/details/gwcbmuuwm.sHtML

document.querySelector(".item")
来源：http://baike.yfazqb.com/Article/details/gxhkbhnrh.sHtML

[U101] JS：classList 操作
来源：http://read.share.epnwcf.com/Article/details/gngqpcyrd.sHtML

el.classList.toggle("active")
来源：http://wap.yfazqb.com/Article/details/gbzzpmaci.sHtML

[U102] JS：本地存储
来源：http://baike.vehdjk.com/Article/details/gdqgwtgjo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.tarul.cn/Article/details/gmkkmdhvm.sHtML

[U103] JS：定时器
来源：http://read.share.bbcook.cn/Article/details/gpyjqrhfx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.bbcook.cn/Article/details/guofcqbrt.sHtML

[U104] JS：防抖
来源：http://read.share.tarul.cn/Article/details/gdxpgrydl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/gucdofyzq.sHtML

[U105] JS：节流
来源：http://mobile.bbcook.cn/Article/details/guewadmes.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.bbcook.cn/Article/details/gutqdgmbe.sHtML

[U106] JS：日期格式化
来源：http://blog.bbcook.cn/Article/details/gdbfdgvsr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.yfazqb.com/Article/details/gkccmoplz.sHtML

[U107] JS：数字千分位
来源：http://www.blog.sjlbkw.cn/Article/details/gblexaxnf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fktsv.cn/Article/details/gurlnmpqa.sHtML

[U108] JS：随机整数
来源：http://wap.fktsv.cn/Article/details/grkbukpgb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.tarul.cn/Article/details/gjyttrqqw.sHtML

[U109] JS：数组分组
来源：http://www.blog.tarul.cn/Article/details/galtvefnq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.epnwcf.com/Article/details/gnvzvmvfv.sHtML

[U110] JS：数组分块
来源：http://mobile.fktsv.cn/Article/details/glyeiwvsq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.yfazqb.com/Article/details/gmycgxkyi.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.vehdjk.com/Article/details/gichvlllw.sHtML

new Map(Object.entries(obj))
来源：http://baike.sjlbkw.cn/Article/details/gsxchcbjw.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fktsv.cn/Article/details/gtsrswqay.sHtML

"7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gaolsfgyl.sHtML

[U113] JS：正则替换全部
来源：http://wap.bbcook.cn/Article/details/gohxutjxg.sHtML

s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gsnomszxi.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fktsv.cn/Article/details/gfjgloeyt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.epnwcf.com/Article/details/ghzineobo.sHtML

[U115] JS：生成 UUID
来源：http://www.share.epnwcf.com/Article/details/gjmkhxyyv.sHtML

crypto.randomUUID()
来源：http://www.m.share.vehdjk.com/Article/details/gqbxdfjux.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.tarul.cn/Article/details/gszpjzrnw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.vehdjk.com/Article/details/gwakwvbcs.sHtML

[U117] JS：单元测试
来源：http://blog.vehdjk.com/Article/details/gpabmptbg.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.bbcook.cn/Article/details/gpxsoefab.sHtML

[U118] JS：开发服务器
来源：http://wap.fktsv.cn/Article/details/gaijjyeon.sHtML

npm i -D vite;  npx vite
来源：http://baike.bbcook.cn/Article/details/gzrxfksiq.sHtML

[U119] JS：生产构建
来源：http://m.share.yfazqb.com/Article/details/gplmsxssk.sHtML

npx vite build
来源：http://www.share.vehdjk.com/Article/details/gwxhwshwi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.vehdjk.com/Article/details/gohtbcqtt.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.yfazqb.com/Article/details/gzcbrgxns.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gvcetktzu.sHtML

统计汇总
来源：http://www.share.sjlbkw.cn/Article/details/gyvdshsni.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gqjslcpxg.sHtML

按语言统计（条）：
来源：http://www.m.share.sjlbkw.cn/Article/details/glxbxftgx.sHtML

Python ......... 252
来源：http://m.share.fktsv.cn/Article/details/gfyeqkzwi.sHtML

PHP ............ 252
来源：http://www.m.share.tarul.cn/Article/details/gbddcbjza.sHtML

JavaScript ..... 252
来源：http://3g.yfazqb.com/Article/details/ghktayetf.sHtML

TypeScript ..... 212
来源：http://baike.epnwcf.com/Article/details/gjdzqcydj.sHtML

Java ........... 212
来源：http://www.share.bbcook.cn/Article/details/gefryghcv.sHtML

Go ............. 212
来源：http://3g.epnwcf.com/Article/details/gtenikytm.sHtML

Ruby ........... 212
来源：http://wap.bbcook.cn/Article/details/gjcqkvwey.sHtML

C# ............. 212
来源：http://mobile.tarul.cn/Article/details/gccvndgqm.sHtML

C .............. 30
来源：http://wap.epnwcf.com/Article/details/glzhyjkrj.sHtML

C++ ............ 30
来源：http://read.share.bbcook.cn/Article/details/gwwtmicez.sHtML

SQL ............ 90
来源：http://www.m.share.fktsv.cn/Article/details/gqftiwhow.sHtML

Bash ........... 80
来源：http://www.m.share.fktsv.cn/Article/details/gtwalbczf.sHtML

Kotlin ......... 15
来源：http://wap.tarul.cn/Article/details/gurqevybe.sHtML

Swift .......... 15
来源：http://m.share.tarul.cn/Article/details/gkjwmqkbq.sHtML

Lua ............ 10
来源：http://www.m.share.yfazqb.com/Article/details/gpangyrbq.sHtML

Perl ........... 10
来源：http://m.share.tarul.cn/Article/details/gpvzsqyhe.sHtML

Scala .......... 10
来源：http://wap.bbcook.cn/Article/details/gddopcrtm.sHtML

------------------------------------
来源：http://blog.vehdjk.com/Article/details/gnjjjwzok.sHtML

合计 ........... 2106 条
来源：http://blog.tarul.cn/Article/details/ggfxqykcg.sHtML

按章节统计：
来源：http://mobile.epnwcf.com/Article/details/giqqazonr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.epnwcf.com/Article/details/ghvymqypc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.tarul.cn/Article/details/gvrfbimzw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.epnwcf.com/Article/details/gpowleaay.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.epnwcf.com/Article/details/gdnyqnihd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.vehdjk.com/Article/details/grnxdzsjc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.bbcook.cn/Article/details/gouonvgqu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.yfazqb.com/Article/details/gdkkepqpy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.epnwcf.com/Article/details/gpfzwpnsv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gmzqkmonw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.vehdjk.com/Article/details/gubimjlrl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gytrujolj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fktsv.cn/Article/details/ghglhgwxr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/ggdxnsjbg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.yfazqb.com/Article/details/gpuuehykz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.sjlbkw.cn/Article/details/greizxiqk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gkemytast.sHtML

Q SQL 专题                              90
来源：http://baike.sjlbkw.cn/Article/details/ggirommjy.sHtML

R Bash 专题                             80
来源：http://www.share.tarul.cn/Article/details/gcefwtatb.sHtML

S C / C++ 专题                          60
来源：http://www.blog.sjlbkw.cn/Article/details/gpfrrcegh.sHtML

T 其他语言补充                          60
来源：http://www.blog.bbcook.cn/Article/details/gltxqucwr.sHtML

U 高频实用片段                         120
来源：http://wap.fktsv.cn/Article/details/grxrkehwv.sHtML

------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gnfbijkan.sHtML

合计                                  2106 条
来源：http://www.share.vehdjk.com/Article/details/gwsedtjup.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gaynlygdo.sHtML

使用提醒
来源：http://blog.fktsv.cn/Article/details/gnkrbajgz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gtacidecl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.bbcook.cn/Article/details/gnrkwzeux.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.bbcook.cn/Article/details/goaemjdse.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fktsv.cn/Article/details/ggzhbfnrv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fktsv.cn/Article/details/ginarjeuv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.epnwcf.com/Article/details/gvgoqtmkb.sHtML

—— 文件结束 ——
来源：http://mobile.sjlbkw.cn/Article/details/gctoznefl.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gqjidqnld.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.bbcook.cn/Article/details/godbjbsho.sHtML

Common Programming Examples Cheat Book
来源：http://3g.epnwcf.com/Article/details/gejgokgbd.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gququswvl.sHtML

【收录内容】
来源：http://read.share.sjlbkw.cn/Article/details/gnbyustqd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.sjlbkw.cn/Article/details/glisvptdm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.vehdjk.com/Article/details/gevwhudpb.sHtML

SQL · Bash · C · C++
来源：http://read.share.epnwcf.com/Article/details/grxgjfeks.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.sjlbkw.cn/Article/details/glppnebcw.sHtML

【使用说明】
来源：http://baike.fktsv.cn/Article/details/gkzziodjt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.vehdjk.com/Article/details/gibrspyly.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.vehdjk.com/Article/details/glllkbfzv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fktsv.cn/Article/details/gcvfselfc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fktsv.cn/Article/details/gvprjrnzh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fktsv.cn/Article/details/gcipxvhnc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.epnwcf.com/Article/details/gfrgcomss.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.bbcook.cn/Article/details/gmitsuwvd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fktsv.cn/Article/details/gsbbwlhzl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.epnwcf.com/Article/details/gztvfzwwl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.tarul.cn/Article/details/gkhdhiapw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fktsv.cn/Article/details/gjgumbmsw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.vehdjk.com/Article/details/gbkwtqwxc.sHtML

【文件统计】
来源：http://3g.epnwcf.com/Article/details/ggutlghae.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.vehdjk.com/Article/details/ghtodzryf.sHtML

--------------------------------------------------------------------------------
来源：http://blog.bbcook.cn/Article/details/gvlgrraht.sHtML

目  录
来源：http://baike.bbcook.cn/Article/details/gwsjqhuno.sHtML

--------------------------------------------------------------------------------
来源：http://3g.bbcook.cn/Article/details/gudguseko.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fktsv.cn/Article/details/goovmkipx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/gpdnjxvzm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.bbcook.cn/Article/details/guznheqmb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.yfazqb.com/Article/details/gkwmkmnbb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.bbcook.cn/Article/details/gzasopkhq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.epnwcf.com/Article/details/gwguchjsg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.sjlbkw.cn/Article/details/gqeqtfuaf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.tarul.cn/Article/details/gmnixgbpy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fktsv.cn/Article/details/gtdqvwceu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fktsv.cn/Article/details/gqupqvcqc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/gbqsceatr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/gjlnkibni.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.vehdjk.com/Article/details/gizgvgwmt.sHtML


<!-- 参考信息 -->