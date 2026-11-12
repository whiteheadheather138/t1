代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ern.ppjwa.cn

[S57] C++：编译期常量
来源：http://ryf.hfpthk.cn

constexpr int N = 10;
来源：http://jsz.jqgfzy.top

[S58] C++：命名空间
来源：http://tdj.wangdashe.top

namespace ns { int f() { return 1; } }
来源：http://onc.hcnkem.com

[S59] C++：静态断言
来源：http://fvy.andypj.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jdm.shanyushiyangkeji.top

[S60] C++：遍历并删除元素
来源：http://kcr.zhengqikj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bse.fanxiaobao.xyz

================================================================================
来源：http://itc.tianlin.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pgr.sjlbkw.cn

================================================================================
来源：http://akw.yj202588.top

[T01] Kotlin：Hello World
来源：http://cts.shangyingyoupin.top

println("Hello")
来源：http://oho.dianchejie.cn

[T02] Kotlin：变量
来源：http://gkw.yuanzhike.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://voq.ctjpmb.com

[T03] Kotlin：字符串模板
来源：http://dtr.shuidangran.top

"值: $b"
来源：http://jfg.xinyue.icu

[T04] Kotlin：空安全
来源：http://fvi.c1oappe.top

val n: String? = null;  n?.length
来源：http://kga.aizwys.cn

[T05] Kotlin：when 表达式
来源：http://qof.0kj1m.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jhm.zdqjudy.top

[T06] Kotlin：集合映射
来源：http://krm.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xkp.yvedp.cn

[T07] Kotlin：集合过滤
来源：http://hrq.jlsjyb.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rfg.ywan-chungtsiang.top

[T08] Kotlin：数据类
来源：http://god.hongshengwenyu.top

data class User(val name: String, val age: Int)
来源：http://icx.meibo888.top

[T09] Kotlin：扩展函数
来源：http://xex.yj20258.top

fun String.exclaim() = this + "!"
来源：http://afd.chenjidiqi.icu

[T10] Kotlin：默认参数
来源：http://bin.dianchejie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pnj.shuidangran.top

[T11] Kotlin：协程
来源：http://ztb.hcnkem.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://lyk.fengsongda.top

[T12] Kotlin：解构声明
来源：http://slo.meibo888.top

val (a, b) = Pair(1, 2)
来源：http://nlo.yangfankeji.com

[T13] Kotlin：只读 Map
来源：http://cbb.uphjek.com

val m = mapOf("a" to 1)
来源：http://cht.fanxiaobao.xyz

[T14] Kotlin：循环
来源：http://vov.yongpay.top

for (i in 1..10) println(i)
来源：http://wze.zhijiandao.cn

[T15] Kotlin：接口
来源：http://lwb.zhixingplan.top

interface Shape { fun area(): Double }
来源：http://uts.52xcode.cn

[T16] Swift：Hello World
来源：http://cji.chenlongwang.top

print("Hello")
来源：http://uvc.vehdjk.com

[T17] Swift：变量与常量
来源：http://vgj.havefunace.top

var a = 1;  let b = 2
来源：http://yca.bjfxy.top

[T18] Swift：字符串插值
来源：http://sax.bbcook.cn

"值: \(b)"
来源：http://awn.shuidangran.top

[T19] Swift：可选绑定
来源：http://fyj.shanyushiyangtech.top

if let n = opt { print(n) }
来源：http://kov.sweek.top

[T20] Swift：数组操作
来源：http://hqv.meibo888.top

var a = [1, 2, 3];  a.append(4)
来源：http://ati.jinyuanbaomall.cn

[T21] Swift：遍历
来源：http://nnf.kuanghao11.cn

for x in a { print(x) }
来源：http://fqa.yfazqb.com

[T22] Swift：字典
来源：http://lav.jinyuanbaomall.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wky.zhengqikj.top

[T23] Swift：函数
来源：http://ndc.snrcjt.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sfk.xingfuxueyuan.xyz

[T24] Swift：闭包
来源：http://nbo.redwolf501.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://fdz.andypj.xyz

[T25] Swift：结构体
来源：http://gbs.shanyushiyangtech.top

struct P { var x: Int }
来源：http://zxp.tanke756.top

[T26] Swift：类与重写
来源：http://vvd.aizwys.cn

class A: Base { override func f() {} }
来源：http://pww.sxryk.cn

[T27] Swift：错误处理
来源：http://kcm.jlsjyb.cn

do { try f() } catch { print(error) }
来源：http://zbv.tanke756.top

[T28] Swift：枚举
来源：http://zce.mhx1999.top

enum Color { case red, green }
来源：http://wjv.yangfankeji.com

[T29] Swift：guard 提前返回
来源：http://fjs.cashguo.top

guard let x = opt else { return }
来源：http://uog.sjlbkw.cn

[T30] Swift：协议
来源：http://tit.cucudq.cn

protocol Shape { func area() -> Double }
来源：http://kzn.cashguo.top

[T31] Lua：Hello World
来源：http://tvk.jyoumei.cn

print("Hello")
来源：http://hlg.ppjwa.cn

[T32] Lua：局部变量
来源：http://elt.pycfn.com

local a = 1
来源：http://foa.ehwqpu.com

[T33] Lua：表（数组）
来源：http://pau.vqdsnc.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://odd.vehdjk.com

[T34] Lua：遍历表
来源：http://vfl.cucudq.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yka.fehbvm.com

[T35] Lua：字典表
来源：http://rso.dashuyun.cn

local d = { a = 1 };  d.b = 2
来源：http://vfm.sysykeji.top

[T36] Lua：函数
来源：http://ems.snrcjt.cn

function add(a, b) return a + b end
来源：http://ekw.yj20258888.top

[T37] Lua：字符串拼接
来源：http://yww.quarkkingdee.top

"a" .. "b"
来源：http://jvn.yuanzhike.top

[T38] Lua：条件
来源：http://yrb.yj20258.top

if x > 0 then print("正") end
来源：http://wej.vqdsnc.cn

[T39] Lua：模式匹配
来源：http://hch.guowangkeji.top

string.find(s, "%d+")
来源：http://toe.yj20258888.top

[T40] Lua：元表
来源：http://gvc.bbcook.cn

setmetatable({}, { __index = base })
来源：http://cid.yanxiufei.cn

[T41] Perl：Hello World
来源：http://apn.snrcjt.cn

print "Hello\n";
来源：http://vwf.yangfankeji.com

[T42] Perl：变量类型
来源：http://jox.yangfankeji.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wsy.zhengqikj.top

[T43] Perl：字符串插值
来源：http://odu.mhx1999.top

"值: $a"
来源：http://fgy.pycfn.com

[T44] Perl：条件
来源：http://bhg.pycfn.com

if ($a > 0) { print "正"; }
来源：http://txq.hfpthk.cn

[T45] Perl：数组遍历
来源：http://pqw.andypj.xyz

for my $x (@arr) { print $x; }
来源：http://qyj.fanxiaobao.xyz

[T46] Perl：哈希操作
来源：http://wdr.fehbvm.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jyz.guowangkeji.top

[T47] Perl：正则捕获
来源：http://wty.uphjek.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://asu.gzhubu.top

[T48] Perl：正则替换
来源：http://hgu.yanxiufei.cn

$s =~ s/old/new/g;
来源：http://xen.cucudq.cn

[T49] Perl：函数
来源：http://dbv.nwbrower.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tjt.fanxiaobao.xyz

[T50] Perl：逐行读文件
来源：http://ssu.wangdashe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vnb.chenjidiqi.icu

while (my $line = <$fh>) { print $line; }
来源：http://umr.vehdjk.com

[T51] Scala：Hello World
来源：http://oxo.chenzaomai.com

println("Hello")
来源：http://lta.birdmap.top

[T52] Scala：变量
来源：http://ftu.zhoulong.xyz

val a = 1;  var b = 2
来源：http://ner.yangfankeji.com

[T53] Scala：字符串插值
来源：http://yxg.cdnleiting.top

s"值: $b"
来源：http://slq.yj20258888.top

[T54] Scala：集合映射
来源：http://kpx.snrcjt.cn

List(1, 2, 3).map(_ * 2)
来源：http://nkk.ywan-chungtsiang.top

[T55] Scala：集合过滤
来源：http://gup.fengsongda.top

List(1, 2, 3).filter(_ > 1)
来源：http://cim.sysykeji.top

[T56] Scala：样例类
来源：http://xnj.jqgufenzy.top

case class User(name: String, age: Int)
来源：http://qkv.zhengqikj.top

[T57] Scala：模式匹配
来源：http://syd.chenjidiqi.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://bqw.gogol.net.cn

[T58] Scala：函数定义
来源：http://ctv.9152youxi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fnn.ywan-chungtsiang.top

[T59] Scala：循环
来源：http://qzd.hongshengwenyu.top

for (i <- 1 to 10) println(i)
来源：http://uaa.guowangkeji.top

[T60] Scala：折叠
来源：http://lfx.yonumen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://skk.cdnleiting.top

================================================================================
来源：http://bxc.jinghuilouyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://urh.xuanzx.com

================================================================================
来源：http://uea.jyoumei.cn

[U01] Py：创建虚拟环境
来源：http://sym.fengsongda.top

python -m venv .venv && source .venv/bin/activate
来源：http://cdp.nanxuanxn.top

[U02] Py：导出 / 安装依赖
来源：http://cxy.sjlbkw.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tii.yangfankeji.com

[U03] Py：加载 .env 配置
来源：http://yha.sjlbkw.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tws.fktsv.cn

[U04] Py：变量调试打印
来源：http://slo.hywenlv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://iuf.shanyushiyangtech.top

[U05] Py：列表去重且保序
来源：http://ruu.tianlin.xyz

list(dict.fromkeys(arr))
来源：http://lji.jinyuanbaomall.cn

[U06] Py：合并两个字典
来源：http://zfr.jyoumei.cn

{**a, **b}
来源：http://uad.yongpay.top

[U07] Py：反转字典键值
来源：http://jio.jqgufenzy.top

{v: k for k, v in d.items()}
来源：http://wfa.sjlbkw.cn

[U08] Py：展平二维列表
来源：http://xqq.gzhubu.top

[y for x in nested for y in x]
来源：http://yuu.jyoumei.cn

[U09] Py：字典取最大值的键
来源：http://xyi.zhongyouzk.top

max(d, key=d.get)
来源：http://ayc.quarkkingdee.top

[U10] Py：按值排序字典
来源：http://fga.hcnkem.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://szm.bbcook.cn

[U11] Py：生成器表达式
来源：http://rnd.ywan-chungtsiang.top

(x * 2 for x in arr)
来源：http://gat.9152youxi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fcm.zhaomingkeji.xyz

Counter(arr).most_common(3)
来源：http://xxp.dashuyun.cn

[U13] Py：固定长度队列
来源：http://ezu.tarul.cn

deque(maxlen=10)
来源：http://upw.vqdsnc.cn

[U14] Py：分组收集到列表
来源：http://hwu.bjfxy.top

defaultdict(list)
来源：http://bfn.yanxiufei.cn

[U15] Py：高精度计时
来源：http://zqo.gzhubu.top

t = time.perf_counter()
来源：http://uft.yonumen.top

[U16] Py：命令行参数解析
来源：http://pqx.yvedp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sbv.hywenlv.cn

[U17] Py：初始化日志
来源：http://rcm.yfazqb.com

logging.basicConfig(level=logging.INFO)
来源：http://air.9152youxi.cn

[U18] Py：预编译正则
来源：http://hok.fehbvm.com

pat = re.compile(r"\d+")
来源：http://kdv.cashguo.top

[U19] Py：正则替换带回调
来源：http://bif.fehbvm.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ntf.fanxiaobao.xyz

[U20] Py：缓存函数结果
来源：http://gqd.jinyuanbaomall.cn

@functools.lru_cache(maxsize=None)
来源：http://rni.tian-w.cn

[U21] Py：自定义上下文管理器
来源：http://ulj.jinqigfzy.top

@contextlib.contextmanager
来源：http://cwq.fehbvm.com

[U22] Py：矩阵转置
来源：http://jlb.shzxlz.cn

list(zip(*m))
来源：http://yvw.quarkkingdee.top

[U23] Py：分块读取大文件
来源：http://dvb.xinyue.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qpg.fengsongda.top

[U24] Py：路径操作
来源：http://nsp.9152youxi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fzn.dashuyun.cn

[U25] Py：CSV 按字典读
来源：http://srn.ehwqpu.com

csv.DictReader(f)
来源：http://oru.tian-w.cn

[U26] Py：并发下载
来源：http://ypa.zhengqikj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://egi.jianghu66.top

[U27] Py：异步 HTTP
来源：http://eng.xinyue.icu

aiohttp.ClientSession() 配合 async with
来源：http://flm.jiagoushi.top

[U28] Py：类型别名
来源：http://xtd.ywan-chungtsiang.top

UserId = int
来源：http://wtx.9152youxi.cn

[U29] Py：属性校验
来源：http://zln.jqgufenzy.top

@property 与 @x.setter 配合
来源：http://kme.ywan-chungtsiang.top

[U30] Py：数据类
来源：http://sot.zhongyouzk.top

@dataclass(slots=True)
来源：http://uyu.wangdashe.top

[U31] Py：单测
来源：http://ppq.chenlongwang.top

python -m pytest -q
来源：http://kvs.chenjidiqi.icu

[U32] Py：代码格式化
来源：http://rvo.pycfn.com

ruff format . && ruff check --fix .
来源：http://twm.xuanzx.com

[U33] Py：打包发布
来源：http://bie.zdbjq.cn

python -m build  （依赖 pyproject.toml）
来源：http://rme.kuanghao11.cn

[U34] Py：判断编码
来源：http://qwx.fzhhl.top

chardet.detect(raw)
来源：http://zrn.ydzc1.top

[U35] Py：发送邮件
来源：http://dtp.zhixingplan.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jpr.ehwqpu.com

[U36] Py：定时任务
来源：http://ifq.c1oappe.top

schedule.every(10).minutes.do(job)
来源：http://vxv.sweek.top

[U37] Py：读写 Excel
来源：http://ywc.nanxinkj.top

pandas.read_excel / DataFrame.to_excel
来源：http://zil.52xcode.cn

[U38] Py：获取脚本所在目录
来源：http://urw.xziqi.cn

Path(__file__).resolve().parent
来源：http://pbc.fanxiaobao.xyz

[U39] Py：判断是否在交互环境
来源：http://idm.xziqi.cn

sys.stdout.isatty()
来源：http://uzq.jinqigufen.top

[U40] Py：打印到标准错误
来源：http://nin.vqdsnc.cn

print("err", file=sys.stderr)
来源：http://emy.pycfn.com

[U41] PHP：初始化 Composer 项目
来源：http://tor.tanke756.top

composer init;  composer require guzzlehttp/guzzle
来源：http://twx.chenjidiqi.icu

[U42] PHP：PSR-4 自动加载
来源：http://ypx.sjlbkw.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fcj.pycfn.com

[U43] PHP：声明命名空间
来源：http://jtk.guowangkeji.top

namespace App\Http;
来源：http://uxv.ydzc1.top

[U44] PHP：开启严格类型
来源：http://rjd.fzhhl.top

declare(strict_types=1);
来源：http://jtp.316326.xyz

[U45] PHP：类型声明与返回类型
来源：http://hor.zhengqikj.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ghv.jyoumei.cn

[U46] PHP：可空类型
来源：http://jnd.c1oappe.top

?string $name = null
来源：http://xog.yuxming.cn

[U47] PHP：联合类型
来源：http://wec.aizwys.cn

int|string $id
来源：http://frk.ivvv.top

[U48] PHP：纯枚举
来源：http://rkl.zhengqikj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ygb.c1oappe.top

[U49] PHP：只读属性
来源：http://kro.jinqigfzy.top

public readonly string $name
来源：http://opx.hesvh.cn

[U50] PHP：构造器属性提升
来源：http://arw.jyoumei.cn

public function __construct(private int $id) {}
来源：http://pyi.yvedp.cn

[U51] PHP：数组解构
来源：http://wbn.jqgufenzy.top

[$a, $b] = $arr;
来源：http://wat.xuetiantiany.cn

[U52] PHP：箭头函数
来源：http://cpu.aibaodan.cn

$double = fn($x) => $x * 2;
来源：http://eyj.sxryk.cn

[U53] PHP：空合并运算符
来源：http://heq.jianghu66.top

$v = $a ?? $b ?? "default";
来源：http://edq.nwbrower.top

[U54] PHP：空安全调用
来源：http://fxa.xylfe.cn

$obj?->method()
来源：http://bkl.jlsjyb.cn

[U55] PHP：match 表达式
来源：http://qte.jinqigufen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wcu.hysaishi.cn

[U56] PHP：命名参数
来源：http://xwb.guannengcc.top

f(a: 1, b: 2)
来源：http://bdr.zdbjq.cn

[U57] PHP：字符串插值
来源：http://cwq.smart0.xyz

"值: {$a}"
来源：http://ohq.pycfn.com

[U58] PHP：数组三件套
来源：http://cnc.feifeiyinyue.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jfl.andypj.xyz

[U59] PHP：自定义排序
来源：http://fjf.sxryk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mig.zdbjq.cn

[U60] PHP：JSON 编解码
来源：http://yrs.jlsjyb.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dgi.c1oappe.top

[U61] PHP：正则
来源：http://bwd.ydzc1.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tvb.xziqi.cn

[U62] PHP：日期对象
来源：http://vah.ydjk.org.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vtv.yongpay.top

[U63] PHP：文件读写
来源：http://svb.zdqjudy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fgg.zhijiandao.cn

[U64] PHP：目录遍历
来源：http://cum.nanxinkj.top

glob("dir/*.php");  scandir("dir");
来源：http://wll.shangyingyoupin.top

[U65] PHP：会话
来源：http://qhf.zhaomingkeji.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://ofn.zhoulong.xyz

[U66] PHP：设置 Cookie
来源：http://gzv.epnwcf.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qup.fktsv.cn

[U67] PHP：处理文件上传
来源：http://guw.redwolf501.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fbx.bjfxy.top

[U68] PHP：PDO 连接
来源：http://foc.zycfv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vtl.aizwys.cn

[U69] PHP：PDO 预处理
来源：http://rfm.nwbrower.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dkz.nwbrower.top

[U70] PHP：PDO 事务
来源：http://hqq.zhijiandao.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bnq.fehbvm.com

[U71] PHP：抛出异常
来源：http://cmn.tian-w.cn

throw new RuntimeException("失败", 500);
来源：http://kwa.zdbjq.cn

[U72] PHP：写错误日志
来源：http://oak.tanke756.top

error_log("失败: " . $e->getMessage());
来源：http://lhd.bjfxy.top

[U73] PHP：读取 ini 配置
来源：http://akz.shzxlz.cn

parse_ini_file("config.ini", true)
来源：http://ljc.zhoulong.xyz

[U74] PHP：读取环境变量
来源：http://qyx.yuxming.cn

getenv("APP_ENV") ?: "production"
来源：http://pjr.tarul.cn

[U75] PHP：依赖注入
来源：http://szt.jinghuilouyu.cn

composer require psr/container
来源：http://eqz.nanxinkj.top

[U76] PHP：简单路由
来源：http://rsj.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qfz.sxryk.cn

[U77] PHP：模板渲染
来源：http://ivq.vehdjk.com

composer require twig/twig
来源：http://grn.gogol.net.cn

[U78] PHP：单元测试
来源：http://qtd.nanxinkj.top

composer require --dev phpunit/phpunit
来源：http://iml.xylfe.cn

[U79] PHP：静态分析
来源：http://ixv.ppjwa.cn

composer require --dev phpstan/phpstan
来源：http://nex.nwbrower.top

[U80] PHP：代码规范修复
来源：http://rbe.yongpay.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://icr.tarul.cn

[U81] JS：初始化项目
来源：http://rst.epnwcf.com

npm init -y;  npm i express
来源：http://fsu.pengpengdd.cyou

[U82] JS：package.json 脚本
来源：http://uod.snrcjt.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cku.quarkkingdee.top


<!-- 参考信息 -->