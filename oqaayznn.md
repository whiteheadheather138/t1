代发 wailian999

[S39] C++：自定义比较器排序
来源：http://fma.fzhhl.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zlp.shuidangran.top

[S40] C++：查找元素
来源：http://ovk.shanyushiyangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tvl.tarul.cn

[S41] C++：类与构造函数
来源：http://qfr.guannengcc.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oob.fanxiaobao.xyz

[S42] C++：继承与虚函数
来源：http://uzi.hongshengwenyu.top

class B : public Base { public: void f() override {} };
来源：http://xtq.guowangkeji.top

[S43] C++：智能指针
来源：http://ukf.bjfxy.top

auto p = std::make_unique<int>(5);
来源：http://dfj.jlsjyb.cn

[S44] C++：引用传参
来源：http://lyx.yj20258888.top

void inc(int &x) { ++x; }
来源：http://oyu.jinqigfzy.top

[S45] C++：lambda
来源：http://qvd.c1oappe.top

auto add = [](int a, int b) { return a + b; };
来源：http://lil.sweek.top

[S46] C++：函数模板
来源：http://jha.sufxvd.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rzu.hfpthk.cn

[S47] C++：结构化绑定遍历
来源：http://ahz.yj20258.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qoc.xylfe.cn

[S48] C++：逐行读文件
来源：http://ujs.hywenlv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zjm.tianlin.xyz

while (std::getline(in, line)) { }
来源：http://gxd.kuanghao11.cn

[S49] C++：写文件
来源：http://sbj.pengpengdd.cyou

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eyv.dashuyun.cn

[S50] C++：格式化数字
来源：http://tfm.wangshuangyany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nmq.jinyuanbaomall.cn

[S51] C++：显式类型转换
来源：http://wkw.uphjek.com

static_cast<double>(a) / b
来源：http://rvt.tanke756.top

[S52] C++：const 与 noexcept
来源：http://ven.meibo888.top

int size() const noexcept { return n_; }
来源：http://tmb.jyoumei.cn

[S53] C++：移动语义
来源：http://nql.316326.xyz

std::vector<int> w = std::move(v);
来源：http://ies.shuidangran.top

[S54] C++：异常处理
来源：http://lsd.zhiwuduotai.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lcy.ehwqpu.com

[S55] C++：结构化绑定
来源：http://zmq.hongshengwenyu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://klz.gzhubu.top

[S56] C++：optional
来源：http://qwk.yuxming.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://enm.daxiang520.top

[S57] C++：编译期常量
来源：http://wbi.iojbl.cn

constexpr int N = 10;
来源：http://fpd.vqdsnc.cn

[S58] C++：命名空间
来源：http://nek.sweek.top

namespace ns { int f() { return 1; } }
来源：http://eyd.chenlongwang.top

[S59] C++：静态断言
来源：http://pxy.daria6918.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://grv.hfpthk.cn

[S60] C++：遍历并删除元素
来源：http://urz.jinyuanbaomall.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ozs.haohaochexian.top

================================================================================
来源：http://psh.vehdjk.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uar.redwolf501.top

================================================================================
来源：http://fkt.52xcode.cn

[T01] Kotlin：Hello World
来源：http://roa.hammf.cn

println("Hello")
来源：http://ysx.yongpay.top

[T02] Kotlin：变量
来源：http://spz.chenjidiqi.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ykh.jianghu66.top

[T03] Kotlin：字符串模板
来源：http://pnj.tianlin.xyz

"值: $b"
来源：http://jyu.yfazqb.com

[T04] Kotlin：空安全
来源：http://eog.jinghuilouyu.cn

val n: String? = null;  n?.length
来源：http://sxy.zdqjudy.top

[T05] Kotlin：when 表达式
来源：http://udq.svipenyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aki.zhoulong.xyz

[T06] Kotlin：集合映射
来源：http://swn.cucudq.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qft.shanyushiyangkeji.top

[T07] Kotlin：集合过滤
来源：http://eov.52xcode.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wzp.yj20258888.top

[T08] Kotlin：数据类
来源：http://efm.fehbvm.com

data class User(val name: String, val age: Int)
来源：http://wyu.0kj1m.cn

[T09] Kotlin：扩展函数
来源：http://inm.yj20258888.top

fun String.exclaim() = this + "!"
来源：http://fhe.gotoacloud.top

[T10] Kotlin：默认参数
来源：http://ohx.gotoacloud.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ety.0kj1m.cn

[T11] Kotlin：协程
来源：http://sti.guowangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://afe.xuetiantiany.cn

[T12] Kotlin：解构声明
来源：http://kaa.hnqzz.top

val (a, b) = Pair(1, 2)
来源：http://qrr.pycfn.com

[T13] Kotlin：只读 Map
来源：http://muq.yueranfly.top

val m = mapOf("a" to 1)
来源：http://qre.zdqjudy.top

[T14] Kotlin：循环
来源：http://jsk.chenjidiqi.icu

for (i in 1..10) println(i)
来源：http://hec.316326.xyz

[T15] Kotlin：接口
来源：http://grs.0kj1m.cn

interface Shape { fun area(): Double }
来源：http://ayw.xinyue.icu

[T16] Swift：Hello World
来源：http://ioq.tarul.cn

print("Hello")
来源：http://acl.hongshengwenyu.top

[T17] Swift：变量与常量
来源：http://gnm.yj20258.top

var a = 1;  let b = 2
来源：http://ckn.sxryk.cn

[T18] Swift：字符串插值
来源：http://atu.hnqzz.top

"值: \(b)"
来源：http://dwu.tanke756.top

[T19] Swift：可选绑定
来源：http://rjq.shanyushiyangtech.top

if let n = opt { print(n) }
来源：http://tox.gaohongyu789.top

[T20] Swift：数组操作
来源：http://swr.sufxvd.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kvf.jqgfzy.top

[T21] Swift：遍历
来源：http://ynr.uphjek.com

for x in a { print(x) }
来源：http://gpm.ivvv.top

[T22] Swift：字典
来源：http://eem.aizwys.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fci.jqgfzy.top

[T23] Swift：函数
来源：http://efe.yanxiufei.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dby.jqgufenzy.top

[T24] Swift：闭包
来源：http://ebc.jinqigufen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://qhg.zhixingplan.top

[T25] Swift：结构体
来源：http://htw.bbcook.cn

struct P { var x: Int }
来源：http://gyy.fehbvm.com

[T26] Swift：类与重写
来源：http://nkc.zhengqikj.top

class A: Base { override func f() {} }
来源：http://yff.gotoacloud.top

[T27] Swift：错误处理
来源：http://bne.ctjpmb.com

do { try f() } catch { print(error) }
来源：http://gxn.jqgufenzy.top

[T28] Swift：枚举
来源：http://txs.aibaodan.cn

enum Color { case red, green }
来源：http://fqk.c1oappe.top

[T29] Swift：guard 提前返回
来源：http://trm.shanyushiyangtech.top

guard let x = opt else { return }
来源：http://brg.jinyuanbaomall.cn

[T30] Swift：协议
来源：http://cvw.guannengcc.top

protocol Shape { func area() -> Double }
来源：http://jup.hcnkem.com

[T31] Lua：Hello World
来源：http://xey.daxiang520.top

print("Hello")
来源：http://xae.fengsongda.top

[T32] Lua：局部变量
来源：http://xvk.yj202588.top

local a = 1
来源：http://rzi.ybcxt.top

[T33] Lua：表（数组）
来源：http://lfz.jinyuanbaomall.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jhc.c1oappe.top

[T34] Lua：遍历表
来源：http://dqp.yuxming.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pgf.sufxvd.cn

[T35] Lua：字典表
来源：http://dpf.chenjidiqi.icu

local d = { a = 1 };  d.b = 2
来源：http://zyf.fehbvm.com

[T36] Lua：函数
来源：http://kzy.yfazqb.com

function add(a, b) return a + b end
来源：http://gbt.quarkkingdee.top

[T37] Lua：字符串拼接
来源：http://xmc.zhoulong.xyz

"a" .. "b"
来源：http://tel.gotoacloud.top

[T38] Lua：条件
来源：http://wgq.jinghuilouyu.cn

if x > 0 then print("正") end
来源：http://dkw.mhx1999.top

[T39] Lua：模式匹配
来源：http://wuo.fengsongda.top

string.find(s, "%d+")
来源：http://xyx.jqgufenzy.top

[T40] Lua：元表
来源：http://vgn.guowangkeji.top

setmetatable({}, { __index = base })
来源：http://ijy.ywan-chungtsiang.top

[T41] Perl：Hello World
来源：http://wvj.ywan-chungtsiang.top

print "Hello\n";
来源：http://fme.dashuyun.cn

[T42] Perl：变量类型
来源：http://mgw.havefunace.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mqq.zhoulong.xyz

[T43] Perl：字符串插值
来源：http://wzd.jiagoushi.top

"值: $a"
来源：http://avf.yvedp.cn

[T44] Perl：条件
来源：http://saa.zhixingplan.top

if ($a > 0) { print "正"; }
来源：http://czf.ybcxt.top

[T45] Perl：数组遍历
来源：http://tfn.xingfuxueyuan.xyz

for my $x (@arr) { print $x; }
来源：http://qiw.zhengqikj.top

[T46] Perl：哈希操作
来源：http://ivy.xziqi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xws.fzhhl.top

[T47] Perl：正则捕获
来源：http://ues.sufxvd.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nkc.fengsongda.top

[T48] Perl：正则替换
来源：http://npj.smart0.xyz

$s =~ s/old/new/g;
来源：http://inu.hcnkem.com

[T49] Perl：函数
来源：http://sor.yfazqb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pdp.fzhhl.top

[T50] Perl：逐行读文件
来源：http://ljt.yj20258.top

open my $fh, "<", "a.txt" or die $!;
来源：http://oys.epnwcf.com

while (my $line = <$fh>) { print $line; }
来源：http://frr.ppjwa.cn

[T51] Scala：Hello World
来源：http://wws.dashuyun.cn

println("Hello")
来源：http://ans.snrcjt.cn

[T52] Scala：变量
来源：http://dsv.ppjwa.cn

val a = 1;  var b = 2
来源：http://rxe.kuanghao11.cn

[T53] Scala：字符串插值
来源：http://hry.tian-w.cn

s"值: $b"
来源：http://snm.nwbrower.top

[T54] Scala：集合映射
来源：http://ksc.zycfv.cn

List(1, 2, 3).map(_ * 2)
来源：http://uyk.zhaomingkeji.xyz

[T55] Scala：集合过滤
来源：http://cdv.bbcook.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rcg.zhiwuduotai.top

[T56] Scala：样例类
来源：http://kcq.hywenlv.cn

case class User(name: String, age: Int)
来源：http://axe.smart0.xyz

[T57] Scala：模式匹配
来源：http://ovj.bjfxy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://riy.fzhhl.top

[T58] Scala：函数定义
来源：http://vde.ctjpmb.com

def add(a: Int, b: Int): Int = a + b
来源：http://xzo.ppjwa.cn

[T59] Scala：循环
来源：http://gmc.xingfuxueyuan.xyz

for (i <- 1 to 10) println(i)
来源：http://xnn.yanxiufei.cn

[T60] Scala：折叠
来源：http://byj.ehwqpu.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fdi.andypj.xyz

================================================================================
来源：http://wey.jiagoushi.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hgl.yonumen.top

================================================================================
来源：http://twb.yj20258888.top

[U01] Py：创建虚拟环境
来源：http://zjh.chenjidiqi.icu

python -m venv .venv && source .venv/bin/activate
来源：http://mux.sweek.top

[U02] Py：导出 / 安装依赖
来源：http://vvx.uphjek.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zqp.zhengqikj.top

[U03] Py：加载 .env 配置
来源：http://mup.yueranfly.top

from dotenv import load_dotenv; load_dotenv()
来源：http://rxa.jlsjyb.cn

[U04] Py：变量调试打印
来源：http://yer.zhongyouzk.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sgd.fktsv.cn

[U05] Py：列表去重且保序
来源：http://fxa.bjfxy.top

list(dict.fromkeys(arr))
来源：http://pso.cheryme.top

[U06] Py：合并两个字典
来源：http://wyk.chenjidiqi.icu

{**a, **b}
来源：http://eik.hongshengwenyu.top

[U07] Py：反转字典键值
来源：http://ksr.pengpengdd.cyou

{v: k for k, v in d.items()}
来源：http://ovb.wangshuangyany.cn

[U08] Py：展平二维列表
来源：http://eph.zhoulong.xyz

[y for x in nested for y in x]
来源：http://pjj.tarul.cn

[U09] Py：字典取最大值的键
来源：http://dpv.smart0.xyz

max(d, key=d.get)
来源：http://ujh.haohaochexian.top

[U10] Py：按值排序字典
来源：http://byt.hesvh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://npx.52xcode.cn

[U11] Py：生成器表达式
来源：http://rpk.zdbjq.cn

(x * 2 for x in arr)
来源：http://ldm.jinghuilouyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://llq.smart0.xyz

Counter(arr).most_common(3)
来源：http://srv.ctjpmb.com

[U13] Py：固定长度队列
来源：http://hjy.cashguo.top

deque(maxlen=10)
来源：http://ykn.shzxlz.cn

[U14] Py：分组收集到列表
来源：http://ijw.xylfe.cn

defaultdict(list)
来源：http://jdb.hnqzz.top

[U15] Py：高精度计时
来源：http://uow.aibaodan.cn

t = time.perf_counter()
来源：http://qxk.guowangkeji.top

[U16] Py：命令行参数解析
来源：http://clr.hysaishi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pdl.jinyuanbaomall.cn

[U17] Py：初始化日志
来源：http://fva.yongpay.top

logging.basicConfig(level=logging.INFO)
来源：http://meg.shzxlz.cn

[U18] Py：预编译正则
来源：http://nlv.yongpay.top

pat = re.compile(r"\d+")
来源：http://nna.zdbjq.cn

[U19] Py：正则替换带回调
来源：http://wxp.xuetiantiany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dba.dianchejie.cn

[U20] Py：缓存函数结果
来源：http://kcl.tanke756.top

@functools.lru_cache(maxsize=None)
来源：http://hhy.jinyuanbaomall.cn

[U21] Py：自定义上下文管理器
来源：http://hhh.ydzc1.top

@contextlib.contextmanager
来源：http://uwi.hfpthk.cn

[U22] Py：矩阵转置
来源：http://peg.yfazqb.com

list(zip(*m))
来源：http://nrd.ppjwa.cn

[U23] Py：分块读取大文件
来源：http://phe.gogol.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uhf.jinqigufen.top

[U24] Py：路径操作
来源：http://cux.svipenyu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sts.shangyingyoupin.top

[U25] Py：CSV 按字典读
来源：http://qne.jinqigfzy.top

csv.DictReader(f)
来源：http://yef.gzhubu.top

[U26] Py：并发下载
来源：http://yop.epnwcf.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hcz.yongpay.top

[U27] Py：异步 HTTP
来源：http://dmf.ydjk.org.cn

aiohttp.ClientSession() 配合 async with
来源：http://lmy.sufxvd.cn

[U28] Py：类型别名
来源：http://sgg.ctjpmb.com

UserId = int
来源：http://nvl.ywan-chungtsiang.top

[U29] Py：属性校验
来源：http://ipq.xinyue.icu

@property 与 @x.setter 配合
来源：http://zan.jinqigfzy.top

[U30] Py：数据类
来源：http://jru.guannengcc.top

@dataclass(slots=True)
来源：http://ezs.ybcxt.top

[U31] Py：单测
来源：http://lpx.cqqwz.cn

python -m pytest -q
来源：http://fbe.vehdjk.com

[U32] Py：代码格式化
来源：http://uvl.fehbvm.com

ruff format . && ruff check --fix .
来源：http://yvj.tian-w.cn

[U33] Py：打包发布
来源：http://sxk.9152youxi.cn

python -m build  （依赖 pyproject.toml）
来源：http://xqz.zhixingplan.top

[U34] Py：判断编码
来源：http://lnt.aibaodan.cn

chardet.detect(raw)
来源：http://unt.shangyingyoupin.top

[U35] Py：发送邮件
来源：http://pqj.hywenlv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wfr.haohaochexian.top

[U36] Py：定时任务
来源：http://hih.shanyushiyangkeji.top

schedule.every(10).minutes.do(job)
来源：http://dob.yanxiufei.cn

[U37] Py：读写 Excel
来源：http://uml.pengpengdd.cyou

pandas.read_excel / DataFrame.to_excel
来源：http://svq.yj20258888.top

[U38] Py：获取脚本所在目录
来源：http://adx.iojbl.cn

Path(__file__).resolve().parent
来源：http://qtj.yj20258888.top

[U39] Py：判断是否在交互环境
来源：http://gwa.xuanzx.com

sys.stdout.isatty()
来源：http://snf.zhixingplan.top

[U40] Py：打印到标准错误
来源：http://tlc.hammf.cn

print("err", file=sys.stderr)
来源：http://bvx.xuetiantiany.cn

[U41] PHP：初始化 Composer 项目
来源：http://ubu.pycfn.com

composer init;  composer require guzzlehttp/guzzle
来源：http://nri.yonumen.top

[U42] PHP：PSR-4 自动加载
来源：http://bfo.guowangkeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bck.nanxuanxn.top

[U43] PHP：声明命名空间
来源：http://bzi.yvedp.cn

namespace App\Http;
来源：http://saj.meibo888.top

[U44] PHP：开启严格类型
来源：http://gma.jyoumei.cn

declare(strict_types=1);
来源：http://rgm.yueranfly.top

[U45] PHP：类型声明与返回类型
来源：http://rtv.cheryme.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ord.hesvh.cn

[U46] PHP：可空类型
来源：http://jft.fengsongda.top

?string $name = null
来源：http://qpw.yuxming.cn

[U47] PHP：联合类型
来源：http://cpe.zhengqikj.top

int|string $id
来源：http://eeu.jqgufenzy.top

[U48] PHP：纯枚举
来源：http://aer.yonumen.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://czo.vehdjk.com

[U49] PHP：只读属性
来源：http://rau.yongpay.top

public readonly string $name
来源：http://qup.pengpengdd.cyou

[U50] PHP：构造器属性提升
来源：http://uys.sweek.top

public function __construct(private int $id) {}
来源：http://ayk.havefunace.top

[U51] PHP：数组解构
来源：http://ucs.zycfv.cn

[$a, $b] = $arr;
来源：http://slk.jinqigufen.top

[U52] PHP：箭头函数
来源：http://xzd.smart0.xyz

$double = fn($x) => $x * 2;
来源：http://vbt.hcnkem.com

[U53] PHP：空合并运算符
来源：http://bnh.hnqzz.top

$v = $a ?? $b ?? "default";
来源：http://gms.xingfuxueyuan.xyz

[U54] PHP：空安全调用
来源：http://iay.iojbl.cn

$obj?->method()
来源：http://shq.jiagoushi.top

[U55] PHP：match 表达式
来源：http://spw.fehbvm.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vqm.tianlin.xyz

[U56] PHP：命名参数
来源：http://sht.ywan-chungtsiang.top

f(a: 1, b: 2)
来源：http://uuv.ppjwa.cn

[U57] PHP：字符串插值
来源：http://gcf.yj20258888.top

"值: {$a}"
来源：http://efe.cashguo.top

[U58] PHP：数组三件套
来源：http://hrs.pycfn.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uro.jyoumei.cn

[U59] PHP：自定义排序
来源：http://ihe.hcnkem.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kin.shanyushiyangtech.top

[U60] PHP：JSON 编解码
来源：http://mgu.ybcxt.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ssk.hcnkem.com

[U61] PHP：正则
来源：http://ysw.cheryme.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qek.chenzaomai.com

[U62] PHP：日期对象
来源：http://qeh.shanyushiyangtech.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ttz.yfazqb.com

[U63] PHP：文件读写
来源：http://kqt.yvedp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mxz.hongshengwenyu.top

[U64] PHP：目录遍历
来源：http://qit.guannengcc.top

glob("dir/*.php");  scandir("dir");
来源：http://hrd.tarul.cn


<!-- 参考信息 -->