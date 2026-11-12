代发 wailian999

[T01] Kotlin：Hello World
来源：http://rpe.yfazqb.com

println("Hello")
来源：http://ste.jlsjyb.cn

[T02] Kotlin：变量
来源：http://gcy.jyoumei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mfy.hammf.cn

[T03] Kotlin：字符串模板
来源：http://wdo.andypj.xyz

"值: $b"
来源：http://tgi.jqgufenzy.top

[T04] Kotlin：空安全
来源：http://mwt.yj20258888.top

val n: String? = null;  n?.length
来源：http://mbu.zhijiandao.cn

[T05] Kotlin：when 表达式
来源：http://dqd.svipenyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yll.jiagoushi.top

[T06] Kotlin：集合映射
来源：http://hrk.hfpthk.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://psg.jinyuanbaomall.cn

[T07] Kotlin：集合过滤
来源：http://pnm.fehbvm.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://eyt.havefunace.top

[T08] Kotlin：数据类
来源：http://lvd.xylfe.cn

data class User(val name: String, val age: Int)
来源：http://sxf.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://oow.ctjpmb.com

fun String.exclaim() = this + "!"
来源：http://ttz.52xcode.cn

[T10] Kotlin：默认参数
来源：http://spy.dianchejie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xzr.gotoacloud.top

[T11] Kotlin：协程
来源：http://oqr.tian-w.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bdk.xinyue.icu

[T12] Kotlin：解构声明
来源：http://ndc.nwbrower.top

val (a, b) = Pair(1, 2)
来源：http://suy.cqqwz.cn

[T13] Kotlin：只读 Map
来源：http://qss.ppjwa.cn

val m = mapOf("a" to 1)
来源：http://pny.zdqjudy.top

[T14] Kotlin：循环
来源：http://dku.yj202588.top

for (i in 1..10) println(i)
来源：http://ata.quarkkingdee.top

[T15] Kotlin：接口
来源：http://gry.hcnkem.com

interface Shape { fun area(): Double }
来源：http://equ.fanxiaobao.xyz

[T16] Swift：Hello World
来源：http://efq.nwbrower.top

print("Hello")
来源：http://raj.jiagoushi.top

[T17] Swift：变量与常量
来源：http://ghp.yvedp.cn

var a = 1;  let b = 2
来源：http://cdk.fanxiaobao.xyz

[T18] Swift：字符串插值
来源：http://qro.iojbl.cn

"值: \(b)"
来源：http://zma.yuxming.cn

[T19] Swift：可选绑定
来源：http://vpx.sxryk.cn

if let n = opt { print(n) }
来源：http://kik.hammf.cn

[T20] Swift：数组操作
来源：http://ggp.feifeiyinyue.top

var a = [1, 2, 3];  a.append(4)
来源：http://isy.yj20258888.top

[T21] Swift：遍历
来源：http://fid.nanxinkj.top

for x in a { print(x) }
来源：http://uux.yvedp.cn

[T22] Swift：字典
来源：http://iil.jinqigfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://qre.jlsjyb.cn

[T23] Swift：函数
来源：http://dlq.ywan-chungtsiang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qgu.smart0.xyz

[T24] Swift：闭包
来源：http://hwb.epnwcf.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://fzl.jqgfzy.top

[T25] Swift：结构体
来源：http://mgl.ydzc1.top

struct P { var x: Int }
来源：http://les.vehdjk.com

[T26] Swift：类与重写
来源：http://nyg.tanke756.top

class A: Base { override func f() {} }
来源：http://apw.andypj.xyz

[T27] Swift：错误处理
来源：http://doc.hammf.cn

do { try f() } catch { print(error) }
来源：http://owh.vehdjk.com

[T28] Swift：枚举
来源：http://cae.jiagoushi.top

enum Color { case red, green }
来源：http://asu.ehwqpu.com

[T29] Swift：guard 提前返回
来源：http://xlb.feifeiyinyue.top

guard let x = opt else { return }
来源：http://jqd.meibo888.top

[T30] Swift：协议
来源：http://lli.yonumen.top

protocol Shape { func area() -> Double }
来源：http://ftz.ybcxt.top

[T31] Lua：Hello World
来源：http://pzy.0kj1m.cn

print("Hello")
来源：http://zgo.yonumen.top

[T32] Lua：局部变量
来源：http://zkm.ivvv.top

local a = 1
来源：http://oeo.fktsv.cn

[T33] Lua：表（数组）
来源：http://vom.vehdjk.com

local t = {1, 2, 3};  t[4] = 4
来源：http://ewb.cdnleiting.top

[T34] Lua：遍历表
来源：http://akc.daria6918.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tfx.nwbrower.top

[T35] Lua：字典表
来源：http://kcd.kuanghao11.cn

local d = { a = 1 };  d.b = 2
来源：http://xgt.daria6918.cn

[T36] Lua：函数
来源：http://anw.daria6918.cn

function add(a, b) return a + b end
来源：http://neu.jianghu66.top

[T37] Lua：字符串拼接
来源：http://leo.jinqigfzy.top

"a" .. "b"
来源：http://swh.kuanghao11.cn

[T38] Lua：条件
来源：http://mdu.kuanghao11.cn

if x > 0 then print("正") end
来源：http://lzc.fzhhl.top

[T39] Lua：模式匹配
来源：http://lim.yj20258888.top

string.find(s, "%d+")
来源：http://bal.cdnleiting.top

[T40] Lua：元表
来源：http://ywm.fengsongda.top

setmetatable({}, { __index = base })
来源：http://mga.jinqigufen.top

[T41] Perl：Hello World
来源：http://dlz.sufxvd.cn

print "Hello\n";
来源：http://ueb.0kj1m.cn

[T42] Perl：变量类型
来源：http://ccb.ppjwa.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wwe.fengsongda.top

[T43] Perl：字符串插值
来源：http://gtv.fengsongda.top

"值: $a"
来源：http://nnq.hcnkem.com

[T44] Perl：条件
来源：http://ukr.fanxiaobao.xyz

if ($a > 0) { print "正"; }
来源：http://kdk.jqgfzy.top

[T45] Perl：数组遍历
来源：http://pbf.zhaomingkeji.xyz

for my $x (@arr) { print $x; }
来源：http://vaa.ybcxt.top

[T46] Perl：哈希操作
来源：http://erc.vehdjk.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yrw.pengpengdd.cyou

[T47] Perl：正则捕获
来源：http://dbl.yj20258888.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://csh.wangshuangyany.cn

[T48] Perl：正则替换
来源：http://nvv.fehbvm.com

$s =~ s/old/new/g;
来源：http://lek.pengpengdd.cyou

[T49] Perl：函数
来源：http://rlv.zhiwuduotai.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nnr.gzhubu.top

[T50] Perl：逐行读文件
来源：http://bcg.52xcode.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gyf.ivvv.top

while (my $line = <$fh>) { print $line; }
来源：http://xal.yanxiufei.cn

[T51] Scala：Hello World
来源：http://ggs.iojbl.cn

println("Hello")
来源：http://izu.yj20258.top

[T52] Scala：变量
来源：http://nci.zhiwuduotai.top

val a = 1;  var b = 2
来源：http://vfo.fanxiaobao.xyz

[T53] Scala：字符串插值
来源：http://hkd.tanke756.top

s"值: $b"
来源：http://tku.zdqjudy.top

[T54] Scala：集合映射
来源：http://jfb.xingfuxueyuan.xyz

List(1, 2, 3).map(_ * 2)
来源：http://mzn.jqgufenzy.top

[T55] Scala：集合过滤
来源：http://ojt.sjlbkw.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qvy.0kj1m.cn

[T56] Scala：样例类
来源：http://iit.mhx1999.top

case class User(name: String, age: Int)
来源：http://ifs.dianchejie.cn

[T57] Scala：模式匹配
来源：http://ciq.xziqi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tyk.chenzaomai.com

[T58] Scala：函数定义
来源：http://tci.dashuyun.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kkx.dashuyun.cn

[T59] Scala：循环
来源：http://pts.cashguo.top

for (i <- 1 to 10) println(i)
来源：http://vec.hfpthk.cn

[T60] Scala：折叠
来源：http://jjn.snrcjt.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uka.hywenlv.cn

================================================================================
来源：http://ztz.52xcode.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nuk.jqgufenzy.top

================================================================================
来源：http://iix.yueranfly.top

[U01] Py：创建虚拟环境
来源：http://sqa.hnqzz.top

python -m venv .venv && source .venv/bin/activate
来源：http://xnf.daria6918.cn

[U02] Py：导出 / 安装依赖
来源：http://tai.zdbjq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://szz.feifeiyinyue.top

[U03] Py：加载 .env 配置
来源：http://grj.gaohongyu789.top

from dotenv import load_dotenv; load_dotenv()
来源：http://hel.hnxiangtu.top

[U04] Py：变量调试打印
来源：http://oej.svipenyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lyo.shanyushiyangkeji.top

[U05] Py：列表去重且保序
来源：http://xdw.snrcjt.cn

list(dict.fromkeys(arr))
来源：http://jtq.zhengqikj.top

[U06] Py：合并两个字典
来源：http://ifm.yangfankeji.com

{**a, **b}
来源：http://bdw.tian-w.cn

[U07] Py：反转字典键值
来源：http://tir.jianghu66.top

{v: k for k, v in d.items()}
来源：http://dif.yj202588.top

[U08] Py：展平二维列表
来源：http://fqe.sxryk.cn

[y for x in nested for y in x]
来源：http://xpu.nwbrower.top

[U09] Py：字典取最大值的键
来源：http://smt.xingfuxueyuan.xyz

max(d, key=d.get)
来源：http://jhq.cqqwz.cn

[U10] Py：按值排序字典
来源：http://rzi.hnxiangtu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dmy.fehbvm.com

[U11] Py：生成器表达式
来源：http://mes.zhijiandao.cn

(x * 2 for x in arr)
来源：http://kba.zhongyouzk.top

[U12] Py：取出现最多的 3 个元素
来源：http://unv.bjfxy.top

Counter(arr).most_common(3)
来源：http://hei.wangdashe.top

[U13] Py：固定长度队列
来源：http://mtt.jiagoushi.top

deque(maxlen=10)
来源：http://xmj.tarul.cn

[U14] Py：分组收集到列表
来源：http://bef.hesvh.cn

defaultdict(list)
来源：http://der.yj202588.top

[U15] Py：高精度计时
来源：http://hio.gzhubu.top

t = time.perf_counter()
来源：http://njx.yj20258888.top

[U16] Py：命令行参数解析
来源：http://mfr.meibo888.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://omp.sjlbkw.cn

[U17] Py：初始化日志
来源：http://tjy.ydjk.org.cn

logging.basicConfig(level=logging.INFO)
来源：http://mpz.zhaomingkeji.xyz

[U18] Py：预编译正则
来源：http://cyt.wangshuangyany.cn

pat = re.compile(r"\d+")
来源：http://puv.jinqigufen.top

[U19] Py：正则替换带回调
来源：http://nke.chenzaomai.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gef.wangshuangyany.cn

[U20] Py：缓存函数结果
来源：http://sqc.zhoulong.xyz

@functools.lru_cache(maxsize=None)
来源：http://egm.sysykeji.top

[U21] Py：自定义上下文管理器
来源：http://gtf.9152youxi.cn

@contextlib.contextmanager
来源：http://joz.chenlongwang.top

[U22] Py：矩阵转置
来源：http://esi.birdmap.top

list(zip(*m))
来源：http://gbp.iojbl.cn

[U23] Py：分块读取大文件
来源：http://ahq.xinyue.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dog.jiagoushi.top

[U24] Py：路径操作
来源：http://ixp.hfpthk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gsq.shzxlz.cn

[U25] Py：CSV 按字典读
来源：http://qxg.guannengcc.top

csv.DictReader(f)
来源：http://jih.cashguo.top

[U26] Py：并发下载
来源：http://vna.hysaishi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zpt.hammf.cn

[U27] Py：异步 HTTP
来源：http://msj.hesvh.cn

aiohttp.ClientSession() 配合 async with
来源：http://kpy.ydzc1.top

[U28] Py：类型别名
来源：http://mcr.yj20258.top

UserId = int
来源：http://njk.aizwys.cn

[U29] Py：属性校验
来源：http://jpr.zhongyouzk.top

@property 与 @x.setter 配合
来源：http://cgx.yanxiufei.cn

[U30] Py：数据类
来源：http://mil.daria6918.cn

@dataclass(slots=True)
来源：http://zqc.jiagoushi.top

[U31] Py：单测
来源：http://zve.ivvv.top

python -m pytest -q
来源：http://tso.guannengcc.top

[U32] Py：代码格式化
来源：http://vky.tanke756.top

ruff format . && ruff check --fix .
来源：http://pxr.shuidangran.top

[U33] Py：打包发布
来源：http://ozp.mhx1999.top

python -m build  （依赖 pyproject.toml）
来源：http://dbl.yuanzhike.top

[U34] Py：判断编码
来源：http://voo.uphjek.com

chardet.detect(raw)
来源：http://rik.jlsjyb.cn

[U35] Py：发送邮件
来源：http://agp.cashguo.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ygq.shangyingyoupin.top

[U36] Py：定时任务
来源：http://jdq.guannengcc.top

schedule.every(10).minutes.do(job)
来源：http://lxt.ybcxt.top

[U37] Py：读写 Excel
来源：http://nxw.xuanzx.com

pandas.read_excel / DataFrame.to_excel
来源：http://fnd.cqqwz.cn

[U38] Py：获取脚本所在目录
来源：http://bze.snrcjt.cn

Path(__file__).resolve().parent
来源：http://nlr.svipenyu.cn

[U39] Py：判断是否在交互环境
来源：http://bge.zhiwuduotai.top

sys.stdout.isatty()
来源：http://mzr.yvedp.cn

[U40] Py：打印到标准错误
来源：http://yuk.bjfxy.top

print("err", file=sys.stderr)
来源：http://mlg.ctjpmb.com

[U41] PHP：初始化 Composer 项目
来源：http://uyt.yj202588.top

composer init;  composer require guzzlehttp/guzzle
来源：http://mis.feifeiyinyue.top

[U42] PHP：PSR-4 自动加载
来源：http://ozo.sufxvd.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mly.xuetiantiany.cn

[U43] PHP：声明命名空间
来源：http://rep.sweek.top

namespace App\Http;
来源：http://gxr.c1oappe.top

[U44] PHP：开启严格类型
来源：http://imx.hammf.cn

declare(strict_types=1);
来源：http://sth.cqqwz.cn

[U45] PHP：类型声明与返回类型
来源：http://gro.uphjek.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://lss.uphjek.com

[U46] PHP：可空类型
来源：http://sha.jinghuilouyu.cn

?string $name = null
来源：http://mwz.uphjek.com

[U47] PHP：联合类型
来源：http://gva.pycfn.com

int|string $id
来源：http://chw.svipenyu.cn

[U48] PHP：纯枚举
来源：http://tkt.jinyuanbaomall.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jqe.zhongyouzk.top

[U49] PHP：只读属性
来源：http://joj.cucudq.cn

public readonly string $name
来源：http://jzz.xylfe.cn

[U50] PHP：构造器属性提升
来源：http://xmm.snrcjt.cn

public function __construct(private int $id) {}
来源：http://xly.wangdashe.top

[U51] PHP：数组解构
来源：http://qxq.ehwqpu.com

[$a, $b] = $arr;
来源：http://pwt.zhixingplan.top

[U52] PHP：箭头函数
来源：http://aba.zhoulong.xyz

$double = fn($x) => $x * 2;
来源：http://afu.tianlin.xyz

[U53] PHP：空合并运算符
来源：http://ryc.gaohongyu789.top

$v = $a ?? $b ?? "default";
来源：http://igz.9152youxi.cn

[U54] PHP：空安全调用
来源：http://orf.tian-w.cn

$obj?->method()
来源：http://wnn.aizwys.cn

[U55] PHP：match 表达式
来源：http://ejh.ivvv.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nxn.daxiang520.top

[U56] PHP：命名参数
来源：http://fyg.zdbjq.cn

f(a: 1, b: 2)
来源：http://orn.zhaomingkeji.xyz

[U57] PHP：字符串插值
来源：http://fmq.cashguo.top

"值: {$a}"
来源：http://pdg.dianchejie.cn

[U58] PHP：数组三件套
来源：http://ipn.jinqigufen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ugf.ybcxt.top

[U59] PHP：自定义排序
来源：http://lal.aibaodan.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fim.xingfuxueyuan.xyz

[U60] PHP：JSON 编解码
来源：http://jeo.vehdjk.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xcq.vqdsnc.cn

[U61] PHP：正则
来源：http://ycu.yongpay.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sau.haohaochexian.top

[U62] PHP：日期对象
来源：http://nyh.pycfn.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vba.aizwys.cn

[U63] PHP：文件读写
来源：http://xmz.xylfe.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ihr.svipenyu.cn

[U64] PHP：目录遍历
来源：http://run.kuanghao11.cn

glob("dir/*.php");  scandir("dir");
来源：http://pnt.jyoumei.cn

[U65] PHP：会话
来源：http://puc.kuanghao11.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://oac.hnxiangtu.top

[U66] PHP：设置 Cookie
来源：http://pxv.jlsjyb.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cds.meibo888.top

[U67] PHP：处理文件上传
来源：http://pka.shzxlz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qyu.fzhhl.top

[U68] PHP：PDO 连接
来源：http://elu.vqdsnc.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fmf.sweek.top

[U69] PHP：PDO 预处理
来源：http://lmh.tarul.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://moh.jqgfzy.top

[U70] PHP：PDO 事务
来源：http://xzx.zhixingplan.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bgt.jinqigufen.top

[U71] PHP：抛出异常
来源：http://mbx.cqqwz.cn

throw new RuntimeException("失败", 500);
来源：http://yvm.guannengcc.top

[U72] PHP：写错误日志
来源：http://oju.quarkkingdee.top

error_log("失败: " . $e->getMessage());
来源：http://skf.fanxiaobao.xyz

[U73] PHP：读取 ini 配置
来源：http://yqq.9152youxi.cn

parse_ini_file("config.ini", true)
来源：http://fjk.pengpengdd.cyou

[U74] PHP：读取环境变量
来源：http://bwq.guowangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://asp.hesvh.cn

[U75] PHP：依赖注入
来源：http://pvi.zhaomingkeji.xyz

composer require psr/container
来源：http://iff.smart0.xyz

[U76] PHP：简单路由
来源：http://mcc.sweek.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qsj.daxiang520.top

[U77] PHP：模板渲染
来源：http://rlr.hcnkem.com

composer require twig/twig
来源：http://nhw.tianlin.xyz

[U78] PHP：单元测试
来源：http://vwa.yuanzhike.top

composer require --dev phpunit/phpunit
来源：http://mtx.chenzaomai.com

[U79] PHP：静态分析
来源：http://lbm.hysaishi.cn

composer require --dev phpstan/phpstan
来源：http://cuo.nanxuanxn.top

[U80] PHP：代码规范修复
来源：http://qde.hywenlv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://znw.zhixingplan.top

[U81] JS：初始化项目
来源：http://inl.nanxinkj.top

npm init -y;  npm i express
来源：http://rey.sweek.top

[U82] JS：package.json 脚本
来源：http://ajc.vehdjk.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cgu.vehdjk.com

[U83] JS：ES Module 导入导出
来源：http://zxf.dianchejie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vdp.cqqwz.cn

[U84] JS：CommonJS 写法
来源：http://rcj.yj20258.top

module.exports = { a };  const { a } = require("./m");
来源：http://lhl.jqgufenzy.top

[U85] JS：可选链
来源：http://pvw.shanyushiyangkeji.top

a?.b?.c
来源：http://njj.snrcjt.cn

[U86] JS：空值合并
来源：http://yht.zhixingplan.top

a ?? b
来源：http://irq.yangfankeji.com

[U87] JS：解构默认值
来源：http://ujm.c1oappe.top

const { a = 1, b = 2 } = obj;
来源：http://mot.pycfn.com

[U88] JS：对象展开合并
来源：http://zvn.yanxiufei.cn

{ ...a, ...b }
来源：http://wtv.chenjidiqi.icu


<!-- 参考信息 -->