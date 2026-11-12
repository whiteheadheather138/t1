代发 wailian999

[S39] C++：自定义比较器排序
来源：http://mwc.ivvv.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wdw.cashguo.top

[S40] C++：查找元素
来源：http://ltk.quarkkingdee.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ytu.wangshuangyany.cn

[S41] C++：类与构造函数
来源：http://gdz.daxiang520.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zwt.zhiwuduotai.top

[S42] C++：继承与虚函数
来源：http://nbe.redwolf501.top

class B : public Base { public: void f() override {} };
来源：http://rdk.jinqigfzy.top

[S43] C++：智能指针
来源：http://vzh.cdnleiting.top

auto p = std::make_unique<int>(5);
来源：http://mnn.gaohongyu789.top

[S44] C++：引用传参
来源：http://uff.shangyingyoupin.top

void inc(int &x) { ++x; }
来源：http://rat.yuxming.cn

[S45] C++：lambda
来源：http://leq.c1oappe.top

auto add = [](int a, int b) { return a + b; };
来源：http://qfk.9152youxi.cn

[S46] C++：函数模板
来源：http://ign.daxiang520.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fjl.sweek.top

[S47] C++：结构化绑定遍历
来源：http://ubq.ydzc1.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://afo.hammf.cn

[S48] C++：逐行读文件
来源：http://uja.yangfankeji.com

std::ifstream in("a.txt");  std::string line;
来源：http://fwy.dashuyun.cn

while (std::getline(in, line)) { }
来源：http://zcj.iojbl.cn

[S49] C++：写文件
来源：http://csb.yfazqb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vqn.xuanzx.com

[S50] C++：格式化数字
来源：http://iyx.haohaochexian.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cgh.yuxming.cn

[S51] C++：显式类型转换
来源：http://xyy.xingfuxueyuan.xyz

static_cast<double>(a) / b
来源：http://rcy.gaohongyu789.top

[S52] C++：const 与 noexcept
来源：http://vhh.fktsv.cn

int size() const noexcept { return n_; }
来源：http://esb.mhx1999.top

[S53] C++：移动语义
来源：http://fuq.dianchejie.cn

std::vector<int> w = std::move(v);
来源：http://eib.feifeiyinyue.top

[S54] C++：异常处理
来源：http://gha.shzxlz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ylt.jqgufenzy.top

[S55] C++：结构化绑定
来源：http://gcw.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yxx.zdqjudy.top

[S56] C++：optional
来源：http://cky.cucudq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cdg.gaohongyu789.top

[S57] C++：编译期常量
来源：http://nqf.hfpthk.cn

constexpr int N = 10;
来源：http://vir.sufxvd.cn

[S58] C++：命名空间
来源：http://zqd.bjfxy.top

namespace ns { int f() { return 1; } }
来源：http://www.fanxiaobao.xyz

[S59] C++：静态断言
来源：http://dih.sxryk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qxm.zhongyouzk.top

[S60] C++：遍历并删除元素
来源：http://rio.shzxlz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mco.zhijiandao.cn

================================================================================
来源：http://cfm.zdbjq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lep.gotoacloud.top

================================================================================
来源：http://fmc.yangfankeji.com

[T01] Kotlin：Hello World
来源：http://jzl.jqgufenzy.top

println("Hello")
来源：http://jaw.nanxinkj.top

[T02] Kotlin：变量
来源：http://dwi.cashguo.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dao.quarkkingdee.top

[T03] Kotlin：字符串模板
来源：http://uvh.quarkkingdee.top

"值: $b"
来源：http://puo.yuanzhike.top

[T04] Kotlin：空安全
来源：http://pct.jqgfzy.top

val n: String? = null;  n?.length
来源：http://wdm.xziqi.cn

[T05] Kotlin：when 表达式
来源：http://byn.fengsongda.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ahn.havefunace.top

[T06] Kotlin：集合映射
来源：http://kty.cdnleiting.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hta.gaohongyu789.top

[T07] Kotlin：集合过滤
来源：http://fyo.fktsv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ray.pycfn.com

[T08] Kotlin：数据类
来源：http://ons.hysaishi.cn

data class User(val name: String, val age: Int)
来源：http://qbu.pengpengdd.cyou

[T09] Kotlin：扩展函数
来源：http://qlr.zhoulong.xyz

fun String.exclaim() = this + "!"
来源：http://stp.nwbrower.top

[T10] Kotlin：默认参数
来源：http://epi.ppjwa.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ufd.xuanzx.com

[T11] Kotlin：协程
来源：http://vil.yueranfly.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ulo.hywenlv.cn

[T12] Kotlin：解构声明
来源：http://vyy.fehbvm.com

val (a, b) = Pair(1, 2)
来源：http://yla.dianchejie.cn

[T13] Kotlin：只读 Map
来源：http://uwb.yj20258.top

val m = mapOf("a" to 1)
来源：http://xca.jqgfzy.top

[T14] Kotlin：循环
来源：http://orh.xinyue.icu

for (i in 1..10) println(i)
来源：http://lll.nwbrower.top

[T15] Kotlin：接口
来源：http://dlg.xuanzx.com

interface Shape { fun area(): Double }
来源：http://cvu.jlsjyb.cn

[T16] Swift：Hello World
来源：http://vva.iojbl.cn

print("Hello")
来源：http://dvp.uphjek.com

[T17] Swift：变量与常量
来源：http://kga.smart0.xyz

var a = 1;  let b = 2
来源：http://llq.wangshuangyany.cn

[T18] Swift：字符串插值
来源：http://qzo.ybcxt.top

"值: \(b)"
来源：http://ict.yvedp.cn

[T19] Swift：可选绑定
来源：http://yck.svipenyu.cn

if let n = opt { print(n) }
来源：http://kdt.jlsjyb.cn

[T20] Swift：数组操作
来源：http://wpn.shanyushiyangtech.top

var a = [1, 2, 3];  a.append(4)
来源：http://hrd.52xcode.cn

[T21] Swift：遍历
来源：http://hne.yvedp.cn

for x in a { print(x) }
来源：http://sip.ctjpmb.com

[T22] Swift：字典
来源：http://pln.52xcode.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cpz.yj20258888.top

[T23] Swift：函数
来源：http://eiv.hongshengwenyu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hld.fengsongda.top

[T24] Swift：闭包
来源：http://iqv.jqgufenzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ryn.ydjk.org.cn

[T25] Swift：结构体
来源：http://kwz.daria6918.cn

struct P { var x: Int }
来源：http://rmj.yj20258888.top

[T26] Swift：类与重写
来源：http://ljs.9152youxi.cn

class A: Base { override func f() {} }
来源：http://slu.snrcjt.cn

[T27] Swift：错误处理
来源：http://erh.jlsjyb.cn

do { try f() } catch { print(error) }
来源：http://dwe.iojbl.cn

[T28] Swift：枚举
来源：http://pjz.nanxinkj.top

enum Color { case red, green }
来源：http://owu.ybcxt.top

[T29] Swift：guard 提前返回
来源：http://juv.shangyingyoupin.top

guard let x = opt else { return }
来源：http://rcz.wangdashe.top

[T30] Swift：协议
来源：http://rza.gaohongyu789.top

protocol Shape { func area() -> Double }
来源：http://lww.hnqzz.top

[T31] Lua：Hello World
来源：http://mxr.nanxuanxn.top

print("Hello")
来源：http://bth.fengsongda.top

[T32] Lua：局部变量
来源：http://yyz.yj20258888.top

local a = 1
来源：http://eil.zhengqikj.top

[T33] Lua：表（数组）
来源：http://iuc.hnqzz.top

local t = {1, 2, 3};  t[4] = 4
来源：http://eet.yuanzhike.top

[T34] Lua：遍历表
来源：http://qlq.zhengqikj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://shd.xylfe.cn

[T35] Lua：字典表
来源：http://dbt.snrcjt.cn

local d = { a = 1 };  d.b = 2
来源：http://nsa.snrcjt.cn

[T36] Lua：函数
来源：http://wdm.52xcode.cn

function add(a, b) return a + b end
来源：http://ney.zycfv.cn

[T37] Lua：字符串拼接
来源：http://icy.sxryk.cn

"a" .. "b"
来源：http://xgx.fengsongda.top

[T38] Lua：条件
来源：http://tqo.chenjidiqi.icu

if x > 0 then print("正") end
来源：http://btw.cashguo.top

[T39] Lua：模式匹配
来源：http://jfk.wangshuangyany.cn

string.find(s, "%d+")
来源：http://qwf.ybcxt.top

[T40] Lua：元表
来源：http://smj.pycfn.com

setmetatable({}, { __index = base })
来源：http://rcu.zhengqikj.top

[T41] Perl：Hello World
来源：http://isv.yongpay.top

print "Hello\n";
来源：http://ooe.hesvh.cn

[T42] Perl：变量类型
来源：http://fko.ydjk.org.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://byr.gaohongyu789.top

[T43] Perl：字符串插值
来源：http://hiu.yangfankeji.com

"值: $a"
来源：http://wjm.fktsv.cn

[T44] Perl：条件
来源：http://sgm.guannengcc.top

if ($a > 0) { print "正"; }
来源：http://quo.hesvh.cn

[T45] Perl：数组遍历
来源：http://xnn.svipenyu.cn

for my $x (@arr) { print $x; }
来源：http://cuf.cqqwz.cn

[T46] Perl：哈希操作
来源：http://bxe.gaohongyu789.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://znz.sxryk.cn

[T47] Perl：正则捕获
来源：http://jqm.yj202588.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xpz.dianchejie.cn

[T48] Perl：正则替换
来源：http://riu.hcnkem.com

$s =~ s/old/new/g;
来源：http://wsd.birdmap.top

[T49] Perl：函数
来源：http://idn.aibaodan.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sxd.pengpengdd.cyou

[T50] Perl：逐行读文件
来源：http://lhl.guannengcc.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vfk.tianlin.xyz

while (my $line = <$fh>) { print $line; }
来源：http://bna.ivvv.top

[T51] Scala：Hello World
来源：http://nfa.ydjk.org.cn

println("Hello")
来源：http://xzz.gzhubu.top

[T52] Scala：变量
来源：http://pkh.epnwcf.com

val a = 1;  var b = 2
来源：http://vgg.ydjk.org.cn

[T53] Scala：字符串插值
来源：http://tdf.cheryme.top

s"值: $b"
来源：http://omb.zhongyouzk.top

[T54] Scala：集合映射
来源：http://nnn.cqqwz.cn

List(1, 2, 3).map(_ * 2)
来源：http://klb.dianchejie.cn

[T55] Scala：集合过滤
来源：http://lgt.yfazqb.com

List(1, 2, 3).filter(_ > 1)
来源：http://xwk.mhx1999.top

[T56] Scala：样例类
来源：http://kbu.aibaodan.cn

case class User(name: String, age: Int)
来源：http://yjx.nwbrower.top

[T57] Scala：模式匹配
来源：http://uct.vqdsnc.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://swi.yfazqb.com

[T58] Scala：函数定义
来源：http://btv.yfazqb.com

def add(a: Int, b: Int): Int = a + b
来源：http://gwu.dianchejie.cn

[T59] Scala：循环
来源：http://xqa.guowangkeji.top

for (i <- 1 to 10) println(i)
来源：http://tiq.zhijiandao.cn

[T60] Scala：折叠
来源：http://qmn.yfazqb.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mfq.hfpthk.cn

================================================================================
来源：http://evv.shanyushiyangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pwr.fzhhl.top

================================================================================
来源：http://amf.xylfe.cn

[U01] Py：创建虚拟环境
来源：http://dmm.aizwys.cn

python -m venv .venv && source .venv/bin/activate
来源：http://evr.aibaodan.cn

[U02] Py：导出 / 安装依赖
来源：http://fih.xingfuxueyuan.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uxx.yj20258888.top

[U03] Py：加载 .env 配置
来源：http://wbu.sufxvd.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://und.daxiang520.top

[U04] Py：变量调试打印
来源：http://avp.yj20258.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lvq.yuanzhike.top

[U05] Py：列表去重且保序
来源：http://ovb.yvedp.cn

list(dict.fromkeys(arr))
来源：http://wno.hysaishi.cn

[U06] Py：合并两个字典
来源：http://aph.guannengcc.top

{**a, **b}
来源：http://uzy.bbcook.cn

[U07] Py：反转字典键值
来源：http://fxy.epnwcf.com

{v: k for k, v in d.items()}
来源：http://txi.yongpay.top

[U08] Py：展平二维列表
来源：http://led.bbcook.cn

[y for x in nested for y in x]
来源：http://hiz.zhaomingkeji.xyz

[U09] Py：字典取最大值的键
来源：http://ypp.zhaomingkeji.xyz

max(d, key=d.get)
来源：http://fep.daria6918.cn

[U10] Py：按值排序字典
来源：http://yun.shanyushiyangtech.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hwb.fengsongda.top

[U11] Py：生成器表达式
来源：http://lbx.316326.xyz

(x * 2 for x in arr)
来源：http://fdo.xziqi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rjw.jinqigufen.top

Counter(arr).most_common(3)
来源：http://gmn.fanxiaobao.xyz

[U13] Py：固定长度队列
来源：http://kkn.daria6918.cn

deque(maxlen=10)
来源：http://rfm.wangshuangyany.cn

[U14] Py：分组收集到列表
来源：http://gpy.hesvh.cn

defaultdict(list)
来源：http://tlq.snrcjt.cn

[U15] Py：高精度计时
来源：http://nib.snrcjt.cn

t = time.perf_counter()
来源：http://ugx.tanke756.top

[U16] Py：命令行参数解析
来源：http://ehl.chenjidiqi.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://snw.gaohongyu789.top

[U17] Py：初始化日志
来源：http://eyx.xingfuxueyuan.xyz

logging.basicConfig(level=logging.INFO)
来源：http://eib.xziqi.cn

[U18] Py：预编译正则
来源：http://eol.jinqigfzy.top

pat = re.compile(r"\d+")
来源：http://tri.yuanzhike.top

[U19] Py：正则替换带回调
来源：http://uxu.yongpay.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wzu.cdnleiting.top

[U20] Py：缓存函数结果
来源：http://vgd.mhx1999.top

@functools.lru_cache(maxsize=None)
来源：http://lzy.yonumen.top

[U21] Py：自定义上下文管理器
来源：http://exz.yonumen.top

@contextlib.contextmanager
来源：http://rrq.guowangkeji.top

[U22] Py：矩阵转置
来源：http://yor.yj20258888.top

list(zip(*m))
来源：http://red.yongpay.top

[U23] Py：分块读取大文件
来源：http://bqb.chenzaomai.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ibs.pycfn.com

[U24] Py：路径操作
来源：http://rhd.shanyushiyangkeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rev.yongpay.top

[U25] Py：CSV 按字典读
来源：http://gax.quarkkingdee.top

csv.DictReader(f)
来源：http://nnp.yuanzhike.top

[U26] Py：并发下载
来源：http://nil.chenlongwang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fxx.haohaochexian.top

[U27] Py：异步 HTTP
来源：http://may.dashuyun.cn

aiohttp.ClientSession() 配合 async with
来源：http://akx.feifeiyinyue.top

[U28] Py：类型别名
来源：http://hvw.gotoacloud.top

UserId = int
来源：http://ukq.c1oappe.top

[U29] Py：属性校验
来源：http://lxk.yvedp.cn

@property 与 @x.setter 配合
来源：http://zvy.gzhubu.top

[U30] Py：数据类
来源：http://orz.zycfv.cn

@dataclass(slots=True)
来源：http://mic.sxryk.cn

[U31] Py：单测
来源：http://htg.zhengqikj.top

python -m pytest -q
来源：http://vck.yangfankeji.com

[U32] Py：代码格式化
来源：http://zst.fengsongda.top

ruff format . && ruff check --fix .
来源：http://qrz.gotoacloud.top

[U33] Py：打包发布
来源：http://cbw.haohaochexian.top

python -m build  （依赖 pyproject.toml）
来源：http://rvr.zdqjudy.top

[U34] Py：判断编码
来源：http://rqt.yj20258.top

chardet.detect(raw)
来源：http://fen.hnxiangtu.top

[U35] Py：发送邮件
来源：http://byh.uphjek.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oek.epnwcf.com

[U36] Py：定时任务
来源：http://bnl.zhijiandao.cn

schedule.every(10).minutes.do(job)
来源：http://ioa.ywan-chungtsiang.top

[U37] Py：读写 Excel
来源：http://unk.hesvh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kfi.zdqjudy.top

[U38] Py：获取脚本所在目录
来源：http://mgk.tian-w.cn

Path(__file__).resolve().parent
来源：http://gnb.zhijiandao.cn

[U39] Py：判断是否在交互环境
来源：http://tpq.vehdjk.com

sys.stdout.isatty()
来源：http://kje.sysykeji.top

[U40] Py：打印到标准错误
来源：http://xun.jinyuanbaomall.cn

print("err", file=sys.stderr)
来源：http://kds.zdbjq.cn

[U41] PHP：初始化 Composer 项目
来源：http://enm.shzxlz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fhu.jqgfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://mkd.ydzc1.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://svo.kuanghao11.cn

[U43] PHP：声明命名空间
来源：http://vxh.chenlongwang.top

namespace App\Http;
来源：http://jyj.wangdashe.top

[U44] PHP：开启严格类型
来源：http://wdk.ydzc1.top

declare(strict_types=1);
来源：http://plt.hysaishi.cn

[U45] PHP：类型声明与返回类型
来源：http://szl.zhaomingkeji.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://xnq.ctjpmb.com

[U46] PHP：可空类型
来源：http://uzw.vehdjk.com

?string $name = null
来源：http://dzv.quarkkingdee.top

[U47] PHP：联合类型
来源：http://fpi.zhiwuduotai.top

int|string $id
来源：http://fmd.xuetiantiany.cn

[U48] PHP：纯枚举
来源：http://xho.sufxvd.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://brp.yueranfly.top

[U49] PHP：只读属性
来源：http://zus.dianchejie.cn

public readonly string $name
来源：http://lnx.jinqigufen.top

[U50] PHP：构造器属性提升
来源：http://skk.xylfe.cn

public function __construct(private int $id) {}
来源：http://ooc.chenlongwang.top

[U51] PHP：数组解构
来源：http://kwk.zhixingplan.top

[$a, $b] = $arr;
来源：http://qai.hesvh.cn

[U52] PHP：箭头函数
来源：http://gyr.sweek.top

$double = fn($x) => $x * 2;
来源：http://nln.ydjk.org.cn

[U53] PHP：空合并运算符
来源：http://uvm.fengsongda.top

$v = $a ?? $b ?? "default";
来源：http://qgb.epnwcf.com

[U54] PHP：空安全调用
来源：http://zvn.xuanzx.com

$obj?->method()
来源：http://lrx.aibaodan.cn

[U55] PHP：match 表达式
来源：http://ium.yanxiufei.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vea.gzhubu.top

[U56] PHP：命名参数
来源：http://oka.hnxiangtu.top

f(a: 1, b: 2)
来源：http://cxi.hongshengwenyu.top

[U57] PHP：字符串插值
来源：http://vpv.yanxiufei.cn

"值: {$a}"
来源：http://amk.gogol.net.cn

[U58] PHP：数组三件套
来源：http://nmb.c1oappe.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wmg.cqqwz.cn

[U59] PHP：自定义排序
来源：http://wqp.hammf.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ruk.iojbl.cn

[U60] PHP：JSON 编解码
来源：http://eie.uphjek.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mxp.hcnkem.com

[U61] PHP：正则
来源：http://zet.yonumen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kbw.xylfe.cn

[U62] PHP：日期对象
来源：http://ais.iojbl.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mch.birdmap.top

[U63] PHP：文件读写
来源：http://kcy.shangyingyoupin.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sju.zhaomingkeji.xyz

[U64] PHP：目录遍历
来源：http://gqq.jqgufenzy.top

glob("dir/*.php");  scandir("dir");
来源：http://rik.zhiwuduotai.top


<!-- 参考信息 -->