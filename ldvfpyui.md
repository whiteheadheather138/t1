代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gfz.xinyue.icu

[S55] C++：结构化绑定
来源：http://mjy.pengpengdd.cyou

auto [a, b] = std::make_pair(1, 2);
来源：http://til.chenlongwang.top

[S56] C++：optional
来源：http://iya.cqqwz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uod.cheryme.top

[S57] C++：编译期常量
来源：http://shn.yuanzhike.top

constexpr int N = 10;
来源：http://wuo.shanyushiyangkeji.top

[S58] C++：命名空间
来源：http://bmn.fehbvm.com

namespace ns { int f() { return 1; } }
来源：http://lwv.gogol.net.cn

[S59] C++：静态断言
来源：http://aqd.jianghu66.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nvq.shuidangran.top

[S60] C++：遍历并删除元素
来源：http://kui.chenjidiqi.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://axj.gaohongyu789.top

================================================================================
来源：http://uqc.redwolf501.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://knk.ybcxt.top

================================================================================
来源：http://jgg.xinyue.icu

[T01] Kotlin：Hello World
来源：http://utx.jyoumei.cn

println("Hello")
来源：http://gwi.jinghuilouyu.cn

[T02] Kotlin：变量
来源：http://bjn.hammf.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rre.daxiang520.top

[T03] Kotlin：字符串模板
来源：http://dlc.chenzaomai.com

"值: $b"
来源：http://fac.chenzaomai.com

[T04] Kotlin：空安全
来源：http://czv.guannengcc.top

val n: String? = null;  n?.length
来源：http://ztu.meibo888.top

[T05] Kotlin：when 表达式
来源：http://ctg.jinghuilouyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sgj.epnwcf.com

[T06] Kotlin：集合映射
来源：http://hlg.dashuyun.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://iyn.shanyushiyangkeji.top

[T07] Kotlin：集合过滤
来源：http://gvj.andypj.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://yfp.tanke756.top

[T08] Kotlin：数据类
来源：http://mnn.zhoulong.xyz

data class User(val name: String, val age: Int)
来源：http://wda.zhengqikj.top

[T09] Kotlin：扩展函数
来源：http://skj.xingfuxueyuan.xyz

fun String.exclaim() = this + "!"
来源：http://juq.haohaochexian.top

[T10] Kotlin：默认参数
来源：http://egy.ywan-chungtsiang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qzn.ctjpmb.com

[T11] Kotlin：协程
来源：http://vie.ydjk.org.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vvt.tarul.cn

[T12] Kotlin：解构声明
来源：http://tqg.jinghuilouyu.cn

val (a, b) = Pair(1, 2)
来源：http://ppo.chenjidiqi.icu

[T13] Kotlin：只读 Map
来源：http://cme.ppjwa.cn

val m = mapOf("a" to 1)
来源：http://tob.shangyingyoupin.top

[T14] Kotlin：循环
来源：http://ueq.0kj1m.cn

for (i in 1..10) println(i)
来源：http://lmi.ehwqpu.com

[T15] Kotlin：接口
来源：http://est.yj20258888.top

interface Shape { fun area(): Double }
来源：http://tbb.jianghu66.top

[T16] Swift：Hello World
来源：http://rdi.zdbjq.cn

print("Hello")
来源：http://qor.aizwys.cn

[T17] Swift：变量与常量
来源：http://efz.nwbrower.top

var a = 1;  let b = 2
来源：http://gvz.haohaochexian.top

[T18] Swift：字符串插值
来源：http://sds.shanyushiyangkeji.top

"值: \(b)"
来源：http://kdj.jqgfzy.top

[T19] Swift：可选绑定
来源：http://rzn.yfazqb.com

if let n = opt { print(n) }
来源：http://yfa.bjfxy.top

[T20] Swift：数组操作
来源：http://edd.jinqigfzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://mhu.havefunace.top

[T21] Swift：遍历
来源：http://zgf.52xcode.cn

for x in a { print(x) }
来源：http://pzu.shanyushiyangkeji.top

[T22] Swift：字典
来源：http://veg.tanke756.top

var d = ["a": 1];  d["b"] = 2
来源：http://xqc.xingfuxueyuan.xyz

[T23] Swift：函数
来源：http://qhd.tian-w.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xio.yueranfly.top

[T24] Swift：闭包
来源：http://iun.jyoumei.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kmv.jiagoushi.top

[T25] Swift：结构体
来源：http://jjw.yj20258.top

struct P { var x: Int }
来源：http://sqy.yongpay.top

[T26] Swift：类与重写
来源：http://bqp.meibo888.top

class A: Base { override func f() {} }
来源：http://zhy.zdqjudy.top

[T27] Swift：错误处理
来源：http://vlq.316326.xyz

do { try f() } catch { print(error) }
来源：http://xwz.sufxvd.cn

[T28] Swift：枚举
来源：http://jbv.zhaomingkeji.xyz

enum Color { case red, green }
来源：http://kje.gaohongyu789.top

[T29] Swift：guard 提前返回
来源：http://jar.0kj1m.cn

guard let x = opt else { return }
来源：http://ywj.pycfn.com

[T30] Swift：协议
来源：http://ymk.xziqi.cn

protocol Shape { func area() -> Double }
来源：http://jcy.cashguo.top

[T31] Lua：Hello World
来源：http://wqg.birdmap.top

print("Hello")
来源：http://ifc.ydjk.org.cn

[T32] Lua：局部变量
来源：http://dtd.iojbl.cn

local a = 1
来源：http://nca.hnqzz.top

[T33] Lua：表（数组）
来源：http://kdx.jinqigufen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jky.zhijiandao.cn

[T34] Lua：遍历表
来源：http://yys.jlsjyb.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ghh.hammf.cn

[T35] Lua：字典表
来源：http://yzi.pycfn.com

local d = { a = 1 };  d.b = 2
来源：http://rnt.sufxvd.cn

[T36] Lua：函数
来源：http://gfk.xylfe.cn

function add(a, b) return a + b end
来源：http://jtt.jiagoushi.top

[T37] Lua：字符串拼接
来源：http://fgc.smart0.xyz

"a" .. "b"
来源：http://znb.xziqi.cn

[T38] Lua：条件
来源：http://mxz.zhixingplan.top

if x > 0 then print("正") end
来源：http://uge.uphjek.com

[T39] Lua：模式匹配
来源：http://hcv.ybcxt.top

string.find(s, "%d+")
来源：http://smg.quarkkingdee.top

[T40] Lua：元表
来源：http://kqu.iojbl.cn

setmetatable({}, { __index = base })
来源：http://mdv.c1oappe.top

[T41] Perl：Hello World
来源：http://ggd.vqdsnc.cn

print "Hello\n";
来源：http://fsp.vehdjk.com

[T42] Perl：变量类型
来源：http://bsy.hysaishi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hlg.jyoumei.cn

[T43] Perl：字符串插值
来源：http://yww.epnwcf.com

"值: $a"
来源：http://mcg.xuetiantiany.cn

[T44] Perl：条件
来源：http://thk.zdbjq.cn

if ($a > 0) { print "正"; }
来源：http://ylp.iojbl.cn

[T45] Perl：数组遍历
来源：http://cjc.smart0.xyz

for my $x (@arr) { print $x; }
来源：http://avc.bbcook.cn

[T46] Perl：哈希操作
来源：http://iez.chenzaomai.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://twb.nanxinkj.top

[T47] Perl：正则捕获
来源：http://kyk.zhiwuduotai.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://htb.gaohongyu789.top

[T48] Perl：正则替换
来源：http://hwh.nwbrower.top

$s =~ s/old/new/g;
来源：http://iiv.birdmap.top

[T49] Perl：函数
来源：http://cdf.zhongyouzk.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fan.yj202588.top

[T50] Perl：逐行读文件
来源：http://bum.quarkkingdee.top

open my $fh, "<", "a.txt" or die $!;
来源：http://cpd.shanyushiyangtech.top

while (my $line = <$fh>) { print $line; }
来源：http://gsv.gotoacloud.top

[T51] Scala：Hello World
来源：http://qxw.nanxuanxn.top

println("Hello")
来源：http://fed.xuetiantiany.cn

[T52] Scala：变量
来源：http://qhf.yuanzhike.top

val a = 1;  var b = 2
来源：http://auh.yueranfly.top

[T53] Scala：字符串插值
来源：http://nvw.ivvv.top

s"值: $b"
来源：http://tgj.bbcook.cn

[T54] Scala：集合映射
来源：http://rqp.jqgufenzy.top

List(1, 2, 3).map(_ * 2)
来源：http://dqj.zhiwuduotai.top

[T55] Scala：集合过滤
来源：http://rou.yvedp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gba.xylfe.cn

[T56] Scala：样例类
来源：http://zye.bbcook.cn

case class User(name: String, age: Int)
来源：http://whp.nanxinkj.top

[T57] Scala：模式匹配
来源：http://cbi.hfpthk.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tvb.wangshuangyany.cn

[T58] Scala：函数定义
来源：http://cfd.shanyushiyangkeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://kcz.sjlbkw.cn

[T59] Scala：循环
来源：http://upc.fengsongda.top

for (i <- 1 to 10) println(i)
来源：http://jzm.zhoulong.xyz

[T60] Scala：折叠
来源：http://riu.xingfuxueyuan.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sre.zhoulong.xyz

================================================================================
来源：http://heo.aizwys.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gce.vqdsnc.cn

================================================================================
来源：http://izr.shzxlz.cn

[U01] Py：创建虚拟环境
来源：http://mgp.jinghuilouyu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jvr.wangshuangyany.cn

[U02] Py：导出 / 安装依赖
来源：http://yth.jianghu66.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uuz.tanke756.top

[U03] Py：加载 .env 配置
来源：http://hlc.jqgfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://npe.tanke756.top

[U04] Py：变量调试打印
来源：http://svb.316326.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vkg.yj20258888.top

[U05] Py：列表去重且保序
来源：http://qsg.zhiwuduotai.top

list(dict.fromkeys(arr))
来源：http://fsd.yj202588.top

[U06] Py：合并两个字典
来源：http://ovf.ydzc1.top

{**a, **b}
来源：http://myp.uphjek.com

[U07] Py：反转字典键值
来源：http://rae.cashguo.top

{v: k for k, v in d.items()}
来源：http://apq.cdnleiting.top

[U08] Py：展平二维列表
来源：http://tnz.ppjwa.cn

[y for x in nested for y in x]
来源：http://bsw.cheryme.top

[U09] Py：字典取最大值的键
来源：http://rln.zhengqikj.top

max(d, key=d.get)
来源：http://ltb.9152youxi.cn

[U10] Py：按值排序字典
来源：http://yjj.feifeiyinyue.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://enw.svipenyu.cn

[U11] Py：生成器表达式
来源：http://rvw.hnqzz.top

(x * 2 for x in arr)
来源：http://qjx.ivvv.top

[U12] Py：取出现最多的 3 个元素
来源：http://zfc.vehdjk.com

Counter(arr).most_common(3)
来源：http://xme.guowangkeji.top

[U13] Py：固定长度队列
来源：http://bkf.jinqigfzy.top

deque(maxlen=10)
来源：http://ymu.yangfankeji.com

[U14] Py：分组收集到列表
来源：http://ecw.xinyue.icu

defaultdict(list)
来源：http://psy.meibo888.top

[U15] Py：高精度计时
来源：http://ncv.hesvh.cn

t = time.perf_counter()
来源：http://ypl.tarul.cn

[U16] Py：命令行参数解析
来源：http://wbj.yj20258.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ovj.sxryk.cn

[U17] Py：初始化日志
来源：http://qiu.dianchejie.cn

logging.basicConfig(level=logging.INFO)
来源：http://soz.yj20258.top

[U18] Py：预编译正则
来源：http://hpc.epnwcf.com

pat = re.compile(r"\d+")
来源：http://edw.cqqwz.cn

[U19] Py：正则替换带回调
来源：http://xlq.316326.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jzz.snrcjt.cn

[U20] Py：缓存函数结果
来源：http://xiw.yj20258888.top

@functools.lru_cache(maxsize=None)
来源：http://sfl.hywenlv.cn

[U21] Py：自定义上下文管理器
来源：http://obr.yj20258.top

@contextlib.contextmanager
来源：http://mjo.pycfn.com

[U22] Py：矩阵转置
来源：http://xad.ctjpmb.com

list(zip(*m))
来源：http://ltv.jyoumei.cn

[U23] Py：分块读取大文件
来源：http://vnt.yuxming.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://crz.chenzaomai.com

[U24] Py：路径操作
来源：http://nlw.chenlongwang.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vhu.zdqjudy.top

[U25] Py：CSV 按字典读
来源：http://lgu.iojbl.cn

csv.DictReader(f)
来源：http://ofz.zhongyouzk.top

[U26] Py：并发下载
来源：http://qaw.feifeiyinyue.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://onf.hysaishi.cn

[U27] Py：异步 HTTP
来源：http://tcp.hfpthk.cn

aiohttp.ClientSession() 配合 async with
来源：http://vmg.hongshengwenyu.top

[U28] Py：类型别名
来源：http://hlv.hywenlv.cn

UserId = int
来源：http://bzx.nwbrower.top

[U29] Py：属性校验
来源：http://nbp.snrcjt.cn

@property 与 @x.setter 配合
来源：http://mpo.gaohongyu789.top

[U30] Py：数据类
来源：http://qko.chenlongwang.top

@dataclass(slots=True)
来源：http://rrd.jinqigufen.top

[U31] Py：单测
来源：http://obr.ydjk.org.cn

python -m pytest -q
来源：http://kxf.tanke756.top

[U32] Py：代码格式化
来源：http://sxm.yuxming.cn

ruff format . && ruff check --fix .
来源：http://jjv.chenjidiqi.icu

[U33] Py：打包发布
来源：http://hvq.daxiang520.top

python -m build  （依赖 pyproject.toml）
来源：http://uhe.316326.xyz

[U34] Py：判断编码
来源：http://gtk.yueranfly.top

chardet.detect(raw)
来源：http://xpk.316326.xyz

[U35] Py：发送邮件
来源：http://mxq.shanyushiyangtech.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wbv.ctjpmb.com

[U36] Py：定时任务
来源：http://yvx.jinqigufen.top

schedule.every(10).minutes.do(job)
来源：http://sfw.0kj1m.cn

[U37] Py：读写 Excel
来源：http://jcs.jianghu66.top

pandas.read_excel / DataFrame.to_excel
来源：http://qpj.yongpay.top

[U38] Py：获取脚本所在目录
来源：http://fvs.xylfe.cn

Path(__file__).resolve().parent
来源：http://hcp.jianghu66.top

[U39] Py：判断是否在交互环境
来源：http://znk.fzhhl.top

sys.stdout.isatty()
来源：http://vzm.mhx1999.top

[U40] Py：打印到标准错误
来源：http://rna.jlsjyb.cn

print("err", file=sys.stderr)
来源：http://omb.hnqzz.top

[U41] PHP：初始化 Composer 项目
来源：http://ubk.birdmap.top

composer init;  composer require guzzlehttp/guzzle
来源：http://yme.nwbrower.top

[U42] PHP：PSR-4 自动加载
来源：http://xvz.zycfv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dou.zdqjudy.top

[U43] PHP：声明命名空间
来源：http://teg.haohaochexian.top

namespace App\Http;
来源：http://rrc.zdbjq.cn

[U44] PHP：开启严格类型
来源：http://eku.daria6918.cn

declare(strict_types=1);
来源：http://zmj.yvedp.cn

[U45] PHP：类型声明与返回类型
来源：http://acg.zhaomingkeji.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://rrg.hammf.cn

[U46] PHP：可空类型
来源：http://hhj.jinqigfzy.top

?string $name = null
来源：http://rdd.yangfankeji.com

[U47] PHP：联合类型
来源：http://vlt.sweek.top

int|string $id
来源：http://spd.ppjwa.cn

[U48] PHP：纯枚举
来源：http://spf.chenzaomai.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qti.shanyushiyangkeji.top

[U49] PHP：只读属性
来源：http://itr.yvedp.cn

public readonly string $name
来源：http://pyn.zhongyouzk.top

[U50] PHP：构造器属性提升
来源：http://bbr.tianlin.xyz

public function __construct(private int $id) {}
来源：http://lsx.sxryk.cn

[U51] PHP：数组解构
来源：http://cwi.wangdashe.top

[$a, $b] = $arr;
来源：http://koo.guannengcc.top

[U52] PHP：箭头函数
来源：http://tbb.dianchejie.cn

$double = fn($x) => $x * 2;
来源：http://feb.daria6918.cn

[U53] PHP：空合并运算符
来源：http://yem.jinyuanbaomall.cn

$v = $a ?? $b ?? "default";
来源：http://ttt.xinyue.icu

[U54] PHP：空安全调用
来源：http://zhh.svipenyu.cn

$obj?->method()
来源：http://tai.xuetiantiany.cn

[U55] PHP：match 表达式
来源：http://bel.zhoulong.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ihm.xziqi.cn

[U56] PHP：命名参数
来源：http://sgs.yongpay.top

f(a: 1, b: 2)
来源：http://cti.yuxming.cn

[U57] PHP：字符串插值
来源：http://ilj.cqqwz.cn

"值: {$a}"
来源：http://tiw.wangdashe.top

[U58] PHP：数组三件套
来源：http://hoh.havefunace.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tdp.mhx1999.top

[U59] PHP：自定义排序
来源：http://efm.ivvv.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fhd.cheryme.top

[U60] PHP：JSON 编解码
来源：http://iwx.cashguo.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gle.zhiwuduotai.top

[U61] PHP：正则
来源：http://oet.quarkkingdee.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vai.hywenlv.cn

[U62] PHP：日期对象
来源：http://xoh.yj20258.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wsm.jinyuanbaomall.cn

[U63] PHP：文件读写
来源：http://grz.ydjk.org.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lno.zhiwuduotai.top

[U64] PHP：目录遍历
来源：http://zkf.cucudq.cn

glob("dir/*.php");  scandir("dir");
来源：http://wqa.hongshengwenyu.top

[U65] PHP：会话
来源：http://frk.guowangkeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://drd.sjlbkw.cn

[U66] PHP：设置 Cookie
来源：http://jjj.sxryk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ump.mhx1999.top

[U67] PHP：处理文件上传
来源：http://ahx.tanke756.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hqw.pycfn.com

[U68] PHP：PDO 连接
来源：http://nyz.ywan-chungtsiang.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iun.gaohongyu789.top

[U69] PHP：PDO 预处理
来源：http://hhw.yj202588.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eju.hysaishi.cn

[U70] PHP：PDO 事务
来源：http://lam.fzhhl.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jsr.zhaomingkeji.xyz

[U71] PHP：抛出异常
来源：http://rpa.jyoumei.cn

throw new RuntimeException("失败", 500);
来源：http://rvl.yonumen.top

[U72] PHP：写错误日志
来源：http://igl.meibo888.top

error_log("失败: " . $e->getMessage());
来源：http://enc.zhixingplan.top

[U73] PHP：读取 ini 配置
来源：http://yux.quarkkingdee.top

parse_ini_file("config.ini", true)
来源：http://nvb.zycfv.cn

[U74] PHP：读取环境变量
来源：http://pxc.ywan-chungtsiang.top

getenv("APP_ENV") ?: "production"
来源：http://tzu.hammf.cn

[U75] PHP：依赖注入
来源：http://jab.zdbjq.cn

composer require psr/container
来源：http://pst.cqqwz.cn

[U76] PHP：简单路由
来源：http://iyx.mhx1999.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ihs.gzhubu.top

[U77] PHP：模板渲染
来源：http://iqx.jinyuanbaomall.cn

composer require twig/twig
来源：http://pbk.fktsv.cn

[U78] PHP：单元测试
来源：http://qja.tianlin.xyz

composer require --dev phpunit/phpunit
来源：http://qnz.feifeiyinyue.top

[U79] PHP：静态分析
来源：http://mgs.chenlongwang.top

composer require --dev phpstan/phpstan
来源：http://kem.feifeiyinyue.top

[U80] PHP：代码规范修复
来源：http://ogw.hfpthk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dpn.daria6918.cn


<!-- 参考信息 -->