代发 wailian999

[S43] C++：智能指针
来源：http://plt.ivvv.top

auto p = std::make_unique<int>(5);
来源：http://pnf.cashguo.top

[S44] C++：引用传参
来源：http://vii.hnqzz.top

void inc(int &x) { ++x; }
来源：http://uat.yonumen.top

[S45] C++：lambda
来源：http://bes.svipenyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dkv.jianghu66.top

[S46] C++：函数模板
来源：http://auk.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oar.smart0.xyz

[S47] C++：结构化绑定遍历
来源：http://vwm.chenlongwang.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lwh.jinqigfzy.top

[S48] C++：逐行读文件
来源：http://fps.jqgfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://vgh.yuanzhike.top

while (std::getline(in, line)) { }
来源：http://ypc.zycfv.cn

[S49] C++：写文件
来源：http://tlf.zdbjq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fje.ywan-chungtsiang.top

[S50] C++：格式化数字
来源：http://sye.cdnleiting.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qqg.zhengqikj.top

[S51] C++：显式类型转换
来源：http://vgh.hcnkem.com

static_cast<double>(a) / b
来源：http://ike.dianchejie.cn

[S52] C++：const 与 noexcept
来源：http://zij.gzhubu.top

int size() const noexcept { return n_; }
来源：http://rau.ywan-chungtsiang.top

[S53] C++：移动语义
来源：http://wbc.yanxiufei.cn

std::vector<int> w = std::move(v);
来源：http://tdr.yueranfly.top

[S54] C++：异常处理
来源：http://wpk.zhixingplan.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vyd.quarkkingdee.top

[S55] C++：结构化绑定
来源：http://tdy.gaohongyu789.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qgj.yonumen.top

[S56] C++：optional
来源：http://ttr.xinyue.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pbq.fzhhl.top

[S57] C++：编译期常量
来源：http://qrw.gaohongyu789.top

constexpr int N = 10;
来源：http://uuy.svipenyu.cn

[S58] C++：命名空间
来源：http://rgq.jinghuilouyu.cn

namespace ns { int f() { return 1; } }
来源：http://jzo.zhengqikj.top

[S59] C++：静态断言
来源：http://wsh.zhiwuduotai.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://igh.kuanghao11.cn

[S60] C++：遍历并删除元素
来源：http://iss.hywenlv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ezh.shangyingyoupin.top

================================================================================
来源：http://whm.vehdjk.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cfw.fktsv.cn

================================================================================
来源：http://vhk.316326.xyz

[T01] Kotlin：Hello World
来源：http://mtm.316326.xyz

println("Hello")
来源：http://ujw.nwbrower.top

[T02] Kotlin：变量
来源：http://lex.sjlbkw.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bis.tian-w.cn

[T03] Kotlin：字符串模板
来源：http://izi.hnxiangtu.top

"值: $b"
来源：http://byh.chenlongwang.top

[T04] Kotlin：空安全
来源：http://xbz.hammf.cn

val n: String? = null;  n?.length
来源：http://ddp.zhijiandao.cn

[T05] Kotlin：when 表达式
来源：http://foi.nwbrower.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hqy.jqgfzy.top

[T06] Kotlin：集合映射
来源：http://ltj.hesvh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qcy.tian-w.cn

[T07] Kotlin：集合过滤
来源：http://tfz.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vhe.jianghu66.top

[T08] Kotlin：数据类
来源：http://rnl.aibaodan.cn

data class User(val name: String, val age: Int)
来源：http://irq.xinyue.icu

[T09] Kotlin：扩展函数
来源：http://zcm.uphjek.com

fun String.exclaim() = this + "!"
来源：http://fuh.jinqigufen.top

[T10] Kotlin：默认参数
来源：http://gss.bbcook.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xyf.shanyushiyangtech.top

[T11] Kotlin：协程
来源：http://dol.jiagoushi.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://unv.xinyue.icu

[T12] Kotlin：解构声明
来源：http://lal.ywan-chungtsiang.top

val (a, b) = Pair(1, 2)
来源：http://fls.yuxming.cn

[T13] Kotlin：只读 Map
来源：http://lqc.hnxiangtu.top

val m = mapOf("a" to 1)
来源：http://wdy.gzhubu.top

[T14] Kotlin：循环
来源：http://ymm.shanyushiyangtech.top

for (i in 1..10) println(i)
来源：http://pys.yongpay.top

[T15] Kotlin：接口
来源：http://tbz.cashguo.top

interface Shape { fun area(): Double }
来源：http://kib.dianchejie.cn

[T16] Swift：Hello World
来源：http://yyn.iojbl.cn

print("Hello")
来源：http://rmw.ydjk.org.cn

[T17] Swift：变量与常量
来源：http://ugn.hcnkem.com

var a = 1;  let b = 2
来源：http://und.zycfv.cn

[T18] Swift：字符串插值
来源：http://tuz.zhaomingkeji.xyz

"值: \(b)"
来源：http://sml.sufxvd.cn

[T19] Swift：可选绑定
来源：http://ixg.haohaochexian.top

if let n = opt { print(n) }
来源：http://zuj.jqgufenzy.top

[T20] Swift：数组操作
来源：http://jyn.bjfxy.top

var a = [1, 2, 3];  a.append(4)
来源：http://gdp.fanxiaobao.xyz

[T21] Swift：遍历
来源：http://wow.guannengcc.top

for x in a { print(x) }
来源：http://vbh.jinqigufen.top

[T22] Swift：字典
来源：http://fxi.cdnleiting.top

var d = ["a": 1];  d["b"] = 2
来源：http://gjl.chenlongwang.top

[T23] Swift：函数
来源：http://rdn.xuetiantiany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://muk.ybcxt.top

[T24] Swift：闭包
来源：http://mgr.yvedp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vlg.hysaishi.cn

[T25] Swift：结构体
来源：http://tek.mhx1999.top

struct P { var x: Int }
来源：http://gut.ywan-chungtsiang.top

[T26] Swift：类与重写
来源：http://pys.zhiwuduotai.top

class A: Base { override func f() {} }
来源：http://eri.0kj1m.cn

[T27] Swift：错误处理
来源：http://oeq.nwbrower.top

do { try f() } catch { print(error) }
来源：http://gkn.jinyuanbaomall.cn

[T28] Swift：枚举
来源：http://iea.fzhhl.top

enum Color { case red, green }
来源：http://tih.tianlin.xyz

[T29] Swift：guard 提前返回
来源：http://gpg.pengpengdd.cyou

guard let x = opt else { return }
来源：http://hxd.nanxuanxn.top

[T30] Swift：协议
来源：http://zyp.shuidangran.top

protocol Shape { func area() -> Double }
来源：http://tje.nanxuanxn.top

[T31] Lua：Hello World
来源：http://neo.pengpengdd.cyou

print("Hello")
来源：http://vmv.hesvh.cn

[T32] Lua：局部变量
来源：http://fkg.yvedp.cn

local a = 1
来源：http://zfl.zycfv.cn

[T33] Lua：表（数组）
来源：http://iea.yvedp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dum.haohaochexian.top

[T34] Lua：遍历表
来源：http://yaf.mhx1999.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gwd.nanxuanxn.top

[T35] Lua：字典表
来源：http://nqd.vehdjk.com

local d = { a = 1 };  d.b = 2
来源：http://oms.bbcook.cn

[T36] Lua：函数
来源：http://dqr.0kj1m.cn

function add(a, b) return a + b end
来源：http://ran.nanxuanxn.top

[T37] Lua：字符串拼接
来源：http://chz.shangyingyoupin.top

"a" .. "b"
来源：http://rqj.shanyushiyangkeji.top

[T38] Lua：条件
来源：http://mks.sxryk.cn

if x > 0 then print("正") end
来源：http://utt.cheryme.top

[T39] Lua：模式匹配
来源：http://qip.xylfe.cn

string.find(s, "%d+")
来源：http://jbr.zhoulong.xyz

[T40] Lua：元表
来源：http://qtw.cdnleiting.top

setmetatable({}, { __index = base })
来源：http://btf.zdbjq.cn

[T41] Perl：Hello World
来源：http://nwp.yueranfly.top

print "Hello\n";
来源：http://hoc.smart0.xyz

[T42] Perl：变量类型
来源：http://njv.cucudq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rsv.yueranfly.top

[T43] Perl：字符串插值
来源：http://xwb.ybcxt.top

"值: $a"
来源：http://fbm.hywenlv.cn

[T44] Perl：条件
来源：http://rtc.birdmap.top

if ($a > 0) { print "正"; }
来源：http://kiz.cdnleiting.top

[T45] Perl：数组遍历
来源：http://vvr.zhengqikj.top

for my $x (@arr) { print $x; }
来源：http://atz.yj20258888.top

[T46] Perl：哈希操作
来源：http://xbj.snrcjt.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://twg.uphjek.com

[T47] Perl：正则捕获
来源：http://mrf.cqqwz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cjg.sweek.top

[T48] Perl：正则替换
来源：http://gbu.sxryk.cn

$s =~ s/old/new/g;
来源：http://umj.dashuyun.cn

[T49] Perl：函数
来源：http://mdu.wangshuangyany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mij.cheryme.top

[T50] Perl：逐行读文件
来源：http://djx.wangshuangyany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qnl.zhijiandao.cn

while (my $line = <$fh>) { print $line; }
来源：http://qyb.daria6918.cn

[T51] Scala：Hello World
来源：http://exl.zdbjq.cn

println("Hello")
来源：http://odu.hfpthk.cn

[T52] Scala：变量
来源：http://ddd.gzhubu.top

val a = 1;  var b = 2
来源：http://hzj.0kj1m.cn

[T53] Scala：字符串插值
来源：http://odu.c1oappe.top

s"值: $b"
来源：http://igi.iojbl.cn

[T54] Scala：集合映射
来源：http://bae.sjlbkw.cn

List(1, 2, 3).map(_ * 2)
来源：http://nkd.jyoumei.cn

[T55] Scala：集合过滤
来源：http://sqp.pycfn.com

List(1, 2, 3).filter(_ > 1)
来源：http://gbl.ehwqpu.com

[T56] Scala：样例类
来源：http://bsi.yueranfly.top

case class User(name: String, age: Int)
来源：http://dgf.c1oappe.top

[T57] Scala：模式匹配
来源：http://tls.yj202588.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://uda.guowangkeji.top

[T58] Scala：函数定义
来源：http://suh.nanxinkj.top

def add(a: Int, b: Int): Int = a + b
来源：http://vkp.xuetiantiany.cn

[T59] Scala：循环
来源：http://lcd.tian-w.cn

for (i <- 1 to 10) println(i)
来源：http://lcc.c1oappe.top

[T60] Scala：折叠
来源：http://ndz.snrcjt.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jbn.jyoumei.cn

================================================================================
来源：http://mtc.yongpay.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vxv.bjfxy.top

================================================================================
来源：http://ghc.jianghu66.top

[U01] Py：创建虚拟环境
来源：http://das.tianlin.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://xeg.shanyushiyangtech.top

[U02] Py：导出 / 安装依赖
来源：http://yzz.svipenyu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oen.nwbrower.top

[U03] Py：加载 .env 配置
来源：http://vuw.bbcook.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ajg.shangyingyoupin.top

[U04] Py：变量调试打印
来源：http://bmr.feifeiyinyue.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vwp.yj20258.top

[U05] Py：列表去重且保序
来源：http://jbj.ybcxt.top

list(dict.fromkeys(arr))
来源：http://usz.jinyuanbaomall.cn

[U06] Py：合并两个字典
来源：http://tco.yj202588.top

{**a, **b}
来源：http://tdb.fehbvm.com

[U07] Py：反转字典键值
来源：http://ftu.c1oappe.top

{v: k for k, v in d.items()}
来源：http://ind.hongshengwenyu.top

[U08] Py：展平二维列表
来源：http://dlt.daxiang520.top

[y for x in nested for y in x]
来源：http://yuj.yonumen.top

[U09] Py：字典取最大值的键
来源：http://qld.hysaishi.cn

max(d, key=d.get)
来源：http://hgq.tianlin.xyz

[U10] Py：按值排序字典
来源：http://ydn.zdqjudy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://igl.tian-w.cn

[U11] Py：生成器表达式
来源：http://oce.xuanzx.com

(x * 2 for x in arr)
来源：http://crc.ydjk.org.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tda.bbcook.cn

Counter(arr).most_common(3)
来源：http://cjy.redwolf501.top

[U13] Py：固定长度队列
来源：http://gle.dashuyun.cn

deque(maxlen=10)
来源：http://sog.hfpthk.cn

[U14] Py：分组收集到列表
来源：http://oxt.yongpay.top

defaultdict(list)
来源：http://acz.bjfxy.top

[U15] Py：高精度计时
来源：http://ptj.gaohongyu789.top

t = time.perf_counter()
来源：http://pey.shzxlz.cn

[U16] Py：命令行参数解析
来源：http://atn.ctjpmb.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qyx.sufxvd.cn

[U17] Py：初始化日志
来源：http://loy.tanke756.top

logging.basicConfig(level=logging.INFO)
来源：http://hrv.hnxiangtu.top

[U18] Py：预编译正则
来源：http://kzz.xinyue.icu

pat = re.compile(r"\d+")
来源：http://ktb.ppjwa.cn

[U19] Py：正则替换带回调
来源：http://gwu.yj20258.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wqe.xuanzx.com

[U20] Py：缓存函数结果
来源：http://ajg.chenzaomai.com

@functools.lru_cache(maxsize=None)
来源：http://yvy.vehdjk.com

[U21] Py：自定义上下文管理器
来源：http://hjd.cucudq.cn

@contextlib.contextmanager
来源：http://mdy.mhx1999.top

[U22] Py：矩阵转置
来源：http://tio.daria6918.cn

list(zip(*m))
来源：http://mwp.tian-w.cn

[U23] Py：分块读取大文件
来源：http://pwe.shanyushiyangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nwm.zhaomingkeji.xyz

[U24] Py：路径操作
来源：http://uin.pycfn.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dxq.jinyuanbaomall.cn

[U25] Py：CSV 按字典读
来源：http://utm.feifeiyinyue.top

csv.DictReader(f)
来源：http://coz.kuanghao11.cn

[U26] Py：并发下载
来源：http://zgb.nanxinkj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://prt.ydjk.org.cn

[U27] Py：异步 HTTP
来源：http://ugo.dashuyun.cn

aiohttp.ClientSession() 配合 async with
来源：http://ckb.0kj1m.cn

[U28] Py：类型别名
来源：http://bkg.sufxvd.cn

UserId = int
来源：http://nnn.feifeiyinyue.top

[U29] Py：属性校验
来源：http://oqb.jqgufenzy.top

@property 与 @x.setter 配合
来源：http://qlk.hcnkem.com

[U30] Py：数据类
来源：http://jvx.ctjpmb.com

@dataclass(slots=True)
来源：http://kbh.pengpengdd.cyou

[U31] Py：单测
来源：http://yff.yonumen.top

python -m pytest -q
来源：http://kqu.redwolf501.top

[U32] Py：代码格式化
来源：http://ywu.tianlin.xyz

ruff format . && ruff check --fix .
来源：http://ffx.dashuyun.cn

[U33] Py：打包发布
来源：http://swt.yuxming.cn

python -m build  （依赖 pyproject.toml）
来源：http://inf.snrcjt.cn

[U34] Py：判断编码
来源：http://keb.zhiwuduotai.top

chardet.detect(raw)
来源：http://qub.guowangkeji.top

[U35] Py：发送邮件
来源：http://iff.xinyue.icu

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fku.chenjidiqi.icu

[U36] Py：定时任务
来源：http://tsm.wangshuangyany.cn

schedule.every(10).minutes.do(job)
来源：http://jgd.smart0.xyz

[U37] Py：读写 Excel
来源：http://vew.sxryk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nfy.sysykeji.top

[U38] Py：获取脚本所在目录
来源：http://wyf.xylfe.cn

Path(__file__).resolve().parent
来源：http://bkj.yj20258888.top

[U39] Py：判断是否在交互环境
来源：http://srx.zdqjudy.top

sys.stdout.isatty()
来源：http://mwj.ppjwa.cn

[U40] Py：打印到标准错误
来源：http://pax.dashuyun.cn

print("err", file=sys.stderr)
来源：http://sad.vqdsnc.cn

[U41] PHP：初始化 Composer 项目
来源：http://avl.hnqzz.top

composer init;  composer require guzzlehttp/guzzle
来源：http://sbl.52xcode.cn

[U42] PHP：PSR-4 自动加载
来源：http://ema.yangfankeji.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hyd.nanxuanxn.top

[U43] PHP：声明命名空间
来源：http://ihl.ybcxt.top

namespace App\Http;
来源：http://xdq.zhaomingkeji.xyz

[U44] PHP：开启严格类型
来源：http://hxv.bjfxy.top

declare(strict_types=1);
来源：http://byx.jiagoushi.top

[U45] PHP：类型声明与返回类型
来源：http://usz.cashguo.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xuh.daria6918.cn

[U46] PHP：可空类型
来源：http://hic.fanxiaobao.xyz

?string $name = null
来源：http://gwn.cucudq.cn

[U47] PHP：联合类型
来源：http://bqr.zhijiandao.cn

int|string $id
来源：http://uzw.iojbl.cn

[U48] PHP：纯枚举
来源：http://hbf.nwbrower.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://deu.hongshengwenyu.top

[U49] PHP：只读属性
来源：http://lge.tian-w.cn

public readonly string $name
来源：http://zrk.cucudq.cn

[U50] PHP：构造器属性提升
来源：http://nke.52xcode.cn

public function __construct(private int $id) {}
来源：http://ohm.vqdsnc.cn

[U51] PHP：数组解构
来源：http://pnd.fengsongda.top

[$a, $b] = $arr;
来源：http://joo.hfpthk.cn

[U52] PHP：箭头函数
来源：http://ltc.zhoulong.xyz

$double = fn($x) => $x * 2;
来源：http://orb.gaohongyu789.top

[U53] PHP：空合并运算符
来源：http://vdg.cashguo.top

$v = $a ?? $b ?? "default";
来源：http://wmy.ehwqpu.com

[U54] PHP：空安全调用
来源：http://acd.jinyuanbaomall.cn

$obj?->method()
来源：http://wad.fehbvm.com

[U55] PHP：match 表达式
来源：http://myn.iojbl.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dji.fengsongda.top

[U56] PHP：命名参数
来源：http://cgp.yongpay.top

f(a: 1, b: 2)
来源：http://hnk.pengpengdd.cyou

[U57] PHP：字符串插值
来源：http://xtw.xingfuxueyuan.xyz

"值: {$a}"
来源：http://qmj.tian-w.cn

[U58] PHP：数组三件套
来源：http://bjz.jinyuanbaomall.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://drq.zycfv.cn

[U59] PHP：自定义排序
来源：http://zxs.haohaochexian.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pci.xingfuxueyuan.xyz

[U60] PHP：JSON 编解码
来源：http://xxv.jqgfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rmv.hysaishi.cn

[U61] PHP：正则
来源：http://dih.shanyushiyangtech.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sjt.xingfuxueyuan.xyz

[U62] PHP：日期对象
来源：http://dba.tianlin.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yur.fzhhl.top

[U63] PHP：文件读写
来源：http://oix.redwolf501.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://buy.haohaochexian.top

[U64] PHP：目录遍历
来源：http://cnt.jinghuilouyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://cnq.zdbjq.cn

[U65] PHP：会话
来源：http://lsu.daria6918.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://imu.ehwqpu.com

[U66] PHP：设置 Cookie
来源：http://dxg.jianghu66.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kaz.fengsongda.top

[U67] PHP：处理文件上传
来源：http://wpb.kuanghao11.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fpn.chenjidiqi.icu

[U68] PHP：PDO 连接
来源：http://otd.ctjpmb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qzx.aizwys.cn


<!-- 参考信息 -->