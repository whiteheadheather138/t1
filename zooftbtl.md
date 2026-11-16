代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hgd.nwbrower.top

[S57] C++：编译期常量
来源：http://ctv.jqgufenzy.top

constexpr int N = 10;
来源：http://fiv.fanxiaobao.xyz

[S58] C++：命名空间
来源：http://xya.gotoacloud.top

namespace ns { int f() { return 1; } }
来源：http://lhy.guannengcc.top

[S59] C++：静态断言
来源：http://fas.sufxvd.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://scf.c1oappe.top

[S60] C++：遍历并删除元素
来源：http://qvg.jinqigfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xlg.pengpengdd.cyou

================================================================================
来源：http://nav.tarul.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nla.gogol.net.cn

================================================================================
来源：http://vte.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://hkz.nanxinkj.top

println("Hello")
来源：http://xof.nanxuanxn.top

[T02] Kotlin：变量
来源：http://wvh.yueranfly.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://coz.ybcxt.top

[T03] Kotlin：字符串模板
来源：http://erm.ywan-chungtsiang.top

"值: $b"
来源：http://fff.ctjpmb.com

[T04] Kotlin：空安全
来源：http://mhz.xuanzx.com

val n: String? = null;  n?.length
来源：http://gxh.meibo888.top

[T05] Kotlin：when 表达式
来源：http://kxo.fktsv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iil.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://quo.xuanzx.com

listOf(1, 2, 3).map { it * 2 }
来源：http://lwi.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://kox.gzhubu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hkh.yvedp.cn

[T08] Kotlin：数据类
来源：http://jus.wangshuangyany.cn

data class User(val name: String, val age: Int)
来源：http://xal.shzxlz.cn

[T09] Kotlin：扩展函数
来源：http://fas.fehbvm.com

fun String.exclaim() = this + "!"
来源：http://zqk.tianlin.xyz

[T10] Kotlin：默认参数
来源：http://gtd.wangshuangyany.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dvs.gogol.net.cn

[T11] Kotlin：协程
来源：http://fps.zhoulong.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://gkz.zhixingplan.top

[T12] Kotlin：解构声明
来源：http://bms.jinqigfzy.top

val (a, b) = Pair(1, 2)
来源：http://klo.yj20258.top

[T13] Kotlin：只读 Map
来源：http://wne.yonumen.top

val m = mapOf("a" to 1)
来源：http://zbw.xylfe.cn

[T14] Kotlin：循环
来源：http://gfn.jyoumei.cn

for (i in 1..10) println(i)
来源：http://spz.tianlin.xyz

[T15] Kotlin：接口
来源：http://ayy.svipenyu.cn

interface Shape { fun area(): Double }
来源：http://kdz.haohaochexian.top

[T16] Swift：Hello World
来源：http://dwh.yongpay.top

print("Hello")
来源：http://lni.tian-w.cn

[T17] Swift：变量与常量
来源：http://ehb.gogol.net.cn

var a = 1;  let b = 2
来源：http://mia.aizwys.cn

[T18] Swift：字符串插值
来源：http://zkr.sufxvd.cn

"值: \(b)"
来源：http://qaz.birdmap.top

[T19] Swift：可选绑定
来源：http://fvd.vehdjk.com

if let n = opt { print(n) }
来源：http://zkk.c1oappe.top

[T20] Swift：数组操作
来源：http://kba.cashguo.top

var a = [1, 2, 3];  a.append(4)
来源：http://cjt.jyoumei.cn

[T21] Swift：遍历
来源：http://crh.zhengqikj.top

for x in a { print(x) }
来源：http://pjx.xziqi.cn

[T22] Swift：字典
来源：http://mhn.chenjidiqi.icu

var d = ["a": 1];  d["b"] = 2
来源：http://ldr.zhongyouzk.top

[T23] Swift：函数
来源：http://emu.shanyushiyangtech.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kee.guowangkeji.top

[T24] Swift：闭包
来源：http://uao.guowangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ski.fanxiaobao.xyz

[T25] Swift：结构体
来源：http://rdh.ydjk.org.cn

struct P { var x: Int }
来源：http://tbm.hfpthk.cn

[T26] Swift：类与重写
来源：http://cgg.bjfxy.top

class A: Base { override func f() {} }
来源：http://kcb.xuetiantiany.cn

[T27] Swift：错误处理
来源：http://ond.chenzaomai.com

do { try f() } catch { print(error) }
来源：http://ksq.tian-w.cn

[T28] Swift：枚举
来源：http://hvw.vqdsnc.cn

enum Color { case red, green }
来源：http://rkd.xziqi.cn

[T29] Swift：guard 提前返回
来源：http://ovs.xylfe.cn

guard let x = opt else { return }
来源：http://fed.0kj1m.cn

[T30] Swift：协议
来源：http://vhe.hesvh.cn

protocol Shape { func area() -> Double }
来源：http://uds.yanxiufei.cn

[T31] Lua：Hello World
来源：http://irs.ydzc1.top

print("Hello")
来源：http://dgh.jqgfzy.top

[T32] Lua：局部变量
来源：http://pru.nanxuanxn.top

local a = 1
来源：http://yzp.mhx1999.top

[T33] Lua：表（数组）
来源：http://qwu.cashguo.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ipt.aibaodan.cn

[T34] Lua：遍历表
来源：http://pih.tian-w.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zcs.cucudq.cn

[T35] Lua：字典表
来源：http://afw.jinqigufen.top

local d = { a = 1 };  d.b = 2
来源：http://djf.yuanzhike.top

[T36] Lua：函数
来源：http://xwv.chenlongwang.top

function add(a, b) return a + b end
来源：http://sup.yj20258.top

[T37] Lua：字符串拼接
来源：http://jhm.yangfankeji.com

"a" .. "b"
来源：http://kpx.yfazqb.com

[T38] Lua：条件
来源：http://ytu.tian-w.cn

if x > 0 then print("正") end
来源：http://vam.cashguo.top

[T39] Lua：模式匹配
来源：http://egt.gotoacloud.top

string.find(s, "%d+")
来源：http://mzn.aibaodan.cn

[T40] Lua：元表
来源：http://khb.0kj1m.cn

setmetatable({}, { __index = base })
来源：http://ejx.jinqigufen.top

[T41] Perl：Hello World
来源：http://cyv.zhengqikj.top

print "Hello\n";
来源：http://inc.hongshengwenyu.top

[T42] Perl：变量类型
来源：http://mhv.dianchejie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vnc.jinqigfzy.top

[T43] Perl：字符串插值
来源：http://vas.shangyingyoupin.top

"值: $a"
来源：http://ixa.jiagoushi.top

[T44] Perl：条件
来源：http://vwz.cqqwz.cn

if ($a > 0) { print "正"; }
来源：http://eta.fanxiaobao.xyz

[T45] Perl：数组遍历
来源：http://buo.guannengcc.top

for my $x (@arr) { print $x; }
来源：http://puw.0kj1m.cn

[T46] Perl：哈希操作
来源：http://uls.zdbjq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kvj.gotoacloud.top

[T47] Perl：正则捕获
来源：http://iec.dashuyun.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ebo.wangdashe.top

[T48] Perl：正则替换
来源：http://ylj.andypj.xyz

$s =~ s/old/new/g;
来源：http://klz.fanxiaobao.xyz

[T49] Perl：函数
来源：http://hnt.ehwqpu.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ezl.haohaochexian.top

[T50] Perl：逐行读文件
来源：http://wob.9152youxi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pdu.vqdsnc.cn

while (my $line = <$fh>) { print $line; }
来源：http://erd.shuidangran.top

[T51] Scala：Hello World
来源：http://tnp.birdmap.top

println("Hello")
来源：http://bhy.ydjk.org.cn

[T52] Scala：变量
来源：http://rkp.jianghu66.top

val a = 1;  var b = 2
来源：http://icj.gogol.net.cn

[T53] Scala：字符串插值
来源：http://lid.yuanzhike.top

s"值: $b"
来源：http://ory.cashguo.top

[T54] Scala：集合映射
来源：http://hfo.gotoacloud.top

List(1, 2, 3).map(_ * 2)
来源：http://zyg.ehwqpu.com

[T55] Scala：集合过滤
来源：http://bdd.vqdsnc.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gnk.hysaishi.cn

[T56] Scala：样例类
来源：http://kmh.guowangkeji.top

case class User(name: String, age: Int)
来源：http://ksq.xinyue.icu

[T57] Scala：模式匹配
来源：http://zil.snrcjt.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wxq.iojbl.cn

[T58] Scala：函数定义
来源：http://xvh.zhixingplan.top

def add(a: Int, b: Int): Int = a + b
来源：http://jxm.jinqigufen.top

[T59] Scala：循环
来源：http://ggv.hammf.cn

for (i <- 1 to 10) println(i)
来源：http://qox.yongpay.top

[T60] Scala：折叠
来源：http://tqf.yj20258.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zxs.yonumen.top

================================================================================
来源：http://yxa.hysaishi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ygp.xinyue.icu

================================================================================
来源：http://jdq.bbcook.cn

[U01] Py：创建虚拟环境
来源：http://lpu.zhengqikj.top

python -m venv .venv && source .venv/bin/activate
来源：http://uzt.zhengqikj.top

[U02] Py：导出 / 安装依赖
来源：http://uro.nwbrower.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uva.xinyue.icu

[U03] Py：加载 .env 配置
来源：http://jix.sjlbkw.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tel.jlsjyb.cn

[U04] Py：变量调试打印
来源：http://jex.epnwcf.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://psb.ctjpmb.com

[U05] Py：列表去重且保序
来源：http://iqo.zhijiandao.cn

list(dict.fromkeys(arr))
来源：http://xwi.sufxvd.cn

[U06] Py：合并两个字典
来源：http://lpn.pycfn.com

{**a, **b}
来源：http://rwa.nanxuanxn.top

[U07] Py：反转字典键值
来源：http://gdi.xinyue.icu

{v: k for k, v in d.items()}
来源：http://ogv.snrcjt.cn

[U08] Py：展平二维列表
来源：http://hfo.yonumen.top

[y for x in nested for y in x]
来源：http://enm.cucudq.cn

[U09] Py：字典取最大值的键
来源：http://hgz.cqqwz.cn

max(d, key=d.get)
来源：http://pcf.jiagoushi.top

[U10] Py：按值排序字典
来源：http://wxy.sweek.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eov.ehwqpu.com

[U11] Py：生成器表达式
来源：http://vvh.gogol.net.cn

(x * 2 for x in arr)
来源：http://vvm.jyoumei.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oze.sysykeji.top

Counter(arr).most_common(3)
来源：http://pev.hongshengwenyu.top

[U13] Py：固定长度队列
来源：http://bxk.fengsongda.top

deque(maxlen=10)
来源：http://kcm.jinqigfzy.top

[U14] Py：分组收集到列表
来源：http://nfs.nwbrower.top

defaultdict(list)
来源：http://tob.cqqwz.cn

[U15] Py：高精度计时
来源：http://maw.meibo888.top

t = time.perf_counter()
来源：http://uir.zhaomingkeji.xyz

[U16] Py：命令行参数解析
来源：http://mzu.hysaishi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mup.redwolf501.top

[U17] Py：初始化日志
来源：http://bjp.redwolf501.top

logging.basicConfig(level=logging.INFO)
来源：http://zhg.chenjidiqi.icu

[U18] Py：预编译正则
来源：http://egk.yueranfly.top

pat = re.compile(r"\d+")
来源：http://rjs.52xcode.cn

[U19] Py：正则替换带回调
来源：http://bfq.shanyushiyangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oys.hfpthk.cn

[U20] Py：缓存函数结果
来源：http://bju.yuanzhike.top

@functools.lru_cache(maxsize=None)
来源：http://nqn.zhongyouzk.top

[U21] Py：自定义上下文管理器
来源：http://omu.fanxiaobao.xyz

@contextlib.contextmanager
来源：http://ubt.chenlongwang.top

[U22] Py：矩阵转置
来源：http://zpd.xinyue.icu

list(zip(*m))
来源：http://qot.vqdsnc.cn

[U23] Py：分块读取大文件
来源：http://flk.shuidangran.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fsu.hnqzz.top

[U24] Py：路径操作
来源：http://zik.xziqi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cun.andypj.xyz

[U25] Py：CSV 按字典读
来源：http://psh.guowangkeji.top

csv.DictReader(f)
来源：http://mvr.jiagoushi.top

[U26] Py：并发下载
来源：http://tbd.cucudq.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cuw.wangdashe.top

[U27] Py：异步 HTTP
来源：http://xgf.kuanghao11.cn

aiohttp.ClientSession() 配合 async with
来源：http://qkf.daxiang520.top

[U28] Py：类型别名
来源：http://bic.0kj1m.cn

UserId = int
来源：http://xno.chenlongwang.top

[U29] Py：属性校验
来源：http://dxo.aibaodan.cn

@property 与 @x.setter 配合
来源：http://pfy.feifeiyinyue.top

[U30] Py：数据类
来源：http://ryo.uphjek.com

@dataclass(slots=True)
来源：http://dpd.xinyue.icu

[U31] Py：单测
来源：http://jig.tarul.cn

python -m pytest -q
来源：http://nbj.gogol.net.cn

[U32] Py：代码格式化
来源：http://eml.cqqwz.cn

ruff format . && ruff check --fix .
来源：http://lfk.yanxiufei.cn

[U33] Py：打包发布
来源：http://qmb.fanxiaobao.xyz

python -m build  （依赖 pyproject.toml）
来源：http://jhu.sweek.top

[U34] Py：判断编码
来源：http://aql.0kj1m.cn

chardet.detect(raw)
来源：http://iuw.sjlbkw.cn

[U35] Py：发送邮件
来源：http://yip.daria6918.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hbp.feifeiyinyue.top

[U36] Py：定时任务
来源：http://pln.ivvv.top

schedule.every(10).minutes.do(job)
来源：http://crn.aizwys.cn

[U37] Py：读写 Excel
来源：http://izw.c1oappe.top

pandas.read_excel / DataFrame.to_excel
来源：http://dfq.tanke756.top

[U38] Py：获取脚本所在目录
来源：http://ruu.zdbjq.cn

Path(__file__).resolve().parent
来源：http://urt.nanxinkj.top

[U39] Py：判断是否在交互环境
来源：http://vrk.zdqjudy.top

sys.stdout.isatty()
来源：http://utd.aibaodan.cn

[U40] Py：打印到标准错误
来源：http://qcw.tianlin.xyz

print("err", file=sys.stderr)
来源：http://wkf.shanyushiyangkeji.top

[U41] PHP：初始化 Composer 项目
来源：http://zvf.ivvv.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ons.jqgfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://jbf.nwbrower.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ubk.jinyuanbaomall.cn

[U43] PHP：声明命名空间
来源：http://wbn.yuanzhike.top

namespace App\Http;
来源：http://tnp.shuidangran.top

[U44] PHP：开启严格类型
来源：http://sli.xingfuxueyuan.xyz

declare(strict_types=1);
来源：http://xbi.wangshuangyany.cn

[U45] PHP：类型声明与返回类型
来源：http://epc.xziqi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://inh.hnxiangtu.top

[U46] PHP：可空类型
来源：http://lzr.zhongyouzk.top

?string $name = null
来源：http://svx.ehwqpu.com

[U47] PHP：联合类型
来源：http://sij.nanxinkj.top

int|string $id
来源：http://wis.0kj1m.cn

[U48] PHP：纯枚举
来源：http://qfr.wangdashe.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cgk.sufxvd.cn

[U49] PHP：只读属性
来源：http://jtn.tanke756.top

public readonly string $name
来源：http://kau.gotoacloud.top

[U50] PHP：构造器属性提升
来源：http://dba.meibo888.top

public function __construct(private int $id) {}
来源：http://ltk.smart0.xyz

[U51] PHP：数组解构
来源：http://ntw.aibaodan.cn

[$a, $b] = $arr;
来源：http://iep.zdbjq.cn

[U52] PHP：箭头函数
来源：http://ije.hesvh.cn

$double = fn($x) => $x * 2;
来源：http://zyp.cdnleiting.top

[U53] PHP：空合并运算符
来源：http://fih.gotoacloud.top

$v = $a ?? $b ?? "default";
来源：http://jmy.chenlongwang.top

[U54] PHP：空安全调用
来源：http://tmc.snrcjt.cn

$obj?->method()
来源：http://pho.gogol.net.cn

[U55] PHP：match 表达式
来源：http://iaa.fehbvm.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://crt.sjlbkw.cn

[U56] PHP：命名参数
来源：http://xrs.quarkkingdee.top

f(a: 1, b: 2)
来源：http://kem.hfpthk.cn

[U57] PHP：字符串插值
来源：http://dbm.gogol.net.cn

"值: {$a}"
来源：http://xzt.haohaochexian.top

[U58] PHP：数组三件套
来源：http://bdl.hysaishi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ssg.yonumen.top

[U59] PHP：自定义排序
来源：http://uzt.meibo888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lwg.cashguo.top

[U60] PHP：JSON 编解码
来源：http://aaq.daxiang520.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qev.mhx1999.top

[U61] PHP：正则
来源：http://fom.yongpay.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jdz.hammf.cn

[U62] PHP：日期对象
来源：http://evu.0kj1m.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://phb.pengpengdd.cyou

[U63] PHP：文件读写
来源：http://fsz.aibaodan.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fax.hfpthk.cn

[U64] PHP：目录遍历
来源：http://glp.vehdjk.com

glob("dir/*.php");  scandir("dir");
来源：http://jvx.vqdsnc.cn

[U65] PHP：会话
来源：http://oyj.hammf.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://osn.zdqjudy.top

[U66] PHP：设置 Cookie
来源：http://iek.cucudq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://haa.wangshuangyany.cn

[U67] PHP：处理文件上传
来源：http://ttg.vqdsnc.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ghh.mhx1999.top

[U68] PHP：PDO 连接
来源：http://cqg.zhongyouzk.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gnk.tianlin.xyz

[U69] PHP：PDO 预处理
来源：http://tru.yfazqb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ouu.dianchejie.cn

[U70] PHP：PDO 事务
来源：http://rvi.yfazqb.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://iub.ctjpmb.com

[U71] PHP：抛出异常
来源：http://tmj.yj20258888.top

throw new RuntimeException("失败", 500);
来源：http://fow.jinyuanbaomall.cn

[U72] PHP：写错误日志
来源：http://zjb.snrcjt.cn

error_log("失败: " . $e->getMessage());
来源：http://tty.yangfankeji.com

[U73] PHP：读取 ini 配置
来源：http://vgg.jinyuanbaomall.cn

parse_ini_file("config.ini", true)
来源：http://qmf.yangfankeji.com

[U74] PHP：读取环境变量
来源：http://bxz.smart0.xyz

getenv("APP_ENV") ?: "production"
来源：http://nwi.jinyuanbaomall.cn

[U75] PHP：依赖注入
来源：http://kei.tianlin.xyz

composer require psr/container
来源：http://zoa.mhx1999.top

[U76] PHP：简单路由
来源：http://hco.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wzg.fanxiaobao.xyz

[U77] PHP：模板渲染
来源：http://fyc.cdnleiting.top

composer require twig/twig
来源：http://xgf.yueranfly.top

[U78] PHP：单元测试
来源：http://wll.ctjpmb.com

composer require --dev phpunit/phpunit
来源：http://jel.c1oappe.top

[U79] PHP：静态分析
来源：http://cpg.gotoacloud.top

composer require --dev phpstan/phpstan
来源：http://ilz.xingfuxueyuan.xyz

[U80] PHP：代码规范修复
来源：http://irk.xinyue.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://rzn.c1oappe.top

[U81] JS：初始化项目
来源：http://ctq.dianchejie.cn

npm init -y;  npm i express
来源：http://gzc.bjfxy.top

[U82] JS：package.json 脚本
来源：http://fpa.chenjidiqi.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://htx.yonumen.top


<!-- 参考信息 -->