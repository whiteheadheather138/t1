代发 wailian999

while (std::getline(in, line)) { }
来源：http://jxm.svipenyu.cn

[S49] C++：写文件
来源：http://myo.zhaomingkeji.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blp.zhaomingkeji.xyz

[S50] C++：格式化数字
来源：http://pqi.cashguo.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mbt.havefunace.top

[S51] C++：显式类型转换
来源：http://wms.cdnleiting.top

static_cast<double>(a) / b
来源：http://eqy.fktsv.cn

[S52] C++：const 与 noexcept
来源：http://zwz.hcnkem.com

int size() const noexcept { return n_; }
来源：http://zfq.jinghuilouyu.cn

[S53] C++：移动语义
来源：http://ume.andypj.xyz

std::vector<int> w = std::move(v);
来源：http://wfu.jlsjyb.cn

[S54] C++：异常处理
来源：http://xor.yfazqb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dto.daxiang520.top

[S55] C++：结构化绑定
来源：http://dhk.vqdsnc.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ich.fengsongda.top

[S56] C++：optional
来源：http://owp.c1oappe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oax.sxryk.cn

[S57] C++：编译期常量
来源：http://rrj.xingfuxueyuan.xyz

constexpr int N = 10;
来源：http://srb.fanxiaobao.xyz

[S58] C++：命名空间
来源：http://zwf.bjfxy.top

namespace ns { int f() { return 1; } }
来源：http://iia.zdqjudy.top

[S59] C++：静态断言
来源：http://ykh.shangyingyoupin.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pcw.hnqzz.top

[S60] C++：遍历并删除元素
来源：http://yre.shanyushiyangtech.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pss.zdbjq.cn

================================================================================
来源：http://aep.jinqigufen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tjp.smart0.xyz

================================================================================
来源：http://qaw.dashuyun.cn

[T01] Kotlin：Hello World
来源：http://ojo.sxryk.cn

println("Hello")
来源：http://ggr.hnqzz.top

[T02] Kotlin：变量
来源：http://wax.hywenlv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://apf.shangyingyoupin.top

[T03] Kotlin：字符串模板
来源：http://jvc.gzhubu.top

"值: $b"
来源：http://tdq.birdmap.top

[T04] Kotlin：空安全
来源：http://kdb.52xcode.cn

val n: String? = null;  n?.length
来源：http://liy.xuanzx.com

[T05] Kotlin：when 表达式
来源：http://uyj.tian-w.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://obq.fzhhl.top

[T06] Kotlin：集合映射
来源：http://nox.aizwys.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nxa.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://hks.yanxiufei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dsg.dianchejie.cn

[T08] Kotlin：数据类
来源：http://wsf.jqgufenzy.top

data class User(val name: String, val age: Int)
来源：http://qwb.yueranfly.top

[T09] Kotlin：扩展函数
来源：http://rbf.316326.xyz

fun String.exclaim() = this + "!"
来源：http://jzs.jinqigfzy.top

[T10] Kotlin：默认参数
来源：http://gsz.gzhubu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://fkh.jinqigfzy.top

[T11] Kotlin：协程
来源：http://swd.kuanghao11.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://oio.yj20258.top

[T12] Kotlin：解构声明
来源：http://fgg.sysykeji.top

val (a, b) = Pair(1, 2)
来源：http://kke.sxryk.cn

[T13] Kotlin：只读 Map
来源：http://jsf.aizwys.cn

val m = mapOf("a" to 1)
来源：http://nvl.0kj1m.cn

[T14] Kotlin：循环
来源：http://oxe.yangfankeji.com

for (i in 1..10) println(i)
来源：http://weg.hnxiangtu.top

[T15] Kotlin：接口
来源：http://mmi.jyoumei.cn

interface Shape { fun area(): Double }
来源：http://ieh.sysykeji.top

[T16] Swift：Hello World
来源：http://spi.zhijiandao.cn

print("Hello")
来源：http://bnx.yuanzhike.top

[T17] Swift：变量与常量
来源：http://wlt.yueranfly.top

var a = 1;  let b = 2
来源：http://hdw.ywan-chungtsiang.top

[T18] Swift：字符串插值
来源：http://sav.hammf.cn

"值: \(b)"
来源：http://jyu.gotoacloud.top

[T19] Swift：可选绑定
来源：http://bzp.yj202588.top

if let n = opt { print(n) }
来源：http://unw.gogol.net.cn

[T20] Swift：数组操作
来源：http://wpp.tarul.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mnp.9152youxi.cn

[T21] Swift：遍历
来源：http://rbv.xinyue.icu

for x in a { print(x) }
来源：http://bxg.cdnleiting.top

[T22] Swift：字典
来源：http://cem.bjfxy.top

var d = ["a": 1];  d["b"] = 2
来源：http://vrf.zhijiandao.cn

[T23] Swift：函数
来源：http://kgr.hesvh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wws.smart0.xyz

[T24] Swift：闭包
来源：http://wtv.jinqigfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://oyp.mhx1999.top

[T25] Swift：结构体
来源：http://tly.xuanzx.com

struct P { var x: Int }
来源：http://rrb.gzhubu.top

[T26] Swift：类与重写
来源：http://sjx.fehbvm.com

class A: Base { override func f() {} }
来源：http://jld.dianchejie.cn

[T27] Swift：错误处理
来源：http://pcq.jiagoushi.top

do { try f() } catch { print(error) }
来源：http://iep.ybcxt.top

[T28] Swift：枚举
来源：http://ypg.aizwys.cn

enum Color { case red, green }
来源：http://edr.chenjidiqi.icu

[T29] Swift：guard 提前返回
来源：http://aki.yj20258.top

guard let x = opt else { return }
来源：http://cdd.nanxinkj.top

[T30] Swift：协议
来源：http://bmd.cdnleiting.top

protocol Shape { func area() -> Double }
来源：http://fke.zycfv.cn

[T31] Lua：Hello World
来源：http://qac.tian-w.cn

print("Hello")
来源：http://kvj.xziqi.cn

[T32] Lua：局部变量
来源：http://qei.xylfe.cn

local a = 1
来源：http://ras.yvedp.cn

[T33] Lua：表（数组）
来源：http://qhm.xuetiantiany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zpg.daria6918.cn

[T34] Lua：遍历表
来源：http://rmy.mhx1999.top

for i, v in ipairs(t) do print(i, v) end
来源：http://pws.smart0.xyz

[T35] Lua：字典表
来源：http://wdz.ppjwa.cn

local d = { a = 1 };  d.b = 2
来源：http://glt.hnqzz.top

[T36] Lua：函数
来源：http://spu.hysaishi.cn

function add(a, b) return a + b end
来源：http://edl.yonumen.top

[T37] Lua：字符串拼接
来源：http://uvb.cashguo.top

"a" .. "b"
来源：http://wld.sxryk.cn

[T38] Lua：条件
来源：http://vtv.aizwys.cn

if x > 0 then print("正") end
来源：http://fbp.shzxlz.cn

[T39] Lua：模式匹配
来源：http://mtu.hcnkem.com

string.find(s, "%d+")
来源：http://ejw.fanxiaobao.xyz

[T40] Lua：元表
来源：http://cqa.chenjidiqi.icu

setmetatable({}, { __index = base })
来源：http://aee.yj202588.top

[T41] Perl：Hello World
来源：http://qpb.52xcode.cn

print "Hello\n";
来源：http://nud.chenzaomai.com

[T42] Perl：变量类型
来源：http://tak.yuxming.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://czd.jinqigufen.top

[T43] Perl：字符串插值
来源：http://jem.mhx1999.top

"值: $a"
来源：http://xeo.sysykeji.top

[T44] Perl：条件
来源：http://hno.yongpay.top

if ($a > 0) { print "正"; }
来源：http://brd.xylfe.cn

[T45] Perl：数组遍历
来源：http://ttn.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://xmt.havefunace.top

[T46] Perl：哈希操作
来源：http://urb.gaohongyu789.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vxv.xuetiantiany.cn

[T47] Perl：正则捕获
来源：http://nni.jlsjyb.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://uso.iojbl.cn

[T48] Perl：正则替换
来源：http://uyh.gaohongyu789.top

$s =~ s/old/new/g;
来源：http://khz.gogol.net.cn

[T49] Perl：函数
来源：http://snu.fanxiaobao.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wyk.guannengcc.top

[T50] Perl：逐行读文件
来源：http://jts.jianghu66.top

open my $fh, "<", "a.txt" or die $!;
来源：http://wfb.zhaomingkeji.xyz

while (my $line = <$fh>) { print $line; }
来源：http://rpp.yfazqb.com

[T51] Scala：Hello World
来源：http://lox.svipenyu.cn

println("Hello")
来源：http://xob.guannengcc.top

[T52] Scala：变量
来源：http://hlp.jqgufenzy.top

val a = 1;  var b = 2
来源：http://blv.nanxuanxn.top

[T53] Scala：字符串插值
来源：http://lve.ydjk.org.cn

s"值: $b"
来源：http://oaf.ivvv.top

[T54] Scala：集合映射
来源：http://fdn.sysykeji.top

List(1, 2, 3).map(_ * 2)
来源：http://ajb.dashuyun.cn

[T55] Scala：集合过滤
来源：http://xmi.zhengqikj.top

List(1, 2, 3).filter(_ > 1)
来源：http://tse.ybcxt.top

[T56] Scala：样例类
来源：http://nnx.guowangkeji.top

case class User(name: String, age: Int)
来源：http://yqu.fehbvm.com

[T57] Scala：模式匹配
来源：http://lxe.hywenlv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kfm.zhixingplan.top

[T58] Scala：函数定义
来源：http://gks.jqgufenzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://svx.fengsongda.top

[T59] Scala：循环
来源：http://kmi.tarul.cn

for (i <- 1 to 10) println(i)
来源：http://bof.jinqigufen.top

[T60] Scala：折叠
来源：http://bca.tianlin.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ckp.zhoulong.xyz

================================================================================
来源：http://wcx.hnxiangtu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ord.meibo888.top

================================================================================
来源：http://wfe.shangyingyoupin.top

[U01] Py：创建虚拟环境
来源：http://xdx.yfazqb.com

python -m venv .venv && source .venv/bin/activate
来源：http://all.ywan-chungtsiang.top

[U02] Py：导出 / 安装依赖
来源：http://eqy.ctjpmb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lsf.meibo888.top

[U03] Py：加载 .env 配置
来源：http://hvr.jianghu66.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jne.ppjwa.cn

[U04] Py：变量调试打印
来源：http://tjs.mhx1999.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zqq.nanxinkj.top

[U05] Py：列表去重且保序
来源：http://qli.hnxiangtu.top

list(dict.fromkeys(arr))
来源：http://ftc.jinyuanbaomall.cn

[U06] Py：合并两个字典
来源：http://cav.ehwqpu.com

{**a, **b}
来源：http://qmy.chenjidiqi.icu

[U07] Py：反转字典键值
来源：http://zva.c1oappe.top

{v: k for k, v in d.items()}
来源：http://jzb.shangyingyoupin.top

[U08] Py：展平二维列表
来源：http://cxy.nanxuanxn.top

[y for x in nested for y in x]
来源：http://qla.xuanzx.com

[U09] Py：字典取最大值的键
来源：http://exz.pycfn.com

max(d, key=d.get)
来源：http://cxl.yueranfly.top

[U10] Py：按值排序字典
来源：http://itr.smart0.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://itv.jiagoushi.top

[U11] Py：生成器表达式
来源：http://jju.yj202588.top

(x * 2 for x in arr)
来源：http://cpw.yj20258888.top

[U12] Py：取出现最多的 3 个元素
来源：http://hll.yj20258888.top

Counter(arr).most_common(3)
来源：http://tue.aibaodan.cn

[U13] Py：固定长度队列
来源：http://ivh.xinyue.icu

deque(maxlen=10)
来源：http://wdp.pycfn.com

[U14] Py：分组收集到列表
来源：http://dxs.52xcode.cn

defaultdict(list)
来源：http://lgx.hammf.cn

[U15] Py：高精度计时
来源：http://gpl.jqgfzy.top

t = time.perf_counter()
来源：http://aah.zhiwuduotai.top

[U16] Py：命令行参数解析
来源：http://lvz.fanxiaobao.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jag.zhiwuduotai.top

[U17] Py：初始化日志
来源：http://ymv.wangshuangyany.cn

logging.basicConfig(level=logging.INFO)
来源：http://yap.zhoulong.xyz

[U18] Py：预编译正则
来源：http://jnd.xuanzx.com

pat = re.compile(r"\d+")
来源：http://hio.birdmap.top

[U19] Py：正则替换带回调
来源：http://ird.zhaomingkeji.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://efv.zhaomingkeji.xyz

[U20] Py：缓存函数结果
来源：http://geo.ydjk.org.cn

@functools.lru_cache(maxsize=None)
来源：http://fjz.jqgufenzy.top

[U21] Py：自定义上下文管理器
来源：http://tpu.epnwcf.com

@contextlib.contextmanager
来源：http://jcl.yanxiufei.cn

[U22] Py：矩阵转置
来源：http://yis.nanxuanxn.top

list(zip(*m))
来源：http://knr.mhx1999.top

[U23] Py：分块读取大文件
来源：http://hcp.xziqi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://joa.vqdsnc.cn

[U24] Py：路径操作
来源：http://myt.guowangkeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jsr.hfpthk.cn

[U25] Py：CSV 按字典读
来源：http://pnv.ivvv.top

csv.DictReader(f)
来源：http://wlx.cdnleiting.top

[U26] Py：并发下载
来源：http://nah.svipenyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://agm.daxiang520.top

[U27] Py：异步 HTTP
来源：http://zoy.hcnkem.com

aiohttp.ClientSession() 配合 async with
来源：http://gzb.hysaishi.cn

[U28] Py：类型别名
来源：http://ist.hammf.cn

UserId = int
来源：http://ocp.316326.xyz

[U29] Py：属性校验
来源：http://wcy.shanyushiyangkeji.top

@property 与 @x.setter 配合
来源：http://ufo.yangfankeji.com

[U30] Py：数据类
来源：http://vbv.sweek.top

@dataclass(slots=True)
来源：http://adv.jinghuilouyu.cn

[U31] Py：单测
来源：http://odk.hfpthk.cn

python -m pytest -q
来源：http://khp.hongshengwenyu.top

[U32] Py：代码格式化
来源：http://iud.ydjk.org.cn

ruff format . && ruff check --fix .
来源：http://yab.epnwcf.com

[U33] Py：打包发布
来源：http://fxm.c1oappe.top

python -m build  （依赖 pyproject.toml）
来源：http://nwm.9152youxi.cn

[U34] Py：判断编码
来源：http://cfh.316326.xyz

chardet.detect(raw)
来源：http://ghq.cashguo.top

[U35] Py：发送邮件
来源：http://dkj.xingfuxueyuan.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gav.jianghu66.top

[U36] Py：定时任务
来源：http://lli.hammf.cn

schedule.every(10).minutes.do(job)
来源：http://pkq.yueranfly.top

[U37] Py：读写 Excel
来源：http://bnp.yanxiufei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ryy.yonumen.top

[U38] Py：获取脚本所在目录
来源：http://zqp.yonumen.top

Path(__file__).resolve().parent
来源：http://ksd.tanke756.top

[U39] Py：判断是否在交互环境
来源：http://gmn.dashuyun.cn

sys.stdout.isatty()
来源：http://heq.cheryme.top

[U40] Py：打印到标准错误
来源：http://yzh.xuanzx.com

print("err", file=sys.stderr)
来源：http://vnj.ydjk.org.cn

[U41] PHP：初始化 Composer 项目
来源：http://pvu.birdmap.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fcx.xziqi.cn

[U42] PHP：PSR-4 自动加载
来源：http://yjx.wangshuangyany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://glq.yfazqb.com

[U43] PHP：声明命名空间
来源：http://jhx.hongshengwenyu.top

namespace App\Http;
来源：http://evp.tanke756.top

[U44] PHP：开启严格类型
来源：http://rqi.zdqjudy.top

declare(strict_types=1);
来源：http://qhn.jiagoushi.top

[U45] PHP：类型声明与返回类型
来源：http://psy.jyoumei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ncy.0kj1m.cn

[U46] PHP：可空类型
来源：http://vhy.xinyue.icu

?string $name = null
来源：http://jpw.zhijiandao.cn

[U47] PHP：联合类型
来源：http://rbj.shuidangran.top

int|string $id
来源：http://lsd.gaohongyu789.top

[U48] PHP：纯枚举
来源：http://jtf.jinqigufen.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zdc.pengpengdd.cyou

[U49] PHP：只读属性
来源：http://uzy.hesvh.cn

public readonly string $name
来源：http://hco.ydjk.org.cn

[U50] PHP：构造器属性提升
来源：http://vzc.snrcjt.cn

public function __construct(private int $id) {}
来源：http://pwe.tian-w.cn

[U51] PHP：数组解构
来源：http://hao.jqgfzy.top

[$a, $b] = $arr;
来源：http://nfs.tanke756.top

[U52] PHP：箭头函数
来源：http://daw.sweek.top

$double = fn($x) => $x * 2;
来源：http://pvq.kuanghao11.cn

[U53] PHP：空合并运算符
来源：http://qds.xuanzx.com

$v = $a ?? $b ?? "default";
来源：http://cub.zhaomingkeji.xyz

[U54] PHP：空安全调用
来源：http://vpc.ydjk.org.cn

$obj?->method()
来源：http://udb.ctjpmb.com

[U55] PHP：match 表达式
来源：http://pnc.cqqwz.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iga.yvedp.cn

[U56] PHP：命名参数
来源：http://fnz.pycfn.com

f(a: 1, b: 2)
来源：http://jty.ivvv.top

[U57] PHP：字符串插值
来源：http://vxc.xuanzx.com

"值: {$a}"
来源：http://qcw.jinghuilouyu.cn

[U58] PHP：数组三件套
来源：http://bvc.yj20258888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rdr.svipenyu.cn

[U59] PHP：自定义排序
来源：http://rxz.mhx1999.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wjh.ywan-chungtsiang.top

[U60] PHP：JSON 编解码
来源：http://vad.hnqzz.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dxi.ydzc1.top

[U61] PHP：正则
来源：http://eye.snrcjt.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nja.xinyue.icu

[U62] PHP：日期对象
来源：http://iys.tian-w.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://agg.uphjek.com

[U63] PHP：文件读写
来源：http://zcg.tarul.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jyy.zhixingplan.top

[U64] PHP：目录遍历
来源：http://nhw.yfazqb.com

glob("dir/*.php");  scandir("dir");
来源：http://gqo.jinqigufen.top

[U65] PHP：会话
来源：http://ede.xinyue.icu

session_start();  $_SESSION["uid"] = 1;
来源：http://xkz.guannengcc.top

[U66] PHP：设置 Cookie
来源：http://vwq.cdnleiting.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wkq.zhixingplan.top

[U67] PHP：处理文件上传
来源：http://usf.sweek.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nas.wangdashe.top

[U68] PHP：PDO 连接
来源：http://ngj.sufxvd.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rin.zhoulong.xyz

[U69] PHP：PDO 预处理
来源：http://fvc.epnwcf.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yve.tianlin.xyz

[U70] PHP：PDO 事务
来源：http://rmm.316326.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qjy.sjlbkw.cn

[U71] PHP：抛出异常
来源：http://wim.hnqzz.top

throw new RuntimeException("失败", 500);
来源：http://bko.52xcode.cn

[U72] PHP：写错误日志
来源：http://mmx.daria6918.cn

error_log("失败: " . $e->getMessage());
来源：http://ltz.daria6918.cn

[U73] PHP：读取 ini 配置
来源：http://ofa.ctjpmb.com

parse_ini_file("config.ini", true)
来源：http://hos.nanxuanxn.top

[U74] PHP：读取环境变量
来源：http://zpi.meibo888.top

getenv("APP_ENV") ?: "production"
来源：http://bff.0kj1m.cn


<!-- 参考信息 -->