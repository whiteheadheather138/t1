代发 wailian999

while (std::getline(in, line)) { }
来源：http://obw.jinqigfzy.top

[S49] C++：写文件
来源：http://yba.hnxiangtu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bdi.hnxiangtu.top

[S50] C++：格式化数字
来源：http://dxe.aizwys.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zmd.hammf.cn

[S51] C++：显式类型转换
来源：http://gam.ehwqpu.com

static_cast<double>(a) / b
来源：http://oct.shuidangran.top

[S52] C++：const 与 noexcept
来源：http://kap.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://geu.cucudq.cn

[S53] C++：移动语义
来源：http://hvc.ivvv.top

std::vector<int> w = std::move(v);
来源：http://acs.zhoulong.xyz

[S54] C++：异常处理
来源：http://rgb.gogol.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ovn.tianlin.xyz

[S55] C++：结构化绑定
来源：http://gax.pengpengdd.cyou

auto [a, b] = std::make_pair(1, 2);
来源：http://hho.shuidangran.top

[S56] C++：optional
来源：http://azm.hnxiangtu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://msj.jinyuanbaomall.cn

[S57] C++：编译期常量
来源：http://cba.xuanzx.com

constexpr int N = 10;
来源：http://kcj.fehbvm.com

[S58] C++：命名空间
来源：http://pcf.sxryk.cn

namespace ns { int f() { return 1; } }
来源：http://wwa.aizwys.cn

[S59] C++：静态断言
来源：http://stz.jqgufenzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qqi.guowangkeji.top

[S60] C++：遍历并删除元素
来源：http://lhm.xziqi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cbo.epnwcf.com

================================================================================
来源：http://ery.gogol.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lwt.bbcook.cn

================================================================================
来源：http://gwf.dashuyun.cn

[T01] Kotlin：Hello World
来源：http://bnl.vehdjk.com

println("Hello")
来源：http://pvz.zhijiandao.cn

[T02] Kotlin：变量
来源：http://xxv.ivvv.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jxw.hammf.cn

[T03] Kotlin：字符串模板
来源：http://mkf.daria6918.cn

"值: $b"
来源：http://xhq.xylfe.cn

[T04] Kotlin：空安全
来源：http://ffa.yongpay.top

val n: String? = null;  n?.length
来源：http://cro.gaohongyu789.top

[T05] Kotlin：when 表达式
来源：http://ays.vehdjk.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ddb.yongpay.top

[T06] Kotlin：集合映射
来源：http://nzx.feifeiyinyue.top

listOf(1, 2, 3).map { it * 2 }
来源：http://iwm.yfazqb.com

[T07] Kotlin：集合过滤
来源：http://pee.snrcjt.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://odl.zhaomingkeji.xyz

[T08] Kotlin：数据类
来源：http://cil.zhoulong.xyz

data class User(val name: String, val age: Int)
来源：http://yrr.zhengqikj.top

[T09] Kotlin：扩展函数
来源：http://dyx.snrcjt.cn

fun String.exclaim() = this + "!"
来源：http://axa.meibo888.top

[T10] Kotlin：默认参数
来源：http://xwd.fanxiaobao.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://hyh.daria6918.cn

[T11] Kotlin：协程
来源：http://ilq.snrcjt.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hlc.52xcode.cn

[T12] Kotlin：解构声明
来源：http://pcm.guannengcc.top

val (a, b) = Pair(1, 2)
来源：http://mkk.cdnleiting.top

[T13] Kotlin：只读 Map
来源：http://swr.xuanzx.com

val m = mapOf("a" to 1)
来源：http://vrk.shuidangran.top

[T14] Kotlin：循环
来源：http://isd.hongshengwenyu.top

for (i in 1..10) println(i)
来源：http://pxz.zhixingplan.top

[T15] Kotlin：接口
来源：http://zyc.fengsongda.top

interface Shape { fun area(): Double }
来源：http://gxl.nwbrower.top

[T16] Swift：Hello World
来源：http://ogy.zhoulong.xyz

print("Hello")
来源：http://kwd.andypj.xyz

[T17] Swift：变量与常量
来源：http://tnt.hongshengwenyu.top

var a = 1;  let b = 2
来源：http://gul.yvedp.cn

[T18] Swift：字符串插值
来源：http://owp.c1oappe.top

"值: \(b)"
来源：http://rjl.zhaomingkeji.xyz

[T19] Swift：可选绑定
来源：http://ifw.snrcjt.cn

if let n = opt { print(n) }
来源：http://pnp.haohaochexian.top

[T20] Swift：数组操作
来源：http://mrw.guowangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://kgv.bbcook.cn

[T21] Swift：遍历
来源：http://nis.guowangkeji.top

for x in a { print(x) }
来源：http://unh.cqqwz.cn

[T22] Swift：字典
来源：http://prb.guannengcc.top

var d = ["a": 1];  d["b"] = 2
来源：http://jhz.havefunace.top

[T23] Swift：函数
来源：http://icx.pengpengdd.cyou

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://quu.vehdjk.com

[T24] Swift：闭包
来源：http://ecr.yongpay.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hnw.hnqzz.top

[T25] Swift：结构体
来源：http://srh.cheryme.top

struct P { var x: Int }
来源：http://rfb.iojbl.cn

[T26] Swift：类与重写
来源：http://par.fengsongda.top

class A: Base { override func f() {} }
来源：http://rju.daxiang520.top

[T27] Swift：错误处理
来源：http://mxu.jqgufenzy.top

do { try f() } catch { print(error) }
来源：http://qes.shanyushiyangtech.top

[T28] Swift：枚举
来源：http://ywp.hysaishi.cn

enum Color { case red, green }
来源：http://ame.jyoumei.cn

[T29] Swift：guard 提前返回
来源：http://rti.sweek.top

guard let x = opt else { return }
来源：http://izc.wangdashe.top

[T30] Swift：协议
来源：http://ifd.guannengcc.top

protocol Shape { func area() -> Double }
来源：http://wma.jyoumei.cn

[T31] Lua：Hello World
来源：http://onx.epnwcf.com

print("Hello")
来源：http://fav.yangfankeji.com

[T32] Lua：局部变量
来源：http://eru.iojbl.cn

local a = 1
来源：http://wtp.sweek.top

[T33] Lua：表（数组）
来源：http://vcn.fanxiaobao.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://zuf.xuetiantiany.cn

[T34] Lua：遍历表
来源：http://xif.hcnkem.com

for i, v in ipairs(t) do print(i, v) end
来源：http://zlv.bjfxy.top

[T35] Lua：字典表
来源：http://ick.hfpthk.cn

local d = { a = 1 };  d.b = 2
来源：http://mkn.xziqi.cn

[T36] Lua：函数
来源：http://ggh.xuanzx.com

function add(a, b) return a + b end
来源：http://qbj.gaohongyu789.top

[T37] Lua：字符串拼接
来源：http://efx.iojbl.cn

"a" .. "b"
来源：http://gmz.hysaishi.cn

[T38] Lua：条件
来源：http://lbc.hnxiangtu.top

if x > 0 then print("正") end
来源：http://axy.bjfxy.top

[T39] Lua：模式匹配
来源：http://znf.zhijiandao.cn

string.find(s, "%d+")
来源：http://rpb.yonumen.top

[T40] Lua：元表
来源：http://nxu.gzhubu.top

setmetatable({}, { __index = base })
来源：http://yre.vehdjk.com

[T41] Perl：Hello World
来源：http://oyv.cqqwz.cn

print "Hello\n";
来源：http://jte.zhijiandao.cn

[T42] Perl：变量类型
来源：http://dcw.hammf.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fzw.52xcode.cn

[T43] Perl：字符串插值
来源：http://cmi.pycfn.com

"值: $a"
来源：http://twl.jinyuanbaomall.cn

[T44] Perl：条件
来源：http://peh.wangshuangyany.cn

if ($a > 0) { print "正"; }
来源：http://fwg.cashguo.top

[T45] Perl：数组遍历
来源：http://vmm.ctjpmb.com

for my $x (@arr) { print $x; }
来源：http://eqx.hnqzz.top

[T46] Perl：哈希操作
来源：http://ppz.iojbl.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rij.zhongyouzk.top

[T47] Perl：正则捕获
来源：http://bma.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hva.ydzc1.top

[T48] Perl：正则替换
来源：http://jfb.zhixingplan.top

$s =~ s/old/new/g;
来源：http://qxs.fktsv.cn

[T49] Perl：函数
来源：http://hns.sufxvd.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://czc.zhoulong.xyz

[T50] Perl：逐行读文件
来源：http://nho.shangyingyoupin.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nvp.jinyuanbaomall.cn

while (my $line = <$fh>) { print $line; }
来源：http://vad.hywenlv.cn

[T51] Scala：Hello World
来源：http://jhy.bbcook.cn

println("Hello")
来源：http://aax.zhoulong.xyz

[T52] Scala：变量
来源：http://ucb.yj202588.top

val a = 1;  var b = 2
来源：http://ncw.hnqzz.top

[T53] Scala：字符串插值
来源：http://ysf.shanyushiyangkeji.top

s"值: $b"
来源：http://czv.ydjk.org.cn

[T54] Scala：集合映射
来源：http://nbd.shanyushiyangtech.top

List(1, 2, 3).map(_ * 2)
来源：http://wre.shzxlz.cn

[T55] Scala：集合过滤
来源：http://vtl.shuidangran.top

List(1, 2, 3).filter(_ > 1)
来源：http://igp.pycfn.com

[T56] Scala：样例类
来源：http://qmh.yuxming.cn

case class User(name: String, age: Int)
来源：http://ldm.jlsjyb.cn

[T57] Scala：模式匹配
来源：http://hxi.zdbjq.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wsx.nwbrower.top

[T58] Scala：函数定义
来源：http://ohl.ivvv.top

def add(a: Int, b: Int): Int = a + b
来源：http://cnu.ivvv.top

[T59] Scala：循环
来源：http://waw.zdbjq.cn

for (i <- 1 to 10) println(i)
来源：http://moa.vehdjk.com

[T60] Scala：折叠
来源：http://gnl.pengpengdd.cyou

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fvi.shanyushiyangkeji.top

================================================================================
来源：http://tup.ydzc1.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pft.chenzaomai.com

================================================================================
来源：http://emt.meibo888.top

[U01] Py：创建虚拟环境
来源：http://oso.chenjidiqi.icu

python -m venv .venv && source .venv/bin/activate
来源：http://zez.tarul.cn

[U02] Py：导出 / 安装依赖
来源：http://ogs.meibo888.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kme.hywenlv.cn

[U03] Py：加载 .env 配置
来源：http://phc.feifeiyinyue.top

from dotenv import load_dotenv; load_dotenv()
来源：http://odg.sysykeji.top

[U04] Py：变量调试打印
来源：http://xfj.yj202588.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hcu.dianchejie.cn

[U05] Py：列表去重且保序
来源：http://wrc.chenzaomai.com

list(dict.fromkeys(arr))
来源：http://nqw.ivvv.top

[U06] Py：合并两个字典
来源：http://ckq.zhijiandao.cn

{**a, **b}
来源：http://uby.dashuyun.cn

[U07] Py：反转字典键值
来源：http://aoj.yonumen.top

{v: k for k, v in d.items()}
来源：http://joq.shanyushiyangkeji.top

[U08] Py：展平二维列表
来源：http://gba.xylfe.cn

[y for x in nested for y in x]
来源：http://kyu.gaohongyu789.top

[U09] Py：字典取最大值的键
来源：http://wes.guowangkeji.top

max(d, key=d.get)
来源：http://qum.gaohongyu789.top

[U10] Py：按值排序字典
来源：http://pce.hcnkem.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jkt.hnqzz.top

[U11] Py：生成器表达式
来源：http://lbw.316326.xyz

(x * 2 for x in arr)
来源：http://kmn.quarkkingdee.top

[U12] Py：取出现最多的 3 个元素
来源：http://dpp.yj20258888.top

Counter(arr).most_common(3)
来源：http://nwl.sysykeji.top

[U13] Py：固定长度队列
来源：http://ylk.hnqzz.top

deque(maxlen=10)
来源：http://jhb.ydjk.org.cn

[U14] Py：分组收集到列表
来源：http://ztq.jianghu66.top

defaultdict(list)
来源：http://scg.zdqjudy.top

[U15] Py：高精度计时
来源：http://jtb.9152youxi.cn

t = time.perf_counter()
来源：http://gzw.fanxiaobao.xyz

[U16] Py：命令行参数解析
来源：http://ibd.cucudq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lht.gzhubu.top

[U17] Py：初始化日志
来源：http://vpj.tanke756.top

logging.basicConfig(level=logging.INFO)
来源：http://kzj.tanke756.top

[U18] Py：预编译正则
来源：http://isf.redwolf501.top

pat = re.compile(r"\d+")
来源：http://qhc.shanyushiyangkeji.top

[U19] Py：正则替换带回调
来源：http://ppe.feifeiyinyue.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tgu.nanxinkj.top

[U20] Py：缓存函数结果
来源：http://wir.shanyushiyangtech.top

@functools.lru_cache(maxsize=None)
来源：http://jmw.xziqi.cn

[U21] Py：自定义上下文管理器
来源：http://odb.nwbrower.top

@contextlib.contextmanager
来源：http://imt.gzhubu.top

[U22] Py：矩阵转置
来源：http://dsl.hfpthk.cn

list(zip(*m))
来源：http://wku.jiagoushi.top

[U23] Py：分块读取大文件
来源：http://kyi.nwbrower.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gze.hcnkem.com

[U24] Py：路径操作
来源：http://lyy.c1oappe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wdt.zdbjq.cn

[U25] Py：CSV 按字典读
来源：http://uhh.haohaochexian.top

csv.DictReader(f)
来源：http://gwj.jianghu66.top

[U26] Py：并发下载
来源：http://xhm.gogol.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jxf.yuanzhike.top

[U27] Py：异步 HTTP
来源：http://peg.chenzaomai.com

aiohttp.ClientSession() 配合 async with
来源：http://vfm.jinqigufen.top

[U28] Py：类型别名
来源：http://fsx.hammf.cn

UserId = int
来源：http://ksl.yj20258.top

[U29] Py：属性校验
来源：http://myj.fanxiaobao.xyz

@property 与 @x.setter 配合
来源：http://vcr.gotoacloud.top

[U30] Py：数据类
来源：http://rzh.jinyuanbaomall.cn

@dataclass(slots=True)
来源：http://mgx.dashuyun.cn

[U31] Py：单测
来源：http://pfc.uphjek.com

python -m pytest -q
来源：http://oph.52xcode.cn

[U32] Py：代码格式化
来源：http://edl.shanyushiyangkeji.top

ruff format . && ruff check --fix .
来源：http://kia.snrcjt.cn

[U33] Py：打包发布
来源：http://iux.hcnkem.com

python -m build  （依赖 pyproject.toml）
来源：http://nmb.zdqjudy.top

[U34] Py：判断编码
来源：http://hgj.xinyue.icu

chardet.detect(raw)
来源：http://equ.iojbl.cn

[U35] Py：发送邮件
来源：http://pea.yj202588.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://szl.hywenlv.cn

[U36] Py：定时任务
来源：http://wea.jyoumei.cn

schedule.every(10).minutes.do(job)
来源：http://hdy.ctjpmb.com

[U37] Py：读写 Excel
来源：http://kjw.quarkkingdee.top

pandas.read_excel / DataFrame.to_excel
来源：http://cet.chenjidiqi.icu

[U38] Py：获取脚本所在目录
来源：http://geb.hywenlv.cn

Path(__file__).resolve().parent
来源：http://ezf.redwolf501.top

[U39] Py：判断是否在交互环境
来源：http://ssz.yanxiufei.cn

sys.stdout.isatty()
来源：http://tup.fengsongda.top

[U40] Py：打印到标准错误
来源：http://evb.yueranfly.top

print("err", file=sys.stderr)
来源：http://jib.yj20258888.top

[U41] PHP：初始化 Composer 项目
来源：http://lza.jyoumei.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://spb.hesvh.cn

[U42] PHP：PSR-4 自动加载
来源：http://xdy.sweek.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cae.kuanghao11.cn

[U43] PHP：声明命名空间
来源：http://vrh.cheryme.top

namespace App\Http;
来源：http://ihn.meibo888.top

[U44] PHP：开启严格类型
来源：http://czi.jqgfzy.top

declare(strict_types=1);
来源：http://ppm.9152youxi.cn

[U45] PHP：类型声明与返回类型
来源：http://ghg.tarul.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ozv.quarkkingdee.top

[U46] PHP：可空类型
来源：http://jjz.tanke756.top

?string $name = null
来源：http://scg.yfazqb.com

[U47] PHP：联合类型
来源：http://gkl.yfazqb.com

int|string $id
来源：http://sbj.yj20258888.top

[U48] PHP：纯枚举
来源：http://wxf.zdqjudy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vam.wangdashe.top

[U49] PHP：只读属性
来源：http://bdk.shanyushiyangkeji.top

public readonly string $name
来源：http://znf.shanyushiyangkeji.top

[U50] PHP：构造器属性提升
来源：http://ezy.yj20258888.top

public function __construct(private int $id) {}
来源：http://byq.cheryme.top

[U51] PHP：数组解构
来源：http://ehu.tarul.cn

[$a, $b] = $arr;
来源：http://taj.ydjk.org.cn

[U52] PHP：箭头函数
来源：http://olk.wangshuangyany.cn

$double = fn($x) => $x * 2;
来源：http://roo.zhijiandao.cn

[U53] PHP：空合并运算符
来源：http://wwq.cdnleiting.top

$v = $a ?? $b ?? "default";
来源：http://nmt.shanyushiyangkeji.top

[U54] PHP：空安全调用
来源：http://gtw.ppjwa.cn

$obj?->method()
来源：http://wmm.fanxiaobao.xyz

[U55] PHP：match 表达式
来源：http://dwn.guowangkeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yzx.ppjwa.cn

[U56] PHP：命名参数
来源：http://hec.cdnleiting.top

f(a: 1, b: 2)
来源：http://ieo.jyoumei.cn

[U57] PHP：字符串插值
来源：http://pxu.iojbl.cn

"值: {$a}"
来源：http://yiu.zhixingplan.top

[U58] PHP：数组三件套
来源：http://qdi.yfazqb.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iwx.jinqigfzy.top

[U59] PHP：自定义排序
来源：http://zjz.zhoulong.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qpn.zhiwuduotai.top

[U60] PHP：JSON 编解码
来源：http://thl.gotoacloud.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nma.gogol.net.cn

[U61] PHP：正则
来源：http://pbq.nanxinkj.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://shd.chenlongwang.top

[U62] PHP：日期对象
来源：http://aao.yangfankeji.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ler.yuanzhike.top

[U63] PHP：文件读写
来源：http://gzc.ydjk.org.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://onl.zhengqikj.top

[U64] PHP：目录遍历
来源：http://sev.xuetiantiany.cn

glob("dir/*.php");  scandir("dir");
来源：http://wlx.yangfankeji.com

[U65] PHP：会话
来源：http://nde.fengsongda.top

session_start();  $_SESSION["uid"] = 1;
来源：http://spg.sjlbkw.cn

[U66] PHP：设置 Cookie
来源：http://pip.birdmap.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ebt.tianlin.xyz

[U67] PHP：处理文件上传
来源：http://cyu.sufxvd.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://eto.shanyushiyangkeji.top

[U68] PHP：PDO 连接
来源：http://awk.xylfe.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gwx.vehdjk.com

[U69] PHP：PDO 预处理
来源：http://zwj.guannengcc.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wac.yueranfly.top

[U70] PHP：PDO 事务
来源：http://tqo.shangyingyoupin.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://biu.jinghuilouyu.cn

[U71] PHP：抛出异常
来源：http://fjw.daria6918.cn

throw new RuntimeException("失败", 500);
来源：http://smt.wangshuangyany.cn

[U72] PHP：写错误日志
来源：http://isi.hysaishi.cn

error_log("失败: " . $e->getMessage());
来源：http://vuv.jlsjyb.cn

[U73] PHP：读取 ini 配置
来源：http://lga.fehbvm.com

parse_ini_file("config.ini", true)
来源：http://ctn.9152youxi.cn

[U74] PHP：读取环境变量
来源：http://yfk.pycfn.com

getenv("APP_ENV") ?: "production"
来源：http://srk.nanxinkj.top


<!-- 参考信息 -->