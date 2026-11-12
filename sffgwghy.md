代发 wailian999

[S45] C++：lambda
来源：http://ksd.hcnkem.com

auto add = [](int a, int b) { return a + b; };
来源：http://vup.52xcode.cn

[S46] C++：函数模板
来源：http://obg.ydzc1.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wit.hywenlv.cn

[S47] C++：结构化绑定遍历
来源：http://not.shuidangran.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ypo.fehbvm.com

[S48] C++：逐行读文件
来源：http://oyx.aizwys.cn

std::ifstream in("a.txt");  std::string line;
来源：http://daw.bbcook.cn

while (std::getline(in, line)) { }
来源：http://mxx.jiagoushi.top

[S49] C++：写文件
来源：http://haa.tian-w.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kdb.xziqi.cn

[S50] C++：格式化数字
来源：http://oai.fzhhl.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rwj.316326.xyz

[S51] C++：显式类型转换
来源：http://qnf.xylfe.cn

static_cast<double>(a) / b
来源：http://fvl.cdnleiting.top

[S52] C++：const 与 noexcept
来源：http://ejw.c1oappe.top

int size() const noexcept { return n_; }
来源：http://koc.yangfankeji.com

[S53] C++：移动语义
来源：http://ljx.pycfn.com

std::vector<int> w = std::move(v);
来源：http://ler.jinghuilouyu.cn

[S54] C++：异常处理
来源：http://zun.gaohongyu789.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dgl.daria6918.cn

[S55] C++：结构化绑定
来源：http://ltg.sxryk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ple.shuidangran.top

[S56] C++：optional
来源：http://cus.hammf.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rrh.vehdjk.com

[S57] C++：编译期常量
来源：http://ijy.shanyushiyangtech.top

constexpr int N = 10;
来源：http://tuh.zhijiandao.cn

[S58] C++：命名空间
来源：http://oxg.vqdsnc.cn

namespace ns { int f() { return 1; } }
来源：http://wdn.chenzaomai.com

[S59] C++：静态断言
来源：http://kfp.tanke756.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uzo.cdnleiting.top

[S60] C++：遍历并删除元素
来源：http://hms.yonumen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yiu.zhiwuduotai.top

================================================================================
来源：http://qlf.vehdjk.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rqe.hongshengwenyu.top

================================================================================
来源：http://iiz.hesvh.cn

[T01] Kotlin：Hello World
来源：http://vcj.jlsjyb.cn

println("Hello")
来源：http://vyj.52xcode.cn

[T02] Kotlin：变量
来源：http://chm.shuidangran.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://crh.quarkkingdee.top

[T03] Kotlin：字符串模板
来源：http://loi.hnxiangtu.top

"值: $b"
来源：http://mpi.tarul.cn

[T04] Kotlin：空安全
来源：http://gca.andypj.xyz

val n: String? = null;  n?.length
来源：http://otx.316326.xyz

[T05] Kotlin：when 表达式
来源：http://wnt.jianghu66.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lad.hnqzz.top

[T06] Kotlin：集合映射
来源：http://tzb.sysykeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://yvn.wangshuangyany.cn

[T07] Kotlin：集合过滤
来源：http://mnj.fktsv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lsv.ivvv.top

[T08] Kotlin：数据类
来源：http://cla.hesvh.cn

data class User(val name: String, val age: Int)
来源：http://liw.ydjk.org.cn

[T09] Kotlin：扩展函数
来源：http://lex.cdnleiting.top

fun String.exclaim() = this + "!"
来源：http://ydl.tianlin.xyz

[T10] Kotlin：默认参数
来源：http://vhc.zhiwuduotai.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hjy.andypj.xyz

[T11] Kotlin：协程
来源：http://fsl.shangyingyoupin.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://yjy.svipenyu.cn

[T12] Kotlin：解构声明
来源：http://abt.guannengcc.top

val (a, b) = Pair(1, 2)
来源：http://ejg.hammf.cn

[T13] Kotlin：只读 Map
来源：http://xmb.vqdsnc.cn

val m = mapOf("a" to 1)
来源：http://nya.hfpthk.cn

[T14] Kotlin：循环
来源：http://gtx.guannengcc.top

for (i in 1..10) println(i)
来源：http://mrh.cashguo.top

[T15] Kotlin：接口
来源：http://whd.yanxiufei.cn

interface Shape { fun area(): Double }
来源：http://xlr.cheryme.top

[T16] Swift：Hello World
来源：http://iek.xingfuxueyuan.xyz

print("Hello")
来源：http://fxo.gaohongyu789.top

[T17] Swift：变量与常量
来源：http://vox.gotoacloud.top

var a = 1;  let b = 2
来源：http://zol.nwbrower.top

[T18] Swift：字符串插值
来源：http://uja.zhiwuduotai.top

"值: \(b)"
来源：http://tqo.zhaomingkeji.xyz

[T19] Swift：可选绑定
来源：http://sux.jiagoushi.top

if let n = opt { print(n) }
来源：http://jes.zhixingplan.top

[T20] Swift：数组操作
来源：http://mwv.yongpay.top

var a = [1, 2, 3];  a.append(4)
来源：http://ber.cqqwz.cn

[T21] Swift：遍历
来源：http://pmw.9152youxi.cn

for x in a { print(x) }
来源：http://eea.aibaodan.cn

[T22] Swift：字典
来源：http://dfp.ppjwa.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sjm.ivvv.top

[T23] Swift：函数
来源：http://kqw.pengpengdd.cyou

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lnp.yonumen.top

[T24] Swift：闭包
来源：http://gsy.kuanghao11.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tjm.svipenyu.cn

[T25] Swift：结构体
来源：http://elc.epnwcf.com

struct P { var x: Int }
来源：http://vcb.gogol.net.cn

[T26] Swift：类与重写
来源：http://gfd.zhengqikj.top

class A: Base { override func f() {} }
来源：http://srs.snrcjt.cn

[T27] Swift：错误处理
来源：http://idu.chenjidiqi.icu

do { try f() } catch { print(error) }
来源：http://lcl.svipenyu.cn

[T28] Swift：枚举
来源：http://tlq.xylfe.cn

enum Color { case red, green }
来源：http://bpr.gotoacloud.top

[T29] Swift：guard 提前返回
来源：http://fjo.xziqi.cn

guard let x = opt else { return }
来源：http://ikz.tarul.cn

[T30] Swift：协议
来源：http://xfw.jqgufenzy.top

protocol Shape { func area() -> Double }
来源：http://abk.dashuyun.cn

[T31] Lua：Hello World
来源：http://jqq.zhiwuduotai.top

print("Hello")
来源：http://myn.bbcook.cn

[T32] Lua：局部变量
来源：http://ryi.xuetiantiany.cn

local a = 1
来源：http://tiw.gaohongyu789.top

[T33] Lua：表（数组）
来源：http://lkw.hesvh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rxo.uphjek.com

[T34] Lua：遍历表
来源：http://nsa.vehdjk.com

for i, v in ipairs(t) do print(i, v) end
来源：http://pvf.fengsongda.top

[T35] Lua：字典表
来源：http://lrb.haohaochexian.top

local d = { a = 1 };  d.b = 2
来源：http://onz.chenlongwang.top

[T36] Lua：函数
来源：http://vmz.316326.xyz

function add(a, b) return a + b end
来源：http://kco.chenlongwang.top

[T37] Lua：字符串拼接
来源：http://ujy.sysykeji.top

"a" .. "b"
来源：http://jad.vehdjk.com

[T38] Lua：条件
来源：http://mbb.zhengqikj.top

if x > 0 then print("正") end
来源：http://olf.aizwys.cn

[T39] Lua：模式匹配
来源：http://ehu.gaohongyu789.top

string.find(s, "%d+")
来源：http://jjm.hcnkem.com

[T40] Lua：元表
来源：http://nln.quarkkingdee.top

setmetatable({}, { __index = base })
来源：http://gqc.zhongyouzk.top

[T41] Perl：Hello World
来源：http://dzl.yangfankeji.com

print "Hello\n";
来源：http://hks.jinghuilouyu.cn

[T42] Perl：变量类型
来源：http://bnd.aibaodan.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xvo.xuetiantiany.cn

[T43] Perl：字符串插值
来源：http://kdr.wangshuangyany.cn

"值: $a"
来源：http://rfw.hnxiangtu.top

[T44] Perl：条件
来源：http://cgg.tianlin.xyz

if ($a > 0) { print "正"; }
来源：http://suz.redwolf501.top

[T45] Perl：数组遍历
来源：http://eyg.yvedp.cn

for my $x (@arr) { print $x; }
来源：http://oxn.cashguo.top

[T46] Perl：哈希操作
来源：http://dlt.jianghu66.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://iqb.jyoumei.cn

[T47] Perl：正则捕获
来源：http://gfj.jqgufenzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vwp.zycfv.cn

[T48] Perl：正则替换
来源：http://xer.nanxinkj.top

$s =~ s/old/new/g;
来源：http://dzo.cdnleiting.top

[T49] Perl：函数
来源：http://alv.hysaishi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vyb.hammf.cn

[T50] Perl：逐行读文件
来源：http://rvx.0kj1m.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://obz.svipenyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://plq.daxiang520.top

[T51] Scala：Hello World
来源：http://hky.sjlbkw.cn

println("Hello")
来源：http://jbl.gogol.net.cn

[T52] Scala：变量
来源：http://cje.bbcook.cn

val a = 1;  var b = 2
来源：http://rfx.shuidangran.top

[T53] Scala：字符串插值
来源：http://fds.jinghuilouyu.cn

s"值: $b"
来源：http://axp.nanxuanxn.top

[T54] Scala：集合映射
来源：http://wpw.cqqwz.cn

List(1, 2, 3).map(_ * 2)
来源：http://vga.hfpthk.cn

[T55] Scala：集合过滤
来源：http://kzt.fktsv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zsz.hfpthk.cn

[T56] Scala：样例类
来源：http://uea.ppjwa.cn

case class User(name: String, age: Int)
来源：http://zvw.hfpthk.cn

[T57] Scala：模式匹配
来源：http://gnm.fzhhl.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://pao.hywenlv.cn

[T58] Scala：函数定义
来源：http://ith.birdmap.top

def add(a: Int, b: Int): Int = a + b
来源：http://pgp.yfazqb.com

[T59] Scala：循环
来源：http://yns.yuxming.cn

for (i <- 1 to 10) println(i)
来源：http://sel.zycfv.cn

[T60] Scala：折叠
来源：http://ggn.aibaodan.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tfr.hywenlv.cn

================================================================================
来源：http://jbn.zdqjudy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yoj.fehbvm.com

================================================================================
来源：http://elv.ivvv.top

[U01] Py：创建虚拟环境
来源：http://qma.dianchejie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gss.yongpay.top

[U02] Py：导出 / 安装依赖
来源：http://lop.pengpengdd.cyou

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yll.hammf.cn

[U03] Py：加载 .env 配置
来源：http://glc.wangshuangyany.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rxw.birdmap.top

[U04] Py：变量调试打印
来源：http://tqo.52xcode.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rud.yj20258.top

[U05] Py：列表去重且保序
来源：http://cbs.gzhubu.top

list(dict.fromkeys(arr))
来源：http://qub.ivvv.top

[U06] Py：合并两个字典
来源：http://npt.ivvv.top

{**a, **b}
来源：http://jru.jinyuanbaomall.cn

[U07] Py：反转字典键值
来源：http://zvb.c1oappe.top

{v: k for k, v in d.items()}
来源：http://bbt.yfazqb.com

[U08] Py：展平二维列表
来源：http://cyd.quarkkingdee.top

[y for x in nested for y in x]
来源：http://eve.snrcjt.cn

[U09] Py：字典取最大值的键
来源：http://sjn.meibo888.top

max(d, key=d.get)
来源：http://aji.yvedp.cn

[U10] Py：按值排序字典
来源：http://xof.gogol.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://euf.ctjpmb.com

[U11] Py：生成器表达式
来源：http://qpq.xingfuxueyuan.xyz

(x * 2 for x in arr)
来源：http://wif.tanke756.top

[U12] Py：取出现最多的 3 个元素
来源：http://lfr.sufxvd.cn

Counter(arr).most_common(3)
来源：http://wrh.snrcjt.cn

[U13] Py：固定长度队列
来源：http://hmw.quarkkingdee.top

deque(maxlen=10)
来源：http://qnp.ydjk.org.cn

[U14] Py：分组收集到列表
来源：http://imf.zhixingplan.top

defaultdict(list)
来源：http://zhk.zycfv.cn

[U15] Py：高精度计时
来源：http://lfe.daxiang520.top

t = time.perf_counter()
来源：http://ido.shuidangran.top

[U16] Py：命令行参数解析
来源：http://vpg.yj20258888.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hcr.hongshengwenyu.top

[U17] Py：初始化日志
来源：http://drg.gogol.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://zsx.yangfankeji.com

[U18] Py：预编译正则
来源：http://vip.nwbrower.top

pat = re.compile(r"\d+")
来源：http://pty.aibaodan.cn

[U19] Py：正则替换带回调
来源：http://thn.wangshuangyany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bbl.cashguo.top

[U20] Py：缓存函数结果
来源：http://mes.meibo888.top

@functools.lru_cache(maxsize=None)
来源：http://jve.daxiang520.top

[U21] Py：自定义上下文管理器
来源：http://kld.hesvh.cn

@contextlib.contextmanager
来源：http://kkn.zhijiandao.cn

[U22] Py：矩阵转置
来源：http://jvr.ybcxt.top

list(zip(*m))
来源：http://xlt.zhiwuduotai.top

[U23] Py：分块读取大文件
来源：http://rsg.ydzc1.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ybm.jinqigufen.top

[U24] Py：路径操作
来源：http://imc.yuxming.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vlx.hysaishi.cn

[U25] Py：CSV 按字典读
来源：http://lit.zdbjq.cn

csv.DictReader(f)
来源：http://syj.jiagoushi.top

[U26] Py：并发下载
来源：http://nhf.jinqigfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://igv.xylfe.cn

[U27] Py：异步 HTTP
来源：http://xjy.redwolf501.top

aiohttp.ClientSession() 配合 async with
来源：http://ywx.shanyushiyangtech.top

[U28] Py：类型别名
来源：http://pzn.yj20258.top

UserId = int
来源：http://pes.zdbjq.cn

[U29] Py：属性校验
来源：http://jav.ywan-chungtsiang.top

@property 与 @x.setter 配合
来源：http://rfp.xinyue.icu

[U30] Py：数据类
来源：http://epf.sufxvd.cn

@dataclass(slots=True)
来源：http://tvx.zhengqikj.top

[U31] Py：单测
来源：http://bvp.fanxiaobao.xyz

python -m pytest -q
来源：http://nhk.zhongyouzk.top

[U32] Py：代码格式化
来源：http://nmo.tian-w.cn

ruff format . && ruff check --fix .
来源：http://dww.yongpay.top

[U33] Py：打包发布
来源：http://xce.guowangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://ytg.jinqigufen.top

[U34] Py：判断编码
来源：http://zyh.wangdashe.top

chardet.detect(raw)
来源：http://inj.hammf.cn

[U35] Py：发送邮件
来源：http://oym.sysykeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eij.fehbvm.com

[U36] Py：定时任务
来源：http://def.daxiang520.top

schedule.every(10).minutes.do(job)
来源：http://mix.chenzaomai.com

[U37] Py：读写 Excel
来源：http://mgf.yfazqb.com

pandas.read_excel / DataFrame.to_excel
来源：http://abm.zhaomingkeji.xyz

[U38] Py：获取脚本所在目录
来源：http://ynx.cheryme.top

Path(__file__).resolve().parent
来源：http://tcr.hcnkem.com

[U39] Py：判断是否在交互环境
来源：http://wcn.xuanzx.com

sys.stdout.isatty()
来源：http://roa.zdbjq.cn

[U40] Py：打印到标准错误
来源：http://lwu.shanyushiyangkeji.top

print("err", file=sys.stderr)
来源：http://jck.sjlbkw.cn

[U41] PHP：初始化 Composer 项目
来源：http://ogr.aizwys.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://iie.hywenlv.cn

[U42] PHP：PSR-4 自动加载
来源：http://gnx.bjfxy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://oae.havefunace.top

[U43] PHP：声明命名空间
来源：http://exz.cqqwz.cn

namespace App\Http;
来源：http://uuv.sjlbkw.cn

[U44] PHP：开启严格类型
来源：http://sli.chenlongwang.top

declare(strict_types=1);
来源：http://wff.hysaishi.cn

[U45] PHP：类型声明与返回类型
来源：http://oda.hnqzz.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hny.316326.xyz

[U46] PHP：可空类型
来源：http://wde.jianghu66.top

?string $name = null
来源：http://oeu.shzxlz.cn

[U47] PHP：联合类型
来源：http://xyl.ctjpmb.com

int|string $id
来源：http://shq.chenlongwang.top

[U48] PHP：纯枚举
来源：http://yos.shzxlz.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ygi.vqdsnc.cn

[U49] PHP：只读属性
来源：http://igu.aibaodan.cn

public readonly string $name
来源：http://laj.wangdashe.top

[U50] PHP：构造器属性提升
来源：http://fdb.ehwqpu.com

public function __construct(private int $id) {}
来源：http://msn.hywenlv.cn

[U51] PHP：数组解构
来源：http://qvi.dashuyun.cn

[$a, $b] = $arr;
来源：http://eiq.9152youxi.cn

[U52] PHP：箭头函数
来源：http://poy.smart0.xyz

$double = fn($x) => $x * 2;
来源：http://bke.fktsv.cn

[U53] PHP：空合并运算符
来源：http://sib.9152youxi.cn

$v = $a ?? $b ?? "default";
来源：http://qdi.bbcook.cn

[U54] PHP：空安全调用
来源：http://ucl.gotoacloud.top

$obj?->method()
来源：http://ctd.tarul.cn

[U55] PHP：match 表达式
来源：http://azv.fzhhl.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qtn.hywenlv.cn

[U56] PHP：命名参数
来源：http://eap.tanke756.top

f(a: 1, b: 2)
来源：http://cdq.feifeiyinyue.top

[U57] PHP：字符串插值
来源：http://pjm.redwolf501.top

"值: {$a}"
来源：http://cpa.shanyushiyangtech.top

[U58] PHP：数组三件套
来源：http://rxu.dianchejie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rxr.cqqwz.cn

[U59] PHP：自定义排序
来源：http://dgl.fengsongda.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ohw.zhijiandao.cn

[U60] PHP：JSON 编解码
来源：http://ngy.redwolf501.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gsk.hongshengwenyu.top

[U61] PHP：正则
来源：http://noq.hesvh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eva.yuanzhike.top

[U62] PHP：日期对象
来源：http://yoj.jinghuilouyu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://iei.hongshengwenyu.top

[U63] PHP：文件读写
来源：http://sbd.hywenlv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qyz.c1oappe.top

[U64] PHP：目录遍历
来源：http://oee.hywenlv.cn

glob("dir/*.php");  scandir("dir");
来源：http://vna.hfpthk.cn

[U65] PHP：会话
来源：http://iig.zdbjq.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://uin.yangfankeji.com

[U66] PHP：设置 Cookie
来源：http://ekh.ehwqpu.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dcw.shuidangran.top

[U67] PHP：处理文件上传
来源：http://ooa.ywan-chungtsiang.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cws.zhaomingkeji.xyz

[U68] PHP：PDO 连接
来源：http://ktf.snrcjt.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uzl.bbcook.cn

[U69] PHP：PDO 预处理
来源：http://hlv.xinyue.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zcy.smart0.xyz

[U70] PHP：PDO 事务
来源：http://zwx.wangdashe.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nhv.52xcode.cn


<!-- 参考信息 -->