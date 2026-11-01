代发 wailian999

[U19] Py：正则替换带回调
来源：http://3g.yfazqb.com/Article/details/godopvdwf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.bbcook.cn/Article/details/gcdwiepsh.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.tarul.cn/Article/details/giycsweks.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.yfazqb.com/Article/details/gdxkmslpk.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.epnwcf.com/Article/details/gjosbsqhv.sHtML

@contextlib.contextmanager
来源：http://www.blog.bbcook.cn/Article/details/gbaomahax.sHtML

[U22] Py：矩阵转置
来源：http://read.share.yfazqb.com/Article/details/gcywqzwnx.sHtML

list(zip(*m))
来源：http://m.share.fktsv.cn/Article/details/gddotyflf.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.epnwcf.com/Article/details/gqhrrafbc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.bbcook.cn/Article/details/gislydfhr.sHtML

[U24] Py：路径操作
来源：http://www.m.share.tarul.cn/Article/details/gvvwbpqmv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.epnwcf.com/Article/details/gjryefmib.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.sjlbkw.cn/Article/details/gzzzxapgp.sHtML

csv.DictReader(f)
来源：http://www.share.fktsv.cn/Article/details/gpolakrex.sHtML

[U26] Py：并发下载
来源：http://www.m.share.vehdjk.com/Article/details/gamyfwrij.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.tarul.cn/Article/details/gsvecfkzz.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.sjlbkw.cn/Article/details/gagggmwwx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.sjlbkw.cn/Article/details/gqsiitzvn.sHtML

[U28] Py：类型别名
来源：http://www.m.share.epnwcf.com/Article/details/gabphecrs.sHtML

UserId = int
来源：http://baike.vehdjk.com/Article/details/gnzlxgoec.sHtML

[U29] Py：属性校验
来源：http://3g.sjlbkw.cn/Article/details/gguebkmzc.sHtML

@property 与 @x.setter 配合
来源：http://read.share.epnwcf.com/Article/details/gffyxpcnx.sHtML

[U30] Py：数据类
来源：http://www.m.share.fktsv.cn/Article/details/gfhgqhknq.sHtML

@dataclass(slots=True)
来源：http://www.m.share.bbcook.cn/Article/details/gfkdgqoof.sHtML

[U31] Py：单测
来源：http://baike.epnwcf.com/Article/details/gojhqsznp.sHtML

python -m pytest -q
来源：http://read.share.vehdjk.com/Article/details/gvbvhkynh.sHtML

[U32] Py：代码格式化
来源：http://3g.sjlbkw.cn/Article/details/ginlnxdwl.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.sjlbkw.cn/Article/details/gnwegyfli.sHtML

[U33] Py：打包发布
来源：http://baike.vehdjk.com/Article/details/gjlppmbrp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fktsv.cn/Article/details/gamslzuiy.sHtML

[U34] Py：判断编码
来源：http://blog.bbcook.cn/Article/details/gkzoszkjh.sHtML

chardet.detect(raw)
来源：http://3g.vehdjk.com/Article/details/gqyeuugyu.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.tarul.cn/Article/details/geetjymtw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.sjlbkw.cn/Article/details/giifmxifs.sHtML

[U36] Py：定时任务
来源：http://m.share.epnwcf.com/Article/details/golvqusuu.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.tarul.cn/Article/details/gdpedlauk.sHtML

[U37] Py：读写 Excel
来源：http://mobile.sjlbkw.cn/Article/details/gmdubprnl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.tarul.cn/Article/details/gtyyrpvvx.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.bbcook.cn/Article/details/gnzqbgnya.sHtML

Path(__file__).resolve().parent
来源：http://baike.fktsv.cn/Article/details/gqjkkeuab.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fktsv.cn/Article/details/gwleffulp.sHtML

sys.stdout.isatty()
来源：http://www.blog.yfazqb.com/Article/details/gxtcojxst.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.bbcook.cn/Article/details/gfriczbih.sHtML

print("err", file=sys.stderr)
来源：http://baike.epnwcf.com/Article/details/grltsnqgj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.yfazqb.com/Article/details/gorfkjgjo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.epnwcf.com/Article/details/gzcsflubn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.yfazqb.com/Article/details/gipisbqsh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.yfazqb.com/Article/details/gbwgefqxt.sHtML

[U43] PHP：声明命名空间
来源：http://wap.tarul.cn/Article/details/gxcpqvhpl.sHtML

namespace App\Http;
来源：http://m.share.epnwcf.com/Article/details/gtnjtvrat.sHtML

[U44] PHP：开启严格类型
来源：http://3g.sjlbkw.cn/Article/details/gexpsthqm.sHtML

declare(strict_types=1);
来源：http://wap.epnwcf.com/Article/details/gzwrvatwx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fktsv.cn/Article/details/grdqrpfjv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/ggrerwxun.sHtML

[U46] PHP：可空类型
来源：http://blog.bbcook.cn/Article/details/gdoemrvkr.sHtML

?string $name = null
来源：http://m.share.fktsv.cn/Article/details/gxrpabkdf.sHtML

[U47] PHP：联合类型
来源：http://read.share.epnwcf.com/Article/details/gjhvpkzle.sHtML

int|string $id
来源：http://3g.vehdjk.com/Article/details/gdiwmlwlg.sHtML

[U48] PHP：纯枚举
来源：http://m.share.bbcook.cn/Article/details/gnkfktdgj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsszikhv.sHtML

[U49] PHP：只读属性
来源：http://m.share.vehdjk.com/Article/details/grampqbeb.sHtML

public readonly string $name
来源：http://www.m.share.bbcook.cn/Article/details/gkfibqhzh.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.sjlbkw.cn/Article/details/gszgxggik.sHtML

public function __construct(private int $id) {}
来源：http://blog.sjlbkw.cn/Article/details/gyyvtkrgr.sHtML

[U51] PHP：数组解构
来源：http://wap.epnwcf.com/Article/details/gmzpcnhwe.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fktsv.cn/Article/details/gbdposxim.sHtML

[U52] PHP：箭头函数
来源：http://mobile.bbcook.cn/Article/details/gsvtviveu.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.tarul.cn/Article/details/gyvyftwcv.sHtML

[U53] PHP：空合并运算符
来源：http://3g.epnwcf.com/Article/details/gwcitmrsq.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.yfazqb.com/Article/details/gixouljds.sHtML

[U54] PHP：空安全调用
来源：http://blog.bbcook.cn/Article/details/gginluenb.sHtML

$obj?->method()
来源：http://3g.sjlbkw.cn/Article/details/ggmwhsllo.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fktsv.cn/Article/details/gkutlaehj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.bbcook.cn/Article/details/ghdxletah.sHtML

[U56] PHP：命名参数
来源：http://read.share.tarul.cn/Article/details/gptfwaihs.sHtML

f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gswbvdupc.sHtML

[U57] PHP：字符串插值
来源：http://blog.fktsv.cn/Article/details/ghqnsdaol.sHtML

"值: {$a}"
来源：http://m.share.fktsv.cn/Article/details/grgabrwsl.sHtML

[U58] PHP：数组三件套
来源：http://www.share.sjlbkw.cn/Article/details/gonnorrjj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.sjlbkw.cn/Article/details/goeymgvjx.sHtML

[U59] PHP：自定义排序
来源：http://mobile.vehdjk.com/Article/details/gkkaptcle.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fktsv.cn/Article/details/gbayrswuj.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.yfazqb.com/Article/details/geqrcvzbq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.bbcook.cn/Article/details/gwjumdyst.sHtML

[U61] PHP：正则
来源：http://blog.epnwcf.com/Article/details/grbsiyghr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.epnwcf.com/Article/details/gchdgovrq.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.vehdjk.com/Article/details/gnudpvsuh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.bbcook.cn/Article/details/grmnpyvia.sHtML

[U63] PHP：文件读写
来源：http://blog.bbcook.cn/Article/details/gwyxlnjnk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fktsv.cn/Article/details/guceqffey.sHtML

[U64] PHP：目录遍历
来源：http://3g.bbcook.cn/Article/details/gqccbdxhc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.epnwcf.com/Article/details/gpwceywsw.sHtML

[U65] PHP：会话
来源：http://3g.sjlbkw.cn/Article/details/gioftcfzx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fktsv.cn/Article/details/gattkwywa.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.epnwcf.com/Article/details/gyzgnvyxh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.tarul.cn/Article/details/gstxbxwhu.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.tarul.cn/Article/details/gzzffnmwz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.tarul.cn/Article/details/gacvozgcn.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.tarul.cn/Article/details/gkthnyskb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.yfazqb.com/Article/details/gmgkeeyzk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fktsv.cn/Article/details/gleuqdaiz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.tarul.cn/Article/details/gpdyiduzc.sHtML

[U70] PHP：PDO 事务
来源：http://baike.yfazqb.com/Article/details/gpwpptcwk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.sjlbkw.cn/Article/details/gycmobqjg.sHtML

[U71] PHP：抛出异常
来源：http://wap.bbcook.cn/Article/details/gykpzjsjc.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.epnwcf.com/Article/details/gjcaqgwfu.sHtML

[U72] PHP：写错误日志
来源：http://mobile.sjlbkw.cn/Article/details/gxhavfupv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.tarul.cn/Article/details/ggpvoudhp.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.yfazqb.com/Article/details/gjtbwwobo.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.vehdjk.com/Article/details/gvzzfcpad.sHtML

[U74] PHP：读取环境变量
来源：http://baike.bbcook.cn/Article/details/gwfoezqwr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.bbcook.cn/Article/details/gaukfxezi.sHtML

[U75] PHP：依赖注入
来源：http://wap.sjlbkw.cn/Article/details/gopjjahha.sHtML

composer require psr/container
来源：http://3g.vehdjk.com/Article/details/gsvnatpcs.sHtML

[U76] PHP：简单路由
来源：http://m.share.bbcook.cn/Article/details/ghqyivuia.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.yfazqb.com/Article/details/gqirvybof.sHtML

[U77] PHP：模板渲染
来源：http://read.share.sjlbkw.cn/Article/details/gdcosohfm.sHtML

composer require twig/twig
来源：http://mobile.vehdjk.com/Article/details/gxlbsfqlx.sHtML

[U78] PHP：单元测试
来源：http://3g.bbcook.cn/Article/details/gtotsivfy.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.tarul.cn/Article/details/grzvlkivz.sHtML

[U79] PHP：静态分析
来源：http://www.share.fktsv.cn/Article/details/gurvpggpu.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fktsv.cn/Article/details/gebjlvyaj.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.epnwcf.com/Article/details/gunozvrsg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.vehdjk.com/Article/details/gyvrkvshf.sHtML

[U81] JS：初始化项目
来源：http://wap.vehdjk.com/Article/details/gwlclwbph.sHtML

npm init -y;  npm i express
来源：http://3g.yfazqb.com/Article/details/gkbgwmueh.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.tarul.cn/Article/details/gpurypeei.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.vehdjk.com/Article/details/gojmtrkwb.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.tarul.cn/Article/details/gxyqueikd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fktsv.cn/Article/details/geadgmipf.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.sjlbkw.cn/Article/details/grxwjgxkp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.tarul.cn/Article/details/gsmbeazdo.sHtML

[U85] JS：可选链
来源：http://www.blog.fktsv.cn/Article/details/gqxucojbw.sHtML

a?.b?.c
来源：http://blog.tarul.cn/Article/details/guwygorgy.sHtML

[U86] JS：空值合并
来源：http://www.share.tarul.cn/Article/details/genuoyxoa.sHtML

a ?? b
来源：http://read.share.vehdjk.com/Article/details/gbmdkksap.sHtML

[U87] JS：解构默认值
来源：http://read.share.bbcook.cn/Article/details/gtyepggrb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzfslauu.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.vehdjk.com/Article/details/gqcflliwo.sHtML

{ ...a, ...b }
来源：http://www.share.tarul.cn/Article/details/gsnubyoex.sHtML

[U89] JS：数组去重
来源：http://3g.sjlbkw.cn/Article/details/groknmrlo.sHtML

[...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/gjnannjqf.sHtML

[U90] JS：数字数组排序
来源：http://read.share.tarul.cn/Article/details/gutvlwlps.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gvteyyhuy.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.sjlbkw.cn/Article/details/gmwsssqwn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.bbcook.cn/Article/details/galqdnhdd.sHtML

[U92] JS：深拷贝
来源：http://read.share.fktsv.cn/Article/details/gahxarewi.sHtML

structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/gfuxlkxzm.sHtML

[U93] JS：模板字符串
来源：http://baike.vehdjk.com/Article/details/gfetyaxxt.sHtML

`共 ${n} 条`
来源：http://read.share.yfazqb.com/Article/details/glinrqwzl.sHtML

[U94] JS：箭头函数
来源：http://mobile.bbcook.cn/Article/details/gnrvqhoyq.sHtML

const double = x => x * 2;
来源：http://3g.vehdjk.com/Article/details/gapsvcxkq.sHtML

[U95] JS：Promise 包装
来源：http://mobile.epnwcf.com/Article/details/gdorsgvjr.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.epnwcf.com/Article/details/gfbysmyxa.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fktsv.cn/Article/details/gxxmmssay.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.sjlbkw.cn/Article/details/gidjpflgf.sHtML

[U97] JS：并发请求
来源：http://read.share.fktsv.cn/Article/details/gnxdffpfa.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gaiyenttm.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.bbcook.cn/Article/details/gsnfwlcxb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.vehdjk.com/Article/details/gvayeythx.sHtML

[U99] JS：事件监听
来源：http://www.m.share.epnwcf.com/Article/details/gwzvppsbb.sHtML

el.addEventListener("click", e => {})
来源：http://wap.vehdjk.com/Article/details/gynwpkpug.sHtML

[U100] JS：DOM 查询
来源：http://wap.bbcook.cn/Article/details/gkyrfnlgf.sHtML

document.querySelector(".item")
来源：http://wap.epnwcf.com/Article/details/gktjeiqqz.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fktsv.cn/Article/details/gxriymvln.sHtML

el.classList.toggle("active")
来源：http://mobile.bbcook.cn/Article/details/gondwgezu.sHtML

[U102] JS：本地存储
来源：http://baike.vehdjk.com/Article/details/gxzlioham.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.sjlbkw.cn/Article/details/gnlmqvhkj.sHtML

[U103] JS：定时器
来源：http://baike.vehdjk.com/Article/details/gwtptuqax.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.bbcook.cn/Article/details/gigwfedob.sHtML

[U104] JS：防抖
来源：http://www.m.share.epnwcf.com/Article/details/gohygtgme.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.vehdjk.com/Article/details/gyfvagxvh.sHtML

[U105] JS：节流
来源：http://baike.fktsv.cn/Article/details/ghrtbubpe.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.epnwcf.com/Article/details/gmullrjgf.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/gpqtvzflw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.bbcook.cn/Article/details/gpmuhyoga.sHtML

[U107] JS：数字千分位
来源：http://read.share.vehdjk.com/Article/details/gcpyfyvlz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.tarul.cn/Article/details/gsudrsffv.sHtML

[U108] JS：随机整数
来源：http://wap.epnwcf.com/Article/details/gnzdodhdy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.bbcook.cn/Article/details/gfrpfcgfm.sHtML

[U109] JS：数组分组
来源：http://read.share.bbcook.cn/Article/details/gkutqckjs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.vehdjk.com/Article/details/glcqgsudy.sHtML

[U110] JS：数组分块
来源：http://www.share.vehdjk.com/Article/details/gcydlvidb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.yfazqb.com/Article/details/gfaujfaew.sHtML

[U111] JS：对象转 Map
来源：http://blog.fktsv.cn/Article/details/ghnwehgto.sHtML

new Map(Object.entries(obj))
来源：http://mobile.sjlbkw.cn/Article/details/gqavduxlk.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.bbcook.cn/Article/details/ginzrmdwi.sHtML

"7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gsqhkbjop.sHtML

[U113] JS：正则替换全部
来源：http://blog.epnwcf.com/Article/details/grzkdzwhv.sHtML

s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gycoejmvm.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fktsv.cn/Article/details/gmltiqlgs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/gafyyvqdp.sHtML

[U115] JS：生成 UUID
来源：http://m.share.yfazqb.com/Article/details/ghsvrdtle.sHtML

crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/ghekchjqr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.yfazqb.com/Article/details/gjcpvznlv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.epnwcf.com/Article/details/gklrawwqc.sHtML

[U117] JS：单元测试
来源：http://wap.tarul.cn/Article/details/gplpkumsg.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.tarul.cn/Article/details/gceymdwgd.sHtML

[U118] JS：开发服务器
来源：http://mobile.bbcook.cn/Article/details/gshnttvnl.sHtML

npm i -D vite;  npx vite
来源：http://mobile.bbcook.cn/Article/details/grhoeapgq.sHtML

[U119] JS：生产构建
来源：http://read.share.vehdjk.com/Article/details/gcfijnxtc.sHtML

npx vite build
来源：http://3g.yfazqb.com/Article/details/gwcxwztap.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.bbcook.cn/Article/details/gumaquzxt.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fktsv.cn/Article/details/gzcbdxmhh.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gvhmptfje.sHtML

统计汇总
来源：http://mobile.tarul.cn/Article/details/goimytxqr.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gdrpvpotw.sHtML

按语言统计（条）：
来源：http://blog.vehdjk.com/Article/details/gbbquvrmq.sHtML

Python ......... 252
来源：http://wap.yfazqb.com/Article/details/gpvupgwmm.sHtML

PHP ............ 252
来源：http://3g.vehdjk.com/Article/details/garajsjge.sHtML

JavaScript ..... 252
来源：http://mobile.vehdjk.com/Article/details/gcdccqcbp.sHtML

TypeScript ..... 212
来源：http://wap.epnwcf.com/Article/details/gqcwlamfo.sHtML

Java ........... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gminshdae.sHtML

Go ............. 212
来源：http://m.share.fktsv.cn/Article/details/gwmskbmha.sHtML

Ruby ........... 212
来源：http://mobile.tarul.cn/Article/details/gfkdwkrun.sHtML

C# ............. 212
来源：http://www.blog.yfazqb.com/Article/details/gyfntfpfi.sHtML

C .............. 30
来源：http://read.share.fktsv.cn/Article/details/glnrjdqse.sHtML

C++ ............ 30
来源：http://www.blog.vehdjk.com/Article/details/geaqyixlo.sHtML

SQL ............ 90
来源：http://mobile.tarul.cn/Article/details/gncasljmw.sHtML

Bash ........... 80
来源：http://www.m.share.sjlbkw.cn/Article/details/giixffgqi.sHtML

Kotlin ......... 15
来源：http://www.share.vehdjk.com/Article/details/gglpnapfi.sHtML

Swift .......... 15
来源：http://baike.fktsv.cn/Article/details/guhkpjeyr.sHtML

Lua ............ 10
来源：http://www.blog.sjlbkw.cn/Article/details/gcvnqnsxh.sHtML

Perl ........... 10
来源：http://www.share.tarul.cn/Article/details/gliebqpxs.sHtML

Scala .......... 10
来源：http://www.m.share.tarul.cn/Article/details/gvblqzcvb.sHtML

------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gdzogcwht.sHtML

合计 ........... 2106 条
来源：http://3g.vehdjk.com/Article/details/glapllqcj.sHtML

按章节统计：
来源：http://www.blog.bbcook.cn/Article/details/gaxooquad.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.bbcook.cn/Article/details/gbbychdfj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.epnwcf.com/Article/details/guvbgrpbj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.bbcook.cn/Article/details/grxckiyiz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.vehdjk.com/Article/details/gdyvwtecy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fktsv.cn/Article/details/gjwjxqlyy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.sjlbkw.cn/Article/details/gtxzfyiew.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.yfazqb.com/Article/details/gatlfjwej.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.yfazqb.com/Article/details/gjpfvzcag.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/gtupksbqn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.sjlbkw.cn/Article/details/ggyjjpdxe.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gqkmfmeaw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gfvaxijqn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.tarul.cn/Article/details/gjqxknxdb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.sjlbkw.cn/Article/details/gyheqqmbf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.bbcook.cn/Article/details/gzwyohnoh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/ghdvxrfyb.sHtML

Q SQL 专题                              90
来源：http://mobile.yfazqb.com/Article/details/gyityuyys.sHtML

R Bash 专题                             80
来源：http://read.share.bbcook.cn/Article/details/gfmefxqdm.sHtML

S C / C++ 专题                          60
来源：http://www.share.tarul.cn/Article/details/ggvblxrml.sHtML

T 其他语言补充                          60
来源：http://www.share.tarul.cn/Article/details/glilitkqf.sHtML

U 高频实用片段                         120
来源：http://m.share.bbcook.cn/Article/details/gfzklngeq.sHtML

------------------------------------
来源：http://3g.bbcook.cn/Article/details/gzaeguunf.sHtML

合计                                  2106 条
来源：http://3g.bbcook.cn/Article/details/ggsohdauq.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/gytjxevnt.sHtML

使用提醒
来源：http://3g.sjlbkw.cn/Article/details/gfaslubxx.sHtML

--------------------------------------------------------------------------------
来源：http://blog.bbcook.cn/Article/details/gftinuzfx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.tarul.cn/Article/details/grmvjkhxt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.epnwcf.com/Article/details/glmqmxtyi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fktsv.cn/Article/details/getpgpmpe.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.epnwcf.com/Article/details/gtlyvsxdx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.yfazqb.com/Article/details/gmaxinbby.sHtML

—— 文件结束 ——
来源：http://www.m.share.fktsv.cn/Article/details/gkhrbykpf.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gkdkrogjc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.vehdjk.com/Article/details/gnqbtogqx.sHtML

Common Programming Examples Cheat Book
来源：http://blog.sjlbkw.cn/Article/details/guvvlskho.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gdmrkiuhs.sHtML

【收录内容】
来源：http://read.share.fktsv.cn/Article/details/ggqkbsyed.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.yfazqb.com/Article/details/gdcbxmtny.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.bbcook.cn/Article/details/gyeontfns.sHtML

SQL · Bash · C · C++
来源：http://3g.epnwcf.com/Article/details/gixenxfld.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.tarul.cn/Article/details/gbcskhexh.sHtML

【使用说明】
来源：http://wap.bbcook.cn/Article/details/gucctjrjr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fktsv.cn/Article/details/getmjixoz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fktsv.cn/Article/details/ggmewkfsu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.sjlbkw.cn/Article/details/glcysrpoq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.vehdjk.com/Article/details/gfjlslkif.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.tarul.cn/Article/details/gdgglojzx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.tarul.cn/Article/details/gdcpxynhy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.sjlbkw.cn/Article/details/gpasisbwx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.bbcook.cn/Article/details/ggzkrvrdw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.tarul.cn/Article/details/gqpegynrk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.sjlbkw.cn/Article/details/gdpdtcjxl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.tarul.cn/Article/details/gitweyrux.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.bbcook.cn/Article/details/gldvbopmy.sHtML

【文件统计】
来源：http://www.m.share.vehdjk.com/Article/details/ghxucmwvr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.bbcook.cn/Article/details/gqvvnkqls.sHtML

--------------------------------------------------------------------------------
来源：http://3g.bbcook.cn/Article/details/gmlupzhnh.sHtML

目  录
来源：http://read.share.sjlbkw.cn/Article/details/gtdhjuduv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.vehdjk.com/Article/details/gsabslzlx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.epnwcf.com/Article/details/glfwndptx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.bbcook.cn/Article/details/gvbelgqyl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.vehdjk.com/Article/details/gsvmwkgst.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fktsv.cn/Article/details/gnezsueuk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.bbcook.cn/Article/details/gkrmqkoqv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.bbcook.cn/Article/details/goqkvekco.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.tarul.cn/Article/details/gcvsugaua.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.yfazqb.com/Article/details/gkewakswp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/gylinokgc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.epnwcf.com/Article/details/gzdqcnozb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.vehdjk.com/Article/details/gwdvuneje.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.sjlbkw.cn/Article/details/gwqmvphsi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/grcfogprx.sHtML


<!-- 参考信息 -->