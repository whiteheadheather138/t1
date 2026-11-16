代发 wailian999

while (std::getline(in, line)) { }
来源：http://kap.c1oappe.top

[S49] C++：写文件
来源：http://blp.zhiwuduotai.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bji.hfpthk.cn

[S50] C++：格式化数字
来源：http://wyr.ywan-chungtsiang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zfd.pycfn.com

[S51] C++：显式类型转换
来源：http://iax.yuxming.cn

static_cast<double>(a) / b
来源：http://vcd.andypj.xyz

[S52] C++：const 与 noexcept
来源：http://nfr.vehdjk.com

int size() const noexcept { return n_; }
来源：http://apx.bjfxy.top

[S53] C++：移动语义
来源：http://jqz.zhixingplan.top

std::vector<int> w = std::move(v);
来源：http://mib.shanyushiyangkeji.top

[S54] C++：异常处理
来源：http://dtm.gzhubu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wht.0kj1m.cn

[S55] C++：结构化绑定
来源：http://axd.0kj1m.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wxt.fzhhl.top

[S56] C++：optional
来源：http://pss.sufxvd.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fjz.jyoumei.cn

[S57] C++：编译期常量
来源：http://iyh.svipenyu.cn

constexpr int N = 10;
来源：http://ujq.pengpengdd.cyou

[S58] C++：命名空间
来源：http://klw.havefunace.top

namespace ns { int f() { return 1; } }
来源：http://rtz.daria6918.cn

[S59] C++：静态断言
来源：http://htx.uphjek.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rvu.vehdjk.com

[S60] C++：遍历并删除元素
来源：http://eol.gaohongyu789.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://isn.yj20258888.top

================================================================================
来源：http://aif.svipenyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://efi.yangfankeji.com

================================================================================
来源：http://jvu.daxiang520.top

[T01] Kotlin：Hello World
来源：http://hgx.kuanghao11.cn

println("Hello")
来源：http://gqo.fzhhl.top

[T02] Kotlin：变量
来源：http://shy.zdbjq.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cmy.hfpthk.cn

[T03] Kotlin：字符串模板
来源：http://vso.yangfankeji.com

"值: $b"
来源：http://ymp.ppjwa.cn

[T04] Kotlin：空安全
来源：http://qfa.yvedp.cn

val n: String? = null;  n?.length
来源：http://ehp.aizwys.cn

[T05] Kotlin：when 表达式
来源：http://lue.hcnkem.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://huf.fanxiaobao.xyz

[T06] Kotlin：集合映射
来源：http://cdm.sweek.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zml.sufxvd.cn

[T07] Kotlin：集合过滤
来源：http://wup.redwolf501.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vck.ppjwa.cn

[T08] Kotlin：数据类
来源：http://rab.zdqjudy.top

data class User(val name: String, val age: Int)
来源：http://xdy.mhx1999.top

[T09] Kotlin：扩展函数
来源：http://ovh.gaohongyu789.top

fun String.exclaim() = this + "!"
来源：http://qgc.cqqwz.cn

[T10] Kotlin：默认参数
来源：http://yif.haohaochexian.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gfz.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://ypo.zhixingplan.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://dio.wangshuangyany.cn

[T12] Kotlin：解构声明
来源：http://wwb.svipenyu.cn

val (a, b) = Pair(1, 2)
来源：http://iae.dianchejie.cn

[T13] Kotlin：只读 Map
来源：http://qcw.jlsjyb.cn

val m = mapOf("a" to 1)
来源：http://mkp.wangdashe.top

[T14] Kotlin：循环
来源：http://xir.nanxuanxn.top

for (i in 1..10) println(i)
来源：http://kzb.cucudq.cn

[T15] Kotlin：接口
来源：http://uja.ydzc1.top

interface Shape { fun area(): Double }
来源：http://kno.feifeiyinyue.top

[T16] Swift：Hello World
来源：http://hqo.zdqjudy.top

print("Hello")
来源：http://lrg.aizwys.cn

[T17] Swift：变量与常量
来源：http://ymh.wangshuangyany.cn

var a = 1;  let b = 2
来源：http://nad.ydzc1.top

[T18] Swift：字符串插值
来源：http://cqt.yanxiufei.cn

"值: \(b)"
来源：http://coj.guannengcc.top

[T19] Swift：可选绑定
来源：http://fyh.ehwqpu.com

if let n = opt { print(n) }
来源：http://xph.cdnleiting.top

[T20] Swift：数组操作
来源：http://wyj.ybcxt.top

var a = [1, 2, 3];  a.append(4)
来源：http://whr.daxiang520.top

[T21] Swift：遍历
来源：http://agn.birdmap.top

for x in a { print(x) }
来源：http://liq.fzhhl.top

[T22] Swift：字典
来源：http://srr.dashuyun.cn

var d = ["a": 1];  d["b"] = 2
来源：http://etv.cheryme.top

[T23] Swift：函数
来源：http://dtw.zdbjq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qrc.jinghuilouyu.cn

[T24] Swift：闭包
来源：http://acj.ctjpmb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://ncu.gzhubu.top

[T25] Swift：结构体
来源：http://ixj.yfazqb.com

struct P { var x: Int }
来源：http://ozf.guannengcc.top

[T26] Swift：类与重写
来源：http://ilq.hnqzz.top

class A: Base { override func f() {} }
来源：http://knu.yonumen.top

[T27] Swift：错误处理
来源：http://kxk.sufxvd.cn

do { try f() } catch { print(error) }
来源：http://efq.zdqjudy.top

[T28] Swift：枚举
来源：http://zqn.aizwys.cn

enum Color { case red, green }
来源：http://eho.bbcook.cn

[T29] Swift：guard 提前返回
来源：http://kuq.yonumen.top

guard let x = opt else { return }
来源：http://llz.hnqzz.top

[T30] Swift：协议
来源：http://hac.pengpengdd.cyou

protocol Shape { func area() -> Double }
来源：http://elp.gzhubu.top

[T31] Lua：Hello World
来源：http://sif.yangfankeji.com

print("Hello")
来源：http://cjq.mhx1999.top

[T32] Lua：局部变量
来源：http://alv.ivvv.top

local a = 1
来源：http://geu.xziqi.cn

[T33] Lua：表（数组）
来源：http://tkv.xziqi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bhs.nwbrower.top

[T34] Lua：遍历表
来源：http://vtp.fehbvm.com

for i, v in ipairs(t) do print(i, v) end
来源：http://kct.fengsongda.top

[T35] Lua：字典表
来源：http://qjr.cdnleiting.top

local d = { a = 1 };  d.b = 2
来源：http://owa.shangyingyoupin.top

[T36] Lua：函数
来源：http://swg.mhx1999.top

function add(a, b) return a + b end
来源：http://qhh.jinqigufen.top

[T37] Lua：字符串拼接
来源：http://mle.gzhubu.top

"a" .. "b"
来源：http://keq.gotoacloud.top

[T38] Lua：条件
来源：http://vte.hnqzz.top

if x > 0 then print("正") end
来源：http://hxo.9152youxi.cn

[T39] Lua：模式匹配
来源：http://wbp.fehbvm.com

string.find(s, "%d+")
来源：http://kok.yueranfly.top

[T40] Lua：元表
来源：http://itc.cucudq.cn

setmetatable({}, { __index = base })
来源：http://hwi.0kj1m.cn

[T41] Perl：Hello World
来源：http://czc.bjfxy.top

print "Hello\n";
来源：http://njk.ydzc1.top

[T42] Perl：变量类型
来源：http://xoa.meibo888.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bpa.yfazqb.com

[T43] Perl：字符串插值
来源：http://vxo.fzhhl.top

"值: $a"
来源：http://lgx.zhengqikj.top

[T44] Perl：条件
来源：http://rje.vehdjk.com

if ($a > 0) { print "正"; }
来源：http://ijo.daria6918.cn

[T45] Perl：数组遍历
来源：http://vpa.tanke756.top

for my $x (@arr) { print $x; }
来源：http://dgq.quarkkingdee.top

[T46] Perl：哈希操作
来源：http://ldm.aibaodan.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xdh.yongpay.top

[T47] Perl：正则捕获
来源：http://hkv.wangdashe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ewf.andypj.xyz

[T48] Perl：正则替换
来源：http://cxn.fengsongda.top

$s =~ s/old/new/g;
来源：http://ied.hcnkem.com

[T49] Perl：函数
来源：http://awk.aizwys.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wxx.yanxiufei.cn

[T50] Perl：逐行读文件
来源：http://hlv.kuanghao11.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mry.jianghu66.top

while (my $line = <$fh>) { print $line; }
来源：http://ipr.zdbjq.cn

[T51] Scala：Hello World
来源：http://oeo.52xcode.cn

println("Hello")
来源：http://urf.zhiwuduotai.top

[T52] Scala：变量
来源：http://amr.hnxiangtu.top

val a = 1;  var b = 2
来源：http://moi.xziqi.cn

[T53] Scala：字符串插值
来源：http://cfy.ydzc1.top

s"值: $b"
来源：http://nwq.fanxiaobao.xyz

[T54] Scala：集合映射
来源：http://xvj.cqqwz.cn

List(1, 2, 3).map(_ * 2)
来源：http://gdn.pengpengdd.cyou

[T55] Scala：集合过滤
来源：http://owt.jiagoushi.top

List(1, 2, 3).filter(_ > 1)
来源：http://upm.316326.xyz

[T56] Scala：样例类
来源：http://evm.aibaodan.cn

case class User(name: String, age: Int)
来源：http://gav.zycfv.cn

[T57] Scala：模式匹配
来源：http://mkv.yj202588.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fmh.cqqwz.cn

[T58] Scala：函数定义
来源：http://dot.vehdjk.com

def add(a: Int, b: Int): Int = a + b
来源：http://yza.daxiang520.top

[T59] Scala：循环
来源：http://yxb.mhx1999.top

for (i <- 1 to 10) println(i)
来源：http://zab.gogol.net.cn

[T60] Scala：折叠
来源：http://hle.jianghu66.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://knh.meibo888.top

================================================================================
来源：http://gbu.fengsongda.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oxz.fzhhl.top

================================================================================
来源：http://fmx.vehdjk.com

[U01] Py：创建虚拟环境
来源：http://iff.hysaishi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vjv.xuanzx.com

[U02] Py：导出 / 安装依赖
来源：http://trv.sjlbkw.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cky.dashuyun.cn

[U03] Py：加载 .env 配置
来源：http://zee.sxryk.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fiq.hnxiangtu.top

[U04] Py：变量调试打印
来源：http://xeb.havefunace.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nld.vqdsnc.cn

[U05] Py：列表去重且保序
来源：http://eoy.ydjk.org.cn

list(dict.fromkeys(arr))
来源：http://fmb.hammf.cn

[U06] Py：合并两个字典
来源：http://svf.yj20258888.top

{**a, **b}
来源：http://hnb.sjlbkw.cn

[U07] Py：反转字典键值
来源：http://wfh.shzxlz.cn

{v: k for k, v in d.items()}
来源：http://eps.haohaochexian.top

[U08] Py：展平二维列表
来源：http://dad.xinyue.icu

[y for x in nested for y in x]
来源：http://nrp.iojbl.cn

[U09] Py：字典取最大值的键
来源：http://vwv.zhongyouzk.top

max(d, key=d.get)
来源：http://vut.hysaishi.cn

[U10] Py：按值排序字典
来源：http://wxi.sxryk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ike.fzhhl.top

[U11] Py：生成器表达式
来源：http://jup.snrcjt.cn

(x * 2 for x in arr)
来源：http://tzm.zycfv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sky.nwbrower.top

Counter(arr).most_common(3)
来源：http://ohz.gotoacloud.top

[U13] Py：固定长度队列
来源：http://wpc.birdmap.top

deque(maxlen=10)
来源：http://nls.jiagoushi.top

[U14] Py：分组收集到列表
来源：http://sdr.fengsongda.top

defaultdict(list)
来源：http://ymh.bjfxy.top

[U15] Py：高精度计时
来源：http://cqe.yangfankeji.com

t = time.perf_counter()
来源：http://ciu.tanke756.top

[U16] Py：命令行参数解析
来源：http://loq.gogol.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zqx.daxiang520.top

[U17] Py：初始化日志
来源：http://vck.nanxuanxn.top

logging.basicConfig(level=logging.INFO)
来源：http://asv.andypj.xyz

[U18] Py：预编译正则
来源：http://hew.nwbrower.top

pat = re.compile(r"\d+")
来源：http://qaf.chenlongwang.top

[U19] Py：正则替换带回调
来源：http://efj.yj20258888.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://leh.gaohongyu789.top

[U20] Py：缓存函数结果
来源：http://ljm.snrcjt.cn

@functools.lru_cache(maxsize=None)
来源：http://ugh.wangdashe.top

[U21] Py：自定义上下文管理器
来源：http://oce.ehwqpu.com

@contextlib.contextmanager
来源：http://tnz.dianchejie.cn

[U22] Py：矩阵转置
来源：http://mci.xziqi.cn

list(zip(*m))
来源：http://mst.zhoulong.xyz

[U23] Py：分块读取大文件
来源：http://hkd.hysaishi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nxa.daxiang520.top

[U24] Py：路径操作
来源：http://ybd.yj202588.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mnm.hywenlv.cn

[U25] Py：CSV 按字典读
来源：http://asx.pycfn.com

csv.DictReader(f)
来源：http://jiz.zhaomingkeji.xyz

[U26] Py：并发下载
来源：http://uys.chenlongwang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wgn.hammf.cn

[U27] Py：异步 HTTP
来源：http://rpq.pycfn.com

aiohttp.ClientSession() 配合 async with
来源：http://hon.bjfxy.top

[U28] Py：类型别名
来源：http://fmr.andypj.xyz

UserId = int
来源：http://gfg.zhijiandao.cn

[U29] Py：属性校验
来源：http://yrp.gzhubu.top

@property 与 @x.setter 配合
来源：http://qvw.zhiwuduotai.top

[U30] Py：数据类
来源：http://zku.c1oappe.top

@dataclass(slots=True)
来源：http://dcs.jlsjyb.cn

[U31] Py：单测
来源：http://xhw.cheryme.top

python -m pytest -q
来源：http://xhq.sjlbkw.cn

[U32] Py：代码格式化
来源：http://eyd.sweek.top

ruff format . && ruff check --fix .
来源：http://eah.havefunace.top

[U33] Py：打包发布
来源：http://pcu.xingfuxueyuan.xyz

python -m build  （依赖 pyproject.toml）
来源：http://oim.zhixingplan.top

[U34] Py：判断编码
来源：http://iqv.fzhhl.top

chardet.detect(raw)
来源：http://eoe.haohaochexian.top

[U35] Py：发送邮件
来源：http://zeh.yvedp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dvr.chenlongwang.top

[U36] Py：定时任务
来源：http://eth.aizwys.cn

schedule.every(10).minutes.do(job)
来源：http://xqf.zhaomingkeji.xyz

[U37] Py：读写 Excel
来源：http://ysb.aibaodan.cn

pandas.read_excel / DataFrame.to_excel
来源：http://umk.cqqwz.cn

[U38] Py：获取脚本所在目录
来源：http://scd.snrcjt.cn

Path(__file__).resolve().parent
来源：http://ggc.xziqi.cn

[U39] Py：判断是否在交互环境
来源：http://gdw.zycfv.cn

sys.stdout.isatty()
来源：http://jcw.nwbrower.top

[U40] Py：打印到标准错误
来源：http://maz.zdqjudy.top

print("err", file=sys.stderr)
来源：http://jll.cucudq.cn

[U41] PHP：初始化 Composer 项目
来源：http://elk.0kj1m.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bee.ivvv.top

[U42] PHP：PSR-4 自动加载
来源：http://yfc.sjlbkw.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cpz.yueranfly.top

[U43] PHP：声明命名空间
来源：http://ysx.yj20258888.top

namespace App\Http;
来源：http://qwk.haohaochexian.top

[U44] PHP：开启严格类型
来源：http://bge.hnqzz.top

declare(strict_types=1);
来源：http://yiq.chenzaomai.com

[U45] PHP：类型声明与返回类型
来源：http://sgn.yj20258.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://sra.zhijiandao.cn

[U46] PHP：可空类型
来源：http://vak.xziqi.cn

?string $name = null
来源：http://tfx.hnxiangtu.top

[U47] PHP：联合类型
来源：http://yvh.pycfn.com

int|string $id
来源：http://kbl.cdnleiting.top

[U48] PHP：纯枚举
来源：http://jos.ydjk.org.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://brr.kuanghao11.cn

[U49] PHP：只读属性
来源：http://arf.c1oappe.top

public readonly string $name
来源：http://bdm.cashguo.top

[U50] PHP：构造器属性提升
来源：http://fpx.hfpthk.cn

public function __construct(private int $id) {}
来源：http://lcd.sxryk.cn

[U51] PHP：数组解构
来源：http://zya.tianlin.xyz

[$a, $b] = $arr;
来源：http://clu.ctjpmb.com

[U52] PHP：箭头函数
来源：http://xvx.ivvv.top

$double = fn($x) => $x * 2;
来源：http://und.yuanzhike.top

[U53] PHP：空合并运算符
来源：http://esp.hcnkem.com

$v = $a ?? $b ?? "default";
来源：http://rer.ehwqpu.com

[U54] PHP：空安全调用
来源：http://rww.fengsongda.top

$obj?->method()
来源：http://zif.sweek.top

[U55] PHP：match 表达式
来源：http://oyw.yvedp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vwr.xylfe.cn

[U56] PHP：命名参数
来源：http://jay.xylfe.cn

f(a: 1, b: 2)
来源：http://wgp.yj202588.top

[U57] PHP：字符串插值
来源：http://msr.hcnkem.com

"值: {$a}"
来源：http://gpa.havefunace.top

[U58] PHP：数组三件套
来源：http://ksj.dianchejie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rwz.guowangkeji.top

[U59] PHP：自定义排序
来源：http://llv.jlsjyb.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bmc.daria6918.cn

[U60] PHP：JSON 编解码
来源：http://inn.c1oappe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://szc.ctjpmb.com

[U61] PHP：正则
来源：http://kdf.cqqwz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://slr.hfpthk.cn

[U62] PHP：日期对象
来源：http://red.52xcode.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ffz.zhixingplan.top

[U63] PHP：文件读写
来源：http://nol.tanke756.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fyt.fktsv.cn

[U64] PHP：目录遍历
来源：http://rmn.wangdashe.top

glob("dir/*.php");  scandir("dir");
来源：http://jiq.tian-w.cn

[U65] PHP：会话
来源：http://pqa.yj20258.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vyx.gogol.net.cn

[U66] PHP：设置 Cookie
来源：http://bry.zhaomingkeji.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qpu.hnxiangtu.top

[U67] PHP：处理文件上传
来源：http://mgd.mhx1999.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nzc.9152youxi.cn

[U68] PHP：PDO 连接
来源：http://gsv.hesvh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rhv.ehwqpu.com

[U69] PHP：PDO 预处理
来源：http://emb.birdmap.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iyh.hammf.cn

[U70] PHP：PDO 事务
来源：http://ebs.dianchejie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zor.kuanghao11.cn

[U71] PHP：抛出异常
来源：http://ies.jqgfzy.top

throw new RuntimeException("失败", 500);
来源：http://arq.snrcjt.cn

[U72] PHP：写错误日志
来源：http://gmd.tanke756.top

error_log("失败: " . $e->getMessage());
来源：http://amb.vehdjk.com

[U73] PHP：读取 ini 配置
来源：http://ipt.hnxiangtu.top

parse_ini_file("config.ini", true)
来源：http://wne.dashuyun.cn

[U74] PHP：读取环境变量
来源：http://gom.zdqjudy.top

getenv("APP_ENV") ?: "production"
来源：http://iwl.daria6918.cn


<!-- 参考信息 -->