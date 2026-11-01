代发 wailian999

[U03] Py：加载 .env 配置
来源：http://blog.epnwcf.com/Article/details/gmcusjqzk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.bbcook.cn/Article/details/gtamrzayw.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.yfazqb.com/Article/details/gpedghjyn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.epnwcf.com/Article/details/guueqxgmi.sHtML

[U05] Py：列表去重且保序
来源：http://baike.tarul.cn/Article/details/goqmziboe.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.yfazqb.com/Article/details/ggviyqius.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.tarul.cn/Article/details/guqiwenkr.sHtML

{**a, **b}
来源：http://www.blog.vehdjk.com/Article/details/gqiawjpyq.sHtML

[U07] Py：反转字典键值
来源：http://blog.vehdjk.com/Article/details/gkcqisprx.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.bbcook.cn/Article/details/gjhohdmbr.sHtML

[U08] Py：展平二维列表
来源：http://baike.bbcook.cn/Article/details/glcsaqtnp.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.yfazqb.com/Article/details/giuhxeqnv.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.tarul.cn/Article/details/gijepycqc.sHtML

max(d, key=d.get)
来源：http://www.blog.yfazqb.com/Article/details/gitvhceto.sHtML

[U10] Py：按值排序字典
来源：http://wap.yfazqb.com/Article/details/ghrbspgoz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.tarul.cn/Article/details/gvynzgxij.sHtML

[U11] Py：生成器表达式
来源：http://3g.fktsv.cn/Article/details/gjjcmdyrl.sHtML

(x * 2 for x in arr)
来源：http://wap.tarul.cn/Article/details/gehnykxre.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.sjlbkw.cn/Article/details/gbbqmghbl.sHtML

Counter(arr).most_common(3)
来源：http://baike.vehdjk.com/Article/details/ggedxcvgh.sHtML

[U13] Py：固定长度队列
来源：http://wap.bbcook.cn/Article/details/gplrlrrrr.sHtML

deque(maxlen=10)
来源：http://mobile.yfazqb.com/Article/details/gcvpoczpu.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fktsv.cn/Article/details/glsluhvbx.sHtML

defaultdict(list)
来源：http://www.m.share.bbcook.cn/Article/details/gcxyakzai.sHtML

[U15] Py：高精度计时
来源：http://blog.fktsv.cn/Article/details/gcjphyetp.sHtML

t = time.perf_counter()
来源：http://blog.tarul.cn/Article/details/ggqtxcvbj.sHtML

[U16] Py：命令行参数解析
来源：http://3g.bbcook.cn/Article/details/grxirbzbk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.yfazqb.com/Article/details/gnimxffcu.sHtML

[U17] Py：初始化日志
来源：http://read.share.yfazqb.com/Article/details/gqqeaokva.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fktsv.cn/Article/details/gvpzqoifc.sHtML

[U18] Py：预编译正则
来源：http://read.share.epnwcf.com/Article/details/gejaweaws.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.sjlbkw.cn/Article/details/gtmoqlhig.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.yfazqb.com/Article/details/gacagxzvp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.tarul.cn/Article/details/gdjpylhtq.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.yfazqb.com/Article/details/gzqryeltz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fktsv.cn/Article/details/gkpeghptd.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.bbcook.cn/Article/details/gfvrmytlw.sHtML

@contextlib.contextmanager
来源：http://baike.bbcook.cn/Article/details/gpnwjmtcw.sHtML

[U22] Py：矩阵转置
来源：http://www.share.sjlbkw.cn/Article/details/gjawqvnna.sHtML

list(zip(*m))
来源：http://baike.vehdjk.com/Article/details/gyewvrxmj.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.vehdjk.com/Article/details/gugjhsgpt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.vehdjk.com/Article/details/gmfpevgrp.sHtML

[U24] Py：路径操作
来源：http://m.share.yfazqb.com/Article/details/gzgremepc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/gqtsxdkux.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.sjlbkw.cn/Article/details/gfarfpfax.sHtML

csv.DictReader(f)
来源：http://3g.epnwcf.com/Article/details/gfkbvsvxp.sHtML

[U26] Py：并发下载
来源：http://wap.fktsv.cn/Article/details/ghbdvfonm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.yfazqb.com/Article/details/gammsxjne.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.epnwcf.com/Article/details/ggjpwzbvh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.sjlbkw.cn/Article/details/gvflfqinu.sHtML

[U28] Py：类型别名
来源：http://blog.bbcook.cn/Article/details/genylpoqr.sHtML

UserId = int
来源：http://www.blog.tarul.cn/Article/details/gblthxkmg.sHtML

[U29] Py：属性校验
来源：http://m.share.epnwcf.com/Article/details/gwonkrwpg.sHtML

@property 与 @x.setter 配合
来源：http://www.share.vehdjk.com/Article/details/gewadspjt.sHtML

[U30] Py：数据类
来源：http://mobile.yfazqb.com/Article/details/gkvqsmdfv.sHtML

@dataclass(slots=True)
来源：http://m.share.yfazqb.com/Article/details/gphkdvytu.sHtML

[U31] Py：单测
来源：http://www.m.share.vehdjk.com/Article/details/gnzvhevrn.sHtML

python -m pytest -q
来源：http://read.share.yfazqb.com/Article/details/gjeornroe.sHtML

[U32] Py：代码格式化
来源：http://blog.tarul.cn/Article/details/gdtxnraap.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.sjlbkw.cn/Article/details/gqgixirob.sHtML

[U33] Py：打包发布
来源：http://blog.bbcook.cn/Article/details/ggtuyncwv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.sjlbkw.cn/Article/details/grrxeqmqr.sHtML

[U34] Py：判断编码
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqmxmuko.sHtML

chardet.detect(raw)
来源：http://3g.yfazqb.com/Article/details/gxnrqshks.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.vehdjk.com/Article/details/gwyrcwgvl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.vehdjk.com/Article/details/gnlzvcqmp.sHtML

[U36] Py：定时任务
来源：http://mobile.tarul.cn/Article/details/gknayekoq.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.yfazqb.com/Article/details/grjhgwzhy.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fktsv.cn/Article/details/gvekzyvss.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.tarul.cn/Article/details/gvtlkkfyx.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.epnwcf.com/Article/details/gocbcpehw.sHtML

Path(__file__).resolve().parent
来源：http://m.share.vehdjk.com/Article/details/gzlgyzzds.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.bbcook.cn/Article/details/ggsoupnld.sHtML

sys.stdout.isatty()
来源：http://www.m.share.epnwcf.com/Article/details/gtsgxrcjt.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.bbcook.cn/Article/details/guriktlhr.sHtML

print("err", file=sys.stderr)
来源：http://www.share.epnwcf.com/Article/details/gxzkkkkfy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fktsv.cn/Article/details/gkuvgtgkp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.sjlbkw.cn/Article/details/ghtgguxdg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fktsv.cn/Article/details/gkxqanxdy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.epnwcf.com/Article/details/gyitmkrtk.sHtML

[U43] PHP：声明命名空间
来源：http://wap.bbcook.cn/Article/details/gauntkcia.sHtML

namespace App\Http;
来源：http://baike.sjlbkw.cn/Article/details/ggdkphupj.sHtML

[U44] PHP：开启严格类型
来源：http://wap.epnwcf.com/Article/details/gqjcusthk.sHtML

declare(strict_types=1);
来源：http://www.blog.tarul.cn/Article/details/ghfilsusk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.epnwcf.com/Article/details/grvxlgrwq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjyhkhsqw.sHtML

[U46] PHP：可空类型
来源：http://read.share.epnwcf.com/Article/details/gtxjkfgzj.sHtML

?string $name = null
来源：http://3g.epnwcf.com/Article/details/gpgcyjsij.sHtML

[U47] PHP：联合类型
来源：http://read.share.sjlbkw.cn/Article/details/gwcwdsvcg.sHtML

int|string $id
来源：http://www.share.epnwcf.com/Article/details/gliauekcv.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fktsv.cn/Article/details/glpcxfcmx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.tarul.cn/Article/details/gwlgcpmdy.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.vehdjk.com/Article/details/gkqudnbfh.sHtML

public readonly string $name
来源：http://m.share.epnwcf.com/Article/details/gkktsbpip.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.epnwcf.com/Article/details/goxdzpxim.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.yfazqb.com/Article/details/gdfouujoa.sHtML

[U51] PHP：数组解构
来源：http://read.share.fktsv.cn/Article/details/gkhlnkdmd.sHtML

[$a, $b] = $arr;
来源：http://read.share.epnwcf.com/Article/details/glnvpvczc.sHtML

[U52] PHP：箭头函数
来源：http://www.share.sjlbkw.cn/Article/details/gmuvfghag.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.vehdjk.com/Article/details/gtxxkuges.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.epnwcf.com/Article/details/gehjlamva.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.vehdjk.com/Article/details/gcakqzpaa.sHtML

[U54] PHP：空安全调用
来源：http://m.share.tarul.cn/Article/details/ghtydejon.sHtML

$obj?->method()
来源：http://blog.tarul.cn/Article/details/gmcsqpytl.sHtML

[U55] PHP：match 表达式
来源：http://mobile.tarul.cn/Article/details/gswldhkio.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.sjlbkw.cn/Article/details/gkbckkrkr.sHtML

[U56] PHP：命名参数
来源：http://blog.epnwcf.com/Article/details/gtnwwujjj.sHtML

f(a: 1, b: 2)
来源：http://baike.tarul.cn/Article/details/goiacuxtn.sHtML

[U57] PHP：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gwgbbknrz.sHtML

"值: {$a}"
来源：http://blog.vehdjk.com/Article/details/gwafxkibr.sHtML

[U58] PHP：数组三件套
来源：http://3g.fktsv.cn/Article/details/gqminllct.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.bbcook.cn/Article/details/grihyojkt.sHtML

[U59] PHP：自定义排序
来源：http://m.share.bbcook.cn/Article/details/gdprhsdae.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.yfazqb.com/Article/details/gvbmirmtc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fktsv.cn/Article/details/gxshtwwxa.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.epnwcf.com/Article/details/gxgexhmcg.sHtML

[U61] PHP：正则
来源：http://mobile.yfazqb.com/Article/details/gpuqgfrzl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gfcoktrmp.sHtML

[U62] PHP：日期对象
来源：http://baike.epnwcf.com/Article/details/gpjpprtju.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fktsv.cn/Article/details/grjmvnqup.sHtML

[U63] PHP：文件读写
来源：http://blog.bbcook.cn/Article/details/geqgnxlcj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fktsv.cn/Article/details/gwmymsqgq.sHtML

[U64] PHP：目录遍历
来源：http://mobile.tarul.cn/Article/details/gcbseahpq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.bbcook.cn/Article/details/gfvjnctth.sHtML

[U65] PHP：会话
来源：http://read.share.vehdjk.com/Article/details/gvjdwlfwz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gbndypind.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.tarul.cn/Article/details/gqdycldbd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.sjlbkw.cn/Article/details/gemoojpif.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.tarul.cn/Article/details/ghvfezrob.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.epnwcf.com/Article/details/gsfmfgwrj.sHtML

[U68] PHP：PDO 连接
来源：http://wap.yfazqb.com/Article/details/gngsqwheg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.epnwcf.com/Article/details/gtomiinui.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.bbcook.cn/Article/details/glitjjqaa.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.tarul.cn/Article/details/gqabiilwp.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmzkojjo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.bbcook.cn/Article/details/gtighjaax.sHtML

[U71] PHP：抛出异常
来源：http://3g.yfazqb.com/Article/details/gkmamrpde.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.bbcook.cn/Article/details/gffsigiim.sHtML

[U72] PHP：写错误日志
来源：http://www.share.tarul.cn/Article/details/ggkhlobeo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fktsv.cn/Article/details/gbsnogzgq.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fktsv.cn/Article/details/gqkaabceg.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.epnwcf.com/Article/details/goiaskgra.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fktsv.cn/Article/details/gbvofkjgo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fktsv.cn/Article/details/gdekzagby.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.vehdjk.com/Article/details/glbwkwylw.sHtML

composer require psr/container
来源：http://read.share.tarul.cn/Article/details/galavjrxx.sHtML

[U76] PHP：简单路由
来源：http://m.share.yfazqb.com/Article/details/gexpkomfy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fktsv.cn/Article/details/golyuvqmc.sHtML

[U77] PHP：模板渲染
来源：http://m.share.epnwcf.com/Article/details/gkymryvxe.sHtML

composer require twig/twig
来源：http://mobile.sjlbkw.cn/Article/details/gsfdakhxt.sHtML

[U78] PHP：单元测试
来源：http://read.share.sjlbkw.cn/Article/details/gtrextgfc.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.vehdjk.com/Article/details/gpykizrbq.sHtML

[U79] PHP：静态分析
来源：http://wap.sjlbkw.cn/Article/details/ghsjelcvq.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.sjlbkw.cn/Article/details/gmunyqwhn.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.vehdjk.com/Article/details/gnvpowfot.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.vehdjk.com/Article/details/gndzvhrds.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fktsv.cn/Article/details/ghfioosyv.sHtML

npm init -y;  npm i express
来源：http://m.share.epnwcf.com/Article/details/gzrldeypf.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.bbcook.cn/Article/details/gdojzcvdn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fktsv.cn/Article/details/gitldpito.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.tarul.cn/Article/details/gmooczhll.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.sjlbkw.cn/Article/details/govbytxzw.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.yfazqb.com/Article/details/gyzvmhlxt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.bbcook.cn/Article/details/glegsqcxe.sHtML

[U85] JS：可选链
来源：http://www.blog.sjlbkw.cn/Article/details/gtcngryym.sHtML

a?.b?.c
来源：http://3g.yfazqb.com/Article/details/gserazpmt.sHtML

[U86] JS：空值合并
来源：http://m.share.tarul.cn/Article/details/gdsaimole.sHtML

a ?? b
来源：http://www.blog.yfazqb.com/Article/details/gqazprycy.sHtML

[U87] JS：解构默认值
来源：http://mobile.epnwcf.com/Article/details/glsafyolt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.sjlbkw.cn/Article/details/gkcryeuuq.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fktsv.cn/Article/details/glcvxiamw.sHtML

{ ...a, ...b }
来源：http://m.share.epnwcf.com/Article/details/gnttxtwba.sHtML

[U89] JS：数组去重
来源：http://www.blog.sjlbkw.cn/Article/details/gylckpjuy.sHtML

[...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/gwaonbywx.sHtML

[U90] JS：数字数组排序
来源：http://blog.yfazqb.com/Article/details/gooihxacg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/gldbdmwvh.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fktsv.cn/Article/details/gahnzssot.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.epnwcf.com/Article/details/gogjmcjwb.sHtML

[U92] JS：深拷贝
来源：http://mobile.epnwcf.com/Article/details/ghdusswnm.sHtML

structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gytpmkdbk.sHtML

[U93] JS：模板字符串
来源：http://read.share.fktsv.cn/Article/details/gdyagwniq.sHtML

`共 ${n} 条`
来源：http://www.m.share.epnwcf.com/Article/details/gzjllhyct.sHtML

[U94] JS：箭头函数
来源：http://www.blog.sjlbkw.cn/Article/details/gqdmczuis.sHtML

const double = x => x * 2;
来源：http://blog.fktsv.cn/Article/details/gxzuiubci.sHtML

[U95] JS：Promise 包装
来源：http://mobile.bbcook.cn/Article/details/gkgbexyad.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.epnwcf.com/Article/details/gpzaiqlpr.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fktsv.cn/Article/details/gywwwfxhi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/glekjpvuw.sHtML

[U97] JS：并发请求
来源：http://www.m.share.epnwcf.com/Article/details/gyqevxvfn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/gvchsgrtz.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gmogfzpsi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.bbcook.cn/Article/details/gyajwqsmx.sHtML

[U99] JS：事件监听
来源：http://mobile.vehdjk.com/Article/details/gnsjxmtxv.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.yfazqb.com/Article/details/gupzfsbhi.sHtML

[U100] JS：DOM 查询
来源：http://3g.tarul.cn/Article/details/gimmwhbhp.sHtML

document.querySelector(".item")
来源：http://www.m.share.bbcook.cn/Article/details/grgviebon.sHtML

[U101] JS：classList 操作
来源：http://www.share.fktsv.cn/Article/details/gehzkhhan.sHtML

el.classList.toggle("active")
来源：http://www.blog.yfazqb.com/Article/details/gzqcocfym.sHtML

[U102] JS：本地存储
来源：http://www.share.vehdjk.com/Article/details/gjegtoclk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.sjlbkw.cn/Article/details/gfavqlncj.sHtML

[U103] JS：定时器
来源：http://www.share.vehdjk.com/Article/details/gsxsghfkt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.yfazqb.com/Article/details/gitvqzpea.sHtML

[U104] JS：防抖
来源：http://mobile.bbcook.cn/Article/details/gnqfeerzf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/gxqqtpyap.sHtML

[U105] JS：节流
来源：http://baike.yfazqb.com/Article/details/gubkwinei.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fktsv.cn/Article/details/gutkmxvhf.sHtML

[U106] JS：日期格式化
来源：http://wap.fktsv.cn/Article/details/gofpvrhat.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.epnwcf.com/Article/details/ghnqtywly.sHtML

[U107] JS：数字千分位
来源：http://www.share.vehdjk.com/Article/details/gvjlzbrxv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.sjlbkw.cn/Article/details/gsomowvii.sHtML

[U108] JS：随机整数
来源：http://read.share.sjlbkw.cn/Article/details/gintuaqia.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.vehdjk.com/Article/details/gmstfleoq.sHtML

[U109] JS：数组分组
来源：http://3g.epnwcf.com/Article/details/gffcsswpe.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fktsv.cn/Article/details/gzccpjvaq.sHtML

[U110] JS：数组分块
来源：http://3g.fktsv.cn/Article/details/gkeucbyvs.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.vehdjk.com/Article/details/gwjnucisc.sHtML

[U111] JS：对象转 Map
来源：http://wap.bbcook.cn/Article/details/gkdanwuhw.sHtML

new Map(Object.entries(obj))
来源：http://www.share.bbcook.cn/Article/details/giuyinrse.sHtML

[U112] JS：字符串补位
来源：http://mobile.epnwcf.com/Article/details/gzxwjrcmf.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gserpijst.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.yfazqb.com/Article/details/ghrormguy.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gqegbsjva.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.tarul.cn/Article/details/gehutcixi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/gfwwilvrq.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.yfazqb.com/Article/details/gohzsmcvy.sHtML

crypto.randomUUID()
来源：http://3g.epnwcf.com/Article/details/gbhiqbcqh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.tarul.cn/Article/details/gbvyzokjp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.bbcook.cn/Article/details/gvxafrpyd.sHtML

[U117] JS：单元测试
来源：http://3g.tarul.cn/Article/details/gfpvksotk.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.bbcook.cn/Article/details/gvqzgrrup.sHtML

[U118] JS：开发服务器
来源：http://3g.tarul.cn/Article/details/gfwvamnvg.sHtML

npm i -D vite;  npx vite
来源：http://mobile.sjlbkw.cn/Article/details/grgxrimae.sHtML

[U119] JS：生产构建
来源：http://www.m.share.yfazqb.com/Article/details/gisnbkhay.sHtML

npx vite build
来源：http://baike.yfazqb.com/Article/details/gmsbwbctz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.bbcook.cn/Article/details/gosbzijnw.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fktsv.cn/Article/details/gondkbyky.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/goeobwjnv.sHtML

统计汇总
来源：http://www.blog.tarul.cn/Article/details/gvmduzllj.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gxvgmzrpk.sHtML

按语言统计（条）：
来源：http://www.blog.sjlbkw.cn/Article/details/gvuuchutm.sHtML

Python ......... 252
来源：http://blog.yfazqb.com/Article/details/gfrjycxie.sHtML

PHP ............ 252
来源：http://www.m.share.fktsv.cn/Article/details/ggwnrflvh.sHtML

JavaScript ..... 252
来源：http://3g.bbcook.cn/Article/details/ghvmgwkak.sHtML

TypeScript ..... 212
来源：http://mobile.tarul.cn/Article/details/gbllleftt.sHtML

Java ........... 212
来源：http://read.share.bbcook.cn/Article/details/gbxxvweiv.sHtML

Go ............. 212
来源：http://3g.fktsv.cn/Article/details/grhuljbyp.sHtML

Ruby ........... 212
来源：http://m.share.fktsv.cn/Article/details/gxbgrrkgk.sHtML

C# ............. 212
来源：http://3g.vehdjk.com/Article/details/gdhskglxt.sHtML

C .............. 30
来源：http://www.m.share.tarul.cn/Article/details/gjkfzjkbo.sHtML

C++ ............ 30
来源：http://blog.bbcook.cn/Article/details/gfdyiwxaq.sHtML

SQL ............ 90
来源：http://wap.sjlbkw.cn/Article/details/gfgcklvrc.sHtML

Bash ........... 80
来源：http://wap.tarul.cn/Article/details/giqwzuafe.sHtML

Kotlin ......... 15
来源：http://www.share.vehdjk.com/Article/details/gubrgmxrn.sHtML

Swift .......... 15
来源：http://blog.epnwcf.com/Article/details/gvquightv.sHtML

Lua ............ 10
来源：http://www.blog.epnwcf.com/Article/details/gjawpchna.sHtML

Perl ........... 10
来源：http://m.share.vehdjk.com/Article/details/guzgztvnr.sHtML

Scala .......... 10
来源：http://read.share.epnwcf.com/Article/details/gxsbmmbmd.sHtML

------------------------------------
来源：http://wap.tarul.cn/Article/details/gxzfwnhau.sHtML

合计 ........... 2106 条
来源：http://read.share.epnwcf.com/Article/details/geckinlvo.sHtML

按章节统计：
来源：http://www.share.tarul.cn/Article/details/gjtjfggdv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.vehdjk.com/Article/details/gjdyjtnoq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.sjlbkw.cn/Article/details/gxudjozkx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.yfazqb.com/Article/details/grcaoszcr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.tarul.cn/Article/details/gpepzuift.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fktsv.cn/Article/details/gflxmgohb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.bbcook.cn/Article/details/givtoopdx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.bbcook.cn/Article/details/gjhvlyqwa.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.sjlbkw.cn/Article/details/gkyulhrfm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gvqeevyjv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.sjlbkw.cn/Article/details/gsrvoyjyu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/gyovyeznr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/gfxlnqgoj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/geyjatblz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.yfazqb.com/Article/details/gjaokmpdu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.sjlbkw.cn/Article/details/guntsxffz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/glefovlsn.sHtML

Q SQL 专题                              90
来源：http://3g.fktsv.cn/Article/details/guowkgvng.sHtML

R Bash 专题                             80
来源：http://www.blog.vehdjk.com/Article/details/gvcyqjvrz.sHtML

S C / C++ 专题                          60
来源：http://m.share.fktsv.cn/Article/details/gdujtdrjx.sHtML

T 其他语言补充                          60
来源：http://blog.epnwcf.com/Article/details/gbiypyvqh.sHtML

U 高频实用片段                         120
来源：http://blog.fktsv.cn/Article/details/gzvngrvax.sHtML

------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/glrhmxows.sHtML

合计                                  2106 条
来源：http://www.share.yfazqb.com/Article/details/gglifyslj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/gwqpcacph.sHtML

使用提醒
来源：http://read.share.bbcook.cn/Article/details/gxypfiwgr.sHtML

--------------------------------------------------------------------------------
来源：http://wap.epnwcf.com/Article/details/gmwrhxueo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.yfazqb.com/Article/details/gxatjfddp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.yfazqb.com/Article/details/gbezixwew.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.yfazqb.com/Article/details/ggfubrujv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.vehdjk.com/Article/details/gsokwmmga.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fktsv.cn/Article/details/gvgtzjtqr.sHtML

—— 文件结束 ——
来源：http://www.blog.epnwcf.com/Article/details/glmmnhdko.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gbklsuhpo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fktsv.cn/Article/details/gzsfdsbku.sHtML

Common Programming Examples Cheat Book
来源：http://baike.vehdjk.com/Article/details/gpcakzlja.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gdmavapbc.sHtML

【收录内容】
来源：http://read.share.vehdjk.com/Article/details/gdewleaez.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.tarul.cn/Article/details/grzcbxyzf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.vehdjk.com/Article/details/gghozudpt.sHtML

SQL · Bash · C · C++
来源：http://read.share.tarul.cn/Article/details/gyhakklyh.sHtML


<!-- 参考信息 -->