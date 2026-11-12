代发 wailian999

[S37] C++：set
来源：http://hio.yfazqb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lqi.hcnkem.com

[S38] C++：排序
来源：http://zfl.9152youxi.cn

std::sort(v.begin(), v.end());
来源：http://gqq.jiagoushi.top

[S39] C++：自定义比较器排序
来源：http://cxv.nanxinkj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wgy.xylfe.cn

[S40] C++：查找元素
来源：http://ore.aibaodan.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://thz.ppjwa.cn

[S41] C++：类与构造函数
来源：http://stw.gotoacloud.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ppl.hammf.cn

[S42] C++：继承与虚函数
来源：http://nol.yuanzhike.top

class B : public Base { public: void f() override {} };
来源：http://rmf.tanke756.top

[S43] C++：智能指针
来源：http://tjz.xuetiantiany.cn

auto p = std::make_unique<int>(5);
来源：http://tqh.zdqjudy.top

[S44] C++：引用传参
来源：http://ved.fehbvm.com

void inc(int &x) { ++x; }
来源：http://tli.jlsjyb.cn

[S45] C++：lambda
来源：http://zlk.havefunace.top

auto add = [](int a, int b) { return a + b; };
来源：http://pnb.xuanzx.com

[S46] C++：函数模板
来源：http://ojn.tianlin.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hgx.nanxuanxn.top

[S47] C++：结构化绑定遍历
来源：http://jbt.yongpay.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qck.yj20258888.top

[S48] C++：逐行读文件
来源：http://lwh.jqgufenzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://qcl.nanxuanxn.top

while (std::getline(in, line)) { }
来源：http://rly.kuanghao11.cn

[S49] C++：写文件
来源：http://spz.hysaishi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dbf.yvedp.cn

[S50] C++：格式化数字
来源：http://lag.andypj.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ikj.nanxinkj.top

[S51] C++：显式类型转换
来源：http://wkt.meibo888.top

static_cast<double>(a) / b
来源：http://frq.c1oappe.top

[S52] C++：const 与 noexcept
来源：http://tqn.xingfuxueyuan.xyz

int size() const noexcept { return n_; }
来源：http://bvk.vehdjk.com

[S53] C++：移动语义
来源：http://ggl.uphjek.com

std::vector<int> w = std::move(v);
来源：http://dyg.yangfankeji.com

[S54] C++：异常处理
来源：http://pkq.mhx1999.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ubd.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://ckn.andypj.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://qin.guowangkeji.top

[S56] C++：optional
来源：http://dzw.hongshengwenyu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nlc.tianlin.xyz

[S57] C++：编译期常量
来源：http://lnf.nanxinkj.top

constexpr int N = 10;
来源：http://fhf.gotoacloud.top

[S58] C++：命名空间
来源：http://jkn.vehdjk.com

namespace ns { int f() { return 1; } }
来源：http://rbx.haohaochexian.top

[S59] C++：静态断言
来源：http://seb.zdqjudy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ser.sufxvd.cn

[S60] C++：遍历并删除元素
来源：http://zql.xziqi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hhr.yangfankeji.com

================================================================================
来源：http://ocz.52xcode.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yuh.xinyue.icu

================================================================================
来源：http://klg.gogol.net.cn

[T01] Kotlin：Hello World
来源：http://uxd.jyoumei.cn

println("Hello")
来源：http://ydg.yonumen.top

[T02] Kotlin：变量
来源：http://vps.shanyushiyangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mmu.daria6918.cn

[T03] Kotlin：字符串模板
来源：http://hso.zhoulong.xyz

"值: $b"
来源：http://uob.gogol.net.cn

[T04] Kotlin：空安全
来源：http://cbu.vehdjk.com

val n: String? = null;  n?.length
来源：http://hkk.hammf.cn

[T05] Kotlin：when 表达式
来源：http://uyx.fengsongda.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bjl.wangshuangyany.cn

[T06] Kotlin：集合映射
来源：http://dli.fzhhl.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qak.bjfxy.top

[T07] Kotlin：集合过滤
来源：http://cmw.guowangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nss.jqgfzy.top

[T08] Kotlin：数据类
来源：http://thm.tarul.cn

data class User(val name: String, val age: Int)
来源：http://gtj.ppjwa.cn

[T09] Kotlin：扩展函数
来源：http://mur.yvedp.cn

fun String.exclaim() = this + "!"
来源：http://mgk.fengsongda.top

[T10] Kotlin：默认参数
来源：http://vgc.snrcjt.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wgt.sufxvd.cn

[T11] Kotlin：协程
来源：http://qle.cheryme.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gsc.yueranfly.top

[T12] Kotlin：解构声明
来源：http://kdf.andypj.xyz

val (a, b) = Pair(1, 2)
来源：http://xkl.zhixingplan.top

[T13] Kotlin：只读 Map
来源：http://csm.fzhhl.top

val m = mapOf("a" to 1)
来源：http://wwa.andypj.xyz

[T14] Kotlin：循环
来源：http://shd.gogol.net.cn

for (i in 1..10) println(i)
来源：http://fwl.aibaodan.cn

[T15] Kotlin：接口
来源：http://nbg.hnqzz.top

interface Shape { fun area(): Double }
来源：http://kfg.quarkkingdee.top

[T16] Swift：Hello World
来源：http://fzj.nanxuanxn.top

print("Hello")
来源：http://iqh.aibaodan.cn

[T17] Swift：变量与常量
来源：http://yts.snrcjt.cn

var a = 1;  let b = 2
来源：http://cae.cdnleiting.top

[T18] Swift：字符串插值
来源：http://ych.fengsongda.top

"值: \(b)"
来源：http://kbk.iojbl.cn

[T19] Swift：可选绑定
来源：http://gey.gzhubu.top

if let n = opt { print(n) }
来源：http://sid.haohaochexian.top

[T20] Swift：数组操作
来源：http://seh.jianghu66.top

var a = [1, 2, 3];  a.append(4)
来源：http://pnl.hywenlv.cn

[T21] Swift：遍历
来源：http://lqj.mhx1999.top

for x in a { print(x) }
来源：http://lze.yanxiufei.cn

[T22] Swift：字典
来源：http://zwe.fanxiaobao.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://hwv.ydzc1.top

[T23] Swift：函数
来源：http://mmx.fanxiaobao.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://paz.ctjpmb.com

[T24] Swift：闭包
来源：http://xbo.yj20258888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://qci.xziqi.cn

[T25] Swift：结构体
来源：http://khc.fengsongda.top

struct P { var x: Int }
来源：http://twl.tian-w.cn

[T26] Swift：类与重写
来源：http://lfv.nwbrower.top

class A: Base { override func f() {} }
来源：http://amk.jinyuanbaomall.cn

[T27] Swift：错误处理
来源：http://hrp.mhx1999.top

do { try f() } catch { print(error) }
来源：http://uxn.xylfe.cn

[T28] Swift：枚举
来源：http://ecu.zdqjudy.top

enum Color { case red, green }
来源：http://syk.yuxming.cn

[T29] Swift：guard 提前返回
来源：http://jyv.xziqi.cn

guard let x = opt else { return }
来源：http://gqj.xuetiantiany.cn

[T30] Swift：协议
来源：http://sbi.jyoumei.cn

protocol Shape { func area() -> Double }
来源：http://kur.aibaodan.cn

[T31] Lua：Hello World
来源：http://ida.svipenyu.cn

print("Hello")
来源：http://kqq.gaohongyu789.top

[T32] Lua：局部变量
来源：http://pji.guowangkeji.top

local a = 1
来源：http://vja.jyoumei.cn

[T33] Lua：表（数组）
来源：http://rou.hesvh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vym.smart0.xyz

[T34] Lua：遍历表
来源：http://vzd.gaohongyu789.top

for i, v in ipairs(t) do print(i, v) end
来源：http://nfx.bjfxy.top

[T35] Lua：字典表
来源：http://ckm.fanxiaobao.xyz

local d = { a = 1 };  d.b = 2
来源：http://uro.jinghuilouyu.cn

[T36] Lua：函数
来源：http://abl.ywan-chungtsiang.top

function add(a, b) return a + b end
来源：http://imn.svipenyu.cn

[T37] Lua：字符串拼接
来源：http://pdn.sxryk.cn

"a" .. "b"
来源：http://cww.yfazqb.com

[T38] Lua：条件
来源：http://uzu.xylfe.cn

if x > 0 then print("正") end
来源：http://hyk.jinqigufen.top

[T39] Lua：模式匹配
来源：http://woc.snrcjt.cn

string.find(s, "%d+")
来源：http://vuq.pycfn.com

[T40] Lua：元表
来源：http://oag.yj20258888.top

setmetatable({}, { __index = base })
来源：http://erx.cashguo.top

[T41] Perl：Hello World
来源：http://rin.andypj.xyz

print "Hello\n";
来源：http://fzk.316326.xyz

[T42] Perl：变量类型
来源：http://ind.nanxuanxn.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yll.kuanghao11.cn

[T43] Perl：字符串插值
来源：http://cgl.xuanzx.com

"值: $a"
来源：http://yyt.uphjek.com

[T44] Perl：条件
来源：http://xxh.quarkkingdee.top

if ($a > 0) { print "正"; }
来源：http://rxi.cashguo.top

[T45] Perl：数组遍历
来源：http://zlx.0kj1m.cn

for my $x (@arr) { print $x; }
来源：http://olb.vqdsnc.cn

[T46] Perl：哈希操作
来源：http://cax.0kj1m.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baz.yfazqb.com

[T47] Perl：正则捕获
来源：http://ahc.xuetiantiany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qil.pycfn.com

[T48] Perl：正则替换
来源：http://gdd.ivvv.top

$s =~ s/old/new/g;
来源：http://hkv.zhiwuduotai.top

[T49] Perl：函数
来源：http://dnv.guannengcc.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://aoc.xinyue.icu

[T50] Perl：逐行读文件
来源：http://dux.zhiwuduotai.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mju.fanxiaobao.xyz

while (my $line = <$fh>) { print $line; }
来源：http://jow.dianchejie.cn

[T51] Scala：Hello World
来源：http://lnr.andypj.xyz

println("Hello")
来源：http://sdd.jiagoushi.top

[T52] Scala：变量
来源：http://rjx.xziqi.cn

val a = 1;  var b = 2
来源：http://bha.yj20258888.top

[T53] Scala：字符串插值
来源：http://jaj.aizwys.cn

s"值: $b"
来源：http://pyu.jyoumei.cn

[T54] Scala：集合映射
来源：http://ftu.vqdsnc.cn

List(1, 2, 3).map(_ * 2)
来源：http://tii.chenlongwang.top

[T55] Scala：集合过滤
来源：http://poz.cucudq.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yup.hcnkem.com

[T56] Scala：样例类
来源：http://nfi.fengsongda.top

case class User(name: String, age: Int)
来源：http://fbj.bbcook.cn

[T57] Scala：模式匹配
来源：http://wan.xinyue.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://rjl.pycfn.com

[T58] Scala：函数定义
来源：http://dhp.zdqjudy.top

def add(a: Int, b: Int): Int = a + b
来源：http://gwu.ywan-chungtsiang.top

[T59] Scala：循环
来源：http://biz.shanyushiyangtech.top

for (i <- 1 to 10) println(i)
来源：http://tub.zhiwuduotai.top

[T60] Scala：折叠
来源：http://uxm.cashguo.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wvy.bbcook.cn

================================================================================
来源：http://ilt.0kj1m.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xar.yongpay.top

================================================================================
来源：http://ull.shzxlz.cn

[U01] Py：创建虚拟环境
来源：http://wxd.gogol.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nms.yuxming.cn

[U02] Py：导出 / 安装依赖
来源：http://gba.xinyue.icu

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://szj.xuanzx.com

[U03] Py：加载 .env 配置
来源：http://evn.aibaodan.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wkb.zhiwuduotai.top

[U04] Py：变量调试打印
来源：http://mak.mhx1999.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wyp.yongpay.top

[U05] Py：列表去重且保序
来源：http://pxj.cucudq.cn

list(dict.fromkeys(arr))
来源：http://num.9152youxi.cn

[U06] Py：合并两个字典
来源：http://ubq.fanxiaobao.xyz

{**a, **b}
来源：http://esd.ivvv.top

[U07] Py：反转字典键值
来源：http://ywm.yuxming.cn

{v: k for k, v in d.items()}
来源：http://kff.nanxuanxn.top

[U08] Py：展平二维列表
来源：http://iei.jinqigfzy.top

[y for x in nested for y in x]
来源：http://fgm.smart0.xyz

[U09] Py：字典取最大值的键
来源：http://khy.gzhubu.top

max(d, key=d.get)
来源：http://cpr.aibaodan.cn

[U10] Py：按值排序字典
来源：http://ydv.yj20258888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eqx.svipenyu.cn

[U11] Py：生成器表达式
来源：http://zzs.cashguo.top

(x * 2 for x in arr)
来源：http://ugh.zhaomingkeji.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://let.quarkkingdee.top

Counter(arr).most_common(3)
来源：http://qwk.fktsv.cn

[U13] Py：固定长度队列
来源：http://uio.yonumen.top

deque(maxlen=10)
来源：http://wce.quarkkingdee.top

[U14] Py：分组收集到列表
来源：http://nyg.sjlbkw.cn

defaultdict(list)
来源：http://nop.xuetiantiany.cn

[U15] Py：高精度计时
来源：http://qma.ywan-chungtsiang.top

t = time.perf_counter()
来源：http://owd.svipenyu.cn

[U16] Py：命令行参数解析
来源：http://ktw.ivvv.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nsc.ehwqpu.com

[U17] Py：初始化日志
来源：http://wdo.fzhhl.top

logging.basicConfig(level=logging.INFO)
来源：http://lmm.bjfxy.top

[U18] Py：预编译正则
来源：http://qft.wangshuangyany.cn

pat = re.compile(r"\d+")
来源：http://nas.ctjpmb.com

[U19] Py：正则替换带回调
来源：http://ftx.sweek.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eip.redwolf501.top

[U20] Py：缓存函数结果
来源：http://uiz.chenzaomai.com

@functools.lru_cache(maxsize=None)
来源：http://hen.jinqigfzy.top

[U21] Py：自定义上下文管理器
来源：http://gda.cdnleiting.top

@contextlib.contextmanager
来源：http://yjy.zhongyouzk.top

[U22] Py：矩阵转置
来源：http://qqb.yuxming.cn

list(zip(*m))
来源：http://qsi.gogol.net.cn

[U23] Py：分块读取大文件
来源：http://ata.yvedp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wdt.chenlongwang.top

[U24] Py：路径操作
来源：http://gdk.gaohongyu789.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jdo.ydzc1.top

[U25] Py：CSV 按字典读
来源：http://nzn.uphjek.com

csv.DictReader(f)
来源：http://xxd.shangyingyoupin.top

[U26] Py：并发下载
来源：http://ewn.uphjek.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ttp.zdqjudy.top

[U27] Py：异步 HTTP
来源：http://dug.tarul.cn

aiohttp.ClientSession() 配合 async with
来源：http://eky.shzxlz.cn

[U28] Py：类型别名
来源：http://npx.pycfn.com

UserId = int
来源：http://utx.yvedp.cn

[U29] Py：属性校验
来源：http://qwb.ywan-chungtsiang.top

@property 与 @x.setter 配合
来源：http://igq.cheryme.top

[U30] Py：数据类
来源：http://ukj.chenzaomai.com

@dataclass(slots=True)
来源：http://piv.fktsv.cn

[U31] Py：单测
来源：http://zjg.birdmap.top

python -m pytest -q
来源：http://dnb.yueranfly.top

[U32] Py：代码格式化
来源：http://tgp.hfpthk.cn

ruff format . && ruff check --fix .
来源：http://ipa.redwolf501.top

[U33] Py：打包发布
来源：http://ivc.c1oappe.top

python -m build  （依赖 pyproject.toml）
来源：http://lrv.fengsongda.top

[U34] Py：判断编码
来源：http://wdc.0kj1m.cn

chardet.detect(raw)
来源：http://srp.meibo888.top

[U35] Py：发送邮件
来源：http://jwv.nanxinkj.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oyr.nanxuanxn.top

[U36] Py：定时任务
来源：http://fig.daria6918.cn

schedule.every(10).minutes.do(job)
来源：http://nwp.shzxlz.cn

[U37] Py：读写 Excel
来源：http://bfa.fengsongda.top

pandas.read_excel / DataFrame.to_excel
来源：http://edg.hesvh.cn

[U38] Py：获取脚本所在目录
来源：http://rmr.zhixingplan.top

Path(__file__).resolve().parent
来源：http://wqf.gaohongyu789.top

[U39] Py：判断是否在交互环境
来源：http://guj.yj20258888.top

sys.stdout.isatty()
来源：http://wus.fktsv.cn

[U40] Py：打印到标准错误
来源：http://eow.zhiwuduotai.top

print("err", file=sys.stderr)
来源：http://nlp.gogol.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://ckt.zhongyouzk.top

composer init;  composer require guzzlehttp/guzzle
来源：http://yil.shzxlz.cn

[U42] PHP：PSR-4 自动加载
来源：http://qsu.zhijiandao.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uyk.dianchejie.cn

[U43] PHP：声明命名空间
来源：http://kjx.jqgufenzy.top

namespace App\Http;
来源：http://mrf.havefunace.top

[U44] PHP：开启严格类型
来源：http://whr.andypj.xyz

declare(strict_types=1);
来源：http://mtk.pengpengdd.cyou

[U45] PHP：类型声明与返回类型
来源：http://qmj.hesvh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ydd.xuetiantiany.cn

[U46] PHP：可空类型
来源：http://aoh.jiagoushi.top

?string $name = null
来源：http://slk.dianchejie.cn

[U47] PHP：联合类型
来源：http://ehc.uphjek.com

int|string $id
来源：http://ljn.zhijiandao.cn

[U48] PHP：纯枚举
来源：http://ozm.smart0.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://saq.hongshengwenyu.top

[U49] PHP：只读属性
来源：http://auc.jinqigfzy.top

public readonly string $name
来源：http://oex.fzhhl.top

[U50] PHP：构造器属性提升
来源：http://aas.yanxiufei.cn

public function __construct(private int $id) {}
来源：http://abp.ppjwa.cn

[U51] PHP：数组解构
来源：http://wnr.zhoulong.xyz

[$a, $b] = $arr;
来源：http://yjb.guowangkeji.top

[U52] PHP：箭头函数
来源：http://gqf.birdmap.top

$double = fn($x) => $x * 2;
来源：http://qrb.tarul.cn

[U53] PHP：空合并运算符
来源：http://qeu.gzhubu.top

$v = $a ?? $b ?? "default";
来源：http://mug.fengsongda.top

[U54] PHP：空安全调用
来源：http://bmg.meibo888.top

$obj?->method()
来源：http://swy.hesvh.cn

[U55] PHP：match 表达式
来源：http://zyr.andypj.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tvv.xylfe.cn

[U56] PHP：命名参数
来源：http://ofn.xinyue.icu

f(a: 1, b: 2)
来源：http://qkf.sxryk.cn

[U57] PHP：字符串插值
来源：http://lyy.chenlongwang.top

"值: {$a}"
来源：http://gvz.cdnleiting.top

[U58] PHP：数组三件套
来源：http://wzm.gogol.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://eoq.zhoulong.xyz

[U59] PHP：自定义排序
来源：http://bfo.ydjk.org.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pmk.jiagoushi.top

[U60] PHP：JSON 编解码
来源：http://ohm.jqgfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zrr.yanxiufei.cn

[U61] PHP：正则
来源：http://myp.jiagoushi.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nls.ivvv.top

[U62] PHP：日期对象
来源：http://pxi.yueranfly.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vnm.shangyingyoupin.top


<!-- 参考信息 -->