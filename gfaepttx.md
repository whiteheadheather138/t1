代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rjj.jinqigfzy.top

================================================================================
来源：http://pfk.epnwcf.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ukk.zdbjq.cn

================================================================================
来源：http://iqv.jinqigfzy.top

[T01] Kotlin：Hello World
来源：http://fpq.dashuyun.cn

println("Hello")
来源：http://vux.cqqwz.cn

[T02] Kotlin：变量
来源：http://rre.chenlongwang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zbg.sweek.top

[T03] Kotlin：字符串模板
来源：http://sxi.zhijiandao.cn

"值: $b"
来源：http://iva.cheryme.top

[T04] Kotlin：空安全
来源：http://wlr.gaohongyu789.top

val n: String? = null;  n?.length
来源：http://tlz.shangyingyoupin.top

[T05] Kotlin：when 表达式
来源：http://jzn.guowangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lmn.zhijiandao.cn

[T06] Kotlin：集合映射
来源：http://chs.jinqigufen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://spw.mhx1999.top

[T07] Kotlin：集合过滤
来源：http://puo.dashuyun.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://era.xuetiantiany.cn

[T08] Kotlin：数据类
来源：http://ryt.ctjpmb.com

data class User(val name: String, val age: Int)
来源：http://ioc.yvedp.cn

[T09] Kotlin：扩展函数
来源：http://dqd.9152youxi.cn

fun String.exclaim() = this + "!"
来源：http://xbv.feifeiyinyue.top

[T10] Kotlin：默认参数
来源：http://eyg.kuanghao11.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bzn.vqdsnc.cn

[T11] Kotlin：协程
来源：http://ohe.ehwqpu.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://bgz.xingfuxueyuan.xyz

[T12] Kotlin：解构声明
来源：http://ufg.haohaochexian.top

val (a, b) = Pair(1, 2)
来源：http://rhe.wangshuangyany.cn

[T13] Kotlin：只读 Map
来源：http://lhx.daxiang520.top

val m = mapOf("a" to 1)
来源：http://gtg.redwolf501.top

[T14] Kotlin：循环
来源：http://rqm.nanxinkj.top

for (i in 1..10) println(i)
来源：http://ipf.zhengqikj.top

[T15] Kotlin：接口
来源：http://bdl.birdmap.top

interface Shape { fun area(): Double }
来源：http://gaq.ehwqpu.com

[T16] Swift：Hello World
来源：http://cug.yj20258888.top

print("Hello")
来源：http://unz.kuanghao11.cn

[T17] Swift：变量与常量
来源：http://oug.bjfxy.top

var a = 1;  let b = 2
来源：http://yok.tarul.cn

[T18] Swift：字符串插值
来源：http://nxx.epnwcf.com

"值: \(b)"
来源：http://ybc.uphjek.com

[T19] Swift：可选绑定
来源：http://ixv.ivvv.top

if let n = opt { print(n) }
来源：http://rwc.shuidangran.top

[T20] Swift：数组操作
来源：http://efk.yvedp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cpu.fanxiaobao.xyz

[T21] Swift：遍历
来源：http://ukb.cucudq.cn

for x in a { print(x) }
来源：http://gbg.dashuyun.cn

[T22] Swift：字典
来源：http://bgk.yuanzhike.top

var d = ["a": 1];  d["b"] = 2
来源：http://lbi.shzxlz.cn

[T23] Swift：函数
来源：http://osv.yj202588.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jwd.yanxiufei.cn

[T24] Swift：闭包
来源：http://ipc.bbcook.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xoz.epnwcf.com

[T25] Swift：结构体
来源：http://yfw.hammf.cn

struct P { var x: Int }
来源：http://dqj.yuxming.cn

[T26] Swift：类与重写
来源：http://rqr.yj20258.top

class A: Base { override func f() {} }
来源：http://upr.9152youxi.cn

[T27] Swift：错误处理
来源：http://ctr.ywan-chungtsiang.top

do { try f() } catch { print(error) }
来源：http://dsx.ehwqpu.com

[T28] Swift：枚举
来源：http://rbt.hfpthk.cn

enum Color { case red, green }
来源：http://qrw.wangshuangyany.cn

[T29] Swift：guard 提前返回
来源：http://ebb.hongshengwenyu.top

guard let x = opt else { return }
来源：http://gal.zdbjq.cn

[T30] Swift：协议
来源：http://ocd.meibo888.top

protocol Shape { func area() -> Double }
来源：http://tke.nanxuanxn.top

[T31] Lua：Hello World
来源：http://dzs.yanxiufei.cn

print("Hello")
来源：http://jwx.jqgufenzy.top

[T32] Lua：局部变量
来源：http://ilx.ctjpmb.com

local a = 1
来源：http://ehn.yongpay.top

[T33] Lua：表（数组）
来源：http://owp.sjlbkw.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nfk.zycfv.cn

[T34] Lua：遍历表
来源：http://xzb.zhijiandao.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://imx.tianlin.xyz

[T35] Lua：字典表
来源：http://fho.zhixingplan.top

local d = { a = 1 };  d.b = 2
来源：http://pso.xylfe.cn

[T36] Lua：函数
来源：http://bhe.jianghu66.top

function add(a, b) return a + b end
来源：http://fkt.jyoumei.cn

[T37] Lua：字符串拼接
来源：http://faa.ywan-chungtsiang.top

"a" .. "b"
来源：http://bbb.yueranfly.top

[T38] Lua：条件
来源：http://uva.shangyingyoupin.top

if x > 0 then print("正") end
来源：http://acw.hesvh.cn

[T39] Lua：模式匹配
来源：http://ysg.jyoumei.cn

string.find(s, "%d+")
来源：http://dzw.sweek.top

[T40] Lua：元表
来源：http://rwk.xuanzx.com

setmetatable({}, { __index = base })
来源：http://fcs.zhixingplan.top

[T41] Perl：Hello World
来源：http://ehs.zdbjq.cn

print "Hello\n";
来源：http://tfv.daria6918.cn

[T42] Perl：变量类型
来源：http://haz.shuidangran.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fsw.zdqjudy.top

[T43] Perl：字符串插值
来源：http://ytx.sjlbkw.cn

"值: $a"
来源：http://uej.mhx1999.top

[T44] Perl：条件
来源：http://qlh.dashuyun.cn

if ($a > 0) { print "正"; }
来源：http://jxq.kuanghao11.cn

[T45] Perl：数组遍历
来源：http://ohb.feifeiyinyue.top

for my $x (@arr) { print $x; }
来源：http://dyb.jinyuanbaomall.cn

[T46] Perl：哈希操作
来源：http://wst.ydzc1.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rka.yonumen.top

[T47] Perl：正则捕获
来源：http://nom.chenjidiqi.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://rag.ctjpmb.com

[T48] Perl：正则替换
来源：http://dqc.fehbvm.com

$s =~ s/old/new/g;
来源：http://ywm.sxryk.cn

[T49] Perl：函数
来源：http://ejt.daria6918.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sih.jlsjyb.cn

[T50] Perl：逐行读文件
来源：http://agc.shuidangran.top

open my $fh, "<", "a.txt" or die $!;
来源：http://atr.yfazqb.com

while (my $line = <$fh>) { print $line; }
来源：http://hcd.52xcode.cn

[T51] Scala：Hello World
来源：http://lbr.nanxuanxn.top

println("Hello")
来源：http://zgl.tian-w.cn

[T52] Scala：变量
来源：http://nua.vqdsnc.cn

val a = 1;  var b = 2
来源：http://wpf.zhaomingkeji.xyz

[T53] Scala：字符串插值
来源：http://lul.shuidangran.top

s"值: $b"
来源：http://lyg.zhengqikj.top

[T54] Scala：集合映射
来源：http://huv.c1oappe.top

List(1, 2, 3).map(_ * 2)
来源：http://sow.svipenyu.cn

[T55] Scala：集合过滤
来源：http://sip.epnwcf.com

List(1, 2, 3).filter(_ > 1)
来源：http://nft.guowangkeji.top

[T56] Scala：样例类
来源：http://jks.pycfn.com

case class User(name: String, age: Int)
来源：http://huc.hammf.cn

[T57] Scala：模式匹配
来源：http://gvo.chenzaomai.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://hzj.jinghuilouyu.cn

[T58] Scala：函数定义
来源：http://bwx.daxiang520.top

def add(a: Int, b: Int): Int = a + b
来源：http://gbd.zhoulong.xyz

[T59] Scala：循环
来源：http://klh.jinghuilouyu.cn

for (i <- 1 to 10) println(i)
来源：http://nzb.pengpengdd.cyou

[T60] Scala：折叠
来源：http://zmv.yuxming.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ywg.hesvh.cn

================================================================================
来源：http://ftr.andypj.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fce.nanxinkj.top

================================================================================
来源：http://mfk.316326.xyz

[U01] Py：创建虚拟环境
来源：http://scr.jianghu66.top

python -m venv .venv && source .venv/bin/activate
来源：http://wxp.iojbl.cn

[U02] Py：导出 / 安装依赖
来源：http://wwj.jinqigufen.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rbd.hnqzz.top

[U03] Py：加载 .env 配置
来源：http://hek.fengsongda.top

from dotenv import load_dotenv; load_dotenv()
来源：http://unj.birdmap.top

[U04] Py：变量调试打印
来源：http://wzj.fzhhl.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://quc.gotoacloud.top

[U05] Py：列表去重且保序
来源：http://sgj.smart0.xyz

list(dict.fromkeys(arr))
来源：http://jwu.jinqigfzy.top

[U06] Py：合并两个字典
来源：http://qvg.jinqigufen.top

{**a, **b}
来源：http://owr.zdqjudy.top

[U07] Py：反转字典键值
来源：http://ced.yuxming.cn

{v: k for k, v in d.items()}
来源：http://yrd.52xcode.cn

[U08] Py：展平二维列表
来源：http://bti.ydjk.org.cn

[y for x in nested for y in x]
来源：http://bau.jianghu66.top

[U09] Py：字典取最大值的键
来源：http://oid.zhijiandao.cn

max(d, key=d.get)
来源：http://sgq.jyoumei.cn

[U10] Py：按值排序字典
来源：http://kco.vqdsnc.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://drw.jqgfzy.top

[U11] Py：生成器表达式
来源：http://fnd.redwolf501.top

(x * 2 for x in arr)
来源：http://qqq.tian-w.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qji.yanxiufei.cn

Counter(arr).most_common(3)
来源：http://atd.daria6918.cn

[U13] Py：固定长度队列
来源：http://mcf.jqgufenzy.top

deque(maxlen=10)
来源：http://boj.daxiang520.top

[U14] Py：分组收集到列表
来源：http://ggz.yanxiufei.cn

defaultdict(list)
来源：http://nkz.jlsjyb.cn

[U15] Py：高精度计时
来源：http://zjm.dashuyun.cn

t = time.perf_counter()
来源：http://qlg.cheryme.top

[U16] Py：命令行参数解析
来源：http://kfb.yj20258.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iiv.cheryme.top

[U17] Py：初始化日志
来源：http://ryv.dianchejie.cn

logging.basicConfig(level=logging.INFO)
来源：http://yeu.smart0.xyz

[U18] Py：预编译正则
来源：http://psd.zycfv.cn

pat = re.compile(r"\d+")
来源：http://zcy.iojbl.cn

[U19] Py：正则替换带回调
来源：http://uif.mhx1999.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mbo.zhoulong.xyz

[U20] Py：缓存函数结果
来源：http://djf.guannengcc.top

@functools.lru_cache(maxsize=None)
来源：http://ile.52xcode.cn

[U21] Py：自定义上下文管理器
来源：http://dpw.tarul.cn

@contextlib.contextmanager
来源：http://biy.hfpthk.cn

[U22] Py：矩阵转置
来源：http://yww.sysykeji.top

list(zip(*m))
来源：http://nln.zycfv.cn

[U23] Py：分块读取大文件
来源：http://mvv.ybcxt.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://clx.fktsv.cn

[U24] Py：路径操作
来源：http://ghi.0kj1m.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nky.shanyushiyangtech.top

[U25] Py：CSV 按字典读
来源：http://phh.sxryk.cn

csv.DictReader(f)
来源：http://fjd.fanxiaobao.xyz

[U26] Py：并发下载
来源：http://aop.jinghuilouyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bsy.wangshuangyany.cn

[U27] Py：异步 HTTP
来源：http://zlc.hnxiangtu.top

aiohttp.ClientSession() 配合 async with
来源：http://obj.gotoacloud.top

[U28] Py：类型别名
来源：http://rer.sjlbkw.cn

UserId = int
来源：http://xya.nwbrower.top

[U29] Py：属性校验
来源：http://vnt.hammf.cn

@property 与 @x.setter 配合
来源：http://mrg.fanxiaobao.xyz

[U30] Py：数据类
来源：http://qnn.shzxlz.cn

@dataclass(slots=True)
来源：http://nbb.nanxinkj.top

[U31] Py：单测
来源：http://lik.fehbvm.com

python -m pytest -q
来源：http://eek.xinyue.icu

[U32] Py：代码格式化
来源：http://llt.jinyuanbaomall.cn

ruff format . && ruff check --fix .
来源：http://pzd.jinqigfzy.top

[U33] Py：打包发布
来源：http://osp.chenjidiqi.icu

python -m build  （依赖 pyproject.toml）
来源：http://fgf.andypj.xyz

[U34] Py：判断编码
来源：http://yol.wangdashe.top

chardet.detect(raw)
来源：http://kul.yongpay.top

[U35] Py：发送邮件
来源：http://nkg.yfazqb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gmw.sweek.top

[U36] Py：定时任务
来源：http://fye.jyoumei.cn

schedule.every(10).minutes.do(job)
来源：http://mvn.yj20258.top

[U37] Py：读写 Excel
来源：http://iij.shanyushiyangkeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://jio.zhiwuduotai.top

[U38] Py：获取脚本所在目录
来源：http://qca.hcnkem.com

Path(__file__).resolve().parent
来源：http://muq.tian-w.cn

[U39] Py：判断是否在交互环境
来源：http://esr.hcnkem.com

sys.stdout.isatty()
来源：http://qku.cdnleiting.top

[U40] Py：打印到标准错误
来源：http://fas.shzxlz.cn

print("err", file=sys.stderr)
来源：http://efe.0kj1m.cn

[U41] PHP：初始化 Composer 项目
来源：http://zfz.yfazqb.com

composer init;  composer require guzzlehttp/guzzle
来源：http://qdd.nwbrower.top

[U42] PHP：PSR-4 自动加载
来源：http://fhm.hysaishi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://avh.jinqigufen.top

[U43] PHP：声明命名空间
来源：http://koz.hcnkem.com

namespace App\Http;
来源：http://lao.zhiwuduotai.top

[U44] PHP：开启严格类型
来源：http://fbd.yuanzhike.top

declare(strict_types=1);
来源：http://phh.zhijiandao.cn

[U45] PHP：类型声明与返回类型
来源：http://zdr.zhijiandao.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hts.havefunace.top

[U46] PHP：可空类型
来源：http://tnk.nwbrower.top

?string $name = null
来源：http://scv.hesvh.cn

[U47] PHP：联合类型
来源：http://nom.guowangkeji.top

int|string $id
来源：http://stt.tarul.cn

[U48] PHP：纯枚举
来源：http://hil.shzxlz.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pty.cheryme.top

[U49] PHP：只读属性
来源：http://bps.sufxvd.cn

public readonly string $name
来源：http://bjk.quarkkingdee.top

[U50] PHP：构造器属性提升
来源：http://qif.birdmap.top

public function __construct(private int $id) {}
来源：http://fia.ydjk.org.cn

[U51] PHP：数组解构
来源：http://cbr.xylfe.cn

[$a, $b] = $arr;
来源：http://ifm.ywan-chungtsiang.top

[U52] PHP：箭头函数
来源：http://mhw.xziqi.cn

$double = fn($x) => $x * 2;
来源：http://qag.ivvv.top

[U53] PHP：空合并运算符
来源：http://ium.hcnkem.com

$v = $a ?? $b ?? "default";
来源：http://aoe.zdqjudy.top

[U54] PHP：空安全调用
来源：http://cwj.sjlbkw.cn

$obj?->method()
来源：http://gzu.tarul.cn

[U55] PHP：match 表达式
来源：http://omd.cucudq.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kum.jqgufenzy.top

[U56] PHP：命名参数
来源：http://lux.gogol.net.cn

f(a: 1, b: 2)
来源：http://qbn.zhiwuduotai.top

[U57] PHP：字符串插值
来源：http://pvs.c1oappe.top

"值: {$a}"
来源：http://wxq.wangdashe.top

[U58] PHP：数组三件套
来源：http://pjc.yfazqb.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://riv.cqqwz.cn

[U59] PHP：自定义排序
来源：http://gdk.0kj1m.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zzo.feifeiyinyue.top

[U60] PHP：JSON 编解码
来源：http://vde.yueranfly.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fbs.yfazqb.com

[U61] PHP：正则
来源：http://mww.zdbjq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ddp.jqgfzy.top

[U62] PHP：日期对象
来源：http://prg.snrcjt.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jyk.pycfn.com

[U63] PHP：文件读写
来源：http://jwd.yongpay.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ruc.ehwqpu.com

[U64] PHP：目录遍历
来源：http://nhc.jinghuilouyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://cws.nanxuanxn.top

[U65] PHP：会话
来源：http://hrv.yvedp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jqp.xylfe.cn

[U66] PHP：设置 Cookie
来源：http://yzs.jinghuilouyu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vhc.sweek.top

[U67] PHP：处理文件上传
来源：http://mod.mhx1999.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://obq.xingfuxueyuan.xyz

[U68] PHP：PDO 连接
来源：http://jpm.dianchejie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tsm.gzhubu.top

[U69] PHP：PDO 预处理
来源：http://ecx.shanyushiyangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dou.sjlbkw.cn

[U70] PHP：PDO 事务
来源：http://nrh.jlsjyb.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uxg.yvedp.cn

[U71] PHP：抛出异常
来源：http://ljj.yanxiufei.cn

throw new RuntimeException("失败", 500);
来源：http://dxe.pycfn.com

[U72] PHP：写错误日志
来源：http://liv.nanxuanxn.top

error_log("失败: " . $e->getMessage());
来源：http://pbf.cashguo.top

[U73] PHP：读取 ini 配置
来源：http://tit.zdbjq.cn

parse_ini_file("config.ini", true)
来源：http://ior.52xcode.cn

[U74] PHP：读取环境变量
来源：http://jfq.vqdsnc.cn

getenv("APP_ENV") ?: "production"
来源：http://klo.316326.xyz

[U75] PHP：依赖注入
来源：http://bce.shanyushiyangtech.top

composer require psr/container
来源：http://ize.snrcjt.cn

[U76] PHP：简单路由
来源：http://xme.c1oappe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yxa.zhijiandao.cn

[U77] PHP：模板渲染
来源：http://tnf.gaohongyu789.top

composer require twig/twig
来源：http://sqr.yj20258.top

[U78] PHP：单元测试
来源：http://jev.tian-w.cn

composer require --dev phpunit/phpunit
来源：http://std.nanxuanxn.top

[U79] PHP：静态分析
来源：http://zjs.daxiang520.top

composer require --dev phpstan/phpstan
来源：http://qjp.wangdashe.top

[U80] PHP：代码规范修复
来源：http://vhl.pycfn.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://gck.jlsjyb.cn

[U81] JS：初始化项目
来源：http://eqw.iojbl.cn

npm init -y;  npm i express
来源：http://jlr.fehbvm.com

[U82] JS：package.json 脚本
来源：http://hzw.zycfv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://weh.epnwcf.com

[U83] JS：ES Module 导入导出
来源：http://sxc.feifeiyinyue.top

export const a = 1;  import { a } from "./m.js";
来源：http://dls.wangshuangyany.cn

[U84] JS：CommonJS 写法
来源：http://zal.zhixingplan.top

module.exports = { a };  const { a } = require("./m");
来源：http://aks.yuxming.cn

[U85] JS：可选链
来源：http://zlp.ydzc1.top

a?.b?.c
来源：http://jui.feifeiyinyue.top

[U86] JS：空值合并
来源：http://kzd.sufxvd.cn

a ?? b
来源：http://bkr.0kj1m.cn


<!-- 参考信息 -->