代发 wailian999

[U03] Py：加载 .env 配置
来源：http://mobile.vehdjk.com/Article/details/gizoinpcj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.yfazqb.com/Article/details/gudmwavcz.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.epnwcf.com/Article/details/gwxzrvtvy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.vehdjk.com/Article/details/genudfsab.sHtML

[U05] Py：列表去重且保序
来源：http://wap.sjlbkw.cn/Article/details/girjundxt.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.epnwcf.com/Article/details/gzlxiqmxf.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.vehdjk.com/Article/details/gsmsljour.sHtML

{**a, **b}
来源：http://m.share.bbcook.cn/Article/details/gbarkmwgg.sHtML

[U07] Py：反转字典键值
来源：http://m.share.yfazqb.com/Article/details/gfeoqvqzu.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.epnwcf.com/Article/details/gshkfitwh.sHtML

[U08] Py：展平二维列表
来源：http://baike.sjlbkw.cn/Article/details/gvxrjsojo.sHtML

[y for x in nested for y in x]
来源：http://baike.yfazqb.com/Article/details/gssradlkd.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.yfazqb.com/Article/details/gllegtddl.sHtML

max(d, key=d.get)
来源：http://baike.vehdjk.com/Article/details/gnhrvgetl.sHtML

[U10] Py：按值排序字典
来源：http://3g.epnwcf.com/Article/details/gspurcwaq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fktsv.cn/Article/details/gtjfldbde.sHtML

[U11] Py：生成器表达式
来源：http://blog.tarul.cn/Article/details/gvqluolvv.sHtML

(x * 2 for x in arr)
来源：http://www.blog.bbcook.cn/Article/details/gfeaagrfu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.yfazqb.com/Article/details/gzsxlomfx.sHtML

Counter(arr).most_common(3)
来源：http://3g.tarul.cn/Article/details/gdwofsavt.sHtML

[U13] Py：固定长度队列
来源：http://blog.yfazqb.com/Article/details/gfprqfstp.sHtML

deque(maxlen=10)
来源：http://baike.fktsv.cn/Article/details/gxnyrwaej.sHtML

[U14] Py：分组收集到列表
来源：http://3g.yfazqb.com/Article/details/gpynqkxuc.sHtML

defaultdict(list)
来源：http://www.share.fktsv.cn/Article/details/gkpwhkcux.sHtML

[U15] Py：高精度计时
来源：http://mobile.bbcook.cn/Article/details/gqmlecmtc.sHtML

t = time.perf_counter()
来源：http://baike.vehdjk.com/Article/details/gbsxtluli.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.bbcook.cn/Article/details/gctjjmzdw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fktsv.cn/Article/details/gletlhulk.sHtML

[U17] Py：初始化日志
来源：http://m.share.bbcook.cn/Article/details/grzpfemsp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.vehdjk.com/Article/details/gmuxmarhj.sHtML

[U18] Py：预编译正则
来源：http://www.share.bbcook.cn/Article/details/ginqyyzqg.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.bbcook.cn/Article/details/giqqkuozh.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fktsv.cn/Article/details/gxnwpmnbb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.vehdjk.com/Article/details/gedvoekxu.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.vehdjk.com/Article/details/gfvtbxklm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.sjlbkw.cn/Article/details/gbmnhcact.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.vehdjk.com/Article/details/goavawwys.sHtML

@contextlib.contextmanager
来源：http://blog.tarul.cn/Article/details/gyxfgnooj.sHtML

[U22] Py：矩阵转置
来源：http://3g.sjlbkw.cn/Article/details/gglcljqxe.sHtML

list(zip(*m))
来源：http://mobile.vehdjk.com/Article/details/gfhukftfl.sHtML

[U23] Py：分块读取大文件
来源：http://blog.tarul.cn/Article/details/geyzqsamd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.yfazqb.com/Article/details/gmrrqjnsy.sHtML

[U24] Py：路径操作
来源：http://blog.bbcook.cn/Article/details/gaqsoddmk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.vehdjk.com/Article/details/gybggqgxc.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.yfazqb.com/Article/details/glxvhbfeq.sHtML

csv.DictReader(f)
来源：http://wap.fktsv.cn/Article/details/gvnrdjndi.sHtML

[U26] Py：并发下载
来源：http://mobile.tarul.cn/Article/details/gqtuzclge.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.epnwcf.com/Article/details/gepkdfztq.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.vehdjk.com/Article/details/gugokuonf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.yfazqb.com/Article/details/gicbqzqvd.sHtML

[U28] Py：类型别名
来源：http://www.share.epnwcf.com/Article/details/ghqhdzjyh.sHtML

UserId = int
来源：http://3g.bbcook.cn/Article/details/gylnmihxk.sHtML

[U29] Py：属性校验
来源：http://baike.vehdjk.com/Article/details/gjzcwjxqg.sHtML

@property 与 @x.setter 配合
来源：http://www.share.vehdjk.com/Article/details/gmrfwqckh.sHtML

[U30] Py：数据类
来源：http://read.share.epnwcf.com/Article/details/gddpwwriv.sHtML

@dataclass(slots=True)
来源：http://wap.epnwcf.com/Article/details/gjorgsass.sHtML

[U31] Py：单测
来源：http://www.m.share.vehdjk.com/Article/details/gleaywepn.sHtML

python -m pytest -q
来源：http://read.share.yfazqb.com/Article/details/gqfycoztb.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.bbcook.cn/Article/details/gdsonsjyk.sHtML

ruff format . && ruff check --fix .
来源：http://baike.yfazqb.com/Article/details/gxbctmnsb.sHtML

[U33] Py：打包发布
来源：http://blog.epnwcf.com/Article/details/gwjkzxxfs.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.bbcook.cn/Article/details/gfpypoztk.sHtML

[U34] Py：判断编码
来源：http://wap.fktsv.cn/Article/details/gbnhvwcef.sHtML

chardet.detect(raw)
来源：http://m.share.epnwcf.com/Article/details/gecrrrdgm.sHtML

[U35] Py：发送邮件
来源：http://blog.yfazqb.com/Article/details/gbggyssts.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.sjlbkw.cn/Article/details/glgtidvkx.sHtML

[U36] Py：定时任务
来源：http://read.share.sjlbkw.cn/Article/details/gtmxpviqo.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.epnwcf.com/Article/details/glicbvlxa.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.yfazqb.com/Article/details/gordnbozg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.bbcook.cn/Article/details/gqvfqzapf.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.bbcook.cn/Article/details/gngsbhiyw.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.vehdjk.com/Article/details/ghpnpsvvc.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.yfazqb.com/Article/details/gqapoiuuu.sHtML

sys.stdout.isatty()
来源：http://m.share.fktsv.cn/Article/details/giwsqpnis.sHtML

[U40] Py：打印到标准错误
来源：http://blog.yfazqb.com/Article/details/gnbanyeea.sHtML

print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/gujqlvele.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fktsv.cn/Article/details/gpmrmszmi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.sjlbkw.cn/Article/details/gcokuqsmb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.bbcook.cn/Article/details/gqsoevgkn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.tarul.cn/Article/details/gusjqnpwq.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.tarul.cn/Article/details/gbybqopmf.sHtML

namespace App\Http;
来源：http://blog.tarul.cn/Article/details/ghagcgphd.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.tarul.cn/Article/details/ghfwlhyjz.sHtML

declare(strict_types=1);
来源：http://blog.epnwcf.com/Article/details/glivpdunh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.yfazqb.com/Article/details/gklctgnnl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/gjfdiepuq.sHtML

[U46] PHP：可空类型
来源：http://m.share.bbcook.cn/Article/details/gxpgvjpwe.sHtML

?string $name = null
来源：http://baike.bbcook.cn/Article/details/ggxzclzao.sHtML

[U47] PHP：联合类型
来源：http://blog.vehdjk.com/Article/details/grnuhidkn.sHtML

int|string $id
来源：http://www.blog.bbcook.cn/Article/details/gyhdrmyah.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.sjlbkw.cn/Article/details/glitnisbx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.epnwcf.com/Article/details/grcmemroe.sHtML

[U49] PHP：只读属性
来源：http://www.blog.bbcook.cn/Article/details/gmsrytqty.sHtML

public readonly string $name
来源：http://read.share.sjlbkw.cn/Article/details/gprtdgtmo.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.epnwcf.com/Article/details/gcgscuwfa.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.epnwcf.com/Article/details/gwtqwdpln.sHtML

[U51] PHP：数组解构
来源：http://blog.fktsv.cn/Article/details/gkseydeim.sHtML

[$a, $b] = $arr;
来源：http://wap.fktsv.cn/Article/details/gbdlqrfme.sHtML

[U52] PHP：箭头函数
来源：http://blog.tarul.cn/Article/details/gfwvdapsl.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.yfazqb.com/Article/details/ggoboahqi.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.sjlbkw.cn/Article/details/grgyrgbve.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.yfazqb.com/Article/details/glvmbyrpw.sHtML

[U54] PHP：空安全调用
来源：http://m.share.bbcook.cn/Article/details/gdtpaitye.sHtML

$obj?->method()
来源：http://3g.yfazqb.com/Article/details/gohkmqdik.sHtML

[U55] PHP：match 表达式
来源：http://www.share.tarul.cn/Article/details/ghjhoahhz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.vehdjk.com/Article/details/gfuwzijxa.sHtML

[U56] PHP：命名参数
来源：http://blog.bbcook.cn/Article/details/gdggsqjer.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/grfsdkedf.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.epnwcf.com/Article/details/gabkifukr.sHtML

"值: {$a}"
来源：http://baike.sjlbkw.cn/Article/details/gwwsxfqec.sHtML

[U58] PHP：数组三件套
来源：http://read.share.vehdjk.com/Article/details/galxewqfu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.vehdjk.com/Article/details/gbypgmxcz.sHtML

[U59] PHP：自定义排序
来源：http://m.share.yfazqb.com/Article/details/gcvsklhau.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fktsv.cn/Article/details/gwrtowkju.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.bbcook.cn/Article/details/gzrjhopgg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.epnwcf.com/Article/details/gczktwcvx.sHtML

[U61] PHP：正则
来源：http://www.share.bbcook.cn/Article/details/giqbaqzsx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.yfazqb.com/Article/details/gskoztfln.sHtML

[U62] PHP：日期对象
来源：http://wap.yfazqb.com/Article/details/gtjsqpuzy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.bbcook.cn/Article/details/gflfskczv.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdwcejda.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.sjlbkw.cn/Article/details/gfnwzkypg.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.epnwcf.com/Article/details/gqamamdiw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.sjlbkw.cn/Article/details/gyjflreyr.sHtML

[U65] PHP：会话
来源：http://blog.sjlbkw.cn/Article/details/gzyaucfgv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.bbcook.cn/Article/details/gdhqhtvgm.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.vehdjk.com/Article/details/gownfmkvx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.sjlbkw.cn/Article/details/giqmcjvjg.sHtML

[U67] PHP：处理文件上传
来源：http://blog.bbcook.cn/Article/details/gjtjwhtvy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.epnwcf.com/Article/details/gkkxzjlim.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fktsv.cn/Article/details/gwtuzawpi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.epnwcf.com/Article/details/gtdjvuvii.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.vehdjk.com/Article/details/gogfdyaah.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.sjlbkw.cn/Article/details/gpwxcccyc.sHtML

[U70] PHP：PDO 事务
来源：http://blog.yfazqb.com/Article/details/glugrauqt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.yfazqb.com/Article/details/gxtfxxrsy.sHtML

[U71] PHP：抛出异常
来源：http://blog.epnwcf.com/Article/details/gvdqqseih.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.sjlbkw.cn/Article/details/gbvyemtif.sHtML

[U72] PHP：写错误日志
来源：http://baike.epnwcf.com/Article/details/geostbtvc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.bbcook.cn/Article/details/gzfldetzh.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.epnwcf.com/Article/details/gqtyvbrny.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.sjlbkw.cn/Article/details/gvgffqgdc.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fktsv.cn/Article/details/gtwgxxmjw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.tarul.cn/Article/details/gnfmiagip.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fktsv.cn/Article/details/gabgryrud.sHtML

composer require psr/container
来源：http://read.share.sjlbkw.cn/Article/details/ghuezmiow.sHtML

[U76] PHP：简单路由
来源：http://m.share.fktsv.cn/Article/details/gtkzdfdst.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.epnwcf.com/Article/details/grznbmvwr.sHtML

[U77] PHP：模板渲染
来源：http://3g.epnwcf.com/Article/details/gwcoojpvi.sHtML

composer require twig/twig
来源：http://read.share.tarul.cn/Article/details/gxplqlxeb.sHtML

[U78] PHP：单元测试
来源：http://m.share.vehdjk.com/Article/details/gpgtlefjk.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.bbcook.cn/Article/details/gchwkdeac.sHtML

[U79] PHP：静态分析
来源：http://mobile.fktsv.cn/Article/details/gyrqrdbtn.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.epnwcf.com/Article/details/gsirwfrwz.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fktsv.cn/Article/details/giwacljwo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.vehdjk.com/Article/details/guqmcytez.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.yfazqb.com/Article/details/grititflb.sHtML

npm init -y;  npm i express
来源：http://m.share.yfazqb.com/Article/details/gxirvwznw.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.tarul.cn/Article/details/gszzfhsjc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.sjlbkw.cn/Article/details/gvmtzqlmr.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fktsv.cn/Article/details/gxwlysbrb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.vehdjk.com/Article/details/gzjgjaexd.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.sjlbkw.cn/Article/details/gnisymxlq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.yfazqb.com/Article/details/ggkuvfdlu.sHtML

[U85] JS：可选链
来源：http://www.blog.epnwcf.com/Article/details/giaanwevy.sHtML

a?.b?.c
来源：http://m.share.fktsv.cn/Article/details/gpyzokgjk.sHtML

[U86] JS：空值合并
来源：http://3g.bbcook.cn/Article/details/gohkafdkv.sHtML

a ?? b
来源：http://read.share.fktsv.cn/Article/details/gcgolqdqu.sHtML

[U87] JS：解构默认值
来源：http://3g.bbcook.cn/Article/details/gzmxbohfk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.epnwcf.com/Article/details/ggwpbtceo.sHtML

[U88] JS：对象展开合并
来源：http://wap.tarul.cn/Article/details/gcvivbzyi.sHtML

{ ...a, ...b }
来源：http://www.m.share.yfazqb.com/Article/details/gqrplmuij.sHtML

[U89] JS：数组去重
来源：http://read.share.epnwcf.com/Article/details/ggmbxzlad.sHtML

[...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/gyofmowqn.sHtML

[U90] JS：数字数组排序
来源：http://3g.sjlbkw.cn/Article/details/gkxzmkzlm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/ggmyglvcz.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.tarul.cn/Article/details/gclocvujk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.yfazqb.com/Article/details/gnbdqcywf.sHtML

[U92] JS：深拷贝
来源：http://baike.fktsv.cn/Article/details/gmshphzon.sHtML

structuredClone(obj)
来源：http://wap.fktsv.cn/Article/details/gzybhpjtd.sHtML

[U93] JS：模板字符串
来源：http://wap.vehdjk.com/Article/details/gwnybszcr.sHtML

`共 ${n} 条`
来源：http://m.share.tarul.cn/Article/details/gyseicqek.sHtML

[U94] JS：箭头函数
来源：http://m.share.epnwcf.com/Article/details/gnkvfcrut.sHtML

const double = x => x * 2;
来源：http://mobile.fktsv.cn/Article/details/gbvsnuphy.sHtML

[U95] JS：Promise 包装
来源：http://www.share.bbcook.cn/Article/details/ghikxhetr.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fktsv.cn/Article/details/gpyoknwhg.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.epnwcf.com/Article/details/gqvnnhgil.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gjpcpphfo.sHtML

[U97] JS：并发请求
来源：http://baike.sjlbkw.cn/Article/details/gidzlzhhe.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/gjkbnpcwg.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fktsv.cn/Article/details/gsqyundip.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.epnwcf.com/Article/details/gzfnxkwbl.sHtML

[U99] JS：事件监听
来源：http://www.blog.fktsv.cn/Article/details/grbivtywr.sHtML

el.addEventListener("click", e => {})
来源：http://wap.sjlbkw.cn/Article/details/gpgjlwgba.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.tarul.cn/Article/details/gmwrhqzee.sHtML

document.querySelector(".item")
来源：http://blog.yfazqb.com/Article/details/ggerhbnrp.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.yfazqb.com/Article/details/gjvngruro.sHtML

el.classList.toggle("active")
来源：http://wap.vehdjk.com/Article/details/gtmmtypqi.sHtML

[U102] JS：本地存储
来源：http://m.share.yfazqb.com/Article/details/gmdkggpah.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.tarul.cn/Article/details/gupisxmec.sHtML

[U103] JS：定时器
来源：http://www.m.share.epnwcf.com/Article/details/gzjsosqvl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.epnwcf.com/Article/details/gzkgxrdvx.sHtML

[U104] JS：防抖
来源：http://m.share.tarul.cn/Article/details/gwijhtnyf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/gbtsexqvw.sHtML

[U105] JS：节流
来源：http://wap.epnwcf.com/Article/details/gfaowdoij.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.vehdjk.com/Article/details/gogprfecx.sHtML

[U106] JS：日期格式化
来源：http://read.share.bbcook.cn/Article/details/gchgcbjkx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.yfazqb.com/Article/details/gymfpqehn.sHtML

[U107] JS：数字千分位
来源：http://m.share.sjlbkw.cn/Article/details/gtkxzqrms.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.yfazqb.com/Article/details/gjhdnneni.sHtML

[U108] JS：随机整数
来源：http://www.share.bbcook.cn/Article/details/getsxospv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.vehdjk.com/Article/details/gjabqzhpg.sHtML

[U109] JS：数组分组
来源：http://mobile.epnwcf.com/Article/details/gsmttkvvo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.epnwcf.com/Article/details/gujehajfr.sHtML

[U110] JS：数组分块
来源：http://www.share.fktsv.cn/Article/details/gcojqfell.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.tarul.cn/Article/details/giyrmgvnm.sHtML

[U111] JS：对象转 Map
来源：http://read.share.sjlbkw.cn/Article/details/gnbqaiesp.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.sjlbkw.cn/Article/details/gkajvvmai.sHtML

[U112] JS：字符串补位
来源：http://m.share.tarul.cn/Article/details/gaiqmoxjy.sHtML

"7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gcsmnivuo.sHtML

[U113] JS：正则替换全部
来源：http://read.share.tarul.cn/Article/details/gnyqtkshg.sHtML

s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/ggvmhibhx.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fktsv.cn/Article/details/gzdmpwwpg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.vehdjk.com/Article/details/gkeoxmhwx.sHtML

[U115] JS：生成 UUID
来源：http://m.share.tarul.cn/Article/details/gocvygghb.sHtML

crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gkwrmjdef.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.epnwcf.com/Article/details/gufewbeem.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.tarul.cn/Article/details/gbeqsggmq.sHtML

[U117] JS：单元测试
来源：http://baike.fktsv.cn/Article/details/gidqatpem.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.tarul.cn/Article/details/gluhxqvwh.sHtML

[U118] JS：开发服务器
来源：http://wap.bbcook.cn/Article/details/gvdariblj.sHtML

npm i -D vite;  npx vite
来源：http://www.share.epnwcf.com/Article/details/gkovgbgsj.sHtML

[U119] JS：生产构建
来源：http://wap.vehdjk.com/Article/details/grnoiwjnu.sHtML

npx vite build
来源：http://wap.sjlbkw.cn/Article/details/gjoqdirbv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.bbcook.cn/Article/details/ghkultskg.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.sjlbkw.cn/Article/details/gntuwqhxh.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gldecwjor.sHtML

统计汇总
来源：http://mobile.bbcook.cn/Article/details/goqqtdusd.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gzikusrcz.sHtML

按语言统计（条）：
来源：http://mobile.fktsv.cn/Article/details/gvoojrupf.sHtML

Python ......... 252
来源：http://www.m.share.sjlbkw.cn/Article/details/glxurxctm.sHtML

PHP ............ 252
来源：http://baike.tarul.cn/Article/details/gxiwyztoo.sHtML

JavaScript ..... 252
来源：http://read.share.bbcook.cn/Article/details/guevtgqhd.sHtML

TypeScript ..... 212
来源：http://read.share.yfazqb.com/Article/details/gfhhtujms.sHtML

Java ........... 212
来源：http://baike.fktsv.cn/Article/details/gskjfszhb.sHtML

Go ............. 212
来源：http://www.share.yfazqb.com/Article/details/golgnwumb.sHtML

Ruby ........... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gicigrbfx.sHtML

C# ............. 212
来源：http://www.share.vehdjk.com/Article/details/ghiplwana.sHtML

C .............. 30
来源：http://www.share.fktsv.cn/Article/details/gltwaupui.sHtML

C++ ............ 30
来源：http://wap.sjlbkw.cn/Article/details/ggrxmmapc.sHtML

SQL ............ 90
来源：http://mobile.fktsv.cn/Article/details/gxyvjplpj.sHtML

Bash ........... 80
来源：http://m.share.yfazqb.com/Article/details/gktrmkwjq.sHtML

Kotlin ......... 15
来源：http://read.share.yfazqb.com/Article/details/giicafioa.sHtML

Swift .......... 15
来源：http://www.share.vehdjk.com/Article/details/gyksmfxos.sHtML

Lua ............ 10
来源：http://www.m.share.vehdjk.com/Article/details/gcfqpjcyv.sHtML

Perl ........... 10
来源：http://mobile.epnwcf.com/Article/details/gxyhmzumn.sHtML

Scala .......... 10
来源：http://baike.bbcook.cn/Article/details/gmuhzywgq.sHtML

------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gnsrjwbbk.sHtML

合计 ........... 2106 条
来源：http://mobile.sjlbkw.cn/Article/details/gcrutneen.sHtML

按章节统计：
来源：http://m.share.tarul.cn/Article/details/gnbzxlfpf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.bbcook.cn/Article/details/grdfpiksa.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.tarul.cn/Article/details/gzlullqll.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.yfazqb.com/Article/details/gjfujppyv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fktsv.cn/Article/details/gjmkrruhm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.yfazqb.com/Article/details/gnosyvbjp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.tarul.cn/Article/details/girjmryfj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/gqpqmpoma.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.vehdjk.com/Article/details/gcvjwyuiy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gdsjovnhi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.yfazqb.com/Article/details/gizaqdldr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gbfkpbbhb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gnpitxbnf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/geklbxtpt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.bbcook.cn/Article/details/guggoouqd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.tarul.cn/Article/details/gevfchjbn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/ggtvpghoy.sHtML

Q SQL 专题                              90
来源：http://www.share.fktsv.cn/Article/details/gelhvbdtj.sHtML

R Bash 专题                             80
来源：http://www.blog.bbcook.cn/Article/details/gxirfutvx.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fktsv.cn/Article/details/gqpeabqwp.sHtML

T 其他语言补充                          60
来源：http://www.share.sjlbkw.cn/Article/details/glvtbxtgs.sHtML

U 高频实用片段                         120
来源：http://baike.sjlbkw.cn/Article/details/gtgauuagn.sHtML

------------------------------------
来源：http://baike.epnwcf.com/Article/details/gtrlehcsi.sHtML

合计                                  2106 条
来源：http://3g.tarul.cn/Article/details/gidffedph.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.tarul.cn/Article/details/gryqhlylg.sHtML

使用提醒
来源：http://3g.yfazqb.com/Article/details/gtoqtxndk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.tarul.cn/Article/details/ghsniefrd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.epnwcf.com/Article/details/gwfzukvrp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.vehdjk.com/Article/details/gvgkdjcyi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.epnwcf.com/Article/details/gvjpemrfw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.epnwcf.com/Article/details/ghnvppbyb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.epnwcf.com/Article/details/gvynikucl.sHtML

—— 文件结束 ——
来源：http://read.share.tarul.cn/Article/details/gukzuqkan.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gjszxjxqm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.yfazqb.com/Article/details/gdhgjjcqp.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.sjlbkw.cn/Article/details/gygmdtgad.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gwhtghauh.sHtML

【收录内容】
来源：http://3g.yfazqb.com/Article/details/gcxilyefv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.bbcook.cn/Article/details/gzfgbdqjw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.vehdjk.com/Article/details/gjrbuecuk.sHtML

SQL · Bash · C · C++
来源：http://mobile.yfazqb.com/Article/details/gxmmlqtbp.sHtML


<!-- 参考信息 -->