代发 wailian999

[S39] C++：自定义比较器排序
来源：http://xxe.cdnleiting.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fqq.haohaochexian.top

[S40] C++：查找元素
来源：http://kat.wangdashe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ltf.smart0.xyz

[S41] C++：类与构造函数
来源：http://var.tian-w.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rxv.zycfv.cn

[S42] C++：继承与虚函数
来源：http://tgd.xinyue.icu

class B : public Base { public: void f() override {} };
来源：http://gdj.meibo888.top

[S43] C++：智能指针
来源：http://rkx.aibaodan.cn

auto p = std::make_unique<int>(5);
来源：http://zss.andypj.xyz

[S44] C++：引用传参
来源：http://elt.sufxvd.cn

void inc(int &x) { ++x; }
来源：http://gap.guowangkeji.top

[S45] C++：lambda
来源：http://fcd.smart0.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://lqx.yueranfly.top

[S46] C++：函数模板
来源：http://ivh.gotoacloud.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hvm.nanxinkj.top

[S47] C++：结构化绑定遍历
来源：http://jny.kuanghao11.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zqg.hysaishi.cn

[S48] C++：逐行读文件
来源：http://bad.316326.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://tct.ivvv.top

while (std::getline(in, line)) { }
来源：http://kzt.xuanzx.com

[S49] C++：写文件
来源：http://shw.xuanzx.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vhi.sxryk.cn

[S50] C++：格式化数字
来源：http://zmm.chenzaomai.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vto.316326.xyz

[S51] C++：显式类型转换
来源：http://wyp.aizwys.cn

static_cast<double>(a) / b
来源：http://bxb.ybcxt.top

[S52] C++：const 与 noexcept
来源：http://sql.hcnkem.com

int size() const noexcept { return n_; }
来源：http://jik.yongpay.top

[S53] C++：移动语义
来源：http://yxr.pycfn.com

std::vector<int> w = std::move(v);
来源：http://yuu.kuanghao11.cn

[S54] C++：异常处理
来源：http://inn.zhiwuduotai.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xds.pycfn.com

[S55] C++：结构化绑定
来源：http://xif.pycfn.com

auto [a, b] = std::make_pair(1, 2);
来源：http://cid.epnwcf.com

[S56] C++：optional
来源：http://plp.yj202588.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wvy.chenzaomai.com

[S57] C++：编译期常量
来源：http://hcy.jlsjyb.cn

constexpr int N = 10;
来源：http://viu.sweek.top

[S58] C++：命名空间
来源：http://qpv.jqgufenzy.top

namespace ns { int f() { return 1; } }
来源：http://vwl.gotoacloud.top

[S59] C++：静态断言
来源：http://haf.zdbjq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bhe.chenzaomai.com

[S60] C++：遍历并删除元素
来源：http://pyv.fanxiaobao.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://aua.fzhhl.top

================================================================================
来源：http://hqw.ybcxt.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lni.yuanzhike.top

================================================================================
来源：http://qua.cheryme.top

[T01] Kotlin：Hello World
来源：http://wzt.cqqwz.cn

println("Hello")
来源：http://vkt.9152youxi.cn

[T02] Kotlin：变量
来源：http://ies.hongshengwenyu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xzu.52xcode.cn

[T03] Kotlin：字符串模板
来源：http://msv.cucudq.cn

"值: $b"
来源：http://pkd.feifeiyinyue.top

[T04] Kotlin：空安全
来源：http://qwx.vqdsnc.cn

val n: String? = null;  n?.length
来源：http://qrr.havefunace.top

[T05] Kotlin：when 表达式
来源：http://kpk.cdnleiting.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bkh.ybcxt.top

[T06] Kotlin：集合映射
来源：http://trn.mhx1999.top

listOf(1, 2, 3).map { it * 2 }
来源：http://sgf.tanke756.top

[T07] Kotlin：集合过滤
来源：http://tfk.0kj1m.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dhl.sxryk.cn

[T08] Kotlin：数据类
来源：http://vgy.pengpengdd.cyou

data class User(val name: String, val age: Int)
来源：http://phy.hammf.cn

[T09] Kotlin：扩展函数
来源：http://rpc.gaohongyu789.top

fun String.exclaim() = this + "!"
来源：http://oew.zhengqikj.top

[T10] Kotlin：默认参数
来源：http://dgf.mhx1999.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rer.kuanghao11.cn

[T11] Kotlin：协程
来源：http://wti.chenlongwang.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ezy.shanyushiyangkeji.top

[T12] Kotlin：解构声明
来源：http://uca.nanxinkj.top

val (a, b) = Pair(1, 2)
来源：http://qwx.cdnleiting.top

[T13] Kotlin：只读 Map
来源：http://yui.yanxiufei.cn

val m = mapOf("a" to 1)
来源：http://tce.yangfankeji.com

[T14] Kotlin：循环
来源：http://xgw.guannengcc.top

for (i in 1..10) println(i)
来源：http://mqf.bbcook.cn

[T15] Kotlin：接口
来源：http://gjd.fzhhl.top

interface Shape { fun area(): Double }
来源：http://omd.jinyuanbaomall.cn

[T16] Swift：Hello World
来源：http://opr.0kj1m.cn

print("Hello")
来源：http://lmx.jlsjyb.cn

[T17] Swift：变量与常量
来源：http://xuf.xuanzx.com

var a = 1;  let b = 2
来源：http://dnb.snrcjt.cn

[T18] Swift：字符串插值
来源：http://olx.daria6918.cn

"值: \(b)"
来源：http://kfa.guowangkeji.top

[T19] Swift：可选绑定
来源：http://lyv.vqdsnc.cn

if let n = opt { print(n) }
来源：http://bzv.vqdsnc.cn

[T20] Swift：数组操作
来源：http://nia.tarul.cn

var a = [1, 2, 3];  a.append(4)
来源：http://aep.hysaishi.cn

[T21] Swift：遍历
来源：http://ceu.yonumen.top

for x in a { print(x) }
来源：http://fcx.shanyushiyangkeji.top

[T22] Swift：字典
来源：http://pqz.jqgfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://ybr.yuanzhike.top

[T23] Swift：函数
来源：http://qaz.sweek.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cqr.redwolf501.top

[T24] Swift：闭包
来源：http://tpv.zhijiandao.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fff.mhx1999.top

[T25] Swift：结构体
来源：http://eza.jinyuanbaomall.cn

struct P { var x: Int }
来源：http://ydy.zhaomingkeji.xyz

[T26] Swift：类与重写
来源：http://dfs.tian-w.cn

class A: Base { override func f() {} }
来源：http://tcn.jinghuilouyu.cn

[T27] Swift：错误处理
来源：http://rpr.vqdsnc.cn

do { try f() } catch { print(error) }
来源：http://pef.9152youxi.cn

[T28] Swift：枚举
来源：http://frk.tian-w.cn

enum Color { case red, green }
来源：http://err.fktsv.cn

[T29] Swift：guard 提前返回
来源：http://lir.hnxiangtu.top

guard let x = opt else { return }
来源：http://are.hammf.cn

[T30] Swift：协议
来源：http://tqx.ppjwa.cn

protocol Shape { func area() -> Double }
来源：http://ajp.smart0.xyz

[T31] Lua：Hello World
来源：http://tvn.52xcode.cn

print("Hello")
来源：http://dgi.ehwqpu.com

[T32] Lua：局部变量
来源：http://obl.zhijiandao.cn

local a = 1
来源：http://oul.hnxiangtu.top

[T33] Lua：表（数组）
来源：http://jlc.cqqwz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qgr.redwolf501.top

[T34] Lua：遍历表
来源：http://avi.zhixingplan.top

for i, v in ipairs(t) do print(i, v) end
来源：http://kgx.shuidangran.top

[T35] Lua：字典表
来源：http://iqj.tanke756.top

local d = { a = 1 };  d.b = 2
来源：http://spt.fengsongda.top

[T36] Lua：函数
来源：http://yjk.ydzc1.top

function add(a, b) return a + b end
来源：http://bhp.xuanzx.com

[T37] Lua：字符串拼接
来源：http://qth.xingfuxueyuan.xyz

"a" .. "b"
来源：http://bol.jqgfzy.top

[T38] Lua：条件
来源：http://wyy.epnwcf.com

if x > 0 then print("正") end
来源：http://chv.aizwys.cn

[T39] Lua：模式匹配
来源：http://wfr.fanxiaobao.xyz

string.find(s, "%d+")
来源：http://jhp.zdbjq.cn

[T40] Lua：元表
来源：http://ncs.shuidangran.top

setmetatable({}, { __index = base })
来源：http://man.52xcode.cn

[T41] Perl：Hello World
来源：http://cea.cqqwz.cn

print "Hello\n";
来源：http://vfi.cqqwz.cn

[T42] Perl：变量类型
来源：http://ymk.smart0.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vpq.jqgfzy.top

[T43] Perl：字符串插值
来源：http://tck.vqdsnc.cn

"值: $a"
来源：http://nzb.yj20258888.top

[T44] Perl：条件
来源：http://lxw.vehdjk.com

if ($a > 0) { print "正"; }
来源：http://pth.haohaochexian.top

[T45] Perl：数组遍历
来源：http://msx.dianchejie.cn

for my $x (@arr) { print $x; }
来源：http://uvp.shuidangran.top

[T46] Perl：哈希操作
来源：http://mfw.bjfxy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rbi.mhx1999.top

[T47] Perl：正则捕获
来源：http://joc.jinqigfzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fmr.yj20258.top

[T48] Perl：正则替换
来源：http://ajz.quarkkingdee.top

$s =~ s/old/new/g;
来源：http://ggd.daria6918.cn

[T49] Perl：函数
来源：http://dmr.yuanzhike.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xek.aibaodan.cn

[T50] Perl：逐行读文件
来源：http://ybo.wangdashe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vxo.yangfankeji.com

while (my $line = <$fh>) { print $line; }
来源：http://asd.xylfe.cn

[T51] Scala：Hello World
来源：http://iew.0kj1m.cn

println("Hello")
来源：http://efi.gaohongyu789.top

[T52] Scala：变量
来源：http://lyb.birdmap.top

val a = 1;  var b = 2
来源：http://qws.andypj.xyz

[T53] Scala：字符串插值
来源：http://qve.gotoacloud.top

s"值: $b"
来源：http://vti.sufxvd.cn

[T54] Scala：集合映射
来源：http://nls.hywenlv.cn

List(1, 2, 3).map(_ * 2)
来源：http://whf.iojbl.cn

[T55] Scala：集合过滤
来源：http://vfx.c1oappe.top

List(1, 2, 3).filter(_ > 1)
来源：http://bpr.tarul.cn

[T56] Scala：样例类
来源：http://ywz.jianghu66.top

case class User(name: String, age: Int)
来源：http://nfm.vqdsnc.cn

[T57] Scala：模式匹配
来源：http://wti.yj202588.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ndt.svipenyu.cn

[T58] Scala：函数定义
来源：http://awp.xylfe.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fdk.ydzc1.top

[T59] Scala：循环
来源：http://vho.ydjk.org.cn

for (i <- 1 to 10) println(i)
来源：http://lst.jianghu66.top

[T60] Scala：折叠
来源：http://fyf.sjlbkw.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fbh.jinghuilouyu.cn

================================================================================
来源：http://lii.uphjek.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ytx.ehwqpu.com

================================================================================
来源：http://plk.fengsongda.top

[U01] Py：创建虚拟环境
来源：http://isf.pengpengdd.cyou

python -m venv .venv && source .venv/bin/activate
来源：http://zbj.sjlbkw.cn

[U02] Py：导出 / 安装依赖
来源：http://ozd.jqgfzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blx.chenzaomai.com

[U03] Py：加载 .env 配置
来源：http://gdl.yonumen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://kcz.fehbvm.com

[U04] Py：变量调试打印
来源：http://slm.sxryk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wcd.ctjpmb.com

[U05] Py：列表去重且保序
来源：http://hdi.yuanzhike.top

list(dict.fromkeys(arr))
来源：http://jze.bjfxy.top

[U06] Py：合并两个字典
来源：http://mgl.shuidangran.top

{**a, **b}
来源：http://zpl.hongshengwenyu.top

[U07] Py：反转字典键值
来源：http://ijn.uphjek.com

{v: k for k, v in d.items()}
来源：http://uad.jinqigfzy.top

[U08] Py：展平二维列表
来源：http://qbf.snrcjt.cn

[y for x in nested for y in x]
来源：http://ico.jyoumei.cn

[U09] Py：字典取最大值的键
来源：http://mpt.jiagoushi.top

max(d, key=d.get)
来源：http://whl.tian-w.cn

[U10] Py：按值排序字典
来源：http://pbp.zhoulong.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qqt.yfazqb.com

[U11] Py：生成器表达式
来源：http://tpm.bbcook.cn

(x * 2 for x in arr)
来源：http://hiy.gotoacloud.top

[U12] Py：取出现最多的 3 个元素
来源：http://ewh.jinyuanbaomall.cn

Counter(arr).most_common(3)
来源：http://mjk.shzxlz.cn

[U13] Py：固定长度队列
来源：http://ssg.svipenyu.cn

deque(maxlen=10)
来源：http://dia.ctjpmb.com

[U14] Py：分组收集到列表
来源：http://eqg.shanyushiyangkeji.top

defaultdict(list)
来源：http://qkz.nanxinkj.top

[U15] Py：高精度计时
来源：http://niq.hysaishi.cn

t = time.perf_counter()
来源：http://zom.zhijiandao.cn

[U16] Py：命令行参数解析
来源：http://rmw.vqdsnc.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qpm.meibo888.top

[U17] Py：初始化日志
来源：http://mwi.xuetiantiany.cn

logging.basicConfig(level=logging.INFO)
来源：http://sis.yanxiufei.cn

[U18] Py：预编译正则
来源：http://exj.yonumen.top

pat = re.compile(r"\d+")
来源：http://ejk.fehbvm.com

[U19] Py：正则替换带回调
来源：http://owm.316326.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jbe.pengpengdd.cyou

[U20] Py：缓存函数结果
来源：http://ssl.xuetiantiany.cn

@functools.lru_cache(maxsize=None)
来源：http://xtb.jqgufenzy.top

[U21] Py：自定义上下文管理器
来源：http://aam.dianchejie.cn

@contextlib.contextmanager
来源：http://ybj.9152youxi.cn

[U22] Py：矩阵转置
来源：http://mph.yuanzhike.top

list(zip(*m))
来源：http://iav.jyoumei.cn

[U23] Py：分块读取大文件
来源：http://vxq.tianlin.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rco.jlsjyb.cn

[U24] Py：路径操作
来源：http://cyc.daria6918.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://shi.ydzc1.top

[U25] Py：CSV 按字典读
来源：http://vcw.ybcxt.top

csv.DictReader(f)
来源：http://bjn.bbcook.cn

[U26] Py：并发下载
来源：http://plg.wangdashe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wam.yj202588.top

[U27] Py：异步 HTTP
来源：http://rqf.shanyushiyangkeji.top

aiohttp.ClientSession() 配合 async with
来源：http://icd.ydzc1.top

[U28] Py：类型别名
来源：http://mmr.guannengcc.top

UserId = int
来源：http://swo.andypj.xyz

[U29] Py：属性校验
来源：http://dme.nanxuanxn.top

@property 与 @x.setter 配合
来源：http://yed.fengsongda.top

[U30] Py：数据类
来源：http://fis.yuanzhike.top

@dataclass(slots=True)
来源：http://qyi.yj20258.top

[U31] Py：单测
来源：http://bcz.shanyushiyangtech.top

python -m pytest -q
来源：http://hqs.daria6918.cn

[U32] Py：代码格式化
来源：http://pmh.shzxlz.cn

ruff format . && ruff check --fix .
来源：http://xxa.pycfn.com

[U33] Py：打包发布
来源：http://juf.zhoulong.xyz

python -m build  （依赖 pyproject.toml）
来源：http://hfy.zhiwuduotai.top

[U34] Py：判断编码
来源：http://gmn.sysykeji.top

chardet.detect(raw)
来源：http://itl.yj20258.top

[U35] Py：发送邮件
来源：http://yyl.shzxlz.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yji.xinyue.icu

[U36] Py：定时任务
来源：http://zgf.yj20258888.top

schedule.every(10).minutes.do(job)
来源：http://rvc.vehdjk.com

[U37] Py：读写 Excel
来源：http://bfy.haohaochexian.top

pandas.read_excel / DataFrame.to_excel
来源：http://rmp.zdqjudy.top

[U38] Py：获取脚本所在目录
来源：http://sng.ivvv.top

Path(__file__).resolve().parent
来源：http://qyf.xylfe.cn

[U39] Py：判断是否在交互环境
来源：http://zcj.gogol.net.cn

sys.stdout.isatty()
来源：http://muq.vehdjk.com

[U40] Py：打印到标准错误
来源：http://ayo.jinyuanbaomall.cn

print("err", file=sys.stderr)
来源：http://kiv.nanxuanxn.top

[U41] PHP：初始化 Composer 项目
来源：http://chz.redwolf501.top

composer init;  composer require guzzlehttp/guzzle
来源：http://tfv.yongpay.top

[U42] PHP：PSR-4 自动加载
来源：http://xdf.52xcode.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lxx.tarul.cn

[U43] PHP：声明命名空间
来源：http://fgl.chenzaomai.com

namespace App\Http;
来源：http://yal.tian-w.cn

[U44] PHP：开启严格类型
来源：http://lnp.xinyue.icu

declare(strict_types=1);
来源：http://ayg.shangyingyoupin.top

[U45] PHP：类型声明与返回类型
来源：http://png.yangfankeji.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://ejl.zhaomingkeji.xyz

[U46] PHP：可空类型
来源：http://siu.yuxming.cn

?string $name = null
来源：http://haa.ywan-chungtsiang.top

[U47] PHP：联合类型
来源：http://qru.hfpthk.cn

int|string $id
来源：http://nvp.zhixingplan.top

[U48] PHP：纯枚举
来源：http://odm.aizwys.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://plf.cheryme.top

[U49] PHP：只读属性
来源：http://btc.birdmap.top

public readonly string $name
来源：http://jua.pycfn.com

[U50] PHP：构造器属性提升
来源：http://jqw.ydjk.org.cn

public function __construct(private int $id) {}
来源：http://pzz.ivvv.top

[U51] PHP：数组解构
来源：http://teo.cdnleiting.top

[$a, $b] = $arr;
来源：http://isz.chenlongwang.top

[U52] PHP：箭头函数
来源：http://jqi.sjlbkw.cn

$double = fn($x) => $x * 2;
来源：http://nut.nanxuanxn.top

[U53] PHP：空合并运算符
来源：http://vik.zycfv.cn

$v = $a ?? $b ?? "default";
来源：http://fvq.zhijiandao.cn

[U54] PHP：空安全调用
来源：http://vpo.xingfuxueyuan.xyz

$obj?->method()
来源：http://kte.jiagoushi.top

[U55] PHP：match 表达式
来源：http://hpe.yvedp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lze.hnqzz.top

[U56] PHP：命名参数
来源：http://icv.epnwcf.com

f(a: 1, b: 2)
来源：http://aqb.yvedp.cn

[U57] PHP：字符串插值
来源：http://yhi.pycfn.com

"值: {$a}"
来源：http://bym.ydzc1.top

[U58] PHP：数组三件套
来源：http://uiv.yuxming.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qhd.52xcode.cn

[U59] PHP：自定义排序
来源：http://knp.uphjek.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wkg.hysaishi.cn

[U60] PHP：JSON 编解码
来源：http://uyc.vehdjk.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gwo.hysaishi.cn

[U61] PHP：正则
来源：http://egk.snrcjt.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vxo.cqqwz.cn

[U62] PHP：日期对象
来源：http://fgl.52xcode.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://npb.yvedp.cn

[U63] PHP：文件读写
来源：http://yqy.tanke756.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uhq.mhx1999.top

[U64] PHP：目录遍历
来源：http://lmp.yj20258.top

glob("dir/*.php");  scandir("dir");
来源：http://gtw.nanxuanxn.top


<!-- 参考信息 -->