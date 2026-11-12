代发 wailian999

[S37] C++：set
来源：http://yvn.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://feh.yj20258.top

[S38] C++：排序
来源：http://mvt.gotoacloud.top

std::sort(v.begin(), v.end());
来源：http://fzx.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://ixr.hammf.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://amy.cucudq.cn

[S40] C++：查找元素
来源：http://rra.hammf.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://afr.sxryk.cn

[S41] C++：类与构造函数
来源：http://tlt.sysykeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wzq.xylfe.cn

[S42] C++：继承与虚函数
来源：http://civ.gaohongyu789.top

class B : public Base { public: void f() override {} };
来源：http://mzc.aibaodan.cn

[S43] C++：智能指针
来源：http://hkh.hysaishi.cn

auto p = std::make_unique<int>(5);
来源：http://rby.xingfuxueyuan.xyz

[S44] C++：引用传参
来源：http://rlt.cheryme.top

void inc(int &x) { ++x; }
来源：http://oco.yuanzhike.top

[S45] C++：lambda
来源：http://rna.xingfuxueyuan.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://onm.ybcxt.top

[S46] C++：函数模板
来源：http://zcy.zdbjq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vak.zdbjq.cn

[S47] C++：结构化绑定遍历
来源：http://gue.316326.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rse.chenlongwang.top

[S48] C++：逐行读文件
来源：http://qdd.redwolf501.top

std::ifstream in("a.txt");  std::string line;
来源：http://mgs.nwbrower.top

while (std::getline(in, line)) { }
来源：http://nyf.zdbjq.cn

[S49] C++：写文件
来源：http://prm.yuxming.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lum.dianchejie.cn

[S50] C++：格式化数字
来源：http://tbo.yangfankeji.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qmo.zhoulong.xyz

[S51] C++：显式类型转换
来源：http://wxv.hfpthk.cn

static_cast<double>(a) / b
来源：http://hwk.xingfuxueyuan.xyz

[S52] C++：const 与 noexcept
来源：http://czy.sjlbkw.cn

int size() const noexcept { return n_; }
来源：http://vxr.svipenyu.cn

[S53] C++：移动语义
来源：http://toq.yfazqb.com

std::vector<int> w = std::move(v);
来源：http://mfx.pengpengdd.cyou

[S54] C++：异常处理
来源：http://ppw.yfazqb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kfh.dashuyun.cn

[S55] C++：结构化绑定
来源：http://hji.pengpengdd.cyou

auto [a, b] = std::make_pair(1, 2);
来源：http://crk.xingfuxueyuan.xyz

[S56] C++：optional
来源：http://wgq.shanyushiyangtech.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ccw.shuidangran.top

[S57] C++：编译期常量
来源：http://njt.svipenyu.cn

constexpr int N = 10;
来源：http://lyu.xziqi.cn

[S58] C++：命名空间
来源：http://hht.fanxiaobao.xyz

namespace ns { int f() { return 1; } }
来源：http://ozr.iojbl.cn

[S59] C++：静态断言
来源：http://gzr.tarul.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qda.tarul.cn

[S60] C++：遍历并删除元素
来源：http://jtg.xinyue.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cji.guannengcc.top

================================================================================
来源：http://ywa.hywenlv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vne.snrcjt.cn

================================================================================
来源：http://rps.yj20258888.top

[T01] Kotlin：Hello World
来源：http://pat.xziqi.cn

println("Hello")
来源：http://qwi.jqgufenzy.top

[T02] Kotlin：变量
来源：http://sdw.yuxming.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eix.hammf.cn

[T03] Kotlin：字符串模板
来源：http://esx.shanyushiyangkeji.top

"值: $b"
来源：http://clq.chenjidiqi.icu

[T04] Kotlin：空安全
来源：http://nyf.yueranfly.top

val n: String? = null;  n?.length
来源：http://hkc.cdnleiting.top

[T05] Kotlin：when 表达式
来源：http://gnu.tanke756.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jfb.dashuyun.cn

[T06] Kotlin：集合映射
来源：http://hht.zhengqikj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zsf.chenzaomai.com

[T07] Kotlin：集合过滤
来源：http://jqs.shangyingyoupin.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ufs.yanxiufei.cn

[T08] Kotlin：数据类
来源：http://ujk.iojbl.cn

data class User(val name: String, val age: Int)
来源：http://yxl.zhongyouzk.top

[T09] Kotlin：扩展函数
来源：http://zkd.ydjk.org.cn

fun String.exclaim() = this + "!"
来源：http://hiz.xziqi.cn

[T10] Kotlin：默认参数
来源：http://haq.dianchejie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gjq.gotoacloud.top

[T11] Kotlin：协程
来源：http://feu.pycfn.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://nus.chenjidiqi.icu

[T12] Kotlin：解构声明
来源：http://kyz.zdbjq.cn

val (a, b) = Pair(1, 2)
来源：http://gks.tarul.cn

[T13] Kotlin：只读 Map
来源：http://lip.nwbrower.top

val m = mapOf("a" to 1)
来源：http://met.havefunace.top

[T14] Kotlin：循环
来源：http://elw.fehbvm.com

for (i in 1..10) println(i)
来源：http://feh.wangdashe.top

[T15] Kotlin：接口
来源：http://tck.xuetiantiany.cn

interface Shape { fun area(): Double }
来源：http://wwy.yongpay.top

[T16] Swift：Hello World
来源：http://nqr.xingfuxueyuan.xyz

print("Hello")
来源：http://cuq.316326.xyz

[T17] Swift：变量与常量
来源：http://ogq.snrcjt.cn

var a = 1;  let b = 2
来源：http://qgp.sxryk.cn

[T18] Swift：字符串插值
来源：http://efd.xziqi.cn

"值: \(b)"
来源：http://gqg.mhx1999.top

[T19] Swift：可选绑定
来源：http://ije.aibaodan.cn

if let n = opt { print(n) }
来源：http://zod.9152youxi.cn

[T20] Swift：数组操作
来源：http://dod.zhaomingkeji.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://zba.iojbl.cn

[T21] Swift：遍历
来源：http://qvd.yongpay.top

for x in a { print(x) }
来源：http://vuw.zhixingplan.top

[T22] Swift：字典
来源：http://tyh.mhx1999.top

var d = ["a": 1];  d["b"] = 2
来源：http://cvq.aibaodan.cn

[T23] Swift：函数
来源：http://pka.hfpthk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wqy.hfpthk.cn

[T24] Swift：闭包
来源：http://rzd.pengpengdd.cyou

let f = { (x: Int) -> Int in x * 2 }
来源：http://ztd.bjfxy.top

[T25] Swift：结构体
来源：http://fqa.daria6918.cn

struct P { var x: Int }
来源：http://qjd.feifeiyinyue.top

[T26] Swift：类与重写
来源：http://csl.zhengqikj.top

class A: Base { override func f() {} }
来源：http://kzj.dianchejie.cn

[T27] Swift：错误处理
来源：http://wtz.c1oappe.top

do { try f() } catch { print(error) }
来源：http://yra.cucudq.cn

[T28] Swift：枚举
来源：http://xqq.tanke756.top

enum Color { case red, green }
来源：http://lsa.gogol.net.cn

[T29] Swift：guard 提前返回
来源：http://jcf.hnqzz.top

guard let x = opt else { return }
来源：http://wrk.xylfe.cn

[T30] Swift：协议
来源：http://hbl.chenlongwang.top

protocol Shape { func area() -> Double }
来源：http://sab.smart0.xyz

[T31] Lua：Hello World
来源：http://tlh.zycfv.cn

print("Hello")
来源：http://cyu.zdbjq.cn

[T32] Lua：局部变量
来源：http://fky.jianghu66.top

local a = 1
来源：http://uza.shanyushiyangtech.top

[T33] Lua：表（数组）
来源：http://khw.zhengqikj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://cpi.ydzc1.top

[T34] Lua：遍历表
来源：http://tzc.pengpengdd.cyou

for i, v in ipairs(t) do print(i, v) end
来源：http://woe.aizwys.cn

[T35] Lua：字典表
来源：http://deq.ehwqpu.com

local d = { a = 1 };  d.b = 2
来源：http://jdv.yj20258.top

[T36] Lua：函数
来源：http://ndf.ydzc1.top

function add(a, b) return a + b end
来源：http://qvd.hysaishi.cn

[T37] Lua：字符串拼接
来源：http://pmp.jlsjyb.cn

"a" .. "b"
来源：http://nld.nanxinkj.top

[T38] Lua：条件
来源：http://uwn.cashguo.top

if x > 0 then print("正") end
来源：http://vra.havefunace.top

[T39] Lua：模式匹配
来源：http://tzb.yanxiufei.cn

string.find(s, "%d+")
来源：http://wtm.cheryme.top

[T40] Lua：元表
来源：http://eto.guannengcc.top

setmetatable({}, { __index = base })
来源：http://unr.hnqzz.top

[T41] Perl：Hello World
来源：http://gkw.hfpthk.cn

print "Hello\n";
来源：http://jbk.hesvh.cn

[T42] Perl：变量类型
来源：http://gcx.wangdashe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zmw.hesvh.cn

[T43] Perl：字符串插值
来源：http://gsx.fengsongda.top

"值: $a"
来源：http://hvf.daxiang520.top

[T44] Perl：条件
来源：http://xms.316326.xyz

if ($a > 0) { print "正"; }
来源：http://lcm.yuanzhike.top

[T45] Perl：数组遍历
来源：http://sku.snrcjt.cn

for my $x (@arr) { print $x; }
来源：http://oeu.ywan-chungtsiang.top

[T46] Perl：哈希操作
来源：http://wpr.zhijiandao.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gib.guowangkeji.top

[T47] Perl：正则捕获
来源：http://tyf.fktsv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://btk.cqqwz.cn

[T48] Perl：正则替换
来源：http://zdf.0kj1m.cn

$s =~ s/old/new/g;
来源：http://fmi.ctjpmb.com

[T49] Perl：函数
来源：http://cpi.shangyingyoupin.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xao.ybcxt.top

[T50] Perl：逐行读文件
来源：http://uxb.sjlbkw.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sqa.zhiwuduotai.top

while (my $line = <$fh>) { print $line; }
来源：http://ihk.svipenyu.cn

[T51] Scala：Hello World
来源：http://dbl.aizwys.cn

println("Hello")
来源：http://jxa.yanxiufei.cn

[T52] Scala：变量
来源：http://vwe.gogol.net.cn

val a = 1;  var b = 2
来源：http://pyz.shuidangran.top

[T53] Scala：字符串插值
来源：http://miw.chenjidiqi.icu

s"值: $b"
来源：http://mrz.yanxiufei.cn

[T54] Scala：集合映射
来源：http://ijk.0kj1m.cn

List(1, 2, 3).map(_ * 2)
来源：http://jnt.nanxuanxn.top

[T55] Scala：集合过滤
来源：http://qvd.xingfuxueyuan.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://gey.aibaodan.cn

[T56] Scala：样例类
来源：http://gmb.jiagoushi.top

case class User(name: String, age: Int)
来源：http://jwy.vehdjk.com

[T57] Scala：模式匹配
来源：http://vyj.redwolf501.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://qhh.xuanzx.com

[T58] Scala：函数定义
来源：http://tpc.hesvh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qog.sxryk.cn

[T59] Scala：循环
来源：http://gat.yangfankeji.com

for (i <- 1 to 10) println(i)
来源：http://goa.xingfuxueyuan.xyz

[T60] Scala：折叠
来源：http://sby.zhijiandao.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uur.hongshengwenyu.top

================================================================================
来源：http://tuj.jqgfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lgp.shanyushiyangkeji.top

================================================================================
来源：http://owd.bbcook.cn

[U01] Py：创建虚拟环境
来源：http://mpg.andypj.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://lxn.zhongyouzk.top

[U02] Py：导出 / 安装依赖
来源：http://yox.xylfe.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rjk.hfpthk.cn

[U03] Py：加载 .env 配置
来源：http://svd.ivvv.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xpt.ppjwa.cn

[U04] Py：变量调试打印
来源：http://mpu.nanxinkj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eai.jqgfzy.top

[U05] Py：列表去重且保序
来源：http://urh.hysaishi.cn

list(dict.fromkeys(arr))
来源：http://sfh.yongpay.top

[U06] Py：合并两个字典
来源：http://uoy.nwbrower.top

{**a, **b}
来源：http://jlj.daria6918.cn

[U07] Py：反转字典键值
来源：http://ftk.svipenyu.cn

{v: k for k, v in d.items()}
来源：http://pns.chenlongwang.top

[U08] Py：展平二维列表
来源：http://ynp.jinqigfzy.top

[y for x in nested for y in x]
来源：http://cra.yuxming.cn

[U09] Py：字典取最大值的键
来源：http://cqf.nwbrower.top

max(d, key=d.get)
来源：http://lks.hammf.cn

[U10] Py：按值排序字典
来源：http://pjt.tian-w.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ofb.cucudq.cn

[U11] Py：生成器表达式
来源：http://ckh.shangyingyoupin.top

(x * 2 for x in arr)
来源：http://hng.yj202588.top

[U12] Py：取出现最多的 3 个元素
来源：http://bqa.andypj.xyz

Counter(arr).most_common(3)
来源：http://sqz.cdnleiting.top

[U13] Py：固定长度队列
来源：http://wpk.haohaochexian.top

deque(maxlen=10)
来源：http://wzw.zhoulong.xyz

[U14] Py：分组收集到列表
来源：http://hsd.wangdashe.top

defaultdict(list)
来源：http://vts.fengsongda.top

[U15] Py：高精度计时
来源：http://qpp.birdmap.top

t = time.perf_counter()
来源：http://pus.pengpengdd.cyou

[U16] Py：命令行参数解析
来源：http://one.jinqigufen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hto.ywan-chungtsiang.top

[U17] Py：初始化日志
来源：http://rdy.xuetiantiany.cn

logging.basicConfig(level=logging.INFO)
来源：http://ohx.kuanghao11.cn

[U18] Py：预编译正则
来源：http://mnx.sjlbkw.cn

pat = re.compile(r"\d+")
来源：http://ljf.sxryk.cn

[U19] Py：正则替换带回调
来源：http://etv.yj20258.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wlk.dianchejie.cn

[U20] Py：缓存函数结果
来源：http://xvl.jinghuilouyu.cn

@functools.lru_cache(maxsize=None)
来源：http://qcc.havefunace.top

[U21] Py：自定义上下文管理器
来源：http://kje.yanxiufei.cn

@contextlib.contextmanager
来源：http://jvk.gzhubu.top

[U22] Py：矩阵转置
来源：http://hhk.bjfxy.top

list(zip(*m))
来源：http://ljc.jinyuanbaomall.cn

[U23] Py：分块读取大文件
来源：http://pbo.aizwys.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pkh.sjlbkw.cn

[U24] Py：路径操作
来源：http://okp.zhixingplan.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ljp.ivvv.top

[U25] Py：CSV 按字典读
来源：http://nnc.zhengqikj.top

csv.DictReader(f)
来源：http://dof.jinyuanbaomall.cn

[U26] Py：并发下载
来源：http://fba.fehbvm.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bnh.aibaodan.cn

[U27] Py：异步 HTTP
来源：http://cyx.ppjwa.cn

aiohttp.ClientSession() 配合 async with
来源：http://wiw.zycfv.cn

[U28] Py：类型别名
来源：http://gns.yanxiufei.cn

UserId = int
来源：http://slr.uphjek.com

[U29] Py：属性校验
来源：http://dky.tian-w.cn

@property 与 @x.setter 配合
来源：http://fyp.zdbjq.cn

[U30] Py：数据类
来源：http://auv.ctjpmb.com

@dataclass(slots=True)
来源：http://hil.jlsjyb.cn

[U31] Py：单测
来源：http://sza.nwbrower.top

python -m pytest -q
来源：http://kxk.yj20258888.top

[U32] Py：代码格式化
来源：http://vwv.yj20258.top

ruff format . && ruff check --fix .
来源：http://kut.yj20258.top

[U33] Py：打包发布
来源：http://zpq.bbcook.cn

python -m build  （依赖 pyproject.toml）
来源：http://dvg.pycfn.com

[U34] Py：判断编码
来源：http://nmw.redwolf501.top

chardet.detect(raw)
来源：http://tbe.hongshengwenyu.top

[U35] Py：发送邮件
来源：http://bck.cdnleiting.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xvg.hongshengwenyu.top

[U36] Py：定时任务
来源：http://nmr.hammf.cn

schedule.every(10).minutes.do(job)
来源：http://nft.aibaodan.cn

[U37] Py：读写 Excel
来源：http://olv.xuetiantiany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hik.shanyushiyangtech.top

[U38] Py：获取脚本所在目录
来源：http://xla.ydjk.org.cn

Path(__file__).resolve().parent
来源：http://pfl.xuetiantiany.cn

[U39] Py：判断是否在交互环境
来源：http://ggk.jqgfzy.top

sys.stdout.isatty()
来源：http://xsm.hongshengwenyu.top

[U40] Py：打印到标准错误
来源：http://sct.fanxiaobao.xyz

print("err", file=sys.stderr)
来源：http://akg.shanyushiyangkeji.top

[U41] PHP：初始化 Composer 项目
来源：http://gyn.yangfankeji.com

composer init;  composer require guzzlehttp/guzzle
来源：http://bbf.tanke756.top

[U42] PHP：PSR-4 自动加载
来源：http://dat.yfazqb.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mwk.yongpay.top

[U43] PHP：声明命名空间
来源：http://uxm.fzhhl.top

namespace App\Http;
来源：http://dgf.hfpthk.cn

[U44] PHP：开启严格类型
来源：http://xco.kuanghao11.cn

declare(strict_types=1);
来源：http://vea.ivvv.top

[U45] PHP：类型声明与返回类型
来源：http://hxl.shanyushiyangtech.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://cjl.cqqwz.cn

[U46] PHP：可空类型
来源：http://ivi.yonumen.top

?string $name = null
来源：http://xom.tarul.cn

[U47] PHP：联合类型
来源：http://aeq.nwbrower.top

int|string $id
来源：http://cwi.xuetiantiany.cn

[U48] PHP：纯枚举
来源：http://att.hammf.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fbc.sysykeji.top

[U49] PHP：只读属性
来源：http://fki.xinyue.icu

public readonly string $name
来源：http://gtf.xuanzx.com

[U50] PHP：构造器属性提升
来源：http://ote.zdqjudy.top

public function __construct(private int $id) {}
来源：http://mmk.52xcode.cn

[U51] PHP：数组解构
来源：http://tqm.fzhhl.top

[$a, $b] = $arr;
来源：http://xkh.yj20258.top

[U52] PHP：箭头函数
来源：http://avd.kuanghao11.cn

$double = fn($x) => $x * 2;
来源：http://jwr.cucudq.cn

[U53] PHP：空合并运算符
来源：http://kkz.daxiang520.top

$v = $a ?? $b ?? "default";
来源：http://nls.ydzc1.top

[U54] PHP：空安全调用
来源：http://rtt.zhaomingkeji.xyz

$obj?->method()
来源：http://glt.chenzaomai.com

[U55] PHP：match 表达式
来源：http://fwr.hammf.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fhd.fzhhl.top

[U56] PHP：命名参数
来源：http://mrw.shanyushiyangtech.top

f(a: 1, b: 2)
来源：http://ypc.feifeiyinyue.top

[U57] PHP：字符串插值
来源：http://uys.ydzc1.top

"值: {$a}"
来源：http://dhd.dashuyun.cn

[U58] PHP：数组三件套
来源：http://jxe.zhongyouzk.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://omb.xylfe.cn

[U59] PHP：自定义排序
来源：http://rce.316326.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ugm.iojbl.cn

[U60] PHP：JSON 编解码
来源：http://fwv.fzhhl.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://byp.yuanzhike.top

[U61] PHP：正则
来源：http://uzp.jyoumei.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xqj.ivvv.top

[U62] PHP：日期对象
来源：http://nbs.gotoacloud.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nhz.jqgufenzy.top


<!-- 参考信息 -->