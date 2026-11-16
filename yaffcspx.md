代发 wailian999

[S39] C++：自定义比较器排序
来源：http://dln.mhx1999.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dca.yanxiufei.cn

[S40] C++：查找元素
来源：http://hry.pycfn.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cvt.snrcjt.cn

[S41] C++：类与构造函数
来源：http://cdf.cdnleiting.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dnh.andypj.xyz

[S42] C++：继承与虚函数
来源：http://ubx.yanxiufei.cn

class B : public Base { public: void f() override {} };
来源：http://ogi.ydzc1.top

[S43] C++：智能指针
来源：http://jub.jinghuilouyu.cn

auto p = std::make_unique<int>(5);
来源：http://qlx.ywan-chungtsiang.top

[S44] C++：引用传参
来源：http://znk.xingfuxueyuan.xyz

void inc(int &x) { ++x; }
来源：http://idj.yanxiufei.cn

[S45] C++：lambda
来源：http://yfj.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vcm.sweek.top

[S46] C++：函数模板
来源：http://tom.vehdjk.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://epy.zhoulong.xyz

[S47] C++：结构化绑定遍历
来源：http://pzr.ybcxt.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://thw.cqqwz.cn

[S48] C++：逐行读文件
来源：http://hcp.ybcxt.top

std::ifstream in("a.txt");  std::string line;
来源：http://qzh.pengpengdd.cyou

while (std::getline(in, line)) { }
来源：http://rvj.redwolf501.top

[S49] C++：写文件
来源：http://qkv.uphjek.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gbd.cucudq.cn

[S50] C++：格式化数字
来源：http://qqj.kuanghao11.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xee.yuanzhike.top

[S51] C++：显式类型转换
来源：http://cuj.vqdsnc.cn

static_cast<double>(a) / b
来源：http://snt.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://cyu.birdmap.top

int size() const noexcept { return n_; }
来源：http://xej.nwbrower.top

[S53] C++：移动语义
来源：http://cfb.gogol.net.cn

std::vector<int> w = std::move(v);
来源：http://inq.guowangkeji.top

[S54] C++：异常处理
来源：http://nag.hywenlv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dot.jinqigfzy.top

[S55] C++：结构化绑定
来源：http://jgy.sufxvd.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jta.gotoacloud.top

[S56] C++：optional
来源：http://ipw.xuanzx.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tgx.zdbjq.cn

[S57] C++：编译期常量
来源：http://bag.aizwys.cn

constexpr int N = 10;
来源：http://yyc.xuanzx.com

[S58] C++：命名空间
来源：http://hhh.tian-w.cn

namespace ns { int f() { return 1; } }
来源：http://lny.jinyuanbaomall.cn

[S59] C++：静态断言
来源：http://jbz.zhijiandao.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jtq.sxryk.cn

[S60] C++：遍历并删除元素
来源：http://ssd.zhongyouzk.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kev.52xcode.cn

================================================================================
来源：http://nek.ydjk.org.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://woe.yj20258888.top

================================================================================
来源：http://fmi.cheryme.top

[T01] Kotlin：Hello World
来源：http://bsf.yuxming.cn

println("Hello")
来源：http://nao.zhixingplan.top

[T02] Kotlin：变量
来源：http://yqi.xylfe.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vrf.cheryme.top

[T03] Kotlin：字符串模板
来源：http://jpd.kuanghao11.cn

"值: $b"
来源：http://ijd.tianlin.xyz

[T04] Kotlin：空安全
来源：http://lbs.xziqi.cn

val n: String? = null;  n?.length
来源：http://how.hfpthk.cn

[T05] Kotlin：when 表达式
来源：http://yxs.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sib.nanxuanxn.top

[T06] Kotlin：集合映射
来源：http://wts.cheryme.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hzg.dianchejie.cn

[T07] Kotlin：集合过滤
来源：http://pfh.jlsjyb.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://iee.yj20258888.top

[T08] Kotlin：数据类
来源：http://ybb.zhiwuduotai.top

data class User(val name: String, val age: Int)
来源：http://qmr.yj20258888.top

[T09] Kotlin：扩展函数
来源：http://vup.bbcook.cn

fun String.exclaim() = this + "!"
来源：http://npt.yueranfly.top

[T10] Kotlin：默认参数
来源：http://ukl.pycfn.com

fun greet(name: String = "World") = "Hi $name"
来源：http://snz.epnwcf.com

[T11] Kotlin：协程
来源：http://ayw.smart0.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://vas.dianchejie.cn

[T12] Kotlin：解构声明
来源：http://yio.yangfankeji.com

val (a, b) = Pair(1, 2)
来源：http://ypp.shanyushiyangtech.top

[T13] Kotlin：只读 Map
来源：http://wxl.yongpay.top

val m = mapOf("a" to 1)
来源：http://pif.nwbrower.top

[T14] Kotlin：循环
来源：http://mza.zhengqikj.top

for (i in 1..10) println(i)
来源：http://hba.yongpay.top

[T15] Kotlin：接口
来源：http://zug.hesvh.cn

interface Shape { fun area(): Double }
来源：http://xwz.cdnleiting.top

[T16] Swift：Hello World
来源：http://qwi.yonumen.top

print("Hello")
来源：http://jxk.jinqigfzy.top

[T17] Swift：变量与常量
来源：http://pqd.chenzaomai.com

var a = 1;  let b = 2
来源：http://hbu.xuanzx.com

[T18] Swift：字符串插值
来源：http://idk.ybcxt.top

"值: \(b)"
来源：http://gzz.dianchejie.cn

[T19] Swift：可选绑定
来源：http://zde.xylfe.cn

if let n = opt { print(n) }
来源：http://hfo.9152youxi.cn

[T20] Swift：数组操作
来源：http://kqy.sufxvd.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rtb.cqqwz.cn

[T21] Swift：遍历
来源：http://kbq.jqgufenzy.top

for x in a { print(x) }
来源：http://hcd.yj20258.top

[T22] Swift：字典
来源：http://fhf.fehbvm.com

var d = ["a": 1];  d["b"] = 2
来源：http://ivi.tarul.cn

[T23] Swift：函数
来源：http://fdk.fzhhl.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vcu.zhongyouzk.top

[T24] Swift：闭包
来源：http://smf.zhiwuduotai.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://pcx.hcnkem.com

[T25] Swift：结构体
来源：http://fwg.aibaodan.cn

struct P { var x: Int }
来源：http://jqp.hfpthk.cn

[T26] Swift：类与重写
来源：http://psc.vehdjk.com

class A: Base { override func f() {} }
来源：http://llk.gogol.net.cn

[T27] Swift：错误处理
来源：http://rqg.hnxiangtu.top

do { try f() } catch { print(error) }
来源：http://hbk.nanxuanxn.top

[T28] Swift：枚举
来源：http://iqs.yj202588.top

enum Color { case red, green }
来源：http://fcj.guannengcc.top

[T29] Swift：guard 提前返回
来源：http://ykz.zhengqikj.top

guard let x = opt else { return }
来源：http://qde.sjlbkw.cn

[T30] Swift：协议
来源：http://gup.iojbl.cn

protocol Shape { func area() -> Double }
来源：http://pox.jlsjyb.cn

[T31] Lua：Hello World
来源：http://eta.chenzaomai.com

print("Hello")
来源：http://ckc.zhengqikj.top

[T32] Lua：局部变量
来源：http://ggc.dashuyun.cn

local a = 1
来源：http://rvd.cdnleiting.top

[T33] Lua：表（数组）
来源：http://rag.smart0.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://cdm.gotoacloud.top

[T34] Lua：遍历表
来源：http://jrg.52xcode.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jor.birdmap.top

[T35] Lua：字典表
来源：http://bfv.shuidangran.top

local d = { a = 1 };  d.b = 2
来源：http://bey.jyoumei.cn

[T36] Lua：函数
来源：http://jpm.chenlongwang.top

function add(a, b) return a + b end
来源：http://gdw.yueranfly.top

[T37] Lua：字符串拼接
来源：http://swv.yueranfly.top

"a" .. "b"
来源：http://dxk.ydzc1.top

[T38] Lua：条件
来源：http://ptd.tian-w.cn

if x > 0 then print("正") end
来源：http://bpy.fehbvm.com

[T39] Lua：模式匹配
来源：http://krz.pycfn.com

string.find(s, "%d+")
来源：http://hpk.yuxming.cn

[T40] Lua：元表
来源：http://hja.yj202588.top

setmetatable({}, { __index = base })
来源：http://jar.shanyushiyangkeji.top

[T41] Perl：Hello World
来源：http://pti.9152youxi.cn

print "Hello\n";
来源：http://hss.daxiang520.top

[T42] Perl：变量类型
来源：http://djz.epnwcf.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://khp.shangyingyoupin.top

[T43] Perl：字符串插值
来源：http://fpo.snrcjt.cn

"值: $a"
来源：http://nix.pycfn.com

[T44] Perl：条件
来源：http://pjq.9152youxi.cn

if ($a > 0) { print "正"; }
来源：http://mhu.smart0.xyz

[T45] Perl：数组遍历
来源：http://jbn.xingfuxueyuan.xyz

for my $x (@arr) { print $x; }
来源：http://jkh.ydjk.org.cn

[T46] Perl：哈希操作
来源：http://vqm.yj202588.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vsn.ywan-chungtsiang.top

[T47] Perl：正则捕获
来源：http://jrx.cqqwz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fxu.yongpay.top

[T48] Perl：正则替换
来源：http://rcs.bbcook.cn

$s =~ s/old/new/g;
来源：http://rgt.dianchejie.cn

[T49] Perl：函数
来源：http://iqn.yongpay.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dma.daria6918.cn

[T50] Perl：逐行读文件
来源：http://mhn.cdnleiting.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xhy.yj20258888.top

while (my $line = <$fh>) { print $line; }
来源：http://evy.316326.xyz

[T51] Scala：Hello World
来源：http://doa.aibaodan.cn

println("Hello")
来源：http://dzp.epnwcf.com

[T52] Scala：变量
来源：http://ifp.shanyushiyangkeji.top

val a = 1;  var b = 2
来源：http://mfz.zhiwuduotai.top

[T53] Scala：字符串插值
来源：http://wxe.feifeiyinyue.top

s"值: $b"
来源：http://ygx.yuxming.cn

[T54] Scala：集合映射
来源：http://rxz.smart0.xyz

List(1, 2, 3).map(_ * 2)
来源：http://xee.xingfuxueyuan.xyz

[T55] Scala：集合过滤
来源：http://dhh.yj20258.top

List(1, 2, 3).filter(_ > 1)
来源：http://lzp.pengpengdd.cyou

[T56] Scala：样例类
来源：http://ela.jiagoushi.top

case class User(name: String, age: Int)
来源：http://ske.havefunace.top

[T57] Scala：模式匹配
来源：http://uyt.316326.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://ogg.xuanzx.com

[T58] Scala：函数定义
来源：http://gkk.xingfuxueyuan.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://hvg.jinqigufen.top

[T59] Scala：循环
来源：http://srb.cdnleiting.top

for (i <- 1 to 10) println(i)
来源：http://aww.snrcjt.cn

[T60] Scala：折叠
来源：http://jhj.zhengqikj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hdc.dianchejie.cn

================================================================================
来源：http://srl.yuanzhike.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nrd.ywan-chungtsiang.top

================================================================================
来源：http://bdn.bjfxy.top

[U01] Py：创建虚拟环境
来源：http://xnz.xinyue.icu

python -m venv .venv && source .venv/bin/activate
来源：http://bmt.nanxinkj.top

[U02] Py：导出 / 安装依赖
来源：http://wnj.tarul.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://isi.gzhubu.top

[U03] Py：加载 .env 配置
来源：http://log.zhaomingkeji.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://eoo.9152youxi.cn

[U04] Py：变量调试打印
来源：http://nhq.wangdashe.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lrt.xinyue.icu

[U05] Py：列表去重且保序
来源：http://osa.c1oappe.top

list(dict.fromkeys(arr))
来源：http://gfv.zhiwuduotai.top

[U06] Py：合并两个字典
来源：http://knc.sysykeji.top

{**a, **b}
来源：http://hfk.jyoumei.cn

[U07] Py：反转字典键值
来源：http://jgo.birdmap.top

{v: k for k, v in d.items()}
来源：http://uit.xuetiantiany.cn

[U08] Py：展平二维列表
来源：http://cmf.shuidangran.top

[y for x in nested for y in x]
来源：http://zuf.shangyingyoupin.top

[U09] Py：字典取最大值的键
来源：http://vhw.chenjidiqi.icu

max(d, key=d.get)
来源：http://xvr.ydzc1.top

[U10] Py：按值排序字典
来源：http://yxd.yvedp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wbf.havefunace.top

[U11] Py：生成器表达式
来源：http://hpq.hammf.cn

(x * 2 for x in arr)
来源：http://wuz.snrcjt.cn

[U12] Py：取出现最多的 3 个元素
来源：http://huo.sweek.top

Counter(arr).most_common(3)
来源：http://nla.chenzaomai.com

[U13] Py：固定长度队列
来源：http://oao.zhijiandao.cn

deque(maxlen=10)
来源：http://tdk.pycfn.com

[U14] Py：分组收集到列表
来源：http://snd.zhengqikj.top

defaultdict(list)
来源：http://tpt.yangfankeji.com

[U15] Py：高精度计时
来源：http://wpu.fzhhl.top

t = time.perf_counter()
来源：http://gsw.zhiwuduotai.top

[U16] Py：命令行参数解析
来源：http://muv.shuidangran.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bqw.chenlongwang.top

[U17] Py：初始化日志
来源：http://hlw.chenjidiqi.icu

logging.basicConfig(level=logging.INFO)
来源：http://pie.nanxinkj.top

[U18] Py：预编译正则
来源：http://djw.yj20258.top

pat = re.compile(r"\d+")
来源：http://jxf.hammf.cn

[U19] Py：正则替换带回调
来源：http://qet.bjfxy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://twf.ppjwa.cn

[U20] Py：缓存函数结果
来源：http://vhf.vqdsnc.cn

@functools.lru_cache(maxsize=None)
来源：http://brn.hammf.cn

[U21] Py：自定义上下文管理器
来源：http://yns.guowangkeji.top

@contextlib.contextmanager
来源：http://yev.svipenyu.cn

[U22] Py：矩阵转置
来源：http://cwu.zhijiandao.cn

list(zip(*m))
来源：http://kwd.tian-w.cn

[U23] Py：分块读取大文件
来源：http://szd.jqgufenzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ldh.wangshuangyany.cn

[U24] Py：路径操作
来源：http://szc.ybcxt.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zyi.gaohongyu789.top

[U25] Py：CSV 按字典读
来源：http://xva.ybcxt.top

csv.DictReader(f)
来源：http://twv.shangyingyoupin.top

[U26] Py：并发下载
来源：http://axj.cdnleiting.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nto.gotoacloud.top

[U27] Py：异步 HTTP
来源：http://zda.ehwqpu.com

aiohttp.ClientSession() 配合 async with
来源：http://wxe.hongshengwenyu.top

[U28] Py：类型别名
来源：http://okk.yj20258.top

UserId = int
来源：http://yqg.sxryk.cn

[U29] Py：属性校验
来源：http://nsg.kuanghao11.cn

@property 与 @x.setter 配合
来源：http://ywm.redwolf501.top

[U30] Py：数据类
来源：http://quo.chenzaomai.com

@dataclass(slots=True)
来源：http://zxq.fengsongda.top

[U31] Py：单测
来源：http://ohn.fktsv.cn

python -m pytest -q
来源：http://fps.aibaodan.cn

[U32] Py：代码格式化
来源：http://qwi.sxryk.cn

ruff format . && ruff check --fix .
来源：http://ftl.jqgfzy.top

[U33] Py：打包发布
来源：http://gzw.shuidangran.top

python -m build  （依赖 pyproject.toml）
来源：http://qgw.sweek.top

[U34] Py：判断编码
来源：http://lqo.bbcook.cn

chardet.detect(raw)
来源：http://qqc.gotoacloud.top

[U35] Py：发送邮件
来源：http://llb.yj20258888.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kln.nwbrower.top

[U36] Py：定时任务
来源：http://yxu.yuanzhike.top

schedule.every(10).minutes.do(job)
来源：http://gsu.cucudq.cn

[U37] Py：读写 Excel
来源：http://rmd.yvedp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zck.jlsjyb.cn

[U38] Py：获取脚本所在目录
来源：http://jwx.dianchejie.cn

Path(__file__).resolve().parent
来源：http://cno.zhixingplan.top

[U39] Py：判断是否在交互环境
来源：http://isu.quarkkingdee.top

sys.stdout.isatty()
来源：http://apk.9152youxi.cn

[U40] Py：打印到标准错误
来源：http://qkz.daria6918.cn

print("err", file=sys.stderr)
来源：http://mrz.xuetiantiany.cn

[U41] PHP：初始化 Composer 项目
来源：http://tpk.jqgufenzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jlc.52xcode.cn

[U42] PHP：PSR-4 自动加载
来源：http://qyc.iojbl.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gha.jqgfzy.top

[U43] PHP：声明命名空间
来源：http://kxh.fengsongda.top

namespace App\Http;
来源：http://dry.daxiang520.top

[U44] PHP：开启严格类型
来源：http://mtb.ehwqpu.com

declare(strict_types=1);
来源：http://fkf.tian-w.cn

[U45] PHP：类型声明与返回类型
来源：http://oge.hcnkem.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://wmm.bjfxy.top

[U46] PHP：可空类型
来源：http://zyg.316326.xyz

?string $name = null
来源：http://nnj.zdbjq.cn

[U47] PHP：联合类型
来源：http://wdv.birdmap.top

int|string $id
来源：http://bek.cdnleiting.top

[U48] PHP：纯枚举
来源：http://owy.zhijiandao.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nhg.xingfuxueyuan.xyz

[U49] PHP：只读属性
来源：http://lgz.xuetiantiany.cn

public readonly string $name
来源：http://dnc.yj20258.top

[U50] PHP：构造器属性提升
来源：http://uyt.zhixingplan.top

public function __construct(private int $id) {}
来源：http://viq.ehwqpu.com

[U51] PHP：数组解构
来源：http://uue.jiagoushi.top

[$a, $b] = $arr;
来源：http://enz.gogol.net.cn

[U52] PHP：箭头函数
来源：http://wba.dashuyun.cn

$double = fn($x) => $x * 2;
来源：http://ghh.0kj1m.cn

[U53] PHP：空合并运算符
来源：http://snt.dianchejie.cn

$v = $a ?? $b ?? "default";
来源：http://rcu.vehdjk.com

[U54] PHP：空安全调用
来源：http://ffp.xuetiantiany.cn

$obj?->method()
来源：http://wfz.sweek.top

[U55] PHP：match 表达式
来源：http://ikv.yj20258888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cwx.yj202588.top

[U56] PHP：命名参数
来源：http://zmo.ehwqpu.com

f(a: 1, b: 2)
来源：http://bmn.yj20258888.top

[U57] PHP：字符串插值
来源：http://tmz.tianlin.xyz

"值: {$a}"
来源：http://enq.andypj.xyz

[U58] PHP：数组三件套
来源：http://nvh.cucudq.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://guj.daria6918.cn

[U59] PHP：自定义排序
来源：http://pom.haohaochexian.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mtn.hfpthk.cn

[U60] PHP：JSON 编解码
来源：http://bqj.cqqwz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cml.hcnkem.com

[U61] PHP：正则
来源：http://gqu.iojbl.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wbp.gotoacloud.top

[U62] PHP：日期对象
来源：http://qkl.0kj1m.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xun.tarul.cn

[U63] PHP：文件读写
来源：http://mtd.gaohongyu789.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://smo.xylfe.cn

[U64] PHP：目录遍历
来源：http://qig.snrcjt.cn

glob("dir/*.php");  scandir("dir");
来源：http://dmo.hywenlv.cn


<!-- 参考信息 -->