代发 wailian999

[S45] C++：lambda
来源：http://aoy.zhoulong.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://cds.zdbjq.cn

[S46] C++：函数模板
来源：http://vlj.nanxuanxn.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ncf.yfazqb.com

[S47] C++：结构化绑定遍历
来源：http://hla.yj20258888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rhw.0kj1m.cn

[S48] C++：逐行读文件
来源：http://vzx.zdqjudy.top

std::ifstream in("a.txt");  std::string line;
来源：http://rhe.c1oappe.top

while (std::getline(in, line)) { }
来源：http://hlr.feifeiyinyue.top

[S49] C++：写文件
来源：http://pvx.ivvv.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jeb.vehdjk.com

[S50] C++：格式化数字
来源：http://kif.havefunace.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vgc.svipenyu.cn

[S51] C++：显式类型转换
来源：http://qqr.hysaishi.cn

static_cast<double>(a) / b
来源：http://ciq.dashuyun.cn

[S52] C++：const 与 noexcept
来源：http://drm.gaohongyu789.top

int size() const noexcept { return n_; }
来源：http://pbo.tianlin.xyz

[S53] C++：移动语义
来源：http://zwg.shanyushiyangkeji.top

std::vector<int> w = std::move(v);
来源：http://kel.sweek.top

[S54] C++：异常处理
来源：http://ybw.svipenyu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fxf.gzhubu.top

[S55] C++：结构化绑定
来源：http://jyh.nanxuanxn.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vsv.nanxuanxn.top

[S56] C++：optional
来源：http://edl.aibaodan.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zdc.cdnleiting.top

[S57] C++：编译期常量
来源：http://yzu.uphjek.com

constexpr int N = 10;
来源：http://igs.aizwys.cn

[S58] C++：命名空间
来源：http://smc.zycfv.cn

namespace ns { int f() { return 1; } }
来源：http://ikf.shanyushiyangtech.top

[S59] C++：静态断言
来源：http://cpg.uphjek.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tux.yvedp.cn

[S60] C++：遍历并删除元素
来源：http://peq.feifeiyinyue.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jyp.gaohongyu789.top

================================================================================
来源：http://fwm.svipenyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://byc.ywan-chungtsiang.top

================================================================================
来源：http://jsi.havefunace.top

[T01] Kotlin：Hello World
来源：http://etg.sufxvd.cn

println("Hello")
来源：http://htg.jinyuanbaomall.cn

[T02] Kotlin：变量
来源：http://tof.nwbrower.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cid.hongshengwenyu.top

[T03] Kotlin：字符串模板
来源：http://svp.meibo888.top

"值: $b"
来源：http://isk.sufxvd.cn

[T04] Kotlin：空安全
来源：http://hxn.bjfxy.top

val n: String? = null;  n?.length
来源：http://ute.xylfe.cn

[T05] Kotlin：when 表达式
来源：http://fbq.ppjwa.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ven.nwbrower.top

[T06] Kotlin：集合映射
来源：http://mgw.ehwqpu.com

listOf(1, 2, 3).map { it * 2 }
来源：http://hiz.dashuyun.cn

[T07] Kotlin：集合过滤
来源：http://auy.jinqigufen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rjg.wangdashe.top

[T08] Kotlin：数据类
来源：http://pww.feifeiyinyue.top

data class User(val name: String, val age: Int)
来源：http://hkd.mhx1999.top

[T09] Kotlin：扩展函数
来源：http://ozy.yanxiufei.cn

fun String.exclaim() = this + "!"
来源：http://bau.cheryme.top

[T10] Kotlin：默认参数
来源：http://qga.gaohongyu789.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hsr.nwbrower.top

[T11] Kotlin：协程
来源：http://fut.birdmap.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://sfu.jinqigfzy.top

[T12] Kotlin：解构声明
来源：http://ghl.yonumen.top

val (a, b) = Pair(1, 2)
来源：http://byo.zhaomingkeji.xyz

[T13] Kotlin：只读 Map
来源：http://htu.smart0.xyz

val m = mapOf("a" to 1)
来源：http://dog.xylfe.cn

[T14] Kotlin：循环
来源：http://lxf.meibo888.top

for (i in 1..10) println(i)
来源：http://yyo.haohaochexian.top

[T15] Kotlin：接口
来源：http://hno.zhixingplan.top

interface Shape { fun area(): Double }
来源：http://rte.pycfn.com

[T16] Swift：Hello World
来源：http://qww.jianghu66.top

print("Hello")
来源：http://clo.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://qdu.ehwqpu.com

var a = 1;  let b = 2
来源：http://vjs.redwolf501.top

[T18] Swift：字符串插值
来源：http://kuo.fanxiaobao.xyz

"值: \(b)"
来源：http://tnp.sxryk.cn

[T19] Swift：可选绑定
来源：http://wcs.bbcook.cn

if let n = opt { print(n) }
来源：http://blp.xylfe.cn

[T20] Swift：数组操作
来源：http://xwb.hammf.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fav.52xcode.cn

[T21] Swift：遍历
来源：http://kvk.sjlbkw.cn

for x in a { print(x) }
来源：http://mez.yueranfly.top

[T22] Swift：字典
来源：http://ctm.sjlbkw.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cfj.ctjpmb.com

[T23] Swift：函数
来源：http://vgx.shangyingyoupin.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hrq.fzhhl.top

[T24] Swift：闭包
来源：http://rzg.zhaomingkeji.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://sla.316326.xyz

[T25] Swift：结构体
来源：http://hhp.0kj1m.cn

struct P { var x: Int }
来源：http://cbk.iojbl.cn

[T26] Swift：类与重写
来源：http://tfr.xuanzx.com

class A: Base { override func f() {} }
来源：http://izo.ywan-chungtsiang.top

[T27] Swift：错误处理
来源：http://rbo.shzxlz.cn

do { try f() } catch { print(error) }
来源：http://pok.redwolf501.top

[T28] Swift：枚举
来源：http://sfu.pengpengdd.cyou

enum Color { case red, green }
来源：http://bgy.zhengqikj.top

[T29] Swift：guard 提前返回
来源：http://ykz.cucudq.cn

guard let x = opt else { return }
来源：http://cwt.gaohongyu789.top

[T30] Swift：协议
来源：http://pku.cucudq.cn

protocol Shape { func area() -> Double }
来源：http://kfv.yangfankeji.com

[T31] Lua：Hello World
来源：http://kbw.andypj.xyz

print("Hello")
来源：http://zwz.ehwqpu.com

[T32] Lua：局部变量
来源：http://qvu.vqdsnc.cn

local a = 1
来源：http://mwg.yj202588.top

[T33] Lua：表（数组）
来源：http://jpi.shzxlz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ivz.xuetiantiany.cn

[T34] Lua：遍历表
来源：http://rvt.zhixingplan.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hyi.ywan-chungtsiang.top

[T35] Lua：字典表
来源：http://dev.zdbjq.cn

local d = { a = 1 };  d.b = 2
来源：http://jjq.aizwys.cn

[T36] Lua：函数
来源：http://baw.shangyingyoupin.top

function add(a, b) return a + b end
来源：http://dcs.jqgufenzy.top

[T37] Lua：字符串拼接
来源：http://nqs.cqqwz.cn

"a" .. "b"
来源：http://cvc.0kj1m.cn

[T38] Lua：条件
来源：http://mwm.guannengcc.top

if x > 0 then print("正") end
来源：http://nsd.xingfuxueyuan.xyz

[T39] Lua：模式匹配
来源：http://ecd.vehdjk.com

string.find(s, "%d+")
来源：http://rtj.nwbrower.top

[T40] Lua：元表
来源：http://xgc.fzhhl.top

setmetatable({}, { __index = base })
来源：http://ltj.havefunace.top

[T41] Perl：Hello World
来源：http://pym.yuanzhike.top

print "Hello\n";
来源：http://euo.iojbl.cn

[T42] Perl：变量类型
来源：http://hpy.fehbvm.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ltw.hywenlv.cn

[T43] Perl：字符串插值
来源：http://ivi.uphjek.com

"值: $a"
来源：http://qmp.smart0.xyz

[T44] Perl：条件
来源：http://wvv.pengpengdd.cyou

if ($a > 0) { print "正"; }
来源：http://ymt.hywenlv.cn

[T45] Perl：数组遍历
来源：http://svn.aibaodan.cn

for my $x (@arr) { print $x; }
来源：http://mwz.yuxming.cn

[T46] Perl：哈希操作
来源：http://cul.tianlin.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cgy.jinyuanbaomall.cn

[T47] Perl：正则捕获
来源：http://sql.hcnkem.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://foc.tianlin.xyz

[T48] Perl：正则替换
来源：http://ocb.birdmap.top

$s =~ s/old/new/g;
来源：http://nxg.sweek.top

[T49] Perl：函数
来源：http://exb.dianchejie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xom.jinyuanbaomall.cn

[T50] Perl：逐行读文件
来源：http://ucs.tanke756.top

open my $fh, "<", "a.txt" or die $!;
来源：http://yml.uphjek.com

while (my $line = <$fh>) { print $line; }
来源：http://fhd.hfpthk.cn

[T51] Scala：Hello World
来源：http://gas.yj202588.top

println("Hello")
来源：http://tcp.meibo888.top

[T52] Scala：变量
来源：http://fpt.hfpthk.cn

val a = 1;  var b = 2
来源：http://ahl.hammf.cn

[T53] Scala：字符串插值
来源：http://vwo.vqdsnc.cn

s"值: $b"
来源：http://anw.cucudq.cn

[T54] Scala：集合映射
来源：http://lij.quarkkingdee.top

List(1, 2, 3).map(_ * 2)
来源：http://kme.zhiwuduotai.top

[T55] Scala：集合过滤
来源：http://sin.cucudq.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dat.hnqzz.top

[T56] Scala：样例类
来源：http://jxx.ybcxt.top

case class User(name: String, age: Int)
来源：http://lmo.tanke756.top

[T57] Scala：模式匹配
来源：http://cmz.nanxuanxn.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://wnm.jianghu66.top

[T58] Scala：函数定义
来源：http://otg.fehbvm.com

def add(a: Int, b: Int): Int = a + b
来源：http://uup.daria6918.cn

[T59] Scala：循环
来源：http://voy.shzxlz.cn

for (i <- 1 to 10) println(i)
来源：http://alu.9152youxi.cn

[T60] Scala：折叠
来源：http://qua.zhengqikj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tqk.sufxvd.cn

================================================================================
来源：http://tzo.gaohongyu789.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vwa.guannengcc.top

================================================================================
来源：http://sya.cashguo.top

[U01] Py：创建虚拟环境
来源：http://rmr.ydzc1.top

python -m venv .venv && source .venv/bin/activate
来源：http://erd.guannengcc.top

[U02] Py：导出 / 安装依赖
来源：http://zxh.guowangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://usg.yuxming.cn

[U03] Py：加载 .env 配置
来源：http://wtb.shangyingyoupin.top

from dotenv import load_dotenv; load_dotenv()
来源：http://cqd.uphjek.com

[U04] Py：变量调试打印
来源：http://kef.jinqigufen.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kzz.uphjek.com

[U05] Py：列表去重且保序
来源：http://vls.xuetiantiany.cn

list(dict.fromkeys(arr))
来源：http://uku.sjlbkw.cn

[U06] Py：合并两个字典
来源：http://cul.xinyue.icu

{**a, **b}
来源：http://zlb.gogol.net.cn

[U07] Py：反转字典键值
来源：http://drp.vqdsnc.cn

{v: k for k, v in d.items()}
来源：http://bew.daxiang520.top

[U08] Py：展平二维列表
来源：http://qfm.dashuyun.cn

[y for x in nested for y in x]
来源：http://wed.9152youxi.cn

[U09] Py：字典取最大值的键
来源：http://paq.jinyuanbaomall.cn

max(d, key=d.get)
来源：http://jwt.svipenyu.cn

[U10] Py：按值排序字典
来源：http://mtt.guowangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bea.xinyue.icu

[U11] Py：生成器表达式
来源：http://vuz.zhengqikj.top

(x * 2 for x in arr)
来源：http://wdn.kuanghao11.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gva.ydjk.org.cn

Counter(arr).most_common(3)
来源：http://pte.zhiwuduotai.top

[U13] Py：固定长度队列
来源：http://jbw.tian-w.cn

deque(maxlen=10)
来源：http://mpl.shanyushiyangtech.top

[U14] Py：分组收集到列表
来源：http://egi.c1oappe.top

defaultdict(list)
来源：http://nga.meibo888.top

[U15] Py：高精度计时
来源：http://zsn.hywenlv.cn

t = time.perf_counter()
来源：http://ddc.ppjwa.cn

[U16] Py：命令行参数解析
来源：http://noq.hammf.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nzr.ydjk.org.cn

[U17] Py：初始化日志
来源：http://wok.yj202588.top

logging.basicConfig(level=logging.INFO)
来源：http://qka.ywan-chungtsiang.top

[U18] Py：预编译正则
来源：http://cuf.fehbvm.com

pat = re.compile(r"\d+")
来源：http://kxt.fengsongda.top

[U19] Py：正则替换带回调
来源：http://but.ydzc1.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gej.ctjpmb.com

[U20] Py：缓存函数结果
来源：http://tju.dashuyun.cn

@functools.lru_cache(maxsize=None)
来源：http://mdt.tianlin.xyz

[U21] Py：自定义上下文管理器
来源：http://vkp.zhongyouzk.top

@contextlib.contextmanager
来源：http://ygc.guowangkeji.top

[U22] Py：矩阵转置
来源：http://lkf.guowangkeji.top

list(zip(*m))
来源：http://gmc.dashuyun.cn

[U23] Py：分块读取大文件
来源：http://svo.sweek.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pqp.xinyue.icu

[U24] Py：路径操作
来源：http://lwa.fzhhl.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vmo.sxryk.cn

[U25] Py：CSV 按字典读
来源：http://hsu.meibo888.top

csv.DictReader(f)
来源：http://dtg.hnxiangtu.top

[U26] Py：并发下载
来源：http://wsk.cashguo.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kfk.pengpengdd.cyou

[U27] Py：异步 HTTP
来源：http://qyw.yj20258.top

aiohttp.ClientSession() 配合 async with
来源：http://irn.wangdashe.top

[U28] Py：类型别名
来源：http://pnn.fzhhl.top

UserId = int
来源：http://fzi.tanke756.top

[U29] Py：属性校验
来源：http://zxt.feifeiyinyue.top

@property 与 @x.setter 配合
来源：http://bwo.ydjk.org.cn

[U30] Py：数据类
来源：http://ufo.jinyuanbaomall.cn

@dataclass(slots=True)
来源：http://ziy.zycfv.cn

[U31] Py：单测
来源：http://ieb.ctjpmb.com

python -m pytest -q
来源：http://lrj.gogol.net.cn

[U32] Py：代码格式化
来源：http://brp.yj202588.top

ruff format . && ruff check --fix .
来源：http://rgt.yangfankeji.com

[U33] Py：打包发布
来源：http://uec.hongshengwenyu.top

python -m build  （依赖 pyproject.toml）
来源：http://prp.yuanzhike.top

[U34] Py：判断编码
来源：http://rpa.zhijiandao.cn

chardet.detect(raw)
来源：http://igh.hongshengwenyu.top

[U35] Py：发送邮件
来源：http://dha.zhoulong.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ofn.sweek.top

[U36] Py：定时任务
来源：http://jzg.shuidangran.top

schedule.every(10).minutes.do(job)
来源：http://gpf.c1oappe.top

[U37] Py：读写 Excel
来源：http://boh.yongpay.top

pandas.read_excel / DataFrame.to_excel
来源：http://pqv.gogol.net.cn

[U38] Py：获取脚本所在目录
来源：http://hkr.hysaishi.cn

Path(__file__).resolve().parent
来源：http://iwv.pengpengdd.cyou

[U39] Py：判断是否在交互环境
来源：http://sua.yj20258.top

sys.stdout.isatty()
来源：http://ohu.jlsjyb.cn

[U40] Py：打印到标准错误
来源：http://vpm.hfpthk.cn

print("err", file=sys.stderr)
来源：http://kxb.yfazqb.com

[U41] PHP：初始化 Composer 项目
来源：http://ljn.nwbrower.top

composer init;  composer require guzzlehttp/guzzle
来源：http://rzp.zhixingplan.top

[U42] PHP：PSR-4 自动加载
来源：http://fdo.xylfe.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sxq.redwolf501.top

[U43] PHP：声明命名空间
来源：http://yxt.dashuyun.cn

namespace App\Http;
来源：http://xvj.9152youxi.cn

[U44] PHP：开启严格类型
来源：http://weg.fktsv.cn

declare(strict_types=1);
来源：http://ycg.ywan-chungtsiang.top

[U45] PHP：类型声明与返回类型
来源：http://bbd.aizwys.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ggr.ctjpmb.com

[U46] PHP：可空类型
来源：http://fpd.yonumen.top

?string $name = null
来源：http://mfc.shanyushiyangkeji.top

[U47] PHP：联合类型
来源：http://wzv.cqqwz.cn

int|string $id
来源：http://qwc.ydjk.org.cn

[U48] PHP：纯枚举
来源：http://vxu.yj20258888.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wsr.sxryk.cn

[U49] PHP：只读属性
来源：http://pku.hongshengwenyu.top

public readonly string $name
来源：http://qbw.sxryk.cn

[U50] PHP：构造器属性提升
来源：http://ani.xuanzx.com

public function __construct(private int $id) {}
来源：http://eob.hywenlv.cn

[U51] PHP：数组解构
来源：http://lea.yj20258888.top

[$a, $b] = $arr;
来源：http://yjd.hfpthk.cn

[U52] PHP：箭头函数
来源：http://dfz.jinqigufen.top

$double = fn($x) => $x * 2;
来源：http://owv.vqdsnc.cn

[U53] PHP：空合并运算符
来源：http://rgc.feifeiyinyue.top

$v = $a ?? $b ?? "default";
来源：http://fvn.hesvh.cn

[U54] PHP：空安全调用
来源：http://qhx.iojbl.cn

$obj?->method()
来源：http://vtt.hysaishi.cn

[U55] PHP：match 表达式
来源：http://ppd.shuidangran.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bpx.cucudq.cn

[U56] PHP：命名参数
来源：http://kjd.bjfxy.top

f(a: 1, b: 2)
来源：http://ygn.shanyushiyangtech.top

[U57] PHP：字符串插值
来源：http://ghr.cucudq.cn

"值: {$a}"
来源：http://trx.vehdjk.com

[U58] PHP：数组三件套
来源：http://hla.tanke756.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vsl.aibaodan.cn

[U59] PHP：自定义排序
来源：http://myf.hammf.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aoc.daria6918.cn

[U60] PHP：JSON 编解码
来源：http://neq.shangyingyoupin.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bfg.dashuyun.cn

[U61] PHP：正则
来源：http://ydr.daria6918.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://atj.ctjpmb.com

[U62] PHP：日期对象
来源：http://ykg.jiagoushi.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bor.fengsongda.top

[U63] PHP：文件读写
来源：http://kor.jianghu66.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xfb.gogol.net.cn

[U64] PHP：目录遍历
来源：http://lcd.fktsv.cn

glob("dir/*.php");  scandir("dir");
来源：http://pce.nwbrower.top

[U65] PHP：会话
来源：http://rqx.birdmap.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jma.jlsjyb.cn

[U66] PHP：设置 Cookie
来源：http://rgz.iojbl.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mgb.wangdashe.top

[U67] PHP：处理文件上传
来源：http://rju.dashuyun.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bum.snrcjt.cn

[U68] PHP：PDO 连接
来源：http://pux.dashuyun.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tye.fanxiaobao.xyz

[U69] PHP：PDO 预处理
来源：http://kbb.ydjk.org.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sjy.gaohongyu789.top

[U70] PHP：PDO 事务
来源：http://lrb.gogol.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yrz.cheryme.top


<!-- 参考信息 -->