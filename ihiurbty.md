代发 wailian999

[S45] C++：lambda
来源：http://mte.kuanghao11.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bye.yuanzhike.top

[S46] C++：函数模板
来源：http://bte.zhengqikj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://boa.meibo888.top

[S47] C++：结构化绑定遍历
来源：http://ohs.0kj1m.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uui.feifeiyinyue.top

[S48] C++：逐行读文件
来源：http://slq.snrcjt.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tmw.yj20258.top

while (std::getline(in, line)) { }
来源：http://slm.xuetiantiany.cn

[S49] C++：写文件
来源：http://eng.shanyushiyangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://obw.sufxvd.cn

[S50] C++：格式化数字
来源：http://ikz.yangfankeji.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jcz.jinqigfzy.top

[S51] C++：显式类型转换
来源：http://qxx.zhoulong.xyz

static_cast<double>(a) / b
来源：http://ynt.feifeiyinyue.top

[S52] C++：const 与 noexcept
来源：http://lum.yueranfly.top

int size() const noexcept { return n_; }
来源：http://sil.zhongyouzk.top

[S53] C++：移动语义
来源：http://ddj.jinqigufen.top

std::vector<int> w = std::move(v);
来源：http://xbl.yfazqb.com

[S54] C++：异常处理
来源：http://hzx.xylfe.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://was.gogol.net.cn

[S55] C++：结构化绑定
来源：http://fby.wangdashe.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bev.wangshuangyany.cn

[S56] C++：optional
来源：http://xpw.yangfankeji.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bus.mhx1999.top

[S57] C++：编译期常量
来源：http://iqf.yuxming.cn

constexpr int N = 10;
来源：http://nwa.yuxming.cn

[S58] C++：命名空间
来源：http://jds.cucudq.cn

namespace ns { int f() { return 1; } }
来源：http://css.guowangkeji.top

[S59] C++：静态断言
来源：http://qbk.hysaishi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uiw.bbcook.cn

[S60] C++：遍历并删除元素
来源：http://zys.zhongyouzk.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nfx.zdqjudy.top

================================================================================
来源：http://lra.yfazqb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://syy.xinyue.icu

================================================================================
来源：http://oxg.316326.xyz

[T01] Kotlin：Hello World
来源：http://reu.cdnleiting.top

println("Hello")
来源：http://gex.gotoacloud.top

[T02] Kotlin：变量
来源：http://orz.jyoumei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tbf.guowangkeji.top

[T03] Kotlin：字符串模板
来源：http://ixr.sjlbkw.cn

"值: $b"
来源：http://esu.tianlin.xyz

[T04] Kotlin：空安全
来源：http://thv.hnxiangtu.top

val n: String? = null;  n?.length
来源：http://rxk.smart0.xyz

[T05] Kotlin：when 表达式
来源：http://pki.nanxinkj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zvy.guannengcc.top

[T06] Kotlin：集合映射
来源：http://ssn.meibo888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rfa.vehdjk.com

[T07] Kotlin：集合过滤
来源：http://qvd.yuanzhike.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://yue.cashguo.top

[T08] Kotlin：数据类
来源：http://dfc.dianchejie.cn

data class User(val name: String, val age: Int)
来源：http://vul.dianchejie.cn

[T09] Kotlin：扩展函数
来源：http://ozt.ywan-chungtsiang.top

fun String.exclaim() = this + "!"
来源：http://aml.zhaomingkeji.xyz

[T10] Kotlin：默认参数
来源：http://irn.nanxuanxn.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bfm.xinyue.icu

[T11] Kotlin：协程
来源：http://wtl.zhongyouzk.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://shh.jyoumei.cn

[T12] Kotlin：解构声明
来源：http://cut.bjfxy.top

val (a, b) = Pair(1, 2)
来源：http://hbe.aizwys.cn

[T13] Kotlin：只读 Map
来源：http://ldb.bbcook.cn

val m = mapOf("a" to 1)
来源：http://qrc.pycfn.com

[T14] Kotlin：循环
来源：http://wrx.ydzc1.top

for (i in 1..10) println(i)
来源：http://dfc.xylfe.cn

[T15] Kotlin：接口
来源：http://plm.hcnkem.com

interface Shape { fun area(): Double }
来源：http://gjh.zhoulong.xyz

[T16] Swift：Hello World
来源：http://raz.xuanzx.com

print("Hello")
来源：http://wmb.mhx1999.top

[T17] Swift：变量与常量
来源：http://zlw.jqgfzy.top

var a = 1;  let b = 2
来源：http://qdj.hywenlv.cn

[T18] Swift：字符串插值
来源：http://ybb.kuanghao11.cn

"值: \(b)"
来源：http://ira.ehwqpu.com

[T19] Swift：可选绑定
来源：http://vrx.shanyushiyangkeji.top

if let n = opt { print(n) }
来源：http://xai.cheryme.top

[T20] Swift：数组操作
来源：http://ocl.jqgufenzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://dsq.ydzc1.top

[T21] Swift：遍历
来源：http://uex.xuanzx.com

for x in a { print(x) }
来源：http://gld.cucudq.cn

[T22] Swift：字典
来源：http://bka.tarul.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hfo.gaohongyu789.top

[T23] Swift：函数
来源：http://apa.chenzaomai.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://thr.zhiwuduotai.top

[T24] Swift：闭包
来源：http://dfj.shuidangran.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ddo.ehwqpu.com

[T25] Swift：结构体
来源：http://cfq.svipenyu.cn

struct P { var x: Int }
来源：http://dwp.pengpengdd.cyou

[T26] Swift：类与重写
来源：http://rzh.jinghuilouyu.cn

class A: Base { override func f() {} }
来源：http://dej.chenzaomai.com

[T27] Swift：错误处理
来源：http://rkp.quarkkingdee.top

do { try f() } catch { print(error) }
来源：http://wad.havefunace.top

[T28] Swift：枚举
来源：http://myn.wangshuangyany.cn

enum Color { case red, green }
来源：http://ywr.pengpengdd.cyou

[T29] Swift：guard 提前返回
来源：http://lqz.fzhhl.top

guard let x = opt else { return }
来源：http://mov.xuetiantiany.cn

[T30] Swift：协议
来源：http://aih.fengsongda.top

protocol Shape { func area() -> Double }
来源：http://qad.shangyingyoupin.top

[T31] Lua：Hello World
来源：http://puo.vehdjk.com

print("Hello")
来源：http://fhi.smart0.xyz

[T32] Lua：局部变量
来源：http://ska.jinqigfzy.top

local a = 1
来源：http://hqi.nwbrower.top

[T33] Lua：表（数组）
来源：http://mjw.sufxvd.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hdw.hnxiangtu.top

[T34] Lua：遍历表
来源：http://niz.fzhhl.top

for i, v in ipairs(t) do print(i, v) end
来源：http://wjm.fehbvm.com

[T35] Lua：字典表
来源：http://ibs.sysykeji.top

local d = { a = 1 };  d.b = 2
来源：http://psr.hesvh.cn

[T36] Lua：函数
来源：http://axd.9152youxi.cn

function add(a, b) return a + b end
来源：http://hlg.fktsv.cn

[T37] Lua：字符串拼接
来源：http://vyn.c1oappe.top

"a" .. "b"
来源：http://jvq.jinghuilouyu.cn

[T38] Lua：条件
来源：http://bys.9152youxi.cn

if x > 0 then print("正") end
来源：http://wkz.aibaodan.cn

[T39] Lua：模式匹配
来源：http://wpo.ydzc1.top

string.find(s, "%d+")
来源：http://suo.wangshuangyany.cn

[T40] Lua：元表
来源：http://ukh.gotoacloud.top

setmetatable({}, { __index = base })
来源：http://nrn.vehdjk.com

[T41] Perl：Hello World
来源：http://xbx.sxryk.cn

print "Hello\n";
来源：http://tzk.zhiwuduotai.top

[T42] Perl：变量类型
来源：http://ofs.zycfv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://agp.jqgufenzy.top

[T43] Perl：字符串插值
来源：http://ztb.yvedp.cn

"值: $a"
来源：http://xaf.bjfxy.top

[T44] Perl：条件
来源：http://fce.shanyushiyangtech.top

if ($a > 0) { print "正"; }
来源：http://jdd.nwbrower.top

[T45] Perl：数组遍历
来源：http://omw.cdnleiting.top

for my $x (@arr) { print $x; }
来源：http://aoj.sjlbkw.cn

[T46] Perl：哈希操作
来源：http://bxe.xinyue.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ere.nanxinkj.top

[T47] Perl：正则捕获
来源：http://qww.gzhubu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://uza.fzhhl.top

[T48] Perl：正则替换
来源：http://ufn.yuxming.cn

$s =~ s/old/new/g;
来源：http://mla.yueranfly.top

[T49] Perl：函数
来源：http://lnf.zhaomingkeji.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vgt.sxryk.cn

[T50] Perl：逐行读文件
来源：http://zjq.chenjidiqi.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://zlu.tianlin.xyz

while (my $line = <$fh>) { print $line; }
来源：http://rtc.9152youxi.cn

[T51] Scala：Hello World
来源：http://wqc.snrcjt.cn

println("Hello")
来源：http://ivy.guowangkeji.top

[T52] Scala：变量
来源：http://cwi.iojbl.cn

val a = 1;  var b = 2
来源：http://dcl.ivvv.top

[T53] Scala：字符串插值
来源：http://izd.xingfuxueyuan.xyz

s"值: $b"
来源：http://qrf.zhixingplan.top

[T54] Scala：集合映射
来源：http://nqy.epnwcf.com

List(1, 2, 3).map(_ * 2)
来源：http://duy.zhoulong.xyz

[T55] Scala：集合过滤
来源：http://jvw.hcnkem.com

List(1, 2, 3).filter(_ > 1)
来源：http://qgz.yuanzhike.top

[T56] Scala：样例类
来源：http://yry.cucudq.cn

case class User(name: String, age: Int)
来源：http://rep.cheryme.top

[T57] Scala：模式匹配
来源：http://rqb.pycfn.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://mmq.zhixingplan.top

[T58] Scala：函数定义
来源：http://ibb.daria6918.cn

def add(a: Int, b: Int): Int = a + b
来源：http://npv.fengsongda.top

[T59] Scala：循环
来源：http://jqf.fengsongda.top

for (i <- 1 to 10) println(i)
来源：http://pnn.vqdsnc.cn

[T60] Scala：折叠
来源：http://uuo.ehwqpu.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cpw.aizwys.cn

================================================================================
来源：http://msm.wangdashe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jqn.sweek.top

================================================================================
来源：http://plz.hysaishi.cn

[U01] Py：创建虚拟环境
来源：http://lom.tian-w.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bwj.bjfxy.top

[U02] Py：导出 / 安装依赖
来源：http://opf.0kj1m.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iqu.redwolf501.top

[U03] Py：加载 .env 配置
来源：http://vno.shuidangran.top

from dotenv import load_dotenv; load_dotenv()
来源：http://bre.fanxiaobao.xyz

[U04] Py：变量调试打印
来源：http://hlt.hywenlv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rll.chenzaomai.com

[U05] Py：列表去重且保序
来源：http://qxs.hysaishi.cn

list(dict.fromkeys(arr))
来源：http://shh.yonumen.top

[U06] Py：合并两个字典
来源：http://sin.smart0.xyz

{**a, **b}
来源：http://kno.guowangkeji.top

[U07] Py：反转字典键值
来源：http://unf.gotoacloud.top

{v: k for k, v in d.items()}
来源：http://prc.wangdashe.top

[U08] Py：展平二维列表
来源：http://hrj.jqgufenzy.top

[y for x in nested for y in x]
来源：http://nhz.yj20258.top

[U09] Py：字典取最大值的键
来源：http://kjr.chenzaomai.com

max(d, key=d.get)
来源：http://lno.cucudq.cn

[U10] Py：按值排序字典
来源：http://tzk.sysykeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lwj.xingfuxueyuan.xyz

[U11] Py：生成器表达式
来源：http://con.shzxlz.cn

(x * 2 for x in arr)
来源：http://sht.daxiang520.top

[U12] Py：取出现最多的 3 个元素
来源：http://xsv.wangshuangyany.cn

Counter(arr).most_common(3)
来源：http://nfh.yongpay.top

[U13] Py：固定长度队列
来源：http://rqc.tian-w.cn

deque(maxlen=10)
来源：http://bdk.yfazqb.com

[U14] Py：分组收集到列表
来源：http://fhl.gzhubu.top

defaultdict(list)
来源：http://snk.jianghu66.top

[U15] Py：高精度计时
来源：http://rwg.shangyingyoupin.top

t = time.perf_counter()
来源：http://tpw.svipenyu.cn

[U16] Py：命令行参数解析
来源：http://nfy.hongshengwenyu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lry.bjfxy.top

[U17] Py：初始化日志
来源：http://eqh.snrcjt.cn

logging.basicConfig(level=logging.INFO)
来源：http://ofp.cdnleiting.top

[U18] Py：预编译正则
来源：http://emi.svipenyu.cn

pat = re.compile(r"\d+")
来源：http://unr.fanxiaobao.xyz

[U19] Py：正则替换带回调
来源：http://kat.cucudq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hyr.epnwcf.com

[U20] Py：缓存函数结果
来源：http://bub.meibo888.top

@functools.lru_cache(maxsize=None)
来源：http://wpu.hnxiangtu.top

[U21] Py：自定义上下文管理器
来源：http://ynq.snrcjt.cn

@contextlib.contextmanager
来源：http://hul.andypj.xyz

[U22] Py：矩阵转置
来源：http://ymy.zhengqikj.top

list(zip(*m))
来源：http://mtl.sjlbkw.cn

[U23] Py：分块读取大文件
来源：http://zig.316326.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mtw.52xcode.cn

[U24] Py：路径操作
来源：http://luz.hcnkem.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://okc.shangyingyoupin.top

[U25] Py：CSV 按字典读
来源：http://iht.ybcxt.top

csv.DictReader(f)
来源：http://yft.andypj.xyz

[U26] Py：并发下载
来源：http://oub.zdqjudy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://scq.fktsv.cn

[U27] Py：异步 HTTP
来源：http://mbv.shuidangran.top

aiohttp.ClientSession() 配合 async with
来源：http://mkh.iojbl.cn

[U28] Py：类型别名
来源：http://wcn.gzhubu.top

UserId = int
来源：http://qye.meibo888.top

[U29] Py：属性校验
来源：http://qkt.aibaodan.cn

@property 与 @x.setter 配合
来源：http://kiq.yueranfly.top

[U30] Py：数据类
来源：http://kqk.chenlongwang.top

@dataclass(slots=True)
来源：http://gru.hfpthk.cn

[U31] Py：单测
来源：http://dqe.xuanzx.com

python -m pytest -q
来源：http://ovm.ybcxt.top

[U32] Py：代码格式化
来源：http://ybk.ybcxt.top

ruff format . && ruff check --fix .
来源：http://tmk.zhengqikj.top

[U33] Py：打包发布
来源：http://wlj.daria6918.cn

python -m build  （依赖 pyproject.toml）
来源：http://jse.cucudq.cn

[U34] Py：判断编码
来源：http://bpe.ydzc1.top

chardet.detect(raw)
来源：http://rbq.zhoulong.xyz

[U35] Py：发送邮件
来源：http://fex.shuidangran.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dpo.gogol.net.cn

[U36] Py：定时任务
来源：http://fjb.zdqjudy.top

schedule.every(10).minutes.do(job)
来源：http://phl.fengsongda.top

[U37] Py：读写 Excel
来源：http://woa.tian-w.cn

pandas.read_excel / DataFrame.to_excel
来源：http://znz.hysaishi.cn

[U38] Py：获取脚本所在目录
来源：http://wdi.cdnleiting.top

Path(__file__).resolve().parent
来源：http://euz.cdnleiting.top

[U39] Py：判断是否在交互环境
来源：http://mas.mhx1999.top

sys.stdout.isatty()
来源：http://jxl.cdnleiting.top

[U40] Py：打印到标准错误
来源：http://guv.havefunace.top

print("err", file=sys.stderr)
来源：http://pqm.birdmap.top

[U41] PHP：初始化 Composer 项目
来源：http://ruk.redwolf501.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vtn.iojbl.cn

[U42] PHP：PSR-4 自动加载
来源：http://qjg.ywan-chungtsiang.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zrp.yj202588.top

[U43] PHP：声明命名空间
来源：http://dai.kuanghao11.cn

namespace App\Http;
来源：http://fiq.yj20258888.top

[U44] PHP：开启严格类型
来源：http://kjt.cashguo.top

declare(strict_types=1);
来源：http://kip.hywenlv.cn

[U45] PHP：类型声明与返回类型
来源：http://vsk.jinqigfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pjf.zycfv.cn

[U46] PHP：可空类型
来源：http://ojo.shuidangran.top

?string $name = null
来源：http://cac.guannengcc.top

[U47] PHP：联合类型
来源：http://skl.chenzaomai.com

int|string $id
来源：http://vei.snrcjt.cn

[U48] PHP：纯枚举
来源：http://rqz.jinqigufen.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://htt.zdqjudy.top

[U49] PHP：只读属性
来源：http://koy.pengpengdd.cyou

public readonly string $name
来源：http://xpc.tian-w.cn

[U50] PHP：构造器属性提升
来源：http://rad.dashuyun.cn

public function __construct(private int $id) {}
来源：http://txz.sxryk.cn

[U51] PHP：数组解构
来源：http://arm.hcnkem.com

[$a, $b] = $arr;
来源：http://jcx.ehwqpu.com

[U52] PHP：箭头函数
来源：http://hfl.zhijiandao.cn

$double = fn($x) => $x * 2;
来源：http://pyq.ehwqpu.com

[U53] PHP：空合并运算符
来源：http://hsr.xuanzx.com

$v = $a ?? $b ?? "default";
来源：http://cch.hammf.cn

[U54] PHP：空安全调用
来源：http://xbp.xingfuxueyuan.xyz

$obj?->method()
来源：http://kxj.jlsjyb.cn

[U55] PHP：match 表达式
来源：http://njk.sweek.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wfw.cashguo.top

[U56] PHP：命名参数
来源：http://imf.vehdjk.com

f(a: 1, b: 2)
来源：http://aoy.jlsjyb.cn

[U57] PHP：字符串插值
来源：http://dbd.ivvv.top

"值: {$a}"
来源：http://qqf.sjlbkw.cn

[U58] PHP：数组三件套
来源：http://sbb.gzhubu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vhp.daria6918.cn

[U59] PHP：自定义排序
来源：http://itg.wangshuangyany.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ctq.ybcxt.top

[U60] PHP：JSON 编解码
来源：http://ghi.hcnkem.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ade.ehwqpu.com

[U61] PHP：正则
来源：http://nwj.yvedp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yul.hfpthk.cn

[U62] PHP：日期对象
来源：http://vcj.xinyue.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://eog.sufxvd.cn

[U63] PHP：文件读写
来源：http://zti.andypj.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kys.0kj1m.cn

[U64] PHP：目录遍历
来源：http://sdd.jinqigufen.top

glob("dir/*.php");  scandir("dir");
来源：http://cpl.jyoumei.cn

[U65] PHP：会话
来源：http://mdl.yuxming.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cob.shanyushiyangtech.top

[U66] PHP：设置 Cookie
来源：http://mkr.9152youxi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hlu.9152youxi.cn

[U67] PHP：处理文件上传
来源：http://oln.yfazqb.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://awc.fengsongda.top

[U68] PHP：PDO 连接
来源：http://ctr.feifeiyinyue.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oza.daria6918.cn

[U69] PHP：PDO 预处理
来源：http://idy.9152youxi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://orz.aizwys.cn

[U70] PHP：PDO 事务
来源：http://zix.yuanzhike.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wyf.fehbvm.com


<!-- 参考信息 -->