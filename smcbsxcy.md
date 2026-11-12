代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xnw.jinqigfzy.top

================================================================================
来源：http://xsl.ppjwa.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ecz.fengsongda.top

================================================================================
来源：http://hil.shuidangran.top

[T01] Kotlin：Hello World
来源：http://kmo.andypj.xyz

println("Hello")
来源：http://jzn.guowangkeji.top

[T02] Kotlin：变量
来源：http://hca.nanxinkj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wmv.sweek.top

[T03] Kotlin：字符串模板
来源：http://ipa.52xcode.cn

"值: $b"
来源：http://guc.nwbrower.top

[T04] Kotlin：空安全
来源：http://xyq.sufxvd.cn

val n: String? = null;  n?.length
来源：http://fmn.cdnleiting.top

[T05] Kotlin：when 表达式
来源：http://mcx.hysaishi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dlo.birdmap.top

[T06] Kotlin：集合映射
来源：http://sot.cqqwz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zcq.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://eyg.zhengqikj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tgx.tanke756.top

[T08] Kotlin：数据类
来源：http://rcm.nwbrower.top

data class User(val name: String, val age: Int)
来源：http://vyq.cashguo.top

[T09] Kotlin：扩展函数
来源：http://qmq.zdqjudy.top

fun String.exclaim() = this + "!"
来源：http://oig.fehbvm.com

[T10] Kotlin：默认参数
来源：http://whx.xylfe.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nej.tarul.cn

[T11] Kotlin：协程
来源：http://uqh.gaohongyu789.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://srk.fehbvm.com

[T12] Kotlin：解构声明
来源：http://zjc.gaohongyu789.top

val (a, b) = Pair(1, 2)
来源：http://znz.uphjek.com

[T13] Kotlin：只读 Map
来源：http://igk.nwbrower.top

val m = mapOf("a" to 1)
来源：http://fbw.birdmap.top

[T14] Kotlin：循环
来源：http://trs.yj20258888.top

for (i in 1..10) println(i)
来源：http://oqd.shangyingyoupin.top

[T15] Kotlin：接口
来源：http://arc.mhx1999.top

interface Shape { fun area(): Double }
来源：http://mcg.jinyuanbaomall.cn

[T16] Swift：Hello World
来源：http://gui.yfazqb.com

print("Hello")
来源：http://jek.vqdsnc.cn

[T17] Swift：变量与常量
来源：http://uxr.yongpay.top

var a = 1;  let b = 2
来源：http://yri.zhixingplan.top

[T18] Swift：字符串插值
来源：http://ljx.havefunace.top

"值: \(b)"
来源：http://xuk.ydzc1.top

[T19] Swift：可选绑定
来源：http://lrk.yvedp.cn

if let n = opt { print(n) }
来源：http://kin.andypj.xyz

[T20] Swift：数组操作
来源：http://gjq.tanke756.top

var a = [1, 2, 3];  a.append(4)
来源：http://ipr.jlsjyb.cn

[T21] Swift：遍历
来源：http://han.shanyushiyangkeji.top

for x in a { print(x) }
来源：http://dpf.zhixingplan.top

[T22] Swift：字典
来源：http://qdj.yj20258.top

var d = ["a": 1];  d["b"] = 2
来源：http://hic.xziqi.cn

[T23] Swift：函数
来源：http://fdp.52xcode.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sdq.daria6918.cn

[T24] Swift：闭包
来源：http://wfl.xziqi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yrp.zhijiandao.cn

[T25] Swift：结构体
来源：http://zpe.epnwcf.com

struct P { var x: Int }
来源：http://ihh.jlsjyb.cn

[T26] Swift：类与重写
来源：http://kdu.yanxiufei.cn

class A: Base { override func f() {} }
来源：http://gko.yfazqb.com

[T27] Swift：错误处理
来源：http://bmq.andypj.xyz

do { try f() } catch { print(error) }
来源：http://uti.gotoacloud.top

[T28] Swift：枚举
来源：http://kgc.vehdjk.com

enum Color { case red, green }
来源：http://ogw.yanxiufei.cn

[T29] Swift：guard 提前返回
来源：http://ufv.andypj.xyz

guard let x = opt else { return }
来源：http://bzp.yangfankeji.com

[T30] Swift：协议
来源：http://xzd.jqgfzy.top

protocol Shape { func area() -> Double }
来源：http://juk.hongshengwenyu.top

[T31] Lua：Hello World
来源：http://vmg.jqgufenzy.top

print("Hello")
来源：http://vwd.yonumen.top

[T32] Lua：局部变量
来源：http://gqu.xziqi.cn

local a = 1
来源：http://ecq.fzhhl.top

[T33] Lua：表（数组）
来源：http://cnf.zhijiandao.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cdz.jyoumei.cn

[T34] Lua：遍历表
来源：http://kfo.smart0.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://gus.shuidangran.top

[T35] Lua：字典表
来源：http://amy.gzhubu.top

local d = { a = 1 };  d.b = 2
来源：http://gon.jinqigfzy.top

[T36] Lua：函数
来源：http://qsx.zhijiandao.cn

function add(a, b) return a + b end
来源：http://thu.hongshengwenyu.top

[T37] Lua：字符串拼接
来源：http://syt.nanxinkj.top

"a" .. "b"
来源：http://qgk.dashuyun.cn

[T38] Lua：条件
来源：http://iai.zhongyouzk.top

if x > 0 then print("正") end
来源：http://hkk.zhengqikj.top

[T39] Lua：模式匹配
来源：http://vkx.ehwqpu.com

string.find(s, "%d+")
来源：http://lvv.mhx1999.top

[T40] Lua：元表
来源：http://zsz.yj20258888.top

setmetatable({}, { __index = base })
来源：http://mnm.havefunace.top

[T41] Perl：Hello World
来源：http://yaw.yuxming.cn

print "Hello\n";
来源：http://xfo.fehbvm.com

[T42] Perl：变量类型
来源：http://kbu.tanke756.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oje.tarul.cn

[T43] Perl：字符串插值
来源：http://fwe.smart0.xyz

"值: $a"
来源：http://tif.316326.xyz

[T44] Perl：条件
来源：http://iln.gaohongyu789.top

if ($a > 0) { print "正"; }
来源：http://mso.guannengcc.top

[T45] Perl：数组遍历
来源：http://vtq.shangyingyoupin.top

for my $x (@arr) { print $x; }
来源：http://dzx.tarul.cn

[T46] Perl：哈希操作
来源：http://oyo.aibaodan.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ohp.ehwqpu.com

[T47] Perl：正则捕获
来源：http://sks.chenjidiqi.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://aqx.sweek.top

[T48] Perl：正则替换
来源：http://otb.zhiwuduotai.top

$s =~ s/old/new/g;
来源：http://urc.jqgfzy.top

[T49] Perl：函数
来源：http://cfs.wangdashe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://axc.zhixingplan.top

[T50] Perl：逐行读文件
来源：http://xdk.hysaishi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vxy.aizwys.cn

while (my $line = <$fh>) { print $line; }
来源：http://zyw.jqgufenzy.top

[T51] Scala：Hello World
来源：http://tnm.wangshuangyany.cn

println("Hello")
来源：http://jgw.hnxiangtu.top

[T52] Scala：变量
来源：http://lfa.yangfankeji.com

val a = 1;  var b = 2
来源：http://nbv.jiagoushi.top

[T53] Scala：字符串插值
来源：http://krt.yuanzhike.top

s"值: $b"
来源：http://dfi.fengsongda.top

[T54] Scala：集合映射
来源：http://soa.shanyushiyangtech.top

List(1, 2, 3).map(_ * 2)
来源：http://rea.yfazqb.com

[T55] Scala：集合过滤
来源：http://sff.jlsjyb.cn

List(1, 2, 3).filter(_ > 1)
来源：http://adi.0kj1m.cn

[T56] Scala：样例类
来源：http://ftt.shanyushiyangtech.top

case class User(name: String, age: Int)
来源：http://ljj.aibaodan.cn

[T57] Scala：模式匹配
来源：http://hws.hysaishi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://eco.zhaomingkeji.xyz

[T58] Scala：函数定义
来源：http://tgr.chenlongwang.top

def add(a: Int, b: Int): Int = a + b
来源：http://mos.zdbjq.cn

[T59] Scala：循环
来源：http://hmy.ybcxt.top

for (i <- 1 to 10) println(i)
来源：http://hfi.sysykeji.top

[T60] Scala：折叠
来源：http://alv.wangdashe.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://shf.fengsongda.top

================================================================================
来源：http://fuk.hongshengwenyu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gfi.bjfxy.top

================================================================================
来源：http://wbl.guowangkeji.top

[U01] Py：创建虚拟环境
来源：http://hhw.ydzc1.top

python -m venv .venv && source .venv/bin/activate
来源：http://uvt.svipenyu.cn

[U02] Py：导出 / 安装依赖
来源：http://ljr.bjfxy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wjb.zhongyouzk.top

[U03] Py：加载 .env 配置
来源：http://gwj.chenzaomai.com

from dotenv import load_dotenv; load_dotenv()
来源：http://uwx.jinyuanbaomall.cn

[U04] Py：变量调试打印
来源：http://lpz.0kj1m.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nco.chenlongwang.top

[U05] Py：列表去重且保序
来源：http://jrd.wangdashe.top

list(dict.fromkeys(arr))
来源：http://ykp.0kj1m.cn

[U06] Py：合并两个字典
来源：http://vir.hysaishi.cn

{**a, **b}
来源：http://des.wangshuangyany.cn

[U07] Py：反转字典键值
来源：http://bsj.yfazqb.com

{v: k for k, v in d.items()}
来源：http://fhg.svipenyu.cn

[U08] Py：展平二维列表
来源：http://fvw.shanyushiyangtech.top

[y for x in nested for y in x]
来源：http://wgs.guowangkeji.top

[U09] Py：字典取最大值的键
来源：http://ozs.jqgfzy.top

max(d, key=d.get)
来源：http://tzd.kuanghao11.cn

[U10] Py：按值排序字典
来源：http://msg.yonumen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rhx.sxryk.cn

[U11] Py：生成器表达式
来源：http://bhb.ehwqpu.com

(x * 2 for x in arr)
来源：http://myb.xuanzx.com

[U12] Py：取出现最多的 3 个元素
来源：http://kws.cucudq.cn

Counter(arr).most_common(3)
来源：http://nqi.fzhhl.top

[U13] Py：固定长度队列
来源：http://bpy.redwolf501.top

deque(maxlen=10)
来源：http://pmb.hysaishi.cn

[U14] Py：分组收集到列表
来源：http://mxo.tian-w.cn

defaultdict(list)
来源：http://aws.tianlin.xyz

[U15] Py：高精度计时
来源：http://rgr.fanxiaobao.xyz

t = time.perf_counter()
来源：http://nnv.c1oappe.top

[U16] Py：命令行参数解析
来源：http://gur.316326.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lps.hfpthk.cn

[U17] Py：初始化日志
来源：http://paf.snrcjt.cn

logging.basicConfig(level=logging.INFO)
来源：http://itt.pycfn.com

[U18] Py：预编译正则
来源：http://klz.shangyingyoupin.top

pat = re.compile(r"\d+")
来源：http://eut.hcnkem.com

[U19] Py：正则替换带回调
来源：http://ooa.bjfxy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rtn.svipenyu.cn

[U20] Py：缓存函数结果
来源：http://ync.yanxiufei.cn

@functools.lru_cache(maxsize=None)
来源：http://ijf.316326.xyz

[U21] Py：自定义上下文管理器
来源：http://fhg.jinyuanbaomall.cn

@contextlib.contextmanager
来源：http://vty.xinyue.icu

[U22] Py：矩阵转置
来源：http://hzh.shuidangran.top

list(zip(*m))
来源：http://vzs.zhengqikj.top

[U23] Py：分块读取大文件
来源：http://pqq.hammf.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://etd.andypj.xyz

[U24] Py：路径操作
来源：http://cgg.meibo888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yca.snrcjt.cn

[U25] Py：CSV 按字典读
来源：http://kyv.yuanzhike.top

csv.DictReader(f)
来源：http://nfn.guowangkeji.top

[U26] Py：并发下载
来源：http://qzd.aizwys.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bnk.dashuyun.cn

[U27] Py：异步 HTTP
来源：http://ywp.guannengcc.top

aiohttp.ClientSession() 配合 async with
来源：http://vuz.fengsongda.top

[U28] Py：类型别名
来源：http://hkl.52xcode.cn

UserId = int
来源：http://qnu.hammf.cn

[U29] Py：属性校验
来源：http://zwb.xinyue.icu

@property 与 @x.setter 配合
来源：http://efa.nwbrower.top

[U30] Py：数据类
来源：http://psa.fanxiaobao.xyz

@dataclass(slots=True)
来源：http://fan.zhiwuduotai.top

[U31] Py：单测
来源：http://wuf.chenzaomai.com

python -m pytest -q
来源：http://xdn.fehbvm.com

[U32] Py：代码格式化
来源：http://nlz.yangfankeji.com

ruff format . && ruff check --fix .
来源：http://apt.hnxiangtu.top

[U33] Py：打包发布
来源：http://zjt.birdmap.top

python -m build  （依赖 pyproject.toml）
来源：http://xoq.haohaochexian.top

[U34] Py：判断编码
来源：http://grc.iojbl.cn

chardet.detect(raw)
来源：http://btb.epnwcf.com

[U35] Py：发送邮件
来源：http://phi.sysykeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xwn.zhijiandao.cn

[U36] Py：定时任务
来源：http://aat.xingfuxueyuan.xyz

schedule.every(10).minutes.do(job)
来源：http://hef.zhongyouzk.top

[U37] Py：读写 Excel
来源：http://azf.sjlbkw.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yqu.52xcode.cn

[U38] Py：获取脚本所在目录
来源：http://crc.svipenyu.cn

Path(__file__).resolve().parent
来源：http://ifk.xylfe.cn

[U39] Py：判断是否在交互环境
来源：http://rxq.aibaodan.cn

sys.stdout.isatty()
来源：http://grj.kuanghao11.cn

[U40] Py：打印到标准错误
来源：http://clr.hesvh.cn

print("err", file=sys.stderr)
来源：http://jjp.fengsongda.top

[U41] PHP：初始化 Composer 项目
来源：http://fun.jlsjyb.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jar.shanyushiyangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://ngs.yanxiufei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uun.jyoumei.cn

[U43] PHP：声明命名空间
来源：http://thm.jinqigufen.top

namespace App\Http;
来源：http://dfl.xingfuxueyuan.xyz

[U44] PHP：开启严格类型
来源：http://szy.hnqzz.top

declare(strict_types=1);
来源：http://hva.yueranfly.top

[U45] PHP：类型声明与返回类型
来源：http://ucp.hnxiangtu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pvf.xylfe.cn

[U46] PHP：可空类型
来源：http://dcz.jlsjyb.cn

?string $name = null
来源：http://bzp.yueranfly.top

[U47] PHP：联合类型
来源：http://oqs.zhongyouzk.top

int|string $id
来源：http://mws.jyoumei.cn

[U48] PHP：纯枚举
来源：http://oes.zhengqikj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mgg.kuanghao11.cn

[U49] PHP：只读属性
来源：http://gbd.birdmap.top

public readonly string $name
来源：http://dmt.316326.xyz

[U50] PHP：构造器属性提升
来源：http://hsm.zhongyouzk.top

public function __construct(private int $id) {}
来源：http://qpd.316326.xyz

[U51] PHP：数组解构
来源：http://aiz.guowangkeji.top

[$a, $b] = $arr;
来源：http://mle.smart0.xyz

[U52] PHP：箭头函数
来源：http://fxj.nwbrower.top

$double = fn($x) => $x * 2;
来源：http://tgj.hammf.cn

[U53] PHP：空合并运算符
来源：http://qgn.jyoumei.cn

$v = $a ?? $b ?? "default";
来源：http://cqz.uphjek.com

[U54] PHP：空安全调用
来源：http://ceq.jinghuilouyu.cn

$obj?->method()
来源：http://nej.c1oappe.top

[U55] PHP：match 表达式
来源：http://uqo.birdmap.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://soy.cdnleiting.top

[U56] PHP：命名参数
来源：http://eyo.yvedp.cn

f(a: 1, b: 2)
来源：http://iwk.tian-w.cn

[U57] PHP：字符串插值
来源：http://jpx.jinyuanbaomall.cn

"值: {$a}"
来源：http://yap.guannengcc.top

[U58] PHP：数组三件套
来源：http://zaz.ywan-chungtsiang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://snu.sjlbkw.cn

[U59] PHP：自定义排序
来源：http://bnv.sysykeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pat.52xcode.cn

[U60] PHP：JSON 编解码
来源：http://nkg.ehwqpu.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://suv.zycfv.cn

[U61] PHP：正则
来源：http://qen.guowangkeji.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hbp.ppjwa.cn

[U62] PHP：日期对象
来源：http://jgb.yuxming.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jbj.zdbjq.cn

[U63] PHP：文件读写
来源：http://txf.yanxiufei.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vry.fanxiaobao.xyz

[U64] PHP：目录遍历
来源：http://lev.wangshuangyany.cn

glob("dir/*.php");  scandir("dir");
来源：http://vqi.c1oappe.top

[U65] PHP：会话
来源：http://afi.fktsv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fiw.jiagoushi.top

[U66] PHP：设置 Cookie
来源：http://ebv.cqqwz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fon.uphjek.com

[U67] PHP：处理文件上传
来源：http://eqn.iojbl.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dte.xylfe.cn

[U68] PHP：PDO 连接
来源：http://xpe.zhiwuduotai.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://syh.gotoacloud.top

[U69] PHP：PDO 预处理
来源：http://exo.tianlin.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fcs.yuxming.cn

[U70] PHP：PDO 事务
来源：http://nwq.shanyushiyangkeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tiw.yfazqb.com

[U71] PHP：抛出异常
来源：http://sux.xuanzx.com

throw new RuntimeException("失败", 500);
来源：http://wle.yj20258.top

[U72] PHP：写错误日志
来源：http://vsf.tarul.cn

error_log("失败: " . $e->getMessage());
来源：http://sar.guowangkeji.top

[U73] PHP：读取 ini 配置
来源：http://cqa.svipenyu.cn

parse_ini_file("config.ini", true)
来源：http://ako.smart0.xyz

[U74] PHP：读取环境变量
来源：http://rfp.snrcjt.cn

getenv("APP_ENV") ?: "production"
来源：http://srs.vehdjk.com

[U75] PHP：依赖注入
来源：http://iqc.smart0.xyz

composer require psr/container
来源：http://xzx.ybcxt.top

[U76] PHP：简单路由
来源：http://irp.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tho.haohaochexian.top

[U77] PHP：模板渲染
来源：http://qvt.sufxvd.cn

composer require twig/twig
来源：http://uym.guannengcc.top

[U78] PHP：单元测试
来源：http://shc.havefunace.top

composer require --dev phpunit/phpunit
来源：http://rhy.tanke756.top

[U79] PHP：静态分析
来源：http://sly.aibaodan.cn

composer require --dev phpstan/phpstan
来源：http://qab.sxryk.cn

[U80] PHP：代码规范修复
来源：http://zer.shanyushiyangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qaq.jianghu66.top

[U81] JS：初始化项目
来源：http://qkt.ybcxt.top

npm init -y;  npm i express
来源：http://ing.zhaomingkeji.xyz

[U82] JS：package.json 脚本
来源：http://xdd.chenjidiqi.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://brl.jinyuanbaomall.cn

[U83] JS：ES Module 导入导出
来源：http://flb.tian-w.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ive.yj20258.top

[U84] JS：CommonJS 写法
来源：http://pgv.hongshengwenyu.top

module.exports = { a };  const { a } = require("./m");
来源：http://lth.hywenlv.cn

[U85] JS：可选链
来源：http://sdh.zhoulong.xyz

a?.b?.c
来源：http://ksj.redwolf501.top

[U86] JS：空值合并
来源：http://bbw.quarkkingdee.top

a ?? b
来源：http://lfd.316326.xyz


<!-- 参考信息 -->