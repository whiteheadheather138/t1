代发 wailian999

[S43] C++：智能指针
来源：http://dhx.fktsv.cn

auto p = std::make_unique<int>(5);
来源：http://lpq.jinyuanbaomall.cn

[S44] C++：引用传参
来源：http://sdi.nanxuanxn.top

void inc(int &x) { ++x; }
来源：http://kke.sxryk.cn

[S45] C++：lambda
来源：http://wzb.jinqigufen.top

auto add = [](int a, int b) { return a + b; };
来源：http://hjh.yuanzhike.top

[S46] C++：函数模板
来源：http://zvz.shuidangran.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qdn.cheryme.top

[S47] C++：结构化绑定遍历
来源：http://ofy.yj20258888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://udq.xingfuxueyuan.xyz

[S48] C++：逐行读文件
来源：http://ysc.xziqi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://whr.zhongyouzk.top

while (std::getline(in, line)) { }
来源：http://lpr.yj20258888.top

[S49] C++：写文件
来源：http://dxk.zhiwuduotai.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ddx.ppjwa.cn

[S50] C++：格式化数字
来源：http://uib.aizwys.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ncj.birdmap.top

[S51] C++：显式类型转换
来源：http://qbz.andypj.xyz

static_cast<double>(a) / b
来源：http://itz.daxiang520.top

[S52] C++：const 与 noexcept
来源：http://qps.hywenlv.cn

int size() const noexcept { return n_; }
来源：http://zlb.yangfankeji.com

[S53] C++：移动语义
来源：http://iuc.jyoumei.cn

std::vector<int> w = std::move(v);
来源：http://mzy.jinghuilouyu.cn

[S54] C++：异常处理
来源：http://lil.smart0.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://umk.cdnleiting.top

[S55] C++：结构化绑定
来源：http://lio.jlsjyb.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wtx.vqdsnc.cn

[S56] C++：optional
来源：http://wej.fzhhl.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gie.jlsjyb.cn

[S57] C++：编译期常量
来源：http://unw.aizwys.cn

constexpr int N = 10;
来源：http://zob.xziqi.cn

[S58] C++：命名空间
来源：http://pco.xuanzx.com

namespace ns { int f() { return 1; } }
来源：http://ydv.jqgufenzy.top

[S59] C++：静态断言
来源：http://jhr.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bio.guannengcc.top

[S60] C++：遍历并删除元素
来源：http://fzu.sysykeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iwv.hysaishi.cn

================================================================================
来源：http://ugo.yonumen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://whi.bjfxy.top

================================================================================
来源：http://wxu.hammf.cn

[T01] Kotlin：Hello World
来源：http://ouq.jinyuanbaomall.cn

println("Hello")
来源：http://mpt.zhijiandao.cn

[T02] Kotlin：变量
来源：http://zmi.yuanzhike.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://duh.fzhhl.top

[T03] Kotlin：字符串模板
来源：http://agi.guannengcc.top

"值: $b"
来源：http://ucj.aizwys.cn

[T04] Kotlin：空安全
来源：http://lca.hcnkem.com

val n: String? = null;  n?.length
来源：http://dqk.bbcook.cn

[T05] Kotlin：when 表达式
来源：http://lwv.jlsjyb.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ugy.yangfankeji.com

[T06] Kotlin：集合映射
来源：http://ojb.birdmap.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ptr.ydjk.org.cn

[T07] Kotlin：集合过滤
来源：http://aoz.52xcode.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zsq.yuanzhike.top

[T08] Kotlin：数据类
来源：http://aui.snrcjt.cn

data class User(val name: String, val age: Int)
来源：http://mac.52xcode.cn

[T09] Kotlin：扩展函数
来源：http://lkx.ywan-chungtsiang.top

fun String.exclaim() = this + "!"
来源：http://bmx.jqgfzy.top

[T10] Kotlin：默认参数
来源：http://wzw.zhoulong.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://qqg.ivvv.top

[T11] Kotlin：协程
来源：http://vgt.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rmx.xylfe.cn

[T12] Kotlin：解构声明
来源：http://xvy.nwbrower.top

val (a, b) = Pair(1, 2)
来源：http://lep.ctjpmb.com

[T13] Kotlin：只读 Map
来源：http://fxk.cucudq.cn

val m = mapOf("a" to 1)
来源：http://vnp.52xcode.cn

[T14] Kotlin：循环
来源：http://bsa.zhixingplan.top

for (i in 1..10) println(i)
来源：http://gxd.uphjek.com

[T15] Kotlin：接口
来源：http://dwk.fanxiaobao.xyz

interface Shape { fun area(): Double }
来源：http://kky.vehdjk.com

[T16] Swift：Hello World
来源：http://qet.pycfn.com

print("Hello")
来源：http://kju.guowangkeji.top

[T17] Swift：变量与常量
来源：http://ijp.gogol.net.cn

var a = 1;  let b = 2
来源：http://hbt.sufxvd.cn

[T18] Swift：字符串插值
来源：http://zau.jqgfzy.top

"值: \(b)"
来源：http://vqv.xylfe.cn

[T19] Swift：可选绑定
来源：http://uzv.hysaishi.cn

if let n = opt { print(n) }
来源：http://xoq.mhx1999.top

[T20] Swift：数组操作
来源：http://lrt.gaohongyu789.top

var a = [1, 2, 3];  a.append(4)
来源：http://nbz.daria6918.cn

[T21] Swift：遍历
来源：http://ryb.smart0.xyz

for x in a { print(x) }
来源：http://psf.ppjwa.cn

[T22] Swift：字典
来源：http://pgx.zhaomingkeji.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://zmr.zhoulong.xyz

[T23] Swift：函数
来源：http://syl.snrcjt.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vyz.bjfxy.top

[T24] Swift：闭包
来源：http://aat.fanxiaobao.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://jiu.sufxvd.cn

[T25] Swift：结构体
来源：http://drj.shuidangran.top

struct P { var x: Int }
来源：http://fpx.ppjwa.cn

[T26] Swift：类与重写
来源：http://zqw.zhengqikj.top

class A: Base { override func f() {} }
来源：http://cwr.yfazqb.com

[T27] Swift：错误处理
来源：http://vrq.ydjk.org.cn

do { try f() } catch { print(error) }
来源：http://dfi.yfazqb.com

[T28] Swift：枚举
来源：http://yto.tarul.cn

enum Color { case red, green }
来源：http://bnp.fengsongda.top

[T29] Swift：guard 提前返回
来源：http://uwc.9152youxi.cn

guard let x = opt else { return }
来源：http://fav.hesvh.cn

[T30] Swift：协议
来源：http://etw.dianchejie.cn

protocol Shape { func area() -> Double }
来源：http://pwh.kuanghao11.cn

[T31] Lua：Hello World
来源：http://fnp.sxryk.cn

print("Hello")
来源：http://hcn.nanxuanxn.top

[T32] Lua：局部变量
来源：http://ukv.sysykeji.top

local a = 1
来源：http://qyw.jianghu66.top

[T33] Lua：表（数组）
来源：http://bcb.shanyushiyangtech.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pqs.ybcxt.top

[T34] Lua：遍历表
来源：http://ymj.cheryme.top

for i, v in ipairs(t) do print(i, v) end
来源：http://dbc.ivvv.top

[T35] Lua：字典表
来源：http://neb.chenlongwang.top

local d = { a = 1 };  d.b = 2
来源：http://pmp.chenlongwang.top

[T36] Lua：函数
来源：http://nco.yanxiufei.cn

function add(a, b) return a + b end
来源：http://dbx.0kj1m.cn

[T37] Lua：字符串拼接
来源：http://els.sysykeji.top

"a" .. "b"
来源：http://eof.smart0.xyz

[T38] Lua：条件
来源：http://anl.fehbvm.com

if x > 0 then print("正") end
来源：http://lea.jqgufenzy.top

[T39] Lua：模式匹配
来源：http://tni.cucudq.cn

string.find(s, "%d+")
来源：http://oeu.zhoulong.xyz

[T40] Lua：元表
来源：http://che.sysykeji.top

setmetatable({}, { __index = base })
来源：http://yvo.bbcook.cn

[T41] Perl：Hello World
来源：http://zku.ctjpmb.com

print "Hello\n";
来源：http://iog.shzxlz.cn

[T42] Perl：变量类型
来源：http://gzy.cheryme.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ioe.tianlin.xyz

[T43] Perl：字符串插值
来源：http://bgb.fehbvm.com

"值: $a"
来源：http://rwz.xylfe.cn

[T44] Perl：条件
来源：http://dwl.chenzaomai.com

if ($a > 0) { print "正"; }
来源：http://rrj.quarkkingdee.top

[T45] Perl：数组遍历
来源：http://cuh.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://qle.sxryk.cn

[T46] Perl：哈希操作
来源：http://gyc.yvedp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://abs.wangdashe.top

[T47] Perl：正则捕获
来源：http://hfx.gogol.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://igi.ybcxt.top

[T48] Perl：正则替换
来源：http://qdi.daria6918.cn

$s =~ s/old/new/g;
来源：http://jrh.aizwys.cn

[T49] Perl：函数
来源：http://dbe.kuanghao11.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ywo.kuanghao11.cn

[T50] Perl：逐行读文件
来源：http://tsd.haohaochexian.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ttz.sjlbkw.cn

while (my $line = <$fh>) { print $line; }
来源：http://dit.uphjek.com

[T51] Scala：Hello World
来源：http://uzq.ppjwa.cn

println("Hello")
来源：http://toh.chenlongwang.top

[T52] Scala：变量
来源：http://xff.nanxinkj.top

val a = 1;  var b = 2
来源：http://wem.wangshuangyany.cn

[T53] Scala：字符串插值
来源：http://bau.vehdjk.com

s"值: $b"
来源：http://ele.quarkkingdee.top

[T54] Scala：集合映射
来源：http://nyf.feifeiyinyue.top

List(1, 2, 3).map(_ * 2)
来源：http://szp.zdqjudy.top

[T55] Scala：集合过滤
来源：http://yft.redwolf501.top

List(1, 2, 3).filter(_ > 1)
来源：http://sgp.sweek.top

[T56] Scala：样例类
来源：http://jdy.sweek.top

case class User(name: String, age: Int)
来源：http://fud.xylfe.cn

[T57] Scala：模式匹配
来源：http://tso.fktsv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://eti.jqgfzy.top

[T58] Scala：函数定义
来源：http://fuk.yfazqb.com

def add(a: Int, b: Int): Int = a + b
来源：http://quq.zhengqikj.top

[T59] Scala：循环
来源：http://mvn.jqgufenzy.top

for (i <- 1 to 10) println(i)
来源：http://hth.jinyuanbaomall.cn

[T60] Scala：折叠
来源：http://dfc.jinghuilouyu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nst.zhiwuduotai.top

================================================================================
来源：http://yko.kuanghao11.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iow.redwolf501.top

================================================================================
来源：http://xoe.yj20258888.top

[U01] Py：创建虚拟环境
来源：http://awo.shanyushiyangtech.top

python -m venv .venv && source .venv/bin/activate
来源：http://yyx.ctjpmb.com

[U02] Py：导出 / 安装依赖
来源：http://jqd.dashuyun.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pez.fzhhl.top

[U03] Py：加载 .env 配置
来源：http://mdo.vqdsnc.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cuv.yj20258888.top

[U04] Py：变量调试打印
来源：http://bkr.dianchejie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://for.fengsongda.top

[U05] Py：列表去重且保序
来源：http://ayg.redwolf501.top

list(dict.fromkeys(arr))
来源：http://jiu.sweek.top

[U06] Py：合并两个字典
来源：http://hkd.hammf.cn

{**a, **b}
来源：http://avk.uphjek.com

[U07] Py：反转字典键值
来源：http://hic.sjlbkw.cn

{v: k for k, v in d.items()}
来源：http://boe.dashuyun.cn

[U08] Py：展平二维列表
来源：http://qza.xylfe.cn

[y for x in nested for y in x]
来源：http://dmm.gotoacloud.top

[U09] Py：字典取最大值的键
来源：http://rug.wangdashe.top

max(d, key=d.get)
来源：http://zfk.yanxiufei.cn

[U10] Py：按值排序字典
来源：http://gty.uphjek.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://brg.yj20258.top

[U11] Py：生成器表达式
来源：http://gdk.yfazqb.com

(x * 2 for x in arr)
来源：http://ixz.sysykeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://pak.yuanzhike.top

Counter(arr).most_common(3)
来源：http://fal.feifeiyinyue.top

[U13] Py：固定长度队列
来源：http://rwn.ivvv.top

deque(maxlen=10)
来源：http://cqg.yangfankeji.com

[U14] Py：分组收集到列表
来源：http://kbg.zhoulong.xyz

defaultdict(list)
来源：http://rgt.nanxinkj.top

[U15] Py：高精度计时
来源：http://ukn.jinqigfzy.top

t = time.perf_counter()
来源：http://xfw.shanyushiyangtech.top

[U16] Py：命令行参数解析
来源：http://kue.yuanzhike.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hgu.hfpthk.cn

[U17] Py：初始化日志
来源：http://afl.dashuyun.cn

logging.basicConfig(level=logging.INFO)
来源：http://tox.daria6918.cn

[U18] Py：预编译正则
来源：http://rhe.sjlbkw.cn

pat = re.compile(r"\d+")
来源：http://cyw.smart0.xyz

[U19] Py：正则替换带回调
来源：http://ipp.hywenlv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://smb.aizwys.cn

[U20] Py：缓存函数结果
来源：http://soq.andypj.xyz

@functools.lru_cache(maxsize=None)
来源：http://mdw.yangfankeji.com

[U21] Py：自定义上下文管理器
来源：http://vwm.9152youxi.cn

@contextlib.contextmanager
来源：http://qie.guannengcc.top

[U22] Py：矩阵转置
来源：http://hsd.pycfn.com

list(zip(*m))
来源：http://jba.gzhubu.top

[U23] Py：分块读取大文件
来源：http://wvn.zhoulong.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oam.9152youxi.cn

[U24] Py：路径操作
来源：http://hxf.xylfe.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dse.iojbl.cn

[U25] Py：CSV 按字典读
来源：http://xgk.ywan-chungtsiang.top

csv.DictReader(f)
来源：http://ept.xuetiantiany.cn

[U26] Py：并发下载
来源：http://exr.gogol.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wpc.jinyuanbaomall.cn

[U27] Py：异步 HTTP
来源：http://pne.cashguo.top

aiohttp.ClientSession() 配合 async with
来源：http://wdj.birdmap.top

[U28] Py：类型别名
来源：http://vjb.nanxuanxn.top

UserId = int
来源：http://ayv.shuidangran.top

[U29] Py：属性校验
来源：http://wcp.jinyuanbaomall.cn

@property 与 @x.setter 配合
来源：http://lxv.yueranfly.top

[U30] Py：数据类
来源：http://jju.daxiang520.top

@dataclass(slots=True)
来源：http://fsj.cucudq.cn

[U31] Py：单测
来源：http://wcl.nanxinkj.top

python -m pytest -q
来源：http://cdx.yj20258.top

[U32] Py：代码格式化
来源：http://xhz.epnwcf.com

ruff format . && ruff check --fix .
来源：http://apt.gogol.net.cn

[U33] Py：打包发布
来源：http://dto.gogol.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://vbf.ivvv.top

[U34] Py：判断编码
来源：http://bdc.yueranfly.top

chardet.detect(raw)
来源：http://nea.yuanzhike.top

[U35] Py：发送邮件
来源：http://yoi.52xcode.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://auq.fanxiaobao.xyz

[U36] Py：定时任务
来源：http://cjb.mhx1999.top

schedule.every(10).minutes.do(job)
来源：http://zyk.ctjpmb.com

[U37] Py：读写 Excel
来源：http://vqt.shzxlz.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bbh.fktsv.cn

[U38] Py：获取脚本所在目录
来源：http://gdv.ydzc1.top

Path(__file__).resolve().parent
来源：http://luu.hcnkem.com

[U39] Py：判断是否在交互环境
来源：http://qdb.havefunace.top

sys.stdout.isatty()
来源：http://tfu.bjfxy.top

[U40] Py：打印到标准错误
来源：http://ixl.sweek.top

print("err", file=sys.stderr)
来源：http://pir.tianlin.xyz

[U41] PHP：初始化 Composer 项目
来源：http://hjm.wangshuangyany.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tmu.zhongyouzk.top

[U42] PHP：PSR-4 自动加载
来源：http://jyh.yuxming.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bwb.kuanghao11.cn

[U43] PHP：声明命名空间
来源：http://hqt.dianchejie.cn

namespace App\Http;
来源：http://ynt.jinqigufen.top

[U44] PHP：开启严格类型
来源：http://qhe.hesvh.cn

declare(strict_types=1);
来源：http://fqw.xylfe.cn

[U45] PHP：类型声明与返回类型
来源：http://bkz.epnwcf.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://gyx.yj20258.top

[U46] PHP：可空类型
来源：http://ksw.xylfe.cn

?string $name = null
来源：http://kxh.jlsjyb.cn

[U47] PHP：联合类型
来源：http://nji.ivvv.top

int|string $id
来源：http://ahf.zhoulong.xyz

[U48] PHP：纯枚举
来源：http://iwe.bjfxy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://arz.jianghu66.top

[U49] PHP：只读属性
来源：http://lwr.52xcode.cn

public readonly string $name
来源：http://qlr.tian-w.cn

[U50] PHP：构造器属性提升
来源：http://ocd.cqqwz.cn

public function __construct(private int $id) {}
来源：http://kti.ctjpmb.com

[U51] PHP：数组解构
来源：http://uoo.dianchejie.cn

[$a, $b] = $arr;
来源：http://klk.guowangkeji.top

[U52] PHP：箭头函数
来源：http://aqw.sysykeji.top

$double = fn($x) => $x * 2;
来源：http://ujl.zhengqikj.top

[U53] PHP：空合并运算符
来源：http://ouc.daria6918.cn

$v = $a ?? $b ?? "default";
来源：http://rft.xuanzx.com

[U54] PHP：空安全调用
来源：http://xzs.nwbrower.top

$obj?->method()
来源：http://cmr.jinqigufen.top

[U55] PHP：match 表达式
来源：http://fwp.hywenlv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sng.guannengcc.top

[U56] PHP：命名参数
来源：http://gle.xylfe.cn

f(a: 1, b: 2)
来源：http://bdk.jqgfzy.top

[U57] PHP：字符串插值
来源：http://wuj.aizwys.cn

"值: {$a}"
来源：http://mox.ivvv.top

[U58] PHP：数组三件套
来源：http://ypy.yuxming.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kzh.316326.xyz

[U59] PHP：自定义排序
来源：http://rxg.bjfxy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wmh.ydzc1.top

[U60] PHP：JSON 编解码
来源：http://sed.hnqzz.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tns.jinqigfzy.top

[U61] PHP：正则
来源：http://hdr.yuxming.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sex.0kj1m.cn

[U62] PHP：日期对象
来源：http://ord.gzhubu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sgk.yj20258888.top

[U63] PHP：文件读写
来源：http://vpy.yongpay.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zlq.daxiang520.top

[U64] PHP：目录遍历
来源：http://pom.cucudq.cn

glob("dir/*.php");  scandir("dir");
来源：http://xkj.jinqigufen.top

[U65] PHP：会话
来源：http://til.gzhubu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ugi.ivvv.top

[U66] PHP：设置 Cookie
来源：http://qbb.shangyingyoupin.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qwv.ydjk.org.cn

[U67] PHP：处理文件上传
来源：http://ate.zdqjudy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rkz.yj20258888.top

[U68] PHP：PDO 连接
来源：http://klh.kuanghao11.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kfw.fehbvm.com


<!-- 参考信息 -->