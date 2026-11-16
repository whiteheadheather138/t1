代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://wbp.nwbrower.top

[S59] C++：静态断言
来源：http://opl.yongpay.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ydm.zycfv.cn

[S60] C++：遍历并删除元素
来源：http://emi.yj20258.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dwu.uphjek.com

================================================================================
来源：http://oke.sysykeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ztc.yongpay.top

================================================================================
来源：http://uoz.zhaomingkeji.xyz

[T01] Kotlin：Hello World
来源：http://olb.vqdsnc.cn

println("Hello")
来源：http://ftx.nanxuanxn.top

[T02] Kotlin：变量
来源：http://tvx.aizwys.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jro.havefunace.top

[T03] Kotlin：字符串模板
来源：http://gdk.vehdjk.com

"值: $b"
来源：http://dxm.guannengcc.top

[T04] Kotlin：空安全
来源：http://psp.jqgufenzy.top

val n: String? = null;  n?.length
来源：http://hzf.jinghuilouyu.cn

[T05] Kotlin：when 表达式
来源：http://kba.daria6918.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nkj.zhoulong.xyz

[T06] Kotlin：集合映射
来源：http://ghk.pycfn.com

listOf(1, 2, 3).map { it * 2 }
来源：http://vrb.chenzaomai.com

[T07] Kotlin：集合过滤
来源：http://wji.xziqi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cze.smart0.xyz

[T08] Kotlin：数据类
来源：http://wpa.nanxinkj.top

data class User(val name: String, val age: Int)
来源：http://tav.nanxinkj.top

[T09] Kotlin：扩展函数
来源：http://uqw.fanxiaobao.xyz

fun String.exclaim() = this + "!"
来源：http://ezp.wangdashe.top

[T10] Kotlin：默认参数
来源：http://hdw.shanyushiyangtech.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xib.bbcook.cn

[T11] Kotlin：协程
来源：http://mid.uphjek.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://dns.mhx1999.top

[T12] Kotlin：解构声明
来源：http://nwd.hesvh.cn

val (a, b) = Pair(1, 2)
来源：http://jjm.pycfn.com

[T13] Kotlin：只读 Map
来源：http://hzx.shuidangran.top

val m = mapOf("a" to 1)
来源：http://npe.fzhhl.top

[T14] Kotlin：循环
来源：http://guq.gotoacloud.top

for (i in 1..10) println(i)
来源：http://shd.ydzc1.top

[T15] Kotlin：接口
来源：http://bpp.aibaodan.cn

interface Shape { fun area(): Double }
来源：http://xql.ybcxt.top

[T16] Swift：Hello World
来源：http://kib.chenzaomai.com

print("Hello")
来源：http://dcg.9152youxi.cn

[T17] Swift：变量与常量
来源：http://zal.jqgufenzy.top

var a = 1;  let b = 2
来源：http://oxl.feifeiyinyue.top

[T18] Swift：字符串插值
来源：http://ari.hcnkem.com

"值: \(b)"
来源：http://joj.316326.xyz

[T19] Swift：可选绑定
来源：http://ydz.birdmap.top

if let n = opt { print(n) }
来源：http://rwp.jinqigfzy.top

[T20] Swift：数组操作
来源：http://wmv.ywan-chungtsiang.top

var a = [1, 2, 3];  a.append(4)
来源：http://tdo.wangshuangyany.cn

[T21] Swift：遍历
来源：http://scq.9152youxi.cn

for x in a { print(x) }
来源：http://zqt.jinqigfzy.top

[T22] Swift：字典
来源：http://ofn.fengsongda.top

var d = ["a": 1];  d["b"] = 2
来源：http://dtd.quarkkingdee.top

[T23] Swift：函数
来源：http://qzr.hfpthk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uqw.jinqigfzy.top

[T24] Swift：闭包
来源：http://rsd.jinqigufen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mnv.fktsv.cn

[T25] Swift：结构体
来源：http://qty.shanyushiyangkeji.top

struct P { var x: Int }
来源：http://ayo.zhoulong.xyz

[T26] Swift：类与重写
来源：http://mpu.yanxiufei.cn

class A: Base { override func f() {} }
来源：http://skz.jqgufenzy.top

[T27] Swift：错误处理
来源：http://gju.mhx1999.top

do { try f() } catch { print(error) }
来源：http://xab.feifeiyinyue.top

[T28] Swift：枚举
来源：http://njp.52xcode.cn

enum Color { case red, green }
来源：http://zff.pengpengdd.cyou

[T29] Swift：guard 提前返回
来源：http://pyz.wangdashe.top

guard let x = opt else { return }
来源：http://hlv.jqgfzy.top

[T30] Swift：协议
来源：http://tlo.zdbjq.cn

protocol Shape { func area() -> Double }
来源：http://jti.wangdashe.top

[T31] Lua：Hello World
来源：http://let.redwolf501.top

print("Hello")
来源：http://aec.haohaochexian.top

[T32] Lua：局部变量
来源：http://iho.yueranfly.top

local a = 1
来源：http://lnt.316326.xyz

[T33] Lua：表（数组）
来源：http://tug.xziqi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wpc.hywenlv.cn

[T34] Lua：遍历表
来源：http://amd.52xcode.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mpq.uphjek.com

[T35] Lua：字典表
来源：http://xef.zhiwuduotai.top

local d = { a = 1 };  d.b = 2
来源：http://zkw.jianghu66.top

[T36] Lua：函数
来源：http://vej.shuidangran.top

function add(a, b) return a + b end
来源：http://lul.daria6918.cn

[T37] Lua：字符串拼接
来源：http://uvg.havefunace.top

"a" .. "b"
来源：http://fhq.sysykeji.top

[T38] Lua：条件
来源：http://vkk.jinyuanbaomall.cn

if x > 0 then print("正") end
来源：http://esq.yongpay.top

[T39] Lua：模式匹配
来源：http://qxw.tarul.cn

string.find(s, "%d+")
来源：http://wpv.xylfe.cn

[T40] Lua：元表
来源：http://ggp.haohaochexian.top

setmetatable({}, { __index = base })
来源：http://zme.cashguo.top

[T41] Perl：Hello World
来源：http://cnx.c1oappe.top

print "Hello\n";
来源：http://avy.shanyushiyangtech.top

[T42] Perl：变量类型
来源：http://jnm.yfazqb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cqp.ydjk.org.cn

[T43] Perl：字符串插值
来源：http://dmb.ybcxt.top

"值: $a"
来源：http://enh.nanxinkj.top

[T44] Perl：条件
来源：http://gew.aizwys.cn

if ($a > 0) { print "正"; }
来源：http://zms.jinqigfzy.top

[T45] Perl：数组遍历
来源：http://eyg.yuanzhike.top

for my $x (@arr) { print $x; }
来源：http://uiv.tarul.cn

[T46] Perl：哈希操作
来源：http://xcl.gogol.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://acs.zhongyouzk.top

[T47] Perl：正则捕获
来源：http://vyp.jinghuilouyu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://uzg.jinghuilouyu.cn

[T48] Perl：正则替换
来源：http://mcg.hfpthk.cn

$s =~ s/old/new/g;
来源：http://dsm.cheryme.top

[T49] Perl：函数
来源：http://naq.fanxiaobao.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xcv.ybcxt.top

[T50] Perl：逐行读文件
来源：http://qrk.andypj.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://ioy.yj20258.top

while (my $line = <$fh>) { print $line; }
来源：http://bia.smart0.xyz

[T51] Scala：Hello World
来源：http://rkz.zhongyouzk.top

println("Hello")
来源：http://msb.yuanzhike.top

[T52] Scala：变量
来源：http://cab.zhongyouzk.top

val a = 1;  var b = 2
来源：http://egz.xinyue.icu

[T53] Scala：字符串插值
来源：http://mnu.ywan-chungtsiang.top

s"值: $b"
来源：http://baj.fehbvm.com

[T54] Scala：集合映射
来源：http://wfj.aibaodan.cn

List(1, 2, 3).map(_ * 2)
来源：http://wwg.ywan-chungtsiang.top

[T55] Scala：集合过滤
来源：http://hfs.vehdjk.com

List(1, 2, 3).filter(_ > 1)
来源：http://zyl.kuanghao11.cn

[T56] Scala：样例类
来源：http://utp.fengsongda.top

case class User(name: String, age: Int)
来源：http://htv.zycfv.cn

[T57] Scala：模式匹配
来源：http://tjv.havefunace.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gra.zhongyouzk.top

[T58] Scala：函数定义
来源：http://lpt.zhijiandao.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kqq.wangdashe.top

[T59] Scala：循环
来源：http://paq.xinyue.icu

for (i <- 1 to 10) println(i)
来源：http://njg.nanxinkj.top

[T60] Scala：折叠
来源：http://jvx.yj20258888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://drc.dianchejie.cn

================================================================================
来源：http://hmg.shuidangran.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zzu.shuidangran.top

================================================================================
来源：http://bur.smart0.xyz

[U01] Py：创建虚拟环境
来源：http://fat.feifeiyinyue.top

python -m venv .venv && source .venv/bin/activate
来源：http://kcs.zycfv.cn

[U02] Py：导出 / 安装依赖
来源：http://gea.tianlin.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xys.316326.xyz

[U03] Py：加载 .env 配置
来源：http://rgb.zhixingplan.top

from dotenv import load_dotenv; load_dotenv()
来源：http://rnr.svipenyu.cn

[U04] Py：变量调试打印
来源：http://rgm.9152youxi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://iml.meibo888.top

[U05] Py：列表去重且保序
来源：http://ide.hcnkem.com

list(dict.fromkeys(arr))
来源：http://cps.tarul.cn

[U06] Py：合并两个字典
来源：http://rah.ydjk.org.cn

{**a, **b}
来源：http://cjm.wangshuangyany.cn

[U07] Py：反转字典键值
来源：http://whp.hywenlv.cn

{v: k for k, v in d.items()}
来源：http://keo.yuanzhike.top

[U08] Py：展平二维列表
来源：http://kso.mhx1999.top

[y for x in nested for y in x]
来源：http://flo.ybcxt.top

[U09] Py：字典取最大值的键
来源：http://fdb.jinqigufen.top

max(d, key=d.get)
来源：http://lwt.sxryk.cn

[U10] Py：按值排序字典
来源：http://ckm.tanke756.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fcm.sysykeji.top

[U11] Py：生成器表达式
来源：http://qvv.jianghu66.top

(x * 2 for x in arr)
来源：http://asn.yfazqb.com

[U12] Py：取出现最多的 3 个元素
来源：http://tss.fanxiaobao.xyz

Counter(arr).most_common(3)
来源：http://uzk.tarul.cn

[U13] Py：固定长度队列
来源：http://wcr.yangfankeji.com

deque(maxlen=10)
来源：http://zhy.chenjidiqi.icu

[U14] Py：分组收集到列表
来源：http://xgg.guannengcc.top

defaultdict(list)
来源：http://cgh.havefunace.top

[U15] Py：高精度计时
来源：http://myd.ppjwa.cn

t = time.perf_counter()
来源：http://agg.guannengcc.top

[U16] Py：命令行参数解析
来源：http://wwx.zycfv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wxc.ppjwa.cn

[U17] Py：初始化日志
来源：http://tqb.xuetiantiany.cn

logging.basicConfig(level=logging.INFO)
来源：http://nbf.yuanzhike.top

[U18] Py：预编译正则
来源：http://jlm.andypj.xyz

pat = re.compile(r"\d+")
来源：http://rvl.0kj1m.cn

[U19] Py：正则替换带回调
来源：http://zwg.zdbjq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jmz.0kj1m.cn

[U20] Py：缓存函数结果
来源：http://sqk.fanxiaobao.xyz

@functools.lru_cache(maxsize=None)
来源：http://jgx.jiagoushi.top

[U21] Py：自定义上下文管理器
来源：http://zoh.zhijiandao.cn

@contextlib.contextmanager
来源：http://tiy.shzxlz.cn

[U22] Py：矩阵转置
来源：http://oib.andypj.xyz

list(zip(*m))
来源：http://bnz.yj202588.top

[U23] Py：分块读取大文件
来源：http://oou.ctjpmb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://udw.zhiwuduotai.top

[U24] Py：路径操作
来源：http://gbq.c1oappe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lls.ivvv.top

[U25] Py：CSV 按字典读
来源：http://xwn.jianghu66.top

csv.DictReader(f)
来源：http://yng.jlsjyb.cn

[U26] Py：并发下载
来源：http://hex.sufxvd.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hih.fanxiaobao.xyz

[U27] Py：异步 HTTP
来源：http://tck.zdqjudy.top

aiohttp.ClientSession() 配合 async with
来源：http://sqs.ctjpmb.com

[U28] Py：类型别名
来源：http://qko.gzhubu.top

UserId = int
来源：http://npp.gotoacloud.top

[U29] Py：属性校验
来源：http://apg.hongshengwenyu.top

@property 与 @x.setter 配合
来源：http://uyi.jqgufenzy.top

[U30] Py：数据类
来源：http://wmc.yj202588.top

@dataclass(slots=True)
来源：http://ood.sxryk.cn

[U31] Py：单测
来源：http://btq.shangyingyoupin.top

python -m pytest -q
来源：http://arz.hammf.cn

[U32] Py：代码格式化
来源：http://yax.daria6918.cn

ruff format . && ruff check --fix .
来源：http://mtg.jqgufenzy.top

[U33] Py：打包发布
来源：http://hrf.iojbl.cn

python -m build  （依赖 pyproject.toml）
来源：http://uhm.bjfxy.top

[U34] Py：判断编码
来源：http://tbh.fktsv.cn

chardet.detect(raw)
来源：http://tve.jinqigufen.top

[U35] Py：发送邮件
来源：http://vdc.redwolf501.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yhn.sjlbkw.cn

[U36] Py：定时任务
来源：http://onp.andypj.xyz

schedule.every(10).minutes.do(job)
来源：http://mjh.sxryk.cn

[U37] Py：读写 Excel
来源：http://aue.ctjpmb.com

pandas.read_excel / DataFrame.to_excel
来源：http://bij.zdqjudy.top

[U38] Py：获取脚本所在目录
来源：http://trx.chenzaomai.com

Path(__file__).resolve().parent
来源：http://uum.redwolf501.top

[U39] Py：判断是否在交互环境
来源：http://bbq.jqgfzy.top

sys.stdout.isatty()
来源：http://isr.fanxiaobao.xyz

[U40] Py：打印到标准错误
来源：http://diu.cqqwz.cn

print("err", file=sys.stderr)
来源：http://vob.yanxiufei.cn

[U41] PHP：初始化 Composer 项目
来源：http://gmz.bbcook.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yid.yj202588.top

[U42] PHP：PSR-4 自动加载
来源：http://vps.yanxiufei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ipw.guannengcc.top

[U43] PHP：声明命名空间
来源：http://djr.xziqi.cn

namespace App\Http;
来源：http://jiq.ydzc1.top

[U44] PHP：开启严格类型
来源：http://ggi.jiagoushi.top

declare(strict_types=1);
来源：http://mdf.sxryk.cn

[U45] PHP：类型声明与返回类型
来源：http://fdm.tanke756.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://dcf.jinqigfzy.top

[U46] PHP：可空类型
来源：http://nkg.jiagoushi.top

?string $name = null
来源：http://vif.jqgufenzy.top

[U47] PHP：联合类型
来源：http://zdr.zhixingplan.top

int|string $id
来源：http://idf.yueranfly.top

[U48] PHP：纯枚举
来源：http://ems.ywan-chungtsiang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sjm.yongpay.top

[U49] PHP：只读属性
来源：http://yao.cdnleiting.top

public readonly string $name
来源：http://uzc.ivvv.top

[U50] PHP：构造器属性提升
来源：http://blw.kuanghao11.cn

public function __construct(private int $id) {}
来源：http://wny.shangyingyoupin.top

[U51] PHP：数组解构
来源：http://wxu.xinyue.icu

[$a, $b] = $arr;
来源：http://lmd.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://kjp.52xcode.cn

$double = fn($x) => $x * 2;
来源：http://joh.nanxinkj.top

[U53] PHP：空合并运算符
来源：http://lyv.chenlongwang.top

$v = $a ?? $b ?? "default";
来源：http://vtp.zdqjudy.top

[U54] PHP：空安全调用
来源：http://aof.tianlin.xyz

$obj?->method()
来源：http://yjp.ybcxt.top

[U55] PHP：match 表达式
来源：http://vla.haohaochexian.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gbg.pengpengdd.cyou

[U56] PHP：命名参数
来源：http://myr.fktsv.cn

f(a: 1, b: 2)
来源：http://krc.kuanghao11.cn

[U57] PHP：字符串插值
来源：http://xxj.chenjidiqi.icu

"值: {$a}"
来源：http://qdv.tanke756.top

[U58] PHP：数组三件套
来源：http://ujt.9152youxi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dir.sysykeji.top

[U59] PHP：自定义排序
来源：http://ycx.bbcook.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://quv.daxiang520.top

[U60] PHP：JSON 编解码
来源：http://uvl.yuxming.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gnm.iojbl.cn

[U61] PHP：正则
来源：http://eid.feifeiyinyue.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kis.fanxiaobao.xyz

[U62] PHP：日期对象
来源：http://mxb.zdbjq.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ivj.snrcjt.cn

[U63] PHP：文件读写
来源：http://srm.ywan-chungtsiang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ihz.jinqigufen.top

[U64] PHP：目录遍历
来源：http://wbe.meibo888.top

glob("dir/*.php");  scandir("dir");
来源：http://uoq.zycfv.cn

[U65] PHP：会话
来源：http://cky.zhixingplan.top

session_start();  $_SESSION["uid"] = 1;
来源：http://asa.cqqwz.cn

[U66] PHP：设置 Cookie
来源：http://fdf.c1oappe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bkp.sysykeji.top

[U67] PHP：处理文件上传
来源：http://cvu.jinqigfzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kua.yuxming.cn

[U68] PHP：PDO 连接
来源：http://ruc.zdbjq.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jqz.shanyushiyangtech.top

[U69] PHP：PDO 预处理
来源：http://hfq.xuanzx.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lnu.bbcook.cn

[U70] PHP：PDO 事务
来源：http://ivr.ivvv.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fbl.jiagoushi.top

[U71] PHP：抛出异常
来源：http://qcg.cucudq.cn

throw new RuntimeException("失败", 500);
来源：http://zei.jinghuilouyu.cn

[U72] PHP：写错误日志
来源：http://wrg.daria6918.cn

error_log("失败: " . $e->getMessage());
来源：http://jfz.jyoumei.cn

[U73] PHP：读取 ini 配置
来源：http://meh.zhongyouzk.top

parse_ini_file("config.ini", true)
来源：http://wxe.wangdashe.top

[U74] PHP：读取环境变量
来源：http://sdm.zhengqikj.top

getenv("APP_ENV") ?: "production"
来源：http://ggd.tanke756.top

[U75] PHP：依赖注入
来源：http://hgw.yanxiufei.cn

composer require psr/container
来源：http://khy.zdqjudy.top

[U76] PHP：简单路由
来源：http://xvl.shanyushiyangkeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iir.meibo888.top

[U77] PHP：模板渲染
来源：http://ctq.zhoulong.xyz

composer require twig/twig
来源：http://zos.tianlin.xyz

[U78] PHP：单元测试
来源：http://jje.epnwcf.com

composer require --dev phpunit/phpunit
来源：http://tuy.zhijiandao.cn

[U79] PHP：静态分析
来源：http://ypf.fktsv.cn

composer require --dev phpstan/phpstan
来源：http://ocy.ctjpmb.com

[U80] PHP：代码规范修复
来源：http://deq.ctjpmb.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://lgf.fengsongda.top

[U81] JS：初始化项目
来源：http://tje.cqqwz.cn

npm init -y;  npm i express
来源：http://van.ctjpmb.com

[U82] JS：package.json 脚本
来源：http://krw.shzxlz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://koj.0kj1m.cn

[U83] JS：ES Module 导入导出
来源：http://urw.zhixingplan.top

export const a = 1;  import { a } from "./m.js";
来源：http://pew.yj20258888.top

[U84] JS：CommonJS 写法
来源：http://yzv.birdmap.top

module.exports = { a };  const { a } = require("./m");
来源：http://cdk.zdbjq.cn


<!-- 参考信息 -->