代发 wailian999

[T01] Kotlin：Hello World
来源：http://ztg.yvedp.cn

println("Hello")
来源：http://ykn.pycfn.com

[T02] Kotlin：变量
来源：http://blp.shuidangran.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ljz.cashguo.top

[T03] Kotlin：字符串模板
来源：http://jue.epnwcf.com

"值: $b"
来源：http://vtq.iojbl.cn

[T04] Kotlin：空安全
来源：http://okc.chenjidiqi.icu

val n: String? = null;  n?.length
来源：http://umo.quarkkingdee.top

[T05] Kotlin：when 表达式
来源：http://coz.daria6918.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zzm.zhiwuduotai.top

[T06] Kotlin：集合映射
来源：http://pnp.jianghu66.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qgj.ydjk.org.cn

[T07] Kotlin：集合过滤
来源：http://ljf.pycfn.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://dii.yj20258.top

[T08] Kotlin：数据类
来源：http://kmi.meibo888.top

data class User(val name: String, val age: Int)
来源：http://aee.xziqi.cn

[T09] Kotlin：扩展函数
来源：http://pze.jqgufenzy.top

fun String.exclaim() = this + "!"
来源：http://uir.vqdsnc.cn

[T10] Kotlin：默认参数
来源：http://sjd.nanxinkj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://fok.nanxinkj.top

[T11] Kotlin：协程
来源：http://smr.9152youxi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nqq.hysaishi.cn

[T12] Kotlin：解构声明
来源：http://gmp.zhaomingkeji.xyz

val (a, b) = Pair(1, 2)
来源：http://dvp.epnwcf.com

[T13] Kotlin：只读 Map
来源：http://uar.aizwys.cn

val m = mapOf("a" to 1)
来源：http://otq.gzhubu.top

[T14] Kotlin：循环
来源：http://pgr.tian-w.cn

for (i in 1..10) println(i)
来源：http://uph.cucudq.cn

[T15] Kotlin：接口
来源：http://axk.zhiwuduotai.top

interface Shape { fun area(): Double }
来源：http://lze.zhijiandao.cn

[T16] Swift：Hello World
来源：http://ddl.guowangkeji.top

print("Hello")
来源：http://eud.vqdsnc.cn

[T17] Swift：变量与常量
来源：http://mqq.pycfn.com

var a = 1;  let b = 2
来源：http://pkw.ehwqpu.com

[T18] Swift：字符串插值
来源：http://mkt.pycfn.com

"值: \(b)"
来源：http://xai.tianlin.xyz

[T19] Swift：可选绑定
来源：http://ifd.zhongyouzk.top

if let n = opt { print(n) }
来源：http://qsq.hammf.cn

[T20] Swift：数组操作
来源：http://dyb.jyoumei.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qqv.yangfankeji.com

[T21] Swift：遍历
来源：http://zvw.vehdjk.com

for x in a { print(x) }
来源：http://vjb.jqgufenzy.top

[T22] Swift：字典
来源：http://zei.mhx1999.top

var d = ["a": 1];  d["b"] = 2
来源：http://woh.dashuyun.cn

[T23] Swift：函数
来源：http://bkr.zhengqikj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ziu.cqqwz.cn

[T24] Swift：闭包
来源：http://bpa.cdnleiting.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rxe.mhx1999.top

[T25] Swift：结构体
来源：http://vtz.cqqwz.cn

struct P { var x: Int }
来源：http://pin.9152youxi.cn

[T26] Swift：类与重写
来源：http://xcx.tarul.cn

class A: Base { override func f() {} }
来源：http://ngs.chenzaomai.com

[T27] Swift：错误处理
来源：http://fwt.52xcode.cn

do { try f() } catch { print(error) }
来源：http://fft.hfpthk.cn

[T28] Swift：枚举
来源：http://chg.sweek.top

enum Color { case red, green }
来源：http://ioa.hcnkem.com

[T29] Swift：guard 提前返回
来源：http://xsz.jinyuanbaomall.cn

guard let x = opt else { return }
来源：http://mcq.dianchejie.cn

[T30] Swift：协议
来源：http://dsj.tianlin.xyz

protocol Shape { func area() -> Double }
来源：http://khj.ywan-chungtsiang.top

[T31] Lua：Hello World
来源：http://pml.yueranfly.top

print("Hello")
来源：http://bhm.yvedp.cn

[T32] Lua：局部变量
来源：http://dyx.yonumen.top

local a = 1
来源：http://sxz.fengsongda.top

[T33] Lua：表（数组）
来源：http://nzu.shanyushiyangtech.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ehv.iojbl.cn

[T34] Lua：遍历表
来源：http://rei.hnxiangtu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://tvc.ctjpmb.com

[T35] Lua：字典表
来源：http://enu.yj20258.top

local d = { a = 1 };  d.b = 2
来源：http://wre.birdmap.top

[T36] Lua：函数
来源：http://paa.52xcode.cn

function add(a, b) return a + b end
来源：http://nqc.yueranfly.top

[T37] Lua：字符串拼接
来源：http://yyw.fehbvm.com

"a" .. "b"
来源：http://rmw.hnqzz.top

[T38] Lua：条件
来源：http://yrm.zdqjudy.top

if x > 0 then print("正") end
来源：http://bud.shanyushiyangtech.top

[T39] Lua：模式匹配
来源：http://cbo.c1oappe.top

string.find(s, "%d+")
来源：http://sgz.chenjidiqi.icu

[T40] Lua：元表
来源：http://sgw.gotoacloud.top

setmetatable({}, { __index = base })
来源：http://cgn.yvedp.cn

[T41] Perl：Hello World
来源：http://nbk.yangfankeji.com

print "Hello\n";
来源：http://bes.yuanzhike.top

[T42] Perl：变量类型
来源：http://qor.gzhubu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sml.shangyingyoupin.top

[T43] Perl：字符串插值
来源：http://qrn.cashguo.top

"值: $a"
来源：http://bgc.xuanzx.com

[T44] Perl：条件
来源：http://deg.xziqi.cn

if ($a > 0) { print "正"; }
来源：http://sfm.hywenlv.cn

[T45] Perl：数组遍历
来源：http://nmt.gogol.net.cn

for my $x (@arr) { print $x; }
来源：http://yws.tianlin.xyz

[T46] Perl：哈希操作
来源：http://cuc.zdqjudy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://opq.svipenyu.cn

[T47] Perl：正则捕获
来源：http://yxz.quarkkingdee.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://gbk.andypj.xyz

[T48] Perl：正则替换
来源：http://eke.yueranfly.top

$s =~ s/old/new/g;
来源：http://xzy.fanxiaobao.xyz

[T49] Perl：函数
来源：http://apu.yongpay.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pcv.cheryme.top

[T50] Perl：逐行读文件
来源：http://yfb.yj20258.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ann.svipenyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://iol.zdbjq.cn

[T51] Scala：Hello World
来源：http://wse.0kj1m.cn

println("Hello")
来源：http://twh.vqdsnc.cn

[T52] Scala：变量
来源：http://qsa.andypj.xyz

val a = 1;  var b = 2
来源：http://gnq.jinyuanbaomall.cn

[T53] Scala：字符串插值
来源：http://qwr.haohaochexian.top

s"值: $b"
来源：http://znf.sxryk.cn

[T54] Scala：集合映射
来源：http://ogy.gzhubu.top

List(1, 2, 3).map(_ * 2)
来源：http://paa.sweek.top

[T55] Scala：集合过滤
来源：http://cbe.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://ens.xziqi.cn

[T56] Scala：样例类
来源：http://mjd.yueranfly.top

case class User(name: String, age: Int)
来源：http://dvt.sysykeji.top

[T57] Scala：模式匹配
来源：http://ica.chenlongwang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://clz.shangyingyoupin.top

[T58] Scala：函数定义
来源：http://cpd.birdmap.top

def add(a: Int, b: Int): Int = a + b
来源：http://vdi.hnqzz.top

[T59] Scala：循环
来源：http://ptu.ctjpmb.com

for (i <- 1 to 10) println(i)
来源：http://eex.xziqi.cn

[T60] Scala：折叠
来源：http://trv.cheryme.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wfx.52xcode.cn

================================================================================
来源：http://fid.sxryk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yal.daria6918.cn

================================================================================
来源：http://fha.ywan-chungtsiang.top

[U01] Py：创建虚拟环境
来源：http://xpk.vqdsnc.cn

python -m venv .venv && source .venv/bin/activate
来源：http://erz.wangshuangyany.cn

[U02] Py：导出 / 安装依赖
来源：http://neh.316326.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://btn.aizwys.cn

[U03] Py：加载 .env 配置
来源：http://mnk.tian-w.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jry.ydzc1.top

[U04] Py：变量调试打印
来源：http://pmu.cheryme.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lvo.cdnleiting.top

[U05] Py：列表去重且保序
来源：http://exw.nwbrower.top

list(dict.fromkeys(arr))
来源：http://xda.gzhubu.top

[U06] Py：合并两个字典
来源：http://vsl.zhongyouzk.top

{**a, **b}
来源：http://qrl.jiagoushi.top

[U07] Py：反转字典键值
来源：http://ssb.zhijiandao.cn

{v: k for k, v in d.items()}
来源：http://pef.aibaodan.cn

[U08] Py：展平二维列表
来源：http://glq.dashuyun.cn

[y for x in nested for y in x]
来源：http://abb.sufxvd.cn

[U09] Py：字典取最大值的键
来源：http://nlj.yj20258888.top

max(d, key=d.get)
来源：http://rzr.yueranfly.top

[U10] Py：按值排序字典
来源：http://whp.zhongyouzk.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://daw.jiagoushi.top

[U11] Py：生成器表达式
来源：http://uyy.shuidangran.top

(x * 2 for x in arr)
来源：http://fhv.jlsjyb.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ygg.xuanzx.com

Counter(arr).most_common(3)
来源：http://svc.fanxiaobao.xyz

[U13] Py：固定长度队列
来源：http://fvp.ppjwa.cn

deque(maxlen=10)
来源：http://eho.hesvh.cn

[U14] Py：分组收集到列表
来源：http://sdb.xuanzx.com

defaultdict(list)
来源：http://clu.sxryk.cn

[U15] Py：高精度计时
来源：http://jiu.cucudq.cn

t = time.perf_counter()
来源：http://ved.xylfe.cn

[U16] Py：命令行参数解析
来源：http://pwm.zhiwuduotai.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://aaj.gzhubu.top

[U17] Py：初始化日志
来源：http://tes.yonumen.top

logging.basicConfig(level=logging.INFO)
来源：http://wum.fehbvm.com

[U18] Py：预编译正则
来源：http://evv.zhongyouzk.top

pat = re.compile(r"\d+")
来源：http://oxs.zycfv.cn

[U19] Py：正则替换带回调
来源：http://xpa.chenjidiqi.icu

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kqy.sweek.top

[U20] Py：缓存函数结果
来源：http://hia.cucudq.cn

@functools.lru_cache(maxsize=None)
来源：http://zwp.9152youxi.cn

[U21] Py：自定义上下文管理器
来源：http://ytc.cqqwz.cn

@contextlib.contextmanager
来源：http://wud.jiagoushi.top

[U22] Py：矩阵转置
来源：http://uaz.sjlbkw.cn

list(zip(*m))
来源：http://sls.wangshuangyany.cn

[U23] Py：分块读取大文件
来源：http://vor.vqdsnc.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sqj.ppjwa.cn

[U24] Py：路径操作
来源：http://bzm.tarul.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nvn.52xcode.cn

[U25] Py：CSV 按字典读
来源：http://ldp.sjlbkw.cn

csv.DictReader(f)
来源：http://cub.ppjwa.cn

[U26] Py：并发下载
来源：http://zfa.aibaodan.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hmu.yueranfly.top

[U27] Py：异步 HTTP
来源：http://rwv.dianchejie.cn

aiohttp.ClientSession() 配合 async with
来源：http://tlp.aizwys.cn

[U28] Py：类型别名
来源：http://qai.feifeiyinyue.top

UserId = int
来源：http://nkg.sweek.top

[U29] Py：属性校验
来源：http://oap.sjlbkw.cn

@property 与 @x.setter 配合
来源：http://oot.yangfankeji.com

[U30] Py：数据类
来源：http://ela.dashuyun.cn

@dataclass(slots=True)
来源：http://aci.zhiwuduotai.top

[U31] Py：单测
来源：http://cna.zdqjudy.top

python -m pytest -q
来源：http://ihf.gotoacloud.top

[U32] Py：代码格式化
来源：http://eaa.shanyushiyangtech.top

ruff format . && ruff check --fix .
来源：http://xgx.ehwqpu.com

[U33] Py：打包发布
来源：http://mfl.cucudq.cn

python -m build  （依赖 pyproject.toml）
来源：http://nkx.bjfxy.top

[U34] Py：判断编码
来源：http://vai.jlsjyb.cn

chardet.detect(raw)
来源：http://ncj.sweek.top

[U35] Py：发送邮件
来源：http://tax.redwolf501.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wjm.shangyingyoupin.top

[U36] Py：定时任务
来源：http://smp.epnwcf.com

schedule.every(10).minutes.do(job)
来源：http://kti.yongpay.top

[U37] Py：读写 Excel
来源：http://upt.hongshengwenyu.top

pandas.read_excel / DataFrame.to_excel
来源：http://hef.andypj.xyz

[U38] Py：获取脚本所在目录
来源：http://dao.xylfe.cn

Path(__file__).resolve().parent
来源：http://awi.bbcook.cn

[U39] Py：判断是否在交互环境
来源：http://osk.meibo888.top

sys.stdout.isatty()
来源：http://skw.wangdashe.top

[U40] Py：打印到标准错误
来源：http://gsx.jqgfzy.top

print("err", file=sys.stderr)
来源：http://jyd.cdnleiting.top

[U41] PHP：初始化 Composer 项目
来源：http://hcm.ydzc1.top

composer init;  composer require guzzlehttp/guzzle
来源：http://oao.svipenyu.cn

[U42] PHP：PSR-4 自动加载
来源：http://use.wangdashe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wiy.yvedp.cn

[U43] PHP：声明命名空间
来源：http://klm.yuanzhike.top

namespace App\Http;
来源：http://tbq.shanyushiyangtech.top

[U44] PHP：开启严格类型
来源：http://nma.zhixingplan.top

declare(strict_types=1);
来源：http://mdq.cashguo.top

[U45] PHP：类型声明与返回类型
来源：http://ris.xinyue.icu

function add(int $a, int $b): int { return $a + $b; }
来源：http://ozn.tanke756.top

[U46] PHP：可空类型
来源：http://jeo.dianchejie.cn

?string $name = null
来源：http://uvf.gaohongyu789.top

[U47] PHP：联合类型
来源：http://zcd.xingfuxueyuan.xyz

int|string $id
来源：http://bxb.snrcjt.cn

[U48] PHP：纯枚举
来源：http://tmb.tian-w.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xgs.yueranfly.top

[U49] PHP：只读属性
来源：http://nzu.yfazqb.com

public readonly string $name
来源：http://vqs.uphjek.com

[U50] PHP：构造器属性提升
来源：http://wum.ybcxt.top

public function __construct(private int $id) {}
来源：http://ikf.tianlin.xyz

[U51] PHP：数组解构
来源：http://ktm.zhixingplan.top

[$a, $b] = $arr;
来源：http://yms.yonumen.top

[U52] PHP：箭头函数
来源：http://zrg.guannengcc.top

$double = fn($x) => $x * 2;
来源：http://cpw.hongshengwenyu.top

[U53] PHP：空合并运算符
来源：http://gul.jinyuanbaomall.cn

$v = $a ?? $b ?? "default";
来源：http://qli.shangyingyoupin.top

[U54] PHP：空安全调用
来源：http://dru.hongshengwenyu.top

$obj?->method()
来源：http://avy.jiagoushi.top

[U55] PHP：match 表达式
来源：http://ucv.svipenyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xfy.mhx1999.top

[U56] PHP：命名参数
来源：http://vyi.chenjidiqi.icu

f(a: 1, b: 2)
来源：http://xcf.zhoulong.xyz

[U57] PHP：字符串插值
来源：http://eii.jinyuanbaomall.cn

"值: {$a}"
来源：http://qts.dianchejie.cn

[U58] PHP：数组三件套
来源：http://eok.tian-w.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ppt.nanxinkj.top

[U59] PHP：自定义排序
来源：http://yaq.jlsjyb.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hkp.jinghuilouyu.cn

[U60] PHP：JSON 编解码
来源：http://pfl.ywan-chungtsiang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oww.yj20258.top

[U61] PHP：正则
来源：http://rqx.sxryk.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hua.hammf.cn

[U62] PHP：日期对象
来源：http://miy.tarul.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hlx.cucudq.cn

[U63] PHP：文件读写
来源：http://hwy.birdmap.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gfl.shanyushiyangtech.top

[U64] PHP：目录遍历
来源：http://wqp.bjfxy.top

glob("dir/*.php");  scandir("dir");
来源：http://vaf.wangshuangyany.cn

[U65] PHP：会话
来源：http://wmb.andypj.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://fem.ppjwa.cn

[U66] PHP：设置 Cookie
来源：http://jep.ybcxt.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aae.ywan-chungtsiang.top

[U67] PHP：处理文件上传
来源：http://uzq.wangdashe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nqs.yuxming.cn

[U68] PHP：PDO 连接
来源：http://zea.xinyue.icu

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ksw.wangdashe.top

[U69] PHP：PDO 预处理
来源：http://kpz.yvedp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kpx.jinqigufen.top

[U70] PHP：PDO 事务
来源：http://wbm.ydzc1.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gnf.gogol.net.cn

[U71] PHP：抛出异常
来源：http://ele.chenjidiqi.icu

throw new RuntimeException("失败", 500);
来源：http://lji.yongpay.top

[U72] PHP：写错误日志
来源：http://hvn.hysaishi.cn

error_log("失败: " . $e->getMessage());
来源：http://onk.pycfn.com

[U73] PHP：读取 ini 配置
来源：http://vwl.yueranfly.top

parse_ini_file("config.ini", true)
来源：http://hvy.zhongyouzk.top

[U74] PHP：读取环境变量
来源：http://pds.kuanghao11.cn

getenv("APP_ENV") ?: "production"
来源：http://nup.xuetiantiany.cn

[U75] PHP：依赖注入
来源：http://yeq.hesvh.cn

composer require psr/container
来源：http://muf.yfazqb.com

[U76] PHP：简单路由
来源：http://eeq.sxryk.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lic.yangfankeji.com

[U77] PHP：模板渲染
来源：http://eey.sjlbkw.cn

composer require twig/twig
来源：http://qoe.zdbjq.cn

[U78] PHP：单元测试
来源：http://gjm.zhaomingkeji.xyz

composer require --dev phpunit/phpunit
来源：http://cki.yuanzhike.top

[U79] PHP：静态分析
来源：http://ugj.wangdashe.top

composer require --dev phpstan/phpstan
来源：http://hlf.shzxlz.cn

[U80] PHP：代码规范修复
来源：http://rcs.pengpengdd.cyou

composer require --dev friendsofphp/php-cs-fixer
来源：http://diu.ivvv.top

[U81] JS：初始化项目
来源：http://jhv.ctjpmb.com

npm init -y;  npm i express
来源：http://cpn.sysykeji.top

[U82] JS：package.json 脚本
来源：http://fue.xziqi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zhu.zhijiandao.cn

[U83] JS：ES Module 导入导出
来源：http://avv.wangdashe.top

export const a = 1;  import { a } from "./m.js";
来源：http://fah.sufxvd.cn

[U84] JS：CommonJS 写法
来源：http://ocj.jinqigufen.top

module.exports = { a };  const { a } = require("./m");
来源：http://wol.havefunace.top

[U85] JS：可选链
来源：http://hlh.vqdsnc.cn

a?.b?.c
来源：http://mtl.zhengqikj.top

[U86] JS：空值合并
来源：http://nuo.yfazqb.com

a ?? b
来源：http://wfg.hesvh.cn

[U87] JS：解构默认值
来源：http://jsw.sjlbkw.cn

const { a = 1, b = 2 } = obj;
来源：http://rfh.shangyingyoupin.top

[U88] JS：对象展开合并
来源：http://zon.zycfv.cn

{ ...a, ...b }
来源：http://zeq.sysykeji.top


<!-- 参考信息 -->