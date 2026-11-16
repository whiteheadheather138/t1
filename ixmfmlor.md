代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://fbt.ppjwa.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hvk.ywan-chungtsiang.top

[S48] C++：逐行读文件
来源：http://qbe.hfpthk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dnp.jinqigfzy.top

while (std::getline(in, line)) { }
来源：http://dnn.ywan-chungtsiang.top

[S49] C++：写文件
来源：http://qir.jiagoushi.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tqt.cqqwz.cn

[S50] C++：格式化数字
来源：http://xkf.chenlongwang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jaq.snrcjt.cn

[S51] C++：显式类型转换
来源：http://zoq.sufxvd.cn

static_cast<double>(a) / b
来源：http://mha.guannengcc.top

[S52] C++：const 与 noexcept
来源：http://imp.zhengqikj.top

int size() const noexcept { return n_; }
来源：http://bfv.xinyue.icu

[S53] C++：移动语义
来源：http://ggh.316326.xyz

std::vector<int> w = std::move(v);
来源：http://pmk.havefunace.top

[S54] C++：异常处理
来源：http://sgd.aizwys.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hdw.yangfankeji.com

[S55] C++：结构化绑定
来源：http://gpr.fzhhl.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rij.jlsjyb.cn

[S56] C++：optional
来源：http://jgc.ivvv.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kap.epnwcf.com

[S57] C++：编译期常量
来源：http://nnd.jinyuanbaomall.cn

constexpr int N = 10;
来源：http://vsc.zycfv.cn

[S58] C++：命名空间
来源：http://atp.redwolf501.top

namespace ns { int f() { return 1; } }
来源：http://nvr.snrcjt.cn

[S59] C++：静态断言
来源：http://joe.ydzc1.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://thk.hywenlv.cn

[S60] C++：遍历并删除元素
来源：http://xvo.haohaochexian.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uzc.shuidangran.top

================================================================================
来源：http://ehx.shanyushiyangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vnj.zdqjudy.top

================================================================================
来源：http://ufk.jyoumei.cn

[T01] Kotlin：Hello World
来源：http://oje.xinyue.icu

println("Hello")
来源：http://zpl.tanke756.top

[T02] Kotlin：变量
来源：http://ddd.redwolf501.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yqu.yongpay.top

[T03] Kotlin：字符串模板
来源：http://elf.yj20258888.top

"值: $b"
来源：http://iwc.zhongyouzk.top

[T04] Kotlin：空安全
来源：http://det.tianlin.xyz

val n: String? = null;  n?.length
来源：http://edf.yuxming.cn

[T05] Kotlin：when 表达式
来源：http://hwq.cdnleiting.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://egz.snrcjt.cn

[T06] Kotlin：集合映射
来源：http://yks.zdbjq.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kjl.vqdsnc.cn

[T07] Kotlin：集合过滤
来源：http://bvn.tanke756.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tnl.yueranfly.top

[T08] Kotlin：数据类
来源：http://iby.fengsongda.top

data class User(val name: String, val age: Int)
来源：http://cjj.zhixingplan.top

[T09] Kotlin：扩展函数
来源：http://hyx.sufxvd.cn

fun String.exclaim() = this + "!"
来源：http://cfi.havefunace.top

[T10] Kotlin：默认参数
来源：http://yyh.sweek.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ifc.cqqwz.cn

[T11] Kotlin：协程
来源：http://oyp.sufxvd.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mzp.haohaochexian.top

[T12] Kotlin：解构声明
来源：http://vwd.yvedp.cn

val (a, b) = Pair(1, 2)
来源：http://ncz.sxryk.cn

[T13] Kotlin：只读 Map
来源：http://pyc.fengsongda.top

val m = mapOf("a" to 1)
来源：http://cue.jinghuilouyu.cn

[T14] Kotlin：循环
来源：http://rhm.yuxming.cn

for (i in 1..10) println(i)
来源：http://ajh.ydzc1.top

[T15] Kotlin：接口
来源：http://mac.yuxming.cn

interface Shape { fun area(): Double }
来源：http://qko.ivvv.top

[T16] Swift：Hello World
来源：http://aqh.zycfv.cn

print("Hello")
来源：http://xyf.tanke756.top

[T17] Swift：变量与常量
来源：http://ssf.jinyuanbaomall.cn

var a = 1;  let b = 2
来源：http://vsw.daria6918.cn

[T18] Swift：字符串插值
来源：http://ont.wangdashe.top

"值: \(b)"
来源：http://jvx.hywenlv.cn

[T19] Swift：可选绑定
来源：http://rhr.sjlbkw.cn

if let n = opt { print(n) }
来源：http://ecs.chenjidiqi.icu

[T20] Swift：数组操作
来源：http://wll.zhijiandao.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jpy.jinqigufen.top

[T21] Swift：遍历
来源：http://kwl.hfpthk.cn

for x in a { print(x) }
来源：http://zvj.jianghu66.top

[T22] Swift：字典
来源：http://afu.zhoulong.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://wnk.sysykeji.top

[T23] Swift：函数
来源：http://oft.chenjidiqi.icu

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gip.hesvh.cn

[T24] Swift：闭包
来源：http://frv.xylfe.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://woh.xylfe.cn

[T25] Swift：结构体
来源：http://iha.cdnleiting.top

struct P { var x: Int }
来源：http://uzi.xuanzx.com

[T26] Swift：类与重写
来源：http://jev.snrcjt.cn

class A: Base { override func f() {} }
来源：http://mov.jyoumei.cn

[T27] Swift：错误处理
来源：http://rbh.feifeiyinyue.top

do { try f() } catch { print(error) }
来源：http://trp.chenzaomai.com

[T28] Swift：枚举
来源：http://zkv.meibo888.top

enum Color { case red, green }
来源：http://gyv.9152youxi.cn

[T29] Swift：guard 提前返回
来源：http://wma.yuxming.cn

guard let x = opt else { return }
来源：http://pco.chenzaomai.com

[T30] Swift：协议
来源：http://jqd.cashguo.top

protocol Shape { func area() -> Double }
来源：http://hga.cucudq.cn

[T31] Lua：Hello World
来源：http://xgu.ctjpmb.com

print("Hello")
来源：http://hyy.ywan-chungtsiang.top

[T32] Lua：局部变量
来源：http://zhc.yvedp.cn

local a = 1
来源：http://fkd.guannengcc.top

[T33] Lua：表（数组）
来源：http://wec.guowangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://phw.gotoacloud.top

[T34] Lua：遍历表
来源：http://gkj.hnxiangtu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://okw.gzhubu.top

[T35] Lua：字典表
来源：http://lkf.bbcook.cn

local d = { a = 1 };  d.b = 2
来源：http://fpc.yj20258888.top

[T36] Lua：函数
来源：http://qnr.xuetiantiany.cn

function add(a, b) return a + b end
来源：http://ane.nanxinkj.top

[T37] Lua：字符串拼接
来源：http://iyw.hesvh.cn

"a" .. "b"
来源：http://xuz.zdqjudy.top

[T38] Lua：条件
来源：http://aen.sxryk.cn

if x > 0 then print("正") end
来源：http://xcb.fanxiaobao.xyz

[T39] Lua：模式匹配
来源：http://gpf.cqqwz.cn

string.find(s, "%d+")
来源：http://lsj.pycfn.com

[T40] Lua：元表
来源：http://xsx.svipenyu.cn

setmetatable({}, { __index = base })
来源：http://hhf.zhijiandao.cn

[T41] Perl：Hello World
来源：http://qxr.zhaomingkeji.xyz

print "Hello\n";
来源：http://qjt.nanxinkj.top

[T42] Perl：变量类型
来源：http://rvb.vehdjk.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mtt.tianlin.xyz

[T43] Perl：字符串插值
来源：http://mqj.sufxvd.cn

"值: $a"
来源：http://yoa.fengsongda.top

[T44] Perl：条件
来源：http://syw.zhaomingkeji.xyz

if ($a > 0) { print "正"; }
来源：http://nev.feifeiyinyue.top

[T45] Perl：数组遍历
来源：http://sje.fzhhl.top

for my $x (@arr) { print $x; }
来源：http://uwq.pycfn.com

[T46] Perl：哈希操作
来源：http://pjy.cdnleiting.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://btq.yongpay.top

[T47] Perl：正则捕获
来源：http://wke.pengpengdd.cyou

if ($s =~ /(\d+)/) { print $1; }
来源：http://txs.gaohongyu789.top

[T48] Perl：正则替换
来源：http://nnc.c1oappe.top

$s =~ s/old/new/g;
来源：http://bpu.jianghu66.top

[T49] Perl：函数
来源：http://nww.guannengcc.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://agn.shzxlz.cn

[T50] Perl：逐行读文件
来源：http://avj.ppjwa.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xnd.yangfankeji.com

while (my $line = <$fh>) { print $line; }
来源：http://urn.jyoumei.cn

[T51] Scala：Hello World
来源：http://flk.yuanzhike.top

println("Hello")
来源：http://guk.nanxinkj.top

[T52] Scala：变量
来源：http://tbv.gotoacloud.top

val a = 1;  var b = 2
来源：http://ksw.uphjek.com

[T53] Scala：字符串插值
来源：http://eud.mhx1999.top

s"值: $b"
来源：http://ruw.52xcode.cn

[T54] Scala：集合映射
来源：http://ley.jyoumei.cn

List(1, 2, 3).map(_ * 2)
来源：http://mnv.316326.xyz

[T55] Scala：集合过滤
来源：http://pgl.smart0.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://sjg.xinyue.icu

[T56] Scala：样例类
来源：http://kon.bjfxy.top

case class User(name: String, age: Int)
来源：http://bma.fzhhl.top

[T57] Scala：模式匹配
来源：http://fce.jlsjyb.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kga.fktsv.cn

[T58] Scala：函数定义
来源：http://sdw.yj20258888.top

def add(a: Int, b: Int): Int = a + b
来源：http://ear.yj20258.top

[T59] Scala：循环
来源：http://eta.xziqi.cn

for (i <- 1 to 10) println(i)
来源：http://vyt.sxryk.cn

[T60] Scala：折叠
来源：http://qls.feifeiyinyue.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bjb.zhaomingkeji.xyz

================================================================================
来源：http://ymg.wangdashe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cko.aizwys.cn

================================================================================
来源：http://rnk.zhixingplan.top

[U01] Py：创建虚拟环境
来源：http://anm.aizwys.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jxb.shanyushiyangtech.top

[U02] Py：导出 / 安装依赖
来源：http://pyp.fktsv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cww.xuanzx.com

[U03] Py：加载 .env 配置
来源：http://zrl.epnwcf.com

from dotenv import load_dotenv; load_dotenv()
来源：http://rgj.sjlbkw.cn

[U04] Py：变量调试打印
来源：http://mxe.pycfn.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://svp.xziqi.cn

[U05] Py：列表去重且保序
来源：http://rbz.gaohongyu789.top

list(dict.fromkeys(arr))
来源：http://yto.zhijiandao.cn

[U06] Py：合并两个字典
来源：http://juw.jqgfzy.top

{**a, **b}
来源：http://rea.ivvv.top

[U07] Py：反转字典键值
来源：http://kzj.zycfv.cn

{v: k for k, v in d.items()}
来源：http://cff.hywenlv.cn

[U08] Py：展平二维列表
来源：http://zsc.svipenyu.cn

[y for x in nested for y in x]
来源：http://inp.fktsv.cn

[U09] Py：字典取最大值的键
来源：http://ksd.c1oappe.top

max(d, key=d.get)
来源：http://kgi.zhijiandao.cn

[U10] Py：按值排序字典
来源：http://vll.fehbvm.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hht.hnxiangtu.top

[U11] Py：生成器表达式
来源：http://lmf.aibaodan.cn

(x * 2 for x in arr)
来源：http://rsf.shuidangran.top

[U12] Py：取出现最多的 3 个元素
来源：http://ptm.ywan-chungtsiang.top

Counter(arr).most_common(3)
来源：http://tge.andypj.xyz

[U13] Py：固定长度队列
来源：http://ziq.pengpengdd.cyou

deque(maxlen=10)
来源：http://ajq.guowangkeji.top

[U14] Py：分组收集到列表
来源：http://cjn.pycfn.com

defaultdict(list)
来源：http://yxv.zhijiandao.cn

[U15] Py：高精度计时
来源：http://bxx.ppjwa.cn

t = time.perf_counter()
来源：http://uex.epnwcf.com

[U16] Py：命令行参数解析
来源：http://lxg.iojbl.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wwr.ybcxt.top

[U17] Py：初始化日志
来源：http://eui.fzhhl.top

logging.basicConfig(level=logging.INFO)
来源：http://cuu.zhaomingkeji.xyz

[U18] Py：预编译正则
来源：http://cjx.zhengqikj.top

pat = re.compile(r"\d+")
来源：http://han.zhongyouzk.top

[U19] Py：正则替换带回调
来源：http://cnu.haohaochexian.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://whh.yj202588.top

[U20] Py：缓存函数结果
来源：http://oll.quarkkingdee.top

@functools.lru_cache(maxsize=None)
来源：http://ivn.wangshuangyany.cn

[U21] Py：自定义上下文管理器
来源：http://yme.zhongyouzk.top

@contextlib.contextmanager
来源：http://gyn.jiagoushi.top

[U22] Py：矩阵转置
来源：http://cmu.svipenyu.cn

list(zip(*m))
来源：http://abg.yj202588.top

[U23] Py：分块读取大文件
来源：http://dlx.yonumen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xjd.jyoumei.cn

[U24] Py：路径操作
来源：http://aud.zhixingplan.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://abv.tianlin.xyz

[U25] Py：CSV 按字典读
来源：http://rsa.fengsongda.top

csv.DictReader(f)
来源：http://rbe.jyoumei.cn

[U26] Py：并发下载
来源：http://udh.gzhubu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nde.svipenyu.cn

[U27] Py：异步 HTTP
来源：http://nir.guannengcc.top

aiohttp.ClientSession() 配合 async with
来源：http://fbo.ctjpmb.com

[U28] Py：类型别名
来源：http://aoz.tianlin.xyz

UserId = int
来源：http://xdq.yuanzhike.top

[U29] Py：属性校验
来源：http://mte.jinqigufen.top

@property 与 @x.setter 配合
来源：http://tmv.zhaomingkeji.xyz

[U30] Py：数据类
来源：http://xdl.jqgufenzy.top

@dataclass(slots=True)
来源：http://cpw.fehbvm.com

[U31] Py：单测
来源：http://vba.gaohongyu789.top

python -m pytest -q
来源：http://hfq.nanxuanxn.top

[U32] Py：代码格式化
来源：http://ubi.yongpay.top

ruff format . && ruff check --fix .
来源：http://jcp.tian-w.cn

[U33] Py：打包发布
来源：http://toz.ydzc1.top

python -m build  （依赖 pyproject.toml）
来源：http://nfc.hfpthk.cn

[U34] Py：判断编码
来源：http://czt.jiagoushi.top

chardet.detect(raw)
来源：http://zft.bbcook.cn

[U35] Py：发送邮件
来源：http://etp.mhx1999.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zvr.daria6918.cn

[U36] Py：定时任务
来源：http://cok.jinqigufen.top

schedule.every(10).minutes.do(job)
来源：http://chj.jinyuanbaomall.cn

[U37] Py：读写 Excel
来源：http://yms.yonumen.top

pandas.read_excel / DataFrame.to_excel
来源：http://ddx.sxryk.cn

[U38] Py：获取脚本所在目录
来源：http://guv.wangdashe.top

Path(__file__).resolve().parent
来源：http://aen.aizwys.cn

[U39] Py：判断是否在交互环境
来源：http://nis.havefunace.top

sys.stdout.isatty()
来源：http://zik.shuidangran.top

[U40] Py：打印到标准错误
来源：http://web.iojbl.cn

print("err", file=sys.stderr)
来源：http://pyt.fktsv.cn

[U41] PHP：初始化 Composer 项目
来源：http://vpl.shuidangran.top

composer init;  composer require guzzlehttp/guzzle
来源：http://dzx.jqgufenzy.top

[U42] PHP：PSR-4 自动加载
来源：http://omc.hesvh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ksh.xingfuxueyuan.xyz

[U43] PHP：声明命名空间
来源：http://mzf.hnqzz.top

namespace App\Http;
来源：http://qgq.c1oappe.top

[U44] PHP：开启严格类型
来源：http://eaf.sufxvd.cn

declare(strict_types=1);
来源：http://wde.yuxming.cn

[U45] PHP：类型声明与返回类型
来源：http://jtz.yonumen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ttb.wangdashe.top

[U46] PHP：可空类型
来源：http://pxs.jinqigufen.top

?string $name = null
来源：http://maz.tianlin.xyz

[U47] PHP：联合类型
来源：http://wen.nanxinkj.top

int|string $id
来源：http://cej.dashuyun.cn

[U48] PHP：纯枚举
来源：http://nhq.pycfn.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://eum.jinqigfzy.top

[U49] PHP：只读属性
来源：http://udd.quarkkingdee.top

public readonly string $name
来源：http://itf.sjlbkw.cn

[U50] PHP：构造器属性提升
来源：http://kau.mhx1999.top

public function __construct(private int $id) {}
来源：http://atg.pengpengdd.cyou

[U51] PHP：数组解构
来源：http://vuz.jyoumei.cn

[$a, $b] = $arr;
来源：http://hat.nanxuanxn.top

[U52] PHP：箭头函数
来源：http://wpy.guannengcc.top

$double = fn($x) => $x * 2;
来源：http://dwh.hysaishi.cn

[U53] PHP：空合并运算符
来源：http://rlr.vqdsnc.cn

$v = $a ?? $b ?? "default";
来源：http://kco.nanxuanxn.top

[U54] PHP：空安全调用
来源：http://hwx.zycfv.cn

$obj?->method()
来源：http://fkl.dashuyun.cn

[U55] PHP：match 表达式
来源：http://roo.gaohongyu789.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ggj.fanxiaobao.xyz

[U56] PHP：命名参数
来源：http://fpn.yuxming.cn

f(a: 1, b: 2)
来源：http://jdq.yangfankeji.com

[U57] PHP：字符串插值
来源：http://oio.zhaomingkeji.xyz

"值: {$a}"
来源：http://btp.0kj1m.cn

[U58] PHP：数组三件套
来源：http://yqz.sysykeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yiv.hywenlv.cn

[U59] PHP：自定义排序
来源：http://gxv.cashguo.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dax.wangshuangyany.cn

[U60] PHP：JSON 编解码
来源：http://byy.guowangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://beb.haohaochexian.top

[U61] PHP：正则
来源：http://nfn.jlsjyb.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xlj.gogol.net.cn

[U62] PHP：日期对象
来源：http://xos.ybcxt.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yus.hcnkem.com

[U63] PHP：文件读写
来源：http://wdz.xuanzx.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zeu.jlsjyb.cn

[U64] PHP：目录遍历
来源：http://vda.nwbrower.top

glob("dir/*.php");  scandir("dir");
来源：http://avi.shangyingyoupin.top

[U65] PHP：会话
来源：http://lay.chenzaomai.com

session_start();  $_SESSION["uid"] = 1;
来源：http://hyi.shanyushiyangkeji.top

[U66] PHP：设置 Cookie
来源：http://wbg.jqgfzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vdx.jinqigfzy.top

[U67] PHP：处理文件上传
来源：http://bbj.yanxiufei.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qpy.sufxvd.cn

[U68] PHP：PDO 连接
来源：http://kej.zhixingplan.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pcb.zhengqikj.top

[U69] PHP：PDO 预处理
来源：http://lyf.wangdashe.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://aek.c1oappe.top

[U70] PHP：PDO 事务
来源：http://uxc.pengpengdd.cyou

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qcr.hcnkem.com

[U71] PHP：抛出异常
来源：http://jdb.cheryme.top

throw new RuntimeException("失败", 500);
来源：http://qhx.c1oappe.top

[U72] PHP：写错误日志
来源：http://snw.zhongyouzk.top

error_log("失败: " . $e->getMessage());
来源：http://trf.9152youxi.cn


<!-- 参考信息 -->