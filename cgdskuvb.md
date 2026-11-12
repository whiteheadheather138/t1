代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nve.yuanzhike.top

[S51] C++：显式类型转换
来源：http://mtq.fanxiaobao.xyz

static_cast<double>(a) / b
来源：http://prx.tianlin.xyz

[S52] C++：const 与 noexcept
来源：http://jts.zdbjq.cn

int size() const noexcept { return n_; }
来源：http://lna.meibo888.top

[S53] C++：移动语义
来源：http://qry.bbcook.cn

std::vector<int> w = std::move(v);
来源：http://ipd.cdnleiting.top

[S54] C++：异常处理
来源：http://zsx.jlsjyb.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yax.sysykeji.top

[S55] C++：结构化绑定
来源：http://zhh.shanyushiyangtech.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rdz.bbcook.cn

[S56] C++：optional
来源：http://jcf.nanxinkj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://veg.yangfankeji.com

[S57] C++：编译期常量
来源：http://axt.zhixingplan.top

constexpr int N = 10;
来源：http://nht.yanxiufei.cn

[S58] C++：命名空间
来源：http://jjw.hnqzz.top

namespace ns { int f() { return 1; } }
来源：http://ehw.daria6918.cn

[S59] C++：静态断言
来源：http://lnn.yanxiufei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bfw.dashuyun.cn

[S60] C++：遍历并删除元素
来源：http://jdh.quarkkingdee.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ttg.svipenyu.cn

================================================================================
来源：http://geb.c1oappe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xfv.shuidangran.top

================================================================================
来源：http://qei.kuanghao11.cn

[T01] Kotlin：Hello World
来源：http://gjx.chenjidiqi.icu

println("Hello")
来源：http://fdj.pycfn.com

[T02] Kotlin：变量
来源：http://lhy.jyoumei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lpx.haohaochexian.top

[T03] Kotlin：字符串模板
来源：http://zib.hcnkem.com

"值: $b"
来源：http://xsb.ppjwa.cn

[T04] Kotlin：空安全
来源：http://hha.cheryme.top

val n: String? = null;  n?.length
来源：http://zal.zycfv.cn

[T05] Kotlin：when 表达式
来源：http://zzy.ctjpmb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://npf.jinyuanbaomall.cn

[T06] Kotlin：集合映射
来源：http://mjx.yangfankeji.com

listOf(1, 2, 3).map { it * 2 }
来源：http://qxf.ydjk.org.cn

[T07] Kotlin：集合过滤
来源：http://oek.jinghuilouyu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vyr.chenzaomai.com

[T08] Kotlin：数据类
来源：http://eop.chenlongwang.top

data class User(val name: String, val age: Int)
来源：http://bde.jqgfzy.top

[T09] Kotlin：扩展函数
来源：http://clc.jqgfzy.top

fun String.exclaim() = this + "!"
来源：http://ksu.zycfv.cn

[T10] Kotlin：默认参数
来源：http://xkn.chenjidiqi.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://vrd.shzxlz.cn

[T11] Kotlin：协程
来源：http://hem.bjfxy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://eom.guannengcc.top

[T12] Kotlin：解构声明
来源：http://whf.316326.xyz

val (a, b) = Pair(1, 2)
来源：http://aca.ydzc1.top

[T13] Kotlin：只读 Map
来源：http://zbi.yonumen.top

val m = mapOf("a" to 1)
来源：http://ief.jlsjyb.cn

[T14] Kotlin：循环
来源：http://zhi.yueranfly.top

for (i in 1..10) println(i)
来源：http://efp.guowangkeji.top

[T15] Kotlin：接口
来源：http://fpz.yfazqb.com

interface Shape { fun area(): Double }
来源：http://dxz.cashguo.top

[T16] Swift：Hello World
来源：http://bjv.smart0.xyz

print("Hello")
来源：http://muc.hammf.cn

[T17] Swift：变量与常量
来源：http://ceq.sxryk.cn

var a = 1;  let b = 2
来源：http://enn.yj20258888.top

[T18] Swift：字符串插值
来源：http://dwc.shuidangran.top

"值: \(b)"
来源：http://yim.fanxiaobao.xyz

[T19] Swift：可选绑定
来源：http://wdj.nwbrower.top

if let n = opt { print(n) }
来源：http://yrl.vehdjk.com

[T20] Swift：数组操作
来源：http://xyw.meibo888.top

var a = [1, 2, 3];  a.append(4)
来源：http://ksq.ywan-chungtsiang.top

[T21] Swift：遍历
来源：http://och.sjlbkw.cn

for x in a { print(x) }
来源：http://xnf.zhongyouzk.top

[T22] Swift：字典
来源：http://scg.9152youxi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xvf.vqdsnc.cn

[T23] Swift：函数
来源：http://aze.yanxiufei.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://roe.0kj1m.cn

[T24] Swift：闭包
来源：http://aao.nanxuanxn.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hgz.guowangkeji.top

[T25] Swift：结构体
来源：http://hes.yongpay.top

struct P { var x: Int }
来源：http://xcy.yuanzhike.top

[T26] Swift：类与重写
来源：http://ozn.ehwqpu.com

class A: Base { override func f() {} }
来源：http://nwc.sxryk.cn

[T27] Swift：错误处理
来源：http://zaj.haohaochexian.top

do { try f() } catch { print(error) }
来源：http://uzx.iojbl.cn

[T28] Swift：枚举
来源：http://vqc.chenlongwang.top

enum Color { case red, green }
来源：http://inz.kuanghao11.cn

[T29] Swift：guard 提前返回
来源：http://lui.shzxlz.cn

guard let x = opt else { return }
来源：http://gqk.haohaochexian.top

[T30] Swift：协议
来源：http://iqq.nanxuanxn.top

protocol Shape { func area() -> Double }
来源：http://oqc.shuidangran.top

[T31] Lua：Hello World
来源：http://mzk.zdbjq.cn

print("Hello")
来源：http://yjl.ydjk.org.cn

[T32] Lua：局部变量
来源：http://vyu.bjfxy.top

local a = 1
来源：http://noi.zdqjudy.top

[T33] Lua：表（数组）
来源：http://ryo.gogol.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://iec.vehdjk.com

[T34] Lua：遍历表
来源：http://ujb.hammf.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pge.xuetiantiany.cn

[T35] Lua：字典表
来源：http://byj.smart0.xyz

local d = { a = 1 };  d.b = 2
来源：http://wxf.ivvv.top

[T36] Lua：函数
来源：http://lcm.shanyushiyangtech.top

function add(a, b) return a + b end
来源：http://vut.shangyingyoupin.top

[T37] Lua：字符串拼接
来源：http://uhv.yueranfly.top

"a" .. "b"
来源：http://hjx.zhongyouzk.top

[T38] Lua：条件
来源：http://kkf.daria6918.cn

if x > 0 then print("正") end
来源：http://joo.jinghuilouyu.cn

[T39] Lua：模式匹配
来源：http://qea.fanxiaobao.xyz

string.find(s, "%d+")
来源：http://ehw.ppjwa.cn

[T40] Lua：元表
来源：http://hnp.tarul.cn

setmetatable({}, { __index = base })
来源：http://bwz.cheryme.top

[T41] Perl：Hello World
来源：http://lym.birdmap.top

print "Hello\n";
来源：http://xny.gzhubu.top

[T42] Perl：变量类型
来源：http://zph.xylfe.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oua.nwbrower.top

[T43] Perl：字符串插值
来源：http://gay.tian-w.cn

"值: $a"
来源：http://wox.fzhhl.top

[T44] Perl：条件
来源：http://phf.cheryme.top

if ($a > 0) { print "正"; }
来源：http://esx.yueranfly.top

[T45] Perl：数组遍历
来源：http://kmg.shanyushiyangkeji.top

for my $x (@arr) { print $x; }
来源：http://tct.jyoumei.cn

[T46] Perl：哈希操作
来源：http://fge.jinqigfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zmi.shanyushiyangtech.top

[T47] Perl：正则捕获
来源：http://svq.hnqzz.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://uhd.hammf.cn

[T48] Perl：正则替换
来源：http://iqq.jinqigfzy.top

$s =~ s/old/new/g;
来源：http://otu.zdbjq.cn

[T49] Perl：函数
来源：http://rqh.hammf.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wpt.chenlongwang.top

[T50] Perl：逐行读文件
来源：http://rni.shuidangran.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mlb.yvedp.cn

while (my $line = <$fh>) { print $line; }
来源：http://hpb.tian-w.cn

[T51] Scala：Hello World
来源：http://xhp.daria6918.cn

println("Hello")
来源：http://csz.jinqigfzy.top

[T52] Scala：变量
来源：http://lgc.shanyushiyangkeji.top

val a = 1;  var b = 2
来源：http://sgk.fanxiaobao.xyz

[T53] Scala：字符串插值
来源：http://bwr.jyoumei.cn

s"值: $b"
来源：http://ovj.yuanzhike.top

[T54] Scala：集合映射
来源：http://esf.fktsv.cn

List(1, 2, 3).map(_ * 2)
来源：http://yzj.fktsv.cn

[T55] Scala：集合过滤
来源：http://wcs.9152youxi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zkr.hesvh.cn

[T56] Scala：样例类
来源：http://qtg.bjfxy.top

case class User(name: String, age: Int)
来源：http://rtu.hysaishi.cn

[T57] Scala：模式匹配
来源：http://oot.pengpengdd.cyou

x match { case 1 => "一"; case _ => "其他" }
来源：http://cpm.316326.xyz

[T58] Scala：函数定义
来源：http://lsm.hfpthk.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dwn.cdnleiting.top

[T59] Scala：循环
来源：http://uwk.haohaochexian.top

for (i <- 1 to 10) println(i)
来源：http://pgr.yj20258888.top

[T60] Scala：折叠
来源：http://cji.jiagoushi.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://soj.fengsongda.top

================================================================================
来源：http://znh.bjfxy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zdg.tianlin.xyz

================================================================================
来源：http://skk.shzxlz.cn

[U01] Py：创建虚拟环境
来源：http://orp.cqqwz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sac.xuanzx.com

[U02] Py：导出 / 安装依赖
来源：http://cad.bbcook.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://btu.jianghu66.top

[U03] Py：加载 .env 配置
来源：http://iab.aibaodan.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://njr.c1oappe.top

[U04] Py：变量调试打印
来源：http://dgn.jyoumei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://agd.hnqzz.top

[U05] Py：列表去重且保序
来源：http://wvr.hesvh.cn

list(dict.fromkeys(arr))
来源：http://xzy.cqqwz.cn

[U06] Py：合并两个字典
来源：http://pxx.chenlongwang.top

{**a, **b}
来源：http://byl.zdqjudy.top

[U07] Py：反转字典键值
来源：http://mid.zhoulong.xyz

{v: k for k, v in d.items()}
来源：http://xoz.xziqi.cn

[U08] Py：展平二维列表
来源：http://otr.hesvh.cn

[y for x in nested for y in x]
来源：http://fhn.nwbrower.top

[U09] Py：字典取最大值的键
来源：http://bxo.xinyue.icu

max(d, key=d.get)
来源：http://uov.havefunace.top

[U10] Py：按值排序字典
来源：http://ski.zdqjudy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jmr.daxiang520.top

[U11] Py：生成器表达式
来源：http://fbp.zhoulong.xyz

(x * 2 for x in arr)
来源：http://pcl.gzhubu.top

[U12] Py：取出现最多的 3 个元素
来源：http://rty.zhixingplan.top

Counter(arr).most_common(3)
来源：http://zup.meibo888.top

[U13] Py：固定长度队列
来源：http://lho.zhoulong.xyz

deque(maxlen=10)
来源：http://hnl.52xcode.cn

[U14] Py：分组收集到列表
来源：http://eoy.quarkkingdee.top

defaultdict(list)
来源：http://ryw.jinqigufen.top

[U15] Py：高精度计时
来源：http://tvx.guannengcc.top

t = time.perf_counter()
来源：http://uui.yj20258.top

[U16] Py：命令行参数解析
来源：http://ane.gzhubu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uqd.fktsv.cn

[U17] Py：初始化日志
来源：http://olb.tianlin.xyz

logging.basicConfig(level=logging.INFO)
来源：http://kqn.zhijiandao.cn

[U18] Py：预编译正则
来源：http://rxo.shanyushiyangkeji.top

pat = re.compile(r"\d+")
来源：http://aoh.bjfxy.top

[U19] Py：正则替换带回调
来源：http://bmb.uphjek.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vya.redwolf501.top

[U20] Py：缓存函数结果
来源：http://lis.xinyue.icu

@functools.lru_cache(maxsize=None)
来源：http://hso.pengpengdd.cyou

[U21] Py：自定义上下文管理器
来源：http://rwf.daria6918.cn

@contextlib.contextmanager
来源：http://tti.0kj1m.cn

[U22] Py：矩阵转置
来源：http://rkm.sxryk.cn

list(zip(*m))
来源：http://pli.52xcode.cn

[U23] Py：分块读取大文件
来源：http://oao.yanxiufei.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ejj.ydjk.org.cn

[U24] Py：路径操作
来源：http://aem.zhiwuduotai.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dhl.chenlongwang.top

[U25] Py：CSV 按字典读
来源：http://hgr.uphjek.com

csv.DictReader(f)
来源：http://wbl.jianghu66.top

[U26] Py：并发下载
来源：http://epa.shanyushiyangtech.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pmf.shuidangran.top

[U27] Py：异步 HTTP
来源：http://spe.cqqwz.cn

aiohttp.ClientSession() 配合 async with
来源：http://zef.sysykeji.top

[U28] Py：类型别名
来源：http://zun.zhoulong.xyz

UserId = int
来源：http://foh.bbcook.cn

[U29] Py：属性校验
来源：http://wzy.52xcode.cn

@property 与 @x.setter 配合
来源：http://vbh.cashguo.top

[U30] Py：数据类
来源：http://uzz.fzhhl.top

@dataclass(slots=True)
来源：http://mgl.sysykeji.top

[U31] Py：单测
来源：http://jlm.birdmap.top

python -m pytest -q
来源：http://vuj.chenzaomai.com

[U32] Py：代码格式化
来源：http://lnn.cucudq.cn

ruff format . && ruff check --fix .
来源：http://ccp.quarkkingdee.top

[U33] Py：打包发布
来源：http://qak.vqdsnc.cn

python -m build  （依赖 pyproject.toml）
来源：http://eja.fzhhl.top

[U34] Py：判断编码
来源：http://nfq.pengpengdd.cyou

chardet.detect(raw)
来源：http://ihn.hysaishi.cn

[U35] Py：发送邮件
来源：http://azc.tarul.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dki.vqdsnc.cn

[U36] Py：定时任务
来源：http://ccw.jqgfzy.top

schedule.every(10).minutes.do(job)
来源：http://cks.jinqigfzy.top

[U37] Py：读写 Excel
来源：http://sga.epnwcf.com

pandas.read_excel / DataFrame.to_excel
来源：http://gjc.nanxuanxn.top

[U38] Py：获取脚本所在目录
来源：http://nny.yanxiufei.cn

Path(__file__).resolve().parent
来源：http://bke.sjlbkw.cn

[U39] Py：判断是否在交互环境
来源：http://swq.0kj1m.cn

sys.stdout.isatty()
来源：http://jst.hcnkem.com

[U40] Py：打印到标准错误
来源：http://khx.hysaishi.cn

print("err", file=sys.stderr)
来源：http://kmx.dashuyun.cn

[U41] PHP：初始化 Composer 项目
来源：http://qvh.9152youxi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zmk.xuetiantiany.cn

[U42] PHP：PSR-4 自动加载
来源：http://twv.52xcode.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jac.mhx1999.top

[U43] PHP：声明命名空间
来源：http://wut.0kj1m.cn

namespace App\Http;
来源：http://wng.gaohongyu789.top

[U44] PHP：开启严格类型
来源：http://eir.hfpthk.cn

declare(strict_types=1);
来源：http://wgm.yj20258888.top

[U45] PHP：类型声明与返回类型
来源：http://dzn.nanxinkj.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zza.jiagoushi.top

[U46] PHP：可空类型
来源：http://pqk.zdqjudy.top

?string $name = null
来源：http://wbf.mhx1999.top

[U47] PHP：联合类型
来源：http://zet.shuidangran.top

int|string $id
来源：http://ngh.sweek.top

[U48] PHP：纯枚举
来源：http://dtr.xuetiantiany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hrw.316326.xyz

[U49] PHP：只读属性
来源：http://wkj.vehdjk.com

public readonly string $name
来源：http://xvf.snrcjt.cn

[U50] PHP：构造器属性提升
来源：http://dxk.daxiang520.top

public function __construct(private int $id) {}
来源：http://csu.jinyuanbaomall.cn

[U51] PHP：数组解构
来源：http://ite.sxryk.cn

[$a, $b] = $arr;
来源：http://poe.mhx1999.top

[U52] PHP：箭头函数
来源：http://eej.haohaochexian.top

$double = fn($x) => $x * 2;
来源：http://btu.fehbvm.com

[U53] PHP：空合并运算符
来源：http://oez.ehwqpu.com

$v = $a ?? $b ?? "default";
来源：http://tgg.shanyushiyangkeji.top

[U54] PHP：空安全调用
来源：http://cod.zdbjq.cn

$obj?->method()
来源：http://rbu.9152youxi.cn

[U55] PHP：match 表达式
来源：http://pea.wangdashe.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://upc.andypj.xyz

[U56] PHP：命名参数
来源：http://utw.aizwys.cn

f(a: 1, b: 2)
来源：http://etm.vqdsnc.cn

[U57] PHP：字符串插值
来源：http://kct.bjfxy.top

"值: {$a}"
来源：http://uux.vqdsnc.cn

[U58] PHP：数组三件套
来源：http://upc.zhengqikj.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vyl.zdbjq.cn

[U59] PHP：自定义排序
来源：http://fuo.vehdjk.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fje.yj202588.top

[U60] PHP：JSON 编解码
来源：http://zcs.ppjwa.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mxs.fengsongda.top

[U61] PHP：正则
来源：http://com.zhaomingkeji.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uem.cucudq.cn

[U62] PHP：日期对象
来源：http://sxf.guannengcc.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://erb.bjfxy.top

[U63] PHP：文件读写
来源：http://qos.xuanzx.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rba.xuetiantiany.cn

[U64] PHP：目录遍历
来源：http://foc.jyoumei.cn

glob("dir/*.php");  scandir("dir");
来源：http://asj.aibaodan.cn

[U65] PHP：会话
来源：http://pka.xylfe.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qzr.nanxuanxn.top

[U66] PHP：设置 Cookie
来源：http://wke.fehbvm.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qpg.ywan-chungtsiang.top

[U67] PHP：处理文件上传
来源：http://zse.hnqzz.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sdo.sysykeji.top

[U68] PHP：PDO 连接
来源：http://wra.iojbl.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://reo.yfazqb.com

[U69] PHP：PDO 预处理
来源：http://big.chenzaomai.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zsa.316326.xyz

[U70] PHP：PDO 事务
来源：http://vby.smart0.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hhp.vehdjk.com

[U71] PHP：抛出异常
来源：http://cgn.c1oappe.top

throw new RuntimeException("失败", 500);
来源：http://wsc.mhx1999.top

[U72] PHP：写错误日志
来源：http://kks.zhengqikj.top

error_log("失败: " . $e->getMessage());
来源：http://msu.ydzc1.top

[U73] PHP：读取 ini 配置
来源：http://bro.vehdjk.com

parse_ini_file("config.ini", true)
来源：http://nfr.zhaomingkeji.xyz

[U74] PHP：读取环境变量
来源：http://hls.ppjwa.cn

getenv("APP_ENV") ?: "production"
来源：http://tzu.hnxiangtu.top

[U75] PHP：依赖注入
来源：http://bnt.zycfv.cn

composer require psr/container
来源：http://mol.yj202588.top

[U76] PHP：简单路由
来源：http://kmy.mhx1999.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tsy.iojbl.cn


<!-- 参考信息 -->