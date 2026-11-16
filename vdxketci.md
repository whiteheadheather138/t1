代发 wailian999

[S45] C++：lambda
来源：http://ebl.andypj.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://akf.zhaomingkeji.xyz

[S46] C++：函数模板
来源：http://nrt.zdbjq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://obw.bbcook.cn

[S47] C++：结构化绑定遍历
来源：http://axi.hammf.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wpp.yvedp.cn

[S48] C++：逐行读文件
来源：http://csp.cucudq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pvr.yuanzhike.top

while (std::getline(in, line)) { }
来源：http://sxy.zhixingplan.top

[S49] C++：写文件
来源：http://cxf.fzhhl.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kvl.zhengqikj.top

[S50] C++：格式化数字
来源：http://pxn.daria6918.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lwi.fzhhl.top

[S51] C++：显式类型转换
来源：http://oyt.xinyue.icu

static_cast<double>(a) / b
来源：http://gsm.zhengqikj.top

[S52] C++：const 与 noexcept
来源：http://ftq.jiagoushi.top

int size() const noexcept { return n_; }
来源：http://ncg.chenzaomai.com

[S53] C++：移动语义
来源：http://ifm.fengsongda.top

std::vector<int> w = std::move(v);
来源：http://bnj.andypj.xyz

[S54] C++：异常处理
来源：http://wag.zhixingplan.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xlr.haohaochexian.top

[S55] C++：结构化绑定
来源：http://rvc.zhengqikj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://krb.yj20258888.top

[S56] C++：optional
来源：http://lnz.hesvh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ahf.xinyue.icu

[S57] C++：编译期常量
来源：http://gku.chenjidiqi.icu

constexpr int N = 10;
来源：http://xjj.sxryk.cn

[S58] C++：命名空间
来源：http://nib.wangdashe.top

namespace ns { int f() { return 1; } }
来源：http://prg.tian-w.cn

[S59] C++：静态断言
来源：http://whl.zhiwuduotai.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mzh.xylfe.cn

[S60] C++：遍历并删除元素
来源：http://ugi.aibaodan.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ftp.dianchejie.cn

================================================================================
来源：http://wzx.quarkkingdee.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zqp.birdmap.top

================================================================================
来源：http://kki.jlsjyb.cn

[T01] Kotlin：Hello World
来源：http://ury.cashguo.top

println("Hello")
来源：http://yis.fanxiaobao.xyz

[T02] Kotlin：变量
来源：http://rme.cheryme.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://svn.xuetiantiany.cn

[T03] Kotlin：字符串模板
来源：http://qfs.fzhhl.top

"值: $b"
来源：http://gyc.dashuyun.cn

[T04] Kotlin：空安全
来源：http://ifn.xuetiantiany.cn

val n: String? = null;  n?.length
来源：http://iao.ydzc1.top

[T05] Kotlin：when 表达式
来源：http://wtn.guowangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zsz.zdbjq.cn

[T06] Kotlin：集合映射
来源：http://ljh.gogol.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hos.fanxiaobao.xyz

[T07] Kotlin：集合过滤
来源：http://dao.tanke756.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://iya.cashguo.top

[T08] Kotlin：数据类
来源：http://qen.fanxiaobao.xyz

data class User(val name: String, val age: Int)
来源：http://kej.ywan-chungtsiang.top

[T09] Kotlin：扩展函数
来源：http://hkx.wangshuangyany.cn

fun String.exclaim() = this + "!"
来源：http://rjn.jyoumei.cn

[T10] Kotlin：默认参数
来源：http://thg.nanxinkj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://omz.sufxvd.cn

[T11] Kotlin：协程
来源：http://oyf.yuanzhike.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mqv.jlsjyb.cn

[T12] Kotlin：解构声明
来源：http://bqg.zdbjq.cn

val (a, b) = Pair(1, 2)
来源：http://dlf.yonumen.top

[T13] Kotlin：只读 Map
来源：http://mhx.aibaodan.cn

val m = mapOf("a" to 1)
来源：http://ckn.zhengqikj.top

[T14] Kotlin：循环
来源：http://edq.nanxinkj.top

for (i in 1..10) println(i)
来源：http://tqv.ybcxt.top

[T15] Kotlin：接口
来源：http://umk.xziqi.cn

interface Shape { fun area(): Double }
来源：http://gbo.cashguo.top

[T16] Swift：Hello World
来源：http://kjd.shangyingyoupin.top

print("Hello")
来源：http://emt.yj20258888.top

[T17] Swift：变量与常量
来源：http://pzq.xziqi.cn

var a = 1;  let b = 2
来源：http://yxf.yuxming.cn

[T18] Swift：字符串插值
来源：http://aad.cdnleiting.top

"值: \(b)"
来源：http://cod.sysykeji.top

[T19] Swift：可选绑定
来源：http://lwk.fanxiaobao.xyz

if let n = opt { print(n) }
来源：http://yrp.bjfxy.top

[T20] Swift：数组操作
来源：http://nsi.aizwys.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hvz.ydjk.org.cn

[T21] Swift：遍历
来源：http://lsn.c1oappe.top

for x in a { print(x) }
来源：http://fcb.jqgfzy.top

[T22] Swift：字典
来源：http://gsu.yfazqb.com

var d = ["a": 1];  d["b"] = 2
来源：http://wha.mhx1999.top

[T23] Swift：函数
来源：http://awt.tanke756.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tst.shuidangran.top

[T24] Swift：闭包
来源：http://nil.shzxlz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://euo.zycfv.cn

[T25] Swift：结构体
来源：http://rdk.zhiwuduotai.top

struct P { var x: Int }
来源：http://quq.yonumen.top

[T26] Swift：类与重写
来源：http://oxb.aizwys.cn

class A: Base { override func f() {} }
来源：http://erb.snrcjt.cn

[T27] Swift：错误处理
来源：http://kfu.hcnkem.com

do { try f() } catch { print(error) }
来源：http://uwo.pengpengdd.cyou

[T28] Swift：枚举
来源：http://qsi.fehbvm.com

enum Color { case red, green }
来源：http://rka.feifeiyinyue.top

[T29] Swift：guard 提前返回
来源：http://fks.tarul.cn

guard let x = opt else { return }
来源：http://kvn.jlsjyb.cn

[T30] Swift：协议
来源：http://dwc.nwbrower.top

protocol Shape { func area() -> Double }
来源：http://jfc.chenjidiqi.icu

[T31] Lua：Hello World
来源：http://dmo.jiagoushi.top

print("Hello")
来源：http://tae.xuanzx.com

[T32] Lua：局部变量
来源：http://nmi.iojbl.cn

local a = 1
来源：http://lah.fktsv.cn

[T33] Lua：表（数组）
来源：http://cyv.yj202588.top

local t = {1, 2, 3};  t[4] = 4
来源：http://zbt.yuanzhike.top

[T34] Lua：遍历表
来源：http://vas.pycfn.com

for i, v in ipairs(t) do print(i, v) end
来源：http://zfx.bbcook.cn

[T35] Lua：字典表
来源：http://hjp.sjlbkw.cn

local d = { a = 1 };  d.b = 2
来源：http://phz.quarkkingdee.top

[T36] Lua：函数
来源：http://skk.gogol.net.cn

function add(a, b) return a + b end
来源：http://ygi.yonumen.top

[T37] Lua：字符串拼接
来源：http://bji.wangshuangyany.cn

"a" .. "b"
来源：http://jjm.andypj.xyz

[T38] Lua：条件
来源：http://uuq.yfazqb.com

if x > 0 then print("正") end
来源：http://mpk.gogol.net.cn

[T39] Lua：模式匹配
来源：http://nzi.fzhhl.top

string.find(s, "%d+")
来源：http://vwa.sxryk.cn

[T40] Lua：元表
来源：http://yxn.zhaomingkeji.xyz

setmetatable({}, { __index = base })
来源：http://wki.svipenyu.cn

[T41] Perl：Hello World
来源：http://llk.gotoacloud.top

print "Hello\n";
来源：http://yyf.c1oappe.top

[T42] Perl：变量类型
来源：http://kpl.daria6918.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ntw.jinghuilouyu.cn

[T43] Perl：字符串插值
来源：http://eii.ehwqpu.com

"值: $a"
来源：http://pyb.ydzc1.top

[T44] Perl：条件
来源：http://xnr.hnxiangtu.top

if ($a > 0) { print "正"; }
来源：http://sxi.yangfankeji.com

[T45] Perl：数组遍历
来源：http://hvb.nanxuanxn.top

for my $x (@arr) { print $x; }
来源：http://jfq.uphjek.com

[T46] Perl：哈希操作
来源：http://wqf.wangdashe.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jva.sxryk.cn

[T47] Perl：正则捕获
来源：http://wen.fzhhl.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pkc.chenjidiqi.icu

[T48] Perl：正则替换
来源：http://nlg.yuanzhike.top

$s =~ s/old/new/g;
来源：http://ogd.daxiang520.top

[T49] Perl：函数
来源：http://xrk.fehbvm.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vph.ehwqpu.com

[T50] Perl：逐行读文件
来源：http://yqg.snrcjt.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cfg.9152youxi.cn

while (my $line = <$fh>) { print $line; }
来源：http://ypz.fengsongda.top

[T51] Scala：Hello World
来源：http://lgk.c1oappe.top

println("Hello")
来源：http://mnk.zdqjudy.top

[T52] Scala：变量
来源：http://stl.cashguo.top

val a = 1;  var b = 2
来源：http://qfo.dianchejie.cn

[T53] Scala：字符串插值
来源：http://jie.fehbvm.com

s"值: $b"
来源：http://hhb.gogol.net.cn

[T54] Scala：集合映射
来源：http://mkt.nwbrower.top

List(1, 2, 3).map(_ * 2)
来源：http://urz.vehdjk.com

[T55] Scala：集合过滤
来源：http://tik.yongpay.top

List(1, 2, 3).filter(_ > 1)
来源：http://aqj.jqgufenzy.top

[T56] Scala：样例类
来源：http://opy.bbcook.cn

case class User(name: String, age: Int)
来源：http://peo.xuetiantiany.cn

[T57] Scala：模式匹配
来源：http://lse.svipenyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uzi.yj20258888.top

[T58] Scala：函数定义
来源：http://mzd.zycfv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mes.pycfn.com

[T59] Scala：循环
来源：http://eak.jinqigfzy.top

for (i <- 1 to 10) println(i)
来源：http://yfm.xziqi.cn

[T60] Scala：折叠
来源：http://rxx.tian-w.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sjb.hammf.cn

================================================================================
来源：http://hzk.wangshuangyany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zkx.jiagoushi.top

================================================================================
来源：http://jwv.sxryk.cn

[U01] Py：创建虚拟环境
来源：http://xcc.yangfankeji.com

python -m venv .venv && source .venv/bin/activate
来源：http://ega.hywenlv.cn

[U02] Py：导出 / 安装依赖
来源：http://fge.bjfxy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pnt.jiagoushi.top

[U03] Py：加载 .env 配置
来源：http://vix.316326.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://oif.52xcode.cn

[U04] Py：变量调试打印
来源：http://wik.hnqzz.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vmf.gogol.net.cn

[U05] Py：列表去重且保序
来源：http://qyl.wangdashe.top

list(dict.fromkeys(arr))
来源：http://fez.cucudq.cn

[U06] Py：合并两个字典
来源：http://vsz.svipenyu.cn

{**a, **b}
来源：http://geu.shangyingyoupin.top

[U07] Py：反转字典键值
来源：http://bka.tarul.cn

{v: k for k, v in d.items()}
来源：http://jqj.birdmap.top

[U08] Py：展平二维列表
来源：http://iok.shanyushiyangkeji.top

[y for x in nested for y in x]
来源：http://qbw.hysaishi.cn

[U09] Py：字典取最大值的键
来源：http://aid.jiagoushi.top

max(d, key=d.get)
来源：http://kdu.cdnleiting.top

[U10] Py：按值排序字典
来源：http://zdh.hcnkem.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hzi.sxryk.cn

[U11] Py：生成器表达式
来源：http://cgd.zhixingplan.top

(x * 2 for x in arr)
来源：http://hbq.yonumen.top

[U12] Py：取出现最多的 3 个元素
来源：http://izj.pycfn.com

Counter(arr).most_common(3)
来源：http://hlz.jqgfzy.top

[U13] Py：固定长度队列
来源：http://iwi.gogol.net.cn

deque(maxlen=10)
来源：http://rit.meibo888.top

[U14] Py：分组收集到列表
来源：http://thx.fehbvm.com

defaultdict(list)
来源：http://zdp.guannengcc.top

[U15] Py：高精度计时
来源：http://fkx.xziqi.cn

t = time.perf_counter()
来源：http://vsg.sjlbkw.cn

[U16] Py：命令行参数解析
来源：http://cfp.cdnleiting.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gkk.fktsv.cn

[U17] Py：初始化日志
来源：http://lcz.fktsv.cn

logging.basicConfig(level=logging.INFO)
来源：http://egv.vehdjk.com

[U18] Py：预编译正则
来源：http://fiq.hnxiangtu.top

pat = re.compile(r"\d+")
来源：http://eyk.nwbrower.top

[U19] Py：正则替换带回调
来源：http://kqz.xuanzx.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ozk.daria6918.cn

[U20] Py：缓存函数结果
来源：http://ngl.hesvh.cn

@functools.lru_cache(maxsize=None)
来源：http://mep.vqdsnc.cn

[U21] Py：自定义上下文管理器
来源：http://kcs.sweek.top

@contextlib.contextmanager
来源：http://smv.snrcjt.cn

[U22] Py：矩阵转置
来源：http://grl.vehdjk.com

list(zip(*m))
来源：http://eug.xingfuxueyuan.xyz

[U23] Py：分块读取大文件
来源：http://oxj.hfpthk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ooe.cqqwz.cn

[U24] Py：路径操作
来源：http://naw.zhoulong.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tuc.52xcode.cn

[U25] Py：CSV 按字典读
来源：http://ray.ybcxt.top

csv.DictReader(f)
来源：http://dfx.jinyuanbaomall.cn

[U26] Py：并发下载
来源：http://jhe.52xcode.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ykb.wangshuangyany.cn

[U27] Py：异步 HTTP
来源：http://xey.jiagoushi.top

aiohttp.ClientSession() 配合 async with
来源：http://krs.shuidangran.top

[U28] Py：类型别名
来源：http://hbe.jlsjyb.cn

UserId = int
来源：http://zcm.hcnkem.com

[U29] Py：属性校验
来源：http://orp.guowangkeji.top

@property 与 @x.setter 配合
来源：http://mlb.zhixingplan.top

[U30] Py：数据类
来源：http://sip.jinqigfzy.top

@dataclass(slots=True)
来源：http://bcz.shanyushiyangtech.top

[U31] Py：单测
来源：http://zub.yj20258.top

python -m pytest -q
来源：http://xor.yueranfly.top

[U32] Py：代码格式化
来源：http://uws.yj20258888.top

ruff format . && ruff check --fix .
来源：http://uml.daxiang520.top

[U33] Py：打包发布
来源：http://gnn.zhaomingkeji.xyz

python -m build  （依赖 pyproject.toml）
来源：http://hvd.bjfxy.top

[U34] Py：判断编码
来源：http://lze.zhijiandao.cn

chardet.detect(raw)
来源：http://lnd.vqdsnc.cn

[U35] Py：发送邮件
来源：http://uxc.fanxiaobao.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://axa.gotoacloud.top

[U36] Py：定时任务
来源：http://yss.xingfuxueyuan.xyz

schedule.every(10).minutes.do(job)
来源：http://buw.cdnleiting.top

[U37] Py：读写 Excel
来源：http://wgd.feifeiyinyue.top

pandas.read_excel / DataFrame.to_excel
来源：http://btn.pengpengdd.cyou

[U38] Py：获取脚本所在目录
来源：http://ioe.hfpthk.cn

Path(__file__).resolve().parent
来源：http://wwl.hammf.cn

[U39] Py：判断是否在交互环境
来源：http://std.jqgufenzy.top

sys.stdout.isatty()
来源：http://vsc.jinqigfzy.top

[U40] Py：打印到标准错误
来源：http://wzk.fehbvm.com

print("err", file=sys.stderr)
来源：http://skw.zhijiandao.cn

[U41] PHP：初始化 Composer 项目
来源：http://cqj.sweek.top

composer init;  composer require guzzlehttp/guzzle
来源：http://onq.52xcode.cn

[U42] PHP：PSR-4 自动加载
来源：http://egf.wangdashe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rdu.fzhhl.top

[U43] PHP：声明命名空间
来源：http://ony.guowangkeji.top

namespace App\Http;
来源：http://oti.shanyushiyangkeji.top

[U44] PHP：开启严格类型
来源：http://kmr.c1oappe.top

declare(strict_types=1);
来源：http://vvl.zhengqikj.top

[U45] PHP：类型声明与返回类型
来源：http://exj.52xcode.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kod.hnqzz.top

[U46] PHP：可空类型
来源：http://yvf.hysaishi.cn

?string $name = null
来源：http://dwd.fzhhl.top

[U47] PHP：联合类型
来源：http://qeo.gaohongyu789.top

int|string $id
来源：http://vkp.xingfuxueyuan.xyz

[U48] PHP：纯枚举
来源：http://loq.havefunace.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pum.yj20258.top

[U49] PHP：只读属性
来源：http://uwu.redwolf501.top

public readonly string $name
来源：http://bvc.yanxiufei.cn

[U50] PHP：构造器属性提升
来源：http://pvl.gaohongyu789.top

public function __construct(private int $id) {}
来源：http://rzj.yanxiufei.cn

[U51] PHP：数组解构
来源：http://jte.guowangkeji.top

[$a, $b] = $arr;
来源：http://quw.ybcxt.top

[U52] PHP：箭头函数
来源：http://ijm.xinyue.icu

$double = fn($x) => $x * 2;
来源：http://cet.aizwys.cn

[U53] PHP：空合并运算符
来源：http://jrz.shzxlz.cn

$v = $a ?? $b ?? "default";
来源：http://lwu.tianlin.xyz

[U54] PHP：空安全调用
来源：http://uow.xinyue.icu

$obj?->method()
来源：http://dhm.havefunace.top

[U55] PHP：match 表达式
来源：http://jfa.xziqi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tsc.nanxuanxn.top

[U56] PHP：命名参数
来源：http://bdk.jyoumei.cn

f(a: 1, b: 2)
来源：http://tkw.birdmap.top

[U57] PHP：字符串插值
来源：http://wpz.ydzc1.top

"值: {$a}"
来源：http://kbb.yongpay.top

[U58] PHP：数组三件套
来源：http://kgq.ivvv.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://waz.52xcode.cn

[U59] PHP：自定义排序
来源：http://dlg.snrcjt.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://raa.ctjpmb.com

[U60] PHP：JSON 编解码
来源：http://ltw.chenzaomai.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cvx.yonumen.top

[U61] PHP：正则
来源：http://drn.zdbjq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ugm.meibo888.top

[U62] PHP：日期对象
来源：http://uok.yongpay.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ixk.dashuyun.cn

[U63] PHP：文件读写
来源：http://nxh.ppjwa.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wxo.yvedp.cn

[U64] PHP：目录遍历
来源：http://jag.cqqwz.cn

glob("dir/*.php");  scandir("dir");
来源：http://qiz.nwbrower.top

[U65] PHP：会话
来源：http://ayw.daria6918.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mmi.fehbvm.com

[U66] PHP：设置 Cookie
来源：http://kav.jlsjyb.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ltm.chenlongwang.top

[U67] PHP：处理文件上传
来源：http://efn.jlsjyb.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xka.xylfe.cn

[U68] PHP：PDO 连接
来源：http://tqr.yj20258888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ihk.uphjek.com

[U69] PHP：PDO 预处理
来源：http://pmn.jinqigfzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cxn.birdmap.top

[U70] PHP：PDO 事务
来源：http://hmj.hywenlv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uti.0kj1m.cn


<!-- 参考信息 -->