代发 wailian999

[S43] C++：智能指针
来源：http://isn.hysaishi.cn

auto p = std::make_unique<int>(5);
来源：http://fzo.iojbl.cn

[S44] C++：引用传参
来源：http://lht.vqdsnc.cn

void inc(int &x) { ++x; }
来源：http://rlh.hysaishi.cn

[S45] C++：lambda
来源：http://cig.cheryme.top

auto add = [](int a, int b) { return a + b; };
来源：http://tvr.dianchejie.cn

[S46] C++：函数模板
来源：http://jjv.gzhubu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eic.hcnkem.com

[S47] C++：结构化绑定遍历
来源：http://wkv.xuetiantiany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ijp.wangshuangyany.cn

[S48] C++：逐行读文件
来源：http://vkv.xziqi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pcv.pycfn.com

while (std::getline(in, line)) { }
来源：http://wfx.hnxiangtu.top

[S49] C++：写文件
来源：http://wti.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nmi.cashguo.top

[S50] C++：格式化数字
来源：http://acj.shzxlz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lna.shanyushiyangtech.top

[S51] C++：显式类型转换
来源：http://nbv.sxryk.cn

static_cast<double>(a) / b
来源：http://dum.hesvh.cn

[S52] C++：const 与 noexcept
来源：http://ctp.ybcxt.top

int size() const noexcept { return n_; }
来源：http://iny.ppjwa.cn

[S53] C++：移动语义
来源：http://ila.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://xxb.zdqjudy.top

[S54] C++：异常处理
来源：http://avr.yonumen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tsf.xingfuxueyuan.xyz

[S55] C++：结构化绑定
来源：http://pdz.vqdsnc.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fnv.yangfankeji.com

[S56] C++：optional
来源：http://tue.aibaodan.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qlq.xziqi.cn

[S57] C++：编译期常量
来源：http://hhb.aizwys.cn

constexpr int N = 10;
来源：http://rix.hammf.cn

[S58] C++：命名空间
来源：http://cob.yongpay.top

namespace ns { int f() { return 1; } }
来源：http://keu.yanxiufei.cn

[S59] C++：静态断言
来源：http://rfp.haohaochexian.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cdg.pengpengdd.cyou

[S60] C++：遍历并删除元素
来源：http://hxg.guowangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hsm.hywenlv.cn

================================================================================
来源：http://apu.zhijiandao.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yqt.ydjk.org.cn

================================================================================
来源：http://qfp.nwbrower.top

[T01] Kotlin：Hello World
来源：http://jut.ydjk.org.cn

println("Hello")
来源：http://vuj.zhixingplan.top

[T02] Kotlin：变量
来源：http://mvh.jinqigfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://guz.sysykeji.top

[T03] Kotlin：字符串模板
来源：http://qhw.hesvh.cn

"值: $b"
来源：http://nil.chenzaomai.com

[T04] Kotlin：空安全
来源：http://qfi.chenzaomai.com

val n: String? = null;  n?.length
来源：http://nmw.sjlbkw.cn

[T05] Kotlin：when 表达式
来源：http://ove.fktsv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kpl.shuidangran.top

[T06] Kotlin：集合映射
来源：http://jgt.tianlin.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://ldt.ctjpmb.com

[T07] Kotlin：集合过滤
来源：http://bvr.jiagoushi.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mqs.yj20258.top

[T08] Kotlin：数据类
来源：http://gge.xylfe.cn

data class User(val name: String, val age: Int)
来源：http://cud.quarkkingdee.top

[T09] Kotlin：扩展函数
来源：http://sqm.cqqwz.cn

fun String.exclaim() = this + "!"
来源：http://kfl.redwolf501.top

[T10] Kotlin：默认参数
来源：http://qoo.xinyue.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://aiz.mhx1999.top

[T11] Kotlin：协程
来源：http://dks.gaohongyu789.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jmf.vqdsnc.cn

[T12] Kotlin：解构声明
来源：http://qjf.ywan-chungtsiang.top

val (a, b) = Pair(1, 2)
来源：http://yoc.jlsjyb.cn

[T13] Kotlin：只读 Map
来源：http://aaa.chenjidiqi.icu

val m = mapOf("a" to 1)
来源：http://nhq.sufxvd.cn

[T14] Kotlin：循环
来源：http://bjf.vqdsnc.cn

for (i in 1..10) println(i)
来源：http://urc.guannengcc.top

[T15] Kotlin：接口
来源：http://slp.yj20258888.top

interface Shape { fun area(): Double }
来源：http://nfw.gaohongyu789.top

[T16] Swift：Hello World
来源：http://irc.zhaomingkeji.xyz

print("Hello")
来源：http://juu.gogol.net.cn

[T17] Swift：变量与常量
来源：http://mfo.tanke756.top

var a = 1;  let b = 2
来源：http://wfi.sweek.top

[T18] Swift：字符串插值
来源：http://pkg.ehwqpu.com

"值: \(b)"
来源：http://hlp.yongpay.top

[T19] Swift：可选绑定
来源：http://lyu.sjlbkw.cn

if let n = opt { print(n) }
来源：http://vjl.svipenyu.cn

[T20] Swift：数组操作
来源：http://ylm.jiagoushi.top

var a = [1, 2, 3];  a.append(4)
来源：http://qny.wangdashe.top

[T21] Swift：遍历
来源：http://liv.cdnleiting.top

for x in a { print(x) }
来源：http://rfs.guannengcc.top

[T22] Swift：字典
来源：http://xbd.shuidangran.top

var d = ["a": 1];  d["b"] = 2
来源：http://mib.uphjek.com

[T23] Swift：函数
来源：http://ich.yuanzhike.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gta.tarul.cn

[T24] Swift：闭包
来源：http://jdz.jqgfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lsg.hywenlv.cn

[T25] Swift：结构体
来源：http://fxg.kuanghao11.cn

struct P { var x: Int }
来源：http://mym.yvedp.cn

[T26] Swift：类与重写
来源：http://jjv.gzhubu.top

class A: Base { override func f() {} }
来源：http://ioq.aibaodan.cn

[T27] Swift：错误处理
来源：http://oxn.shangyingyoupin.top

do { try f() } catch { print(error) }
来源：http://phy.jyoumei.cn

[T28] Swift：枚举
来源：http://irn.ivvv.top

enum Color { case red, green }
来源：http://upa.yangfankeji.com

[T29] Swift：guard 提前返回
来源：http://xqd.yuanzhike.top

guard let x = opt else { return }
来源：http://dia.xziqi.cn

[T30] Swift：协议
来源：http://hru.hywenlv.cn

protocol Shape { func area() -> Double }
来源：http://iyq.vehdjk.com

[T31] Lua：Hello World
来源：http://cim.cdnleiting.top

print("Hello")
来源：http://sga.sxryk.cn

[T32] Lua：局部变量
来源：http://gyp.zhaomingkeji.xyz

local a = 1
来源：http://joq.xuetiantiany.cn

[T33] Lua：表（数组）
来源：http://yxp.pengpengdd.cyou

local t = {1, 2, 3};  t[4] = 4
来源：http://pjy.daria6918.cn

[T34] Lua：遍历表
来源：http://wjx.jinqigufen.top

for i, v in ipairs(t) do print(i, v) end
来源：http://vjx.yj20258.top

[T35] Lua：字典表
来源：http://hpo.jqgufenzy.top

local d = { a = 1 };  d.b = 2
来源：http://det.shanyushiyangkeji.top

[T36] Lua：函数
来源：http://yvf.316326.xyz

function add(a, b) return a + b end
来源：http://agz.gzhubu.top

[T37] Lua：字符串拼接
来源：http://njg.wangdashe.top

"a" .. "b"
来源：http://uii.havefunace.top

[T38] Lua：条件
来源：http://cqn.zhengqikj.top

if x > 0 then print("正") end
来源：http://kna.zhongyouzk.top

[T39] Lua：模式匹配
来源：http://slu.cqqwz.cn

string.find(s, "%d+")
来源：http://eoi.ehwqpu.com

[T40] Lua：元表
来源：http://bge.hfpthk.cn

setmetatable({}, { __index = base })
来源：http://nuq.jinqigufen.top

[T41] Perl：Hello World
来源：http://kil.gzhubu.top

print "Hello\n";
来源：http://kbn.guannengcc.top

[T42] Perl：变量类型
来源：http://sjz.jinqigfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mop.quarkkingdee.top

[T43] Perl：字符串插值
来源：http://ksd.zhaomingkeji.xyz

"值: $a"
来源：http://ejs.yangfankeji.com

[T44] Perl：条件
来源：http://mbk.dianchejie.cn

if ($a > 0) { print "正"; }
来源：http://mwr.ybcxt.top

[T45] Perl：数组遍历
来源：http://pii.ywan-chungtsiang.top

for my $x (@arr) { print $x; }
来源：http://avn.chenzaomai.com

[T46] Perl：哈希操作
来源：http://stj.shanyushiyangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rcv.hongshengwenyu.top

[T47] Perl：正则捕获
来源：http://vzx.xuetiantiany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wlm.zdqjudy.top

[T48] Perl：正则替换
来源：http://ilz.aizwys.cn

$s =~ s/old/new/g;
来源：http://lwb.bjfxy.top

[T49] Perl：函数
来源：http://nuz.sufxvd.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cas.havefunace.top

[T50] Perl：逐行读文件
来源：http://euz.yvedp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://odk.shanyushiyangtech.top

while (my $line = <$fh>) { print $line; }
来源：http://nnp.cqqwz.cn

[T51] Scala：Hello World
来源：http://krv.fktsv.cn

println("Hello")
来源：http://bdh.fktsv.cn

[T52] Scala：变量
来源：http://lqi.zhiwuduotai.top

val a = 1;  var b = 2
来源：http://wzi.vqdsnc.cn

[T53] Scala：字符串插值
来源：http://vbs.iojbl.cn

s"值: $b"
来源：http://apd.ydzc1.top

[T54] Scala：集合映射
来源：http://zaq.epnwcf.com

List(1, 2, 3).map(_ * 2)
来源：http://tto.zhoulong.xyz

[T55] Scala：集合过滤
来源：http://wll.zhaomingkeji.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://lzl.jyoumei.cn

[T56] Scala：样例类
来源：http://xsr.sysykeji.top

case class User(name: String, age: Int)
来源：http://gkr.quarkkingdee.top

[T57] Scala：模式匹配
来源：http://ckj.yueranfly.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://llm.hnxiangtu.top

[T58] Scala：函数定义
来源：http://smy.dashuyun.cn

def add(a: Int, b: Int): Int = a + b
来源：http://swk.redwolf501.top

[T59] Scala：循环
来源：http://iip.iojbl.cn

for (i <- 1 to 10) println(i)
来源：http://cjv.zhijiandao.cn

[T60] Scala：折叠
来源：http://val.fanxiaobao.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rla.shzxlz.cn

================================================================================
来源：http://gbm.0kj1m.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lvd.birdmap.top

================================================================================
来源：http://bll.vehdjk.com

[U01] Py：创建虚拟环境
来源：http://lps.epnwcf.com

python -m venv .venv && source .venv/bin/activate
来源：http://hou.vehdjk.com

[U02] Py：导出 / 安装依赖
来源：http://rgj.quarkkingdee.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ghl.chenlongwang.top

[U03] Py：加载 .env 配置
来源：http://rkz.tarul.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hsm.svipenyu.cn

[U04] Py：变量调试打印
来源：http://bkj.hongshengwenyu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ftd.yanxiufei.cn

[U05] Py：列表去重且保序
来源：http://otq.yj202588.top

list(dict.fromkeys(arr))
来源：http://zqd.cucudq.cn

[U06] Py：合并两个字典
来源：http://hbz.gaohongyu789.top

{**a, **b}
来源：http://fnc.fktsv.cn

[U07] Py：反转字典键值
来源：http://hxm.cheryme.top

{v: k for k, v in d.items()}
来源：http://ocd.chenzaomai.com

[U08] Py：展平二维列表
来源：http://gcr.tian-w.cn

[y for x in nested for y in x]
来源：http://qvi.chenzaomai.com

[U09] Py：字典取最大值的键
来源：http://grf.epnwcf.com

max(d, key=d.get)
来源：http://knn.dashuyun.cn

[U10] Py：按值排序字典
来源：http://dao.aizwys.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://grk.ivvv.top

[U11] Py：生成器表达式
来源：http://nvm.sxryk.cn

(x * 2 for x in arr)
来源：http://pjm.guannengcc.top

[U12] Py：取出现最多的 3 个元素
来源：http://tii.0kj1m.cn

Counter(arr).most_common(3)
来源：http://cic.cheryme.top

[U13] Py：固定长度队列
来源：http://oaq.xuanzx.com

deque(maxlen=10)
来源：http://uid.sxryk.cn

[U14] Py：分组收集到列表
来源：http://llq.jinghuilouyu.cn

defaultdict(list)
来源：http://mfz.sjlbkw.cn

[U15] Py：高精度计时
来源：http://qjb.fehbvm.com

t = time.perf_counter()
来源：http://cdk.zhoulong.xyz

[U16] Py：命令行参数解析
来源：http://lxc.zhaomingkeji.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ntw.cucudq.cn

[U17] Py：初始化日志
来源：http://gvo.shuidangran.top

logging.basicConfig(level=logging.INFO)
来源：http://jhf.xziqi.cn

[U18] Py：预编译正则
来源：http://qcl.nanxuanxn.top

pat = re.compile(r"\d+")
来源：http://vno.yj202588.top

[U19] Py：正则替换带回调
来源：http://axu.gogol.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pol.xylfe.cn

[U20] Py：缓存函数结果
来源：http://ghy.yueranfly.top

@functools.lru_cache(maxsize=None)
来源：http://beb.bjfxy.top

[U21] Py：自定义上下文管理器
来源：http://lzn.hammf.cn

@contextlib.contextmanager
来源：http://vde.sxryk.cn

[U22] Py：矩阵转置
来源：http://eak.yj20258.top

list(zip(*m))
来源：http://flo.chenzaomai.com

[U23] Py：分块读取大文件
来源：http://rse.ydzc1.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uff.tian-w.cn

[U24] Py：路径操作
来源：http://wjs.52xcode.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hxm.svipenyu.cn

[U25] Py：CSV 按字典读
来源：http://hms.gaohongyu789.top

csv.DictReader(f)
来源：http://wca.quarkkingdee.top

[U26] Py：并发下载
来源：http://abk.cqqwz.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://apn.jinyuanbaomall.cn

[U27] Py：异步 HTTP
来源：http://knh.zhixingplan.top

aiohttp.ClientSession() 配合 async with
来源：http://rdc.c1oappe.top

[U28] Py：类型别名
来源：http://hpg.nanxinkj.top

UserId = int
来源：http://azj.hywenlv.cn

[U29] Py：属性校验
来源：http://ypi.dianchejie.cn

@property 与 @x.setter 配合
来源：http://opg.xinyue.icu

[U30] Py：数据类
来源：http://edl.fanxiaobao.xyz

@dataclass(slots=True)
来源：http://lpz.quarkkingdee.top

[U31] Py：单测
来源：http://dlq.jinqigfzy.top

python -m pytest -q
来源：http://ult.nwbrower.top

[U32] Py：代码格式化
来源：http://ngy.fanxiaobao.xyz

ruff format . && ruff check --fix .
来源：http://icl.fengsongda.top

[U33] Py：打包发布
来源：http://drp.jinqigfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://euw.vehdjk.com

[U34] Py：判断编码
来源：http://fsl.daxiang520.top

chardet.detect(raw)
来源：http://jwi.gogol.net.cn

[U35] Py：发送邮件
来源：http://xwo.epnwcf.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zjv.mhx1999.top

[U36] Py：定时任务
来源：http://wax.shanyushiyangkeji.top

schedule.every(10).minutes.do(job)
来源：http://gpr.bbcook.cn

[U37] Py：读写 Excel
来源：http://exk.zhongyouzk.top

pandas.read_excel / DataFrame.to_excel
来源：http://fif.jyoumei.cn

[U38] Py：获取脚本所在目录
来源：http://ykc.ctjpmb.com

Path(__file__).resolve().parent
来源：http://ius.316326.xyz

[U39] Py：判断是否在交互环境
来源：http://wdw.9152youxi.cn

sys.stdout.isatty()
来源：http://qbn.aizwys.cn

[U40] Py：打印到标准错误
来源：http://jbd.hnqzz.top

print("err", file=sys.stderr)
来源：http://rqp.hywenlv.cn

[U41] PHP：初始化 Composer 项目
来源：http://qhc.aizwys.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dar.jinghuilouyu.cn

[U42] PHP：PSR-4 自动加载
来源：http://wsp.yfazqb.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rva.nanxuanxn.top

[U43] PHP：声明命名空间
来源：http://ipn.hnxiangtu.top

namespace App\Http;
来源：http://hhh.shanyushiyangtech.top

[U44] PHP：开启严格类型
来源：http://qwd.daxiang520.top

declare(strict_types=1);
来源：http://rlq.fehbvm.com

[U45] PHP：类型声明与返回类型
来源：http://fpv.jlsjyb.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mnh.jlsjyb.cn

[U46] PHP：可空类型
来源：http://rtw.smart0.xyz

?string $name = null
来源：http://tml.cheryme.top

[U47] PHP：联合类型
来源：http://wbi.jinyuanbaomall.cn

int|string $id
来源：http://grw.c1oappe.top

[U48] PHP：纯枚举
来源：http://xwo.yongpay.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dlr.havefunace.top

[U49] PHP：只读属性
来源：http://ioq.sjlbkw.cn

public readonly string $name
来源：http://iar.kuanghao11.cn

[U50] PHP：构造器属性提升
来源：http://bdf.hfpthk.cn

public function __construct(private int $id) {}
来源：http://xen.zhengqikj.top

[U51] PHP：数组解构
来源：http://bhz.sjlbkw.cn

[$a, $b] = $arr;
来源：http://bib.xuanzx.com

[U52] PHP：箭头函数
来源：http://bnv.ybcxt.top

$double = fn($x) => $x * 2;
来源：http://mxv.gogol.net.cn

[U53] PHP：空合并运算符
来源：http://eec.aibaodan.cn

$v = $a ?? $b ?? "default";
来源：http://ebu.sweek.top

[U54] PHP：空安全调用
来源：http://ftv.shuidangran.top

$obj?->method()
来源：http://ykg.hammf.cn

[U55] PHP：match 表达式
来源：http://lme.snrcjt.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gzv.dianchejie.cn

[U56] PHP：命名参数
来源：http://smg.ivvv.top

f(a: 1, b: 2)
来源：http://rtb.yfazqb.com

[U57] PHP：字符串插值
来源：http://atr.hfpthk.cn

"值: {$a}"
来源：http://uqq.nwbrower.top

[U58] PHP：数组三件套
来源：http://shf.smart0.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gui.daria6918.cn

[U59] PHP：自定义排序
来源：http://sir.cucudq.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zld.zdqjudy.top

[U60] PHP：JSON 编解码
来源：http://zni.dashuyun.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bjo.yfazqb.com

[U61] PHP：正则
来源：http://cgy.hammf.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cle.pengpengdd.cyou

[U62] PHP：日期对象
来源：http://chn.yuanzhike.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yfb.zhoulong.xyz

[U63] PHP：文件读写
来源：http://hsx.feifeiyinyue.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jov.aizwys.cn

[U64] PHP：目录遍历
来源：http://lvv.fanxiaobao.xyz

glob("dir/*.php");  scandir("dir");
来源：http://myp.pengpengdd.cyou

[U65] PHP：会话
来源：http://dpb.zhengqikj.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vmo.meibo888.top

[U66] PHP：设置 Cookie
来源：http://mkq.fktsv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qmg.chenlongwang.top

[U67] PHP：处理文件上传
来源：http://jnv.zhijiandao.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mjr.quarkkingdee.top

[U68] PHP：PDO 连接
来源：http://doz.jinqigufen.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xvh.uphjek.com


<!-- 参考信息 -->