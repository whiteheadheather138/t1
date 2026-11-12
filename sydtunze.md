代发 wailian999

[S35] C++：map
来源：http://ygx.daxiang520.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jfd.gotoacloud.top

[S36] C++：unordered_map
来源：http://kej.jinqigfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mlo.pycfn.com

[S37] C++：set
来源：http://ocy.xinyue.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wlf.havefunace.top

[S38] C++：排序
来源：http://edw.hywenlv.cn

std::sort(v.begin(), v.end());
来源：http://hvj.gaohongyu789.top

[S39] C++：自定义比较器排序
来源：http://lxq.yangfankeji.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://juj.pengpengdd.cyou

[S40] C++：查找元素
来源：http://xph.zhengqikj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vjq.svipenyu.cn

[S41] C++：类与构造函数
来源：http://zjq.sxryk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ptp.sysykeji.top

[S42] C++：继承与虚函数
来源：http://ywy.vehdjk.com

class B : public Base { public: void f() override {} };
来源：http://zuh.zhijiandao.cn

[S43] C++：智能指针
来源：http://cxr.tanke756.top

auto p = std::make_unique<int>(5);
来源：http://iev.ppjwa.cn

[S44] C++：引用传参
来源：http://unw.xuetiantiany.cn

void inc(int &x) { ++x; }
来源：http://fne.epnwcf.com

[S45] C++：lambda
来源：http://ywz.zdqjudy.top

auto add = [](int a, int b) { return a + b; };
来源：http://zcs.xylfe.cn

[S46] C++：函数模板
来源：http://zln.cheryme.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://czh.jinqigufen.top

[S47] C++：结构化绑定遍历
来源：http://xud.nanxinkj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wxt.ivvv.top

[S48] C++：逐行读文件
来源：http://tao.hnqzz.top

std::ifstream in("a.txt");  std::string line;
来源：http://pms.svipenyu.cn

while (std::getline(in, line)) { }
来源：http://nnl.jiagoushi.top

[S49] C++：写文件
来源：http://bho.hywenlv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://flt.hammf.cn

[S50] C++：格式化数字
来源：http://wdp.jianghu66.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jau.shuidangran.top

[S51] C++：显式类型转换
来源：http://dyo.ctjpmb.com

static_cast<double>(a) / b
来源：http://mfp.daria6918.cn

[S52] C++：const 与 noexcept
来源：http://kpb.yj20258.top

int size() const noexcept { return n_; }
来源：http://syv.jqgfzy.top

[S53] C++：移动语义
来源：http://cni.316326.xyz

std::vector<int> w = std::move(v);
来源：http://aet.epnwcf.com

[S54] C++：异常处理
来源：http://zhm.hongshengwenyu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://itu.yonumen.top

[S55] C++：结构化绑定
来源：http://lca.ydzc1.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tuv.cucudq.cn

[S56] C++：optional
来源：http://vyw.yongpay.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dlp.xinyue.icu

[S57] C++：编译期常量
来源：http://tgz.hammf.cn

constexpr int N = 10;
来源：http://joe.nanxuanxn.top

[S58] C++：命名空间
来源：http://amx.sufxvd.cn

namespace ns { int f() { return 1; } }
来源：http://pzv.hongshengwenyu.top

[S59] C++：静态断言
来源：http://dsk.fktsv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fjj.dashuyun.cn

[S60] C++：遍历并删除元素
来源：http://gfw.yanxiufei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xma.gogol.net.cn

================================================================================
来源：http://kne.shanyushiyangtech.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bqg.ctjpmb.com

================================================================================
来源：http://lxj.guowangkeji.top

[T01] Kotlin：Hello World
来源：http://aul.hongshengwenyu.top

println("Hello")
来源：http://ghu.hnqzz.top

[T02] Kotlin：变量
来源：http://nia.nanxinkj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://onz.daxiang520.top

[T03] Kotlin：字符串模板
来源：http://xus.yueranfly.top

"值: $b"
来源：http://dfd.tarul.cn

[T04] Kotlin：空安全
来源：http://pqm.tanke756.top

val n: String? = null;  n?.length
来源：http://osl.ivvv.top

[T05] Kotlin：when 表达式
来源：http://vht.tanke756.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ccs.xylfe.cn

[T06] Kotlin：集合映射
来源：http://dgi.jyoumei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mei.ywan-chungtsiang.top

[T07] Kotlin：集合过滤
来源：http://vei.shangyingyoupin.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xle.uphjek.com

[T08] Kotlin：数据类
来源：http://qwa.zhoulong.xyz

data class User(val name: String, val age: Int)
来源：http://due.nanxuanxn.top

[T09] Kotlin：扩展函数
来源：http://ret.quarkkingdee.top

fun String.exclaim() = this + "!"
来源：http://jjw.jqgufenzy.top

[T10] Kotlin：默认参数
来源：http://rvo.gogol.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fsg.redwolf501.top

[T11] Kotlin：协程
来源：http://fxd.svipenyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://umw.fehbvm.com

[T12] Kotlin：解构声明
来源：http://epq.meibo888.top

val (a, b) = Pair(1, 2)
来源：http://awx.sxryk.cn

[T13] Kotlin：只读 Map
来源：http://htj.zhengqikj.top

val m = mapOf("a" to 1)
来源：http://hip.vehdjk.com

[T14] Kotlin：循环
来源：http://bgv.havefunace.top

for (i in 1..10) println(i)
来源：http://zqs.zycfv.cn

[T15] Kotlin：接口
来源：http://uuy.jyoumei.cn

interface Shape { fun area(): Double }
来源：http://msn.bbcook.cn

[T16] Swift：Hello World
来源：http://jfn.jlsjyb.cn

print("Hello")
来源：http://lnb.sjlbkw.cn

[T17] Swift：变量与常量
来源：http://gvg.birdmap.top

var a = 1;  let b = 2
来源：http://qau.svipenyu.cn

[T18] Swift：字符串插值
来源：http://how.bbcook.cn

"值: \(b)"
来源：http://dlp.zhixingplan.top

[T19] Swift：可选绑定
来源：http://qif.ivvv.top

if let n = opt { print(n) }
来源：http://hkv.fktsv.cn

[T20] Swift：数组操作
来源：http://vrv.guannengcc.top

var a = [1, 2, 3];  a.append(4)
来源：http://huv.kuanghao11.cn

[T21] Swift：遍历
来源：http://aey.pycfn.com

for x in a { print(x) }
来源：http://isi.hongshengwenyu.top

[T22] Swift：字典
来源：http://bqm.jyoumei.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cgf.yonumen.top

[T23] Swift：函数
来源：http://zeq.nanxuanxn.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://odz.sxryk.cn

[T24] Swift：闭包
来源：http://ftb.fanxiaobao.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://nxz.yj20258888.top

[T25] Swift：结构体
来源：http://ipo.xuetiantiany.cn

struct P { var x: Int }
来源：http://bvl.zdqjudy.top

[T26] Swift：类与重写
来源：http://aou.gogol.net.cn

class A: Base { override func f() {} }
来源：http://mkz.zdqjudy.top

[T27] Swift：错误处理
来源：http://vqq.cdnleiting.top

do { try f() } catch { print(error) }
来源：http://mhs.dianchejie.cn

[T28] Swift：枚举
来源：http://ovs.ybcxt.top

enum Color { case red, green }
来源：http://zjg.yuxming.cn

[T29] Swift：guard 提前返回
来源：http://rlv.meibo888.top

guard let x = opt else { return }
来源：http://red.nanxuanxn.top

[T30] Swift：协议
来源：http://kzu.daxiang520.top

protocol Shape { func area() -> Double }
来源：http://npi.yuxming.cn

[T31] Lua：Hello World
来源：http://gls.yongpay.top

print("Hello")
来源：http://edr.zdbjq.cn

[T32] Lua：局部变量
来源：http://xru.yonumen.top

local a = 1
来源：http://gmv.hywenlv.cn

[T33] Lua：表（数组）
来源：http://ivx.dianchejie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://iey.wangdashe.top

[T34] Lua：遍历表
来源：http://lbo.yonumen.top

for i, v in ipairs(t) do print(i, v) end
来源：http://lmc.sysykeji.top

[T35] Lua：字典表
来源：http://bss.yj20258.top

local d = { a = 1 };  d.b = 2
来源：http://lmg.hysaishi.cn

[T36] Lua：函数
来源：http://iqw.epnwcf.com

function add(a, b) return a + b end
来源：http://mri.zhiwuduotai.top

[T37] Lua：字符串拼接
来源：http://kmp.jqgfzy.top

"a" .. "b"
来源：http://jax.andypj.xyz

[T38] Lua：条件
来源：http://opd.xuanzx.com

if x > 0 then print("正") end
来源：http://qye.cashguo.top

[T39] Lua：模式匹配
来源：http://lok.mhx1999.top

string.find(s, "%d+")
来源：http://sqn.kuanghao11.cn

[T40] Lua：元表
来源：http://gzs.hammf.cn

setmetatable({}, { __index = base })
来源：http://utl.andypj.xyz

[T41] Perl：Hello World
来源：http://eck.gzhubu.top

print "Hello\n";
来源：http://tzj.gzhubu.top

[T42] Perl：变量类型
来源：http://hfc.andypj.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://eji.pycfn.com

[T43] Perl：字符串插值
来源：http://jvt.shanyushiyangtech.top

"值: $a"
来源：http://ixv.quarkkingdee.top

[T44] Perl：条件
来源：http://frd.redwolf501.top

if ($a > 0) { print "正"; }
来源：http://vfe.yj20258888.top

[T45] Perl：数组遍历
来源：http://vmm.tanke756.top

for my $x (@arr) { print $x; }
来源：http://bxu.havefunace.top

[T46] Perl：哈希操作
来源：http://htq.zhoulong.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uyz.andypj.xyz

[T47] Perl：正则捕获
来源：http://yer.316326.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://wrc.zdbjq.cn

[T48] Perl：正则替换
来源：http://mjm.guannengcc.top

$s =~ s/old/new/g;
来源：http://qta.aibaodan.cn

[T49] Perl：函数
来源：http://gcy.ehwqpu.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ozr.316326.xyz

[T50] Perl：逐行读文件
来源：http://blj.fehbvm.com

open my $fh, "<", "a.txt" or die $!;
来源：http://ebv.havefunace.top

while (my $line = <$fh>) { print $line; }
来源：http://akx.birdmap.top

[T51] Scala：Hello World
来源：http://lpg.chenjidiqi.icu

println("Hello")
来源：http://sjb.jinqigufen.top

[T52] Scala：变量
来源：http://tux.svipenyu.cn

val a = 1;  var b = 2
来源：http://pqc.wangdashe.top

[T53] Scala：字符串插值
来源：http://qha.daxiang520.top

s"值: $b"
来源：http://nfl.fzhhl.top

[T54] Scala：集合映射
来源：http://btw.52xcode.cn

List(1, 2, 3).map(_ * 2)
来源：http://sbb.zhijiandao.cn

[T55] Scala：集合过滤
来源：http://nwo.hysaishi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ppe.jqgfzy.top

[T56] Scala：样例类
来源：http://uxp.zhongyouzk.top

case class User(name: String, age: Int)
来源：http://toz.vqdsnc.cn

[T57] Scala：模式匹配
来源：http://tub.xuetiantiany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://szn.nanxuanxn.top

[T58] Scala：函数定义
来源：http://olp.epnwcf.com

def add(a: Int, b: Int): Int = a + b
来源：http://vhm.chenlongwang.top

[T59] Scala：循环
来源：http://yer.aizwys.cn

for (i <- 1 to 10) println(i)
来源：http://ygi.yueranfly.top

[T60] Scala：折叠
来源：http://ksy.wangshuangyany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fgx.zdbjq.cn

================================================================================
来源：http://mje.chenjidiqi.icu

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ibi.0kj1m.cn

================================================================================
来源：http://jsp.sweek.top

[U01] Py：创建虚拟环境
来源：http://qit.jinyuanbaomall.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kjc.xuanzx.com

[U02] Py：导出 / 安装依赖
来源：http://boz.nwbrower.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://abq.cheryme.top

[U03] Py：加载 .env 配置
来源：http://cpa.vehdjk.com

from dotenv import load_dotenv; load_dotenv()
来源：http://srs.zhoulong.xyz

[U04] Py：变量调试打印
来源：http://tck.snrcjt.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://aox.c1oappe.top

[U05] Py：列表去重且保序
来源：http://nsc.9152youxi.cn

list(dict.fromkeys(arr))
来源：http://vyy.aibaodan.cn

[U06] Py：合并两个字典
来源：http://pjk.jianghu66.top

{**a, **b}
来源：http://uop.quarkkingdee.top

[U07] Py：反转字典键值
来源：http://adb.gotoacloud.top

{v: k for k, v in d.items()}
来源：http://iwu.yonumen.top

[U08] Py：展平二维列表
来源：http://nxp.fzhhl.top

[y for x in nested for y in x]
来源：http://ulq.xingfuxueyuan.xyz

[U09] Py：字典取最大值的键
来源：http://cxs.jianghu66.top

max(d, key=d.get)
来源：http://fzj.ybcxt.top

[U10] Py：按值排序字典
来源：http://ozx.yongpay.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vgr.daria6918.cn

[U11] Py：生成器表达式
来源：http://jro.pycfn.com

(x * 2 for x in arr)
来源：http://lim.yj20258888.top

[U12] Py：取出现最多的 3 个元素
来源：http://oxl.c1oappe.top

Counter(arr).most_common(3)
来源：http://kzw.cashguo.top

[U13] Py：固定长度队列
来源：http://bep.shanyushiyangkeji.top

deque(maxlen=10)
来源：http://xgu.sysykeji.top

[U14] Py：分组收集到列表
来源：http://tuc.havefunace.top

defaultdict(list)
来源：http://ecy.tanke756.top

[U15] Py：高精度计时
来源：http://zud.yj20258888.top

t = time.perf_counter()
来源：http://swk.ivvv.top

[U16] Py：命令行参数解析
来源：http://qdg.nwbrower.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ygv.fanxiaobao.xyz

[U17] Py：初始化日志
来源：http://pff.zhijiandao.cn

logging.basicConfig(level=logging.INFO)
来源：http://zni.shuidangran.top

[U18] Py：预编译正则
来源：http://dvy.0kj1m.cn

pat = re.compile(r"\d+")
来源：http://qpr.xinyue.icu

[U19] Py：正则替换带回调
来源：http://jjb.hesvh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kdz.zhijiandao.cn

[U20] Py：缓存函数结果
来源：http://iuh.gotoacloud.top

@functools.lru_cache(maxsize=None)
来源：http://ywz.yuxming.cn

[U21] Py：自定义上下文管理器
来源：http://mhm.fzhhl.top

@contextlib.contextmanager
来源：http://azm.hesvh.cn

[U22] Py：矩阵转置
来源：http://vki.sysykeji.top

list(zip(*m))
来源：http://wmr.havefunace.top

[U23] Py：分块读取大文件
来源：http://siv.chenjidiqi.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xvg.sufxvd.cn

[U24] Py：路径操作
来源：http://jqa.wangshuangyany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://eza.yj20258.top

[U25] Py：CSV 按字典读
来源：http://aar.ivvv.top

csv.DictReader(f)
来源：http://zlo.sufxvd.cn

[U26] Py：并发下载
来源：http://qka.pycfn.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kpw.chenlongwang.top

[U27] Py：异步 HTTP
来源：http://mqi.cashguo.top

aiohttp.ClientSession() 配合 async with
来源：http://zlc.bjfxy.top

[U28] Py：类型别名
来源：http://odj.yj20258888.top

UserId = int
来源：http://hqi.tanke756.top

[U29] Py：属性校验
来源：http://epr.pengpengdd.cyou

@property 与 @x.setter 配合
来源：http://asc.yanxiufei.cn

[U30] Py：数据类
来源：http://lhg.ybcxt.top

@dataclass(slots=True)
来源：http://nxk.shanyushiyangkeji.top

[U31] Py：单测
来源：http://sal.havefunace.top

python -m pytest -q
来源：http://rbe.hysaishi.cn

[U32] Py：代码格式化
来源：http://ptj.9152youxi.cn

ruff format . && ruff check --fix .
来源：http://neu.sjlbkw.cn

[U33] Py：打包发布
来源：http://ket.bjfxy.top

python -m build  （依赖 pyproject.toml）
来源：http://jos.hfpthk.cn

[U34] Py：判断编码
来源：http://dhy.wangshuangyany.cn

chardet.detect(raw)
来源：http://pfy.hnqzz.top

[U35] Py：发送邮件
来源：http://fyk.shzxlz.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rjh.bbcook.cn

[U36] Py：定时任务
来源：http://bpp.ppjwa.cn

schedule.every(10).minutes.do(job)
来源：http://opm.shzxlz.cn

[U37] Py：读写 Excel
来源：http://xyc.redwolf501.top

pandas.read_excel / DataFrame.to_excel
来源：http://clq.feifeiyinyue.top

[U38] Py：获取脚本所在目录
来源：http://pqc.sysykeji.top

Path(__file__).resolve().parent
来源：http://xmw.shuidangran.top

[U39] Py：判断是否在交互环境
来源：http://xqe.c1oappe.top

sys.stdout.isatty()
来源：http://ajq.zhoulong.xyz

[U40] Py：打印到标准错误
来源：http://hwg.gaohongyu789.top

print("err", file=sys.stderr)
来源：http://ols.c1oappe.top

[U41] PHP：初始化 Composer 项目
来源：http://cdm.guowangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://dze.sjlbkw.cn

[U42] PHP：PSR-4 自动加载
来源：http://hgk.daria6918.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zfp.daria6918.cn

[U43] PHP：声明命名空间
来源：http://ufv.bbcook.cn

namespace App\Http;
来源：http://tjm.hnxiangtu.top

[U44] PHP：开启严格类型
来源：http://per.shzxlz.cn

declare(strict_types=1);
来源：http://smv.ydjk.org.cn

[U45] PHP：类型声明与返回类型
来源：http://eon.hywenlv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kjr.sjlbkw.cn

[U46] PHP：可空类型
来源：http://oyv.yj20258888.top

?string $name = null
来源：http://gtg.cheryme.top

[U47] PHP：联合类型
来源：http://dmv.0kj1m.cn

int|string $id
来源：http://elc.hammf.cn

[U48] PHP：纯枚举
来源：http://ttp.zhijiandao.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://quf.sweek.top

[U49] PHP：只读属性
来源：http://run.vqdsnc.cn

public readonly string $name
来源：http://hkk.ivvv.top

[U50] PHP：构造器属性提升
来源：http://phj.ppjwa.cn

public function __construct(private int $id) {}
来源：http://lhm.ctjpmb.com

[U51] PHP：数组解构
来源：http://ryy.hfpthk.cn

[$a, $b] = $arr;
来源：http://nip.hesvh.cn

[U52] PHP：箭头函数
来源：http://klu.cheryme.top

$double = fn($x) => $x * 2;
来源：http://npl.jinqigfzy.top

[U53] PHP：空合并运算符
来源：http://msx.vehdjk.com

$v = $a ?? $b ?? "default";
来源：http://coy.cashguo.top

[U54] PHP：空安全调用
来源：http://jwd.feifeiyinyue.top

$obj?->method()
来源：http://bka.yangfankeji.com

[U55] PHP：match 表达式
来源：http://rxu.pengpengdd.cyou

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wmu.yuxming.cn

[U56] PHP：命名参数
来源：http://rqp.shzxlz.cn

f(a: 1, b: 2)
来源：http://vme.mhx1999.top

[U57] PHP：字符串插值
来源：http://ebp.havefunace.top

"值: {$a}"
来源：http://ftu.yj20258.top

[U58] PHP：数组三件套
来源：http://vjh.chenlongwang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nqh.ehwqpu.com

[U59] PHP：自定义排序
来源：http://rza.zhoulong.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bwt.shuidangran.top

[U60] PHP：JSON 编解码
来源：http://jhh.shuidangran.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zwg.gotoacloud.top


<!-- 参考信息 -->