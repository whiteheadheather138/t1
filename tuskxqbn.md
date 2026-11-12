代发 wailian999

[S43] C++：智能指针
来源：http://yqi.vqdsnc.cn

auto p = std::make_unique<int>(5);
来源：http://pul.dashuyun.cn

[S44] C++：引用传参
来源：http://yec.xinyue.icu

void inc(int &x) { ++x; }
来源：http://xng.yueranfly.top

[S45] C++：lambda
来源：http://xym.hysaishi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://evz.ctjpmb.com

[S46] C++：函数模板
来源：http://vux.wangshuangyany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gzr.vqdsnc.cn

[S47] C++：结构化绑定遍历
来源：http://tfc.tian-w.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qbm.gogol.net.cn

[S48] C++：逐行读文件
来源：http://jop.yj20258.top

std::ifstream in("a.txt");  std::string line;
来源：http://god.jianghu66.top

while (std::getline(in, line)) { }
来源：http://eqg.guannengcc.top

[S49] C++：写文件
来源：http://aig.jinyuanbaomall.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vnh.snrcjt.cn

[S50] C++：格式化数字
来源：http://lsy.jinghuilouyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zya.hongshengwenyu.top

[S51] C++：显式类型转换
来源：http://brz.tianlin.xyz

static_cast<double>(a) / b
来源：http://ovt.gaohongyu789.top

[S52] C++：const 与 noexcept
来源：http://syb.zdqjudy.top

int size() const noexcept { return n_; }
来源：http://wyc.bbcook.cn

[S53] C++：移动语义
来源：http://wde.zycfv.cn

std::vector<int> w = std::move(v);
来源：http://jfw.kuanghao11.cn

[S54] C++：异常处理
来源：http://tke.quarkkingdee.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pes.zycfv.cn

[S55] C++：结构化绑定
来源：http://fwp.c1oappe.top

auto [a, b] = std::make_pair(1, 2);
来源：http://eir.bjfxy.top

[S56] C++：optional
来源：http://kzw.zhaomingkeji.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jyi.gaohongyu789.top

[S57] C++：编译期常量
来源：http://idp.tianlin.xyz

constexpr int N = 10;
来源：http://udw.sweek.top

[S58] C++：命名空间
来源：http://plh.haohaochexian.top

namespace ns { int f() { return 1; } }
来源：http://rwh.yj20258.top

[S59] C++：静态断言
来源：http://fzu.hcnkem.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lvx.jyoumei.cn

[S60] C++：遍历并删除元素
来源：http://rjv.nanxuanxn.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lwk.ehwqpu.com

================================================================================
来源：http://dkz.zhijiandao.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://end.aizwys.cn

================================================================================
来源：http://zop.daria6918.cn

[T01] Kotlin：Hello World
来源：http://xgx.ehwqpu.com

println("Hello")
来源：http://lmz.zhengqikj.top

[T02] Kotlin：变量
来源：http://ifk.mhx1999.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lvu.xinyue.icu

[T03] Kotlin：字符串模板
来源：http://rpu.9152youxi.cn

"值: $b"
来源：http://xzk.shanyushiyangtech.top

[T04] Kotlin：空安全
来源：http://lft.cqqwz.cn

val n: String? = null;  n?.length
来源：http://tul.smart0.xyz

[T05] Kotlin：when 表达式
来源：http://mol.yuanzhike.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oby.zhongyouzk.top

[T06] Kotlin：集合映射
来源：http://uhg.daxiang520.top

listOf(1, 2, 3).map { it * 2 }
来源：http://emv.pycfn.com

[T07] Kotlin：集合过滤
来源：http://blg.haohaochexian.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ghj.jlsjyb.cn

[T08] Kotlin：数据类
来源：http://aqw.shuidangran.top

data class User(val name: String, val age: Int)
来源：http://uza.ydjk.org.cn

[T09] Kotlin：扩展函数
来源：http://gzh.cheryme.top

fun String.exclaim() = this + "!"
来源：http://vzg.tian-w.cn

[T10] Kotlin：默认参数
来源：http://jqs.vehdjk.com

fun greet(name: String = "World") = "Hi $name"
来源：http://ifu.shangyingyoupin.top

[T11] Kotlin：协程
来源：http://rct.aibaodan.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jpj.hesvh.cn

[T12] Kotlin：解构声明
来源：http://tur.cucudq.cn

val (a, b) = Pair(1, 2)
来源：http://fik.gzhubu.top

[T13] Kotlin：只读 Map
来源：http://jod.jianghu66.top

val m = mapOf("a" to 1)
来源：http://pyo.chenlongwang.top

[T14] Kotlin：循环
来源：http://ghv.zhixingplan.top

for (i in 1..10) println(i)
来源：http://clo.iojbl.cn

[T15] Kotlin：接口
来源：http://pxt.feifeiyinyue.top

interface Shape { fun area(): Double }
来源：http://awy.316326.xyz

[T16] Swift：Hello World
来源：http://dal.cdnleiting.top

print("Hello")
来源：http://kpf.cucudq.cn

[T17] Swift：变量与常量
来源：http://brb.fktsv.cn

var a = 1;  let b = 2
来源：http://xik.chenlongwang.top

[T18] Swift：字符串插值
来源：http://ixa.shanyushiyangkeji.top

"值: \(b)"
来源：http://xyf.andypj.xyz

[T19] Swift：可选绑定
来源：http://yim.ywan-chungtsiang.top

if let n = opt { print(n) }
来源：http://bsd.xuanzx.com

[T20] Swift：数组操作
来源：http://qux.chenlongwang.top

var a = [1, 2, 3];  a.append(4)
来源：http://yih.zhongyouzk.top

[T21] Swift：遍历
来源：http://jib.shanyushiyangtech.top

for x in a { print(x) }
来源：http://yqh.sweek.top

[T22] Swift：字典
来源：http://zmq.yueranfly.top

var d = ["a": 1];  d["b"] = 2
来源：http://fxt.xuetiantiany.cn

[T23] Swift：函数
来源：http://xtw.andypj.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sxk.hnqzz.top

[T24] Swift：闭包
来源：http://tzt.zhengqikj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ilh.yj20258.top

[T25] Swift：结构体
来源：http://ydy.xinyue.icu

struct P { var x: Int }
来源：http://tus.meibo888.top

[T26] Swift：类与重写
来源：http://uop.kuanghao11.cn

class A: Base { override func f() {} }
来源：http://igd.pengpengdd.cyou

[T27] Swift：错误处理
来源：http://bee.jianghu66.top

do { try f() } catch { print(error) }
来源：http://aba.gzhubu.top

[T28] Swift：枚举
来源：http://byn.zhaomingkeji.xyz

enum Color { case red, green }
来源：http://ywn.zhaomingkeji.xyz

[T29] Swift：guard 提前返回
来源：http://fzy.sweek.top

guard let x = opt else { return }
来源：http://vzt.tanke756.top

[T30] Swift：协议
来源：http://dvh.yj202588.top

protocol Shape { func area() -> Double }
来源：http://yzd.wangshuangyany.cn

[T31] Lua：Hello World
来源：http://zca.ppjwa.cn

print("Hello")
来源：http://smu.tanke756.top

[T32] Lua：局部变量
来源：http://cug.316326.xyz

local a = 1
来源：http://blu.mhx1999.top

[T33] Lua：表（数组）
来源：http://mjm.zhengqikj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vmw.daria6918.cn

[T34] Lua：遍历表
来源：http://qac.yuanzhike.top

for i, v in ipairs(t) do print(i, v) end
来源：http://man.ybcxt.top

[T35] Lua：字典表
来源：http://opx.tian-w.cn

local d = { a = 1 };  d.b = 2
来源：http://goz.yvedp.cn

[T36] Lua：函数
来源：http://ull.xylfe.cn

function add(a, b) return a + b end
来源：http://aix.wangdashe.top

[T37] Lua：字符串拼接
来源：http://szm.jinqigfzy.top

"a" .. "b"
来源：http://dwc.zdbjq.cn

[T38] Lua：条件
来源：http://fcx.shzxlz.cn

if x > 0 then print("正") end
来源：http://vvf.quarkkingdee.top

[T39] Lua：模式匹配
来源：http://vpq.fzhhl.top

string.find(s, "%d+")
来源：http://fjy.haohaochexian.top

[T40] Lua：元表
来源：http://dqc.vehdjk.com

setmetatable({}, { __index = base })
来源：http://rnr.fengsongda.top

[T41] Perl：Hello World
来源：http://qsc.vqdsnc.cn

print "Hello\n";
来源：http://jwu.zhiwuduotai.top

[T42] Perl：变量类型
来源：http://mxl.gzhubu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xxf.yj20258.top

[T43] Perl：字符串插值
来源：http://nnl.meibo888.top

"值: $a"
来源：http://quk.cashguo.top

[T44] Perl：条件
来源：http://seh.ywan-chungtsiang.top

if ($a > 0) { print "正"; }
来源：http://tjw.jinyuanbaomall.cn

[T45] Perl：数组遍历
来源：http://vic.ydzc1.top

for my $x (@arr) { print $x; }
来源：http://avc.cheryme.top

[T46] Perl：哈希操作
来源：http://quj.nwbrower.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jzf.cucudq.cn

[T47] Perl：正则捕获
来源：http://bkc.sxryk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xsa.chenjidiqi.icu

[T48] Perl：正则替换
来源：http://yrq.0kj1m.cn

$s =~ s/old/new/g;
来源：http://bwx.gaohongyu789.top

[T49] Perl：函数
来源：http://vnk.zhengqikj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eyu.chenzaomai.com

[T50] Perl：逐行读文件
来源：http://rku.shzxlz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cfe.xuanzx.com

while (my $line = <$fh>) { print $line; }
来源：http://zjj.jinghuilouyu.cn

[T51] Scala：Hello World
来源：http://hzr.vehdjk.com

println("Hello")
来源：http://fvs.hnxiangtu.top

[T52] Scala：变量
来源：http://fhe.nwbrower.top

val a = 1;  var b = 2
来源：http://eko.aibaodan.cn

[T53] Scala：字符串插值
来源：http://znw.hesvh.cn

s"值: $b"
来源：http://brj.fengsongda.top

[T54] Scala：集合映射
来源：http://nef.quarkkingdee.top

List(1, 2, 3).map(_ * 2)
来源：http://zvb.vqdsnc.cn

[T55] Scala：集合过滤
来源：http://ckx.gogol.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://shm.wangshuangyany.cn

[T56] Scala：样例类
来源：http://ggx.jinyuanbaomall.cn

case class User(name: String, age: Int)
来源：http://lfm.zdqjudy.top

[T57] Scala：模式匹配
来源：http://bbc.fengsongda.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://npt.hesvh.cn

[T58] Scala：函数定义
来源：http://snk.meibo888.top

def add(a: Int, b: Int): Int = a + b
来源：http://gdf.fanxiaobao.xyz

[T59] Scala：循环
来源：http://uuo.mhx1999.top

for (i <- 1 to 10) println(i)
来源：http://nil.vehdjk.com

[T60] Scala：折叠
来源：http://szi.jinyuanbaomall.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qxp.chenlongwang.top

================================================================================
来源：http://njx.yvedp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fkj.havefunace.top

================================================================================
来源：http://sbu.tianlin.xyz

[U01] Py：创建虚拟环境
来源：http://wkl.iojbl.cn

python -m venv .venv && source .venv/bin/activate
来源：http://svg.c1oappe.top

[U02] Py：导出 / 安装依赖
来源：http://ixp.yj20258888.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qye.shuidangran.top

[U03] Py：加载 .env 配置
来源：http://nka.jiagoushi.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ica.52xcode.cn

[U04] Py：变量调试打印
来源：http://rwu.xuetiantiany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://aft.yfazqb.com

[U05] Py：列表去重且保序
来源：http://cee.chenlongwang.top

list(dict.fromkeys(arr))
来源：http://szj.yueranfly.top

[U06] Py：合并两个字典
来源：http://iyo.sweek.top

{**a, **b}
来源：http://ano.gotoacloud.top

[U07] Py：反转字典键值
来源：http://unq.hesvh.cn

{v: k for k, v in d.items()}
来源：http://jgg.jyoumei.cn

[U08] Py：展平二维列表
来源：http://ruo.nanxuanxn.top

[y for x in nested for y in x]
来源：http://gjc.smart0.xyz

[U09] Py：字典取最大值的键
来源：http://arx.c1oappe.top

max(d, key=d.get)
来源：http://ckh.sysykeji.top

[U10] Py：按值排序字典
来源：http://tfx.gzhubu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oyz.jianghu66.top

[U11] Py：生成器表达式
来源：http://aim.cdnleiting.top

(x * 2 for x in arr)
来源：http://awu.chenjidiqi.icu

[U12] Py：取出现最多的 3 个元素
来源：http://kym.zhixingplan.top

Counter(arr).most_common(3)
来源：http://wfh.hammf.cn

[U13] Py：固定长度队列
来源：http://oci.shanyushiyangtech.top

deque(maxlen=10)
来源：http://deq.zhixingplan.top

[U14] Py：分组收集到列表
来源：http://xoa.zhixingplan.top

defaultdict(list)
来源：http://fip.nanxinkj.top

[U15] Py：高精度计时
来源：http://kjx.fengsongda.top

t = time.perf_counter()
来源：http://vcj.dianchejie.cn

[U16] Py：命令行参数解析
来源：http://tfj.chenzaomai.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dky.yj20258.top

[U17] Py：初始化日志
来源：http://cnb.sufxvd.cn

logging.basicConfig(level=logging.INFO)
来源：http://irv.tanke756.top

[U18] Py：预编译正则
来源：http://uvp.zhongyouzk.top

pat = re.compile(r"\d+")
来源：http://okb.iojbl.cn

[U19] Py：正则替换带回调
来源：http://gml.andypj.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hal.yj20258888.top

[U20] Py：缓存函数结果
来源：http://qhh.jqgufenzy.top

@functools.lru_cache(maxsize=None)
来源：http://qja.redwolf501.top

[U21] Py：自定义上下文管理器
来源：http://ucv.zhengqikj.top

@contextlib.contextmanager
来源：http://hva.yvedp.cn

[U22] Py：矩阵转置
来源：http://enh.ydjk.org.cn

list(zip(*m))
来源：http://dcr.yvedp.cn

[U23] Py：分块读取大文件
来源：http://qqt.bjfxy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wqk.tanke756.top

[U24] Py：路径操作
来源：http://acd.shangyingyoupin.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uxy.gotoacloud.top

[U25] Py：CSV 按字典读
来源：http://kbw.gotoacloud.top

csv.DictReader(f)
来源：http://jod.sufxvd.cn

[U26] Py：并发下载
来源：http://eia.zdqjudy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ghu.yuxming.cn

[U27] Py：异步 HTTP
来源：http://cub.hysaishi.cn

aiohttp.ClientSession() 配合 async with
来源：http://ibs.dashuyun.cn

[U28] Py：类型别名
来源：http://nvy.316326.xyz

UserId = int
来源：http://end.fengsongda.top

[U29] Py：属性校验
来源：http://bco.zhijiandao.cn

@property 与 @x.setter 配合
来源：http://omd.zdqjudy.top

[U30] Py：数据类
来源：http://epr.birdmap.top

@dataclass(slots=True)
来源：http://iod.wangdashe.top

[U31] Py：单测
来源：http://lxl.yuanzhike.top

python -m pytest -q
来源：http://moy.chenlongwang.top

[U32] Py：代码格式化
来源：http://kxn.wangdashe.top

ruff format . && ruff check --fix .
来源：http://enz.svipenyu.cn

[U33] Py：打包发布
来源：http://jcs.jiagoushi.top

python -m build  （依赖 pyproject.toml）
来源：http://yyj.jyoumei.cn

[U34] Py：判断编码
来源：http://grr.xuetiantiany.cn

chardet.detect(raw)
来源：http://osg.hesvh.cn

[U35] Py：发送邮件
来源：http://itz.svipenyu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uta.daria6918.cn

[U36] Py：定时任务
来源：http://cnx.iojbl.cn

schedule.every(10).minutes.do(job)
来源：http://taj.quarkkingdee.top

[U37] Py：读写 Excel
来源：http://rpw.guannengcc.top

pandas.read_excel / DataFrame.to_excel
来源：http://yzv.gaohongyu789.top

[U38] Py：获取脚本所在目录
来源：http://giy.shanyushiyangtech.top

Path(__file__).resolve().parent
来源：http://mzc.316326.xyz

[U39] Py：判断是否在交互环境
来源：http://wey.daria6918.cn

sys.stdout.isatty()
来源：http://von.zdbjq.cn

[U40] Py：打印到标准错误
来源：http://jsg.hysaishi.cn

print("err", file=sys.stderr)
来源：http://vxy.ctjpmb.com

[U41] PHP：初始化 Composer 项目
来源：http://apv.cucudq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tch.andypj.xyz

[U42] PHP：PSR-4 自动加载
来源：http://hah.sxryk.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jmj.shuidangran.top

[U43] PHP：声明命名空间
来源：http://yea.andypj.xyz

namespace App\Http;
来源：http://zur.redwolf501.top

[U44] PHP：开启严格类型
来源：http://drn.smart0.xyz

declare(strict_types=1);
来源：http://xjy.uphjek.com

[U45] PHP：类型声明与返回类型
来源：http://ejo.sxryk.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://reb.wangshuangyany.cn

[U46] PHP：可空类型
来源：http://zkt.sweek.top

?string $name = null
来源：http://jxp.hesvh.cn

[U47] PHP：联合类型
来源：http://bef.chenzaomai.com

int|string $id
来源：http://oqp.shzxlz.cn

[U48] PHP：纯枚举
来源：http://stn.ywan-chungtsiang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xvm.snrcjt.cn

[U49] PHP：只读属性
来源：http://whf.yfazqb.com

public readonly string $name
来源：http://ats.chenzaomai.com

[U50] PHP：构造器属性提升
来源：http://wjs.yueranfly.top

public function __construct(private int $id) {}
来源：http://eks.sxryk.cn

[U51] PHP：数组解构
来源：http://gww.yfazqb.com

[$a, $b] = $arr;
来源：http://lrw.316326.xyz

[U52] PHP：箭头函数
来源：http://cpz.cashguo.top

$double = fn($x) => $x * 2;
来源：http://bnm.xuetiantiany.cn

[U53] PHP：空合并运算符
来源：http://wlz.smart0.xyz

$v = $a ?? $b ?? "default";
来源：http://qmg.9152youxi.cn

[U54] PHP：空安全调用
来源：http://qqj.shangyingyoupin.top

$obj?->method()
来源：http://aym.mhx1999.top

[U55] PHP：match 表达式
来源：http://ndu.smart0.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cxr.zhoulong.xyz

[U56] PHP：命名参数
来源：http://tda.cucudq.cn

f(a: 1, b: 2)
来源：http://kzj.yj202588.top

[U57] PHP：字符串插值
来源：http://ekc.yonumen.top

"值: {$a}"
来源：http://kcp.jyoumei.cn

[U58] PHP：数组三件套
来源：http://zhc.fehbvm.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://eid.dianchejie.cn

[U59] PHP：自定义排序
来源：http://cxh.tianlin.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ozw.sxryk.cn

[U60] PHP：JSON 编解码
来源：http://kbm.havefunace.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oxk.zhixingplan.top

[U61] PHP：正则
来源：http://wbr.zhaomingkeji.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zhw.pycfn.com

[U62] PHP：日期对象
来源：http://mbr.zhoulong.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dtk.nwbrower.top

[U63] PHP：文件读写
来源：http://jhl.ywan-chungtsiang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hng.yonumen.top

[U64] PHP：目录遍历
来源：http://ahl.guowangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://jim.ppjwa.cn

[U65] PHP：会话
来源：http://feg.shanyushiyangtech.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ief.vehdjk.com

[U66] PHP：设置 Cookie
来源：http://zoh.zhiwuduotai.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cty.ydzc1.top

[U67] PHP：处理文件上传
来源：http://wlk.aibaodan.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xhq.zhixingplan.top

[U68] PHP：PDO 连接
来源：http://gpp.xziqi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kwn.xingfuxueyuan.xyz


<!-- 参考信息 -->