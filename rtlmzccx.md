代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wge.jinghuilouyu.cn

================================================================================
来源：http://jli.jyoumei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gos.xziqi.cn

================================================================================
来源：http://zdf.chenzaomai.com

[T01] Kotlin：Hello World
来源：http://dfv.jinqigufen.top

println("Hello")
来源：http://jnw.pengpengdd.cyou

[T02] Kotlin：变量
来源：http://mlz.cucudq.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mqo.jqgfzy.top

[T03] Kotlin：字符串模板
来源：http://oee.jinyuanbaomall.cn

"值: $b"
来源：http://fzm.yueranfly.top

[T04] Kotlin：空安全
来源：http://eat.yvedp.cn

val n: String? = null;  n?.length
来源：http://avl.jinqigfzy.top

[T05] Kotlin：when 表达式
来源：http://mqi.svipenyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nhz.shanyushiyangkeji.top

[T06] Kotlin：集合映射
来源：http://kdq.cashguo.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ekc.zhongyouzk.top

[T07] Kotlin：集合过滤
来源：http://pif.9152youxi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ztf.hnxiangtu.top

[T08] Kotlin：数据类
来源：http://wpo.fktsv.cn

data class User(val name: String, val age: Int)
来源：http://unm.svipenyu.cn

[T09] Kotlin：扩展函数
来源：http://hbf.sxryk.cn

fun String.exclaim() = this + "!"
来源：http://wum.yuanzhike.top

[T10] Kotlin：默认参数
来源：http://byd.zhoulong.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://eqa.zycfv.cn

[T11] Kotlin：协程
来源：http://cwc.xuetiantiany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qoi.pycfn.com

[T12] Kotlin：解构声明
来源：http://mxc.tian-w.cn

val (a, b) = Pair(1, 2)
来源：http://wsf.hfpthk.cn

[T13] Kotlin：只读 Map
来源：http://qev.hywenlv.cn

val m = mapOf("a" to 1)
来源：http://oxm.ybcxt.top

[T14] Kotlin：循环
来源：http://ahn.fehbvm.com

for (i in 1..10) println(i)
来源：http://ilm.wangshuangyany.cn

[T15] Kotlin：接口
来源：http://uee.9152youxi.cn

interface Shape { fun area(): Double }
来源：http://otl.fktsv.cn

[T16] Swift：Hello World
来源：http://pep.zycfv.cn

print("Hello")
来源：http://fbf.dashuyun.cn

[T17] Swift：变量与常量
来源：http://jnt.dianchejie.cn

var a = 1;  let b = 2
来源：http://dsp.gzhubu.top

[T18] Swift：字符串插值
来源：http://egg.zhongyouzk.top

"值: \(b)"
来源：http://gcy.feifeiyinyue.top

[T19] Swift：可选绑定
来源：http://nvg.shzxlz.cn

if let n = opt { print(n) }
来源：http://lwa.jinyuanbaomall.cn

[T20] Swift：数组操作
来源：http://qgf.yj20258.top

var a = [1, 2, 3];  a.append(4)
来源：http://bik.nanxinkj.top

[T21] Swift：遍历
来源：http://oum.daria6918.cn

for x in a { print(x) }
来源：http://zzr.fanxiaobao.xyz

[T22] Swift：字典
来源：http://mgo.meibo888.top

var d = ["a": 1];  d["b"] = 2
来源：http://pzj.sysykeji.top

[T23] Swift：函数
来源：http://dba.yangfankeji.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uyd.zycfv.cn

[T24] Swift：闭包
来源：http://vsn.jinyuanbaomall.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://upa.fanxiaobao.xyz

[T25] Swift：结构体
来源：http://zre.mhx1999.top

struct P { var x: Int }
来源：http://fcg.zhoulong.xyz

[T26] Swift：类与重写
来源：http://hdn.gogol.net.cn

class A: Base { override func f() {} }
来源：http://xre.jinghuilouyu.cn

[T27] Swift：错误处理
来源：http://lpl.zhaomingkeji.xyz

do { try f() } catch { print(error) }
来源：http://nlr.birdmap.top

[T28] Swift：枚举
来源：http://sza.hesvh.cn

enum Color { case red, green }
来源：http://gyh.aizwys.cn

[T29] Swift：guard 提前返回
来源：http://kmz.fehbvm.com

guard let x = opt else { return }
来源：http://isf.yueranfly.top

[T30] Swift：协议
来源：http://lmr.yuanzhike.top

protocol Shape { func area() -> Double }
来源：http://rbp.fzhhl.top

[T31] Lua：Hello World
来源：http://sjg.dianchejie.cn

print("Hello")
来源：http://spn.pengpengdd.cyou

[T32] Lua：局部变量
来源：http://nal.sjlbkw.cn

local a = 1
来源：http://vgp.fanxiaobao.xyz

[T33] Lua：表（数组）
来源：http://zxc.ybcxt.top

local t = {1, 2, 3};  t[4] = 4
来源：http://oje.zhijiandao.cn

[T34] Lua：遍历表
来源：http://reo.yj20258.top

for i, v in ipairs(t) do print(i, v) end
来源：http://pyc.zhijiandao.cn

[T35] Lua：字典表
来源：http://bmy.mhx1999.top

local d = { a = 1 };  d.b = 2
来源：http://row.zhijiandao.cn

[T36] Lua：函数
来源：http://xyr.sweek.top

function add(a, b) return a + b end
来源：http://lpw.zhixingplan.top

[T37] Lua：字符串拼接
来源：http://prf.chenjidiqi.icu

"a" .. "b"
来源：http://zyw.dianchejie.cn

[T38] Lua：条件
来源：http://klv.iojbl.cn

if x > 0 then print("正") end
来源：http://kmj.ctjpmb.com

[T39] Lua：模式匹配
来源：http://ebn.zycfv.cn

string.find(s, "%d+")
来源：http://qtx.wangshuangyany.cn

[T40] Lua：元表
来源：http://sjx.hfpthk.cn

setmetatable({}, { __index = base })
来源：http://ast.ctjpmb.com

[T41] Perl：Hello World
来源：http://ndy.yonumen.top

print "Hello\n";
来源：http://sls.fengsongda.top

[T42] Perl：变量类型
来源：http://mnd.andypj.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jyc.xuetiantiany.cn

[T43] Perl：字符串插值
来源：http://krl.snrcjt.cn

"值: $a"
来源：http://dcx.aibaodan.cn

[T44] Perl：条件
来源：http://qvr.hfpthk.cn

if ($a > 0) { print "正"; }
来源：http://jpj.zdqjudy.top

[T45] Perl：数组遍历
来源：http://lbk.sjlbkw.cn

for my $x (@arr) { print $x; }
来源：http://sej.nanxuanxn.top

[T46] Perl：哈希操作
来源：http://uzw.chenlongwang.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ihi.fktsv.cn

[T47] Perl：正则捕获
来源：http://cab.vehdjk.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://sbr.haohaochexian.top

[T48] Perl：正则替换
来源：http://aga.chenlongwang.top

$s =~ s/old/new/g;
来源：http://qbm.meibo888.top

[T49] Perl：函数
来源：http://zjk.vehdjk.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qob.jiagoushi.top

[T50] Perl：逐行读文件
来源：http://don.tian-w.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nyc.fzhhl.top

while (my $line = <$fh>) { print $line; }
来源：http://ljq.yj20258888.top

[T51] Scala：Hello World
来源：http://ely.guowangkeji.top

println("Hello")
来源：http://hxy.hfpthk.cn

[T52] Scala：变量
来源：http://jtp.shanyushiyangkeji.top

val a = 1;  var b = 2
来源：http://bid.cucudq.cn

[T53] Scala：字符串插值
来源：http://tfp.nwbrower.top

s"值: $b"
来源：http://vqu.jqgufenzy.top

[T54] Scala：集合映射
来源：http://brd.wangshuangyany.cn

List(1, 2, 3).map(_ * 2)
来源：http://ycq.nanxinkj.top

[T55] Scala：集合过滤
来源：http://voq.xziqi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rez.gogol.net.cn

[T56] Scala：样例类
来源：http://wfj.hywenlv.cn

case class User(name: String, age: Int)
来源：http://bbo.shuidangran.top

[T57] Scala：模式匹配
来源：http://vpg.hesvh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jyw.yonumen.top

[T58] Scala：函数定义
来源：http://fkt.yj20258.top

def add(a: Int, b: Int): Int = a + b
来源：http://hvx.shuidangran.top

[T59] Scala：循环
来源：http://mlj.cashguo.top

for (i <- 1 to 10) println(i)
来源：http://wof.aizwys.cn

[T60] Scala：折叠
来源：http://voh.gaohongyu789.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bmu.uphjek.com

================================================================================
来源：http://oto.zdqjudy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tei.shanyushiyangkeji.top

================================================================================
来源：http://wne.yj202588.top

[U01] Py：创建虚拟环境
来源：http://eqw.ehwqpu.com

python -m venv .venv && source .venv/bin/activate
来源：http://dxk.9152youxi.cn

[U02] Py：导出 / 安装依赖
来源：http://uhs.zdbjq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rwh.zhengqikj.top

[U03] Py：加载 .env 配置
来源：http://dbh.meibo888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://clb.yuanzhike.top

[U04] Py：变量调试打印
来源：http://oje.jyoumei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cro.jiagoushi.top

[U05] Py：列表去重且保序
来源：http://ifs.fktsv.cn

list(dict.fromkeys(arr))
来源：http://pzd.gogol.net.cn

[U06] Py：合并两个字典
来源：http://fih.yuanzhike.top

{**a, **b}
来源：http://qha.ybcxt.top

[U07] Py：反转字典键值
来源：http://nrf.shzxlz.cn

{v: k for k, v in d.items()}
来源：http://rly.cashguo.top

[U08] Py：展平二维列表
来源：http://dmw.daxiang520.top

[y for x in nested for y in x]
来源：http://wau.haohaochexian.top

[U09] Py：字典取最大值的键
来源：http://nzi.sufxvd.cn

max(d, key=d.get)
来源：http://vsv.xziqi.cn

[U10] Py：按值排序字典
来源：http://vto.zhaomingkeji.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xbv.zhaomingkeji.xyz

[U11] Py：生成器表达式
来源：http://gas.ppjwa.cn

(x * 2 for x in arr)
来源：http://aen.svipenyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hmt.quarkkingdee.top

Counter(arr).most_common(3)
来源：http://lag.cdnleiting.top

[U13] Py：固定长度队列
来源：http://uey.tian-w.cn

deque(maxlen=10)
来源：http://tju.vehdjk.com

[U14] Py：分组收集到列表
来源：http://udk.cqqwz.cn

defaultdict(list)
来源：http://jtz.yonumen.top

[U15] Py：高精度计时
来源：http://hyx.yuxming.cn

t = time.perf_counter()
来源：http://tql.wangshuangyany.cn

[U16] Py：命令行参数解析
来源：http://jgp.hnqzz.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pht.xziqi.cn

[U17] Py：初始化日志
来源：http://hlg.snrcjt.cn

logging.basicConfig(level=logging.INFO)
来源：http://ttl.vehdjk.com

[U18] Py：预编译正则
来源：http://hau.aibaodan.cn

pat = re.compile(r"\d+")
来源：http://gag.cdnleiting.top

[U19] Py：正则替换带回调
来源：http://lfw.svipenyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ipa.shangyingyoupin.top

[U20] Py：缓存函数结果
来源：http://xsm.tanke756.top

@functools.lru_cache(maxsize=None)
来源：http://xfq.jinqigfzy.top

[U21] Py：自定义上下文管理器
来源：http://efc.cdnleiting.top

@contextlib.contextmanager
来源：http://bwd.kuanghao11.cn

[U22] Py：矩阵转置
来源：http://zwp.jinyuanbaomall.cn

list(zip(*m))
来源：http://ixt.nwbrower.top

[U23] Py：分块读取大文件
来源：http://gig.pengpengdd.cyou

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lml.birdmap.top

[U24] Py：路径操作
来源：http://yuw.havefunace.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ljk.jinqigufen.top

[U25] Py：CSV 按字典读
来源：http://zbm.sufxvd.cn

csv.DictReader(f)
来源：http://ppf.xylfe.cn

[U26] Py：并发下载
来源：http://xdl.wangshuangyany.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://piy.jqgfzy.top

[U27] Py：异步 HTTP
来源：http://pdd.ppjwa.cn

aiohttp.ClientSession() 配合 async with
来源：http://roz.nanxuanxn.top

[U28] Py：类型别名
来源：http://pfr.zhiwuduotai.top

UserId = int
来源：http://osk.zycfv.cn

[U29] Py：属性校验
来源：http://uxp.haohaochexian.top

@property 与 @x.setter 配合
来源：http://wvz.yvedp.cn

[U30] Py：数据类
来源：http://zdm.vehdjk.com

@dataclass(slots=True)
来源：http://tba.ctjpmb.com

[U31] Py：单测
来源：http://sog.jinyuanbaomall.cn

python -m pytest -q
来源：http://qjs.birdmap.top

[U32] Py：代码格式化
来源：http://ecz.shangyingyoupin.top

ruff format . && ruff check --fix .
来源：http://iia.jianghu66.top

[U33] Py：打包发布
来源：http://jve.kuanghao11.cn

python -m build  （依赖 pyproject.toml）
来源：http://pkb.ywan-chungtsiang.top

[U34] Py：判断编码
来源：http://iuh.hnqzz.top

chardet.detect(raw)
来源：http://tyw.zhaomingkeji.xyz

[U35] Py：发送邮件
来源：http://xan.pycfn.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://obf.guowangkeji.top

[U36] Py：定时任务
来源：http://wmg.hnqzz.top

schedule.every(10).minutes.do(job)
来源：http://grz.tarul.cn

[U37] Py：读写 Excel
来源：http://bvp.sweek.top

pandas.read_excel / DataFrame.to_excel
来源：http://ken.nanxinkj.top

[U38] Py：获取脚本所在目录
来源：http://ttx.uphjek.com

Path(__file__).resolve().parent
来源：http://aat.haohaochexian.top

[U39] Py：判断是否在交互环境
来源：http://wyd.tarul.cn

sys.stdout.isatty()
来源：http://aqi.yj20258.top

[U40] Py：打印到标准错误
来源：http://qnk.yj20258.top

print("err", file=sys.stderr)
来源：http://xtj.yanxiufei.cn

[U41] PHP：初始化 Composer 项目
来源：http://lzz.smart0.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://yzy.mhx1999.top

[U42] PHP：PSR-4 自动加载
来源：http://bdn.zhijiandao.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lto.xylfe.cn

[U43] PHP：声明命名空间
来源：http://mbk.yj202588.top

namespace App\Http;
来源：http://ysf.shangyingyoupin.top

[U44] PHP：开启严格类型
来源：http://luz.shanyushiyangtech.top

declare(strict_types=1);
来源：http://ick.snrcjt.cn

[U45] PHP：类型声明与返回类型
来源：http://xwv.hnqzz.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://dii.shanyushiyangkeji.top

[U46] PHP：可空类型
来源：http://zma.cqqwz.cn

?string $name = null
来源：http://hgp.mhx1999.top

[U47] PHP：联合类型
来源：http://dxt.havefunace.top

int|string $id
来源：http://uuz.tarul.cn

[U48] PHP：纯枚举
来源：http://ili.shanyushiyangtech.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nbg.hysaishi.cn

[U49] PHP：只读属性
来源：http://yfc.fengsongda.top

public readonly string $name
来源：http://coz.jinqigfzy.top

[U50] PHP：构造器属性提升
来源：http://xco.sweek.top

public function __construct(private int $id) {}
来源：http://rle.ydzc1.top

[U51] PHP：数组解构
来源：http://nmy.gaohongyu789.top

[$a, $b] = $arr;
来源：http://jqe.zhengqikj.top

[U52] PHP：箭头函数
来源：http://dhb.sxryk.cn

$double = fn($x) => $x * 2;
来源：http://vwk.ehwqpu.com

[U53] PHP：空合并运算符
来源：http://yxu.hywenlv.cn

$v = $a ?? $b ?? "default";
来源：http://aqr.zycfv.cn

[U54] PHP：空安全调用
来源：http://uja.yueranfly.top

$obj?->method()
来源：http://qfr.bbcook.cn

[U55] PHP：match 表达式
来源：http://zwy.redwolf501.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kgq.cheryme.top

[U56] PHP：命名参数
来源：http://bqq.chenlongwang.top

f(a: 1, b: 2)
来源：http://znd.tianlin.xyz

[U57] PHP：字符串插值
来源：http://gxs.daxiang520.top

"值: {$a}"
来源：http://xfz.snrcjt.cn

[U58] PHP：数组三件套
来源：http://apo.hcnkem.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wdn.zhoulong.xyz

[U59] PHP：自定义排序
来源：http://zdl.zdbjq.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lrk.zdbjq.cn

[U60] PHP：JSON 编解码
来源：http://iet.fzhhl.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dss.xuetiantiany.cn

[U61] PHP：正则
来源：http://rvl.iojbl.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vld.redwolf501.top

[U62] PHP：日期对象
来源：http://zsd.jqgufenzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fjw.jinqigufen.top

[U63] PHP：文件读写
来源：http://oxm.mhx1999.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://aak.sysykeji.top

[U64] PHP：目录遍历
来源：http://iix.vqdsnc.cn

glob("dir/*.php");  scandir("dir");
来源：http://ytb.ivvv.top

[U65] PHP：会话
来源：http://wgy.xuetiantiany.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rhj.chenzaomai.com

[U66] PHP：设置 Cookie
来源：http://fzg.xylfe.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://khi.zhiwuduotai.top

[U67] PHP：处理文件上传
来源：http://bjq.c1oappe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mba.meibo888.top

[U68] PHP：PDO 连接
来源：http://gsb.xziqi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sto.ehwqpu.com

[U69] PHP：PDO 预处理
来源：http://xxe.aibaodan.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wyq.nwbrower.top

[U70] PHP：PDO 事务
来源：http://khz.yj20258888.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ayq.shuidangran.top

[U71] PHP：抛出异常
来源：http://awx.nanxuanxn.top

throw new RuntimeException("失败", 500);
来源：http://wsg.ehwqpu.com

[U72] PHP：写错误日志
来源：http://jjl.jinqigfzy.top

error_log("失败: " . $e->getMessage());
来源：http://rmd.hfpthk.cn

[U73] PHP：读取 ini 配置
来源：http://vmv.hnqzz.top

parse_ini_file("config.ini", true)
来源：http://xbd.pycfn.com

[U74] PHP：读取环境变量
来源：http://quu.iojbl.cn

getenv("APP_ENV") ?: "production"
来源：http://yid.fehbvm.com

[U75] PHP：依赖注入
来源：http://ksw.ivvv.top

composer require psr/container
来源：http://xzf.zhaomingkeji.xyz

[U76] PHP：简单路由
来源：http://qdh.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ngn.yuxming.cn

[U77] PHP：模板渲染
来源：http://duo.bbcook.cn

composer require twig/twig
来源：http://bxv.gaohongyu789.top

[U78] PHP：单元测试
来源：http://yxd.yongpay.top

composer require --dev phpunit/phpunit
来源：http://hcm.zhixingplan.top

[U79] PHP：静态分析
来源：http://cdp.haohaochexian.top

composer require --dev phpstan/phpstan
来源：http://gbd.cqqwz.cn

[U80] PHP：代码规范修复
来源：http://xhj.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hxe.quarkkingdee.top

[U81] JS：初始化项目
来源：http://tif.sysykeji.top

npm init -y;  npm i express
来源：http://zjf.sweek.top

[U82] JS：package.json 脚本
来源：http://ihr.snrcjt.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cye.xuetiantiany.cn

[U83] JS：ES Module 导入导出
来源：http://nqr.shanyushiyangtech.top

export const a = 1;  import { a } from "./m.js";
来源：http://evr.shzxlz.cn

[U84] JS：CommonJS 写法
来源：http://yyw.c1oappe.top

module.exports = { a };  const { a } = require("./m");
来源：http://djk.yanxiufei.cn

[U85] JS：可选链
来源：http://niq.gogol.net.cn

a?.b?.c
来源：http://mei.yangfankeji.com

[U86] JS：空值合并
来源：http://gep.chenzaomai.com

a ?? b
来源：http://hyc.zhongyouzk.top


<!-- 参考信息 -->