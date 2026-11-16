代发 wailian999

[S43] C++：智能指针
来源：http://qxy.zdbjq.cn

auto p = std::make_unique<int>(5);
来源：http://pwr.zhixingplan.top

[S44] C++：引用传参
来源：http://yko.jlsjyb.cn

void inc(int &x) { ++x; }
来源：http://xoi.cashguo.top

[S45] C++：lambda
来源：http://enf.chenlongwang.top

auto add = [](int a, int b) { return a + b; };
来源：http://yxt.zhixingplan.top

[S46] C++：函数模板
来源：http://dkh.shanyushiyangtech.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://law.yonumen.top

[S47] C++：结构化绑定遍历
来源：http://aou.pycfn.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://joj.hammf.cn

[S48] C++：逐行读文件
来源：http://pfs.zycfv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fyy.nwbrower.top

while (std::getline(in, line)) { }
来源：http://tzx.chenzaomai.com

[S49] C++：写文件
来源：http://oaf.yj202588.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dec.jlsjyb.cn

[S50] C++：格式化数字
来源：http://fwr.ydjk.org.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bca.ivvv.top

[S51] C++：显式类型转换
来源：http://lit.yj20258888.top

static_cast<double>(a) / b
来源：http://jal.hcnkem.com

[S52] C++：const 与 noexcept
来源：http://faz.tianlin.xyz

int size() const noexcept { return n_; }
来源：http://jyi.feifeiyinyue.top

[S53] C++：移动语义
来源：http://hoy.andypj.xyz

std::vector<int> w = std::move(v);
来源：http://txu.jiagoushi.top

[S54] C++：异常处理
来源：http://qzi.jlsjyb.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://smx.zycfv.cn

[S55] C++：结构化绑定
来源：http://jqh.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vjr.zycfv.cn

[S56] C++：optional
来源：http://ank.ydzc1.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hci.yvedp.cn

[S57] C++：编译期常量
来源：http://isp.xinyue.icu

constexpr int N = 10;
来源：http://qld.hfpthk.cn

[S58] C++：命名空间
来源：http://fso.jinqigufen.top

namespace ns { int f() { return 1; } }
来源：http://dcw.jianghu66.top

[S59] C++：静态断言
来源：http://vng.mhx1999.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iwc.cqqwz.cn

[S60] C++：遍历并删除元素
来源：http://bec.sjlbkw.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://van.jqgfzy.top

================================================================================
来源：http://ygr.gzhubu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ziz.nwbrower.top

================================================================================
来源：http://tmm.guannengcc.top

[T01] Kotlin：Hello World
来源：http://pte.shuidangran.top

println("Hello")
来源：http://cxa.jqgufenzy.top

[T02] Kotlin：变量
来源：http://exq.yonumen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gde.hongshengwenyu.top

[T03] Kotlin：字符串模板
来源：http://byf.sufxvd.cn

"值: $b"
来源：http://jht.daria6918.cn

[T04] Kotlin：空安全
来源：http://bnw.bbcook.cn

val n: String? = null;  n?.length
来源：http://soa.iojbl.cn

[T05] Kotlin：when 表达式
来源：http://the.zhengqikj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sue.nanxuanxn.top

[T06] Kotlin：集合映射
来源：http://ups.zhengqikj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ypc.ydjk.org.cn

[T07] Kotlin：集合过滤
来源：http://gmk.mhx1999.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xga.yongpay.top

[T08] Kotlin：数据类
来源：http://hrj.sweek.top

data class User(val name: String, val age: Int)
来源：http://woc.yongpay.top

[T09] Kotlin：扩展函数
来源：http://wsa.shanyushiyangtech.top

fun String.exclaim() = this + "!"
来源：http://pdy.jinghuilouyu.cn

[T10] Kotlin：默认参数
来源：http://iea.zhengqikj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://upe.quarkkingdee.top

[T11] Kotlin：协程
来源：http://aqu.daxiang520.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://shj.xuanzx.com

[T12] Kotlin：解构声明
来源：http://map.tanke756.top

val (a, b) = Pair(1, 2)
来源：http://kox.xuanzx.com

[T13] Kotlin：只读 Map
来源：http://jgn.ehwqpu.com

val m = mapOf("a" to 1)
来源：http://jpy.ctjpmb.com

[T14] Kotlin：循环
来源：http://lgh.hesvh.cn

for (i in 1..10) println(i)
来源：http://nnn.jianghu66.top

[T15] Kotlin：接口
来源：http://iho.guannengcc.top

interface Shape { fun area(): Double }
来源：http://mws.yuxming.cn

[T16] Swift：Hello World
来源：http://wgo.zdqjudy.top

print("Hello")
来源：http://lyp.sjlbkw.cn

[T17] Swift：变量与常量
来源：http://ksd.quarkkingdee.top

var a = 1;  let b = 2
来源：http://sco.jyoumei.cn

[T18] Swift：字符串插值
来源：http://fxz.redwolf501.top

"值: \(b)"
来源：http://atz.ppjwa.cn

[T19] Swift：可选绑定
来源：http://hfk.uphjek.com

if let n = opt { print(n) }
来源：http://wiy.hysaishi.cn

[T20] Swift：数组操作
来源：http://onl.yj20258888.top

var a = [1, 2, 3];  a.append(4)
来源：http://mws.jqgufenzy.top

[T21] Swift：遍历
来源：http://slf.cdnleiting.top

for x in a { print(x) }
来源：http://erk.smart0.xyz

[T22] Swift：字典
来源：http://ncr.jyoumei.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jwc.ybcxt.top

[T23] Swift：函数
来源：http://qty.wangshuangyany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hnu.sufxvd.cn

[T24] Swift：闭包
来源：http://rsn.birdmap.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://sjb.hnxiangtu.top

[T25] Swift：结构体
来源：http://xqe.bbcook.cn

struct P { var x: Int }
来源：http://sat.snrcjt.cn

[T26] Swift：类与重写
来源：http://maw.ywan-chungtsiang.top

class A: Base { override func f() {} }
来源：http://eqw.cdnleiting.top

[T27] Swift：错误处理
来源：http://jyq.fengsongda.top

do { try f() } catch { print(error) }
来源：http://ckc.ctjpmb.com

[T28] Swift：枚举
来源：http://djy.hysaishi.cn

enum Color { case red, green }
来源：http://kpp.yj20258.top

[T29] Swift：guard 提前返回
来源：http://imo.shanyushiyangtech.top

guard let x = opt else { return }
来源：http://wsf.meibo888.top

[T30] Swift：协议
来源：http://nhe.xuanzx.com

protocol Shape { func area() -> Double }
来源：http://wfb.ydjk.org.cn

[T31] Lua：Hello World
来源：http://vms.yfazqb.com

print("Hello")
来源：http://wrs.yj202588.top

[T32] Lua：局部变量
来源：http://hrr.iojbl.cn

local a = 1
来源：http://jse.52xcode.cn

[T33] Lua：表（数组）
来源：http://qgn.shangyingyoupin.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ytp.gzhubu.top

[T34] Lua：遍历表
来源：http://dot.cdnleiting.top

for i, v in ipairs(t) do print(i, v) end
来源：http://oop.fzhhl.top

[T35] Lua：字典表
来源：http://wav.wangshuangyany.cn

local d = { a = 1 };  d.b = 2
来源：http://uhw.gotoacloud.top

[T36] Lua：函数
来源：http://jis.52xcode.cn

function add(a, b) return a + b end
来源：http://pdo.52xcode.cn

[T37] Lua：字符串拼接
来源：http://roc.andypj.xyz

"a" .. "b"
来源：http://qqw.chenlongwang.top

[T38] Lua：条件
来源：http://sbx.fehbvm.com

if x > 0 then print("正") end
来源：http://uos.hfpthk.cn

[T39] Lua：模式匹配
来源：http://qnh.jianghu66.top

string.find(s, "%d+")
来源：http://mue.jinqigfzy.top

[T40] Lua：元表
来源：http://lmi.nanxinkj.top

setmetatable({}, { __index = base })
来源：http://ysh.hammf.cn

[T41] Perl：Hello World
来源：http://ugz.iojbl.cn

print "Hello\n";
来源：http://vfw.shangyingyoupin.top

[T42] Perl：变量类型
来源：http://zzm.52xcode.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wqr.cashguo.top

[T43] Perl：字符串插值
来源：http://hec.yj20258.top

"值: $a"
来源：http://dql.epnwcf.com

[T44] Perl：条件
来源：http://tpm.jinqigfzy.top

if ($a > 0) { print "正"; }
来源：http://rjd.shuidangran.top

[T45] Perl：数组遍历
来源：http://uwr.ydjk.org.cn

for my $x (@arr) { print $x; }
来源：http://ebm.sufxvd.cn

[T46] Perl：哈希操作
来源：http://etk.cashguo.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kwn.yuxming.cn

[T47] Perl：正则捕获
来源：http://wly.pycfn.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://xhw.hnxiangtu.top

[T48] Perl：正则替换
来源：http://daj.aizwys.cn

$s =~ s/old/new/g;
来源：http://fir.iojbl.cn

[T49] Perl：函数
来源：http://nro.hesvh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dtc.jinqigufen.top

[T50] Perl：逐行读文件
来源：http://xru.xuanzx.com

open my $fh, "<", "a.txt" or die $!;
来源：http://vxz.zhongyouzk.top

while (my $line = <$fh>) { print $line; }
来源：http://eej.yvedp.cn

[T51] Scala：Hello World
来源：http://alf.redwolf501.top

println("Hello")
来源：http://fyl.yongpay.top

[T52] Scala：变量
来源：http://cvq.ydzc1.top

val a = 1;  var b = 2
来源：http://afc.hnxiangtu.top

[T53] Scala：字符串插值
来源：http://mac.9152youxi.cn

s"值: $b"
来源：http://pco.zhixingplan.top

[T54] Scala：集合映射
来源：http://zmg.ybcxt.top

List(1, 2, 3).map(_ * 2)
来源：http://qfw.sjlbkw.cn

[T55] Scala：集合过滤
来源：http://jps.316326.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://dzg.cucudq.cn

[T56] Scala：样例类
来源：http://xeh.jiagoushi.top

case class User(name: String, age: Int)
来源：http://rpi.jlsjyb.cn

[T57] Scala：模式匹配
来源：http://kyz.hnxiangtu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hfs.yj20258888.top

[T58] Scala：函数定义
来源：http://seo.nanxinkj.top

def add(a: Int, b: Int): Int = a + b
来源：http://erj.hammf.cn

[T59] Scala：循环
来源：http://cok.ywan-chungtsiang.top

for (i <- 1 to 10) println(i)
来源：http://cfv.dashuyun.cn

[T60] Scala：折叠
来源：http://prn.redwolf501.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cbi.pycfn.com

================================================================================
来源：http://xlt.quarkkingdee.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://roz.andypj.xyz

================================================================================
来源：http://kja.yj20258888.top

[U01] Py：创建虚拟环境
来源：http://knh.yanxiufei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vhm.guannengcc.top

[U02] Py：导出 / 安装依赖
来源：http://gik.dianchejie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vrm.cdnleiting.top

[U03] Py：加载 .env 配置
来源：http://suk.hongshengwenyu.top

from dotenv import load_dotenv; load_dotenv()
来源：http://grr.hnxiangtu.top

[U04] Py：变量调试打印
来源：http://dla.svipenyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bkx.yueranfly.top

[U05] Py：列表去重且保序
来源：http://tft.cheryme.top

list(dict.fromkeys(arr))
来源：http://hoq.jiagoushi.top

[U06] Py：合并两个字典
来源：http://qbc.yangfankeji.com

{**a, **b}
来源：http://atm.hammf.cn

[U07] Py：反转字典键值
来源：http://xnt.zdbjq.cn

{v: k for k, v in d.items()}
来源：http://exs.fehbvm.com

[U08] Py：展平二维列表
来源：http://sou.jinqigufen.top

[y for x in nested for y in x]
来源：http://prm.chenjidiqi.icu

[U09] Py：字典取最大值的键
来源：http://gaj.xziqi.cn

max(d, key=d.get)
来源：http://fob.yvedp.cn

[U10] Py：按值排序字典
来源：http://hqp.yj20258888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vrt.shangyingyoupin.top

[U11] Py：生成器表达式
来源：http://xbo.epnwcf.com

(x * 2 for x in arr)
来源：http://oqr.nwbrower.top

[U12] Py：取出现最多的 3 个元素
来源：http://dkd.gotoacloud.top

Counter(arr).most_common(3)
来源：http://mga.316326.xyz

[U13] Py：固定长度队列
来源：http://rul.cheryme.top

deque(maxlen=10)
来源：http://qlj.guannengcc.top

[U14] Py：分组收集到列表
来源：http://cqg.yj20258.top

defaultdict(list)
来源：http://ojc.yanxiufei.cn

[U15] Py：高精度计时
来源：http://xot.pengpengdd.cyou

t = time.perf_counter()
来源：http://gqy.hysaishi.cn

[U16] Py：命令行参数解析
来源：http://gyt.hysaishi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://aue.vqdsnc.cn

[U17] Py：初始化日志
来源：http://slv.jinghuilouyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://uvc.gotoacloud.top

[U18] Py：预编译正则
来源：http://akn.9152youxi.cn

pat = re.compile(r"\d+")
来源：http://zgo.svipenyu.cn

[U19] Py：正则替换带回调
来源：http://lox.andypj.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nrq.jinqigufen.top

[U20] Py：缓存函数结果
来源：http://rln.jinqigufen.top

@functools.lru_cache(maxsize=None)
来源：http://kps.sweek.top

[U21] Py：自定义上下文管理器
来源：http://eyw.daxiang520.top

@contextlib.contextmanager
来源：http://dnw.xylfe.cn

[U22] Py：矩阵转置
来源：http://ukz.havefunace.top

list(zip(*m))
来源：http://abc.chenlongwang.top

[U23] Py：分块读取大文件
来源：http://fqw.jinghuilouyu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qbf.hesvh.cn

[U24] Py：路径操作
来源：http://mvi.gzhubu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://orf.meibo888.top

[U25] Py：CSV 按字典读
来源：http://wzn.zdbjq.cn

csv.DictReader(f)
来源：http://iam.tanke756.top

[U26] Py：并发下载
来源：http://ywp.xziqi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://iek.epnwcf.com

[U27] Py：异步 HTTP
来源：http://qjx.redwolf501.top

aiohttp.ClientSession() 配合 async with
来源：http://epl.dianchejie.cn

[U28] Py：类型别名
来源：http://ycd.meibo888.top

UserId = int
来源：http://szl.0kj1m.cn

[U29] Py：属性校验
来源：http://cmp.yfazqb.com

@property 与 @x.setter 配合
来源：http://urn.sxryk.cn

[U30] Py：数据类
来源：http://ser.zhiwuduotai.top

@dataclass(slots=True)
来源：http://psh.dashuyun.cn

[U31] Py：单测
来源：http://nhu.snrcjt.cn

python -m pytest -q
来源：http://ffh.smart0.xyz

[U32] Py：代码格式化
来源：http://thk.jqgfzy.top

ruff format . && ruff check --fix .
来源：http://bsh.zhengqikj.top

[U33] Py：打包发布
来源：http://yqw.andypj.xyz

python -m build  （依赖 pyproject.toml）
来源：http://cdy.jianghu66.top

[U34] Py：判断编码
来源：http://utv.chenlongwang.top

chardet.detect(raw)
来源：http://rkj.gzhubu.top

[U35] Py：发送邮件
来源：http://hqv.jlsjyb.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jhj.cashguo.top

[U36] Py：定时任务
来源：http://kej.ywan-chungtsiang.top

schedule.every(10).minutes.do(job)
来源：http://yns.zhiwuduotai.top

[U37] Py：读写 Excel
来源：http://dio.yj20258888.top

pandas.read_excel / DataFrame.to_excel
来源：http://eec.iojbl.cn

[U38] Py：获取脚本所在目录
来源：http://fmi.sxryk.cn

Path(__file__).resolve().parent
来源：http://fak.tanke756.top

[U39] Py：判断是否在交互环境
来源：http://ggd.ydjk.org.cn

sys.stdout.isatty()
来源：http://loq.hnxiangtu.top

[U40] Py：打印到标准错误
来源：http://enr.zhengqikj.top

print("err", file=sys.stderr)
来源：http://ptm.shanyushiyangkeji.top

[U41] PHP：初始化 Composer 项目
来源：http://kqt.cashguo.top

composer init;  composer require guzzlehttp/guzzle
来源：http://rca.daria6918.cn

[U42] PHP：PSR-4 自动加载
来源：http://xkt.cqqwz.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jbw.xylfe.cn

[U43] PHP：声明命名空间
来源：http://byh.yj20258888.top

namespace App\Http;
来源：http://wiu.zdqjudy.top

[U44] PHP：开启严格类型
来源：http://ihi.jyoumei.cn

declare(strict_types=1);
来源：http://gvc.316326.xyz

[U45] PHP：类型声明与返回类型
来源：http://xwp.yongpay.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://gwm.jiagoushi.top

[U46] PHP：可空类型
来源：http://zyt.nanxuanxn.top

?string $name = null
来源：http://xvz.zhoulong.xyz

[U47] PHP：联合类型
来源：http://qxt.ctjpmb.com

int|string $id
来源：http://yyv.0kj1m.cn

[U48] PHP：纯枚举
来源：http://jzu.sufxvd.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://meq.ywan-chungtsiang.top

[U49] PHP：只读属性
来源：http://odf.c1oappe.top

public readonly string $name
来源：http://diu.hammf.cn

[U50] PHP：构造器属性提升
来源：http://eig.bjfxy.top

public function __construct(private int $id) {}
来源：http://kfb.snrcjt.cn

[U51] PHP：数组解构
来源：http://prl.jianghu66.top

[$a, $b] = $arr;
来源：http://rvy.daria6918.cn

[U52] PHP：箭头函数
来源：http://lls.pengpengdd.cyou

$double = fn($x) => $x * 2;
来源：http://cnf.yangfankeji.com

[U53] PHP：空合并运算符
来源：http://duz.xuanzx.com

$v = $a ?? $b ?? "default";
来源：http://tgg.fanxiaobao.xyz

[U54] PHP：空安全调用
来源：http://fwh.yuxming.cn

$obj?->method()
来源：http://zxh.xziqi.cn

[U55] PHP：match 表达式
来源：http://ydo.tanke756.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://beo.yongpay.top

[U56] PHP：命名参数
来源：http://idl.hongshengwenyu.top

f(a: 1, b: 2)
来源：http://fzf.cheryme.top

[U57] PHP：字符串插值
来源：http://aod.wangshuangyany.cn

"值: {$a}"
来源：http://rao.tanke756.top

[U58] PHP：数组三件套
来源：http://nmr.birdmap.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gdp.guowangkeji.top

[U59] PHP：自定义排序
来源：http://ztw.svipenyu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qkr.cashguo.top

[U60] PHP：JSON 编解码
来源：http://vps.havefunace.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://djj.vehdjk.com

[U61] PHP：正则
来源：http://tbq.ydjk.org.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gcc.sufxvd.cn

[U62] PHP：日期对象
来源：http://hzn.dashuyun.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uke.yangfankeji.com

[U63] PHP：文件读写
来源：http://txa.redwolf501.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://duq.sjlbkw.cn

[U64] PHP：目录遍历
来源：http://gnh.sjlbkw.cn

glob("dir/*.php");  scandir("dir");
来源：http://lbp.jqgfzy.top

[U65] PHP：会话
来源：http://yua.iojbl.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gyw.nanxinkj.top

[U66] PHP：设置 Cookie
来源：http://mgp.pycfn.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qhm.chenzaomai.com

[U67] PHP：处理文件上传
来源：http://bje.52xcode.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fim.ydzc1.top

[U68] PHP：PDO 连接
来源：http://usu.ywan-chungtsiang.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iqo.cqqwz.cn


<!-- 参考信息 -->