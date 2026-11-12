代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://xyk.guannengcc.top

[S59] C++：静态断言
来源：http://sts.ehwqpu.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://khf.sysykeji.top

[S60] C++：遍历并删除元素
来源：http://jmw.sxryk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://skl.yuanzhike.top

================================================================================
来源：http://rhp.yuanzhike.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lfv.sysykeji.top

================================================================================
来源：http://hvw.tarul.cn

[T01] Kotlin：Hello World
来源：http://khe.nanxinkj.top

println("Hello")
来源：http://jxw.gogol.net.cn

[T02] Kotlin：变量
来源：http://blz.xingfuxueyuan.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hty.nanxinkj.top

[T03] Kotlin：字符串模板
来源：http://yok.tanke756.top

"值: $b"
来源：http://wsk.fktsv.cn

[T04] Kotlin：空安全
来源：http://yoh.quarkkingdee.top

val n: String? = null;  n?.length
来源：http://tdl.aizwys.cn

[T05] Kotlin：when 表达式
来源：http://mdm.316326.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kny.hywenlv.cn

[T06] Kotlin：集合映射
来源：http://knh.uphjek.com

listOf(1, 2, 3).map { it * 2 }
来源：http://ucd.ctjpmb.com

[T07] Kotlin：集合过滤
来源：http://ccv.redwolf501.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://oen.zdqjudy.top

[T08] Kotlin：数据类
来源：http://bhv.ydzc1.top

data class User(val name: String, val age: Int)
来源：http://xbx.ehwqpu.com

[T09] Kotlin：扩展函数
来源：http://wkf.tianlin.xyz

fun String.exclaim() = this + "!"
来源：http://lcm.shuidangran.top

[T10] Kotlin：默认参数
来源：http://dvy.zhoulong.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://mat.jinqigufen.top

[T11] Kotlin：协程
来源：http://onp.guowangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hht.wangshuangyany.cn

[T12] Kotlin：解构声明
来源：http://hlu.yangfankeji.com

val (a, b) = Pair(1, 2)
来源：http://lzn.hnqzz.top

[T13] Kotlin：只读 Map
来源：http://tii.zhaomingkeji.xyz

val m = mapOf("a" to 1)
来源：http://jbo.smart0.xyz

[T14] Kotlin：循环
来源：http://ihr.chenzaomai.com

for (i in 1..10) println(i)
来源：http://sut.tanke756.top

[T15] Kotlin：接口
来源：http://shn.yvedp.cn

interface Shape { fun area(): Double }
来源：http://nty.yonumen.top

[T16] Swift：Hello World
来源：http://ixh.hywenlv.cn

print("Hello")
来源：http://zst.tanke756.top

[T17] Swift：变量与常量
来源：http://puh.ehwqpu.com

var a = 1;  let b = 2
来源：http://lcu.wangdashe.top

[T18] Swift：字符串插值
来源：http://fnr.hcnkem.com

"值: \(b)"
来源：http://eza.hnqzz.top

[T19] Swift：可选绑定
来源：http://oja.yuanzhike.top

if let n = opt { print(n) }
来源：http://tuf.fktsv.cn

[T20] Swift：数组操作
来源：http://pct.yueranfly.top

var a = [1, 2, 3];  a.append(4)
来源：http://vhy.yj20258888.top

[T21] Swift：遍历
来源：http://squ.wangshuangyany.cn

for x in a { print(x) }
来源：http://fsn.sysykeji.top

[T22] Swift：字典
来源：http://mtz.sysykeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://zuv.dashuyun.cn

[T23] Swift：函数
来源：http://hdb.quarkkingdee.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tbh.hesvh.cn

[T24] Swift：闭包
来源：http://jnn.fzhhl.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lgr.pycfn.com

[T25] Swift：结构体
来源：http://ild.jqgufenzy.top

struct P { var x: Int }
来源：http://lfw.ivvv.top

[T26] Swift：类与重写
来源：http://lzf.mhx1999.top

class A: Base { override func f() {} }
来源：http://ikl.sxryk.cn

[T27] Swift：错误处理
来源：http://kmi.smart0.xyz

do { try f() } catch { print(error) }
来源：http://pbm.jyoumei.cn

[T28] Swift：枚举
来源：http://med.aibaodan.cn

enum Color { case red, green }
来源：http://ngi.jyoumei.cn

[T29] Swift：guard 提前返回
来源：http://mkb.smart0.xyz

guard let x = opt else { return }
来源：http://oer.aibaodan.cn

[T30] Swift：协议
来源：http://wkd.vehdjk.com

protocol Shape { func area() -> Double }
来源：http://vqk.yuanzhike.top

[T31] Lua：Hello World
来源：http://rxd.xuetiantiany.cn

print("Hello")
来源：http://jgx.hesvh.cn

[T32] Lua：局部变量
来源：http://uzl.cdnleiting.top

local a = 1
来源：http://ngj.quarkkingdee.top

[T33] Lua：表（数组）
来源：http://asf.tarul.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rii.yvedp.cn

[T34] Lua：遍历表
来源：http://yzi.hesvh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://aip.vehdjk.com

[T35] Lua：字典表
来源：http://yjx.meibo888.top

local d = { a = 1 };  d.b = 2
来源：http://lpb.sweek.top

[T36] Lua：函数
来源：http://jcy.shanyushiyangkeji.top

function add(a, b) return a + b end
来源：http://zvb.aibaodan.cn

[T37] Lua：字符串拼接
来源：http://dhn.pycfn.com

"a" .. "b"
来源：http://qsr.dashuyun.cn

[T38] Lua：条件
来源：http://pvv.jinqigfzy.top

if x > 0 then print("正") end
来源：http://qov.cdnleiting.top

[T39] Lua：模式匹配
来源：http://kzp.fzhhl.top

string.find(s, "%d+")
来源：http://srj.yj202588.top

[T40] Lua：元表
来源：http://vmg.yuxming.cn

setmetatable({}, { __index = base })
来源：http://pbr.nwbrower.top

[T41] Perl：Hello World
来源：http://npa.xuetiantiany.cn

print "Hello\n";
来源：http://dew.cqqwz.cn

[T42] Perl：变量类型
来源：http://sna.chenjidiqi.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jce.hnqzz.top

[T43] Perl：字符串插值
来源：http://jpe.ywan-chungtsiang.top

"值: $a"
来源：http://xfn.hywenlv.cn

[T44] Perl：条件
来源：http://gfz.nwbrower.top

if ($a > 0) { print "正"; }
来源：http://dzc.wangdashe.top

[T45] Perl：数组遍历
来源：http://lnh.sxryk.cn

for my $x (@arr) { print $x; }
来源：http://qlz.wangshuangyany.cn

[T46] Perl：哈希操作
来源：http://xct.yanxiufei.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nxi.xingfuxueyuan.xyz

[T47] Perl：正则捕获
来源：http://yci.cheryme.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://axb.yongpay.top

[T48] Perl：正则替换
来源：http://uvm.vqdsnc.cn

$s =~ s/old/new/g;
来源：http://lms.aibaodan.cn

[T49] Perl：函数
来源：http://jej.nanxuanxn.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cal.hysaishi.cn

[T50] Perl：逐行读文件
来源：http://zbi.cucudq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jqz.nanxinkj.top

while (my $line = <$fh>) { print $line; }
来源：http://ddk.nanxuanxn.top

[T51] Scala：Hello World
来源：http://jso.zycfv.cn

println("Hello")
来源：http://hut.sjlbkw.cn

[T52] Scala：变量
来源：http://pph.yonumen.top

val a = 1;  var b = 2
来源：http://bhb.svipenyu.cn

[T53] Scala：字符串插值
来源：http://szq.yj202588.top

s"值: $b"
来源：http://wvu.ctjpmb.com

[T54] Scala：集合映射
来源：http://xcy.cheryme.top

List(1, 2, 3).map(_ * 2)
来源：http://lub.yvedp.cn

[T55] Scala：集合过滤
来源：http://mde.jqgufenzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://yly.redwolf501.top

[T56] Scala：样例类
来源：http://iwd.kuanghao11.cn

case class User(name: String, age: Int)
来源：http://vyb.wangdashe.top

[T57] Scala：模式匹配
来源：http://czk.ydjk.org.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ttv.fengsongda.top

[T58] Scala：函数定义
来源：http://eue.hcnkem.com

def add(a: Int, b: Int): Int = a + b
来源：http://jnv.gotoacloud.top

[T59] Scala：循环
来源：http://mqf.yj20258888.top

for (i <- 1 to 10) println(i)
来源：http://pgt.vehdjk.com

[T60] Scala：折叠
来源：http://jxd.jqgufenzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ujb.yj20258888.top

================================================================================
来源：http://xta.snrcjt.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://llb.jqgfzy.top

================================================================================
来源：http://nnd.chenlongwang.top

[U01] Py：创建虚拟环境
来源：http://pao.epnwcf.com

python -m venv .venv && source .venv/bin/activate
来源：http://fyv.sufxvd.cn

[U02] Py：导出 / 安装依赖
来源：http://suo.ybcxt.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://coi.daxiang520.top

[U03] Py：加载 .env 配置
来源：http://kpg.sjlbkw.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://udz.zhiwuduotai.top

[U04] Py：变量调试打印
来源：http://woc.xuanzx.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lhf.fktsv.cn

[U05] Py：列表去重且保序
来源：http://iii.xylfe.cn

list(dict.fromkeys(arr))
来源：http://yfc.hywenlv.cn

[U06] Py：合并两个字典
来源：http://jjd.cheryme.top

{**a, **b}
来源：http://tsl.yvedp.cn

[U07] Py：反转字典键值
来源：http://swk.xziqi.cn

{v: k for k, v in d.items()}
来源：http://wrx.wangdashe.top

[U08] Py：展平二维列表
来源：http://tem.pengpengdd.cyou

[y for x in nested for y in x]
来源：http://ezf.cashguo.top

[U09] Py：字典取最大值的键
来源：http://gga.tian-w.cn

max(d, key=d.get)
来源：http://vkq.fzhhl.top

[U10] Py：按值排序字典
来源：http://opx.yonumen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tut.xziqi.cn

[U11] Py：生成器表达式
来源：http://kxn.yangfankeji.com

(x * 2 for x in arr)
来源：http://dfu.hysaishi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ouu.sufxvd.cn

Counter(arr).most_common(3)
来源：http://yan.pycfn.com

[U13] Py：固定长度队列
来源：http://hki.cdnleiting.top

deque(maxlen=10)
来源：http://pff.shuidangran.top

[U14] Py：分组收集到列表
来源：http://xqb.jinghuilouyu.cn

defaultdict(list)
来源：http://phl.uphjek.com

[U15] Py：高精度计时
来源：http://aax.jiagoushi.top

t = time.perf_counter()
来源：http://flk.redwolf501.top

[U16] Py：命令行参数解析
来源：http://kgn.feifeiyinyue.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wzy.hongshengwenyu.top

[U17] Py：初始化日志
来源：http://zxq.ctjpmb.com

logging.basicConfig(level=logging.INFO)
来源：http://awl.redwolf501.top

[U18] Py：预编译正则
来源：http://ssp.sxryk.cn

pat = re.compile(r"\d+")
来源：http://gas.shanyushiyangkeji.top

[U19] Py：正则替换带回调
来源：http://gjo.aibaodan.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kxr.zdbjq.cn

[U20] Py：缓存函数结果
来源：http://adn.daxiang520.top

@functools.lru_cache(maxsize=None)
来源：http://mdw.sxryk.cn

[U21] Py：自定义上下文管理器
来源：http://jdt.jinqigfzy.top

@contextlib.contextmanager
来源：http://sla.zhixingplan.top

[U22] Py：矩阵转置
来源：http://djc.sweek.top

list(zip(*m))
来源：http://jku.iojbl.cn

[U23] Py：分块读取大文件
来源：http://xbm.nwbrower.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gag.epnwcf.com

[U24] Py：路径操作
来源：http://rgs.chenjidiqi.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://edk.tanke756.top

[U25] Py：CSV 按字典读
来源：http://rpl.xziqi.cn

csv.DictReader(f)
来源：http://mtz.snrcjt.cn

[U26] Py：并发下载
来源：http://cra.fehbvm.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xbv.nwbrower.top

[U27] Py：异步 HTTP
来源：http://ern.xuanzx.com

aiohttp.ClientSession() 配合 async with
来源：http://pgg.hongshengwenyu.top

[U28] Py：类型别名
来源：http://zwp.chenzaomai.com

UserId = int
来源：http://piz.epnwcf.com

[U29] Py：属性校验
来源：http://vvx.nanxuanxn.top

@property 与 @x.setter 配合
来源：http://pll.52xcode.cn

[U30] Py：数据类
来源：http://vcm.jinyuanbaomall.cn

@dataclass(slots=True)
来源：http://dnk.yanxiufei.cn

[U31] Py：单测
来源：http://gam.ehwqpu.com

python -m pytest -q
来源：http://jom.jqgfzy.top

[U32] Py：代码格式化
来源：http://rzp.birdmap.top

ruff format . && ruff check --fix .
来源：http://mda.zhiwuduotai.top

[U33] Py：打包发布
来源：http://ofa.vqdsnc.cn

python -m build  （依赖 pyproject.toml）
来源：http://cxk.jyoumei.cn

[U34] Py：判断编码
来源：http://acs.cqqwz.cn

chardet.detect(raw)
来源：http://xfr.andypj.xyz

[U35] Py：发送邮件
来源：http://hsw.ctjpmb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mfu.cdnleiting.top

[U36] Py：定时任务
来源：http://yld.0kj1m.cn

schedule.every(10).minutes.do(job)
来源：http://siy.hnqzz.top

[U37] Py：读写 Excel
来源：http://rco.hesvh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yfl.jinqigufen.top

[U38] Py：获取脚本所在目录
来源：http://ggf.bbcook.cn

Path(__file__).resolve().parent
来源：http://kla.jyoumei.cn

[U39] Py：判断是否在交互环境
来源：http://ldb.kuanghao11.cn

sys.stdout.isatty()
来源：http://ylr.ctjpmb.com

[U40] Py：打印到标准错误
来源：http://vpa.yj20258888.top

print("err", file=sys.stderr)
来源：http://ang.yj202588.top

[U41] PHP：初始化 Composer 项目
来源：http://kxq.sxryk.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gvs.feifeiyinyue.top

[U42] PHP：PSR-4 自动加载
来源：http://sjc.hongshengwenyu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xye.jyoumei.cn

[U43] PHP：声明命名空间
来源：http://mup.shanyushiyangkeji.top

namespace App\Http;
来源：http://ykl.zhiwuduotai.top

[U44] PHP：开启严格类型
来源：http://jtq.wangshuangyany.cn

declare(strict_types=1);
来源：http://rlh.guannengcc.top

[U45] PHP：类型声明与返回类型
来源：http://cqq.tanke756.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xea.cashguo.top

[U46] PHP：可空类型
来源：http://uys.hywenlv.cn

?string $name = null
来源：http://vdq.tianlin.xyz

[U47] PHP：联合类型
来源：http://jgl.dashuyun.cn

int|string $id
来源：http://lry.epnwcf.com

[U48] PHP：纯枚举
来源：http://puq.316326.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xvl.jinghuilouyu.cn

[U49] PHP：只读属性
来源：http://okp.hnxiangtu.top

public readonly string $name
来源：http://tht.andypj.xyz

[U50] PHP：构造器属性提升
来源：http://fvc.gogol.net.cn

public function __construct(private int $id) {}
来源：http://knw.havefunace.top

[U51] PHP：数组解构
来源：http://fau.ivvv.top

[$a, $b] = $arr;
来源：http://fqi.ybcxt.top

[U52] PHP：箭头函数
来源：http://vcf.nwbrower.top

$double = fn($x) => $x * 2;
来源：http://wol.fengsongda.top

[U53] PHP：空合并运算符
来源：http://roe.jqgfzy.top

$v = $a ?? $b ?? "default";
来源：http://ovh.xuetiantiany.cn

[U54] PHP：空安全调用
来源：http://zgx.wangdashe.top

$obj?->method()
来源：http://uaz.pengpengdd.cyou

[U55] PHP：match 表达式
来源：http://vnm.yuanzhike.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wxk.cucudq.cn

[U56] PHP：命名参数
来源：http://tkr.fengsongda.top

f(a: 1, b: 2)
来源：http://peo.zhijiandao.cn

[U57] PHP：字符串插值
来源：http://ybm.sysykeji.top

"值: {$a}"
来源：http://rdd.jinyuanbaomall.cn

[U58] PHP：数组三件套
来源：http://fpq.epnwcf.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gqx.xingfuxueyuan.xyz

[U59] PHP：自定义排序
来源：http://btd.tarul.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dps.hnxiangtu.top

[U60] PHP：JSON 编解码
来源：http://gyd.gaohongyu789.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qhz.feifeiyinyue.top

[U61] PHP：正则
来源：http://imc.hywenlv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ucw.iojbl.cn

[U62] PHP：日期对象
来源：http://zvc.birdmap.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dfb.guannengcc.top

[U63] PHP：文件读写
来源：http://vrd.fanxiaobao.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bia.zhongyouzk.top

[U64] PHP：目录遍历
来源：http://mlv.yangfankeji.com

glob("dir/*.php");  scandir("dir");
来源：http://ogm.0kj1m.cn

[U65] PHP：会话
来源：http://esf.tianlin.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://pqk.jqgfzy.top

[U66] PHP：设置 Cookie
来源：http://yrk.aizwys.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fun.hesvh.cn

[U67] PHP：处理文件上传
来源：http://fct.shzxlz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ykk.hysaishi.cn

[U68] PHP：PDO 连接
来源：http://wbq.ydzc1.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wgv.jiagoushi.top

[U69] PHP：PDO 预处理
来源：http://xmk.jiagoushi.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://icz.zdqjudy.top

[U70] PHP：PDO 事务
来源：http://nnt.cheryme.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rcg.ywan-chungtsiang.top

[U71] PHP：抛出异常
来源：http://uwi.jinyuanbaomall.cn

throw new RuntimeException("失败", 500);
来源：http://zek.yongpay.top

[U72] PHP：写错误日志
来源：http://rmr.yfazqb.com

error_log("失败: " . $e->getMessage());
来源：http://eih.yuanzhike.top

[U73] PHP：读取 ini 配置
来源：http://fck.smart0.xyz

parse_ini_file("config.ini", true)
来源：http://hbv.daxiang520.top

[U74] PHP：读取环境变量
来源：http://uab.yangfankeji.com

getenv("APP_ENV") ?: "production"
来源：http://ksp.haohaochexian.top

[U75] PHP：依赖注入
来源：http://vbv.andypj.xyz

composer require psr/container
来源：http://ras.zhijiandao.cn

[U76] PHP：简单路由
来源：http://hwl.vqdsnc.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ogp.hysaishi.cn

[U77] PHP：模板渲染
来源：http://gsr.0kj1m.cn

composer require twig/twig
来源：http://utu.hammf.cn

[U78] PHP：单元测试
来源：http://pzs.cucudq.cn

composer require --dev phpunit/phpunit
来源：http://dwx.ehwqpu.com

[U79] PHP：静态分析
来源：http://yya.hongshengwenyu.top

composer require --dev phpstan/phpstan
来源：http://zql.gogol.net.cn

[U80] PHP：代码规范修复
来源：http://xyq.0kj1m.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bxo.chenjidiqi.icu

[U81] JS：初始化项目
来源：http://imq.meibo888.top

npm init -y;  npm i express
来源：http://rae.ydjk.org.cn

[U82] JS：package.json 脚本
来源：http://cze.pengpengdd.cyou

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xyh.yuxming.cn

[U83] JS：ES Module 导入导出
来源：http://zcl.yuxming.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xps.zhaomingkeji.xyz

[U84] JS：CommonJS 写法
来源：http://fqn.dashuyun.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wuu.hnqzz.top


<!-- 参考信息 -->