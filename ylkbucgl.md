代发 wailian999

[S43] C++：智能指针
来源：http://yvr.guannengcc.top

auto p = std::make_unique<int>(5);
来源：http://hnq.0kj1m.cn

[S44] C++：引用传参
来源：http://wxt.pycfn.com

void inc(int &x) { ++x; }
来源：http://ryp.hammf.cn

[S45] C++：lambda
来源：http://lgl.vehdjk.com

auto add = [](int a, int b) { return a + b; };
来源：http://wtt.meibo888.top

[S46] C++：函数模板
来源：http://zra.cheryme.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ito.xinyue.icu

[S47] C++：结构化绑定遍历
来源：http://wnz.zhongyouzk.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hdu.hammf.cn

[S48] C++：逐行读文件
来源：http://ozx.zycfv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qgp.xuetiantiany.cn

while (std::getline(in, line)) { }
来源：http://kqs.yonumen.top

[S49] C++：写文件
来源：http://erk.pengpengdd.cyou

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hxd.tanke756.top

[S50] C++：格式化数字
来源：http://cio.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nnj.sjlbkw.cn

[S51] C++：显式类型转换
来源：http://kts.tianlin.xyz

static_cast<double>(a) / b
来源：http://htj.sjlbkw.cn

[S52] C++：const 与 noexcept
来源：http://gdd.zdqjudy.top

int size() const noexcept { return n_; }
来源：http://zxz.xuanzx.com

[S53] C++：移动语义
来源：http://qyd.sysykeji.top

std::vector<int> w = std::move(v);
来源：http://jtg.jinqigfzy.top

[S54] C++：异常处理
来源：http://nuf.gogol.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uas.vqdsnc.cn

[S55] C++：结构化绑定
来源：http://ons.fktsv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://elh.snrcjt.cn

[S56] C++：optional
来源：http://rpw.epnwcf.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jme.vehdjk.com

[S57] C++：编译期常量
来源：http://tck.xingfuxueyuan.xyz

constexpr int N = 10;
来源：http://xcr.ivvv.top

[S58] C++：命名空间
来源：http://bys.sxryk.cn

namespace ns { int f() { return 1; } }
来源：http://gpz.hnqzz.top

[S59] C++：静态断言
来源：http://qfu.pycfn.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mpo.sufxvd.cn

[S60] C++：遍历并删除元素
来源：http://skh.nanxinkj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fpe.ywan-chungtsiang.top

================================================================================
来源：http://swd.cucudq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hzq.mhx1999.top

================================================================================
来源：http://ayt.tian-w.cn

[T01] Kotlin：Hello World
来源：http://klq.vqdsnc.cn

println("Hello")
来源：http://eyk.daria6918.cn

[T02] Kotlin：变量
来源：http://ycs.yangfankeji.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hfr.wangdashe.top

[T03] Kotlin：字符串模板
来源：http://irw.jianghu66.top

"值: $b"
来源：http://avj.zhoulong.xyz

[T04] Kotlin：空安全
来源：http://qvt.sjlbkw.cn

val n: String? = null;  n?.length
来源：http://lqg.tianlin.xyz

[T05] Kotlin：when 表达式
来源：http://hgq.hfpthk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bhf.ydzc1.top

[T06] Kotlin：集合映射
来源：http://ivp.dianchejie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dgo.tarul.cn

[T07] Kotlin：集合过滤
来源：http://ebm.ybcxt.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mtg.cqqwz.cn

[T08] Kotlin：数据类
来源：http://evl.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://tgk.hywenlv.cn

[T09] Kotlin：扩展函数
来源：http://xfe.ehwqpu.com

fun String.exclaim() = this + "!"
来源：http://cpj.zdqjudy.top

[T10] Kotlin：默认参数
来源：http://dnb.cucudq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://apo.yj20258.top

[T11] Kotlin：协程
来源：http://mws.snrcjt.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vxf.cdnleiting.top

[T12] Kotlin：解构声明
来源：http://ywe.ehwqpu.com

val (a, b) = Pair(1, 2)
来源：http://fon.yj202588.top

[T13] Kotlin：只读 Map
来源：http://tpl.feifeiyinyue.top

val m = mapOf("a" to 1)
来源：http://gbg.shuidangran.top

[T14] Kotlin：循环
来源：http://tpf.vqdsnc.cn

for (i in 1..10) println(i)
来源：http://qdl.tarul.cn

[T15] Kotlin：接口
来源：http://owh.mhx1999.top

interface Shape { fun area(): Double }
来源：http://pil.xuetiantiany.cn

[T16] Swift：Hello World
来源：http://bdk.jinyuanbaomall.cn

print("Hello")
来源：http://kad.vqdsnc.cn

[T17] Swift：变量与常量
来源：http://ulo.52xcode.cn

var a = 1;  let b = 2
来源：http://jfc.bjfxy.top

[T18] Swift：字符串插值
来源：http://cso.wangdashe.top

"值: \(b)"
来源：http://kdk.ppjwa.cn

[T19] Swift：可选绑定
来源：http://zys.meibo888.top

if let n = opt { print(n) }
来源：http://zbn.sxryk.cn

[T20] Swift：数组操作
来源：http://qed.sweek.top

var a = [1, 2, 3];  a.append(4)
来源：http://gvq.fktsv.cn

[T21] Swift：遍历
来源：http://arj.zdqjudy.top

for x in a { print(x) }
来源：http://naa.gzhubu.top

[T22] Swift：字典
来源：http://iiy.yanxiufei.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sue.nanxuanxn.top

[T23] Swift：函数
来源：http://hxg.xuanzx.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://skz.yongpay.top

[T24] Swift：闭包
来源：http://hfb.fktsv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ncs.redwolf501.top

[T25] Swift：结构体
来源：http://cct.shanyushiyangtech.top

struct P { var x: Int }
来源：http://vnr.xziqi.cn

[T26] Swift：类与重写
来源：http://vgu.havefunace.top

class A: Base { override func f() {} }
来源：http://xax.hysaishi.cn

[T27] Swift：错误处理
来源：http://ixs.quarkkingdee.top

do { try f() } catch { print(error) }
来源：http://tkz.gotoacloud.top

[T28] Swift：枚举
来源：http://tny.cdnleiting.top

enum Color { case red, green }
来源：http://lzw.0kj1m.cn

[T29] Swift：guard 提前返回
来源：http://vjm.svipenyu.cn

guard let x = opt else { return }
来源：http://ams.cheryme.top

[T30] Swift：协议
来源：http://dpv.ybcxt.top

protocol Shape { func area() -> Double }
来源：http://jxz.sxryk.cn

[T31] Lua：Hello World
来源：http://ijh.shanyushiyangtech.top

print("Hello")
来源：http://prc.dashuyun.cn

[T32] Lua：局部变量
来源：http://gpl.yuxming.cn

local a = 1
来源：http://cpw.hammf.cn

[T33] Lua：表（数组）
来源：http://zww.pycfn.com

local t = {1, 2, 3};  t[4] = 4
来源：http://ppt.shuidangran.top

[T34] Lua：遍历表
来源：http://ibp.vehdjk.com

for i, v in ipairs(t) do print(i, v) end
来源：http://ipi.316326.xyz

[T35] Lua：字典表
来源：http://ekp.cqqwz.cn

local d = { a = 1 };  d.b = 2
来源：http://xdw.chenzaomai.com

[T36] Lua：函数
来源：http://eqj.nanxinkj.top

function add(a, b) return a + b end
来源：http://rmh.guannengcc.top

[T37] Lua：字符串拼接
来源：http://jxk.sweek.top

"a" .. "b"
来源：http://nwp.gaohongyu789.top

[T38] Lua：条件
来源：http://blm.yanxiufei.cn

if x > 0 then print("正") end
来源：http://osi.zhixingplan.top

[T39] Lua：模式匹配
来源：http://vne.xuetiantiany.cn

string.find(s, "%d+")
来源：http://ivh.fanxiaobao.xyz

[T40] Lua：元表
来源：http://kbd.hywenlv.cn

setmetatable({}, { __index = base })
来源：http://tuw.ppjwa.cn

[T41] Perl：Hello World
来源：http://ssf.hcnkem.com

print "Hello\n";
来源：http://anu.jinyuanbaomall.cn

[T42] Perl：变量类型
来源：http://zex.cashguo.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://len.xuetiantiany.cn

[T43] Perl：字符串插值
来源：http://zvo.chenjidiqi.icu

"值: $a"
来源：http://rfw.ybcxt.top

[T44] Perl：条件
来源：http://xre.jqgufenzy.top

if ($a > 0) { print "正"; }
来源：http://yxj.pengpengdd.cyou

[T45] Perl：数组遍历
来源：http://hox.jianghu66.top

for my $x (@arr) { print $x; }
来源：http://pql.feifeiyinyue.top

[T46] Perl：哈希操作
来源：http://nil.ywan-chungtsiang.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://byo.cqqwz.cn

[T47] Perl：正则捕获
来源：http://dva.zdbjq.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vmu.xziqi.cn

[T48] Perl：正则替换
来源：http://qit.zdqjudy.top

$s =~ s/old/new/g;
来源：http://brc.hnqzz.top

[T49] Perl：函数
来源：http://cfb.0kj1m.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pde.vehdjk.com

[T50] Perl：逐行读文件
来源：http://hii.tianlin.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://eyn.zhijiandao.cn

while (my $line = <$fh>) { print $line; }
来源：http://zoy.zhijiandao.cn

[T51] Scala：Hello World
来源：http://jiq.bbcook.cn

println("Hello")
来源：http://xwz.andypj.xyz

[T52] Scala：变量
来源：http://owo.cashguo.top

val a = 1;  var b = 2
来源：http://loy.0kj1m.cn

[T53] Scala：字符串插值
来源：http://chb.ehwqpu.com

s"值: $b"
来源：http://myq.jinqigufen.top

[T54] Scala：集合映射
来源：http://lfq.jinqigufen.top

List(1, 2, 3).map(_ * 2)
来源：http://bhl.xylfe.cn

[T55] Scala：集合过滤
来源：http://wfr.fehbvm.com

List(1, 2, 3).filter(_ > 1)
来源：http://lln.jinqigfzy.top

[T56] Scala：样例类
来源：http://gkz.iojbl.cn

case class User(name: String, age: Int)
来源：http://jvr.zhongyouzk.top

[T57] Scala：模式匹配
来源：http://gje.hcnkem.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://lrw.chenlongwang.top

[T58] Scala：函数定义
来源：http://xol.gogol.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zfw.chenzaomai.com

[T59] Scala：循环
来源：http://dmh.zhiwuduotai.top

for (i <- 1 to 10) println(i)
来源：http://wjc.shzxlz.cn

[T60] Scala：折叠
来源：http://cox.zdbjq.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vjz.yfazqb.com

================================================================================
来源：http://qgt.haohaochexian.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tef.aibaodan.cn

================================================================================
来源：http://uiy.jinqigufen.top

[U01] Py：创建虚拟环境
来源：http://ika.guowangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://kav.uphjek.com

[U02] Py：导出 / 安装依赖
来源：http://ifu.0kj1m.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pfa.chenzaomai.com

[U03] Py：加载 .env 配置
来源：http://hgn.chenzaomai.com

from dotenv import load_dotenv; load_dotenv()
来源：http://edm.zhaomingkeji.xyz

[U04] Py：变量调试打印
来源：http://qro.yj20258888.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fyy.jinqigfzy.top

[U05] Py：列表去重且保序
来源：http://cyl.hongshengwenyu.top

list(dict.fromkeys(arr))
来源：http://pyp.yanxiufei.cn

[U06] Py：合并两个字典
来源：http://ciz.sysykeji.top

{**a, **b}
来源：http://qiu.svipenyu.cn

[U07] Py：反转字典键值
来源：http://osz.pycfn.com

{v: k for k, v in d.items()}
来源：http://efj.zhengqikj.top

[U08] Py：展平二维列表
来源：http://uwo.gogol.net.cn

[y for x in nested for y in x]
来源：http://qyh.yuanzhike.top

[U09] Py：字典取最大值的键
来源：http://mpl.52xcode.cn

max(d, key=d.get)
来源：http://rni.iojbl.cn

[U10] Py：按值排序字典
来源：http://mfz.dianchejie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vcg.vehdjk.com

[U11] Py：生成器表达式
来源：http://heq.52xcode.cn

(x * 2 for x in arr)
来源：http://nfz.yuanzhike.top

[U12] Py：取出现最多的 3 个元素
来源：http://dcz.cdnleiting.top

Counter(arr).most_common(3)
来源：http://rqi.yj20258.top

[U13] Py：固定长度队列
来源：http://pmr.zhijiandao.cn

deque(maxlen=10)
来源：http://yvy.gzhubu.top

[U14] Py：分组收集到列表
来源：http://fsk.yanxiufei.cn

defaultdict(list)
来源：http://rzw.cashguo.top

[U15] Py：高精度计时
来源：http://jwu.iojbl.cn

t = time.perf_counter()
来源：http://kom.haohaochexian.top

[U16] Py：命令行参数解析
来源：http://mfo.guowangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ysr.iojbl.cn

[U17] Py：初始化日志
来源：http://evz.cashguo.top

logging.basicConfig(level=logging.INFO)
来源：http://swg.birdmap.top

[U18] Py：预编译正则
来源：http://seq.shanyushiyangkeji.top

pat = re.compile(r"\d+")
来源：http://qbq.redwolf501.top

[U19] Py：正则替换带回调
来源：http://zpn.epnwcf.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xtb.jlsjyb.cn

[U20] Py：缓存函数结果
来源：http://cbp.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://yql.shzxlz.cn

[U21] Py：自定义上下文管理器
来源：http://trc.mhx1999.top

@contextlib.contextmanager
来源：http://mez.andypj.xyz

[U22] Py：矩阵转置
来源：http://fwj.0kj1m.cn

list(zip(*m))
来源：http://mbr.fanxiaobao.xyz

[U23] Py：分块读取大文件
来源：http://wfd.chenlongwang.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xxc.fzhhl.top

[U24] Py：路径操作
来源：http://juc.gaohongyu789.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://plh.iojbl.cn

[U25] Py：CSV 按字典读
来源：http://rzq.shuidangran.top

csv.DictReader(f)
来源：http://euj.hywenlv.cn

[U26] Py：并发下载
来源：http://phf.hywenlv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yno.hywenlv.cn

[U27] Py：异步 HTTP
来源：http://ynb.zycfv.cn

aiohttp.ClientSession() 配合 async with
来源：http://zxy.yanxiufei.cn

[U28] Py：类型别名
来源：http://uvw.daxiang520.top

UserId = int
来源：http://fys.xuanzx.com

[U29] Py：属性校验
来源：http://vcx.zdqjudy.top

@property 与 @x.setter 配合
来源：http://ddw.9152youxi.cn

[U30] Py：数据类
来源：http://ufy.meibo888.top

@dataclass(slots=True)
来源：http://jij.shuidangran.top

[U31] Py：单测
来源：http://xdu.jqgufenzy.top

python -m pytest -q
来源：http://chp.sufxvd.cn

[U32] Py：代码格式化
来源：http://owo.zdqjudy.top

ruff format . && ruff check --fix .
来源：http://vsp.0kj1m.cn

[U33] Py：打包发布
来源：http://hsk.bbcook.cn

python -m build  （依赖 pyproject.toml）
来源：http://oix.hnxiangtu.top

[U34] Py：判断编码
来源：http://qyu.52xcode.cn

chardet.detect(raw)
来源：http://ccl.xziqi.cn

[U35] Py：发送邮件
来源：http://pwo.9152youxi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cih.cucudq.cn

[U36] Py：定时任务
来源：http://ocl.xuetiantiany.cn

schedule.every(10).minutes.do(job)
来源：http://muc.xinyue.icu

[U37] Py：读写 Excel
来源：http://tuq.zhijiandao.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dst.jyoumei.cn

[U38] Py：获取脚本所在目录
来源：http://udv.ydjk.org.cn

Path(__file__).resolve().parent
来源：http://hjf.mhx1999.top

[U39] Py：判断是否在交互环境
来源：http://qud.yueranfly.top

sys.stdout.isatty()
来源：http://vxa.daria6918.cn

[U40] Py：打印到标准错误
来源：http://fvt.zycfv.cn

print("err", file=sys.stderr)
来源：http://wey.yuxming.cn

[U41] PHP：初始化 Composer 项目
来源：http://hnh.yuanzhike.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jvf.fzhhl.top

[U42] PHP：PSR-4 自动加载
来源：http://ggl.smart0.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nxi.yongpay.top

[U43] PHP：声明命名空间
来源：http://ixj.jinqigufen.top

namespace App\Http;
来源：http://ler.daxiang520.top

[U44] PHP：开启严格类型
来源：http://itp.yongpay.top

declare(strict_types=1);
来源：http://pak.vqdsnc.cn

[U45] PHP：类型声明与返回类型
来源：http://ybd.xylfe.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fsg.nwbrower.top

[U46] PHP：可空类型
来源：http://gau.vehdjk.com

?string $name = null
来源：http://srx.vehdjk.com

[U47] PHP：联合类型
来源：http://jwn.hnqzz.top

int|string $id
来源：http://gya.cqqwz.cn

[U48] PHP：纯枚举
来源：http://kht.9152youxi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vwy.52xcode.cn

[U49] PHP：只读属性
来源：http://esa.haohaochexian.top

public readonly string $name
来源：http://ios.jlsjyb.cn

[U50] PHP：构造器属性提升
来源：http://rtg.sweek.top

public function __construct(private int $id) {}
来源：http://kse.jianghu66.top

[U51] PHP：数组解构
来源：http://nii.zhiwuduotai.top

[$a, $b] = $arr;
来源：http://uul.ydzc1.top

[U52] PHP：箭头函数
来源：http://cif.jiagoushi.top

$double = fn($x) => $x * 2;
来源：http://xtj.fzhhl.top

[U53] PHP：空合并运算符
来源：http://unc.xziqi.cn

$v = $a ?? $b ?? "default";
来源：http://xvl.zhaomingkeji.xyz

[U54] PHP：空安全调用
来源：http://pjw.tianlin.xyz

$obj?->method()
来源：http://tab.hnxiangtu.top

[U55] PHP：match 表达式
来源：http://tbm.ppjwa.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kqn.iojbl.cn

[U56] PHP：命名参数
来源：http://tjv.zdbjq.cn

f(a: 1, b: 2)
来源：http://lew.sweek.top

[U57] PHP：字符串插值
来源：http://kat.hywenlv.cn

"值: {$a}"
来源：http://nwv.nanxuanxn.top

[U58] PHP：数组三件套
来源：http://cvy.andypj.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iiq.cheryme.top

[U59] PHP：自定义排序
来源：http://ejt.chenjidiqi.icu

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rxl.gzhubu.top

[U60] PHP：JSON 编解码
来源：http://tkq.tian-w.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mka.hongshengwenyu.top

[U61] PHP：正则
来源：http://vnh.wangdashe.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ezn.pengpengdd.cyou

[U62] PHP：日期对象
来源：http://axi.yj202588.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cyh.nanxuanxn.top

[U63] PHP：文件读写
来源：http://seb.cdnleiting.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kgz.bjfxy.top

[U64] PHP：目录遍历
来源：http://cye.zhiwuduotai.top

glob("dir/*.php");  scandir("dir");
来源：http://ihr.zhiwuduotai.top

[U65] PHP：会话
来源：http://zcb.9152youxi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://axy.bbcook.cn

[U66] PHP：设置 Cookie
来源：http://mnt.uphjek.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jao.gaohongyu789.top

[U67] PHP：处理文件上传
来源：http://eyd.shangyingyoupin.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kob.zhaomingkeji.xyz

[U68] PHP：PDO 连接
来源：http://fcg.yuanzhike.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jnz.tarul.cn


<!-- 参考信息 -->