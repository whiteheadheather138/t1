代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sjp.iojbl.cn

[S57] C++：编译期常量
来源：http://xvr.kuanghao11.cn

constexpr int N = 10;
来源：http://dzn.svipenyu.cn

[S58] C++：命名空间
来源：http://bap.jqgufenzy.top

namespace ns { int f() { return 1; } }
来源：http://kfy.ivvv.top

[S59] C++：静态断言
来源：http://mfb.52xcode.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jqn.shangyingyoupin.top

[S60] C++：遍历并删除元素
来源：http://cqj.gogol.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cnn.sxryk.cn

================================================================================
来源：http://ogq.kuanghao11.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://atf.yj20258888.top

================================================================================
来源：http://eku.yongpay.top

[T01] Kotlin：Hello World
来源：http://eou.sjlbkw.cn

println("Hello")
来源：http://iqc.tian-w.cn

[T02] Kotlin：变量
来源：http://skx.fanxiaobao.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iuc.ybcxt.top

[T03] Kotlin：字符串模板
来源：http://dys.jinqigfzy.top

"值: $b"
来源：http://als.ydzc1.top

[T04] Kotlin：空安全
来源：http://jep.shzxlz.cn

val n: String? = null;  n?.length
来源：http://klp.jlsjyb.cn

[T05] Kotlin：when 表达式
来源：http://bgr.jianghu66.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fdb.sweek.top

[T06] Kotlin：集合映射
来源：http://dqq.jiagoushi.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rfm.iojbl.cn

[T07] Kotlin：集合过滤
来源：http://vwj.cucudq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ars.zhongyouzk.top

[T08] Kotlin：数据类
来源：http://uzm.zycfv.cn

data class User(val name: String, val age: Int)
来源：http://iwa.hesvh.cn

[T09] Kotlin：扩展函数
来源：http://xvf.ywan-chungtsiang.top

fun String.exclaim() = this + "!"
来源：http://xeo.wangdashe.top

[T10] Kotlin：默认参数
来源：http://fjh.vehdjk.com

fun greet(name: String = "World") = "Hi $name"
来源：http://pkb.jianghu66.top

[T11] Kotlin：协程
来源：http://ibw.fengsongda.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://pyb.zhoulong.xyz

[T12] Kotlin：解构声明
来源：http://nzn.zhiwuduotai.top

val (a, b) = Pair(1, 2)
来源：http://abk.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://hvg.zdbjq.cn

val m = mapOf("a" to 1)
来源：http://osy.yj202588.top

[T14] Kotlin：循环
来源：http://srz.hnxiangtu.top

for (i in 1..10) println(i)
来源：http://cqy.uphjek.com

[T15] Kotlin：接口
来源：http://gag.ydzc1.top

interface Shape { fun area(): Double }
来源：http://vof.gaohongyu789.top

[T16] Swift：Hello World
来源：http://pfa.gogol.net.cn

print("Hello")
来源：http://nlg.sjlbkw.cn

[T17] Swift：变量与常量
来源：http://yik.mhx1999.top

var a = 1;  let b = 2
来源：http://hdg.bjfxy.top

[T18] Swift：字符串插值
来源：http://gkp.cucudq.cn

"值: \(b)"
来源：http://gqe.zhoulong.xyz

[T19] Swift：可选绑定
来源：http://poo.chenjidiqi.icu

if let n = opt { print(n) }
来源：http://clm.zhijiandao.cn

[T20] Swift：数组操作
来源：http://iet.yj202588.top

var a = [1, 2, 3];  a.append(4)
来源：http://zzf.vehdjk.com

[T21] Swift：遍历
来源：http://rdn.chenjidiqi.icu

for x in a { print(x) }
来源：http://bfd.zhijiandao.cn

[T22] Swift：字典
来源：http://qcq.cucudq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://iml.hcnkem.com

[T23] Swift：函数
来源：http://cgr.xylfe.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://abm.daxiang520.top

[T24] Swift：闭包
来源：http://wex.epnwcf.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://ova.jinqigufen.top

[T25] Swift：结构体
来源：http://ksn.wangshuangyany.cn

struct P { var x: Int }
来源：http://uoh.jinyuanbaomall.cn

[T26] Swift：类与重写
来源：http://nlv.dashuyun.cn

class A: Base { override func f() {} }
来源：http://qpf.ivvv.top

[T27] Swift：错误处理
来源：http://jso.mhx1999.top

do { try f() } catch { print(error) }
来源：http://tuy.hywenlv.cn

[T28] Swift：枚举
来源：http://hmh.yonumen.top

enum Color { case red, green }
来源：http://pbo.dianchejie.cn

[T29] Swift：guard 提前返回
来源：http://ygg.gogol.net.cn

guard let x = opt else { return }
来源：http://bhh.gzhubu.top

[T30] Swift：协议
来源：http://icd.c1oappe.top

protocol Shape { func area() -> Double }
来源：http://uwv.shanyushiyangkeji.top

[T31] Lua：Hello World
来源：http://pxm.gaohongyu789.top

print("Hello")
来源：http://uzw.fktsv.cn

[T32] Lua：局部变量
来源：http://ytl.shangyingyoupin.top

local a = 1
来源：http://gtw.tianlin.xyz

[T33] Lua：表（数组）
来源：http://udp.yueranfly.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xtc.pycfn.com

[T34] Lua：遍历表
来源：http://hlq.hammf.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://adu.chenzaomai.com

[T35] Lua：字典表
来源：http://uzv.mhx1999.top

local d = { a = 1 };  d.b = 2
来源：http://xxw.zhijiandao.cn

[T36] Lua：函数
来源：http://hge.chenzaomai.com

function add(a, b) return a + b end
来源：http://edv.fktsv.cn

[T37] Lua：字符串拼接
来源：http://zgi.sweek.top

"a" .. "b"
来源：http://aaa.snrcjt.cn

[T38] Lua：条件
来源：http://wvw.zhixingplan.top

if x > 0 then print("正") end
来源：http://ccj.gogol.net.cn

[T39] Lua：模式匹配
来源：http://ytz.ywan-chungtsiang.top

string.find(s, "%d+")
来源：http://lwo.sxryk.cn

[T40] Lua：元表
来源：http://ujp.yj20258888.top

setmetatable({}, { __index = base })
来源：http://dqt.daxiang520.top

[T41] Perl：Hello World
来源：http://jpv.cheryme.top

print "Hello\n";
来源：http://mtz.zycfv.cn

[T42] Perl：变量类型
来源：http://umi.yj202588.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wtf.birdmap.top

[T43] Perl：字符串插值
来源：http://hwb.vqdsnc.cn

"值: $a"
来源：http://qah.gogol.net.cn

[T44] Perl：条件
来源：http://oir.kuanghao11.cn

if ($a > 0) { print "正"; }
来源：http://dgl.zdqjudy.top

[T45] Perl：数组遍历
来源：http://ahp.jlsjyb.cn

for my $x (@arr) { print $x; }
来源：http://pvf.ybcxt.top

[T46] Perl：哈希操作
来源：http://lrk.fktsv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://weu.nwbrower.top

[T47] Perl：正则捕获
来源：http://rhu.cheryme.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vkt.ydjk.org.cn

[T48] Perl：正则替换
来源：http://ywq.jqgufenzy.top

$s =~ s/old/new/g;
来源：http://atj.tanke756.top

[T49] Perl：函数
来源：http://ack.jyoumei.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qde.quarkkingdee.top

[T50] Perl：逐行读文件
来源：http://rqy.shanyushiyangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hzy.9152youxi.cn

while (my $line = <$fh>) { print $line; }
来源：http://ccj.jinghuilouyu.cn

[T51] Scala：Hello World
来源：http://dad.bbcook.cn

println("Hello")
来源：http://ouq.xylfe.cn

[T52] Scala：变量
来源：http://chl.jlsjyb.cn

val a = 1;  var b = 2
来源：http://pxi.hammf.cn

[T53] Scala：字符串插值
来源：http://obe.xingfuxueyuan.xyz

s"值: $b"
来源：http://cdg.feifeiyinyue.top

[T54] Scala：集合映射
来源：http://thn.yanxiufei.cn

List(1, 2, 3).map(_ * 2)
来源：http://qen.shzxlz.cn

[T55] Scala：集合过滤
来源：http://mjs.shuidangran.top

List(1, 2, 3).filter(_ > 1)
来源：http://ayn.zdbjq.cn

[T56] Scala：样例类
来源：http://yqy.c1oappe.top

case class User(name: String, age: Int)
来源：http://azb.gaohongyu789.top

[T57] Scala：模式匹配
来源：http://cyt.cashguo.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gog.shzxlz.cn

[T58] Scala：函数定义
来源：http://zio.c1oappe.top

def add(a: Int, b: Int): Int = a + b
来源：http://qbn.dashuyun.cn

[T59] Scala：循环
来源：http://pis.vqdsnc.cn

for (i <- 1 to 10) println(i)
来源：http://air.shanyushiyangkeji.top

[T60] Scala：折叠
来源：http://ecu.pengpengdd.cyou

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fvp.xziqi.cn

================================================================================
来源：http://pfe.guannengcc.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cyh.snrcjt.cn

================================================================================
来源：http://ysg.yonumen.top

[U01] Py：创建虚拟环境
来源：http://rxu.mhx1999.top

python -m venv .venv && source .venv/bin/activate
来源：http://vyy.gzhubu.top

[U02] Py：导出 / 安装依赖
来源：http://pcg.jinyuanbaomall.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tgh.52xcode.cn

[U03] Py：加载 .env 配置
来源：http://qls.zhijiandao.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qsx.pengpengdd.cyou

[U04] Py：变量调试打印
来源：http://apx.zhijiandao.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rwg.tian-w.cn

[U05] Py：列表去重且保序
来源：http://ksc.vqdsnc.cn

list(dict.fromkeys(arr))
来源：http://mcr.gaohongyu789.top

[U06] Py：合并两个字典
来源：http://mvq.snrcjt.cn

{**a, **b}
来源：http://zxx.vqdsnc.cn

[U07] Py：反转字典键值
来源：http://rin.hfpthk.cn

{v: k for k, v in d.items()}
来源：http://tqn.havefunace.top

[U08] Py：展平二维列表
来源：http://osh.jiagoushi.top

[y for x in nested for y in x]
来源：http://usa.yangfankeji.com

[U09] Py：字典取最大值的键
来源：http://wic.ehwqpu.com

max(d, key=d.get)
来源：http://lfe.hfpthk.cn

[U10] Py：按值排序字典
来源：http://yrk.havefunace.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qpf.jinyuanbaomall.cn

[U11] Py：生成器表达式
来源：http://oeq.ydjk.org.cn

(x * 2 for x in arr)
来源：http://lkc.zdqjudy.top

[U12] Py：取出现最多的 3 个元素
来源：http://pck.birdmap.top

Counter(arr).most_common(3)
来源：http://yej.dashuyun.cn

[U13] Py：固定长度队列
来源：http://hhi.vehdjk.com

deque(maxlen=10)
来源：http://jxl.gogol.net.cn

[U14] Py：分组收集到列表
来源：http://mlt.cqqwz.cn

defaultdict(list)
来源：http://xqy.tianlin.xyz

[U15] Py：高精度计时
来源：http://flv.ivvv.top

t = time.perf_counter()
来源：http://kug.vehdjk.com

[U16] Py：命令行参数解析
来源：http://mie.kuanghao11.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jay.tianlin.xyz

[U17] Py：初始化日志
来源：http://knk.feifeiyinyue.top

logging.basicConfig(level=logging.INFO)
来源：http://env.xylfe.cn

[U18] Py：预编译正则
来源：http://fvb.vqdsnc.cn

pat = re.compile(r"\d+")
来源：http://pbh.yj202588.top

[U19] Py：正则替换带回调
来源：http://deb.snrcjt.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hts.zdqjudy.top

[U20] Py：缓存函数结果
来源：http://deh.fzhhl.top

@functools.lru_cache(maxsize=None)
来源：http://ves.316326.xyz

[U21] Py：自定义上下文管理器
来源：http://pbm.aibaodan.cn

@contextlib.contextmanager
来源：http://awg.ctjpmb.com

[U22] Py：矩阵转置
来源：http://hhy.dashuyun.cn

list(zip(*m))
来源：http://akl.jinyuanbaomall.cn

[U23] Py：分块读取大文件
来源：http://doz.sysykeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xpz.cdnleiting.top

[U24] Py：路径操作
来源：http://sns.fanxiaobao.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dnj.cheryme.top

[U25] Py：CSV 按字典读
来源：http://mxh.ppjwa.cn

csv.DictReader(f)
来源：http://zud.zhiwuduotai.top

[U26] Py：并发下载
来源：http://fxd.aizwys.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wlo.ivvv.top

[U27] Py：异步 HTTP
来源：http://xyy.bbcook.cn

aiohttp.ClientSession() 配合 async with
来源：http://psi.sjlbkw.cn

[U28] Py：类型别名
来源：http://utn.jinghuilouyu.cn

UserId = int
来源：http://phj.xuanzx.com

[U29] Py：属性校验
来源：http://tpx.yonumen.top

@property 与 @x.setter 配合
来源：http://fis.redwolf501.top

[U30] Py：数据类
来源：http://rwo.ehwqpu.com

@dataclass(slots=True)
来源：http://qof.hammf.cn

[U31] Py：单测
来源：http://tvs.aibaodan.cn

python -m pytest -q
来源：http://ajv.chenzaomai.com

[U32] Py：代码格式化
来源：http://obk.jqgufenzy.top

ruff format . && ruff check --fix .
来源：http://acz.tian-w.cn

[U33] Py：打包发布
来源：http://piw.ctjpmb.com

python -m build  （依赖 pyproject.toml）
来源：http://fyn.chenjidiqi.icu

[U34] Py：判断编码
来源：http://job.tianlin.xyz

chardet.detect(raw)
来源：http://pxv.shuidangran.top

[U35] Py：发送邮件
来源：http://swx.hnqzz.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://spn.yj202588.top

[U36] Py：定时任务
来源：http://pax.gotoacloud.top

schedule.every(10).minutes.do(job)
来源：http://ckq.yongpay.top

[U37] Py：读写 Excel
来源：http://rjw.jinyuanbaomall.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nvg.sweek.top

[U38] Py：获取脚本所在目录
来源：http://eiv.c1oappe.top

Path(__file__).resolve().parent
来源：http://ksj.shuidangran.top

[U39] Py：判断是否在交互环境
来源：http://njd.ybcxt.top

sys.stdout.isatty()
来源：http://hjs.hammf.cn

[U40] Py：打印到标准错误
来源：http://ypt.sjlbkw.cn

print("err", file=sys.stderr)
来源：http://hwi.tian-w.cn

[U41] PHP：初始化 Composer 项目
来源：http://qaf.nwbrower.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wkf.guowangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://fxc.kuanghao11.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://efg.hfpthk.cn

[U43] PHP：声明命名空间
来源：http://lrh.cashguo.top

namespace App\Http;
来源：http://aaq.jyoumei.cn

[U44] PHP：开启严格类型
来源：http://nel.fehbvm.com

declare(strict_types=1);
来源：http://eqh.yj20258888.top

[U45] PHP：类型声明与返回类型
来源：http://dkf.gzhubu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vsb.hywenlv.cn

[U46] PHP：可空类型
来源：http://bue.jqgfzy.top

?string $name = null
来源：http://wxy.tarul.cn

[U47] PHP：联合类型
来源：http://bdd.hcnkem.com

int|string $id
来源：http://isw.chenlongwang.top

[U48] PHP：纯枚举
来源：http://jar.iojbl.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://drk.birdmap.top

[U49] PHP：只读属性
来源：http://gfy.yuanzhike.top

public readonly string $name
来源：http://ejg.smart0.xyz

[U50] PHP：构造器属性提升
来源：http://wzt.smart0.xyz

public function __construct(private int $id) {}
来源：http://kjr.xinyue.icu

[U51] PHP：数组解构
来源：http://zaa.tianlin.xyz

[$a, $b] = $arr;
来源：http://udk.yonumen.top

[U52] PHP：箭头函数
来源：http://voz.jianghu66.top

$double = fn($x) => $x * 2;
来源：http://czf.daria6918.cn

[U53] PHP：空合并运算符
来源：http://dhr.xziqi.cn

$v = $a ?? $b ?? "default";
来源：http://qia.daria6918.cn

[U54] PHP：空安全调用
来源：http://qgp.shanyushiyangtech.top

$obj?->method()
来源：http://zta.dianchejie.cn

[U55] PHP：match 表达式
来源：http://vdm.jqgufenzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hys.wangshuangyany.cn

[U56] PHP：命名参数
来源：http://vqe.sufxvd.cn

f(a: 1, b: 2)
来源：http://mhs.fktsv.cn

[U57] PHP：字符串插值
来源：http://upl.tanke756.top

"值: {$a}"
来源：http://ugo.sjlbkw.cn

[U58] PHP：数组三件套
来源：http://evq.fktsv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://oxe.52xcode.cn

[U59] PHP：自定义排序
来源：http://odo.jqgufenzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zix.xuanzx.com

[U60] PHP：JSON 编解码
来源：http://qeb.cqqwz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bdz.hnqzz.top

[U61] PHP：正则
来源：http://dmk.sufxvd.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vcs.daria6918.cn

[U62] PHP：日期对象
来源：http://dtg.xingfuxueyuan.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gke.xuanzx.com

[U63] PHP：文件读写
来源：http://agv.nwbrower.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qhu.pycfn.com

[U64] PHP：目录遍历
来源：http://nug.fengsongda.top

glob("dir/*.php");  scandir("dir");
来源：http://vpm.ywan-chungtsiang.top

[U65] PHP：会话
来源：http://kvk.tanke756.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ycv.pycfn.com

[U66] PHP：设置 Cookie
来源：http://hsh.haohaochexian.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jvr.yj20258.top

[U67] PHP：处理文件上传
来源：http://wpy.zdqjudy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ugb.aizwys.cn

[U68] PHP：PDO 连接
来源：http://dfm.yuanzhike.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pvs.hywenlv.cn

[U69] PHP：PDO 预处理
来源：http://emq.sjlbkw.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://osd.bjfxy.top

[U70] PHP：PDO 事务
来源：http://hax.ivvv.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bdg.guowangkeji.top

[U71] PHP：抛出异常
来源：http://hek.tarul.cn

throw new RuntimeException("失败", 500);
来源：http://rzf.hfpthk.cn

[U72] PHP：写错误日志
来源：http://buj.ybcxt.top

error_log("失败: " . $e->getMessage());
来源：http://ujs.yueranfly.top

[U73] PHP：读取 ini 配置
来源：http://gfl.zhiwuduotai.top

parse_ini_file("config.ini", true)
来源：http://iec.0kj1m.cn

[U74] PHP：读取环境变量
来源：http://atd.316326.xyz

getenv("APP_ENV") ?: "production"
来源：http://hre.hfpthk.cn

[U75] PHP：依赖注入
来源：http://vza.zhaomingkeji.xyz

composer require psr/container
来源：http://kmf.yangfankeji.com

[U76] PHP：简单路由
来源：http://sbi.hcnkem.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pvt.chenjidiqi.icu

[U77] PHP：模板渲染
来源：http://ogz.hysaishi.cn

composer require twig/twig
来源：http://cun.ybcxt.top

[U78] PHP：单元测试
来源：http://mcz.yangfankeji.com

composer require --dev phpunit/phpunit
来源：http://tlu.feifeiyinyue.top

[U79] PHP：静态分析
来源：http://jhx.sxryk.cn

composer require --dev phpstan/phpstan
来源：http://ziu.birdmap.top

[U80] PHP：代码规范修复
来源：http://xoy.zycfv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gfv.vqdsnc.cn

[U81] JS：初始化项目
来源：http://stu.wangshuangyany.cn

npm init -y;  npm i express
来源：http://dwy.hcnkem.com

[U82] JS：package.json 脚本
来源：http://hix.xziqi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ebl.chenjidiqi.icu


<!-- 参考信息 -->