代发 wailian999

[S39] C++：自定义比较器排序
来源：http://zaq.zhoulong.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oap.kuanghao11.cn

[S40] C++：查找元素
来源：http://zcg.epnwcf.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xoy.fehbvm.com

[S41] C++：类与构造函数
来源：http://rta.jiagoushi.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jbi.wangdashe.top

[S42] C++：继承与虚函数
来源：http://sep.xuetiantiany.cn

class B : public Base { public: void f() override {} };
来源：http://rht.shanyushiyangtech.top

[S43] C++：智能指针
来源：http://lfm.nwbrower.top

auto p = std::make_unique<int>(5);
来源：http://tzr.zdbjq.cn

[S44] C++：引用传参
来源：http://efs.52xcode.cn

void inc(int &x) { ++x; }
来源：http://zpr.yvedp.cn

[S45] C++：lambda
来源：http://qry.pycfn.com

auto add = [](int a, int b) { return a + b; };
来源：http://xya.nwbrower.top

[S46] C++：函数模板
来源：http://hmw.jinqigfzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://anl.xylfe.cn

[S47] C++：结构化绑定遍历
来源：http://hlp.xinyue.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rdc.birdmap.top

[S48] C++：逐行读文件
来源：http://pev.daria6918.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wnk.daria6918.cn

while (std::getline(in, line)) { }
来源：http://tvh.jiagoushi.top

[S49] C++：写文件
来源：http://asc.hnxiangtu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vbv.cheryme.top

[S50] C++：格式化数字
来源：http://wmi.hongshengwenyu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fau.zhoulong.xyz

[S51] C++：显式类型转换
来源：http://foh.shanyushiyangtech.top

static_cast<double>(a) / b
来源：http://dwb.smart0.xyz

[S52] C++：const 与 noexcept
来源：http://czt.hammf.cn

int size() const noexcept { return n_; }
来源：http://rbo.xinyue.icu

[S53] C++：移动语义
来源：http://urz.tian-w.cn

std::vector<int> w = std::move(v);
来源：http://wky.shanyushiyangtech.top

[S54] C++：异常处理
来源：http://vub.gotoacloud.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hho.zhiwuduotai.top

[S55] C++：结构化绑定
来源：http://tvh.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fpx.cucudq.cn

[S56] C++：optional
来源：http://qlk.birdmap.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qwz.yj20258888.top

[S57] C++：编译期常量
来源：http://gio.smart0.xyz

constexpr int N = 10;
来源：http://mwc.birdmap.top

[S58] C++：命名空间
来源：http://srz.aibaodan.cn

namespace ns { int f() { return 1; } }
来源：http://edu.sufxvd.cn

[S59] C++：静态断言
来源：http://zko.fanxiaobao.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zkx.nanxinkj.top

[S60] C++：遍历并删除元素
来源：http://ncf.gogol.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mkc.gotoacloud.top

================================================================================
来源：http://eym.cucudq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cxt.yonumen.top

================================================================================
来源：http://wkc.ywan-chungtsiang.top

[T01] Kotlin：Hello World
来源：http://uwt.yonumen.top

println("Hello")
来源：http://zgl.sxryk.cn

[T02] Kotlin：变量
来源：http://kim.dianchejie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tpq.guannengcc.top

[T03] Kotlin：字符串模板
来源：http://ktn.vehdjk.com

"值: $b"
来源：http://dmh.nwbrower.top

[T04] Kotlin：空安全
来源：http://wpz.gaohongyu789.top

val n: String? = null;  n?.length
来源：http://pcu.zhaomingkeji.xyz

[T05] Kotlin：when 表达式
来源：http://kpj.chenlongwang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://abr.guannengcc.top

[T06] Kotlin：集合映射
来源：http://meo.smart0.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://gpr.xinyue.icu

[T07] Kotlin：集合过滤
来源：http://wcu.zdqjudy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xac.ctjpmb.com

[T08] Kotlin：数据类
来源：http://boz.ywan-chungtsiang.top

data class User(val name: String, val age: Int)
来源：http://pvl.shanyushiyangkeji.top

[T09] Kotlin：扩展函数
来源：http://tfm.guannengcc.top

fun String.exclaim() = this + "!"
来源：http://qms.xziqi.cn

[T10] Kotlin：默认参数
来源：http://jwf.aibaodan.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pxb.nwbrower.top

[T11] Kotlin：协程
来源：http://hja.ivvv.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://cyq.yonumen.top

[T12] Kotlin：解构声明
来源：http://hav.wangshuangyany.cn

val (a, b) = Pair(1, 2)
来源：http://kfm.feifeiyinyue.top

[T13] Kotlin：只读 Map
来源：http://vuh.gogol.net.cn

val m = mapOf("a" to 1)
来源：http://xxn.chenlongwang.top

[T14] Kotlin：循环
来源：http://ume.gaohongyu789.top

for (i in 1..10) println(i)
来源：http://jxc.kuanghao11.cn

[T15] Kotlin：接口
来源：http://zbd.tanke756.top

interface Shape { fun area(): Double }
来源：http://hgj.gzhubu.top

[T16] Swift：Hello World
来源：http://zzs.guannengcc.top

print("Hello")
来源：http://dli.jinqigufen.top

[T17] Swift：变量与常量
来源：http://zaf.havefunace.top

var a = 1;  let b = 2
来源：http://wkt.hcnkem.com

[T18] Swift：字符串插值
来源：http://jrd.gaohongyu789.top

"值: \(b)"
来源：http://csb.yanxiufei.cn

[T19] Swift：可选绑定
来源：http://shu.jiagoushi.top

if let n = opt { print(n) }
来源：http://xcp.tarul.cn

[T20] Swift：数组操作
来源：http://cmq.vqdsnc.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zke.ctjpmb.com

[T21] Swift：遍历
来源：http://tvf.tanke756.top

for x in a { print(x) }
来源：http://udk.wangshuangyany.cn

[T22] Swift：字典
来源：http://cqj.sjlbkw.cn

var d = ["a": 1];  d["b"] = 2
来源：http://amf.gotoacloud.top

[T23] Swift：函数
来源：http://icc.epnwcf.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://geh.nwbrower.top

[T24] Swift：闭包
来源：http://gse.hongshengwenyu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://jnx.ybcxt.top

[T25] Swift：结构体
来源：http://ark.smart0.xyz

struct P { var x: Int }
来源：http://mms.birdmap.top

[T26] Swift：类与重写
来源：http://ddc.jqgfzy.top

class A: Base { override func f() {} }
来源：http://ysp.cucudq.cn

[T27] Swift：错误处理
来源：http://las.ywan-chungtsiang.top

do { try f() } catch { print(error) }
来源：http://idg.zhijiandao.cn

[T28] Swift：枚举
来源：http://adq.birdmap.top

enum Color { case red, green }
来源：http://jom.shanyushiyangkeji.top

[T29] Swift：guard 提前返回
来源：http://mxe.zdqjudy.top

guard let x = opt else { return }
来源：http://iby.jinqigfzy.top

[T30] Swift：协议
来源：http://zmx.bbcook.cn

protocol Shape { func area() -> Double }
来源：http://nqj.mhx1999.top

[T31] Lua：Hello World
来源：http://wva.xuanzx.com

print("Hello")
来源：http://dvt.zhongyouzk.top

[T32] Lua：局部变量
来源：http://cxf.zycfv.cn

local a = 1
来源：http://aqc.yonumen.top

[T33] Lua：表（数组）
来源：http://vhq.hysaishi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yhd.shuidangran.top

[T34] Lua：遍历表
来源：http://jnp.9152youxi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://weu.nwbrower.top

[T35] Lua：字典表
来源：http://gxz.nanxinkj.top

local d = { a = 1 };  d.b = 2
来源：http://quh.jinyuanbaomall.cn

[T36] Lua：函数
来源：http://zhw.zycfv.cn

function add(a, b) return a + b end
来源：http://itg.hesvh.cn

[T37] Lua：字符串拼接
来源：http://fua.redwolf501.top

"a" .. "b"
来源：http://nen.sxryk.cn

[T38] Lua：条件
来源：http://kak.yj20258888.top

if x > 0 then print("正") end
来源：http://mwe.dianchejie.cn

[T39] Lua：模式匹配
来源：http://cxn.jqgfzy.top

string.find(s, "%d+")
来源：http://kze.meibo888.top

[T40] Lua：元表
来源：http://tkk.yongpay.top

setmetatable({}, { __index = base })
来源：http://ifx.yuxming.cn

[T41] Perl：Hello World
来源：http://nqz.hesvh.cn

print "Hello\n";
来源：http://xbv.tianlin.xyz

[T42] Perl：变量类型
来源：http://azo.yonumen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://skm.tanke756.top

[T43] Perl：字符串插值
来源：http://dag.aibaodan.cn

"值: $a"
来源：http://nsx.dashuyun.cn

[T44] Perl：条件
来源：http://ljc.pycfn.com

if ($a > 0) { print "正"; }
来源：http://ysy.ivvv.top

[T45] Perl：数组遍历
来源：http://mxg.chenjidiqi.icu

for my $x (@arr) { print $x; }
来源：http://mww.yuanzhike.top

[T46] Perl：哈希操作
来源：http://bhl.shangyingyoupin.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dxd.yj20258888.top

[T47] Perl：正则捕获
来源：http://esn.yongpay.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lrw.zhengqikj.top

[T48] Perl：正则替换
来源：http://wdn.yj20258888.top

$s =~ s/old/new/g;
来源：http://ywa.sysykeji.top

[T49] Perl：函数
来源：http://ilg.feifeiyinyue.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gpr.daria6918.cn

[T50] Perl：逐行读文件
来源：http://pxb.chenzaomai.com

open my $fh, "<", "a.txt" or die $!;
来源：http://wxp.aibaodan.cn

while (my $line = <$fh>) { print $line; }
来源：http://beq.kuanghao11.cn

[T51] Scala：Hello World
来源：http://cxd.jqgufenzy.top

println("Hello")
来源：http://crx.jqgufenzy.top

[T52] Scala：变量
来源：http://xob.zhixingplan.top

val a = 1;  var b = 2
来源：http://fup.hesvh.cn

[T53] Scala：字符串插值
来源：http://xfi.vehdjk.com

s"值: $b"
来源：http://mai.zhongyouzk.top

[T54] Scala：集合映射
来源：http://hks.ctjpmb.com

List(1, 2, 3).map(_ * 2)
来源：http://uyz.quarkkingdee.top

[T55] Scala：集合过滤
来源：http://rln.9152youxi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bqc.guowangkeji.top

[T56] Scala：样例类
来源：http://ajq.aizwys.cn

case class User(name: String, age: Int)
来源：http://fwc.nwbrower.top

[T57] Scala：模式匹配
来源：http://ftp.kuanghao11.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qig.fehbvm.com

[T58] Scala：函数定义
来源：http://djd.wangshuangyany.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bps.aibaodan.cn

[T59] Scala：循环
来源：http://box.c1oappe.top

for (i <- 1 to 10) println(i)
来源：http://qne.zhoulong.xyz

[T60] Scala：折叠
来源：http://fdn.hywenlv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ipl.yfazqb.com

================================================================================
来源：http://drh.ydjk.org.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yns.zhixingplan.top

================================================================================
来源：http://hcb.chenlongwang.top

[U01] Py：创建虚拟环境
来源：http://xuo.cashguo.top

python -m venv .venv && source .venv/bin/activate
来源：http://hnr.ybcxt.top

[U02] Py：导出 / 安装依赖
来源：http://zkh.yj20258.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hbm.gaohongyu789.top

[U03] Py：加载 .env 配置
来源：http://iai.jyoumei.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pzg.redwolf501.top

[U04] Py：变量调试打印
来源：http://kcm.bbcook.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://csg.cucudq.cn

[U05] Py：列表去重且保序
来源：http://shg.cdnleiting.top

list(dict.fromkeys(arr))
来源：http://wlu.hywenlv.cn

[U06] Py：合并两个字典
来源：http://neg.xuanzx.com

{**a, **b}
来源：http://eok.epnwcf.com

[U07] Py：反转字典键值
来源：http://uvm.ppjwa.cn

{v: k for k, v in d.items()}
来源：http://kge.ivvv.top

[U08] Py：展平二维列表
来源：http://kpz.svipenyu.cn

[y for x in nested for y in x]
来源：http://gnp.hcnkem.com

[U09] Py：字典取最大值的键
来源：http://oll.chenlongwang.top

max(d, key=d.get)
来源：http://jhw.pycfn.com

[U10] Py：按值排序字典
来源：http://ozw.xingfuxueyuan.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ces.gogol.net.cn

[U11] Py：生成器表达式
来源：http://hza.yj20258888.top

(x * 2 for x in arr)
来源：http://yop.haohaochexian.top

[U12] Py：取出现最多的 3 个元素
来源：http://css.feifeiyinyue.top

Counter(arr).most_common(3)
来源：http://lyo.hongshengwenyu.top

[U13] Py：固定长度队列
来源：http://rce.zhiwuduotai.top

deque(maxlen=10)
来源：http://xnh.shzxlz.cn

[U14] Py：分组收集到列表
来源：http://mxw.jinyuanbaomall.cn

defaultdict(list)
来源：http://eiz.fzhhl.top

[U15] Py：高精度计时
来源：http://yxi.guowangkeji.top

t = time.perf_counter()
来源：http://rtz.bbcook.cn

[U16] Py：命令行参数解析
来源：http://hoi.andypj.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ptr.shanyushiyangkeji.top

[U17] Py：初始化日志
来源：http://shb.gzhubu.top

logging.basicConfig(level=logging.INFO)
来源：http://wce.wangshuangyany.cn

[U18] Py：预编译正则
来源：http://hcg.jinyuanbaomall.cn

pat = re.compile(r"\d+")
来源：http://nyo.haohaochexian.top

[U19] Py：正则替换带回调
来源：http://qjq.xingfuxueyuan.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qsu.fktsv.cn

[U20] Py：缓存函数结果
来源：http://zae.smart0.xyz

@functools.lru_cache(maxsize=None)
来源：http://qee.redwolf501.top

[U21] Py：自定义上下文管理器
来源：http://oht.gotoacloud.top

@contextlib.contextmanager
来源：http://arm.jianghu66.top

[U22] Py：矩阵转置
来源：http://ggk.hesvh.cn

list(zip(*m))
来源：http://tht.chenjidiqi.icu

[U23] Py：分块读取大文件
来源：http://rwp.sysykeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://anv.meibo888.top

[U24] Py：路径操作
来源：http://nmh.smart0.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xws.jqgufenzy.top

[U25] Py：CSV 按字典读
来源：http://zrp.chenlongwang.top

csv.DictReader(f)
来源：http://yer.yueranfly.top

[U26] Py：并发下载
来源：http://kuj.havefunace.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rsv.zhoulong.xyz

[U27] Py：异步 HTTP
来源：http://bzw.yongpay.top

aiohttp.ClientSession() 配合 async with
来源：http://fcu.ydjk.org.cn

[U28] Py：类型别名
来源：http://ekl.iojbl.cn

UserId = int
来源：http://gtp.jianghu66.top

[U29] Py：属性校验
来源：http://xcu.yj202588.top

@property 与 @x.setter 配合
来源：http://etl.jqgufenzy.top

[U30] Py：数据类
来源：http://ulo.316326.xyz

@dataclass(slots=True)
来源：http://phs.aibaodan.cn

[U31] Py：单测
来源：http://mof.guowangkeji.top

python -m pytest -q
来源：http://nqi.iojbl.cn

[U32] Py：代码格式化
来源：http://mxl.9152youxi.cn

ruff format . && ruff check --fix .
来源：http://lsm.zhiwuduotai.top

[U33] Py：打包发布
来源：http://bce.zhengqikj.top

python -m build  （依赖 pyproject.toml）
来源：http://yth.guannengcc.top

[U34] Py：判断编码
来源：http://mya.hnxiangtu.top

chardet.detect(raw)
来源：http://kte.xuetiantiany.cn

[U35] Py：发送邮件
来源：http://psz.zhongyouzk.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ebg.nanxinkj.top

[U36] Py：定时任务
来源：http://rsr.cheryme.top

schedule.every(10).minutes.do(job)
来源：http://kme.hesvh.cn

[U37] Py：读写 Excel
来源：http://xul.zhixingplan.top

pandas.read_excel / DataFrame.to_excel
来源：http://mrk.jyoumei.cn

[U38] Py：获取脚本所在目录
来源：http://hrf.nwbrower.top

Path(__file__).resolve().parent
来源：http://gkh.andypj.xyz

[U39] Py：判断是否在交互环境
来源：http://qxd.iojbl.cn

sys.stdout.isatty()
来源：http://xkn.hammf.cn

[U40] Py：打印到标准错误
来源：http://sds.zhixingplan.top

print("err", file=sys.stderr)
来源：http://nsk.yangfankeji.com

[U41] PHP：初始化 Composer 项目
来源：http://cew.iojbl.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ypa.hysaishi.cn

[U42] PHP：PSR-4 自动加载
来源：http://igz.cdnleiting.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pui.fktsv.cn

[U43] PHP：声明命名空间
来源：http://sly.tarul.cn

namespace App\Http;
来源：http://zyh.meibo888.top

[U44] PHP：开启严格类型
来源：http://ebg.zhengqikj.top

declare(strict_types=1);
来源：http://ato.wangdashe.top

[U45] PHP：类型声明与返回类型
来源：http://oml.hcnkem.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://qib.fanxiaobao.xyz

[U46] PHP：可空类型
来源：http://mik.sjlbkw.cn

?string $name = null
来源：http://sqw.chenlongwang.top

[U47] PHP：联合类型
来源：http://vca.zdbjq.cn

int|string $id
来源：http://sny.yonumen.top

[U48] PHP：纯枚举
来源：http://tmx.tanke756.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rtj.hongshengwenyu.top

[U49] PHP：只读属性
来源：http://ybe.sxryk.cn

public readonly string $name
来源：http://bie.zhengqikj.top

[U50] PHP：构造器属性提升
来源：http://zrn.sufxvd.cn

public function __construct(private int $id) {}
来源：http://lda.cashguo.top

[U51] PHP：数组解构
来源：http://mue.quarkkingdee.top

[$a, $b] = $arr;
来源：http://hnr.uphjek.com

[U52] PHP：箭头函数
来源：http://gbe.guannengcc.top

$double = fn($x) => $x * 2;
来源：http://lau.uphjek.com

[U53] PHP：空合并运算符
来源：http://rng.hesvh.cn

$v = $a ?? $b ?? "default";
来源：http://ixl.birdmap.top

[U54] PHP：空安全调用
来源：http://eks.ydjk.org.cn

$obj?->method()
来源：http://rlp.xylfe.cn

[U55] PHP：match 表达式
来源：http://hax.hfpthk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://itf.yj20258.top

[U56] PHP：命名参数
来源：http://wjr.yongpay.top

f(a: 1, b: 2)
来源：http://dne.zhijiandao.cn

[U57] PHP：字符串插值
来源：http://gwz.fktsv.cn

"值: {$a}"
来源：http://yjq.shuidangran.top

[U58] PHP：数组三件套
来源：http://miw.jiagoushi.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xte.smart0.xyz

[U59] PHP：自定义排序
来源：http://mvx.feifeiyinyue.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zbc.zdqjudy.top

[U60] PHP：JSON 编解码
来源：http://gtw.quarkkingdee.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bkk.zhongyouzk.top

[U61] PHP：正则
来源：http://nsw.xylfe.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://alr.tarul.cn

[U62] PHP：日期对象
来源：http://rvo.sysykeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fyz.ybcxt.top

[U63] PHP：文件读写
来源：http://ygh.yj20258888.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kyg.yj20258888.top

[U64] PHP：目录遍历
来源：http://bjn.9152youxi.cn

glob("dir/*.php");  scandir("dir");
来源：http://ekx.jqgfzy.top


<!-- 参考信息 -->