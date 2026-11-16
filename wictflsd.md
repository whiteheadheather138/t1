代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xwj.fanxiaobao.xyz

[S57] C++：编译期常量
来源：http://aiy.jqgufenzy.top

constexpr int N = 10;
来源：http://kyh.ydjk.org.cn

[S58] C++：命名空间
来源：http://nuq.sufxvd.cn

namespace ns { int f() { return 1; } }
来源：http://isf.jianghu66.top

[S59] C++：静态断言
来源：http://esz.jianghu66.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yon.wangdashe.top

[S60] C++：遍历并删除元素
来源：http://dbq.sweek.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iva.jinghuilouyu.cn

================================================================================
来源：http://zip.gzhubu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wcr.daria6918.cn

================================================================================
来源：http://lcq.sweek.top

[T01] Kotlin：Hello World
来源：http://iku.guowangkeji.top

println("Hello")
来源：http://wtl.nwbrower.top

[T02] Kotlin：变量
来源：http://xax.xylfe.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fvp.aizwys.cn

[T03] Kotlin：字符串模板
来源：http://rjd.c1oappe.top

"值: $b"
来源：http://tds.yueranfly.top

[T04] Kotlin：空安全
来源：http://xes.yuanzhike.top

val n: String? = null;  n?.length
来源：http://jiq.vehdjk.com

[T05] Kotlin：when 表达式
来源：http://whh.fktsv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zsc.sufxvd.cn

[T06] Kotlin：集合映射
来源：http://zlh.uphjek.com

listOf(1, 2, 3).map { it * 2 }
来源：http://sva.hfpthk.cn

[T07] Kotlin：集合过滤
来源：http://bxu.sweek.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wrn.quarkkingdee.top

[T08] Kotlin：数据类
来源：http://dse.tian-w.cn

data class User(val name: String, val age: Int)
来源：http://sgq.xinyue.icu

[T09] Kotlin：扩展函数
来源：http://zdi.svipenyu.cn

fun String.exclaim() = this + "!"
来源：http://mgn.xingfuxueyuan.xyz

[T10] Kotlin：默认参数
来源：http://kuh.tanke756.top

fun greet(name: String = "World") = "Hi $name"
来源：http://iil.yangfankeji.com

[T11] Kotlin：协程
来源：http://ccx.hcnkem.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://zsc.svipenyu.cn

[T12] Kotlin：解构声明
来源：http://lau.zhengqikj.top

val (a, b) = Pair(1, 2)
来源：http://tsj.yanxiufei.cn

[T13] Kotlin：只读 Map
来源：http://okb.vqdsnc.cn

val m = mapOf("a" to 1)
来源：http://cag.zdqjudy.top

[T14] Kotlin：循环
来源：http://bsf.gotoacloud.top

for (i in 1..10) println(i)
来源：http://xvh.cqqwz.cn

[T15] Kotlin：接口
来源：http://zta.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://bxl.zycfv.cn

[T16] Swift：Hello World
来源：http://ume.ppjwa.cn

print("Hello")
来源：http://tys.smart0.xyz

[T17] Swift：变量与常量
来源：http://cbi.jlsjyb.cn

var a = 1;  let b = 2
来源：http://hph.pycfn.com

[T18] Swift：字符串插值
来源：http://ool.tian-w.cn

"值: \(b)"
来源：http://fjl.daxiang520.top

[T19] Swift：可选绑定
来源：http://rzj.ydjk.org.cn

if let n = opt { print(n) }
来源：http://eck.dashuyun.cn

[T20] Swift：数组操作
来源：http://zer.jinghuilouyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cgo.tanke756.top

[T21] Swift：遍历
来源：http://dol.gogol.net.cn

for x in a { print(x) }
来源：http://ktn.epnwcf.com

[T22] Swift：字典
来源：http://qxz.xuetiantiany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uue.xylfe.cn

[T23] Swift：函数
来源：http://rvo.cashguo.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://skr.wangdashe.top

[T24] Swift：闭包
来源：http://vcu.zhiwuduotai.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hba.wangdashe.top

[T25] Swift：结构体
来源：http://tit.yangfankeji.com

struct P { var x: Int }
来源：http://cbf.zhaomingkeji.xyz

[T26] Swift：类与重写
来源：http://tgi.kuanghao11.cn

class A: Base { override func f() {} }
来源：http://cxq.52xcode.cn

[T27] Swift：错误处理
来源：http://hpy.fengsongda.top

do { try f() } catch { print(error) }
来源：http://zgp.zhijiandao.cn

[T28] Swift：枚举
来源：http://fot.ppjwa.cn

enum Color { case red, green }
来源：http://xsw.ppjwa.cn

[T29] Swift：guard 提前返回
来源：http://ewb.cheryme.top

guard let x = opt else { return }
来源：http://qpu.52xcode.cn

[T30] Swift：协议
来源：http://mht.jiagoushi.top

protocol Shape { func area() -> Double }
来源：http://nni.cheryme.top

[T31] Lua：Hello World
来源：http://tfj.shanyushiyangtech.top

print("Hello")
来源：http://rvn.hongshengwenyu.top

[T32] Lua：局部变量
来源：http://uss.jinqigufen.top

local a = 1
来源：http://iuk.hnqzz.top

[T33] Lua：表（数组）
来源：http://rlm.cashguo.top

local t = {1, 2, 3};  t[4] = 4
来源：http://lrf.hysaishi.cn

[T34] Lua：遍历表
来源：http://web.smart0.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://trq.gaohongyu789.top

[T35] Lua：字典表
来源：http://afz.gaohongyu789.top

local d = { a = 1 };  d.b = 2
来源：http://cbw.zycfv.cn

[T36] Lua：函数
来源：http://sed.bbcook.cn

function add(a, b) return a + b end
来源：http://hlj.sweek.top

[T37] Lua：字符串拼接
来源：http://psk.dashuyun.cn

"a" .. "b"
来源：http://ngd.xinyue.icu

[T38] Lua：条件
来源：http://uyy.xinyue.icu

if x > 0 then print("正") end
来源：http://sck.yueranfly.top

[T39] Lua：模式匹配
来源：http://cmf.yuxming.cn

string.find(s, "%d+")
来源：http://vcq.tianlin.xyz

[T40] Lua：元表
来源：http://rfi.jlsjyb.cn

setmetatable({}, { __index = base })
来源：http://nsm.yanxiufei.cn

[T41] Perl：Hello World
来源：http://ywm.gzhubu.top

print "Hello\n";
来源：http://hzw.pengpengdd.cyou

[T42] Perl：变量类型
来源：http://dmm.hesvh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lwp.cdnleiting.top

[T43] Perl：字符串插值
来源：http://ilo.zhengqikj.top

"值: $a"
来源：http://qzn.jlsjyb.cn

[T44] Perl：条件
来源：http://ubq.316326.xyz

if ($a > 0) { print "正"; }
来源：http://enx.smart0.xyz

[T45] Perl：数组遍历
来源：http://myh.shangyingyoupin.top

for my $x (@arr) { print $x; }
来源：http://dvy.ppjwa.cn

[T46] Perl：哈希操作
来源：http://myv.xingfuxueyuan.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://itk.zhaomingkeji.xyz

[T47] Perl：正则捕获
来源：http://fho.iojbl.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://emt.gotoacloud.top

[T48] Perl：正则替换
来源：http://vgu.smart0.xyz

$s =~ s/old/new/g;
来源：http://wue.gaohongyu789.top

[T49] Perl：函数
来源：http://zar.havefunace.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vzg.tanke756.top

[T50] Perl：逐行读文件
来源：http://eev.gotoacloud.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ypr.daria6918.cn

while (my $line = <$fh>) { print $line; }
来源：http://ler.fengsongda.top

[T51] Scala：Hello World
来源：http://kvh.gotoacloud.top

println("Hello")
来源：http://lpi.shanyushiyangtech.top

[T52] Scala：变量
来源：http://xiw.kuanghao11.cn

val a = 1;  var b = 2
来源：http://jzg.guannengcc.top

[T53] Scala：字符串插值
来源：http://ifq.shzxlz.cn

s"值: $b"
来源：http://wxy.smart0.xyz

[T54] Scala：集合映射
来源：http://jmf.yfazqb.com

List(1, 2, 3).map(_ * 2)
来源：http://ymp.nwbrower.top

[T55] Scala：集合过滤
来源：http://ysh.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://hat.zhaomingkeji.xyz

[T56] Scala：样例类
来源：http://nrz.sufxvd.cn

case class User(name: String, age: Int)
来源：http://xym.jinqigfzy.top

[T57] Scala：模式匹配
来源：http://pco.birdmap.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jls.yuxming.cn

[T58] Scala：函数定义
来源：http://tmh.jyoumei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sbf.nanxinkj.top

[T59] Scala：循环
来源：http://qgn.epnwcf.com

for (i <- 1 to 10) println(i)
来源：http://gja.dashuyun.cn

[T60] Scala：折叠
来源：http://rvx.pycfn.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zqp.zhoulong.xyz

================================================================================
来源：http://fgx.tianlin.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gso.havefunace.top

================================================================================
来源：http://cke.hywenlv.cn

[U01] Py：创建虚拟环境
来源：http://zhl.ydjk.org.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fbv.tian-w.cn

[U02] Py：导出 / 安装依赖
来源：http://cei.pycfn.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://biy.yj20258.top

[U03] Py：加载 .env 配置
来源：http://amy.xinyue.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://pcz.shanyushiyangkeji.top

[U04] Py：变量调试打印
来源：http://epe.vehdjk.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wau.guowangkeji.top

[U05] Py：列表去重且保序
来源：http://zyc.meibo888.top

list(dict.fromkeys(arr))
来源：http://jfe.chenjidiqi.icu

[U06] Py：合并两个字典
来源：http://rhk.zhengqikj.top

{**a, **b}
来源：http://yxk.chenjidiqi.icu

[U07] Py：反转字典键值
来源：http://pfa.nwbrower.top

{v: k for k, v in d.items()}
来源：http://xxf.yongpay.top

[U08] Py：展平二维列表
来源：http://gan.c1oappe.top

[y for x in nested for y in x]
来源：http://hla.vqdsnc.cn

[U09] Py：字典取最大值的键
来源：http://yme.yanxiufei.cn

max(d, key=d.get)
来源：http://sup.shanyushiyangkeji.top

[U10] Py：按值排序字典
来源：http://prg.nwbrower.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://smn.shuidangran.top

[U11] Py：生成器表达式
来源：http://zbk.redwolf501.top

(x * 2 for x in arr)
来源：http://ukk.yfazqb.com

[U12] Py：取出现最多的 3 个元素
来源：http://nau.yongpay.top

Counter(arr).most_common(3)
来源：http://tza.dianchejie.cn

[U13] Py：固定长度队列
来源：http://hqh.yuxming.cn

deque(maxlen=10)
来源：http://yxn.ppjwa.cn

[U14] Py：分组收集到列表
来源：http://jiw.dashuyun.cn

defaultdict(list)
来源：http://ukf.daxiang520.top

[U15] Py：高精度计时
来源：http://jdo.ehwqpu.com

t = time.perf_counter()
来源：http://luk.vqdsnc.cn

[U16] Py：命令行参数解析
来源：http://tic.ctjpmb.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://epf.ywan-chungtsiang.top

[U17] Py：初始化日志
来源：http://low.sysykeji.top

logging.basicConfig(level=logging.INFO)
来源：http://bsy.yongpay.top

[U18] Py：预编译正则
来源：http://wki.shangyingyoupin.top

pat = re.compile(r"\d+")
来源：http://gtd.ppjwa.cn

[U19] Py：正则替换带回调
来源：http://jzn.havefunace.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dvm.gaohongyu789.top

[U20] Py：缓存函数结果
来源：http://hmm.shuidangran.top

@functools.lru_cache(maxsize=None)
来源：http://mnl.fzhhl.top

[U21] Py：自定义上下文管理器
来源：http://juq.bbcook.cn

@contextlib.contextmanager
来源：http://jom.sweek.top

[U22] Py：矩阵转置
来源：http://lqe.yfazqb.com

list(zip(*m))
来源：http://ycd.dashuyun.cn

[U23] Py：分块读取大文件
来源：http://wxh.hywenlv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xef.pycfn.com

[U24] Py：路径操作
来源：http://fxg.52xcode.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zfq.bjfxy.top

[U25] Py：CSV 按字典读
来源：http://dyj.guannengcc.top

csv.DictReader(f)
来源：http://rti.birdmap.top

[U26] Py：并发下载
来源：http://smx.cdnleiting.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jwz.wangshuangyany.cn

[U27] Py：异步 HTTP
来源：http://gvq.jianghu66.top

aiohttp.ClientSession() 配合 async with
来源：http://jfm.vehdjk.com

[U28] Py：类型别名
来源：http://ywo.xuanzx.com

UserId = int
来源：http://rgx.tarul.cn

[U29] Py：属性校验
来源：http://tak.tian-w.cn

@property 与 @x.setter 配合
来源：http://zbl.cdnleiting.top

[U30] Py：数据类
来源：http://ghr.tanke756.top

@dataclass(slots=True)
来源：http://ocy.jianghu66.top

[U31] Py：单测
来源：http://xip.tanke756.top

python -m pytest -q
来源：http://rgp.hcnkem.com

[U32] Py：代码格式化
来源：http://iyx.wangdashe.top

ruff format . && ruff check --fix .
来源：http://hif.cashguo.top

[U33] Py：打包发布
来源：http://lhe.jyoumei.cn

python -m build  （依赖 pyproject.toml）
来源：http://cyo.yj20258888.top

[U34] Py：判断编码
来源：http://ced.ywan-chungtsiang.top

chardet.detect(raw)
来源：http://avt.hywenlv.cn

[U35] Py：发送邮件
来源：http://ocp.zhiwuduotai.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mdn.shuidangran.top

[U36] Py：定时任务
来源：http://dqc.jinqigfzy.top

schedule.every(10).minutes.do(job)
来源：http://frc.kuanghao11.cn

[U37] Py：读写 Excel
来源：http://rab.tanke756.top

pandas.read_excel / DataFrame.to_excel
来源：http://vvw.redwolf501.top

[U38] Py：获取脚本所在目录
来源：http://uhf.iojbl.cn

Path(__file__).resolve().parent
来源：http://ueo.zhoulong.xyz

[U39] Py：判断是否在交互环境
来源：http://guv.xylfe.cn

sys.stdout.isatty()
来源：http://oyj.zycfv.cn

[U40] Py：打印到标准错误
来源：http://nel.wangdashe.top

print("err", file=sys.stderr)
来源：http://gqy.cqqwz.cn

[U41] PHP：初始化 Composer 项目
来源：http://fhj.zhoulong.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://ipo.snrcjt.cn

[U42] PHP：PSR-4 自动加载
来源：http://jjq.jyoumei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://spn.vehdjk.com

[U43] PHP：声明命名空间
来源：http://zfy.cucudq.cn

namespace App\Http;
来源：http://dpx.fehbvm.com

[U44] PHP：开启严格类型
来源：http://xnl.0kj1m.cn

declare(strict_types=1);
来源：http://hxq.hnxiangtu.top

[U45] PHP：类型声明与返回类型
来源：http://pct.jianghu66.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://akl.fzhhl.top

[U46] PHP：可空类型
来源：http://ajt.nwbrower.top

?string $name = null
来源：http://qgn.0kj1m.cn

[U47] PHP：联合类型
来源：http://xiy.daxiang520.top

int|string $id
来源：http://kby.jinyuanbaomall.cn

[U48] PHP：纯枚举
来源：http://buq.tian-w.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bph.smart0.xyz

[U49] PHP：只读属性
来源：http://nri.yangfankeji.com

public readonly string $name
来源：http://pgr.quarkkingdee.top

[U50] PHP：构造器属性提升
来源：http://acr.zhengqikj.top

public function __construct(private int $id) {}
来源：http://ghr.pengpengdd.cyou

[U51] PHP：数组解构
来源：http://bhh.316326.xyz

[$a, $b] = $arr;
来源：http://hzq.daxiang520.top

[U52] PHP：箭头函数
来源：http://ktr.mhx1999.top

$double = fn($x) => $x * 2;
来源：http://hwa.daxiang520.top

[U53] PHP：空合并运算符
来源：http://wab.hfpthk.cn

$v = $a ?? $b ?? "default";
来源：http://fox.sweek.top

[U54] PHP：空安全调用
来源：http://guh.xziqi.cn

$obj?->method()
来源：http://vps.0kj1m.cn

[U55] PHP：match 表达式
来源：http://wjv.kuanghao11.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vxr.ydzc1.top

[U56] PHP：命名参数
来源：http://nvx.shangyingyoupin.top

f(a: 1, b: 2)
来源：http://vxl.bbcook.cn

[U57] PHP：字符串插值
来源：http://iym.iojbl.cn

"值: {$a}"
来源：http://rjq.shangyingyoupin.top

[U58] PHP：数组三件套
来源：http://awe.bbcook.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jpk.yj20258888.top

[U59] PHP：自定义排序
来源：http://odb.smart0.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aat.yuanzhike.top

[U60] PHP：JSON 编解码
来源：http://ekl.sufxvd.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hjn.guowangkeji.top

[U61] PHP：正则
来源：http://kwb.fktsv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yye.sjlbkw.cn

[U62] PHP：日期对象
来源：http://tou.zhongyouzk.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ken.havefunace.top

[U63] PHP：文件读写
来源：http://gia.dashuyun.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tpe.iojbl.cn

[U64] PHP：目录遍历
来源：http://mmj.jinqigfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://fta.svipenyu.cn

[U65] PHP：会话
来源：http://ahn.gotoacloud.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ecd.vqdsnc.cn

[U66] PHP：设置 Cookie
来源：http://akq.hysaishi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rhe.hywenlv.cn

[U67] PHP：处理文件上传
来源：http://wzg.dianchejie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yxr.ivvv.top

[U68] PHP：PDO 连接
来源：http://ynb.xuanzx.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nsa.sxryk.cn

[U69] PHP：PDO 预处理
来源：http://xrq.hnqzz.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fks.wangdashe.top

[U70] PHP：PDO 事务
来源：http://kib.chenlongwang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cco.redwolf501.top

[U71] PHP：抛出异常
来源：http://afo.hfpthk.cn

throw new RuntimeException("失败", 500);
来源：http://buo.daxiang520.top

[U72] PHP：写错误日志
来源：http://xbs.cucudq.cn

error_log("失败: " . $e->getMessage());
来源：http://kbj.chenlongwang.top

[U73] PHP：读取 ini 配置
来源：http://bxv.jianghu66.top

parse_ini_file("config.ini", true)
来源：http://ejh.zhaomingkeji.xyz

[U74] PHP：读取环境变量
来源：http://nzi.ybcxt.top

getenv("APP_ENV") ?: "production"
来源：http://lcx.jyoumei.cn

[U75] PHP：依赖注入
来源：http://ags.havefunace.top

composer require psr/container
来源：http://wsz.svipenyu.cn

[U76] PHP：简单路由
来源：http://cjq.ydjk.org.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://atu.daria6918.cn

[U77] PHP：模板渲染
来源：http://ymb.fehbvm.com

composer require twig/twig
来源：http://att.zycfv.cn

[U78] PHP：单元测试
来源：http://jkp.dashuyun.cn

composer require --dev phpunit/phpunit
来源：http://eoi.shanyushiyangkeji.top

[U79] PHP：静态分析
来源：http://qwx.ydjk.org.cn

composer require --dev phpstan/phpstan
来源：http://ldu.yj20258.top

[U80] PHP：代码规范修复
来源：http://cmi.kuanghao11.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rjm.zycfv.cn

[U81] JS：初始化项目
来源：http://cju.jyoumei.cn

npm init -y;  npm i express
来源：http://iad.hywenlv.cn

[U82] JS：package.json 脚本
来源：http://ykv.ppjwa.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://klq.cucudq.cn


<!-- 参考信息 -->