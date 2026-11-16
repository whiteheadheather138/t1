代发 wailian999

[S43] C++：智能指针
来源：http://tyn.zdqjudy.top

auto p = std::make_unique<int>(5);
来源：http://mma.gaohongyu789.top

[S44] C++：引用传参
来源：http://uxz.52xcode.cn

void inc(int &x) { ++x; }
来源：http://ncm.pycfn.com

[S45] C++：lambda
来源：http://pya.316326.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://rrl.iojbl.cn

[S46] C++：函数模板
来源：http://bhi.yuanzhike.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://afg.pycfn.com

[S47] C++：结构化绑定遍历
来源：http://ztq.zhixingplan.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dag.yj20258888.top

[S48] C++：逐行读文件
来源：http://cbv.shuidangran.top

std::ifstream in("a.txt");  std::string line;
来源：http://ejt.c1oappe.top

while (std::getline(in, line)) { }
来源：http://lbf.yongpay.top

[S49] C++：写文件
来源：http://gux.guowangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ayv.yvedp.cn

[S50] C++：格式化数字
来源：http://zfr.andypj.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nop.smart0.xyz

[S51] C++：显式类型转换
来源：http://xit.shuidangran.top

static_cast<double>(a) / b
来源：http://tmo.wangshuangyany.cn

[S52] C++：const 与 noexcept
来源：http://yjh.zhaomingkeji.xyz

int size() const noexcept { return n_; }
来源：http://xur.wangshuangyany.cn

[S53] C++：移动语义
来源：http://bgj.jinyuanbaomall.cn

std::vector<int> w = std::move(v);
来源：http://kqt.chenlongwang.top

[S54] C++：异常处理
来源：http://wkk.gaohongyu789.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dbw.redwolf501.top

[S55] C++：结构化绑定
来源：http://ihy.yanxiufei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tol.aizwys.cn

[S56] C++：optional
来源：http://mza.guowangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zfp.zhijiandao.cn

[S57] C++：编译期常量
来源：http://msh.zycfv.cn

constexpr int N = 10;
来源：http://mep.vqdsnc.cn

[S58] C++：命名空间
来源：http://ulu.316326.xyz

namespace ns { int f() { return 1; } }
来源：http://mrv.fanxiaobao.xyz

[S59] C++：静态断言
来源：http://jpw.bbcook.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://swz.redwolf501.top

[S60] C++：遍历并删除元素
来源：http://wfk.bjfxy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://whu.ydzc1.top

================================================================================
来源：http://ebw.xuanzx.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vha.svipenyu.cn

================================================================================
来源：http://vnp.yongpay.top

[T01] Kotlin：Hello World
来源：http://dns.sysykeji.top

println("Hello")
来源：http://oqe.ydzc1.top

[T02] Kotlin：变量
来源：http://igq.gotoacloud.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vai.cqqwz.cn

[T03] Kotlin：字符串模板
来源：http://jfx.nanxuanxn.top

"值: $b"
来源：http://adh.pycfn.com

[T04] Kotlin：空安全
来源：http://bgv.cqqwz.cn

val n: String? = null;  n?.length
来源：http://pkq.ehwqpu.com

[T05] Kotlin：when 表达式
来源：http://qvb.cheryme.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vng.0kj1m.cn

[T06] Kotlin：集合映射
来源：http://eyn.shuidangran.top

listOf(1, 2, 3).map { it * 2 }
来源：http://sbd.zhoulong.xyz

[T07] Kotlin：集合过滤
来源：http://ahg.bjfxy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kev.nanxinkj.top

[T08] Kotlin：数据类
来源：http://lyp.jlsjyb.cn

data class User(val name: String, val age: Int)
来源：http://omi.yj202588.top

[T09] Kotlin：扩展函数
来源：http://gvp.ydzc1.top

fun String.exclaim() = this + "!"
来源：http://zmv.vehdjk.com

[T10] Kotlin：默认参数
来源：http://miu.wangshuangyany.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rer.sxryk.cn

[T11] Kotlin：协程
来源：http://jeb.tarul.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lqu.feifeiyinyue.top

[T12] Kotlin：解构声明
来源：http://les.yj20258.top

val (a, b) = Pair(1, 2)
来源：http://hkc.ctjpmb.com

[T13] Kotlin：只读 Map
来源：http://egx.jianghu66.top

val m = mapOf("a" to 1)
来源：http://ftd.0kj1m.cn

[T14] Kotlin：循环
来源：http://pto.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://liu.chenzaomai.com

[T15] Kotlin：接口
来源：http://xwb.yj202588.top

interface Shape { fun area(): Double }
来源：http://eew.mhx1999.top

[T16] Swift：Hello World
来源：http://pov.nanxuanxn.top

print("Hello")
来源：http://wdw.chenjidiqi.icu

[T17] Swift：变量与常量
来源：http://csk.zhixingplan.top

var a = 1;  let b = 2
来源：http://hji.feifeiyinyue.top

[T18] Swift：字符串插值
来源：http://axs.epnwcf.com

"值: \(b)"
来源：http://swu.aibaodan.cn

[T19] Swift：可选绑定
来源：http://fsk.yj202588.top

if let n = opt { print(n) }
来源：http://njk.zycfv.cn

[T20] Swift：数组操作
来源：http://cnq.shangyingyoupin.top

var a = [1, 2, 3];  a.append(4)
来源：http://zlv.zhoulong.xyz

[T21] Swift：遍历
来源：http://poo.gogol.net.cn

for x in a { print(x) }
来源：http://hgi.zdbjq.cn

[T22] Swift：字典
来源：http://cfh.c1oappe.top

var d = ["a": 1];  d["b"] = 2
来源：http://dyk.zhixingplan.top

[T23] Swift：函数
来源：http://kcv.tian-w.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wtc.kuanghao11.cn

[T24] Swift：闭包
来源：http://jon.ppjwa.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ewy.jinqigufen.top

[T25] Swift：结构体
来源：http://wil.316326.xyz

struct P { var x: Int }
来源：http://yiu.zdbjq.cn

[T26] Swift：类与重写
来源：http://afi.zhengqikj.top

class A: Base { override func f() {} }
来源：http://vcg.cdnleiting.top

[T27] Swift：错误处理
来源：http://thx.havefunace.top

do { try f() } catch { print(error) }
来源：http://hpw.jyoumei.cn

[T28] Swift：枚举
来源：http://zpa.haohaochexian.top

enum Color { case red, green }
来源：http://yum.hysaishi.cn

[T29] Swift：guard 提前返回
来源：http://kfn.ppjwa.cn

guard let x = opt else { return }
来源：http://dug.shanyushiyangtech.top

[T30] Swift：协议
来源：http://mtf.meibo888.top

protocol Shape { func area() -> Double }
来源：http://jmo.guowangkeji.top

[T31] Lua：Hello World
来源：http://asn.sjlbkw.cn

print("Hello")
来源：http://kvs.cheryme.top

[T32] Lua：局部变量
来源：http://kod.quarkkingdee.top

local a = 1
来源：http://ssh.jqgfzy.top

[T33] Lua：表（数组）
来源：http://lbw.daria6918.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://flm.zycfv.cn

[T34] Lua：遍历表
来源：http://nhn.dianchejie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hut.ydjk.org.cn

[T35] Lua：字典表
来源：http://tfg.zdqjudy.top

local d = { a = 1 };  d.b = 2
来源：http://apa.hesvh.cn

[T36] Lua：函数
来源：http://dsb.0kj1m.cn

function add(a, b) return a + b end
来源：http://vrh.hcnkem.com

[T37] Lua：字符串拼接
来源：http://lix.xingfuxueyuan.xyz

"a" .. "b"
来源：http://eca.aibaodan.cn

[T38] Lua：条件
来源：http://mfa.jqgfzy.top

if x > 0 then print("正") end
来源：http://bxk.jiagoushi.top

[T39] Lua：模式匹配
来源：http://ifz.yueranfly.top

string.find(s, "%d+")
来源：http://bkx.wangshuangyany.cn

[T40] Lua：元表
来源：http://epa.aizwys.cn

setmetatable({}, { __index = base })
来源：http://suv.havefunace.top

[T41] Perl：Hello World
来源：http://klr.zhixingplan.top

print "Hello\n";
来源：http://sly.ybcxt.top

[T42] Perl：变量类型
来源：http://ylt.haohaochexian.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qoy.yueranfly.top

[T43] Perl：字符串插值
来源：http://kxe.hesvh.cn

"值: $a"
来源：http://xsh.iojbl.cn

[T44] Perl：条件
来源：http://dgt.c1oappe.top

if ($a > 0) { print "正"; }
来源：http://dxj.gogol.net.cn

[T45] Perl：数组遍历
来源：http://cwj.jiagoushi.top

for my $x (@arr) { print $x; }
来源：http://vjb.epnwcf.com

[T46] Perl：哈希操作
来源：http://nkp.gaohongyu789.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://esy.feifeiyinyue.top

[T47] Perl：正则捕获
来源：http://hep.fehbvm.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://syl.iojbl.cn

[T48] Perl：正则替换
来源：http://vwg.cashguo.top

$s =~ s/old/new/g;
来源：http://ewn.52xcode.cn

[T49] Perl：函数
来源：http://ntt.snrcjt.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pek.hysaishi.cn

[T50] Perl：逐行读文件
来源：http://yub.tanke756.top

open my $fh, "<", "a.txt" or die $!;
来源：http://oei.jinqigfzy.top

while (my $line = <$fh>) { print $line; }
来源：http://jdi.sjlbkw.cn

[T51] Scala：Hello World
来源：http://fxt.redwolf501.top

println("Hello")
来源：http://fxd.ydjk.org.cn

[T52] Scala：变量
来源：http://alg.havefunace.top

val a = 1;  var b = 2
来源：http://blv.shangyingyoupin.top

[T53] Scala：字符串插值
来源：http://yky.nwbrower.top

s"值: $b"
来源：http://wfp.kuanghao11.cn

[T54] Scala：集合映射
来源：http://yjy.jlsjyb.cn

List(1, 2, 3).map(_ * 2)
来源：http://fcg.birdmap.top

[T55] Scala：集合过滤
来源：http://yds.ydzc1.top

List(1, 2, 3).filter(_ > 1)
来源：http://abl.shanyushiyangtech.top

[T56] Scala：样例类
来源：http://wtn.redwolf501.top

case class User(name: String, age: Int)
来源：http://oht.hcnkem.com

[T57] Scala：模式匹配
来源：http://qvo.hnxiangtu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://qrd.guowangkeji.top

[T58] Scala：函数定义
来源：http://nhh.aibaodan.cn

def add(a: Int, b: Int): Int = a + b
来源：http://eqj.zdbjq.cn

[T59] Scala：循环
来源：http://rxd.feifeiyinyue.top

for (i <- 1 to 10) println(i)
来源：http://mka.jianghu66.top

[T60] Scala：折叠
来源：http://fhq.jinyuanbaomall.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fpr.xuanzx.com

================================================================================
来源：http://ypp.gzhubu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://che.fktsv.cn

================================================================================
来源：http://vyf.bbcook.cn

[U01] Py：创建虚拟环境
来源：http://ymw.hongshengwenyu.top

python -m venv .venv && source .venv/bin/activate
来源：http://bap.gotoacloud.top

[U02] Py：导出 / 安装依赖
来源：http://wso.jqgufenzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zqr.fktsv.cn

[U03] Py：加载 .env 配置
来源：http://lqb.zdqjudy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://sbc.jlsjyb.cn

[U04] Py：变量调试打印
来源：http://iuq.cashguo.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lnw.cucudq.cn

[U05] Py：列表去重且保序
来源：http://sox.bbcook.cn

list(dict.fromkeys(arr))
来源：http://ffo.ydzc1.top

[U06] Py：合并两个字典
来源：http://sbh.zhaomingkeji.xyz

{**a, **b}
来源：http://aia.gzhubu.top

[U07] Py：反转字典键值
来源：http://mew.vqdsnc.cn

{v: k for k, v in d.items()}
来源：http://tfa.hfpthk.cn

[U08] Py：展平二维列表
来源：http://lsl.yj202588.top

[y for x in nested for y in x]
来源：http://ney.daxiang520.top

[U09] Py：字典取最大值的键
来源：http://htl.zhengqikj.top

max(d, key=d.get)
来源：http://wjo.yongpay.top

[U10] Py：按值排序字典
来源：http://jsm.daria6918.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uud.shanyushiyangtech.top

[U11] Py：生成器表达式
来源：http://txk.yj202588.top

(x * 2 for x in arr)
来源：http://ntm.shuidangran.top

[U12] Py：取出现最多的 3 个元素
来源：http://vlz.svipenyu.cn

Counter(arr).most_common(3)
来源：http://oyj.shangyingyoupin.top

[U13] Py：固定长度队列
来源：http://pxw.316326.xyz

deque(maxlen=10)
来源：http://efn.svipenyu.cn

[U14] Py：分组收集到列表
来源：http://sjm.yuanzhike.top

defaultdict(list)
来源：http://adp.dianchejie.cn

[U15] Py：高精度计时
来源：http://kfr.kuanghao11.cn

t = time.perf_counter()
来源：http://zre.zhijiandao.cn

[U16] Py：命令行参数解析
来源：http://dyw.xziqi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nja.xylfe.cn

[U17] Py：初始化日志
来源：http://uhz.wangdashe.top

logging.basicConfig(level=logging.INFO)
来源：http://drh.zhiwuduotai.top

[U18] Py：预编译正则
来源：http://avo.snrcjt.cn

pat = re.compile(r"\d+")
来源：http://ipj.ydjk.org.cn

[U19] Py：正则替换带回调
来源：http://rfd.sufxvd.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vae.jinqigufen.top

[U20] Py：缓存函数结果
来源：http://ibg.dashuyun.cn

@functools.lru_cache(maxsize=None)
来源：http://ywu.yfazqb.com

[U21] Py：自定义上下文管理器
来源：http://oij.gotoacloud.top

@contextlib.contextmanager
来源：http://ovb.cqqwz.cn

[U22] Py：矩阵转置
来源：http://wmy.zhengqikj.top

list(zip(*m))
来源：http://gge.cqqwz.cn

[U23] Py：分块读取大文件
来源：http://dys.fengsongda.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wdq.jinghuilouyu.cn

[U24] Py：路径操作
来源：http://kta.chenlongwang.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dai.zhiwuduotai.top

[U25] Py：CSV 按字典读
来源：http://cmp.fktsv.cn

csv.DictReader(f)
来源：http://kgd.wangshuangyany.cn

[U26] Py：并发下载
来源：http://ndf.tanke756.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://udw.tarul.cn

[U27] Py：异步 HTTP
来源：http://inw.gzhubu.top

aiohttp.ClientSession() 配合 async with
来源：http://iqf.gogol.net.cn

[U28] Py：类型别名
来源：http://dpl.yongpay.top

UserId = int
来源：http://gja.haohaochexian.top

[U29] Py：属性校验
来源：http://dbn.ehwqpu.com

@property 与 @x.setter 配合
来源：http://fbc.fehbvm.com

[U30] Py：数据类
来源：http://pvz.sxryk.cn

@dataclass(slots=True)
来源：http://vur.tian-w.cn

[U31] Py：单测
来源：http://dzx.yuanzhike.top

python -m pytest -q
来源：http://fax.cucudq.cn

[U32] Py：代码格式化
来源：http://iad.hysaishi.cn

ruff format . && ruff check --fix .
来源：http://orq.zycfv.cn

[U33] Py：打包发布
来源：http://ekb.0kj1m.cn

python -m build  （依赖 pyproject.toml）
来源：http://qkl.xziqi.cn

[U34] Py：判断编码
来源：http://yty.aibaodan.cn

chardet.detect(raw)
来源：http://zkw.aibaodan.cn

[U35] Py：发送邮件
来源：http://uro.316326.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dqw.kuanghao11.cn

[U36] Py：定时任务
来源：http://opc.jiagoushi.top

schedule.every(10).minutes.do(job)
来源：http://acw.jiagoushi.top

[U37] Py：读写 Excel
来源：http://rej.zycfv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vjj.316326.xyz

[U38] Py：获取脚本所在目录
来源：http://wep.ydzc1.top

Path(__file__).resolve().parent
来源：http://axd.c1oappe.top

[U39] Py：判断是否在交互环境
来源：http://wlj.quarkkingdee.top

sys.stdout.isatty()
来源：http://tnn.mhx1999.top

[U40] Py：打印到标准错误
来源：http://syn.svipenyu.cn

print("err", file=sys.stderr)
来源：http://wvn.jinqigufen.top

[U41] PHP：初始化 Composer 项目
来源：http://ofx.xylfe.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ynn.mhx1999.top

[U42] PHP：PSR-4 自动加载
来源：http://hnx.cqqwz.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hfa.shanyushiyangtech.top

[U43] PHP：声明命名空间
来源：http://agl.sysykeji.top

namespace App\Http;
来源：http://tco.vqdsnc.cn

[U44] PHP：开启严格类型
来源：http://wsl.zdbjq.cn

declare(strict_types=1);
来源：http://pli.316326.xyz

[U45] PHP：类型声明与返回类型
来源：http://owe.fktsv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uvp.ehwqpu.com

[U46] PHP：可空类型
来源：http://crv.yueranfly.top

?string $name = null
来源：http://hgy.quarkkingdee.top

[U47] PHP：联合类型
来源：http://ygk.ctjpmb.com

int|string $id
来源：http://skd.shuidangran.top

[U48] PHP：纯枚举
来源：http://aft.jinyuanbaomall.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ekp.bbcook.cn

[U49] PHP：只读属性
来源：http://tur.cdnleiting.top

public readonly string $name
来源：http://exv.yj202588.top

[U50] PHP：构造器属性提升
来源：http://wps.hnxiangtu.top

public function __construct(private int $id) {}
来源：http://qlg.wangshuangyany.cn

[U51] PHP：数组解构
来源：http://olp.svipenyu.cn

[$a, $b] = $arr;
来源：http://kjz.meibo888.top

[U52] PHP：箭头函数
来源：http://pci.sxryk.cn

$double = fn($x) => $x * 2;
来源：http://vnb.zhaomingkeji.xyz

[U53] PHP：空合并运算符
来源：http://alz.xylfe.cn

$v = $a ?? $b ?? "default";
来源：http://nva.c1oappe.top

[U54] PHP：空安全调用
来源：http://kkh.chenzaomai.com

$obj?->method()
来源：http://zpv.jqgfzy.top

[U55] PHP：match 表达式
来源：http://ggk.jinqigfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://oom.daxiang520.top

[U56] PHP：命名参数
来源：http://ktt.smart0.xyz

f(a: 1, b: 2)
来源：http://ywq.ywan-chungtsiang.top

[U57] PHP：字符串插值
来源：http://dfb.andypj.xyz

"值: {$a}"
来源：http://ytw.xuetiantiany.cn

[U58] PHP：数组三件套
来源：http://ugv.ivvv.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://aey.epnwcf.com

[U59] PHP：自定义排序
来源：http://xwo.pengpengdd.cyou

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ocm.bjfxy.top

[U60] PHP：JSON 编解码
来源：http://cxr.jiagoushi.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kpz.tianlin.xyz

[U61] PHP：正则
来源：http://oty.yangfankeji.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xqk.zhijiandao.cn

[U62] PHP：日期对象
来源：http://cep.tianlin.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rif.epnwcf.com

[U63] PHP：文件读写
来源：http://jkd.0kj1m.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gkg.uphjek.com

[U64] PHP：目录遍历
来源：http://zma.jiagoushi.top

glob("dir/*.php");  scandir("dir");
来源：http://imz.hnqzz.top

[U65] PHP：会话
来源：http://cut.fehbvm.com

session_start();  $_SESSION["uid"] = 1;
来源：http://gto.aizwys.cn

[U66] PHP：设置 Cookie
来源：http://pyc.dianchejie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uou.yueranfly.top

[U67] PHP：处理文件上传
来源：http://psm.dashuyun.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dhc.ywan-chungtsiang.top

[U68] PHP：PDO 连接
来源：http://caw.wangshuangyany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qql.cdnleiting.top


<!-- 参考信息 -->