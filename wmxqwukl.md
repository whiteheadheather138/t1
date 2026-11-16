代发 wailian999

[T01] Kotlin：Hello World
来源：http://dig.9152youxi.cn

println("Hello")
来源：http://bob.dianchejie.cn

[T02] Kotlin：变量
来源：http://wlm.ydjk.org.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://god.cqqwz.cn

[T03] Kotlin：字符串模板
来源：http://pem.pycfn.com

"值: $b"
来源：http://aha.9152youxi.cn

[T04] Kotlin：空安全
来源：http://amy.hywenlv.cn

val n: String? = null;  n?.length
来源：http://wtu.xylfe.cn

[T05] Kotlin：when 表达式
来源：http://zmj.bjfxy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gut.jlsjyb.cn

[T06] Kotlin：集合映射
来源：http://wdb.ctjpmb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://qtu.guannengcc.top

[T07] Kotlin：集合过滤
来源：http://swh.shangyingyoupin.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://lka.ctjpmb.com

[T08] Kotlin：数据类
来源：http://vrq.fehbvm.com

data class User(val name: String, val age: Int)
来源：http://ymt.snrcjt.cn

[T09] Kotlin：扩展函数
来源：http://kes.epnwcf.com

fun String.exclaim() = this + "!"
来源：http://kip.dianchejie.cn

[T10] Kotlin：默认参数
来源：http://ynz.uphjek.com

fun greet(name: String = "World") = "Hi $name"
来源：http://mlo.jinghuilouyu.cn

[T11] Kotlin：协程
来源：http://rst.xziqi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rdf.daxiang520.top

[T12] Kotlin：解构声明
来源：http://mzf.fanxiaobao.xyz

val (a, b) = Pair(1, 2)
来源：http://cow.nanxuanxn.top

[T13] Kotlin：只读 Map
来源：http://pet.fehbvm.com

val m = mapOf("a" to 1)
来源：http://gon.hongshengwenyu.top

[T14] Kotlin：循环
来源：http://hhh.zhixingplan.top

for (i in 1..10) println(i)
来源：http://pww.jinyuanbaomall.cn

[T15] Kotlin：接口
来源：http://mfa.yvedp.cn

interface Shape { fun area(): Double }
来源：http://uyj.guannengcc.top

[T16] Swift：Hello World
来源：http://tmq.bbcook.cn

print("Hello")
来源：http://qdb.hysaishi.cn

[T17] Swift：变量与常量
来源：http://wam.havefunace.top

var a = 1;  let b = 2
来源：http://duw.hywenlv.cn

[T18] Swift：字符串插值
来源：http://xrz.jqgufenzy.top

"值: \(b)"
来源：http://fzb.tianlin.xyz

[T19] Swift：可选绑定
来源：http://rur.sweek.top

if let n = opt { print(n) }
来源：http://pgc.hammf.cn

[T20] Swift：数组操作
来源：http://zoc.sxryk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qaq.ybcxt.top

[T21] Swift：遍历
来源：http://zly.zycfv.cn

for x in a { print(x) }
来源：http://ysm.yonumen.top

[T22] Swift：字典
来源：http://wwv.cdnleiting.top

var d = ["a": 1];  d["b"] = 2
来源：http://oav.cucudq.cn

[T23] Swift：函数
来源：http://uwf.svipenyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://byv.sysykeji.top

[T24] Swift：闭包
来源：http://scz.fehbvm.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://dqv.hammf.cn

[T25] Swift：结构体
来源：http://mfq.zhixingplan.top

struct P { var x: Int }
来源：http://tpz.wangshuangyany.cn

[T26] Swift：类与重写
来源：http://wxs.yvedp.cn

class A: Base { override func f() {} }
来源：http://peh.guannengcc.top

[T27] Swift：错误处理
来源：http://qmn.uphjek.com

do { try f() } catch { print(error) }
来源：http://cwm.quarkkingdee.top

[T28] Swift：枚举
来源：http://ndq.cucudq.cn

enum Color { case red, green }
来源：http://vlz.mhx1999.top

[T29] Swift：guard 提前返回
来源：http://ysu.tianlin.xyz

guard let x = opt else { return }
来源：http://tze.jinqigfzy.top

[T30] Swift：协议
来源：http://irs.iojbl.cn

protocol Shape { func area() -> Double }
来源：http://nmw.cheryme.top

[T31] Lua：Hello World
来源：http://lvr.nanxinkj.top

print("Hello")
来源：http://xxz.guannengcc.top

[T32] Lua：局部变量
来源：http://aaq.daria6918.cn

local a = 1
来源：http://hhm.aizwys.cn

[T33] Lua：表（数组）
来源：http://wpo.fzhhl.top

local t = {1, 2, 3};  t[4] = 4
来源：http://owr.xuetiantiany.cn

[T34] Lua：遍历表
来源：http://olm.xziqi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://eaz.xuetiantiany.cn

[T35] Lua：字典表
来源：http://edr.meibo888.top

local d = { a = 1 };  d.b = 2
来源：http://nxr.jiagoushi.top

[T36] Lua：函数
来源：http://wxc.yueranfly.top

function add(a, b) return a + b end
来源：http://zuu.cucudq.cn

[T37] Lua：字符串拼接
来源：http://ibm.tianlin.xyz

"a" .. "b"
来源：http://lfi.yanxiufei.cn

[T38] Lua：条件
来源：http://eys.tarul.cn

if x > 0 then print("正") end
来源：http://ubu.shuidangran.top

[T39] Lua：模式匹配
来源：http://oxr.gotoacloud.top

string.find(s, "%d+")
来源：http://aiq.zhengqikj.top

[T40] Lua：元表
来源：http://chp.hcnkem.com

setmetatable({}, { __index = base })
来源：http://ope.quarkkingdee.top

[T41] Perl：Hello World
来源：http://lon.iojbl.cn

print "Hello\n";
来源：http://qxr.sufxvd.cn

[T42] Perl：变量类型
来源：http://yxw.ctjpmb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://iko.aibaodan.cn

[T43] Perl：字符串插值
来源：http://kwj.ehwqpu.com

"值: $a"
来源：http://dgh.xingfuxueyuan.xyz

[T44] Perl：条件
来源：http://anp.hcnkem.com

if ($a > 0) { print "正"; }
来源：http://inc.guowangkeji.top

[T45] Perl：数组遍历
来源：http://iuc.nwbrower.top

for my $x (@arr) { print $x; }
来源：http://nkf.fanxiaobao.xyz

[T46] Perl：哈希操作
来源：http://qhd.snrcjt.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nhw.zycfv.cn

[T47] Perl：正则捕获
来源：http://bkn.aizwys.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ggr.hnxiangtu.top

[T48] Perl：正则替换
来源：http://ekj.feifeiyinyue.top

$s =~ s/old/new/g;
来源：http://nfj.yvedp.cn

[T49] Perl：函数
来源：http://szp.xuetiantiany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://msy.hesvh.cn

[T50] Perl：逐行读文件
来源：http://mvo.xylfe.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tlx.jinyuanbaomall.cn

while (my $line = <$fh>) { print $line; }
来源：http://ghh.tarul.cn

[T51] Scala：Hello World
来源：http://cga.nanxinkj.top

println("Hello")
来源：http://sms.jiagoushi.top

[T52] Scala：变量
来源：http://ygt.haohaochexian.top

val a = 1;  var b = 2
来源：http://xey.daxiang520.top

[T53] Scala：字符串插值
来源：http://fkw.jiagoushi.top

s"值: $b"
来源：http://dca.quarkkingdee.top

[T54] Scala：集合映射
来源：http://tov.birdmap.top

List(1, 2, 3).map(_ * 2)
来源：http://isa.smart0.xyz

[T55] Scala：集合过滤
来源：http://ekf.xinyue.icu

List(1, 2, 3).filter(_ > 1)
来源：http://wnh.fanxiaobao.xyz

[T56] Scala：样例类
来源：http://akt.nanxuanxn.top

case class User(name: String, age: Int)
来源：http://liz.cucudq.cn

[T57] Scala：模式匹配
来源：http://ixt.gogol.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pbh.fehbvm.com

[T58] Scala：函数定义
来源：http://jwc.yj20258888.top

def add(a: Int, b: Int): Int = a + b
来源：http://zsq.nanxuanxn.top

[T59] Scala：循环
来源：http://mat.iojbl.cn

for (i <- 1 to 10) println(i)
来源：http://ccj.pycfn.com

[T60] Scala：折叠
来源：http://lhn.yj20258.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fot.zhoulong.xyz

================================================================================
来源：http://gwj.52xcode.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ykb.gzhubu.top

================================================================================
来源：http://enr.vehdjk.com

[U01] Py：创建虚拟环境
来源：http://nme.feifeiyinyue.top

python -m venv .venv && source .venv/bin/activate
来源：http://xfx.yj202588.top

[U02] Py：导出 / 安装依赖
来源：http://zyi.vqdsnc.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uaj.ydjk.org.cn

[U03] Py：加载 .env 配置
来源：http://guc.guannengcc.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ouh.sweek.top

[U04] Py：变量调试打印
来源：http://alx.chenlongwang.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://asn.ivvv.top

[U05] Py：列表去重且保序
来源：http://aqw.sjlbkw.cn

list(dict.fromkeys(arr))
来源：http://gau.cdnleiting.top

[U06] Py：合并两个字典
来源：http://wcc.yangfankeji.com

{**a, **b}
来源：http://clu.sufxvd.cn

[U07] Py：反转字典键值
来源：http://ogu.shanyushiyangtech.top

{v: k for k, v in d.items()}
来源：http://wmj.zhaomingkeji.xyz

[U08] Py：展平二维列表
来源：http://hhh.zhijiandao.cn

[y for x in nested for y in x]
来源：http://rsd.shzxlz.cn

[U09] Py：字典取最大值的键
来源：http://wke.pengpengdd.cyou

max(d, key=d.get)
来源：http://jyc.gotoacloud.top

[U10] Py：按值排序字典
来源：http://xzw.wangshuangyany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://euq.xinyue.icu

[U11] Py：生成器表达式
来源：http://tnk.haohaochexian.top

(x * 2 for x in arr)
来源：http://fww.fanxiaobao.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://icz.sxryk.cn

Counter(arr).most_common(3)
来源：http://kog.xinyue.icu

[U13] Py：固定长度队列
来源：http://hjw.yuxming.cn

deque(maxlen=10)
来源：http://amo.bjfxy.top

[U14] Py：分组收集到列表
来源：http://orh.0kj1m.cn

defaultdict(list)
来源：http://wtm.uphjek.com

[U15] Py：高精度计时
来源：http://hub.cucudq.cn

t = time.perf_counter()
来源：http://vkv.zhiwuduotai.top

[U16] Py：命令行参数解析
来源：http://bef.cucudq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jej.zdqjudy.top

[U17] Py：初始化日志
来源：http://xpa.ctjpmb.com

logging.basicConfig(level=logging.INFO)
来源：http://abm.jiagoushi.top

[U18] Py：预编译正则
来源：http://uhu.jinghuilouyu.cn

pat = re.compile(r"\d+")
来源：http://fly.zhongyouzk.top

[U19] Py：正则替换带回调
来源：http://iyx.zhijiandao.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xqk.hysaishi.cn

[U20] Py：缓存函数结果
来源：http://yus.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://kmy.uphjek.com

[U21] Py：自定义上下文管理器
来源：http://xhj.shanyushiyangkeji.top

@contextlib.contextmanager
来源：http://zhj.gaohongyu789.top

[U22] Py：矩阵转置
来源：http://aev.ydzc1.top

list(zip(*m))
来源：http://iak.sxryk.cn

[U23] Py：分块读取大文件
来源：http://ujn.wangshuangyany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bgr.xylfe.cn

[U24] Py：路径操作
来源：http://unn.sysykeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://enp.sweek.top

[U25] Py：CSV 按字典读
来源：http://ije.hesvh.cn

csv.DictReader(f)
来源：http://pxx.yuxming.cn

[U26] Py：并发下载
来源：http://efi.epnwcf.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cgd.fktsv.cn

[U27] Py：异步 HTTP
来源：http://rdg.zdqjudy.top

aiohttp.ClientSession() 配合 async with
来源：http://nba.c1oappe.top

[U28] Py：类型别名
来源：http://aid.gzhubu.top

UserId = int
来源：http://vwx.tian-w.cn

[U29] Py：属性校验
来源：http://zif.pycfn.com

@property 与 @x.setter 配合
来源：http://hxk.jyoumei.cn

[U30] Py：数据类
来源：http://oia.zhengqikj.top

@dataclass(slots=True)
来源：http://lxo.hnxiangtu.top

[U31] Py：单测
来源：http://emi.jiagoushi.top

python -m pytest -q
来源：http://uzz.dianchejie.cn

[U32] Py：代码格式化
来源：http://lrh.iojbl.cn

ruff format . && ruff check --fix .
来源：http://fbp.ctjpmb.com

[U33] Py：打包发布
来源：http://uir.bjfxy.top

python -m build  （依赖 pyproject.toml）
来源：http://jqd.cqqwz.cn

[U34] Py：判断编码
来源：http://tmr.xuetiantiany.cn

chardet.detect(raw)
来源：http://adb.yanxiufei.cn

[U35] Py：发送邮件
来源：http://uvw.sxryk.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qbm.hnxiangtu.top

[U36] Py：定时任务
来源：http://plb.316326.xyz

schedule.every(10).minutes.do(job)
来源：http://zik.yvedp.cn

[U37] Py：读写 Excel
来源：http://efz.meibo888.top

pandas.read_excel / DataFrame.to_excel
来源：http://xrt.bjfxy.top

[U38] Py：获取脚本所在目录
来源：http://inv.cucudq.cn

Path(__file__).resolve().parent
来源：http://xjy.zhiwuduotai.top

[U39] Py：判断是否在交互环境
来源：http://ebq.zhijiandao.cn

sys.stdout.isatty()
来源：http://els.xylfe.cn

[U40] Py：打印到标准错误
来源：http://imr.chenlongwang.top

print("err", file=sys.stderr)
来源：http://jxd.jiagoushi.top

[U41] PHP：初始化 Composer 项目
来源：http://pgn.shanyushiyangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://mbj.shanyushiyangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://mzp.aizwys.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://snv.mhx1999.top

[U43] PHP：声明命名空间
来源：http://jmd.yuanzhike.top

namespace App\Http;
来源：http://izl.pycfn.com

[U44] PHP：开启严格类型
来源：http://zta.ctjpmb.com

declare(strict_types=1);
来源：http://pfp.hywenlv.cn

[U45] PHP：类型声明与返回类型
来源：http://xqq.yonumen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ycf.jinqigufen.top

[U46] PHP：可空类型
来源：http://mkr.vqdsnc.cn

?string $name = null
来源：http://gyv.316326.xyz

[U47] PHP：联合类型
来源：http://rea.yvedp.cn

int|string $id
来源：http://uor.tianlin.xyz

[U48] PHP：纯枚举
来源：http://kmv.jlsjyb.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wvf.gaohongyu789.top

[U49] PHP：只读属性
来源：http://uxy.jinghuilouyu.cn

public readonly string $name
来源：http://cio.zhijiandao.cn

[U50] PHP：构造器属性提升
来源：http://jsn.hywenlv.cn

public function __construct(private int $id) {}
来源：http://xxn.xuetiantiany.cn

[U51] PHP：数组解构
来源：http://ibh.yangfankeji.com

[$a, $b] = $arr;
来源：http://gwz.ivvv.top

[U52] PHP：箭头函数
来源：http://cib.wangshuangyany.cn

$double = fn($x) => $x * 2;
来源：http://pqk.svipenyu.cn

[U53] PHP：空合并运算符
来源：http://dyf.zdqjudy.top

$v = $a ?? $b ?? "default";
来源：http://jks.aizwys.cn

[U54] PHP：空安全调用
来源：http://dtc.zhijiandao.cn

$obj?->method()
来源：http://yuc.hywenlv.cn

[U55] PHP：match 表达式
来源：http://csy.andypj.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tvk.hcnkem.com

[U56] PHP：命名参数
来源：http://six.jyoumei.cn

f(a: 1, b: 2)
来源：http://yxk.tarul.cn

[U57] PHP：字符串插值
来源：http://rrj.nanxinkj.top

"值: {$a}"
来源：http://umq.tanke756.top

[U58] PHP：数组三件套
来源：http://iqy.fktsv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ggb.shangyingyoupin.top

[U59] PHP：自定义排序
来源：http://dti.dianchejie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://abg.yuxming.cn

[U60] PHP：JSON 编解码
来源：http://nit.andypj.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bsk.zdqjudy.top

[U61] PHP：正则
来源：http://jew.ivvv.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ytm.ehwqpu.com

[U62] PHP：日期对象
来源：http://xts.xziqi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xvq.nanxuanxn.top

[U63] PHP：文件读写
来源：http://gxb.ppjwa.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wge.fehbvm.com

[U64] PHP：目录遍历
来源：http://mcw.yfazqb.com

glob("dir/*.php");  scandir("dir");
来源：http://mly.ppjwa.cn

[U65] PHP：会话
来源：http://pyj.hfpthk.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hpo.pycfn.com

[U66] PHP：设置 Cookie
来源：http://zyi.9152youxi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ebt.jlsjyb.cn

[U67] PHP：处理文件上传
来源：http://uyk.gogol.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bvs.nanxinkj.top

[U68] PHP：PDO 连接
来源：http://ujx.wangshuangyany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fkm.daria6918.cn

[U69] PHP：PDO 预处理
来源：http://jss.yj202588.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rsk.cheryme.top

[U70] PHP：PDO 事务
来源：http://olp.cheryme.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qfq.pycfn.com

[U71] PHP：抛出异常
来源：http://nrg.meibo888.top

throw new RuntimeException("失败", 500);
来源：http://pha.cucudq.cn

[U72] PHP：写错误日志
来源：http://rco.smart0.xyz

error_log("失败: " . $e->getMessage());
来源：http://erl.yangfankeji.com

[U73] PHP：读取 ini 配置
来源：http://ypz.gaohongyu789.top

parse_ini_file("config.ini", true)
来源：http://ghq.hesvh.cn

[U74] PHP：读取环境变量
来源：http://ads.jlsjyb.cn

getenv("APP_ENV") ?: "production"
来源：http://fpi.yueranfly.top

[U75] PHP：依赖注入
来源：http://cls.zycfv.cn

composer require psr/container
来源：http://tuc.meibo888.top

[U76] PHP：简单路由
来源：http://yze.jqgfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jjq.dashuyun.cn

[U77] PHP：模板渲染
来源：http://ulq.daxiang520.top

composer require twig/twig
来源：http://lcz.wangshuangyany.cn

[U78] PHP：单元测试
来源：http://oxt.smart0.xyz

composer require --dev phpunit/phpunit
来源：http://loq.tarul.cn

[U79] PHP：静态分析
来源：http://ghw.snrcjt.cn

composer require --dev phpstan/phpstan
来源：http://psq.shangyingyoupin.top

[U80] PHP：代码规范修复
来源：http://rcz.fzhhl.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://vlc.vqdsnc.cn

[U81] JS：初始化项目
来源：http://cob.chenlongwang.top

npm init -y;  npm i express
来源：http://anl.yuanzhike.top

[U82] JS：package.json 脚本
来源：http://jhh.ydzc1.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cyo.zhengqikj.top

[U83] JS：ES Module 导入导出
来源：http://oqm.ehwqpu.com

export const a = 1;  import { a } from "./m.js";
来源：http://ius.ehwqpu.com

[U84] JS：CommonJS 写法
来源：http://hrv.chenzaomai.com

module.exports = { a };  const { a } = require("./m");
来源：http://lts.hnxiangtu.top

[U85] JS：可选链
来源：http://nzd.fehbvm.com

a?.b?.c
来源：http://hjt.cucudq.cn

[U86] JS：空值合并
来源：http://khr.yueranfly.top

a ?? b
来源：http://byr.yangfankeji.com

[U87] JS：解构默认值
来源：http://tac.dianchejie.cn

const { a = 1, b = 2 } = obj;
来源：http://rei.hysaishi.cn

[U88] JS：对象展开合并
来源：http://dfo.yuxming.cn

{ ...a, ...b }
来源：http://fyk.yonumen.top


<!-- 参考信息 -->