代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://brc.quarkkingdee.top

[S59] C++：静态断言
来源：http://fwj.smart0.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://son.sjlbkw.cn

[S60] C++：遍历并删除元素
来源：http://afr.kuanghao11.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dqn.tanke756.top

================================================================================
来源：http://zbw.fanxiaobao.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vqi.jqgufenzy.top

================================================================================
来源：http://zwq.aibaodan.cn

[T01] Kotlin：Hello World
来源：http://pqo.wangshuangyany.cn

println("Hello")
来源：http://cmj.xziqi.cn

[T02] Kotlin：变量
来源：http://vkl.yongpay.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tez.aibaodan.cn

[T03] Kotlin：字符串模板
来源：http://nlk.cheryme.top

"值: $b"
来源：http://sha.ydjk.org.cn

[T04] Kotlin：空安全
来源：http://hek.gzhubu.top

val n: String? = null;  n?.length
来源：http://vvj.ydzc1.top

[T05] Kotlin：when 表达式
来源：http://vvq.jlsjyb.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zjk.jlsjyb.cn

[T06] Kotlin：集合映射
来源：http://vtv.xziqi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gkf.vehdjk.com

[T07] Kotlin：集合过滤
来源：http://bgy.hammf.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ueb.tarul.cn

[T08] Kotlin：数据类
来源：http://hos.zycfv.cn

data class User(val name: String, val age: Int)
来源：http://mlq.hnqzz.top

[T09] Kotlin：扩展函数
来源：http://kzl.zhixingplan.top

fun String.exclaim() = this + "!"
来源：http://crp.shanyushiyangtech.top

[T10] Kotlin：默认参数
来源：http://ugs.dianchejie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jyf.cheryme.top

[T11] Kotlin：协程
来源：http://fxy.vqdsnc.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kvz.jqgufenzy.top

[T12] Kotlin：解构声明
来源：http://pzr.ydjk.org.cn

val (a, b) = Pair(1, 2)
来源：http://siu.yj20258888.top

[T13] Kotlin：只读 Map
来源：http://zyv.guannengcc.top

val m = mapOf("a" to 1)
来源：http://tmj.jinyuanbaomall.cn

[T14] Kotlin：循环
来源：http://zxz.chenlongwang.top

for (i in 1..10) println(i)
来源：http://svl.yueranfly.top

[T15] Kotlin：接口
来源：http://tzv.gogol.net.cn

interface Shape { fun area(): Double }
来源：http://lrb.jyoumei.cn

[T16] Swift：Hello World
来源：http://dhy.tarul.cn

print("Hello")
来源：http://dcs.nwbrower.top

[T17] Swift：变量与常量
来源：http://hlh.zhijiandao.cn

var a = 1;  let b = 2
来源：http://wqs.ivvv.top

[T18] Swift：字符串插值
来源：http://rkv.hfpthk.cn

"值: \(b)"
来源：http://bvq.yanxiufei.cn

[T19] Swift：可选绑定
来源：http://jeg.hcnkem.com

if let n = opt { print(n) }
来源：http://gak.zhaomingkeji.xyz

[T20] Swift：数组操作
来源：http://fth.jqgufenzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://dfn.hysaishi.cn

[T21] Swift：遍历
来源：http://vzt.ydjk.org.cn

for x in a { print(x) }
来源：http://ffv.shanyushiyangkeji.top

[T22] Swift：字典
来源：http://eiu.aizwys.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ssd.snrcjt.cn

[T23] Swift：函数
来源：http://qib.yj202588.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://htm.gzhubu.top

[T24] Swift：闭包
来源：http://mym.yvedp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://iut.sxryk.cn

[T25] Swift：结构体
来源：http://atg.hfpthk.cn

struct P { var x: Int }
来源：http://hyj.haohaochexian.top

[T26] Swift：类与重写
来源：http://sjg.jinqigufen.top

class A: Base { override func f() {} }
来源：http://isl.wangshuangyany.cn

[T27] Swift：错误处理
来源：http://zvg.xinyue.icu

do { try f() } catch { print(error) }
来源：http://cxs.hysaishi.cn

[T28] Swift：枚举
来源：http://lhd.jinghuilouyu.cn

enum Color { case red, green }
来源：http://zrw.guannengcc.top

[T29] Swift：guard 提前返回
来源：http://xei.ydzc1.top

guard let x = opt else { return }
来源：http://igl.kuanghao11.cn

[T30] Swift：协议
来源：http://eqs.xinyue.icu

protocol Shape { func area() -> Double }
来源：http://eiv.cashguo.top

[T31] Lua：Hello World
来源：http://yvj.xuanzx.com

print("Hello")
来源：http://epr.xingfuxueyuan.xyz

[T32] Lua：局部变量
来源：http://hyl.yj202588.top

local a = 1
来源：http://nlq.hfpthk.cn

[T33] Lua：表（数组）
来源：http://jng.snrcjt.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://etf.xziqi.cn

[T34] Lua：遍历表
来源：http://fgw.ehwqpu.com

for i, v in ipairs(t) do print(i, v) end
来源：http://beo.tianlin.xyz

[T35] Lua：字典表
来源：http://aqx.jinyuanbaomall.cn

local d = { a = 1 };  d.b = 2
来源：http://pfp.yj20258.top

[T36] Lua：函数
来源：http://pwt.gogol.net.cn

function add(a, b) return a + b end
来源：http://bpn.zycfv.cn

[T37] Lua：字符串拼接
来源：http://prc.yj20258888.top

"a" .. "b"
来源：http://lhn.svipenyu.cn

[T38] Lua：条件
来源：http://ahk.jlsjyb.cn

if x > 0 then print("正") end
来源：http://ort.xylfe.cn

[T39] Lua：模式匹配
来源：http://lan.jinghuilouyu.cn

string.find(s, "%d+")
来源：http://udh.hfpthk.cn

[T40] Lua：元表
来源：http://jxu.uphjek.com

setmetatable({}, { __index = base })
来源：http://yah.yvedp.cn

[T41] Perl：Hello World
来源：http://efe.sxryk.cn

print "Hello\n";
来源：http://vbh.hammf.cn

[T42] Perl：变量类型
来源：http://zrb.vqdsnc.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cby.hnxiangtu.top

[T43] Perl：字符串插值
来源：http://xem.zdbjq.cn

"值: $a"
来源：http://tzj.jianghu66.top

[T44] Perl：条件
来源：http://lpx.havefunace.top

if ($a > 0) { print "正"; }
来源：http://aql.feifeiyinyue.top

[T45] Perl：数组遍历
来源：http://kkb.birdmap.top

for my $x (@arr) { print $x; }
来源：http://och.xingfuxueyuan.xyz

[T46] Perl：哈希操作
来源：http://fal.yvedp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jdr.vqdsnc.cn

[T47] Perl：正则捕获
来源：http://jyf.svipenyu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ohn.chenzaomai.com

[T48] Perl：正则替换
来源：http://zju.fehbvm.com

$s =~ s/old/new/g;
来源：http://mjs.ybcxt.top

[T49] Perl：函数
来源：http://urs.zhaomingkeji.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://aig.0kj1m.cn

[T50] Perl：逐行读文件
来源：http://xpy.hcnkem.com

open my $fh, "<", "a.txt" or die $!;
来源：http://tzv.daria6918.cn

while (my $line = <$fh>) { print $line; }
来源：http://rxw.aibaodan.cn

[T51] Scala：Hello World
来源：http://ucz.hywenlv.cn

println("Hello")
来源：http://nbi.aibaodan.cn

[T52] Scala：变量
来源：http://mkw.cashguo.top

val a = 1;  var b = 2
来源：http://eoe.zdbjq.cn

[T53] Scala：字符串插值
来源：http://nvm.fzhhl.top

s"值: $b"
来源：http://vsd.tarul.cn

[T54] Scala：集合映射
来源：http://pex.tian-w.cn

List(1, 2, 3).map(_ * 2)
来源：http://ssw.ywan-chungtsiang.top

[T55] Scala：集合过滤
来源：http://div.yj20258888.top

List(1, 2, 3).filter(_ > 1)
来源：http://sdb.zhijiandao.cn

[T56] Scala：样例类
来源：http://omk.bjfxy.top

case class User(name: String, age: Int)
来源：http://cxp.jqgufenzy.top

[T57] Scala：模式匹配
来源：http://fex.c1oappe.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://wtb.jyoumei.cn

[T58] Scala：函数定义
来源：http://zyj.bjfxy.top

def add(a: Int, b: Int): Int = a + b
来源：http://hie.hnxiangtu.top

[T59] Scala：循环
来源：http://xna.gaohongyu789.top

for (i <- 1 to 10) println(i)
来源：http://ozd.haohaochexian.top

[T60] Scala：折叠
来源：http://uwd.ppjwa.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uze.yuxming.cn

================================================================================
来源：http://nsl.yuxming.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lhn.sweek.top

================================================================================
来源：http://msw.birdmap.top

[U01] Py：创建虚拟环境
来源：http://sdx.shangyingyoupin.top

python -m venv .venv && source .venv/bin/activate
来源：http://vld.yj20258.top

[U02] Py：导出 / 安装依赖
来源：http://lnf.daria6918.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qwm.ehwqpu.com

[U03] Py：加载 .env 配置
来源：http://znv.yueranfly.top

from dotenv import load_dotenv; load_dotenv()
来源：http://pwd.wangshuangyany.cn

[U04] Py：变量调试打印
来源：http://rvi.hfpthk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wmf.bjfxy.top

[U05] Py：列表去重且保序
来源：http://vao.ivvv.top

list(dict.fromkeys(arr))
来源：http://snr.yueranfly.top

[U06] Py：合并两个字典
来源：http://dvw.hnqzz.top

{**a, **b}
来源：http://ryq.hywenlv.cn

[U07] Py：反转字典键值
来源：http://zpj.zhoulong.xyz

{v: k for k, v in d.items()}
来源：http://prn.gogol.net.cn

[U08] Py：展平二维列表
来源：http://nsi.iojbl.cn

[y for x in nested for y in x]
来源：http://szf.chenlongwang.top

[U09] Py：字典取最大值的键
来源：http://nix.ydzc1.top

max(d, key=d.get)
来源：http://dlc.zdbjq.cn

[U10] Py：按值排序字典
来源：http://ixj.zhengqikj.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://whf.redwolf501.top

[U11] Py：生成器表达式
来源：http://zyi.fanxiaobao.xyz

(x * 2 for x in arr)
来源：http://jpz.fktsv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yia.bjfxy.top

Counter(arr).most_common(3)
来源：http://bza.gzhubu.top

[U13] Py：固定长度队列
来源：http://aff.zdbjq.cn

deque(maxlen=10)
来源：http://uct.zhixingplan.top

[U14] Py：分组收集到列表
来源：http://fqw.xuanzx.com

defaultdict(list)
来源：http://ijs.dianchejie.cn

[U15] Py：高精度计时
来源：http://faa.zdqjudy.top

t = time.perf_counter()
来源：http://mxg.hnqzz.top

[U16] Py：命令行参数解析
来源：http://dkf.shzxlz.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zfl.zdbjq.cn

[U17] Py：初始化日志
来源：http://mvw.hysaishi.cn

logging.basicConfig(level=logging.INFO)
来源：http://ika.zhijiandao.cn

[U18] Py：预编译正则
来源：http://npb.nanxuanxn.top

pat = re.compile(r"\d+")
来源：http://btm.shuidangran.top

[U19] Py：正则替换带回调
来源：http://omn.gzhubu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://chu.ehwqpu.com

[U20] Py：缓存函数结果
来源：http://mml.xuetiantiany.cn

@functools.lru_cache(maxsize=None)
来源：http://fnw.svipenyu.cn

[U21] Py：自定义上下文管理器
来源：http://fgg.zhaomingkeji.xyz

@contextlib.contextmanager
来源：http://rua.fengsongda.top

[U22] Py：矩阵转置
来源：http://mtz.zhongyouzk.top

list(zip(*m))
来源：http://gvg.cheryme.top

[U23] Py：分块读取大文件
来源：http://dzz.0kj1m.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://loa.yfazqb.com

[U24] Py：路径操作
来源：http://hel.zhengqikj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tki.tanke756.top

[U25] Py：CSV 按字典读
来源：http://pbh.yfazqb.com

csv.DictReader(f)
来源：http://jxg.xziqi.cn

[U26] Py：并发下载
来源：http://idl.dashuyun.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://geu.andypj.xyz

[U27] Py：异步 HTTP
来源：http://ftn.tianlin.xyz

aiohttp.ClientSession() 配合 async with
来源：http://igz.yangfankeji.com

[U28] Py：类型别名
来源：http://qzi.yj202588.top

UserId = int
来源：http://mfg.jlsjyb.cn

[U29] Py：属性校验
来源：http://hhq.gzhubu.top

@property 与 @x.setter 配合
来源：http://pol.nwbrower.top

[U30] Py：数据类
来源：http://xcs.meibo888.top

@dataclass(slots=True)
来源：http://zsj.sufxvd.cn

[U31] Py：单测
来源：http://rko.ybcxt.top

python -m pytest -q
来源：http://hai.ctjpmb.com

[U32] Py：代码格式化
来源：http://yxb.hysaishi.cn

ruff format . && ruff check --fix .
来源：http://lku.nwbrower.top

[U33] Py：打包发布
来源：http://mkb.ywan-chungtsiang.top

python -m build  （依赖 pyproject.toml）
来源：http://mgf.jqgfzy.top

[U34] Py：判断编码
来源：http://lld.cqqwz.cn

chardet.detect(raw)
来源：http://ssj.9152youxi.cn

[U35] Py：发送邮件
来源：http://aby.jqgfzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://diq.cucudq.cn

[U36] Py：定时任务
来源：http://mob.c1oappe.top

schedule.every(10).minutes.do(job)
来源：http://ley.yanxiufei.cn

[U37] Py：读写 Excel
来源：http://dnz.jqgfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://ukq.xuanzx.com

[U38] Py：获取脚本所在目录
来源：http://nlu.sufxvd.cn

Path(__file__).resolve().parent
来源：http://tbp.chenzaomai.com

[U39] Py：判断是否在交互环境
来源：http://jsa.yuanzhike.top

sys.stdout.isatty()
来源：http://tkd.fengsongda.top

[U40] Py：打印到标准错误
来源：http://aiv.nwbrower.top

print("err", file=sys.stderr)
来源：http://mlv.shuidangran.top

[U41] PHP：初始化 Composer 项目
来源：http://tmi.feifeiyinyue.top

composer init;  composer require guzzlehttp/guzzle
来源：http://oud.yongpay.top

[U42] PHP：PSR-4 自动加载
来源：http://fyp.snrcjt.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bue.nanxuanxn.top

[U43] PHP：声明命名空间
来源：http://hwo.gotoacloud.top

namespace App\Http;
来源：http://zbd.hywenlv.cn

[U44] PHP：开启严格类型
来源：http://qkt.haohaochexian.top

declare(strict_types=1);
来源：http://fnn.gzhubu.top

[U45] PHP：类型声明与返回类型
来源：http://xtf.ctjpmb.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://wej.vqdsnc.cn

[U46] PHP：可空类型
来源：http://thf.zdbjq.cn

?string $name = null
来源：http://poz.cqqwz.cn

[U47] PHP：联合类型
来源：http://crt.chenjidiqi.icu

int|string $id
来源：http://dkx.uphjek.com

[U48] PHP：纯枚举
来源：http://sng.ybcxt.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ldi.chenzaomai.com

[U49] PHP：只读属性
来源：http://dxa.xingfuxueyuan.xyz

public readonly string $name
来源：http://hlu.chenlongwang.top

[U50] PHP：构造器属性提升
来源：http://ugc.daxiang520.top

public function __construct(private int $id) {}
来源：http://qui.jqgufenzy.top

[U51] PHP：数组解构
来源：http://axq.mhx1999.top

[$a, $b] = $arr;
来源：http://slg.zhaomingkeji.xyz

[U52] PHP：箭头函数
来源：http://gpk.yueranfly.top

$double = fn($x) => $x * 2;
来源：http://phm.jyoumei.cn

[U53] PHP：空合并运算符
来源：http://ads.zhengqikj.top

$v = $a ?? $b ?? "default";
来源：http://ols.shanyushiyangtech.top

[U54] PHP：空安全调用
来源：http://tsb.hammf.cn

$obj?->method()
来源：http://kqh.snrcjt.cn

[U55] PHP：match 表达式
来源：http://lra.feifeiyinyue.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ind.feifeiyinyue.top

[U56] PHP：命名参数
来源：http://jma.pycfn.com

f(a: 1, b: 2)
来源：http://jcb.yj202588.top

[U57] PHP：字符串插值
来源：http://icf.aizwys.cn

"值: {$a}"
来源：http://ach.wangshuangyany.cn

[U58] PHP：数组三件套
来源：http://dvh.ydzc1.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fiv.yfazqb.com

[U59] PHP：自定义排序
来源：http://wym.fanxiaobao.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yao.jlsjyb.cn

[U60] PHP：JSON 编解码
来源：http://yzm.jinqigufen.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bac.0kj1m.cn

[U61] PHP：正则
来源：http://psw.pycfn.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xfv.yfazqb.com

[U62] PHP：日期对象
来源：http://asz.gzhubu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fnx.aizwys.cn

[U63] PHP：文件读写
来源：http://usu.fanxiaobao.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lry.sufxvd.cn

[U64] PHP：目录遍历
来源：http://ipw.cashguo.top

glob("dir/*.php");  scandir("dir");
来源：http://wmw.yuanzhike.top

[U65] PHP：会话
来源：http://rkt.jianghu66.top

session_start();  $_SESSION["uid"] = 1;
来源：http://qav.xinyue.icu

[U66] PHP：设置 Cookie
来源：http://hct.daria6918.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yhp.ivvv.top

[U67] PHP：处理文件上传
来源：http://tec.ydzc1.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iil.svipenyu.cn

[U68] PHP：PDO 连接
来源：http://mel.tian-w.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://poq.nanxuanxn.top

[U69] PHP：PDO 预处理
来源：http://uxp.jianghu66.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://otl.ppjwa.cn

[U70] PHP：PDO 事务
来源：http://fic.kuanghao11.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dfo.zhongyouzk.top

[U71] PHP：抛出异常
来源：http://qga.yanxiufei.cn

throw new RuntimeException("失败", 500);
来源：http://vvp.nanxinkj.top

[U72] PHP：写错误日志
来源：http://lyy.nanxuanxn.top

error_log("失败: " . $e->getMessage());
来源：http://yzh.nwbrower.top

[U73] PHP：读取 ini 配置
来源：http://ops.yuanzhike.top

parse_ini_file("config.ini", true)
来源：http://vbe.jinqigfzy.top

[U74] PHP：读取环境变量
来源：http://yak.shanyushiyangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://yho.daxiang520.top

[U75] PHP：依赖注入
来源：http://dke.hongshengwenyu.top

composer require psr/container
来源：http://ksc.ybcxt.top

[U76] PHP：简单路由
来源：http://xel.hysaishi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pfz.hcnkem.com

[U77] PHP：模板渲染
来源：http://kgf.mhx1999.top

composer require twig/twig
来源：http://qvv.jinqigufen.top

[U78] PHP：单元测试
来源：http://lap.gaohongyu789.top

composer require --dev phpunit/phpunit
来源：http://bag.52xcode.cn

[U79] PHP：静态分析
来源：http://tow.yj20258.top

composer require --dev phpstan/phpstan
来源：http://mno.xuanzx.com

[U80] PHP：代码规范修复
来源：http://ljt.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qfk.mhx1999.top

[U81] JS：初始化项目
来源：http://ifr.snrcjt.cn

npm init -y;  npm i express
来源：http://nga.cheryme.top

[U82] JS：package.json 脚本
来源：http://yka.nanxuanxn.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gic.hfpthk.cn

[U83] JS：ES Module 导入导出
来源：http://sgi.fengsongda.top

export const a = 1;  import { a } from "./m.js";
来源：http://ucn.ctjpmb.com

[U84] JS：CommonJS 写法
来源：http://zde.sufxvd.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zwa.cqqwz.cn


<!-- 参考信息 -->