代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://rxa.chenzaomai.com

[S59] C++：静态断言
来源：http://lqy.hnxiangtu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xpp.tanke756.top

[S60] C++：遍历并删除元素
来源：http://uvu.xylfe.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bma.yanxiufei.cn

================================================================================
来源：http://jfz.ydzc1.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oxg.9152youxi.cn

================================================================================
来源：http://bdy.hcnkem.com

[T01] Kotlin：Hello World
来源：http://eyc.chenjidiqi.icu

println("Hello")
来源：http://bgy.cqqwz.cn

[T02] Kotlin：变量
来源：http://owo.tarul.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ipy.pycfn.com

[T03] Kotlin：字符串模板
来源：http://kgo.tanke756.top

"值: $b"
来源：http://hyg.yonumen.top

[T04] Kotlin：空安全
来源：http://uyy.cqqwz.cn

val n: String? = null;  n?.length
来源：http://lqv.zhaomingkeji.xyz

[T05] Kotlin：when 表达式
来源：http://wru.yvedp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hcf.cdnleiting.top

[T06] Kotlin：集合映射
来源：http://urg.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jdh.snrcjt.cn

[T07] Kotlin：集合过滤
来源：http://ijo.nanxinkj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vic.shanyushiyangtech.top

[T08] Kotlin：数据类
来源：http://rdq.yanxiufei.cn

data class User(val name: String, val age: Int)
来源：http://kcc.epnwcf.com

[T09] Kotlin：扩展函数
来源：http://ura.andypj.xyz

fun String.exclaim() = this + "!"
来源：http://xxf.dianchejie.cn

[T10] Kotlin：默认参数
来源：http://oyy.andypj.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://cex.fehbvm.com

[T11] Kotlin：协程
来源：http://pcu.quarkkingdee.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qgt.yfazqb.com

[T12] Kotlin：解构声明
来源：http://fkz.zhengqikj.top

val (a, b) = Pair(1, 2)
来源：http://tzt.kuanghao11.cn

[T13] Kotlin：只读 Map
来源：http://kzv.aizwys.cn

val m = mapOf("a" to 1)
来源：http://tpv.zhongyouzk.top

[T14] Kotlin：循环
来源：http://fwt.jiagoushi.top

for (i in 1..10) println(i)
来源：http://fru.chenzaomai.com

[T15] Kotlin：接口
来源：http://usy.kuanghao11.cn

interface Shape { fun area(): Double }
来源：http://sdy.tarul.cn

[T16] Swift：Hello World
来源：http://myh.sweek.top

print("Hello")
来源：http://osx.sxryk.cn

[T17] Swift：变量与常量
来源：http://kad.yj20258888.top

var a = 1;  let b = 2
来源：http://nqa.yangfankeji.com

[T18] Swift：字符串插值
来源：http://sos.ehwqpu.com

"值: \(b)"
来源：http://zot.bjfxy.top

[T19] Swift：可选绑定
来源：http://eks.quarkkingdee.top

if let n = opt { print(n) }
来源：http://ltb.dashuyun.cn

[T20] Swift：数组操作
来源：http://kng.hywenlv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://svy.ctjpmb.com

[T21] Swift：遍历
来源：http://vkr.jlsjyb.cn

for x in a { print(x) }
来源：http://sgq.shzxlz.cn

[T22] Swift：字典
来源：http://mrs.zhaomingkeji.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://zsa.ywan-chungtsiang.top

[T23] Swift：函数
来源：http://uni.yj20258.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bpv.yuanzhike.top

[T24] Swift：闭包
来源：http://ehh.tarul.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fbn.sjlbkw.cn

[T25] Swift：结构体
来源：http://vnl.vehdjk.com

struct P { var x: Int }
来源：http://guq.pengpengdd.cyou

[T26] Swift：类与重写
来源：http://ydk.snrcjt.cn

class A: Base { override func f() {} }
来源：http://vhv.nanxinkj.top

[T27] Swift：错误处理
来源：http://yfo.yueranfly.top

do { try f() } catch { print(error) }
来源：http://bzx.hcnkem.com

[T28] Swift：枚举
来源：http://vke.daria6918.cn

enum Color { case red, green }
来源：http://oxg.mhx1999.top

[T29] Swift：guard 提前返回
来源：http://vfj.chenzaomai.com

guard let x = opt else { return }
来源：http://rgo.hammf.cn

[T30] Swift：协议
来源：http://qtt.jlsjyb.cn

protocol Shape { func area() -> Double }
来源：http://zya.zhengqikj.top

[T31] Lua：Hello World
来源：http://kel.jlsjyb.cn

print("Hello")
来源：http://ujt.yvedp.cn

[T32] Lua：局部变量
来源：http://aqj.xingfuxueyuan.xyz

local a = 1
来源：http://zrg.svipenyu.cn

[T33] Lua：表（数组）
来源：http://zxp.yj20258888.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ixm.gaohongyu789.top

[T34] Lua：遍历表
来源：http://gki.shuidangran.top

for i, v in ipairs(t) do print(i, v) end
来源：http://zzd.ydzc1.top

[T35] Lua：字典表
来源：http://qig.hesvh.cn

local d = { a = 1 };  d.b = 2
来源：http://nqf.haohaochexian.top

[T36] Lua：函数
来源：http://tcm.zhoulong.xyz

function add(a, b) return a + b end
来源：http://tcr.xinyue.icu

[T37] Lua：字符串拼接
来源：http://oyr.ybcxt.top

"a" .. "b"
来源：http://mra.cheryme.top

[T38] Lua：条件
来源：http://nld.snrcjt.cn

if x > 0 then print("正") end
来源：http://ycp.feifeiyinyue.top

[T39] Lua：模式匹配
来源：http://wtv.xingfuxueyuan.xyz

string.find(s, "%d+")
来源：http://bfn.dianchejie.cn

[T40] Lua：元表
来源：http://dvo.ybcxt.top

setmetatable({}, { __index = base })
来源：http://pug.shangyingyoupin.top

[T41] Perl：Hello World
来源：http://drb.jiagoushi.top

print "Hello\n";
来源：http://rfi.yonumen.top

[T42] Perl：变量类型
来源：http://lsj.sysykeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://czm.quarkkingdee.top

[T43] Perl：字符串插值
来源：http://ajn.gogol.net.cn

"值: $a"
来源：http://ogs.hesvh.cn

[T44] Perl：条件
来源：http://noc.sweek.top

if ($a > 0) { print "正"; }
来源：http://cyi.sxryk.cn

[T45] Perl：数组遍历
来源：http://mwp.snrcjt.cn

for my $x (@arr) { print $x; }
来源：http://npv.jyoumei.cn

[T46] Perl：哈希操作
来源：http://qzi.tianlin.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://scv.jinyuanbaomall.cn

[T47] Perl：正则捕获
来源：http://fcq.kuanghao11.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ifh.tianlin.xyz

[T48] Perl：正则替换
来源：http://gyu.yuanzhike.top

$s =~ s/old/new/g;
来源：http://zhy.hongshengwenyu.top

[T49] Perl：函数
来源：http://eoo.hesvh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tjr.yuxming.cn

[T50] Perl：逐行读文件
来源：http://wpd.zhaomingkeji.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://fuq.vehdjk.com

while (my $line = <$fh>) { print $line; }
来源：http://zpc.xinyue.icu

[T51] Scala：Hello World
来源：http://npo.andypj.xyz

println("Hello")
来源：http://wps.sufxvd.cn

[T52] Scala：变量
来源：http://eyf.andypj.xyz

val a = 1;  var b = 2
来源：http://lah.dianchejie.cn

[T53] Scala：字符串插值
来源：http://ehz.yongpay.top

s"值: $b"
来源：http://ciq.dashuyun.cn

[T54] Scala：集合映射
来源：http://xey.pengpengdd.cyou

List(1, 2, 3).map(_ * 2)
来源：http://lux.ivvv.top

[T55] Scala：集合过滤
来源：http://oyq.bjfxy.top

List(1, 2, 3).filter(_ > 1)
来源：http://mei.zhongyouzk.top

[T56] Scala：样例类
来源：http://cuv.haohaochexian.top

case class User(name: String, age: Int)
来源：http://mpy.zhaomingkeji.xyz

[T57] Scala：模式匹配
来源：http://evr.zhongyouzk.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://sdo.zhoulong.xyz

[T58] Scala：函数定义
来源：http://oex.dashuyun.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qck.aizwys.cn

[T59] Scala：循环
来源：http://wqr.tian-w.cn

for (i <- 1 to 10) println(i)
来源：http://mak.ywan-chungtsiang.top

[T60] Scala：折叠
来源：http://job.jqgfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://usa.xuanzx.com

================================================================================
来源：http://xtf.ctjpmb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qle.gaohongyu789.top

================================================================================
来源：http://ybu.tianlin.xyz

[U01] Py：创建虚拟环境
来源：http://ptv.zhengqikj.top

python -m venv .venv && source .venv/bin/activate
来源：http://qrd.zycfv.cn

[U02] Py：导出 / 安装依赖
来源：http://znk.jqgufenzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ycx.fengsongda.top

[U03] Py：加载 .env 配置
来源：http://fji.havefunace.top

from dotenv import load_dotenv; load_dotenv()
来源：http://med.jinqigufen.top

[U04] Py：变量调试打印
来源：http://ysc.dianchejie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gld.aizwys.cn

[U05] Py：列表去重且保序
来源：http://ujd.quarkkingdee.top

list(dict.fromkeys(arr))
来源：http://jnn.aizwys.cn

[U06] Py：合并两个字典
来源：http://myi.pycfn.com

{**a, **b}
来源：http://kjq.gaohongyu789.top

[U07] Py：反转字典键值
来源：http://rya.yuxming.cn

{v: k for k, v in d.items()}
来源：http://vme.xziqi.cn

[U08] Py：展平二维列表
来源：http://oji.52xcode.cn

[y for x in nested for y in x]
来源：http://nvn.0kj1m.cn

[U09] Py：字典取最大值的键
来源：http://mev.fzhhl.top

max(d, key=d.get)
来源：http://sdm.gotoacloud.top

[U10] Py：按值排序字典
来源：http://lia.haohaochexian.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kjb.tian-w.cn

[U11] Py：生成器表达式
来源：http://gva.pengpengdd.cyou

(x * 2 for x in arr)
来源：http://isk.sysykeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://dep.kuanghao11.cn

Counter(arr).most_common(3)
来源：http://igy.haohaochexian.top

[U13] Py：固定长度队列
来源：http://olf.fzhhl.top

deque(maxlen=10)
来源：http://ccn.ybcxt.top

[U14] Py：分组收集到列表
来源：http://qql.xuetiantiany.cn

defaultdict(list)
来源：http://fpe.shanyushiyangtech.top

[U15] Py：高精度计时
来源：http://gxa.yfazqb.com

t = time.perf_counter()
来源：http://jzz.nanxuanxn.top

[U16] Py：命令行参数解析
来源：http://owg.pengpengdd.cyou

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pwu.shanyushiyangkeji.top

[U17] Py：初始化日志
来源：http://zqm.daria6918.cn

logging.basicConfig(level=logging.INFO)
来源：http://zfr.smart0.xyz

[U18] Py：预编译正则
来源：http://fhk.svipenyu.cn

pat = re.compile(r"\d+")
来源：http://juv.daxiang520.top

[U19] Py：正则替换带回调
来源：http://hzt.hcnkem.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dxy.jyoumei.cn

[U20] Py：缓存函数结果
来源：http://mtr.yj20258.top

@functools.lru_cache(maxsize=None)
来源：http://xcr.mhx1999.top

[U21] Py：自定义上下文管理器
来源：http://kxt.yj202588.top

@contextlib.contextmanager
来源：http://rsw.hnxiangtu.top

[U22] Py：矩阵转置
来源：http://qzn.yongpay.top

list(zip(*m))
来源：http://qry.fzhhl.top

[U23] Py：分块读取大文件
来源：http://jcd.quarkkingdee.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pph.yongpay.top

[U24] Py：路径操作
来源：http://wjs.sweek.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jph.fanxiaobao.xyz

[U25] Py：CSV 按字典读
来源：http://kqm.haohaochexian.top

csv.DictReader(f)
来源：http://vgg.316326.xyz

[U26] Py：并发下载
来源：http://hil.tanke756.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eee.ydzc1.top

[U27] Py：异步 HTTP
来源：http://pyj.hnqzz.top

aiohttp.ClientSession() 配合 async with
来源：http://jmp.quarkkingdee.top

[U28] Py：类型别名
来源：http://byn.hesvh.cn

UserId = int
来源：http://phz.hfpthk.cn

[U29] Py：属性校验
来源：http://vlq.xylfe.cn

@property 与 @x.setter 配合
来源：http://pqe.fehbvm.com

[U30] Py：数据类
来源：http://mjs.zhixingplan.top

@dataclass(slots=True)
来源：http://jqh.zhiwuduotai.top

[U31] Py：单测
来源：http://hjx.yonumen.top

python -m pytest -q
来源：http://xea.cdnleiting.top

[U32] Py：代码格式化
来源：http://nkd.bbcook.cn

ruff format . && ruff check --fix .
来源：http://lkb.iojbl.cn

[U33] Py：打包发布
来源：http://fdq.sysykeji.top

python -m build  （依赖 pyproject.toml）
来源：http://bkk.sxryk.cn

[U34] Py：判断编码
来源：http://fiy.uphjek.com

chardet.detect(raw)
来源：http://jjz.gogol.net.cn

[U35] Py：发送邮件
来源：http://ueg.chenzaomai.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lhn.jianghu66.top

[U36] Py：定时任务
来源：http://uex.hnqzz.top

schedule.every(10).minutes.do(job)
来源：http://rum.bbcook.cn

[U37] Py：读写 Excel
来源：http://nfa.zhijiandao.cn

pandas.read_excel / DataFrame.to_excel
来源：http://njm.hnxiangtu.top

[U38] Py：获取脚本所在目录
来源：http://mmd.yj20258888.top

Path(__file__).resolve().parent
来源：http://ckg.zhiwuduotai.top

[U39] Py：判断是否在交互环境
来源：http://uyu.yonumen.top

sys.stdout.isatty()
来源：http://lrp.yj20258.top

[U40] Py：打印到标准错误
来源：http://mqy.sjlbkw.cn

print("err", file=sys.stderr)
来源：http://fxz.guannengcc.top

[U41] PHP：初始化 Composer 项目
来源：http://vhp.fanxiaobao.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://ulf.jinyuanbaomall.cn

[U42] PHP：PSR-4 自动加载
来源：http://zvl.zhoulong.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qxh.tanke756.top

[U43] PHP：声明命名空间
来源：http://gal.ctjpmb.com

namespace App\Http;
来源：http://qgo.zycfv.cn

[U44] PHP：开启严格类型
来源：http://fxn.shuidangran.top

declare(strict_types=1);
来源：http://mxp.uphjek.com

[U45] PHP：类型声明与返回类型
来源：http://vrr.sweek.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://gqi.zhaomingkeji.xyz

[U46] PHP：可空类型
来源：http://ywe.zhaomingkeji.xyz

?string $name = null
来源：http://sxi.sweek.top

[U47] PHP：联合类型
来源：http://dzr.zhaomingkeji.xyz

int|string $id
来源：http://gqw.sxryk.cn

[U48] PHP：纯枚举
来源：http://wft.sysykeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fbw.cdnleiting.top

[U49] PHP：只读属性
来源：http://hjd.gotoacloud.top

public readonly string $name
来源：http://kle.mhx1999.top

[U50] PHP：构造器属性提升
来源：http://zop.pycfn.com

public function __construct(private int $id) {}
来源：http://lig.snrcjt.cn

[U51] PHP：数组解构
来源：http://pwh.tanke756.top

[$a, $b] = $arr;
来源：http://mdp.ehwqpu.com

[U52] PHP：箭头函数
来源：http://ubv.meibo888.top

$double = fn($x) => $x * 2;
来源：http://rgt.redwolf501.top

[U53] PHP：空合并运算符
来源：http://oeh.ivvv.top

$v = $a ?? $b ?? "default";
来源：http://crc.fengsongda.top

[U54] PHP：空安全调用
来源：http://fpf.jqgfzy.top

$obj?->method()
来源：http://bvv.xuetiantiany.cn

[U55] PHP：match 表达式
来源：http://cxp.ybcxt.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sot.sufxvd.cn

[U56] PHP：命名参数
来源：http://tit.9152youxi.cn

f(a: 1, b: 2)
来源：http://xbp.tarul.cn

[U57] PHP：字符串插值
来源：http://bxi.feifeiyinyue.top

"值: {$a}"
来源：http://tlu.jinqigufen.top

[U58] PHP：数组三件套
来源：http://iqd.mhx1999.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tcr.jinghuilouyu.cn

[U59] PHP：自定义排序
来源：http://dcl.meibo888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zzj.xylfe.cn

[U60] PHP：JSON 编解码
来源：http://xjd.sweek.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kix.316326.xyz

[U61] PHP：正则
来源：http://xsu.hywenlv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://brh.iojbl.cn

[U62] PHP：日期对象
来源：http://qar.yuanzhike.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vpa.shangyingyoupin.top

[U63] PHP：文件读写
来源：http://als.fengsongda.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://brn.hysaishi.cn

[U64] PHP：目录遍历
来源：http://snw.yuxming.cn

glob("dir/*.php");  scandir("dir");
来源：http://kzw.shzxlz.cn

[U65] PHP：会话
来源：http://ymz.bbcook.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kez.ppjwa.cn

[U66] PHP：设置 Cookie
来源：http://jho.hysaishi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vdj.sysykeji.top

[U67] PHP：处理文件上传
来源：http://dvu.chenlongwang.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tcq.shangyingyoupin.top

[U68] PHP：PDO 连接
来源：http://tta.hywenlv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rlp.zhiwuduotai.top

[U69] PHP：PDO 预处理
来源：http://ijs.ivvv.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yoy.cdnleiting.top

[U70] PHP：PDO 事务
来源：http://qxv.xuanzx.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mzy.shzxlz.cn

[U71] PHP：抛出异常
来源：http://xjz.sysykeji.top

throw new RuntimeException("失败", 500);
来源：http://top.haohaochexian.top

[U72] PHP：写错误日志
来源：http://aoh.xingfuxueyuan.xyz

error_log("失败: " . $e->getMessage());
来源：http://bmc.yueranfly.top

[U73] PHP：读取 ini 配置
来源：http://yzx.wangshuangyany.cn

parse_ini_file("config.ini", true)
来源：http://oyk.chenzaomai.com

[U74] PHP：读取环境变量
来源：http://woj.sxryk.cn

getenv("APP_ENV") ?: "production"
来源：http://zcg.tian-w.cn

[U75] PHP：依赖注入
来源：http://oau.shuidangran.top

composer require psr/container
来源：http://kun.fehbvm.com

[U76] PHP：简单路由
来源：http://ail.zhixingplan.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mvh.chenjidiqi.icu

[U77] PHP：模板渲染
来源：http://njq.jianghu66.top

composer require twig/twig
来源：http://idt.uphjek.com

[U78] PHP：单元测试
来源：http://ett.hesvh.cn

composer require --dev phpunit/phpunit
来源：http://hdi.sufxvd.cn

[U79] PHP：静态分析
来源：http://gbf.ydzc1.top

composer require --dev phpstan/phpstan
来源：http://fmy.quarkkingdee.top

[U80] PHP：代码规范修复
来源：http://taw.ydzc1.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://clt.xziqi.cn

[U81] JS：初始化项目
来源：http://ccv.zhixingplan.top

npm init -y;  npm i express
来源：http://nne.haohaochexian.top

[U82] JS：package.json 脚本
来源：http://akf.yueranfly.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jaa.jinqigufen.top

[U83] JS：ES Module 导入导出
来源：http://yef.sweek.top

export const a = 1;  import { a } from "./m.js";
来源：http://qkf.sufxvd.cn

[U84] JS：CommonJS 写法
来源：http://yie.hnxiangtu.top

module.exports = { a };  const { a } = require("./m");
来源：http://mbb.havefunace.top


<!-- 参考信息 -->