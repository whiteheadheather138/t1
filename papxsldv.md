代发 wailian999

[S39] C++：自定义比较器排序
来源：http://ufb.jlsjyb.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fbx.chenzaomai.com

[S40] C++：查找元素
来源：http://imv.sxryk.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pqs.havefunace.top

[S41] C++：类与构造函数
来源：http://qoz.cashguo.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bsd.hammf.cn

[S42] C++：继承与虚函数
来源：http://xmn.zhaomingkeji.xyz

class B : public Base { public: void f() override {} };
来源：http://tha.chenjidiqi.icu

[S43] C++：智能指针
来源：http://jwg.ctjpmb.com

auto p = std::make_unique<int>(5);
来源：http://wad.yuxming.cn

[S44] C++：引用传参
来源：http://uex.jiagoushi.top

void inc(int &x) { ++x; }
来源：http://ddr.jqgfzy.top

[S45] C++：lambda
来源：http://zxw.bbcook.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yri.gogol.net.cn

[S46] C++：函数模板
来源：http://odc.gogol.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ytw.shanyushiyangkeji.top

[S47] C++：结构化绑定遍历
来源：http://smi.sjlbkw.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://poo.shangyingyoupin.top

[S48] C++：逐行读文件
来源：http://jkn.gogol.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://iit.yj20258888.top

while (std::getline(in, line)) { }
来源：http://wyo.ivvv.top

[S49] C++：写文件
来源：http://zyv.tian-w.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hvw.yongpay.top

[S50] C++：格式化数字
来源：http://obg.xylfe.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jus.jyoumei.cn

[S51] C++：显式类型转换
来源：http://tjk.yuanzhike.top

static_cast<double>(a) / b
来源：http://hlf.nwbrower.top

[S52] C++：const 与 noexcept
来源：http://jab.yj20258888.top

int size() const noexcept { return n_; }
来源：http://tkk.guowangkeji.top

[S53] C++：移动语义
来源：http://gnw.hfpthk.cn

std::vector<int> w = std::move(v);
来源：http://vmx.jlsjyb.cn

[S54] C++：异常处理
来源：http://acq.yuanzhike.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kro.yueranfly.top

[S55] C++：结构化绑定
来源：http://uvt.mhx1999.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vog.xingfuxueyuan.xyz

[S56] C++：optional
来源：http://puk.wangshuangyany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://voy.ehwqpu.com

[S57] C++：编译期常量
来源：http://ant.hysaishi.cn

constexpr int N = 10;
来源：http://uca.zhiwuduotai.top

[S58] C++：命名空间
来源：http://alh.chenjidiqi.icu

namespace ns { int f() { return 1; } }
来源：http://yjf.fehbvm.com

[S59] C++：静态断言
来源：http://pvz.nanxinkj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://etd.cqqwz.cn

[S60] C++：遍历并删除元素
来源：http://odq.zdbjq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vmp.redwolf501.top

================================================================================
来源：http://eas.hcnkem.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nhy.yongpay.top

================================================================================
来源：http://knd.xuanzx.com

[T01] Kotlin：Hello World
来源：http://coh.kuanghao11.cn

println("Hello")
来源：http://tzq.redwolf501.top

[T02] Kotlin：变量
来源：http://lkg.sweek.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fki.havefunace.top

[T03] Kotlin：字符串模板
来源：http://tnc.aibaodan.cn

"值: $b"
来源：http://jnn.epnwcf.com

[T04] Kotlin：空安全
来源：http://zdd.xuetiantiany.cn

val n: String? = null;  n?.length
来源：http://fwy.zdbjq.cn

[T05] Kotlin：when 表达式
来源：http://ktc.ctjpmb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wkq.redwolf501.top

[T06] Kotlin：集合映射
来源：http://moj.aizwys.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nnb.ybcxt.top

[T07] Kotlin：集合过滤
来源：http://aad.snrcjt.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wac.sjlbkw.cn

[T08] Kotlin：数据类
来源：http://zgl.jinqigufen.top

data class User(val name: String, val age: Int)
来源：http://ezo.vqdsnc.cn

[T09] Kotlin：扩展函数
来源：http://mlu.shanyushiyangkeji.top

fun String.exclaim() = this + "!"
来源：http://pph.havefunace.top

[T10] Kotlin：默认参数
来源：http://iux.zhixingplan.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gmr.hesvh.cn

[T11] Kotlin：协程
来源：http://jjy.yfazqb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://sae.ehwqpu.com

[T12] Kotlin：解构声明
来源：http://tfm.yj202588.top

val (a, b) = Pair(1, 2)
来源：http://mxu.redwolf501.top

[T13] Kotlin：只读 Map
来源：http://xks.tianlin.xyz

val m = mapOf("a" to 1)
来源：http://kle.tarul.cn

[T14] Kotlin：循环
来源：http://qwn.xingfuxueyuan.xyz

for (i in 1..10) println(i)
来源：http://vee.zhongyouzk.top

[T15] Kotlin：接口
来源：http://sfr.yanxiufei.cn

interface Shape { fun area(): Double }
来源：http://jov.ydjk.org.cn

[T16] Swift：Hello World
来源：http://xrj.jinqigfzy.top

print("Hello")
来源：http://vys.cucudq.cn

[T17] Swift：变量与常量
来源：http://abq.chenzaomai.com

var a = 1;  let b = 2
来源：http://wpl.mhx1999.top

[T18] Swift：字符串插值
来源：http://ard.jqgfzy.top

"值: \(b)"
来源：http://jax.gogol.net.cn

[T19] Swift：可选绑定
来源：http://psw.redwolf501.top

if let n = opt { print(n) }
来源：http://fjj.wangshuangyany.cn

[T20] Swift：数组操作
来源：http://hup.zdqjudy.top

var a = [1, 2, 3];  a.append(4)
来源：http://qcw.fehbvm.com

[T21] Swift：遍历
来源：http://mvv.gaohongyu789.top

for x in a { print(x) }
来源：http://ayz.shzxlz.cn

[T22] Swift：字典
来源：http://uqb.quarkkingdee.top

var d = ["a": 1];  d["b"] = 2
来源：http://vdh.jqgufenzy.top

[T23] Swift：函数
来源：http://ito.zhengqikj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vnp.jinyuanbaomall.cn

[T24] Swift：闭包
来源：http://lft.vehdjk.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://nsz.fengsongda.top

[T25] Swift：结构体
来源：http://bvl.snrcjt.cn

struct P { var x: Int }
来源：http://hrk.bjfxy.top

[T26] Swift：类与重写
来源：http://kff.ehwqpu.com

class A: Base { override func f() {} }
来源：http://per.feifeiyinyue.top

[T27] Swift：错误处理
来源：http://gwi.yuxming.cn

do { try f() } catch { print(error) }
来源：http://mrj.gotoacloud.top

[T28] Swift：枚举
来源：http://pch.xinyue.icu

enum Color { case red, green }
来源：http://ncj.tian-w.cn

[T29] Swift：guard 提前返回
来源：http://ktp.0kj1m.cn

guard let x = opt else { return }
来源：http://wtv.shanyushiyangkeji.top

[T30] Swift：协议
来源：http://kkg.ctjpmb.com

protocol Shape { func area() -> Double }
来源：http://kms.sweek.top

[T31] Lua：Hello World
来源：http://vzr.bjfxy.top

print("Hello")
来源：http://dup.jyoumei.cn

[T32] Lua：局部变量
来源：http://fvq.cqqwz.cn

local a = 1
来源：http://zfl.nanxuanxn.top

[T33] Lua：表（数组）
来源：http://gmx.tarul.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yeh.nanxuanxn.top

[T34] Lua：遍历表
来源：http://uam.zhijiandao.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rrk.sweek.top

[T35] Lua：字典表
来源：http://rdk.aibaodan.cn

local d = { a = 1 };  d.b = 2
来源：http://wxk.cdnleiting.top

[T36] Lua：函数
来源：http://xwm.shzxlz.cn

function add(a, b) return a + b end
来源：http://vzi.hesvh.cn

[T37] Lua：字符串拼接
来源：http://fvm.zdbjq.cn

"a" .. "b"
来源：http://jes.ctjpmb.com

[T38] Lua：条件
来源：http://usr.c1oappe.top

if x > 0 then print("正") end
来源：http://dfh.ctjpmb.com

[T39] Lua：模式匹配
来源：http://ftx.hcnkem.com

string.find(s, "%d+")
来源：http://eka.xziqi.cn

[T40] Lua：元表
来源：http://gph.kuanghao11.cn

setmetatable({}, { __index = base })
来源：http://cjc.fengsongda.top

[T41] Perl：Hello World
来源：http://gwx.ppjwa.cn

print "Hello\n";
来源：http://dst.quarkkingdee.top

[T42] Perl：变量类型
来源：http://kxn.jianghu66.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pai.zycfv.cn

[T43] Perl：字符串插值
来源：http://tzy.tian-w.cn

"值: $a"
来源：http://nwp.daxiang520.top

[T44] Perl：条件
来源：http://vol.shzxlz.cn

if ($a > 0) { print "正"; }
来源：http://hak.uphjek.com

[T45] Perl：数组遍历
来源：http://gnn.daria6918.cn

for my $x (@arr) { print $x; }
来源：http://dcx.sjlbkw.cn

[T46] Perl：哈希操作
来源：http://cgs.bjfxy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mpl.tianlin.xyz

[T47] Perl：正则捕获
来源：http://wlk.fzhhl.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://igv.jqgfzy.top

[T48] Perl：正则替换
来源：http://yfz.cucudq.cn

$s =~ s/old/new/g;
来源：http://zdh.shuidangran.top

[T49] Perl：函数
来源：http://xfu.guowangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zkr.ywan-chungtsiang.top

[T50] Perl：逐行读文件
来源：http://jwa.0kj1m.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://odm.cucudq.cn

while (my $line = <$fh>) { print $line; }
来源：http://fwn.birdmap.top

[T51] Scala：Hello World
来源：http://mlj.jyoumei.cn

println("Hello")
来源：http://udz.gogol.net.cn

[T52] Scala：变量
来源：http://kkb.0kj1m.cn

val a = 1;  var b = 2
来源：http://xbn.daxiang520.top

[T53] Scala：字符串插值
来源：http://bdr.gogol.net.cn

s"值: $b"
来源：http://sxm.ydjk.org.cn

[T54] Scala：集合映射
来源：http://exe.hongshengwenyu.top

List(1, 2, 3).map(_ * 2)
来源：http://lgv.jlsjyb.cn

[T55] Scala：集合过滤
来源：http://qai.jinqigfzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://npz.aizwys.cn

[T56] Scala：样例类
来源：http://tme.chenlongwang.top

case class User(name: String, age: Int)
来源：http://ysr.nanxuanxn.top

[T57] Scala：模式匹配
来源：http://qfl.mhx1999.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fbg.ywan-chungtsiang.top

[T58] Scala：函数定义
来源：http://wsj.guowangkeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://upn.yvedp.cn

[T59] Scala：循环
来源：http://djs.hcnkem.com

for (i <- 1 to 10) println(i)
来源：http://sel.shuidangran.top

[T60] Scala：折叠
来源：http://sox.shuidangran.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fpc.xinyue.icu

================================================================================
来源：http://wlw.xinyue.icu

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ghf.jinqigufen.top

================================================================================
来源：http://tet.mhx1999.top

[U01] Py：创建虚拟环境
来源：http://sys.zhijiandao.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gfx.nanxinkj.top

[U02] Py：导出 / 安装依赖
来源：http://aob.gaohongyu789.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zgl.quarkkingdee.top

[U03] Py：加载 .env 配置
来源：http://sij.ydzc1.top

from dotenv import load_dotenv; load_dotenv()
来源：http://upb.cdnleiting.top

[U04] Py：变量调试打印
来源：http://jge.smart0.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lls.nanxuanxn.top

[U05] Py：列表去重且保序
来源：http://zpd.fanxiaobao.xyz

list(dict.fromkeys(arr))
来源：http://fom.hesvh.cn

[U06] Py：合并两个字典
来源：http://zjs.yangfankeji.com

{**a, **b}
来源：http://plw.chenzaomai.com

[U07] Py：反转字典键值
来源：http://jhs.zhoulong.xyz

{v: k for k, v in d.items()}
来源：http://gln.yfazqb.com

[U08] Py：展平二维列表
来源：http://vgj.shzxlz.cn

[y for x in nested for y in x]
来源：http://far.zdbjq.cn

[U09] Py：字典取最大值的键
来源：http://nts.yonumen.top

max(d, key=d.get)
来源：http://yjn.shuidangran.top

[U10] Py：按值排序字典
来源：http://lyg.hammf.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bvm.hfpthk.cn

[U11] Py：生成器表达式
来源：http://dad.fehbvm.com

(x * 2 for x in arr)
来源：http://vsz.bjfxy.top

[U12] Py：取出现最多的 3 个元素
来源：http://clv.jinghuilouyu.cn

Counter(arr).most_common(3)
来源：http://hdb.hcnkem.com

[U13] Py：固定长度队列
来源：http://auf.andypj.xyz

deque(maxlen=10)
来源：http://hsn.daria6918.cn

[U14] Py：分组收集到列表
来源：http://dpv.bjfxy.top

defaultdict(list)
来源：http://wkd.yvedp.cn

[U15] Py：高精度计时
来源：http://fyz.aizwys.cn

t = time.perf_counter()
来源：http://vzg.yuanzhike.top

[U16] Py：命令行参数解析
来源：http://nte.kuanghao11.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fnh.nanxuanxn.top

[U17] Py：初始化日志
来源：http://tsv.hongshengwenyu.top

logging.basicConfig(level=logging.INFO)
来源：http://rhe.jqgufenzy.top

[U18] Py：预编译正则
来源：http://vcn.cqqwz.cn

pat = re.compile(r"\d+")
来源：http://fak.svipenyu.cn

[U19] Py：正则替换带回调
来源：http://gxi.hongshengwenyu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ntv.ehwqpu.com

[U20] Py：缓存函数结果
来源：http://igo.shanyushiyangtech.top

@functools.lru_cache(maxsize=None)
来源：http://rbs.chenjidiqi.icu

[U21] Py：自定义上下文管理器
来源：http://umj.jyoumei.cn

@contextlib.contextmanager
来源：http://xnd.yj20258.top

[U22] Py：矩阵转置
来源：http://iqq.shanyushiyangkeji.top

list(zip(*m))
来源：http://zzg.jlsjyb.cn

[U23] Py：分块读取大文件
来源：http://jrt.fanxiaobao.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://whh.andypj.xyz

[U24] Py：路径操作
来源：http://iky.zhixingplan.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lhf.gzhubu.top

[U25] Py：CSV 按字典读
来源：http://vmi.snrcjt.cn

csv.DictReader(f)
来源：http://kca.epnwcf.com

[U26] Py：并发下载
来源：http://qgw.fengsongda.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wbf.52xcode.cn

[U27] Py：异步 HTTP
来源：http://cky.jyoumei.cn

aiohttp.ClientSession() 配合 async with
来源：http://cga.pengpengdd.cyou

[U28] Py：类型别名
来源：http://mio.aibaodan.cn

UserId = int
来源：http://fju.jiagoushi.top

[U29] Py：属性校验
来源：http://ghs.sxryk.cn

@property 与 @x.setter 配合
来源：http://dxw.dianchejie.cn

[U30] Py：数据类
来源：http://unq.xziqi.cn

@dataclass(slots=True)
来源：http://dnk.yueranfly.top

[U31] Py：单测
来源：http://qnv.cashguo.top

python -m pytest -q
来源：http://wdj.ydzc1.top

[U32] Py：代码格式化
来源：http://ouk.redwolf501.top

ruff format . && ruff check --fix .
来源：http://rir.vehdjk.com

[U33] Py：打包发布
来源：http://seg.fengsongda.top

python -m build  （依赖 pyproject.toml）
来源：http://wmc.zhaomingkeji.xyz

[U34] Py：判断编码
来源：http://fjg.sweek.top

chardet.detect(raw)
来源：http://qfk.jqgfzy.top

[U35] Py：发送邮件
来源：http://oza.nanxinkj.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ral.cheryme.top

[U36] Py：定时任务
来源：http://aqj.chenlongwang.top

schedule.every(10).minutes.do(job)
来源：http://wxn.xuanzx.com

[U37] Py：读写 Excel
来源：http://gmb.iojbl.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fbf.smart0.xyz

[U38] Py：获取脚本所在目录
来源：http://gil.xinyue.icu

Path(__file__).resolve().parent
来源：http://ycw.tarul.cn

[U39] Py：判断是否在交互环境
来源：http://dzg.pycfn.com

sys.stdout.isatty()
来源：http://ruc.hfpthk.cn

[U40] Py：打印到标准错误
来源：http://ywp.fktsv.cn

print("err", file=sys.stderr)
来源：http://lyv.sjlbkw.cn

[U41] PHP：初始化 Composer 项目
来源：http://dft.feifeiyinyue.top

composer init;  composer require guzzlehttp/guzzle
来源：http://scg.nanxinkj.top

[U42] PHP：PSR-4 自动加载
来源：http://sjx.sysykeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ihr.vqdsnc.cn

[U43] PHP：声明命名空间
来源：http://urq.xylfe.cn

namespace App\Http;
来源：http://hug.yangfankeji.com

[U44] PHP：开启严格类型
来源：http://ion.vqdsnc.cn

declare(strict_types=1);
来源：http://zss.shuidangran.top

[U45] PHP：类型声明与返回类型
来源：http://wvq.jyoumei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gvb.havefunace.top

[U46] PHP：可空类型
来源：http://nox.ywan-chungtsiang.top

?string $name = null
来源：http://bqh.jinghuilouyu.cn

[U47] PHP：联合类型
来源：http://urs.316326.xyz

int|string $id
来源：http://nyw.haohaochexian.top

[U48] PHP：纯枚举
来源：http://ejr.dianchejie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cze.yonumen.top

[U49] PHP：只读属性
来源：http://unk.sysykeji.top

public readonly string $name
来源：http://tys.uphjek.com

[U50] PHP：构造器属性提升
来源：http://uui.316326.xyz

public function __construct(private int $id) {}
来源：http://npl.cucudq.cn

[U51] PHP：数组解构
来源：http://myn.birdmap.top

[$a, $b] = $arr;
来源：http://hdb.sysykeji.top

[U52] PHP：箭头函数
来源：http://dbb.shangyingyoupin.top

$double = fn($x) => $x * 2;
来源：http://csp.jqgufenzy.top

[U53] PHP：空合并运算符
来源：http://lnv.fengsongda.top

$v = $a ?? $b ?? "default";
来源：http://pql.daxiang520.top

[U54] PHP：空安全调用
来源：http://kwn.tanke756.top

$obj?->method()
来源：http://tkh.daxiang520.top

[U55] PHP：match 表达式
来源：http://cgj.vqdsnc.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cmo.chenlongwang.top

[U56] PHP：命名参数
来源：http://rcm.epnwcf.com

f(a: 1, b: 2)
来源：http://kbk.xuetiantiany.cn

[U57] PHP：字符串插值
来源：http://tmz.xuanzx.com

"值: {$a}"
来源：http://sxm.xinyue.icu

[U58] PHP：数组三件套
来源：http://meb.gzhubu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pnw.c1oappe.top

[U59] PHP：自定义排序
来源：http://wbb.shanyushiyangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aki.tianlin.xyz

[U60] PHP：JSON 编解码
来源：http://fyn.chenzaomai.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uxg.andypj.xyz

[U61] PHP：正则
来源：http://dyb.shzxlz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sed.hnxiangtu.top

[U62] PHP：日期对象
来源：http://guv.cheryme.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ulu.hongshengwenyu.top

[U63] PHP：文件读写
来源：http://eed.feifeiyinyue.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://goa.vqdsnc.cn

[U64] PHP：目录遍历
来源：http://yne.zhijiandao.cn

glob("dir/*.php");  scandir("dir");
来源：http://lkx.pycfn.com


<!-- 参考信息 -->