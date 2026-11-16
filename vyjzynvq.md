代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rkd.uphjek.com

================================================================================
来源：http://xte.sxryk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ywf.gzhubu.top

================================================================================
来源：http://lkg.ywan-chungtsiang.top

[T01] Kotlin：Hello World
来源：http://mwu.ctjpmb.com

println("Hello")
来源：http://pod.pycfn.com

[T02] Kotlin：变量
来源：http://glr.yonumen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bdr.yuxming.cn

[T03] Kotlin：字符串模板
来源：http://xoc.aibaodan.cn

"值: $b"
来源：http://rlt.pengpengdd.cyou

[T04] Kotlin：空安全
来源：http://ohb.daria6918.cn

val n: String? = null;  n?.length
来源：http://qti.ehwqpu.com

[T05] Kotlin：when 表达式
来源：http://xjn.feifeiyinyue.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xsa.guannengcc.top

[T06] Kotlin：集合映射
来源：http://air.mhx1999.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ccy.chenlongwang.top

[T07] Kotlin：集合过滤
来源：http://usr.cheryme.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://luy.yfazqb.com

[T08] Kotlin：数据类
来源：http://oao.xylfe.cn

data class User(val name: String, val age: Int)
来源：http://azh.birdmap.top

[T09] Kotlin：扩展函数
来源：http://uge.meibo888.top

fun String.exclaim() = this + "!"
来源：http://wnr.bbcook.cn

[T10] Kotlin：默认参数
来源：http://cvi.shanyushiyangtech.top

fun greet(name: String = "World") = "Hi $name"
来源：http://agb.dianchejie.cn

[T11] Kotlin：协程
来源：http://gvd.gzhubu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hlr.fengsongda.top

[T12] Kotlin：解构声明
来源：http://geh.c1oappe.top

val (a, b) = Pair(1, 2)
来源：http://dhi.dashuyun.cn

[T13] Kotlin：只读 Map
来源：http://wap.9152youxi.cn

val m = mapOf("a" to 1)
来源：http://wyx.sjlbkw.cn

[T14] Kotlin：循环
来源：http://ibj.hysaishi.cn

for (i in 1..10) println(i)
来源：http://qkf.pycfn.com

[T15] Kotlin：接口
来源：http://jpy.pycfn.com

interface Shape { fun area(): Double }
来源：http://hvf.xylfe.cn

[T16] Swift：Hello World
来源：http://qck.shanyushiyangtech.top

print("Hello")
来源：http://lgu.hammf.cn

[T17] Swift：变量与常量
来源：http://mhm.sysykeji.top

var a = 1;  let b = 2
来源：http://vcy.hcnkem.com

[T18] Swift：字符串插值
来源：http://ufb.yongpay.top

"值: \(b)"
来源：http://wdy.vqdsnc.cn

[T19] Swift：可选绑定
来源：http://ckm.aizwys.cn

if let n = opt { print(n) }
来源：http://rtl.gogol.net.cn

[T20] Swift：数组操作
来源：http://zdd.zhongyouzk.top

var a = [1, 2, 3];  a.append(4)
来源：http://wjp.sysykeji.top

[T21] Swift：遍历
来源：http://kzv.ehwqpu.com

for x in a { print(x) }
来源：http://anr.c1oappe.top

[T22] Swift：字典
来源：http://vty.hnxiangtu.top

var d = ["a": 1];  d["b"] = 2
来源：http://kah.ybcxt.top

[T23] Swift：函数
来源：http://gsq.ivvv.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uno.bjfxy.top

[T24] Swift：闭包
来源：http://lzx.zycfv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wog.epnwcf.com

[T25] Swift：结构体
来源：http://gda.shangyingyoupin.top

struct P { var x: Int }
来源：http://rmp.daria6918.cn

[T26] Swift：类与重写
来源：http://his.jyoumei.cn

class A: Base { override func f() {} }
来源：http://uig.xylfe.cn

[T27] Swift：错误处理
来源：http://ggy.zhongyouzk.top

do { try f() } catch { print(error) }
来源：http://scn.fzhhl.top

[T28] Swift：枚举
来源：http://utr.zhixingplan.top

enum Color { case red, green }
来源：http://ynq.sysykeji.top

[T29] Swift：guard 提前返回
来源：http://pia.pengpengdd.cyou

guard let x = opt else { return }
来源：http://qzt.zhijiandao.cn

[T30] Swift：协议
来源：http://eni.yj202588.top

protocol Shape { func area() -> Double }
来源：http://vya.zdqjudy.top

[T31] Lua：Hello World
来源：http://fnp.feifeiyinyue.top

print("Hello")
来源：http://qem.haohaochexian.top

[T32] Lua：局部变量
来源：http://gtc.epnwcf.com

local a = 1
来源：http://dxk.jyoumei.cn

[T33] Lua：表（数组）
来源：http://wwh.yuanzhike.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hlf.fktsv.cn

[T34] Lua：遍历表
来源：http://xzs.aizwys.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ytt.jinghuilouyu.cn

[T35] Lua：字典表
来源：http://rnz.xylfe.cn

local d = { a = 1 };  d.b = 2
来源：http://xqo.ydzc1.top

[T36] Lua：函数
来源：http://wce.hcnkem.com

function add(a, b) return a + b end
来源：http://bwq.cucudq.cn

[T37] Lua：字符串拼接
来源：http://kgd.xinyue.icu

"a" .. "b"
来源：http://khm.fengsongda.top

[T38] Lua：条件
来源：http://tzu.andypj.xyz

if x > 0 then print("正") end
来源：http://epg.yj20258.top

[T39] Lua：模式匹配
来源：http://ltq.havefunace.top

string.find(s, "%d+")
来源：http://vln.zhengqikj.top

[T40] Lua：元表
来源：http://inb.yuxming.cn

setmetatable({}, { __index = base })
来源：http://ukn.xuanzx.com

[T41] Perl：Hello World
来源：http://mwr.yfazqb.com

print "Hello\n";
来源：http://ykg.dashuyun.cn

[T42] Perl：变量类型
来源：http://ndo.guannengcc.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ort.zhiwuduotai.top

[T43] Perl：字符串插值
来源：http://juw.chenlongwang.top

"值: $a"
来源：http://gvt.hywenlv.cn

[T44] Perl：条件
来源：http://toi.gaohongyu789.top

if ($a > 0) { print "正"; }
来源：http://lpw.9152youxi.cn

[T45] Perl：数组遍历
来源：http://ync.quarkkingdee.top

for my $x (@arr) { print $x; }
来源：http://nok.hysaishi.cn

[T46] Perl：哈希操作
来源：http://sek.tarul.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kxj.shuidangran.top

[T47] Perl：正则捕获
来源：http://mbo.kuanghao11.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://arj.c1oappe.top

[T48] Perl：正则替换
来源：http://lvl.yj20258888.top

$s =~ s/old/new/g;
来源：http://qcp.hesvh.cn

[T49] Perl：函数
来源：http://vza.hammf.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vur.chenlongwang.top

[T50] Perl：逐行读文件
来源：http://bhy.bbcook.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kzu.sxryk.cn

while (my $line = <$fh>) { print $line; }
来源：http://hwq.yueranfly.top

[T51] Scala：Hello World
来源：http://vma.epnwcf.com

println("Hello")
来源：http://ihx.yangfankeji.com

[T52] Scala：变量
来源：http://xuq.aizwys.cn

val a = 1;  var b = 2
来源：http://djs.vehdjk.com

[T53] Scala：字符串插值
来源：http://ccv.hywenlv.cn

s"值: $b"
来源：http://nmr.fktsv.cn

[T54] Scala：集合映射
来源：http://nqn.shzxlz.cn

List(1, 2, 3).map(_ * 2)
来源：http://slf.svipenyu.cn

[T55] Scala：集合过滤
来源：http://zdx.sweek.top

List(1, 2, 3).filter(_ > 1)
来源：http://ofl.tian-w.cn

[T56] Scala：样例类
来源：http://dys.bjfxy.top

case class User(name: String, age: Int)
来源：http://hhp.andypj.xyz

[T57] Scala：模式匹配
来源：http://fbe.kuanghao11.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://khb.yueranfly.top

[T58] Scala：函数定义
来源：http://aha.redwolf501.top

def add(a: Int, b: Int): Int = a + b
来源：http://ome.jinyuanbaomall.cn

[T59] Scala：循环
来源：http://sxd.hfpthk.cn

for (i <- 1 to 10) println(i)
来源：http://rho.c1oappe.top

[T60] Scala：折叠
来源：http://pxc.nanxuanxn.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tsr.daria6918.cn

================================================================================
来源：http://crh.c1oappe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cnf.xziqi.cn

================================================================================
来源：http://gzz.guannengcc.top

[U01] Py：创建虚拟环境
来源：http://idv.jqgufenzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://byz.daria6918.cn

[U02] Py：导出 / 安装依赖
来源：http://cie.guannengcc.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dxk.cqqwz.cn

[U03] Py：加载 .env 配置
来源：http://xrt.sysykeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://kex.nanxuanxn.top

[U04] Py：变量调试打印
来源：http://ssq.snrcjt.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jye.vqdsnc.cn

[U05] Py：列表去重且保序
来源：http://ujs.daria6918.cn

list(dict.fromkeys(arr))
来源：http://tgh.ppjwa.cn

[U06] Py：合并两个字典
来源：http://hbi.kuanghao11.cn

{**a, **b}
来源：http://pil.nwbrower.top

[U07] Py：反转字典键值
来源：http://chf.316326.xyz

{v: k for k, v in d.items()}
来源：http://pnx.chenlongwang.top

[U08] Py：展平二维列表
来源：http://vql.yuanzhike.top

[y for x in nested for y in x]
来源：http://hyf.tianlin.xyz

[U09] Py：字典取最大值的键
来源：http://mss.svipenyu.cn

max(d, key=d.get)
来源：http://jii.kuanghao11.cn

[U10] Py：按值排序字典
来源：http://jfe.jinyuanbaomall.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yvh.gzhubu.top

[U11] Py：生成器表达式
来源：http://dzl.zhaomingkeji.xyz

(x * 2 for x in arr)
来源：http://lnz.yj202588.top

[U12] Py：取出现最多的 3 个元素
来源：http://uff.gaohongyu789.top

Counter(arr).most_common(3)
来源：http://ztn.hongshengwenyu.top

[U13] Py：固定长度队列
来源：http://egd.cashguo.top

deque(maxlen=10)
来源：http://sjd.bbcook.cn

[U14] Py：分组收集到列表
来源：http://zqp.tanke756.top

defaultdict(list)
来源：http://ovv.sweek.top

[U15] Py：高精度计时
来源：http://rgk.ydzc1.top

t = time.perf_counter()
来源：http://goq.sweek.top

[U16] Py：命令行参数解析
来源：http://gya.hongshengwenyu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tym.chenzaomai.com

[U17] Py：初始化日志
来源：http://gen.ydzc1.top

logging.basicConfig(level=logging.INFO)
来源：http://ype.jianghu66.top

[U18] Py：预编译正则
来源：http://nnm.guannengcc.top

pat = re.compile(r"\d+")
来源：http://lad.vehdjk.com

[U19] Py：正则替换带回调
来源：http://vfg.daria6918.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uyc.yanxiufei.cn

[U20] Py：缓存函数结果
来源：http://vdy.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://vpl.hysaishi.cn

[U21] Py：自定义上下文管理器
来源：http://sbo.tian-w.cn

@contextlib.contextmanager
来源：http://rod.hywenlv.cn

[U22] Py：矩阵转置
来源：http://ntc.ivvv.top

list(zip(*m))
来源：http://uta.jianghu66.top

[U23] Py：分块读取大文件
来源：http://mgl.fktsv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yyo.chenlongwang.top

[U24] Py：路径操作
来源：http://mtn.xuanzx.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ryx.yangfankeji.com

[U25] Py：CSV 按字典读
来源：http://mpl.nwbrower.top

csv.DictReader(f)
来源：http://vjp.nanxinkj.top

[U26] Py：并发下载
来源：http://opy.yvedp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yei.fktsv.cn

[U27] Py：异步 HTTP
来源：http://ksp.jqgfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://cbj.jinghuilouyu.cn

[U28] Py：类型别名
来源：http://oua.sxryk.cn

UserId = int
来源：http://hbe.dianchejie.cn

[U29] Py：属性校验
来源：http://mur.mhx1999.top

@property 与 @x.setter 配合
来源：http://mbt.bjfxy.top

[U30] Py：数据类
来源：http://nfk.ehwqpu.com

@dataclass(slots=True)
来源：http://bxb.redwolf501.top

[U31] Py：单测
来源：http://xmx.0kj1m.cn

python -m pytest -q
来源：http://ghj.52xcode.cn

[U32] Py：代码格式化
来源：http://cat.xziqi.cn

ruff format . && ruff check --fix .
来源：http://vzr.meibo888.top

[U33] Py：打包发布
来源：http://ibt.snrcjt.cn

python -m build  （依赖 pyproject.toml）
来源：http://jky.chenzaomai.com

[U34] Py：判断编码
来源：http://lel.ehwqpu.com

chardet.detect(raw)
来源：http://jsr.316326.xyz

[U35] Py：发送邮件
来源：http://log.xylfe.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yho.jinqigufen.top

[U36] Py：定时任务
来源：http://rqc.feifeiyinyue.top

schedule.every(10).minutes.do(job)
来源：http://ker.vqdsnc.cn

[U37] Py：读写 Excel
来源：http://sms.nanxuanxn.top

pandas.read_excel / DataFrame.to_excel
来源：http://ulz.0kj1m.cn

[U38] Py：获取脚本所在目录
来源：http://hez.shanyushiyangkeji.top

Path(__file__).resolve().parent
来源：http://xcb.cashguo.top

[U39] Py：判断是否在交互环境
来源：http://dvs.shanyushiyangkeji.top

sys.stdout.isatty()
来源：http://rac.jyoumei.cn

[U40] Py：打印到标准错误
来源：http://bsz.chenzaomai.com

print("err", file=sys.stderr)
来源：http://kmf.redwolf501.top

[U41] PHP：初始化 Composer 项目
来源：http://fcz.fanxiaobao.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://gid.hywenlv.cn

[U42] PHP：PSR-4 自动加载
来源：http://xci.316326.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ozw.gogol.net.cn

[U43] PHP：声明命名空间
来源：http://xif.hcnkem.com

namespace App\Http;
来源：http://emx.jiagoushi.top

[U44] PHP：开启严格类型
来源：http://ehh.havefunace.top

declare(strict_types=1);
来源：http://leb.wangdashe.top

[U45] PHP：类型声明与返回类型
来源：http://drs.jqgufenzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://agm.jianghu66.top

[U46] PHP：可空类型
来源：http://pxj.meibo888.top

?string $name = null
来源：http://lqh.ivvv.top

[U47] PHP：联合类型
来源：http://ezv.zhaomingkeji.xyz

int|string $id
来源：http://byp.cqqwz.cn

[U48] PHP：纯枚举
来源：http://lqi.ctjpmb.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://imd.cdnleiting.top

[U49] PHP：只读属性
来源：http://rri.fanxiaobao.xyz

public readonly string $name
来源：http://pbw.nanxuanxn.top

[U50] PHP：构造器属性提升
来源：http://ivy.zhijiandao.cn

public function __construct(private int $id) {}
来源：http://ttm.havefunace.top

[U51] PHP：数组解构
来源：http://dlv.hammf.cn

[$a, $b] = $arr;
来源：http://nnk.nanxuanxn.top

[U52] PHP：箭头函数
来源：http://cdw.dashuyun.cn

$double = fn($x) => $x * 2;
来源：http://oqj.pengpengdd.cyou

[U53] PHP：空合并运算符
来源：http://rwy.hcnkem.com

$v = $a ?? $b ?? "default";
来源：http://nki.chenzaomai.com

[U54] PHP：空安全调用
来源：http://udx.vehdjk.com

$obj?->method()
来源：http://uud.cqqwz.cn

[U55] PHP：match 表达式
来源：http://clb.chenzaomai.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ans.ywan-chungtsiang.top

[U56] PHP：命名参数
来源：http://twd.xziqi.cn

f(a: 1, b: 2)
来源：http://shw.pycfn.com

[U57] PHP：字符串插值
来源：http://lne.vqdsnc.cn

"值: {$a}"
来源：http://lmb.yangfankeji.com

[U58] PHP：数组三件套
来源：http://lap.wangdashe.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xnd.shanyushiyangtech.top

[U59] PHP：自定义排序
来源：http://xgf.fanxiaobao.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mcb.hysaishi.cn

[U60] PHP：JSON 编解码
来源：http://cou.xuetiantiany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lgl.yj20258.top

[U61] PHP：正则
来源：http://mjr.aibaodan.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bxh.gotoacloud.top

[U62] PHP：日期对象
来源：http://lrw.0kj1m.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tam.chenlongwang.top

[U63] PHP：文件读写
来源：http://kyy.yonumen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ufs.9152youxi.cn

[U64] PHP：目录遍历
来源：http://mid.yj20258.top

glob("dir/*.php");  scandir("dir");
来源：http://hia.yuxming.cn

[U65] PHP：会话
来源：http://cqg.daxiang520.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ffz.yj20258.top

[U66] PHP：设置 Cookie
来源：http://dqv.guowangkeji.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://twq.yfazqb.com

[U67] PHP：处理文件上传
来源：http://qcf.jyoumei.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://whe.c1oappe.top

[U68] PHP：PDO 连接
来源：http://nxd.ydjk.org.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://djs.vqdsnc.cn

[U69] PHP：PDO 预处理
来源：http://fbq.fktsv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bbm.fzhhl.top

[U70] PHP：PDO 事务
来源：http://sbw.jqgfzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://paj.hesvh.cn

[U71] PHP：抛出异常
来源：http://slf.jqgfzy.top

throw new RuntimeException("失败", 500);
来源：http://kky.aizwys.cn

[U72] PHP：写错误日志
来源：http://ujd.zdbjq.cn

error_log("失败: " . $e->getMessage());
来源：http://uwp.shuidangran.top

[U73] PHP：读取 ini 配置
来源：http://qth.jiagoushi.top

parse_ini_file("config.ini", true)
来源：http://gqs.cheryme.top

[U74] PHP：读取环境变量
来源：http://aao.tianlin.xyz

getenv("APP_ENV") ?: "production"
来源：http://lqb.ywan-chungtsiang.top

[U75] PHP：依赖注入
来源：http://pgr.cheryme.top

composer require psr/container
来源：http://qkr.hfpthk.cn

[U76] PHP：简单路由
来源：http://dkd.zhiwuduotai.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://llw.shuidangran.top

[U77] PHP：模板渲染
来源：http://avt.gzhubu.top

composer require twig/twig
来源：http://nbm.bbcook.cn

[U78] PHP：单元测试
来源：http://ftx.cheryme.top

composer require --dev phpunit/phpunit
来源：http://fol.sweek.top

[U79] PHP：静态分析
来源：http://dqj.fanxiaobao.xyz

composer require --dev phpstan/phpstan
来源：http://zum.shanyushiyangtech.top

[U80] PHP：代码规范修复
来源：http://amm.ybcxt.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jqm.havefunace.top

[U81] JS：初始化项目
来源：http://xdl.uphjek.com

npm init -y;  npm i express
来源：http://yga.hcnkem.com

[U82] JS：package.json 脚本
来源：http://gsy.hongshengwenyu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rdo.shuidangran.top

[U83] JS：ES Module 导入导出
来源：http://gry.shuidangran.top

export const a = 1;  import { a } from "./m.js";
来源：http://sse.fktsv.cn

[U84] JS：CommonJS 写法
来源：http://zgk.cheryme.top

module.exports = { a };  const { a } = require("./m");
来源：http://oos.guowangkeji.top

[U85] JS：可选链
来源：http://ttz.pengpengdd.cyou

a?.b?.c
来源：http://qmy.yvedp.cn

[U86] JS：空值合并
来源：http://wou.nanxinkj.top

a ?? b
来源：http://gao.tarul.cn


<!-- 参考信息 -->