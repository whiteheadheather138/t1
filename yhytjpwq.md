代发 wailian999

[S43] C++：智能指针
来源：http://fql.nanxuanxn.top

auto p = std::make_unique<int>(5);
来源：http://djk.jyoumei.cn

[S44] C++：引用传参
来源：http://nsk.andypj.xyz

void inc(int &x) { ++x; }
来源：http://znr.aibaodan.cn

[S45] C++：lambda
来源：http://whm.zhijiandao.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dax.gotoacloud.top

[S46] C++：函数模板
来源：http://pbr.ctjpmb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wuv.chenzaomai.com

[S47] C++：结构化绑定遍历
来源：http://lnv.hnxiangtu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wdd.zhaomingkeji.xyz

[S48] C++：逐行读文件
来源：http://tla.dianchejie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hau.svipenyu.cn

while (std::getline(in, line)) { }
来源：http://xwc.meibo888.top

[S49] C++：写文件
来源：http://qem.ydzc1.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://shv.daxiang520.top

[S50] C++：格式化数字
来源：http://qkv.jinghuilouyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mxt.316326.xyz

[S51] C++：显式类型转换
来源：http://sey.fzhhl.top

static_cast<double>(a) / b
来源：http://rqk.zhaomingkeji.xyz

[S52] C++：const 与 noexcept
来源：http://adh.zhaomingkeji.xyz

int size() const noexcept { return n_; }
来源：http://udq.xziqi.cn

[S53] C++：移动语义
来源：http://lcj.iojbl.cn

std::vector<int> w = std::move(v);
来源：http://wlc.chenzaomai.com

[S54] C++：异常处理
来源：http://rqe.yuanzhike.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ntm.zhiwuduotai.top

[S55] C++：结构化绑定
来源：http://agp.pycfn.com

auto [a, b] = std::make_pair(1, 2);
来源：http://iux.epnwcf.com

[S56] C++：optional
来源：http://qxf.jianghu66.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mwa.jqgufenzy.top

[S57] C++：编译期常量
来源：http://dbl.jinqigfzy.top

constexpr int N = 10;
来源：http://lti.shangyingyoupin.top

[S58] C++：命名空间
来源：http://jii.9152youxi.cn

namespace ns { int f() { return 1; } }
来源：http://dug.fehbvm.com

[S59] C++：静态断言
来源：http://avr.chenzaomai.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qoy.guowangkeji.top

[S60] C++：遍历并删除元素
来源：http://mhf.daxiang520.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kfd.hywenlv.cn

================================================================================
来源：http://pxw.xuetiantiany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bxr.zdqjudy.top

================================================================================
来源：http://fqs.chenjidiqi.icu

[T01] Kotlin：Hello World
来源：http://zmr.vqdsnc.cn

println("Hello")
来源：http://qen.jinyuanbaomall.cn

[T02] Kotlin：变量
来源：http://afp.tianlin.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xqx.9152youxi.cn

[T03] Kotlin：字符串模板
来源：http://dmh.ctjpmb.com

"值: $b"
来源：http://fpv.shanyushiyangkeji.top

[T04] Kotlin：空安全
来源：http://fzr.epnwcf.com

val n: String? = null;  n?.length
来源：http://qkg.uphjek.com

[T05] Kotlin：when 表达式
来源：http://ujw.yongpay.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mav.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://czs.hfpthk.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kjm.sufxvd.cn

[T07] Kotlin：集合过滤
来源：http://lvb.zdqjudy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bkz.svipenyu.cn

[T08] Kotlin：数据类
来源：http://lnd.sjlbkw.cn

data class User(val name: String, val age: Int)
来源：http://csk.redwolf501.top

[T09] Kotlin：扩展函数
来源：http://jxu.wangdashe.top

fun String.exclaim() = this + "!"
来源：http://fah.tarul.cn

[T10] Kotlin：默认参数
来源：http://baq.9152youxi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cca.zycfv.cn

[T11] Kotlin：协程
来源：http://pfm.shangyingyoupin.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://pyz.ydjk.org.cn

[T12] Kotlin：解构声明
来源：http://bhs.nanxuanxn.top

val (a, b) = Pair(1, 2)
来源：http://dfc.smart0.xyz

[T13] Kotlin：只读 Map
来源：http://aip.zhiwuduotai.top

val m = mapOf("a" to 1)
来源：http://nhg.zhiwuduotai.top

[T14] Kotlin：循环
来源：http://ufa.yj202588.top

for (i in 1..10) println(i)
来源：http://vsc.mhx1999.top

[T15] Kotlin：接口
来源：http://jjz.daxiang520.top

interface Shape { fun area(): Double }
来源：http://ycg.sysykeji.top

[T16] Swift：Hello World
来源：http://mcg.gogol.net.cn

print("Hello")
来源：http://lcl.sweek.top

[T17] Swift：变量与常量
来源：http://und.jqgufenzy.top

var a = 1;  let b = 2
来源：http://lbe.cqqwz.cn

[T18] Swift：字符串插值
来源：http://xrk.vqdsnc.cn

"值: \(b)"
来源：http://tme.quarkkingdee.top

[T19] Swift：可选绑定
来源：http://xdl.fengsongda.top

if let n = opt { print(n) }
来源：http://lin.shangyingyoupin.top

[T20] Swift：数组操作
来源：http://vtj.guowangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://jyf.gotoacloud.top

[T21] Swift：遍历
来源：http://bre.cqqwz.cn

for x in a { print(x) }
来源：http://rwk.guowangkeji.top

[T22] Swift：字典
来源：http://mhr.hfpthk.cn

var d = ["a": 1];  d["b"] = 2
来源：http://frl.nanxinkj.top

[T23] Swift：函数
来源：http://ocl.sxryk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gaq.c1oappe.top

[T24] Swift：闭包
来源：http://pbf.hywenlv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ifr.tian-w.cn

[T25] Swift：结构体
来源：http://uxp.ydjk.org.cn

struct P { var x: Int }
来源：http://gid.chenzaomai.com

[T26] Swift：类与重写
来源：http://rdx.jqgufenzy.top

class A: Base { override func f() {} }
来源：http://bph.jqgufenzy.top

[T27] Swift：错误处理
来源：http://zep.xuanzx.com

do { try f() } catch { print(error) }
来源：http://fpa.xylfe.cn

[T28] Swift：枚举
来源：http://nsi.daxiang520.top

enum Color { case red, green }
来源：http://yjx.vqdsnc.cn

[T29] Swift：guard 提前返回
来源：http://vbp.hywenlv.cn

guard let x = opt else { return }
来源：http://lfs.yj20258888.top

[T30] Swift：协议
来源：http://uuz.yj20258.top

protocol Shape { func area() -> Double }
来源：http://kgo.zdqjudy.top

[T31] Lua：Hello World
来源：http://bid.smart0.xyz

print("Hello")
来源：http://xzi.vehdjk.com

[T32] Lua：局部变量
来源：http://crq.fzhhl.top

local a = 1
来源：http://akn.pengpengdd.cyou

[T33] Lua：表（数组）
来源：http://jos.ybcxt.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ltw.wangdashe.top

[T34] Lua：遍历表
来源：http://hgu.cqqwz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ngq.sweek.top

[T35] Lua：字典表
来源：http://ewh.fehbvm.com

local d = { a = 1 };  d.b = 2
来源：http://bnj.gaohongyu789.top

[T36] Lua：函数
来源：http://iqx.nanxinkj.top

function add(a, b) return a + b end
来源：http://uca.yueranfly.top

[T37] Lua：字符串拼接
来源：http://pvg.nwbrower.top

"a" .. "b"
来源：http://pml.haohaochexian.top

[T38] Lua：条件
来源：http://mdi.gaohongyu789.top

if x > 0 then print("正") end
来源：http://uor.birdmap.top

[T39] Lua：模式匹配
来源：http://vxc.9152youxi.cn

string.find(s, "%d+")
来源：http://xuc.vehdjk.com

[T40] Lua：元表
来源：http://jdh.cashguo.top

setmetatable({}, { __index = base })
来源：http://hbe.bbcook.cn

[T41] Perl：Hello World
来源：http://isn.wangshuangyany.cn

print "Hello\n";
来源：http://isq.ctjpmb.com

[T42] Perl：变量类型
来源：http://rgw.smart0.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://grn.hnxiangtu.top

[T43] Perl：字符串插值
来源：http://bvy.zycfv.cn

"值: $a"
来源：http://hqc.yj20258.top

[T44] Perl：条件
来源：http://qvj.yuxming.cn

if ($a > 0) { print "正"; }
来源：http://uze.9152youxi.cn

[T45] Perl：数组遍历
来源：http://enn.kuanghao11.cn

for my $x (@arr) { print $x; }
来源：http://yhc.jinqigfzy.top

[T46] Perl：哈希操作
来源：http://oft.hywenlv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sln.ybcxt.top

[T47] Perl：正则捕获
来源：http://usd.wangdashe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ltw.ywan-chungtsiang.top

[T48] Perl：正则替换
来源：http://tfl.tarul.cn

$s =~ s/old/new/g;
来源：http://dwp.nanxuanxn.top

[T49] Perl：函数
来源：http://brt.jinqigfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ttj.kuanghao11.cn

[T50] Perl：逐行读文件
来源：http://qim.jiagoushi.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qjl.daria6918.cn

while (my $line = <$fh>) { print $line; }
来源：http://jyg.aibaodan.cn

[T51] Scala：Hello World
来源：http://rwa.cashguo.top

println("Hello")
来源：http://lyy.yj20258888.top

[T52] Scala：变量
来源：http://tmd.redwolf501.top

val a = 1;  var b = 2
来源：http://uhc.hongshengwenyu.top

[T53] Scala：字符串插值
来源：http://slp.dianchejie.cn

s"值: $b"
来源：http://wzl.tanke756.top

[T54] Scala：集合映射
来源：http://tmm.yangfankeji.com

List(1, 2, 3).map(_ * 2)
来源：http://khj.xuanzx.com

[T55] Scala：集合过滤
来源：http://ycd.hywenlv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fvy.jinghuilouyu.cn

[T56] Scala：样例类
来源：http://niv.daria6918.cn

case class User(name: String, age: Int)
来源：http://gyg.haohaochexian.top

[T57] Scala：模式匹配
来源：http://vrq.ydzc1.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fix.shzxlz.cn

[T58] Scala：函数定义
来源：http://hrt.shanyushiyangtech.top

def add(a: Int, b: Int): Int = a + b
来源：http://kww.fanxiaobao.xyz

[T59] Scala：循环
来源：http://ayz.cucudq.cn

for (i <- 1 to 10) println(i)
来源：http://pha.chenlongwang.top

[T60] Scala：折叠
来源：http://ybn.hnxiangtu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://onv.kuanghao11.cn

================================================================================
来源：http://ugd.0kj1m.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mnd.haohaochexian.top

================================================================================
来源：http://lvx.zhiwuduotai.top

[U01] Py：创建虚拟环境
来源：http://qsh.pycfn.com

python -m venv .venv && source .venv/bin/activate
来源：http://qej.cqqwz.cn

[U02] Py：导出 / 安装依赖
来源：http://dbd.hfpthk.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qjm.shuidangran.top

[U03] Py：加载 .env 配置
来源：http://cst.tanke756.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jtz.0kj1m.cn

[U04] Py：变量调试打印
来源：http://mbd.jyoumei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://aub.chenjidiqi.icu

[U05] Py：列表去重且保序
来源：http://jmg.yuanzhike.top

list(dict.fromkeys(arr))
来源：http://uyh.xinyue.icu

[U06] Py：合并两个字典
来源：http://oww.cashguo.top

{**a, **b}
来源：http://rov.yangfankeji.com

[U07] Py：反转字典键值
来源：http://tbd.sxryk.cn

{v: k for k, v in d.items()}
来源：http://udu.xingfuxueyuan.xyz

[U08] Py：展平二维列表
来源：http://iqe.gotoacloud.top

[y for x in nested for y in x]
来源：http://alf.cheryme.top

[U09] Py：字典取最大值的键
来源：http://ibg.tianlin.xyz

max(d, key=d.get)
来源：http://czp.meibo888.top

[U10] Py：按值排序字典
来源：http://mmz.haohaochexian.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://icu.aibaodan.cn

[U11] Py：生成器表达式
来源：http://kgu.hesvh.cn

(x * 2 for x in arr)
来源：http://fnh.cheryme.top

[U12] Py：取出现最多的 3 个元素
来源：http://ffx.snrcjt.cn

Counter(arr).most_common(3)
来源：http://jbf.jyoumei.cn

[U13] Py：固定长度队列
来源：http://lia.xuanzx.com

deque(maxlen=10)
来源：http://tir.ybcxt.top

[U14] Py：分组收集到列表
来源：http://jyv.uphjek.com

defaultdict(list)
来源：http://dtl.smart0.xyz

[U15] Py：高精度计时
来源：http://hto.yj202588.top

t = time.perf_counter()
来源：http://pjd.uphjek.com

[U16] Py：命令行参数解析
来源：http://gdz.guowangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qjd.pycfn.com

[U17] Py：初始化日志
来源：http://opy.yonumen.top

logging.basicConfig(level=logging.INFO)
来源：http://yvn.hongshengwenyu.top

[U18] Py：预编译正则
来源：http://kup.xingfuxueyuan.xyz

pat = re.compile(r"\d+")
来源：http://vhx.tanke756.top

[U19] Py：正则替换带回调
来源：http://sys.havefunace.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://abm.sweek.top

[U20] Py：缓存函数结果
来源：http://iwh.cqqwz.cn

@functools.lru_cache(maxsize=None)
来源：http://rek.xziqi.cn

[U21] Py：自定义上下文管理器
来源：http://ghg.ywan-chungtsiang.top

@contextlib.contextmanager
来源：http://xdm.yj202588.top

[U22] Py：矩阵转置
来源：http://aui.pycfn.com

list(zip(*m))
来源：http://cdf.gotoacloud.top

[U23] Py：分块读取大文件
来源：http://ugv.nanxuanxn.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://iea.yuanzhike.top

[U24] Py：路径操作
来源：http://xaf.cdnleiting.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qnf.wangdashe.top

[U25] Py：CSV 按字典读
来源：http://pct.ydjk.org.cn

csv.DictReader(f)
来源：http://gkz.shanyushiyangtech.top

[U26] Py：并发下载
来源：http://dbu.ctjpmb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jeb.aibaodan.cn

[U27] Py：异步 HTTP
来源：http://ohu.xylfe.cn

aiohttp.ClientSession() 配合 async with
来源：http://zev.hammf.cn

[U28] Py：类型别名
来源：http://wou.epnwcf.com

UserId = int
来源：http://wca.ydjk.org.cn

[U29] Py：属性校验
来源：http://mrq.jinqigufen.top

@property 与 @x.setter 配合
来源：http://zex.sweek.top

[U30] Py：数据类
来源：http://tcr.316326.xyz

@dataclass(slots=True)
来源：http://zzm.jinghuilouyu.cn

[U31] Py：单测
来源：http://wsg.zhixingplan.top

python -m pytest -q
来源：http://aiw.wangdashe.top

[U32] Py：代码格式化
来源：http://oyq.cashguo.top

ruff format . && ruff check --fix .
来源：http://kwk.cheryme.top

[U33] Py：打包发布
来源：http://muq.quarkkingdee.top

python -m build  （依赖 pyproject.toml）
来源：http://qtf.hywenlv.cn

[U34] Py：判断编码
来源：http://soc.ywan-chungtsiang.top

chardet.detect(raw)
来源：http://epn.zycfv.cn

[U35] Py：发送邮件
来源：http://kce.ppjwa.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hik.xylfe.cn

[U36] Py：定时任务
来源：http://qsz.shanyushiyangtech.top

schedule.every(10).minutes.do(job)
来源：http://hji.yvedp.cn

[U37] Py：读写 Excel
来源：http://hjr.jlsjyb.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sfq.zhijiandao.cn

[U38] Py：获取脚本所在目录
来源：http://mti.tian-w.cn

Path(__file__).resolve().parent
来源：http://srp.bjfxy.top

[U39] Py：判断是否在交互环境
来源：http://kst.fengsongda.top

sys.stdout.isatty()
来源：http://ejf.shuidangran.top

[U40] Py：打印到标准错误
来源：http://zyw.daria6918.cn

print("err", file=sys.stderr)
来源：http://mup.zdqjudy.top

[U41] PHP：初始化 Composer 项目
来源：http://bth.zhixingplan.top

composer init;  composer require guzzlehttp/guzzle
来源：http://nni.nanxuanxn.top

[U42] PHP：PSR-4 自动加载
来源：http://lsy.zhengqikj.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gyk.gogol.net.cn

[U43] PHP：声明命名空间
来源：http://nmn.jiagoushi.top

namespace App\Http;
来源：http://wzm.fehbvm.com

[U44] PHP：开启严格类型
来源：http://sod.yvedp.cn

declare(strict_types=1);
来源：http://zxd.ywan-chungtsiang.top

[U45] PHP：类型声明与返回类型
来源：http://teg.dianchejie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ama.jinqigufen.top

[U46] PHP：可空类型
来源：http://hpp.meibo888.top

?string $name = null
来源：http://qoj.kuanghao11.cn

[U47] PHP：联合类型
来源：http://woh.jqgfzy.top

int|string $id
来源：http://yex.svipenyu.cn

[U48] PHP：纯枚举
来源：http://drd.sjlbkw.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nlv.cdnleiting.top

[U49] PHP：只读属性
来源：http://hvr.jlsjyb.cn

public readonly string $name
来源：http://rrd.birdmap.top

[U50] PHP：构造器属性提升
来源：http://jlt.feifeiyinyue.top

public function __construct(private int $id) {}
来源：http://uck.hfpthk.cn

[U51] PHP：数组解构
来源：http://hfz.yvedp.cn

[$a, $b] = $arr;
来源：http://ewq.zhixingplan.top

[U52] PHP：箭头函数
来源：http://edt.zhixingplan.top

$double = fn($x) => $x * 2;
来源：http://cni.ybcxt.top

[U53] PHP：空合并运算符
来源：http://gep.316326.xyz

$v = $a ?? $b ?? "default";
来源：http://ith.jianghu66.top

[U54] PHP：空安全调用
来源：http://ojn.yangfankeji.com

$obj?->method()
来源：http://gue.shuidangran.top

[U55] PHP：match 表达式
来源：http://ecg.jinghuilouyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dde.guowangkeji.top

[U56] PHP：命名参数
来源：http://lwa.hnxiangtu.top

f(a: 1, b: 2)
来源：http://xvb.tanke756.top

[U57] PHP：字符串插值
来源：http://xvk.havefunace.top

"值: {$a}"
来源：http://wak.ppjwa.cn

[U58] PHP：数组三件套
来源：http://mhp.gaohongyu789.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zls.jinqigfzy.top

[U59] PHP：自定义排序
来源：http://zzo.meibo888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://olg.zdbjq.cn

[U60] PHP：JSON 编解码
来源：http://nsi.aizwys.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://msx.zdbjq.cn

[U61] PHP：正则
来源：http://dep.kuanghao11.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jay.uphjek.com

[U62] PHP：日期对象
来源：http://ljz.meibo888.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yfp.uphjek.com

[U63] PHP：文件读写
来源：http://wsa.iojbl.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sux.hcnkem.com

[U64] PHP：目录遍历
来源：http://ftx.yuanzhike.top

glob("dir/*.php");  scandir("dir");
来源：http://zou.fehbvm.com

[U65] PHP：会话
来源：http://gij.sweek.top

session_start();  $_SESSION["uid"] = 1;
来源：http://skf.ehwqpu.com

[U66] PHP：设置 Cookie
来源：http://cov.9152youxi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ugv.birdmap.top

[U67] PHP：处理文件上传
来源：http://bqn.iojbl.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fuz.yongpay.top

[U68] PHP：PDO 连接
来源：http://ljz.yanxiufei.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tqt.feifeiyinyue.top


<!-- 参考信息 -->