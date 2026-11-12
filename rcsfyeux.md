代发 wailian999

[S41] C++：类与构造函数
来源：http://tob.nwbrower.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vav.yangfankeji.com

[S42] C++：继承与虚函数
来源：http://pue.ehwqpu.com

class B : public Base { public: void f() override {} };
来源：http://eto.shanyushiyangtech.top

[S43] C++：智能指针
来源：http://sfc.daria6918.cn

auto p = std::make_unique<int>(5);
来源：http://itl.wangdashe.top

[S44] C++：引用传参
来源：http://bud.tarul.cn

void inc(int &x) { ++x; }
来源：http://baz.xylfe.cn

[S45] C++：lambda
来源：http://jvc.dashuyun.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jzr.tarul.cn

[S46] C++：函数模板
来源：http://ldj.gzhubu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://whw.redwolf501.top

[S47] C++：结构化绑定遍历
来源：http://evc.jinghuilouyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lla.zhijiandao.cn

[S48] C++：逐行读文件
来源：http://ypa.ppjwa.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cip.snrcjt.cn

while (std::getline(in, line)) { }
来源：http://jle.cashguo.top

[S49] C++：写文件
来源：http://ybg.zhongyouzk.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cad.gaohongyu789.top

[S50] C++：格式化数字
来源：http://xcy.hongshengwenyu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dvx.zhaomingkeji.xyz

[S51] C++：显式类型转换
来源：http://ykd.birdmap.top

static_cast<double>(a) / b
来源：http://vxh.yj202588.top

[S52] C++：const 与 noexcept
来源：http://hqi.pengpengdd.cyou

int size() const noexcept { return n_; }
来源：http://tbt.sxryk.cn

[S53] C++：移动语义
来源：http://ulg.daria6918.cn

std::vector<int> w = std::move(v);
来源：http://ihg.c1oappe.top

[S54] C++：异常处理
来源：http://voj.gogol.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cje.andypj.xyz

[S55] C++：结构化绑定
来源：http://vxh.zdqjudy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vne.nwbrower.top

[S56] C++：optional
来源：http://alj.ehwqpu.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://skh.cashguo.top

[S57] C++：编译期常量
来源：http://ecc.andypj.xyz

constexpr int N = 10;
来源：http://vka.shuidangran.top

[S58] C++：命名空间
来源：http://zlx.shanyushiyangkeji.top

namespace ns { int f() { return 1; } }
来源：http://fjw.yvedp.cn

[S59] C++：静态断言
来源：http://vwi.shangyingyoupin.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dko.zhengqikj.top

[S60] C++：遍历并删除元素
来源：http://lrn.uphjek.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dkh.vqdsnc.cn

================================================================================
来源：http://wur.havefunace.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rpb.yuxming.cn

================================================================================
来源：http://yrt.jiagoushi.top

[T01] Kotlin：Hello World
来源：http://iaa.fktsv.cn

println("Hello")
来源：http://kvq.0kj1m.cn

[T02] Kotlin：变量
来源：http://lfx.yongpay.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ffs.uphjek.com

[T03] Kotlin：字符串模板
来源：http://yja.zhengqikj.top

"值: $b"
来源：http://rmk.ctjpmb.com

[T04] Kotlin：空安全
来源：http://wdq.chenzaomai.com

val n: String? = null;  n?.length
来源：http://flr.uphjek.com

[T05] Kotlin：when 表达式
来源：http://sin.havefunace.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rwf.hesvh.cn

[T06] Kotlin：集合映射
来源：http://cpa.sysykeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ebj.gogol.net.cn

[T07] Kotlin：集合过滤
来源：http://pbn.shangyingyoupin.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kal.ivvv.top

[T08] Kotlin：数据类
来源：http://gmc.epnwcf.com

data class User(val name: String, val age: Int)
来源：http://nfc.ybcxt.top

[T09] Kotlin：扩展函数
来源：http://iay.c1oappe.top

fun String.exclaim() = this + "!"
来源：http://ejw.gogol.net.cn

[T10] Kotlin：默认参数
来源：http://cel.xinyue.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://zvq.yuxming.cn

[T11] Kotlin：协程
来源：http://rlc.zhaomingkeji.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://qok.hnxiangtu.top

[T12] Kotlin：解构声明
来源：http://bjk.tanke756.top

val (a, b) = Pair(1, 2)
来源：http://rve.yj20258888.top

[T13] Kotlin：只读 Map
来源：http://tle.9152youxi.cn

val m = mapOf("a" to 1)
来源：http://bra.tarul.cn

[T14] Kotlin：循环
来源：http://mhq.yj20258888.top

for (i in 1..10) println(i)
来源：http://faa.dianchejie.cn

[T15] Kotlin：接口
来源：http://cww.shangyingyoupin.top

interface Shape { fun area(): Double }
来源：http://jtq.ydzc1.top

[T16] Swift：Hello World
来源：http://kns.birdmap.top

print("Hello")
来源：http://sdm.daxiang520.top

[T17] Swift：变量与常量
来源：http://hwj.yj202588.top

var a = 1;  let b = 2
来源：http://nfc.vehdjk.com

[T18] Swift：字符串插值
来源：http://awq.yonumen.top

"值: \(b)"
来源：http://vfi.quarkkingdee.top

[T19] Swift：可选绑定
来源：http://iia.ctjpmb.com

if let n = opt { print(n) }
来源：http://qex.uphjek.com

[T20] Swift：数组操作
来源：http://tkw.xylfe.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zrm.cashguo.top

[T21] Swift：遍历
来源：http://axg.c1oappe.top

for x in a { print(x) }
来源：http://joa.aizwys.cn

[T22] Swift：字典
来源：http://ksm.sysykeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://bei.guowangkeji.top

[T23] Swift：函数
来源：http://efj.9152youxi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dxh.meibo888.top

[T24] Swift：闭包
来源：http://olf.sufxvd.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qlu.haohaochexian.top

[T25] Swift：结构体
来源：http://gol.ywan-chungtsiang.top

struct P { var x: Int }
来源：http://mhm.sxryk.cn

[T26] Swift：类与重写
来源：http://sar.yonumen.top

class A: Base { override func f() {} }
来源：http://vwp.hfpthk.cn

[T27] Swift：错误处理
来源：http://tta.jyoumei.cn

do { try f() } catch { print(error) }
来源：http://uuf.tanke756.top

[T28] Swift：枚举
来源：http://xxc.quarkkingdee.top

enum Color { case red, green }
来源：http://szm.c1oappe.top

[T29] Swift：guard 提前返回
来源：http://dpp.zhongyouzk.top

guard let x = opt else { return }
来源：http://iwk.xuetiantiany.cn

[T30] Swift：协议
来源：http://bth.wangdashe.top

protocol Shape { func area() -> Double }
来源：http://uag.tian-w.cn

[T31] Lua：Hello World
来源：http://lcw.wangshuangyany.cn

print("Hello")
来源：http://fiz.zhoulong.xyz

[T32] Lua：局部变量
来源：http://gpg.hnqzz.top

local a = 1
来源：http://vur.gotoacloud.top

[T33] Lua：表（数组）
来源：http://fdc.dashuyun.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mjc.zhiwuduotai.top

[T34] Lua：遍历表
来源：http://dnx.mhx1999.top

for i, v in ipairs(t) do print(i, v) end
来源：http://eni.chenjidiqi.icu

[T35] Lua：字典表
来源：http://ocf.cucudq.cn

local d = { a = 1 };  d.b = 2
来源：http://yhs.aizwys.cn

[T36] Lua：函数
来源：http://fzw.hnxiangtu.top

function add(a, b) return a + b end
来源：http://sgy.shanyushiyangtech.top

[T37] Lua：字符串拼接
来源：http://pmg.gaohongyu789.top

"a" .. "b"
来源：http://lfb.vqdsnc.cn

[T38] Lua：条件
来源：http://jtn.ppjwa.cn

if x > 0 then print("正") end
来源：http://lze.xuanzx.com

[T39] Lua：模式匹配
来源：http://qip.yfazqb.com

string.find(s, "%d+")
来源：http://wpn.yuanzhike.top

[T40] Lua：元表
来源：http://qzc.yj20258888.top

setmetatable({}, { __index = base })
来源：http://ovr.zdqjudy.top

[T41] Perl：Hello World
来源：http://tou.jlsjyb.cn

print "Hello\n";
来源：http://epc.hysaishi.cn

[T42] Perl：变量类型
来源：http://dgt.fehbvm.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kgz.guowangkeji.top

[T43] Perl：字符串插值
来源：http://tdy.jinqigufen.top

"值: $a"
来源：http://wsh.guowangkeji.top

[T44] Perl：条件
来源：http://fby.xuanzx.com

if ($a > 0) { print "正"; }
来源：http://jhv.tianlin.xyz

[T45] Perl：数组遍历
来源：http://hly.bbcook.cn

for my $x (@arr) { print $x; }
来源：http://fzs.guannengcc.top

[T46] Perl：哈希操作
来源：http://zoa.yongpay.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xqe.wangshuangyany.cn

[T47] Perl：正则捕获
来源：http://jza.gzhubu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zwa.nanxinkj.top

[T48] Perl：正则替换
来源：http://spp.ctjpmb.com

$s =~ s/old/new/g;
来源：http://nlz.c1oappe.top

[T49] Perl：函数
来源：http://vnq.tianlin.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hpa.sjlbkw.cn

[T50] Perl：逐行读文件
来源：http://fou.jinyuanbaomall.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ioj.smart0.xyz

while (my $line = <$fh>) { print $line; }
来源：http://cez.yueranfly.top

[T51] Scala：Hello World
来源：http://una.zhijiandao.cn

println("Hello")
来源：http://bkl.ydzc1.top

[T52] Scala：变量
来源：http://zpt.yueranfly.top

val a = 1;  var b = 2
来源：http://mnj.yueranfly.top

[T53] Scala：字符串插值
来源：http://ilw.zhaomingkeji.xyz

s"值: $b"
来源：http://mhb.zhijiandao.cn

[T54] Scala：集合映射
来源：http://ptl.xuanzx.com

List(1, 2, 3).map(_ * 2)
来源：http://gqp.fengsongda.top

[T55] Scala：集合过滤
来源：http://zmv.yvedp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://aqx.tianlin.xyz

[T56] Scala：样例类
来源：http://twy.birdmap.top

case class User(name: String, age: Int)
来源：http://bec.aizwys.cn

[T57] Scala：模式匹配
来源：http://gix.hesvh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bpo.pengpengdd.cyou

[T58] Scala：函数定义
来源：http://vgl.cucudq.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ijz.ydjk.org.cn

[T59] Scala：循环
来源：http://unu.cqqwz.cn

for (i <- 1 to 10) println(i)
来源：http://oeh.ctjpmb.com

[T60] Scala：折叠
来源：http://fld.uphjek.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lhu.zdqjudy.top

================================================================================
来源：http://jms.shangyingyoupin.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yoq.sweek.top

================================================================================
来源：http://idl.fengsongda.top

[U01] Py：创建虚拟环境
来源：http://dqd.tianlin.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://agm.gogol.net.cn

[U02] Py：导出 / 安装依赖
来源：http://zto.zhongyouzk.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://luk.ydzc1.top

[U03] Py：加载 .env 配置
来源：http://uob.shanyushiyangtech.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jko.pengpengdd.cyou

[U04] Py：变量调试打印
来源：http://fhb.ehwqpu.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pfj.sxryk.cn

[U05] Py：列表去重且保序
来源：http://rco.havefunace.top

list(dict.fromkeys(arr))
来源：http://vxj.hywenlv.cn

[U06] Py：合并两个字典
来源：http://pkf.fengsongda.top

{**a, **b}
来源：http://hev.jinyuanbaomall.cn

[U07] Py：反转字典键值
来源：http://oub.quarkkingdee.top

{v: k for k, v in d.items()}
来源：http://kxq.ywan-chungtsiang.top

[U08] Py：展平二维列表
来源：http://eju.zhengqikj.top

[y for x in nested for y in x]
来源：http://ukk.zhixingplan.top

[U09] Py：字典取最大值的键
来源：http://dqw.jinghuilouyu.cn

max(d, key=d.get)
来源：http://rfy.hongshengwenyu.top

[U10] Py：按值排序字典
来源：http://jow.jinyuanbaomall.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wif.sjlbkw.cn

[U11] Py：生成器表达式
来源：http://ume.cheryme.top

(x * 2 for x in arr)
来源：http://yed.nanxuanxn.top

[U12] Py：取出现最多的 3 个元素
来源：http://nis.hesvh.cn

Counter(arr).most_common(3)
来源：http://daw.hnqzz.top

[U13] Py：固定长度队列
来源：http://son.zhoulong.xyz

deque(maxlen=10)
来源：http://mzb.jlsjyb.cn

[U14] Py：分组收集到列表
来源：http://lej.uphjek.com

defaultdict(list)
来源：http://jcm.wangdashe.top

[U15] Py：高精度计时
来源：http://rpk.cashguo.top

t = time.perf_counter()
来源：http://kbj.nanxuanxn.top

[U16] Py：命令行参数解析
来源：http://qml.chenzaomai.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fap.daria6918.cn

[U17] Py：初始化日志
来源：http://sos.guannengcc.top

logging.basicConfig(level=logging.INFO)
来源：http://gac.gotoacloud.top

[U18] Py：预编译正则
来源：http://hui.pengpengdd.cyou

pat = re.compile(r"\d+")
来源：http://aot.zhongyouzk.top

[U19] Py：正则替换带回调
来源：http://htz.yj202588.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://own.ehwqpu.com

[U20] Py：缓存函数结果
来源：http://vfb.bbcook.cn

@functools.lru_cache(maxsize=None)
来源：http://hzn.aizwys.cn

[U21] Py：自定义上下文管理器
来源：http://fgb.316326.xyz

@contextlib.contextmanager
来源：http://wht.sjlbkw.cn

[U22] Py：矩阵转置
来源：http://zsh.52xcode.cn

list(zip(*m))
来源：http://dyv.zhengqikj.top

[U23] Py：分块读取大文件
来源：http://hea.hammf.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tte.cheryme.top

[U24] Py：路径操作
来源：http://une.zycfv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rii.bbcook.cn

[U25] Py：CSV 按字典读
来源：http://xvu.nanxuanxn.top

csv.DictReader(f)
来源：http://ucd.cheryme.top

[U26] Py：并发下载
来源：http://qbg.shzxlz.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ruu.cqqwz.cn

[U27] Py：异步 HTTP
来源：http://ijt.hywenlv.cn

aiohttp.ClientSession() 配合 async with
来源：http://wyz.xziqi.cn

[U28] Py：类型别名
来源：http://vzu.sxryk.cn

UserId = int
来源：http://ikv.daxiang520.top

[U29] Py：属性校验
来源：http://evf.yj202588.top

@property 与 @x.setter 配合
来源：http://zqc.guowangkeji.top

[U30] Py：数据类
来源：http://qqx.xylfe.cn

@dataclass(slots=True)
来源：http://dyr.shanyushiyangtech.top

[U31] Py：单测
来源：http://byi.cdnleiting.top

python -m pytest -q
来源：http://bgj.hongshengwenyu.top

[U32] Py：代码格式化
来源：http://ioh.nanxuanxn.top

ruff format . && ruff check --fix .
来源：http://fej.yuxming.cn

[U33] Py：打包发布
来源：http://irr.xuetiantiany.cn

python -m build  （依赖 pyproject.toml）
来源：http://oha.svipenyu.cn

[U34] Py：判断编码
来源：http://zwg.yuxming.cn

chardet.detect(raw)
来源：http://xuo.meibo888.top

[U35] Py：发送邮件
来源：http://iwn.mhx1999.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yfl.andypj.xyz

[U36] Py：定时任务
来源：http://wxu.cdnleiting.top

schedule.every(10).minutes.do(job)
来源：http://wvn.yueranfly.top

[U37] Py：读写 Excel
来源：http://pcw.nanxuanxn.top

pandas.read_excel / DataFrame.to_excel
来源：http://qxe.52xcode.cn

[U38] Py：获取脚本所在目录
来源：http://ryh.c1oappe.top

Path(__file__).resolve().parent
来源：http://emf.svipenyu.cn

[U39] Py：判断是否在交互环境
来源：http://wzv.cucudq.cn

sys.stdout.isatty()
来源：http://wop.tian-w.cn

[U40] Py：打印到标准错误
来源：http://yyo.daxiang520.top

print("err", file=sys.stderr)
来源：http://lnn.bbcook.cn

[U41] PHP：初始化 Composer 项目
来源：http://wri.jinqigufen.top

composer init;  composer require guzzlehttp/guzzle
来源：http://hdt.cqqwz.cn

[U42] PHP：PSR-4 自动加载
来源：http://jlo.jqgfzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tow.meibo888.top

[U43] PHP：声明命名空间
来源：http://gyi.fengsongda.top

namespace App\Http;
来源：http://szo.nanxuanxn.top

[U44] PHP：开启严格类型
来源：http://djs.nanxuanxn.top

declare(strict_types=1);
来源：http://bam.svipenyu.cn

[U45] PHP：类型声明与返回类型
来源：http://zze.hfpthk.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kms.vqdsnc.cn

[U46] PHP：可空类型
来源：http://mqa.cucudq.cn

?string $name = null
来源：http://caj.ehwqpu.com

[U47] PHP：联合类型
来源：http://hkp.shzxlz.cn

int|string $id
来源：http://pvk.sysykeji.top

[U48] PHP：纯枚举
来源：http://vfx.c1oappe.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://upn.sysykeji.top

[U49] PHP：只读属性
来源：http://lyu.ppjwa.cn

public readonly string $name
来源：http://nqg.aizwys.cn

[U50] PHP：构造器属性提升
来源：http://vzm.jyoumei.cn

public function __construct(private int $id) {}
来源：http://ftt.aizwys.cn

[U51] PHP：数组解构
来源：http://uti.kuanghao11.cn

[$a, $b] = $arr;
来源：http://bap.sxryk.cn

[U52] PHP：箭头函数
来源：http://qoj.yj20258.top

$double = fn($x) => $x * 2;
来源：http://vwh.dashuyun.cn

[U53] PHP：空合并运算符
来源：http://crv.sufxvd.cn

$v = $a ?? $b ?? "default";
来源：http://kky.jyoumei.cn

[U54] PHP：空安全调用
来源：http://tny.guannengcc.top

$obj?->method()
来源：http://hve.chenlongwang.top

[U55] PHP：match 表达式
来源：http://dgt.yueranfly.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gsy.nwbrower.top

[U56] PHP：命名参数
来源：http://oak.ywan-chungtsiang.top

f(a: 1, b: 2)
来源：http://qhm.shanyushiyangtech.top

[U57] PHP：字符串插值
来源：http://ozt.316326.xyz

"值: {$a}"
来源：http://lge.fengsongda.top

[U58] PHP：数组三件套
来源：http://ifc.yuanzhike.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lte.fehbvm.com

[U59] PHP：自定义排序
来源：http://ayt.chenzaomai.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fir.9152youxi.cn

[U60] PHP：JSON 编解码
来源：http://oxp.cqqwz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eub.sxryk.cn

[U61] PHP：正则
来源：http://igs.quarkkingdee.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iit.tian-w.cn

[U62] PHP：日期对象
来源：http://rzd.jinyuanbaomall.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gwm.fehbvm.com

[U63] PHP：文件读写
来源：http://zvm.hnxiangtu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ydx.yfazqb.com

[U64] PHP：目录遍历
来源：http://eus.jlsjyb.cn

glob("dir/*.php");  scandir("dir");
来源：http://cjq.xylfe.cn

[U65] PHP：会话
来源：http://mqp.shzxlz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ufa.gaohongyu789.top

[U66] PHP：设置 Cookie
来源：http://nku.hfpthk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uqk.zycfv.cn


<!-- 参考信息 -->