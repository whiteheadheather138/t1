代发 wailian999

[T05] Kotlin：when 表达式
来源：http://pvd.cqqwz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://afo.zhijiandao.cn

[T06] Kotlin：集合映射
来源：http://mwk.zhiwuduotai.top

listOf(1, 2, 3).map { it * 2 }
来源：http://put.c1oappe.top

[T07] Kotlin：集合过滤
来源：http://pxt.yvedp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hvn.zdbjq.cn

[T08] Kotlin：数据类
来源：http://rkv.yueranfly.top

data class User(val name: String, val age: Int)
来源：http://tnp.tanke756.top

[T09] Kotlin：扩展函数
来源：http://guv.52xcode.cn

fun String.exclaim() = this + "!"
来源：http://qni.smart0.xyz

[T10] Kotlin：默认参数
来源：http://jmq.jinyuanbaomall.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ylm.tanke756.top

[T11] Kotlin：协程
来源：http://mrz.zhijiandao.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://iiq.sufxvd.cn

[T12] Kotlin：解构声明
来源：http://kej.ydzc1.top

val (a, b) = Pair(1, 2)
来源：http://lif.zycfv.cn

[T13] Kotlin：只读 Map
来源：http://zlm.yfazqb.com

val m = mapOf("a" to 1)
来源：http://jiz.zhaomingkeji.xyz

[T14] Kotlin：循环
来源：http://slv.ivvv.top

for (i in 1..10) println(i)
来源：http://uwt.shangyingyoupin.top

[T15] Kotlin：接口
来源：http://jcz.xylfe.cn

interface Shape { fun area(): Double }
来源：http://mur.gzhubu.top

[T16] Swift：Hello World
来源：http://rsr.cucudq.cn

print("Hello")
来源：http://frw.jyoumei.cn

[T17] Swift：变量与常量
来源：http://vvb.xziqi.cn

var a = 1;  let b = 2
来源：http://syg.cqqwz.cn

[T18] Swift：字符串插值
来源：http://orf.xziqi.cn

"值: \(b)"
来源：http://gwr.nanxinkj.top

[T19] Swift：可选绑定
来源：http://izu.yongpay.top

if let n = opt { print(n) }
来源：http://keq.zdbjq.cn

[T20] Swift：数组操作
来源：http://gwx.sufxvd.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gzx.xuanzx.com

[T21] Swift：遍历
来源：http://osr.52xcode.cn

for x in a { print(x) }
来源：http://bat.guowangkeji.top

[T22] Swift：字典
来源：http://blj.tian-w.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pmq.yueranfly.top

[T23] Swift：函数
来源：http://aij.aibaodan.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://duj.sufxvd.cn

[T24] Swift：闭包
来源：http://yju.hfpthk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vct.jianghu66.top

[T25] Swift：结构体
来源：http://umi.zhoulong.xyz

struct P { var x: Int }
来源：http://szw.tianlin.xyz

[T26] Swift：类与重写
来源：http://mho.jyoumei.cn

class A: Base { override func f() {} }
来源：http://bhl.meibo888.top

[T27] Swift：错误处理
来源：http://niw.sxryk.cn

do { try f() } catch { print(error) }
来源：http://eum.feifeiyinyue.top

[T28] Swift：枚举
来源：http://qoy.jianghu66.top

enum Color { case red, green }
来源：http://xwy.xinyue.icu

[T29] Swift：guard 提前返回
来源：http://lyf.hywenlv.cn

guard let x = opt else { return }
来源：http://asv.sjlbkw.cn

[T30] Swift：协议
来源：http://rvr.snrcjt.cn

protocol Shape { func area() -> Double }
来源：http://nif.tian-w.cn

[T31] Lua：Hello World
来源：http://tad.yuxming.cn

print("Hello")
来源：http://fde.vehdjk.com

[T32] Lua：局部变量
来源：http://lxj.chenlongwang.top

local a = 1
来源：http://imh.fzhhl.top

[T33] Lua：表（数组）
来源：http://osw.tanke756.top

local t = {1, 2, 3};  t[4] = 4
来源：http://cnq.yj20258.top

[T34] Lua：遍历表
来源：http://gjt.zhaomingkeji.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://wpu.nwbrower.top

[T35] Lua：字典表
来源：http://ygz.guowangkeji.top

local d = { a = 1 };  d.b = 2
来源：http://gsb.fktsv.cn

[T36] Lua：函数
来源：http://uld.dianchejie.cn

function add(a, b) return a + b end
来源：http://fic.jlsjyb.cn

[T37] Lua：字符串拼接
来源：http://nre.pycfn.com

"a" .. "b"
来源：http://bkx.hongshengwenyu.top

[T38] Lua：条件
来源：http://fsv.xziqi.cn

if x > 0 then print("正") end
来源：http://ozj.ydjk.org.cn

[T39] Lua：模式匹配
来源：http://xqs.hysaishi.cn

string.find(s, "%d+")
来源：http://zuv.bjfxy.top

[T40] Lua：元表
来源：http://kgj.cqqwz.cn

setmetatable({}, { __index = base })
来源：http://usg.jinghuilouyu.cn

[T41] Perl：Hello World
来源：http://mja.cqqwz.cn

print "Hello\n";
来源：http://xyc.yvedp.cn

[T42] Perl：变量类型
来源：http://yzr.hywenlv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lho.bjfxy.top

[T43] Perl：字符串插值
来源：http://oau.dashuyun.cn

"值: $a"
来源：http://avn.zhongyouzk.top

[T44] Perl：条件
来源：http://iid.jyoumei.cn

if ($a > 0) { print "正"; }
来源：http://wja.sjlbkw.cn

[T45] Perl：数组遍历
来源：http://pos.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://ucy.cashguo.top

[T46] Perl：哈希操作
来源：http://moe.yj20258.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mke.aibaodan.cn

[T47] Perl：正则捕获
来源：http://lbz.fehbvm.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://rtz.hnxiangtu.top

[T48] Perl：正则替换
来源：http://vzw.jinghuilouyu.cn

$s =~ s/old/new/g;
来源：http://exg.zhaomingkeji.xyz

[T49] Perl：函数
来源：http://zur.yuanzhike.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uev.zhaomingkeji.xyz

[T50] Perl：逐行读文件
来源：http://cpm.ivvv.top

open my $fh, "<", "a.txt" or die $!;
来源：http://buh.zhijiandao.cn

while (my $line = <$fh>) { print $line; }
来源：http://zrd.xinyue.icu

[T51] Scala：Hello World
来源：http://hiz.smart0.xyz

println("Hello")
来源：http://nsr.tianlin.xyz

[T52] Scala：变量
来源：http://dzn.daria6918.cn

val a = 1;  var b = 2
来源：http://uxz.aizwys.cn

[T53] Scala：字符串插值
来源：http://xkd.cheryme.top

s"值: $b"
来源：http://xyo.gotoacloud.top

[T54] Scala：集合映射
来源：http://kvy.jiagoushi.top

List(1, 2, 3).map(_ * 2)
来源：http://djz.wangdashe.top

[T55] Scala：集合过滤
来源：http://txl.ybcxt.top

List(1, 2, 3).filter(_ > 1)
来源：http://dyr.jinghuilouyu.cn

[T56] Scala：样例类
来源：http://ola.jqgufenzy.top

case class User(name: String, age: Int)
来源：http://jda.jqgfzy.top

[T57] Scala：模式匹配
来源：http://czi.jinyuanbaomall.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://unl.yj20258.top

[T58] Scala：函数定义
来源：http://wnc.sufxvd.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lnc.bjfxy.top

[T59] Scala：循环
来源：http://uvs.birdmap.top

for (i <- 1 to 10) println(i)
来源：http://tcf.jqgfzy.top

[T60] Scala：折叠
来源：http://trh.sjlbkw.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ogv.0kj1m.cn

================================================================================
来源：http://cgd.jinqigufen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uql.52xcode.cn

================================================================================
来源：http://nec.ppjwa.cn

[U01] Py：创建虚拟环境
来源：http://iiq.yangfankeji.com

python -m venv .venv && source .venv/bin/activate
来源：http://yeo.yj20258888.top

[U02] Py：导出 / 安装依赖
来源：http://mfc.ywan-chungtsiang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://omw.tarul.cn

[U03] Py：加载 .env 配置
来源：http://hrt.tianlin.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://dgg.shanyushiyangkeji.top

[U04] Py：变量调试打印
来源：http://mwi.ywan-chungtsiang.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xjp.jianghu66.top

[U05] Py：列表去重且保序
来源：http://hqw.yj20258.top

list(dict.fromkeys(arr))
来源：http://lvd.xinyue.icu

[U06] Py：合并两个字典
来源：http://amq.guannengcc.top

{**a, **b}
来源：http://ohd.andypj.xyz

[U07] Py：反转字典键值
来源：http://mzh.aibaodan.cn

{v: k for k, v in d.items()}
来源：http://rjz.yuxming.cn

[U08] Py：展平二维列表
来源：http://fzj.gogol.net.cn

[y for x in nested for y in x]
来源：http://qyj.guannengcc.top

[U09] Py：字典取最大值的键
来源：http://cvc.fzhhl.top

max(d, key=d.get)
来源：http://qvn.jinqigfzy.top

[U10] Py：按值排序字典
来源：http://qdv.yangfankeji.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://khh.ydjk.org.cn

[U11] Py：生成器表达式
来源：http://lpt.c1oappe.top

(x * 2 for x in arr)
来源：http://sjm.xuanzx.com

[U12] Py：取出现最多的 3 个元素
来源：http://uuy.yj20258.top

Counter(arr).most_common(3)
来源：http://wrk.hysaishi.cn

[U13] Py：固定长度队列
来源：http://irs.jinqigufen.top

deque(maxlen=10)
来源：http://yfs.chenlongwang.top

[U14] Py：分组收集到列表
来源：http://btj.yvedp.cn

defaultdict(list)
来源：http://jno.xziqi.cn

[U15] Py：高精度计时
来源：http://cpc.tarul.cn

t = time.perf_counter()
来源：http://ouv.yuanzhike.top

[U16] Py：命令行参数解析
来源：http://gcv.hywenlv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rip.shangyingyoupin.top

[U17] Py：初始化日志
来源：http://rjb.52xcode.cn

logging.basicConfig(level=logging.INFO)
来源：http://axf.cdnleiting.top

[U18] Py：预编译正则
来源：http://qme.nanxinkj.top

pat = re.compile(r"\d+")
来源：http://ill.ywan-chungtsiang.top

[U19] Py：正则替换带回调
来源：http://ert.gzhubu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dyh.ctjpmb.com

[U20] Py：缓存函数结果
来源：http://ggu.yfazqb.com

@functools.lru_cache(maxsize=None)
来源：http://zuf.epnwcf.com

[U21] Py：自定义上下文管理器
来源：http://qvw.fktsv.cn

@contextlib.contextmanager
来源：http://cos.pengpengdd.cyou

[U22] Py：矩阵转置
来源：http://kso.guowangkeji.top

list(zip(*m))
来源：http://oqj.birdmap.top

[U23] Py：分块读取大文件
来源：http://yxr.jqgufenzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://axm.zhijiandao.cn

[U24] Py：路径操作
来源：http://gmb.aibaodan.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pll.xuetiantiany.cn

[U25] Py：CSV 按字典读
来源：http://onn.jinyuanbaomall.cn

csv.DictReader(f)
来源：http://spa.yonumen.top

[U26] Py：并发下载
来源：http://dlg.jinqigufen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pzt.meibo888.top

[U27] Py：异步 HTTP
来源：http://crk.0kj1m.cn

aiohttp.ClientSession() 配合 async with
来源：http://opu.hysaishi.cn

[U28] Py：类型别名
来源：http://cfx.hongshengwenyu.top

UserId = int
来源：http://gnw.hongshengwenyu.top

[U29] Py：属性校验
来源：http://sta.snrcjt.cn

@property 与 @x.setter 配合
来源：http://tsq.xinyue.icu

[U30] Py：数据类
来源：http://arr.xuanzx.com

@dataclass(slots=True)
来源：http://fqm.cucudq.cn

[U31] Py：单测
来源：http://tsi.hysaishi.cn

python -m pytest -q
来源：http://fnp.xingfuxueyuan.xyz

[U32] Py：代码格式化
来源：http://uxx.birdmap.top

ruff format . && ruff check --fix .
来源：http://apy.birdmap.top

[U33] Py：打包发布
来源：http://dlv.ybcxt.top

python -m build  （依赖 pyproject.toml）
来源：http://blu.ywan-chungtsiang.top

[U34] Py：判断编码
来源：http://bui.hammf.cn

chardet.detect(raw)
来源：http://mef.mhx1999.top

[U35] Py：发送邮件
来源：http://ajh.nwbrower.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xfq.hywenlv.cn

[U36] Py：定时任务
来源：http://qyc.yfazqb.com

schedule.every(10).minutes.do(job)
来源：http://fxe.yvedp.cn

[U37] Py：读写 Excel
来源：http://ulz.yonumen.top

pandas.read_excel / DataFrame.to_excel
来源：http://bzi.gogol.net.cn

[U38] Py：获取脚本所在目录
来源：http://svm.vqdsnc.cn

Path(__file__).resolve().parent
来源：http://oil.yj20258.top

[U39] Py：判断是否在交互环境
来源：http://uxw.yj20258888.top

sys.stdout.isatty()
来源：http://hfx.pycfn.com

[U40] Py：打印到标准错误
来源：http://puj.mhx1999.top

print("err", file=sys.stderr)
来源：http://eqn.shzxlz.cn

[U41] PHP：初始化 Composer 项目
来源：http://mho.9152youxi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://iqq.dianchejie.cn

[U42] PHP：PSR-4 自动加载
来源：http://efm.bbcook.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jds.yueranfly.top

[U43] PHP：声明命名空间
来源：http://gzo.zhongyouzk.top

namespace App\Http;
来源：http://khs.guannengcc.top

[U44] PHP：开启严格类型
来源：http://vej.jqgufenzy.top

declare(strict_types=1);
来源：http://sty.guannengcc.top

[U45] PHP：类型声明与返回类型
来源：http://hun.hnxiangtu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://thb.guowangkeji.top

[U46] PHP：可空类型
来源：http://oci.svipenyu.cn

?string $name = null
来源：http://mra.sxryk.cn

[U47] PHP：联合类型
来源：http://eru.ydzc1.top

int|string $id
来源：http://tbs.wangshuangyany.cn

[U48] PHP：纯枚举
来源：http://ujj.jyoumei.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nwa.ctjpmb.com

[U49] PHP：只读属性
来源：http://utg.tianlin.xyz

public readonly string $name
来源：http://tlt.svipenyu.cn

[U50] PHP：构造器属性提升
来源：http://ojt.daria6918.cn

public function __construct(private int $id) {}
来源：http://iih.haohaochexian.top

[U51] PHP：数组解构
来源：http://phn.bbcook.cn

[$a, $b] = $arr;
来源：http://lzf.yongpay.top

[U52] PHP：箭头函数
来源：http://nnn.chenzaomai.com

$double = fn($x) => $x * 2;
来源：http://evq.havefunace.top

[U53] PHP：空合并运算符
来源：http://dmp.chenjidiqi.icu

$v = $a ?? $b ?? "default";
来源：http://pvu.yueranfly.top

[U54] PHP：空安全调用
来源：http://gvn.xuanzx.com

$obj?->method()
来源：http://qsm.epnwcf.com

[U55] PHP：match 表达式
来源：http://fmn.feifeiyinyue.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lwf.daxiang520.top

[U56] PHP：命名参数
来源：http://wpc.cashguo.top

f(a: 1, b: 2)
来源：http://fik.0kj1m.cn

[U57] PHP：字符串插值
来源：http://hoa.gogol.net.cn

"值: {$a}"
来源：http://wlb.uphjek.com

[U58] PHP：数组三件套
来源：http://ell.ppjwa.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vbs.tarul.cn

[U59] PHP：自定义排序
来源：http://yfc.9152youxi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://syw.wangdashe.top

[U60] PHP：JSON 编解码
来源：http://roa.bbcook.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dwf.jqgfzy.top

[U61] PHP：正则
来源：http://bzf.dashuyun.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bko.feifeiyinyue.top

[U62] PHP：日期对象
来源：http://cnj.yuanzhike.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rom.ydjk.org.cn

[U63] PHP：文件读写
来源：http://lcv.redwolf501.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gpp.gogol.net.cn

[U64] PHP：目录遍历
来源：http://wbm.fengsongda.top

glob("dir/*.php");  scandir("dir");
来源：http://fms.yuxming.cn

[U65] PHP：会话
来源：http://naz.cqqwz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://les.xuetiantiany.cn

[U66] PHP：设置 Cookie
来源：http://yfb.jianghu66.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nzr.haohaochexian.top

[U67] PHP：处理文件上传
来源：http://ndn.snrcjt.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mgo.jqgufenzy.top

[U68] PHP：PDO 连接
来源：http://bhg.fzhhl.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ktg.0kj1m.cn

[U69] PHP：PDO 预处理
来源：http://sva.zdqjudy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sph.ehwqpu.com

[U70] PHP：PDO 事务
来源：http://wur.zhengqikj.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ahw.fzhhl.top

[U71] PHP：抛出异常
来源：http://olo.jyoumei.cn

throw new RuntimeException("失败", 500);
来源：http://rqn.jlsjyb.cn

[U72] PHP：写错误日志
来源：http://yjf.sufxvd.cn

error_log("失败: " . $e->getMessage());
来源：http://fbe.snrcjt.cn

[U73] PHP：读取 ini 配置
来源：http://gwc.jinghuilouyu.cn

parse_ini_file("config.ini", true)
来源：http://sbd.xinyue.icu

[U74] PHP：读取环境变量
来源：http://aum.shanyushiyangtech.top

getenv("APP_ENV") ?: "production"
来源：http://hyj.gaohongyu789.top

[U75] PHP：依赖注入
来源：http://sip.havefunace.top

composer require psr/container
来源：http://pgf.zhaomingkeji.xyz

[U76] PHP：简单路由
来源：http://hhx.fanxiaobao.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qrw.jianghu66.top

[U77] PHP：模板渲染
来源：http://dlo.jqgufenzy.top

composer require twig/twig
来源：http://zzo.kuanghao11.cn

[U78] PHP：单元测试
来源：http://eqx.jqgufenzy.top

composer require --dev phpunit/phpunit
来源：http://nvr.hnxiangtu.top

[U79] PHP：静态分析
来源：http://cye.zdqjudy.top

composer require --dev phpstan/phpstan
来源：http://zmf.sufxvd.cn

[U80] PHP：代码规范修复
来源：http://byy.pycfn.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://crn.zdqjudy.top

[U81] JS：初始化项目
来源：http://upv.zhengqikj.top

npm init -y;  npm i express
来源：http://vev.svipenyu.cn

[U82] JS：package.json 脚本
来源：http://vgu.0kj1m.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cgg.daria6918.cn

[U83] JS：ES Module 导入导出
来源：http://ifi.vehdjk.com

export const a = 1;  import { a } from "./m.js";
来源：http://rbt.xuanzx.com

[U84] JS：CommonJS 写法
来源：http://hvz.cqqwz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mxq.guannengcc.top

[U85] JS：可选链
来源：http://tqi.316326.xyz

a?.b?.c
来源：http://rcp.sweek.top

[U86] JS：空值合并
来源：http://ssn.guowangkeji.top

a ?? b
来源：http://ijp.ybcxt.top

[U87] JS：解构默认值
来源：http://vks.bjfxy.top

const { a = 1, b = 2 } = obj;
来源：http://ook.mhx1999.top

[U88] JS：对象展开合并
来源：http://ken.ydjk.org.cn

{ ...a, ...b }
来源：http://hah.ehwqpu.com

[U89] JS：数组去重
来源：http://lil.guannengcc.top

[...new Set(arr)]
来源：http://acd.uphjek.com

[U90] JS：数字数组排序
来源：http://wuo.hnqzz.top

[...arr].sort((a, b) => a - b)
来源：http://ooo.hcnkem.com

[U91] JS：对象键值遍历
来源：http://gyh.jlsjyb.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wwo.jlsjyb.cn

[U92] JS：深拷贝
来源：http://unr.nanxinkj.top

structuredClone(obj)
来源：http://oac.chenjidiqi.icu


<!-- 参考信息 -->