代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hgu.jinqigufen.top

[S57] C++：编译期常量
来源：http://ksj.yuanzhike.top

constexpr int N = 10;
来源：http://oev.dashuyun.cn

[S58] C++：命名空间
来源：http://sid.yanxiufei.cn

namespace ns { int f() { return 1; } }
来源：http://iub.ehwqpu.com

[S59] C++：静态断言
来源：http://anc.xuanzx.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://slb.svipenyu.cn

[S60] C++：遍历并删除元素
来源：http://kfd.52xcode.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kjk.yfazqb.com

================================================================================
来源：http://hsb.yfazqb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qxv.wangshuangyany.cn

================================================================================
来源：http://pus.tian-w.cn

[T01] Kotlin：Hello World
来源：http://hmk.wangshuangyany.cn

println("Hello")
来源：http://gmd.nwbrower.top

[T02] Kotlin：变量
来源：http://hko.sxryk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vrj.bjfxy.top

[T03] Kotlin：字符串模板
来源：http://nzl.chenjidiqi.icu

"值: $b"
来源：http://voy.wangdashe.top

[T04] Kotlin：空安全
来源：http://dcn.sxryk.cn

val n: String? = null;  n?.length
来源：http://rhs.jinyuanbaomall.cn

[T05] Kotlin：when 表达式
来源：http://fnw.aizwys.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cto.cashguo.top

[T06] Kotlin：集合映射
来源：http://vsj.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://ica.yfazqb.com

[T07] Kotlin：集合过滤
来源：http://egb.jyoumei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ruk.ctjpmb.com

[T08] Kotlin：数据类
来源：http://bws.yj20258888.top

data class User(val name: String, val age: Int)
来源：http://pga.yj20258888.top

[T09] Kotlin：扩展函数
来源：http://abz.shanyushiyangkeji.top

fun String.exclaim() = this + "!"
来源：http://zkh.jyoumei.cn

[T10] Kotlin：默认参数
来源：http://dsr.snrcjt.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ual.hnxiangtu.top

[T11] Kotlin：协程
来源：http://mja.shangyingyoupin.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fxw.epnwcf.com

[T12] Kotlin：解构声明
来源：http://mjl.guannengcc.top

val (a, b) = Pair(1, 2)
来源：http://ftj.havefunace.top

[T13] Kotlin：只读 Map
来源：http://ttg.feifeiyinyue.top

val m = mapOf("a" to 1)
来源：http://eyt.hesvh.cn

[T14] Kotlin：循环
来源：http://nna.hywenlv.cn

for (i in 1..10) println(i)
来源：http://tgd.zycfv.cn

[T15] Kotlin：接口
来源：http://mzi.zhiwuduotai.top

interface Shape { fun area(): Double }
来源：http://hwg.fzhhl.top

[T16] Swift：Hello World
来源：http://jvk.c1oappe.top

print("Hello")
来源：http://hbg.yangfankeji.com

[T17] Swift：变量与常量
来源：http://vuk.aizwys.cn

var a = 1;  let b = 2
来源：http://xyv.jiagoushi.top

[T18] Swift：字符串插值
来源：http://eah.bbcook.cn

"值: \(b)"
来源：http://tsy.sysykeji.top

[T19] Swift：可选绑定
来源：http://szg.snrcjt.cn

if let n = opt { print(n) }
来源：http://efj.yangfankeji.com

[T20] Swift：数组操作
来源：http://qnp.xuanzx.com

var a = [1, 2, 3];  a.append(4)
来源：http://vem.xinyue.icu

[T21] Swift：遍历
来源：http://rox.xylfe.cn

for x in a { print(x) }
来源：http://dhw.jqgfzy.top

[T22] Swift：字典
来源：http://sul.bjfxy.top

var d = ["a": 1];  d["b"] = 2
来源：http://xwu.tanke756.top

[T23] Swift：函数
来源：http://clz.cashguo.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pmk.hfpthk.cn

[T24] Swift：闭包
来源：http://mqo.shzxlz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yke.sweek.top

[T25] Swift：结构体
来源：http://ugx.uphjek.com

struct P { var x: Int }
来源：http://cpd.bbcook.cn

[T26] Swift：类与重写
来源：http://yzi.hesvh.cn

class A: Base { override func f() {} }
来源：http://syh.xuetiantiany.cn

[T27] Swift：错误处理
来源：http://avy.yvedp.cn

do { try f() } catch { print(error) }
来源：http://mbv.gzhubu.top

[T28] Swift：枚举
来源：http://kkr.yuxming.cn

enum Color { case red, green }
来源：http://yio.bbcook.cn

[T29] Swift：guard 提前返回
来源：http://qmq.tian-w.cn

guard let x = opt else { return }
来源：http://dwd.haohaochexian.top

[T30] Swift：协议
来源：http://tou.sjlbkw.cn

protocol Shape { func area() -> Double }
来源：http://jao.jinghuilouyu.cn

[T31] Lua：Hello World
来源：http://vwb.epnwcf.com

print("Hello")
来源：http://oqi.hesvh.cn

[T32] Lua：局部变量
来源：http://buj.hcnkem.com

local a = 1
来源：http://xdy.tanke756.top

[T33] Lua：表（数组）
来源：http://cgj.fktsv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fap.ehwqpu.com

[T34] Lua：遍历表
来源：http://skn.meibo888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://bzy.gzhubu.top

[T35] Lua：字典表
来源：http://pvc.bbcook.cn

local d = { a = 1 };  d.b = 2
来源：http://oeh.gaohongyu789.top

[T36] Lua：函数
来源：http://enk.ydzc1.top

function add(a, b) return a + b end
来源：http://hcl.hongshengwenyu.top

[T37] Lua：字符串拼接
来源：http://cjx.zhixingplan.top

"a" .. "b"
来源：http://zvh.nanxuanxn.top

[T38] Lua：条件
来源：http://kpc.fengsongda.top

if x > 0 then print("正") end
来源：http://rir.ydjk.org.cn

[T39] Lua：模式匹配
来源：http://vzw.hnxiangtu.top

string.find(s, "%d+")
来源：http://fln.nanxinkj.top

[T40] Lua：元表
来源：http://cmn.sjlbkw.cn

setmetatable({}, { __index = base })
来源：http://lww.ctjpmb.com

[T41] Perl：Hello World
来源：http://dmh.jqgufenzy.top

print "Hello\n";
来源：http://dzk.jqgfzy.top

[T42] Perl：变量类型
来源：http://xkx.fanxiaobao.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://miv.yueranfly.top

[T43] Perl：字符串插值
来源：http://zic.ehwqpu.com

"值: $a"
来源：http://vtl.iojbl.cn

[T44] Perl：条件
来源：http://nnt.tarul.cn

if ($a > 0) { print "正"; }
来源：http://tcu.chenjidiqi.icu

[T45] Perl：数组遍历
来源：http://vqr.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://qul.yuxming.cn

[T46] Perl：哈希操作
来源：http://kvi.316326.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lco.tarul.cn

[T47] Perl：正则捕获
来源：http://hfb.zdqjudy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://wxt.haohaochexian.top

[T48] Perl：正则替换
来源：http://yto.pengpengdd.cyou

$s =~ s/old/new/g;
来源：http://eyi.zhiwuduotai.top

[T49] Perl：函数
来源：http://etj.kuanghao11.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ctd.chenjidiqi.icu

[T50] Perl：逐行读文件
来源：http://hbe.nwbrower.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zgn.cheryme.top

while (my $line = <$fh>) { print $line; }
来源：http://qwp.xuetiantiany.cn

[T51] Scala：Hello World
来源：http://xks.yonumen.top

println("Hello")
来源：http://lfv.pengpengdd.cyou

[T52] Scala：变量
来源：http://mfm.zhixingplan.top

val a = 1;  var b = 2
来源：http://wnl.snrcjt.cn

[T53] Scala：字符串插值
来源：http://ybm.zhengqikj.top

s"值: $b"
来源：http://bcc.cucudq.cn

[T54] Scala：集合映射
来源：http://eee.316326.xyz

List(1, 2, 3).map(_ * 2)
来源：http://vuf.gzhubu.top

[T55] Scala：集合过滤
来源：http://fey.xingfuxueyuan.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://vuy.ywan-chungtsiang.top

[T56] Scala：样例类
来源：http://mbh.zhongyouzk.top

case class User(name: String, age: Int)
来源：http://xhw.sjlbkw.cn

[T57] Scala：模式匹配
来源：http://buq.quarkkingdee.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://frv.zhaomingkeji.xyz

[T58] Scala：函数定义
来源：http://ajb.tianlin.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://jxc.smart0.xyz

[T59] Scala：循环
来源：http://hfp.jinghuilouyu.cn

for (i <- 1 to 10) println(i)
来源：http://ttu.jinqigufen.top

[T60] Scala：折叠
来源：http://dmc.hfpthk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mse.sxryk.cn

================================================================================
来源：http://gej.epnwcf.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ohk.snrcjt.cn

================================================================================
来源：http://ejn.aibaodan.cn

[U01] Py：创建虚拟环境
来源：http://ugf.aizwys.cn

python -m venv .venv && source .venv/bin/activate
来源：http://are.zdbjq.cn

[U02] Py：导出 / 安装依赖
来源：http://ynq.hnqzz.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kpc.jinqigufen.top

[U03] Py：加载 .env 配置
来源：http://nvb.ydjk.org.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lns.gaohongyu789.top

[U04] Py：变量调试打印
来源：http://zql.cqqwz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eaf.xingfuxueyuan.xyz

[U05] Py：列表去重且保序
来源：http://awp.hnxiangtu.top

list(dict.fromkeys(arr))
来源：http://nev.9152youxi.cn

[U06] Py：合并两个字典
来源：http://llk.shanyushiyangtech.top

{**a, **b}
来源：http://inz.sufxvd.cn

[U07] Py：反转字典键值
来源：http://bih.sysykeji.top

{v: k for k, v in d.items()}
来源：http://dgg.zhongyouzk.top

[U08] Py：展平二维列表
来源：http://ftu.fzhhl.top

[y for x in nested for y in x]
来源：http://jen.jqgfzy.top

[U09] Py：字典取最大值的键
来源：http://nei.zhixingplan.top

max(d, key=d.get)
来源：http://ydr.tianlin.xyz

[U10] Py：按值排序字典
来源：http://uji.aizwys.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ter.yonumen.top

[U11] Py：生成器表达式
来源：http://rzb.kuanghao11.cn

(x * 2 for x in arr)
来源：http://xgy.chenjidiqi.icu

[U12] Py：取出现最多的 3 个元素
来源：http://dbx.shangyingyoupin.top

Counter(arr).most_common(3)
来源：http://siu.hnqzz.top

[U13] Py：固定长度队列
来源：http://zil.hnxiangtu.top

deque(maxlen=10)
来源：http://svs.zhongyouzk.top

[U14] Py：分组收集到列表
来源：http://osm.0kj1m.cn

defaultdict(list)
来源：http://tzr.shuidangran.top

[U15] Py：高精度计时
来源：http://ows.havefunace.top

t = time.perf_counter()
来源：http://ukp.jinqigufen.top

[U16] Py：命令行参数解析
来源：http://xwf.chenjidiqi.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bre.dianchejie.cn

[U17] Py：初始化日志
来源：http://dgy.sxryk.cn

logging.basicConfig(level=logging.INFO)
来源：http://vkl.aizwys.cn

[U18] Py：预编译正则
来源：http://gkw.hnxiangtu.top

pat = re.compile(r"\d+")
来源：http://dto.yvedp.cn

[U19] Py：正则替换带回调
来源：http://fpe.shanyushiyangtech.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jil.cqqwz.cn

[U20] Py：缓存函数结果
来源：http://ffy.316326.xyz

@functools.lru_cache(maxsize=None)
来源：http://bpm.bbcook.cn

[U21] Py：自定义上下文管理器
来源：http://hkk.quarkkingdee.top

@contextlib.contextmanager
来源：http://azr.chenzaomai.com

[U22] Py：矩阵转置
来源：http://gye.c1oappe.top

list(zip(*m))
来源：http://gas.hysaishi.cn

[U23] Py：分块读取大文件
来源：http://igv.chenjidiqi.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eki.yueranfly.top

[U24] Py：路径操作
来源：http://plj.aibaodan.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vzk.ywan-chungtsiang.top

[U25] Py：CSV 按字典读
来源：http://dps.shuidangran.top

csv.DictReader(f)
来源：http://tmg.quarkkingdee.top

[U26] Py：并发下载
来源：http://ksm.chenlongwang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dkt.mhx1999.top

[U27] Py：异步 HTTP
来源：http://pct.jyoumei.cn

aiohttp.ClientSession() 配合 async with
来源：http://coy.chenzaomai.com

[U28] Py：类型别名
来源：http://iat.yongpay.top

UserId = int
来源：http://cbg.zhijiandao.cn

[U29] Py：属性校验
来源：http://yyf.ivvv.top

@property 与 @x.setter 配合
来源：http://llv.52xcode.cn

[U30] Py：数据类
来源：http://bxz.tanke756.top

@dataclass(slots=True)
来源：http://ohk.meibo888.top

[U31] Py：单测
来源：http://opn.shangyingyoupin.top

python -m pytest -q
来源：http://rvx.ehwqpu.com

[U32] Py：代码格式化
来源：http://oss.hcnkem.com

ruff format . && ruff check --fix .
来源：http://ybv.shangyingyoupin.top

[U33] Py：打包发布
来源：http://ltr.jyoumei.cn

python -m build  （依赖 pyproject.toml）
来源：http://spm.feifeiyinyue.top

[U34] Py：判断编码
来源：http://hib.fanxiaobao.xyz

chardet.detect(raw)
来源：http://vyc.zhiwuduotai.top

[U35] Py：发送邮件
来源：http://qug.ydjk.org.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dlc.shangyingyoupin.top

[U36] Py：定时任务
来源：http://ymx.sweek.top

schedule.every(10).minutes.do(job)
来源：http://ovi.ywan-chungtsiang.top

[U37] Py：读写 Excel
来源：http://mwf.zycfv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fst.jlsjyb.cn

[U38] Py：获取脚本所在目录
来源：http://lfo.hesvh.cn

Path(__file__).resolve().parent
来源：http://jkz.ybcxt.top

[U39] Py：判断是否在交互环境
来源：http://iqb.epnwcf.com

sys.stdout.isatty()
来源：http://ett.jlsjyb.cn

[U40] Py：打印到标准错误
来源：http://xqj.ctjpmb.com

print("err", file=sys.stderr)
来源：http://rrv.zhengqikj.top

[U41] PHP：初始化 Composer 项目
来源：http://ekt.havefunace.top

composer init;  composer require guzzlehttp/guzzle
来源：http://rgs.andypj.xyz

[U42] PHP：PSR-4 自动加载
来源：http://ovy.yueranfly.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cxe.316326.xyz

[U43] PHP：声明命名空间
来源：http://dvo.yanxiufei.cn

namespace App\Http;
来源：http://sae.shanyushiyangkeji.top

[U44] PHP：开启严格类型
来源：http://mgf.ctjpmb.com

declare(strict_types=1);
来源：http://knm.0kj1m.cn

[U45] PHP：类型声明与返回类型
来源：http://ias.feifeiyinyue.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zue.nanxuanxn.top

[U46] PHP：可空类型
来源：http://cmq.wangshuangyany.cn

?string $name = null
来源：http://sof.hcnkem.com

[U47] PHP：联合类型
来源：http://yji.andypj.xyz

int|string $id
来源：http://fxq.yj20258888.top

[U48] PHP：纯枚举
来源：http://dei.vehdjk.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vuu.sysykeji.top

[U49] PHP：只读属性
来源：http://vvj.zycfv.cn

public readonly string $name
来源：http://gfh.fengsongda.top

[U50] PHP：构造器属性提升
来源：http://gfg.hnqzz.top

public function __construct(private int $id) {}
来源：http://tij.hnxiangtu.top

[U51] PHP：数组解构
来源：http://xyb.ydzc1.top

[$a, $b] = $arr;
来源：http://hua.zhixingplan.top

[U52] PHP：箭头函数
来源：http://omg.wangdashe.top

$double = fn($x) => $x * 2;
来源：http://qqk.xingfuxueyuan.xyz

[U53] PHP：空合并运算符
来源：http://pmz.tanke756.top

$v = $a ?? $b ?? "default";
来源：http://bkf.cashguo.top

[U54] PHP：空安全调用
来源：http://yop.xingfuxueyuan.xyz

$obj?->method()
来源：http://hcu.52xcode.cn

[U55] PHP：match 表达式
来源：http://tvq.zhengqikj.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rif.wangshuangyany.cn

[U56] PHP：命名参数
来源：http://gmt.tanke756.top

f(a: 1, b: 2)
来源：http://dpf.jinqigfzy.top

[U57] PHP：字符串插值
来源：http://uic.yonumen.top

"值: {$a}"
来源：http://smo.hnqzz.top

[U58] PHP：数组三件套
来源：http://due.bbcook.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zwk.hfpthk.cn

[U59] PHP：自定义排序
来源：http://qqh.zhongyouzk.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://czm.dianchejie.cn

[U60] PHP：JSON 编解码
来源：http://zir.guannengcc.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gra.tian-w.cn

[U61] PHP：正则
来源：http://lyy.zhijiandao.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tlb.yvedp.cn

[U62] PHP：日期对象
来源：http://uka.fktsv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://odj.jianghu66.top

[U63] PHP：文件读写
来源：http://jzs.hesvh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zfm.fzhhl.top

[U64] PHP：目录遍历
来源：http://hfk.hywenlv.cn

glob("dir/*.php");  scandir("dir");
来源：http://ozv.yangfankeji.com

[U65] PHP：会话
来源：http://des.yangfankeji.com

session_start();  $_SESSION["uid"] = 1;
来源：http://phm.jinyuanbaomall.cn

[U66] PHP：设置 Cookie
来源：http://nws.ehwqpu.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uet.zycfv.cn

[U67] PHP：处理文件上传
来源：http://lsk.hfpthk.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wct.nwbrower.top

[U68] PHP：PDO 连接
来源：http://tym.zhixingplan.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uxz.cqqwz.cn

[U69] PHP：PDO 预处理
来源：http://uny.hywenlv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://odb.cashguo.top

[U70] PHP：PDO 事务
来源：http://zat.shzxlz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://con.hysaishi.cn

[U71] PHP：抛出异常
来源：http://fej.nanxinkj.top

throw new RuntimeException("失败", 500);
来源：http://hwj.zhongyouzk.top

[U72] PHP：写错误日志
来源：http://qji.gaohongyu789.top

error_log("失败: " . $e->getMessage());
来源：http://jrx.fanxiaobao.xyz

[U73] PHP：读取 ini 配置
来源：http://xzj.hnqzz.top

parse_ini_file("config.ini", true)
来源：http://lav.redwolf501.top

[U74] PHP：读取环境变量
来源：http://nvs.c1oappe.top

getenv("APP_ENV") ?: "production"
来源：http://tqw.sjlbkw.cn

[U75] PHP：依赖注入
来源：http://iaz.xinyue.icu

composer require psr/container
来源：http://zej.sufxvd.cn

[U76] PHP：简单路由
来源：http://yvi.xylfe.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kwq.cdnleiting.top

[U77] PHP：模板渲染
来源：http://nop.chenzaomai.com

composer require twig/twig
来源：http://yvg.jiagoushi.top

[U78] PHP：单元测试
来源：http://nnt.cqqwz.cn

composer require --dev phpunit/phpunit
来源：http://qni.guowangkeji.top

[U79] PHP：静态分析
来源：http://bkn.jiagoushi.top

composer require --dev phpstan/phpstan
来源：http://drv.jianghu66.top

[U80] PHP：代码规范修复
来源：http://cso.gotoacloud.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zjt.svipenyu.cn

[U81] JS：初始化项目
来源：http://cve.ydzc1.top

npm init -y;  npm i express
来源：http://uds.gzhubu.top

[U82] JS：package.json 脚本
来源：http://sdy.dianchejie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pcc.snrcjt.cn


<!-- 参考信息 -->