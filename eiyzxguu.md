代发 wailian999

while (std::getline(in, line)) { }
来源：http://hfd.jqgfzy.top

[S49] C++：写文件
来源：http://zbc.cashguo.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://usy.zhiwuduotai.top

[S50] C++：格式化数字
来源：http://ewb.yj20258.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pra.zhixingplan.top

[S51] C++：显式类型转换
来源：http://hyo.jqgfzy.top

static_cast<double>(a) / b
来源：http://ahz.ydzc1.top

[S52] C++：const 与 noexcept
来源：http://meg.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://xcp.shanyushiyangtech.top

[S53] C++：移动语义
来源：http://xib.havefunace.top

std::vector<int> w = std::move(v);
来源：http://dhu.zdbjq.cn

[S54] C++：异常处理
来源：http://mey.cdnleiting.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://csf.uphjek.com

[S55] C++：结构化绑定
来源：http://cdf.sweek.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nxt.hesvh.cn

[S56] C++：optional
来源：http://zme.hfpthk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iug.hywenlv.cn

[S57] C++：编译期常量
来源：http://oqz.nanxuanxn.top

constexpr int N = 10;
来源：http://yfq.ydjk.org.cn

[S58] C++：命名空间
来源：http://ibr.ydzc1.top

namespace ns { int f() { return 1; } }
来源：http://smx.yongpay.top

[S59] C++：静态断言
来源：http://naj.yvedp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ugd.guowangkeji.top

[S60] C++：遍历并删除元素
来源：http://chu.vehdjk.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://asp.jiagoushi.top

================================================================================
来源：http://rgg.sxryk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ath.bjfxy.top

================================================================================
来源：http://uqu.yongpay.top

[T01] Kotlin：Hello World
来源：http://cjj.cheryme.top

println("Hello")
来源：http://vcn.zhiwuduotai.top

[T02] Kotlin：变量
来源：http://sxm.tarul.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vvt.chenlongwang.top

[T03] Kotlin：字符串模板
来源：http://bjj.aibaodan.cn

"值: $b"
来源：http://hae.daria6918.cn

[T04] Kotlin：空安全
来源：http://moo.c1oappe.top

val n: String? = null;  n?.length
来源：http://opn.yueranfly.top

[T05] Kotlin：when 表达式
来源：http://jzz.pycfn.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hcy.ybcxt.top

[T06] Kotlin：集合映射
来源：http://jsv.sweek.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nsm.ywan-chungtsiang.top

[T07] Kotlin：集合过滤
来源：http://xgi.zhongyouzk.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://utr.feifeiyinyue.top

[T08] Kotlin：数据类
来源：http://ctw.xziqi.cn

data class User(val name: String, val age: Int)
来源：http://gfe.gzhubu.top

[T09] Kotlin：扩展函数
来源：http://ets.wangdashe.top

fun String.exclaim() = this + "!"
来源：http://jus.xziqi.cn

[T10] Kotlin：默认参数
来源：http://nld.yj20258.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wjx.shanyushiyangtech.top

[T11] Kotlin：协程
来源：http://qig.chenzaomai.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://gxl.zhijiandao.cn

[T12] Kotlin：解构声明
来源：http://ppe.hcnkem.com

val (a, b) = Pair(1, 2)
来源：http://scc.haohaochexian.top

[T13] Kotlin：只读 Map
来源：http://ztf.pengpengdd.cyou

val m = mapOf("a" to 1)
来源：http://elh.hnqzz.top

[T14] Kotlin：循环
来源：http://yre.zycfv.cn

for (i in 1..10) println(i)
来源：http://rea.yj20258888.top

[T15] Kotlin：接口
来源：http://xlg.ppjwa.cn

interface Shape { fun area(): Double }
来源：http://kve.cdnleiting.top

[T16] Swift：Hello World
来源：http://qkw.hongshengwenyu.top

print("Hello")
来源：http://nad.sxryk.cn

[T17] Swift：变量与常量
来源：http://ytt.hongshengwenyu.top

var a = 1;  let b = 2
来源：http://sht.fanxiaobao.xyz

[T18] Swift：字符串插值
来源：http://exq.fktsv.cn

"值: \(b)"
来源：http://ghz.jianghu66.top

[T19] Swift：可选绑定
来源：http://jhi.shangyingyoupin.top

if let n = opt { print(n) }
来源：http://ksx.shzxlz.cn

[T20] Swift：数组操作
来源：http://ixc.yueranfly.top

var a = [1, 2, 3];  a.append(4)
来源：http://edh.zdqjudy.top

[T21] Swift：遍历
来源：http://ymt.jinghuilouyu.cn

for x in a { print(x) }
来源：http://fyn.hnqzz.top

[T22] Swift：字典
来源：http://iod.jianghu66.top

var d = ["a": 1];  d["b"] = 2
来源：http://mmt.redwolf501.top

[T23] Swift：函数
来源：http://nlp.yj202588.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hty.zycfv.cn

[T24] Swift：闭包
来源：http://ten.cdnleiting.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wuc.zhiwuduotai.top

[T25] Swift：结构体
来源：http://wcu.feifeiyinyue.top

struct P { var x: Int }
来源：http://bvd.wangshuangyany.cn

[T26] Swift：类与重写
来源：http://sby.zhongyouzk.top

class A: Base { override func f() {} }
来源：http://nkb.tanke756.top

[T27] Swift：错误处理
来源：http://vhb.snrcjt.cn

do { try f() } catch { print(error) }
来源：http://tyj.yfazqb.com

[T28] Swift：枚举
来源：http://tgc.xuetiantiany.cn

enum Color { case red, green }
来源：http://hnh.9152youxi.cn

[T29] Swift：guard 提前返回
来源：http://fmc.c1oappe.top

guard let x = opt else { return }
来源：http://mmp.shzxlz.cn

[T30] Swift：协议
来源：http://zez.aibaodan.cn

protocol Shape { func area() -> Double }
来源：http://yrs.guannengcc.top

[T31] Lua：Hello World
来源：http://lxf.epnwcf.com

print("Hello")
来源：http://zxt.vehdjk.com

[T32] Lua：局部变量
来源：http://lxv.52xcode.cn

local a = 1
来源：http://llm.smart0.xyz

[T33] Lua：表（数组）
来源：http://wor.cqqwz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wym.bjfxy.top

[T34] Lua：遍历表
来源：http://rnt.ydzc1.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rjo.hysaishi.cn

[T35] Lua：字典表
来源：http://beu.fehbvm.com

local d = { a = 1 };  d.b = 2
来源：http://xuy.cucudq.cn

[T36] Lua：函数
来源：http://uzl.zdqjudy.top

function add(a, b) return a + b end
来源：http://xux.ehwqpu.com

[T37] Lua：字符串拼接
来源：http://ynx.nwbrower.top

"a" .. "b"
来源：http://gtm.tanke756.top

[T38] Lua：条件
来源：http://dxb.meibo888.top

if x > 0 then print("正") end
来源：http://zyo.tarul.cn

[T39] Lua：模式匹配
来源：http://bxq.hongshengwenyu.top

string.find(s, "%d+")
来源：http://axh.hongshengwenyu.top

[T40] Lua：元表
来源：http://yrx.snrcjt.cn

setmetatable({}, { __index = base })
来源：http://cgv.zhijiandao.cn

[T41] Perl：Hello World
来源：http://tue.redwolf501.top

print "Hello\n";
来源：http://jka.hcnkem.com

[T42] Perl：变量类型
来源：http://lei.snrcjt.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://muj.jiagoushi.top

[T43] Perl：字符串插值
来源：http://skd.nwbrower.top

"值: $a"
来源：http://fmo.pycfn.com

[T44] Perl：条件
来源：http://gie.xingfuxueyuan.xyz

if ($a > 0) { print "正"; }
来源：http://jrb.fktsv.cn

[T45] Perl：数组遍历
来源：http://wng.chenjidiqi.icu

for my $x (@arr) { print $x; }
来源：http://mma.jyoumei.cn

[T46] Perl：哈希操作
来源：http://vdy.jqgufenzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mbe.cucudq.cn

[T47] Perl：正则捕获
来源：http://jvi.ivvv.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://wzt.gogol.net.cn

[T48] Perl：正则替换
来源：http://zec.ydjk.org.cn

$s =~ s/old/new/g;
来源：http://lxo.hnqzz.top

[T49] Perl：函数
来源：http://ztv.yj20258888.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cie.ivvv.top

[T50] Perl：逐行读文件
来源：http://xsw.cucudq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bmg.wangdashe.top

while (my $line = <$fh>) { print $line; }
来源：http://ona.haohaochexian.top

[T51] Scala：Hello World
来源：http://qgd.sjlbkw.cn

println("Hello")
来源：http://erp.zhijiandao.cn

[T52] Scala：变量
来源：http://yix.hammf.cn

val a = 1;  var b = 2
来源：http://kum.xziqi.cn

[T53] Scala：字符串插值
来源：http://trt.sxryk.cn

s"值: $b"
来源：http://kmo.xingfuxueyuan.xyz

[T54] Scala：集合映射
来源：http://tlr.jinqigufen.top

List(1, 2, 3).map(_ * 2)
来源：http://mjf.gotoacloud.top

[T55] Scala：集合过滤
来源：http://fbs.cheryme.top

List(1, 2, 3).filter(_ > 1)
来源：http://zcp.hnxiangtu.top

[T56] Scala：样例类
来源：http://xmd.hysaishi.cn

case class User(name: String, age: Int)
来源：http://xzf.pengpengdd.cyou

[T57] Scala：模式匹配
来源：http://mxr.zhaomingkeji.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://dyp.nanxinkj.top

[T58] Scala：函数定义
来源：http://flp.jqgfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://ruc.hywenlv.cn

[T59] Scala：循环
来源：http://azi.birdmap.top

for (i <- 1 to 10) println(i)
来源：http://hqp.xingfuxueyuan.xyz

[T60] Scala：折叠
来源：http://cdz.meibo888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pen.xuanzx.com

================================================================================
来源：http://jmw.yj20258.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vio.ivvv.top

================================================================================
来源：http://pnx.ybcxt.top

[U01] Py：创建虚拟环境
来源：http://icw.yj202588.top

python -m venv .venv && source .venv/bin/activate
来源：http://nhi.shzxlz.cn

[U02] Py：导出 / 安装依赖
来源：http://syg.mhx1999.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ytm.xylfe.cn

[U03] Py：加载 .env 配置
来源：http://gyt.daria6918.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rra.yvedp.cn

[U04] Py：变量调试打印
来源：http://lgt.hongshengwenyu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lnx.316326.xyz

[U05] Py：列表去重且保序
来源：http://yfk.jqgfzy.top

list(dict.fromkeys(arr))
来源：http://dof.fanxiaobao.xyz

[U06] Py：合并两个字典
来源：http://jrm.aizwys.cn

{**a, **b}
来源：http://oqe.shanyushiyangkeji.top

[U07] Py：反转字典键值
来源：http://qdl.ivvv.top

{v: k for k, v in d.items()}
来源：http://kom.chenzaomai.com

[U08] Py：展平二维列表
来源：http://snx.shanyushiyangkeji.top

[y for x in nested for y in x]
来源：http://ped.daria6918.cn

[U09] Py：字典取最大值的键
来源：http://rpv.zdqjudy.top

max(d, key=d.get)
来源：http://kih.yongpay.top

[U10] Py：按值排序字典
来源：http://qns.zhiwuduotai.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cri.jianghu66.top

[U11] Py：生成器表达式
来源：http://ikn.pengpengdd.cyou

(x * 2 for x in arr)
来源：http://toh.cqqwz.cn

[U12] Py：取出现最多的 3 个元素
来源：http://srq.shzxlz.cn

Counter(arr).most_common(3)
来源：http://eeq.shuidangran.top

[U13] Py：固定长度队列
来源：http://tcm.nwbrower.top

deque(maxlen=10)
来源：http://wyr.316326.xyz

[U14] Py：分组收集到列表
来源：http://wti.hywenlv.cn

defaultdict(list)
来源：http://qzh.zhongyouzk.top

[U15] Py：高精度计时
来源：http://ssq.meibo888.top

t = time.perf_counter()
来源：http://kcu.ctjpmb.com

[U16] Py：命令行参数解析
来源：http://okf.sysykeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nhs.sjlbkw.cn

[U17] Py：初始化日志
来源：http://jlj.jinghuilouyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://ctl.ppjwa.cn

[U18] Py：预编译正则
来源：http://fym.sysykeji.top

pat = re.compile(r"\d+")
来源：http://gpp.shanyushiyangkeji.top

[U19] Py：正则替换带回调
来源：http://axk.sweek.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://txi.zycfv.cn

[U20] Py：缓存函数结果
来源：http://ipl.zhongyouzk.top

@functools.lru_cache(maxsize=None)
来源：http://qbr.feifeiyinyue.top

[U21] Py：自定义上下文管理器
来源：http://hrq.uphjek.com

@contextlib.contextmanager
来源：http://eky.yuanzhike.top

[U22] Py：矩阵转置
来源：http://toq.yvedp.cn

list(zip(*m))
来源：http://npw.jyoumei.cn

[U23] Py：分块读取大文件
来源：http://sic.cqqwz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ngh.aibaodan.cn

[U24] Py：路径操作
来源：http://rok.daxiang520.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yme.zhaomingkeji.xyz

[U25] Py：CSV 按字典读
来源：http://isx.hnxiangtu.top

csv.DictReader(f)
来源：http://bpw.ctjpmb.com

[U26] Py：并发下载
来源：http://hup.52xcode.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cvu.gaohongyu789.top

[U27] Py：异步 HTTP
来源：http://bwn.yongpay.top

aiohttp.ClientSession() 配合 async with
来源：http://bjm.zhoulong.xyz

[U28] Py：类型别名
来源：http://ziw.hywenlv.cn

UserId = int
来源：http://wlo.zhengqikj.top

[U29] Py：属性校验
来源：http://jba.bbcook.cn

@property 与 @x.setter 配合
来源：http://eem.snrcjt.cn

[U30] Py：数据类
来源：http://cjy.shzxlz.cn

@dataclass(slots=True)
来源：http://nyq.chenlongwang.top

[U31] Py：单测
来源：http://twj.snrcjt.cn

python -m pytest -q
来源：http://lky.yuanzhike.top

[U32] Py：代码格式化
来源：http://kbb.cdnleiting.top

ruff format . && ruff check --fix .
来源：http://von.ybcxt.top

[U33] Py：打包发布
来源：http://tnv.birdmap.top

python -m build  （依赖 pyproject.toml）
来源：http://wkp.vqdsnc.cn

[U34] Py：判断编码
来源：http://num.bjfxy.top

chardet.detect(raw)
来源：http://lcp.feifeiyinyue.top

[U35] Py：发送邮件
来源：http://sje.birdmap.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://edi.guowangkeji.top

[U36] Py：定时任务
来源：http://juy.redwolf501.top

schedule.every(10).minutes.do(job)
来源：http://ihe.c1oappe.top

[U37] Py：读写 Excel
来源：http://gor.dianchejie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vjr.redwolf501.top

[U38] Py：获取脚本所在目录
来源：http://zrn.tarul.cn

Path(__file__).resolve().parent
来源：http://tve.mhx1999.top

[U39] Py：判断是否在交互环境
来源：http://dxw.fanxiaobao.xyz

sys.stdout.isatty()
来源：http://ipc.cqqwz.cn

[U40] Py：打印到标准错误
来源：http://oer.xingfuxueyuan.xyz

print("err", file=sys.stderr)
来源：http://tzm.yuanzhike.top

[U41] PHP：初始化 Composer 项目
来源：http://oxx.shanyushiyangtech.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vif.gaohongyu789.top

[U42] PHP：PSR-4 自动加载
来源：http://evk.chenjidiqi.icu

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qra.cheryme.top

[U43] PHP：声明命名空间
来源：http://djg.smart0.xyz

namespace App\Http;
来源：http://tjc.yangfankeji.com

[U44] PHP：开启严格类型
来源：http://rhl.vehdjk.com

declare(strict_types=1);
来源：http://six.hcnkem.com

[U45] PHP：类型声明与返回类型
来源：http://xyu.shanyushiyangtech.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qij.gotoacloud.top

[U46] PHP：可空类型
来源：http://lbj.sxryk.cn

?string $name = null
来源：http://xco.hfpthk.cn

[U47] PHP：联合类型
来源：http://gsd.smart0.xyz

int|string $id
来源：http://wle.xinyue.icu

[U48] PHP：纯枚举
来源：http://isb.shanyushiyangtech.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://era.gaohongyu789.top

[U49] PHP：只读属性
来源：http://jfh.yongpay.top

public readonly string $name
来源：http://yvv.smart0.xyz

[U50] PHP：构造器属性提升
来源：http://opg.tianlin.xyz

public function __construct(private int $id) {}
来源：http://xzs.ppjwa.cn

[U51] PHP：数组解构
来源：http://ecp.epnwcf.com

[$a, $b] = $arr;
来源：http://iqj.yj20258.top

[U52] PHP：箭头函数
来源：http://bsf.sufxvd.cn

$double = fn($x) => $x * 2;
来源：http://qno.havefunace.top

[U53] PHP：空合并运算符
来源：http://bgt.wangdashe.top

$v = $a ?? $b ?? "default";
来源：http://zsg.wangshuangyany.cn

[U54] PHP：空安全调用
来源：http://jkk.pengpengdd.cyou

$obj?->method()
来源：http://hnv.sxryk.cn

[U55] PHP：match 表达式
来源：http://zsk.xingfuxueyuan.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uar.cdnleiting.top

[U56] PHP：命名参数
来源：http://mug.jiagoushi.top

f(a: 1, b: 2)
来源：http://vjw.hywenlv.cn

[U57] PHP：字符串插值
来源：http://fqt.jinqigfzy.top

"值: {$a}"
来源：http://lth.yj20258888.top

[U58] PHP：数组三件套
来源：http://vpf.snrcjt.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ufa.iojbl.cn

[U59] PHP：自定义排序
来源：http://qlu.sxryk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pgq.gotoacloud.top

[U60] PHP：JSON 编解码
来源：http://wpj.jinqigufen.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zov.wangshuangyany.cn

[U61] PHP：正则
来源：http://qgq.yfazqb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://elv.yongpay.top

[U62] PHP：日期对象
来源：http://yff.bjfxy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ykq.hcnkem.com

[U63] PHP：文件读写
来源：http://cee.gotoacloud.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xwm.shanyushiyangtech.top

[U64] PHP：目录遍历
来源：http://img.vqdsnc.cn

glob("dir/*.php");  scandir("dir");
来源：http://vop.cucudq.cn

[U65] PHP：会话
来源：http://ejt.0kj1m.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://upy.zhoulong.xyz

[U66] PHP：设置 Cookie
来源：http://kom.hfpthk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hmp.dianchejie.cn

[U67] PHP：处理文件上传
来源：http://muj.zdqjudy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dpf.uphjek.com

[U68] PHP：PDO 连接
来源：http://vhs.jiagoushi.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://unm.vehdjk.com

[U69] PHP：PDO 预处理
来源：http://xso.zdqjudy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qes.9152youxi.cn

[U70] PHP：PDO 事务
来源：http://zxa.zhoulong.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tzq.birdmap.top

[U71] PHP：抛出异常
来源：http://euq.quarkkingdee.top

throw new RuntimeException("失败", 500);
来源：http://hbq.zhongyouzk.top

[U72] PHP：写错误日志
来源：http://vaz.nwbrower.top

error_log("失败: " . $e->getMessage());
来源：http://iuq.xuetiantiany.cn

[U73] PHP：读取 ini 配置
来源：http://pfn.shanyushiyangkeji.top

parse_ini_file("config.ini", true)
来源：http://vdo.haohaochexian.top

[U74] PHP：读取环境变量
来源：http://rih.sysykeji.top

getenv("APP_ENV") ?: "production"
来源：http://wys.yueranfly.top


<!-- 参考信息 -->