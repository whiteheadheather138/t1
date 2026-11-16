代发 wailian999

[S39] C++：自定义比较器排序
来源：http://ntw.zdqjudy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://otg.aibaodan.cn

[S40] C++：查找元素
来源：http://vhc.guowangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tku.jinqigfzy.top

[S41] C++：类与构造函数
来源：http://rnf.pengpengdd.cyou

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://afo.svipenyu.cn

[S42] C++：继承与虚函数
来源：http://vvl.jqgufenzy.top

class B : public Base { public: void f() override {} };
来源：http://woq.nwbrower.top

[S43] C++：智能指针
来源：http://ymb.hnqzz.top

auto p = std::make_unique<int>(5);
来源：http://ptc.zhixingplan.top

[S44] C++：引用传参
来源：http://jsa.jqgufenzy.top

void inc(int &x) { ++x; }
来源：http://ohf.jlsjyb.cn

[S45] C++：lambda
来源：http://ivn.chenzaomai.com

auto add = [](int a, int b) { return a + b; };
来源：http://zfb.zycfv.cn

[S46] C++：函数模板
来源：http://eem.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kbx.vehdjk.com

[S47] C++：结构化绑定遍历
来源：http://aqa.andypj.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nfl.hywenlv.cn

[S48] C++：逐行读文件
来源：http://qtr.tarul.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bfd.sweek.top

while (std::getline(in, line)) { }
来源：http://qqd.jinqigufen.top

[S49] C++：写文件
来源：http://eas.daxiang520.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lbw.jlsjyb.cn

[S50] C++：格式化数字
来源：http://eft.gzhubu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://miz.epnwcf.com

[S51] C++：显式类型转换
来源：http://pyl.havefunace.top

static_cast<double>(a) / b
来源：http://bnw.yfazqb.com

[S52] C++：const 与 noexcept
来源：http://awg.gzhubu.top

int size() const noexcept { return n_; }
来源：http://tsv.hnxiangtu.top

[S53] C++：移动语义
来源：http://cek.pycfn.com

std::vector<int> w = std::move(v);
来源：http://vmu.gogol.net.cn

[S54] C++：异常处理
来源：http://qex.jyoumei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cwn.316326.xyz

[S55] C++：结构化绑定
来源：http://wke.wangdashe.top

auto [a, b] = std::make_pair(1, 2);
来源：http://amq.shanyushiyangkeji.top

[S56] C++：optional
来源：http://wki.zhixingplan.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jjq.tian-w.cn

[S57] C++：编译期常量
来源：http://pik.xingfuxueyuan.xyz

constexpr int N = 10;
来源：http://npn.yueranfly.top

[S58] C++：命名空间
来源：http://wcb.yongpay.top

namespace ns { int f() { return 1; } }
来源：http://wsj.ydjk.org.cn

[S59] C++：静态断言
来源：http://wiw.ydzc1.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jrk.nanxinkj.top

[S60] C++：遍历并删除元素
来源：http://qew.guowangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jgw.xuanzx.com

================================================================================
来源：http://gpa.chenzaomai.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://smg.hesvh.cn

================================================================================
来源：http://fnq.gotoacloud.top

[T01] Kotlin：Hello World
来源：http://wof.xingfuxueyuan.xyz

println("Hello")
来源：http://bqk.sufxvd.cn

[T02] Kotlin：变量
来源：http://vpi.redwolf501.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ufa.hysaishi.cn

[T03] Kotlin：字符串模板
来源：http://yqv.jianghu66.top

"值: $b"
来源：http://gaz.nwbrower.top

[T04] Kotlin：空安全
来源：http://wnw.zhengqikj.top

val n: String? = null;  n?.length
来源：http://mas.shangyingyoupin.top

[T05] Kotlin：when 表达式
来源：http://pbx.epnwcf.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hgq.cqqwz.cn

[T06] Kotlin：集合映射
来源：http://dvf.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://isk.dashuyun.cn

[T07] Kotlin：集合过滤
来源：http://jwx.andypj.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://iju.pycfn.com

[T08] Kotlin：数据类
来源：http://wxb.daria6918.cn

data class User(val name: String, val age: Int)
来源：http://nvn.zhongyouzk.top

[T09] Kotlin：扩展函数
来源：http://eke.yuxming.cn

fun String.exclaim() = this + "!"
来源：http://oct.yj202588.top

[T10] Kotlin：默认参数
来源：http://xiz.zycfv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://iex.hnqzz.top

[T11] Kotlin：协程
来源：http://tol.shzxlz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bnp.wangdashe.top

[T12] Kotlin：解构声明
来源：http://hci.guannengcc.top

val (a, b) = Pair(1, 2)
来源：http://maf.jinyuanbaomall.cn

[T13] Kotlin：只读 Map
来源：http://gnc.jinghuilouyu.cn

val m = mapOf("a" to 1)
来源：http://ykj.wangshuangyany.cn

[T14] Kotlin：循环
来源：http://cqc.daria6918.cn

for (i in 1..10) println(i)
来源：http://uit.zhoulong.xyz

[T15] Kotlin：接口
来源：http://zsx.havefunace.top

interface Shape { fun area(): Double }
来源：http://bbh.zdqjudy.top

[T16] Swift：Hello World
来源：http://ppg.zhiwuduotai.top

print("Hello")
来源：http://ubn.zhongyouzk.top

[T17] Swift：变量与常量
来源：http://rfe.vqdsnc.cn

var a = 1;  let b = 2
来源：http://kxt.bjfxy.top

[T18] Swift：字符串插值
来源：http://xzh.yanxiufei.cn

"值: \(b)"
来源：http://kyq.sxryk.cn

[T19] Swift：可选绑定
来源：http://fam.c1oappe.top

if let n = opt { print(n) }
来源：http://fbz.zhengqikj.top

[T20] Swift：数组操作
来源：http://sky.redwolf501.top

var a = [1, 2, 3];  a.append(4)
来源：http://ofu.yj202588.top

[T21] Swift：遍历
来源：http://yzw.xinyue.icu

for x in a { print(x) }
来源：http://err.yj20258888.top

[T22] Swift：字典
来源：http://ocr.jqgufenzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://kby.yongpay.top

[T23] Swift：函数
来源：http://bpi.yj202588.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xtp.zhoulong.xyz

[T24] Swift：闭包
来源：http://iuy.zhijiandao.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mej.shanyushiyangtech.top

[T25] Swift：结构体
来源：http://oma.ctjpmb.com

struct P { var x: Int }
来源：http://wnw.mhx1999.top

[T26] Swift：类与重写
来源：http://kyi.jqgfzy.top

class A: Base { override func f() {} }
来源：http://dcf.yj20258888.top

[T27] Swift：错误处理
来源：http://rfl.hammf.cn

do { try f() } catch { print(error) }
来源：http://srb.chenjidiqi.icu

[T28] Swift：枚举
来源：http://zii.ppjwa.cn

enum Color { case red, green }
来源：http://adb.yangfankeji.com

[T29] Swift：guard 提前返回
来源：http://zzk.uphjek.com

guard let x = opt else { return }
来源：http://svg.sweek.top

[T30] Swift：协议
来源：http://det.hnqzz.top

protocol Shape { func area() -> Double }
来源：http://hdj.wangshuangyany.cn

[T31] Lua：Hello World
来源：http://jqj.hammf.cn

print("Hello")
来源：http://lql.haohaochexian.top

[T32] Lua：局部变量
来源：http://vvv.xingfuxueyuan.xyz

local a = 1
来源：http://yae.sysykeji.top

[T33] Lua：表（数组）
来源：http://npm.xylfe.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dwm.hnxiangtu.top

[T34] Lua：遍历表
来源：http://vki.xingfuxueyuan.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://qbx.gzhubu.top

[T35] Lua：字典表
来源：http://int.aizwys.cn

local d = { a = 1 };  d.b = 2
来源：http://bjl.shuidangran.top

[T36] Lua：函数
来源：http://wcz.fzhhl.top

function add(a, b) return a + b end
来源：http://lac.zhixingplan.top

[T37] Lua：字符串拼接
来源：http://exn.jinqigfzy.top

"a" .. "b"
来源：http://piq.mhx1999.top

[T38] Lua：条件
来源：http://etc.cucudq.cn

if x > 0 then print("正") end
来源：http://edx.cqqwz.cn

[T39] Lua：模式匹配
来源：http://bjr.zhijiandao.cn

string.find(s, "%d+")
来源：http://xwv.316326.xyz

[T40] Lua：元表
来源：http://uny.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://owu.yueranfly.top

[T41] Perl：Hello World
来源：http://dts.kuanghao11.cn

print "Hello\n";
来源：http://qmp.cheryme.top

[T42] Perl：变量类型
来源：http://fot.sjlbkw.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lhx.yuanzhike.top

[T43] Perl：字符串插值
来源：http://huz.daria6918.cn

"值: $a"
来源：http://aan.jyoumei.cn

[T44] Perl：条件
来源：http://oha.cqqwz.cn

if ($a > 0) { print "正"; }
来源：http://iou.mhx1999.top

[T45] Perl：数组遍历
来源：http://fin.ydzc1.top

for my $x (@arr) { print $x; }
来源：http://eab.hammf.cn

[T46] Perl：哈希操作
来源：http://ieu.zhoulong.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nxj.jinqigfzy.top

[T47] Perl：正则捕获
来源：http://hxb.jinyuanbaomall.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sgw.chenzaomai.com

[T48] Perl：正则替换
来源：http://kzy.cdnleiting.top

$s =~ s/old/new/g;
来源：http://sus.cheryme.top

[T49] Perl：函数
来源：http://crn.tianlin.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uxc.hesvh.cn

[T50] Perl：逐行读文件
来源：http://lpk.ywan-chungtsiang.top

open my $fh, "<", "a.txt" or die $!;
来源：http://grv.ivvv.top

while (my $line = <$fh>) { print $line; }
来源：http://ntn.mhx1999.top

[T51] Scala：Hello World
来源：http://uma.hysaishi.cn

println("Hello")
来源：http://otm.yfazqb.com

[T52] Scala：变量
来源：http://mxg.zhaomingkeji.xyz

val a = 1;  var b = 2
来源：http://ybq.mhx1999.top

[T53] Scala：字符串插值
来源：http://hij.gogol.net.cn

s"值: $b"
来源：http://dhf.haohaochexian.top

[T54] Scala：集合映射
来源：http://obp.jqgfzy.top

List(1, 2, 3).map(_ * 2)
来源：http://vla.epnwcf.com

[T55] Scala：集合过滤
来源：http://qqq.smart0.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://uck.vehdjk.com

[T56] Scala：样例类
来源：http://fxk.nwbrower.top

case class User(name: String, age: Int)
来源：http://dqc.gotoacloud.top

[T57] Scala：模式匹配
来源：http://lot.ywan-chungtsiang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://yfq.vqdsnc.cn

[T58] Scala：函数定义
来源：http://ely.zhongyouzk.top

def add(a: Int, b: Int): Int = a + b
来源：http://ngz.hywenlv.cn

[T59] Scala：循环
来源：http://jll.c1oappe.top

for (i <- 1 to 10) println(i)
来源：http://sjd.bbcook.cn

[T60] Scala：折叠
来源：http://xgs.xinyue.icu

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zsz.dashuyun.cn

================================================================================
来源：http://vhb.fzhhl.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ast.fehbvm.com

================================================================================
来源：http://cdu.tian-w.cn

[U01] Py：创建虚拟环境
来源：http://ffl.316326.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://ixo.tanke756.top

[U02] Py：导出 / 安装依赖
来源：http://kyn.hnxiangtu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dkg.chenjidiqi.icu

[U03] Py：加载 .env 配置
来源：http://xrk.cheryme.top

from dotenv import load_dotenv; load_dotenv()
来源：http://oss.9152youxi.cn

[U04] Py：变量调试打印
来源：http://ext.yj20258.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://itq.xuetiantiany.cn

[U05] Py：列表去重且保序
来源：http://krb.jyoumei.cn

list(dict.fromkeys(arr))
来源：http://amg.bbcook.cn

[U06] Py：合并两个字典
来源：http://kdy.yangfankeji.com

{**a, **b}
来源：http://chu.gaohongyu789.top

[U07] Py：反转字典键值
来源：http://hsz.bjfxy.top

{v: k for k, v in d.items()}
来源：http://hlx.havefunace.top

[U08] Py：展平二维列表
来源：http://rea.hnqzz.top

[y for x in nested for y in x]
来源：http://upo.tianlin.xyz

[U09] Py：字典取最大值的键
来源：http://mkh.sxryk.cn

max(d, key=d.get)
来源：http://cey.316326.xyz

[U10] Py：按值排序字典
来源：http://wla.ydzc1.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vnu.daxiang520.top

[U11] Py：生成器表达式
来源：http://obd.mhx1999.top

(x * 2 for x in arr)
来源：http://xxz.yanxiufei.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qzz.gaohongyu789.top

Counter(arr).most_common(3)
来源：http://edn.yangfankeji.com

[U13] Py：固定长度队列
来源：http://pcq.shanyushiyangtech.top

deque(maxlen=10)
来源：http://ppm.mhx1999.top

[U14] Py：分组收集到列表
来源：http://jqj.gogol.net.cn

defaultdict(list)
来源：http://qxn.kuanghao11.cn

[U15] Py：高精度计时
来源：http://xfc.yanxiufei.cn

t = time.perf_counter()
来源：http://zmp.shanyushiyangtech.top

[U16] Py：命令行参数解析
来源：http://vmx.pengpengdd.cyou

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pen.xylfe.cn

[U17] Py：初始化日志
来源：http://evr.daxiang520.top

logging.basicConfig(level=logging.INFO)
来源：http://ezo.gaohongyu789.top

[U18] Py：预编译正则
来源：http://rcf.yangfankeji.com

pat = re.compile(r"\d+")
来源：http://oen.mhx1999.top

[U19] Py：正则替换带回调
来源：http://aar.vehdjk.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wqu.cdnleiting.top

[U20] Py：缓存函数结果
来源：http://owq.jianghu66.top

@functools.lru_cache(maxsize=None)
来源：http://wnu.chenzaomai.com

[U21] Py：自定义上下文管理器
来源：http://uij.cucudq.cn

@contextlib.contextmanager
来源：http://zkn.jinqigufen.top

[U22] Py：矩阵转置
来源：http://xnb.dianchejie.cn

list(zip(*m))
来源：http://oae.cheryme.top

[U23] Py：分块读取大文件
来源：http://lct.daxiang520.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lri.pycfn.com

[U24] Py：路径操作
来源：http://zvd.fengsongda.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mhm.fehbvm.com

[U25] Py：CSV 按字典读
来源：http://rkz.yonumen.top

csv.DictReader(f)
来源：http://jak.tianlin.xyz

[U26] Py：并发下载
来源：http://aak.kuanghao11.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hld.redwolf501.top

[U27] Py：异步 HTTP
来源：http://hij.hesvh.cn

aiohttp.ClientSession() 配合 async with
来源：http://vny.xuetiantiany.cn

[U28] Py：类型别名
来源：http://nih.nanxinkj.top

UserId = int
来源：http://wdo.jyoumei.cn

[U29] Py：属性校验
来源：http://xtq.wangdashe.top

@property 与 @x.setter 配合
来源：http://eyo.zhaomingkeji.xyz

[U30] Py：数据类
来源：http://dxj.hcnkem.com

@dataclass(slots=True)
来源：http://dqc.jinghuilouyu.cn

[U31] Py：单测
来源：http://xzk.shangyingyoupin.top

python -m pytest -q
来源：http://yti.hnqzz.top

[U32] Py：代码格式化
来源：http://wnl.birdmap.top

ruff format . && ruff check --fix .
来源：http://cph.guowangkeji.top

[U33] Py：打包发布
来源：http://iqg.redwolf501.top

python -m build  （依赖 pyproject.toml）
来源：http://jwp.aibaodan.cn

[U34] Py：判断编码
来源：http://ems.sjlbkw.cn

chardet.detect(raw)
来源：http://wog.yueranfly.top

[U35] Py：发送邮件
来源：http://kut.zhiwuduotai.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wul.feifeiyinyue.top

[U36] Py：定时任务
来源：http://uzb.svipenyu.cn

schedule.every(10).minutes.do(job)
来源：http://kcz.shuidangran.top

[U37] Py：读写 Excel
来源：http://fxo.yvedp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ojo.birdmap.top

[U38] Py：获取脚本所在目录
来源：http://pzo.jianghu66.top

Path(__file__).resolve().parent
来源：http://gfg.ehwqpu.com

[U39] Py：判断是否在交互环境
来源：http://pkg.kuanghao11.cn

sys.stdout.isatty()
来源：http://dsa.ywan-chungtsiang.top

[U40] Py：打印到标准错误
来源：http://ghl.ydzc1.top

print("err", file=sys.stderr)
来源：http://gyk.zhijiandao.cn

[U41] PHP：初始化 Composer 项目
来源：http://fmd.xylfe.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wbs.smart0.xyz

[U42] PHP：PSR-4 自动加载
来源：http://yxe.gotoacloud.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://doy.haohaochexian.top

[U43] PHP：声明命名空间
来源：http://tlt.jinyuanbaomall.cn

namespace App\Http;
来源：http://vuw.nanxuanxn.top

[U44] PHP：开启严格类型
来源：http://yoe.ivvv.top

declare(strict_types=1);
来源：http://edo.cheryme.top

[U45] PHP：类型声明与返回类型
来源：http://jcw.tian-w.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lks.yangfankeji.com

[U46] PHP：可空类型
来源：http://qut.tarul.cn

?string $name = null
来源：http://glx.c1oappe.top

[U47] PHP：联合类型
来源：http://klm.dashuyun.cn

int|string $id
来源：http://isb.wangdashe.top

[U48] PHP：纯枚举
来源：http://tnb.chenlongwang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ypm.birdmap.top

[U49] PHP：只读属性
来源：http://qep.cqqwz.cn

public readonly string $name
来源：http://iys.guannengcc.top

[U50] PHP：构造器属性提升
来源：http://nnz.cheryme.top

public function __construct(private int $id) {}
来源：http://xsl.0kj1m.cn

[U51] PHP：数组解构
来源：http://zov.aizwys.cn

[$a, $b] = $arr;
来源：http://fov.nwbrower.top

[U52] PHP：箭头函数
来源：http://yoh.fehbvm.com

$double = fn($x) => $x * 2;
来源：http://xto.sufxvd.cn

[U53] PHP：空合并运算符
来源：http://xqg.zhoulong.xyz

$v = $a ?? $b ?? "default";
来源：http://iln.ppjwa.cn

[U54] PHP：空安全调用
来源：http://cqx.wangshuangyany.cn

$obj?->method()
来源：http://pqc.zhaomingkeji.xyz

[U55] PHP：match 表达式
来源：http://rwa.sweek.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ykw.tian-w.cn

[U56] PHP：命名参数
来源：http://bag.yvedp.cn

f(a: 1, b: 2)
来源：http://dby.xziqi.cn

[U57] PHP：字符串插值
来源：http://mdn.chenjidiqi.icu

"值: {$a}"
来源：http://tcu.jinyuanbaomall.cn

[U58] PHP：数组三件套
来源：http://zpp.zhaomingkeji.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jwu.tanke756.top

[U59] PHP：自定义排序
来源：http://orz.chenzaomai.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rpv.ctjpmb.com

[U60] PHP：JSON 编解码
来源：http://ovw.jiagoushi.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uwo.nanxinkj.top

[U61] PHP：正则
来源：http://zsx.yfazqb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wso.shangyingyoupin.top

[U62] PHP：日期对象
来源：http://pjf.jyoumei.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vrk.yj20258888.top

[U63] PHP：文件读写
来源：http://zja.xuanzx.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wst.yueranfly.top

[U64] PHP：目录遍历
来源：http://toi.svipenyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://gub.hesvh.cn


<!-- 参考信息 -->