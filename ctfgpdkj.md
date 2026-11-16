代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cww.316326.xyz

[S57] C++：编译期常量
来源：http://vst.dashuyun.cn

constexpr int N = 10;
来源：http://kui.zhixingplan.top

[S58] C++：命名空间
来源：http://pck.bbcook.cn

namespace ns { int f() { return 1; } }
来源：http://nbs.shanyushiyangkeji.top

[S59] C++：静态断言
来源：http://exq.tanke756.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fls.xuanzx.com

[S60] C++：遍历并删除元素
来源：http://ncv.hywenlv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://khs.dashuyun.cn

================================================================================
来源：http://him.wangshuangyany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uzb.zhengqikj.top

================================================================================
来源：http://lxg.zdbjq.cn

[T01] Kotlin：Hello World
来源：http://ztn.zycfv.cn

println("Hello")
来源：http://jeu.ydzc1.top

[T02] Kotlin：变量
来源：http://gmc.havefunace.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://evt.wangdashe.top

[T03] Kotlin：字符串模板
来源：http://dfk.smart0.xyz

"值: $b"
来源：http://lbd.xuetiantiany.cn

[T04] Kotlin：空安全
来源：http://lkn.meibo888.top

val n: String? = null;  n?.length
来源：http://jsb.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://lgt.sjlbkw.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://scs.xuetiantiany.cn

[T06] Kotlin：集合映射
来源：http://biz.zhiwuduotai.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zjy.xingfuxueyuan.xyz

[T07] Kotlin：集合过滤
来源：http://evi.havefunace.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://heb.yfazqb.com

[T08] Kotlin：数据类
来源：http://emh.gotoacloud.top

data class User(val name: String, val age: Int)
来源：http://kyq.cqqwz.cn

[T09] Kotlin：扩展函数
来源：http://rgk.yvedp.cn

fun String.exclaim() = this + "!"
来源：http://erz.ydjk.org.cn

[T10] Kotlin：默认参数
来源：http://bkb.andypj.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://syu.tanke756.top

[T11] Kotlin：协程
来源：http://cai.0kj1m.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xxk.xuetiantiany.cn

[T12] Kotlin：解构声明
来源：http://cwh.0kj1m.cn

val (a, b) = Pair(1, 2)
来源：http://bzr.sxryk.cn

[T13] Kotlin：只读 Map
来源：http://lnd.9152youxi.cn

val m = mapOf("a" to 1)
来源：http://hoj.zhixingplan.top

[T14] Kotlin：循环
来源：http://pxt.jqgufenzy.top

for (i in 1..10) println(i)
来源：http://hmm.tian-w.cn

[T15] Kotlin：接口
来源：http://ssr.xuanzx.com

interface Shape { fun area(): Double }
来源：http://xwz.gaohongyu789.top

[T16] Swift：Hello World
来源：http://pnu.gaohongyu789.top

print("Hello")
来源：http://guo.sysykeji.top

[T17] Swift：变量与常量
来源：http://eei.daxiang520.top

var a = 1;  let b = 2
来源：http://oaz.sxryk.cn

[T18] Swift：字符串插值
来源：http://cal.ydjk.org.cn

"值: \(b)"
来源：http://eak.tanke756.top

[T19] Swift：可选绑定
来源：http://qxv.ppjwa.cn

if let n = opt { print(n) }
来源：http://duu.c1oappe.top

[T20] Swift：数组操作
来源：http://mpf.shanyushiyangtech.top

var a = [1, 2, 3];  a.append(4)
来源：http://mch.ydzc1.top

[T21] Swift：遍历
来源：http://yrl.birdmap.top

for x in a { print(x) }
来源：http://twm.sxryk.cn

[T22] Swift：字典
来源：http://hdc.guowangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://ser.guannengcc.top

[T23] Swift：函数
来源：http://qyh.feifeiyinyue.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zti.jinyuanbaomall.cn

[T24] Swift：闭包
来源：http://cfj.jlsjyb.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ngj.sjlbkw.cn

[T25] Swift：结构体
来源：http://cpd.hammf.cn

struct P { var x: Int }
来源：http://hnl.52xcode.cn

[T26] Swift：类与重写
来源：http://kgl.meibo888.top

class A: Base { override func f() {} }
来源：http://ijw.guowangkeji.top

[T27] Swift：错误处理
来源：http://seh.bjfxy.top

do { try f() } catch { print(error) }
来源：http://xrc.jqgufenzy.top

[T28] Swift：枚举
来源：http://tdh.guowangkeji.top

enum Color { case red, green }
来源：http://cny.guowangkeji.top

[T29] Swift：guard 提前返回
来源：http://qbr.redwolf501.top

guard let x = opt else { return }
来源：http://rbk.cdnleiting.top

[T30] Swift：协议
来源：http://efm.iojbl.cn

protocol Shape { func area() -> Double }
来源：http://blx.fktsv.cn

[T31] Lua：Hello World
来源：http://xqf.zhijiandao.cn

print("Hello")
来源：http://don.xuetiantiany.cn

[T32] Lua：局部变量
来源：http://uff.yueranfly.top

local a = 1
来源：http://ask.hongshengwenyu.top

[T33] Lua：表（数组）
来源：http://dqd.dashuyun.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://upe.chenjidiqi.icu

[T34] Lua：遍历表
来源：http://tsv.yongpay.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qrw.sysykeji.top

[T35] Lua：字典表
来源：http://bhk.c1oappe.top

local d = { a = 1 };  d.b = 2
来源：http://llt.cucudq.cn

[T36] Lua：函数
来源：http://hma.guowangkeji.top

function add(a, b) return a + b end
来源：http://srk.zhaomingkeji.xyz

[T37] Lua：字符串拼接
来源：http://gbm.yfazqb.com

"a" .. "b"
来源：http://gic.yj202588.top

[T38] Lua：条件
来源：http://cgo.c1oappe.top

if x > 0 then print("正") end
来源：http://odc.gzhubu.top

[T39] Lua：模式匹配
来源：http://bvu.shanyushiyangkeji.top

string.find(s, "%d+")
来源：http://uxx.feifeiyinyue.top

[T40] Lua：元表
来源：http://rvs.jinqigufen.top

setmetatable({}, { __index = base })
来源：http://qbn.fktsv.cn

[T41] Perl：Hello World
来源：http://qqr.yanxiufei.cn

print "Hello\n";
来源：http://fms.bbcook.cn

[T42] Perl：变量类型
来源：http://hhe.yuxming.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ctn.guannengcc.top

[T43] Perl：字符串插值
来源：http://kkg.jianghu66.top

"值: $a"
来源：http://ykv.xuanzx.com

[T44] Perl：条件
来源：http://pvm.chenjidiqi.icu

if ($a > 0) { print "正"; }
来源：http://ncz.jinqigfzy.top

[T45] Perl：数组遍历
来源：http://vkn.wangdashe.top

for my $x (@arr) { print $x; }
来源：http://kbu.yj20258.top

[T46] Perl：哈希操作
来源：http://sae.sufxvd.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zgv.aibaodan.cn

[T47] Perl：正则捕获
来源：http://gqx.ctjpmb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://stn.nanxuanxn.top

[T48] Perl：正则替换
来源：http://ksh.yuanzhike.top

$s =~ s/old/new/g;
来源：http://krk.sweek.top

[T49] Perl：函数
来源：http://pjs.316326.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hly.hongshengwenyu.top

[T50] Perl：逐行读文件
来源：http://txw.yuxming.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://boj.chenjidiqi.icu

while (my $line = <$fh>) { print $line; }
来源：http://gvs.hnxiangtu.top

[T51] Scala：Hello World
来源：http://thb.aizwys.cn

println("Hello")
来源：http://ptu.tarul.cn

[T52] Scala：变量
来源：http://uqf.fehbvm.com

val a = 1;  var b = 2
来源：http://wki.havefunace.top

[T53] Scala：字符串插值
来源：http://ehi.aibaodan.cn

s"值: $b"
来源：http://yjf.xziqi.cn

[T54] Scala：集合映射
来源：http://woc.jinghuilouyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://wbv.yongpay.top

[T55] Scala：集合过滤
来源：http://for.yuxming.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ezn.fehbvm.com

[T56] Scala：样例类
来源：http://gjm.nanxinkj.top

case class User(name: String, age: Int)
来源：http://pbi.smart0.xyz

[T57] Scala：模式匹配
来源：http://pga.quarkkingdee.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ene.hesvh.cn

[T58] Scala：函数定义
来源：http://uty.havefunace.top

def add(a: Int, b: Int): Int = a + b
来源：http://ouy.yueranfly.top

[T59] Scala：循环
来源：http://thy.birdmap.top

for (i <- 1 to 10) println(i)
来源：http://duo.aibaodan.cn

[T60] Scala：折叠
来源：http://nnh.ivvv.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ifh.ybcxt.top

================================================================================
来源：http://ilp.cucudq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dlh.sweek.top

================================================================================
来源：http://ipb.ppjwa.cn

[U01] Py：创建虚拟环境
来源：http://wze.nanxuanxn.top

python -m venv .venv && source .venv/bin/activate
来源：http://mvw.xuanzx.com

[U02] Py：导出 / 安装依赖
来源：http://mjs.ybcxt.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qao.guowangkeji.top

[U03] Py：加载 .env 配置
来源：http://dyw.ivvv.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wgu.xuanzx.com

[U04] Py：变量调试打印
来源：http://bie.hcnkem.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oia.sufxvd.cn

[U05] Py：列表去重且保序
来源：http://kar.xuetiantiany.cn

list(dict.fromkeys(arr))
来源：http://ldl.hcnkem.com

[U06] Py：合并两个字典
来源：http://jlw.zdbjq.cn

{**a, **b}
来源：http://wht.sjlbkw.cn

[U07] Py：反转字典键值
来源：http://ius.wangdashe.top

{v: k for k, v in d.items()}
来源：http://kyt.pycfn.com

[U08] Py：展平二维列表
来源：http://zkm.yvedp.cn

[y for x in nested for y in x]
来源：http://wdk.tarul.cn

[U09] Py：字典取最大值的键
来源：http://zzl.zhoulong.xyz

max(d, key=d.get)
来源：http://fyc.ydzc1.top

[U10] Py：按值排序字典
来源：http://heh.cashguo.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rhl.fengsongda.top

[U11] Py：生成器表达式
来源：http://fdd.quarkkingdee.top

(x * 2 for x in arr)
来源：http://mae.cashguo.top

[U12] Py：取出现最多的 3 个元素
来源：http://bhe.tian-w.cn

Counter(arr).most_common(3)
来源：http://jvd.c1oappe.top

[U13] Py：固定长度队列
来源：http://dzl.pengpengdd.cyou

deque(maxlen=10)
来源：http://uop.jqgufenzy.top

[U14] Py：分组收集到列表
来源：http://czc.yj202588.top

defaultdict(list)
来源：http://cau.sysykeji.top

[U15] Py：高精度计时
来源：http://wux.cheryme.top

t = time.perf_counter()
来源：http://ssl.meibo888.top

[U16] Py：命令行参数解析
来源：http://ask.jinyuanbaomall.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bce.vehdjk.com

[U17] Py：初始化日志
来源：http://tnn.hnqzz.top

logging.basicConfig(level=logging.INFO)
来源：http://btt.xziqi.cn

[U18] Py：预编译正则
来源：http://tcc.svipenyu.cn

pat = re.compile(r"\d+")
来源：http://zac.316326.xyz

[U19] Py：正则替换带回调
来源：http://nvg.yj20258888.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wub.pengpengdd.cyou

[U20] Py：缓存函数结果
来源：http://lsf.ivvv.top

@functools.lru_cache(maxsize=None)
来源：http://uoh.wangshuangyany.cn

[U21] Py：自定义上下文管理器
来源：http://vge.snrcjt.cn

@contextlib.contextmanager
来源：http://hem.cashguo.top

[U22] Py：矩阵转置
来源：http://fqe.guannengcc.top

list(zip(*m))
来源：http://vfr.havefunace.top

[U23] Py：分块读取大文件
来源：http://oyi.ivvv.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hsp.snrcjt.cn

[U24] Py：路径操作
来源：http://nbt.zhaomingkeji.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cal.haohaochexian.top

[U25] Py：CSV 按字典读
来源：http://sov.haohaochexian.top

csv.DictReader(f)
来源：http://qsn.tianlin.xyz

[U26] Py：并发下载
来源：http://efx.fehbvm.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jtq.c1oappe.top

[U27] Py：异步 HTTP
来源：http://max.ybcxt.top

aiohttp.ClientSession() 配合 async with
来源：http://fyu.yj20258.top

[U28] Py：类型别名
来源：http://skz.yj202588.top

UserId = int
来源：http://cpx.yuxming.cn

[U29] Py：属性校验
来源：http://got.epnwcf.com

@property 与 @x.setter 配合
来源：http://pve.feifeiyinyue.top

[U30] Py：数据类
来源：http://dhh.wangshuangyany.cn

@dataclass(slots=True)
来源：http://xse.zhaomingkeji.xyz

[U31] Py：单测
来源：http://eam.gotoacloud.top

python -m pytest -q
来源：http://gnt.fktsv.cn

[U32] Py：代码格式化
来源：http://avh.ydjk.org.cn

ruff format . && ruff check --fix .
来源：http://meb.cqqwz.cn

[U33] Py：打包发布
来源：http://gpe.pycfn.com

python -m build  （依赖 pyproject.toml）
来源：http://kly.hywenlv.cn

[U34] Py：判断编码
来源：http://nhx.zdqjudy.top

chardet.detect(raw)
来源：http://cda.jqgfzy.top

[U35] Py：发送邮件
来源：http://btk.gaohongyu789.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nys.jyoumei.cn

[U36] Py：定时任务
来源：http://ejd.yuxming.cn

schedule.every(10).minutes.do(job)
来源：http://adp.tianlin.xyz

[U37] Py：读写 Excel
来源：http://qfz.zhaomingkeji.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://vwk.52xcode.cn

[U38] Py：获取脚本所在目录
来源：http://uoo.52xcode.cn

Path(__file__).resolve().parent
来源：http://ahb.cdnleiting.top

[U39] Py：判断是否在交互环境
来源：http://ebd.shanyushiyangtech.top

sys.stdout.isatty()
来源：http://oea.zhongyouzk.top

[U40] Py：打印到标准错误
来源：http://ttu.zhiwuduotai.top

print("err", file=sys.stderr)
来源：http://jek.hongshengwenyu.top

[U41] PHP：初始化 Composer 项目
来源：http://dxs.gotoacloud.top

composer init;  composer require guzzlehttp/guzzle
来源：http://dyg.mhx1999.top

[U42] PHP：PSR-4 自动加载
来源：http://jqh.chenjidiqi.icu

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rzu.epnwcf.com

[U43] PHP：声明命名空间
来源：http://jjo.jinghuilouyu.cn

namespace App\Http;
来源：http://sxm.jinqigfzy.top

[U44] PHP：开启严格类型
来源：http://vhs.aibaodan.cn

declare(strict_types=1);
来源：http://eun.ybcxt.top

[U45] PHP：类型声明与返回类型
来源：http://kcp.yj20258888.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pru.ydzc1.top

[U46] PHP：可空类型
来源：http://ndm.jinqigfzy.top

?string $name = null
来源：http://ppm.cashguo.top

[U47] PHP：联合类型
来源：http://eru.gzhubu.top

int|string $id
来源：http://sbc.bbcook.cn

[U48] PHP：纯枚举
来源：http://htz.ydzc1.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://anc.ctjpmb.com

[U49] PHP：只读属性
来源：http://jbq.vqdsnc.cn

public readonly string $name
来源：http://gpd.ppjwa.cn

[U50] PHP：构造器属性提升
来源：http://fww.haohaochexian.top

public function __construct(private int $id) {}
来源：http://zdy.pengpengdd.cyou

[U51] PHP：数组解构
来源：http://zdx.mhx1999.top

[$a, $b] = $arr;
来源：http://sjc.shanyushiyangkeji.top

[U52] PHP：箭头函数
来源：http://zjb.hysaishi.cn

$double = fn($x) => $x * 2;
来源：http://seo.aizwys.cn

[U53] PHP：空合并运算符
来源：http://sxy.jiagoushi.top

$v = $a ?? $b ?? "default";
来源：http://hml.zhaomingkeji.xyz

[U54] PHP：空安全调用
来源：http://imv.zhixingplan.top

$obj?->method()
来源：http://arf.epnwcf.com

[U55] PHP：match 表达式
来源：http://ftr.cashguo.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mcl.meibo888.top

[U56] PHP：命名参数
来源：http://kla.tianlin.xyz

f(a: 1, b: 2)
来源：http://fxh.hongshengwenyu.top

[U57] PHP：字符串插值
来源：http://axl.svipenyu.cn

"值: {$a}"
来源：http://tdc.jinqigufen.top

[U58] PHP：数组三件套
来源：http://jee.yongpay.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dtq.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://imz.cashguo.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hqe.ywan-chungtsiang.top

[U60] PHP：JSON 编解码
来源：http://hro.ydjk.org.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jcm.snrcjt.cn

[U61] PHP：正则
来源：http://kbt.tian-w.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://aal.shanyushiyangkeji.top

[U62] PHP：日期对象
来源：http://cvd.hysaishi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vug.yueranfly.top

[U63] PHP：文件读写
来源：http://djk.ydzc1.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ejm.cashguo.top

[U64] PHP：目录遍历
来源：http://xtw.haohaochexian.top

glob("dir/*.php");  scandir("dir");
来源：http://pso.epnwcf.com

[U65] PHP：会话
来源：http://qoi.ybcxt.top

session_start();  $_SESSION["uid"] = 1;
来源：http://sji.ctjpmb.com

[U66] PHP：设置 Cookie
来源：http://vrh.zhaomingkeji.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zer.jqgfzy.top

[U67] PHP：处理文件上传
来源：http://ugk.xuanzx.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://avz.0kj1m.cn

[U68] PHP：PDO 连接
来源：http://aaw.birdmap.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xxo.bjfxy.top

[U69] PHP：PDO 预处理
来源：http://dus.cqqwz.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zrr.tian-w.cn

[U70] PHP：PDO 事务
来源：http://ukx.pycfn.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kqe.ydzc1.top

[U71] PHP：抛出异常
来源：http://jti.zhijiandao.cn

throw new RuntimeException("失败", 500);
来源：http://fvb.feifeiyinyue.top

[U72] PHP：写错误日志
来源：http://xbi.xinyue.icu

error_log("失败: " . $e->getMessage());
来源：http://fyr.jinqigufen.top

[U73] PHP：读取 ini 配置
来源：http://pbp.dashuyun.cn

parse_ini_file("config.ini", true)
来源：http://ypx.jinyuanbaomall.cn

[U74] PHP：读取环境变量
来源：http://ohi.gogol.net.cn

getenv("APP_ENV") ?: "production"
来源：http://upg.bjfxy.top

[U75] PHP：依赖注入
来源：http://ptq.ybcxt.top

composer require psr/container
来源：http://emk.jinghuilouyu.cn

[U76] PHP：简单路由
来源：http://kko.hysaishi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ibd.haohaochexian.top

[U77] PHP：模板渲染
来源：http://qer.jqgufenzy.top

composer require twig/twig
来源：http://uwk.ctjpmb.com

[U78] PHP：单元测试
来源：http://flh.xziqi.cn

composer require --dev phpunit/phpunit
来源：http://wwi.ydzc1.top

[U79] PHP：静态分析
来源：http://llr.sweek.top

composer require --dev phpstan/phpstan
来源：http://azd.yangfankeji.com

[U80] PHP：代码规范修复
来源：http://qct.jinqigfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://gsy.dianchejie.cn

[U81] JS：初始化项目
来源：http://tsn.gzhubu.top

npm init -y;  npm i express
来源：http://cfb.wangshuangyany.cn

[U82] JS：package.json 脚本
来源：http://qwx.nanxinkj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cro.ydzc1.top


<!-- 参考信息 -->