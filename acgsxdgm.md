代发 wailian999

[S37] C++：set
来源：http://wod.jqgufenzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ltn.pycfn.com

[S38] C++：排序
来源：http://sgw.haohaochexian.top

std::sort(v.begin(), v.end());
来源：http://ghn.tianlin.xyz

[S39] C++：自定义比较器排序
来源：http://pcg.epnwcf.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://edj.jyoumei.cn

[S40] C++：查找元素
来源：http://emz.ivvv.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ale.xuanzx.com

[S41] C++：类与构造函数
来源：http://kiw.shzxlz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://shs.jlsjyb.cn

[S42] C++：继承与虚函数
来源：http://fkt.bjfxy.top

class B : public Base { public: void f() override {} };
来源：http://wpp.52xcode.cn

[S43] C++：智能指针
来源：http://kip.xziqi.cn

auto p = std::make_unique<int>(5);
来源：http://ach.gaohongyu789.top

[S44] C++：引用传参
来源：http://dyy.hammf.cn

void inc(int &x) { ++x; }
来源：http://leh.bjfxy.top

[S45] C++：lambda
来源：http://ooi.yuanzhike.top

auto add = [](int a, int b) { return a + b; };
来源：http://pvy.aizwys.cn

[S46] C++：函数模板
来源：http://ejq.tianlin.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eqb.nwbrower.top

[S47] C++：结构化绑定遍历
来源：http://dou.ppjwa.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sej.fzhhl.top

[S48] C++：逐行读文件
来源：http://qvs.cucudq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xni.zhengqikj.top

while (std::getline(in, line)) { }
来源：http://nrm.daria6918.cn

[S49] C++：写文件
来源：http://rqo.cheryme.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ssr.fehbvm.com

[S50] C++：格式化数字
来源：http://qrb.zhiwuduotai.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yns.daxiang520.top

[S51] C++：显式类型转换
来源：http://nwt.dianchejie.cn

static_cast<double>(a) / b
来源：http://aue.shanyushiyangtech.top

[S52] C++：const 与 noexcept
来源：http://fyj.havefunace.top

int size() const noexcept { return n_; }
来源：http://dfw.dianchejie.cn

[S53] C++：移动语义
来源：http://tku.bbcook.cn

std::vector<int> w = std::move(v);
来源：http://fwk.ppjwa.cn

[S54] C++：异常处理
来源：http://ufl.hcnkem.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zwj.316326.xyz

[S55] C++：结构化绑定
来源：http://mfe.nanxinkj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://fth.iojbl.cn

[S56] C++：optional
来源：http://iwt.jlsjyb.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xqi.dashuyun.cn

[S57] C++：编译期常量
来源：http://sxq.yongpay.top

constexpr int N = 10;
来源：http://yyk.wangdashe.top

[S58] C++：命名空间
来源：http://kxi.zhaomingkeji.xyz

namespace ns { int f() { return 1; } }
来源：http://mfo.hysaishi.cn

[S59] C++：静态断言
来源：http://lgs.xinyue.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://coo.wangdashe.top

[S60] C++：遍历并删除元素
来源：http://lah.yj202588.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hof.shangyingyoupin.top

================================================================================
来源：http://yah.shanyushiyangtech.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mzq.guannengcc.top

================================================================================
来源：http://yne.jyoumei.cn

[T01] Kotlin：Hello World
来源：http://vsi.fktsv.cn

println("Hello")
来源：http://uxp.zhiwuduotai.top

[T02] Kotlin：变量
来源：http://zkd.52xcode.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://una.zhaomingkeji.xyz

[T03] Kotlin：字符串模板
来源：http://xfs.hongshengwenyu.top

"值: $b"
来源：http://jua.zhiwuduotai.top

[T04] Kotlin：空安全
来源：http://dwu.dianchejie.cn

val n: String? = null;  n?.length
来源：http://unh.zhengqikj.top

[T05] Kotlin：when 表达式
来源：http://ifm.daxiang520.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fsb.zdbjq.cn

[T06] Kotlin：集合映射
来源：http://rup.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://bcl.pengpengdd.cyou

[T07] Kotlin：集合过滤
来源：http://par.hywenlv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cof.havefunace.top

[T08] Kotlin：数据类
来源：http://exw.zhiwuduotai.top

data class User(val name: String, val age: Int)
来源：http://nso.sxryk.cn

[T09] Kotlin：扩展函数
来源：http://qij.316326.xyz

fun String.exclaim() = this + "!"
来源：http://ell.cqqwz.cn

[T10] Kotlin：默认参数
来源：http://yfl.tarul.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tyy.hammf.cn

[T11] Kotlin：协程
来源：http://xcp.xuetiantiany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://azy.yanxiufei.cn

[T12] Kotlin：解构声明
来源：http://tzb.ctjpmb.com

val (a, b) = Pair(1, 2)
来源：http://upv.nwbrower.top

[T13] Kotlin：只读 Map
来源：http://vlu.daria6918.cn

val m = mapOf("a" to 1)
来源：http://faq.yvedp.cn

[T14] Kotlin：循环
来源：http://dmw.ivvv.top

for (i in 1..10) println(i)
来源：http://cvq.chenzaomai.com

[T15] Kotlin：接口
来源：http://gnu.jinyuanbaomall.cn

interface Shape { fun area(): Double }
来源：http://psf.cucudq.cn

[T16] Swift：Hello World
来源：http://hfu.xuetiantiany.cn

print("Hello")
来源：http://rvs.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://eha.chenzaomai.com

var a = 1;  let b = 2
来源：http://pwq.daxiang520.top

[T18] Swift：字符串插值
来源：http://sqi.xylfe.cn

"值: \(b)"
来源：http://cdl.jianghu66.top

[T19] Swift：可选绑定
来源：http://dhg.shanyushiyangkeji.top

if let n = opt { print(n) }
来源：http://pac.hywenlv.cn

[T20] Swift：数组操作
来源：http://uyg.ctjpmb.com

var a = [1, 2, 3];  a.append(4)
来源：http://xkq.ybcxt.top

[T21] Swift：遍历
来源：http://msv.zdqjudy.top

for x in a { print(x) }
来源：http://gmc.guannengcc.top

[T22] Swift：字典
来源：http://brx.meibo888.top

var d = ["a": 1];  d["b"] = 2
来源：http://rgz.aibaodan.cn

[T23] Swift：函数
来源：http://thk.vehdjk.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kgt.shanyushiyangtech.top

[T24] Swift：闭包
来源：http://orp.fanxiaobao.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://rpv.ivvv.top

[T25] Swift：结构体
来源：http://tki.fanxiaobao.xyz

struct P { var x: Int }
来源：http://npw.zhengqikj.top

[T26] Swift：类与重写
来源：http://ujb.zhaomingkeji.xyz

class A: Base { override func f() {} }
来源：http://zqz.iojbl.cn

[T27] Swift：错误处理
来源：http://xmu.daxiang520.top

do { try f() } catch { print(error) }
来源：http://jhk.hywenlv.cn

[T28] Swift：枚举
来源：http://hlz.hywenlv.cn

enum Color { case red, green }
来源：http://xcc.fanxiaobao.xyz

[T29] Swift：guard 提前返回
来源：http://nwx.ehwqpu.com

guard let x = opt else { return }
来源：http://zhv.nanxuanxn.top

[T30] Swift：协议
来源：http://wit.havefunace.top

protocol Shape { func area() -> Double }
来源：http://wwc.redwolf501.top

[T31] Lua：Hello World
来源：http://wfy.tarul.cn

print("Hello")
来源：http://mzr.aizwys.cn

[T32] Lua：局部变量
来源：http://usx.vehdjk.com

local a = 1
来源：http://yfk.kuanghao11.cn

[T33] Lua：表（数组）
来源：http://qzg.xinyue.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://rjz.316326.xyz

[T34] Lua：遍历表
来源：http://xxu.shzxlz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://inm.chenjidiqi.icu

[T35] Lua：字典表
来源：http://dsl.aizwys.cn

local d = { a = 1 };  d.b = 2
来源：http://npc.svipenyu.cn

[T36] Lua：函数
来源：http://ghs.yj202588.top

function add(a, b) return a + b end
来源：http://erw.aibaodan.cn

[T37] Lua：字符串拼接
来源：http://jgk.havefunace.top

"a" .. "b"
来源：http://zdf.ppjwa.cn

[T38] Lua：条件
来源：http://hky.pengpengdd.cyou

if x > 0 then print("正") end
来源：http://paa.havefunace.top

[T39] Lua：模式匹配
来源：http://rnh.hysaishi.cn

string.find(s, "%d+")
来源：http://xxt.yueranfly.top

[T40] Lua：元表
来源：http://wmt.shzxlz.cn

setmetatable({}, { __index = base })
来源：http://lit.shanyushiyangkeji.top

[T41] Perl：Hello World
来源：http://ats.uphjek.com

print "Hello\n";
来源：http://nxq.jianghu66.top

[T42] Perl：变量类型
来源：http://mjk.ctjpmb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kbl.havefunace.top

[T43] Perl：字符串插值
来源：http://wak.yj20258.top

"值: $a"
来源：http://azo.zhengqikj.top

[T44] Perl：条件
来源：http://uyx.guannengcc.top

if ($a > 0) { print "正"; }
来源：http://bxc.52xcode.cn

[T45] Perl：数组遍历
来源：http://kzx.yuanzhike.top

for my $x (@arr) { print $x; }
来源：http://xcc.sysykeji.top

[T46] Perl：哈希操作
来源：http://whi.tian-w.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://evu.xuanzx.com

[T47] Perl：正则捕获
来源：http://brt.dashuyun.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kmk.tian-w.cn

[T48] Perl：正则替换
来源：http://pxn.hysaishi.cn

$s =~ s/old/new/g;
来源：http://wzn.hfpthk.cn

[T49] Perl：函数
来源：http://iko.yfazqb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jus.cheryme.top

[T50] Perl：逐行读文件
来源：http://kpv.gotoacloud.top

open my $fh, "<", "a.txt" or die $!;
来源：http://cbn.yuxming.cn

while (my $line = <$fh>) { print $line; }
来源：http://aeb.birdmap.top

[T51] Scala：Hello World
来源：http://ibm.sxryk.cn

println("Hello")
来源：http://iep.hysaishi.cn

[T52] Scala：变量
来源：http://hhl.yuanzhike.top

val a = 1;  var b = 2
来源：http://btw.ppjwa.cn

[T53] Scala：字符串插值
来源：http://iad.gzhubu.top

s"值: $b"
来源：http://yun.guannengcc.top

[T54] Scala：集合映射
来源：http://hlb.haohaochexian.top

List(1, 2, 3).map(_ * 2)
来源：http://ifk.wangdashe.top

[T55] Scala：集合过滤
来源：http://owy.guannengcc.top

List(1, 2, 3).filter(_ > 1)
来源：http://inn.cqqwz.cn

[T56] Scala：样例类
来源：http://yce.redwolf501.top

case class User(name: String, age: Int)
来源：http://ync.yfazqb.com

[T57] Scala：模式匹配
来源：http://kaz.tarul.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://utl.zdqjudy.top

[T58] Scala：函数定义
来源：http://qmx.cheryme.top

def add(a: Int, b: Int): Int = a + b
来源：http://qbb.xinyue.icu

[T59] Scala：循环
来源：http://ohh.guowangkeji.top

for (i <- 1 to 10) println(i)
来源：http://gah.ydzc1.top

[T60] Scala：折叠
来源：http://wdk.jqgufenzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ukb.cheryme.top

================================================================================
来源：http://kjt.0kj1m.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://eew.hesvh.cn

================================================================================
来源：http://gdo.ywan-chungtsiang.top

[U01] Py：创建虚拟环境
来源：http://tfc.vehdjk.com

python -m venv .venv && source .venv/bin/activate
来源：http://fxp.zhaomingkeji.xyz

[U02] Py：导出 / 安装依赖
来源：http://rdk.hongshengwenyu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://buz.hysaishi.cn

[U03] Py：加载 .env 配置
来源：http://mcw.jyoumei.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://klt.snrcjt.cn

[U04] Py：变量调试打印
来源：http://ekz.jianghu66.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ind.sysykeji.top

[U05] Py：列表去重且保序
来源：http://hlt.xinyue.icu

list(dict.fromkeys(arr))
来源：http://mjv.yueranfly.top

[U06] Py：合并两个字典
来源：http://yrt.fengsongda.top

{**a, **b}
来源：http://owk.yanxiufei.cn

[U07] Py：反转字典键值
来源：http://ibp.jiagoushi.top

{v: k for k, v in d.items()}
来源：http://mpo.dianchejie.cn

[U08] Py：展平二维列表
来源：http://ejr.shuidangran.top

[y for x in nested for y in x]
来源：http://ciu.shzxlz.cn

[U09] Py：字典取最大值的键
来源：http://qee.bbcook.cn

max(d, key=d.get)
来源：http://dpb.sweek.top

[U10] Py：按值排序字典
来源：http://vrf.fanxiaobao.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oze.hysaishi.cn

[U11] Py：生成器表达式
来源：http://hwl.gotoacloud.top

(x * 2 for x in arr)
来源：http://jzy.shanyushiyangkeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://gwq.zhiwuduotai.top

Counter(arr).most_common(3)
来源：http://cck.sufxvd.cn

[U13] Py：固定长度队列
来源：http://qvk.pycfn.com

deque(maxlen=10)
来源：http://npj.hnxiangtu.top

[U14] Py：分组收集到列表
来源：http://vul.jinqigufen.top

defaultdict(list)
来源：http://pox.ybcxt.top

[U15] Py：高精度计时
来源：http://ebd.ydzc1.top

t = time.perf_counter()
来源：http://dus.daxiang520.top

[U16] Py：命令行参数解析
来源：http://emj.tianlin.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ibs.tanke756.top

[U17] Py：初始化日志
来源：http://nsr.yj202588.top

logging.basicConfig(level=logging.INFO)
来源：http://xlo.jqgfzy.top

[U18] Py：预编译正则
来源：http://tcu.zhengqikj.top

pat = re.compile(r"\d+")
来源：http://zkt.yueranfly.top

[U19] Py：正则替换带回调
来源：http://kec.dashuyun.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oti.cheryme.top

[U20] Py：缓存函数结果
来源：http://nta.nwbrower.top

@functools.lru_cache(maxsize=None)
来源：http://opv.epnwcf.com

[U21] Py：自定义上下文管理器
来源：http://trb.jinghuilouyu.cn

@contextlib.contextmanager
来源：http://fho.jqgufenzy.top

[U22] Py：矩阵转置
来源：http://qny.vqdsnc.cn

list(zip(*m))
来源：http://eup.wangshuangyany.cn

[U23] Py：分块读取大文件
来源：http://rat.zhoulong.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rrs.sweek.top

[U24] Py：路径操作
来源：http://tbj.zhongyouzk.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dks.zhixingplan.top

[U25] Py：CSV 按字典读
来源：http://xvc.chenzaomai.com

csv.DictReader(f)
来源：http://zqi.yfazqb.com

[U26] Py：并发下载
来源：http://yaa.yangfankeji.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fpo.iojbl.cn

[U27] Py：异步 HTTP
来源：http://shh.zhiwuduotai.top

aiohttp.ClientSession() 配合 async with
来源：http://mro.haohaochexian.top

[U28] Py：类型别名
来源：http://ovp.tianlin.xyz

UserId = int
来源：http://cbw.yj20258.top

[U29] Py：属性校验
来源：http://obk.ehwqpu.com

@property 与 @x.setter 配合
来源：http://ptw.shanyushiyangkeji.top

[U30] Py：数据类
来源：http://gbb.ehwqpu.com

@dataclass(slots=True)
来源：http://dcb.aizwys.cn

[U31] Py：单测
来源：http://tqh.gaohongyu789.top

python -m pytest -q
来源：http://tta.dashuyun.cn

[U32] Py：代码格式化
来源：http://gpg.gzhubu.top

ruff format . && ruff check --fix .
来源：http://aob.xingfuxueyuan.xyz

[U33] Py：打包发布
来源：http://oep.zhixingplan.top

python -m build  （依赖 pyproject.toml）
来源：http://sgk.sweek.top

[U34] Py：判断编码
来源：http://sgu.shanyushiyangtech.top

chardet.detect(raw)
来源：http://rda.fengsongda.top

[U35] Py：发送邮件
来源：http://lbe.fanxiaobao.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gld.fzhhl.top

[U36] Py：定时任务
来源：http://iif.sysykeji.top

schedule.every(10).minutes.do(job)
来源：http://ivt.sufxvd.cn

[U37] Py：读写 Excel
来源：http://nju.dashuyun.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qia.meibo888.top

[U38] Py：获取脚本所在目录
来源：http://lft.vehdjk.com

Path(__file__).resolve().parent
来源：http://boj.gaohongyu789.top

[U39] Py：判断是否在交互环境
来源：http://rso.nanxinkj.top

sys.stdout.isatty()
来源：http://tyw.ehwqpu.com

[U40] Py：打印到标准错误
来源：http://tsl.yanxiufei.cn

print("err", file=sys.stderr)
来源：http://ura.jqgufenzy.top

[U41] PHP：初始化 Composer 项目
来源：http://umu.yueranfly.top

composer init;  composer require guzzlehttp/guzzle
来源：http://pfh.vehdjk.com

[U42] PHP：PSR-4 自动加载
来源：http://ufa.nanxuanxn.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vlo.yj20258888.top

[U43] PHP：声明命名空间
来源：http://qin.yj20258.top

namespace App\Http;
来源：http://qwj.jlsjyb.cn

[U44] PHP：开启严格类型
来源：http://iow.daxiang520.top

declare(strict_types=1);
来源：http://zyn.uphjek.com

[U45] PHP：类型声明与返回类型
来源：http://hzf.fehbvm.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://ixa.xuetiantiany.cn

[U46] PHP：可空类型
来源：http://dhg.redwolf501.top

?string $name = null
来源：http://aou.mhx1999.top

[U47] PHP：联合类型
来源：http://kum.shzxlz.cn

int|string $id
来源：http://urn.vehdjk.com

[U48] PHP：纯枚举
来源：http://nay.hysaishi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hxk.wangshuangyany.cn

[U49] PHP：只读属性
来源：http://ysg.cucudq.cn

public readonly string $name
来源：http://qds.cucudq.cn

[U50] PHP：构造器属性提升
来源：http://uty.shzxlz.cn

public function __construct(private int $id) {}
来源：http://aiz.wangshuangyany.cn

[U51] PHP：数组解构
来源：http://bvf.aizwys.cn

[$a, $b] = $arr;
来源：http://dnp.guowangkeji.top

[U52] PHP：箭头函数
来源：http://lre.shuidangran.top

$double = fn($x) => $x * 2;
来源：http://jun.sysykeji.top

[U53] PHP：空合并运算符
来源：http://wao.zhixingplan.top

$v = $a ?? $b ?? "default";
来源：http://hio.hysaishi.cn

[U54] PHP：空安全调用
来源：http://hzq.daxiang520.top

$obj?->method()
来源：http://ilo.yvedp.cn

[U55] PHP：match 表达式
来源：http://ioy.zhoulong.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://voi.nwbrower.top

[U56] PHP：命名参数
来源：http://ikx.vqdsnc.cn

f(a: 1, b: 2)
来源：http://hju.svipenyu.cn

[U57] PHP：字符串插值
来源：http://rsu.yj20258888.top

"值: {$a}"
来源：http://flv.yongpay.top

[U58] PHP：数组三件套
来源：http://esi.vehdjk.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bps.hesvh.cn

[U59] PHP：自定义排序
来源：http://uid.nanxinkj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iil.316326.xyz

[U60] PHP：JSON 编解码
来源：http://kkt.zhixingplan.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://acs.yueranfly.top

[U61] PHP：正则
来源：http://jtl.zycfv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dew.uphjek.com

[U62] PHP：日期对象
来源：http://eob.jianghu66.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bvh.xuanzx.com


<!-- 参考信息 -->