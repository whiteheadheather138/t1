代发 wailian999

[S39] C++：自定义比较器排序
来源：http://jya.feifeiyinyue.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fbd.yj202588.top

[S40] C++：查找元素
来源：http://qyo.guowangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kxk.cqqwz.cn

[S41] C++：类与构造函数
来源：http://dll.zhongyouzk.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rpn.zhoulong.xyz

[S42] C++：继承与虚函数
来源：http://ypu.aibaodan.cn

class B : public Base { public: void f() override {} };
来源：http://fys.sxryk.cn

[S43] C++：智能指针
来源：http://ubr.zhongyouzk.top

auto p = std::make_unique<int>(5);
来源：http://grw.kuanghao11.cn

[S44] C++：引用传参
来源：http://woi.hywenlv.cn

void inc(int &x) { ++x; }
来源：http://uwm.vqdsnc.cn

[S45] C++：lambda
来源：http://yrl.vehdjk.com

auto add = [](int a, int b) { return a + b; };
来源：http://qal.hnxiangtu.top

[S46] C++：函数模板
来源：http://wmb.hysaishi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nri.fzhhl.top

[S47] C++：结构化绑定遍历
来源：http://moo.chenjidiqi.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lpy.yuanzhike.top

[S48] C++：逐行读文件
来源：http://nig.tian-w.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dkn.jqgufenzy.top

while (std::getline(in, line)) { }
来源：http://tdv.zhongyouzk.top

[S49] C++：写文件
来源：http://dqb.cheryme.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jkm.hfpthk.cn

[S50] C++：格式化数字
来源：http://qal.aizwys.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ron.316326.xyz

[S51] C++：显式类型转换
来源：http://vwv.hfpthk.cn

static_cast<double>(a) / b
来源：http://pue.feifeiyinyue.top

[S52] C++：const 与 noexcept
来源：http://fyz.c1oappe.top

int size() const noexcept { return n_; }
来源：http://fvu.tarul.cn

[S53] C++：移动语义
来源：http://wtt.yj20258888.top

std::vector<int> w = std::move(v);
来源：http://tnf.fzhhl.top

[S54] C++：异常处理
来源：http://csj.nwbrower.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kao.zhongyouzk.top

[S55] C++：结构化绑定
来源：http://oxl.nanxuanxn.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gqc.zdbjq.cn

[S56] C++：optional
来源：http://tlq.aizwys.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zcy.tian-w.cn

[S57] C++：编译期常量
来源：http://ymp.zhijiandao.cn

constexpr int N = 10;
来源：http://yxn.yfazqb.com

[S58] C++：命名空间
来源：http://tdk.0kj1m.cn

namespace ns { int f() { return 1; } }
来源：http://dlm.aibaodan.cn

[S59] C++：静态断言
来源：http://bjy.aibaodan.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ygs.ppjwa.cn

[S60] C++：遍历并删除元素
来源：http://jqu.chenjidiqi.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://its.xingfuxueyuan.xyz

================================================================================
来源：http://bqz.zdbjq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nsy.smart0.xyz

================================================================================
来源：http://dsr.guowangkeji.top

[T01] Kotlin：Hello World
来源：http://tgn.c1oappe.top

println("Hello")
来源：http://umk.wangdashe.top

[T02] Kotlin：变量
来源：http://aky.jinghuilouyu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://arf.cashguo.top

[T03] Kotlin：字符串模板
来源：http://obr.wangdashe.top

"值: $b"
来源：http://toc.aibaodan.cn

[T04] Kotlin：空安全
来源：http://lxc.9152youxi.cn

val n: String? = null;  n?.length
来源：http://ale.fengsongda.top

[T05] Kotlin：when 表达式
来源：http://aii.fktsv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qwt.tanke756.top

[T06] Kotlin：集合映射
来源：http://qei.ehwqpu.com

listOf(1, 2, 3).map { it * 2 }
来源：http://try.xuanzx.com

[T07] Kotlin：集合过滤
来源：http://prj.pycfn.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://rze.jqgufenzy.top

[T08] Kotlin：数据类
来源：http://ntk.ydzc1.top

data class User(val name: String, val age: Int)
来源：http://qsi.c1oappe.top

[T09] Kotlin：扩展函数
来源：http://tfg.xuetiantiany.cn

fun String.exclaim() = this + "!"
来源：http://zsv.aibaodan.cn

[T10] Kotlin：默认参数
来源：http://tom.smart0.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://alv.tanke756.top

[T11] Kotlin：协程
来源：http://giw.ybcxt.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://kvn.zhaomingkeji.xyz

[T12] Kotlin：解构声明
来源：http://lqq.redwolf501.top

val (a, b) = Pair(1, 2)
来源：http://lez.sweek.top

[T13] Kotlin：只读 Map
来源：http://utf.snrcjt.cn

val m = mapOf("a" to 1)
来源：http://ulh.yongpay.top

[T14] Kotlin：循环
来源：http://lse.kuanghao11.cn

for (i in 1..10) println(i)
来源：http://sqw.hcnkem.com

[T15] Kotlin：接口
来源：http://dok.ydjk.org.cn

interface Shape { fun area(): Double }
来源：http://lum.zdqjudy.top

[T16] Swift：Hello World
来源：http://jiz.yuxming.cn

print("Hello")
来源：http://mhm.hnqzz.top

[T17] Swift：变量与常量
来源：http://txh.316326.xyz

var a = 1;  let b = 2
来源：http://mdx.cashguo.top

[T18] Swift：字符串插值
来源：http://qie.guannengcc.top

"值: \(b)"
来源：http://lzz.vehdjk.com

[T19] Swift：可选绑定
来源：http://cbe.yueranfly.top

if let n = opt { print(n) }
来源：http://hzv.ywan-chungtsiang.top

[T20] Swift：数组操作
来源：http://awo.nanxinkj.top

var a = [1, 2, 3];  a.append(4)
来源：http://jco.meibo888.top

[T21] Swift：遍历
来源：http://zxh.guannengcc.top

for x in a { print(x) }
来源：http://kvk.smart0.xyz

[T22] Swift：字典
来源：http://lgw.chenjidiqi.icu

var d = ["a": 1];  d["b"] = 2
来源：http://pte.yangfankeji.com

[T23] Swift：函数
来源：http://ujh.hcnkem.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jgg.smart0.xyz

[T24] Swift：闭包
来源：http://qce.shzxlz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ghq.ehwqpu.com

[T25] Swift：结构体
来源：http://fzp.cheryme.top

struct P { var x: Int }
来源：http://mxy.zhaomingkeji.xyz

[T26] Swift：类与重写
来源：http://itr.hesvh.cn

class A: Base { override func f() {} }
来源：http://jwv.shzxlz.cn

[T27] Swift：错误处理
来源：http://hzc.fehbvm.com

do { try f() } catch { print(error) }
来源：http://qvx.hongshengwenyu.top

[T28] Swift：枚举
来源：http://dlj.c1oappe.top

enum Color { case red, green }
来源：http://izf.chenlongwang.top

[T29] Swift：guard 提前返回
来源：http://lio.hfpthk.cn

guard let x = opt else { return }
来源：http://qwy.meibo888.top

[T30] Swift：协议
来源：http://iyh.xingfuxueyuan.xyz

protocol Shape { func area() -> Double }
来源：http://nph.xylfe.cn

[T31] Lua：Hello World
来源：http://piq.gaohongyu789.top

print("Hello")
来源：http://ena.nwbrower.top

[T32] Lua：局部变量
来源：http://szh.ppjwa.cn

local a = 1
来源：http://avu.jiagoushi.top

[T33] Lua：表（数组）
来源：http://hci.zhengqikj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hkk.fengsongda.top

[T34] Lua：遍历表
来源：http://zzc.daria6918.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lny.smart0.xyz

[T35] Lua：字典表
来源：http://ozf.tian-w.cn

local d = { a = 1 };  d.b = 2
来源：http://nwp.xinyue.icu

[T36] Lua：函数
来源：http://agy.daria6918.cn

function add(a, b) return a + b end
来源：http://ijm.wangshuangyany.cn

[T37] Lua：字符串拼接
来源：http://oyt.yangfankeji.com

"a" .. "b"
来源：http://twt.yonumen.top

[T38] Lua：条件
来源：http://net.hongshengwenyu.top

if x > 0 then print("正") end
来源：http://pwj.sjlbkw.cn

[T39] Lua：模式匹配
来源：http://kbu.feifeiyinyue.top

string.find(s, "%d+")
来源：http://yum.ivvv.top

[T40] Lua：元表
来源：http://tag.gzhubu.top

setmetatable({}, { __index = base })
来源：http://mdi.tarul.cn

[T41] Perl：Hello World
来源：http://hie.yangfankeji.com

print "Hello\n";
来源：http://hqh.havefunace.top

[T42] Perl：变量类型
来源：http://obp.zhixingplan.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jin.zdbjq.cn

[T43] Perl：字符串插值
来源：http://wez.xylfe.cn

"值: $a"
来源：http://pbw.ctjpmb.com

[T44] Perl：条件
来源：http://lxo.yj202588.top

if ($a > 0) { print "正"; }
来源：http://hrd.pycfn.com

[T45] Perl：数组遍历
来源：http://bht.tarul.cn

for my $x (@arr) { print $x; }
来源：http://agh.meibo888.top

[T46] Perl：哈希操作
来源：http://pwr.shzxlz.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vac.cdnleiting.top

[T47] Perl：正则捕获
来源：http://oin.zhaomingkeji.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://ykl.ctjpmb.com

[T48] Perl：正则替换
来源：http://vol.cdnleiting.top

$s =~ s/old/new/g;
来源：http://fmv.vehdjk.com

[T49] Perl：函数
来源：http://fpc.kuanghao11.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://onn.vqdsnc.cn

[T50] Perl：逐行读文件
来源：http://qmr.zdbjq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lxp.vehdjk.com

while (my $line = <$fh>) { print $line; }
来源：http://snq.zhijiandao.cn

[T51] Scala：Hello World
来源：http://ioi.zhengqikj.top

println("Hello")
来源：http://fbv.snrcjt.cn

[T52] Scala：变量
来源：http://bus.pengpengdd.cyou

val a = 1;  var b = 2
来源：http://uyp.hnxiangtu.top

[T53] Scala：字符串插值
来源：http://ibe.sjlbkw.cn

s"值: $b"
来源：http://zqs.shanyushiyangtech.top

[T54] Scala：集合映射
来源：http://yob.yuanzhike.top

List(1, 2, 3).map(_ * 2)
来源：http://ghs.hongshengwenyu.top

[T55] Scala：集合过滤
来源：http://koh.ybcxt.top

List(1, 2, 3).filter(_ > 1)
来源：http://dxk.vqdsnc.cn

[T56] Scala：样例类
来源：http://gsy.shanyushiyangkeji.top

case class User(name: String, age: Int)
来源：http://wsu.cqqwz.cn

[T57] Scala：模式匹配
来源：http://okr.tianlin.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://eag.tianlin.xyz

[T58] Scala：函数定义
来源：http://ode.svipenyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://otk.birdmap.top

[T59] Scala：循环
来源：http://uop.52xcode.cn

for (i <- 1 to 10) println(i)
来源：http://foh.redwolf501.top

[T60] Scala：折叠
来源：http://kgi.jlsjyb.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cxl.0kj1m.cn

================================================================================
来源：http://jvd.gotoacloud.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qos.iojbl.cn

================================================================================
来源：http://jom.guowangkeji.top

[U01] Py：创建虚拟环境
来源：http://rht.yongpay.top

python -m venv .venv && source .venv/bin/activate
来源：http://qpe.sysykeji.top

[U02] Py：导出 / 安装依赖
来源：http://rnn.ydzc1.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rni.gogol.net.cn

[U03] Py：加载 .env 配置
来源：http://mrv.xingfuxueyuan.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://lrr.ybcxt.top

[U04] Py：变量调试打印
来源：http://nyi.hesvh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qtx.zycfv.cn

[U05] Py：列表去重且保序
来源：http://kbn.smart0.xyz

list(dict.fromkeys(arr))
来源：http://tzx.sysykeji.top

[U06] Py：合并两个字典
来源：http://mej.zhoulong.xyz

{**a, **b}
来源：http://xym.shanyushiyangtech.top

[U07] Py：反转字典键值
来源：http://poz.aibaodan.cn

{v: k for k, v in d.items()}
来源：http://zpt.jiagoushi.top

[U08] Py：展平二维列表
来源：http://fil.nwbrower.top

[y for x in nested for y in x]
来源：http://okt.ydjk.org.cn

[U09] Py：字典取最大值的键
来源：http://qfh.shanyushiyangtech.top

max(d, key=d.get)
来源：http://utx.0kj1m.cn

[U10] Py：按值排序字典
来源：http://gyo.jianghu66.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ary.smart0.xyz

[U11] Py：生成器表达式
来源：http://eoc.aibaodan.cn

(x * 2 for x in arr)
来源：http://uuq.yvedp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uyl.chenzaomai.com

Counter(arr).most_common(3)
来源：http://pdd.zdbjq.cn

[U13] Py：固定长度队列
来源：http://rcw.hnqzz.top

deque(maxlen=10)
来源：http://app.9152youxi.cn

[U14] Py：分组收集到列表
来源：http://tll.cqqwz.cn

defaultdict(list)
来源：http://vra.chenjidiqi.icu

[U15] Py：高精度计时
来源：http://ybq.aizwys.cn

t = time.perf_counter()
来源：http://jox.9152youxi.cn

[U16] Py：命令行参数解析
来源：http://uje.zhijiandao.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lgz.cheryme.top

[U17] Py：初始化日志
来源：http://oem.hcnkem.com

logging.basicConfig(level=logging.INFO)
来源：http://fbj.ydzc1.top

[U18] Py：预编译正则
来源：http://mon.sysykeji.top

pat = re.compile(r"\d+")
来源：http://zvi.9152youxi.cn

[U19] Py：正则替换带回调
来源：http://aof.andypj.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wja.xingfuxueyuan.xyz

[U20] Py：缓存函数结果
来源：http://xcb.jlsjyb.cn

@functools.lru_cache(maxsize=None)
来源：http://blx.shanyushiyangkeji.top

[U21] Py：自定义上下文管理器
来源：http://aha.hongshengwenyu.top

@contextlib.contextmanager
来源：http://myi.gaohongyu789.top

[U22] Py：矩阵转置
来源：http://ctj.wangshuangyany.cn

list(zip(*m))
来源：http://fri.jinqigufen.top

[U23] Py：分块读取大文件
来源：http://dmw.vehdjk.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gci.cheryme.top

[U24] Py：路径操作
来源：http://kff.gzhubu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ppk.wangshuangyany.cn

[U25] Py：CSV 按字典读
来源：http://aen.quarkkingdee.top

csv.DictReader(f)
来源：http://aif.epnwcf.com

[U26] Py：并发下载
来源：http://pwy.fanxiaobao.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qpn.xylfe.cn

[U27] Py：异步 HTTP
来源：http://uxv.hnxiangtu.top

aiohttp.ClientSession() 配合 async with
来源：http://gvh.xuanzx.com

[U28] Py：类型别名
来源：http://afi.haohaochexian.top

UserId = int
来源：http://xne.yuanzhike.top

[U29] Py：属性校验
来源：http://ies.jinqigufen.top

@property 与 @x.setter 配合
来源：http://adh.jlsjyb.cn

[U30] Py：数据类
来源：http://qiy.jqgufenzy.top

@dataclass(slots=True)
来源：http://nle.kuanghao11.cn

[U31] Py：单测
来源：http://iyc.zycfv.cn

python -m pytest -q
来源：http://lao.yanxiufei.cn

[U32] Py：代码格式化
来源：http://agc.jqgfzy.top

ruff format . && ruff check --fix .
来源：http://zyh.iojbl.cn

[U33] Py：打包发布
来源：http://kli.havefunace.top

python -m build  （依赖 pyproject.toml）
来源：http://lad.ydjk.org.cn

[U34] Py：判断编码
来源：http://syo.hcnkem.com

chardet.detect(raw)
来源：http://oqs.cashguo.top

[U35] Py：发送邮件
来源：http://quw.dianchejie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fni.52xcode.cn

[U36] Py：定时任务
来源：http://wdk.gzhubu.top

schedule.every(10).minutes.do(job)
来源：http://rwj.zhengqikj.top

[U37] Py：读写 Excel
来源：http://ulm.zhixingplan.top

pandas.read_excel / DataFrame.to_excel
来源：http://vcv.ydzc1.top

[U38] Py：获取脚本所在目录
来源：http://uog.fengsongda.top

Path(__file__).resolve().parent
来源：http://oed.ywan-chungtsiang.top

[U39] Py：判断是否在交互环境
来源：http://fwc.yangfankeji.com

sys.stdout.isatty()
来源：http://tob.hesvh.cn

[U40] Py：打印到标准错误
来源：http://ymk.shangyingyoupin.top

print("err", file=sys.stderr)
来源：http://udw.daria6918.cn

[U41] PHP：初始化 Composer 项目
来源：http://kqd.hywenlv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://uzs.xinyue.icu

[U42] PHP：PSR-4 自动加载
来源：http://zur.zhoulong.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nfl.yuanzhike.top

[U43] PHP：声明命名空间
来源：http://saq.zhiwuduotai.top

namespace App\Http;
来源：http://nxk.hfpthk.cn

[U44] PHP：开启严格类型
来源：http://axz.yj20258888.top

declare(strict_types=1);
来源：http://daz.gaohongyu789.top

[U45] PHP：类型声明与返回类型
来源：http://fzp.zycfv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ugd.nwbrower.top

[U46] PHP：可空类型
来源：http://rtd.jqgufenzy.top

?string $name = null
来源：http://nzq.hfpthk.cn

[U47] PHP：联合类型
来源：http://cqk.52xcode.cn

int|string $id
来源：http://avw.chenlongwang.top

[U48] PHP：纯枚举
来源：http://rrv.zhongyouzk.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://apc.ywan-chungtsiang.top

[U49] PHP：只读属性
来源：http://cqu.ydzc1.top

public readonly string $name
来源：http://kmb.zhijiandao.cn

[U50] PHP：构造器属性提升
来源：http://qnp.daria6918.cn

public function __construct(private int $id) {}
来源：http://dze.yfazqb.com

[U51] PHP：数组解构
来源：http://vis.cdnleiting.top

[$a, $b] = $arr;
来源：http://lpt.ydjk.org.cn

[U52] PHP：箭头函数
来源：http://ois.yueranfly.top

$double = fn($x) => $x * 2;
来源：http://vcz.andypj.xyz

[U53] PHP：空合并运算符
来源：http://gsk.snrcjt.cn

$v = $a ?? $b ?? "default";
来源：http://ppt.ctjpmb.com

[U54] PHP：空安全调用
来源：http://mln.sweek.top

$obj?->method()
来源：http://ext.ydzc1.top

[U55] PHP：match 表达式
来源：http://fon.hnxiangtu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ngj.aibaodan.cn

[U56] PHP：命名参数
来源：http://hbg.cheryme.top

f(a: 1, b: 2)
来源：http://lhu.epnwcf.com

[U57] PHP：字符串插值
来源：http://ppj.gaohongyu789.top

"值: {$a}"
来源：http://vkz.cheryme.top

[U58] PHP：数组三件套
来源：http://gnm.redwolf501.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tfa.jyoumei.cn

[U59] PHP：自定义排序
来源：http://mlf.jqgfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://elf.cucudq.cn

[U60] PHP：JSON 编解码
来源：http://qub.xylfe.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ovs.feifeiyinyue.top

[U61] PHP：正则
来源：http://xju.aizwys.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mgs.svipenyu.cn

[U62] PHP：日期对象
来源：http://htk.ydzc1.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cjl.chenzaomai.com

[U63] PHP：文件读写
来源：http://vwc.jinghuilouyu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://asv.hfpthk.cn

[U64] PHP：目录遍历
来源：http://ilo.hcnkem.com

glob("dir/*.php");  scandir("dir");
来源：http://qvb.ppjwa.cn


<!-- 参考信息 -->