代发 wailian999

[S45] C++：lambda
来源：http://imm.bjfxy.top

auto add = [](int a, int b) { return a + b; };
来源：http://mwb.cheryme.top

[S46] C++：函数模板
来源：http://uja.xuanzx.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kgu.guannengcc.top

[S47] C++：结构化绑定遍历
来源：http://usy.daria6918.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zaz.chenzaomai.com

[S48] C++：逐行读文件
来源：http://tfd.ppjwa.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xxf.hywenlv.cn

while (std::getline(in, line)) { }
来源：http://okq.yangfankeji.com

[S49] C++：写文件
来源：http://wri.sweek.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hsl.smart0.xyz

[S50] C++：格式化数字
来源：http://hvv.xylfe.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bqg.zhiwuduotai.top

[S51] C++：显式类型转换
来源：http://ijq.cashguo.top

static_cast<double>(a) / b
来源：http://awd.hammf.cn

[S52] C++：const 与 noexcept
来源：http://qum.jqgufenzy.top

int size() const noexcept { return n_; }
来源：http://set.zhongyouzk.top

[S53] C++：移动语义
来源：http://azh.52xcode.cn

std::vector<int> w = std::move(v);
来源：http://cij.yj20258888.top

[S54] C++：异常处理
来源：http://psm.zdqjudy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rot.ivvv.top

[S55] C++：结构化绑定
来源：http://kig.dashuyun.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ymv.bbcook.cn

[S56] C++：optional
来源：http://tgv.iojbl.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yjy.nanxinkj.top

[S57] C++：编译期常量
来源：http://ysa.yvedp.cn

constexpr int N = 10;
来源：http://yjg.nanxinkj.top

[S58] C++：命名空间
来源：http://bzz.c1oappe.top

namespace ns { int f() { return 1; } }
来源：http://cwk.ctjpmb.com

[S59] C++：静态断言
来源：http://wdj.hywenlv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fyd.chenzaomai.com

[S60] C++：遍历并删除元素
来源：http://hjc.dashuyun.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kki.9152youxi.cn

================================================================================
来源：http://qnn.snrcjt.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eeu.zycfv.cn

================================================================================
来源：http://ejh.gogol.net.cn

[T01] Kotlin：Hello World
来源：http://uhx.jianghu66.top

println("Hello")
来源：http://bsy.fktsv.cn

[T02] Kotlin：变量
来源：http://qxo.tanke756.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yva.zhoulong.xyz

[T03] Kotlin：字符串模板
来源：http://whu.bjfxy.top

"值: $b"
来源：http://xbx.jqgufenzy.top

[T04] Kotlin：空安全
来源：http://fzh.hysaishi.cn

val n: String? = null;  n?.length
来源：http://lon.cheryme.top

[T05] Kotlin：when 表达式
来源：http://czu.dianchejie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lbc.quarkkingdee.top

[T06] Kotlin：集合映射
来源：http://rhs.sjlbkw.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qdp.sxryk.cn

[T07] Kotlin：集合过滤
来源：http://jgd.zdqjudy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ilw.zhixingplan.top

[T08] Kotlin：数据类
来源：http://mrx.tanke756.top

data class User(val name: String, val age: Int)
来源：http://yvf.yongpay.top

[T09] Kotlin：扩展函数
来源：http://mim.snrcjt.cn

fun String.exclaim() = this + "!"
来源：http://jpl.jqgufenzy.top

[T10] Kotlin：默认参数
来源：http://zha.xziqi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lmo.guowangkeji.top

[T11] Kotlin：协程
来源：http://aqm.daria6918.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://erv.jianghu66.top

[T12] Kotlin：解构声明
来源：http://zwl.jqgufenzy.top

val (a, b) = Pair(1, 2)
来源：http://gry.sweek.top

[T13] Kotlin：只读 Map
来源：http://xtx.nwbrower.top

val m = mapOf("a" to 1)
来源：http://lhz.redwolf501.top

[T14] Kotlin：循环
来源：http://uwk.tianlin.xyz

for (i in 1..10) println(i)
来源：http://goe.mhx1999.top

[T15] Kotlin：接口
来源：http://acr.cheryme.top

interface Shape { fun area(): Double }
来源：http://gih.hywenlv.cn

[T16] Swift：Hello World
来源：http://ohk.svipenyu.cn

print("Hello")
来源：http://vtt.ctjpmb.com

[T17] Swift：变量与常量
来源：http://dsw.fanxiaobao.xyz

var a = 1;  let b = 2
来源：http://qvk.xziqi.cn

[T18] Swift：字符串插值
来源：http://mkz.aibaodan.cn

"值: \(b)"
来源：http://qmx.uphjek.com

[T19] Swift：可选绑定
来源：http://gxb.wangdashe.top

if let n = opt { print(n) }
来源：http://ufj.ywan-chungtsiang.top

[T20] Swift：数组操作
来源：http://cxq.316326.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://zfl.smart0.xyz

[T21] Swift：遍历
来源：http://wka.shzxlz.cn

for x in a { print(x) }
来源：http://wpk.snrcjt.cn

[T22] Swift：字典
来源：http://kvu.chenlongwang.top

var d = ["a": 1];  d["b"] = 2
来源：http://hir.c1oappe.top

[T23] Swift：函数
来源：http://pop.gogol.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ctj.zdqjudy.top

[T24] Swift：闭包
来源：http://brz.jyoumei.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kft.redwolf501.top

[T25] Swift：结构体
来源：http://rvu.fehbvm.com

struct P { var x: Int }
来源：http://gso.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://rko.svipenyu.cn

class A: Base { override func f() {} }
来源：http://asr.0kj1m.cn

[T27] Swift：错误处理
来源：http://jru.iojbl.cn

do { try f() } catch { print(error) }
来源：http://lnp.yonumen.top

[T28] Swift：枚举
来源：http://uaa.hfpthk.cn

enum Color { case red, green }
来源：http://ewi.zhoulong.xyz

[T29] Swift：guard 提前返回
来源：http://xyn.jqgufenzy.top

guard let x = opt else { return }
来源：http://jxq.guowangkeji.top

[T30] Swift：协议
来源：http://zvj.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://cgl.shanyushiyangtech.top

[T31] Lua：Hello World
来源：http://ohk.iojbl.cn

print("Hello")
来源：http://kxj.nanxuanxn.top

[T32] Lua：局部变量
来源：http://pjs.jqgfzy.top

local a = 1
来源：http://qmx.zhixingplan.top

[T33] Lua：表（数组）
来源：http://ymn.shanyushiyangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://gxa.zhiwuduotai.top

[T34] Lua：遍历表
来源：http://gez.jinyuanbaomall.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qtf.yuxming.cn

[T35] Lua：字典表
来源：http://ttm.zdqjudy.top

local d = { a = 1 };  d.b = 2
来源：http://kbw.meibo888.top

[T36] Lua：函数
来源：http://kcl.hywenlv.cn

function add(a, b) return a + b end
来源：http://kex.quarkkingdee.top

[T37] Lua：字符串拼接
来源：http://aym.zhongyouzk.top

"a" .. "b"
来源：http://mbs.cqqwz.cn

[T38] Lua：条件
来源：http://jhh.shanyushiyangkeji.top

if x > 0 then print("正") end
来源：http://vod.zhaomingkeji.xyz

[T39] Lua：模式匹配
来源：http://yru.yfazqb.com

string.find(s, "%d+")
来源：http://oii.xylfe.cn

[T40] Lua：元表
来源：http://kxm.hcnkem.com

setmetatable({}, { __index = base })
来源：http://ijs.mhx1999.top

[T41] Perl：Hello World
来源：http://ven.cqqwz.cn

print "Hello\n";
来源：http://ohw.dianchejie.cn

[T42] Perl：变量类型
来源：http://owv.nanxuanxn.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lzu.xinyue.icu

[T43] Perl：字符串插值
来源：http://izw.fehbvm.com

"值: $a"
来源：http://lgd.cheryme.top

[T44] Perl：条件
来源：http://vhu.feifeiyinyue.top

if ($a > 0) { print "正"; }
来源：http://pne.vehdjk.com

[T45] Perl：数组遍历
来源：http://edz.shangyingyoupin.top

for my $x (@arr) { print $x; }
来源：http://ocq.zhaomingkeji.xyz

[T46] Perl：哈希操作
来源：http://two.yongpay.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dme.gaohongyu789.top

[T47] Perl：正则捕获
来源：http://zxw.haohaochexian.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://unl.aizwys.cn

[T48] Perl：正则替换
来源：http://zrs.nwbrower.top

$s =~ s/old/new/g;
来源：http://zvw.xuanzx.com

[T49] Perl：函数
来源：http://iio.xingfuxueyuan.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qgk.xylfe.cn

[T50] Perl：逐行读文件
来源：http://dww.daxiang520.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xvi.sjlbkw.cn

while (my $line = <$fh>) { print $line; }
来源：http://swr.uphjek.com

[T51] Scala：Hello World
来源：http://zub.hammf.cn

println("Hello")
来源：http://fik.yuxming.cn

[T52] Scala：变量
来源：http://gmv.sxryk.cn

val a = 1;  var b = 2
来源：http://xxd.birdmap.top

[T53] Scala：字符串插值
来源：http://gjx.epnwcf.com

s"值: $b"
来源：http://sgs.yanxiufei.cn

[T54] Scala：集合映射
来源：http://hvx.ivvv.top

List(1, 2, 3).map(_ * 2)
来源：http://hln.zhoulong.xyz

[T55] Scala：集合过滤
来源：http://hzh.gzhubu.top

List(1, 2, 3).filter(_ > 1)
来源：http://tkt.pengpengdd.cyou

[T56] Scala：样例类
来源：http://qvy.pycfn.com

case class User(name: String, age: Int)
来源：http://mqg.iojbl.cn

[T57] Scala：模式匹配
来源：http://hmz.gaohongyu789.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xcb.ppjwa.cn

[T58] Scala：函数定义
来源：http://zfw.jqgufenzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://wvl.pycfn.com

[T59] Scala：循环
来源：http://gzy.guannengcc.top

for (i <- 1 to 10) println(i)
来源：http://zlo.sjlbkw.cn

[T60] Scala：折叠
来源：http://iwm.shanyushiyangkeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bvm.sweek.top

================================================================================
来源：http://tyi.guannengcc.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ooy.sweek.top

================================================================================
来源：http://toq.mhx1999.top

[U01] Py：创建虚拟环境
来源：http://tfk.ivvv.top

python -m venv .venv && source .venv/bin/activate
来源：http://ble.hcnkem.com

[U02] Py：导出 / 安装依赖
来源：http://rmi.zdbjq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iwy.hfpthk.cn

[U03] Py：加载 .env 配置
来源：http://upv.xinyue.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://zfc.gogol.net.cn

[U04] Py：变量调试打印
来源：http://bdh.haohaochexian.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xqz.dashuyun.cn

[U05] Py：列表去重且保序
来源：http://pbv.bbcook.cn

list(dict.fromkeys(arr))
来源：http://zvt.zhongyouzk.top

[U06] Py：合并两个字典
来源：http://cpb.cqqwz.cn

{**a, **b}
来源：http://uaf.guowangkeji.top

[U07] Py：反转字典键值
来源：http://ppq.zdqjudy.top

{v: k for k, v in d.items()}
来源：http://ftl.nwbrower.top

[U08] Py：展平二维列表
来源：http://bbp.uphjek.com

[y for x in nested for y in x]
来源：http://zpl.yonumen.top

[U09] Py：字典取最大值的键
来源：http://dpk.zycfv.cn

max(d, key=d.get)
来源：http://pby.ybcxt.top

[U10] Py：按值排序字典
来源：http://mpq.hysaishi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mxo.gzhubu.top

[U11] Py：生成器表达式
来源：http://pgb.guowangkeji.top

(x * 2 for x in arr)
来源：http://jqw.yj202588.top

[U12] Py：取出现最多的 3 个元素
来源：http://aul.daxiang520.top

Counter(arr).most_common(3)
来源：http://muh.epnwcf.com

[U13] Py：固定长度队列
来源：http://vsc.nanxinkj.top

deque(maxlen=10)
来源：http://qqk.jianghu66.top

[U14] Py：分组收集到列表
来源：http://gfw.guannengcc.top

defaultdict(list)
来源：http://oiq.dashuyun.cn

[U15] Py：高精度计时
来源：http://qic.sxryk.cn

t = time.perf_counter()
来源：http://poc.fktsv.cn

[U16] Py：命令行参数解析
来源：http://mki.nwbrower.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mxt.yonumen.top

[U17] Py：初始化日志
来源：http://ral.ctjpmb.com

logging.basicConfig(level=logging.INFO)
来源：http://xuw.zhongyouzk.top

[U18] Py：预编译正则
来源：http://wav.smart0.xyz

pat = re.compile(r"\d+")
来源：http://xoa.yongpay.top

[U19] Py：正则替换带回调
来源：http://wlw.c1oappe.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fyq.hammf.cn

[U20] Py：缓存函数结果
来源：http://pmm.ydzc1.top

@functools.lru_cache(maxsize=None)
来源：http://hnv.jinyuanbaomall.cn

[U21] Py：自定义上下文管理器
来源：http://svl.yfazqb.com

@contextlib.contextmanager
来源：http://kks.ybcxt.top

[U22] Py：矩阵转置
来源：http://zli.hcnkem.com

list(zip(*m))
来源：http://jjf.andypj.xyz

[U23] Py：分块读取大文件
来源：http://eso.snrcjt.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://woc.andypj.xyz

[U24] Py：路径操作
来源：http://tpc.haohaochexian.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://opn.uphjek.com

[U25] Py：CSV 按字典读
来源：http://byi.hcnkem.com

csv.DictReader(f)
来源：http://oma.hesvh.cn

[U26] Py：并发下载
来源：http://hbv.c1oappe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zmv.jqgufenzy.top

[U27] Py：异步 HTTP
来源：http://wgj.jqgfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://cfy.yanxiufei.cn

[U28] Py：类型别名
来源：http://pew.jianghu66.top

UserId = int
来源：http://bwu.andypj.xyz

[U29] Py：属性校验
来源：http://ifm.hysaishi.cn

@property 与 @x.setter 配合
来源：http://ynb.feifeiyinyue.top

[U30] Py：数据类
来源：http://bhz.zycfv.cn

@dataclass(slots=True)
来源：http://vzx.gzhubu.top

[U31] Py：单测
来源：http://wyj.snrcjt.cn

python -m pytest -q
来源：http://dpv.aizwys.cn

[U32] Py：代码格式化
来源：http://kyw.9152youxi.cn

ruff format . && ruff check --fix .
来源：http://xuc.cashguo.top

[U33] Py：打包发布
来源：http://wlq.hongshengwenyu.top

python -m build  （依赖 pyproject.toml）
来源：http://cga.yongpay.top

[U34] Py：判断编码
来源：http://exa.jinghuilouyu.cn

chardet.detect(raw)
来源：http://fhm.xuanzx.com

[U35] Py：发送邮件
来源：http://cmp.tian-w.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wlp.haohaochexian.top

[U36] Py：定时任务
来源：http://gay.zhengqikj.top

schedule.every(10).minutes.do(job)
来源：http://vbw.vehdjk.com

[U37] Py：读写 Excel
来源：http://irz.vehdjk.com

pandas.read_excel / DataFrame.to_excel
来源：http://hck.jqgfzy.top

[U38] Py：获取脚本所在目录
来源：http://erd.dianchejie.cn

Path(__file__).resolve().parent
来源：http://xop.52xcode.cn

[U39] Py：判断是否在交互环境
来源：http://cau.nwbrower.top

sys.stdout.isatty()
来源：http://rta.zhengqikj.top

[U40] Py：打印到标准错误
来源：http://cas.fktsv.cn

print("err", file=sys.stderr)
来源：http://mof.quarkkingdee.top

[U41] PHP：初始化 Composer 项目
来源：http://oot.zhiwuduotai.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ajm.xuanzx.com

[U42] PHP：PSR-4 自动加载
来源：http://hcm.cheryme.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hjf.hnqzz.top

[U43] PHP：声明命名空间
来源：http://kxp.yj20258888.top

namespace App\Http;
来源：http://buz.aibaodan.cn

[U44] PHP：开启严格类型
来源：http://dva.shzxlz.cn

declare(strict_types=1);
来源：http://umf.hesvh.cn

[U45] PHP：类型声明与返回类型
来源：http://utq.jianghu66.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vac.zhijiandao.cn

[U46] PHP：可空类型
来源：http://edk.xingfuxueyuan.xyz

?string $name = null
来源：http://uve.ivvv.top

[U47] PHP：联合类型
来源：http://san.haohaochexian.top

int|string $id
来源：http://fql.sweek.top

[U48] PHP：纯枚举
来源：http://alw.havefunace.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://iic.cqqwz.cn

[U49] PHP：只读属性
来源：http://pta.meibo888.top

public readonly string $name
来源：http://mqi.bbcook.cn

[U50] PHP：构造器属性提升
来源：http://tyl.ehwqpu.com

public function __construct(private int $id) {}
来源：http://uxl.zhongyouzk.top

[U51] PHP：数组解构
来源：http://wls.0kj1m.cn

[$a, $b] = $arr;
来源：http://gvn.svipenyu.cn

[U52] PHP：箭头函数
来源：http://pha.guannengcc.top

$double = fn($x) => $x * 2;
来源：http://ejl.zhongyouzk.top

[U53] PHP：空合并运算符
来源：http://zqs.yuanzhike.top

$v = $a ?? $b ?? "default";
来源：http://vrn.jqgufenzy.top

[U54] PHP：空安全调用
来源：http://nlk.daria6918.cn

$obj?->method()
来源：http://yhz.fanxiaobao.xyz

[U55] PHP：match 表达式
来源：http://zwi.hywenlv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nsc.xylfe.cn

[U56] PHP：命名参数
来源：http://zan.tian-w.cn

f(a: 1, b: 2)
来源：http://ess.nanxinkj.top

[U57] PHP：字符串插值
来源：http://woz.jyoumei.cn

"值: {$a}"
来源：http://rsk.nanxinkj.top

[U58] PHP：数组三件套
来源：http://ify.gzhubu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rlr.yuxming.cn

[U59] PHP：自定义排序
来源：http://fmt.xuetiantiany.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://znk.guowangkeji.top

[U60] PHP：JSON 编解码
来源：http://xne.jianghu66.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://itz.yvedp.cn

[U61] PHP：正则
来源：http://bjq.feifeiyinyue.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hto.tian-w.cn

[U62] PHP：日期对象
来源：http://tee.nwbrower.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://utt.gzhubu.top

[U63] PHP：文件读写
来源：http://tqb.xingfuxueyuan.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rzo.yfazqb.com

[U64] PHP：目录遍历
来源：http://vmh.guannengcc.top

glob("dir/*.php");  scandir("dir");
来源：http://nhw.zdbjq.cn

[U65] PHP：会话
来源：http://epu.svipenyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zej.pycfn.com

[U66] PHP：设置 Cookie
来源：http://fjr.feifeiyinyue.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nuf.ppjwa.cn

[U67] PHP：处理文件上传
来源：http://stx.yueranfly.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tsn.shangyingyoupin.top

[U68] PHP：PDO 连接
来源：http://uqr.smart0.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lzd.bbcook.cn

[U69] PHP：PDO 预处理
来源：http://kyz.zdbjq.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://osr.xuetiantiany.cn

[U70] PHP：PDO 事务
来源：http://usj.pycfn.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vzr.ppjwa.cn


<!-- 参考信息 -->