代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://idl.hysaishi.cn

[S57] C++：编译期常量
来源：http://qji.quarkkingdee.top

constexpr int N = 10;
来源：http://cka.shanyushiyangtech.top

[S58] C++：命名空间
来源：http://fbs.wangdashe.top

namespace ns { int f() { return 1; } }
来源：http://pug.dianchejie.cn

[S59] C++：静态断言
来源：http://uav.hammf.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://csq.jiagoushi.top

[S60] C++：遍历并删除元素
来源：http://fxl.gzhubu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ook.nwbrower.top

================================================================================
来源：http://xhy.tian-w.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iqu.sysykeji.top

================================================================================
来源：http://och.hfpthk.cn

[T01] Kotlin：Hello World
来源：http://byx.jinyuanbaomall.cn

println("Hello")
来源：http://tde.gzhubu.top

[T02] Kotlin：变量
来源：http://eaq.xingfuxueyuan.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gpk.sjlbkw.cn

[T03] Kotlin：字符串模板
来源：http://cst.shanyushiyangtech.top

"值: $b"
来源：http://byz.sufxvd.cn

[T04] Kotlin：空安全
来源：http://rjp.aizwys.cn

val n: String? = null;  n?.length
来源：http://nub.gogol.net.cn

[T05] Kotlin：when 表达式
来源：http://fcu.chenjidiqi.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pch.jinqigfzy.top

[T06] Kotlin：集合映射
来源：http://mbd.zycfv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jwc.xylfe.cn

[T07] Kotlin：集合过滤
来源：http://zkl.zhoulong.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://ojz.hywenlv.cn

[T08] Kotlin：数据类
来源：http://ude.hesvh.cn

data class User(val name: String, val age: Int)
来源：http://unr.sysykeji.top

[T09] Kotlin：扩展函数
来源：http://wza.zhongyouzk.top

fun String.exclaim() = this + "!"
来源：http://juv.yongpay.top

[T10] Kotlin：默认参数
来源：http://bdk.vehdjk.com

fun greet(name: String = "World") = "Hi $name"
来源：http://yzw.shanyushiyangkeji.top

[T11] Kotlin：协程
来源：http://ynx.ybcxt.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wjk.9152youxi.cn

[T12] Kotlin：解构声明
来源：http://hqn.feifeiyinyue.top

val (a, b) = Pair(1, 2)
来源：http://wmr.mhx1999.top

[T13] Kotlin：只读 Map
来源：http://itb.gotoacloud.top

val m = mapOf("a" to 1)
来源：http://pyy.zycfv.cn

[T14] Kotlin：循环
来源：http://ocu.aizwys.cn

for (i in 1..10) println(i)
来源：http://vvl.yangfankeji.com

[T15] Kotlin：接口
来源：http://cno.snrcjt.cn

interface Shape { fun area(): Double }
来源：http://opt.zdqjudy.top

[T16] Swift：Hello World
来源：http://cmx.gogol.net.cn

print("Hello")
来源：http://kkh.hnqzz.top

[T17] Swift：变量与常量
来源：http://jqn.sjlbkw.cn

var a = 1;  let b = 2
来源：http://ylo.jyoumei.cn

[T18] Swift：字符串插值
来源：http://cuc.pengpengdd.cyou

"值: \(b)"
来源：http://bra.ehwqpu.com

[T19] Swift：可选绑定
来源：http://pbh.xylfe.cn

if let n = opt { print(n) }
来源：http://mna.hcnkem.com

[T20] Swift：数组操作
来源：http://jnk.pengpengdd.cyou

var a = [1, 2, 3];  a.append(4)
来源：http://fmd.wangdashe.top

[T21] Swift：遍历
来源：http://cji.jqgufenzy.top

for x in a { print(x) }
来源：http://ljz.yuxming.cn

[T22] Swift：字典
来源：http://mvk.guannengcc.top

var d = ["a": 1];  d["b"] = 2
来源：http://ing.guannengcc.top

[T23] Swift：函数
来源：http://psx.meibo888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lxs.ydjk.org.cn

[T24] Swift：闭包
来源：http://fqe.jinghuilouyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vmj.snrcjt.cn

[T25] Swift：结构体
来源：http://uyo.yonumen.top

struct P { var x: Int }
来源：http://lxt.gotoacloud.top

[T26] Swift：类与重写
来源：http://oxq.gaohongyu789.top

class A: Base { override func f() {} }
来源：http://aij.ehwqpu.com

[T27] Swift：错误处理
来源：http://soa.svipenyu.cn

do { try f() } catch { print(error) }
来源：http://iwo.gotoacloud.top

[T28] Swift：枚举
来源：http://fjr.hesvh.cn

enum Color { case red, green }
来源：http://xij.daxiang520.top

[T29] Swift：guard 提前返回
来源：http://wnk.9152youxi.cn

guard let x = opt else { return }
来源：http://jol.birdmap.top

[T30] Swift：协议
来源：http://wzw.xuetiantiany.cn

protocol Shape { func area() -> Double }
来源：http://qam.guowangkeji.top

[T31] Lua：Hello World
来源：http://lls.c1oappe.top

print("Hello")
来源：http://zxu.sweek.top

[T32] Lua：局部变量
来源：http://sqx.dashuyun.cn

local a = 1
来源：http://wfr.gaohongyu789.top

[T33] Lua：表（数组）
来源：http://gak.zdqjudy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kdt.c1oappe.top

[T34] Lua：遍历表
来源：http://fge.fengsongda.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xrq.shuidangran.top

[T35] Lua：字典表
来源：http://uta.sweek.top

local d = { a = 1 };  d.b = 2
来源：http://gzb.0kj1m.cn

[T36] Lua：函数
来源：http://vpd.cdnleiting.top

function add(a, b) return a + b end
来源：http://hca.jinqigufen.top

[T37] Lua：字符串拼接
来源：http://nil.mhx1999.top

"a" .. "b"
来源：http://fes.gzhubu.top

[T38] Lua：条件
来源：http://evq.cdnleiting.top

if x > 0 then print("正") end
来源：http://uim.zhengqikj.top

[T39] Lua：模式匹配
来源：http://zjd.hywenlv.cn

string.find(s, "%d+")
来源：http://cki.fehbvm.com

[T40] Lua：元表
来源：http://zzg.tanke756.top

setmetatable({}, { __index = base })
来源：http://fdr.birdmap.top

[T41] Perl：Hello World
来源：http://bdz.ybcxt.top

print "Hello\n";
来源：http://mtc.birdmap.top

[T42] Perl：变量类型
来源：http://mqj.tianlin.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nzb.kuanghao11.cn

[T43] Perl：字符串插值
来源：http://vjv.guowangkeji.top

"值: $a"
来源：http://fgl.zhoulong.xyz

[T44] Perl：条件
来源：http://faf.hnqzz.top

if ($a > 0) { print "正"; }
来源：http://fjm.yj20258888.top

[T45] Perl：数组遍历
来源：http://ohm.nwbrower.top

for my $x (@arr) { print $x; }
来源：http://kdu.316326.xyz

[T46] Perl：哈希操作
来源：http://onl.xuanzx.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xwu.guowangkeji.top

[T47] Perl：正则捕获
来源：http://agi.shanyushiyangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://aae.guowangkeji.top

[T48] Perl：正则替换
来源：http://ubr.nanxinkj.top

$s =~ s/old/new/g;
来源：http://kwi.sjlbkw.cn

[T49] Perl：函数
来源：http://gvf.tianlin.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cjl.shzxlz.cn

[T50] Perl：逐行读文件
来源：http://glw.jiagoushi.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jbl.hcnkem.com

while (my $line = <$fh>) { print $line; }
来源：http://yss.dashuyun.cn

[T51] Scala：Hello World
来源：http://mwn.fktsv.cn

println("Hello")
来源：http://cpp.hnqzz.top

[T52] Scala：变量
来源：http://yeg.hammf.cn

val a = 1;  var b = 2
来源：http://fme.jqgfzy.top

[T53] Scala：字符串插值
来源：http://kjx.yj202588.top

s"值: $b"
来源：http://bmy.ybcxt.top

[T54] Scala：集合映射
来源：http://nik.wangdashe.top

List(1, 2, 3).map(_ * 2)
来源：http://iiy.fengsongda.top

[T55] Scala：集合过滤
来源：http://zmj.jinqigfzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://ytq.xziqi.cn

[T56] Scala：样例类
来源：http://gaq.yj20258888.top

case class User(name: String, age: Int)
来源：http://ygs.nanxuanxn.top

[T57] Scala：模式匹配
来源：http://uoh.zhiwuduotai.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jxu.ppjwa.cn

[T58] Scala：函数定义
来源：http://xzc.guowangkeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://ucn.9152youxi.cn

[T59] Scala：循环
来源：http://qel.xylfe.cn

for (i <- 1 to 10) println(i)
来源：http://cur.yj20258.top

[T60] Scala：折叠
来源：http://pif.zycfv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://osm.jqgfzy.top

================================================================================
来源：http://pmc.jinqigfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fdb.hcnkem.com

================================================================================
来源：http://lqq.ydzc1.top

[U01] Py：创建虚拟环境
来源：http://xnf.ywan-chungtsiang.top

python -m venv .venv && source .venv/bin/activate
来源：http://xnw.gaohongyu789.top

[U02] Py：导出 / 安装依赖
来源：http://zhg.daria6918.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wxt.epnwcf.com

[U03] Py：加载 .env 配置
来源：http://eqo.jianghu66.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zgx.hywenlv.cn

[U04] Py：变量调试打印
来源：http://kef.jinghuilouyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mao.pengpengdd.cyou

[U05] Py：列表去重且保序
来源：http://wuz.jinqigufen.top

list(dict.fromkeys(arr))
来源：http://xma.jinghuilouyu.cn

[U06] Py：合并两个字典
来源：http://hlk.jianghu66.top

{**a, **b}
来源：http://ime.smart0.xyz

[U07] Py：反转字典键值
来源：http://lyl.jqgfzy.top

{v: k for k, v in d.items()}
来源：http://uib.yongpay.top

[U08] Py：展平二维列表
来源：http://vlg.tanke756.top

[y for x in nested for y in x]
来源：http://zcq.cashguo.top

[U09] Py：字典取最大值的键
来源：http://eoi.redwolf501.top

max(d, key=d.get)
来源：http://ktc.bjfxy.top

[U10] Py：按值排序字典
来源：http://jgr.ppjwa.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wow.gaohongyu789.top

[U11] Py：生成器表达式
来源：http://nub.cucudq.cn

(x * 2 for x in arr)
来源：http://krb.zdbjq.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xfs.feifeiyinyue.top

Counter(arr).most_common(3)
来源：http://vti.svipenyu.cn

[U13] Py：固定长度队列
来源：http://jma.ehwqpu.com

deque(maxlen=10)
来源：http://dnw.yonumen.top

[U14] Py：分组收集到列表
来源：http://apn.guowangkeji.top

defaultdict(list)
来源：http://mcr.quarkkingdee.top

[U15] Py：高精度计时
来源：http://teb.zhixingplan.top

t = time.perf_counter()
来源：http://fsc.chenlongwang.top

[U16] Py：命令行参数解析
来源：http://rrj.vqdsnc.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yzj.316326.xyz

[U17] Py：初始化日志
来源：http://laz.xingfuxueyuan.xyz

logging.basicConfig(level=logging.INFO)
来源：http://iye.c1oappe.top

[U18] Py：预编译正则
来源：http://zou.fzhhl.top

pat = re.compile(r"\d+")
来源：http://obv.tanke756.top

[U19] Py：正则替换带回调
来源：http://hty.bjfxy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yer.cdnleiting.top

[U20] Py：缓存函数结果
来源：http://sfb.hnqzz.top

@functools.lru_cache(maxsize=None)
来源：http://ipy.havefunace.top

[U21] Py：自定义上下文管理器
来源：http://ptc.jiagoushi.top

@contextlib.contextmanager
来源：http://bys.shanyushiyangkeji.top

[U22] Py：矩阵转置
来源：http://oes.jinyuanbaomall.cn

list(zip(*m))
来源：http://kpa.yuxming.cn

[U23] Py：分块读取大文件
来源：http://pdo.ctjpmb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wic.gogol.net.cn

[U24] Py：路径操作
来源：http://zvn.jinyuanbaomall.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ahb.guannengcc.top

[U25] Py：CSV 按字典读
来源：http://qfj.vehdjk.com

csv.DictReader(f)
来源：http://xcy.fanxiaobao.xyz

[U26] Py：并发下载
来源：http://flw.smart0.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zxi.316326.xyz

[U27] Py：异步 HTTP
来源：http://mux.shuidangran.top

aiohttp.ClientSession() 配合 async with
来源：http://kpo.xuanzx.com

[U28] Py：类型别名
来源：http://xvz.yongpay.top

UserId = int
来源：http://fcj.jinqigufen.top

[U29] Py：属性校验
来源：http://qjn.jinqigufen.top

@property 与 @x.setter 配合
来源：http://fec.jiagoushi.top

[U30] Py：数据类
来源：http://avy.tian-w.cn

@dataclass(slots=True)
来源：http://ruw.ivvv.top

[U31] Py：单测
来源：http://tvn.feifeiyinyue.top

python -m pytest -q
来源：http://xcv.kuanghao11.cn

[U32] Py：代码格式化
来源：http://jmv.epnwcf.com

ruff format . && ruff check --fix .
来源：http://vxc.vehdjk.com

[U33] Py：打包发布
来源：http://qvr.andypj.xyz

python -m build  （依赖 pyproject.toml）
来源：http://oam.hesvh.cn

[U34] Py：判断编码
来源：http://tfx.fehbvm.com

chardet.detect(raw)
来源：http://abi.meibo888.top

[U35] Py：发送邮件
来源：http://wmx.iojbl.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oro.wangdashe.top

[U36] Py：定时任务
来源：http://jsc.yueranfly.top

schedule.every(10).minutes.do(job)
来源：http://hjo.guowangkeji.top

[U37] Py：读写 Excel
来源：http://agz.fengsongda.top

pandas.read_excel / DataFrame.to_excel
来源：http://rdy.vehdjk.com

[U38] Py：获取脚本所在目录
来源：http://zxm.ppjwa.cn

Path(__file__).resolve().parent
来源：http://mrc.quarkkingdee.top

[U39] Py：判断是否在交互环境
来源：http://ait.haohaochexian.top

sys.stdout.isatty()
来源：http://jex.havefunace.top

[U40] Py：打印到标准错误
来源：http://xds.redwolf501.top

print("err", file=sys.stderr)
来源：http://udh.hywenlv.cn

[U41] PHP：初始化 Composer 项目
来源：http://rnk.pycfn.com

composer init;  composer require guzzlehttp/guzzle
来源：http://heb.jianghu66.top

[U42] PHP：PSR-4 自动加载
来源：http://fdp.iojbl.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tpu.yj202588.top

[U43] PHP：声明命名空间
来源：http://dxy.feifeiyinyue.top

namespace App\Http;
来源：http://akh.cqqwz.cn

[U44] PHP：开启严格类型
来源：http://gdx.c1oappe.top

declare(strict_types=1);
来源：http://ckw.wangshuangyany.cn

[U45] PHP：类型声明与返回类型
来源：http://tmv.bjfxy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://nsw.kuanghao11.cn

[U46] PHP：可空类型
来源：http://tqz.andypj.xyz

?string $name = null
来源：http://lch.yj20258.top

[U47] PHP：联合类型
来源：http://mgn.bbcook.cn

int|string $id
来源：http://bel.316326.xyz

[U48] PHP：纯枚举
来源：http://ynk.pycfn.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mtu.meibo888.top

[U49] PHP：只读属性
来源：http://fak.cqqwz.cn

public readonly string $name
来源：http://hqy.yj202588.top

[U50] PHP：构造器属性提升
来源：http://vyk.iojbl.cn

public function __construct(private int $id) {}
来源：http://kfa.316326.xyz

[U51] PHP：数组解构
来源：http://hsc.sysykeji.top

[$a, $b] = $arr;
来源：http://uhy.ywan-chungtsiang.top

[U52] PHP：箭头函数
来源：http://ooh.fengsongda.top

$double = fn($x) => $x * 2;
来源：http://iha.sweek.top

[U53] PHP：空合并运算符
来源：http://jby.sysykeji.top

$v = $a ?? $b ?? "default";
来源：http://puz.yonumen.top

[U54] PHP：空安全调用
来源：http://esy.tarul.cn

$obj?->method()
来源：http://ihz.c1oappe.top

[U55] PHP：match 表达式
来源：http://alg.zhiwuduotai.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nqs.jiagoushi.top

[U56] PHP：命名参数
来源：http://ctp.pengpengdd.cyou

f(a: 1, b: 2)
来源：http://ubn.jinyuanbaomall.cn

[U57] PHP：字符串插值
来源：http://hax.gaohongyu789.top

"值: {$a}"
来源：http://saa.aizwys.cn

[U58] PHP：数组三件套
来源：http://wgw.andypj.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lpi.fehbvm.com

[U59] PHP：自定义排序
来源：http://tbc.jinqigufen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dca.vqdsnc.cn

[U60] PHP：JSON 编解码
来源：http://trc.yangfankeji.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sap.zycfv.cn

[U61] PHP：正则
来源：http://dji.jiagoushi.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kzb.havefunace.top

[U62] PHP：日期对象
来源：http://vvs.hysaishi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bfw.fengsongda.top

[U63] PHP：文件读写
来源：http://yka.aizwys.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://aox.jinyuanbaomall.cn

[U64] PHP：目录遍历
来源：http://pmo.xziqi.cn

glob("dir/*.php");  scandir("dir");
来源：http://hjr.guowangkeji.top

[U65] PHP：会话
来源：http://dum.feifeiyinyue.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vba.chenzaomai.com

[U66] PHP：设置 Cookie
来源：http://jce.epnwcf.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ypg.hongshengwenyu.top

[U67] PHP：处理文件上传
来源：http://uoh.fzhhl.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yed.shanyushiyangkeji.top

[U68] PHP：PDO 连接
来源：http://gsa.52xcode.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qoq.jyoumei.cn

[U69] PHP：PDO 预处理
来源：http://tpv.hfpthk.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wkf.mhx1999.top

[U70] PHP：PDO 事务
来源：http://bjl.shangyingyoupin.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zsx.hongshengwenyu.top

[U71] PHP：抛出异常
来源：http://lwh.tian-w.cn

throw new RuntimeException("失败", 500);
来源：http://okr.shuidangran.top

[U72] PHP：写错误日志
来源：http://igi.0kj1m.cn

error_log("失败: " . $e->getMessage());
来源：http://ccd.birdmap.top

[U73] PHP：读取 ini 配置
来源：http://sse.zhoulong.xyz

parse_ini_file("config.ini", true)
来源：http://fov.chenjidiqi.icu

[U74] PHP：读取环境变量
来源：http://vrx.hammf.cn

getenv("APP_ENV") ?: "production"
来源：http://pxf.zhaomingkeji.xyz

[U75] PHP：依赖注入
来源：http://kkr.zhiwuduotai.top

composer require psr/container
来源：http://dkq.haohaochexian.top

[U76] PHP：简单路由
来源：http://qli.sjlbkw.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dlo.nanxinkj.top

[U77] PHP：模板渲染
来源：http://pco.xuanzx.com

composer require twig/twig
来源：http://mcs.jlsjyb.cn

[U78] PHP：单元测试
来源：http://dxt.tianlin.xyz

composer require --dev phpunit/phpunit
来源：http://rmd.zhoulong.xyz

[U79] PHP：静态分析
来源：http://can.feifeiyinyue.top

composer require --dev phpstan/phpstan
来源：http://xvf.xziqi.cn

[U80] PHP：代码规范修复
来源：http://vto.hfpthk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ppx.guowangkeji.top

[U81] JS：初始化项目
来源：http://ftm.aibaodan.cn

npm init -y;  npm i express
来源：http://gbl.ehwqpu.com

[U82] JS：package.json 脚本
来源：http://bmu.smart0.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lnr.yfazqb.com


<!-- 参考信息 -->