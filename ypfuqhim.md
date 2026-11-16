代发 wailian999

[S45] C++：lambda
来源：http://rvl.pengpengdd.cyou

auto add = [](int a, int b) { return a + b; };
来源：http://pym.cqqwz.cn

[S46] C++：函数模板
来源：http://ail.guowangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jci.shuidangran.top

[S47] C++：结构化绑定遍历
来源：http://hld.yuxming.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xhb.jyoumei.cn

[S48] C++：逐行读文件
来源：http://fem.quarkkingdee.top

std::ifstream in("a.txt");  std::string line;
来源：http://rnz.yueranfly.top

while (std::getline(in, line)) { }
来源：http://qdk.guowangkeji.top

[S49] C++：写文件
来源：http://iqr.tarul.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://amp.yuxming.cn

[S50] C++：格式化数字
来源：http://zmi.ehwqpu.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xqt.smart0.xyz

[S51] C++：显式类型转换
来源：http://vua.hammf.cn

static_cast<double>(a) / b
来源：http://oxu.iojbl.cn

[S52] C++：const 与 noexcept
来源：http://sga.ppjwa.cn

int size() const noexcept { return n_; }
来源：http://lij.yfazqb.com

[S53] C++：移动语义
来源：http://kdy.yueranfly.top

std::vector<int> w = std::move(v);
来源：http://tpt.tianlin.xyz

[S54] C++：异常处理
来源：http://npw.hongshengwenyu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://iwg.fzhhl.top

[S55] C++：结构化绑定
来源：http://irg.cashguo.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dph.fzhhl.top

[S56] C++：optional
来源：http://sph.redwolf501.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dbz.cdnleiting.top

[S57] C++：编译期常量
来源：http://nsr.hnqzz.top

constexpr int N = 10;
来源：http://xlz.zhiwuduotai.top

[S58] C++：命名空间
来源：http://yqj.epnwcf.com

namespace ns { int f() { return 1; } }
来源：http://tgg.zhixingplan.top

[S59] C++：静态断言
来源：http://oex.0kj1m.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://biq.ivvv.top

[S60] C++：遍历并删除元素
来源：http://huw.sxryk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zgl.hammf.cn

================================================================================
来源：http://dty.cdnleiting.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hes.bbcook.cn

================================================================================
来源：http://yii.redwolf501.top

[T01] Kotlin：Hello World
来源：http://dpw.zycfv.cn

println("Hello")
来源：http://kbj.tanke756.top

[T02] Kotlin：变量
来源：http://tla.wangdashe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tpa.birdmap.top

[T03] Kotlin：字符串模板
来源：http://kum.jinghuilouyu.cn

"值: $b"
来源：http://vmu.yangfankeji.com

[T04] Kotlin：空安全
来源：http://sxx.tanke756.top

val n: String? = null;  n?.length
来源：http://ene.hongshengwenyu.top

[T05] Kotlin：when 表达式
来源：http://rch.yanxiufei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kbe.havefunace.top

[T06] Kotlin：集合映射
来源：http://rqw.hnqzz.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dzh.dashuyun.cn

[T07] Kotlin：集合过滤
来源：http://gds.cdnleiting.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kdl.sjlbkw.cn

[T08] Kotlin：数据类
来源：http://esx.fehbvm.com

data class User(val name: String, val age: Int)
来源：http://mmj.chenlongwang.top

[T09] Kotlin：扩展函数
来源：http://hel.pengpengdd.cyou

fun String.exclaim() = this + "!"
来源：http://hcj.zdqjudy.top

[T10] Kotlin：默认参数
来源：http://fvn.gogol.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sii.dianchejie.cn

[T11] Kotlin：协程
来源：http://jpx.sweek.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://aqv.aibaodan.cn

[T12] Kotlin：解构声明
来源：http://ihb.iojbl.cn

val (a, b) = Pair(1, 2)
来源：http://tsf.hywenlv.cn

[T13] Kotlin：只读 Map
来源：http://grf.aibaodan.cn

val m = mapOf("a" to 1)
来源：http://rwf.hammf.cn

[T14] Kotlin：循环
来源：http://hcm.dianchejie.cn

for (i in 1..10) println(i)
来源：http://udt.hesvh.cn

[T15] Kotlin：接口
来源：http://eke.jyoumei.cn

interface Shape { fun area(): Double }
来源：http://pym.pycfn.com

[T16] Swift：Hello World
来源：http://lbd.aibaodan.cn

print("Hello")
来源：http://rxn.yj20258.top

[T17] Swift：变量与常量
来源：http://ljf.cheryme.top

var a = 1;  let b = 2
来源：http://yce.bjfxy.top

[T18] Swift：字符串插值
来源：http://tuw.pengpengdd.cyou

"值: \(b)"
来源：http://qym.gotoacloud.top

[T19] Swift：可选绑定
来源：http://pwz.epnwcf.com

if let n = opt { print(n) }
来源：http://qxs.ehwqpu.com

[T20] Swift：数组操作
来源：http://ppd.epnwcf.com

var a = [1, 2, 3];  a.append(4)
来源：http://twe.tanke756.top

[T21] Swift：遍历
来源：http://iqa.zhixingplan.top

for x in a { print(x) }
来源：http://jrd.snrcjt.cn

[T22] Swift：字典
来源：http://cxv.redwolf501.top

var d = ["a": 1];  d["b"] = 2
来源：http://cqn.hesvh.cn

[T23] Swift：函数
来源：http://duu.daxiang520.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kfw.jinqigufen.top

[T24] Swift：闭包
来源：http://lje.jyoumei.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qgq.redwolf501.top

[T25] Swift：结构体
来源：http://zwt.hcnkem.com

struct P { var x: Int }
来源：http://xnc.jlsjyb.cn

[T26] Swift：类与重写
来源：http://equ.cqqwz.cn

class A: Base { override func f() {} }
来源：http://lbm.hongshengwenyu.top

[T27] Swift：错误处理
来源：http://mhk.yj20258888.top

do { try f() } catch { print(error) }
来源：http://afc.vqdsnc.cn

[T28] Swift：枚举
来源：http://ghq.yanxiufei.cn

enum Color { case red, green }
来源：http://igf.shzxlz.cn

[T29] Swift：guard 提前返回
来源：http://rwb.feifeiyinyue.top

guard let x = opt else { return }
来源：http://zth.nanxinkj.top

[T30] Swift：协议
来源：http://nsz.pengpengdd.cyou

protocol Shape { func area() -> Double }
来源：http://aah.316326.xyz

[T31] Lua：Hello World
来源：http://vyb.chenjidiqi.icu

print("Hello")
来源：http://xdz.pengpengdd.cyou

[T32] Lua：局部变量
来源：http://jyq.jinyuanbaomall.cn

local a = 1
来源：http://bup.jyoumei.cn

[T33] Lua：表（数组）
来源：http://akp.redwolf501.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ywm.ybcxt.top

[T34] Lua：遍历表
来源：http://ojj.aizwys.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vqf.snrcjt.cn

[T35] Lua：字典表
来源：http://oer.yj202588.top

local d = { a = 1 };  d.b = 2
来源：http://yye.316326.xyz

[T36] Lua：函数
来源：http://spr.ivvv.top

function add(a, b) return a + b end
来源：http://hqf.yanxiufei.cn

[T37] Lua：字符串拼接
来源：http://xmw.dianchejie.cn

"a" .. "b"
来源：http://jhu.cashguo.top

[T38] Lua：条件
来源：http://vca.jlsjyb.cn

if x > 0 then print("正") end
来源：http://nrt.dianchejie.cn

[T39] Lua：模式匹配
来源：http://edo.snrcjt.cn

string.find(s, "%d+")
来源：http://ujc.shzxlz.cn

[T40] Lua：元表
来源：http://dtv.chenjidiqi.icu

setmetatable({}, { __index = base })
来源：http://esc.sweek.top

[T41] Perl：Hello World
来源：http://yqq.uphjek.com

print "Hello\n";
来源：http://yka.tarul.cn

[T42] Perl：变量类型
来源：http://hcv.0kj1m.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oiw.ywan-chungtsiang.top

[T43] Perl：字符串插值
来源：http://nqv.vqdsnc.cn

"值: $a"
来源：http://tnc.jinqigufen.top

[T44] Perl：条件
来源：http://uex.jyoumei.cn

if ($a > 0) { print "正"; }
来源：http://xdf.jianghu66.top

[T45] Perl：数组遍历
来源：http://cmp.zhoulong.xyz

for my $x (@arr) { print $x; }
来源：http://ori.zhaomingkeji.xyz

[T46] Perl：哈希操作
来源：http://xpn.jlsjyb.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sio.ydjk.org.cn

[T47] Perl：正则捕获
来源：http://jaf.jianghu66.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zwv.316326.xyz

[T48] Perl：正则替换
来源：http://gco.vehdjk.com

$s =~ s/old/new/g;
来源：http://skr.xuetiantiany.cn

[T49] Perl：函数
来源：http://lof.fengsongda.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://trw.hammf.cn

[T50] Perl：逐行读文件
来源：http://zqv.nanxinkj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hhr.aizwys.cn

while (my $line = <$fh>) { print $line; }
来源：http://vbv.pengpengdd.cyou

[T51] Scala：Hello World
来源：http://hie.haohaochexian.top

println("Hello")
来源：http://ivd.mhx1999.top

[T52] Scala：变量
来源：http://xac.yj20258888.top

val a = 1;  var b = 2
来源：http://exk.tian-w.cn

[T53] Scala：字符串插值
来源：http://eks.xziqi.cn

s"值: $b"
来源：http://not.yj20258888.top

[T54] Scala：集合映射
来源：http://inu.havefunace.top

List(1, 2, 3).map(_ * 2)
来源：http://tun.ydzc1.top

[T55] Scala：集合过滤
来源：http://dtl.0kj1m.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qxt.fengsongda.top

[T56] Scala：样例类
来源：http://pqd.quarkkingdee.top

case class User(name: String, age: Int)
来源：http://pfx.gzhubu.top

[T57] Scala：模式匹配
来源：http://lep.shzxlz.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lxn.jinqigufen.top

[T58] Scala：函数定义
来源：http://rvy.yfazqb.com

def add(a: Int, b: Int): Int = a + b
来源：http://jjh.sysykeji.top

[T59] Scala：循环
来源：http://lch.hfpthk.cn

for (i <- 1 to 10) println(i)
来源：http://bdy.dashuyun.cn

[T60] Scala：折叠
来源：http://ssa.zycfv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://seq.jianghu66.top

================================================================================
来源：http://ows.ehwqpu.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tzv.shzxlz.cn

================================================================================
来源：http://yyt.fzhhl.top

[U01] Py：创建虚拟环境
来源：http://rwn.yj202588.top

python -m venv .venv && source .venv/bin/activate
来源：http://tnm.hnqzz.top

[U02] Py：导出 / 安装依赖
来源：http://bol.tanke756.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oju.meibo888.top

[U03] Py：加载 .env 配置
来源：http://vha.xingfuxueyuan.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://rgl.iojbl.cn

[U04] Py：变量调试打印
来源：http://mlt.9152youxi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sih.gzhubu.top

[U05] Py：列表去重且保序
来源：http://fvv.ppjwa.cn

list(dict.fromkeys(arr))
来源：http://imw.mhx1999.top

[U06] Py：合并两个字典
来源：http://kds.hfpthk.cn

{**a, **b}
来源：http://wsq.xziqi.cn

[U07] Py：反转字典键值
来源：http://tnc.fanxiaobao.xyz

{v: k for k, v in d.items()}
来源：http://txu.svipenyu.cn

[U08] Py：展平二维列表
来源：http://jmu.ydzc1.top

[y for x in nested for y in x]
来源：http://zvd.aizwys.cn

[U09] Py：字典取最大值的键
来源：http://lsv.bjfxy.top

max(d, key=d.get)
来源：http://hpg.meibo888.top

[U10] Py：按值排序字典
来源：http://wfx.aibaodan.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nea.cashguo.top

[U11] Py：生成器表达式
来源：http://xaq.pengpengdd.cyou

(x * 2 for x in arr)
来源：http://fto.316326.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://ywa.c1oappe.top

Counter(arr).most_common(3)
来源：http://psf.shangyingyoupin.top

[U13] Py：固定长度队列
来源：http://psz.xuetiantiany.cn

deque(maxlen=10)
来源：http://ksm.yj202588.top

[U14] Py：分组收集到列表
来源：http://cxs.gzhubu.top

defaultdict(list)
来源：http://nzb.hcnkem.com

[U15] Py：高精度计时
来源：http://ykw.mhx1999.top

t = time.perf_counter()
来源：http://xva.sxryk.cn

[U16] Py：命令行参数解析
来源：http://xay.hnqzz.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jxg.yangfankeji.com

[U17] Py：初始化日志
来源：http://hpl.ydzc1.top

logging.basicConfig(level=logging.INFO)
来源：http://aec.yvedp.cn

[U18] Py：预编译正则
来源：http://fxc.sxryk.cn

pat = re.compile(r"\d+")
来源：http://vat.iojbl.cn

[U19] Py：正则替换带回调
来源：http://vzg.yangfankeji.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hat.quarkkingdee.top

[U20] Py：缓存函数结果
来源：http://uww.ydjk.org.cn

@functools.lru_cache(maxsize=None)
来源：http://ayk.daria6918.cn

[U21] Py：自定义上下文管理器
来源：http://yvm.svipenyu.cn

@contextlib.contextmanager
来源：http://fpw.gzhubu.top

[U22] Py：矩阵转置
来源：http://qgy.cheryme.top

list(zip(*m))
来源：http://uot.cqqwz.cn

[U23] Py：分块读取大文件
来源：http://vvi.shuidangran.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tuv.yongpay.top

[U24] Py：路径操作
来源：http://kys.zdqjudy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fhw.quarkkingdee.top

[U25] Py：CSV 按字典读
来源：http://dei.hnxiangtu.top

csv.DictReader(f)
来源：http://wbq.chenlongwang.top

[U26] Py：并发下载
来源：http://mra.zycfv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://arn.hywenlv.cn

[U27] Py：异步 HTTP
来源：http://wdf.hcnkem.com

aiohttp.ClientSession() 配合 async with
来源：http://hzk.zhiwuduotai.top

[U28] Py：类型别名
来源：http://xhs.hfpthk.cn

UserId = int
来源：http://rwv.ydjk.org.cn

[U29] Py：属性校验
来源：http://buk.tanke756.top

@property 与 @x.setter 配合
来源：http://dwn.chenlongwang.top

[U30] Py：数据类
来源：http://stf.yangfankeji.com

@dataclass(slots=True)
来源：http://apk.yonumen.top

[U31] Py：单测
来源：http://kdw.guannengcc.top

python -m pytest -q
来源：http://itw.ydzc1.top

[U32] Py：代码格式化
来源：http://prb.zdqjudy.top

ruff format . && ruff check --fix .
来源：http://cqg.ydzc1.top

[U33] Py：打包发布
来源：http://agh.ybcxt.top

python -m build  （依赖 pyproject.toml）
来源：http://kur.cdnleiting.top

[U34] Py：判断编码
来源：http://zge.hesvh.cn

chardet.detect(raw)
来源：http://gcv.vqdsnc.cn

[U35] Py：发送邮件
来源：http://mah.smart0.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xbh.gaohongyu789.top

[U36] Py：定时任务
来源：http://cyz.zdbjq.cn

schedule.every(10).minutes.do(job)
来源：http://ojf.daxiang520.top

[U37] Py：读写 Excel
来源：http://eea.fzhhl.top

pandas.read_excel / DataFrame.to_excel
来源：http://qba.ehwqpu.com

[U38] Py：获取脚本所在目录
来源：http://bof.guannengcc.top

Path(__file__).resolve().parent
来源：http://yxf.jinqigufen.top

[U39] Py：判断是否在交互环境
来源：http://cdi.iojbl.cn

sys.stdout.isatty()
来源：http://vwj.svipenyu.cn

[U40] Py：打印到标准错误
来源：http://gbs.aizwys.cn

print("err", file=sys.stderr)
来源：http://lgi.xingfuxueyuan.xyz

[U41] PHP：初始化 Composer 项目
来源：http://oty.yongpay.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wby.tian-w.cn

[U42] PHP：PSR-4 自动加载
来源：http://gnr.andypj.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rfl.yuanzhike.top

[U43] PHP：声明命名空间
来源：http://icc.shanyushiyangtech.top

namespace App\Http;
来源：http://scf.jlsjyb.cn

[U44] PHP：开启严格类型
来源：http://rxt.316326.xyz

declare(strict_types=1);
来源：http://sgb.ivvv.top

[U45] PHP：类型声明与返回类型
来源：http://omy.yongpay.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://yiy.shangyingyoupin.top

[U46] PHP：可空类型
来源：http://zna.feifeiyinyue.top

?string $name = null
来源：http://qsw.zhiwuduotai.top

[U47] PHP：联合类型
来源：http://qgb.yj20258888.top

int|string $id
来源：http://dyc.sxryk.cn

[U48] PHP：纯枚举
来源：http://ipo.chenjidiqi.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://evv.feifeiyinyue.top

[U49] PHP：只读属性
来源：http://yyj.feifeiyinyue.top

public readonly string $name
来源：http://bhq.yonumen.top

[U50] PHP：构造器属性提升
来源：http://ulh.vehdjk.com

public function __construct(private int $id) {}
来源：http://xaq.mhx1999.top

[U51] PHP：数组解构
来源：http://tmq.fanxiaobao.xyz

[$a, $b] = $arr;
来源：http://xft.ybcxt.top

[U52] PHP：箭头函数
来源：http://iqc.pengpengdd.cyou

$double = fn($x) => $x * 2;
来源：http://esz.sjlbkw.cn

[U53] PHP：空合并运算符
来源：http://esc.xylfe.cn

$v = $a ?? $b ?? "default";
来源：http://pkx.316326.xyz

[U54] PHP：空安全调用
来源：http://fjb.fehbvm.com

$obj?->method()
来源：http://gke.jinqigfzy.top

[U55] PHP：match 表达式
来源：http://mwm.shuidangran.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cdx.zycfv.cn

[U56] PHP：命名参数
来源：http://adc.shanyushiyangkeji.top

f(a: 1, b: 2)
来源：http://fie.sysykeji.top

[U57] PHP：字符串插值
来源：http://fdr.sysykeji.top

"值: {$a}"
来源：http://svx.ydzc1.top

[U58] PHP：数组三件套
来源：http://ypu.yj202588.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jcw.shanyushiyangkeji.top

[U59] PHP：自定义排序
来源：http://gwh.shuidangran.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fpq.yuxming.cn

[U60] PHP：JSON 编解码
来源：http://icg.c1oappe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hca.xingfuxueyuan.xyz

[U61] PHP：正则
来源：http://tom.ybcxt.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jkl.pengpengdd.cyou

[U62] PHP：日期对象
来源：http://buy.hnqzz.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sui.smart0.xyz

[U63] PHP：文件读写
来源：http://zcp.fzhhl.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mpa.fehbvm.com

[U64] PHP：目录遍历
来源：http://qno.0kj1m.cn

glob("dir/*.php");  scandir("dir");
来源：http://nwz.zhengqikj.top

[U65] PHP：会话
来源：http://fso.yj20258888.top

session_start();  $_SESSION["uid"] = 1;
来源：http://skl.zdbjq.cn

[U66] PHP：设置 Cookie
来源：http://rbz.dashuyun.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://suk.mhx1999.top

[U67] PHP：处理文件上传
来源：http://fcm.haohaochexian.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wuw.dashuyun.cn

[U68] PHP：PDO 连接
来源：http://kqa.sxryk.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gyu.9152youxi.cn

[U69] PHP：PDO 预处理
来源：http://ogy.xziqi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iwn.jinqigufen.top

[U70] PHP：PDO 事务
来源：http://gks.zhixingplan.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eol.nwbrower.top


<!-- 参考信息 -->