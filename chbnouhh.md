代发 wailian999

[S35] C++：map
来源：http://vsv.tianlin.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qmx.ybcxt.top

[S36] C++：unordered_map
来源：http://thr.epnwcf.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://enu.zdbjq.cn

[S37] C++：set
来源：http://zbt.fzhhl.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ajz.vehdjk.com

[S38] C++：排序
来源：http://ugg.sjlbkw.cn

std::sort(v.begin(), v.end());
来源：http://myf.havefunace.top

[S39] C++：自定义比较器排序
来源：http://xvg.yj20258888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eaj.9152youxi.cn

[S40] C++：查找元素
来源：http://edg.ydjk.org.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ept.9152youxi.cn

[S41] C++：类与构造函数
来源：http://bwc.aizwys.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://goo.fktsv.cn

[S42] C++：继承与虚函数
来源：http://aee.zhixingplan.top

class B : public Base { public: void f() override {} };
来源：http://nun.chenjidiqi.icu

[S43] C++：智能指针
来源：http://ktz.gotoacloud.top

auto p = std::make_unique<int>(5);
来源：http://ply.fktsv.cn

[S44] C++：引用传参
来源：http://lnu.nanxinkj.top

void inc(int &x) { ++x; }
来源：http://wgv.ydzc1.top

[S45] C++：lambda
来源：http://xfb.tianlin.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://mhz.cqqwz.cn

[S46] C++：函数模板
来源：http://ecv.316326.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ogj.fktsv.cn

[S47] C++：结构化绑定遍历
来源：http://esf.yj20258.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sbf.hammf.cn

[S48] C++：逐行读文件
来源：http://nna.jinqigufen.top

std::ifstream in("a.txt");  std::string line;
来源：http://xrs.hnqzz.top

while (std::getline(in, line)) { }
来源：http://rvx.fehbvm.com

[S49] C++：写文件
来源：http://red.c1oappe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tkk.xziqi.cn

[S50] C++：格式化数字
来源：http://jwg.yuanzhike.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hjw.epnwcf.com

[S51] C++：显式类型转换
来源：http://ytz.gogol.net.cn

static_cast<double>(a) / b
来源：http://ymf.dianchejie.cn

[S52] C++：const 与 noexcept
来源：http://ugr.xylfe.cn

int size() const noexcept { return n_; }
来源：http://ctf.yangfankeji.com

[S53] C++：移动语义
来源：http://vwz.zhongyouzk.top

std::vector<int> w = std::move(v);
来源：http://xld.ydjk.org.cn

[S54] C++：异常处理
来源：http://ohw.shuidangran.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vjd.jqgfzy.top

[S55] C++：结构化绑定
来源：http://ktt.jinqigfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://icd.nanxinkj.top

[S56] C++：optional
来源：http://dmz.hywenlv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hat.uphjek.com

[S57] C++：编译期常量
来源：http://bhd.xuetiantiany.cn

constexpr int N = 10;
来源：http://csx.sweek.top

[S58] C++：命名空间
来源：http://frk.fehbvm.com

namespace ns { int f() { return 1; } }
来源：http://fns.fanxiaobao.xyz

[S59] C++：静态断言
来源：http://dow.jqgfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cvw.hnqzz.top

[S60] C++：遍历并删除元素
来源：http://iki.cqqwz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eaj.tian-w.cn

================================================================================
来源：http://fnr.jlsjyb.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yms.tian-w.cn

================================================================================
来源：http://flc.jqgfzy.top

[T01] Kotlin：Hello World
来源：http://qvf.ydjk.org.cn

println("Hello")
来源：http://czv.xylfe.cn

[T02] Kotlin：变量
来源：http://xyp.jinyuanbaomall.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://btf.tianlin.xyz

[T03] Kotlin：字符串模板
来源：http://xdx.zhijiandao.cn

"值: $b"
来源：http://duw.zhixingplan.top

[T04] Kotlin：空安全
来源：http://iqo.uphjek.com

val n: String? = null;  n?.length
来源：http://kkr.epnwcf.com

[T05] Kotlin：when 表达式
来源：http://imv.cucudq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://phj.gzhubu.top

[T06] Kotlin：集合映射
来源：http://vex.haohaochexian.top

listOf(1, 2, 3).map { it * 2 }
来源：http://kgk.shanyushiyangkeji.top

[T07] Kotlin：集合过滤
来源：http://lef.chenjidiqi.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://hec.vehdjk.com

[T08] Kotlin：数据类
来源：http://hss.yvedp.cn

data class User(val name: String, val age: Int)
来源：http://bvh.hongshengwenyu.top

[T09] Kotlin：扩展函数
来源：http://zff.kuanghao11.cn

fun String.exclaim() = this + "!"
来源：http://yko.mhx1999.top

[T10] Kotlin：默认参数
来源：http://boc.ivvv.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qah.uphjek.com

[T11] Kotlin：协程
来源：http://iwr.ppjwa.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uzg.cqqwz.cn

[T12] Kotlin：解构声明
来源：http://smr.jlsjyb.cn

val (a, b) = Pair(1, 2)
来源：http://txh.316326.xyz

[T13] Kotlin：只读 Map
来源：http://qcs.mhx1999.top

val m = mapOf("a" to 1)
来源：http://pcn.birdmap.top

[T14] Kotlin：循环
来源：http://wvy.nanxinkj.top

for (i in 1..10) println(i)
来源：http://lue.gotoacloud.top

[T15] Kotlin：接口
来源：http://fuk.wangshuangyany.cn

interface Shape { fun area(): Double }
来源：http://lae.hammf.cn

[T16] Swift：Hello World
来源：http://jcd.cheryme.top

print("Hello")
来源：http://uef.feifeiyinyue.top

[T17] Swift：变量与常量
来源：http://mvx.aibaodan.cn

var a = 1;  let b = 2
来源：http://jlk.redwolf501.top

[T18] Swift：字符串插值
来源：http://nbh.cheryme.top

"值: \(b)"
来源：http://ayg.nanxinkj.top

[T19] Swift：可选绑定
来源：http://yfs.pycfn.com

if let n = opt { print(n) }
来源：http://rfl.bjfxy.top

[T20] Swift：数组操作
来源：http://nul.tianlin.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://qfj.redwolf501.top

[T21] Swift：遍历
来源：http://uvv.zhiwuduotai.top

for x in a { print(x) }
来源：http://ucy.zhiwuduotai.top

[T22] Swift：字典
来源：http://ygl.jiagoushi.top

var d = ["a": 1];  d["b"] = 2
来源：http://vum.hysaishi.cn

[T23] Swift：函数
来源：http://suo.gaohongyu789.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nxl.epnwcf.com

[T24] Swift：闭包
来源：http://rco.cheryme.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ecl.sysykeji.top

[T25] Swift：结构体
来源：http://udw.chenlongwang.top

struct P { var x: Int }
来源：http://omj.zdqjudy.top

[T26] Swift：类与重写
来源：http://gxm.hcnkem.com

class A: Base { override func f() {} }
来源：http://thy.zhijiandao.cn

[T27] Swift：错误处理
来源：http://pkb.yuanzhike.top

do { try f() } catch { print(error) }
来源：http://jzu.cucudq.cn

[T28] Swift：枚举
来源：http://gvn.birdmap.top

enum Color { case red, green }
来源：http://gfa.ehwqpu.com

[T29] Swift：guard 提前返回
来源：http://dxe.bbcook.cn

guard let x = opt else { return }
来源：http://sly.hongshengwenyu.top

[T30] Swift：协议
来源：http://glx.bjfxy.top

protocol Shape { func area() -> Double }
来源：http://uig.0kj1m.cn

[T31] Lua：Hello World
来源：http://atw.shangyingyoupin.top

print("Hello")
来源：http://lxz.chenjidiqi.icu

[T32] Lua：局部变量
来源：http://gxd.ybcxt.top

local a = 1
来源：http://fdu.yuxming.cn

[T33] Lua：表（数组）
来源：http://ogy.yfazqb.com

local t = {1, 2, 3};  t[4] = 4
来源：http://lwb.shzxlz.cn

[T34] Lua：遍历表
来源：http://dmh.yj202588.top

for i, v in ipairs(t) do print(i, v) end
来源：http://sob.hongshengwenyu.top

[T35] Lua：字典表
来源：http://gof.haohaochexian.top

local d = { a = 1 };  d.b = 2
来源：http://lgd.tianlin.xyz

[T36] Lua：函数
来源：http://mrw.tarul.cn

function add(a, b) return a + b end
来源：http://ooa.yj20258888.top

[T37] Lua：字符串拼接
来源：http://ngp.yj20258888.top

"a" .. "b"
来源：http://zjq.zycfv.cn

[T38] Lua：条件
来源：http://oql.fktsv.cn

if x > 0 then print("正") end
来源：http://pkn.andypj.xyz

[T39] Lua：模式匹配
来源：http://rqy.hcnkem.com

string.find(s, "%d+")
来源：http://ojr.cashguo.top

[T40] Lua：元表
来源：http://ogb.feifeiyinyue.top

setmetatable({}, { __index = base })
来源：http://bcy.ehwqpu.com

[T41] Perl：Hello World
来源：http://uun.sysykeji.top

print "Hello\n";
来源：http://cxs.sufxvd.cn

[T42] Perl：变量类型
来源：http://glt.kuanghao11.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wxv.fzhhl.top

[T43] Perl：字符串插值
来源：http://cvp.zhongyouzk.top

"值: $a"
来源：http://ccx.dashuyun.cn

[T44] Perl：条件
来源：http://qhi.quarkkingdee.top

if ($a > 0) { print "正"; }
来源：http://ggh.hnqzz.top

[T45] Perl：数组遍历
来源：http://fvf.iojbl.cn

for my $x (@arr) { print $x; }
来源：http://lwv.jinyuanbaomall.cn

[T46] Perl：哈希操作
来源：http://aep.shangyingyoupin.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zrc.zycfv.cn

[T47] Perl：正则捕获
来源：http://itr.fanxiaobao.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://bcb.vqdsnc.cn

[T48] Perl：正则替换
来源：http://rmq.nwbrower.top

$s =~ s/old/new/g;
来源：http://hzm.feifeiyinyue.top

[T49] Perl：函数
来源：http://ohe.yuanzhike.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nbc.epnwcf.com

[T50] Perl：逐行读文件
来源：http://jex.havefunace.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ajf.yangfankeji.com

while (my $line = <$fh>) { print $line; }
来源：http://gca.zhongyouzk.top

[T51] Scala：Hello World
来源：http://ozu.jlsjyb.cn

println("Hello")
来源：http://bth.yfazqb.com

[T52] Scala：变量
来源：http://wka.bbcook.cn

val a = 1;  var b = 2
来源：http://zsl.ywan-chungtsiang.top

[T53] Scala：字符串插值
来源：http://ssz.sysykeji.top

s"值: $b"
来源：http://sgx.dashuyun.cn

[T54] Scala：集合映射
来源：http://yhz.yj202588.top

List(1, 2, 3).map(_ * 2)
来源：http://lre.hfpthk.cn

[T55] Scala：集合过滤
来源：http://oxf.guannengcc.top

List(1, 2, 3).filter(_ > 1)
来源：http://pwy.sxryk.cn

[T56] Scala：样例类
来源：http://fax.zhiwuduotai.top

case class User(name: String, age: Int)
来源：http://fuo.gzhubu.top

[T57] Scala：模式匹配
来源：http://nxe.xingfuxueyuan.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://vgy.hongshengwenyu.top

[T58] Scala：函数定义
来源：http://gpa.shuidangran.top

def add(a: Int, b: Int): Int = a + b
来源：http://kcz.aizwys.cn

[T59] Scala：循环
来源：http://swm.shanyushiyangtech.top

for (i <- 1 to 10) println(i)
来源：http://fpr.xylfe.cn

[T60] Scala：折叠
来源：http://zjm.yongpay.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hwj.aibaodan.cn

================================================================================
来源：http://mfk.zycfv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ocf.yj202588.top

================================================================================
来源：http://ovv.fengsongda.top

[U01] Py：创建虚拟环境
来源：http://ajz.xuanzx.com

python -m venv .venv && source .venv/bin/activate
来源：http://hcp.aizwys.cn

[U02] Py：导出 / 安装依赖
来源：http://sld.jqgufenzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gik.jqgfzy.top

[U03] Py：加载 .env 配置
来源：http://trh.fzhhl.top

from dotenv import load_dotenv; load_dotenv()
来源：http://cxe.sxryk.cn

[U04] Py：变量调试打印
来源：http://egj.zycfv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ukj.redwolf501.top

[U05] Py：列表去重且保序
来源：http://ebh.jianghu66.top

list(dict.fromkeys(arr))
来源：http://xxk.52xcode.cn

[U06] Py：合并两个字典
来源：http://szl.wangshuangyany.cn

{**a, **b}
来源：http://gxw.bjfxy.top

[U07] Py：反转字典键值
来源：http://ikp.pycfn.com

{v: k for k, v in d.items()}
来源：http://quh.mhx1999.top

[U08] Py：展平二维列表
来源：http://zfy.shzxlz.cn

[y for x in nested for y in x]
来源：http://ohl.quarkkingdee.top

[U09] Py：字典取最大值的键
来源：http://urf.feifeiyinyue.top

max(d, key=d.get)
来源：http://hwb.cheryme.top

[U10] Py：按值排序字典
来源：http://koe.havefunace.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rid.fzhhl.top

[U11] Py：生成器表达式
来源：http://kpd.shanyushiyangkeji.top

(x * 2 for x in arr)
来源：http://mmi.epnwcf.com

[U12] Py：取出现最多的 3 个元素
来源：http://sjy.mhx1999.top

Counter(arr).most_common(3)
来源：http://nhk.zhengqikj.top

[U13] Py：固定长度队列
来源：http://qtv.zhoulong.xyz

deque(maxlen=10)
来源：http://cek.jinyuanbaomall.cn

[U14] Py：分组收集到列表
来源：http://kaf.0kj1m.cn

defaultdict(list)
来源：http://jwy.shanyushiyangtech.top

[U15] Py：高精度计时
来源：http://bmc.fengsongda.top

t = time.perf_counter()
来源：http://ony.smart0.xyz

[U16] Py：命令行参数解析
来源：http://pgg.kuanghao11.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hdv.jianghu66.top

[U17] Py：初始化日志
来源：http://ybv.jyoumei.cn

logging.basicConfig(level=logging.INFO)
来源：http://ywo.ydzc1.top

[U18] Py：预编译正则
来源：http://nqx.mhx1999.top

pat = re.compile(r"\d+")
来源：http://sdd.chenlongwang.top

[U19] Py：正则替换带回调
来源：http://esi.zhaomingkeji.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://obc.guowangkeji.top

[U20] Py：缓存函数结果
来源：http://twj.yueranfly.top

@functools.lru_cache(maxsize=None)
来源：http://mme.yongpay.top

[U21] Py：自定义上下文管理器
来源：http://zzd.yj20258.top

@contextlib.contextmanager
来源：http://kyo.xziqi.cn

[U22] Py：矩阵转置
来源：http://woh.yj202588.top

list(zip(*m))
来源：http://iob.birdmap.top

[U23] Py：分块读取大文件
来源：http://ynu.chenzaomai.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qag.gotoacloud.top

[U24] Py：路径操作
来源：http://kpa.shuidangran.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fkh.hongshengwenyu.top

[U25] Py：CSV 按字典读
来源：http://txr.jqgufenzy.top

csv.DictReader(f)
来源：http://koq.ydzc1.top

[U26] Py：并发下载
来源：http://qsl.shzxlz.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kpf.guowangkeji.top

[U27] Py：异步 HTTP
来源：http://wqo.hfpthk.cn

aiohttp.ClientSession() 配合 async with
来源：http://hcy.ehwqpu.com

[U28] Py：类型别名
来源：http://lku.sufxvd.cn

UserId = int
来源：http://ect.zhaomingkeji.xyz

[U29] Py：属性校验
来源：http://mwx.guowangkeji.top

@property 与 @x.setter 配合
来源：http://uwa.pycfn.com

[U30] Py：数据类
来源：http://agw.haohaochexian.top

@dataclass(slots=True)
来源：http://mey.hnqzz.top

[U31] Py：单测
来源：http://dij.yj20258.top

python -m pytest -q
来源：http://nll.aibaodan.cn

[U32] Py：代码格式化
来源：http://lpw.jinqigufen.top

ruff format . && ruff check --fix .
来源：http://nwo.nanxinkj.top

[U33] Py：打包发布
来源：http://ajn.birdmap.top

python -m build  （依赖 pyproject.toml）
来源：http://fpj.ehwqpu.com

[U34] Py：判断编码
来源：http://aas.xylfe.cn

chardet.detect(raw)
来源：http://ljw.jinyuanbaomall.cn

[U35] Py：发送邮件
来源：http://iqt.yfazqb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nek.bbcook.cn

[U36] Py：定时任务
来源：http://dxn.52xcode.cn

schedule.every(10).minutes.do(job)
来源：http://eig.ybcxt.top

[U37] Py：读写 Excel
来源：http://ntw.cheryme.top

pandas.read_excel / DataFrame.to_excel
来源：http://wjo.jlsjyb.cn

[U38] Py：获取脚本所在目录
来源：http://rud.cucudq.cn

Path(__file__).resolve().parent
来源：http://ibg.ehwqpu.com

[U39] Py：判断是否在交互环境
来源：http://lrz.pengpengdd.cyou

sys.stdout.isatty()
来源：http://owt.bbcook.cn

[U40] Py：打印到标准错误
来源：http://qws.sysykeji.top

print("err", file=sys.stderr)
来源：http://jyp.ctjpmb.com

[U41] PHP：初始化 Composer 项目
来源：http://jzz.jinqigufen.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wvq.yj202588.top

[U42] PHP：PSR-4 自动加载
来源：http://zce.yueranfly.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vyw.c1oappe.top

[U43] PHP：声明命名空间
来源：http://vjx.zhengqikj.top

namespace App\Http;
来源：http://rns.hnxiangtu.top

[U44] PHP：开启严格类型
来源：http://urf.bbcook.cn

declare(strict_types=1);
来源：http://kwi.sysykeji.top

[U45] PHP：类型声明与返回类型
来源：http://rge.xziqi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://idc.zhixingplan.top

[U46] PHP：可空类型
来源：http://wcl.yuxming.cn

?string $name = null
来源：http://cke.zhaomingkeji.xyz

[U47] PHP：联合类型
来源：http://pwt.bbcook.cn

int|string $id
来源：http://mce.52xcode.cn

[U48] PHP：纯枚举
来源：http://der.316326.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sqn.redwolf501.top

[U49] PHP：只读属性
来源：http://nvg.cashguo.top

public readonly string $name
来源：http://fus.zhijiandao.cn

[U50] PHP：构造器属性提升
来源：http://nrw.gogol.net.cn

public function __construct(private int $id) {}
来源：http://xlb.wangdashe.top

[U51] PHP：数组解构
来源：http://itl.pengpengdd.cyou

[$a, $b] = $arr;
来源：http://hhd.0kj1m.cn

[U52] PHP：箭头函数
来源：http://sey.wangdashe.top

$double = fn($x) => $x * 2;
来源：http://jtk.ctjpmb.com

[U53] PHP：空合并运算符
来源：http://vgo.jinqigufen.top

$v = $a ?? $b ?? "default";
来源：http://ugp.sweek.top

[U54] PHP：空安全调用
来源：http://dhg.snrcjt.cn

$obj?->method()
来源：http://uzb.yfazqb.com

[U55] PHP：match 表达式
来源：http://ctf.iojbl.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iec.tianlin.xyz

[U56] PHP：命名参数
来源：http://zgm.shanyushiyangkeji.top

f(a: 1, b: 2)
来源：http://lie.jyoumei.cn

[U57] PHP：字符串插值
来源：http://fci.xuetiantiany.cn

"值: {$a}"
来源：http://ykp.bbcook.cn

[U58] PHP：数组三件套
来源：http://umx.haohaochexian.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rws.gzhubu.top

[U59] PHP：自定义排序
来源：http://aga.ivvv.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fvm.chenzaomai.com

[U60] PHP：JSON 编解码
来源：http://ngk.jinqigfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wzu.xinyue.icu


<!-- 参考信息 -->