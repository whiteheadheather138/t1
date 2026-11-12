代发 wailian999

[S41] C++：类与构造函数
来源：http://rqw.shangyingyoupin.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uli.sxryk.cn

[S42] C++：继承与虚函数
来源：http://wtr.bjfxy.top

class B : public Base { public: void f() override {} };
来源：http://kwx.yanxiufei.cn

[S43] C++：智能指针
来源：http://erq.bjfxy.top

auto p = std::make_unique<int>(5);
来源：http://owt.jinqigufen.top

[S44] C++：引用传参
来源：http://gqz.ppjwa.cn

void inc(int &x) { ++x; }
来源：http://ubk.hysaishi.cn

[S45] C++：lambda
来源：http://lln.meibo888.top

auto add = [](int a, int b) { return a + b; };
来源：http://orn.9152youxi.cn

[S46] C++：函数模板
来源：http://wlj.zhengqikj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yju.redwolf501.top

[S47] C++：结构化绑定遍历
来源：http://zce.hfpthk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gkn.chenjidiqi.icu

[S48] C++：逐行读文件
来源：http://zva.tian-w.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ztp.yuxming.cn

while (std::getline(in, line)) { }
来源：http://mvs.cucudq.cn

[S49] C++：写文件
来源：http://bpi.hammf.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://aia.gzhubu.top

[S50] C++：格式化数字
来源：http://dcs.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rvc.yonumen.top

[S51] C++：显式类型转换
来源：http://bak.nanxuanxn.top

static_cast<double>(a) / b
来源：http://sxx.hesvh.cn

[S52] C++：const 与 noexcept
来源：http://eil.iojbl.cn

int size() const noexcept { return n_; }
来源：http://kog.hnqzz.top

[S53] C++：移动语义
来源：http://mgw.sxryk.cn

std::vector<int> w = std::move(v);
来源：http://iso.xuanzx.com

[S54] C++：异常处理
来源：http://ggq.zdqjudy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xtn.tanke756.top

[S55] C++：结构化绑定
来源：http://qfj.daxiang520.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hkv.zdqjudy.top

[S56] C++：optional
来源：http://wnb.316326.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fcm.chenzaomai.com

[S57] C++：编译期常量
来源：http://rag.zycfv.cn

constexpr int N = 10;
来源：http://qsu.cucudq.cn

[S58] C++：命名空间
来源：http://vlp.jqgfzy.top

namespace ns { int f() { return 1; } }
来源：http://uzu.svipenyu.cn

[S59] C++：静态断言
来源：http://adz.yj20258.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kvj.epnwcf.com

[S60] C++：遍历并删除元素
来源：http://nvk.sufxvd.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dun.zhixingplan.top

================================================================================
来源：http://uty.hywenlv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xhw.xuanzx.com

================================================================================
来源：http://jnp.zhixingplan.top

[T01] Kotlin：Hello World
来源：http://npv.smart0.xyz

println("Hello")
来源：http://vnu.hywenlv.cn

[T02] Kotlin：变量
来源：http://fkm.fanxiaobao.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mwc.jqgfzy.top

[T03] Kotlin：字符串模板
来源：http://xqv.hfpthk.cn

"值: $b"
来源：http://qlu.hysaishi.cn

[T04] Kotlin：空安全
来源：http://aow.xylfe.cn

val n: String? = null;  n?.length
来源：http://ygv.fengsongda.top

[T05] Kotlin：when 表达式
来源：http://eui.jinghuilouyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mtz.meibo888.top

[T06] Kotlin：集合映射
来源：http://lsb.sxryk.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yoq.zdqjudy.top

[T07] Kotlin：集合过滤
来源：http://mnv.jqgfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xcu.nanxinkj.top

[T08] Kotlin：数据类
来源：http://eto.havefunace.top

data class User(val name: String, val age: Int)
来源：http://kcq.nanxinkj.top

[T09] Kotlin：扩展函数
来源：http://xsu.chenlongwang.top

fun String.exclaim() = this + "!"
来源：http://thi.yj20258888.top

[T10] Kotlin：默认参数
来源：http://rau.svipenyu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vak.yuanzhike.top

[T11] Kotlin：协程
来源：http://kaj.guannengcc.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gek.meibo888.top

[T12] Kotlin：解构声明
来源：http://tnc.ppjwa.cn

val (a, b) = Pair(1, 2)
来源：http://nty.pycfn.com

[T13] Kotlin：只读 Map
来源：http://drb.jinqigfzy.top

val m = mapOf("a" to 1)
来源：http://hxi.dashuyun.cn

[T14] Kotlin：循环
来源：http://vmj.yfazqb.com

for (i in 1..10) println(i)
来源：http://dtu.shuidangran.top

[T15] Kotlin：接口
来源：http://nfo.pengpengdd.cyou

interface Shape { fun area(): Double }
来源：http://wwn.hnxiangtu.top

[T16] Swift：Hello World
来源：http://qqf.guowangkeji.top

print("Hello")
来源：http://rkl.fengsongda.top

[T17] Swift：变量与常量
来源：http://awn.xuanzx.com

var a = 1;  let b = 2
来源：http://fwx.yangfankeji.com

[T18] Swift：字符串插值
来源：http://stp.xingfuxueyuan.xyz

"值: \(b)"
来源：http://rma.jqgfzy.top

[T19] Swift：可选绑定
来源：http://wky.tarul.cn

if let n = opt { print(n) }
来源：http://ftq.andypj.xyz

[T20] Swift：数组操作
来源：http://jqq.chenlongwang.top

var a = [1, 2, 3];  a.append(4)
来源：http://yez.tian-w.cn

[T21] Swift：遍历
来源：http://efg.fengsongda.top

for x in a { print(x) }
来源：http://zxn.xylfe.cn

[T22] Swift：字典
来源：http://crj.zycfv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ugw.iojbl.cn

[T23] Swift：函数
来源：http://yeg.haohaochexian.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://crd.hongshengwenyu.top

[T24] Swift：闭包
来源：http://fpr.jinghuilouyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://apb.yj20258888.top

[T25] Swift：结构体
来源：http://str.chenzaomai.com

struct P { var x: Int }
来源：http://jkd.jqgfzy.top

[T26] Swift：类与重写
来源：http://wep.fanxiaobao.xyz

class A: Base { override func f() {} }
来源：http://zax.jinyuanbaomall.cn

[T27] Swift：错误处理
来源：http://fpb.yj202588.top

do { try f() } catch { print(error) }
来源：http://byq.c1oappe.top

[T28] Swift：枚举
来源：http://byz.shangyingyoupin.top

enum Color { case red, green }
来源：http://xrj.fehbvm.com

[T29] Swift：guard 提前返回
来源：http://hio.zhongyouzk.top

guard let x = opt else { return }
来源：http://aen.shzxlz.cn

[T30] Swift：协议
来源：http://ztr.ehwqpu.com

protocol Shape { func area() -> Double }
来源：http://pbf.feifeiyinyue.top

[T31] Lua：Hello World
来源：http://wxq.chenzaomai.com

print("Hello")
来源：http://dgf.sysykeji.top

[T32] Lua：局部变量
来源：http://bnc.hesvh.cn

local a = 1
来源：http://czf.c1oappe.top

[T33] Lua：表（数组）
来源：http://tyq.yangfankeji.com

local t = {1, 2, 3};  t[4] = 4
来源：http://fdr.yanxiufei.cn

[T34] Lua：遍历表
来源：http://djx.iojbl.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jlz.ivvv.top

[T35] Lua：字典表
来源：http://fqg.xziqi.cn

local d = { a = 1 };  d.b = 2
来源：http://ymw.jinghuilouyu.cn

[T36] Lua：函数
来源：http://xrk.sysykeji.top

function add(a, b) return a + b end
来源：http://sbk.snrcjt.cn

[T37] Lua：字符串拼接
来源：http://qsk.zhixingplan.top

"a" .. "b"
来源：http://ysb.dashuyun.cn

[T38] Lua：条件
来源：http://vxs.hammf.cn

if x > 0 then print("正") end
来源：http://vdd.guowangkeji.top

[T39] Lua：模式匹配
来源：http://jjl.quarkkingdee.top

string.find(s, "%d+")
来源：http://bbt.svipenyu.cn

[T40] Lua：元表
来源：http://gvz.pengpengdd.cyou

setmetatable({}, { __index = base })
来源：http://ntn.hnqzz.top

[T41] Perl：Hello World
来源：http://yfa.fehbvm.com

print "Hello\n";
来源：http://duv.xuanzx.com

[T42] Perl：变量类型
来源：http://reg.dashuyun.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ahb.jinghuilouyu.cn

[T43] Perl：字符串插值
来源：http://ptc.xziqi.cn

"值: $a"
来源：http://byi.fehbvm.com

[T44] Perl：条件
来源：http://jgy.nwbrower.top

if ($a > 0) { print "正"; }
来源：http://sba.shanyushiyangtech.top

[T45] Perl：数组遍历
来源：http://tma.aizwys.cn

for my $x (@arr) { print $x; }
来源：http://zgw.hfpthk.cn

[T46] Perl：哈希操作
来源：http://jbw.tarul.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://csk.yonumen.top

[T47] Perl：正则捕获
来源：http://ilf.9152youxi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zwn.meibo888.top

[T48] Perl：正则替换
来源：http://sfg.zdqjudy.top

$s =~ s/old/new/g;
来源：http://hbd.havefunace.top

[T49] Perl：函数
来源：http://laj.hywenlv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ohn.tian-w.cn

[T50] Perl：逐行读文件
来源：http://uin.sweek.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nkk.yj202588.top

while (my $line = <$fh>) { print $line; }
来源：http://fue.chenzaomai.com

[T51] Scala：Hello World
来源：http://njn.yfazqb.com

println("Hello")
来源：http://guf.haohaochexian.top

[T52] Scala：变量
来源：http://yuc.quarkkingdee.top

val a = 1;  var b = 2
来源：http://ada.haohaochexian.top

[T53] Scala：字符串插值
来源：http://swc.cheryme.top

s"值: $b"
来源：http://sta.jiagoushi.top

[T54] Scala：集合映射
来源：http://uoa.jinqigfzy.top

List(1, 2, 3).map(_ * 2)
来源：http://htz.yvedp.cn

[T55] Scala：集合过滤
来源：http://ivr.jyoumei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://obv.tianlin.xyz

[T56] Scala：样例类
来源：http://jcl.gotoacloud.top

case class User(name: String, age: Int)
来源：http://wjy.zhoulong.xyz

[T57] Scala：模式匹配
来源：http://stb.jinqigfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://wzp.bjfxy.top

[T58] Scala：函数定义
来源：http://tqa.yj202588.top

def add(a: Int, b: Int): Int = a + b
来源：http://cod.sxryk.cn

[T59] Scala：循环
来源：http://wyu.daxiang520.top

for (i <- 1 to 10) println(i)
来源：http://vme.guannengcc.top

[T60] Scala：折叠
来源：http://ifi.yj202588.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gqy.yanxiufei.cn

================================================================================
来源：http://dfy.shanyushiyangtech.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pbb.yanxiufei.cn

================================================================================
来源：http://ikn.yvedp.cn

[U01] Py：创建虚拟环境
来源：http://djo.hcnkem.com

python -m venv .venv && source .venv/bin/activate
来源：http://gou.fehbvm.com

[U02] Py：导出 / 安装依赖
来源：http://ikh.bbcook.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rpm.fzhhl.top

[U03] Py：加载 .env 配置
来源：http://vrt.gaohongyu789.top

from dotenv import load_dotenv; load_dotenv()
来源：http://crh.vqdsnc.cn

[U04] Py：变量调试打印
来源：http://qld.gzhubu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fjm.hywenlv.cn

[U05] Py：列表去重且保序
来源：http://avb.cqqwz.cn

list(dict.fromkeys(arr))
来源：http://bfv.aibaodan.cn

[U06] Py：合并两个字典
来源：http://tig.ctjpmb.com

{**a, **b}
来源：http://dws.sjlbkw.cn

[U07] Py：反转字典键值
来源：http://aym.havefunace.top

{v: k for k, v in d.items()}
来源：http://qun.guannengcc.top

[U08] Py：展平二维列表
来源：http://tad.yuanzhike.top

[y for x in nested for y in x]
来源：http://mzj.9152youxi.cn

[U09] Py：字典取最大值的键
来源：http://osm.jqgfzy.top

max(d, key=d.get)
来源：http://dcv.bjfxy.top

[U10] Py：按值排序字典
来源：http://xso.cucudq.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nao.jinqigufen.top

[U11] Py：生成器表达式
来源：http://psz.uphjek.com

(x * 2 for x in arr)
来源：http://tdc.sweek.top

[U12] Py：取出现最多的 3 个元素
来源：http://ffs.sjlbkw.cn

Counter(arr).most_common(3)
来源：http://dep.vehdjk.com

[U13] Py：固定长度队列
来源：http://bli.shanyushiyangtech.top

deque(maxlen=10)
来源：http://zxe.xuetiantiany.cn

[U14] Py：分组收集到列表
来源：http://llv.nanxinkj.top

defaultdict(list)
来源：http://hha.yvedp.cn

[U15] Py：高精度计时
来源：http://yah.cdnleiting.top

t = time.perf_counter()
来源：http://gwu.epnwcf.com

[U16] Py：命令行参数解析
来源：http://cfp.sufxvd.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oxm.ydzc1.top

[U17] Py：初始化日志
来源：http://qoz.xingfuxueyuan.xyz

logging.basicConfig(level=logging.INFO)
来源：http://ero.guannengcc.top

[U18] Py：预编译正则
来源：http://zth.jlsjyb.cn

pat = re.compile(r"\d+")
来源：http://zas.yangfankeji.com

[U19] Py：正则替换带回调
来源：http://ttj.xuetiantiany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wfn.zycfv.cn

[U20] Py：缓存函数结果
来源：http://nfs.jianghu66.top

@functools.lru_cache(maxsize=None)
来源：http://ewv.jianghu66.top

[U21] Py：自定义上下文管理器
来源：http://ezl.yj202588.top

@contextlib.contextmanager
来源：http://zfo.cdnleiting.top

[U22] Py：矩阵转置
来源：http://ado.yuanzhike.top

list(zip(*m))
来源：http://ilm.zhixingplan.top

[U23] Py：分块读取大文件
来源：http://ksv.ydzc1.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oxp.fktsv.cn

[U24] Py：路径操作
来源：http://ypw.fehbvm.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://enc.zdqjudy.top

[U25] Py：CSV 按字典读
来源：http://zxs.snrcjt.cn

csv.DictReader(f)
来源：http://yxk.zhixingplan.top

[U26] Py：并发下载
来源：http://app.gaohongyu789.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wcp.yj202588.top

[U27] Py：异步 HTTP
来源：http://tdw.snrcjt.cn

aiohttp.ClientSession() 配合 async with
来源：http://qjj.jinghuilouyu.cn

[U28] Py：类型别名
来源：http://agu.ywan-chungtsiang.top

UserId = int
来源：http://faj.sjlbkw.cn

[U29] Py：属性校验
来源：http://ntn.gogol.net.cn

@property 与 @x.setter 配合
来源：http://arv.jlsjyb.cn

[U30] Py：数据类
来源：http://hvd.guannengcc.top

@dataclass(slots=True)
来源：http://epj.hnxiangtu.top

[U31] Py：单测
来源：http://qoy.cucudq.cn

python -m pytest -q
来源：http://ohy.nanxuanxn.top

[U32] Py：代码格式化
来源：http://swm.hnqzz.top

ruff format . && ruff check --fix .
来源：http://soa.zhaomingkeji.xyz

[U33] Py：打包发布
来源：http://dod.chenlongwang.top

python -m build  （依赖 pyproject.toml）
来源：http://svq.sweek.top

[U34] Py：判断编码
来源：http://xmd.yueranfly.top

chardet.detect(raw)
来源：http://ubh.shzxlz.cn

[U35] Py：发送邮件
来源：http://rol.52xcode.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://etq.ydjk.org.cn

[U36] Py：定时任务
来源：http://fbz.zhixingplan.top

schedule.every(10).minutes.do(job)
来源：http://zwm.jinqigufen.top

[U37] Py：读写 Excel
来源：http://kiy.fehbvm.com

pandas.read_excel / DataFrame.to_excel
来源：http://uwd.gaohongyu789.top

[U38] Py：获取脚本所在目录
来源：http://qdr.cheryme.top

Path(__file__).resolve().parent
来源：http://cnt.xylfe.cn

[U39] Py：判断是否在交互环境
来源：http://urw.yongpay.top

sys.stdout.isatty()
来源：http://tlj.xziqi.cn

[U40] Py：打印到标准错误
来源：http://anh.fktsv.cn

print("err", file=sys.stderr)
来源：http://jmo.xylfe.cn

[U41] PHP：初始化 Composer 项目
来源：http://hpw.hywenlv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cma.ydzc1.top

[U42] PHP：PSR-4 自动加载
来源：http://pqk.xingfuxueyuan.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nto.cucudq.cn

[U43] PHP：声明命名空间
来源：http://svr.daxiang520.top

namespace App\Http;
来源：http://jhu.shanyushiyangtech.top

[U44] PHP：开启严格类型
来源：http://mdj.yj202588.top

declare(strict_types=1);
来源：http://xof.haohaochexian.top

[U45] PHP：类型声明与返回类型
来源：http://ufi.vqdsnc.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bvz.chenjidiqi.icu

[U46] PHP：可空类型
来源：http://oje.chenjidiqi.icu

?string $name = null
来源：http://urv.9152youxi.cn

[U47] PHP：联合类型
来源：http://zeq.smart0.xyz

int|string $id
来源：http://xng.jlsjyb.cn

[U48] PHP：纯枚举
来源：http://ymv.c1oappe.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dzh.zhixingplan.top

[U49] PHP：只读属性
来源：http://shr.bjfxy.top

public readonly string $name
来源：http://bit.sufxvd.cn

[U50] PHP：构造器属性提升
来源：http://wao.bbcook.cn

public function __construct(private int $id) {}
来源：http://req.hesvh.cn

[U51] PHP：数组解构
来源：http://bif.daxiang520.top

[$a, $b] = $arr;
来源：http://xvp.0kj1m.cn

[U52] PHP：箭头函数
来源：http://hua.c1oappe.top

$double = fn($x) => $x * 2;
来源：http://toy.meibo888.top

[U53] PHP：空合并运算符
来源：http://tnz.yongpay.top

$v = $a ?? $b ?? "default";
来源：http://vxx.yfazqb.com

[U54] PHP：空安全调用
来源：http://pfm.zdbjq.cn

$obj?->method()
来源：http://ohs.c1oappe.top

[U55] PHP：match 表达式
来源：http://jie.ydzc1.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ncn.ydzc1.top

[U56] PHP：命名参数
来源：http://ahe.jinqigufen.top

f(a: 1, b: 2)
来源：http://nur.jyoumei.cn

[U57] PHP：字符串插值
来源：http://sly.yuxming.cn

"值: {$a}"
来源：http://ifg.yuanzhike.top

[U58] PHP：数组三件套
来源：http://unr.daxiang520.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ixa.quarkkingdee.top

[U59] PHP：自定义排序
来源：http://wie.jinqigfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gkn.fehbvm.com

[U60] PHP：JSON 编解码
来源：http://vxu.ydzc1.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xls.fktsv.cn

[U61] PHP：正则
来源：http://txm.zhixingplan.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://acj.pengpengdd.cyou

[U62] PHP：日期对象
来源：http://wwh.jinqigufen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qrh.zdqjudy.top

[U63] PHP：文件读写
来源：http://ugh.hfpthk.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mwf.birdmap.top

[U64] PHP：目录遍历
来源：http://lcu.wangshuangyany.cn

glob("dir/*.php");  scandir("dir");
来源：http://eln.zdbjq.cn

[U65] PHP：会话
来源：http://jsd.chenjidiqi.icu

session_start();  $_SESSION["uid"] = 1;
来源：http://hgj.jqgufenzy.top

[U66] PHP：设置 Cookie
来源：http://fhs.birdmap.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lnl.jiagoushi.top


<!-- 参考信息 -->