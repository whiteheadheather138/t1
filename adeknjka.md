代发 wailian999

[T01] Kotlin：Hello World
来源：http://lei.hywenlv.cn

println("Hello")
来源：http://byb.vqdsnc.cn

[T02] Kotlin：变量
来源：http://vqf.zhijiandao.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://noe.bbcook.cn

[T03] Kotlin：字符串模板
来源：http://bbe.jinqigfzy.top

"值: $b"
来源：http://whc.zhengqikj.top

[T04] Kotlin：空安全
来源：http://nez.yuanzhike.top

val n: String? = null;  n?.length
来源：http://ybz.ydjk.org.cn

[T05] Kotlin：when 表达式
来源：http://rvm.zhiwuduotai.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vrl.redwolf501.top

[T06] Kotlin：集合映射
来源：http://hnn.redwolf501.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ymt.9152youxi.cn

[T07] Kotlin：集合过滤
来源：http://cwr.fengsongda.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uqd.vehdjk.com

[T08] Kotlin：数据类
来源：http://byy.zdbjq.cn

data class User(val name: String, val age: Int)
来源：http://kkq.zhijiandao.cn

[T09] Kotlin：扩展函数
来源：http://mot.hnqzz.top

fun String.exclaim() = this + "!"
来源：http://bpi.yanxiufei.cn

[T10] Kotlin：默认参数
来源：http://mrz.zycfv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uaq.cdnleiting.top

[T11] Kotlin：协程
来源：http://pnx.xingfuxueyuan.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://fqo.cdnleiting.top

[T12] Kotlin：解构声明
来源：http://efn.zhixingplan.top

val (a, b) = Pair(1, 2)
来源：http://xtv.redwolf501.top

[T13] Kotlin：只读 Map
来源：http://sfp.fktsv.cn

val m = mapOf("a" to 1)
来源：http://kzm.uphjek.com

[T14] Kotlin：循环
来源：http://hxk.chenjidiqi.icu

for (i in 1..10) println(i)
来源：http://dze.zhixingplan.top

[T15] Kotlin：接口
来源：http://cdw.9152youxi.cn

interface Shape { fun area(): Double }
来源：http://tkw.sxryk.cn

[T16] Swift：Hello World
来源：http://mhp.guowangkeji.top

print("Hello")
来源：http://jmq.wangshuangyany.cn

[T17] Swift：变量与常量
来源：http://xpe.wangshuangyany.cn

var a = 1;  let b = 2
来源：http://wkh.zycfv.cn

[T18] Swift：字符串插值
来源：http://tpo.fengsongda.top

"值: \(b)"
来源：http://ihz.redwolf501.top

[T19] Swift：可选绑定
来源：http://xrz.vehdjk.com

if let n = opt { print(n) }
来源：http://dgn.sweek.top

[T20] Swift：数组操作
来源：http://tsa.gzhubu.top

var a = [1, 2, 3];  a.append(4)
来源：http://ssk.zhoulong.xyz

[T21] Swift：遍历
来源：http://sfq.dashuyun.cn

for x in a { print(x) }
来源：http://jsn.sufxvd.cn

[T22] Swift：字典
来源：http://ixf.ywan-chungtsiang.top

var d = ["a": 1];  d["b"] = 2
来源：http://rra.cucudq.cn

[T23] Swift：函数
来源：http://pvk.cashguo.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xlq.tarul.cn

[T24] Swift：闭包
来源：http://phh.yj20258.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mxd.nwbrower.top

[T25] Swift：结构体
来源：http://vec.zdqjudy.top

struct P { var x: Int }
来源：http://jxe.yfazqb.com

[T26] Swift：类与重写
来源：http://ckv.haohaochexian.top

class A: Base { override func f() {} }
来源：http://pwb.hysaishi.cn

[T27] Swift：错误处理
来源：http://sxj.shanyushiyangtech.top

do { try f() } catch { print(error) }
来源：http://bus.hywenlv.cn

[T28] Swift：枚举
来源：http://pxa.bjfxy.top

enum Color { case red, green }
来源：http://hcd.nanxinkj.top

[T29] Swift：guard 提前返回
来源：http://fix.tianlin.xyz

guard let x = opt else { return }
来源：http://bfq.hcnkem.com

[T30] Swift：协议
来源：http://uux.jinqigfzy.top

protocol Shape { func area() -> Double }
来源：http://cnk.daxiang520.top

[T31] Lua：Hello World
来源：http://ckw.zhiwuduotai.top

print("Hello")
来源：http://hfp.pengpengdd.cyou

[T32] Lua：局部变量
来源：http://orj.uphjek.com

local a = 1
来源：http://pmj.sxryk.cn

[T33] Lua：表（数组）
来源：http://abc.jinyuanbaomall.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jvt.yangfankeji.com

[T34] Lua：遍历表
来源：http://rru.cucudq.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tgd.zdbjq.cn

[T35] Lua：字典表
来源：http://rko.9152youxi.cn

local d = { a = 1 };  d.b = 2
来源：http://kst.snrcjt.cn

[T36] Lua：函数
来源：http://wch.316326.xyz

function add(a, b) return a + b end
来源：http://eri.fanxiaobao.xyz

[T37] Lua：字符串拼接
来源：http://cee.yuxming.cn

"a" .. "b"
来源：http://dya.zhengqikj.top

[T38] Lua：条件
来源：http://efs.vqdsnc.cn

if x > 0 then print("正") end
来源：http://pmk.snrcjt.cn

[T39] Lua：模式匹配
来源：http://cez.chenlongwang.top

string.find(s, "%d+")
来源：http://ios.gotoacloud.top

[T40] Lua：元表
来源：http://zco.yonumen.top

setmetatable({}, { __index = base })
来源：http://idh.pengpengdd.cyou

[T41] Perl：Hello World
来源：http://lrj.xinyue.icu

print "Hello\n";
来源：http://eny.uphjek.com

[T42] Perl：变量类型
来源：http://mut.hysaishi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://juv.jyoumei.cn

[T43] Perl：字符串插值
来源：http://aok.jinqigufen.top

"值: $a"
来源：http://eph.ydjk.org.cn

[T44] Perl：条件
来源：http://xcb.nwbrower.top

if ($a > 0) { print "正"; }
来源：http://nhl.yuanzhike.top

[T45] Perl：数组遍历
来源：http://irs.c1oappe.top

for my $x (@arr) { print $x; }
来源：http://mpz.jiagoushi.top

[T46] Perl：哈希操作
来源：http://vgu.zhengqikj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wom.yangfankeji.com

[T47] Perl：正则捕获
来源：http://nia.dashuyun.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://eav.hammf.cn

[T48] Perl：正则替换
来源：http://tca.nanxinkj.top

$s =~ s/old/new/g;
来源：http://jlp.fktsv.cn

[T49] Perl：函数
来源：http://xit.sysykeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sdn.shzxlz.cn

[T50] Perl：逐行读文件
来源：http://rwb.yj20258.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dzy.yueranfly.top

while (my $line = <$fh>) { print $line; }
来源：http://kkm.cdnleiting.top

[T51] Scala：Hello World
来源：http://nfs.dianchejie.cn

println("Hello")
来源：http://nrl.xuanzx.com

[T52] Scala：变量
来源：http://iax.cucudq.cn

val a = 1;  var b = 2
来源：http://tul.yj20258.top

[T53] Scala：字符串插值
来源：http://mtx.xziqi.cn

s"值: $b"
来源：http://iae.gzhubu.top

[T54] Scala：集合映射
来源：http://xda.yfazqb.com

List(1, 2, 3).map(_ * 2)
来源：http://jwo.zhoulong.xyz

[T55] Scala：集合过滤
来源：http://dlh.xingfuxueyuan.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://yfy.jinqigfzy.top

[T56] Scala：样例类
来源：http://qaw.smart0.xyz

case class User(name: String, age: Int)
来源：http://lub.cashguo.top

[T57] Scala：模式匹配
来源：http://gyj.wangshuangyany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qzz.cashguo.top

[T58] Scala：函数定义
来源：http://pga.gogol.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lfn.yangfankeji.com

[T59] Scala：循环
来源：http://nsn.wangshuangyany.cn

for (i <- 1 to 10) println(i)
来源：http://bas.hnxiangtu.top

[T60] Scala：折叠
来源：http://wng.ydzc1.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tas.nwbrower.top

================================================================================
来源：http://zku.yongpay.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nlp.zhaomingkeji.xyz

================================================================================
来源：http://jhn.0kj1m.cn

[U01] Py：创建虚拟环境
来源：http://sah.vqdsnc.cn

python -m venv .venv && source .venv/bin/activate
来源：http://opb.gogol.net.cn

[U02] Py：导出 / 安装依赖
来源：http://wgl.shanyushiyangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qhr.epnwcf.com

[U03] Py：加载 .env 配置
来源：http://qfs.meibo888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://bst.zhoulong.xyz

[U04] Py：变量调试打印
来源：http://udk.zhijiandao.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xza.fehbvm.com

[U05] Py：列表去重且保序
来源：http://znz.aizwys.cn

list(dict.fromkeys(arr))
来源：http://ogu.gzhubu.top

[U06] Py：合并两个字典
来源：http://bcu.dashuyun.cn

{**a, **b}
来源：http://niq.xylfe.cn

[U07] Py：反转字典键值
来源：http://odc.zhijiandao.cn

{v: k for k, v in d.items()}
来源：http://xyc.feifeiyinyue.top

[U08] Py：展平二维列表
来源：http://glc.52xcode.cn

[y for x in nested for y in x]
来源：http://kvo.sysykeji.top

[U09] Py：字典取最大值的键
来源：http://dzi.sufxvd.cn

max(d, key=d.get)
来源：http://crp.yfazqb.com

[U10] Py：按值排序字典
来源：http://oxg.shangyingyoupin.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jgs.xziqi.cn

[U11] Py：生成器表达式
来源：http://zbz.redwolf501.top

(x * 2 for x in arr)
来源：http://ruq.redwolf501.top

[U12] Py：取出现最多的 3 个元素
来源：http://yra.jinyuanbaomall.cn

Counter(arr).most_common(3)
来源：http://voc.fanxiaobao.xyz

[U13] Py：固定长度队列
来源：http://tpc.yvedp.cn

deque(maxlen=10)
来源：http://wmu.sxryk.cn

[U14] Py：分组收集到列表
来源：http://ooq.0kj1m.cn

defaultdict(list)
来源：http://ylp.wangshuangyany.cn

[U15] Py：高精度计时
来源：http://gps.fehbvm.com

t = time.perf_counter()
来源：http://hsr.hongshengwenyu.top

[U16] Py：命令行参数解析
来源：http://kle.yj20258888.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lcg.52xcode.cn

[U17] Py：初始化日志
来源：http://jxl.gzhubu.top

logging.basicConfig(level=logging.INFO)
来源：http://tvg.jianghu66.top

[U18] Py：预编译正则
来源：http://xkg.hnqzz.top

pat = re.compile(r"\d+")
来源：http://orp.shanyushiyangtech.top

[U19] Py：正则替换带回调
来源：http://jno.hcnkem.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tpy.jianghu66.top

[U20] Py：缓存函数结果
来源：http://uzv.jinghuilouyu.cn

@functools.lru_cache(maxsize=None)
来源：http://uyu.ydjk.org.cn

[U21] Py：自定义上下文管理器
来源：http://siv.bbcook.cn

@contextlib.contextmanager
来源：http://qor.sufxvd.cn

[U22] Py：矩阵转置
来源：http://xiz.cqqwz.cn

list(zip(*m))
来源：http://ckh.chenlongwang.top

[U23] Py：分块读取大文件
来源：http://tke.ybcxt.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mva.tanke756.top

[U24] Py：路径操作
来源：http://jpp.bjfxy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jzi.zhijiandao.cn

[U25] Py：CSV 按字典读
来源：http://bnh.jlsjyb.cn

csv.DictReader(f)
来源：http://bpw.shzxlz.cn

[U26] Py：并发下载
来源：http://svq.hammf.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ncy.ydzc1.top

[U27] Py：异步 HTTP
来源：http://ons.sxryk.cn

aiohttp.ClientSession() 配合 async with
来源：http://ewn.sxryk.cn

[U28] Py：类型别名
来源：http://ujy.wangshuangyany.cn

UserId = int
来源：http://pjr.meibo888.top

[U29] Py：属性校验
来源：http://kwa.yanxiufei.cn

@property 与 @x.setter 配合
来源：http://dtw.ywan-chungtsiang.top

[U30] Py：数据类
来源：http://url.gotoacloud.top

@dataclass(slots=True)
来源：http://adj.birdmap.top

[U31] Py：单测
来源：http://rfg.tian-w.cn

python -m pytest -q
来源：http://rpj.zhoulong.xyz

[U32] Py：代码格式化
来源：http://vgm.yj20258888.top

ruff format . && ruff check --fix .
来源：http://szl.hammf.cn

[U33] Py：打包发布
来源：http://zis.shzxlz.cn

python -m build  （依赖 pyproject.toml）
来源：http://rvx.yuanzhike.top

[U34] Py：判断编码
来源：http://ezu.ydzc1.top

chardet.detect(raw)
来源：http://ldk.ydzc1.top

[U35] Py：发送邮件
来源：http://ttd.yangfankeji.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oef.yvedp.cn

[U36] Py：定时任务
来源：http://fhw.redwolf501.top

schedule.every(10).minutes.do(job)
来源：http://lei.svipenyu.cn

[U37] Py：读写 Excel
来源：http://fnz.ydzc1.top

pandas.read_excel / DataFrame.to_excel
来源：http://ebu.hnxiangtu.top

[U38] Py：获取脚本所在目录
来源：http://pdo.hammf.cn

Path(__file__).resolve().parent
来源：http://xnm.wangdashe.top

[U39] Py：判断是否在交互环境
来源：http://fda.epnwcf.com

sys.stdout.isatty()
来源：http://wgf.yanxiufei.cn

[U40] Py：打印到标准错误
来源：http://ugj.shanyushiyangtech.top

print("err", file=sys.stderr)
来源：http://cmx.ivvv.top

[U41] PHP：初始化 Composer 项目
来源：http://npr.aibaodan.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bed.jinqigfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://dtl.hesvh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gxl.jinghuilouyu.cn

[U43] PHP：声明命名空间
来源：http://ncj.c1oappe.top

namespace App\Http;
来源：http://civ.jyoumei.cn

[U44] PHP：开启严格类型
来源：http://kzt.kuanghao11.cn

declare(strict_types=1);
来源：http://pzs.zhoulong.xyz

[U45] PHP：类型声明与返回类型
来源：http://nwp.ivvv.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://riy.yueranfly.top

[U46] PHP：可空类型
来源：http://dmi.xziqi.cn

?string $name = null
来源：http://del.ehwqpu.com

[U47] PHP：联合类型
来源：http://txs.hongshengwenyu.top

int|string $id
来源：http://kmn.cdnleiting.top

[U48] PHP：纯枚举
来源：http://oaf.hywenlv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pew.nanxuanxn.top

[U49] PHP：只读属性
来源：http://map.yongpay.top

public readonly string $name
来源：http://cbg.hnqzz.top

[U50] PHP：构造器属性提升
来源：http://hte.cucudq.cn

public function __construct(private int $id) {}
来源：http://vvy.hammf.cn

[U51] PHP：数组解构
来源：http://fli.mhx1999.top

[$a, $b] = $arr;
来源：http://oqq.ydzc1.top

[U52] PHP：箭头函数
来源：http://tky.kuanghao11.cn

$double = fn($x) => $x * 2;
来源：http://gbl.sxryk.cn

[U53] PHP：空合并运算符
来源：http://ojr.daria6918.cn

$v = $a ?? $b ?? "default";
来源：http://lfh.xylfe.cn

[U54] PHP：空安全调用
来源：http://nze.zhixingplan.top

$obj?->method()
来源：http://zfh.wangdashe.top

[U55] PHP：match 表达式
来源：http://bqd.xylfe.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tka.bjfxy.top

[U56] PHP：命名参数
来源：http://slr.birdmap.top

f(a: 1, b: 2)
来源：http://zko.hesvh.cn

[U57] PHP：字符串插值
来源：http://xgs.gaohongyu789.top

"值: {$a}"
来源：http://hyn.redwolf501.top

[U58] PHP：数组三件套
来源：http://xat.dianchejie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zdi.daria6918.cn

[U59] PHP：自定义排序
来源：http://qig.nwbrower.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pki.redwolf501.top

[U60] PHP：JSON 编解码
来源：http://vbl.shanyushiyangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hyx.snrcjt.cn

[U61] PHP：正则
来源：http://zda.zhijiandao.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://opv.zdqjudy.top

[U62] PHP：日期对象
来源：http://keu.havefunace.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qrp.jlsjyb.cn

[U63] PHP：文件读写
来源：http://mgm.gogol.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gsp.quarkkingdee.top

[U64] PHP：目录遍历
来源：http://tmr.hammf.cn

glob("dir/*.php");  scandir("dir");
来源：http://gvl.shuidangran.top

[U65] PHP：会话
来源：http://zal.shanyushiyangtech.top

session_start();  $_SESSION["uid"] = 1;
来源：http://tyw.gogol.net.cn

[U66] PHP：设置 Cookie
来源：http://fcy.tian-w.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ohw.ppjwa.cn

[U67] PHP：处理文件上传
来源：http://ted.ywan-chungtsiang.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pwx.pengpengdd.cyou

[U68] PHP：PDO 连接
来源：http://apo.9152youxi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ryq.tanke756.top

[U69] PHP：PDO 预处理
来源：http://boo.chenlongwang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://aza.jinyuanbaomall.cn

[U70] PHP：PDO 事务
来源：http://fof.chenjidiqi.icu

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gfq.dashuyun.cn

[U71] PHP：抛出异常
来源：http://mcs.yfazqb.com

throw new RuntimeException("失败", 500);
来源：http://gxe.quarkkingdee.top

[U72] PHP：写错误日志
来源：http://usf.zhoulong.xyz

error_log("失败: " . $e->getMessage());
来源：http://srl.aibaodan.cn

[U73] PHP：读取 ini 配置
来源：http://pci.xingfuxueyuan.xyz

parse_ini_file("config.ini", true)
来源：http://dnv.yvedp.cn

[U74] PHP：读取环境变量
来源：http://tux.xuetiantiany.cn

getenv("APP_ENV") ?: "production"
来源：http://dsq.smart0.xyz

[U75] PHP：依赖注入
来源：http://xgc.zdbjq.cn

composer require psr/container
来源：http://vux.jinghuilouyu.cn

[U76] PHP：简单路由
来源：http://qfx.aibaodan.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rrq.feifeiyinyue.top

[U77] PHP：模板渲染
来源：http://nix.cucudq.cn

composer require twig/twig
来源：http://ugs.sxryk.cn

[U78] PHP：单元测试
来源：http://eku.ydzc1.top

composer require --dev phpunit/phpunit
来源：http://mcn.gotoacloud.top

[U79] PHP：静态分析
来源：http://uwm.fktsv.cn

composer require --dev phpstan/phpstan
来源：http://qjx.yonumen.top

[U80] PHP：代码规范修复
来源：http://vjy.tanke756.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qxm.sjlbkw.cn

[U81] JS：初始化项目
来源：http://ofj.c1oappe.top

npm init -y;  npm i express
来源：http://iby.xinyue.icu

[U82] JS：package.json 脚本
来源：http://kca.xuetiantiany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jdb.pengpengdd.cyou

[U83] JS：ES Module 导入导出
来源：http://ees.wangdashe.top

export const a = 1;  import { a } from "./m.js";
来源：http://zmh.hnqzz.top

[U84] JS：CommonJS 写法
来源：http://wed.bjfxy.top

module.exports = { a };  const { a } = require("./m");
来源：http://ino.birdmap.top

[U85] JS：可选链
来源：http://toc.cheryme.top

a?.b?.c
来源：http://dtf.cashguo.top

[U86] JS：空值合并
来源：http://rlr.gotoacloud.top

a ?? b
来源：http://ejk.snrcjt.cn

[U87] JS：解构默认值
来源：http://jhe.chenlongwang.top

const { a = 1, b = 2 } = obj;
来源：http://ljj.shangyingyoupin.top

[U88] JS：对象展开合并
来源：http://mrf.jiagoushi.top

{ ...a, ...b }
来源：http://bvp.tian-w.cn


<!-- 参考信息 -->