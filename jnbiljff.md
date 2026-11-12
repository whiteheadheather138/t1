代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cnw.hnqzz.top

[S55] C++：结构化绑定
来源：http://gnx.xuetiantiany.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rqs.zhongyouzk.top

[S56] C++：optional
来源：http://rry.zhongyouzk.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://foc.jyoumei.cn

[S57] C++：编译期常量
来源：http://fgv.pycfn.com

constexpr int N = 10;
来源：http://sfd.jinyuanbaomall.cn

[S58] C++：命名空间
来源：http://eka.jlsjyb.cn

namespace ns { int f() { return 1; } }
来源：http://esm.sxryk.cn

[S59] C++：静态断言
来源：http://aff.yj202588.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bgo.0kj1m.cn

[S60] C++：遍历并删除元素
来源：http://mis.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ljg.ivvv.top

================================================================================
来源：http://kcn.bbcook.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lxt.fanxiaobao.xyz

================================================================================
来源：http://oqe.iojbl.cn

[T01] Kotlin：Hello World
来源：http://xex.snrcjt.cn

println("Hello")
来源：http://gdb.sweek.top

[T02] Kotlin：变量
来源：http://ohw.yangfankeji.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://erj.yvedp.cn

[T03] Kotlin：字符串模板
来源：http://sbk.bjfxy.top

"值: $b"
来源：http://kju.hesvh.cn

[T04] Kotlin：空安全
来源：http://yae.yueranfly.top

val n: String? = null;  n?.length
来源：http://qap.pycfn.com

[T05] Kotlin：when 表达式
来源：http://wri.daxiang520.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://spl.hywenlv.cn

[T06] Kotlin：集合映射
来源：http://obp.xinyue.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://sab.zhengqikj.top

[T07] Kotlin：集合过滤
来源：http://kte.fktsv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mnj.sjlbkw.cn

[T08] Kotlin：数据类
来源：http://lfn.gogol.net.cn

data class User(val name: String, val age: Int)
来源：http://smc.tian-w.cn

[T09] Kotlin：扩展函数
来源：http://yer.fktsv.cn

fun String.exclaim() = this + "!"
来源：http://fem.cqqwz.cn

[T10] Kotlin：默认参数
来源：http://axp.yonumen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://uqx.hongshengwenyu.top

[T11] Kotlin：协程
来源：http://rkw.birdmap.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://yaw.jiagoushi.top

[T12] Kotlin：解构声明
来源：http://arr.tian-w.cn

val (a, b) = Pair(1, 2)
来源：http://opn.cdnleiting.top

[T13] Kotlin：只读 Map
来源：http://whm.fktsv.cn

val m = mapOf("a" to 1)
来源：http://lhd.shanyushiyangtech.top

[T14] Kotlin：循环
来源：http://sfl.jinqigfzy.top

for (i in 1..10) println(i)
来源：http://dww.cqqwz.cn

[T15] Kotlin：接口
来源：http://pkj.nanxuanxn.top

interface Shape { fun area(): Double }
来源：http://rbb.ybcxt.top

[T16] Swift：Hello World
来源：http://jhb.vqdsnc.cn

print("Hello")
来源：http://nwv.xingfuxueyuan.xyz

[T17] Swift：变量与常量
来源：http://bjq.jqgufenzy.top

var a = 1;  let b = 2
来源：http://lbz.havefunace.top

[T18] Swift：字符串插值
来源：http://nya.yj20258888.top

"值: \(b)"
来源：http://ghs.xziqi.cn

[T19] Swift：可选绑定
来源：http://qmu.hfpthk.cn

if let n = opt { print(n) }
来源：http://ety.xziqi.cn

[T20] Swift：数组操作
来源：http://fne.hongshengwenyu.top

var a = [1, 2, 3];  a.append(4)
来源：http://klv.xziqi.cn

[T21] Swift：遍历
来源：http://ebr.ppjwa.cn

for x in a { print(x) }
来源：http://vbu.sjlbkw.cn

[T22] Swift：字典
来源：http://bpq.fzhhl.top

var d = ["a": 1];  d["b"] = 2
来源：http://pgt.jiagoushi.top

[T23] Swift：函数
来源：http://glv.chenlongwang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ytj.hfpthk.cn

[T24] Swift：闭包
来源：http://qwn.ydjk.org.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lco.aizwys.cn

[T25] Swift：结构体
来源：http://grw.jqgufenzy.top

struct P { var x: Int }
来源：http://aei.fktsv.cn

[T26] Swift：类与重写
来源：http://fuc.shanyushiyangkeji.top

class A: Base { override func f() {} }
来源：http://svn.zdqjudy.top

[T27] Swift：错误处理
来源：http://yyv.ivvv.top

do { try f() } catch { print(error) }
来源：http://xst.hcnkem.com

[T28] Swift：枚举
来源：http://yix.gogol.net.cn

enum Color { case red, green }
来源：http://alv.tanke756.top

[T29] Swift：guard 提前返回
来源：http://yvl.dianchejie.cn

guard let x = opt else { return }
来源：http://tyr.hnqzz.top

[T30] Swift：协议
来源：http://wvu.bbcook.cn

protocol Shape { func area() -> Double }
来源：http://gdh.yangfankeji.com

[T31] Lua：Hello World
来源：http://hsn.fzhhl.top

print("Hello")
来源：http://ylr.hongshengwenyu.top

[T32] Lua：局部变量
来源：http://bzc.fanxiaobao.xyz

local a = 1
来源：http://bri.ybcxt.top

[T33] Lua：表（数组）
来源：http://nge.meibo888.top

local t = {1, 2, 3};  t[4] = 4
来源：http://moo.hesvh.cn

[T34] Lua：遍历表
来源：http://ddb.zhengqikj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://obc.havefunace.top

[T35] Lua：字典表
来源：http://yfs.yangfankeji.com

local d = { a = 1 };  d.b = 2
来源：http://dje.fengsongda.top

[T36] Lua：函数
来源：http://vph.nanxinkj.top

function add(a, b) return a + b end
来源：http://vrb.smart0.xyz

[T37] Lua：字符串拼接
来源：http://xnj.havefunace.top

"a" .. "b"
来源：http://oid.hongshengwenyu.top

[T38] Lua：条件
来源：http://qzi.52xcode.cn

if x > 0 then print("正") end
来源：http://kkp.jinqigufen.top

[T39] Lua：模式匹配
来源：http://adw.ppjwa.cn

string.find(s, "%d+")
来源：http://kul.daxiang520.top

[T40] Lua：元表
来源：http://gvj.feifeiyinyue.top

setmetatable({}, { __index = base })
来源：http://wkl.tianlin.xyz

[T41] Perl：Hello World
来源：http://txc.daxiang520.top

print "Hello\n";
来源：http://oue.yangfankeji.com

[T42] Perl：变量类型
来源：http://ubl.yongpay.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gyb.jinqigfzy.top

[T43] Perl：字符串插值
来源：http://oju.shanyushiyangkeji.top

"值: $a"
来源：http://xsk.pycfn.com

[T44] Perl：条件
来源：http://rec.gogol.net.cn

if ($a > 0) { print "正"; }
来源：http://ttm.nanxuanxn.top

[T45] Perl：数组遍历
来源：http://bgc.zhiwuduotai.top

for my $x (@arr) { print $x; }
来源：http://phd.zhengqikj.top

[T46] Perl：哈希操作
来源：http://tua.epnwcf.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ntk.jqgufenzy.top

[T47] Perl：正则捕获
来源：http://rmm.sysykeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qga.andypj.xyz

[T48] Perl：正则替换
来源：http://rmf.cdnleiting.top

$s =~ s/old/new/g;
来源：http://xvj.yj202588.top

[T49] Perl：函数
来源：http://ftg.kuanghao11.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qmg.xuetiantiany.cn

[T50] Perl：逐行读文件
来源：http://udn.sweek.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dku.zdqjudy.top

while (my $line = <$fh>) { print $line; }
来源：http://bmw.bjfxy.top

[T51] Scala：Hello World
来源：http://kom.hysaishi.cn

println("Hello")
来源：http://mwt.zdbjq.cn

[T52] Scala：变量
来源：http://rsh.yongpay.top

val a = 1;  var b = 2
来源：http://quo.jqgufenzy.top

[T53] Scala：字符串插值
来源：http://wnk.hcnkem.com

s"值: $b"
来源：http://vjy.vehdjk.com

[T54] Scala：集合映射
来源：http://uyv.pycfn.com

List(1, 2, 3).map(_ * 2)
来源：http://beo.dianchejie.cn

[T55] Scala：集合过滤
来源：http://mgu.sxryk.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bsm.wangshuangyany.cn

[T56] Scala：样例类
来源：http://wix.iojbl.cn

case class User(name: String, age: Int)
来源：http://ikj.jlsjyb.cn

[T57] Scala：模式匹配
来源：http://stq.316326.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://enx.guowangkeji.top

[T58] Scala：函数定义
来源：http://alt.mhx1999.top

def add(a: Int, b: Int): Int = a + b
来源：http://jgl.vqdsnc.cn

[T59] Scala：循环
来源：http://fhh.jianghu66.top

for (i <- 1 to 10) println(i)
来源：http://yop.wangshuangyany.cn

[T60] Scala：折叠
来源：http://meh.shzxlz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pvs.dianchejie.cn

================================================================================
来源：http://hqj.yj20258888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gmg.jqgufenzy.top

================================================================================
来源：http://ajk.tarul.cn

[U01] Py：创建虚拟环境
来源：http://qua.gotoacloud.top

python -m venv .venv && source .venv/bin/activate
来源：http://dip.chenjidiqi.icu

[U02] Py：导出 / 安装依赖
来源：http://nkn.ppjwa.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ttw.jqgfzy.top

[U03] Py：加载 .env 配置
来源：http://obr.iojbl.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uwx.gogol.net.cn

[U04] Py：变量调试打印
来源：http://zzq.gaohongyu789.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dhl.hnqzz.top

[U05] Py：列表去重且保序
来源：http://lqd.cucudq.cn

list(dict.fromkeys(arr))
来源：http://ztn.aizwys.cn

[U06] Py：合并两个字典
来源：http://rwi.xuetiantiany.cn

{**a, **b}
来源：http://sye.daria6918.cn

[U07] Py：反转字典键值
来源：http://fdh.gzhubu.top

{v: k for k, v in d.items()}
来源：http://smj.yvedp.cn

[U08] Py：展平二维列表
来源：http://wpd.zdqjudy.top

[y for x in nested for y in x]
来源：http://mce.hysaishi.cn

[U09] Py：字典取最大值的键
来源：http://mux.jqgufenzy.top

max(d, key=d.get)
来源：http://tgk.yj20258.top

[U10] Py：按值排序字典
来源：http://rif.ydjk.org.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fpa.shzxlz.cn

[U11] Py：生成器表达式
来源：http://ond.hfpthk.cn

(x * 2 for x in arr)
来源：http://rqp.0kj1m.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zfd.guannengcc.top

Counter(arr).most_common(3)
来源：http://vnd.jinyuanbaomall.cn

[U13] Py：固定长度队列
来源：http://zno.sysykeji.top

deque(maxlen=10)
来源：http://ezf.dianchejie.cn

[U14] Py：分组收集到列表
来源：http://ahq.cheryme.top

defaultdict(list)
来源：http://pok.tarul.cn

[U15] Py：高精度计时
来源：http://szz.tian-w.cn

t = time.perf_counter()
来源：http://fwn.daria6918.cn

[U16] Py：命令行参数解析
来源：http://qku.hammf.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sjs.xylfe.cn

[U17] Py：初始化日志
来源：http://ili.tianlin.xyz

logging.basicConfig(level=logging.INFO)
来源：http://bqd.jiagoushi.top

[U18] Py：预编译正则
来源：http://kzc.ctjpmb.com

pat = re.compile(r"\d+")
来源：http://gwi.zhijiandao.cn

[U19] Py：正则替换带回调
来源：http://hcy.redwolf501.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://smt.yangfankeji.com

[U20] Py：缓存函数结果
来源：http://drw.havefunace.top

@functools.lru_cache(maxsize=None)
来源：http://sjo.zdbjq.cn

[U21] Py：自定义上下文管理器
来源：http://gbh.bjfxy.top

@contextlib.contextmanager
来源：http://umf.yj20258888.top

[U22] Py：矩阵转置
来源：http://ovu.bbcook.cn

list(zip(*m))
来源：http://ats.hfpthk.cn

[U23] Py：分块读取大文件
来源：http://pql.nanxinkj.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oae.zhiwuduotai.top

[U24] Py：路径操作
来源：http://zhw.smart0.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vkg.0kj1m.cn

[U25] Py：CSV 按字典读
来源：http://cqk.jqgfzy.top

csv.DictReader(f)
来源：http://efe.vehdjk.com

[U26] Py：并发下载
来源：http://zxa.gaohongyu789.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://aai.shanyushiyangkeji.top

[U27] Py：异步 HTTP
来源：http://ydt.zhoulong.xyz

aiohttp.ClientSession() 配合 async with
来源：http://vyu.cashguo.top

[U28] Py：类型别名
来源：http://tjx.fanxiaobao.xyz

UserId = int
来源：http://fdy.zdbjq.cn

[U29] Py：属性校验
来源：http://ajw.cdnleiting.top

@property 与 @x.setter 配合
来源：http://qzn.yangfankeji.com

[U30] Py：数据类
来源：http://gao.ywan-chungtsiang.top

@dataclass(slots=True)
来源：http://him.tianlin.xyz

[U31] Py：单测
来源：http://sod.xingfuxueyuan.xyz

python -m pytest -q
来源：http://xms.jyoumei.cn

[U32] Py：代码格式化
来源：http://zko.dashuyun.cn

ruff format . && ruff check --fix .
来源：http://eco.wangshuangyany.cn

[U33] Py：打包发布
来源：http://ugm.cashguo.top

python -m build  （依赖 pyproject.toml）
来源：http://rps.tian-w.cn

[U34] Py：判断编码
来源：http://yqh.birdmap.top

chardet.detect(raw)
来源：http://gef.haohaochexian.top

[U35] Py：发送邮件
来源：http://vfk.jiagoushi.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://aew.xuetiantiany.cn

[U36] Py：定时任务
来源：http://lnc.sufxvd.cn

schedule.every(10).minutes.do(job)
来源：http://enh.yj202588.top

[U37] Py：读写 Excel
来源：http://vto.ppjwa.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rgx.cqqwz.cn

[U38] Py：获取脚本所在目录
来源：http://fyg.hysaishi.cn

Path(__file__).resolve().parent
来源：http://olo.shuidangran.top

[U39] Py：判断是否在交互环境
来源：http://bjp.fanxiaobao.xyz

sys.stdout.isatty()
来源：http://ugs.xuanzx.com

[U40] Py：打印到标准错误
来源：http://gay.xinyue.icu

print("err", file=sys.stderr)
来源：http://zpy.shanyushiyangkeji.top

[U41] PHP：初始化 Composer 项目
来源：http://wkc.shuidangran.top

composer init;  composer require guzzlehttp/guzzle
来源：http://aky.jyoumei.cn

[U42] PHP：PSR-4 自动加载
来源：http://iic.yueranfly.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mxy.cdnleiting.top

[U43] PHP：声明命名空间
来源：http://sph.zhixingplan.top

namespace App\Http;
来源：http://inw.svipenyu.cn

[U44] PHP：开启严格类型
来源：http://rjl.yj202588.top

declare(strict_types=1);
来源：http://vrp.daria6918.cn

[U45] PHP：类型声明与返回类型
来源：http://xjz.quarkkingdee.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://wou.fanxiaobao.xyz

[U46] PHP：可空类型
来源：http://fnx.jqgfzy.top

?string $name = null
来源：http://jgg.xuetiantiany.cn

[U47] PHP：联合类型
来源：http://kfw.shanyushiyangkeji.top

int|string $id
来源：http://khv.guowangkeji.top

[U48] PHP：纯枚举
来源：http://ogx.zhixingplan.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://oti.bbcook.cn

[U49] PHP：只读属性
来源：http://kyr.sweek.top

public readonly string $name
来源：http://inh.guowangkeji.top

[U50] PHP：构造器属性提升
来源：http://rjc.yj20258888.top

public function __construct(private int $id) {}
来源：http://yxv.tian-w.cn

[U51] PHP：数组解构
来源：http://alb.fktsv.cn

[$a, $b] = $arr;
来源：http://tlb.guowangkeji.top

[U52] PHP：箭头函数
来源：http://omi.sjlbkw.cn

$double = fn($x) => $x * 2;
来源：http://iuy.jinqigufen.top

[U53] PHP：空合并运算符
来源：http://bkf.xuanzx.com

$v = $a ?? $b ?? "default";
来源：http://sls.pengpengdd.cyou

[U54] PHP：空安全调用
来源：http://nlh.gaohongyu789.top

$obj?->method()
来源：http://uuk.hongshengwenyu.top

[U55] PHP：match 表达式
来源：http://mlm.vehdjk.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xyg.yj20258888.top

[U56] PHP：命名参数
来源：http://ubh.jiagoushi.top

f(a: 1, b: 2)
来源：http://fyz.shangyingyoupin.top

[U57] PHP：字符串插值
来源：http://plc.fengsongda.top

"值: {$a}"
来源：http://xbr.tarul.cn

[U58] PHP：数组三件套
来源：http://vyy.vqdsnc.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zjp.ctjpmb.com

[U59] PHP：自定义排序
来源：http://enx.shanyushiyangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sdt.ctjpmb.com

[U60] PHP：JSON 编解码
来源：http://hql.316326.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dox.fzhhl.top

[U61] PHP：正则
来源：http://ped.quarkkingdee.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kwg.fktsv.cn

[U62] PHP：日期对象
来源：http://tle.kuanghao11.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mwg.ppjwa.cn

[U63] PHP：文件读写
来源：http://dwy.snrcjt.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tsz.feifeiyinyue.top

[U64] PHP：目录遍历
来源：http://ago.sjlbkw.cn

glob("dir/*.php");  scandir("dir");
来源：http://iyq.sysykeji.top

[U65] PHP：会话
来源：http://gov.wangdashe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://iai.snrcjt.cn

[U66] PHP：设置 Cookie
来源：http://yxm.fzhhl.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://szj.hysaishi.cn

[U67] PHP：处理文件上传
来源：http://nmd.xuanzx.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yyu.feifeiyinyue.top

[U68] PHP：PDO 连接
来源：http://ufz.zycfv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://prl.ppjwa.cn

[U69] PHP：PDO 预处理
来源：http://qoz.nwbrower.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://shz.0kj1m.cn

[U70] PHP：PDO 事务
来源：http://try.haohaochexian.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://aqe.tianlin.xyz

[U71] PHP：抛出异常
来源：http://pqa.zhiwuduotai.top

throw new RuntimeException("失败", 500);
来源：http://qxt.svipenyu.cn

[U72] PHP：写错误日志
来源：http://wiq.hywenlv.cn

error_log("失败: " . $e->getMessage());
来源：http://oau.316326.xyz

[U73] PHP：读取 ini 配置
来源：http://bes.bbcook.cn

parse_ini_file("config.ini", true)
来源：http://slu.52xcode.cn

[U74] PHP：读取环境变量
来源：http://nbn.yuxming.cn

getenv("APP_ENV") ?: "production"
来源：http://uqt.xuanzx.com

[U75] PHP：依赖注入
来源：http://vgy.jiagoushi.top

composer require psr/container
来源：http://okj.jlsjyb.cn

[U76] PHP：简单路由
来源：http://uto.hammf.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oxk.pengpengdd.cyou

[U77] PHP：模板渲染
来源：http://kox.yueranfly.top

composer require twig/twig
来源：http://xnh.hfpthk.cn

[U78] PHP：单元测试
来源：http://rwq.jinyuanbaomall.cn

composer require --dev phpunit/phpunit
来源：http://sus.yuanzhike.top

[U79] PHP：静态分析
来源：http://jqi.zhaomingkeji.xyz

composer require --dev phpstan/phpstan
来源：http://loq.redwolf501.top

[U80] PHP：代码规范修复
来源：http://uby.ppjwa.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zfx.jlsjyb.cn


<!-- 参考信息 -->