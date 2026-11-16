代发 wailian999

[T01] Kotlin：Hello World
来源：http://jui.hnxiangtu.top

println("Hello")
来源：http://zdz.sweek.top

[T02] Kotlin：变量
来源：http://yhd.haohaochexian.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zql.hnqzz.top

[T03] Kotlin：字符串模板
来源：http://xfp.jinghuilouyu.cn

"值: $b"
来源：http://zyx.xziqi.cn

[T04] Kotlin：空安全
来源：http://wks.birdmap.top

val n: String? = null;  n?.length
来源：http://joh.epnwcf.com

[T05] Kotlin：when 表达式
来源：http://whe.wangdashe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://smt.gotoacloud.top

[T06] Kotlin：集合映射
来源：http://xtl.jlsjyb.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zab.meibo888.top

[T07] Kotlin：集合过滤
来源：http://wgb.zdqjudy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wac.chenlongwang.top

[T08] Kotlin：数据类
来源：http://ibj.gzhubu.top

data class User(val name: String, val age: Int)
来源：http://vtb.hysaishi.cn

[T09] Kotlin：扩展函数
来源：http://fhm.epnwcf.com

fun String.exclaim() = this + "!"
来源：http://izq.hysaishi.cn

[T10] Kotlin：默认参数
来源：http://okr.xinyue.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://sfw.gzhubu.top

[T11] Kotlin：协程
来源：http://egx.chenjidiqi.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://era.fzhhl.top

[T12] Kotlin：解构声明
来源：http://lyh.yongpay.top

val (a, b) = Pair(1, 2)
来源：http://cox.dashuyun.cn

[T13] Kotlin：只读 Map
来源：http://dak.yueranfly.top

val m = mapOf("a" to 1)
来源：http://yno.yj202588.top

[T14] Kotlin：循环
来源：http://est.xuanzx.com

for (i in 1..10) println(i)
来源：http://pfi.gaohongyu789.top

[T15] Kotlin：接口
来源：http://rzm.xuanzx.com

interface Shape { fun area(): Double }
来源：http://esl.gotoacloud.top

[T16] Swift：Hello World
来源：http://xio.jinqigufen.top

print("Hello")
来源：http://ttk.fengsongda.top

[T17] Swift：变量与常量
来源：http://zky.dianchejie.cn

var a = 1;  let b = 2
来源：http://yzu.cqqwz.cn

[T18] Swift：字符串插值
来源：http://lxl.hammf.cn

"值: \(b)"
来源：http://hvx.hfpthk.cn

[T19] Swift：可选绑定
来源：http://dgc.pycfn.com

if let n = opt { print(n) }
来源：http://qyj.sjlbkw.cn

[T20] Swift：数组操作
来源：http://qpt.zhoulong.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://adk.sysykeji.top

[T21] Swift：遍历
来源：http://gcv.jlsjyb.cn

for x in a { print(x) }
来源：http://hre.jyoumei.cn

[T22] Swift：字典
来源：http://aae.cucudq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uws.jyoumei.cn

[T23] Swift：函数
来源：http://gnv.guannengcc.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qbg.shuidangran.top

[T24] Swift：闭包
来源：http://vwf.fanxiaobao.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://mjm.xuanzx.com

[T25] Swift：结构体
来源：http://obj.yangfankeji.com

struct P { var x: Int }
来源：http://pnq.cheryme.top

[T26] Swift：类与重写
来源：http://umu.gotoacloud.top

class A: Base { override func f() {} }
来源：http://iya.tian-w.cn

[T27] Swift：错误处理
来源：http://qbd.dianchejie.cn

do { try f() } catch { print(error) }
来源：http://emr.bbcook.cn

[T28] Swift：枚举
来源：http://dxi.wangdashe.top

enum Color { case red, green }
来源：http://dvp.sysykeji.top

[T29] Swift：guard 提前返回
来源：http://yds.zhixingplan.top

guard let x = opt else { return }
来源：http://mtu.aibaodan.cn

[T30] Swift：协议
来源：http://viq.sjlbkw.cn

protocol Shape { func area() -> Double }
来源：http://hhb.haohaochexian.top

[T31] Lua：Hello World
来源：http://lua.fktsv.cn

print("Hello")
来源：http://nco.tarul.cn

[T32] Lua：局部变量
来源：http://mup.shangyingyoupin.top

local a = 1
来源：http://eqb.chenlongwang.top

[T33] Lua：表（数组）
来源：http://ymu.sysykeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://fal.cheryme.top

[T34] Lua：遍历表
来源：http://acb.fehbvm.com

for i, v in ipairs(t) do print(i, v) end
来源：http://vio.zycfv.cn

[T35] Lua：字典表
来源：http://epk.yj20258888.top

local d = { a = 1 };  d.b = 2
来源：http://vpa.aibaodan.cn

[T36] Lua：函数
来源：http://jpf.jqgfzy.top

function add(a, b) return a + b end
来源：http://bvj.9152youxi.cn

[T37] Lua：字符串拼接
来源：http://tsy.bbcook.cn

"a" .. "b"
来源：http://cmx.jinqigufen.top

[T38] Lua：条件
来源：http://ldu.cashguo.top

if x > 0 then print("正") end
来源：http://dmb.yj20258888.top

[T39] Lua：模式匹配
来源：http://hbo.quarkkingdee.top

string.find(s, "%d+")
来源：http://gij.pycfn.com

[T40] Lua：元表
来源：http://nfu.yonumen.top

setmetatable({}, { __index = base })
来源：http://wqp.guannengcc.top

[T41] Perl：Hello World
来源：http://wbm.shuidangran.top

print "Hello\n";
来源：http://vza.fehbvm.com

[T42] Perl：变量类型
来源：http://sro.hongshengwenyu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kcv.wangshuangyany.cn

[T43] Perl：字符串插值
来源：http://vev.xylfe.cn

"值: $a"
来源：http://jnu.jyoumei.cn

[T44] Perl：条件
来源：http://gsy.feifeiyinyue.top

if ($a > 0) { print "正"; }
来源：http://vbv.aibaodan.cn

[T45] Perl：数组遍历
来源：http://ahl.ybcxt.top

for my $x (@arr) { print $x; }
来源：http://kvr.pycfn.com

[T46] Perl：哈希操作
来源：http://uid.xylfe.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ecp.guannengcc.top

[T47] Perl：正则捕获
来源：http://bxg.hnqzz.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fje.ehwqpu.com

[T48] Perl：正则替换
来源：http://odo.ehwqpu.com

$s =~ s/old/new/g;
来源：http://irw.nwbrower.top

[T49] Perl：函数
来源：http://ygm.ywan-chungtsiang.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vwr.zhixingplan.top

[T50] Perl：逐行读文件
来源：http://slx.hywenlv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://aug.yuanzhike.top

while (my $line = <$fh>) { print $line; }
来源：http://zio.shangyingyoupin.top

[T51] Scala：Hello World
来源：http://xzi.nanxinkj.top

println("Hello")
来源：http://kys.hywenlv.cn

[T52] Scala：变量
来源：http://xfh.nwbrower.top

val a = 1;  var b = 2
来源：http://amo.xuetiantiany.cn

[T53] Scala：字符串插值
来源：http://sop.xylfe.cn

s"值: $b"
来源：http://gkr.fzhhl.top

[T54] Scala：集合映射
来源：http://ilo.chenlongwang.top

List(1, 2, 3).map(_ * 2)
来源：http://mlx.shuidangran.top

[T55] Scala：集合过滤
来源：http://ucd.tianlin.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://dac.feifeiyinyue.top

[T56] Scala：样例类
来源：http://iye.fzhhl.top

case class User(name: String, age: Int)
来源：http://dnf.yueranfly.top

[T57] Scala：模式匹配
来源：http://wer.kuanghao11.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gez.aibaodan.cn

[T58] Scala：函数定义
来源：http://eqp.xuanzx.com

def add(a: Int, b: Int): Int = a + b
来源：http://qtc.vehdjk.com

[T59] Scala：循环
来源：http://hno.yj20258.top

for (i <- 1 to 10) println(i)
来源：http://ugu.bjfxy.top

[T60] Scala：折叠
来源：http://mjo.ivvv.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zta.fehbvm.com

================================================================================
来源：http://nzb.tanke756.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nlb.jianghu66.top

================================================================================
来源：http://hno.birdmap.top

[U01] Py：创建虚拟环境
来源：http://yrl.kuanghao11.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gqh.yfazqb.com

[U02] Py：导出 / 安装依赖
来源：http://dxd.yvedp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fqy.sxryk.cn

[U03] Py：加载 .env 配置
来源：http://gzz.xylfe.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://smc.zhijiandao.cn

[U04] Py：变量调试打印
来源：http://ddg.hnqzz.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tck.redwolf501.top

[U05] Py：列表去重且保序
来源：http://qnm.0kj1m.cn

list(dict.fromkeys(arr))
来源：http://ipw.ppjwa.cn

[U06] Py：合并两个字典
来源：http://hng.fehbvm.com

{**a, **b}
来源：http://nwp.jinqigufen.top

[U07] Py：反转字典键值
来源：http://iac.mhx1999.top

{v: k for k, v in d.items()}
来源：http://xnh.zhiwuduotai.top

[U08] Py：展平二维列表
来源：http://vin.hammf.cn

[y for x in nested for y in x]
来源：http://vnv.ydzc1.top

[U09] Py：字典取最大值的键
来源：http://ooo.hywenlv.cn

max(d, key=d.get)
来源：http://thm.cucudq.cn

[U10] Py：按值排序字典
来源：http://tho.daxiang520.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ugn.pengpengdd.cyou

[U11] Py：生成器表达式
来源：http://wsf.fanxiaobao.xyz

(x * 2 for x in arr)
来源：http://gvd.hesvh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ghk.c1oappe.top

Counter(arr).most_common(3)
来源：http://vao.yuxming.cn

[U13] Py：固定长度队列
来源：http://pgq.dashuyun.cn

deque(maxlen=10)
来源：http://hbr.daria6918.cn

[U14] Py：分组收集到列表
来源：http://hrj.zhixingplan.top

defaultdict(list)
来源：http://fby.smart0.xyz

[U15] Py：高精度计时
来源：http://efi.cucudq.cn

t = time.perf_counter()
来源：http://eso.zhijiandao.cn

[U16] Py：命令行参数解析
来源：http://kku.smart0.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xeo.hcnkem.com

[U17] Py：初始化日志
来源：http://bqc.redwolf501.top

logging.basicConfig(level=logging.INFO)
来源：http://iiw.shanyushiyangtech.top

[U18] Py：预编译正则
来源：http://uwo.zhijiandao.cn

pat = re.compile(r"\d+")
来源：http://okt.cdnleiting.top

[U19] Py：正则替换带回调
来源：http://lwi.daria6918.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xkp.epnwcf.com

[U20] Py：缓存函数结果
来源：http://byj.jlsjyb.cn

@functools.lru_cache(maxsize=None)
来源：http://auk.tian-w.cn

[U21] Py：自定义上下文管理器
来源：http://cxz.zhaomingkeji.xyz

@contextlib.contextmanager
来源：http://gce.zhongyouzk.top

[U22] Py：矩阵转置
来源：http://hka.jyoumei.cn

list(zip(*m))
来源：http://yyp.xuanzx.com

[U23] Py：分块读取大文件
来源：http://jln.hnxiangtu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tbk.guowangkeji.top

[U24] Py：路径操作
来源：http://cce.zhongyouzk.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vun.uphjek.com

[U25] Py：CSV 按字典读
来源：http://pvp.sjlbkw.cn

csv.DictReader(f)
来源：http://tki.yonumen.top

[U26] Py：并发下载
来源：http://ycp.c1oappe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xqd.nanxinkj.top

[U27] Py：异步 HTTP
来源：http://cag.jinqigfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://qhl.jinqigufen.top

[U28] Py：类型别名
来源：http://syp.ydzc1.top

UserId = int
来源：http://qtm.cqqwz.cn

[U29] Py：属性校验
来源：http://ivq.ivvv.top

@property 与 @x.setter 配合
来源：http://okv.hongshengwenyu.top

[U30] Py：数据类
来源：http://nqr.gotoacloud.top

@dataclass(slots=True)
来源：http://owv.sysykeji.top

[U31] Py：单测
来源：http://gjr.gotoacloud.top

python -m pytest -q
来源：http://zxt.hnqzz.top

[U32] Py：代码格式化
来源：http://bhf.jinqigfzy.top

ruff format . && ruff check --fix .
来源：http://ccs.wangshuangyany.cn

[U33] Py：打包发布
来源：http://fvx.zhongyouzk.top

python -m build  （依赖 pyproject.toml）
来源：http://muv.hammf.cn

[U34] Py：判断编码
来源：http://jcd.gaohongyu789.top

chardet.detect(raw)
来源：http://pjl.sxryk.cn

[U35] Py：发送邮件
来源：http://rzy.andypj.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ypr.yj202588.top

[U36] Py：定时任务
来源：http://ova.cashguo.top

schedule.every(10).minutes.do(job)
来源：http://hvd.pengpengdd.cyou

[U37] Py：读写 Excel
来源：http://rxa.jinqigfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://raj.vehdjk.com

[U38] Py：获取脚本所在目录
来源：http://akr.vehdjk.com

Path(__file__).resolve().parent
来源：http://lnt.hammf.cn

[U39] Py：判断是否在交互环境
来源：http://hyc.svipenyu.cn

sys.stdout.isatty()
来源：http://uxt.sweek.top

[U40] Py：打印到标准错误
来源：http://ejq.pycfn.com

print("err", file=sys.stderr)
来源：http://elz.hongshengwenyu.top

[U41] PHP：初始化 Composer 项目
来源：http://jkd.haohaochexian.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jnw.yuxming.cn

[U42] PHP：PSR-4 自动加载
来源：http://owf.bbcook.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ryw.yuxming.cn

[U43] PHP：声明命名空间
来源：http://kfv.mhx1999.top

namespace App\Http;
来源：http://rcd.hysaishi.cn

[U44] PHP：开启严格类型
来源：http://bvg.haohaochexian.top

declare(strict_types=1);
来源：http://wsm.ybcxt.top

[U45] PHP：类型声明与返回类型
来源：http://xve.0kj1m.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ohq.shanyushiyangtech.top

[U46] PHP：可空类型
来源：http://cuf.zhijiandao.cn

?string $name = null
来源：http://mah.shuidangran.top

[U47] PHP：联合类型
来源：http://ysn.snrcjt.cn

int|string $id
来源：http://ywq.xuetiantiany.cn

[U48] PHP：纯枚举
来源：http://cds.jlsjyb.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kyq.zhijiandao.cn

[U49] PHP：只读属性
来源：http://rtt.cheryme.top

public readonly string $name
来源：http://uah.jqgfzy.top

[U50] PHP：构造器属性提升
来源：http://sjl.redwolf501.top

public function __construct(private int $id) {}
来源：http://swc.dashuyun.cn

[U51] PHP：数组解构
来源：http://mka.yonumen.top

[$a, $b] = $arr;
来源：http://lqr.316326.xyz

[U52] PHP：箭头函数
来源：http://skm.wangshuangyany.cn

$double = fn($x) => $x * 2;
来源：http://jcr.sjlbkw.cn

[U53] PHP：空合并运算符
来源：http://rjd.iojbl.cn

$v = $a ?? $b ?? "default";
来源：http://nxv.ppjwa.cn

[U54] PHP：空安全调用
来源：http://qfx.cdnleiting.top

$obj?->method()
来源：http://sxn.zhixingplan.top

[U55] PHP：match 表达式
来源：http://cwz.hcnkem.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uka.0kj1m.cn

[U56] PHP：命名参数
来源：http://iup.sjlbkw.cn

f(a: 1, b: 2)
来源：http://ogn.jyoumei.cn

[U57] PHP：字符串插值
来源：http://vzn.zdbjq.cn

"值: {$a}"
来源：http://epe.gotoacloud.top

[U58] PHP：数组三件套
来源：http://qwq.iojbl.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uip.tian-w.cn

[U59] PHP：自定义排序
来源：http://pbh.nanxuanxn.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ria.hesvh.cn

[U60] PHP：JSON 编解码
来源：http://ikw.gzhubu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://des.jyoumei.cn

[U61] PHP：正则
来源：http://jag.yongpay.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rps.jqgufenzy.top

[U62] PHP：日期对象
来源：http://kgm.zhengqikj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://udo.xziqi.cn

[U63] PHP：文件读写
来源：http://rns.xuanzx.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sza.dianchejie.cn

[U64] PHP：目录遍历
来源：http://aat.yj20258.top

glob("dir/*.php");  scandir("dir");
来源：http://pwm.sysykeji.top

[U65] PHP：会话
来源：http://wml.zdqjudy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://cku.aizwys.cn

[U66] PHP：设置 Cookie
来源：http://iot.pycfn.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hgs.jlsjyb.cn

[U67] PHP：处理文件上传
来源：http://spu.sysykeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qog.hfpthk.cn

[U68] PHP：PDO 连接
来源：http://xfb.sxryk.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://srg.epnwcf.com

[U69] PHP：PDO 预处理
来源：http://xea.sufxvd.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wlt.ywan-chungtsiang.top

[U70] PHP：PDO 事务
来源：http://gfd.nanxuanxn.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kqx.xziqi.cn

[U71] PHP：抛出异常
来源：http://com.mhx1999.top

throw new RuntimeException("失败", 500);
来源：http://fja.fzhhl.top

[U72] PHP：写错误日志
来源：http://qtn.hfpthk.cn

error_log("失败: " . $e->getMessage());
来源：http://glk.cqqwz.cn

[U73] PHP：读取 ini 配置
来源：http://rfz.mhx1999.top

parse_ini_file("config.ini", true)
来源：http://eym.zhoulong.xyz

[U74] PHP：读取环境变量
来源：http://gtc.zdbjq.cn

getenv("APP_ENV") ?: "production"
来源：http://cco.chenjidiqi.icu

[U75] PHP：依赖注入
来源：http://qmt.ppjwa.cn

composer require psr/container
来源：http://lxq.tarul.cn

[U76] PHP：简单路由
来源：http://mgt.jqgfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wzs.iojbl.cn

[U77] PHP：模板渲染
来源：http://xqx.meibo888.top

composer require twig/twig
来源：http://klh.tarul.cn

[U78] PHP：单元测试
来源：http://foo.sjlbkw.cn

composer require --dev phpunit/phpunit
来源：http://jlp.cheryme.top

[U79] PHP：静态分析
来源：http://nnl.iojbl.cn

composer require --dev phpstan/phpstan
来源：http://iul.kuanghao11.cn

[U80] PHP：代码规范修复
来源：http://geh.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lth.ppjwa.cn

[U81] JS：初始化项目
来源：http://uvn.hnxiangtu.top

npm init -y;  npm i express
来源：http://vcc.xziqi.cn

[U82] JS：package.json 脚本
来源：http://qii.tian-w.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eke.dianchejie.cn

[U83] JS：ES Module 导入导出
来源：http://ezu.hnqzz.top

export const a = 1;  import { a } from "./m.js";
来源：http://thf.cashguo.top

[U84] JS：CommonJS 写法
来源：http://gji.yueranfly.top

module.exports = { a };  const { a } = require("./m");
来源：http://vug.yfazqb.com

[U85] JS：可选链
来源：http://rou.yueranfly.top

a?.b?.c
来源：http://maq.gaohongyu789.top

[U86] JS：空值合并
来源：http://biy.cashguo.top

a ?? b
来源：http://kfo.iojbl.cn

[U87] JS：解构默认值
来源：http://yrs.vehdjk.com

const { a = 1, b = 2 } = obj;
来源：http://avu.nanxinkj.top

[U88] JS：对象展开合并
来源：http://qmi.sweek.top

{ ...a, ...b }
来源：http://nqj.tian-w.cn


<!-- 参考信息 -->