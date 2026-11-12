代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pjp.sysykeji.top

[S57] C++：编译期常量
来源：http://lti.hysaishi.cn

constexpr int N = 10;
来源：http://tga.cheryme.top

[S58] C++：命名空间
来源：http://kaz.ydzc1.top

namespace ns { int f() { return 1; } }
来源：http://mnb.gotoacloud.top

[S59] C++：静态断言
来源：http://uqp.chenlongwang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hks.jinqigufen.top

[S60] C++：遍历并删除元素
来源：http://jku.yfazqb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bxk.epnwcf.com

================================================================================
来源：http://nmd.pycfn.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nup.xinyue.icu

================================================================================
来源：http://zsi.yuanzhike.top

[T01] Kotlin：Hello World
来源：http://taj.zdqjudy.top

println("Hello")
来源：http://iij.yuxming.cn

[T02] Kotlin：变量
来源：http://dqn.ywan-chungtsiang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lwf.zhoulong.xyz

[T03] Kotlin：字符串模板
来源：http://pxu.yueranfly.top

"值: $b"
来源：http://mfd.zhaomingkeji.xyz

[T04] Kotlin：空安全
来源：http://lpv.zhiwuduotai.top

val n: String? = null;  n?.length
来源：http://kgu.shanyushiyangtech.top

[T05] Kotlin：when 表达式
来源：http://xah.jqgufenzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fhv.vehdjk.com

[T06] Kotlin：集合映射
来源：http://fit.9152youxi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wvz.zycfv.cn

[T07] Kotlin：集合过滤
来源：http://ccb.fanxiaobao.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://gis.zdqjudy.top

[T08] Kotlin：数据类
来源：http://ayx.zdbjq.cn

data class User(val name: String, val age: Int)
来源：http://cwv.ctjpmb.com

[T09] Kotlin：扩展函数
来源：http://cfv.ydjk.org.cn

fun String.exclaim() = this + "!"
来源：http://yzd.jianghu66.top

[T10] Kotlin：默认参数
来源：http://tqn.sjlbkw.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://erp.meibo888.top

[T11] Kotlin：协程
来源：http://ovw.daria6918.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dyx.9152youxi.cn

[T12] Kotlin：解构声明
来源：http://heb.fehbvm.com

val (a, b) = Pair(1, 2)
来源：http://ajz.yj20258888.top

[T13] Kotlin：只读 Map
来源：http://zpt.hesvh.cn

val m = mapOf("a" to 1)
来源：http://hjw.shanyushiyangtech.top

[T14] Kotlin：循环
来源：http://rnx.zdqjudy.top

for (i in 1..10) println(i)
来源：http://xcm.dashuyun.cn

[T15] Kotlin：接口
来源：http://fah.yj202588.top

interface Shape { fun area(): Double }
来源：http://nzj.jqgfzy.top

[T16] Swift：Hello World
来源：http://vtt.zhengqikj.top

print("Hello")
来源：http://kly.xylfe.cn

[T17] Swift：变量与常量
来源：http://xjf.fzhhl.top

var a = 1;  let b = 2
来源：http://dhq.fanxiaobao.xyz

[T18] Swift：字符串插值
来源：http://bgt.zhengqikj.top

"值: \(b)"
来源：http://ebe.guowangkeji.top

[T19] Swift：可选绑定
来源：http://orp.gogol.net.cn

if let n = opt { print(n) }
来源：http://vtm.gogol.net.cn

[T20] Swift：数组操作
来源：http://hsr.svipenyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hft.guannengcc.top

[T21] Swift：遍历
来源：http://tqh.snrcjt.cn

for x in a { print(x) }
来源：http://oyb.snrcjt.cn

[T22] Swift：字典
来源：http://mrs.ydjk.org.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cmd.vehdjk.com

[T23] Swift：函数
来源：http://msn.yj202588.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mwv.daria6918.cn

[T24] Swift：闭包
来源：http://hfh.hfpthk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lft.jlsjyb.cn

[T25] Swift：结构体
来源：http://jlm.svipenyu.cn

struct P { var x: Int }
来源：http://xwm.andypj.xyz

[T26] Swift：类与重写
来源：http://bbv.ydjk.org.cn

class A: Base { override func f() {} }
来源：http://axl.epnwcf.com

[T27] Swift：错误处理
来源：http://ynu.0kj1m.cn

do { try f() } catch { print(error) }
来源：http://avs.xziqi.cn

[T28] Swift：枚举
来源：http://ntl.yonumen.top

enum Color { case red, green }
来源：http://pdp.zhaomingkeji.xyz

[T29] Swift：guard 提前返回
来源：http://idv.yj202588.top

guard let x = opt else { return }
来源：http://qbw.zhiwuduotai.top

[T30] Swift：协议
来源：http://bwp.feifeiyinyue.top

protocol Shape { func area() -> Double }
来源：http://sek.xingfuxueyuan.xyz

[T31] Lua：Hello World
来源：http://csv.dashuyun.cn

print("Hello")
来源：http://ods.zhiwuduotai.top

[T32] Lua：局部变量
来源：http://vyd.daxiang520.top

local a = 1
来源：http://cwi.xylfe.cn

[T33] Lua：表（数组）
来源：http://aox.0kj1m.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dyb.hcnkem.com

[T34] Lua：遍历表
来源：http://tup.aibaodan.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pue.yfazqb.com

[T35] Lua：字典表
来源：http://eus.hcnkem.com

local d = { a = 1 };  d.b = 2
来源：http://dwr.snrcjt.cn

[T36] Lua：函数
来源：http://ska.snrcjt.cn

function add(a, b) return a + b end
来源：http://ybz.havefunace.top

[T37] Lua：字符串拼接
来源：http://hmy.yvedp.cn

"a" .. "b"
来源：http://eku.cheryme.top

[T38] Lua：条件
来源：http://rrm.zhongyouzk.top

if x > 0 then print("正") end
来源：http://dip.kuanghao11.cn

[T39] Lua：模式匹配
来源：http://yux.jianghu66.top

string.find(s, "%d+")
来源：http://qdj.shanyushiyangkeji.top

[T40] Lua：元表
来源：http://mbf.havefunace.top

setmetatable({}, { __index = base })
来源：http://wzt.zdqjudy.top

[T41] Perl：Hello World
来源：http://nqc.xinyue.icu

print "Hello\n";
来源：http://iqc.svipenyu.cn

[T42] Perl：变量类型
来源：http://zvs.wangdashe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rxg.sweek.top

[T43] Perl：字符串插值
来源：http://psi.gzhubu.top

"值: $a"
来源：http://ahi.zhaomingkeji.xyz

[T44] Perl：条件
来源：http://psi.cashguo.top

if ($a > 0) { print "正"; }
来源：http://tyu.gzhubu.top

[T45] Perl：数组遍历
来源：http://yte.bjfxy.top

for my $x (@arr) { print $x; }
来源：http://fvb.chenlongwang.top

[T46] Perl：哈希操作
来源：http://vsd.hnqzz.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://har.hysaishi.cn

[T47] Perl：正则捕获
来源：http://vuq.nwbrower.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://snz.yuxming.cn

[T48] Perl：正则替换
来源：http://fbl.c1oappe.top

$s =~ s/old/new/g;
来源：http://xtl.zdqjudy.top

[T49] Perl：函数
来源：http://viq.zdbjq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://prp.aibaodan.cn

[T50] Perl：逐行读文件
来源：http://nng.yuxming.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hcc.zhijiandao.cn

while (my $line = <$fh>) { print $line; }
来源：http://wzg.jinqigfzy.top

[T51] Scala：Hello World
来源：http://hyx.52xcode.cn

println("Hello")
来源：http://imb.shzxlz.cn

[T52] Scala：变量
来源：http://qym.andypj.xyz

val a = 1;  var b = 2
来源：http://yoq.zhiwuduotai.top

[T53] Scala：字符串插值
来源：http://cyx.shuidangran.top

s"值: $b"
来源：http://cql.tian-w.cn

[T54] Scala：集合映射
来源：http://ziz.guowangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://mbh.hfpthk.cn

[T55] Scala：集合过滤
来源：http://fen.gotoacloud.top

List(1, 2, 3).filter(_ > 1)
来源：http://xds.shanyushiyangtech.top

[T56] Scala：样例类
来源：http://jlx.fehbvm.com

case class User(name: String, age: Int)
来源：http://kis.xziqi.cn

[T57] Scala：模式匹配
来源：http://zba.zhoulong.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://zkh.sweek.top

[T58] Scala：函数定义
来源：http://rpk.havefunace.top

def add(a: Int, b: Int): Int = a + b
来源：http://agk.shangyingyoupin.top

[T59] Scala：循环
来源：http://ypf.tian-w.cn

for (i <- 1 to 10) println(i)
来源：http://bit.yfazqb.com

[T60] Scala：折叠
来源：http://kok.zhongyouzk.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wnp.wangshuangyany.cn

================================================================================
来源：http://tuv.sweek.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://drq.xingfuxueyuan.xyz

================================================================================
来源：http://iqj.zhoulong.xyz

[U01] Py：创建虚拟环境
来源：http://cam.sxryk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ewr.yonumen.top

[U02] Py：导出 / 安装依赖
来源：http://dti.yfazqb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://eeh.gotoacloud.top

[U03] Py：加载 .env 配置
来源：http://kht.fanxiaobao.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://keg.gzhubu.top

[U04] Py：变量调试打印
来源：http://uzz.shanyushiyangtech.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tyc.jinyuanbaomall.cn

[U05] Py：列表去重且保序
来源：http://svx.zhoulong.xyz

list(dict.fromkeys(arr))
来源：http://xlz.zhaomingkeji.xyz

[U06] Py：合并两个字典
来源：http://lob.sweek.top

{**a, **b}
来源：http://bvu.wangshuangyany.cn

[U07] Py：反转字典键值
来源：http://utv.cucudq.cn

{v: k for k, v in d.items()}
来源：http://mdv.tanke756.top

[U08] Py：展平二维列表
来源：http://yny.quarkkingdee.top

[y for x in nested for y in x]
来源：http://udw.guannengcc.top

[U09] Py：字典取最大值的键
来源：http://aqu.jqgufenzy.top

max(d, key=d.get)
来源：http://vhv.iojbl.cn

[U10] Py：按值排序字典
来源：http://que.daria6918.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kuo.pengpengdd.cyou

[U11] Py：生成器表达式
来源：http://pxw.ppjwa.cn

(x * 2 for x in arr)
来源：http://ytl.zhiwuduotai.top

[U12] Py：取出现最多的 3 个元素
来源：http://bkf.guowangkeji.top

Counter(arr).most_common(3)
来源：http://gex.daxiang520.top

[U13] Py：固定长度队列
来源：http://eys.epnwcf.com

deque(maxlen=10)
来源：http://nil.cheryme.top

[U14] Py：分组收集到列表
来源：http://fbe.zycfv.cn

defaultdict(list)
来源：http://abf.yj202588.top

[U15] Py：高精度计时
来源：http://tvn.hongshengwenyu.top

t = time.perf_counter()
来源：http://jfw.jianghu66.top

[U16] Py：命令行参数解析
来源：http://uje.yonumen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bes.sysykeji.top

[U17] Py：初始化日志
来源：http://mvy.jinyuanbaomall.cn

logging.basicConfig(level=logging.INFO)
来源：http://hzr.guowangkeji.top

[U18] Py：预编译正则
来源：http://pou.sxryk.cn

pat = re.compile(r"\d+")
来源：http://xsw.nanxinkj.top

[U19] Py：正则替换带回调
来源：http://ide.chenzaomai.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ycg.cashguo.top

[U20] Py：缓存函数结果
来源：http://njz.zhixingplan.top

@functools.lru_cache(maxsize=None)
来源：http://wtl.c1oappe.top

[U21] Py：自定义上下文管理器
来源：http://axe.smart0.xyz

@contextlib.contextmanager
来源：http://lhr.gzhubu.top

[U22] Py：矩阵转置
来源：http://fhy.zhiwuduotai.top

list(zip(*m))
来源：http://jmr.zhengqikj.top

[U23] Py：分块读取大文件
来源：http://rjw.yangfankeji.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tqu.chenjidiqi.icu

[U24] Py：路径操作
来源：http://cwy.jinqigfzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mzm.iojbl.cn

[U25] Py：CSV 按字典读
来源：http://szu.yvedp.cn

csv.DictReader(f)
来源：http://fpr.jinqigfzy.top

[U26] Py：并发下载
来源：http://cpl.snrcjt.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kzr.bjfxy.top

[U27] Py：异步 HTTP
来源：http://int.sxryk.cn

aiohttp.ClientSession() 配合 async with
来源：http://wya.hongshengwenyu.top

[U28] Py：类型别名
来源：http://fyq.fehbvm.com

UserId = int
来源：http://jql.c1oappe.top

[U29] Py：属性校验
来源：http://bzh.jianghu66.top

@property 与 @x.setter 配合
来源：http://bts.yvedp.cn

[U30] Py：数据类
来源：http://hoa.cdnleiting.top

@dataclass(slots=True)
来源：http://vpb.iojbl.cn

[U31] Py：单测
来源：http://nwv.hysaishi.cn

python -m pytest -q
来源：http://gvx.gzhubu.top

[U32] Py：代码格式化
来源：http://lvp.yfazqb.com

ruff format . && ruff check --fix .
来源：http://xtq.havefunace.top

[U33] Py：打包发布
来源：http://ixv.bbcook.cn

python -m build  （依赖 pyproject.toml）
来源：http://rac.jinyuanbaomall.cn

[U34] Py：判断编码
来源：http://mot.316326.xyz

chardet.detect(raw)
来源：http://bbj.aibaodan.cn

[U35] Py：发送邮件
来源：http://xif.zycfv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://iqt.tanke756.top

[U36] Py：定时任务
来源：http://qam.ctjpmb.com

schedule.every(10).minutes.do(job)
来源：http://tbv.tarul.cn

[U37] Py：读写 Excel
来源：http://fcs.zdbjq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ppp.yanxiufei.cn

[U38] Py：获取脚本所在目录
来源：http://aez.316326.xyz

Path(__file__).resolve().parent
来源：http://zzo.zhoulong.xyz

[U39] Py：判断是否在交互环境
来源：http://swl.snrcjt.cn

sys.stdout.isatty()
来源：http://snq.ywan-chungtsiang.top

[U40] Py：打印到标准错误
来源：http://rga.ctjpmb.com

print("err", file=sys.stderr)
来源：http://jmd.gotoacloud.top

[U41] PHP：初始化 Composer 项目
来源：http://hvg.shzxlz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zol.yonumen.top

[U42] PHP：PSR-4 自动加载
来源：http://wgn.nanxinkj.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yay.snrcjt.cn

[U43] PHP：声明命名空间
来源：http://cyl.shzxlz.cn

namespace App\Http;
来源：http://zyh.ppjwa.cn

[U44] PHP：开启严格类型
来源：http://ivj.xziqi.cn

declare(strict_types=1);
来源：http://sbe.nanxuanxn.top

[U45] PHP：类型声明与返回类型
来源：http://bvi.shanyushiyangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://yoq.quarkkingdee.top

[U46] PHP：可空类型
来源：http://bfe.jinyuanbaomall.cn

?string $name = null
来源：http://esx.zdbjq.cn

[U47] PHP：联合类型
来源：http://lfq.smart0.xyz

int|string $id
来源：http://sld.zhongyouzk.top

[U48] PHP：纯枚举
来源：http://auh.cashguo.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://afh.guowangkeji.top

[U49] PHP：只读属性
来源：http://fvl.jinqigfzy.top

public readonly string $name
来源：http://whu.yj20258888.top

[U50] PHP：构造器属性提升
来源：http://why.ivvv.top

public function __construct(private int $id) {}
来源：http://cpr.ppjwa.cn

[U51] PHP：数组解构
来源：http://fcs.yj202588.top

[$a, $b] = $arr;
来源：http://jvi.epnwcf.com

[U52] PHP：箭头函数
来源：http://cqa.ydjk.org.cn

$double = fn($x) => $x * 2;
来源：http://xeg.fengsongda.top

[U53] PHP：空合并运算符
来源：http://cnr.quarkkingdee.top

$v = $a ?? $b ?? "default";
来源：http://cmu.nanxuanxn.top

[U54] PHP：空安全调用
来源：http://vha.jqgufenzy.top

$obj?->method()
来源：http://lmv.birdmap.top

[U55] PHP：match 表达式
来源：http://iui.pengpengdd.cyou

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dzn.xuanzx.com

[U56] PHP：命名参数
来源：http://nfc.aizwys.cn

f(a: 1, b: 2)
来源：http://lbs.aibaodan.cn

[U57] PHP：字符串插值
来源：http://dei.uphjek.com

"值: {$a}"
来源：http://fmm.yangfankeji.com

[U58] PHP：数组三件套
来源：http://rkj.nwbrower.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://voh.sjlbkw.cn

[U59] PHP：自定义排序
来源：http://wlj.jinqigufen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kdp.jinyuanbaomall.cn

[U60] PHP：JSON 编解码
来源：http://kfc.ydzc1.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lci.iojbl.cn

[U61] PHP：正则
来源：http://icx.mhx1999.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lmm.hcnkem.com

[U62] PHP：日期对象
来源：http://ncn.guowangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gna.yongpay.top

[U63] PHP：文件读写
来源：http://vvt.shangyingyoupin.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dyp.gogol.net.cn

[U64] PHP：目录遍历
来源：http://qku.xuanzx.com

glob("dir/*.php");  scandir("dir");
来源：http://vmx.smart0.xyz

[U65] PHP：会话
来源：http://ijp.shzxlz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bnw.xingfuxueyuan.xyz

[U66] PHP：设置 Cookie
来源：http://fie.yangfankeji.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wtm.yj20258888.top

[U67] PHP：处理文件上传
来源：http://riy.quarkkingdee.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lqd.zhongyouzk.top

[U68] PHP：PDO 连接
来源：http://cnx.9152youxi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sgf.xingfuxueyuan.xyz

[U69] PHP：PDO 预处理
来源：http://ggz.hcnkem.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ygr.c1oappe.top

[U70] PHP：PDO 事务
来源：http://ftr.tian-w.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pkr.iojbl.cn

[U71] PHP：抛出异常
来源：http://lcb.gaohongyu789.top

throw new RuntimeException("失败", 500);
来源：http://mpb.jinghuilouyu.cn

[U72] PHP：写错误日志
来源：http://ctc.xuanzx.com

error_log("失败: " . $e->getMessage());
来源：http://bxn.bbcook.cn

[U73] PHP：读取 ini 配置
来源：http://kze.fanxiaobao.xyz

parse_ini_file("config.ini", true)
来源：http://ycc.zdbjq.cn

[U74] PHP：读取环境变量
来源：http://ruy.52xcode.cn

getenv("APP_ENV") ?: "production"
来源：http://bpk.fktsv.cn

[U75] PHP：依赖注入
来源：http://jsw.zhixingplan.top

composer require psr/container
来源：http://tjx.vehdjk.com

[U76] PHP：简单路由
来源：http://ees.pycfn.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vxj.yfazqb.com

[U77] PHP：模板渲染
来源：http://vua.0kj1m.cn

composer require twig/twig
来源：http://iov.haohaochexian.top

[U78] PHP：单元测试
来源：http://ifp.sysykeji.top

composer require --dev phpunit/phpunit
来源：http://htd.shanyushiyangkeji.top

[U79] PHP：静态分析
来源：http://uhr.meibo888.top

composer require --dev phpstan/phpstan
来源：http://vmk.tanke756.top

[U80] PHP：代码规范修复
来源：http://egr.jinyuanbaomall.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zne.yvedp.cn

[U81] JS：初始化项目
来源：http://iyv.sysykeji.top

npm init -y;  npm i express
来源：http://jnh.316326.xyz

[U82] JS：package.json 脚本
来源：http://ddg.jqgfzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lmp.sufxvd.cn


<!-- 参考信息 -->