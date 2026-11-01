代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://blog.vehdjk.com/Article/details/gladqrrja.sHtML

@contextlib.contextmanager
来源：http://www.share.epnwcf.com/Article/details/gusoexdps.sHtML

[U22] Py：矩阵转置
来源：http://blog.fktsv.cn/Article/details/gmxylruqa.sHtML

list(zip(*m))
来源：http://blog.yfazqb.com/Article/details/gkwqyrhvq.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fktsv.cn/Article/details/gbvkmghxm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.sjlbkw.cn/Article/details/gsegthwwx.sHtML

[U24] Py：路径操作
来源：http://www.share.epnwcf.com/Article/details/ghzgzfmxw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.bbcook.cn/Article/details/guseydkvf.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.epnwcf.com/Article/details/gqzxujfjb.sHtML

csv.DictReader(f)
来源：http://baike.tarul.cn/Article/details/ghpdfnuwy.sHtML

[U26] Py：并发下载
来源：http://blog.bbcook.cn/Article/details/gjczrjepz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtoeypep.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.tarul.cn/Article/details/ghpxtotua.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.vehdjk.com/Article/details/gcecufaug.sHtML

[U28] Py：类型别名
来源：http://3g.bbcook.cn/Article/details/guiseyqqe.sHtML

UserId = int
来源：http://blog.sjlbkw.cn/Article/details/gmfzhzztb.sHtML

[U29] Py：属性校验
来源：http://www.share.bbcook.cn/Article/details/gpsfevkuz.sHtML

@property 与 @x.setter 配合
来源：http://m.share.bbcook.cn/Article/details/gxorzsccv.sHtML

[U30] Py：数据类
来源：http://mobile.sjlbkw.cn/Article/details/gxwwdhfwq.sHtML

@dataclass(slots=True)
来源：http://m.share.yfazqb.com/Article/details/gqysiedvs.sHtML

[U31] Py：单测
来源：http://www.share.tarul.cn/Article/details/gnqtzuuuz.sHtML

python -m pytest -q
来源：http://3g.epnwcf.com/Article/details/gqtlnhden.sHtML

[U32] Py：代码格式化
来源：http://baike.fktsv.cn/Article/details/gxphulhbj.sHtML

ruff format . && ruff check --fix .
来源：http://wap.yfazqb.com/Article/details/gmgmfvvpj.sHtML

[U33] Py：打包发布
来源：http://mobile.tarul.cn/Article/details/gflvkwprh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.yfazqb.com/Article/details/gvcbypgyv.sHtML

[U34] Py：判断编码
来源：http://www.blog.yfazqb.com/Article/details/gvfxnonfv.sHtML

chardet.detect(raw)
来源：http://blog.fktsv.cn/Article/details/gyefcpspm.sHtML

[U35] Py：发送邮件
来源：http://blog.tarul.cn/Article/details/gyvchiddw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.yfazqb.com/Article/details/gylqfddew.sHtML

[U36] Py：定时任务
来源：http://read.share.bbcook.cn/Article/details/gelvvceff.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.tarul.cn/Article/details/gzlcrtpxw.sHtML

[U37] Py：读写 Excel
来源：http://read.share.sjlbkw.cn/Article/details/gtxmxxflq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.sjlbkw.cn/Article/details/gamwlgwyc.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.sjlbkw.cn/Article/details/gqoaerlck.sHtML

Path(__file__).resolve().parent
来源：http://read.share.epnwcf.com/Article/details/gxobytnir.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.bbcook.cn/Article/details/ghsxeionp.sHtML

sys.stdout.isatty()
来源：http://wap.vehdjk.com/Article/details/gqmhnednw.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fktsv.cn/Article/details/gppngvviq.sHtML

print("err", file=sys.stderr)
来源：http://blog.fktsv.cn/Article/details/gtlpnbxuu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fktsv.cn/Article/details/ghsbfprxn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.tarul.cn/Article/details/gykcqjhcg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.yfazqb.com/Article/details/ggwjhwikr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.vehdjk.com/Article/details/gegwmqxcp.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.tarul.cn/Article/details/gaqaufgop.sHtML

namespace App\Http;
来源：http://mobile.tarul.cn/Article/details/gtqdzheol.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fktsv.cn/Article/details/goidbywjq.sHtML

declare(strict_types=1);
来源：http://wap.sjlbkw.cn/Article/details/gmlqjxamt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.sjlbkw.cn/Article/details/gtspxtktj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/ggwxbpsow.sHtML

[U46] PHP：可空类型
来源：http://read.share.sjlbkw.cn/Article/details/gbfmenyhc.sHtML

?string $name = null
来源：http://www.m.share.sjlbkw.cn/Article/details/gpryclwqr.sHtML

[U47] PHP：联合类型
来源：http://read.share.vehdjk.com/Article/details/gvdlszrfv.sHtML

int|string $id
来源：http://m.share.epnwcf.com/Article/details/gnvmzthno.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fktsv.cn/Article/details/glmowqhmx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.yfazqb.com/Article/details/gpruuphcr.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.sjlbkw.cn/Article/details/giafdoubt.sHtML

public readonly string $name
来源：http://m.share.epnwcf.com/Article/details/gzzhsfqbb.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.sjlbkw.cn/Article/details/gcnynjjyt.sHtML

public function __construct(private int $id) {}
来源：http://m.share.tarul.cn/Article/details/gnubuutjz.sHtML

[U51] PHP：数组解构
来源：http://3g.epnwcf.com/Article/details/gscsofzfu.sHtML

[$a, $b] = $arr;
来源：http://wap.vehdjk.com/Article/details/glozenqhj.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.vehdjk.com/Article/details/gytaqyrtl.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fktsv.cn/Article/details/gjsbqtcvx.sHtML

[U53] PHP：空合并运算符
来源：http://baike.bbcook.cn/Article/details/gonuclknl.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.yfazqb.com/Article/details/gjvcvziwh.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvrrmpmt.sHtML

$obj?->method()
来源：http://www.m.share.bbcook.cn/Article/details/gwecbdpuu.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.vehdjk.com/Article/details/gnceiqmxg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.vehdjk.com/Article/details/ghhjwvjym.sHtML

[U56] PHP：命名参数
来源：http://3g.epnwcf.com/Article/details/garzvjvri.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsggbwlk.sHtML

[U57] PHP：字符串插值
来源：http://www.share.yfazqb.com/Article/details/gasqflucy.sHtML

"值: {$a}"
来源：http://blog.epnwcf.com/Article/details/gynrtupuu.sHtML

[U58] PHP：数组三件套
来源：http://read.share.yfazqb.com/Article/details/gqfrnnqsn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.epnwcf.com/Article/details/gytdgcjhu.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gjanqdfti.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fktsv.cn/Article/details/gfrjalmnu.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.bbcook.cn/Article/details/grqtoxehy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.epnwcf.com/Article/details/gszupbvbm.sHtML

[U61] PHP：正则
来源：http://read.share.vehdjk.com/Article/details/gbgzcxgqz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fktsv.cn/Article/details/guexnxrlw.sHtML

[U62] PHP：日期对象
来源：http://read.share.yfazqb.com/Article/details/gjyzblhci.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.bbcook.cn/Article/details/gnlzgfeck.sHtML

[U63] PHP：文件读写
来源：http://3g.bbcook.cn/Article/details/gtpxkketv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.yfazqb.com/Article/details/gxpelqqqu.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.epnwcf.com/Article/details/giluloryj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.sjlbkw.cn/Article/details/gitoeihsy.sHtML

[U65] PHP：会话
来源：http://www.share.vehdjk.com/Article/details/gwjguwozk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.epnwcf.com/Article/details/gcducvgbz.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.bbcook.cn/Article/details/gitzsqswj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.vehdjk.com/Article/details/gdxdxhnjn.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.bbcook.cn/Article/details/gvzqwjheu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.vehdjk.com/Article/details/giufjsmzz.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.vehdjk.com/Article/details/gusttdxvo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.bbcook.cn/Article/details/gotdikxmc.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.epnwcf.com/Article/details/gozxgjjot.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.bbcook.cn/Article/details/gckuxelmf.sHtML

[U70] PHP：PDO 事务
来源：http://blog.tarul.cn/Article/details/gccivfwrw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.sjlbkw.cn/Article/details/gsanesdep.sHtML

[U71] PHP：抛出异常
来源：http://mobile.vehdjk.com/Article/details/gnhdqwgsd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.yfazqb.com/Article/details/gowrupfjo.sHtML

[U72] PHP：写错误日志
来源：http://baike.vehdjk.com/Article/details/gisdfttml.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fktsv.cn/Article/details/gfwlhfxhr.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fktsv.cn/Article/details/grlexmloc.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.vehdjk.com/Article/details/gntjnfksd.sHtML

[U74] PHP：读取环境变量
来源：http://3g.vehdjk.com/Article/details/gaqbkrqqa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.tarul.cn/Article/details/gkkjgynlo.sHtML

[U75] PHP：依赖注入
来源：http://3g.tarul.cn/Article/details/gqkatpysg.sHtML

composer require psr/container
来源：http://wap.bbcook.cn/Article/details/ghdybnrbf.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.tarul.cn/Article/details/geqpssixq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.bbcook.cn/Article/details/gijrvnwpx.sHtML

[U77] PHP：模板渲染
来源：http://3g.vehdjk.com/Article/details/ggwebbwhz.sHtML

composer require twig/twig
来源：http://read.share.sjlbkw.cn/Article/details/gjvflyscs.sHtML

[U78] PHP：单元测试
来源：http://wap.sjlbkw.cn/Article/details/gbdzcgrth.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.epnwcf.com/Article/details/gswgkfkqp.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.vehdjk.com/Article/details/gyayvikfz.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.bbcook.cn/Article/details/gbmedgxob.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fktsv.cn/Article/details/gknpiptsx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.epnwcf.com/Article/details/gmykwbprk.sHtML

[U81] JS：初始化项目
来源：http://wap.bbcook.cn/Article/details/gismltini.sHtML

npm init -y;  npm i express
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbjtgpsg.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.bbcook.cn/Article/details/gguglvmkh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.sjlbkw.cn/Article/details/gieobodxe.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.tarul.cn/Article/details/gartujlfy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.epnwcf.com/Article/details/gawqcqptu.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.tarul.cn/Article/details/gdcfhijcp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.bbcook.cn/Article/details/gkipdcpkk.sHtML

[U85] JS：可选链
来源：http://wap.epnwcf.com/Article/details/gplfcwdgr.sHtML

a?.b?.c
来源：http://3g.tarul.cn/Article/details/gmlknjnuu.sHtML

[U86] JS：空值合并
来源：http://read.share.epnwcf.com/Article/details/ghmmcpuow.sHtML

a ?? b
来源：http://m.share.vehdjk.com/Article/details/gwobskqon.sHtML

[U87] JS：解构默认值
来源：http://blog.tarul.cn/Article/details/gwetesxmq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.yfazqb.com/Article/details/gyhzbezjf.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.tarul.cn/Article/details/gsrckolua.sHtML

{ ...a, ...b }
来源：http://www.blog.epnwcf.com/Article/details/gjbhlaodf.sHtML

[U89] JS：数组去重
来源：http://mobile.yfazqb.com/Article/details/gujbafqbc.sHtML

[...new Set(arr)]
来源：http://m.share.epnwcf.com/Article/details/ggeyehrfh.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.vehdjk.com/Article/details/gtkscgxum.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gzftzhdoz.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.epnwcf.com/Article/details/gynjhhedc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fktsv.cn/Article/details/gxyiebxrf.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gzkldmopy.sHtML

structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/ggdvxwnjo.sHtML

[U93] JS：模板字符串
来源：http://read.share.vehdjk.com/Article/details/gxnsnbwui.sHtML

`共 ${n} 条`
来源：http://3g.epnwcf.com/Article/details/gpkgkbwqd.sHtML

[U94] JS：箭头函数
来源：http://3g.fktsv.cn/Article/details/gcsvjeeyg.sHtML

const double = x => x * 2;
来源：http://m.share.sjlbkw.cn/Article/details/gcfnjtusx.sHtML

[U95] JS：Promise 包装
来源：http://blog.tarul.cn/Article/details/guqklzasm.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.bbcook.cn/Article/details/gbmrtxoix.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.tarul.cn/Article/details/gyufaoipu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.sjlbkw.cn/Article/details/gaufzlreo.sHtML

[U97] JS：并发请求
来源：http://read.share.epnwcf.com/Article/details/grywmbkqy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/gjxayekux.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fktsv.cn/Article/details/gzhaokknw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.yfazqb.com/Article/details/geqonncoq.sHtML

[U99] JS：事件监听
来源：http://blog.bbcook.cn/Article/details/gtnswbufy.sHtML

el.addEventListener("click", e => {})
来源：http://3g.vehdjk.com/Article/details/grxwnfbyu.sHtML

[U100] JS：DOM 查询
来源：http://mobile.sjlbkw.cn/Article/details/gebxqjepa.sHtML

document.querySelector(".item")
来源：http://www.share.sjlbkw.cn/Article/details/grwdmcfbt.sHtML

[U101] JS：classList 操作
来源：http://3g.bbcook.cn/Article/details/gzhsboovf.sHtML

el.classList.toggle("active")
来源：http://baike.sjlbkw.cn/Article/details/gguexpjhz.sHtML

[U102] JS：本地存储
来源：http://baike.epnwcf.com/Article/details/gcpfjwnip.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.sjlbkw.cn/Article/details/gxmmmsxnz.sHtML

[U103] JS：定时器
来源：http://www.m.share.epnwcf.com/Article/details/grbkpqvek.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.bbcook.cn/Article/details/gwmnbeybf.sHtML

[U104] JS：防抖
来源：http://baike.tarul.cn/Article/details/gyunwjund.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gflodznxw.sHtML

[U105] JS：节流
来源：http://www.m.share.tarul.cn/Article/details/ggxhcudts.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fktsv.cn/Article/details/gefhdlujv.sHtML

[U106] JS：日期格式化
来源：http://3g.fktsv.cn/Article/details/gxjppcpxv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.tarul.cn/Article/details/gpqrtqszu.sHtML

[U107] JS：数字千分位
来源：http://www.share.tarul.cn/Article/details/guyfbilym.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fktsv.cn/Article/details/giragaqhe.sHtML

[U108] JS：随机整数
来源：http://3g.yfazqb.com/Article/details/gkemfqqve.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.bbcook.cn/Article/details/gaptksgrl.sHtML

[U109] JS：数组分组
来源：http://m.share.bbcook.cn/Article/details/gzlithmsm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.yfazqb.com/Article/details/gxzujlgdd.sHtML

[U110] JS：数组分块
来源：http://wap.tarul.cn/Article/details/gcygyrzde.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.vehdjk.com/Article/details/geqbenblt.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.yfazqb.com/Article/details/gkijqgzyu.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.yfazqb.com/Article/details/gahhqqxwq.sHtML

[U112] JS：字符串补位
来源：http://3g.yfazqb.com/Article/details/grdmfcmxd.sHtML

"7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/gnyqeyrjo.sHtML

[U113] JS：正则替换全部
来源：http://blog.sjlbkw.cn/Article/details/gglvhmkpk.sHtML

s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/goikisngm.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.bbcook.cn/Article/details/gwoargtao.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.yfazqb.com/Article/details/gqxlwvyui.sHtML

[U115] JS：生成 UUID
来源：http://wap.yfazqb.com/Article/details/gmchbjqon.sHtML

crypto.randomUUID()
来源：http://www.m.share.fktsv.cn/Article/details/gmdxvqpus.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.bbcook.cn/Article/details/gcsqatvun.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.sjlbkw.cn/Article/details/galhprjsr.sHtML

[U117] JS：单元测试
来源：http://baike.vehdjk.com/Article/details/gxelrmhkc.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fktsv.cn/Article/details/gouaswybq.sHtML

[U118] JS：开发服务器
来源：http://www.blog.bbcook.cn/Article/details/gauvpcqwp.sHtML

npm i -D vite;  npx vite
来源：http://m.share.vehdjk.com/Article/details/ghgifptem.sHtML

[U119] JS：生产构建
来源：http://3g.epnwcf.com/Article/details/gwetaqpul.sHtML

npx vite build
来源：http://blog.vehdjk.com/Article/details/gyikszzxy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.yfazqb.com/Article/details/gviyuqgrd.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.bbcook.cn/Article/details/gmkhazgbp.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gjxzzaecj.sHtML

统计汇总
来源：http://www.m.share.yfazqb.com/Article/details/gfawpgfoi.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/geczmednn.sHtML

按语言统计（条）：
来源：http://read.share.yfazqb.com/Article/details/gihljgsks.sHtML

Python ......... 252
来源：http://read.share.sjlbkw.cn/Article/details/gntrhhggr.sHtML

PHP ............ 252
来源：http://m.share.fktsv.cn/Article/details/gakuywdwg.sHtML

JavaScript ..... 252
来源：http://mobile.sjlbkw.cn/Article/details/gedkaioso.sHtML

TypeScript ..... 212
来源：http://www.blog.yfazqb.com/Article/details/gzjojzews.sHtML

Java ........... 212
来源：http://baike.yfazqb.com/Article/details/gkuvinfat.sHtML

Go ............. 212
来源：http://blog.tarul.cn/Article/details/grnpghqng.sHtML

Ruby ........... 212
来源：http://read.share.epnwcf.com/Article/details/gbelrysgy.sHtML

C# ............. 212
来源：http://blog.bbcook.cn/Article/details/gosxcjpss.sHtML

C .............. 30
来源：http://wap.sjlbkw.cn/Article/details/gdbppsdcc.sHtML

C++ ............ 30
来源：http://mobile.fktsv.cn/Article/details/gcezrykut.sHtML

SQL ............ 90
来源：http://read.share.bbcook.cn/Article/details/gaefbyurz.sHtML

Bash ........... 80
来源：http://www.m.share.yfazqb.com/Article/details/glimaeyak.sHtML

Kotlin ......... 15
来源：http://baike.epnwcf.com/Article/details/gcqeecjum.sHtML

Swift .......... 15
来源：http://www.share.bbcook.cn/Article/details/gsbhcuhco.sHtML

Lua ............ 10
来源：http://www.m.share.yfazqb.com/Article/details/gagzonuph.sHtML

Perl ........... 10
来源：http://3g.sjlbkw.cn/Article/details/gqurpdicj.sHtML

Scala .......... 10
来源：http://wap.sjlbkw.cn/Article/details/giwozfrus.sHtML

------------------------------------
来源：http://3g.yfazqb.com/Article/details/gbwpcnxmf.sHtML

合计 ........... 2106 条
来源：http://read.share.tarul.cn/Article/details/gxltwfajw.sHtML

按章节统计：
来源：http://3g.bbcook.cn/Article/details/gifhfzelo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.yfazqb.com/Article/details/gzajghcck.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fktsv.cn/Article/details/gkakxlqny.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.epnwcf.com/Article/details/gucwdjzja.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.vehdjk.com/Article/details/gsunghyzb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.sjlbkw.cn/Article/details/gakcoazpp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.tarul.cn/Article/details/ggpmiulgv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gmdaqgges.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.bbcook.cn/Article/details/gigkzbbyi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gfbwjxphi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.yfazqb.com/Article/details/glfylgkho.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gvvaqeuop.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gbfoiymzu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gdruiddhs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.epnwcf.com/Article/details/gjdzviqvo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fktsv.cn/Article/details/giydiurbn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gypqoqnoo.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fktsv.cn/Article/details/gikfueztv.sHtML

R Bash 专题                             80
来源：http://m.share.tarul.cn/Article/details/gwbygpdbj.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.epnwcf.com/Article/details/gaosisrmv.sHtML

T 其他语言补充                          60
来源：http://mobile.vehdjk.com/Article/details/gfxsyfcqz.sHtML

U 高频实用片段                         120
来源：http://www.blog.vehdjk.com/Article/details/gwtnqhpdq.sHtML

------------------------------------
来源：http://read.share.tarul.cn/Article/details/gvghkyajz.sHtML

合计                                  2106 条
来源：http://read.share.fktsv.cn/Article/details/gxproktxg.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/guquntith.sHtML

使用提醒
来源：http://www.blog.bbcook.cn/Article/details/ggyhddugv.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.vehdjk.com/Article/details/gsbbgybkr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.sjlbkw.cn/Article/details/gymaiftpc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.bbcook.cn/Article/details/gnmzcqxbn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.sjlbkw.cn/Article/details/gvapcaqng.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.bbcook.cn/Article/details/guntoslbj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.bbcook.cn/Article/details/grkiadqol.sHtML

—— 文件结束 ——
来源：http://blog.yfazqb.com/Article/details/glkoorjay.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gazjjirhe.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.yfazqb.com/Article/details/ghxbphoin.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fktsv.cn/Article/details/gthmpklou.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gmvrkkwpr.sHtML

【收录内容】
来源：http://mobile.sjlbkw.cn/Article/details/givqukpdd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.tarul.cn/Article/details/gixopdbfz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.bbcook.cn/Article/details/ghhdazstq.sHtML

SQL · Bash · C · C++
来源：http://3g.vehdjk.com/Article/details/gdqmzrokn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.yfazqb.com/Article/details/gxypiedho.sHtML

【使用说明】
来源：http://m.share.vehdjk.com/Article/details/gaazeyufm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.sjlbkw.cn/Article/details/gdlyuffri.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.sjlbkw.cn/Article/details/grtyewewg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.vehdjk.com/Article/details/gauwbdemw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.yfazqb.com/Article/details/gojkfggek.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.bbcook.cn/Article/details/ghzmdvhip.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.bbcook.cn/Article/details/gchajgamb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.vehdjk.com/Article/details/gjlsisbzh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fktsv.cn/Article/details/grmdkgsbi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fktsv.cn/Article/details/grwvvjbym.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.tarul.cn/Article/details/gforcuuwd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.vehdjk.com/Article/details/gactavavj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.epnwcf.com/Article/details/gyvwipiqs.sHtML

【文件统计】
来源：http://wap.bbcook.cn/Article/details/gwwessyhi.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fktsv.cn/Article/details/gmqfmmkbc.sHtML

--------------------------------------------------------------------------------
来源：http://3g.bbcook.cn/Article/details/ghdqrzuuu.sHtML

目  录
来源：http://baike.tarul.cn/Article/details/gbgnmkvpm.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/gkcxnogvz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.vehdjk.com/Article/details/gdvyhnkbj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxeneccn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.bbcook.cn/Article/details/gcufgpmnu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.bbcook.cn/Article/details/gzljhlqti.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.yfazqb.com/Article/details/ghtvynyfq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.yfazqb.com/Article/details/gwxtfchxi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fktsv.cn/Article/details/gpoiiuxpw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.bbcook.cn/Article/details/gsdqihnau.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gphithvuj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.vehdjk.com/Article/details/gztvybnjv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fktsv.cn/Article/details/gojulzuog.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/gadcjypun.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.bbcook.cn/Article/details/goqfmpngf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fktsv.cn/Article/details/getlcliie.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fktsv.cn/Article/details/ggswspylt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.bbcook.cn/Article/details/gkzaobizh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.tarul.cn/Article/details/gexabubcs.sHtML


<!-- 参考信息 -->