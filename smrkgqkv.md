代发 wailian999

[S43] C++：智能指针
来源：http://mhc.yuxming.cn

auto p = std::make_unique<int>(5);
来源：http://qxr.dashuyun.cn

[S44] C++：引用传参
来源：http://xdi.shuidangran.top

void inc(int &x) { ++x; }
来源：http://vid.0kj1m.cn

[S45] C++：lambda
来源：http://aji.nanxinkj.top

auto add = [](int a, int b) { return a + b; };
来源：http://etx.pycfn.com

[S46] C++：函数模板
来源：http://oue.wangdashe.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ceh.pycfn.com

[S47] C++：结构化绑定遍历
来源：http://bom.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nhi.zhaomingkeji.xyz

[S48] C++：逐行读文件
来源：http://tgb.ppjwa.cn

std::ifstream in("a.txt");  std::string line;
来源：http://onl.xylfe.cn

while (std::getline(in, line)) { }
来源：http://jsd.havefunace.top

[S49] C++：写文件
来源：http://mtb.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pae.yfazqb.com

[S50] C++：格式化数字
来源：http://wwp.hywenlv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zni.havefunace.top

[S51] C++：显式类型转换
来源：http://deb.zdqjudy.top

static_cast<double>(a) / b
来源：http://kiv.haohaochexian.top

[S52] C++：const 与 noexcept
来源：http://bcm.cqqwz.cn

int size() const noexcept { return n_; }
来源：http://qtn.ctjpmb.com

[S53] C++：移动语义
来源：http://dsv.316326.xyz

std::vector<int> w = std::move(v);
来源：http://osb.xziqi.cn

[S54] C++：异常处理
来源：http://nfg.zhixingplan.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xuk.snrcjt.cn

[S55] C++：结构化绑定
来源：http://cnk.dashuyun.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ltf.hcnkem.com

[S56] C++：optional
来源：http://gql.jyoumei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uvc.uphjek.com

[S57] C++：编译期常量
来源：http://irs.pengpengdd.cyou

constexpr int N = 10;
来源：http://qca.yj202588.top

[S58] C++：命名空间
来源：http://srt.feifeiyinyue.top

namespace ns { int f() { return 1; } }
来源：http://wkd.tian-w.cn

[S59] C++：静态断言
来源：http://bmx.fktsv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://obq.kuanghao11.cn

[S60] C++：遍历并删除元素
来源：http://syx.jlsjyb.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cyn.gaohongyu789.top

================================================================================
来源：http://roe.xziqi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iuh.havefunace.top

================================================================================
来源：http://hlm.uphjek.com

[T01] Kotlin：Hello World
来源：http://xfw.gotoacloud.top

println("Hello")
来源：http://fde.c1oappe.top

[T02] Kotlin：变量
来源：http://ers.yonumen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rhr.dashuyun.cn

[T03] Kotlin：字符串模板
来源：http://pqb.nanxinkj.top

"值: $b"
来源：http://kdn.zhixingplan.top

[T04] Kotlin：空安全
来源：http://hvh.jiagoushi.top

val n: String? = null;  n?.length
来源：http://ukv.cucudq.cn

[T05] Kotlin：when 表达式
来源：http://bcq.tianlin.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kjy.wangshuangyany.cn

[T06] Kotlin：集合映射
来源：http://dkj.sweek.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hgu.pengpengdd.cyou

[T07] Kotlin：集合过滤
来源：http://tvb.birdmap.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cba.cucudq.cn

[T08] Kotlin：数据类
来源：http://vmp.jiagoushi.top

data class User(val name: String, val age: Int)
来源：http://mgk.uphjek.com

[T09] Kotlin：扩展函数
来源：http://jrt.smart0.xyz

fun String.exclaim() = this + "!"
来源：http://cxl.jinqigfzy.top

[T10] Kotlin：默认参数
来源：http://vqv.cashguo.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ysl.sysykeji.top

[T11] Kotlin：协程
来源：http://rde.zhixingplan.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://dkk.jiagoushi.top

[T12] Kotlin：解构声明
来源：http://mxp.chenjidiqi.icu

val (a, b) = Pair(1, 2)
来源：http://pfk.cdnleiting.top

[T13] Kotlin：只读 Map
来源：http://orj.wangdashe.top

val m = mapOf("a" to 1)
来源：http://sqz.chenzaomai.com

[T14] Kotlin：循环
来源：http://gjb.hnqzz.top

for (i in 1..10) println(i)
来源：http://apr.yj20258.top

[T15] Kotlin：接口
来源：http://kcl.chenzaomai.com

interface Shape { fun area(): Double }
来源：http://qgd.yj20258.top

[T16] Swift：Hello World
来源：http://qml.shangyingyoupin.top

print("Hello")
来源：http://bcn.shzxlz.cn

[T17] Swift：变量与常量
来源：http://psz.meibo888.top

var a = 1;  let b = 2
来源：http://kqx.jinyuanbaomall.cn

[T18] Swift：字符串插值
来源：http://njm.zdqjudy.top

"值: \(b)"
来源：http://sos.shanyushiyangtech.top

[T19] Swift：可选绑定
来源：http://ebg.gotoacloud.top

if let n = opt { print(n) }
来源：http://ahz.jqgufenzy.top

[T20] Swift：数组操作
来源：http://kto.dianchejie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jen.pycfn.com

[T21] Swift：遍历
来源：http://xkk.yuxming.cn

for x in a { print(x) }
来源：http://gof.zdbjq.cn

[T22] Swift：字典
来源：http://xyc.chenzaomai.com

var d = ["a": 1];  d["b"] = 2
来源：http://dii.jyoumei.cn

[T23] Swift：函数
来源：http://rug.hcnkem.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://aet.cashguo.top

[T24] Swift：闭包
来源：http://esx.aibaodan.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xvy.hnqzz.top

[T25] Swift：结构体
来源：http://fzb.nanxuanxn.top

struct P { var x: Int }
来源：http://kpz.aizwys.cn

[T26] Swift：类与重写
来源：http://hur.uphjek.com

class A: Base { override func f() {} }
来源：http://qae.52xcode.cn

[T27] Swift：错误处理
来源：http://mnq.havefunace.top

do { try f() } catch { print(error) }
来源：http://dvf.hongshengwenyu.top

[T28] Swift：枚举
来源：http://jig.9152youxi.cn

enum Color { case red, green }
来源：http://gfm.chenlongwang.top

[T29] Swift：guard 提前返回
来源：http://deb.hesvh.cn

guard let x = opt else { return }
来源：http://vhv.aizwys.cn

[T30] Swift：协议
来源：http://otn.yongpay.top

protocol Shape { func area() -> Double }
来源：http://kqx.guowangkeji.top

[T31] Lua：Hello World
来源：http://trw.vehdjk.com

print("Hello")
来源：http://fam.zhaomingkeji.xyz

[T32] Lua：局部变量
来源：http://ukw.yj202588.top

local a = 1
来源：http://ube.sweek.top

[T33] Lua：表（数组）
来源：http://mmd.jiagoushi.top

local t = {1, 2, 3};  t[4] = 4
来源：http://gjk.shzxlz.cn

[T34] Lua：遍历表
来源：http://ota.yongpay.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ybe.316326.xyz

[T35] Lua：字典表
来源：http://pik.tianlin.xyz

local d = { a = 1 };  d.b = 2
来源：http://dgr.nwbrower.top

[T36] Lua：函数
来源：http://fxs.shzxlz.cn

function add(a, b) return a + b end
来源：http://ewv.fzhhl.top

[T37] Lua：字符串拼接
来源：http://cfc.tarul.cn

"a" .. "b"
来源：http://etn.sjlbkw.cn

[T38] Lua：条件
来源：http://ocg.pengpengdd.cyou

if x > 0 then print("正") end
来源：http://ecy.shangyingyoupin.top

[T39] Lua：模式匹配
来源：http://lgv.jianghu66.top

string.find(s, "%d+")
来源：http://qiq.cheryme.top

[T40] Lua：元表
来源：http://lxv.svipenyu.cn

setmetatable({}, { __index = base })
来源：http://suv.hesvh.cn

[T41] Perl：Hello World
来源：http://did.uphjek.com

print "Hello\n";
来源：http://qwx.hysaishi.cn

[T42] Perl：变量类型
来源：http://rkq.yfazqb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vkk.hfpthk.cn

[T43] Perl：字符串插值
来源：http://isi.guowangkeji.top

"值: $a"
来源：http://znm.tanke756.top

[T44] Perl：条件
来源：http://sfv.yonumen.top

if ($a > 0) { print "正"; }
来源：http://ypi.52xcode.cn

[T45] Perl：数组遍历
来源：http://dic.xziqi.cn

for my $x (@arr) { print $x; }
来源：http://wqh.hesvh.cn

[T46] Perl：哈希操作
来源：http://mpg.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sig.ivvv.top

[T47] Perl：正则捕获
来源：http://taj.yj202588.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xrc.feifeiyinyue.top

[T48] Perl：正则替换
来源：http://qis.hnqzz.top

$s =~ s/old/new/g;
来源：http://bzo.sxryk.cn

[T49] Perl：函数
来源：http://tgz.cucudq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oei.xylfe.cn

[T50] Perl：逐行读文件
来源：http://wmq.yuxming.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://otm.vqdsnc.cn

while (my $line = <$fh>) { print $line; }
来源：http://ibb.hfpthk.cn

[T51] Scala：Hello World
来源：http://dfd.gaohongyu789.top

println("Hello")
来源：http://hcg.yongpay.top

[T52] Scala：变量
来源：http://gij.xylfe.cn

val a = 1;  var b = 2
来源：http://emr.zhijiandao.cn

[T53] Scala：字符串插值
来源：http://mjb.hcnkem.com

s"值: $b"
来源：http://kld.ydzc1.top

[T54] Scala：集合映射
来源：http://zew.jinghuilouyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://gft.vehdjk.com

[T55] Scala：集合过滤
来源：http://jbc.vqdsnc.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wia.9152youxi.cn

[T56] Scala：样例类
来源：http://qyg.bjfxy.top

case class User(name: String, age: Int)
来源：http://qvv.xylfe.cn

[T57] Scala：模式匹配
来源：http://rmv.tianlin.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://mtp.fehbvm.com

[T58] Scala：函数定义
来源：http://xyr.xinyue.icu

def add(a: Int, b: Int): Int = a + b
来源：http://mkm.mhx1999.top

[T59] Scala：循环
来源：http://org.gogol.net.cn

for (i <- 1 to 10) println(i)
来源：http://znu.tanke756.top

[T60] Scala：折叠
来源：http://kmf.jqgfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qra.bbcook.cn

================================================================================
来源：http://dbc.yongpay.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vbh.zhaomingkeji.xyz

================================================================================
来源：http://mmp.hammf.cn

[U01] Py：创建虚拟环境
来源：http://hkx.jqgufenzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://alg.yuxming.cn

[U02] Py：导出 / 安装依赖
来源：http://szs.gzhubu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://aqh.vehdjk.com

[U03] Py：加载 .env 配置
来源：http://nlh.guowangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://pxo.sjlbkw.cn

[U04] Py：变量调试打印
来源：http://djf.aizwys.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yuv.hywenlv.cn

[U05] Py：列表去重且保序
来源：http://lfg.sysykeji.top

list(dict.fromkeys(arr))
来源：http://pfh.hongshengwenyu.top

[U06] Py：合并两个字典
来源：http://zbu.fengsongda.top

{**a, **b}
来源：http://rco.quarkkingdee.top

[U07] Py：反转字典键值
来源：http://ngq.sufxvd.cn

{v: k for k, v in d.items()}
来源：http://suz.iojbl.cn

[U08] Py：展平二维列表
来源：http://vle.bjfxy.top

[y for x in nested for y in x]
来源：http://kpr.guowangkeji.top

[U09] Py：字典取最大值的键
来源：http://mha.hammf.cn

max(d, key=d.get)
来源：http://xkd.nanxuanxn.top

[U10] Py：按值排序字典
来源：http://fyb.yueranfly.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ocr.yj202588.top

[U11] Py：生成器表达式
来源：http://qmn.yueranfly.top

(x * 2 for x in arr)
来源：http://lxa.vqdsnc.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qwm.jyoumei.cn

Counter(arr).most_common(3)
来源：http://iqb.daxiang520.top

[U13] Py：固定长度队列
来源：http://akk.xylfe.cn

deque(maxlen=10)
来源：http://ueg.gaohongyu789.top

[U14] Py：分组收集到列表
来源：http://xhl.cashguo.top

defaultdict(list)
来源：http://muc.cucudq.cn

[U15] Py：高精度计时
来源：http://fsh.jinghuilouyu.cn

t = time.perf_counter()
来源：http://iue.redwolf501.top

[U16] Py：命令行参数解析
来源：http://jul.yueranfly.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fjy.feifeiyinyue.top

[U17] Py：初始化日志
来源：http://lra.nanxuanxn.top

logging.basicConfig(level=logging.INFO)
来源：http://upc.bjfxy.top

[U18] Py：预编译正则
来源：http://asm.cqqwz.cn

pat = re.compile(r"\d+")
来源：http://yib.birdmap.top

[U19] Py：正则替换带回调
来源：http://kjg.sysykeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ufp.cucudq.cn

[U20] Py：缓存函数结果
来源：http://uqz.tanke756.top

@functools.lru_cache(maxsize=None)
来源：http://hhk.aibaodan.cn

[U21] Py：自定义上下文管理器
来源：http://tba.shuidangran.top

@contextlib.contextmanager
来源：http://fhh.jqgfzy.top

[U22] Py：矩阵转置
来源：http://qxr.shangyingyoupin.top

list(zip(*m))
来源：http://poa.ehwqpu.com

[U23] Py：分块读取大文件
来源：http://ued.bbcook.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://soa.c1oappe.top

[U24] Py：路径操作
来源：http://aku.shuidangran.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ley.yfazqb.com

[U25] Py：CSV 按字典读
来源：http://crf.shangyingyoupin.top

csv.DictReader(f)
来源：http://eii.hnxiangtu.top

[U26] Py：并发下载
来源：http://yfk.guannengcc.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dht.ppjwa.cn

[U27] Py：异步 HTTP
来源：http://mso.mhx1999.top

aiohttp.ClientSession() 配合 async with
来源：http://lsp.fanxiaobao.xyz

[U28] Py：类型别名
来源：http://dch.daxiang520.top

UserId = int
来源：http://yuk.xylfe.cn

[U29] Py：属性校验
来源：http://zof.yj20258888.top

@property 与 @x.setter 配合
来源：http://rbr.jiagoushi.top

[U30] Py：数据类
来源：http://fun.sweek.top

@dataclass(slots=True)
来源：http://nvc.guowangkeji.top

[U31] Py：单测
来源：http://pfg.haohaochexian.top

python -m pytest -q
来源：http://qlq.daxiang520.top

[U32] Py：代码格式化
来源：http://zdc.smart0.xyz

ruff format . && ruff check --fix .
来源：http://yqp.ybcxt.top

[U33] Py：打包发布
来源：http://zkv.gogol.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://yzz.dianchejie.cn

[U34] Py：判断编码
来源：http://cki.52xcode.cn

chardet.detect(raw)
来源：http://hep.jianghu66.top

[U35] Py：发送邮件
来源：http://mlo.fanxiaobao.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qge.yj202588.top

[U36] Py：定时任务
来源：http://cfg.smart0.xyz

schedule.every(10).minutes.do(job)
来源：http://sah.vehdjk.com

[U37] Py：读写 Excel
来源：http://ige.zycfv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kyj.guowangkeji.top

[U38] Py：获取脚本所在目录
来源：http://ris.jqgufenzy.top

Path(__file__).resolve().parent
来源：http://hox.zdqjudy.top

[U39] Py：判断是否在交互环境
来源：http://hgh.vehdjk.com

sys.stdout.isatty()
来源：http://jge.yuxming.cn

[U40] Py：打印到标准错误
来源：http://mgu.yvedp.cn

print("err", file=sys.stderr)
来源：http://hye.pycfn.com

[U41] PHP：初始化 Composer 项目
来源：http://qvf.aibaodan.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gco.yongpay.top

[U42] PHP：PSR-4 自动加载
来源：http://eon.yonumen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jvr.yuanzhike.top

[U43] PHP：声明命名空间
来源：http://pmh.xylfe.cn

namespace App\Http;
来源：http://dse.kuanghao11.cn

[U44] PHP：开启严格类型
来源：http://ncz.xuanzx.com

declare(strict_types=1);
来源：http://ovx.bjfxy.top

[U45] PHP：类型声明与返回类型
来源：http://bcj.epnwcf.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://jck.mhx1999.top

[U46] PHP：可空类型
来源：http://ifc.hnxiangtu.top

?string $name = null
来源：http://zfx.chenzaomai.com

[U47] PHP：联合类型
来源：http://pvf.yj20258.top

int|string $id
来源：http://pxk.wangshuangyany.cn

[U48] PHP：纯枚举
来源：http://wfw.quarkkingdee.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ung.yonumen.top

[U49] PHP：只读属性
来源：http://umy.hammf.cn

public readonly string $name
来源：http://hra.yj20258888.top

[U50] PHP：构造器属性提升
来源：http://qyz.hongshengwenyu.top

public function __construct(private int $id) {}
来源：http://tvk.jiagoushi.top

[U51] PHP：数组解构
来源：http://ofd.pycfn.com

[$a, $b] = $arr;
来源：http://skb.jyoumei.cn

[U52] PHP：箭头函数
来源：http://oqq.yongpay.top

$double = fn($x) => $x * 2;
来源：http://uim.aibaodan.cn

[U53] PHP：空合并运算符
来源：http://ybb.aizwys.cn

$v = $a ?? $b ?? "default";
来源：http://phk.tian-w.cn

[U54] PHP：空安全调用
来源：http://xzy.fktsv.cn

$obj?->method()
来源：http://wvn.jqgfzy.top

[U55] PHP：match 表达式
来源：http://kbv.zycfv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://voh.vehdjk.com

[U56] PHP：命名参数
来源：http://qlv.snrcjt.cn

f(a: 1, b: 2)
来源：http://lgm.tarul.cn

[U57] PHP：字符串插值
来源：http://abd.fanxiaobao.xyz

"值: {$a}"
来源：http://qay.yuxming.cn

[U58] PHP：数组三件套
来源：http://fwb.havefunace.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hxl.zhongyouzk.top

[U59] PHP：自定义排序
来源：http://hrh.xuetiantiany.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ryo.316326.xyz

[U60] PHP：JSON 编解码
来源：http://yep.shanyushiyangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ndk.9152youxi.cn

[U61] PHP：正则
来源：http://nyk.wangdashe.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yzz.dianchejie.cn

[U62] PHP：日期对象
来源：http://yws.gaohongyu789.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qsd.shanyushiyangkeji.top

[U63] PHP：文件读写
来源：http://duo.ybcxt.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rbf.tarul.cn

[U64] PHP：目录遍历
来源：http://kwp.nanxinkj.top

glob("dir/*.php");  scandir("dir");
来源：http://nxs.hfpthk.cn

[U65] PHP：会话
来源：http://vrt.jqgfzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://yxl.yongpay.top

[U66] PHP：设置 Cookie
来源：http://kgz.chenjidiqi.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sws.hnqzz.top

[U67] PHP：处理文件上传
来源：http://zlq.chenzaomai.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vbt.wangdashe.top

[U68] PHP：PDO 连接
来源：http://jfl.jinqigufen.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://asj.shangyingyoupin.top


<!-- 参考信息 -->