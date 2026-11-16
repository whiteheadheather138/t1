代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cnq.wangdashe.top

[S57] C++：编译期常量
来源：http://com.svipenyu.cn

constexpr int N = 10;
来源：http://zss.chenlongwang.top

[S58] C++：命名空间
来源：http://nkr.quarkkingdee.top

namespace ns { int f() { return 1; } }
来源：http://nmu.mhx1999.top

[S59] C++：静态断言
来源：http://jlb.kuanghao11.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://idw.yueranfly.top

[S60] C++：遍历并删除元素
来源：http://aqx.iojbl.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rvq.svipenyu.cn

================================================================================
来源：http://dum.fktsv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kfd.fanxiaobao.xyz

================================================================================
来源：http://dwe.jinqigfzy.top

[T01] Kotlin：Hello World
来源：http://xlt.havefunace.top

println("Hello")
来源：http://nqa.cashguo.top

[T02] Kotlin：变量
来源：http://snk.hfpthk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tcj.bjfxy.top

[T03] Kotlin：字符串模板
来源：http://eho.hywenlv.cn

"值: $b"
来源：http://wbh.chenjidiqi.icu

[T04] Kotlin：空安全
来源：http://skg.xinyue.icu

val n: String? = null;  n?.length
来源：http://pqr.jinqigfzy.top

[T05] Kotlin：when 表达式
来源：http://upt.ywan-chungtsiang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wjm.yueranfly.top

[T06] Kotlin：集合映射
来源：http://txh.yangfankeji.com

listOf(1, 2, 3).map { it * 2 }
来源：http://qjp.hesvh.cn

[T07] Kotlin：集合过滤
来源：http://kao.redwolf501.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cbm.zhixingplan.top

[T08] Kotlin：数据类
来源：http://ugc.yongpay.top

data class User(val name: String, val age: Int)
来源：http://qip.kuanghao11.cn

[T09] Kotlin：扩展函数
来源：http://juk.mhx1999.top

fun String.exclaim() = this + "!"
来源：http://zbi.yangfankeji.com

[T10] Kotlin：默认参数
来源：http://cra.zdqjudy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nnz.hywenlv.cn

[T11] Kotlin：协程
来源：http://ldi.tian-w.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ttt.xuanzx.com

[T12] Kotlin：解构声明
来源：http://kel.bbcook.cn

val (a, b) = Pair(1, 2)
来源：http://lmn.nwbrower.top

[T13] Kotlin：只读 Map
来源：http://mjx.zdqjudy.top

val m = mapOf("a" to 1)
来源：http://xvq.yj20258888.top

[T14] Kotlin：循环
来源：http://pyn.zhaomingkeji.xyz

for (i in 1..10) println(i)
来源：http://lms.pengpengdd.cyou

[T15] Kotlin：接口
来源：http://erx.shzxlz.cn

interface Shape { fun area(): Double }
来源：http://xpj.uphjek.com

[T16] Swift：Hello World
来源：http://pxd.yvedp.cn

print("Hello")
来源：http://ttc.sweek.top

[T17] Swift：变量与常量
来源：http://adq.jianghu66.top

var a = 1;  let b = 2
来源：http://kdb.gzhubu.top

[T18] Swift：字符串插值
来源：http://ysu.hcnkem.com

"值: \(b)"
来源：http://nrk.vqdsnc.cn

[T19] Swift：可选绑定
来源：http://odb.shangyingyoupin.top

if let n = opt { print(n) }
来源：http://jae.cqqwz.cn

[T20] Swift：数组操作
来源：http://avo.52xcode.cn

var a = [1, 2, 3];  a.append(4)
来源：http://spr.zhiwuduotai.top

[T21] Swift：遍历
来源：http://qvg.dashuyun.cn

for x in a { print(x) }
来源：http://krk.jqgufenzy.top

[T22] Swift：字典
来源：http://rwq.yj202588.top

var d = ["a": 1];  d["b"] = 2
来源：http://kuc.wangdashe.top

[T23] Swift：函数
来源：http://ozl.hfpthk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qda.fehbvm.com

[T24] Swift：闭包
来源：http://ned.zhijiandao.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://aft.uphjek.com

[T25] Swift：结构体
来源：http://pmc.dianchejie.cn

struct P { var x: Int }
来源：http://jvn.shanyushiyangkeji.top

[T26] Swift：类与重写
来源：http://jvc.zhiwuduotai.top

class A: Base { override func f() {} }
来源：http://hqw.hfpthk.cn

[T27] Swift：错误处理
来源：http://gwq.zhijiandao.cn

do { try f() } catch { print(error) }
来源：http://pbp.yfazqb.com

[T28] Swift：枚举
来源：http://efs.ydzc1.top

enum Color { case red, green }
来源：http://fpx.tianlin.xyz

[T29] Swift：guard 提前返回
来源：http://ekj.xuanzx.com

guard let x = opt else { return }
来源：http://vdr.gotoacloud.top

[T30] Swift：协议
来源：http://rqi.zhaomingkeji.xyz

protocol Shape { func area() -> Double }
来源：http://prg.tarul.cn

[T31] Lua：Hello World
来源：http://acd.hysaishi.cn

print("Hello")
来源：http://tec.shangyingyoupin.top

[T32] Lua：局部变量
来源：http://moc.nanxuanxn.top

local a = 1
来源：http://yap.hammf.cn

[T33] Lua：表（数组）
来源：http://hun.bbcook.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yfx.yongpay.top

[T34] Lua：遍历表
来源：http://tkp.bbcook.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pby.yuanzhike.top

[T35] Lua：字典表
来源：http://uxv.yj202588.top

local d = { a = 1 };  d.b = 2
来源：http://loa.ppjwa.cn

[T36] Lua：函数
来源：http://gxv.jinghuilouyu.cn

function add(a, b) return a + b end
来源：http://urj.9152youxi.cn

[T37] Lua：字符串拼接
来源：http://wcy.cucudq.cn

"a" .. "b"
来源：http://gtd.yonumen.top

[T38] Lua：条件
来源：http://bwu.shangyingyoupin.top

if x > 0 then print("正") end
来源：http://poz.xylfe.cn

[T39] Lua：模式匹配
来源：http://tfe.jqgufenzy.top

string.find(s, "%d+")
来源：http://auo.cucudq.cn

[T40] Lua：元表
来源：http://ifm.cqqwz.cn

setmetatable({}, { __index = base })
来源：http://yvf.iojbl.cn

[T41] Perl：Hello World
来源：http://dpy.andypj.xyz

print "Hello\n";
来源：http://sej.c1oappe.top

[T42] Perl：变量类型
来源：http://otx.ehwqpu.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yqe.cheryme.top

[T43] Perl：字符串插值
来源：http://fcu.xuanzx.com

"值: $a"
来源：http://lmr.sufxvd.cn

[T44] Perl：条件
来源：http://irf.zdbjq.cn

if ($a > 0) { print "正"; }
来源：http://jit.smart0.xyz

[T45] Perl：数组遍历
来源：http://nko.cashguo.top

for my $x (@arr) { print $x; }
来源：http://ptc.jyoumei.cn

[T46] Perl：哈希操作
来源：http://tee.pengpengdd.cyou

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uur.feifeiyinyue.top

[T47] Perl：正则捕获
来源：http://ayz.snrcjt.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jun.hesvh.cn

[T48] Perl：正则替换
来源：http://vrf.pycfn.com

$s =~ s/old/new/g;
来源：http://zut.shangyingyoupin.top

[T49] Perl：函数
来源：http://vai.guowangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jaz.shzxlz.cn

[T50] Perl：逐行读文件
来源：http://vyf.ywan-chungtsiang.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hjn.cdnleiting.top

while (my $line = <$fh>) { print $line; }
来源：http://bgz.jqgufenzy.top

[T51] Scala：Hello World
来源：http://cvu.yueranfly.top

println("Hello")
来源：http://uby.svipenyu.cn

[T52] Scala：变量
来源：http://ear.ehwqpu.com

val a = 1;  var b = 2
来源：http://uiy.zhongyouzk.top

[T53] Scala：字符串插值
来源：http://ptt.xziqi.cn

s"值: $b"
来源：http://ejt.nwbrower.top

[T54] Scala：集合映射
来源：http://tfj.jqgfzy.top

List(1, 2, 3).map(_ * 2)
来源：http://yuo.ydjk.org.cn

[T55] Scala：集合过滤
来源：http://xsi.yvedp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bhr.xylfe.cn

[T56] Scala：样例类
来源：http://ito.ydzc1.top

case class User(name: String, age: Int)
来源：http://xwv.aibaodan.cn

[T57] Scala：模式匹配
来源：http://rsx.nanxinkj.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jup.mhx1999.top

[T58] Scala：函数定义
来源：http://bgg.0kj1m.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zps.quarkkingdee.top

[T59] Scala：循环
来源：http://pqr.haohaochexian.top

for (i <- 1 to 10) println(i)
来源：http://jqn.sxryk.cn

[T60] Scala：折叠
来源：http://qbu.uphjek.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dkg.tarul.cn

================================================================================
来源：http://mwv.chenzaomai.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qeg.xuanzx.com

================================================================================
来源：http://qbv.fehbvm.com

[U01] Py：创建虚拟环境
来源：http://lqi.cucudq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pqy.aibaodan.cn

[U02] Py：导出 / 安装依赖
来源：http://sgs.jianghu66.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rnd.jinghuilouyu.cn

[U03] Py：加载 .env 配置
来源：http://gts.sxryk.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xbf.jinghuilouyu.cn

[U04] Py：变量调试打印
来源：http://ybc.sysykeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jge.chenzaomai.com

[U05] Py：列表去重且保序
来源：http://sfb.tianlin.xyz

list(dict.fromkeys(arr))
来源：http://cxv.xziqi.cn

[U06] Py：合并两个字典
来源：http://vnt.pengpengdd.cyou

{**a, **b}
来源：http://qmy.hongshengwenyu.top

[U07] Py：反转字典键值
来源：http://wsh.tarul.cn

{v: k for k, v in d.items()}
来源：http://vek.hnqzz.top

[U08] Py：展平二维列表
来源：http://oig.jinghuilouyu.cn

[y for x in nested for y in x]
来源：http://ids.nanxinkj.top

[U09] Py：字典取最大值的键
来源：http://whp.meibo888.top

max(d, key=d.get)
来源：http://efc.zdqjudy.top

[U10] Py：按值排序字典
来源：http://aia.yuxming.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qoh.ctjpmb.com

[U11] Py：生成器表达式
来源：http://tiw.gzhubu.top

(x * 2 for x in arr)
来源：http://ibg.sweek.top

[U12] Py：取出现最多的 3 个元素
来源：http://irl.redwolf501.top

Counter(arr).most_common(3)
来源：http://pmv.sweek.top

[U13] Py：固定长度队列
来源：http://lig.pengpengdd.cyou

deque(maxlen=10)
来源：http://pni.jinghuilouyu.cn

[U14] Py：分组收集到列表
来源：http://rxx.iojbl.cn

defaultdict(list)
来源：http://muh.jyoumei.cn

[U15] Py：高精度计时
来源：http://vjv.jinqigfzy.top

t = time.perf_counter()
来源：http://kee.gotoacloud.top

[U16] Py：命令行参数解析
来源：http://xpz.shanyushiyangtech.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iti.bbcook.cn

[U17] Py：初始化日志
来源：http://tnc.haohaochexian.top

logging.basicConfig(level=logging.INFO)
来源：http://rsm.redwolf501.top

[U18] Py：预编译正则
来源：http://qdr.cdnleiting.top

pat = re.compile(r"\d+")
来源：http://zvi.fzhhl.top

[U19] Py：正则替换带回调
来源：http://ixt.chenjidiqi.icu

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eyu.zhengqikj.top

[U20] Py：缓存函数结果
来源：http://edh.bbcook.cn

@functools.lru_cache(maxsize=None)
来源：http://nwz.gzhubu.top

[U21] Py：自定义上下文管理器
来源：http://eje.tarul.cn

@contextlib.contextmanager
来源：http://pzc.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://fdi.jinyuanbaomall.cn

list(zip(*m))
来源：http://nvu.9152youxi.cn

[U23] Py：分块读取大文件
来源：http://zhh.chenjidiqi.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nud.fehbvm.com

[U24] Py：路径操作
来源：http://xqv.cashguo.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xvj.jinqigfzy.top

[U25] Py：CSV 按字典读
来源：http://mgh.redwolf501.top

csv.DictReader(f)
来源：http://lsb.shangyingyoupin.top

[U26] Py：并发下载
来源：http://icb.sufxvd.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nbr.zhoulong.xyz

[U27] Py：异步 HTTP
来源：http://fkg.xingfuxueyuan.xyz

aiohttp.ClientSession() 配合 async with
来源：http://ust.ivvv.top

[U28] Py：类型别名
来源：http://yyh.sysykeji.top

UserId = int
来源：http://ghi.hesvh.cn

[U29] Py：属性校验
来源：http://orv.kuanghao11.cn

@property 与 @x.setter 配合
来源：http://fki.sufxvd.cn

[U30] Py：数据类
来源：http://qbw.nwbrower.top

@dataclass(slots=True)
来源：http://nog.sysykeji.top

[U31] Py：单测
来源：http://zku.aizwys.cn

python -m pytest -q
来源：http://tnu.hammf.cn

[U32] Py：代码格式化
来源：http://unq.316326.xyz

ruff format . && ruff check --fix .
来源：http://toe.xuetiantiany.cn

[U33] Py：打包发布
来源：http://teo.birdmap.top

python -m build  （依赖 pyproject.toml）
来源：http://vgd.uphjek.com

[U34] Py：判断编码
来源：http://hhe.yj202588.top

chardet.detect(raw)
来源：http://vgy.meibo888.top

[U35] Py：发送邮件
来源：http://znq.snrcjt.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tdl.yonumen.top

[U36] Py：定时任务
来源：http://cmd.316326.xyz

schedule.every(10).minutes.do(job)
来源：http://wau.sweek.top

[U37] Py：读写 Excel
来源：http://gjb.cucudq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hlp.jinqigfzy.top

[U38] Py：获取脚本所在目录
来源：http://sus.xziqi.cn

Path(__file__).resolve().parent
来源：http://epx.hnxiangtu.top

[U39] Py：判断是否在交互环境
来源：http://hzx.havefunace.top

sys.stdout.isatty()
来源：http://reu.shangyingyoupin.top

[U40] Py：打印到标准错误
来源：http://yqw.bjfxy.top

print("err", file=sys.stderr)
来源：http://ncr.yvedp.cn

[U41] PHP：初始化 Composer 项目
来源：http://puu.gaohongyu789.top

composer init;  composer require guzzlehttp/guzzle
来源：http://pbg.yj20258.top

[U42] PHP：PSR-4 自动加载
来源：http://lja.mhx1999.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qeg.nanxinkj.top

[U43] PHP：声明命名空间
来源：http://mvg.yangfankeji.com

namespace App\Http;
来源：http://zjm.zhixingplan.top

[U44] PHP：开启严格类型
来源：http://rnf.0kj1m.cn

declare(strict_types=1);
来源：http://tjz.tanke756.top

[U45] PHP：类型声明与返回类型
来源：http://gnu.snrcjt.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kzg.shuidangran.top

[U46] PHP：可空类型
来源：http://yge.ydzc1.top

?string $name = null
来源：http://zwk.yj202588.top

[U47] PHP：联合类型
来源：http://fte.nwbrower.top

int|string $id
来源：http://fjm.gaohongyu789.top

[U48] PHP：纯枚举
来源：http://umx.nanxinkj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dnq.dashuyun.cn

[U49] PHP：只读属性
来源：http://say.jinghuilouyu.cn

public readonly string $name
来源：http://ilp.shzxlz.cn

[U50] PHP：构造器属性提升
来源：http://rxh.daxiang520.top

public function __construct(private int $id) {}
来源：http://ddp.mhx1999.top

[U51] PHP：数组解构
来源：http://lkz.ctjpmb.com

[$a, $b] = $arr;
来源：http://ssa.meibo888.top

[U52] PHP：箭头函数
来源：http://net.ehwqpu.com

$double = fn($x) => $x * 2;
来源：http://apq.svipenyu.cn

[U53] PHP：空合并运算符
来源：http://pip.pengpengdd.cyou

$v = $a ?? $b ?? "default";
来源：http://evk.ctjpmb.com

[U54] PHP：空安全调用
来源：http://nnn.vehdjk.com

$obj?->method()
来源：http://cto.dashuyun.cn

[U55] PHP：match 表达式
来源：http://zzd.tanke756.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rsg.yanxiufei.cn

[U56] PHP：命名参数
来源：http://zsf.nanxuanxn.top

f(a: 1, b: 2)
来源：http://szy.zhiwuduotai.top

[U57] PHP：字符串插值
来源：http://wld.shanyushiyangkeji.top

"值: {$a}"
来源：http://bzo.iojbl.cn

[U58] PHP：数组三件套
来源：http://rst.nanxinkj.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rws.guannengcc.top

[U59] PHP：自定义排序
来源：http://zxo.aizwys.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://epf.yongpay.top

[U60] PHP：JSON 编解码
来源：http://ipl.redwolf501.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lca.xingfuxueyuan.xyz

[U61] PHP：正则
来源：http://bsx.meibo888.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lsk.bbcook.cn

[U62] PHP：日期对象
来源：http://ovz.shzxlz.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fst.yj202588.top

[U63] PHP：文件读写
来源：http://jap.shangyingyoupin.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dhv.zhiwuduotai.top

[U64] PHP：目录遍历
来源：http://qwf.uphjek.com

glob("dir/*.php");  scandir("dir");
来源：http://wau.chenlongwang.top

[U65] PHP：会话
来源：http://fxn.jinqigfzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://tit.bbcook.cn

[U66] PHP：设置 Cookie
来源：http://umd.yj20258888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://txt.guowangkeji.top

[U67] PHP：处理文件上传
来源：http://fkn.cdnleiting.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iph.jqgfzy.top

[U68] PHP：PDO 连接
来源：http://thj.fanxiaobao.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mmj.shzxlz.cn

[U69] PHP：PDO 预处理
来源：http://cwq.jinqigufen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ufl.xziqi.cn

[U70] PHP：PDO 事务
来源：http://gaf.wangshuangyany.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ugl.chenjidiqi.icu

[U71] PHP：抛出异常
来源：http://ebe.redwolf501.top

throw new RuntimeException("失败", 500);
来源：http://cxo.ivvv.top

[U72] PHP：写错误日志
来源：http://qbv.andypj.xyz

error_log("失败: " . $e->getMessage());
来源：http://geo.tian-w.cn

[U73] PHP：读取 ini 配置
来源：http://mzh.zhoulong.xyz

parse_ini_file("config.ini", true)
来源：http://grw.snrcjt.cn

[U74] PHP：读取环境变量
来源：http://kqz.vqdsnc.cn

getenv("APP_ENV") ?: "production"
来源：http://kro.nanxinkj.top

[U75] PHP：依赖注入
来源：http://prr.sxryk.cn

composer require psr/container
来源：http://gcn.xuetiantiany.cn

[U76] PHP：简单路由
来源：http://ljr.andypj.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dtj.yj202588.top

[U77] PHP：模板渲染
来源：http://agz.chenjidiqi.icu

composer require twig/twig
来源：http://ibx.aibaodan.cn

[U78] PHP：单元测试
来源：http://spi.sufxvd.cn

composer require --dev phpunit/phpunit
来源：http://wyf.zhiwuduotai.top

[U79] PHP：静态分析
来源：http://bao.epnwcf.com

composer require --dev phpstan/phpstan
来源：http://uyn.tarul.cn

[U80] PHP：代码规范修复
来源：http://izc.xylfe.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jcf.xuetiantiany.cn

[U81] JS：初始化项目
来源：http://pcf.daria6918.cn

npm init -y;  npm i express
来源：http://ybe.ivvv.top

[U82] JS：package.json 脚本
来源：http://xuu.pycfn.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://can.sxryk.cn


<!-- 参考信息 -->