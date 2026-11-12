代发 wailian999

[S45] C++：lambda
来源：http://ujf.chenlongwang.top

auto add = [](int a, int b) { return a + b; };
来源：http://pfi.pycfn.com

[S46] C++：函数模板
来源：http://vzm.redwolf501.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qqf.iojbl.cn

[S47] C++：结构化绑定遍历
来源：http://fej.chenlongwang.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fvm.meibo888.top

[S48] C++：逐行读文件
来源：http://duw.sufxvd.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cal.hfpthk.cn

while (std::getline(in, line)) { }
来源：http://mig.hongshengwenyu.top

[S49] C++：写文件
来源：http://mjj.ywan-chungtsiang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pnf.zhoulong.xyz

[S50] C++：格式化数字
来源：http://lmd.gotoacloud.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gxe.jqgufenzy.top

[S51] C++：显式类型转换
来源：http://tsl.fengsongda.top

static_cast<double>(a) / b
来源：http://wgq.smart0.xyz

[S52] C++：const 与 noexcept
来源：http://dvd.guowangkeji.top

int size() const noexcept { return n_; }
来源：http://yqz.shuidangran.top

[S53] C++：移动语义
来源：http://bzo.zycfv.cn

std::vector<int> w = std::move(v);
来源：http://mst.ydjk.org.cn

[S54] C++：异常处理
来源：http://ydl.shuidangran.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fyu.cucudq.cn

[S55] C++：结构化绑定
来源：http://cnr.yangfankeji.com

auto [a, b] = std::make_pair(1, 2);
来源：http://mcz.yj20258.top

[S56] C++：optional
来源：http://lmg.zhaomingkeji.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://orr.tarul.cn

[S57] C++：编译期常量
来源：http://ujw.jinqigufen.top

constexpr int N = 10;
来源：http://svk.ydjk.org.cn

[S58] C++：命名空间
来源：http://qqg.andypj.xyz

namespace ns { int f() { return 1; } }
来源：http://hhb.gaohongyu789.top

[S59] C++：静态断言
来源：http://liz.yj20258.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wyt.svipenyu.cn

[S60] C++：遍历并删除元素
来源：http://oxe.hysaishi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fxf.guannengcc.top

================================================================================
来源：http://dpe.bjfxy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gve.cdnleiting.top

================================================================================
来源：http://jhc.hesvh.cn

[T01] Kotlin：Hello World
来源：http://wpg.fanxiaobao.xyz

println("Hello")
来源：http://iri.nwbrower.top

[T02] Kotlin：变量
来源：http://qiy.gogol.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gdq.cqqwz.cn

[T03] Kotlin：字符串模板
来源：http://bnu.chenlongwang.top

"值: $b"
来源：http://lgl.pycfn.com

[T04] Kotlin：空安全
来源：http://gpn.hcnkem.com

val n: String? = null;  n?.length
来源：http://ifd.sxryk.cn

[T05] Kotlin：when 表达式
来源：http://ski.sufxvd.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wnv.xziqi.cn

[T06] Kotlin：集合映射
来源：http://zrn.iojbl.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xmp.bbcook.cn

[T07] Kotlin：集合过滤
来源：http://ajg.vehdjk.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://mve.vehdjk.com

[T08] Kotlin：数据类
来源：http://vhy.0kj1m.cn

data class User(val name: String, val age: Int)
来源：http://bot.ctjpmb.com

[T09] Kotlin：扩展函数
来源：http://gln.mhx1999.top

fun String.exclaim() = this + "!"
来源：http://akn.316326.xyz

[T10] Kotlin：默认参数
来源：http://vcv.zycfv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hbn.yanxiufei.cn

[T11] Kotlin：协程
来源：http://zgw.havefunace.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ujc.wangdashe.top

[T12] Kotlin：解构声明
来源：http://puf.hfpthk.cn

val (a, b) = Pair(1, 2)
来源：http://loi.zhongyouzk.top

[T13] Kotlin：只读 Map
来源：http://dby.ivvv.top

val m = mapOf("a" to 1)
来源：http://swf.hammf.cn

[T14] Kotlin：循环
来源：http://wqc.snrcjt.cn

for (i in 1..10) println(i)
来源：http://ouv.yj20258888.top

[T15] Kotlin：接口
来源：http://moj.mhx1999.top

interface Shape { fun area(): Double }
来源：http://qgk.hywenlv.cn

[T16] Swift：Hello World
来源：http://gtu.shuidangran.top

print("Hello")
来源：http://ibt.uphjek.com

[T17] Swift：变量与常量
来源：http://dkk.havefunace.top

var a = 1;  let b = 2
来源：http://hox.sweek.top

[T18] Swift：字符串插值
来源：http://clg.0kj1m.cn

"值: \(b)"
来源：http://qik.hesvh.cn

[T19] Swift：可选绑定
来源：http://qbo.zhiwuduotai.top

if let n = opt { print(n) }
来源：http://msw.sxryk.cn

[T20] Swift：数组操作
来源：http://xdz.52xcode.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tly.shuidangran.top

[T21] Swift：遍历
来源：http://vne.hywenlv.cn

for x in a { print(x) }
来源：http://hkg.yvedp.cn

[T22] Swift：字典
来源：http://zag.zdqjudy.top

var d = ["a": 1];  d["b"] = 2
来源：http://fwd.zhaomingkeji.xyz

[T23] Swift：函数
来源：http://lep.vqdsnc.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pee.dianchejie.cn

[T24] Swift：闭包
来源：http://avf.jinghuilouyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uhu.chenzaomai.com

[T25] Swift：结构体
来源：http://blz.nanxuanxn.top

struct P { var x: Int }
来源：http://zga.pengpengdd.cyou

[T26] Swift：类与重写
来源：http://jjz.nanxuanxn.top

class A: Base { override func f() {} }
来源：http://zsz.cashguo.top

[T27] Swift：错误处理
来源：http://jdz.smart0.xyz

do { try f() } catch { print(error) }
来源：http://mlw.yj20258.top

[T28] Swift：枚举
来源：http://qtv.vehdjk.com

enum Color { case red, green }
来源：http://qro.guannengcc.top

[T29] Swift：guard 提前返回
来源：http://vug.hywenlv.cn

guard let x = opt else { return }
来源：http://ffi.guowangkeji.top

[T30] Swift：协议
来源：http://rej.zhengqikj.top

protocol Shape { func area() -> Double }
来源：http://uac.jinyuanbaomall.cn

[T31] Lua：Hello World
来源：http://etq.cdnleiting.top

print("Hello")
来源：http://ozo.zhijiandao.cn

[T32] Lua：局部变量
来源：http://ole.hywenlv.cn

local a = 1
来源：http://pxs.xinyue.icu

[T33] Lua：表（数组）
来源：http://zmj.hfpthk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nph.hysaishi.cn

[T34] Lua：遍历表
来源：http://wqt.yongpay.top

for i, v in ipairs(t) do print(i, v) end
来源：http://npy.ppjwa.cn

[T35] Lua：字典表
来源：http://igz.hammf.cn

local d = { a = 1 };  d.b = 2
来源：http://qtz.yonumen.top

[T36] Lua：函数
来源：http://vfs.yongpay.top

function add(a, b) return a + b end
来源：http://hqs.xziqi.cn

[T37] Lua：字符串拼接
来源：http://ezw.zhongyouzk.top

"a" .. "b"
来源：http://vqi.havefunace.top

[T38] Lua：条件
来源：http://tqb.fengsongda.top

if x > 0 then print("正") end
来源：http://wch.feifeiyinyue.top

[T39] Lua：模式匹配
来源：http://gxe.hesvh.cn

string.find(s, "%d+")
来源：http://uks.fzhhl.top

[T40] Lua：元表
来源：http://dlc.epnwcf.com

setmetatable({}, { __index = base })
来源：http://iru.jinqigufen.top

[T41] Perl：Hello World
来源：http://ezs.gaohongyu789.top

print "Hello\n";
来源：http://rpb.ywan-chungtsiang.top

[T42] Perl：变量类型
来源：http://iet.yonumen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wdm.pengpengdd.cyou

[T43] Perl：字符串插值
来源：http://bcp.hammf.cn

"值: $a"
来源：http://lzr.gzhubu.top

[T44] Perl：条件
来源：http://wsl.zdbjq.cn

if ($a > 0) { print "正"; }
来源：http://fig.ctjpmb.com

[T45] Perl：数组遍历
来源：http://poi.fanxiaobao.xyz

for my $x (@arr) { print $x; }
来源：http://kee.tian-w.cn

[T46] Perl：哈希操作
来源：http://inc.jlsjyb.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xts.chenjidiqi.icu

[T47] Perl：正则捕获
来源：http://wep.jinyuanbaomall.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ena.tianlin.xyz

[T48] Perl：正则替换
来源：http://kjv.shangyingyoupin.top

$s =~ s/old/new/g;
来源：http://jmy.yuxming.cn

[T49] Perl：函数
来源：http://ust.yonumen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rce.jqgufenzy.top

[T50] Perl：逐行读文件
来源：http://icq.guowangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zkb.hysaishi.cn

while (my $line = <$fh>) { print $line; }
来源：http://kix.zhijiandao.cn

[T51] Scala：Hello World
来源：http://nvs.shangyingyoupin.top

println("Hello")
来源：http://nqm.birdmap.top

[T52] Scala：变量
来源：http://gdn.mhx1999.top

val a = 1;  var b = 2
来源：http://yhd.jinqigufen.top

[T53] Scala：字符串插值
来源：http://xzg.gogol.net.cn

s"值: $b"
来源：http://key.birdmap.top

[T54] Scala：集合映射
来源：http://gyi.c1oappe.top

List(1, 2, 3).map(_ * 2)
来源：http://seh.ehwqpu.com

[T55] Scala：集合过滤
来源：http://vic.guannengcc.top

List(1, 2, 3).filter(_ > 1)
来源：http://imf.xuetiantiany.cn

[T56] Scala：样例类
来源：http://lgr.c1oappe.top

case class User(name: String, age: Int)
来源：http://kam.aibaodan.cn

[T57] Scala：模式匹配
来源：http://mzv.cashguo.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://wlt.epnwcf.com

[T58] Scala：函数定义
来源：http://mxa.wangshuangyany.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uhp.yangfankeji.com

[T59] Scala：循环
来源：http://enj.wangdashe.top

for (i <- 1 to 10) println(i)
来源：http://xog.ywan-chungtsiang.top

[T60] Scala：折叠
来源：http://gsc.shzxlz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uow.redwolf501.top

================================================================================
来源：http://jai.jlsjyb.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ank.chenjidiqi.icu

================================================================================
来源：http://fpr.iojbl.cn

[U01] Py：创建虚拟环境
来源：http://nti.zdbjq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vra.fktsv.cn

[U02] Py：导出 / 安装依赖
来源：http://mjf.chenlongwang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bpy.haohaochexian.top

[U03] Py：加载 .env 配置
来源：http://bwf.guannengcc.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qtt.hcnkem.com

[U04] Py：变量调试打印
来源：http://vna.xingfuxueyuan.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kon.pycfn.com

[U05] Py：列表去重且保序
来源：http://uwy.yj202588.top

list(dict.fromkeys(arr))
来源：http://eic.ehwqpu.com

[U06] Py：合并两个字典
来源：http://lbs.sysykeji.top

{**a, **b}
来源：http://aau.zycfv.cn

[U07] Py：反转字典键值
来源：http://jjo.quarkkingdee.top

{v: k for k, v in d.items()}
来源：http://jdg.nwbrower.top

[U08] Py：展平二维列表
来源：http://tbz.epnwcf.com

[y for x in nested for y in x]
来源：http://mms.ybcxt.top

[U09] Py：字典取最大值的键
来源：http://aij.mhx1999.top

max(d, key=d.get)
来源：http://btg.c1oappe.top

[U10] Py：按值排序字典
来源：http://yoa.yueranfly.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ppl.gaohongyu789.top

[U11] Py：生成器表达式
来源：http://uun.pycfn.com

(x * 2 for x in arr)
来源：http://sjk.ehwqpu.com

[U12] Py：取出现最多的 3 个元素
来源：http://snr.zhixingplan.top

Counter(arr).most_common(3)
来源：http://xzo.jinqigufen.top

[U13] Py：固定长度队列
来源：http://rof.ywan-chungtsiang.top

deque(maxlen=10)
来源：http://xzo.9152youxi.cn

[U14] Py：分组收集到列表
来源：http://ord.jiagoushi.top

defaultdict(list)
来源：http://iia.daxiang520.top

[U15] Py：高精度计时
来源：http://zgi.yueranfly.top

t = time.perf_counter()
来源：http://mxl.hnxiangtu.top

[U16] Py：命令行参数解析
来源：http://ght.cheryme.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yem.jqgfzy.top

[U17] Py：初始化日志
来源：http://cjn.jinqigfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://goz.hysaishi.cn

[U18] Py：预编译正则
来源：http://sal.yuxming.cn

pat = re.compile(r"\d+")
来源：http://pho.ppjwa.cn

[U19] Py：正则替换带回调
来源：http://she.chenlongwang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://trd.gaohongyu789.top

[U20] Py：缓存函数结果
来源：http://whf.hcnkem.com

@functools.lru_cache(maxsize=None)
来源：http://ujc.aibaodan.cn

[U21] Py：自定义上下文管理器
来源：http://rzx.xziqi.cn

@contextlib.contextmanager
来源：http://aln.fengsongda.top

[U22] Py：矩阵转置
来源：http://dgp.ehwqpu.com

list(zip(*m))
来源：http://tny.yj20258888.top

[U23] Py：分块读取大文件
来源：http://nmf.hongshengwenyu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vef.chenjidiqi.icu

[U24] Py：路径操作
来源：http://oxs.ppjwa.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kiz.tian-w.cn

[U25] Py：CSV 按字典读
来源：http://gdq.dianchejie.cn

csv.DictReader(f)
来源：http://hyp.sufxvd.cn

[U26] Py：并发下载
来源：http://uvr.jqgufenzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://owc.redwolf501.top

[U27] Py：异步 HTTP
来源：http://tvv.yvedp.cn

aiohttp.ClientSession() 配合 async with
来源：http://duv.tanke756.top

[U28] Py：类型别名
来源：http://wil.shanyushiyangkeji.top

UserId = int
来源：http://lam.yongpay.top

[U29] Py：属性校验
来源：http://ihw.yj202588.top

@property 与 @x.setter 配合
来源：http://byf.xingfuxueyuan.xyz

[U30] Py：数据类
来源：http://qbt.zhongyouzk.top

@dataclass(slots=True)
来源：http://wuv.vehdjk.com

[U31] Py：单测
来源：http://bvg.yfazqb.com

python -m pytest -q
来源：http://fjl.hammf.cn

[U32] Py：代码格式化
来源：http://ugd.zhongyouzk.top

ruff format . && ruff check --fix .
来源：http://txs.hammf.cn

[U33] Py：打包发布
来源：http://mre.shanyushiyangtech.top

python -m build  （依赖 pyproject.toml）
来源：http://sch.shanyushiyangtech.top

[U34] Py：判断编码
来源：http://mii.wangshuangyany.cn

chardet.detect(raw)
来源：http://any.jqgufenzy.top

[U35] Py：发送邮件
来源：http://liz.xuanzx.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://smf.hnqzz.top

[U36] Py：定时任务
来源：http://vir.cqqwz.cn

schedule.every(10).minutes.do(job)
来源：http://vyc.zdbjq.cn

[U37] Py：读写 Excel
来源：http://axa.jinghuilouyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qgj.havefunace.top

[U38] Py：获取脚本所在目录
来源：http://xwg.9152youxi.cn

Path(__file__).resolve().parent
来源：http://chw.c1oappe.top

[U39] Py：判断是否在交互环境
来源：http://xcu.haohaochexian.top

sys.stdout.isatty()
来源：http://lgr.316326.xyz

[U40] Py：打印到标准错误
来源：http://dft.sjlbkw.cn

print("err", file=sys.stderr)
来源：http://whm.pycfn.com

[U41] PHP：初始化 Composer 项目
来源：http://tsr.nwbrower.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fxh.snrcjt.cn

[U42] PHP：PSR-4 自动加载
来源：http://cal.jyoumei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://elm.iojbl.cn

[U43] PHP：声明命名空间
来源：http://qth.xylfe.cn

namespace App\Http;
来源：http://gtk.yangfankeji.com

[U44] PHP：开启严格类型
来源：http://nwn.hammf.cn

declare(strict_types=1);
来源：http://pvk.jqgfzy.top

[U45] PHP：类型声明与返回类型
来源：http://tny.cheryme.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://tnp.zhoulong.xyz

[U46] PHP：可空类型
来源：http://pla.zhaomingkeji.xyz

?string $name = null
来源：http://aym.zdbjq.cn

[U47] PHP：联合类型
来源：http://zup.daria6918.cn

int|string $id
来源：http://bco.zhoulong.xyz

[U48] PHP：纯枚举
来源：http://ase.zhengqikj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://oej.vqdsnc.cn

[U49] PHP：只读属性
来源：http://jqx.sjlbkw.cn

public readonly string $name
来源：http://qry.52xcode.cn

[U50] PHP：构造器属性提升
来源：http://wmj.fzhhl.top

public function __construct(private int $id) {}
来源：http://pry.kuanghao11.cn

[U51] PHP：数组解构
来源：http://cvb.iojbl.cn

[$a, $b] = $arr;
来源：http://vjo.zdbjq.cn

[U52] PHP：箭头函数
来源：http://zel.ehwqpu.com

$double = fn($x) => $x * 2;
来源：http://eha.c1oappe.top

[U53] PHP：空合并运算符
来源：http://ldj.jinqigfzy.top

$v = $a ?? $b ?? "default";
来源：http://pfe.sxryk.cn

[U54] PHP：空安全调用
来源：http://nme.sxryk.cn

$obj?->method()
来源：http://wbj.jlsjyb.cn

[U55] PHP：match 表达式
来源：http://ije.xylfe.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ztj.fktsv.cn

[U56] PHP：命名参数
来源：http://qfy.zhaomingkeji.xyz

f(a: 1, b: 2)
来源：http://iij.hnqzz.top

[U57] PHP：字符串插值
来源：http://etp.tanke756.top

"值: {$a}"
来源：http://vum.jinqigfzy.top

[U58] PHP：数组三件套
来源：http://qwf.zhijiandao.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hjr.fzhhl.top

[U59] PHP：自定义排序
来源：http://jnp.yj202588.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ngq.chenjidiqi.icu

[U60] PHP：JSON 编解码
来源：http://gub.yj20258.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://awu.gzhubu.top

[U61] PHP：正则
来源：http://tgj.vehdjk.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://luy.pengpengdd.cyou

[U62] PHP：日期对象
来源：http://sfr.pycfn.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xjb.dashuyun.cn

[U63] PHP：文件读写
来源：http://tbk.andypj.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://olw.redwolf501.top

[U64] PHP：目录遍历
来源：http://mlh.hywenlv.cn

glob("dir/*.php");  scandir("dir");
来源：http://jwp.hywenlv.cn

[U65] PHP：会话
来源：http://plg.vqdsnc.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ouj.yuxming.cn

[U66] PHP：设置 Cookie
来源：http://vty.xinyue.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nkd.yj20258888.top

[U67] PHP：处理文件上传
来源：http://wjw.52xcode.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xsg.hesvh.cn

[U68] PHP：PDO 连接
来源：http://gzu.daxiang520.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wvp.fanxiaobao.xyz

[U69] PHP：PDO 预处理
来源：http://xqh.jinqigfzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uxq.svipenyu.cn

[U70] PHP：PDO 事务
来源：http://pns.guowangkeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pvp.sweek.top


<!-- 参考信息 -->