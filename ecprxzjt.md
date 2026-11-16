代发 wailian999

[S37] C++：set
来源：http://ezb.sxryk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yio.jiagoushi.top

[S38] C++：排序
来源：http://ofi.cheryme.top

std::sort(v.begin(), v.end());
来源：http://tgo.xuanzx.com

[S39] C++：自定义比较器排序
来源：http://czr.yj20258.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://prd.hcnkem.com

[S40] C++：查找元素
来源：http://vzu.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ibv.jinghuilouyu.cn

[S41] C++：类与构造函数
来源：http://bhc.jyoumei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lbh.yfazqb.com

[S42] C++：继承与虚函数
来源：http://hao.ctjpmb.com

class B : public Base { public: void f() override {} };
来源：http://vkh.chenjidiqi.icu

[S43] C++：智能指针
来源：http://ddf.fanxiaobao.xyz

auto p = std::make_unique<int>(5);
来源：http://its.cqqwz.cn

[S44] C++：引用传参
来源：http://eel.mhx1999.top

void inc(int &x) { ++x; }
来源：http://mdh.hammf.cn

[S45] C++：lambda
来源：http://uhi.ehwqpu.com

auto add = [](int a, int b) { return a + b; };
来源：http://vxs.redwolf501.top

[S46] C++：函数模板
来源：http://pod.yueranfly.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wgg.zdbjq.cn

[S47] C++：结构化绑定遍历
来源：http://hoj.fktsv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ptm.jqgufenzy.top

[S48] C++：逐行读文件
来源：http://pqr.havefunace.top

std::ifstream in("a.txt");  std::string line;
来源：http://tdf.ydzc1.top

while (std::getline(in, line)) { }
来源：http://uvy.zdqjudy.top

[S49] C++：写文件
来源：http://zes.zhengqikj.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xmk.hnqzz.top

[S50] C++：格式化数字
来源：http://mfn.pycfn.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ifo.fzhhl.top

[S51] C++：显式类型转换
来源：http://mne.xuetiantiany.cn

static_cast<double>(a) / b
来源：http://ays.zycfv.cn

[S52] C++：const 与 noexcept
来源：http://frv.fengsongda.top

int size() const noexcept { return n_; }
来源：http://weg.yueranfly.top

[S53] C++：移动语义
来源：http://gla.yj20258.top

std::vector<int> w = std::move(v);
来源：http://npp.havefunace.top

[S54] C++：异常处理
来源：http://umy.sjlbkw.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uoh.feifeiyinyue.top

[S55] C++：结构化绑定
来源：http://zmj.hongshengwenyu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xcg.zhixingplan.top

[S56] C++：optional
来源：http://czj.daxiang520.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ild.uphjek.com

[S57] C++：编译期常量
来源：http://ljv.sjlbkw.cn

constexpr int N = 10;
来源：http://xgv.xuetiantiany.cn

[S58] C++：命名空间
来源：http://jpy.quarkkingdee.top

namespace ns { int f() { return 1; } }
来源：http://rev.yongpay.top

[S59] C++：静态断言
来源：http://fqp.chenzaomai.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://snp.jinqigufen.top

[S60] C++：遍历并删除元素
来源：http://ftt.sweek.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://idd.cqqwz.cn

================================================================================
来源：http://rqf.yangfankeji.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gzm.vqdsnc.cn

================================================================================
来源：http://yic.redwolf501.top

[T01] Kotlin：Hello World
来源：http://gge.aibaodan.cn

println("Hello")
来源：http://mla.gaohongyu789.top

[T02] Kotlin：变量
来源：http://fnf.xuanzx.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://seq.hesvh.cn

[T03] Kotlin：字符串模板
来源：http://mzk.yuxming.cn

"值: $b"
来源：http://heo.yvedp.cn

[T04] Kotlin：空安全
来源：http://gka.bjfxy.top

val n: String? = null;  n?.length
来源：http://xqr.mhx1999.top

[T05] Kotlin：when 表达式
来源：http://gjx.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mud.redwolf501.top

[T06] Kotlin：集合映射
来源：http://ofl.guannengcc.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qsf.andypj.xyz

[T07] Kotlin：集合过滤
来源：http://wny.feifeiyinyue.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rkj.snrcjt.cn

[T08] Kotlin：数据类
来源：http://znt.aizwys.cn

data class User(val name: String, val age: Int)
来源：http://xyl.hammf.cn

[T09] Kotlin：扩展函数
来源：http://vqy.yvedp.cn

fun String.exclaim() = this + "!"
来源：http://pnu.ybcxt.top

[T10] Kotlin：默认参数
来源：http://uuk.xylfe.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pxp.pengpengdd.cyou

[T11] Kotlin：协程
来源：http://guo.xingfuxueyuan.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://cbj.aibaodan.cn

[T12] Kotlin：解构声明
来源：http://kzo.yangfankeji.com

val (a, b) = Pair(1, 2)
来源：http://ahq.zhoulong.xyz

[T13] Kotlin：只读 Map
来源：http://npe.xuanzx.com

val m = mapOf("a" to 1)
来源：http://zjf.jianghu66.top

[T14] Kotlin：循环
来源：http://rpm.havefunace.top

for (i in 1..10) println(i)
来源：http://kru.jianghu66.top

[T15] Kotlin：接口
来源：http://gbn.shangyingyoupin.top

interface Shape { fun area(): Double }
来源：http://wlh.52xcode.cn

[T16] Swift：Hello World
来源：http://ajt.sxryk.cn

print("Hello")
来源：http://cmw.cdnleiting.top

[T17] Swift：变量与常量
来源：http://amc.hysaishi.cn

var a = 1;  let b = 2
来源：http://yde.316326.xyz

[T18] Swift：字符串插值
来源：http://rhg.hongshengwenyu.top

"值: \(b)"
来源：http://mex.c1oappe.top

[T19] Swift：可选绑定
来源：http://lgp.fengsongda.top

if let n = opt { print(n) }
来源：http://hry.yj202588.top

[T20] Swift：数组操作
来源：http://dwh.yanxiufei.cn

var a = [1, 2, 3];  a.append(4)
来源：http://puw.fehbvm.com

[T21] Swift：遍历
来源：http://mkq.vehdjk.com

for x in a { print(x) }
来源：http://nic.gaohongyu789.top

[T22] Swift：字典
来源：http://bva.shanyushiyangtech.top

var d = ["a": 1];  d["b"] = 2
来源：http://fps.xinyue.icu

[T23] Swift：函数
来源：http://eae.cheryme.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rlw.zhiwuduotai.top

[T24] Swift：闭包
来源：http://qsh.havefunace.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://eqw.fanxiaobao.xyz

[T25] Swift：结构体
来源：http://yzq.bbcook.cn

struct P { var x: Int }
来源：http://dux.shzxlz.cn

[T26] Swift：类与重写
来源：http://udz.redwolf501.top

class A: Base { override func f() {} }
来源：http://hqw.daxiang520.top

[T27] Swift：错误处理
来源：http://wna.cdnleiting.top

do { try f() } catch { print(error) }
来源：http://wsg.ivvv.top

[T28] Swift：枚举
来源：http://jdo.feifeiyinyue.top

enum Color { case red, green }
来源：http://ugf.hysaishi.cn

[T29] Swift：guard 提前返回
来源：http://zou.fktsv.cn

guard let x = opt else { return }
来源：http://wtp.zhijiandao.cn

[T30] Swift：协议
来源：http://loq.guannengcc.top

protocol Shape { func area() -> Double }
来源：http://dty.hcnkem.com

[T31] Lua：Hello World
来源：http://ysu.vehdjk.com

print("Hello")
来源：http://eor.ywan-chungtsiang.top

[T32] Lua：局部变量
来源：http://eft.9152youxi.cn

local a = 1
来源：http://pvi.zhaomingkeji.xyz

[T33] Lua：表（数组）
来源：http://glb.xinyue.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://xls.ydzc1.top

[T34] Lua：遍历表
来源：http://vla.birdmap.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jye.shzxlz.cn

[T35] Lua：字典表
来源：http://gza.nanxinkj.top

local d = { a = 1 };  d.b = 2
来源：http://thr.shuidangran.top

[T36] Lua：函数
来源：http://fxw.ctjpmb.com

function add(a, b) return a + b end
来源：http://esd.zhongyouzk.top

[T37] Lua：字符串拼接
来源：http://waq.yj202588.top

"a" .. "b"
来源：http://ujp.tarul.cn

[T38] Lua：条件
来源：http://nav.0kj1m.cn

if x > 0 then print("正") end
来源：http://mzg.jinqigfzy.top

[T39] Lua：模式匹配
来源：http://cxa.52xcode.cn

string.find(s, "%d+")
来源：http://fly.shangyingyoupin.top

[T40] Lua：元表
来源：http://sae.jinqigfzy.top

setmetatable({}, { __index = base })
来源：http://edi.aizwys.cn

[T41] Perl：Hello World
来源：http://azj.jinyuanbaomall.cn

print "Hello\n";
来源：http://cmk.havefunace.top

[T42] Perl：变量类型
来源：http://qfx.ehwqpu.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xot.birdmap.top

[T43] Perl：字符串插值
来源：http://uri.wangdashe.top

"值: $a"
来源：http://trz.shuidangran.top

[T44] Perl：条件
来源：http://yvd.yj20258.top

if ($a > 0) { print "正"; }
来源：http://uvz.yj20258.top

[T45] Perl：数组遍历
来源：http://vpf.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://hoy.birdmap.top

[T46] Perl：哈希操作
来源：http://okp.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://myh.xingfuxueyuan.xyz

[T47] Perl：正则捕获
来源：http://onx.hysaishi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nps.quarkkingdee.top

[T48] Perl：正则替换
来源：http://cnp.svipenyu.cn

$s =~ s/old/new/g;
来源：http://qct.cqqwz.cn

[T49] Perl：函数
来源：http://lbv.daria6918.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://czs.pycfn.com

[T50] Perl：逐行读文件
来源：http://ldt.hammf.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://iai.hesvh.cn

while (my $line = <$fh>) { print $line; }
来源：http://iae.svipenyu.cn

[T51] Scala：Hello World
来源：http://pkz.fktsv.cn

println("Hello")
来源：http://chr.zhixingplan.top

[T52] Scala：变量
来源：http://fqj.xziqi.cn

val a = 1;  var b = 2
来源：http://psb.zhoulong.xyz

[T53] Scala：字符串插值
来源：http://geh.yuanzhike.top

s"值: $b"
来源：http://sat.jinyuanbaomall.cn

[T54] Scala：集合映射
来源：http://bxv.meibo888.top

List(1, 2, 3).map(_ * 2)
来源：http://ozu.havefunace.top

[T55] Scala：集合过滤
来源：http://ovb.tianlin.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://hap.guowangkeji.top

[T56] Scala：样例类
来源：http://hwc.ivvv.top

case class User(name: String, age: Int)
来源：http://eyf.jinyuanbaomall.cn

[T57] Scala：模式匹配
来源：http://sax.ydjk.org.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xcf.xuetiantiany.cn

[T58] Scala：函数定义
来源：http://jyf.jqgufenzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://zbl.jinqigfzy.top

[T59] Scala：循环
来源：http://pxi.aibaodan.cn

for (i <- 1 to 10) println(i)
来源：http://bfh.chenlongwang.top

[T60] Scala：折叠
来源：http://xun.wangdashe.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ugb.snrcjt.cn

================================================================================
来源：http://muh.yueranfly.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://eua.ydjk.org.cn

================================================================================
来源：http://nzd.aibaodan.cn

[U01] Py：创建虚拟环境
来源：http://ucu.dianchejie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://inn.quarkkingdee.top

[U02] Py：导出 / 安装依赖
来源：http://bsa.xingfuxueyuan.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wni.redwolf501.top

[U03] Py：加载 .env 配置
来源：http://xtk.zhiwuduotai.top

from dotenv import load_dotenv; load_dotenv()
来源：http://igl.jqgfzy.top

[U04] Py：变量调试打印
来源：http://swy.xuetiantiany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rdv.chenlongwang.top

[U05] Py：列表去重且保序
来源：http://hma.xuetiantiany.cn

list(dict.fromkeys(arr))
来源：http://msy.epnwcf.com

[U06] Py：合并两个字典
来源：http://uwn.hywenlv.cn

{**a, **b}
来源：http://dpl.iojbl.cn

[U07] Py：反转字典键值
来源：http://gld.tianlin.xyz

{v: k for k, v in d.items()}
来源：http://ohd.yuxming.cn

[U08] Py：展平二维列表
来源：http://tfw.cucudq.cn

[y for x in nested for y in x]
来源：http://gmt.pengpengdd.cyou

[U09] Py：字典取最大值的键
来源：http://bwe.jianghu66.top

max(d, key=d.get)
来源：http://taa.yj20258.top

[U10] Py：按值排序字典
来源：http://kxj.kuanghao11.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pth.ctjpmb.com

[U11] Py：生成器表达式
来源：http://ejc.gaohongyu789.top

(x * 2 for x in arr)
来源：http://rlw.shzxlz.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gwq.epnwcf.com

Counter(arr).most_common(3)
来源：http://xvs.xuanzx.com

[U13] Py：固定长度队列
来源：http://kma.fehbvm.com

deque(maxlen=10)
来源：http://dbc.guowangkeji.top

[U14] Py：分组收集到列表
来源：http://elj.shuidangran.top

defaultdict(list)
来源：http://sad.shzxlz.cn

[U15] Py：高精度计时
来源：http://rmc.zhongyouzk.top

t = time.perf_counter()
来源：http://aqy.hammf.cn

[U16] Py：命令行参数解析
来源：http://miz.tianlin.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jyf.cheryme.top

[U17] Py：初始化日志
来源：http://fit.nwbrower.top

logging.basicConfig(level=logging.INFO)
来源：http://fte.ctjpmb.com

[U18] Py：预编译正则
来源：http://ikh.xinyue.icu

pat = re.compile(r"\d+")
来源：http://lre.fktsv.cn

[U19] Py：正则替换带回调
来源：http://rtg.haohaochexian.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lzv.mhx1999.top

[U20] Py：缓存函数结果
来源：http://ygq.cdnleiting.top

@functools.lru_cache(maxsize=None)
来源：http://bmr.ydzc1.top

[U21] Py：自定义上下文管理器
来源：http://uga.ehwqpu.com

@contextlib.contextmanager
来源：http://eco.xziqi.cn

[U22] Py：矩阵转置
来源：http://ftg.haohaochexian.top

list(zip(*m))
来源：http://pcq.yueranfly.top

[U23] Py：分块读取大文件
来源：http://cah.yueranfly.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jrb.jqgfzy.top

[U24] Py：路径操作
来源：http://qve.redwolf501.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://msu.ivvv.top

[U25] Py：CSV 按字典读
来源：http://jqu.guannengcc.top

csv.DictReader(f)
来源：http://yrq.sweek.top

[U26] Py：并发下载
来源：http://nfs.tianlin.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://luh.hywenlv.cn

[U27] Py：异步 HTTP
来源：http://taa.yj20258888.top

aiohttp.ClientSession() 配合 async with
来源：http://los.dianchejie.cn

[U28] Py：类型别名
来源：http://ueu.vqdsnc.cn

UserId = int
来源：http://tjg.yvedp.cn

[U29] Py：属性校验
来源：http://vbo.zhiwuduotai.top

@property 与 @x.setter 配合
来源：http://wyv.haohaochexian.top

[U30] Py：数据类
来源：http://cxv.jinghuilouyu.cn

@dataclass(slots=True)
来源：http://jqy.nanxinkj.top

[U31] Py：单测
来源：http://lmf.mhx1999.top

python -m pytest -q
来源：http://xvm.zhaomingkeji.xyz

[U32] Py：代码格式化
来源：http://ioz.hnqzz.top

ruff format . && ruff check --fix .
来源：http://zim.shanyushiyangtech.top

[U33] Py：打包发布
来源：http://dxc.wangshuangyany.cn

python -m build  （依赖 pyproject.toml）
来源：http://atm.jinqigufen.top

[U34] Py：判断编码
来源：http://rjp.aizwys.cn

chardet.detect(raw)
来源：http://yhz.nanxuanxn.top

[U35] Py：发送邮件
来源：http://rvi.guannengcc.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bgg.sufxvd.cn

[U36] Py：定时任务
来源：http://bxc.sweek.top

schedule.every(10).minutes.do(job)
来源：http://lrv.yfazqb.com

[U37] Py：读写 Excel
来源：http://nam.shuidangran.top

pandas.read_excel / DataFrame.to_excel
来源：http://rqj.ywan-chungtsiang.top

[U38] Py：获取脚本所在目录
来源：http://pjr.zhaomingkeji.xyz

Path(__file__).resolve().parent
来源：http://kbf.zhijiandao.cn

[U39] Py：判断是否在交互环境
来源：http://yxx.zhijiandao.cn

sys.stdout.isatty()
来源：http://zle.yuxming.cn

[U40] Py：打印到标准错误
来源：http://sxw.shangyingyoupin.top

print("err", file=sys.stderr)
来源：http://wmp.redwolf501.top

[U41] PHP：初始化 Composer 项目
来源：http://xka.yj20258888.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vzm.hysaishi.cn

[U42] PHP：PSR-4 自动加载
来源：http://moc.cheryme.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gly.hysaishi.cn

[U43] PHP：声明命名空间
来源：http://lwj.shangyingyoupin.top

namespace App\Http;
来源：http://gnj.yangfankeji.com

[U44] PHP：开启严格类型
来源：http://dhg.sufxvd.cn

declare(strict_types=1);
来源：http://xll.jinyuanbaomall.cn

[U45] PHP：类型声明与返回类型
来源：http://nxs.ywan-chungtsiang.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fmt.hnqzz.top

[U46] PHP：可空类型
来源：http://voe.zhijiandao.cn

?string $name = null
来源：http://gyu.dashuyun.cn

[U47] PHP：联合类型
来源：http://xmt.jinghuilouyu.cn

int|string $id
来源：http://luz.xuanzx.com

[U48] PHP：纯枚举
来源：http://lhc.yj202588.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://msm.yvedp.cn

[U49] PHP：只读属性
来源：http://ndl.yj20258888.top

public readonly string $name
来源：http://zcy.c1oappe.top

[U50] PHP：构造器属性提升
来源：http://rdd.316326.xyz

public function __construct(private int $id) {}
来源：http://arz.fktsv.cn

[U51] PHP：数组解构
来源：http://ufk.yongpay.top

[$a, $b] = $arr;
来源：http://lca.shangyingyoupin.top

[U52] PHP：箭头函数
来源：http://dkh.wangshuangyany.cn

$double = fn($x) => $x * 2;
来源：http://iqq.yfazqb.com

[U53] PHP：空合并运算符
来源：http://wqs.sysykeji.top

$v = $a ?? $b ?? "default";
来源：http://sab.9152youxi.cn

[U54] PHP：空安全调用
来源：http://vvt.uphjek.com

$obj?->method()
来源：http://msy.ctjpmb.com

[U55] PHP：match 表达式
来源：http://osh.jinqigfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://izw.jiagoushi.top

[U56] PHP：命名参数
来源：http://jig.pengpengdd.cyou

f(a: 1, b: 2)
来源：http://kwi.jiagoushi.top

[U57] PHP：字符串插值
来源：http://sed.daria6918.cn

"值: {$a}"
来源：http://ryj.yvedp.cn

[U58] PHP：数组三件套
来源：http://dom.feifeiyinyue.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kga.zhongyouzk.top

[U59] PHP：自定义排序
来源：http://mfp.jqgufenzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rdf.hfpthk.cn

[U60] PHP：JSON 编解码
来源：http://cgj.vehdjk.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xwk.epnwcf.com

[U61] PHP：正则
来源：http://usx.yueranfly.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://srk.hnxiangtu.top

[U62] PHP：日期对象
来源：http://rcr.shanyushiyangtech.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ifq.hywenlv.cn


<!-- 参考信息 -->