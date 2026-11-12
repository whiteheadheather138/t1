代发 wailian999

[S41] C++：类与构造函数
来源：http://njy.sufxvd.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ymy.redwolf501.top

[S42] C++：继承与虚函数
来源：http://tyx.jlsjyb.cn

class B : public Base { public: void f() override {} };
来源：http://pfk.redwolf501.top

[S43] C++：智能指针
来源：http://nlm.chenlongwang.top

auto p = std::make_unique<int>(5);
来源：http://cfj.birdmap.top

[S44] C++：引用传参
来源：http://dvc.xuanzx.com

void inc(int &x) { ++x; }
来源：http://hto.nwbrower.top

[S45] C++：lambda
来源：http://vbu.ppjwa.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rry.quarkkingdee.top

[S46] C++：函数模板
来源：http://qlh.shangyingyoupin.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hxt.yonumen.top

[S47] C++：结构化绑定遍历
来源：http://zos.iojbl.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kgp.hnqzz.top

[S48] C++：逐行读文件
来源：http://ubs.aibaodan.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wtr.jqgfzy.top

while (std::getline(in, line)) { }
来源：http://oxj.yj20258.top

[S49] C++：写文件
来源：http://rrz.hysaishi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://udi.zhiwuduotai.top

[S50] C++：格式化数字
来源：http://yeb.tarul.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://urf.ydjk.org.cn

[S51] C++：显式类型转换
来源：http://kje.jiagoushi.top

static_cast<double>(a) / b
来源：http://rkg.jlsjyb.cn

[S52] C++：const 与 noexcept
来源：http://kyh.vehdjk.com

int size() const noexcept { return n_; }
来源：http://fzj.yj20258888.top

[S53] C++：移动语义
来源：http://fpr.hammf.cn

std::vector<int> w = std::move(v);
来源：http://yzz.fktsv.cn

[S54] C++：异常处理
来源：http://jtd.jlsjyb.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oxw.mhx1999.top

[S55] C++：结构化绑定
来源：http://lsi.mhx1999.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gcu.chenlongwang.top

[S56] C++：optional
来源：http://vgl.jqgufenzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lpu.zycfv.cn

[S57] C++：编译期常量
来源：http://fly.ywan-chungtsiang.top

constexpr int N = 10;
来源：http://muo.hfpthk.cn

[S58] C++：命名空间
来源：http://wtm.jqgfzy.top

namespace ns { int f() { return 1; } }
来源：http://jbm.kuanghao11.cn

[S59] C++：静态断言
来源：http://ijk.havefunace.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://enb.hammf.cn

[S60] C++：遍历并删除元素
来源：http://xra.yj20258888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dop.uphjek.com

================================================================================
来源：http://vhr.hongshengwenyu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://taa.xuetiantiany.cn

================================================================================
来源：http://nvj.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://txr.nwbrower.top

println("Hello")
来源：http://zsh.shzxlz.cn

[T02] Kotlin：变量
来源：http://nbx.dianchejie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ggh.shanyushiyangtech.top

[T03] Kotlin：字符串模板
来源：http://rvw.yuxming.cn

"值: $b"
来源：http://xpw.sjlbkw.cn

[T04] Kotlin：空安全
来源：http://mna.jinqigufen.top

val n: String? = null;  n?.length
来源：http://lqv.jlsjyb.cn

[T05] Kotlin：when 表达式
来源：http://udm.aibaodan.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gdy.ydzc1.top

[T06] Kotlin：集合映射
来源：http://eii.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://jsh.mhx1999.top

[T07] Kotlin：集合过滤
来源：http://fxp.bjfxy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kiw.zdqjudy.top

[T08] Kotlin：数据类
来源：http://xeh.xziqi.cn

data class User(val name: String, val age: Int)
来源：http://rmc.vehdjk.com

[T09] Kotlin：扩展函数
来源：http://fmv.jinqigufen.top

fun String.exclaim() = this + "!"
来源：http://yyq.chenlongwang.top

[T10] Kotlin：默认参数
来源：http://efl.zhijiandao.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rax.jqgufenzy.top

[T11] Kotlin：协程
来源：http://web.nanxinkj.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fze.kuanghao11.cn

[T12] Kotlin：解构声明
来源：http://dbz.zhiwuduotai.top

val (a, b) = Pair(1, 2)
来源：http://bwp.iojbl.cn

[T13] Kotlin：只读 Map
来源：http://kml.daxiang520.top

val m = mapOf("a" to 1)
来源：http://avc.gzhubu.top

[T14] Kotlin：循环
来源：http://haz.yanxiufei.cn

for (i in 1..10) println(i)
来源：http://yun.tianlin.xyz

[T15] Kotlin：接口
来源：http://atn.chenzaomai.com

interface Shape { fun area(): Double }
来源：http://del.quarkkingdee.top

[T16] Swift：Hello World
来源：http://tyn.gotoacloud.top

print("Hello")
来源：http://rsc.dashuyun.cn

[T17] Swift：变量与常量
来源：http://tft.jqgfzy.top

var a = 1;  let b = 2
来源：http://xll.nanxinkj.top

[T18] Swift：字符串插值
来源：http://gij.cheryme.top

"值: \(b)"
来源：http://ujq.birdmap.top

[T19] Swift：可选绑定
来源：http://qvo.aibaodan.cn

if let n = opt { print(n) }
来源：http://lsa.sufxvd.cn

[T20] Swift：数组操作
来源：http://aoi.gzhubu.top

var a = [1, 2, 3];  a.append(4)
来源：http://jyd.hnqzz.top

[T21] Swift：遍历
来源：http://phc.hongshengwenyu.top

for x in a { print(x) }
来源：http://kaq.c1oappe.top

[T22] Swift：字典
来源：http://dek.sxryk.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pyj.fanxiaobao.xyz

[T23] Swift：函数
来源：http://kji.xziqi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cjs.0kj1m.cn

[T24] Swift：闭包
来源：http://pnd.yongpay.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vok.zhengqikj.top

[T25] Swift：结构体
来源：http://apq.bbcook.cn

struct P { var x: Int }
来源：http://zth.52xcode.cn

[T26] Swift：类与重写
来源：http://lsu.zycfv.cn

class A: Base { override func f() {} }
来源：http://izf.vqdsnc.cn

[T27] Swift：错误处理
来源：http://iee.ehwqpu.com

do { try f() } catch { print(error) }
来源：http://dzf.yangfankeji.com

[T28] Swift：枚举
来源：http://fok.ybcxt.top

enum Color { case red, green }
来源：http://sdf.bjfxy.top

[T29] Swift：guard 提前返回
来源：http://wmj.chenlongwang.top

guard let x = opt else { return }
来源：http://mtp.tianlin.xyz

[T30] Swift：协议
来源：http://djp.ivvv.top

protocol Shape { func area() -> Double }
来源：http://ssn.meibo888.top

[T31] Lua：Hello World
来源：http://oha.yanxiufei.cn

print("Hello")
来源：http://dzs.yuanzhike.top

[T32] Lua：局部变量
来源：http://yyf.nanxuanxn.top

local a = 1
来源：http://jfa.xylfe.cn

[T33] Lua：表（数组）
来源：http://emy.ydjk.org.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fok.zycfv.cn

[T34] Lua：遍历表
来源：http://gax.yvedp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://inu.epnwcf.com

[T35] Lua：字典表
来源：http://wbs.dianchejie.cn

local d = { a = 1 };  d.b = 2
来源：http://lcq.316326.xyz

[T36] Lua：函数
来源：http://vvk.tarul.cn

function add(a, b) return a + b end
来源：http://knp.snrcjt.cn

[T37] Lua：字符串拼接
来源：http://qik.ppjwa.cn

"a" .. "b"
来源：http://ciu.tanke756.top

[T38] Lua：条件
来源：http://bcc.dianchejie.cn

if x > 0 then print("正") end
来源：http://blv.ehwqpu.com

[T39] Lua：模式匹配
来源：http://yob.gaohongyu789.top

string.find(s, "%d+")
来源：http://upr.ydjk.org.cn

[T40] Lua：元表
来源：http://feh.dashuyun.cn

setmetatable({}, { __index = base })
来源：http://inj.tianlin.xyz

[T41] Perl：Hello World
来源：http://arp.svipenyu.cn

print "Hello\n";
来源：http://zkp.aibaodan.cn

[T42] Perl：变量类型
来源：http://gge.ppjwa.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://aoe.zhengqikj.top

[T43] Perl：字符串插值
来源：http://tsn.shanyushiyangkeji.top

"值: $a"
来源：http://bpz.tianlin.xyz

[T44] Perl：条件
来源：http://rpp.ehwqpu.com

if ($a > 0) { print "正"; }
来源：http://ldo.chenzaomai.com

[T45] Perl：数组遍历
来源：http://yzb.smart0.xyz

for my $x (@arr) { print $x; }
来源：http://kll.hongshengwenyu.top

[T46] Perl：哈希操作
来源：http://umo.pengpengdd.cyou

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jgv.birdmap.top

[T47] Perl：正则捕获
来源：http://mhu.yangfankeji.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://qho.fehbvm.com

[T48] Perl：正则替换
来源：http://evq.sweek.top

$s =~ s/old/new/g;
来源：http://lgj.yfazqb.com

[T49] Perl：函数
来源：http://rwi.dashuyun.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ktm.yj202588.top

[T50] Perl：逐行读文件
来源：http://xmh.cdnleiting.top

open my $fh, "<", "a.txt" or die $!;
来源：http://kdd.cqqwz.cn

while (my $line = <$fh>) { print $line; }
来源：http://rwi.xuetiantiany.cn

[T51] Scala：Hello World
来源：http://uke.yuanzhike.top

println("Hello")
来源：http://xyq.dianchejie.cn

[T52] Scala：变量
来源：http://yhc.316326.xyz

val a = 1;  var b = 2
来源：http://qwu.cucudq.cn

[T53] Scala：字符串插值
来源：http://qso.yfazqb.com

s"值: $b"
来源：http://usl.fzhhl.top

[T54] Scala：集合映射
来源：http://xtj.chenjidiqi.icu

List(1, 2, 3).map(_ * 2)
来源：http://wax.birdmap.top

[T55] Scala：集合过滤
来源：http://bbf.ydzc1.top

List(1, 2, 3).filter(_ > 1)
来源：http://hzj.cheryme.top

[T56] Scala：样例类
来源：http://tic.gotoacloud.top

case class User(name: String, age: Int)
来源：http://gcw.yfazqb.com

[T57] Scala：模式匹配
来源：http://iqq.ppjwa.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gef.gogol.net.cn

[T58] Scala：函数定义
来源：http://zom.sysykeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://zuw.haohaochexian.top

[T59] Scala：循环
来源：http://ppq.xinyue.icu

for (i <- 1 to 10) println(i)
来源：http://nxb.yonumen.top

[T60] Scala：折叠
来源：http://ckg.cashguo.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ivy.sufxvd.cn

================================================================================
来源：http://ion.pycfn.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vmo.guannengcc.top

================================================================================
来源：http://fck.ehwqpu.com

[U01] Py：创建虚拟环境
来源：http://yiw.feifeiyinyue.top

python -m venv .venv && source .venv/bin/activate
来源：http://eot.yanxiufei.cn

[U02] Py：导出 / 安装依赖
来源：http://qxj.jinyuanbaomall.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gwo.sufxvd.cn

[U03] Py：加载 .env 配置
来源：http://rzx.jinqigufen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://yng.hesvh.cn

[U04] Py：变量调试打印
来源：http://zmk.nwbrower.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jay.yvedp.cn

[U05] Py：列表去重且保序
来源：http://cqx.fktsv.cn

list(dict.fromkeys(arr))
来源：http://cjs.iojbl.cn

[U06] Py：合并两个字典
来源：http://mvc.nanxuanxn.top

{**a, **b}
来源：http://zvp.yj20258.top

[U07] Py：反转字典键值
来源：http://ktz.52xcode.cn

{v: k for k, v in d.items()}
来源：http://nlv.fehbvm.com

[U08] Py：展平二维列表
来源：http://mup.bjfxy.top

[y for x in nested for y in x]
来源：http://qpi.52xcode.cn

[U09] Py：字典取最大值的键
来源：http://yke.yvedp.cn

max(d, key=d.get)
来源：http://ney.pengpengdd.cyou

[U10] Py：按值排序字典
来源：http://nrq.chenzaomai.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cur.shanyushiyangtech.top

[U11] Py：生成器表达式
来源：http://mbx.yvedp.cn

(x * 2 for x in arr)
来源：http://hia.xuetiantiany.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oeo.ehwqpu.com

Counter(arr).most_common(3)
来源：http://gcm.zhengqikj.top

[U13] Py：固定长度队列
来源：http://qkw.pengpengdd.cyou

deque(maxlen=10)
来源：http://xfv.fzhhl.top

[U14] Py：分组收集到列表
来源：http://eny.zhongyouzk.top

defaultdict(list)
来源：http://sce.nanxuanxn.top

[U15] Py：高精度计时
来源：http://xnh.guannengcc.top

t = time.perf_counter()
来源：http://nul.zhixingplan.top

[U16] Py：命令行参数解析
来源：http://tbn.zycfv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://crg.wangdashe.top

[U17] Py：初始化日志
来源：http://odg.kuanghao11.cn

logging.basicConfig(level=logging.INFO)
来源：http://mrq.vehdjk.com

[U18] Py：预编译正则
来源：http://ecq.hongshengwenyu.top

pat = re.compile(r"\d+")
来源：http://oep.ppjwa.cn

[U19] Py：正则替换带回调
来源：http://cwy.yj202588.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kcr.cdnleiting.top

[U20] Py：缓存函数结果
来源：http://hvk.dashuyun.cn

@functools.lru_cache(maxsize=None)
来源：http://qww.fehbvm.com

[U21] Py：自定义上下文管理器
来源：http://feh.xuetiantiany.cn

@contextlib.contextmanager
来源：http://asw.chenzaomai.com

[U22] Py：矩阵转置
来源：http://xuh.meibo888.top

list(zip(*m))
来源：http://hod.shangyingyoupin.top

[U23] Py：分块读取大文件
来源：http://fqv.xuetiantiany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hhg.birdmap.top

[U24] Py：路径操作
来源：http://hcr.cqqwz.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lzn.sufxvd.cn

[U25] Py：CSV 按字典读
来源：http://hwh.shzxlz.cn

csv.DictReader(f)
来源：http://mvi.shzxlz.cn

[U26] Py：并发下载
来源：http://zve.316326.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ofc.tian-w.cn

[U27] Py：异步 HTTP
来源：http://jbe.ivvv.top

aiohttp.ClientSession() 配合 async with
来源：http://ixq.yonumen.top

[U28] Py：类型别名
来源：http://tgj.andypj.xyz

UserId = int
来源：http://esr.jqgfzy.top

[U29] Py：属性校验
来源：http://hwl.ctjpmb.com

@property 与 @x.setter 配合
来源：http://pgu.shangyingyoupin.top

[U30] Py：数据类
来源：http://mps.wangshuangyany.cn

@dataclass(slots=True)
来源：http://cwv.9152youxi.cn

[U31] Py：单测
来源：http://pkn.pengpengdd.cyou

python -m pytest -q
来源：http://gxg.epnwcf.com

[U32] Py：代码格式化
来源：http://yxh.hywenlv.cn

ruff format . && ruff check --fix .
来源：http://csi.52xcode.cn

[U33] Py：打包发布
来源：http://awe.ivvv.top

python -m build  （依赖 pyproject.toml）
来源：http://uvq.ywan-chungtsiang.top

[U34] Py：判断编码
来源：http://ubf.nanxinkj.top

chardet.detect(raw)
来源：http://jqs.yfazqb.com

[U35] Py：发送邮件
来源：http://zps.redwolf501.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eay.shanyushiyangkeji.top

[U36] Py：定时任务
来源：http://ufk.yueranfly.top

schedule.every(10).minutes.do(job)
来源：http://ghs.yj20258888.top

[U37] Py：读写 Excel
来源：http://vzc.shangyingyoupin.top

pandas.read_excel / DataFrame.to_excel
来源：http://xne.xinyue.icu

[U38] Py：获取脚本所在目录
来源：http://wln.ydzc1.top

Path(__file__).resolve().parent
来源：http://ncp.ybcxt.top

[U39] Py：判断是否在交互环境
来源：http://elx.yvedp.cn

sys.stdout.isatty()
来源：http://rpc.hammf.cn

[U40] Py：打印到标准错误
来源：http://vzr.shuidangran.top

print("err", file=sys.stderr)
来源：http://gtn.shuidangran.top

[U41] PHP：初始化 Composer 项目
来源：http://qli.guowangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://omz.shanyushiyangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://gkw.xylfe.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nmu.316326.xyz

[U43] PHP：声明命名空间
来源：http://yyq.zycfv.cn

namespace App\Http;
来源：http://okn.snrcjt.cn

[U44] PHP：开启严格类型
来源：http://fcj.svipenyu.cn

declare(strict_types=1);
来源：http://sqe.redwolf501.top

[U45] PHP：类型声明与返回类型
来源：http://llq.fanxiaobao.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://rww.wangdashe.top

[U46] PHP：可空类型
来源：http://tgs.hysaishi.cn

?string $name = null
来源：http://sum.jqgufenzy.top

[U47] PHP：联合类型
来源：http://wcw.wangdashe.top

int|string $id
来源：http://cfq.sxryk.cn

[U48] PHP：纯枚举
来源：http://ynr.sjlbkw.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://axc.meibo888.top

[U49] PHP：只读属性
来源：http://kbk.shuidangran.top

public readonly string $name
来源：http://xwq.fengsongda.top

[U50] PHP：构造器属性提升
来源：http://emh.ctjpmb.com

public function __construct(private int $id) {}
来源：http://oxj.yangfankeji.com

[U51] PHP：数组解构
来源：http://mol.sjlbkw.cn

[$a, $b] = $arr;
来源：http://lul.jinqigufen.top

[U52] PHP：箭头函数
来源：http://djy.gogol.net.cn

$double = fn($x) => $x * 2;
来源：http://iqs.zhoulong.xyz

[U53] PHP：空合并运算符
来源：http://yml.uphjek.com

$v = $a ?? $b ?? "default";
来源：http://lwa.shanyushiyangkeji.top

[U54] PHP：空安全调用
来源：http://uyz.jqgufenzy.top

$obj?->method()
来源：http://ptk.yvedp.cn

[U55] PHP：match 表达式
来源：http://emz.svipenyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vde.shangyingyoupin.top

[U56] PHP：命名参数
来源：http://irj.gzhubu.top

f(a: 1, b: 2)
来源：http://wmo.jianghu66.top

[U57] PHP：字符串插值
来源：http://crh.jianghu66.top

"值: {$a}"
来源：http://ksh.nanxuanxn.top

[U58] PHP：数组三件套
来源：http://orp.shuidangran.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://frd.sufxvd.cn

[U59] PHP：自定义排序
来源：http://sut.hesvh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hqh.zdbjq.cn

[U60] PHP：JSON 编解码
来源：http://ruk.yueranfly.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://frc.chenzaomai.com

[U61] PHP：正则
来源：http://jnk.fzhhl.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yry.sweek.top

[U62] PHP：日期对象
来源：http://dpd.gaohongyu789.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://shk.zhijiandao.cn

[U63] PHP：文件读写
来源：http://hui.shanyushiyangtech.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zta.jqgufenzy.top

[U64] PHP：目录遍历
来源：http://uvz.chenlongwang.top

glob("dir/*.php");  scandir("dir");
来源：http://hpn.yj20258.top

[U65] PHP：会话
来源：http://ftb.c1oappe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://mwo.hnqzz.top

[U66] PHP：设置 Cookie
来源：http://ohx.epnwcf.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dtj.chenjidiqi.icu


<!-- 参考信息 -->