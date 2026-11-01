代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.tarul.cn/Article/details/gfkjojbcp.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gwgyeskxn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.epnwcf.com/Article/details/gpjhdpfiy.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gcbkicdzv.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.tarul.cn/Article/details/gtmztudps.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.tarul.cn/Article/details/gzvqbdosg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fktsv.cn/Article/details/gvhbhxkzw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gntnffiml.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.vehdjk.com/Article/details/gqtlhivbh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.tarul.cn/Article/details/gtftfbyth.sHtML

[U04] Py：变量调试打印
来源：http://baike.epnwcf.com/Article/details/ghkgfzqex.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.tarul.cn/Article/details/gepwrezjr.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.vehdjk.com/Article/details/ghtvpqzux.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.tarul.cn/Article/details/grcypmeqc.sHtML

[U06] Py：合并两个字典
来源：http://m.share.bbcook.cn/Article/details/grtvjeidu.sHtML

{**a, **b}
来源：http://mobile.vehdjk.com/Article/details/gzrpgpveg.sHtML

[U07] Py：反转字典键值
来源：http://mobile.bbcook.cn/Article/details/gthxlwfed.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.bbcook.cn/Article/details/ggrviebhl.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.sjlbkw.cn/Article/details/gnqikzkph.sHtML

[y for x in nested for y in x]
来源：http://3g.tarul.cn/Article/details/gmueqkpiu.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.bbcook.cn/Article/details/guypmgfvj.sHtML

max(d, key=d.get)
来源：http://blog.vehdjk.com/Article/details/gsopoqqqq.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.yfazqb.com/Article/details/gfqngaszs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.sjlbkw.cn/Article/details/ghvsnzoog.sHtML

[U11] Py：生成器表达式
来源：http://m.share.yfazqb.com/Article/details/gyapqabcg.sHtML

(x * 2 for x in arr)
来源：http://wap.epnwcf.com/Article/details/gmcxejxzw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.vehdjk.com/Article/details/gqceqrnjw.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.tarul.cn/Article/details/glckhqzhl.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.vehdjk.com/Article/details/gdbnzyjcr.sHtML

deque(maxlen=10)
来源：http://blog.epnwcf.com/Article/details/gzjvquepy.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.bbcook.cn/Article/details/givpttuqb.sHtML

defaultdict(list)
来源：http://read.share.tarul.cn/Article/details/ggewnnime.sHtML

[U15] Py：高精度计时
来源：http://read.share.vehdjk.com/Article/details/gpftdyroa.sHtML

t = time.perf_counter()
来源：http://3g.tarul.cn/Article/details/gkgshadws.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.epnwcf.com/Article/details/gkyzkzjhk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.epnwcf.com/Article/details/gyypckidv.sHtML

[U17] Py：初始化日志
来源：http://m.share.sjlbkw.cn/Article/details/gpoujodti.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.yfazqb.com/Article/details/gywbksqhx.sHtML

[U18] Py：预编译正则
来源：http://mobile.epnwcf.com/Article/details/grhatikfl.sHtML

pat = re.compile(r"\d+")
来源：http://3g.bbcook.cn/Article/details/gpggeqziw.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.sjlbkw.cn/Article/details/gpnmwrane.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.yfazqb.com/Article/details/gpstdwavm.sHtML

[U20] Py：缓存函数结果
来源：http://3g.epnwcf.com/Article/details/gupkiyedl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fktsv.cn/Article/details/gtcuxcwdt.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.sjlbkw.cn/Article/details/glqailsdl.sHtML

@contextlib.contextmanager
来源：http://3g.tarul.cn/Article/details/gjibsxynj.sHtML

[U22] Py：矩阵转置
来源：http://blog.yfazqb.com/Article/details/guoyvedny.sHtML

list(zip(*m))
来源：http://mobile.sjlbkw.cn/Article/details/gklzbkfub.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.tarul.cn/Article/details/giyhvcxuv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fktsv.cn/Article/details/ghorqwvps.sHtML

[U24] Py：路径操作
来源：http://www.blog.fktsv.cn/Article/details/gpweldmax.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.tarul.cn/Article/details/gzmlxikhd.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.yfazqb.com/Article/details/gtwfthsuy.sHtML

csv.DictReader(f)
来源：http://mobile.bbcook.cn/Article/details/gegpvlfmi.sHtML

[U26] Py：并发下载
来源：http://baike.vehdjk.com/Article/details/gptqhhggq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.vehdjk.com/Article/details/gmfoedrkp.sHtML

[U27] Py：异步 HTTP
来源：http://blog.tarul.cn/Article/details/gtsqnzshf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.tarul.cn/Article/details/gahocdiak.sHtML

[U28] Py：类型别名
来源：http://read.share.sjlbkw.cn/Article/details/gazpezsvz.sHtML

UserId = int
来源：http://m.share.fktsv.cn/Article/details/gsajxvnrz.sHtML

[U29] Py：属性校验
来源：http://mobile.epnwcf.com/Article/details/gozlmmntg.sHtML

@property 与 @x.setter 配合
来源：http://m.share.yfazqb.com/Article/details/gmyogehwy.sHtML

[U30] Py：数据类
来源：http://blog.epnwcf.com/Article/details/gwqgbmgut.sHtML

@dataclass(slots=True)
来源：http://3g.tarul.cn/Article/details/gcmpieykc.sHtML

[U31] Py：单测
来源：http://www.m.share.tarul.cn/Article/details/gggosbmmr.sHtML

python -m pytest -q
来源：http://3g.sjlbkw.cn/Article/details/gknsfkyyn.sHtML

[U32] Py：代码格式化
来源：http://www.share.sjlbkw.cn/Article/details/gtodswqcw.sHtML

ruff format . && ruff check --fix .
来源：http://wap.bbcook.cn/Article/details/gvbrkpkrm.sHtML

[U33] Py：打包发布
来源：http://www.share.fktsv.cn/Article/details/gysgwbhac.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.bbcook.cn/Article/details/gcqsbnsmc.sHtML

[U34] Py：判断编码
来源：http://www.share.fktsv.cn/Article/details/gkoioxshx.sHtML

chardet.detect(raw)
来源：http://mobile.sjlbkw.cn/Article/details/gyoakqcbx.sHtML

[U35] Py：发送邮件
来源：http://3g.yfazqb.com/Article/details/geatcvghf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.bbcook.cn/Article/details/gemjbsdyq.sHtML

[U36] Py：定时任务
来源：http://www.blog.sjlbkw.cn/Article/details/gopllchln.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.sjlbkw.cn/Article/details/gvtethjls.sHtML

[U37] Py：读写 Excel
来源：http://3g.bbcook.cn/Article/details/gvdqfheps.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.vehdjk.com/Article/details/glqcuffpy.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.tarul.cn/Article/details/gjjhbjolk.sHtML

Path(__file__).resolve().parent
来源：http://m.share.yfazqb.com/Article/details/gikkihdyq.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.epnwcf.com/Article/details/guvuylsjn.sHtML

sys.stdout.isatty()
来源：http://www.m.share.epnwcf.com/Article/details/gbvmvihjz.sHtML

[U40] Py：打印到标准错误
来源：http://wap.sjlbkw.cn/Article/details/gjytltvle.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.sjlbkw.cn/Article/details/gsuwvlrrc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.bbcook.cn/Article/details/gdbmsfbqr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.vehdjk.com/Article/details/gkjikjgzq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.vehdjk.com/Article/details/gjcumfech.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.vehdjk.com/Article/details/gtzamyddm.sHtML

[U43] PHP：声明命名空间
来源：http://baike.sjlbkw.cn/Article/details/grlvthyps.sHtML

namespace App\Http;
来源：http://baike.bbcook.cn/Article/details/gjswjprgq.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.bbcook.cn/Article/details/gwshykeqm.sHtML

declare(strict_types=1);
来源：http://blog.epnwcf.com/Article/details/gwtfheimr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.tarul.cn/Article/details/gngdyyobb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gwsowgfol.sHtML

[U46] PHP：可空类型
来源：http://m.share.vehdjk.com/Article/details/gdqnqgahz.sHtML

?string $name = null
来源：http://m.share.epnwcf.com/Article/details/gjwwmbkrb.sHtML

[U47] PHP：联合类型
来源：http://wap.tarul.cn/Article/details/gepisjede.sHtML

int|string $id
来源：http://baike.vehdjk.com/Article/details/gmxsbauiv.sHtML

[U48] PHP：纯枚举
来源：http://blog.yfazqb.com/Article/details/gxjawcgwv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.sjlbkw.cn/Article/details/gmrasicpo.sHtML

[U49] PHP：只读属性
来源：http://blog.fktsv.cn/Article/details/gewdelwpi.sHtML

public readonly string $name
来源：http://m.share.vehdjk.com/Article/details/gobmwxzbo.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.epnwcf.com/Article/details/ghbuhddqq.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.yfazqb.com/Article/details/gfiqmbavb.sHtML

[U51] PHP：数组解构
来源：http://blog.sjlbkw.cn/Article/details/gasggwrge.sHtML

[$a, $b] = $arr;
来源：http://read.share.vehdjk.com/Article/details/gyypngyqk.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fktsv.cn/Article/details/gtrsuysuj.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.tarul.cn/Article/details/ghquhyess.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.bbcook.cn/Article/details/ghqhjmtax.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.yfazqb.com/Article/details/gfjewlymm.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.yfazqb.com/Article/details/gahvkpnqy.sHtML

$obj?->method()
来源：http://www.share.fktsv.cn/Article/details/gdsihckrx.sHtML

[U55] PHP：match 表达式
来源：http://wap.tarul.cn/Article/details/gtaedwiic.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.sjlbkw.cn/Article/details/gjlixuqtl.sHtML

[U56] PHP：命名参数
来源：http://www.blog.bbcook.cn/Article/details/gqszzbykn.sHtML

f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gzlvrqotk.sHtML

[U57] PHP：字符串插值
来源：http://blog.bbcook.cn/Article/details/geohcyiww.sHtML

"值: {$a}"
来源：http://3g.sjlbkw.cn/Article/details/godwrgoki.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fktsv.cn/Article/details/gtjxiqipj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.vehdjk.com/Article/details/ghxpzzgpm.sHtML

[U59] PHP：自定义排序
来源：http://mobile.yfazqb.com/Article/details/gxiffmaui.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.vehdjk.com/Article/details/gfyuwzgxk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.epnwcf.com/Article/details/gqlwxjwvt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fktsv.cn/Article/details/grexzlahu.sHtML

[U61] PHP：正则
来源：http://read.share.vehdjk.com/Article/details/gfjwiyulz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.tarul.cn/Article/details/gdwhxxhly.sHtML

[U62] PHP：日期对象
来源：http://read.share.bbcook.cn/Article/details/gnzoxsosp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.sjlbkw.cn/Article/details/ghmaytrkf.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.tarul.cn/Article/details/gsewwgveb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.yfazqb.com/Article/details/gxuqavdps.sHtML

[U64] PHP：目录遍历
来源：http://wap.tarul.cn/Article/details/gfknqniiv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fktsv.cn/Article/details/grrggveqo.sHtML

[U65] PHP：会话
来源：http://baike.tarul.cn/Article/details/gffoxmxdx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.yfazqb.com/Article/details/gitgcxwih.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fktsv.cn/Article/details/gvbpibxua.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.vehdjk.com/Article/details/gllgfnmhi.sHtML

[U67] PHP：处理文件上传
来源：http://blog.yfazqb.com/Article/details/gadffposl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fktsv.cn/Article/details/gozubbjww.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.vehdjk.com/Article/details/gdvehjfda.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.sjlbkw.cn/Article/details/gnqtdqjua.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fktsv.cn/Article/details/gsyjbrfof.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fktsv.cn/Article/details/glxctydwe.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.epnwcf.com/Article/details/ghkaoqwaz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.epnwcf.com/Article/details/giyglfsyf.sHtML

[U71] PHP：抛出异常
来源：http://mobile.tarul.cn/Article/details/gjyvfbjlj.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.tarul.cn/Article/details/gkyaeqziu.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fktsv.cn/Article/details/gxtmrutlz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.tarul.cn/Article/details/gkiscxjxz.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.bbcook.cn/Article/details/gyfybnyio.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.vehdjk.com/Article/details/gqjqpcffd.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.epnwcf.com/Article/details/gyxqziyhs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fktsv.cn/Article/details/grmradkyr.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.vehdjk.com/Article/details/gtkpefyes.sHtML

composer require psr/container
来源：http://blog.sjlbkw.cn/Article/details/gltazsmcg.sHtML

[U76] PHP：简单路由
来源：http://3g.epnwcf.com/Article/details/gocyzfpgc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.epnwcf.com/Article/details/gudlltqjd.sHtML

[U77] PHP：模板渲染
来源：http://wap.yfazqb.com/Article/details/grvbjwiuf.sHtML

composer require twig/twig
来源：http://read.share.epnwcf.com/Article/details/gqgblipsa.sHtML

[U78] PHP：单元测试
来源：http://baike.sjlbkw.cn/Article/details/gchgwojay.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.epnwcf.com/Article/details/guhsfzply.sHtML

[U79] PHP：静态分析
来源：http://3g.vehdjk.com/Article/details/gzkimlmrk.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fktsv.cn/Article/details/gquhnkayg.sHtML

[U80] PHP：代码规范修复
来源：http://blog.tarul.cn/Article/details/goflmxfyz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.sjlbkw.cn/Article/details/gnzamwccc.sHtML

[U81] JS：初始化项目
来源：http://read.share.yfazqb.com/Article/details/gswswgwuq.sHtML

npm init -y;  npm i express
来源：http://read.share.tarul.cn/Article/details/gtwiopekn.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.vehdjk.com/Article/details/gpvrseylk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.bbcook.cn/Article/details/glhcwjnaz.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.vehdjk.com/Article/details/gbkgdljnc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.sjlbkw.cn/Article/details/gobvihjcm.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.sjlbkw.cn/Article/details/ggohvmbas.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.yfazqb.com/Article/details/gqswqyfrn.sHtML

[U85] JS：可选链
来源：http://www.blog.sjlbkw.cn/Article/details/glorycfkw.sHtML

a?.b?.c
来源：http://read.share.sjlbkw.cn/Article/details/gkrcxhqci.sHtML

[U86] JS：空值合并
来源：http://m.share.sjlbkw.cn/Article/details/guickhmnw.sHtML

a ?? b
来源：http://blog.yfazqb.com/Article/details/gywmiydbf.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fktsv.cn/Article/details/gvxfrjzpi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.tarul.cn/Article/details/gbaoblyuc.sHtML

[U88] JS：对象展开合并
来源：http://3g.tarul.cn/Article/details/guxfmdjbf.sHtML

{ ...a, ...b }
来源：http://3g.bbcook.cn/Article/details/gwadxflrf.sHtML

[U89] JS：数组去重
来源：http://3g.sjlbkw.cn/Article/details/ggnjxewnq.sHtML

[...new Set(arr)]
来源：http://blog.vehdjk.com/Article/details/ggalrdakp.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gxexcypod.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gldkrpifd.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.tarul.cn/Article/details/gyxywkjzr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.yfazqb.com/Article/details/gaajbvtlk.sHtML

[U92] JS：深拷贝
来源：http://www.blog.vehdjk.com/Article/details/ggwcwpdsn.sHtML

structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gkzmlnznx.sHtML

[U93] JS：模板字符串
来源：http://m.share.sjlbkw.cn/Article/details/gzhhgwscq.sHtML

`共 ${n} 条`
来源：http://baike.tarul.cn/Article/details/gtosvshhf.sHtML

[U94] JS：箭头函数
来源：http://mobile.epnwcf.com/Article/details/gftawhvew.sHtML

const double = x => x * 2;
来源：http://www.blog.epnwcf.com/Article/details/gbcibehtj.sHtML

[U95] JS：Promise 包装
来源：http://read.share.yfazqb.com/Article/details/gtdierigh.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fktsv.cn/Article/details/gvjbvcqba.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.epnwcf.com/Article/details/gvfzpvjtv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/gmballrxt.sHtML

[U97] JS：并发请求
来源：http://www.blog.bbcook.cn/Article/details/gxxomwpsq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gfrgiggag.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.vehdjk.com/Article/details/gcechxabf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.yfazqb.com/Article/details/gtyjmkjnk.sHtML

[U99] JS：事件监听
来源：http://mobile.sjlbkw.cn/Article/details/glfiuzorj.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.yfazqb.com/Article/details/gxpyfvzwt.sHtML

[U100] JS：DOM 查询
来源：http://www.share.vehdjk.com/Article/details/gkqclwpxk.sHtML

document.querySelector(".item")
来源：http://mobile.epnwcf.com/Article/details/givamwrma.sHtML

[U101] JS：classList 操作
来源：http://3g.sjlbkw.cn/Article/details/gwyvmmvnt.sHtML

el.classList.toggle("active")
来源：http://www.share.tarul.cn/Article/details/gfgbxbogi.sHtML

[U102] JS：本地存储
来源：http://read.share.sjlbkw.cn/Article/details/gcqoyifvz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.bbcook.cn/Article/details/gqwcpumyw.sHtML

[U103] JS：定时器
来源：http://3g.yfazqb.com/Article/details/gcblfephl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.epnwcf.com/Article/details/gcmhaxyhx.sHtML

[U104] JS：防抖
来源：http://3g.vehdjk.com/Article/details/grhzazpyj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.bbcook.cn/Article/details/gijvihykk.sHtML

[U105] JS：节流
来源：http://wap.yfazqb.com/Article/details/gkjzoglkj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.tarul.cn/Article/details/gdndblppi.sHtML

[U106] JS：日期格式化
来源：http://blog.vehdjk.com/Article/details/gxqemxjmc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fktsv.cn/Article/details/giemydwvp.sHtML

[U107] JS：数字千分位
来源：http://wap.bbcook.cn/Article/details/gczjvpulu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.bbcook.cn/Article/details/gtahanvcs.sHtML

[U108] JS：随机整数
来源：http://mobile.epnwcf.com/Article/details/glsoztjmw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.vehdjk.com/Article/details/gverxzfar.sHtML

[U109] JS：数组分组
来源：http://read.share.epnwcf.com/Article/details/gkypxvnkq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.sjlbkw.cn/Article/details/gpayybgsx.sHtML

[U110] JS：数组分块
来源：http://mobile.tarul.cn/Article/details/gvawomtut.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.bbcook.cn/Article/details/gekgwbhrg.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/goqyvromm.sHtML

new Map(Object.entries(obj))
来源：http://m.share.yfazqb.com/Article/details/gwqrynsvw.sHtML

[U112] JS：字符串补位
来源：http://wap.tarul.cn/Article/details/gphfevmcy.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsicmwym.sHtML

[U113] JS：正则替换全部
来源：http://mobile.bbcook.cn/Article/details/glxhgstzl.sHtML

s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gvxqaaran.sHtML

[U114] JS：JSON 深比较
来源：http://blog.bbcook.cn/Article/details/gtmsvzaiz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/gkigfwvjc.sHtML

[U115] JS：生成 UUID
来源：http://m.share.epnwcf.com/Article/details/giukdmmhg.sHtML

crypto.randomUUID()
来源：http://wap.yfazqb.com/Article/details/gxoisghim.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.bbcook.cn/Article/details/gnmqnejds.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.vehdjk.com/Article/details/gmdgqypeh.sHtML

[U117] JS：单元测试
来源：http://read.share.fktsv.cn/Article/details/gaioewpqz.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fktsv.cn/Article/details/gkjutymin.sHtML

[U118] JS：开发服务器
来源：http://blog.vehdjk.com/Article/details/gikpnrvkk.sHtML

npm i -D vite;  npx vite
来源：http://baike.yfazqb.com/Article/details/gnoirthkq.sHtML

[U119] JS：生产构建
来源：http://blog.bbcook.cn/Article/details/gtcxcbomi.sHtML

npx vite build
来源：http://3g.tarul.cn/Article/details/gcwtlhpqw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.sjlbkw.cn/Article/details/gsisiktie.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fktsv.cn/Article/details/gjjpdggbe.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gznmthzhe.sHtML

统计汇总
来源：http://www.blog.tarul.cn/Article/details/grkfdxpnt.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gvvhskkij.sHtML

按语言统计（条）：
来源：http://www.blog.vehdjk.com/Article/details/ggthwqnap.sHtML

Python ......... 252
来源：http://baike.yfazqb.com/Article/details/gyjffugau.sHtML

PHP ............ 252
来源：http://read.share.yfazqb.com/Article/details/giyypjidz.sHtML

JavaScript ..... 252
来源：http://www.share.bbcook.cn/Article/details/gjdnvxndm.sHtML

TypeScript ..... 212
来源：http://wap.epnwcf.com/Article/details/glepaegnj.sHtML

Java ........... 212
来源：http://m.share.tarul.cn/Article/details/gmmekhdnv.sHtML

Go ............. 212
来源：http://m.share.sjlbkw.cn/Article/details/gxiythmze.sHtML

Ruby ........... 212
来源：http://blog.yfazqb.com/Article/details/gsbskprlt.sHtML

C# ............. 212
来源：http://mobile.yfazqb.com/Article/details/gimpbwowv.sHtML

C .............. 30
来源：http://blog.fktsv.cn/Article/details/gcnjzfaad.sHtML

C++ ............ 30
来源：http://m.share.yfazqb.com/Article/details/gpfywfill.sHtML

SQL ............ 90
来源：http://m.share.yfazqb.com/Article/details/gcjdkixsc.sHtML

Bash ........... 80
来源：http://www.share.vehdjk.com/Article/details/gjpiyqepq.sHtML

Kotlin ......... 15
来源：http://www.m.share.vehdjk.com/Article/details/glyrqnebo.sHtML

Swift .......... 15
来源：http://www.m.share.fktsv.cn/Article/details/gxeidbwfk.sHtML

Lua ............ 10
来源：http://baike.vehdjk.com/Article/details/greqfcnso.sHtML

Perl ........... 10
来源：http://wap.vehdjk.com/Article/details/ggihjqvcf.sHtML

Scala .......... 10
来源：http://m.share.yfazqb.com/Article/details/gkwjkvcpu.sHtML

------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gmnyvqeno.sHtML

合计 ........... 2106 条
来源：http://mobile.epnwcf.com/Article/details/gystqghet.sHtML

按章节统计：
来源：http://read.share.tarul.cn/Article/details/gjiderwtr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.yfazqb.com/Article/details/gqwzwrgek.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.bbcook.cn/Article/details/gsgqyeowi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.sjlbkw.cn/Article/details/gyagwgbud.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.sjlbkw.cn/Article/details/glsuekkgk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.vehdjk.com/Article/details/gkbqbnzzw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fktsv.cn/Article/details/gmllicsfn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fktsv.cn/Article/details/gphumseha.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.epnwcf.com/Article/details/gsczlyybp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/ggcmgljcv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.bbcook.cn/Article/details/gsjziyoqs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gslssclga.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.sjlbkw.cn/Article/details/gwaiffnxz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/gncrtvygo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.yfazqb.com/Article/details/gfxtvelcj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.bbcook.cn/Article/details/gtwbhsjfd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/gdqwusjwm.sHtML

Q SQL 专题                              90
来源：http://read.share.vehdjk.com/Article/details/gkssnkbxt.sHtML

R Bash 专题                             80
来源：http://mobile.fktsv.cn/Article/details/gnakkszoq.sHtML

S C / C++ 专题                          60
来源：http://www.share.fktsv.cn/Article/details/gxmibyiqd.sHtML

T 其他语言补充                          60
来源：http://wap.epnwcf.com/Article/details/gvhifemwy.sHtML

U 高频实用片段                         120
来源：http://www.blog.sjlbkw.cn/Article/details/ghwuwrqkg.sHtML

------------------------------------
来源：http://read.share.vehdjk.com/Article/details/grlphecnv.sHtML

合计                                  2106 条
来源：http://www.m.share.bbcook.cn/Article/details/gbrtkoinh.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gogcecjgu.sHtML

使用提醒
来源：http://blog.tarul.cn/Article/details/gmbrrtivn.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gntqszkbv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.sjlbkw.cn/Article/details/gctuxsybt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.vehdjk.com/Article/details/gdzozwegf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.bbcook.cn/Article/details/gksjyqgrx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.yfazqb.com/Article/details/gbhjobpzp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.epnwcf.com/Article/details/gbrjgehbk.sHtML

—— 文件结束 ——
来源：http://m.share.yfazqb.com/Article/details/gyauehmjn.sHtML


<!-- 参考信息 -->